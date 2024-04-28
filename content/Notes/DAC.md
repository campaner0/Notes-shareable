---
type: note
aliases:
  - Digital-Analog Converter
---
03/24/2023 13:41

Tags: #Signals 

A DAC, or digital-analog converter, converts digital signals to analog signals. It is the inverse of a [[ADC]], or analog-digital converter. The DAC takes in a digital signal of an arbitrary number of bits. The more bits, the higher the resolution of the output, which is how much the output "steps" up or down when the digital input changes. This is usually given by:
$$
\text{Resolution}=\frac{V_{ref}}{2^n-1}
$$
where
 - $V_{ref}=V_{ref}^+-V_{ref}^-$ = reference [[Voltage]]
 - $n$ = number of input bits

>[!note]
>The reference voltage is usually the highest voltage the DAC can output

### Binary Weighted DAC
A binary weighted DAC uses [[Resistance|Resistor]]s with in ascending value from LSb to MSb. If the LSb has a resistor value of R, each lower bit increases in resistance by $2^{n-k}$, where $n$ is the number of bits and $k$ is the bit that is being calculated. All these are connected to an [[Operational Amplifier|Op-Amp]], which creates an inverting summing amp. This configuration is not often used anymore.


---

### R-2R Ladder DAC
A R-2R Ladder DAC uses an op-amp 

#### Inverting 
$$
V_o=
$$

---

#### Non-Inverting