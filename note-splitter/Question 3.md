# Question 3

(a)

- $H_0: \mu_{C} = \mu_{H} = \mu_{Q} = \mu_{T} = \mu_{HT} = \mu_{QT}$
- $H_A : \text{There are some differences in the means}$

(b)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcYWrmmJ1lHirZ-0j0tC_f5QEtecpApucfJkI1DFH6CZfgzSWRlZY6e54mdu8pYuKqVruGTOPj4_Feaa0Cbd5Ur4JvQihPe5Wn2MPcgF9hO7ejLTlUy4tmrg06_iKZlaQ70CiK?key=IQAsPUclo3cAIZczkFx_qYMk)

- The sum-of-squares residual from fitting the Reduced model is the Total row of the above ANOVA table, it is $19672.550$
- 
- The sum-of-squares residual from fitting the Full model is the Within row of the above ANOVA table, it is $11240.700$
- 
- The pooled estimate of the common population variance is the mean square of fitting the full model which is the Within row of the above ANOVA table, it is $64.602$
- 
- The test statistic is given by the following formula where the subscript denotes (F)ull or (R)educed
- $$F_0 = \frac{(SSR_R - SSR_F)/(df_R - df_F)}{SSR_F / df_F} = \frac{(19672.550 - 11240.700)/(179 - 174)}{11240.700 / 174} \approx 26.1041$$
- This is consistent with the F test statistic as provided by SPSS in the above ANOVA table

- The p value can be calcuated with the following formula
- $p = P(F^{df_R-df_F}_{df_F} > F_0) = P(F^5_{174} > F_0) < 0.01$

- Given that our p value is lower than the signifigance level of $0.01$ we reject the null hypothesis that there is no difference in the teaching strategies