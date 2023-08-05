Sea (V,⟨·, ·⟩) un F-espacio vectorial con producto interno. Decimos que un endomorfismo T ∈ L(V )
es un operador positivo si es autoadjunto y ⟨T v, v⟩ ≥ 0 para todo v ∈ V .
(a) Sea U ⊂ V un subespacio de V . Pruebe que la proyección ortogonal pU es operador positivo.
(b) Si T es un operador definido positivo, pruebe que los autovalores de T son no negativos.
(c) Si T es un operador definido positivo y v, w ∈ V son dos vectores tales que T v = w y T w = v,
entonces v = w.

a)
	Sea $V$ un ev con pi, $S \subseteq V$ un sev de $V$ y $p_S$ la proyección ortogonal sobre $S$, $p_S$ es una transformación autoadjunta

	$p_s(v) = \begin{cases}v & v \in S \\ 0 & v \notin S\end{cases}$
	Sea $B'=\{v_1,\dots v_k\}$ una bon de $S$, extiendo $B'$ a una base de $B$ y luego la convierto en una base ortonormal $B=\{v_1,\dots,v_k,v_{k+1},\dots,v_n\}$ usando gran schimidt.

	$v_i \in S \implies [p_S(v_i)]_B = [v_i]_B = e_i$
	$v_i \notin S \implies [p_S(v_i)]_B = [0]_B = 0$

	$$[p_S]_B = \begin{pmatrix} 
	1 & 0 & \dots & 0 & 0 & 0\\ 
	0 & 1 & \dots & 0 & 0 & 0\\ 
	\vdots &  \vdots & \ddots & \vdots & \vdots & \vdots\\ 
	0 & 0 & \dots & 0 & 0 & 0\\
	\vdots &  \vdots & \vdots & \vdots & \ddots & \vdots\\ 
	0 & 0 & 0 & 0 & 0 & 0
	\end{pmatrix}$$
	$[p_S]$ es una matriz diagonal con 1s y 0s en la diagonal, es hermitica y por lo tanto $p_S$ es autoadjunta.
	$<p_S(v), v> = \begin{cases} <v,v> = ||v||^2 & v \in S \\ <0,v> = 0\end{cases} \implies \langle p_S(v),v\rangle \geq 0$
b)
	Sea $\lambda$ autovalor de $T$ y $v$ su autovector asociado
	$\langle Tv, v \rangle = \langle \lambda v,v\rangle = \lambda||v||^2 \geq 0 \implies \lambda \geq 0$
	$\lambda$ es no negativo
c)
	$T(v)=w$
	$T(w)=v$
	$T(v-w)=T(v)-T(w)=w-v=-(v-w)$
	Si $v-w\neq 0$, $-1$ es un autovalor pero como $T$ es un operador positivo esto no puede ser.
	Resulta $v-w = 0$ y $v=w$.