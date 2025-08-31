s
# Gradient
The gradient is a unary function, which takes in a multivariable function, and returns a vector of all partial derivatives of said function. That means that if the function has 2 variables, it returns a vector of 2 partial derivatives, and so on.

Another name for that is the Del operator, `del`,  `grad`, etc.

It represents the fastest increase of a scalar function.

- $\nabla : scalar \rightarrow vector$

- $\nabla f = \mymatrixp{f_x\\f_y}$
- $\nabla f = \mymatrixp{f_x\\f_y\\f_z}$

# Curl

In essence. Let $F = (F_1, F_2, F_3)$, while $F_n$ being itself vectors $F_n = (F_{n,x},F_{n,y},F_{n,z})$.
- $\nabla \times F = F_{2,x} - F_{1,y}$

- $\nabla \times F = \mymatrixp{F_{3,y} - F_{2,z}\\ F_{1, z} - F_{3,x}\\ F_{2,x} - F_{1, y}}$


# Divergence
In essence:
- $\nabla \cdot V =f_{1,x}+f_{2, y}$ or
- $\nabla \cdot V =f_{1,x}+f_{2, y}+f_{3, z}$


# Relation between them
$\nabla \cdot \nabla f = \Delta f$
This is also called the the *Laplacian*. It tells how much quantity is spreading out or diffusing in space.
