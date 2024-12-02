1. 
	 (a)  $-9 - 24i$
	 (b)  $-15 + 15i$
	 (c)  $0 - i$
	 (d) $-46 -9i$
	 (e) $\frac{13}{29} - \frac{11}{29}i$
	 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
2. 
	 Let $A = a+bi \quad a,b \in \mathbb{R}, \quad A \in \mathbb{C}$
	 Let $B = c+di \quad c,d \in \mathbb{R}, \quad B \in \mathbb{C}$
	 Let $C = e+fi \quad e,f \in \mathbb{R}, \quad C \in \mathbb{C}$
	 
	 We are trying to prove that $A(B+C)= AB+ AC$
	 The LHS of the equation turns into
	 $\Rightarrow (a+bi)((c+di) + (e+fi))$
	 $\Rightarrow (a+bi)((c + e) + (d + f)i)$  
	 $\Rightarrow a(c+e) + ai(d + f) + bi(c + e) - b(d + f)$
	 $\Rightarrow (a(c+e) - b(d+f)) + i(a(d+f) + b(c+e))$

	 The RHS of the equation turns into 
	 $\Rightarrow (a+bi)(c+di) + (a+bi)(e+fi)$
	 $\Rightarrow (ac + adi + bci - bd) + (ae + afi + ebi - bf)$
	 $\Rightarrow (ac - bd) + i(ad + bc) + (ae - bf) + i(af + eb)$
	 $\Rightarrow (ac - bd + ae - bf) + i(ad + bc + af + be)$
	 $\Rightarrow (a(c+e) -b(d+f)) + i(a(d+f) + b(c+e))$
	 
	 LHS = RHS
	 QED
	 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
3. 
	 Let $A = (a, b)  \quad A \in F$
	 $\exists (0,0)$ Such that $A + (0, 0) = A$
	 $\Rightarrow (a,b) + (0, 0) = (a,b)$
	 $\Rightarrow (a+0,b+0) = (a,b)$
	 $\Rightarrow (a,b) = (a,b)$
	 $\therefore (0,0)$ is the additive identity

	$\exists (1,1)$ Such that $A \times (1,1) = A$
	 $\Rightarrow (a,b)(1,1) = (a,b)$
	 $\Rightarrow (1a,1b) = (a,b)$
	 $\Rightarrow (a,b) = (a,b)$
	 $\therefore (1,1)$ is the multiplicative identity
	 
	 We are trying to prove that $F$ is not a field, we suggest the following counter example to $F$ being a field
	 
	 Let $B = (1, 0)  \quad B \in F$
	 The axiom of multiplicative inverse states that 
	 $BB^{-1} = (1,1)$ if $B \neq (0,0)$

	 The LHS of the equation turns into
	 $(1,0)(a,b)$ where $(a,b) = B^{-1}\quad a,b \in \mathbb{R}$
	 simplifying down to 
	 $\Rightarrow (a, 0)$

	 $(a,0) \neq (1,1) \quad \forall b \in \mathbb{R}$
	 $LHS \neq RHS$
	 QED
	 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
4. 
	 (a)
		 $\exists  (0,0)$ Such that $(a,b) + (0,0) = (a,b), \quad (a,b) \in F$
		 $\Rightarrow (a+0,b+0) = (a,b)$
		 $\Rightarrow (a,b) = (a,b)$
		 $\therefore$ the additive identity for F is $(0,0)$
	 (b)
		 $\exists (1,0)$ Such that $(a,b)(1,0) = (a,b), \quad (a,b) \in F$
		 $\Rightarrow (1a - 0b, 0a + 1b) = (a,b)$
		 $\Rightarrow (a,b) = (a,b)$
		  $\therefore$ the multiplicative identity for F is $(1,0)$
	 (c)
		 Let $A = (a,b), \quad a,b \in \mathbb{Q}, \quad A \in F$
		 $AA^{-1} = (1,0)$ if $A \neq (0,0)$
		 $\Rightarrow (a,b)(\frac{a}{a^2+b^2}, \frac{-b}{a^2+b^2}) = (1,0)$, $A \neq (0,0)$
		 $\Rightarrow (\frac {a^2}{a^2+b^2} - \frac{-b^2}{a^2+b^2}, \frac{-ab}{a^2+b^2} + \frac{ab}{a^2+b^2}) = (1, 0)$, $A \neq (0,0)$
		 $\Rightarrow (\frac{a^2+b^2}{a^2+b^2}, \frac{ab-ab}{a^2+b^2}) = (1,0)$, $A \neq (0,0)$
		 $\Rightarrow (1,0) = (1,0)$, $A \neq (0,0)$
		 $\therefore$ the multiplicative inverse of any ordered pair $(a,b) \in F$ is defined to be $(a,b)^{-1} = (\frac{a}{a^2+b^2}, \frac{-b}{a^2+b^2})$ , $(a,b) \neq (0,0)$
		 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
