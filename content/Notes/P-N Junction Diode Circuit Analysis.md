---
type: note
---
01/26/2023 09:33

Tags: #Semiconductor_Devices #Circuit_Analysis 

 The [[P-N Junction Diode]] is a nonlinear circuit element, so its behavior cannot be fully described using linear equatons such as [[Ohm's Law]]. Therefore, a variety of models may be used to describe its behavior under certain circumstances. In circuit diagrams, the diode is represented as below:
 
![[PN Junction Diode 2023-01-26 09.35.31.excalidraw]]

 The anode is on the left and the cathode is on the right such that current flows relativly freely from left to right but flow from right to left is impeded.
 
![[P-N Junction Diode Circuit Analysis 2023-01-31 09.40.25.excalidraw]]

## Ideal Diode Model
While the diode behaves as in its characteristic graph, for the purposes of circuit analysis, the ideal diode model states that the diode can be treated as a wire under forward bias and an open circuit under reverse bias. Therefore current must be greater than 0 under forward and 0 under reverse:

Region | $V_D$ | $I_D$ |Equivalent Function
-----|-----|-----|-----
Forward Bias | $V_D=0$| $I_{D}>0$| Wire/Short
Reverse Bias | $V_D<0$| $I_{D}=0$| Open

where
- $V_D$ = [[Voltage]] across diode
- $I_D$ = [[Current]] through diode

>[!note]
>built in voltage, resistance

---
## Constant Voltage Drop Model
In the constant voltage drop model, the border of the reverse/forward bias regions is set at the diode's built in voltage. The voltage across the diode can less than or equal to the built in voltage. Under forward bias, the diode is treated as a source with voltage $V_{bi}$. Under reverse bias, it is an open circuit.

Region | $V_D$ | $I_D$ | Equivalent Function
-----|-----|-----|-----
Forward Bias | $V_D=V_{bi}$| $I_{D}>0$| Voltage Source w/ value $V_{bi}$
Reverse Bias | $V_D<V_{bi}$| $I_{D}=0$| Open

where
- $V_{bi}$ = built in voltage (see [[P-N Junction Diode]])



---

## Piecewise Linear Model
In this model, $V_{bi}\ne0$ and the diode's internal resistance is nonzero. Under forward bias, the diode is equivalent to a voltage source and resistor in series. Under reverse bias, it is an open circuit.

Region | $V_D$ | $I_D$ | Equivalent Function
-----|-----|-----|-----
Forward Bias | $V_D=V_{bi}+(I_DR_D)$| $I_{D}>0$| Source ($V_{bi}$) and Resistor ($R_D$) in Series
Reverse Bias | $V_D<V_{bi}$| $I_{D}=0$| Open

where
- $R_D$ = internal [[Resistance]] of diode

![[P-N Junction Diode Circuit Analysis 2023-01-31 10.12.18.excalidraw]]