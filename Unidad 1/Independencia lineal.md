Un conjunto finito de vectores $S=\{v_1,v_n\}$ es linealmente independiente o li si y solo si:
$$\forall a_1...a_n \in \mathbb F, \sum_{i=0}^n a_i \cdot v_i = 0 \implies a_i=0$$
El conjunto vacío es li.
Un conjunto infinito es li si todo subconjunto finito del mismo es li
Un conjunto que no es li es linealmente dependiente o ld.

## Propiedades
1) $S \text{ es ld }\iff \exists a_1...a_n \in \mathbb F \text{ donde al menos uno es no nulo } : \sum_{i=0}^n a_i \cdot v_i = 0$
	Viene de la contrarrecíproca de la definición de li
2) $0 \in S \implies S \text{ es ld }$
	Sea $v_n = 0$, $\sum_{i=0}^n a_i v_i = \sum_{i=0}^{n-1} a_i \cdot v_i + a_n \cdot 0$
	Poniendo todos los $a_i$ en 0 y $a_n$ en 1 queda que $\sum_{i=0}^n a_i v_i = 0$ y por lo tanto $S$ es ld.
3) Si $S \text{ es ld } \implies \forall T \supseteq S, \text{T es ld}$
	Dados los escalares $a_1... a_n$ de la combinación lineal de vectores de $S$ que tiene como resultado $0$ donde al menos uno es $\neq 0$(que existen dado que $S$ es ld), la combinación lineal de vectores de $T$ con escalares $a_1...a_n,0...0$ tiene como resultado al vector nulo. Por lo tanto $T$ es ld.
4) Si $S$ es li $\implies \forall T \subseteq S, T$ es li
	Si $T$ fuese ld entonces $S$ no puede ser li(la combinación lineal con escalares $\chi_T(v_i)a_i$ es el vector nulo, $a_i$ es el escalar correspondiente a $v_i$ que hace que la cl de vectores de $T$ sea nula).
5) $v \in V$, $\{v\}$ es ld $\iff v = 0$
	Si $v=0$ entonces $\{v\}$ es ld por uno
	Si $\{v\}$ es ld entonces existe $a \neq 0$ tal que $a\cdot v = 0$ y resulta $v=0$
6) $v,u \in V$, $\{v,u\}$ es ld $\iff \exists \lambda \in \mathbb F : \lambda \neq 0 \cdot u = v$
	Si $\{u,v\}$ es ld existen $a,b$ escalares con al menos uno distinto de 0 tal que $au+bv = 0$.
	Suponiendo que $a\neq 0$, entonces $au = -bv$ y $u = -\frac b a v$, luego $\lambda = -\frac b a$
	En la proposicion contraria: $\lambda u = v \implies \lambda u - v = 0$ y por lo tanto $\{u,v\}$ es ld
7) $S$ es ld $\iff$ existe un vector de $S$ que es cl de los demas
	Suponiendo $S$ ld, $\exists a_k \neq 0 : \sum_{i=0}^n a_i v_i = 0$ y de aca resulta $a_k v_k = \sum_{i=0, i\neq k}^n -a_i v_i$ y finalmente $v_k = \sum_{i=0, i\neq k}^n -\frac{a_i}{a_k} v_i$
	Suponiendo que hay algun vector $v_k$ que es cl de los demas, entonces $v_k = \sum_{i=0, i\neq k}^n a_i v_i$ y finalmente $\sum_{i=0, i\neq k}^n -a_i v_i - v_k = 0$, $S$ es ld