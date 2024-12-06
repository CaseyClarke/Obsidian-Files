1. 
	<br>(a) 
	
	The domain is $P_2(\mathbb{F}_{17})$ and the codomain is $\mathbb{F}_{17}^2$
	
	(b)
	
	$Let \; u = ax^2 + bx + c \quad v = lx^2+mx+n \quad a,b,c,l,m,n,k \in \mathbb{F}_{17}$
	
	$T(u+v) \stackrel{?}{=} T(u) + T(v)$
	$T(ax^2 + bx + c + lx^2 + mx + n) \stackrel{?}{=} T(ax^2 + bx + c) + T(lx^2 + mx + n)$
	$T((a+l)x^2 + (b+m)x + (c + n)) \stackrel{?}{=} (2a+b, a-b) + (2l + m, l-m)$
	$(2(a+l) + (b+m), (a+l) - (b+m)) \stackrel{?}{=} (2a+b, a-b) + (2l + m, l-m)$
	$(2(a+l) + (b+m), (a+l) - (b+m)) \stackrel{?}{=} (2(a+l) + (b+m), (a+l) - (b+m))$
	$LHS = RHS$
	Vector addition is preserved
	
	$T(ku) \stackrel{?}{=} kT(u)$
	$T(akx^2 + bkx + ck) \stackrel{?}{=} k(2a +b, a-b)$
	$(2ak + bk, ak - bk) \stackrel{?}{=} k(2a +b, a-b)$
	$(2ak + bk, ak - bk) \stackrel{?}{=} (2ak + bk, ak - bk)$
	$LHS = RHS$
	Scalar multiplication is preserved
	
	$QED$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. 
	<br>$T(k(1,1)) \stackrel{?}{=} kT(1,1)$
	$T(k,k) \stackrel{?}{=} k(2,0)$
	$(2k^3, 0) \stackrel{?}{=} (2k,0)$
	$LHS \neq RHS$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. 
	<br>$T(-2,2,8,-3)= -1T(2,0,0,3) + 2T(0,1,4,0)$
	$T(-2,2,8,-3)= -1(1,2) + 2(0,6)$
	$T(-2,2,8,-3)= (-1,10)$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
	<br>$f$ preserves group multiplication by definition in the question
	
	Identity to Identity
	 $f(1_G) \stackrel{?}{=} 1_H$
	 $f(1_G \cdot 1_G) = f(1_G) \cdot f(1_G)$
	 $f(1_G) = f(1_G) \cdot f(1_G)$
	 $f(1_g)^{-1} f(1_g) = f(1_G)$
	 $f(1_G) = 1_H$
	
	Inverse to Inverse
	$f(g^{-1}) \stackrel{?}{=} f(g)^{-1}$
	$f(gg^{-1}) = f(g)f(g^{-1})$
	$f(1_G) = f(g)f(g^{-1})$
	$1_H = f(g)f(g^{-1})$
	$f(g)^{-1}1_H = f(g^{-1})$
	$f(g)^{-1} = f(g^{-1})$
	
	$QED$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. 
	<br>$Let \; p(x), q(x) \in P_2(\mathbb{R})$
	
	$T(p(x) + q(x)) \stackrel{?}{=} T(p(x)) + T(q(x))$
	$$\begin{pmatrix}   (p+q)(0)&0\\\frac{d}{dx}(p(1) + q(1))&\int_0^1(p(x) + q(x))dx\\ \end{pmatrix} \stackrel{?}{=} \begin{pmatrix}   p(0)&0\\\frac{d}{dx}p(1)&\int_0^1p(x)dx\\ \end{pmatrix} \begin{pmatrix}   q(0)&0\\\frac{d}{dx}q(1)&\int_0^1q(x)dx\\ \end{pmatrix}$$
	$$\displaylines{\text{Due to the respective properties of functions, derivatives, and integrals}\\\text{they can all be distributed over adddition}}$$
	$$\begin{pmatrix}   p(0) + q(0)&0+0\\\frac{d}{dx}p(1) + \frac{d}{dx}q(1)&\int_0^1p(x) + \int_0^1q(x)dx\\ \end{pmatrix} \stackrel{?}{=} \begin{pmatrix}   p(0)&0\\\frac{d}{dx}p(1)&\int_0^1p(x)dx\\ \end{pmatrix} \begin{pmatrix}   q(0)&0\\\frac{d}{dx}q(1)&\int_0^1q(x)dx\\ \end{pmatrix}$$
	$$\begin{pmatrix}   p(0)&0\\\frac{d}{dx}p(1)&\int_0^1p(x)dx\\ \end{pmatrix} \begin{pmatrix}   q(0)&0\\\frac{d}{dx}q(1)&\int_0^1q(x)dx\\ \end{pmatrix} \stackrel{?}{=} \begin{pmatrix}   p(0)&0\\\frac{d}{dx}p(1)&\int_0^1p(x)dx\\ \end{pmatrix} \begin{pmatrix}   q(0)&0\\\frac{d}{dx}q(1)&\int_0^1q(x)dx\\ \end{pmatrix}$$
	
	$LHS = RHS$
	Vector Addition is preserved
	
	$kT(p(x) \stackrel{?}{=} T(kp(x)$
	$$k\begin{pmatrix}   p(0)&0\\\frac{d}{dx}p(1)&\int_0^1p(x)dx\\ \end{pmatrix} \stackrel{?}{=} \begin{pmatrix}   kp(0)&0\\\frac{d}{dx}kp(1)&\int_0^1kp(x)dx\\ \end{pmatrix}$$
	$$\begin{pmatrix}   kp(0)&0\\k\frac{d}{dx}p(1)&k\int_0^1p(x)dx\\ \end{pmatrix} \stackrel{?}{=} \begin{pmatrix}   kp(0)&0\\k\frac{d}{dx}p(1)&k\int_0^1p(x)dx\\ \end{pmatrix}$$
	$LHS = RHS$
	Scalar multiplication is preserved
	$QED$
	
	It is one-to-one but not onto as the kernel is trivial and the 0 entry in the matrix immediately excludes a large part of the codomain
	
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. 
	<br>$Let \; p(x), q(x) \in Poly(\mathbb{F})$
	
	(a)
	
	$T(p(x) + q(x)) \stackrel{?}{=} T(p(x)) + T(q(x))$
	$x(p(x) + q(x)) \stackrel{?}{=} x(p(x)) + x(q(x))$
	$xp(x) + xq(x) \stackrel{?}{=} xp(x) + xq(x)$
	$LHS = RHS$
	
	$kT(p(x)) = T(kp(x))$
	$k(xp(x)) = x(kp(x))$
	$k(xp(x)) = k(xp(x))$
	$LHS = RHS$
	
	$QED$
	
	(b)
	
	$T(p(x)) = T(q(x)) \stackrel{?}{\implies} p(x) = q(x)$
	$T(p(x)) = T(q(x))$
	$xp(x) = xq(x)$
	$p(x)= q(x)$
	
	$\therefore$ T is one-to-one
	
	(c)
	
	$\text{For any } p(x) \in Poly(\mathbb{F}) \quad \exists \; q(x) \text{ Such That } T(p(x)) = q(x)$
	Counterexample:
	$q(x) = 1$
	$T(p(x)) = 1$
	$xp(x) = 1$
	$p(x) = \frac{1}{x}$ 
	But $\frac 1x$ is a rational function not a polynomial so there is no solution for the above equation  in $Poly(\mathbb{F})$
	
	$\therefore$ T is not onto

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

7. 
	<br>(a)
	
	$T : \mathbb{F}_{23}^6 \rightarrow \mathbb{F}_{23}^4$
	
	(b)
	
	 The standard matrix of T is A
	
	(c)
	
	$Im_B = \text{Column space of A} = \left( \begin{pmatrix} 1\\-1\\2\\-3\end{pmatrix}, \begin{pmatrix} -1\\1\\-3\\2\end{pmatrix}, \begin{pmatrix} 2\\2\\2\\0\end{pmatrix} \right)$
	
	(d)
	
	$x_6 = t$
	$x_5 = s$
	$x_4 = -s -2t$
	$x_3 = 3t$
	$x_2 = r$
	$x_1 = -2r + s + 5t$
	
	$\begin{pmatrix} -2r + s +5t\\ r\\ 3t\\-s -2t \\ s\\ t  \;\\\end{pmatrix} = t\begin{pmatrix} 5\\0\\3\\-2 \\0 \\ 1 \end{pmatrix} + s\begin{pmatrix} 1\\0\\0\\-1 \\1 \\ 0 \end{pmatrix} + r\begin{pmatrix} -2\\1\\0\\0 \\ 0\\ 0\end{pmatrix}$
	
	$Ker_B = Null_B = \left( \begin{pmatrix} 5\\0\\3\\-2 \\0 \\ 1 \end{pmatrix}, \begin{pmatrix} 1\\0\\0\\-1 \\1 \\ 0 \end{pmatrix}, \begin{pmatrix} -2\\1\\0\\0 \\ 0\\ 0\end{pmatrix} \right)$
	
	(e)
	
	The range = image of T is a 3-dimensional subspace of $\mathbb{F}_{23}^4$. The kernel of T is a 3-dimensional subspace of $\mathbb{F}_{23}^6$.

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

8. 
	<br>$Let \; u,v \in \mathbb{F}$
	
	Closure of vector addition:
	$T(u + v) = T(u) + T(v)$
	$u+v = u+v$
	$u+v \in s$
	
	Closure of scalar multiplication:
	$kT(u) = T(ku)$
	$ku = ku$
	$ku \in S$
	
	Zero vector:
	$T(0_v) = 0_v$
	$0_v \in S$
	
	$QED$
	