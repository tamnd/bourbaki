---
book: int
book_title: Integration
chapter: VIII
chapter_title: Convolution et représentations
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: int-vii-viii-fr
pdf_pages: 0207-0224
extraction: ocr
statements: 0
exercises: 0
content_sha256: 0d81e65aaa8d165a13d8aa1138b9ae86d0b71f357a8f98b13c043d53a07ec7ca
---

# NOTE HISTORIQUE
(chapitres VII et VIII)

(N.B. — Les chiffres romains renvoient à la bibliographie placée à la fin de cette note.)

Les notions de longueur, d’aire et de volume chez les Grecs sont essentiellement fondées sur leur invariance par les déplacements : « Des choses qui coïncident (ἐφαρμοσονται) sont égales » (Eucl. El., Livre I, « Notion commune » 4); et c’est par un usage ingénieux de ce principe que sont obtenues toutes les formules donnant les aires ou volumes des « figures » classiques (polygones, coniques, polyèdres, sphères, etc.), tantôt par des procédés de décomposition finie, tantôt par « exhaustion » (*). En langage moderne, on peut dire que ce que font les géomètres grecs, c’est démontrer l’existence de « fonctions d’ensembles » additives et invariantes par déplacements, mais définies seulement pour des ensembles d’un type fort particulier. Le calcul intégral peut être considéré comme répondant au besoin d’élargir le domaine de définition de ces fonctions d’ensemble, et, de Cavalieri à H. Lebesgue, c’est cette préoccupation qui sera au premier plan des recherches des analystes; quant à la propriété d’invariance par déplacements, elle passe au second plan, étant devenue une conséquence triviale de la formule

