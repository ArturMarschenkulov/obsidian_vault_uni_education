A linear differential equation is a type of first-order differential equation that can be expressed in this general form:
$$a(x)y'+b(x)y=c(x)$$
Let the coefficients $a(x), b(x), c(x)$ be functions of $x$ which are continuous on an interval $I$ and $a(x) \neq 0$.

Or even more general:
$$\sum_{i=0}^{n}a_i(x)y^{(i)}=b(x)$$


For easier solving, it is preferable to transform it into its standard form by performing a few substitutions:

>$p(x)=\dfrac{b(x)}{a(x)}$
>$q(x)=\dfrac{c(x)}{a(x)}$

Thus resulting into the following:
$$y'+p(x)y=q(x)$$

If $c(x)=0$ and thus also $q(x)=0$, then the differential equation is regarded as homogeneous. If $c(x) \neq 0$, then it is inhomogeneous.

# Types
## Homogeneity
Linear ODEs can be divided into homogeneous and non-homogeneous.

A linear ODE is homogeneous, when $q(x)=0$, otherwise it is non-homogeneous.

The solutions to non-homogeneous linear ODEs looks like this:
$$y=y_h+y_p$$
$y_h$ is the solution to the linear ODE if one sets $q(x)=0$, while $y_p$ is the particular solution

## Autonomous
Basically when $q(x)$ and $p(x)$ are constants, usually then written as $q$ and $p$.

## Exactness
$$M(x, y) dx + N(x,y)dy=0$$
# Methods
Below are various methods of solving linear differential equations. 

## Integrating Factor Method
The integrating factor method is the main solving method.

It is based on multiplying the whole equation with a so called integrating factor, usually denoted like this, given $y'+p(x)y=q(x)$:
$$\mu(x)=e^{\int p(x) dx}$$
The result is this:
$$y=\dfrac{1}{\mu(x)}\int\mu(x)q(x)dx$$
If the ODE is homogeneous, that is $q(x)=0$, then it even simplifies to this:
$$y=c_1\dfrac{1}{\mu(x)}=c_1\mu(x)^{-1}=c_1e^{-\int p(x)dx}$$
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

## Separation of Variables
If the linear ODE has appropriate coefficients $q(x)$ and $p(x)$, then it is a [[Separable Differential Equation|separable one]].

The simple cases are:
+ $q(x)=0$
+ $p(x)=0$
+ $q(x)=kp(x)$ with $k$ being some constant

However to be more exact it should fit the below equation:
$$f(x)g(y)=q(x)-p(x)y$$
Note however, that when $q(x)$ the equation is homogeneous. Thus this method is a good one to solve homogenous first order linear ODEs.

The result is that we have an equation which can be written like this:
$$y'=f(x)g(y)$$
Once we have that form, we put all $y$ on the left and everything else on the right.
$$\frac{1}{g(y)}y'=f(x)$$
Now we integrate both sides:
$$\int \frac{1}{g(y)}y' dx=\int f(x) dx$$
However to simplify, there is a neat trick. One can substitute $y'dx$, or rather $\frac{dy}{dx} dx$, with $dy$. As a rough (but wrong) mental model, some simply say the $dx$s cancel out. Thus:
$$\int \frac{1}{g(y)}dy=\int f(x) dx$$

If $g(y)$ is $g(y)=ay+b$, then:
$$\frac{ln(a y + c)}{a}=\int f(x) dx$$
$$ln(ay+c) = a^{-1} \int f(x) dx$$
$$e^{ln(ay+c)}=ay+c = e^{a^{-1} \int f(x) dx}$$
$$y = a^{-1}(e^{a^{-1} \int f(x) dx} - c) = \frac{e^{\frac{\int f(x) dx}{a}} - c}{a}$$
If $a=1$, then:
$$y = e^{\int f(x) dx} - c$$

## Method of Undetermined Coefficients
Usually used on ODEs with the form $y''+ py'+qy=q(x)$, where $q(x)$ is a relatively simple function and $p$ and $q$ are constants/coefficients.

It is based on the fact that $y=y_p+y_h$.

The first step is to get $y_h$. This usually done by the [[Characteristic Equation]], $ar²+br+c$, where $a b c$ match the coefficients of the differential equation in question. Then one find the roots (or root if the coefficient before $y''$ is $0$). Something like that is the result $c_1e^{rx}+c_2e^{rx}$.

The second step is $y_p$. This is based on first analyzing how $q(x)$ looks like.

| $q(x)$ | the guess for $y_h$ |
| ---- | ---- |
| $ke^{ax}$ | $Ae^{a x}$ |
| $kx^n,  n= 0, 1, 2, ...$ | $\sum_{i=0}^nK_i x^i$, $K_i= A, B, C, ...$ |
| $k \cos(ax)$ or $k \sin(ax)$ | $K \cos(ax) + M sin(ax)$ |
| $ke^{ax} \cos(bx)$ or $ke^{ax} \sin(bx)$ | $e^{ax}(K \cos(bx)+M \sin(bx))$ |
|  |  |




## Variation of Parameters
Used for non-homogeneous linear ODEs. This one is used when [[Linear Differential Equation#Methods#Method of Undetermined Coefficients|method of undetermined coefficients]] doesn't work, be it because it is not autonomous or because the non-homogenous part is more complex.
