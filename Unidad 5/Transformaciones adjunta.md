Si $V$ es un $\mathbb F$-ev con producto interno y $T \in L(V)$. Existe $T^* \in L(V)$ tal que
$$<Tu,v> = <u,T^*v>$$
Para cualquier par de vectores $u,v \in V$


La transformación adjunta es única
Si $T \in L(V)$ y $S,U \in L(V)^*$ transformaciones adjuntas a $T$
$\forall w,v \in V$
$<w,T^*v> = <w,Sv> = <w,Uv>$
$<w,Sv>-<w,Uv>=0$
$<w,(S-U)v>=0$
En particular para $w=(S-U)v$:
$(S-U)v=0$
$S(v)=U(v)$
$S=U$
## Algebra de transformaciones adjuntas
$T,S \in L(V)$
$(T+S)^* = T^* + S^*$ )
	$<(T+S)v,u> = <Tv + Sv,u> = <Tv,u>+<Sv,u> = <v,T^*u>+<v,S^*u>$
	$=<v,T^*u+S^*u> = <v,(T^*+S^*),u>$
	$T^*+S^*=(T+S)^*$
$(kT)^* = \overline k T^*$ )
	$<kTv,u>=k<Tv,u>=k<v,T^*u>=<v,\overline k T^*u>$
	$(kT)^* = \overline k T^*$
$(T \circ S)^* = S^* \circ T^*$ )
	Sea $B$ base de $V$:
	$[(T \circ S)^*]_B = [T \circ S]_B^* = ([T]_B \cdot [S]_B)^*$
	
	$A,B \in \mathbb F^{n \times n}:$
	$(A \cdot B)^t = B^t \cdot A^t$
	$\overline{A \cdot B} = \overline A \cdot \overline B$:
		$(\overline A \cdot \overline B)_{ij} = \sum_{k=1}^n \overline a_{ik}\overline b_{kj} = \overline{\sum_{k=1}^n a_{ik}b_{kj}} = \overline{(A\cdot B)_{ij}} = (\overline{AB})_{ij}$
	Por lo tanto $(A\cdot B)^* = B^* \cdot A^*$
	$([T]_B \cdot [S]_B)^* = [S^*]_B \cdot [T^*]_B$
	$(T \cdot S)^* = S^* \cdot T^*$
$T^{**}=T^*$ )
	Trivial sabiendo que $\forall A \in \mathbb F^{n \times n}: A^{**}=A$
