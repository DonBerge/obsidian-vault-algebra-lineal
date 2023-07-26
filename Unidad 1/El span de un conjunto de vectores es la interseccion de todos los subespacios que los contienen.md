Dado $S$ un conjunto de vectores de $V$ probar que:

$$\Span(S) = \bigcap \{U \text{ sev de } V : S \subseteq U\}$$
Para probar que dos conjuntos son iguales, puedo ver que uno esta contenido en el otro y viceversa, sea $\mathcal F = \{U \text{ sev de } V : S \subseteq U\}$:

$\Span(S) \subseteq \bigcap \{U \text{ sev de } V : S \subseteq U\}$)
	Sea un $U \in \mathcal F$ y $v \in \Span(S)$,
	$v = \sum_{i=0}^n a_i w_i$ con $a_i$ un escalar y $w_i \in S$
	$w_i \in U$ y $U$ es un sev de $V$ por ser [[Axiomas de los espacios vectorial |la suma una operación cerrada en U]], $v \in U$. Dado que $U$ es un conjunto cualquiera de $\mathcal F$ y $v$ un vector cualquiera del span, se cumple que $\Span(S) \subseteq \bigcap \{U \text{ sev de } V : S \subseteq U\}$
$\Span(S) \supseteq \bigcap \{U \text{ sev de } V : S \subseteq U\})$
	$span(S) \in \mathcal F$, [[El span de un conjunto es un subespacio vectorial| el span de S es un sev de V]] y además $S \subseteq \Span(S)$ debido a que un vector $v \in S$ se puede escribir como $1 \cdot v$ que es una [[Combinacion lineal|cl]] de vectores de $S$. Debido a esto cualquier vector de  $\bigcap \{U \text{ sev de } V : S \subseteq U\})$ tiene que estar en $\Span S$ por lo que la proposición se cumple.

Al cumplirse la doble inclusión, se cumple la proposición a probar. Esto tambien demuestra que $\Span(S)$ es el menor sev de $V$ que contiene a todos los elementos de $S$.
