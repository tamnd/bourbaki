---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ÉLÉMENTS D'HISTOIRE DES MATHÉMATIQUES
section: 25
section_title: Groupes de Lie et algèbres de Lie
lang: fr
source: hist-fr
pdf_pages: 0307-0331
extraction: ocr
statements: 0
exercises: 0
content_sha256: 1271bc08eebd59c729cae3cb5b7aa2288df606f0768dfd0031fc17ebf9bf2c5b
---

## 25. GROUPES DE LIE ET ALGÈBRES DE LIE

I. GENÈSE

La théorie, appelée depuis près d’un siècle « théorie des groupes de Lie », a été édifiée essentiellement par un mathématicien : Sophus Lie.

Avant d’en aborder l’histoire, nous résumerons brièvement diverses recherches antérieures qui en préparèrent le développement.

a) Groupes de transformations (Klein-Lie, 1869-1872)

Vers 1860, la théorie des groupes de permutations d’un ensemble fini se développe et commence à être utilisée (Serret, Kronecker, Mathieu, Jordan). D’autre part, la théorie des invariants, alors en plein essor, familiarise les mathématiciens avec certains ensembles infinis de transformations géométriques stables par composition (notamment les transformations linéaires ou projectives). Mais, avant le travail de 1868 de Jordan [174 b] sur les « groupes de mouvements » (sous-groupes fermés du groupe des déplacements de l’espace euclidien à 3 dimensions), il ne semble pas que l’on ait établi de lien conscient entre ces deux courants d’idées.

En 1869, le jeune Félix Klein (1849-1925), élève de Plücker, se lie d’amitié à Berlin avec le norvégien Sophus Lie (1842-1899), de quelques années plus âgé, dont le rapproche leur intérêt commun pour la « géométrie des droites » de Plücker et notamment la théorie des complexes de droites (p. 167). C’est vers cette période que Lie conçoit l’une de ses idées les plus originales, l’introduction de la notion d’invariant en Analyse et en géométrie différentielle ; l’une des sources en est son observation que les méthodes classiques d’intégration « par quadratures » des équations différentielles reposent toutes sur le fait que l’équation est invariante par une famille « continue » de transformations. C’est de 1869 que date le premier travail (rédigé par Klein) où Lie utilise cette idée; il y étudie le « complexe de Reye » (ensemble des droites coupant les faces d’un tétraèdre en 4 points ayant un birapport donné) et les courbes et surfaces admettant pour tangentes des droites de ce complexe ([202], vol. 1, Abh. V, p. 68-77): sa méthode repose sur l’invariance du complexe de Reye par le groupe commutatif à 3 paramètres (tore maximal de $\mathbf{PGL}(4, \mathbf{C})$) laissant invariants les sommets du tétraèdre. Cette même idée domine le travail écrit en commun par Klein et Lie alors qu’ils se trouvent à Paris au printemps 1870 ([/82], t. I, p. 416-420); ils y déterminent essentiellement les sous-groupes connexes commutatifs du groupe projectif du plan $\mathbf{PGL}(3, \mathbf{C})$, et étudient les propriétés géométriques de leurs orbites (sous le nom de courbes ou surfaces V); cela leur donne, par un procédé uniforme, des propriétés de courbes variées, algébriques ou transcendantes. telles que $y = cx^m$ ou les spirales logarithmiques. Leurs témoignages s’accordent à souligner l’impression profonde qu’ont produite sur eux les théories de Galois et de Jordan (le commentaire de Jordan sur Galois avait paru aux Math. Annalen en 1869; du reste. Lie avait entendu parler de la théorie de Galois dès 1863). Klein, qui en 1871 commence à s’intéresser aux géométries non-euclidiennes, y voit le début de sa recherche d’un principe de classification de toutes les géométries connues, recherche qui devait le conduire en 1872 au « programme d’Erlangen ». De son côté, Lie, dans une lettre de 1873 à A. Mayer ([202], vol. 5, p. 584), date de son séjour à Paris l’origine de ses idées sur les groupes de transformations, et dans un travail de 1871 ([202], vol. I, Abh. XII, p. 153-214), il utilise déjà le terme de « groupe de transformations » et pose explicitement le problème de la détermination de tous les sous-groupes (« continuus ou discontinus ») de $\mathbf{GL}(n, \mathbf{C})$. À vrai dire, Klein et Lie ont dû l’un et l’autre éprouver quelque difficulté à s’insérer dans ce nouvel univers mathématique, et Klein parle du « Traité » de Jordan, nouvellement paru, comme d’un « livre scellé de sept sceaux » ([/82], t. I, p. 51); il écrit par ailleurs à propos de ([/82], t. I, p. 424-459): « C’est à Lie qu’appartient tout ce qui se rapporte à l’idée heuristique d’un groupe continu d’opérateurs, en particulier tout ce qui touche à l’intégration des équations différentielles ou aux dérivées partielles. Toutes les notions qu’il développa plus tard dans sa théorie des groupes continus se trouvaient déjà en germe chez lui, mais toutefois si peu élaborées, que je dus le convaincre de maints détails, par exemple au début l’existence même des courbes V, au cours de longs entretiens » ([/82], t. I, p. 415).

b) Transformations infinitésimales

La conception d'une transformation « infiniment petite » remonte au moins aux débuts du Calcul infinitésimal ; on sait que Descartes découvre le centre instantané de rotation en admettant que « dans l'infiniment petit » tout mouvement plan peut être assimilé à une rotation ; l'élaboration de la Mécanique analytique, au XVIIIe siècle, est tout entière fondée sur des idées semblables. En 1851, Sylvester, cherchant à former des invariants du groupe linéaire $\mathbf{GL}(3, \mathbf{C})$ ou de certains de ses sous-groupes, donne aux paramètres $z_j$ figurant dans ces matrices des accroissements « infiniment petits » de la forme $\alpha_j dt$, et exprime qu'une fonction $f((z_j))$ est invariante en écrivant l'équation $f((z_j + \alpha_j dt)) = f((z_j))$; ceci lui donne pour $f$ l'équation linéaire aux dérivées partielles $Xf = 0$, où

$$
Xf = \sum_j \alpha_j \frac{\partial f}{\partial z_j},
$$

$X$ étant donc un opérateur différentiel, « dérivée dans la direction de paramètres directeurs $\alpha_j$ » ([304], vol. 3, p. 326 et 327); Sylvester semble sentir qu'il y a là un principe général d'une assez grande portée, mais ne paraît pas être revenu sur la question. Un peu plus tard, Cayley ([58], t. II, p. 164-178) procède de même pour les invariants de $\mathbf{SL}(2, \mathbf{C})$ dans certaines représentations de ce groupe et montre que ce sont les solutions de deux équations aux dérivées partielles du premier ordre $Xf = 0$, $Yf = 0$, où $X$ et $Y$ sont obtenus comme ci-dessus à partir des transformations « infiniment petites »

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

En termes modernes, cela s'explique par le fait que $X$ et $Y$ engendrent l'algèbre de Lie $\mathfrak{sl}(2, \mathbf{C})$; d'ailleurs Cayley calcule explicitement le crochet $XY - YX$ et montre qu'il provient lui aussi d'une transformation « infiniment petite ».

Dans son mémoire de 1868 sur les groupes de mouvements [174 b], Jordan utilise d'un bout à l'autre le concept de « transformation infiniment petite », mais exclusivement d'un point de vue géométrique. C'est sans doute chez lui qu'apparaît l'idée d'un groupe à un paramètre « engendré » par une transformation infiniment petite : pour Jordan, c'est l'ensemble des transformations obtenues en « répétant convenablement » la transformation infiniment petite (loc. cit., p. 243).

