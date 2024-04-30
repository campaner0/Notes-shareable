---
type: note
tags: [Digital_Logic]
---
08/31/2022 17:37

  

DeMorgan's theorem is a [[Boolean Algebra]] theorem that states:
$$
\overline{X+Y}=\overline{X}\cdot\overline{Y}
$$
$$
\overline{X\cdot Y}=\overline{X}+\overline{Y}
$$
This may be proven through its truth table:

| X   | Y   | $\overline{X+Y}$ | $\bar{X}\cdot\bar{Y}$ |
| --- | --- | ---------------- | --------------------- |
| 0   | 0   | 1                | 1                     |
| 0   | 1   | 1                | 1                     |
| 1   | 0   | 1                | 1                     |
| 1   | 1   | 0                | 0                     |

