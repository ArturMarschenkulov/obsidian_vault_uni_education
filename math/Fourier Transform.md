
It is a special case of the [[Laplace Transform]].



| $f(t)$                | $F(f)$                                       |
| --------------------- | -------------------------------------------- |
|                       | $F(f)=\int_{-\infty}^{\infty}f(t)e^{-jft}dt$ |
| $f(t-t_0)$            | $F(f)e^{jft_0}$                              |
| $f(t)e^{jf_0t}$       | $F(f-f_0)$                                   |
| $f(at)$               | $\dfrac{1}{\|a\|}F(\dfrac{f}{a})$            |
| $1$                   | $\delta(f)$                                  |
| $\delta(t)$           | $1$                                          |
| $\delta(t-t_0)$       | $\delta(f-\dfrac{1}{t_0})$                   |
| $\rect(\dfrac{t}{T})$ | $\|T\|\si(\pi f T)$                          |
| $\sgn(t)$             | $\dfrac{-j}{\pi f}, \dfrac{2}{jf}$           |
| $\dfrac{1}{\pi t}$    | $-j \sgn(f)$                                 |
| $e^{j2\pi f_0t}$      | $\delta(f-f_0)$                              |
| $e^{jf_0t}$           | $2\pi \delta (f-f_0)$                        |
| $\cos(2\pi f_0t)$     | $\dfrac{1}{2}(\delta(f+f_0)+\delta(f-f_0))$  |
| $\sin(2\pi f_0t)$     | $\dfrac{j}{2}(\delta(f+f_0)-\delta(f-f_0))$  |
| $\delta(t)$           | $\frac{1}{jf}+\pi\delta(f)$                  |
