---
book: int
book_title: Integration
chapter: VI
chapter_title: Intégration vectorielle
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: int-vi-fr
pdf_pages: 0100-0106
extraction: ocr
statements: 0
exercises: 0
content_sha256: 806387d2f2245b8d6371cbeda14cf88eeb5791acb08d92d951fc1a43fd873125
---

# NOTE HISTORIQUE

(N.-B. --- Les chiffres romains renvoient à la bibliographie placée à la fin de cette note.)

Avec le développement du « calcul vectoriel » au cours du xixe siècle, il était courant d’avoir à intégrer des fonctions vectorielles, mais tant qu’il ne s’agissait que de fonctions à valeurs dans des espaces de dimension finie, cette opération ne posait aucun problème. C’est seulement avec la théorie spectrale de Hilbert que l’on rencontre des opérations qui mènent naturellement à une notion plus générale d’intégrale : cette théorie conduit en effet à associer à toute forme hermitienne continue $\Phi(x, y)$ sur un espace hilbertien $\mathbf{H}$, une famille $(E(\lambda))_{\lambda \in \mathbf{R}}$ de projecteurs orthogonaux ayant la propriété que, pour tout couple $(x, y)$ de vecteurs de $\mathbf{H}$, la fonction $\lambda \to (E(\lambda)x | y)$ soit à variation bornée et que l’on ait $\Phi(x, y) = \int \lambda d((E(\lambda)x | y))$; si l’on associe à $\Phi$ l’opérateur hermitien $A$ tel que $\Phi(x; y) = (Ax | y)$, il était tentant d’écrire la formule précédente $A = \int \lambda dE(\lambda)$. Mais c’est seulement à partir de 1935 environ, après l’introduction par Bochner de l’intégration (« forte ») d’une fonction à valeurs dans un espace de Banach, qu’on commença à se préoccuper de définir l’intégrale de fonctions vectorielles (ou l’intégrale par rapport à une mesure vectorielle) de façon à pouvoir écrire légitimement des formules telles que la précédente. Cette extension fut réalisée essentiellement par Gelfand (III), Dunford et Pettis (IV) et (V)); leurs résultats sont énoncés pour des espaces de Banach, mais s’étendent sans peine à des espaces localement convexes plus généraux.

L’idée de décomposer un volume en « tranches » et de ramener une intégrale étendue à ce volume à une intégrale sur chaque tranche, suivie d’une intégration simple, a toujours été utilisée en Analyse depuis les débuts du Calcul infinitésimal (le « Calcul des indivisibles » de Cavalieri n’étant qu’une première ébauche de ce principe, que l’on pourrait même faire remonter à Archimède (v. Note hist. du Livre IV, chap. I-II-III)). Mais dans les applications classiques, les « tranches » étaient toujours de nature très spéciale et très régulière (le plus souvent des parties ouvertes de surfaces analytiques dépendant analytiquement d’un paramètre) ; il ne pouvait d’ailleurs guère en être autrement en l’absence d’une théorie générale de l’intégration. Le problème général de la désintégration d’une mesure fut posé et résolu par von Neumann en 1932, à propos de la théorie ergodique (I) ; presque en même temps (et indépendamment) Kolmogoroff, en posant les fondements axiomatiques de la Théorie des Probabilités, était amené à définir de façon générale la notion de « probabilité conditionnelle » et à en prouver l’existence, problème essentiellement équivalent à celui de la désintégration d’une mesure (II).

(I) J. von Neumann, Zur Operatorenmethode in der klassischen Mechanik, Ann. of Math., (2), t. XXXIII (1932), p. 587-642.
(II) A. Kolmogoroff, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer), 1933.
(III) I. Gelfand, Abstrakte Funktionen und lineare Operatoren, Mat. Sborn., (N. S.), t. IV (1938), p. 235-284.
(IV) N. Dunford, Uniformity in linear spaces, Trans. Amer. Math. Soc., t. XLIV (1938), p. 305-356.
(V) N. Dunford and B. Pettis, Linear operations on summable functions, Trans. Amer. Math. Soc., t. XLVII (1940), p. 323-392.

