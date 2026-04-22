# Question 1

(a)
$Y = c \implies \Pr(X,N) = c \quad (mod \space 3)$
$Pr(Y = 0) = Pr(0,0) + Pr(1,2) + Pr(2,1)$
$= (0.5)(0.7) + (0.3)(0.1) + (0.2)(0.2)$
$= 0.42$
$Pr(Y = 1) = Pr(0,1) + Pr(1,0) + Pr(2,2)$
$= (0.5)(0.2) + (0.3)(0.7) + (0.2)(0.1)$
$= 0.33$
$Pr(Y = 2) = Pr(0,2) + Pr(1,1) + Pr(2,0)$
$= (0.5)(0.1) + (0.3)(0.2) + (0.2)(0.7)$
$= 0.25$
$0.42 + 0.33 + 0.25 = 1 \implies \text{Valid PMF}$ 
(b)
$Pr(L = 1) = (0.42)(0.1) + (0.33)(0.4) + (0.8)(0.25) = 0.3740$
(c)
$Pr(L = 1, X = 0) = 0.5((0.1)(0.7) + 0.4(0.2) + 0.8(0.1)) = 0.115$
$Pr(L = 1, X = 1) = 0.3((0.4)(0.7) + 0.8(0.2) + 0.1(0.1)) = 0.135$
$Pr(L = 1, X = 2) = 0.2((0.8)(0.7) + 0.1(0.2) + 0.4(0.1)) = 0.124$
$Pr(L = 1) = 0.3740$ (From previous part)
$Pr(X = 0, L = 1) = \frac{0.115}{0.3740} = 0.3075$
$Pr(X = 1, L = 1) = \frac{0.135}{0.3740} = 0.3610$
$Pr(X = 2, L = 1) = \frac{0.124}{0.3740} = 0.3316$
(d)
$E[x] = 0(0.5) + 1(0.3) + 2(0.2) = 0.7$
$E[X, L = 1] = 0(0.3075) + 1(0.3610) + 2(0.3316) = 1.0242$
$E[X^2, L = 1] = 0^2(0.3075) + 1^2(0.3610) + 2^2(0.3316) = 1.6874$
$Var(X, L = 1) = 1.6874 - (1.0242)^2 = 0.6384$
(e)
$Pr(Y = y, X = x) = Pr(Y = y) \implies \text{Independence}$
$Pr(Y = 0, X = 0) = 0.7$
$Pr(Y = 0) = 0.42$
$0.7 \neq 0.42 \implies \text{Not Independent}$
$Pr(X = x, L = 1) = 0.3610$
$Pr(X = 1) = 3.0$
$0.3 \neq 0.3610 \implies \text{Not Independent}$
(f)
$Cov(X,L) = E[XL] - E[X]E[L]$
$E[XL] = (1.0242)(0.3740) = 0.3831$
$E[X]E[L] = (0.7)(0.3740) = 0.2618$
$Cov(X,L) = 0.3831 - 0.2618 = 0.1213$
Positive Covariance means that Riskier sessions are more likely to be logged
# Question 2

$E[sgn(m-X)] = \int_{-\infty}^{\infty}sgn(m-x)p(x)dx$
$=\int_{-\infty}^{m}p(x)dx - \int_{m}^{\infty}p(x)dx$
$=Pr(X<m) - Pr(X > m)$
$E[sgn(m-X)] = Pr(X<m) - Pr(X > m) = 0$
$Pr(X<m) = Pr(X > m)$
$\implies m \quad \text{Is the median of X}$
# Question 3

$\hat{\mu}_n = \frac1n (\sum_{i = 1}^{n}X_i - \sum_{i = 1}^{n}c) + c$
$= \frac1n \sum_{i = 1}^{n}X_i$ 
Meaning the estimator is just the sample mean
$\tilde{\mu}_n = \overline{X}$

(a)
$E[\hat{\mu}_n] = \frac1n \sum_{i = 1}^{n}(E[X_i -c]) +E[c]$
$= \mu - c + c = \mu$
$E[\hat{\mu}_n] = \mu$
Meaning this is unbiased $\forall c \in \mathbb{R}$
(b)
The variance of the sample mean is $\frac{\sigma^2}{n}$
(c)
Since they are the same thing they have the same variance
The choice of $c$ does not affect the variance since $c$ does not matter in the estimator equation
# Question 4

(a)
Standard one:
$Bias(V) = \frac{n-1}{n}\sigma^2 - \sigma^2 = -\frac1n \sigma^2$
$MSE(V) = (-\frac1n \sigma^2)^2 + \frac{2(n-1)}{n^2}\sigma^4$
$= \frac{2n-1}{n^2}\sigma^4$
The unbiased one:
$Bias(V) = 0$
$MSE(V) = \frac{2}{n-1}\sigma^4$

check
$\frac{2n-1}{n^2}\sigma^4 \stackrel{?}{<} \frac{2}{n-1}\sigma^4$
$-3n + 1 \stackrel{?}{<} 0$
$n > \frac13$
which is always true since $n$ must be $> 1$
Therefore the biased one has a lower MSE
(b)
$0.01 \geq 2e^{-2n(0.02)^2}$
$0.01 \geq 2e^{-0.0008n}$
$e^{-0.0008n} \leq 0.005$
$-0.0008n \leq ln(0.005)$
$n \geq \frac{5.298}{0.0008}$
$n \geq 6622.5$













