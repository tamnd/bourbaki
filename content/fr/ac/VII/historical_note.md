---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: Diviseurs
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: ac-v-vii-fr
pdf_pages: 0306-0346
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8bcc1e93fc82a2afdc8177bd0da28b9320120bd88e8fafc4cac629a5b42ba698
---

# NOTE HISTORIQUE

(chap. I à VII)

(N.B. — Les chiffres romains placés entre parenthèses renvoient à la bibliographie placée à la fin de cette note.)

L’algèbre commutative « abstraite » est de création récente, mais son développement ne peut se comprendre qu’en fonction de celui de la théorie des nombres algébriques et de la géométrie algébrique, qui lui ont donné naissance.

On a pu conjecturer sans trop d’invraisemblance que la fameuse « démonstration » que prétendait posséder Fermat de l’impossibilité de l’équation $ x^p + y^p = z^p $ pour $ p $ premier impair et $ x, y, z $ entiers $ \neq 0 $, aurait reposé sur la décomposition

$$
(x + y)(x + \zeta y) \ldots (x + \zeta^{p-1} y) = z^p
$$

dans l’anneau $ \mathbf{Z}[\zeta] $ (où $ \zeta \neq 1 $ est une racine $ p $-ème de l’unité), et sur un raisonnement de divisibilité dans cet anneau, en le supposant principal. On trouve en tout cas un raisonnement analogue ébauché chez Lagrange ((II), t. II, p. 531); c’est par des raisonnements de ce genre, avec diverses variantes (notamment des changements de variables destinés à abaisser le degré de l’équation) qu’Euler ((I), t. I, p. 488)(* ) et Gauss ((III), t. II, p. 387) démontrent le théorème de Fermat pour $ p = 3 $, Gauss (loc. cit.) et Dirichlet ((IV), t. I, p. 42) pour $ p = 5 $, et Dirichlet l’impossibilité de l’équation $ x^{14} + y^{14} = z^{14} $ ((IV), t. I, p. 190). Enfin, dans ses premières recherches sur la théorie des nombres, Kummer avait cru obtenir de cette façon une démonstration générale, et c’est sans doute cette erreur (qui lui fut signalée par Dirichlet) qui l’amena à ses études sur l’arithmétique des corps cyclotomiques, d’où il devait enfin réussir à déduire une version correcte de sa démonstration pour les nombres premiers $ p < 100 $ (VII d)).

D’un autre côté, le célèbre mémoire de Gauss de 1831 sur les résidus biquadratiques, dont les résultats sont déduits d’une étude détaillée

(*) Dans sa démonstration, Euler procède comme si $ \mathbf{Z}[\sqrt{-3}] $ était principal, ce qui n’est pas le cas; toutefois, son raisonnement peut être rendu correct par la considération du conducteur de $ \mathbf{Z}[\rho] $ ($ \rho $ racine cubique de l’unité) sur $ \mathbf{Z}[\sqrt{-3}] $ (cf. SOMMER, Introduction à la théorie des nombres algébriques (trad. A. Lévy), Paris (Hermann), 1911, p. 190).

de la divisibilité dans l’anneau $ \mathbf{Z}[i] $ des « entiers de Gauss » ((III), t. II, p. 109) montrait clairement l’intérêt que pouvait présenter pour les problèmes classiques de la théorie des nombres l’extension de la notion de divisibilité aux nombres algébriques(*); aussi n’est-il pas surprenant qu’entre 1830 et 1850 cette théorie ait fait l’objet de nombreux travaux des mathématiciens allemands, Jacobi, Dirichlet et Eisenstein d’abord, puis, un peu plus tard, Kummer et son élève et ami Kronecker. Nous n’avons pas à parler ici de la théorie des unités, trop particulière à la théorie des nombres, où les progrès sont rapides, Eisenstein obtenant la structure du groupe des unités pour les corps cubiques, Kronecker pour les corps cyclotomiques, peu avant que Dirichlet, en 1846 ((IV), t. I, p. 640) ne démontre le théorème général, auquel était presque parvenu de son côté Hermite ((VIII), t. I, p. 159). Beaucoup plus difficile apparaissait la question (centrale dans toute la théorie) de la décomposition en facteurs premiers. Depuis que Lagrange avait donné des exemples de nombres de la forme $ x^2 + Dy^2 $ ($ x, y, D $ entiers) ayant des diviseurs qui ne sont pas de la forme $ m^2 + Dn^2 $ ((II), t. II, p. 465), on savait en substance qu’il ne fallait pas s’attendre en général à ce que les anneaux $ \mathbf{Z}[\sqrt{-D}] $ fussent principaux, et à la témérité d’Euler avait succédé une grande circonspection; quand Dirichlet, par exemple, démontre que la relation $ p^2 - 5q^2 = r^5 $ ($ p, q, r $ entiers) équivaut à $ p + q\sqrt{5} = (x + y\sqrt{5})^5 $ pour $ x, y $ entiers, il se borne à signaler en note qu’« *il y a des théorèmes analogues pour beaucoup d’autres nombres premiers [que 5]* » ((IV), t. I, p. 31). Avec le mémoire de Gauss de 1831 et le travail d’Eisenstein sur les résidus cubiques (VIa)), on avait bien, il est vrai, des études poussées de l’arithmétique dans les anneaux principaux $ \mathbf{Z}[i] $ et $ \mathbf{Z}[\rho] $ ($ \rho = (-1 + i\sqrt{3})/2 $, racine cubique de l’unité) en parfaite analogie avec la théorie des entiers rationnels, et sur ces exemples au moins, le lien étroit entre l’arithmétique dans les corps quadratiques et la théorie des formes quadratiques binaires développée par Gauss était très apparent; mais il manquait pour le cas général un « dictionnaire » qui eût permis de traiter du corps quadratique par une simple traduction de la théorie de Gauss(†).

En fait, ce n’est pas pour les corps quadratiques, mais bien pour les corps cyclotomiques (et pour des raisons qui n’apparaîtront nettement que bien plus tard (cf. p. 119)) que l’énigme allait d’abord être résolue. Dès 1837, Kummer, analyste à ses débuts, se tourne vers l’arithmétique des corps cyclotomiques, qui ne va plus cesser de l’occuper de façon presque exclusive pendant 25 ans. Comme ses prédécesseurs, il étudie la divisibilité dans les anneaux $ \mathbf{Z}[\zeta] $, où $ \zeta $ est une racine $ p $-ème de l’unité

(*) Les recherches de Gauss sur la division de la lemniscate et les fonctions elliptiques liées à cette courbe, non publiées de son vivant, mais datant des environs de 1800, avaient dû l’amener dès cette époque à réfléchir sur les propriétés arithmétiques de l’anneau $ \mathbf{Z}[i] $, la division par les nombres de cet anneau jouant un rôle important dans la théorie; voir ce que dit à ce propos Jacobi ((V), t. VI, p. 275) ainsi que les calculs relatifs à ces questions trouvés dans les papiers de Gauss ((III), t. II, p. 411; voir aussi (III), t. X_2, p. 33 et suiv.)

(†) Le lecteur trouvera une description précise de cette correspondance entre formes quadratiques et corps quadratiques dans SOMMER, loc. cit., p. 205–229.

≠ 1 (p premier impair); il s’aperçoit vite que, là aussi, on rencontre des anneaux non principaux, bloquant tout progrès dans l’extension des lois de l’arithmétique (VII a)), et c’est seulement en 1845, au bout de 8 ans d’efforts, qu’apparaît enfin la lumière, grâce à sa définition des « nombres idéaux » (VII c) et d)).

Ce que fait Kummer revient exactement, en langage moderne, à définir les valuations sur le corps $ \mathbf{Q}(\zeta) $: elles sont en correspondance biunivoque avec ses « nombres premiers idéaux », l’« exposant » avec lequel un tel facteur figure dans la « décomposition » d’un nombre $ x \in \mathbf{Z}[\zeta] $ n’étant autre que la valeur en $ x $ de la valuation correspondante. Comme les conjugués de $ x $ appartiennent aussi à $ \mathbf{Z}[\zeta] $, et que leur produit $ N(x) $ (la « norme » de $ x(*) $) est un entier rationnel, les « facteurs premiers idéaux » à définir devaient aussi être « facteurs » des nombres premiers rationnels, et pour en donner la définition, on pouvait se borner à dire ce qu’étaient les « diviseurs premiers idéaux » d’un nombre premier $ q \in \mathbf{Z} $. Pour $ q = p $, Kummer avait déjà prouvé en substance (VII a)) que l’idéal principal $ (1 - \zeta) $ était premier et que sa puissance $ (p - 1)$-ème était l’idéal principal $ (p) $; ce cas ne soulevait donc aucun problème nouveau. Pour $ q \neq p $, l’idée qui semble avoir guidé Kummer est de remplacer l’équation cyclotomique $ \Phi_p(z) = 0 $ par la congruence $ \Phi_p(u) \equiv 0 $ (mod. $ q $), autrement dit de décomposer le polynôme cyclotomique $ \Phi_p(X) $ sur le corps $ \mathbf{F}_q $, et d’associer à chaque facteur irréductible de ce polynôme un « facteur premier idéal ». Un cas simple (explicitement cité dans la Note (VII b)) où Kummer annonce ses résultats sans démonstration) est celui où $ q \equiv 1 $ (mod. $ p $); si $ q = mp + 1 $ et si $ \gamma \in \mathbf{F}_q $ est une racine $ (q - 1)$-ème primitive de 1, on a, dans $ \mathbf{F}_q[X] $,

$$
\Phi_p(X) = \prod_{k=1}^{p-1} (X - \gamma^{km})
$$

puisque $ \gamma^{pm} = 1 $. Associant alors à chaque facteur $ X - \gamma^{km} $ un « facteur premier idéal » $ q_k $ de $ q $, Kummer dit qu’un élément $ x \in \mathbf{Z}[\zeta] $, dont P est le polynôme minimal sur $ \mathbf{Q} $, est divisible par $ q_k $ si dans $ \mathbf{F}_q $ on a $ P(\gamma^{km}) = 0 $; en somme, en langage moderne, il écrit l’anneau quotient $ \mathbf{Z}[\zeta]/q \mathbf{Z}[\zeta] $ comme composé direct de corps isomorphes à $ \mathbf{F}_q $. Pour $ q \not\equiv 1 $ (mod. $ p $), les facteurs irréductibles de $ \Phi_p(X) $ dans $ \mathbf{F}_q[X] $ ne sont plus du premier degré, et il faudrait donc substituer à $ X $ dans $ P(X) $ des

(*) La notion de norme d’un nombre algébrique remonte à Lagrange : si $ \alpha_i (1 \leq i \leq n) $ sont les racines d’un polynôme de degré $ n $, il considère même la « forme norme »

$$
N(x_0, x_1, \ldots, x_{n-1}) = \prod_{i=1}^n (x_0 + \alpha_i x_1 + \ldots + \alpha_i^{n-1} x_{n-1})
$$

en les variables $ x_i $, qui lui avait sans doute été suggérée par ses recherches sur la résolution des équations et les « résolvantes de Lagrange » ((II), t. VII, p. 170). Il est à noter que c’est la propriété multiplicative de la norme qui conduit Lagrange à son identité sur les formes quadratiques binaires, d’où Gauss devait tirer la « composition » de ces formes ((II), t. II, p. 522). D’autre part, lorsque la théorie des nombres algébriques débute aux environs de 1830, c’est très souvent sous forme de résolution d’équations $ N(x_0, \ldots, x_{n-1}) = \lambda $ (en particulier avec $ \lambda = 1 $ pour la recherche des unités) ou d’étude des « formes normes » (dites aussi « formes décomposables ») que sont présentés les problèmes ; et même dans des travaux récents, les propriétés de ces équations diophantiennes particulières sont utilisées avec fruit, notamment en théorie des nombres $ p $-adiques (Skolem, Chabauty).

racines « imaginaires de Galois » des facteurs de $ \Phi_p $ dans $ \mathbf{F}_q[X] $. Kummer évite cette difficulté en passant, comme nous dirions aujourd’hui, dans le corps de décomposition $ K $ de $ q $: si $ f $ est le plus petit entier tel que $ q^f \equiv 1 \pmod{p} $, et si l’on pose $ p - 1 = ef $, $ K $ n’est autre que le sous-corps de $ \mathbf{Q}(\zeta) $ formé des invariants du sous-groupe d’ordre $ f $ du groupe de Galois (cyclique d’ordre $ p - 1 $) de $ \mathbf{Q}(\zeta) $ sur $ \mathbf{Q} $; autrement dit c’est l’unique sous-corps de $ \mathbf{Q}(\zeta) $ qui soit de degré $ e $ sur $ \mathbf{Q} $; il était fort bien connu depuis les Disquisitiones de Gauss, étant engendré par les « périodes »

$$
\eta_k = \zeta_k + \zeta_{k+f} + \zeta_{k+2f} + \cdots + \zeta_{k+(e-1)f}
$$

$(0 \leq k \leq e-1,\ \zeta_v = \zeta^{g^v} $ où $ g $ est une racine primitive de la congruence $ z^{p-1} \equiv 1 \pmod{p} $), qui en forment une base normale. Si $ R(X) $ est le polynôme minimal (unitaire et à coefficients entiers rationnels) d’une quelconque de ces « périodes » $ \eta $, Kummer, se basant sur les formules de Gauss, prouve que, sur le corps $ \mathbf{F}_q $, $ R(X) $ se décompose encore en facteurs distincts du premier degré $ X - u_j (1 \leq j \leq e) $, et c’est à chacun des $ u_j $ qu’il associe cette fois un « facteur premier idéal » $ q_j $. Pour définir la « divisibilité par $ q_j $ », Kummer écrit tout $ x \in \mathbf{Z}[\zeta] $ sous la forme $ x = \sum_{k=0}^{f-1} \zeta^k y_k $, où chaque $ y_k \in K $ s’écrit lui-même d’une façon unique comme polynôme de degré $ \leq e-1 $ en $ \eta $, à coefficients entiers rationnels; il dit que $ x $ est divisible par $ q_j $ si et seulement si, lorsqu’on substitue $ u_j $ à $ \eta $ dans chacun des $ y_k $, les éléments de $ \mathbf{F}_q $ obtenus sont tous nuls. Mais il fallait encore définir l'« exposant » de $ q_j $ dans $ x $. Pour cela, Kummer introduit ce que nous appellerions maintenant une uniformisante pour $ q_j $, c’est-à-dire un élément $ \rho_j \in K $ tel que $ N(\rho_j) \equiv 0 \pmod{q} $, $ N(\rho_j) \not\equiv 0 \pmod{q^2} $, et enfin tel que $ \rho_j $ soit divisible par $ q_j $ (au sens défini ci-dessus) mais par aucun autre des facteurs idéaux $ \neq q_j $ de $ q $. L’existence d’un tel $ \rho_j $ avait en substance été prouvée par Kronecker dans sa dissertation l’année précédente ((IX a)), p. 23); posant alors $ \rho_j' = N(\rho_j)/\rho_j $, Kummer dit que l’exposant de $ q_j $ dans $ x $ est égal à $ h $ si l’on a $ x \rho_j'^h \equiv 0 \pmod{q^h} $, mais $ x \rho_j'^{h+1} \not\equiv 0 \pmod{q^{h+1}} $; il commence bien entendu par prouver que la relation $ x \rho_j' \equiv 0 \pmod{q} $ équivaut au fait que $ x $ est divisible par $ q_j $ (au sens antérieur). Une fois ces définitions posées, l’extension à $ \mathbf{Z}[\zeta] $ des lois usuelles de divisibilité pour les « nombres idéaux » n’offrait plus de difficulté sérieuse; et dès son premier mémoire (VII c)) Kummer put même, en utilisant la « méthode des tiroirs » de Dirichlet, démontrer que les « classes » de « facteurs idéaux » étaient en nombre fini(*).

Nous ne poursuivrons pas l’histoire des travaux ultérieurs de Kummer sur les corps cyclotomiques, en ce qui concerne la détermination du

(*) Il ne fait d’ailleurs en cela que reprendre un raisonnement de Kronecker dans sa dissertation, relatif aux classes de solutions d’équations de la forme $ N(x_0, x_1, \ldots, x_{n-1}) = a $ ((IX a)), p. 25). D’autre part, Kummer fait plusieurs fois allusion à des résultats qu’aurait obtenus Dirichlet sur des équations de ce type (pour un corps de nombres algébriques quelconque); mais ces résultats n’ont été ni publiés, ni retrouvés dans les papiers de Dirichlet.

