Sean $B_1=\{v_1,...,v_n\}$ y $B_2=\{w_1,...,w_n\}$ dos bases de $V$ y $W$ y $T \in L(V,W)$:

Defino $[T]_{B_1B_2}$ como $([T]_{B_1B_2})_{i,j} = [T(v_j)]_i$

Se cumple que $\forall v \in V, [T]_{B_1B_2} [v]_{B_1}^t = [T(v)]_{B_2}^t$

Defino:
$c_{i,j} = ([T(v_j)]_{B_2})_i$
$a_i = ([v]_{B_1}^t)_i$
$b_i = ([T]_{B_1B_2} [v]_{B_1}^t)_i = \sum_{k=0}^k c_{i,k}a_{k}$

$\sum_{k=0}^n c_{k,j}w_k = T(v_k)$

$\sum_{i=0}^n b_i w_i = \sum_{i=0}^n \sum_{k=0}^n c_{i,k}a_{k} w_i = \sum_{k=0}^n a_{k} \sum_{i=0}^n c_{i,k} w_i = \sum_{i=0}^n a_kT(v_k) = T(v_k)$

$(b_1,...,b_n)$ es el vector de coordenadas de $T(v)$ en la base $B_2$
