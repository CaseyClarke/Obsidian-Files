# Question 1

$f(x) = \frac12\ln(\frac{1+x}{1-x}) = \frac12(\ln(1+x) - \ln(1-x))$

$\frac{1}{1-x} = \sum_{n = 0}^\infty x^n$
$\int\frac{1}{1-x}dx = \int\sum_{n = 0}^\infty x^ndx$
$-\ln|1-x| = \sum_{n = 0}^\infty \int x^ndx$
$\ln(1-x) = -\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1}$ (ignore absolute value)
constant of integration is 0 (plug  $x = 0$ into both sides)
$\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1} = \sum_{k = 1}^\infty \frac{x^{k}}{k}$

$M \space f(x) = \frac12(\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} + -\sum_{k = 1}^\infty \frac{x^{k}}{k})$
$M \space f(x) = \frac12\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} - \frac{x^{k}}{k}$ (valid to combine since both series converge in the radius of convergence)
$M \space f(x) = \frac12\sum_{k = 1}^\infty \frac{x^{k}}{k} ((-1)^{k-1}-1)$
the alternating part is $0$ when $k-1$ is even and its 2 when $k-1$ is odd
so it's essentially just $\frac12\sum_{k = 1}^\infty 2\frac{x^k}{k} = \sum_{k = 1}^\infty \frac{x^k}{k} \iff k$ is odd 
which you can rewrite as 
$M \space f(x) = \sum_{n = 0}^\infty \frac{x^{2n+1}}{2n+1}$

# Question 2

$f(x) = \frac{1}{x}$
$f'(x) = \frac{-2}{x^2}$
$f''(x) = \frac{6}{x^3}$
$\dots$
$f^{(n)}(x) = \frac{n!(-1)^n}{x^{n+1}}$
$f^{(n)}(-1) = \frac{n!(-1)^n}{{(-1)(-1)}^{n}}$
$f^{(n)}(-1) = -n!$
$T(-1)\space f(x) = \sum_{n = 0}^\infty\frac{f^{(k)}(-1)}{n!}(x+1)^n$
$T(-1)\space f(x) = \sum_{n = 0}^\infty\frac{-n!}{n!}(x+1)^n$
$T(-1)\space f(x) = -\sum_{n = 0}^\infty(x+1)^n$

# Question 3

$\sinh(x) = \frac12(e^x-e^{-x})$
$M \space \sinh(x) = \frac12(\sum_{k = 0}^\infty \frac{x^k}{k!}-\sum_{k = 0}^\infty \frac{(-x)^k}{k!})$
$M \space \sinh(x) = \frac12(\sum_{k = 0}^\infty \frac{x^k}{k!}+ \sum_{k = 0}^\infty (-1)^{k+1}\frac{x^k}{k!})$
$M \space \sinh(x) = \frac12\sum_{k = 0}^\infty \frac{x^k}{k!}+ (-1)^{k+1}\frac{x^k}{k!}$
$M \space \sinh(x) = \frac12\sum_{k = 0}^\infty \frac{x^k}{k!}((-1)^{k+1}+1)$
essentially same as Q1 the alternating part is $0$ when $k+1$ is odd and $2$ when $k+1$ is even
so it's  $\frac12\sum_{k = 0}^\infty 2\frac{x^k}{k!} = \sum_{k = 0}^\infty \frac{x^k}{k!} \iff k+1$ is even
$k+1$ is even means $k+1 = 2n$ for some $n$
$k = 2n-1$
rewriting
$M \space \sinh(x) = \sum_{k = 0}^\infty \frac{x^{2n-1}}{(2n-1)!}$



