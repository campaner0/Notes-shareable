---
type: note
alias: Complex Number
tags: [Math, Circuit_Analysis]
---
04/08/2022 14:34

  , 

Complex numbers are numbers with an imaginary component, that is, with a part that is a multiple of $i$ ($j$ in electrical engineering contexts), where $i^2=-1$. The real numbers are a subset of the complex numbers with an imaginary part of zero. Complex numbers are displayed on the complex plane, where the vertical axis is the imaginary axis and the horizontal is the real axis. 


## Rectangular
Complex numbers written in rectangular form are in the form
$$
a+bi
$$
where $a$ is the real part, and $b$ is the imaginary part. Addition/subtraction in this form is easier than in polar, but multiplication is harder.

---

## Polar
Polar form looks like
$$
Ae^{i\theta}=A\angle\theta
$$
where $A$ is the magnitude of a [[Vector]] that locates the point which the complex number represents on the complex plane, and $\theta$ is the vector's angle from the real axis. Multiplication/division is easier in this form due to its exponential nature.

>[!note]
>This form is related to the trigonometric functions through [[Euler's Formula]]

---

## Conversion
The two forms are different ways of refering to the same point on the comlex plane. Their relationship can be thought of as each being different parts of a right triangle: $a$ and $b$ are the legs and $A$ is the hypotonuse, with $\theta$ being the angle between $A$ and $a$. When thought of this way, conversion is possible through trigonometry:
### Rectangular to polar
$$\begin{align*}
A&=|a+bi|=\sqrt{a^2+b^2}\\[5pt]
\theta&=\tan^{-1}\left(\frac{b}{a}\right)
\end{align*}$$

>[!note]
>If the complex number is in the second or third quadrent, $180^\circ$ must be added to get the correct angle because of the domain of inverse [[Tangent]]

---

### Polar to Rectangular
$$\begin{align*}
a&=A\cos(\theta)\\[5pt]
b&=A\sin(\theta)
\end{align*}$$