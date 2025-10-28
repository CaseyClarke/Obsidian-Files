# Question 1

$m_A = \frac{m_td_1sin(90)}{d_1+d_2} = \frac{(1.850)(0.041)}{0.16} = 0.4740625$

$m_A = 0.4740625$

$\delta m_td_1 = \left|m_td_1\right| \sqrt{(\frac{\delta m_t}{m_t})^2 + (\frac{\delta d_1}{d_1})^2}$
$\delta m_A = \left|\frac{m_t d_1}{d_1 + d_2}\right| \sqrt{ \left( \frac{\delta (m_t d_1)}{m_t d_1} \right)^2 + \left( \frac{\delta (d_1+d_2)}{d_1+d_2}\right)^2 }$
$\delta m_A = \left| \frac{m_t d_1}{d_1 + d_2} \right| \sqrt{ \left( \frac{|m_t d_1| \sqrt{\left(\frac{\delta m_t}{m_t}\right)^2 + \left(\frac{\delta d_1}{d_1}\right)^2}}{m_t d_1} \right)^2 + \left( \frac{\delta (d_1+d_2)}{d_1+d_2} \right)^2 }$
$\delta m_A = \left|m_A\right|\sqrt{(\frac{\delta m_t}{m_t})^2 + (\frac{\delta d_1}{d_1})^2 + (\frac{\delta (d_1+d_2)}{d_1+d_2})^2}$ 
$\delta m_A = \left|0.4740625\right|\sqrt{(\frac{0.020}{1.850})^2 + (\frac{0.01}{0.041})^2 + (\frac{0.01}{0.16})^2} = 0.119470826295$  

$\delta m_A = 0.119470826295 \space kg$
$m_A = 0.5 \pm 0.1 \space kg$

We found $\delta m_t$ by balancing the arm and then adding weight until the bubble moved for us that was 20 grams or 0.02 kg
# Question 2

$m_td_1 sin(50) - m_A(d_1+d_2) = 0$
$m_t(0.041)(0.766) = 0.4740625(0.16)$
$m_t= \frac{0.4740625(0.16)}{0.041(0.766)} = 2.41514360313 \space kg$
$m_t = 2.41514360313 \space kg$
We found $m_{t,exp} = 2.370 \space kg$ with $\delta m_{t,exp} = 0.08 \space kg$
so $m_{t,exp} = 2.37 \pm 0.08 \space kg$
Given our massive uncertainty, the experimental value of $m_t$ is within 1 error interval from the expected value so we are in good agreement with it

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
$m_t =  2.41514360313 \space kg$
We found $m_{t,exp} = 2.350 \space kg$ with $\delta m_{t,exp} = 0.03 \space kg$
so $m_{t,exp} = 2.35 \pm 0.03 \space kg$
The experimental value of $m_t$ is within 3 error interval from the expected value so we are in disagreement with it. 
The only thing that actually (mathematically) changed from Q2 to Q4 was us measuring the uncertainty more accurately and a slight difference in $m_t$ measurement. The angle is different but the forces are the same.

# Question 5

There shouldn't have been any difference in the $m_t$ needed to balance it since $sin(130) = sin(50)$
but we measured a slight difference probably due to the stiffness of the arm. The real difference though was the type of equilibria, at $\theta = 50$ the arm was at a stable equilibrium, if you added more than the required weight to balance it would slowly go up and if you didn't add enough it would slowly go down. While at $\theta = 130$ the arm is at an unstable equilibrium, any slight movement up or down will snap the arm shut in the direction it was moving. 

# Question 6
$m_td_1 sin(50) - m_l(d_1+ d_2+d_3) - m_A(d_1+d_2) = 0$
$m_t(0.041)(0.766) - (0.150)(0.314) - 0.4740625(0.16) = 0$
$m_t = \frac{(0.150)(0.314) + 0.4740625(0.16)}{(0.041)(0.766)} = 3.91485703369$
$m_t = 3.91485703369 \space kg$

$m_{t,exp} = 5.0 \pm 0.2$

$T = m_tg$
$\sum F_{x} = 0 \implies F_{E,x} = T_x = cos(50)m_tg$
$\sum F_{y} = 0 \implies F_{E,y} + F_L + F_G = T_y$
$F_{E,y} = T_y - F_L - F_G = sin(50)m_tg - m_Lg - m_Ag$

$F_E = \sqrt{F_{E,x}^2 + F_{E,y}^2}$
$F_E = \sqrt{(cos(50)m_tg)^2 + (sin(50)m_tg - m_Lg - m_Ag)^2}$
$F_E = \sqrt{(cos(50)(3.91485703369)(9.81))^2 + (sin(50)(3.91485703369)(9.81) -}$
$\overline{- (0.150)(9.81) - (0.4740625)(9.81))^2} = 40.4447915943$
$F_E = 40.4447915943 \space N$

Both the force and the tension are almost doubled by only adding 150 grams as the load, this shows how much work it takes to hold even a small object in your hand with your arm outstretched

# Question 7

$m_td_1 sin(70) - m_l(d_1+ d_2+d_3) - m_A(d_1+d_2) = 0$
$m_t(0.041)(0.939692621) - (0.150)(0.314) - 0.4740625(0.16) = 0$
$m_t = \frac{(0.150)(0.314) + 0.4740625(0.16)}{(0.041)(0.939692621)} = 3.19123553893$
$m_t = 3.19123553893 \space kg$
$m_{t,exp} = 4.0 \pm 0.1$


# Question 8

It is a fairly good approximation of a human arm since it approximates the major important parts of the arm however, it does ignore some of the smaller details such as the hand being separate from the forearm and the singular muscle instead of the many muscles in the real arm. Although I don't actually think that this affects the model all that much as those smaller details add really small effects and the model accurately captures the main joints and the main muscle of the arm.
The main thing I would change would be to add a wrist joint and another "muscle" attached to the wrist, since the current apparatus only factors in the forces required to hold an object by your bicep and ignores the fact that (at least in my own personal experience) the difficulty of holding a weight with your arm outstretched comes more from keeping your wrist straight with the forearm muscle than the bicep.

# Question 9
Acknowledgements: 
- Adam Connaghan and Nikola Uletilovic (lab partners)
- I collaborated with the above people for the collection of data, all analysis in this document is my own 

References:
- Isaac, et al. 2025. Lab Manual PHYS 124. Edmonton: University of Alberta, Department of Physics.


# Appendix

Raw Data:

| $\theta(degrees)$ | $m_L(kg)$ | $m_t(kg)$ | $\delta m_t(kg)$ |
| ----------------- | --------- | --------- | ---------------- |
| 90                | 0         | 1.850     | 0.020            |
| 50                | 0         | 2.370     | 0.08             |
| 130               | 0         | 2.350     | 0.03             |
| 50                | 0.150     | 4.950     | 0.150            |
| 70                | 0.150     | 3.970     | 0.100            |

