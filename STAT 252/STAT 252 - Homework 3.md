# Question 1


Filled in ANOVA table

|       | Ss                               | df         | Ms                      | F                                        |          |
| ----- | -------------------------------- | ---------- | ----------------------- | ---------------------------------------- | -------- |
| REGER | $2391.564$                       | $1$        | $2391.564$              | $\frac{2391.564}{73.5267} = 32.5265$<br> | 0.000055 |
| ERROR | $3420.938 - 2391.564 = 1029.374$ | $n-2 = 14$ | $1029.374/14 = 73.5267$ |                                          |          |
| Total | $3420.938$                       | $n-1 = 15$ |                         |                                          |          |


(a)

- $\hat{y} = \hat{\mu}(mass|age) = \hat{\beta_0} + \hat{\beta_1}age = 155.143 -1.013age$

(b)

- $\frac{SS_{REGER}}{SS_{T}}\times (100\%) = \frac{2391.564}{3420.938}\times(100\%) \approx 69.91\%$ 

(c)

- $\hat{\sigma} = \sqrt{MSE} = \sqrt{73.5267} = 8.5748$

(d)

- The ANOVA Test for Significance of the Model and the Slope of a Population Regression line would be most appropriate
- Assumptions are satisfied 
- 
- $H_0 : \beta_1 = 0$
- $H_a : \beta_1 \neq 0$
- Some relationship vs. no realationship

- $F^* = 32.5265$ (From filled in table above)

- $p = P(F^1_{14} > F^*) < 0.001$ (Very strong evidence against $H_0$)
- $p_{comp} = 0.000055$

- Given that $\alpha = 0.01$, $p < \alpha$ 
- We reject the null hypothesis that there is no relation between the two variables and thus we conclude that there is infact a linear relationship between the two variables

(e)

- $r = \sqrt{\frac{SS_{REGER}}{SS_T}} = \sqrt{\frac{2391.564}{3420.938}} = -0.836119596074$
- $df = n-2 = 14$

(f)

- The Regression t-Test for Significance of the Slope of a Population Regression line would be most appropriate 
- Assumptions are satisifed

- $H_0 = \beta_1 = 0$
- $H_A = \beta_1 < 0$

- $\hat{\sigma} = 8.5748$ (From (c))

- $S_{XX} = (n-1)S^2_{age} = (15)(12.46846)^2 = 2331.93742157$
- $SE(\hat{\beta_1}) = \frac{\hat{\sigma}}{\sqrt{S_{XX}}} = \frac{8.5748}{\sqrt{2331.93742157}} = 0.177568347639$

- $t = \frac{\hat{\beta_1}}{SE(\hat{\beta_1})} = \frac{-1.013}{0.177568347639} = -5.70484556211$
- 
- $p = P(T_{14} < t) < 0.0005$

- $t_{comp} = \frac{\hat{\beta_1}}{SE{\hat{\beta_1}}} = \frac{-1.013}{0.178} = -5.69101123596$
- $p_{comp} = P(T_{14} < t) < 0.0005$

- My t value and the computers t value are very similar (>0.01 difference) so it would make sense that the p value ranges are very similar

- Given that $\alpha = 0.01$, $p < \alpha$ 

- We reject the null hypothesis that there is no relation between the variables in favor of the alternative hypothesis that age and muscle mass are negatively correlated

(g)

- $t^2 = F$

(h)

| Model | $R$               | $R^2$            | $R^2_{ADJ}$ | $SE({\hat{\beta}})$ |
| ----- | ----------------- | ---------------- | ----------- | ------------------- |
| 1     | $-0.836119596074$ | $0.699095978939$ |             | $0.178$             |

(i)

- 

# Question 2


