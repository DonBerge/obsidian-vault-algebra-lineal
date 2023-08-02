Sea $V$ un $\mathbb F$ ev con producto interno y $\varphi \in V^*$ entonces existe un único vector $u \in V$ tal que $\varphi(v)=\langle v,u\rangle$.

Sea $B=\{v_1,\dots,v_n\}$ una bon de $V$
$v \in V \implies v = \sum_{i=1}^n \langle v,v_i \rangle v_i$
$\varphi(v)=\varphi(\sum_{i=1}^n \langle v,v_i \rangle v_i)=\sum_{i=1}^n \langle v,v_i \rangle \varphi(v_i)=\sum_{i=1}^n \langle v,\overline{\varphi(v_i)v_i}\rangle = \langle v, \sum_{i=1}^n \overline{\varphi(v_i)}v_i \rangle$
$u:=\sum_{i=1}^n \overline{\varphi(v_i)}v_i$ es el vector que cumple el enunciado.

Suponiendo que existe otro vector $u'$ tal que $\varphi(v)=\langle v, u' \rangle$
$\varphi(v) = \langle v, u' \rangle = \langle v,u\rangle$
$\langle v, u'-u \rangle = 0$
$\langle u'-u, u'-u \rangle = 0$
$u'-u=0$
$u'=u$

El vector u definido es único

## Isomorfismo entre un ev y su dual
Sea V un $\mathbb R$ ev.
Definiendo $\Phi: V \to V^*$ definida como $\Phi(v)=\varphi_u$ donde $\varphi(v)=\langle v,u \rangle$ se tiene que
$\Phi$ esta bien definida)
	$\varphi_v$ existe por el teorema de representación de Riez
	$\varphi_u(av+bw)=\langle av+bw, u\rangle = a\langle v,u \rangle + b \langle w,u \rangle = a\varphi_u(v) + b \varphi_u(w)$
	$\varphi_u$ es una tl de $V \to \mathbb F$. $\Phi$ esta definida para todo $v \in V$.
	$\Phi(av+bw)(u)=\varphi_{av+bw}(u)=\langle u,av+bw \rangle$
	$=\langle u,av \rangle + \langle u, bw \rangle$
	$=a\langle u,v \rangle + b \langle u , w \rangle$
	$=a\varphi_v(u) + b \varphi_w(u)$
	$=a \Phi(v)(u) + b \Phi(w)(u)$
	$\Phi$ es una tl
$\Phi$ es un monomorfismo)
	 $\ker(\Phi)=\{v \in V : \Phi(v)(u)=0 \ \forall u \in V\}$
	 $\Phi(v)(u)=0$ $\forall u \in V$ $\iff$ $\langle u,v \rangle = 0$ $\forall u \in V$ $\iff$ $v=0$
	 $\ker(\Phi)=\{0\}$
	 $\Phi$ es un monomorfismmo
$\Phi$ es un epimorfismo)
	$\dim(\ker(\Phi))+\dim(Im(\Phi))=\dim(V)=\dim(V^*)$
	$0+\dim(Im(\Phi))=\dim(V^*)$
	$\dim(Im(\Phi))=\dim(V^*)$
	$\Phi$ es un epimorfismo
Como consecuencia $\Phi$ es un isomorfismo