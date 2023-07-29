Si $T \in L(V)$ con $\dim(V) = n$ es una matriz $n$ pasos nilpotente entonces $m_T(X)=X^n$
Como $gr(m)=gr(\chi)$, $\chi_T=m_T$

$B=\{v,Tv,T^2v,\dots,T^{n-1}v\}$ es un conjunto li(si fuera ld entonces el polinomio minimal tendría grado $n-1$) de $n$ vectores, por lo que es base de $V$.

$i<n-1 \implies [T(T^i v)]_B = [T^{i+1}v]_B = e_{i+1}$
$[T(T^{n-1})v]_B = [T^n v]_B = [0]_B$

$$[T]_B = 
\begin{pmatrix}
	0 & 0 & 0 & \dots & 0 & 0\\
	1 & 0 & 0 & \dots & 0 & 0\\
	0 & 1 & 0 & \dots & 0 & 0\\
	0 & 0 & 1 & \dots & 0 & 0\\
	\vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\
	0 & 0 & 0 &\dots & 1 & 0
\end{pmatrix}$$