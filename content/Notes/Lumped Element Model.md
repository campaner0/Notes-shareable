---
type: note
---
11/11/2022 11:07

Tags: #Electromagnetics 

The lumped element model is a [[Transmission Lines|Transmission Line]] model for any TEM line. It divides the two lines into differential segments of length $\Delta z$, each of which contains elements representing the transmission line parameters:

![[Pasted image 20221111111313.png]]

where the parameters are:
- $R'$ = combined [[Resistance]] of both lines per unit length
- $L'$ = combined [[Inductance]] per unit length
- $G'$ = [[Conductance]] of dielectric separating lines per unit length
- $C'$ = [[Capacitance]] between lines per unit length


These parameters are defined for the certain TEM lines as:

![[Pasted image 20221111112738.png]]

where
- $R_S=\sqrt{\frac{\pi f\mu_c}{\sigma_c}}$ = surface resistance 
	- $\mu_c, \sigma_c$ = permiability, conductivity of conductors
	- $f$ = [[Frequency]]
- $\varepsilon, \mu, \sigma$ = [[Permittivity]], [[Permeability|Permeability]], and [[Conductivity]] of insulator

>[!note]
>For all TEM lines:
>$$\begin{align*}
L'C'&=\mu\varepsilon\\
\frac{G'}{C'}&=\frac{\sigma}{\varepsilon}\\
\end{align*}$$

---

### Telegrapher's Equations
Applying [[Kirchhoff's Voltage Law|Kirchhoff's Voltage]] and [[Kirchhoff's Current Law|Current Laws]] to the model, two differential wave equations for [[Voltage]] and [[Current]] result:
$$\begin{align*}
-\frac{d\widetilde{V}(z)}{dz}&=(R'+j\omega L')\widetilde{I}(z)\\
-\frac{d\widetilde{I}(z)}{dz}&=(G'+j\omega C')\widetilde{V}(z)
\end{align*}$$
These are called the telegrapher's equations, shown in phasor form.