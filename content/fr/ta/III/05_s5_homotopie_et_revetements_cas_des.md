---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 5
section_title: Homotopie et revêtements (cas des espaces localement connexes par arcs)
lang: fr
source: ta-i-iv-fr
book_pages: A III.308-A III.338
pdf_pages: 0324-0354
extraction: native
subsections:
    - "no": 1
      title: Condition homotopique de relèvement des applications continues
      page: 308
      pdf_page: 324
    - "no": 2
      title: Opérations du groupe de Poincaré et morphismes de revêtements
      page: 310
      pdf_page: 326
    - "no": 3
      title: Opérations sans monodromie locale du groupoïde de Poincaré
      page: 312
      pdf_page: 328
    - "no": 4
      title: Topologie admissible des groupes de Poincaré
      page: 315
      pdf_page: 331
statements: 23
exercises: 0
content_sha256: d7dace0e868d5da2a87b4d684c939e100489fda9ba8b12f6e4d9839d8b4aef32
---

## § 5. HOMOTOPIE ET REVÊTEMENTS (CAS DES ESPACES LOCALEMENT CONNEXES PAR ARCS)

### 1. Condition homotopique de relèvement des applications continues

#### Proposition 1 {#ta-iii-s5-prop-1 .statement tag=01ZL}

Soit B un espace topologique et soit $(E, p)$ un revêtement de B. Soit Y un espace topologique et soit $f: Y\rightarrow B$ une application continue. Soient $y\in$ Y$,x\in$ E$,b\in$ B des points tels que $f(y) =p(x) =b$. Supposons l’espace Y connexe et localement connexe par arcs. Pour qu’il existe un relèvement continu $g: Y\rightarrow E$ de $f$ tel que $g(y) =x$, il faut et il suffit que l’image de l’homomorphisme $\pi_1(f, y):\pi_1(Y, y)\rightarrow \pi_1(B, b)$ soit contenue dans l’image de l’homomorphisme $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, b)$.

La condition est nécessaire sans hypothèse sur l’espace Y. En effet, si un tel relèvement $g$ existe, on a $\pi_1(f, y) =\pi_1(p, x)\circ \pi_1(g, y)$.

Démontrons qu’elle est suffisante. Notons $s: \Lambda_b(B)\rightarrow \Lambda_x(E)$ l’homéomorphisme réciproque de l’homéomorphisme $c\mapsto p\circ c($III, p. 302, cor. 2 de la prop. 3) et soit $\varphi : \Lambda_y(Y)\rightarrow \Lambda_x(E)$ l’application $d\mapsto$ $s(f\circ d)$. L’application $\varphi$ est continue (I, p. 132, lemme).

Soient $d$ et $d'\in \Lambda_y(Y)$ des chemins d’origine $y$ ayant le même terme ; démontrons que les chemins $\varphi (d)$ et $\varphi (d')$ ont même terme. Posons $c=f\circ d,c'=f\circ d'$. Comme le chemin $d*\overline{d'}$ est un lacet dans Y en $y$, le chemin $c*\overline{c'}$ est un lacet dans B en $b$ et sa classe appartient à l’image de l’homomorphisme $\pi_1(f, y)$, donc à l’image de l’homomorphisme $\pi_1(p, x)$ par hypothèse. D’après le cor. 2 de la prop. 4 (III, p. 303), le chemin $s(c*\overline{c'})$ est un lacet dans E en $x$. Il en est de même du chemin $s(c'*\overline{c})$ qui, par unicité du relèvement des chemins, est égal à $s(c*\overline{c'})$. On a donc $s(c'*\overline{c})(\frac{1}{2}) =s(c')(1) =s(c)(1)$, ce qu’on voulait démontrer.

Notons respectivement $e_E: \Lambda_x(E)\rightarrow E$ et $e_Y: \Lambda_y(Y)\rightarrow Y$ les applications terme. Comme l’espace Y est supposé connexe et localement connexe par arcs, l’application $e_Y$ est surjective et ouverte (III, p. 262, prop. 10). D’après l’alinéa précédent, il existe une unique application $g: Y\rightarrow E$ telle que $e_E\circ \varphi =g\circ e_Y$. Elle est continue, car l’application $e_Y$ stricte ( I, p. 18, exemple 2).

Vérifions enfin que l’application $g$ relève l’application $f$ et que $g(y) =x$. Tout point $z$ de Y est le terme d’un chemin $c$ d’origine $y$. Le chemin $\varphi (c)$ est un relèvement de $f\circ c$ d’origine $x$ et de terme le point $g(z)$. On a donc $p(g(z)) =f(z)$. Pour $z=y$ et $c=e_y$, on a $\varphi (e_y) =e_x$, d’où $g(y) =x$.

#### Corollaire 1 {#ta-iii-s5-prop-1-cor-1 .statement tag=01ZM}

Soit B un espace topologique connexe et localement connexe par arcs, et soit $b$ un point de B. Pour qu’un revêtement $(E, p)$ de B soit trivialisable, il faut et il suffit que, pour tout point $x$ de la fibre $E_b$, l’homomorphisme $\pi_1(p, x)$ soit bijectif.

Rappelons que l’homomorphisme $\pi_1(p, x)$ est injectif (III, p. 303, cor. 1 de la prop. 4). L’énoncé résulte donc de la prop. 1 et de I, p. 81, cor. 4 de la prop. 6.

#### Remarque {#ta-iii-s5-n1-rem-1 .statement tag=01ZN}

Soit B un espace topologique localement connexe par arcs, soit $b$ un point de B et soit V un voisinage ouvert et connexe de $b$ tel que l’homomorphisme de $\pi_1(V, b)$ dans $\pi_1(B, b)$ ait pour image le sous-groupe réduit à l’élément neutre. D’après le cor. 1, tout revêtement de B est trivialisable au-dessus de V, et a fortiori au-dessus de toute partie de B contenue dans V.

#### Corollaire 2 {#ta-iii-s5-prop-1-cor-2 .statement tag=01ZO}

Soit B un espace topologique connexe et localement connexe par arcs. Si, pour un point $b$ de B, le groupe $\pi_1(B, b)$ est réduit à l’élément neutre, l’espace B est simplement connexe.

En effet, il résulte du corollaire 1 que, sous ces hypothèses, tout revêtement de B est trivialisable.

#### Corollaire 3 {#ta-iii-s5-prop-1-cor-3 .statement tag=01ZP}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Supposons que E soit un revêtement de B et que l’espace $B'$ soit connexe et localement connexe par arcs. Soient $b'$ un point de $B'$ et $b=f(b')$. Pour que $(E', p')$ soit un revêtement trivialisable de $B'$, il faut et il suffit que, pour tout point $x$ de la fibre $E_b$, l’image de $\pi_1(p, x)$ contienne l’image de $\pi_1(f, b)$.

Cela résulte de la prop. 1 et de I, p. 81, cor. 5 de la prop. 6.

### 2. Opérations du groupe de Poincaré et morphismes de revêtements

Soit B un espace topologique connexe et localement connexe par arcs et soit $b$ un point de B.

Soit E un revêtement de B. Comme l’espace B est supposé connexe, la fibre $E_b$ n’est pas vide si E n’est pas vide (I, p. 74, prop. 4). D’après l’assertion a) du théorème 1 de III, p. 305, le revêtement E est connexe et non vide si et seulement si le groupe $\pi_1(B, b)$ opère transitivement sur $E_b$.

#### Proposition 2 {#ta-iii-s5-prop-2 .statement tag=01ZQ}

Soient E et $E'$ des revêtements de B.

a) Soit $f: E\rightarrow E'$ un B-morphisme. L’application $f_b: E_b\rightarrow E'_b$ déduite de $f$ est compatible avec les opérations de $\pi_1(B, b)$ sur $E_b$ et $E'_b$ respectivement. Elle est bijective si et seulement si $f$ est un isomorphisme.

b) L’application $f\mapsto f_b$ est une bijection de l’ensemble $\mathscr{C}_B(E; E')$ des B-morphismes de E dans $E'$ sur l’ensemble $\mathscr{F}_{\pi_1(B,b)}(E_b; E'_b)$ des $\pi_1(B, b)$-morphismes de $E_b$ dans $E'_b$.

Si $f$ est un B-morphisme de E dans $E'$, l’application $f_b: E_b\rightarrow E'_b$ est un $\pi_1(B, b)$-morphisme (cf. III, p. 305). De plus, deux B-morphismes de E dans $E'$ qui coïncident sur la fibre $E_b$ sont égaux (I, p. 80, cor. 3 de la prop. 6).

Soit $\varphi : E_b\rightarrow E'_b$ un morphisme de $\pi_1(B, b)$-ensembles ; démontrons qu’il existe un B-morphisme $f$ de E dans $E'$ tel que $f_b=\varphi$. On peut supposer les espaces E et $E'$ connexes et non vides, de sorte que $E_b$ et $E'_b$ sont des $\pi_1(B, b)$-ensembles homogènes. Soit $x$ un point de $E_b$; son fixateur G est l’image de l’application $\pi_1(p, x)$ (III, p. 305, théorème 1). Comme l’application $\varphi$ est un $\pi_1(B, b)$-morphisme, le groupe G fixe le point $x'=\varphi (x)$ de $E'_b$, donc est contenu dans l’image de l’application $\pi_1(p', x')$. D’après la prop. 1 de III, p. 308, il existe un B-morphisme $f$ de E dans $E'$ tel que $f(x) =x'$. Les applications $f_b$ et $\varphi$ sont des $\pi_1(B, b)$-morphismes du $\pi_1(B, b)$-ensemble homogène $E_b$ dans $E'_b$ qui coïncident au point $x$; elles sont donc égales.

Si $f: E\rightarrow E'$ est un B-isomorphisme, l’application $f_b: E_b\rightarrow E'_b$ est bijective. Inversement, supposons l’application $f_b$ bijective et soit $g: E'\rightarrow$ E un B-morphisme tel que $g_b= (f_b)^{-1}$. Le B-morphisme $g\circ f: E\rightarrow E$ induit sur $E_b$ l’application identique ; il résulte donc de la proposition que $g\circ f=$ Id$_E$. De même, $f\circ g=$ Id$_{E'}$, ce qui prouve que $f$ est un B-isomorphisme.

#### Corollaire 1 {#ta-iii-s5-prop-2-cor-1 .statement tag=01ZR}

Les revêtements E et $E'$ sont isomorphes si et seulement si les $\pi_1(B, b)$-ensembles $E_b$ et $E'_b$ sont isomorphes.

#### Corollaire 2 {#ta-iii-s5-prop-2-cor-2 .statement tag=01ZS}

Soient $(E, p)$ et $(E', p')$ des revêtements connexes de B. Soient $x$ un point de $E_b$ et $x'$ un point de $E'_b$. Pour qu’il existe un B-morphisme $g: E\rightarrow E'$ tel que $g(x) =x'$, il faut et il suffit que l’on ait $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. Un tel morphisme est alors unique et est un isomorphisme si et seulement si les sous-groupes $p_*(\pi_1(E, x))$ et $p'_*(\pi_1(E', x'))$ de $\pi_1(B, b)$ sont égaux.

D’après III, p. 305, théorème 1, l’application de $\pi_1(B, b)$ sur $E_b$ définie par $\gamma \mapsto x\cdot \gamma$ induit par passage au quotient un isomorphisme du $\pi_1(B, b)$-ensemble $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ sur $E_b$. De même, il existe un unique isomorphisme de $\pi_1(B, b)$-ensembles de $p_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ sur $E'_b$. D’après la proposition 2, il existe un B-morphisme $g: E\rightarrow E'$ tel que $g(x) =x'$ si et seulement s’il existe un morphisme de $\pi_1(B, b)$-ensembles de $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ sur $p'_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ qui envoie la classe $p_*(\pi_1(E, x))$ sur la classe $p'_*(\pi_1(E', x'))$. Un tel morphisme existe si et seulement si l’on a $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. Il est alors unique, car l’espace E est supposé connexe (I, p. 34, cor. 2 de la prop. 11). C’est un isomorphisme si et seulement si les sous-groupes $p_*(\pi_1(E, x))$ et $p'_*(\pi_1(E', x'))$ de $\pi_1(B, b)$ sont égaux.

#### Corollaire 3 {#ta-iii-s5-prop-2-cor-3 .statement tag=01ZT}

Soit $(E, p)$ un revêtement connexe de B et soit $x$ un point de la fibre $E_b$. Notons N le normalisateur de $p_*(\pi_1(E, x))$ dans $\pi_1(B, b)$. Pour tout élément $\gamma$ de N, il existe un unique B-automorphisme $g$ de E tel que $g(x) =x\cdot \gamma$, et l’application $\gamma \mapsto g$ définit par passage au quotient un isomorphisme de groupes de $N/p_*(\pi_1(E, x))$ sur Aut$_B(E)$.

Soit $\gamma \in \pi_1(B, b)$ ; on a $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot \gamma )))$ (III, p. 305, théorème 1, c)). D’après le corollaire 2, pour qu’il existe un B-automorphisme $g$ de E tel que $g(x) =x\cdot \gamma$, il faut et il suffit que $\gamma$ appartienne à N. Un tel isomorphisme est alors unique. Notons $\alpha : N\rightarrow$ Aut$_B(E)$ l’application $\gamma \mapsto g$ ainsi définie.

