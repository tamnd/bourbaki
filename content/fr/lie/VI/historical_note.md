---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: Systèmes de racines
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0233-0284
extraction: ocr
statements: 0
exercises: 0
content_sha256: 9626f48d30bbf5ac4033c626e916e4dee9a97eaa41ff146764e30635b34b9467
---

# NOTE HISTORIQUE

(N.B. — Les chiffres romains placés entre parenthèses renvoient à la bibliographie placée à la fin de cette note).

Les groupes étudiés dans ces chapitres sont apparus à propos de questions variées de Géométrie, d’Analyse et de Théorie des groupes de Lie, tantôt sous forme de groupes de permutations, tantôt sous forme de groupes de déplacements en géométrie euclidienne ou hyperbolique, et ces divers points de vue n’ont été coordonnés qu’à date récente.

Historiquement, les débuts de la théorie sont bien antérieurs à l’introduction du concept de groupe : elle prend en effet sa source dans les études sur la « régularité » ou les « symétries » des figures géométriques, et notamment dans la détermination des polygones et des polyèdres réguliers (remontant sans doute aux Pythagoriciens), qui constitue le couronnement des Éléments d’Euclide, et une des créations les plus admirables du génie grec. Plus tard, notamment chez les auteurs arabes du haut Moyen âge, puis chez Képler, apparaissent les débuts d’une théorie mathématique des « pavages » réguliers du plan ou de la sphère par des polygones congruents deux à deux (mais non nécessairement réguliers), sans doute liés à l’origine aux divers types d’ornements imaginés par les civilisations antiques et arabe (que l’on peut à bon droit considérer comme une partie authentique des mathématiques développées par ces civilisations (XII)).

Vers 1830-1840, les études de cristallographie (Hessel, Bravais, Möbius) conduisent à étudier un problème qui est exactement celui de la détermination des groupes finis de déplacements dans l’espace euclidien à 3 dimensions, bien que les auteurs précités n’usent pas encore du langage de la théorie des groupes ; ce dernier n’entre guère dans l’usage que vers 1860, et c’est sous forme de classification de groupes que Jordan, en 1869 (VI), détermine les sous-groupes discrets de déplacements de $\mathbf{R}^3$ conservant l’orientation (et plus généralement, tous les sous-groupes fermés du groupe des déplacements conservant l’orientation).

Jusqu’aux dernières années du xixe siècle, ce courant d’idées se développe dans plusieurs directions, dont les plus marquantes sont les suivantes :
1° Conformément à une tendance qui apparaît de très bonne heure dans la théorie des groupes finis, on cherche à « présenter » les groupes finis de déplacements par des générateurs et relations d’un type simple. C’est ainsi que Hamilton, dès 1856 (V), prouve que les groupes finis de rotations dans l’espace euclidien $\mathbf{R}^3$ sont engendrés par deux générateurs S, T liés par les relations $S^p = T^q = (ST)^3 = 1$ pour des valeurs convenables de $p$ et $q$.
2° Les groupes discrets de déplacements peuvent ou non contenir des réflexions. Dès 1852, Möbius détermine en substance les groupes finis de déplacements en géométrie sphérique engendrés par des réflexions (ce qui est équivalent au même problème pour les groupes finis de déplacements euclidiens dans $\mathbf{R}^3$); il trouve qu’exception faite des groupes cycliques, un tel groupe a pour domaine fondamental un triangle sphérique ayant des angles de la forme $\pi/p, \pi/q, \pi/r$, où $p, q, r$ sont trois entiers > 1 tel que $\frac{1}{p} + \frac{1}{q} + \frac{1}{r} > 1$ (III) (cf. chap. V, § 4, exerc. 4). Il constate aussi que ces groupes contiennent tous les groupes finis de déplacements comme sous-groupes.
3° Ce dernier courant d’idées trouve une amplification nouvelle lorsqu’à la suite des travaux de Riemann et Schwarz sur les fonctions hypergéométriques et la représentation conforme, commence l’étude des « pavages » du plan complexe ou du demi-plan par des figures limitées par des arcs de cercle; Klein et Poincaré en font le fondement de la théorie des « fonctions automorphes », et y reconnaissent (pour le cas des arcs de cercle orthogonaux à une droite fixe) un problème équivalent à celui de la recherche des sous-groupes discrets du groupe des déplacements du plan non-euclidien hyperbolique (identifié au « demi-plan de Poincaré ») (X).
4° Les notions de polyèdre régulier et de pavage de $\mathbf{R}^3$ par de tels polyèdres sont étendues à tous les espaces euclidiens $\mathbf{R}^n$ par Schlafli, dans un travail qui remonte aux environs de 1850, mais ne fut publié que beaucoup plus tard et resta longtemps ignoré (IV); il détermine complètement les « polytopes » réguliers dans chaque $\mathbf{R}^n$, le groupe des déplacements laissant invariant un tel polytope, et un domaine fondamental de ce groupe, qui, comme dans le cas $n = 3$ étudié par Möbius, est une « chambre » dont la trace sur la sphère $\mathbf{S}_{n-1}$ est un simplexe sphérique. Toutefois, il n’aborde pas le problème inverse de la recherche des groupes finis de déplacements engendrés par des réflexions dans $\mathbf{R}^n$; ce problème ne sera résolu que beaucoup plus tard, par Goursat (VII) pour $n = 4$, et, pour $n$ quelconque, sa solution devra attendre les travaux de E. Cartan (IX f)) et de Coxeter (XIV), sur lesquels nous reviendrons plus bas.

\* \* \*

Vers 1890, avec les premiers travaux de Killing et de E. Cartan sur les groupes de Lie, débute un nouveau courant d’idées qui pendant longtemps se développera sans lien avec les précédents. Killing (VIII) et Cartan (IX a)), dans leur étude de la structure des algèbres de Lie semi-simples complexes, font tout de suite jouer un rôle primordial à certaines formes linéaires $\omega_\alpha$ sur une « sous-algèbre de Cartan » $\mathfrak{h}$ d’une telle algèbre de Lie $\mathfrak{g}$; ce sont les « racines » relatives à $\mathfrak{h}$, ainsi nommées parce que chez Killing elles apparaissent comme les racines de l’équation caractéristique $\det(\mathrm{ad}_\mathfrak{g}(x) - T) = 0$, considérées comme fonctions de $x \in \mathfrak{h}$. Les propriétés de ces « racines » établies par Killing et Cartan reviennent à affirmer que, dans le langage géométrique du chap. VI, elles forment un « système de racines réduit » (cf. chap. VI, § 1, no 4); ils montrent ensuite que la classification des algèbres de Lie semi-simples complexes se ramène à celle des « systèmes de racines » associés, qui elle-même se réduit à la détermination de certaines matrices à coefficients entiers (appelées plus tard « matrices de Cartan »; cf. chap. VI, § 1, no 5). Killing et Cartan mettent aussi en évidence, pour toute racine $\omega_x$, l’existence d’une permutation involutive $S_\alpha$ de l’ensemble des racines (*); ils se servent de façon essentielle de la transformation $C = S_{\alpha_1} S_{\alpha_2} \ldots S_{\alpha_l}$, produit des permutations associées à $l$ racines formant un système fondamental (transformation appelée à présent « transformation de Coxeter »); ils étendent même cette permutation en une transformation linéaire de l’espace vectoriel engendré par les racines fondamentales $\omega_{\alpha_i}$ ($1 \leq i \leq l$), et étudient ses valeurs propres ((VIII, II)), p. 20; (IX, a), p. 58). Mais ni Killing, ni tout d’abord Cartan, ne paraissent songer à considérer le groupe $\mathcal{G}'$ engendré par les $S_\alpha$; et lorsque Cartan, un peu plus tard (IX b)), détermine le groupe de Galois $\mathcal{G}$ de l’équation caractéristique

$$
\det(\mathrm{ad}_\mathfrak{g}(x) - T) = 0
$$

d’un « élément général » $x \in \mathfrak{h}$, il l’étudie d’abord sans faire intervenir les $S_\alpha$; 30 ans plus tard, déjà sous l’influence des travaux de H. Weyl, il prouve (IX c)) que $\mathcal{G}$ a pour sous-groupe distingué le groupe $\mathcal{G}'$ et détermine dans tous les cas la structure du groupe quotient $\mathcal{G}/\mathcal{G}'$ qui (pour une algèbre simple $\mathfrak{g}$) est d’ordre 1 ou 2 sauf pour le type $D_4$ où il est isomorphe à $S_3$; c’est aussi à cette occasion qu’il interprète $\mathcal{G}'$ comme groupe induit par les automorphismes intérieurs d’une algèbre de Lie semi-simple complexe, laissant stable une sous-algèbre de Cartan (**).

Les travaux de H. Weyl, auxquels nous venons de faire allusion, sont ceux qui inaugurent l’interprétation géométrique du groupe $\mathcal{G}'$ (appelé depuis « groupe de Weyl » de $\mathfrak{g}$); de même que Killing et Cartan l’avaient fait pour la transformation $C$, il a l’idée de considérer les $S_\alpha$ comme des réflexions dans l’espace vectoriel des formes linéaires sur $\mathfrak{h}$. C’est aussi dans le mémoire de

(*) Les notations $\omega_\alpha$ et $S_\alpha$ correspondent respectivement aux notations $\alpha$ et $s_\alpha$ du chap. VI, § 1.
(**) Les notations $\mathcal{G}$ et $\mathcal{G}'$ correspondent respectivement aux notations $\mathrm{A}(\mathbf{R})$ et $\mathrm{W}(\mathbf{R})$ du chap. VI, § 1, no 1.

H. Weyl (XIII) que l’on voit apparaître le domaine fondamental du « groupe de Weyl affine » (sans d’ailleurs que le lien avec le « groupe de Weyl » $\mathfrak{g}'$ soit très clairement indiqué); Weyl l’utilise pour prouver que le groupe fondamental d’un groupe compact semi-simple est fini, point capital dans sa démonstration de la complète réductibilité des représentations linéaires d’une algèbre de Lie semi-simple complexe. Peu après, E. Cartan réalise la synthèse des points de vue globaux de H. Weyl, de sa propre théorie des algèbres de Lie semi-simples réelles ou complexes, et de la théorie des espaces riemanniens symétriques qu’il édifiait à cette époque. Dans le mémoire (IX d)), il complète la détermination des polytopes fondamentaux du groupe de Weyl et du groupe de Weyl affine, et introduit les réseaux des poids et des poids radiciels (chap. VI, § 1, n° 9); dans (IX e)), il étend cette discussion aux espaces symétriques, et rencontre ainsi notamment les premiers exemples de systèmes de racines non réduits (chap. VI, § 4, n° 1). Enfin l’article (IX f)) donne la première démonstration du fait que tout groupe fini engendré par des réflexions dans $\mathbf{R}^n$ et irréductible a un domaine fondamental ayant pour trace sur $S_{n-1}$ un simplexe sphérique; c’est aussi dans ce travail qu’il prouve l’unicité de la plus grande racine (pour un ordre lexicographique quelconque sur un système de racines) par des considérations géométriques.

Un peu plus tard, van der Waerden (XVI), s’appuyant sur le mémoire de H. Weyl, montre que la classification des algèbres de Lie semi-simples complexes équivaut à celle des systèmes de racines réduits, qu’il effectue par des considérations géométriques élémentaires (alors que, chez Killing et Cartan, cette classification résulte de calculs compliqués de déterminants). À peu près en même temps, Coxeter détermine explicitement tous les groupes finis irréductibles de déplacements euclidiens qui sont engendrés par des réflexions (XIV c)); il complète ainsi les résultats du mémoire (IX d)) de E. Cartan, qui n’avait déterminé que les groupes « cristallographiques » (i.e. associés à un système de racines, ou encore susceptibles d’être plongés dans un groupe discret infini de déplacements). L’année suivante (XIV d)), Coxeter montre que les groupes finis engendrés par des réflexions sont les seuls groupes finis (à isomorphie près) admettant une présentation par des générateurs involutifs $R_i$ soumis à des relations de la forme $(R_i R_j)^{m_{ij}} = 1$ ($m_{ij}$ entiers), d’où le nom de « groupes de Coxeter » donnés depuis aux groupes (finis ou non) admettant une telle présentation.

**Le premier lien entre les deux courants de recherche que nous avons décrits ci-dessus semble avoir été établi par Coxeter (XIV bis), puis par Witt (XVII). Ils constatent que les groupes irréductibles infinis de déplacements euclidiens engendrés par des réflexions correspondent biunivoquement (à isomorphisme près) aux algèbres de Lie simples complexes. Witt donne une nouvelle détermination des groupes discrets de ce type, et étend en outre le th. de Coxeter de (XIV d)) rappelé ci-dessus en caractérisant également les groupes de Coxeter isomorphes aux groupes discrets infinis de déplacements euclidiens. Ce résultat, et le fait que les groupes analogues en géométrie hyperbolique sont aussi des groupes de Coxeter (*) a conduit à aborder franchement l’étude de ces derniers, tout d’abord (cf. chap. V, § 4) en mettant l’accent sur une réalisation géométrique ((XV), (XXV)), puis, à la suite de J. Tits (XXV) dans le cadre purement algébrique adopté dans ce traité (chap. IV, § 1).

A partir des travaux de Witt, la théorie des groupes de Lie semi-simples et celles des groupes discrets engendrés par des réflexions ne vont cesser de réagir de façon extrêmement fructueuse l’une sur l’autre. Dès 1941, Stiefel (XVIII) remarque que les groupes de Weyl sont exactement les groupes finis engendrés par des réflexions, et qui laissent invariant un réseau. Chevalley (XIX a)) et Harish-Chandra (XX a)) donnent en 1948-51 des démonstrations $a\ priori$ de la correspondance biunivoque entre groupes « cristallographiques » et algèbres de Lie semi-simples complexes; on ne savait jusque là que vérifier séparément cette correspondance sur chaque type d’algèbre de Lie simple.

Vers 1950, on remarque d’autre part que les polynômes invariants par le groupe de Weyl jouent un rôle important en théorie des représentations linéaires de dimension infinie (XX a)) et dans la topologie des groupes de Lie. De son côté, Coxeter (XIV f )), reprenant l’étude de la transformation $C$, produit des réflexions fondamentales d’un groupe fini $W$ engendré par des réflexions, constate (par un examen séparé de chaque type) que l’algèbre des polynômes invariants par $W$ est engendré par des éléments algébriquement indépendants, dont les degrés sont liés de façon simple aux valeurs propres de $C$ (cf. chap. V, §§ 5 et 6). Des démonstrations $a\ priori$ de ces résultats furent ensuite données par Chevalley (XIX b)) pour le premier, et par Coleman (XXIII) et Steinberg (XXIV) pour le second.

\* \*

Avec le travail de A. Borel sur les groupes algébriques linéaires (XXII) commencent de nouveaux développements de la théorie des groupes de Lie qui devaient conduire à un notable élargissement de celle-ci. A. Borel met en évidence l’importance des sous-groupes résolubles connexes maximaux (appelés depuis « sous-groupes de Borel ») dans un groupe de Lie, et en fait l’outil principal pour transposer une grande partie de la théorie classique aux groupes algébriques sur un corps algébriquement clos (sans toutefois obtenir encore une classification des groupes algébriques simples (**)). Les sous-groupes

(*) Ces groupes, étudiés à fond dans le cas de dimension 2, n’ont été considérés en dimension $\geqslant 3$ qu’incidemment jusqu’à ces dernières années.
(**) Un groupe algébrique de dimension $> 0$ est dit *simple* (au sens de la géométrie algébrique) s’il ne contient aucun sous-groupe distingué algébrique de dimension $> 0$ autre que lui-même. Il est dit *semi-simple* s’il est isogène à un produit de groupes simples non commutatifs.

