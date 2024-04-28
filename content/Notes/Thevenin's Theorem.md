---
type: note
---
03/27/2022 19:03

  #Circuit_Analysis 

Thevenin's Theorem states that any linear circuit consisting of only [[Voltage]]/[[Current]] sources and resistors can be reduced to an equivalent circuit of one voltage source $V_{th}$ and one resistor $R_{th}$ in series accross a load [[Resistance]] $R_{load}$.

To find a Thevenin equivalent circuit:
1. Remove load
2. Calculate potential accross load terminals
3. Deactivate sources (voltage becomes short, current becomes open)
4. Calculate resistance between load terminals ($R_{load}$ still removed)

>[!note]
>Maximum power is delivered to a load when $R_{th}=R_{load}$
