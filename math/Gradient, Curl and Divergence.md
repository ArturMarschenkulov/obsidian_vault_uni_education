


# Gradient
The gradient is a unary function, which takes in a multivariable function, and returns a vector of all partial derivatives of said function. That means that if the function has 2 variables, it returns a vector of 2 partial derivatives, and so on.

Another name for that is the Del operator, `del`,  `grad`, etc.

It represents the fastest increase of a scalar function.

- $\nabla : scalar \rightarrow vector$

- $\nabla f = (\frac{\delta f}{\delta x},\frac{\delta f}{\delta y})$
- $\nabla f = (\frac{\delta f}{\delta x},\frac{\delta f}{\delta y}, \frac{\delta f}{\delta z} )$

# Curl

In essence.
- $\nabla \times V = \frac{\delta f_y}{\delta x} - \frac{\delta f_x}{\delta y}$

- $\nabla \times V = (\frac{\delta f_z}{\delta y} - \frac{\delta f_y}{\delta z}, \frac{\delta f_x}{\delta z} - \frac{\delta f_z}{\delta x}, \frac{\delta f_y}{\delta x} - \frac{\delta f_x}{\delta y})$


# Divergence
In essence:
- $\nabla \cdot V = \frac{\delta f_x}{\delta x} + \frac{\delta f_y}{\delta y}$ or
- $\nabla \cdot V = \frac{\delta f_x}{\delta x} + \frac{\delta f_y}{\delta y} + \frac{\delta f_z}{\delta z}$
