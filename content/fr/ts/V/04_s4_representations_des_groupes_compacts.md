---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 4
section_title: Représentations des groupes compacts
lang: fr
source: ts-iii-v-fr
book_pages: TS V.456-TS V.482, TS V.504-TS V.516
pdf_pages: 0469-0495, 0517-0529
extraction: native
subsections:
    - "no": 1
      title: Semi-simplicité des représentations de dimension finie
      page: 456
      pdf_page: 469
    - "no": 2
      title: Représentations irréductibles
      page: 457
      pdf_page: 470
    - "no": 3
      title: Le théorème de Peter–Weyl
      page: 462
      pdf_page: 475
    - "no": 4
      title: Coefficients matriciels et fonctions G-finies
      page: 464
      pdf_page: 477
    - "no": 5
      title: Représentations dans un espace séparé quasi-complet
      page: 464
      pdf_page: 477
    - "no": 6
      title: Caractères et classes de conjugaison
      page: 466
      pdf_page: 479
    - "no": 7
      title: La cotransformation de Fourier
      page: 470
      pdf_page: 483
    - "no": 8
      title: La transformation de Fourier
      page: 471
      pdf_page: 484
    - "no": 9
      title: Indicateur de Frobenius–Schur et alternative de Larsen
      page: 476
      pdf_page: 489
statements: 54
exercises: 32
content_sha256: de6bb5480b1019f4ef8bd38dc3d7c88a01da27bcb3eba5fe1ff7bae49ed568f1
---

## § 4. REPRÉSENTATIONS DES GROUPES COMPACTS

Dans ce paragraphe, tous les espaces vectoriels topologiques considérés sont complexes, sauf mention explicite du contraire.

On fixe un groupe topologique compact G, dont on note $e$ l’élément neutre. Le groupe G est unimodulaire (INT, VII, p. 20, § 1, n$^o3$, cor. de la prop. 3). On note $\mu$ la mesure de Haar normalisée sur G (c’est-à-dire telle que $\mu(G) = 1)$ et pour $1\leqslant p\leqslant +\infty$, on note $\mathscr{L}^p(G)$ (resp. $L^p(G))$ l’espace $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (resp. l’espace $L^p_{\mathbf{C}}(G, \mu))$. Les convolutions seront toujours considérées relativement à la mesure $\mu$. Soit $p\in [1,+\infty ]$. On identifie $\mathscr{C}(G)$ à un sous-espace de $L^p$(G), ce qui est loisible puisque le support de $\mu$ est égal à G.

Pour toute représentation irréductible unitaire $\pi \in \widehat{G}$, on note $E_{\pi}$ l’espace de $\pi$.

### 1. Semi-simplicité des représentations de dimension finie

On rappelle (INT, VII, p. 71, § 3, n$^o1$, lemme 1) que pour toute représentation continue $\varrho$ de G dans un espace hilbertien E, il existe une forme hermitienne positive non dégénérée $q$ sur E telle que la structure d’espace vectoriel topologique de E définie par $q$ est identique à la structure initiale de E, et telle que $\varrho$ est une représentation unitaire de G dans l’espace hilbertien E muni du produit scalaire $q$.

#### Proposition 1 {#ts-v-s4-prop-1 .statement tag=03DN}

Soit $\varrho$ une représentation linéaire de dimension finie de G dans un espace vectoriel topologique séparé E. Il existe un produit scalaire $q$ sur E tel que $\varrho$ soit une représentation unitaire dans l’espace hilbertien E muni de $q$. En particulier, $\varrho$ est semi-simple.

Puisque E est de dimension finie, il existe une structure d’espace hilbertien sur E. Le résultat en découle en appliquant la remarque précédente et le corollaire 2 de V, p. 392.

#### Remarque {#ts-v-s4-n1-rem-1 .statement tag=03DO}

On verra plus loin (cor. 4 de V, p. 466) que toute représentation unitaire de G est semi-simple.

#### Corollaire {#ts-v-s4-n1-cor-1 .statement tag=03DP}

Soient $\varrho_1$ et $\varrho_2$ des représentations de dimension finie de G. Les représentations $\varrho_1$ et $\varrho_2$ sont isomorphes si et seulement si leurs caractères sont égaux.

Cela résulte de la proposition et du corollaire 3 de V, p. 392.

### 2. Représentations irréductibles

#### Lemme 1 {#ts-v-s4-lem-1 .statement tag=03DQ}

Toute représentation unitaire irréductible de G est de carré intégrable.

En effet, les coefficients matriciels d’une représentation unitaire irréductible sont continus et bornés, et sont donc de carré intégrable sur G, puisque G est compact.

#### Proposition 2 {#ts-v-s4-prop-2 .statement tag=03DR}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. La dimension de E est finie et égale au degré formel de $\pi$.

La représentation $\pi$ étant de carré intégrable (lemme 1), son degré formel $c_\mu(\pi )$ relativement à $\mu$ est défini (déf. 4 de V, p. 423) ; c’est un nombre réel strictement positif. Soit $(e_i)_{i\in I}$ une famille finie orthonormale dans E. Soit $x$ un élément de E de norme 1 (il en existe puisque E est non nul). Pour $i\in I$, on a

$$
c_\mu(\pi )\int_G|\langle e_i|\pi (g)x\rangle |^2d\mu(g) = 1
$$

(prop. 8 de V, p. 424). Sommons cette formule sur $i\in I$. On obtient

Card(I) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
\leqslant c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

d’après l’inégalité de Bessel (EVT, V, p. 21, prop. 4). Donc le cardinal de I est majoré par $c_\mu(\pi )$. Cela entraîne que la dimension de E est finie.

On peut alors appliquer ce qui précède à une base orthonormale $(e_i)_{i\in I}$ de E. On obtient, d’après EVT, V, p. 22, prop. 5,

dim(E) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
=c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

ce qui conclut la preuve.

En particulier, il est donc loisible de parler du caractère $\chi_{\pi}$ d’une représentation unitaire irréductible $\pi$ de G. C’est une fonction continue sur G.

#### Corollaire 1 {#ts-v-s4-prop-2-cor-1 .statement tag=03DS}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. Le caractère de $\pi$ est un élément hermitien de l’algèbre involutive $L^1(G)$.

Soit $x\in G$. Puisque G est unimodulaire, on a $\chi^*_{\pi}(x) =$ Tr($\pi (x^{-1})$), d’où $\chi^*_{\pi}(x) =$ Tr($\pi (x)$) puisque $\pi$ est une représentation unitaire.

#### Corollaire 2 {#ts-v-s4-prop-2-cor-2 .statement tag=03DT}

a) Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. On a

$\int'$ 1 $''$

$$
\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y\rangle d\mu(g) =\langle x|y\rangle  \langle x|y\rangle
$$

$_G$ dim(E)

pour tout $(x, y, x', y')\in E^4$;

b) Soit $\pi_1($resp. $\pi_2)$ une représentation unitaire irréductible de G dans un espace hilbertien $E_1($resp. $E_2)$. Si $\pi_1$ et $\pi_2$ ne sont pas isomorphes, on a

$$
\int_G\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\mu(g) = 0
$$

pour tout $(x, x', y, y')\in E^2_1\times E^2_2$.

Cela découle aussitôt de la prop. 8 de V, p. 424 et de la prop. 9 de V, p. 424, compte tenu du lemme 1 et de la formule $c_\mu(\pi ) =$ dim(E) (prop. 2).

#### Corollaire 3 {#ts-v-s4-prop-2-cor-3 .statement tag=03DU}

Soient $\pi_1$ et $\pi_2$ des représentations irréductibles de G. Dans l’espace hilbertien $L^2(G)$, on a $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 1$ si $\pi_1$ et $\pi_2$ sont isomorphes et $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 0$ sinon. Autrement dit, la famille des caractères des classes $\pi \in \widehat{G}$ est une famille orthonormale dans $L^2(G)$.

Cela résulte de la proposition 1 de V, p. 457 et du corollaire 2 en notant que pour toute base orthonormale $(e_i)_{i\in I}$ de l’espace d’une représentation unitaire $\pi$ de dimension finie de G, et pour tout $g\in G$, on a la formule

$$
\chi_{\pi}(g) =\sum_{i\in I}\langle e_i|\pi (g)e_i\rangle
$$

#### Corollaire 4 {#ts-v-s4-prop-2-cor-4 .statement tag=03DV}

a) Soit $\varrho$ une représentation continue de dimension finie de G. On a

$\chi_{\varrho}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho ))\chi_{\pi}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\varrho , \pi ))\chi_{\pi}$.

b) Soient $\varrho_1$ et $\varrho_2$ des représentations continues de dimension finie de G. On a

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =$ dim(Hom$_G(\varrho_1, \varrho_2)) =$ dim(Hom$_G(\varrho_2, \varrho_1))$.

c) Une représentation continue $\varrho$ de dimension finie de G est irréductible si et seulement si $\|\chi_{\varrho}\|^2= 1$.

Puisque $\varrho$ est semi-simple, elle est isomorphe à la somme directe de ses composantes $\pi$-isotypiques $M_{\pi}(\varrho )$ pour $\pi \in \widehat{G}$. Notant $m_{\pi}(\varrho )$ la multiplicité de $\pi$ dans $\varrho$ (déf. 10 de V, p. 398), on a alors

$$
\chi_{\varrho}=\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho )\chi_{\pi}
$$

L’assertion a) résulte donc du fait que

$m_{\pi}(\varrho ) =$ dim Hom$_G(\pi , \varrho ) =$ dim Hom$_G(\varrho , \pi )$

(formule (1) de V, p. 377 et cor. 2 de V, p. 387).

Par bilinéarité et orthonormalité des caractères, l’assertion a) implique que

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho_1))$ dim(Hom$_G(\pi , \varrho_2))$, et d’autre part on a des isomorphismes canoniques

Hom$_G(\varrho_1, \varrho_2)\rightarrow \bigoplus_{(\pi_1,\pi_2)\in\widehat{G}\times\widehat{G}}$ Hom$_G(M_{\pi_1}(\varrho_1),M_{\pi_2}(\varrho_2))$

$\rightarrow \bigoplus_{\pi\in\widehat{G}}$ Hom$_G(M_{\pi}(\varrho_1),M_{\pi}(\varrho_2))$

(formule (1) de V, p. 377) d’où il résulte que

dim(Hom$_G(\varrho_1, \varrho_2)) =\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho_1)m_{\pi}(\varrho_2)$,

d’où l’assertion b). L’assertion c) résulte également de a) et du lemme de Schur (prop. 6 de V, p. 386).

#### Corollaire 5 {#ts-v-s4-prop-2-cor-5 .statement tag=03DW}

Soient $\pi_1$ et $\pi_2$ des représentations unitaires irréductibles de G. On a $\pi_1(\overline{\chi}_{\pi_2}) = 0$ si $\pi_1$ n’est pas isomorphe à $\pi_2$, et $\pi_1(\overline{\chi}_{\pi_1})$ est la multiplication par $1/$ dim($\pi_1$).

