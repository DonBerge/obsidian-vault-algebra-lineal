Dado un vector $v$ de $V$ y $B_1=\{v_1,...,v_n\}$, $B_2=\{w_1,...,w_n\}$ dos bases de $V$:

$$\exists C \in F^{n\times n}, C_{i,j} = ([v_j]^t_{B_2})_i : C [v]^t_{B_1} = [v]^t_{B_2}$$

Defino: 
$a_i := \left([v]^t_{B_1}\right)_i$
$c_{i,j} = C_{i,j}$
$b_{i} = (C [v]^t_{B_1})_{i} = \sum_{k=0}^n c_{i,k} a_{k}$

$\sum_{i=0}^n b_{i}w_i = \sum_{i=0}^n \sum_{k=0}^n c_{i,k} a_{k} w_i = \sum_{k=0}^n a_{k} \sum_{i=0}^n c_{i,k} w_i = \sum_{k=0}^n a_k v_k = v$

$(C [v]^t_{B_1})_{i} = ([v]^t_{B_2})_i$

## La matriz de cambio de base es única

Suponiendo que existen 2 matrices $C$ y $C'$ que cumplen que:

$$\forall v \in V: C [v]^t_{B_1} = C' [v]^t_{B_1}$$
$C=C'$ por la [[Propiedad cancelativa del producto matricial|propiedad cancelativa del producto matricial]]

## Propiedades adicionales
$C_{B_1B_2}:=$ la matriz de cambio de base entre 2 bases $B_1$ y $B_2$ de $V$

1) $C_{B_1B_3}=C_{B_2B_3}C_{B_1B_2}$
	$C_{B_2B_3}C_{B_1B_2} \cdot [v]^t_{B_1} = C_{B_2B_3} \cdot [v]^t_{B_2} = [v]^t_{B_3}$
	La igualdad se cumple debido a que la matriz de cambio de base es única
2) $C_{B_2B_1} = (C_{B_1B_2})^{-1}$
	La matriz de cambio de base es invertible debido a que todo vector de coordenadas en una base se puede reescribir de manera única en otra base con otras coordenadas(El sistema $C_{B_2B_1}x = [v]^t_{B_1}$ tiene una única solución).
	Después se tiene que:
	$[v]^t_{B_1} = I [v]^t_{B_1} = C_{B_2B_1}C_{B_1B_2}[v]^t_{B_1}$
	$I = C_{B_2B_1}C_{B_1B_2}$
	$(C_{B_1B_2})^{-1} = C_{B_2B_1}$
3) Toda matriz invertible es una matriz de cambio de base, $\forall A \in F^{n\times n} \text{ invertible }, \exists B_1,B_2 \text{ bases de } V : A = C_{B_1B_2}$
	$A$ invertible implica que ninguna de sus columnas es cl de la otra(de lo contrario, $\det(A)=0$), las columnas de $A$ forman un conjunto li de $n$ vectores(y por lo tanto un conjunto generador y base). Sea $B$ la base que forman y $E$ la base canónica de $F^n$, $A = C_{BE}$
4) Para una matriz invertible y una base $B=\{v_1,...,v_n\}$, existe otra base $B'=\{w_1,...,w_n\}$ tal que $A = C_{BB'}$
	Defino la tl $T(v_i) = \sum_{k=0}^n A_{k,i}v_k$, $T$ es un isomorfismo
	$T(v) = \sum_{k=0}^n A_{k,i}v_k = 0 \iff \forall k, A_{k,i} = 0 \lor v=0$
	$\forall k, A_{k,i} = 0$ es falso porque $A$ es invertible, $v=0$ y $T$ es un monomorfismo

	Defino ahora $w_i = T(v_i)$,
	Dado que $T$ es un monomorfismo, preserva aquellos conjuntos que son li, $B=\{v_1,...,v_n\}$ es li por lo tanto $B'=\{T(v_1),...,T(v_n)\}$ es un conjunto li.

	$\dim(Im(T)) \ngtr n \land \dim(Im(T)) \geq n$, por lo tanto $\dim(Im(T)) = n$ y $Im(T) = V$, $T$ es un epimorfismo.

	$T$ resulta ser un isomorfismo de $V \to V$, por lo que preserva las bases, $B'$ es una base de $V$
	$[v_i]_{B'} = \{A_{1,i},...,A_{n,i}\}$, $A$ es la matriz de cambio de base entre $B$ y $B'$

5) Para una matriz invertible y una base $B = \{v_1,...,v_n\}$ existe otra base $B' = \{w_1,...,w_n\}$ tal que $A = C_{B'B}$
	$w_i := \sum_{j=0}^n A_{j,i}v_j$
	$B'$ es una base:
	$\sum_{i=0}^nb_i w_i = 0 \iff \sum_{i=0}^n \sum_{j=0}^n b_i A_{j,i}v_j = 0 \iff \sum_{j=0}^n (\sum_{i=0}^n b_i A_{j,i})v_j = 0 \iff$
	$\forall j,\sum_{i=0}^n b_i A_{j,i} = 0 \iff \forall b_i = 0$(de lo contrario, las columnas de $A$ son ld y $A$ no es invertible)
	
	$B'$ es un conjunto li, al tener cardinal $n$ y ser $\Span(B) \subseteq V$, $B$ es un conjunto generador y por lo tanto una base.

	Luego, $A$ es la matriz de cambio de base entre $B'$ y $B$ 