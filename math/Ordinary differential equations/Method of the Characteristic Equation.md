s a method to solve nth order differential equations. It only works when the differential equation is linear and homogeneous and has constant coefficients. In practice it is usually used on [[2nd Order Differential Equation|second order]] differential equation, however they are also used on lower ones (first order) and higher.

$ay''+by'+cy=0$ becomes $ar^2+br+c=0$.

Then the next step is to get the roots and depending on how the roots look like it determines how the solution looks like.

The pq or abc formula is very important in this one:
- $$-\frac{p}{2} \pm \sqrt{(\frac{p}{2})^2-q}$$
- $$\frac{-b \pm \sqrt{b^2-4ac}}{2a}$$


In case of a 2 order polynomial, use this to decide what type it is.
- $b^2 > 4ac$ => real and distinct roots
- $b^2 < 4ac$ => complex roots
- $b^2 = 4ac$ => repeated roots

It is related to [[Euler's Number]]. It can only be used with [[Linear Differential Equation]].
# Roots
## Distinct real roots
e.g.:
- $y(t)=c_1e^{r_1t}+c_2e^{r_2t}$
## Repeated real roots
e.g.:
- $y(t)=c_1e^{rt}+c_2te^{rt}=(c_1+c_2t)e^{rt}$

## Complex roots
e.g.:
- $y(t)=e^{at}(c_1\cos(bt)+c_2\sin(bt))=(Ae^{(a+bi)t}+Be^{(a-bi)t})$ where $c_1=A+B$ and $c_2=A-B$.

Look [[Exponential Function]]