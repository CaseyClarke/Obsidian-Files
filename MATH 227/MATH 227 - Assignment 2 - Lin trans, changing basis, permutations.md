
# Question 1

(a)

$dim(domain) = dim(Ker(T) + dim(Im(T)$
$\Rightarrow 4 = dim(Ker(T) + dim(Im(T)$
$dim(Ker(T)) \in (0,4)$
$\Rightarrow dim(Ker(T)) = 4 - dim(Im(T))$
$dim(Im(T)) \in (0,4)$

(b)

$dim(domain) = dim(Ker(S) + dim(Im(S)$
$\Rightarrow 6 = dim(Ker(S) + dim(Im(S)$
$dim(Im(S)) \in (0,4)$
$\Rightarrow dim(Ker(S)) = 6 - dim(Im(S))$
$dim(Ker(S)) \in (2,6)$

{{ENDQUESTION}}

# Question 2

(a)

Any complex number is in the form $a +bi \quad a,b \in \mathbb{R}$
The linear combination of the two basis vectors can be written as
$c_1(1) + c_2(i) \quad c_1,c_2 \in \mathbb{R}$
$a,b = c_1,c_2$
The linear combination is in the exact form of any complex number
They are linearly independent as the only solution to $a(1) + b(i) = 0$
is $a = 0 \text{ and } b = 0$

(b)

$z,z' \in \mathbb{C} \quad c \in \mathbb{R}$

$T(z + z') = (2+3i)\overline{z + z'}$
$T(z + z') = (2+3i)\overline{z} + (2+3i)\overline{z'} = T(z) + T(z')$

$T(cz) = (2+3i)\overline{cz} = c(2+3i)\overline{z} = cT(z)$

(c)

$[T(1)]_{\beta} = \begin{pmatrix} 2 \\3 \end{pmatrix}$
$[T(i)]_{\beta}  = [3-2i]_B =\begin{pmatrix} 3 \\2 \end{pmatrix}$
$[T]_{\beta \leftarrow \beta} = \begin{pmatrix} 2 & 3 \\ 3 & -2 \end{pmatrix}$

(d)

$[T^{-1}]_{\beta \leftarrow \beta} = ([T]_{\beta \leftarrow \beta}) = \begin{pmatrix} 2 & 3 \\ 3 & -2 \end{pmatrix}$
$$\begin{pmatrix} 2 & 3 \\ 3 & -2 \\ \end{pmatrix}^{-1} = \frac{1}{-13}\begin{pmatrix} -2 & -3 \\ -3 & 2 \\ \end{pmatrix} = \begin{pmatrix} 2/13 & 3/13 \\ 3/13 & -2/13  \end{pmatrix}$$
$T^{-1}(x+iy)= \begin{pmatrix} 2/13 & 3/13 \\ 3/13 & -2/13  \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 2/13(x) + 3/13(y) \\ 3/13(x) - 2/13(y)  \end{pmatrix}$
$= (2/13(x) + 3/13(y)) + i(3/13(x) - 2/13(y))$

{{ENDQUESTION}}

# Question 3

Domain: $\mathbb{R}^2$
Codomain: $P_1(\mathbb{R})$

$\beta = (1, x)$
$\beta' = ((1,0),(0,1))$
$$[T(1)]_{\beta'} = [(1,1)]_{\beta} = \begin{pmatrix} 1 \\ 1 \end{pmatrix}$$ 
$$[T(x)]_{\beta'} = [(0,2)]_{\beta} = \begin{pmatrix} 0 \\ 2 \end{pmatrix}$$ 
$$[T]_{\beta' \leftarrow \beta} = \begin{pmatrix} 1 & 0\\ 1 & 2\end{pmatrix}$$
$$\begin{pmatrix} 1 & 0\\ 1 & 2\end{pmatrix}^{-1} = \frac 12 \begin{pmatrix} 2 & 0\\ -1 & 1\end{pmatrix} = \begin{pmatrix} 1 & 0\\ -1/2 & 1/2\end{pmatrix}$$

{ENDQUESTION}}

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


{{ENDQUESTION}}

# Question 5

(a)

$$[p(t)]_{\beta} = \begin{pmatrix} 0 \\ -1 \\ 4 \end{pmatrix}$$
$$[p(t)]_{\beta'} = \begin{pmatrix} 7 \\ 2 \\ -3 \end{pmatrix}$$

(b)

$$[P]_{\beta \leftarrow \beta'} = \begin{pmatrix}
2 & 3 & 1 \\
0 & 1 & 1 \\
1 & 0 & 1 ​
\end{pmatrix}$$
$$[P]_{\beta' \leftarrow \beta} = [P]_{\beta \leftarrow \beta'}^{-1} = \begin{pmatrix}
-4 & -5 & 9 \\
-4 & -4 & 8 \\
4 & 5 & 9 ​
\end{pmatrix}$$
$$[P]_{\beta \leftarrow \beta''} = \begin{pmatrix}
1 & 0 & 1 \\
1 & 0 & 2 \\
2 & 1 & 0 ​
\end{pmatrix}$$
$$[P]_{\beta'' \leftarrow \beta} = [P]_{\beta \leftarrow \beta''}^{-1} = \begin{pmatrix}
2 & -1 & 0 \\
-4 & 2 & 1 \\
-1 & 1 & 0 ​
\end{pmatrix}$$

(c)

$$\begin{pmatrix}
-4 & -5 & 9 \\
-4 & -4 & 8 \\
4 & 5 & 9 ​
\end{pmatrix}\begin{pmatrix} 0 \\ -1 \\ 4 \end{pmatrix} = \begin{pmatrix} 7 \\ 2 \\ -3 \end{pmatrix}$$
(d)

$$\begin{pmatrix}
2 & -1 & 0 \\
-4 & 2 & 1 \\
-1 & 1 & 0 ​
\end{pmatrix}
\begin{pmatrix} 0 \\ -1 \\ 4 \end{pmatrix} = \begin{pmatrix} 1 \\ 2 \\ -1 \end{pmatrix}$$
(e)




# Question 6

(a)

$$\begin{pmatrix} 1 & 2 & 3 & 4 \\ 1 & 3 & 4 & 2 \\ \end{pmatrix} \circ \begin{pmatrix} 1 & 2 & 3 & 4 \\ 3 & 1 & 4 & 2 \\ \end{pmatrix} = \begin{pmatrix} 1 & 2 & 3 & 4 \\ 4 & 1 & 2 & 3 \\ \end{pmatrix}$$
$$\begin{pmatrix} 1 & 2 & 3 & 4 \\ 3 & 1 & 4 & 2 \\ \end{pmatrix}\circ \begin{pmatrix} 1 & 2 & 3 & 4 \\ 1 & 3 & 4 & 2 \\ \end{pmatrix}   = \begin{pmatrix} 1 & 2 & 3 & 4 \\ 3 & 4 & 2 & 1 \\ \end{pmatrix}$$
(b)

$$h^{-1} = \begin{pmatrix} 2 & 3 & 4 & 1 \\ 1 & 2 & 3 & 4 \\ \end{pmatrix} = \begin{pmatrix} 1 & 2 & 3 & 4 \\ 4 & 1 & 2 & 3 \\ \end{pmatrix}$$

(c)

$$P(h) = 
\begin{pmatrix} 0 & 0 & 0 & 1 \\ 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \end{pmatrix}$$