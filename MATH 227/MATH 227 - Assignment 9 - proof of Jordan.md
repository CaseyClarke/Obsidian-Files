# Question 1

$m_A(x) = (x-0)^2(x-4)^2$

{{ENDQUESTION}}

# Question 2

$$\begin{pmatrix} 4 & 1 & 0 & 0 \\ 0 & 4 &1 & 0  \\ 0 & 0 & 4 & 0 \\ 0 & 0 & 0 & 4\end{pmatrix}$$
{{ENDQUESTION}}

# Question 3

$A^5 -6A^4+2A^3 - A^2 + A + I \mod (-A^3 + A^2) = -A^2 +5A + 3$

{{ENDQUESTION}}

# Question 4

(a)

- By the definition of generalized eigen space we know that there exists some $l$ such that 
- $(A-\lambda I)^lv = 0 \land (A-\lambda I)^{l-1}v \neq 0$
- This shows that there is an $l$ such that $(A-\lambda I)^{l-1}v \neq 0$ (non-zero)

- $Let \; k \text{ be the smallest positive integer such that } (A-\lambda I)^kv = 0 \land (A-\lambda I)^{k-1}v \neq 0$ 
- $Let \; x = (A-\lambda I)^{k-1}v \neq 0$

- $(A-\lambda I)x = (A-\lambda I)(A-\lambda I)^{k-1}x = (A-\lambda I)^{k} = 0$
- $(A-\lambda I)x = 0 \implies x \in E_\lambda$

- So for the integer $l-1$ that follows the rule  $(A-\lambda I)^lv = 0 \land (A-\lambda I)^{l-1}v \neq 0$
- both properties hold

(b)

- If $\lambda$ is not an eigenvalue $E_\lambda = \{0\}$ 
- Suppose for contradition that $GE_\lambda(A)$ contains some non-zero vector, from part (a) we know that if we left multiply that non-zero vector by $(A-\lambda I)$ some ($l-1$) amout of times we get a vector in $E_\lambda$ but that is a contradiction since $E_\lambda = \{0\}$ thus $GE_\lambda(A) = \{0\}$

(c)

- $m_A(x) = (x-\lambda)^kp(x)$
- $m_A(A) = (A-\lambda I)^kp(A) = 0$
- 
- we know that $p(A) \neq 0$ as 
- $p(A) = 0 \implies m_A(x) \; | \; p(x)$ which would imply that $(x-\lambda)^k \;| \; 1$ but that is not a polynomial so contradiction
- meaning that $vp(A) \neq 0$ for some $v \in A$  since $(nonzero)(nonzero) = (nonzero)$
- $m_A(A) = (A-\lambda)^k(vp(A)) = 0$ since we have shown that $(A-\lambda)^k = 0$
- $w = vp(A)$
- $m_A(A) = (A - \lambda)^kw = 0$
- $w \in GE_\lambda(A)$ by definition
- by part (a) we know that this implies that $w \in E_\lambda$

{{ENDQUESTION}}

# Question 5

(a)

- $v \in GE_\lambda(A) \implies (A-\lambda I)^kv = 0$
- $(A-\lambda I)^k(p(A)v)$
- $p(A)(A-\lambda I)^Kv = p(A)0 = 0$
- $\implies p(A)v \in GE_\lambda(A)$
- 
(b)

- We know that $Av = \lambda v$ by definition and that $A^nv = \lambda^n v$ by repeatedly applying this fact
- $p(A)v = (a_0Iv + a_1Av + a_2A^2v + \dots + a_nA^nv)$
- $p(A)v = (a_0v + a_1\lambda v + a_2\lambda^2v + \dots + a_n\lambda^nv)$
- $p(A)v = p(\lambda)v$

{{ENDQUESTION}}

# Question 6

(a)

- Assume for contradiction that $(A-\mu I)^mv = 0$
- $let \; p(x) = (x - \mu I) ^m$
- $p(A)v = 0$
- but we know that $p(A)v = p(\lambda)v \in GE_\lambda(A)$
- but then $p(A)v \neq 0$ since $0 \notin GE_\lambda(A)$
- contradiction

(b)

$$\frac{1}{m_A(x)} = \sum_{i = 1}^k \frac{a_i(x)}{(x-\lambda_i I)^{l_i}}$$
$$m_A(x)\frac{1}{m_A(x)} = \sum_{i = 1}^k m_A(x)\frac{a_i(x)}{(x-\lambda_i I)^{l_i}}$$
$$1(v) = \sum_{i = 1}^k m_A(x)\frac{a_i(x)}{(x-\lambda_i I)^{l_i}}(v)$$
$$v = \sum_{i = 1}^k m_A(x)\frac{a_i(x)}{(x-\lambda_i I)^{l_i}}v$$
$$v_i = m_A(x)\frac{a_i(x)}{(x-\lambda_i I)^{l_i}}v$$

$$v = \sum_{i = 1}^k v_i$$
now we just need to verify that each $v_i \in GE_\lambda(A)$

$$v_i = m_A(x)\frac{a_i(x)}{(x-\lambda_i I)^{l_i}}v$$
