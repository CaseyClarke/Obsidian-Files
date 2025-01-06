1.       
	 ‎ 
	Multiplicative Identity:
	$\exists 1 \in R \text{ such that } 1a=a$
	$\Rightarrow 1a -a = a -a$
	$\Rightarrow a(1-1) = a(1-1)$
	$\Rightarrow a(0) = a(0)$
	$\Rightarrow 0 = 0$
	(a)
	
	$a0 = 0$
	$\Rightarrow a0 + a = 0 + a$
	$\Rightarrow a0 + a = a$
	$\Rightarrow a(0+1) = a$
	$\Rightarrow a1 = a$
	$\Rightarrow a=a$ 
	(b)
	
	$-x = -1(x)$
	$\Rightarrow -x + x = -1(x) + x$
	$\Rightarrow x(-1 + 1) = x(-1 +1)$
	$\Rightarrow x(0) = x(0)$
	$\Rightarrow 0 = 0$
	(c)
	
	$a((b+c)+d) = ab + (ac + ad)$
	LHS:
	$ab+(ac+ad)$
	$\Rightarrow ab+a(c+d)$
	$\Rightarrow a(b+(c+d))$
	$\Rightarrow a((b+c)+d)$
	$LHS = RHS$
	
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. 
	‎ 
	I will be using $\varnothing$ to denote an empty set for this question
	
	(a)
	
	$\text{All elements in } R=2^s: (\quad \varnothing, \quad \{a,b,c\},  \quad \{a\},  \quad \{b\},  \quad \{c\}, \quad \{a,b\},  \quad \{a,c\}, \quad  \{b, c\})$
	
	(b)
	
	$\exists \; \varnothing \in R=2^s \text{ such that } A \oplus \varnothing = A \quad \forall A \in R=2^s$ 
	$A \oplus \varnothing = A$
	$A \triangle \varnothing = A$
	By the definition of a symmetric difference all of the elements in A are either in A and $\varnothing$ but not in both. As $\varnothing$ has no elements it could never overlap with A and remove elements from the result. 
	$A=A$
	
	(c)
	
	$\exists \; B \text{ such that } A \oplus B = \varnothing \quad \forall A \in R$
	For a symmetric difference to return the empty set both sets must have exactly the same elements so that all elements are in both sets thus returning none of them.
	$\Rightarrow B=A$
	$\Rightarrow A \oplus A = \varnothing$
	$\therefore$ the additive inverse for any number in $R = 2^S$ is itself
	
	(d)
	
	$\exists \; S \in R=2^s \text{ such that } A \odot S = A \quad \forall A \in R=2^s$ 
	$A \odot S = A$
	By the definition of an intersection only the common elements remain, therefore by choosing the whole set as the multiplicative identity we can guarantee that every element in A is common between the sets as S contains every element A could possibly have.
	
	(e)
	
	$\exists \; A^{-1} \in R=2^s \text{ such that } A \odot A^{-1} = S \quad \forall A \in R=2^s$
	The only way that the equation $A \odot A^{-1} = S$ can be true is if both $A, A^{-1} = S$ as they both must have the whole set as common elements for $A \cap A^{-1} = S$ to be true. Therefore $A = S$ is the only element in this Ring that has a multiplicative inverse
	
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. 
$$BCA= \begin{pmatrix}
	1&-2&-2\\
	2&1&3\\
	2&1&4\\
	\end{pmatrix}$$
$$BC= \begin{pmatrix}
	1&-2&-2\\
	2&1&3\\
	2&1&4\\
	\end{pmatrix}A^{-1}$$
$$BC= \begin{pmatrix}
	1&-2&-2\\
	2&1&3\\
	2&1&4\\
	\end{pmatrix}
	\begin{pmatrix}
	0&-3&-1\\
	1&2&1\\
	4&2&1\\
	\end{pmatrix}$$
$$BC= \begin{pmatrix}
	0(1) + 1(-2) + 4(-2)&-3(1) + 2(-2) + 2(-2)&-1(1) + 1(-2) + 1(-2)\\
	0(2) + 1(1) + 4(3)&-3(2) + 2(1) + 2(3)&-1(2) + 1(1) + 1(3)\\
	0(2) + 1(1) + 4(4)&-3(2) + 2(1) + 2(4)&-1(2) + 1(1) + 1(4)\\
	\end{pmatrix}$$
