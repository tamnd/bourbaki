---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 2
section_title: Classification
lang: fr
source: ts-i-ii-fr
book_pages: A II.244-A II.250, A II.304-A II.308
pdf_pages: 0256-0262, 0316-0320
extraction: native
subsections:
    - "no": 1
      title: Groupes engendrés par une partie compacte
      page: 244
      pdf_page: 256
    - "no": 2
      title: Cas général
      page: 248
      pdf_page: 260
statements: 16
exercises: 14
content_sha256: d85cbf22c0db2c51875f7be3d59191d2cccf2b9a7c13aea75ecd2b3ccc64b4b0
---

## § 2. CLASSIFICATION

### 1. Groupes engendrés par une partie compacte

#### Lemme 1 {#ts-ii-s2-lem-1 .statement tag=02M9}

Soit H un groupe localement compact, et soit R l’un des groupes $\mathbf{R}$ ou $\mathbf{Z}$. Soit $\varphi$ un morphisme continu de R dans H. Si $\varphi$ n’est pas un isomorphisme topologique de R sur un sous-groupe de H, alors l’image de R dans H est relativement compacte.

Soit I l’image de $\varphi$. Quitte à remplacer H par $\overline{I}$, on peut supposer que I est dense dans H. On doit alors montrer que H est compact si $\varphi$ n’est pas un isomorphisme topologique de R sur I.

Supposons qu’il existe un voisinage V de $e$ dans H et un entier $M>0$ tels que, pour tout $t >M$ dans R, on ait $\varphi (t)\notin V$. Alors $\varphi$ est injective : si $\varphi (u) =e$, on a $\varphi (nu) =e$ pour tout entier $n\geqslant 1$, donc l’ensemble $\mathbf{N}u$ est borné dans R, ce qui signifie que $u= 0$. La restriction de $\varphi$ à $[-M,M]\cap R$ est donc un homéomorphisme sur son image, qui contient $V\cap I$. La restriction de $\varphi^{-1}$ à $V\cap I$ étant continue, il s’ensuit que $\varphi$ est un isomorphisme topologique de R sur I.

Supposons maintenant que $\varphi$ n’est pas un isomorphisme topologique de R sur I. Soient W un voisinage ouvert relativement compact de $e$ dans H, et V un voisinage symétrique de $e$ tel que $V^2\subset W$. Pour tout $x\in$ H = I, il existe un élément $s\in$ R tel que $x\in \varphi (s)V$. D’après l’alinéa précédent et l’hypothèse sur $\varphi$, il existe $t\in$ R tel que $t >|s|$ et $\varphi (t)\in V$. On a alors $x\in \varphi (t+s)\varphi (t)^{-1}V\subset \varphi (t+s)W$, et $t+s >0$. Par suite, les ensembles ouverts $\varphi (u)W$ pour $u >0$ forment un recouvrement ouvert de H. Comme W est relativement compact, il existe un entier $n\geqslant 1$ et des éléments $u_1, . . . , u_n$ de R, strictement positifs, tels que $W\subset \bigcup_{1\leqslant i\leqslant n}\varphi (u_i)W$. Soit U le plus grand des $u_i$.

Soit $x\in H$ et soit $s=$ inf$\{t\in R|t\geqslant 0,\varphi (t)x^{-1}\in \overline{W}\}$. Comme $\overline{W}$ est compact, on a alors $\varphi (s)x^{-1}\in \overline{W}$. Il existe un entier $i$ tel que $\varphi (s)x^{-1}\in \varphi (u_i)W$, d’où $\varphi (s-u_i)x^{-1}\in \overline{W}$. La définition de $s$ entraîne $s-u_i<0$, d’où $s\leqslant U$. Il en résulte que $H =\varphi ([0,U]\cap R)W$ est compact.

#### Lemme 2 {#ts-ii-s2-lem-2 .statement tag=02MA}

Si G est engendré par une partie compacte V, il existe un entier $n\geqslant 0$ et un sous-groupe discret D de G isomorphe à $\mathbf{Z}^n$ tels que $G/D$ soit compact.