Le caractère de $\pi_2$ est une fonction centrale continue sur G donc l’application linéaire $u$ = $\pi_1(\overline{\chi}_{\pi_2})$ est définie et appartient à l’espace Hom$_G(\pi_1, \pi_1)$. C’est une homothétie d’après le lemme de Schur (prop. 6 de V, p. 386) dont la trace est

Tr($u$) $=$ Tr $\int_G\overline{\chi_{\pi_2}(g)}\pi_1(g)d\mu(g)$

$$
=\int_G\overline{\chi_{\pi_2}(g)}\chi_{\pi_1}(g)d\mu(g)
$$

D’après les relations d’orthogonalité, la trace de $u$ est donc nulle si $\pi_1$ n’est pas isomorphe à $\pi_2$, et égale à 1 sinon. L’assertion en résulte.

#### Remarque {#ts-v-s4-n2-rem-1 .statement tag=03DX}

Lorsque G est fini, la relation d’orthogonalité de Schur (resp. la formule d’orthogonalité des caractères) coïncide avec celle de A, VIII, p. 399 (resp. celle de A, VIII, p. 400, prop. 4). Par contre, la « seconde relation d’orthogonalité » des caractères des groupes finis (A, VIII, p. 402, formule (32)) n’a pas d’analogue exact lorsque G est compact.

Pour G fini, le cas particulier de la seconde formule d’orthogonalité correspondant à la classe de conjugaison de $e$ est la formule

1 1 si $g=e$

$\sum$ dim($\pi$ )$\chi_{\pi}(g) =$

Card $G_{\pi\in\widehat{G}}$ 0 sinon, qui s’interprète aussi comme le calcul du caractère de la représentation régulière $\boldsymbol{\gamma }_G$ de G, et qui est équivalente à la formule Tr($\boldsymbol{\gamma }_G(f)$) $=f(e)$ pour toute fonction $f$ de G dans $\mathbf{C}$.

Soit G de nouveau un groupe compact quelconque. Pour toute fonction $f\in \mathscr{C}$(G), l’endomorphisme $\boldsymbol{\gamma }_G(f)$ de $L^2(G)$ coïncide avec l’endomorphisme $\varphi \mapsto f*\varphi$, et il est de trace finie (lemme 4 de V, p. 407 et corollaire 2 de III, p. 33). D’après loc. cit. et le th. 2 de IV, p. 177, on a également

Tr($\boldsymbol{\gamma }_G(f)$) $=\int_Gf(x^{-1}x)d\mu(x) =f(e)$.

#### Proposition 3 {#ts-v-s4-prop-3 .statement tag=03DY}

Supposons que $G = G_1\times G_2$ où $G_1$ et $G_2$ sont des groupes compacts. L’application $b$ de $\widehat{G}_1\times \widehat{G}_2$ dans $\widehat{G}$ qui à $(\pi_1, \pi_2)$ associe la classe de $\pi_1\boxtimes \pi_2$ est une bijection.

D’après le cor. 6 de V, p. 389, l’application $b$ est bien définie.

Soient $\pi_1$ et $\pi_2$ des éléments de $\widehat{G}$. Soit $\pi \in \widehat{G}$. La composante $\pi$-isotypique de la restriction $\varpi$ de $\pi_1\boxtimes \pi_2$ à $G_1\times  \{e\}$ est égale à $\varpi$ si $\pi_1=\pi$ et est nulle dans le cas contraire (lemme 8 de V, p. 384). Ainsi, la représentation unitaire $\pi_1\boxtimes \pi_2$ détermine $\pi_1$ à isomorphisme près ; de même, elle détermine $\pi_2$, ce qui démontre que $b$ est injective.

Démontrons que $b$ est surjective. Soit $\pi$ une représentation unitaire irréductible de $G_1\times G_2$ dans un espace hilbertien E. Elle est de dimension finie (prop. 2). Soit $\pi_1$ une représentation unitaire irréductible de $G_1$ dans un espace hilbertien $E_1$ telle que la restriction de $\pi$ à $G_1\times  \{e\}$ contient une sous-représentation isomorphe à $\pi_1$ (lemme 3 de V, p. 379). Notons F = Hom$_{G_1}(\pi_1, \pi )$. C’est un espace vectoriel non nul de dimension finie. Pour $h\in G_2$ et $u\in F$, soit $\varrho (h)(u)$ l’application linéaire de $E_1$ dans E définie par $x\mapsto \pi (e, h)(u(x))$. Puisque $G_1\times  \{e\}$ et $\{e\} \times G_2$ commutent dans G, l’application $\varrho (h)(u)$ appartient à l’espace F. L’application $\varrho$ est une représentation linéaire de $G_2$ dans l’espace F ; elle est continue. Comme F n’est pas réduit à 0, il existe une sous-représentation irréductible $\pi_2$ de $\varrho$ (lemme 3 de V, p. 379). Soit $E_2$ l’espace de $\pi_2$. L’application linéaire $v: E_1\otimes E_2\rightarrow E$ telle que $x\otimes u\mapsto u(x)$ pour $x\in E_1$ et $u\in E_2$ est alors un G-morphisme non nul de $\pi_1\boxtimes \pi_2$ dans $\pi$; comme les représentations $\pi$ et $\pi_1\boxtimes \pi_2$ sont irréductibles et de dimension finie, le morphisme $v$ est un isomorphisme (lemme 2 de V, p. 378).

Cette proposition est à comparer avec le th. 1 de A, VIII, p. 208.

### 3. Le théorème de Peter–Weyl

On rappelle qu’on note Θ(G) l’espace des coefficients matriciels des représentations unitaires de dimension finie de G. L’espace Θ(G) est une sous-algèbre unifère de $\mathscr{C}(G)$ stable par la conjugaison complexe (prop. 5 de V, p. 386).

Pour $\pi \in \widehat{G}$, on note $\boldsymbol{\varrho }_G(\pi )$ le sous-espace de $\mathscr{C}(G)$ engendré par les coefficients matriciels de $\pi$. On l’identifie à un sous-espace de $L^2(G)$.

L’espace Θ(G) coïncide avec la somme des espaces $\boldsymbol{\varrho }_G(\pi )$ pour $\pi \in \widehat{G}$ (en effet, tout élément de Θ(G) est somme de coefficients matriciels de représentations irréductibles de G puisque les représentations de dimension finie de G sont semi-simples d’après la prop. 1 de V, p. 457). De plus, cette somme est directe puisque, d’après le cor. 2 de V, p. 458, les espaces $\boldsymbol{\varrho }_G(\pi )$ sont deux à deux orthogonaux.

#### Proposition 4 {#ts-v-s4-prop-4 .statement tag=03DZ}

L’espace Θ(G) est dense dans $\mathscr{C}(G)$ et dans $L^2(G)$.

La sous-algèbre unifère Θ(G) de $\mathscr{C}(G)$ est stable par conjugaison. Elle coïncide avec la sous-algèbre Υ(G) par la prop. 2 de V, p. 457, donc elle sépare les points de G (cor. du th. 4 de V, p. 454). Par conséquent, elle est dense dans $\mathscr{C}(G)$ d’après TG, X, p. 40, cor. 2, et a fortiori, elle est dense dans l’espace $L^2(G) ($cf. INT, IV, p. 155, §4, n$^o7$, prop. 13).

Rappelons que la représentation unitaire birégulière de G est la représentation $\boldsymbol{\varrho }_G$ de $G\times G$ dans $L^2(G)$ telle que $(g_1, g_2)\mapsto \boldsymbol{\gamma }_G(g_1)\boldsymbol{\delta }_G(g_2)$.

#### Proposition 5 {#ts-v-s4-prop-5 .statement tag=03E0}

Soit $\pi \in \widehat{G}$. L’espace $\boldsymbol{\varrho }_G(\pi )$ est une sous-représentation de $\boldsymbol{\varrho }_G$ qui est isomorphe à $\overline{\pi}\boxtimes \pi$. En particulier, c’est une représentation irréductible de $G\times G$.

D’après la prop. 7 de V, p. 422 (appliquée avec $Z =\{e\})$, l’espace $\boldsymbol{\varrho }_G(\pi )$ est une sous-représentation de $\boldsymbol{\varrho }_G$ et l’application linéaire de $E_{\pi}\otimes E_{\pi}$ dans $L^2(G)$ qui associe à $x\otimes y$ le coefficient matriciel $g\mapsto  \langle x|\pi (g)y\rangle$ est un $(G\times$ G)-isomorphisme de $\overline{\pi}\boxtimes \pi$ dans $\boldsymbol{\varrho }_G(\pi )$. La sous-représentation $\boldsymbol{\varrho }_G(\pi )$ est donc irréductible (prop. 3 de V, p. 461).

#### Théorème 1 (Peter–Weyl) {#ts-v-s4-thm-1 .statement tag=03E1}

Soit G un groupe topologique compact. La représentation birégulière $\boldsymbol{\varrho }_G$ de G est la somme hilbertienne des sous-représentations $\boldsymbol{\varrho }_G(\pi )$ pour $\pi \in \widehat{G}$.

Les espaces $\boldsymbol{\varrho }_G(\pi )$ sont deux à deux orthogonaux ; ce sont des sous-représentations irréductibles de la représentation birégulière de G (prop. 5) qui sont deux à deux non isomorphes (prop. 3 de V, p. 461). Le théorème résulte alors du fait que la somme Θ(G) des espaces $\boldsymbol{\varrho }_G(\pi )$ pour $\pi$ parcourant $\widehat{G}$ est dense dans $L^2(G)$ (prop. 4).

#### Corollaire 1 {#ts-v-s4-thm-1-cor-1 .statement tag=03E2}

Pour tout $\pi \in \widehat{G}$, la sous-représentation $\boldsymbol{\varrho }_G(\pi )$ est la composante $(\overline{\pi}\boxtimes \pi )$-isotypique de $\boldsymbol{\varrho }_G$.

Soit F la composante $(\overline{\pi}\boxtimes \pi$)-isotypique de $\boldsymbol{\varrho }_G$. L’espace F contient $\boldsymbol{\varrho }_G(\pi )$ (prop. 5). De plus, pour tout $\tau \in \widehat{G}$ différent de $\pi$, l’intersection de F et $\boldsymbol{\varrho }_G(\tau )$ est nulle (prop. 3 de V, p. 461). On en déduit que $F =\boldsymbol{\varrho }_G(\pi )$ en appliquant le théorème.

#### Corollaire 2 {#ts-v-s4-thm-1-cor-2 .statement tag=03E3}

Soient $\pi_1$ et $\pi_2$ des représentations irréductibles non isomorphes de G. La composante $(\overline{\pi}_1\boxtimes \pi_2)$-isotypique de $\boldsymbol{\varrho }_G$ est nulle.

#### Corollaire 3 {#ts-v-s4-thm-1-cor-3 .statement tag=03E4}

La représentation régulière droite (resp. gauche) de G est isomorphe à la somme hilbertienne

$\pi \bigoplus\in \widehat{G}\pi$dim($\pi$ ).

