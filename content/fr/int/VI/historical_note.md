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
pdf_pages: 0100-0102
extraction: ocr
statements: 0
exercises: 0
content_sha256: 96d52c27ef79c471f835881a6b133fbe2f312d467ee0f1b54c23d4222fd1bfd9
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
