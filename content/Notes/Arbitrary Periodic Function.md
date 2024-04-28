---
type: note
alias: Arbitrary Periodic Functions
---
04/26/2023 13:54

Tags: #Signals 

The equation for a periodic function with an arbitrary waveform can be formed by summing sections of another function which have been shifted along the horizontal axis. The desired waveform can be selected from a function using a difference of [[Step Function]]s, and then the sections are summed such that the nth period is the chosen section shifted by n periods:

$$
\sum\limits_{n=-\infty}^{\infty}f(t-nT)[u(t-nT\pm\alpha_n)-u(t-nT\pm\beta_n)]
$$
where
- $n$ = number of repetitions ($\infty$ for a true periodic function)
- $T$ = desired period
- $\alpha_n$ = left limit 
- $\beta_n$ = right limit

>[!note]
>If $T\ne|\alpha_n-\beta_n|$, If the period is greater, the resulting function will appear to have a shortened duty cycle. If the period is less, the window that is repeated will shift along $f(t)$ as the periodic function repeats

