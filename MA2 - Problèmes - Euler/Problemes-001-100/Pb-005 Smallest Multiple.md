Précédent : [[Pb-004 Largest Palindrome Product]]
Suivant : [[Pb-006 Sum Square Difference]]

$2520$ est le plus petit nombre divisible par les nombres allant de $1$ à $10$ sans restes.
Quel est le plus petit nombre divisible par les nombres allant de $1$ à $20$ sans restes.

Un nombre $n$ est divisible par $n_0$ si il peut s'exprimer de la forme $n=n_0\times n_1$. Pour le cas de l'exemple:
$$
\begin{align*}
2520 &= 252 \times 10 \\
\end{align*}
$$
Le problème fait référence à la décomposition en produit de #facteurs-premiers du [[Pb-003 Largest Prime Factor]]. Le fait qu'un nombre est une unique décomposition en produit de facteurs premiers:
$$
2520 = 2^3 \times 3^2 \times 5 \times 7
$$
Dans la décomposition on observe que le facteur premier $2$ est multiplier $3$ fois par lui même. Ce qui assure la multiplicité de $2520$ avec:
$$
\begin{align*}
2^1 &= 2 \\ 
2^2 &= 4 \\
2^3 &= 8
\end{align*}
$$
Et le multiple d'un facteur premier avec un autre assure d'autre multiplicité comme:
$$
2520 = 2^2 \times 6 \times 3^1 \times 5 \times 7
$$
Et la séquence contient au moins tous les nombres premiers entre $[1:20]$ puisque uniquement divisibles par eux-mêmes. Soit $2,3,5,7,11,13,17,19$.
Donc on peut reproduire une tel séquence et permutations pour déduire un nombre divisible par les nombres de $[1:20]$ soit:
$$
\begin{align*}
2^4 &\implies 2, 4, 8, 16 \\
3^2 &\implies 3, 9, 6(2), 12(2^2), 18(2) \\
5   &\implies 5, 10(2), 15(3), 20(2^2) \\
7   &\implies 7, 14(2) \\
11  &\implies 11 \\
13  &\implies 13 \\
17  &\implies 17 \\
19  &\implies 19 \\
\end{align*}
$$
Donc le nombre recherche est:
$$
s = 2^4 \times 3^2 \times 5 \times 7 \times 11 \times 13 \times 17 \times 19
$$

