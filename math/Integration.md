

# Rules
$\int dx$
Note, that + $C$ is always implied.
## Power rule
The power rule can be considered as one of the most fundamental integration rules.

In the simple case, on most likely most frequent case, it looks like this:
$$\int x^n dx = \dfrac{1}{n+1}x^{n+1}$$
In case that the place if $x$ is more complex, one has this.
$$\int (ax+b)^n dx = \dfrac{1}{a(n+1)}x^{n+1}$$

If $n=-1$, it is a special case.
$$\int x^{-1} dx = \int \dfrac{1}{x} = \ln|x|$$
- $\int (ax+b)^{-1} dx = a^{-1}\ln|ax+b|$
* $\int f(x)^{-1}dx$ a general form for this is difficult to calculate.
* $\int \dfrac{1}{ax+b} = \dfrac{1}{a} \ln|ax+b|$
## Exponential rule

* $\int c^{ax+b} dx = (a\ln(c))^{-1}c^{ax+b} = \dfrac{1}{a\ln(c)}c^{ax+b}$
* $\int e^{ax+b} dx = a^{-1}e^{ax+b} = \dfrac{1}{a}c^{ax+b}$

## Other
* $\int \ln(x) dx=x(\ln(x)-1)$

* $\int f gdx = f G - \int f' G dx$


# Trigs

$\cos \to \sin$
$\sin \to -\cos$
$\tan \to -\ln|\cos(x)|$


# Integration by Parts

- $\int uv dx = u \int v dx - \int u' (\int v dx) dx$
- $\int uv dx = u V - \int u' V dx$

## ILATE

The ILATE is a mnemonic to help which term should be $u$ or $v$. The reason is that that $u$ should have


|     |                       |                           |
| --- | --------------------- | ------------------------- |
| I   | Inverse trigonometric | $\sin^{-1}x$, $cos^{-1}x$ |
| L   | logarithmic           | $\log{x}$, $\ln{x}$       |
| A   | algebraic             | $x^2$, $\sqrt{x}$         |
| T   | trigonometric         | $\sin x$, $\cos x$        |
| E   | exponential           | $e^x$, $2^x$              |
