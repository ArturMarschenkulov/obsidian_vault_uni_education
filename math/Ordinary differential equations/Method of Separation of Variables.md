
> [!theorem]
> A differential equation is called *separable* if it can be expressed in the form: $\frac{dy}{dt}=f(y)g(t)$ where $f(y)$ and $g(t)$ are functions of $y$ and $t$ respectively.

> [!theorem]
> Furthermore, this definition extends to higher order differential equations such that: $\frac{d^n y}{dt^n} = y^{(n)} = f(y^{(n-1)})g(t)$ where $y^{(n-1)}$ represents the $(n-1)$th derivative of $y$ with respect to $t$.

The method is primarily used for solving [[1st Order differential Equation|first-order differential equations]]. 

Once one has identified it is separable, one puts it into the following form: $$\frac{1}{f(y)}dy=g(t)dt$$
- $\dfrac{dy}{dx} = y'=g(t)f(y)$
- $f(y)^{-1}y' = f(y)^{-1} \dfrac{dy}{dx} = g(t)$ 
- $\int f(y)^{-1} \dfrac{dy}{dx} dx = \int f(y)^{-1} dx = \int g(t) dx + c_1$

If $f(y) = y$ then we can further generalize.
>$\int f(y)^{-1} dx = \int y^{-1} dx = \int g(t) dx + c_1$
>$\ln |y|  = \int g(t)dx + c_1$
>$e^{\ln |y|} = |y| = e^{\int g(t) dx + c_1} = e^{c_1} e^{\int g(t) dx}$
>$\sqrt{|y|^2} = y = \sqrt{(e^{c_1} e^{\int g(t) dx})^2}$
>$y = \pm e^{c_1} e^{\int g(t) dx} = c_1 e^{\int g(t) dx}$





Upon recognizing that an equation is separable, it can be transformed into the form:

$$\frac{1}{f(y)} \, dy = g(t) \, dt$$

Where the differential equation $\frac{dy}{dx} = y' = g(t)f(y)$ leads to the following manipulations:

1. Divide both sides by $f(y)$:
   $$ f(y)^{-1}y' = f(y)^{-1} \frac{dy}{dx} = g(t) $$

2. Integrate both sides with respect to $x$:
   $$ \int f(y)^{-1} \frac{dy}{dx} \, dx = \int g(t) \, dx + c_1 $$

   Simplifying further, if $f(y) = y$, then:

   $$ \int y^{-1} \, dy = \ln |y| $$
   $$ \ln |y| = \int g(t) \, dx + c_1 $$
   $$ |y| = e^{\int g(t) \, dx + c_1} = e^{c_1}e^{\int g(t) \, dx} $$
   $$ y = \pm e^{c_1} e^{\int g(t) \, dx} = c_1 e^{\int g(t) \, dx} $$

This notation describes the process of separating, integrating, and solving a first-order separable differential equation step-by-step in a clear and concise manner.

## Separation of Variables
If the linear ODE has appropriate coefficients $q(t)$ and $p(t)$, then it is a separable one (see: [[Method of Separation of Variables]]).

The simple cases are:
+ $q(t)=0$
+ $p(t)=0$
+ $q(t)=kp(t)$ with $k$ being some constant

However to be more exact it should fit the below equation:
$$f(t)g(y)=q(t)-p(t)y$$
Note however, that when $q(t)$ the equation is homogeneous. Thus this method is a good one to solve homogenous first order linear ODEs.

The result is that we have an equation which can be written like this:
$$y'=f(t)g(y)$$
Once we have that form, we put all $y$ on the left and everything else on the right.
$$\frac{1}{g(y)}y'=f(t)$$
Now we integrate both sides:
$$\int \frac{1}{g(y)}y' dx=\int f(t) dx$$
However to simplify, there is a neat trick. One can substitute $y'dx$, or rather $\frac{dy}{dx} dx$, with $dy$. As a rough (but wrong) mental model, some simply say the $dx$s cancel out. Thus:
$$\int \frac{1}{g(y)}dy=\int f(t) dx$$

If $g(y)$ is $g(y)=ay+b$, then:
$$\frac{ln(a y + c)}{a}=\int f(t) dx$$
$$ln(ay+c) = a^{-1} \int f(t) dx$$
$$e^{ln(ay+c)}=ay+c = e^{a^{-1} \int f(t) dx}$$
$$y = a^{-1}(e^{a^{-1} \int f(t) dx} - c) = \frac{e^{\frac{\int f(t) dx}{a}} - c}{a}$$
If $a=1$, then:
$$y = e^{\int f(t) dx} - c$$





separable differential equation