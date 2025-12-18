
big oh limit rules

$\lim_{n \to \infty} \frac{h(n)}{f(n)}$

$lim = \infty \implies h\in \Omega(f), \omega(f)$
$lim = k \implies h \in \Theta(f)$
$lim = 0 \implies h \in O(f), o(f)$

![[Pasted image 20251218102840.png]]

Loop invariant

initialization
maintenance
term 1# = does it end
term 2# = when it ends is it correct

recurrence tree

running time is amount of levels * cost per level

i.e if merge sort n per level k = log(n) levels


Master Theorem
The Master Theorem applies to recurrences of the following form:
T (n) = aT (n/b) + f (n)
where a ≥ 1 and b > 1 are constants and f (n) is an asymptotically positive function.
There are 3 cases:
1. If f (n) = O(nlogb a−) for some constant  > 0, then T (n) = Θ(nlogb a).
2. If f (n) = Θ(nlogb a logk n) with1 k ≥ 0, then T (n) = Θ(nlogb a logk+1 n).
3. If f (n) = Ω(nlogb a+) with  > 0, and f (n) satisfies the regularity condition, then T (n) = Θ(f (n)).
Regularity condition: af (n/b) ≤ cf (n) for some constant c < 1 and all sufficiently large n.

arr to tree 
leftchild(i) = 2i
rightchild(i) = 2i+1
parent(i) = floor(i/2)

almost heap = root not correct
max-heapify turns almost heap to heap

go from bottom of tree to top heapifiying along the way to fully heap it

![[Pasted image 20251218111117.png]]

avl tree rotations

greedy substitution property - any optimal decision to problem can be altered to become the greedy choice without being less optimal

optimal substructure - sub problems are the same as the whole

exponentiation by halving