
[[Elementary signals]]

# Properties
## Shifting
Shifting the whole signal to right or left done by adding or subtracting something to the input, let's call it $t_0$. If $x(t)$ is the unshifted signal, then $x(t-t_0)$ is the shifted one. Depending on the $t_0$ it is shifted to the left or right. If $t_0 > 0$, then it is a right shift and $t_0<0$ is a left shift.

## Symmetry
Every signal has an even and an odd part.

- $x(t)=x_e(t)+x_o(t)$

For even signals, the below applies:
- $x_e(t)=x_e(-t)$
- $x_e(t)=\dfrac{1}{2}(x(t)+x(-t))$

For odd signals, the below applies:
- $x_o(t)=-x_o(-t)$
- $x_o(t)=\dfrac{1}{2}(x(t)-x(-t))$

### Complex Signals
Complex signals have special symmetries.

A signal is conjugate even, if the real part is even and the imaginary part is odd. This applies then:
- $x(t) = x^*(-t)$
- $x_R(t)+jx_I(t)=x_R(-t)-jx_I(-t)$

A signal is conjugate odd, if the real part is odd and the imaginary part is even. This applies then:
- $x(t)=-x^*(-t)$
- $x_R(t)+jx_I(t)=-x_R(-t)+jx_I(-t)$


- $x_R(t)=\frac{x(t)+x^*(t)}{2}$
- $x_I(t)=\frac{x(t)-x^*(t)}{2j}$
- $x_e(t)=\frac{x(t)+x(-t)}{2}$
- $x_o(t)=\frac{x(t)-x(-t)}{2}$
## Scaling
Scaling is done by multiplying the input with $a$, like this $x(at)$.
