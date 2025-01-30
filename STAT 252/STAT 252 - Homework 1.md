# Question 1

(a)

- Tomato Crop Plots

(b)

- Irrigation levels - Ordinal - $mm$
- Fertilizer type - Categorical - $A\lor B$

(c)

- Yield per Plot - Continuous- $kg/m^2$

(d)

- This is an experimental study as the researchers are actively manipulating variables

(e)

- Causal inferences are possible as there is random allocation
- Population inferences are not possible as there is no indication that these plots are indicative of some larger population

{{ENDQUESTION}}

# Question 2

(a)

- (i) 
	- A t-test is the most appropriate where the sample is $\mu_{2019}$
- (ii) 
	- $H_0 : \mu_{2019} = 279$
	- $H_A : \mu_{2019} \neq 279$
- (iii) 
	- $\text{Estimate} = \bar{y} = 305.72$
	- $\mu = 279$
	- $s = 40.05$
	- $n = 12$
	- $SE(\bar{y}) = \frac{s}{\sqrt{n}} = \frac{40.05}{\sqrt{12}} = 11.5614$
	- $t = \frac{\bar{y}- \mu}{SE(\bar{y})} = \frac{305.72- 279}{11.5614} = 2.31113$
- (iv)
	- $df = n-1 = 11$
	- $p \in  (0.04, 0.05) \implies$ strong to moderate evidence against $H_0$
	- $p < a = 0.05 \implies$ we reject the null hypothesis 
- (v)
	- At a significance level of $0.05$ we reject the claim that the average cost of residential electrical bills in 2019 is the same as the average cost of residential electrical bills in 2017

(b)

- Variables are carried over from the previous part, only change is $a = 0.01$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{11,0.005} = 3.106$
- (ii)
	- $\bar{y} \pm  t^*_{11,0.005}SE({\bar{y}}) = 305.72 \pm  (3.106)11.5614 = (269.8103, 341.6297)$
- (iii) 
	- given that $279$ is in the confidence interval we can say with $99\%$ confidence that there is insufficient evidence to conclude a difference between the two means

(c)

- They gave different conclusions as part(a) had a much less strict confidence level compared to part (b), the strength of the evidence did not change, just our level of confidence

{{ENDQUESTION}}

# Question 3

### Experiment 1

(a)

- A pooled t-test would be the most appropriate in this situation with $H_0 : \mu_\text{Treatment} - \mu_\text{Control} = 0$ and $H_A : \mu_\text{Treatment} - \mu_\text{Control} > 0$  as the samples are Independent and randomly sampled and allocated which implies that the variances are equal. 
- The assumptions are as follows
	- Independent random samples - This is true from the experiment design
	- Normality - Given that the population and sample sizes are large enough we can assume normality
	- Equal Variability - Can be assumed from the fact that samples are independent

(b)

- (i) 
	- From part (a)
- (ii) 
	- From part (a)
- (iii) 
	- $\text{Estimate} = \mu_\text{Treatment} - \mu_\text{Control} = 6.0667$
	- $n = n1 , n2 = 30$
	- $SE(\text{Estimate}) = s_p\sqrt{\frac{2}{n}} = 19.8537\sqrt{\frac{1}{15}} = 5.1262$
	- $t = \frac{\mu_\text{Treatment} - \mu_\text{Control}}{SE(\text{Estimate})} = \frac{6.0667}{5.1262} = 1.1835$
- (iv)
	- $df = 2n-2 = 58$
	- $p \in  (0.1, 0.15) \implies$ strong to moderate evidence against $H_0$
	- $p > a = 0.01 \implies$ we fail reject the null hypothesis 
- (v)
	- At a significance level of $0.01$ we fail reject the claim that the treatment does not raise the platelet count significantly

(c)

- Variables are carried over from the previous part, only change is $a = 0.05$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{58,0.025} = 2.009$
- (ii)
	- $\mu_\text{Treatment} - \mu_\text{Control} \pm  t^*_{58,0.025}SE({\text{Estimate}})$
	- $\Rightarrow 6.0667 \pm 2.009(5.1262) = (-4.2318358, 16.3652358)$
- (iii) 
	- given that $0$ is in the confidence interval we can say with $95\%$ confidence that there is not sufficient evidence to conclude a difference between the two means


