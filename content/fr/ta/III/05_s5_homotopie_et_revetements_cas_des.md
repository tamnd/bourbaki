---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 5
section_title: Homotopie et revêtements (cas des espaces localement connexes par arcs)
lang: fr
source: ta-i-iv-fr
book_pages: A III.308-A III.320, A III.334-A III.338
pdf_pages: 0324-0336, 0350-0354
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
exercises: 10
content_sha256: 05a8005752a7259f0a3387f624d400f50bd0040446bc44eecabcfbe739d7fa53
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

## EXERCICES {#ta-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
