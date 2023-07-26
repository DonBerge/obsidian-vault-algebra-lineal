Sean $U_1$ Y $U_2$ subespacios vectoriales de $V$
$$\dim U_1 + \dim U_2 - \dim U_1 \cap U_2 = \dim U_1 + U_2$$
Dada una base $B$ de $U_1 \cap U_2$, la extiendo a una base $B_1$ de $U_1$ y a una base $B_2$ de $U_2$ de aquí resulta:

$|B| = m$
$|B_1| = m +r$
$|B_2| = m + s$
$B = \{v_1,...,v_{m}\}$
$B_1 = \{u_1,...,u_{m+r}\}$
$B_2 = \{w_1,...,w_{m+s}\}$

Luego $B_1 \cup B_2$ es una base de $U_1 + U_2$:

$v \in \Span(B_1 \cup B_2) \iff v = \sum_{i=0}^{m+r} a_i \cdot u_i  + \sum_{i=0}^{m+s} b_i \cdot w_i \iff v \in U_1 + U_2$

Ahora planteo:
$\sum_{i=0}^{m} a_i\cdot v_i + \sum_{i=m+1}^{r} b_i \cdot u_i + \sum_{i=0}^{s} c_i \cdot w_i = 0$
$-\sum_{i=0}^{m} a_i\cdot v_i -\sum_{i=m+1}^{r} b_i \cdot u_i = \sum_{i=0}^{s} c_i \cdot w_i$
La parte izquierda que pertenece a $U_1$ es igual a la parte derecha que pertenece a $U_2$
por lo tanto ambas pertenecen a $U_1 \cap U_2$

La parte izquierda entonces se puede escribir como cl de vectores de $B_1 \cap B_2$ por lo que:
$-\sum_{i=0}^{m} a_i\cdot v_i -\sum_{i=m+1}^{r} b_i \cdot u_i = \sum_{i=0}^m d_i v_i = \sum_{i=0}^{s} c_i \cdot w_i$
$\sum_{i=0}^m d_i v_i + \sum_{i=0}^{s} -c_i \cdot w_i = 0$
Me quedaron todos vectores de $B_2$, como $B_2$ es li, resulta que $c_i=0$ y $d_i=0$ $\forall i$ 

Como $-\sum_{i=0}^{m} a_i\cdot v_i -\sum_{i=m+1}^{r} b_i = \sum_{i=0}^m d_i v_i = 0$, $a_i=0$ y $b_i=0$ $\forall i$ dado que $B_1$ es un conjunto li.

Queda entonces que $B_1 \cup B_2$ es base de $U_1 \cap U_2$ y finalmente:

$|B_1 \cup B_2| = |B_1| + |B_2| - |B_1 \cap B_2| = |B_1| + |B_2| - |B|$
$\dim U_1 + U_2 = \dim U_1 + \dim U_2 - \dim U_1 \cap U_2$