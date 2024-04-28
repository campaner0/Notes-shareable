---
type: note
alias: Transmission Line
---
11/10/2022 21:30

  #Electromagnetics 

Transmission lines that carry an electromagnetic signal connect a generator and load in specific cases of high [[Frequency]] and long lines. In other cases, the system can be modeled with ideal connections, that is, without taking into account the transmission line effects of [[Phase Angle|Phase]] shift, reflected signals, [[Electrical Power|Power]] loss, and dispersion.

---

### Phase Shift
The phase shift of a signal between generator and load for a transmission line is defined as:
$$
\phi_0= \frac{\omega \ell}{c}=2\pi\frac{\ell}{\lambda}
$$
where
- $\omega$ = [[Angular Velocity|Angular Frequency]]
- $\ell$ = length of wire
- $c$ = [[Speed of Light]]
- $\lambda$ = [[Wavelength]]

>[!note]
>When ${\ell}/{\lambda}>0.01$, transmission line effects may need to be taken into account. Below this arbitrary line, they are generally ignored. 

---

### Wave Propagation
By manipulating the telegrapher's equations derived from the [[Lumped Element Model]], two wave equations for [[Voltage]] and [[Current]] in a transmission line result:
$$\begin{align*}
\frac{d^2\widetilde{V}(z)}{dz^2}-\gamma^2\widetilde{V}(z)&=0\\[5pt]
\frac{d^2\widetilde{I}(z)}{dz^2}-\gamma^2\widetilde{I}(z)&=0
\end{align*}$$
where
- $\gamma=\sqrt{(R'+j\omega L')(G'+j\omega C')}$ = [[Propagation Constant]]
- $z$ = [[Distance]] from load
- $\widetilde{V}(z)$ = [[Voltage]] wave
- $\widetilde{I}(z)$ = [[Current]] wave

These equations have travelling wave solutions of the form: 
$$\begin{align*}
\widetilde{V}(z)&= V_0^+e^{-\gamma z}+V_0^-e^{\gamma z}\\[5pt]
\widetilde{I}(z)&= I_0^+e^{-\gamma z}+I_0^-e^{\gamma z}
\end{align*}$$where 
- $V_0^+$ = amplitude of Incident wave, or voltage wave propagating in $+z$ direction
- $V_0^-$ =  amplitude of reflected wave, or voltage wave propagating in $-z$ direction

The ratio of these amplitudes defines the [[Characteristic Impedance]] of the transmission line:
$$
Z_0= \frac{V_0^+}{I_0^+}=\frac{-V_0^-}{I_0^-}
$$


---

### Lossless Transmission Line
In the case of a lossless transmission line, $R'$ and $G'$ are negligible, which results in:
$$
\gamma=j\omega\sqrt{L'C'}
$$
which implies:
$$\begin{align*}
\alpha&=0\\[5pt]\hline
\beta&=\omega\sqrt{L'C'}\\
&= \omega\sqrt{\mu\varepsilon}\\[10pt]\hline
Z_0&= \sqrt{\frac{L'}{C'}}\\[10pt]\hline
u_p&= \frac{1}{\sqrt{L'C'}}\\
&= \frac{1}{\sqrt{\mu\varepsilon}}
\end{align*}$$
where
- $\alpha$ = [[Attenuation]] constant
- $\beta$ = [[Wave Number]]
- $u_p$ = [[Waves#Phase Velocity|Phase Velocity]]
- $\mu$ = [[Permeability]] of insulator
- $\varepsilon$ = [[Permittivity]] of insulator

