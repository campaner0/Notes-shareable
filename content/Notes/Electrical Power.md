---
type: note
alias: Power
tags: [Circuit_Analysis, Physics]
---
04/22/2022 15:10

 , 

Power is defined as the amount of energy per second expended by a component, or the amount of [[Work]] done by the component. Therefore, if a component releases energy into the circuit its power will be negative, and if it absorbes energy, its power is positive. Its unit is defined as one joule per second or one Watt ($W$).

## DC
Power must be proportional to the amount of charge per second passing through the component and the amount of force needed to move the charge through. Therefore:
$$
P=VI
$$
where
- $P$ = power
- $V$ = [[Voltage]]
- $I$ = [[Current]]

Applying [[Ohm's Law]] gives the following alternate forms for a resistor:
$$\begin{align*}
P=&I^2R\\
=&\frac{V^2}{R}
\end{align*}$$
where
- $R$ = [[Resistance]]

---

## AC
Power in [[Alternating Current]] has an imaginary component in the frequency domain. Since voltage and current are time varying functions, the one component's power is also time varying. Therefore power can only be calculated at an instant or as an average.

#### Instantaneous Power
In sinusoidal steady state, instantaneous power is the product of the sinusoidal voltage and current. Using a trig identity, it can be written as:
$$
p(t)=\frac 12V_mI_m\cos(\theta_V-\theta_I)+\frac 12V_mI_m\cos(2\omega t+\theta_V+\theta_I)
$$
where
- $\theta_V$ = [[Phase Angle]] of voltage
- $\theta_I$ = phase angle of current

---

#### Complex Power
The total power, real and imaginary parts. This is the source power, denoted in Volt-Amps (VA)
$$
S=P+jQ=V_{RMS}I_{RMS}\angle(\theta_V-\theta_I)
$$
where
- $P$ = real/average power
- $Q$ = reactive power

It's magnitude is the apparent power: $\left|S\right| =V_{RMS}I_{RMS}$ 

##### Real power
Also called resistive or average power, the power dissipated by resistors. Measured in watts. This is the power refered to in DC circuits. This can be calculated similarly to DC using RMS values:
$$
P=I_{RMS}^2R=\frac{V_{RMS}^2}R
$$
It can also be found from instantaneous power: the second term is a sinusoidal function so its average is 0, therefore the average is simply the first term, a constant:
$$
P_{avg}=V_{RMS}I_{RMS}\cos(\theta_V-\theta_I)
$$

---

##### Reactive Power
In AC, this is the part denoted in imaginary numbers. Measured in VAR, or Volt Amp Reactive. 
$$
Q=V_{RMS}I_{RMS}\sin(\theta_V-\theta_I)
$$

---

##### Power Factor
Unitless number. It is the ratio of average and apparant power:
$$
PF=\frac P{\left|S\right|}=\cos(\theta_V-\theta_I)
$$
The closer the ratio is to 1, the more efficient the circuit is.

Power factor is either leading or lagging, based on whether the current phasor is in front of or behind the voltage phasor.
- Leading (capacitive): $\theta_V>\theta_I$ 
- Lagging (inductive): $\theta_V<\theta_I$

---

#### Polyphase Power
![[Polyphase Sources#Power]]