
# Linear Differential Equations

A linear differential equation is a type of first-order differential equation that follows this general form:

$$a(x)y' + b(x)y = c(x)$$

Here, $a(x)$, $b(x)$, and $c(x)$ are functions of $x$.

## Transforming into Standard Form

We aim to have the equation in a more tractable form, which we refer to as the standard form. To achieve this, we can use the following substitutions:

* $p(x) = \dfrac{b(x)}{a(x)}$
* $q(x) = \dfrac{c(x)}{a(x)}$

The standard form of the linear differential equation thus becomes:

$$y' + p(x)y = q(x)$$

## Solutions

Linear differential equations are amenable to solution using a number of methods, including:

1. **Integration Factor Method**:
   
   This method involves multiplying the equation by an integrating factor, typically denoted as $\mu(x)$, which is obtained as:
   $$\mu(x) = e^{\int p(x)dx}$$
   Thus, the differential equation transforms into:

   $$\mu(x)y' + \mu(x)p(x)y = \mu(x)q(x)$$
   $$\mu(x)y' + \mu(x)p(x)y = \mu(x)q(x)$$
   We use the fact that $\mu(x)p(x)=\mu'(x)$.
   $$\mu(x)y' + \mu'(x)y = \mu(x)q(x) \Leftrightarrow \dfrac{d}{dx}[\mu(x)y]$$
   We can then integrate both sides of the equation to find the solution:

   $$\int \mu(x)y'dx = \int \mu(x)q(x)dx$$

2. **Separation of Variables**:

   If the equation is separable, we can write it in the form:

   $$\dfrac{dy}{dx} = g(x)f(y)$$

   Then we separate variables and integrate:

   $$\int \dfrac{1}{f(y)} dy = \int g(x) dx$$

## General and Particular Solutions

Linear differential equations have general solutions which encompass a family of curves. Particular solutions can be found by applying initial conditions to the general solutions.

## Homogeneous and Non-Homogeneous Equations

Linear differential equations can be classified into homogeneous and non-homogeneous equations. 

- For homogeneous equations, where $q(x) = 0$, the general solution can be written as:

  $$y = Ce^{-\int p(x)dx}$$

- For non-homogeneous equations, the solution includes a particular solution which satisfies the non-homogeneous part and the complementary function which satisfies the homogeneous part.