---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: int-ix-fr
pdf_pages: 0111-0131
extraction: ocr
statements: 0
exercises: 0
content_sha256: 7ddf36d54aaa79b3e139a5b576f29f9f98172a65f3e65d2b9ac9671efae2745e
---

# NOTE HISTORIQUE

(N.B. Les chiffres romains renvoient à la bibliographie située à la fin de cette note.)

Si l’étude des liens entre la topologie et la théorie de la mesure remonte aux débuts de la théorie moderne des fonctions de variables réelles, ce n’est que fort récemment que l’intégration dans les espaces topologiques séparés a été mise au point de manière générale. Avant de faire l’historique des travaux qui ont précédé la synthèse actuelle, nous rappellerons quelques étapes de l’évolution des idées concernant les relations entre topologie et mesure.

Pour Lebesgue, il n’est question que d’intégrer des fonctions d’une ou plusieurs variables réelles. En 1913, Radon définit les mesures générales sur $\mathbf{R}^n$ et les intégrales correspondantes ; cette théorie est exposée en détail dans l’ouvrage (I) de Ch. de la Vallée Poussin et s’appuie de manière constante sur les propriétés topologiques des espaces euclidiens. Un peu plus tard, en 1915, Fréchet définit dans (II, a)) les mesures « abstraites » sur un ensemble muni d’une tribu et les intégrales par rapport à ces mesures ; il note qu’on peut établir ainsi les principaux résultats de la théorie de Lebesgue sans utiliser de moyens topologiques. Il justifie son entreprise par les mots suivants, tirés de l’introduction de (II, b), première partie) : « Que par exemple dans l’espace à une infinité de coordonnées où diverses applications de l’Analyse avaient conduit à diverses définitions non équivalentes d’une suite convergente, on remplace une de ces définitions par une autre, rien ne sera changé dans les propriétés des familles et fonctions additives d’ensembles dans ces espaces ». Les recherches de Fréchet sont complétées par Carathéodory, à qui l’on doit un important théorème de prolongement d’une fonction d’ensemble en une mesure. Le début du livre de Saks (III) offre un exposé condensé de ce point de vue.

La découverte de la mesure de Haar sur les groupes localement compacts (cf. Note historique des chap. VII et VIII) et les nombreuses applications qu’elle reçoit aussitôt, puis les travaux de Weil et Gelfand en Analyse Harmonique, amènent vers 1940 à une modification profonde de ce point de vue : dans ce genre de questions, le plus commode est de considérer une mesure comme une forme linéaire sur un espace de fonctions continues. Cette méthode oblige à se restreindre aux espaces compacts ou localement compacts, mais ce n’est pas une gêne pour la presque totalité des applications; bien mieux, l’introduction de l’Analyse Harmonique sur les groupes $p$-adiques et les groupes d’adèles par J. Tate et A. Weil a permis un renouvellement spectaculaire de la Théorie analytique des Nombres.

C’est d’une tout autre direction que provient la nécessité d’élargir ce point de vue par la considération de mesures sur des espaces topologiques non localement compacts: peu à peu, le Calcul des Probabilités amène à l’étude de tels espaces et fournit de nombreux exemples non triviaux. Peut-être faut-il rechercher la raison de l’influence tardive de ces développements sur la théorie de la mesure dans l’isolement relatif du Calcul des Probabilités, resté en marge des disciplines mathématiques traditionnelles jusqu’à une époque récente.

Mesures sur les espaces de suites

Une des branches les plus développées du Calcul des Probabilités classique est celle des théorèmes limites (loi des grands nombres, tendance vers la loi de Gauss-Laplace, ...); il s’agit d’un approfondissement de la notion de régularité statistique manifestée par les phénomènes mettant en jeu des populations très nombreuses. La formulation mathématique correcte de ces problèmes nécessite l’introduction de mesures sur des espaces de suites; ces espaces, qui constituent la généralisation la plus évidente des espaces de dimension finie, sont le sujet de prédilection des recherches d’« Analyse Générale » entreprises vers 1920 par Fréchet, Lévy, Lusin, ... Il n’est d’ailleurs pas fortuit que Khintchine et Kolmogoroff, les créateurs des méthodes nouvelles du Calcul des Probabilités, soient tous deux disciples de Lusin, et que Lévy se soit très vite tourné vers les problèmes probabilistes: ceux-ci constituaient la pierre de touche des nouvelles méthodes.

