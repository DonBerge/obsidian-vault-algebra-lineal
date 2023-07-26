Dada una [[Transformacion lineal|transformacion lineal]] $T:V\to W$ y dos espacios vectoriales $S \subseteq V$ y $R \subseteq W$:
1) $T(S) \subseteq W$
2) $T^{-1}(R) \subseteq V$

1) Prueba de 1)
	Dados $u,v \in T(S)$,  $\exists u',v' \in S : T(u') = u, T(v') = v$
	$au+vb = aT(u')+bT(v') = T(au'+bv')$
	$au'+bv' \in S \therefore T(au'+bv') \in T(S)$
	$T(S)$ es sev
1) Prueba de 2)
	Dados $u,v \in T^{-1}(R), \exists u',v' \in R : T(u)=u', T(v) = v'$
	$au'+bv' \in R$
	$au'+bv' = aT(u)+bT(v) = T(au+bv)$
	$T(au+bv) \in R \implies au+bv \in T^{-1}(R)$
	$T^{-1}(R)$ es sev