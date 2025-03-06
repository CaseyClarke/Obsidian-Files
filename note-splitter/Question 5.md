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
-(-1)^n5^nf_1+7(5)^nf_1-5f_1+6(-1)^n5^nf_2-6(5)^nf_2-5(-1)^n5^nf_3-5^nf_3+6f_3 \\
\dots \\
\dots
\end{pmatrix}$$

$f_n = f_1(6 + (-2(-5)^{n}-3(5)^{n})) - f_2((5)^n+(-5)^n) + f_3(-5 + (3(-5)^n+4(5)^n))$