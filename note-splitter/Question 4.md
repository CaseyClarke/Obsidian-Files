# Question 4

(a)

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

(b) (cardinality)

$g \sim g' \implies g^{-1}g' \in H \implies g' = gh \quad h \in H$
Meaning that 
$\forall h \in H \; gh \in [g] \quad \text{ Where } [g] \text{ is some eqivalence class with a representative } g$
Define $F : H \rightarrow [g] \quad F(h) = gh$
One-to-one-ness of $F$:
- $gh_1, \; gh_2 \in [g]$
- Assume $gh_1 = gh_2$
- $g^{-1}gh_1 = g^{-1}gh_2 \implies h_1 = h_2$
Onto-ness of $F$:
- F is onto from the definition of $[g]$
We now have a bijection that maps from $H$ to $[g]$ meaning that we can say that $H$ and $[g]$ have the same size

(c)

Since we know that the equivalence relation $g \sim g' \iff g^{-1}g \in H$ partitions G into some number of partitions of size $H$ we can say that $size(G) = n \times size(H) \text{ for some } n \in \mathbb{N}$
This is the definition of evenly dividing