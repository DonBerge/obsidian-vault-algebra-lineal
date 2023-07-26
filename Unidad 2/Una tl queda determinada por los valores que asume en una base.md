Dada una base $B=\{v_1,...,v_n\}$ y un conjunto de vectores $B' = \{w_1,...,w_n\}$ de un ev $V$: $\exists! T:V\to W : T(v_i) = w_i \forall i \in [[1,n]]$

Primero voy a probar que existe dicha tl:
Dado un vector $v$ de $V$, este se puede escribir de una única forma como:
$v=\sum_{i=0}^n a_iv_i$, $a_i$ son valores escalares.

$T: V \to W$
$T(\sum_{i=0}^n a_iv_i) = \sum_{i=0}^n a_iT(v_i)$ es una tl

$T(\lambda\sum_{i=0}^n a_iv_i + \sum_{i=0}^n b_iv_i) = T(\sum_{i=0}^n (\lambda a_i + b_i)v_i)=\sum_{i=0}^n(\lambda a_i + b_i)T(v_i) = \sum_{i=0}^n(\lambda a_iT(v_i) + b_iT(v_i))$
$=T(\lambda\sum_{i=0}^n a_iv_i) + T(\sum_{i=0}^n b_iv_i) = \lambda T(\sum_{i=0}^n a_iv_i) + T(\sum_{i=0}^n b_iv_i)$

$T$ es la única transformación lineal que cumple con el enunciado, suponiendo que existe otra tl $\overline{T}(v)$ que cumple lo mismo

$T(\sum_{i=0}^n a_iv_i) = \sum_{i=0}^n a_iT(v_i) = \sum_{i=0}^n a_i\overline T(v_i) = \overline T(\sum_{i=0}^n a_i v_i)$

Por principio de extensionalidad queda que $T = \overline T$