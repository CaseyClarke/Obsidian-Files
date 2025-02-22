# Question 1

 (a)

- (i)

	- A one-way ANOVA test with 5 means is the most appropriate with the paramaters being $\mu_{A}, \mu_{B}, \mu_{C}, \mu_{D}, \mu_{E}$

- (ii)

	- $H_0: \mu_{A} = \mu_{B} = \mu_{C} = \mu_{D}  = \mu_{E}$
	- $H_A : \text{There are some differences in the means}$

- (iii)


- $n = 30 \text{ (Number of Observations) } \quad a = 5 \text{ (Number of groups) }$ 

| Sales   |       |            | ANOVA Table          |                                    |                       |
| ------- | ----- | ---------- | -------------------- | ---------------------------------- | --------------------- |
|         | Ss    | df         | Ms                   | F                                  | Sig.                  |
| Between | 4.083 | $a-1=4$    | $4.083/4 = 1.02075$  | $\frac{1.02075}{0.22472} = 4.5423$ | $p \in (0.025, 0.01)$ |
| Within  | 5.618 | $n-a = 25$ | $5.618/25 = 0.22472$ |                                    |                       |
| Total   | 9.702 | $n-1 = 29$ |                      |                                    |                       |

- (iv)

	- $\alpha = 0.05$
	- $p = P(F^{4}_{25} > 4.5423) \in (0.025, 0.01) < \alpha \implies$Reject the null hypothesis


- (v)

	- At a significance level of $0.05$ we reject the claim that the there is no difference in the mean sales between the different stores


(b)

- $S_p = \sqrt{MSE} = \sqrt{0.22472} = 0.47405$

(c)

| A      | B      | C      | D      | E      |
| ------ | ------ | ------ | ------ | ------ |
| 1.883  | 1.783  | 1.183  | 1.333  | 0.900  |
| ------ | ------ | ------ | ------ |        |
|        | ------ | ------ | ------ |        |
|        |        | ------ | ------ | ------ |
|        |        |        | ------ | ------ |
