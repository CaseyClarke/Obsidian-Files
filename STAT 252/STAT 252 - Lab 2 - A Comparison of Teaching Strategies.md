# Question 1

(a)

- The population of interest is high school math students, the subjects are grade 12 math students from a large high school. The factor is teaching strategies, the levels are as follows:
	- Group 1: C (control group, only lecture notes and discussion)
	- Group 2: H (control plus weekly homework assignments)
	- Group 3: Q (control plus weekly quizzes)
	- Group 4: T (control plus computer tutorials)
	- Group 5: HT (control plus weekly homework as well as computer tutorials)
	- Group 6: QT (control plus weekly quizzes well as computer tutorials)

(b)

- Since this is an experiment but without random sampling and allocation we cannot make causal inferences and population inferences are not possible as the sample was only from one grade of math students not all of the grades in high school

{{ENDQUESTION}}

# Question 2

(a)

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc5tUyFWprZlM_uta2ro_HlhI4WyzDwgwtEa7HSONt2tlm72v9sb34oT8uLWrEIXLPkJIErME9YBrxJTBEJp_oNdEkDYJg1_vI0qPii1Y_n__8NaTaewhihQfEEyNBMBs3WVt0x2Q?key=IQAsPUclo3cAIZczkFx_qYMk)

- HT seems to be the best strategy and C seems to be the worst just based off of comparing the means.

- The standard deviations stay roughly in the range of $(7, 9.5)$ and the ratio of the largest vs. the smallest standard deviations is about $1.3626$ meaning that we can safely assume equal variablity is satisified

(b)


> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXctoM_DH9Ru9mwGMDDRv9WEzRjtIJ8ECcoUAbTDp3YRFWsJbC-WrPvYa-2Kh7fVv-2eu_VagiuPDqZqUs_rtKCzB9GKOC7r9LkDlRLW0pc-P21VAypnXL9RvXV3Yz62HRsmVU9VnA?key=IQAsPUclo3cAIZczkFx_qYMk)


C: Skewed - slightly left
H: Symmetric but with an outlier
HT: Roughly Symmetric
Q: Roughly Symmetric
QT: Roughly Symmetric
T Skewed - slightly right

The centers are vastly different

There is a lot of variance in the spreads and centers of the boxplots and there is an outlier in the H group. Given that the groups are only slightly skewed at max and there is only one outlier we can assume that normaility is preserved


(c)

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc4Vb2gcnSpiAK-eliyoaKahHDpfRWAShK0eiL0HwDeoXrJYFt02i3FEi9c7ch4WdgkL5vnDE8OyRNb7kFBOVFs1ttgJvBgdlAKoeDwRBUs9pmwAm_5nqmFpIk18BwvSFjxkWpKqA?key=IQAsPUclo3cAIZczkFx_qYMk)

All of the plots seem roughly normal, the dots stay close to the trend line and it is roughly $45°$

If the assumption of normality was violated it would pose a signifigant problem as it it a requirement for the following statistical tests and would affect the results greatly

{{ENDQUESTION}}

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


{{ENDQUESTION}}


# Question 4

(a)

- (i)

	- $\gamma_H = \frac{(\mu_2 - \mu_1) + (\mu_5 - \mu_4)}{2} = -\frac12 \mu_1 + \frac 12 \mu_2 + 0\mu_3 -\frac12 \mu_4 + \frac12 \mu_5 + 0 \mu_6$

- (ii)

	- $\gamma_Q = \frac{(\mu_3 - \mu_1) + (\mu_6 - \mu_4)}{2} = -\frac12 \mu_1 + 0\mu_2 + \frac12 \mu_3 -\frac12 \mu_4 + 0 \mu_5 + \frac12 \mu_6$
- 
- (iii)

	- $\gamma_T = \frac{(\mu_4 - \mu_1) + (\mu_5 - \mu_2) + (\mu_6 - \mu_3)}{3}$
	- $\Rightarrow -\frac13 \mu_1 + -\frac13 \mu_2  -\frac13 \mu_3 + \frac13  \mu_4 + \frac13 \mu_5 + \frac13 \mu_6$

(b)

> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXekWxrQySaO9tl-pGnqX497qMlvYX-ZwSK4Z4s-KAeO48fJoM8bMJIvRPKPKlUHNXXDh5tHOsX2C_hzjwL-bvG1QZWWFV1qczXGij5mnjeQq_5knFzXQ7LJuL9PE8hIjyJPCReQpg?key=qNqmTtS7lvHFneQk3oyTP06V)


> ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfWkJdHlZFL1Ifef2wG4BZRlv6f0vQLHnhbdGSms-539fux-_IDMLh4oSLctZBhuZL2nj4Jr3rS1IH7CveR5BrBqnnxh4sGP7VtY8XXKVPb55DvS1_vrHSpG41UMf_DnJNQ_BsZGg?key=qNqmTtS7lvHFneQk3oyTP06V)

- For homework assignments:
	- The midterm scores were on average affected by the value of contrast which is $13.18$ grade points
	- The standard error is $1.467$
	- The test statistic is high at $t = 8.984$
	- The p value is very low at $p < 0.001$
	- All of this points to the fact that homework assignments have a high effect on the midterm scores
- For weekly quizzes:
	- The midterm scores were on average affected by the value of contrast which is $1.07$ grade points
	- The standard error is $1.467$
	- The test statistic is low at $t = 0.727$
	- The p value is high at $p = 0.468$
	- All of this points to the fact that weekly quizzes have a very low effect on midterm scores
- For computer tutorials:
	- The coefficients for this contrast were multiplied by 3 when inputted into SPSS so the Value of contrast and St. Error are divided by 3 when reported here
	- The midterm scores were on average affected by the value of contrast which is $6.543$ grade points
	- The standard error is $1.198$
	- The test statistic fairly high at $t = 5.462$
	- The p value is very low at $p < 0.001$
	- All of this points to the fact that computer tutorials have a medium effect on the midterm scores

- Homework assignments are the most influential and weekly quizzes are the least influential, most evident by comparing the Value of Contrast for the 3 types

(c)

- $95\% \text{ CI}_H = \text{ Value of Contrast} \pm SE(\gamma_H)t^*_{df} = 13.18 \pm 1.467(1.660) = (10.745, 15.615)$ 
- ==INTERPRETATION==

(d)

- $\gamma_{H-Q} = \gamma_H - \gamma_Q = 0 \mu_1 + \frac 12 \mu_2 -\frac12\mu_3 -0 \mu_4 + \frac12 \mu_5  - \frac12 \mu_6$
-  $90\% \text{ CI}_{H-Q} = \text{ Value of Contrast} \pm SE(\gamma_{H-Q})t^*_{df} = 12.12 \pm 1.467(1.290) = (10.228, 14.012)$ 
- ==INTERPRETATON==

{{ENDQUESTION}}

# Question 5

>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcDKuqHPEhong0HB2HTvvfY_qil9LxuePqq3YW-QSfsXoWPQWKzRADa-Y6PaHVSuCLmf1lfmqeFqHd-51CeznMynKl0w-JpHLKN3yj94k3Meh-wZFJFuZpA6cMdlvA2j2EFowov8Q?key=qNqmTtS7lvHFneQk3oyTP06V)


| C     | Q     | T     | QT    | H     | HT    |
| ----- | ----- | ----- | ----- | ----- | ----- |
| ----- | ----- |       |       |       |       |
|       |       | ----- | ----- |       |       |
|       |       |       | ----- | ----- |       |
|       |       |       |       | ----- | ----- |

==COMMENTS==

{{ENDQUESTION}}

# Question 6

4 Mean Model (Reduced)
>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf9aIGbUF_PfiTGletDguKI9Ro9cWK99femWKgvEB9TubGFF2_ImjIa4D_fRfFtPQhhZrOPRHn95du316Un3_Lg34hWkd-4yCRWUn2tC64IoPkDx0f9xq8wJ7KHDHbijMCXP_fe?key=qNqmTtS7lvHFneQk3oyTP06V)

Sum-of-squares residuals = 11297.367
$df_{ER} = 176$

6 Mean Model (Full)
>![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcYWrmmJ1lHirZ-0j0tC_f5QEtecpApucfJkI1DFH6CZfgzSWRlZY6e54mdu8pYuKqVruGTOPj4_Feaa0Cbd5Ur4JvQihPe5Wn2MPcgF9hO7ejLTlUy4tmrg06_iKZlaQ70CiK?key=IQAsPUclo3cAIZczkFx_qYMk)

Sum-of-squares residuals = 11240.700
$df_{EF} = 174$


$F = \frac{(SS_{ER} - SS_{EF}) \div (df_{ER} - df_{EF})}{(SS_{EF}) \div (df_{EF})} =  \frac{(11297.367 - 11240.700) \div (176 - 174)}{(11240.700) \div (174)} = 1.4766$