Quitte à remplacer V par $V\cup V^{-1}$, on peut supposer que V est symétrique ; l’hypothèse signifie alors que G est la réunion des ensembles $V^n$ où $n\in \mathbf{N}$.

Comme $V^2$ est compact, il existe un entier $k\geqslant 1$ et des éléments $x_1, . . . , x_k\in G$ tels que $V^2\subset \bigcup_{1\leqslant i\leqslant k}x_iV$. Soit $D_0$ le sous-groupe de G engendré par la famille $(x_i)_{1\leqslant i\leqslant k}$. On a $V^2\subset D_0V$, d’où par récurrence $V^n\subset D_0V$ pour tout entier $n\geqslant 1$, et donc $G = D_0V$ puisque V engendre G. Soit alors J une partie de $\{1,2, . . . , k\}$ telle que le sous-groupe D engendré par la famille $(x_i)_{i\in J}$ soit topologiquement isomorphe à $\mathbf{Z}^{Card(J)}$, et maximale pour cette propriété. Montrons que $G/D$ est compact.

Soit $p$ la surjection canonique de G sur $G/D$. Soit $i\in  \{1,2, . . . , k\}-J$. Si le sous-groupe $H_i$ de $G/D$ engendré par $p(x_i)$ est topologiquement isomorphe à $\mathbf{Z}$, le sous-groupe de G engendré par D et $x_i$ est discret et l’application $(d, n)\mapsto dx^n_i$ est un isomorphisme de $D\times \mathbf{Z}$ sur ce sous-groupe, contrairement à la maximalité de J. Le lemme 1 entraîne donc que $\overline{H}_i$ est compact. Donc $G/D = (\prod_{i\notin J}\overline{H}_i)p(V)$ est compact

#### Lemme 3 {#ts-ii-s2-lem-3 .statement tag=02MB}

Soient A et B des groupes commutatifs tels que A est divisible. Soit C un sous-groupe de B et $\varphi$ un morphisme de C dans A. Il existe un morphisme de B dans A qui prolonge $\varphi$.

Soit $\mathscr{O}$ l’ensemble des couples $(X, f)$, où X est un sous-groupe de B contenant C et $f$ un morphisme de X dans A prolongeant $\varphi$. Ordonnons $\mathscr{O}$ par la relation « $X\subset X'$ et $f'$ prolonge $f$ ». On vérifie que $\mathscr{O}$ est inductif. Soit $(X, f)$ un élément maximal de $\mathscr{O}$ (E, III, p. 20 , th. 2). Si $X\not= B$, prenons un élément $b$ de B-X et soit $X'$ le sous-groupe engendré par X et $b$. La commutativité de B montre que $X'$ est l’ensemble des éléments $b^nx$ pour $n\in \mathbf{Z}$ et $x\in X$. Supposons d’abord que $b^n\notin X$ pour tout entier $n\not= 0$ et définissons $f'$ de $X'$ dans A en prenant un élément $y\in A$ arbitraire et en posant $f'(b^nx) =y^nf(x)$ pour tout $n\in \mathbf{Z}$ et tout $x\in X$. Comme A est commutatif, $f'$ est un morphisme, et il prolonge $f$. Supposons maintenant qu’il existe $n\not= 0$ tel que $b^n\in X$ et soit $m >0$ tel que $m\mathbf{Z}=\{n\in \mathbf{Z}|b^n\in X\}$. Puisque A est divisible, il existe un élément $y\in A$ tel que $y^m=f(b^m)$. On prolonge alors $f$ en un morphisme de $X'$ dans A par $f'(b^nx) =y^nf(x)$ pour $n\in  \{0,1, . . . , m-1\}$ et $x\in X$. Dans les deux cas, $(X, f)$ ne serait pas maximal. Donc on a X = B et le lemme est démontré.

#### Remarque {#ts-ii-s2-n1-rem-1 .statement tag=02MC}

Dans le langage des catégories, le lemme dit que les groupes divisibles sont des objets injectifs dans la catégorie des groupes commutatifs ; cf. A, VII, p. 53, exerc. 3.