Klein et Lie, dans leur mémoire de 1871, utilisent la même expression « transformation infiniment petite répétée » ([182], t. I, p. 424-459), mais le contexte montre qu’ils entendent par là une intégration d’un système différentiel. Si le groupe à un paramètre qu’ils considèrent est formé des transformations $x' = f(x, y, t),\ y' = g(x, y, t)$, la « transformation infiniment petite » correspondante est donnée par
$$
dx = p(x, y)dt,\qquad dy = q(x, y)dt
$$
où $p(x, y) = \frac{\partial f}{\partial t}(x, y, t_0),\ q(x, y) = \frac{\partial g}{\partial t}(x, y, t_0)$, et $t_0$ correspond à la transformation identique du groupe. Comme Klein et Lie connaissent explicitement les fonctions $f$ et $g$, ils n’ont pas de peine à vérifier que les fonctions
$$
t \mapsto f(x, y, t)\qquad \text{et}\qquad t \mapsto g(x, y, t)
$$
donnent sous forme paramétrique la courbe intégrale de l’équation différentielle
$$
q(\xi, \eta)d\xi = p(\xi, \eta)d\eta
$$
passant par le point $(x, y)$, mais n’en donnent aucune raison générale; ils n’utilisent d’ailleurs plus ce fait dans la suite de leur mémoire.

c) Transformations de contact

Dans les deux années suivantes, Lie paraît abandonner la théorie des groupes de transformations (bien qu’il reste en contact très suivi avec Klein, qui publie en 1872 son « Programme ») pour étudier les transformations de contact, l’intégration des équations aux dérivées partielles du premier ordre et les relations entre ces deux théories. Nous n’avons pas à faire l’historique de ces questions ici, et nous nous bornerons à mentionner quelques points qui paraissent avoir joué un rôle important dans la genèse de la théorie des groupes de transformations.

La notion de transformation de contact généralise à la fois les transformations ponctuelles et les transformations par polaires réciproques. Grosso modo, une transformation de contact \* dans $\mathbf{C}^n$ est

\* Il s’agit ici de transformations de contact « homogènes ». Antérieurement, la considération d’équations du type (2), mais où $z$ intervient dans $F$, avait amené Lie à considérer des transformations de contact à $2n + 1$ variables $z, x_1, \ldots, x_n, p_1, \ldots, p_n$, où il s’agit de trouver $2n + 2$ fonctions $Z, P_i, X_i$ ($1 \leq i \leq n$) et $\rho$ (cette dernière $\neq 0$ en tout point) telles que $dZ - \sum P_i dX_i = \rho(dz - \sum p_i dx_i)$.

Ce cas en apparence plus général se ramène d’ailleurs aisément au cas « homogène » ([203], t. 2, p. 135-146).

un isomorphisme d’un ouvert $\Omega$ de la variété $T'(\mathbf{C}^n)$ des vecteurs cotangents à $\mathbf{C}^n$ sur un autre ouvert $\Omega'$ de $T'(\mathbf{C}^n)$ transformant la 1-forme canonique de $\Omega$ en celle de $\Omega'$. En d’autres termes, si $(x_1, \ldots, x_n, p_1, \ldots, p_n)$ désignent les coordonnées canoniques de $T'(\mathbf{C}^n)$, une transformation de contact est un isomorphisme $(x_i, p_i) \mapsto (X_i, P_i)$ satisfaisant à la relation $\sum_{i=1}^n P_i dX_i = \sum_{i=1}^n p_i dx_i$.

De telles transformations interviennent dans l’étude de l’intégration des équations aux dérivées partielles de la forme

$$
\text{(2)} \quad F\left(x_1, x_2, \ldots, x_n, \frac{\partial z}{\partial x_1}, \ldots, \frac{\partial z}{\partial x_n}\right) = 0.
$$

Lie se familiarise au cours de ses recherches sur ces questions avec le maniement des parenthèses de Poisson

$$
\text{(3)} \quad (f, g) = \sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \frac{\partial g}{\partial p_i} - \frac{\partial g}{\partial x_i} \frac{\partial f}{\partial p_i} \right)
$$

et des crochets \* $[X, Y] = XY - YX$ d’opérateurs différentiels du type (1); il interprète la parenthèse de Poisson (3) comme l’effet sur $f$ d’une transformation de type (1) associée à $g$, et observe à cette occasion que l’identité de Jacobi pour les parenthèses de Poisson signifie que le crochet des opérateurs différentiels correspondant à $g$ et $h$ est associé à la parenthèse $(g, h)$. La recherche de fonctions $g$ telles que $(F, g) = 0$, qui intervient dans la méthode de Jacobi pour intégrer l’équation aux dérivées partielles (2), devient pour Lie celle d’une transformation infinitésimale de contact laissant invariante l’équation donnée. Enfin, Lie est amené à étudier des ensembles de fonctions $(u_j)_{1 \leq j \leq m}$ des $x_i$ et des $p_i$ tels que les parenthèses $(u_j, u_k)$ soient fonctions des $u_h$, et nomme « groupes » ces ensembles (déjà considérés en substance par Jacobi).

\* Ceux-ci intervenaient déjà dans la théorie de Jacobi-Clebsch des « systèmes complets » d’équations aux dérivées partielles du premier ordre $X_j f = 0$ ($1 \leq j \leq r$), notion équivalente à celle de « système complètement intégrable » de Frobenius : le théorème fondamental (équivalent au « théorème de Frobenius ») qui caractérise ces systèmes est que les crochets $[X_i, X_j]$ doivent être des combinaisons linéaires (à coefficients variables) des $X_k$.

II. GROUPES CONTINUS
ET TRANSFORMATIONS INFINITÉSIMALES

Brusquement, à l’automne 1873, Lie reprend l’étude des groupes de transformations et obtient des résultats décisifs. Pour autant qu’on puisse suivre le cheminement de sa pensée dans quelques lettres à A. Mayer des années 1873-1874 ([202], vol. 5, p. 584-608), il part d’un « groupe continu » de transformations sur $n$ variables

$$
x_i' = f_i(x_1, \ldots, x_n, a_1, \ldots, a_r) \quad (1 \leq i \leq n)
$$

dépendant effectivement \* de $r$ paramètres $a_1, \ldots, a_r$; il observe que, si la transformation (4) est l’identité pour les valeurs $a_1^0, \ldots, a_r^0$ des paramètres **, alors les développements de Taylor des $x_i$, limités au premier ordre :

$$
f_i(x_1, \ldots, x_n, a_1^0 + z_1, \ldots, a_r^0 + z_r) =
x_i + \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) + \ldots \quad (1 \leq i \leq n)
$$

donnent une transformation infiniment petite « générique » dépendant linéairement des $r$ paramètres $z_j$

$$
dx_i = \left( \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) \right) dt \quad (1 \leq i \leq n).
$$

Procédant comme dans son mémoire avec Klein, Lie intègre le système différentiel

$$
\frac{d\xi_1}{\sum_k z_k X_{k1}(\xi_1, \ldots, \xi_n)} = \ldots = \frac{d\xi_n}{\sum_k z_k X_{kn}(\xi_1, \ldots, \xi_n)} = dt,
$$

ce qui lui donne, pour tout point $(z_1, \ldots, z_r)$, un groupe à un paramètre

$$
t \mapsto x_i' = g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, t) \quad (1 \leq i \leq n)
$$

\* Lie entend par là que les $f_i$ ne peuvent s’exprimer à l’aide de moins de $r$ fonctions des $a_j$, ou encore que la matrice jacobienne $(\partial f_i / \partial a_j)$ est de rang $r$ « en général ».
** Dans ses premières notes, Lie pense pouvoir démontrer $a$ priori l’existence de l’identité et de l’inverse dans tout ensemble de transformations (4) stable par composition; il reconnaît plus tard que sa démonstration était incorrecte, et Engel lui fournit un contre-exemple reproduit dans ([203], t. 1, § 44). Toutefois, Lie montre comment on ramène les systèmes « continus » (4) stables par composition aux groupuscules de transformations : un tel système est de la forme $G \circ h$, où $G$ est un groupuscule de transformations et $h$ une transformation du système ([203], t. 1, th. 26, p. 163 et t. 3, th. 46, p. 572).

