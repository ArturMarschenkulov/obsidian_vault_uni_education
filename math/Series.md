


[[Sequence]]


> [!definition] Infinite Series
> 
> Consider the sequence of numbers
> $a_0, a_1, a_2, a_3, \ldots$ from $\mathbb{R}$. Adding these elements sequentially generates another sequence:
> $s_0 = a_0,$
> $s_1 = a_0 + a_1,$
> $s_2 = a_0 + a_1 + a_2,$
> $\ldots$
> which is called an *infinite series*. This infinite series is symbolically represented by:
> $\sum_{k=0}^{\infty} a_k = a_0 + a_1 + a_2 + a_3 + \ldots$
> The terms $a_n$ of the sequence $(a_n)$ are also called the terms of the series $\sum_{k=0}^{\infty} a_k$. The index of summation $k$ can be replaced by any other letter. The sums:
> $s_n = \sum_{k=0}^n a_k \tag{3.1}$
> are called the partial sums of the series. The smallest value of the summation index need not be 0; if $p \in \mathbb{Z}$, then
> $\sum_{k=p}^{\infty} a_k$
> is understood as the sequence of partial sums $(s_n^0)$ with
> $s_0^0 = a_p,$
> $s_0^1 = a_p + a_{p+1},$
> $s_0^2 = a_p + a_{p+1} + a_{p+2},$
> $\ldots$
> Setting $b_k = a_{k+p}$ (for $k = 0, 1, 2, \ldots$) leads to: $\sum_{k=p}^{\infty} a_k = \sum_{k=0}^{\infty} b_k$, thus shifting the series from a starting index of $p$ to a starting index of 0. From an infinite series, one can extract any arbitrary (finite) partial sum; that is, for $p \in \mathbb{N}$:
> $\sum_{k=0}^{\infty} a_k = a_0 + a_1 + \ldots + a_{p-1} + \sum_{k=p}^{\infty} a_k.$
> 
> As an example, consider the specific geometric series:
> $\sum_{k=0}^{\infty} \frac{1}{2^k} = 1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \ldots$

>[!theorem] Cauchy Criterion
Let $\{a_k\}$ be a sequence in a field $\mathbb{F}$. The series $\sum_{k=1}^\infty a_k$ converges if and only if for every $\epsilon > 0$, there exists an integer $N$ such that for all integers $n \geq m \geq N$, the inequality
$$
\left| \sum_{k=m}^n a_k \right| < \epsilon
$$
holds.

> [!theorem] Cauchy Series
> Let $S$ be a series, it is a *Cauchy Series*  $:= \forall \varepsilon > 0, \exists N \in \mathbb{N}, \forall n \geq N, \left| \sum_{k=m}^n a_k \right| < \epsilon$ 



>[!theorem] Cauchy product
Let $A=\sum_{k=n_0}^\infty a_k$ and $B=\sum_{k=n_1}^\infty b_k$ be two series in $\mathbb{F}$. Then $$AB=\sum_{k=n_0+n_1}^\infty c_k$$ with $c_k=\sum_{l=n_0}^{k-n_1}a_lb_{k-l}$, or $$AB=\sum_{k=n_0+n_1}^\infty \left( \sum_{l=n_0}^{k-n_1}a_lb_{k-l} \right)$$ 

> [!definition] Absolute Convergence of a Series
> A series $\sum_{k=0}^\infty a_k$ is said to be **absolutely convergent** if the series of the absolute values of its terms converges, that is, if $\sum_{k=0}^\infty |a_k|$ is convergent.

>[!theorem] 
>If a *series* $\sum_{n=1}^\infty a_n$ converges, then the *sequence* $(a_n)$ converges to $0$.



Root criterion
The $\sum^\infty_{k=0}a_k$ is *absolute convergent* $\iff$ $\exists c \in R_{>0}: \forall k: c < 1: \sqrt[k]{|a_k|} \leq c$.