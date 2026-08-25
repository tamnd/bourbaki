---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE)
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: evt-i-v-fr
pdf_pages: 0341-0372
extraction: ocr
statements: 0
exercises: 0
content_sha256: cc0c689a14aafd40b443957db241e72bf344008b71e0521568d6635432c88bbd
---

# NOTE HISTORIQUE
(chapitres I à V)

(N.B. — Les chiffres romains renvoient à la bibliographie placée à la fin de cette note.)

La théorie générale des espaces vectoriels topologiques a été fondée dans la période qui va de 1920 à 1930 environ. Mais elle avait été préparée de longue date par l’étude de nombreux problèmes d’Analyse fonctionnelle ; on ne peut retracer son histoire sans indiquer, au moins de façon sommaire, comment l’étude de ces problèmes amena peu à peu les mathématiciens (surtout à partir du début du xx\textsuperscript{e} siècle) à prendre conscience de la parenté entre les questions considérées, et de la possibilité de les formuler de façon beaucoup plus générale et de leur appliquer des procédés de solution uniformes.

On peut dire que les analogies entre Algèbre et Analyse, et l’idée de considérer des équations fonctionnelles (c’est-à-dire où l’inconnue est une fonction) comme des « cas limites » d’équations algébriques, remontent aux débuts du Calcul infinitésimal, qui en un certain sens répond à ce besoin de généralisation « du fini à l’infini ». Mais l’ancêtre algébrique direct du Calcul infinitésimal est le calcul des différences finies (\emph{cf.} FVR, Note historique des chap. I-II-III, p. 54-58), et non la résolution des systèmes linéaires généraux ; ce n’est pas avant le milieu du xviii\textsuperscript{e} siècle que se manifestent les premières analogies entre cette dernière et des problèmes de Calcul différentiel, à propos de l’équation des cordes vibrantes. Nous n’entrerons pas ici dans le détail de l’histoire de ce problème ; mais il nous faut relever l’apparition de deux idées fondamentales, qui se retrouveront constamment par la suite, et qui toutes deux paraissent dues à D. Bernoulli. La première consiste à considérer l’oscillation de la corde comme « cas limite » de l’oscillation d’un système de $n$ masses ponctuelles, lorsque $n$ augmente indéfiniment ; on sait que, pour $n$ fini, ce problème devait un peu plus tard donner le premier exemple de recherche de valeurs propres d’une transformation linéaire (\emph{cf.} A, Note historique des chap. VI-VII) ; à ces nombres correspondent, dans le « passage à la limite » envisagé, les fréquences des « oscillations propres » de la corde, observées expérimentalement de longue date, et dont l’existence théorique avait été établie (notamment par Taylor) au début du siècle. Cette analogie formelle, bien qu’assez rarement mentionnée par la suite ((I, b), p. 390), ne paraît jamais avoir été perdue de vue au cours du xix\textsuperscript{e} siècle ; mais, comme nous le verrons plus loin, elle n’acquerra toute son importance que vers 1890-1900.

L’autre idée de D. Bernoulli (peut-être inspirée par les faits expérimentaux) est le « principe de superposition », d’après lequel l’oscillation la plus générale de la corde doit pouvoir se « décomposer » en superposition d’« oscillations propres », ce qui, mathématiquement parlant, signifie que la solution générale de l’équation aux cordes vibrantes doit pouvoir se développer en série $\sum_n c_n \varphi_n(x, t)$, où les $\varphi_n(x, t)$ représentent les oscillations propres. On sait que ce principe devait déclencher une longue querelle sur la possibilité de développer une fonction « arbitraire » en série trigonométrique, querelle qui ne fut tranchée que par les travaux de Fourier et de Dirichlet dans le premier tiers du xixe siècle. Mais avant même que ce résultat ne fût atteint, on avait rencontré d’autres exemples de développements en séries de fonctions « orthogonales » \* : fonctions sphériques et polynômes de Legendre, ainsi que divers systèmes de la forme $(e^{i\lambda_n x})$, où les $\lambda_n$ ne sont plus multiples d’un même nombre, et qui avaient été introduits dès le xviiie siècle dans des problèmes d’oscillation, ainsi que par Fourier et Poisson au cours de leurs recherches sur la théorie de la chaleur. Vers 1830, tous les phénomènes observés dans ces divers cas particuliers sont systématisés par Sturm (I) et Liouville (II) en une théorie générale des oscillations, pour les fonctions d’une variable : ils considèrent l’équation différentielle

(1)
$$
\frac{d}{dx} \left( p(x) \frac{dy}{dx} \right) + \lambda \rho(x) y = 0 \quad (p(x) > 0, \rho(x) > 0)
$$
avec les conditions aux limites
(2)
$$
\begin{align*}
k_1 y'(a) - h_1 y(a) &= 0 \\
k_2 y'(b) + h_2 y(b) &= 0
\end{align*}
$$
$(h_1 k_1 \neq 0, h_2 k_2 \neq 0, a < b)$

et démontrent les résultats fondamentaux suivants :
1) le problème n’a de solution $\neq 0$ que lorsque $\lambda$ prend l’une des valeurs d’une suite $(\lambda_n)$ de nombres $> 0$, tendant vers $+ \infty$;
2) pour chaque $\lambda_n$, les solutions sont multiples d’une même fonction $v_n$, qu’on peut supposer « normée » par la condition $\int_a^b \rho v_n^2 dx = 1$, et on a $\int_a^b \rho v_m v_n dx = 0$ pour $m \neq n$;
3) toute fonction $f$, deux fois différentiable dans $[a, b]$, et satisfaisant aux conditions aux limites (2), est développable en série uniformément convergente
$$
f(x) = \sum_n c_n v_n(x), \text{ où } c_n = \int_a^b \rho f v_n dx;
$$
4) on a l’égalité $\int_a^b \rho f^2 dx = \sum_n c_n^2$ (déjà démontrée par Parseval en 1799 — de façon purement formelle, d’ailleurs — pour le système des fonctions trigonométriques, et d’où découle aussitôt l’« inégalité de Bessel » énoncée par ce dernier (toujours pour les séries trigonométriques) en 1828).

\* Ce terme n’apparaît toutefois pas avant les travaux de Hilbert.

Un demi-siècle plus tard, ces propriétés sont complétées par les travaux de Gram (III) qui, poursuivant des recherches de Tchebichef, met en lumière la relation entre les développements en séries de fonctions orthogonales et le problème de la « meilleure approximation quadratique » (issu directement de la « méthode des moindres carrés » de Gauss, dans la théorie des erreurs) : ce dernier consiste, étant donnée une suite finie de fonctions $(\psi_i)_{1 \leq i \leq n}$, à trouver, pour une fonction $f$, la combinaison linéaire $\sum_i a_i \psi_i$ pour laquelle l’intégrale $\int_a^b \rho(f - \sum_i a_i \psi_i)^2 dx$ atteint son minimum. Il ne s’agit là en principe que d’un problème d’algèbre linéaire banal, mais Gram le résout d’une façon originale, en appliquant aux $\psi_i$ le processus d’« orthonormalisation » décrit au chap. V, p. 23 (et généralement connu sous le nom d’Erhard Schmidt). Passant ensuite au cas d’un système orthonormal infini $(\varphi_n)$, il se pose la question de savoir quand la « meilleure approximation quadratique » $\mu_n$ d’une fonction $f$ par les combinaisons linéaires des $n$ premières fonctions de la suite, tend vers 0 lorsque $n$ augmente indéfiniment \* ; il est ainsi amené à définir la notion de système orthonormal complet, et reconnaît que cette propriété équivaut à la non-existence de fonctions $\neq 0$ orthogonales à toutes les $\varphi_n$. Il cherche même à élucider le concept de « convergence en moyenne quadratique », mais, avant l’introduction des notions fondamentales de la théorie de la mesure, il ne pouvait guère obtenir dans cette direction que des résultats très particuliers.

Dans la seconde moitié du xixe siècle, l’effort principal des analystes se porte plutôt vers l’extension de la théorie de Sturm-Liouville aux fonctions de plusieurs variables, à quoi conduisait notamment l’étude des équations aux dérivées partielles de type elliptique de la Physique mathématique, et des problèmes aux limites qui leur sont naturellement associés. L’intérêt se concentre principalement sur l’équation des « membranes vibrantes »

(3)
$$
L_\lambda(u) \equiv \Delta u + \lambda u = 0
$$
où l’on cherche dans un domaine $G$ assez régulier les solutions qui s’annulent au contour ; ce n’est que peu à peu que furent surmontées les difficultés analytiques considérables présentées par ce problème, auquel on ne pouvait songer à appliquer les méthodes qui avaient réussi pour les fonctions d’une seule variable. Rappelons les principales étapes vers la solution : l’introduction de la « fonction de Green » de $G$, dont l’existence est démontrée par Schwarz ; la démonstration, due aussi à Schwarz, de l’existence de la plus petite valeur propre ; enfin, en 1894, dans un mémoire célèbre (V a), H. Poincaré parvient à démontrer l’existence et les propriétés essentielles de toutes les valeurs propres, en considérant, pour un « second membre » $f$ donné, la solution $u_\lambda$ de l’équation $L_\lambda(u) = f$ qui s’annule au contour, et en prouvant, par une habile généralisation de la méthode de Schwarz, que $u_\lambda$

\* Il est à noter que, dans toute cette étude, Gram ne se limite pas à la considération des fonctions continues, mais insiste sur l’importance de la condition $\int_a^b \rho f^2 dx < + \infty$.

est fonction méromorphe de la variable complexe $\lambda$, n’ayant que des pôles simples réels $\lambda_n$, qui sont justement les valeurs propres cherchées.

Ces recherches se relient étroitement aux débuts de la théorie des équations intégrales linéaires, qui devait sans doute contribuer le plus à l’avènement des idées modernes. Nous nous bornerons ici à donner quelques brèves indications sur le développement de cette théorie (renvoyant, pour de plus amples détails, aux Notes historiques qui suivront les chapitres de ce Traité consacrés à la théorie spectrale). Ce type d’équations fonctionnelles, apparu d’abord sporadiquement dans la première moitié du xixe siècle (Abel, Liouville), avait acquis de l’importance depuis que Beer et C. Neumann avaient ramené la solution du « problème de Dirichlet » pour un domaine assez régulier G, à la résolution d’une « équation intégrale de deuxième espèce »

$$
u(x) + \int_a^b K(x, y) u(y) \, dy = f(x)
$$

pour la fonction inconnue $u$; équation que C. Neumann était parvenu à résoudre au moyen d’un procédé d’« approximations successives » en 1877. Mû sans doute autant par les analogies algébriques déjà mentionnées que par les résultats qu’il venait d’obtenir sur l’équation des membranes vibrantes, H. Poincaré, en 1896 (V b), a l’idée d’introduire un paramètre variable $\lambda$ devant l’intégrale dans l’équation précédente, et affirme que, comme pour l’équation des membranes vibrantes, la solution est alors fonction méromorphe de $\lambda$; mais il ne parvint pas à démontrer ce résultat, qui ne fut établi (pour un « noyau » K continu et un intervalle $[a, b]$ fini) que par I. Fredholm sept ans plus tard (VI). Ce dernier, plus consciemment peut-être encore que ses prédécesseurs, se laisse complètement guider par l’analogie de (4) avec le système linéaire

$$
\sum_{q=1}^n (\delta_{pq} + \frac{1}{n} a_{pq}) x_q = b_p \quad (1 \leq p \leq n)
$$

pour obtenir la solution de (4) comme quotient de deux expressions, formées sur le modèle des déterminants qui interviennent dans les formules de Cramer. Ce n’était d’ailleurs pas là une idée nouvelle : dès le début du xixe siècle, la méthode des « coefficients indéterminés » (consistant à obtenir une fonction inconnue supposée développable en série $\sum c_n \varphi_n$, où les $\varphi_n$ sont des fonctions connues, en calculant les coefficients $c_n$), avait conduit à des « systèmes linéaires à une infinité d’inconnues »

$$
\sum_{j=1}^\infty a_{ij} x_j = b_i \quad (i = 1, 2, \ldots)
$$

