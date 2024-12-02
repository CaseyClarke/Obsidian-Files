1. 
	<br>(a)
	
	The general form for $P_2(\mathbb{C})$ is 
	$ax^2 + bx + c$
	Given that $P(1) = 0$
	$0 = a + b + c$
	$a = -b-c$
	$0 =(-b-c)x^2 + bx + c$
	$0 =-bx^2-cx^2 + bx + c$
	$0 =b(-x^2+x) + c(-x^2 + 1)$
	
	This is the form of a linear combination for $\{-x^2 + x, -x^2 + 1\}$
	$\therefore \{-x^2 + x, -x^2 + 1\}$ forms a basis for  $P_2(\mathbb{C})$ Given the initial condition $P(1) = 0$
	
	(b)
	
	The dimension of U is 2
	
	(c)
	
	$\left[x^2 + 2x - 3\right]_B = \begin{pmatrix}   2\\-3\\ \end{pmatrix}$

<div style="page-break-after: always;"></div>

2. 
	<br>(a)
	
	To check if these vectors form a basis we check if they are linearly independent, they can be represented in the form of a matrix as 
	$$A = \begin{pmatrix}   1&1&2\\1&2&2\\2&4&3 \end{pmatrix}$$
	Which has an RREF of 
	$$RREF(A) = \begin{pmatrix}   1&0&0\\0&1&0\\0&0&1 \end{pmatrix}$$
	Which means they are linearly independent and they span the space by definition these 3 vectors form the basis
	$B = \{(1,1,2), (1,2,4), (2,4,3)\}$
	
	(b)
	
	By the make-your-life-easy-theorem we know that a basis for $\mathbb{R}^3$ contains 3 linearly independent vectors exactly, our basis is 3 linearly independent vectors in $\mathbb{R}^3$ so they must form a basis for the whole of $\mathbb{R}^3$ as well
	
	(c)
	
	The rank of A is the dimension of the vector space, that is 3
	
	(d)
	
	There is no basis for $NULL(A)$ as $RREF(A)$ is the identity matrix and so it has a dimension of 0
	
	(e)
	
	Yes as we have shown that the column space of A forms a basis for $\mathbb{R}^3$ and all of those values lie in $\mathbb{R}^3$

<div style="page-break-after: always;"></div>

3. 
	<br>(a)
	
	$$B = \begin{pmatrix}   1&0&2\\1&1&3\\3&1&7 \end{pmatrix}$$
	$$RREF(B) = \begin{pmatrix}   1&0&2\\0&1&1\\0&0&0 \end{pmatrix}$$
	We get the row space by taking the non-zero rows of the RREF of the matrix, therefore the row space basis is 
	$R_B = \Bigg{\langle} \begin{pmatrix}   1 \\ 0\\2 \end{pmatrix}, \begin{pmatrix}   0 \\ 1\\ 1\end{pmatrix} \Bigg{\rangle}$
	
	We get the column space by taking the pivot columns corresponding to the original matrix, therefore the column space basis is 
	$C_B = \Bigg{\langle} \begin{pmatrix}   1 \\ 1\\3 \end{pmatrix}, \begin{pmatrix}   0 \\ 1\\ 1\end{pmatrix} \Bigg{\rangle}$
	
	We get the null space by finding any paramaterized solutions to the matrix equation $Bx = 0$
	$N_B = \Bigg{\langle} \begin{pmatrix}   -2\\-1\\1 \end{pmatrix} \Bigg{\rangle}$
	
	(b)
	
	The rank of B is 2 and the dimension of the row and column space is 2 while the null space has a dimension of 1
	
	(c)
	
	Yes as it is just $-1 \cdot \begin{pmatrix}   -2\\-1\\1 \end{pmatrix} = \begin{pmatrix}   2\\1\\-1 \end{pmatrix}$

<div style="page-break-after: always;"></div>