Soient $\gamma$ et $\gamma '$ deux éléments de N. Posons $g=\alpha (\gamma ),g'=\alpha (\gamma ')$ ; on a $g(g'(x)) =g(x\cdot \gamma ') =g(x)\cdot \gamma '= (x\cdot \gamma )\cdot \gamma '=x\cdot (\gamma \gamma ')$ d’après les relations (4), III, p. 305 et (1), p. 304. Par suite, $\alpha$ est un homomorphisme de groupes. Pour que $\alpha (\gamma ) =$ Id$_E$, il faut et il suffit que l’on ait $x\cdot \gamma =x$, en vertu de l’unicité de $\alpha (\gamma )$, c’est-à-dire $\gamma \in p_*(\pi_1(E, x))$ (III, p. 305, théorème 1, b)). Enfin, si $g$ est un B-automorphisme de E, il existe un chemin $c$ joignant $x$ à $g(x)$ dans E (qui est connexe par arcs), et l’on a alors $g(x) =x\cdot \gamma$, où $\gamma$ est la classe du chemin $p\circ c$. Cela prouve que l’homomorphisme $\alpha$ est surjectif.

Le groupe Aut$_B(E)$ opère sur la fibre $E_b$ et s’identifie au groupe des automorphismes du $\pi_1(B, b)$-ensemble (à droite) homogène $E_b($cf. A, I, p. 56, prop. 5 et 6).

#### Corollaire 4 {#ta-iii-s5-prop-2-cor-4 .statement tag=01ZU}

Soit $(E, p)$ un revêtement connexe de B et soit $x$ un point de la fibre $E_b$. Pour que E soit un revêtement galoisien de B, il faut et il suffit que $p_*(\pi_1(E, x))$ soit un sous-groupe distingué de $\pi_1(B, b)$. Le groupe Aut$_B(E)$ est alors isomorphe au groupe quotient $\pi_1(B, b)/p_*(\pi_1(E, x))$.

Si $p_*(\pi_1(E, x))$ est un sous-groupe distingué de $\pi_1(B, b)$, le groupe Aut$_B(E)$ opère transitivement sur la fibre $E_b$ d’après le corollaire 3, de sorte que E est un revêtement galoisien de B (I, p. 102, th. 2). La réciproque est l’assertion d) du théorème 1 (III, p. 305). La dernière assertion résulte du corollaire 3.

### 3. Opérations sans monodromie locale du groupoïde de Poincaré

#### Lemme 1 {#ta-iii-s5-lem-1 .statement tag=01ZV}

Soit B un espace topologique localement connexe par arcs, soient $p: E\rightarrow B$ et $p': E'\rightarrow B$ des applications étales et séparées qui vérifient la propriété de relèvement des chemins (III, p. 302). Soit $g: E\rightarrow E'$ une application telle que $p'\circ g=p$. On suppose que $g$ est compatible avec les opérations canoniques du groupoïde $\varpi (B)$ sur E et $E'$. Alors, $g$ est continue.

Soit $c$ un chemin dans E ; posons $c'=g\circ c$ et démontrons que l’application $c'$ est continue. Notons $d$ le chemin $p\circ c$ dans B et, pour tout $t\in \mathbf{I}$, notons $d_t$ le chemin $s\mapsto d(st)$. Pour tout $t\in \mathbf{I}$, on a $c(t) =c(0)\cdot d_t($III, p. 304, remarque 3), d’où $c'(t) =c'(0)\cdot d_t$ d’après l’hypothèse faite sur $g$, ce qui prouve que $c'$ est un chemin relevant le chemin $d$, d’après cette même remarque. Cela prouve que l’application $g$ est continue par arcs. Comme l’espace E est localement connexe par arcs (III, p. 261, cor. 2), l’application $g$ est continue (III, p. 269, corollaire de la prop. 13).

Soit B un espace topologique. Considérons une opération $\varphi$ = $(\varphi_{a,b})_{(a,b)\in B\times B}$ du groupoïde $\varpi (B)$ sur un ensemble E, relativement à une application $p: E\rightarrow B$. On dit que $\varpi (B)$ opère sans monodromie sur E (cf. II, p. 168) si pour tout $b\in$ B et toute classe de lacet $\gamma \in \pi_1(B, b)$, l’action de $\gamma$ sur la fibre $E_b$ est triviale. Si B est connexe par arcs, il suffit qu’il en soit ainsi pour un point de B (loc. cit.). Nous dirons que l’opération $\varphi$ du groupoïde $\varpi (B)$ est sans monodromie locale si tout point de B possède un voisinage V tel que $\varpi (V)$ opère sans monodromie sur l’ensemble $E_V$ = $\overset{-1}{p}(V)$ relativement à l’application $p_V=p|\overset{-1}{p}(V)$.

#### Remarque {#ta-iii-s5-n3-rem-1 .statement tag=01ZW}

Soit B un espace topologique localement connexe par arcs et supposons que tout point $b$ de B possède un voisinage V tel que l’image de $\pi_1(V, b)$ dans $\pi_1(B, b)$ soit réduite à l’élément neutre (cf. IV, p. 340, déf. 2). Alors, toute opération du groupoïde $\varpi (B)$ est sans monodromie locale.

En effet, considérons un ensemble E, une application $p: E\rightarrow B$ et une opération $\varphi$ du groupoïde $\varpi (B)$ sur E relativement à $p$. Soit $a$ un point de B et soit V un voisinage de $a$ tel que l’image de $\pi_1(V, a)$ dans $\pi_1(B, a)$ soit réduite à l’élément neutre. Soit U un voisinage connexe par arcs de $a$ contenu dans V. Soit $b$ un point de U et soit $\gamma \in \pi_1(U, b)$. Soit $\delta$ la classe d’un chemin reliant $a$ à $b$ dans U. Alors, $\delta \gamma \delta^{-1}$ est la classe d’un lacet en $a$ dans U ; son image dans $\pi_1(B, a)$ est donc triviale. On a ainsi $\varphi_{a,a}(\delta \gamma \delta^{-1}) =$ Id$_{E_a}$, d’où $\varphi_{b,b}(\gamma ) =$ Id$_{E_b}$. Cela démontre que l’opération de $\varpi (U)$ sur le U-espace $E_U$ est sans monodromie. Par suite, l’opération $\varphi$ est sans monodromie locale.

#### Proposition 3 {#ta-iii-s5-prop-3 .statement tag=01ZX}

Soit B un espace topologique localement connexe par arcs et soit E un ensemble muni d’une opération sans monodromie locale $\varphi$ du groupoïde $\varpi (B)$, relativement à une application $p: E\rightarrow B$. Il existe alors sur E une unique topologie pour laquelle les conditions suivantes sont satisfaites :

(i) L’ensemble E muni de cette topologie et de l’application $p$ est un revêtement de B;

(ii) L’opération canonique de $\varpi (B)$ sur ce revêtement est identique à l’opération $\varphi$.

L’unicité d’une telle topologie résulte du lemme 1 de III, p. 312, où l’on prend pour $g$ l’application identique de E. Pour démontrer son existence, on peut en outre supposer que B est connexe et non vide.

Supposons tout d’abord que l’opération $\varphi = (\varphi_{a,b})_{(a,b)\in B\times B}$ du groupoïde $\varpi (B)$ sur l’ensemble E, relativement à $p$, soit sans monodromie.

Soit $a$ un point de B. Pour tout point $b\in B$, il existe un chemin $c$ dans B joignant $a$ à $b$. Si $\gamma \in \varpi_{a,b}(B)$ désigne la classe du chemin $c$, la bijection $\varphi_{a,b}(\gamma ): E_a\rightarrow E_b$ est indépendante du chemin $c$, car l’opération est sans monodromie ; on note $f_{a,b}$ cette bijection. L’application $\Phi_a: B\times E_a\rightarrow$ E définie par $(b, x)\mapsto f_{a,b}(x)$ est une bijection ; la bijection réciproque associe à $x\in E$ le couple $(p(x), f_{p(x),a}(x))$. Munissons l’ensemble $E_a$ de la topologie discrète, de sorte que le B-espace $B\times E_a$ est un revêtement trivial de B. Par transport de structure, la bijection $\Phi_a$ munit E d’une topologie qui en fait un revêtement de B.

Démontrons que l’opération canonique de $\varpi (B)$ sur E est identique à l’opération $\varphi$. Soient $x$ un point de $E_a$ et $b$ un point de B. Soit $c$ un chemin dans B qui joint le point $a$ au point $b$; l’application $t\mapsto \Phi_a(c(t), x)$ est alors un chemin dans E qui joint le point $x$ au point $\Phi_a(b, x) =f_{a,b}(x)$. Si $\gamma \in \varpi_{a,b}(B)$ désigne la classe du chemin $c$, on a ainsi $x\cdot \gamma =f_{a,b}(x)$. Cela démontre que l’opération canonique de $\varpi (B)$ sur le revêtement E et l’opération $\varphi$ coïncident sur les classes de chemins d’origine $a$. Comme ces classes engendrent le groupoïde $\varpi (B)$, les deux opérations sont égales.

Traitons maintenant le cas général. Soit $\mathscr{B}$ l’ensemble des parties ouvertes V de E telles que $\varpi (V)$ opère sans monodromie sur $\overset{-1}{p}(V)$. Par hypothèse, les éléments de $\mathscr{B}$ recouvrent B. D’après ce qui précède, il existe pour tout $V\in \mathscr{B}$, une unique topologie sur l’ensemble $\overset{-1}{p}(V)$ telle que $(\overset{-1}{p}(V), p_V)$ soit un revêtement de V et que l’opération canonique de $\varpi (V)$ sur ce revêtement coïncide avec l’opération induite par $\varphi$.