de Borel (dans le cas des groupes classiques réels ou complexes) étaient déjà intervenus quelques années auparavant dans les travaux de Gelfand et Neumark sur les représentations de dimension infinie; et en 1954, F. Bruhat avait découvert le fait remarquable que, pour les groupes simples classiques, la décomposition du groupe en doubles classes suivant un groupe de Borel est indexée de façon canonique par le groupe de Weyl (XXI). Ce résultat fut ensuite étendu à tous les groupes semi-simples réels et complexes par Harish-Chandra (XX b)). D’autre part, en 1955, Chevalley (XIX c)) avait réussi à associer à toute algèbre de Lie semi-simple complexe g et à tout corps commutatif k, un groupe de matrices à coefficients dans k, possédant une décomposition de Bruhat; et il utilisa ce dernier fait pour montrer qu’à un petit nombre d’exceptions près, le groupe ainsi défini était simple (au sens de la théorie des groupes abstraits). Il « expliquait » ainsi la coïncidence, déjà observée depuis Jordan et Lie, entre les groupes de Lie simples (au sens de la théorie des groupes de Lie) des types A, B, C, D et les groupes simples classiques définis de façon purement algébrique sur un corps quelconque (coïncidence qui n’avait pu jusque là être étendue qu’au type exceptionnel G_2 par Dickson (XI)). En particulier, en prenant un corps fini k, la construction de Chevalley fournit, pour chaque type d’algèbre de Lie simple complexe, une famille de groupes simples finis, contenant une grande partie des groupes simples finis connus jusqu’alors, ainsi que quatre nouvelles séries (correspondant aux types d’algèbres de Lie simples F_4, E_6, E_7 et E_8). Peu après, par divers procédés, utilisant des modifications des méthodes de Chevalley, plusieurs auteurs (Hertzig, Suzuki, Ree, Steinberg et Tits) d’une part montrèrent que l’on peut obtenir de façon analogue les autres groupes simples finis connus à cette époque, à l’exception des groupes alternés et des groupes de Mathieu, et d’autre part construisirent d’autres séries de nouveaux groupes simples finis (cf. (XXIX)).

Presqu’en même temps, Chevalley (XIX d)), utilisant toujours la technique des décompositions de Bruhat, jointe à un résultat clé sur le normalisateur d’un sous-groupe de Borel, reprenait l’étude des groupes linéaires algébriques et parvenait au résultat que sur un corps algébriquement clos k de caractéristique quelconque, la théorie des groupes linéaires algébriques semi-simples (*) conduit essentiellement aux mêmes types que dans la classification de Killing-Cartan pour k = \mathbf{C}. Par la suite, J. Tits (XXV a) et b)), en analysant les méthodes de Chevalley, est parvenu à une version axiomatisée (les « BN-paires ») des décompositions de Bruhat, sous une forme remarquablement souple, ne faisant intervenir que la structure de groupe; c’est cette notion qui a été exposée sous le nom de « système de Tits » au chap. IV, § 2. Tous les groupes simples (aux divers sens du mot) dont il a été question plus haut sont canoniquement munis de systèmes de Tits, et Tits lui-même (XXV c)) a prouvé que l’existence

(*) L’existence de nombreuses algèbres de Lie simples « pathologiques » sur un corps de caractéristique $p > 0$ avait pu faire douter certains du caractère universel de la classification de Killing-Cartan.

d’un tel système dans un groupe abstrait G, jointe à quelques propriétés supplémentaires de pure théorie des groupes, permet de démontrer que G est simple, théorème qui couvre la plupart des démonstrations de simplicité données jusque-là pour ces groupes (cf. chap. IV, § 2 n° 6). En collaboration avec A. Borel, il a d’autre part généralisé les résultats de Chevalley de (XIX d)), en montrant l’existence de systèmes de Tits dans le groupe des points rationnels d’un groupe algébrique linéaire semi-simple sur un corps quelconque (XXVII).

Tous les systèmes de Tits rencontrés dans ces questions ont un groupe de Weyl fini. Une autre catégorie d’exemples a été découverte par Iwahori et Matsumoto (XXVI); ils ont montré que si, dans la construction de Chevalley de (XIX c)), k est un corps $p$-adique, alors le groupe obtenu a un système de Tits dont le groupe de Weyl est le groupe de Weyl affine de l’algèbre de Lie semi-simple complexe d’où l’on est parti. Ce résultat vient d’être étendu par Bruhat et Tits (XXVIII) à tous les groupes algébriques semi-simples sur un corps local.

(I) J. HESSEL, Krystallometrie oder Krystallonomie und Krystallographie (1830, repr. dans Ostwald’s Klassiker, nos 88 et 89, Leipzig (Teubner), 1897).

(II) A. BRAVAIS, Mémoires sur les polyèdres de forme symétrique, Journal de Math., (1), t. XIV (1849), p. 141-180.

(III) A. MöBIUS : a) Ueber das Gesetz der Symmetrie der Krystalle und die Anwendung dieses Gesetze auf die Eintheilung der Krystalle in Systeme, J. de Crelle, t. XLIII (1852), p. 365-374 (= Gesammelte Werke, t. II, Leipzig (Hirzel), 1886, p. 349-360); b) Theorie der symmetrischen Figuren, Gesammelte Werke, t. II, Leipzig (Hirzel), 1886, p. 561-708.

(IV) L. SCHLÄFLI, Theorie der vielfachen Kontinuität, Denkschr. der Schweiz. naturforsch. Gesellschaft, t. XXXVIII (1901), p. 1-237 (= Ges. math. Abhandlungen, t. I, Basel (Birkhäuser), 1950, p. 167-387).

(V) W. R. HAMILTON, Memorandum respecting a new system of roots of unity, Phil. Mag., (4) t. XII (1856), p. 446.

(VI) C. JORDAN, Mémoire sur les groupes de mouvements, Ann. di Mat., t. II (1868-69), p. 167-215 et 322-345 (= Œuvres, t. IV, Paris (Gauthier-Villars), 1964, p. 231-302).

(VII) E. GOURSAT, Sur les substitutions orthogonales et les divisions régulières de l’espace, Ann. Ec. Norm. Sup., (3), t. VI (1889), p. 9-102.

(VIII) W. KILLING, Die Zusammensetzung der stetigen endlichen Transformationsgruppen : I) Math. Ann., t. XXXI (1888), p. 252-290; II), ibid., t. XXXIII (1889), p. 1-48; III) ibid., t. XXXIV (1889), p. 57-122; IV) ibid., t. XXXVI (1890), p. 161-189.

(IX) E. CARTAN : a) Sur la structure des groupes de transformations finis et continus (Thèse), Paris (Nony), 1894 (= Œuvres complètes, Paris, (Gauthier-Villars), 1952, t. I₁, p. 137-287); b) Sur la réduction à sa forme canonique de la structure d’un groupe de transformations fini et continu, Amer. Journ. of Math., t. XVIII (1896), p. 1-46 (= Œuvres complètes, t. I₁, p. 293-353); c) Le principe de dualité et la théorie des groupes simples et semi-simples, Bull. Sci. Math., t. XLIX (1925), p. 361-374 (= Œuvres complètes, t. I₁, p. 555-568); d) La géométrie des groupes simples, Ann. di Mat., (4), t. IV (1927), p. 209-256 (= Œuvres complètes, t. I₂, p. 793-840); e) Sur certaines formes riemanniennes remarquables des géométries à groupe fondamental simple, Ann. Ec. Norm. Sup., (3), t. XLIV (1927), p. 345-467 (= Œuvres complètes, t. I₂, p. 867-989); f) Complément au mémoire « Sur la géométrie des groupes simples », Ann. di Mat., (4), t. V (1928), p. 253-260 (= Œuvres complètes, t. I₂, p. 1003-1010).

(X) R. Fricke und F. Klein, Theorie der automorphen Funktionen, Leipzig (Teubner), 1897.

(XI) L. E. Dickson : a) Theory of linear groups in an arbitrary field, Trans. Amer. Math. Soc., t. II (1901), p. 363-394; b) A new system of simple groups, Math. Ann., t. LX (1905), p. 137-150.

(XII) A. Speiser, Theorie der Gruppen von endlicher Ordnung, Berlin (Springer), 1924.

(XIII) H. Weyl, Theorie der Darstellung kontinuierlicher halb-einfacher Gruppen durch lineare Transformationen, Math. Zeitschr., t. XXIII (1925), p. 271-309, t. XXIV (1926), p. 328-395 et 789-791 (= Selecta, Basel-Stuttgart (Birkhäuser), 1956, p. 262-366).

(XIV) H. S. M. Coxeter : a) Groups whose fundamental regions are simplex, Journ. Lond. Math. Soc., t. VI (1931), p. 132-136; b) The polytopes with regular prismatic figures, Proc. Lond. Math. Soc., (2), t. XXXIV (1932), p. 126-189; c) Discrete groups generated by reflections, Ann. of Math., (2), t. XXXV (1934), p. 588-621; d) The complete enumeration of finite groups of the form $R_i^2 = (R_i . R_j)^{k_{ij}} = 1$, Journ. Lond. Math. Soc., t. X (1935), p. 21-25; e) Regular polytopes, New York (Macmillan), 1948 (2e éd., 1963); f) The product of generators of a finite group generated by reflections, Duke Math. Journ., t. XVIII (1951), p. 765-782.

(XIV bis) H. S. M. Coxeter in H. Weyl, The structure and representation of continuous groups (Inst. for Adv. Study, notes miméographiées par N. Jacobson et R. Brauer, 1934-35) : Appendix.

(XV) H. S. M. Coxeter and W. O. J. Moser, Generators and relations for discrete groups, Ergeb. der Math., Neue Folge, Bd. 14, Berlin (Springer), 1957 (2e éd., 1965).

(XVI) B. L. van der Waerden, Die Klassification der einfachen Lieschen Gruppen, Math. Zeitschr., t. XXXVII (1933), p. 446-462.

(XVII) E. Witt, Spiegelungsgruppen und Aufzählung halbeinfacher Liescher Ringe, Abh. Math. Sem. Hamb. Univ., t. XIV (1941), p. 289-322.

(XVIII) E. Stiefel, Ueber eine Beziehung zwischen geschlossenen Lie’sche Gruppen und diskontinuierlichen Bewegungsgruppen euklidischer Räume und ihre Anwendung auf die Aufzählung der einfachen Lie’schen Gruppen, Comm. Math. Helv., t. XIV (1941-42), p. 350-380.

(XIX) C. Chevalley : a) Sur la classification des algèbres de Lie simples et de leurs représentations, C.R. Acad. Sci., t. CCXXVII (1948), p. 1136-1138; b) Invariants of finite groups generated by reflections, Amer. Journ. of Math., t. LXXVII (1955), p. 778-782; c) Sur certains groupes simples, Tohoku Math. Journ., (2), t. VII (1955), p. 14-66; d) Classification des groupes de Lie algébriques, 2 vol., Paris (Inst. H. Poincaré), 1956-58.

(XX) Harish Chandra : a) On some applications of the universal enveloping algebra of a semi-simple Lie algebra, Trans. Amer. Math. Soc., t. LXX (1951), p. 28-96; b) On a lemma of Bruhat, Journ. de Math., (9), t. XXXV (1956), p. 203-210.

(XXI) F. Bruhat, Représentations induites des groupes de Lie semi-simples complexes, C.R. Acad. Sci., t. CCXXXVIII (1954), p. 437-439.

(XXII) A. Borel, Groupes linéaires algébriques, Ann. of Math., (2), t. LXIV (1956), p. 20-80.

(XXIII) A. J. Coleman, The Betti numbers of the simple groups, Can. Journ. of Math., t. X (1958), p. 349-356.

(XXIV) R. Steinberg, Finite reflection groups, Trans. Amer. Math. Soc., t. XCI (1959), p. 493-504.

(XXV) J. Tits : a) Groupes simples et géométries associées, Proc. Int. Congress Math., Stockholm, 1962, p. 197-221; b) Théorème de Bruhat et sous-groupes paraboliques, C.R. Acad. Sci., t. CCLIV (1962), p. 2910-2912; c) Algebraic and abstract simple groups, Ann. of Math., (2), t. LXXX (1964), p. 313-329.

(XXVI) N. Iwahori and H. Matsumoto, On some Bruhat decomposition and the structure of the Hecke rings of $p$-adic Chevalley groups, Publ. math. I.H.E.S., n° 25 (1965), p. 5-48.

(XXVII) A. Borel et J. Tits, Groupes réductifs, Publ. Math. I.H.E.S., n° 27 (1965), p. 55-150.

(XXVIII) F. Bruhat et J. Tits, Groupes algébriques simples sur un corps local, Proc. Conf. on Local Fields, p. 23-36, Berlin (Springer), 1967.

(XXIX) R. Carter, Simple groups and simple Lie algebras, Journ. Lond. Math. Soc., t. XL (1965), p. 193-240.

Les chiffres de référence indiquent successivement le chapitre, le paragraphe et le numéro.

$A_l$ (système de racines de type) : VI, 4,1; VI, 4,7 et Planche I.
$\tilde{A}_l$ : VI, 4,3.
$A[P]$ : VI, 3,1.
$A(R)$ : VI, 1,1.
$\tilde{\alpha}$ (plus grande racine) : VI, 1,8; VI, 4,3.
$\alpha_0 = -\tilde{\alpha}$ : VI, 4,3.
$(\alpha_1, \ldots, \alpha_l)$ : VI, 1,5.
B : IV, 2,1.
B(C) (base définie par la chambre C) : VI, 1,5.
$B_l$ (système de racines de type) : VI, 4,1; VI, 4,5 et Planche II.
$\tilde{B}_l$ : VI, 4,3.
$B_M$ (forme bilinéaire associée à la matrice de Coxeter $M$) : V, 4,1.
C (chambre) : V, 1,3; VI, 1,5.
c (transformation de Coxeter) : V, 6,1; VI, 1,11.
$C_l$ (système de racines de type) : VI, 4,1; VI, 4,6 et Planche III.
$\tilde{C}_l$ : VI, 4,3.
$\gamma_l, \Gamma_C$ : VI, 2,3.
$\gamma(R)$ : VI, 1,12.
$d = \prod_{\alpha > 0} (e^{\alpha/2} - e^{-\alpha/2})$ : VI, 3,3.
$D_l$ (système de racines de type) : VI, 4,1; VI, 4,8 et Planche IV.
$\tilde{D}_l$ : VI, 4,3.
E : VI, 4,4.
$E_6, E_7, E_8$ (système de racines de type) : VI, 4,1; VI, 4,10; VI, 4,11; VI, 4,12 et Planches V, VI, VII.
$\tilde{E}_6, \tilde{E}_7, \tilde{E}_8$ : VI, 4,3.
$\varepsilon_1, \ldots, \varepsilon_n$ : VI, 4,4.

