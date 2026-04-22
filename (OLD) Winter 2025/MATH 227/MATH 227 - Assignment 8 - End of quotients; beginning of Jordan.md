# Question 1

(a)

- Homomorphism: $f(xy) = |xy| = |x||y|$
- Kernal: $|x| = 1 \iff x = -1,1 \quad |1| = 1 \quad |-1| = 1$
- Onto: $\forall y \in \mathbb{R}_{>0}^\times \implies y \in \mathbb{R}^\times$

(b)

- By Theorem 1 we know it is isomorphic to $\mathbb{R}^\times_{>0}$
- as $\mathbb{R}^\times_{\neq 0}  / ker(f) \cong img(f)$
- where $ker(f) = {\pm 1}$
- and $img(f) = \mathbb{R}^\times_{>0}$

{{ENDQUESTION}}

# Question 2

$\forall r \in R, s \in S_a$
$rs = r(an)$ for some $n \in \mathbb{Z}$
$arn = ak$ for some $k \in \mathbb{Z}$
$ak \in S_a$ by definition

Non-empty:
- $0 \in S_a$

Closure of negation:
- $-x \in S_a$ as every x corresponds to another -x $\in S_a$

Closure of addition
- $x,y \in S_a$
- $x + y = an+am$ for some $n,m \in R$
- $\Rightarrow a(n+m) \in S_a$ by definition

{{ENDQUESTION}}
# Question 3

(a)

- Non-empty:
	- $0_R = 0x + 0y^2 \in S$

- Closure of negation:
	- $-xp(x,y) -y^2(q(x,y) \in S$ as $-p(x,y), -q(x,y) \in R$
	- $x(-p(x,y)) + y^2(-q(x,y)) = xR + y^2R$

- Closure of additon:
	- $u,v \in S$
	- $u + v = xR_1 + y^2R_2 + xR'_1 + y^2R'_2$
	- $u + v = x(R_1 + R'_1) + y^2(R_2 + R'_2)$
	- $Q = R_1+ R'_1, R = R_2 + R_2' \in R$
	- $u + v = xQ + y^2Q \implies u + v \in S$

- Ideal:
	- $\forall r \in R, s = xr'_1 +y^2r'_2 \in S$
	- $rs = r(xr'_1 + y^2r'_2)$
	- $rs = xrr'_1 + y^2rr'_2$
	- $Q = rr'_1 , Q' = rr'_2 \in R$ 
	- $rs = xQ + y^2Q' \implies rs \in S$

(b)

- Since this quotient is essientially $\mod rx+r'y^2$ for some $r,r' \in R$
- by choosing the r's we can remove all multiples of $x$ but because of the $y^2$
- we can only remove multiples of $y^2$ not $y$ as $\nexists r \in R$ S.T. $ry^2 = y \; \lor rx = y$ 

(c)

- $[x+y][x-y] + [x+y]^2 + 2[1+y]^3 = [x^2 - y^2] + [x^2 + 2xy +y^2] + [2(1+ 3y +3y^2 + 3y^3)]$
- $[0- 0] + [0 + 0 + 0] + [2 + 6y]$
- $2[1] + 6[y]$


{{ENDQUESTION}}

# Question 4

- I am not going to write them all out but it is essentially all 12 permutations of the list 
- $l =(1,1,2,3)$ arranged in the form
$$\begin{pmatrix} 
l_1 &0 & 0 & 0 \\ 0 & 1_2 & 0 & 0 \\ 0 & 0 & l_3 & 0 \\ 0 & 0 & 0 & l_4
\end{pmatrix}$$

{{ENDQUESTION}}

# Question 5

$[J_3(2) \oplus J_2(5)]$

$$\begin{pmatrix} 
2 &1 & 0 & 0 & 0 \\ 
0 & 2 & 1 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 1 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

$[J_3(2) \oplus J_1(5) \oplus J_1(5)]$
$$\begin{pmatrix} 
2 &1 & 0 & 0 & 0 \\ 
0 & 2 & 1 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 0 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

$[J_2(2) \oplus J_1(2) \oplus J_2(5)]$

$$\begin{pmatrix} 
2 &1 & 0 & 0 & 0 \\ 
0 & 2 & 0 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 1 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

$[J_2(2) \oplus J_1(2) \oplus J_1(5) \oplus J_1(5)]$

$$\begin{pmatrix} 
2 &1 & 0 & 0 & 0 \\ 
0 & 2 & 0 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 0 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

$[J_1(2) \oplus J_1(2) \oplus J_1(2) \oplus J_2(5)]$

$$\begin{pmatrix} 
2 &0 & 0 & 0 & 0 \\ 
0 & 2 & 0 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 1 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

$[J_1(2) \oplus J_1(2) \oplus J_1(2) \oplus J_1(5) \oplus J_1(5)]$

$$\begin{pmatrix} 
2 &0 & 0 & 0 & 0 \\ 
0 & 2 & 0 & 0 & 0 \\ 
0 & 0 & 2 & 0 & 0 \\ 
0 & 0 & 0 & 5 & 0 \\
0 & 0 & 0 & 0 & 5
\end{pmatrix}$$

{{ENDQUESTION}}


# Question 6

$p_B(t) = det(B-\lambda I)$
$p_A(t) = det(A-\lambda I)$

$A \sim B \stackrel{?}{\implies} p_B(t) = p_A(t)$
- $A \sim B \implies A = PBP^{-1}$
- $p_A(t) = det(A-\lambda I) = det(PBP^{-1} - \lambda I) = det(PBP^{-1} - - P(\lambda I)P^{-1}$
- $det(P(B-\lambda I) P^{-1}) = det(P)det(B-\lambda I)det(P)^{-1}$
- $p_A(t) = det(B-\lambda I) = p_B(t)$
- $QED$

$p_B(t) = p_A(t)\stackrel{?}{\implies} A \sim B$
- This is not true when one matrix is diagonalisable normally but another one is only diagonalizable using jordan blocks
- Counterexample:
- $A = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} \quad B = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$
- $p_A(t) = p_B(t) = \lambda^2$
- A diagonalises as itself so its jordan form is also itself
- B has jordan form of itself since it cannot be diagonalised so it consists of a block $J_2(0)$
- but A and B are not similar since the jordan form are not equal
- $\therefore$  The converse is not true
- $QED$

{{ENDQUESTION}}
 
