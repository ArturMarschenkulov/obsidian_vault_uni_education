
>[!definition]
Let $X$ and $Y$ be two sets. The *binary relation* $R$ is also defined as a triple $R=(X, Y, G)$ with $G\subseteq X \times Y$.  A $x \in X$ and $y\in Y$ are only related if $(x, y) \in G$, this is also denoted as $xRy$.

>[!note]
>While using the triplet $R=(X, Y, G)$ is the more rigorous way to define it. However $R$ is also frequently simply defined as $R\subseteq X \times Y$. Also $xRy\iff (x, y) \in R$.

>[!definition] Domain
The *domain* of $R$ is defined as: $$\text{Dom}(R):=X$$

>[!definition] Codomain
The *codomain* of $R$ is defined as: $$\text{Cdm}(R):=Y$$

>[!definition] Image
The *image* of $R$ is defined as: $$\text{Img}(R):= R[S] = \{y\in Y: \exists x \in X: xRy\}$$

>[!definition] Preimage
The *preimage* of $R$ is defined as: $$\text{Img}^{-1}(R):= R^{-1}[S] = \{x\in X: \exists y \in Y: xRy\}$$



>[!theorem]
A binary relation $xRy$ is *left-total* $\iff$: $$\forall x \in X: \exists y \in Y: xRy$$

>[!theorem]
A binary relation $xRy$ is *right-total*/*surjective* $\iff$: $$\forall y \in Y: \exists x \in X: xRy$$

>[!theorem] Functional
A binary relation $xRy$ is *functional*/*right-unique*/*many-to-one*, $\iff$:
$$\forall x \in X: \forall y_1, y_2 \in Y: x R y_1 \land xRy_2 \implies y_1=y_2$$
A *functional binary relationship* is more commonly known as a *mapping* or even more commonly as a *function*.




A binary relation $xRy$ is *injective*/*left-unique*/*one-to-many* $\iff$: $$\forall x_1, x_2 \in X, y \in Y, x_1Ry \land x_2Ry \implies x_1=x_2$$

A binary relation $xRy$ is *one-to-one* $\iff$ it is *injective*/*one-to-many*/*right-unique* and *functional*/*many-to-one*/*left-unique*.

A binary relation $xRy$ is *many-to-many* $\iff$ it is neither *many-to-one* nor *one-to-many*.

A binary relation $xRy$ is *bijective* $\iff$ it is *injective* and *surjective*.



Part of [[Set Theory]]

