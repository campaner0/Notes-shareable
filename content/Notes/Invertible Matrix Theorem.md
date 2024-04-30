---
type: note
tags: [Math]
---
11/16/2022 12:03

  

Given a $n\times n$ [[Matrix]] $A$, the following statements are equivalent:

- $A$ is [[Inverse of a Matrix|Invertible]]
- $A$ is row equivalent to the $n\times n$ [[Identity Matrix]] $I$
	- that is, it can be reduced to $I$ through [[Elementary Row Operations]]
- $A$ has $n$ pivot positions
- $Ax=0$ has only the trivial solution
- The columns of $A$ form a [[Linear Independence|Linearly Independent]] set
- $x\mapsto Ax$ is [[1-1 Functions|One-To-One]]
- $Ax=b$ has at least one solution for $b\in\mathbb{R}^n$
- The columns of $A$ [[Span]] $\mathbb{R}^n$
- $x\mapsto Ax$ maps $\mathbb{R}^n$ [[Onto]] $\mathbb{R}^n$
- $\exists$ an $n\times n$ matrix $C$ such that $CA=I$
- $\exists$ an $n\times n$ matrix $D$ such that $AD=I$
- $A^T$ is an invertible matrix
	- where $A^T$ is $A$ [[Matrix Operations#Transposition|Transpose]]
- $\operatorname{Col}(A)=\mathbb{R}^n$
- $\operatorname{dim}(\operatorname{Col}(A))=n$
- $\operatorname{Rank}(A)=n$
- $\operatorname{Nul}(A)=0$