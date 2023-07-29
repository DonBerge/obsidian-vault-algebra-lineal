$\DeclareMathOperator{\Span}{span}$

Sea $A \in \mathbb F^{n\times n}$, a partir del [[Teorema de Cayley-Hamilton]] se tiene lo siguiente:
$gr(m_A) \leq n$)
	Trivial sabiendo que $m_A | \chi_A$
$gr(m_A)=n \implies m_A = \chi_A$)
	A partir de la hipótesis por el algoritmo de la división se tiene que $\chi_A = m_A \cdot q(x) + r(x)$. $gr(q)=0$ y $gr(r)=0$ porque $m_A | \chi_A$ así que existe una constante $\alpha$ tal que $\chi_A = \alpha m_A$. Como $m_A$ es mónico, $\alpha = 1$ y $m_A = \chi_A$.
$\exists v \in \mathbb F^n : gr(m_v) = n \implies m_v = m_a = \chi_a$)
	Si $v=0 \implies gr(m_v) = 0 \neq n$
	Si $v \neq 0$, puedo extender $\{v\}$ a una base de $B$ de $\mathbb F^n$, entonces $m_a = mcm(m_{v_1},...,m_{v_n})$ para $v_i \in B$. Los $m_{v_i}$ con $v_i \neq v$ tienen que ser polinomios constantes $\neq 0$(sino $m_A > n$ lo cual es imposible). Además tienen que ser todos $m_{v_i}=1$ porque sino no serian mónicos, por lo que $mcm(m_{v_1},...,m_{v_n})=m_v=m_A$ y como $gr(m_A)=n$, $m_v=m_A=\chi_A$.
Si $A$ es invertible entonces $A^{-1} \in \Span(I,A,...,A^{n-1})$
	$\chi_A(A)=0$ y $gr(\chi_A) = n$ $\implies$ existen escalares $a_0,...,a_n$ tal que $\chi_A(X)=\sum_{i=0}^n a_i A^i$ 
	$\chi_A(A)=\sum_{i=0}^n a_i A^i=0$
	$A^{-1}\left(\sum_{i=0}^n a_i A^i\right)=A^{-1}\cdot0$
	$\sum_{i=-1}^{n-1} a_{i+1} A^i=\sum_{i=0}^{n-1} a_{i+1} A^i+a_0A^{-1} = 0$
	$\sum_{i=0}^{n-1} a_{i+1} A^i = -a_0A^{-1}$

	$\chi_A(0) = \det(0I-A) = \det(A) = a_0 \neq 0$
	$\sum_{i=0}^{n-1} a_{i+1} A^i = -a_0A^{-1}$
	$\sum_{i=0}^{n-1} \frac{a_{i+1}}{a_0} A^i = A^{-1}$
	$A^{-1} \in \Span(I,A,...,A^{n-1})$
$A$ diagonalizable en $\mathbb F^{n \times n} \iff m_A$ tiene todas sus raices en $\mathbb F$ y son simples
	$\implies$)
		Si $A$ es diagonalizable entonces existe una base $B$ de $\mathbb F^n$ formada por autovectores de $A$.
		$v \in B$ su polinomio minimal es $m_v(X) = X-\lambda \cdot I$ donde $\lambda$ es el autovalor asociado a $v$
		($m_v(v) = m_v(A)v = (A-\lambda I)v = Av-\lambda v = \lambda v - \lambda v = 0$).
		Resulta $m_A = mcm\{m_v : v \in B\}$, $m_A$ es un polinomio con raices simples en $\mathbb F$.
	$\impliedby$)
		