# Solving
## 1st order
- $y'+p(t)y=q(t)$.
- $y_h=cy_1=ce^{-\int p(t)dt}$
- $y_p=vy_1$
- $v(t)=\int \frac{q(t)}{y_1} dt$

$y=y_h+y_p=cy_1+vy_1=(C+v)y_1=(C+v)e^{- \int p(t) dt}$
## 2nd order
Let consider this $y''+p(t)y'+q(t)y=g(t)$. Find the the homogeneous solution $y_h=c_1y_1(t)+c_2y_2(t)$.

We introduce two new functions $v_1(t)$ and $v_2(t)$.  And assume $y_p=v_1y_1+v_2y_2$. In the end:
- $v_1=-\int\frac{g(t)y_2}{W(y_1, y_2)}dt$
- $v_2=\int\frac{g(t)y_1}{W(y_1, y_2)}dt$

Or to ignore the [[Wronskian]]:
- $v_1=-\int\frac{g(t)y_2}{y_1y_2'-y_2y_1'}dt$
- $v_2=\int\frac{g(t)y_1}{y_1y_2'-y_2y_1'}dt$

Thus we have: $$y=y_h+y_p=c_1y_1+c_2y_2+v_1y_1+v_2y_2$$ and if we simplify: $$y=y_1(c_1+v_1)+y_2(c_2+v_2)$$

# Derivation

- $y''+p(t)y'+q(t)y=g(t)$
- $y_h=c_1y_1(t)+c_2y_2(t)$


Assume $y_p(t)=v_1(t)y_1(t)+v_2(t)y_2(t)=v_1y_1+v_2y_2$.
- $y_p''+p(t)y_p'+q(t)y_p=g(t)$
- $y_p'=v_1'y_1+v_1y_1'+v_2'y_2+v_2y_2'$
- $y_p''=v_1''y_1+v_1'y_1'+v_1'y_1'+v_1y_1''+v_2''y_2+v_2'y_2'+v_2'y_2'+v_2y_2''$
- $y_p''=v_1''y_1+2v_1'y_1'+v_1y_1''+v_2''y_2+2v_2'y_2'+v_2y_2''$

- $$(v_1''y_1+2v_1'y_1'+v_1y_1''+v_2''y_2+2v_2'y_2'+v_2y_2'')+p(t)(v_1'y_1+v_1y_1'+v_2'y_2+v_2y_2')+q(t)(v_1y_1+v_2y_2)=g(t)$$
One can factor out $v_1y_1$ and $v_2y_2$, thus resulting into: $$(v_1''y_1+2v_1'y_1'+v_2''y_2+2v_2'y_2')+p(t)(v_1'y_1+v_2'y_2)=g(t)$$

We make a new assumption: $v_1'y_1+v_2'y_2=0$. Which also means $v_1'y_1+v_1y_1'+v_2'y_2+v_2y_2'=0$ and thus also $v_1''y_1+v_2''y_2=-v_1'y_1'-v_2'y_2'$.

This results in: $$v_1'y_1'+v_2'y_2'=g(t)$$
$$
\begin{pmatrix}
y_1 & y_2\\
y_1' & y_2'
\end{pmatrix}
\begin{pmatrix}
v_1 \\
v_1' 
\end{pmatrix}
=
\begin{pmatrix}
0 \\
g(t) 
\end{pmatrix}
$$

Using [[Cramer's Rule]] and [[Wronskian]] we get:

$$v_1'=\frac{\begin{vmatrix} 0 &y_2 \\ g(t) &y_2'\end{vmatrix}}{\begin{vmatrix}y_1& y_2 \\ y_1'&y_2'\end{vmatrix}}=\frac{-y_2g(t)}{W(y_1, y_2)}$$

$$v_2'=\frac{\begin{vmatrix} y_1 & 0 \\ y_1' & g(t) \end{vmatrix}}{\begin{vmatrix}y_1& y_2 \\ y_1'&y_2'\end{vmatrix}}=\frac{y_1g(t)}{W(y_1, y_2)}$$

And then integrating:
- $v_1=-\int\frac{g(t)y_2}{W(y_1, y_2)}dt$
- $v_2=\int\frac{g(t)y_1}{W(y_1, y_2)}dt$


# Resources
Youtube:
- Houston Math Prep
	- https://www.youtube.com/watch?v=3mKyKo58_LI
- Michael Penn:
	- https://www.youtube.com/watch?v=kWPbxrEpaZE