nombre de classes et l’application à la démonstration du théorème de Fermat dans divers cas. Mentionnons seulement la manière dont, en 1859, il étend sa méthode pour obtenir (au moins partiellement) les « nombres premiers idéaux » dans un « corps kummerien » $ \mathbf{Q}(\zeta, \mu) $, où $ \mu $ est une racine d’un polynôme irréductible $ P(X) = X^p - \alpha $, avec $ \alpha \in \mathbf{Z}[\zeta] $ (VII e)). Il est intéressant que Kummer envisage le problème en considérant précisément $ \mathbf{Q}(\zeta, \mu) $ comme une extension cyclique du corps $ \mathbf{Q}(\zeta) $ pris comme « corps de base »(*): il part d’un « nombre premier idéal » q de $ \mathbf{Z}[\zeta] $, qu’il suppose ne pas diviser $ p $ ni $ \alpha $, et cette fois, il examine (en termes modernes) le polynôme $ \bar{P}(X) = X^p - \bar{\alpha} $ dans le corps résiduel $ k $ de la valuation de $ \mathbf{Q}(\zeta) $ correspondant à q ($ \bar{\alpha} $ étant l’image canonique de $ \alpha $ dans $ k $). Comme $ \mathbf{Q}(\zeta) $ est le corps des racines $ p $-èmes de l’unité, $ \bar{P} $ est, soit irréductible sur $ k $, soit produit de facteurs du premier degré. Dans le premier cas, Kummer dit que q reste premier dans $ \mathbf{Z}[\zeta, \mu] $; dans le second, il introduit des éléments $ w_i $ ($ 1 \leq i \leq p $) de $ \mathbf{Z}[\zeta] $ dont les images dans $ k $ sont les racines de $ \bar{P} $, et il associe à chaque indice $ i $ un facteur premier idéal $ r_i $ de q; posant ensuite $ W_i(X) = \prod_{j \neq i} (X - w_j) $, il dit que, pour un polynôme $ f $ à coefficients dans $ \mathbf{Z}[\zeta], f(\mu) $ contient $ m $ fois le facteur idéal $ r_i $ si l’on a
$$
f(w_i) W_i^m(w_i) \equiv 0 \pmod{q^m}
$$
mais
$$
f(w_i) W_i^{m+1}(w_i) \not\equiv 0 \pmod{q^{m+1}}.
$$
En somme, il obtient de cette façon les valuations de $ \mathbf{Q}(\zeta, \mu) $ non ramifiées sur $ \mathbf{Q} $, ce qui lui suffit pour les applications qu’il a en vue.

\*

**

Kummer avait eu la chance de rencontrer, dans l’étude des corps particuliers auxquels ses recherches sur le théorème de Fermat l’avaient conduit d’abord, nombre de circonstances fortuites qui en rendaient l’étude beaucoup plus abordable. L’extension au cas général des résultats de Kummer présentait de redoutables difficultés et allait coûter des années d’efforts.

Avec Kronecker et Dedekind, qui y tiennent les rôles principaux, l’histoire de la théorie des nombres algébriques, pendant les 40 années qui suivent la découverte de Kummer, n’est pas sans rappeler (mais heureusement sans le même caractère d’acrimonie) celle de la rivalité de Newton et de Leibniz 180 ans plus tôt, autour de l’invention du Calcul infinitésimal. Elève et bientôt collègue de Kummer à Berlin, Kronecker

(*) Dans son mémoire sur les formes quadratiques à coefficients dans l’anneau des entiers de Gauss ((IV), t. I, p. 533–618) Dirichlet avait, à divers endroits, été amené à considérer la norme relative du corps $ \mathbf{Q}(\sqrt{D}, i) $ sur son sous-corps quadratique $ \mathbf{Q}(\sqrt{D}) $. De même, Eisenstein, étudiant les racines 8-èmes de l’unité, considère le corps qu’elles engendrent comme extension quadratique de $ \mathbf{Q}(i) $ et utilise la norme relative à ce sous-corps ((VI b)), p. 253). Mais le travail de Kummer est le premier exemple d’étude arithmétique approfondie d’un « corps relatif ».

(dont la thèse, comme nous l’avons vu, avait servi à Kummer pour un point essentiel de sa théorie) s’intéressait de très près aux « nombres idéaux » dans le dessein de les appliquer à ses propres recherches ; et nous admirons son étonnante pénétration lorsque nous le voyons, dès 1853 ((IX b)), p. 10), énoncer le théorème général sur la structure des extensions abéliennes de $ \mathbf{Q} $, et, ce qui est peut-être plus remarquable encore, créer, dans les années qui suivent, la théorie de la multiplication complexe et découvrir le premier germe de la théorie du corps de classes (IX c) et d)). Une lettre de Kronecker à Dirichlet, en 1857 ((IX), t. V, p. 418–421), le montre déjà, à cette époque, en possession d’une généralisation de la théorie de Kummer, ce que confirme d’ailleurs Kummer lui-même dans un de ses propres travaux ((VII e)), p. 57), et Kronecker fera mainte fois allusion à cette théorie dans ses mémoires entre 1860 et 1880(*).

Mais bien qu’à cette époque aucun des mathématiciens de l’école allemande de Théorie des nombres n’ignorât l’existence de ces travaux de Kronecker, ce dernier ne semble avoir communiqué les principes de ses méthodes qu’à un cercle restreint d’amis et d’élèves, et lorsqu’il se décide enfin à les publier, dans son mémoire de 1881 sur le discriminant (IX e)) et surtout dans son grand « Festschrift » de 1882 (IX f)), Dedekind ne peut s’empêcher d’exprimer sa surprise ((X), t. III, p. 427), ayant imaginé de tout autres procédés d’après les échos qu’il en avait eus ((X), t. III, p. 287). Kronecker était d’ailleurs loin de posséder au même degré les remarquables dons d’exposition et de clarté de Dedekind, et il n’est donc pas étonnant que ce soient surtout les méthodes de ce dernier, publiées dès 1871, qui aient formé l’armature de la théorie des nombres algébriques ; pour intéressante qu’elle soit, la méthode d’« adjonction d’indéterminées » de Kronecker, en ce qui concerne la Théorie des nombres, n’est plus guère à nos yeux qu’une variante de celle de Dedekind (cf. chap. VII, § 1, exerc. 31) et c’est surtout dans une autre direction, orientée vers la Géométrie algébrique, que les idées de Kronecker acquièrent toute leur importance pour l’histoire de l’Algèbre commutative, comme nous le verrons plus loin.

Pour des raisons qui ne pouvaient apparaître clairement que beaucoup plus tard, un premier préalable à tout essai de théorie générale était bien entendu la clarification de la notion d’entier algébrique. Celle-ci est acquise vers 1845–50, bien qu’il soit assez difficile de dater son apparition de façon précise ; il paraît vraisemblable que c’est l’idée de système stable par addition et multiplication (ou, plus précisément, ce que nous appelons maintenant une $ \mathbf{Z}$-algèbre de rang fini) qui, plus ou moins consciemment, ait conduit à la définition générale des entiers algébriques : on tombe en effet inévitablement sur cette définition quand on impose à une $ \mathbf{Z}$-algèbre de la forme $ \mathbf{Z}[\theta] $ d’être de rang fini, par analogie avec l’anneau $ \mathbf{Z}[\zeta] $ engendré par une racine de l’unité, qui était au centre des préoccupations des arithméticiens de cette époque. Toujours est-il que lorsque, de façon indépendante, Dirichlet ((IV), t. I,

(*) Sur l’évolution de ses idées sur ce sujet, voir la très intéressante introduction de son mémoire de 1881 sur le discriminant ((IX e)), p. 195).

p. 640), Hermite ((VIII), t. I, p. 115 et 146) et Eisenstein ((VIc)), p. 236) introduisent la notion d’entier algébrique, ils n’ont pas l’air de considérer qu’il s’agisse d’une idée nouvelle ni de juger qu’il soit utile d’en faire une étude détaillée; seul Eisenstein démontre en substance (loc. cit.) que la somme et le produit de deux entiers algébriques sont des entiers algébriques, sans prétendre d’ailleurs que ce résultat soit original.

Un point beaucoup plus caché était la détermination des anneaux dans lesquels on pouvait espérer généraliser la théorie de Kummer. Ce dernier, dans sa première note (VII b)), n’hésite pas à affirmer qu’il peut retrouver par sa méthode la théorie des formes quadratiques binaires de Gauss en considérant les anneaux $ \mathbf{Z}[\sqrt{D}] $ (D entier); il ne développa jamais cette idée, mais il semble bien que ni lui, ni personne avant Dedekind ne se soit aperçu que la décomposition unique en facteurs premiers « idéaux » n’est pas possible dans les anneaux $ \mathbf{Z}[\sqrt{D}] $ lorsque $ D \equiv 1 $ (mod. 4) (bien que l’exemple des racines cubiques de l’unité montrât que l’anneau $ \mathbf{Z}[\rho] $ considéré depuis Gauss est distinct de $ \mathbf{Z}[\sqrt{-3}] $)(*). Avant Dedekind et Kronecker, les seuls anneaux étudiés sont toujours du type $ \mathbf{Z}[\theta] $ ou parfois certains anneaux particuliers du type $ \mathbf{Z}[\theta, \theta'] $ (†). En ce qui concerne Kronecker, il est possible que l’idée de considérer l’anneau de tous les entiers d’une extension algébrique lui ait d’abord été suggérée par l’étude des corps de fonctions algébriques, où cet anneau s’introduit de façon naturelle comme l’ensemble des fonctions « finies à distance finie »; il insiste en tout cas dans son mémoire de 1881 sur le discriminant (écrit et annoncé à l’Académie de Berlin dès 1862) sur cette caractérisation des « entiers » dans ces corps (IX e)). Dedekind ne donne pas d’indication quant à l’origine de ses propres idées sur ce point, mais dès ses premières publications sur les corps de nombres en 1871, l’anneau de tous les entiers d’un tel corps joue un rôle capital dans sa théorie; c’est aussi Dedekind qui clarifie le rapport entre un tel anneau et ses sous-anneaux ayant même corps des fractions, par l’introduction de la notion de conducteur (X c)).

Mais là n’était pas la seule difficulté. Pour généraliser les idées de Kummer, il fallait d’abord se débarrasser du passage par le corps de décomposition, qui ne pouvait naturellement avoir d’analogue dans le cas d’un corps non abélien. Ce détour paraît d’ailleurs à première vue très surprenant et artificiel, car si l’on part du polynôme irréductible $ \Phi_p(X) $ de $ \mathbf{Z}[X] $, on se demande pourquoi Kummer ne pousse pas jusqu’au bout les conséquences logiques de ses idées, et ce qui l’empêche de se servir de la théorie des « imaginaires de Galois », bien connue à cette époque. L’obstacle apparaît plus clairement à la lumière d’une tentative

(*) Bien que Kronecker ait dû être amené à étudier l’arithmétique des anneaux $ \mathbf{Z}[\sqrt{-D}] $ ($ D > 0 $) par ses travaux sur la multiplication complexe, il n’a rien publié à ce sujet, et la caractérisation des entiers d’un corps quadratique quelconque $ \mathbf{Q}(\sqrt{D}) $ est donnée explicitement pour la première fois par Dedekind en 1871 ((X c)), p. 105–106).

(†) On a vu plus haut l’exemple de l’anneau $ \mathbf{Z}[\zeta, \mu] $ introduit par Kummer (VII e)). Auparavant, Eisenstein avait été amené à envisager un sous-anneau engendré par deux éléments de l’anneau des entiers dans le corps des racines 21-èmes de l’unité (VI b)).

malheureuse de généralisation faite dès 1865 par Selling, un élève de Dedekind : étant donné un polynôme irréductible $ P \in \mathbf{Z}[X] $, Selling décompose le polynôme correspondant $ \bar{P}(X) $ en facteurs irréductibles dans $ F_q[X] $; les racines de ce polynôme appartiennent donc à une extension finie $ F_r $ de $ F_q $; mais Selling, pour définir à la façon de Kummer l’exposant d’un « facteur premier idéal » de $ q $ dans un entier du corps des racines de $ P(X) $, n’hésite pas à parler *dans le corps* $ F_r $ de congruences modulo une *puissance de q* ((XI), p. 26); et un peu plus loin, lorsqu’il essaie d’aborder la question de la ramification, il « adjoint » à $ F_r $ des « racines imaginaires » d’une équation de la forme $ x^h = q $ ((XI), p. 34). Il est clair que ces hardiesses (qui se justifieraient en remplaçant le corps fini $ F_q $ par le corps $ q $-adique) ne pouvaient à cette époque aboutir qu’à des non-sens. Heureusement, Dedekind venait en 1857 (X a)), sous le nom de « théorie des congruences supérieures », de reprendre sous une autre forme la théorie des corps finis(*): il interprète les éléments de ces derniers comme « restes » des polynômes de $ \mathbf{Z}[X] $ suivant un « double module » formé des combinaisons linéaires, à coefficients dans $ \mathbf{Z}[X] $, d’un nombre premier $ p $ et d’un polynôme unitaire irréductible $ P \in \mathbf{Z}[X] $ (ce qui est sans doute pour lui, comme pour Kronecker, à l’origine de l’idée générale de *module* à laquelle ils vont aboutir indépendamment un peu plus tard). À son propre témoignage ((X d)), p. 218) il semble que Dedekind ait commencé par attaquer le problème des « facteurs idéaux » de $ p $ dans un corps $ \mathbf{Q}(\xi) $, où $ P \in \mathbf{Z}[X] $ est le polynôme minimal de $ \xi $, de la façon suivante (tout au moins dans le cas « non ramifié », c’est-à-dire lorsque dans $ F_p[X] $ le polynôme $ \bar{P} $ correspondant à $ P $ n’a pas de racine multiple): on écrit, dans $ \mathbf{Z}[X] $,

$$
P = P_1 P_2 \ldots P_h + p \cdot G
$$

où les $ \bar{P}_i $ sont irréductibles et distincts dans $ F_p[X] $; on peut supposer que $ G $ n’est divisible (dans $ \mathbf{Z}[X] $) par aucun des $ P_i $, et pour tout $ i $, on pose $ W_i = \prod_{j \neq i} P_j $; alors, si $ f \in \mathbf{Z}[X] $, on dira que $ f(\xi) $ contient $ k $ fois le « facteur idéal » $ p_i $ de $ p $ correspondant à $ P_i $ si l’on a

$$
f W_i^k \equiv 0 \pmod{p^k, P}
$$

et

$$
f W_i^{k+1} \not\equiv 0 \pmod{p^{k+1}, P}.
$$

La parenté avec la méthode suivie par Kummer pour les « corps kummeriens » est ici manifeste, et l’on peut également, de cette façon, rejoindre aisément la définition initiale de Kummer pour les corps cyclotomiques (voir par exemple le travail de Zolotareff (XIV) qui, d’abord indépendamment de Dedekind, développe ces idées un peu plus tard).

(*) On sait que certains résultats de cette théorie, publiés d’abord par Galois, avaient été obtenus (dans le langage des congruences) par Gauss vers 1800; après la mort de Gauss, Dedekind s’était chargé de la publication d’une partie de ses œuvres et avait en particulier retrouvé dans les papiers laissés par Gauss le mémoire sur les corps finis ((III), t. II, p. 212–240).

Toutefois, ni Dedekind, ni Kronecker qui paraît avoir aussi fait des essais analogues, ne devaient poursuivre plus avant dans cette voie, arrêtés l’un et l’autre par les difficultés présentées par la ramification ((X d)), p. 218 et (IX f)), p. 325)(*). Si l’anneau des entiers A du corps de nombres K que l’on considère admet une base (sur Z) formée des puissances d’un même entier θ, il n’est pas difficile de généraliser la méthode précédente pour les nombres premiers ramifiés dans Z[θ] (comme l’indique Zolotareff (loc. cit.)). Mais il y a des corps K où aucune base de ce type n’existe dans l’anneau A; et Dedekind finit même par découvrir qu’il y a des cas où certains nombres premiers p (les « facteurs extraordinaires du discriminant » du corps K) sont tels que, quel que soit θ ∈ A, l’application de la méthode précédente au polynôme minimal de θ sur Q conduirait à attribuer à p des facteurs idéaux multiples alors qu’en fait p ne se ramifie pas dans A(†); il avoue avoir été longtemps arrêté par cette difficulté imprévue, avant de parvenir à la surmonter en créant de toutes pièces la théorie des modules et des idéaux, exposée de façon magistrale (et déjà toute moderne, contrastant avec le style discursif de ses contemporains) dans ce qui est sans doute son chef-d’oeuvre, le fameux « XIe supplément » au livre de Dirichlet sur la Théorie des nombres (Xf)). Cet ouvrage connaîtra trois versions successives, mais dès la première (publiée comme « Xe supplément » à la seconde édition du livre de Dirichlet en 1871 (IV bis)) l’essentiel de la méthode est déjà acquis, et presque d’un seul coup la théorie des nombres algébriques passe des ébauches et des tâtonnements antérieurs à une discipline en pleine maturité et déjà en possession de ses outils essentiels : dès le début, l’anneau de tous les entiers d’un corps de nombres est placé au centre de la théorie; Dedekind prouve l’existence d’une base de cet anneau sur Z, et en déduit la définition du discriminant du corps, comme carré du déterminant formé des éléments d’une base de l’anneau des entiers et de leurs conjugués ; il ne donne toutefois dans le XIe supplément la caractérisation des nombres premiers ramifiés (comme facteurs premiers du discriminant) que pour les corps quadratiques ((X f)), p. 202), alors qu’il était en possession du théorème général depuis 1871(‡). Le résultat central de l’ouvrage est le théorème d’existence et d’unicité de la décomposition des idéaux en facteurs premiers, pour lequel Dedekind commence par développer une théorie élémentaire des « modules »; en fait, dans le XIe supplément, il réserve ce nom aux sous-Z-modules d’un corps de nombres, mais la conception qu’il s’en forme et les résultats qu’il démontre sont déjà exposés de façon immédiatement

