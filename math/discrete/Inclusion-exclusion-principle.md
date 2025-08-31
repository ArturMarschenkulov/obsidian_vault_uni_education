


$|A \cup B|=|A|+|B|-|A \cap B|$

$|A \cup B \cup C|=|A|+|B|+|C|-|A \cap B|- |A\cap C|- |B \cap C|+ |A \cap B \cap C|$

Let $A_1, A_2, A_3, \dots, A_n$.

$$\sum_{i=1}^nf(A_i)-\sum_{1\leq i < j \leq n}(A_i\cap A_j)$$
$$\left|\bigcup_{i=1}^n A_i\right|=\sum_{k=1}^n \left((-1)^{k-1} \sum_{\substack{I \subseteq [n] \\ |I| = k}} \left|\bigcap_{j\in I} A_{j}\right|\right),\nonumber$$


$$\left|\bigcap_{i=1}^n A_i^c\right|=|S|+\sum_{k=1}^n (-1)^k \sum \left|\bigcap_{j=1}^k A_{i_j}\right|,\nonumber$$


The formula you've provided beautifully captures the inclusion-exclusion principle using summation notation. To express it in a way that emphasizes "big iteration notation," which typically aims to highlight the recursive or iterative nature of the calculation across subsets of indices, we can utilize the set notation more prominently along with a structured iterative expression. Here’s a structured way to present it:

$$
\left|\bigcup_{i=1}^n A_i\right| = \sum_{k=1}^n (-1)^{k-1} \left(\sum_{\substack{I \subseteq [n] \\ |I| = k}} \left|\bigcap_{j \in I} A_j\right|\right)
$$

Here's a breakdown of the expression:

1. **Outer Summation**: \( \sum_{k=1}^n \) iterates over the sizes of the subsets \( I \) that will be considered. The term \( (-1)^{k-1} \) accounts for alternating sums and differences in the inclusion-exclusion principle.

2. **Inner Summation**: \( \sum_{\substack{I \subseteq [n] \\ |I| = k}} \) iterates over all subsets \( I \) of the set \( [n] = \{1, 2, \ldots, n\} \) such that the number of elements in \( I \) is exactly \( k \). This ensures that every combination of \( k \) sets is considered for intersection.

3. **Intersection Size**: \( \left|\bigcap_{j \in I} A_j\right| \) computes the size of the intersection of sets indexed by the elements in \( I \).

This format uses big set and intersection symbols to emphasize the iterative selection of sets and their combinations, aligning with the notion of "big iteration notation." It provides a clear visual and symbolic representation of the step-by-step computation involved in applying the inclusion-exclusion principle.