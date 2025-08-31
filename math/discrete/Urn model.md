
[[Binomial coefficient]]
[[Factorial]]

# Combi
Let $n, k \in \mathbb{N}_0$ and $M$ a set where $|M|=n$.
## Ordered samples with Replacement
$M^k=\{(c_1, \dots, c_k): c_i \in M, \forall i \in [k]\}$

Let $k$ be the amount of experiments and each experiment has $n$ outcomes.
$$|M^k|=n^k$$
## Ordered samples without Replacement
$$M^\underline{k}=\{(c_1, \dots, c_k): c_i \in M, \forall i \in [k], c_i \neq c_j, \forall i \neq \in [k] \}$$

$$|M^\underline{k}|=\prod_{i=0}^{k-1}=:n^\underline{k}$$

$n^\underline{k}$ is also called the *falling factorial* and can be expressed as: $$n^\underline{k}=\frac{n!}{(n-k)!}$$

## Unordered samples without Replacement
$$\binom{M}{k}:=\{\{c_1, \dots, c_k\}: c_i\in M, \forall i \in [k], c_i \neq c_j, \forall i \neq j \in [k]\}$$

$$\left|\binom{M}{k}\right|=\frac{n^\underline{k}}{k!}=\frac{n!}{k!(n-k)!}=\binom{n}{k}$$
## Unordered samples with Replacement
Let $\phi: M \to \mathbb{N}_0$.
$$\genfrac{\langle}{\rangle}{0pt}{}{M}{k}:=\set{(M, \phi):\sum_{m \in M} \phi(m)=k}$$

$$\frac{(n+k-1)!}{k!(n-1)!}=\binom{n+k-1}{k}$$
[[Factorial]] [[Binomial coefficient]]

# Exercises
>[!example]
Consider a room with a rectangular floor plan where each of the $4$ walls is to be painted. You have $7$ colors to choose from. Determine the number of possible ways to paint all the walls under the following conditions:
>- **a) Each wall can be painted in any arbitrary color.** $$
\text{Total possibilities} = 7^4 \quad (\text{Product Rule})$$
>- **b) No two walls may have the same color.** $$\text{Total possibilities} = 7^\underline{4} = 7 \times 6 \times 5 \times 4$$
>- **c) Exactly three different colors must be used.** $$\text{Total possibilities} = \binom{4}{2} \cdot 7^3$$


# Resources
- https://www.probabilitycourse.com/chapter2/2_1_0_counting.php