[[Pb-005 Smallest Multiple]]

La somme du carré de chaque nombre naturels allant de $1$ à $10$ est:
$$
1^2 + 2^2 + 3^3 ... + 10^2 = 385
$$
Le carré de la somme de chaque nombre naturel allant de $1$ à $10$ est:
$$
(1+2+3+...+10)^2 = 55^2 = 3025
$$
La différence des deux termes précédents est:
$$
3025 - 385 = 2640
$$
Trouver le résultat pour les naturels pour $[1:100]$.

Le problème est directement en lien avec [[Pb-001 Multiples of 3 or 5]]. Notamment pour la somme des entiers allant de $1$ à $n$. Or ici on cherche $x$ pour $n$:
$$
x = (\sum_{k=1}^{n}k)^2 - \sum_{k=1}^{n}k^2
$$
Bloquer par le développement du carré de la somme car le développement de $(n-1)^2$, fait intervenir à nouveau une somme de carré qui dépends de la variable muette $k$. Sur internet, une solution est expliqué en considérant le cube pour utilisé l'identité: $(n+1)^3 = n^3 + 3n^2 + 3n +1$.
Soit, les suites:
$$
\begin{align*}
\sum_{k=1}^{n}k &= S_n = 1 + 2 + 3 + ... + n  \\
\sum_{k=1}^{n}k^2  &= S_n^2 = 1^2 + 2^2 + 3^2 + ... + n^2 \\
\sum_{k=1}^{n}k^3 &= S_n^3 = 1^3 + 2^3 + 3^3 + ... + n^3 
\end{align*}
$$
Si on applique l'identité remarquable à chaque terme de la somme des cube pour $n+1$ ($S_{n+1}^3$), on obtient:
$$
\begin{align*}
(n+1)^3 &= n^3 + 3n^2 + 3n + 1 \\
(n+0)^3 &= (n-1)^3 + 3(n-1)^2 + 3(n-1) + 1 \\
(n-1)^3 &= (n-2)^3 + 3(n-2)^2 + 3(n-2) + 1 \\
&... \\
3^3 &= 2^3 + 3\times2^2 + 3\times2 + 1 \\ 
2^3 &= 1^3 + 3\times1^2 + 3\times1 + 1 \\
1^3 &= 0^3 + 3\times0^2 + 3\times0 + 1 \\
\end{align*}
$$
Soit la somme des termes de gauche de l'égalité est égal à $S_{n+1}^3$ on peut recomposé cette somme avec les autres suites:
$$
\begin{align*}
S_{n+1}^3 &= S_n^3 + 3 S_n^2 + 3S_n + n+1 \\
S_{n+1}^3 - S_n^3 &= 3S_n^2 + 3S_n + n+1 \\
(n+1)^3 &= 3S_n^2 + 3S_n + n + 1 \\
3S_n^2 &= -3S_n-n-1+(n+1)^3 \\
3S_n^2 &= -3\frac{n(n+1)}{2}-n-1+n^3+3n^2+3n+1 \\
6S_n^2 &= -3n(n+1)-2n-2+2n^3+6n^2+6n+2 \\
6S_n^2 &=  -3n^2-3n-2n-2+2n^3+6n^2+6n+2 \\
6S_n^2 &= 2n^3 + 3n^2 + n\\
6S_n^2 &= n(2n^2+3n +1 )\\
6S_n^2 &= n(n+1)(2n+1)\\
S_n^2 &= \frac{n(n+1)(2n+1)}{6} \\
\sum_{k=1}^{n}k &= \frac{n(n+1)(2n+1)}{6} \\
\end{align*}
$$
Donc pour résoudre le problème:
$$
\begin{align*}
(\sum_{k=1}^{n}k)^2 - \sum_{k=1}^{n}k^2 &= (\frac{n(n+1)}{2})^2 - \frac{n(n+1)(2n+1)}{6} \\
&= \frac{n^2(n+1)^2}{4} - \frac{2n^3+3n^2+n}{6} \\
&= \frac{n^2(n^2+2n+1)}{4} -  \frac{2n^3+3n^2+n}{6} \\
&= \frac{n^2(n^2+2n+1)}{4} -  \frac{2n^3+3n^2+n}{6} \\
&= \frac{n^4+2n^3+n^2}{4} -  \frac{2n^3+3n^2+n}{6} \\
&= \frac{6n^4 + 12n^3 + 6n^2 - 8n^3-12n^2-4n}{24} \\
&= \frac{6n^4 + 4n^3 - 6n^2-4n}{24} \\
&= \frac{3n^4 + 2n^3 - 3n^2-2n}{12} \\
\end{align*}
$$
[[Pb-007 10001st Prime]]