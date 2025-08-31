

Relates to [[Set Theory]]

A *magma* is an algebraic structure $(G,\circ)$ with the following properties:
- $\forall a, b \in G: a \circ b \in G$ (Closure)

A *semigroup* is an algebraic structure $(G,\circ)$ with the following properties:
- $\forall a, b \in G: a \circ b \in G$ (Closure)
- $\forall a, b, c \in G: a \circ (b \circ c) = (a \circ b) \circ c$ (Associativity)

A *monoid* is an algebraic structure $(G,\circ)$ with the following properties:
- $\forall a, b \in G: a \circ b \in G$ (Closure)
- $\forall a, b, c \in G: a \circ (b \circ c) = (a \circ b) \circ c$ (Associativity)
- $\exists e \in G: \forall a \in G: e \circ a = a = a \circ e$ (Identity)

A *group* is an algebraic structure $(G,\circ)$ with the following properties:
- $\forall a, b \in G: a \circ b \in G$ (Closure)
- $\forall a, b, c \in G: a \circ (b \circ c) = (a \circ b) \circ c$ (Associativity)
- $\exists e \in G: \forall a \in G: e \circ a = a = a \circ e$ (Identity)
- $\forall a \in G: \exists b \in G: a \circ b = e = b \circ a$ (Inverse)

An *abelian group* is an algebraic structure $(G,\circ)$ with the following properties:
- $\forall a, b \in G: a \circ b \in G$ (Closure)
- $\forall a, b, c \in G: a \circ (b \circ c) = (a \circ b) \circ c$ (Associativity)
- $\exists e \in G: \forall a \in G: e \circ a = a = a \circ e$ (Identity)
- $\forall a \in G: \exists b \in G: a \circ b = e = b \circ a$ (Inverse)
- $\forall a, b \in G : a \circ b = b \circ a$ (Commutativity)


A *field* is $(F, +, \times) \iff$:
- $(F, +)$ is an abelian group
- $(F*, \times)$ is an abelian group with $F*=F \setminus \set{0_F}$
- operation $\times$ distributes over $+$


A *vector space* $(V, +, \cdot)$:
- 