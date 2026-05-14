# Question 1

$f(x) = \frac12\ln(\frac{1+x}{1-x}) = \frac12(\ln(1+x) - \ln(1-x))$

$\frac{1}{1-x} = \sum_{n = 0}^\infty x^n$
$\int\frac{1}{1-x}dx = \int\sum_{n = 0}^\infty x^ndx$
$-\ln|1-x| = \sum_{n = 0}^\infty \int x^ndx$
$\ln(1-x) = -\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1}$ (ignore absolute value)
constant of integration is 0 (plug  $x = 0$ into both sides)
$\sum_{n = 0}^\infty \frac{x^{n+1}}{n+1} = \sum_{k = 1}^\infty \frac{x^{k}}{k}$

$f(x) = \frac12(\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} + -\sum_{k = 1}^\infty \frac{x^{k}}{k})$
$f(x) = \frac12\sum_{k = 1}^\infty(-1)^{k-1}\frac{x^k}{k} - \frac{x^{k}}{k}$ (valid to combine since both series converge in the radius of convergence)
$f(x) = \frac12\sum_{k = 1}^\infty \frac{x^{k}}{k} ((-1)^{k-1}-1)$
the alternating part is $0$ when $k-1$ is even and its 2 when $k-1$ is odd
so it's essentially just $\frac12\sum_{k = 1}^\infty 2\frac{x^k}{k} = \sum_{k = 1}^\infty \frac{x^k}{k} \iff k$ is odd 
which you can rewrite as 
$f(x) = \sum_{n = 0}^\infty \frac{x^{2n+1}}{2n+1}$

# Question 2

$f(x) = \frac{1}{x}$
$f'(x) = \frac{-1}{x^2}$
$f''(x) = \frac{1}{x^3}$
$\dots$
$f^{(n)}(x) = \frac{(-1)^n}{x^n}$

$T\space f(x) = \sum_{n = 0}^\infty\frac{f^{(k)}(-1)}{n!}(x+1)^n$
$T\space f(x) = \sum_{n = 0}^\infty\frac{\frac{(-1)^n}{(-1)^n}}{n!}(x+1)^n$
$T\space f(x) = \sum_{n = 0}^\infty\frac{(x+1)^n}{n!}$


