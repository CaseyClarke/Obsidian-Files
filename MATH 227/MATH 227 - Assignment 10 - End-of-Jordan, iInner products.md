# Question 1

Size of matrix is $10\times10$

$\operatorname{Dim}(\operatorname{Null}((A-\pi I))) = 3 \implies$ 3 blocks with size $\geq 1$
$\operatorname{Dim}(\operatorname{Null}((A-\pi I)^2))-  \operatorname{Dim}(\operatorname{Null}((A-\pi I)))= 3 \implies$ 3 blocks with size $\geq 2$
$\operatorname{Dim}(\operatorname{Null}((A-\pi I)^3))-  \operatorname{Dim}(\operatorname{Null}((A-\pi I)^2))= 2 \implies$ 2 blocks with size $\geq 3$
$\operatorname{Dim}(\operatorname{Null}((A-\pi I)^4))-  \operatorname{Dim}(\operatorname{Null}((A-\pi I)^3))= 2 \implies$ 2 blocks with size $\geq 4$

We then know that size cannot be $\geq 5$ since we need 3 blocks so there must be two blocks of 4 and that leaves us with the only option that the last one is a block of 2

$J(A) = J_4(\pi)\oplus J_4(\pi)\oplus J_2(\pi)$

{{ENDQUESTION}}

# Question 2

(a)

- $\operatorname{det}(A-\lambda I) = \lambda^4 \quad \lambda = 0$
- $\operatorname{Dim}(\operatorname{Null}(A - 0I)) = \operatorname{Dim}(\operatorname{Null}(A))$ 
- $\operatorname{Null}(A) = \left\{ \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix} \right\}$
- $\operatorname{Null}(A^2) = \left\{ \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\0 \\ 1 \\ 0 \end{pmatrix} \right\}$
- $\operatorname{Null}(A^3) = \left\{ \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\0 \\ 1 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\0 \\ 0 \\ 1 \end{pmatrix}  \right\}$
- 
- $\operatorname{Dim}(\operatorname{Null}(A)) = 2 \implies$ There are 2 Jordan blocks
- $\operatorname{Dim}(\operatorname{Null}(A^2)) = 3$
- $\operatorname{Dim}(\operatorname{Null}(A^3)) = 4$

