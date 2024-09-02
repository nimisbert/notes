[[Pb-007 10001st Prime]]

Un nombre composé de 1000 chiffres est fourni en donné. Le plus grand produit composé de quatre chiffres consécutifs (dans ce nombre) est $9 \times 9 \times 8 \times 9 = 5832$. Déterminer le produit pour $13$ chiffres consécutifs.

Considérons une fenêtres de $n$ chiffres à inspecter. Il reste $1000-n$ chiffres à inspecter. 
Pour $i$ opérations allant de $0$ à $1000-n$ on doit effectuer le produit des $n$ nombres de la fenêtre. 
Si le produit est supérieur on modifie la réponse de la fonction calculant la réponse au problème.

[[Pb-009 Special Pythagorean Triplet]]