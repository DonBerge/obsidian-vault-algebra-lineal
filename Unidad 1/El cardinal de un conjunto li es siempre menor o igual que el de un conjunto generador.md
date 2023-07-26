
Dado $V$ un espacio vectorial finito. Sea $S$ un conjunto li de vectores de $V$ y $T$ un conjunto generador de $V$, $|S| \leq |T|$

Suponiendo $S=\{u_1,...,u_n\}$ y $T = \{v_1,...,v_n\}$, los vectores de S se pueden escribir como cl de vectores de $T$

$$u_1 = a_{11}v_1 + a_{12}v_2 + ... + a_{1n}v_n$$
$$u_2 = a_{21}v_1 + a_{22}v_2 + ... + a_{2n}v_n$$
$$.$$
$$.$$
$$.$$
$$u_m = a_{m1}v_1 + a_{m2}v_2 + ... + a_{mn}v_n$$
Sea el sistema:

$$\begin{pmatrix}
	a_{11} & . & a_{n1} \\
	. & . & . \\
	a_{1m} & . & a_{nm}
\end{pmatrix} \cdot \begin{pmatrix}x_1 \\ . \\ x_n\end{pmatrix} = \begin{pmatrix}0 \\ . \\ 0\end{pmatrix}$$
Sea $(b_1,.,b_n)$ una solución del sistema, esto quiere decir que:
$$a_{11}b_1 + a_{21}b_2 + ... + a_{n1}b_n = 0$$
$$a_{12}b_1 + a_{22}b_2 + ... + a_{n2}b_n = 0$$
$$.$$
$$.$$
$$.$$
$$a_{1m}b_1 + a_{2m}b_2 + ... + a_{nm}b_n = 0$$
Y en general: $\sum_{i=0}^n b_i a_{ij} = 0$

Se tiene que:
$\sum_{i=0}^m b_i u_i =\sum_{i=0}^n b_i \left(\sum_{j=0}^n a_{ij}v_j\right) = \sum_{i=0}^n \sum_{j=0}^n b_i \cdot a_{ij} \cdot v_j =\sum_{j=0}^n \sum_{i=0}^n b_i \cdot a_{ij} \cdot v_j = \sum_{j=0}^n v_j \cdot \left(\sum_{i=0}^n b_i \cdot a_{ij}\right) = 0$

Como los vectores $u$ son li, los coeficientes $b$ tienen que ser todos 0 por lo que el sistema anterior tiene una única solución. Dado que no hay variables libres se tiene que hay mas columnas que filas y resulta $m\leq n$. $|S| = m$ y $|T| = n$, el conjunto li tiene menos elementos que el conjunto generador.

## Corolarios

Sea $S$ un conjunto de vectores de $V$ y $B$ una [[Base de un espacio vectorial|base]] de $V$ 

1) $|S| > |B| \implies S$ es ld
	Si $S$ fuera li entonces $|S| \leq |B|$ debido a que $B$ es un conjunto generador, lo cual es una contradicción.
2) Si $|S| < |B| \implies S$ no genera a $V$
	Si $S$ generara a $B$, entonces $|S|\geq |B|$ debido a que $B$ es li. Contradicción
3) Todas las bases tienen la misma cardinalidad
	Dadas dos bases $B_1$ Y $B_2$ de $V$:
	$B_1$ es li y $B_2$ es generador, $|B_1| \leq |B_2|$
	$B_2$ es li y $B_1$ es generador, $|B_1|\leq |B_2|$
	De aqui sale que $|B_1| = |B_2|$.