tel que $g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, 0) = x_i$ pour tout $i$. Il montre de façon ingénieuse, en utilisant le fait que les transformations (4) forment un ensemble stable par composition, que le groupe à un paramètre (8) est un sous-groupe du groupe donné ([202], vol. 5, Abh. VII, p. 32-63). L’idée nouvelle, clé de toute la théorie, est de pousser jusqu’au second ordre les développements de Taylor des fonctions (4). La marche de son raisonnement est assez confuse et heuristique ([202], vol. 5, Abh. VII, p. 32-63 et [202], vol. 5, p. 600-601); on peut la présenter de la façon suivante. Pour les $z_j$ assez petits, on peut faire $t = 1$ dans (8), et on obtient ainsi de nouveaux paramètre $z_1, \ldots, z_r$ pour les transformations du groupe (c’est en fait la première apparition des « paramètres canoniques »). On a par définition, vu (7)

$$
\frac{\partial g_i}{\partial t} = \sum_k z_k X_{ki}(x'_1, \ldots, x'_n),
$$

d’où

$$
\frac{\partial^2 g_i}{\partial t^2} = \sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x'_1, \ldots, x'_n) \frac{\partial x'_j}{\partial t}
$$
$$
= \sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x'_1, \ldots, x'_n) \left( \sum_h z_h X_{hj}(x'_1, \ldots, x'_n) \right)
$$

ce qui donne

$$
x'_i = x_i + \left( \sum_k z_k X_{ki}(x_1, \ldots, x_n) \right)t
$$
$$
+ \frac{1}{2} \left( \sum_{k,h,j} z_k z_h \frac{\partial X_{ki}}{\partial x_j}(x_1, \ldots, x_n) X_{hj}(x_1, \ldots, x_n) \right) t^2 + \ldots,
$$

d’où, pour $t = 1$, les développements de Taylor par rapport aux paramètres $z_j$

(9) $x'_i = x_i + \left( \sum_k z_k X_{ki} \right) + \frac{1}{2} \left( \sum_{k,h,j} z_k z_h X_{hj} \frac{\partial X_{ki}}{\partial x_j} \right) + \ldots$

$$(1 \leqslant i \leqslant n).$$

Écrivons en abrégé ces relations $x' = G(x, z)$ entre vecteurs

$$
x = (x_1, \ldots, x_n), \quad x' = (x'_1, \ldots, x'_n), \quad z = (z_1, \ldots, z_r);
$$

la propriété fondamentale de stabilité de l’ensemble de ces transformations par composition s’écrit

(10) $G(G(x, u), v) = G(x, H(u, v))$ où $H = (H_1, \ldots, H_r)$ est indépendant de $x$; il est immédiat que $H(u, 0) = u,\ H(0, v) = v$, d’où les développements

$$
\text{(11)} \quad H_i(u, v) = u_i + v_i + \frac{1}{2} \sum_{h,k} c_{i kh} u_h v_k + \ldots,
$$

les termes non écrits étant non linéaires en $u$ ou en $v$. Transformant (10) à l’aide de (9) et (11), puis comparant les termes en $u_h v_k$ des deux membres, Lie obtient les relations

$$
\text{(12)} \quad \sum_{j=1}^n \left( X_{hj} \frac{\partial X_{ki}}{\partial x_j} - X_{kj} \frac{\partial X_{hi}}{\partial x_j} \right) = \sum_{l=1}^r c_{lhk} X_{li}
$$
$$
(1 \leq h, k \leq r, 1 \leq i \leq n).
$$

Sa pratique de la théorie des équations aux dérivées partielles l’amène à écrire ces conditions sous une forme plus simple : suivant le modèle de (1), il associe à chacune des $r$ transformations infiniment petites obtenues en faisant $z_k = 1,\ z_h = 0$ pour $h \neq k$ dans (6), l’opérateur différentiel

$$
\text{(13)} \quad A_k(f) = \sum_{i=1}^n X_{ki} \frac{\partial f}{\partial x_i},
$$

et récrit les conditions (12) sous la forme

$$
\text{(14)} \quad [A_h, A_k] = \sum_l c_{lhk} A_l,
$$

pierre angulaire de sa théorie. Jusque-là, il avait utilisé indifféremment les termes « transformation infiniment petite » et « transformation infinitésimale » (*e.g.* [202], vol. 5, Abh. I, p. 1-4); la simplicité des relations (14) le conduit à appeler l’opérateur (13) le « symbole » de la transformation infinitésimale $dx_i = X_{ki} dt$ ($1 \leq i \leq n$) ([202], vol. 5, Abh. III, p. 42-75) et très rapidement, c’est l’opérateur (13) lui-même qu’il appellera « *transformation infinitésimale* » ([202], vol. 5, Abh. III, p. 42-75 et [202], vol. 5, p. 589).

Il devient alors conscient des liens étroits qui unissent la théorie des « groupes continus » à ses recherches antérieures sur les transformations de contact et les équations aux dérivées partielles. Ce rapprochement le remplit d’enthousiasme : « *Mes anciens travaux étaient pour ainsi dire tout prêts d’avance pour fonder la nouvelle théorie des groupes de transformations* » écrit-il à Mayer en 1874 ([202], vol. 5, p. 586).

Dans les années suivantes, Lie poursuit l’étude des groupes de transformations. Outre les théorèmes généraux résumés ci-après

§ III), il obtient un certain nombre de résultats plus particuliers : détermination des groupes de transformations de la droite et du plan, des sous-groupes de petite codimension des groupes projectifs, des groupes à au plus 6 paramètres, etc. Il n’abandonne pas pour autant les équations différentielles. En fait, il semble même que, pour lui, la théorie des groupes de transformations devait être un instrument pour intégrer les équations différentielles, où le groupe de transformations jouerait un rôle analogue à celui du groupe de Galois d’une équation algébrique *. Notons que ces recherches l’amènent également à introduire certains ensembles de transformations à une infinité de paramètres, qu’il appelle « groupes infinis et continus » **; il réserve le nom de « groupes finis et continus » aux groupes de transformation à un nombre fini de paramètres du type (4) ci-dessus.

III. LE « DICTIONNAIRE » GROUPES DE .LIE-ALGÈBRES DE LIE

La théorie des groupes « finis et continus », développée par Lie dans de nombreux mémoires à partir de 1874, est exposée systématiquement dans l’imposant traité « Theorie der Transformationsgruppen » ([203], 1888-1893), écrit en collaboration avec F. Engel *** ; elle y fait l’objet du premier volume et des cinq derniers chapitres du troisième, le second étant consacré aux transformations de contact.

Comme l’indique le titre, il n’est jamais question dans cet ouvrage que de groupes de transformations, au sens des équations (4), où l’espace des « variables » $x_i$ et l’espace des « paramètres » $a_j$ jouent

\* Ces recherches n’ont eu que peu d’influence sur la théorie générale des équations différentielles, le groupe d’automorphismes d’une telle équation étant le plus souvent trivial. En revanche, pour certains types d’équations (par exemple linéaires), des résultats intéressants ont été obtenus ultérieurement par Picard, Vessiot, puis, plus récemment, Ritt et Kolchin.
** On les appelle aujourd’hui « pseudo-groupes de Lie »; on aura soin de ne pas les confondre avec les groupes de Lie « banachiques ».
*** De 1886 à 1898, Lie occupa à Leipzig la chaire laissée vacante par Klein et eut Engel pour assistant; cette circonstance favorisa l’éclosion d’une active école mathématique ainsi que la diffusion des idées de Lie, assez peu connues jusque-là (en raison, notamment, du fait que ses premiers mémoires étaient le plus souvent écrits en norvégien, et publiés dans les Comptes Rendus de l’Académie de Christiania, peu répandus ailleurs). C’est ainsi qu’à une époque où il n’était guère d’usage pour les jeunes mathématiciens français d’aller s’instruire en Allemagne, E. Vessiot et A. Tresse passèrent une année d’études à Leipzig, avec Sophus Lie.