D’après le théorème et la proposition 5, la restriction de la représentation birégulière de G au sous-groupe $H =\{e\} \times G$ est isomorphe à la somme hilbertienne des restrictions à H des représentations $\overline{\pi}\boxtimes \pi$ pour $\pi \in \widehat{G}$. Celles-ci sont isomorphes à la somme directe de dim($\pi$ ) copies de $\pi$ (lemme 8 de V, p. 384). Cela implique le résultat pour la représentation régulière droite, et le cas de la représentation régulière gauche est similaire.

#### Corollaire 4 {#ts-v-s4-thm-1-cor-4 .statement tag=03E5}

Soit $\pi \in \widehat{G}$. La composante $\pi$-isotypique de $\boldsymbol{\delta }_G$ (resp. la composante $\overline{\pi}$-isotypique de $\boldsymbol{\gamma }_G)$ est égale à $\boldsymbol{\varrho }_G(\pi )$.

L’argument est similaire à celui du corollaire précédent, en considérant $\boldsymbol{\varrho }_G(\pi )$ comme sous-représentation de $\boldsymbol{\delta }_G$ (resp. de $\boldsymbol{\gamma }_G)$.

#### Remarque 1 {#ts-v-s4-n3-rem-1 .statement tag=03E6}

Si G est fini, ces énoncés correspondent aux résultats de A, VIII, p. 398, remarque.

#### Remarque 2 {#ts-v-s4-n3-rem-2 .statement tag=03E7}

Supposons que G est commutatif. L’ensemble $\widehat{G}$ s’identifie au groupe dual de G (V, p. 393, remarque). Pour tout $\chi \in \widehat{G}$, l’espace de $\boldsymbol{\varrho }_G(\chi )$ est le sous-espace de dimension 1 de $L^2(G)$ engendré par $\chi$. Le théorème 1 pour G est donc alors équivalent au cor. du th. 1 de II, p. 215.

#### Remarque 3 {#ts-v-s4-n3-rem-3 .statement tag=03E8}

S’il existe un entier $n\geqslant 0$ tel que G est un sous-groupe compact de $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$, la représentation identique de G dans $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$ suffit à séparer les points de G, et on peut donc alors démontrer directement la proposition 4, puis le théorème de Peter–Weyl, sans faire appel au théorème de Gelfand–Raikov.

#### Remarque 4 {#ts-v-s4-n3-rem-4 .statement tag=03E9}

Le théorème de Peter–Weyl implique en particulier que l’homomorphisme continu naturel de G dans $\prod_{\pi\in\widehat{G}}\mathbf{U}(E_{\pi})$ est injectif.

### 4. Coefficients matriciels et fonctions G-finies

#### Proposition 6 {#ts-v-s4-prop-6 .statement tag=03EA}

Les sous-espaces suivants de $L^2(G)$ sont égaux :

a) L’espace Θ(G) ;

b) La somme directe algébrique des sous-espaces $\boldsymbol{\varrho }_G(\pi )$ de $L^2(G)$;

c) L’espace des vecteurs G-finis (cf. V, p. 376) de $\boldsymbol{\gamma }_G$;

d) L’espace des vecteurs G-finis de $\boldsymbol{\delta }_G$;

e) L’espace des vecteurs $(G\times G)$-finis de $\boldsymbol{\varrho }_G$.

En particulier, tout vecteur G-fini de $\boldsymbol{\gamma }_G,\boldsymbol{\delta }_G$ ou $\boldsymbol{\varrho }_G$ appartient à $\mathscr{C}(G)$.

Notons $F_a$ (resp. $F_b, F_c, F_d, F_e)$ l’espace défini par la condition a) (resp. b), c), d), e)). On a déjà remarqué que $F_a= F_b$.

On a $F_b\subset F_c$ car $\boldsymbol{\varrho }_G(\pi )$ est une sous-représentation de dimension finie de $\boldsymbol{\gamma }_G$ pour tout $\pi \in \widehat{G}$. Réciproquement, soit $f$ un vecteur G-fini de $\boldsymbol{\gamma }_G$. Le sous-espace $E_f$ engendré par les fonctions $\boldsymbol{\gamma }_G(g)f$ pour $g\in G$ est une sous-représentation de dimension finie de $\boldsymbol{\gamma }_G$. Elle est égale à la somme directe de ses composantes $\pi$-isotypiques pour $\pi \in \widehat{G}$ (prop. 1 de V, p. 457). D’après le cor. 4 de V, p. 463, cela implique que $E_f$ est contenu dans la somme des espaces $\boldsymbol{\varrho }_G(\pi )$, donc $F_c\subset F_b$.

Par un raisonnement analogue, on obtient $F_b= F_d$, et comme $\boldsymbol{\varrho }_G(\pi )$ est une sous-représentation de $\boldsymbol{\varrho }_G$, on établit de même que $F_b= F_e$.

#### Corollaire {#ts-v-s4-n4-cor-1 .statement tag=03EB}

Soit $E\subset L^2(G)$ un sous-espace vectoriel de dimension finie définissant une sous-représentation de $\boldsymbol{\gamma }_G($resp. de $\boldsymbol{\delta }_G$, de $\boldsymbol{\varrho }_G)$. Alors E est contenu dans $\mathscr{C}(G)$.

En effet, tout élément de E est un vecteur G-fini de la représentation $\boldsymbol{\gamma }_G$.

### 5. Représentations dans un espace séparé quasi-complet

#### Proposition 7 {#ts-v-s4-prop-7 .statement tag=03EC}

Soit $\varrho$ une représentation continue de G dans un espace localement convexe séparé et quasi-complet E. La somme des sous-représentations de dimension finie de E est dense dans E.

Soit $x\in E$ et soit U un voisinage ouvert de $x$. L’ensemble des mesures $\nu \in \mathscr{M}(G)$ telles que $\varrho (\nu )x\in U$ est ouvert dans $\mathscr{M}(G)$ pour la topologie de la convergence compacte (cf. n$^o2$ de V, p. 400). Il contient $\varepsilon_e$, donc il contient une mesure de la forme $\nu =f_1\cdot \mu$ où $f_1\in \mathscr{C}(G)$ (INT, VIII, p. 171, § 4, n$^o7$, prop. 19) et, par conséquent, il contient une mesure de la forme $f_2\cdot \mu$ où $f_2$ est une fonction G-finie (prop. 6 de V, p. 464 et prop. 4 de V, p. 462).

La sous-représentation F de $\boldsymbol{\gamma }_G$ engendrée par $f_2$ est de dimension finie. Soit $\widetilde{F}$ l’image de l’application linéaire $f\mapsto \varrho (f)x$ de F dans E. L’espace $\widetilde{F}$ est de dimension finie, et il contient l’élément $\varrho (f_2)x$ de U. Puisque $\varrho (g)\varrho (f) =\varrho (\boldsymbol{\gamma }_G(g)f)$ pour tout $g\in G$ et tout $f\in F$ (formule (1) de V, p. 406), l’espace $\widetilde{F}$ est une sous-représentation de $\varrho$ qui rencontre U. La proposition est démontrée.

#### Corollaire 1 {#ts-v-s4-prop-7-cor-1 .statement tag=03ED}

Soit $\pi$ une représentation continue irréductible de G dans un espace localement convexe séparé quasi-complet E. L’espace E est de dimension finie.

#### Corollaire 2 {#ts-v-s4-prop-7-cor-2 .statement tag=03EE}

Soit $\varrho$ une représentation continue de G dans un espace localement convexe séparé quasi-complet E et soit $\pi$ une représentation continue irréductible de G.

a) Le G-morphisme $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ de E dans E est un projecteur continu de E dont l’image est la composante $\pi$-isotypique de $\varrho$;

b) Si $\varrho$ est une représentation unitaire, alors le projecteur $p_{\pi}$ est l’orthoprojecteur de E d’image $M_{\pi}(\varrho )$.

Démontrons a). L’application linéaire $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ est bien définie, puisque E est quasi-complet et que G est compact (V, p. 401). C’est un élément de Hom$_G(\varrho , \varrho )$ puisque le caractère de $\pi$ est une fonction centrale continue sur G.

Soient $\varpi$ une sous-représentation de dimension finie de E et F son espace. L’application $p_{\pi}$ induit, par passage aux sous-espaces, l’endomorphisme (dim $\pi )\varpi (\overline{\chi}_{\pi})$ de F. Cet endomorphisme est donc nul si $\varpi$ n’est pas isomorphe à $\pi$, et est l’application identique de F sinon (en effet, c’est le cas si $\varpi$ est irréductible d’après le cor. 5 de V, p. 460, et le cas général s’en déduit puisque $\varpi$ est semi-simple d’après la prop. 1 de V, p. 457).

Finalement, puisque la somme des sous-représentations de dimension finie de E est dense dans E (prop. 7) et que $p_{\pi}$ est continu, on conclut que $p_{\pi}$ est un projecteur dont l’image est la composante $\pi$-isotypique de $\varrho$. Si E est hilbertien, le projecteur $p_{\pi}$ est hermitien d’après le cor. 1 de V, p. 458 donc c’est un orthoprojecteur (lemme 3, (ii) de I, p. 133).

#### Corollaire 3 {#ts-v-s4-prop-7-cor-3 .statement tag=03EF}

Soit $\varrho$ une représentation continue de G dans un espace localement convexe séparé quasi-complet E. L’endomorphisme

$$
x\mapsto \int_G\varrho (g)x d\mu(g)
$$

de E est un projecteur de E dont l’image est l’espace $E^G$ des vecteurs invariants dans E. En particulier, si E est de dimension finie, alors

dim(E$^G) =\int_G\chi_{\varrho}(g)d\mu(g)$.

La première assertion est le cas particulier du corollaire précédent lorsque $\pi$ est la représentation triviale de dimension 1 de G. La seconde en résulte puisque la dimension de $E^G$ est la trace de l’orthoprojecteur sur $E^G$, c’est-à-dire

dim(E$^G) =$ Tr $\int_G\varrho (g)d\mu(g)=\int_G\chi_{\varrho}(g)d\mu(g)$.

En particulier, lorsque E est de dimension finie, il existe un vecteur $x\not = 0$ dans E tel que $\varrho (g)x=x$ pour tout $g\in G$ si et seulement si

$$
\int_G\chi_{\varrho}(g)d\mu(g)\not = 0
$$

#### Corollaire 4 {#ts-v-s4-prop-7-cor-4 .statement tag=03EG}

Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien E. L’espace E est la somme hilbertienne des composantes $\pi$-isotypiques $M_{\pi}(\varrho )$ pour $\pi \in \widehat{G}$. En particulier, la représentation $\varrho$ est semi-simple.

Les composantes isotypiques de $\varrho$ correspondant à des représentations irréductibles non isomorphes de G sont orthogonales (prop. 8 de V, p. 394). Puisque toute représentation unitaire de dimension finie de G est semi-simple (prop. 1 de V, p. 457), la somme des composantes isotypiques $M_{\pi}(\varrho )$ pour $\pi \in \widehat{G}$ est dense dans E (prop. 7). Le corollaire en résulte.

