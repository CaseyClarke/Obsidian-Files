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