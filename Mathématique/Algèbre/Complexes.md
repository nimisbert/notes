Source :
- Département Mathématique et Informatique L1S1, Uni. Blaise Pascal Clermont-Ferrand

Pour résoudre $n+1=0$, il a fallu sortir sortir de $\mathbb{N}$ et aller dans $\mathbb{Z}$:-1 est un entier relatif qui n'est pas un entier naturel. Pour résoudre $2n=1$, il a fallu sortir de $\mathbb{Z}$ et aller dans $\mathbb{Q}$. Enfin pour résoudre $x^2=2$ il à fallu sortir de $\mathbb{Q}$ et aller dans $\mathbb{R}$. Pour résoudre $x^2=-1$, on va donc construire un ensemble contenant strictement $\mathbb{R}$, muni d'une addition et d'une multiplication aux propriétés analogues à celles que ces opérations ont dans $\mathbb{Q}$ ou $\mathbb{R}$ et dans lequel cette équation a (au moins) une solution: L'ensemble des nombres complexes.
C'est un résultat profond, appelé théorème de D'Alembert-Gauss, que toute équation polynomiale à coefficients complexes admet une solution complexe. Deux cas particuliers sont à considérer dans un premier temps, les équations:
- $ax^2+bx+c=0$ , avec a, b et c des nombres complexes donnés et $a\neq0$
- $x^n=Z$ , avec $n$ entier naturel $\geq2$ et $Z$ nombre complexe donnés 
## 1. Définitions 
### 1.1. Définition d'un nombre complexe
Un nombre complexe est un couple $(a,b)$ de nombres réels. Deux nombres complexes $(a,b)$ et $(a',b')$ sont égaux si, par définition, on à les égalités $a=a'$ et $b=b'$.
Un nombre complexe est donc, par définition, un élément de 
$$
\mathbb{R}^2=\{ (x,y) | x,y \in \mathbb{R}\}
$$
Convenons d'identifier $\mathbb{R}$ au sous-ensemble $\{ (x,0) | x \in \mathbb{R} \}$ de $\mathbb{R}^2$ constitué des couples dont la seconde coordonnée est nulle et de noter par $i$ le nombre complexe $(0,1)$. On a alors:
$$
(a,b)=a(1,0)+b(0,1)=a+bi
$$
Il faut encore définir les lois d'addition et de multiplication sur les nombres complexes dont on a parlé plus haut.

### 1.2. Définition de l'addition 
Si $(a,b)$ et $(c,d)$ sont deux nombres complexes, leur somme est définie comme étant le nombre complexe:
$$
(a,b)+(c,d)=(a+c,b+d)
$$
Autrement dit, on a:
$$
(a+ib)+(c+id)=a+c+i(b+d)
$$
### 1.3. Définition de la multiplication 
Si $(a,b)$ et $(c,d)$ sont deux nombres complexes, leur produit est défini comme étant le nombre complexe:
$$
(a,b)\times(c,d)=(ac-bd,ad+bd)
$$
Autrement dit, on a:
$$
(a+ib)\times(c+id) = ac-bd+i(ad+bc)
$$
#### 1.3.1. Remarque notation du produit 
Lorsque cela n'induit pas d'ambiguïté, on omet bien souvent le symbole $\times$ (ou $\cdot$) et on omet écrit simplement $zz'$ en lieu et place de $z\times z'$ ou $z \cdot z'$
#### 1.3.2. Remarque sur le carré du nombre complexe
En appliquant la définition du produit $i^2=i\times i$, on obtient la formule fondamentale suivante:
$$
i^2=-1
$$
### 1.4. Définition de l'ensemble $\mathbb{C}$
L'ensemble $\mathbb{R}^2$ muni de l'addition et de la multiplication ainsi définies s'appelle l'ensemble des nombres complexes et se note $\mathbb{C}$.
#### 1.4.1. Remarque notation sur les ensembles
Si $\mathbb{K}$ désigne l'un désigne l'un des ensembles $\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$, $\mathbb{R}$ ou $\mathbb{C}$, on note $\mathbb{K}$ ou $\mathbb{K} \setminus \{0\}$
l'ensemble des éléments non nuls de $\mathbb{K}$. L'ensemble des nombres réels positifs se note $\mathbb{R}_+$, celui des réels négatifs $\mathbb{R}_-$. Quant à l'ensemble des réels strictement positifs (resp. strictement négatifs), on le note $\mathbb{R}_+^*$ (resp. $\mathbb{R}_-^*$). On définit de même:
$$
\mathbb{Q}_-=\{ x\in\mathbb{Q} | x \leq 0 \}, \quad \mathbb{Q}_+= \{ x \in \mathbb{Q} | x \geq 0 \}
$$
et:
$$
\mathbb{Q_-^*}= \{ x \in \mathbb{Q} | x < 0 \}, \quad \mathbb{Q_+^*} = \{ x \in \mathbb{Q} | x>0 \}
$$
Noter que la notion "être positif" (ou "être négatif") a bien un sens dans $\mathbb{R}$ (et ses sous-ensembles, comme par exemple $\mathbb{Q}$), mais en aucun cas dans $\mathbb{C}$.
### 1.5. Définition représentation algébrique d'un complexe
Les opérations d'addition et de multiplication dans $\mathbb{C}$ sont définies pour que les calculs se fassent avec les mêmes réflexes que dans $\mathbb{R}$ en ajoutant uniquement la nouvelle règle $i^2=-1$. Nous listons maintenant les règles de calculs dans $\mathbb{C}$. Soit $z,z',z''\in\mathbb{C}$.
