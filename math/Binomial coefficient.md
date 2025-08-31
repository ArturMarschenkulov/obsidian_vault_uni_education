
>[!definition] 
>$$\binom{n}{k}=\frac{n!}{k!(n-k)!}$$

It is related to [[Factorial]]

>[!theorem] Identities
 It is *symmetric*:
$$\binom{n}{k}=\binom{n}{n-k}$$

>[!theorem] Pascal's Rule
$$\binom{n-1}{k-1}+\binom{n-1}{k}=\binom{n}{k}: n, k \geq 1 \land k \leq n -1$$


$$\binom{n}{k}=\binom{n-1}{k}+\binom{n-1}{k-1}$$or $$\binom{n+1}{k}=\binom{n}{k}+\binom{n}{k-1}$$
>[!theorem] Vandermonde's identity
$$\sum_{l=0}^k \binom{n}{l} \binom{m}{k-l}=\binom{n+m}{k}$$

$\binom{n}{2}=\sum_{i=0}^{n-1}i$


>[!theorem] 
$$\sum_{i=0}^n \binom{n}{i}=2^n$$

Usually that only works for natural numbers, however using the [[Gamma function]] one can expand that also to the real and even complex numbers.
$$\binom{n}{k}=\frac{\Gamma(n+1)}{\Gamma(k+1)\Gamma(n-k+1)}$$



Catalan number
$$\frac{1}{n+1}\binom{2n}{n}=\frac{(2n)!}{(n+1)!n!}=\prod\frac{n+k}{k}, \quad n \geq 0$$
# Examples
>[!example]
$\binom{1}{0}=1$, $\binom{1}{1}=1$
$\binom{2}{0}=1$, $\binom{2}{1}=2$, $\binom{2}{2}=1$
$\binom{3}{0}=1$, $\binom{3}{1}=3$, $\binom{3}{2}=3$, $\binom{3}{3}=1$
$\binom{4}{0}=1$, $\binom{4}{1}=4$, $\binom{4}{2}=6$, $\binom{4}{3}=4$, $\binom{4}{4}=1$



```tikz
\usepackage{tikz}

\begin{document}
\begin{tikzpicture}
\def\rows{7}
\foreach \row in {0,...,\rows} {
  % Add a line and the row number at the beginning of each row
  \draw[thick] (-0.5-\row/2,-\row-0.3) -- (\row/2+0.5,-\row-0.3) node[at start, left] {\row};
  \foreach \col in {0,...,\row} {
    \pgfmathtruncatemacro{\value}{\row! / (\col! * (\row-\col)!)};
    \node at (\col-\row/2,-\row) {\value};
  }
}
\end{tikzpicture}
\end{document}

```