(*) On peut montrer que si deux polygones plans P, P’ ont même aire, il y a deux polygones R ⊃ P, R’ ⊃ P’ qui peuvent être décomposés chacun en un nombre fini de polygones R_i (resp. R'_i) (1 ≤ i ≤ m) sans point intérieur commun, tels que R_i et R'_i se déduisent l’un de l’autre par un déplacement (dépendant de i), et tels que R (resp. R’) soit réunion d’une famille finie de polygones S_j (resp. S'_j) (0 ≤ j ≤ n), sans point intérieur commun, avec S_0 = P, S'_0 = P’, et S_j se déduisant de S_j par un déplacement pour 1 ≤ j ≤ n. Par contre, M. Dehn a démontré (Ueber den Rauminhalt, Math. Ann., t. LV (1902), pp. 465-478) que cette propriété n’est plus valable pour le volume des polyèdres, et que les procédés d’exhaustion employés depuis Eudoxe étaient par suite inévitables.

générale de changement de variables dans les intégrales doubles ou triples et du fait qu'une transformation orthogonale a un déterminant égal à $\pm 1$. Même dans les géométries non-euclidiennes (ou pourtant le groupe des déplacements est différent), le point de vue reste le même : de façon générale, Riemann définit les éléments infinitésimaux d’aire ou de volume (ou leurs analogues pour les dimensions $\geqslant 3$) à partir d’un $ds^2$ par les formules euclidiennes classiques, et leur invariance par les transformations qui laissent invariant le $ds^2$ est donc presque une tautologie.

C’est seulement vers 1890 qu’apparaissent d’autres extensions moins immédiates de la notion de mesure invariante par un groupe, avec le développement de la théorie des invariants intégraux, notamment par H. Poincaré et E. Cartan ; H. Poincaré n’envisage que des groupes à un paramètre opérant dans une portion d’espace, tandis que E. Cartan s’intéresse surtout aux groupes de déplacements, mais opérant dans d’autres espaces que celui où ils sont définis. Par exemple, il détermine ainsi entre autres (II) la mesure invariante (par le groupe des déplacements) dans l’espace des droites de $\mathbf{R}^2$ ou de $\mathbf{R}^3 (*)$; en outre, il signale que de façon générale les invariants intégraux pour un groupe de Lie ne sont autres que des invariants différentiels particuliers, et qu’il est donc possible de les déterminer tous par les méthodes de Lie. Il ne semble pas toutefois que l’on ait songé à considérer ni à utiliser une mesure invariante sur le groupe lui-même avant le travail fondamental de A. Hurwitz en 1897 (V). Cherchant à former les polynômes (sur $\mathbf{R}^n$) invariants par le groupe orthogonal, Hurwitz part de la remarque que, pour un groupe fini de transformations linéaires, le problème se résout aussitôt en prenant la moyenne des transformés s.P d’un polynôme quelconque P par tous les éléments s du groupe ; ce qui lui donne l’idée de remplacer, pour le groupe orthogonal, la moyenne par une intégrale relative à une mesure invariante ; il donne explicitement l’expres-

(*) La mesure invariante sur l’espace des droites du plan avait déjà été essentiellement déterminée à l’occasion de problèmes de « probabilités géométriques », notamment par Crofton, dont E. Cartan ne connaissait probablement pas les travaux à cette époque.

sion de cette dernière à l’aide de la représentation paramétrique par les angles d’Euler, mais observe aussitôt (indépendamment de E. Cartan) que les méthodes de Lie fournissent l’existence d’une mesure invariante pour tout groupe de Lie. Peut-être à cause du déclin de la théorie des invariants au début du xx\textsuperscript{e} siècle, les idées de Hurwitz n’eurent guère d’écho immédiat, et ne devaient être mises en valeur qu’à partir de 1924, avec l’extension aux groupes de Lie compacts, par I. Schur et H. Weyl, de la théorie classique de Frobenius sur les représentations linéaires des groupes finis. Le premier se borne au cas du groupe orthogonal, et montre comment la méthode de Hurwitz permet d’étendre les classiques relations d’orthogonalité des caractères ; idée que H. Weyl combine avec les travaux de E. Cartan sur les algèbres de Lie semi-simples pour obtenir l’expression explicite des caractères des représentations irréductibles des groupes de Lie compacts et le théorème de complète réductibilité (XI\textsuperscript{a}), puis, par une extension hardie de la notion de « représentation régulière », le célèbre théorème de Peter-Weyl, analogue parfait de la décomposition de la représentation régulière en ses composantes irréductibles dans la théorie des groupes finis (XI\textsuperscript{b}).

Un an auparavant, O. Schreier avait fondé la théorie générale des groupes topologiques, et dès ce moment il était clair que les raisonnements du mémoire de Peter-Weyl devaient rester valables tels quels pour tout groupe topologique sur lequel on pourrait définir une « mesure invariante ». À vrai dire, les notions générales sur la topologie et la mesure étaient encore à cette époque en pleine formation, et ni la catégorie de groupes topologiques sur lesquels on pouvait espérer définir une mesure invariante, ni les ensembles pour lesquels cette « mesure » serait définie, ne semblaient clairement délimités. Le seul point évident était qu’on ne pouvait espérer étendre au cas général les méthodes infinitésimales prouvant l’existence d’une mesure invariante sur un groupe de Lie. Or, un autre courant d’idées, issu de travaux sur la mesure de Lebesgue, conduisait précisément à des méthodes d’attaque plus directes. Hausdorff avait prouvé, en 1914, qu’il n’existe pas de fonction d’ensemble additive non identiquement nulle définie pour tous les sous-ensembles de $\mathbf{R}^3$ et invariante par déplacements, et il était naturel de chercher si ce résultat était encore valable pour $\mathbf{R}$ et $\mathbf{R}^2$: problème qui fut résolu par S. Banach en 1923 de façon surprenante, en montrant au contraire que dans ces deux cas une telle « mesure » existait bel et bien (I); son procédé, fort ingénieux, repose déjà sur une construction par induction transfinie et sur la considération des « moyennes »
$$
\frac{1}{n} \sum_{k=1}^{n} f(x + \alpha_k)
$$
de translatées d’une fonction par des éléments du groupe (*). Ce sont des idées analogues qui permirent à A. Haar, en 1933 (IV), de faire le pas décisif, en prouvant l’existence d’une mesure invariante pour les groupes localement compacts à base dénombrable d’ouverts : s’inspirant de la méthode d’approximation d’un volume, en Calcul intégral classique, par une juxtaposition de cubes congruents de côté arbitrairement petit, il obtient, à l’aide du procédé diagonal, la mesure invariante comme limite d’une suite de « mesures approchées », procédé qui est encore essentiellement celui que nous avons utilisé au chap. VII, § 1. Cette découverte eut un très grand retentissement, en particulier parce qu’elle permit aussitôt à J. von Neumann de résoudre, pour les groupes compacts, le fameux « 5e problème » de Hilbert sur la caractérisation des groupes de Lie par des propriétés purement topologiques (à l’exclusion de toute structure différentielle préalablement donnée). Mais on s’aperçut aussitôt que, pour pouvoir utiliser la mesure invariante de façon efficace, il fallait non seulement connaître son existence, mais encore savoir qu’elle était unique à un facteur près ; ce point fut d’abord démontré par J. von Neumann pour les groupes compacts, en utilisant une méthode de définition de la mesure de Haar par des « moyennes » de fonctions continues, analogues à celles de Banach (VII a)); puis J. von Neumann (VII b)) et A. Weil (X),

(*) J. von Neumann montra, en 1929, que la raison profonde de la différence de comportement entre $\mathbf{R}$ et $\mathbf{R}^2$ d’une part, et les $\mathbf{R}^n$ pour $n \geqslant 3$ de l’autre, devait être cherchée dans la commutativité du groupe des rotations de l’espace $\mathbf{R}^n$.

