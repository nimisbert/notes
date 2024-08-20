$DL$ pour $a=0$, se nomme aussi série de Maclaurin, cas particulier des séries de Taylor.

| $\mathbf{f(x)}$  | $\mathbf{Maclaurin}$                                  | $\mathbf{Dévellopement \quad limité}$                       |
| :--------------: | :---------------------------------------------------- | :---------------------------------------------------------- |
|      $e^x$       | $\sum_{n=0}^{\infty} \frac{x^n}{n!}$                  | $1+x+\frac{1}{2}x^2+\frac{1}{6}x^3+...+\frac{1}{n}x^n+o(n)$ |
|    $ln(x+1)$     | $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n}x^n$         |                                                             |
|     $sin(x)$     | $\sum_{n=0}^{\infty} \frac{(-1)^n}{(2n+1)!} x^{2n+1}$ |                                                             |
|     $cos(x)$     | $\sum_{n=0}^{\infty} \frac{(-1)^n}{2n} x^{2n}$        |                                                             |
|     $sh(x)$      | $\sum_{n=0}^{\infty} \frac{1}{(2n+1)!} x^{2n+1}$      |                                                             |
|     $ch(x)$      | $\sum_{n=0}^{\infty} \frac{1}{(2n)!} x^{2n}$          |                                                             |
| $(1+x)^{\alpha}$ |                                                       |                                                             |
### Formule de Taylor-Young
$$
\begin{align*}
f(x) &\approx \sum_{n=0}^{n} \frac{f^{(n)}(a)}{n!} (x-a)^{n} \\
f(x) &\approx f(a) + \frac{f'(a)}{1!}(x-a)+\frac{f''(a)}{2!}(x-a)^2+...+\frac{f^{(n)}(a)}{n!}(x-a)^n + o(x^n)
\end{align*}
$$
