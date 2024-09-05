Suivant : [[Pb-002 Even Fibonacci Numbers]]
### Identifier les éléments unitaires du problème
Un nombre $n$ est un multiple de $k$ si il peut se décomposé comme le produit de:
$$
m = ki
$$
### Ne pas faire le bourrin avec l'ordinateur
Utilisé les maths pour réduire la complexité de calcul. Tel que:
$$
\begin{align*}
s &= \sum_{i=1}^{\frac{999}{3}}3i + \sum_{i=1}^{\frac{999}{5}}5i - \sum_{i=1}^{\frac{999}{15}}15i \\
&= 3\sum i + 5 \sum i - 15 \sum i
\end{align*}
$$
Or la formule de la somme des entiers de $1$ à $n$ est:
#somme-de-n
$$
\sum_{i=1}^{n}i= \frac{n(n+1)}{2}
$$
Se qui signifie que:
$$
\begin{align*}
s &= 3\sum i + 5\sum i - 15 \sum i \\
  &= 3\frac{333\times334}{2}+ 5\frac{199\times200}{2}-15\frac{66\times67}{2}
\end{align*}
$$
Ce qui transforme $3 \sum$ de $1$ à $1000$ en simple addition, soustraction, multiplication.
