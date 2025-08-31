If a differential equation can be expressed as 

Let $$\sum_{i=0}^{n} a_i(t)y^{(i)}(t)=b(t)$$, with $n$ being the order. $b(t)$ is called the non-homogeneous term, also called source function.

Usually, only first and second order are considered $$a(t)y'+b(t)y=c(t)$$ and $$a(t)y''+b(t)y'+c(t)y=d(t)$$
For easier solving, it is preferable to transform it into its standard form by performing a few substitutions:

>$p(t)=\dfrac{b(t)}{a(t)}$
>$q(t)=\dfrac{c(t)}{a(t)}$

Thus resulting into the following:
$$y'+p(t)y=q(t)$$

If $c(t)=0$ and thus also $q(t)=0$, then the differential equation is regarded as homogeneous. If $c(t) \neq 0$, then it is non-homogeneous.


In other words if one sees $y^n$, $sin(y)$, $ln(y)$ etc it is not linear.


# Methods
Below are various methods of solving linear differential equations. 

## Integrating Factor Method
Read about it here: [[Integrating Factor]].

## Separation of Variables
[[Method of Separation of Variables]]
## Method of Undetermined Coefficients
See here [[Method of Undetermined Coefficients]].

## Variation of Parameters
Used for non-homogeneous linear ODEs. This one is used when method of undetermined coefficients [[Method of Undetermined Coefficients]] doesn't work, be it because it is not autonomous or because the non-homogenous part is more complex.

Find the homogeneous solution $y_h$.

- https://www.youtube.com/watch?v=3mKyKo58_LI