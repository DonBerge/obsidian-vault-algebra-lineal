Sea $A \in \mathbb F^{n\times n}$ y $v=\{v_1,...,v_n\}$ base de $\mathbb F^n$ entonces:
$$m_A = mcm\{m_{v_1},...,m_{v_n}\}$$
Sea $p = mcm\{m_{v_1},...,m_{v_n}\}$.

Lema: $q \in \mathbb F[X], q(v) = 0 \iff m_v | q$
	$\implies$)
		Sea $q$ un polinomio que anula a $v$, por lo que $gr(m_v) \leq gr(q)$
		Por el algoritmo de la división existen polinomios $c,r$ tal que: $q(x)=m_v(x)c(x)+r(x)$
		$q(v)=m_v(v)q(v)+r(v)=r(v) = 0$, $gr(r) \leq gr(m_v)$ por lo que la única opción es que $r(v)=0$(sino $m_v$ no es minimal). Por lo tanto: $m_v | q$
	$\impliedby$)
		$m_v | q \implies \exists c \in \mathbb F[X] : q(x) = m_v(x)c(x) \implies q(v) = m_v(v)c(v) = 0$

$m_A(v) = m_A(A)v = 0$, $m_v | m_A$

Entonces $\forall m_{v_i} : m_{v_i} | m_A$. Por lo que $p | m_A$

Sea $v \in \mathbb F^n$ tal que para ciertos escalares $a_1,...,a_n$: $v= \sum_{i=0}^n a_iv_i$

$p(v) = p(A)v = p(A)\sum_{i=0}^n a_i v_i = \sum_{i=0}^n a_i p(A) v_i = \sum_{i=0}^n a_i p(v_i)$

$m_{v_{i}} | p \implies p(v_i) = 0$, por lo tanto $\sum_{i=0}^n a_i p(v_i) = 0$.
Como $\forall A \in \mathbb F^{n \times n}, p(A)v = 0$ por [[Propiedad cancelativa del producto matricial| la propiedad cancelativa del producto matricial]], $p(A) = 0$. $m_A | p(A)$ y resulta $m_A = p = mcm\{m_{v_1},...,m_{v_n}\}$
