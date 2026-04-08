# Question 1

(a)

$P(D|w) = \Pi_{i=1}^np(y_i|x_i,w) = \Pi_{i=1}^n \sigma(x_i^{\intercal}w)^{y_i}(1 -\sigma(x_i^{\intercal}w))^{1-y_i}$
$-ln (P(D|w)) = -\Sigma_{i=1}^n y_iln (\sigma(x_i^{\intercal}w))(1-y_i)ln((1 -\sigma(x_i^{\intercal}w)))$
$ln (P(D|w)) = c(w) =\frac1n \Sigma_{i=1}^n[-y_iln(\sigma(x_i^{\intercal}w)-(1-y_i)ln(1 -\sigma(x_i^{\intercal}w))]$
$ln(\sigma(x_i^{\intercal}w)) = -ln(1+e^{-x_i^{\intercal}w})$
$ln(1 -\sigma(x_i^{\intercal}w) = -ln(1+e^{x_i^{\intercal}w})$
$c(w) =\frac1n \Sigma_{i=1}^n[y_iln(1+e^{-x_i^{\intercal}w})+(1-y_i)ln(1+e^{x_i^{\intercal}w})]$
$c(w) =\frac1n \Sigma_{i=1}^n[y_iln(1+e^{x_i^{\intercal}w})- y_ix_i^{\intercal}w+(1-y_i)ln(1+e^{x_i^{\intercal}w})]$
$c(w) = \frac1n \Sigma_{i=1}^n[ln(1+e^{x_i^{\intercal}w})- y_ix_i^{\intercal}w]$

(b)

$\sigma(x_i^{\intercal}w) \geq 0.75$
$\frac1{1+e^{-x_i^{\intercal}w}} \geq 0.75$
$0.25 \geq 0.75e^{-x_i^{\intercal}w}$
$1/3 \geq e^{-x_i^{\intercal}w}$
$ln(1/3) \geq -x_i^{\intercal}w$
$ln(1/3) \leq x_i^{\intercal}w$
$C = ln(1/3)$

(c)
(i)
$c_{reg}(w) = \frac1n \Sigma_{i=1}^n[ln(1+e^{x_i^{\intercal}w})- y_ix_i^{\intercal}w] + \frac\lambda2 \Sigma^d_{i=1}(w_i^2)$
(ii)
$\frac{\partial }{\partial w}ln(1+e^{x_i^{\intercal}w}) = \sigma(x_i^{\intercal}w)x_i$
$\frac{\partial }{\partial w}y_ix_i^{\intercal}w = y_ix_i$
$\frac{\partial }{\partial w}( \frac\lambda2 \Sigma^d_{i=1}(w_i^2)) = \lambda(0 || w) = (0, \lambda w_1, \lambda w_2, \dots, \lambda w_d)$
$\nabla c_{reg}(w) = \frac1n \Sigma_{i=1}^n(\sigma(x_i^{\intercal}w) - y_i)x_i + \lambda(0||w))$
(iii)
$w_{t+1} = w_t - n(\frac1n \Sigma_{i=1}^n(\sigma(x_i^{\intercal}w) - y_i)x_i + \lambda(0||w)))$
(iv)

Feature weights go through both regularization and the data gradient step but the intercept only goes through the data gradient step since for i = 0 the term vanishes. This lets the intercept more accuratly capture the prior.

# Question 2

(a)

$f^*(x) = x^2$
$f^*(-1) = 1$
$f^*(0) = 0$
$f^*(1) = 1$

(b)

$G = E[(w_0 + w_1X − Y )^2]$
$G = \frac13 \sum_{\{-1,0,1\}}E[(w_0 + w_1x − Y )^2 | X = x]$
$G = \frac13 \sum_{\{-1,0,1\}}1 +(w_0 + w_1x-x^2)^2$
$G = (1 + \frac13)((w_0-w_1-1)^2 + w_0^2 + (w_0 + w_1 - 1)^2)$

$\frac{\partial G}{\partial w_0} = \frac23 ((w_0-w_1-1) + w_0 + (w_0 + w_1 - 1)) = 0$
$w_0 = \frac23$
$\frac{\partial G}{\partial w_1} = \frac23(- (w_0-w_1-1)+ (w_0 + w_1 - 1))$
$w_1 = 0$

so best linear is $f^*(x) = \frac23 + 0x = \frac23$

(c)

normal dist centered at 0 and 1 and then a line in the middle of each of them and then a line at 2/3

(d)

irreducible error is just E(VAR) and that's just 1
reducible is $E[(\frac23 - X^2)^2]$
$= \frac13 [(E[(\frac23 - (-1)^2)^2]) + (E[(\frac23 - (0)^2)^2]) + (E[(\frac23 - (1)^2)^2])]$
$= \frac13(\frac19 + \frac49 + \frac19) =\frac29$

total cost $= 1 + \frac29$

(e) 

given the best predictor is x^2, a quadradic fit can model it perfectly so the reducible error goes to 0 but the irreducible error stays at 1 given it's name so total error is 1

# Question 3

(a)

Model A overfits given the difference between the losses is quite high and the training loss is extremely low while the testing loss is quite high

(b)

(i)
$45 \pm 2.064\frac{10}{\sqrt{25}} = (40.872,49.128)$
(ii)
$38 \pm 2.064\frac{8}{\sqrt{25}} = (34.6976,41.3024)$
(iii)
There is a slight overlap around 41 but that doesn't imply anything about statistical difference you would need the CI of their difference to do that

(c)

(i)

NULL: $\mu_{d} = 0$
ALT: $\mu_{d}> 0$

$t = \frac{7}{3/\sqrt{25}} = 11.6666666667$

(ii)

This means there is very high evidence against the null hypothesis, at $\alpha = 0.05$ we reject the null in favor of the alternative

(iii)

$7 \pm 2.064\frac{3}{\sqrt{25}} = (5.7616, 8.2384)$

zero is not in the confidence interval which leads to the same conclusion as (ii), statistical signifigance of difference

(d)

(i)

$\alpha' = 2+5 = 7$
$\beta' = (50-5) + 2 = 47$

$E[X] = \frac7{7+47} = 0.12962962963$

(ii)

normal dist

# Question 4

(a)

(i)

$f^*(x) = x^2 + 10$

(ii)

reducible is affected since the irreducible cannot be reduced, in other words it's irreducible

(b)

(i)

as d gets much larger than n you get overfitting, the training loss become really low while the testing loss becomes really high

(ii)

the intercept is just meant to be an offset so it shouldn't be affected by regularization so that it can capture the prior better

(iii)

who knows

(c)

(i)

$p(T_i | x_i, w ) = \sigma(w^{\intercal} x_i )^{T_i}(1-\sigma (w^{\intercal} x_i ))^{1-T_i}$
$L(w) = -\frac1n \Sigma_{i = 1}^n[T_iln(\sigma(w^{\intercal} x_i )) + (1-T_i)ln((1-\sigma (w^{\intercal} x_i )))]$

(ii)

$s^2 = 0.12(1-0.12) = 0.1056$
$SE = \sqrt{\frac{0.1056}{64}} = 0.0406201920232$

$CI = 0.12 \pm 2(0.0406201920232) = (0.0387596159536, 0.201240384046)$