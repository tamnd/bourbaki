---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS. FORMULE SOMMATOIRE D’EULER–MACLAURIN
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0287-0291
extraction: ocr
statements: 0
exercises: 0
content_sha256: e7497f645f773fe7ffabe4b83371defb7f68109e39b33facc5e37fa558f53f06
---

# NOTE HISTORIQUE
(Chapitres V et VI)

(N.B. — Les chiffres romains entre parenthèses renvoient à la bibliographie placée à la fin de cette note.)

La distinction entre les « infiniment petits » (ou « infiniment grands ») de divers ordres, apparaît implicitement dès les premiers écrits sur le Calcul différentiel, et par exemple dans ceux de Fermat; elle devient pleinement consciente chez Newton et Leibniz, avec la théorie des « différences d’ordre supérieur »; et on ne tarde pas à observer que, dans les cas les plus simples, la limite (ou « vraie valeur ») d’une expression de la forme $f(x)/g(x)$, en un point où $f$ et $g$ tendent toutes deux vers 0, est donnée par le développement de Taylor de ces fonctions au voisinage du point considéré (« règle de l’Hôpital », due vraisemblablement à Johann Bernoulli).

En dehors de ce cas élémentaire, le principal problème d’« évaluation asymptotique » qui se pose aux mathématiciens dès la fin du xvii\textsuperscript{e} siècle est le calcul, exact ou approché, de sommes de la forme $\sum_{k=1}^{n} f(k)$, lorsque $n$ est très grand; un tel calcul est en effet nécessaire aussi bien pour l’interpolation et l’évaluation numérique de la somme d’une série, que dans le Calcul des probabilités, où les « fonctions de grands nombres » telles que $n!$ ou $\binom{a}{n}$ jouent un rôle prépondérant. Déjà Newton, pour obtenir des valeurs approchées de $\sum_{k=1}^{n} \frac{1}{a+k}$ lorsque $n$ est grand, indique une méthode qui revient (sur ce cas particulier) à calculer les premiers termes de la formule d’Euler-Maclaurin (I). Vers la fin du siècle, Jakob Bernoulli, au cours de recherches sur le Calcul des probabilités, se propose de déterminer les sommes $S_k(n) = \sum_{p=1}^{n-1} p^k$, polynômes en $n$ dont il découvre la loi générale de formation (sans en donner de démonstration)\footnote{Ce sont les primitives des « polynômes de Bernoulli » $B_k(x)$}, introduisant ainsi pour la première fois, dans l’expression des coefficients de ces polynômes, les nombres qui portent son nom, et la relation de récurrence qui permet de les calculer ((III), p. 97). En 1730, Stirling obtient un développement asymptotique pour $\sum_{k=1}^{n} \log (x + ka)$, $n$ croissant indéfiniment, avec un procédé de calcul des coefficients par récurrence.

De 1730 à 1745 se placent les travaux décisifs d’Euler sur les séries et les questions qui s’y rattachent. Posant $S(n) = \sum_{k=1}^{n} f(k)$, il applique à la fonction $S(n)$ la formule de Taylor, ce qui lui donne

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2S}{dn^2} + \frac{1}{3!} \frac{d^3S}{dn^3} - \ldots,
$$

équation qu’il « inverse » par la méthode des coefficients indéterminés, en cherchant une solution de la forme

$$
S(n) = \alpha \int f(n)\ dn + \beta f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2f}{dn^2} + \cdots;
$$

il obtient ainsi de proche en proche

$$
S(n) = \int f(n)\ dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3f}{dn^3} + \frac{1}{30\ 240} \frac{d^5f}{dn^5} - \ldots
$$

sans pouvoir tout d’abord déterminer la loi de formation des coefficients (III $a$ et $d$). Mais vers 1735, par analogie avec la décomposition d’un polynôme en facteurs du premier degré, il n’hésite pas à écrire la formule

$$
1 - \frac{\sin s}{\sin \alpha} = \left(1 - \frac{s}{\alpha}\right) \left(1 - \frac{s}{\pi - \alpha}\right) \left(1 - \frac{s}{-\pi - \alpha}\right) \left(1 - \frac{s}{2\pi - \alpha}\right)
$$
$$
\left(1 - \frac{s}{-2\pi + \alpha}\right) \cdots
$$

