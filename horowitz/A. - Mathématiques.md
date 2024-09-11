## A.1. - Trigonométrie, exponentiels, logarithmes
__Formules Quadratiques__ #A-1-1 
$$
\begin{align*}
& ax^2 + bx + c = 0 \\
& x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\end{align*}
$$
__Formules Trigonométriques__ #A-1-2
$$
\begin{align*}
sin(x \pm y) &= sin(x)cos(y) \pm cos(x)sin(y) \\
cos(x \pm y) &= cos(x)cos(y) \mp sin(x)sin(y) \\
sin(2x) &= 2sin(x)cos(x) \\
cos(x)cos(y) &= \frac{1}{2}[cos(x+y)+cos(x-y)] \\
sin(x)sin(y) &= \frac{1}{2}[sin(x+y)-sin(x-y)] \\
sin(x)sin(y) &= \frac{1}{2}[cos(x-y)-cos(x+y)]
\end{align*}
$$
__Formules Exponentiels__ #A-1-3
$$
\begin{align*}
e^{x+y} &= e^x e^y \\
e^{x-y} &= e^x / e^y \\
x^{a/b} &= \sqrt[b]{x^a}
\end{align*}
$$
__Formules Logarithmiques__ #A-1-4
$$
\begin{align*}
\log_e &= ln \\
e^{\log_{e}x} &= x \\
\log_e(xy) &= \log_e(x) + \log_e(y) \\
\log_e(x/y) &= \log_e(x) - \log_e(y) \\
\log_e(x^n) &= n\log_e(x) \\
\log_e(e^x) &= x \\
\log_e(x) &= \log_e \log_{10}(x) \\
a^x &= e^{x\log_e(a)}
\end{align*}
$$
## A.2. - Nombres complexes
Notation des complexes en gras dans le livre de Horowitz, et du conjugué avec $*$.
Les normes de notation $EE$ change la notation standard du complexe $i$ par $j$.
Soit:
__Nombres complexes__ #A-2-1
$$
\begin{align*}
& \mathbf{N} = a + jb \\
& \mathbf{N}^* = a - jb \\
& |\mathbf{N}| = \sqrt{\mathbf{N}\mathbf{N}^*} = |a+jb| = \sqrt{a^2+b^2}
\end{align*}
$$
__Formules sur les complexes__ #A-2-2
$$
\begin{align*}
(a+jb) + (c + jd) &= (a+c)+j(b+d) \\
(a+jb) - (c + jd) &= (a-c)+j(b-d) \\
(a+jb) (c+id) &= (ac-bd)+j(bc+ad) \\
\frac{a+jb}{c+jd} &= \frac{(a+jb)(c-jd)}{(c+jd)(c-jd)} = \frac{ac+bd}{c^2 + d^2} + j \frac{bc - ad}{c^2 + d^2} 
\end{align*}
$$
__Plan complexe__ #A-2-3
En représentation vectorielle dans le plan complexe, tel que $a$ la coordonnée réelle, $b$ la coordonnée imaginaire (coordonnées cartésiennes), $r$ le module, $\theta$ la phase (coordonnées polaires).
$$
\begin{align*}
\mathbf{N} &= a+jb = re^{j\theta} \\
r &= \sqrt{a^2 + b^2} \\
\theta &= tan^{-1}(b/a) 
\end{align*}
$$
__Conversion polaire/cartésienne__ #A-2-4
$$
\begin{align*}
&re^{j\theta} = r\cos(\theta) + jr\sin(\theta) \\
&a = \mathbb{Re}(re^{j\theta}) = r\cos(\theta) \\
&b = \mathbb{Im}(re^{j\theta}) = r\sin(\theta) \\
&\mathbf{N}e^{j\theta} = (a\cos(\theta) - b \sin(\theta)) + j(b\cos(\theta) + a\sin(\theta)) \\
\end{align*}
$$
## A.3. - Dérivation
__Dérivées usuelles__ #A-3-1
$$
\begin{align*}
&\frac{d}{dx}a = 0 \\
&\frac{d}{dx}ax = a \\
&\frac{d}{dx}ax^n = anx^{n-1} \\
&\frac{d}{dx}\sin(ax) = a \cos(ax) \\
&\frac{d}{dx}\cos(ax) = -a \sin(ax) \\
&\frac{d}{dx}e^{ax} = ae^{ax} \\
&\frac{d}{dx}\log_{e}(x) = \frac{1}{x}
\end{align*}
$$
__Combinaison de dérivés__ #A-3-2
$$
\begin{align*}
&\frac{d}{dx}au(x) = a \frac{d}{dx}u(x) \\
&\frac{d}{dx}(u+v) = \frac{du}{dx} + \frac{dv}{dx} \\
&\frac{d}{dx}(uv) = u\frac{dv}{dx} + v \frac{du}{dx} \\
&\frac{d}{dx}(\frac{u}{v}) = \frac{v\frac{du}{dx} - u \frac{dv}{dx}}{v^2} \\
&\frac{d}{dx}\log_eu = \frac{1}{u}\frac{du}{dx} \\
&\frac{d}{dx}(u(v(x))) = \frac{du}{dv}\frac{dv}{dx}
\end{align*}
$$
