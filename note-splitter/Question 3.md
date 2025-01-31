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