Soient V et $V'\in \mathscr{B}$. La topologie de $\overset{-1}{p}(V\cap V')$ induite par la topologie de $\overset{-1}{p}(V)$ (resp. de $\overset{-1}{p}(V')$) définie ci-dessus en fait un revêtement de $V\cap V'$ sur lequel l’opération canonique de $\varpi (V\cap V')$ est induite par l’opération $\varphi$. Ces topologies coïncident donc avec celle de $\overset{-1}{p}(V\cap V')$. Il existe alors une unique topologie sur E induisant sur chaque $\overset{-1}{p}(V)$ la topologie précédemment définie (cf. I, § 2, p. 16).

Lorsque E est muni de cette topologie, l’application $p$ est continue et le B-espace E est un revêtement. L’opération canonique de $\varpi (B)$ sur ce revêtement coïncide avec l’opération $\varphi$ sur les classes de chemins dont l’image est contenue dans un des ouverts de $\mathscr{B}$. D’après le lemme 4 de III, p. 272, ces classes engendrent le groupoïde $\varpi (B)$. Il en résulte que ces deux opérations sont égales (II, p. 167).

#### Corollaire {#ta-iii-s5-n3-cor-1 .statement tag=01ZY}

Soit B un espace topologique connexe et localement connexe par arcs, soit $(E, p)$ un B-espace dont la projection $p$ est étale, séparée et possède la propriété de relèvement des chemins. Si l’opération canonique de $\varpi (B)$ sur l’ensemble E, relativement à $p$, est sans monodromie locale, alors E est un revêtement de B.

Munissons E de l’opération canonique de $\varpi (B)$ définie par le relèvement des chemins (III, p. 303, n$^o3$). Il existe une topologie sur E pour laquelle les conditions (i) et (ii) de la prop. 3 sont satisfaites. Cette topologie coïncide avec la topologie donnée sur E d’après le lemme 1 de III, p. 312.

### 4. Topologie admissible des groupes de Poincaré

Soit B un espace topologique et soit $a$ un point de B. On dit qu’un sous-groupe H de $\pi_1(B, a)$ est admissible si tout point $b$ de B a un voisinage V tel que l’on ait $\gamma i_*(\delta )\gamma^{-1}\in H$ pour tout $\gamma \in \varpi_{a,b}(B)$ et tout $\delta \in \pi_1(V, b)$, où $i: V\rightarrow$ B est l’injection canonique. Si H est un sous-groupe distingué de $\pi_1(B, a)$, il suffit, pour que H soit admissible, que cette condition soit vérifiée pour une classe de chemins $\gamma \in \varpi_{a,b}(B)$.

#### Proposition 4 {#ta-iii-s5-prop-4 .statement tag=01ZZ}

Il existe une unique topologie sur $\pi_1(B, a)$, compatible avec sa structure de groupe, pour laquelle les sous-groupes distingués admissibles de $\pi_1(B, a)$ forment un système fondamental de voisinages de l’élément neutre. Pour cette topologie, les sous-groupes ouverts sont exactement les sous-groupes admissibles.

Les faits suivants résultent de la définition d’un sous-groupe admissible :

a) Le groupe $\pi_1(B, a)$ est admissible ;

b) Un sous-groupe contenant un sous-groupe admissible est admissible ;

c) L’intersection d’une famille finie de sous-groupes admissibles est admissible ;

d) Pour tout sous-groupe admissible H de $\pi_1(B, a)$ l’intersection des sous-groupes $\gamma H\gamma^{-1}$, lorsque $\gamma$ parcourt $\pi_1(B, a)$, est admissible. En particulier, l’ensemble des sous-groupes distingués admissibles est une base de filtre formée de sous-groupes de $\pi_1(B, a)$ vérifiant l’axiome (GV$'_{III})$ de III, p. 4, d’où la première partie de la proposition d’après TG, III, p. 5, exemple. La seconde partie est alors immédiate (cf. TG, III, p. 7, corollaire de la prop. 4).

La topologie sur le groupe $\pi_1(B, a)$ caractérisée dans la proposition 4 est appelée la topologie admissible.

#### Remarque 1 {#ta-iii-s5-n4-rem-1 .statement tag=0200}

Si $B_0$ désigne la composante connexe par arcs de $a$ dans B, l’isomorphisme canonique $\pi_1(B_0, a)\rightarrow \pi_1(B, a)$ est un isomorphisme de groupes topologiques lorsque ces groupes sont munis de la topologie admissible.

#### Remarque 2 {#ta-iii-s5-n4-rem-2 .statement tag=0201}

Soit B un espace topologique. Soient $b$ et $b'$ des points de B qui appartiennent à la même composante connexe par arcs et soit $\gamma$ un élément de $\varpi_{b,b'}(B)$. Il résulte de la définition d’un sous-groupe admissible que, pour tout sous-groupe admissible H de $\pi_1(B, b')$, le sous-groupe $\gamma H\gamma^{-1}$ de $\pi_1(B, b)$ est admissible. Par suite, l’isomorphisme $u_{\gamma}:\delta \mapsto \gamma \delta \gamma^{-1}$ de $\pi_1(B, b')$ sur $\pi_1(B, b)$ (cf. III, p. 292) est un homéo-morphisme lorsqu’on munit ces groupes des topologies admissibles.

#### Remarque 3 {#ta-iii-s5-n4-rem-3 .statement tag=0202}

Soient A et B des espaces topologiques, soit $a$ un point de A et soit $f: A\rightarrow B$ une application continue. Posons $b=f(a)$. Si H est un sous-groupe admissible de $\pi_1(B, b)$, son image réciproque par l’homomorphisme $\pi_1(f, a)$ est un sous-groupe admissible de $\pi_1(A, a)$. Par conséquent, l’homomorphisme de groupes $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ est continu, lorsque ces groupes sont munis de la topologie admissible.

#### Proposition 5 {#ta-iii-s5-prop-5 .statement tag=0203}

Soit B un espace topologique localement connexe par arcs et soit $a$ un point de B. Pour qu’un sous-groupe H de $\pi_1(B, a)$ soit admissible, il faut et il suffit qu’il existe un revêtement $(E, p)$ de B et un point $x\in E_a$ tel que $H =p_*(\pi_1(E, x))$.

Soit $(E, p)$ un revêtement de B et soit $x$ un point de $E_a$; posons $H =p_*(\pi_1(E, x))$ et montrons que c’est un sous-groupe admissible de $\pi_1(B, a)$. Soit $b$ un point de B et soit V un voisinage de $b$ tel que $E_V=$ $(\overset{-1}{p}(V), p_V)$ soit un revêtement trivialisable de V. Soit $\gamma \in \varpi_{a,b}(B)$ ; nous allons démontrer que pour tout élément $\delta \in \pi_1(V, b)$, la classe de chemins $\gamma \delta \gamma^{-1}$ appartient à H.

D’après III, p. 301, prop. 3, il existe une unique classe d’homotopie stricte $\gamma '$ de chemin d’origine $x$ dans E telle que $p_*(\gamma ') =\gamma$ Soit $y$ le terme de $\gamma '$; on a $p(y) =b($III, p. 302, prop. 4). Soit alors $\delta '$ l’unique classe de chemin d’origine $y$ dans E telle que $p_*(\delta ') =\delta$. Comme $E_V$ est trivialisable, $\delta '$ est la classe d’un lacet en $y$. Alors, $\gamma '\delta '(\gamma ')^{-1}$ est la classe d’un lacet en $a$ dans E dont l’image par $p_*$ est la classe $\gamma \delta \gamma^{-1}$, ce qu’il fallait démontrer.

Inversement, soit H un sous-groupe admissible de $\pi_1(B, a)$. Soit $\lambda_a(B)$ le quotient de l’espace $\Lambda_a(B)$ des chemins d’origine $a$ pour la relation d’homotopie stricte ; comme deux chemins strictement homotopes ont même terme, l’application terme $e: \Lambda_a(B)\rightarrow B$ définit par passage au quotient une application $\varepsilon :\lambda_a(B)\rightarrow B$. La composition des classes de chemins munit l’ensemble $\lambda_a(B)$ d’une action à gauche du groupe $\pi_1(B, a)$. Munissons-le de l’action du groupe H déduite par restriction et notons $H\backslash \lambda_a(B)$ l’ensemble de ses orbites.

L’application $\varepsilon :\lambda_a(B)\rightarrow B$ induit, par passage au quotient, une application $q: H\backslash \lambda_a(B)\rightarrow B$. La composition des classes de chemins munit l’ensemble $H\backslash \lambda_a(B)$ d’une opération à droite du groupoïde $\varpi (B)$ relativement à l’application $q$.

Cette opération est sans monodromie locale. Soit en effet $b$ un point de B et soit V un voisinage de $b$ tel que $\gamma i_*(\pi_1(V, b))\gamma^{-1}\subset H$ pour toute classe de chemins $\gamma$ reliant $a$ à $b$ dans B, où $i$ désigne l’inclusion de V dans B. Comme B est localement connexe par arcs, on peut en outre supposer que V est connexe par arcs. Soit $c\in V$, soit $\delta$ la classe dans $\pi_1(B, c)$ d’un lacet en $c$ contenu dans V et soit $\delta '$ un élément de $\lambda_a(B)$ tel que $\varepsilon (\delta ') =c$. Soit $\delta ''$ un élément de $\varpi_{c,b}(V)$ et posons $\gamma =\delta '\delta ''$. Par définition de V, l’élément $\delta '\delta (\delta ')^{-1}=\gamma ((\delta '')^{-1}\delta \delta '')\gamma^{-1}$ de $\pi_1(B, a)$ appartient à H. Alors, $H\delta '\cdot \delta = H\delta '$; cela démontre que $\pi_1(V, c)$ agit trivialement sur l’ensemble $\overset{-1}{q}(c)$.

D’après III, p. 313, prop. 3, il existe une unique topologie sur $H\backslash \lambda_a(B)$ pour laquelle $q$ est continue et le B-espace $(H\backslash \lambda_a(B), q)$ est un revêtement tel que l’opération canonique de $\varpi (B)$ sur ce revêtement soit l’opération définie ci-dessus. D’après l’assertion b) du théorème 1 de III, p. 305, le groupe $q_*(\pi_1(H\backslash \lambda_a(B),H))$ est égal à H.

Nous dirons qu’une opération du groupe $\pi_1(B, b)$ sur un ensemble X est admissible si le noyau de l’application canonique $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ est un sous-groupe ouvert de $\pi_1(B, b)$. Cela revient à dire que l’homomorphisme $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ est continu si le groupe $\mathfrak{S}_X$ est muni de la topologie discrète. L’application $\pi_1(B, b)\times X\rightarrow X$ est alors continue, lorsque X est muni de la topologie discrète. Inversement, considérons une opération continue de $\pi_1(B, b)$ sur un espace discret X. Soit $x$ un point de X ; son fixateur est un sous-groupe ouvert H de $\pi_1(B, b)$ par hypothèse. Pour $\gamma \in \pi_1(B, b)$, le fixateur de $\gamma \cdot x$ est le sous-groupe $\gamma H\gamma^{-1}$, de sorte que le sous-groupe de $\pi_1(B, b)$ fixant chaque élément de l’orbite de $x$ est l’intersection des sous-groupes $\gamma H\gamma^{-1}$, pour $\gamma$ parcourant $\pi_1(B, b)$. C’est un sous-groupe ouvert car les sous-groupes ouverts distingués de $\pi_1(B, b)$ forment une base de sa topologie (III, p. 315, prop. 4). Cela entraîne qu’une opération continue de $\pi_1(B, b)$ sur un espace discret X est admissible si elle est transitive ou, plus généralement, si l’ensemble des orbites des éléments de X est fini.

Pour tout groupe discret G, tout revêtement E de B principal de groupe G et tout point $x\in E_b$, rappelons que l’application $h_{(E,x)}$ de $\pi_1(B, b)$ dans G qui, à $\gamma \in \pi_1(B, b)$, associe l’unique élément $g\in G$ tel que $x\cdot g=x\cdot \gamma^{-1}$ est un homomorphisme de groupes (III, p. 306, prop. 5).

#### Proposition 6 {#ta-iii-s5-prop-6 .statement tag=0204}

Soit B un espace topologique et soit $b$ un point de B. Munissons le groupe $\pi_1(B, b)$ de la topologie admissible.

a) Pour tout groupe discret G, tout revêtement E de B, principal de groupe G et tout $x\in E_b$, l’homomorphisme $h_{(E,x)}$ est un homomorphisme continu de groupes topologiques.

b) Pour tout revêtement E de B, l’opération canonique de $\pi_1(B, b)$ sur la fibre $E_b$ est admissible.

Il suffit de démontrer la seconde assertion. Soit K l’ensemble des éléments $k\in \pi_1(B, b)$ tels que $x\cdot k=x$ pour tout $x\in E_b$; démontrons que K est un sous-groupe admissible de $\pi_1(B, b)$.

Soit $b'$ un point de B et soit $V'$ un voisinage de $b'$ dans B au-dessus duquel le revêtement E est trivialisable. Soit $\gamma$ la classe d’un chemin $c$ reliant $b$ à $b'$ dans B et soit $c'$ l’unique chemin d’origine $x$ dans E qui relève $c$. Pour tout $\delta \in \pi_1(V', b')$ et tout $x'\in E_{b'}$, on a $x'\cdot \delta =x'$. Par suite, pour $x\in E_b$ et $\delta \in \pi_1(V', b')$, on a

$$
x\cdot \gamma \delta \gamma^{-1}= ((x\cdot \gamma )\cdot \delta )\cdot \gamma^{-1}= (x\cdot \gamma )\cdot \gamma^{-1}=x
$$

si bien que $\gamma \delta \gamma^{-1}$ appartient à K. Autrement dit, K est un sous-groupe admissible, d’où la proposition.

#### Proposition 7 {#ta-iii-s5-prop-7 .statement tag=0205}

Soit B un espace topologique connexe et localement connexe par arcs et soit $b$ un point de B. Munissons le groupe $\pi_1(B, b)$ de la topologie admissible.

a) Soit G un groupe topologique discret. Pour tout homomorphisme continu $f:\pi_1(B, b)\rightarrow$ G, il existe un revêtement E de B, principal de groupe G et un point $x$ de $E_b$ tels que $h_{(E,x)}=f$.