5. 
	 (a) 
		 Let $A = (a+bi, c+di), \quad A \in F, \quad a,b,c,d \in \mathbb{R}$
		 We are trying to prove that $\exists (1,0)$ such that $A \times (1,0) = A$ 
		 The LHS of the equation turns into
		 $\Rightarrow (a+bi,c+di)(1,0)$
		 $\Rightarrow ((a+bi)(1) - (c+di)(0), (a+bi)(0) + (c+di)(1)$
		 $\Rightarrow (a+bi, c+di)$
		 $\Rightarrow A$
		 The RHS stays as $A$
		 $A=A$
		 $LHS = RHS$
		 $\therefore$ the multiplicative identity of $F$ is defined to be $(1,0)$
	 (b)
		 $\exists(0,0) \in F$ Such that $(a,b) + (0,0) = (a,b), \quad a,b \in \mathbb{C}$
		 $\Rightarrow (a + 0, b + 0) = (a,b)$
		 $\Rightarrow (a,b) = (a,b)$
		 Let $A = (a,b), \quad a,b \in \mathbb{C}, \quad A \in F$
		 $AA^{-1} = (1,0)$ if $A \neq (0,0)$
		 $\Rightarrow (a,b)(\frac{a}{a^2+b^2}, \frac{-b}{a^2+b^2}) = (1,0)$
		 $\Rightarrow (\frac {a^2}{a^2+b^2} - \frac{-b^2}{a^2+b^2}, \frac{-ab}{a^2+b^2} + \frac{ab}{a^2+b^2}) = (1, 0)$
		 $\Rightarrow (\frac{a^2+b^2}{a^2+b^2}, \frac{ab-ab}{a^2+b^2}) = (1,0)$
		 $\Rightarrow (1,0) = (1,0), \quad a^2 + b^2 \neq 0$
		 $\therefore$ $\exists (a,b)^{-1} \in  F \; \forall  \; a,b \in \mathbb{C} \text{ where } a^2 + b^2 \neq 0$
	 (c)
		 F is not a field due to the fact that there exist some elements in F that do not have a multiplicative inverse, an example is (1, i) because $1^2 + i^2 = 0$ which we showed in the last question means it does not have a multiplicative inverse 
		 $\Rightarrow (1,i)(\frac{1}{1^2 + i^2}, \frac{-i}{1^2 + i^2}) \stackrel{?}{=} (1,0)$
		 $\Rightarrow (\frac {1^2}{1^2+i^2} - \frac{-i^2}{1^2+i^2}, \frac{-1i}{1^2+i^2} + \frac{1i}{1^2+i^2}) \stackrel{?}{=} (1,i)$
		 $\Rightarrow (\frac {1}{0} - \frac{1}{0}, \frac{-i}{0} + \frac{i}{0}) \stackrel{?}{=} (1,i)$
		 $\Rightarrow undefined \neq (1,i)$
		 $RHS \neq LHS$
		 $\therefore$ F is not a field
		 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
6. 
	 (a)
		 Let $x = a +b\sqrt{3}, \quad y = c +d\sqrt{3}, \quad a,b,c,d \in \mathbb{Q}, \quad x,y \in F$
		 We are trying to prove that F is closed under addition
		 $\Rightarrow x+y$
		 $\Rightarrow a+b\sqrt{3} + c + d\sqrt{3}$
		 $\Rightarrow (a+b) + (c+d)\sqrt{3}$
		 $(a+b)$ and $(c+d)$ $\in \mathbb{Q}$ as $\mathbb{Q}$ is closed under addition
		 $\therefore (a+b) + (c+d)\sqrt{3} \in F$ as it follows the form $a' + b'\sqrt{3}, \quad a',b' \in \mathbb{Q}$  which means F is closed under addition
		 We are trying to prove that F is closed under multiplication
		 $\Rightarrow xy$
		 $\Rightarrow (a +b\sqrt{3})(c+d \sqrt{3})$
		 $\Rightarrow ac + ad\sqrt{3} + bc\sqrt{3} + 3bd$
		 $\Rightarrow (ac+3bd) + (ad+bd)\sqrt{3}$
		 $(ac+3bd)$ and $(ad+bd)$ $\in \mathbb{Q}$ as $\mathbb{Q}$ is closed under addition and multiplication
		 $\therefore (ac+3bd) + (ad+bd)\sqrt{3} \in F$ as it follows the form $a' + b'\sqrt{3}, \quad a',b' \in \mathbb{Q}$  which means F is closed under multiplication
	 (b)
		 $\mathbb{R}$ is a field which means that associativity, commutativity, and distributivity are satisfied for $\mathbb{R}$, $F$ is a subset of $\mathbb{R}$ and is closed under multiplication and addition (as proved in the previous question) therefore it follows that $F$ satisfies associativity, commutativity, and distributivity
	 (c)
		 The additive identity for $\mathbb{R}$ is $0$, this can be written in $F$ as $0 +0\sqrt{3}$  
		 $\Rightarrow A + (0 + 0\sqrt{3}) = A$ 
		 $\Rightarrow A = A$,   $\forall A \in F$
		 We are trying to show that the additive inverse exists for all $F$ and is contained in $\mathbb{R}$
		 Let $x = a + b\sqrt{3}$,     $x \in F$,     $a,b \in \mathbb{Q}$  
		 $\Rightarrow x + -(x) = 0 + 0\sqrt{3}$
		 $\Rightarrow a + b\sqrt{3} + -(a + b\sqrt{3}) = 0 + 0\sqrt{3}$
		 $\Rightarrow a + b\sqrt{3} + -a - b\sqrt{3} = 0 + 0\sqrt{3}$
		 $\Rightarrow (a-a) + (b-b)\sqrt{3} = 0 + 0\sqrt{3}$
		 $\Rightarrow 0 + 0\sqrt{3} = 0 + 0\sqrt{3}$
		 $LHS = RHS$
		 because $\mathbb{R}$ is a field that is closed under addition and multiplication there is no way that we could have exited  $\mathbb{R}$ during the previous steps
		 QED
	 (d)
		 The multiplicative identity of $\mathbb{R}$ is 1 which can be written in $F$ as $1 + 0\sqrt{3}$ 
		 $\Rightarrow A(1 + 0\sqrt{3}) = A$
		 $\Rightarrow 1A + 0A\sqrt{3} = A$
		 $\Rightarrow A = A$,   $\forall A \in F$ 
		 We are trying to prove that the multiplicative inverse exists for all non-zero $F$ and is contained in $\mathbb{R}$
		 Let $x = a + b\sqrt{3}$,     $x \in F$,     $a,b \in \mathbb{Q}$  
		 $\Rightarrow xx^{-1} = 1 + 0\sqrt{3}$ 
		 $\Rightarrow (a + b\sqrt{3})(\frac{a-b\sqrt{3}}{a^2-3b^2}) = 1 + 0\sqrt{3}$
		 $\Rightarrow (\frac{(a + b\sqrt{3})(a-b\sqrt{3})}{a^2-3b^2}) = 1 + 0\sqrt{3}$
		 $\Rightarrow (\frac{a^2-3b^2}{a^2-3b^2}) = 1 + 0\sqrt{3}$                , $a^2-3b^2 \neq 0$
		 $\Rightarrow 1 = 1 + 0\sqrt{3}$                             , $a^2-3b^2 \neq 0$
		 $\Rightarrow 1 = 1$                                           , $a^2-3b^2 \neq 0$
		 $a^2-3b^2 \neq 0 \quad \Rightarrow \quad a \neq b\sqrt{3} \quad \Rightarrow \quad x \neq 0 + 0\sqrt{3}$
		 $LHS = RHS$  $\forall x \neq 0 + 0\sqrt{3}$
		 because $\mathbb{R}$ is a field that is closed under addition and multiplication there is no way that we could have exited  $\mathbb{R}$ during the previous steps
		 QED
		 <div style="page-break-after: always; visibility: hidden">\pagebreak</div>
7. 
	let $a,b,c,d$ be polynomials with coefficients in $\mathbb{R}$ and $a,b,c,d\neq 0$

	Multiplication can be defined as $\frac{a}{b} \times \frac{c}{d} = \frac{ac}{bd}$ 
	The multiplication of polynomials is closed therefore $ac$ and $bd$ can be written as polynomials, lets call them $p$ and $q$ respectively. $\frac{p}{q} \in F$   $\therefore$  $F$ is closed over Multiplication

	Addition can be defined as $\frac{a}{b} + \frac{c}{d} = \frac{ad + cb}{bd}$
	The multiplication and addition of polynomials is closed therefore $ad+cb$ and $bd$ can be written as polynomials, lets call them $p$ and $q$ respectively. $\frac{p}{q} \in F$   $\therefore$  $F$ is closed over Addition