(*) Zolotareff tourne la difficulté par un raffinement de sa méthode, qui ne paraît plus guère présenter qu’un intérêt anecdotique (XIV).

(†) Kronecker dit avoir rencontré le même phénomène dans un sous-corps du corps des racines 13èmes de l’unité, qu’il ne précise d’ailleurs pas ((IX f)), p. 384). L’exemple de facteur extraordinaire du discriminant donné par Dedekind est traité en détail dans HASSE, Zahlentheorie (Berlin, Akad. Verlag, 1949), p. 333 ; un peu plus loin, Hasse donne un exemple de corps K où il n’y a pas de facteur extraordinaire du discriminant, mais où il n’existe aucun θ ∈ A tel que A = Z[θ] (loc. cit., p. 335).

(‡) Il ne publia la démonstration de ce théorème que dans son mémoire de 1882 sur la différente (X e)).

applicables aux modules les plus généraux(*); il faut noter entre autres, dès 1871, l’introduction de la notion de « transporteur » qui joue un rôle important (ainsi d’ailleurs que la « condition des chaînes ascendantes ») dans la première démonstration du théorème d’unique factorisation. Dans les deux éditions suivantes, Dedekind devait encore donner deux autres démonstrations de ce théorème, qu’il considérait à juste titre comme la pierre angulaire de sa théorie. Il faut noter ici que c’est dans la troisième démonstration qu’interviennent les idéaux fractionnaires (déjà introduits par Kummer dès 1859 pour les corps cyclotomiques) et le fait qu’ils forment un groupe; nous reviendrons plus loin sur la seconde démonstration (p. 127).

Tous ces résultats (au langage près) étaient sans doute déjà connus de Kronecker vers 1860 comme cas particuliers de ses conceptions plus générales dont nous parlons plus bas (alors que Dedekind reconnaît n’avoir surmonté les dernières difficultés de sa théorie qu’en 1869–70 ((X e)), p. 351))(†); en ce qui concerne les corps de nombres, il faut en particulier souligner que, dès cette époque, Kronecker savait que toute la théorie est applicable sans changement essentiel quand on part d’un « corps de base » $ k $ qui est lui-même un corps de nombres (autre que $ \mathbf{Q} $), point de vue auquel conduisait naturellement la théorie de la multiplication complexe; il avait ainsi reconnu, pour certains corps $ k $, l’existence d’extensions algébriques $ K \neq k $ non ramifiées sur $ k $ ((IX f)), p. 269) ce qui ne peut pas se produire pour $ k = \mathbf{Q} $ (comme il résulte de minorations de Hermite et Minkowski pour le discriminant). Dedekind ne devait jamais développer ce dernier point de vue (bien qu’il en indique la possibilité dans son mémoire de 1882 sur la différente), et le premier exposé systématique de la théorie du « corps relatif » est dû à Hilbert (XVI d)).

Enfin, en 1882 (X e)), Dedekind complète la théorie par l’introduction de la différente, qui lui donne une nouvelle définition du discriminant et lui permet de préciser les exposants des facteurs premiers idéaux dans la décomposition de ce dernier. C’est aussi vers cette époque qu’il s’intéresse aux particularités présentées par les extensions galoisiennes, introduisant les notions de groupe de décomposition et de groupe d’inertie (dans un mémoire (X g)) qui ne fut publié qu’en 1894), et même (dans des papiers non publiés de son vivant ((X), t. II, p. 410–411)) une ébauche des groupes de ramification, que Hilbert (indépendamment de Dedekind) développera un peu plus tard (XVI c) et d)).

Ainsi, vers 1895, la théorie des nombres algébriques a terminé la première étape de son développement; les outils forgés au cours de cette période de formation vont lui permettre d’aborder presque aussitôt l’étape suivante, la théorie générale du corps de classes (ou, ce qui

(*) Dans son mémoire de 1882 sur les courbes algébriques (en commun avec H. Weber) (X bis), il utilise de la même manière la théorie des modules sur l’anneau $ \mathbf{C}[X] $.

(†) Kronecker n’avait toutefois pas réussi à obtenir par ses méthodes la caractérisation complète des idéaux ramifiés dans le cas des corps de nombres. Par contre, il a cette caractérisation pour les corps de fonctions algébriques d’une variable, et prouve en outre que dans ce cas il n’y a pas de « facteur extraordinaire » du discriminant (IX e)).

revient au même, la théorie des extensions abéliennes des corps de nombres) qui se poursuit jusqu’à nos jours et que nous n’avons pas à décrire ici. Du point de vue de l’Algèbre commutative, on peut dire qu’à la même époque la théorie des anneaux de Dedekind est pratiquement achevée, mises à part leur caractérisation axiomatique, ainsi que la structure des modules de type fini sur ces anneaux (qui, pour le cas des corps de nombres, sera seulement élucidée en substance par Steinitz en 1912 (XX b))(*).

\* \* \*

Les progrès ultérieurs de l’Algèbre commutative vont surtout provenir de problèmes assez différents, issus de la Géométrie algébrique (qui d’ailleurs influencera de façon directe la Théorie des nombres, même avant les développements « abstraits » de l’époque contemporaine).

Nous n’avons pas ici à faire l’histoire détaillée de la Géométrie algébrique, qui, jusqu’à la mort de Riemann, ne touche guère notre sujet. Qu’il suffise de rappeler qu’elle avait surtout pour but l’étude des courbes algébriques dans le plan projectif complexe, abordée le plus souvent par les méthodes de la géométrie projective (avec ou sans usage de coordonnées). Parallèlement s’était développée, avec Abel, Jacobi, Weierstrass et Riemann, la théorie des « fonctions algébriques » d’une variable complexe et de leurs intégrales ; on était évidemment conscient du lien entre cette théorie et la géométrie des courbes algébriques planes, et on savait à l’occasion « appliquer l’Analyse à la Géométrie » ; mais les méthodes utilisées pour l’étude des fonctions algébriques étaient surtout de nature « transcendante », même avant Riemann(†) ; ce caractère s’accentue encore dans les travaux de ce dernier, avec l’introduction des « surfaces de Riemann » et des fonctions analytiques quelconques définies sur une telle surface. Presque aussitôt après la mort de Riemann, Roch, et surtout Clebsch, reconnurent la possibilité de tirer des profonds résultats obtenus par les méthodes transcendantes de Riemann de nombreuses et frappantes applications à la géométrie projective des courbes, ce qui devait naturellement inciter les géomètres contemporains à donner de ces résultats des démonstrations purement « géométriques » ; ce programme, incomplètement suivi par Clebsch et Gordan, fut

(*) Un début d’étude des modules sur un anneau d’entiers algébriques avait déjà été amorcé par Dedekind (X h)).

(†) Il faut noter toutefois que Weierstrass, dans ses recherches sur les fonctions abéliennes (qui remontent à 1857 mais ne furent exposées dans ses cours que vers 1865 et publiées seulement dans ses Oeuvres complètes ((XVII), t. IV)), donne, au contraire de Riemann, une définition purement algébrique du genre d’une courbe, comme le plus petit entier $ p $ tel qu’il y ait des fonctions rationnelles sur la courbe ayant des pôles en $ p + 1 $ points arbitraires donnés. Il est intéressant de signaler que, cherchant à obtenir des éléments qui lui tiennent lieu de fonctions n’ayant qu’un seul pôle sur la courbe, Weierstrass, avant d’utiliser finalement à cet effet des fonctions transcendantes, avait, au témoignage de Kronecker ((IX e)), p. 197), incité ce dernier à étendre aux fonctions algébriques d’une variable les résultats qu’il venait à cette époque d’obtenir sur les corps de nombres (les « facteurs premiers idéaux » jouant effectivement le rôle désiré par Weierstrass).

accompli par Brill et M. Noether quelques années plus tard (XIII), à l’aide de l’étude des systèmes de points variables sur une courbe donnée et des courbes auxiliaires (les « adjectives ») passant par de tels systèmes de points. Mais même pour les contemporains, les méthodes transcendentantes de Riemann (et notamment son usage de notions topologiques et du « principe de Dirichlet ») paraissaient reposer sur des fondements incertains; et bien que Brill et Noether soient plutôt plus soigneux que la plupart des géomètres « synthétiques » contemporains (voir plus loin p. 126), leurs raisonnements géométrico-analytiques ne sont pas à l’abri de tout reproche. C’est essentiellement pour donner à la théorie des courbes algébriques planes une base solide que Dedekind et Weber publient en 1882 leur grand mémoire sur ce sujet (X bis): « Les recherches publiées ci-dessous », disent-ils, « ont pour but de poser les fondements de la théorie des fonctions algébriques d’une variable, une des créations principales de Riemann, d’une façon à la fois simple, rigoureuse et entièrement générale. Dans les recherches antérieures sur ce sujet, on fait en général des hypothèses restrictives sur les singularités des fonctions considérées, et les soi-disant cas d’exception sont, ou bien mentionnés en passant comme des cas limites, ou bien entièrement négligés. De même, on admet certains théorèmes fondamentaux sur la continuité ou l’analyticité, dont l’« évidence » s’appuie sur des intuitions géométriques de nature variée » ((X bis), p. 181)(*). L’idée essentielle de leur travail est de calquer la théorie des fonctions algébriques d’une variable sur la théorie des nombres algébriques telle que venait de la développer Dedekind; pour ce faire, ils doivent d’abord se placer au point de vue « affine » (au contraire de leurs contemporains, qui considéraient invariablement les courbes algébriques comme plongées dans l’espace projectif complexe): ils partent donc d’une extension algébrique finie K du corps C(X) des fractions rationnelles, et de l’anneau A des « fonctions algébriques entières » dans K, i.e. des éléments de ce corps entiers sur l’anneau C[X] des polynômes; leur résultat fondamental, qu’ils obtiennent sans utiliser aucune considération topologique(†), est que A est un anneau de Dedekind, auquel s’appliquent mutatis mutandis (et même, comme le remarquent Dedekind et Weber sans en voir encore clairement la raison ((X), t. I. p. 268), d’une façon plus simple) tous les résultats du « XIe supplément ». Cela fait, ils prouvent que leurs théorèmes sont

(*) On sait que, malgré les efforts de Dedekind, Weber et Kronecker, le relâchement dans la conception de ce qui constituait une démonstration correcte, déjà sensible dans l’école allemande de Géométrie algébrique des années 1870–1880, ne devait que s’aggraver de plus en plus dans les travaux des géomètres français et surtout italiens des deux générations suivantes, qui, à la suite des géomètres allemands, et en développant leurs méthodes, s’attaquent à la théorie des surfaces algébriques: « scandale » mainte fois dénoncé (surtout à partir de 1920) par les algébristes, mais que n’étaient pas sans justifier en une certaine mesure les brillants succès obtenus par ces méthodes « non rigoureuses », contrastant avec le fait que, jusque vers 1940, les successeurs orthodoxes de Dedekind s’étaient révélés incapables de formuler avec assez de souplesse et de puissance les notions algébriques qui eussent permis de donner de ces résultats des démonstrations correctes.

(†) Ils soulignent que, grâce à ce fait, tous leurs résultats resteraient valables en remplaçant le corps C par le corps de tous les nombres algébriques ((X), t. I, p. 240).

en fait birationnellement invariants (autrement dit, ne dépendent que du corps K) et en particulier ne dépendent pas du choix de la « droite à l’infini » fait au départ. Ce qui est sans doute encore plus intéressant pour nous, c’est que, voulant définir les points de la « surface de Riemann » correspondant à K (et en particulier les « points à l’infini », qui ne pouvaient correspondre à des idéaux de A), ils sont amenés à introduire la notion de place du corps K : ils se trouvent devant la situation que retrouvera Gelfand en 1940 pour fonder la théorie des algèbres normées, savoir un ensemble K d’éléments qui ne sont pas donnés à l’avance comme fonctions, mais que pourtant on veut pouvoir considérer comme telles ; et, pour obtenir l’ensemble de définition de ces fonctions hypothétiques, ils ont pour la première fois l’idée (que reprendra Gelfand, et qui est devenue banale à force d’être utilisée à tout propos dans la mathématique moderne) d’associer à un point x d’un ensemble E et à un ensemble $ \mathcal{F} $ d’applications de E dans un ensemble G l’application $ f \to f(x) $ de $ \mathcal{F} $ dans G, autrement dit de considérer, dans l’expression $ f(x) $, $ f $ comme variable et $ x $ comme fixe, au rebours de la tradition classique. Enfin, ils n’ont pas de peine, à partir de la notion de place, à définir les « diviseurs positifs » (« Polygone » dans leur terminologie) qui comprennent les idéaux de A comme cas particuliers et correspondent aux « systèmes de points » de Brill et Noether ; mais, bien qu’ils écrivent les diviseurs principaux et les diviseurs de différentielles comme « quotients » de diviseurs positifs, ils ne donnent pas la définition générale des diviseurs, et c’est seulement en 1902 que Hensel et Landsberg introduiront, par analogie avec les idéaux fractionnaires, cette notion qui embarrasse toujours les tenants des méthodes purement « géométriques » (obligés malgré eux de les définir sous le nom de « systèmes virtuels », mais gênés de ne pouvoir leur donner une interprétation « concrète »).

La même année 1882 voit aussi paraître le grand mémoire de Kronecker attendu depuis plus de 20 ans (IX f)). Beaucoup plus ambitieux que le travail de Dedekind–Weber, il est malheureusement aussi beaucoup plus vague et plus obscur. Son thème central est (en langage moderne) l’étude des idéaux d’une algèbre finie intègre sur un des anneaux de polynômes $ \mathbf{C}[X_1, \ldots, X_n] $ ou $ \mathbf{Z}[X_1, \ldots, X_n] $; Kronecker se limite $ a $ priori à ceux de ces idéaux qui sont de type fini (le fait qu’ils le sont tous devait seulement être prouvé (pour les idéaux de $ \mathbf{C}[X_1, \ldots, X_n] $) quelques années plus tard par Hilbert au cours de ses travaux sur les invariants (XVI a))). En ce qui concerne $ \mathbf{C}[X_1, \ldots, X_n] $ ou $ \mathbf{Z}[X_1, \ldots, X_n] $, on était naturellement amené à associer à tout idéal de l’un de ces anneaux la « variété algébrique » formée par les zéros communs à tous les éléments de l’idéal ; et les études de géométrie en dimensions 2 et 3 faites au cours du XIXe siècle devaient conduire intuitivement à l’idée que toute variété est réunion de variétés « irréductibles » en nombre fini dont les « dimensions » ne sont pas nécessairement les mêmes. Il semble que la démonstration de ce fait soit le but que se propose Kronecker, bien qu’il ne le dise explicitement nulle part, et qu’on ne puisse trouver dans son mémoire aucune définition de « variété irréductible » ni de « dimension ». En fait, il se borne à indiquer sommairement comment une méthode générale d’élimination(*) donne, à partir d’un système de générateurs de l’idéal considéré, un nombre fini de variétés algébriques, pour chacune desquelles, dans un système de coordonnées convenable, un certain nombre de coordonnées sont arbitraires et les autres en sont des « fonctions algébriques »(†). Mais, si c’est vraiment la décomposition en variétés irréductibles que vise Kronecker, force est de reconnaître qu’il n’y arrive que dans le cas élémentaire d’un idéal principal, où il prouve en substance, en étendant un lemme classique de Gauss sur $ \mathbf{Z}[X] $ ((III), t. I, p. 34), que les anneaux $ \mathbf{C}[X_1, \ldots, X_n] $ et $ \mathbf{Z}[X_1, \ldots, X_n] $ sont factoriels; et, dans le cas général, on peut même se demander si Kronecker était en possession de la notion d’idéal premier (ce qu’il appelle « Primmodulsystem » est un idéal indécomposable en produit de deux autres ((IX f)), p. 336); cela est d’autant plus étonnant que la définition donnée depuis 1871 par Dedekind était parfaitement générale).