des rôles initialement aussi importants. D’ailleurs le concept de groupe « abstrait » n’est pas clairement dégagé à cette époque ; quand en 1883 ([202], vol. 5, Abh. XII, p. 311-313) Lie remarque qu’avec les notations de (10), l’équation $w = H(u, v)$ qui donne les paramètres de la composée de deux transformations du groupe définit un nouveau groupe, c’est comme groupe de transformations sur l’espace des paramètres qu’il le considère, obtenant ainsi ce qu’il appelle le « groupe des paramètres » (il en obtient même deux, qui ne sont autres que le groupe des translations à gauche et le groupe des translations à droite) *.

Les variables $x_i$ et les paramètres $a_j$ dans les équations (4) sont en principe supposés complexes (sauf dans les chap. XIX-XXIV du t. 3), et les fonctions $f_i$ analytiques ; Lie et Engel sont bien entendu conscients du fait que ces fonctions ne sont pas en général définies pour toutes les valeurs complexes des $x_i$ et des $a_j$ et que, par suite, la composition de telles transformations soulève de sérieuses difficultés ([203], t. 1, p. 15-17, p. 33-40 et passim); et bien que, par la suite, ils s’expriment presque toujours comme si la composition des transformations qu’ils étudient était possible sans restriction, ce n’est sans doute que pour la commodité des énoncés, et ils rétablissent explicitement le point de vue « local » chaque fois que c’est nécessaire (cf. loc. cit., p. 168 ou 189 par exemple ou ibid., t. 3, p. 2, note de bas de page); en d’autres termes, l’objet mathématique qu’ils étudient est voisin de ce que nous appelons maintenant un morceau de loi d’opération. Ils ne se font pas faute, à l’occasion, de considérer des groupes globaux, par exemple les 4 séries de groupes classiques ([203], t. 3, p. 682), mais ne paraissent pas s’être posé la question de ce que peut être en général un « groupe global »; il leur suffit de pouvoir obtenir, pour les « paramètres » des groupes classiques (les « variables » de ces groupes n’introduisent aucune difficulté, puisqu’il s’agit de transformations linéaires de $\mathbf{C}^n$), des systèmes de paramètres « locaux » au voisinage de la transformation identique, sans qu’ils s’inquiètent du domaine de validité des formules qu’ils écrivent. Ils se posent toutefois un problème qui sort nettement de la théorie locale ** : l’étude des groupes « mixtes », c’est-à-dire des groupes ayant un

\* La notion analogue pour les groupes de permutations avait été introduite et étudiée par Jordan dans son « Traité ».
** Rappelons (p. 151), qu’à la suite d’une Note de H. Poincaré([251], t. V, p. 77-79) divers auteurs ont étudié le groupe des éléments inversibles d’une algèbre associative de dimension finie. Il est intéressant de noter à ce propos que E. Study, dans ses travaux sur ce sujet, introduit un symbolisme qui revient en substance à envisager le groupe abstrait défini par le groupe des paramètres.

nombre fini de composantes connexes, tel le groupe orthogonal ([203], t. 1, p. 7). Ils présentent cette étude comme celle d’un ensemble de transformations stable par composition et passage à l’inverse, qui est réunion d’ensembles $H_j$ dont chacun est décrit par des systèmes de fonctions $(f_i^{(j)})$ comme dans (4); le nombre de paramètres (essentiels) de chaque $H_j$ est même $a$ priori supposé dépendre de $j$, mais ils montrent qu’en fait ce nombre est le même pour tous les $H_j$. Leur résultat principal est alors l’existence d’un groupe fini et continu $G$ tel que $H_j = G \circ h_j$ pour un $h_j \in H_j$ et pour tout $j$; ils établissent aussi que $G$ est distingué dans le groupe mixte et remarquent que la détermination des invariants de ce dernier se ramène à celle des invariants de $G$ et d’un groupe discontinu ([203], t. 1, chap. 18).

La théorie générale développée dans [203] aboutit (sans que cela soit dit de façon très systématique par les auteurs) à forger un « dictionnaire » faisant passer des propriétés des groupes « finis et continus » à celles de l’ensemble de leurs transformations infinitésimales. Il est basé sur les « trois théorèmes de Lie », dont chacun est formé d’une assertion et de sa réciproque.

Le premier théorème ([203], t. 1, p. 33 et 72 et t. 3, p. 563) affirme en premier lieu que si dans (4) les paramètres sont effectifs, les fonctions $f_i$ vérifient un système d’équations aux dérivées partielles de la forme

$$
\frac{\partial f_i}{\partial a_j} = \sum_{k=1}^r \xi_{ki}(f(x, a)) \psi_{kj}(a) \quad (1 \leq i \leq n)
$$

où la matrice $(\xi_{ki})$ est de rang maximum et $\det(\psi_{kj}) \neq 0$; réciproquement, si les fonctions $f_i$ ont cette propriété, les formules (4) définissent un groupuscule de transformations.

Le deuxième théorème ([203], t. 1, p. 149 et 158, et t. 3, p. 590) donne des relations entre les $\xi_{ki}$ d’une part, les $\psi_{lj}$ de l’autre : les conditions sur les $\xi_{kl}$ s’écrivent sous la forme

$$
\sum_{k=1}^n \left( \xi_{ik} \frac{\partial \xi_{jl}}{\partial x_k} - \xi_{jk} \frac{\partial \xi_{il}}{\partial x_k} \right) = \sum_{k=1}^r c_{ij}^k \xi_{kl}
$$
$$
(1 \leq i, j \leq r, 1 \leq l \leq n)
$$

où les $c_{ij}^k$ sont des constantes $(1 \leq i, j, k \leq r)$ antisymétriques en $i, j$. Les conditions sur les $\psi_{lj}$, sous la forme donnée par Maurer, sont :

$$
\frac{\partial \psi_{kl}}{\partial a_m} - \frac{\partial \psi_{km}}{\partial a_l} = \frac{1}{2} \sum_{1 \leq i, j \leq r} c_{ij}^k (\psi_{li} \psi_{jm} - \psi_{ji} \psi_{im})
$$
$$
(1 \leq k, l, m \leq r).
$$

En introduisant la matrice $(\alpha_{ij})$ contragrédiente de $(\psi_{ij})$ et les transformations infinitésimales

(18) $$
X_k = \sum_{i=1}^n \xi_{ki} \frac{\partial}{\partial x_i}, \quad A_k = \sum_{j=1}^r \alpha_{kj} \frac{\partial}{\partial a_j} \quad (1 \leq k \leq r),
$$

on peut écrire (16) et (17) respectivement :

(19) $$
[X_i, X_j] = \sum_{k=1}^r c_{ij}^k X_k $$
$$(1 \leq i, j \leq r).$$

(20) $$
[A_i, A_j] = \sum_{k=1}^r c_{ij}^k A_k.
$$

Réciproquement, si l’on se donne $r$ transformations infinitésimales $X_k$ $(1 \leq k \leq r)$ linéairement indépendantes et vérifiant les conditions (19), les sous-groupes à un paramètre engendrés par ces transformations engendrent un groupe de transformations à $r$ paramètres essentiels.

Enfin, le troisième théorème ([203], t. 1, p. 170 et 297 et t. 3, p. 597) ramène la détermination des systèmes de transformations infinitésimales $(X_k)_{1 \leq k \leq r}$ vérifiant (29) à un problème purement algébrique : on doit avoir

(21) $$
c_{ij}^k + c_{ji}^k = 0
$$

(22) $$
\sum_{l=1}^r (c_{il}^m c_{jk}^l + c_{kl}^m c_{ij}^l + c_{jl}^m c_{kl}^l) = 0 \quad (1 \leq i, j, k, m \leq r).
$$

