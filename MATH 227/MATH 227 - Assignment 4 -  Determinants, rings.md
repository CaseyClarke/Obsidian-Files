# Question 1 

(a)
- $\operatorname{det}\begin{pmatrix}3 & -4 & -2 \\0 & 1 & 1 \\-6 & 7 & 5\end{pmatrix}=6$ by criss cross
- $\operatorname{det} \neq 0 \implies$ Linearly independant

(b)
-  $\operatorname{det}\begin{pmatrix}1 & -3 & -4 \\-2 & 5 & 5 \\3 & 7 & 6\end{pmatrix}= 0$ by criss cross
- $\operatorname{det} = 0 \implies$ Linearly dependant
- By make your life easy they cannot span all of $P_2(\mathbb{R})$
- 
{{ENDQUESTION}}

# Question 2

(a)

- $\vec{u} = (2,-3)$
- $\vec{v} = (-1,1)$
- $area = \operatorname{det}\begin{pmatrix} -1 & 1 \\ 2 & -3\end{pmatrix} = 1$

(b)

- Translating all points by $(-2,3)$ so that we have a point at $(0,0)$ for easy calculation we get
- $\vec{u} = (-4,1)$
- $\vec{v} = (-3,4)$
- $area = \frac12\operatorname{det}\begin{pmatrix} -4 & -3 \\ 1 & 4\end{pmatrix} = \frac12\left|-13\right| =\frac{13}{2}$

{{ENDQUESTION}}

# Question 3

$$
\operatorname{det}
\begin{vmatrix}
1 & 1 & 2 \\
-2 & 1 & -2 \\
2 & -1 & 1 
\end{vmatrix}
=
1
\begin{vmatrix}
-2 & -2 \\
2 & 1
\end{vmatrix}
+1
\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
-1
\begin{vmatrix}
1 & 2 \\
-2 & -2
\end{vmatrix}
=
2 + -3 -2
=
-3

$$
{{ENDQUESTION}}

# Question 4

$\operatorname{det}(A) = 76$ by criss cross
$$
(A^{-1})_{1,2} = \frac{(-1)^{1+2}}{\operatorname{det}(A)}
\begin{vmatrix} 4 & -1 \\ -2  & 5 \end{vmatrix}
=
\frac{-1}{76}
(18)
=
\frac{-18}{76}
$$
{{ENDQUESTION}}

# Question 5

$\operatorname{det}(A) = 6 \equiv 1$ by criss cross

$$x = \frac{
\begin{vmatrix}
A & 1 & -1 \\
B & 4 & 0 \\
C & 1 & 2
\end{vmatrix}
}{1}
=
3A-3B+4C
$$
$$y = \frac{
\begin{vmatrix}
1 & A & -1 \\
2 & B & 0 \\
1 & C & 2
\end{vmatrix}
}{1}
=
−4A+3B−2C
$$
$$z = \frac{
\begin{vmatrix}
1 & 1 & A \\
2 & 4 & B \\
1 & 1 & C
\end{vmatrix}
}{1}
=
-2A + 2C
$$

{{ENDQUESTION}}

# Question 6 


Multiplicitive identity:
- $1_R1_R = 1_R = 1_R1_R$
- $1_R \in U$ as it is its own inverse

Closure:
- $uv(v^{-1}u^{-1}) = 1_R = (v^{-1}u^{-1})uv$
- $uv \in U$ as $v^{-1}u^{-1}$ is it's inverse

Multiplicitive inverse:
- $u \in U \implies uu^{-1} = 1_R = u^{-1}u$
- $u^{-1} \in U$ as $u$ is it's inverse

{{ENDQUESTION}}


# Question 7

Let the matricies be $A,B,C$ Respectivly, determinants taken by criss cross
$\operatorname{det}(A) = -1 \implies$ Invertible as $-1 \in U(\mathbb{Z}[x])$
$\operatorname{det}(B)) = −21x^2+7x−4 \implies$ not invertible as $−21x^2+7x−4 \notin U(\mathbb{Z}[x])$
$\operatorname{det}(C) = -1 \implies$ Invertible as $-1 \in U(\mathbb{Z}[x])$

$A^{-1} = \frac{1}{-1}\begin{pmatrix} -1 & -2x^3+3x - 5 \\ 0 & 1\end{pmatrix} = \begin{pmatrix} 1 & 2x^3-3x + 5 \\ 0 & -1\end{pmatrix} = A$

$C^{-1} = \frac{1}{-1}\begin{pmatrix} 2x+1 & -4 \\ -x^2 & 2x-1 \end{pmatrix} = \begin{pmatrix} -2x-1 & 4 \\ x^2 & -2x+1 \end{pmatrix}$

{{ENDQUESTION}}