Il faut dire toutefois que la méthode d’élimination de Kronecker, convenablement appliquée, conduit bien à la décomposition d’une variété algébrique en ses composantes irréductibles: c’est ce qui est clairement établi par E. Lasker au début de son grand mémoire de 1905 sur les idéaux de polynômes (XIX); il définit correctement la notion de variété irréductible (dans $ \mathbf{C}^n $) comme une variété algébrique V telle qu’un produit de deux polynômes ne puisse s’annuler dans toute la variété V que si l’un d’eux s’y annule, et il a aussi une définition de la dimension indépendante des axes choisis. Dans les intéressantes considérations historiques qu’il insère dans ce travail, Lasker indique d’autre part qu’il se rattache, non seulement à la tendance purement algébrique de Kronecker et Dedekind, mais aussi aux problèmes soulevés par les méthodes géométriques de l’école de Clebsch et M. Noether, et notamment au fameux théorème démontré par ce dernier en 1873 (XII). Il s’agit essentiellement, comme nous dirions aujourd’hui, de la détermination de l’idéal $ \alpha $ des polynômes de $ \mathbf{C}[X_1, \ldots, X_n] $ qui s’annulent aux points d’un ensemble donné M dans $ \mathbf{C}^n $; le plus souvent, M était la « variété algébrique » des zéros communs à des polynômes $ f_i $ en nombre fini, et pendant longtemps il semble que l’on ait admis (bien entendu sans justification) que, tout au moins pour $ n = 2 $ ou $ n = 3 $, l’idéal $ \alpha $ était tout bonnement engendré par les $ f_i $(‡); M. Noether

(*) Par un changement linéaire de coordonnées, on peut supposer que les générateurs $ F_i (1 \leq i \leq r) $ de l’idéal sont des polynômes où le terme de plus haut degré en $ X_1 $ est de la forme $ c_i X_1^{m_i} $, où $ c_i $ est une constante $ \neq 0 $. On peut aussi supposer que les $ F_i $ n’ont aucun facteur commun. On considère alors pour $ 2r $ indéterminées $ u_i, v_i (1 \leq i \leq r) $ les polynômes $ \sum_{i=1}^r u_i F_i $ et $ \sum_{i=1}^r v_i F_i $, en tant que polynômes en $ X_1 $; on forme leur résultant de Sylvester, qui est un polynôme en les $ u_i $ et $ v_i $, à coefficients dans $ \mathbf{C}[X_2, \ldots, X_n] $ (resp. $ \mathbf{Z}[X_2, \ldots, X_n] $); en annulant ces coefficients, on obtient un système d’équations dont les solutions $ (x_2, \ldots, x_n) $ sont exactement les projections des solutions $ (x_1, \ldots, x_n) $ du système d’équations $ F_i(x_1, x_2, \ldots, x_n) = 0 (1 \leq i \leq r) $. On peut alors poursuivre l’application de la méthode par récurrence sur $ n $.

(†) C’est ce nombre de coordonnées arbitraires qu’il appelle la dimension (« Stufe »).

(‡) Voir les remarques de M. Noether au début de son mémoire (XIII). Il est intéressant de noter à ce propos que, selon Lasker, Cayley, vers 1860, aurait conjecturé que pour toute courbe gauche algébrique dans $ \mathbf{C}^3 $, il y avait un nombre fini de polynômes engendrant avait montré que déjà pour $ n = 2 $ et pour deux polynômes $ f_1, f_2 $, cela est généralement inexact, et il avait donné des conditions suffisantes pour que $ a $ soit engendré par $ f_1 $ et $ f_2 $. Dix ans plus tard, Netto prouve que, sans hypothèse sur $ f_1 $ et $ f_2 $, une puissance de $ a $ est en tout cas contenue dans l’idéal engendré par $ f_1 $ et $ f_2 $ (XV), théorème que généralise Hilbert en 1893 dans son célèbre « théorème des zéros » (XVI b)). C’est sans doute inspiré par ce résultat que Lasker, dans son mémoire, introduit la notion générale d’idéal primaire(*) dans les anneaux $ \mathbf{C}[X_1, \ldots, X_n] $ et $ \mathbf{Z}[X_1, \ldots, X_n] $ (après avoir donné dans ces anneaux la définition des idéaux premiers, en transcrivant la définition de Dedekind), et démontre(†) l’existence d’une décomposition primaire pour tout idéal dans ces anneaux(‡). Il ne semble pas s’être soucié des questions d’unicité dans cette décomposition ; c’est Macaulay qui, un peu plus tard (XXI) introduit la distinction entre idéaux primaires « immergés » et « non immergés » et montre que les seconds sont déterminés de façon unique, mais non les premiers. Il est enfin à noter que Lasker étend aussi ses résultats à l’anneau des séries entières convergentes au voisinage d’un point, en s’appuyant sur le « théorème de préparation » de Weierstrass. Cette partie de son mémoire est sans doute le premier endroit où cet anneau ait été considéré d’un point de vue purement algébrique, et les méthodes que développe à cette occasion Lasker devaient fortement influencer Krull lorsqu’en 1938 il créera la théorie générale des anneaux locaux (cf. (XXIX d)), p. 204 et passim).

l’idéal des polynômes de $ \mathbf{C}[X, Y, Z] $ qui s’annulent sur la courbe (autrement dit, un cas particulier du th. de finitude de Hilbert (XVI a))).

(*) Des exemples d’idéaux primaires non puissances d’idéaux premiers avaient été rencontrés par Dedekind dans les « ordres », i.e. les anneaux de nombres algébriques ayant un corps de nombres donné comme corps des fractions ((X), t. III, p. 306). Kronecker donne aussi comme exemple d’idéal « indécomposable » en produit de deux autres non triviaux, l’idéal de $ \mathbf{Z}[X] $ engendré par $ p^2 $ et $ X^2 + p $, où $ p $ est un nombre premier (idéal qui est primaire pour l’idéal premier engendré par $ X $ et $ p $ ((IX f)), p. 341)).

(†) Lasker procède par récurrence sur la dimension maxima $ h $ des composantes irréductibles de la variété $ V $ des zéros de l’idéal considéré $ a $. En termes modernes, il considère d’abord les idéaux premiers $ p_i $ ($ 1 \leq i \leq r $) contenant $ a $, qui correspondent aux composantes irréductibles de dimension maxima $ h $ de $ V $. A chaque $ p_i $, il associe le saturé $ q_i $ de $ a $ relativement à $ p_i $ (cf. chap. IV, § 2, n° 3, prop. 5); il considère ensuite le transporteur $ b_i = a : q_i $ de $ q_i $ dans $ a $, prend dans $ \sum b_i $ un élément $ c $ n’appartenant à aucun des $ p_i $ et montre d’une part que $ a $ est intersection des $ q_i $ et de $ a + (c) = a' $, et d’autre part que la variété $ V' $ des zéros de $ a' $ n’a que des composantes irréductibles de dimension $ \leq h - 1 $, ce qui lui permet de conclure par récurrence.

‡) Il est intéressant de remarquer que la seconde démonstration de Dedekind pour le théorème d’unique décomposition procède en établissant d’abord l’existence d’une décomposition primaire réduite unique ; et dans un passage non publié dans le XIe supplément, Dedekind observe explicitement que cette partie de la démonstration vaut non seulement pour l’anneau $ A $ de tous les entiers d’un corps de nombres $ K $, mais aussi pour tous les « ordres » de $ K $ ((X), t. III, p. 303). C’est seulement ensuite, après avoir prouvé explicitement que $ A $ est « complètement intégralement clos » (à la terminologie près) qu’il démontre, en utilisant ce fait, que les idéaux primaires de la décomposition précédente sont en fait des puissances d’idéaux premiers ((X), t. III, p. 307).

Le mouvement d’idées qui aboutira à l’Algèbre commutative moderne commence à prendre forme aux environs de 1910. Si la notion générale de corps est acquise dès le début du XXe siècle, par contre le premier travail où soit définie la notion générale d’anneau est sans doute celui de Fraenkel en 1914 (XXIII). À cette époque, on avait déjà comme exemples d’anneaux, non seulement les anneaux intègres de la Théorie des nombres et de la Géométrie algébrique, mais aussi les anneaux de séries (formelles ou convergentes), et enfin les algèbres (commutatives ou non) sur un corps de base. Toutefois, tant pour la théorie des anneaux que pour celle des corps, le rôle catalyseur semble avoir été joué par la théorie des nombres $ p $-adiques de Hensel, que Fraenkel aussi bien que Steinitz (XX a)) mentionnent tout spécialement comme point de départ de leurs recherches.

La première publication de Hensel sur ce sujet remonte à 1897; il y part de l’analogie mise en lumière par Dedekind et Weber entre les points d’une surface de Riemann d’un corps de fonctions algébriques K et les idéaux premiers d’un corps de nombres $ k $; il se propose de transporter en Théorie des nombres les « développements de Puiseux » (classiques depuis le milieu du XIXe siècle) qui, au voisinage d’un point quelconque de la surface de Riemann de K, permettent d’exprimer tout élément $ x \in K $ sous forme d’une série convergente de puissances de l’« uniformisante » au point considéré (séries n’ayant qu’un nombre fini de termes à exposants négatifs). Hensel montre de même que si $ p $ est un idéal premier de $ k $ au-dessus d’un nombre premier $ p $, on peut associer à tout $ x \in k $ une « série $ p $-adique » de la forme $ \sum_i \alpha_i p^i $ (ou $ \sum_i \alpha_i p^{i/e} $ lorsque $ p $ est ramifié au-dessus de $ p $) les $ \alpha_i $ étant pris dans un système de représentants donné du corps de restes de l’idéal $ p $; mais sa grande originalité est d’avoir eu l’idée de considérer de tels « développements » même lorsqu’ils ne correspondent à aucun élément de $ k $, par analogie avec les développements en série entière des fonctions transcendantes sur une surface de Riemann (XVIII a)).

Pendant toute la suite de sa carrière, Hensel va s’attacher à polir et perfectionner peu à peu son nouveau calcul; et si sa démarche peut nous paraître hésitante ou pesante, il ne faut pas oublier qu’au début tout au moins il ne dispose encore d’aucun des outils topologiques ou algébriques de la mathématique actuelle qui lui auraient facilité sa tâche. Dans ses premières publications il ne parle guère d’ailleurs de notions topologiques, et en somme pour lui l’anneau des entiers $ p $-adiques ($ p $ idéal premier de l’anneau des entiers A d’un corps de nombres $ k $), c’est, en termes modernes, la limite projective des anneaux $ A/p^n $ pour $ n $ croissant indéfiniment, au sens purement algébrique; et pour établir les propriétés de cet anneau et de son corps des fractions, il doit à chaque pas utiliser plus ou moins péniblement des raisonnements $ ad hoc $ (par exemple pour prouver que les nombres $ p $-adiques forment un anneau intègre). L’idée d’introduire dans un corps $ p $-adique des notions topologiques n’apparaît guère chez Hensel avant 1905 (XVIII d)); et c’est seulement en 1907, après avoir entièrement écrit le livre où il réexpose suivant ses idées la théorie des nombres algébriques (XVIII f)), qu’il arrive à la définition et aux propriétés essentielles des valeurs absolues p-adiques (XVIII e)), à partir desquelles il pourra développer, en la calquant sur la théorie de Cauchy, toute une « analyse p-adique » qu’il saura appliquer avec fruit en Théorie des nombres (notamment avec l’utilisation de l’exponentielle et du logarithme p-adiques), et dont l’importance n’a cessé de croître depuis.

Hensel avait fort bien vu, dès le début, les simplifications qu’apportait sa théorie aux exposés classiques, en permettant de « localiser » les problèmes et de se placer dans un corps où non seulement les propriétés de divisibilité sont triviales, mais encore où, grâce au lemme fondamental qu’il dégagea dès 1902 (XVIII c)), l’étude des polynômes dont le polynôme « réduit » mod. $ p $ est sans racine multiple se ramène à l’étude des polynômes sur un corps fini. Il avait donné dès 1897 (XVIII b)) des exemples frappants de ces simplifications, notamment dans les questions relatives au discriminant (en particulier, une courte démonstration du critère donné par lui quelques années auparavant pour l’existence des « diviseurs extraordinaires »). Mais pendant longtemps il semble que les nombres $ p $-adiques aient inspiré aux mathématiciens contemporains une grande méfiance; attitude courante sans doute vis-à-vis d’idées trop « abstraites », mais que l’enthousiasme un peu excessif de leur auteur (si fréquent en mathématiques parmi les zélateurs de théories nouvelles) n’était pas sans justifier en partie. Non content en effet d’appliquer sa théorie avec fruit aux nombres algébriques, Hensel, impressionné comme tous ses contemporains par les démonstrations de transcendance de $ e $ et $ \pi $, et peut-être abusé par le qualificatif « transcendant » appliqué à la fois aux nombres et aux fonctions, en était arrivé à penser qu’il existait un lien entre ses nombres $ p $-adiques et les nombres réels transcendants, et il avait cru un moment obtenir ainsi une démonstration simple de la transcendance de $ e $ et même de $ e^e $ ((XVIII d)), p. 556)(*).

Peu après 1910, la situation change, avec la montée de la génération suivante, influencée par les idées de Fréchet et de F. Riesz sur la topologie, par celles de Steinitz sur l’algèbre, et dès l’abord conquise à l’« abstraction »; elle va savoir rendre assimilables et mettre à leur vraie place les travaux de Hensel. Dès 1913, Kürschak (XXII) définit de façon générale la notion de valeur absolue, reconnaît l’importance des valeurs absolues ultramétriques (dont la valeur absolue $ p $-adique donnait l’exemple), prouve (en calquant la démonstration sur le cas des nombres réels) l’existence du complété d’un corps par rapport à une valeur absolue, et surtout démontre de façon générale la possibilité du prolongement d’une valeur absolue à une extension algébrique quelconque du corps donné. Mais il n’avait pas vu que le caractère ultramétrique d’une

(*) Cette recherche à tout prix d’un étroit parallélisme entre séries $ p $-adiques et séries de Taylor pousse aussi Hensel à se poser d’étranges problèmes: il prouve par exemple que tout entier $ p $-adique peut s’écrire sous forme d’une série $ \sum_{k=0}^{\infty} a_k p^k $ où les $ a_k $ sont des nombres rationnels choisis de sorte que la série converge non seulement dans $ \mathbf{Q}_p $, mais aussi dans $ \mathbf{R} $ (sans doute par souvenir des séries de Taylor qui convergent en plusieurs places à la fois?) (XVIII e) et f)).

valeur absolue se décelait déjà dans le corps premier; ce point fut établi par Ostrowski, à qui l’on doit aussi la détermination de toutes les valeurs absolues sur le corps $ \mathbf{Q} $, et le théorème fondamental caractérisant les corps munis d’une valeur absolue non ultramétrique comme sous-corps de $ \mathbf{C} $ (XXIV). Dans les années qui vont de 1920 à 1935, la théorie s’achèvera par une étude plus détaillée des valeurs absolues non nécessairement discrètes, comprenant entre autres l’examen des diverses circonstances qui se produisent quand on passe à une extension algébrique ou transcendante (Ostrowski, Deuring, F.K.Schmidt); d’autre part, en 1931, Krull introduit et étudie la notion générale de valuation (XXIX b)) qui sera fort utilisée dans les années qui suivent par Zariski et son école de Géométrie algébrique(*). Il nous faut aussi mentionner ici, bien que cela sorte de notre cadre, les études plus profondes sur la structure des corps valués complets et anneaux locaux complets, qui datent de la même époque (Hasse-Schmidt, Witt, Teichmüller, I. Cohen).

\* \* \*

Le travail de Fraenkel mentionné plus haut (p. 128) ne traitait qu’un type d’anneau très particulier (les anneaux artiniens n’ayant qu’un seul idéal premier, qui est en outre supposé principal). Si l’on excepte l’ouvrage de Steinitz sur les corps (XX a)), les premiers travaux importants dans l’étude des anneaux commutatifs généraux sont les deux grands mémoires de E. Noether sur la théorie des idéaux : celui de 1921 (XXV a)), consacré à la décomposition primaire, qui reprend sur le plan le plus général et complète sur bien des points les résultats de Lasker et Macaulay ; et celui de 1927 caractérisant axiomatiquement les anneaux de Dedekind (XXV b)). De même que Steinitz l’avait montré pour les corps, on voit dans ces mémoires comment un petit nombre d’idées abstraites, comme la notion d’idéal irréductible, les conditions de chaînes et l’idée d’anneau intégralement clos (les deux dernières, comme nous l’avons vu, déjà mises en évidence par Dedekind) peuvent à elles seules conduire à des résultats généraux qui semblaient inextricablement liés à des résultats de pur calcul dans les cas où on les connaissait auparavant.

Avec ces mémoires de E. Noether, joints aux travaux légèrement postérieurs d’Artin–van der Waerden sur les idéaux divisoriels (XXXI) et de Krull reliant ces idéaux aux valuations essentielles (XXIX b)) s’achève ainsi la longue étude de la décomposition des idéaux commencée un siècle auparavant(†), en même temps que s’inaugure l’Algèbre commutative moderne.

(*) Un exemple de valuation de hauteur 2 avait déjà été incidemment introduit par H. Jung en 1925 (XXVIII).

(†) A la suite de la définition des idéaux divisoriels, d’assez nombreuses recherches (Prüfer, Krull, Lorenzen, etc.) ont été entreprises sur les idéaux qui sont stables par d’autres opérations $ a \to a' $ vérifiant des conditions axiomatiques analogues aux propriétés de l’opération $ a \to A : (A : a) $ qui donne naissance aux idéaux divisoriels ; les résultats obtenus dans cette voie n’ont pas trouvé d’application jusqu’ici en Géométrie algébrique ou en Théorie des nombres.

Les innombrables recherches ultérieures d’Algèbre commutative se groupent le plus aisément suivant quelques grandes tendances directrices :

A) Anneaux locaux et topologies. Bien que contenue en germe dans tous les travaux antérieurs de Théorie des nombres et de Géométrie algébrique, l’idée générale de localisation se dégage fort lentement. La notion générale d’anneau de fractions n’est définie qu’en 1926 par H. Grell, un élève de E. Noether, et seulement pour les anneaux intègres (XXVIII); son extension aux anneaux plus généraux ne sera donnée qu’en 1944 par C. Chevalley pour les anneaux noethériens et en 1948 par Uzkov dans le cas général. Jusqu’en 1940 environ, Krull et son école sont pratiquement seuls à utiliser dans des raisonnements généraux la considération des anneaux locaux $ A_p $ d’un anneau intègre $ A $; ces anneaux ne commenceront à apparaître explicitement en Géométrie algébrique qu’avec les travaux de Chevalley et Zariski à partir de 1940(*).

L’étude générale des anneaux locaux eux-mêmes ne commence qu’en 1938 avec le grand mémoire de Krull (XXIX d)). Les résultats les plus importants de ce travail concernent la théorie de la dimension et les anneaux réguliers, dont nous n’avons pas à parler ici; mais c’est là aussi qu’apparaît pour la première fois le complété d’un anneau local noethérien quelconque, ainsi qu’une forme encore imparfaite de l’anneau gradué associé à un anneau local(†); ce dernier ne sera défini que vers 1948 par P. Samuel (XXXVI) et indépendamment dans les recherches de Topologie algébrique de Leray et H. Cartan. Krull, dans le travail précité, n’utilise guère le langage topologique; mais dès 1928 (XXIX a)), il avait prouvé que, dans un anneau noethérien $ A $, l’intersection des puissances d’un même idéal $ a $ est l’ensemble des $ x \in A $ tels que $ x(1-a)=0 $ pour un $ a \in a $; on déduit aisément de là que pour tout idéal $ m $ de $ A $, la topologie $ m $-adique sur $ A $ induit sur un idéal $ a $ la topologie $ m $-adique de $ a $; dans son mémoire de 1938, Krull complète ce résultat en prouvant que dans un anneau local noethérien, tout idéal est fermé. Ces théorèmes furent peu après étendus par Chevalley aux anneaux semi-locaux noethériens, puis par Zariski aux anneaux qui portent son nom (XXXIII b)); c’est aussi à Chevalley que remonte l’introduction de la « compacité linéaire » dans les anneaux topologiques, ainsi que la détermination de la structure des anneaux semi-locaux complets (XXXII b)).

B) Passage du local au global. Depuis Weierstrass, on a pris l’habitude d’associer une fonction analytique d’une variable (et en

(*) Dans les travaux de Hensel et de ses élèves sur la Théorie des nombres, les anneaux locaux $ A_p $ sont systématiquement négligés au profit de leurs complétés, sans doute en raison de la possibilité d’appliquer le lemme de Hensel à ces derniers.

(†) Si $ m $ est l’idéal maximal de l’anneau local noethérien $ A $ considéré, $ (\alpha_i)_{1 \leq i \leq r} $ un système minimal de générateurs de $ m $, Krull définit pour tout $ x \neq 0 $ dans $ A $ les « formes initiales » de $ x $ de la façon suivante: si $ j $ est le plus grand entier tel que $ x \in m^j $, les formes initiales de $ x $ sont tous les polynômes homogènes de degré $ j $, $ P(X_1, \ldots, X_r) $, à coefficients dans le corps résiduel $ k = A/m $, tels que $ x \equiv P(\alpha_1, \ldots, \alpha_r) $ (mod. $ m^{j+1} $). À tout idéal $ a $ de $ A $ il fait correspondre l’idéal gradué de $ k[X_1, \ldots, X_r] $ engendré par les formes initiales de tous les éléments de $ a $ (« Leitideal »); ces deux notions lui tiennent lieu de l’anneau gradué associé.

particulier une fonction algébrique) à l’ensemble de ses «développements» en tous les points de la surface de Riemann où elle est définie. Dans l’introduction de son livre sur la Théorie des nombres ((XVIII f), p. V), Hensel associe de même à tout élément d’un corps $ k $ de nombres algébriques l’ensemble des éléments qui lui correspondent dans les complétés de $ k $ pour toutes les valeurs absolues sur $ k(*) $. On peut dire que c’est ce point de vue qui, en Algèbre commutative moderne, a remplacé la formule de décomposition d’un idéal en produit d’idéaux premiers (prolongeant en un certain sens le point de vue initial de Kummer). La remarque de Hensel revient implicitement à plonger $ k $ dans le produit de tous ses complétés; c’est ce que fait explicitement Chevalley en 1936 avec sa théorie des « idèles » (XXXII a)), qui perfectionne des idées antérieures analogues de Prüfer et von Neumann (ces derniers se bornaient à plonger $ k $ dans le produit de ses complétés $ p $-adiques)(†). Bien que cela sorte quelque peu de notre cadre, il importe de mentionner ici que, grâce à une topologie appropriée sur le groupe des idèles, on peut ainsi appliquer à la Théorie des nombres toute la technique des groupes localement compacts (y compris la mesure de Haar) de façon très efficace.

Dans un ordre d’idées plus général, le théorème de Krull (XXIX b)) caractérisant un anneau intégralement clos comme intersection d’anneaux de valuation (ce qui revient encore à plonger l’anneau considéré dans un produit d’anneaux de valuation) facilite souvent l’étude de ces anneaux, bien que la méthode ne soit vraiment maniable que pour les valuations essentielles des anneaux de Krull. On trouve d’ailleurs fréquemment chez Krull (XXIX e)) des exemples (assez élémentaires) de la méthode du «passage du local au global» consistant à démontrer une propriété d’un anneau intègre $ A $ en se ramenant à la vérifier pour les «localisés» $ A_p $ de $ A $ en tous ses idéaux premiers(‡); plus récemment, Serre s’est aperçu que cette méthode est valable pour les anneaux commutatifs quelconques $ A $, qu’elle s’applique aussi aux $ A $-modules et à leurs homomorphismes et qu’il suffit même souvent de «localiser» en

(*) Hensel prend, comme valeurs absolues non ultramétriques sur un corps $ K $ de degré $ n $ sur $ \mathbf{Q} $, les fonctions $ x \to |x^{(i)}| $ (où les $ x^{(i)} $ pour $ 1 \leq i \leq n $ sont les conjugués de $ x $) couramment utilisées depuis Dirichlet; Ostrowski montra un peu plus tard que ces fonctions sont essentiellement les seules valeurs absolues non ultramétriques sur $ K $.

(†) En raison de cette remarque de Hensel, on a pris l’habitude d’appeler (par abus de langage) « places à l’infini » d’un corps de nombres $ K $ les valeurs absolues non ultramétriques de $ K $, par analogie avec le processus par lequel Dedekind et Weber définissent les « points à l’infini » de la surface de Riemann d’une courbe affine (cf. p. 125).

(‡) Quand on parle du « passage du local au global », on fait souvent allusion à des questions beaucoup plus difficiles, liées à la théorie du corps de classes, et dont les exemples les plus connus sont ceux traités dans les mémoires de Hasse (XXVI a) et b)) sur les formes quadratiques sur un corps de nombres algébriques $ k $; il y montre entre autres que pour qu’une équation $ f(x_1, \ldots, x_n) = a $ ait une solution dans $ k^n $ ($ f $ forme quadratique, $ a \in k $), il faut et il suffit qu’elle ait une solution dans chacun des complétés de $ k $. Au témoignage de Hasse, l’idée de ce type de théorèmes lui aurait été suggérée par son maître Hensel (XXVI c)). L’extension de ce « principe de Hasse » à d’autres groupes que le groupé orthogonal est l’un des objectifs de la théorie moderne des « adélisés » des groupes algébriques.

les idéaux maximaux de A (chap. II, § 3, th. 1): point de vue qui se rattache étroitement aux idées sur les «spectres» et sur les faisceaux définis sur ces spectres (voir plus bas, p. 135).

C) Entiers et clôture intégrale. Nous avons vu que la notion d’entier algébrique, d’abord introduite pour les corps de nombres, avait déjà été étendue par Kronecker et Dedekind aux corps de fonctions algébriques, bien que dans ce cas elle pût paraître assez artificielle (ne correspondant pas à une notion projective). Le mémoire de E. Noether de 1927, suivi par les travaux de Krull à partir de 1931, devaient montrer l’intérêt que présentent ces notions pour les anneaux les plus généraux(*). C’est à Krull en particulier que l’on doit les théorèmes de relèvement des idéaux premiers dans les algèbres entières (XXIX c)), ainsi que l’extension de la théorie des groupes de décomposition et d’inertie de Dedekind-Hilbert (XXIX b)). Quant à E. Noether, on lui doit la formulation générale du lemme de normalisation(†) (d’où découle entre autres le théorème des zéros de Hilbert) ainsi que le premier critère général (transcription des raisonnements classiques de Kronecker et Dedekind) permettant d’affirmer que la clôture intégrale d’un anneau intègre est finie sur cet anneau.

Enfin, il faut signaler ici qu’une des raisons de l’importance moderne de la notion d’anneau intégralement clos est due aux études de Zariski sur les variétés algébriques; il a découvert en effet que les variétés «normales» (c’est-à-dire celles dont les anneaux locaux sont intégralement clos) se distinguent par des propriétés particulièrement agréables, notamment le fait qu’elles n’ont pas de « singularité de codimension 1 »; et l’on s’est aperçu ensuite que des phénomènes analogues ont lieu pour les « espaces analytiques ». Aussi la « normalisation » (c’est-à-dire l’opération qui, pour les anneaux locaux d’une variété, consiste à prendre leurs clôtures intégrales) est-elle devenue un outil puissant dans l’arsenal de la Géométrie algébrique moderne.

D) L’étude des modules et l’influence de l’Algèbre homologique. Une des caractéristiques marquantes de l’oeuvre de E. Noether et W. Krull en Algèbre est la tendance à la «linéarisation», prolongeant la direction analogue imprimée à la théorie des corps par Dedekind et Steinitz; en d’autres termes, c’est comme modules que sont avant tout considérés les idéaux, et on est donc amené à leur appliquer toutes les constructions de l’Algèbre linéaire (quotient, produit, et plus récemment produit tensoriel et formation de modules d’homomorphismes) donnant en général des modules qui ne sont plus des idéaux. On s’aperçoit ainsi rapidement que dans beaucoup de questions (qu’il s’agisse d’ailleurs

(*) Krull et E. Noether se limitent aux anneaux intègres, mais l’extension de leurs méthodes au cas général n’est pas difficile; le mémoire le plus intéressant à cet égard est celui où I. Cohen et Seidenberg étendent les théorèmes de relèvement de Krull, en indiquant exactement leurs limites de validité (XXXV). Il convient de noter que E. Noether avait explicitement mentionné la possibilité de telles généralisations dans son mémoire de 1927 ((XXV b)), p. 30).

(†) Un cas particulier avait déjà été énoncé par Hilbert en 1893 ((XVI b)), p. 316).

d’anneaux commutatifs ou non commutatifs), on n’a pas intérêt à se borner à l’étude des idéaux d’un anneau A, mais qu’il faut au contraire énoncer plus généralement les théorèmes pour des A-modules (éventuellement soumis à certaines conditions de finitude).

L’intervention de l’Algèbre homologique n’a fait que renforcer la tendance précédente, puisque cette branche de l’Algèbre s’occupe essentiellement de questions de nature linéaire. Nous n’avons pas ici à en retracer l’histoire ; mais il est intéressant de signaler que plusieurs des notions fondamentales de l’Algèbre homologique (telles que celle de module projectif et celle du foncteur Tor) ont pris naissance à l’occasion d’une étude serrée du comportement des modules sur un anneau de Dedekind relativement au produit tensoriel, étude entreprise par H. Cartan en 1948.

Inversement, on pouvait prévoir que les nouvelles classes de modules introduites de façon naturelle par l’Algèbre homologique comme «annulateurs universels» des foncteurs Ext (modules projectifs et modules injectifs) et des foncteurs Tor (modules plats) jettéraient une lumière nouvelle sur l’Algèbre commutative. Il se trouve que ce sont surtout les modules projectifs et plus encore les modules plats qui se sont révélés utiles : l’importance de ces derniers tient avant tout à la remarque, faite d’abord par Serre (XXXVIII b)), que localisation et complétion introduisent naturellement des modules plats, «expliquant» ainsi de façon beaucoup plus satisfaisante les propriétés déjà connues de ces deux opérations et rendant beaucoup plus aisée leur utilisation. Il convient de mentionner d’ailleurs (ainsi que nous le verrons dans des chapitres ultérieurs) que les applications de l’Algèbre homologique sont loin de se limiter là, et qu’elle joue un rôle de plus en plus profond dans la Géométrie algébrique.

E) La notion de spectre. La dernière en date des notions nouvelles de l’Algèbre commutative a une histoire complexe. Le théorème spectral de Hilbert introduisait des ensembles ordonnés de projecteurs orthogonaux d’un espace hilbertien, formant une «algèbre booléenne» (ou mieux un réseau booléien)(*), en correspondance biunivoque avec un réseau booléien de classes de parties mesurables (pour une mesure convenable) de $ \mathbf{R} $. Ce sont sans doute ses travaux antérieurs sur les opérateurs dans les espaces hilbertiens qui, vers 1935, amènent M. H. Stone à étudier de façon générale les réseaux booléiens, et notamment à en chercher des «représentations» par des parties d’un ensemble (ou des classes de parties pour une certaine relation d’équivalence). Il observe qu’un réseau booléien devient un anneau commutatif (d’un type très spécial d’ailleurs), lorsqu’on y définit la multiplication par $ xy = \inf(x, y) $ et l’addition par $ x + y = \sup(\inf(x, y'), \inf(x', y)) $. Dans le cas particulier où l’on part du réseau booléien $ \mathfrak{B}(X) $ de toutes les parties d’un ensemble fini $ X $, on voit aussitôt que les éléments de $ X $ sont en correspondance

(*) Un réseau booléien est un ensemble ordonné réticulé E, ayant un plus petit élément $ \alpha $ et un plus grand élément $ \omega $, où chacune des lois sup et inf est distributive par rapport à l’autre et où, pour tout $ a \in E $, il existe un $ a' \in E $ et un seul tel que $ \inf(a, a') = \alpha $ et $ \sup(a, a') = \omega $ (cf. Ens., chap. III, 2e éd., § 1, exerc. 17).

biunivoque naturelle avec les idéaux maximaux de l’anneau «booléien» correspondant; et Stone obtient précisément son théorème général de représentation d’un réseau booléien en considérant de même l’ensemble des idéaux maximaux de l’anneau correspondant, et en associant à tout élément du réseau booléien l’ensemble des idéaux maximaux qui le contiennent (XXX a)).

D’autre part, on connaissait, comme exemple classique de réseau booléien, l’ensemble des parties à la fois ouvertes et fermées d’un espace topologique. Dans un second travail (XXX b)), Stone montra qu’en fait tout réseau booléien est aussi isomorphe à un réseau booléien de cette nature. Il fallait naturellement pour cela définir une topologie sur l’ensemble des idéaux maximaux d’un anneau «booléien»; ce qui se fait très simplement en prenant pour ensembles fermés, pour chaque idéal a, l’ensemble des idéaux maximaux contenant a.

