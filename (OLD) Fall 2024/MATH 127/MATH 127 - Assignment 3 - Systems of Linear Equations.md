1
(a)
$$\begin{pmatrix}
	3&2&1&3\\
	2&4&-3&-8\\
	1&1&-2&-4\\
	2&1&3&7\\
	\end{pmatrix}	$$
$R_4 \leftarrow R_4 + R_3$
$R_4 \leftarrow R_4 - R_1$ 
$R_1 \leftarrow R_1 - R_2$
$$\begin{pmatrix}
	1&-2&4&11\\
	2&4&-3&-8\\
	1&1&-2&-4\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - 2R_3$
$R_3 \leftarrow R_3 - R_1$
$R_3 \leftarrow \frac13R_3$
$$\begin{pmatrix}
	1&-2&4&11\\
	0&2&1&0\\
	0&1&-2&-5\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_1 \leftarrow R_1 + R_2$
$R_2 \leftarrow R_2 - R_3$
$$\begin{pmatrix}
	1&0&5&11\\
	0&1&3&5\\
	0&1&-2&-5\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_3 \leftarrow R_3 - R_2$
$R_3 \leftarrow \frac{1}{-5}R_3$
$R_2 \leftarrow R_2 - 3R_3$
$R_1 \leftarrow R_1 -5R_3$
$$\begin{pmatrix}
	1&0&0&1\\
	0&1&0&-1\\
	0&0&1&2\\
	0&0&0&0\\
	\end{pmatrix}$$
$x = 1, y = -1, z = 2$

(b)

$$\begin{pmatrix}
	1&1&-2&3\\
	3&4&2&9\\
	2&3&4&6\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - R_3$
$R_2 \leftarrow R_2 - R_1$
$R_2 \leftrightarrow R_3$
$$\begin{pmatrix}
	1&1&-2&3\\
	2&3&4&6\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - 2R_1$
$R_1 \leftarrow R_1 - R_2$
$$\begin{pmatrix}
	1&0&-10&3\\
	0&1&8&0\\
	0&0&0&0\\
	\end{pmatrix}$$
$w = t_1$
$v= - 8t_1$
$u = 10t_1 + 3$

(c)

$$\begin{pmatrix}
	1&-5&-2&6\\
	3&2&-6&1\\
	5&1&-10&1\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - 3R_1$
$R_3 \leftarrow R_3 -5R_1$
$R_2 \leftarrow \frac{1}{17}R_2$
$R_1 \leftarrow R_1 + 5R_2$
$R_3 \leftarrow R_3 - 26R_2$
$$\begin{pmatrix}
	1&0&-2&1\\
	0&1&0&-1\\
	0&0&0&-3\\
	\end{pmatrix}$$
$0 \neq -3$
$\therefore$ the system is incosistent

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2
$$\begin{pmatrix}
	5&-2&6&0\\
	-2&1&3&1\\
	\end{pmatrix}$$
$R_1 \leftarrow R_1 + 2R_2$
$$\begin{pmatrix}
	1&0&12&2\\
	-2&1&3&1\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 + 2R_1$
$$\begin{pmatrix}
	1&0&12&2\\
	0&1&27&5\\
	\end{pmatrix}$$
$z = t_1$
$y = 5 - 27t$
$x= 2- 12t$

It is in the form of a line as there is one linear paramater and both x and y are linear equations
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3$$
\begin{pmatrix}
i&-(i+1)&i\\
1&-2&2-i\\
\end{pmatrix}$$
$R_2 \leftarrow R_2 - iR_1$
$$\begin{pmatrix}
	i&-(i+1)&i\\
	0&-(i+1)&1-i\\
	\end{pmatrix}$$

$R_2 \leftarrow \frac{1}{i+1} R_2$
$$\begin{pmatrix}
	i&-(i+1)&i\\
	0&-1&\frac{1-i}{i+1}\\
	\end{pmatrix}$$
$$\begin{pmatrix}
	i&-(i+1)&i\\
	0&-1&-i\\
	\end{pmatrix}$$
