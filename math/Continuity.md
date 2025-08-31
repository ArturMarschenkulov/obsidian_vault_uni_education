


$f$ is *continuous at x* $\iff \lim\limits_{y\to x}$ exists and

>[!theorem] Uniform continuity
Let $I \subseteq \mathbb{R}$ be a *real interval*. A function $f: I \to \mathbb{R}$ is said to be *uniformly continuous* on $I$ $\iff$: $$\forall \epsilon \in \mathbb{R}_{\geq0}: \exists \delta \in \mathbb{R}_{\geq0}:(\forall x, y \in I: |x-y|<\delta \implies|f(x)-f(y)|<\epsilon)$$
Let $d(x, y)=|x - y|$ then the same can be expressed as :
$$\forall \epsilon>0: \exists \delta>0:(\forall x, y \in I: d(x,y)<\delta \implies d(f(x),f(y))<\epsilon)$$

>[!theorem] Absolute continuity
Let $I \subseteq \mathbb{R}$ be a *real interval*. A function $f: I \to \mathbb{R}$ is said to be *absolutely continuous* on $I$ $\iff$: 
$$\forall \epsilon \in \mathbb{R}_{\geq0}: \exists \delta \in \mathbb{R}_{\geq0}: (\forall \{(x_k, y_k)\}_{k=1}^n \subseteq I \times I \text{ finite set of non-overlapping intervals }: \sum_{k=1}^n |y_k - x_k| < \delta \implies \sum_{k=1}^n |f(y_k) - f(x_k)| < \epsilon)$$


>[!theorem] Lipschitz Continuity
Let $A \subseteq \mathbb{R}$.
$\exists K \in \mathbb{R}_{\geq0}: \forall x, y \in I: |f(x) - f(y)| \leq K |x - y|$
$\exists K \in \mathbb{R}_{\geq0}: \forall x, y \in I: d(f(x), f(y)) \leq K d(x, y)$
$\exists K \geq0: \forall x, y \in I: |f(x) - f(y)| \leq K |x - y|$

The idea is that