# Question 4

$$[T(1,0,0)]_{\beta} = [3, 0, 3]_{\beta} = \begin{pmatrix} 3 \\ 0 \\ 3\end{pmatrix}$$
$$[T(0,1,0)]_{\beta} = [1, -1, -1]_{\beta} = \begin{pmatrix} 1 \\ -1 \\ -1\end{pmatrix}$$
$$[T(0,0,1)]_{\beta} = [1, 1, 1]_{\beta} = \begin{pmatrix} 1 \\ 1 \\ 1\end{pmatrix}$$
$$[T]_{\beta \leftarrow \beta} = \begin{pmatrix} 3 & 1 & 1 \\ 0 & -1 & 1  \\ 3 & -1 & 1\end{pmatrix}$$

$$[T(0,1,4)]_{\beta} = [(5,3,3)]_{\beta} = \begin{pmatrix} 5 \\ 3 \\ 3\end{pmatrix}$$
$$[T(1, 0 , -3)]_{\beta} = [(0, -3, 0)]_{\beta} = \begin{pmatrix} 0 \\ -3 \\ 0\end{pmatrix}$$
$$[T(2,3,7)]_{\beta} = [(16, 4, 10)]_{\beta} = \begin{pmatrix} 16 \\ 4 \\ 10\end{pmatrix}$$
$$[T]_{\beta \leftarrow \beta'} = \begin{pmatrix} 5 & 0 & 16 \\ 3 & -3 & 4 \\ 3 & 0 & 10\end{pmatrix}$$

$$[P]_{\beta' \leftarrow \beta} = \begin{pmatrix} 0 & 1 & 2 \\ 1 & 0 & 3  \\ 4 & -3 & 7\end{pmatrix}$$
$$[P]_{\beta \leftarrow \beta'} = [P]_{\beta' \leftarrow \beta}^{-1} = \begin{pmatrix} -9 & 13 & -3 \\ -5 & 8 & -2  \\ 3 & -4 & 1\end{pmatrix}$$

$$[T]_{\beta' \leftarrow \beta'} = [P]_{\beta \leftarrow \beta'}[T]_{\beta \leftarrow \beta}[P]_{\beta' \leftarrow \beta} = \begin{pmatrix} -9 & 13 & -3 \\ -5 & 8 & -2  \\ 3 & -4 & 1\end{pmatrix}\begin{pmatrix} 3 & 1 & 1 \\ 0 & -1 & 1  \\ 3 & -1 & 1\end{pmatrix}\begin{pmatrix} 0 & 1 & 2 \\ 1 & 0 & 3  \\ 4 & -3 & 7\end{pmatrix}$$
$$ = \begin{pmatrix}
-2 & -1 &-5 \\
6 & -11 & -13 \\
6 & -1 & 3​
\end{pmatrix}$$