La première intervention implicite d’une mesure sur un espace de suites apparaît dans le travail consacré par E. Borel en 1909 aux probabilités dénombrables (IV). Une idée très originale de Borel consiste en l’application des résultats probabilistes qu’il vient d’obtenir à la démonstration de propriétés possédées par le développement décimal de presque tout nombre réel compris entre 0 et 1. Cette application repose sur la remarque fondamentale suivante: définissons tout nombre réel compris entre 0 et 1 par la suite des chiffres de son développement dans une base $q$ donnée ($q \geqslant 2$); si l’on tire au sort successivement les divers chiffres d’un nombre $x$, indépendamment les uns des autres et avec une égale probabilité $1/q$ pour $0, 1, \ldots, q - 1$, la probabilité que $x$ se trouve dans un intervalle de $(0, 1[$ est égale à la longueur de cet intervalle.

En 1923, Steinhaus (V) établit rigoureusement ces résultats et décrit le modèle mathématique précis de la suite illimitée de tirages au sort considérée par Borel: prenons $q = 2$ pour simplifier et notons I l’ensemble à deux éléments $\{0, 1\}$; on munit I de la mesure $\mu$ définie par $\mu(0) = \mu(1) = \frac{1}{2}$; les éléments de l’espace produit $I^\mathbf{N}$ sont les suites $\varepsilon = (\varepsilon(n))_{n \in \mathbf{N}}$ de nombres égaux à 0 ou 1 et l’application $\varphi : \varepsilon \mapsto \sum_{n \geq 0} \varepsilon(n) \cdot 2^{-n-1}$ est, à un ensemble dénombrable près, une bijection de $I^\mathbf{N}$ sur l’intervalle $(0, 1)$; de plus, $\varphi^{-1}$ transforme la mesure de Lebesgue sur $(0, 1)$ en la mesure P sur $I^\mathbf{N}$ produit des mesures $\mu$ sur chacun des facteurs. En fait, Steinhaus ne dispose pas d’une construction des mesures produits ; il utilise l’existence de la quasi-bijection $\varphi$ pour construire la mesure P sur $I^\mathbf{N}$ à partir de la mesure de Lebesgue sur $(0, 1)$, puis il donne une caractérisation axiomatique de P. L’isomorphisme ainsi obtenu permet de traduire le langage des probabilités en celui de la mesure et d’appliquer les théorèmes connus sur l’intégrale de Lebesgue.

Dans le même travail, Steinhaus considère la série aléatoire $\sum_{n \geq 0} \sigma_n \cdot a_n$, où les signes $\sigma_n = \pm 1$ sont choisis au hasard indépendamment les uns des autres et avec même probabilité $\frac{1}{2}$; entre 1928 et 1935, il étudie de nombreuses autres séries aléatoires. De leur côté, Paley, Wiener et Zygmund considèrent les séries de Fourier aléatoires (1) de la forme $\sum_{n = -\infty}^{\infty} a_n \exp (2\pi i (nt + \Phi_n))$; les « amplitudes » $a_n$ sont fixes, et les « phases » $\Phi_n$ sont des variables aléatoires indépendantes uniformément réparties sur $(0, 1)$. Si les difficultés analytiques varient énormément de l’un à l’autre de ces problèmes, la traduction en termes de théorie de la mesure est la même dans tous les cas et représente une extension du cas traité par Borel et Steinhaus ; il s’agit de construire une mesure sur $\mathbf{R}^\mathbf{N}$, produit d’une famille de mesures toutes identiques à une même mesure positive $\mu$ de masse 1 sur $\mathbf{R}$; par exemple, les séries de Fourier aléatoires précédentes correspondent au cas où $\mu$ est la mesure de Lebesgue sur $(0, 1)$.

Pour construire de telles mesures produits, on peut utiliser deux méthodes. La première est une méthode directe, mise au point pour la première fois par Daniell (VI, a)) en 1918 ; elle est retrouvée en 1934 par Jessen (VII) qui fera une étude détaillée du cas où $\mu$ est la mesure de Lebesgue sur $(0, 1)$. La deuxième méthode est la recherche d’artifices analogues à celui de Steinhaus pour se ramener à la mesure de Lebesgue sur $(0, 1)$; cette façon de procéder avait l’avantage de la commodité tant qu’on ne disposait pas d’exposé complet de la théorie de la mesure générale, car elle permettait d’employer sans nouvelle démonstration les théorèmes de Lebesgue (2).

1. Pour une mise au point sur les séries de Fourier aléatoires, voir l’exposé de J.-P. KAHANE au Séminaire Bourbaki (n° 200, 12e année, 1959/60, Benjamin, New-York).
2. Wiener prend aussi soin à de nombreuses reprises (cf. par exemple (XI), chap. IX) de montrer que la mesure du mouvement brownien est isomorphe à la mesure de Lebesgue sur $(0, 1)$. La possibilité de tels artifices trouve son explication dans un théorème général de von Neumann qui donne une caractérisation axiomatique des mesures isomorphes à la mesure de Lebesgue sur $(0, 1)$.

La théorie du mouvement brownien

Cette théorie occupe une place exceptionnelle dans le développement scientifique contemporain par l’échange constant et fécond dont elle témoigne entre les problèmes physiques et les mathématiques « pures ». L’étude du mouvement brownien, découvert en 1829 par le botaniste Brown, a été menée intensivement au 19e siècle par de nombreux physiciens (3), mais le premier modèle mathématique satisfaisant a été inventé par Einstein en 1905 seulement. Dans le cas simple d’une particule se déplaçant le long d’une droite, les hypothèses fondamentales d’Einstein se formulent ainsi : si $x(t)$ est l’abscisse de la particule à l’instant $t$, et si $t_0 < t_1 < \cdots < t_{n-1} < t_n$, les déplacements successifs $x(t_i) - x(t_{i-1})$ (pour $1 \leq i \leq n$) sont des variables aléatoires gaussiennes indépendantes. Ce n’est pas le lieu d’évoquer ici en détail les importants travaux expérimentaux de J. Perrin que motiva la théorie d’Einstein ; pour notre propos, il convient de retenir seulement une remarque de Perrin, selon laquelle l’observation des trajectoires du mouvement brownien lui suggère irrésistiblement « les fonctions sans dérivée de mathématiciens ». Cette remarque sera l’étincelle initiale pour Wiener.

Un tout autre courant d’idées tire son origine de la théorie cinétique des gaz, développée entre 1870 et 1900 par Boltzmann et Gibbs. Considérons un gaz formé de N molécules de masse $m$ à la température (absolue) $T$ et notons $\mathbf{v}_1, \ldots, \mathbf{v}_N$ les vitesses des N molécules du gaz ; l’énergie cinétique du système est égale à

$$
\frac{m}{2} (\mathbf{v}_1^2 + \cdots + \mathbf{v}_N^2) = 3NkT
$$

où $k$ est la constante de Boltzmann. D’après les idées de Gibbs, la multitude des chocs entre molécules ne permet pas de déterminer avec précision les vitesses des molécules, et il convient d’introduire une loi de probabilité $P$ sur la sphère $S$ de l’espace de dimension $3N$ définie par l’équation (1). L’hypothèse « micro-canonique » consiste à supposer que $P$ est la mesure de masse 1 invariante par rotation sur la sphère $S$. Par ailleurs, la loi des vitesses de Maxwell énonce que la loi de probabilité d’une composante de la vitesse d’une molécule est une mesure gaussienne de variance $2kT/m$ ($§ 6,$ no 5, Remarque 3). Borel semble avoir été le premier à remarquer en 1914 que la loi de Maxwell est conséquence des hypothèses de Gibbs et de propriétés de la sphère lorsque le nombre des molécules est très grand. Il considère une sphère $S$ dans un espace euclidien de grande dimension et la mesure $P$ de masse 1 invariante par rotation sur $S$ ; utilisant les méthodes classiques d’approximation fondées sur la formule de Stirling, il montre que la projection de $P$ sur un axe de coordonnées est approximativement gaus-

3. On trouvera un exposé très vivant de cette histoire dans l’ouvrage récent de E. Nelson, Dynamical theories of brownian motion, Mathematical Notes, Princeton, 1967.

sienne. Ces résultats sont précisés un peu plus tard par Gâteaux et Lévy (IX, a)). Etant donnés un entier $m \geqslant 1$ et un nombre $r > 0$, notons $S_{m,r}$ l’ensemble des suites de la forme $(x_1, \ldots, x_m, 0, 0, \ldots)$ avec $x_1^2 + \cdots + x_m^2 = r^2$; notons aussi $\sigma_{m,r}$ la mesure de masse 1 invariante par rotation sur $S_{m,r}$. Enoncé en langage moderne, le résultat de Gâteaux et Lévy est le suivant: la suite des mesures $\sigma_{m,1}$ tend étroitement vers la masse unité à l’origine $(0, 0, \ldots)$ et la suite des mesures $\sigma_{m,\sqrt{m}}$ tend étroitement vers une mesure $\Gamma$ de la forme

$$
d\Gamma(x_1, x_2, \ldots) = \prod_{n=1}^{\infty} d\gamma(x_n)
$$