par des méthodes différentes, obtinrent simultanément l’unicité dans le cas des groupes localement compacts, A. Weil indiquant en même temps comment le procédé de Haar pouvait s’étendre aux groupes localement compacts généraux. C’est aussi A. Weil (loc. cit.) qui obtint la condition d’existence d’une mesure relativement invariante sur un espace homogène, et montra enfin que l’existence d’une « mesure » (douée de propriétés raisonnables) sur un groupe topologique séparé, entraînait ipso facto que le groupe est localement précompact. Ces travaux achevaient essentiellement la théorie générale de la mesure de Haar ; la seule addition plus récente à citer est la notion de mesure quasi-invariante, qui ne s’est guère dégagée qu’aux environs de 1950, en liaison avec la théorie des représentations des groupes localement compacts dans les espaces hilbertiens.

L’histoire du produit de convolution est plus complexe. Dès le début du xixe siècle, on observe que si, par exemple, F(x, t) est une intégrale d’une équation aux dérivées partielles en x et t, linéaire et à coefficients constants, alors

$$
\int_{-\infty}^{+\infty} F(x - s, t)f(s)ds
$$

est aussi une intégrale de la même équation ; Poisson, entre autres, dès avant 1820, utilise cette idée pour écrire les intégrales de l’équation de la chaleur sous la forme

(1)
$$
\int_{-\infty}^{+\infty} \exp\left(-\frac{(x - s)^2}{4t}\right)f(s)ds.
$$

Un peu plus tard, l’expression

(2)
$$
\frac{1}{2\pi} \int_{-\pi}^{+\pi} \frac{\sin \frac{2n + 1}{2}(x - t)}{\sin \frac{x - t}{2}} f(t)dt
$$

de la somme partielle d’une série de Fourier et l’étude, faite par Dirichlet, de la limite de cette intégrale lorsque n tend vers +∞, donne le premier exemple de « régularisation » $f \to \rho_n * f$ sur le tore $\mathbf{T}$ (à vrai dire par une suite de « noyaux » $\rho_n$ non positifs, ce qui en complique singulièrement l’étude); sous le nom d’« intégrales singulières », les expressions intégrales analogues seront un sujet de prédilection des analystes de la fin du xixe siècle et du début du xx e siècle, de P. du Bois-Reymond à H. Lebesgue. Sur $\mathbf{R}$, Weierstrass utilise l’intégrale (1) pour la démonstration de son théorème d’approximation par les polynômes, et donne à ce propos le principe général de la régularisation par une suite de « noyaux » positifs $\rho_n$ de la forme $x \to c_n \rho(x/n)$. Sur $\mathbf{T}$, le plus célèbre exemple d’une régularisation par noyaux positifs est donné un peu plus tard par Fejér, et à partir de ce moment, c’est le procédé standard qui sera à la base de la plupart des « méthodes de sommation » des séries de fonctions.

Toutefois, ces travaux, en raison de la dissymétrie des rôles qu’y jouent le « noyau » et la fonction régularisée, ne faisaient guère apparaître les propriétés algébriques du produit de convolution. C’est à Volterra surtout que l’on doit d’avoir mis l’accent sur ce point. Il étudie de façon générale la « composition » $F * G$ de deux fonctions de deux variables

$$
(F * G)(x, y) = \int_x^y F(x, t)G(t, y)dt
$$

qu’il envisage comme une généralisation, par « passage du fini à l’infini », du produit de deux matrices (IX). Il distingue très tôt le cas (dit « du cycle fermé » en raison de son interprétation dans la théorie de l’hérédité) où F et G ne dépendent que de $y - x$; il en est alors de même de $H = F * G$, et si l’on pose $F(x, y) = f(y - x)$, $G(x, y) = g(y - x)$, on a

$$
H(x, y) = h(y - x),
$$

avec

$$
h(t) = \int_0^t f(t - s)g(s)ds
$$

de sorte que, pour $t \geqslant 0$, $h$ coïncide avec la convolution des fonctions $f_1, g_1$ égales respectivement à $f$ et $g$ pour $t \geqslant 0$, et à 0 pour $t < 0$.

