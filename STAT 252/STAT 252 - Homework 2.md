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
	- $p = P(F^{4}_{25} > 4.5423) \in (0.025, 0.01) \implies$ Weak evidence against the null hypothesis
	- $p < a \implies$Reject the null hypothesis


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

(d)

- $n = 30$
- $n_i = n_j = 6$
- $k = 5$
- $MSE = 0.22472 \text{ (From previous part) }$
- $m = \frac{k(k-1)}{2} = \frac{5(5-1)}{2} = 10$
- $\alpha_1 = \frac{\alpha_F}{m} = \frac{0.05}{10} = 0.0005$
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
	- $p = 2P(t_{25} > 2.9716) \in (0.005,0.01) \implies$ strong to moderate evidence against $H_0$
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
	- $p = 2P(t_{25} > -3.9367) \in (0.0005,0.001) \implies$ Strong evidence against $H_0$
	- $\alpha = 0.05$
	- $p < \alpha \implies$ Reject the null hypothesis

- (v)

	- At a signifigance level of $0.05$ we reject the null hypothesis that there is a signifigant difference in the sales of store E in comparison with stores A and B (combined)


{{ENDQUESTION}}

# Question 2

Filled in ANOVA tables for later use

$n = 36 \text{ (Number of Observations) }$ 

Table 1

 $k = 6 \text{ (Number of groups) }$

| Sales          |        |            | ANOVA Table |     |      |
| -------------- | ------ | ---------- | ----------- | --- | ---- |
|                | Ss     | df         | Ms          | F   | Sig. |
| Between        | 7.692  | $k-1=5$    |             |     |      |
| Within (error) | 6.393  | $n-k = 30$ |             |     |      |
| Total          | 14.086 | $n-1 = 35$ |             |     |      |

Table 2

 $k = 2 \text{ (Number of groups) }$

| Sales          |        |            | ANOVA Table |     |      |
| -------------- | ------ | ---------- | ----------- | --- | ---- |
|                | Ss     | df         | Ms          | F   | Sig. |
| Between        | 0.934  | $k-1=1$    |             |     |      |
| Within (error) | 13.151 | $n-k = 34$ |             |     |      |
| Total          | 14.086 | $n-1 = 35$ |             |     |      |

Table 3

$k = 3 \text{ (Number of groups) }$

| Sales          |        |            | ANOVA Table |     |      |
| -------------- | ------ | ---------- | ----------- | --- | ---- |
|                | Ss     | df         | Ms          | F   | Sig. |
| Between        | 6.749  | $k-1=2$    |             |     |      |
| Within (error) | 7.337  | $n-k = 33$ |             |     |      |
| Total          | 14.086 | $n-1 = 35$ |             |     |      |


(a)

- (i)

	- A two way ANOVA test would be most appropriate here with paramaters defined in the question

- (ii)

	- $H_0 : \mu_{A-Sa} =  \mu_{A-Su}, \; \mu_{B-Sa} =  \mu_{B-Su}, \; \mu_{C-Sa} =  \mu_{C-Su}$
	- $H_A : \text{ There are some differences in the means}$
	- (reduced 3 vs. full 6)

- (iii)

	- EF (Error Full) = row 2 table 1
	- ER (Error Reduced) = row 2 table 3
	- $df_{EF} = 30$
	- $df_{ER} = 33$
	- $F = \frac{(SS_{ER} - SS_{EF}) \div (df_{ER} - df_{EF})}{(SS_{EF}) \div (df_{EF})} =  \frac{(7.337 - 6.393) \div (33 - 30)}{(6.393) \div (30)} = 1.4766$

- (iv)

	- $\alpha = 0.05$
	- $df_{extra} = 33- 30 = 3$
	- $p = P(F^{3}_{30} > 1.4766) \in (0.25, 0.1) \implies$ Weak evidence against the null hypothesis
	- $p > \alpha \implies$ Fail to reject the null hypothesis

