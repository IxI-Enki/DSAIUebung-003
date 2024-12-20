<!-- ============================================================================================================ -->
<!--                         made by               Jan Ritt       -       https://github.com/IxI-Enki             -->
<!-- ============================================================================================================ -->

<div style="page-break-before: always;">

# DSAIUebung-003 -- Karnaugh-Veitch Method

- ### <p align="left"> a ) <sub>*Create Truth Tables* </sub></p>  
- ### <p align="left"> b ) <sub> *Optimize the Boolean expression using the Karnaugh-Veitch method* </sub></p>

--- 

<!-- - - - - - - - - - - - - exercise #1 - - - - - - - - - - - - -->
# <p align="left"> 1 ) <sub> [ `3` Variables ] </sub>
### 🅰️ </p>  
<div align="center">

| A | B | C | P(A,B,C) |
|:-:|:-:|:-:|:---------|
| 0 | 0 | 0 |   `1`    |
| 0 | 0 |`1`|    0     |
| 0 |`1`| 0 |   `1`    |
| 0 |`1`|`1`|   `1`    |
|`1`| 0 | 0 |    0     |
> ###### *..hier könnten weitere Zeilen stehen..*

### <p align="left">🅱️</p>
|    | AB | A¬B | ¬A¬B | ¬AB |
|:--:|:--:|:---:|:----:|:---:|
|  C |  0 |  0  |   0  | `1` |
| ¬C |  0 |  0  |  `1` | `1` |   

> ### <p align="left">***Ergebnis*** :</p>
> ##  `𝑃`<sub>`(𝐴,𝐵,𝐂)`</sub> ≡ `(¬A∧¬C) ∨ (¬A∧B)`
> ##### *<p align="right"> Quot erat demonstrandum. </p>*
 
 --- 
</div></div>

<!-- - - - - - - - - - - - - exercise #2 - - - - - - - - - - - - -->
<div style="page-break-before: always;">

# <p align="left"> 2 ) <sub> [ `4` Variables ] </sub> 
### 🅰️ </p>  
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
> ###### *..hier könnten weitere Zeilen stehen..*

### <p align="left">🅱️</p>
|      | ¬AB | AB | A¬B | ¬A¬B |
|:----:|:---:|:--:|:---:|:----:|
|   CD |  0  | 0  |  0  |   0  |
|  C¬D |  0  | 0  |  0  |   0  |
| ¬C¬D |  0  |`1` | `1` |   0  |
|  ¬CD | `1` |`1` | `1` |   0  | 

> ### <p align="left">***Ergebnis*** :</p>
> ##  `𝑃`<sub>`(𝐴,𝐵,𝐂,𝐃)`</sub> ≡ `(A∧¬𝐂) ∨ (¬𝐂∧𝐃)`
> ##### *<p align="right"> Quot erat demonstrandum. </p>*
 
 --- 
</div></div>  

<!-- ============================================================================================================ -->
<!--                         made by               Jan Ritt       -       https://github.com/IxI-Enki             -->
<!-- ============================================================================================================ -->

<!-- fast access to my formating "helper-code" ( 💭 → ✎insert here ): 

// USE THIS TO ENSURE PAGE-BREAKS
//
<div style="page-break-before: always;">
💭
</div>


// USE THIS TO ALIGN CONTENT
//
<p align="left"> 💭 </p>
<div align="center"> 💭 </p>


// USE THIS CENTERED TABLE
//
<div align="center">
  |   |   |   |  
  |:-:|:-:|:-:|  
  |   |   |   |  
</div>


// USE THESE CHARACTERS FOR BEAUTIFUL NOTATIONS
// 
// UNICODE - TABLE of all mathematical operators & symbols:
//     https://en.wikipedia.org/wiki/Mathematical_operators_and_symbols_in_Unicode
//
  ✕ ✖ ⅹ ×  ∓ ∗   ∞   ∧ ⋀ ∨ ⋁   ¬   ≡ 
  ⟹   ⇐ ⇒ ⇔   ← → ↔   ⇽ ⇾ ⇿   ⇠ ⇢   ⇦ ⇨
  ∀  ∃ ∄   ∈ ∋  ∊ ∍
  Ⅰ Ⅱ Ⅲ Ⅳ Ⅴ Ⅵ Ⅶ Ⅷ Ⅸ Ⅹ Ⅺ Ⅻ 
  𝐴 𝐵 𝑃 𝑄
  ∘ ∙ • …   ✓ ✔  ✗ ✘  
  ⚐ ⚡

-->
