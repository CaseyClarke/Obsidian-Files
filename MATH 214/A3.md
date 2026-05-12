# Question 1

(a) 
converges, written out solution by integral test given in A2 Q3 (b)

or just DCT with $\sum_{k = 1}^\infty\frac{1}{k^3}$
$k^2 + k^3 \geq k^3$ 
$(k \geq 1)$
$0 \leq \frac{1}{k^2 + k^3} \leq \frac{1}{k^3}$

$\sum_{k = 1}^\infty\frac{1}{k^3}$ converges by p-series as $p = 3 > 1$
the series is bounded above by a convergent series so it converges

(b)
root test
$|b_k| = \frac{1}{k^k}$
$L = \lim_{k \to \infty}\frac{1}{k}(\frac{1}{k^k})^{\frac1k}$
$L = \lim_{k \to \infty}\frac{1}{k}(k^{-k})^{\frac1k}$
$L = \lim_{k \to \infty}\frac{1}{k}k^{-1}$
$L = \lim_{k \to \infty}\frac{1}{k} = 0$

$L = 0 < 1$ $\implies \sum_{k = 1}^\infty\frac{1}{k^k}$ converges

(c)
test absolute convergence
$|sin(3k)| \leq 1$
$|\frac{sin(3k)}{1 + 2^k}| \leq \frac{1}{1 + 2^k}$
$|\frac{sin(3k)}{1 + 2^k}| \leq \frac{1}{1 + 2^k} \leq \frac{1}{2^k}$
DCT with $\sum_{k = 1}^\infty\frac{1}{2^k}$
$\frac{1}{2^k} = (\frac{1}{2})^k$
$\sum_{k = 1}^\infty(\frac{1}{2})^k$
this is a geo series with $r = 1/2 < 1$ so it converges
since $|\frac{sin(3k)}{1 + 2^k}| \leq \frac{1}{1 + 2^k} \leq \frac{1}{2^k}$
the absolute value of the series is bounded above by a convergent series so it absolutely converges

(d)
ratio test
$d_{k+1} = \frac{(k+1)^{k+1}}{3^{k+1}(k+1)!}$
$L = \lim_{k \to \infty}|\frac{d_{k+1}}{d_k}| = \lim_{k \to \infty}\frac{(k+1)^{k+1}}{3^{k+1}(k+1)!} \frac{3^kk!}{k^k}$
$L = \lim_{k \to \infty}\frac{(k+1)^{k}(k+1)}{3(k+1)(k)!} \frac{k!}{k^k}$
$L = \lim_{k \to \infty}\frac{(k+1)^{k}}{3} \frac{1}{k^k}$
$L = \frac13\lim_{k \to \infty}\frac{(k+1)^{k}}{k^k}$
$L = \frac13\lim_{k \to \infty}(\frac{k+1}{k})^k$
$L = \frac13\lim_{k \to \infty}(1 + \frac{1}{k})^k$
the above limit is the definition of $e$
so $\lim_{k \to \infty}|\frac{d_{K+1}}{d_k}| = \frac13 e$
$L =\frac13 e < 1 \implies$ the series converges absolutely

(e)

look at the second term in $e_k$
$2^{2k-3}e^{-k+2}$
$2^{2k}2^{-3}e^{-k}e^{2}$
$\frac{e^{2}}{8}\frac{4^{k}}{e^{k}}$
$\frac{e^{2}}{8}(\frac{4}{e})^k$
this is a geo series with $r = \frac{4}{e}> 1 \implies$ diverges to $+\infty$
adding back in the $\frac{1}{k^4}$ will only serve to make the sum bigger so the whole series must diverge

{{ENDQUESTION}}
# Question 2

(a)

$\lim_{n \to \infty}\cos(\frac{1}{n^2}) = \lim_{n \to \infty}\cos(0) = 1$
fails screening test

(b)

limit comparison test with $\sum_{k = 1}^\infty\frac{1}{n^2}$ which is known to converge by p-series
$\lim_{n \to \infty}\frac{\sin(\frac{1}{n^2})}{\frac{1}{n^2}}$
take $x = \frac{1}{n^2}$
as $n \to \infty$ $x \to 0$
$\lim_{x \to 0}\frac{\sin(x)}{x}$
the above is a famous limit that $\to 1$
since the answer from the limit comparison test is positive finite and the series that we compared with is convergent, the series we want to know about converges

(c)
AST

