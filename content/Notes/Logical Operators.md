---
type: note
---
08/17/2022 18:07

Tags: #Digital_Logic 

In [[Boolean Algebra]], the following logical operators are commonly used:

### AND
$Z=X\cdot Y$

| x   | y   | z   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 1   |

---

### OR
$Z=X+Y$

|x|y|z|
|-----|------|------|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

---

### NOT
$Z=\bar{X}$ 

|x|z|
|-----|------|
|0|1|
|1|0|

---

### NAND
$Z=\overline{X\cdot Y}$

| x   | y   | z   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 0   | 1   |
| 1   | 1   | 0   |

---

### NOR
$Z=\overline{X+Y}$

|x|y|z|
|-------|-------|------|
|0|0|1|
|0|1|0|
|1|0|0|
|1|1|0|

---

### XOR
$Z=X\bar{Y}+\bar{X}Y=X\oplus Y$

|x|y|z|
|-------|-------|------|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|0|

---

### XNOR
$Z=XY+\overline{XY}=\overline{X\oplus Y}$

|x|y|z|
|-------|-------|------|
|0|0|1|
|0|1|0|
|1|0|0|
|1|1|0|