#### Proposition 1 {#ts-ii-s2-prop-1 .statement tag=02MD}

Les conditions suivantes sont équivalentes :

(i) G est engendré par une partie compacte;

(ii) il existe des entiers positifs $p$ et $q$ et un groupe compact K tels que G soit isomorphe à $\mathbf{R}^p\times \mathbf{Z}^q\times K$;

(iii) il existe un entier $n\geqslant 0$ tel que $\widehat{G}$ est localement isomorphe à $\mathbf{R}^n$;

(iv) il existe des entiers positifs $p$ et $q$ et un groupe discret D tels que $\widehat{G}$ soit isomorphe à $\mathbf{R}^p\times \mathbf{T}^q\times D$.

(i) $=\Rightarrow$ (iii) : si G possède la propriété (i), il existe un entier $n\geqslant 0$ et un sous-groupe D de G isomorphe à $\mathbf{Z}^n$ tel que $G/D$ soit compact (lemme 2). Alors $D^{\bot}$, qui s’identifie au dual de $G/D$, est discret (th. 4 de II, p. 226 et prop. 18 de II, p. 233). Donc $\widehat{G}$ est localement isomorphe à $\widehat{G}/D^{\bot}$, c’est-à-dire à $\widehat{D}$, qui est isomorphe à $\mathbf{T}^n$ (th. 4 de II, p. 226 et prop. 18 de II, p. 233). Or $\mathbf{T}^n$ est localement isomorphe à $\mathbf{R}^n$.

(iii) $=\Rightarrow$ (iv) : si $\widehat{G}$ est localement isomorphe à $\mathbf{R}^n$, il existe un entier $p$ tel que $0\leqslant p\leqslant n$ de sorte que la composante neutre $\widehat{G}_0$ de $\widehat{G}$ soit un sous-groupe ouvert isomorphe à $\mathbf{R}^p\times \mathbf{T}^{n-p}$ (TG, VII, p. 13, th. 1). En particulier, $\widehat{G}_0$ est un groupe divisible. Appliquons alors le lemme 3 à l’application identique du sous-groupe $\widehat{G}_0$ du groupe $\widehat{G}$ dans le groupe divisible $\widehat{G}_0$. Il existe donc un morphisme $\pi$ de $\widehat{G}$ dans $\widehat{G}_0$ qui est l’application identique sur $\widehat{G}_0$. Par conséquent, on a $\pi \circ \pi =\pi$, et $\pi$ est un projecteur. Il est continu, puisque sa restriction au sous-groupe ouvert $\widehat{G}_0$ l’est. Par suite, $\widehat{G}$ est produit direct de $\widehat{G}_0$ et du sous-groupe $\overset{-1}{\pi}(e)$, qui est discret puisque isomorphe à $\widehat{G}/\widehat{G}_0$ (TG, III, p. 47, cor.)

(iv) $=\Rightarrow$ (ii) : découle de la prop. 2 de II, p. 206, de la prop. 18 de II, p. 233 et du corollaire 3 de II, p. 236.

(ii) $=\Rightarrow$ (i) : pour tout groupe compact K, le groupe $\mathbf{R}^p\times \mathbf{Z}^q\times K$ est engendré par l’ensemble compact $[0,1]^p\times  \{0,1\}^q\times K$.

#### Corollaire 1 {#ts-ii-s2-prop-1-cor-1 .statement tag=02ME}

Supposons que G soit engendré par un voisinage compact de $e$.

a) Il existe un sous-groupe compact K de G et des entiers positifs $p$ et $q$ tels que G soit isomorphe à $\mathbf{R}^p\times \mathbf{Z}^q\times K$.

b) Inversement, soient K un groupe compact, $p$ et $q$ des entiers positifs, et G un groupe isomorphe à $\mathbf{R}^p\times \mathbf{Z}^q\times K$. Alors K est l’unique sous-groupe compact maximal de G, et les entiers $(p, q)$ sont déterminés de manière unique par G.

L’assertion a) résulte de la prop. 1. Soit alors K un groupe compact, et $p,q$ des entiers positifs. Supposons que G soit isomorphe au groupe $\mathbf{R}^p\times \mathbf{Z}^q\times K$, et identifions G à ce groupe. Par la projection canonique de G sur $\mathbf{R}^p\times \mathbf{Z}^q$, l’image de tout sous-groupe compact de G est un sous-groupe compact de $\mathbf{R}^p\times \mathbf{Z}^q$, donc est réduit à l’élément neutre. Donc $K'\subset K$ et K est le plus grand sous-groupe compact de G. Le sous-groupe $\mathbf{R}^p\times K$ est aussi unique car $\mathbf{R}^p$ est la composante neutre de $G/K$. Compte tenu de TG, VII, p. 13, cor. 3, l’entier $p$ est déterminé de manière unique par G. Puisque $G/(\mathbf{R}^p\times K)$ est isomorphe à $\mathbf{Z}^q$, l’entier $q$ est également déterminé de manière unique par G.

#### Remarque {#ts-ii-s2-n1-rem-2 .statement tag=02MF}

Par dualité, $\widehat{G}$ est isomorphe à $\mathbf{R}^p\times \mathbf{T}^q\times D$ (prop. 3 (iv)) où les sous-groupes $\mathbf{R}^p\times \mathbf{T}^q$ et $\mathbf{T}^q$, et les entiers $p$ et $q$, sont déterminés de manière unique.

#### Corollaire 2 {#ts-ii-s2-prop-1-cor-2 .statement tag=02MG}

Les conditions suivantes sont équivalentes :

(i) Les groupes G et $\widehat{G}$ sont engendrés par des parties compactes ;

(ii) Il existe des entiers positifs $n$ et $m$ tels que G est localement isomorphe à $\mathbf{R}^m$ et $\widehat{G}$ à $\mathbf{R}^n$;

(iii) Il existe des entiers positifs $p,q$ et $r$ et un groupe fini A tels que G est isomorphe à $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$ ;

(iv) Il existe des entiers positifs $p,q$ et $r$ et un groupe fini A tels que $\widehat{G}$ est isomorphe à un produit $\mathbf{R}^p\times \mathbf{Z}^q\times \mathbf{T}^r\times A$.

On a (i) $\Leftrightarrow$ (ii) d’après la prop. 1, et (iii) $\Leftrightarrow$ (iv) par dualité, donc (iii) $\Rightarrow$ (i). Finalement, si (i) est vrai, alors $\widehat{G}$ est isomorphe à $\mathbf{R}^p\times \mathbf{T}^r\times D$ où D est discret (prop. 1). Le groupe D est engendré par une partie compacte, donc finie, de D. Par conséquent, il existe $q\geqslant 0$ tel que D soit isomorphe à $\mathbf{Z}^q\times A$, où A est un groupe fini (A, VII, p. 22, th. 3).

#### Remarque {#ts-ii-s2-n1-rem-3 .statement tag=02MH}

Avec les notations du cor. 2, si l’on identifie G à $\mathbf{R}^p\times$ $\mathbf{T}^q\times \mathbf{Z}^r\times A$, le sous-groupe $\mathbf{R}^p\times \mathbf{T}^q$ est la composante neutre de G, le sous-groupe $\mathbf{T}^q\times A$ est son plus grand sous-groupe compact et $\mathbf{T}^q$ est la composante neutre de celui-ci ; les entiers $p, q, r$ sont déterminés de manière unique par G d’après la remarque précédente, et le groupe A est déterminé par G à isomorphisme près.

#### Proposition 2 {#ts-ii-s2-prop-2 .statement tag=02MI}

Supposons G compact. Il existe une famille filtrante décroissante $(H_i)_{i\in I}$ de sous-groupes fermés de G tels que

a) le groupe G s’identifie à la limite projective des $G/H_i$;

b) pour tout $i$, il existe un entier $q\geqslant 0$ et un groupe fini A tels que $G/H_i$ est isomorphe à $\mathbf{T}^q\times A$.

