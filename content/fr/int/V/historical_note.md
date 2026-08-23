---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: int-v-fr
pdf_pages: 0141-0159
extraction: ocr
statements: 0
exercises: 0
content_sha256: 1d8583c22b821b60231eea98c762933f92086cfa7997f9affce93abd7143a87d
---

# NOTE HISTORIQUE

(Chapitres II à V)

(N.-B. — Les chiffres romains renvoient à la bibliographie placée à la fin de cette note.)

Le développement de la notion moderne d’intégrale est étroitement lié à l’évolution de l’idée de fonction, et à l’étude approfondie des fonctions numériques de variables réelles, qui s’est poursuivie depuis le début du xixe siècle. On sait qu’Euler concevait déjà la notion de fonction d’une manière assez générale, puisque pour lui la donnée d’une courbe « arbitraire » rencontrée en un seul point par toute parallèle à l’axe Oy définit une fonction $ y = f(x) $ (cf. Fonct. var. réelle, Note hist. des chap. I–II–III, p. 173); mais, ainsi que la plupart de ses contemporains, il se refusait à admettre que de telles fonctions pussent s’exprimer « analytiquement ». Ce point de vue ne devait guère se modifier jusqu’aux travaux de Fourier; mais la découverte, par ce dernier, de la possibilité de représenter des fonctions discontinues comme sommes de séries trigonométriques*, allait exercer une influence décisive sur les générations suivantes. À vrai dire, les démonstrations de Fourier manquaient totalement de rigueur, et leur domaine de validité n’apparaissait pas clairement; toutefois, les formules intégrales

$$
a_n = \frac{1}{\pi} \int_{-\pi}^{+\pi} \varphi(x) \cos nx \, dx, \quad b_n = \frac{1}{\pi} \int_{-\pi}^{+\pi} \varphi(x) \sin nx \, dx \quad (n \geqslant 1)
$$

donnant les coefficients du développement de $ \varphi $ en série de Fourier, avaient un sens intuitivement évident dès qu’on supposait $ \varphi $ continue et monotone par morceaux**. Aussi est-ce tout d’abord à ces fonctions que se borne Dirichlet, dans le célèbre mémoire (II) où il établissait la convergence de la série de Fourier; mais déjà, à la fin de son travail, il se préoccupe de l’extension de ses résultats à des classes de fonctions plus étendues. On sait que c’est à cette occasion que Dirichlet, précisant

\* Il ne s’agit d’ailleurs de « découverte » qu’en un sens tout à fait relatif: Euler connaissait déjà les développements en série trigonométrique de fonctions non périodiques telles que $ x $ ou $ x^2 $, et les formules (1) se trouvent dans un travail de Clairaut dès 1754, et chez Euler dans un mémoire de 1777. Mais là où le xviiiie siècle, faute d’une conception claire de ce que signifie un développement en série, négligeait de tels résultats et gardait intacte la croyance à l’impossibilité d’obtenir de tels développements pour des fonctions « discontinues », Fourier, au contraire, proclame que ses développements sont convergents « quelle que puisse être la courbe donnée qui répond à $ \varphi(x) $, soit qu’on puisse lui assigner une équation analytique, soit qu’elle ne dépende d’aucune loi régulière » (Œuvres, t. I, Paris (Gauthier-Villars), 1888, p. 210).

** Pour Fourier, l’intégrale est encore définie en faisant appel à la notion d’aire; la définition analytique de l’intégrale n’apparaît, rappelons-le, qu’avec Cauchy (cf. Fonct. var. réelle, Note hist. des chap. I–II–III, p. 174–175).

les idées de Fourier, définit la notion générale de fonction telle que nous l’entendons aujourd’hui; le premier point à élucider était naturellement de savoir dans quels cas il était encore possible d’attacher un sens aux formules (1). « Lorsque les solutions de continuité [de $ \varphi $] sont en nombre infini ... » dit Dirichlet ((II), p. 169), «il est nécessaire qu’alors la fonction $ \varphi(x) $ soit telle que, si l’on désigne par $ a $ et $ b $ deux quantités quelconques comprises entre $ -\pi $ et $ +\pi $, on puisse toujours placer entre $ a $ et $ b $ d’autres quantités $ r $ et $ s $ assez rapprochées pour que la fonction reste continue dans l’intervalle de $ r $ à $ s $. On sentira facilement la nécessité de cette restriction en considérant que les différents termes de la série [de Fourier] sont des intégrales définies et en remontant à la notion fondamentale des intégrales. On verra alors que l’intégrale d’une fonction ne signifie quelque chose qu’autant que la fonction satisfait à la condition précédemment énoncée. »

En termes modernes, Dirichlet semble croire que l’intégrabilité équivaut au fait que les points de discontinuité forment un ensemble rare; il signale d’ailleurs, quelques lignes plus loin, le célèbre exemple de la fonction égale à $ c $ pour $ x $ rationnel, à une valeur différente $ d $ pour $ x $ irrationnel, et affirme que cette fonction « ne saurait être substituée » dans l’intégrale. Il annonçait d’ailleurs des travaux ultérieurs sur ce sujet, mais ces travaux ne furent jamais publiés*, et pendant 25 ans, personne ne semble avoir cherché à avancer dans cette voie, peut-être parce que la considération de fonctions aussi « pathologiques » paraissait à l’époque tout à fait dénuée d’intérêt; en tout cas, lorsque Riemann, en 1854 ((III), p. 227-264), reprend la question (toujours à propos des séries trigonométriques**), il éprouve le besoin de justifier son travail: « Quelle que soit notre ignorance touchant la façon dont les forces et les états de la matière varient avec le temps et le lieu dans l’infiniment petit, nous pouvons pourtant tenir pour certain que les fonctions auxquelles les recherches de Dirichlet ne s’appliquent pas, n’interviennent pas dans les phénomènes naturels. Toutefois », poursuit-il, « il semble que ces cas non traités par Dirichlet méritent l’attention pour deux raisons. Premièrement, comme Dirichlet lui-même le remarque à la fin de son travail, ce sujet est en relation très étroite avec les principes du calcul infinitésimal, et peut servir à apporter plus de clarté et de certitude à ces principes. De ce point de vue, son étude a un intérêt immédiat. En second lieu, l’application des séries de Fourier n’est pas limitée aux recherches de physique; elles sont à présent appliquées aussi avec succès dans un domaine des mathématiques pures, la théorie des nombres, et là il semble que ce soient précisément les fonctions dont le développement en série trigonométrique n’a pas été étudié par Dirichlet, qui présentent de l’importance » ((III), p. 237-238).

\* Selon certaines indications (assez obscures) de Lipschitz (J. de Crelle, t. LXIII (1864), p. 296; traduit en français par P. Montel, dans Acta Math., t. XXXVI (1912), p. 261–295), Dirichlet aurait peut-être cru que si l’ensemble des points de discontinuité est rare, son « dérivé » est fini, et aurait en tout cas limité ses investigations au cas où il en est ainsi.

** De Dirichlet et Riemann à nos jours, nous verrons se poursuivre cette étroite association entre l’intégration et ce que nous appelons maintenant l’« analyse harmonique », qui en constitue en quelque sorte la pierre de touche.

L’idée de Riemann est de partir du procédé d’approximation de l’intégrale, remis en honneur par Cauchy, et de déterminer quand les « sommes de Riemann » d’une fonction $ f $, dans un intervalle borné $ (a, b) $, tendent vers une limite (la longueur maxima des intervalles de la subdivision tendant vers 0); problème dont il obtient sans peine la solution, sous la forme suivante: pour tout $ \alpha > 0 $, il y a une subdivision de $ (a, b) $ en intervalles partiels de longueur maxima assez petite pour que la somme des longueurs des intervalles de cette subdivision, où l’oscillation de $ f $ est $ > \alpha $, soit arbitrairement petite. Il montre en outre que cette condition est vérifiée, non seulement pour des fonctions continues et monotones par morceaux, mais aussi pour des fonctions pouvant avoir un ensemble partout dense de points de discontinuité*.

Le mémoire de Riemann ne fut publié qu’après sa mort, en 1867. Mais cette fois, l’époque était plus favorable à ce genre de recherches, et l’« intégrale de Riemann » prit naturellement sa place dans le courant d’idées qui conduisait alors à une étude poussée du « continu » et des fonctions de variables réelles (Weierstrass, Du Bois-Reymond, Hankel, Dini) et allait aboutir, avec Cantor, à l’éclosion de la théorie des ensembles. La forme donnée par Riemann à la condition d’intégrabilité suggérait l’idée de « mesure » pour l’ensemble des points de discontinuité d’une fonction dans un intervalle; mais près de 30 ans devaient s’écouler avant que l’on parvînt à donner une définition féconde et commode de cette notion.

Les premières tentatives dans cette direction sont dues à Stolz, Harnack et Cantor (1884–85); les deux premiers, pour définir la « mesure » d’une partie bornée E de $ \mathbf{R} $, considèrent des ensembles $ F \supset E $ qui sont réunions finies d’intervalles, prennent pour chaque F la somme des longueurs des intervalles correspondants, et appellent « mesure » de E la borne inférieure de ces nombres; tandis que Cantor, se plaçant d’emblée dans l’espace $ \mathbf{R}^n $, considère pour un ensemble borné E et pour $ \rho > 0 $ le voisinage $ V(\rho) $ de E formé des points dont la distance à E est $ \leq \rho $, et prend la borne inférieure du « volume » de $ V(\rho) $**. Avec cette définition, la « mesure » d’un ensemble était égale à celle de son adhérence, d’où résulte en particulier que la « mesure » de la réunion de deux ensembles sans point commun pouvait être strictement inférieure à la somme des « mesures » de ces deux ensembles. Sans doute pour pallier cette dernière difficulté, Peano (V) et Jordan (VI), quelques années plus tard, introduisent, à côté de la « mesure » de Cantor $ \mu(A) $ d’un ensemble A contenu dans un pavé I, sa « mesure intérieure » $ \mu(I) - \mu(I - A) $, et appellent « mesurables » les ensembles A (dits

\* Par contre, H. J. Smith donna, dès 1875, le premier exemple d’une fonction non intégrable au sens de Riemann, et dont l’ensemble des points de discontinuité est rare (Proc. Lond. Math. Soc., (1), t. VI (1875), p. 140–153).

** Cantor ne donne pas de définition précise de ce « volume » et se borne à dire qu’on peut le calculer par une intégrale multiple ((IV), p. 229–236 et 257–258). On voit facilement que sa définition équivaut à celle de Stolz-Harnack, par application du théorème de Borel-Lebesgue.

maintenant « quarrables ») pour lesquels ces deux nombres coïncident. La réunion de deux ensembles quarrables $ A, B $ sans point commun est alors quarrable et a pour « mesure » la somme des « mesures » de $ A $ et de $ B $; mais un ensemble ouvert borné n’est pas nécessairement quarrable, et l’ensemble des nombres rationnels contenus dans un intervalle borné ne l’est pas non plus, ce qui enlevait beaucoup d’intérêt à la notion de Peano-Jordan.

C’est à E. Borel (IX) que revient le mérite d’avoir su discerner les défauts des définitions antérieures et vu comment on pouvait y remédier. On savait depuis Cantor que tout ensemble ouvert $ U $ dans $ \mathbf{R} $ est réunion de la famille dénombrable de ses « composantes », intervalles ouverts deux à deux sans point commun; au lieu de chercher à approcher $ U $ « par le dehors » en l’enfermant dans une suite finie d’intervalles, Borel, s’appuyant sur le résultat précédent, propose de prendre comme mesure de $ U $ (lorsque $ U $ est borné) la somme des longueurs de ses composantes. Puis il décrit très sommairement* la classe d’ensembles (appelés depuis « boréliens ») qu’on peut obtenir, à partir des ensembles ouverts, en itérant indéfiniment les opérations de réunion dénombrable et de « différence » $ A - B $, et indique que, pour ces ensembles, on peut définir une mesure qui possède la propriété fondamentale d’additivité complète : si une suite $ (A_n) $ est formée d’ensembles boréliens deux à deux disjoints, la mesure de leur réunion (supposée bornée) est égale à la somme de leurs mesures.

Cette définition devait inaugurer une ère nouvelle en Analyse : d’une part, en liaison avec les travaux contemporains de Baire, elle formait le point de départ de toute une série de recherches de nature topologique sur la classification des ensembles de points ; et surtout, elle allait servir de base à l’extension de la notion d’intégrale, réalisée par Lebesgue dans les premières années du xx\textsuperscript{e} siècle.

Dans sa thèse (X a)), Lebesgue commence par préciser et développer les indications succinctes d’E. Borel ; imitant la méthode de Peano-Jordan, la « mesure extérieure » d’un ensemble borné $ A \subset \mathbf{R} $ est définie comme borne inférieure des mesures des ensembles ouverts contenant $ A $; puis, si $ I $ est un intervalle contenant $ A $, la « mesure intérieure » de $ A $ est la différence des mesures extérieures de $ I $ et de $ I - A $; on obtient ainsi une notion d’« ensemble mesurable » qui ne diffère de la définition « constructive » initiale de Borel que par adjonction d’une partie d’un ensemble de mesure nulle au sens de Borel. Cette définition s’étendait aussitôt aux espaces $ \mathbf{R}^n $; la vieille conception de l’intégrale définie $ \int_a^b f(t)\,dt $ d’une fonction bornée et $ \geqslant 0 $ comme « aire » limitée par la courbe $ y = f(x) $, les droites $ x = a, x = b $ et $ y = 0 $, fournissait donc une extension immédiate de l’intégrale de Riemann à toutes les fonctions $ f $ pour lesquelles la mesure de l’ensemble précédent se trouvait définie.

\* La mesure n’est encore pour Borel, à ce moment, qu’un moyen technique en vue de l’étude de certaines séries de fonctions rationnelles, et il souligne lui-même que, pour le but qu’il se propose, l’utilité de la mesure tient surtout au fait qu’un ensemble de mesure non nulle n’est pas dénombrable ((IX), p. 48).

Mais l’originalité de Lebesgue ne réside pas tellement dans l’idée de cette extension*, que dans sa découverte du théorème fondamental sur le passage à la limite dans l’intégrale ainsi conçue, théorème qui apparaît chez lui comme conséquence de l’additivité complète de la mesure**; il en aperçoit aussitôt toute l’importance, et en fait la pierre angulaire de l’exposé didactique de sa théorie qu’il donne, dès 1904, dans les célèbres « Leçons sur l’intégration et la recherche des fonctions primitives » (X b))***.

Nous ne pouvons décrire ici dans le détail les innombrables progrès que les résultats de Lebesgue devaient entraîner dans l’étude des problèmes classiques du Calcul infinitésimal; nous aurons l’occasion d’insister sur certains d’entre eux dans des Livres ultérieurs. Lebesgue lui-même avait déjà, dans sa thèse, appliqué sa théorie à l’extension des notions classiques de longueur et d’aire à des ensembles plus généraux que les courbes et surfaces usuelles; sur le développement considérable de cette théorie depuis un demi-siècle, nous renvoyons le lecteur à l’exposé récent de L. Cesari (XXVI). Mentionnons aussi les applications aux séries trigonométriques, développées par Lebesgue presque aussitôt après sa thèse (X c)), et qui allaient ouvrir à cette théorie de nouveaux horizons, dont l’exploration est loin d’être terminée de nos jours (voir (XXV)). Enfin et surtout, la définition des espaces $ L^p $ et le théorème de Fischer-Riesz ((XIII), (XV a)) et (XV b)); cf. Note historique du Livre V) mettaient en lumière le rôle que pouvait jouer en Analyse fonctionnelle la nouvelle notion d’intégrale; rôle qui ne devait que grandir avec les généralisations ultérieures de cette notion, dont nous allons parler dans un moment.

Auparavant, nous nous arrêterons un peu plus longuement sur un des problèmes auxquels Lebesgue consacra le plus d’efforts, la liaison entre les notions d’intégrale et de primitive. Avec la généralisation de l’intégrale introduite par Riemann s’était naturellement posée la question de savoir si la correspondance classique entre intégrale et primitive, valable pour les fonctions continues, subsistait encore dans des cas plus généraux. Or, il est facile de donner des exemples de fonctions $ f $, intégrables au sens de Riemann, et telles que $ \int_a^x f(t)\, dt $ n’ait pas de dérivée (ni

\* Indépendamment de Lebesgue, W. H. Young avait eu cette même idée pour les fonctions semi-continues (XI a)).
** Le cas particulier de ce théorème, où il s’agit d’une suite de fonctions intégrables au sens de Riemann dans un intervalle compact, uniformément bornées, et dont la limite est intégrable au sens de Riemann, avait été démontré par Arzelà (VII).
*** Parmi les conséquences les plus importantes de ce théorème dans la théorie générale de l’intégration, il faut mentionner en particulier le théorème d’Egoroff sur la convergence des suites de fonctions mesurables (XVI), précisant des remarques antérieures de Borel et Lebesgue. D’autre part, les fonctions mesurables (numériques) avaient d’abord été définies par Lebesgue par la propriété que, pour une telle fonction $ f $, l’image réciproque par $ f $ de tout intervalle de $ \mathbf{R} $ est un ensemble mesurable. Mais, dès 1903, Borel et Lebesgue avaient attiré l’attention sur les propriétés topologiques de ces fonctions; elles furent mises sous leur forme définitive par Vitali, qui, en 1905 (XII a)), formula le premier la propriété des fonctions mesurables que nous avons prise comme définition au chap. IV, § 5 (théorème retrouvé en 1912 par N. Lusin et connu d’ordinaire sous son nom).

$$
g(x) - g(a) = \int_a^x g'(t)\, dt;
$$

la différence entre les deux membres de cette relation est une fonction à variation bornée non constante et de dérivée nulle presque partout (fonction « singulière »). Il restait à caractériser les fonctions à variation bornée g telles que la relation (2) ait lieu. Lebesgue établit que ces fonctions (dites « absolument continues » par Vitali, qui en fit une étude détaillée) sont celles qui ont la propriété suivante: la variation totale de g dans un ensemble ouvert U (somme des variations totales de g dans chacune des composantes connexes de U) tend vers 0 avec la mesure de U.

Nous verrons ci-dessous comment, sous une forme affaiblie, ces résultats devaient plus tard acquérir une portée beaucoup plus générale. Sous leur forme initiale, leur champ d’application est demeuré assez restreint, et n’a pas dépassé le cadre de la théorie « fine » des fonctions de variables réelles; aussi restent-ils en dehors du plan de ce Traité***.

\* Les nombres dérivés à droite de g au point x sont les deux limites

$$
\lim_{h \to 0, h > 0} \sup (g(x + h) - g(x))/h, \qquad \lim_{h \to 0, h > 0} \inf (g(x + h) - g(x))/h.
$$

On définit de même les nombres dérivés à gauche.

** Ces fonctions avaient été introduites par Jordan, à propos de la rectification des courbes (VI); il montra qu’on peut en donner les deux définitions équivalentes suivantes:
a) f est différence de deux fonctions croissantes; b) pour toute subdivision de l’intervalle $ [a, b] $ par une suite finie croissante de points $ (x_i)_{0 \leq i \leq n} $, avec $ a = x_0, b = x_n $, la somme $ \sum_{i=1}^n |f(x_i) - f(x_{i-1})| $ est bornée par un nombre indépendant de la subdivision considérée.
La borne supérieure de ces sommes est la variation totale de f dans $ [a, b] $.

*** Mentionnons toutefois que la théorie moderne des « martingales » dans le Calcul des probabilités utilise constamment des raisonnements présentant une grande analogie avec ceux que l’on emploie pour l’étude de la dérivation.

A plus forte raison en est-il de même des développements ultérieurs de la théorie des primitives; nous nous contenterons de mentionner ici les profonds travaux de Denjoy et de ses émules et continuateurs (Perron, de la Vallée-Poussin, Khintchine, Lusin, Banach, etc.); le lecteur en trouvera un exposé détaillé dans le livre de S. Saks (XXIV).

