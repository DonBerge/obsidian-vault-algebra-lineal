$T \in L(V,W)$ entonces se define $T^* \in L(W^*,V^*)$ como
$$(T^*(\varphi))(v) = \varphi(T(v))$$
## Algebra de aplicaciones duales
1) $S,T \in L(V,W) \implies (aS+bT)^*=aS^*+bT^*$
	$v \in V$
	$(aS+bT)^*(\varphi)(v)=\varphi((aS+bT)(v))=\varphi(aS(v)+bT(v))$
	$=a\varphi(S(v))+b\varphi(T(v))=aS^*(v)+bT^*(v)$
2) $T \in L(U,V), S \in L(V,W) \implies (S \circ T)^* = T^* \circ S^*$
	$((S \circ T)^*(\varphi))(u)=\varphi((S \circ T)(U))=\varphi(S(T(u)))$
	$(T^* \circ S^*)(\varphi)(u)=(T^*(S^*(\varphi)))(u)$
	$=T^*(\varphi(S(u)))=\varphi(S(T(u)))$