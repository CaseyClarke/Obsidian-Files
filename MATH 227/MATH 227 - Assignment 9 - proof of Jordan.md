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

- 
- 