Fourier, qui rencontre un tel système, le « résout » encore comme un mathématicien du xviiiie siècle : il supprime tous les termes ayant un indice $i$ ou $j$ supérieur à $n$, résout explicitement le système fini obtenu, par les formules de Cramer, puis « passe à la limite » en faisant tendre $n$ vers $+ \infty$ dans la solution ! Lorsque plus tard on ne se contenta plus de pareils tours de passe-passe, c’est encore par la théorie des déterminants qu’on chercha d’abord à attaquer le problème ; à partir de 1886 (à la suite de travaux de Hill), H. Poincaré, puis H. von Koch, avaient édifié une théorie des « déterminants infinis » qui permet de résoudre certains types de systèmes (6) suivant le modèle classique ; et si ces résultats n’étaient pas directement applicables au problème visé par Fredholm, du moins est-il certain que la théorie de von Koch, en particulier, lui servit de modèle pour la formation de ses « déterminants ».

C’est à ce moment que Hilbert entre en scène et donne une impulsion nouvelle à la théorie (VII). Il commence par compléter les travaux de Fredholm en réalisant effectivement le passage à la limite qui conduit de la solution de (5) à celle de (4) ; mais il y ajoute aussitôt le passage à la limite correspondant pour la théorie des formes quadratiques réelles, à quoi conduisaient naturellement les types d’équations intégrales à noyau symétrique (c’est-à-dire telles que $K(y, x) = K(x, y)$), de beaucoup les plus fréquentes en Physique mathématique. Il parvient ainsi à la formule fondamentale qui généralise directement la réduction d’une forme quadratique à ses axes

$$
\int_a^b \int_a^b K(s, t) \ x(s) \ x(t) \ dsdt = \sum_{n=1}^\infty \frac{1}{\lambda_n} \left( \int_a^b \varphi_n(s) \ x(s) \ ds \right)^2,
$$

les $\lambda_n$ étant les valeurs propres (nécessairement réelles) du noyau $K$, les $\varphi_n$ formant le système orthonormal des fonctions propres correspondantes, et le second membre de la formule (7) étant une série convergente pour $\int_a^b x^2(s) \ ds \leq 1$. Il montre aussi comment toute fonction « représentable » sous la forme $f(x) = \int_a^b K(x, y) \ g(y) \ dy$ admet le « développement » $\sum_{n=1}^\infty \varphi_n(x) \int_a^b \varphi_n(y) \ f(y) \ dy$, et, poursuivant l’analogie avec la théorie classique des formes quadratiques, il indique un procédé de détermination des $\lambda_n$ par une méthode variationnelle, qui n’est autre que l’extension des propriétés extrémales bien connues des axes d’une quadrique ((VII), p. 1-38).

Ces premiers résultats de Hilbert furent presque aussitôt repris par E. Schmidt, sous une forme plus simple et plus générale, évitant l’introduction des « déterminants de Fredholm » ainsi que le passage du fini à l’infini, et déjà très proche d’un exposé abstrait, les propriétés fondamentales de linéarité et de positivité de l’intégrale étant visiblement seules utilisées dans les démonstrations (VIII a). Mais déjà Hilbert était parvenu à des conceptions bien plus générales encore. Tous les travaux précédents faisaient ressortir l’importance des fonctions de carré intégrable, et la formule de Parseval établissait un lien étroit entre ces fonctions et les suites $(c_n)$ telles que $\sum_n c_n^2 < + \infty$. C’est sans doute cette idée qui guide Hilbert dans ses mémoires de 1906 ((VII), chap. XI-XIII) où, reprenant la vieille méthode des « coefficients indéterminés », il montre que la résolution de l’équation intégrale (4) est équivalente au système d’une infinité d’équations linéaires

(8)
$$
x_p' + \sum_{q=1}^{\infty} k_{pq} x_q = b_p \quad (p = 1, 2, ...)
$$
pour les « coefficients de Fourier » $x_p = \int_a^b u(t) \omega_p(t) \, dt$ de la fonction inconnue $u$
par rapport à un système orthonormal complet donné ($\omega_n$) (avec $b_p = \int_a^b f(t) \omega_p(t) \, dt$)
et $k_{pq} = \int_a^b \int_a^b K(s, t) \omega_p(s) \omega_q(t) \, dsdt$. En outre, les seules solutions de (8) à considérer de ce point de vue sont celles pour lesquelles $\sum_n x_n^2 < + \infty$; aussi est-ce à ce type de solution que se limite systématiquement Hilbert ; mais il élargit par contre les conditions imposées à la « matrice infinie » ($k_{pq}$) (qui, dans (8), est telle que $\sum_{p,q} k_{pq}^2 < + \infty$). Dès ce moment, il est clair que l’« espace de Hilbert » des suites $x = (x_n)$ de nombres réels telles que $\sum_n x_n^2 < + \infty$, bien que non explicitement introduit, est sous-jacent à toute la théorie, et apparaît comme un « passage à la limite » à partir de l’espace euclidien de dimension finie. De plus, ce qui est particulièrement important pour les développements ultérieurs, Hilbert est amené à introduire dans cet espace, non pas seulement une, mais deux notions distinctes de convergence (correspondant à ce que l’on a appelé depuis la topologie faible et la topologie forte *), ainsi qu’un « principe de choix » qui n’est autre que la propriété de compacité faible de la boule unité. La nouvelle algèbre linéaire qu’il développe à propos de la résolution des systèmes (8) repose tout entière sur ces notions topologiques : applications linéaires, formes linéaires et formes bilinéaires (associées aux applications linéaires) sont classées et étudiées suivant leurs propriétés de « continuité » **. En particulier, Hilbert découvre que le succès de la méthode de Fredholm repose sur la notion de « complète continuité » qu’il dégage en la formulant pour les formes bilinéaires *** et étudie de façon approfondie ; pour plus de détails, nous renvoyons à la partie de ce Traité où seront développés cette importante notion, et les admirables et profonds travaux où Hilbert inaugure la théorie spectrale des formes bilinéaires symétriques (bornées ou non).

Le langage de Hilbert reste encore classique, et, tout au long des « Grundzüge »,

\* Le Calcul des variations avait déjà conduit de façon naturelle à envisager des notions de convergence différentes sur un même ensemble de fonctions (suivant que l’on exigeait seulement la convergence uniforme des fonctions, ou la convergence uniforme des fonctions et d’un certain nombre de leurs dérivées) ; mais les modes de convergence définis par Hilbert étaient d’un type tout à fait nouveau à cette époque.
** Il faut noter que, jusque vers 1935, par fonction « continue » on entend pratiquement toujours une application transformant toute suite convergente en une suite convergente.
*** Pour Hilbert, une forme bilinéaire B(x, y) est complètement continue si, lorsque les suites $(x_n), (y_n)$ tendent faiblement vers x et y respectivement, B($x_n, y_n$) tend vers B(x, y).

il ne cesse d’avoir en vue les applications de la théorie, dont il développe de nombreux exemples (occupant à peu près la moitié du volume). La génération suivante va déjà adopter un point de vue beaucoup plus abstrait. Sous l’influence des idées de Fréchet et de F. Riesz sur la topologie générale (voir Note historique de TG, chap. I), E. Schmidt (VIII b) et Fréchet lui-même introduisent délibérément, en 1907-1908, le langage de la géométrie euclidienne dans l’« espace de Hilbert » (réel ou complexe) ; c’est dans ces travaux qu’on trouve la première mention de la norme (avec la notation actuelle $\|x\|$), l’inégalité du triangle qu’elle vérifie, le fait que l’espace de Hilbert est « séparable » et complet ; en outre, E. Schmidt démontre l’existence de la projection orthogonale sur une variété linéaire fermée, ce qui lui permet de donner une forme plus simple et plus générale à la théorie des systèmes linéaires de Hilbert. En 1907 aussi, Fréchet et F. Riesz remarquent que l’espace des fonctions de carré sommable a une « géométrie » tout à fait analogue ; analogie qui s’explique parfaitement lorsque, quelques mois plus tard, F. Riesz et E. Fischer démontrent que cet espace est complet et isomorphe à l’« espace de Hilbert », mettant en même temps en évidence de façon éclatante la valeur de l’outil nouvellement créé par Lebesgue. Dès ce moment les points essentiels de la théorie élémentaire des espaces hilbertiens peuvent être considérés comme acquis ; parmi les progrès plus récents, il faut notamment mentionner la présentation axiomatique de la théorie donnée vers 1930 par M. H. Stone et J. von Neumann, ainsi que l’abandon des restrictions de « séparabilité », qui s’effectue aux environs de 1934, dans les travaux de Rellich, Löwig, et F. Riesz (IX e).

Cependant d’autres courants d’idées venaient, dans les premières années du xx\textsuperscript{e} siècle, renforcer la tendance qui menait à la théorie des espaces normés. L’idée générale de « fonctionnelle » (c’est-à-dire une fonction à valeurs numériques définie dans un ensemble dont les éléments sont eux-mêmes des fonctions numériques d’une ou de plusieurs variables réelles) s’était dégagée dans les dernières décennies du xix\textsuperscript{e} siècle, en liaison avec le calcul des variations, d’une part, la théorie des équations intégrales de l’autre. Mais si c’est principalement à l’école italienne, autour de Pincherle et surtout de Volterra, que l’on doit d’avoir mis en lumière cette notion, ainsi que l’idée plus générale d’« opérateur », les travaux de cette école restaient souvent de nature passablement formelle et attachés à des problèmes de type particulier, faute d’une analyse assez poussée des concepts topologiques sous-jacents. En 1903, Hadamard inaugure la théorie moderne de la dualité « topologique », en cherchant les « fonctionnelles » linéaires continues les plus générales sur l’espace $\mathcal{C}(I)$ des fonctions continues numériques dans un intervalle compact I (espace muni de la topologie de la convergence uniforme), et en les caractérisant comme limites de suites d’intégrales $x \mapsto \int_I k_n(t)\ x(t)\ dt$. En 1907, Fréchet et F. Riesz montrent de même que, sur l’espace de Hilbert, les formes linéaires continues sont les formes « bornées » introduites par Hilbert ; puis, en 1909, F. Riesz met sous une forme définitive le th. de Hadamard, en exprimant toute fonctionnelle linéaire continue sur $\mathcal{C}(I)$ par une intégrale de Stieltjes, théorème qui devait plus tard servir dé point de départ à la théorie moderne de l’Intégration (voir Note hist. d’INT, chap. II-V).

L’année suivante, c’est encore F. Riesz (IX a) qui fait faire de nouveaux et importants progrès à la théorie par l’introduction et l’étude (calquée sur la théorie de l’espace de Hilbert) des espaces $L^p(I)$ des fonctions de puissance $p$-ième intégrable dans un intervalle I (pour un exposant $p$ tel que $1 < p < + \infty$), étude qu’il fait suivre trois ans plus tard (IX c) d’un travail analogue sur les espaces de suites $\ell^p(\mathbf{N})$; ces recherches, comme nous le verrons plus loin, devaient grandement contribuer à éclaircir les idées sur la dualité, du fait que l’on rencontrait ici pour la première fois deux espaces en dualité et non naturellement isomorphes *.

Dès ce moment, F. Riesz pensait à une étude axiomatique englobant tous ces résultats ((IX a), p. 452), et il semble que seul un scrupule d’analyste soucieux de ne pas trop s’éloigner des mathématiques classiques l’ait retenu d’écrire sous cette forme son célèbre mémoire de 1918 sur la théorie de Fredholm (IX d). Il y considère en principe l’espace $C(I)$ des fonctions continues dans un intervalle compact ; mais, après avoir défini la norme de cet espace, et avoir remarqué que $C(I)$, muni de cette norme, est complet, il n’utilise plus jamais, dans ses raisonnements, autre chose que les axiomes des espaces normés complets **. Sans entrer ici dans l’examen détaillé de ce travail, mentionnons que c’est là que se trouve pour la première fois définie de façon générale la notion d’application linéaire complètement continue (par la propriété de transformer un voisinage en un ensemble relativement compact) *** ; par un chef-d’œuvre d’analyse axiomatique, toute la théorie de Fredholm (sous son aspect qualitatif) est ramenée à un seul théorème fondamental, savoir que tout espace normé localement compact est de dimension finie.

La définition générale des espaces normés fut donnée en 1920-1922 par S. Banach, H. Hahn et E. Helly (ce dernier ne considérant que des espaces de suites de nombres réels ou complexes). Dans les dix années qui suivent, la théorie de ces espaces se développe principalement autour de deux questions d’une importance fondamentale dans les applications : la théorie de la dualité et les théorèmes se rattachant à la notion de « catégorie » de Baire.

