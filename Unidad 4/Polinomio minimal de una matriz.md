Sea $A \in \mathbb F^{n\times n}$, existe un unico polinomio $p$ con coeficientes en $\mathbb F$ que anula a $A$, es monico y tiene grado minimo. 

[[Siempre existe un polinomio que anula a una matriz dada]], sea $H_A = \{gr(p) : p(A) = 0\}$(el conjunto formado por los grados de los polinomios que anulan a $A$). $H_A$ es no vacio y es un subconjunto de $\mathbb N$ acotado inferiormente, por lo que tiene un elemento minimo. Sea $q(x)$ un polinomio que anula a $A$ y $gr(q) = \min H_A$ y $\alpha$ su coeficiente principal, el polinomio $h(x) = \frac{q(x)}\alpha$ es el polinomio monico y de grado minimo buscado.

Para probar unicidad, suponiendo que hay 2 polinomios $q(x)$ y $q'(x)$ que cumplen lo pedido, se tiene que los 2 tienen el mismo grado. Sea $r$ el grado de los mismos, el polinomio $h(x)=q(x)-q'(x)$ tiene grado $r-1>0$ y $h(A)=q(A)-q(A') = 0$, lo cual es absurdo porque $q$ es el polinomio de menor grado que cumple lo pedido. Por lo tanto $q(x) = q'(x)$.

El polinomio $q$ se denomina polinomio minimal de $A$ y se denota $m_A$