4. 
	 <br>(a)
	
	To find the basis of this span that is conveniently represented by the matrix A, we look at $REF(A) = R$  and find the non-zero rows, they are 1, 2, 3 which means the basis is then
	
	$B = \left\{ (x^5 -2x^4 -x-5), (x^3-3), (x^2 + x + 2) \right\}$
	
	(b)
	
	We can represent these matrices as vectors in $\mathbb{R}^4$ and represent these vectors as a matrix, this is conveniently the matrix A. We find the columns with pivots in $REF(A) = R$ and those columns correspond to the elements in the basis, the columns with pivots are 1, 3, 4 so the basis is then
	
	$B = \Bigg{\langle} \begin{pmatrix}   1 \\ -1 \\2 \\ -3 \end{pmatrix}, \begin{pmatrix}   -1 \\ 1 \\-3 \\ 2 \end{pmatrix},  \begin{pmatrix}   2 \\ 2 \\2 \\ 0 \end{pmatrix}\Bigg{\rangle}$ 
	
	Or in the original matrix form
	
	$B = \Bigg{\langle} \begin{pmatrix}   1 & -1\\2 & -3 \end{pmatrix}, \begin{pmatrix}   -1 & 1 \\-3 & 2 \end{pmatrix},  \begin{pmatrix}   2 & 2 \\ 2 & 0 \end{pmatrix}\Bigg{\rangle}$
	
	(c)
	
	$x_5 -2t -s -5r = 0 = 2t + s + 5r$
	$x_4 = t$
	$x_3 - 3r = 0 = 3r$
	$x_2 + s + 2r = 0 = -s - 2r$
	$x_1 = s$
	$x_0 = r$
	
	$$\begin{pmatrix}   2t + 1s + 5r \\ 1t + 0s + 0r \\ 0t + 0s + 3r \\ 0t -s -2r \\ 0t - 1s + 0r \\ 0t + 0s + 1r \end{pmatrix} = t\begin{pmatrix}   2 \\ 1 \\0 \\ 0 \\ 0 \\ 0 \end{pmatrix} + s\begin{pmatrix}   1 \\ 0 \\0 \\ -1 \\ 1 \\ 0\end{pmatrix} + r\begin{pmatrix}   5 \\ 0 \\3 \\ -2 \\ 0 \\ 1\end{pmatrix}$$
	$$N_B = \Bigg{\langle} \begin{pmatrix}   2 \\ 1 \\0 \\ 0 \\ 0 \\ 0 \end{pmatrix}, \begin{pmatrix}   1 \\ 0 \\0 \\ -1 \\ 1 \\ 0\end{pmatrix},\begin{pmatrix}   5 \\ 0 \\3 \\ -2 \\ 0 \\ 1\end{pmatrix} \Bigg{\rangle}$$
	
	(d)
	
	The column space of A is a $\bbox[lightgreen]{3}$-dimensional subspace of $\mathbb{R}^{\bbox[lightgreen]{4}}$. 
	The row-space of A is a $\bbox[lightgreen]{3}$-dimensional subspace of $\mathbb{R}^{\bbox[lightgreen]{6}}$. 
	The null-space of A is a $\bbox[lightgreen]{3}$-dimensional subspace of $\mathbb{R}^{\bbox[lightgreen]{6}}$. The rank of A is $\bbox[lightgreen]{3}$

<div style="page-break-after: always;"></div>

5. 
	<br>Dimension of Row-Space: 4
	
	Dimension of Column-Space: 4
	
	Dimension of Null-Space: 3

<div style="page-break-after: always;"></div>

6. 
	<br>We are trying to find functions $f: S \rightarrow \mathbb{F}$ such that we can create any element in $\mathbb{F}^3$ from the given inputs a, b, c
	
	This space is essentially $\mathbb{F}^3$ as our elements are 3-tuple maps with elements in $\mathbb{F}$ just hidden behind a function which is the definition of $\mathbb{F}^3$
	
	Let 0, 1 be the additive and multiplicative identities respectively in the arbitrary field $\mathbb{F}$
	
	Here we are essentially creating the standard basis of  $\mathbb{F}^3$ 
	$$f_1(n) = \begin{cases} f_1(a) = 1 \\ f_1(b) = 0 \\ f_1(c) = 0\end{cases}$$
	$$f_2(n) = \begin{cases} f_2(a) = 0 \\ f_2(b) = 1 \\ f_2(c) = 0\end{cases}$$
	$$f_3(n) = \begin{cases} f_3(a) = 0 \\ f_3(b) = 0 \\ f_3(c) = 1\end{cases}$$
	$B = \langle f_1, f_2, f_3 \rangle$
	
	The dimension is 3