The integrating factor is a function, usually denoted as $\mu(t)$, which facilitates solving integrals.

It is especially useful to solve [[1st Order differential Equation|first order]] ODEs.

It is based on multiplying the whole equation with a so called integrating factor. Let this be a linear ODE $y'+p(t)y=q(t)$ applying the integrating factor would look like this $\mu(t)y'+\mu(t)p(t)y=\mu(t)q(t)$.

# ODE
## Linear
For [[Linear Differential Equation|linear]], $y'+p(t)y=q(t)$ , ODEs the integrating factor is this:
$$\mu(t)=e^{\int p(t) dt}$$
Thus result is this:
$$y=\dfrac{1}{\mu(t)}\int\mu(t)q(t)dt$$
If the ODE is homogeneous, that is $qt=0$, then it even simplifies to this:
$$y=c_1e^{-\int p(t)dt}$$
## Non-Linear
# Derivation
This is not needed to solve [[Linear Differential Equation|linear]] ODEs, but still good to know.

The idea behind the integrating factor is that given $y' + p(t) y = q(t)$, one multiplies the whole equation with $\mu(t)$ ad thus $\mu(t) y' + \mu(t) p(t) y = \mu(t) q(t)$.

The idea is to define $\mu(t)$ in such a way that one can rewrite the equation as $\mu(t) y' + \mu'(t) y =\dfrac{d}{dt}[\mu(t)y] = \mu(t) q(t)$. This creates the constraint $\mu(t)p(t)=\mu'(t)$. 


We then integrate both sides:
$$\int\dfrac{d}{dx}[\mu(t)y]dx=\mu(t)y=\int\mu(t)q(t)dx$$
Thus, ultimately resulting into (this is actually one one should use, everything before is just the derivation):
$$y=\dfrac{1}{\mu(t)}\int\mu(t)q(t)dx$$
If the ODE is homogeneous, that is $q(t)=0$, then it even simplifies to this:
$$y=c_1e^{-\int p(t)dx}=c_1\dfrac{1}{\mu(t)}=c_1\mu(t)^{-1}$$

## Derivation 2
This is build on understanding how [[Exact equation]] work. Given $$M(t, y)dt + N(t, y)dy = 0$$ and $M_y \neq N_t$, that is it is not exact. Then we can find an integrating factor $\mu$ so that $(\mu M)_y = (\mu N)_t$. $$N\mu_t+\mu N_t=M\mu_y+\mu M_y$$ this leads to:
$$N\mu_t-M\mu_y=\mu(M_y-N_t)$$



If $\mu_y=0$  for $\mu(t)$: $$\frac{1}{\mu}\frac{d\mu}{dt}=\frac{1}{N}(M_y-N_t)$$
If $\mu_t=0$ for $\mu(y)$: $$\frac{1}{\mu}\frac{d\mu}{dy}=-\frac{1}{M}(M_y-N_t)$$

If $\mu$: $$\frac{1}{\mu}\frac{d\mu}{dz}=-\frac{1}{Nz_t-Mz_y}(M_y-N_t)$$

----