et en égalant les coefficients des développements des deux membres en série entière il obtient en particulier (pour $\alpha = \pi/2$) les célèbres expressions des séries $\sum_{n=1}^{\infty} \frac{1}{n^{2k}}$ à l’aide des puissances de $\pi$ (III $b$)$^1$. Quelques années plus tard, il s’aperçoit enfin que les coefficients de ces puissances de $\pi$ sont donnés par les mêmes équations que ceux de sa formule sommatoire, et reconnaît leur lien avec les nombres introduits par Bernoulli, et avec les coefficients du développement en série de $z/(e^z - 1)$ (III $g$).

Indépendamment d’Euler, Maclaurin était arrivé vers la même époque à la même formule sommatoire, par une voie un peu moins hasardeuse, voisine de celle que nous avons suivie dans le texte ; il itère en effet la formule « taylorienne » qui exprime $f(x)$ à l’aide des différences $f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$, formule qu’il obtient en « inversant » les développements de Taylor de ces différences par la méthode des coefficients indéterminés (IV) ; il n’aperçoit d’ailleurs pas la loi de formation des coefficients, découverte par Euler.

$^1$ En 1743, Euler, pour répondre à diverses critiques de ses contemporains, donne une dérivation un peu plus plausible des « développements eulériens » des fonctions trigonométriques ; par exemple, le développement en produit infini de sin $x$ est tiré de l’expression $\sin x = \frac{1}{2i} (e^{-ix} - e^{ix})$, et du fait que $e^{ix}$ est limite du polynôme $\left(1 + \frac{ix}{n}\right)^n$ (III $e$).

Mais Maclaurin, comme Euler et tous les mathématiciens de son temps, présente toutes ses formules comme des développements en série, dont la convergence n’est même pas étudiée. Ce n’est pas que la notion de série convergente fût totalement négligée à cette époque : on savait depuis Jakob Bernoulli que la série harmonique est divergente, et Euler avait lui-même précisé ce résultat en évaluant la somme des $n$ premiers termes de cette série à l’aide de sa formule sommatoire (III c et d) ; c’est aussi Euler qui remarque que le rapport de deux nombres de Bernoulli consécutifs croît indéfiniment, et par suite qu’une série entière ayant ces nombres pour coefficients ne peut converger ((III f), p. 357)¹. Mais la tendance au calcul formel est la plus forte, et l’extraordinaire intuition d’Euler lui-même ne l’empêche pas de tomber parfois dans l’absurde, lorsqu’il écrit par exemple $0 = \sum_{n=-\infty}^{+\infty} x^n$ ((III f), p. 362)².

Nous avons dit ailleurs (Note hist. du chap. IV) comment les mathématiciens du début du xixe siècle, lassés de ce formalisme sans frein et sans fondement, ramenèrent l’Analyse dans les voies de la rigueur. Une fois la notion de série convergente précisée, apparut la nécessité de critères simples permettant de démontrer la convergence des intégrales et des séries par comparaison avec des intégrales ou séries connues ; Cauchy donne un certain nombre de ces critères dans son Analyse algébrique (V a), tandis qu’Abel, dans un mémoire posthume (VI), obtient les critères logarithmiques de convergence. Cauchy, d’autre part (V b), élucide le paradoxe des séries telles que la série de Stirling, obtenues par application de la formule d’Euler-Maclaurin (et souvent appelées « séries semi-convergentes ») ; il montre que si (en raison de la remarque d’Euler sur les nombres de Bernoulli) le terme général $u_k(n)$ d’une telle série, pour une valeur fixe de $n$, croît indéfiniment avec $k$, il n’en reste pas moins que, pour une valeur fixe de $k$, la somme partielle $s_k(n) = \sum_{h=1}^k u_h(n)$ donne un développement asymptotique (pour $n$ tendant vers $+\infty$) de la fonction « représentée » par la série, d’autant plus précis que $k$ est plus grand.

Dans la plupart des calculs de l’Analyse classique, il est possible d’obtenir une loi générale de formation des développements asymptotiques d’une fonction, ayant un nombre de termes arbitrairement grand ; ce fait a contribué à créer une confusion durable (tout au moins dans le langage) entre séries et développements asymptotiques ; si bien que H. Poincaré, lorsqu’il prend la peine, en 1886 (VIII), de codifier les règles élémentaires des développements asymptotiques (suivant les puissances entières de $1/x$ au voisinage de $+\infty$), emploie encore le vocabulaire de