b) Pour tout espace topologique discret F muni d’une opération à droite, admissible, du groupe $\pi_1(B, b)$, il existe un revêtement E de B tel que les $\pi_1(B, b)$-ensembles F et $E_b$ soient isomorphes.

Démontrons a). Soit $f$ un homomorphisme continu de $\pi_1(B, b)$ dans un groupe discret G. Son noyau est un sous-groupe ouvert distingué K de $\pi_1(B, b)$ ; notons H le groupe $\pi_1(B, b)/K$ et $\overline{f}: H\rightarrow G$ l’homomorphisme de groupes déduit de $f$ par passage au quotient. D’après III, p. 316, prop. 5, il existe un revêtement connexe $E'$ de B tel que le sous-groupe K soit le fixateur de tout point de la fibre $E'_b$; le revêtement $E'$ est principal de groupe $H =\pi_1(B, b)/K$. Soit $x'$ un point de $E'_b$; l’homomorphisme $h_{(E',x')}:\pi_1(B, b)\rightarrow H$ est surjectif de noyau K (III, p. 306, prop. 5). Soit donc $\varphi : H\rightarrow G$ l’unique homomorphisme de groupes tel que $\varphi \circ h_{(E',x')}=f$. Le revêtement associé $E = E'\times^HG$ de B est principal de groupe G et l’on a $h_{(E,x)}=\varphi \circ h_{(E',x')}=f$ (III, p. 307, exemple 2). Cela démontre l’assertion a).

Démontrons b). Soit F un ensemble muni d’une opération à droite, admissible, du groupe $\pi_1(B, b)$. Notons $f:\pi_1(B, b)\rightarrow \mathfrak{S}_F$ cette opération et munissons le groupe $\mathfrak{S}_F$ de la topologie discrète. D’après a), il existe un revêtement E de B, principal de groupe $\mathfrak{S}_F$, et un point $x\in E$ tels que l’homomorphisme $h_{(E,x)}$ soit égal à $f$. L’opération canonique du groupe $\pi_1(B, b)$ sur la fibre en $b$ du revêtement associé $E\times^{\mathfrak{S}_F}F$ de B s’identifie à l’opération de $\pi_1(B, b)$ sur F (III, p. 306, exemple 1).

#### Remarque 4 {#ta-iii-s5-n4-rem-4 .statement tag=0206}

La topologie admissible sur $\pi_1(B, b)$ est la topologie la moins fine pour laquelle l’opération de $\pi_1(B, b)$ sur $E_b$ est continue pour tout revêtement connexe E de B (prop. 6 de III, p. 318 et prop. 7 de III, p. 318). Si E est un revêtement connexe de B et $x$ un point de la fibre $E_b$, l’application $c'\mapsto c'(1)$ de $\Lambda_x(E)$ dans E est continue Par conséquent, l’application $c\mapsto x\cdot c$ de $\Lambda_b(B)$ dans E est continue (III, p. 302, cor. 2 de la prop. 3). Par restriction à $\Omega_b(B)$ et passage au quotient, on en déduit que l’application $\gamma \mapsto x\cdot \gamma$ est continue lorsqu’on munit le groupe $\pi_1(B, b)$ de la topologie d’espace quotient de $\Omega_b(B)$. La topologie admissible sur $\pi_1(B, b)$ est donc moins fine que la topologie quotient de la topologie de la convergence compacte. Elle peut être strictement moins fine (III, p. 337, exerc. 7).

#### Remarque 5 {#ta-iii-s5-n4-rem-5 .statement tag=0207}

Soit B un espace topologique connexe et localement connexe par arcs, soit $a$ un point de B et soit H un sous-groupe de $\pi_1(B, a)$. D’après la remarque précédente, si H est admissible, il est aussi ouvert pour la topologie quotient de la topologie de la convergence compacte. Inversement, supposons que H soit un sous-groupe distingué de $\pi_1(B, a)$ qui est ouvert pour la topologie quotient de la topologie de la convergence compacte. Soit $x$ un point de B et soit $\gamma \in \varpi_{a,x}(B)$. Le sous-groupe $\gamma^{-1}H\gamma$ de $\pi_1(B, x)$ est encore ouvert pour la topologie quotient de la topologie de la convergence compacte (III, p. 293, remarque 3). Il existe donc un voisinage V de $x$ dans B tel que $\gamma^{-1}H\gamma$ contienne la classe de tout lacet en $x$ dont l’image est contenue dans V. On a ainsi $\gamma \pi_1(V, x)\gamma^{-1}\subset H$; comme H est distingué, cela entraîne que H est un sous-groupe admissible de $\pi_1(B, a)$.

# Exercices

§1

1) Pour tout $\theta \in \mathbf{R}$, soit $C_{\theta}$ le segment du plan d’extrémités $(0,0)$ et (cos(2$\pi \theta )$, sin(2$\pi \theta ))$; posons

C = $\bigcup C_{\theta}$.

$\theta \in \mathbf{Q}\cap [1/6,1/4]$

a) L’espace C est contractile en 0, mais en aucun autre point.

b) Soit D la réunion des translatés $(0, n) + C$ de C, pour $n\in \mathbf{Z}$. Démontrer que l’espace D est homéotope à un point mais qu’il n’est contractile en aucun de ses points.

2) Soit B une partie de $\mathbf{R}^n$, soit $a$ un point intérieur à B; notons S la frontière de B. Supposons que B soit étoilée en $a$ et que toute demi-droite d’origine $a$ rencontre S en un point unique. Soit $f:\mathbf{R}_+^*\times S\rightarrow \mathbf{R}^n-\{a\}$ l’application définie par $f(t, y) =ty+ (1-t)a$. Démontrer que $f$ est un homéomorphisme tel que $f(]0,1]\times S) = B-\{a\}$ et $f(\{1\} \times S) = S$.

Ce résultat s’applique notamment lorsque B est un ensemble convexe, fermé et borné de $\mathbf{R}^n$ et $a$ un point adhérent à B (cf. I, p. 123, prop. 2 et EVT, II, p. 15, prop. 16).

3) Soit X l’espace topologique obtenu à partir de l’espace $\mathbf{R}$ par contraction du sous-ensemble $\mathbf{Q}($III, p. 252, déf. 10). La surjection canonique $p:\mathbf{R}\rightarrow X$ n’est ni ouverte ni fermée.

4) Soit X l’intervalle $[-1,1]$ de $\mathbf{R}$ et soit A = X $-\{0\}$. L’application canonique de X sur $X/A$ est une homéotopie mais il n’existe pas d’homotopie $\sigma$ d’origine Id$_X$ vérifiant les hypothèses de la prop. 10 de III, p. 252.

5) Soit A l’adhérence dans $\mathbf{R}$ de l’ensemble des nombres réels de la forme $1/n$, où $n$ parcourt l’ensemble des entiers $\geqslant$ 1. Soit $i$ l’injection canonique de A dans $\mathbf{R}$. L’application canonique de Côn$(i)$ sur $\mathbf{R}/A$ n’est pas une homéotopie.

6) Soit X un espace topologique métrisable de type dénombrable. On dit que X est un rétracte absolu [^1] si pour tout espace topologique métrisable de type dénombrable Y et toute partie fermée B de Y, toute application continue $f: B\rightarrow X$ s’étend en une application continue de Y dans X.

a) Soit X un espace topologique métrisable de type dénombrable. Pour que X soit un rétracte absolu, il faut et il suffit que, pour tout espace métrisable de type dénombrable Y et toute application continue, injective et fermée $f$ de X dans Y, il existe une application continue $g: Y\rightarrow X$ telle que $g\circ f=$ Id$_X$. b) Démontrer que les espaces $\mathbf{I}$ et $\mathbf{R}$ sont des rétractes absolus.

c) Démontrer que l’espace produit d’une famille dénombrable de rétractes absolus est un rétracte absolu.

d) Soit X un rétracte absolu, soit A un sous-espace de X qui est un rétracte de X. Démontrer que A est un rétracte absolu.

7) Soit X un espace topologique métrisable de type dénombrable. On dit que X est un rétracte absolu de voisinage si pour tout espace topologique métrisable de type dénombrable Y et toute partie fermée B de Y, toute application continue $f: B\rightarrow X$ s’étend en une application continue d’un voisinage de B dans X.

a) Soit X un espace topologique métrisable de type dénombrable. Pour que X soit un rétracte absolu de voisinage, il faut et il suffit que pour tout espace métrisable de type dénombrable Y et toute application continue, injective et fermée $f$ de X dans Y, il existe un voisinage U de $f(X)$ et une application continue $g: U\rightarrow X$ tels que $g\circ f=$ Id$_X$.

b) Soit X un rétracte absolu de voisinage et soit A une partie de X. Si A possède un voisinage U dont il est rétracte, alors A est un rétracte absolu de voisinage. En particulier, tout ouvert de X, tout rétracte de X, est un rétracte absolu de voisinage. c) Démontrer que l’espace produit d’une famille finie de rétractes absolus de voisinage est un rétracte absolu de voisinage.

d) Démontrer que la sphère $\mathbf{S}_n$ est un rétracte absolu de voisinage.

e) Soit X un espace topologique métrisable de type dénombrable, soient $A_1$ et $A_2$ des parties fermées de X telles que $X = A_1\cup A_2$. On suppose que $A_1\cap A_2$ est un rétracte absolu de voisinage. Pour que X soit un rétracte absolu de voisinage, il faut et il suffit qu’il en soit de même de $A_1$ et de $A_2$.

f) Soit X un espace topologique métrisable de type dénombrable. Si X est réunion de deux parties ouvertes qui sont des rétractes absolus de voisinage, alors X est un rétracte absolu de voisinage.

g) Soit X un espace topologique métrisable de type dénombrable dont tout point possède un voisinage qui est un rétracte absolu de voisinage. Démontrer que X est un rétracte absolu de voisinage.

8) Soit X un espace topologique métrisable ; soit $d$ une distance qui définit sa topologie. Soit $\mathscr{C}_b(X;\mathbf{R})$ l’espace vectoriel des fonctions à valeurs réelles sur X qui sont continues et bornées ; on le munit de la norme définie par $\|f\|=$ sup$_{x\in X}|f(x)|$ pour $f\in \mathscr{C}_b(X;\mathbf{R})$.

a) On définit une application $j: X\rightarrow \mathscr{C}_b(X;\mathbf{R})$ en posant $j(x):y\mapsto$ $d(x, y)/(1 +d(x, y))$. Démontrer que l’application $j$ induit un homéomorphisme de X sur son image.

b) Soit V l’intersection de toutes les parties convexes de $\mathscr{C}_b(X;\mathbf{R})$ qui contiennent $j(X)$. Démontrer que $j(X)$ est fermé dans V.

c) Soit X un espace métrisable de type dénombrable. Démontrer qu’il existe une partie convexe Z de $\mathbf{I}^{\mathbf{N}}$ telle que X soit homéomorphe à une partie fermée de Z.

9) Si X et Y sont des espaces topologiques et $\mathscr{U}$ un ensemble de parties de X, on dit que des applications $f, g: Y\rightarrow X$ sont $\mathscr{U}$ -proches si pour tout point $y\in Y$, il existe $U\in \mathscr{U}$ tel que $f(y)$ et $g(y)$ appartiennent à U ; on dit qu’une homotopie $\sigma : Y\times \mathbf{I}\rightarrow X$ est $\mathscr{U}$ -petite si pour tout point $y\in Y$, il existe $U\in \mathscr{U}$ tel que $\sigma (y, t)\in U$ pour tout $t\in \mathbf{I}$.

Soit X un sous-espace fermé d’une partie convexe Z de $\mathbf{I}^{\mathbf{N}}($cf. exercice 8) ; on suppose que X est un rétracte absolu de voisinage.

