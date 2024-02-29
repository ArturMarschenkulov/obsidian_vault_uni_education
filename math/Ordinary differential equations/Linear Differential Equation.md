1A linear differential equation is a type of first-order differential equation that can be expressed in this general form:
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

- https://math24.net/exact-differential-equations.html
# Methods
Below are various methods of solving linear differential equations. 

## Integrating Factor Method
Read about it [[Integrating Factor |here ]].

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
See [[Linear Differential Equation|here]].

## Variation of Parameters
Used for non-homogeneous linear ODEs. This one is used when [[Linear Differential Equation#Methods#Method of Undetermined Coefficients|method of undetermined coefficients]] doesn't work, be it because it is not autonomous or because the non-homogenous part is more complex.

Find the homogeneous solution $y_h$.

- https://www.youtube.com/watch?v=3mKyKo58_LI