
# Question 1

(a)

- $A = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}$

(b)

- $p = \begin{pmatrix} p_1 \\ p_2 \\ p_3 \end{pmatrix}$
- $Ap = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\begin{pmatrix} p_1 \\ p_2 \\ p_3 \end{pmatrix} = \begin{pmatrix} 0p_1 + 2/3 p_2 + 2/3p_3 \\ 1/2p_1 + 0 p_2 + 1/3p_3 \\ 1/2 p_1 + 1/3 p_2 + 0p_3 \end{pmatrix}$
- $(0p_1 + 2/3 p_2 + 2/3p_3) + (1/2p_1 + 0 p_2 + 1/3p_3 )+ (1/2 p_1 + 1/3 p_2 + 0p_3)$
- $\Rightarrow (0 + 1/2 + 1/2)p_1 + (2/3 + 0 + 1/3)p_2 + (2/3 + 1/3 + 0)p_3 =  p_1 + p_2 + p_3 = 1$ 
- $\therefore Ap$ is a probablility vector

(c)

- To compute this probability we use the probability vector
- $p = \begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}$
- and left multiply by A twice 

- $A(Ap) = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\left(\begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}\right)$
- but $Ap = \begin{pmatrix} 2/3 \\ 0 \\ 1/3 \end{pmatrix}$ by the rules of the question
- $A(Ap) = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\begin{pmatrix} 2/3 \\ 0 \\ 1/3 \end{pmatrix} = \begin{pmatrix} 2/9 \\ 4/9 \\ 1/3 \end{pmatrix}$
- $\therefore$ The probability of having bacterial broth on the first day and then again 2 days later is $4/9$

(d)

