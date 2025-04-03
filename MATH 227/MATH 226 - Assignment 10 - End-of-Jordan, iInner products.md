# Question 1

Size of matrix is $10\times10$

$\operatorname{Dim}(\operatorname{Null}((A-\pi I))) = 3$

$J(A) = J_4(\pi)\oplus J_3(\pi)\oplus J_3(\pi)$

{{ENDQUESTION}}

# Question 2

(a)

- $\operatorname{det}(A-\lambda I) = \lambda^4 \quad \lambda = 0$
- $\operatorname{Dim}(\operatorname{Null}(A - 0I)) = \operatorname{Dim}(\operatorname{Null}(A))$ 
- $\operatorname{Null}(A) = \left\{ \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix} \right\}$
- $\operatorname{Dim}(\operatorname{Null}(A)) = 2 \implies$ There are 2 Jordan blocks

- $A^2 = \begin{pmatrix} 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & -2 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ \end{pmatrix}$

- $\operatorname{Dim}(\operatorname{Null}(A^2)) = 4 - 2 = 2 \implies$ At least 2 blocks of size 2

- $J = \begin{pmatrix} J_2(0) & 0 \\ 0 & J_2(0)\end{pmatrix}$
- The columns of P are the 2 vectors of $\operatorname{Null}(A)$ $v_1 =  \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix} v_3 = \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix}$ 
  plus 2 generalised eigenvectors, $x,y$ where $Ax = v_1$ and $Ay = v_3$
- solving these equations gives 
  $x = \begin{pmatrix} 0 \\ 0 \\ 1 \\ 0 \end{pmatrix} y = \begin{pmatrix} 0 \\0 \\ 5 \\ 1 \end{pmatrix}$
- Meaning that $P = \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 5 \\ 0 & 0 & 0 & 1\end{pmatrix}$

(b)

- $\operatorname{det}(A-\lambda I) = \lambda^4 - 4\lambda^3+4\lambda^2$
- $\lambda^4 - 4\lambda^3+4\lambda^2 = \lambda^2(\lambda^2 - 4\lambda + 4\lambda) = \lambda^2(\lambda - 2)^2$
- $\lambda = 2, 0$
- 
- $\operatorname{Ker}(A-0I) = \operatorname{Ker}(A) = \begin{pmatrix} 1 \\ 1 \\ 1 \\ -1 \end{pmatrix}$
- $\operatorname{Ker}(A-2I) = \left\{ \begin{pmatrix} 1 \\ 1 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\ 0 \\ 1 \\ 1 \end{pmatrix} \right\}$
- $\operatorname{Dim}(\operatorname{Ker}(A)) = 1 \implies$ One jordan block for $\lambda = 0$
- $\operatorname{Dim}(\operatorname{Ker}(A-2I)) = 2 \implies$ Two jordan blocks for $\lambda = 2$

- $J = \begin{pmatrix} J_2(0) & 0 & 0 \\ 0 & J_1(2) & 0 \\ 0 & 0 &  J_1(2) \end{pmatrix}$

==Still need to find P==

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
	- $\langle p(x), uq(x) + vq'(x)\rangle =$

- Positive
	- Stuff

- ==Not complete==


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


{{ENDQUESTION}}

# Question 7

Symmetry:
- Since intersect is commuatative this is trivial

Non-Degenerate:
- For any $v \neq 0$ we can find another vector $w$ such that $\langle v, w\rangle \neq 0$ by defining $w$ as the original set $v$ plus some other letter that is not in $v$ this makes is so the intersect only contains a single element and the length squared of a single element is just $1 \mod 2 \neq 0$ which is always true

Bilinear:
- $\langle au + bv, cu' + dv' \rangle = ||(au \cup bv) \cap (cu' \cup dv')|| \mod 2$
- $(au \cup bv) \cap (cu' \cup dv') = ((au \cup bv) \cap cu') \cup ((au \cup bv) \cap dv')$
- $((au \cup bv) \cap cu') \cup ((au \cup bv) \cap dv') =((au \cap cu') \cup (bv \cap cu') ) \cup ((au\cap dv') \cup (bv \cap dv'))$
- $au \cap bv = ab\langle u,v \rangle$ as if $a \lor b = 0$ then $au \cap bv = 0$ and if $a \lor b = 1$ then nothing happens to the intersection 
- $ac\langle u,u'\rangle + bc\langle v,u'\rangle + ad\langle u,v'\rangle + bd\langle v,v'\rangle$

{{ENDQUESTION

# Question 8

Reflexive:
- The "do nothing" transformation $T(v) = v$ trivially makes this true

Symmetric:
- 

Transitive: