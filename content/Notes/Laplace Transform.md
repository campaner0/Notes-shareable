---
type: note
---
10/31/2022 16:23

Tags: #math #Circuit_Analysis 

The Laplace transform converts a real-valued function into its complex-valued equivalent. This can be useful for functions that are easier to manipulate and compute in the frequency domain (e.g. differential equations become algebraic). To find the Laplace transform of a function: 
$$
\mathscr{L}\{f(t)\}=F(s)=\int_{-\infty}^{\infty}e^{-st}f(t)dt
$$
where
- $F(s)$ = complex-valued function
- $s$ = [[Complex Frequency]]
- $t$ = [[Time]]

>[!note]
>If only part of a function is of interest or is only defined for certain values, the limits of the integral can be changed accordingly. 
>>[!example]
>>The one-sided Laplace transform:
>>$\mathscr{L}\{u(t)\}=\int_{0}^{\infty}e^{-st}dt$

---

### Identities

Laplace Transform Pairs:
$$
\begin{array}{l|l}
        
        \boldsymbol{f(t)} & \boldsymbol{F(s)}\\[5pt]
		\hline
		0&0\\
		\hline
        t^n\mid n\ge0& \displaystyle{ \frac{n!}{s^{n+1}} }\\[5pt]
        \hline
        e^{at}& \displaystyle{ \frac{1}{s-a} }\\[5pt]
        \hline
        \sin(\omega t)& \displaystyle{ \frac{\omega}{s^{2}+\omega^{2}} }\\[5pt]
        \hline
        \cos(\omega t)& \displaystyle{ \frac{s}{s^{2}+\omega^{2}} }\\[5pt]
        \hline
        \sin(\omega t+\theta) & \displaystyle{ \frac{s\sin(\theta)+\omega\cos(\theta)}{s^{2}+\omega^{2}} }\\[5pt]
        \hline
        \cos(\omega t+\theta) & \displaystyle{ \frac{s\sin(\theta)+\omega\cos(\theta)}{s^{2}+\omega^{2}} }\\[5pt]
        \hline
        e^{-at}\sin(\omega t)& \displaystyle{ \frac{\omega}{(s+a)^{2}+\omega^{2}} }\\[5pt]
        \hline
        e^{-at}\cos(\omega t) & \displaystyle{ \frac{s+\alpha}{(s+a)^{2}+\omega^{2}} }\\[5pt]
        \hline
        u(t-a) & \displaystyle{ \frac{1}{s}e^{-as} }\\[5pt]
        \delta(t-a)& e^{-as}\\[5pt]
        \hline
        1-e^{-at}& \displaystyle{ \frac{a}{s(s+a)} }\\[5pt]
        \hline
        \displaystyle{ \frac{1}{\beta-\alpha}(e^{-\alpha t}-e^{-\beta t}) } & \displaystyle{ \frac{1}{(s+\alpha)(s+\beta)} }\\[5pt]
        
\end{array}
$$
where
- $a\in\mathbb{R}$   
- $u(t-a)$ = [[Step Function]]
- $\delta(t-a)$ = [[Unit Impulse Function]]


Laplace Operations:
$$
\begin{array}{l|l|l}
\mathbf{Operation} & \boldsymbol{f(t)} & \boldsymbol{F(s)}\\[5pt]
\hline
\text{Addition} & f_{1}(t)\pm f_{2}(t) & F_{1}(s)\pm F_{2}(s)\\[5pt]
\hline
\text{Scalar Multiplication} & kf(t) & kF(s)\\[5pt]
\hline
\text{Time Differentiation} & \displaystyle{ \frac{df}{dt} } & sF(s)-f(0^{-})\\[5pt]
& \displaystyle{ \frac{d^{2}f}{dt^{2}} } & s^{2}F(s)-sf(0^{-})-f'(0^{-})\\[5pt]
& \displaystyle{ \frac{d^{3}f}{dt^{3}} } & s^{3}F(s)-s^{2}f(0^{-})-sf'(0^{-})-f''(0^{-})\\[5pt]
\hline
\text{Time Integration} & \displaystyle{ \int_{0^{-}}^{t}f(t)dt } & \displaystyle{ \frac{1}{s}F(s) }\\[5pt]
& \displaystyle{ \int_{-\infty}^{t}f(t)dt } & \displaystyle{ {\frac{1}{s}}F(s)+{\frac{1}{s}}\int_{-\infty}^{0^{-}}f(t)\,dt }\\[5pt]
\hline
\text{Convolution} & f_{1}(t)* f_{2}(t) & F_{1}(s)F_{2}(s)\\[5pt]
\hline
\text{Time Shift} & f(t-a)u(t-a),a\geq0 & e^{-as}F(s)\\[5pt]
\hline
\text{Frequency Shift} & f(t)e^{-at} & F(s+a)\\[5pt]
\hline
\text{Frequency Differentiation} & tf(t) & \displaystyle{ -{\frac{dF(\mathrm{s})}{ds}} }\\[5pt]
\hline
\text{Frequency Integration} & \displaystyle{ \frac{f(t)}{t} } & \displaystyle{ \int_{s}^{\infty}F(s)ds }\\[5pt]
\hline
\text{Scaling} & f(at),a\ge0 & \displaystyle{ \frac{1}{a}F\left(\frac{s}{a}\right) }\\[5pt]
\hline
\text{Intial Value} & f(0^{+}) & \displaystyle{ \lim_{s\rightarrow \infty}sF(s) }\\[5pt]
\hline
\text{Final Value} & f(\infty) & \displaystyle{ \lim_{s\rightarrow 0}sF(s) },\,\text{all poles of }sF(s)\,\text{in LHP}\\[5pt]
\hline
\text{Time Periodicity} 
& 
 \begin{array}{l} 
  f(t) = f(t+nT),\\ 
  n=1,2,\dots 
 \end{array} 
& 
 \begin{array}{l}
  \displaystyle{\frac{1}{1-e^{-T s}}F_{1}(s),}\\ 
  \text{where}\,F_{1}(s) = \displaystyle{ \int_{0^{-}}^{T}f(t)e^{-st}\,dt }
 \end{array}
\end{array}
$$


>[!note]
>These identities are for the one-sided Laplace Transform

---

### The Inverse Laplace Transform
To find the real-valued equivalent of a complex function, or to reverse the Laplace transform, the following functon can be used:
$$
f(t)= \frac{1}{2\pi j}\int_{\sigma_0-j\infty}^{\sigma_0+\infty}e^{st}F(s)ds
$$
where
- $\sigma_0$ = [[Attenuation|Neper Frequency]]