($\gamma$ est la mesure gaussienne de variance 1 sur $\mathbf{R}$).

La mesure $\Gamma$ précédente joue le rôle d’une mesure gaussienne en dimension infinie. Il semble bien que Lévy ait confusément espéré définir de manière intrinsèque une mesure gaussienne sur tout espace de Hilbert de dimension infinie. De fait, comme l’ont montré Lévy et Wiener, la mesure $\Gamma$ est invariante en un certain sens (4) par les automorphismes de $l^2$; malheureusement, l’ensemble $l^2$ des suites $(x_1, x_2, \ldots, x_n, \ldots)$ de carré sommable est de mesure nulle pour $\Gamma$. On sait aujourd’hui qu’il faut se contenter d’une promesure gaussienne sur un espace de Hilbert de dimension infinie (5).

On doit à Wiener le progrès essentiel: si l’on n’a pas de mesure de Gauss raisonnable sur un espace de Hilbert de dimension infinie, on peut construire par l’opération de primitive une mesure $w$ sur un espace de fonctions continues à partir d’une promesure gaussienne (cf. § 6, n° 7, th. 1 pour les détails). Nous allons expliquer succinctement la construction initiale de $w$ par Wiener (X); elle est directement influencée par la relation $\Gamma = \lim_{m \to \infty} \sigma_{m, \sqrt{m}}$ de Gâteaux et Lévy.

Pour tout entier $m \geqslant 1$, notons $H_m$ l’ensemble des fonctions sur $T = ]0, 1]$ qui sont constantes dans chacun des intervalles $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$ (pour $k = 1, 2, \ldots, m$), et $\pi_m$ la mesure de masse 1 invariante par rotation sur la sphère euclidienne de rayon 1 dans $\mathbf{R}^m$. Soit $f_m$ l’isomorphisme de $H_m$ sur $\mathbf{R}^m$ qui associe à toute fonction prenant la valeur $a_k$ sur l’intervalle $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$ le vecteur $(a_1, a_2 - a_1, \ldots, a_m - a_{m-1})$ (d’où le nom de « differential space » affectionné par Wiener); notons $w_m$ la mesure sur $H_m$ image de $\pi_m$ par $f_m^{-1}$. Wiener définit la mesure

4. De manière précise, on a le résultat suivant. Soient $U$ un automorphisme de l’espace de Hilbert $l^2$ et $(u_{mn})$ la matrice de $U$. Soient E l’espace vectoriel de toutes les suites réelles $(x_n)_{n \geqslant 1}$ et F le sous-espace de E formé des suites $(x_n)_{n \geqslant 1}$ pour lesquelles les séries $\sum_{n \geqslant 1} u_{mn} x_n$ convergent pour tout $m \geqslant 1$.
La formule $(\tilde{U}x)_m = \sum_{n \geqslant 1} u_{mn} x_n$ définit une application linéaire $\tilde{U}$ de F dans E, la mesure $\Gamma$ est concentrée sur F et l’on a $\tilde{U}(\Gamma) = \Gamma$.
5. Cette notion a été introduite sous le nom de « weak canonical distribution » par I. Segal (Trans. Amer. Math. Soc., t. 88 (1958), p. 12–42). On doit à cet auteur une étude détaillée des promesures gaussiennes, et leur application à certains problèmes de théorie quantique des champs.

cherchée $w$ comme la limite des mesures $w_m$. De manière précise, notons $H$ l’ensemble des fonctions réglées sur $T$, avec la topologie de la convergence uniforme (on a $H_m \subset H$ pour tout entier $m \geqslant 1$) ; pour toute fonction uniformément continue et bornée $F$ sur $H$, la limite $A\{F\} = \lim_{m \to \infty} \int_{H_m} F(x)\ dw_m(x)$ existe ; Wiener obtient ensuite certaines majorations par une analyse subtile des fluctuations du jeu de pile ou face, et reprenant les arguments de compacité mis en évidence par Daniell, il montre que l’on est dans les conditions d’application du théorème de prolongement de Daniell. On conclut à l’existence d’une mesure $w$ portée par $C(T)$ et telle que $A\{F\} = \int_{C(T)} F(x)\ dw(x)$. Wiener peut alors montrer que la mesure $w$ correspond aux hypothèses d’Einstein (6), et ses estimations lui permettent de donner un sens précis à la remarque de Perrin sur les fonctions sans dérivées : l’ensemble des fonctions satisfaisant à une condition de Lipschitz d’ordre $\frac{1}{2}$ est négligeable pour $w$ (par contre, pour tout $a$ avec $0 < a < \frac{1}{2}$, presque toute fonction satisfait à une condition de Lipschitz d’ordre $a$).

On connaît aujourd’hui de nombreuses constructions de la mesure de Wiener. Ainsi, Paley et Wiener utilisent les séries de Fourier aléatoires (XI, chap. IX) : pour toute suite réelle $a = (a_n)_{n \geqslant 1}$ et tout entier $m \geqslant 0$, définissons la fonction $f_{m, a}$ sur $]0, 1]$ par
$$
f_{m, a}(t) = a_1 t + 2 \sum_{k=2}^{2m+1} \frac{1}{\pi k} a_{k-1} \sin \pi k t;
$$
on peut montrer que, pour $\Gamma$-presque toute suite $a$, la suite des fonctions $f_{m, a}$ tend vers une fonction continue $f_a$ et que $w$ est l’image de $\Gamma$ par l’application (définie presque partout) $a \mapsto f_a$. Plus tard, Lévy a donné dans (IX, b), c)) une construction très voisine de celle que nous avons exposée au § 6, n° 7. Enfin, Kac, Donsker et Erdös montrent vers 1950 comment remplacer dans la construction initiale de Wiener les mesures sphériques $\pi_m$ sur $\mathbf{R}^m$ par des mesures plus générales. Leurs résultats établissent un lien solide entre la mesure de Wiener et les théorèmes limites du Calcul des Probabilités ; ils seront complétés et systématisés par Prokhorov (XIII) dans un travail sur lequel nous reviendrons plus loin.

Ce n’est pas le lieu d’analyser les nombreux et importants travaux probabilistes occasionnés par la découverte de Wiener ; aujourd’hui, le mouvement brownien

