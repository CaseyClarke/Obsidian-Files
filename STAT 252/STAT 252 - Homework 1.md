# Question 1

(a)

- Tomato Crop Plots

(b)

- Irrigation levels - Ordinal - $mm$
- Fertilizer type - Categorical - $A\lor B$

(c)

- Yield per Plot - Ordinal - $kg/m^2$

(d)

- This is an experimental study as the researchers are actively manipulating variables

(e)

- Causal inferences are possible as there is random allocation
- Population inferences are not possible because idk man i feel like it

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
	- $SE(\text{Estimate}) = s_p\sqrt{\frac{1}{2n}} = 19.8537\sqrt{\frac{1}{60}} = 2.5631$
	- $t = \frac{\mu_\text{Treatment} - \mu_\text{Control}}{SE(\text{Estimate})} = \frac{6.0667}{2.5631} = 2.3669$
- (iv)
	- $df = 2n-2 = 58$
	- $p \in  (0.01, 0.02) \implies$ strong to moderate evidence against $H_0$
	- $p > a = 0.01 \implies$ we fail reject the null hypothesis 
- (v)
	- At a significance level of $0.01$ we fail reject the claim that the treatment does not raise the platelet count significantly

(c)

- Variables are carried over from the previous part, only change is $a = 0.05$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{58,0.025} = 2.009$
- (ii)
	- $\mu_\text{Treatment} - \mu_\text{Control} \pm  t^*_{58,0.025}SE({\text{Estimate}})$
	- $\Rightarrow 6.0667 \pm 2.009(2.3669) = (1.3115979, 10.8218021)$
- (iii) 
	- given that $0$ is in not the confidence interval we can say with $95\%$ confidence that there is sufficient evidence to conclude a difference between the two means


### Experiment 2

(d)

- A paired t-test would be the most appropriate in this situation with $H_0 : \mu_d = 0$ and $H_A : \mu_d > 0$  as the samples are Independent and randomly sampled and allocated which implies that the variances are equal. 
- The assumptions are as follows
	- Independent random samples - This is true from the experiment design
	- Normality - Given that the population and sample sizes are large enough we can assume normality
	- Paired Measurements - Given from the "Before and After" design of the experiment

(e)

- (i) 
	- From part (a)
- (ii) 
	- From part (a)
- (iii) 
	- $\text{Estimate} = \mu_d = 3.7667$
	- $n = 30$
	- $SE(\text{Estimate}) = \frac{S_d}{\sqrt{n}} = \frac{5.6366}{\sqrt{30}} = 1.0291$
	- $t = \frac{\mu_d}{SE(\text{Estimate})} = \frac{3.7667}{1.0291} = 3.6602$
- (iv)
	- $df = n-1 = 29$
	- $p <  0.0005 \implies$ convincing to strong evidence against $H_0$
	- $p < a = 0.01 \implies$ we fail reject the null hypothesis 
- (v)
	- At a significance level of $0.01$ we reject the claim that the treatment does not raise the platelet count significantly

(f)

- Variables are carried over from the previous part, only change is $a = 0.05$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{29,0.025} = 2.756$
- (ii)
	- $\mu_d \pm  t^*_{29,0.025}SE({\text{Estimate}})$
	- $\Rightarrow 3.7667 \pm 2.756(1.0291) = (0.9305004, 6.6028996)$
- (iii) 
	- given that $0$ is in not the confidence interval we can say with $95\%$ confidence that there is sufficient evidence to conclude a difference between the two means

(g)

- Since we got the same answer for both parts that would suggest that the drug does actually have the proposed affect

{{ENDQUESTION}}

# Question 4

(a)

- $\text{Estimate} = \mu_\text{hotels} - \mu_\text{cabins} = 5.1353$
- $n = n_1,n_2 = 20$
- $SE(\text{Estimate}) = s_p\sqrt{\frac{1}{2n}} = 0.55099\sqrt{\frac{1}{40}} = 0.0871$
- $t = \frac{\mu_\text{hotels} - \mu_\text{cabins}}{SE(\text{Estimate})} = \frac{5.1353}{0.0871} = 3.6602$

- (i)
	- $C.V. = t^*_{df,a/2} = t^*_{29,0.025} = 2.756$
- (ii)
	- $\mu_d \pm  t^*_{29,0.025}SE({\text{Estimate}})$
	- $\Rightarrow 3.7667 \pm 2.756(1.0291) = (0.9305004, 6.6028996)$
- (iii) 
	- given that $0$ is in not the confidence interval we can say with $95\%$ confidence that there is sufficient evidence to conclude a difference between the two means



