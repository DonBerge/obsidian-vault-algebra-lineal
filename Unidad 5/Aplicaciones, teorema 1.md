$V$ un $\mathbb F$-ev con pi, $\dim(V ) = n, T ∈ L(V )$. Son equivalentes:
1. Existe $B$ bon de $V$ tal que $T(B)$ bon de $V$ .
2. $\forall v, u ∈ V$ , $<T(v), T(u)>$ = $<v, u>$.
3. $\forall B$ bon de $V$ , $T(B)$ bon de $V$
4. $\forall v ∈ V$ , $||T(v)|| = ||v||$
5. $T^* \circ T = T \circ T^* = Id_V$

$1 \implies 2$) 
	Sea $B=\{u_1,\dots,u_n\}$ bon de $V$ tal que $T(B)$ es bon de $V$
	$v = \sum_{i=1}^n a_i v_i$
	$w=\sum_{j=1}^n b_j v_j$
	$<v,w> = \left\langle \sum_{i=1}^n a_i v_i, \sum_{j=1}^n b_j v_j \right\rangle = \sum_{i=1}^n \sum_{j=1}^n a_i \overline{b_j} <v_i,v_j>$
	$=\sum_{i=1}^n a_i \overline{b_j} ||v_i||^2 = \sum_{i=1}^n a_i \overline{b_j}$
	$<T(v),T(w)> = \left\langle \sum_{i=1}^n a_i T(v_i), \sum_{j=1}^n b_j T(v_j) \right\rangle$
	$=\sum_{i=1}^n a_i \overline{b_j} = <v,w>$
$2 \implies 5$)
	$<v,u>=<T(v),T(u)> = <v,T^*(T(u))>$
	$<v,u-T^*(T(u))=0$
	Tomando $v=u-T^*(T(u))$:
	$||u-T^*(T(u))|| = 0$
	$u = T^*(T(u))$
	$T^* \circ T = Id_V$
	$(T^* \circ T)^* = Id_V^*$
	$T \circ T^* = Id_V$
	Se cumple $(5)$
$5 \implies 4)$
	$||T(v)|| = \sqrt{\langle T(v),T(v) \rangle} = \sqrt{\langle v, (T^* \circ T)(v) \rangle}$
	$=\sqrt{\langle v,v \rangle} = ||v||$
	Se cumple (4)
$4 \implies 3$)
	Sea $B=\{u_1,\dots u_n\}$ una bon de $V$
	$T(B)$ es un conjunto normalizado
	$T$ es un isomorfismo:
	Si $T(v) = 0$ entonces: 
	$0=||T(v)||=||v||$
	$v=0$
	$\ker(T) = \{0\}$, $T$ es un monomorfismo y un endomorfismo. Por lo tanto $T$ es un isomorfismo.
	Como $T$ es un isomorfismo, $T$ preserva bases
	Por las identidades de polarización
	$||u_i+i u_j|| = ||T(u_i+iu_j)|| = ||T(u_i)+iT(u_j)$
	Sea $i\neq j$:
	$0 = <u_i,u_j> = 1/4 ||u_i+u_j||^2 - 1/4 ||u_i-u_j||^2 + i/4 ||u_i+iu_j|| - i/4 ||u_i-iu_j||$
	$=1/4 ||T(u_i)+T(u_j)||^2 - 1/4 ||T(u_i)-T(u_j)||^2 + i/4 ||T(u_i)+iT(u_j)|| - i/4 ||T(u_i)-iT(u_j)||$
	$=<T(u_i),T(u_j)>$
	$T(B)$ es una bon
	Se cumple $(3)$
$3 \implies 1$)
	Trivial
 