6. Ceci se traduit par la formule
$$
\int_{C(T)} f(x(t_1), \ldots, x(t_n))\ dw(x)
= (2\pi)^{-n/2} \prod_{i=1}^n (t_i - t_{i-1})^{-1/2} \int \cdots \int f(x_1, \ldots, x_n) \exp \left( -\frac{1}{2} \sum_{i=1}^n \frac{(x_i - x_{i-1})^2}{t_i - t_{i-1}} \right) dx_1 \ldots dx_n
$$
où $f$ est une fonction continue bornée arbitraire sur $\mathbf{R}^n$ et où l’on a $0 = t_0 < t_1 < \cdots < t_n \leqslant 1$ (on fait la convention $x_0 = 0$). Wiener, formé à la rigueur analytique par Hardy, et défiant à juste titre à l’égard des fondements du Calcul des Probabilités à cette époque, prend soin de n’utiliser ni la terminologie ni les résultats probabilistes. Il en résulte que ses mémoires sont pleins de formidables formules dont la précédente est un échantillon ; cette particularité est un des facteurs qui ont retardé la diffusion des idées de Wiener.

n’apparaît plus que comme un des exemples les plus importants de processus markovien. Nous mentionnerons seulement l’application faite par Kac de la mesure de Wiener à la résolution de certaines équations aux dérivées partielles paraboliques; il s’agit là d’une adaptation des idées de Feynman en théorie quantique des champs — un exemple de plus de cette influence réciproque des mathématiques et des problèmes de physique.

Limites projectives de mesures

Il s’agit d’une théorie qui s’est développée surtout en fonction des besoins du Calcul des Probabilités. Les problèmes concernant une suite finie de variables aléatoires $X_1, \ldots, X_n$ sont résolus en principe lorsqu’on connaît la loi $P_X$ de cette suite: c’est une mesure positive de masse 1 sur $\mathbf{R}^n$, telle que la probabilité d’obtenir simultanément les inégalités $a_1 \leq X_1 \leq b_1, \ldots, a_n \leq X_n \leq b_n$ soit égale à $P_X(C)$ où $C$ est le pavé fermé $[a_1, b_1] \times \cdots \times [a_n, b_n]$ de $\mathbf{R}^n$. En pratique, la mesure $P_X$ a un support discret ou bien admet une densité par rapport à la mesure de Lebesgue. Lorsqu’on a affaire à une suite infinie $(X_n)_{n \geq 1}$ de variables aléatoires, on connaît en général la loi $P_n$ de la suite partielle $(X_1, \ldots, X_n)$ pour tout entier $n \geq 1$; ces données satisfont à une condition de compatibilité qui exprime que la suite $(P_n)_{n \geq 1}$ est un système projectif de mesures. Jusque vers 1920, on définissait de manière plus ou moins implicite les probabilités d’événements liés à la suite infinie par des passages à la limite « naturels » à partir de probabilités du cas fini; on admettra ainsi que la probabilité qu’un jeu se termine est la limite, pour $n$ tendant vers l’infini, de la probabilité qu’il se termine en au plus $n$ parties. Naturellement, une telle théorie est assez peu cohérente, et rien n’exclut la présence de « paradoxes », une même probabilité recevant deux estimations distinctes selon qu’on l’évalue par l’un ou l’autre de deux procédés aussi « naturels » l’un que l’autre.

Steinhaus (V) semble avoir été le premier à ressentir la nécessité de considérer (pour le jeu de pile ou face) non seulement le système projectif $(P_n)_{n \geq 1}$ mais sa limite. Un peu auparavant, en 1919, Daniell (VI, b)) avait démontré en général l’existence de telles limites projectives (7), mais ce résultat semble être resté inconnu en Europe. Il est retrouvé en 1933 par Kolmogoroff dans l’ouvrage (XII) où cet auteur formule la conception axiomatique du Calcul des Probabilités. Les démonstrations de Daniell et Kolmogoroff utilisent un argument de compacité, qui est à peu de choses près celui que nous avons employé au th. 2 du § 4, n° 3 et repose sur le th. de Dini.

7. Daniell traite le cas des mesures sur un produit $\prod_{n \geq 1} I_n$ d’intervalles compacts de $\mathbf{R}$, mais sa méthode s’étend immédiatement au cas d’un produit quelconque d’espaces compacts; c’est au fond celle que nous avons utilisée au chap. III, § 4, n° 5.

Le théorème de Daniell–Kolmogoroff ne laissait rien à désirer pour le cas des suites aléatoires $(X_n)_{n \geq 1}$, mais l’étude des fonctions aléatoires entreprise à partir de 1935 par Kolmogoroff, Feller et Doob recèle des difficultés d’une tout autre ampleur. Considérons par exemple un intervalle $T$ de $\mathbf{R}$, qui représente l’ensemble des instants d’observation d’un « processus stochastique »; l’ensemble des trajectoires possibles est l’espace produit $\mathbf{R}^T$, considéré comme limite projective des produits partiels $\mathbf{R}^H$, où $H$ parcourt l’ensemble des parties finies de $T$; on se donne en général un système projectif de mesures $(\mu_H)$ (cf. § 4, n° 3). Le théorème de Kolmogoroff fournit bien une mesure sur $\mathbf{R}^T$, mais elle est définie sur une tribu notablement plus petite que la tribu borélienne (8). Une variante de la construction de Kolmogoroff, qui fournit une mesure sur un espace topologique, est due à Kakutani (*Proc. Imp. Acad. Tokyo, XIX* (1943), p. 184–188), et a été redécouverte plusieurs fois depuis: on considère $\mu_H$ comme une mesure sur $\overline{\mathbf{R}}^H$ portée par $\mathbf{R}^H$ (9); l’espace compact $E = \overline{\mathbf{R}}^T$ est limite projective des produits finis $\overline{\mathbf{R}}^H$ et l’on peut définir une mesure $\mu$ sur $E$ limite projective des $\mu_H$ (cf. chap. III, § 4, n° 5). Mais ce procédé possède un grave inconvénient; les éléments de $\overline{\mathbf{R}}^T$ ne possèdent aucune propriété de régularité permettant de pousser plus loin l’étude probabiliste du processus — ou même simplement d’éliminer les valeurs parasites $±\infty$ introduites par la compactification $\overline{\mathbf{R}}$ de $\mathbf{R}$. On peut y remédier en induisant la mesure $\mu$ de $\overline{\mathbf{R}}^T$ sur tel ou tel sous-espace (par exemple $\mathcal{C}(T)$ dans le cas du mouvement brownien); la difficulté fondamentale provient de ce qu’un espace fonctionnel, même d’un type usuel, n’est pas nécessairement $\mu$-mesurable dans $\overline{\mathbf{R}}^T$, et le choix même de l’espace fonctionnel peut faire question (10).

Un pas décisif a été accompli en 1956 par Prokhorov dans un travail (XIII) qui a exercé une influence déterminante sur la théorie des processus stochastiques. En mettant sous forme axiomatique convenable les méthodes utilisées par Wiener dans l’article analysé plus haut, il établit un théorème général d’existence de limites projectives de mesures sur les espaces fonctionnels qui est le cas particulier du th. 1 du § 4, n° 2 correspondant aux espaces polonais.

