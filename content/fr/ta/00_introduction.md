---
book: ta
book_title: Topologie algébrique
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: fr
source: ta-i-iv-fr
pdf_pages: 0012-0015
extraction: native
statements: 0
exercises: 0
content_sha256: bac57c1565b556784f0c497ef2fe5450c8af0eb67cb4ae628bbae4dc7752d614
---

## INTRODUCTION

La Topologie algébrique vise à étudier les espaces topologiques en leur associant fonctoriellement diverses structures algébriques (modules, groupoïdes, etc.) dont les propriétés reflètent celles des espaces considérés.

Les chapitres I à IV de ce Livre concernent la théorie des revêtements et du groupe de Poincaré ; ils aboutissent à une formulation générale du théorème de van Kampen. Les chapitres suivants traiteront d’homologie et de cohomologie, des groupes d’homotopie supérieurs et des espaces cellulaires.

La notion de revêtement fait l’objet du chapitre I. Bien que cette notion porte sur certaines applications continues $p: E\rightarrow B$, où E et B sont des espaces topologiques, la terminologie adoptée considère que l’espace E est le revêtement, l’espace B étant sa base, et l’application $p$ est le plus souvent sous-entendue. Nous sommes ainsi amenés à étudier de façon générale la structure de B-espace (§1). Les B-espaces étalés sont définis au §2, mais il est souvent utile de les étudier du point de vue équivalent des faisceaux sur B (§3). La notion d’espace fibré localement trivial est introduite au §4 ; ce sont les B-espaces localement isomorphes à un produit $B\times F$, où la fibre F est un espace topologique. Les revêtements sont ceux dont la fibre est un espace topologique discret. Au §5, nous définissons la notion de revêtement galoisien et démontrons que si la base B est non vide, connexe et localement connexe, tout revêtement est associable à un revêtement galoisien. Les espaces simplement connexes sont définis au §6 : ce sont ceux dont tout revêtement est trivialisable ; un intervalle de $\mathbf{R}$, une partie convexe de

xi l’espace numérique $\mathbf{R}^n$, la sphère $\mathbf{S}_n$ de dimension $n\geqslant 2$ sont des espaces simplement connexes, mais pas le cercle $\mathbf{S}_1$.

La notion algébrique de groupoïde est définie au chapitre II ; elle généralise celle de groupe et avait été introduite par H. Brandt dans son étude des idéaux fractionnaires inversibles des algèbres de quaternions. Les notions de carquois, graphes et catégories sont définies aux §1, 2 et 3 du chapitre II ; un groupoïde est une catégorie dont toute flèche est inversible. Les résultats des §4 et 5 permettront de déduire du théorème de van Kampen, formulé en termes de groupoïdes, des présentations explicites des groupes de Poincaré dans diverses situations.

La classification des revêtements d’un espace topologique donné B se fait par l’introduction, au chapitre III, §3, de son groupoïde de Poincaré $\varpi (B)$, qui est défini en termes de classes d’équivalences de chemins dans B modulo la relation d’homotopie stricte. Lorsque $b$ est un point de B, le groupe de Poincaré $\pi_1(B, b)$ apparaît comme le groupe d’isotropie en $b$ du groupoïde $\varpi (B)$. La notion d’homotopie est introduite au §1 ; on y étudie en particulier l’importante propriété d’extension des homotopies. Le §2 est consacré à la notion de chemin dans un espace topologique et aux notions d’espace connexe par arcs et d’espace localement connexe par arcs. On y établit aussi un théorème de relèvement des chemins.

Le lien entre homotopie et revêtements est étudié aux §4 et 5. Si E est un revêtement d’un espace topologique B et si $b\in B$, la fibre $E_b$ est munie d’une opération naturelle du groupe $\pi_1(B, b)$ ; cette construction donne lieu à un foncteur de la catégorie des revêtements de B dans celle des ensembles munis d’une action de $\pi_1(B, b)$. Lorsque B est un espace topologique connexe et localement connexe par arcs, ce foncteur est pleinement fidèle ; son image est constituée des opérations du groupe $\pi_1(B, b)$ sur un ensemble discret qui sont continues pour une certaine topologie, dite « admissible », sur le groupe $\pi_1(B, b)$.

Le chapitre IV est consacré aux espaces délaçables ; ce sont les espaces topologiques localement connexes par arcs pour lesquels la topologie admissible des groupes de Poincaré est la topologie discrète. Pour ces espaces, la correspondance entre revêtements et opérations du groupe de Poincaré est ainsi parfaite : le foncteur décrit ci-dessus fournit une équivalence de catégories entre la catégorie des revêtements de B et celle des ensembles munis d’une opération du groupe $\pi_1(B, b)$.

xii

On dit qu’un espace topologique B est simplement connexe par arcs s’il est connexe par arcs et si le groupe $\pi_1(B, b)$ est trivial pour tout point $b$ de B. On démontre qu’un espace délaçable non vide possède un revêtement universel qui est simplement connexe par arcs et galoisien. On prouve aussi que le groupe de Poincaré d’un espace topologique compact et délaçable est de présentation finie (§2) ; sans l’hypothèse que l’espace est délaçable, ce groupe de Poincaré peut avoir la puissance du continu (théorème de Shelah). On démontre au §3 que le groupe de Poincaré en l’élément neutre d’un groupe topologique connexe est abélien et (dans le cas délaçable) que son revêtement universel possède une structure naturelle de groupe topologique.

