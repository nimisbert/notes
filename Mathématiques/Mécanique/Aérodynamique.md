L'étude des flux de fluide, souvent d'air, appliquants des forces sur un objet.

____
## 1. Les paramètres de l'aérodynamique

### 1.1. Concept de fluide 
Du point de vue de l'aérodynamique, la matière peut-être dans deux états solide ou fluide. Un solide peut résister la déformation sous l'exercice de forces tangentielles par déformation statique. Un fluide ne le peut pas. Le corollaire est la condition de stresse hydrostatique. Un fluide au repos ne subit pas de force tangentielles.
### 1.2. Continuité d'un fluide
L'aérodynamique représente les fluides par des volumes élémentaires. L'approximation de continuité d'un fluide est valide, lorsque le plus petit volume élémentaire contient suffisamment de particules pour déterminer des grandeurs statistiques soient représentatives en tout point du volume. Quantitativement le nombre de Knudsen est utilisé, c'est le rapport entre la distance moyenne libre de particules et une grandeur caractéristique du volume élémentaire. La continuité est valable si $Knudsen>>0.1$ .
### 1.3. Température 
Une grandeur en $[°C]$ ou Kelvin $[K]$ (donc en réalité sans unités), représentant l'agitation des particules d'un corps. Deux corps en contact thermique ne subissant pas de changement d'une propriété observable ont une température égale. Deux corps égaux en température à un troisième corps doivent être égaux en température entre eux. 
### 1.4. Pression
L'amplitude de la force exercé par le mouvement des molécules sur une surface en $[N.m^{-2}]$. Le standard de pression atmosphérique est :
- En unités S.I. $1.01325 N.m^{-2}$
- En unités U.S. $14.696Ibf.in^{-2}=2116.22Ib.in^{-2}$
Beaucoup d'application en aérodynamique s'intéresse à la différence de pression absolue mais les instruments ont pour référence la pression atmosphérique.
### 1.5. Densité 
La masse par unités de volume en $[g.m^{-3}]$. La densité pour un fluide qui respecte la continuité en un point s'exprime :
$$
\rho = lim_{\delta_{(vol)} \rightarrow 0} \frac{\delta_{(mass)}}{\delta_{(vol)}}
$$ 
La relation entre $\rho(composition,T,p)$ est connu comme l'équation d'état d'un fluide. Pour un gaz parfait l'équation d'état est :
$$
\rho = \frac{p}{RT}
$$

Tel que :
- $T$ la température absolue donc en $[K]$ ou $[°R]$
- $p$ la pression du gaz en $[N.m^{-2}]$
- $\rho$ la densité du gaz en $[g.m^{-3}]$
- $R$ est une constante des gaz parfait :
	- En unités S.I. $287.05N.m.kg^{-1}$
	- En unités U.S. $53.34ft.Ibf.Ibm^{-1}.°R$ ou $1716.16ft^2.s^{-R}.°R$
De manière général, pour des véhicules dont la vitesse est supérieur à $100m.s^{-2}$ l'équation d'état pour un gaz parfait n'est pas valable, puisque les forces et moments qui intéresse l'étude résultent d'une variation de pression qui n'est pas constante dans un volume d'étude.
### 1.6. Viscosité
Pour les fluides Newtoniens, la déformation tangentielle est proportionnelle au forces qui la génère, selon un coefficient de viscosité noté $\mu$. Dans certaines applications d'aérodynamiques les fluides peuvent être considéré comme non visqueux. Soit le coefficient de viscosité est suffisamment petit pour considérer des forces résultant de la viscosité du fluide. Pour les température inférieurs à $3000K$ le coefficient de viscosité s'exprime par l'équation de Sutherland :
$$
\mu=1.458\times10^{-6}\frac{T^{1.5}}{T+110.4}
$$
Tel que :
- $T$ la température en $[K]$
- $\mu$ le coefficient de viscosité en $[g.s^{-1}.m^{-1}]$
L'équation permettant de calculé un coefficient de viscosité dépends du modèle employé pour d'écrire les interactions moléculaires. Il existe un abaque pour l'air, créer par Svehla (1962) et comparé aux valeurs de Sutherland.

### 1.7. Viscosité cinématique
Une grandeur représentant la viscosité par rapport à la densité d'un fluide.
$$
v = \frac{\mu}{\rho}
$$
Tel que :
- $\mu$ la viscosité du fluide en $[g.s^{-1}.m]$
- $\rho$ la densité du fluide en $[g.m^{-3}]$
- $v$ la viscosité cinématique $[m^{2}.s^{-1}]$
### 1.8. La vitesse du son
La vitesse à laquelle une perturbation infinitésimale se propage dans un fluide au repos, noté $a$. Pour un gaz parfait :
$$
a = \sqrt{\gamma R T}
$$
Tel que :
- $\gamma$ le rapport de chaleurs spécifique d'un gaz
- $R$ la constante des gaz parfait
- $T$ la température du gaz
Pour des plages de température tel que l'air est assimilable à un gaz parfait, $\gamma = 1.4$. L'équation de la vitesse du son en fonction de la température, devient :
$$
\begin{split}
a = 20.047\sqrt{T} \quad ; \quad [S.I.] \\
a = 49.02\sqrt{T} \quad ; \quad [U.S.]
\end{split}
$$
Tel que :
- $a$ en $[m.s^{-1}]$ ou $[ft.s^{-1}]$
- $T$ en $[K]$ ou $[R]$
