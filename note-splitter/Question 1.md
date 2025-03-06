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
- $\hat{v} = \begin{pmatrix} 0.4 \\ 0.3 \\ 0.3 \end{pmatrix}$
 - Meaning that the probabilities stabilise all to 0.4, 0.3, and 0.3 respectively as $n \rightarrow \infty$