\* Bien que la dualité entre $L^1$ et $L^\infty$ soit implicite dans la plupart des travaux de cette époque sur l’intégrale de Lebesgue, c’est seulement en 1918 que H. Steinhaus démontra que toute forme linéaire continue sur $L^1(I)$ (I intervalle fini) est de la forme $x \mapsto \int_I f(t) \, x(t) \, dt$, où $f \in L^\infty(I)$.

** F. Riesz remarque d’ailleurs explicitement que l’application de ses théorèmes aux fonctions continues n’est là que comme « pierre de touche » de conceptions beaucoup plus générales ((IX d), p. 71).

*** Dans ses travaux sur les espaces $L^p$, F. Riesz avait défini les applications complètement continues comme étant celles qui transforment toute suite faiblement convergente en suite fortement convergente ; ce qui (compte tenu de la compacité faible de la boule unité dans les $L^p$ pour $1 < p < + \infty$) est équivalent, dans ce cas, à la définition précédente ; en outre, F. Riesz avait indiqué que, pour l’espace $L^2$, sa définition était équivalente à celle de Hilbert (en la traduisant du langage des applications linéaires dans celui des formes bilinéaires ((IX a), p. 487)).

Nous avons vu que l’idée de dualité (au sens topologique) remonte au début du xx\textsuperscript{e} siècle ; elle est sous-jacente à la théorie de Hilbert et occupe une place centrale dans l’œuvre de F. Riesz. Ce dernier observe par exemple, dès 1911 ((IX b), p. 41-42), que la relation $|f(x)| \leq M \|x\|$ (prise comme définition des fonctionnelles linéaires « bornées » dans l’espace de Hilbert) est équivalente à la continuité de $f$ lorsqu’on se place dans l’espace $\mathcal{C}(I)$, et ce par un raisonnement de caractère tout à fait général. À propos de la caractérisation des fonctionnelles linéaires continues sur $\mathcal{C}(I)$, il remarque aussi que la condition pour qu’un ensemble A soit total dans $\mathcal{C}(I)$ est qu’il n’existe aucune mesure de Stieltjes $\mu \neq 0$ sur I qui soit « orthogonale » à toute fonction de A (généralisant ainsi la condition de Gram pour les systèmes orthonormaux complets) ; il constate enfin, dans le même travail, que le dual de l’espace $L^\infty$ est « plus grand » que l’espace des mesures de Stieltjes ((IX b), p. 62).

D’autre part, dans ses travaux sur les espaces $L^p(I)$ et $\ell^p(\mathbf{N})$, F. Riesz parvient à modifier la méthode de résolution des systèmes linéaires dans l’espace de Hilbert, donnée par E. Schmidt (VIII b), de façon à la rendre applicable à des cas plus généraux. L’idée de E. Schmidt consistait à déterminer une solution « extrémale » de (6) en cherchant le point de la variété linéaire fermée représentée par les équations (6), dont la distance à l’origine est minima. En utilisant la même idée, F. Riesz montre qu’une condition nécessaire et suffisante pour qu’il existe une fonction $x \in L^p(a, b)$ satisfaisant aux équations

$$
\int_a^b \alpha_i(t) \, x(t) \, dt = b_i \quad (i = 1, 2, ...)
$$

(où les $\alpha_i$ appartiennent à $L^q$ (avec $\frac{1}{p} + \frac{1}{q} = 1$)), et telle en outre que $\int_a^b |x(t)|^p dt \leq M^p$, est que, pour toute suite finie $(\lambda_i)_{1 \leq i \leq n}$ de nombres réels, on ait

$$
|\sum_{i=1}^n \lambda_i b_i| \leq M \left( \int_a^b |\sum_{i=1}^n \lambda_i \alpha_i(t)|^q dt \right)^{1/q}
$$

En 1911 (IX b), il traite de façon analogue le « problème des moments généralisés », consistant à résoudre le système

$$
\int_a^b \alpha_i(t) \, d\xi(t) = b_i \quad (i = 1, 2, ...)
$$

où les $\alpha_i$ sont continues et l’inconnue est une mesure de Stieltjes $\xi$* ; il est visible