$R_2 \leftarrow -R_2$
$$\begin{pmatrix}
	i&-(i+1)&i\\
	0&1&i\\
	\end{pmatrix}$$
$R_1 \leftarrow -iR_1$
$$\begin{pmatrix}
	1&i-1&1\\
	0&1&i\\
	\end{pmatrix}$$
$R_1 \leftarrow R_1 - (i-1)R_2$
$$\begin{pmatrix}
	1&0&2+ i\\
	0&1&i\\
	\end{pmatrix}$$
$x = 2+i, y = i$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4
(a)
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	2&-3&k^2-8&k-2\\
	\end{pmatrix}$$
to have multiple solutions there must be a redundant equation, to make this redundant equation we do the following row operation $R_3 \leftarrow R_3 - R_1$ giving
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	0&0&k^2-11&k+2\\
	\end{pmatrix}$$
solving for the values of  k such that the whole row is zero gives the system of equations 
$k^2 - 11 = 5$
$k+2 = -2$

$k^2 - 11 = 5$
$k = \pm 4$

$k+2 = -2$
$k = -4$

with a common solution of $k = -4$

$\therefore k = -4$ gives multiple equations,
$k=4$ is the extraneous root of this system thus giving no solutions,
Any other k should give a unique solution

(I)
$k \neq -4, 4$
(II)
$k = 4$
(III)
$k=-4$


(b)
(I)
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	2&-3&k^2-8&k-2\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - 3R_1$
$R_3 \leftarrow R_3 - 2R_1$
$$\begin{pmatrix}
	1&2&-3&4\\
	0&-7&14&-14\\
	0&-7&k^2-2&k-10\\
	\end{pmatrix}$$
$R_2 \leftarrow -\frac17 R_2$
$$\begin{pmatrix}
	1&2&-3&4\\
	0&1&-2&2\\
	0&-7&k^2-2&k-10\\
	\end{pmatrix}$$
$R_3 \leftarrow R_3 + 7R_2$
$R_1 \leftarrow R_1 - 2R_2$
$R_3 \leftarrow \frac{1}{k^2-16}R_3$
$$\begin{pmatrix}
	1&0&1&0\\
	0&1&-2&2\\
	0&0&1&\frac{1}{k-4}\\
	\end{pmatrix}$$

$R_2 \leftarrow R_2 + 2R_3$
$R_1 \leftarrow R_1 - R_3$
$$\begin{pmatrix}
	1&0&0&-\frac{1}{k-4}\\
	0&1&0&2 + \frac{2}{k-4}\\
	0&0&1&\frac{1}{k-4}\\
	\end{pmatrix}$$
$x=-\frac{1}{k-4},\quad y = 2 + \frac{2}{k-4},\quad z= \frac{1}{k-4}$

(III)
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	2&-3&k^2-8&k-2\\
	\end{pmatrix}$$
Substituting $k =-4$
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	2&-3&8&-6\\
	\end{pmatrix}$$
$R_3 \leftarrow R_3 + R_1$
$R_3 \leftarrow R_3 - R_2$
$$\begin{pmatrix}
	1&2&-3&4\\
	3&-1&5&-2\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_2 \leftarrow R_2 - 3R_1$
$R_2 \leftarrow -\frac17 R_2$
$$\begin{pmatrix}
	1&2&-3&4\\
	0&1&-2&-2\\
	0&0&0&0\\
	\end{pmatrix}$$
$R_1 \leftarrow R_1 - 2R_2$
$$\begin{pmatrix}
	1&0&1&0\\
	0&1&-2&-2\\
	0&0&0&0\\
	\end{pmatrix}$$
