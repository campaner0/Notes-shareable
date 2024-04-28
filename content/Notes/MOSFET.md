---
type: note
alias: MOSFETs
---
11/09/2022 17:33

  #Semiconductor_Devices #Digital_Logic #Circuit_Analysis 

MOSFETs, or metal oxide semiconductor field effect transistors, are three terminal devices like [[BJT]]s, but, unlike them, only two of the terminals are connected to the semiconductor material. The third is insulated from the silicon by an oxide layer. This third terminal is voltage biased to such that the [[Electric Field]] draws charge carriers from the silicon to the oxide barrier, effectively inverting the type of silicon just under the oxide, which bridges the gap between the other two terminals. This allows current to flow between them.

>[!note]
>Due to the insulator between the gate terminal and the semiconductor body, gate current is negligible, so $I_D=I_S$ 

## N/P-Type
In MOSFETs, n and p-type refer to the silicon where the source and drain attatch, e.g. n-type has n-type at the source and drain and a p-type body. This is inverted for a p-type transistor.

---

## Regions of Operation

### Cut-Off

#### N-Type
No inversion layer under insulator, equivalent to open. $V_{GS}<V_{tn}$  

#### P-Type
Equivalent to open $V_{SG}<|V_{tp}|$

---

### Non-Saturation
Aka linear or triode region.
#### N-Type
$V_{GS}\ge V_{tn}$ 
$$
I_{D} = \frac{k_n'w}{2L}\left[2(V_{GS}-V_{tn})V_{DS}-V_{DS}^2\right]
$$
where
- $I_D$ = drain [[Current]]
- $k_n'$ = [[Transconductance Parameter]]

To verify: $V_{DS}<V_{OV}=V_{GS}-V_{tn}$

#### P-Type
$V_{SG}\ge |V_{tp}|$

To verify: $V_{SD}<V_{OV}=V_{SG}-|V_{tp}|$

---

### Saturation

#### N-Type
$V_{GS}\ge V_{tn}$

$$
I_{D}= \frac{k_n'w}{2L}(V_{GS}-V_{tn})^2(1+\lambda V_{DS})
$$
To verify: $V_{DS}\ge V_{OV}=V_{GS}-V_{tn}$ 

#### P-Type
$V_{SG}\ge |V_{tp}|$

To verify: $V_{SD}\ge V_{OV}=V_{SG}-|V_{tp}|$

>[!note]
>When solving the quadratic in saturation/nonsaturation, choose the answer that supports assumption, if any. Complex values mean assumption is wrong.

---

## Channel Length mod parameter
As $V_{DS}$ becomes larger, the voltage difference between gate and drain decreases. This causes the inversion channel to become thinner on the drain side until it is 1 electron thick. If $V_{DS}$ continues to increase, the inversion channel wedge begins to get smaller. This effect is expressed mathmatically with the channel length modulation parameter:
$$
\lambda=\frac{1}{V_{A}}
$$
where
- $V_A$ = early voltage, similar concept to BJT

This parameter can affect $I_D$ in the right circumstances. 

---

## AC Model

$$\begin{align*}
i_{d}&= g_mV_{gs}\\[5pt]
r_{o}&= \frac{1}{\lambda I_{DQ}}\\[5pt]
g_{m}&= \sqrt{\frac{2k_{n}'w}{LI_{DQ}}}\\[5pt]
&= 2\sqrt{K_nI_{DQ}}\\[5pt]
&= \frac{2I_{DQ}}{V_{OV}}\\[5pt]
&= \frac{2I_{DQ}}{V_{GS}-V_{tn}}\\[5pt]
&= 2K_nV_{OV}\\[5pt]
&= 2K_n(V_{GS}-V_{tn})
\end{align*}$$
where
- $i_d$ = drain current
- $r_o$ = output/internal resistance
- $g_m$ = transconductance
- $I_{DQ}$ = DC drain current
- $K_n$ = transconductance parameter

### Common Amplifier Configurations

#### Common Source
- gate input
- drain output
- very high input [[Impedance]]
- moderate output impedance
- moderate to high voltage gain

---

#### Common Drain
- gate input
- source output
- very high input impedance
- very low output impedance
- close to 1 voltage gain (voltage follower)

---

#### Common Gate
- source input
- drain ouput
- very low input impedance
- very high output impedance
- moderate voltage gain
- close to 1 current gain