¹ Comme la série que considère Euler en cet endroit est introduite en vue du calcul numérique, il n’en prend que la somme des termes qui vont en décroissant, et à partir de l’indice où les termes commencent à croître, il les remplace par un reste dont il n’indique pas l’origine (le reste de la formule d’Euler–Maclaurin sous sa forme générale n’apparaît pas avant Cauchy).
² Il est piquant que cette formule suive, à une page de distance, un passage où Euler met en garde contre l’usage inconsidéré des séries divergentes!

la théorie des séries. Ce n’est guère qu’avec l’apparition des développements asymptotiques provenant de la théorie analytique des nombres que s’est enfin opérée la distinction nette entre la notion de développement asymptotique et celle de série, en raison du fait que, dans la plupart des problèmes que traite cette théorie, on ne peut obtenir explicitement qu’un très petit nombre de termes (le plus souvent un seul) du développement cherché.

Ces problèmes ont aussi familiarisé les mathématiciens avec l’usage d’échelles de comparaison autres que celle des puissances de la variable (réelle ou entière). Cette extension remonte surtout aux travaux de P. du Bois-Reymond (VII) qui, le premier, aborda systématiquement les problèmes de comparaison des fonctions au voisinage d’un point, et, dans des travaux très originaux, reconnut le caractère « non archimédien » des échelles de comparaison, en même temps qu’il étudiait de façon générale l’intégration et la dérivation des relations de comparaison, et en tirait une foule de conséquences intéressantes (VII b). Ses démonstrations manquent toutefois de clarté et de rigueur, et c’est à G. H. Hardy (IX) que revient la présentation correcte des résultats de du Bois-Reymond: sa contribution principale a consisté à reconnaître et démontrer l’existence d’un ensemble de « fonctions élémentaires », les fonctions (H), où les opérations usuelles de l’Analyse (notamment la dérivation) sont applicables aux relations de comparaison¹.

¹ Il n’entrait pas dans notre propos de développer dans ces chapitres les méthodes qui permettent d’obtenir des développements asymptotiques de fonctions se classant dans certaines catégories particulières, comme par exemple certains types d’intégrales dépendant d’un paramètre, qui interviennent fréquemment en Analyse; sur ce point (et en particulier sur les importantes méthodes de Laplace et de Darboux) le lecteur pourra consulter le livre cité de Hardy (IX), qui contient une bibliographie très complète.

(I) I. Newton, in St. P. Rigaud, Correspondence of scientific men, Oxford, 1841, t. II, p. 309–310.
(II) Jakob Bernoulli, Ars conjectandi, Bâle, 1713.
(III) L. Euler, Opera omnia (1), t. XIV; Commentationes analyticae..., Leipzig-Berlin (Teubner), 1924: a) Methodus generalis summandi progressiones, p. 42–72 (=Comm. Acad. petrop., t. VI (1732–33)); b) De summis serierum reciprocarum, p. 73–86 (=Comm. Acad. petrop., t. VII (1734–35)); c) De progressionibus harmonicis observationes, p. 87–100 (ibid.); d) Inventio summae cujusque serici..., p. 108–123 (=Comm. Acad. petrop., t. VIII (1736)); e) De summis serierum reciprocarum... dissertatio altera..., p. 138–155 (=Misc. Berol., t. VII (1743)); f) Consideratio progressionis..., p. 350–363 (=Comm. Acad. petrop., t. XI (1739)); g) De seriebus quibusdam considerationes, p. 407–462 (=Comm. Acad. petrop., t. XII (1740)).
(IV) C. MacLaurin, A complete treatise of fluxions, Edinburgh, 1742.
(V) A. L. Cauchy: a) Cours d’Analyse de l’Ecole Royale Polytechnique, 1re partie, 1821 (=Œuvres, (2), t. III, Paris (Gauthier-Villars), 1897); b) Œuvres, (1), t. VIII, p. 18–25, Paris (Gauthier-Villars), 1893.
(VI) N. H. Abel, Œuvres, t. II, p. 197–205, éd. Sylow et Lie, Christiania, 1881.
(VII) P. du Bois-Reymond: a) Sur la grandeur relative des infinis des fonctions, Ann. di Mat. (2), t. IV (1871), p. 338–353; b) Ueber asymptotische Werthe, infinitäre Approximationen und infinitäre Auflösung von Gleichungen, Math. Ann., t. VIII (1875), p. 362–414.
(VIII) H. Poincaré, Sur les intégrales irrégulières des équations linéaires, Acta Math., t. VIII (1886), p. 295–344.
(IX) G. H. Hardy, Orders of infinity, Cambridge tracts, n° 12, 2e éd., Cambridge University Press, 1924.
