# Question 1

Size of matrix is $10\times10$

$\operatorname{Dim}(\operatorname{Null}((A-\pi I))) = 3$

$J(A) = J_4(\pi)\oplus J_3(\pi)\oplus J_3(\pi)$

{{ENDQUESTION}}

# Question 2

(a)

- $\operatorname{det}(A-\lambda I) = \lambda^4 \quad \lambda = 0$
- $\operatorname{Dim}(\operatorname{Null}(A - 0I)) = \operatorname{Dim}(\operatorname{Null}(A))$ 
- $\operatorname{Null}(A) = \left\{ \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix} \right\}$
- $\operatorname{Dim}(\operatorname{Null}(A)) = 2 \implies$ There are 2 Jordan blocks

- $A^2 = \begin{pmatrix} 0 & 0 & 0 & 1 \\ 0 & 0 & 0 & -2 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ \end{pmatrix}$

- $\operatorname{Dim}(\operatorname{Null}(A^2)) = 4 - 2 = 2 \implies$ At least 2 blocks of size 2

- $J = \begin{pmatrix} J_2(0) & 0 \\ 0 & J_2(0)\end{pmatrix}$
- The columns of P are the 2 vectors of $\operatorname{Null}(A)$ $v_1 =  \begin{pmatrix} 1 \\ 0 \\ 0 \\ 0 \end{pmatrix} v_3 = \begin{pmatrix} 0 \\1 \\ 0 \\ 0 \end{pmatrix}$ 
  plus 2 generalised eigenvectors, $x,y$ where $Ax = v_1$ and $Ay = v_3$
- solving these equations gives 
  $x = \begin{pmatrix} 0 \\ 0 \\ 1 \\ 0 \end{pmatrix} y = \begin{pmatrix} 0 \\0 \\ 5 \\ 1 \end{pmatrix}$
- Meaning that $P = \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 5 \\ 0 & 0 & 0 & 1\end{pmatrix}$
(b)9

- $\operatorname{det}(A-\lambda I) = \lambda^4 - 4\lambda^3+4\lambda^2$
- $\lambda^4 - 4\lambda^3+4\lambda^2 = \lambda^2(\lambda^2 - 4\lambda + 4\lambda)$