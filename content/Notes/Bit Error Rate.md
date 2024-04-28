---
type: note
aliases:
  - BER
tags: [comunication_systems]
---
11/06/2023 14:42

  

The bit error rate is the number of errors in bit transmission per unit time in a [[Digital Modulation]] transmission. Errors can be caused by noise, interference, distortion, attenuation, or bit synchronization error. 

For 16 QAM:
$$
\text{BER}\approx\frac{3}{4}\text{erfc}\left(\sqrt{\frac{4E_{b}}{9N_{0}}}\right)
$$
where
- $\text{erfc}()$ = [[Complementary Error Function]]
- $\frac{E_b}{N_{0}}$ = bit energy to noise floor ratio (signal to noise ratio)