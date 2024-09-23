## 1. - Double cellule RC
Un circuit composé de deux circuits RC en cascade:
$$
\begin{align*}
R_1 &= 2.7 k\ohm \\
C_1 &= 220 nF \\
R_2 &= 1.2 k\ohm \\
C_2 &= 22 nF \\
R_3 &= 2.2 k\ohm
\end{align*}
$$
En Laplace, les impédances sont de la forme:
$$
\begin{align*}
Z_R(p) &= R \\
Z_L(p) &= pL \\
Z_C(p) &= \frac{1}{pC}
\end{align*}
$$
On cherche la fonction de transfert de $T(p)$, d'abord sans la résistance $R_3$. Avec Thévenin sur le premiers circuit $RC$:
