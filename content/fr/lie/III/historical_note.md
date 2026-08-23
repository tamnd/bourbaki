---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 0
section_title: Historical Note
kind: historical
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0284-0293
extraction: ocr
statements: 0
exercises: 0
content_sha256: 3ea52a069506bc2f4d227e6bedb50458fd9263744a3903d20e90ff704bef841d
---

# NOTE HISTORIQUE
Chapitres I à III

I. Genèse

La théorie, appelée depuis près d’un siècle « théorie des groupes de Lie », a été édifiée essentiellement par un mathématicien : Sophus Lie.
Avant d’en aborder l’histoire, nous résumerons brièvement diverses recherches antérieures qui en préparèrent le développement.

a) Groupes de transformations (Klein–Lie, 1869–1872)

Vers 1860, la théorie des groupes de permutations d’un ensemble fini se développe et commence à être utilisée (Serret, Kronecker, Mathieu, Jordan). D’autre part, la théorie des invariants, alors en plein essor, familiarise les mathématiciens avec certains ensembles infinis de transformations géométriques stables par composition (notamment les transformations linéaires ou projectives). Mais, avant le travail de 1868 de Jordan (VII) sur les « groupes de mouvements » (sous-groupes fermés du groupe des déplacements de l’espace euclidien à 3 dimensions), il ne semble pas que l’on ait établi de lien conscient entre ces deux courants d’idées.

En 1869, le jeune Félix Klein (1849–1925), élève de Plücker, se lie d’amitié à Berlin avec le norvégien Sophus Lie (1842–1899), de quelques années plus âgé, dont le rapproche leur intérêt commun pour la « géométrie des droites » de Plücker et notamment la théorie des complexes de droites. C’est vers cette période que Lie conçoit l’une de ses idées les plus originales, l’introduction de la notion d’invariant en Analyse et en géométrie différentielle; l’une des sources en est son observation que les méthodes classiques d’intégration « par quadratures » des équations différentielles reposent toutes sur le fait que l’équation est invariante par une famille « continue » de transformations. C’est de 1869 que date le premier travail (rédigé par Klein) où Lie utilise cette idée; il y étudie le « complexe de Reye » (ensemble des droites coupant les faces d’un tétraèdre en 4 points ayant un birapport donné) et les courbes et surfaces admettant pour tangentes des droites de ce complexe (III a)) : sa méthode repose sur l’invariance du complexe de Reye par le groupe commutatif à 3 paramètres (tore maximal de $ \mathbf{PGL}(4, \mathbf{C}) $) laissant invariants les sommets du tétraèdre. Cette même idée domine le travail écrit en commun par Klein et Lie alors qu’ils se trouvent à Paris au printemps 1870 (I a)) ; ils y déterminent essentiellement les sous-groupes connexes commutatifs du groupe projectif du plan $ \mathbf{PGL}(3, \mathbf{C}) $, et étudient les propriétés géométriques de leurs orbites (sous le nom de courbes ou surfaces V) ; cela leur donne, par un procédé uniforme, des propriétés de courbes variées, algébriques ou transcendantes, telles que $ y = cx^m $ ou les spirales logarithmiques. Leurs témoignages s’accordent à souligner l’impression profonde qu’ont produite sur eux les théories de Galois et de Jordan (le commentaire de Jordan sur Galois avait paru aux Math. Annalen en 1869 ; du reste, Lie avait entendu parler de la théorie de Galois dès 1863). Klein, qui en 1871 commence à s’intéresser aux géométries non-euclidiennes, y voit le début de sa recherche d’un principe de classification de toutes les géométries connues, recherche qui devait le conduire en 1872 au « programme d’Erlangen ». De son côté, Lie, dans une lettre de 1873 à A. Mayer (III, vol. V, p. 584), date de son séjour à Paris l’origine de ses idées sur les groupes de transformations, et dans un travail de 1871 (III b)), il utilise déjà le terme de « groupe de transformations » et pose explicitement le problème de la détermination de tous les sous-groupes (« continuus ou discontinus ») de $ \mathbf{GL}(n, \mathbf{C}) $. A vrai dire, Klein et Lie ont dû l’un et l’autre éprouver quelque difficulté à s’insérer dans ce nouvel univers mathématique, et Klein parle du « Traité » de Jordan, nouvellement paru, comme d’un « livre scellé de sept sceaux » (II, p. 51) ; il écrit par ailleurs à propos de (I a) et b)) : « C’est à Lie qu’appartient tout ce qui se rapporte à l’idée heuristique d’un groupe continu d’opérateurs, en particulier tout ce qui touche à l’intégration des équations différentielles ou aux dérivées partielles. Toutes les notions qu’il développa plus tard dans sa théorie des groupes continus se trouvaient déjà en germe chez lui, mais toutefois si peu élaborées, que je dus le convaincre de maints détails, par exemple au début l’existence même des courbes V, au cours de longs entretiens » (II, p. 415).

