It is a [[Ordinary Differential Equation]].
- $a(t)y''+b(t)y'+c(t)y=0$
- $y''+p(t)y'+q(t)y=0$


# Ways to solve them

- [[Method of Undetermined Coefficients]]
- [[Method of Variation of Parameters]]
- [[Method of Reduction of Order]]



# Examples
Second Order constant coefficient linear ODE:
$$y''+py'+qy=s(t)$$


For the homogenous one, $y''+py'+qy=0$:
$$y=c_1e^{-\frac{1}{2}pt}e^{-\frac{1}{2}kt}+c_2e^{-\frac{1}{2}pt}e^{\frac{1}{2}kp}$$, with $k:=\sqrt{p^2-4q}$. $m:=e^{\frac{1}{2}pt}$, $n:=e^{\frac{1}{2}kt}$, thus $$y=c_1n^{-1}m^{-1}+c_2n^{-1}m$$
Note, $y=y_h+y_p$ and $y_h=c_1y_1+c_2y_2$, thus $y_1=n^{-1}m^{-1}$ and $y_2=n^{-1}m$.