Un des progrès essentiels apportés par la théorie de Lebesgue concerne les intégrales multiples. Cette notion s’était introduite vers le milieu du xviii\textsuperscript{e} siècle, et d’abord sous forme d’« intégrale indéfinie » (par analogie avec la théorie de l’intégrale des fonctions d’une seule variable, $ \iint f(x, y) dx dy $ désigne une solution de l’équation $ \frac{\partial^2 z}{\partial x \partial y} = f(x, y) $); mais, dès 1770, Euler a une conception fort claire de l’intégrale double étendue à un domaine borné (limité par des arcs de courbe analytiques), et écrit correctement la formule évaluant une telle intégrale au moyen de deux intégrales simples successives (I). Il n’était pas difficile de justifier cette formule en partant des « sommes de Riemann », tant que la fonction intégrée était continue, et le domaine d’intégration pas trop compliqué; mais dès qu’on voulait aborder des cas plus généraux, le procédé de Riemann rencontrait de sérieuses difficultés ($ f(x, y) $ peut être intégrable au sens de Riemann, sans que $ \int dx \int f(x, y) dy $ ait un sens lorsque les intégrales simples sont prises au sens de Riemann). Ces difficultés s’évanouissent quand on passe à la définition de Lebesgue; déjà ce dernier avait montré dans sa thèse que, lorsque $ f(x, y) $ est une « fonction de Baire » bornée, il en est de même des fonctions $ y \mapsto f(x, y) $ (pour tout $ x $) et $ x \mapsto \int f(x, y) dy $, et on a la formule

$$
\iint f(x, y) dx dy = \int dx \int f(x, y) dy
$$

(intégrale prise dans un rectangle). Un peu plus tard, Fubini (XIV) apporta à ce résultat un complément important en prouvant que, si on suppose seulement $ f $ intégrable, alors l’ensemble des $ x $ tels que $ y \mapsto f(x, y) $ ne soit pas intégrable est de mesure nulle, ce qui permettait d’étendre aussitôt la formule (3) à ce cas.

Enfin, en 1910 (X d)), Lebesgue aborde l’extension aux intégrales multiples de ses résultats sur les dérivées des intégrales simples. Il est ainsi amené à associer à une fonction $ f $, intégrable dans toute partie compacte de $ \mathbf{R}^n $, la *fonction d’ensemble* $ F(E) = \int_E f(x) dx $, définie pour toute partie intégrable $ E $ de $ \mathbf{R}^n $, qui généralise le concept d’« intégrale indéfinie »; et il observe à cette occasion que cette fonction possède les deux propriétés suivantes: 1\textsuperscript{o} elle est complètement additive; 2\textsuperscript{o} elle est « absolument continue » en ce sens que $ F(E) $ tend vers 0 avec la mesure de $ E $. La partie essentielle du mémoire de Lebesgue consiste à démontrer la réciproque de cette proposition*. Mais il ne s’en tient pas là et, dans la même direction, signale la possibilité de généraliser la notion de

\* L’outil principal, dans cette démonstration, est un théorème de recouvrement, démontré quelque temps auparavant par Vitali (XII b)) et qui est resté fondamental dans ce genre de questions.

fonction à variation bornée, en considérant les fonctions d’ensemble mesurable F(E), complètement additives et telles que $ \sum_n |F(E_n)| $ reste bornée pour toute partition dénombrable de E en parties mesurables $ E_n $. Et, s’il se borne en fait à ne considérer de telles fonctions que dans l’ensemble des pavés de $ \mathbf{R}^n $, il est bien clair qu’il ne restait plus qu’un pas à franchir pour aboutir à la notion générale de mesure que va définir J. Radon en 1913, englobant dans une même synthèse l’intégrale de Lebesgue et l’intégrale de Stieltjes, dont il nous faut parler maintenant.

En 1894, T. Stieltjes publiait, sous le titre « Recherches sur les fractions continues » (VIII), un mémoire très original où, à partir d’une question en apparence bien particulière, se trouvaient posés et résolus, avec une rare élégance, des problèmes d’une nature toute nouvelle dans la théorie des fonctions analytiques et celle des fonctions d’une variable réelle*. Afin de représenter la limite d’une certaine suite de fonctions analytiques, Stieltjes y était amené, entre autres, à introduire, sur la droite, le concept d’une «distribution de masse» positive, notion familière depuis longtemps dans les sciences physiques, mais qui n’avait jusque-là été considérée en mathématiques que sous des hypothèses restrictives (en général, l’existence d’une «densité» en tout point, variant de façon continue); il remarque que la donnée d’une telle distribution équivaut à celle de la fonction croissante $ \varphi(x) $ qui donne la masse totale contenue dans l’intervalle d’extrémités 0 et x pour $ x > 0 $, et cette masse changée de signe pour $ x < 0 $, les discontinuités de $ \varphi $ correspondant aux masses «concentrées en un point»**. Stieltjes forme alors, pour une telle distribution de masse dans un intervalle $ [a, b] $, les «sommes de Riemann» $ \sum_i f(\xi_i)(\varphi(x_{i+1}) - \varphi(x_i)) $ et montre que, lorsque $ f $ est continue dans $ [a, b] $, ces sommes tendent vers une limite qu’il note $ \int_a^b f(x)\,d\varphi(x) $. N’ayant besoin que d’intégrer des fonctions continues (et même des fonctions dérivables) Stieltjes ne poussa pas plus avant l’étude de cette intégrale*** et pendant une dizaine d’années cette notion ne parait pas avoir attiré l’attention****. Mais, en 1909, F. Riesz (XV c),

\* C’est là entre autres qu’est formulé et résolu le célèbre «problème des moments» (cf. Note hist. du Livre V).

** Stieltjes ne fait pas encore de différence entre les diverses espèces d’intervalles ayant mêmes extrémités $ a, b $, ce qui le conduit à concevoir qu’aux points de discontinuité $ c $ de $ \varphi $, une partie de la masse concentrée en $ c $ appartient à l’intervalle d’origine $ c $, et l’autre partie à l’intervalle d’extrémité $ c $, suivant la valeur de $ \varphi(c) $.

*** Il faut cependant noter la première apparition, chez Stieltjes, de l’idée de «convergence» d’une suite de mesures ((VIII), p. 95; il s’agit en fait de la limite forte).

**** Elle prend toutefois de l’importance avec le développement de la théorie spectrale des opérateurs, à partir de 1906, par Hilbert et son école. C’est à cette occasion que Hellinger, vers 1907, définit des intégrales telles que celle qu’il notait $ \int \frac{(dg)^2}{df} $, et qui paraissaient au premier abord plus générales que celle de Stieltjes; mais en fait, Hahn montra, dès 1912, qu’elles se ramènent à cette dernière (ce sont des cas particuliers de la notion de «fonction de mesures»; cf. chap. V, § 5, n° 9).

Presque aussitôt après la parution du mémoire de Radon, Fréchet remarquait que presque tous les résultats de ce travail pouvaient s’étendre au cas où la « fonction complètement additive d’ensemble », au lieu d’être définie pour les parties mesurables de $ \mathbf{R}^n $, est définie pour certaines parties d’un ensemble E quelconque (ces parties étant telles que les opérations de réunion dénombrable et de « différence » donnent encore des ensembles pour lesquels la fonction est définie). Toutefois, l’expression d’une mesure de base $ \mu $ sous la forme $ g . \mu $ reposait, chez Lebesgue et Radon, sur des raisonnements faisant intervenir de façon essentielle la topologie de $ \mathbf{R}^n $ (et nous avons vu que la démonstration de Radon ne s’applique que si $ \mu $ est une mesure ayant pour base la mesure de Lebesgue); c’est seulement en 1930 que O. Nikodym (XX) obtint ce théorème sous sa forme générale, par un raisonnement direct (notablement simplifié quelques années plus tard par J. von Neumann, grâce à l’utilisation des propriétés des espaces $ L^2 $ ((XXII), p. 127–130)).