### 6. Caractères et classes de conjugaison

Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien E de dimension finie. Le caractère de $\varrho$ vérifie $|\chi_{\varrho}|\leqslant$ dim(E). Soit $(e_i)_{i\in I}$ une base orthonormale de E ; le caractère $\chi_{\varrho}$ est la somme des coefficients matriciels diagonaux $g\mapsto  \langle e_i|\varrho (g)e_i\rangle$ de $\varrho$. En particulier, le caractère de $\varrho$ est une fonction G-finie, et si $\varrho$ est irréductible, alors $\chi_{\varrho}\in \boldsymbol{\varrho }_G(\varrho )$.

On a les formules suivantes

$$
\chi_{\varrho_1\oplus\varrho_2}=\chi_{\varrho_1}+\chi_{\varrho_2},\chi_{\varrho_1\otimes\varrho_2}=\chi_{\varrho_1}\chi_{\varrho_2},\chi_{\breve{\varrho}}=\chi_{\overline{\varrho}}=\overline{\chi}_{\varrho}
$$

(cf. A, VIII, p. 388–389).

#### Proposition 8 {#ts-v-s4-prop-8 .statement tag=03EH}

On a

(1) $\chi_{\pi}*\chi_{\sigma}= 0$ pour tous $\pi , \sigma$ appartenant à $\widehat{G}, \pi \not =\sigma$,

1

(2) $\chi_{\pi}*\chi_{\pi}=\chi_{\pi}$ pour tout $\pi$ appartenant à $\widehat{G}$.

dim($\pi$ )

Soient $\pi$ et $\sigma$ des représentations irréductibles de G. On a

dim($\pi$ )$(\chi_{\pi}*\chi_{\sigma}) =$ dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$

(lemme 4 de V, p. 407). La fonction dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$ est la projection orthogonale de $\chi_{\sigma}$ sur la composante $\overline{\pi}$-isotypique de $\boldsymbol{\gamma }_G$ (cor. 2 de V, p. 465), c’est-à-dire sur $\boldsymbol{\varrho }_G(\pi )$ (cor. 4 de V, p. 463). Comme $\chi_{\sigma}$ appartient à $\boldsymbol{\varrho }_G(\sigma )$, le résultat découle du théorème 1 de V, p. 462.

#### Lemme 2 {#ts-v-s4-lem-2 .statement tag=03EI}

Le graphe de la relation d’équivalence « $x\in G$ et $y\in G$ et $x$ est conjugué à $y$ » dans G est fermé.

En effet, ce graphe est l’image de l’application continue de l’espace compact $G\times G$ dans lui-même définie par $(x, y)\mapsto (x, yxy^{-1})$.

On note $G^{\sharp}$ l’espace des classes de conjugaison de G muni de la topologie quotient ; c’est un espace compact d’après le lemme 2 et TG, I, p. 78, prop. 8. Soit $\varpi : G\rightarrow G^{\sharp}$ la projection canonique. L’application de $\mathscr{C}(G^{\sharp})$ dans $\mathscr{C}(G)$ définie par $f\mapsto f\circ \varpi$ identifie l’algèbre stellaire $\mathscr{C}(G^{\sharp})$ à la sous-algèbre stellaire de $\mathscr{C}(G)$ formée des fonctions centrales continues.

Les mesures sur $G^{\sharp}$ s’identifient aux mesures centrales sur G (V, p. 402, déf. 1).

La forme linéaire sur $\mathscr{C}(G^{\sharp})$ définie par $f\mapsto \int_Gf$ est alors une mesure positive de masse 1 sur $G^{\sharp}$, qui est notée $\mu^{\sharp}$. Pour tout $p\in [1,+\infty ]$, on note $\mathscr{L}^p(G^{\sharp})$ (resp. $L^p(G^{\sharp}))$ l’espace $\mathscr{L}_{\mathbf{C}}^p(G^{\sharp}, \mu^{\sharp})$ (resp. $L^p_{\mathbf{C}}(G^{\sharp}, \mu^{\sharp}))$. On identifie $L^p(G^{\sharp})$ à l’adhérence de $\mathscr{C}(G^{\sharp})$ dans $L^p(G)$; en particulier, c’est un sous-espace fermé de $L^p(G)$.

On note aussi $\Theta (G^{\sharp}) = \Theta (G)\cap \mathscr{C}(G^{\sharp})$ l’espace des coefficients matriciels centraux de G. C’est une sous-algèbre involutive unifère de $\mathscr{C}(G^{\sharp})$.

Lorsque G est un groupe de Lie, l’espace $\Theta (G^{\sharp})$ est également noté ZΘ(G) dans LIE, IX, p. 71.

#### Lemme 3 {#ts-v-s4-lem-3 .statement tag=03EJ}

Soit $\pi$ une représentation unitaire irréductible de G. L’espace vectoriel $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ est de dimension un et engendré par le caractère de $\pi$.

Considérons la représentation unitaire $\sigma$ de G dans l’espace $\boldsymbol{\varrho }_G(\pi )$ définie par $\sigma (g) =\boldsymbol{\varrho }_G(g, g)$. Puisque la représentation unitaire $\boldsymbol{\varrho }_G(\pi )$ de $G\times G$ est isomorphe à $\overline{\pi}\boxtimes \pi$ (prop. 5 de V, p. 462), son caractère est donné par

$$
\chi_{\sigma}(g) =\chi_{\overline{\pi}\boxtimes\pi}(g, g) =|\chi_{\pi}(g)|^2
$$

pour tout $g\in G$. L’espace $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ est le sous-espace des éléments invariants de cette représentation, et sa dimension est égale à

$$
\int_G\chi_{\sigma}(g)d\mu(g) =\int_G|\chi_{\pi}(g)|^2d\mu(g) = 1
$$

(cor. 3 de V, p. 466 et cor. 3 de V, p. 459). Puisque le caractère de $\pi$ est un élément non nul de $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$, c’est une base de cet espace.

#### Proposition 9 {#ts-v-s4-prop-9 .statement tag=03EK}

La famille $(\chi_{\pi})_{\pi\in\widehat{G}}$ des caractères des représentations unitaires irréductibles de G est une base orthonormale de $L^2(G^{\sharp})$.

D’après le théorème de Peter–Weyl (th. 1 de V, p. 462), le sous-espace fermé $L^2(G^{\sharp})$ de $L^2(G)$ formé des éléments invariants de la représentation unitaire $g\mapsto \boldsymbol{\varrho }_G(g, g)$ de G est la somme hilbertienne des sous-espaces $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ pour $\pi \in \widehat{G}$. La proposition résulte donc du lemme précédent et du cor. 3 de V, p. 459.

#### Corollaire 1 {#ts-v-s4-prop-9-cor-1 .statement tag=03EL}

L’espace vectoriel $\Theta (G^{\sharp})$ est dense dans $\mathscr{C}(G^{\sharp})$ et dans $L^2(G^{\sharp})$.

La seconde assertion résulte de la prop. 9. Pour ce qui est de la première assertion, considérons la représentation linéaire $\varrho$ de G sur l’espace de Banach $\mathscr{C}(G)$ définie par

$$
\varrho (g)f(x) =f(g^{-1}xg)
$$

pour tout $f\in \mathscr{C}(G)$ et tout $x\in G$. C’est une représentation continue et isométrique et $\mathscr{C}(G^{\sharp})$ est l’espace des éléments invariants de cette représentation. Le projecteur continu $p=\varrho (1)$ de $\mathscr{C}(G)$ a donc pour image $\mathscr{C}(G^{\sharp})$ (cor. 3 de V, p. 466) ; il est de norme $\leqslant 1$.

Soit $f\in \mathscr{C}(G^{\sharp})$ et soit $\varepsilon  >0$. Il existe $\widetilde{f}\in \Theta (G)$ telle que $\|f-\widetilde{f}\|\leqslant \varepsilon$ (prop. 4 de V, p. 462), et on a alors $\|f-p(\widetilde{f})\|=\|p(f-\widetilde{f})\|\leqslant \varepsilon$; comme $p(\widetilde{f})\in \mathscr{C}(G^{\sharp})$, on conclut que $\Theta (G^{\sharp})$ est dense dans $\mathscr{C}(G^{\sharp})$.

On note R(G) l’anneau de Grothendieck des représentations continues de G dans des espaces vectoriels complexes séparés de dimension finie (cf. LIE, IX, p. 70 et A, VIII, p. 182, appliqué à la classe additive des représentations continues de G dans des espaces vectoriels complexes séparés de dimension finie, vues comme $\mathbf{C}$[G]-modules). Puisque toute représentation linéaire continue de G dans un espace vectoriel topologique séparé de dimension finie est semi-simple (prop. 1 de V, p. 457), le groupe abélien R(G) est libre et les classes de représentations unitaires irréductibles $\pi \in \widehat{G}$ en forment une base (A, VIII, p. 186, prop. 7).

#### Corollaire 2 {#ts-v-s4-prop-9-cor-2 .statement tag=03EM}

a) La famille des caractères des représentations irréductibles de G est une base de $\Theta (G^{\sharp})$;

b) L’application $u: R(G)\otimes_{\mathbf{Z}}\mathbf{C}\rightarrow \Theta (G^{\sharp})$ telle que $u(\pi \otimes 1) =\chi_{\pi}$ pour tout $\pi \in \widehat{G}$ est un isomorphisme d’algèbres sur $\mathbf{C}$.

La première assertion résulte de la proposition 9 et du corollaire 1.

Puisque les classes des représentations $\pi \in \widehat{G}$ forment une base du $\mathbf{Z}$-module libre R(G), l’application $u$ est bien définie. C’est un morphisme de $\mathbf{C}$-algèbres, et c’est un isomorphisme d’après a).

#### Corollaire 3 {#ts-v-s4-prop-9-cor-3 .statement tag=03EN}

Soit H un groupe topologique localement compact tel que G est un sous-groupe compact de H. Soit $\varrho$ une représentation unitaire de H dans un espace hilbertien E. Si la composante $\pi$-isotypique de la restriction de $\varrho$ à G est de dimension finie pour tout $\pi \in \widehat{G}$, alors la représentation $\varrho$ de H est semi-simple et toute représentation unitaire irréductible de H est de multiplicité finie dans $\varrho$.

Notons $\sigma$ la restriction de $\varrho$ au sous-groupe compact G de H. Soit $\pi$ une représentation irréductible de G. L’endomorphisme $\sigma (\chi_{\pi})\in \mathscr{L}(E)$ est de rang fini, puisque son image est la composante $\overline{\pi}$-isotypique de $\sigma$ (cor. 2 de V, p. 465) et que celle-ci est de dimension finie par hypothèse. Par conséquent, l’endomorphisme $\sigma (f)$ est de rang fini pour tout $f\in \Theta (G^{\sharp})$ et est compact pour tout $f\in \mathscr{C}(G^{\sharp})$ (cor. 1 de V, p. 468 et cor. de la prop. 2 de III, p. 4).

