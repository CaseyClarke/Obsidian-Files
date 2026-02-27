# Question 1

1.
$p(D|w) = \Pi_{i = 1}^np(y_i|x_i, w) = (2\pi)^{-n/2}e^{(-\frac12 \sum^n_{i = 1}(y_i - wx_i)^2)}$
$-log(p(D|w)) = \frac n2 log(2\pi) + \frac 12 \sum^n_{i = 1}(y_i - wx_i)^2$
Ignoring terms without w
$-log(p(D|w)) = \frac 12 \sum^n_{i = 1}(y_i - wx_i)^2$

2.
$\frac{d}{dw}(-log(p(D|w))) = -\sum^n_{i = 1}x_i(y_i - wx_i) = 0$
$\sum^n_{i = 1}(x_iy_i) = w\sum^n_{i = 1}x^2_i$
$w_{MLE} = \frac{\sum^n_{i = 1}(x_iy_i)}{w\sum^n_{i = 1}x^2_i}$
$w_{MLE} = \frac{(1)(1) + (2)(2) + (3)(2) + (4)(5)}{1^2 + 2^2 + 3^2 + 4^2}$
$w_{MLE} = 1.0\overline{3}$

3.
$-log(p(w|D)) = -log(p(D|w)) - log(p(w)) + c$
$-log(p(D|w)) = \frac 12 \sum^n_{i = 1}(y_i - wx_i)^2$ (from part 1)
$-log(p(w)) = \frac{1}{2\tau^2}w^2 + c$
$w_{MAP} = \frac 12 \sum^n_{i = 1}(y_i - wx_i)^2 + \frac{1}{2\tau^2}w^2$
$\frac{d}{dw}w_{MAP} = -\sum_{i = 1}^nx_iy_i + w \sum^n_{i = 1}x^2_i+ \frac{w}{\tau^2} = 0$
$w_{MAP} = \frac{\sum_{i = 1}^nx_iy_i}{\sum_{i = 1}^n x^2_i + \frac{1}{\tau^2}}$
$w_{MAP} =  \frac{(1)(1) + (2)(2) + (3)(2) + (4)(5)}{1^2 + 2^2 + 3^2 + 4^2 + \frac{1}{4}}$
$w_{MAP} \approx 1.02479$

MLE is only finding the best fit for the current data whereas MAP is doing that while knowing that the value is likely near 0, meaning that he MAP value is going to be lower since it's being "pulled down" towards 0 by the prior being close to 0

4.
$\nabla J(w) = -\sum^n_{i = 1}x_i(y_i - wx_i)$
$\nabla J(w) = 30w - 31$
$w_{t + 1} = w_t - \eta(30w_t - 31)$
$\eta = 0.03, w_0 = 0$
$w_1 = -0.03(-31) = 0.93$
$w_2 = 0.93 - 0.03(30(0.93)- 31) = 1.023$
$w_3 = 1.023 - 0.03(30(1.023)- 31) = 1.0323$
$w_4 = 1.0323- 0.03(30(1.0323)- 31) = 1.03323$

5.

The MLE and Gradient Descent values are very close after only 4 iterations showing that Gradient Descent is correctly converging to the closed form solution. It is useful when there exists a closed form solution as it is often cheaper computationally than the closed form solutions for more complicated inputs.

# Question 2

1.


