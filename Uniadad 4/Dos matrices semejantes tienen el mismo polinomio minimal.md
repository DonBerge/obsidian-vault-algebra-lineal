Sean $A,B \in \mathbb F^{n\times n}$ con $A \sim B$ entonces $m_A = m_B$

Lema 1: $p \in \mathbb F[x], p(A) = 0 \iff m_A | p$
$\implies$)
	p anula a A, $gr(m_a) \leq gr(p)$(sino $m_a$ no tendria grado mínimo) por el algoritmo de la division existen polinomios $q$ y $r$ donde $p(x)=q(x)m_A(x)+r(x)$, $p(A)=q(A)m_A(A)+r(A) = r(A) = 0$. Luego $r(x)=0$(sino $r$ tendria menor grado que el minimal). $m_a | p$.
$\impliedby$)
	$m_A|p$, por lo que existe $q$ tal que $p(x)=q(x)m_A(x)$ y $p(A)=q(A)m_A(A)=0$

Lema 2: $A \sim B \implies p(A) \sim p(B)$:
	$A \sim B \implies \exists C \in \mathbb F^{n\times n}$ invertible $: A = CBC^{-1}$
	$p(X) = \sum_{i=0}^{gr(p)} \alpha_i X^i$
	$p(A) = \sum_{i=0}^{gr(p)} \alpha_i A^i = \sum_{i=0}^{gr(p)} \alpha_i ({CBC^{-1}})^i$
	$(CBC^{-1})^i = CB^iC^{-1}$
	Por inducción en $i$:
	CB) $i=0$
		$(CBC^{-1})^0 = I = C C^{-1} = C I C^{-1} = C B^0 C^{-1}$
	HI) $(CBC^{-1})^i = CB^iC^{-1}$
	PI) 
		$(CBC^{-1})^{i+1} = (CBC^{-1})^{i}CBC^{-1} \overset{HI}= CB^iC^{-1}CBC^{-1} = CB^{i+1}C^{-1}$
		$\sum_{i=0}^{gr(p)} \alpha_i ({CBC^{-1}})^i = \sum_{i=0}^{gr(p)} \alpha_i CB^iC^{-1} = C\left(\sum_{i=0}^{gr(p)} \alpha_i B^i\right)C^{-1} = Cp(B)C^{-1}$
	$p(A) \sim p(B)$

Lema 3: $A \sim B \implies p(A) = 0 \iff p(B)=0$
	Por lema 2:
	$p(A) = Cp(B)C^{-1}$
	$0 = Cp(B)C^{-1}$
	$0 = p(B)$
	La reversa se prueba igual.

$m_A(A) = 0 \overset{\text{Lema 3}}\iff m_A(B) = 0 \overset{Lema 1}{\iff} m_B | m_A$
$m_B(A) = 0 \overset{\text{Lema 3}}\iff m_B(B) = 0 \overset{Lema 1}{\iff} m_A | m_B$

$m_A = q_1 m_B$
$m_B = q_2 m_a$

$m_A = q_1 m_B = q_1 q_2 m_A \implies q_1 q_2 = 1 \implies q_1 = q_2^{-1}$

$q_1$ y $q_2$ tienen grado 1(son escalares), como ambos minimales son monicos la única opción posible es que $q_1 = 1$ y $q_2 = 1^{-1} = 1$ por lo que $m_A = m_B$