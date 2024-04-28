---
type: note
alias: Synchronous Generator
---
03/14/2023 18:40

Tags: #Electric_Machines 



The induced RMS voltage in the stator is the the same as the induced voltage in an [[AC Motors|AC Motor]] under the same conditions:
$$
V_{A}=\sqrt{2}\pi N_{C}\Phi f
$$
where
- $N_C$ = number of turns
- $\Phi$ = [[Magnetic Flux]]



## Measuring Parameters
To find the synchronous [[Reactance]], armature [[Resistance]], and the relationship between [[Current]] and flux in a generator, an open or short circuit test may be performed. 

#### Open Circuit Test
For this test, the generator is not connected to any load and is turned at its rated speed. The terminal voltage is measured as the field current is increased incrementally. Since the terminals are open, $I_A=0$ so $E_A=V_\phi$

---

#### Short Circuit Test
For a short circuit test, the terminals are shorted. The armature or line current is measured as field current is increased incrementally.

---

## Parallel Operation
Multiple generators can be operated in parallel, and this allows multiple generators to spin up and down for maintenence or failure without disconnecting the load. This also allows the amount of generators to be varied so that the generators are operated near capacity for efficiency. This scheme has several requirements:
1. Line voltages must be equal
2. Phase sequence must be the same
3. Phase angles  of A phase must the same
4. A new generator must have a slightly higher frequency when adding it

---

## Ratings
Synchronous machines are rated based on their intended voltage, frequency, speed, apparant power, power factor, field current, and service factor. 

### Capability Curves
The capability curve of a generator shows its safe nominal operating area on a graph of P vs Q ([[Electrical Power|Power]]). They consist of two circles, one of constant armature current centered at the origin, and another of constant field current centered another point:
$$\begin{array}{c|c}

\end{array}$$

---
## Misc
### Reactive Loads
When a non-reactive load is connected to a generator, the terminal voltage and $V_\phi$ drop slightly. With an inductive (lagging) reactive load, this drop is much greater, and with a capacitive load, the voltage actually increases. Either way is undesireable, and the [[Electrical Power|Power]] factor is ideally close to 1 for efficiency in generation. 