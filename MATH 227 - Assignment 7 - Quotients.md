
# Question 1

(a)

- Identity:
	- $0_V \in W$ as $(0,0,0, \dots) \in V \land W$
- 
- Closure of addition:
	- $\forall v,w \in W \; v + w = (0,0,0, v_4 + w_4, v_5 + w_5, \dots) \in W$

- Closure of Scalar multiplication:
	- $\forall k \in \mathbb{F}, w \in W \;kw = (k0, k0, k0, k_4 \times w_4, k_5 \times w_5, \dots) =  (0, 0, 0, k_4 \times w_4, k_5 \times w_5, \dots)\in W$ 
- 
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
- 