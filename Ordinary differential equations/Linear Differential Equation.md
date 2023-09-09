A linear differential equation is a type of first-order differential equation that follows this general form:

$$a(x)y'+b(x)y=c(x)$$

Let the coefficients $a(x), b(x), c(x)$ be functions of $x$ which are continuous on an interval $I$ and $a(x) \neq 0$.

For easier solving, it is preferable to transform it into its standard form by performing a few substitutions:

* $p(x)=\dfrac{b(x)}{a(x)}$
* $q(x)=\dfrac{c(x)}{a(x)}$
Thus resulting into the following:

$$y'+p(x)y=q(x)$$

If $c(x)=0$ and thus also $q(x)=0$, then the differential equation is regarded as homogeneous. If $c(x) \neq 0$, then it is inhomogeneous.


# Integrating Factor Method
$\mu(x)=e^{\int p(x) dx}$
$\mu(x) y' + \mu(x) p(x) y = \mu(x) q$

$y=\mu^{-1}\int \mu q(x) dx$

$\int (\mu(x)y'+\mu(x)p(x)y) dx = \int \mu(x)q(x) dx$
$\mu(x)y = \int \mu(x)q(x) dx + C$

# Separable

If $q(x)=0$,
