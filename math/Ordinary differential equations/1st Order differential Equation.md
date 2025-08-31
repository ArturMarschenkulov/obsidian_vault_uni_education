It is a [[Ordinary Differential Equation]].
- $F(t, y, y')=0$
- $y'=F(t, y)$
- $y'=f(t, y)$


# Types
## Exactness
$$M(x, y) dx + N(x,y)dy=0$$

- https://math24.net/exact-differential-equations.html

# Ways to solve them
- [[Method of Separation of Variables]]
- [[Integrating Factor]]
- [[Exact equation]]


# Real life examples
## Radioactive Decay
$N(t)$ is the quantity of radioactive isotopes at time $t$.

$N'= - \lambda N$

Using standard variables, this would be $y'=-py \iff y'+py=0$.


## Newton's Law of Heating and Cooling
$T' = r(T-T_a)=rT-rT_a$

$y'= py-ps$


## Logistic Growth

$$P'(t)=r\left(1-\frac{P(t)}{m}\right)P(t)$$

$$y'(t)=r\left(1-\frac{y(t)}{m}\right)y(t)=ry-\frac{r}{m}y^2$$
This can further be formed into $$y'-ry=-\frac{r}{m}y^2$$
# Examples

For the general linear first order ODE the following formula holds:
$$a(t)y'+b(t)y=c(t)$$ but firstly to simplify $p(t):=b(t)/a(t)$ and $q(t):=c(t)/a(t)$, to get the standard form: $$y'+p(t)y=q(t)$$
Given that this leads to $$y=c_1e^{-\int p(t) dt}+e^{-\int p(t) dt}\int q(t) e^{\int p(t)dt}dt$$
With $k(t):=e^{-\int p(t)dt}$ one can simplify it to this:$$y=\frac{c_1+\int k(t)q(t)dt}{k(t)}$$