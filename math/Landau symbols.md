[[Limit]]


- $f(n) \in O(g(n)) \iff \exists k > 0: \exists n_0 \in \mathbb{N}: \forall n >n_0:|f(n)|\leq k \cdot | g(n)|$. $\limsup\limits_{n \to \infty}\frac{f(n)}{g(n)}<\infty$
- $f(n) \in \Omega(g(n)) \iff \exists k > 0: \exists n_0 \in \mathbb{N}: \forall n >n_0: |f(n)|\geq k \cdot | g(n)|$. $\liminf\limits_{n \to \infty}\frac{f(n)}{g(n)}>\infty$
- $f(n) \in o(g(n)) \iff \forall k > 0: \exists n_0 \in \mathbb{N}: \forall n >n_0:|f(n)|\leq k \cdot | g(n)|$. $\lim\limits_{n \to \infty}\frac{f(n)}{g(n)}=0$
- $f(n) \in \omega(g(n)) \iff \forall k > 0: \exists n_0 \in \mathbb{N}: \forall n >n_0:|f(n)| > k \cdot | g(n)|$. $\lim\limits_{n \to \infty}\frac{f(n)}{g(n)}=\infty$
- $f(n) \sim g(n)$ . $\lim\limits_{n\to\infty} \frac{f(n)}{g(n)}=1$


$\forall n,k \in \mathbb{N}: k < n$
- $(\frac{n}{e})^n \leq n! \leq n^n$
- $(\frac{n}{k})^k \leq \binom{n}{k} \leq (\frac{en}{k})^k$