Avec le mémoire de Radon, la théorie générale de l’intégration pouvait être considérée comme achevée dans ses grandes lignes ; comme

\* C’est aussi dans ce travail qu’apparaît la notion de limite vague d’une suite de mesures ((XV c), p. 49).

acquisitions ultérieures substantielles, on ne peut guère mentionner que la définition du produit infini de mesures, due à Daniell (XIX b)), et celle de l’intégrale d’une fonction à valeurs dans un espace de Banach, donnée par Bochner en 1933 (XXI), et qui préludait à l’étude de l’« intégrale faible » dont nous traiterons au chap. VI. Mais il restait à populariser la nouvelle théorie, et à en faire un instrument mathématique d’usage courant, alors que la majorité des mathématiciens, vers 1910, ne voyait encore dans l’« intégrale de Lebesgue » qu’un instrument de haute précision, de maniement délicat, destiné seulement à des recherches d’une extrême subtilité et d’une extrême abstraction. Cé fut là l’œuvre de Carathéodory, dans un livre longtemps resté classique (XVIII) et qui enrichit d’ailleurs la théorie de Radon de nombreuses remarques originales.

Mais c’est avec ce livre aussi que la notion d’intégrale, qui avait été au premier plan des préoccupations de Lebesgue (comme le marquent suffisamment les titres de sa thèse (X a)) et de son principal ouvrage sur ces questions (X b))) cède le pas pour la première fois à celle de mesure, qui avait été chez Lebesgue (comme avant lui chez Jordan) un moyen technique auxiliaire. Ce changement de point de vue était dû sans doute, chez Carathéodory, à l’excessive importance qu’il semble avoir attachée aux « mesures $ p $-dimensionnelles »*. Depuis lors, les auteurs qui ont traité d’intégration se sont partagés entre ces deux points de vue, non sans entrer dans des débats qui ont fait couler beaucoup d’encre sinon beaucoup de sang**. Les uns ont suivi Carathéodory ; dans leurs exposés sans cesse plus abstraits et plus axiomatisés, la mesure, avec tous les raffinements techniques auxquels elle se prête, non seulement joue le rôle dominant, mais encore elle tend à perdre contact avec les structures topologiques auxquelles en fait elle est liée dans la plupart des problèmes où elle intervient. D’autres exposés, dont le présent Traité, suivent de plus ou moins près une méthode déjà indiquée en 1911 par W. H. Young, dans un mémoire malheureusement peu remarqué (XI b)), et développée ensuite par Daniell. Le premier, traitant de l’intégrale de Lebesgue, partait de l’« intégrale de Cauchy » des fonctions continues à support compact, supposée connue, pour définir successivement (comme nous l’avons fait au chap. IV, § 1) l’intégrale supérieure des fonctions semi-continues inférieurement, puis des fonctions numériques quelconques, d’où une définition des fonctions intégrables, calquée sur celle de Lebesgue pour les ensembles, par des moyens purement « fonctionnels ».

\* Il s’agit là de la généralisation de la notion de « longueur d’une courbe plane » à des valeurs quelconques $ n $ et $ p $ de la dimension de l’espace ambiant et de la dimension de l’espace étudié ; on suppose bien entendu qu’on a $ 0 \leq p \leq n $, mais on ne suppose pas toujours que $ p $ soit entier. Cette question a fait l’objet de travaux de nombreux auteurs depuis Minkowski, Carathéodory et Hausdorff ; Lebesgue lui-même, qui en aborde des cas particuliers dans sa thèse, ne semble pas y avoir vu autre chose qu’une occasion de mettre à l’essai la puissance des outils qu’il venait de forger.

** Cf. les comptes rendus par P. Halmos du premier volume de ce Livre (Bull. Amer. Math. Soc., t. LIX (1953), p. 249) et par J. Dieudonné du livre de Mayrhofer (ibid., t. LIX (1953), p. 479).

Daniell, en 1918 ((XIX a)); cf. (XXVII)) étendit cet exposé, avec quelques variantes, à des fonctions définies sur un ensemble quelconque; son principal mérite fut d’apercevoir le rôle joué dans la théorie abstraite par la condition $ \lim_{n \to \infty} \int f_n d\mu = 0 $ pour toute suite décroissante $(f_n)$ tendant simplement vers 0 (ce qui ne pouvait apparaître aussi clairement dans la théorie des mesures de Radon, où cette condition est automatiquement vérifiée en vertu du théorème de Dini). Dans le même ordre d’idées (et en liaison étroite avec les méthodes utilisées en théorie spectrale avant Gelfand), il nous faut aussi signaler le mémoire de F. Riesz (XV d)) qui met sous une forme concise et élégante les quelques résultats de la théorie des espaces ordonnés qui jouent un rôle dans la théorie de l’intégration; nous avons suivi d’assez près son exposé au chap. II.

Plutôt que dans des ouvrages d’exposition, plus ou moins agréables à lire, mais dont le contenu substantiel ne pouvait plus beaucoup varier, c’est du côté des applications qu’il faut chercher les progrès réalisés par la théorie de l’Intégration depuis 1920: théorie des probabilités (autrefois prétexte à devinettes et à paradoxes, et devenue une branche de la théorie de l’Intégration depuis son axiomatisation par Kolmogoroff (XXIII), mais branche autonome avec ses méthodes et ses problèmes propres); théorie ergodique; théorie spectrale et analyse harmonique, depuis que la découverte par Haar de la mesure qui porte son nom, et le mouvement d’idées provoqué par cette découverte, ont fait de l’intégrale l’un des plus importants outils en théorie des groupes. Avec ces questions, nous sortons du cadre de la présente Note; quelques-unes d’entre elles seront traitées dans des chapitres ou Livres ultérieurs.

