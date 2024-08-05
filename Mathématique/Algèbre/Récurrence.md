Source :
- Département Mathématique et Informatique L1S1, Uni. Blaise Pascal Clermont-Ferrand
## 1. Le Principe de Récurrence
### 1.1. Proposition du principe de récurrence
Soit $P(n)$ un énoncé dépendant d'un paramètre entier relatif à n. 
Si $P(n_0)$ est vrai pour un entier relatif $n_0$ et s'il est prouvé que lorsque $P(n)$ est vrai pour un entier $n$ supérieur ou égale à $n_0$, $P(n+1)$ est vrai aussi, alors $P(n)$ est vrai pour tous les entiers supérieurs ou égaux à $n_0$.

### 1.2. Remarque sur le principe de récurrence 
Il faut bien comprendre la phrase "s'il est prouvé que lorsque $P(n)$ est vrai pour un entier $n$ supérieur ou égal à $n_0$, $P(n+1)$ est vrai aussi". Elle ne dit absolument pas qu'on suppose $P(n)$ vrai pour tout $n \geq n_0$ ! Elle dit qu'on suppose vraie l'implication "si $P(n)$ vrai alors $P(n+1)$ est vrai". Avoir en tête l'analogie "si vous travaillez bien vous aurez de bons résultats" est vraie mais qu'elle ne dit pas que vous travaillerez bien.

### 1.3. Exemple de récurrence  
Un raisonnement par récurrence contient plusieurs étapes _initialisation_ et _hérédité_. 
#### 1.3.1. Énoncé 
Soit $n$ un entier $\geq 1$ et $P(n)$ l'énoncé :
$$
1+2+...+n = \frac{n(n+1)}{2}
$$
#### 1.3.2. Initialisation
On démontre l'énoncé au premier rang, ici pour $n=1$ soit on vérifie que $P(1)$ est vrai. En effet, d'une part la somme des entiers de 1 à 1 vaut 1 et, d'autre part, $\frac{1+1}{2}=1$. D'où $P(1)$ vrai.

#### 1.3.3. Hérédité
On suppose désormais que l'énoncé $P(n)\implies P(n+1)$ est vrai pour $n\geq 1$. calculons la somme de tous les entiers de $1$ à $n+1$. On a :
$$
\begin{split}
1+2+...+n+1 = (1+2+...+n) + (n+1) \\
= \frac{n(n+1)}{2}+(n+1) \\
= \frac{(n+1)(n+2)}{2}
\end{split}
$$
Pour tout entier $n \geq 1$ nous avons montré que l'énoncé $P(n)$ vrai, alors l'énoncé $P(n+1)$ est vrai. Nous avons de plus montré que l'énoncé $P(1)$ est vrai. Le principe de récurrence permet de conclure que l'énoncé $P(n)$ est vrai pour tout $n\geq 1$.

### 1.4. Remarque sur le raisonnement de récurrence 
La structure du raisonnement par récurrence est identique quel que soit l'énoncé à démontrer. N'importe quel raisonnement par récurrence prendra donc toujours la forme suivante où valeur initiale désigne un entier (1 dans l'exemple précédent) et où les pointillés sont à compléter en fonction de l'énoncé :
$$
P(n) \quad = \quad ...
$$
### 1.5. Remarque sur les pièges à éviter 
1. L'oubli d'une étape du raisonnement, notamment l'énoncé de la proposition ou de la conclusion.
2. L'énoncé de la proposition de récurrence dépends d'un entier relatif. En particulier celui-ci ne peut en aucun cas contenir une phrase du type "Pour tout entier $n$". De plus l'hérédité ne peut pas débuter par "On suppose $P(n)$ vrai" sans précision car dans ce cas il n'y a plus rien à démontrer.
3. L'hypothèse de récurrence doit servir est être indiqué dans le raisonnement à l'étape de l'hérédité. Si l'hypothèse de récurrence est inutile cela signifie qu'un raisonnement direct suffit pour arrivé à une conclusion.

### 1.6. Exemple 
$$
1+3+...+(2n-1)=n^2
$$