Une classe plus restreinte de systèmes projectifs a été introduite par Bochner (XIV) en 1947; il s’agit des systèmes projectifs formés d’espaces vectoriels réels de dimension finie et d’applications linéaires surjectives. La limite projective d’un tel système s’identifie de manière naturelle au dual algébrique $E^*$ d’un espace vectoriel réel $E$ muni de la topologie faible $\sigma(E^*, E)$; un système projectif

8. La mesure de Kolmogoroff n’est définie que pour les ensembles boréliens dans $\mathbf{R}^T$ de la forme $A \times \mathbf{R}^{T-D}$ où $D$ est une partie dénombrable de $T$, et $A$ une partie borélienne de $\mathbf{R}^D$; de ce fait, le théorème de Kolmogoroff pour un produit quelconque $\mathbf{R}^T$ est une conséquence immédiate du cas des produits dénombrables.
9. On pourrait remplacer $\overline{\mathbf{R}}$ par n’importe quel espace compact contenant $\mathbf{R}$ comme sous-espace dense.
10. Pour une discussion détaillée du problème de la construction des mesures sur les espaces fonctionnels, et les méthodes utilisées avant Prokhorov, voir J. L. Doob, *Bull. Amer. Math. Soc.*, 53 (1947), p. 15–30.

correspondant de mesures à une limite qui est une mesure $\mu$ définie sur une tribu notablement plus petite que la tribu borélienne de $E^*$. Bochner caractérisa complètement de telles « promesures » par leur transformée de Fourier, qui est une fonction sur $E$. Mais ce résultat n’est guère utilisable en l’absence d’une topologie sur $E$, auquel cas il faut examiner la possibilité de considérer $\mu$ comme une mesure sur le dual topologique $E'$ de $E$. De manière indépendante, R. Fortet et E. Mourier, en cherchant à généraliser aux variables aléatoires à valeurs dans un espace de Banach certains résultats classiques du Calcul des Probabilités (loi des grands nombres, théorème central limite) mirent aussi en évidence le rôle fondamental joué par la transformation de Fourier dans ces questions. Mais un progrès substantiel ne fut réalisé qu’en 1956 lorsque Gelfand (XV, b)) suggéra que le cadre naturel pour la transformation de Fourier n’est pas celui des espaces de Banach ou de Hilbert, mais celui des espaces de Fréchet nucléaires. Il conjectura que toute fonction continue de type positif sur un tel espace est la transformée de Fourier d’une mesure sur son dual, résultat établi tôt après par Minlos (XVI). Son importance provient surtout de ce qu’il s’applique aux espaces de distributions, et que la quasi-totalité des espaces fonctionnels sont des parties boréliennes de l’espace des distributions (qui constitue donc un bien meilleur réceptacle que $\mathbf{R}^T$) (11). La théorie des distributions aléatoires est un domaine en pleine expansion, et nous nous contenterons de renvoyer le lecteur à l’ouvrage de Gelfand et Vilenkin (XVII).

Les résultats que nous venons de mentionner sur les limites projectives utilisent l’existence de topologies sur les espaces de base. On peut se demander s’il existe une théorie analogue dans le cas des mesures « abstraites ». Von Neumann a démontré dès 1935 l’existence de mesures produits dans tous les cas, mais la découverte d’un contre-exemple par Jessen et Andersen (XVIII) a ruiné l’espoir que tout système projectif de mesures admette une limite. On a découvert deux palliatifs : en 1949, C. Ionescu-Tulcea a établi l’existence de limites projectives dénombrables, moyennant l’existence de désintégrations convenables (12), résultat fort intéressant pour l’étude des processus markoviens ; par ailleurs, on s’est rendu compte que la topologie des espaces n’intervenait que par l’intermédiaire de l’ensemble des parties compactes. Il était donc naturel de chercher à axiomatiser cette situation à l’intérieur de la théorie abstraite, au moyen de la notion de classe compacte de parties d’un ensemble. Ce travail fut fait en 1953 par Marczewski (qui établit par ce moyen un théorème de limites projectives abstrait) et Ryll–Nardzewski (qui traita de la désintégration des mesures) (13).

11. On pourra consulter la mise au point de X. Fernique, Ann. Inst. Fourier, t. XVII (1967), p. 1–92, qui contient aussi de nombreux résultats sur la convergence étroite.
12. Il semble que ce soit l’absence d’une théorie satisfaisante des désintégrations qui marque la limite de la théorie des mesures « abstraites ». Cette difficulté réapparaît de manière insistante dans le Calcul des Probabilités à propos des probabilités conditionnelles.
13. Pour un exposé de cette théorie, on pourra se reporter à J. Pfanzagl et W. Pierlo, Lecture Notes in Mathematics (Springer Verlag), vol. 16 (1966).

Mesures sur les espaces topologiques généraux et convergence étroite

L’étude des liens entre la topologie et la théorie de la mesure a été surtout conçue comme l’étude des propriétés de régularité des mesures, et en particulier celle de la régularité « extérieure » et de la régularité « intérieure » (14); la régularité intérieure est équivalente à la régularité extérieure sur un espace localement compact dénombrable à l’infini. La construction que Lebesgue donne de la mesure des ensembles sur la droite met en évidence ces deux espèces de régularité, et la propriété de régularité extérieure des mesures sur un espace polonais semble avoir été de notoriété publique vers 1935. Mais ce n’est qu’en 1940, dans un article dont la guerre retarda la diffusion, qu’A. D. Alexandroff (XIX) met en évidence le rôle de la régularité intérieure et montre que celle-ci est possédée par les mesures sur un espace polonais; ce résultat est retrouvé plus tard par Prokhorov (XIII) et est souvent attribué à tort à cet auteur. On ne s’est aperçu que fort récemment que cette propriété s’étendait aux espaces sousliniens; de ce fait, l’importance de ces espaces s’est beaucoup accrue, d’autant plus qu’on s’est rendu compte que leur théorie pouvait se faire sans hypothèse de métrisabilité, et que la quasi-totalité des espaces fonctionnels étaient sousliniens (et même le plus souvent lusiniens) (15). Ce sont ces raisons qui nous ont poussé à mettre l’accent sur les mesures intérieurement régulières dans ce chapitre.

La définition d’un mode de convergence (vague ou étroite) pour les mesures se fait de la manière la plus commode en mettant en dualité l’espace des mesures avec un espace de fonctions continues. Généralisant un résultat ancien de F. Riesz, A. A. Markoff a établi en 1938 une correspondance biunivoque entre les fonctionnelles positives sur $\mathcal{C}(X)$ et les mesures régulières sur un espace compact X. Dans le travail (XIX) déjà cité, A. D. Alexandroff étend ces résultats au cas d’un espace complètement régulier: il introduit une hiérarchie dans l’ensemble des formes linéaires positives sur l’espace $\mathcal{C}^b(X)$ des fonctions continues bornées sur un espace complètement régulier X (16), il définit la convergence

