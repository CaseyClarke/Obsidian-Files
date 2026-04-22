# Question 1

(a)

$\nabla c_z(w) = (wx_z-y_z)x_z$
$E(\nabla c_z(w)) = \sum^n_{z=1}P(J=z)\nabla c_z(w) = \frac1n \sum_{z=1}^n \nabla c_z(w)$
$\frac1n \sum_{z=1}^n \nabla c_z(w) = \nabla c(w)$
$E(\nabla c_z(w)) = \nabla c(w)$

(b)

$\nabla c_3(w^{(1)}) = (0(3)-9)3 = -27$
$w^{(1)} = 0 - 0.1(-27) = 2.7$

$\nabla c_1(w^{(2)} = (2.7(1)-2)1 = 0.7$
$w^{(2)} = 2.7 - 0.1(0.7) = 2.63$

(c)

Near the optimum $w^*$ the gradients have small magnitude because $G(t)$ is increasing as t increases meaning that $\beta_t$ decreases. This means that as the training goes on the step size becomes smaller and smaller, leading to larger steps when we are further from the value and more precision as we get closer to $w^*$. With a large fixed step size it will overshoot the optimum repeatedly causing oscillation around the value.

# Question 2

(a)
$w_{t+1} - w_t = -n\nabla J(w_t)$
$J(w_{t+1}) \leq J(w_t) + \nabla(w_t)^\intercal(-n\nabla J(w_t)) + \frac{L}{2} ||-n\nabla J(w_t)||^2$
$J(w_{t+1}) \leq J(w_t) + -n||\nabla J(w_t)||^2 + \frac{Ln^2}{2} ||\nabla J(w_t)||^2$
$J(w_{t+1}) \leq J(w_t) + (\frac{Ln^2}{2} -n) ||\nabla J(w_t)||^2$
$n = \frac1L$
$J(w_{t+1}) \leq J(w_t) + (\frac{Ln^2}{2} -n) ||\nabla J(w_t)||^2$
$J(w_{t+1}) \leq J(w_t) - \frac{1}{2L} ||\nabla J(w_t)||^2$
norm is positive so 
$J(w_{t+1}) \leq J(w_t)$

(b) 

$b= 1$
if you only take one random sample each time SGD is very sensitive to noise so if you happen to get a sample that isn't a great representation of the whole dataset it might throw off your value temporarily and if this happens over and over again it causes oscillations

$b = n$
There is no random noise to throw off the calculations so the calculations are always going to be smoothly going towards the optimum

# Question 3

(a)

$T = n \times 1\mu s = 10 s$
10 seconds

(b)

Full-Batch
$T = 100 \times 10s = 1000s$
1000 seconds

SGD
$T = 10000 \times 1\mu s = 0.01s$
0.01seconds

pretty obvious that SGD is magnitudes faster than full batch

# Question 4

(a)

gradient:
$\frac{\partial}{\partial w_i}f(w) = \frac12(A+A^\intercal)w = Aw$

hessian:
$\nabla^2 f(w) = A$

(b)

$w^{(t+1)} = w^{(t)} - \alpha Aw^{(t)} = (I-\alpha A)w^{(t)}$

if $\alpha$ is large it might cause oscillations around the optimum value and if large enough it can overpower the contributions of the previous values and cause the oscillations to get more and more intense, thus causing the algorithm to diverge

(c)

(i)
$w^{(t+1)} = w^{(t)} - (A)^{-1}Aw^{(t)}$
(ii)
$w^{(t+1)} = 0$
(iii)
Newton's method fits a second order and given the function is a quadratic it's not an approximation it's exact so it just "skips" to the minimum in one step











