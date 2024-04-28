---
type: note
alias: Active Filter
---
02/08/2023 19:19

  #Circuit_Analysis 

Active filters are [[Filters]] that include an [[Operational Amplifier|Op-Amp]] to filter frequencies and amplify the passband by a gain determined by the circuit configuration. A higher order filter is related to the slope of the stop band:

### 1st Order Active High-Pass Filter

![[Pasted image 20230208191018.png]]

This filter has the [[Transfer Function]]:
$$
H(\omega)=-\frac{R_{F}}{R_{1}}\left(\frac{1}{1+ \frac{1}{R_{1}j\omega C}}\right)
$$
and cutoff [[Frequency]]:
$$
\omega_c=\frac{1}{R_{1}C}
$$

---

### 1st Order Active Low-Pass Filter

![[Operational Amplifier 2023-01-24 09.46.24.excalidraw]]

Transfer function:
$$
H(\omega)=-\frac{R_{F}}{R_{1}}\left(\frac{1}{1+R_{F}j\omega C}\right)
$$

Cutoff frequency:
$$
\omega_{c}=\frac{1}{R_{F}C}
$$

---