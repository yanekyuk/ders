# PHIL 131 - LOGIC

## ‘All’ and ‘Some’

### Symbols and Sentences

### Translation and Symbolization

#### PS

- State whether or not the following are symbolic formula
  - ⋁y( ⋀xHA →  ⋀xIB ) :heavy_check_mark:
  - ⋀yP→P :heavy_check_mark:
  - ⋀AHx→⋀xJx :heavy_multiplication_x:
  - ⋁y( ⋀xKx → ⋀xJx ) :heavy_check_mark:
  - ⋀xEx → (⋁xP → P ) :heavy_multiplication_x:
- Symbolic sentence [closed formulas]: Sym. formulas in which there is no free variable. State whether or not the following are symbolic sentences
  - ⋁y( ⋀xHA∨Hy → ⋀xJx ) :heavy_check_mark:
  - ⋁yP → P  :heavy_check_mark:
  - ⋀x( Ha → ⋀xJx ∨ Gy ) :heavy_multiplication_x: (formula but not sentence)
  - ⋁y( ⋀xKx → Jx )  :heavy_multiplication_x:
  - ⋁xHA → ⋀xJB :heavy_check_mark:
- Translations:
  - *If a woman is married and all married women are wives, then she is a wife.*<br>**F**: a is a woman, **G**: a is married, **H**: a is a wife<br>⋀x( (Fx ∧ Gx) ∧ ⋀y(Fy ∧ Gy→Hy) → Hx )
  - *Mary is a power hungry crafty politician.*<br>**A**: Mary, **F**: a is power hungry, **G**: a is crafty, **H**: a is a politician<br>FA∧GA∧HA
  - (i) *Alfred married an intelligent woman and Rudolf married one too.*<br>(ii) *Alfred married an intelligent woman and Rudolf married her too.*<br>**F**: Alfred married a, **G**: Rudolf married a, **H**: is an intelligent woman<br>(i) ⋁x( Hx ∧ Fx ) ⋁x ( Hx ∧ Gx )<br>(ii) ⋁x ( Hx ∧ Fx ∧ Gx )
  - *Jane cannot solve every question, but it is not the case that she cannot solve any question.*<br>**F**: a is a question, **G**: a can be solved by Jane<br>~⋀x( Fx→Gx ) ∧ ~⋀x( Fx→~Gx )
  - *Something is a fake Rolex watch* here<br>**F**: a is a fake Rolex watch, **G**: a is here<br>⋁x( Fx ∧ Gx )
  - (i) *If anyone is an honest politician, Trump is*<br>(ii) *If everyone is an honest politician, Trump is*<br>**F**: a is an honest politician, **A**: Trump, **G**: a is a person<br>(i) ⋀x( Fx→FA ) == ⋁x( Fx ) → FA<br>(ii) ⋀xFx→FA
  - (i) *If anything can go wrong, something will go wrong*<br>**F**: a can go wrong, **G**: a will go wrong<br>⋀x(Fx→Gx) == ⋁xFx→⋁xGx
- Derivations
  - ⋀xP ∴ P	**UI<sup>x</sup>**
  - ⋁xP ∴ P	**EI<sup>x</sup>**
  - p142 From the formula Fx→Gx, which of formulas are derived from EG
    - ⋁y( Fy→Gy ) :heavy_check_mark: EG<sup>x</sup><sub>y</sub>
    - ⋁y( Fy→Gx ) :heavy_check_mark: EG<sup>x</sup><sub>y</sub>
    - ⋁y( Fx→Gy ) :heavy_check_mark: EG<sup>x</sup><sub>y</sub>
    - ⋁y( Fx→Gx ) :heavy_check_mark: EG<sup>x</sup><sub>y</sub>
    - ⋁x( Fx→Gx ) :heavy_check_mark: EG<sup>x</sup><sub>x</sub>
    - ⋁xFx→Gy :heavy_multiplication_x:
  - FA↔Gx by EG?
    - ⋁x(Fx↔Gx) :heavy_multiplication_x: 
    - ⋁y(Fy↔Gx) :heavy_check_mark: EG<sup>A</sup><sub>y</sub>
    - ⋁x(FA↔Gx) :heavy_check_mark: EG<sup>x</sup><sub>x</sub>
    - FA↔VxGx :heavy_multiplication_x:
  - ⋁x(Fx∧Gy) by EI?
    - Fz∧Gy :heavy_check_mark: EI<sup>x</sup><sub>z</sub>
    - Fy∧Gy :heavy_multiplication_x:
    - FA∧Gy :heavy_multiplication_x:
- Derivation

|      |                         |                              |
| ---- | ----------------------- | ---------------------------- |
| 1    | <s>Show</s> ⋁x(⋁xFx→Fx) | **7,10 ID**                  |
| 2    | \| ~⋁x(⋁xFx→Fx)         | AID                          |
| 3    | \| ⋀x~(⋁xFx→Fx)         | 2 QN                         |
| 4    | \| ~(⋁xFx→Fx)           | 3 UI<sup>x</sup>             |
| 5    | \| ⋁xFx ∧ ~Fx           | 4 NC                         |
| 6    | \| ⋁xFx                 | 5 S                          |
| 7    | \| Fa                   | 6 EI<sup>x</sup><sub>a</sub> |
| 8    | \| ~(⋁xFx→Fa)           | 3 UI<sup>x</sup><sub>a</sub> |
| 9    | \| ⋁xFx ∧ ~Fa           | 8 NC                         |
| 10   | \| ~Fa                  | 9 S                          |

|      |                      |                  |
| ---- | -------------------- | ---------------- |
| 1    | <s>Show</s> ⋁yP↔P    | **8 DD**         |
| 2    | \| <s>Show</s> ⋁yP→P | **3,4 CD**       |
| 3    | \| \| ⋁yP            | ACD              |
| 4    | \| \| P              | 3 EI<sup>y</sup> |
| 5    | \| <s>Show</s> P→⋁yP | **6,7 CD**       |
| 6    | \| \| P              | ACD              |
| 7    | \| \| ⋁yP            | 6 EG<sup>y</sup> |
| 8    | \| ⋁yP↔P             | 2,5 CB           |

