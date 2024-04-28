---
type: note
---
10/25/2023 14:59

  #comunication_systems 


Digital modulation is the process of translating bits into an analog waveform for transmission. In this case, the information transmitted is digital, as opposed to [[Amplitude Modulation|AM]] or [[Angle Modulation|FM]] transmission, where analog information is transmitted.



## Linear Modulation
In linear modulation, bits are transmitted by a series of rectangular pules where the amplitude of each pulse represents a bit value or a series of bit values. When using more amplitude states, more bits can be transmitted in one pulse. For example, 4PAM, or 4 pulse amplitude modulation, each pulse transmits two bits. In 2PAM, there are two availible states, so each pulse represents one bit. With more availible states, the pulse amplitude changes less often, resulting in less high-frequency content and, therefore, less susceptibility to noise.

### Intersymbol Interference
The rectangular pulses of linear modulation cause interference between pulses as a rectangular pulse in the time domain will have a [[Sinc]] frequency shape. The oscillating tails of the function will interfere with subsequent pulses. This can be mitigated with a [[Cosine Squared Filter]] or [[Raised Cosine Filter]]. 