Les chiffres de référence indiquent successivement le paragraphe et le numéro (ou, exceptionnellement, l'exercice).

F', F'', F'^*, F_\sigma (F espace localement convexe séparé) : Introduction.
\mathcal{K}(T), \mathcal{K}_\mathbf{R}(T), \mathcal{K}_\mathbf{C}(T), \mathcal{K}(T, A), \mathcal{K}_\mathbf{C}(T, A) : Introduction.
$\langle f, z' \rangle, \langle z', f \rangle$ : 1.

\int f d\mu, \int f(t) d\mu(t) (f fonction vectorielle, \mu mesure positive) : 1, 1.

gf, fg (f fonction vectorielle, g fonction scalaire) : 1, 1.

$\mathcal{C}'(T)$ : 1, 6.

\int f dm, \int f(t) dm(t) (f fonction numérique, m mesure vectorielle) : 2, 1 et 2, 2.

g.m (g fonction numérique, m mesure vectorielle) : 2, 1.

$\mathcal{L}(m)$ : 2, 2.

q(m), |m| (q semi-norme, m mesure vectorielle) : 2, 3.

f.\mu (f fonction vectorielle, \mu mesure positive) : 2, 4.

$\mathcal{L}_{F_s}^\infty, L_{F_s}^\infty$ : 2, 5.

\langle f, g \rangle (f, g fonctions vectorielles) : 2, 6.

I_{\Phi, m}, \int f dm (f fonction vectorielle, m mesure vectorielle) : 2, 7.

|m|, \int f dm (m mesure complexe) : 2, 8.

\mathcal{L}_F^p(T, m), \overline{\mathcal{L}}_F^p(T, m), L_F^p(T, m) (m mesure complexe) : 2, 8.

h.m (m mesure complexe) : 2, 8.

\overline{m} (m mesure complexe) : 2, 8.

||m|| (m mesure complexe) : 2, 9.

\pi(m), m_Y, m \otimes m' (m, m' mesures complexes) : 2, 10.

\mathcal{B}(F_1, F_2), r\Phi, l\Phi : App., 1.

E_\sigma, F_\sigma, E'_s, F'_s, \mathcal{B}(E, F) : App., 1.

