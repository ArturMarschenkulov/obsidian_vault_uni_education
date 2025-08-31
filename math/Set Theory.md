(Mengenlehre)

> [!definition]
> A *set* is an unordered collection of distinct objects. An item that belongs to a set is said to be an *element* of the set. If $x$ is an element of the set $A$, we denote this by $x \in A$ ("$x$ is an element of $A$"). If $x$ is not an element of the set $A$, we denote this by $x \not \in A$. 


```tikz
\usepackage{tikz}
\begin{document}

\def\firstcircle{(0,0) circle (1.5cm)}
\def\secondcircle{(0:2cm) circle (1.5cm)}

\colorlet{circle edge}{blue!80}
\colorlet{circle area}{red!80}

\tikzset{filled/.style={fill=circle area, draw=circle edge, thick},
    outline/.style={draw=circle edge, thick}}

\setlength{\parskip}{5mm}
\begin{tikzpicture}
    \begin{scope}
        \clip \firstcircle;
        \fill[filled] \secondcircle;
    \end{scope}
    
    \draw[outline] \firstcircle node {$A$};
    \draw[outline] \secondcircle node {$B$};
    \node[anchor=south] at (current bounding box.north) {$A \cap B$};
\end{tikzpicture}
\end{document}
```

```tikz
\usepackage{tikz}
\begin{document}

\def\firstcircle{(0,0) circle (1.5cm)}
\def\secondcircle{(0:2cm) circle (1.5cm)}

\colorlet{circle edge}{blue!80}
\colorlet{circle area}{red!80}

\tikzset{filled/.style={fill=circle area, draw=circle edge, thick},
    outline/.style={draw=circle edge, thick}}

\setlength{\parskip}{5mm}
\begin{tikzpicture}
    \begin{scope}
        \fill[filled] \firstcircle;
        \fill[filled] \secondcircle;
    \end{scope}

    \draw[outline] \firstcircle node {$A$};
    \draw[outline] \secondcircle node {$B$};
    \node[anchor=south] at (current bounding box.north) {$A \cup B$};
\end{tikzpicture}
\end{document}
```
$$A\cup B:= \set{x:x\in A \lor B}$$
$$A\cap B:= \set{x:x\in A \land B}$$

Cartesian product: $$A \times B=\set{(a, b) : a \in A \land b \in B}$$
$$A\subseteq B \iff \forall a : (a\in A \implies a \in B)$$
Let $x\in \mathbb{F}$. The $\varepsilon$-neighborhood of $x$ is: $$B_\varepsilon(x)=\set{y \in \mathbb{F}: |x - y|< \varepsilon}$$
Let set $M \subset \mathbb{F}$.  $M$ is the neighborhood of $x$ $\iff \exists \varepsilon > 0: B_\varepsilon(x) \subset  M$.

Let $M \subset \mathbb{F}$. Then $M$ is:
1) *bounded* $\iff \exists c\in \mathbb{R}: \forall x\in M: |x| \leq c$ 
2) *open* $\iff \forall x \in M: B_\varepsilon(x) \subset  M$


$$\set{x \in C:\exists \varepsilon>0:B_\varepsilon(x) \subset C}$$



$H(x) = b_n \, ^n x + b_{n-1} \, ^{n-1} x + \dots + b_2 \, ^2 x + b_1 x + b_0,$

Axiom of regularity:
$\forall x:(x\neq \varnothing \implies \exists y : (y \in x \land y \cap x = \varnothing))$

Let $M \subseteq \mathbb{R}$
- $b \in \mathbb{R}$ is an *upper bound* $\iff \exists b \in \mathbb{R} : \forall x \in M: x\leq b$
- $b \in \mathbb{R}$ is a *lower bound* $\iff \exists b \in \mathbb{R} : \forall x \in M: x \geq b$
- $M$ has an *upper bound* $\implies$ $M$ is *bounded from above*
- $M$ has a *lower bound* $\implies$ $M$ is *bounded from below*
- $M$ has an *upper bound* and a *lower bound* $\implies$ $M$ is *bounded*
- $d \in M$ is *maximal element* $\iff \forall x \in M: x\leq b$
- $d \in M$ is *minimal element* $\iff \forall x \in M: x\geq b$



# Multiset

A
# Misc

arbitrarily small  : $\forall \varepsilon > 0: \exists x \in \mathbb{R}:|x| \leq \varepsilon: P(x)$
sufficiently small: $\exists \varepsilon > 0: \forall x \in \mathbb{R}: |x| \leq \varepsilon: P(x)$

arbitrarily   large: $\forall a \in \mathbb{R}: \exists x \in \mathbb{R}: x \geq a: P(x)$
sufficiently large: $\exists a \in \mathbb{R}: \forall x \in \mathbb{R}: x \leq a: P(x)$