F_4 (système de racines de type) : VI, 4,1; VI, 4,9 et Planche VIII.
\tilde{F}_4 : VI, 4,3.
G : VI, 2,3.
G_2 (système de racines de type) : VI, 4,1; VI, 4,13 et Planche IX.
\tilde{G}_2 : VI, 4,3.
\mathfrak{s} : V, 3,1.
h (nombre de Coxeter) : V, 6,1; VI, 1,11.
H_3, H_4 (systèmes de Coxeter de type) : VI, 4,1.
I_2(p) (système de Coxeter de type) : VI, 4,1.
J(e^p) = \sum_{w \in W} \det(w)e^{w(p)} : VI, 3,3.
L_0, L_1, L_2, L_3 (réseaux de \mathbf{R}^n) : VI, 4,4.
l(w), l_S(w) (longueur d'un élément w) : IV, 1,1.
m(s, s') : IV, 1,9.
N : IV, 2,1.
P(R) : VI, 1,9.
Q(R) : VI, 1,9.
R (système de racines) : VI, 1,1.
R^\vee : VI, 1,1.
\rho = \frac{1}{2} \sum_{\alpha > 0} \alpha : VI, 1,10; VI, 3,3.
S : IV, 1,1.
S(e^p) = \sum_{g \in W.p} e^g : VI, 3,4.
S_w : IV, 1,8.
T = B \cap N : IV, 2,1.
V : VI, 1,1; VI, 4,4.
W = N/T : IV, 2,1.
W : V, 3,1.
w_0 : VI, 1,6.
W(R) : VI, 1,1.
W^+(R) : VI, 4, exercices.
W_X : IV, 1,8.
\Phi_R : VI, 1,12.
(\overline{\omega}_1, \ldots, \overline{\omega}_l) : VI, 1,10.

Les chiffres de référence indiquent successivement le chapitre, le paragraphe et le numéro (ou, exceptionnellement, l’exercice).

Affine (groupe de Weyl) : VI, 2,1.
Alcôve : VI, 2,1.
Angle de deux racines : VI, 1,2.
Anti-invariant : V, 5,4 et VI, 3,3.
Appartement : IV, 1, exerc. 15.
Arbre : IV, Annexe, 3.
Arête : IV, Annexe, 1.
Associée (forme bilinéaire — à un système de Coxeter) : V, 4,1.
Base d’un système de racines : VI, 1,5.
Canonique (forme bilinéaire) : VI, 1,12.
Canonique (matrice de Cartan) : VI, 1,5.
Caractéristiques (degrés) : V, 5,1.
Cartan (matrice de) : VI, 1,5.
Chaîne : IV, Annexe, 3.
Chaîne de racines : VI, 1,3.
Chambre : V, 1,3 et V, 3,1.
Chambre d’un immeuble : IV, 1, exerc. 15.
Chambre d’un système de racines : VI, 1,5.
Chemin : IV, Annexe, 2.
Circuit : IV, Annexe, 3.
Classes (doubles) : IV, 2,1.
Clos (ensemble — de racines) : VI, 1,7.
Composantes connexes d’un graphe : IV, Annexe, 2.
Composantes irréductibles d’un système de Coxeter : IV, 1,9.
Conjugués (éléments — d’un groupe) : IV, 1,3.
Connexe (graphe) : IV, Annexe, 2.
Connexion (indice de) : VI, 1,9.

Contragrédiente (représentation) : V, 4,4.
Coxeter (graphe de) : IV, 1,9.
Coxeter (groupe de) : IV, 1,3.
Coxeter (matrice de) : IV, 1,9.
Coxeter (nombre de) : V, 6,1 et VI, 1,11.
Coxeter (système de) : IV, 1,3.
Coxeter (transformation de) : V, 6,1, et VI, 1,11.
Cristallographique (groupe) : VI, 2,5.
Demi-espace : V, 1,1.
Diédral (groupe) : IV, 1,2.
Dominant (poids) : VI, 1,10.
Dynkin (graphe de) : VI, 4,2.
Échange (condition d’—) : IV, 1,5.
Essentiel (groupe — engendré par des réflexions) : V, 3,7.
Exposants d’un groupe de Coxeter fini : V, 6,2.
Face d’une chambre : V, 1,4.
Facette : V, 1,2.
Fondamental (poids) : VI, 1,10.
Forêt : IV, Annexe, 3.
Fortement orthogonales (racines) : VI, 1,3.
Galerie : IV, 1, exerc. 15.
Grande (plus — racine) : VI, 1,8.
Graphe : IV, Annexe, 1.
Graphe de Coxeter : IV, 1, 9.
Graphe de Dynkin : VI, 4, 2.
Graphe de Dynkin complété : VI, 4, 3.
Hecke (algèbre de) : V, 2, exerc. 22.
Hyperbolique (groupe de Coxeter de type) : V, 4, exerc. 12.
Hyperbolique compact (groupe de Coxeter de type) : V, 4, exerc. 12.
Hyperplan d’une pseudo-réflexion : V, 2,1.
Immeuble : IV, 1, exerc. 15.
Indivisible (racine) : VI, 1,3.
Inverse (système de racines) : VI, 1,1.
Irréductible (groupe — engendré par des réflexions) : V, 3,7.
Irréductible (système de Coxeter) : IV, 1,9.
Irréductible (système de racines) : VI, 1,2.
Liés (éléments — d’un graphe) : IV, Annexe, 1.
Longueur d’un chemin dans un graphe : IV, Annexe, 2.
Longueur d’un élément d’un groupe : IV, 1,1.
Longueur d’une racine : VI, 1,2.
Minuscule (poids) : VI, 1, exerc. 24.
Mitoyennes (chambres) : IV, 1, exerc. 15.
Mur d’une chambre : V, 1,4.

Normalisateur : IV, 2,6.
Normé (graphe) : VI, 4,2.
Opposées (facettes) : IV, 1, exerc. 18.
Ordre d'une arête : VI, 4,1.
Orthogonale (réflexion) : V, 2,3.
Parabolique (sous-groupe) : IV, 2,6.
Plein (sous-graphe) : IV, Annexe, 1.
Pliage d'un appartement : IV, 1, exerc. 18.
Poids : VI, 1,9.
Poincaré (série de ) : V, 5,1.
Polynômes (algèbre graduée de) : V, 5,1.
Positive (racine) : VI, 1,6.
Présentation d'un groupe : IV, 1,3.
Pseudo-réflexion : V, 2,1.
Racines (système de) : VI, 1,1.
Radiciels (poids) : VI, 1,9.
Ramification (point de — d'un graphe) : IV, Annexe, 1.
Rang (d'un système de racines) : VI, 1,1.
Réduit (système de racines) : VI, 1,4.
Réduite (décomposition) : IV, 1,1.
Réflexion : V, 2,2.
Représentation associée à une matrice de Coxeter : V, 4,3.
Restreint (produit direct) : IV, 1,9.
Saturé (ensemble de poids) : VI, 1, exerc. 23.
Signature d'un élément d'un groupe de Coxeter : IV, 1,3.
Simplement transitive (action — d'un groupe) : IV, 2, exerc. 3.
Simplexe : V, 1,6.
Simplicial (cône) : V, 1,6.
Sommet d'un graphe : IV, Annexe, 1.
Sous-graphe : IV, Annexe, 1.
Spacieux (immeuble) : IV, 1, exerc. 24.
Spécial (point) : V, 3,10.
Structuré (immeuble) : IV, 1, exerc. 24.
Support d'une facette : V, 1,2.
Terminal (sommet — d'un graphe) : IV, Annexe, 1.
Tits (sous-groupe de) : IV, 2, exerc. 3.
Tits (système de) : IV, 2,1.
Tits (théorème de) : V, 4,4.
Vecteur d'une pseudo-réflexion : V, 2,1.
Weyl (groupe de — d'un système de racines) : VI, 1,1.
Weyl (groupe de — d'un système de Tits) : IV, 2,1.

PLANCHE I

SYSTÈMES DE TYPE $\mathrm{A}_l$ ($l \geqslant 1$)

(I) V est l'hyperplan de $\mathrm{E} = \mathbf{R}^{l+1}$ formé des points dont la somme des coordonnées est nulle.
Racines : $\varepsilon_i - \varepsilon_j$ ($i \neq j$, $1 \leqslant i \leqslant l+1$, $1 \leqslant j \leqslant l+1$).
Nombre de racines : $n = l(l+1)$.

(II) Base : $\alpha_1 = \varepsilon_1 - \varepsilon_2$, $\alpha_2 = \varepsilon_2 - \varepsilon_3$, $\ldots$, $\alpha_l = \varepsilon_l - \varepsilon_{l+1}$.
Racines positives : $\varepsilon_i - \varepsilon_j = \sum_{i \leqslant k < j} \alpha_k$ ($1 \leqslant i < j \leqslant l+1$).

(III) Nombre de Coxeter : $h = l + 1$.

(IV) Plus grande racine : $\tilde{\alpha} = \varepsilon_1 - \varepsilon_{l+1} = \alpha_1 + \alpha_2 + \cdots + \alpha_l = \varpi_1 + \varpi_l$.
Graphe de Dynkin complété ($l \geqslant 2$) : la chaîne $\alpha_1, \alpha_2, \ldots, \alpha_{l-1}, \alpha_l$, chaque sommet joint au suivant par une arête simple, et un sommet de plus au dessus de la chaîne, joint à $\alpha_1$ et à $\alpha_l$, ce qui ferme le cycle.

Pour $l = 1$, le graphe de Coxeter du groupe de Weyl affine est : deux sommets joints par une arête portant $\infty$.

(V) $\mathrm{R}^\vee = \mathrm{R}$,

$$
\Phi_{\mathrm{R}}(x, y) = \frac{(x|y)}{2(l+1)} \qquad \gamma(\mathrm{R}) = (l+1)^2 .
$$

(VI) Poids fondamentaux :

$$
\begin{aligned}
\varpi_i &= (\varepsilon_1 + \cdots + \varepsilon_i) - \frac{i}{l+1} \sum_{j=1}^{l+1} \varepsilon_j \\
&= \frac{1}{l+1} \big[ (l-i+1)\alpha_1 + 2(l-i+1)\alpha_2 + \cdots + (i-1)(l-i+1)\alpha_{i-1} \\
&\qquad\qquad + i(l-i+1)\alpha_i + i(l-i)\alpha_{i+1} + \cdots + i\alpha_l \big] .
\end{aligned}
$$

(VII) Somme des racines positives:

$$
2\rho = l\varepsilon_1 + (l-2)\varepsilon_2 + (l-4)\varepsilon_3 + \cdots - (l-2)\varepsilon_l - l\varepsilon_{l+1}
= l\alpha_1 + 2(l-1)\alpha_2 + \cdots + i(l-i+1)\alpha_i + \cdots + l\alpha_l.
$$

(VIII) $Q(R)$: ensemble des vecteurs à coordonnées entières de somme nulle.
$P(R)$: engendré par $Q(R)$ et $\varepsilon_1 - (l+1)^{-1}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l+1})$.
$P(R)/Q(R)$ isomorphe à $\mathbf{Z}/(l+1)\mathbf{Z}$.
Indice de connexion: $l+1$.

(IX) Exposants: 1, 2, ..., l.

(X) $W(R) = \mathfrak{S}_{l+1}$, identifié au groupe des permutations des $\varepsilon_i$. Ordre de $W(R)$: $(l+1)!$.

(XI) $l = 1$: $A(R) = W(R); w_0 = -1$.
$l \geqslant 2$: $A(R) = W(R) \times \{1, -1\}$ et $w_0$ transforme $\alpha_i$ en $-\alpha_{l+1-i}$.

(XII) Le groupe $P(R^\vee)/Q(R^\vee)$ est cyclique d'ordre $(l+1)$; il opère sur le graphe de Dynkin complété par permutations circulaires. Si $l \geqslant 2$, l'unique élément non neutre de $A(R)/W(R)$ opère sur $P(R)/Q(R)$ par l'automorphisme $x \mapsto -x$.

(XIII) Matrice de Cartan ($l \times l$):

$$
\begin{pmatrix}
2 & -1 & 0 & 0 & \ldots & 0 & 0 \\
-1 & 2 & -1 & 0 & \ldots & 0 & 0 \\
0 & -1 & 2 & -1 & \ldots & 0 & 0 \\
0 & 0 & -1 & 2 & \ldots & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & 0 & \ldots & -1 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE B_l $(l \geq 2)$

(I) $V = E = \mathbf{R}^l$.
Racines : $\pm \varepsilon_i \ (1 \leq i \leq l), \ \pm \varepsilon_i \pm \varepsilon_j \ (1 \leq i < j \leq l)$.
Nombre de racines : $n = 2l^2$.

(II) Base : $\alpha_1 = \varepsilon_1 - \varepsilon_2, \ \alpha_2 = \varepsilon_2 - \varepsilon_3, \ \ldots, \ \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \ \alpha_l = \varepsilon_l$.

Racines positives
$$
\begin{cases}
\varepsilon_i = \sum_{i \leq k \leq l} \alpha_k & (1 \leq i \leq l), \\
\varepsilon_i - \varepsilon_j = \sum_{i \leq k < j} \alpha_k & (1 \leq i < j \leq l), \\
\varepsilon_i + \varepsilon_j = \sum_{i \leq k < j} \alpha_k + 2 \sum_{j \leq k \leq l} \alpha_k & (1 \leq i < j \leq l).
\end{cases}
$$

(III) Nombre de Coxeter : $h = 2l$.

(IV) Plus grande racine :
$$
\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + 2\alpha_3 + \cdots + 2\alpha_l.
$$
On a $\tilde{\alpha} = 2\omega_2$ si $l = 2$, $\tilde{\alpha} = \omega_2$ si $l \geq 3$.
Graphe de Dynkin complété :
pour $l = 2$
$$
\begin{array}{c}
\circ \xrightarrow{\alpha_2} \circ \xleftarrow{\alpha_1} \circ
\end{array}
$$
pour $l \geq 3$
$$
\begin{array}{c}
\circ \xrightarrow{\alpha_1} \circ \xrightarrow{\alpha_2} \circ \xrightarrow{\alpha_3} \cdots \xrightarrow{\alpha_{l-1}} \circ \xleftarrow{\alpha_l}
\end{array}
$$

(V) $R^\vee$ est l'ensemble des vecteurs
$$
\pm 2\varepsilon_i \ (1 \leq i \leq l), \ \pm \varepsilon_i \pm \varepsilon_j \ (1 \leq i < j \leq l).
$$
$$
\Phi_R(x, y) = \frac{(x|y)}{4l-2} \quad \gamma(R) = (l+1)(4l-2)
$$

(VI) Poids fondamentaux:

$$
\begin{align*}
\overline{\omega}_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \quad (1 \leq i < l) \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_l) \\
\overline{\omega}_l &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l) \\
&= \frac{1}{2} (\alpha_1 + 2\alpha_2 + \cdots + l\alpha_l).
\end{align*}
$$

(VII) Somme des racines positives:

$$
\begin{align*}
2\rho &= (2l-1)\varepsilon_1 + (2l-3)\varepsilon_2 + \cdots + 3\varepsilon_{l-1} + \varepsilon_l \\
&= (2l-1)\alpha_1 + 2(2l-2)\alpha_2 + \cdots + i(2l-i)\alpha_i + \cdots + l^2\alpha_l.
\end{align*}
$$

(VIII) $Q(R) = \bigoplus_{i=1}^l \mathbf{Z}\varepsilon_i, \quad P(R) = \bigoplus_{i=1}^l \mathbf{Z}\varepsilon_i + \mathbf{Z} \left( \frac{1}{2} \sum_{i=1}^l \varepsilon_i \right).$

$P(R)/Q(R)$ isomorphe à $\mathbf{Z}/2\mathbf{Z}$, engendré par l'image de $\overline{\omega}_l$.

Indice de connexion : 2.

(IX) Exposants : 1, 3, 5, ..., $2l-1$.

(X) $W(R)$ est produit semi-direct du groupe $\mathfrak{S}_l$, opérant par permutation sur les $\varepsilon_i$, et du groupe $(\mathbf{Z}/2\mathbf{Z})^l$, opérant par $\varepsilon_i \mapsto (\pm 1)_i \varepsilon_i$. Son ordre est $2^l.l!$.

(XI) $A(R) = W(R), \ w_0 = -1$.

(XII) L'unique élément non trivial de $P(R^\vee)/Q(R^\vee)$ définit l'unique automorphisme non trivial du graphe de Dynkin complété.

(XIII) Matrice de Cartan $(l \times l)$:

$$
\begin{pmatrix}
2 & -1 & 0 & 0 & \ldots & 0 & 0 \\
-1 & 2 & -1 & 0 & \ldots & 0 & 0 \\
0 & -1 & 2 & -1 & \ldots & 0 & 0 \\
0 & 0 & -1 & 2 & \ldots & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & 0 & \ldots & 2 & -2 \\
0 & 0 & 0 & 0 & \ldots & -1 & 2
\end{pmatrix}
$$

SYSTÈMES DE TYPE $C_l$ ($l \geq 2$)

(I) $V = E = \mathbf{R}^l$.
Racines : $\pm 2\varepsilon_i \quad (1 \leq i \leq l), \quad \pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq l)$.
Nombre de racines : $n = 2l^2$.

(II) Base : $\alpha_1 = \varepsilon_1 - \varepsilon_2, \alpha_2 = \varepsilon_2 - \varepsilon_3, \ldots, \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \alpha_l = 2\varepsilon_l$.
Racines positives
$$
\begin{cases}
\varepsilon_i - \varepsilon_j = \sum_{i \leq k < j} \alpha_k & (1 \leq i < j \leq l), \\
\varepsilon_i + \varepsilon_j = \sum_{i \leq k < j} \alpha_k + 2 \sum_{j \leq k < l} \alpha_k + \alpha_l & (1 \leq i < j \leq l), \\
2\varepsilon_l = 2 \sum_{i \leq k < l} \alpha_k + \alpha_l & (1 \leq i \leq l).
\end{cases}
$$

(III) Nombre de Coxeter : $h = 2l$.

(IV) Plus grande racine : $\tilde{\alpha} = 2\varepsilon_1 = 2\alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-1} + \alpha_l$.
Graphe de Dynkin complété :

$$
\begin{array}{ccccccccc}
\circ & \longrightarrow & \circ & \cdots & \circ & \longrightarrow & \circ & \longrightarrow & \circ \\
& & & & & & & & \\
\alpha_1 & \alpha_2 & & & \alpha_{l-2} & \alpha_{l-1} & \alpha_l &
\end{array}
$$

(V) $R^\vee$ est l’ensemble des vecteurs $\pm \varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j$.

$$
\Phi_R(x, y) = \frac{(x|y)}{4(l+1)} \qquad \gamma(R) = (l+1)(4l-2).
$$

(VI) Poids fondamentaux :
$$
\overline{\omega}_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \quad (1 \leq i \leq l)
$$
$$
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-1} + \frac{1}{2}\alpha_l).
$$

