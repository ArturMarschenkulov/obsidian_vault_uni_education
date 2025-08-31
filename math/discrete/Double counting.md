# Proposition 1.7: Double Counting
## Overview
Proposition 1.7, also known as the **double counting principle**, states that for two sets $A$ and $B$ with a binary relation $R \subset A \times B$, the following equality holds:
$\sum_{a \in A} | \{ b \in B : (a, b) \in R \} | = |R| = \sum_{b \in B} | \{ a \in A : (a, b) \in R \} |$
This proposition emphasizes that counting the relations from \(A\) to \(B\) or vice versa yields the same total.

## Application Examples
1. [Complete Graph Edges](#Example-1.8-Complete-Graph-Edges)
2. [Average Number of Divisors](#Example-1.9-Average-Number-of-Divisors)
3. [C4-free Graphs](#Example-1.10-C4-free-Graphs)

---

# Example 1.8: Complete Graph Edges
## Context
Using Proposition 1.7 to count edges in a complete graph $K_n$ with node set $[n]$ and edge set $E = \{ \{v, w\} : v, w \in V, v \neq w \}$.
## Calculation
- **Node set** ($A$) and **edge set** ($B$) are defined as $V$ and $E$ respectively.
- **Relation** ($R$) defined such that a node $a$ and an edge $b = \{b1, b2\}$ are in relation if $a \in b$.
- Resulting double count: $|R| = 2|E| = (n - 1)n$
- Conclusion: $|E| = \frac{n(n - 1)}{2}$

---

# Example 1.9: Average Number of Divisors
## Context
The average number of divisors for numbers in $[n]$ can be derived using double counting.
## Calculation
- **Relation** (\(R\)) defined such that \( (i, j) \in R \) if \(i\) divides \(j\).
- Double counting gives: $t(n) = \frac{1}{n} \sum_{i=1}^n \frac{n}{i} \approx 1 + \ln(n)$
- This shows the average number of divisors grows logarithmically with $n$.

---

# Example 1.10: C4-free Graphs
## Context
Estimating the number of edges in a graph $G = (V, E)$ that does not contain a cycle with 4 nodes (C4) using the double counting principle.
## Calculation
- **Relation** ($R$) defined such that two nodes $a$ and $b = \{b1, b2\}$ are in relation if they form a path with $a$ as the middle point.
- Using convexity and counting degrees:
  - Each node $a$ contributes $\frac{deg(a)(deg(a) - 1)}{2}$ to $|R|$.
  - Sum over all nodes provides a lower bound for \(|R|\).
- Resulting bounds: $|E| \leq n^{3/2}$


# Resources
- https://en.wikipedia.org/wiki/Double_counting_(proof_technique)
