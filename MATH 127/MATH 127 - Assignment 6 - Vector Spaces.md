1. 
$$A$$
$$\left[
	\begin{array}{ccc|ccc}
	1&0&0&2&7&1\\
	0&1&0&1&4&-1\\
	0&0&1&1&3&0\\
	\end{array}
\right]$$
$R_1 \leftarrow R_1 - R_2$
$R_2 \leftarrow R_2 - R_3$
$R_1 \leftarrow R_1 - R_3$
$R_1 \leftrightarrow R_3$
$$\left[
	\begin{array}{ccc|ccc}
	0&0&1&1&3&0\\
	0&1&-1&0&1&-1\\
	1&-1&-1&0&0&2\\
	\end{array}
\right]$$
$R_3 \leftarrow \frac12 R_3$
$R_2 \leftarrow R_2 + R_3$
$R_1 \leftarrow R_1 - 3R_2$
$$\left[
	\begin{array}{ccc|ccc}
	-9&-9&-2&1&0&0\\
	3&3&1&0&1&0\\
	3&2&2&0&0&1\\
	\end{array}
\right]$$
Simplifying
$$\left[
	\begin{array}{ccc|ccc}
	1&1&3&1&0&0\\
	3&3&1&0&1&0\\
	3&2&2&0&0&1\\
	\end{array}
\right]$$

$$\therefore A^{-1} = \left[
	\begin{array}{ccc}
	1&1&3\\
	3&3&1\\
	3&2&2\\
	\end{array}
\right]$$

