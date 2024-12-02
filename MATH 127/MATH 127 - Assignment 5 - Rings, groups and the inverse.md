1. 
	(a)
	
	To show that $R^S$ forms a ring we need to prove each individual axiom
	
	$Let \; f(s), g(s), h(s) \in R^S$
	
	The following properties hold as the functions $S \rightarrow R$ inherit the properties of a ring as by definition the outputs are in R 
	
	Closure under Multiplication
	$(fg)(s) = f(s)g(s)$
	
	Closure under Addition
	$(f+g)(s) = f(s)+g(s)$
	
	Associativity of Multiplication
	$f(s)(g(s)h(s)) = (f(s)g(s))h(s)$
	$\Rightarrow f(s)((gh)(s)) = ((fg)(s))h(s)$
	$\Rightarrow (fgh)(s) = (fgh)(s)$
	
	Associativity of Addition
	$f(s) + (g(s) + h(s)) = (f(s) + g(s)) + h(s)$
	$\Rightarrow f(s) + ((g+h)(s)) = ((f+g)(s)) + h(s)$
	$\Rightarrow  (f+ g+h)(s) = (f+ g+h)(s)$
	
	Distributivity
	$f(s)(g(s)+h(s)) = f(s)g(s) + f(s)h(s)$
	$\Rightarrow f(s)(g+h)(s) = (fg)(s) + (fh)(s)$
	$\Rightarrow (f(g+h))(s) = (fg+fh)(s)$
	$\Rightarrow (f(g+h))(s) = (f(g+h))(s)$
	
	Commutativity of addition
	$f(s) + g(s) = g(s) + f(s)$
	$\Rightarrow (f+g)(s) = (g+f)(s)$
	$\Rightarrow (f+g)(s) = (f+g)(s)$
	
	Additive Identity
	$\exists \; 0(s) = 0_R \in R^S \text{ Such That } f(s) + 0(s) = f(s) \quad$
	where $0_R$ is the additive identity of the given ring
	 $f(s) + 0(s) = f(s)$
	$\Rightarrow (f+0)(s) = f(s)$
	$\Rightarrow f(s) = f(s)$
	
	Multiplicative identity
	$\exists \; 1(s) = 1_R \in R^S \text{ Such That } f(s)1(s) = f(s) = 1(s)f(s)$
	where $1_R$ is the multiplicative identity of the given ring
	$f(s)1(s) = f(s) = 1(s)f(s)$
	$\Rightarrow (f+1)(s) = f(s) = (1+f)(s)$
	$\Rightarrow f(s) = f(s) = f(s)$
	
	Additive Inverse
	$\exists \; -l(s) \in R^S \text{ Such That } l(s) + -l(s) = 0(s) \quad \forall l(s) \in R^S$
	$l(s) + -l(s) = 0(s)$
	$\Rightarrow (l-l)(s) = 0(s)$
	$\Rightarrow 0(s) = 0(s)$
	
	(b)
	
	We want to show that $\mathbb{Z}^\mathbb{Z}$ does not form a ring. Assume that it is a ring, the following is a counter example
	
	$f(n) = (n+1)^2$
	$g(n) = n+1$
	$h(n) = n$
	
	Axiom of Distributivity:
	$f(n)\left( g(n)+h(n)\right) = f(n)g(n) + f(n)h(n)$
	
	LHS:
	$f(n)\left( g(n)+h(n)\right)$
	$\Rightarrow f(n)\left( 2n+1\right)$
	$\Rightarrow (2n+2)^2$
	
	RHS:
	$f(n)g(n) + f(n)h(n)$
	$\Rightarrow ((n+2)^2 + (n+1)^2)$
	
	$LHS \neq RHS$
	$\therefore \text{ The opposite of our original assumption must be true so } \mathbb{Z}^\mathbb{Z} \text{ is not a ring}$
	$QED$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