(VII) Somme des racines positives:

$$
2\rho = 2l \varepsilon_1 + (2l - 2)\varepsilon_2 + \cdots + 4\varepsilon_{l-1} + 2\varepsilon_l \\
= 2l \alpha_1 + 2(2l - 1)\alpha_2 + \cdots + i(2l - i + 1)\alpha_i + \cdots \\
+ (l - 1)(l + 2)\alpha_{l-1} + \frac{1}{2}l(l + 1)\alpha_l.
$$

(VIII) $Q(R)$: ensemble des points à coordonnées entières de somme paire.

$$
P(R) = \bigoplus_{i=1}^{l} \mathbf{Z}\varepsilon_i.
$$
$P(R)/Q(R)$ isomorphe à $\mathbf{Z}/2\mathbf{Z}$, engendré par l’image de $\overline{\omega}_1$.
Indice de connexion : 2.

(IX) Exposants : 1, 3, 5, ..., $2l - 1$.

(X) $W(R)$ est produit semi-direct du groupe $\mathfrak{S}_l$, opérant par permutations des $\varepsilon_i$, et du groupe $(\mathbf{Z}/2\mathbf{Z})^l$, opérant par $\varepsilon_i \mapsto (\pm 1)_i \varepsilon_i$. Son ordre est $2^l . l!$.

(XI) $A(R) = W(R); w_0 = -1$.

(XII) L’unique élément non trivial de $P(R^\vee)/Q(R^\vee)$ définit l’unique automorphisme non trivial du graphe de Dynkin complété.

(XIII) Matrice de Cartan ($l \times l$):

$$
\begin{pmatrix}
2 & -1 & 0 & 0 & \ldots & 0 & 0 \\
-1 & 2 & -1 & 0 & \ldots & 0 & 0 \\
0 & -1 & 2 & -1 & \ldots & 0 & 0 \\
0 & 0 & -1 & 2 & \ldots & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & 0 & 0 & \ldots & 2 & -1 \\
0 & 0 & 0 & 0 & \ldots & -2 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE D_l (l \geq 3)

(I) V = E = \mathbf{R}^l.
Racines: $\pm \varepsilon_i \pm \varepsilon_j$ ($1 \leq i < j \leq l$; $(\varepsilon_i)$ base canonique de $\mathbf{R}^l$).
Nombre de racines: $n = 2l(l-1)$.

(II) Base:
$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3,\ \ldots,\ \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l,\ \alpha_l = \varepsilon_{l-1} + \varepsilon_l.
$$
Racines positives
$$
\begin{cases}
\varepsilon_i - \varepsilon_j = \sum_{i<k<j} \alpha_k & (1 \leq i < j \leq l), \\
\varepsilon_i + \varepsilon_l = \sum_{i \leq k \leq l} \alpha_l & (1 \leq i < l), \\
\varepsilon_i + \varepsilon_j = \sum_{i \leq k < j} \alpha_k + 2 \sum_{j \leq k < l-1} \alpha_k + \alpha_{l-1} + \alpha_l & (1 \leq i < j < l).
\end{cases}
$$

(III) Nombre de Coxeter: $h = 2l - 2$.

(IV) Plus grande racine:
$$
\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l.
$$
On a $\tilde{\alpha} = \overline{\omega}_2 + \overline{\omega}_3$ si $l = 3$ et $\tilde{\alpha} = \overline{\omega}_2$ si $l \geq 4$.
Graphe de Dynkin complété ($l \geq 4$):

![Graphe de Dynkin completé](../images/dynkin_d_l.png)

(V) $R^\vee = R$.
$$
\Phi_R(x, y) = \frac{(x|y)}{4(l-1)}, \quad \gamma(R) = 4(l-1)^2.
$$

(VI) Poids fondamentaux:
$$
\overline{\omega}_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \quad (1 \leq i \leq l-2)
$$
$$
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2}) + \frac{1}{2}i(\alpha_{l-1} + \alpha_l)
$$

$$
\overline{\omega}_{l-1} = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} - \varepsilon_l)
$$
$$
= \frac{1}{2} (\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2} l\alpha_{l-1} + \frac{1}{2} (l-2)\alpha_l)
$$
$$
\overline{\omega}_l = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} + \varepsilon_l)
$$
$$
= \frac{1}{2} (\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2} (l-2)\alpha_{l-1} + \frac{1}{2} l\alpha_l).
$$

(VII) Somme des racines positives:

$$
2\rho = 2(l-1)\varepsilon_1 + 2(l-2)\varepsilon_2 + \cdots + 2\varepsilon_{l-1}
$$
$$
= 2(l-1)\alpha_1 + 2(2l-3)\alpha_2 + \cdots
$$
$$
+ 2(il - \frac{i(i+1)}{2})\alpha_i + \cdots + \frac{l(l-1)}{2}(\alpha_{l-1} + \alpha_l).
$$

(VIII) Q(R): ensemble des points à coordonnées entières de somme paire.

$$
P(R) = \bigoplus_{i=1}^l \mathbf{Z}\varepsilon_i + \mathbf{Z} \left( \frac{1}{2} \sum_{i=1}^l \varepsilon_i \right)
$$

l impair: P(R)/Q(R) est isomorphe à \mathbf{Z}/4\mathbf{Z}, engendré par l'image de \overline{\omega}_l; on a \overline{\omega}_1 \equiv 2\overline{\omega}_l et \overline{\omega}_{l-1} \equiv 3\overline{\omega}_l \mod Q(R).
l pair: P(R)/Q(R) est isomorphe à (\mathbf{Z}/2\mathbf{Z}) \times (\mathbf{Z}/2\mathbf{Z}); les trois éléments d'ordre deux sont les images de \overline{\omega}_1, \overline{\omega}_{l-1} et \overline{\omega}_l.
Indice de connexion: 4.

(IX) Exposants: 1, 3, 5, ..., 2l-5, 2l-3, l-1 (ce dernier apparaissant deux fois si l pair, une fois si l impair).

(X) W(R) est produit semi-direct du groupe \mathfrak{S}_l, opérant par permutations des \varepsilon_i, et du groupe (\mathbf{Z}/2\mathbf{Z})^{l-1}, opérant par \varepsilon_i \mapsto (\pm 1)_i \varepsilon_i avec \prod_i (\pm 1)_i = 1. Son ordre est $2^{l-1}l!$.

(XI) $l \neq 4$: A(R)/W(R) = \mathbf{Z}/2\mathbf{Z} opérant sur le graphe de Dynkin par transposition des sommets \alpha_{l-1} et \alpha_l.
$l = 4$: A(R)/W(R) = \mathfrak{S}_3, opérant sur le graphe de Dynkin par permutations des sommets \alpha_1, \alpha_3 et \alpha_4.
$w_0 = -1$ si l est pair; $w_0 = -\varepsilon$ si l est impair, où \varepsilon est l'automorphisme qui permutte \alpha_{l-1} et \alpha_l et laisse fixes les autres \alpha_i.

(XII) Action de P(R^\vee)/Q(R^\vee) = P(R)/Q(R) sur le graphe de Dynkin complété:
l impair: \omega_l transforme \alpha_0 en \alpha_l, \alpha_l en \alpha_1, \alpha_1 en \alpha_{l-1} et \alpha_{l-1} en \alpha_0; il échange \alpha_j et \alpha_{l-j} pour $2 \leq j \leq l-2$.
l pair: \omega_l (resp. \omega_{l-1}) échange \alpha_0 et \alpha_l (resp. \alpha_0 et \alpha_{l-1}), \alpha_1 et \alpha_{l-1} (resp. \alpha_1 et \alpha_l) et échange \alpha_j et \alpha_{l-j} pour $2 \leq j \leq l-2$.

(XIII) Matrice de Cartan $(l \times l)$:

$$
\begin{pmatrix}
2 & -1 & \ldots & 0 & 0 & 0 & 0 \\
-1 & 2 & \ldots & 0 & 0 & 0 & 0 \\
\ldots & \ldots & \ldots & \ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & 2 & -1 & 0 & 0 \\
0 & 0 & \ldots & -1 & 2 & -1 & -1 \\
0 & 0 & \ldots & 0 & -1 & 2 & 0 \\
0 & 0 & \ldots & 0 & -1 & 0 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE E₆

(I) V est le sous-espace de $E = \mathbf{R}^8$ formé des points dont les coordonnées $(\xi_i)$ sont telles que $\xi_6 = \xi_7 = -\xi_8$.
Racines : $\pm \varepsilon_i \pm \varepsilon_j \ (1 \leq i < j \leq 5)$,
$$
\pm \frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec } \sum_{i=1}^5 \nu(i) \text{ pair.}
$$
Nombre de racines : $n = 72$.

(II) Base : $\alpha_1 = \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7)$, $\alpha_2 = \varepsilon_1 + \varepsilon_2$,
$\alpha_3 = \varepsilon_2 - \varepsilon_1$, $\alpha_4 = \varepsilon_3 - \varepsilon_2$, $\alpha_5 = \varepsilon_4 - \varepsilon_3$, $\alpha_6 = \varepsilon_5 - \varepsilon_4$.
Racines positives : $\pm \varepsilon_i + \varepsilon_j \ (1 \leq i < j \leq 5)$,
$$
\frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec } \sum_{i=1}^5 \nu(i) \text{ pair.}
$$
Racines positives ayant un coefficient $\geq 2$ (*) (on note $acdef$ la racine $a\alpha_1 + b\alpha_2 + c\alpha_3 + d\alpha_4 + e\alpha_5 + f\alpha_6$) :
$$
\begin{array}{cccccccc}
01210, & 11210, & 01211, & 12210, & 11211, & 01221, & 12211, \\
1 & 1 & 1 & 1 & 1 & 1 & 1 \\
11221, & 12221, & 12321, & 12321. \\
1 & 1 & 1 & 2
\end{array}
$$

(III) Nombre de Coxeter : $h = 12$.

(IV) Plus grande racine :
$$
\tilde{\alpha} = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8)
$$
$$
= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6 = \overline{\omega}_2.
$$

(*) Les autres racines positives s’obtiennent en appliquant le cor. 3 de la prop. 19 du Chap. VI, § 1, n° 6.

Graphe de Dynkin complété:

(V)   R = R^∨.

$$
\Phi_R(x, y) = \frac{(x|y)}{24}, \quad \gamma(R) = 144.
$$

(VI) Poids fondamentaux:

$$
\begin{align*}
\overline{\omega}_1 &= \frac{2}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) \\
&= \frac{1}{3} (4\alpha_1 + 3\alpha_2 + 5\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6) \\
\overline{\omega}_2 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8) \\
&= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6 \\
\overline{\omega}_3 &= \frac{5}{6} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \frac{1}{2} (-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5) \\
&= \frac{1}{3} (5\alpha_1 + 6\alpha_2 + 10\alpha_3 + 12\alpha_4 + 8\alpha_5 + 4\alpha_6) \\
\overline{\omega}_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6 \\
\overline{\omega}_5 &= \frac{2}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_4 + \varepsilon_5 \\
&= \frac{1}{3} (4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 5\alpha_6) \\
\overline{\omega}_6 &= \frac{1}{3} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_5 \\
&= \frac{1}{3} (2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6).
\end{align*}
$$

(VII) Somme des racines positives:

$$
\begin{align*}
2\rho &= 2(\varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 4(\varepsilon_8 - \varepsilon_7 - \varepsilon_6)) \\
&= 2(8\alpha_1 + 11\alpha_2 + 15\alpha_3 + 21\alpha_4 + 15\alpha_5 + 8\alpha_6).
\end{align*}
$$

(VIII) P(R)/Q(R) isomorphe à $\mathbf{Z}/3\mathbf{Z}$.
Indice de connexion : 3.

(IX) Exposants : 1, 4, 5, 7, 8, 11.

(X) Ordre de W(R) : $2^7 \cdot 3^4 \cdot 5$.

(XI) $A(R) = W(R) \times \{1, -1\}; w_0$ transforme $\alpha_1, \alpha_2, \alpha_3, \alpha_4, \alpha_5, \alpha_6$
respectivement en $-\alpha_6, -\alpha_2, -\alpha_5, -\alpha_4, -\alpha_3, -\alpha_1.$

(XII) L’élément non neutre de $A(R)/W(R)$ définit l’automorphisme $x \mapsto -x$ de $P(R)/Q(R)$.
Le groupe des automorphismes du schéma de Dynkin complété est isomorphe à $\mathfrak{S}_3$; ses éléments d’ordre 3 sont induits par les deux éléments non triviaux de $P(R^\vee)/Q(R^\vee)$.

(XIII) Matrice de Cartan:

$$
\begin{pmatrix}
2 & 0 & -1 & 0 & 0 & 0 \\
0 & 2 & 0 & -1 & 0 & 0 \\
-1 & 0 & 2 & -1 & 0 & 0 \\
0 & -1 & -1 & 2 & -1 & 0 \\
0 & 0 & 0 & -1 & 2 & -1 \\
0 & 0 & 0 & 0 & -1 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE E_7

(I) V est l’hyperplan de $E = \mathbf{R}^8$ orthogonal à $\varepsilon_7 + \varepsilon_8$.
Racines : $\pm \varepsilon_i \pm \varepsilon_j \ (1 \leq i < j \leq 6), \ \pm (\varepsilon_7 - \varepsilon_8),$
$$
\pm \frac{1}{2} (\varepsilon_7 - \varepsilon_8 + \sum_{i=1}^6 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec} \quad \sum_{i=1}^6 \nu(i) \text{ impair.}
$$
Nombre de racines : $n = 126$.