Notons $j$ l’injection canonique de G dans H. C’est une application continue qui est $\nu$-propre pour toute mesure $\nu$ sur G (INT, V, p. 69, § 6, n$^o1$, remarque 1). Soit $\mathfrak{B}$ le filtre des voisinages compacts de l’élément $e$ dans G. Pour tout $V\in \mathfrak{B}$, il existe une fonction centrale continue positive $f_V$ sur G à support contenu dans V dont l’intégrale sur G vaut 1. Notons $\beta_V$ la mesure image $j(f_V\cdot \mu)$; c’est une mesure positive à support compact sur H telle que $\varrho (\beta_V) =\sigma (f_V)$ (INT, V, p. 71, § 6, n$^o2$, th. 1). D’après ce qui précède, la base de filtre sur $\mathscr{M}_c(H)$ image de $\mathfrak{B}$ par l’application $V\mapsto \beta_V$ vérifie les conditions de la proposition 2 de V, p. 402 et l’assertion en résulte.

Corollaire 4 (Critère d’équirépartition de Weyl)

Soit M un ensemble de mesures positives centrales sur G tel que $\nu (G) = 1$ pour tout $\nu \in M$. Soit $\mathfrak{F}$ un filtre sur M. Pour que le filtre $\mathfrak{F}$ converge vaguement vers la mesure $\mu^{\sharp}$ sur $G^{\sharp}$, il faut et il suffit que, pour toute représentation unitaire irréductible non triviale $\pi$, on ait

lim$_{\nu ,\mathfrak{F}}\int_G\chi_{\pi}(x)d\nu (x) = 0$.

Puisque $\nu (G^{\sharp}) = 1 =\mu^{\sharp}(G^{\sharp})$ pour $\nu \in M$, l’hypothèse signifie que

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}\chi_{\pi}(x)d\nu (x) =\int_{G^{\sharp}}\chi_{\pi}(x)d\mu^{\sharp}(x)$

pour toute représentation $\pi \in \widehat{G}$, donc elle équivaut à la condition

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}f(x)d\nu (x) =\int_{G^{\sharp}}f(x)d\mu^{\sharp}(x)$

pour toute fonction $f\in \Theta (G^{\sharp})$ par linéarité. Comme l’espace $\Theta (G^{\sharp})$ est dense dans $\mathscr{C}(G^{\sharp})$ (corollaire 1), l’hypothèse est donc équivalente à la convergence du filtre $\mathfrak{F}$ vers $\mu^{\sharp}$ dans $\mathscr{M}(G^{\sharp})$ muni de la topologie de la convergence simple dans $\mathscr{C}$ (G), qui coïncide avec la topologie de la convergence vague puisque G est compact (cf. INT, III, p. 59, § 1, n$^o9)$.

### 7. La cotransformation de Fourier

On munit l’ensemble $\widehat{G}$ de la topologie discrète. On note $F(\widehat{G})$ l’algèbre produit des End(E$_{\pi})$ pour $\pi$ appartenant à $\widehat{G}$ et $F_b(\widehat{G})$ l’algèbre stellaire produit des End(E$_{\pi})$ (exemple 5 de I, p. 103) ; c’est l’ensemble des familles $(u_{\pi})_{\pi\in\widehat{G}}$ telles que sup$\|u_{\pi}\|<+\infty$.

On note $F_0(\widehat{G})$ la sous-algèbre stellaire fermée de $F^{\pi\in\widehat{G}}_b(\widehat{G})$ formée des familles $(u_{\pi})_{\pi\in\widehat{G}}$ telles que $\|u_{\pi}\|$ tend vers 0 à l’infini.

Soit $\nu \in \mathscr{M}^1(G)$. Pour tout $\pi \in \widehat{G}$, on a $\|\pi (\nu )\|\leqslant \|\nu \|$, donc la famille $(\pi (\nu ))_{\pi\in\widehat{G}}$ appartient à $F_b(\widehat{G})$.

#### Définition 1 {#ts-v-s4-def-1 .statement tag=03EO}

Pour toute mesure $\nu \in \mathscr{M}^1(G)$, l’élément $(\pi (\nu ))_{\pi\in\widehat{G}}$ de $F_b(\widehat{G})$ est noté $\mathscr{F}_G(\nu )$. L’application de $\mathscr{M}^1(G)$ dans $F_b(\widehat{G})$ ainsi définie est appelée la cotransformation de Fourier de G, et $\overline{\mathscr{F}}_G(\nu )$ est appelée la cotransformée de Fourier de la mesure $\nu$.

Pour $f\in L^1$(G), on notera $\overline{\mathscr{F}}_G(f) =\overline{\mathscr{F}}_G(f\cdot \mu)$.

Pour toute représentation $\pi \in \widehat{G}$, l’application $\nu \mapsto \pi (\nu )$ est un morphisme unifère d’algèbres de Banach involutives de $\mathscr{M}^1(G)$ dans End(E$_{\pi})$ (lemme 1 de V, p. 401). La cotransformation de Fourier est donc un morphisme unifère d’algèbres de Banach involutives de $\mathscr{M}^1(G)$ dans $F_b(\widehat{G})$.

### 8. La transformation de Fourier

On garde les notations du numéro précédent.

Soit $\pi \in \widehat{G}$. On munit l’espace vectoriel End(E$_{\pi})$ de la structure d’espace hilbertien dont le produit scalaire est donné par

$\langle u_1|u_2\rangle =$ dim($\pi$)Tr($u^*_1u_2$) $=$ dim($\pi$)Tr($u_2u^*_1$)

pour $u_1,u_2$ dans End(E$_{\pi}) ($cf. EVT, V, p. 52, th. 1).

On note $\|u\|_2$ = $\overline{\langle u|u\rangle}$ la norme d’un élément $u$ de End(E$_{\pi})$ pour $\pi \in \widehat{G}$. Pour tout $g\in G$, on a $\|\pi (g)\|_2=$ dim($\pi$ ) puisque $\pi (g)$ est unitaire.

La norme notée ici $\|u\|_2$ diffère par un facteur dim($\pi$ ) de la norme définie dans EVT, V, p. 52 sur l’espace des applications de Hilbert– Schmidt de $E_{\pi}$.

#### Lemme 4 {#ts-v-s4-lem-4 .statement tag=03EP}

Soit $\pi$ une représentation irréductible de G. L’application $f\mapsto \pi (f)$ définit par passage aux sous-espaces un isomorphisme isométrique de $\boldsymbol{\varrho }_G(\overline{\pi})$ dans End(E$_{\pi})$.

Posons $\varepsilon_{\pi}(g, h)u=\pi (g)\circ u\circ \pi (h^{-1})$ pour tout $(g, h)\in G\times G$ et pour tout $u\in$ End(E$_{\pi})$. L’application $\varepsilon_{\pi}$ est une représentation continue de $G\times G$ dans End(E$_{\pi})$. Elle est unitaire. En effet, puisque $\pi$ elle-même est unitaire, il vient

$\|\varepsilon_{\pi}(g, h)u\|^2_2=$ dim($\pi$ ) Tr $(\pi (g)u\pi (h^{-1}))^*\pi (g)u\pi (h^{-1})$

= dim($\pi$ ) Tr($\pi (h)u^*u\pi (h)^{-1}$) $=$ dim($\pi$ ) Tr($u^*u$) $=\|u\|^2_2$ pour tout $(g, h)\in G\times G$ et tout $u\in$ End(E$_{\pi})$.

L’application Ψ définie par $f\mapsto \pi (f)$ est un $(G\times$ G)-morphisme de $\boldsymbol{\varrho }_G(\overline{\pi})$ dans End(E$_{\pi})$, puisque

$$
\pi (\boldsymbol{\varrho }_G(g, h)f) =\int_Gf(g^{-1}xh)\pi (x)d\mu(x) =\pi (g)\pi (f)\pi (h^{-1})
$$

pour tout $(g, h)\in G\times G$ et tout $f\in \boldsymbol{\varrho }_G(\overline{\pi})$. Puisque $\boldsymbol{\varrho }_G(\overline{\pi})$ est une représentation irréductible (th. 1, a) de V, p. 462), il existe $\lambda \in \mathbf{C}^*$ tel que l’application $\lambda \Psi$ est nulle ou isométrique (cor. 5, a) de V, p. 388).

Soit $f=$ dim($\pi$ )$\overline{\chi}_{\pi}\in \boldsymbol{\varrho }_G(\overline{\pi})$. Il vient $\pi (f) = 1_{E_{\pi}}$ (cor. 2 de V, p. 465), d’où $\|\pi (f)\|_2=$ dim($\pi$ ) $=\|f\|$ (cor. 3 de V, p. 459). Par conséquent, l’application Ψ est isométrique. Comme $\boldsymbol{\varrho }_G(\overline{\pi})$ et End(E$_{\pi})$ sont de même dimension, Ψ est un isomorphisme isométrique.

On note $F^2(\widehat{G})$ la somme hilbertienne des espaces hilbertiens End(E$_{\pi})$. La norme d’un élément $x\in F^2(\widehat{G})$ est encore notée $\|x\|_2$.

Dans LIE, IX, p. 79, cet espace est noté $L^2(\widehat{G})$, notation que nous préférons éviter ici pour ne pas créer de confusion avec l’espace $\ell^2(\widehat{G})$.

Soit $(u_{\pi})$ un élément de $F^2(\widehat{G})$. Puisque

$^{\pi\in\widehat{G}}\sum_{\pi\in\widehat{G}}\|u_{\pi}\|^2_2=\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($u^*_{\pi}u_{\pi}$)$<+\infty$

et que $\|u_{\pi}\|^2\leqslant$ Tr($u^*_{\pi}u_{\pi}$) $($cf. EVT, V, p. 52, formule (33)), la norme dans $\mathscr{L}(E_{\pi})$ de l’endomorphisme $u_{\pi}$ tend vers 0 à l’infini. On peut donc identifier $F^2(\widehat{G})$ à un sous-espace de $F_0(\widehat{G})$.

Soient $\pi \in \widehat{G}$ et $u\in$ End(E$_{\pi})$. On note $\mathscr{F}_{\pi}(u)$ la fonction sur G définie par $\mathscr{F}_{\pi}(u)(g) =\langle \pi (g)|u\rangle =$ dim($\pi$)Tr($\pi (g)^*u$) pour tout $g\in G$. C’est une fonction continue sur G. Si G est un groupe de Lie réel compact, alors la fonction $\mathscr{F}_{\pi}(u)$ est analytique sur G (LIE, III, § 8, n$^o1$, th. 1).

Puisque G est compact, on peut identifier $L^2(G)$ à un sous-espace de $L^1(G)$.

#### Théorème 2 {#ts-v-s4-thm-2 .statement tag=03EQ}

La cotransformation de Fourier de G induit par passage aux sous-espaces un isomorphisme isométrique de $L^2(G)$ sur $F^2(\widehat{G})$. Son inverse $\mathscr{F}_G$ associe à un élément $(u_{\pi})_{\pi\in\widehat{G}}$ de $F^2(\widehat{G})$ la somme de la série

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

