
$$\mathcal{L}\{f(t)\} = F(s) = \int_0^\infty f(t)e^{-st}dt$$

$$F(s)=\int_0^\infty f(t)e^{-(a+jb)t}dt$$

[[Fourier Transform]] is a more specific version of this.


# Table

https://tutorial.math.lamar.edu/Classes/DE/Laplace_Table.aspx

|                            |                                                                    |
| -------------------------- | ------------------------------------------------------------------ |
| $1$                        | $\frac{1}{s}$                                                      |
| $e^{at}$                   | $\frac{1}{s-a}$                                                    |
| $t$                        | $\frac{1}{s^{2}}$                                                  |
| $t^n$                      | $\frac{n!}{s^{n+1}}$                                               |
| $t^{n-\frac{1}{2}}$        | $\frac{1*3*5 ... (2n-1) \sqrt{\pi}}{2^ns^{n+\frac{1}{2}}}$         |
| $\sqrt{t}=t^{\frac{1}{2}}$ | $\frac{\sqrt{\pi}}{2s^{\frac{3}{2}}}=\frac{(1/2)!}{s^{(1/2)+2/2}}$ |
| $t^ne^{at}$                | $\frac{n!}{(s-a)^{n+1}}$                                           |
| $f(ct)$                    | $\frac{1}{c}F(\frac{s}{c})$                                        |
| $f(t)$                     | $F(s)=\int_0^\infty f(t)e^{-st}dt$                                 |
| $f'(t)$                    | $sF(s)-f(0)$                                                       |
| $f''(t)$                   | $s^2F(s)-sf(0)-f'(0)$                                              |
| $f'''(t)$                  | $s^3F(s)-s^2f(0)-sf'(0)-f''(0)$                                    |
| $f^{(4)}(t)$               | $s^4F(s)-s^3f(0)-s^2f'(0)-sf''(0)-f'''(0)$                         |
| $f^{n}(t)$                 | $s^nF(s) - \sum_{k=1}^{n}s^{n-k}f^{(k-1)}(0)$                      |
| $\sin(at)$                 | $\frac{a}{s^2+a^2}$                                                |
| $\cos(at)$                 | $\frac{s}{s^2+a^2}$                                                |
| $\sinh(at)$                | $\frac{a}{s^2-a^2}$                                                |
| $\cosh(at)$                | $\frac{s}{s^2-a^2}$                                                |