(II) Base :
$$
\alpha_1 = \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7),
$$
$$
\alpha_2 = \varepsilon_1 + \varepsilon_2, \ \alpha_3 = \varepsilon_2 - \varepsilon_1, \ \alpha_4 = \varepsilon_3 - \varepsilon_2, \ \alpha_5 = \varepsilon_4 - \varepsilon_3,
$$
$$
\alpha_6 = \varepsilon_5 - \varepsilon_4, \ \alpha_7 = \varepsilon_6 - \varepsilon_5.
$$

Racines positives :

$$
\pm \varepsilon_i + \varepsilon_j \ (1 \leq i < j \leq 6), \quad \varepsilon_8 - \varepsilon_7,
$$
$$
\frac{1}{2} (\varepsilon_8 - \varepsilon_7 + \sum_{i=1}^6 (-1)^{\nu(i)} \varepsilon_i) \quad \text{avec} \quad \sum_{i=1}^6 \nu(i) \text{ impair.}
$$

Racines positives contenant $\alpha_7$ et ayant un coefficient $\geq 2$ (*) (on note $a c d e f g$ la racine $a \alpha_1 + b \alpha_2 + c \alpha_3 + d \alpha_4 + e \alpha_5 + f \alpha_6 + g \alpha_7$):

<table>
  <tr>
    <th>012111</th><th>112111</th><th>012211</th><th>122111</th><th>112211</th><th>012221</th>
  </tr>
  <tr>
    <td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td>
  </tr>
  <tr>
    <th>122211</th><th>112221</th><th>122221</th><th>123211</th><th>123221</th><th>123211</th>
  </tr>
  <tr>
    <td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>2</td>
  </tr>
  <tr>
    <th>123321</th><th>123221</th><th>123321</th><th>124321</th><th>134321</th><th>234321</th>
  </tr>
  <tr>
    <td>1</td><td>2</td><td>2</td><td>2</td><td>2</td><td>2</td>
  </tr>
</table>

(III) Nombre de Coxeter : $h = 18$.

(*) Les racines positives ne contenant pas $\alpha_7$ proviennent de $E_6$. Les racines positives dont tous les coefficients sont $\leq 1$ s’obtiennent en appliquant le cor. 3 de la prop. 19 du Chap. VI, § 1, no 6.

(IV) Plus grande racine:
$$
\tilde{\alpha} = \varepsilon_8 - \varepsilon_7 = 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7 = \overline{\omega}_1.
$$
Graphe de Dynkin complété:

$$
\begin{array}{ccccccccc}
\circ & \circ & \circ & \circ & \circ & \circ & \circ \\
\alpha_1 & \alpha_3 & \alpha_4 & \alpha_5 & \alpha_6 & \alpha_7 \\
\alpha_2
\end{array}
$$

(V) $R^\vee = R$.

$$
\Phi_R(x, y) = \frac{(x|y)}{36}, \quad \gamma(R) = 324.
$$

(VI) Poids fondamentaux:

$$
\begin{align*}
\overline{\omega}_1 &= \varepsilon_8 - \varepsilon_7 \\
&= 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7 \\
\overline{\omega}_2 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 2\varepsilon_7 + 2\varepsilon_8) \\
&= \frac{1}{2} (4\alpha_1 + 7\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 6\alpha_6 + 3\alpha_7) \\
\overline{\omega}_3 &= \frac{1}{2} (-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 3\varepsilon_7 + 3\varepsilon_8) \\
&= 3\alpha_1 + 4\alpha_2 + 6\alpha_3 + 8\alpha_4 + 6\alpha_5 + 4\alpha_6 + 2\alpha_7 \\
\overline{\omega}_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + 2(\varepsilon_8 - \varepsilon_7) \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 6\alpha_6 + 3\alpha_7 \\
\overline{\omega}_5 &= \frac{1}{2} (2\varepsilon_4 + 2\varepsilon_5 + 2\varepsilon_6 + 3(\varepsilon_8 - \varepsilon_7)) \\
&= \frac{1}{2} (6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 10\alpha_6 + 5\alpha_7) \\
\overline{\omega}_6 &= \varepsilon_5 + \varepsilon_6 - \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 2\alpha_7 \\
\overline{\omega}_7 &= \varepsilon_6 + \frac{1}{2} (\varepsilon_8 - \varepsilon_7) \\
&= \frac{1}{2} (2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7).
\end{align*}
$$

(VII) Somme des racines positives:

$$
\begin{align*}
2\rho &= 2\varepsilon_2 + 4\varepsilon_3 + 6\varepsilon_4 + 8\varepsilon_5 + 10\varepsilon_6 - 17\varepsilon_7 + 17\varepsilon_8 \\
&= 34\alpha_1 + 49\alpha_2 + 66\alpha_3 + 96\alpha_4 + 75\alpha_5 + 52\alpha_6 + 27\alpha_7.
\end{align*}
$$

(VIII) $P(R)/Q(R)$ isomorphe à $\mathbf{Z}/2\mathbf{Z}$.
Indice de connexion : 2.

(IX) Exposants : 1, 5, 7, 9, 11, 13, 17.

(X) Ordre de $W(R) : 2^{10} \cdot 3^4 \cdot 5 \cdot 7.$

(XI) $A(R) = W(R),\ w_0 = -1.$
(XII) $P(R^\vee)/Q(R^\vee)$ a un seul élément non neutre; celui-ci définit l’unique automorphisme non trivial du graphe de Dynkin complété.
(XIII) Matrice de Cartan:

$$
\begin{pmatrix}
2 & 0 & -1 & 0 & 0 & 0 & 0 \\
0 & 2 & 0 & -1 & 0 & 0 & 0 \\
-1 & 0 & 2 & -1 & 0 & 0 & 0 \\
0 & -1 & -1 & 2 & -1 & 0 & 0 \\
0 & 0 & 0 & -1 & 2 & -1 & 0 \\
0 & 0 & 0 & 0 & -1 & 2 & -1 \\
0 & 0 & 0 & 0 & 0 & -1 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE E₈

(I) $V = E = \mathbf{R}^8$.
Racines : $\pm \varepsilon_i \pm \varepsilon_j \quad (i < j)$, $\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i$ avec $\sum_{i=1}^8 \nu(i)$ pair.
Nombre de racines : $n = 240$.

(II) Base :
$$
\alpha_1 = \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7),
$$
$$
\alpha_2 = \varepsilon_1 + \varepsilon_2, \quad \alpha_3 = \varepsilon_2 - \varepsilon_1, \quad \alpha_4 = \varepsilon_3 - \varepsilon_2, \quad \alpha_5 = \varepsilon_4 - \varepsilon_3,
$$
$$
\alpha_6 = \varepsilon_5 - \varepsilon_4, \quad \alpha_7 = \varepsilon_6 - \varepsilon_5, \quad \alpha_8 = \varepsilon_7 - \varepsilon_6.
$$

Racines positives :
$\pm \varepsilon_i + \varepsilon_j \quad (i < j)$, $\frac{1}{2} (\varepsilon_8 + \sum_{i=1}^7 (-1)^{\nu(i)} \varepsilon_i)$ avec $\sum_{i=1}^7 \nu(i)$ pair.

Racines positives contenant $\alpha_8$ et ayant un coefficient $\geq 2$ (*) (on note $a c d e f g h$ la racine $a \alpha_1 + b \alpha_2 + c \alpha_3 + d \alpha_4 + e \alpha_5 + f \alpha_6 + g \alpha_7 + h \alpha_8$):

<table>
  <tr>
    <th>0121111</th><th>0122111</th><th>1121111</th><th>0122211</th><th>1221111</th><th>1122111</th>
  </tr>
  <tr>
    <td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td>
  </tr>
  <tr>
    <th>1222111</th><th>1122211</th><th>0122221</th><th>1232111</th><th>1222211</th><th>1122221</th>
  </tr>
  <tr>
    <td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td>
  </tr>
  <tr>
    <th>1232111</th><th>1232211</th><th>1222221</th><th>1232211</th><th>1233211</th><th>1232221</th>
  </tr>
  <tr>
    <td>2</td><td>1</td><td>1</td><td>2</td><td>1</td><td>1</td>
  </tr>
  <tr>
    <th>1233211</th><th>1232221</th><th>1233221</th><th>1243211</th><th>1233221</th><th>1233321</th>
  </tr>
  <tr>
    <td>2</td><td>2</td><td>1</td><td>2</td><td>2</td><td>1</td>
  </tr>
  <tr>
    <th>1343211</th><th>1243221</th><th>1233321</th><th>2343211</th><th>1343221</th><th>1243321</th>
  </tr>
  <tr>
    <td>2</td><td>2</td><td>2</td><td>2</td><td>2</td><td>2</td>
  </tr>
  <tr>
    <th>2343221</th><th>1343321</th><th>1244321</th><th>2343321</th><th>1344321</th><th>1354321</th>
  </tr>
  <tr>
    <td>2</td><td>2</td><td>2</td><td>2</td><td>2</td><td>2</td>
  </tr>
  <tr>
    <th>2344321</th><th>1354321</th><th>2354321</th><th>2354321</th><th>2454321</th><th>2454321</th>
  </tr>
  <tr>
    <td>2</td><td>3</td><td>2</td><td>3</td><td>2</td><td>3</td>
  </tr>
  <tr>
    <th>2464321</th><th>2465321</th><th>2465421</th><th>2465431</th><th>2465432</th><th></th>
  </tr>
  <tr>
    <td>3</td><td>3</td><td>3</td><td>3</td><td>3</td><td></td>
  </tr>
</table>

(*) Les racines positives ne contenant pas $\alpha_8$ proviennent de $E_7$. Les racines positives dont tous les coefficients sont $\leq 1$ s’obtiennent en appliquant le cor. 3 de la prop. 19 du Chap. VI, § 1, no 6.

(III) Nombre de Coxeter : $h = 30$.

(IV) Plus grande racine :

$$
\tilde{\alpha} = \varepsilon_7 + \varepsilon_8 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8 = \overline{\omega}_8.
$$

Graphe de Dynkin complété :

![Graphe de Dynkin completé](https://i.imgur.com/3Q5z5QG.png)

(V) $R^\vee = R$.

$$
\Phi_R(x, y) = \frac{(x|y)}{60}, \quad \gamma(R) = 900.
$$

(VI) Poids fondamentaux :

$$
\begin{align*}
\overline{\omega}_1 &= 2\varepsilon_8 \\
&= 4\alpha_1 + 5\alpha_2 + 7\alpha_3 + 10\alpha_4 + 8\alpha_5 + 6\alpha_6 + 4\alpha_7 + 2\alpha_8 \\
\overline{\omega}_2 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8) \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\overline{\omega}_3 &= \frac{1}{2} (-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 7\varepsilon_8) \\
&= 7\alpha_1 + 10\alpha_2 + 14\alpha_3 + 20\alpha_4 + 16\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\overline{\omega}_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8 \\
&= 10\alpha_1 + 15\alpha_2 + 20\alpha_3 + 30\alpha_4 + 24\alpha_5 + 18\alpha_6 + 12\alpha_7 + 6\alpha_8 \\
\overline{\omega}_5 &= \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 4\varepsilon_8 \\
&= 8\alpha_1 + 12\alpha_2 + 16\alpha_3 + 24\alpha_4 + 20\alpha_5 + 15\alpha_6 + 10\alpha_7 + 5\alpha_8 \\
\overline{\omega}_6 &= \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 3\varepsilon_8 \\
&= 6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\overline{\omega}_7 &= \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8 \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 8\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\overline{\omega}_8 &= \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8.
\end{align*}
$$

(VII) Somme des racines positives :

$$
\begin{align*}
2\rho &= 2(\varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 5\varepsilon_6 + 6\varepsilon_7 + 23\varepsilon_8) \\
&= 2(46\alpha_1 + 68\alpha_2 + 91\alpha_3 + 135\alpha_4 + 110\alpha_5 + 84\alpha_6 + 57\alpha_7 + 29\alpha_8).
\end{align*}
$$

(VIII) $Q(R)$ : ensemble des points de coordonnées $\xi_i$ telles que $2\xi_i \in \mathbf{Z}$,

$$
\xi_i - \xi_j \in \mathbf{Z}, \quad \sum_{i=1}^8 \xi_i \in 2\mathbf{Z}.
$$

$P(R) = Q(R)$.

Indice de connexion : 1.

(IX) Exposants : 1, 7, 11, 13, 17, 19, 23, 29.
(X) Ordre de W(R) : $2^{14} \cdot 3^5 \cdot 5^2 \cdot 7$.
(XI) et (XII) : $A(R) = W(R)$, $w_0 = -1$.
(XIII) Matrice de Cartan :

$$
\begin{pmatrix}
2 & 0 & -1 & 0 & 0 & 0 & 0 & 0 \\
0 & 2 & 0 & -1 & 0 & 0 & 0 & 0 \\
-1 & 0 & 2 & -1 & 0 & 0 & 0 & 0 \\
0 & -1 & -1 & 2 & -1 & 0 & 0 & 0 \\
0 & 0 & 0 & -1 & 2 & -1 & 0 & 0 \\
0 & 0 & 0 & 0 & -1 & 2 & -1 & 0 \\
0 & 0 & 0 & 0 & 0 & -1 & 2 & -1 \\
0 & 0 & 0 & 0 & 0 & 0 & -1 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE F₄