14. Une mesure « abstraite » $\mu$ sur la tribu borélienne d’un espace topologique séparé est dite extérieurement régulière si la mesure de tout ensemble borélien est la borne inférieure des mesures des ensembles ouverts qui le contiennent; la mesure $\mu$ est dite intérieurement régulière si la mesure de tout ensemble borélien est la borne supérieure des mesures de ses parties compactes.
15. Pour tenter de résoudre certaines difficultés probabilistes (particulièrement les liens entre diverses notions d’indépendance ou de dépendance stochastique), plusieurs auteurs introduisent des classes restreintes de mesures « abstraites »: espaces « parfaits » de Kolmogoroff–Gnedenko, espaces « lusiniens » de Blackwell, espaces « de Lebesgue » de Rokhlin. En fait (tout au moins moyennant une hypothèse de dénombrabilité assez faible), toutes ces définitions donnent des caractérisations des mesures « abstraites » isomorphes à une mesure positive bornée sur un espace souslinien. On pourra consulter à ce sujet l’ouvrage cité dans la note (13).
16. Il distingue par ordre de généralité décroissante les $\sigma$-mesures (mesures « abstraites » sur la tribu borélienne de X), les $\tau$-mesures (mesures extérieurement régulières) et les mesures tendues (mesures intérieurement régulières). Lorsque X est polonais, ces trois notions coïncident. La terminologie elle-même est due à Mac Shane et Le Cam (XX). On trouvera une mise au point des travaux suscités par cette classification dans V. S. Varadarajan (Amer. Math. Soc. Translations (2), vol. 48, p. 161–228).

étroite des mesures bornées et démontre entre autres les deux théorèmes suivants:

a) si X est polonais, l’ensemble des formes linéaires sur $\mathcal{C}^b(X)$ correspondant aux mesures est fermé pour la convergence faible des suites;
b) si une suite de mesures bornées a une limite étroite, « il n’y a pas de masse fuyant à l’infini » (c’est une forme faible de la réciproque du théorème de convergence étroite de Prokhorov).

De cette foison de notions et de théorèmes, Prokhorov saura extraire les résultats importants pour la théorie des processus stochastiques, et les présenter sous une forme simple et frappante. Dans son grand travail de 1956 déjà cité (XIII), une partie importante est consacrée aux mesures positives bornées sur un espace polonais; en généralisant une construction de Lévy, il définit sur l’ensemble des mesures positives de masse 1 une distance qui en fait un espace polonais, puis il établit un critère important de compacité pour la convergence étroite (cf. § 5, n° 5, th. 1). Indépendamment de Prokhorov, Le Cam (XX) a obtenu un certain nombre de résultats de compacité pour la convergence étroite des mesures; il ne fait aucune hypothèse de métrisabilité sur les espaces qu’il considère, et ses résultats se réduisent à des théorèmes antérieurs de Dieudonné dans le cas localement compact.

I. Ch. de la Vallée Poussin, Intégrales de Lebesgue, Fonctions d’ensembles, Classes de Baire, Paris (Gauthier-Villars), 1e édit. 1916, 2e édit. 1936.

II. M. Fréchet, a) Sur l’intégrale d’une fonctionnelle étendue à un ensemble abstrait, Bull. Soc. Math. de France, t. XLIII (1915), p. 248–265.
    b) Les familles et fonctions additives d’ensembles abstraits, Fund. Math., t. IV (1923), p. 329–265, et t. V (1924), p. 206–251.

III. S. Saks, Theory of the Integral, 2e édit., New York (Stechert), 1937.

IV. E. Borel, Les probabilités dénombrables et leurs applications arithmétiques, Rend. Circ. Math. Palermo, t. XXVII (1909), p. 247–271.

V. H. Steinhaus, Les probabilités dénombrables et leur rapport à la théorie de la mesure, Fund. Math., t. IV (1923), p. 286–310.

VI. P. J. Daniell: a) Integrals in an infinite number of dimensions, Ann. of Math., t. XX (1918–19), p. 281–288.
    b) Functions of limited variation in an infinite number of dimensions, Ann. of Maths., t. XXI (1919–20), p. 30–38.

VII. B. Jessen, The theory of integration in a space of an infinite number of dimensions, Acta Math., t. LXIII (1934), p. 249–323.

VIII. A. Einstein, Investigations on the Theory of the Brownian Movement, New York (Dover), 1956.

IX. P. Lévy: a) Leçons d’Analyse Fonctionnelle, Paris (Gauthier-Villars), 1922 (la deuxième édition est parue en 1951 chez le même éditeur sous le titre: Problèmes concrets d’Analyse Fonctionnelle).
    b) Processus stochastiques et mouvement brownien, Paris (Gauthier-Villars), 1948.
    c) Le mouvement brownien, Mémorial des Sciences Mathématiques, t. CXXVI (1954).

X. N. Wiener, Differential space, J. Math. Phys. MIT, t. II (1923), p. 131–174 (= Selecta, p. 55–98, Cambridge (MIT Press), 1964).

XI. R. E. A. C. Paley et N. Wiener, Fourier transforms in the complex domain, Amer. Math. Soc. Coll. Publ. n° 19, New York, 1934.

XII. A. N. Kolmogoroff, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer) 1933.

XIII. Ju. V. Prokhorov, Convergence of random processes and limit theorems in probability theory, Theor. Prob. Appl., t. I (1956), p. 156–214.

XIV. S. Bochner, Harmonic Analysis and the Theory of Probability, Berkeley (University of California Press), 1960.

XV. I. M. Gelfand: a) Processus stochastiques généralisés (en russe), Dokl. Akad. Nauk, SSSR, t. C (1955), p. 853–856.
    b) Some problems of functional analysis (en russe), Uspekhi Mat. Nauk, t. XI (1956), p. 3–12. (= AMS translations (2), vol. XVI (1960), p. 315–324).

XVI. R. A. Minlos, Generalized random processes and their extension to a measure (en russe), Trudy Mosk. Mat. Obschtsch., t. VIII (1959), p. 497–518 (= Selected translations in math. statistics and probability, III (19) p. 291–313).

XVII. I. M. GELFAND et N. Ya. VILENKIN, Generalized Functions, vol. IV, New York (Academic Press), 1964 (Traduction anglaise).

XVIII. E. SPARRE-ANDERSSON et B. JESSEN, On the introduction of measures in infinite product sets, Dansk. Vid. Selbskab. Mat. Fys. Medd., t. XXV (1948), n° 4, p. 1–7.

