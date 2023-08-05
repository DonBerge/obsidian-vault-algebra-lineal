Si $V$ es un $\mathbb F$-ev con producto interno de dimensión finita y $T \in L(V)$ entonces son equivalentes:
1) $T$ es una tl autoadjunta
2) $\forall B$ bon de $V$, $[T]_B$ es hermitica
3) $\exists B$ bon de $V$, $[T]_B$ es hermitica

$1 \implies 2$)
	Si $T$ es una matriz autoadjunta entonces $<T(u),v> = <u,T(v)>$ para $u,v \in V$
	Sea $B$ una bon de $V$, $g=I$
	$<T(v),u>=<v,T(u)>$
	$([T]_B[v]_B)\cdot [u]_B^* = [v]_B ([T]_B [u]_B)^*$
	$[T]_B([v_B]\cdot [u]_B^*) = ([v]_B[u]_B^*)[T]_B^*$
	$[T]_B<v,u> = <v,u>[T]_B^*$
	Tomando $v=u$, $<v,u>=1$
	$[T]_B=[T]_B^*$
$2 \implies 3$)
	Trivial
$3 \implies 1$)
	Sea $B$ una bon tal que $[T]_B=[T]_B^*$:
	$[T]_B=[T]_B^*$
	$[T]_B<v,u>=<v,u>[T]_B^*$
	$[T]_B([v_B]\cdot [u]_B^*) = ([v]_B[u]_B^*)[T]_B^*$
	$([T]_B[v]_B)\cdot [u]_B^* = [v]_B ([T]_B [u]_B)^*$
	$<T(v),u>=<v,T(u)>$
	$T$ es autoadjunta