$$B$$
$$\left[
	\begin{array}{cccc}
	-3&5&0&2\\
	-1&2&−1&0\\
	0&1&2&−4\\
	1&−2&−4&2\\
	\end{array}
\right]$$
$R_4 \leftarrow R_4 + R_2$
$R_1 \leftarrow R_1 -3R_2$
$R_2 \leftrightarrow R_1$
$R_3 \leftarrow R_3 + R_2$
$R_4 \leftarrow R_4 + R_3$
$$\left[
	\begin{array}{cccc}
	-1&2&−1&0\\
	0&-1&3&2\\
	0&0&5&−2\\
	0&0&0&0\\
	\end{array}
\right]$$
$$B\text{ is not invertible as } RREF(B) \text{ has a row of 0's}$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. 
	(a)
	$\exists \; 0_V = (-1,1) \in V \text{ Such That } u + 0_V = u \quad \forall u \in V$
	$Let \; u = (a,b)$
	$(a,b) + (-1,1) = (a,b)$
	$\Rightarrow (a + -1 + 1, b + 1 - 1) = (a,b)$
	$\Rightarrow (a,b) = (a,b)$
	$\therefore$ the 0-vector is $(-1,1)$ for the vector space $V$
	(b)
	$(2,5) + (-4, -3) = (-1,1)$
	$(2 + -4 + 1, 5 + -3 - 1) = (-1,1)$
	$(-1,1) = (-1,1)$
	$\therefore$ the additive inverse of $(2,5)$ is $(-4, -3)$
	(c)
	To prove that $\mathbb{F}_{17}^2$ is a vector field we need to prove that the 10 axioms hold
	
	$Let \; u,v,w \in V \quad Let \; a, b  \in \mathbb{F}_{17}$
	$Let \; u = (u_1, u_2)$
	$Let \; v = (v_1, v_2)$
	$Let \; w = (w_1, w_2)$
	
	Closure of A:
	$u + v \in V$
	$(u_1 + v_1 + 1, u_2 + v_2 - 1)$
	As $\mathbb{F}_{17}$ is closed under addition
	$(u_1 + v_1 + 1, u_2 + v_2 - 1) \in V$
	$QED$
	
	Commutativity of A:
	$u + v = v + u$
	$(u_1 + v_1 + 1, u_2 + v_2 - 1) = (v_1 + u_1 + 1, v_2 + u_2 - 1)$
	As addition is commutative in $\mathbb{F}_{17}$ 
	$(u_1 + v_1 + 1, u_2 + v_2 - 1) = (u_1 + v_1 + 1, u_2 + v_2 - 1)$
	$LHS = RHS$
	$QED$
	
	Associativity of A:
	$(u+v) + w = u + (v + w)$
	$(u_1 + v_1 + 1, u_2 + v_2 - 1) + w = u + (v_1 + w_1 + 1, v_2 + w_2 - 1)$
	$(u_1 + v_1 + w_1 + 2, u_2 + v_2 + w_2 - 2) = (u_1 + v_1 + w_1 + 2, u_2 + v_2 + w_2 - 2)$
	$LHS = RHS$
	$QED$
	
	Additive Identity:
	Proved in (a)
	
	Additive Inverse:
	$u + -u = (-1, 1)$
	Using $(-1)u = -u$ as proved in class
	$(-1)u = -u$
	$\Rightarrow (-1u_1 -1 -1, -1u_2 + 1 + 1) = -u$
	$\Rightarrow (-u_1 -2, -u_2 + 2) = -u$
	$\therefore$  the additive inverse for any $u$ is, $-u = (-u_1 -2, -u_2 + 2)$ 
	$QED$
	
	Closure of M:
	$au \in V$
	$\Rightarrow (au_1 + a - 1)$
	As our vectors and scalars are both in $\mathbb{F}_{17}$ addition and multiplication are closed and so 
	$\Rightarrow (au_1 + a - 1) \in V$
	$QED$
	
	Associativity of M:
	$a(bu) = (ab)u$
	$\Rightarrow a(bu_1 + b - 1, bu_2 - b + 1) = (abu_1 + ab - 1, abu_2 - ab + 1)$
	$\Rightarrow (a(bu_1 + b - 1) + a - 1, a(bu_2 - b + 1) - a + 1) = (abu_1 + ab - 1, abu_2 - ab + 1)$
	$\Rightarrow (abu_1 + ab - a1 + a - 1, abu_2 - ab + a1 - a + 1) = (abu_1 + ab - 1, abu_2 - ab + 1)$
	$\Rightarrow (abu_1 + ab - 1, abu_2 - ab + 1) = (abu_1 + ab - 1, abu_2 - ab + 1)$
	$LHS = RHS$
	$QED$
	
	Unit Property:
	$1u = u$
	$\Rightarrow (1u_1 + 1 - 1, 1u_2 - 1 + 1) = u$
	$\Rightarrow (1u_1, 1u_2) = u$
	$\Rightarrow (u_1, u_2) = u$
	$\Rightarrow u = u$
	$LHS = RHS$
	$QED$
	
	Distributivity #1:
	$a(u+v) = au + av$
	$\Rightarrow a(u_1+v_1 + 1, u_2 + v_2 - 1) = (au_1 + a -1, au_2 - a + 1) + (av_1 + a -1, av_2 - a + 1)$
	$\Rightarrow (a(u_1+v_1 + 1) + a - 1, a(u_2 + v_2 - 1) -a + 1) =$
	$(au_1 + a -1, au_2 - a + 1) + (av_1 + a -1, av_2 - a + 1)$
	$\Rightarrow (au_1 + av_1 + 2a - 1, au_2 + av_2 - 2a + 1) =$
	$((au_1 + a -1) + (av_1 + a -1) + 1, (au_2 - a + 1) + (av_2 - a + 1) - 1)$
	$\Rightarrow (au_1 + av_1 + 2a - 1, au_2 + av_2+ 1) = (au_1 + av_1 + 2a -1, au_2 + av_2 - 2a + 1)$
	$LHS = RHS$
	$QED$
	
	Distributivity #2:
	$(a+b)u = au +bu$
	$\Rightarrow ((a+b)u_1 + (a+b) - 1, (a+b)u_1 - (a+b) + 1) = au +bu$
	$\Rightarrow (au_1 + bu_1 + a + b - 1, au_1 + bu_1 -a -b + 1) = au +bu$
	$\Rightarrow (au_1 + bu_1 + a + b - 1, au_1 + bu_1 -a -b + 1) =$
	$(au_1 + a - 1, au_2 - a + 1) + (bu_1 + b - 1, bu_2 - b + 1)$
	$\Rightarrow (au_1 + bu_1 + a + b - 1, au_1 + bu_1 -a -b + 1) =$
	$(au_1 + bu_1 + a + b - 1, au_1 + bu_1 -a -b + 1)$
	$LHS = RHS$
	$QED$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
	
3. 
	Assume that $1$ is the multiplicative identity of $V$
	$\vec{u} + \vec{u}  = 2\vec{u}$
	$RHS$:
	$2\vec{u}$
	$\Rightarrow (1+1)\vec{u} \quad \quad \quad \quad \text{Used: 1+1=2}$
	$\Rightarrow 1\vec{u} + 1\vec{u}  \quad \quad \quad \quad \text{Axiom Used: Distributivity}$
	$\Rightarrow \vec{u} + \vec{u}  \quad \quad \quad \quad \text{Axiom Used: Multiplicitive identity}$
	
	$LHS = RHS$
	$QED$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
	Suppose that for contradiction $V$ is a vector space, meaning that it must have a unique additive identity $0_V = (a,b) \in V \quad a,b \in \mathbb{Q}$
	$Let \; U = (u_1, u_2) \in V \quad u_1, u_2 \in \mathbb{Q}$
	$U + 0_v = U$
	$\Rightarrow (u_1, u_2) + (a,b) = (u_1, u_2)$
	$\Rightarrow (2u_1 + 2a, u_2 + b) = (u_1, u_2)$
	Making the above equation into a system of equations
	$u_1 = 2u_1 + 2a$
	$u_2 = u_2+b$
	First Equation:
	$u_1 = 2u_1 + 2a$
	$\Rightarrow 2a = u_1 - 2u_1$
	$\Rightarrow a = \frac{u_1}{2} - u_1$
	$\Rightarrow a = -\frac{u_1}{2}$
	Second Equation:
	$u_2 = u_2+b$
	$\Rightarrow b = 0$
	So we get that the additive identity  is $0_V = (-\frac{u_1}{2}, 0)$ which depends in on $U$ making it not unique meaning that there is no unique additive identity for $V$ 
	$\therefore$ The original assumption that $V$ is a vector space must be incorrect. $V$ is not a vector space 
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. 
	To prove that $V$ is a vector field we need to prove that the 10 axioms hold
	
	$Let \; u,v,w \in V \quad Let \; a, b  \in \mathbb{F}$
	$Let \; u = (u_1, u_2)$
	$Let \; v = (v_1, v_2)$
	$Let \; w = (w_1, w_2)$
	
	All 4 of the additive axioms and closure under addition hold as matrix addition of the same size forms a commutative group under addition
	
	Closure of M:
	$au \in V$
	$A(au) = 0$
	$a(Au) = 0$
	$a0 = 0$
	$0 = 0$
	
	Associativity of M:
	$a(bu) = (ab)u$
	$au_{bi, bj} = u_{(ab)i, (ab)j}$
	$u_{(ab)i, (ab)j} = u_{(ab)i, (ab)j}$
	
	Unit Property 
	$1u = u$
	Since the elements of the matrix are in $\mathbb{F}$ and $1a = a$ holds for all fields, all of the elements in $u$ are unchanged after this operation, therefore this holds
	
	Distributivity #1:
	$a(u+v) = au + av$
	$\Rightarrow a(u+v)_{i,j} = au_{i,j} + av_{i,j}$
	$\Rightarrow (u+v)_{ai,aj} = u_{ai,aj} + v_{ai,aj}$
	$\Rightarrow (u+v)_{ai,aj} = (u+v)_{ai,aj}$
	
	Distributivity #2:
	$(a+b)u = au + bu$
	$\Rightarrow u_{(a+b)i, (a+b)j} = u_{ai,aj} + u_{bi,bj}$
	$\Rightarrow u_{(a+b)i, (a+b)j} = u_{ai + bi,aj + bj}$
	$\Rightarrow u_{(a+b)i, (a+b)j} = u_{(a+b)i,(a+b)j}$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. 
	(a)
	We need to prove that the 10 axioms hold
	
	$Let \; u,v,w \in V \quad Let \; a, b  \in \mathbb{Q}$
	$Let \; u = (u_1, u_2)$
	$Let \; v = (v_1, v_2)$
	$Let \; w = (w_1, w_2)$
	
	Closure of A:
	$u + v \in V$
	$\mathbb{R}$ is closed under addition using usual addition
	
	Associativity of A:
	$u + (v+w) = (u+v) + w$
	$\mathbb{R}$ is associative under addition using usual addition
	
	Commutativity of A:
	$u + w = w + u$
	$\mathbb{R}$ is commutative under addition using usual addition
	
	Identity of A:
	$\exists \; 0 \in V \text{ Such That } u + 0 = u$
	$\mathbb{R}$ has an additive identity $0$ using usual addition
	
	Inverse of A:
	$\exists \; -u \in V \text{ Such That } u + -u = 0$
	$\mathbb{R}$ is closed under additive inverses using usual addition
	
	Closure of M:
	$au \in V$
	Since $\mathbb{Q}$ is a subfield of $\mathbb{R}$ both $a, u \in \mathbb{R}$ and since $\mathbb{R}$ is closed under usual multiplication this holds
	
	Associativity of M:
	$a(bu) = (ab)u$
	Since $\mathbb{Q}$ is a subfield of $\mathbb{R}$  $a, b, u \in \mathbb{R}$ and since $\mathbb{R}$ is associative under usual multiplication this holds
	
	Unit Property:
	$\exists \; 1 \in \mathbb{Q} \text{ Such That } 1u = u$
	Since $\mathbb{Q}$ is a subfield of $\mathbb{R}$  $1, u \in \mathbb{R}$ and since $\mathbb{R}$ has the multiplicative identity 1 this holds 
	
	Distributivity #1:
	$a(u+v) = au + av$
	Since $\mathbb{Q}$ is a subfield of $\mathbb{R}$  $a, u, v \in \mathbb{R}$ and since $\mathbb{R}$ follows distributivity this holds
	
	Distributivity #2:
	$(a+b)v = av + bv$
	Since $\mathbb{Q}$ is a subfield of $\mathbb{R}$  $a, b, v \in \mathbb{R}$ and since $\mathbb{R}$ follows distributivity this holds
	
	(b)
	Assume that this forms a vector space for contradiction, what follows is a counter example
	$Let \; v = \pi \; \in V$
	$Let \; a = 0 \in \mathbb{F}$
	$av \in V$
	$\Rightarrow av$
	$\Rightarrow 0\pi$
	$\Rightarrow 0$
	$0 \notin V$
	$\therefore$ our original assumption must be wrong, this does not form a vector field
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

7. 
	$((\vec{v_1} + \vec{v_2}) + \vec{v_3}) + \vec{v_4} = ((\vec{v_4} + \vec{v_3}) + \vec{v_2}) + \vec{v_1}$
	$RHS$:
	$((\vec{v_4} + \vec{v_3}) + \vec{v_2}) + \vec{v_1}$
	$\Rightarrow \vec{v_1} +((\vec{v_4} + \vec{v_3}) + \vec{v_2}) \quad \quad \quad \quad \text{Axiom Used: Commutativity of Addition}$
	$\Rightarrow \vec{v_1} +(\vec{v_2} +(\vec{v_4} + \vec{v_3})) \quad \quad \quad \quad \text{Axiom Used: Associativity of Addition}$
	$\Rightarrow (\vec{v_1} + \vec{v_2}) + (\vec{v_4} + \vec{v_3})  \quad \quad \quad \quad \text{Axiom Used: Associativity of Addition}$
	$\Rightarrow (\vec{v_1} + \vec{v_2}) + (\vec{v_3} + \vec{v_4}) \quad \quad \quad \quad \text{Axiom Used: Commutativity of Addition}$
	$\Rightarrow ((\vec{v_1} + \vec{v_2}) + \vec{v_3}) + \vec{v_4}) \quad \quad \quad \quad \text{Axiom Used: Associativity of Addition}$
	
	$LHS = RHS$
	$QED$