# Question 1

(a)

For any $p(x)$ to be invertible there must exists a $q(x)$ in the same domain such that $p(x)q(x) = 1$
The degree of the RHS is 0 which means that $0 = deg(p(x)q(x))$ and since $x^ax^b = x^{a+b}$
$0 = deg(p(x)) + deg(q(x))$ meaning that $p(x)$ and $q(x)$ are both constants as a polynomial cannot have negitive degree

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