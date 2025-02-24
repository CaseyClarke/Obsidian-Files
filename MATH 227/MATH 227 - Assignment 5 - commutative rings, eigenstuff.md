
# Question 1

(a)

For any $p(x)$ to be invertible there must exists a $q(x)$ in the same domain such that $p(x)q(x) = 1$
The degree of the LHS is 0 which means that $0 = deg(p(x)q(x))$ and since $x^ax^b = x^{a+b}$
$0 = deg(p(x)) + deg(q(x))$ meaning that $p(x)$ and $q(x)$ are both constants

so we can only take the case of $p(x) = a$ for some constant $a \in R$ since this "polynomial" is actually just some element in R we can say that any $p(x)$ in $R[x]$ is only invertible if $a$ is invertible in R

(b)

$r(x),s(x) \in R[x]$

Case 1: $r(x) \neq 0$

$r(x)q(x) = 0$
$r(x)q(x) = r(x)0$
$\implies q(x) = 0$

Case 2: $q(x) \neq 0$

$r(x)q(x) = 0$
$r(x)q(x) = 0q(x)$
$\implies r(x) = 0$

(c)

Same argument as (a)
$p(x,y)q(x,y) = 1$
$deg(1) = deg(p(x,y)q(x,y))$
$(0,0) = deg(p(x,y)) + deg(q(x,y))$
meaning that the x degree and the y degree must be both 0
so $p(x,y) = a \quad a \in R$  is invertible iff $a$ is invertible in R
$\therefore$ $U(R[x,y]) = U(R[x]) = U(R)$

{{ENDQUESTION}

# Question 2

(a)

- $(1,6)$

(b)

- $\{1,5,7,11\}$

(c)

- $(1,6)$

(d)

- $\{\pm 1\}$

{{ENDQUESTION}}

# Question 3

(a)

$p(x).(u+v) = (a_0 + a_1(2)^1 + a_2(2)^2 + \dots + a_n(2)^n)(u+v)$
Since both elements are now just real numbers we can use distributivity
$p(2) = a_0 + a_1(2)^1 + a_2(2)^2 + \dots + a_n(2)^n$
$p(x).(u+v) = (p(2))u + (p(2))v$
$p(x).(u+v) = (p(x)).u + (p(x)).v$

(b)

Assume for contradiction there is such a $T$, Let $T(1) = w$

$T(p(x).1) = p(x).T(1) = p(x).w = p(3)w$
$T(p(x).1) = T(p(2)1) = p(2)T(1) = p(2)w$
$p(3)w = p(2)w$
$p(3) = p(2)$
this is a contradiction as for example it is not true for $p(x) = x$

{{ENDQUESTION}}

# Question 4

(a)

$det(A-\lambda I) = (1-\lambda)(-\lambda) - 6 = \lambda^2-\lambda - 6$
$\lambda^2-\lambda - 6 = 0$
$(\lambda + 2)(\lambda - 3) = 0$
$\lambda = -2,3$

but $-2 \equiv 3$ (mod 5) so the P matrix would have two dependant columns meaning we cannot diagonalize the matrix

(b)

starting from where we left off in (a)

$\operatorname{Null}(A-3I) = \begin{pmatrix} 3 \\ 1\end{pmatrix}$
$\operatorname{Null}(A+2I) = \begin{pmatrix} -2 \\ 1\end{pmatrix}$

$P = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}$

$P^{-1} = \frac15 \begin{pmatrix}  1 & 2 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix}$

$D = \begin{pmatrix}  3 & 0 \\ 0 & -2 \end{pmatrix}$

(c)

$\sqrt{B} = P\sqrt{D}P^{-1}$
as $\sqrt{B}\sqrt{B} = P\sqrt{D}P^{-1}P\sqrt{D}P^{-1} = PDP^{-1}$

$\sqrt{3} = \sqrt{25} = \pm 5$
$\sqrt{-2} = \sqrt{9} = \pm3$

$\sqrt{B}_1 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  5 & 0 \\ 0 & 3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  2 & -2 \\ -4 & -5 \end{pmatrix}$
$\sqrt{B}_2 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  -5 & 0 \\ 0 & 3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  -4 & -3 \\ 5 & 2 \end{pmatrix}$
$\sqrt{B}_3 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  5 & 0 \\ 0 & -3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  4 & 3 \\ -5 & -2 \end{pmatrix}$
$\sqrt{B}_4 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  -5 & 0 \\ 0 & -3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  -2 & 2 \\ 4 & 5 \end{pmatrix}$

{{ENDQUESTION}}
# Question 5

$det(B-\lambda I) = (-1-\lambda)(-3-\lambda) + 2 = \lambda^2 +4\lambda + 5$

$\lambda = \frac{-4 \pm \sqrt{-4}}{2} =  \frac{-4 \pm 2i}{2} = -2 \pm i$

$\operatorname{Null}(B-(-2+i)I) = \begin{pmatrix} -1-i \\ 1\end{pmatrix}$
$\operatorname{Null}(B-(-2-i)I) = \begin{pmatrix} -1+i \\ 1\end{pmatrix}$

$P = \begin{pmatrix} -1-i & -1 + i \\ 1 & 1\end{pmatrix}$

$D = \begin{pmatrix} -2 + i & 0 \\ 0 & -2 - i\end{pmatrix}$

{{ENDQUESTION}}
# Question 6

$T$ map: 
- $T(\hat{v}) = \lambda\hat{w}$
- we have that the $ith$ entry of the eigenvector $\hat{w}$ is of the form $\hat{w}_i = a\hat{v}_{i+1}$ 
- with eigenvalue $\lambda = \frac 1a$

$S$ map:
- $S(\hat{v}) = \lambda\hat{w}$
- The $ith$ entry of the eigenvector $\hat{w}$ is of the form $\hat{w}_i = a\hat{v}_{i-1}$ where $\hat{v}_{-1} = 0$
- with eigenvalue $\lambda = \frac1a$