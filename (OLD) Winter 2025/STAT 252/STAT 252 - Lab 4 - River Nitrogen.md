# Question 1

The study is an observational study looking at statistics about rivers and not controlling any variables. From that we know that population inferences can be made but casual inferences cannot be made. We cannot say for certain that human activites are the cause of NO3 levels but we can show that there is a correlation between the two, another difficulty is that the real relationship may not be linear and there may be other confounding variables that are not explored in the study

{{ENDQUESTION}}

# Question 2

(a)

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcirXUXw6Vu-2z4b-6j4DxLa1rv-9zSc6mJqe5D3Y1iBgb_054nrO0nRO7Qh8u0bP6SQaLAxX0puKK3TFk6LZtRqd9fOXpxBaWQ3n90jVK_upkuoKdKnfVCQCziIgGplUy00LwX8g?key=Y0atQW0GXv1vnQpUimEG73Gv)
> 


It seems as if 
- DEP and NPREC 
  DENSITY and NO3
  NPREC and Density

show a linear strong linear relationship and 
  - NO3 and NPREC
  - PREC and Density
  
show a linear moderate linear relationship


(b)

- NO3 vs.
	- DISCHARG - Non-linear relationship
	- RUNOFF - Non-linear relationship
	- AREA - Non-linear relationship
	- Density - Solid linear relationship
	- DEP - Very Roughly linear relationship
	- NPREC - Roughly linear relationship
	- PREC - Non-linear relationship


- DENSITY would be the one I would choose If i had to choose only one predictor variable as it is the closest to a linear realationship
- A linear model would not be appropriate as over half of them do not show a linear relationship in the slightest

{{ENDQUESTION}}

# Question 3

(a)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfZi9ZF0w7qajgtzYYupopz8o73Yxcc03kCMKNLmQlKx5DtWAhlmQBjlc_KKMdIASpuFZRA8ddJhnWYLxU8Muxlt_TLorOAx30XGTEN-H03xN4nklM4P_XyetX2B5Obmva9U5bsmQ?key=Y0atQW0GXv1vnQpUimEG73Gv)


For the pairs of variables that were already linear the transform did not really change all that much but for the other variables they are a lot closer to linear or are at least closer to being randomly scattered around the middle of the graph and not the bottom left as a lot of graphs were in the previous question

(b)

 >![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeNyQQCY8xUNoSeFBvuomE3jamZAfHbLP0v9IcNLkbfzr_KSoRsfCMx5EualS8R2mU8waGBOFcdBHFkQ-kwuKHmJVsyxxcXmRYxifvWntbhSas36e7NoTex_YsPVV4E4DAIVabq5w?key=Y0atQW0GXv1vnQpUimEG73Gv)


Several variables show strong correlations indicating potential collinearity, this implies that some predictor variables may be redundant in regression models

{{ENDQUESTION}}

# Question 4

$LNNO_3 = \beta_0 + \beta_1LNDISCHARG + \beta_2LNRUNOFF + \beta_3LNAREA +$ $\beta_4LNDENSITY + \beta_5LNDEP + \beta_6LNNPREC + \beta_7LNPREC + \epsilon$
$\mu(LNNO_3) = \beta_0 + \beta_1LNDISCHARG + \beta_2LNRUNOFF + \beta_3LNAREA +$
$\beta_4LNDENSITY + \beta_5LNDEP + \beta_6LNNPREC + \beta_7LNPREC$

Model assumptions are as follows
- $\sim N(0, c) \quad \text{For some } c \in \mathbb{R^+}$
- Independence of the error term $\epsilon$

{{ENDQUESTION}}

# Question 5

(a)

- At the end there were 5 variables removed in the following order (first removed to last removed):
	- LNdep
	- LNrunoff
	- LNprec	
	- LNarea	
	- LNdischarg

(b)

- The final equation at the end of the backwards elemination was $LNO_3 = 0.973 + 0.508LNDENSITY + 0.274LNNPREC$
- Percentage of variation explained by the explanitory variables is $R^2 \times 100 \% = 0.806(100 \%) = 80.6\%$

(c)

- SPSS reports the p value (from the last column of the ANOVA table) to be 0 to 13 decimal points of accuracy so we can be fairly certain that $p < \alpha = 0.05$

- The p value corresponding to the $\beta_0$ term is $0.01$ meaning it is signifigant at $\alpha = 0.05$ 
- The p value corresponding to the $\beta_1LNDENSITY$ term is 0 to 9 decimals meaning it is signifigant at $\alpha = 0.05$ 
- The p value corresponding to the $\beta_2LNNPREC$ term is $0.026$ decimals meaning it is signifigant at $\alpha = 0.05$ 

- It is clear that while all of them are signifigant the $LNDENSITY$ is clearly the term that is contributing the most signifigance and thus giving us that very low p value

{{ENDQUESTION}}

# Question 6 

(a)

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFtL30MeegmxKxFjYbZMIwV9HaTUOpWwOCsZuU3BEoJt0LjgxZI6OtttYUi7JS_Bnw6X9DJOCaMDfu7Irnl9nMaMpv8tTsE4cUwQXmWmAjKUnF-4nOpBkrmQp_78tk8cq_R7mZEw?key=Y0atQW0GXv1vnQpUimEG73Gv)


Variance does not seem to be constant as the spread of the points on the graph is vastly different for different standardized predicted values, for example when the standardized predicted value is 1 the spread is far tighter then when it is -1
This might imply that our assumption of equal varience has been violated
There also does not appear to be any egregious ouliers