Réciproquement *, si (21) et (22) sont vérifiées, il existe un système de transformations infinitésimales satisfaisant aux relations (19), d’où un groupe de transformations à $r$ paramètres (en d’autres termes, les combinaisons linéaires à coefficients constants des $X_k$ forment une algèbre de Lie, et inversement toute algèbre de Lie de dimension finie peut être obtenue de cette manière).

Ces résultats sont complétés par l’étude des questions d’iso-

\* Cette réciproque n’a pas été obtenue sans peine. La première démonstration qu’en donne Lie ([202], vol. 5, Abh. III, p. 42-75) consiste à passer au groupe adjoint et n’est en fait valable que si le centre de l’algèbre de Lie donnée est réduit à 0: Il en donne ensuite deux démonstrations générales ([203], t. 2, chap. XVII et t. 3, p. 599-604); il est assez significatif que la première soit basée sur les transformations de contact et que Lie la trouve plus naturelle que la deuxième.

morphisme. Deux groupes de transformations sont dits semblables si l’on passe de l’un à l’autre par une transformation inversible de coordonnées sur les variables et une transformation inversible de coordonnées sur les paramètres : dès le début de ses recherches, Lie avait rencontré naturellement cette notion à propos de la définition des « paramètres canoniques ». Il montre que deux groupes sont semblables si, par une transformation sur les « variables », on peut amener les transformations infinitésimales de l’un sur celles de l’autre ([203], t. 1, p. 329). Une condition nécessaire pour qu’il en soit ainsi est que les algèbres de Lie des deux groupes soient isomorphes, ce que Lie exprime en disant que les groupes sont « gleichzusammengesetzt »; mais cette condition n’est pas suffisante, et tout un chapitre ([203], t. 1, chap. 19) est consacré à obtenir des conditions supplémentaires assurant que les groupes sont « semblables ». La théorie des groupes de permutations fournissait d’autre part la notion d’« isomorphisme holoédrique » de deux tels groupes (isomorphisme des groupes « abstraits » sous-jacents); Lie transpose cette notion aux groupes de transformations, et montre que deux tels groupes sont « holoédriquement isomorphes » si et seulement si leurs algèbres de Lie sont isomorphes ([203], t. 1, p. 418). En particulier, tout groupe de transformations est holoédriquement isomorphe à chacun de ses groupes de paramètres, et cela montre que, lorsqu’on veut étudier la structure du groupe, les « variables » sur lesquelles il opère importent peu et qu’en fait tout se ramène à l’algèbre de Lie *.

Toujours par analogie avec la théorie des groupes de permutations, Lie introduit les notions de sous-groupes, sous-groupes distingués, « isomorphismes mériédriques » (homomorphismes surjectifs), et montre qu’elles correspondent à celles de sous-algèbres, idéaux et homomorphismes surjectifs d’algèbres de Lie; il avait d’ailleurs rencontré très tôt un exemple particulièrement important d’« isomorphisme mériédrique », la représentation adjointe, et reconnu ses liens avec le centre du groupe ([202], vol. 5, Abh. III, p. 42-75). Pour ces résultats, comme pour les théorèmes fondamentaux, l’outil essentiel est le théorème de Jacobi-Clebsch donnant

\* On peut constater une évolution semblable dans la théorie des groupes « abstraits », en particulier finis. Ils ont été tout d’abord définis comme groupes de transformations, mais déjà Cayley remarquait que l’essentiel est la manière dont les transformations se composent entre elles, et non la nature de la représentation concrète du groupe de permutations d’objets particuliers.

la complète intégrabilité d’un système différentiel (l’une des formes du théorème dit « de Frobenius »); il en donne du reste une démonstration nouvelle utilisant les groupes à un paramètre ([203], t. 1, chap. 6).

Les notions de transitivité et de primitivité, si importantes pour les groupes de permutations, se présentaient aussi naturellement pour les groupes « finis et continus » de transformations, et le traité de Lie-Engel en fait une étude détaillée ([203], t. 1, chap. 13 et passim); les relations avec les sous-groupes stabilisateurs d’un point et la notion d’espace homogène sont aperçues (pour autant qu’elles pouvaient l’être sans se placer au point de vue global) ([203], t. 1, p. 425).

Enfin, le « dictionnaire » se complète, dans [203], par l’introduction des notions de groupe dérivé et de groupe résoluble (appelé « groupe intégrable » par Lie; cette terminologie, suggérée par la théorie des équations différentielles, restera en usage jusqu’aux travaux de H. Weyl) ([203], t. 1, p. 261 et t. 3, p. 678-679); la relation entre commutateurs et crochets avait d’ailleurs été perçue par Lie dès 1883 ([202], vol. 5, p. 358).

Autres démonstrations des théorèmes fondamentaux

Dans [278 b], F. Schur montre qu’en coordonnées canoniques les $\psi_{i k}$ de (15) satisfont aux équations différentielles

$$
\frac{d}{dt}(t \psi_{i k}(t a)) = \delta_{i k} + \sum_{j, l} c_{j l}^k t a_l \psi_{j l}(t a).
$$

Celles-ci s’intègrent et donnent une formule équivalente à la formule

$$
\varpi(X) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\operatorname{ad}(X))^n
$$

pour la différentielle droite $\varpi(X)$ de l’application exponentielle au point $X$; en particulier, en coordonnées canoniques, les $\psi_{i j}$ se prolongent en fonctions entières des $a_k$. F. Schur en déduit un résultat précisant une remarque antérieure de Lie : si, dans la définition (4) des groupes de transformations, on suppose seulement que les $f_i$ sont de classe $C^2$, alors le groupe est holoédriquement isomorphe à un groupe analytique *. A la suite de ses recherches sur l’intégration des systèmes différentiels, E. Cartan ([52 a], t. II2, p. 371) introduit en 1904 les formes de Pfaff

(25)
$$
\omega_k = \sum_{i=1}^r \psi_{ki} da_i \quad (1 \leq i \leq r)
$$
(avec les notations de (15)), appelées plus tard formes de Maurer-Cartan. Les conditions (17) de Maurer peuvent alors s’écrire
$$
d\omega_k = -\frac{1}{2} \sum_{i,j} c_{ij}^k \omega_i \wedge \omega_j;
$$
E. Cartan montre que l’on peut développer la théorie des groupes finis et continus à partir des $\omega_k$ et établit l’équivalence de ce point de vue et de celui de Lie. Mais, pour lui, l’intérêt de cette méthode est surtout qu’elle s’adapte aux « groupes infinis et continus » dont il pousse la théorie beaucoup plus loin que ne l’avait fait Lie, et qu’elle permet d’édifier sa théorie du « repère mobile » généralisé.

IV. LA THÉORIE DES ALGÈBRES DE LIE

Une fois acquise la correspondance entre groupes de transformations et algèbres de Lie, la théorie va prendre un tour nettement plus algébrique et sera centrée sur une étude approfondie des algèbres de Lie **

\* Lie avait déjà énoncé sans démonstration un résultat de ce genre ([202], vol. 6, Abh. V, p. 230-236). Il y avait été amené par ses recherches sur les fondements de la géométrie (« problème de Helmholtz »), où il avait remarqué que les hypothèses d’analyticité ne sont pas naturelles.

Le résultat de F. Schur devait amener Hilbert, en 1900, à demander si la même conclusion restait valable si l’on suppose seulement les $f_i$ continues (« 5e problème de Hilbert »). Ce problème a suscité de nombreuses recherches. Le résultat le plus complet dans cet ordre d’idées est le théorème suivant, démontré par A. Gleason, D. Montgomery et L. Zippin : tout groupe topologique localement compact possède un sous-groupe ouvert qui est limite projective de groupes de Lie; il entraîne que tout groupe localement euclidien est un groupe de Lie. Pour plus de détails sur cette question, cf. [226].

