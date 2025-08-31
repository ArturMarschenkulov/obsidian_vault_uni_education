This is a first stop for all things related to combinatorics in uni.

>[!definition] 
>Let $\mathbb{N}=\{1, 2, 3, \dots\}$, that is only positive natural numbers. Let $n \in \mathbb{N}$. Then $[n] = \{1, 2, \dots, n\}$


> [!theorem] Counting by Bijection (Zählen durch Bijektion)
> Let $A$ and $B$ be finite sets and $f:A \to B$ a mapping. Then the following holds:
> - If $f$ is bijective, then $|A|=|B|$
> - If $|A| = |B|$, then $f$ injective $\iff$ $f$ surjective $\iff$ $f$ bijective


> [!theorem] [[Double Counting]] (doppeltes Abzählen)
> Let $A$ and $B$ be two sets and $R \subset A \times B$ a binary relation. Then, the following holds:
> 
> $
> \sum_{a \in A} | \{b \in B : (a, b) \in R\} | = |R| = \sum_{b \in B} | \{a \in A : (a, b) \in R\} |
> $

> [!theorem] Average Number of Divisors (Durchschnittliche Anzahl Teiler)
> We can use the principle of double counting to determine the average number of divisors of all numbers in $[n]$. Specifically: For $j \in N$, let $t(j)$ be the number of natural divisors of $j$. We are now interested in the average number of divisors, given by:
> $t(n) := \frac{1}{n} \sum_{j=1}^n t(j)$

> [!theorem] Pigeonhole Principle (Schubfachprinzip).
> Given finite sets $M$ and $S$, and a mapping
> $f : M → S$. Then there exists an $s \in S$ such that $|f^{-1}(s)| ≥ \frac{|M|}{|S|}$.


>[!example] Pigeonhole Principle Example 1
Let $n \in \mathbb{N}$ and $X \subset [2n]$ be a subset of size $|X|=n + 1$. Then there exist two distinct elements $x_1, x_2 \in X$ such that $x_1$ is a divisor of $x_2$.


**Proof:**  
Define a function $f: X \rightarrow U$ as $f(x) = \text{the largest odd divisor of } x$. Note, $|X|=n+1$ and $|U|=n$.By the pigeonhole principle, there exists a $y \in U$ such that $|f^{-1}(y)| \geq \lceil\frac{|X|}{|U|} \rceil = \lceil\frac{n + 1}{n} \rceil = 2$. Therefore, there are two elements $x_1, x_2 \in X$ with $f(x_1) = f(x_2)$. Without loss of generality, assume $x_1 < x_2$ and $f(x_1) = f(x_2) = y$. Then, there exist $a, b \in \mathbb{N}_0$ with $a < b$ such that $x_1 = 2^a y$ and $x_2 = 2^b y$. Hence, $x_1$ is a divisor of $x_2$.

>[!example] Pigeonhole Principle Example 2 (Erdős-Szekeres)
Every finite sequence $(a_1, a_2, \ldots, a_{n^2})$ of $n^2$ pairwise distinct real numbers contains a monotonic subsequence of length $n$.
**Proof:**
Let $K$ be the length of the longest monotonic subsequence. Suppose for contradiction that $K < n$. Consider the mapping $f : [n^2] \rightarrow [K]^2$ defined by $i \mapsto (f_i, s_i)$, where $f_i$ denotes the length of the longest decreasing subsequence ending in $a_i$, and $s_i$ the length of the longest increasing subsequence ending in $a_i$. By the pigeonhole principle, there must exist indices $i < j$ in $[n^2]$ such that $f(i) = f(j)$. Thus, we have $(f_i, s_i) = (f_j, s_j)$. However, $f_j > f_i$ if $a_j < a_i$ and $s_j > s_i$ if $a_j > a_i$. Therefore, $(f_i, s_i) \neq (f_j, s_j)$, leading to a contradiction.



> [!theorem]
> **Theorem 2.4** Let $A(x) = \sum_{n=0}^\infty a_n x^n$ and $B(x) = \sum_{n=0}^\infty b_n x^n$ be power series convergent in $x \in \mathbb{R}$. Let $\lambda, q \in \mathbb{R}$.
> 
> a) **Addition and Scalar Multiplication:** The series $A(x) + B(x)$ and $\lambda A(x)$ are also convergent in $x$, with:
> $
> A(x) + B(x) = \sum_{n=0}^\infty (a_n + b_n) x^n
> $
> $
> \lambda A(x) = \sum_{n=0}^\infty (\lambda a_n) x^n
> $
> 
> b) **Multiplication (Cauchy Product):** If
> $
> C(x) = \sum_{n=0}^\infty c_n x^n \quad \text{where} \quad c_n = \sum_{k=0}^n a_k b_{n-k} \text{ for all } n \in \mathbb{N}_0,
> $
> then $C(x)$ is also convergent in $x$, and it holds that $C(x) = A(x)B(x)$. Explicitly:
> $
> (a_0 + a_1 x + a_2 x^2 + \ldots)(b_0 + b_1 x + b_2 x^2 + \ldots) = a_0 b_0 + (a_0 b_1 + a_1 b_0) x + (a_0 b_2 + a_1 b_1 + a_2 b_0) x^2 + \ldots
> $
> 
> c) **Differentiation:** $A(x)$ is differentiable within the interior of its convergence range, the derivative $A'(x)$ has the same radius of convergence as $A(x)$, and it holds that:
> $
> A'(x) = \sum_{n=1}^\infty n a_n x^{n-1} = \sum_{n=0}^\infty (n+1) a_{n+1} x^n.
> $
> 
> d) **Geometric Series:** Let $q \in \mathbb{R}$ be arbitrary. For all $x \in \mathbb{R}$ with $|x| < |q|^{-1}$, it holds that:
> $
> \sum_{n=0}^\infty q^n x^n = \frac{1}{1 - qx}
> $
> 
> e) **k-th Derivative:** Differentiating $\sum_{n=0}^\infty x^n = \frac{1}{1-x}$ $k$ times yields:
> $
> \sum_{n=k}^\infty n(n-1) \cdots (n-k+1) x^{n-k} = \frac{k!}{(1-x)^{k+1}}
> $
> and therefore, for all $k \in \mathbb{N}_0$, $x \in \mathbb{R}$ with $|x| < 1$:
> $
> \sum_{n=k}^\infty \binom{n}{k} x^{n-k} = \frac{x^k}{(1-x)^{k+1}}
> $


[[Inclusion-exclusion-principle]]