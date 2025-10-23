# Question 1

$m_A = \frac{m_td_1sin(90)}{d_1+d_2} = \frac{(1.850)(0.041)}{0.16} = 0.4740625$
$\delta m_td_1 = \left|m_td_1\right| \sqrt{(\frac{\delta m_t}{m_t})^2 + (\frac{\delta d_1}{d_1})^2}$
$\delta m_A = \left|\frac{m_t d_1}{d_1 + d_2}\right| \sqrt{ \left( \frac{\delta (m_t d_1)}{m_t d_1} \right)^2 + \left( \frac{\delta (d_1+d_2)}{d_1+d_2}\right)^2 }$
$\delta m_A = \left| \frac{m_t d_1}{d_1 + d_2} \right| \sqrt{ \left( \frac{|m_t d_1| \sqrt{\left(\frac{\delta m_t}{m_t}\right)^2 + \left(\frac{\delta d_1}{d_1}\right)^2}}{m_t d_1} \right)^2 + \left( \frac{\delta (d_1+d_2)}{d_1+d_2} \right)^2 }$
$\delta m_A = \left| \frac{m_t d_1}{d_1 + d_2} \right| \sqrt{ \left(\frac{\delta m_t}{m_t}\right)^2 + \left(\frac{\delta d_1}{d_1}\right)^2 + \left( \frac{\delta (d_1+d_2)}{d_1+d_2} \right)^2 }$
$\delta m_A = \left|m_A\right|\sqrt{(\frac{\delta m_t}{m_t})^2 + (\frac{\delta d_1}{d_1})^2 + (\frac{\delta (d_1+d_2)}{d_1+d_2})^2}$ 
$\delta m_A = \left|0.4740625\right|\sqrt{(\frac{0.020}{1.850})^2 + (\frac{0.01}{0.041})^2 + (\frac{0.01}{0.16})^2} = 0.119470826295$  

$m_A = 0.5 \pm 0.1 \space kg$

We found $\delta m_t$ by balancing the arm and then adding weight until the bubble moved for us that was 20 grams or 0.02 kg
# Question 2

$m_td_1 sin(50) - m_A(d_1+d_2) = 0$
$m_t(0.041)(0.766) = 0.4740625(0.16)$
$m_t= \frac{0.4740625(0.16)}{0.041(0.766)} = 2.41514360313 \space kg$
We found $m_{t,exp} = 2.370 \space kg$ with $\delta m_{t,exp} = 0.08 \space kg$
so $m_{t,exp} = 2.37 \pm 0.08 \space kg$
Given our massive uncertainty, the experimental value of $m_t$ is within 1 error interval from the expected value so we are in agreement with it

# Question 3
$T = m_tg$
$\sum F_{x} = 0 \implies F_{E,x} = T_x = cos(50)m_tg$
$\sum F_{y} = 0 \implies F_{E,y} + F_L + F_G = T_y$
$F_{E,y} = T_y - F_L - F_G = sin(50)m_tg - 0 - m_Ag$
$F_E = \sqrt{F_{E,x}^2 + F_{E,y}^2} = \sqrt{(cos(50)m_tg)^2 + (sin(50)m_tg - m_Ag)^2}$
$F_E = \sqrt{(cos(50)(2.370)(9.81))^2 + (sin(50)(2.370)(9.81) - (0.4740625)(9.81))^2} = 24.8779865232$
$F_E = 24.8779865232 \space N$

# Question 4
Exact same derivation as Q2
$m_td_1 sin(50) - m_A(d_1+d_2) = 0$
$m_t(0.041)(0.766) = 0.4740625(0.16)$
$m_t= \frac{0.4740625(0.16)}{0.041(0.766)} = 2.41514360313 \space kg$
We found $m_{t,exp} = 2.350 \space kg$ with $\delta m_{t,exp} = 0.03 \space kg$
so $m_{t,exp} = 2.35 \pm 0.03 \space kg$
The experimental value of $m_t$ is within 3 error interval from the expected value so we are in disagreement with it. 
The only thing that actually changed from Q2-Q4 was us measuring the uncertainty more accurately

# Question 5

There shouldn't have been any difference in the $m_t$ needed to balance it since $sin(130) = sin(50)$
but we measured a slight difference probably due to the stiffness of the arm. The real difference though was the type of equilibria, at $\theta = 50$ the arm was at a stable equilibrium, if you added more than the required weight to balance it would slowly go up and if you didn't add enough it would slowly go down. While at $\theta = 130$


$m_t = \frac{m_A(d_1+d_2)}{d_1sin(50)}$

$T = m_tg$
$\sum F_{x} = 0 \implies F_{E,x} = T_x$
$\sum F_{y} = 0 \implies F_{E,y} + F_L + F_G = T_y$
$F_E = \sqrt{F_{E,x}^2 + F_{E,y}^2}$

| $\theta(degrees)$ | $m_L(kg)$ | $m_t(kg)$ | $\delta m_t(kg)$ |
| ----------------- | --------- | --------- | ---------------- |
|                   |           |           |                  |
|                   |           |           |                  |
| 90                | 0         | 1.850     | 0.020            |
| 50                | 0         | 2.370     | 0.08             |
| 130               | 0         | 2.350     | 0.03             |
| 50                | 0.150     | 4.950     | 0.150            |
| 70                | 0.150     | 3.970     | 0.100            |

$m_t = \frac{m_L(d_1 + d_2 + d_3) + m_A(d_1+d_2)}{d_1sin(\theta)}$
full equation with load