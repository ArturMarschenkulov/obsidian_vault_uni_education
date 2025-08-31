# Questions
## What is an inhomogeneous system of diff. eq.
-

## What is a real fundamental system


# How to Find Eigenvalues and Eigenvectors of a 2x2 Matrix

Eigenvalues and eigenvectors are fundamental concepts in linear algebra, playing crucial roles in areas such as stability analysis, quantum mechanics, and machine learning algorithms. This note provides a concise guide on how to calculate the eigenvalues and eigenvectors of a 2x2 matrix, with an illustrative example to aid understanding.

## Definitions

- **Eigenvalues**: Scalars that determine how much the direction of a vector changes when a linear transformation (matrix) is applied.
- **Eigenvectors**: Non-zero vectors that only change by a scalar factor when that linear transformation is applied.

## Steps to Find Eigenvalues

Given a 2x2 matrix \( A = \begin{pmatrix} a & b \\ c & d \end{pmatrix} \), the eigenvalues \( \lambda \) are found by solving the characteristic equation:

1. **Set up the characteristic polynomial**: 
   
   \[
   \text{det}(A - \lambda I) = 0
   \]
   
   where \( I \) is the identity matrix \( \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} \). This leads to:
   
   \[
   \text{det} \left( \begin{pmatrix} a - \lambda & b \\ c & d - \lambda \end{pmatrix} \right) = 0
   \]

2. **Calculate the determinant**:
   
   \[
   (a - \lambda)(d - \lambda) - bc = 0
   \]

3. **Solve the quadratic equation**:
   
   The characteristic equation is a quadratic in terms of \( \lambda \):
   
   \[
   \lambda^2 - (a + d)\lambda + (ad - bc) = 0
   \]

   Use the quadratic formula:
   
   \[
   \lambda = \frac{(a + d) \pm \sqrt{(a + d)^2 - 4(ad - bc)}}{2}
   \]

These solutions are the eigenvalues \( \lambda_1 \) and \( \lambda_2 \).

## Steps to Find Eigenvectors

Once the eigenvalues are determined, eigenvectors for each eigenvalue can be found by solving the system:

$$
(A - \lambda I) \vec{v} = 0
$$

1. **Substitute each eigenvalue**:
   
   For \( \lambda_1 \), solve:
   
   $$
   \begin{pmatrix} a - \lambda_1 & b \\ c & d - \lambda_1 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}
   $$

2. **Solve the linear system**:
   
   This typically results in a free variable, and you can set it to any non-zero value to find a corresponding eigenvector.

## Example

Consider the matrix \( A = \begin{pmatrix} 3 & 1 \\ -2 & 4 \end{pmatrix} \):

1. **Find Eigenvalues**:
   
   \[
   \lambda^2 - 7\lambda + 10 = 0 \implies \lambda = 5, 2
   \]

2. **Find Eigenvectors**:

   - For \( \lambda = 5 \):
     
     \[
     \begin{pmatrix} -2 & 1 \\ -2 & -1 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \implies \vec{v}_1 = \begin{pmatrix} 1 \\ 2 \end{pmatrix}
     \]

   - For \( \lambda = 2 \):
     
     \[
     \begin{pmatrix} 1 & 1 \\ -2 & 2 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \implies \vec{v}_2 = \begin{pmatrix} 1 \\ -1 \end{pmatrix}
     \]

This guide should help you understand the steps to determine eigenvalues and eigenvectors for 2x2 matrices, enhancing your ability to tackle problems in various scientific and engineering fields.