(I) $V = E = \mathbf{R}^4$.
Racines:
$$
\pm \varepsilon_i \quad (1 \leq i \leq 4), \qquad \pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 4),
$$
$$
\frac{1}{2} (\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
Nombre de racines : $n = 48$.

(II) Base :
$$
\alpha_1 = \varepsilon_2 - \varepsilon_3, \quad \alpha_2 = \varepsilon_3 - \varepsilon_4, \quad \alpha_3 = \varepsilon_4, \quad \alpha_4 = \frac{1}{2} (\varepsilon_1 - \varepsilon_2 - \varepsilon_3 - \varepsilon_4).
$$
Racines positives : $\varepsilon_i \quad (1 \leq i \leq 4), \quad \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 4),$
$$
\frac{1}{2} (\varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
Racines positives ayant un coefficient $\geq 2$ (*) (on note $a \ b \ c \ d$ la racine $a \alpha_1 + b \alpha_2 + c \alpha_3 + d \alpha_4$) :
$$
\begin{array}{cccccccc}
0120 & 1120 & 0121 & 1220 & 1121 & 0122 & 1221 & 1122 \\
1231 & 1222 & 1232 & 1242 & 1342 & 2342
\end{array}
$$

(III) Nombre de Coxeter : $h = 12$.

(IV) Plus grande racine : $\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = 2 \alpha_1 + 3 \alpha_2 + 4 \alpha_3 + 2 \alpha_4 = \omega_1$.
Graphe de Dynkin complété :

$$
\begin{array}{c}
\circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\alpha_1 \quad \alpha_2 \quad \alpha_3 \quad \alpha_4
\end{array}
$$

(*) Les autres racines positives s’obtiennent en appliquant le cor. 3 de la prop. 19 du Chap. VI, § 1, no 6.

(V)   R$^\vee$ est l'ensemble des vecteurs $\pm 2\varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j, \pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4$.

$$
\Phi_R(x, y) = \frac{(x|y)}{18}, \quad \gamma(R) = 162.
$$

(VI)   Poids fondamentaux:

$$
\begin{align*}
\overline{\omega}_1 &= \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4 \\
\overline{\omega}_2 &= 2\varepsilon_1 + \varepsilon_2 + \varepsilon_3 = 3\alpha_1 + 6\alpha_2 + 8\alpha_3 + 4\alpha_4 \\
\overline{\omega}_3 &= \frac{1}{2}(3\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4) = 2\alpha_1 + 4\alpha_2 + 6\alpha_3 + 3\alpha_4 \\
\overline{\omega}_4 &= \varepsilon_1 = \alpha_1 + 2\alpha_2 + 3\alpha_3 + 2\alpha_4.
\end{align*}
$$

(VII)   Somme des racines positives:

$$
2\rho = 11\varepsilon_1 + 5\varepsilon_2 + 3\varepsilon_3 + \varepsilon_4 = 16\alpha_1 + 30\alpha_2 + 42\alpha_3 + 22\alpha_4.
$$

(VIII)   Q(R) = $\bigoplus_{i=1}^4 \mathbf{Z}\varepsilon_i + \mathbf{Z}(\frac{1}{2} \sum_{i=1}^4 \varepsilon_i )$.
P(R) = Q(R).
Indice de connexion: 1.

(IX)   Exposants: 1, 5, 7, 11.

(X)   W(R) produit semi-direct de $\mathfrak{S}_3$ par un groupe lui-même produit semi-direct de $\mathfrak{S}_4$ par $(\mathbf{Z}/2\mathbf{Z})^3$.
Ordre de W(R): $2^7 \cdot 3^2$.

(XI) et (XII): A(R) = W(R), $w_0 = -1$.

(XIII) Matrice de Cartan:

$$
\begin{pmatrix}
2 & -1 & 0 & 0 \\
-1 & 2 & -2 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2
\end{pmatrix}
$$

SYSTÈME DE TYPE G₂

(I) V est l’hyperplan de $E = \mathbf{R}^3$ d’équation $\xi_1 + \xi_2 + \xi_3 = 0$.
Racines : $\pm (\varepsilon_1 - \varepsilon_2), \pm (\varepsilon_1 - \varepsilon_3), \pm (\varepsilon_2 - \varepsilon_3),$
$\pm (2\varepsilon_1 - \varepsilon_2 - \varepsilon_3), \quad \pm (2\varepsilon_2 - \varepsilon_1 - \varepsilon_3), \quad \pm (2\varepsilon_3 - \varepsilon_1 - \varepsilon_2).$
Nombre de racines : 12.

(II) Base : $\alpha_1 = \varepsilon_1 - \varepsilon_2, \alpha_2 = -2\varepsilon_1 + \varepsilon_2 + \varepsilon_3.$
Racines positives : $\alpha_1, \alpha_2, \alpha_1 + \alpha_2, 2\alpha_1 + \alpha_2, 3\alpha_1 + \alpha_2, 3\alpha_1 + 2\alpha_2.$

(III) Nombre de Coxeter : $h = 6.$

(IV) Plus grande racine : $\tilde{\alpha} = -\varepsilon_1 - \varepsilon_2 + 2\varepsilon_3 = 3\alpha_1 + 2\alpha_2 = \overline{\omega}_2.$
Graphe de Dynkin complété :

$$
\begin{array}{c}
\alpha_1 \leftrightarrow \alpha_2 \\
\end{array}
$$

(V) $R^\vee$ est l’ensemble des vecteurs $\pm \alpha_1, \pm (\alpha_1 + \alpha_2), \pm (2\alpha_1 + \alpha_2),$
$\pm \frac{1}{3} \alpha_2, \pm \frac{1}{3} (3\alpha_1 + \alpha_2), \pm \frac{1}{3} (3\alpha_1 + 2\alpha_2).$

$$
\Phi_R(x, y) = \frac{(x|y)}{24}, \quad \gamma(R) = 48.
$$

(VI) Poids fondamentaux :

$$
\overline{\omega}_1 = 2\alpha_1 + \alpha_2, \quad \overline{\omega}_2 = 3\alpha_1 + 2\alpha_2.
$$

(VII) Somme des racines positives :

$$
2\rho = 2(5\alpha_1 + 3\alpha_2).
$$

(VIII) $P(R) = Q(R)$.
Indice de connexion : 1.

(IX) Exposants : 1, 5.
(X) $W(R)$ : groupe diédral d'ordre 12.
(XI) et (XII) : $A(R) = W(R)$, $w_0 = -1$.
(XIII) Matrice de Cartan:

$$
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

SYSTÈMES IRRÉDUCTIBLES DE RANG 2

A₂    G₂
B₂    BC₂

Les trois premières figures ci-dessus représentent les systèmes de racines R de type A₂, B₂ et G₂. La région hachurée représente la chambre C correspondant à la base ($\alpha_1, \alpha_2$). On a tracé en tirets la droite $(x|\beta) = 1$, où $\beta$ désigne la plus grande racine du système inverse $R^\vee$ et la région hachurée deux fois représente l’alcôve de $R^\vee$ de sommet 0 contenue dans C.

La dernière figure représente l’unique système de racines irréductible non réduit de rang 2.

(Nous nous limitons dans ce résumé au cas du corps des nombres réels et aux systèmes de racines réduits.)

1) Soit V un espace vectoriel réel. On appelle système de racines réduit dans V un sous-ensemble R de V qui possède les propriétés suivantes :
   (i) R est fini, et engendre V.
   (ii) Pour tout $\alpha \in R$, il existe $\alpha^\vee \in V^*$ tel que $\langle \alpha, \alpha^\vee \rangle = 2$, et que l’application
   $$
   s_\alpha : x \mapsto x - \langle x, \alpha^\vee \rangle \alpha
   $$
   de V dans V transforme R en R.
   (iii) Pour tout $\alpha \in R$, on a $\alpha^\vee(R) \subset \mathbf{Z}$.
   (iv) Si $\alpha \in R$, on a $2\alpha \notin R$.

   Compte tenu de (i), l’élément $\alpha^\vee$ dont l’existence est affirmée par (ii) est unique; ceci donne un sens à (iii). L’application $s_\alpha$ est une réflexion laissant fixes les points de $L_\alpha = \mathrm{Ker}(\alpha^\vee)$ et transformant $\alpha$ en $-\alpha$.

   Les éléments de R s’appellent les racines. La dimension de V s’appelle le rang du système de racines.

2) Le groupe des automorphismes de V qui laissent stable R se note $A(R)$. Les $s_\alpha (\alpha \in R)$ engendrent un sous-groupe $W(R)$ de $A(R)$, appelé groupe de Weyl de R ; ce sous-groupe est distingué dans $A(R)$. Les seules réflexions appartenant à $W(R)$ sont les $s_\alpha$.

3) L’ensemble $R^\vee$ des $\alpha^\vee$ (pour $\alpha \in R$) est un système de racines réduit dans $V^*$, appelé système inverse de R. L’application $\alpha \mapsto \alpha^\vee$ est une bijection, dite canonique, de R sur $R^\vee$. On a $(R^\vee)^\vee = R$, et les bijections canoniques $R \to R^\vee, R^\vee \to R$ sont réciproques l’une de l’autre. L’application $u \mapsto t_u^{-1}$ définit un isomorphisme de $W(R)$ sur $W(R^\vee)$ par lequel on identifie ces deux groupes.

4) Soit V un espace vectoriel réel somme directe de sous-espaces vectoriels $V_1, \ldots, V_r$. Pour tout i, soit $R_i$ un système de racines réduit dans $V_i$. Alors la réunion R des $R_i$ est un système de racines dans V, appelé somme directe des $R_i$. Le groupe $W(R)$ s’identifie au produit des $W(R_i)$. On dit que R est irréductible si $R \neq \varnothing$ et si $R$ n’est pas somme directe de deux systèmes de racines non vides. Il revient au même de dire que $W(R)$ est irréductible. Tout système de racines réduit $R$ est somme directe de systèmes de racines irréductibles réduits bien déterminés à une permutation près, et appelés les composants irréductibles de $R$.

5) Soit $R$ un système de racines réduit dans $V$. Il existe des produits scalaires dans $V$ invariants par $W(R)$. Dans toute la suite, on note $(x|y)$ un tel produit scalaire. Si on identifie $V$ à $V^*$ à l’aide de $(x|y)$, on a $\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)}$. La réflexion $s_\alpha$ est la réflexion orthogonale qui transforme $\alpha$ en $-\alpha$. Le groupe de Weyl est transitif dans l’ensemble des racines de même longueur. Si $R$ est irréductible, le produit scalaire $(x|y)$ est unique à la multiplication près par une constante.

6) Soit $R$ un système de racines réduit. Pour $\alpha, \beta \in R$, on pose
$$
\langle \alpha, \beta^\vee \rangle = n(\alpha, \beta) \in \mathbf{Z}.
$$
On a
$$
s_\beta(\alpha) = \alpha - n(\alpha, \beta)\beta.
$$
$$
n(\alpha, \beta) = \frac{2(\alpha|\beta)}{(\beta|\beta)}.
$$
Les seules possibilités sont les suivantes, à l’échange près de $\alpha$ et $\beta$:

$$
\begin{array}{ll}
n(\alpha, \beta) = n(\beta, \alpha) = 0; & (\widehat{\alpha, \beta}) = \frac{\pi}{2}; \quad s_\alpha s_\beta \text{ d’ordre } 2 \\
n(\alpha, \beta) = n(\beta, \alpha) = 1; & (\widehat{\alpha, \beta}) = \frac{\pi}{3}; \quad \| \alpha \| = \| \beta \|; \quad s_\alpha s_\beta \text{ d’ordre } 3 \\
n(\alpha, \beta) = n(\beta, \alpha) = -1; & (\widehat{\alpha, \beta}) = \frac{2\pi}{3}; \quad \| \alpha \| = \| \beta \|; \quad s_\alpha s_\beta \text{ d’ordre } 3 \\
n(\alpha, \beta) = 1, \quad n(\beta, \alpha) = 2; & (\widehat{\alpha, \beta}) = \frac{\pi}{4}; \quad \| \beta \| = \sqrt{2} \| \alpha \|; \quad s_\alpha s_\beta \text{ d’ordre } 4 \\
n(\alpha, \beta) = -1, \ n(\beta, \alpha) = -2; & (\widehat{\alpha, \beta}) = \frac{3\pi}{4}; \quad \| \beta \| = \sqrt{2} \| \alpha \|; \quad s_\alpha s_\beta \text{ d’ordre } 4 \\
n(\alpha, \beta) = 1, \quad n(\beta, \alpha) = 3; & (\widehat{\alpha, \beta}) = \frac{\pi}{6}; \quad \| \beta \| = \sqrt{3} \| \alpha \|; \quad s_\alpha s_\beta \text{ d’ordre } 6 \\
n(\alpha, \beta) = -1, \ n(\beta, \alpha) = -3; & (\widehat{\alpha, \beta}) = \frac{5\pi}{6}; \quad \| \beta \| = \sqrt{3} \| \alpha \|; \quad s_\alpha s_\beta \text{ d’ordre } 6 \\
n(\alpha, \beta) = n(\beta, \alpha) = 2; & \alpha = \beta \\
n(\alpha, \beta) = n(\beta, \alpha) = -2; & \alpha = -\beta.
\end{array}
$$

7) Soient $\alpha, \beta \in R$. Si $(\alpha|\beta) > 0$, $\alpha - \beta$ est une racine sauf si $\alpha = \beta$. Si $(\alpha|\beta) < 0$, $\alpha + \beta$ est une racine sauf si $\alpha = -\beta$.

8) Soient $\alpha, \beta$ deux racines non proportionnelles. L’ensemble I des $j \in \mathbf{Z}$ tels que $\beta + j\alpha \in \mathbf{R}$ est un intervalle $(-q, p)$ de $\mathbf{Z}$ contenant 0. On a
$$
p - q = -n(\beta, \alpha), \quad \frac{q+1}{p} = \frac{(\beta + \alpha|\beta + \alpha)}{(\beta|\beta)}.
$$
Soit S l’ensemble des $\beta + j\alpha$ pour $j \in I$. Alors $s_\alpha(S) = S$ et $s_\alpha(\beta + p\alpha) = \beta - q\alpha$. On dit que S est la $\alpha$-chaîne de racines définie par $\beta$, que $\beta - q\alpha$ est l’origine de la chaîne et $\beta + p\alpha$ son extrémité, et que $p + q$ est sa longueur.
Si T est une $\alpha$-chaîne d’origine $\gamma$, la longueur de T est $-n(\gamma, \alpha)$.

9) Soit X la réunion des Ker $\alpha^\vee$ ($\alpha \in \mathbf{R}$). Les composantes connexes de $V - X$ s’appellent les chambres de R dans V. Ce sont des cônes simpliciaux ouverts. Le groupe de Weyl opère de façon simplement transitive dans l’ensemble des chambres. Si C est une chambre, $\overline{C}$ est un domaine fondamental pour $W(R)$. On a $(x|y) > 0$ pour $x, y \in C$. La bijection de V sur $V^*$ correspondant à $(x|y)$ définit une bijection de l’ensemble des chambres de R dans V sur l’ensemble des chambres de $R^\vee$ dans $V^*$; on note $C^\vee$ la chambre image de C par cette bijection.

10) Soit C une chambre de R. Soient $L_1, L_2, \ldots, L_l$ les murs de C. Pour tout i, il existe une racine $\alpha_i$ et une seule telle que $L_i = L_{\alpha_i}$, et telle que $\alpha_i$ soit du même côté que C de $H_i$. La famille $(\alpha_1, \ldots, \alpha_l)$ est une base de V, et C est l’ensemble des $x \in V$ tels que $\langle \alpha_i^\vee, x \rangle > 0$ pour tout i, c’est-à-dire tels que $(\alpha_i|x) > 0$ pour tout i. On dit que $\{\alpha_1, \ldots, \alpha_l\}$ est la base B(C) de R définie par C. On a $(\alpha_i|\alpha_j) \leq 0$ lorsque $i \neq j$. Le groupe $W(R)$ opère de façon simplement transitive sur l’ensemble des bases. Toute racine est transformée par un élément de $W(R)$ d’un élément de B(C). On a $\{\alpha_1^\vee, \ldots, \alpha_l^\vee\} = B(C^\vee)$.

11) Posons $s_{\alpha_i} = s_i$, soit S l’ensemble des $s_i$, et soit $m_{ij}$ l’ordre de $s_i s_j$. Le couple $(W(R), S)$ est un système de Coxeter de matrice $(m_{ij})$; autrement dit, $W(R)$ est défini par la famille génératrice $(s_i)_{1 \leq i \leq l}$ et par les relations $(s_i s_j)^{m_{ij}} = 1$. Pour que $s_i$ et $s_j$ soient conjugués dans $W(R)$, il faut et il suffit qu’il existe une suite d’indices $(i_1, i_2, \ldots, i_q)$ tels que $i_1 = i, i_q = j$ et que chacun des $m_{i_t i_{t+1}}$ soit égal à 3.

12) Soit $n_{ij} = n(\alpha_i, \alpha_j)$. La matrice $(n_{ij})_{1 \leq i, j \leq l}$ s’appelle la matrice de Cartan de R. Elle est indépendante (à une permutation près de 1, 2, ..., l) du choix de C. On a $n_{ii} = 2, n_{ij} \in \{0, -1, -2, -3\}$ pour $i \neq j$. Si deux systèmes de racines ont même matrice de Cartan, ils sont isomorphes.

13) Soit G le sous-groupe de $A(R)$ qui laisse stable $B(C)$. Alors $A(R)$ est produit semi-direct de G et de $W(R)$.

14) On appelle relation d’ordre définie par C dans V (resp. $V^*$) la relation d’ordre, compatible avec la structure d’espace vectoriel de V (resp. $V^*$), pour laquelle les éléments $\geq 0$ sont les combinaisons linéaires des $\alpha_i$ (resp. $\alpha_i^\vee$) à coefficients $\geqslant 0$. Ces éléments sont dits positifs pour $C$, ou pour $B(C)$. Ces relations d’ordre sont aussi définies par $C^\vee$. Un élément de $V$ est $\geqslant 0$ si et seulement si ses valeurs sur $C^\vee$ sont $\geqslant 0$. L’ensemble des éléments $\geqslant 0$ pour $C$ contient $\overline{C}$ mais est en général distinct de $\overline{C}$. Soit $x \in V$. Pour que $x \in \overline{C}$, il faut et il suffit que $x \geqslant w(x)$ pour tout $w \in W(R)$. Pour que $x \in C$, il faut et il suffit que $x > w(x)$ pour tout $w \in W(R)$ distinct de 1.

