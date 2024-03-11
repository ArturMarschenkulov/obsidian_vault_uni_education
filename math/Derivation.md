

$f'(x)=\lim_{h \to 0} \dfrac{f(x+h)-f(x)}{h}$

$\dfrac{d}{dx}[]$

# Rules
Let $f, g$ be functions. Let $c, n$ be constants.



* $\dfrac{d}{dx}[f(x)]=f'(x)$

Constants can be simply moved outside of the differentiation.
$\dfrac{d}{dx}[cf]=c\dfrac{d}{dx}[f]$

Differentiation is linear:
$\dfrac{d}{dx}[f \pm g]=\dfrac{d}{dx}[f] \pm \dfrac{d}{dx}[g]$


$\dfrac{d}{dx}[fg]=f\dfrac{d}{dx}[g]+\dfrac{d}{dx}[f]g$




## Power rule

* $\dfrac{d}{dx}[x^n] = nx^{n-1}$
The more general version is this below:
* $\dfrac{d}{dx}[x^{an+b}] = (an+b)x^{an+b-1}$

In fact, the reason why $\dfrac{d}{dx}[c]=0$ is because $\dfrac{d}{dx}[cx^0]=0cx^{-1}=0$.
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



## Misc 0
* $\dfrac{d}{dx}[f(x)]=f'(x)$


## Trigono

|           |                   |
| --------- | ----------------- |
| $\sin(x)$ | $\cos(x)$         |
| $\cos(x)$ | $-sin(x)$         |
| $\tan(x)$ | $\sec^2(x)$       |
| $\cot(x)$ | $-csc^2(x)$       |
| $\sec(x)$ | $\sec(x)\tan(x)$  |
| $\csc(x)$ | $-\cot(x)\csc(x)$ |
|           |                   |


|                |                                          |
| -------------- | ---------------------------------------- |
| $\sin^{-1}(x)$ | $\dfrac{1}{1-x^2}$                       |
| $\cos^{-1}(x)$ | $-\dfrac{1}{1-x^2}$                      |
| $\tan^{-1}(x)$ | $\dfrac{1}{1+x^2}$                       |
| $\cot^{-1}(x)$ | $-\dfrac{1}{1+x^2}$                      |
| $\sec^{-1}(x)$ | $\dfrac{1}{\sqrt{1-\dfrac{1}{x^2}x^2}}$  |
| $\csc^{-1}(x)$ | $-\dfrac{1}{\sqrt{1-\dfrac{1}{x^2}x^2}}$ |

$\DeclareMathOperator{\sech}{sech}$
$\DeclareMathOperator{\csch}{csch}$

|            |                                     |
| ---------- | ----------------------------------- |
| $\sinh(x)$ | $\dfrac{e^x+e^{-x}}{2}=\cosh(x)$    |
| $\cosh(x)$ | $\dfrac{e^x-e^{-x}}{2}=\sinh(x)$    |
| $\tanh(x)$ | $\dfrac{1}{\cosh^2(x)}= \sech^2(x)$ |
| $\coth(x)$ | $-\csch^2(x)$                       |
| $\sech(x)$ | $\sec(x)\tan(x)$                    |
| $\csch(x)$ | $-\cot(x)\csc(x)$                   |
|            |                                     |

