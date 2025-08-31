

$(a_n)_{n\in\mathbb{N}}$

- *monotonically increasing* $\iff \forall n \in \mathbb{N}: a_n \leq a_{n+1}$
- *strictly monotonically increasing* $\iff \forall n \in \mathbb{N}: a_n < a_{n+1}$
- *monotonically decreasing* $\iff \forall n \in \mathbb{N}: a_n \geq a_{n+1}$
- *strictly monotonically decreasing* $\iff \forall n \in \mathbb{N}: a_n > a_{n+1}$


- *bounded* $\iff \exists  c\in \mathbb{R}:  \forall n\in \mathbb{N}: |a_n| \leq c$
- *unbounded* $\iff \forall  c\in \mathbb{R}:  \exists n\in \mathbb{N}: |a_n| > c$
- *bounded from above* $\iff \exists  c\in \mathbb{R}:  \forall n\in \mathbb{N}: a_n \leq c$
- *bounded from below* $\iff \exists  c\in \mathbb{R}:  \forall n\in \mathbb{N}: a_n \geq c$


- *convergent to* $a \in \mathbb{F} \iff \forall \varepsilon > 0: \exists N\in \mathbb{N}: \forall n \geq N: |a_n-a|<\varepsilon \iff \lim\limits_{n\to\infty}a_n=a$ 
- *divergent*     $\iff \forall a \in \mathbb{F}: \exists \varepsilon > 0: \forall N\in \mathbb{N}: \exists n > N: |a_n-a|\geq \varepsilon$
- *divergent to*  $\infty$ $\iff \forall a\in \mathbb{R}: \exists N \in \mathbb{N}: \forall n \geq N: a_n \geq a$
- *divergent to* $-\infty$ $\iff \forall a\in \mathbb{R}: \exists N \in \mathbb{N}: \forall n \geq N: a_n \leq a$

![[Pasted image 20240912115853.png]]



Convergent sequences are linear:
- $\lim\limits_{n\to\infty}(a_n+b_n)=\lim\limits_{n\to\infty}(a_n)+\lim\limits_{n\to\infty}(b_n)$

>[!definition] Cauchy Sequence
A sequence $(a_n)_{n\in \mathbb{N}}$ is a *cauchy sequence* $\iff \forall \varepsilon > 0: \exists N \in \mathbb{N}: \forall n,m \geq N: |a_n-a_m|<\varepsilon$


# Special Sequences
# Natural Numbers
$$a_n=n, \quad n \geq 1$$

>[!theorem] Axiom of Archimedes, aka Archimedean Property
$\forall x \in \mathbb{R}_: \exists n \in \mathbb{N}: n>x$
## Arithmetic Sequence
## Geometric Sequence
## Fibonacci Sequence
