

$\int dx$
Note, that + $C$ is always implied.
# Power rule
The power rule can be considered as one of the most fundamental integration rules.
> [!theorem] Power rule
> $\int x^n \, dx = \dfrac{1}{n+1}x^{n+1} + C, \quad n \neq -1$
> 
> $\int x^{-1} dx = \int \dfrac{1}{x} = \ln|x| + C, \quad n = -1$
If $n=-1$, it is a special case.
$$\int x^{-1} dx = \int \dfrac{1}{x} = \ln|x|$$
* $\int f(x)^{-1}dx$ a general form for this is difficult to calculate.

## Generalization to Linear Transformations

In case that the place if $x$ is more complex, one has this.
$$\int (ax+b)^n dx = \dfrac{1}{a(n+1)}x^{n+1}$$


- $\int (ax+b)^{-1} dx = a^{-1}\ln|ax+b|$
* $\int \dfrac{1}{ax+b} = \dfrac{1}{a} \ln|ax+b|$
# Exponential rule

* $\int c^{ax+b} dx = (a\ln(c))^{-1}c^{ax+b} = \dfrac{1}{a\ln(c)}c^{ax+b}$
* $\int e^{ax+b} dx = a^{-1}e^{ax+b} = \dfrac{1}{a}c^{ax+b}$
* $\int e^xdx=e^x$

## Other
* $\int \ln(x) dx=x(\ln(x)-1)$

* $\int f gdx = f G - \int f' G dx$

## Substitution
This is basically chain rule of integration, or the reverse of it.


The idea behind that is to rewrite a given integral into this $\int f(g(t))g'(t)dt$. Because this allows to do this: $\int f(u)g'(t) \frac{1}{g'(t)}du$ and thus $\int f(u)du$.

It works also if 



The idea is that one finds a way to turn $f(g(t))$ into something like $f(\gamma(t)\gamma'(t)$

- $\int f(g(t)) dt$
- $\int f(u)\frac{1}{g'(t)}dt$.

# Trigs

$\cos \to \sin$
$\sin \to -\cos$
$\tan \to -\ln|\cos(x)|$


# Integration by Parts

- $\int uv dx = u \int v dx - \int u' (\int v dx) dx$
- $\int uv dx = u V - \int u' V dx$

## ILATE

The ILATE is a mnemonic to help which term should be $u$ or $v$. The reason is that that $u$ should have


|     |                       |                           | deriv                                               | inte                                         |
| --- | --------------------- | ------------------------- | --------------------------------------------------- | -------------------------------------------- |
| I   | Inverse trigonometric | $\sin^{-1}x$, $cos^{-1}x$ | $\frac{1}{\sqrt{1-x^2}}$, $-\frac{1}{\sqrt{1-x^2}}$ |                                              |
| L   | logarithmic           | $\log_{10}{x}$, $\ln{x}$  | $\frac{1}{\ln{10}x}$,$\frac{1}{x}$                  | $\frac{x(\ln{x}-1)}{\ln{10}}$, $x(\ln{x}-1)$ |
| A   | algebraic             | $x^2$, $\sqrt{x}$         | $2x$, $\frac{1}{2\sqrt{x}}$                         | $\frac{2}{3}x^\frac{3}{2}$,$\frac{x^3}{3}$   |
| T   | trigonometric         | $\sin x$, $\cos x$        | $\cos{x}$, $-\sin{x}$                               | $-\cos{x}$, $\sin{x}$                        |
| E   | exponential           | $e^x$, $2^x$              | $e^x$, $\ln{2}2^x$                                  | $e^x$, $\frac{1}{\ln{2}}2^x$,                |
