Sea una [[Base de un espacio vectorial|base]] $B=\{v_1,...,v_n\}$ de un espacio vectorial entonces:
$$\forall u \in V, \exists! a_1,...a_n : \sum_{i=0}^n a_i \cdot v_i = u$$
Mas aún, esta implicación es un si y solo si.

$\implies$)
Suponiendo que haya 2 formas de escribir al vector $u$ con vectores de $B$:
$\sum_{i=0}^n a_i v_i = \sum_{i=0}^n {a'}_i v_i = u$
$\sum_{i=0}^n a_i v_i - \sum_{i=0}^n {a'}_i v_i = 0$
$\sum_{i=0}^n (a_i - {a'}_i) v_i = 0$
$a_i - {a'}_i = 0$(esto es debido a que $B$ es un conjunto li)
$a_i = {a'}_i$

$\impliedby$)
Como existe una cl de vectores de $B$ que genera cualquier vector de $U$, $B$ genera a $V$.
Como existe una única forma de generar cada vector de $V$, existe una unica forma de generar el $0$, la trivial con $a_i = 0$ para cada $i$. $B$ es li.
Por lo tanto $B$ es una base.