- (v)

	- At a signifigance level of $0.05$ we fail to reject the null hypothesis that there is a signifigant difference in the sales of stores on saturdays and sundays after accounting for the different stores

(b)

- The specified t-test would be equivalent to table 2 meaning that 
- $df = 34$
- $t = \sqrt{F} = 1.5543$
- $p = 0.129373$


{{ENDQUESTION}}

# Question 3


number of Lab sections = 12
number of Graders = 5
$n = 25 \times 12 = 300 \text{ (Number of Observations) }$

(a)

- One way ANOVA
- $k = 12 \text{ (Number of groups) }$ 
- $H_0 : \mu_1 = \mu_2 = \dots = \mu_k$
- $H_A : \text{There is some difference in the means}$
- $df_{B} = k - 1 = 11$
- $df_{W} = 300 - 12 = 288$

(b)

- Two way ANOVA
- $H_0 : \mu_1 = \mu_2 = \mu_3 , \; \mu_4, \; \mu_5 = \mu_6 = \mu_7, \; \mu_8 = \mu_9 = \mu_{10}, \; \mu_{11} = \mu_{12}$
- $H_A : \text{ There are some differences between the sections graded by same grader}$
- $df_{LAB} = 12 - 1 = 11$
- $df_{GRADER} = 5 - 1 = 4$
- $df_E = 300 - 12 = 288$

(c)

- Two way ANOVA
- $H_0 : \mu_{Q1} = \mu{R1} = \mu{S1}$
- $H_A : \text{ There are some differences in the means}$
- $df_{LEC} = 12 - 5 = 2$
- $df_{LAB} = 12 - 3 = 9$
- $df_{E} = 300 - 12 = 288$ 

{{ENDQUESTION}}
# Question 4

The Kruskal-Wallis test would be the most appropriate here as
1. The provided data is not normal and the logged transformed data is also not normal given the p values in the Shapiro-Wilk tests are above the lower bound for true signifigance in all cases except Nicaragua
2. $n<30\implies$ CRT does not apply 

- Because of the last 2 we cannot use a normal ANOVA test so the following are the assumptions for the Kruskal-Wallis test

3. Roughly same shape of the distributions as seen the in histograms given in the question
4. Assumption that all of the groups have size $\geq 5$ satisfied

$H_0 : \text{ The distribution is the same across the 3 countries}$
$H_A : \text{ The distribution is not the same across the 3 countries}$

| Cuba      | Cuba Rank  | Nicaragua | Nicaragua Rank | Costa Rica | Costa Rica Rank |
| --------- | ---------- | --------- | -------------- | ---------- | --------------- |
| 0.5       | 1          | 1         | 3              | 1          | 3               |
| 1.3       | 5          | 1         | 3              | 2          | 7.5             |
| 3.6       | 10         | 1.5       | 6              | 4.7        | 11              |
| 5.5       | 12         | 2         | 7.5            | 8.7        | 13              |
| 9.7       | 14         | 2.3       | 9              | 14.2       | 16              |
| 11.4      | 15         | 25.6      | 19             |            |                 |
| 15.3      | 17         |           |                |            |                 |
| 23.8      | 18         |           |                |            |                 |
| $n_1 = 8$ | $R_1 = 92$ | $n_2 = 6$ | $R_2 = 47.5$   | $n_3 = 5$  | $R_3 = 50.5$    |

$H = \frac{12}{n(n+1)}(\frac{R_1^2}{n_1} + \frac{R_2^2}{n_2} + \frac{R_3^2}{n_3})-3(n+1)$
$\Rightarrow \frac{12}{19(20)}(\frac{92^2}{8} + \frac{47.5^2}{6} + \frac{50.5^2}{5})-3(20) = 1.3924$
$\alpha = 0.1$
$p = P(\chi^2_{2} > 1.3924) > 0.2  \implies$ weak evidence against the null hypothesis
$p > a \implies$ Fail to reject the null hypothesis

At a signifigance level of $0.1$ we fail to reject the null hypothesis that there is a signifigant difference in the distribution of swimming speed of turtles between the three countries