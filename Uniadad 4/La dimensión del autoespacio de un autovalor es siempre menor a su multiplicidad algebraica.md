Sea $\lambda$ un autovalor de la matriz $A$ y $r$ su multiplicidad como raíz de $\chi_A$
$$\dim(E_\lambda) \leq r$$
Sea $T(x)=Ax$ una tl de $\mathbb F^n$ a $\mathbb F^n$.

Existe una base $B_\lambda=\{v_1,...,v_s\}$ de $E_\lambda$, extiendo dicha base a una base $B$ de $\mathbb F^n$, se tiene que:
$v_k \in B_{\lambda} \implies Av_k = \lambda v_k \implies T(v_k) = \lambda v_k \implies [T(v_k)]_B = [\lambda v_k]_B = \lambda e_k$

Y resulta:

$$
[T]_B = \begin{pmatrix} 
	\lambda I_s & | & B \\
	\hline 
	0 & | & C
\end{pmatrix}
$$
y
$$
x \cdot I - [T]_B = \begin{pmatrix} 
	(x-\lambda) I_s & | & .B \\
	\hline 
	0 & | & xI_{n-s} - C
\end{pmatrix}$$
Y $\chi_{{[T]}_B}(x) = \det(xI-[T]_B) = (x-\lambda)^{\dim(E_\lambda)} \cdot \det(xI_s - C)$(Desarrollo el determinante por la 1era columna)

$[T]_B \sim A$ por lo que $\chi_{{[T]}_B} = \chi_A$. Dado que es posible que $\det(xI_s - C)$ tenga a $\lambda$ como raiz, resulta $\dim(E_\lambda) \leq r$