b) Transformations infinitésimales

La conception d’une transformation « infiniment petite » remonte au moins aux débuts du Calcul infinitésimal ; on sait que Descartes découvre le centre instantané de rotation en admettant que « dans l’infiniment petit » tout mouvement plan peut être assimilé à une rotation ; l’élaboration de la Mécanique analytique, au XVIIIe siècle, est tout entière fondée sur des idées semblables. En 1851, Sylvester, cherchant à former des invariants du groupe linéaire $ \mathbf{GL}(3, \mathbf{C}) $ ou de certains de ses sous-groupes, donne aux paramètres $ z_j $ figurant dans ces matrices des accroissements « infiniment petits » de la forme $ \alpha_j dt $, et exprime qu’une fonction $ f((z_j)) $ est invariante en écrivant l’équation $ f((z_j + \alpha_j dt)) = f((z_j)) $; ceci lui donne pour $ f $ l’équation linéaire aux dérivées partielles $ Xf = 0 $, où

$$
Xf = \sum_j \alpha_j \frac{\partial f}{\partial z_j},
$$

$ X $ étant donc un opérateur différentiel, « dérivée dans la direction de paramètres directeurs $ \alpha_j $ » (V, vol. 3, p. 326 et 327); Sylvester semble sentir qu’il y a là un principe général d’une assez grande portée, mais ne paraît pas être revenu sur la question. Un peu plus tard, Cayley (VI, t. II, p. 164–178) procède de même pour les invariants de $ \mathbf{SL}(2, \mathbf{C}) $ dans certaines représentations de ce groupe et montre que ce sont les solutions de deux équations aux dérivées partielles du premier ordre $ Xf = 0, Yf = 0 $, où $ X $ et $ Y $ sont obtenus comme ci-dessus à partir des transformations « infiniment petites »

$$
\begin{pmatrix}
0 & 0 \\
dt & 0
\end{pmatrix}
\text{ et }
\begin{pmatrix}
0 & dt \\
0 & 0
\end{pmatrix}.
$$

En termes modernes, cela s’explique par le fait que $ X $ et $ Y $ engendrent l’algèbre de Lie $ \mathfrak{sl}(2, \mathbf{C}) $; d’ailleurs Cayley calcule explicitement le crochet $ XY - YX $ et montre qu’il provient lui aussi d’une transformation « infiniment petite ».

Dans son mémoire de 1868 sur les groupes de mouvements (VII), Jordan utilise d’un bout à l’autre le concept de « transformation infiniment petite », mais exclusivement d’un point de vue géométrique. C’est sans doute chez lui qu’apparaît l’idée d’un groupe à un paramètre « engendré » par une transformation infiniment petite : pour Jordan, c’est l’ensemble des transformations obtenues en « répétant convenablement » la transformation infiniment petite (*loc. cit.*, p. 243). Klein et Lie, dans leur mémoire de 1871, utilisent la même expression « transformation infiniment petite répétée » (I b)), mais le contexte montre qu’ils entendent par là une intégration d’un système différentiel. Si le groupe à un paramètre qu’ils considèrent est formé des transformations $ x' = f(x, y, t),\ y' = g(x, y, t) $, la « transformation infiniment petite » correspondante est donnée par

$$
dx = p(x, y)\ dt,\quad dy = q(x, y)\ dt
$$