qui converge dans $L^2(G)$.

D’après le théorème de Peter–Weyl (th. 1 de V, p. 462), l’espace hilbertien $L^2(G)$ est la somme hilbertienne des espaces $\boldsymbol{\varrho }_G(\overline{\pi})$ pour $\pi \in \widehat{G}$. Pour tout $\pi \in \widehat{G}$, l’application linéaire $f\mapsto \pi (f)$ de $\boldsymbol{\varrho }_G(\overline{\pi})$ dans End(E$_{\pi})$ est un isomorphisme isométrique (lemme 4). Par conséquent, la restriction à $L^2(G)$ de la cotransformation de Fourier définit un isomorphisme isométrique de $L^2(G)$ sur $F^2(\widehat{G})$.

Soit $f\in L^2(G)$. Soit $\pi \in \widehat{G}$ et soit $f_{\overline{\pi}}\in \mathscr{C}(G)$ la projection orthogonale de $f$ sur $\boldsymbol{\varrho }_G(\overline{\pi})$ (th. 1 de V, p. 462). Cet espace étant la composante $\overline{\pi}$-isotypique de $\boldsymbol{\delta }_G$ (cor. 4 de V, p. 463), on a $f_{\overline{\pi}}=$ dim($\pi$ )$\boldsymbol{\delta }_G(\chi_{\pi})(f)$ d’après le cor. 2 de V, p. 465. Pour tout $x\in G$, il vient

$f_{\overline{\pi}}(x) =$ dim($\pi$ )$\int_G\chi_{\pi}(g)(\boldsymbol{\delta }_G(g)f)(x)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(g)f(xg)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(x^{-1}y)f(y)d\mu(y)$

= dim($\pi$)Tr($\pi (x^{-1})\pi (f)$) $=\langle \pi (x)|\pi (f)\rangle$,

c’est-à-dire $f_{\overline{\pi}}=\mathscr{F}_{\pi}(\pi (f))$.

Comme $f$ est la somme dans $L^2(G)$ de la famille $(f_{\overline{\pi}})$ d’après le théorème de Peter–Weyl, on obtient

$$
f=\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(\pi (f))
$$

où la série converge dans $L^2(G)$. Cela démontre le théorème.

#### Définition 2 {#ts-v-s4-def-2 .statement tag=03ER}

L’isomorphisme isométrique $\mathscr{F}_G$ de $F^2(\widehat{G})$ sur $L^2(G)$ inverse de l’isomorphisme induit par la cotransformation de Fourier est appelé la transformation de Fourier de G. L’image d’un élément de $F^2(\widehat{G})$ est appelé sa transformée de Fourier.

#### Remarque 1 {#ts-v-s4-n8-rem-1 .statement tag=03ES}

La transformée de Fourier de $(u_{\pi})_{\pi\in\widehat{G}}\in F^2(\widehat{G})$ est donc la classe dans $L^2(G)$ de la série

$g\mapsto \sum_{\pi\in\widehat{G}}\langle \pi (g)|u_{\pi}\rangle =\sum_{\pi\in\widehat{G}}$ dim($\pi$)Tr($u_{\pi}\circ \pi (g)^{-1}$).

#### Remarque 2 {#ts-v-s4-n8-rem-2 .statement tag=03ET}

Soit $f\in L^2(G)$. On a alors la formule de Plancherel

$$
\|f\|^2=\|\overline{\mathscr{F}}_G(f)\|^2=\sum_{\pi\in\widehat{G}}\|\pi (f)\|^2
$$

De plus, d’après le théorème 2$,f$ est la somme dans $L^2(G)$ de la famille $(f_{\pi})_{\pi\in\widehat{G}}$ où

$$
f_{\pi}(x) =\mathscr{F}_{\pi}(\pi (f))(x)
$$

$=\langle \pi (x)|\pi (f)\rangle =$ dim($\pi$ )$\int_Gf(g)\chi_{\pi}(x^{-1}g)d\mu(g)$

pour tout $x\in G$ et toute $\pi \in \widehat{G}$.

Supposons que G est commutatif. Puisque les représentations irréductibles de G sont de dimension 1 (cor. 7 de V, p. 390) et que le groupe dual $\widehat{G}$ est discret (prop. 18 de II, p. 233), les algèbres $F_b(\widehat{G})$ et $F_0(\widehat{G})$ s’identifient, respectivement, à l’algèbre $\mathscr{C}_b(\widehat{G})$ des fonctions continues bornées sur $\widehat{G}$ et à l’algèbre $\mathscr{C}_0(\widehat{G})$ des fonctions continues tendant vers 0 à l’infini sur $\widehat{G}$. Comme G est compact, la mesure de Haar sur $\widehat{G}$ duale de $\mu$ est la mesure de comptage $\widehat{\mu}$ (prop. 18 de II, p. 233). La somme hilbertienne $F^2(\widehat{G})$ des espaces End(E$_{\pi})$ pour $\pi \in \widehat{G}$ s’identifie à l’espace hilbertien $L^2(\widehat{G},\widehat{\mu})$.

Soit $\nu \in \mathscr{M}^1(G)$. Alors, pour tout caractère unitaire $\chi \in \widehat{G}$, on a

$$
\chi (\nu ) =\int_G\chi  \nu
$$

ce qui démontre que la cotransformation de Fourier définie ci-dessus coïncide avec la cotransformation de Fourier de G définie dans II, p. 206.

Tout $f\in \mathscr{L}^2(G)$ est intégrable et la formule $\|\overline{\mathscr{F}}_G(f)\|_2=\|f\|$ est la formule de Plancherel (II, p. 215, théorème 1).

#### Proposition 10 {#ts-v-s4-prop-10 .statement tag=03EU}

La cotransformation de Fourier est un morphisme injectif d’algèbres de Banach involutives de $\mathscr{M}^1(G)$ dans $F_b(\widehat{G})$ qui envoie $L^1(G)$ dans $F_0(\widehat{G})$.

Comme G est compact, l’espace $\mathscr{C}(G)$ est inclus et dense dans $\mathscr{L}^1(G)$ et $\mathscr{L}^2(G)$.

Soit $\nu \in \mathscr{M}^1(G)$ telle que $\overline{\mathscr{F}}_G(\nu ) = 0$. Pour toute fonction $f$ continue sur G, on a alors $\overline{\mathscr{F}}_G(\nu *f) = 0$. Or $\nu *f$ appartient à $\mathscr{C}(G)$ (INT, VIII, p. 152, § 4, n$^o2$, prop. 3). Comme, d’après le théorème 2, la cotransformation de Fourier est injective sur $L^2$(G), et a fortiori, sur l’espace $\mathscr{C}$ (G), on a $\nu *f= 0$ pour $f\in \mathscr{C}(G)$. En particulier, il vient

$$
\int_Gf(x)d\nu (x) = (\nu *\check{f})(e) = 0
$$

pour toute fonction $f\in \mathscr{C}(G)$ (INT, VIII, loc. cit.), donc la mesure $\nu$ est nulle.

L’image de $\mathscr{C}(G)$ par la cotransformation de Fourier est contenue dans $F^2(\widehat{G})$, et a fortiori dans $F_0(\widehat{G})$. Puisque $F_0(\widehat{G})$ est fermé dans $F_b(\widehat{G})$ et que $\mathscr{C}(G)$ est dense dans $L^1$(G), l’image de $L^1(G)$ par la cotransformation de Fourier est également contenue dans $F_0(\widehat{G})$.

#### Proposition 11 {#ts-v-s4-prop-11 .statement tag=03EV}

a) Soit $u= (u_{\pi})_{\pi\in\widehat{G}}$ un élément de $F(\widehat{G})$. Si la famille $(\mathscr{F}_{\pi}(u_{\pi}))_{\pi\in\widehat{G}}$ est uniformément sommable dans $\mathscr{C}(G)$, alors sa somme $f$ est une fonction continue sur G dont la cotransformée de Fourier est $u$;

b) Soit $f\in L^1(G)$. Si la famille $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ est uniformément sommable dans $\mathscr{C}(G)$, alors sa somme est une fon$\widehat{c}$tion continue sur G dont la classe dans $L^1(G)$ est égale à $f$.

Démontrons l’assertion a). Puisque G est compact, la somme $f$ de la famille $(\mathscr{F}_{\pi}(u_{\pi}))$ appartient à $L^2(G)$ et la série

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

converge dans $L^2(G)$ vers $f$ (INT, IV, p. 127, § 3, n$^o3$, prop. 4). On a donc $\mathscr{F}_G((u_{\pi})_{\pi}) =f$ dans $L^2$(G), d’où $(u_{\pi})_{\pi\in\widehat{G}}=\overline{\mathscr{F}}_G(f)$ (théorème 2).

Démontrons l’assertion b). On peut appliquer l’assertion a) à la famille $(\pi (f))_{\pi\in G}$. La somme $g$ de la famille $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ est une fonction continue, donc appartenant à $L^2$(G), telle que $\mathscr{F}_G(g) = (\pi (f))_{\pi\in G}$. Puisque $\mathscr{F}_G$ est injective sur $L^2$(G), on a $f=g$ dans $L^2$(G), donc dans $L^1(G)$.

L’algèbre $\mathscr{C}(\widehat{G})$ des fonctions à valeurs complexes sur $\widehat{G}$ s’identifie au centre de l’algèbre $F(\widehat{G})$ par l’application qui à $f:\widehat{G}\rightarrow \mathbf{C}$ associe l’élément central $(f(\pi )1_{E_{\pi}})_{\pi\in\widehat{G}}$ de $F(\widehat{G})$. Notons $\mathscr{M}^1(G^{\sharp})$ l’espace des mesures bornées centrales sur G. C’est un sous-espace fermé de l’algèbre de Banach $\mathscr{M}^1(G)$. Pour toute mesure $\nu \in \mathscr{M}^1(G^{\sharp})$ et toute représentation $\pi \in \widehat{G}$, on a $\pi (\nu )\in$ End$_G(E_{\pi})$ donc $\pi (\nu )$ est un multiple de l’application identique de $E_{\pi}$ d’après le lemme de Schur (prop. 6 de V, p. 386). La restriction de la cotransformation de Fourier à $\mathscr{M}^1(G^{\sharp})$ s’identifie donc à un morphisme unifère d’algèbres de Banach involutives de $\mathscr{M}^1(G^{\sharp})$ dans $\mathscr{C}(\widehat{G})$. Ce morphisme est injectif ; l’image de $L^1(G^{\sharp})$ est contenue dans $\mathscr{C}_b(\widehat{G})$ et sa restriction à $L^2(G^{\sharp})$ est un isomorphisme isométrique sur $L^2(\widehat{G},\widehat{\mu})$.

### 9. Indicateur de Frobenius–Schur et alternative de Larsen

