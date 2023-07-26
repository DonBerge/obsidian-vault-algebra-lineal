Dado $S \subseteq V$, probar que:
$$S = \Span(S)$$
Pruebo por doble inclusión

$S \subseteq \Span(S)$ ya que todo vector $v$ de $S$ es igual a $1\cdot v$ y por lo tanto es una [[Combinacion lineal|combinación lineal]] de vectores de $S$.

Suponiendo que $\Span(S) \nsubseteq S$, existe una combinación lineal de vectores de $S$ que no esta en $S$. Esto invalida la [[Caracterización de un subespacio vectorial|caracterización de un sev]]. Por absurdo, $\Span(S) \subseteq S$.

Por doble inclusión: $S = \Span(S)$