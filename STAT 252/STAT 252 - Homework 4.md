# Question 1 

Filled in ANOVA table

|       | Ss          | df             | Ms                                 | F                                                     | sig. |
| ----- | ----------- | -------------- | ---------------------------------- | ----------------------------------------------------- | ---- |
| REGER | $28715.964$ | $k = 3$        | $28715.964 / 3 =$<br>$9571.988$    | $\frac{9571.988}{77.3783846154} =$<br>$123.703642142$ |      |
| ERROR | $1005.919$  | $n-k - 1 = 13$ | $1005.919/13 =$<br>$77.3783846154$ |                                                       |      |
| Total | $29721.882$ | $n-1  = 16$    |                                    |                                                       |      |

(a)

- A Multiple Regression ANOVA Test (F-Test) would be most appropriate

- $H_0: \text{The model is not useful for making predictions}$
- $H_A: \text{The model is useful for making predictions}$

- $F^* = 123.703642142$ (from above table)

- $p = P(F^3_{13} > F^*) < 0.001 \implies$ strong evidence against $H_0$
- $p < \alpha = 0.05 \implies$ reject $H_0$

- $\therefore$ We conclude that at $\alpha = 0.05$ this is a useful model

(b)

- $R^2 = (0.983)^2 = 0.966289$
- $\implies$ about $96.63\%$ of the variation is explained by the model

(c)

- $R^2_{adj} = 1- \frac{(1-R^2)(n-1)}{n-k-1} = 1- \frac{(1-0.966289)(16)}{13} = 0.958509538462$
- $\implies$ about $95.85\%$ of the variation is explained by the model (adjusted)

(d)

- $SE = \sqrt{\frac{SS_R}{df_R}} = \sqrt{\frac{1005.919}{13}} = 8.79649842923$

(e)

- A Multiple Regression t-test for the Usefulness of Particular Predictor Variables would be most appropriate

- $H_0: \beta_1 = 0$
- $H_A: \beta_1 < 0$

- $\hat{\beta_1} = -1.441$
- $SE(\hat{\beta_1}) = 0.676$
- $t^* = \frac{\hat{\beta_1}}{SE(\hat{\beta_1})} = \frac{-1.441}{0.676} = -2.13165680473$
- $df = n-(k+1) = 17 - 4 = 13$

- $p = P(t_{13} > t^*) \in (0.025, 0.05) \implies$ Moderate evidence against $H_0$
- $p_{computer} = 0.053/2 = 0.0265$
- $p < \alpha = 0.05 \implies$ reject $H_0$

- $\therefore$ We conclude that at $\alpha = 0.05$ there is a negative relationship between years driving and monthly premiums

(f)

- $\hat{\beta_3} = -0.772$
- $SE(\hat{\beta_3}) = 0.244$
- $df = 13$ (from previous part)
- $t_{0.025} = 2.160$
- $\hat{\beta_3} \pm t_{0.025}SE(\hat{\beta_3)} = -0.772 \pm 2.160(0.244) = (-1.29904, -0.24496)$

- Since the confidence interval does not contain 0 we can say with $95\%$ confidence that the interaction term (interaction between driving experiece and number of violations) has a signifigant effect on montly premiums

(g)

- Observed $= \hat{\gamma} = 96.740 + (-1.441 \times 10 ) + (22.313 \times 3) + (-0.772 \times 30) = 126.109$

- Residual $= 100 - \hat{\gamma} = 100 - 126.109 = -26.109$  

(h)


- $\hat{\gamma} = 96.740 + (-1.441 \times 10 ) + (22.313 \times 3) + (-0.772 \times 30) = 126.109$
- $t_{0.025} = 2.160$
- $MSE = 77.3783846154$ (from above table)
- $\hat{\gamma}\pm t_{0.025}\sqrt{MSE + SE(fit)^2}$
-  $=126.109 \pm 2.160\sqrt{77.3783846154 + (3.249)^2} = (105.853959404, 146.364040596)$

- $\therefore$ We are $95\%$ confident that for a driver that has been driving for 10 years and has gotten 3 tickets in the past 3 years, thier monthly premiums lie in the range 
- $(105.853959404, 146.364040596)$ dollars

(i)

- $\hat{\gamma} = 96.740 + (-1.441 \times 10 ) + (22.313 \times 3) + (-0.772 \times 30) = 126.109$
- $t_{0.025} = 2.160$
- $\hat{\gamma}\pm t_{0.025}SE(fit) = 126.109 \pm 2.160(3.249) = (119.09116, 133.12684)$

