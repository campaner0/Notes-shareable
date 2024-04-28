---
type: note
---
### Bandpass Filter
The bandpass filter allows only a limited band to pass. It behaves like a high-pass and lowpass put together, attenuating high and low frequencies beyond its two corner frequencies. A passive filter can be constructed with an [[RLC Circuits|RLC Circuit]]:

![[Pasted image 20221116162441.png]]

Its transfer function:
$$
H(s)=\frac{RCs}{LCs^2+RCs+1}
$$
The allowed bandwidth is $R/L$ with a center frequency of:
$$
\omega_0= \frac{1}{\sqrt{LC}}
$$


---