Si $A \in \mathbb F^{n\times n}$ es un bloque de Jordan de la forma:

$$A = 
\begin{pmatrix}
	0 & 0 & 0 & \dots & 0 & 0\\
	1 & 0 & 0 & \dots & 0 & 0\\
	0 & 1 & 0 & \dots & 0 & 0\\
	0 & 0 & 1 & \dots & 0 & 0\\
	\vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\
	0 & 0 & 0 &\dots & 1 & 0
\end{pmatrix}$$
Es decir $A_{ij} = \delta_{i+1,j}$
Entonces $(A^k)_{ij}=\delta_{i+k,j}$

Por inducción en la dimensión de la matriz:
CB) $n=2$
$A=\begin{pmatrix} 0 & 0 \\ 1 & 0\end{pmatrix}$
$A^2 = \begin{pmatrix} 0 & 0 \\ 1 & 0\end{pmatrix}^2 = \begin{pmatrix} 0 & 0 \\ 0 & 0\end{pmatrix}$
La hipótesis se cumple.
HI) $A_{ij} = \delta_{i+1,j} \implies (A^k)_{ij}=\delta_{i+k,j}$
PI)
	$A^{n+1} = A \cdot A^n$
	$(A\cdot A^n)_{ij} = \sum_{k=0}^n A_{ik}\cdot A^n_{kj} = \sum_{k=1}^n \delta_{i+1,k}\cdot \delta_{k+n,j} = \delta_{i+n+1,j}$

Por inducción: $(A^k)_{ij}=\delta_{i+k,j}$

Corolario: Si $A$ es un bloque de Jordan $n\times n$, $ran(A^k)=n-k$