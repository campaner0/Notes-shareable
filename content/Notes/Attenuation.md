---
type: note
aliases:
  - Attenuates
  - Attenuate
  - Attenuated
tags: [Electromagnetics, Circuit_Analysis]
---
11/01/2022 17:53

  

The attenuation of an oscillating signal is the measure of how quickly the energy of the wave changes (in most cases it is reduced) such that the amplitude of the wave approaches infinity or zero. 


### The Exponentially Damped Sinusoid

The most general case of attenuation is the exponentially damped sinusoid with a [[Complex Frequency]]. All others are a special case of this description.
$$
v(t)= \frac{1}{2}Ae^{j\theta}e^{j(\sigma+j\omega)t}+\frac{1}{2}Ae^{-j\theta}e^{j(\sigma-j\omega)t}
$$
where
- $A$ = amplitude
- $\theta$ = [[Phase Angle]]
- $\sigma$ = [[Neper Frequency]]
- $\omega$ = [[Angular Velocity|Angular Frequency]]

The complex constants of $s_1$ and $s_2\,$, $K_1$ and $K_2$ are conjugates, hence: $s_1=s_2^*=\sigma+j\omega$ and $K_1=K_2^*=\frac{1}{2}V_me^{j\theta}$. This is the only way for the function to represent a real voltage.

>[!note]
>The sinusoidal function is rewritten as an exponential using [[Euler's Formula]]

---

### Special Cases

>[!example] Purely Real Damped Sinusoid
>In this case, the imaginary part of the complex frequency is zero:
>$$
v(t)=\mathfrak{Re}\{Ae^{j\theta}e^{st}\}=Ae^{\sigma t}\cos(\omega t+\theta)
$$

>[!example] Undamped Sinusoid
>In this case, the real part of the complex frequency is zero:
>$$
v(t)=K_1e^{s_1t}+K_2e^{s_2t}
$$

>[!example] Exponential
>This case is simply the exponential function with the imaginary part of the complex frequency equal to zero:
>$$
v(t)=Ae^{\sigma t}
$$

>[!example] DC
>A DC signal is simply an exponential with complex frequency $s=0$
>$$
v(t)=A
$$