où $ p(x, y) = \frac{\partial f}{\partial t}(x, y, t_0),\ q(x, y) = \frac{\partial g}{\partial t}(x, y, t_0) $, et $ t_0 $ correspond à la transformation identique du groupe. Comme Klein et Lie connaissent explicitement les fonctions $ f $ et $ g $, ils n’ont pas de peine à vérifier que les fonctions

$$
t \mapsto f(x, y, t) \quad \text{et} \quad t \mapsto g(x, y, t)
$$

donnent sous forme paramétrique la courbe intégrale de l’équation différentielle

$$
q(\xi, \eta)\ d\xi = p(\xi, \eta)\ d\eta
$$

passant par le point $ (x, y) $, mais n’en donnent aucune raison générale ; ils n’utilisent d’ailleurs plus ce fait dans la suite de leur mémoire.

c) Transformations de contact

Dans les deux années suivantes, Lie paraît abandonner la théorie des groupes de transformations (bien qu’il reste en contact très suivi avec Klein, qui publie en 1872 son « Programme ») pour étudier les transformations de contact, l’intégration des équations aux dérivées partielles du premier ordre et les relations entre ces deux théories. Nous n’avons pas à faire l’historique de ces questions ici, et nous nous bornerons à mentionner quelques points qui paraissent avoir joué un rôle important dans la genèse de la théorie des groupes de transformations.

La notion de transformation de contact généralise à la fois les transformations ponctuelles et les transformations par polaires réciproques. Grosso modo, une transformation de contact¹ dans $ \mathbf{C}^n $ est un isomorphisme d’un ouvert $ \Omega $ de la variété $ T'(\mathbf{C}^n) $ des vecteurs cotangents à $ \mathbf{C}^n $ sur un autre ouvert $ \Omega' $ de $ T'(\mathbf{C}^n) $ transformant la 1-forme canonique de $ \Omega $ en celle de $ \Omega' $. En d’autres termes, si $ (x_1, \ldots, x_n, p_1, \ldots, p_n) $ désignent les coordonnées canoniques de $ T'(\mathbf{C}^n) $, une transformation de contact est un isomorphisme $ (x_i, p_i) \mapsto (X_i, P_i) $ satisfaisant à la relation $ \sum_{i=1}^n P_i\, dX_i = \sum_{i=1}^n p_i\, dx_i $. De telles transformations interviennent dans l’étude de l’intégration des équations aux dérivées partielles de la forme

$$
F\left(x_1, x_2, \ldots, x_n, \frac{\partial z}{\partial x_1}, \ldots, \frac{\partial z}{\partial x_n}\right) = 0.
$$

Lie se familiarise au cours de ses recherches sur ces questions avec le maniement des parenthèses de Poisson

$$
(f, g) = \sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \frac{\partial g}{\partial p_i} - \frac{\partial g}{\partial x_i} \frac{\partial f}{\partial p_i} \right)
$$

et des crochets² $ [X, Y] = XY - YX $ d’opérateurs différentiels du type (1); il interprète la parenthèse de Poisson (3) comme l’effet sur $ f $ d’une transformation de type (1) associée à $ g $, et observe à cette occasion que l’identité de Jacobi pour les parenthèses de Poisson signifie que le crochet des opérateurs différentiels correspondant à $ g $ et $ h $ est associé à la parenthèse $ (g, h) $. La recherche de fonctions $ g $ telles que $ (F, g) = 0 $, qui intervient dans la méthode de Jacobi pour intégrer

¹ Il s’agit ici de transformations de contact « homogènes ». Antérieurement, la considération d’équations du type (2), mais où $ z $ intervient dans $ F $, avait amené Lic à considérer des transformations de contact à $ 2n + 1 $ variables $ z, x_1, \ldots, x_n, p_1, \ldots, p_n $, où il s’agit de trouver $ 2n + 2 $ fonctions $ Z, P_i, X_i $ $ (1 \leq i \leq n) $ et $ \rho $ (cette dernière $ \neq 0 $ en tout point) telles que $ dZ - \sum_i P_i\, dX_i = \rho(dz - \sum_i p_i\, dx_i) $.