\* Le « problème des moments » classique correspond au cas où l’intervalle $]a, b[$ est $]0, +\infty[$ (ou $]-\infty, +\infty[$), et où $\alpha_i(t) = t^i$; en outre on impose à la mesure $\xi$ d’être positive (F. Riesz indique dans son mémoire de 1911 comment ses conditions générales doivent être modifiées lorsqu’on cherche des solutions de cette nature). Parmi les diverses méthodes de résolution du problème des moments classique, il faut en particulier signaler celle de M. Riesz, qui combine avec élégance les idées générales du Calcul fonctionnel et la théorie des fonctions d’une variable complexe pour obtenir des conditions explicites sur les $b_i$. (Sur le problème des moments, 3, Ark. för Math., t. XVII (1922-1923), n° 16, 52 p.)

ici que l’on peut énoncer le problème en disant qu’il s’agit de déterminer une fonctionnelle linéaire continue sur $\mathcal{C}(I)$ par ses valeurs en une suite de points donnés dans cet espace. C’est aussi sous cette forme que Helly traite le problème en 1912 — obtenant les conditions de F. Riesz par une méthode assez différente et de plus ample portée \* — et qu’il le reprend en 1921, dans des conditions beaucoup plus générales. Introduisant la notion de norme (sur les espaces de suites) comme nous l’avons vu plus haut, il remarque que cette notion généralise celle de « jauge » d’un corps convexe de l’espace à $n$ dimensions, utilisée par Minkowski dans ses célèbres travaux sur la « géométrie des nombres » (IV). Au cours de ces travaux, Minkowski avait aussi défini (dans $\mathbf{R}^n$) les notions d’hyperplan d’appui et de « fonction d’appui » (IV $b$), et démontré l’existence d’un hyperplan d’appui en tout point frontière d’un corps convexe ((IV $a$), p. 33-35). Helly étend ces notions à un espace de suites $E$, muni d’une norme quelconque ; il établit une dualité entre $E$ et l’espace $E'$ des suites $u = (u_n)$ telles que, pour tout $x = (x_n) \in E$, la série $(u_n x_n)$ soit convergente ; $\langle u, x \rangle$ désignant la somme de cette série, il définit dans $E'$ une norme par la formule $\sup_{x \neq 0} |\langle u, x \rangle| / \|x\|$, qui donne la fonction d’appui dans les espaces de dimension finie **. La résolution d’un système (6) dans $E$, où chacune des suites $u_i = (a_{ij})_{j \geq 1}$ est supposée appartenir à $E'$, revient, comme le montre alors Helly, à résoudre successivement les deux problèmes suivants : 1° trouver une forme linéaire continue $L$ sur l’espace normé $E'$, telle que $L(u_i) = b_i$ pour tout indice $i$, ce qui, comme il l’indique, conduit à des conditions du type (10) ; 2° chercher si une telle forme linéaire peut s’écrire $u \mapsto \langle u, x \rangle$ pour un $x \in E$. Ce dernier problème, comme l’observe Helly, n’a pas nécessairement de solution même lorsque $L$ existe, et il se borne à donner quelques conditions suffisantes qui entraînent l’existence de la solution $x \in E$ dans certains cas particuliers (X).

Ces idées acquièrent leur forme définitive en 1927, dans un mémoire fondamental de H. Hahn (XI) dont les résultats sont retrouvés (de façon indépendante) par S. Banach deux ans plus tard (XII $b$). Le procédé de Minkowski-Helly est appliqué par Hahn à un espace normé quelconque, et donne donc sur le dual une structure d’espace normé (complet), ce qui permet aussitôt à Hahn de considérer les duals successifs d’un espace normé, et de poser de façon générale le problème des espaces réflexifs, entrevu par Helly. Mais surtout le problème capital du prolongement d’une fonctionnelle linéaire continue avec conservation de sa norme est définitivement résolu par Hahn de façon tout à fait générale, par un raisonnement de récurrence transfinie sur la dimension — donnant ainsi un des premiers exemples d’une application importante de l’axiome du choix à l’Analyse fonctionnelle ***. A ces résultats,

\* Comme F. Riesz ((IX $b$), p. 49-50), Helly utilise dans cette démonstration un « principe de choix » qui n’est autre, bien entendu, que la compacité faible de la boule unité dans l’espace des mesures de Stieltjes ; F. Riesz avait aussi fait usage de la propriété analogue dans les espaces $L^p(1 < p < +\infty)$.
** Pour obtenir ainsi une norme, il faut supposer que la relation $\langle u, x \rangle = 0$ pour tout $x \in E$ entraîne $u = 0$, comme le remarque d’ailleurs explicitement Helly.
*** Banach avait déjà fait un raisonnement analogue en 1923, pour définir une mesure invariante dans le plan (définie pour toute partie bornée) (XII $a$).

Banach ajoute une étude poussée des relations entre une application linéaire continue et sa transposée, étendant aux espaces normés généraux des résultats connus seulement jusque-là pour les espaces $L^p$ (IX a), au moyen d’un théorème très profond sur les parties faiblement fermées d’un dual (cf. IV, p. 25, cor. 2); ces résultats s’expriment d’ailleurs de façon plus frappante en utilisant la notion d’espace quotient d’un espace normé, introduite quelques années plus tard par Hausdorff et Banach lui-même. Enfin, c’est encore Banach qui découvre le lien entre la compacité faible de la boule unité (observée dans de nombreux cas particuliers, comme nous l’avons signalé ci-dessus) et la réflexivité, tout au moins pour les espaces de type dénombrable ((XII c), p. 189). La théorie de la dualité des espaces normés peut, dès ce moment, être considérée comme fixée dans ses grandes lignes.

A la même époque s’éclaircissent aussi des théorèmes d’allure paradoxale dont les premiers exemples remontent aux environs de 1910. Hellinger et Toeplitz avaient en effet démontré en substance, cette année-là, qu’une suite de formes bilinéaires bornées $B_n(x, y)$ sur un espace de Hilbert, dont les valeurs $B_n(a, b)$ pour tout couple donné $(a, b)$ sont majorées (par un nombre dépendant $a$ priori de $a$ et $b$), est en fait uniformément bornée dans toute boule. Leur démonstration procède par l’absurde et consiste à construire un couple $(a, b)$ particulier violant l’hypothèse, par une méthode de récurrence connue depuis sous le nom de « méthode de la bosse glissante », et qui rend encore des services dans bien des questions analogues (cf. IV, p. 54, exerc. 15). Dès 1905, Lebesgue avait d’ailleurs utilisé un procédé analogue pour démontrer l’existence de fonctions continues dont la série de Fourier diverge en certains points et, la même année que Hellinger et Toeplitz, il appliquait la même méthode pour démontrer qu’une suite faiblement convergente dans $L^1$ est bornée en norme *. Ces exemples se multiplient dans les années qui suivent, mais sans introduction d’idées nouvelles jusqu’en 1927, date où Banach et Steinhaus (avec la collaboration partielle de S. Saks) relient ces phénomènes à la notion d’ensemble maigre et au th. de Baire dans les espaces métriques complets, obtenant un énoncé général qui englobe tous les cas particuliers antérieurs (XIII). L’étude des questions de « catégorie » dans les espaces normés complets conduit d’ailleurs Banach, à la même époque, à de nombreux autres résultats sur les applications linéaires continues ; le plus remarquable et sans doute le plus profond est le th. du « graphe fermé » qui, comme le th. de Banach-Steinhaus, s’est révélé un outil de premier ordre dans l’Analyse fonctionnelle moderne (XII b).

La publication du traité de Banach sur les « Opérations linéaires » (XII c) marque, pourrait-on dire, le début de l’âge adulte pour la théorie des espaces normés. Tous les résultats dont nous venons de parler, ainsi que beaucoup d’autres, se trouvent exposés dans ce volume, de façon encore un peu désordonnée, mais accompagnés de multiples exemples frappants tirés de domaines variés de l’Analyse, et qui

\* Notons aussi le théorème analogue (plus facile) démontré par Landau en 1907 et qui servit de point de départ à F. Riesz dans sa théorie des espaces $L^p$ : si la série de terme général $u_n x_n$ converge pour toute suite $(x_n) \in \ell^p(\mathbf{N})$, la suite $(u_n)$ appartient à $\ell^q(\mathbf{N})$ (avec $\frac{1}{p} + \frac{1}{q} = 1$).

semblaient présager un brillant avenir à la théorie. De fait, l’ouvrage eut un succès considérable, et un de ses effets les plus immédiats fut l’adoption quasi universelle du langage et des notations utilisés par Banach. Mais, malgré un grand nombre de recherches entreprises depuis 40 ans sur les espaces de Banach (XVII), si l’on excepte la théorie des algèbres de Banach et ses applications à l’analyse harmonique commutative et non commutative, l’absence presque totale de nouvelles applications de la théorie aux grands problèmes de l’Analyse classique a quelque peu déçu les espoirs fondés sur elle.

C’est plutôt dans le sens d’un élargissement et d’une analyse axiomatique plus poussée des conceptions relatives aux espaces normés que se sont produits les développements les plus féconds. Bien que les espaces fonctionnels rencontrés depuis le début du xx\textsuperscript{e} siècle se fussent présentés pour la plupart munis d’une norme « naturelle », on n’avait pas été sans remarquer quelques exceptions. Vers 1910, E. H. Moore avait proposé de généraliser la notion de convergence uniforme en la remplaçant par la notion de « convergence uniforme relative », où un voisinage de 0 est constitué par les fonctions $f$ satisfaisant à une relation $|f(t)| \leq \varepsilon g(t)$, $g$ étant une fonction partout $> 0$, pouvant varier avec le voisinage. On avait d’autre part observé, avant 1930, que des notions telles que la convergence simple, la convergence en mesure pour les fonctions mesurables, ou la convergence compacte pour les fonctions entières, ne se laissaient pas définir au moyen d’une norme ; et en 1926, Fréchet avait noté que des espaces vectoriels de cette nature peuvent être métrisables et complets. Mais la théorie de ces espaces plus généraux ne devait se développer de façon fructueuse qu’en liaison avec l’idée de convexité. Cette dernière (que nous avons vu apparaître chez Helly) fit l’objet d’études de Banach et de ses élèves, qui reconnurent la possibilité d’interpréter ainsi de façon plus géométrique de nombreux énoncés de la théorie des espaces normés, préparant la voie à la définition générale des espaces localement convexes, donnée par Kolmogoroff et J. von Neumann en 1935. La théorie de ces espaces, et notamment les questions touchant à la dualité, ont surtout été développées dans les années 1950, et nous avons exposé dans ce Livre les résultats essentiels de cette étude. Il faut noter à ce propos, d’une part, les progrès en simplicité et en généralité rendus possibles par la mise au point des notions fondamentales de Topologie générale, réalisée entre 1930 et 1940 ; en second lieu, l’importance prise par la notion d’ensemble borné, introduite par Kolmogoroff et von Neumann en 1935, et dont le rôle fondamental dans la théorie de la dualité a été mis en lumière par les travaux de Mackey (XIV) et de Grothen-dieck (XVIII). Enfin et surtout, il est certain que l’impulsion principale qui a motivé ces recherches est venue de nouvelles possibilités d’application à l’Analyse, dans des domaines où la théorie de Banach était inopérante : il faut mentionner à cet égard la théorie des espaces de suites, développée par Köthe, Toeplitz et leurs élèves depuis 1934 dans une série de mémoires (XV), la mise au point de la théorie des « fonctionnelles analytiques » de Fantappié, et surtout la théorie des distributions de L. Schwartz (XVI), où la théorie moderne des espaces localement convexes a trouvé un champ d’applications qui est sans doute loin d’être épuisé.

Bibliographie

(I) C. Sturm : a) Sur les équations différentielles linéaires du second ordre, Journ. de Math. (1), t. I (1836), p. 106-186 ; b) Sur une classe d’opérations à différences partielles, ibid., p. 373-444.
(II) J. Liouville : a) Sur le développement des fonctions ou parties de fonctions en séries dont les divers termes sont assujettis à satisfaire à une même équation différentielle du second ordre contenant un paramètre variable, Journ. de Math. (1), t. I (1836), p. 253-265, t. II (1837), p. 16-35 et 418-436 ; b) D’un théorème dû à M. Sturm et relatif à une classe de fonctions transcendantes, ibid., t. I (1836), p. 269-277.
(III) J. P. Gram, Ueber die Entwicklung reeller Functionen in Reihen mittelst der Methode der kleinsten Quadrate, J. de Crelle, t. XCIV (1883), p. 41-73.
(IV) H. Minkowski : a) Geometrie der Zahlen, 1re éd., Leipzig (Teubner), 1896 ; b) Theorie der konvexen Körper, Gesammelte Abhandlungen, t. II, p. 131-229, Leipzig-Berlin (Teubner), 1911. (Réimpression, New York (Chelsea), 1967.)
(V) H. Poincaré : a) Sur les équations de la Physique mathématique, Rend. Palermo, t. VIII (1894), p. 57-156 (= Œuvres, t. IX, p. 123-196, Paris (Gauthier-Villars), 1954) ; b) La méthode de Neumann et le problème de Dirichlet, Acta Mathematica, t. XX (1896), p. 59-142 (= Œuvres, t. IX, p. 202-272, Paris (Gauthier-Villars), 1954).
(VI) I. Fredholm, Sur une classe d’équations fonctionnelles, Acta Mathematica, t. XXVII (1903), p. 365-390.
(VII) D. Hilbert, Grundzüge einer allgemeinen Theorie der linearen Integralgleichungen, New York (Chelsea), 1953 (= Gött. Nachr., 1904, 1905, 1906, 1910).
(VIII) E. Schmidt : a) Zur Theorie der linearen und nichtlinearen Integralgleichungen. I. Teil : Entwicklung willkürlicher Funktionen nach Systemen vorgeschriebener, Math. Ann., t. LXIII (1907), p. 433-476 ; b) Ueber die Auflösung linearer Gleichungen mit unendlich vielen Unbekannten, Rend. Palermo, t. XXV (1908), p. 53-77.
(IX) F. Riesz : a) Untersuchungen über Systeme integrierbarer Funktionen, Math. Ann., t. LXIX (1910), p. 449-497 ; b) Sur certains systèmes singuliers d’équations intégrales, Ann. Ec. Norm. Sup. (3), t. XXVIII (1911), p. 33-62 ; c) Les systèmes d’équations linéaires à une infinité d’inconnues, Paris (Gauthier-Villars), 1913 ; d) Ueber lineare Funktionalgleichungen, Acta Mathematica, t. XLI (1918), p. 71-98 ; e) Zur Theorie des Hilbertschen Raumes, Acta litt. ac scient. (Szeged), t. VII (1934-35), p. 34-38.
(X) E. Helly, Ueber Systeme linearer Gleichungen mit unendlich vielen Unbekannten, Monatshefte für Math. und Phys., t. XXXI (1921), p. 60-91.
(XI) H. Hahn, Ueber lineare Gleichungssysteme in linearen Räumen, J. de Crelle, t. CLVII (1927), p. 214-229.
(XII) S. Banach : a) Sur le problème de la mesure, Fund. Math., t. IV (1923), p. 7-33 ; b) Sur les fonctionnelles linéaires, Studia Math., t. I (1929), p. 211-216 et 223-239 ; c) Théorie des opérations linéaires, Warszawa, 1932. (Réimpression, New York (Chelsea), 1963.)
(XIII) S. Banach et H. Steinhaus, Sur le principe de condensation des singularités, Fund. Math., t. IX (1927), p. 50-61.
(XIV) G. W. Mackey : a) On infinite-dimensional linear spaces, Trans. Amer. Math. Soc., t. LVII (1945), p. 155-207 ; b) On convex topological spaces, Trans. Amer. Math. Soc., t. LX (1946), p. 519-537.
(XV) G. Köthe, Neubegründung der Theorie der vollkommenen Räume, Math. Nachr., t. IV (1951), p. 70-80.
(XVI) L. Schwartz, Théorie des distributions, 2e édition, Paris (Hermann), 1966.
(XVII) J. Lindenstrauss and L. Tzafriri, Classical Banach spaces, t. I, Berlin-Heidelberg-New York (Springer), 1977.
(XVIII) A. Grothendieck : a) Produits tensoriels topologiques et espaces nucléaires, Mem. Amer. Math. Soc., n° 16 (1955) ; b) Espaces vectoriels topologiques, 3e éd., São Paulo (Publ. Soc. Mat. São Paulo), 1964.

Index des notations

Chapitre I :
|ξ|, \|x\| : I, p. 3.
$\mathcal{B}(I; K)$, $\mathcal{B}_K(I)$, $\ell_K^\infty(I)$, $\ell_K^1(I)$, $\mathcal{B}(I)$, $\ell^1(I)$ : I, p. 4.

Chapitre II :
E_A (A ensemble convexe symétrique dans un espace vectoriel réel E) : II, p. 28.
$\langle x, y \rangle$ : II, p. 45.
σ(F, G) : II, p. 45.
M°, M°° : II, p. 47.
'u (u application linéaire) : II, p. 50.

Chapitre III :
$\mathcal{R}(X)$ : III, p. 9.
$\mathcal{C}^\infty(U)$ : III, p. 9.
$\mathcal{C}_H^\infty(U)$, $\mathcal{C}_c^\infty(U)$ : III, p. 9.
$\mathcal{G}_{s,M}(I)$, $\mathcal{G}_s(I)$, $\mathcal{C}(I)$ : III, p. 10.
$\mathcal{H}(U)$, $\mathcal{H}(L)$ (U ouvert de $\mathbf{C}^n$, L compact de $\mathbf{C}^n$) : III, p. 10.
$\mathcal{L}(E; F)$ : III, p. 13.
$\mathcal{L}_\Xi(E; F)$ : III, p. 14.
$\mathcal{L}_s(E; F)$, $\mathcal{L}_c(E; F)$, $\mathcal{L}_{pc}(E; F)$, $\mathcal{L}_{cc}(E; F)$, $\mathcal{L}_b(E; F)$ : III, p. 14.
E', E'_\Xi, E'_s, E'_c, E'_{pc}, E'_{cc}, E'_b : III, p. 14.
$\mathcal{L}(E)$, $\mathcal{L}_\Xi(E)$, $\mathcal{L}_s(E)$, $\mathcal{L}_c(E)$, $\mathcal{L}_{pc}(E)$, $\mathcal{L}_{cc}(E)$, $\mathcal{L}_b(E)$ : III, p. 14.
$p_M$ (p semi-norme, M partie bornée) : III, p. 14.
$\mathcal{C}_0(\mathbf{R})$ : III, p. 18.

Chapitre IV :
τ(E, F) : IV, p. 2.
β(E, F) : IV, p. 4.
c_E : IV, p. 14.
$\ell^\infty(N)$, $c_0(N)$, $\ell^1(N)$ : IV, p. 17.
S(E) : IV, p. 26.
H_p : IV, p. 26.
E_\sigma : IV, p. 32.
$\mathcal{C}_s(X)$ : IV, p. 33.
$\mathcal{C}^b(X)$, $\mathcal{C}(X)$ : IV, p. 36.
$\mathcal{B}(X; \mathbf{R})$ : IV, p. 40.
Ind(u) (u opérateur de Fredholm) : IV, p. 67; exerc. 21.

Chapitre V :
$\overline{\xi}$ : V, p. 1.
$\ell^2$, $\ell^2(N)$ : V, p. 4.
E_{(c)} : V, p. 4.
$\langle x|y \rangle, \|x\| = \langle x|x \rangle^{1/2}, (x|y) = \langle y|x \rangle$ : V, p. 5.
$\overline{E}$ (E espace préhilbertien complexe) : V, p. 6.
$\mathcal{H}^s$ (espace de Sobolev) : V, p. 7.
H^2(D) : V, p. 7.