Cependant, le formalisme algébrique développé par Volterra ne faisait pas apparaître les liens avec la structure de groupe de $\mathbf{R}$ et la transformation de Fourier. Nous n’avons pas à faire ici l’histoire de cette dernière ; mais il convient de noter qu’à partir de Cauchy les analystes qui traitent de l’intégrale de Fourier s’attachent surtout à trouver des conditions de plus en plus larges pour la validité des diverses formules d’« inversion », et négligent quelque peu ses propriétés algébriques. On ne pourrait certes en dire autant des travaux de Fourier lui-même (ou de ceux de Laplace sur l’intégrale analogue $\int_0^\infty e^{-st}f(t)dt$) ; mais ces transformations avaient été introduites essentiellement à propos de problèmes linéaires, et il n’est donc pas très surprenant que l’on n’ait pas songé avant longtemps à considérer le produit de deux transformées de Fourier (exception faite des produits de séries trigonométriques ou de séries entières, mais le lien avec la convolution des mesures discrètes ne pouvait évidemment pas être aperçu au xixe siècle). La première mention de ce produit et de la convolution sur $\mathbf{R}$ se trouve probablement dans un mémoire de Tchebychef (VIII), à propos de questions de calcul des probabilités. En effet, dans cette théorie, la convolution $\mu * \nu$ de deux « lois de probabilité » sur $\mathbf{R}$ (mesures positives de masse totale 1) n’est autre que la loi de probabilité « composée » de $\mu$ et $\nu$ (pour l’addition des « variables aléatoires » correspondantes). Bien entendu, chez Tchebychef, il n’est encore question que de convolution de lois de probabilités ayant une densité (par rapport à la mesure de Lebesgue), donc de convolution de fonctions ; elle n’intervient d’ailleurs chez lui que d’une façon épisodique, et il en sera ainsi dans les quelques rares travaux où elle apparaît avant la période 1920-1930. En 1920, P. J. Daniell, dans une note peu remarquée (III), définit la convolution de deux mesures quelconques sur $\mathbf{R}$ et la transformée de Fourier d’une telle mesure, et observe explicitement que la transformation de

Fourier fait passer de la convolution au produit ordinaire ; formalisme qui, à partir de 1925, va être intensivement utilisé par les probabilistes, à la suite de P. Lévy surtout. Mais l’importance fondamentale de la convolution en théorie des groupes n’est reconnue pleinement que par H. Weyl en 1927 ; il s’aperçoit que, pour un groupe compact, la convolution des fonctions joue le rôle de la multiplication dans l’algèbre d’un groupe fini, et lui permet par suite de définir la « représentation régulière » ; en même temps, il trouve dans la régularisation l’équivalent de l’élément unité de l’algèbre d’un groupe fini. Il restait à faire la synthèse de tous ces points de vue, qui s’accomplit dans le livre de A. Weil (X), préludant aux généralisations ultérieures que constitueront, d’une part les algèbres normées de I. Gelfand, et de l’autre la convolution des distributions.

La mesure de Haar et la convolution sont rapidement devenues des outils essentiels dans la tendance à l’algébrisation qui marque si fortement l’Analyse moderne ; nous aurons à en développer de nombreuses applications dans des Livres ultérieurs. La seule que nous ayons traitée dans ces chapitres concerne la « variation » des sous-groupes fermés (et notamment des sous-groupes discrets) d’un groupe localement compact. Cette théorie, partant d’un résultat de K. Mahler en Géométrie des nombres, a été inaugurée en 1950 par C. Chabauty, et vient d’être considérablement développée et approfondie par Macbeath et Swierczkowski (VI), dont nous avons reproduit les principaux résultats.

(I) S. Banach, Sur le problème de la mesure, Fund. Math., t. IV (1923), p. 7-33.
(II) E. Cartan, Le principe de dualité et certaines intégrales multiples de l’espace tangentiel et de l’espace réglé, Bull. Soc. Math. France, t. XXIV (1896), p. 140-177 (= Œuvres complètes, t. II₁, p. 265-302).
(III) P. J. Daniell, Stieltjes-Volterra products, Congr. Intern. des Math., Strasbourg, 1920, p. 130-136.
(IV) A. Haar, Der Maassbegriff in der Theorie der kontinuierlichen Gruppen, Ann. of Math., (2), t. XXXIV (1933), p. 147-169 (= Gesammelte Arbeiten, p. 600-622).
(V) A. Hurwitz, Ueber die Erzeugung der Invarianten durch Integration, Gött. Nachr., 1897, p. 71-90 (= Math. Werke, t. II, p. 546-564).
(VI) A. M. Macbeath, S. Swierczkowski, Limits of lattices in a compactly generated group, Can. Journ. of Math., t. XII (1960), p. 427-437.
(VII) J. von Neumann : a) Zum Haarschen Mass in topologischen Gruppen, Comp. Math., t. I (1934), p. 106-114 (= Collected Works, t. II, n° 22); b) The uniqueness of Haar’s measure, Mat. Sbornik, t. I (XLIII) (1936), p. 721-734 (= Collected Works, t. IV, n° 6).
(VIII) P. Tchebychef, Sur deux théorèmes relatifs aux probabilités, Acta Math., t. XIV (1890), p. 305-315 (= Œuvres, t. II, p. 481-491).
(IX) V. Volterra, Leçons sur les fonctions de lignes, Paris (Gauthier-Villars), 1913.
(X) A. Weil, L’intégration dans les groupes topologiques et ses applications, Actual Scient. et Ind., n° 869, Paris, Hermann, 1940 (2e éd., ibid., n° 869-1145, Paris, Hermann, 1953).
(XI) H. Weyl : a) Theorie des Darstellung kontinuierlicher halbeinfacher Gruppen durch lineare Transformationen, Math. Zeit., t. XXIII (1925), p. 271-309, XXIV (1926), p. 328-395 et 789-791 (= Selecta, Basel-Stuttgart (Birkhäuser), 1956, p. 262-366); b) (mit F. Peter) Die Vollständigkeit der primitiven Darstellungen einer geschlossenen kontinuierlichen Gruppe, Math. Ann., t. XCVII (1927), p. 737-755 (= Selecta, p. 387-404).