a) Soit $\mathscr{U}$ un recouvrement de X par des parties ouvertes de $\mathbf{I}^{\mathbf{N}}$. Démontrer qu’il existe une famille $\mathscr{V}$ de parties ouvertes et convexes de $\mathbf{I}^{\mathbf{N}}$ telle que, pour tout ouvert $v\in \mathscr{V}$, il existe un ouvert $u\in \mathscr{U}$ tel que $v\cap X\subset u$, et une rétraction continue $r$ de l’injection canonique de X dans la réunion V de la famille $\mathscr{V}$. b) Soit Y un espace topologique et soit B un sous-espace fermé de Y. Soient $f, g: Y\rightarrow X$ des applications continues qui sont $\mathscr{V}$ -proches, soit $\sigma : B\times \mathbf{I}\rightarrow X$ une homotopie $\mathscr{V}$ -petite dont l’origine est égale à $f|_B$.

Démontrer qu’il existe un voisinage W de B dans Y et une application continue $h$ du sous-espace $(Y\times  \{0,1\})\cup (W\times \mathbf{I})$ de $Y\times \mathbf{I}$. dans X telle que $h(y,0) =f(y)$ et $h(y,1) =g(y)$ pour tout $y\in Y$, et $h(y, t) =\sigma (y, t)$ pour tout $y\in B$ et tout $t\in \mathbf{I}$. Démontrer qu’il existe un voisinage $W'$ de B contenu dans W tel que $h|W'\times \mathbf{I}$ soit une homotopie $\mathscr{V}$ -petite.

c) Soit $u: Y\rightarrow \mathbf{I}$ une application continue telle que $u(y) = 1$ pour $y\in B$ et $u(y) = 0$ au voisinage de Y-W ; poser

$\{(1-u(y))((1-t)f(y) +tg(y)) +u(y)h(y, t)$ si $y\in V$

$$
h'(y, t) =
$$

$(1-t)f(y) +tg(y)$ sinon.

Démontrer que $h'$ est continue et que son image est contenue dans V.

d) En déduire qu’il existe une homotopie $\widetilde{\sigma}: Y\times \mathbf{I}\rightarrow X$ d’origine $f$, de terme $g$, et qui est $\mathscr{U}$ -petite.

10) Soit X un espace topologique. On suppose qu’il existe un recouvrement ouvert $\mathscr{U}$ de X tel que pour tout espace topologique Y et tout sous-espace fermé B de Y, deux applications $f_0, f_1$ de Y dans X qui sont $\mathscr{U}$ -proches sont homotopes s’il existe une homotopie $\mathscr{U}$ -petite reliant $f_0|B$ à $f_1|B$.

a) Soit $a$ un point de X et soit U un élément de $\mathscr{U}$ tel que $a\in U$. Démontrer qu’il existe une homotopie $\sigma : U\times \mathbf{I}\rightarrow X$ tel que $\sigma (x,0) =a,\sigma (x,1) =x$ et $\sigma (a, t) =a$ pour tout $x\in X$ et tout $t\in \mathbf{I}$.

b) Soit V un voisinage ouvert de $a$ tel que $\sigma (V\times \mathbf{I})\subset U$. Démontrer que V est un rétracte absolu de voisinage.

c) Démontrer que X est un rétracte absolu de voisinage.

11) Soit X un rétracte absolu de voisinage.

a) Démontrer que X est « semi-localement contractile », c’est-à-dire que tout point $x$ de X possède un voisinage V tel que l’injection canonique de $(V, x)$ dans X soit strictement homotope à l’application constante d’image $x$. (Utiliser l’exercice 9.)

b) Soit A un espace topologique compact. Démontrer que les composantes connexes par arcs de l’espace $\mathscr{C}_c(A; X)$ sont ouvertes.

c) Démontrer que X est localement connexe par arcs.

12) Soient X et Y des espaces topologiques ; on dit que la propriété d’extension des homotopies vaut pour les applications continues de but X et de source Y si pour toute application continue F: Y $\rightarrow X$, tout sous-espace fermé B de Y et toute homotopie $\sigma : B\times \mathbf{I}\rightarrow X$ d’origine $F|B$, il existe une homotopie $\widetilde{\sigma}: Y\times \mathbf{I}\rightarrow X$ d’origine F qui prolonge $\sigma$.

a) Soit X un espace topologique qui est un rétracte absolu de voisinage. Démontrer que la propriété d’extension des homotopies vaut pour les applications continues de but X et de source un espace métrisable de type dénombrable.

b) Démontrer l’équivalence des deux propriétés suivantes :

(i) L’espace X est un rétracte absolu de voisinage ;

(ii) Tout point de X possède un voisinage V tel que pour tout espace topologique métrisable de type dénombrable Y, tout sous-espace fermé B de Y, toute application continue de B dans V s’étend en une application continue de Y dans X.

c) On suppose que X est semi-localement contractile (cf. exercice 9) et que la propriété d’extension des homotopies vaut pour les applications continues de but X. Démontrer que X est un rétracte absolu de voisinage. [^2]

d) Démontrer que l’espace $X =\mathbf{Q}$ n’est pas un rétracte absolu de voisinage mais que la propriété d’extension des homotopies vaut pour les applications continues de but X.

13) Soit X un espace topologique qui est un rétracte absolu de voisinage. Soit A une partie de X telle que l’injection canonique de A dans X soit une homéotopie et une cofibration. Il existe une contraction de X sur A.

14) Soit X l’espace topologique $\mathbf{I}$ et posons $A =\{0,1\}$. Démontrer qu’il existe une homotopie reliant l’application identique de X à une application constante mais que l’application canonique $X\rightarrow X/A$ n’est pas une homéo-topie.

15) Soit X le sous-espace de $[0,1]\times [0,1]$ formé des couples $(x, y)$ tels que $x\in  \{0,1\}$, ou $y\in  \{0,1\}$, ou $x= 0\not$ et $1/x\in \mathbf{N}$. Soit $A =\{0\} \times [0,1]$. Démontrer que l’application canonique de X sur $X/A$ n’est pas une homéotopie, bien que A soit contractile.

16) Soient X et Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. Notons $\varphi : C(X)\rightarrow$ Côn$(f)$ l’application canonique. Démontrer que les espaces $Y/f(X)$ et Côn$(f)/\varphi (C(X))$ sont homéomorphes.

17) Soit X un espace topologique et soit A un sous-espace de X. Notons $i: A\rightarrow X$ et $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ les injections canoniques. a) On suppose que $X =\mathbf{R}$ et $A = ]0,1[$; démontrer que l’application $j$ n’est pas stricte.

b) Supposons que tout point de X a une base dénombrable de voisinages fermés. Pour que l’application $j$ soit stricte, il faut et il suffit que A soit fermé. c) On suppose que A est la demi-droite d’Alexandroff (TG, IV, p. 49, exerc. 12) et que X est son compactifié d’Alexandroff. Montrer que l’application $j$ est stricte bien que A ne soit pas fermé dans X.

18) On dit qu’un espace topologique X est localement équiconnexe si l’application diagonale de X dans $X\times X$ est une cofibration.

a) Démontrer que le produit d’une famille finie d’espaces localement équiconnexes est localement équiconnexe.

Soit X un espace localement équiconnexe.

b) Démontrer qu’il existe un recouvrement de X par une suite $(U_n)_{n\in\mathbf{N}}$ de parties ouvertes de X telles que, pour tout $n$, l’injection de $U_n$ dans X soit homotope à une application constante.

c) Démontrer que X est séparé.

d) Soit $u: X\rightarrow \mathbf{I}$ une application continue et soit U l’ensemble des points $x\in X$ tels que $u(x)>0$. Démontrer que les composantes connexes par arcs de U sont ouvertes. En particulier, les composantes connexes par arcs de X sont ouvertes.

e) Soit A un sous-espace fermé de X qui est un rétracte de X. Démontrer que A est localement équiconnexe et que le couple $(X,A)$ possède la propriété d’extension des homotopies. (« Théorème de Dyer et Eilenberg ».)

f) Soit A un sous-espace de X tel que le couple $(X,A)$ possède la propriété d’extension des homotopies. Démontrer que A est localement équiconnexe.

19) Soit B un espace topologique, soit $u: X\rightarrow \mathbf{I}$ une application continue et soit $A =\overset{-1}{u}(0)$.

a) Démontrer que l’application $p$ de $X\times \mathbf{I}$ dans lui-même donnée par $p(x, t) = (x, tu(x))$ est fermée.

b) Soit Y un espace topologique et soit $\sigma : X\times \mathbf{I}\rightarrow Y$ une homotopie fixe sur A. Soit $\tau : X\times \mathbf{I}\rightarrow Y$ l’application donnée par $\tau (x, t) =\sigma (x$, inf(1$, t/u(x)))$ si $u(x)>0$ et $\tau (x, t) =\sigma (x,1)$ sinon. Démontrer que $\tau$ est continue.

c) Soit C un sous-espace de X; on suppose que le couple $(X,C)$ jouit de la propriété d’extension des homotopies. Soit $f: X\rightarrow Y$ une application continue et soit $\sigma : C\times \mathbf{I}\rightarrow Y$ une homotopie d’origine $f|C$ qui est fixe sur $A\cap C$. Démontrer qu’il existe une homotopie $\tau : X\times \mathbf{I}\rightarrow Y$ d’origine $f$ qui prolonge $\sigma$ et qui est fixe sur A.

20) Soit X un espace topologique et soient A, B et C des sous-espaces fermés de X tels que $A = B\cap C$.

a) Si les couples $(X,B)$, $(X,C)$ et $(X,A)$ jouissent de la propriété d’extension des homotopies, démontrer qu’il en est de même du couple $(X,B\cup C)$.

b) On suppose que les couples $(X,A)$ et $(X,B\cup C)$ jouissent de la propriété d’extensions des homotopies. Démontrer qu’il en est de même des couples $(X,B)$ et $(X,C)$.

c) On suppose que X est un espace normal et que $A\subset \mathring{B}\cup \mathring{C}$. Si les couples $(X,B)$ et $(X,C)$ jouissent de la propriété d’extensions des homotopies, démontrer qu’il en est de même du couple $(X,A)$.

21) Soit X un espace topologique paracompact, soit $\mathscr{A}$ un ensemble de parties fermées de X tel que $B\cap C\in \mathscr{A}$ pour tout couple $(B,C)$ d’éléments de $\mathscr{A}$. Soit $A =\bigcup_{C\in\mathscr{A}}C$; on suppose que, pour tout point $x$ de X, il existe un voisinage V de $x$ et une partie finie $\mathscr{A}_x$ de $\mathscr{A}$ tels que $V\cap A = V\cap \bigcup_{C\in\mathscr{A}_x}C$. a) Démontrer que A est une partie fermée de X.

b) On suppose que, pour tout $B\in \mathscr{A}$, le couple $(X,B)$ jouit de la propriété d’extension des homotopies. Démontrer qu’il en est de même du couple $(X,A)$.

22) Soient X et Y des espaces topologiques, soit A un sous-espace de X et soit B un sous-espace de Y.

a) On suppose que les couples $(X,A)$ et $(Y,B)$ sont homéotopes. Si le couple $(X,A)$ jouit de la propriété d’extension des homotopies, démontrer qu’il en est de même du couple $(Y,B)$.

b) On suppose inversement que les couples $(X,A)$ et $(Y,B)$ jouissent de la propriété d’extension des homotopies. Soit $f: X\rightarrow Y$ une homéotopie qui induit, par passage aux sous-espaces, un homéomorphisme de A sur B. Prouver que $f$ est une homéotopie du couple $(X,A)$ sur le couple $(Y,B)$.

23) Soient X et Y des espaces topologiques. On dit qu’une homotopie $\sigma : X\times$ $\mathbf{I}\rightarrow Y$ est stationnaire s’il existe un nombre réel $\delta  >0$ tel que $\sigma (x, t) =\sigma (x,0)$ pour tout $x\in X$ et tout $t\in [0, \delta ]$. Soit A un sous-espace fermé de X ; on note $j$ l’injection canonique de A dans X. On dit que le couple $(X,A)$ possède la propriété d’extension des homotopies stationnaires si, pour tout espace topologique Y, toute application continue $f: X\rightarrow Y$ et toute homotopie stationnaire $\sigma : A\times \mathbf{I}\rightarrow Y$ dont l’origine est égale à $f|A$, il existe une homotopie $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Y$ d’origine $f$ qui étend $\sigma$.

