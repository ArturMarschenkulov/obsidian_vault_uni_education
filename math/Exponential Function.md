The exponential function is the [[Euler's Number]] with the exponent $x$, that is $e^x$.

This function can also be represented using the Taylor Series.

>[!definition] 
>A definition of the *exponential function* is by using the [[Power series]], $\sum_{n=0}^\infty a_n x^n$ with $a_n=\frac{1}{n!}$, that is inverse [[Factorial]].
> $$e^x:=\sum_{n=0}^\infty\frac{x^n}{n!}=\sum_{n=0}^\infty \frac{1}{n!}x^n$$
>or
>$$e^x:=\lim_{n \to \infty} (1 + \frac{x}{n})^n$$



```desmos-graph
left=-4; right=4
bottom=-4; top=4
---
y=e^x
```

It's inverse is the natural [[logarithm]] $\ln{x}$ or $\log_e{x}$.
