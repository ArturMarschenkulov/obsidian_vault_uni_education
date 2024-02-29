The integrating factor method is the main solving method. It is very useful to solving homogenous solutions.

It is based on multiplying the whole equation with a so called integrating factor, usually denoted like this, given $y'+p(x)y=q(x)$:
$$\mu(x)=e^{\int p(x) dx}$$
The result is this:
$$y=\dfrac{1}{\mu(x)}\int\mu(x)q(x)dx$$
If the ODE is homogeneous, that is $q(x)=0$, then it even simplifies to this:
$$y=c_1e^{-\int p(x)dx}$$
### Derivation
This is not needed to solve equations, but still good to know.

One multiplies the whole equation with that, so that the result is this:
$$\mu(x) y' + \mu(x) p(x) y = \mu(x) q(x)$$
We use the fact that $\mu(x)p(x)=\mu'(x)$, or rather that is the whole point of $\mu(x)$, to get this:
$$\mu(x) y' + \mu'(x) y = \mu(x) q(x)$$
This allows us to do the differentiation rule called factor rule, in reverse.
$$\dfrac{d}{dx}[\mu(x)y]=\mu(x)q(x)$$
We then integrate both sides:
$$\int\dfrac{d}{dx}[\mu(x)y]dx=\mu(x)y=\int\mu(x)q(x)dx$$
Thus ultimately resulting into (this is actually one one should use, everything before is just the derivation):
$$y=\dfrac{1}{\mu(x)}\int\mu(x)q(x)dx$$
If the ODE is homogeneous, that is $q(x)=0$, then it even simplifies to this:
$$y=c_1e^{-\int p(x)dx}=c_1\dfrac{1}{\mu(x)}=c_1\mu(x)^{-1}$$