a) Démontrer que les propriétés suivantes sont équivalentes :

(i) Le couple $(X,A)$ a la propriété d’extension des homotopies stationnaires ;

(ii) Les couples $(X,A)$ et (Cyl($j$)$, \alpha_j(A\times  \{0\})$ sont homéotopes ;

(iii) Il existe une application continue $\varphi : X\rightarrow \mathbf{I}$ telle que $\varphi (a) = 0$ pour tout $a\in A$ et une homotopie $\sigma : X\times \mathbf{I}\rightarrow X$ telle que $\sigma (x,0) =x$ pour $x\in X$, $\sigma (a, t) =a$ pour $(a, t)\in A\times \mathbf{I}$, et $\sigma (x,1)\in A$ si $\varphi (x)<1$.

(iv) Il existe une application continue $\varphi : X\rightarrow \mathbf{I}$, un sous-espace V de X et une homotopie $\sigma : V\times \mathbf{I}\rightarrow X$ tels que $\varphi (x) = 1$ si $x\notin V,\varphi (a) = 0$ pour $a\in A,\sigma (x,0) =x$ pour $x\in V,\sigma (a, t) =a$ pour $(a, t)\in A\times \mathbf{I},\sigma (x,1)\in A$ si $\varphi (x)<1$.

b) On suppose que le couple $(X,A)$ possède la propriété d’extension des homotopies stationnaires et qu’il existe une fonction continue $u: X\rightarrow \mathbf{I}$ telle que $\overset{-1}{u}(0) = A$. Démontrer que le le couple $(X,A)$ possède la propriété d’extension des homotopies.

24) Soit M un ensemble non dénombrable, soit X l’espace $\mathbf{I}^M$ et soit A le sous-espace $\{0\}^M$ de X.

a) Démontrer que le couple $(X,A)$ a la propriété d’extension des homotopies stationnaires (exerc. 23).

b) Démontrer que le couple $(X,A)$ n’a pas la propriété d’extension des homotopies. (Prouver que l’ensemble A n’est pas l’intersection d’une famille dénombrable d’ouverts.)

c) Démontrer que le couple $(X\times \mathbf{I},X\times  \{0\} \cup A\times \mathbf{I})$ n’a pas la propriété d’extension des homotopies stationnaires.

25) a) Soient X et Y des espaces topologiques, soit A un sous-espace fermé de X et soit B un sous-espace fermé de Y. Soit $f: X\rightarrow Y$ une application continue ; on suppose que $f$ induit, par passage aux sous-espaces, un homéo-morphisme de A sur B. Si $f$ possède un inverse à gauche à homéotopie près et si $(Y,B)$ possède la propriété d’extension des homotopies stationnaires (exerc. 23), il en est de même de $(X,A)$.

b) Si les couples $(X,A)$ et $(Y,B)$ sont homéotopes, alors $(X,A)$ a la propriété d’extension des homotopies stationnaires si et seulement s’il en est de même de $(Y,B)$.

c) Soit C l’ensemble des points du plan de la forme $(t/n, t)$, pour $t\in \mathbf{I}$ et $n\in \mathbf{N}^*$, soit X son adhérence et soit $A =\{0\} \times \mathbf{I}$. Démontrer que le couple $(X,A)$ ne possède pas la propriété d’extension des homotopies stationnaires.

26) On munit l’ensemble $X =\{0,1\}$ de la topologie pour laquelle les ensembles ouverts sont $\emptyset ,\{0\}$ et X. On pose $A =\{0\}$. Démontrer que le couple $(X,A)$ possède la propriété d’extension des homotopies mais que le couple $(X\times X,(X\times A)\cup (A\times X))$ ne la possède pas.

27) Soit X un espace topologique et soit A un sous-espace (non nécessairement fermé) de X ; on note C le sous-espace $(X\times  \{0\})\cup (A\times \mathbf{I})$ de $X\times \mathbf{I}$. On suppose que C est un rétracte de $X\times \mathbf{I}$. Soit U une partie de C telle que $U\cap (X\times \{0\})$ et $U\cap (A\times \mathbf{I})$ soient ouverts dans $X\times \{0\}$ et $A\times \mathbf{I}$ respectivement. a) Soit $V_0$ l’ensemble des $x\in X$ tels que $(x,0)\in U$ ; pour $n\geqslant 1$, soit $V_n$ la réunion des ouverts W de X tels que $(W\cap A)\times [0,1/n[$ soit contenu dans U.

Démontrer que $A\cap V_0=\bigcup_{n\geqslant 1}A\cap V_n$; prouver aussi que tout ouvert W de X tel que $W\cap A\subset V_n$ est contenu dans $V_n$.

b) Démontrer que $V\subset \bigcup_{n\geqslant 1}V_n$.

c) Démontrer que U est ouvert dans C.

d) Démontrer que le couple $(X,A)$ possède la propriété d’extension des homotopies.

28) Soit X un espace topologique, soit A un sous-espace de X tel que le couple $(X,A)$ possède la propriété d’extension des homotopies. Démontrer qu’il en est de même du couple $(X,A)$.

29) Soit B un espace topologique. On dit qu’un recouvrement $(V_i)_{i\in I}$ de B est numérique s’il existe une partition continue de l’unité $(g_j)_{j\in J}$ sur B, localement finie, telle que pour tout $j\in J,\overset{-1}{g_{j}}(]0,1])$ est contenu dans l’un des $V_i$.

a) Démontrer que B est paracompact si et seulement si tout recouvrement ouvert de B est numérique.

b) Démontrer que B est normal si et seulement si tout recouvrement ouvert localement fini de B est numérique.

c) Soit $(V_i)$ un recouvrement numérique de B, soit $B'$ un espace topologique et soit $f: B'\rightarrow B$ une application continue. Démontrer que le recouvrement $(\overset{-1}{f}(V_i))$ de $B'$ est numérique.

30) Soit B un espace topologique paracompact, soit F un espace topologique contractile, soit E un espace fibré localement trivial de base B et de fibre-type F. Démontrer que le faisceau des germes de sections continues de E est mou.

31) Soit B un espace topologique. Soient A et V des sous-espaces de B; on dit que V est un halo de A s’il existe une application continue $\varphi : B\rightarrow \mathbf{I}$ qui est égale à 1 en tout point A et à 0 en tout point de $\complement V$. On dit qu’un B-espace $(E, p)$ possède la propriété d’extension des sections si, pour tout sous-espace A de B, tout halo V de A et toute section $s$ de $E_V$, il existe une section $s'$ de E telle que $s'|A =s|A$. a) Soient $(E, p)$ et $(E', p')$ des B-espaces ; on suppose qu’il existe des morphismes de B-espaces, $f: E\rightarrow E'$ et $g: E'\rightarrow$ E, et une homotopie $\sigma : E\times \mathbf{I}\rightarrow E$ d’origine Id$_E$ et de terme $g\circ f$ telle que $p(\sigma (x, t)) =p(x)$ pour tout $(x, t)\in E\times \mathbf{I}$. Si le B-espace $E'$ possède la propriété d’extension des sections, il en est de même du B-espace E.

b) Soit E un B-espace et soit A un sous-espace de B qui est un rétracte de B. On suppose que le A-espace induit $E_A$ possède la propriété d’extension des sections ; démontrer qu’il en est de même du B-espace E.

c) Soit E un B-espace qui possède la propriété d’extension des sections. Soit

$f: B\rightarrow \mathbf{I}$ une application continue et soit $V =\overset{-1}{f}(]0,1])$. Démontrer que le V-espace $E_V$ possède la propriété d’extension des sections. (Soit A un sous-espace de V et soit W un halo de A dans V ; construire des suites $(A_n)$ et $(V_n)$ de sous-espaces de B vérifiant les propriétés suivantes : pour tout $n,A_n$ est contenu dans W, $V_n$ est un halo de $A_n$, et l’intersection des $A_n$ est égale à A.)

32) Soit B un espace topologique et soit $(E, p)$ un B-espace. Soit $(V_i)_{i\in I}$ un recouvrement numérique de B tel que, pour tout $i\in I$, le $V_i$-espace $E_{V_i}$ possède la propriété d’extension des sections.

a) On suppose qu’il existe une partition continue de l’unité $(f_i)$ sur B, localement finie, telle que $V_i=\overset{-1}{f_{i}}(]0,1])$ pour tout $i$. Soit $g: B\rightarrow [0,1]$ une application continue. On pose $A =\overset{-1}{g}(1)$ et $W =\overset{-1}{g}(]0,1])$ ; soit $s$ une section de E sur W. Démontrer qu’il existe une section de E qui coïncide avec $s$ sur A. (Considérer un élément maximal de l’ensemble des couples $(J, t)$, où J est une partie de I et $t$ est une section de E sur $W\cup \bigcup_{i\in J}V_i$ qui coïncide avec $s$ sur A, muni de la relation d’ordre donnée par $(J, t)\prec (J', t')$ si $J\subset J'$ et $t'$ prolonge $t.)$

b) Démontrer que le B-espace E possède la propriété d’extension des sections.

§2

1) Soit X un espace topologique et soient $x,y$ des points de X. Démontrer que les applications $p_x$ et $p_y$ constantes d’image respectivement $x$ et $y$ sont homotopes si et seulement si $x$ et $y$ appartiennent à la même composante connexe par arcs de X.

2) Soit S le graphe de la fonction de $]0,1]$ dans $\mathbf{R}$ donnée par $x\mapsto$ sin($\pi /x$); soit $\overline{S}$ son adhérence dans $\mathbf{R}^2$.

a) Démontrer que les espaces S et $\overline{S}$ sont connexes.

b) Démontrer qu’une partie connexe et compacte de $\overline{S}$ contenant les points $(1,0)$ et les points $(0,1)$ est nécessairement égale à S, mais qu’il n’existe pas d’homéomorphisme de $\mathbf{I}$ sur $\overline{S}$ appliquant 0 sur $(1,0)$ et 1 sur $(0,1)$.

c) Déterminer les composantes connexes par arcs de l’espace $\overline{S}$.

d) Démontrer que l’espace $\overline{S}$ n’est pas localement connexe.

3) Soit $a\in \overline{S}$. Démontrer que l’espace pointé $(S, a)$ possède un revêtement universel si et seulement si $a\in  \{0\} \times [-1,1]$.

4) Soit $D = [0,1]\cap (\mathbf{R}-\mathbf{Q})$.

a) Soit $\varphi$ une application de D dans $[0,1]$ et soit X le complémentaire dans $[0,1]^2$ de l’ensemble formé des $(x, \varphi (x))$ pour $x\in D$. Démontrer que X est connexe.

b) Démontrer qu’il existe une application bijective Φ de D sur l’ensemble des chemins d’origine $(0,0)$ et de terme $(1,1)$ dans $[0,1]^2$. Pour tout $x\in D$, soit $\psi (x)$ un point d’abscisse $x$ sur le chemin $\Phi (x)$. Soit alors Y le complémentaire dans $[0,1]^2$ de l’ensemble formé des $\psi (x)$ pour $x\in D$. Démontrer que l’espace Y est connexe, localement connexe mais qu’il n’est pas connexe par arcs.

5) Soit $r$ un élément de $\mathbf{N}\cup  \{\infty , \omega \}$, soient $n$ et $d$ des entiers, soit X une sous-variété de classe $C^r$ de $\mathbf{R}^n$, fermée, purement de dimension $d$.[^3]

a) Démontrer qu’il existe un voisinage U de X dans $\mathbf{R}^n$ et un isomorphisme de classe $C^r$ de $X\times ]-1; 1[^{n-d}$ sur U.

b) Tout chemin dans X est strictement homotope à un chemin de classe $C^r$. c) Si deux chemins de classe $C^r$ dans X sont homotopes, ils sont reliés par une homotopie de classe $C^r$.

6) Soit U un ouvert d’un espace numérique $\mathbf{R}^n$. On dit qu’un chemin $c:\mathbf{I}\rightarrow U$ est affine par morceaux s’il existe une suite finie $(t_0, . . . , t_n)$ telle que $0 =t_0< t_1<\cdots < t_n= 1$ et telle que la restriction de $c$ à chaque intervalle $[t_{i-1}, t_i]$ est affine. Démontrer que tout chemin dans U est strictement homotope à un chemin affine par morceaux.

