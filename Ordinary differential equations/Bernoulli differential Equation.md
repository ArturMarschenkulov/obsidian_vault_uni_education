A Bernoulli differential equation is a type of first-order differential equation that has a the following general form.
 $$a(x)y'+b(x)y=c(x)y^n$$
Where $a(x), b(x), c(x)$ are function of $x$ with $n \in \mathbb{Z}$.

# Transforming into Standard Form
To better be able to solve this type of ODE, it is necessary to transform it into its standard form, by dividing the whole equation by $a(x)$ and then using the following substitutions:

* $p(x)=\dfrac{b(x)}{a(x)}$
* $q(x)=\dfrac{c(x)}{a(x)}$

This results into the following standard form:

* $y'+p(x)y=q(x)y^n$

# Special case n=0 and n=1
Usually, only equations with $n \notin \{0, 1\}$ are regarded as Bernoulli differential equations. The reason is that are 

The reason being that those are regular linear differential equations and can be solved using the methods for linear differential equations. If $n = 1$, it is even a [[Separable Differential Equation|separable differential equation]].

If $n=0$, the equation simplifies to a linear ODE:
* $y'+p(x)y=q(x)y^0 = q(x)$

If $n=1$, the equation remains linear and becomes also separable:
* $y' + p(x)y=q(x)y^1=q(x)y$
* $y'=q(x)y-p(x)y=(q(x)-p(x))y$
* $y^{-1}y'=q(x)-p(x)$

# Transformation to Linear Differential Equation
A Bernoulli differential equation can be transformed to a linear differential equation, using the following substitution and its transformations:
* $v=y^{1-n}$
* $v'=(1-n)y^{-n}y'$
* $y^{-n}y'=(1-n)^{-1}v'$

It is useful to firstly reshuffle the equation.
* $y'+p(x)y=q(x)y^n$
* $y^{-n}y'+p(x)y^{1-n} = q(x)$

Now one can see the relationship:
* $v=y^{1-n}$
* $v'=(1-n)y^{1-n-1}=(1-n)y^{-n}y'$
* $y^{-n}y'=(1-n)^{-1}v'$

No we substitute:
* $(1-n)^{-1}v'+p(x)v=q(x)$
* $v'+(1-n)p(x)v=(1-n)q(x)$