$\mathcal{C}_0^1(U)$ : V, p. 8.
$p_H$ (H convexe séparé et complet dans un espace préhilbertien) : V, p. 10.
$x^*$ (x vecteur d’un espace hilbertien) : V, p. 15 et p. 39.
$\bigoplus_{i \in I} E_i$, $\bigoplus_{i \in I} E_i$ : V, p. 18.
$E_1 \oplus E_2 \oplus \ldots \oplus E_n$ (E_i espaces hilbertiens) : V, p. 18.
$\ell_E^2(I)$, $\ell^2(I)$ (E espace hilbertien) : V, p. 18.
$E_1 \otimes_2 E_2$, $\|z\|_2$ ($z \in E_1 \otimes_2 E_2$) : V, p. 26.
$E_1 \otimes_2 E_2 \otimes_2 \ldots \otimes_2 E_n$, $\bigotimes_{i=1}^n E_i$, $\|z\|_2$ ($z \in \bigotimes_{i=1}^n E_i$) : V, p. 27.
$E_1 \hat{\otimes}_2 E_2 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$, $\bigotimes_{1 \leq i \leq n} E_i$ : V, p. 28 et p. 29.
$u_1 \hat{\otimes}_2 u_2 \hat{\otimes}_2 \ldots \hat{\otimes}_2 u_n$ ($u_i$ applications linéaires) : V, p. 28.
$\hat{T}^n(E)$, $E^{\hat{\otimes}n}$ : V, p. 29.
$\hat{S}^n(E)$, $\hat{S}(E)$ : V, p. 30.
$\hat{T}^n(u)$, $\hat{S}^n(u)$ ($u$ application linéaire) : V, p. 32.
$\hat{\Lambda}^n(E)$, $\hat{\Lambda}(E)$ : V, p. 34.
$\hat{\Lambda}^n(u)$ ($u$ application linéaire) : V, p. 34.
$v.u,\ v u$ ($u,\ v$ applications linéaires) : V, p. 37.
$u^*$ ($u$ application linéaire) : V, p. 38.
$\mathcal{H}(E)$ (E espace hilbertien) : V, p. 43.
$u \geq 0$ ($u$ endomorphisme d’espace hilbertien) : V, p. 45.
$\mathcal{L}_+(E)$ : V, p. 45.
$u \geq v$ ($u,\ v$ dans $\mathcal{L}(E)$, E espace hilbertien) : V, p. 45.
$\tau(u)$ ($u$ endomorphisme de rang fini) : V, p. 48.
$\mathrm{Tr}(u)$ ($u \geq 0$ dans $\mathcal{L}(E)$) : V, p. 49.
$\mathcal{L}^1(E)$ (E espace hilbertien) : V, p. 50.
$\mathcal{L}^2(E; F)$, $\mathcal{L}^2(E)$ (E, F espaces hilbertiens) : V, p. 51.
$\|u\|_2$ ($u \in \mathcal{L}(E; F)$, E, F espaces hilbertiens) : V, p. 52.
$\mathrm{Tr}(Q/H)$ (Q, H formes quadratiques positives) : V, p. 57.

Index terminologique

Absorbant (ensemble), absorption d’un ensemble par un autre : I, p. 7.
Adaptée (bornologie) : III, p. 3.
Adjoint : V, p. 38.
Affaiblie (topologie) : IV, p. 4.
Affine (transformation) : IV, p. 39.
Application bilinéaire $\mathcal{S}$-hypocontinue, $\mathcal{T}$-hypocontinue, ($\mathcal{S}, \mathcal{T}$)-hypocontinue : III, p. 31.
Application bilinéaire séparément continue : III, p. 28.
Application canonique de $\bigoplus_{i \in I} E'_i$ dans $(\prod_{i \in I} E_i)'$ : IV, p. 13.
Application canonique de $E$ dans $E''$ : IV, p. 14.
Application canonique de $E$ sur $E'$ (E espace hilbertien) : V, p. 15.
Application (linéaire) compacte : III, p. 6.
Application de Hilbert-Schmidt : V, p. 51.
Application partiellement isométrique : V, p. 41.
Associé (espace vectoriel topologique séparé) à un espace vectoriel topologique : I, p. 4.
Automorphisme d’un espace vectoriel topologique : I, p. 3.

Banach (espace de) : I, p. 5.
Banach (théorème de) : I, p. 17.
Banach-Dieudonné (théorème de) : IV, p. 24.
Banach-Saks-Kakutani (théorème de) : V, p. 67, exerc. 33.
Banach-Steinhaus (théorème de) : III, p. 26.
Base algébrique d’un espace hilbertien : V, p. 22.
Base banachique : IV, p. 70, exerc. 14.
Base banachique complète, base banachique contractante : IV, p. 70, exerc. 15.
Base banachique inconditionnelle : IV, p. 71, exerc. 16.
Base d’une bornologie : III, p. 1.
Base orthonormale : V, p. 22.
Bessel (inégalité de) : V, p. 21.
Bidual : IV, p. 14.
Bipolaires (théorème des) : II, p. 48.
Birkhoff-Alaoglu (théorème de) : V, p. 77, exerc. 13.
Bishop-Phelps (théorème de) : II, p. 82, exerc. 4.
Borné (ensemble) : III, p. 2 et p. 38, exerc. 1.
Bornivore (ensemble) : III, p. 40, exerc. 11.
Bornologie : III, p. 1.
Bornologie adaptée : III, p. 3.
Bornologie canonique : III, p. 3.
Bornologie convexe : III, p. 2.
Bornologie engendrée par un ensemble de parties : III, p. 1.
Bornologie produit : III, p. 1.
Bornologique (espace localement convexe) : III, p. 12.

Canonique (bornologie) : III, p. 3.
Canonique (topologie) sur un espace vectoriel de dimension finie : I, p. 2.
Carré scalaire : V, p. 5.
Cauchy-Schwarz (inégalité de) : V, p. 3.
Chapeau : II, p. 61.
Cobord : IV, p. 73. exerc. 3, exerc. 3.

l-cocycle continu : IV, p. 73, exerc. 3.
Compacte (application) : III, p. 6.
Compatible avec la dualité (topologie localement convexe) : IV, p. 1.
Compatibles (structure d’espace vectoriel et topologie) : I, p. 1.
Compatibles (structure d’espace vectoriel et préordre) : II, p. 13.
Compatibles (topologie et structure d’espace vectoriel ordonné) : II, p. 17.
Complet (espace vectoriel topologique) : I, p. 5.
Complété d’un espace préhilbertien séparé : V, p. 8.
Complété d’un espace vectoriel topologique séparé : I, p. 6.
Complexe (forme linéaire) : II, p. 65.
Complexe (variété linéaire) : II, p. 65.
Complexifié d’un espace préhilbertien réel : V, p. 5
Complexité d’un espace vectoriel topologique sur $\mathbf{R}$ : II, p. 65.
Concave (fonction) : II, p. 18.
Cône, cône épointé, cône pointé : II, p. 11.
Cône asymptote : II, p. 41, exerc. 14.
Cône convexe, cône convexe pointé saillant : II, p. 11.
Cône convexe engendré par un ensemble : II, p. 12.
Cône polyédral : II, p. 96, exerc. 24.
Conjugué d’un espace préhilbertien complexe : V, p. 6.
Convexe (bornologie) : III, p. 2.
Convexe (ensemble) : II, p. 8 et p. 66.
Convexe (fonction) : II, p. 17.
Convexe équilibrée (enveloppe) d’un ensemble : II, p. 10 et p. 66.
Convexe symétrique (enveloppe) d’un ensemble : II, p. 10.
Coordonnées par rapport à une base orthonormale : V, p. 22.
Côté (points d’un même, points strictement d’un même) d’un hyperplan : II, p. 9.

Décomposition polaire d’un opérateur de Hilbert-Schmidt : V, p. 78, exerc. 14.
Demi-espaces fermés (ouverts) déterminés par un hyperplan fermé : II, p. 16.
Densité d’ordre $\alpha$ : V, p. 7.
Déterminant de Gram : V, p. 70, exerc. 7.
Dimension d’un ensemble convexe : II, p. 10.
Dimension hilbertienne : V, p. 25.
Dirichlet (espace de) : V, p. 8.
Distal (ensemble) : IV, p. 72, exerc. 1.
Distingué (espace) : IV, p. 52, exerc. 4.
Dual algébrique d’un espace vectoriel topologique réel : II, p. 45.
Dual d’un espace vectoriel topologique réel : II, p. 45.
Dual d’un espace localement convexe (réel ou complexe) : III, p. 14.
Dual faible, dual fort : III, p. 14.
Dualité séparante en F, dualité séparante : II, p. 44.
Dualité (espaces vectoriels en) : II, p. 43.
Dvoretzky-Rogers (théorème de) : V, p. 62, exerc. 14.

Eberlein (théorème d’) : IV, p. 35.
D. Edwards (théorème de) : II, p. 100, exerc. 41.
Endomorphisme hermitien : V, p. 43.
Endomorphisme normal : V, p. 42.
Endomorphisme positif : V, p. 45.
Engendrée (bornologie) par un ensemble de parties : III, p. 1.
Ensemble absorbant : I, p. 7.
Ensemble convexe : II, p. 8 et p. 66.
Ensemble équilibré : I, p. 6.
Ensemble filtrant de semi-normes : II, p. 3.
Ensemble orthonormal : V, p. 21.
Ensemble topologiquement libre : I, p. 12.

Ensemble total : I, p. 12.
Ensembles orthogonaux : V, p. 12.
Enveloppe convexe d’un ensemble : II, p. 10.
Enveloppe convexe équilibrée d’un ensemble : II, p. 10.
Enveloppe convexe symétrique d’un ensemble : II, p. 10.
Enveloppe équilibrée d’un ensemble : I, p. 6.
Enveloppe fermée convexe d’un ensemble : II, p. 14.
Enveloppe fermée convexe équilibrée d’un ensemble : II, p. 14 et p. 66.
Enveloppe fermée convexe symétrique d’un ensemble : II, p. 14.
Épointé (cône) : II, p. 11.
\mathcal{S}-équihypocontinu, \mathcal{T}-équihypocontinu, (\mathcal{S}, \mathcal{T})-équihypocontinu (ensemble) : III, p. 49, exerc. 7.
Équilibré (ensemble) : I, p. 6.
Équilibré (noyau) d’un ensemble : I, p. 7.
Équilibrée (enveloppe) d’un ensemble : I, p. 6.
Espace bornologique : III, p. 12.
Espace de Banach : I, p. 5.
Espace de Dirichlet : V, p. 8.
Espace de Fock antisymétrique : V, p. 34.
Espace de Fock symétrique : V, p. 33.
Espace de Fréchet : II, p. 26 et p. 66.
Espace de Gevrey : III, p. 10.
Espace de Hardy : V, p. 7.
Espace de Hilbert : V, p. 6.
Espace de R. C. James : IV, p. 72, exerc. 18.
Espace de Montel : IV, p. 18.
Espace de Sobolev : V, p. 7.
Espace (DF) : IV, p. 58, exerc. 2.
Espace faible : II, p. 45.
Espace gaussien : V, p. 33.
Espace hilbertien : V, p. 6.
Espace limite inductive d’une famille d’espaces localement convexes : II, p. 31.
Espace limite inductive stricte d’une suite d’espaces localement convexes : II, p. 36.
Espace localement convexe complexe : II, p. 66.
Espace localement convexe réel : II, p. 25.
Espace préhilbertien complexe, espace préhilbertien réel : V, p. 4.
Espace quasi-complet : III, p. 8.
Espace réflexif : IV, p. 16.
Espace semi-complet : III, p. 7.
Espace semi-réflexif : IV, p. 15.
Espace semi-tonnelé : IV, p. 21.
Espace tonnelé : III, p. 24.
Espace vectoriel ordonné, espace vectoriel préordonné : II, p. 13.
Espace vectoriel sous-jacent à un espace vectoriel topologique : I, p. 1.
Espace vectoriel topologique : I, p. 1.
Espace vectoriel topologique complet : I, p. 5.
Espace vectoriel topologique métrisable : I, p. 16.
Espace vectoriel topologique séparé associé à un espace vectoriel topologique : I, p. 4.
Étoilé (ensemble) : II, p. 69, exerc. 1.
Exhaustion d’un espace localement convexe séparé, espace exhaustible : III, p. 50, exerc. 1.
Extrémal (point) d’un ensemble convexe : II, p. 57.
Extrémale (générateurice) d’un cône convexe : II, p. 60.

Facette : II, p. 92, exerc. 3.
Facettes duales : II, p. 93, exerc. 6.
Faible (dual) : III, p. 14.
Faible (topologie, espace) : II, p. 45.

