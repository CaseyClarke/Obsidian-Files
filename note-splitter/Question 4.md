# Question 4

(a)
- $ln(\mu_{L} - \mu_{S}) = 1.8370 - 1.5910 = 0.246$
- $e^{0.246} \approx 1.2789$

- From log rules we know that 
- $$e^{ln(\mu_{L} - \mu_{S})} = e^{ln(\frac{\mu_{L}}{\mu_{S}})} = \frac{\mu_{L}}{\mu_{S}}$$
- Therefore the antilogarithm of the difference is the ratio of the brain sizes, e.g. on average the LARGE group has $1.2789\times$ the brain size compared to those of the SMALL group


(b)

- 
  > ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIt8NyPLpHrva4bB5xP-ESYneFlu-BDMeolaeGA8d3DHZzA6gCcLI0_m1h-W4VwWaM_bbTGwZDxhPZ8pwDEP7tWz0XHZdh8h457Lvl5aG5vQXJAYn8nkjUkzG6GHNaupg8JGuroA?key=_VwyLlKMddU95SYPlK_KuEQP)
  > [Full Size Image](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIt8NyPLpHrva4bB5xP-ESYneFlu-BDMeolaeGA8d3DHZzA6gCcLI0_m1h-W4VwWaM_bbTGwZDxhPZ8pwDEP7tWz0XHZdh8h457Lvl5aG5vQXJAYn8nkjUkzG6GHNaupg8JGuroA?key=_VwyLlKMddU95SYPlK_KuEQP)

- $H_0 : ln(\mu_L  - \mu_S) = 0$
- $H_A : ln(\mu_L - \mu_S) \neq 0$
- $t = -1.247$
- $p = 0.216$
- The distribution under the null hypothesis is normal. 
- Given that the p-value is bigger than our significance level of $0.01$ we fail to reject the null hypothesis

(c)

- $CI_{99} = (e^{-0.76525}, e^{0.27334}) \approx (0.46522, 1.31435)$

- From part (a) we know that a difference log transformed can be thought of as a ratio which means to form a conclusion from the confidence interval we need to check if it contains $1$ as that would mean that both means are equal, since it does in fact contain $1$ we can conclude that with $95\%$ confidence there is no difference between the means. This is the same conclusion we came to in part (a)