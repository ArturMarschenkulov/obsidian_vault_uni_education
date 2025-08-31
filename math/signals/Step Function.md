

> [!definition]
> $\varepsilon(t)=
> \begin{cases}
> 	0 & : t < 0\\
> 	\dfrac{1}{2}& : t = 0 \\
> 	1 &: t >0
> \end{cases}$


> [!definition]
> $
> \varepsilon(t) = \lim_{k \rightarrow \infty} \dfrac{1}{2}(1 + \tanh(kx))=\lim_{k \rightarrow \infty} \dfrac{1}{1+e^{-2kx}}
> $


> [!note]
> - It creates a causal signal: $x_c(t)=x(t)\varepsilon(t)$
> - it is a power signal

> [!note] Derivative
> $\dfrac{d}{dt}\varepsilon(t)=\delta(t)$

> [!note] Integral
> $\int_{-\infty}^t\varepsilon(\tau)d\tau=t\varepsilon(t)=\rho(t)$