Rappelons (LIE, VIII, §7, n$^o6$, déf. 2) qu’une représentation irréductible de G dans un espace vectoriel complexe E de dimension finie est dite de type orthogonal (resp. de type symplectique) s’il existe une forme bilinéaire symétrique non nulle sur E invariante par G (resp. s’il existe une forme bilinéaire alternée non nulle sur E invariante par G). Elle est dite de type complexe s’il n’existe pas de forme bilinéaire non nulle sur E invariante par G.

Lorsqu’une représentation irréductible dans E est de type orthogonal (resp. symplectique), l’espace des formes bilinéaires symétriques (resp. alternées) G-invariantes sur E est de dimension 1 et toute forme bilinéaire G-invariante non nulle sur E est séparante.

Une représentation de type orthogonal est parfois dite de type réel, et une représentation de type symplectique est parfois dite de type quaternionien (cf. LIE, IX, App. II).

Soit $\pi$ une représentation irréductible de G dans un espace vectoriel complexe E. Les trois possibilités ci-dessus sont distinguées par la valeur de la quantité

FS($\pi$ ) $=\int_G\chi_{\pi}(g^2)d\mu(g)$,

qui est appelée indicateur de Frobenius–Schur de $\pi$. On a en effet

1 si $\pi$ est de type orthogonal,

FS($\pi$ ) $=-1$ si $\pi$ est de type symplectique,

0 si $\pi$ est de type complexe.

(LIE, IX, App. 2, p. 103, prop. 3 et p. 105, prop. 4).

Lorsque G est un groupe de Lie, on peut calculer FS($\pi$ ) à l’aide de la prop. 1 de LIE, IX, p. 69.

#### Définition 3 {#ts-v-s4-def-3 .statement tag=03EW}

Soit $\varrho$ une représentation unitaire de dimension finie de G dans un espace hilbertien E. Soit $k$ un entier positif. On appelle moment absolu d’ordre $2k$ de $\varrho$, et on note $M_{2k}(\varrho )$, la dimension du sous-espace des éléments G-invariants dans la représentation $\overline{\varrho}^{\otimes k}\otimes \varrho^{\otimes k}$.

#### Théorème 3 (Alternative de Larsen) {#ts-v-s4-thm-3 .statement tag=03EX}

Supposons que G est infini. Soit $\pi$ une représentation unitaire fidèle de G dans un espace hilbertien E de dimension finie $\geqslant 2$.

a) Supposons que le groupe dérivé de G est infini. On a $M_4(\pi )\geqslant 2$ avec égalité si et seulement si G contient $\mathbf{S}\mathbf{U}(E)$;

b) Supposons que dim(E) $\geqslant 3$, que $\pi$ est de type orthogonal ou symplectique, et que dim(E) $\not = 4$ si $\pi$ est de type orthogonal. Alors $M_4(\pi )\geqslant 3$ avec égalité si et seulement si l’algèbre de Lie complexifiée de G est égale à l’algèbre de Lie d’une forme bilinéaire séparante G-invariante sur E. *C’est le cas si et seulement si la composante neutre $G_0$ de G est un sous-groupe compact maximal du groupe des automorphismes d’une telle forme bilinéaire.*

Nous utiliserons dans la démonstration les lemmes suivants.

#### Lemme 5 {#ts-v-s4-lem-5 .statement tag=03EY}

Soit $\pi$ une représentation unitaire de G dans un espace hilbertien E de dimension finie. Soient $(\varrho_i)_{i\in I}$ une famille de représentations unitaires non nulles de G et $(n_i)_{i\in I}$ une famille d’entiers $\geqslant 1$ tels que la représentation $\overline{\pi}\otimes \pi$ de G (resp. la représentation $\pi \otimes \pi )$ soit isomorphe à la somme directe $\bigoplus_{i\in I}\varrho^{n_i}_i$. Alors on a

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

avec égalité si et seulement si les représentations $\varrho_i$ sont irréductibles et deux à deux non isomorphes.

Notons $\chi_i$ le caractère de $\varrho_i$ pour $i\in I$. On a

$|\chi_{\pi}|^2=\chi_{\overline{\pi}\otimes\pi}=\sum_{i\in I}n_i\chi_i$, (resp. $\chi^2_{\pi}=\chi_{\pi\otimes\pi}=\sum_{i\in I}n_i\chi_i)$.

D’après la définition et le cor. 3 de V, p. 466, il vient

$$
M_4(\pi ) =\int_G|\chi_{\pi}|^4d\mu
$$

d’où, dans les deux cas, la formule

$M_4(\pi ) =\sum_{i,j}n_in_j\int_G\chi_i\overline{\chi}_jd\mu=\sum_{i,j}n_in_j$ dim Hom$_G(\varrho_i, \varrho_j)$

(cor. 4, b) de V, p. 459). Soit $i\in I$. Comme la représentation $\varrho_i$ n’est pas nulle, l’espace Hom$_G(\varrho_i, \varrho_i)$ n’est pas nul, et on en déduit la minoration

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

De plus, puisque $n_i\geqslant$ 1, il y a égalité si et seulement si on a dim Hom$_G(\varrho_i, \varrho_j) = 0$ si $i\not =j$ et dim Hom$_G(\varrho_i, \varrho_i) = 1$ pour tout $i$. La seconde condition est valide si et seulement si les représentations $\varrho_i$ sont irréductibles (loc. cit.). La première est alors satisfaite si et seulement si les représentations $\varrho_i$ sont deux à deux non isomorphes, d’après le lemme de Schur (V, p. 387, cor. 2).

Si E est un module sur un anneau commutatif A, on appellera carré symétrique (resp. carré extérieur) de E le A-module $\mathsf{S}^2(E)$ (resp. $\wedge^2E)$.

#### Lemme 6 {#ts-v-s4-lem-6 .statement tag=03EZ}

Soit $q$ une forme bilinéaire séparante sur un espace vectoriel complexe E de dimension finie $\geqslant 3$.

a) Si $q$ est symétrique, alors la représentation adjointe de l’algèbre de Lie orthogonale $\mathfrak{s}\mathfrak{o}(q)$ est isomorphe au carré extérieur $\wedge^2E$ de la représentation naturelle $\mathfrak{s}\mathfrak{o}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$;

b) Si $q$ est alternée, alors la représentation adjointe de l’algèbre de Lie symplectique $\mathfrak{s}\mathfrak{p}(q)$ est isomorphe au carré symétrique $\mathsf{S}^2(E)$ de la représentation naturelle $\mathfrak{s}\mathfrak{p}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$.

Munissons $\mathbf{C}$ de l’automorphisme involutif identique. La forme bilinéaire $q$ est alors $\varepsilon$-hermitienne (A, IX, § 3, n$^o1$, déf. 1) avec $\varepsilon = 1$ dans le cas a) et $\varepsilon =-1$ dans le cas b). Pour tout $u\in$ End(E), on note $^tu$ l’adjoint de $u$ par rapport à $q$. On a donc $q(x, u(y)) =q(^tu(x), y)$ pour tout $(x, y)\in E\times E$. Notons $v$ l’unique automorphisme de $E\otimes E$ tel que $v(x\otimes y) =y\otimes x$ pour tout $(x, y)\in E^2$.

Il existe une unique application linéaire $w$ de $E\otimes E$ dans End(E) telle que $w(a\otimes b)$ est l’application linéaire définie par $x\mapsto q(a, x)b$ pour tout $(a, b, x)\in E^3$. L’application $w$ est un isomorphisme. Pour tout $s\in E\otimes E$, on a

$$
t(w(s)) =\varepsilon  w(v(s)) \tag{3}
$$

En effet, pour tous $(x, y)$ et $(a, b)$ dans $E\times E$, il vient

$$
q(x, w(a\otimes b)y) =q(a, y)q(x, b) =\varepsilon q(b, x)q(a, y) =q(\varepsilon w(b\otimes a)x, y)
$$

Notons enfin $x\mapsto x^*$ l’isomorphisme de E sur $E'$ déduit de $q$, c’est-àdire tel que $\langle x^*, y\rangle =q(x, y)$ pour tout $(x, y)\in E^2$.

Ces notations étant établies, notons H le groupe orthogonal (resp. symplectique) de $q$. C’est un sous-groupe de Lie de $\mathbf{G}\mathbf{L}(E)$ dont l’algèbre de Lie $\mathfrak{h}$ est le sous-espace de End(E) constitué des $u\in$ End(E) tels que $^tu=-u$ (LIE, III, p. 146, cor. 1). Comme la forme $q$ est H-invariante, il vient

$$
\langle (ga)^*, b\rangle =q(ga, b) =\langle a, g^{-1}b\rangle
$$

pour tout $g\in H$ et tout $(a, b)\in E\times E$.

Munissons End(E) de la représentation adjointe Ad de H. L’application linéaire $w$ est un morphisme de représentations de H : en effet, pour tout $g\in H$ et tout $(a, b, x)\in E^3$, on a

$$
w(g(a\otimes b))(x) =\langle (ga)^*, x\rangle gb=\langle a, g^{-1}x\rangle gb
$$

$=g(\langle a, g^{-1}x\rangle b) =$ Ad($g$)$(w(a\otimes b))x$,

d’où la conclusion par linéarité.

Comme $v$ est également un morphisme de représentations de H, il en est de même de l’application linéaire $\theta =w-\varepsilon  w\circ v$; celle-ci est donc un morphisme de $\mathfrak{h}$-modules.

Notons F $\subset E\otimes E$ le sous-espace des éléments $s\in E\otimes E$ tels que $v(s) =-\varepsilon s$. Si $\varepsilon =-1$, la restriction à F de l’application canonique de $E\otimes E$ dans le carré symétrique de E est un isomorphisme de $\mathbf{C}$-espaces vectoriels (A, III, p. 72) ; si $\varepsilon = 1$, la restriction à F de l’application canonique de $E\otimes E$ dans le carré extérieur de E est un isomorphisme de $\mathbf{C}$-espaces vectoriels (loc. cit., p. 82).

L’image de F par $\theta$ est contenue dans $\mathfrak{h}:$ en effet, pour tout $s\in F$, la formule (3) implique

$$
^t\theta (s) =^tw(s)-\varepsilon^tw(v(s)) =\varepsilon  w(v(s))-w(s) =-\theta (s)
$$

Par définition de F, la restriction de l’application $\theta$ à F coïncide avec celle de $2w$ et l’application linéaire $\theta$ est donc injective sur F. Puisque dim(F) = dim($\mathfrak{h}$) (A, III, p. 75, th. 1 et p. 87, cor. 1 et LIE, VIII, p. 192 et p. 201), on conclut que $\theta$ induit par passage aux sous-espaces un isomorphisme de $\mathfrak{h}$-modules de F dans $\mathfrak{h}$, d’où le lemme.

#### Lemme 7 {#ts-v-s4-lem-7 .statement tag=03F0}

Soit $H_2$ un groupe de Lie réel et soit $H_1$ un sous-groupe fermé de $H_2$. L’algèbre de Lie complexifiée de $H_1$ s’identifie à une sous-représentation de la représentation adjointe de $H_1$ sur l’algèbre de Lie complexifiée de $H_2$.

