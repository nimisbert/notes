## 1. - Circuit de résistances
Avec les circuits parfaitement linéaire ont peut appliquer le théorème de superposition. Considérer toutes les sources (une à une) et faire la somme de leurs contributions pour déterminer le signal de sortie.
Considérons $e_2$ à la masse, $R_2$ en parallèle avec $R_3$, noté $R_{23}$, en série avec $R_1$:
$$
\begin{align*}
e_1 &= U_{R_1} + s  \\
e_1 &= iR_1 + iR_{23} \\
i &= \frac{e_1}{R_1+R_{23}} \\
s &= iR_{23} \\
s &= e_1 \frac{R_{23}}{R_1+R_{23}}
\end{align*}
$$
Idem pour $e_2$, en considérant $e_1$ à la masse on obtient $R_1$ en parallèle avec $R_3$, noté $R_{13}$  :
$$
s = e_2 \frac{R_{13}}{R_2+R_{13}}
$$
Avec le théorème de superposition, en considérons $e_1$ et $e_2$ activent:
#1-1
$$
s = e_1 \frac{R_{23}}{R_1+R_{23}} + e_2 \frac{R_{13}}{R_2+R_{13}}
$$
Avec SPICE on peut vérifier l'état d'un circuit en statique avec l'opérateur de commande $.op$ et comparé le résultat à la formule analytique #1-1 , avec une application numérique, soit:
$$
\begin{align*}
e_1 &= 1.0 V \\
e_2 &= 2.0 V \\
R_1 &= 3.3 k\ohm \\
R_2 &= 6.8 k\ohm \\
R_3 &= 4.7 k\ohm \\
s &= 0.901 V
\end{align*}
$$
## 2. - Intégrateur RC
On cherche la réponse harmonique (fonction de transfert dans le domaine fréquentiel), d'un intégrateur tel que, $R = 3.3 k\ohm$ et $C = 10 nF$.
$$
\begin{align*}
Z_R &= R \\
Z_C &= \frac{1}{j\omega C}
\end{align*}
$$
Comme le circuit précédent, mais avec des impédances, on à:
$$
\begin{align*}
\mathbf{i} &= \mathbf{e} \frac{1}{Z_R + Z_C} \\
\mathbf{s} &= \mathbf{i}Z_C \\
\mathbf{s} &= \mathbf{e} \frac{Z_C}{Z_R + Z_C} \\
\mathbf{s} &= \mathbf{e} \frac{1}{j\omega RC + 1 } \\
\mathbf{H}(j\omega) &= \frac{1}{1+j\omega RC}
\end{align*}
$$
Pour déterminer la réponse en fréquence ont peut traiter les asymptotes:
$$
\begin{align*}
\omega \rightarrow 0 &: \mathbf{H}(j\omega) \approx 1 \\
\omega \rightarrow +\infty &: \mathbf{H}(j\omega) \approx 0 
\end{align*}
$$
Avec une pente de $-20dB/décades$, avec une intersection à:
$$
\begin{align*}
\omega_{fc} &= \frac{1}{RC} = 30303 rad.s^{-1}\\
f_{fc} &= \frac{1}{2\pi RC} = 4822 Hz
\end{align*}
$$
Avec SPICE on peut représenter la réponse en fréquence avec l'opérateur de commande $.ac$ et comparé le graphique avec les résultats numériques.
## 3. - Circuit LR
On cherche à déterminer la forme d'onde du circuit $LR$, donc une solution exprimant le signal de sortie en fonction du signal d'entré dans le domaine temporel. Tel que $E_0 = 3V$ un échelon de tension à $t=0s$, $R=50 \ohm$ et $L = 1 mH$. 
$$
\begin{align*}
e(t) &= Ri(t) + L\frac{di(t)}{dt} \\
i(t) &= \frac{E_0}{R}(1-e^{-t/\tau}) \\
\tau &= \frac{L}{R}
\end{align*}
$$
En utilisant les transformés de Laplace:
$$
\begin{align*}
U_R(p) &= RI(p) \\
U_L(p) &= pLI(p) \\
E(p) &= U_L(p) + U_R(p) \\
E(p) &= (R+pL)I(p) \\
I(p) &= \frac{E(p)}{R+pL} \\
\end{align*}
$$En utilisant la décomposition en éléments simples:
$$
\begin{align*}
I(p) = \frac{E_0}{R}(\frac{1}{p}-\frac{1}{(R/L) + p})
\end{align*}
$$
Se qui devient, avec les tables de transformées de Laplace:
$$
\begin{align*}
i(t) &= \frac{E_0}{R}(1-e^{-t/\tau}) \\
\tau &= L/R = 20\micro s
\end{align*}
$$
## 4. - Exercices
## 4.1. - Montage de résistances
Un montage de 3 sources et 4 résistances tel que:
$$
\begin{align*}
R_1 &= 3.3 k\ohm \\
R_2 &= 6.8 k\ohm \\
R_3 &= 4.7 k\ohm \\
R_4 &= 2.2 k\ohm \\
e_1 &= 1V \\
e_2 &= 2V \\
i_1 &= 1mA
\end{align*}
$$
Comme dans le cas 1. on applique la superposition et on fixe à la masse les sources, une à une. Pour le cas de $e_1$ seule:
$$
\begin{align*}
&R_1 + (R_2//R_3//R_4) \\
&R_{234} = \frac{R_2R_3R_4 + R_3 + R_4}{R_2R_4+R_3R_4}
\end{align*}
$$ 