Ce cas en apparence plus général se ramène d’ailleurs aisément au cas « homogène » (IV, t. 2, p. 135–146).

² Ceux-ci intervenaient déjà dans la théorie de Jacobi-Clebsch des « systèmes complets » d’équations aux dérivées partielles du premier ordre $ X_j f = 0 $ $ (1 \leq j \leq r) $, notion équivalente à celle de « système complètement intégrable » de Frobenius : le théorème fondamental (équivalent au « théorème de Frobenius ») qui caractérise ces systèmes est que les crochets $ [X_i, X_j] $ doivent être des combinaisons linéaires (à coefficients variables) des $ X_k $.

l’équation aux dérivées partielles (2), devient pour Lie celle d’une transformation infinitésimale de contact laissant invariante l’équation donnée. Enfin, Lie est amené à étudier des ensembles de fonctions $(u_j)_{1 \leq j \leq m}$ des $x_i$ et des $p_i$ tels que les parenthèses $(u_j, u_k)$ soient fonctions des $u_h$, et nomme « groupes » ces ensembles (déjà considérés en substance par Jacobi).

II. Groupes continus et transformations infinitésimales

Brusquement, à l’automne 1873, Lie reprend l’étude des groupes de transformations et obtient des résultats décisifs. Pour autant qu’on puisse suivre le cheminement de sa pensée dans quelques lettres à A. Mayer des années 1873–1874 (III, t. 5, p. 584–608), il part d’un « groupe continu » de transformations sur $n$ variables

$$
x'_i = f_i(x_1, \ldots, x_n, a_1, \ldots, a_r) \quad (1 \leq i \leq n)
$$

dépendant effectivement¹ de $r$ paramètres $a_1, \ldots, a_r$; il observe que, si la transformation (4) est l’identité pour les valeurs $a_1^0, \ldots, a_r^0$ des paramètres,² alors les développements de Taylor des $x_i$, limités au premier ordre:

$$
f_i(x_1, \ldots, x_n, a_1^0 + z_1, \ldots, a_r^0 + z_r) = x_i + \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) + \cdots \quad (1 \leq i \leq n)
$$

donnent une transformation infiniment petite « générique » dépendant linéairement des $r$ paramètres $z_j$

$$
dx_i = \left( \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) \right) dt \quad (1 \leq i \leq n).
$$

Procédant comme dans son mémoire avec Klein, Lie intègre le système différentiel

$$
\frac{d\xi_1}{\sum_k z_k X_{k1}(\xi_1, \ldots, \xi_n)} = \cdots = \frac{d\xi_n}{\sum_k z_k X_{kn}(\xi_1, \ldots, \xi_n)} = dt,
$$

ce qui lui donne, pour tout point $(z_1, \ldots, z_r)$, un groupe à un paramètre

$$
t \mapsto x'_i = g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, t) \quad (1 \leq i \leq n)
$$

¹ Lie entend par là que les $f_i$ ne peuvent s’exprimer à l’aide de moins de $r$ fonctions des $a_j$, ou encore que la matrice jacobienne $(\partial f_i / \partial a_j)$ est de rang $r$ « en général ».
² Dans ses premières notes, Lie pense pouvoir démontrer a priori l’existence de l’identité et de l’inverse dans tout ensemble de transformations (4) stable par composition; il reconnaît plus tard que sa démonstration était incorrecte, et Engel lui fournit un contre-exemple reproduit dans (IV, vol. 1, § 44). Toutefois, Lie montre comment on ramène les systèmes « continus » (4) stables par composition aux groupuscules de transformations: un tel système est de la forme $G \circ h$, où $G$ est un groupuscule de transformations et $h$ une transformation du système (IV, vol. 1, th. 26, p. 163 et vol. 3, th. 46, p. 572) tel que $ g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, 0) = x_i $ pour tout $ i $. Il montre de façon ingénieuse, en utilisant le fait que les transformations (4) forment un ensemble stable par composition, que le groupe à un paramètre (8) est un sous-groupe du groupe donné (III d)). L’idée nouvelle, clé de toute la théorie, est de pousser jusqu’au second ordre les développements de Taylor des fonctions (4). La marche de son raisonnement est assez confuse et heuristique ((III d)) et (III, vol. 5, p. 600–601)); on peut la présenter de la façon suivante. Pour les $ z_j $ assez petits, on peut faire $ t = 1 $ dans (8), et on obtient ainsi de nouveaux paramètres $ z_1, \ldots, z_r $ pour les transformations du groupe (c’est en fait la première apparition des « paramètres canoniques »). On a par définition, vu (7)