Faiblement bornée (partie de E') : III, p. 14.
Famille orthonormale : V, p. 21.
Famille topologiquement libre : I, p. 12.
Fermée convexe (enveloppe) d’un ensemble : II, p. 14.
Fermée convexe équilibrée (enveloppe) d’un ensemble : II, p. 14.
Fermée convexe symétrique (enveloppe) d’un ensemble : II, p. 14.
Fermés (demi-espaces) déterminés par un hyperplan fermé : II, p. 16.
Filtrant (ensemble) de semi-normes : II, p. 3.
Final (sous-espace) : V, p. 41.
Finale (topologie localement convexe) : II, p. 30.
Fock (espaces de) : V, p. 33-34.
Fonction concave, convexe, strictement concave, strictement convexe : II, p. 17-18.
Fonction de type positif : V, p. 9.
Fonction positivement homogène, fonction sous-linéaire : II, p. 21.
Forme bilinéaire mettant deux espaces en dualité : II, p. 43.
Forme hermitienne (à gauche) : V, p. 1.
Forme hermitienne positive : V, p. 2.
Forme hermitienne séparante associée à une forme hermitienne : V, p. 2.
Forme linéaire complexe, forme linéaire réelle : II, p. 65.
Forme linéaire positive : II, p. 14.
Formules de polarisation : V, p. 2.
Fort (dual) : III, p. 14.
Fortement bornée (partie de E') : III, p. 14.
Fréchet (espace de) : II, p. 26 et p. 66.

Gaussien (espace) : V, p. 33.
Génératrice extrémale d’un cône convexe : II, p. 60.
Gevrey (espace de) : III, p. 10.
Graphe fermé (théorème du) : I, p. 19.
Grothendieck (théorème de) : III, p. 20.

Haar (théorème de) : II, p. 88, exerc. 8.
Hadamard (inégalités de) : V, p. 37,
Hahn-Banach (théorème de) : II, p. 24, p. 39 et p. 67.
Hardy (espace de) : V, p. 7.
Helly (théorème de) : II, p. 73, exerc. 21.
Hermitien (endomorphisme) : V, p. 43.
Hilbert (espace de) : V, p. 6.
Hilbert-Schmidt (application de) : V, p. 51.
Hilbertien (espace) : V, p. 6.
\mathcal{S}-hypocontinue, \mathcal{T}-hypocontinue, (\mathcal{S}, \mathcal{T})-hypocontinue (application bilinéaire) : III, p. 31.
Hyperplan d’appui d’un ensemble : II, p. 40.

Indice d’un opérateur de Fredholm : IV, p. 67, exerc. 21.
Induite (structure préhilbertienne) sur un sous-espace vectoriel : V, p. 6.
Inégalité de Bessel : V, p. 21,
Inégalité de Cauchy-Schwarz : V, p. 3.
Inégalités de Hadamard : V, p. 37.
Infratonné (espace) : III, p. 45, exerc. 7.
Initial (sous-espace) : V, p. 41.
Interne (point) d’un ensemble convexe : II, p. 28.
Isomorphisme d’espaces vectoriels topologiques : I, p. 3.
Isomorphisme d’espaces préhilbertiens : V, p. 5.

R. C. James (espace de) : IV, p. 72, exerc. 18.
James-Klee (théorème de) : IV, p. 57, exerc. 25.
Jauge d’un ensemble convexe : II, p. 22.

Krein (théorème de) : IV, p. 37.
Krein-Milman (théorème de) : II, p. 59.

Limite inductive d’espaces (de topologies) localement convexes : II, p. 31.
Limite inductive stricte d’espaces (de topologies) localement convexes : II, p. 36.
Localement convexe complexe (espace) : II, p. 66.
Localement convexe réel (espace) : II, p. 25.
Localement convexe (topologie) : II, p. 25 et p. 66.

Mackey (théorème de) : IV, p. 2.
Mackey (topologie de) : IV, p. 2.
Markoff-Kakutani (théorème de) : IV, p. 39.
Matrice par rapport à des bases orthonormales : V, p. 22.
Matrice de Hilbert : V, p. 74, exerc. 3.
Métrisable (espace vectoriel topologique) : I, p. 16.
Minimal (espace localement convexe de type) : II, p. 90, exerc. 13.
Montel (espace de) : IV, p. 18.
Moyenne : IV, p. 40.
Moyennable (groupe) : IV, p. 73, exerc. 4.

Normal (endomorphisme) : V, p. 42.
Noyau équilibré d’un ensemble : I, p. 7.

Opérateur de Fredholm : IV, p. 67, exerc. 21.
Opérateur unitaire : V, p. 40.
Ordonné (espace vectoriel) : II, p. 13.
Orthogonal d’un sous-espace (pour des espaces en dualité) : II, p. 48.
Orthogonal à un sous-ensemble (pour un vecteur d’un espace préhilbertien) : V, p. 12.
Orthogonales (parties d’espaces en dualité) : II, p. 44.
Orthogonaux (ensembles) dans un espace préhilbertien : V, p. 12.
Orthogonaux (vecteurs) dans des espaces en dualité : II, p. 44.
Orthogonaux (vecteurs) dans un espace préhilbertien : V, p. 5.
Orthonormal (ensemble, famille) : V, p. 21.
Orthonormale (base) : V, p. 22.
Orthonormalisation : V, p. 24.
Orthoprojecteur : V, p. 13.
Orthoprojecteur initial, final : V, p. 41.
Ouverts (demi-espaces) déterminés par un hyperplan fermé : II, p. 16.

Parabolique (ensemble convexe) : II, p. 71, exerc. 17.
Parseval (relation de) : V, p. 22.
Partiellement isométrique (application) : V, p. 41.
Parties orthogonales de deux espaces en dualité : II, p. 44.
Point extrémal d’un ensemble convexe : II, p. 57.
Point interne d’un ensemble convexe : II, p. 28.
Pointé (cône) : II, p. 11.
Points d’un même côté, points strictement d’un même côté d’un hyperplan : II, p. 9.
Points de lissité, de stricte convexité : II, p. 93, exerc. 6.
Polaire d’un ensemble : II, p. 47 et p. 68.
Polyèdre : II, p. 96, exerc. 24.
Polynôme de Legendre : V, p. 24.
Positif (endomorphisme) : V, p. 45.
Positive (forme hermitienne) : V, p. 2.
Positive (forme linéaire) : II, p. 14.
Positivement homogène (fonction) : II, p. 21.
Prédual : IV, p. 56, exerc. 23.
Préhilbertien (espace) : V, p. 4.

Préhilbertienne (semi-norme) : V, p. 4.
Préordonné (espace vectoriel) : II, p. 13.
Principe de condensation des singularités : III, p. 43, exerc. 10.
Produit (bornologie) : III, p. 1.
Produit scalaire : V, p. 5.
Produit tensoriel d’espaces préhilbertiens : V, p. 26.
Produit tensoriel hilbertien : V, p. 28.
Projecteur orthogonal : V, p. 13.
Projection sur un ensemble convexe : V, p. 11.
Pythagore (théorème de) : V, p. 12.

Quasi-complet (espace) : III, p. 8.

Réelle (forme linéaire, variété linéaire affine) : II, p. 65.
Réflexif (espace) : IV, p. 16.
Relation de Parseval : V, p. 22.
Relativement borné (espace) : III, p. 45, exerc. 6.
Représentation unitaire : IV, p. 44.
Ryll-Nardzewski (théorème de) : IV, p. 43.

Saillant (cône convexe pointé) : II, p. 11.
Segment fermé, ouvert, fermé en x et ouvert en y : II, p. 7.
Semelle d’un cône : II, p. 64.
Semi-automorphisme d’espaces préhilbertiens : V, p. 6.
Semi-complet (espace) : III, p. 7.
Semi-norme : II, p. 1.
Semi-norme préhilbertienne : V, p. 4.
Semi-normé (espace) : II, p. 3.
Semi-réflexif (espace) : IV, p. 15.
Semi-tonnelé (espace) : IV, p. 21.
Séparante (dualité) : II, p. 44.
Séparé complété d’un espace vectoriel topologique : I, p. 6.
Séparé complété d’un espace préhilbertien : V, p. 8.
Séparément continue (application bilinéaire) : III, p. 28.
Séparément équicontinu (ensemble) : III, p. 48, exerc. 6.
Séparés (ensembles) par un hyperplan fermé : II, p. 39.
Simplexe : II, p. 76, exerc. 41.
Šmulian (théorème de) : IV, p. 36.
Sobolev (espace de) : V, p. 7.
Somme directe topologique d’espaces (de topologies) localement convexes : II, p. 32.
Somme hilbertienne externe d’espaces hilbertiens : V, p. 18.
Somme hilbertienne de sous-espaces vectoriels : V, p. 18.
Sous-espace final, sous-espace initial d’une application linéaire continue : V, p. 41.
Sous-espace préhilbertien : V, p. 6.
Sous-jacent (espace vectoriel) à un espace vectoriel topologique : I, p. 1.
Sous-linéaire (fonction) : II, p. 21.
Strictement concave, strictement convexe (fonction) : II, p. 17-18.
Strictement séparés (ensembles) par un hyperplan fermé : II, p. 39.
Supplémentaire orthogonal : V, p. 13.
Système fondamental de semi-normes : II, p. 3.

Tchebycheff (théorème de) : II, p. 89, exerc. 8.
Théorème de Banach : I, p. 17.
Théorème de Banach-Dieudonné : IV, p. 24.
Théorème de Banach-Saks-Kakutani : V, p. 67, exerc. 33.
Théorème de Banach-Steinhaus : III, p. 26.
Théorème de Birkhoff-Alaoglu : V, p. 77, exerc. 13.

Théorème de Bishop-Phelps : II, p. 82, exerc. 4.
Théorème de Dvoretzky-Rogers : V, p. 62, exerc. 14.
Théorème d’Eberlein : IV, p. 35.
Théorème de D. Edwards : II, p. 100, exerc. 41.
Théorème de Grothendieck : III, p. 20.
Théorème de Haar : II, p. 88, exerc. 8.
Théorème de Hahn-Banach : II, p. 24, p. 39 et p. 67.
Théorème de Helly : II, p. 73, exerc. 21.
Théorème de James-Klee : IV, p. 57, exerc. 25.
Théorème de Krein : IV, p. 37.
Théorème de Krein-Milman : II, p. 59.
Théorème de Mackey : IV, p. 2.
Théorème de Markoff-Kakutani : IV, p. 39.
Théorème de Pythagore : V, p. 12.
Théorème de Ryll-Nardzewski : IV, p. 43.
Théorème de Šmulian : IV, p. 36.
Théorème de Tchebycheff : II, p. 89, exerc. 8.
Théorème des bipolaires : II, p. 48
Théorème du graphe fermé : I, p. 19.
Tonneau : III, p. 24.
Tonnelé (espace) : III, p. 24.
$\mathcal{S}$-topologie : III, p. 13 et IV, p. 2.
Topologie affaiblie : IV, p. 4.
Topologie compatible avec une structure d’espace vectoriel : I, p. 1.
Topologie compatible avec une structure d’espace vectoriel ordonné : II, p. 17.
Topologie définie par une semi-norme, par un ensemble de semi-normes : II, p. 3.
Topologie de la convergence simple, compacte, précompacte, convexe compacte, bornée : III, p. 14.
Topologie de Mackey : IV, p. 2.
Topologie faible : II, p. 45.
Topologie initiale : IV, p. 4.
Topologie limite inductive d’une famille de topologies localement convexes : II, p. 31.
Topologie limite inductive stricte d’une suite de topologies localement convexes : II, p. 36.
Topologie localement convexe : II, p. 25 et p. 66.
Topologie localement convexe finale : II, p. 30.
Topologie somme directe d’une famille de topologies localement convexes : II, p. 32.
Topologiquement libre (ensemble, famille) : I, p. 12.
Total (ensemble) : I, p. 12.
Trace d’un endomorphisme : V, p. 49.
Trace d’une forme quadratique par rapport à une autre : V, p. 57.
Transformation affine : IV, p. 39.
Transposée d’une application linéaire continue : II, p. 50 et IV, p. 6.

Ultrabornologique (espace) : III, p. 47, exerc. 19.
Ultranorme : I, p. 26, exerc. 12.
Ultra-semi-norme : II, p. 2.
Unitaire (opérateur) : V, p. 40.

Variété d’appui : II, p. 92, exerc. 3.
Variété linéaire complexe, variété linéaire réelle : II, p. 65.
Vecteur orthogonal à un sous-espace dans un espace préhilbertien : V, p. 12.
Vecteurs orthogonaux dans deux espaces en dualité : II, p. 44.
Vecteurs orthogonaux dans un espace préhilbertien : V, p. 5.

Résumé de quelques propriétés importantes des espaces de Banach

Nous rassemblons pour la commodité du lecteur les principaux résultats concernant les espaces normés et plus particulièrement les espaces de Banach. Le corps K des scalaires est égal à $\mathbf{R}$ ou $\mathbf{C}$.

Espaces d’applications linéaires ; dual

1) Soient E et F deux espaces normés. Pour qu’une application linéaire $u$ de E dans F soit continue, il faut et il suffit que

$$
\|u\| = \sup_{\|x\| \leq 1} \|u(x)\|
$$

soit fini. L’application $u \mapsto \|u\|$ est une norme sur l’espace vectoriel $\mathcal{L}(E; F)$ des applications linéaires continues de E dans F.

Supposons que F soit un espace de Banach. Alors $\mathcal{L}(E; F)$ est un espace de Banach. Le complété $\hat{E}$ de E est un espace de Banach, et l’application $u \mapsto u|E$ est une isométrie bijective de $\mathcal{L}(\hat{E}; F)$ sur $\mathcal{L}(E; F)$.

2) Soit E un espace normé. On pose $E' = \mathcal{L}(E; K)$ où K est muni de la norme $\lambda \mapsto |\lambda|$. L’espace de Banach $E'$ s’appelle le dual de E, et le dual $E''$ de $E'$ s’appelle le bidual de E.