Nous n’avons pas à parler ici de l’influence de ces idées en Analyse fonctionnelle, où elles jouèrent un rôle important dans la naissance de la théorie des algèbres normées développée par I. Gelfand et son école. Mais en 1945, Jacobson observe (XXXIV) que le procédé de définition d’une topologie, imaginé par Stone, peut en fait s’appliquer à tout anneau A (commutatif ou non) pourvu que l’on prenne comme ensemble d’idéaux non pas l’ensemble des idéaux maximaux, mais l’ensemble des idéaux «primitifs» bilatères (i.e. les idéaux bilatères b tels que A/b soit un anneau primitif); pour un anneau commutatif, on retrouve bien entendu les idéaux maximaux. De son côté, Zariski, en 1944 (XXXIII a)), utilise une méthode analogue pour définir une topologie sur l’ensemble des places d’un corps de fonctions algébriques. Toutefois, ces topologies restaient pour la plupart des algébristes de simples curiosités, en raison du fait qu’elles sont d’ordinaire non séparées, et qu’on éprouvait une répugnance assez compréhensible à travailler sur des objets aussi insolites. Cette méfiance ne fut dissipée que lorsque A. Weil montra, en 1952, que toute variété algébrique peut être munie de façon naturelle d’une topologie du type précédent et que cette topologie permet de définir, en parfaite analogie avec le cas des variétés différentiables ou analytiques, la notion d’espace fibré (XXXVII); peu après, Serre eut l’idée d’étendre à ces variétés ainsi topologisées la théorie des faisceaux cohérents, grâce à laquelle la topologie rend dans le cas des variétés «abstraites» les mêmes services que la topologie usuelle lorsque le corps de base est C, notamment en ce qui concerne l’application des méthodes de la Topologie algébrique (XXXVIII a) et b)).

Dès lors il était naturel d’utiliser ce langage géométrique dans toute l’Algèbre commutative. On s’est rapidement aperçu que la considération des idéaux maximaux est d’ordinaire insuffisante pour obtenir des énoncés commodes(*), et que la notion adéquate est celle de l’ensemble

(*) L’inconvénient de se borner au «spectre maximal» provient de ce que, si $ \varphi : A \to B $ est un homomorphisme d’anneaux et n un idéal maximal de B, $ \bar{\varphi}^1(n) $ n’est pas nécessairement un idéal maximal de A, alors que pour tout idéal premier p de B, $ \bar{\varphi}^1(p) $ est un idéal premier de A. On ne peut donc en général associer à $ \varphi $ de façon naturelle une application de l’ensemble des idéaux maximaux de B dans l’ensemble des idéaux maximaux de A.

des idéaux premiers de l’anneau, topologisé de la même manière. Avec l’introduction de la notion de spectre, on dispose maintenant d’un dictionnaire permettant d’exprimer tout théorème d’Algèbre commutative dans un langage géométrique très proche de celui de la Géométrie algébrique de l’époque Weil-Zariski ; ce qui d’ailleurs a amené aussitôt à élargir considérablement le cadre de cette dernière, de sorte que l’Algèbre commutative n’en est plus guère, de ce point de vue, que la partie la plus élémentaire (XXXIX).

(I) L. Euler, Vollständige Anleitung zur Algebra (= Opera Omnia (1), t. I, Leipzig–Berlin (Teubner), 1911).

(II) J. L. Lagrange, Oeuvres, 14 vol., Paris (Gauthier–Villars), 1867–1892.

(III) C. F. Gauss, Werke, 12 vol., Göttingen, 1870–1927.

(IV) P. G. Lejeune-Dirichlet, Werke, 2 vol., Berlin (Reimer), 1889–1897.

(IV bis) P. G. Lejeune-Dirichlet, Vorlesungen über Zahlentheorie, 2te Aufl., Braunschweig (Vieweg), 1871.

(V) C. G. J. Jacobi, Gesammelte Werke, 7 vol., Berlin (Reimer), 1881–1891.

(VI) G. Eisenstein: a) Beweis der Reciprocitätsgesetze für die cubischen Reste in der Theorie der aus dritten Wurzeln der Einheit zusammengesetzten Zahlen, J. de Crelle, t. XXVII (1844), p. 289–310; b) Zur Theorie der quadratischen Zerfällung der Primzahlen $8n + 3$, $7n + 2$ und $7n + 4$, J. de Crelle, t. XXXVII (1848), p. 97–126; c) Über einige allgemeine Eigenschaften der Gleichung von welcher die Teilung der ganzen Lemniscate abhängt, nebst Anwendungen derselben auf die Zahlentheorie, J. de Crelle, t. XXXIX (1850), p. 160–179 et 224–287.

(VII) E. Kummer: a) Sur les nombres complexes qui sont formés avec les nombres entiers réels et les racines de l’unité, J. de Math., (1), t. XII (1847), p. 185–212; b) Zur Theorie der complexen Zahlen, J. de Crelle, t. XXXV (1847), p. 319–326; c) Ueber die Zerlegung der aus Wurzeln der Einheit gebildeten complexen Zahlen in Primfactoren, J. de Crelle, t. XXXV (1847), p. 327–367; d) Mémoire sur les nombres complexes composés de racines de l’unité et des nombres entiers, J. de Math., (1), t. XVI (1851), p. 377–498; e) Über die allgemeinen Reciprocitätsgesetze unter den Resten und Nichtresten der Potenzen deren Grad eine Primzahl ist (Abh. der Kön. Akad. der Wiss. zu Berlin (1859), Math. Abhandl., p. 19–159).

(VIII) C. Hermite, Oeuvres, 4 vol., Paris (Gauthier-Villars), 1905–1917.

(IX) L. Kronecker, Werke, 5 vol., Leipzig (Teubner), 1895–1930: a) De unitatibus complexis, vol. I, p. 5–71 (= Inaug. Diss., Berolini, 1845); b) Über die algebraisch auflösbaren Gleichungen I, vol. IV, p. 1–11 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1853, p. 365–374); c) Über die elliptischen Functionen für welche complexe Multiplication stattfindet, vol. IV, p. 177–183 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1857, p. 455–460); d) Über die complexe Multiplication der elliptischen Functionen, vol. IV, p. 207–217 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1862, p. 363–372); e) Über die Discriminante algebraischer Functionen einer Variabeln, vol. II, p. 193–236 (= J. de Crelle, t. XCI (1881), p. 301–334); f) Grundzüge einer arithmetischen Theorie der algebraischen Grössen, vol. II, p. 237–387 (= J. de Crelle, t. XCII (1882), p. 1–122).

(X) R. Dedekind, Gesammelte mathematische Werke, 3 vol., Braunschweig (Vieweg), 1932: a) Abriss einer Theorie der höheren Kongruenzen in bezug auf einen reellen Primzahl-Modulus, vol. I, p. 40–66 (= J. de Crelle, t. LIV (1857), p. 1–26); b) Sur la Théorie des Nombres entiers algébriques, vol. III, p. 262–296 (= Bull. Sci. Math., (1), t. XI (1876), p. 278–288 et (2), t. I, (1877), p. 17–41, 69–92, 144–164, 207–248); c) Über die Anzahl der Ideal-Klassen in den verschiedenen Ordnungen eines endlichen Körpers, vol. I, p. 105–157 (= Festschrift der Technischen Hochschule in Braunschweig zur Säkularfeier des Geburtstages von C. F. Gauss, Braunschweig, 1877, p. 1–55); d) Über den Zusammenhang zwischen der Theorie der Ideals une der Theorie der höheren Kongruenzen, vol. I, p. 202–230 (= Abh. Kön. Ges. Wiss. zu Göttingen, t. XXIII (1878), p. 1–23); e) Über die Diskriminanten endlicher Körper, vol. I, p. 351–396 (= Abh. Kön. Ges. Wiss. zu Göttingen, t. XXIX (1882), p. 1–56); f) Über die Theorie der ganzen algebraischen Zahlen, vol. III, p. 1–222 (= Supplement XI von Dirichlets Vorlesungen über Zahlentheorie, 4. Aufl. (1894), p. 434–657): g) Zur Theorie der Ideale, vol. II, p. 43–48 (= Nachr. Göttingen, 1894, p. 272–277); h) Über eine Erweiterung des Symbols (a, b) in der Theorie der Moduln, vol. II, p. 59–85 (= Nachr. Göttingen, 1895, p. 183–208).

(X bis) R. Dedekind–H. Weber, Theorie der algebraischen Funktionen einer Veränderlichen, J. de Crelle, t. XCII (1882), p. 181–290 (= R. Dedekind, Ges. Math. Werke, t. I, p. 238–349).

(XI) E. Selling, Ueber die idealen Primfactoren der complexen Zahlen, welche aus den Wurzeln einer beliebigen irreductiblen Gleichung rational gebildet sind, Zeitschr. für Math. und Phys., t. X (1865), p. 17–47.

(XII) M. Noether, Über einen Satz aus der Theorie der algebraischen Funktionen, Math. Ann., t. VI (1873), p. 351–359.

(XIII) A. Brill–M. Noether, Ueber algebraische Funktionen, Math. Ann., t. VII (1874), p. 269–310.

(XIV) G. Zolotareff, Sur la théorie des nombres complexes, J. de Math., (3), t. VI (1880), p. 51–84 et 129–166.

(XV) E. Netto, Zur Theorie der Elimination, Acta Math., t. VII (1885), p. 101–104.

(XVI) D. Hilbert: a) Über die Theorie der algebraischen Formen, Math. Ann., t. XXXVI (1890), p. 473–534; b) Über die vollen Invariantensysteme, Math. Ann., t. XLII (1893), p. 313–373; c) Grundzüge einer Theorie des Galoischen Zahlkörpers, Gött. Nachr., (1894), p. 224–236; d) Zahlbericht, Jahresber. der D.M.V., t. IV (1897), p. 175–546 (trad. française par A. Lévy et Th. Got sous le nom « Théorie des corps de nombres algébriques », Paris (Hermann), 1913).

(XVII) K. Weierstrass, Mathematische Werke, 7 vol. Berlin (Mayer und Müller), 1894–1927.

(XVIII) K. Hensel: a) Über eine neue Begründung der Theorie der algebraischen Zahlen, Jahresber. der D.M.V., t. VI (1899), p. 83–88; b) Ueber die Fundamentalgleichung und die ausserwesentlichen Diskriminantenteiler eines algebraischen Körpers, Gött. Nachr., (1897), p. 254–260; c) Neue Grundlagen der Arithmetik, J. de Crelle, t. CXXVII (1902), p. 51–84; d) Über die arithmetische Eigenschaften der algebraischen und transzendenten Zahlen, Jahresber. der D.M.V., t. XIV (1905), p. 545–558; e) Ueber die arithmetischen Eigenschaften der Zahlen, Jahresber. der D.M.V., t. XVI (1907), p. 299–319, 388–393, 474–496; f) Theorie der algebraischen Zahlen, Leipzig (Teubner), 1908.

(XIX) E. Lasker, Zur Theorie der Moduln und Ideale, Math. Ann., t. LX (1905), p. 20–116.

(XX) E. Steinitz: a) Algebraische Theorie der Körper, J. de Crelle, t. CXXXVII (1910), p. 167–308; b) Rechteckige Systeme und Moduln in algebraischen Zahlkörpern, Math. Ann., t. LXXI (1912), p. 328–354 et t. LXXII (1912), p. 297–345.

(XXI) F. S. Macaulay, On the resolution of a given modular system into primary systems including some properties of Hilbert numbers, Math. Ann., t. LXXIV (1913), p. 66–121.

(XXII) J. KÜRSCHAK, Über Limesbildung und allgemeine Körpertheorie, J. de Crelle, t. CXLII (1913), p. 211–253.

(XXIII) A. FRAENKEL, Über die Teiler der Null und die Zerlegung von Ringen, J. de Crelle, t. CXLV (1914), p. 139–176.

(XXIV) A. OSTROWSKI, Über einige Lösungen der Funktionalgleichung $ \varphi(x)\varphi(y) = \varphi(x \cdot y) $, Acta Math., t. XLI (1917), p. 271–284.

(XXV) E. NOETHER: a) Idealtheorie in Ringbereichen, Math. Ann., t. LXXXIII (1921), p. 24–66; b) Abstrakter Aufbau der Idealtheorie in algebraischen Zahl- und Funktionenkörpern, Math. Ann., t. XCVI (1927), p. 26–61.

(XXVI) H. HASSE: a) Ueber die Darstellbarkeit von Zahlen durch quadratischen Formen im Körper der rationalen Zahlen, J. de Crelle, t. CLII (1923), p. 129–148; b) Ueber die Äquivalenz quadratischer Formen im Körper der rationalen Zahlen, J. de Crelle, t. CLII (1923), p. 205–224; c) Kurt Hensels entscheidender Anstoss zur Entdeckung des Lokal-Global-Prinzips, J. de Crelle, t. CCIX (1960), p. 3–4.

(XXVII) H. JUNG, Algebraischen Flächen, Hannover (Helwing), 1925.

(XXVIII) H. GRELL, Beziehungen zwischen den Idealen verschiedener Ringe, Math. Ann., t. XCVII (1927), p. 490–523.

(XXIX) W. KRULL: a) Primidealketten in allgemeine Ringbereichen, Sitz. Ber. Heidelberg Akad. Wiss., 1928; b) Allgemeine Bewertungstheorie, J. de Crelle, t. CLXVII (1931), p. 160–196; c) Beiträge zur Arithmetik kommutativer Integritätsbereiche, III, Math. Zeitschr., t. XLII (1937), p. 745–766; d) Dimensionstheorie in Stellenringen, J. de Crelle, t. CLXXIX (1938), p. 204–226; e) Idealtheorie, Berlin (Springer), 1935.

(XXX) M. H. STONE: a) The theory of representation for Boolean algebras, Trans. Amer. Math. Soc., t. XL (1936), p. 37–111; b) Applications of the theory of Boolean rings to general topology, Trans. Amer. Math. Soc., t. XLI (1937), p. 375–481.

(XXXI) B. L. van der WAERDEN, Moderne Algebra, t. II, Berlin (Springer), 1931.

(XXXII) C. CHEVALLEY: a) Généralisation de la théorie du corps de classes pour les extensions infinies, J. de Math., (9), t. XV (1936), p. 359–371; b) On the theory of local rings, Ann. of Math., t. XLIV (1943), p. 690–708.

(XXXIII) O. ZARISKI: a) The compactness of the Riemann manifold of an abstract field of algebraic functions, Bull. Amer. Math. Soc., t. L (1944), p. 683–691; b) Generalized semi-local rings, Summa Bras. Math., t. I (1946), p. 169–195.

(XXXIV) N. JACOBSON, A topology for the set of primitive ideals in an arbitrary ring, Proc. Nat. Acad. Sci. U.S.A., t. XXXI (1945), p. 333–338.

(XXXV) I. COHEN–A. SEIDENBERG, Prime ideals and integral dependence, Bull. Amer. Math. Soc., t. LII (1946), p. 252–261.

(XXXVI) P. SAMUEL, La notion de multiplicité en Algèbre et en Géométrie algébrique, J. de Math., (9), t. XXX (1951), p. 159–274.

(XXXVII) A. WEIL, Fibre-spaces in Algebraic Geometry (Notes by A. Wallace), Chicago Univ., 1952.

(XXXVIII) J. P. SERRE: a) Faisceaux algébriques cohérents, Ann. of Math., t. LXI (1955), p. 197–278; b) Géométrie algébrique et géométrie analytique, Ann. Inst. Fourier, t. VI (1956), p. 1–42.

(XXXIX) A. GROTHENDIECK, Eléments de géométrie algébrique, Publ. math. Inst. Htes. Et. Scient., 1960.

Index des notations

Les chiffres de référence indiquent successivement le chapitre, le paragraphe et le numéro.

