Un sev $U \subset V$ es un subespacio invariante por una tl $T \in L(V)$ si $T(U) \subseteq U$

$\ker(T)$ es invariante por $T$ )
	$v \in ker(T) \implies T(v) = 0$ y $0 \in ker(T)$ por lo tanto $T(\ker(T)) \subseteq ker(T)$
$V$ es invariante por $T$ )
	El codominio de $T$ es $V$ por lo que $im(T) = T(V) \subseteq V$
$U$ es $T$ invariante con $\dim(U)=1$ $\iff$ $U = span(v)$ donde $v$ es un autovector de $T$
	$\implies$)
		$\dim(U) = 1 \implies U = span(v)$ con $v \in \mathbb V$.
		$U$ es $T$ invariante por lo que si $w \in U \implies T(w) \in U$
		$T(w) = w'$
		$\dim(U) \neq 0 \implies \exists w \in U : w\neq 0$
		Tomando $w \neq 0$
		$T(w)=w'$
		$T(\lambda_1 v) = \lambda_2 v$
		$\lambda_1T(v) = \lambda_2 v$
		$T(v) = \frac{\lambda_2}{\lambda_1}v$, $v$ es un autovector de $T$
	$\impliedby$)
		$U = span(v)$, $u \in U \implies \exists \lambda : u = \lambda v$
		$v$ autovector de $T$
		$\forall u \in U, T(u) = T(\lambda v) = \lambda T(v) = \lambda \cdot \rho  \cdot v \in U$
		$U$ es $T$-invariante
$U,W$ $T$-invariantes $\implies$ $U \cap W$ y $U+W$ son $T$-invariantes:
	$v \in U \cap W \implies v \in U \land v \in W \implies T(v) \in U \land T(v) \in W \implies T(v) \in U \cap W$.
	$v \in U+W \implies v = u+w, u \in U \land w \in W \implies T(v) = T(u) + T(w), T(u) \in U \land T(w) \in W \implies T(v) \in U+W$
Sea $T \in L(V)$, $U\subseteq V$ $T$-invariante y $T_U \in L(U)$ $T$ restringida a $U$ entonces:
$m_{T_U} | m_T$)
	Sea $B_u = \{v_1,...,v_s\}$ base de $U$, extiendo a una base $B=\{v_1,...,v_n\}$ de $V$:
	$m_T=mcm(m_{v_1},...,m_{v_n})$
	$m_{v_i} | m_T$ asi que $m_{T_U}=mcm(m_{v_1},...m_{v_s}) | m_T$
$\chi_{T_U} | \chi_T$)
	Sea $B_u = \{v_1,...,v_s\}$ base de $U$, extiendo a una base $B=\{v_1,...,v_n\}$ de $V$:
	$v \in B_u \implies T(v) \in U$ asi que se puede escribir como cl de vectores de $B_U$ $T(v) = \sum_{i=0}^s \alpha_i v_i + \sum_{j=s+1}^n 0 \cdot v_j$
	$[T]_B = \begin{pmatrix} [T_U]_{B_U} & B \\ 0 & C\end{pmatrix}$
	$XI_n-[T]_B = \begin{pmatrix} XI_s - [T_U]_{B_U} & -B \\ 0 & XI_{n-s} -C\end{pmatrix}$
	$\chi_T(X) = \det(XI_n-[T]_B) = \det(XI_s - [T_U]_{B_U})\det(XI_{n-s} - C) = \chi_{T_U}(X)Q(X)$
	$\chi_{T_U} | \chi_T$
	