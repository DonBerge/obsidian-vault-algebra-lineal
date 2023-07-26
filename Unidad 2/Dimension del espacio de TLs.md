Sea $V$ un ev con $\dim V = n$ y $W$ un ev con $\dim W$:
$$\dim(L(V,W)) = nm$$
Dada $B_V = \{v_1,...,v_n\}$ base de $V$ y $B_W=\{w_1,...,w_n\}$ base de $W$.

[[Una tl queda determinada por los valores que asume en una base]], así que defino las tls
$E_{i,j}(v_k)=\delta_{i,k}w_j$
Estas tls asignan el vector $v_i$ al vector $w_j$ y todos los demás $v$ son asignados al vector nulo.

El conjunto $B=\{E_{i,j} : 0 \leq i \leq n, 0 \leq j \leq m\}$ es una base de $L(V,W)$:

$\Span(B) \subseteq L(V,W)$
$T \in L(V,W) \implies T$ esta definida para cada vector $v_k$

$T(v_k) = \sum_{j=0}^m a_{k,j}w_j = \sum_{j=0}^m \left(\sum_{i=0}^n \delta_{i,k} a_{i,j}\right)w_j = \sum_{j=0}^m \sum_{i=0}^n a_{i,j} \delta_{i,k} w_j = \sum_{j=0}^m \sum_{i=0}^n E_{i,j}(v_k)$

$T \in \Span(B)$

$B$ es un conjunto li de vectores:

Sea una cl de B tal que $T=\sum_{j=0}^m \sum_{i=0}^n a_{i,j}E_{i,j} = 0$(la tl nula), T es nula para todo vector de $V$:
$T(v_k)=\sum_{j=0}^m \sum_{i=0}^n a_{i,j} E_{i,j}(v_k) = \sum_{j=0}^m \sum_{i=0}^n a_{i,j} \delta_{i,k}w_j = \sum_{j=0}^m a_{k,j} w_j = 0 \iff \forall a_{k,j}, a_{k,j} = 0$ 

$k$ asume valores en $[[0,n]]$ y $j$ asume valores en $[[0,m]]$ de modo que las tls $E_{ij}$ son todas li. 