

$$y'=q_0(t)+q_1(t)y+q_2(t)y^2=\sum_{k=0}^{2}q_k(t)y^k$$
Or shorter: $$y'=q_0+q_1y+q_2y^2$$
It is a first-order ODE and because of $y^2$ it is non-linear.

If $q_0=0$ it reduces into the [[Bernoulli Differential Equation]]. If $q_2=0$ it becomes a linear ODE.
# Solving
## Completely
Define $P(t):=\frac{q_2'}{q_2}+q_1$ and $Q(t)=q_0q_2$. Through the substitutions $v=q_2y$ and $v=\frac{-u'}{u}$, resulting in two equations:
- $v'=Q(t)+P(t)v+v^2$
- $u''-u'P(t)+Q(t)u=0$

This results into $y=\frac{-u'}{q_2u}=-q_2^{-1}(log(u))'$.
## Particular solution given
- $z=\frac{1}{y-y_p} \Longleftrightarrow y = y_p+ \frac{1}{z}$
- $z'=-(q_1+2q_2y_p)z-q_2(t)$

# Derivation
Substitute using $v=q_2y$. 

$$v'=(q_2y)'=q_2'y+q_2y'$$
$$v'=q_2'y+q_2(q_0+q_1y+q_2y^2)$$
$$=q_2'y+q_0q_2+q_1q_2y+q_2^2y^2$$
Note however that $y=\frac{v}{q_2}$, thus: $$=q_2'y+q_0q_2+q_1q_2y+q_2^2\frac{v^2}{q_2^2}$$
thus: $$=q_0q_2+(\frac{q_2'}{q_2}+q_1)v+v^2$$
We define $P(t)=\frac{q_2'}{q_2}+q_1$ and $Q(t)=q_0q_2$, so that: $$v'=Q(t)+P(t)v+v^2$$
Substitute $v=\frac{-u'}{u}$. This results into $$u''-u'P(t)+Q(t)u=0$$


$$y=\frac{v}{q_2}=\frac{-u'}{q_2u}$$

- https://math24.net/riccati-equation.html