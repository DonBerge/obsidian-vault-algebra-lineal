Sea $V$ un $\mathbb F$-ev con pi y de dimensión finita y $T \in L(V)$ una transformación autoadjunta existe $B$ bon de $V$ tal que $[T]_B$ es una matriz diagonal real

Pruebo por inducción en $\dim(V$)

CB) $\dim(V)=1$
	$\exists u \in V : v \in span(u)$  
	$T(u)=w$, $w\in V$
	$T(u)=\lambda u$
	$\lambda$ autovalor, como $T$ es autoadjunta $\lambda \in \mathbb R$
	$\{u\}$ bon de $V$
	$[T]_{\{u\}} = \lambda$
	$\lambda$ es una matriz diagonal real
HI) Si $1<\dim(V)<n-1$ entonces se verifica el teorema	
PI)
	$\dim(V)=1$
	$T$ autoadjunta
	$T$ tiene al menos un autovalor real $\lambda$
	Sea $v$ un autovector de $T$ y $w:= \frac v {||v||}$. $T(w)=T\left(\frac{v}{||v||}\right)=\frac{1}{||v||}T(v) = \frac{1}{||v||}\lambda v = \lambda w$.
	$w$ es un autovector de $T$ asociado al autovalor $\lambda$
	$U=span(w)^\perp$ es un sev de $V$ de dimensión $n-1$
	Sea $B=\{w\} \cup B_U$ con $B_U$ una bon de $U$
	$[T]_B = \begin{pmatrix} \lambda & |  & 0 \\ - & - & -  \\ 0 & | & [T|_U]_{B_U}\end{pmatrix}$ 
	$[T|_U]_{B_U}$ es autoadjunta(sino $T$ no lo seria)
	Por hipótesis inductiva $[T]_{B_U}$ es una matriz diagonal real. $[T]_B$ es una matriz diagonal real.