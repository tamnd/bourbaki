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
pdf_pages: 0233-0242
extraction: ocr
statements: 0
exercises: 0
content_sha256: 07158e7b6d6960166ec657441207283ea61602ecd97ccf833867d644df988fb3
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
