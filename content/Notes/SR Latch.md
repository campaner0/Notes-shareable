---
type: note
tags: [Digital_Logic]
---
10/12/2022 17:26

  

The SR Latch is a storage circuit comprised of two cross-coupled [[Logical Operators#NOR|NOR]] gates:

![[SR Latch.png]]

This circuit's output is dependent on the previous input. When one input is high, one output is high. When the high input is turned off, the output persists until the previously low input goes high. At this point, the output changes. In this way, data can be stored.

Its truth table is:
$$\begin{array}{c|c|c|c}
S&R&Q&\bar{Q}\\
\hline
0&1&0&1\\
0&0&0&1\\
\hline
1&0&1&0\\
0&0&1&0
\end{array}$$
This circuit has an undefined state where both inputs are high, resulting in both outputs being low, which contradicts the complementary labels of the outputs.

>[!note]
>It is possible to build this circuit using [[Logical Operators#NAND|NAND]] gates, but the truth table will be inverted

---

### D Latch
The D latch prevents the undefined state from happening. It makes it impossible that both inputs will be high by using a data ($D$) and control ($C$) input:

![[D Latch.png]]

In this setup, D inputs to memory and C controls whether the input is stored. It has the truth table:
$$\begin{array}{c|c|c}
C&D&Q\\
\hline
0&X&\text{Previous State}\\
1&0&0\\
1&1&1
\end{array}$$
