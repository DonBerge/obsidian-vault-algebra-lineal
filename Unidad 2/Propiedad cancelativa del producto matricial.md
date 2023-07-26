Dadas dos matrices $A,A' \in \mathbb F^{n \times n}$:
$$\forall x \in \mathbb F^n : Ax = A'x \iff A=A'$$
$\implies$)
	$Ax = A'x \implies (A-A')x = 0$
	$A \neq A' \implies$ Existe una columna de $A-A'$ que no es nula, suponiendo que la $i$-esima columna cumple esta propiedad entonces $(A-A')\cdot e_i \neq 0$
	Por reducción al absurdo debe ser $A-A'=0$ y por lo tanto $A=A'$.
$\impliedby)$
	Trivial