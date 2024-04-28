---
type: note
tags: [Circuit_Analysis]
---
02/16/2023 09:35

  

A [[Voltage]] limiter circuit employs one or two [[P-N Junction Diode|Diode]]s and voltage sources to limit the voltage output to a certain range, even when input voltage changes. With ideal diodes, the voltage will be held at $V_x$ when $V_{in}>V_x$


where
- $V_y=-V_x$

With a piecewise linear model, the voltage outside the range of $V_x$ and $V_y$ has a slope:


where 
- slope outside $V_x$ or $V_y$ = $\frac{r_D}{r_D+R_{1}}$ 