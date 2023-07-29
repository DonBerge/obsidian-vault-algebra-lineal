Si $T \in L(V)$ es $k$ pasos nilpotente($T^k=0$) entonces
$$ \{0\} \subset \ker(T) \subset \ker(T^2) \subset \dots \subset \ker(T^k) = V$$
$\ker(T^k) = \ker(\{0\}) = V$
$\ker(T^i) \subset \ker(T^{i+1})$)
	$v \in \ker(T^i) \implies T^i(v) = 0 \implies T(T^i(v)) = T(0) \implies T^{i+1}(v) = 0 \implies v \in \ker(T^{i+1})$
	Suponiendo que $\ker(T^i) = \ker(T^{i+1})$:
		$v \in \ker(T^{i+2})$
		$\implies$
		$T^{i+2}(v) = 0$
		$\implies$
		$T^{i+1}(T(v)) = 0$
		$\implies$
		$T(v) \in \ker(T^{i+1})$
		$\implies$
		$T(v) \in \ker(T^i)$
		$\implies$
		$T^i(T(v))=0$
		$\implies$
		$T^{i+1}(v) = 0$
		$\implies$
		$v \in \ker(T^{i+1})$
		$\begin{rcases}\ker(T^{i+2}) \subseteq \ker(T^{i+1}) \\ \ker(T^{i+1})\subseteq \ker(T^{i+2})\end{rcases} \implies \ker(T^i) = \ker(T^{i+1}) = \ker(T^{i+2})$
		Por lo que
		$$\ker(T^i) = \ker(T^{i+1}) = \ker(T^{i+2}) = \dots = \ker(T^k) = V$$
		$T^i = 0$, asi que $T$ es $i<k$ pasos nilpotente, absurdo.
		$\ker(T^i) \neq \ker(T^{i+1}) \implies \ker(T^i) \subset \ker(T^{i+1})$
