---
type: note
alias: Bipolar Junction Transistor
---
02/28/2023 10:12

  #Circuit_Analysis 

A BJT, or bipolar junction [[Transistor]], has three terminals: collector, base, and emitter. They come in p-type and n-type like [[MOSFET]]s, but have a different construction and behavior. Unlike the MOSFET, the base terminal is connected directly to the junction. This makes it a current controlled current device.

## States of Operation (DC Models)
BJTs consist of two [[P-N Junction]]s arranged in an npn (n-type) or pnp (p-type) format. This results in four possible states:

### Cut-Off
B-E, B-C junctions in reverse bias ($V_{BE}<V_{BE(on)}$ where $V_{BE(on)}$ = base-emitter turn on [[Voltage]]). Transistor equivalent to open.

---

### Forward Active
B-E in forward bias (equivalent to source of $V_{tn}$), B-C in reverse bias (equivalent to dependent current source). Due to how the depletion region [[Electric Field]] expands, most electrons from the emitter flow to the collecter.
$$\begin{align*}
I_C&= \beta I_B\\
I_{E}&= I_{C}+I_{B}=(1+\beta)I_B\\
V_{BE}&= V_{BE(on)}
\end{align*}$$
where
- $\beta$ = [[Current]] gain

To verify:
$$
V_{CE}>V_{CE-sat}
$$

---

### Saturation
B-E, B-C forward biased.
$$\begin{align*}
V_{BE}&= V_{BE(on)}\\
V_{CE}&= V_{CE-sat}\\
I_{E}&= I_{C}+I_{B}\\
V_{CE-sat}&= V_{BE(on)}-V_{BC(on)}
\end{align*}$$

To verify:
$$
\frac{I_{C}}{I_{B}}<\beta
$$


---

### Inverse Active
B-E in reverse bias, B-C in forward. Generally avoided

---
## Q-Point
The Q-point, or DC quiescent point, or bias of the transistor, is the DC voltage part of $V_{CE}$  ($V_{EC}$ for pnp) and the collecter current. It is written in the form of an ordered pair. This point must be in the middle of the forward active region for the most area of uniform gain, but it may be moved if desired. 
$$
\text{Q-Point}=(V_{CE},\,I_{C})
$$

>[!note]
The boundary points on the characteristic plot of the BJT exist in both regions of operation that it borders. Therefore, the equations for both regions are valid at these points.

---

## AC (small signal) Model
In AC analysis, a DC-AC superposistion is used.
1. DC Analysis: All AC sources zeroed, capacitors treated as open
2. AC Analysis: All independent DC sources become zeroed and [[Capacitance|Capacitors]] are treated as a short.

$$\begin{align*}
r_{\pi}&= \beta\frac{V_T}{I_{CQ}}\\[5pt]
g_{m}&= \frac{I_{CQ}}{V_{T}}\\[5pt]
\beta&= r_{\pi}g_m\\[5pt]
i_{c}&= \beta i_b=g_mV_\pi\\[5pt]
r_{o}&= \frac{V_{A}}{I_{CQ}}
\end{align*}$$
where
- $r_\pi$ = base [[Resistance]]
- $V_T$ = thermal voltage
- $I_{CQ}$ = collecter current from Q point
- $g_m$ = transconductance
- $r_o$ = output/internal resistance
- $V_A$ = early voltage

---
bias stable
$$
R_{th}=(R_{1}||R_{2})\cong0.1(1+\beta)R_{E}
$$
load line - kvl on load side of transistor

homework:
find Vth using normal means = 