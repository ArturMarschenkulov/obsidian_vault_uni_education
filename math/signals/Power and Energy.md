Notes about energy and power:


|        | dimension    | usual unit   |                     |
| ------ | ------------ | ------------ | ------------------- |
| Force  | $MLT^{-2}$   | newton $N$   | mass * acceleration |
| Energy | $ML^2T^{-2}$ | joule $J=Nm$ | force * length      |
| Power  | $ML^2T^{-3}$ | watt $W=J/s$ | energy / time       |
|        |              |              |                     |


- Energy:
	- dimensions: $L^2MT^2$
	- unit: joule $J$
- Power:
	- dimensions: $L^2MT^{-3}$

Given signal $x(t)$.

the instantaneous power is:
$$P_{x,i}=|x(t)|^2$$
the power is: 
$$P_x=\lim_{t \rightarrow \infty} \dfrac{1}{2T} \int_{-T}^{T}|x(t)|^2dt$$

the energy:
$$E_x=\int_{-\infty}^\infty|x(t)|^2dt=\int_{-\infty}^\infty P_{x,i}dt$$


- if $E_x=\infty$ or $P_x<\infty$, then $x(t)$ is a power signal. 
- if $E_x < \infty$ or $P_x=0$, then $x(t)$ is an energy signal.