** Le terme « algèbre de Lie » a été introduit par H. Weyl en 1934 : dans ses travaux de 1925, il avait utilisé l’expression « groupe infinitésimal ». Auparavant, on parle simplement des « transformations infinitésimales $X_1 f, \ldots, X_r f$ » du groupe, ce que Lie et Engel abrègent fréquemment en disant « le groupe $X_1 f, \ldots, X_r f$ »!

Une première et courte période, de 1888 à 1894, marquée par les travaux d’Engel, de son élève Umlauf et surtout de Killing et E. Cartan, aboutit à une série de résultats spectaculaires sur les algèbres de Lie complexes. Nous avons vu plus haut que la notion d’algèbre de Lie résoluble était due à Lie lui-même, qui avait démontré (dans le cas complexe) le théorème de réduction des algèbres de Lie linéaires résolubles à la forme triangulaire ([203], t. 1, p. 270) *. Killing observe [180] qu’il existe dans une algèbre de Lie un plus grand idéal résoluble (qu’on appelle aujourd’hui le radical), et que le quotient de l’algèbre de Lie par son radical a un radical nul; il appelle semi-simples les algèbres de Lie de radical nul, et prouve que ce sont des produits d’algèbres simples (cette dernière notion avait déjà été introduite par Lie, qui avait prouvé la simplicité des algèbres de Lie « classiques » ([203], t. 3, p. 682)).

D’autre part, Killing introduit, dans une algèbre de Lie, l’équation caractéristique det(ad(x) — ω.l) = 0, déjà rencontrée par Lie en étudiant les sous-algèbres de Lie de dimension 2 contenant un élément donné d’une algèbre de Lie. Nous renvoyons à d’autres Notes historiques pour l’analyse des méthodes par lesquelles Killing, en étudiant de manière pénétrante les propriétés des racines de l’équation caractéristique « générique » pour une algèbre semi-simple, aboutit au plus remarquable de ses résultats, la détermination complète des algèbres de Lie simples (complexes)**.

Killing prouve que l’algèbre dérivée d’un algèbre résoluble est « de rang 0 » (ce qui signifie que ad x est nilpotent pour tout élément x de l’algèbre). Peu de temps après, Engel démontre que les algèbres « de rang 0 » sont résolubles (cet énoncé est en substance ce que l’on appelle aujourd’hui le théorème d’Engel). Dans sa thèse, E. Cartan introduit d’autre part ce qu’on appelle maintenant la « forme de Killing », et établit les deux critères fondamentaux qui caractérisent au moyen de cette forme les algèbres de Lie résolubles et les algèbres de Lie semi-simples.

Killing avait affirmé ([180], IV) que l’algèbre dérivée d’une

\* Presque au début de ses recherches, Lie avait rencontré des groupes linéaires résolubles, et même en fait nilpotents ([202], vol. 5, Abh IV, p. 78-133).
** A cela près qu’il trouve deux algèbres exceptionnelles de dimension 52, dont il ne remarque pas l’isomorphisme. (Il s’agit uniquement d’algèbres de Lie simples complexes, car on n’envisageait pas de problème plus général à cette époque; les méthodes de Killing valent en fait pour tout corps algébriquement clos de caractéristique 0).

algèbre de Lie est somme d'une algèbre semi-simple et de son radical, qui est nilpotent, mais sa démonstration était incomplète. Un peu plus tard, E. Cartan annonçait sans démonstration ([52 a], t. I₁, p. 104) que plus généralement toute algèbre de Lie est somme de son radical et d'une sous-algèbre semi-simple; le seul résultat dans cette direction établi de façon indiscutable à cette époque est un théorème d'Engel affirmant l'existence, dans toute algèbre de Lie non résoluble, d'une sous-algèbre de Lie simple de dimension 3. La première démonstration publiée (pour les algèbres de Lie complexes) de l'énoncé de Cartan est due à E. E. Levi [200]; une autre démonstration (valable également dans le cas réel) fut donnée par J. H. C. Whitehead en 1936 [334 a]. En 1942, A. Malcev compléta ce résultat par le théorème d'unicité des « sections de Levi » à conjugaison près.

Dès ses premiers travaux, Lie s'était posé le problème de l'isomorphisme de toute algèbre de Lie avec une algèbre de Lie linéaire. Il avait cru le résoudre affirmativement en considérant la représentation adjointe (et en déduire ainsi une preuve de son « troisième théorème ») ([202], vol. 5, Abh. III, p. 42-75); il reconnut rapidement que sa démonstration n'était correcte que pour les algèbres de Lie de centre nul; après lui, la question resta très longtemps ouverte, et fut résolue affirmativement par Ado en 1935 [2 a]. D'autre part, Lie s'était posé en substance le problème de déterminer les représentations linéaires de dimension minimale des algèbres de Lie simples, et l'avait résolu pour les algèbres classiques; dans sa Thèse, Cartan résout aussi ce problème pour les algèbres simples exceptionnelles *; les méthodes qu'il emploie à cet effet seront généralisées par lui vingt ans plus tard pour obtenir toutes les représentations irréductibles des algèbres de Lie simples réelles ou complexes..

La propriété de réductibilité complète d'une représentation linéaire semble avoir été rencontrée pour la première fois (sous une forme géométrique) par Study. Dans un manuscrit non publié, mais cité dans ([203], t. 3, p. 785-788) il démontre cette propriété pour les représentations linéaires de l'algèbre de Lie de $\mathbf{SL}(2, \mathbf{C})$, et obtient des résultats partiels pour $\mathbf{SL}(3, \mathbf{C})$ et $\mathbf{SL}(4, \mathbf{C})$. Lie et Engel conjecturent à cette occasion que le théorème de réductibilité complète

\* Le point de vue de Cartan consiste à étudier les algèbres de Lie extensions non triviales d'une algèbre de Lie simple et d'un radical (commutatif) de dimension minimale.

vaut pour $\mathbf{SL}(n, \mathbf{C})$ quel que soit $n$. La réductibilité complète des représentations linéaires des algèbres de Lie semi-simples fut établie par H. Weyl en 1925 \* par un argument de nature globale (voir plus loin). La première démonstration algébrique a été obtenue en 1935 par Casimir et van der Waerden [55]; d'autres démonstrations algébriques ont été données ensuite par R. Brauer [34 b] et J. H. C. Whitehead [334 b].

Enfin, au cours de ses recherches sur l’application exponentielle (cf. infra), H. Poincaré ([251], t. III) considère l’algèbre associative d’opérateurs différentiels de tous ordres, engendrée par les opérateurs d’une algèbre de Lie; il montre en substance que, si $(X_i)_{1 \leq i \leq n}$ est une base de l’algèbre de Lie, l’algèbre associative engendrée par les $X_i$ a pour base certaines fonctions symétriques des $X_i$ (sommes des « monômes » non commutatifs déduits d’un monôme donné par toutes les permutations de facteurs). L’essentiel de sa démonstration est de nature algébrique, et permet d’obtenir la structure de l’algèbre enveloppante. Des démonstrations analogues ont été données en 1937 par G. Birkhoff [22 b] et E. Witt [337 b] **.

La plupart des travaux cités ci-dessus se limitent aux algèbres de Lie réelles ou complexes, qui seules correspondent à des groupes de Lie au sens usuel. L’étude des algèbres de Lie sur un corps autre que $\mathbf{R}$ ou $\mathbf{C}$ est abordée par Jacobson [172 a] qui montre que la plus grande partie des résultats classiques restent valables sur un corps de caractéristique zéro.

V. EXPONENTIELLE ET FORMULE DE HAUSDORFF

Les premières recherches concernant l’application exponentielle sont dues à E. Study et F. Engel; Engel [104 b] remarque que l’exponentielle n’est pas surjective pour $\mathbf{SL}(2, \mathbf{C})$ (par exemple $\begin{pmatrix} -1 & a \\ 0 & -1 \end{pmatrix}$)