Les chiffres de référence indiquent successivement le chapitre, le paragraphe et le numéro.

γ_X(s), γ(s) : VII, 1, 1.
γ(s)f, γ(s)μ (f fonction, μ mesure) : VII, 1, 1.
dμ(s^{-1}x) : VII, 1, 1.
δ_X(s), δ(s), δ(s)f, δ(s)μ, dμ(xs) : VII, 1, 1.
f̃, ũ, dμ(x^{-1}) (f fonction, μ mesure) : VII, 1, 1.
Δ_G, Δ : VII, 1, 3.
mod_G φ, mod φ (φ automorphisme) : VII, 1, 4.
\mathbf{Z}_p (p nombre premier) : VII, 1, 6.
K^+ (K corps) : VII, 1, 10.
mod_K a, mod a (a élément d’un corps localement compact K) : VII, 1, 10.
α* (α mesure sur le groupe additif d’un corps localement compact K) : VII, 1, 10.
\mathcal{H}^\chi(X), \mathcal{H}_+^\chi(X), \mathcal{H}^1(X), f^\chi, f^1 (X espace localement compact où opère un groupe localement compact H, χ représentation continue de H dans \mathbf{R}_+) : VII, 2, 1.
f^b : VII, 2, 2.
λ#, \frac{\mu}{\beta}, \mu/\beta : VII, 2, 2.
m# (m mesure vectorielle) : VII, 2, 2.
T_J, T_1(n, K), T(n, K), T(n, K)* : VII, 3, 3.
\prod_{i=1}^n \* \mu_i, *_{\varphi(\mu_i)}_{1 \leq i \leq n}, \mu_1 \* \mu_2 \* \ldots \* \mu_n : VIII, 1, 1.
γ_χ : VIII, 2, 3 et VIII, 2, 4.
γ_{χ,p} : VIII, 2, 5.
U(μ) (U représentation d’un groupe localement compact G, μ mesure sur G) : VIII, 2, 6.
\mathcal{M}^p(G) (G groupe localement compact) : VIII, 3, 1.
μ *^β f, μ \* f (μ mesure, f fonction) : VIII, 4, 1.
\mathcal{L}(G) (G groupe localement compact) : VIII, 4, 5.

Les chiffres de référence indiquent successivement le chapitre, le paragraphe et le numéro (ou, exceptionnellement, l’exercice).

Algèbre trigonale supérieure, inférieure : VII, 3, 3.
Continue (représentation linéaire) : VIII, 2, 1.
Contragrédiente (représentation linéaire) : VIII, 2, 2.
Convolable, $\varphi$-convolable (suite finie de mesures) : VIII, 1, 1.
Convolables (mesure et fonction) : VIII, 4, 1.
Convolables (fonctions) : VIII, 4, 5.
Convolution (produit de) d’une suite finie de mesures : VIII, 1, 1.
Convolution (produit de) d’une mesure et d’une fonction : VIII, 4, 1.
Convolution (produit de) de fonctions : VIII, 4, 5.
Décomposition d’Iwasawa de $\mathbf{GL}(n, K)$ : VII, 3, 3.
Domaine fondamental : VII, 2, 10.
Entiers $p$-adiques : VII, 1, 6.
Equicontinue (représentation linéaire) : VIII, 2, 1.
Fondamental (domaine) : VII, 2, 10.
Groupe trigonal large supérieur, inférieur : VII, 3, 3.
Groupe trigonal spécial supérieur, inférieur : VII, 3, 3.
Groupe trigonal strict supérieur, inférieur : VII, 3, 3.
Groupe unimodulaire : VII, 1, 3.
Haar (mesure de) : VII, 1, 2.
Inégalité de Brunn-Minkowski : VII, 1, exerc. 25.
Invariante (mesure) par un groupe d’opérateurs : VII, 1, 1.
Invariante à gauche, à droite (mesure) sur un groupe : VII, 1, 1.
Isométrique (représentation linéaire) : VIII, 2, 1.
Iwasawa (décomposition d’) : VII, 3, 3.
Limite projective de mesures sur une limite projective de groupes localement compacts : VII, 1, 6.
Mesure de Haar à gauche, à droite sur un groupe localement compact : VII, 1, 2.
Mesure de Haar normalisée sur un groupe compact, sur un groupe discret : VII, 1, 3.
Mesure de Haar normalisée sur $\mathbf{Q}_p$ : VII, 1, 6.

