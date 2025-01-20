# Question 2

(a)

We need to show that $\vec{u} \sim \vec{v} \implies f(\vec{u}) = f(\vec{v}) \quad \forall \; \vec{u}, \vec{v} \in \mathbb{C}^3/\sim$
However this is not true for the example relation given in the question

$\vec{u} = (-i, i + 1, i -1), \quad \vec{v} = (0,0,0)$ 
$\vec{u} \sim \vec{v}$
$f(\vec{u}) = (-i, i + 1)$
$f(\vec{v}) = (0,0)$
$(-i, i + 1) \neq (0,0)$

$\therefore \; f$ is not well defined over $\mathbb{C}^3/\sim$

(b)

We need to show that $p(x) \sim q(x) \implies f(p(x)) = f(q(x)) \quad \forall \; p(x), q(x) \in \mathbb{Q}[x]/\sim$
$\implies (2p(1) + 3p(2) - 5p(3)) = (2q(1) + 3q(2) - 5q(3)) \text{ and } (p(1) - p(-1)) = (q(1) - q(-1))$
Given that $p(x) \sim q(x)$ we know that from the properties of derivatives $q(x) = p(x) + c$ for some rational value of c 

$(2p(1) + 3p(2) - 5p(3)) = (2q(1) + 3q(2) - 5q(3))$:
$(2p(1) + 3p(2) - 5p(3)) = (2(p(1) + c) + 3(p(2) + c) - 5(p(3) + c))$
$(2p(1) + 3p(2) - 5p(3)) = (2p(1) + 2c + 3p(2) + 3c - 5p(3) + -5c)$
$(2p(1) + 3p(2) - 5p(3)) = (2p(1) + 3p(2) - 5p(3))$
$LHS = RHS$

$(p(1) - p(-1)) = (q(1) - q(-1))$:
$(p(1) - p(-1)) = (p(1) + c -(p(-1) + c)$
$(p(1) - p(-1)) = (p(1) - p(-1))$
$LHS = RHS$

$\therefore f$ is well defined over $\mathbb{Q}[x]/\sim$