En effet, la restriction à $H_1$ de la représentation adjointe de $H_2$ sur son algèbre de Lie s’identifie à la représentation adjointe de $H_1$.

#### Lemme 8 {#ts-v-s4-lem-8 .statement tag=03F1}

Soit E un espace hilbertien complexe de dimension finie $n$.

a) Les groupes $\mathbf{S}\mathbf{U}(E)$ et $\mathbf{U}(E)$ sont connexes ;

b) Le groupe dérivé de $\mathbf{S}\mathbf{U}(E)$ est égal à $\mathbf{S}\mathbf{U}(E)$;

c) Le groupe dérivé de $\mathbf{U}(E)$ est égal à $\mathbf{S}\mathbf{U}(E)$.

On peut supposer que $n\geqslant 1$ et que $E =\mathbf{C}^n$.

Soit A le sous-groupe de $\mathbf{U}(E)$ formé des matrices diagonales ; il est homéomorphe à $\mathbf{U}^n$, et donc connexe (TG, VI, p. 11, cor. 2 et I, p. 83, prop. 8). Son intersection avec $\mathbf{S}\mathbf{U}(E)$ est homéomorphe à $\mathbf{U}^{n-1}$, donc est également connexe.

D’après le th. 1 de IV, p. 149, le groupe $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E))$ est la réunion des sous-ensembles connexes $gAg^{-1}$ pour $g\in G$ (resp. des sous-ensembles connexes $g(A\cap \mathbf{S}\mathbf{U}(E))g^{-1})$; comme l’élément neutre appartient à chacun de ces ensembles, l’espace $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E))$ est connexe (TG, I, p. 81, prop. 2).

Démontrons b). L’assertion est vraie lorsque $n= 1$, puisque $\mathbf{S}\mathbf{U}(E)$ est alors réduit à l’élément neutre. Supposons donc que $n\geqslant 2$. L’algèbre de Lie de $\mathbf{S}\mathbf{U}(E)$ est alors simple (LIE, IX, p. 20, § 3, n$^o4)$ donc le groupe dérivé de $\mathbf{S}\mathbf{U}(E)$ est d’indice fini dans $\mathbf{S}\mathbf{U}(E)$. On en déduit le résultat puisque $\mathbf{S}\mathbf{U}(E)$ est connexe d’après a).

L’assertion c) résulte de b) puisque le groupe dérivé de $\mathbf{U}(E)$ est contenu dans $\mathbf{S}\mathbf{U}(E)$.

Démontrons maintenant le théorème 3. Notons $n$ la dimension de l’espace hilbertien E. Comme la représentation $\pi$ est fidèle, on peut supposer que G est un sous-groupe compact de $\mathbf{U}(E)$. Le groupe G est fermé dans le groupe de Lie réel $\mathbf{U}$(E), donc est un groupe de Lie réel compact (LIE, III, §8, n$^o2$, th. 2). Par hypothèse, G est infini, donc de dimension $\geqslant 1$. Soit $\mathfrak{g}$ son algèbre de Lie ; elle est non nulle.

Démontrons a). Supposons que le groupe dérivé D(G) est infini. On a la décomposition G-invariante End(E) $=\mathbf{C}1_E\oplus \mathfrak{s}\mathfrak{l}(E)$. Les représentations de G sur $\mathbf{C}1_E$ et sur $\mathfrak{s}\mathfrak{l}(E)$ ne sont pas isomorphes, puisque dim $\mathfrak{s}\mathfrak{l}(E)\geqslant 2$. D’après le lemme 5, on a donc $M_4(\pi )\geqslant 2$ avec égalité si et seulement si la représentation de G dans $\mathfrak{s}\mathfrak{l}(E)$ est irréductible. Or, le groupe dérivé de G est contenu dans $\mathbf{S}\mathbf{L}$(E), et la complexification de l’algèbre de Lie de D(G) s’identifie donc à un sous-espace de $\mathfrak{s}\mathfrak{l}$(E), qui est une sous-représentation de la représentation de G dans $\mathfrak{s}\mathfrak{l}(E)$ (lemme 7). Cette sous-représentation n’est pas nulle, puisque D(G) est infini. On a donc $M_4(\pi ) = 2$ si et seulement si $(\mathscr{D}\mathfrak{g})_{(\mathbf{C})}=\mathfrak{s}\mathfrak{l}(E)$. Puisque D(G) est contenu dans $\mathbf{S}\mathbf{U}$(E), et puisque $\mathbf{S}\mathbf{U}(E) = D(\mathbf{S}\mathbf{U}(E))$ (lemme 8), cette condition équivaut à $\mathbf{S}\mathbf{U}(E)\subset G$.

Pour la démonstration de l’assertion b), on reprend les notations de LIE, VIII, §13, n$^o$ 2–4.

Supposons que $\pi$ est de type symplectique et que dim(E) $\geqslant 3$. Soit $q$ une forme bilinéaire alternée non nulle G-invariante sur E ; elle est séparante (LIE, IX, p. 103, App. 2, prop. 3) et G est un sous-groupe compact du groupe symplectique $\mathbf{S}\mathbf{p}(q)$. Notons $q^*\in \wedge^2E$ l’élément auquel la forme alternée $q$ s’identifie. L’algèbre de Lie complexifiée $\mathfrak{g}_{(\mathbf{C})}$ de G est contenue dans $\mathfrak{s}\mathfrak{p}(q)$. Or, puisque dim(E) $\geqslant 3$, la représentation de $\mathfrak{s}\mathfrak{p}(q)$ dans $E\otimes E$ admet la décomposition en somme directe

$$
E\otimes E =\mathsf{S}^2(E)\oplus \wedge^2E =\mathsf{S}^2(E)\oplus E_2\oplus \mathbf{C}q^*
$$

où $E_2$ est la seconde représentation fondamentale de $\mathfrak{s}\mathfrak{p}(q)$ (LIE, VIII, p. 202, §13, n$^o3$, (IV)). Les représentations $E_2$ et $\mathbf{C}q^*$ de $\mathfrak{s}\mathfrak{p}(q)$ sont irréductibles (loc. cit.) et la représentation $\mathsf{S}^2(E)$ est non nulle.

D’après le lemme 5, on a donc $M_4(\pi )\geqslant 3$ avec égalité si et seulement si les représentations de G dans $\mathsf{S}^2$(E), $E_2$ et $\mathbf{C}q^*$ sont irréductibles et deux à deux non isomorphes.

Supposons que $M_4(\pi ) = 3$. Comme la représentation $\mathsf{S}^2(E)$ s’identifie à la représentation adjointe de $\mathfrak{s}\mathfrak{p}(q)$ (lemme 6), elle contient comme sous-représentation la complexification de la représentation adjointe de G (lemme 7). On a donc $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$.

Réciproquement, supposons que $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$. La représentation adjointe de $\mathfrak{s}\mathfrak{p}(q)$ et la représentation $E_2$ de $\mathfrak{s}\mathfrak{p}(q)$ sont irréductibles, de dimensions $n(n+ 1)/2$ et $n(n-1)/2-1$ respectivement (LIE, VIII, p. 202, §13, n$^o3$, (IV)), qui sont différentes et $\geqslant 2$ puisque $n\geqslant 3$, d’où $M_4(\pi ) = 3$.

Finalement, supposons que $\pi$ est de type réel et que dim(E) $\geqslant 3$ et dim(E) $\not = 4$. Soit $q$ une forme bilinéaire symétrique non nulle, G-invariante sur E ; elle est séparante (LIE, IX, p. 103, App. 2, prop. 3) et G est un sous-groupe compact du groupe orthogonal $\mathbf{O}(q)$. Notons $q^*\in \mathsf{S}^2(E)$ l’élément auquel $q$ s’identifie.

L’algèbre de Lie complexifiée $\mathfrak{g}_{(\mathbf{C})}$ de G est contenue dans $\mathfrak{s}\mathfrak{o}(q)$. La représentation de $\mathfrak{s}\mathfrak{o}(q)$ dans $E\otimes E$ admet la décomposition en somme directe

$$
E\otimes E =\wedge^2E\oplus \mathsf{S}^2(E) =\wedge^2E\oplus \mathsf{S}^2_0(E)\oplus \mathbf{C}q^*
$$

où $\mathsf{S}^2_0(E)$ est l’orthogonal de $q^*$ dans $\mathsf{S}^2(E)$. Ces représentations sont de dimension au moins 2 puisque dim(E) $\geqslant 3$. D’après le lemme 5, on a $M_4(\pi )\geqslant 3$ avec égalité si et seulement si les représentations de G dans $\wedge^2E$ et $\mathsf{S}^2_0(E)$ sont irréductibles et non isomorphes.

Supposons que $M_4(\pi ) = 3$. Comme la représentation $\wedge^2E$ s’identifie à la représentation adjointe de $\mathfrak{s}\mathfrak{o}(q)$ (lemme 6), elle contient comme sous-représentation la complexification de la représentation adjointe de G (lemme 7). La condition $M_4(\pi ) = 3$ implique donc que $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

Réciproquement, supposons que $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$. La représentation adjointe de $\mathfrak{s}\mathfrak{o}(q)$ est irréductible, puisque dim(E) $\not = 4$ (LIE, VIII, § 13, p. 193, (I) et p. 206, (I)), et de dimension $n(n-1)/2$. La représentation $\mathsf{S}^2_0(E)$ de $\mathfrak{s}\mathfrak{o}(q)$ a comme plus grand poids $2\varpi_1$. En comparant sa dimension avec celle de la représentation irréductible de $\mathfrak{s}\mathfrak{o}(q)$ de plus grand poids $2\varpi_1$, calculée par la formule de Weyl (cf. LIE, VIII, §9, n$^o2$, th. 2 et LIE, VI, planches II et IV), on vérifie que $\mathsf{S}^2_0(E)$ est irréductible. On conclut donc que $M_4(\pi ) = 3$ si $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

#### Remarque 1 {#ts-v-s4-n9-rem-1 .statement tag=03F2}

La condition « G est infini » est nécessaire dans le théorème 3 (exercice 9 de V, p. 507).

#### Remarque 2 {#ts-v-s4-n9-rem-2 .statement tag=03F3}

Soit $n\in \mathbf{N}$. Pour toute représentation unitaire $\varrho$ d’un groupe compact dans un espace hilbertien de dimension $n$, on a $M_4(\varrho )\leqslant n^2$; l’égalité est possible (exercice 15 de V, p. 508).

#### Remarque 3 {#ts-v-s4-n9-rem-3 .statement tag=03F4}

On peut démontrer (cf. R. Guralnick et P.H. Tiep, Decomposition of small tensor powers and Larsen’s conjecture, Representation Theory **9** (2005), 138–208) que la condition que G est infini peut être omise si l’on suppose que E est de dimension $\geqslant 7$ et si l’on remplace l’hypothèse $M_4(\pi ) = 2$ (resp. $M_4(\pi ) = 3)$ par $M_8(\pi ) = 24$ (resp. $M_8(\pi ) = 105)$.

## EXERCICES {#ts-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
