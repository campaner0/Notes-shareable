---
type: note
tags: [Math]
---
11/17/2022 18:01

  

An eigenvector of a $n\times n$ [[Matrix]] $A$ is a nonzero [[Vector]] $x$ such that $Ax=\lambda x$ for some scalar $\lambda$, an eigenvalue of $A$. The eigenvectors of a matrix are the vectors that stay on their [[Span]] when the transformation is applied to the [[Vector Space]] that contains the vectors. That is, they are not rotated or shifted. Therefore, a rotation matrix has no eigenvectors. 

For $\lambda$ to be an eigenvalue of $A$, the following equation must be true for $x\ne 0$:
$$
(A-\lambda I)x=0
$$
To find the eigen values of $A$:
1. Calculate the [[Determinant]] $\text{det}(A-\lambda I)$
2. Solve the resulting polynomial for $\lambda$
3. For each value of $\lambda$, reduce the augmented matrix $[\begin{array}{c|c}A-\lambda I&0\end{array}]$ 
4. The span of resulting vectors is the eigenspace for that eigenvalue

>[!note]
>The eigenspace of $A$ is simply the set of all eigenvectors of $A$:
$$
\text{Eigenspace}=\{x\mid Ax=\lambda x\}
$$

