Dado un subespacio vectorial $U$ de $V$ existe otro subespacio $W$ de $V$ tal que $U \oplus W = V$.

[[Todo conjunto li se puede extender a una base de V]], se toma una base $B_1$ de $U$ y se extiende a una base $B$ de $V$, el espacio $W$ buscado es $\Span(B-B_1)$.

Sea $B_1=\{v_1,...,v_m\}$ y $B_2=\{v_{m+1},...,v_n\}$ donde $B=B_1 \cup B_2$:
$\Span(B_1)= U$ y $\Span(B_2) = W$, ambos son sev de $V$.

$U + W = V$, por doble inclusión:
$U+W \subseteq V$)
	$V = \Span(B)$
	$u \in U+W \implies u = \sum_{i=0}^m a_i v_i + \sum_{i=m+1}^n a_i v_i \implies u \in \Span(B)$
$V \subseteq U + W$)
	$V = \Span(B)$
	$v \in V \implies v \in \Span(B) \implies \sum_{i=0}^m a_i v_i + \sum_{i=m+1}^n a_i v_i \implies v \in U + W$

$u \in \Span(B_1) \cap \Span(B_2) \implies u = \sum_{i=0}^m a_i v_i = \sum_{i=m+1}^n a_i v_i$
$\implies 0 = \sum_{i=0}^m a_i v_i - \sum_{i=m+1}^n a_i v_i \implies \forall i, a_i = 0$ dado que el conjunto $B$ es una base. Por lo tanto $u=0$ y $U \oplus W = V$