\* H. Weyl remarque à cette occasion que la construction donnée par E. Cartan des représentations irréductibles utilise implicitement cette propriété.
** La première utilisation des opérateurs différentiels d’ordre supérieur engendrés par les $X_i$ est sans doute l’emploi de l’« opérateur de Casimir » pour la démonstration du th. de réductibilité complète. Après 1950, les recherches de Gelfand et de son école, et de Harish-Chandra, sur les représentations linéaires de dimension infinie, ont porté ces opérateurs au premier plan.

n’est pas une exponentielle si $a \neq 0$), mais qu’elle l’est pour $\mathbf{GL}(n, \mathbf{C})$, donc aussi pour $\mathbf{PGL}(n, \mathbf{C})$ (cette dernière propriété avait déjà été notée par Study pour $n = 2$); ainsi $\mathbf{SL}(2, \mathbf{C})$ et $\mathbf{PGL}(2, \mathbf{C})$ donnent un exemple de deux groupes localement isomorphes, mais qui sont néanmoins très différents du point de vue global. Engel montre aussi que l’exponentielle est surjective dans les autres groupes classiques, augmentés des homothéties; ces travaux sont repris et poursuivis par Maurer, Study et d’autres, sans apporter de substantielles nouveautés.

En 1899, H. Poincaré ([251], t. III, p. 169-172 et 173-212), aborde l’étude de l’application exponentielle d’un point de vue différent. Ses mémoires paraissent avoir été hâtivement rédigés, car à plusieurs endroits il affirme que tout élément d’un groupe connexe est une exponentielle, alors qu’il donne des exemples du contraire ailleurs. Ses résultats portent principalement sur le groupe adjoint : il montre qu’un élément semi-simple d’un tel groupe G peut être l’exponentielle d’une infinité d’éléments de l’algèbre de Lie L(G), alors qu’un élément non semi-simple peut ne pas être une exponentielle. Si ad(X) n’a pas de valeur propre multiple non nul de $2\pi i$, alors exp est étale en X. Il prouve aussi que, si U et V décrivent des lacets dans L(G), et si l’on définit par continuité W tel que $e^U . e^V = e^W$, on ne retombe pas nécessairement sur la détermination initiale de W. Il utilise une formule de résidus qui revient essentiellement à

$$
\Phi(\mathrm{ad}\ X) = \frac{1}{2\pi i} \int \frac{\Phi(\xi)\ d\xi}{\xi - \mathrm{ad}\ X}
$$

où $\mathrm{ad}(X)$ est un élément semi-simple dont les valeurs propres non nulles sont de multiplicité 1, $\Phi$ une série entière de rayon de convergence suffisamment grand, l’intégrale étant étendue à un lacet enveloppant les valeurs propres de $\mathrm{ad}\ X$; il étudie aussi ce qui se passe lorsque X tend vers une transformation ayant des valeurs propres multiples.

La recherche d’expressions de W en fonction de U et V dans la formule $e^U . e^V = e^W$ avait déjà, peu avant le travail de Poincaré, fait l’objet de deux mémoires de Campbell [46 a et b]. Comme l’écrit un peu plus tard Baker « ...la théorie de Lie suggère de façon évidente que le produit $e^U e^V$ est de la forme $e^W$ où W est une série d’alternants en U et V... ». Les travaux ultérieurs sur ce sujet visent à préciser cette assertion et à donner une formule explicite (ou une méthode de construction) pour W (« formule de Hausdorff »). Après Campbell et Poincaré, Pascal, Baker [13] et Hausdorff [152 a] reviennent sur la question; chacun considère que les démonstrations de ses prédécesseurs ne sont pas convaincantes; la difficulté principale réside dans ce qu’il faut entendre par « alternants » : s’agit-il d’éléments de l’algèbre de Lie particulière que l’on considère, ou d’expressions « symboliques » universelles? Ni Campbell, ni Poincaré, ni Baker ne s’expriment clairement sur ce point. Le mémoire de Hausdorff, par contre, est parfaitement précis; il travaille d’abord dans l’algèbre des séries formelles associatives (non commutatives) en un nombre fini d’indéterminées et considère U, V, W comme des éléments de cette algèbre. Il démontre l’existence de W par un argument d’équation différentielle analogue à celui de ses prédécesseurs. Le même argument lui sert à prouver la convergence de la série lorsqu’on y remplace les indéterminées par des éléments d’une algèbre de Lie de dimension finie. Comme l’avait remarqué Baker, et indépendamment Poincaré, ce résultat peut servir à donner une démonstration du troisième théorème de Lie; il éclaire la correspondance entre groupes et algèbres de Lie, par exemple en ce qui concerne le groupe des commutateurs.

En 1947, Dynkin [98 a] reprend la question, et obtient les coefficients explicites de la formule de Hausdorff, en considérant d’emblée une algèbre de Lie normée (de dimension finie ou non, sur $\mathbf{R}, \mathbf{C}$ ou un corps ultramétrique) \*

VI. REPRÉSENTATIONS LINÉAIRES ET GROUPES DE LIE GLOBAUX

Aucun des travaux dont nous venons de parler n’abordait franchement le problème de la définition et de l’étude des groupes de Lie globaux. C’est à H. Weyl que reviennent les premiers pas dans cette voie. Il s’inspire de deux théories, qui s’étaient jusque-là développées indépendamment : celle des représentations linéaires des algèbres de Lie semi-simples complexes, due à E. Cartan, et celle des représentations linéaires des groupes finis, due à Frobenius et

\* Dans le cas ultramétrique, la méthode classique des majorantes ne peut s’étendre sans précautions, à cause du comportement asymptotique de la valeur absolue $p$-adique de $1/n$ quand $n$ tend vers l’infini.

qui venait d’être transposée au groupe orthogonal par I. Schur, en utilisant une idée de Hurwitz. Ce dernier avait montré [168] comment on peut former des invariants pour le groupe orthogonal ou le groupe unitaire en remplaçant l’opération de moyenne sur un groupe fini par une intégration relativement à une mesure invariante. Il avait aussi remarqué qu’en appliquant cette méthode au groupe unitaire, on obtient des invariants pour le groupe linéaire général, premier exemple du « unitarian trick ». En 1924, I. Schur [279 e] utilise ce procédé pour montrer la complète réductibilité des représentations du groupe orthogonal $\mathbf{O}(n)$ et du groupe unitaire $\mathbf{U}(n)$, par construction d’une forme hermitienne positive non-dégénérée invariante ; il en déduit, par le « unitarian trick », la complète réductibilité des représentations holomorphes de $\mathbf{O}(n, \mathbf{C})$, et de $\mathbf{SL}(n, \mathbf{C})$, établit des relations d’orthogonalité pour les caractères de $\mathbf{O}(n)$ et de $\mathbf{U}(n)$ et détermine les caractères de $\mathbf{O}(n)$. H. Weyl étend aussitôt cette méthode aux algèbres de Lie semi-simples complexes [331 b]. Étant donnée une telle algèbre $g$, il montre qu’elle possède une « forme réelle compacte » (ce qui revient à dire qu’elle provient par extension des scalaires de $\mathbf{R}$ à $\mathbf{C}$ d’une algèbre $g_0$ sur $\mathbf{R}$ dont le groupe adjoint $G_0$ est compact). De plus, il montre que le groupe fondamental de $G_0$ est fini, donc que le revêtement universel \* de $G_0$ est compact. Il en déduit, par une adaptation convenable du procédé de Schur, la réductibilité complète des représentations de $g$, et donne aussi, par voie globale, la détermination des caractères des représentations de $g$. Dans une lettre à I. Schur [331 a], H. Weyl résume les résultats de Cartan, que Schur ne connaissait pas (cf. [279 e], p. 299, note de bas de page) et compare les deux points de vue : la méthode de Cartan fournit toutes les représentations holomorphes du groupe simplement connexe d’algèbre de Lie $g$; dans le cas du groupe orthogonal, on obtient ainsi des représentations d’un revêtement à deux feuillets (appelé plus tard le groupe des spineurs), qui échappent à Schur ; d’un autre côté, la méthode de Schur a l’avantage de démontrer la complète réductibilité et de donner explicitement les caractères.