$$BC= \begin{pmatrix}
	-10&-11&-5\\
	13&2&2\\
	17&4&3\\
	\end{pmatrix}$$
$$C= B^{-1}\begin{pmatrix}
	-10&-11&-5\\
	13&2&2\\
	17&4&3\\
	\end{pmatrix}$$
$$C= \begin{pmatrix}
	1&2&-1\\
	2&2&4\\
	1&3&-3\\
	\end{pmatrix}
	\begin{pmatrix}
	-10&-11&-5\\
	13&2&2\\
	17&4&3\\
	\end{pmatrix}$$
$$\text{Simplifing the numbers in the right matrix given that we are working in } \mathbb{F}_{11}$$
$$C= \begin{pmatrix}
	1&2&-1\\
	2&2&4\\
	1&3&-3\\
	\end{pmatrix}
	\begin{pmatrix}
	1&0&6\\
	2&2&2\\
	6&4&3\\
	\end{pmatrix}$$
$$C= \begin{pmatrix}
	1(1) + 2(2) + 6(-1)&0(1) + 2(2) + 4(-1)&-3(1) + 6(2) +-4(-1)\\
	1(2) + 2(2) + 6(4)&0(2) + 2(2) + 4(4)&-3(2) + 6(2) +-4(4)\\
	1(1) + 2(3) + 6(-3)&0(1) + 2(3) + 4(-3)&-3(1) + 6(3) +-4(-3)\\
	\end{pmatrix}$$
$$C= \begin{pmatrix}
	-1&0&7\\
	30&20&28\\
	-11&-6&3
	\end{pmatrix}$$
$$\text{Simplifing the numbers in the matrix given that we are working in } \mathbb{F}_{11}$$
$$C= \begin{pmatrix}
	-1&0&7\\
	-3&-2&6\\
	0&5&3
	\end{pmatrix}$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
$$(2I_2-A^T)^{-1} = \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}$$
$$(2I_2-A^T) = \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}^{-1}$$
$$\text{The above matrix is has an inverse due to the fact that}$$
$$det\begin{pmatrix}2&1 \\ -1&0\end{pmatrix} = (2)(0) - (-1)(1) = 1 \neq 0$$
$$-A^T = \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}^{-1} - 2I_2$$
$$A^T = 2I_2 - \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}^{-1} $$
$$A^T = 2\begin{pmatrix}1&0 \\ 0&1\end{pmatrix} - \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}^{-1} $$
$$A^T = \begin{pmatrix}2&0 \\ 0&2\end{pmatrix} - \frac{1}{(2)(0) - (-1)(1)}\begin{pmatrix}0&-1 \\ 1&2\end{pmatrix}$$
$$A^T = \begin{pmatrix}2&0 \\ 0&2\end{pmatrix} - \begin{pmatrix}0&-1 \\ 1&2\end{pmatrix}$$
$$A^T = \begin{pmatrix}2&1 \\ -1&0\end{pmatrix}$$
$$A = \begin{pmatrix}2&-1 \\ 1&0\end{pmatrix}$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. 
	‎ 
	Proof that $A$ is invertible:
	
	We must show that $AB = BA = I_9$ for an arbitrary matrix $B$ with the same dimensions as $A$ 
	$3A^2-5A- I_9 = 0_{9x9}$
	$\Rightarrow (3A-5I_9)A = I_9$
	The above equation is in the form $BA = I_9$ where $B = 3A-5I_9$ 
	
	$3A^2-5A- I_9 = 0_{9x9}$
	$\Rightarrow A^23-A5- I_9 = 0_{9x9}$
	$\Rightarrow A(A3-I_95) = I_9$
	The above equation is in the form $AB = I_9$ where $B = A3-I_95$ 
	
	$B$ is the same in both equations by commutativity of multiplication in any arbitrary field
	$3A-5I_9 = A3-I_95$
	$3A-5I_9 = 3A-5I_9$
	$\therefore AB = BA  = I_9$ Holds for $A$
	QED
	
	Solving for for $A^{-1}$
	$3A^2-5A- I_9 = 0_{9x9}$
	$\Rightarrow (3A-5I_9)A = I_9$
	$\Rightarrow (3A-5I_9)AA^{-1} = I_9A^{-1}$
	$\Rightarrow (3A-5I_9) = A^{-1}$
	$A^{-1} = (3A-5I_9)$