Lorsque $f: Y\rightarrow$ X est une application continue et E est un Y-espace, on décrit au §4 en termes de données de descente les éventuels X-espaces dont E provient par changement de base. Nous traduisons ainsi dans le cadre de la Topologie générale un procédé utilisé systématiquement par A. Grothendieck en Géométrie algébrique. On donne aussi des conditions garantissant qu’un revêtement de Y provient d’un revêtement de X. Sous certaines hypothèses sur $f$, cela permet de démontrer la formulation générale du théorème de van Kampen : le groupoïde de Poincaré de X est isomorphe à un certain groupoïde (coégalisateur, chapitre II, §5) construit à l’aide du groupoïde de Poincaré de Y et de celui du carré fibré $Y\times_XY$.

Pour les applications, il est toutefois nécessaire d’en déduire une présentation du groupe de Poincaré de X en un point. Au §5, on applique ainsi les calculs généraux du chapitre II pour obtenir de telles présentations dans de nombreux exemples. On y calcule en particulier le groupe de Poincaré de X lorsqu’on s’est donné un recouvrement de X par une famille de parties ouvertes et connexes par arcs. Ainsi que l’a notamment montré R. Brown, le point de vue des groupoïdes permet de ne faire aucune hypothèse sur la connexité des intersections deux à deux de ces parties. Sous certaines conditions de délaçabilité, on traite également le cas de recouvrements localement finis de X par des parties fermées. On y calcule aussi le groupe de Poincaré du quotient d’un espace délaçable par l’action propre et libre d’un groupe discret. On y explicite enfin le théorème originel de van Kampen, sous des hypothèses un peu différentes.

Enfin, on étudie au §6 la notion d’espace classifiant pour un groupe topologique G : lorsqu’on dispose d’un tel espace $B_G$, l’étude des classes

xiii d’isomorphisme d’espaces fibrés principaux de groupe G et de base paracompacte B se traduit en un problème d’étude des classes d’homotopies d’applications de B dans $B_G$. Lorsque G est discret, on construit un espace classifiant qui est un espace métrisable.

Les résultats des chapitres I à IV dépendent des quatre premiers Livres (E, A, TG, FVR) ; certains exemples et remarques utilisent en outre des résultats d’EVT, VAR, LIE III et LIE IV.

Il était initialement prévu que ce Livre fît l’objet du chapitre XI du Livre de Topologie générale. Dans les Livres précédents, les références à TG, XI, doivent ainsi être modifiées comme suit :

LIE, III, §1, n°9, p. 114, note 1. Lire « Cf. TA, IV, p. 379, prop. 6. »

LIE, III, §6, p. 192, note 1. Lire « Rappelons (TA, I, p. 124, déf. 3) qu’un espace

est dit simplement connexe si chacun de ses revêtements est trivialisable ;

un espace simplement connexe est connexe. Rappelons aussi (TA, I, p. 100,

cor. 3) que si $G_1,G_2$, sont des groupes topologiques connexes, si $\varphi$ est un

homomorphisme continu ouvert de $G_1$ sur $G_2$ à noyau discret, et si $G_2$ est

simplement connexe, alors $\varphi$ est un homéomorphisme. »

LIE, III, §6, n°7, p. 206, ligne 11. Au lieu de « d’après TG, XI », lire « d’après

TA, IV, p. 379, prop. 6 ».

LIE, VII, p. 66, appendice II, exercice 1. Au lieu de « TG, XI », lire « TA, I,

p. 69, déf. 2 ».

LIE, IX, §2, n°4, p. 12, ligne $-9$. Au lieu de « TG, XI, à paraître », lire « TA,

VII, à paraître ».

LIE, IX, §3, n°6, p. 22. Au lieu de « TG, XI, à paraître », lire « TA, I, p. 127,

exemple 3 ».

LIE, IX, §4, n°2, p. 27, ligne 11. Au lieu de « TG, XI, à paraître », lire « TA,

VII, à paraître ».

LIE, IX, §4, n°6, p. 34, ligne $-6$. Au lieu de « TG, XI, à paraître », lire « TA,

VII, à paraître ».

LIE, IX, §4, n°9, p. 39, ligne 13. Au lieu de « TG, XI, à paraître », lire « d’après

TA, IV, p. 379, prop. 6 ».

LIE, IX, §5, n°4, p. 51, ligne $-13$. Au lieu de « TG, XI, à paraître », lire « d’après

TA, IV, p. 358, exemple ».

LIE, IX, §5, n°4, p. 51, ligne $-4$. Au lieu de « cf. TG, XI, à paraître », lire « TA,

I, p. 106, exemple 4 et p. 111, prop. 10 ».

LIE, IX, §9, n°1, p. 89, ligne 9. Au lieu de « d’après TG, XI », lire « d’après TA,

I, p. 37, th. 2 ».

LIE, IX, p. 112, exercice 8. Au lieu de « TG, XI », lire « TA, VII ».

LIE, IX, p. 118, exercice 2. Au lieu de « TG, XI », lire « TA, III, p. 229, déf. 1 ».

xiv
