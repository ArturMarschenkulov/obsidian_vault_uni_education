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

The reason being that those are regular linear differential equations and can be solved using the methods for linear differential equations. If $n = 1$, it is even a separable differential equation (see [[Separable Differential Equation]]).

If $n=0$, the equation simplifies to a linear ODE:
* $y'+p(x)y=q(x)y^0 = q(x)$

If $n=1$, the equation remains linear and becomes also separable:
* $y' + p(x)y=q(x)y^1=q(x)y$
* $y'=q(x)y-p(x)y=(q(x)-p(x))y$
* $y^{-1}y'=q(x)-p(x)$


# How to solve it
First of, when you detected a Bernoulli differential equation, put it into its standard form, $y'+p(x)y=q(x)y^n$.

To get the solution, use the below equation: 

 
$$y=\sqrt[1-n]{\mu_v^{-1}(1-n)\int \mu_v q(x)dx}$$
with:
$$\mu_b=e^{(1-n)\int p(x)dx}$$
Note, that $\mu_b$ is not the regular integrating factor ([[Integrating Factor]]), but a special one tailored for the Bernoulli equation. In essence one multiplies the normal ones with the "Bernoulli factor" $1-n$. The derivation of that you can see here: [[Bernoulli differential Equation#Derivation]].

It means that, after calculating the usually simple integral $\int p(x) dx$, the main task is to calculate $\int \mu_v q(x)dx$.
 
## Derivation
A Bernoulli differential equation can be transformed to a linear differential equation.

Firstly, one reshuffles the standard form, $y'+p(x)y=q(x)y^n$, into this:
* $y^{-n}y'+p(x)y^{1-n} = q(x)$

Then, one does substitution:
* $v=y^{1-n}=\frac{1}{y^{n-1}}$
To be useful we transform it to this:
* $y^{-n}y'=(1-n)^{-1}v'$
	* through: $v' = (1-n)y^{-n}y'$
Now we substitute:
* $(1-n)^{-1}v'+p(x)v=q(x)$
And if we reshuffle we get it into the standard form:
* $v'+(1-n)p(x)v=(1-n)q(x)$
We define new variables:
- $p_v(x)=(1-n)p(x)=-(n-1)p(x)$
- $q_v(x)=(1-n)q(x)=-(n-1)q(x)$:
- $v'+p_v(x)v=q_v(x)$

This means we can use the [[Integrating Factor]]:

$$\mu=e^{\int p_v(x)dx}=e^{(1-n)\int p(x)dx}$$
$$v=y^{1-n}=\mu^{-1}\int \mu q_v(x)dx$$
$$v=y^{1-n}=\mu^{-1}\int \mu q_v(x)dx$$
$$y=(\mu^{-1}\int \mu q_v(x)dx)^\dfrac{1}{1-n}=\sqrt[1-n]{\mu^{-1}\int \mu q_v(x)dx}$$
$$y=\sqrt[1-n]{\mu^{-1}(1-n)\int \mu q(x)dx}$$
$y=\sqrt[n-1]{\frac{1}{\mu^{-1}\int \mu q_v(x)dx}}$

$$y=\sqrt[n-1]{\frac{1}{\mu^{-1}\int \mu q_v(x)dx}}=\sqrt[n-1]{\frac{\mu}{(1-n)\int \mu q(x)dx}}$$



# Links
- https://www.cfm.brown.edu/people/dobrush/am33/Mathematica/ch2/bernoulli.html
- https://tutorial.math.lamar.edu/classes/de/bernoulli.aspx
- https://www.youtube.com/watch?v=BoI_ej-T0V4