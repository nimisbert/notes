[[Pb-008 Largest Product in a Series]]

Un triplet Pythagoricien est un triplet de nombre $0 < a < b < c$ tel que:
$$
a^2 + b^2 = c^2
$$
Par exemple:
$$
3^2 + 4^2 = 5^2
$$
Il existe un unique triplet tel que $a + b + c = 1000$. Déterminer le triplet ?

Génération de triplets Pythagoricien:
$$
\begin{align*}
z     &= p + iq \\
z^2   &= p^2 - q^2 + 2pqi \\
|z^2| &= \sqrt{(p^2-q^2)^2 + (2pq)^2} \\
|z|^2 &= \sqrt{p^2 + q^2} \\
|z|^2 &= |z^2|
\end{align*}
$$
On en déduit le que $a, b, c$ est un triplet Pythagoricien si:
$$
\begin{align*}
a &= p^2 - q^2 \\
b &= 2pq \\
c &= p^2 + q^2 
\end{align*}
$$
Avec la formule de contrainte:
$$
\begin{align*}
a + b + c &= 1000 \\
2p^2 + 2pq &= 1000 \\ 
p(p+q) &= 500 \\
\end{align*}
$$


