---
type: note
alias: AM
tags: [Circuit_Analysis]
---
02/16/2023 10:15

  

When communicating with [[Electromagnetic Wave]]s, the amplitude of the wave may be varied, or modulated, in a certain way to encode information. This is done on a high [[Frequency]] carrier wave, and the rate at which the amplitude of the carrier wave changes is called the envelope, which is the encoded signal. 

This envelope is recovered on the receiving end with an [[Envelope Detector]].

To attach a message to a carrier, multiply the message wave by the carrier:
$$
m(t)c(t)=s(t)
$$
where
- $m$ = message wave
- $c$ = carrier wave
- $s$ = transmitted signal

## Double Side Band Suppressed Carrier
For a double side band (DSB) transmission, the message is multiplied by a sinusoidal carrier in the time domain:
$$
u_{DSB}(t)=Am(t)\cos(2\pi f_ct)
$$
which is achieved by convolution in the frequency domain. 

This results in four impulses where the frequencies overlap, the two side bands around each suppressed carrier, that is, a zero amplitude carrier. Convolve with the carrier again in the frequency domain to recover the message, filtering out artifacts with a [[Low-Pass Filter]].

### Conventional AM
Conventional AM is a DSB-SC signal with the carrier added again:
$$
u_{AM}(t)=Am(t)\cos(2\pi f_ct)+A_{c}\cos(2\pi f_{c}t)
$$
This creates impulses in the frequency domain at $f_c$ along with the previous impulses. With a large enough $A_c$ the transmission waveform does not cross 0, which eliminates chirping, and eliminates the need for the carrier to be generated at the receiver. The message can be decoded with an envelope detector.