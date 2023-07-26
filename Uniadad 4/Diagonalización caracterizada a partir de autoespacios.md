Sea $A \in \mathbb F ^{n\times n}$ y $\lambda_1,...\lambda_r$ autovalores distintos de $A$, son equivalentes:

1) $A$ es diagonalizable
2) $\bigoplus_{i=0}^n E_{\lambda_i} = \mathbb F^n$
3) $\chi_A(x) = \sum_{i=0}^n (x-\lambda_i)^{a_i}$ con $a_i = \dim(E_{\lambda_i})$

$1 \implies 2$)
	Si $A$ es diagonalizable existe una base $B$ de $\mathbb F^n$ formada por autovectores de $A$, de modo que algún autovector de la base tiene asociado un autovalor por lo que $\forall v \in B \exists \lambda : v \in E_{\lambda}$ y dado que $B$ es una base de ${\mathbb {F}}^{n}$ y [[El span de un conjunto de vectores es la interseccion de todos los subespacios que los contienen |el menor sev que contiene a todos los vectores de B es su span]], resulta $\mathbb F^n = \Span(B) \subseteq \sum_{i=0}^n E_{\lambda_i}$. Como todos los $v \in \mathbb F^n$, $\sum_{i=0}^n E_{\lambda_i} \subseteq \mathbb F^n$ y resulta $\mathbb F^n = \sum_{i=0}^n E_{\lambda_i}$. El hecho de que [[Los autoespacios se suman de manera directa|los autoespacios se sumen de manera directa]] implica que $\mathbb F^n = \bigoplus_{i=0}^n E_{\lambda_i}$.
$2 \implies 3$) 
	$\bigoplus_{i=0}^n E_{\lambda_i} = \mathbb F^n$. Como se suman de manera directa [[Dimensión de la suma de espacios vectoriales|la dimensión de la suma de dichos autoespacios]] es $n$.

	[[La dimensión del autoespacio de un autovalor es siempre menor a su multiplicidad algebraica]], por lo que $\sum_{i=0}^n \dim{E_{\lambda_i}} \leq \sum_{i=0}^n \text{mul}_{\chi_A}(\lambda_i) = n$(el grado del polinomio caracteristico es n)
	Por lo tanto se tiene que los polinomios $\sum_{i=0}^n (x-\lambda_i)^{\dim(\lambda_i)}$ y $\sum_{i=0}^n (x-\lambda_i)^{\text{mul}_{\chi_A}(\lambda_i)}=\chi_{A}$ son iguales. (3) se cumple
$3 \implies 1)$
	Sea $B_i$ una base del autoespacio $E_{\lambda_i}$ y $B = \bigcup_{i=0}^r B_i$, $B$ es una base de $\mathbb F^n$ formada por autovectores de $A$,
	$B$ es un conjunto li: Dados dos ev $U$ y $V$, si $U \cap V = \{0\} \implies B_U \cup B_V$ es li donde $B_U$ es una base de $U$ y $B_V$ una base de $V$. 
	Sea $0 = \sum_{i=0}^s a_i u_i + \sum_{i=0}^r b_i u_i$ con $a_i,b_i \in \mathbb F$, $u_i \in U$ y $v_i \in V$ de aquí sigue que:
	$\sum_{i=0}^s a_i u_i = -\sum_{i=0}^r b_i u_i = w$, $w \in U \cap V$ por hipótesis resulta $w=0$
	$0 = \sum_{i=0}^s a_i u_i \iff a_i = 0 \forall i$
	$0 = \sum_{i=0}^r b_i u_i \iff b_i = 0 \forall i$
	$B_U \cup B_V$ es li.
	La suma de las dimensiones resulta ser $n$(por ser este el grado del polinomio característico) y como $E_i \subseteq \mathbb F^n$, la suma de los autoespacios es también un sev de $\mathbb F^n$. Por lo que $B$ es un conjunto generador de $\mathbb F^n$ li formado por autovectores de $A$. $A$ es diagonalizable.
