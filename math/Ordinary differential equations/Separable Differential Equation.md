$\dfrac{dy}{dx} = y'=g(x)f(y)$
$f(y)^{-1}y' = f(y)^{-1} \dfrac{dy}{dx} = g(x)$ 
$\int f(y)^{-1} \dfrac{dy}{dx} dx = \int f(y)^{-1} dx = \int g(x) dx + c_1$

If $f(y) = y$ then we can further generalize.
>$\int f(y)^{-1} dx = \int y^{-1} dx = \int g(x) dx + c_1$
>$\ln |y|  = \int g(x)dx + c_1$
>$e^{\ln |y|} = |y| = e^{\int g(x) dx + c_1} = e^{c_1} e^{\int g(x) dx}$
>$\sqrt{|y|^2} = y = \sqrt{(e^{c_1} e^{\int g(x) dx})^2}$
>$y = \pm e^{c_1} e^{\int g(x) dx} = c_1 e^{\int g(x) dx}$















separable differential equation