- Given that $P_{n+1} = Ap_n$ we know that $P_n = A^np_0$ where $p_0$ is the initial probability vector
- we can diagonalize $A$ as $A = QDQ^{-1}$ and $A^n = QD^nQ^{-1}$
- $lim_{n\rightarrow \infty}A^n = Q\begin{pmatrix} 1^n & 0 & 0 \\ 0 & (-2/3)^n & 0 \\ 0 & 0 & (-1/3)^n\end{pmatrix}Q^{-1}$
- and from the useful fact in the question we know that
- $lim_{n\rightarrow \infty}A^n = Q\begin{pmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0\end{pmatrix}Q^{-1}$
- Which implies that the eigenvector corresponding to the eigenvalue of 1 is stable as n goes to infinity but the other eigenvalues decay to 0, meaning that finding the eigenvector that corresponds to 1 would give us the long running probabilities regardless of the initial input

- $\operatorname{Null}(A-(1)I) = \operatorname{Null}\begin{pmatrix} -1 & 2/3 & 2/3  \\ 1/2 & -1 & 1/3 \\ 1/2 & 1/3 & -1\end{pmatrix}$
- Solving for this null space with the additional stipulation that $p_1 + p_2 + p_3 = 1$
- we get that 
- $\hat{v} = \begin{pmatrix} 1/3 \\ 1/3 \\ 1/3 \end{pmatrix}$

{{ENDQUESTION}}

# Question 2

We need to show that $A \sim B \implies det(A) = det(B)$ 
$A = PBP^{-1}$
$det(A) = det(PBP^{-1}) = det(P)det(B)det(P^{-1}) = \frac{det(P)}{det(P)}det(B) = det(B)$
$det(A) = det(B)$

{{ENDQUESTION}}

# Question 3

(a)

- any $r \in \mathbb{Q}$ can be written in the form $r = r + 0\sqrt{3}$
- $C(r) = C(r+0\sqrt{3}) = r -0\sqrt{3} = r$
- $C(r) = r$

(b)

- $C = C^{-1}$
- as $C(C(a+b\sqrt{3})) = a+b\sqrt{3}$

(c)

- $x = a+b\sqrt{3}$
- $y = c+d\sqrt{3}$

- $C(0) = 0$
	- $0 = 0 + 0\sqrt{3}$
	- $C(0+0\sqrt{3}) = 0 - 0 \sqrt{3} = 0$
	- $C(0) = 0$

- $C(1) = 1$
	- $1 = 1 + 0\sqrt{3}$
	- $C(1+0\sqrt{3}) = 1-0\sqrt{3} = 1$
	-  $C(1) = 1$

- $C(x+y) = C(x) + C(y)$
	- $C(a+b\sqrt{3} + c + d\sqrt{3}) = C((a+c) + (b+d)\sqrt{3}) = (a+c) - (b+d)\sqrt{3}$
	- $\Rightarrow (a-b\sqrt{3}) + (c-d\sqrt{3}) = C(x) + C(y)$

- $C(xy) = C(x)C(y)$
	- $C(xy) = C((ac + 3bd) +(ad+bc)\sqrt{3}) = (ac + 3bd) -(ad+bc)\sqrt{3}$
	- $C(x)C(y) = (a-b\sqrt{3})(c-d\sqrt{3}) = (ac + 3bd) -(ad+bc)\sqrt{3}$
	- $C(xy) = C(x)C(y)$
- 
{{ENDQUESTION}}

# Question 4

 - $P_A$
	- $\text{Size} = 2$
	- $det(A) = -1$
	- $\text{Trace} = 0$
	- $\text{Invertible} = \text{True}$
	- $\lambda = \pm 1$
 - $P_B$
	- $\text{Size} = 2$
	- $det(A) = 1$
	- $\text{Trace} = 2$
	- $\text{Invertible} = \text{True}$
	- $\lambda = 1$
 - $P_C$
	- $\text{Size} = 4$
	- $det(A) = 0$
	- $\text{Trace} = 0$
	- $\text{Invertible} = \text{False}$
	- $\lambda = 0$
 - $P_D$
	- $\text{Size} = 3$
	- $det(A) = 0$
	- $\text{Trace} = 1$
	- $\text{Invertible} = \text{False}$
	- $\lambda = -2, 0, 1$

{{ENDQUESTION}}

# Question 5

$v_n = \begin{pmatrix} f_{n} \\ f_{n+1} \\ f_{n+2}\end{pmatrix}$
$v_{n+1} = \begin{pmatrix} f_{n+1} \\ f_{n+2} \\ f_{n+3}\end{pmatrix}$

$v_{n+1} = Av_n$

$\begin{pmatrix} f_{n+1} \\ f_{n+2} \\ f_{n+3}\end{pmatrix} = A\begin{pmatrix} f_{n} \\ f_{n+1} \\ f_{n+2}\end{pmatrix}$

$A = \begin{pmatrix} 1 & -9 & 9 \\ 1 & 0 & 0 \\ 0 & 1 & 0\end{pmatrix}$

$v_n = A^n\begin{pmatrix} f_1 \\ f_2 \\ f_3\end{pmatrix}$

$\operatorname{det}(A-\lambda I) = -\lambda^3+\lambda^2 - 9\lambda + 9 = -(1-\lambda)(\lambda^2 + 9)$
$\lambda = 1, \pm 5$

$\operatorname{null}(A-\lambda) = \begin{pmatrix} 1 \\ 1 \\ 1\end{pmatrix}$
$\operatorname{null}(A-5\lambda) = \begin{pmatrix} 1 \\ 7 \\ -2\end{pmatrix}$
$\operatorname{null}(A+5\lambda) = \begin{pmatrix} 1 \\ 10 \\ -2\end{pmatrix}$
$P = \begin{pmatrix} 1 & 1 & 1 \\ 1 & 7 & 10 \\ 1 & -2 & -2 \end{pmatrix}$
$D = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 5 & 0 \\ 0 & 0 & -5\end{pmatrix}$
$P^{-1} \begin{pmatrix} -5 & 0 & 6 \\ 7 & -6 & -1 \\ -1 & 6 & -5 \end{pmatrix}$
$A^n = PD^nP^{-1}$


$$
A^n = 
\begin{pmatrix} 
-(-5)^n+7(5)^n-5 & 6(-5)^n-6(5)^n & -5(-5)^n-5^n+6 \\
\dots & \dots & \dots \\
\dots & \dots & \dots \\
\end{pmatrix}$$

$$v_n = A^n\begin{pmatrix} f_1 \\ f_2 \\ f_3\end{pmatrix} = \begin{pmatrix} 
-(-5)^n+7(5)^n-5 & 6(-5)^n-6(5)^n & -5(-5)^n-5^n+6 \\
\dots & \dots & \dots \\
\dots & \dots & \dots \\
\end{pmatrix}
\begin{pmatrix} f_1 \\ f_2 \\ f_3\end{pmatrix}
$$
$$=
\begin{pmatrix} 
f_1(-(-5)^n+7(5)^n-5) + f_2(6(-5)^n-6(5)^n) + f_3(-5(-5)^n-5^n+6) \\
\dots \\
\dots
\end{pmatrix}  
$$
$$\begin{pmatrix} f_{n} \\ f_{n+1} \\ f_{n+2}\end{pmatrix} = \begin{pmatrix} 
f_1(-(-5)^n+7(5)^n-5) + f_2(6(-5)^n-6(5)^n) + f_3(-5(-5)^n-5^n+6) \\
\dots \\
\dots
\end{pmatrix}$$
$f_n = f_1(-(-5)^n+7(5)^n-5) + f_2(6(-5)^n-6(5)^n) + f_3(-5(-5)^n-5^n+6)$










