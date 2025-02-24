
# Question 1

(a)

For any $p(x)$ to be invertible there must exists a $q(x)$ in the same domain such that $p(x)q(x) = 1$
The degree of the LHS is 0 which means that $0 = deg(p(x)q(x))$ and since $x^ax^b = x^{a+b}$
$0 = deg(p(x)) + deg(q(x))$ meaning that $p(x)$ and $q(x)$ are both constants

so we can only take the case of $p(x) = a$ for some constant $a \in R$ since this "polynomial" is actually just some element in R we can say that any $p(x)$ in $R[x]$ is only invertible if $a$ is invertible in R

(b)

Suppose for contradiction that $f(x)$ and $g(x)$ are non-zero polynomials with $n$ and $m$ degree respectively and leading coeffecients $C_f$ and $C_g$
If $f(x)g(x) = 0$ every term must be zero so for a general leading term: $C_fC_gx^{m+n}$  by the zero property of $R$ either $C_f = 0$ or $C_g = 0$ meaning that either $f(x)$ or $g(x)$ has a leading term of zero we can inductively continue this down making every next leading term 0 until the whole polynomial is 0 which is a contradiction

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

$A^n = PD^nP^{-1}$
$\sqrt{B} = P\sqrt{D}P^{-1}$

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
- $T(\hat{v}) = \lambda\hat{v}$
- $(a_2,a_3,a_4\dots) = \lambda(a_1,a_2,a_3,\dots) = (\lambda a_1,\lambda a_2,\lambda a_3,\dots)$
- $a_2 = \lambda a_1$
- $a_3 = \lambda a_2 = \lambda^2a_1$
- $\dots$
- $a_n = \lambda^{n-1} a_1 \quad n > 0$
- $\therefore$ The eigenvectors for this map are in the form $(a_1, \lambda a_1, \lambda^2 a_1, \lambda^3 a_1, \dots)$ with eigen values $\lambda \neq 0$ and $a_1 \neq 0$ so that we don't get the trivial space

$S$ map:
- $S(\hat{v}) = \lambda\hat{v}$
- $(0, a_1, a_2, a_3, \dots) = \lambda(a_1,a_2,a_3,\dots) = (\lambda a_1,\lambda a_2,\lambda a_3,\dots)$
- $0 = \lambda a_1 \implies \; \lambda = 0 \lor a_1 = 0$ 
- In either case the proposed eigenvector becomes the 0 vector meaning that it cannot be an eigenvector
- $\therefore$ This map has no eigenvectors or eigenvalues