(I) L. Euler, Opera Omnia: De formulis integralibus duplicatis (1), t. XVII, Leipzig-Berlin (Teubner), 1915, p. 289–315.
(II) G. Lejeune-Dirichlet, Sur la convergence des séries trigonométriques qui servent à représenter une fonction arbitraire entre des limites données, J. de Crelle, t. IV (1829), p. 157–169 (= Werke, t. I, p. 118–132, Berlin (G. Reimer), 1889).
(III) B. Riemann, Gesammelte Mathematische Werke, 2e éd., Leipzig (Teubner), 1892.
(IV) G. Cantor, Gesammelte Abhandlungen, Berlin (Springer), 1932.
(V) G. Peano, Applicazioni geometriche del calcolo infinitesimale, Turin, 1887.
(VI) C. Jordan, Cours d’Analyse, t. I, 2e éd., Paris (Gauthier-Villars), 1893.
(VII) C. Arzelà: a) Sulla integrabilità di una serie di funzioni, Rendic. Acc. dei Lincei, (4), t. I (1885), p. 321–326; b) Sulla integrazione per serie, ibid., p. 532–537 et 566–569.
(VIII) T. Stieltjes, Recherches sur les fractions continues, Ann. Fac. Sci. de Toulouse, t. VIII (1894), J. 1 à J. 122.
(IX) E. Borel, Leçons sur la théorie des fonctions, Paris (Gauthier-Villars), 1898.
(X) H. Lebesgue: a) Intégrale, longueur, aire, Annali di Mat., (3), t. VII (1902), p. 231–359; b) Leçons sur l’Intégration et la recherche des fonctions primitives, Paris (Gauthier-Villars), 1904; c) Sur les séries trigonométriques, Ann. Ec. Norm. Sup., (3), t. XX (1903), p. 453–485; d) Sur l’intégration des fonctions discontinues, Ann. Ec. Norm. Sup., (3), t. XXVII (1910), p. 361–450.
(XI) W. H. Young: a) On upper and lower integration, Proc. Lond. Math. Soc., (2), t. II (1905), p. 52–66; b) A new method in the theory of integration, Proc. Lond. Math. Soc., (2), t. IX (1911), p. 15–50.
(XII) G. Vitali: a) Una proprieta delle funzioni misurabili, R. Ist. Lombardo, Rendiconti, (2), t. XXXVIII (1905), p. 599–603; b) Sui gruppi di punti e sulle funzioni di variabili reali, Rendic. Acc. Sci. di Torino, t. XLIII (1908) p. 229–236.
(XIII) E. Fischer, Sur la convergence en moyenne, C. R. Acad. Sci., t. CXLIV (1907), p. 1022–1024.
(XIV) G. Fubini, Sugli integrali multipli, Rendic. Acc. dei Lincei, (5), t. XVI (1907), p. 608–614.
(XV) F. Riesz: a) Sur les systèmes orthogonaux de fonctions, C. R. Acad. Sci., t. CXLIV (1907), p. 615–619; b) Untersuchungen über Systeme integrierbarer Funktionen, Math. Ann., t. LXIX (1910), p. 449–497; c) Sur certains systèmes singuliers d’équations intégrales, Ann. Ec. Norm. Sup., (3), t. XXVIII (1911), p. 33–62; d) Sur quelques notions fondamentales dans la théorie générale des opérations linéaires, Ann. of Math., (2), t. XLI (1940), p. 174–206.
(XVI) D. Egoroff, Sur les suites de fonctions mesurables, C. R. Acad. Sci., t. CLII (1911), p. 244.
(XVII) J. Radon, Theorie und Anwendungen der absolut additiven Mengenfunktionen, Sitzungsber. der math. naturwiss. Klasse der Akad. der Wiss. (Wien), t. CXXII, Abt. II a (1913), p. 1295–1438.
(XVIII) C. Carathéodory, Vorlesungen über reelle Funktionen, Leipzig-Berlin (Teubner), 1918.
(XIX) P. J. Daniell: a) A general form of integral, Ann. of Math., (2), t. XIX (1918), p. 279–294; b) Integrals in an infinite number of dimensions, Ann. of Math., (2), t. XX (1919), p. 281–288.

(XX) O. Nikodym, Sur une généralisation des intégrales de M. J. Radon, Fund. Math., t. XV (1930), p. 131–179.
(XXI) S. Bochner, Integration von Funktionen deren Werte die Elemente eines Vektorraumes sind, Fund. Math., t. XX (1933), p. 262–276.
(XXII) J. von Neumann, On rings of Operators III, Ann. of Math., (2), t. XLI (1940), p. 94–161.
(XXIII) A. Kolmogoroff, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer), 1933.
(XXIV) S. Saks, Theory of the integral, 2e éd., New York (Stechert), 1937.
(XXV) A. Zygmund, Trigonometric series, Warszawa, 1935 (2e éd., Cambridge University Press, 1959).
(XXVI) L. Cesari, Surface area, Princeton, 1954.
(XXVII) L.-H. Loomis, An introduction to abstract harmonic analysis, London–New York–Toronto (van Nostrand), 1953.

INDEX DES NOTATIONS

Les chiffres de référence indiquent successivement le paragraphe et le numéro (ou, exceptionnellement, l’exercice).

