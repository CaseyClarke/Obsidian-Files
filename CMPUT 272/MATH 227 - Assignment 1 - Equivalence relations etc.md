1. 
	   <br>To show that $\vec{v} \sim \vec{v'}$ is an equivalence relation we need to show that it follows the 3 properties of an equivalence relation
	
	Reflexive Property:
		$T(\vec{v}) = T(\vec{v'}) \implies \vec{v} = \vec{v'}$
	Symmetric Property:
		$T(\vec{v}) = T(\vec{v'}) \implies \vec{v} = \vec{v'} \implies \vec{v'} = \vec{v}$
	Transitive Property
		$T(\vec{v}) = T(\vec{v'})$
		$T(\vec{v'}) = T(\vec{v''})$
		$T(\vec{v}) = T(\vec{v'}) = T(\vec{v''}) \implies T(\vec{v}) = T(\vec{v''})$
	$QED$

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

3. <br>(a)
	
	A vector space is isomorphic to another if their dimensions are equal
	$dim(V) = n$
	$dim(V \oplus V) = 2n$
	$dim(V) = dim(V \oplus V) \implies n = 2n$
	$n = 0$ is the only case in which this holds which shows that this is only true for the trivial vector space
	
	(b)
	
	A linear map is an isomorphism iff it is one to one and onto
	
	==Prove using odd and even arguments==
	
	(c)
	
	$Poly(\mathbb{F})$ is not finite dimensional

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
	
	==prove that this is a well defined bijection==
	
	(c)
	
	==idk man==

5. <br>(a)
	
	(i)
	
	Composition preserves linearity
	$(ST)(T^{-1}S^{-1}) = (T^{-1}S^{-1}) (ST) = 1_G$
	$(S(T(V))(T^{-1}(S^{-1}(V)) = (T^{-1}(S^{-1}(V))(S(T(V)) = 1_G$
	$(S(T(T^{-1}(S^{-1}(V))) = (S(T((T^{-1}(S^{-1}(V)))) = 1_G$
	$1_G = 1_G = 1_G$
	$\therefore$ It is closed as the properties of linearity and invertibility hold
	
	(ii)
	
	$(ST)R = S(TR)$
	$S(T(V)R = S(T(R(V)$
	$S(T(R(V) = S(T(R(V)$
	
	(iii)
	
	$I(V) = V$
	Which is trivially linear and is invertible as $I^{-1} = I$ 
	
	(iv)	
	
	Any element's has an inverse by definition