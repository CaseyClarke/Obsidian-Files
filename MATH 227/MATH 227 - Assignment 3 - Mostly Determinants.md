
# Question 1 

$f_{\text{terms}} = A_{1,\sigma(1)}A_{2,\sigma(2)}A_{3,\sigma(3)}A_{4,\sigma(4)}sign(\sigma)$
$\Rightarrow A_{1,1}A_{2,3}A_{3,4}A_{4,2}sign(\sigma)$
$\Rightarrow (2)(-4)(5)(8)(1)$
$\Rightarrow -320$

$g_{\text{terms}} = A_{1,\sigma(1)}A_{2,\sigma(2)}A_{3,\sigma(3)}A_{4,\sigma(4)}sign(\sigma)$
$\Rightarrow A_{1,3}A_{2,1}A_{3,4}A_{4,2}sign(\sigma)$
$\Rightarrow (1)(-1)(5)(8)(-1)$
$\Rightarrow 40$

$h_{\text{terms}} = A_{1,\sigma(1)}A_{2,\sigma(2)}A_{3,\sigma(3)}A_{4,\sigma(4)}sign(\sigma)$
$\Rightarrow A_{1,2}A_{2,3}A_{3,4}A_{4,1}sign(\sigma)$
$\Rightarrow (0)A_{2,3}A_{3,4}A_{4,1}sign(\sigma)$
$\Rightarrow 0$

{{ENDQUESTION}}

# Question 2

$F(a+2b,a-2b) = F(a,a) -2F(a,b) + 2F(b,a) + 4F(b,b)$
$F(a+2b,a-2b) = 1 -2F(a,b) + 2F(b,a) + 4$
$F(a,b) = F(b,a)$
$F(a+2b,a-2b) = 1 -2F(a,b) + 2F(a,b) + 4$
$F(a+2b,a-2b) = -3$

{{ENDQUESTION}}

# Question 3

$$
\begin{pmatrix}
a & b & c & d \\
-a+b & 0 & -c+b & -d+b \\
0 & 1 & 2 & 3 \\
a & a+1 & a+2 & a+3
\end{pmatrix}
\xrightarrow{
    \begin{subarray}{l}
        R_2 \leftarrow  R_2 + R_1\\
        R_4 \leftarrow  R_4 - R_3
    \end{subarray}
}
\begin{pmatrix}
a & b & c & d \\
b & b & b & b \\
0 & 1 & 2 & 3 \\
a & a & a & a
\end{pmatrix}
\xrightarrow{
    \begin{subarray}{l}
        R_4 \leftarrow  (a^{-1}R_4) - (b^{-1}R_2)
    \end{subarray}
}
\begin{pmatrix}
a & b & c & d \\
1 & 1 & 1 & 1 \\
0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0
\end{pmatrix}
$$

Row of 0's $\implies$not invertible

{{ENDQUESTION}}

# Question 4

(a)

$\operatorname{det}(-5A^2B^3A^T) = \operatorname{det}(-5)\operatorname{det}(A^2)\operatorname{det}(B^3)\operatorname{det}(A^T) \neq 0$
$\operatorname{det}(-5A^2B^3A^T) = (-5)^n\operatorname{det}(A)^2\operatorname{det}(B)^3\operatorname{det}(A) \neq 0$
$\operatorname{det}(-5A^2B^3A^T) = (-5)^n\operatorname{det}(A)^3\operatorname{det}(B)^3 \neq 0$
$\therefore \; \operatorname{det}(A) \neq 0\text{ and } \operatorname{det}(B) \neq 0 \implies$ invertible

(b)

$\operatorname{det}(2AB^{-1}A^TB^2) = 2^3\operatorname{det}(A)\operatorname{det}(B)^{-1}\operatorname{det}(A)\operatorname{det}(B)^2$
$\operatorname{det}(2AB^{-1}A^TB^2) = 8(-1)2^{-1}(-1)(4)$
$\operatorname{det}(2AB^{-1}A^TB^2) = 16$

(c)

$\operatorname{det}(A^T) = \operatorname{det}(A)$
$\operatorname{det}(-A) = \operatorname{det}(A)$
$\operatorname{det}(-A) = \operatorname{det}(-I_7)\operatorname{det}(A)$
$\operatorname{det}(-A) = (-1)^7 \operatorname{det}(A)$
$\operatorname{det}(-A) = -\operatorname{det}(A) = \operatorname{det}(A)$
$\operatorname{det}(A) = -\operatorname{det}(A) \implies \operatorname{det}(A) = 0 \implies$ not invertible

{{ENDQUESTION}}

# Question 5

$\operatorname{det}(A) = (1)(0)(a) + (-1)(-1)(2) + (3)(1)(1) - (3)(0)(2) - (1)(-1)(1) - (a)(1)(-1) \neq 0$
$\operatorname{det}(A) = a+6 \neq 0$
$a \neq -6$ (mod 13)

{{ENDQUESTION}}

# Question 6

$$
\begin{pmatrix}
2 & 0 & 1 & 2 \\
-1 & 2 & -4 & -1 \\
-4 & 3 & -1 & 0 \\
-5 & 8 & -4 & 3
\end{pmatrix}
\xrightarrow{
    \begin{subarray}{l}
        R_4 \leftarrow R_4 -(2R_1 + 1R_2 + 2R_3)\\
    \end{subarray}
}
\begin{pmatrix}
2 & 0 & 1 & 2 \\
-1 & 2 & -4 & -1 \\
-4 & 3 & -1 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix}
$$

Row of 0's $\implies$not invertible $\implies$ $\operatorname{det}(A) = 0$

{{ENDQUESTION}}


