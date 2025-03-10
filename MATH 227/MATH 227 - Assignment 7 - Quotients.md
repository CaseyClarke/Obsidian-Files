# Question 1

(a)

- Identity:
	- $0_V \in W$ as $(0,0,0, \dots) \in V \land W$
- 
- Closure of addition:
	- $\forall v,w \in W \; v + w = (0,0,0, v_4 + w_4, v_5 + w_5, \dots) \in W$

- Closure of Scalar multiplication:
	- $\forall k \in \mathbb{F}, w \in W \;kw = (k0, k0, k0, k_4 \times w_4, k_5 \times w_5, \dots) =  (0, 0, 0, k_4 \times w_4, k_5 \times w_5, \dots)\in W$ 


(b)

- A basis for $W$ is 
- $$\{ b_4 = (0,0,0,1,0,0,\dots), \; b_5 = (0,0,0,0,1,0,0,\dots), \;b_6 = (0,0,0,0,0,1,0,\dots), \;  \dots \}$$
- A basis for V based off of extending the basis for $W$ is
-  $$\{ b_1 = (1,0,0,0,0,0,\dots), \; b_2 = (0,1,0,0,0,0,0,\dots), \;b_3 = (0,0,1,0,0,0,0,\dots), \;  b_4, b_5, b_6 \dots \}$$
- Meaning that the basis for $V/W$ is 
- $$\{(1,0,0,0,0,0,\dots), \; (0,1,0,0,0,0,0,\dots), \; (0,0,1,0,0,0,0,\dots)\}$$

(c)

- The dimension of their respective basises are the same $(3)$ meaning they must be isomorphic to each other, we can also see this by ignoring all of the terms past $n = 3$ in the basis for $V/W$ as they are all 0 and contribute nothing to the basis, this gives us the standard basis for $\mathbb{F}^3$


{{ENDQUESTION}}

# Question 2

(a)

- $[D] = \begin{pmatrix} 0 & 0 & 0 \\ 2 & 0 & 0 \\ 0 & 1 & 0 \end{pmatrix}$

(b)

- $K = \operatorname{Null}(D) = \begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$
- $\overline{B} = [P_2(\mathbb{R}) / K] = [((1,0,0), (0,1,0))]_{\mathbb{F^3}} = [(x^2, x)]_{P_2(\mathbb{F})}$

(c)

- Given that two polynomials are equivalent if they differ by a multiple of $K$ that means that they are equivalent if they differ by only a constant term, and since derivatives of polynomials erase constants anyway, any element of the same equivalence class will have the same derivative

(d)

- $[D'] = \begin{pmatrix} 0 & 0  \\ 2 & 0 \\ 0 & 1  \end{pmatrix}$

(e)

- $[D''] = \begin{pmatrix} 0 & 0 & 0 \\ 2 & 0 & 0 \end{pmatrix}$

(f)

- Same argument as (c), i'll write it algebraically this time
- for some $q(x), p(x)$ they are equivalent iff they differy by only a constant e.g.
- $p(x) - q(x) = c$
- $D(p(x) - q(x)) = D(c)$
- $D(p(x)) - D(q(x)) = 0$
- $D(p(x)) = D(q(x))$
- Meaning that any element in the same equivalence class will have the same derivative, meaning function is well defined

(g)

- $[D'''] = \begin{pmatrix} 0 & 0 \\ 2 & 0 \end{pmatrix}$

{{ENDQUESTION}}

# Question 3

(a)

- $\{A \in G \ | \operatorname{det}(A) = 1\}$

(b)

- The equivalence classes in $G/H$ are all matrices with the same determinant,
- thus we can write a representative of any of these classes as 
- $[a] = \begin{pmatrix} a  & 0 & \dots \\ 0 & 1 & \dots \\ \vdots & \vdots & \ddots \end{pmatrix}$
- which is a diagonal matrix with $\operatorname{det}(A) = a$ 

{{ENDQUESTION}}

# Question 4

(a)

- Identity: 
	- $\operatorname{sgn}(1_g) = 1 \implies \in H$

- Closure of Multiplication:
	- $\operatorname{sgn}(g \circ g') = \operatorname{sgn}(g)\operatorname{sgn}(g') = (1)(1) = 1 \implies \in H$

- Closure of inverse:
	- $\operatorname{sgn}(g^{-1}) = \operatorname{sgn}(g)^{-1} = (1)^{-1} = 1 \implies \in H$

- Normality:
	- $\operatorname{sgn}(ghg^{-1}) = \operatorname{sgn}(g)\operatorname{sgn}(h)\operatorname{sgn}(g)^{-1} = \operatorname{sgn}(g)(1)\operatorname{sgn}(g)^{-1} = 1 \implies \in H$

(b)

- The equivalence classses of $G/H$ are $[\text{Even Permuatations}]$ and $[\text{Odd Permutations}]$
- $f([g]) = \operatorname{sgn}(g) \mod 2$

- Homomorphism:
	-  $\operatorname{sgn}(g \circ g') = \operatorname{sgn}(g)\operatorname{sgn}(g')$
	-  $f([g \circ g']) = \operatorname{sgn}(g)\operatorname{sgn}(g') \mod 2$
	- $\times \equiv + \mod 2$
	-  $f(g \circ g') = \operatorname{sgn}(g) + \operatorname{sgn}(g')$

- One-to-one:
	- $\operatorname{Ker}(f) = H$ and $H = 1_g$ which is the trivial kernal

- Onto:
	- $\operatorname{Img}(f) = \operatorname{sgn}(g) \mod 2 = \{0,1\} = \mathbb{Z}_2$


{{ENDQUESTION}}

# Question 5

Closure of Addition:
- $k,k' \in K$
- $f(k) = 0_r \quad f(k') = 0_r$
- $f(k+k') = f(k) + f(k')$
- $f(k+k') = 0_r + 0_r = 0_r$
- $\implies k + k' \in K$

Ideal:
- $f(rkr') = f(r)f(k)f(r')$
- $f(rkr') = f(r)(0_r)f(r') = 0_r$
- $\implies rkr' \in K$


{{ENDQUESTION}}

# Question 6

(a)

- Identity:
	- $0_r = x^3(0) \implies 0 \in S$

- Closure of addition
	- $p(x) + q(x) = x^3p'(x) + x^3q'(x) = x^3(p'(x) + q'(x))$
	- $r(x) = p'(x) + q'(x) \in R$
	- $x^3r(x) \in S \implies p(x) + q(x) \in S$

	Inverses:
	- $-p(x) = -x^3(p'(x)) = x^3(-p'(x)) \implies -p(x) \in S$

- Ideal:
	- $p(x)s(x) = p(x)x^3s'(x) = x^3p(x)s'(x)$
	- $r(x) = p(x)s'(x) \in R$
	- $x^3r(x) \in S \implies p(x)s(x) \in S$


(b)

- $p(x),q(x)$ are in the same equivalence class if they differ by some polynomial multiple of $x^3$
- $p(x) - q(x) = x^3r(x)$
- $p(x) = x^3r(x) + q(x)$
- This is the exact form of polymomial division with quotient $r(x)$ and remainder $q(x)$
- The degree of the remainder of a polynomial division must be strictly less than the degree of the divisior i.e $\operatorname{deg}(x^3) > \operatorname{deg}(q(x)) \implies \operatorname{deg}(q(x)) \leq 2$
- but $p(x) \sim q(x)$ 
- meaning that we can choose $q(x)$ as the representative and it will always have degree $\leq 2$

(c)

- $[(x^2 + 1)(x-1)] = [x^3 -x^2 + x -1] =  [-x^2 + x - 1]$
- 
- 