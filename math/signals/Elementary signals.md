  $\DeclareMathOperator{\rect}{rect}$

# List
## Step
[[Step Function]]

## Ramp
Essentially, [[Step Function]] times a the variable.

> [!definition]
> It can be defined in several ways:
> 
> - $\rho(t)=t\varepsilon(t)=\max(t, 0)$
> - $\rho(t)=\int_{-\infty}^t\varepsilon(x)dx$
> - $\rho(t)=\varepsilon(t)*\varepsilon(t)$

> [!note]
> - power signal
> - causal

> [!note] Derivative
> $\frac{d}{dt}\rho(t)=\varepsilon(t)$

> [!note] Integral
> $\int \rho(t)$

> [!note] [[Fourier Transform]]
> $\mathcal{F}\{\rho(t)\}(f) = \frac{i\delta'(f)}{4\pi}-\frac{1}{4\pi^2f^2}$

> [!note] [[Laplace Transform]]
> $\mathcal{L}\{\rho(t)\}(s)=\frac{1}{s^2}$
## Sign Function
$$sgn(t)=\begin{cases}
-1 &: t < 0\\
0 &: t = 0\\
1 &: t>0
\end{cases}$$

- $sgn(t) = 2\varepsilon(t)-1$

Used to create 

$|x(t)| = sgn(x(t))x(t)$


- power signal
- non-causal



- $\int sgn(t)dt = 2\delta(t)$


## Dirac
[[Dirac Delta Function]]


## Rectangular
Also called the unit pulse function.

$$\rect(t)=\begin{cases}
0 &: |t| > \dfrac{1}{2}\\
\dfrac{1}{2} &: |t| = \dfrac{1}{2}\\
1 &: |t| < \dfrac{1}{2}
\end{cases}$$

The rectangular function can also be modelled using 2 step functions.
$$\rect(t)=\varepsilon(t+\dfrac{1}{2})-\varepsilon(t-\dfrac{1}{2})$$

- energy signal
- non-causal

derivative:
- $\frac{d}{dt}\rect(t)=\delta(t+\frac{1}{2})-\delta-\frac{1}{2})$
- 
integral:
fourier:
- $\mathcal{F}\{\rect\}(f)=\si(\pi f)$
laplace:
- $\mathcal{L}\{\rect\}(s)=\frac{1-e^\frac{s}{2}}{s}$

## Triangular

It's the [[convolution]] of two rectangular functions
- $\tri(t) = \rect(t) * \rect(t)$


- energy signal
- non-causal
## si-Function

$\si$ is used for the unnormalized version, while $\sinc$
 for the normalized version.
 - $\si(t)=\frac{\sin(t)}{t}$
 - $\sinc(t)=\frac{\sin(\pi t)}{\pi t}=\si(\pi t)$
 
- energy signal
- non-causal