On note $\sigma(E, E')$ la topologie la moins fine sur E rendant continues les formes linéaires $x' \in E'$; on l’appelle la topologie affaiblie de E. On note $\sigma(E', E)$ la topologie la moins fine sur $E'$ rendant continues les formes linéaires $x' \mapsto \langle x', x \rangle$ sur $E'$, où x parcourt E ; on appelle $\sigma(E', E)$ la topologie faible sur $E'$. La topologie sur $E'$ déduite de la norme s’appelle la topologie forte.

3) Soient E un espace normé et M un sous-espace vectoriel fermé de E. Soit $\pi$ l’application canonique de E sur E/M. On définit une norme sur l’espace vectoriel E/M par
$$
\| \xi \| = \inf_{\pi(x) = \xi} \| x \|.
$$
Lorsque E est un espace de Banach, il en est de même de M et E/M. Pour tout espace normé F, l’application linéaire $u \mapsto u \circ \pi$ de $\mathcal{L}(E/M; F)$ dans $\mathcal{L}(E; F)$ est isométrique.

4) Soit E un espace normé. Pour tout $x' \in E'$, on a par définition
$$
\| x' \| = \sup_{\substack{\| x \| \leq 1 \\ x \in E}} | \langle x', x \rangle | .
$$
De plus (« th. de Hahn-Banach »), on a
$$
\| x \| = \sup_{\substack{\| x' \| \leq 1 \\ x' \in E'}} | \langle x', x \rangle |
$$
pour tout $x \in E$. Autrement dit, l’application canonique de E dans son bidual $E''$ est isométrique.

Polaires et orthogonaux

5) Soit E un espace normé. Pour toute partie A de E (resp. B de E’), on appelle polaire de A (resp. B) et l’on note $A^\circ$ (resp. $B^\circ$) l’ensemble des $x' \in E'$ (resp. $x \in E$) tels que l’on ait
$$
\Re \langle x', x \rangle \geq -1
$$
pour tout $x \in A$ (resp. $x' \in B$). Lorsque A (resp. B) est un sous-espace vectoriel, la relation (5) équivaut à $\langle x', x \rangle = 0$, et l’on dit alors que $A^\circ$ (resp. $B^\circ$) est l’orthogonal de A (resp. B).

6) (« Th. des bipolaires »). Soit E un espace normé. Soit A (resp. B) une partie de E (resp. E’) contenant 0. Alors le bipolaire $A^{\circ \circ}$ de A (resp. $B^{\circ \circ}$ de B) est l’adhérence pour $\sigma(E, E')$ (resp. $\sigma(E', E)$) de l’enveloppe convexe de A (resp. B).

7) Soit A une partie d’un espace normé E. Soit x un point adhérent à A pour $\sigma(E, E')$. Alors x est limite (pour la norme) d’une suite d’éléments de l’enveloppe convexe de A. En particulier, les sous-ensembles convexes de E qui sont fermés pour la topologie d’espace normé ou pour la topologie $\sigma(E, E')$, sont les mêmes.

8) Soient E un espace normé et M un sous-espace vectoriel de E. Pour toute forme linéaire $u_0 \in M'$, il existe une forme linéaire $u \in E'$ prolongeant $u_0$ et telle que $\| u \| = \| u_0 \|$. Soit H l’orthogonal de M dans E’ ; alors l’orthogonal $H^\circ$ de H est l’adhérence de M dans E.

Transposition

9) Soient E et F deux espaces normés et $u \in \mathcal{L}(E; F)$. La transposée ${}^t u \in \mathcal{L}(F'; E')$ de $u$ est définie par la relation
$$
\langle {}^t u(y'), x \rangle = \langle y', u(x) \rangle \quad \text{quels que soient } x \in E, y' \in F'.
$$

On a $\|t'u\| = \|u\|$. Le noyau de $u$ est l’orthogonal dans E de l’image de $t'u$. Le noyau de $t'u$ est l’orthogonal dans F’ de l’image de $u$.

10) Soient E un espace normé, M un sous-espace vectoriel fermé de E et $F = E/M$. Soit i l’injection canonique de M dans E et soit $\pi$ la surjection canonique de E sur F. Alors $t'i$ a pour noyau l’orthogonal $M^\circ$ de M et définit par passage au quotient une isométrie de $E'/M^\circ$ sur $M'$. De plus, $t'\pi$ est une isométrie de $F'$ sur $M^\circ$.

Critères de continuité d’une application linéaire

11) Soient E et F deux espaces de Banach et $u$ une application linéaire de E dans F. Supposons que, pour toute suite $(x_n)_{n \geq 0}$ de points de E tendant vers 0, et telle que $(u(x_n))_{n \geq 0}$ ait une limite $y$ dans F, on ait $y = 0$. Alors $u$ est continue.

\* Supposons que, pour toute partie compacte K de E, toute mesure positive $\mu$ sur K et toute forme linéaire continue $y'$ sur F, la restriction de $y' \circ u$ à K soit $\mu$-mesurable. Alors $u$ est continue. \*

12) Soient E et F deux espaces de Banach et $u \in \mathcal{L}(E; F)$. Alors, ou bien $u(E)$ est maigre, ou bien $u$ est surjective.

Supposons $u$ surjective. Alors il existe un nombre $C > 0$ tel que, pour tout $y \in F$, il existe $x \in E$ avec $u(x) = y$ et $\|x\| \leq C.\|y\|$. Si N est le noyau de $u$, alors $u$ définit par passage au quotient un homéomorphisme de $E/N$ sur F.

13) Soient E et F deux espaces de Banach. Si $u$ est une application linéaire continue et bijective de E dans F, alors $u^{-1}$ est continue.

14) Soient E et F deux espaces de Banach, $u \in \mathcal{L}(E; F)$ et $x' \in E'$. Pour que $x'$ appartienne à l’image de $t'u$, il faut et il suffit qu’il existe un nombre $C > 0$ tel que l’on ait

$$
| \langle x', x \rangle | \leq C.\|u(x)\| \quad \text{pour tout } x \in E .
$$

15) Soient E et F deux espaces de Banach et $u \in \mathcal{L}(E; F)$. Pour que $u$ soit surjective, il faut et il suffit qu’il existe un nombre $C > 0$ tel que l’on ait $\|t'u(y')\| \geq C.\|y'\|$ pour tout $y' \in F'$.

Th. de Banach-Steinhaus

16) (« Th. de Banach-Steinhaus »). Soient E un espace de Banach, F un espace normé et $(u_i)_{i \in I}$ une famille d’éléments de $\mathcal{L}(E; F)$. Soit A l’ensemble des $x \in E$ tels que $\sup_{i \in I} \|u_i(x)\| < +\infty$. Alors ou bien A est maigre et son complémentaire est dense dans E, ou bien on a $\sup_{i \in I} \|u_i\| < +\infty$. En particulier, lorsque $A = E$, on a $\sup_{i \in I} \|u_i\| < +\infty$.

17) Soient E et F deux espaces de Banach et $(u_n)_{n \geq 0}$ une suite d’éléments de $\mathcal{L}(E; F)$. On suppose que la limite $u(x) = \lim_{n \to \infty} u_n(x)$ existe pour tout $x \in E$. Alors, on a $\sup_n \|u_n\| < +\infty$, $u$ est continue et la suite $(u_n)$ tend vers $u$ uniformément sur toute partie compacte de E.

Propriétés de la topologie faible sur un dual

18) Soient E un espace de Banach et B' une partie de E'. Les conditions suivantes sont équivalentes :
(i) B' est contenue dans une boule de E'.
(ii) B' est relativement compacte pour la topologie σ(E', E).
(iii) Pour tout x ∈ E, on a sup |⟨x', x⟩| < +∞.