### Experiment 2

(d)

- A paired t-test would be the most appropriate in this situation with $H_0 : \mu_d = 0$ and $H_A : \mu_d > 0$  as the samples are Independent and randomly sampled and allocated which implies that the variances are equal. 
- The assumptions are as follows
	- Independent random samples - This is true from the experiment design
	- Normality - Given that the population and sample sizes are large enough we can assume normality
	- Paired Measurements - Given from the "Before and After" design of the experiment

(e)

- (i) 
	- From part (d)
- (ii) 
	- From part (d)
- (iii) 
	- $\text{Estimate} = \mu_d = 3.7667$
	- $n = 30$
	- $SE(\text{Estimate}) = \frac{S_d}{\sqrt{n}} = \frac{5.6366}{\sqrt{30}} = 1.0291$
	- $t = \frac{\mu_d}{SE(\text{Estimate})} = \frac{3.7667}{1.0291} = 3.6602$
- (iv)
	- $df = n-1 = 29$
	- $p <  0.0005 \implies$ convincing to strong evidence against $H_0$
	- $p < a = 0.01 \implies$ we reject the null hypothesis 
- (v)
	- At a significance level of $0.01$ we reject the claim that the treatment does not raise the platelet count significantly

(f)

- Variables are carried over from the previous part, only change is $a = 0.05$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{29,0.025} = 2.045$
- (ii)
	- $\mu_d \pm  t^*_{29,0.025}SE({\text{Estimate}})$
	- $\Rightarrow 3.7667 \pm 2.045(1.0291) = (1.6621905, 5.8712095)$
- (iii) 
	- given that $0$ is in not the confidence interval we can say with $95\%$ confidence that there is sufficient evidence to conclude a difference between the two means

(g)

- Since they are different trials the difference in experiment design and random chance with respect to the effect on the study participants is probably why the answers are different

{{ENDQUESTION}}
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

{{ENDQUESTION}}
# Question 5

(a)

A Mann-Witney U test with
$H_0 : \text{There is no difference in the amount of hours spent watching horror movies between youth and adults}$
$H_A : \text{There is a difference in the amount of hours spent watching horror movies between youth and adults}$
would be the most appropriate here as the Shapiro-Wilk test for normality on the youth group for both the logged and original data is less than $0.05$ which means we cannot assume normality for either and the data is not paired, there are no assumptions for this test

(b)

| Sample 1 | Sample 2 | Rank 1   | Rank 2 |
| -------- | -------- | -------- | ------ |
| 0        | 0        | 2.5      | 2.5    |
| 1        | 0        | 6        | 2.5    |
| 1        | 0        | 6        | 2.5    |
| 2        | 1        | 8.5      | 6      |
| 3        | 2        | 10.5     | 8.5    |
| 5        | 3        | 13       | 10.5   |
| 8        | 4        | 14       | 12     |
| 12       | 9        | 16       | 15     |
| 18       | 13       | 18       | 17     |
| 22       | 20       | 20       | 19     |
| 26       | 28       | 21       | 22     |
| 39       | 29       | 26       | 23     |
| 42       | 30       | 27       | 24     |
| 44       | 33       | 28       | 25     |
| 47       |          | 29       |        |
| 48       |          | 30       |        |
| 49       |          | 31       |        |

- (i) 
	- From part (a)
- (ii) 
	- From part (a)
- (iii) 
	- $M_1 = 306.5$
	- $n_1 = 17$
	- $n_2 = 14$
	- $\mu_M = \frac{n_1(1+n_1+n_2)}{2} =  \frac{17(1+14+17)}{2} = 272$
	- $SE(M) = \sqrt{\frac{n_1n_2(1+n_1+n_2)}{12}} = \sqrt{\frac{(14)(17)(1+14+17)}{12}} = 25.1926$
	- $Z^*_0 = \frac{M_1 - \mu_M}{SE(M)} = \frac{306.5 - 272}{25.1926} = 1.3694$
- (iv)
	- $p =  0.1706 \implies$ weak evidence against $H_0$
	- $p < a = 0.1 \implies$ we fail to reject the null hypothesis 
- (v)
	- At a significance level of $0.1$ we fail to reject that claim that there is no difference in the amount of hours spent watching horror movies between youth and adults


