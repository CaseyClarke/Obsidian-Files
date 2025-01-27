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
$[T(i)]_{\beta}  = [3-2i]_B =\begin{pmatrix} 3 \\ -2 \end{pmatrix}$
$[T]_{\beta \leftarrow \beta} = \begin{pmatrix} 2 & 3 \\ 3 & -2 \end{pmatrix}$

(d)

$[T^{-1}]_{\beta \leftarrow \beta} = ([T]_{\beta \leftarrow \beta})^{-1} = \begin{pmatrix} 2 & 3 \\ 3 & -2 \end{pmatrix}^{-1}$
$$\begin{pmatrix} 2 & 3 \\ 3 & -2 \\ \end{pmatrix}^{-1} = \frac{1}{-13}\begin{pmatrix} -2 & -3 \\ -3 & 2 \\ \end{pmatrix} = \begin{pmatrix} 2/13 & 3/13 \\ 3/13 & -2/13  \end{pmatrix}$$
$T^{-1}(x+iy)= \begin{pmatrix} 2/13 & 3/13 \\ 3/13 & -2/13  \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 2/13(x) + 3/13(y) \\ 3/13(x) - 2/13(y)  \end{pmatrix}$
$= (2/13(x) + 3/13(y)) + i(3/13(x) - 2/13(y))$