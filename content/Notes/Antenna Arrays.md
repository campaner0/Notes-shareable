---
type: note
aliases:
  - Antenna Array
---
02/28/2024 15:39

Tags: #Antennas #Electromagnetics 

An antenna array is a collection of [[Antennas]] with the same source or receiver. Because they are connected in this way, the antennas act as one larger antenna. By controlling the amplitude and phase of the signal fed into each antenna, the radiation pattern and direction can be be controlled electronically, even creating multiple beams. 

The power density of an array is given by:
$$
S(R_{0},\theta,\phi)=S_{e}(R_{0},\theta,\phi)F_{a}(\theta)
$$
where
- $S_e(R_{0},\theta,\phi)$ = [[Poynting Vector|Power Density]] radiated by one element
- $F_a(\theta)$ = Array factor

The array factor is the far field radiation intensity of the array if the elements were isotropic antennas. 
$$
F_{a}(\theta) = \left|\sum_{i=0}^{N-1}a_{i}e^{j\psi_{i}}e^{j i k d\cos\theta}\right|^{2}
$$
where
- $\theta$ = elevation angle
- $N$ = number of antennas in array
- $a_{i}$ = amplitude of element $i$
- $\psi_{i}$ = [[Phase Angle]]  of element $i$
- $k$ = angular [[Wave Number]] 
- $d$ = [[Distance]] between elements 

>[!info]+ Special Cases
>For an array with uniform phase:
>$$
F_{a}(\gamma) = \left|\sum_{i=0}^{N-1}a_{i}e^{j i \gamma}\right|^{2}
$$
>
>For uniform phase and amplitude:
>$$
F_{a}(\gamma) =\frac{\sin^2(N\gamma/2)}{\sin^{2}(\gamma/2)}
$$
>where $\gamma=kd\cos\theta$ 


## Beam Steering
Steering the beam electronically is achieved with a linear phase distribution. That is, the distance between each element is the same. 

The angle of the beam depends on the change in the broadside frequency:
$$
\cos\theta_{0}=\frac{2n_{0}\pi}{kd}\left(\frac{\Delta f}{f_{0}}\right)
$$
where
- $\theta_0$ = desired angle of beam
- $n_0$ = 
- $\Delta f$ = 
- $f_0$ = transmission frequency