Mesure invariante, relativement invariante, quasi-invariante par un groupe d’opérateurs : VII, 1, 1.
Mesure invariante à gauche, à droite sur un groupe localement compact : VII, 1, 1.
Mesure quasi-invariante sur un groupe localement compact : VII, 1, 9.
Mesure relativement invariante sur un groupe localement compact : VII, 1, 8.
Module d’un automorphisme : VII, 1, 4.
Module d’un groupe localement compact : VII, 1, 3.
Moyenne orbitale : VII, 2, 2.
Multiplicateur d’une mesure relativement invariante par un groupe d’opérateurs : VII, 1, 1.
Multiplicateur à gauche, à droite d’une mesure relativement invariante sur un groupe localement compact : VII, 1, 8.
Multiplicateur sur un produit G × X d’un groupe G et d’un ensemble X dans lequel G opère : VIII, 2, 3.
Normalisée (mesure de Haar) sur un groupe compact, sur un groupe discret : VII, 1, 3.
Normalisée (mesure de Haar) sur Q_p : VII, 1, 6.
Orbitale (moyenne) : VII, 2, 2.
p-adiques (entiers) : VII, 1, 6.
Produit de convolution de mesures pour une application : VIII, 1, 1.
Produit de convolution d’une mesure et d’une fonction : VIII, 4, 1.
Produit de convolution de fonctions : VIII, 4, 5.
Quasi-invariante (mesure) par un groupe d’opérateurs : VII, 1, 1.
Quasi-invariante (mesure) sur un groupe localement compact : VII, 1, 9.
Quotient d’une mesure sur un espace localement compact X par une mesure de Haar d’un groupe opérant dans X : VII, 2, 2.
Relativement invariante (mesure) par un groupe d’opérateurs : VII, 1, 1.
Relativement invariante (mesure) sur un groupe localement compact : VII, 1, 8.
Régulière (représentation) gauche, droite : VIII, 2, 5.
Représentation continue, séparément continue, équicontinue, isométrique : VIII, 2, 1.
Représentation linéaire transposée, contragrédiente d’une représentation linéaire : VIII, 2, 2.
Représentation régulière droite, gauche : VIII, 2, 5.
Représentation unitaire : VIII, 2, exerc. 4.
Séparément continue (représentation linéaire) : VIII, 2, 1.
Suite finie φ-convolable de mesures : VIII, 1, 1.
Théorème de Minkowski : VII, 1, exerc. 27.
Transposée (représentation linéaire) : VIII, 2, 2.
Trigonal large, trigonal strict, trigonal spécial (groupe) : VII, 3, 3.
Trigonale (algèbre) : VII, 3, 3.
Unimodulaire (groupe) : VII, 1, 3.

CHAPITRE VII. — Mesure de Haar ......................... 7

§ 1. Construction d'une mesure de Haar .................... 7
    1. Définitions et notations ............................. 7
    2. Le théorème d'existence et d'unicité ................. 13
    3. Module ............................................. 18
    4. Module d'un automorphisme ........................... 21
    5. Mesure de Haar d'un produit .......................... 22
    6. Mesure de Haar d'une limite projective ............... 23
    7. Définition locale d'une mesure de Haar .............. 28
    8. Mesures relativement invariantes ..................... 29
    9. Mesures quasi-invariantes ........................... 30
   10. Corps localement compacts ............................ 32
   11. Algèbres de dimension finie sur un corps localement compact .................................................. 37

§ 2. Quotient d'un espace par un groupe ; espaces homogènes .. 39
    1. Résultats généraux .................................. 39
    2. Cas où $\chi = 1$ .................................. 42
    3. Autre interprétation de $\lambda^*$ ................ 45
    4. Cas où $X/H$ est paracompact ..................... 50
    5. Mesures quasi-invariantes sur un espace homogène .... 53
    6. Mesures invariantes sur un espace homogène .......... 58
    7. Mesure de Haar sur un groupe quotient ............... 60
    8. Une propriété de transitivité ....................... 61
    9. Construction de la mesure de Haar d'un groupe à partir des mesures de Haar de certains sous-groupes .......... 65
   10. Intégration dans un domaine fondamental ............. 67

§ 3. Applications et exemples ............................. 70
    1. Groupes compacts d'applications linéaires ............ 70
    2. Trivialité d'espaces fibrés et d'extensions de groupes ... 72
    3. Exemples : 1. Groupe linéaire ....................... 79
        2. Groupe affine .................................. 80
        3. Groupe trigonal strict .......................... 81
        4. Groupe trigonal large .......................... 82

5. Groupe trigonal spécial ..................... 86
6. Groupe linéaire spécial ..................... 87
7. Décomposition d’Isawawa de GL(n,K) .. 90
8. Espaces de formes hermitiennes ............ 93
Appendice I ............................................. 96
Appendice II ............................................. 98
Exercices du § 1 ........................................ 100
Exercices du § 2 ........................................ 111
Exercices du § 3 ........................................ 115