\Lambda_{F'}^p(T, \mu), M_p, M'_p : 1, exerc. 16.

Les chiffres de référence indiquent successivement le paragraphe et le numéro (ou, exceptionnellement, l'exercice).

Application $m$-propre ($m$ mesure complexe) : 2, 10.
Base (mesure vectorielle de --- $\mu$) : 2, 4.
Base (mesure de --- $m$) : 2, 8.
Bornée (mesure complexe) : 2, 9.
Classe pseudo-image d'une classe de mesures : 3, 2 .
Complexe (mesure) : 2, 8.
Conjuguée (mesure complexe) : 2, 8.
Densité d'une mesure vectorielle par rapport à une mesure positive : 2, 4.
Densité par rapport à une mesure complexe : 2, 8.
Désintégration d'une mesure $\mu$ relativement à une application $\mu$-propre : 3, 1.
Désintégration d'une mesure $\mu$ relative à une pseudo-image de $\mu$ : 3, 3.
Désintégration d'une mesure par une relation d'équivalence mesurable : 3, 5.
Equivalentes (mesures complexes) : 2, 8.
Essentiellement intégrable (fonction) pour une mesure vectorielle : 2, 2.
Fonction essentiellement intégrable pour une mesure vectorielle : 2, 2.
Fonction scalairement bien intégrable : 1, exerc. 19.
Fonction scalairement essentiellement intégrable : 1, 1.
Image d'une mesure complexe : 2, 10.
Imaginaire (partie) d'une mesure complexe : 2, 8.
Induite (mesure complexe) : 2, 10.
Intégrale d'une fonction numérique par rapport à une mesure vectorielle : 2, 2.
Intégrale d'une fonction vectorielle par rapport à une mesure positive : 1, 1.
Intégrale d'une fonction vectorielle par rapport à une mesure vectorielle : 2, 7.
Majorable (mesure, mesure $q$) : 2, 3.
Mesurable (relation d'équivalence) : 3, 4.
Mesurable (section) : 3, 4.
Mesure complexe : 2, 8.
Mesure complexe bornée : 2, 9.
Mesure complexe conjuguée : 2, 8.
Mesure complexe de base $m$ : 2, 8.
Mesure complexe induite : 2, 10.
Mesure complexe produit : 2, 10.
Mesure pseudo-image : 3, 2.
Mesure quotient d'une mesure par une relation d'équivalence : 3, 5.
Mesure réelle : 2, 1.
Mesure scalaire : 2, 1.

Mesure vectorielle : 2, 1.
Mesure vectorielle de base $\mu$ : 2, 4.
Mesure vectorielle majorable : 2, 3.
Mesure vectorielle $q$-majorable : 2, 3.
Mesure vectorielle scalairement de base $\mu$ : 2, 5.
Mesures complexes équivalentes : 2, 8.
Partie imaginaire, partie réelle d'une mesure complexe : 2, 8.
Propre (application $m$) : 2, 10.
Propriété de relèvement : 2, 5.
Propriété (GDF) : 1, 4.
Pseudo-image (classe, mesure) : 3, 2.
Quotient par une relation d'équivalence (mesure) : 3, 5.
Réelle (mesure) : 2, 1
Réelle (partie) d'une mesure complexe : 2, 8.
Relation d'équivalence mesurable : 3, 4.
Relation d'équivalence séparée : 3, 4.
Relèvement (propriété de) : 2, 5.
Scalaire (mesure) : 2, 1.
Scalairement (fonction possédant — une propriété) : 1, 1.
Scalairement bien intégrable : 1, exerc. 19.
Scalairement de base $\mu$ (mesure) : 2, 5.
Scalairement essentiellement intégrable (fonction) : 1, 1 et 2, 10.
Section mesurable : 3, 4.
Séparée (relation d'équivalence) : 3, 4.
Support d'une mesure vectorielle : 2, 1.
Valeur absolue d'une mesure complexe : 2, 8
Vectorielle (mesure) : 2, 1.

CHAPITRE VI. — Intégration vectorielle ............................................. 7
§ 1. Intégration des fonctions vectorielles ................................. 8
    1. Fonctions scalairement essentiellement intégrables ............ 8
    2. Propriétés de l'intégrale d'une fonction scalairement essentiellement intégrable .................................................. 11
    3. Intégrales d'opérateurs .................................................. 14
    4. La propriété (GDF) ....................................................... 17
    5. Applications mesurables et applications scalairement mesurables ................................................................. 21
    6. Applications : I. Extension d'une fonction continue à un espace de mesures ......................................................... 22
    7. Applications : II. Extension à un espace de mesures d'une fonction continue à valeurs dans un espace d'opérateurs .... 25
§ 2. Mesures vectorielles ......................................................... 29
    1. Définition d'une mesure vectorielle ................................. 29
    2. Intégration par rapport à une mesure vectorielle ............... 31
    3. Mesures vectorielles majorables ..................................... 35
    4. Mesures vectorielles de base μ ....................................... 39
    5. Le théorème de Dunford-Pettis ...................................... 42
    6. Dual de l'espace L^1_F (F espace de Banach de type dénombrable). 47
    7. Intégration d'une fonction vectorielle par rapport à une mesure vectorielle ......................................................... 48
    8. Mesures complexes ....................................................... 50
    9. Mesures complexes bornées ........................................... 54
   10. Image d'une mesure complexe ; mesure complexe induite ; produit de mesures complexes ............................................. 55
§ 3. Désintégration des mesures ............................................... 57
    1. Désintégration d'une mesure μ relativement à une application μ-propre ................................................................. 57
    2. Mesures pseudo-images .................................................. 63
    3. Désintégration d'une mesure μ relative à une pseudo-image de μ. 64
    4. Relations d'équivalence mesurables ................................ 66
    5. Désintégration d'une mesure par une relation d'équivalence mesurable ................................................................. 70
Appendice : Compléments sur les espaces vectoriels topologiques ...... 73
    1. Formes bilinéaires et applications linéaires ..................... 73
    2. Quelques types d'espaces ayant la propriété (GDF) ............. 75
Exercices du § 1 ................................................................. 78
Exercices du § 2 ................................................................. 87
Exercices du § 3 ................................................................. 97
Note historique ................................................................. 100
Index des notations ............................................................ 103
Index terminologique .......................................................... 104
Définitions du chapitre VI .................................................. Dépliant
