<!-- ============================================================================================================ -->
<!--                         made by               Jan Ritt       -       https://github.com/IxI-Enki             -->
<!-- ============================================================================================================ -->

<div style="page-break-before: always;">

# DSAIUebung-003 -- Karnaugh-Veitch Method

## <p align="left"> a ) - Create Truth Tables </p>  
## <p align="left"> b ) - Optimize the Boolean expression using the Karnaugh-Veitch method</p>

--- 

# <p align="left"> 1 ) <sub>[ `3` Variables ]</sub> </p>   

<div align="center">


| A | B | C | P(A,B,C) |
|:-:|:-:|:-:|:---------|
| 0 | 0 | 0 |   `1`    |
| 0 | 0 |`1`|    0     |
| 0 |`1`| 0 |   `1`    |
| 0 |`1`|`1`|   `1`    |
|`1`| 0 | 0 |    0     |
 
<sub><sup> 
--- 
</sup></sub>

|    | AB | A¬B | ¬A¬B | ¬AB |
|:--:|:--:|:---:|:----:|:---:|
|  C |  0 |  0  |   0  | `1` |
| ¬C |  0 |  0  |  `1` | `1` |   

### P(A,B,C) ≡  (¬A∧¬C) ∨ (¬A∧B)
</div>
</div>

---

<div style="page-break-before: always;">


# <p align="left"> 2 ) <sub>[ `4` Variables ]</sub> </p>   
<div align="center">

| A | B | C | D | P(A,B,C,D) |
|:-:|:-:|:-:|:-:|:-----------|
|`1`| 0 | 0 | 0 |     `1`    |
| 0 |`1`|`1`|`1`|      0     |
|`1`|`1`| 0 |`1`|     `1`    |
| 0 |`1`| 0 |`1`|     `1`    |
|`1`|`1`| 0 | 0 |     `1`    |
|`1`| 0 |`1`| 0 |      0     |
|`1`| 0 | 0 |`1`|     `1`    |
 
<sub><sup> 
--- 
</sup></sub>

|      | AB | A¬B | ¬A¬B | ¬AB |
|:----:|:--:|:---:|:----:|:---:|
|   CD | 0  |  0  |   0  |  0  |
|  C¬D | 0  |  0  |   0  |  0  |
| ¬C¬D |`1` | `1` |   0  |  0  |
|  ¬CD |`1` | `1` |   0  | `1` | 

## *P(A,B,C,D) ≡ A¬C ∨ ¬CD*
</div>  
</div>  

--- 



<!-- ============================================================================================================ -->
<!--                         made by               Jan Ritt       -       https://github.com/IxI-Enki             -->
<!-- ============================================================================================================ -->

<!-- fast access to my formating "helper-code" ( 💭 → ✎insert here ): 

// USE THIS TO ENSURE PAGE-BREAKS
<div style="page-break-before: always;">
💭
</div>

// USE THIS TO ALIGN CONTENT
<p align="left"> 💭 </p>
<div align="center"> 💭 </p>

// USE THIS CENTERED TABLE
<div align="center">
  |   |   |   |  
  |:-:|:-:|:-:|  
  |   |   |   |  
</div>

// USE THESE CHARACTERS FOR BEAUTIFUL NOTATIONS
  ✕ ✖ ⅹ ×  ∓ ∗   ∞   ∧ ⋀ ∨ ⋁   ¬   ≡ 
  ⟹   ⇐ ⇒ ⇔   ← → ↔   ⇽ ⇾ ⇿   ⇠ ⇢   ⇦ ⇨
  ∀  ∃ ∄   ∈ ∋  ∊ ∍
  Ⅰ Ⅱ Ⅲ Ⅳ Ⅴ Ⅵ Ⅶ Ⅷ Ⅸ Ⅹ Ⅺ Ⅻ 
  𝐴 𝐵 𝑃 𝑄
  ∘ ∙ • …   ✓ ✔  ✗ ✘  
  ⚐ ⚡
-->