CHAPITRE VIII. — Convolution et représentations .......... 120
§ 1. Convolution ........................................ 120
  1. Définitions et exemples .......................... 120
  2. Associativité ....................................... 122
  3. Cas des mesures bornées .......................... 125
  4. Propriétés concernant les supports .............. 126
  5. Expression vectorielle du produit de convolution .... 127
§ 2. Représentations linéaires des groupes ............. 128
  1. Représentations linéaires continues ............. 128
  2. Représentation contragrédiente .................. 131
  3. Exemple : représentations linéaires dans des espaces de fonctions continues .......................... 132
  4. Exemple : représentations linéaires dans des espaces de mesures ........................................ 134
  5. Exemple : représentations linéaires dans les espaces L^p . 134
  6. Prolongement d’une représentation linéaire de G aux mesures sur G ........................................ 136
  7. Relations entre les endomorphismes U(μ) et les endomorphismes U(s) ........................................ 137
§ 3. Convolution des mesures sur les groupes ............ 140
  1. Algèbres de mesures ............................... 140
  2. Cas d’un groupe opérant sur un espace ........... 144
  3. Convolution et représentations linéaires .......... 145
§ 4. Convolution des mesures et des fonctions ........... 148
  1. Convolution d’une mesure et d’une fonction ........ 148
  2. Exemples de mesures et de fonctions convolables... 152
  3. Convolution et transposition ..................... 159
  4. Convolution d’une mesure et d’une fonction sur un groupe. 163
  5. Convolution des fonctions sur un groupe .......... 164
  6. Applications ....................................... 169
  7. Régularisation ..................................... 171
§ 5. L’espace des sous-groupes fermés .................. 174
  1. L’espace des mesures de Haar des sous-groupes fermés de G ................................................. 174
  2. Semi-continuité du volume de l’espace homogène .... 177
  3. L’espace des sous-groupes fermés de G ............. 180
  4. Cas des groupes sans sous-groupes finis arbitrairement petits 183
  5. Cas des groupes commutatifs ........................ 185
  6. Autre interprétation de la topologie de l’espace des sous-groupes fermés ................................. 188

222                                      INTÉGRATION
Exercices du § 1 ........................................ 190
Exercices du § 2 ........................................ 190
Exercices du § 3 ........................................ 192
Exercices du § 4 ........................................ 196
Exercices du § 5 ........................................ 206
Note historique (chap. VII et VIII) ..................... 208
Index des notations ..................................... 217
Index terminologique ................................... 218
Principales formules du chapitre VII ................... Dépliant I
Conditions suffisantes pour l’existence du produit de convo-
    lution .............................................. Dépliant II

CONDITIONS SUFFISANTES POUR L’EXISTENCE
DU PRODUIT DE CONVOLUTION

I.  Cas où le produit de convolution μ \* ν de deux mesures existe :

(a) \* est défini par une application continue φ : X × Y → Z :
μ,ν bornées (alors μ \* ν est bornée et ‖μ \* ν‖ ≤ ‖μ‖.‖ν‖).
μ,ν à support compact (alors μ \* ν est à support compact et
Supp(μ \* ν) ⊂ φ(Supp μ × Supp ν)).

(b) \* est défini par un groupe opérant à gauche continûment dans
un espace : μ à support compact, ν quelconque.

(c) \* est défini par la multiplication dans un groupe G :
l’une des deux mesures à support compact.
μ, ν dans ℳ₀(G) (alors μ \* ν ∈ ℳ₀(G), et ‖μ \* ν‖₀ ≤ ‖μ‖₀‖ν‖₀).

II. — Cas où le produit de convolution μ \* f d’une mesure et d’une
fonction existe :

(a) \* est défini par un groupe G opérant à gauche continûment
dans un espace X muni d’une mesure β ≥ 0 telle que γ(s)β = χ(s⁻¹, .)β, χ
étant continue :
μ à support compact, f localement β-intégrable (si f est continue,
μ \* f est continue ; si f est continue à support compact, μ \* f est conti-
nue à support compact).

G opère proprement dans X, f ∈ 𝒦(X) (μ \* f est continue).

(b) les χ(s, .) sont bornées ; soit ρ(s) = sup χ(s⁻¹, x) :
x∈X
μ ∈ ℳ₀(G), f ∈ L∞(X, β) (alors μ \* f ∈ L∞(X, β) ; si f ∈ 𝒞⁰(X),
μ \* f ∈ 𝒞⁰(X) ; si f ∈ 𝒦(X), μ \* f ∈ 𝒦(X)).

μ ∈ ℳ₀$^{1/p}$(G), f ∈ $L^p$(X, β) où 1/p + 1/q = 1 (alors μ \* f ∈ $L^p$(X, β)
et ‖μ \* f‖ₚ ≤ ‖μ‖_{1/p}‖f‖ₚ).

III. — Cas où le produit de convolution f \* g de deux fonctions
localement β-intégrables existe (β mesure ≥ 0 relativement invariante
sur un groupe G, de multiplicateurs à gauche et à droite χ et χ’) :