- $\therefore$ We are $95\%$ confident that for a driver that has been driving for 10 years and has gotten 3 tickets in the past 3 years, thier monthly premiums lie in the range $(119.09116, 133.12684)$ dollars

{{ENDQUESTION}}

# Question 2

(a)

General formula $= \beta_1 + \beta_6male + \beta_7D1 + \beta_8D2+ \beta_9D3 + \beta_{10}(male \times D1) + \beta_{11}(male \times D2) + \beta_{12}(male \times D3)$

| Gender | IBP | Effect                                     |
| ------ | --- | ------------------------------------------ |
| Male   | 0   | $\beta_1 + \beta_6$                        |
| Male   | 1   | $\beta_1 + \beta_6 + \beta_7 + \beta_{10}$ |
| Male   | 2   | $\beta_1 + \beta_6 + \beta_8 + \beta_{11}$ |
| Male   | 3   | $\beta_1 + \beta_6 + \beta_9 + \beta_{12}$ |
| Female | 0   | $\beta_1$                                  |
| Female | 1   | $\beta_1 + \beta_7$                        |
| Female | 2   | $\beta_1 + \beta_8$                        |
| Female | 3   | $\beta_1 + \beta_9$                        |

(b)

- To find the constraints just set each effect with the same dosage equal to each other
- $D(0)$:
	- $\beta_1 + \beta_6 = \beta_1$
	- $\beta_6 = 0$

- $D(1)$:
	- $\beta_1 + \beta_6 + \beta_7 + \beta_{10} = \beta_1 + \beta_7$

- $D(2)$:
	- $\beta_1 + \beta_6 + \beta_8 + \beta_{11} = \beta_1 + \beta_8$

- $D(3)$:
	- $\beta_1 + \beta_6 + \beta_9 + \beta_{12} = \beta_1 + \beta_9$

- The $\beta_6 = 0$ equation cascades down and sets all constraints to 0 so
- The constraints are $\beta_{6}, \beta_{10}, \beta_{11}, \beta_{12} = 0$

(c)

- Setting all female effects equal to each other we get $\beta_{7}, \beta_{8}, \beta_{9} = 0$

- $H_0: \beta_{7}, \beta_{8}, \beta_{9} = 0$
- $H_A: \text{At least one }\beta_{7}, \beta_{8}, \beta_{9} \neq 0$

- Under null it is an $F^{\#contraints}_{n-p-1} = F^3_{130-13-1} = F^3_{116}$

(d)

General formula $= \beta_2 + \beta_6(weight) + \beta_{10}(weight \times D1) + \beta_{11}(weight \times D2) + \beta_{12}(weight \times D3)$

| IBP | Effect                                           |
| --- | ------------------------------------------------ |
| 0   | $\beta_2 + \beta_6(weight)$                      |
| 1   | $\beta_2 + \beta_6(weight) + \beta_{10}(weight)$ |
| 2   | $\beta_2 + \beta_6(weight) + \beta_{11}(weight)$ |
| 3   | $\beta_2 + \beta_6(weight) + \beta_{12}(weight)$ |

(e)

$$\beta_0 + \beta_1 (weight) + \beta_3 D1 + \beta_4 D2 + \beta_5 D3 + \beta_7 (weight \times D1) + \beta_8 (weight \times D2) + \beta_9 (weight \times D3)$$

(f) 

- A Extra-Sum-of-Squares F-Test in MLR would be most appropriate here

- $H_0: \beta_4 = \beta_5 = 0$
- $H_A: \text{ At least one }\beta_4, \beta_5 \neq 0$

- Using model 3 as full and 2 as reduced

- $df = [df_{ER} - df_{EF} = 3, df_{EF} = 123]$

- $F = \frac{(SS_{ER} - SS_{EF}) / (df_{ER} - df_{EF})}{SS_{EF} / df_{EF}} = \frac{(94.441 - 1.121) / (126 - 123)}{1.121 / 123} = 3413.13113292$

- Given the insanely high F statistic
- $p < 0.000001 \implies$ strong evidence against $H_0$
- $p < \alpha = 0.01 \implies$ reject $H_0$

- $\therefore$ We conclude that at $\alpha = 0.01$ we reject the null hypoethesis and conclude that that dose has a significant effect on Pressure after controlling for weight, age, and gender.
