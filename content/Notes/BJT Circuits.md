---
type: note
---
03/21/2023 09:39

  #Circuit_Analysis 



## Logic Circuits




---

## eeeeee

### Resistor-Like Transistor
When the collector and base of a [[BJT]] are connected with a wire, the transistor is in forward active and behaves like a resistor across the collector and emitter terminals with resistance: 
$$
R= \frac{V_{CE}}{I}
$$
where
- $R$ = [[Resistance]]
- $V_{CE}$ = collector-emitter voltage
- $I$ = current

---

### BJT Amplifier
A BJT can be used as a linear-gain amplifier. The transistor is operated in forward active and can be analyzed using these steps (similar to [[Superposition (Circuit Analysis Technique)|Superposition]]):
1. DC analysis - [[Capacitance|Capacitor]]s open, analyse for Q-point
2. AC analysis - capacitors shorted, independent sources zeroed

#### Common Terminals
Common terminal amplifiers refer to the terminal which is neither input nor output.

##### Common Emitter
Base input, Collector output

Often used as the middle stage of a three-stage amplifier.

##### Common Collector
Base input, Emitter output

- Non-Inverting or Voltage follower, since $A_{v}\le 1$. The output resembles the input very closely 
- $Z_{in}$ - moderate to high
- $Z_{out}$ - very small

Input or output stage of multistage amp.

##### Common Base

- excels at delivering/recieving current

