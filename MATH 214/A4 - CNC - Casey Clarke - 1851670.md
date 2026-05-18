little "lemma" for Q1 and Q3
for series in the form $\sum_{n = 0}^\infty \frac{x^{2n+1}}{c(n)}$ ($c(n)$ is just some function in $n$)
transform with $u = x^2$
$\sum_{n = 0}^\infty \frac{x^{2n+1}}{c(n)} = x\sum_{n = 0}^\infty \frac{u^n}{c(n)}$
this is now the correct form to be able to use the fomulas for $R$ on $\frac{1}{c(n)}$
(technically this finds $R$ in terms of $u$ and you would have to back transform it to get the $R$ in terms of $x$ but in both the questions where i use this $R_u = R_x$ anyways so it doesn't matter)

# Question 1

$f(x) = \frac12\ln(\frac{1+x}{1-x}) = \frac12(\ln(1+x) - \ln(1-x))$
$\frac{1}{1-x} = \sum_{n = 0}^\infty x^n$
$\int\frac{1}{1-x}dx = \int\sum_{n = 0}^\infty x^ndx$
$-\ln|1-x| = \sum_{n = 0}^\infty \int x^ndx$
$\ln(1-x) = -\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1}$ (ignore absolute value)
constant of integration is 0 (plug  $x = 0$ into both sides)
$\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1} = \sum_{k = 1}^\infty \frac{x^{k}}{k}$

$M \space f(x) = \frac12(\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} + \sum_{k = 1}^\infty \frac{x^{k}}{k})$
$M \space f(x) = \frac12(\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} + \frac{x^{k}}{k})$ (valid to combine since both series converge in the radius of convergence)
$M \space f(x) = \frac12\sum_{k = 1}^\infty \frac{x^{k}}{k} ((-1)^{k-1}+1)$
the alternating part is $2$ when $k-1$ is even and its $0$ when $k-1$ is odd
so it's essentially just $\frac12\sum_{k = 1}^\infty 2\frac{x^k}{k} = \sum_{k = 1}^\infty \frac{x^k}{k} \iff k-1$ is even 
$k-1$ is even means $k$ is odd
$k = 2n+1 \iff$ k is odd for some n
rewriting
$M \space f(x) = \sum_{n = 0}^\infty \frac{x^{2n+1}}{2n+1}$

radius of convergence: 
use lemma: $c(n)= \frac{1}{2n+1}$
ratio formula
$R = \lim_{n \to \infty}|\frac{1/(2n+1)}{1/(2n+3)}|$
$R = \lim_{n \to \infty}|\frac{2n+3}{2n+1}|$
$R = 1$
so intermediate interval is $(-1, 1)$
test $x = -1$
$\sum_{n = 0}^\infty \frac{(-1)^{2n+1}}{2n+1}$
$\sum_{n = 0}^\infty \frac{-1}{2n+1}$
diverges by p-series so we can't include $x = -1$
test $x = 1$
$\sum_{n = 0}^\infty \frac{(1)^{2n+1}}{2n+1}$
$\sum_{n = 0}^\infty \frac{1}{2n+1}$
diverges by p-series so we can't include $x = 1$

final interval: $x$ converges $\iff x \in (-1,1)$

{{ENDQUESTION}}
# Question 2

$f(x) = \frac{1}{x}$
$f'(x) = \frac{-1}{x^2}$
$f''(x) = \frac{2}{x^3}$
$\dots$
$f^{(n)}(x) = \frac{n!(-1)^n}{x^{n+1}}$
$f^{(n)}(-1) = \frac{n!(-1)^n}{{(-1)(-1)}^{n}}$
$f^{(n)}(-1) = -n!$
$T(-1)\space f(x) = \sum_{n = 0}^\infty\frac{f^{(k)}(-1)}{n!}(x+1)^n$
$T(-1)\space f(x) = \sum_{n = 0}^\infty\frac{-n!}{n!}(x+1)^n$
$T(-1)\space f(x) = -\sum_{n = 0}^\infty(x+1)^n$

radius of convergence: 
its a geo series with $r = x+1$
to converge we need $|x+1| < 1$
so $R = 1$
so intermediate interval is $(-2, 0)$

test $x = -2$
$-\sum_{n = 0}^\infty(-1)^n$
diverges by AST so we can't include $x = -2$
test $x = 0$
$-\sum_{n = 0}^\infty(1)^n$
fails screening test so we can't include $x = 0$

final interval: $x$ converges $\iff x \in (-2,0)$

{{ENDQUESTION}}
# Question 3

$\sinh(x) = \frac12(e^x-e^{-x})$
$M \space \sinh(x) = \frac12(\sum_{k = 0}^\infty \frac{x^k}{k!}-\sum_{k = 0}^\infty \frac{(-x)^k}{k!})$
$M \space \sinh(x) = \frac12(\sum_{k = 0}^\infty \frac{x^k}{k!}+ \sum_{k = 0}^\infty (-1)^{k+1}\frac{x^k}{k!})$
$M \space \sinh(x) = \frac12(\sum_{k = 0}^\infty \frac{x^k}{k!}+ (-1)^{k+1}\frac{x^k}{k!})$
$M \space \sinh(x) = \frac12\sum_{k = 0}^\infty \frac{x^k}{k!}((-1)^{k+1}+1)$
essentially same as Q1 the alternating part is $0$ when $k+1$ is odd and $2$ when $k+1$ is even
so it's  $\frac12\sum_{k = 0}^\infty 2\frac{x^k}{k!} = \sum_{k = 0}^\infty \frac{x^k}{k!} \iff k+1$ is even
$k+1$ is even means $k$ is odd
$k = 2n+1 \implies k$ is odd for some n 
rewriting
$M \space \sinh(x) = \sum_{n = 0}^\infty \frac{x^{2n+1}}{(2n+1)!}$

radius of convergence: 
use lemma: $c(n) = \frac{1}{(2n+1)!}$
ratio formula
$R = \lim_{n \to \infty}|\frac{1/(2n+1)!}{1/(2n+3)!}|$
$R = \lim_{n \to \infty}|\frac{(2n+3)!}{(2n+1)!}|$
$R = \lim_{n \to \infty}|\frac{(2n+3)(2n+2)(2n+1)!}{(2n+1)!}|$
$R = \lim_{n \to \infty}|\frac{(2n+3)(2n+2)}{1}|$
$R = \infty$
final interval: $x$ converges $\iff x \in (-\infty,\infty)$
