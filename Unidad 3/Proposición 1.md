Sea $V$ un $F$-ev, $\dim_F(V) = n$ y $B = \{v_1, \dots , v_n\}$ base de $V$ . Entonces existe un único
pi $⟨·, ·⟩$ en $V$ tal que la base $B$ es ortonormal respecto de ese pi

$\langle u,v\rangle = [u]_B \cdot [v]_B^*$ es el pi buscado.

Es lineal en la primera variable
	$\langle au+w,v \rangle = [au+w]_B \cdot [v]_B^* = (a[u]_B + [w]_B) \cdot [v]_B^*$
	$=a[u]_B [v]_B^* + [w]_B [v]_B^* = a\langle u,v \rangle + \langle w,v \rangle$
Es simétrico respecto al complemento:
	$\overline{[v]_B \cdot [u]_B^*} = \overline{[v]_B} \cdot [u]_B^t = \left([u]_B \cdot [v]_B^*\right)^t = [u]_B \cdot [v]_B^*$
	La ultima igualdad surge de que $[u]_B \cdot [v]_B^*$ es un escalar
Es definido positivo:
	$\forall z \in \mathbb C: z\cdot \overline z = |z|^2 >0$ si $z \neq 0$
	$([v]_B\cdot[v]_B^*)=\sum_{i=1}^n v_i \cdot \overline{v_i} = \sum_{i=1}^n |v_i|^2 > 0$ si $v \neq 0$

$i \neq j \implies <v_i,v_j> = [v_i]_B \cdot [v_j]_B^* = e_i \cdot e_j^* = 0$
$i=j \implies <v_i,v_i> = [v_i]_B \cdot [v_i]_B^* = e_i \cdot e_i^* = 1$

$B$ es una bon en el pi definido