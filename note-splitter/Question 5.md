# Question 5

(a)

(i)

Composition preserves linearity
$(S \circ T)^{-1} = T^{-1} \circ S^{-1}$
$(S \circ T)^{-1}(V) \circ  (T^{-1} \circ S^{-1})(V) = S(T(T^{-1}(S^{-1}(V)))) = V$
$(T^{-1} \circ S^{-1})(V) \circ (S \circ T)^{-1}(V) = T^{-1}(S^{-1}(S(T(V)))) = V$
$\therefore$ It is closed as the properties of linearity and invertibility hold

(ii)

$(S \circ T) \circ R = S \circ (T \circ R)$
$S(T(V) \circ R = S \circ (T(R(V)$
$S(T(R(V) = S(T(R(V)$

(iii)

$I(V) = V$
Which is trivially linear and is invertible as $I^{-1} = I$ 

(iv)	

Any element has an inverse by definition and from the properties of function composition we know $(T \circ T^{-1})(V) = (T^{-1} \circ T)(V) = V = I(V) \quad \forall \; T \in IL(V)$

(b)

(i)

From the previous question we know that function composition forms a group over $IL(V)$ so this is automatically satisfied as $f$ is just the composition of functions

(ii)

$f(T \circ T') = S \circ (T \circ T') \circ S^{-1}$
$f(T) \circ f(T') = (S \circ T \circ S^{-1}) \circ (S \circ T' \circ S^{-1})$
$f(T) \circ f(T') = (S \circ T \circ T' \circ S^{-1}) = S \circ (T \circ T') \circ S^{-1}$
$f(T) \circ f(T') = f(T \circ T')$

(iii)

$f^{-1}(T) = S^{-1} \circ T \circ S$
$f(T) \circ f^{-1}(T) = f^{-1}(T) \circ f(T) = T$

Since $f^{-1}$ is simply a string of function compositions it preserves the group structure meaning that (i), (ii), and (iii) are all automatically satisfied making it a homomorphism as well