7) a) Soit R un ensemble. Si S est une partie de R, on note $j_S$ l’application de $\mathbf{I}^S$ dans $\mathbf{I}^R$ qui applique une fonction $f: S\rightarrow \mathbf{I}$ sur l’unique fonction de R dans $\mathbf{I}$ dont la restriction à S égale $f$ et qui est nulle en tout point de R-S.

Démontrer que $j_S$ est un homéomorphisme de $\mathbf{I}^S$ sur le sous-espace de $\mathbf{I}^R$ formé des fonctions nulles hors de S.

b) Soit X l’ensemble des applications de R dans $\mathbf{I}$ qui sont nulles en dehors d’un sous-ensemble dénombrable de R. On note Y la limite inductive de la famille d’espaces $(\mathbf{I}^S)$, où S parcourt l’ensemble des parties dénombrables de R, et on le munit de la topologie limite inductive des topologies produits.

Les applications canoniques de $\mathbf{I}^S$ dans $\mathbf{I}^{\mathbf{R}}$ induisent une bijection continue $j$ de Y dans X. Cette bijection n’est pas un homéomorphisme si R n’est pas dénombrable.

c) Démontrer que, pour tout chemin $c:\mathbf{I}\rightarrow X$, il existe un sous-ensemble dénombrable S de R tel que $c(t)(s) = 0$ pour tout $t\in \mathbf{I}$ et tout $s\in R-S$. d) En déduire que l’application $j^{-1}$ est continue par arcs.

8) Soit X un espace topologique connexe compact de cardinal $\geqslant 2$. On suppose que pour tout couple $(x, y)$ de points distincts de X, l’espace X $\{x, y\}$ n’est pas connexe.

a) Démontrer que pour tout $x\in X$, l’espace X $-\{x\}$ est connexe.

b) Soient $a, b$ des points distincts de X et soient $U,V$ des parties ouvertes et fermées, non vides, de X telles que X$-\{a, b\}= U\cup V$. Démontrer que l’on a $U = U\cup  \{a, b\},V = V\cup  \{a, b\}$ et que ces ensembles sont connexes.

c) On suppose que X possède une partie dénombrable partout dense. Démontrer alors que X est homéomorphe au cercle $\mathbf{S}_1$. (Prouver qu’il existe un homéomorphisme de $\mathbf{I}$ sur $\overline{U}$ qui applique 0 sur $a$ et 1 sur $b.)$

9) Soit A un ensemble bien ordonné non dénombrable dont tout segment $[u, v]$ est dénombrable.

a) Démontrer que l’ensemble $L = A\times [0,1[$, totalement ordonné par l’ordre lexicographique et muni de la topologie $\mathscr{T}_0(L)$ (TG, I, p. 91, exerc. 5), est connexe (TG, IV, p. 48, exerc. 7). L’espace L est appelé droite d’Alexandroff. b) Démontrer que, pour tout point $x\in L$, l’espace topologique L$-\{x\}$ n’est pas connexe.

c) Soit $\overline{L}$ l’ensemble ordonné obtenu en adjoignant à L des points $-\infty$ et $+\infty$ tels que $-\infty < x <+\infty$ pour tout $x\in L$. Munissons-le de la topologie $\mathscr{T}_0(L)$; on l’appelle la droite d’Alexandroff achevée. Démontrer que $\overline{L}$ est compact et connexe.

d) Démontrer qu’il n’existe pas d’homéomorphisme de $[0,1]$ sur $\overline{L}$ qui applique 0 sur $-\infty$ et 1 sur $+\infty$.

10) Soit $\overline{L}$ la droite d’Alexandroff achevée et soit S l’espace topologique déduit de $\overline{L}$ par identification des points $-\infty$ et $+\infty$.

a) Démontrer que l’espace S est compact et connexe, de cardinal au moins 2.

b) Démontrer que pour tout couple $(x, y)$ de points distincts de S, l’espace topologique S $-\{x, y\}$ n’est pas connexe.

c) Démontrer que l’espace S n’est pas homéomorphe à un cercle.

11) a) Soit X l’espace quotient de l’espace $\mathbf{R}\times \{1,2\}$ par la relation d’équivalence la plus fine pour laquelle $(t,1)$ est équivalent à $(t,2)$ si $t\in \mathbf{R}^*$. Démontrer qu’il n’existe pas de chemin injectif dans X dont les extrémités soient les images des points $(0,1)$ et $(0,2)$.

b) Soit $c:\mathbf{I}\rightarrow \mathbf{S}^1$ le chemin défini par $c(t) =e^{3\pi it}$; il relie le point 1 au point $-1$. Démontrer qu’il n’y a pas de chemin injectif dans $\mathbf{S}_1$ qui soit strictement homotope au chemin $c$.

12) Soit X un espace paracompact dans lequel tout point possède un voisinage homéomorphe à un espace métrique complet. Démontrer qu’il existe une distance sur X, compatible avec sa topologie, qui en fait un espace métrique complet (cf. TG, IX, p. 110, exerc. 34).

13) Soit X un espace topologique séparé ; on suppose que tout point de X possède un voisinage U tel que tout couple de points de U soit relié par un chemin injectif dans U. Si X est connexe, démontrer (sans faire usage de la proposition 18 de III, p. 282) que X est connexe par arcs et que tout couple de points de X est relié par un chemin injectif.

14) Soit X un ensemble et soit $\mathfrak{c}$ un cardinal infini tel que $\mathfrak{c}<$ Card(X).

a) Soit $\mathscr{U}_{\mathfrak{c}}$ l’ensemble des parties V de X telles que Card(X-V) $\leqslant \mathfrak{c}$ ou $V =\emptyset$. Démontrer que $\mathscr{U}_{\mathfrak{c}}$ est une topologie sur X.

b) Montrer que l’ensemble X, muni de cette topologie, est connexe et localement connexe, mais que ses composantes connexes par arcs sont réduites à un élément.

c) Montrer que le cône C(X) est connexe par arcs, localement connexe, mais n’est pas localement connexe par arcs. Cela démontre que dans le corollaire 2 de III, p. 267, on ne peut omettre l’hypothèse que l’espace est localement compact et métrisable.

§3

1) Soit X un espace topologique, soit $\sigma : X\times \mathbf{I}\rightarrow X$ une homotopie dont l’origine et le terme sont égaux à l’application identique de X. Soit $x\in X$ et soit $\delta \in \pi_1(X, x)$ la classe du lacet $t\mapsto \sigma (x, t)$ en $x$. Démontrer que $\delta$ appartient au centre du groupe $\pi_1(X, x)$.

2) Soient $(X, a)$ et $(Y, b)$ des espaces topologiques pointés ; on suppose que le sous-espace $\{a\}$ de X est fermé et que le couple $(X,\{a\})$ possède la propriété d’extension des homotopies.

a) Soit $f: X\rightarrow Y$ une application continue et soit $c$ un chemin dans Y. Démontrer qu’il existe une homotopie $\sigma : X\times \mathbf{I}\rightarrow Y$ telle que $\sigma (a, t) =c(t)$ pour tout $t\in \mathbf{I}$ et $\sigma (x,0) =f(x)$ pour tout $x\in X$.

b) Démontrer qu’il existe une unique action à droite du groupe $\pi_1(Y, b)$ sur l’ensemble $[(X, a); (Y, b)]$ telle que $[f]\cdot [c]$ soit la classe de l’application $x\mapsto \sigma (x,1)$, pour toute application continue pointée $f: (X, a)\rightarrow (Y, b)$, tout lacet $c$ dans Y en $b$, et toute homotopie $\sigma$ comme ci-dessus.

c) On suppose que Y est connexe par arcs. Démontrer que toute application continue de X dans Y est homotope à une application continue pointée de $(X, a)$ dans $(Y, b)$.

d) Soient $f$ et $g$ des applications continues pointées de $(X, a)$ dans $(Y, b)$. Pour que $f$ et $g$ soient l’origine et le terme d’une homotopie pointée, il faut et il suffit qu’il existe une classe de lacet $\gamma \in \pi_1(Y, b)$ telle que $[f]\cdot \gamma = [g]$.

§4

1) On considère le revêtement $(E, p)$ introduit dans l’exercice 4 de I, p. 148. Démontrer qu’il n’est pas galoisien, mais que le sous-groupe $p_*(\pi_1(E, x))$ de $\pi_1(B, b)$ est distingué. Cela fournit un contre-exemple à la réciproque du théorème 1 (III, p. 305).

§5

1) Soit X un espace connexe par arcs, soit $x$ un point de $x$, et soit $\mathscr{U}= (U_i)$ un recouvrement ouvert de X ; pour tout $i$, soit $c_i$ la classe d’un chemin dans X d’origine un point $u_i$ de $U_i$ et de terme $x$. Notons $G_{\mathscr{U}}$ le plus petit sous-groupe distingué de $\pi_1(X, x)$ tel que Int($c_i$)$(G_{\mathscr{U}})$ contient la classe de tout lacet dans $U_i$ en $u_i$. Alors $G_{\mathscr{U}}$ est un sous-groupe ouvert de $\pi_1(X, x)$ pour la topologie admissible.

2) Soit X un espace topologique et soit $a$ un point de X. On dit qu’un sous-groupe H de $\pi_1(X, a)$ est adéquat si, pour tout $b\in X$ et toute classe de chemin $\gamma \in \varpi_{a,b}(X)$, il existe un voisinage V de $b$ tel que pour tout lacet $c\in \Omega_b(V)$, la classe du lacet $\gamma [c]\gamma^{-1}$ appartient à H.

a) Montrer qu’il existe une unique topologie de groupe sur $\pi_1(X, a)$ pour laquelle les sous-groupes adéquats sont les sous-groupes ouverts.

b) Montrer que cette topologie est plus fine que la topologie de la convergence compacte mais que ces deux topologies ont mêmes sous-groupes ouverts distingués.

c) Si X est localement connexe par arcs, la topologie adéquate et la topologie de la convergence compacte ont mêmes sous-groupes ouverts.

3) Soit C le cercle de diamètre $((0,0),(0,1))$ dans $\mathbf{R}^2$ et soit P la réunion des $2^nC$, pour $n\in \mathbf{Z}$. Soit E le quotient de l’espace $P\times \mathbf{R}$ par la relation d’équivalence la moins fine pour laquelle $(x, t)\sim (2x, t+ 1)$ pour tout $(x, t)\in$ $P\times \mathbf{R}$. Notons $p$ la surjection canonique de $P\times \mathbf{R}$ sur E. Soit $a$ le point $(0,0)$ de P et posons $e=p(a,0)$.

a) Montrer que $p$ fait de $P\times \mathbf{R}$ un revêtement galoisien de groupe $\mathbf{Z}$. Montrer que $p_*(\pi_1(P\times \mathbf{R},(a,0)))$ est un sous-groupe distingué ouvert de $\pi_1(E, e)$, de quotient $\mathbf{Z}$.

b) Soit $\varphi : P\rightarrow P$ l’application définie par $\varphi (x) =x$ si $x\in C$ et $\varphi (x) = (0,0)$ sinon. Montrer qu’elle est continue.

c) Montrer que le noyau de l’homomorphisme $\varphi_*=\pi_1(\varphi ,(a,0))$ est un sous-groupe de $\pi_1(P\times \mathbf{R},(a,0))$ qui est ouvert pour la topologie de la convergence compacte.

d) Soit $u:\mathbf{I}\rightarrow C$ le lacet donné par $t\mapsto \frac{1}{2}(1-$ cos(2$\pi t)$, sin(2$\pi t))$ et soit $c\in \Omega_e(E)$ le lacet donné par $t\mapsto (u(t),0)$. Montrer que l’image de $\varphi_*$ est un sous-groupe ouvert de $\pi_1(E, e)$ qui ne contient pas la classe du lacet $c$.

e) Soit $c_n:\mathbf{I}\rightarrow E$ le lacet défini par $c_n(t) =p(2^{-n}u(t),0)$ et soit $d:\mathbf{I}\rightarrow E$ le lacet donné par $t\mapsto p(a, t)$. Montrer que $d^nc_n\overline{d}^n$ est strictement homotope à $c$. En déduire que la classe $[c]$ est contenue dans tout sous-groupe admissible de $\pi_1(E, e)$.

