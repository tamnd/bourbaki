---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ÉLÉMENTS D'HISTOIRE DES MATHÉMATIQUES
section: 18
section_title: Développements asymptotiques
lang: fr
source: hist-fr
pdf_pages: 0248-0252
extraction: ocr
statements: 0
exercises: 0
content_sha256: 50ad2908fb92b5da799c80cd7fc6b4a1d018980b83fde99eb313ed6253d7087a
---

## 18. DÉVELOPPEMENTS ASYMPTOTIQUES

La distinction entre les « infiniment petits » (ou « infiniment grands ») de divers ordres, apparaît implicitement dès les premiers écrits sur le Calcul différentiel, et par exemple dans ceux de Fermat ; elle devient pleinement consciente chez Newton et Leibniz, avec la théorie des « différences d’ordre supérieur » ; et on ne tarde pas à observer que, dans les cas les plus simples, la limite (ou « vraie valeur ») d’une expression de la forme $f(x)/g(x)$, en un point où $f$ et $g$ tendent toutes deux vers 0, est donnée par le développement de Taylor de ces fonctions au voisinage du point considéré (« règle de l’Hôpital », due vraisemblablement à Johann Bernoulli).

En dehors de ce cas élémentaire, le principal problème d’« évaluation asymptotique » qui se pose aux mathématiciens dès la fin du xviiie siècle est le calcul, exact ou approché, de sommes de la forme

$$
\sum_{k=1}^{n} f(k),
$$

lorsque $n$ est très grand ; un tel calcul est en effet nécessaire aussi bien pour l’interpolation et l’évaluation numérique de la somme d’une série, que dans le Calcul des probabilités, où les « fonctions de grands nombres » telles que $n!$ ou $\binom{a}{n}$ jouent un rôle prépondérant.

Déjà Newton, pour obtenir des valeurs approchées de $\sum_{k=1}^{n} \frac{1}{a+k}$

lorsque $n$ est grand, indique une méthode qui revient (sur ce cas particulier) à calculer les premiers termes de la formule d’Euler-Maclaurin ([262], t. II, p. 309-310). Vers la fin du siècle, Jakob Bernoulli, au cours de recherches sur le Calcul des probabilités, se propose de déterminer les sommes $S_k(n) = \sum_{p=1}^{n} p^k$, polynômes en $n$

• Ce sont les primitives des « polynômes de Bernoulli » $B_k(x)$.

dont il découvre la loi générale de formation (sans en donner de démonstration), introduisant ainsi pour la première fois, dans l’expression des coefficients de ces polynômes, les nombres qui portent son nom, et la relation de récurrence qui permet de les calculer ([19 b], p. 97). En 1730, Stirling obtient un développement asymptotique pour $\sum_{k=1}^{n} \log(x + ka)$, $n$ croissant indéfiniment, avec un procédé de calcul des coefficients par récurrence.

De 1730 à 1745 se placent les travaux décisifs d’Euler sur les séries et les questions qui s’y rattachent. Posant $S(n) = \sum_{k=1}^{n} f(k)$, il applique à la fonction $S(n)$ la formule de Taylor, ce qui lui donne

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2S}{dn^2} + \frac{1}{3!} \frac{d^3S}{dn^3} - \ldots,
$$

équation qu’il « inverse » par la méthode des coefficients indéterminés, en cherchant une solution de la forme

$$
S(n) = \alpha \int f(n) dn + \beta f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2f}{dn^2} + \ldots;
$$

il obtient ainsi de proche en proche

$$
S(n) = \int f(n) dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3f}{dn^3} + \frac{1}{30.240} \frac{d^5f}{dn^5} - \ldots
$$

sans pouvoir tout d’abord déterminer la loi de formation des coefficients ([108 a], (1), t. XIV, p. 42-72 et 108-123). Mais vers 1735, par analogie avec la décomposition d’un polynôme en facteurs du premier degré, il n’hésite pas à écrire la formule

$$
1 - \frac{\sin s}{\sin \alpha} = \left(1 - \frac{s}{\alpha}\right)\left(1 - \frac{s}{\pi - \alpha}\right)\left(1 - \frac{s}{-\pi - \alpha}\right)\left(1 - \frac{s}{2\pi + \alpha}\right)\left(1 - \frac{s}{-2\pi + \alpha}\right)...
$$

et en égalant les coefficients des développements des deux membres en série entière, il obtient en particulier (pour $\alpha = \frac{\pi}{2}$) les célèbres expressions des séries $\sum_{n=1}^{\infty} \frac{1}{n^{2k}}$ à l’aide des puissances de $\pi$ \* (loc. cit., p. 73-86). Quelques années plus tard, il s’aperçoit enfin que les coefficients de ces puissances de $\pi$ sont donnés par les mêmes équations que ceux de sa formule sommatoire, et reconnaît leur lien avec les nombres introduits par Bernoulli, et avec les coefficients du développement en série de $z/(e^z - 1)$ (loc. cit., p. 407-462).

Indépendamment d’Euler, Maclaurin était arrivé vers la même époque à la même formule sommatoire, par une voie un peu moins hasardeuse, voisine ce celle suivie aujourd’hui : il itère en effet la formule « taylorienne » qui exprime $f(x)$ à l’aide des différences $f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$, formule qu’il obtient en « inversant » les développements de Taylor de ces différences par la méthode des coefficients indéterminés ([214], t. II, p. 672-675); il n’aperçoit d’ailleurs pas la loi de formation des coefficients, découverte par Euler.

