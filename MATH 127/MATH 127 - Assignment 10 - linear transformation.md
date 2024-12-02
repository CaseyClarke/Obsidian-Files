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
	
	 $I_G \rightarrow I_H$:


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

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. 
	<br>(a)
	
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
	
	