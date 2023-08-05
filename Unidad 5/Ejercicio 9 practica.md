Sea $V$ un espacio vectorial y sea $v \in V$. Entonces $v$ induce una aplicación $L_v: V^* \to \mathbb F$ definida por
$$L_v(f) = f(v)$$
$L_v$ es lineal)
	$f,g \in V^*$
	$a,b \in \mathbb F$
	$L_v(af+bg)=(af+bg)(v)=af(v)+bg(v) = aL_v(f)+bL_v(g)$
Si $V$ es de dimensión finita y $v \neq 0$ entonces existe $f \in V^*$ tal que $f(v) \neq 0$)
	Sea $B=\{v,u_1,u_2,\dots,u_{n-1}\}$ una base de $V$ que incluye a $v$, existe una base de $V^*=\{\varphi_v,\varphi_1,\varphi_2,\dots,\varphi_{n-1}\}$ donde $\varphi_v(w) =\begin{cases} 1 & w = v \\ 0 & w \neq v \end{cases}$   y $\varphi_i(w)=\begin{cases} 0 & w = v \\ 1 & w=v_i \\ 0 & w \neq v \land w \neq v_i\end{cases}$
	 $\varphi_v \in V^*$ y $\varphi_v(v) \neq 0$, la afirmación es verdadera.
Si $V$ es de dimensión finita, la aplicación $\Omega(v) = L_v$ es un isomorfismo de $V$ en $V^{**}$)
	$\ker(\Omega)=\{v \in V : \Omega(v) = 0\} = \{v \in V : \Omega(v) = 0\}$ ($0$ es la transformación nula)
	$v \neq 0$ existe $f$ tal que $L_v(f) \neq 0$ por lo que $L_v$ es distinta de la transformación nula.
	$\ker(\Omega) = \{0\}$
	$\Omega$ es un monomorfismo
	$\dim(V^{**}) = \dim(L(V^*,\mathbb F)) = \dim(L(L(V,\mathbb F), \mathbb F),\mathbb F)$
	$=\dim(L(V,\mathbb F)) \cdot \dim(\mathbb F) = \dim(V) \cdot \dim(\mathbb F) \cdot \dim(\mathbb F) = \dim(V)$
	Sigue que $\Omega$ es un isomorfismo
Si $L \in V^{**}$ existe un único vector $v$ tal que  $L(f)=f(v)$ $\forall f \in V^*$
	$L_v \in V^{**}$ es una tl que cumple lo pedido
	Suponiendo que existe otro vector $u$ tal que $\forall f \in V^*, L(f)=f(u)$
	$L(f)=f(v)=f(u)$
	$f(v)-f(u)=0$
	$f(v-u)=0$, para toda $f \in V^*$
	Si $v-u \neq 0$, existe una $f \in V^*$ que hace que $f(v)\neq 0$ lo cual es una contradicción
	Resulta $v-u=0$ y $v=u$.
