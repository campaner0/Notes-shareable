---
type: note
tags: [math]
---
03/12/2024 17:56

  

Formulas for conversion between Cartesian Coordinates, [[Cylindrical Coordinates]], and [[Spherical Coordinates]]

$$
\begin{array}{c}

 \begin{array}{l|c}
  \text{Cartesian to:}\\
  \hline
  \text{Cylindrical} & 
  
   \begin{array}{}
    r= +\sqrt{x^2+y^2}\\
    \phi= \tan^{-1}(y/x)\\
    z= z
   \end{array}\\
   
  \hline
  \text{Spherical} & 
  
   \begin{array}{}
    R= +\sqrt{x^2+y^2+z^2}\\
    \theta= \tan^{-1}\left(\frac{+\sqrt{x^2+y^2}}{z}\right)\\
    \phi= \tan^{-1}(y/x)
   \end{array}\\
   
 \end{array}
 
&

 \begin{array}{l|c}
  \text{Cylindrical to:}\\
  \hline
  \text{Cartesian} &
  
   \begin{array}{}
    x= r\cos\phi\\
    y= r\sin\phi\\
    z= z
   \end{array}\\
  \hline
  \text{Spherical} &
  
   \begin{array}{}
    R= +\sqrt{r^2+z^2}\\
    \theta= \tan^{-1}(r/z)\\
    \phi= \phi
   \end{array}\\
  \end{array}
  
&
 \begin{array}{l|c}
  \text{Spherical to:}\\
  \hline
  \text{Cartesian} &
  
   \begin{array}{}
    x= R\sin\theta\cos\phi\\
    y= R\sin\theta\sin\phi\\
    z= R\cos\theta
   \end{array}\\
   
  \hline
  \text{Cylindrical} &
  
   \begin{array}{}
    r= R\sin\theta\\
    \phi=\phi\\
    z= R\cos\theta
   \end{array}\\
   
 \end{array}

\end{array}$$
