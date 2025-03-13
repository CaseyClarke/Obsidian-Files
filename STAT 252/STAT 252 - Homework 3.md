# Question 1


Filled in ANOVA table

|       | Ss         | df         | Ms                      | F                                        | sig.     |
| ----- | ---------- | ---------- | ----------------------- | ---------------------------------------- | -------- |
| REGER | $2391.564$ | $1$        | $2391.564$              | $\frac{2391.564}{73.5267} = 32.5265$<br> | 0.000055 |
| ERROR | $1029.374$ | $n-2 = 14$ | $1029.374/14 = 73.5267$ |                                          |          |
| Total | $3420.938$ | $n-1 = 15$ |                         |                                          |          |
$SS_{ERROR} = 3420.938 - 2391.564$

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

- $\delta  = \mu(mass|age + 3) - \mu(mass|age) = \beta_0 + \beta_1(age + 3) - (\beta_0 + \beta_1age) = 3\beta_1$

- Given that $SE(ax) = |a|SE(x) \quad a \in R$
- $SE(\delta) = SE(3\hat{\beta_1}) = 3SE(\hat{\beta_1}) = 3(0.177568347639) = 0.532705042917$ (From (f))

- $\alpha = 0.05$
- $(1-\alpha)\times 100\% \ CI:$
- $\delta \pm t_{14, 0.025}SE(\delta) = 3\hat{\beta_1} \pm t_{14, 0.025}SE(3\hat{\beta_1})$
- $\Rightarrow 3(-1.013) \pm 2.145 (0.532705042917)0.532705042917$
- $(-3.6476966516, -2.4303033484)$
- 

(j)

- $\hat{y} = \hat{\beta_0} + \hat{\beta_1}(60) = 155.143 - 1.013(60) = 94.363$
- $S_{XX} = (n-1)S^2_{age} = (15)(12.46846)^2 = 2331.93742157$
- $\hat{\sigma} = \sqrt{MSE} = \sqrt{73.5267} = 8.5748$
- $SE(\hat{y}) = \hat{\sigma}\sqrt{\frac 1n + \frac{(60 - \mu_{age})^2}{S_{XX}}} = 8.5748\sqrt{\frac {1}{16} + \frac{(60 - 60.4375)^2}{2331.93742157}} = 2.14510718339$
- $\alpha = 0.05$
- $(1-\alpha)\times 100\% \ CI:$
- $\hat{y} \pm t_{14, 0.025}SE(\hat{y})$
- $94.363 \pm 2.145(2.14510718339)$
- $(89.7617450916, 98.9642549084)$

(k)

- $\hat{y} = \hat{\beta_0} + \hat{\beta_1}(60) = 155.143 - 1.013(60) = 94.363$
- $S_{XX} = (n-1)S^2_{age} = (15)(12.46846)^2 = 2331.93742157$
- $\hat{\sigma} = \sqrt{MSE} = \sqrt{73.5267} = 8.5748$
- $SE(\hat{y}) = \hat{\sigma}\sqrt{1 + \frac 1n + \frac{(60 - \mu_{age})^2}{S_{XX}}} = 8.5748\sqrt{1 + \frac {1}{16} + \frac{(60 - 60.4375)^2}{2331.93742157}} = 8.83904292716$
- $\alpha = 0.05$
- $(1-\alpha)\times 100\% \ CI:$
- $\hat{y} \pm t_{14, 0.025}SE(\hat{y})$
- $94.363 \pm 2.145(8.83904292716)$
- $(75.4032529212, 113.322747079)$

(l)

- The first one is narrower as it is only accounting for uncertainty in the estimation while the second one accounts for that as well as variability within samples of the same age, mathematically this is just a difference of $+1$ in the root of the standard error

{{ENDQUESTION}}
# Question 2

(a)

- $\beta_0 + \beta_1(weight + 1) - (\beta_0 + \beta_1(weight)) = \beta_1(weight + 1) -\beta_1(weight) = \beta_1$

(b)

- $(e^{0.006}, e^{0.016}) = (1.00601803605, 1.01612868541)$

- This means that we are $95\%$ confident that a $1 \ kg$ increase in birthweight corresponds to a between $1.00601803605$ and $1.01612868541$ times increase in gestation time

(c)

- $(e^{4.59}, e^{5.9}) = (98.4944301619, 365.037467865)$

- This means that we are $95\%$ confident that given a $1.2 \ kg$ lion the gestation period will be between $98.4944301619$ and $365.037467865$ unknown units (days?)

{{ENDQUESTION}}
# Question 3

ANOVA:

- Normality: The response variables must be normally distributed 
- Equal S.D.'s: Must have Homogeneity of variances

SLR: 

- Normality: The residuals must be normally distributed 
- Equal S.D.'s: Must have Homoscedasticity
