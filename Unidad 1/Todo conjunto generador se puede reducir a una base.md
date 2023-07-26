Si $S$ es un conjunto generador de $V$, se puede reducir a un conjunto li de vectores, y por lo tanto a una base de $V$.

Primero voy a demostrar el siguiente enunciado: Si se tiene que $v \in \Span(S - \{v\}) \implies \Span(S - \{v\}) = \Span(S)$ 

El caso donde $v \notin S$ es trivial, así que voy a probar el caso donde $v \in S$.

Pruebo por doble inclusión, sea $S = \{w_1...w_m\} \cup \{v\}$:
$\Span(S - \{v\}) \subseteq \Span(S)$)
	Si $u \in \Span(S - \{v\}) \implies u = \sum_{i=0}^m a_i w_i = \sum_{i=0}^m a_i w_i + 0\cdot v \implies u \in \Span(S)$
$\Span(S - \{v\}) \supseteq \Span(S)$)
	$v \in \Span(S - \{v\}) \implies v = \sum_{i=0}^m b_i w_i$
	$u \in \Span(S) \implies \sum_{i=0}^m a_i w_i + \beta\cdot v = \sum_{i=0}^m a_i w_i + \beta\cdot \left(\sum_{i=0}^m b_i w_i\right) = \sum_{i=0}^m (a_i+\beta b_i) w_i \implies u \in \Span(S - \{v\})$

Por lo tanto $v \in \Span(S - \{v\}) \implies \Span(S - \{v\}) = \Span(S)$.


Para reducir el conjunto generador a una base se procede como sigue:
Se inicializa el conjunto $S' = S$ y se revisan uno por uno los vectores de $S$:
Suponiendo que se esta viendo el vector $v$
- Si $v \in \Span(S' - \{v\})$, entonces el conjunto pasa a ser $S' = S'-\{v\}$
- Si no se deja $S'$ como esta.
Después de este proceso, $\nexists v \in S' : \Span(S'-\{v\}) = \Span(S')$. El conjunto $S'$ resultante es una base
- Por el enunciado anterior, se cumple que $\Span(S') = \Span(S)$. $S'$ genera a $V$.
- $\nexists v \in S' : \Span(S'-\{v\}) = \Span(S')$ implica que no hay ningún vector de $S'$ que sea combinación lineal de los demás y por lo tanto $S'$ es un conjunto li.