XIX. A. D. ALEXANDROFF, Additive set functions in abstract spaces, Mat. Sbornik, I (chap. 1), t. VIII (1940), p. 307–348; II (chap. 2 et 3), t. IX (1941), p. 563–628; III (chap. 4 à 6), t. XIII (1943), p. 169–238.

XX. L. LE CAM, Convergence in distribution of stochastic processes, Univ. Cal. Publ. Statistics, n° 11 (1957), p. 207–236.

Les chiffres de référence indiquent successivement le paragraphe et le numéro.

$\mathcal{F}_+(T), \mathcal{F}_+, f_A, f^0$: conventions préliminaires.
$\pi(p), p_A$ ou $p|A$: 1,1.
$w^*(f), \int^* f d\omega, \int^* f(t) d\omega(t)$: 1,2.
$w^*, w_K^*$: 1,2.
$w^+, w^-, |w|$: 1,2.
$\mu(f), \mu(A)$: 1,5.
$\mathrm{Supp}(\mu)$: 1,6.
$\sum_{i \in I} \mu_i$: 1,7.
$\mu^*(f), \mu^*(A), \int^* f d\mu, \int^* f(t) d\mu(t)$: 1,9.
$\mu^*$: 1,9.
$\overline{\mathcal{L}}^p(T, \mu), \overline{\mathcal{L}}_F^p(T, \mu), \mathcal{L}^p(T, \mu), \mathcal{L}_F^p(T, \mu)$ (pour $1 \leq p \leq +\infty$): 1,10.
$\overline{\mathcal{L}}_F^p(\mu), \overline{\mathcal{L}}_F^p, \overline{\mathcal{L}}^p, \overline{\mathcal{L}}^p(\mu)$: 1,10.
$\overline{N}^p(f), N_p(f)$: 1,10.
$L_F^p(\mu), L_F^p$: 1,10.
$\int f d\mu, \mu(f), \int f(t) d\mu(t)$: 1,10.
$\mu_X^*, \mu_X, \mu|X$: 2,1.
$f \cdot \mu$: 2,2.
$\pi(\mu)$: 2,3.
$\lambda \otimes \mu$: 2,5.
$\mathfrak{A}(T), \mathfrak{B}(T)$: conventions du § 3.
$\mathcal{C}^b(T, F), \mathcal{C}^b(T), \mathcal{C}^b, \mathcal{C}_+^b(T), \mathcal{C}_+^b$: conventions du § 5.
$\mathcal{M}^b(T, \mathbf{C}), \mathcal{M}^b(T), \mathcal{M}^b, \mathcal{M}_+^b(T), \mathcal{M}_+^b$: conventions du § 5.
$\mathcal{L}\mu$: 5,7.
$\mathcal{F}(E)$: 6,1.
$p_v, p_{vw}$: 6,1.
$Q(E)$: 6,1.
$\tilde{\lambda}$: 6,1.

u(\mu) (\mu promesure): 6,2.
\mathcal{F}_{\mu} (\mu promesure ou mesure): 6,3.
\Gamma_{a}, \gamma_{a}: 6,5.
\gamma_{c}: 6,6.
\mathrm{Tr}(\mathbf{Q}/\mathbf{H}): \text{Annexe, 1}.
u^{*}: \text{Annexe, 2}.

Les chiffres de référence indiquent successivement le paragraphe et le numéro.

Additive (fonction d’ensemble): 3,2.
Adjointe d’une application linéaire: Annexe, 2.
Application $\mu$-propre: 2,3.
Application de Hilbert-Schmidt: Annexe, 2.
Associée (promesure) à une mesure: 6,1.
Base (mesure de) $\mu$: 2,2.
Bochner (théorème de): 6,12.
Borné (encombrement): 1,1.
Bornée (fonction d’ensemble): 3,2.
Bornée (mesure): 1,2.
Caractère d’un monoïde: 5,7.
Concassage: 1,8.
Concentré (encombrement) sur une partie: 1,1.
Concentrée (mesure) sur une partie: 1,4.
Condition de Prokhorov: 4,2 et 5,5.
Covariance d’une promesure gaussienne sur $\mathbf{R}^T$: 6,6.
Dénombrablement additive (fonction d’ensemble): 3,2.
Densité d’une mesure par rapport à une autre: 2,2.
Désintégration d’une mesure: 2,7.
Encombrement: 1,1.
Encombrement borné: 1,1.
Encombrement concentré sur une partie: 1,1.
Encombrement image: 1,1.
Encombrement induit: 1,1.
Encombrement localement borné: 1,1.
Ensemble intégrable: 1,9.
Ensemble localement négligeable: 1,4.
Ensemble mesurable: 1,5.
Ensemble modéré: 1,9.
Ensemble négligeable: 1,9.

Ensemble universellement mesurable: 3,3.
Espace fortement radonien: 3,3.
Espace radonien: 3,3.
Espace nucléaire: 6,10.
Essentielle (intégrale supérieure): 1,2.
Etroite (topologie): 5,3.
Extérieure (mesure): 1,9.
Fonction d’ensemble bornée: 3,2.
Fonction d’ensemble dénombrablement additive: 3,2.
Fonction d’ensemble intérieurement régulière: 3,2.
Fonction d’ensemble localement bornée: 3,2.
Fonction de type positif: 6,12.
Fonction essentiellement intégrable: 1,10.
Fonction génératrice d’une suite: 5,7.
Fonction intégrable: 1,10.
Fonction localement intégrable: 2,2.
Fonction localement négligeable: 1,4.
Fonction mesurable: 1,5.
Fonction modérée: 1,9.
Fonction négligeable: 1,9.
Fonction universellement mesurable: 2,7.
Forme quadratique nucléaire: Annexe, 1.
Fortement radonien (espace): 3,3.
Gaussienne (mesure, promesure): 6,5.
Gaussienne canonique (promesure) sur un espace hilbertien réel: 6,6.
Gaussienne (promesure) de covariance K: 6,6.
Gaussienne (mesure) de matrice de covariance C: 6,6.
Génératrice (fonction) d’une suite: 5,7.
Hilbert–Schmidt (application de): Annexe, 2.
Image d’un encombrement: 1,1.
Image d’une mesure: 2,3.
Image d’une promesure: 6,2.
Induit (encombrement): 1,1.
Induite (mesure): 2,1.
Intégrable (ensemble): 1,9.
Intégrable (fonction): 1,10.
Intégrale d’une fonction: 1,10.
Intégrale supérieure: 1,9.
Intégrale supérieure essentielle: 1,2.
Laplace (transformation de): 5,7.
Limite projective de mesures: 4,2.
Localement bornée (fonction d’ensembles): 3,2.

