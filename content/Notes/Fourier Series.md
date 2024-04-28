---
type: note
---
03/29/2023 13:49

  #Signals 

Any continuous periodic function $f(t)$ can be formed by an infinite sum of sin and cos called a Fourier series. Practically, a finite sum can be used for a very good approximation. The infinite sum of a function $f(t)$ is given by:
$$
f(t)=a_0+\sum\limits^\infty_{n=1}a_n\cos(n\omega_0 t)+b_n\sin(n\omega_0 t)
$$
where
- $a_{0}=\frac{1}{T}\int_Tf(t)dt$
- $a_n=\frac{2}{T}\int_Tf(t)\cos(n\omega_0 t)dt$
- $b_n=\frac{2}{T}\int_Tf(t)\sin(n\omega_0 t)dt$
- $T$ = period of function
- $\omega_0$ = [[Angular Velocity|Angular Frequency]] of function
- $t$ = [[Time]]

---

## Compact Fourier Series

$$
f(t)=a_0+\sum\limits_{n=1}^{\infty}C_n\cos(n\omega_0t+\theta_n)
$$
where
- $C_n=\sqrt{a_n^2+b_n^2}$
- $\omega_{0}$ = fundamental angular frequency
- $\theta_n=\tan^{-1}\left(\frac{-b_{n}}{a_{n}}\right)$ 