---
type: note
alias: Op-Amp
---
01/12/2023 09:34

  #Circuit_Analysis 

The operational amplifier is a non-linear circuit device that has a variety of uses. For ideal calculations around the op-amp, the input [[Impedance]] at the input terminals is infinite, therefore there is no input [[Current]]. the ideal op-amp is also drawn without the supply terminals, which limit the voltage of the output to their applied voltage.

![[Op-amp_symbol.svg.png]]

Pin out:
- $V^+$ = non-inverting input
- $V^-$ = inverting input
- $V_{S+}$ = positive supply [[Voltage]] (rail)
- $V_{S-}$ = negative supply

The function of an op-amp can be described with a formula:
$$
V_{out}=A_{OD}(V^+-V^-)
$$
where $A_{OD}$ is the open loop difference gain, or gain with no feedback connections, which is often very large ($\ge10^5$). 

>[!note]
>An op-amp drawn without the supply terminals is the symbol for an ideal op amp, whose ouput is unlimited

## No Feedback
An op-amp without any feedback, but with a DC source at its inverting input and a sinusoidal [[Alternating Current|AC]] source at the non-inverting input will produce a square wave at its output. If $V_{DC}\ne0$, the duty cycle will be changed. If $V_{DC}>0$, the negative portion of the output wave will be longer, if less than 0, the positive portion will be longer.

![[Pasted image 20230208194750.png]]


---

## Feedback Design
In a feedback design, the output of the op-amp is connected to one of its input terminals, usually through a resistor.


### Negative Feedback
A negative feedback design would have $V_{out}$ connected to $V^-$ through a [[Resistance|Resistor]].


>[!info]
>In a negative feedback configuration, the summing point constraint applies:
>$$\begin{align*}
V^+-V^-&=0\\
V^+&=V^-
\end{align*}$$

#### Inverting Op-Amp
The inverting op-amp is a feedback design where the output is connected to the inverting input. The output of this amplifier will be $180^\circ$ out of [[Phase Angle|Phase]] with the input, hence its name.

![[Pasted image 20230113134210.png]]

Applying circuit anaylsis techniques and the above summing point constraint, the output voltage may be found:
$$
V_{out}=-\left(\frac{R_F}{R_1}\right)V_{in}
$$
where the voltage gain $A_V=-\frac{R_F}{R_1}$ 

##### Inverting Summing Amp
When two or more voltages inputs are present at the inverting input, the op-amp is known as an inverting summing amplifier. 

![[Pasted image 20230117135501.png]]

When the input resistances are the same for each voltage, the voltages simply add to form $V_{in}$:
$$
V_{out}=-\frac{R_F}{R_1}\left(V_1+V_2\right)
$$

When the resistances are not the same, the following formula is used for $n$ voltage inputs:
$$
V_{out}=-R_{F}\left(\frac{V_1}{R_{1}}+ \frac{V_2}{R_{2}}+\cdots+ \frac{V_n}{R_{n}}\right)
$$

---

#### Non-Inverting Op-Amp
Unlike the inverting op-amp, this design does not change the phase of the input signal. That is, the output and input signals will be in phase with each other. This is achieved by connecting the source to the non-inverting input: 

![[Pasted image 20230113134621.png]]

For this design:
$$
V_{out}=\left(1+ \frac{R_F}{R_1}\right)V_{in}
$$
where the voltage gain $A_V=\left(1+ \frac{R_F}{R_1}\right)$ 

---

#### Difference Amplifier
A difference amplifier is so called because its output voltage is a multiple of the difference between the voltages at its input terminals. An op-amp with no feedback is a difference amplifier, but its gain will be the open loop difference gain. To have a controlled gain, a feedback design must be used:

![[Pasted image 20230124095430.png]]

In the ideal scenario of:
$$
\frac{R_2}{R_1}= \frac{R_4}{R_3}
$$
then:
$$
V_{out}= \frac{R_2}{R_1}(V_2-V_1)
$$

Otherwise:
$$
V_{out}=V_{2}\left( \frac{R_{4}}{R_{3}+R_{4}}\right)\left(1+\frac{R_{2}}{R_{1}}\right)-V_1\left(\frac{R_{2}}{R_{1}}\right)
$$


##### Instrumentation Amp Circuit
This circuit has two stages, the first is two inverting op-amps whose outputs are the inputs of the second stage, a difference amplifier:


$$
V_{out}=\left(1+\frac{R_2}{R_1}\right)\left( \frac{R_B}{R_A}\right)(V_{P1}-V_{P2})
$$

---

#### Differentiator
This circuit's output is the derivative of the input, but also acts as an [[Active Filters#1st Order Active High-Pass Filter|Active High-Pass Filter]] 
![[Operational Amplifier 2023-01-24 10.42.08.excalidraw]]

---

#### Integrator
The integrator circuit is the same as a [[Active Filters#1st Order Active Low-Pass Filter|Active Low-Pass Filter]] 
![[Operational Amplifier 2023-01-24 09.46.24.excalidraw]]


---

### Buffer
This configuration has a negative feedback design without a resistor between the output and non-inverting input:

![[Pasted image 20230124103413.png]]

Therefore, $V_{out}=V_{in}$ 

When placed between two passive [[Active Filters]], one high-pass and the other lowpass, the loading effects of connecting them with a wire are mitigated and a bandgap filter is now possible.

---

### Cascaded Op-Amps
Cascaded amps, where the output of one is the input of the other, the output voltage is simply the product of the input and each op-amp's gain. The equation may need modification if one of the amplifiers has more than one input, however.