$z = t$
$y = 2t-2$
$x = -t$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5
$$(A-B)(C-A+2I_n) + (C-B+0_{nxn})(A-C) + (C-A)^2$$
$$(AC-A^2 + 2A -BC +BA -2B) + (C-B)(A-C) + (C-A)(C-A)$$
$$(AC-A^2 + 2A -BC +BA -2B) + (CA-C^2-BA +BC) + (C^2 -CA -AC + A^2)$$
$$AC-A^2+2A -BC +BA -2B + CA-C^2-BA +BC + C^2 -CA -AC + A^2$$
$$2A -2B$$
$$2(A-B)$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6
$$Aw =b$$
Substituting in w	$$A(\frac{3p+q}{4}+5u-7v)= b$$
$$\frac14 (3Ap+Aq) +5Au-7Av= b$$Substituting in the given equations $Ap, Aq = b$ and $Au, Av = 0$
$$\frac14 (3b+b) +5(0)-7(0)= b$$	$$\frac14 (4b)= b$$
$$b= b$$
$\therefore w = \frac{3p+q}{4}+5u-7v$ is a solution to $Aw=b$ 
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

7
(a)
$A_{1,2} = -3$
$A_{2,1} = 0$
$A_{3, 3} = DNE$

(b)
$A = (2,3)$
$B = (3,2)$
$C = (2,2)$
$D = (2,2)$
$E = (2,1)$
$F = (1,2)$

(c)
$A-A = \begin{pmatrix}0&0&0\\0&0&0\\\end{pmatrix}$
$A+2B = DNE$
$A+2B^T = \begin{pmatrix}0&-3&2\\0&1&3\\\end{pmatrix} + 2\begin{pmatrix}2&1&3\\-2&-1&-3\\\end{pmatrix}$
$$\Rightarrow \begin{pmatrix}0&-3&2\\0&1&3\\\end{pmatrix} + \begin{pmatrix}4&2&6\\-4&-2&-6\\\end{pmatrix}$$
$$\Rightarrow \begin{pmatrix}4&-1&8\\-4&-1&-3\\\end{pmatrix}$$
$D+0E = D + 0_{2,1} = DNE$
$A^2 = DNE$
$AB =\begin{pmatrix}0&-3&2\\0&1&3\\\end{pmatrix}\begin{pmatrix}2&-2\\1&-1\\3&-3\end{pmatrix}$
$$\Rightarrow\begin{pmatrix}0(2) - 3(1) +2(3)&0(-2) - 3(-1) +2(-3)\\
0(2) + 1(1) +3(3)&0(-2) + 1(-1) +3(-3)\\\end{pmatrix}$$
$$\Rightarrow\begin{pmatrix}3&-3\\
10&-10\\\end{pmatrix}$$

$BA=\begin{pmatrix}2&-2\\1&-1\\3&-3\end{pmatrix}\begin{pmatrix}0&-3&2\\0&1&3\\\end{pmatrix}$
$$\Rightarrow\begin{pmatrix}
2(0) -2(0)&2(-3) -2(1)&2(2) -2(3)\\
1(0) -1(0)&1(-3) -1(1)&1(2) -1(3)\\
3(0) -3(0)&3(-3) -3(1)&3(2) -3(3)\\
\end{pmatrix}$$
$$\Rightarrow\begin{pmatrix}
0&-8&-2\\
0&-4&-1\\
0&-12&-3\\
\end{pmatrix}$$
$AC = DNE$
$A^TC = \begin{pmatrix}0&0\\-3&1\\2&3\end{pmatrix} \begin{pmatrix}0&2\\0&0\\\end{pmatrix}$
$$\Rightarrow \begin{pmatrix}0&0\\0&-6\\ 0&4\end{pmatrix}$$
$BD = \begin{pmatrix}2&-2\\1&-1\\3&-3\end{pmatrix} \begin{pmatrix}0&2\\1&3\\\end{pmatrix}$
$$\Rightarrow \begin{pmatrix}2(0) -2(1)&2(2) -2(3)\\1(0) - 1(1)& 1(2) - 1(3) \\ 3(0) - 3(1)&3(2) -3(3)\end{pmatrix}$$
$$\Rightarrow \begin{pmatrix}-2&-2\\-1&-1\\-3&-3\end{pmatrix}$$
$BF = DNE$
$FE  = \begin{pmatrix}1&1\end{pmatrix}\begin{pmatrix}-1 \\ -2\end{pmatrix} = (-3)$