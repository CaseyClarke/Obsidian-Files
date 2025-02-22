# Question 1

 (a)

- (i)

	- A one-way ANOVA test with 5 means is the most appropriate with the paramaters being $\mu_{A}, \mu_{B}, \mu_{C}, \mu_{D}, \mu_{E}$

- (ii)

	- $H_0: \mu_{A} = \mu_{B} = \mu_{C} = \mu_{D}  = \mu_{E}$
	- $H_A : \text{There are some differences in the means}$

- (iii)


- $n = 30 \text{ (Number of Observations) } \quad a = 5 \text{ (Number of groups) }$ 

| Sales          |       |            | ANOVA Table          |                                    |                       |
| -------------- | ----- | ---------- | -------------------- | ---------------------------------- | --------------------- |
|                | Ss    | df         | Ms                   | F                                  | Sig.                  |
| Between        | 4.083 | $a-1=4$    | $4.083/4 = 1.02075$  | $\frac{1.02075}{0.22472} = 4.5423$ | $p \in (0.025, 0.01)$ |
| Within (error) | 5.618 | $n-a = 25$ | $5.618/25 = 0.22472$ |                                    |                       |
| Total          | 9.702 | $n-1 = 29$ |                      |                                    |                       |

- (iv)

	- $\alpha = 0.05$
	- $p = P(F^{4}_{25} > 4.5423) \in (0.025, 0.01) < \alpha \implies$Reject the null hypothesis


- (v)

	- At a significance level of $0.05$ we reject the claim that the there is no difference in the mean sales between the different stores


(b)

- $S_p = \sqrt{MSE} = \sqrt{0.22472} = 0.47405$

(c)

| E      | D      | C      | B      | A      |
| ------ | ------ | ------ | ------ | ------ |
| 0.900  | 1.333  | 1.183  | 1.783  | 1.883  |
| ------ | ------ | ------ |        |        |
|        | ------ | ------ | ------ |        |
|        |        |        | ------ | ------ |
|        |        |        | ------ | ------ |

(d)

- $n = 30$
- $n_i = n_j = 6$
- $k = 5$
- $MSE = 0.22472 \text{ (From previous part) }$
- $m = \frac{k(k-1)}{2} = \frac{5(5-1)}{2} = 10$
- $\alpha_1 = \frac{\alpha_F}{m} = \frac{0.05}{15} = 0.00334$
- $df = n-k = 30 - 5 = 25$
- $t_{df,\alpha/2} = t_{25,0.025} = 2.060$
- $ME_{ij} = t_{df,\alpha/2}\sqrt{MSE}\sqrt{\frac{2}{n_i}} = 2.06\sqrt{0.22472}\sqrt{\frac{2}{6}} = 0.5638$


|     | A                  | B                  | C                 | D                 | E   |
| --- | ------------------ | ------------------ | ----------------- | ----------------- | --- |
| A   |                    |                    |                   |                   |     |
| B   | $0.1 < 0.5638$     |                    |                   |                   |     |
| C   | $0.7 > 0.5638$*    | $0.6 > 0.5638$*    |                   |                   |     |
| D   | $0.55 > 0.5638$*   | $0.45 < 0.5638$    | $0.15 < 0.5638$   |                   |     |
| E   | $0.9833 > 0.5683$* | $0.8833 > 0.5638$* | $0.2833 < 0.5638$ | $0.4333 < 0.5638$ |     |

| E      | D      | C      | B      | A      |
| ------ | ------ | ------ | ------ | ------ |
| 0.900  | 1.333  | 1.183  | 1.783  | 1.883  |
| ------ | ------ | ------ |        |        |
|        | ------ | ------ | ------ |        |
|        |        |        | ------ | ------ |

(e)

- They are the same but due to the differences in the calcuation of confidence intervals they could have been different as Bonferroni's method produces wider confidence interals while Tukey's produces smaller intervals, in this case though it did not matter as the differences were signifigant enough that they appeared in both tests

(f)

- (i)

	- A t test with would be the most appropriate with paramater
	- $\gamma = \frac{\mu_A + \mu_B}{2} - \frac{\mu_C + \mu_D}{2} = \frac12 \mu_A + \frac12 \mu_B - \frac12 \mu_C - \frac12 \mu_D$

- (ii)

	- $H_0 : \gamma = 0$
	- $H_A : \gamma \neq 0$

- (iii)

	- $\hat{\gamma} = \frac12 (1.883) + \frac12 (1.783) - \frac12 (1.183) - \frac12 (1.333) = 0.575$
	- $s_p = 0.47405 \text{ (From part (b)) }$
	- $n_i = n_j = 6$
	- $SE(\hat{\gamma}) = s_p\sqrt{\frac{(C_1)^2}{n_i} + \frac{(C_2)^2}{n_i} + \frac{(C_3)^2}{n_i} + \frac{(C_4)^2}{n_i}}$
	- $SE(\hat{\gamma}) = 0.47405\sqrt{\frac{(1/2)^2}{6} + \frac{(1/2)^2}{6} + \frac{(-1/2)^2}{6} + \frac{(-1/2)^2}{6}} = 0.1935$
	- $t = \frac{\hat{\gamma}}{SE(\hat{\gamma})} = \frac{0.575}{0.1935} = 2.9716$

- (iv)

	- $df = n-k = 25$
	- $p = 2P(t_{25} > 2.9716) \in (0.01,0.005) \implies$ ==Evidence==
	- $\alpha = 0.05$
	- $p < \alpha \implies$ Reject the null hypothesis

- (v)

	- At a signifigance level of $0.05$ we reject the null hypothesis that there is a signifigant difference in the sales of stores A and B (combined) in comparison with stores C and D (combined)

(g)

- (i)

	- A t test with would be the most appropriate with paramater
	- $\gamma = \mu_E - \frac{\mu_A + \mu_B}{2} = \mu_E -\frac12 \mu_A -\frac12 \mu_B$

- (ii)

	- $H_0 : \gamma = 0$
	- $H_A : \gamma \neq 0$

- (iii)

	- $\hat{\gamma} = 0.9 -\frac12 (1.883) - \frac12 (1.783) = -0.933$
	- $s_p = 0.47405 \text{ (From part (b)) }$
	- $n_i = n_j = 6$
	- $SE(\hat{\gamma}) = s_p\sqrt{\frac{(C_1)^2}{n_i} + \frac{(C_2)^2}{n_i} + \frac{(C_3)^2}{n_i}}$
	- $SE(\hat{\gamma}) = 0.47405\sqrt{\frac{(1)^2}{6} + \frac{(-1/2)^2}{6} + \frac{(-1/2)^2}{6}} = 0.2370$
	- $t = \frac{\hat{\gamma}}{SE(\hat{\gamma})} = \frac{-0.933}{0.2370} = -3.9367$

- (iv)

	- $df = n-k = 25$
	- $p = 2P(t_{25} > -3.9367) \in (0.01,0.005) \implies$ ==Evidence==
	- $\alpha = 0.05$
	- $p < \alpha \implies$ Reject the null hypothesis

- (v)

	- At a signifigance level of $0.05$ we reject the null hypothesis that there is a signifigant difference in the sales of stores A and B (combined) in comparison with stores C and D (combined)

