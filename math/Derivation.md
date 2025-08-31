
> [!definition]
> Let $I$ be an *open real interval*. Let $f: I \to \mathbb{R}$. Let $x \in I$ be a point in $I$.
> $f'(x)=\lim_{h \to 0} \dfrac{f(x+h)-f(x)}{h}$
> $f'(x)=\lim_{x \to a} \dfrac{f(a)-f(x)}{a-x}$
> 
> Another form to $f'$ is $\frac{df}{dt}=\lim_{\Delta t \to 0} \frac{\Delta f}{\Delta t}$

> [!definition] **Derivative** 
> Let $I$ be an open real interval, $f: I \to \mathbb{R}$ a function, and $x \in I$. The derivative of $f$ at $x$, denoted $f'(x)$, is defined as: 
>  $$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h},$$ 
>  provided this limit exists. An equivalent expression is: 
> $$f'(x) = \lim_{a \to x} \frac{f(a) - f(x)}{a - x}.$$ 
>  Another notation for the derivative is: 
>   $$\frac{df}{dt} = \lim_{\Delta t \to 0} \frac{\Delta f}{\Delta t}.$$


# Notation for Derivatives 

| Notation Style | Example                              | Description                                               |     |
| -------------- | ------------------------------------ | --------------------------------------------------------- | --- |
| Leibniz        | $\frac{dy}{dx}$, $\frac{d^2y}{dx^2}$ | Notation for derivatives and higher order derivatives.    |     |
| Lagrange       | $y'$, $y''$                          | Prime notation commonly used in simple derivatives.       |     |
| Newton         | $\dot{y}$, $\ddot{y}$                | Notation used primarily for time derivatives in dynamics. |     |
| Euler          | $D y$, $D^2 y$                       | Operator notation for derivatives.                        |     |

# Rules

> [!theorem] **Linearity of Differentiation** 
> Let $f, g$ be functions and $c$ a constant. The derivative operator is linear: 
> $$\frac{d}{dx}[cf] = c\frac{d}{dx}[f],$$ 
> $$\frac{d}{dx}[f \pm g] = \frac{d}{dx}[f] \pm \frac{d}{dx}[g].$$


> [!theorem] **Product Rule** 
> For functions $f$ and $g$: 
> $$\frac{d}{dx}[fg] = f\frac{d}{dx}[g] + g\frac{d}{dx}[f].$$

## Temp
if function sometimes:

- $u(y) = \frac{1}{y(t)} => -\frac{1}{y^2(t)}y'(t)$

## Power rule

> [!theorem] **Power Rule** 
> Let $n \in \mathbb{R}$. The derivative of $x^n$ with respect to $x$ is given by: 
> $$\frac{d}{dx}(x^n) = nx^{n-1}.$$ 


> [!theorem] **Constant Rule** 
> The derivative of a constant is zero: 
> $$\frac{d}{dx}(c) = 0.$$ 
> This is a specific case of the power rule, where $n=0$.
### Generalization to Linear Transformations
The more general version is this below:
* $\dfrac{d}{dx}[x^{an+b}] = (an+b)x^{an+b-1}$


## Chain rule


| $f$         | $f'$                        |
| ----------- | --------------------------- |
| $f(g(x))$   | $f'(g(x))g'(x)$             |
| $c^{ax+b}$  | $ac^{ax+b}\ln(c)$           |
| $e^{ax+b}$  | $ae^{ax+b}\ln(e)=ae^{ax+b}$ |
| $\ln(ax+b)$ | $(ax+b)^{-1}a$              |
|             |                             |
|             |                             |
|             |                             |

The [[Integration]] counterpart is substitution.


## Trigonometric Functions

| $f(x)$    | $f'(x)$           |
| --------- | ----------------- |
| $\sin(x)$ | $\cos(x)$         |
| $\cos(x)$ | $-sin(x)$         |
| $\tan(x)$ | $\sec^2(x)$       |
| $\cot(x)$ | $-csc^2(x)$       |
| $\sec(x)$ | $\sec(x)\tan(x)$  |
| $\csc(x)$ | $-\cot(x)\csc(x)$ |
|           |                   |

## Inverse Trigonometric Functions

| $f(x)$         | $f'(x)$                                  |
| -------------- | ---------------------------------------- |
| $\sin^{-1}(x)$ | $\dfrac{1}{1-x^2}$                       |
| $\cos^{-1}(x)$ | $-\dfrac{1}{1-x^2}$                      |
| $\tan^{-1}(x)$ | $\dfrac{1}{1+x^2}$                       |
| $\cot^{-1}(x)$ | $-\dfrac{1}{1+x^2}$                      |
| $\sec^{-1}(x)$ | $\dfrac{1}{\sqrt{1-\dfrac{1}{x^2}x^2}}$  |
| $\csc^{-1}(x)$ | $-\dfrac{1}{\sqrt{1-\dfrac{1}{x^2}x^2}}$ |

$\DeclareMathOperator{\sech}{sech}$
$\DeclareMathOperator{\csch}{csch}$
## Hyperbolic Functions

| $f(x)$     | $f'(x)$                             |
| ---------- | ----------------------------------- |
| $\sinh(x)$ | $\dfrac{e^x+e^{-x}}{2}=\cosh(x)$    |
| $\cosh(x)$ | $\dfrac{e^x-e^{-x}}{2}=\sinh(x)$    |
| $\tanh(x)$ | $\dfrac{1}{\cosh^2(x)}= \sech^2(x)$ |
| $\coth(x)$ | $-\csch^2(x)$                       |
| $\sech(x)$ | $\sec(x)\tan(x)$                    |
| $\csch(x)$ | $-\cot(x)\csc(x)$                   |
|            |                                     |

