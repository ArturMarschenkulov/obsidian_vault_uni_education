A Bernoulli differential equation is a type of [[1st Order differential Equation|first-order]] and [[Non-Linear Differential Equation|non-linear]] differential equation that has a the following general form. $$y'+p(t)y=q(t)y^n$$
>[!theorem]
>Let $y'+p(t)y=q(t)y^n$ be an ODE, then:
$$y=\sqrt[1-n]{\mu_v^{-1}(1-n)\int \mu_v q(t)dx}$$
or
$$y^{1-n}=\mu_v^{-1}(1-n)\int \mu_v q(t)dx$$
with: $\mu_v=e^{(1-n)\int p(t)dx}$


> [!note]
> Note, that $\mu_v$ is not the regular integrating factor ([[Integrating Factor]]), but a special one tailored for the Bernoulli equation. In essence one multiplies the normal ones with the "Bernoulli factor" $1-n$. The derivation of that you can see here: [[Bernoulli Differential Equation#Derivation]].

Usually only if $n \notin {0, 1}$, is the above ODE considered to be a Bernoulli ODE.  If $n=0$, then the ODE becomes [[Linear Differential Equation |]], and it simplifies to [[Integrating Factor|integrating factor method]].

>[!theorem] Special case: $n=0$
Let $y'+p(t)y=q(t)y^0=q(t)$ be an ODE, then:
$$y=\sqrt[1-0]{\mu_v^{-1}(1-0)\int \mu_v q(t)dx}=\mu_v^{-1}\int \mu_v q(t)dx$$
with: $\mu_v=e^{(1-0)\int p(t)dx}=e^{\int p(t)dx}$

>[!theorem] Special case: $n=1$
Let $y'+p(t)y=q(t)y^1=q(t)y$ be an ODE, then:
$$y^{1-1}=\mu_v^{-1}(1-1)\int \mu_v q(t)dx=1=1 \cdot 0 \cdot \int 1 \cdot q(t)dx$$
with: $\mu_v=e^{(1-1)\int p(t)dx}=1$
$$1=0 \cdot \int q(t)dx \iff \frac{1}{\int q(t)dx}=0$$
Instead of the above one simply uses the [[Method of Separation of Variables]].
$$\frac{dy}{dt}=(q(t)-p(t))y$$
$$\frac{1}{y} dy=(q(t)-p(t))dt$$


> [!theorem] Special case: $q(t) = 0$
> If $q(t) = 0$, then it simplifies to a simple homogeneous linear ODE: $y'+p(t)y=0 \cdot y^n=0$
> 

# How to solve it
So basically, once one has put the equation into the standard Bernoulli form, one identifies $p(t)$, $q(t)$, $n$, calculates $1-n$, $\int p(t) dt$, to get $\mu_v$. Those are usually simple. The main task is to then calculate $\int \mu_v q(t)dx$

- $y'^{1-n}=u'=(1-n)(p(t)y+q(t))$
# Proof
A Bernoulli differential equation can be transformed to a linear differential equation.

Firstly, one reshuffles the standard form, $y'+p(t)y=q(t)y^n$, into this:
* $y^{-n}y'+p(t)y^{1-n} = q(t)$

Then, through the following substitution, derivation and transformation, one gets the following equations:
* $v=y^{1-n}$
* $v' = (1-n)y^{-n}y'$
* $y^{-n}y'=(1-n)^{-1}v'$
Now we substitute:
* $(1-n)^{-1}v'+p(t)v=q(t)$

Now we can transform that into a linear first order ODE, of the form $y'+P(t)y=Q(t)$ with $P(t)=(1-n)p(t)$ and $Q(t)=(1-n)q(t)$.
- $v'+(1-n)p(t)v=(1-n)q(t)$
- $v'=(1-n)(q(t)-p(t)v)$.
We define new variables:
- $p_v(t)=(1-n)p(t)$
- $q_v(t)=(1-n)q(t)$:
- $v'+p_v(t)v=q_v(t)$

This means we can use the [[Integrating Factor]]:

$$\mu=e^{\int p_v(t)dt}=e^{(1-n)\int p(t)dt}$$
$$\mu v= \mu y^{1-n}=\int \mu q_v(t)dx$$
$$v=y^{1-n}=\mu^{-1}\int \mu q_v(t)dx$$
$$y=(\mu^{-1}\int \mu q_v(t)dx)^\frac{1}{1-n}=\sqrt[1-n]{\mu^{-1}\int \mu q_v(t)dx}$$
$$y=\sqrt[1-n]{\mu^{-1}(1-n)\int \mu q(t)dx}$$



# Links
- https://www.cfm.brown.edu/people/dobrush/am33/Mathematica/ch2/bernoulli.html
- https://tutorial.math.lamar.edu/classes/de/bernoulli.aspx
- https://www.youtube.com/watch?v=BoI_ej-T0V4
