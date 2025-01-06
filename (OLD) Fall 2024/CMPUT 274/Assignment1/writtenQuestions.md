1. 
	By the definition of Big-Oh notation
	$g(n) \leq C_1f(n) \; \forall n \geq n_0$
	$h(n) \leq C_2f(n) \; \forall n \geq n_1$
	Multiplying by arbitrary constants $a,b > 0$
	$ag(n) \leq aC_1f(n)$
	$bh(n) \leq bC_2f(n)$
	Adding the equations
	$Let \; n_2 = max(n_0, n_1)$ So that the below equation satisfies the bounds of both original equations
	$ag(n) + bh(n) \leq aC_1f(n) + bC_2f(n) \; \forall n \geq n_2$
	$\Rightarrow ag(n) + bh(n) \leq f(n)(aC_1+bC_2)\; \forall n \geq n_2$
	$Let \; C = (aC_1+bC_2)$
	$\Rightarrow ag(n) + bh(n) \leq Cf(n)\; \forall n \geq n_2$
	$Let \; l(n) = ag(n) + bh(n)$
	$\Rightarrow l(n) \leq Cf(n)\; \forall n \geq n_2$
	The above equation is the definition of Big-Oh notation for the function $l(n)$
	$\therefore I(n) = ag(n) + bh(n) \in O(f(n))$
2. 
	Base Case $n=0$:
		LHS:$$\sum_{i=0}^0r^i = 1$$
		RHS:$$\frac{1-r^{0+1}}{1-r} = \frac{1-r}{1-r} = 1$$
		$RHS = LHS \text{ for } n=0, r \neq 1$
		$\therefore$ the proposed formula holds for $n=0$
	Inductive Hypothesis:
		Assume the equation holds for $m \geq 0$:$$\sum_{i=0}^mr^i = \frac{1-r^{m+1}}{1-r}$$
		We need to prove that this equation works for $n = m+1$
	Inductive Step:
		LHS:$$\sum_{j=0}^{m+1}r^i = \sum_{j=0}^{m}r^i + r^{m+1}$$
		Using our Inductive Hypothesis for the first term of the above equation gives:$$\Rightarrow \frac{1-r^{m+1}}{1-r} + r^{m+1} = \frac{1-r^{m+1}}{1-r} + \frac{r^{m+1}(1-r)}{1-r} = \frac{1-r^{m+1} + r^{m+1}(1-r)}{1-r}$$$$\Rightarrow \frac{1+r^{m+1}-rr^{m+1}-r^{m+1}}{1-r} = \frac{1-r^{m+2}}{1-r}$$
		RHS:$$\frac{1-r^{(m+1)+1}}{1-r} = \frac{1-r^{m+2}}{1-r}$$
		$RHS = LHS$
	since $S_0$ is true and $S_n \implies S_{n+1}$ by induction $S_n$ is true $\forall n \geq 0$
	$\therefore \sum_{i=0}^nr^i = \frac{1-r^{n+1}}{1-r} \text{ holds } \forall n \geq 0, 0 < r < 1$ 
3. 
	Let the Big-Oh of $algorithm1 = a(n) \quad a(n) \leq C_1 nlog(n) \quad \forall n \geq n_1 \quad C_1\in \mathbb{R} \quad n_2 \in \mathbb{Z}$
	Let the Big-Oh of $algorithm2 = b(n) \quad b(n) \leq C_2 n \quad \forall n \geq n_2 \quad C_2 \in \mathbb{R} \quad n_2 \in \mathbb{Z}$
	
	Given that $algorithm2$ calls $algorithm1$ we can multiply the time complexities to find the overall time that  $algorithm2$ takes giving the equation
	$a(n)b(n) \leq C_1nlog(n)C_2n \quad \forall n \geq n_0$
	Let $T(n) = a(n)b(n)$
	Let $n_0 = max(n1,n2)$
	Let $C = C_1C_2$
	$T(n) \leq Cn^2log(n) \quad \forall n \geq n_0$
	
	The above equation is the definition of Big-Oh notation for the function $T(n)$. Meaning that the Big-Oh of $T(n)$ is $O(n^2log(n))$ 
	
	As $T(n)$ is the total time complexity for $algorithm2$ the Big-Oh of $algorithm2$ is $O(n^2log(n))$	

4. 
	a.
		$f(n) = 4n$
	b.
		$g(n) = 2 + 4n(4+4n) = 2 + 4n + 4n^2$
		Explanation:
		The first and the last line happen every time and take 1 step each so there is a constant + 2 added
		The for-loop does n iterations which do $(1+1+1+ ?+1)$ steps each giving $n(1+1+1+1+?)$. Substituting in my answer for (a) gives $n(4+4n) = 4n+4n^2$
		Adding them together gives $\Rightarrow 2 + 4n + 4n^2$
	c.
		$O(n^2)$
		Explanation:
		I will use $g(n)$ as found in part (b) and $f(n) = n^2$
		From the definition of Big-Oh notation
		$g(n) \leq Cf(n) \; \forall n \geq n_0, C>0$
		Choose $C=1000, n_0 = 30$
		$2 + 3(30) + 4(30)^2 \leq 1000(30)^2$
		$3692 \leq 27000$
		QED
	d.
		The exact number of steps of the program written by the friend is given by $h(n) = 2 + nlog(n) + 4nlog(n)$
		Which has the Big-Oh notation of $O(nlog(n))$
		$O(nlog(n)) < O(n^2)$
		$\Rightarrow nlog(n) < n^2$
		$\Rightarrow log(n) < n$
		$\Rightarrow n < 2^n \; \forall n > 0$
		$\therefore$  The running time of the friends algorithm is asymptotically smaller than the TA's for sufficiently large $n$ 