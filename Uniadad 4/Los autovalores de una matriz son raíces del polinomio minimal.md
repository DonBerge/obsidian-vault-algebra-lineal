Sea $A \in \mathbb F^{n\times n}$ y $\lambda \in \mathbb F$
$$\lambda \text{ autovalor de } A \iff \lambda \text{ es raiz de } m_A$$
$\implies$)
	Por el algoritmo de la division, existen $Q(X)$ y $R(X)$ polinomios en $\mathbb F$ tal que $m_A(X) = (X - \lambda I)Q(X) + R(X)$. $0 \leq gr(R) < gr(X-\lambda I)$ por lo que $R(X)=rI$ es un polinomio constante 
	$m_A(A) = (A-\lambda I)Q(X) + rI = 0$
	Sea $v$ un autovector asociado a $\lambda$
	$(A-\lambda I)Q(X) + rI = 0$
	$((A-\lambda I)Q(X) + rI)v = 0v = 0$
	$((A-\lambda I)Q(X) + rI)v = (A-\lambda I)Q(X)v + rIv = (Av-\lambda Iv)Q(X) + rIv = (\lambda v-\lambda v)Q(X) + rv = rv$
	$rv = 0$, como $v\neq 0$ por ser un autovector resulta $r=0$ y por lo tanto $(X - \lambda I) |m_A(X)$. $\lambda$ es raíz de $m_A$

$\impliedby$)
	Como $m_A$ tiene a $\lambda$ como raíz, $m_A(X) = (X-\lambda I)C(X)$ con $C(X)$ un polinomio de grado menor a $m_A$. Por lo que $m_A(A) = (A-\lambda I)C(A) = 0$. $C(A)\neq 0$ por ser un polinomio de menor grado al minimal. Esto implica que existe un vector $w$ tal que $C(A)\cdot w = v \neq 0$.
	$(A-\lambda I)C(A) \cdot w = 0\cdot w$
	$(A-\lambda I)v = 0$
	$v$ es un autovector de $A$ asociado al autovalor $\lambda$. $\lambda$ es un autovalor de $\lambda$