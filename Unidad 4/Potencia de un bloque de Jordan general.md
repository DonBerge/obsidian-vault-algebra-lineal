Si $A \in \mathbb F^{p \times p}$ es un bloque de Jordan asociado al autovalor $\lambda$:

$$A = 
\begin{pmatrix}
	\lambda & 0 & 0 & \dots & 0 & 0\\
	1 & \lambda & 0 & \dots & 0 & 0\\
	0 & 1 & \lambda & \dots & 0 & 0\\
	0 & 0 & 1 & \dots & 0 & 0\\
	\vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\
	0 & 0 & 0 &\dots & 1 & \lambda
\end{pmatrix}$$
Es decir: $A_{ij} = \delta_{i+1,j} + \delta_{i,j} \lambda$, entonces $(A^n)_{ij} = \sum_{k=0}^n \delta_{i+n-k,j} \binom n k \lambda^{k}$

Por inducción en los naturales:

CB)
	$n=2$
	$A^2 = A \cdot A$
	$A^2_{ij} = (\delta_{i+1,k}+\delta_{ik}\lambda)(\delta_{k+1,j}+\delta_{kj}\lambda)$
	$=\delta_{i+1,k}\delta_{k+1,j}+\delta_{ik}\lambda \delta_{k+1,j} + \delta_{i+1,k}\delta_{kj}\lambda + \delta_{ik}\delta_{kj}\lambda^2$
	$=\delta_{i+2,j}+\delta_{i+1,j}\lambda+\delta_{i+1,j}\lambda+\delta_{ij}\lambda^2$
	$=\delta_{i+2-0,j} \binom 2 0 \lambda^{0}+\delta_{i+2-1,j}\binom 2 1 \lambda^{1} + \delta_{i+2-2,j} \binom 2 2 \lambda^{2}$
	$=\sum_{k=0}^2 \delta_{i+2-k,j} \binom 2 k \lambda^k$

HI) $A_{ij} = \delta_{i+1,j} + \delta_{i,j} \lambda \implies (A^n)_{ij} = \sum_{k=0}^n \delta_{i+n-k,j} \binom n k \lambda^{k}$

PI)
	$A^{n+1} = A \cdot A^n$
	$A^{n+1}_{ij}=\sum_{s=1}^p A_{is}{A^n}_{sj} = \sum_{s=1}^p (\delta_{i+1,s} + \delta_{i,s} \lambda)(\sum_{k=0}^n \delta_{s+n-k,j} \binom n k \lambda^{k})$
	$=\sum_{s=1}^p \sum_{k=0}^n \delta_{i+1,s}\delta_{s+n-k,j}\binom n k \lambda^k + \sum_{s=1}^p \sum_{k=0}^n \delta_{i,s}\lambda \cdot \delta_{s+n-k,j}\binom n k \lambda^k$
	$=\sum_{k=0}^n \delta_{i+n+1-k,j} \binom n k \lambda^k + \sum_{k=0}^n \delta_{i+n-k,j} \binom n k \lambda^{k+1}$
	$=\sum_{k=0}^n \delta_{i+n+1-k,j} \binom n k \lambda^k + \sum_{k=1}^{n+1} \delta_{i+n-(k-1),j} \binom n {k-1} \lambda^k$
	$= \sum_{k=0}^n \delta_{i+n+1-k,j}\binom n k \lambda^k + \sum_{k=0}^n \delta_{i+n+1-k,j} \binom n {k-1} \lambda^k + \delta_{i+n-(n+1-1),j} \binom n {n+1-1} \lambda^{n+1}$
	$= \delta_{ij} \binom n n \lambda^{n+1} + \sum_{k=0}^n \delta_{i+n+1-k,j} \left(\binom n k + \binom n {k-1}\right) \lambda^k$
	$=\delta_{i+(n+1)-(n+1),j} \binom{n+1}{n+1} \lambda^{n+1} + \sum_{k=0}^n \delta_{i+n+1-k} \binom{n+1} k \lambda^k$
	$=\sum_{k=0}^n \delta_{i+n+1-k} \binom{n+1} k \lambda^k$
$\blacksquare$
