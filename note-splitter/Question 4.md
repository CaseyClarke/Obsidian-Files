# Question 4

(a)

- $\text{Estimate} = \mu_\text{hotels} - \mu_\text{cabins} = 5.6555 - 4.6152 = 1.0403$
- $n = n_1,n_2 = 20$
- $df = 2n-2 = 38$
- $S_p = \sqrt{\frac{(n-1)(S_1)^2+(n-1)(S_2)^2}{2n-2}} = \sqrt{\frac{(19)(0.1451)^2+(19)(0.18008)^2}{38}}$
- $\Rightarrow 0.1635$
- $SE(\text{Estimate}) = s_p\sqrt{\frac{2}{n}} = 0.1635\sqrt{\frac{1}{10}} = 0.05170$
- $C.V. = t^*_{df,a/2} = t^*_{38, 0.05} = 1.697$
- $\mu_d \pm  t^*_{38,0.05}SE({\text{Estimate}})$
- $\Rightarrow 1.0403 \pm 1.697(0.05170) = (0.9525651, 1.1280349)$
- Back transformed C.I. $= (e^{0.9525651}, e^{1.1280349}) = (2.59235077709, 3.08957919874)$

(b)

- Since this is a back transformed $ln(x)$ C.I. to test for equal means we check if 1 is in the C.I. Given that $1$ is not in the confidence interval we can say with $90\%$ confidence that there is sufficient evidence to conclude a difference between the two means