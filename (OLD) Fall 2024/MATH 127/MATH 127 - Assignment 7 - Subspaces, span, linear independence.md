1. 
	<br>(a)
	$Let \; R = M_{2x2}(\mathbb{Z})$
	$Let \; S \subset R \text{ Such That } tr(s) = 0 \; \forall s \in S$
	
	To check if something is a subring we have to check that both operations are closed and that both identities are in the subset.
	
	Identity matrix:
	$1_R \in S$
	$1_R =\begin{vmatrix}1&0\\0&1\end{vmatrix}$
	$tr(1_R) = 2 \implies 1_R \notin S$
	$\therefore S$ is not a subring 
	
	(b)
	
	$Let \; R = M_{2x2}(\mathbb{Z})$
	$Let \; S \subset R \text{ Such That } s_{2, 1} = 0 \; \forall s \in S$
	$Let \; A = \begin{vmatrix}a&b\\0&d\end{vmatrix}$
	$Let \; B = \begin{vmatrix}u&v\\0&w\end{vmatrix}$
	
	To check if something is a subring we have to check that both operations are closed and that both identities are in the subset.
	
	Closure of Addition
	$A+B \in S$
	$A+B = \begin{vmatrix}a+u&b+v\\0+0&w+d\end{vmatrix}$
	$(A+B)_{2,1} = 0 \implies A+B \in S$
	
	Closure of Multiplication:
	$AB \in S$
	$AB = \begin{vmatrix}au + b0&av+ bw\\0u + d0&0v + dw\end{vmatrix}$
	$AB_{2,1} = 0 \implies AB \in S$ 
	
	Identity matrix:
	$1_R \in S$
	$1_R =\begin{vmatrix}1&0\\0&1\end{vmatrix}$
	$1_{R_{2,1}} = 0 \implies 1_R \in S$
	
	Zero matrix:
	$0_R \in S$
	$0_R =\begin{vmatrix}0&0\\0&0\end{vmatrix}$
	$1_{R_{2,1}} = 0 \implies 1_R \in S$
	
	$\therefore S$ is a subring
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
	
2. 
	<br>(a)
	$$\left((0,0), 0x^2 +0x + 0, \; \begin{pmatrix}0&0&0\\0&0&0\end{pmatrix}\right)$$
	(b)
	$$
	\left(2, \; \begin{pmatrix}i&0\\0&-2i\end{pmatrix}\right)^{-1} = 
	\left(-2, \; \begin{pmatrix}i&0\\0&-2i\end{pmatrix}^{-1}\right)
	$$
	$$\left[
	\begin{array}{cc|cc}
	1&0&i&0\\
	0&1&0&-2i\\
	\end{array}
	\right]$$
	$R_1 \leftarrow -iR_1$
	$R_2 \leftarrow \frac{i}{2}R_2$
	$$\left[
		\begin{array}{cc|cc}
		-i&0&1&0\\
		0&\frac{i}{2}&0&1\\
		\end{array}
	\right]$$
	$$
	\left(2, \; \begin{pmatrix}i&0\\0&-2i\end{pmatrix}\right)^{-1} = 
	\left(-2, \; \begin{pmatrix}-i&0\\0&\frac{i}{2}\end{pmatrix}\right)
	$$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
	
3. 
	<br>(a)
	Any Subspace must contain the zero vector of the superspace 
	$0_{R^3} = (0,0,0)$
	$(x, y, 2x +y -1)$
	$\Rightarrow (0, 0, 2x +y -1)$
	$\Rightarrow (0, 0, -1)$
	$(0,0,0) \neq (0,0,-1)$
	$\therefore$ it is not a subspace
	
	(b)
	$Let \; A = (1, 1, \sqrt{1^2+1^2}) = (1, 1, \sqrt{2})$
	The elements of the subspace must be closed under scalar multiplication
	$-1A = -1(1,1,\sqrt{2}) = (-1,-1,-\sqrt{2})$
	The 3rd term of this vector is negative which cannot happen in the general term as there is a square root therefore this does not form a subspace
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
	<br>$Let \; A = (a,b, 5a- 2b, a+b) \in S$
	$Let \; B = (c,d, 5c- 2d, c+d) \in S$
	$Let \; z,c_1,c_2 \in \mathbb{F}_{17}$
	
	(a)
	
	Zero Vector:
	$0_{\mathbb{F}^4_{17}} \in S$
	$(0,0,0,0) \in S$
	$(0,0, 5x-2y, x+y)$
	$\Rightarrow (0,0, 5(0)-2(0), 0+0)$
	$\Rightarrow (0,0,0,0)\implies \in S$
	
	Closure of Addition:
	$A+B \in S$
	$(a+c,b+d,5a-2b + 5c-2d, a+b+c+d)$
	$\Rightarrow ((a+c),(b+d),5(a+c)-2(b+d), (a+c)+(b+d))$
	 $Let\;  e = a+c \quad f = b+d$
	 $\Rightarrow (e,f,5e-2f, e+f) \implies \in S$
	
	Closure of Multiplication:
	$zA \in S$
	$(az, bz, z(5a-2b), z(a+b))$
	$\Rightarrow (az, bz, z5a-z2b, za+zb)$
	$Let \; u = az \; v = bz$
	$\Rightarrow (u, v, 5u-2v, u+v) \implies \in S$
	
	(b)
	Separating V into x and y components by finding the vectors $x = 0, \; y =y$ and $x = x, \; y =0$
	$V = (x,0,5x,x) + (0,y,-2y,y)$
	$V = x(1,0,5,1) + y(0,1,-2,1)$
	This is a linear combination with scalars $x,y$ which means we can write it as a span
	$span((1,0,5,1), (0,1,-2,1)) = V$
	Since the span is always a subspace V is a subspace
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
	