En effet, $\widehat{G}$ est discret (prop. 18 de II, p. 233), donc réunion d’une famille filtrante croissante $(D_i)_{i\in I}$ de sous-groupes de type fini. Posons $H_i= D^{\bot}_i$ ; le groupe G s’identifie à la limite projective des $G/H_i($II, p. 234, cor. 3), et $(H_i)$ est une famille filtrante décroissante.

Soit $i\in I$. Il existe un entier $q\geqslant 0$ et un groupe fini A tels que le groupe $D_i$ est isomorphe à $\mathbf{Z}^q\times A$ (A, VII, p. 22, th. 3), donc $G/H_i$ est isomorphe à $\mathbf{T}^q\times \widehat{A}($cf. corollaire 1 de II, p. 232).

#### Corollaire {#ts-ii-s2-n1-cor-1 .statement tag=02MJ}

Si le groupe G est engendré par une partie compacte, alors il est limite projective de groupes isomorphes à des groupes de la forme $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, où A est un groupe fini et $p,q,r$ sont des entiers positifs.

D’après le (ii) de la prop. 1 de II, p. 246, le corollaire résulte de la prop. 2.

### 2. Cas général

Dans ce numéro, G désigne un groupe localement compact commutatif.

#### Proposition 3 {#ts-ii-s2-prop-3 .statement tag=02MK}

a) Il existe un entier $n\geqslant 0$ et un sous-groupe L tel que G est produit direct de L et d’un sous-groupe isomorphe à $\mathbf{R}^n$, et de plus L admet un sous-groupe ouvert compact K tel que $L/K$ est discret;

b) Le groupe G est réunion d’une famille filtrante croissante de sous-groupes ouverts, chacun étant limite projective de groupes isomorphes à des groupes de la forme $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, où A est un groupe fini et $p,q,r$ sont des entiers positifs.

Démontrons b). Pour tout voisinage compact V de $e$, notons $G_V$ le sous-groupe de G engendré par V. Il est ouvert, et d’après le corollaire de la prop. 2, le groupe $G_V$ est limite projective de groupes de la forme $\mathbf{R}^p\times \mathbf{T}^q\times \mathbf{Z}^r\times A$, où A est un groupe compact et $p,q$ et $r$ dans $\mathbf{N}$. Lorsque V parcourt les voisinages compacts de $e$, ces sous-groupes $G_V$ forment une famille filtrante (puisque $G_V$ et $G_W$ sont contenus dans $G_{V\cup W}$ pour tous voisinages compacts V et W de $e)$. Finalement, le groupe G est la réunion des sous-groupes $G_V$.

Soit H un sous-groupe ouvert de G engendré par un voisinage compact de $e$. Il existe un groupe compact K et des entiers positifs $p$ et $q$ tels que H est isomorphe à $\mathbf{R}^p\times \mathbf{Z}^q\times K$ (prop. 1 de II, p. 246) ; identifions H à ce produit. La surjection canonique de H sur le groupe divisible $\mathbf{R}^p$ se prolonge en un morphisme $\pi$ de G sur $\mathbf{R}^p$ (lemme 3 de II, p. 245). C’est un projecteur $\pi$ de G sur $\mathbf{R}^p$, qui est continu puisque sa restriction au sous-groupe ouvert H est continue. Donc G est produit direct de $\mathbf{R}^p$ et du noyau L de $\pi$ (TG, III, p. 47, cor.). On a $\mathbf{Z}^q\times K = H\cap L$, donc $\mathbf{Z}^q\times K$ est un sous-groupe ouvert de L. Ainsi K est un sous-groupe compact ouvert de L, et par conséquent $L/K$ est discret.

#### Proposition 4 {#ts-ii-s2-prop-4 .statement tag=02ML}

Soit $B_G$ l’ensemble des éléments de G qui engendrent un sous-groupe relativement compact de G. Alors $B_G$ est un sous-groupe fermé de G et $B^{\bot}_G$ est la composante neutre de $\widehat{G}$.

L’ensemble $B_G$ est un sous-groupe de G puisque le produit de deux parties compactes de G est une partie compacte de G.

