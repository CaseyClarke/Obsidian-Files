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