Localement borné (encombrement): 1,1.
Localement intégrable (fonction): 2,2.
Localement négligeable (ensemble): 1,4.
Localement négligeable (fonction): 1,4.
Localement presque partout: 1,4.
Marges d'une mesure sur un espace fonctionnel: 4,3.
Masse totale d'une promesure: 6,1.
Mesurable (ensemble): 1,5.
Mesurable (fonction): 1,5.
Mesure: 1,2.
Mesure bornée: 1,2.
Mesure de base $\mu$: 2,2.
Mesure de densité $f$ par rapport à une mesure $\mu$: 2,2.
Mesure extérieure d'un ensemble: 1,9.
Mesure gaussienne de matrice de covariance $C$: 6,6.
Mesure gaussienne de variance $Q$: 6,5.
Mesure image: 2,3.
Mesure induite: 2,1.
Mesure modérée: 1,9.
Mesure produit: 2,5.
Mesure de Wiener: 6,7.
Minlos (théorème de): 6,10.
Modéré (ensemble): 1,9.
Modérée (fonction): 1,9.
Modérée (mesure): 1,9.
Négligeable (ensemble): 1,9.
Négligeable (fonction): 1,9.
Noyau de type positif: 6,6.
Nucléaire (espace): 6,10.
Nucléaire (forme quadratique): Annexe, 1.
Plein (sous-monoïde): 5,7.
Positive (prémesure, mesure): 1,2.
Prémesure: 1,2.
Prémesure positive: 1,2.
Prémesure réelle: 1,2.
Presque partout: 1,9.
Produit de deux mesures: 2,5.
Produit d'une famille de mesures: 4,3.
Projectif (système) de mesures: 4,2.
Projective (limite) de mesures: 4,2.
Prokhorov (conditions de): 4,2 et 5,5.
Promesure: 6,1.

Promesure associée à une mesure: 6,1.
Promesure gaussienne canonique d’un espace hilbertien réel: 6,6.
Promesure gaussienne de covariance K sur $\mathbf{R}^T$: 6,6.
Promesure gaussienne de variance Q: 6,5.
Promesure image: 6,2.
Promesure (masse totale d’une): 6,1.
Promesure (transformée de Fourier d’une): 6,3.
Propre (application $\mu$-): 2,3.
Radonien (espace): 3,3.
Réelle (mesure, prémesure): 1,2.
Sazonov (topologie de): 6,10.
Somme d’une famille de mesures: 1,7.
Sous-monoïde plein: 5,7.
Sous-projectif (système) de mesures: 4,2.
Supérieure (intégrale): 1,9.
Support d’une mesure: 1,6.
Système projectif de mesures: 4,2.
Système sous-projectif de mesures: 4,2.
Théorème de Bochner: 6,12.
Théorème de Minlos: 6,10.
Topologie étroite: 5,3.
Topologie de Sazonov: 6,10.
Trace d’une forme quadratique par rapport à une autre: Annexe, 1.
Transformée de Fourier d’une mesure, d’une promesure: 6,3.
Transformée de Laplace d’une mesure: 5,7.
Type positif (fonction de): 6,12.
Type positif (noyau de): 6,6.
Universellement mesurable (ensemble): 3,3.
Universellement mesurable (fonction): 2,7.
Variance d’une mesure: 6,5.
Wiener (mesure de): 6,7.

§ 1. Prémesures et mesures sur un espace topologique ........................ 7
        1. Encombrements......................................................... 7
        2. Prémesures et mesures................................................. 8
        3. Exemples de mesures.................................................. 11
        4. Ensembles et fonctions localement négligeables........................ 13
        5. Ensembles et fonctions mesurables.................................... 14
        6. Familles filtrantes; support d’une mesure............................. 15
        7. Enveloppes supérieures et sommes de mesures........................... 17
        8. Concassages.......................................................... 18
        9. Intégrale supérieure................................................. 21
       10. Théorie de l’intégration............................................. 24

    § 2. Opérations sur les mesures............................................. 26
        1. Mesure induite sur un sous-espace mesurable........................... 26
        2. Mesures définies par des densités numériques.......................... 27
        3. Image d’une mesure................................................... 29
        4. Relèvement de mesures............................................... 32
        5. Produit de deux mesures.............................................. 34
        6. Intégration par rapport au produit de deux mesures.................... 36
        7. Un résultat sur la désintégration des mesures........................ 39

    § 3. Mesures et fonctions additives d’ensemble............................... 42
        1. Mesures et fonctions additives de compacts............................ 43
        2. Fonctions d’ensemble intérieurement régulières....................... 45
        3. Espaces radoniens.................................................... 47

    § 4. Limites projectives de mesures......................................... 50
        1. Compléments sur les espaces compacts et les limites projectives....... 50
        2. Systèmes projectifs de mesures....................................... 51
        3. Cas des systèmes projectifs dénombrables.............................. 53

    § 5. Mesures sur les espaces complètement réguliers.......................... 55
        1. Mesures et fonctions continues bornées............................... 55
        2. Mesures bornées et formes linéaires sur C(T)........................ 58

TABLE DES MATIERES
   3. Convergence étroite des mesures bornées ........................ 59
   4. Application: propriétés topologiques de l’espace ℋ⁺(T) ....... 61
   5. Critère de compacité pour la convergence étroite ............... 63
   6. Convergence étroite des mesures et convergence compacte des
      fonctions ..................................................... 65
   7. Application: transformation de Laplace ........................ 66
§ 6. Promesures et mesures sur un espace localement convexe .......... 70
   1. Promesures sur un espace localement convexe .................... 70
   2. Image d’une promesure ......................................... 72
   3. Transformée de Fourier d’une promesure ......................... 72
   4. Calculs d’intégrales gaussiennes ............................... 74
   5. Promesures et mesures gaussiennes .............................. 76
   6. Exemples de promesures gaussiennes ............................. 79
   7. Mesure de Wiener .............................................. 81
   8. Continuité de la transformée de Fourier ........................ 87
   9. Le lemme de Minlos ............................................. 89
   10. Mesures sur le dual d’un espace nucléaire ..................... 91
   11. Mesures sur un espace de Hilbert .............................. 92
  *12. Relations avec les fonctions de type positif,* ............... 94
ANNEXE: Compléments sur les espaces hilbertiens ....................... 96
   1. Trace d’une forme quadratique par rapport à une autre .......... 96
   2. Applications de Hilbert-Schmidt ............................... 98
Exercices du § 1 .................................................... 100
Exercices du § 2 .................................................... 101
Exercices du § 3 .................................................... 102
Exercices du § 4 .................................................... 106
Exercices du § 5 .................................................... 106
Exercices du § 6 .................................................... 110
Exercices de l’Annexe ............................................... 110
Note historique ...................................................... 113
Bibliographie ....................................................... 124
Index des notations ................................................ 126
Index terminologique ............................................... 128