19) Soit E un espace de Banach et soit B' la boule unité (fermée) de E'. Alors B' est compacte pour σ(E', E). Supposons qu'il existe dans E une partie dénombrable totale ; alors B' est métrisable pour σ(E', E), et il existe dans E' une partie dénombrable dense pour σ(E', E).

20) Soient E un espace de Banach, u une forme linéaire sur E' et B' la boule unité de E'. Les conditions suivantes sont équivalentes :
(i) Il existe x ∈ E tel que u(x') = ⟨x', x⟩ pour tout x' ∈ E'.
(ii) La restriction de u à B' est continue pour la topologie σ(E', E).
(iii) Pour toute suite d'éléments (x'_n) de E' tendant vers 0 pour σ(E', E), on a lim_{n→∞} u(x'_n) = 0.

21) Soient E un espace de Banach, B' la boule unité de E', et C une partie convexe de E' (en particulier, un sous-espace vectoriel). Pour que C soit fermée pour σ(E', E), il faut et il suffit que l'intersection C ∩ rB' soit fermée pour σ(E', E) quel que soit le nombre réel r > 0.

Espaces réflexifs

22) Soient E un espace normé, E'' son bidual et i l'application canonique de E dans E''. La boule unité de E'' est l'adhérence pour σ(E'', E') de l'image par i de la boule unité de E.

Les conditions suivantes sont équivalentes :
(i) L'application isométrique i : E ↦ E'' est surjective.
(ii) La boule unité dans E est compacte pour σ(E, E').

Lorsque ces conditions sont remplies, on dit que E est réflexif.

Topologies compatibles avec la dualité

23) Soit E un espace de Banach et soit T une topologie localement convexe sur E. Les conditions suivantes sont équivalentes :
(i) La topologie T est plus fine que σ(E, E') et moins fine que la topologie définie sur E par la norme.
(ii) E' est l'ensemble des formes linéaires sur E continues pour T.

Supposons ces conditions satisfaites. Soit A une partie de E. Pour que A soit relativement compacte pour T, il faut et il suffit que toute suite de points de A possède dans E une valeur d'adhérence pour T. S'il en est ainsi, l'enveloppe convexe équilibrée de A est relativement compacte pour T.

Table des matières

Chapitre I. — Espaces vectoriels topologiques sur un corps valué ... I.1

§ 1. Espaces vectoriels topologiques ......................... I.1
    1. Définition d’un espace vectoriel topologique ............ I.1
    2. Espaces normés sur un corps valué ....................... I.3
    3. Sous-espaces vectoriels et espaces quotients d’un espace vectoriel topologique ; produits d’espaces vectoriels topologiques ; somme directe topologique de sous-espaces .................. I.4
    4. Structure uniforme et complétion d’un espace vectoriel topologique ............................................. I.5
    5. Voisinages de l’origine dans un espace vectoriel topologique sur un corps valué ................................. I.6
    6. Critères de continuité et d’équicontinuité ............... I.8
    7. Topologies initiales d’espaces vectoriels ................ I.9

§ 2. Variétés linéaires dans un espace vectoriel topologique .......... I.11
    1. Adhérence d’une variété linéaire .......................... I.11
    2. Droites et hyperplans fermés ............................... I.13
    3. Sous-espaces vectoriels de dimension finie ............... I.14
    4. Espaces vectoriels topologiques localement compacts ...... I.15

§ 3. Espaces vectoriels topologiques métrisables .................. I.16
    1. Voisinages de zéro dans un espace vectoriel topologique métrisable ............................................. I.16
    2. Propriétés des espaces vectoriels métrisables ............ I.17
    3. Fonctions linéaires continues dans un espace vectoriel métrisable ............................................. I.17

Exercices du § 1 .................................................. I.22
Exercices du § 2 .................................................. I.25
Exercices du § 3 .................................................. I.28

Chapitre II. — Ensembles convexes et espaces localement convexes . II.1

§ 1. Semi-normes .................................................. II.1
    1. Définition des semi-normes ................................. II.1
    2. Topologies définies par des semi-normes .................. II.2
    3. Semi-normes dans les espaces quotients et les espaces produits II.4

4. Critères d’équicontinuité des applications multilinéaires pour les topologies définies par des semi-normes ................. II.6

§ 2. Ensembles convexes ............................................. II.7
    1. Définition d’un ensemble convexe ............................ II.7
    2. Intersections d’ensembles convexes. Produits d’ensembles convexes .................................................. II.9
    3. Enveloppe convexe d’un ensemble ............................. II.10
    4. Cônes convexes .................................................. II.11
    5. Espaces vectoriels ordonnés ................................. II.13
    6. Ensembles convexes dans les espaces vectoriels topologiques . II.14
    7. Topologies sur les espaces vectoriels ordonnés ............... II.17
    8. Fonctions convexes ............................................. II.17
    9. Opérations sur les fonctions convexes ....................... II.19
   10. Fonctions convexes dans un ensemble convexe ouvert ........ II.20
   11. Semi-normes et ensembles convexes .......................... II.21

§ 3. Le théorème de Hahn-Banach (forme analytique) ............... II.22
    1. Prolongement des formes linéaires positives ............... II.22
    2. Le théorème de Hahn-Banach (forme analytique) ............. II.24

§ 4. Espaces localement convexes .................................. II.25
    1. Définition d’un espace localement convexe .................. II.25
    2. Exemples d’espaces localement convexes .................... II.27
    3. Topologies localement convexes initiales ................... II.29
    4. Topologies localement convexes finales ...................... II.29
    5. Somme directe topologique d’une famille d’espaces localement convexes ............................................. II.32
    6. Limites inductives de suites d’espaces localement convexes .. II.34
    7. Relèvements dans les espaces de Fréchet .................... II.37

§ 5. Séparation des ensembles convexes ............................ II.39
    1. Le théorème de Hahn-Banach (forme géométrique) .......... II.39
    2. Séparation des ensembles convexes dans un espace vectoriel topologique ............................................... II.39
    3. Séparation des ensembles convexes dans un espace localement convexe ............................................... II.41
    4. Approximation des fonctions convexes ....................... II.42

§ 6. Topologies faibles ........................................... II.43
    1. Espaces vectoriels en dualité ............................... II.43
    2. Topologies faibles ........................................... II.45
    3. Ensembles polaires et sous-espaces orthogonaux ............ II.47
    4. Transposée d’une application linéaire continue ............. II.49

5. Sous-espaces et espaces quotients d’un espace faible ............ II.51
6. Produits de topologies faibles ............................................. II.53
7. Espaces faiblement complets ................................................. II.54
8. Cônes convexes complets dans les espaces faibles .................. II.56

§ 7. Points extrémaux et génératrices extrémales ......................... II.57
    1. Points extrémaux des ensembles convexes compacts ............... II.57
    2. Génératrices extrémales des cônes convexes ..................... II.60
    3. Cônes convexes à semelle compacte ................................. II.63

§ 8. Espaces localement convexes complexes ............................... II.64
    1. Espaces vectoriels topologiques sur C ............................. II.64
    2. Espaces localement convexes complexes ............................ II.65
    3. Le théorème de Hahn-Banach et ses applications ................. II.67
    4. Topologies faibles sur les espaces vectoriels complexes ...... II.68

Exercices du § 2 ............................................................. II.69
Exercices du § 3 ............................................................. II.76
Exercices du § 4 ............................................................. II.78
Exercices du § 5 ............................................................. II.81
Exercices du § 6 ............................................................. II.87
Exercices du § 7 ............................................................. II.92
Exercices du § 8 ............................................................. II.100

CHAPITRE III. — ESPACES D’APPLICATIONS LINÉAIRES CONTINUES .......... III.1

§ 1. Bornologie dans un espace vectoriel topologique ................. III.1
    1. Bornologies .......................................................... III.1
    2. Parties bornées d’un espace vectoriel topologique ............. III.2
    3. Image par une application continue ............................... III.4
    4. Parties bornées dans certaines limites inductives .............. III.5
    5. Les espaces E_A (A borné) .......................................... III.7
    6. Ensembles bornés complets et espaces quasi-complets .......... III.8
    7. Exemples ............................................................ III.9

§ 2. Espaces bornologiques .................................................. III.11

§ 3. Espaces d’applications linéaires continues ........................ III.13
    1. Les espaces L_S (E ; F) ............................................. III.13
    2. Condition pour que L_S (E ; F) soit séparé ..................... III.15
    3. Relation entre L (E ; F) et L (Ê ; F) ............................ III.16
    4. Parties équicontinues de L (E ; F) ................................. III.16
    5. Parties équicontinues de E' ....................................... III.19
    6. Le complété d’un espace localement convexe .................... III.20
    7. S-bornologies sur L (E ; F) ....................................... III.22
    8. Parties complètes de L_S (E ; F) .................................. III.22

§ 4. Le théorème de Banach-Steinhaus ........................................ III.24
    1. Tonneaux et espaces tonnelés ........................................ III.24
    2. Le théorème de Banach-Steinhaus .................................... III.25
    3. Parties bornées de $\mathcal{L}(E ; F)$ (cas quasi-complet) ........ III.27

§ 5. Applications bilinéaires hypocontinues ................................. III.28
    1. Applications bilinéaires séparément continues ..................... III.28
    2. Applications bilinéaires séparément continues sur un produit d’espaces de Fréchet .................................................. III.30
    3. Applications bilinéaires hypocontinues ............................. III.31
    4. Prolongement d’une application bilinéaire hypocontinue .......... III.32
    5. Hypocontinuité de l’application $(u, v) \mapsto v \circ u$ .......... III.33

§ 6. Le théorème du graphe borélien .......................................... III.34
    1. Le théorème du graphe borélien ....................................... III.34
    2. Espaces localement convexes lusiniens ............................... III.35
    3. Applications linéaires mesurables sur un espace de Banach .. III.36

Exercices du § 1 ............................................................................. III.38
Exercices du § 2 ............................................................................. III.41
Exercices du § 3 ............................................................................. III.42
Exercices du § 4 ............................................................................. III.44
Exercices du § 5 ............................................................................. III.48
Exercices du § 6 ............................................................................. III.50

CHAPITRE IV. — LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES IV.1

§ 1. Dualité .................................................................................. IV.1
    1. Topologies compatibles avec une dualité ............................... IV.1
    2. Topologie de Mackey et topologie affaiblie sur un espace localement convexe ......................................................... IV.4
    3. Transposée d’une application linéaire continue ..................... IV.6
    4. Dual d’un espace quotient et d’un sous-espace ..................... IV.8
    5. Dual d’une somme directe, d’un produit .............................. IV.11

§ 2. Bidual. Espaces réflexifs ..................................................... IV.14
    1. Bidual .................................................................................. IV.14
    2. Espaces semi-réflexifs ....................................................... IV.15
    3. Espaces réflexifs ............................................................... IV.16
    4. Cas des espaces normés ..................................................... IV.16
    5. Espaces de Montel ............................................................. IV.18

§ 3. Dual d’un espace de Fréchet .................................................. IV.20
    1. Espaces semi-tonnelés ....................................................... IV.20
    2. Dual d’un espace localement convexe métrisable ................. IV.21
    3. Bidual d’un espace localement convexe métrisable ............... IV.22

4. Dual d’un espace de Fréchet réflexif ......................... IV.23
5. La topologie de la convergence compacte sur le dual d’un espace de Fréchet ............................................. IV.24
6. Applications bilinéaires séparément continues ............... IV.25

§ 4. Morphismes stricts d’espaces de Fréchet .................... IV.26
    1. Caractérisations des morphismes stricts .................. IV.26
    2. Morphismes stricts d’espaces de Fréchet ................. IV.28
    3. Critères de surjectivité .................................. IV.30

§ 5. Critères de compacité ........................................ IV.32
    1. Remarques générales ...................................... IV.32
    2. Compacité simple des ensembles de fonctions continues .... IV.33
    3. Les théorèmes d’Eberlein et de Šmulian .................. IV.35
    4. Cas des espaces de fonctions continues bornées .......... IV.36
    5. Enveloppe convexe d’un ensemble faiblement compact ...... IV.37

Appendice. Points fixes des groupes de transformations affines ..... IV.39
    1. Cas des groupes résolubles ............................... IV.39
    2. Moyennes invariantes ...................................... IV.40
    3. Le théorème de Ryll-Nardzewski .......................... IV.41
    4. Applications ............................................... IV.44

Exercices du § 1 .................................................. IV.47
Exercices du § 2 .................................................. IV.52
Exercices du § 3 .................................................. IV.58
Exercices du § 4 .................................................. IV.62
Exercices du § 5 .................................................. IV.67
Exercices de l’Appendice .......................................... IV.72
Tableau des principaux types d’espaces localement convexes ........ IV.75
Tableau des principales bornologies sur le dual d’un espace localement convexe E ............................................. IV.76

CHAPITRE V. — ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE) ............ V.1

§ 1. Espaces préhilbertiens et espaces hilbertiens ................. V.1
    1. Formes hermitiennes ....................................... V.1
    2. Formes hermitiennes positives ............................ V.2
    3. Espaces préhilbertiens .................................... V.4
    4. Espaces hilbertiens ....................................... V.6
    5. Sous-ensembles convexes d’un espace préhilbertien ........ V.9
    6. Sous-espaces vectoriels et orthoprojecteurs ............... V.12
    7. Dual d’un espace hilbertien .............................. V.15

§ 2. Familles orthogonales dans un espace hilbertien ............... V.17
    1. Somme hilbertienne externe d’espaces hilbertiens ........ V.17

2. Somme hilbertienne de sous-espaces orthogonaux d’un espace hilbertien .................................................. V.18
3. Familles orthonormales ............................................. V.21
4. Orthonormalisation .................................................. V.23

§ 3. Produit tensoriel d’espaces hilbertiens ......................... V.25
    1. Produit tensoriel d’espaces préhilbertiens .................... V.25
    2. Produit tensoriel hilbertien d’espaces hilbertiens ............ V.28
    3. Puissances symétriques hilbertiennes .......................... V.29
    4. Puissances extérieures hilbertiennes .......................... V.33
    5. Multiplication extérieure ....................................... V.35

§ 4. Quelques classes d’opérateurs dans les espaces hilbertiens ...... V.37
    1. Adjoint .......................................................... V.37
    2. Applications linéaires partiellement isométriques .............. V.41
    3. Endomorphismes normaux ......................................... V.42
    4. Endomorphismes hermitiens ...................................... V.43
    5. Endomorphismes positifs ......................................... V.45
    6. Trace d’un endomorphisme ....................................... V.47
    7. Applications de Hilbert-Schmidt ................................. V.51
    8. Diagonalisation des applications de Hilbert-Schmidt .......... V.54
    9. Trace d’une forme quadratique par rapport à une autre ...... V.56

Exercices du § 1 ..................................................... V.59
Exercices du § 2 ..................................................... V.69
Exercices du § 3 ..................................................... V.72
Exercices du § 4 ..................................................... V.73
Note historique ..................................................... V.79
Bibliographie ........................................................ V.91
Index des notations .................................................. 350
Index terminologique ................................................ 352
Résumé de quelques propriétés importantes des espaces de Banach ..... 359
Table des matières .................................................. 363
