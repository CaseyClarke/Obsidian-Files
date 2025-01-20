# Question 3

(a)

A vector space is isomorphic to another if their dimensions are equal
$dim(V) = n$
$dim(V \oplus V) = 2n$
$dim(V) = dim(V \oplus V) \implies n = 2n$
$n = 0$ is the only case in which this holds which shows that this is only true for the trivial vector space

(b)

Isomorphism = bijection = onto and one-to-one

Linear:
- $T((p+ p')(x), (q + q')(x))$
- $\Rightarrow (p+ p')(x^2) + x(q + q')(x^2)$
- $\Rightarrow p(x^2) + p'(x^2) + xq(x^2) + xq'(x^2)$
- $\Rightarrow p(x^2) + xq(x^2) + p'(x^2) + xq'(x^2)$
- $\Rightarrow T(p(x),q(x)) + T(p'(x),q'(x))$

- $T(c(p(x),q(x))$
- $\Rightarrow cp(x^2) +cxq(x^2)$
- $\Rightarrow c(p(x^2 + xq(x^2)$
- $\Rightarrow cT(p(x),q(x))$

Onto:
- T can be split up into to components, $p(x^2)$ and $xq(x^2)$ 
- these can be represented as $x^{2k}$ and $x^{2x+1} \quad \forall \; k \in \mathbb{N}$  respectively 
- $x^{2k}$ can be used to represent any polynomial with only even degrees
- $x^{2k+1}$ can be used to represent any polynomial with only odd degrees
- Thus adding them together as such  $x^{2k} + x^{2k+1} = T(p(x), q(x)) = p(x^2) + xq(x^2)$ we can get polynomials with any degree meaning that the codomain is $Poly(\mathbb{F})$ which means that T is onto

One-to-one:
- $T(p(x), q(x)) = T(p'(x),q'(x))$
- $\Rightarrow p(x^2) + xq(x^2) = p'(x^2) + xq'(x^2)$
- $\Rightarrow p(x) = p'(x) \text{ and } q(x) = q'(x)$


(c)

$Poly(\mathbb{F})$ is not finite dimensional so the previous statement does not apply