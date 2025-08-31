Also known as the unit impulse. First of, it is not a "function" in the general sense, but a distribution and those only make sense if they are under a integral sign (and multiplied by another function???).

> [!definition] **Dirac Delta Function** 
> The Dirac delta function, denoted as $\delta(t)$, is not a function in the traditional sense but a _distribution_ or _generalized function_ designed for mathematical analysis, primarily in the fields of engineering and physics.


The cornerstone of how this function is defined is this. It is not mathematically rigorous, but it gives a gist.
The most widely used definition is the one below, however it is not mathematically rigorous.
$$\delta(t)=

\begin{cases}
+\infty & : t = 0\\
0       & : t \neq 0
\end{cases}$$
The most important and defined feature of this function is its integral:
$$
\int^a_b \delta(t) dt = 1, b < 0 < a
$$

There are better ways to define this function:
- $\delta(t) =$
	- $\lim_{a \to 0} \dfrac{1}{a} rect(\dfrac{t}{a})$
	- $\lim_{a \to 0} \dfrac{1}{\pi}\dfrac{a}{a^2+t^2}$
	- $\frac{1}{2\pi}\int e^{i\tau t}d\tau$


# Properties


Below is the sifting property.
- $\int f(t)\delta(t-t_0)dt=f(t_0)$

If $t_0=0$, then the above equation simplifies to:
- $\int f(t)\delta(t)dt=f(0)$

- $\delta(at) = \frac{1}{|a|}\delta(t)$
- $\delta(-t)=\delta(t)$
- $\delta(f(t))=\sum_i\frac{\delta(t-t_0)}{|f'(t_i)|}$




derivative:

>[!theorem] integral
$$\int^{\infty}_{-\infty}\delta(t)dt=1$$
$$\int^x_{-\infty} \delta(t-t_0) dt=\varepsilon(t-t_0)$$

fourier:
- $\mathcal{F}\{\delta(t)\}(f) = 1$
laplace:
- $\mathcal{L}\{\delta(t)\}(f) = \frac{1}{s}$


- $f(t)* \delta(t-t_0)=f(t-t_0)$
- $f(t)* \delta(t-t_0)=\int_{-\infty}^\infty f(\tau)\delta(t-\tau-t_0)$


# Links
- https://math.libretexts.org/Bookshelves/Differential_Equations/Introduction_to_Partial_Differential_Equations_(Herman)/09%3A_Transform_Techniques_in_Physics/9.04%3A_The_Dirac_Delta_Function
- https://lpsa.swarthmore.edu/BackGround/ImpulseFunc/ImpFunc.html
- https://books.physics.oregonstate.edu/LinAlg/deltaintro.html