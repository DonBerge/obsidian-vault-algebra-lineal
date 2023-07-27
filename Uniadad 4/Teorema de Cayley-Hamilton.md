Una matriz es anulada por su polinomio característico

Sea $A \in \mathbb F^{n\times n}$, $T(x)=Ax$, $v \in \mathbb F^n$ y $k$ un entero tal que el conjunto $\{v,Tv,T^2v,...T^kv\}$ es li. $\{v,Tv,T^2v,...T^kv,T^{k+1}v\}$ es ld y existen escalares $a_1,...,a_k$ tal que $T^{k+1}=\sum_{i=0}^n a_iT^iv$.

Extiendo el conjunto li a una base de $\mathbb F^n$ $B=\{v,Tv,T^2v,...,T^kv,w_{k+2},...,w_n\}$

Voy a escribir $[T]_B$, para un cierto $i$ dado:
$$[T(T^iv)]_B = [T^{i+1}v] = \begin{cases}
	e_{i+1} & 1 \leq i < k \\
	(a_1,...a_k,0,...0) & i=k
\end{cases}$$
$T^{i+1}v \in \mathbb F^n$, por lo tanto queda:
$$
[T]_B = 
\begin{pmatrix}
	0 & 0 & 0 & \dots & 0 & | & a_0 & |\\
	1 & 0 & 0 &\dots & 0 & | & a_1 & |\\
	0 & 1 & 0 &\dots & 0 & | & a_2 & |\\
	0 & 0 & 1 & \dots & 0 & | & a_3 & | & N\\
	\vdots & \vdots & \vdots & \ddots & \vdots & | & \vdots & |\\
	0 & 0 & 0 & \dots & 1 & | & a_k & |\\
	\hline \\
	\ & \ & 0  & \ & \ & | & 0 & | & M\\
\end{pmatrix}
$$
$$XI-[T]_B = \begin{pmatrix}
	X & 0 & 0 & \dots & 0 & | & -a_0 & |\\
	-1 & X & 0 &\dots & 0 & | & -a_1 & |\\
	0 & -1 & X &\dots & 0 & | & -a_2 & |\\
	\vdots & \vdots & \vdots & \ddots & \vdots & | & \vdots & | & -N\\
	0 & 0 & 0 & \dots & X & | & -a_3 & |\\
	0 & 0 & 0 & \dots & -1 & | & X-a_k & |\\
	\hline \\
	\ & \ & 0  & \ & \ & | & 0 & | & XI_{n-(k+1),n-(k+1)}-M\\
\end{pmatrix}$$
Lema: Si $M \in \mathbb F^{n \times n}$ es una matriz por bloques de la forma $M = \begin{pmatrix}A & B \\ 0 & D\end{pmatrix}$ entonces $\det(M)=\det(A) \cdot \det(D)$
	Suponiendo que $A$ es una matriz $r\times r$.
	Por definición: $\det(M)=\sum_{\sigma \in S_n} sgn(\sigma) \prod_{i=1}^n M_{i\sigma(i)}$
	Donde
	$$M_{i\sigma(i)}=
	\begin{cases} 
	a_{i\sigma(i)} & i\leq r \land \sigma(i) \leq r \\ 
	b_{i,\sigma(i)-r} & i \leq r \land \sigma(i) > r \\ 
	0 & i > r \land \sigma(i) \leq r \\ 
	d_{i-r,\sigma(i)-r} &  i > r \land \sigma(i) > r
	\end{cases}$$
	Si $\sigma(i) > r \land \sigma(i)\leq r$ se tiene que $sgn(\sigma)M_{i\sigma(i)}=0$, por lo que esta permutación no cuenta para el determinante. Así que las permutaciones $\sigma$ que cuentan para el determinante tienen que mandar elementos $>r$ a elementos $>r$. Esto también garantiza que la misma permutación tiene que mandar elementos $\leq r$ a elementos $\leq r$(sino la permutacion puede ser no inyectiva, lo cual es imposible). Asi que las permutaciones $\sigma \in S_n$ se puede representar como una combinación de dos permutaciones $\pi \in S_r$ y $\tau \in S_{n-r}$ donde:
	$$\sigma(i) = \begin{cases}
		\pi(i) & i\leq r\\
		\tau(i-r) & i > r 
	\end{cases}$$
	Respecto al signo de la permutación $\sigma$, la cantidad de transiciones necesarias para representar $\sigma$ es $\text{cantidad de transiciones para }\pi + \text{cantidad de transciciones para }\tau$ por principio de la suma. Así, si $\pi$ y $\tau$ son ambas impares o ambas pares $\sigma$ es par y si una es par y la otra impar entonces $\sigma$ es par por lo tanto $sgn(\sigma) = sgn(\pi) \cdot sgn(\tau)$.
	Luego $\det(M)=\sum_{\sigma \in S_n} sgn(\sigma) \prod_{i=1}^n M_{i\sigma(i)} = \sum_{\sigma \in S_n} sgn(\sigma) \prod_{i=1}^r M_{i\sigma(i)} \prod_{i=r+1}^n M_{i\sigma(i)}$ 
	$=\sum_{\sigma \in S_n} sgn(\pi)\cdot sgn(\tau) \prod_{i=1}^r a_{i\pi(i)} \prod_{i=r+1}^n d_{i\tau(i)}$

s



$\det(XI-[T]_B) = \det\begin{pmatrix} X & 0 & 0 & \dots & 0 & -a_1 \\ -1 & X & 0 & \dots & 0 & -a_2 \\ 0 & -1 & X & \dots & 0 & -a_3\\ \vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & 0 & \dots & X & -a_{k-1} \\ 0 & 0 & 0 & \dots & -1 & X-a_k \\ 0 & 0 & 0 & \dots & 0 & 0 \end{pmatrix} \cdot \det(XI_{n-(k+1),n-(k+1)}-M)$

$\det\begin{pmatrix} X & 0 & 0 & \dots & 0 & -a_1 \\ -1 & X & 0 & \dots & 0 & -a_2 \\ 0 & -1 & X & \dots & 0 & -a_3\\ \vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & 0 & \dots & X & -a_{k-1} \\ 0 & 0 & 0 & \dots & -1 & X-a_k \\ 0 & 0 & 0 & \dots & 0 & 0 \end{pmatrix} \overset{\text{Desarrollo por la k+2-nesima columna}}=\sum_{i=1}^{k+2}(-1)^{k+2+1}$
