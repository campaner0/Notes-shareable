---
type: note
alias: Discrete Signal
---
03/22/2023 14:02

  #Signals 

Discrete signals are a sequence of values that correspond to moments in time of an analog signal. These moments are the sample times, and the frequency of sample times is the sampling rate. The sampling rate must be greater than double the frequency of the analog signal to avoid aliasing (Nyquist Criteria). An analog signal must be converted to a discrete signal in order to transmit using [[Digital Modulation]].

$$
u(t)=\sum\limits_nb[n]p(t-nT)
$$
where
- $u$ = discrete signal
- $n$ = number of samples 
- $b$ = sequence of samples
- $p$ = modulating pulse
- $t$ = [[Time]]
- $T$ = period of signal

For example, if an analog signal is defined as:
$$
x(t)=0.01\sin(2\pi (61.74)t)
$$
then a discrete representation of the signal would be represented by:
$$
x[n]=\sum\limits_{n}^{}0.01\sin[2\pi(61.74)(t-nT)]
$$
where
- $N$ = the nth sample