$$
\frac{\partial g_i}{\partial t} = \sum_k z_k X_{ki}(x'_1, \ldots, x'_n),
$$

d’où

$$
\frac{\partial^2 g_i}{\partial t^2} = \sum_{k,j} z_k \frac{\partial X_{kt}}{\partial x_j} (x'_1, \ldots, x'_n) \frac{\partial x'_j}{\partial t}
$$
$$
= \sum_{k,j} z_k \frac{\partial X_{kt}}{\partial x_j} (x'_1, \ldots, x'_n) \left( \sum_h z_h X_{hj}(x'_1, \ldots, x'_n) \right)
$$

ce qui donne

$$
x'_i = x_i + \left( \sum_k z_k X_{ki}(x_1, \ldots, x_n) \right)t
$$
$$
+ \frac{1}{2} \left( \sum_{k,h,j} z_k z_h \frac{\partial X_{kt}}{\partial x_j} (x_1, \ldots, x_n) X_{hj}(x_1, \ldots, x_n) \right)t^2 + \cdots,
$$

d’où, pour $ t = 1 $, les développements de Taylor par rapport aux paramètres $ z_j $

(9) $$ x'_i = x_i + \left( \sum_k z_k X_{ki} \right) + \frac{1}{2} \left( \sum_{k,h,j} z_k z_h X_{hj} \frac{\partial X_{ki}}{\partial x_j} \right) + \cdots \quad (1 \leq i \leq n). $$

Ecrivons en abrégé ces relations $ x' = G(x, z) $ entre vecteurs

$$
x = (x_1, \ldots, x_n), \qquad x' = (x'_1, \ldots, x'_n), \qquad z = (z_1, \ldots, z_r);
$$

la propriété fondamentale de stabilité de l’ensemble de ces transformations par composition s’écrit

(10) $$ G(G(x, u), v) = G(x, H(u, v)) $$

où $ H = (H_1, \ldots, H_r) $ est indépendant de $ x $; il est immédiat que $ H(u, 0) = u, H(0, v) = v $, d’où les développements

(11) $$ H_i(u, v) = u_i + v_i + \frac{1}{2} \sum_{h,k} c_{ikh} u_h v_k + \cdots, $$

les termes non écrits étant non linéaires en $ u $ ou en $ v $. Transformant (10) à l’aide de (9) et (11), puis comparant les termes en $ u_h v_k $ des deux membres, Lie obtient les relations

$$
(12) \quad \sum_{j=1}^n \left( X_{hj} \frac{\partial X_{ki}}{\partial x_j} - X_{kj} \frac{\partial X_{hi}}{\partial x_j} \right) = \sum_{l=1}^r c_{lhk} X_{li} \qquad (1 \leq h, k \leq r, 1 \leq i \leq n).
$$

Sa pratique de la théorie des équations aux dérivées partielles l’amène à écrire ces conditions sous une forme plus simple: suivant le modèle de (1), il associe à chacune des $ r $ transformations infiniment petites obtenues en faisant $ z_k = 1 $, $ z_h = 0 $ pour $ h \neq k $ dans (6), l’opérateur différentiel

$$
(13) \qquad A_k(f) = \sum_{i=1}^n X_{ki} \frac{\partial f}{\partial x_i},
$$

et récrit les conditions (12) sous la forme

$$
(14) \qquad [A_h, A_k] = \sum_l c_{lhk} A_l,
$$

pierre angulaire de sa théorie. Jusque là, il avait utilisé indifféremment les termes « transformation infiniment petite » et « transformation infinitésimale » (*e.g.* (III c)) ; la simplicité des relations (14) le conduit à appeler l’opérateur (13) le « symbole » de la transformation infinitésimale $ dx_i = X_{ki} dt $ ($ 1 \leq i \leq n $) (III e)) et très rapidement, c’est l’opérateur (13) lui-même qu’il appellera « *transformation infinitésimale* » ((III e)) et (III, vol. 5, p. 589)).

