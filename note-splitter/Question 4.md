# Question 4

(a)

$det(A-\lambda I) = (1-\lambda)(-\lambda) - 6 = \lambda^2-\lambda - 6$
$\lambda^2-\lambda - 6 = 0$
$(\lambda + 2)(\lambda - 3) = 0$
$\lambda = -2,3$

but $-2 \equiv 3$ (mod 5) so the P matrix would have two dependant columns meaning we cannot diagonalize the matrix

(b)

starting from where we left off in (a)

$\operatorname{Null}(A-3I) = \begin{pmatrix} 3 \\ 1\end{pmatrix}$
$\operatorname{Null}(A+2I) = \begin{pmatrix} -2 \\ 1\end{pmatrix}$

$P = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}$

$P^{-1} = \frac15 \begin{pmatrix}  1 & 2 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix}$

$D = \begin{pmatrix}  3 & 0 \\ 0 & -2 \end{pmatrix}$

(c)

$A^n = PD^nP^{-1}$
$\sqrt{B} = P\sqrt{D}P^{-1}$

$\sqrt{3} = \sqrt{25} = \pm 5$
$\sqrt{-2} = \sqrt{9} = \pm3$

$\sqrt{B}_1 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  5 & 0 \\ 0 & 3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  2 & -2 \\ -4 & -5 \end{pmatrix}$
$\sqrt{B}_2 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  -5 & 0 \\ 0 & 3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  -4 & -3 \\ 5 & 2 \end{pmatrix}$
$\sqrt{B}_3 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  5 & 0 \\ 0 & -3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  4 & 3 \\ -5 & -2 \end{pmatrix}$
$\sqrt{B}_4 = \begin{pmatrix}  3 & -2 \\ 1 & 1 \end{pmatrix}\begin{pmatrix}  -5 & 0 \\ 0 & -3 \end{pmatrix}\begin{pmatrix}  9 & 7 \\ 2 & 5 \end{pmatrix} = \begin{pmatrix}  -2 & 2 \\ 4 & 5 \end{pmatrix}$