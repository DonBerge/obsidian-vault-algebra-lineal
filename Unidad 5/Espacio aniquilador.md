Sea $U$ un sev de $V$ se define
$$U^0 = \{\varphi \in V^* : \varphi(u) = 0 \: \forall u \in U\} = \{\varphi  \in V^* : U \subseteq \ker(\varphi)\}$$
como el aniquilador de $U^0$.

## El aniquilador es un sev de V
$\varphi, \tau \in U^0$, $u \in U$
$\varphi,\tau \in V^*$
$(\alpha \varphi + \beta \tau)(u) = \alpha\varphi(u) + \beta \tau(u) = \alpha 0 + \beta 0 = 0$
$\alpha \varphi + \beta \tau \in U^0$
$U^0$ es un sev de $V^*$

## Dimensión del aniquilador
Se tiene que:
$$\dim(U) + \dim(U^0) = \dim(V)$$
Sea $B_U = \{u_1,\dots,u_r\}$ base de $U$, extiendo a una base $B$ de $V$
$B=\{v_1,\dots,v_r,\dots,v_n\}$ y $B^*=\{\varphi_1,\dots,\varphi_r,\dots,\varphi_n\}$, $\{\varphi_{r+1}\dots \varphi_n\}$ es una base de $U^0$

Si $1\leq i\leq r,n \geq j\geq r+1$, $\varphi_{j}(u_i) = \delta_{ji} = 0$. $\varphi_j \in U^0$, $span(\varphi_{r+1},\varphi_n) \subseteq U^0$

$\{\varphi_{r+1}\dots \varphi_n\}$ son li ya que de lo contrario $B^*$ no seria li.

$\tau \in U^0 \implies \tau \in V^* \implies \tau(u) = \sum_{i=1}^n b_i \varphi_i$, $b_1\dots b_n$ escalares.
$b_1,\dots b_r = 0$, sino entonces para algun $i$ tal que $1\leq i \leq r$, $\tau(v_i) = b_i \neq 0$ y $\tau \notin U^0$.
Por lo tanto $\tau = \sum_{i=r+1}^n b_i \varphi_i$ y $span(\varphi_{r+1},\varphi_n) = U^0$

$\{\varphi_{r+1}\dots \varphi_n\}$ es base de $U^0$

## Algebra de aniquiladores
1) $(U+W)^0 = U^0 \cap W^0$
	$\varphi \in (U+W)^0 \iff \varphi(u+w)=0 \: \forall u \in U, w \in W$
	En particular, $\varphi(u+0)=0$ ya que $0 \in W$, por lo que $\varphi(u)=0$ y lo mismo ocurre para $w$.
	$\varphi(u+w)=0 \: \forall u \in U, w \in W \iff \varphi(u)=0 \: \forall u \in U \land \varphi(w)=0 \forall w \in W \iff \varphi \in U^0 \cap W^0$

2) $(U \cap W)^0 = U^0 + W^0$
	$\varphi \in U^0 + W^0 \implies \varphi = \varphi_U + \varphi_W$, $\varphi_U \in U^0$, $\varphi_W \in W^0$
	$v \in U \cap W \implies \varphi(v) = \varphi_U(v) + \varphi_W(v)=0+0=0$
	$v \in (U \cap W)^0$, $(U \cap W)^0 \subseteq U^0 + W^0$

	$\dim(U^0 + W^0) = \dim(U^0) + \dim(W^0) - \dim(U^0 \cap W^0)$
	$=\dim(U^0)+\dim(W^0)-\dim((U + W)^0)$
	$=\dim(V)-\dim(U)+\dim(V)-\dim(W)-\dim(V)+\dim(U+W)$
	$=\dim(V)+-\dim(U) - \dim(W) + \dim(U)+\dim(W)-\dim(U \cap W)$
	$=\dim(V)-\dim(U \cap W) = \dim((U \cap W)^0)$

	Sigue que $U^0+W^0 = (U \cap W)^0$
	