Chapitre V
A $ \mathcal{G} $ (A algèbre, $ \mathcal{G} $ groupe opérant sur A) : V, 1, 9.
$ \mathcal{G}^Z(p') $, $ \mathcal{G}^Z $, $ A^Z(p') $, $ A^Z(\mathcal{G}) $ groupe opérant sur un anneau $ A' $, $ p' $ idéal premier de $ A' $ : V, 2, 2.
$ \mathcal{G}^{T}(p') $, $ \mathcal{G}^{T} $, $ A^{T}(p') $, $ A^{T}(\mathcal{G}) $ groupe opérant sur un anneau $ A' $, $ p' $ idéal premier de $ A' $ : V, 2, 2.
$ K^Z(p') $, $ K^Z $, $ K^{T}(p') $, $ K^{T} $ (K corps des fractions d’un anneau intégralement clos $ A $, $ p' $ idéal premier dans la fermeture intégrale de $ A $ dans une extension quasi-galoisienne de $ K $) : V, 2, 3.
$ Y^p $ (avec $ p = (p_1, ..., p_m) $, les $ p_i $ entiers $ \geqslant 0 $) : V, 3, 1.

Chapitre VI
$ m(A) $, $ \kappa(A) $, $ U(A) $ (A anneau local) : VI.
$ K, \infty $ : VI, 2, 1.
$ + \infty $ : VI, 3, 1.
$ \Gamma_A, \varphi_A $ : VI, 3, 2.
$ \alpha(M) $ (M ensemble majeur) : VI, 3, 5.
$ h(G) $ (G groupe totalement ordonné) : VI, 4, 4.
$ \mathcal{C}_v $ ($ v $ valuation) : VI, 5, 2.
$ e(v'/v), e(A'/A), e(L/K) $ : VI, 8, 1.
$ f(v'/v), f(A'/A), f(L/K) $ : VI, 8, 1.
$ \varepsilon(G, H) $ (G groupe totalement ordonné, H sous-groupe d’indice fini de G) : VI, 8, 4.
$ \varepsilon(v'/v) $ ($ v $ valuation, $ v' $ prolongement de $ v $) : VI, 8, 4.
$ \operatorname{mod}(x), \operatorname{mod}_K(x) $ (K corps localement compact non discret, $ x \in K $) : VI, 9, 1.
$ r(G) $ (rang rationnel d’un groupe commutatif) : VI, 10, 2.
$ d(K'/K), s(v'/v), r(v'/v) $ ($ v $ valuation sur K, $ v' $ prolongement de $ v $ à une extension transcendante $ K' $ de K) : VI, 10, 3.

Chapitre VII
I(A), D(A) (A anneau intègre) : VII, 1, 1.
$ a < b $, div(a), div(x) (a, b idéaux fractionnaires, x élément du corps des fractions) : VII, 1, 1.
$ \tilde{a} $ (a idéal fractionnaire) : VII, 1, 1.
$ d_1 \leq d_2 $ ($ d_1, d_2 $ diviseurs) : VII, 1, 1.
$ b : a $ (a, b idéaux fractionnaires) : VII, 1, 1.
J(A) (A anneau intègre) : VII, 1, 2.
P(A) (A anneau de Krull) : VII, 1, 3.
$ p^{(n)} $ (p idéal premier divisoriel) : VII, 1, 4.
$ v_p $ (p idéal premier de hauteur 1 dans un anneau de Krull) : VII, 1, 10.
F(A), C(A) (A anneau de Krull) : VII, 1, 10.
$ e(\mathfrak{B}/p) $ ($ p \in P(A), \mathfrak{B} \in P(B) $. A et B anneaux de Krull, $ A \subset B, \mathfrak{B} \cap A = p $) : VII, 1, 10.
$ i $ (homomorphisme de D(A) dans D(B), ou de C(A) dans C(B)) : VII, 1, 10.
$ \overline{i} $ (homomorphisme de C(A) dans C(B)) : VII, 1, 10.
$ A, A_0, \Delta(K) $ (anneaux d’adèles restreints) : VII, 2, 4.
$ \mathfrak{B}^*, \mathfrak{B}^*(A) $ (A anneau intègre) : VII, 3, 2.
$ M^* $ (réseau dual d’un réseau M) : VII, 4, 2.
$ l_p(T), \chi(T) $ (T A-module de torsion, p idéal premier de hauteur 1) : VII, 4, 5.
$ F(A), T(A), cl(M) $ : VII, 4, 5.
$ \chi(M, M') $ (M, $ M' $ réseaux) : VII, 4, 6.
$ c(d) $ (d diviseur) : VII, 4, 7.
$ c(M), r(M), \gamma(M) $ (M réseau) : VII, 4, 7.
$ \mathfrak{B}/p, e_{\mathfrak{B}/p}, f_{\mathfrak{B}/p}, f(\mathfrak{B}/p) $ (A $ \subset $ B anneaux de Krull tels que B soit une A-algèbre finie, $ p \in P(A), \mathfrak{B} \in P(B), \mathfrak{B} \cap A = p $) : VII, 4, 8.
$ N_{B/A}, N, i_{B/A} $ : VII, 4, 8.

Index terminologique

Les chiffres de référence indiquent successivement le paragraphe et le numéro (ou exceptionnellement, l’exercice).

Adèle restreint, adèle restreint principal : VII, 2, 4.
Algèbre entière, finie, sur un anneau : V, 1, 1.
Algébrique (fermeture) d’un corps dans une algèbre : V, 1, 2.
Algébriquement fermé (corps) dans une algèbre : V, 1, 2.
Anneau bezoutien (ou de Bezout) : VII, 1, exerc. 20.
Anneau complètement intégralement clos : V, 1, 4.
Anneau de décomposition : V, 2, 2.
Anneau de Dedekind : VII, 2, 1.
Anneau de Jacobson : V, 3, 4.
Anneau de Krull : VII, 1, 3.
Anneau de valuation, anneau de valuation pour un corps : VI, 1, 1.
Anneau d’inertie : V, 2, 2.
Anneau d’une place : VI, 2, 3.
Anneau d’une valuation : VI, 3, 2.
Anneau factoriel : VII, 3, 1.
Anneau intégralement clos : V, 1, 2.
Anneau intégralement clos de caractère fini : VII, 1, exerc. 25, 26, 28.
Anneau intégralement fermé dans une algèbre : V, 1, 2.
Anneau intégralement noethérien : V, 3, exerc. 6.
Anneau local dominant un anneau local : VI, 1, 1.
Anneau local intègre de dimension 1 : VI, 4, exerc. 7.
Anneau non ramifié : V, 2, exerc. 19.
Anneau prüférien (ou de Prüfer) : VII, 2, exerc. 12.
Anneau pseudo-bezoutien : VII, 1, exerc. 21.
Anneau pseudo-principal : VII, 1, exerc. 21.
Anneau pseudo-prüférien : VII, 2, exerc. 19.
Anneau régulièrement intégralement clos : VII, 1, exerc. 30.
Anneaux de valuation indépendants : VI, 7, 2.
Apparentés (anneaux locaux) : VI, 1, exerc. 1.
Approximation (théorème d’) pour les valuations : VI, 7, 2.
Approximation (théorème d’) pour les valeurs absolues : VI, 7, 3.
Associés (anneau, place, valuation) : VI, 3, 3.
Au-dessus (idéal) d’un idéal : V, 2, 1.

Canonique (décomposition) d’une place : VI, 2, 3.
Canonique (factorisation) d’une valuation : VI, 3, 2.
Canonique (homomorphisme) du groupe de décomposition d’un idéal premier $ p' $ de $ A' $ dans le groupe des automorphismes de $ A'/p' $ : V, 2, 2.
Classe de diviseurs attachée à un module de type fini : VII, 4, 7.

Classes de diviseurs (monoïde des) : VII, 1, 2.
Clôture intégrale d’un anneau intègre : V, 1, 2.
Complet (système) de prolongements d’une valuation : VI, 8, 2.
Complètement intégralement clos (anneau) : V, 1, 4.
Conducteur d’un sous-anneau : V, 1, 5.
Contenu d’un module de torsion : VII, 4, 5.
Contenu d’un polynôme sur un anneau pseudo-bezoutien : VII, 1, exerc. 23.
Corps algébriquement fermé dans une algèbre : V, 1, 2.
Corps de décomposition : V, 2, 3.
Corps des valeurs d’une place : VI, 2, 2.
Corps projectif : VI, 2, 1.
Corps résiduel d’une place : VI, 2, 3.
Corps résiduel d’une valuation : VI, 3, 2.
Critère d’irréductibilité d’Eisenstein : VII, 3, exerc. 20.

Décomposition canonique d’une place : VI, 2, 3.
Décomposition complète d’un idéal premier : V, 2, 2.
Décomposition en facteurs premiers d’un idéal dans un anneau de Dedekind :
VII, 2, 3.
Décomposition (groupe, anneau de) d’un idéal premier : V, 2, 2.
Décomposition (corps de) d’un idéal premier : V, 2, 3.
Dedekind (anneau de) : VII, 2, 1.
Degré résiduel d’une valuation sur une autre : VI, 8, 1.
Dépendance intégrale (équation de) : V, 1, 1.
Discrète (valuation) : VI, 3, 6.
Distingué (polynôme) : VII, 3, 8.
Diviseur, diviseur principal : VIII, 1, 1.
Diviseur déterminantiel : VII, 4, exerc. 11.
Diviseur de type fini : VII, 1, exerc. 11.
Diviseurs équivalents : VII, 1, 2.
Divisoriel (idéal fractionnaire) : VII, 1, 1.
Dominant (anneau local) un anneau local : VI, 1, 1.
Dual (réseau) : VII, 4, 2.
Dual torique algébrique d’un module : VI, 5, exerc. 9.
Dual torique topologique : VI, 5, exerc. 10.

Ensemble majeur dans un groupe totalement ordonné : VI, 3, 5.
Entier algébrique : V, 1, 1.
Entier (idéal) : VII, 1, 1.
Entier sur un anneau : V, 1, 1.
Entier de Gauss : V, 1, 1.
Entière (algèbre) sur un anneau : V, 1, 1.
Équivalents (diviseurs) : VII, 1, 2.
Équivalentes (valuations) : VI, 3, 2.
Essentielle (valuation) : VII, 1, 4.
Euclidien (corps ordonné) : VI, 2, exerc. 4.
Extension quasi galoisienne : V, 2, 2.

Facteur invariant : VII, 4, exerc. 11 et 14.
Factoriel (anneau) : VII, 3, 1.
Factorisation canonique d’une valuation : VI, 3, 2.
Fermeture algébrique d’un corps dans une algèbre : V, 1, 2.

Fermeture intégrale d’un anneau dans une algèbre : V, 1, 2.
Finie (algèbre) sur un anneau : V, 1, 1.
Finie (place) en un élément : VI, 2, 2.
Fractionnaire (idéal) : VII, 1, 1.

Gauss (entier de) : V, 1, 1.
Gauss (lemme de) : VII, 3, 5.
Gelfand-Mazur (théorème de) : VI, 6, 4.
Groupe de décomposition : V, 2, 2.
Groupe des ordres d’une valuation : VI, 3, 2.
Groupe d’inertie : V, 2, 2.
Groupe d’opérateurs localement fini : V, 1, 9.
Groupe opérant sur un anneau : V, 1, 9.
Groupe ordonné de hauteur $ n $, de hauteur $ +\infty $ : VI, 4, 4.

Hauteur d’un groupe ordonné, d’une valuation : VI, 4, 4.
Hauteur $ \leq 1 $ (idéal premier de) : VII, 1, 6.
Homomorphisme canonique du groupe de décomposition d’un idéal premier $ p' $ de $ A' $ dans le groupe des automorphismes de $ A'/p' $ : V, 2, 2.
Homomorphisme pseudo-injectif, pseudo-surjectif, pseudo-nul, pseudo-bijectif : VII, 4, 4.

Idéal au-dessus d’un idéal : V, 2, 1.
Idéal déterminantiel : VII, 4, exerc. 10 et 14.
Idéal d’une place : VI, 2, 3.
Idéal d’une valuation : VI, 3, 2.
Idéal entier, idéal fractionnaire : VII, 1, 1.
Idéal non ramifié : V, 2, exerc. 18 et 19.
Idéal premier de hauteur $ \leq 1 $ : VII, 1, 6.
Idéal premier se décomposant complètement : V, 2, 2.
Identité de Cauchy : VII, 3, exerc. 18.
Impropre (valuation) : VI, 3, 1.
Indépendants (anneaux de valuation) : VI, 7, 2.
Indépendantes (valuations) : VI, 7, 2.
Indice de ramification : VI, 8, 1.
Indice initial d’un sous-groupe d’un groupe ordonné, indice initial de ramification d’une valuation : VI, 8, 4.
Inertie (anneau, groupe d’) : V, 2, 2.
Inertie (corps d’) : V, 2, 3.
Initial (indice) de ramification : VI, 8, 4.
Intégrale (clôture) : V, 1, 2.
Intégrale (fermeture) : V, 1, 2.
Intégralement clos (anneau) : V, 1, 2.
Intégralement fermé dans une algèbre (anneau) : V, 1, 2.
Invariant relatif d’un réseau par rapport à un autre : VII, 4, 6.
Isolé (sous-groupe) : VI, 4, 2.

Jacobson (anneau de) : V, 3, 4.

Krull (anneau de) : VII, 1, 3.
Krull-Akizuki (théorème de) : VII, 2, 5.

Lemme de Gauss : VII, 3, 5.
Lemme de normalisation : V, 3, 1.
Localement fini (groupe d’opérateurs) : V, 1, 9.

Majeur (ensemble) : VI, 3, 5.
Minimal (polynôme) : V, 1, 3.
Module pseudo-nul : VII, 4, 4.
Monoïde des classes de diviseurs : VII, 1, 2.
Morphisme pour des lois de composition non partout définies : VI, 2, 1.

Non ramifiée (valuation) : VI, 8, 1.
Normalisation (lemme de) : V, 3, 1.
Normée (valuation discrète) : VI, 3, 6.

Ordre d’un élément pour une valuation : VI, 3, 2.
Ordre réduit d’une série formelle : VII, 3, 8.
Ordres (groupe des) d’une valuation : VI, 3, 2.
Ostrowski (théorème d’) : VI, 6, 4.

Place d’un corps : VI, 2, 2.
Place finie en x : VI, 2, 2.
Place triviale : VI, 2, 2.
Polygone de Newton : VI, 4, exerc. 11.
Polynôme minimal : V, 1, 3.
Polynôme distingué : VII, 3, 8.
Préparation (théorème de) : VII, 3, 8.
Presque tout p ∈ P(A) (propriété valable pour) : VII, 4, 3.
Principal (adèle restreint) : VII, 2, 4.
Principal (diviseur) : VII, 1, 1.
Projectif (corps) : VI, 2, 1.
Pseudo-injectif, pseudo-surjectif, pseudo-nul, pseudo-bijectif (homomorphisme) : VII, 4, 4.
Pseudo-isomorphisme : VII, 4, 4.
Pseudo-nul (module) : VII, 4, 4.

Quasi-galoisienne (extension) : V, 2, 2.

Rang rationnel d’un groupe commutatif : VI, 10, 2.
Rang résiduel : VI, 8, 5.
Rationnel (rang) d’un groupe commutatif : VI, 10, 2.
Réduit (ordre) : VIII, 3, 8.
Réduite (série) : VII, 3, 8.
Réflexif (réseau) : VII, 4, 2.
Représentatif (système) d’éléments extrémaux : VII, 3, 3.
Réseau : VII, 4, 1.
Réseau dual : VII, 4, 2.
Réseau réflexif : VII, 4, 2.
Résiduel (degré) d’une valuation : VI, 8, 1.
Résiduel (rang) d’une valuation : VI, 8, 5.
Résolution libre finie d’un module : VII, 4, 7.
Restreint (adèle) : VII, 2, 4.

Série réduite : VII, 3, 8.
Sous-groupe isolé d’un groupe ordonné : VI, 4, 2.
Système complet de prolongements d’une valuation : VI, 8, 2.
Système représentatif d’éléments extrémaux : VII, 3, 3.

Théorème d’approximation pour les valuations : VI, 7, 2.
Théorème d’approximation pour les valeurs absolues : VI, 7, 3.
Théorème de Gelfand-Mazur : VI, 6, 4.
Théorème de Krull-Akizuki : VII, 2, 5.
Théorème de préparation : VII, 3, 8.
Théorème de Stickelberger : VI, 8, exerc. 18.
Théorème d’Ostrowski : VI, 6, 3.
Théorème principal de Zariski : V, 3, exerc. 7.
Théorème des zéros de Hilbert : V, 3, 3.
Triviale (place) : VI, 2, 2.

Ultramétrique (valeur absolue) : VI, 6, 1.
Uniformisante pour une valuation discrète : VI, 3, 6.

Valeur absolue ultramétrique : VI, 6, 1.
Valeurs (corps des) d’une place : VI, 2, 2.
Valuation, valuation d’un élément x : VI, 3, 1 et VI, 3, 2.
Valuation (anneau de) : VI, 1, 1.
Valuation impropre : VI, 3, 1.
Valuation discrète, valuation discrète normée : VI, 3, 6.
Valuation essentielle : VII, 1, 4 et 1, exerc. 26.
Valuation non ramifiée : VI, 8, 1.
Valuations équivalentes : VI, 3, 2.
Valuations indépendantes : VI, 7, 2.

Zéros (théorème des) : V, 3, 3.

CHAPITRE V. — Entiers .................................................... 5
§ 1. Notion d’élément entier ............................................. 5
    1. Éléments entiers sur un anneau .................................... 5
    2. Fermeture intégrale d’un anneau. Anneaux intégralement
        clos ............................................................ 11
    3. Exemples d’anneaux intégralement clos ............................ 13
    4. Anneaux complètement intégralement clos .......................... 16
    5. Fermeture intégrale d’un anneau de fractions ..................... 18
    6. Normes et traces d’entiers ....................................... 20
    7. Extension des scalaires dans une algèbre intégralement close ..... 23
    8. Entiers sur un anneau gradué ..................................... 25
    9. Application : invariants d’un groupe d’automorphismes
        d’une algèbre ................................................... 28
§ 2. Relèvement des idéaux premiers ..................................... 31
    1. Le premier théorème d’existence .................................. 31
    2. Groupe de décomposition et groupe d’inertie ...................... 36
    3. Décomposition et inertie pour les anneaux intégralement
        clos ............................................................ 45
    4. Deuxième théorème d’existence .................................... 52
§ 3. Algèbres de type fini sur un corps ................................. 54
    1. Le lemme de normalisation ........................................ 54
    2. Fermeture intégrale d’une algèbre de type fini sur un corps ...... 59
    3. Le théorème des zéros ............................................ 60
    4. Anneaux de Jacobson .............................................. 62
Exercices du § 1 ........................................................ 66
Exercices du § 2 ........................................................ 73
Exercices du § 3 ........................................................ 80

CHAPITRE VI. — Valuations ............................................... 84
§ 1. Anneaux de valuation ............................................... 84
    1. Relation de domination entre anneaux locaux ...................... 84
    2. Anneaux de valuation ............................................. 85
    3. Caractérisation des éléments entiers ............................. 88
    4. Exemples d’anneaux de valuation .................................. 89
§ 2. Places ............................................................. 91
    1. Notion de morphisme pour les lois de composition non
        partout définies ................................................ 91
    2. Places ........................................................... 92
    3. Places et anneaux de valuation ................................... 93
    4. Extension des places ............................................. 95
    5. Caractérisation des éléments entiers au moyen des places ......... 96

§ 3. Valuations ......................................................... 97
    1. Valuations sur un anneau ......................................... 97
    2. Valuations sur un corps .......................................... 98
    3. Traductions ..................................................... 101
    4. Exemples de valuations .......................................... 102
    5. Idéaux d’un anneau de valuation ................................. 104
    6. Valuations discrètes ............................................ 104
§ 4. Hauteur d’une valuation ........................................... 106
    1. Inclusion des anneaux de valuation d’un même corps .............. 106
    2. Sous-groupes isolés d’un groupe ordonné ......................... 108
    3. Comparaison des valuations ...................................... 109
    4. Hauteur d’une valuation ......................................... 110
    5. Valuations de hauteur 1 ......................................... 111
§ 5. Topologie définie par une valuation ............................... 113
    1. Topologie définie par une valuation ............................. 113
    2. Espaces vectoriels topologiques sur un corps muni d’une
        valuation ...................................................... 116
    3. Complétion d’un corps muni d’une valuation ...................... 117
§ 6. Valeurs absolues .................................................. 118
    1. Préliminaires sur les valeurs absolues .......................... 118
    2. Valeurs absolues ultramétriques ................................. 120
    3. Valeurs absolues sur Q .......................................... 121
    4. Structure des corps munis d’une valeur absolue non ultramé-
        trique ......................................................... 123
§ 7. Théorème d’approximation .......................................... 128
    1. Intersection d’un nombre fini d’anneaux de valuation ............ 128
    2. Valuations indépendantes ........................................ 130
    3. Cas des valeurs absolues ........................................ 132
§ 8. Prolongements d’une valuation à une extension algébrique .......... 133
    1. Indice de ramification. Degré résiduel .......................... 133
    2. Prolongement d’une valuation et complétion ...................... 136
    3. La relation $ \sum e_i f_i \leq n $ ............................. 138
    4. Indice initial de ramification .................................. 141
    5. La relation $ \sum e_i f_i = n $ ................................ 142
    6. Anneaux de valuation dans une extension algébrique .............. 147
    7. Prolongement des valeurs absolues ............................... 149
§ 9. Application : corps localement compacts ........................... 151
    1. Fonction module sur un corps localement compact ................. 151
    2. Existence de représentants ...................................... 153
    3. Structure des corps localement compacts ......................... 154
§ 10. Prolongements d’une valuation à une extension transcendante ...... 156
    1. Cas d’une extension transcendante monogène ...................... 156
    2. Rang rationnel d’un groupe commutatif ........................... 159
    3. Cas d’une extension transcendante quelconque .................... 161
Exercices du § 1 ....................................................... 164
Exercices du § 2 ....................................................... 167
Exercices du § 3 ....................................................... 169
Exercices du § 4 ....................................................... 171
Exercices du § 5 ....................................................... 177
Exercices du § 6 ....................................................... 181

Exercices du § 7 ....................................................... 182
Exercices du § 8 ....................................................... 183
Exercices du § 9 ....................................................... 191
Exercices du § 10 ...................................................... 193

CHAPITRE VII. — Diviseurs .............................................. 195
§ 1. Anneaux de Krull .................................................. 195
    1. Idéaux divisoriels d’un anneau intègre .......................... 195
    2. Structure de monoïde sur D(A) ................................... 198
    3. Anneaux de Krull ................................................ 200
    4. Valuations essentielles d’un anneau de Krull .................... 203
    5. Approximation pour les valuations essentielles .................. 206
    6. Idéaux premiers de hauteur 1 d’un anneau de Krull ............... 207
    7. Application : nouvelles caractérisations des anneaux de
        valuation discrète ............................................. 209
    8. Fermeture intégrale d’un anneau de Krull dans une extension
        finie de son corps des fractions ............................... 209
    9. Anneaux de polynômes sur un anneau de Krull ..................... 210
    10. Classes de diviseurs dans les anneaux de Krull ................. 212
§ 2. Anneaux de Dedekind ............................................... 216
    1. Définition des anneaux de Dedekind .............................. 216
    2. Caractérisations des anneaux de Dedekind ........................ 217
    3. Décomposition des idéaux en produits d’idéaux premiers .......... 219
    4. Théorème d’approximation dans les anneaux de Dedekind ........... 220
    5. Le théorème de Krull-Akizuki .................................... 223
§ 3. Anneaux factoriels ................................................ 226
    1. Définition des anneaux factoriels ............................... 226
    2. Caractérisation des anneaux factoriels .......................... 226
    3. Décomposition en éléments extrémaux ............................. 228
    4. Anneaux de fractions d’un anneau factoriel ...................... 229
    5. Anneaux de polynômes sur un anneau factoriel .................... 229
    6. Anneaux factoriels et anneaux de Zariski ........................ 231
    7. Préliminaires sur les automorphismes des anneaux de séries
        formelles ...................................................... 231
    8. Le théorème de préparation ...................................... 232
    9. Factorialité des anneaux de séries formelles .................... 236
§ 4. Modules sur les anneaux noethériens intégralement clos ............ 237
    1. Réseaux ......................................................... 238
    2. Dualité ; modules réflexifs ..................................... 243
    3. Construction locale de modules réflexifs ........................ 248
    4. Pseudo-isomorphismes ............................................ 250
    5. Diviseurs attachés aux modules de torsion ....................... 254
    6. Invariant relatif de deux réseaux ............................... 257
    7. Classes de diviseurs attachées aux modules de type fini ......... 259
    8. Propriétés relatives aux extensions finies de l’anneau des
        scalaires ...................................................... 263
    9. Un théorème de réduction ........................................ 269
    10. Modules sur les anneaux de Dedekind ............................ 272
Exercices du § 1 ....................................................... 275
Exercices du § 2 ....................................................... 285
Exercices du § 3 ....................................................... 291

Exercices du § 4 ....................................................... 299
Note historique (chap. I à VII) ........................................ 307
Index des notations .................................................... 335
Index terminologique ................................................... 337
Tableau des stabilités I ............................................... 348
Tableau des stabilités II .............................................. 349
Stabilités par complétion .............................................. 350
Tableau des implications ............................................... 351

Dans ce tableau et le suivant, chaque ligne correspond à une propriété que peut posséder un anneau, et chaque colonne à un anneau déduit de l’anneau A. L’anneau A est supposé posséder la propriété indiquée dans la ligne : le mot « oui » (resp. « non ») à l’intersection de cette ligne et d’une colonne veut dire qu’il est vrai (resp. faux) que tout anneau construit à partir de A par le procédé indiqué par la colonne a la propriété indiquée par la ligne.

Les références renvoient à l’endroit de ce Livre ou du Livre d’Algèbre où le résultat en question est démontré.

Dans ce tableau, p désigne un idéal premier de l’anneau (commutatif) A, S une partie multiplicative de A ne contenant pas 0, et A’ la fermeture intégrale de A (supposé intègre) dans une extension de degré fini L du corps des fractions K de A.

<table>
  <tr>
    <th></th>
    <th>A/p</th>
    <th>S<sup>-1</sup> A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A principal</td>
    <td>OUI</td>
    <td>OUI</td>
    <td>NON<br>A, VII, p. 48, exerc. 1</td>
    <td>NON</td>
    <td>NON<br>A, VII, p. 51, exerc. 12</td>
  </tr>
  <tr>
    <td>A anneau de Dedekind</td>
    <td>OUI</td>
    <td>OUI<br>VII, § 2, n° 1, exemple 4</td>
    <td>NON<br>VIII, § 1, n° 3, exemple 4</td>
    <td>NON<br>VII, § 1, exerc. 9</td>
    <td>OUI<br>VII, § 2, cor. 2 de la prop. 5</td>
  </tr>
  <tr>
    <td>A anneau factoriel</td>
    <td>NON<br>V, § 1, exerc. 9</td>
    <td>OUI<br>VII, § 3, prop. 3</td>
    <td>OUI<br>VII, § 3, th. 2</td>
    <td>NON (*)<br>VII, § 3, exerc. 8</td>
    <td>NON<br>A, VII, p. 51, exerc. 12</td>
  </tr>
  <tr>
    <td>A noethérien intégralement clos</td>
    <td>NON<br>V, § 1, exerc. 9</td>
    <td>OUI<br>V, § 1, cor. 1 de la prop. 16 et II, § 2, cor. 2 de la prop. 10</td>
    <td>OUI<br>V, § 1, cor. 1 de la prop. 13 et III, § 2, cor. 1 du th. 2</td>
    <td>OUI<br>V, § 1, prop. 14 et III, § 2, cor. 6 du th. 2</td>
    <td>NON (**)<br>V, § 1, exerc. 21</td>
  </tr>
  <tr>
    <td>A corps ou anneau de valuation discrète</td>
    <td>OUI<br>VI, § 3, n° 6</td>
    <td>OUI<br>VI, § 3, n° 6</td>
    <td>NON</td>
    <td>NON<br>VI, § 1, n° 4</td>
    <td>NON<br>V, § 1 exerc. 13</td>
  </tr>
  <tr>
    <td>A corps ou anneau de valuation de hauteur 1</td>
    <td>OUI<br>VI, § 4,</td>
    <td>OUI<br>VI, § 4, prop. 1</td>
    <td>NON</td>
    <td>NON<br>VI, § 1, n° 4</td>
    <td>NON<br>V, § 1 exerc. 13</td>
  </tr>
  <tr>
    <td>A anneau de valuation</td>
    <td>OUI<br>VI, § 1, th. 1</td>
    <td>OUI<br>VI, § 1, th. 1</td>
    <td>NON</td>
    <td>NON<br>VI, § 1, n° 4</td>
    <td>NON<br>V, § 1 exerc. 13</td>
  </tr>
  <tr>
    <td>A anneau de valuation complet</td>
    <td>NON</td>
    <td>OUI<br>VI, § 7, prop. 3</td>
    <td>NON</td>
    <td>NON<br>VI, § 1, n° 4</td>
    <td>NON<br>V, § 1 exerc. 13</td>
  </tr>
  <tr>
    <td>A anneau de Krull</td>
    <td>NON<br>V, § 1, exerc. 9</td>
    <td>OUI<br>VII, § 1, prop. 6</td>
    <td>OUI<br>VII, § 1, prop. 13</td>
    <td>OUI<br>VII, § 1, exerc. 9</td>
    <td>OUI<br>VII, § 1, prop. 12</td>
  </tr>
</table>

(*) OUI, cependant, si l’anneau A est principal (VII, § 3, exerc. 9).

(**) OUI, cependant, si l’extension L de K est séparable (V, § 1, cor. 1 de la prop. 18).

Dans ce tableau, $ a $ désigne un idéal de $ A $ distinct de $ A $, $ S $ une partie multiplicative de $ A $, et $ A' $ la clôture intégrale de $ A $, supposé intègre.

<table>
  <tr>
    <th></th>
    <th>A/a</th>
    <th>S^{-1}A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A local</td>
    <td>OUI</td>
    <td>NON<br>II, § 2,<br>prop. 11</td>
    <td>NON</td>
    <td>OUI<br>A, IV, p. 26,<br>prop. 6</td>
    <td>NON<br>V, § 2,<br>exerc. 20</td>
  </tr>
  <tr>
    <td>A local séparé et complet</td>
    <td>NON<br>OUI si A est noethérien (III, § 3,<br>prop. 6)</td>
    <td>NON<br>II, § 2<br>prop. 11</td>
    <td>NON</td>
    <td>OUI<br>III, § 2,<br>prop. 6</td>
    <td>NON (*)</td>
  </tr>
  <tr>
    <td>A semi-local</td>
    <td>OUI</td>
    <td>NON<br>II, § 2,<br>prop. 11</td>
    <td>NON</td>
    <td>OUI<br>A, IV, p. 26,<br>prop. 6</td>
    <td>NON<br>OUI si A est noethérien (V, § 2,<br>exerc. 7)</td>
  </tr>
  <tr>
    <td>A semi-local séparé et complet</td>
    <td>NON<br>OUI si A est noethérien (III, § 3,<br>prop. 6)</td>
    <td>NON<br>II, § 2,<br>prop. 11</td>
    <td>NON</td>
    <td>OUI<br>III, § 2,<br>prop. 6</td>
    <td></td>
  </tr>
  <tr>
    <td>A noethérien</td>
    <td>OUI<br><i>Alg.</i> VIII, § 2,<br>prop. 6</td>
    <td>OUI<br>II, § 2, cor. 2<br>de la prop. 10</td>
    <td>OUI<br>III, § 2,<br>cor. 1 du th. 2</td>
    <td>OUI<br>III, § 2,<br>cor. 6 du th. 2</td>
    <td>NON (*)<br>V, § 1,<br>exerc. 21,<br>mais A' est un anneau de Krull<br>(IX, § 4,<br>exerc. 14)</td>
  </tr>
</table>

(*) Cependant si l’anneau $ A $ est un anneau local noethérien intègre, séparé et complet, l’anneau $ A' $ possède les mêmes propriétés (IX, § 4, cor. du th. 2 et lemme 1).

a) Soient $ A $ un anneau, et $ m $ un idéal de $ A $ distinct de $ A $. On munit $ A $ de la topologie $ m $-adique, et on note $ \hat{A} $ son séparé complété.

$$
\begin{array}{ll}
\text{A séparé} & \text{OUI} \\
\text{A noethérien} & \text{OUI (III, § 3, prop. 8)} \\
\text{A local} & \text{OUI (*)} \\
\text{A semi-local} & \text{OUI (*)} \\
\text{A anneau de Zariski} & \text{OUI (III, § 3, prop. 8)} \\
& (*) \text{En effet } \hat{m} \text{ est contenu dans le radical de } \hat{A} \text{ (III, § 2, n° 13, lemme 3) et l'homomorphisme cononique } A/m \to \hat{A}/\hat{m} \text{ est bijectif (III, § 2, n° 12, formule (21))}.
\end{array}
$$

b) On suppose maintenant que $ A $ est local noethérien, et que $ m $ est son idéal maximal.

$$
\begin{array}{ll}
\text{A intègre} & \text{NON (III, § 3, exerc. 15 b))} \\
\text{A intégralement clos} & \text{NON (1)} \\
\text{A anneau de valuation discrète} & \text{OUI pour les anneaux excellents (2)} \\
\text{A réduit} & \text{OUI (VI, § 5, prop. 5)} \\
& \text{NON (IX, § 4, exerc. 1 et V, § 1, exerc. 20)} \\
& \text{OUI pour les anneaux de Nagata (IX, § 4, prop. 4)}
\end{array}
$$

(1) M. Nagata, Local rings, Interscience (New York), 1962.
(2) A. Grothendieck, Eléments de Géométrie algébrique, chap. IV (Publ. Inst. Htes Etudes Scient., n°s 20 et 24, 1964).

anneau réduit
    ↑
anneau intègre
    ↑
anneau intégralement clos
    ↑ (*)
anneau complètement intégralement clos
    ↑ (*)
anneau de Krull
anneau noethérien
    ↼
anneau de Dedekind
    ↼
anneau principal
    ↼
anneau factoriel
    ↼
anneau semi-local
    ↑
anneau local
    ↑
anneau de valuation
    ↑
anneau de valuation de hauteur 1
    ↑
(*)
anneau de valuation discrète

Les flèches signalées par un astérisque (*) sont des équivalences dans le cas des anneaux noethériens.