Il devient alors conscient des liens étroits qui unissent la théorie des « groupes continus » à ses recherches antérieures sur les transformations de contact et les équations aux dérivées partielles. Ce rapprochement le remplit d’enthousiasme : « *Mes anciens travaux étaient pour ainsi dire tout prêts d’avance pour fonder la nouvelle théorie des groupes de transformations* » écrit-il à Mayer en 1874 (III, t. 5, p. 586).

Dans les années suivantes, Lie poursuit l’étude des groupes de transformations. Outre les théorèmes généraux résumés ci-après (§ III), il obtient un certain nombre de résultats plus particuliers : détermination des groupes de transformations de la droite et du plan, des sous-groupes de petite codimension des groupes projectifs, des groupes à au plus 6 paramètres, etc. Il n’abandonne pas pour autant les équations différentielles. En fait, il semble même que, pour lui, la théorie des groupes de transformations devait être un instrument pour intégrer les équations différentielles, où le groupe de transformations jouerait un rôle analogue à celui du groupe de Galois d’une équation algébrique.\footnote{Ces recherches n’ont eu que peu d’influence sur la théorie générale des équations différentielles, le groupe d’automorphismes d’une telle équation étant le plus souvent trivial. En revanche, pour certains types d’équations (par exemple linéaires), des résultats intéressants ont été obtenus ultérieurement par Picard, Vessiot, puis, plus récemment, Ritt et Kolchin.} Notons que ces recherches l’amènent également à introduire certains ensembles de transformations à une infinité de paramètres, qu’il appelle « groupes infinis et continus »¹ ; il réserve le nom de « groupes finis et continus » aux groupes de transformation à un nombre fini de paramètres du type (4) ci-dessus.

III. Le « dictionnaire » groupes de Lie-algèbres de Lie

La théorie des groupes « finis et continus », développée par Lie dans de nombreux mémoires à partir de 1874, est exposée systématiquement dans l’imposant traité « Theorie der Transformationsgruppen » ((IV), 1888–1893), écrit en collaboration avec F. Engel² ; elle y fait l’objet du premier volume et des cinq derniers chapitres du troisième, le second étant consacré aux transformations de contact.

Comme l’indique le titre, il n’est jamais question dans cet ouvrage que de groupes de transformations, au sens des équations (4), où l’espace des « variables » $ x_i $ et l’espace des « paramètres » $ a_j $ jouent des rôles initialement aussi importants. D’ailleurs le concept de groupe « abstrait » n’est pas clairement dégagé à cette époque; quand en 1883 (III g)) Lie remarque qu’avec les notations de (10), l’équation $ w = \mathrm{H}(u, v) $ qui donne les paramètres de la composée de deux transformations du groupe définit un nouveau groupe, c’est comme groupe de transformations sur l’espace des paramètres qu’il le considère, obtenant ainsi ce qu’il appelle le « groupe de paramètres » (il en obtient même deux, qui ne sont autres que le groupe des translations à gauche et le groupe des translations à droite³).

Les variables $ x_i $ et les paramètres $ a_j $ dans les équations (4) sont en principe supposés complexes (sauf dans les chapitres XIX–XXIV du tome 3), et les fonctions $ f_i $ analytiques; Lie et Engel sont bien entendu conscients du fait que ces fonctions ne sont pas en général définies pour toutes les valeurs complexes des $ x_i $ et des $ a_j $ et que, par suite, la composition de telles transformations soulève de sérieuses difficultés (IV, t. 1, p. 15–17, p. 33–40 et passim); et bien que, par la suite, ils s’expriment presque toujours comme si la composition des transformations qu’ils étudient était possible sans restriction, ce n’est sans doute que pour la commodité des énoncés, et ils rétablissent explicitement le point de vue « local » chaque fois que c’est nécessaire (cf. loc. cit., p. 168 ou 189 par exemple ou ibid., t. 3, p. 2, note de bas de page); en d’autres termes, l’objet mathématique