2. 
	(a)
	
	$A$ is diagonal which means it is also both upper and lower triangular
	$B$ is upper triangular
	$C$ is not any of these identities
	$D$ is lower triangular
	
	(b)
	$$A = \begin{pmatrix}
	1&0&0\\
	0&-2&0\\
	0&0&-1\\
	\end{pmatrix}$$
	$$A^{-1} = \begin{pmatrix}
	1&0&0\\
	0&-9&0\\
	0&0&-1\\
	\end{pmatrix}$$
	$B$ is not invertible as its RREF has a row of 0s and is inconsistent. Alternatively $det(B)= 0$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. 
	(a)
	$$\begin{pmatrix}
	3&7\\
	2&5\\
	\end{pmatrix}
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	3\\
	1\\
	\end{pmatrix}
	$$

	$$\begin{pmatrix}
	2&7&1&5\\
	1&4&-1&-3\\
	6&3&0&1\\
	\end{pmatrix}
	\begin{pmatrix}
	a\\
	b\\
	c\\
	d\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	3\\
	1\\
	1\\
	\end{pmatrix}
	$$
	(b)
	$$\begin{pmatrix}
	3&7\\
	2&5\\
	\end{pmatrix}
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	3\\
	1\\
	\end{pmatrix}
	$$
	$ad-bc = 3(5) - 7(2) = 1$
	$$\begin{pmatrix}
	3&7\\
	2&5\\
	\end{pmatrix}^{-1} 
	= 
	\frac{1}{1}
	\begin{pmatrix}
	5&-7\\
	-2&3\\
	\end{pmatrix}
	= 
	\begin{pmatrix}
	5&-7\\
	-2&3\\
	\end{pmatrix}
	$$
	$$
	\begin{pmatrix}
	5&-7\\
	-2&3\\
	\end{pmatrix}
	\begin{pmatrix}
	3&7\\
	2&5\\
	\end{pmatrix}
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	5&-7\\
	-2&3\\
	\end{pmatrix}
	\begin{pmatrix}
	3\\
	1\\
	\end{pmatrix}
	$$
	$$
	\begin{pmatrix}
	1&0\\
	0&1\\
	\end{pmatrix}
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	5&-7\\
	-2&3\\
	\end{pmatrix}
	\begin{pmatrix}
	3\\
	1\\
	\end{pmatrix}
	$$
	$$
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	5(3) -7(1)\\
	-2(3) +3(1)\\
	\end{pmatrix}
	$$
	$$
	\begin{pmatrix}
	x_1\\
	x_2\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	8\\
	-3\\
	\end{pmatrix}
	$$
	
	$$\therefore \text{ The system of equations has a solution } x_1 = 8, x_2 = -3$$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
	We need to prove that the orthogonal matrices form a group, we do this by proving the group axioms as follows, $\text{ Let G be the set of all orthogonal matrices } A \in M_{nxn}(\mathbb{F})$
	Closure
		$\exists \; A,B \in G \text{ Such That } (AB)(AB)^T = I_n = (AB)^T(AB)$
		$(AB)(AB)^T = I_n = (AB)^T(AB)$
		$\Rightarrow (AB)B^TA^T = I_n = B^TA^T(AB)$
		$\Rightarrow A(BB^T)A^T = I_n = B^T(A^TA)B$
		$\Rightarrow AA^T = I_n = B^TB$
		$\Rightarrow I_n = I_n = I_n$
		$QED$
	Associativity
		$\exists \; A,B,C \in G \text{ Such That } A(BC) = (AB)C$
		$\Rightarrow A(BC) = (AB)C$
		$\Rightarrow A^{T}A(BC) = A^{T}(AB)C$
		$\Rightarrow BC= A^{T}(AB)C$
		$\Rightarrow BCC^{T}= A^{T}(AB)CC^{T}$
		$\Rightarrow B= A^{T}(AB)$
		$\Rightarrow AB= AA^{T}(AB)$
		$\Rightarrow AB= AB$
		$LHS = RHS$
		$QED$
	Inverse
		$\exists \; A \in G \text{ Such That } AA^{-1} = I_n$
		$AA^{-1} = I_n =AA^{T}$
		$A^{-1} = A^T$
		Every element in G has a transpose by definition and that transpose is exactly equal to the inverse and the inverse/transpose of any element in G also lies in G as
		$A^{T}(A^{T})^{T} = I_n = (A^{T})^{T}A^{T}$
		$\Rightarrow A^{T}A = I_n = AA^{T}$
		$\Rightarrow I_n= I_n = I_n$
		$\therefore \text{ Every element in G has an inverse and that inverse lies in G}$
		$QED$
	Identity
		$\exists \; I_n \in G \text{ Such That } AA^{-1} = I_n \quad  \forall \; A \in G$
		The identity matrix lies in G as it satisfies the equation
		$I_nI_n^{T} = I_n = I_n^{T}I_n$
		$\Rightarrow I_n= I_n = I_n$
		$QED$
	$\therefore \text{G forms a group as all of the group axioms hold}$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. 
	We need to prove that G forms a group, we do this by proving the group axioms as follows
	
	Closure
		$\exists \; a = x_a +iy_a, \; b = x_b +iy_b \in G \text{ Such That } ab  = x+iy \quad x,y \in \mathbb{R} \text{ Such That } x^2 + y^2  = 1$
		$ab = x+iy$
		$\Rightarrow (x_a+iy_a)(x_b+iy_b) = x+iy$
		$\Rightarrow x_ax_b +x_aiy_b + iy_ax_b -y_ay_b = x+iy$
		$\Rightarrow x_ax_b - y_ay_b +i(x_ay_b + y_ax_b)  = x+iy$
		$x = x_ax_b - y_ay_b$
		$y = x_ay_b + y_ax_b$
		$x^2 + y^2  = 1$
		$\Rightarrow (x_ax_b - y_ay_b)^2 + (x_ay_b + y_ax_b)^2 = 1$
		$\Rightarrow x_a^2x_b^2-2x_ax_by_ay_b + y_a^2y_b^2 + x_a^2y_b^2 + 2x_ax_by_ay_b + y_a^2x_b^2  = 1$
		$\Rightarrow x_a^2x_b^2 + y_a^2y_b^2 + x_a^2y_b^2 + y_a^2x_b^2  = 1$
		$\Rightarrow x_a^2(x_b^2 + y_b^2) + y_a^2(x_b^2 + y_b^2)  = 1$
		Recall that $x_b^2 + y_b^2 = 1$
		$\Rightarrow x_a^2 + y_a^2  = 1$
		$\therefore ab \in G \text{ as it is in the form } x+iy \text{ and satisfies the equation } x^2 +y^2 = 1$
		$QED$
	Associativity
		Complex number multiplication with coefficients in $\mathbb{R}$ is always associative so it is automatically satisfied
	Identity
		$\exists 1+0i \in G \text{ Such That } a(1+0i) = a \quad \forall a \in G$
		$a(1+0i) = a$
		$\Rightarrow a(1+0i) = a$
		$\Rightarrow a + 0ia= a$
		$\Rightarrow a = a$
		$QED$
	Inverse
		$\exists \; \overline{a} \in G \text{ Such That } a\overline{a} = 1 \quad \forall a \in G$
		$let \; a = x+yi, \quad \overline{a} = x-yi$
		$a\overline{a} = 1$
		$\Rightarrow (x+yi)(x-yi) = 1$
		$\Rightarrow x^2 + y^2 = 1$
		By the definition of $G$ the above equation is true		
		$QED$
	$\therefore \text{G forms a group as all of the group axioms hold}$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. 
	To find the elementary matrix we start by finding the elementary row operations that transform the left matrix to be equal to the right matrix 
	$$\begin{pmatrix}
	1&1&-3&4\\
	0&2&-1&1\\
	3&5&-4&1\\
	\end{pmatrix}$$
	$$R_2 \leftarrow R_2 + 2R_1$$
	$$\begin{pmatrix}
	1&1&-3&4\\
	2&4&-7&9\\
	3&5&-4&1\\
	\end{pmatrix}$$
	Then we apply the exact same operations to an identity matrix of the correct size
	$$\begin{pmatrix}
	1&0&0\\
	0&1&0\\
	0&0&1\\
	\end{pmatrix}$$
	$$R_2 \leftarrow R_2 + 2R1$$
	$$\begin{pmatrix}
	1&0&0\\
	2&1&0\\
	0&0&1\\
	\end{pmatrix}$$
	$$\text{ Substituing in our proposed E into the original equation}$$
	$$\begin{pmatrix}
	1&0&0\\
	2&1&0\\
	0&0&1\\
	\end{pmatrix}\begin{pmatrix}
	1&1&-3&4\\
	0&2&-1&1\\
	3&5&-4&1\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	1&1&-3&4\\
	2&4&-7&9\\
	3&5&-4&1\\
	\end{pmatrix}
	$$
	$$
	\begin{pmatrix}
	1&1&-3&4\\
	2&4&-7&9\\
	3&5&-4&1\\
	\end{pmatrix}
	=
	\begin{pmatrix}
	1&1&-3&4\\
	2&4&-7&9\\
	3&5&-4&1\\
	\end{pmatrix}
	$$
	$$\therefore E = \begin{pmatrix}
	1&0&0\\
	2&1&0\\
	0&0&1\\
	\end{pmatrix}$$