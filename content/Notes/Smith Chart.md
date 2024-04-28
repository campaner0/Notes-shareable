---
type: note
---
01/08/2024 16:40

  #Electromagnetics #Antennas

The Smith chart was independently developed by Tosaku Mizuhashi in 1937, Amiel R. Volpert in 1939, and P. H. Smith also in 1939. It is a tool used for RF calculations involving [[Transmission Lines]].

![[2305_C1_EMC_fig1.jpg]]

The chart is a transformed version complex plane such that the boundary separates complex numbers with positive (inside the circle) and negative (outside) real parts. The concentric circles which grow in size to the left represent the real parts ([[Resistance]]) of the normalized load impedance, while the circles which are only partially shown in the chart and which grow in size in the vertical directions represent the imaginary parts ([[Reactance]]). 

$$
z_L=r_L+jx_L
$$

These are shown as circles 




if electrical length = 0.1$\lambda$ 
physical length = $0.1(c/f)$

finding input impedance for certain length transmission line:
1. normalize load impedance and plot
2. draw SWR circle and line through point
3. add length of line to length given by line through load
4. draw line from center to this length on edge
5. intersection with SWR circle is normalized input impedance