15) Toute racine est soit positive, soit négative pour $C$. On note $R_+(C)$ l’ensemble des racines positives pour $C$, de sorte que $R = R_+(C) \cup (-R_+(C))$ est une partition de $R$. La réflexion $s_i$ transforme $\alpha_i$ en $-\alpha_i$ et permutent entre eux les éléments de $R_+(C)$ distincts de $\alpha_i$.

16) Soit $B$ une base de $R$. Toute racine positive (resp. négative) pour $B$ est combinaison linéaire des éléments de $B$ à coefficients entiers $\geqslant 0$ (resp. $\leqslant 0$).

17) Soit $(\beta_1, \beta_2, \ldots, \beta_n)$ une suite de racines positives pour $C$ telles que $\beta_1 + \beta_2 + \cdots + \beta_n$ soit une racine. Il existe une permutation $\pi \in S_n$ telle que, pour tout $i \in \{1, 2, \ldots, n\}$, $\beta_{\pi(1)} + \beta_{\pi(2)} + \cdots + \beta_{\pi(i)}$ soit une racine.

18) Soit $\alpha \in R_+(C)$. Pour que $\alpha \in B(C)$, il faut et il suffit que $\alpha$ ne puisse pas s’écrire comme somme de deux racines positives.

19) Soient $C$ une chambre, $(\alpha_1, \alpha_2, \ldots, \alpha_l)$ la base correspondante. Pour toute partie $J$ de $I = \{1, 2, \ldots, l\}$, soit $W_J$ le sous-groupe de $W(R)$ engendré par les $s_i$ tels que $i \in J$. Soit $C_J$ l’ensemble des combinaisons linéaires à coefficients $> 0$ des $\alpha_j$ pour $j \notin J$, de sorte que $C_J$ est une facette de $C$.
Soient $J \subset I$, $g \in W(R)$. Les conditions suivantes sont équivalentes :
a) $g$ laisse invariant un point de $C_J$;
b) $g$ laisse invariant tout point de $C_J$;
c) $g$ laisse invariant tout point de $\overline{C}_J$;
d) $g(C_J) = C_J$;
e) $g(\overline{C}_J) = \overline{C}_J$;
f) $g \in W_J$.

Soient $J, J' \subset \{1, 2, \ldots, l\}$ et $g, g' \in W(R)$. Les conditions suivantes sont équivalentes :
a) $g(C_J) = g'(C_{J'})$;
b) $g(C_J) \cap g'(C_{J'}) \neq \emptyset$;
c) $gW_J = g'W_{J'}$;
d) $J = J'$ et $g' \in gW_J$.

Soient $J_1, J_2, \ldots, J_r \subset I$ et $J = J_1 \cap \cdots \cap J_r$. Alors $W_J = W_{J_1} \cap \cdots \cap W_{J_r}$.
Pour tout $g \in W(R)$, il existe $J \subset I$ tel que $\overline{C} \cap g(\overline{C}) = \overline{C}_J$ et que $g \in W_J$.

20) Soit $P$ un sous-ensemble de $R$. On dit que $P$ est clos si les conditions $\alpha \in P, \beta \in P, \alpha + \beta \in R$ impliquent $\alpha + \beta \in P$. On dit que $P$ est parabolique si $P$ est clos et si $P \cup (-P) = R$. Les conditions suivantes sont équivalentes :
    a) $P$ est parabolique;
    b) $P$ est clos et il existe une chambre $C$ telle que $P \supset R_+(C)$;
    c) il existe une chambre $C$ et une partie $\Sigma$ de $B(C)$ telle que $P$ soit la réunion de $R_+(C)$ et de l’ensemble $Q$ des racines combinaisons linéaires à coefficients entiers $\leq 0$ des éléments de $\Sigma$.

Supposons ces conditions vérifiées, et soit $V_1$ le sous-espace vectoriel de $V$ engendré par $\Sigma$. On a
$$
P \cap (-P) = Q \cup (-Q) = V_1 \cap R,
$$
et $P \cap (-P)$ est un système de racines dans $V_1$ de base $\Sigma$.

Soient $P', C', \Sigma'$ avec des propriétés analogues. S’il existe un élément de $W(R)$ transformant $P$ en $P'$, il existe un élément de $W(R)$ transformant $C$ en $C'$, $\Sigma$ en $\Sigma'$ et $P$ en $P'$.

21) Soit $P$ un sous-ensemble de $R$. Les conditions suivantes sont équivalentes :
    a) il existe une chambre $C$ telle que $P = R_+(C)$;
    b) $P$ est clos, et $\{P, -P\}$ est une partition de $R$.
La chambre $C$ est alors unique.

Supposons $V$ muni d’une structure d’espace vectoriel ordonné telle que toute racine soit positive ou négative. Soit $R_+$ l’ensemble des racines positives pour cette structure. Il existe une chambre $C$ et une seule telle que $R_+ = R_+(C)$.

22) Pour qu’une partie $B$ de $R$ soit une base de $R$, il faut et il suffit que les éléments de $B$ soient linéairement indépendants, et que toute racine soit combinaison linéaire d’éléments de $B$ à coefficients tous $\geq 0$ ou tous $\leq 0$.

23) Soit $P$ un sous-ensemble clos de $R$ tel que $P \cap (-P) = \varnothing$. Il existe une chambre $C$ telle que $P \subset R_+(C)$.

24) Un sous-ensemble $P$ de $R$ est dit symétrique si $P = -P$. Soient $P$ un sous-ensemble de $R$, et $V_1$ (resp. $\Gamma$) le sous-espace vectoriel (resp. le sous-groupe additif) de $V$ engendré par $P$. Les conditions suivantes sont équivalentes :
    a) $P$ est clos et symétrique;
    b) $P$ est clos et $P$ est un système de racines dans $V_1$;
    c) $\Gamma \cap R = P$.

25) On suppose $R$ irréductible. Soit $C$ une chambre; posons
$$
B(C) = \{\alpha_1, \ldots, \alpha_l\}.
$$
Il existe un plus grand élément dans $R$ (pour l’ordre défini par $C$), c’est-à-dire un élément $\tilde{\alpha} = n_1 \alpha_1 + \cdots + n_l \alpha_l$ de $R$ tel que, pour toute racine
$$
p_1 \alpha_1 + \cdots + p_l \alpha_l,
$$
on ait $n_1 \geq p_1, \ldots, n_l \geq p_l$. On a $\tilde{\alpha} \in \overline{C}$, et $\| \tilde{\alpha} \| \geq \| \alpha \|$ pour toute racine $\alpha$.

26) On note $Q(R)$ le sous-groupe de $V$ engendré par $R$; les éléments de $Q(R)$ s’appellent les poids radiciels de $R$. Le groupe $Q(R)$ est un sous-groupe discret de $V$ de rang $l = \dim V$. Toute base de $R$ est une base de $Q(R)$.

On note $P(R)$ le sous-groupe de $V$ associé à $Q(R^\vee)$; les éléments de $P(R)$ s’appellent les poids de $R$. Le groupe $P(R)$ est un sous-groupe discret de $V$ de rang $l$ contenant $Q(R)$. Les groupes $P(R)/Q(R)$, $P(R^\vee)/Q(R^\vee)$ sont finis et isomorphes; leur ordre $f$ s’appelle l’indice de connexion de $R$. Avec les notations de 25), l’ordre de $W(R)$ est $l! n_1 n_2 \ldots n_l f$.

Le groupe $A(R)$ laisse stables $P(R)$, $Q(R)$, donc opère dans $P(R)/Q(R)$. Le groupe $W(R)$ opère trivialement dans $P(R)/Q(R)$, donc $A(R)/W(R)$ opère dans $P(R)/Q(R)$.

27) Soit $C$ une chambre. Soit $B = (\alpha_1, \ldots, \alpha_l)$ la base de $R$ correspondante. La base duale $(\overline{\omega}_1, \ldots, \overline{\omega}_l)$ de $(\alpha_1^\vee, \ldots, \alpha_l^\vee)$ est une base de $P(R)$. Les $\overline{\omega}_i$ s’appellent les poids fondamentaux (pour $C$, ou pour $B$). L’ensemble des combinaisons linéaires des $\overline{\omega}_i$ à coefficients $> 0$ (resp. $\geqslant 0$) est $C$ (resp. $\overline{C}$). Les combinaisons linéaires des $\overline{\omega}_i$ à coefficients entiers $\geqslant 0$ s’appellent les poids dominants. Tout élément de $P(R)$ est transformé par $W(R)$ d’un poids dominant et d’un seul. Les poids dominants sont les éléments $\overline{\omega}$ de $V$ tels que $\frac{2(\overline{\omega}|\alpha_i)}{(\alpha_i|\alpha_i)}$ soit un entier $\geqslant 0$ pour tout $i$.

28) Soit $\rho = \frac{1}{2} \sum_{\alpha \in R_+(C)} \alpha$. On a $\rho = \overline{\omega}_1 + \cdots + \overline{\omega}_l \in C$.

29) Soit $T$ le groupe des translations de $V^*$ dont les vecteurs appartiennent à $Q(R^\vee)$. Le groupe de transformations affines de $V^*$ engendré par $T$ et $W(R)$ est produit semi-direct de $W(R)$ et de $T$. Ce groupe s’appelle le groupe de Weyl affine de $R$ et se note $W_a(R)$. Il opère proprement dans $V^*$. Pour $\alpha \in R$ et $\lambda \in \mathbf{Z}$, soit $s_{\alpha, \lambda}$ l’application $x^* \mapsto x^* - \langle x^*, \alpha \rangle \alpha^\vee + \lambda \alpha^\vee$; c’est une réflexion affine, et l’ensemble $L_{\alpha, \lambda}$ de ses points invariants est défini par l’équation $\langle x^*, \alpha \rangle = -\lambda$; on a $L_{\alpha, \lambda} = L_\alpha - \frac{1}{2} \lambda \alpha^\vee$. Les $s_{\alpha, \lambda}$ sont les réflexions affines appartenant à $W_a(R)$, et engendrent le groupe $W_a(R)$.

30) Soit $E$ la réunion des $L_{\alpha, \lambda}$ pour $\alpha \in R$ et $\lambda \in \mathbf{Z}$. Les composantes connexes de $V^* - E$ s’appellent les alcôves de $R$. Si $R$ est irréductible, chaque alcôve est un simplexe ouvert; en général, une alcôve est un produit de simplex ouverts. Le groupe $W_a(R)$ opère de façon simplement transitive sur l’ensemble des alcôves. Si $C$ est une alcôve, $\overline{C}$ est un domaine fondamental pour $W_a(R)$. Soient $\sigma_1, \sigma_2, \ldots, \sigma_q$ les réflexions de $W_a(R)$ correspondant aux murs de $C$; soit $\mu_{ij}$ l’ordre de $\sigma_i \sigma_j$. Alors $W_a(R)$ est défini par les générateurs $\sigma_i$ et les relations $(\sigma_i \sigma_j)^{\mu_{ij}} = 1$.

31) Si $p \in P(R^\vee)$, il existe une alcôve $C$ telle que $p$ soit point extrémal de $\overline{C}$. Si $C'$ est une alcôve, $\overline{C}'$ admet un poids radiciel et un seul pour point extrémal.

Soit $x^* \in V^*$; les conditions suivantes sont équivalentes :
a) $x^* \in P(R^\vee)$;
b) pour tout $\alpha \in R$, l’hyperplan parallèle à $L_\alpha$ et passant par $x^*$ est un $L_{\alpha,\lambda}$.

Soit $C'$ une chambre de $R^\vee$. Il existe une alcôve $C$ et une seule contenue dans $C'$ et telle que $0 \in \overline{C}$. Supposons $R$ irréductible, et soit $\beta$ la plus grande racine de $R$ (pour $C'$); alors $C$ est l’ensemble des $x^* \in C'$ tels que $\langle x^*, \beta \rangle < 1$.

32) Soient $S$ l’algèbre symétrique de $V$, $S^W$ la sous-algèbre formée des éléments invariants par $W = W(R)$, $g$ l’ordre de $W$, $l = \dim V$. Il existe des éléments $I_1, I_2, \ldots, I_l$ de $S^W$, homogènes, algébriquement indépendants, qui engendrent $S^W$. Le $S^W$-module $S$ admet une base formée de $g$ éléments homogènes. Soit $a$ l’idéal de $S$ engendré par les éléments homogènes de $S^W$ de degré $> 0$; la représentation de $W$ dans $S/a$ déduite par passage au quotient de la représentation de $W$ dans $S$ est isomorphe à la représentation régulière de $W$ (sur $\mathbf{R}$).

33) Soient $I_1, I_2, \ldots, I_l$ des éléments de $S^W$, homogènes, algébriquement indépendants, engendrant $S^W$. Leurs degrés $k_1, k_2, \ldots, k_l$ sont déterminés de manière unique (à l’ordre près) par $R$. On a $g = k_1 k_2 \ldots k_l$. Le nombre de racines est $2 \sum_{i=1}^l (k_i - 1)$.

34) Un élément $A$ de $S$ est dit anti-invariant par $W$ si $w(A) = \det(w) . A$ pour tout $w \in W$. Soit $R = R_1 \cup (-R_1)$ une partition de $R$, et posons $\pi = \prod_{\alpha \in R_1} \alpha$. L’élément $\pi$ de $S$ est anti-invariant; les éléments anti-invariants de $S$ sont les éléments de la forme $\pi I$, avec $I \in S^W$.

35) Soit $E$ l’algèbre $\mathbf{Z}[P]$ du groupe des poids $P$ de $R$. Si $p \in P$, on note $e^p$ l’élément correspondant de $E$. On a $e^p e^{p'} = e^{p+p'}$ et les $e^p$ forment une base de $E$. Le groupe $W$ opère dans $E$ de telle sorte que $w(e^p) = e^{w(p)}$ si $w \in W$ et $p \in P$. Un élément $z \in E$ est dit anti-invariant si $w(z) = \det(w) . z$ pour tout $w \in W$. Pour tout $z \in E$, posons $J(z) = \sum_{w \in W} \det(w) . w(z)$. Soit $C$ une chambre. Les éléments $J(e^p)$, où $p \in P \cap C$, forment une base du groupe des éléments anti-invariants de $E$. Si $\rho$ est la demi-somme des racines positives, on a :

$$
J(e^p) = e^{\rho} \prod_{\alpha > 0} (1 - e^{-\alpha}) = \prod_{\alpha > 0} (e^{\alpha/2} - e^{-\alpha/2}),
$$

les produits étant pris sur l’ensemble des racines $> 0$.

36) Avec les notations de 35), posons

$$
z_p = J(e^{p+\rho}) / J(e^{\rho}) \quad \text{pour } p \in P.
$$

Les $z_p$, pour $p \in P \cap \overline{C}$, forment une base du groupe $E^W$ des éléments de $E$ invariants par $W$. Si $\omega_1, \ldots, \omega_l$ sont les poids fondamentaux de $R$, les éléments $z_{\omega_i}, \ 1 \leq i \leq l$, sont algébriquement indépendants et engendrent l’anneau $E^W$.

37) Soient $C$ une chambre de $R$, $(\alpha_1, \ldots, \alpha_l)$ la base correspondante. L’élément $c = s_1 s_2 \ldots s_l$ de $W$ s’appelle une transformation de Coxeter de $R$. La classe de conjugaison de $c$ dans $W$ ne dépend ni de $C$ ni de la numérotation des $\alpha_i$. L’ordre $h$ de $c$ s’appelle le nombre de Coxeter de $R$. Les valeurs propres de $c$ sont de la forme $\exp \frac{2i \pi m_j}{h}$, où les entiers $m_1, m_2, \ldots, m_l$ (appelés exposants de $R$) sont tels que $1 \leq m_1 \leq m_2 \leq \cdots \leq m_l \leq h - 1$.
Supposons $R$ irréductible. On a alors

