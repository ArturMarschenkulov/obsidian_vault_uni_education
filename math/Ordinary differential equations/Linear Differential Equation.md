A linear differential equation is a type of first-order differential equation that can be expressed in this general form:
>$$a(x)y'+b(x)y=c(x)$$

Let the coefficients $a(x), b(x), c(x)$ be functions of $x$ which are continuous on an interval $I$ and $a(x) \neq 0$.

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
We use the fact that $\mu(x)p(x)=\mu'(x)$, to get this:
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

## Method of Undetermined Coefficients
Used for non-homogeneous autonomous linear ODEs where the non-homogeneous term, that is $q(x)$, is a simple function.
## Variation of Parameters
Used for non-homogeneous linear ODEs. This one is used when [[Linear Differential Equation#Methods#Method of Undetermined Coefficients|method of undetermined coefficients]] doesn't work, be it because it is not autonomous or because the non-homogenous part is more complex.