¹ On les appelle aujourd’hui « pseudo-groupes de Lie »; on aura soin de ne pas les confondre avec les groupes de Lie « banachiques » définis dans ce volume.
² De 1886 à 1898, Lie occupa à Leipzig la chaire laissée vacante par Klein et eut Engel pour assistant; cette circonstance favorisa l’éclosion d’une active école mathématique ainsi que la diffusion des idées de Lie, assez peu connues jusque là (en raison, notamment, du fait que ses premiers mémoires étaient le plus souvent écrits en norvégien, et publiés dans les Comptes Rendus de l’Académie de Christiania, peu répandus ailleurs). C’est ainsi qu’à une époque où il n’était guère d’usage pour les jeunes mathématiciens français d’aller s’instruire en Allemagne, E. Vessiot et A. Tresse passèrent une année d’études à Leipzig, avec Sophus Lie.
³ La notion analogue pour les groupes de permutations avait été introduite et étudiée par Jordan dans son « Traité ».

qu’ils étudient est voisin de ce que nous appelons dans ce traité un morceau de loi d’opération. Ils ne se font pas faute, à l’occasion, de considérer des groupes globaux, par exemple les 4 séries de groupes classiques (IV, t. 3, p. 682), mais ne paraissent pas s’être posé la question de ce que peut être en général un « groupe global »; il leur suffit de pouvoir obtenir, pour les « paramètres » des groupes classiques (les « variables » de ces groupes n’introduisent aucune difficulté, puisqu’il s’agit de transformations linéaires de $ \mathbf{C}^n $), des systèmes de paramètres « locaux » au voisinage de la transformation identique, sans qu’ils s’inquiètent du domaine de validité des formules qu’ils écrivent. Ils se posent toutefois un problème qui sort nettement de la théorie locale¹: l’étude des groupes « mixtes », c’est-à-dire des groupes ayant un nombre fini de composantes connexes, tel le groupe orthogonal (IV, t. 1, p. 7). Ils présentent cette étude comme celle d’un ensemble de transformations stable par composition et passage à l’inverse qui est réunion d’ensembles $ H_j $ dont chacun est décrit par des systèmes de fonctions $ (f_i^{(j)}) $ comme dans (4); le nombre de paramètres (essentiels) de chaque $ H_j $ est même $ a priori $ supposé dépendre de $ j $, mais ils montrent qu’en fait ce nombre est le même pour tous les $ H_j $. Leur résultat principal est alors l’existence d’un groupe fini et continu $ G $ tel que $ H_j = G \circ h_j $ pour un $ h_j \in H_j $ et pour tout $ j $; ils établissent aussi que $ G $ est distingué dans le groupe mixte et remarquent que la détermination des invariants de ce dernier se ramène à celle des invariants de $ G $ et d’un groupe discontinu (IV, t. 1, chap. 18).

La théorie générale développée dans (IV) aboutit (sans que cela soit dit de façon très systématique par les auteurs) à forger un « dictionnaire » faisant passer des propriétés des groupes « finis et continus » à celles de l’ensemble de leurs transformations infinitésimales. Il est basé sur les « trois théorèmes de Lie », dont chacun est formé d’une assertion et de sa réciproque.

Le premier théorème (IV, t. 1, p. 33 et 72 et t. 3, p. 563) affirme en premier lieu que si dans (4) les paramètres sont effectifs, les fonctions $ f_i $ vérifient un système d’équations aux dérivées partielles de la forme

$$
\frac{\partial f_i}{\partial a_j} = \sum_{k=1}^r \xi_{kji}(f(x, a)) \psi_{kj}(a) \qquad (1 \leq i \leq n)
$$

où la matrice $ (\xi_{kji}) $ est de rang maximum et $ \det(\psi_{kj}) \neq 0 $; réciproquement, si les fonctions $ f_i $ ont cette propriété, les formules (4) définissent un groupuscule de transformations.

Le deuxième théorème (IV, t. 1, p. 149 et 158, et t. 3, p. 590) donne des relations

