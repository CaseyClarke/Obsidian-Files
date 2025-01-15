1. <br>To show that $\vec{v} \sim \vec{v'}$ is an equivalence relation we need to show that it follows the 3 properties of an equivalence relation
	
	Reflexive Property:
		$T(\vec{v}) = T(\vec{v'}) \implies \vec{v} = \vec{v'}$
	Symmetric Property:
		$T(\vec{v}) = T(\vec{v'}) \implies \vec{v} = \vec{v'} \implies \vec{v'} = \vec{v}$
	Transitive Property
		$T(\vec{v}) = T(\vec{v'})$
		$T(\vec{v'}) = T(\vec{v''})$
		$T(\vec{v}) = T(\vec{v'}) = T(\vec{v''}) \implies T(\vec{v}) = T(\vec{v''})$
	$QED$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. <br>(a)
	
	We need to show that $\vec{u} \sim \vec{v} \implies f(\vec{u}) = f(\vec{v}) \quad \forall \; \vec{u}, \vec{v} \in \mathbb{C}^3/\sim$
	However this is not true for the example relation given in the question
	
	$\vec{u} = (-i, i + 1, i -1), \quad \vec{v} = (0,0,0)$ 
	$\vec{u} \sim \vec{v}$
	$f(\vec{u}) = (-i, i + 1)$
	$f(\vec{v}) = (0,0)$
	$(-i, i + 1) \neq (0,0)$
	
	$\therefore \; f$ is not well defined over $\mathbb{C}^3/\sim$
	
	(b)
	
	We need to show that $p(x) \sim q(x) \implies f(p(x)) = f(q(x)) \quad \forall \; p(x), q(x) \in \mathbb{Q}[x]/\sim$
	$\implies (2p(1) + 3p(2) - 5p(3)) = (2q(1) + 3q(2) - 5q(3)) \text{ and } (p(1) - p(-1)) = (q(1) - q(-1))$
	Given that $p(x) \sim q(x)$ we know that from the properties of derivatives $q(x) = p(x) + c$ for some rational value of c 
	
	$(2p(1) + 3p(2) - 5p(3)) = (2q(1) + 3q(2) - 5q(3))$:
	$(2p(1) + 3p(2) - 5p(3)) = (2(p(1) + c) + 3(p(2) + c) - 5(p(3) + c))$
	$(2p(1) + 3p(2) - 5p(3)) = (2p(1) + 2c + 3p(2) + 3c - 5p(3) + -5c)$
	$(2p(1) + 3p(2) - 5p(3)) = (2p(1) + 3p(2) - 5p(3))$
	$LHS = RHS$
	
	$(p(1) - p(-1)) = (q(1) - q(-1))$:
	$(p(1) - p(-1)) = (p(1) + c -(p(-1) + c)$
	$(p(1) - p(-1)) = (p(1) - p(-1))$
	$LHS = RHS$
	
	$\therefore f$ is well defined over $\mathbb{Q}[x]/\sim$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. <br>(a)
	
	A vector space is isomorphic to another if their dimensions are equal
	$dim(V) = n$
	$dim(V \oplus V) = 2n$
	$dim(V) = dim(V \oplus V) \implies n = 2n$
	$n = 0$ is the only case in which this holds which shows that this is only true for the trivial vector space
	
	(b)
	
	A linear map is an isomorphism iff it is one to one and onto
	
	T can be split up into to components, $p(x^2)$ and $xq(x^2)$ these can be represented as $x^{2k}$ and $x^{2x+1} \quad \forall \; k \in \mathbb{N}$  respectively 
	$x^{2k}$ can be used to represent any polynomial with only even degrees
	$x^{2k+1}$ can be used to represent any polynomial with only odd degrees
	Thus adding them together as such  $x^{2k} + x^{2k+1} = T(p(x), q(x)) = p(x^2) + xq(x^2)$ we can get polynomials with any degree meaning that the output space is $Poly(\mathbb{F})$ 
	
	(c)
	
	$Poly(\mathbb{F})$ is not finite dimensional

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. <br>(a)
	
	We need to show that this relation satisfies the 3 properties of an equivalence relation
	
	Reflexive:
	
	$g^{-1}g = 1_G \in H$ as $H$ must contain the identity if it is a subgroup
	
	Symmetric:
	
	$g \sim g' \implies g^{-1}g' \in H$
	$(g^{-1}g')^{-1} = g{'}^{-1}g \implies g{'}^{-1}g \in H$ since inverse is closed
	$\implies g' \sim g$
	
	Transitive:
	
	$g \sim g'$
	$g' \sim g''$
	$(g^{-1}g')(g{'}^{-1}g'') = g^{-1}g'' \in H$ since multiplication is closed
	$\implies g \sim g''$
	
	$\therefore$ This is a valid equivalence relation
	
	(b)
	
	==prove that this is well defined and invertible (onto and one to one)==
	
	(c)
	
	==idk man==

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. <br>(a)
	
	(i)
	
	Composition preserves linearity
	$(S \circ T)^{-1} = T^{-1} \circ S^{-1}$
	$(S \circ T)^{-1}(V) \circ  (T^{-1} \circ S^{-1})(V) = S(T(T^{-1}(S^{-1}(V)))) = V$
	$(T^{-1} \circ S^{-1})(V) \circ (S \circ T)^{-1}(V) = T^{-1}(S^{-1}(S(T(V)))) = V$
	$\therefore$ It is closed as the properties of linearity and invertibility hold
	
	(ii)
	
	$(S \circ T) \circ R = S \circ (T \circ R)$
	$S(T(V) \circ R = S \circ (T(R(V)$
	$S(T(R(V) = S(T(R(V)$
	
	(iii)
	
	$I(V) = V$
	Which is trivially linear and is invertible as $I^{-1} = I$ 
	
	(iv)	
	
	Any element has an inverse by definition and from the properties of function composition we know $(T \circ T^{-1})(V) = (T^{-1} \circ T)(V) = V = I(V) \quad \forall \; T \in IL(V)$
	
	(b)
	
	(i)
	
	From the previous question we know that function composition forms a group over $IL(V)$ so this is automatically satisfied as $f$ is just the composition of functions
	
	(ii)
	
	$f(T \circ T) = S \circ (T \circ T) \circ S^{-1}$
	$f(T) \circ f(T) = (S \circ T \circ S^{-1}) \circ (S \circ T \circ S^{-1})$
	$f(T) \circ f(T) = (S \circ T \circ T \circ S^{-1}) = S \circ (T \circ T) \circ S^{-1}$
	$f(T) \circ f(T) = f(T \circ T)$
	
	(iii)
	
	$f^{-1}(T) = S^{-1} \circ T \circ S$
	$f(T) \circ f^{-1}(T) = f^{-1}(T) \circ f(T) = T$
	
	Since $f$ is simply a string of function compositions it preserves the group structure meaning that (i), (ii), and (iii) are all automatically satisfied making it a homomorphism as well
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

6. <br>(a)
	
	$$[T(x^4)]_{\beta'} = \begin{pmatrix} 2\\1\\1\\0 \end{pmatrix}$$ 
	$$[T(x^3)]_{\beta'} = \begin{pmatrix} -2\\-1\\-1\\0 \end{pmatrix}$$ 
	$$[T(x^2)]_{\beta'} = \begin{pmatrix} -1\\-2\\-2\\1 \end{pmatrix}$$ 
	$$[T(x)]_{\beta'} = \begin{pmatrix} 0\\3\\0\\1 \end{pmatrix}$$ 
	$$[T(1)]_{\beta'} = \begin{pmatrix} 1\\-1\\-1\\1 \end{pmatrix}$$ 
	$$[T]_{\beta' \leftarrow \beta} = \begin{pmatrix} 2 & -2 & -1& 0 & 1\\1 & -1 & -2 & 3 & -1\\1 & -1 & -2 & 0 & -1\\0 & 0 & 1 & 1 & 1 \end{pmatrix} $$
	(b)
	
	$$[T(x^4 - x^3 + x)]_{\beta} = \begin{pmatrix} 1\\1\\0\\1\\0 \end{pmatrix}$$ 
	$$[T(x^4 - x^3 + x)]_{\beta'} = \begin{pmatrix} 0\\3\\0\\1\ \end{pmatrix}$$ 
	$$[T(x^4 - x^3 + x)]_{\beta'} = \begin{pmatrix} 2 & -2 & -1& 0 & 1\\1 & -1 & -2 & 3 & -1\\1 & -1 & -2 & 0 & -1\\0 & 0 & 1 & 1 & 1 \end{pmatrix}\begin{pmatrix} 1\\1\\0\\1\\0 \end{pmatrix} = \begin{pmatrix} 0\\3\\0\\1 \end{pmatrix}$$
	
	They both get the same answer so the formula holds

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

7. <br>(a)
	
	$$[T(x^2)]_{\beta} = \begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}$$
	$$[T(x)]_{\beta} = \begin{pmatrix} 0 \\ 2 \\ 0 \end{pmatrix}$$
	$$[T(1)]_{\beta} = \begin{pmatrix} 1 \\ 1 \\ -4 \end{pmatrix}$$
	$$[T]_{\beta \leftarrow \beta'} = \begin{pmatrix} 0 & 0 & 1 \\ 0 & 2 & 1 \\ 0 & 0 & -4 \end{pmatrix}$$
	$$[S(1,0,0)]_{\beta} = \begin{pmatrix} 1 \\ 1 \\ 0 \\ 1 \end{pmatrix}$$
	$$[S(0,1,0)]_{\beta} = \begin{pmatrix} 1 \\ 0 \\ 0 \\ 1 \end{pmatrix}$$
	$$[S(0,0,1)]_{\beta} = \begin{pmatrix} 0 \\ -1 \\ 2 \\ 1 \end{pmatrix}$$
	$$[S]_{\beta''\leftarrow \beta} = \begin{pmatrix} 1 & 1 & 0 \\ 1 & 0 & -1 \\ 0 & 0 & 2 \\ 1 & 1 & 1  \end{pmatrix} $$
	(b)
	
	$$[S \circ T]_{\beta'' \leftarrow \beta} = \begin{pmatrix} 1 & 1 & 0 \\ 1 & 0 & -1 \\ 0 & 0 & 2 \\ 1 & 1 & 1  \end{pmatrix}\begin{pmatrix} 0 & 0 & 1 \\ 0 & 2 & 1 \\ 0 & 0 & -4 \end{pmatrix} = \begin{pmatrix} 0 & 2 & 2 \\ 0 & 0 & 5 \\ 0 & 0 & -8 \\ 0 & 2 & -2  \end{pmatrix}$$