(b)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZSFG8XE2LMm2n9MzyeOkPV4ngQD3bwcqteuLOzg-jgXmr24-DGwYXyhNcfe1iawVVBqHW0yxM8ZJkBf4jKLH4LpoeO6D4j9EWH_hoEsXINMQT9W1nMSp1glnLhUC9udbz_NzoZw?key=Y0atQW0GXv1vnQpUimEG73Gv)


The points do not deviate severly from the line so we can assume that normality holds

{{ENDQUESTION}}

# Question 7

(a)

- $R^2 = 0.130$
  It is so low because at the end of the forwards selection only one variable remained
- Meaning that only about $13\%$ of the variation in LNNO3 is explained by the variables in this model, this could suggest that this model might not be the best

(b)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcZOcI1bOdiBGPTxSG2vc9GK8V_lPcmIEoSuLowyHh68dOaAmookSWxrOB-Oy1f1qdOGYT21D79ukmyKue1UiCvYjwAmsfdya_0mthK02wc-SHKOxAu6bVdPm4K7-7X0sHJMfViOQ?key=6JOuZrwQDQoB9AFCBWEhKmOj)

The influential case is case 3 (Caragh, Ireland) with $COO = 0.861 \quad LEV = 0.153 \quad SRE = -2.833$ 
There is only one influential case as this is the only cases that is infuential in all 3 variables
It is marked on the graph with its case number

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeXeCHlSjXCF8Vofcmyyn8mr7qm7bygToVlFXr4TATb4d171EqpgQ8439RvJ9cwXirvjX2mXi8r6Mn5BMiQxl8rv-cUmW3XG5Itr-2Of4Mb8CkIJ9iNjA7py-3gHOvcol4DrSrKUA?key=Y0atQW0GXv1vnQpUimEG73Gv)

It's also pretty clear from looking at the graph that this case is influential

After removing case 3 $R^2 = 0.261$ This is a signifigant increase from before case 3 was removed 
$\mu(LNO_3) = 6.148490 - 0.362858LNDISCHARG$

(c)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcioGuLel122cSGC9iwG0clPfR99B71c6FIsvAhbwhdZkNSx0AOecBwiuKfG_Fiy77Wb0M3bt9W1cLK6u4zN8Yk6euYwC1oMihZGkqlR53XPl7D7ZZ8wrygMHZ_QaVuf0YZ0hog?key=6JOuZrwQDQoB9AFCBWEhKmOj)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdCcf7A4-7pgSS-IzMlypEgK-tgwaPXjIqe1iFDOkU2wrrzpm0CiK_RIfRCg0CkVY463denWV8e9VP6bHKTlLDXijyJUMzNiHaUbXMW4plEWs4-B7apEMbyNtviOAl_J39Wm5r9xA?key=6JOuZrwQDQoB9AFCBWEhKmOj)


$\mu(LNO_3) = \beta_1 + \beta_2LNDISCHARG$ (b)
$\mu(LNO_3) = \beta_1 + \beta_2LNDISCHARG + \beta_2LNDEP + \beta_3LNNPREC$ (c)

$H_0: \beta_2 = \beta_3 = 0$ (R = Reduced)
$H_A: \text{ At least one }\beta_2,\beta_3 \text{ differs from 0}$ (F = Full)

Using ESS F test, SS/df values found from ANOVA tables in (b) and (c)

$F^* = \frac{(SSR_R - SSR_F) / (df_r - df_f)}{SSR_F/df_F} = \frac{(51.587 - 33.054) / (39 - 37)}{33.054/37} = 10.372738549$

$p = P(F^2_{37} > F^*) < 0.001$

Given that the p value is very low (lower than standard level of signifigance $\alpha = 0.05$) we reject the null hypothesis in favor of the alternative, that is that the Full model is statistically signifigant

{{ENDQUESTION}}

# Question 8

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdV2vYXC_sCYTzr6VvRdm6wbAAi42MF9XS8A8NDWdS4M_qStnfnHz9DxRL3mos_Gz_pg5s1VTSZCwyPH-KN9zBIgwpXupQCPlZPzgs1fszSoEBCtu1aGicwgk2c4N7n7Re_4Dpnrw?key=6JOuZrwQDQoB9AFCBWEhKmOj)

$\mu(LNO_3) = \beta_1 + \beta_2LNDISCHARG + \beta_2LNDEP + \beta_3LNNPREC$ q7(c)
$\mu(LNO_3) = \beta_1 + \beta_2LNDISCHARG + \beta_2LNDEP + \beta_3LNNPREC + \beta_4LNDENSITY$ q8

Using ESS F test, SS/df values found from ANOVA tables in q7(c) and q8

$H_0: \beta_4 = 0$ (R = Reduced)
$H_A: \beta_4 \neq 0$ (F = Full)

$F^* = \frac{(SSR_R - SSR_F) / (df_r - df_f)}{SSR_F/df_F} = \frac{(33.054 - 11.873) / (37 - 35)}{11.873/35} = 31.2193632612$

$p = P(F^2_{35} > F^*) < 0.001$

Given that the p value is very low (lower than standard level of signifigance $\alpha = 0.05$) we reject the null hypothesis in favor of the alternative, that is that the Full model is statistically signifigant e.g. adding Density signifigantly improved the accuracy of the model

