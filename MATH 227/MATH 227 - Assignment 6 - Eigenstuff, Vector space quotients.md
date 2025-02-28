
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

- To compute this probability we use the probability matrix
- $p = \begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}$
- and left multiply by A twice 

- $A(Ap) = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\left(\begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}\right)$
- but $Ap = \begin{pmatrix} 2/3 \\ 0 \\ 1/3 \end{pmatrix}$ by the rules of the question
- $A(Ap) = \begin{pmatrix} 0 & 2/3 & 2/3  \\ 1/2 & 0 & 1/3 \\ 1/2 & 1/3 & 0\end{pmatrix}\begin{pmatrix} 2/3 \\ 0 \\ 1/3 \end{pmatrix} = \begin{pmatrix} 2/9 \\ 4/9 \\ 1/3 \end{pmatrix}$
- $\therefore$ The probability of having bacterial broth on the first day and then again 2 days later is $4/9$

(d)

- Given that $P_{n+1} = Ap_n$ we know that $P_n = A^np_0$ where $p_0$ is the initial probability vector
- 
- 
- 