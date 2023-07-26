Si $V$ es un ev con dimension $n$, entonces es isomorfo a $F^n$

$E=\{e_1,...,e_n\}$ es una base de $F^n$($(e_i)_j = \delta_{i,j}$)
Dada una base $B=\{v_1,...,v_n\}$ de $V$, defino las siguientes tls

$T: V \to F^n$
$T(v_i) = e_i$

$S: F^n \to V$
$S(e_i) = v_i$

Se tiene que para $u \in F^n$ y $v \in V$:
$T(S(u)) = T(S(\sum_{i=0}^n a_i e_i))=T(\sum_{i=0}^n a_i v_i) = \sum_{i=0}^n a_i e_i = u$
$S(T(v)) = S(T(\sum_{i=0}^n a_i v_i)) = S(\sum_{i=0}^n a_i e_i) = \sum_{i=0}^n a_i v_i = v$

$T$ es inversa de $S$ y viceversa, ambas son biyectivas y por lo tanto $V \overset{T}{\simeq} F^n$