Soit H un sous-groupe ouvert de G engendré par un voisinage compact de $e$. Il existe des entiers positifs $p$ et $q$ et un groupe compact K tel que le sous-groupe H soit isomorphe à $\mathbf{R}^p\times \mathbf{Z}^q\times K$ (prop. 1 de II, p. 246). Si l’on identifie ces groupes, on voit que $B_G\cap H = K$ est fermé dans H. Comme la famille des sous-groupes ouverts H engendrés par les voisinages compacts est un recouvrement ouvert de G (par exemple, $x$ appartient au sous-groupe engendré par $U\cap  \{x\}$ pour tout voisinage compact fixé U de $e)$, on en déduit que $B_G$ est fermé.

Calculons maintenant $B^{\bot}_G$. Par la prop. 3, a), il existe un entier positif $n\geqslant 0$ et un groupe L admettant un sous-groupe ouvert compact tel que G puisse s’identifier à $\mathbf{R}^n\times L$. Alors $B_G$ s’identifie à $\{0\} \times B_L$, et $B^{\bot}_G$ à $\mathbf{R}^n\times B^{\bot}_L$. On est donc ramené au cas où G = L admet un sous-groupe ouvert compact K.

On a alors $K\subset B_G$; si l’on identifie $G/\widehat{K}$ à $K^{\bot}$ (théorème 4 de II, p. 226), l’orthogonal $(B_G/K)^{\bot}$ de $B_G/K$ dans $\widehat{G}/K$ s’identifie à $B^{\bot}_G$. Mais d’autre part $B_G/K = B_{G/K}$, et comme $K^{\bot}$ est un sous-groupe ouvert de $\widehat{G}$ (cor. 2 de II, p. 233), la composante neutre $\widehat{G}_0$ de $\widehat{G}$ est également la composante neutre de $K^{\bot}$ (TG, III, p. 35, prop. 14). Donc l’assertion pour le groupe discret $G/K$ est équivalente à celle pour G.

Finalement, supposons que G est discret. Le groupe $\widehat{G}$ est alors compact (prop. 18 de II, p. 233). La composante neutre $(\widehat{G})_0$ est l’intersection des sous-groupes ouverts de $\widehat{G}$ (TG, III, p. 35, prop. 14) et un sous-groupe de $\widehat{G}$ est ouvert si et seulement si il est fermé et d’indice fini, ou encore si son orthogonal est fini (corollaire 2 de II, p. 233) ; le corollaire 4 de II, p. 228 montre que $(\widehat{G})^{\bot}_0$ est la réunion des sous-groupes finis de G, qui n’est autre que $B_G$ puisque G est discret. On conclut par dualité.

#### Corollaire 1 {#ts-ii-s2-prop-4-cor-1 .statement tag=02MM}

Supposons G compact. Alors les conditions suivantes sont équivalentes :

(i) Le groupe G est connexe;

(ii) Le groupe $\widehat{G}$ est sans torsion ;

(iii) Le groupe G est divisible.

Ceci résulte de la prop. 4 et du cor. 7 de II, p. 229 puisque $B_G= G$.

#### Corollaire 2 {#ts-ii-s2-prop-4-cor-2 .statement tag=02MN}

Supposons G compact. Alors G est totalement discontinu si et seulement si $\widehat{G}$ est un groupe de torsion.

Le groupe G est totalement discontinu si et seulement sa composante neutre est réduite à $\{e\}$; la prop. 4 montre que cette condition équivaut à $B_{\widehat{G}}=\widehat{G}$. Comme le groupe $\widehat{G}$ est discret (prop. 18 de II, p. 233), cela revient à dire que chaque élément de $\widehat{G}$ engendre un groupe fini, donc que $\widehat{G}$ est de torsion.

#### Corollaire 3 {#ts-ii-s2-prop-4-cor-3 .statement tag=02MO}

Si G est connexe, alors G est divisible.

En effet, il existe un groupe compact connexe K et un entier $n\geqslant 0$ tel que G est isomorphe à $\mathbf{R}^n\times K$ (II, p. 248, prop. 3, où on doit avoir L = K). Le corollaire 1 montre que K est divisible, et donc G est divisible.

## EXERCICES {#ts-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