\mathcal{F}_+(E), \mathcal{F}_+ (E ensemble): Conventions préliminaires.
\mu^*(f), \mu^*(A), \int^* f d\mu, \int^* f(t) d\mu(t), \int^* f\mu: 1, 1.
\bar{\mathcal{F}}_F^p(T, \mu), \bar{\mathcal{F}}_F^p(\mu), \bar{\mathcal{F}}_F^p: 1, 3.
\overline{N}_p(f), \overline{\mathcal{L}}_F^p(T, \mu), \overline{\mathcal{L}}_F^p(\mu), \overline{\mathcal{L}}_F^p: 1, 3.
\overline{\mathcal{L}}_F^p(T, \theta) (\theta mesure complexe): 1, 3.
\int \lambda_t d\mu(t) (t \mapsto \lambda_t famille de mesures positives): 3, 1.
\int d\mu(t) \int f(x) d\lambda_t(x): 3, 1.
\|\Lambda\| (\Lambda diffusion): 3, 5.
\langle \eta, h \rangle: 3, 5.
\Lambda f, \mu \Lambda: 3, 5.
\Lambda \mathbf{H}: 3, 6.
\mathcal{L}_{loc}^1(T, \mu; F), L_{loc}^1(T, \mu; F): 5, 1.
u . \theta (u fonction complexe, \theta mesure complexe): 5, 2.
\int_A^* f d\mu: 5, 3.
u(\mu_1, \ldots, \mu_n) (u fonction numérique positivement homogène): 5, 9.
\pi(\mu) (\pi application \mu-propre): 6, 1.
\pi(\theta) (\theta mesure complexe, \pi application |\theta|-propre): 6, 4.
\int \int^* f(t, t') d\mu(t) d\mu'(t'), \int \int^* f(t, t') d\mu(t) d\mu'(t'), \int \int f(t, t') d\mu(t) d\mu'(t'): 8, 1.

Les chiffres de référence indiquent successivement le paragraphe et le numéro (ou, exceptionnellement, l’exercice).

Adapté (couple $ \mu $-): 4, 1.
Adéquate (application $ \mu $-): 3, 1.
Application $ \mu $-adéquate: 3, 1.
Application $ \mu $-pré-adéquate: 3, 1.
Application $ \mu $-propre (ou propre pour $ \mu $): 6, 1 et 6, 4.
Appartenant au domaine d’une diffusion (mesure): 3, 5.
Base (mesure de) $ \mu $: 5, 2.
Bornée (diffusion): 3, 5.
Composée (diffusion): 3, 6.
Concentrée (mesure) sur un ensemble: 5, 7.
Couple $ \mu $-adapté: 4, 1.
Décomposition en tranches d’une mesure: 6, 6.
Densité (mesure de) $ g $ par rapport à $ \theta $: 5, 2.
Désintégration d’une mesure: 6, 6.
Diffuse (mesure): 5, 10.
Diffusion: 3, 5.
Diffusion bornée: 3, 5.
Diffusion composée: 3, 6.
Ensemble essentiellement $ \mu $-intégrable: 1, 3.
Ensemble portant une mesure: 5, 7.
Ensemble universellement mesurable: 3, 4.
Equivalentes (mesures): 5, 6.
Essentielle (intégrale supérieure): 1, 1.
Essentiellement $ \mu $-intégrable (ensemble, fonction): 1, 3.
Essentiellement intégrable dans A (fonction): 5, 3.
Etrangères*(mesures): 5, 7.
Famille localement dénombrable de fonctions $ \geqslant 0 $: 5, 4.
Famille sommable de mesures positives: 2, 1.
Fonction de puissance p-ème essentiellement intégrable: 1, 3.
Fonction essentiellement intégrable: 1, 3.
Fonction essentiellement intégrable dans A: 5, 3.
Fonction localement intégrable: 5, 1.
Fonction localement intégrable dans A: 5, 3.
Fonction $ \mu $-mesurable dans A: 5, 3.
Fonction $ \mu $-modérée: 1, 2.
Fonction scalairement essentiellement intégrable: 3, 1.
Fonction universellement mesurable: 3, 4.
Fonction vaguement continue: 3, 1.
Fonction vaguement $ \mu $-mesurable: 3, 1.
Image d’une mesure: 6, 1 et 6, 4.
Image réciproque d’une mesure par un homéomorphisme local: 6, 6.
Intégrale d’une fonction essentiellement intégrable: 1, 3.
Intégrale d’une fonction dans A (ou étendue à A): 5, 3.
Intégrale supérieure essentielle: 1, 1.
Intégration par parties: 8, exerc. 9.
Lebesgue (théorème de décomposition de): 5, 7.

Lebesgue-Fubini (théorème de): 8, 4.
Lebesgue-Nikodym (théorème de): 5, 5.
Localement dénombrable (famille de fonctions $ \geq 0 $): 5, 4.
Localement intégrable (fonction): 5, 1.
Localement intégrable dans A (fonction): 5, 1.
Mesurable dans A (fonction): 5, 3.
Mesure appartenant au domaine d'une diffusion: 3, 5.
Mesure concentrée sur un ensemble: 5, 7.
Mesure de base $ \mu $: 5, 2.
Mesure de densité g par rapport à $ \theta $: 5, 2.
Mesure diffuse: 5, 10.
Mesure modérée: 1, 2.
Mesure de Stieltjes: 6, exerc. 5.
Mesures équivalentes: 5, 6.
Mesures étrangères: 5, 7.
Modérée (fonction $ \mu $-): 1, 2.
Modérée (mesure): 1, 2.
Modérée (partie $ \mu $-): 1, 2.
Norme d'une diffusion: 3, 5.
Partie $ \mu $-modérée: 1, 2.
Portant une mesure (ensemble): 5, 7.
Pré-adéquate (application $ \mu $-): 3, 1.
Produit d'une mesure par une fonction localement intégrable: 5, 2.
Propre (application $ \mu $-): 6, 1 et 6, 4.
Scalairement essentiellement intégrable (fonction): 3, 1.
Sommable (famille) de mesures positives: 2, 1.
Théorème de décomposition de Lebesgue: 5, 7.
Théorème de Lèbesgue-Fubini: 8, 4.
Théorème de Lebesgue-Nikodym: 5, 5.
Universellement mesurable (ensemble, fonction): 3, 4.
Vaguement continue (fonction): 3, 1.
Vaguement $ \mu $-mesurable (fonction): 3, 1.

CHAPITRE V. — Intégration des mesures .................................................. 1
§ 1. Intégrale supérieure essentielle ..................................................... 2
    1. Définition de l'intégrale supérieure essentielle ......................... 2
    2. Fonctions et mesures modérées ................................................. 4
    3. Fonctions essentiellement intégrables ....................................... 7
    4. Une propriété spéciale à l'intégrale supérieure essentielle .......... 11
§ 2. Familles sommables de mesures positives ....................................... 12
    1. Définition des familles sommables de mesures ............................. 12
    2. Intégration par rapport à une somme de mesures positives ............. 13
    3. Décomposition d'une mesure en somme de mesures à supports compacts ................................................................. 15
§ 3. Intégration de mesures positives .................................................. 16
    1. Fonctions à valeurs dans un espace de mesures ............................ 16
    2. Intégrales superposées de fonctions positives ............................. 21
    3. Intégrales superposées de fonctions à valeurs dans un espace de Banach ................................................................. 25
    4. Fonctions universellement mesurables ....................................... 28
    5. Diffusions .................................................................................. 29
    6. Composition des diffusions bornées ............................................. 32
§ 4. Intégration de mesures positives ponctuelles ................................... 34
    1. Familles de mesures ponctuelles ............................................... 34
    2. Intégrales supérieures de fonctions positives par rapport à une intégrale de mesures ponctuelles ................................. 36
    3. Mesurabilité par rapport à une intégrale de mesures ponctuelles .... 39
    4. Intégration des fonctions à valeurs dans un espace de Banach, par rapport à une intégrale de mesures ponctuelles .................... 40
§ 5. Mesures définies par des densités numériques ................................ 41
    1. Fonctions localement intégrables .............................................. 41
    2. Mesures définies par des densités numériques ............................. 43
    3. Intégration par rapport à une mesure définie par une densité ...... 46
    4. Comportement du produit par rapport aux opérations usuelles ....... 49
    5. Caractérisation des mesures de base $ \mu $ ................................. 52
    6. Mesures équivalentes ............................................................. 57
    7. Mesures étrangères .................................................................. 59
    8. Applications: I. Dualité des espaces $ L^p $ ................................. 61
    9. Applications: II. Fonctions de mesures ....................................... 65
    10. Mesures diffuses; mesures atomiques ....................................... 67
§ 6. Images d'une mesure ................................................................. 68
    1. Image d'une mesure positive .................................................... 68
    2. Intégration par rapport à l'image d'une mesure positive ............. 70
    3. Propriétés de l'image d'une mesure positive ............................. 72
    4. Image d'une mesure complexe .................................................. 74
    5. Application: changement de variable dans l'intégrale de Lebesgue .. 75
    6. Décomposition en tranches. Image réciproque d'une mesure par un homéomorphisme local ......................................................... 78
§ 7. Intégration par rapport à une mesure induite ................................. 81
    1. Intégration par rapport à une mesure induite ............................. 81
    2. Propriétés des mesures induites .............................................. 84

§ 8. Produits de mesures ..................................................... 86
    1. Interprétation de la mesure produit comme intégrale de mesures .. 86
    2. Fonctions mesurables par rapport à un produit de deux mesures.... 89
    3. Intégration de fonctions positives ................................. 91
    4. Intégration de fonctions à valeurs dans un espace de Banach..... 96
    5. Opérations sur le produit de deux mesures ....................... 98
    6. Intégration par rapport à un produit fini de mesures ........... 100
    7. Application: Mesure de la boule euclidienne dans R" ............. 101

Exercices du § 1 .......................................................... 103
Exercices du § 2 .......................................................... 104
Exercices du § 3 .......................................................... 104
Exercices du § 4 .......................................................... 107
Exercices du § 5 .......................................................... 108
Exercices du § 6 .......................................................... 118
Exercices du § 7 .......................................................... 124
Exercices du § 8 .......................................................... 126

Note historique (chap. II à V) ........................................... 136
Bibliographie ............................................................ 147

Index des notations ..................................................... 148
Index terminologique ................................................... 149
Table de concordance .................................................. 153

TABLE DE CONCORDANCE
DE LA PREMIÈRE ET DE LA SECONDE ÉDITION

1re édition                2e édition
§ 1, Déf. 1                Chap. IV, § 5,
                            n° 7, déf. 4
§ 1, lemme 1               Chap. IV, § 5,
                            n° 7, lemme 2
§ 1, prop. 1               Chap. IV, § 5,
                            n° 8, prop. 12
§ 1, déf. 2                 Chap. IV, § 5,
                            n° 8, déf. 6
§ 1, prop. 2               Chap. IV, § 5,
                            n° 8, prop. 13
§ 1, prop. 3               Chap. IV, § 5,
                            n° 10, prop. 15
§ 1, déf. 3                 Chap. IV, § 5,
                            n° 9, déf. 7
§ 1, prop. 4               Chap. IV, § 5,
                            n° 9, prop. 14
§ 1, prop. 5               Chap. IV, § 5,
                            n° 10, prop. 16
§ 1, exerc. 1              Chap. IV, § 5,
                            exerc. 21
§ 1, exerc. 2              Supprimé
§ 2, déf. 1                 § 1, déf. 1
§ 2, prop. 1               § 1, prop. 10
§ 2, prop. 2               § 1, prop. 4
§ 2, prop. 3               § 1, prop. 7
§ 2, cor. de la prop. 3    § 1, prop. 7 et
                            Remarque 2 du
                            n° 2
§ 2, prop. 4               § 1, prop. 1
§ 2, prop. 5               § 1, lemme 1
§ 2, lemme 1               Supprimé
§ 2, lemme 2               § 1, prop. 2
§ 2, cor. de la prop. 5    § 1, n° 3
§ 2, déf. 2                 § 1, n° 3
§ 2, prop. 6               § 1, n° 3
§ 2, prop. 7               § 1, prop. 9
§ 2, prop. 8               § 1, prop. 10
§ 2, prop. 9               § 1, exerc. 3 a)
§ 2, exerc. 1              § 1, prop. 1
§ 2, exerc. 2              § 1, exerc. 1
§ 2, exerc. 3              § 1, exerc. 2
§ 2, exerc. 4              § 1, prop. 3
§ 2, exerc. 5              § 1, exerc. 4
§ 2, exerc. 6              § 1, exerc. 3 b)
§ 2, exerc. 7              § 1, exerc. 5