$$
m_1 = 1, \quad m_l = h - 1.
$$
$$
m_j + m_{l+1-j} = h \quad (1 \leq j \leq l).
$$
$$
m_1 + m_2 + \cdots + m_l = \frac{1}{2} lh = \frac{1}{2} \operatorname{Card}(R).
$$

Tout $m \in \{1, 2, \ldots, h-1\}$ étranger à $h$ est égal à l’un des $m_j$ et à un seul. Les nombres $m_1 + 1, m_2 + 1, \ldots, m_l + 1$ coïncident, à l’ordre près, avec les entiers notés $n_1, n_2, \ldots, n_l$ dans 33). Avec les notations de 25), $n_1 + \cdots + n_l = h - 1$.
Il existe $l$ orbites de $\{1, c, c^2, \ldots, c^{h-1}\}$ dans $R$, et elles ont toutes $h$ éléments.
Si $h$ est pair, $c^{h/2}$ transforme $C$ en $-C$. Pour que $-1 \in W$, il faut et il suffit que les exposants de $W$ soient tous impairs; lorsqu’il en est ainsi, $h$ est pair et $c^{h/2} = -1$.

INTRODUCTION AUX CHAPITRES IV, V ET VI ......................... 7

CHAPITRE IV. — Groupes de Coxeter et systèmes de Tits ............... 9

§ 1. Groupes de Coxeter ............................................. 9
    1. Longueur et décompositions réduites ......................... 9
    2. Groupes diédraux ............................................. 10
    3. Premières propriétés des groupes de Coxeter ............... 11
    4. Décompositions réduites dans un groupe de Coxeter ...... 13
    5. La condition d'échange ..................................... 15
    6. Caractérisation des groupes de Coxeter .................. 17
    7. Familles de partitions .................................... 18
    8. Sous-groupes des groupes de Coxeter .................... 19
    9. Matrices et graphes de Coxeter .......................... 20

§ 2. Systèmes de Tits ............................................. 22
    1. Définition et premières propriétés ....................... 22
    2. Un exemple ................................................ 24
    3. Décomposition de G en doubles classes .................. 25
    4. Relations avec les systèmes de Coxeter ................. 25
    5. Sous-groupes de G contenant B .......................... 27
    6. Sous-groupes paraboliques ............................... 29
    7. Théorème de simplicité ................................... 30

Annexe. — Graphes ............................................... 33
    1. Définitions ................................................ 33
    2. Composantes connexes d'un graphe ....................... 33
    3. Forêts et arbres .......................................... 35

Exercices du § 1 .................................................. 37
Exercices du § 2 .................................................. 46

CHAPITRE V. — Groupes engendrés par des réflexions ......................... 57
    § 1. Hyperplans, chambres et facettes ............................................. 57
        1. Notations ................................................................. 57
        2. Facettes ................................................................. 58
        3. Chambres ................................................................. 60
        4. Murs et faces ............................................................ 61
        5. Dièdres ................................................................. 63
        6. Exemples : cônes simpliciaux et simplexés ............................. 64
    § 2. Réflexions ............................................................................. 66
        1. Pseudo-réflexions ......................................................... 66
        2. Réflexions ................................................................. 67
        3. Réflexions orthogonales .................................................. 68
        4. Réflexions orthogonales dans un espace affine euclidien .. 69
        5. Compléments sur les rotations planes ............................... 70
    § 3. Groupes de déplacements engendrés par des réflexions ............ 72
        1. Résultats préliminaires ................................................ 72
        2. Relation avec les systèmes de Coxeter .............................. 74
        3. Domaine fondamental, stabilisateurs ................................. 75
        4. Matrice et graphe de Coxeter de W ................................. 76
        5. Systèmes de vecteurs à produits scalaires négatifs ............. 77
        6. Théorèmes de finitude .................................................. 79
        7. Décomposition de la représentation linéaire de W dans T. 81
        8. Décomposition de l’espace affine E en produit ................. 83
        9. Structure des chambres ................................................ 85
       10. Points spéciaux .......................................................... 87
    § 4. Représentation géométrique d’un groupe de Coxeter ............... 89
        1. Forme associée à une matrice de Coxeter ......................... 89
        2. Le plan E_{s,s'} et le groupe engendré par σ_s et σ_{s'} .......... 90
        3. Groupe et représentation associés à une matrice de Coxeter .... 91
        4. La représentation contragrédiente .................................. 92
        5. Démonstration du lemme 1 ............................................. 94
        6. Domaine fondamental de W dans la réunion des chambres. ...... 96
        7. Irréductibilité de la représentation géométrique d’un groupe de Coxeter ......................................................... 97
        8. Critères de finitude .................................................... 98
        9. Cas où B_M est positive et dégénérée ............................... 100
    § 5. Invariants dans l’algèbre symétrique ................................. 102
        1. Série de Poincaré des algèbres graduées ......................... 102
        2. Invariants d’un groupe linéaire fini : propriétés de module 105
        3. Invariants d’un groupe linéaire fini : propriétés d’anneau ................................................................. 107

4. Éléments anti-invariants ......................... 112
5. Compléments ........................................ 114

§ 6. Transformation de Coxeter.......................... 116
    1. Définition des transformations de Coxeter .......... 116
    2. Valeurs propres d'une transformation de Coxeter. Exposants............................................. 117

Annexe. — Compléments sur les représentations linéaires ............ 124

Exercices du § 2 ........................................ 127
Exercices du § 3 ........................................ 128
Exercices du § 4 ........................................ 130
Exercices du § 5 ........................................ 135
Exercices du § 6 ........................................ 139

CHAPITRE VI. — Systèmes de racines ....................... 142

§ 1. Systèmes de racines .................................. 142
    1. Définition d'un système de racines ................. 142
    2. Somme directe de systèmes de racines ............... 146
    3. Relations entre deux racines ....................... 147
    4. Systèmes de racines réduits ......................... 151
    5. Chambres et bases d'un système de racines .......... 153
    6. Racines positives ................................... 155
    7. Ensembles clos de racines ........................... 160
    8. Plus grande racine .................................. 165
    9. Poids, poids radiciels .............................. 166
   10. Poids fondamentaux, poids dominants ................. 167
   11. Transformation de Coxeter .......................... 169
   12. Forme bilinéaire canonique ......................... 171

§ 2. Groupe de Weyl affine ............................... 173
    1. Groupe de Weyl affine ............................... 173
    2. Poids et points spéciaux ............................ 174
    3. Le normalisateur de $W_a$ ....................... 175
    4. Application : ordre du groupe de Weyl .............. 177
    5. Systèmes de racines et groupes engendrés par des réflexions ............................................. 178

§ 3. Invariants exponentiels ............................. 181
    1. L'algèbre d'un groupe commutatif libre .............. 181
    2. Cas du groupe des poids : termes maximaux .......... 183
    3. Éléments anti-invariants ............................ 183
    4. Éléments invariants ................................ 186

§ 4. Classification des systèmes de racines ............................................. 188
    1. Groupes de Coxeter finis ......................................................... 188
    2. Graphes de Dynkin ................................................................. 195
    3. Groupe de Weyl affine et graphe de Dynkin complété ... 198
    4. Préliminaires à la construction des systèmes de racines .... 200
    5. Systèmes de type B_l (l \geq 2) .................................................. 202
    6. Systèmes de type C_l (l \geq 2) .................................................. 204
    7. Systèmes de type A_l (l \geq 1) .................................................. 205
    8. Systèmes de type D_l (l \geq 3) .................................................. 208
    9. Système de type F_4 ................................................................. 211
   10. Système de type E_8 ................................................................. 213
   11. Système de type E_7 ................................................................. 216
   12. Système de type E_6 ................................................................. 218
   13. Système de type G_2 ................................................................. 220
   14. Systèmes de racines irréductibles non réduits ............... 222

Exercices du § 1 ................................................................. 223
Exercices du § 2 ................................................................. 227
Exercices du § 3 ................................................................. 228
Exercices du § 4 ................................................................. 228

Note historique ................................................................. 234
Bibliographie ................................................................. 241
Index des notations ............................................................ 244
Index terminologique .......................................................... 246

Plancher I : Systèmes de type A_l (l \geq 1) ................................. 250
Plancher II : Systèmes de type B_l (l \geq 2) .................................. 252
Plancher III : Systèmes de type C_l (l \geq 2) .................................. 254
Plancher IV : Systèmes de type D_l (l \geq 3) .................................. 256
Plancher V : Système de type E_6 .................................................. 260
Plancher VI : Système de type E_7 .................................................. 264
Plancher VII : Système de type E_8 .................................................. 268
Plancher VIII : Système de type F_4 .................................................. 272
Plancher IX : Système de type G_2 .................................................. 274
Plancher X : Systèmes irréductibles de rang 2 ............................... 276
Résumé des principales propriétés des systèmes de racines ............ 277 p. 8, l. 5 du bas, au lieu de : (G, N, B, S), lire : (G, B, N, S).
p. 11, l. 17, les deux relations doivent être séparées par une virgule.
p. 12, l. 4 du bas et l. 3 du bas, au lieu de I, lire : S.
p. 14, l. 17, au lieu de distints, lire : distincts.
p. 16, l. 16, au lieu de : 0 ≤ j ≤ q, lire : 0 ≤ j ≤ q + 1.
p. 16, l. 21 et 23, au lieu de : 1 ≤ k ≤ q, lire : 0 ≤ k ≤ q.
p. 30, l. 10 du bas, supprimer « il en est... commutatif ».
p. 32, l. 3 du bas, au lieu de : adjoint lire : des automorphismes intérieurs.
p. 32, l. 2 du bas, au lieu de : chap. III, lire : chap. III, § 6, n° 2, prop. 2.
p. 33, l. 12 du bas, au lieu de : correspondants, lire : correspondant.
p. 38, l. 1 de l’exercice 10, supprimer « d’ordre n ».
p. 40, note (*) de bas de page, première ligne, remplacer : ensemble par : ensemble non vide.
p. 41, l. 3 de l’exercice 17, au lieu de : les éléments de H, lire : les éléments de $\mathfrak{H}$.
p. 43, l. 5 de l’exercice 23, remplacer A par Aut (A).
p. 47, dernière ligne de l’exercice 3, au lieu de : (G, N, B, S), lire : (G, B, N, S).
p. 49, l. 15 du bas, au lieu de : l’application t(C, C’), lire : l’application C’ ↦ t(C, C’).
p. 54, exercice 21, c), deuxième ligne, remplacer : (H, N, B ∩ H, { s }) par : (H, B ∩ H, N, { s }).
p. 55, l. 7, au lieu de : f)*, lire : *f).
p. 67, l. 14 du bas, remplacer V_s par V_s^−.
p. 88, énoncé de la proposition 11, dernière ligne, remplacer C par C’.
p. 111, l. 2, au lieu de : dim_K S^G, lire : dim_K S_n^G.
p. 112, l. 14 du bas, au lieu de : biunivoque, lire : bijective.
p. 114, l. 12 et 11 du bas, supprimer « On sait que... Card (G) = q (Alg. comm., chap. V, § 2, n° 2); ».
p. 114, l. 8 du bas, après : est séparable, insérer : (Alg. comm., chap. V, § 2, n° 2, cor. à la prop. 5).
p. 118, lemme 2, ajouter l’hypothèse : dim V ≥ 2.
p. 121, l. 6, remplacer : D ⊂ C par D ⊗ C.
p. 121, proposition 2, ajouter l’hypothèse que W est irréductible.
p. 128, ligne 3 de l’exercice 5, au lieu de : pour H ∈ S, lire : pour H ∈ J.
p. 132, l. 3, remplacer : mesure par : mesure positive non nulle.
p. 133, exercice 13, dernière ligne, remplacer − V^0 par − H_0.

p. 134, l. 5, le premier graphe doit être

p. 134, exercice 17, premier graphe : la première arête doit être surmontée d’un 4.
p. 143, l. 3, au lieu de : s_α(x) = x − ⟨ α^∨, x ⟩, lire : s_α(x) = x − ⟨ α^∨, x ⟩ α .
p. 144, l. 12, au lieu de : α^∨ ∈ R, lire : α^∨ ∈ R^∨.
p. 146, l. 11, au lieu de : omme, lire : somme.
p. 149, l. 5 du bas, remplacer : p = 0 par : q = 0.
p. 150, l. 5, dessin de gauche : la première flèche est affectée de la lettre γ.
p. 152, l. 7 du bas, au lieu de : α, β ∈ R, lire : α ∈ R.
p. 153, l. 10 du bas, remplacer : (x | y) < 0 par : (x | y) > 0.
p. 169, l. 15 du bas, remplacer : Lemme 3 par : Lemme 4.
p. 169, l. 6 du bas, au lieu de : (*), lire : (Alg., chap. V, nouvelle édition).
p. 169, supprimer la note de bas de page.
p. 171, l. 18 à 25 remplacer : D’après la Remarque... ce qui achève de prouver (iv), par le texte suivant :
Chaque orbite de Γ dans R a au plus h éléments, et il y a au plus l orbites distinctes, d’après ce qui précède.
Or (chap. V, § 6, n° 2, théorème 2, ii)), le cardinal de R est égal à hl, ce qui implique aussitôt (iv).
p. 175, l. 11, au lieu de : déf. 3, lire : déf. 2.
p. 176, l. 3 du bas, remplacer : n_i α par : n_i α_i.
p. 181, l. 10, supprimer : Munissons... par G.
p. 185, l. 20, remplacer : ∑ par : ∏.
p. 192, l. 9 du bas, au lieu de : i, j_1, k_1, lire : i_1, j_1, k_1.

p. 197, l. 9, le graphe doit être : E₆

p. 199, l. 1, remplacer A₁ par Ā₁.
p. 205, l. 11 du bas, au lieu de : n° 6, lire : n° 5.
p. 226, l. 8 du bas, lire : $\sum_i n_i \alpha_i'$.

p. 227, la note de bas de page se réfère à l'exercice 22 de la page précédente.
p. 228, l. 9 au lieu de : dominant, lire : maximal.
p. 230, l. 1 au lieu de : b), lire : b)).
p. 238, l. 10, au lieu de : celles, lire : celle.
p. 239, l. 17, au lieu de : au type exceptionnel G₂, lire : aux types exceptionnels G₂ et F₄.
p. 239, l. 18, au lieu de : (XI), lire : (XI b) et c)).
p. 240, l. 4, insérer une virgule après : § 2.
p. 242, l. 5, ajouter à la fin de la ligne : c) A class of groups in an arbitrary realm connected with the configuration of the 27 lines on a cubic surface, Quart. Journ. of Math., t. XXXIII (1901), p. 145-173, et t. XXXIX (1908), p. 205-209.
p. 252, l. 1 du bas, insérer une virgule avant : γ(R).
p. 254, l. 4 du bas, insérer une virgule avant : γ(R).
p. 256, l. 4 de (II), au lieu de : $\varepsilon_i + \varepsilon_l = \sum_{i \leq k \leq l} \alpha_i$, lire : $\sum_{i \leq k \leq l-2} \alpha_k + \alpha_l$.

p. 257, lignes 12 du bas et 10 du bas, les signes = sont incorrects.
p. 278, lignes 10 et 11, remplacer : Le groupe de Weyl... longueur par : Si R est irréductible, le groupe de Weyl opère transitivement dans l’ensemble des racines de longueur donnée.
p. 279, troisième ligne de 10), remplacer : Hᵢ par : Lᵢ.
p. 282, ligne 13 du bas, les deux signes — doivent être des signes +.
p. 284, ligne 5 du bas, remplacer : n₁, n₂, ..., nₗ par : k₁, ..., kₗ et remplacer : n₁ + ⋯ + nₗ par : k₁ + ⋯ + kₗ.