f) Montrer que la topologie admissible sur $\pi_1(E, e)$ est strictement moins fine que la topologie de la convergence compacte.

4) Soit L la demi-droite d’Alexandroff (TG, IV, p. 49, exerc. 12) et soit $L^*$ son compactifié d’Alexandroff ; soit $\omega$ l’unique point de $L^*-$ L. Soit A un ensemble ayant au moins deux éléments et soit $a$ un point de A ; on pose $X = L^*\times A$ et Y = X $-\{(\omega , a)\}$.

a) Démontrer que l’injection canonique $j$ de Y dans X est étale, séparée, et possède la propriété de relèvement des chemins.

b) Démontrer que l’application $j$ ne fait pas de Y un revêtement de X.

5) Soit $X_0$ le cercle unité du plan numérique $\mathbf{R}^2$; soit $X_1$ la réunion des segments reliant le point $(1,0)$ aux points $(3,1/n)$, pour $n\in \mathbf{N}^*$; soit $X_2$ l’ensemble des points $(x, y)$ du plan tels que $(x-2)^2+y^2= 1$ et $y\leqslant 0$ ; on pose $X = X_0\cup X_1\cup X_2$.

a) Soit $Y = X\cup (-X)$. Soit $p: Y\rightarrow X$ l’application définie comme suit : on a $p$(cos($t$), sin($t$)) $=$ (cos(2$t)$, sin(2$t))$ pour $t\in \mathbf{R}$ et $p(z) =p(-z) =z$ pour $z\in X_1\cup X_2$. Démontrer que $p$ fait de Y un revêtement de degré 2 de X.

b) Soit $Z_2$ l’ensemble des points du plan tels que $(x-1)^2+y^2= 4$ et $y\leqslant 0$ ; on pose $Z = X_0\cup X_1\cup (-X_1)\cup Z_2\cup (-Z_2)$. Soit $q: Z\rightarrow X$ l’application définie par $q$(cos($t$), sin($t$)) $=$ (cos(2$t)$, sin(2$t))$ pour $t\in \mathbf{R},q(z) =q(-z) =z$ pour $z\in X_1$ et $q(z) =q(-z) = 1 +\frac{1}{2}z$ pour $z\in Z_2$. Démontrer que $q$ fait de Z un revêtement de degré 2 de X.

c) Démontrer que $q_*\pi_1(Z,(1,0)) =p_*\pi_1(Y,(1,0))$ mais qu’il n’existe pas d’application continue $f: Z\rightarrow Y$ telle que $p\circ f=q$.[^4]

6) Pour tout entier $n\geqslant 1$, on pose $x_n= (1/n,0)$ et on note $C_n$ le cercle du plan numérique de diamètre $(0, x_n)$. Soit P la réunion des espaces $C_n$, pour $n\in \mathbf{N}$ (« boucle d’oreille hawaïenne », cf. I, p. 146, exerc. 5) ; pour tout entier $n\geqslant 1$, on note $P_n$ la réunion des espaces $C_m$, pour $1\leqslant m\leqslant n$ et $P^n$ la réunion des espaces $C_m$, pour $m > n$.

a) Soit $n$ un entier $\geqslant 1$ et soit $r_n$ l’application de P dans $P_n$ qui applique un point $x\in P$ sur lui-même si $x\in P_n$, et sur 0 sinon. Démontrer que $r_n$ est une rétraction continue de l’injection canonique de $P_n$ dans P.

b) Démontrer que $P_n$ est localement contractile. En déduire que tout point de P distinct de l’origine a un voisinage contractile en ce point.

c) Démontrer que les inclusions canoniques de $P_n$ et $P^n$ dans P induisent un isomorphisme de groupes du produit libre $\pi_1(P_n,0)*\pi_1(P^n,0)$ sur $\pi_1(P,0)$. (Démontrer que l’injection canonique de $P^n$ dans le complémentaire $U_n$ de l’ensemble $\{x_1, . . . , x_n\}$ est une homéotopie. Appliquer alors la proposition 2 de IV, p. 422 au recouvrement $(P_n,U_n)$ de P.) d) Soit $\gamma \in \pi_1(P,0)$ une classe de lacets telle que $(r_n)_*(\gamma ) =\varepsilon_0$ pour tout entier $n\geqslant 1$ ; démontrer que $\gamma =\varepsilon_0$.

e) L’homomorphisme canonique de $\pi_1(P,0)$ dans lim$\leftarrow -_n\pi_1(P_n,0)$ déduit de la famille $((r_n)_*)$ est injectif et la topologie admissible sur $\pi_1(P,0)$ est l’image réciproque de la topologie de la limite projective sur lim$\leftarrow -_n\pi_1(P_n,0)$, les groupes $\pi_1(P_n,0)$ étant munis de la topologie discrète.

f) Démontrer que les composantes connexes par arcs de $\Omega_0(P)$ sont fermées, de même que celles de $\Omega_{(0,0)}(P\times P)$.

7) On reprend les notations de l’exercice 6.

a) Pour tout entier $n\geqslant 1$, soit $\alpha_n\in \pi_1(P,0)$ la classe d’un lacet dans $C_n$ dont la classe engendre $\pi_1(C_n,0)$. Posons alors $\beta_n=\alpha_1\alpha_n\alpha^{-1}_1\alpha^{-1}_n$ et $\gamma_n=\beta_n^n$. La suite $(\gamma_n)$ tend vers $\varepsilon_0$ pour la topologie admissible.

b) Soit $n\in \mathbf{N}^*$. Pour tout $c\in \Omega_0(P)$, on note $\omega_n(c)$ la borne supérieure des entiers $k$ tels qu’il existe une suite strictement croissante $(t_1, . . . , t_{2k})$ d’éléments de $\mathbf{I}$ tels que $c(t_{2i}) = 0$ et $c(t_{2i-1}) =x_n$ pour $i\in  \{1, . . . , k\}$. Prouver que $\omega_n(c)$ est un entier. Démontrer que l’application $\omega_n$ de $\Omega_0(P)$ dans $\mathbf{N}$ est semi-continue supérieurement.

c) Pour tout entier $n\geqslant 1$, soit $c_n$ un chemin dont la classe est $\gamma_n$. Démontrer que $\omega_1(c_n)\geqslant 4n$. En déduire que la suite $(c_n)$ n’a pas de limite dans $\mathscr{C}_c(\mathbf{I}; P)$. d) La topologie admissible sur le groupe $\pi_1(P,0)$ est séparée, non discrète, et strictement moins fine que la topologie de la convergence compacte. *L’espace P n’est en particulier pas délaçable.*

8) On reprend les notations des exercices 6 et 7; soit aussi $p: \Omega_0(P)\rightarrow$ $\pi_1(P,0)$ la surjection canonique.

a) Pour tout couple $(m, n)$ d’entiers $\geqslant$ 1 tels que $m=\not n$, on pose $\lambda_{m,n}= (\alpha_m\alpha_n\alpha^{-1}_m\alpha^{-1}_n)^{m+n}$ et $\lambda_{m,n}= (\alpha_1\alpha_m\alpha^{-1}_1\alpha^{-1}_m)^n$; soit S l’ensemble des couples de la forme $(\lambda_{m,n}, \mu_{m,n})$ dans $\pi_1(P,0)\times \pi_1(P,0)$. Démontrer que S n’est pas fermé mais que son image réciproque dans $\Omega_0(P)\times \Omega_0(P)$ l’est. En déduire que l’application $p\times p: \Omega_0(P)^2\times \pi_1(P,0)^2$ n’est pas stricte.

b) Soit T l’ensemble des classes de lacets de la forme $\lambda_{m,n}\mu_{m,n}$ dans $\pi_1(P,0)$. Démontrer que T est fermé.

c) Démontrer que la loi de composition de $\pi_1(P,0)$ n’est pas continue lorsqu’on munit le groupe $\pi_1(P,0)$ de la topologie quotient de la convergence compacte.[^5]

9) Reprenons les notations de l’exercice 6. Pour tout entier $n\in \mathbf{N}^*$, soit $c_n:\mathbf{I}\rightarrow C_n$ le lacet en l’origine défini par $t\mapsto \frac{1}{2n}(1-$ cos(2$\pi t)$, sin(2$\pi t))$.

a) Pour toute suite $\alpha \in  \{0,1\}^{\mathbf{N}^*}$, soit $c_{\alpha}$ l’application définie par $c_{\alpha}(0) = 0$ par $c_{\alpha}(t) =\alpha_nc_n(2^nt-1)$ pour tout entier $n\geqslant 1$ et tout $t\in \mathbf{I}$ tel que $2^{-n}\leqslant$ $t\leqslant 2^{1-n}$. Montrer que c’est un lacet en l’origine. Montrer que l’application $\alpha \mapsto [c_{\alpha}]$ de $\{0,1\}^{\mathbf{N}^*}$ dans $\pi_1(P,0)$ est injective.

b) Pour tout entier $n\geqslant 1$, soit $q_n$ l’application de P dans $C_n$ donnée par $q_n(x) =x$ si $x\in C_n$ et $q_n(x) = 0$ sinon. Elle est continue. Montrer que l’homomorphisme de groupes $\psi :\pi_1(P,0)\rightarrow \prod_{n\geqslant 1}\pi_1(C_n,0)$ donné par $\psi (\gamma ) = ((q_n)_*(\gamma ))_n$ admet une section.

10) Pour tout entier $n\geqslant$ 1, soit $C_n$ le cercle du plan numérique de centre $(1/n,0)$ et de rayon $1/n$; soit P la réunion des espaces $C_n$, pour $n\geqslant 1$. Pour tout entier $n\geqslant 1$, soit $B_n$ l’ensemble des points $(x, y)$ du plan tels que $(nx-1)^2+n^2y^2\leqslant 1\leqslant ((n+1)x-1)^2+(n+1)^2y^2$; soit B l’ensemble des points $(x, y)$ du plan tels que $(x-1)^2+y^2\leqslant 1$. Posons $B_0= P$ et soit A l’espace quotient de l’espace somme de la famille $(B_n)_{n\geqslant 0}$ par la relation d’équivalence la moins fine qui identifie $(b, n)$ et $(b,0)$ si $b\in C_n\cup C_{n+1}$.

a) Démontrer qu’il existe une unique application continue $p: A\rightarrow B$ qui, pour tout entier $n\geqslant 0$ et tout $b\in B_n$, associe le point $b$ à la classe de $(b, n)$. Démontrer que $p$ est bijective mais que ce n’est pas un homéomorphisme. b) Démontrer que l’espace A est localement connexe par arcs.

c) Soit $a$ la classe du point $(0,0)$. Démontrer que la topologie quotient de la topologie de la convergence compacte sur $\pi_1(A, a)$ est la topologie grossière. d) Démontrer que l’espace A est simplement connexe.

e) Soit $j$ l’application canonique de $C = B_0$ dans A. Démontrer que l’application $j_*:\pi_1(C,0)\rightarrow \pi_1(A, j(0))$ est surjective et que son noyau a la puissance du continu.

f) Démontrer que le groupe $\pi_1(A, j(0))$ a la puissance du continu. *En particulier, l’espace A n’est pas délaçable.*

[^1]: Cet exercice et les suivants reprennent les articles de K. Borsuk, « Sur les rétractes », Fund. Math. 17 (1931), p. 152–170 ; « Über eine Klasse von lokal zusammenhängenden Räumen », Fund. Math. 19 (1932), p. 220–242 ; O. Hanner, « Some theorems on absolute neighborhood retracts », Ark. Mat. 1, (1951), p. 389–408.
[^2]: K. Borsuk a construit un espace semi-localement contractile qui n’est pas un rétracte absolu de voisinage, voir « Sur un espace localement contractile qui n’est pas un rétracte absolu de voisinage », Fund. Math. 35, (1948), p. 175–180.
[^3]: D’après des théorèmes de Whitney et Grauert, toute variété de classe $C^r$, de dimension finie et dont la topologie est de type dénombrable est isomorphe à une sous-variété fermée d’un espace numérique.
[^4]: Cet exemple est dû à E. C. Zeeman.
[^5]: Cet exemple est dû à P. Fabel, « Multiplication is discontinuous in the Hawaiian earring group (with the quotient topology) », Bull. Polish Acad. Sci. Math. **59** (2011), p. 77-83.
