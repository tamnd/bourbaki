---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 2
section_title: Une propriété de connexion
appendix: true
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0047-0049
extraction: ocr
statements: 3
exercises: 0
content_sha256: d5fcb33ec953de803fd05646024be670cc378c726ebc7fd900c1b5ec819e8750
---

## APPENDICE II

# Une propriété de connexion

#### Lemme 1 {#lie-vii-a2-lem-1 .statement tag=00XN}

*Soient $X$ un espace topologique connexe et $\Omega$ un ouvert dense dans $X$. Si, quel que soit $x \in X$, il existe un voisinage $V$ de $x$ tel que $V \cap \Omega$ soit connexe, alors $\Omega$ est connexe.*

Soit en effet $\Omega_0$ une partie ouverte et fermée non vide de $\Omega$. Soit $x \in X$ et soit $V$ un voisinage de $x$ tel que $V \cap \Omega$ soit connexe. Si $x \in \overline{\Omega}_0$, on a

$$
(V \cap \Omega) \cap \Omega_0 = V \cap \Omega_0 \neq \emptyset,
$$

donc $V \cap \Omega \subset \Omega_0$. Puisque $\Omega$ est dense dans $X$, $\overline{\Omega}_0$ est donc un voisinage de $x$.

Par conséquent, $\overline{\Omega}_0$ est ouvert et fermé, non vide, et puisque $X$ est connexe, $\overline{\Omega}_0 = X$. Puisque $\Omega_0$ est fermé dans $\Omega$, ceci entraîne $\Omega_0 = \Omega \cap \overline{\Omega}_0 = \Omega$, ce qui prouve que $\Omega$ est connexe.

#### Lemme 2 {#lie-vii-a2-lem-2 .statement tag=00XO}

Soient $U$ une boule ouverte de $\mathbf{C}^n$ et $f : U \to \mathbf{C}$ une fonction holomorphe non identiquement nulle. Soit $A$ une partie de $U$ telle que $f = 0$ sur $A$. Alors $U - A$ est dense dans $U$ et connexe.

La densité de $U - A$ résulte de VAR, R, 3.2.5. Supposons d’abord $n = 1$. Si $a \in A$, le développement de $f$ en série entière au point $a$ (VAR, R, 3.2.1) n’est pas réduit à 0, et on en déduit qu’il existe un voisinage $V_a$ de $a$ dans $U$ tel que $f$ ne s’annule pas sur $V_a - \{a\}$. Ainsi, $a$ est isolé dans $A$, ce qui prouve que $A$ est une partie discrète de $U$, donc dénombrable puisque $U$ est dénombrable à l’infini. Soient $x, y \in U - A$. La réunion des droites affines réelles joignant $x$ (resp. $y$) à un point de $A$ est maigre (TG, IX, § 5, p. 53). Il existe donc $z \in U - A$ tel qu’aucun des segments $[x, z]$ et $[y, z]$ ne rencontre $A$. Les points $x, y, z$ appartiennent donc à une même composante connexe de $U - A$, ce qui démontre le lemme dans le cas $n = 1$. Passons au cas général. On peut supposer que $A$ est l’ensemble des zéros de $f$ (TG, I, p. 81, prop. 1). Soient $x, y \in U - A$ et soit $L$ une droite affine contenant $x$ et $y$. La restriction de $f$ à $L \cap U$ n’est pas identiquement nulle puisque $x \in L \cap U$. D’après ce qui précède, $x$ et $y$ appartiennent à une même composante connexe de $(L \cap U) - (L \cap A)$ donc à une même composante connexe de $U - A$.

#### Lemme 3 {#lie-vii-a2-lem-3 .statement tag=00XP}

Soit $X$ une variété analytique complexe connexe de dimension finie et soit $A$ une partie de $X$ vérifiant la condition:
Pour tout $x \in X$, il existe un germe de fonction analytique $f_x$ non nul en $x$ tel que le germe de $A$ en $x$ soit contenu dans le germe en $x$ de l’ensemble des zéros de $f_x$.
Alors $X - A$ est dense dans $X$ et connexe.

La densité de $X - A$ résulte de VAR, R, 3.2.5. On peut supposer que $A$ est fermé (TG, I, p. 81, prop. 1). Pour tout $x \in X$, il existe un voisinage ouvert $V$ de $x$ et un isomorphisme $c$ de $V$ sur une boule ouverte de $\mathbf{C}^n$ tels que $c(A \cap V)$ soit contenu dans l’ensemble des zéros d’une fonction holomorphe non identiquement nulle sur $c(V)$. D’après le lemme 2, $V \cap (X - A)$ est alors connexe. Compte tenu du lemme 1, ceci prouve que $X - A$ est connexe.

Exercices

Les algèbres de Lie et les modules sur ces algèbres sont supposés de dimension finie sur k; à partir du § 3, on suppose k de caractéristique zéro.
