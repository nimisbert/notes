Source :
- Département Mathématique et Informatique L1S1, Uni. Blaise Pascal Clermont-Ferrand
## 1. Le symbole de somme $\Sigma$
On défini dans ce paragraphe une notation qui rend plus commode (et moins ambiguë) l'écriture de sommes (finies). Commençons par un exemple. On considère la somme:
$$
10+11+12+...+98+99+100
$$
Donc la somme de tous les entiers entre 10 et 100, que l'on veut écrire sans les pointillés. On se donne alors un paramètre, disons $n$, et une fonction notée par exemple $f$ tels que $f(n)$ décrit exactement l'ensemble des termes de la somme lorsque $n$ varie entre une valeur initiale et une valeur finale. Dans notre exemple, on pose simplement $f(n)=n$ entier compris entre 10 et 100:
$$
10+11+12+...+98+99+100 = \Sigma_{n=10}^{100}n
$$
D'une manière générale, étant donné deux entiers (relatifs) $a\leq b$ et une fonction $f$ (définie sur les entiers entre $a$ et $b$), le symbole:
$$
\Sigma_{n=a}^{b}=f(n)
$$
Ce symbole désigne le résultat obtenu en considérant successivement tous les entiers de $a$ à $b$, en calculant pour chaque tel entier $n$ la valeur $f(n)$ et en ajoutant le résultat à la somme précédemment calculée:
$$
\Sigma_{n=a}^{b}=f(a)+f(a+1)+...+f(b-1)+f(b)
$$
### 1.1. Exemples
Calculer les sommes suivantes:
$$
\Sigma_{k=-3}^{5}2^k, \quad \Sigma_{m=3}^{8}(-2+3m), \quad \Sigma_{j=0}^{5}(3j^2+1)
$$
Écrire avec le symbole de somme les formules suivantes:
$$
\begin{split}
2+4+6+...+98+100 \\
\frac{1}{2}-\frac{1}{3}+\frac{1}{4}-\frac{1}{5}+\frac{1}{6}-\frac{1}{7}+\frac{1}{8}-\frac{1}{9}+\frac{1}{10} \\
1+2^2 +3^2+...+30^2\\
\frac{3}{4}+\frac{4}{3}+\frac{4}{5}+\frac{5}{4}+\frac{5}{6}+\frac{6}{5}+\frac{6}{7}+\frac{7}{6}+\frac{7}{8}+\frac{8}{7}
\end{split}
$$
### 1.2. Remarques sur la variable muette 
Noter que dans l'écriture la variable $n$ m'intervient pas dans le résultat. On parle de variable "muette". On peut en particulier lui donner le nom que l'on souhaite. Ainsi on a par exemple:
$$
\Sigma_{n=-2}^5 = \Sigma_{k=-2}^5
$$
Rien n'empêche en revanche d'avoir des bornes de sommation qui dépendent d'une variable donnée. Par exemple, on peut considérer, comme dans l'exemple ci-dessus, la somme des $n$ premiers entiers naturels impairs avec un $n$ entier naturel $n\geq 1$ quelconque. Avec le symbole $\Sigma$, elle s'écrit:
$$
1+3+...+(2n-1)=\Sigma_{k=1}^{n}(2k-1)
$$
### 1.3. Exemple 
Soit $n$ un entier naturel $\geq 2$. Écrire avec le symbole $\Sigma$ la somme:
1. des inverses des entiers naturels non nuls inférieurs ou égaux à $n$
2. des entiers naturels pairs inférieurs ou égaux à $n$
3. des $n$ premiers cubes d'entiers naturels non nuls
4. des $n$ premiers entiers naturels de la forme $3k+1$ entier.
Que valent ces sommes pour $n=2$, $n=3$ ?

### 1.4. Changement de variable dans une somme 
Il est possible d'effectuer des changement de variables dans une somme. Par exemple, en effectuant le changement de variables $k'=k+1$ dans la somme suivante: 
$$
\begin{split}
\Sigma_{k=0}^{n-1}2^k = \Sigma_{k=1}^{n}2^{k'-1}\\
\end{split}
$$
Si le procédé est surprenant au premier abord, c'est néanmoins totalement licite (comme on peut s'en convaincre en développant la somme ci-dessus) et extrêmement utile dans la pratique.