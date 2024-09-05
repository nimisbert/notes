Précédent : [[Pb-003 Largest Prime Factor]]
Suivant : [[Pb-005 Smallest Multiple]]

Plus grand palindrome issu du produit de $2$ nombres à $3$ chiffres. Les nombres à $3$ chiffres sont $[100:999]$. Le plus grands produits de ces deux nombres est $998 001$. Donc le plus grands palindrome, est de la forme $abccba$, au maximum composé de $6$ chiffres. Si on exprime un nombre comme la somme d'un produit de puissance de $10$ on a, pour $a,b,c \in [0:9]$:
$$
\begin{align*}
p &= a\times10^6 + b\times10^5 + c\times10^4 + c\times10^3 + b\times10^2 + a\times10^1 \\
  &= a\times100 000 + b\times10000 + c\times1000 + c\times100 + b\times10 + a \\
  &= a\times100001 + b\times10010 + c\times1100 \\
  &= 11(9091a + 910b + 100c)
\end{align*}
$$
Donc le résultat recherché est un multiple de $11$. Pour le calcul, on cherche le plus grands palindrome donc commencer les boucles par $990$ et décrémenter de $11$ en $11$.

Pour le Palindrome, convertir en chaîne de caractères. #palindrome