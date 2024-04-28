---
type: note
---
09/21/2022 15:53

  #Circuit_Analysis 

#### Definitions
For a polyphase system, the voltage across two terminals is the line voltage. The line current is the current from a terminal of the source to its corresponding terminal of the load.

The phase voltages are the voltages across the terminals of the source or load to neutral. The phase currents are the currents from one terminal of the load to another. 

---

## Three Phase
### Y-Y

![[Three phase Y-Y circuit.png]]

For a balanced Y-Y source-load connection, assumming no [[Impedance]] in the wires, the voltages across the load terminals are equal to the phase voltages:
$$\begin{align*}
&\vec{V}_{AN}=\vec{V}_{an}\\
&\vec{V}_{BN}=\vec{V}_{bn}\\
&\vec{V}_{CN}=\vec{V}_{cn}\\
\end{align*}$$
where
- $\vec{V}_{AN}=\vec{V}_L$ = load [[Voltage]]
- $\vec{V}_{an}=\vec{V}_\Phi$ = phase voltage

The line voltages are a multiple of the phase voltages:
$$
\vec{V}_{ab}=V_{an}-V_{bn}=V_{an}(\sqrt{3})\angle30^\circ
$$

Since the system is balanced, current for one phase is given by:
$$
I_\Phi=I_L=\frac{V_\Phi}{Z_p}
$$
>[!note]
>In a Y-Y conection, phase current and line current are the same

---

### Y-Delta

![[Three phase Y-Delta circuit.png]]

The line voltages for a Y-$\Delta$ connection are:
$$
\vec{V}_{\Phi}=V_{peak}(\sqrt{3})\angle30^\circ
$$
>[!note]
>In a Y-$\Delta$ connection, Line and Phase voltage are the same


Phase [[Current]]:
$$
\vec{I}_{\Phi}=\frac{\vec{V}_{L}}{\vec{Z}_p}
$$
Line current:
$$
\vec{I}_L=(\sqrt{3}\angle\text{-}30^\circ)\vec{I}_\Phi
$$

---

#### Load Transformation
Balanced three phase loads can be transformed between Y and $\Delta$ configurations by the following relation:
$$
Z_Y=\frac{Z_\Delta}{3}
$$
where
- $Z_Y$ = per phase load impedance in Y config
- $Z_\Delta$ = per phase load impedance in $\Delta$

---

#### Power
For one phase in a three phase system, the average power produced is given by (when using non-RMS values):
$$
P_{phase}=\frac{1}{2}V_{\Phi}I_\Phi\cos(\theta_V-\theta_I)
$$
where
- $V_\Phi$ = phase voltage magnitude
- $I_\Phi$ = phase current magnitude
- $\theta_V$ = voltage [[Phase Angle]]
- $\theta_I$ = current phase angle

>[!note]
When using RMS values, the $\frac{1}{2}$ is removed from the equation.