1re édition                2e édition
Déf. 1                     § 3
                            Supprimée (remplacée par une définition plus générale)
Prop. 1                     Supprimée
Cor. de la prop. 1         Prop. 2
Prop. 2                     Prop. 3
Cor de la prop. 2          Cor. 1 de la prop. 3
Prop. 3                     Prop. 4
Prop. 4                     Prop. 5
Cor. de la prop. 4         Cor de la prop. 5
Prop. 5                     § 2, prop 1 et 3
                            et cor. 3 de la prop. 1
Cor. 1 de la prop. 5       § 2, cor. 1 de la prop. 1
Cor. 2 de la prop. 5       § 2, cor. 2 de la prop. 1
Prop. 6                     § 2, prop. 2
Cor. 1 de la prop. 6       § 2, Cor. 1 de la prop. 3
Cor. 2 de la prop. 6       Supprimé
Exerc. 6                    § 1, exerc. 4 a)
Exerc. 7 a)                 § 2, exerc. 1
Exerc. 7 b)                 § 2, exerc. 2
Exerc. 7 c)                 § 2, exerc. 3
Exerc. 8                    Exerc. 6 b)

§ 4
Exerc. 1                    Prop. 1
Exerc. 2                    Exerc. 1
Exerc. 3                    Exerc. 2

§ 5
Prop. 2                     Prop. 3
Prop. 3                     Prop. 4
Prop. 4                     Supprimée
Prop. 5                     Cor. de la prop. 2
Cor. 1 de la prop. 5        Cor. 2 de la prop. 3
Cor. 2 de la prop. 5        Cor. 2 de la prop. 3 1re édition        2e édition        1re édition        2e édition

§ 5
Cor. 3 de la prop. 5    Cor. 3 de la prop. 3    Prop. 1    Prop. 5
Prop. 6    Cor. de la prop. 6    Prop. 2    Prop. 6
Prop. 7    Prop. 8    Cor. de la prop. 2    Cor. 1 de la prop. 7
Prop. 8    Supprimée    Prop. 3    Prop. 2
Th. 2    Th. 2 et cor. 5 du th. 2    Cor. du th. 1    Cor. 2 de la prop. 7
Cor. du th. 2    Cor. 2 du th. 2    Prop. 4    Prop. 7
Cor. de la prop. 13    Cor. 1 de la prop. 13    Prop. 5    Cor. 1 de la prop. 8
Lemme 1    Lemme 4    Cor. 1 de la prop. 5    Cor. 3 de la prop. 5
Déf. 6    Chap. III, § 1, n° 3, Exemple 1    Cor. 2 de la prop. 5    Prop. 8
Exerc. 5    Supprimé    Cor. 3 de la prop. 5    Cor. 1 de la prop. 3
Exerc. 6    Exerc. 5    Cor. 4 de la prop. 5    Cor. 2 de la prop. 3
Exerc. 7    Supprimé    Cor. 5 de la prop. 5    Prop. 9
Exerc. n (8 ≤ n ≤ 28)    Exerc. n − 2    Cor. 6 de la prop. 5    Supprimé
Prop. 6    Cor. 1 de la prop. 6    Cor. 7 de la prop. 5    Prop. 9
Cor. de la prop. 6    Cor. 2 de la prop. 6    Cor. 8 de la prop. 5    Prop. 4
Prop. 7    Prop. 8    Cor. 9 de la prop. 5    Cor. de la prop. 4
Cor. de la prop. 7    Cor. de la prop. 8    Prop. 6    Prop. 10
Prop. 8    Prop. 9    Prop. 7    Prop. 11
Prop. 8    Prop. 8    Exerc. 19    Prop. 12
Cor. du th. 1    Cor. 1 du th. 1    Chap. III, § 4, n° 5, prop. 8
Cor. de la prop. 3    Cor. 2 de la prop. 3    Prop. 5    Cor. 2 du th. 1
Prop. 5    Prop. 3    Prop. 6    Prop. 11
Prop. 6    Prop. 3    Cor. 1 de la prop. 3    Chap. III, § 4, n° 5, prop. 8
