Sea $T:V \to W$ una tl, se cumple que:

$$\dim(\ker(T)) + \dim(Im(T))) = \dim(V)$$
$k:=\dim(ker(T))$
$n:=\dim(V)$
Dada una base de $\ker(T)$, $\{v_1,...,v_k\}$, la extiendo a una base de $V$ usando los vectores $\{v_{k+1},...,v_n\}$. $\{T(v_{k+1}),...,T(v_n)\}$ es una base de $Im(T)$.

$\sum_{i=k+1}^n a_i T(v_i) = 0 \iff T(\sum_{i=k+1}^n a_i v_i) = 0 \implies \sum_{i=k+1}^n a_i v_i \in \ker(T)$

Por lo tanto
$\sum_{i=k+1}^n a_i v_i = \sum_{i=0}^k b_i v_i \implies \sum_{i=k+1}^n a_i v_i - \sum_{i=0}^k b_i v_i = 0 \implies \forall i, b_i=0 \land a_i=0$

Los vectores $T(v_i)$ son li.

Los $T(v_i)$ vectores generan $Im(T)$,
$\Span(T(v_i)) \subseteq Im(T)$
$v \in Im(T) \implies \exists u \in V : T(u)=v$
$T(u)=T(\sum_{i=0}^na_i v_i) \implies \sum_{i=0}^n a_i T(v_i) \implies \sum_{i=k+1}^n a_i T(v_i)$(Los $v_i$ de $0$ a $k$ se cancelan por ser vectores de $\ker(T)$). Luego $v \in \Span(T(v_i))$.

$\dim(\ker(T)) = k$
$\dim(Im(T))=n-k$
$\dim(V)=n$
$\dim(\ker(T)) + \dim(Im(T))) = \dim(V)$