¹ Rappelons (Note historique d’Alg., chap. VIII, p. 170) qu’à la suite d’une Note de H. Poincaré (XIV, t. V, p. 77–79) divers auteurs ont étudié le groupe des éléments inversibles d’une algèbre associative de dimension finie. Il est intéressant de noter à ce propos que E. Study, dans ses travaux sur ce sujet, introduit un symbolisme qui revient en substance à envisager le groupe abstrait défini par le groupe des paramètres.

entre les $ \xi_{kli} $ d’une part, les $ \psi_{ij} $ de l’autre : les conditions sur les $ \xi_{kli} $ s’écrivent sous la forme

$$
(16) \quad \sum_{k=1}^{n} \left( \xi_{ik} \frac{\partial \xi_{jl}}{\partial x_k} - \xi_{jk} \frac{\partial \xi_{il}}{\partial x_k} \right) = \sum_{k=1}^{r} c_{ij}^{kc} \xi_{kl} \qquad (1 \leq i, j \leq r, 1 \leq l \leq n)
$$

où les $ c_{ij}^{k} $ sont des constantes ($ 1 \leq i, j, k \leq r $) antisymétriques en $ i, j $. Les conditions sur les $ \psi_{ij} $, sous la forme donnée par Maurer (X), sont :

$$
(17) \quad \frac{\partial \psi_{kl}}{\partial a_m} - \frac{\partial \psi_{km}}{\partial a_l} = \frac{1}{2} \sum_{1 \leq i, j \leq r} c_{ij}^{k} (\psi_{il} \psi_{jm} - \psi_{jl} \psi_{im}) \qquad (1 \leq k, l, m \leq r).
$$

En introduisant la matrice $ (\alpha_{ij}) $ contragrédiente de $ (\psi_{ij}) $ et les transformations infinitésimales

$$
(18) \quad X_k = \sum_{i=1}^{n} \xi_{kli} \frac{\partial}{\partial x_i}, \qquad A_k = \sum_{j=1}^{r} \alpha_{kj} \frac{\partial}{\partial a_j} \qquad (1 \leq k \leq r),
$$

on peut écrire (16) et (17) respectivement :

$$
(19) \quad [X_i, X_j] = \sum_{k=1}^{r} c_{ij}^{k} X_k \qquad (1 \leq i, j \leq r).
$$
$$
(20) \quad [A_i, A_j] = \sum_{k=1}^{r} c_{ij}^{k} A_k
$$

Réciproquement, si l’on se donne $ r $ transformations infinitésimales $ X_k $ ($ 1 \leq k \leq r $) linéairement indépendantes et vérifiant les conditions (19), les sous-groupes à un paramètre engendrés par ces transformations engendrent un groupe de transformations à $ r $ paramètres essentiels.

Enfin, le troisième théorème (IV, t. 1, p. 170 et 297 et t. 3, p. 597) ramène la détermination des systèmes de transformations infinitésimales $ (X_k)_{1 \leq k \leq r} $ vérifiant (19) à un problème purement algébrique : on doit avoir

$$
(21) \quad c_{ij}^{k} + c_{ji}^{k} = 0
$$
$$
(22) \quad \sum_{l=1}^{r} (c_{il}^{m} c_{jk}^{l} + c_{kl}^{m} c_{ij}^{l} + c_{jl}^{m} c_{ki}^{l}) = 0 \qquad (1 \leq i, j, k, m \leq r).
$$

Réciproquement,$^1$ si (21) et (22) sont vérifiées, il existe un système de transformations infinitésimales satisfaisant aux relations (19), d’où un groupe de transformations à $ r $ paramètres (en d’autres termes, les combinaisons linéaires à

$ ^1 $ Cette réciproque n’a pas été obtenue sans peine. La première démonstration qu’en donne Lie (III e)) consiste à passer au groupe adjoint et n’est en fait valable que si le centre de l’algèbre de Lie donnée est réduit à 0. Il en donne ensuite deux démonstrations générales (IV, vol. 2, chap. XVII et vol. 3, p. 599-604); il est assez significatif que la première soit basée sur les transformations de contact et que Lie la trouve plus naturelle que la deuxième.