Après les travaux de H. Weyl, E. Cartan adopte un point de vue

\* H. Weyl ne définit pas explicitement cette notion, avec laquelle il était familier depuis la rédaction de son cours sur les surfaces de Riemann (1913). C’est O. Schreier [276 a et b] qui, en 1926-1927, donne, pour la première fois, la définition d’un groupe topologique et celle d’un groupe « continu » (i.e. localement homéomorphe à un espace euclidien), ainsi que la construction du revêtement universel d’un tel groupe.

franchement global dans ses recherches sur les espaces symétriques et les groupes de Lie. C’est ce point de vue qui est à la base de son exposé de 1930 ([52 a], t. I₂, p. 1165-1225) de la théorie des groupes « finis et continus ». On y trouve en particulier la première démonstration de la variante globale du troisième théorème fondamental (existence d’un groupe de Lie d’algèbre de Lie donnée); Cartan montre aussi que tout sous-groupe fermé d’un groupe de Lie réel est un groupe de Lie, ce qui généralise un résultat de J. von Neumann sur les sous-groupes fermés du groupe linéaire [324 b]. Dans ce Mémoire, von Neumann montrait aussi que toute représentation continue d’un groupe semi-simple complexe est analytique réelle.

Après ces travaux, la théorie des groupes de Lie au sens « classique » (c’est-à-dire de dimension finie sur $\mathbf{R}$ ou $\mathbf{C}$) est à peu près fixée dans ses grandes lignes. Le premier exposé détaillé en est donné par Pontrjagin dans son livre sur les groupes topologiques [253]; il y garde un point de vue encore assez proche de celui de Lie, mais en distinguant soigneusement le local du global. Il est suivi par le livre de Chevalley [62 d] qui renferme aussi la première discussion systématique de la théorie des variétés analytiques et du calcul différentiel extérieur; les « transformations infinitésimales » de Lie y apparaissent comme des champs de vecteurs et l’algèbre de Lie d’un groupe de Lie G est identifiée à l’espace des champs de vecteurs invariants à gauche sur G. Il laisse de côté l’aspect « groupuscules » et l’aspect « groupes de transformations ».

VII. EXTENSIONS DE LA NOTION DE GROUPE DE LIE

De nos jours, la vitalité de la théorie de Lie se manifeste par la diversité de ses applications (en topologie, géométrie différentielle, arithmétique, etc.), ainsi que par la création de théories parallèles où la structure de variété différentielle sous-jacente est remplacée par une structure voisine (variété $p$-adique, algébrique, schéma, schéma formel, ...). Nous n’avons pas à faire ici l’historique de tous ces développements, et nous nous bornerons à deux d’entre eux : groupes de Lie banachiques et groupes de Lie $p$-adiques.

a) Groupes de Lie banachiques

Il s’agit de groupes de Lie « de dimension infinie ». Du point de vue local, on remplace un voisinage de 0 dans un espace euclidien par un voisinage de 0 dans un espace de Banach. C’est ce que fait G. Birkhoff en 1936 [22 a], aboutissant ainsi à la notion d’algèbre de Lie normée complète et à sa correspondance avec un « grou-puscule » défini sur un ouvert d’un espace de Banach. Vers 1950, Dynkin complète ces résultats par une extension à ce cas de la formule de Hausdorff (cf. supra).

Les définitions et résultats de Birkhoff et Dynkin sont locaux. Jusqu’à une date récente, il ne semble pas que l’on ait cherché à expliciter la théorie globale correspondante, sans doute faute d’applications,

b) Groupes de Lie p-adiques

De tels groupes se rencontrent pour la première fois en 1907 dans les travaux de Hensel [157 e] sur les fonctions analytiques p-adiques (définies par des développements en séries entières). Celui-ci étudie notamment l’exponentielle et le logarithme; malgré le comportement a priori surprenant des séries qui les définissent (par exemple la série exponentielle ne converge pas partout), leurs propriétés fonctionnelles fondamentales restent valables, ce qui fournit un isomorphisme local entre le groupe additif et le groupe multiplicatif de $\mathbf{Q}_p$ (ou, plus généralement, de tout corps ultramétrique complet de caractéristique zéro).

C’est également de groupes commutatifs (mais non linéaires cette fois) qu’il s’agit dans les travaux de A. Weil [330 a] et E. Lutz [21C; sur les courbes elliptiques p-adiques (1936). Outre des applications arithmétiques, on y trouve la construction d’un isomorphisme local du groupe avec le groupe additif, basé sur l’intégration d’une forme différentielle invariante. Cette méthode s’applique également aux variétés abéliennes, comme le remarque peu après C. Chabauty qui l’utilise sans plus d’explication pour démontrer un cas particulier de la « conjecture de Mordell » [61].

Dès ce moment, il était clair que la théorie locale des groupes de Lie s’appliquait à peu près sans changement au cas p-adique. Les théorèmes fondamentaux du « dictionnaire » groupes de Lie-algèbres de Lie sont établis en 1942 dans la thèse de R. Hooke [166], élève de Chevalley; ce travail contient aussi l’analogue $p$-adique du théorème de E. Cartan sur les sous-groupes fermés des groupes de Lie réels.

Plus récemment, M. Lazard [195 b] développe une forme plus précise du « dictionnaire » pour les groupes analytiques compacts sur $\mathbf{Q}_p$. Il montre que l’existence d’une structure analytique $p$-adique sur un groupe compact G est étroitement liée à celle de certaines filtrations sur G, et en donne diverses applications (par exemple à la cohomologie de G). L’un des outils de Lazard est une amélioration des résultats de Dynkin sur la convergence de la série de Hausdorff $p$-adique [195 a].

VIII. ALGÈBRES DE LIE LIBRES

Il nous reste à parler d’une série de travaux sur les algèbres de Lie où le lien avec la théorie des groupes de Lie est fort ténu; ces recherches ont par contre des applications importantes en théorie des groupes « abstraits » et plus spécialement des groupes nilpotents.

L’origine en est le travail de P. Hall [144], paru en 1932. Il n’y est pourtant pas question d’algèbres de Lie : P. Hall a en vue l’étude d’une certaine classe de $p$-groupes, ceux qu’il appelle « réguliers ». Mais cela l’amène à examiner en détail les commutateurs itérés et la suite centrale descendante d’un groupe; il établit à cette occasion une variante de l’identité de Jacobi, ainsi que la « formule de Hall »

$$(xy)^n = x^n y^n(x, y)^{n(1-n)/2} \ldots$$

Peu après (en 1935-1937) paraissent les travaux fondamentaux de W. Magnus [215 a et b] et E. Witt [337 b]. Dans [215 a] Magnus utilise la même algèbre de séries formelles $\hat{A}$ que Hausdorff (appelée depuis « algèbre de Magnus »); il y plonge le groupe libre F et utilise la filtration naturelle de $\hat{A}$ pour obtenir une suite décroissante ($F_n$) de sous-groupes de F; c’est l’un des premiers exemples de filtration. Il conjecture que les $F_n$ coïncident avec les termes de la suite centrale descendante de F. Cette conjecture est démontrée dans son second mémoire [215 b]; c’est également là qu’il fait explicitement le rapprochement entre ses idées et celles de P. Hall, et qu’il définit l’algèbre de Lie libre L (comme sous-algèbre de A) dont il montre en substance qu’elle s’identifie au gradué de F. Dans [337 b], Witt complète ce résultat sur divers points. Il montre notamment que l’algèbre enveloppante de L est une algèbre associative libre et en déduit aussitôt le rang des composantes homogènes de L (« formules de Witt »).

Quant à la détermination de la base de L connue sous le nom de « base de Hall », il semble qu’elle n’apparaisse pour la première fois qu’en 1950, dans une note de M. Hall [143], bien qu’elle soit implicite dans les travaux de P. Hall et W. Magnus cités ci-dessus.