- $\operatorname{Dim}(\operatorname{Null}(A^3) - \operatorname{Dim}(\operatorname{Null}(A^2) = 4-3 = 1 \implies$ 1 block with size $\geq 3$

- $J = \begin{pmatrix} J_3(0) & 0 \\ 0 & J_1(0)\end{pmatrix}$

- We need to find vectors such that $A^3v = 0 \land A^2v \neq 0$
- Start with $v_1 = \begin{pmatrix} 0 \\0 \\ 0 \\ 1 \end{pmatrix}$
- Then find $v_2 = Av_1 \quad Av_2 = v_3 \quad Av_3 = 0$
- Solving the equations we get that 
- $v_1 = \begin{pmatrix} 0 \\0 \\ 0 \\ 1 \end{pmatrix}$
- $v_2 = \begin{pmatrix} 2 \\ 3 \\ 1 \\ 0 \end{pmatrix}$
- $v_3 = \begin{pmatrix} 1 \\ -2 \\ 0 \\ 0 \end{pmatrix}$
- 
- Now to fill in the last vector $v_4$ we just choose a vector such that $Av = 0$, we already know that $v_4 = \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}$ is in the null of A and it is also linearily independant from the other 3 vectors so this works
- Meaning that $P = \begin{pmatrix} 1 & 2 & 0 & 1 \\ -2 & 3 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0\end{pmatrix}$

(b)

- $\operatorname{det}(A-\lambda I) = \lambda^4 - 4\lambda^3+4\lambda^2$
- $\lambda^4 - 4\lambda^3+4\lambda^2 = \lambda^2(\lambda^2 - 4\lambda + 4\lambda) = \lambda^2(\lambda - 2)^2$
- $\lambda = 2, 0$
- 
- $\operatorname{Ker}(A-0I) = \operatorname{Ker}(A) = \begin{pmatrix} 0 \\ -1 \\ 1 \\0 \end{pmatrix}$
- $\operatorname{Ker}(A-2I) = \left\{ \begin{pmatrix} 1 \\ -2 \\ 1 \\ 0 \end{pmatrix}, \begin{pmatrix} -1 \\ 0 \\ 0 \\ 1 \end{pmatrix} \right\}$
- $\operatorname{Dim}(\operatorname{Ker}(A)) = 1 \implies$ One jordan block for $\lambda = 0$
- $\operatorname{Dim}(\operatorname{Ker}(A-2I)) = 2 \implies$ Two jordan blocks for $\lambda = 2$

- $J = \begin{pmatrix} J_2(0) & 0 & 0 \\ 0 & J_1(2) & 0 \\ 0 & 0 &  J_1(2) \end{pmatrix}$

- To find p we just need to "fill in" another generalised eigen vector for $\lambda = 0$
- solving the equation $Ax = \begin{pmatrix} 0 \\ -1 \\ 1 \\ 0\end{pmatrix}$
- we get that $x = \begin{pmatrix} -1 \\ -1 \\ 0 \\ 1\end{pmatrix}$
- Therefore
- 
- $P = \begin{pmatrix}  0 & -1 &  1 & -1 \\-1 &  -1 &-2 & 0 \\ 1 & 0 &   1 &  0 \\0 & 1 &   0 & 1 \\ \end{pmatrix}$

{{ENDQUESTION}}

# Question 3

(a)

- $p(x) = x^2 - x$
- $\langle p(x), p(x)\rangle = 0$ 
- but $p(x) \neq 0$ 
 
(b)

- Symmetry
	- Multiplication is commutative in $\mathbb{R}$ so this is trivially symetric

- Bilinearity
	- $uq(x) + vq'(x) = (ua_q + va_{q'})x^2 + (ub_q + vb_{q'})x + (uc_q + vc_{q'})$
	- $\langle uq(x) + vq'(x), p(x)\rangle = 2(ua_q + va_{q'})(a_p) + (ub_q + vb_{q'})(b_p)$
	- $+ (uc_q + vc_{q'})(c_p) + (ua_q + va_{q'})(b_p) + (ub_q + vb_{q'})(a_p)$
	- Grouping all $u$ and $v$ terms together you get
	- $\langle uq(x) + vq'(x), p(x)\rangle = u(2a_qa_p +b_qb_p + c_qc_p + b_qb_p + a_qb_p + b_qa_p)$
	- $+ v(2a_{q'}a_p +b_{q'}b_p + c_{q'}c_p + b_{q'}b_p + a_{q'}b_p + b_{q'}a_p)$
	- $\langle uq(x) + vq'(x), p(x)\rangle = u\langle q(x), p(x) \rangle + v\langle q'(x), p(x) \rangle$

- Positive
	- $\langle ax^2 + bx + c, ax^2 + bx + c\rangle = 2a^2 + b^2 + c^2 + 2ab$
	- $2a^2 + b^2 + c^2 + 2ab = a^2 + 2ab + b^2 + a^2 +b^2 + c^2$
	- $a^2 + 2ab + b^2 + a^2 +b^2 + c^2 =(a+b)^2 + a^2 +b^2 + c^2$
	- Any real number squared is positive and the sum of positive numbers is positive

{{ENDQUESTION}}

# Question 4

$||A|| = \sqrt{\operatorname{Trace}(AA^T)} = \sqrt{6}$
$||B|| = \sqrt{\operatorname{Trace}(BB^T)} = \sqrt{6}$
$\langle A, B \rangle = \operatorname{Trace}(AB^T) = -3$

$\cos(\theta) = \frac{\langle A, B \rangle}{|A||B|} = \frac{-3}{\sqrt6 \sqrt6} = -\frac12$

$\theta = \cos^{-1}(-\frac12)$

$\theta = \frac{2\pi}{3}$

{{ENDQUESTION}}

# Question 5

(a)

- $\langle 4v-w, 2u+v+w\rangle = (4 \times 2)\langle v,u\rangle + 4\langle v,v\rangle + 4\langle v,w\rangle -2\langle w,u\rangle -\langle w,v\rangle -\langle w,w\rangle$
- $8(-1) + 4(2) + 4(1) -2(2) -(1) -(3)$
- $-4$

(b)

- $\langle v, u + xv + yw\rangle = 0$
	- $\langle v,u\rangle + x\langle v,v\rangle + y\langle v,w\rangle = 0$
	- $-1 + 2x + y = 0$
- 
- $\langle w, u + xv + yw\rangle = 0$
	- $\langle w,u\rangle + x\langle w,v\rangle + y\langle w,w\rangle = 0$
	- $2 + x + 3y = 0$
- 
	Solving the system of equations we get that $y = -1 \quad x = 1$

{{ENDQUESTION}}

# Question 6

Symmetry:
- Since mulitplication is commuatative in $\mathbb{R}$ this is trivial

Non-Degenerate:
- For any non-zero vector $u$ at least one of it's elements are non-zero, take any such element and define it's index as $l$ then create a new vector $v$ such that $v_i = 0$ if $i \neq l$ and $v_i = 1$ if $i = l$
- $\langle u, v\rangle$
- Case 1 $l$ lies in the $m$ "half" of the vector:
	- $\langle u, v\rangle = u_l$

- Case 2 $l$ lies in the $n$ "half" of the vector:
	- $\langle u, v \rangle = -u_l$

- Either way this method of constructing the vector the inner product is non-zero

Bilinear:
- $\langle au + bv, w \rangle = \sum_{i=1}^m(au_i + bv_i)w_i -\sum_{j = m + 1}^{m+n}(au_j+bv_j)w_j$
- $a(\sum_{i=1}^mu_iw_i - \sum_{j = m + 1}^{m+n}u_jw_j) +b(\sum_{i=1}^mv_iw_i - \sum_{j = m + 1}^{m+n}v_jw_j)$
- $\langle au + bv, w \rangle = a\langle u,w\rangle + b\langle v,w\rangle$

Not an inner product:
- $n = 4 \quad m = 1$
- $\langle (0,0,0,0,1), (0,0,0,0,1) \rangle = -1 < 0$


{{ENDQUESTION}}

# Question 7

Symmetry:
- Since intersect is commuatative this is trivial

Non-Degenerate:
- For any $v \neq 0$ we can find another vector $w$ such that $\langle v, w\rangle \neq 0$ by defining $w$ as 
- $|u|$ is even:
	- $w = v$ with a single letter removed if $|u|$ is even, thus $|v \cap w| = 1$ as $|u| = |w| - 1 \implies w$ is odd meaning that $|w| \mod 2 = 1$
- $|w|$ is odd:
	- $w =v$ as $|w| = |v| =$ some odd number meaning that $|w| \mod 2 = 1$

Bilinear:
- $\langle au + bv, cu' + dv' \rangle = ||(au \cup bv) \cap (cu' \cup dv')|| \mod 2$
- $(au \cup bv) \cap (cu' \cup dv') = ((au \cup bv) \cap cu') \cup ((au \cup bv) \cap dv')$
- $((au \cup bv) \cap cu') \cup ((au \cup bv) \cap dv') =((au \cap cu') \cup (bv \cap cu') ) \cup ((au\cap dv') \cup (bv \cap dv'))$
- $au \cap bv = ab\langle u,v \rangle$ as if $a \lor b = 0$ then $au \cap bv = 0$ and if $a \lor b = 1$ then nothing changes
- $ac\langle u,u'\rangle + bc\langle v,u'\rangle + ad\langle u,v'\rangle + bd\langle v,v'\rangle$

{{ENDQUESTION}}

# Question 8

Reflexive:
- The "do nothing" transformation $T(v) = v$ trivially makes this true

Symmetric:
- $\langle u,v \rangle_v = \langle Tu, Tv \rangle_w$
- We know that $T^{-1}$ exists so just apply it to both sides
- $\langle T^{-1}u,T^{-1}v \rangle_v = \langle w, w' \rangle_w$

Transitive:
- V ortho equiv W ortho eqiv U
- 
- $\langle u,v \rangle_v = \langle Tu, Tv \rangle_w$
- $\langle u,v \rangle_w = \langle T'u, T'v \rangle_U$
- 
- $\langle u,v \rangle_v = \langle Tu, Tv \rangle_w = \langle Tu,Tv \rangle_w = \langle T(T'u), T(T'v) \rangle_U$
- $T'' = T \circ T'$
- $\langle u,v \rangle_v = \langle T''u, T''v \rangle_U$
- Thus V is ortho equiv to U