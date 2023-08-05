Sea $U$ sev de $V$($V$ es un $\mathbb F$-ev con pi) y $W=U^\perp$,
$$\dim(U) + \dim(U^\perp) = \dim(V)$$
Sea $B'$ una bon de $U=\{v_1,\dots.v_k\}$, la extiendo a una base de $V$ y luego aplico el proceso de ortonormalizacion de gramm-schmidt para convertirla en una bon $B=\{v_1,\dots,v_k,v_{k+1},\dots,v_n\}$

$\{v_{k+1},\dots,v_n\}$ es un conjunto li
$u \in U^{\perp} \implies u \in V \implies u = \sum_{i=1}^n <u,v_i>v_i = \sum_{i=1}^k <u,v_i>v_i + \sum_{i=k+1}^n <u,v_i>v_i$
$=\sum_{i=1}^k 0 \cdot v_i + \sum_{i=k+1}^n <u,v_i>v_i = \sum_{i=k+1}^n <u,v_i>v_i \implies v \in span(\{v_{k+1},\dots,v_n\})$

$v \in span(\{v_{k+1},\dots,v_n\})=u = \sum_{i=k+1}^n <u,v_i>v_i$
$u \in U \implies u = \sum_{i=1}^k <u,v_i>v_i$
$<u,v>=<\sum_{i=1}^k <u,v_i>v_i,\sum_{j=k+1}^n <u,v_j>v_j> =$
$\sum_{i=1}^k \sum_{j=k+1}^n < <u,v_i>v_i, <u,v_j> v_j >$
$\sum_{i=1}^k \sum_{j=k+1}^n <u,v_i><v_j,u> <v_i, v_j >$
$=0 \implies v \in U^\perp$

$U^{\perp}=span(\{v_{k+1},\dots,v_n\})$

$\dim(U)+\dim(U^{\perp})=\dim(V)$