5. 
	<br>$(1,2,3) = 9(1,1,1) -9(-1,-3,-5)$
	$\Rightarrow (1,2,3) = (9,9,9) + (9, 27, 45)$
	$\Rightarrow (1,2,3) = (18, 36, 54)$
	Given that we are working in $mod \; 17$
	$\Rightarrow (1,2,3) = (1,2,3)$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. 
	<br>(a)
	$a(2,2,1) + b(k, 2, 4) = (3,0,1)$
	$\Rightarrow (a2,a2,a1) + (bk, b2, b4) = (3,0,1)$
	$\Rightarrow (2a + bk,2a + 2b,a + 4b) = (3,0,1)$
	$$\begin{pmatrix}
	2&k&3\\
	2&2&0\\
	1&4&1\\
	\end{pmatrix}$$
	Simplifying
	$$\begin{pmatrix}
	2&k&3\\
	0&2-k&-3\\
	1&4&1\\
	\end{pmatrix}$$
	
	If $k = 2$ then the matrix is inconsistent leading to no possibility of a linear combination
	$\therefore (3,0,1)$ cannot be made with a linear combination of  $(2,2,1) \text{ and } (2, 2, 4)$
	
	(b)
	$(3,0,1) = a(2,2,1) + b(k,2,-1)$
	$-1 \equiv 4 \; mod \; 5$
	$(3,0,1) = a(2,2,1) + b(k,2,4)$
	This is the same as part (a) meaning that this span does not contain $(3,0,1) \; \text{if} \; k = 2$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
7. 
	<br>$span((a, b), (b, c), (a, c)) = z_1(a,b) + z_2(b,c) + z_3(a,c)$
	Since we are working in $mod \; 2$ we only have to worry about the scalars being 0 or 1 
	$(a,b) + (b,c) + (a,c) = \varnothing$
	$(a,b) + (b,c) = (a,c)$
	$(b,c) + (a,c) = (a,b)$
	$(a,b) + (a,c) = (b,c)$
	
	$\therefore \; \text{ this span contains the 4 folowing vectors } \varnothing, (a,c), (a,b), (b,c)$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

8. 
	<br>To check for linear dependence we check if the linear combination of the vectors equaling zero has a non trivial solution
	
	(a)
	$c_1(2,-3,-1,k) + c_2(1,0,1,0) + c_3(0,1,1,1) = (0,0,0,0)$
	$$\begin{pmatrix}
	1&0&2&0\\
	0&1&-3&0\\
	1&1&-1&0\\
	0&1&k&0
	\end{pmatrix}$$
	Simplifying
	$$\begin{pmatrix}
	1&0&2&0\\
	0&1&-3&0\\
	0&0&0&0\\
	0&0&k+3&0
	\end{pmatrix}$$
	The only way that this system has a non trivial solution is if $k \equiv -3$
	$c_1 = 2 \; c_2 = -3$
	$\therefore$ these vectors are dependant if $k \equiv -3$
	 $(2,-3,-1,-3) = 2(1,0,1,0) + -3(0,1,1,1)$
	$(2,-3,-1,-3) = (2,0,2,0) + (0,-3,-3,-3)$
	$(2,-3,-1,-3) = (2,-3,-1,-3)$
	
	(b)
	$c_1(−1, 2, k, 1) + c_2(1, 1, 1, 2) + c_3(1, −1, 2, 0) = (0,0,0,0)$
	
	$$\begin{pmatrix}
	1&1&-1&0\\
	1&-1&2&0\\
	1&2&k&0\\
	2&0&1&0
	\end{pmatrix}$$
	Simplifying
	$$\begin{pmatrix}
	1&1&-1&0\\
	1&-1&2&0\\
	0&0&k+11&0\\
	0&0&0&0
	\end{pmatrix}$$
	The only way that this system has a non trivial solution is if $k \equiv -11$
	$\therefore$ these vectors are dependant if $k \equiv -11$
	$(−1, 2, -11, 1) = 9(1, 1, 1, 2) + 7(1, −1, 2, 0)$
	$(−1, 2, -11, 1) = (9, 9, 9, 18) + (7, −7, 14, 0)$
	$(−1, 2, -11, 1) = (−1, 2, -11, 1)$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

9. 
	<br>To show linear independence we show that the linear combination of the vectors has only one solution $a_1, a_2, \dots a_n = b_1, b_2, \dots b_n = 0$
	$a_1(v_1,0_w) + a_2(v_2,0_w) + \dots + a_n(v_n,0_w) + b_1(0_v, w_1) + b_2(0_v, w_w) + \dots + b_n(0_v, w_n) = (0_v,0_w)$
	Because this is a direct sum we can split this into components
	$a_1v_1 + a_2v_2 + \dots + a_nv_n + b_10_v + b_20_v + \dots + b_n0_v = 0_v$
	$b_1w_1 + b_2w_2 + \dots + b_nw_n + a_10_w + a_20_w + \dots + a_n0_w = 0_w$
	The zero terms cancel out giving
	$a_1v_1 + a_2v_2 + \dots + a_nv_n = 0_v$
	$b_1w_1 + b_2w_2 + \dots + b_nw_n = 0_w$
	These equations are the definition for linear combinations for the vectors $v_n$ and $w_n$ respectively, because we know that both of these sets of vectors are linearly independent we know that $a_1, a_2, \dots a_n = 0$ and $b_1, b_2, \dots b_n = 0$ 
	Thus we have shown that the only solution to the direct sum linear combination equation is $a_1, a_2, \dots a_n = b_1, b_2, \dots b_n = 0$, which by definition means that the vectors are linearly independent
	