is $\frac{1}{3+ 5k}$ positive and decreasing?
positive: yes trivially
decreasing:
$\frac{d}{dk}\frac{1}{3+5k} = -5(3+5k)$
$-5(3+5k) = 0$
$k = -3/5$
test $k = 1$
$-5(3+5(1)) < 0$
so $\forall k > 1$ $\frac{1}{3+ 5k}$ is decreasing
$\lim_{k \to \infty}\frac{1}{3+ 5k} = 0$
passes the AST so it converges

(d)
ratio test
$d_{k+1} = \frac{(-1)^{k+1}(2(k+1))!}{3^{k+1}((k+1)!)^2}$
$\lim_{k \to \infty}|\frac{d_{k+1}}{d_k}| = \lim_{k \to \infty}\frac{(2(k+1))!}{3^{k+1}((k+1)!)^2}\frac{3^k(k!)^2}{2k!}$
$\lim_{k \to \infty}\frac{(2k+2)!}{3^{k}3(k+1)!(k+1)!}\frac{3^kk!k!}{2k!}$
$\lim_{k \to \infty}\frac{(2k+2)(2k+1)(2k)!}{3(k+1)(k)!(k+1)(k)!}\frac{k!k!}{2k!}$
$\lim_{k \to \infty}\frac{(2k+2)(2k+1)}{3(k+1)(k+1)}$
$\frac13\lim_{k \to \infty}\frac{4k^2+6k+2}{k^2 + 2k + 1}$
$\lim_{k \to \infty}|\frac{d_{k+1}}{d_k}| = \frac13\lim_{k \to \infty}\frac{4k^2+6k+2}{k^2 + 2k + 1} = 4 > 1 \implies$ diverges

(e)
roughly the series grows like $\frac{\sqrt{k^3}}{k^3} = \frac{k^{3/2}}{k^3} = \frac{1}{k^{\frac{3}{2}}}$
so limit comparison test with $\sum_{k = 1}^\infty\frac{1}{k^\frac{3}{2}}$ which converges by p-series
$\lim_{k \to \infty}\frac{\frac{\sqrt{k^3+1}}{3k^3+4k^2 +2}}{\frac{1}{k^\frac{3}{2}}}$
$\lim_{k \to \infty}\frac{\sqrt{k^3+1}}{3k^3+4k^2 +2} k^{\frac{3}{2}}$
$\lim_{k \to \infty}\frac{\sqrt{k^3(1+\frac{1}{k^3})}}{3k^3+4k^2 +2} k^{\frac{3}{2}}$
$\lim_{k \to \infty}\frac{k^3\sqrt{(1+\frac{1}{k^3})}}{3k^3+4k^2 +2}$
$\lim_{k \to \infty}\frac{k^3\sqrt{1}}{3k^3+4k^2 +2} = \frac13$
since the limit is positive and finite and the series we compared it to converges the series we want to know about must converge too

{{ENDQUESTION}}
# Question 3

centered at $-3$
Ratio formula
$R = \lim_{k \to \infty}|\frac{\frac{1}{2^k\sqrt{k}}}{\frac{1}{2^{k+1}\sqrt{k+1}}}|$
$R = \lim_{k \to \infty}\frac{2^{k+1}\sqrt{k+1}}{2^k\sqrt{k}}$
$R = \lim_{k \to \infty}\frac{2\sqrt{k+1}}{\sqrt{k}}$
$R = \lim_{k \to \infty}\frac{2\sqrt{k}\sqrt{1+\frac{1}{k}}}{\sqrt{k}}$
$R = \lim_{k \to \infty}\frac{2\sqrt{k}}{\sqrt{k}} = 2$
Radius of convergence is $R = 2$
intermediate interval of convergence is $(-5, -1)$
test endpoints
$x = -1$
$\sum_{k = 1}^\infty\frac{(2)^k}{\sqrt{k}2^k}$
$\sum_{k = 1}^\infty\frac{1}{\sqrt{k}}$
this diverges by p-series so we can't include $x = -1$

$x = -5$

$\sum_{k = 1}^\infty\frac{(-2)^k}{\sqrt{k}2^k}$
$\sum_{k = 1}^\infty\frac{(-1)^k(2)^k}{\sqrt{k}2^k}$
$\sum_{k = 1}^\infty\frac{(-1)^k}{\sqrt{k}}$
this converges by AST so we can include $x = -5$

final interval of convergence is $[-5, -1)$
