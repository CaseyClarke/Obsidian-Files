
# Question 1 

Filled in ANOVA table

|       | Ss          | df             | Ms                                 | F                                                     | sig. |
| ----- | ----------- | -------------- | ---------------------------------- | ----------------------------------------------------- | ---- |
| REGER | $28715.964$ | $k = 3$        | $28715.964 / 3 =$<br>$9571.988$    | $\frac{9571.988}{77.3783846154} =$<br>$123.703642142$ |      |
| ERROR | $1005.919$  | $n-k - 1 = 13$ | $1005.919/13 =$<br>$77.3783846154$ |                                                       |      |
| Total | $29721.882$ | $n-1  = 16$    |                                    |                                                       |      |

(a)

- A Multiple Regression ANOVA Test (F-Test) would be most appropriate

- $H_0: \text{The model is useful for making predictions}$
- $H_A: \text{The model is not useful for making predictions}$

- $F^* = 123.703642142$ (from above table)

- $p = P(F^3_{13} > F^*) \in (0.005, 0.001) \implies$ strong evidence against $H_0$
- $p < \alpha = 0.05 \implies$ reject $H_0$

- $\therefore$ We conclude that yes this is a useful model with very high certainty

(b)

- $R^2 = (0.983)^2 = 0.966289$
- $\implies$ about $96.63\%$ of the variation is explained by the model

(c)

- $R^2_{adj} = 1- \frac{(1-R^2)(n-1)}{n-k-1} = 1- \frac{(1-0.966289)(16)}{13} = 0.958509538462$
- $\implies$ about $95.85\%$ of the variation is explained by the model (adjusted)

(d)

