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