f ou g continue, f ou g à support compact (alors f \* g est continue ;
si f, g dans 𝒦(G), f \* g ∈ 𝒦(G)).

fχ⁻¹/p ∈ L¹(G, β) et g ∈ $L^p$(G, β) (1/p + 1/q = 1) (alors f \* g ∈ $L^p$(G, β)
et ‖f \* g‖ₚ ≤ ‖fχ⁻¹/p‖₁‖g‖ₚ).

f ∈ $L^p$(G, β) et gχ’⁻¹ ∈ L¹(G, β) (alors f \* g ∈ $L^p$(G, β) et
‖f \* g‖ₚ ≤ ‖f‖ₚ‖gχ’⁻¹‖₁).

fχ⁻¹ ∈ L¹(G, β) et g ∈ 𝒞⁰(G) (resp. 𝒦(G)) (alors f \* g ∈ 𝒞⁰(G)
(resp. 𝒦(G))).

f ∈ 𝒞⁰(G) (resp. 𝒦(G)) et gχ’⁻¹ ∈ L¹(G, β) (alors f \* g ∈ 𝒞⁰(G)
(resp. 𝒦(G))).

f ∈ $L^p$(G, β), g ∈ $L^q$(G, β) avec 1/p + 1/q = 1, 1 < p < +∞, β
invariante à gauche (alors f \* g ∈ 𝒦(G) et ‖f \* g‖∞ ≤ ‖f‖ₚ‖g‖q).

Formules concernant les γ(s) et les δ(s).

Soit G un groupe topologique opérant continûment à gauche dans
un espace localement compact X par (s, x) → sx.

γ(sx) = sx                                      (s ∈ G, x ∈ X)
γ(st) = γ(s)γ(t)                                (s, t dans G)
(γ(s)f)(x) = f(s⁻¹x)                            (f fonction sur X)
⟨f, γ(s)μ⟩ = ⟨γ(s⁻¹)f, μ⟩                       (μ mesure sur X)
d(γ(s)μ)(x) = dμ(s⁻¹x)
(γ(s)μ)(A) = μ(s⁻¹A)                            (A ensemble γ(s)μ-intégrable).

Si μ est relativement invariante de multiplicateur χ,

γ(s)μ = χ(s)⁻¹μ
dμ(sx) = χ(s)dμ(x).

Soit G un groupe topologique opérant continûment à droite dans
un espace localement compact X par (s, x) → xs.

δ(s)x = xs⁻¹
δ(st) = δ(s)δ(t)
(δ(s)f)(x) = f(xs)
⟨f, δ(s)μ⟩ = ⟨δ(s⁻¹)f, μ⟩
d(δ(s)μ)(x) = dμ(xs)
(δ(s)μ)(A) = μ(As).

Si μ est relativement invariante de multiplicateur χ′,

δ(s)μ = χ′(s)μ.
dμ(xs) = χ′(s)dμ(x)

Formules concernant les mesures de Haar.

Soient G un groupe localement compact, Δ son module, μ une mesure de Haar à gauche, ν une mesure de Haar à droite.

1) On a

$$
\gamma(s)\mu = \mu \qquad \delta(s)\mu = \Delta(s)\mu \qquad \tilde{\mu} = \Delta^{-1}.\mu \\
d\mu(sx) = d\mu(x) \qquad d\mu(xs) = \Delta(s)d\mu(x) \qquad d\mu(x^{-1}) = \Delta(x)^{-1}d\mu(x)
$$

Si f est μ-intégrable,

$$
\int f(sx)d\mu(x) = \int f(x)d\mu(x) \qquad \int f(xs)d\mu(x) = \Delta(s)^{-1}\int f(x)d\mu(x) \\
\int f(x^{-1})\Delta(x)^{-1}d\mu(x) = \int f(x)d\mu(x).
$$

Si A ⊂ G est μ-intégrable,

$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A).
$$

2) On a

$$
\delta(s)\nu = \nu \qquad \gamma(s)\nu = \Delta(s)\nu \qquad \tilde{\nu} = \Delta.\nu. \\
d\nu(xs) = d\nu(x) \qquad d\nu(s^{-1}x) = \Delta(s)d\nu(x) \qquad d\nu(x^{-1}) = \Delta(x)d\nu(x).
$$

Si f est ν-intégrable,

$$
\int f(xs)d\nu(x) = \int f(x)d\nu(x) \qquad \int f(sx)d\nu(x) = \Delta(s)\int f(x)d\nu(x) \\
\int f(x^{-1})\Delta(x)d\nu(x) = \int f(x)d\nu(x).
$$

Si A ⊂ G est ν-intégrable,

$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s^{-1})\nu(A).
$$

3) ν est proportionnelle à Δ^{-1}.\mu, μ est proportionnelle à Δ.\nu.
