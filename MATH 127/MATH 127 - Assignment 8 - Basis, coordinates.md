1. 
	<br>To find the "Ring-Span" of a ring we try to find it's basis, 
	It is easy to see how we can create any integer by doing linear combinations of $i \times i = -1$ but since we do not have the multiplicative inverse we cannot get any higher set. 
	We can also get any linear combination of $i$ itself.
	From this we can see that we can get any number of the form $a+bi \quad \forall a,b \in \mathbb{Z}$
	$\therefore$ The "Ring-Span" of $<i> \; = \{a+bi \; | \; a,b \in \mathbb{Z}\}$ 

<div style="page-break-after: always;"></div>

2. 
	<br>This similar to the previous question except now we have access to the multiplicative inverse meaning that we can create any rational number from linear combinations of $i$.
	$\therefore$ The "Field-Span" of $<i> \;  = \{a+bi \; | \; a,b \in \mathbb{Q}\}$ 

<div style="page-break-after: always;"></div>

3. 
	<br>Due to the fact that we are using a group we can only use two operations on $i$, multiplying and taking the inverse, from multiplication we can get $\{i, -1, -i, 1\}$, which all satisfy $x^2 + y^2 = 1$. And from taking the inverse we get the exact same set
	$\therefore$ The "Group-Span" of $<i>\;  = \{i, -1, -i, 1\}$ 
	
<div style="page-break-after: always;"></div>


4. 
	<br>(a)
	
	Non empty-ness:
	As $V$ is the set of all subsets of $X$ it must contain $\varnothing$ which is the zero vector in the alphabet vector space
	
	Closure of Vector addition:
	$Let \; u,v \in V$
	$u+v \in V$
	By the definition of symmetric difference it must be also in $V$
	
	Closure of Scalar Multiplication:
	$Let \; v \in V \quad a \in \mathbb{F}_2$
	$av \in V$
	If $a = 1$ then the result is the vector itself and if $a = 0$ then it is the empty set, both are in V
	
	$QED$
	
	(b)
	
	Linear Independence:
	It is evident that they are linearly independent as they are individual elements in the alphabet vector space
	
	Spanning the whole space:
	$A = z_1\{a\} +z_2\{b\}  + z_3\{c\}$
	where $z_n \in \{0,1\}$ 
	If $z_n$ is 1 we include the letter in our word, if it is not we don't, it is evident that we can get any word that only contains a b or c in it from this.
	
	As these vectors are linearly independent and they span the whole vector space by the theorem proved in class this is a basis
	
	(c)
	
	$\{a,b\} = (1,1,0)$
	$\{b,c\} = (0,1,1)$
	$\{c,a\} = (1,0,1)$
	
<div style="page-break-after: always;"></div>


5. 
	<br>(a)
	
	$B = \Bigg{\langle} \begin{pmatrix}   0 & 0\\   1 & 0 \end{pmatrix}, \begin{pmatrix}   0 & 1\\   0 & 0 \end{pmatrix},\begin{pmatrix}   1 & 0\\   0 & -1 \end{pmatrix} \Bigg{\rangle}$
	
	(b)
	
	$\left[\begin{pmatrix}   1 & 2\\   3 & -1 \end{pmatrix}\right]_B = \begin{pmatrix}   3\\2\\1 \end{pmatrix}$
	
<div style="page-break-after: always;"></div>


6. 
	<br>(a)
	
	Linear Independence:
	$x\vec{a} + y\vec{b} = \vec{0} \quad \forall \; x,y \in \mathbb{F}^2_{17}$
	$x(1,0) + y(-1,0) = (-1,1)$
	$(2x-1,-x+1) + (-1,-y+1) = (-1,1)$
	$(2x-1 -1+1, -x+1 -y+1-1) = (-1,1)$
	$(2x -1, -x -y + 1) = (-1,1)$
	$2x-1 = -1$
	$-x-y+1 = 1$
	$x = 0$
	$-x = y$
	$y = 0$
	As the only solution to the equation is $x,y = 0$ They are linearly independent
	
	Spanning the whole vector space:
	$x\vec{a} + y\vec{b} = (c_1,c_2) \quad \forall \; c_1,c_2 \in \mathbb{F}^2_{17}$
	Using our work from the previous part
	$(2x -1, -x -y + 1) = (c_1,c_2)$
	$c_1 = 2x-1$
	$c_2 = -x-y+1$
	$x = \frac{c_1 +1}{2}$
	$y = -x + 1 - c_2$
	$y = -\frac{c_1 +1}{2} + 1 - c_2$
	As we can write $x,y$ in terms of the original vector that means that we can write any vector in the field with these two vectors 
	
	As these vectors are linearly independent and they span the whole vector space by the theorem proved in class this is a basis
	
	(b)
	
	$$\left[(2,0)\right]_B = \begin{pmatrix}   \frac{3}{2}\\1 - \frac{3}{2} \end{pmatrix} = \begin{pmatrix}   10\\-9 \end{pmatrix}$$
	$$\left[(0,0)\right]_B = \begin{pmatrix}  \frac{1}{2}\\-\frac{1}{2} + 1 \end{pmatrix} = \begin{pmatrix}   9\\9 \end{pmatrix}$$
	$$\left[(-1,1)\right]_B = \begin{pmatrix}  0\\0 \end{pmatrix}$$
	
<div style="page-break-after: always;"></div>

7. 
	<br>(a)
	
	The basis for $P_2$ must have 3 elements by the make-your-life-easy theorem so at least one of these 4 vectors is linearly dependent on the others
	
	(b)
	
	There is no way that you can write the span of the $M_{2x3}(\mathbb{Q})$ in less than 6 matrices by the make-your-life-easy theorem so no these 4 matrices do not span the whole space
	
<div style="page-break-after: always;"></div>

8. 
	<br>(a)
	
	If these three vectors are linearly independent they must form a basis of $\mathbb{R}^3$ by the make-your Life-easy Theorem
	$$\begin{pmatrix} 3 & -4 & -2 \\ 0 & 1& 1 \\ -6 & 7 & 5 \end{pmatrix}$$
	Which has the RREF of 
	$$\begin{pmatrix}   1 & 0 & 0\\   0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$
	Which means that they are linearly independent and thus form a basis


	(b)
	
	If these three vectors are linearly independent they must form a basis of $P_2(\mathbb{F}_{17})$ by the make-your-Life-easy Theorem
	They can be represented as a matrix as 
	
	$$\begin{pmatrix}  1 & -3 & -4\\   -2 & 5 & 5 \\ 3 & 7 & 6 \end{pmatrix}$$
	
	Which has the RREF of 
	$$\begin{pmatrix}   1 & 0 & 0\\   0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$

	Which means that they are linearly independent and thus form a basis

<div style="page-break-after: always;"></div>

