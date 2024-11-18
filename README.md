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

| 𝐴 | 𝐵 | 𝐂 | `𝑃`<sub>`(𝐴,𝐵,𝐂)`</sub> |
|:-:|:-:|:-:|:--------:|
| 0 | 0 | 0 | ![¬𝐴∧¬𝐶∧¬𝐵](https://img.shields.io/badge/1-yellow?style=for-the-badge)   |
| $\color{grey}{0}$ | $\color{grey}{0}$ |$\color{grey}{1}$ |    ![Static Badge](https://img.shields.io/badge/0-black?style=for-the-badge)    |
| 0 |`1`| 0 | ![1](https://img.shields.io/badge/1-darklime?style=for-the-badge)  |
| 0 |`1`|`1`| ![¬𝐴∧𝐵∧𝐶](https://img.shields.io/badge/1-royalblue?style=for-the-badge)  |
|`1`| $\color{grey}{0}$ | $\color{grey}{0}$ |   ![Static Badge](https://img.shields.io/badge/0-black?style=for-the-badge)     |
> ###### *..hier könnten weitere Zeilen stehen..*

### <p align="left">🅱️</p>
|    | AB | A¬B | ¬A¬B | ¬AB |
|:--:|:--:|:---:|:----:|:---:|
|  C | $\color{gray}{0}$ | $\color{gray}{0}$ | $\color{gray}{0}$ | $\color{royalblue}{1}$ |
| ¬C | $\color{gray}{0}$ | $\color{gray}{0}$ | $\color{yellow}{1}$ | $\color{lime}{1}$ |   

> ### <p align="left">***Ergebnis*** :</p>
> ##  `𝑃`<sub>`(𝐴,𝐵,𝐂)`</sub> ≡ ($\color{yellow}{¬A∧¬C}$) ∨ ($\color{royalblue}{¬A∧B}$)
> ##### *<p align="right"> Quot erat demonstrandum. </p>*
 
 --- 
</div></div>

<!-- - - - - - - - - - - - - exercise #2 - - - - - - - - - - - - -->
<div style="page-break-before: always;">

# <p align="left"> 2 ) <sub> [ `4` Variables ] </sub> 
### 🅰️ </p>  
<div align="center">

| 𝐴 | 𝐵 | 𝐂 | 𝐃 | `𝑃`<sub>`(𝐴,𝐵,𝐂,𝐃)`</sub> |
|:-:|:-:|:-:|:-:|:----------:|
|`1`| 0 | 0 | 0 |     ![`1`](https://img.shields.io/badge/1-royalblue?style=for-the-badge)    |
| $\color{grey}{0}$ |`1`|`1`|`1`|![Static Badge](https://img.shields.io/badge/0-black?style=for-the-badge)    |
|`1`|`1`| 0 |`1`|     ![`1`](https://img.shields.io/badge/1-darklime?style=for-the-badge)    |
| 0 |`1`| 0 |`1`|     ![`1`](https://img.shields.io/badge/1-yellow?style=for-the-badge)    |
|`1`|`1`| 0 | 0 |      ![`1`](https://img.shields.io/badge/1-royalblue?style=for-the-badge)    |
|`1`| $\color{grey}{0}$ |`1`| $\color{grey}{0}$ |![Static Badge](https://img.shields.io/badge/0-black?style=for-the-badge)|
|`1`| 0 | 0 |`1`|     ![`1`](https://img.shields.io/badge/1-darklime?style=for-the-badge)    |
> ###### *..hier könnten weitere Zeilen stehen..*

### <p align="left">🅱️</p>
|      | ¬AB | AB | A¬B | ¬A¬B |
|:----:|:---:|:--:|:---:|:----:|
|   CD |  $\color{gray}{0}$  |   $\color{gray}{0}$    |   $\color{gray}{0}$    | $\color{gray}{0}$ |
|  C¬D |  $\color{gray}{0}$  |   $\color{gray}{0}$    |   $\color{gray}{0}$    | $\color{gray}{0}$ |
| ¬C¬D |  $\color{gray}{0}$  | $\color{royalblue}{1}$ | $\color{royalblue}{1}$ | $\color{gray}{0}$ |
|  ¬CD | $\color{yellow}{1}$ |    $\color{lime}{1}$   |    $\color{lime}{1}$   | $\color{gray}{0}$ | 

> ### <p align="left">***Ergebnis*** :</p>
> ##  `𝑃`<sub>`(𝐴,𝐵,𝐂,𝐃)`</sub> ≡ ($\color{royalblue}{A∧¬𝐂}$) ∨ ($\color{yellow}{¬𝐂∧𝐃}$)
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