Mais Maclaurin, comme Euler et tous les mathématiciens de son temps, présente toutes ses formules comme des développements en série, dont la convergence n’est même pas étudiée. Ce n’est pas que la notion de série convergente fût totalement négligée à cette époque : on savait depuis Jakob Bernoulli que la série harmonique est divergente, et Euler avait lui-même précisé ce résultat en évaluant la somme des $n$ premiers termes de cette série à l’aide de sa formule sommatoire ([108 a], (1), t. XIV, p. 87-100 et 108-123); c’est aussi Euler qui remarque que le rapport de deux nombres de Bernoulli consécutifs croît indéfiniment, et par suite qu’une série entière ayant ces nombres pour coefficients ne peut converger (loc. cit., p. 357) **. Mais la tendance au calcul formel est la plus forte, et l’extraordinaire intuition d’Euler lui-même ne l’empêche pas de tomber parfois dans

• En 1743, Euler, pour répondre à diverses critiques de ses contemporains, donne une dérivation un peu plus plausible des « développements eulériens » des fonctions trigonométriques ; par exemple, le développement en produit infini de $\sin x$ est tiré de l’expression $\sin x = \frac{1}{2i}(e^{ix} - e^{-ix})$, et du fait que $e^{ix}$ est limite du polynome $\left(1 + \frac{ix}{n}\right)^n$ (loc. cit., p. 138-155).

** Comme la série que considère Euler en cet endroit est introduite en vue du calcul numérique, il n’en prend que la somme des termes qui vont en décroissant, et à partir de l’indice où les termes commencent à croître, il les remplace par un reste dont il n’indique pas l’origine (le reste de la formule d’Euler-Maclaurin sous sa forme générale n’apparaît pas avant Cauchy).

l’absurde, lorsqu’il écrit par exemple $0 = \sum_{n=-\infty}^{+\infty} x^n$ (loc. cit., p. 362) *.

Nous avons dit ailleurs (voir p. 192) comment les mathématiciens du début du XIXe siècle, lassés de ce formalisme sans frein et sans fondement, ramenèrent l’Analyse dans les voies de la rigueur. Une fois la notion de série convergente précisée, apparut la nécessité de critères simples permettant de démontrer la convergence des intégrales et des séries par comparaison avec des intégrales ou séries connues ; Cauchy donne un certain nombre de ces critères dans son Analyse algébrique ([56 a], (2), t. III), tandis qu’Abel, dans un mémoire posthume ([1], t. II, p. 197-205), obtient les critères logarithmiques de convergence. Cauchy, d’autre part ([56 a], (1), t. VIII, p. 18-25), élucide le paradoxe des séries telles que la série de Stirling, obtenues par application de la formule d’Euler-Maclaurin (et souvent appelées « séries semi-convergentes ») : il montre que si (en raison de la remarque d’Euler sur les nombres de Bernoulli) le terme général $u_k(n)$ d’une telle série, pour une valeur fixe de $n$, croît indéfiniment avec $k$, il n’en reste pas moins que, pour une valeur fixe de $k$, la somme partielle $s_k(n) = \sum_{h=1}^k u_h(n)$ donne un développement asymptotique (pour $n$ tendant vers $+\infty$) de la fonction « représentée » par la série, d’autant plus précis que $k$ est plus grand.

Dans la plupart des calculs de l’Analyse classique, il est possible d’obtenir une loi générale de formation des développements asymptotiques d’une fonction, ayant un nombre de termes arbitrairement grand ; ce fait a contribué à créer une confusion durable (tout au moins dans le langage) entre séries et développements asymptotiques ; si bien que H. Poincaré, lorsqu’il prend la peine, en 1886 ([251 a], t. I, p. 290-296), de codifier les règles élémentaires des développements asymptotiques (suivant les puissances entières de $1/x$ au voisinage de $+\infty$), emploie encore le vocabulaire de la théorie des séries. Ce n’est guère qu’avec l’apparition des développements asymptotiques provenant de la théorie analytique des nombres que s’est enfin opérée la distinction nette entre la notion de développement asymptotique et celle de série, en raison du fait que, dans la plupart des problèmes

\* Il est piquant que cette formule suive, à une page de distance, un passage où Euler met en garde contre l’usage inconsidéré des séries divergentes !

que traite cette théorie, on ne peut obtenir explicitement qu’un très petit nombre de termes (le plus souvent un seul) du développement cherché.

Ces problèmes ont aussi familiarisé les mathématiciens avec l’usage d’échelles de comparaison autres que celle des puissances de la variable (réelle ou entière). Cette extension remonte surtout aux travaux de P. du Bois-Reymond [94 a et b] qui, le premier, aborda systématiquement les problèmes de comparaison des fonctions au voisinage d’un point, et, dans des travaux très originaux, reconnut le caractère « non archimédien » des échelles de comparaison, en même temps qu’il étudiait de façon générale l’intégration et la dérivation des relations de comparaison, et en tirait une foule de conséquences intéressantes [94 b]. Ses démonstrations manquent toutefois de clarté et de rigueur, et c’est à G. H. Hardy [147] que revient la présentation correcte des résultats de du Bois-Reymond : sa contribution principale a consisté à reconnaître et démontrer l’existence d’un ensemble de « fonctions élémentaires », les fonctions (H), où les opérations usuelles de l’Analyse (notamment la dérivation) sont applicables aux relations de comparaison.
