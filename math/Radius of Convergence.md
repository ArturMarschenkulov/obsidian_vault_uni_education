


Let $A(x)=\sum_{n=0}^\infty a_n x^n$ be a power series ([[Power series]])

## Convergence Scenarios

For a given [[Power series]] $A(x)$, exactly one of the following three scenarios will occur:

1. **Global Convergence:** $A(x)$ converges for all $x \in \mathbb{R}$.
2. **Convergence at Zero:** $A(x)$ converges only at $x = 0$.
3. **Convergence within Radius:** There exists a radius $r > 0$ such that $A(x)$ converges for all $x \in \mathbb{R}$ with $|x| < r$. This radius $r$ is the largest such value and is known as the *convergence radius*.

## Calculating the Convergence Radius

The convergence radius of a power series can often be determined if certain limits exist:

- **Ratio Test Limit:** 
  $$
  \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right|
  $$
  If this limit exists, it equals the convergence radius. [[Ratio test]]

- **Root Test Limit:** 
  $$
  \lim_{n \to \infty} \sqrt[n]{|a_n|}
  $$
  If this limit exists, the reciprocal of this value equals the convergence radius.

These methods are based on the *ratio test* and the *root test* respectively, which are commonly used to determine the convergence of series.

## Conclusion

Understanding the convergence behavior of power series is crucial in mathematical analysis, especially when dealing with functions representable by series. The convergence radius provides valuable insights into the domain within which the series converges absolutely.

