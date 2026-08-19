---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 4
section_title: Opérateurs partiels
lang: fr
source: ts-iii-v-fr
book_pages: TS IV.224-TS IV.261, TS IV.344-TS IV.352
pdf_pages: 0237-0274, 0357-0365
extraction: native
subsections:
    - "no": 1
      title: Opérateurs partiels
      page: 224
      pdf_page: 237
    - "no": 2
      title: Opérateurs fermés, fermables et à domaine dense
      page: 227
      pdf_page: 240
    - "no": 3
      title: Exemples d’opérateurs partiels
      page: 231
      pdf_page: 244
    - "no": 4
      title: Adjoint
      page: 235
      pdf_page: 248
    - "no": 5
      title: Critères élémentaires pour les opérateurs auto-adjoints
      page: 239
      pdf_page: 252
    - "no": 6
      title: Opérateurs différentiels
      page: 242
      pdf_page: 255
    - "no": 7
      title: Spectre et résolvante
      page: 243
      pdf_page: 256
    - "no": 8
      title: Pseudo-spectre
      page: 250
      pdf_page: 263
    - "no": 9
      title: Opérateurs de multiplication
      page: 252
      pdf_page: 265
    - "no": 10
      title: Extensions auto-adjointes d’un opérateur symétrique
      page: 255
      pdf_page: 268
statements: 74
exercises: 24
content_sha256: 7a1879cdb38ba3edbe58035bdb927411940e5d51061ec1842dd83ec41c145e01
---

## § 4. OPÉRATEURS PARTIELS

### 1. Opérateurs partiels

Dans ce numéro, K est un corps commutatif.

On rappelle (E, II, §3, p. 9–10) qu’un graphe[^1] est un ensemble dont tous les éléments sont des couples. Si A et B sont des ensembles, une correspondance entre A et B est un triplet $(\Gamma ,A,B)$, où Γ est un graphe contenu dans $A\times B$; son ensemble de définition (aussi appelé domaine) est pr$_1$(Γ), et l’ensemble de ses valeurs est pr$_2(\Gamma )$. Une correspondance est une fonction (E, II, p. 13, déf. 9) si son graphe est fonctionnel et si son ensemble de départ coïncide avec son ensemble de définition. Toute partie d’un graphe fonctionnel est un graphe fonctionnel.

#### Définition 1 {#ts-iv-s4-def-1 .statement tag=032J}

Soient E et F des espaces vectoriels sur K. Un opérateur partiel $u$ de E dans F est une correspondance $(\Gamma ,E,F)$ entre E et F vérifiant les conditions suivantes:

(i) Le graphe Γ est un sous-espace vectoriel de $E\times F$;

(ii) Le graphe Γ est fonctionnel.

Si E = F, on dit que $u$ est un opérateur partiel sur E.

Soit $u$ un opérateur partiel de E dans F. Le graphe Γ de la correspondance $u$ est appelé le graphe de l’opérateur partiel $u$, et est aussi noté $\Gamma_u$. On note $\mathscr{P}(E; F)$ l’ensemble des opérateurs partiels de E dans F ; on note simplement $\mathscr{P}(E) =\mathscr{P}(E; E)$.

Se donner un opérateur partiel de E dans F revient à se donner un sous-espace vectoriel D de E et une application linéaire $u$ de D dans F, l’opérateur partiel associé étant la correspondance $(\Gamma ,E,F)$ où $\Gamma \subset D\times F$ est le graphe de $u$.

Le domaine de définition d’un opérateur partiel $u$ est appelé simplement le domaine de $u$, et noté dom($u$).

Toute application linéaire $u$ de E dans F est un opérateur partiel de E dans F.

Si $D\subset E$ est un sous-espace vectoriel, on notera $1_D$ l’opérateur partiel de domaine D qui est l’application identique sur D, c’est-à-dire la correspondance $(\Delta_D,E,E)$ où $\Delta_D$ est la diagonale de $D\times D$ (E, II, p. 13, déf. 8). On notera $0_D$ l’opérateur partiel de domaine D qui est nul sur D, c’est-à-dire la correspondance $(D\times  \{0\},E,F)$.

Des opérateurs partiels $u= (\Gamma ,E,F)$ et $u'= (\Gamma ',E,F)$ de E dans F sont égaux si et seulement si dom($u$) $=$ dom($u'$) et si les applications linéaires $u$ et $u'$ de dom($u$) dans F coïncident.

Suivant E, II, §3, les notions suivantes sont définies :

(i) Soit $u$ un opérateur partiel de E dans F ; soient D son domaine et $u: D\rightarrow F$ l’application linéaire associée. L’image d’un sous-ensemble A de E par $u$ est le sous-ensemble $u(A\cap D)$ de F ; on la note simplement $u(A)$. L’image réciproque par $u$ d’un sous-ensemble B de F par $u$ est le sous-ensemble $\overset{-1}{u}(B)$ de D.

Si A (resp. B) est un sous-espace vectoriel de E (resp. de F), alors son image par $u$ (resp. son image réciproque) est un sous-espace vectoriel de F (resp. de E).

L’image de $u$ est le sous-espace vectoriel $u(D)$ de F, noté aussi Im($u$). On dit que $u$ est un opérateur partiel surjectif si Im($u$) $= F$. Le noyau de $u$ est le sous-espace vectoriel $\overset{-1}{u}(\{0\})$ de E, noté aussi Ker($u$). Le noyau de $u$ est réduit à 0 si et seulement si l’application linéaire $u$ de dom($u$) dans F est injective. On dit alors que $u$ est injectif. Si $u$ est injectif et surjectif, on dit qu’il est bijectif.

(ii) Si E, F et G sont des espaces vectoriels sur K et $u= (\Gamma ,E,F)$, $v= (\Gamma ',F,G)$ sont des opérateurs partiels de E dans F et de F dans G, respectivement, la correspondance composée $v\circ u= (\Gamma '\circ \Gamma ,E,G)$ est un opérateur partiel de E dans G. Son domaine est $\overset{-1}{u}$(dom($v$)). Si H est un espace vectoriel sur K et $w= (\Gamma '',G,H)$ un opérateur partiel de G dans H, on a $w\circ (v\circ u) = (w\circ v)\circ u$. On écrira parfois $vu$ au lieu de $v\circ u$.

(iii) En particulier, pour tout opérateur partiel $u$ de E dans F et tout $a\in K$, les opérateurs partiels $au= (a1_F)\circ u$ et $ua=u\circ (a1_E)$ sont définis. Ils sont égaux si $a\not = 0$, ou si le domaine de $u$ est égal à E ; on a $u0 = 0_E$ et $0u= 0_{dom(u)}$.

Soit E un espace vectoriel. D’après ce qui précède, l’ensemble $\mathscr{P}$(E), muni de la loi de composition définie par $(u, v)\mapsto u\circ v$, est un magma associatif unifère (A, I, p. 4, déf. 5 et A, I, p. 12, déf. 2) d’élément neutre $1_E$. Pour tout $n\in \mathbf{N}$, on notera $u^n$ le composé $\overset{n}{\circ}u$ (A, I, p. 13).

Par ailleurs, on définit les notions suivantes :

(i) Si $u= (\Gamma ,E,F)$ est un opérateur partiel de E dans F, et si G est un sous-espace vectoriel de E, la réduction de $u$ à G est l’opérateur partiel $(\Gamma \cap (G\times F),E,F)$ de E dans F. Son domaine est dom($u$)$\cap G$; on le notera parfois $u|G$, quand aucune confusion avec la restriction de $u$ au sous-espace G n’est à craindre.

(ii) Soit $v$ un opérateur partiel injectif de F dans E. La correspondance réciproque $v^{-1}= (\Gamma^{-1},E,F)$ de $v$ est alors un opérateur partiel tel que dom($v^{-1}$) $=$ Im($v$). On dit que $v^{-1}$ est l’opérateur partiel réciproque de $v$. On a les égalités $v\circ v^{-1}= 1_{dom(v^{-1})}$ dans $\mathscr{P}(E)$ et $v^{-1}\circ v= 1_{dom(v)}$ dans $\mathscr{P}(F)$. L’opérateur partiel $v^{-1}$ est injectif et on a $(v^{-1})^{-1}=v$.

(iii) Soient E, F et G des espaces vectoriels. Soit $u$ (resp. $v)$ un opérateur partiel injectif de E dans F (resp. de F dans G). Alors l’opérateur partiel $v\circ u$ est injectif et $(v\circ u)^{-1}=u^{-1}\circ v^{-1}$.

(iv) Si $u$ et $v$ sont des opérateurs partiels de E dans F, on dit que $v$ est une extension de $u$, et on note $u\subset v$, si le graphe de $u$ est contenu dans le graphe de $v$. Cela implique que dom($u$)$\subset$ dom($v$) et que $u$ est la réduction de $v$ à dom($u$). La relation « $u\subset v$ » est une relation d’ordre dans $\mathscr{P}(E; F)$. On a par exemple $au\subset ua$ pour tout $a\in K$ et tout $u\in \mathscr{P}(E; F)$.

(v) Soient E un espace vectoriel sur K et $(F_i)_{i\in I}$ une famille d’espaces vectoriels sur K. Pour $i\in I$, soit $u_i$ un opérateur partiel de E dans $F_i$. L’opérateur partiel produit des $u_i$ est l’opérateur partiel de E dans l’espace vectoriel produit des espaces $F_i$ dont le domaine est l’intersection D des espaces dom($u_i$) et qui associe à $x\in D$ la famille $(u_i(x))_{i\in I}$. On le note $(u_i)_{i\in I}$.

(vi) Soit $A : F\times F\rightarrow F$ l’application linéaire $(x, y)\mapsto x+y$. Soient $u$ et $v$ des opérateurs partiels de E dans F. La somme $u+v$ est l’opérateur partiel $A\circ (u, v)$ de E dans F. Son domaine est dom($u$)$\cap$ dom($v$). Pour $u,v,w$ dans $\mathscr{P}(E; F)$, on a $(u+v) +w=u+ (v+w)$.

Soit G un espace vectoriel sur K. Pour tous $u$ et $v$ dans $\mathscr{P}(E; F)$ et tout $w\in \mathscr{P}(F; G)$, on a $w\circ u+w\circ v\subset w\circ (u+v)$. En général, il n’y a pas égalité dans cette formule (exercice 1 de IV, p. 344), mais c’est le cas lorsque le domaine de $w$ est égal à F. Pour $w\in \mathscr{P}(G; E)$, on a $u\circ w+v\circ w= (u+v)\circ w$.

(vii) Soit L une extension du corps K. Soient E et F des espaces vectoriels sur K et $E_{(L)}= L\otimes_KE, F_{(L)}= L\otimes_KF$ les L-espaces vectoriels obtenus par extension des scalaires de K à L (A, II, p. 82). Pour tout opérateur partiel $u$ de E dans F, on note $u_{(L)}$ l’opérateur partiel de $E_{(L)}$ dans $F_{(L)}$ dont le graphe est le sous-espace vectoriel $L\otimes_K\Gamma_u$ de $E_{(L)}\times F_{(L)}$; son domaine est $L\otimes_K$ dom($u$), et il coïncide sur celui-ci avec l’unique application linéaire qui envoie $1\otimes x$ sur $1\otimes u(x)$ pour tout $x\in$ dom($u$).

Soit $v$ un opérateur partiel de E dans F. On a $u\subset v$ si et seulement si $u_{(L)}\subset v_{(L)}$.

(viii) Soient $E_1, F_1, E_2, F_2$ des K-espaces vectoriels. Soit $u$ (resp. $v)$ un opérateur partiel de $E_1$ dans $F_1$ (resp. de $E_2$ dans $F_2)$. On note $u\otimes v$ l’opérateur partiel de $E_1\otimes F_1$ dans $E_2\otimes F_2$ de domaine dom($u$)$\otimes$dom($v$) tel que $(u\otimes v)(x\otimes y) =u(x)\otimes v(y)$ pour tout $(x, y)\in E_1\times E_2$.

### 2. Opérateurs fermés, fermables et à domaine dense

Dans ce numéro, K désigne un corps topologique commutatif (TG, III, p. 54).

#### Définition 2 {#ts-iv-s4-def-2 .statement tag=032K}

Soient E et F des espaces vectoriels topologiques sur K (EVT, I, p. 1, déf. 1). Soit $u\in \mathscr{P}(E; F)$ un opérateur partiel de E dans F.

On dit que $u$ est un opérateur à domaine dense si le domaine de $u$ est dense dans E.

On dit que $u$ est fermé si le graphe de $u$ est fermé dans l’espace vectoriel topologique $E\times F$. On dit que $u$ est fermable s’il possède une extension fermée.

Soient E, F et G des espaces vectoriels topologiques sur K. Toute extension d’un opérateur $u\in \mathscr{P}(E; F)$ à domaine dense est à domaine dense. De plus, si $v\in \mathscr{L}(E; F)$, alors $u+v$ est un opérateur à domaine dense. Si $v: F\rightarrow G$ (resp. $w: G\rightarrow E)$ est un isomorphisme d’espaces vectoriels topologiques, alors $v\circ u$ (resp $u\circ w)$ est un opérateur à domaine dense.

#### Exemple {#ts-iv-s4-n2-exa-1 .statement tag=032L}

Soient E et F des espaces vectoriels topologiques sur K.

1) Supposons l’espace F séparé. Soit $u$ une application linéaire de E dans F. Si $u$ est continue, alors l’opérateur partiel $u$ est fermé (TG, I, p. 53, cor. 2). Supposons de plus que K est un corps valué non discret et que E et F sont des espaces vectoriels topologiques métrisables et complets sur K. D’après le théorème du graphe fermé (EVT, I, p. 19, cor. 5), l’opérateur partiel défini par $u$ est alors fermé si et seulement si $u$ est continue.

2) Supposons l’espace E séparé. Soit $v$ une application linéaire injective continue de F dans E. L’opérateur partiel $v^{-1}\in \mathscr{P}(E; F) ($cf. IV, p. 226) est alors fermé, puisque son graphe est l’image du graphe de $v$, qui est fermé, par l’isomorphisme d’espaces vectoriels topologiques de $F\times E$ dans $E\times F$ défini par $(y, x)\mapsto (x, y)$.

#### Proposition 1 {#ts-iv-s4-prop-1 .statement tag=032M}

Soient E et F des espaces vectoriels topologiques sur K. Un opérateur partiel $u$ de E dans F est fermable si et seulement si l’adhérence du graphe $\Gamma_u$ de $u$ dans $E\times F$ est un graphe fonctionnel. Il existe alors un unique opérateur partiel $v$ de E dans F dont le graphe est $\overline{\Gamma}_u$, et c’est la plus petite extension fermée de $u$.

Si l’adhérence du graphe de $u$ dans $E\times F$ est un graphe fonctionnel, c’est le graphe d’un opérateur partiel, et celui-ci est une extension fermée de $u$, qui est donc fermable. Réciproquement, supposons que $u\subset w$ avec $w$ fermé. L’adhérence $\overline{\Gamma}_u$ du graphe de $u$ dans $E\times F$ est contenue dans $\Gamma_w$, donc $\Gamma_u$ est un graphe fonctionnel.

La dernière assertion résulte du fait que si $w$ est une extension fermée de $u$, alors le graphe de $w$ contient $\overline{\Gamma}_u$.

#### Définition 3 {#ts-iv-s4-def-3 .statement tag=032N}

Soient E et F des espaces vectoriels topologiques sur K. Soit $u$ un opérateur fermable de E dans F. L’opérateur fermé dont le graphe est $\Gamma_u$ est appelé la fermeture de $u$. Il est noté $\overline{u}$.

#### Remarque {#ts-iv-s4-n2-rem-1 .statement tag=032O}

Soient E et F des espaces vectoriels topologiques sur K. Soit $u$ un opérateur fermable de E dans F. Le domaine de la fermeture de $u$ est contenu dans l’adhérence du domaine de $u$ dans E. En général, il en est distinct (exercice 1 de IV, p. 344, b)).

Si $u\in \mathscr{P}(E; F)$ est fermable et dom($u$) $= E$, alors $u=\overline{u}$ est fermé, puisqu’alors dom($\overline{u}$) $=$ dom($u$).

#### Proposition 2 {#ts-iv-s4-prop-2 .statement tag=032P}

Soit $K =\mathbf{R}$ et soient E et F des espaces vectoriels topologiques sur $\mathbf{R}$. Soit $u$ un opérateur partiel de E dans F. Alors $u$ est à domaine dense (resp. est fermé, est fermable) si et seulement si $u_{(\mathbf{C})}$ est à domaine dense (resp. est fermé, est fermable).

Supposons que le domaine de $u$ est dense dans E. Tout voisinage de 0 dans $E_{(\mathbf{C})}$ contient un voisinage de la forme $V +iV$ (EVT, II, p. 65), où V est un voisinage de 0 dans E, donc contient un élément du domaine de $u_{(\mathbf{C})}$; cet opérateur partiel est donc à domaine dense. La réciproque est également vraie puisque l’application de $E_{(\mathbf{C})}$ dans E qui à $x+iy$ associe $x$ pour tout $(x, y)\in E\times E$ est continue et surjective.

Le graphe de $u_{(\mathbf{C})}$ s’identifie à l’espace vectoriel topologique complexifié du graphe de $u$. Il est donc fermé dans $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$ si le graphe de $u$ est fermé dans $E\times E$. Réciproquement, on a $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$ dans $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$; comme $E\times E$ est fermé dans $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$, l’opérateur partiel $u$ est fermé lorsque $u_{(\mathbf{C})}$ l’est.

Un opérateur partiel $v$ de E dans F est une extension de $u$ si et seulement si $v_{(\mathbf{C})}$ est une extension de $u_{(\mathbf{C})}$, donc l’opérateur partiel $u_{(\mathbf{C})}$ est fermable si $u$ est fermable. Réciproquement, si $u_{(\mathbf{C})}$ est fermable, l’opérateur partiel $u$ l’est aussi puisque $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$, qui est alors un graphe fonctionnel (prop. 1).

#### Lemme 1 {#ts-iv-s4-lem-1 .statement tag=032Q}

Soient E, F et G des espaces vectoriels topologiques sur K. Soit $u$ un opérateur fermé de E dans F.

a) Pour tout $v\in \mathscr{L}(E; F)$, l’opérateur partiel $u+v$ est fermé.

b) Pour tout $v\in \mathscr{L}(G; E)$, l’opérateur partiel $u\circ v$ est fermé.

Démontrons a). Soit $\gamma$ l’application $(x, y)\mapsto (x, y-v(x))$ de $E\times F$ dans lui-même ; elle est continue. Pour tout $(x, y)\in E\times F$, on a $\gamma (x, y)\in \Gamma_u$ si et seulement si $x\in$ dom($u$) et $y=u(x) +v(x)$, c’est-àdire que $\overset{-1}{\gamma}(\Gamma_u) = \Gamma_{u+v}$. L’assertion en résulte.

Démontrons b). L’application $\eta = (v,1_F)$ de $G\times F$ dans $E\times F$ est continue ; pour tout $(z, y)\in G\times F$, on a $\eta (z, y) = (v(z), y)$, donc $\overset{-1}{\eta}(\Gamma_u) = \Gamma_{u\circ v}$. L’assertion en résulte.

Soient E et F des espaces vectoriels topologiques sur K, l’espace F étant séparé. Soit $a\in K$. Si $u\in \mathscr{P}(E; F)$ est fermable, alors il en est de même de $au$. Si $a\not = 0$, on a $\overline{au}=au$, et $u$ est fermé si et seulement si $au$ l’est. Si $a= 0$, la fermeture de $au$ est $0_{\overline{dom(u)}}$, et $au$ est égal à $0_{dom(\overline{u})}$; il se peut donc que $u$ soit fermé mais que $au$ ne le soit pas.

#### Proposition 3 {#ts-iv-s4-prop-3 .statement tag=032R}

Soient E et F des espaces vectoriels topologiques sur K, l’espace F étant séparé. Soit $u$ un opérateur partiel fermé de E dans F. Le noyau de $u$ est un sous-espace fermé de E.

En effet, le noyau de $u$ est l’image inverse du sous-espace fermé $\Gamma_u\cap (E\times  \{0\})$ de $E\times F$ par l’application linéaire continue $x\mapsto (x,0)$ de E dans $E\times F$.

Dans la suite de ce numéro, on suppose que K est un corps valué non discret.

#### Définition 4 {#ts-iv-s4-def-4 .statement tag=032S}

Soient E et F des espaces normés sur K et soit $u$ un opérateur partiel de E dans F. Pour $x$ dans dom($u$), on note

$$
\|x\|_u= (\|x\|^2_E+\|u(x)\|^2_F)^{1/2}
$$

L’application $x\mapsto  \|x\|_u$ ainsi définie est une norme sur dom($u$). On note $E_u$ l’espace normé ainsi obtenu.

#### Remarque {#ts-iv-s4-n2-rem-2 .statement tag=032T}

Soient E et F des espaces normés sur K et soit $u$ un opérateur partiel de E dans F.

1) L’injection canonique de $E_u$ dans E est continue puisqu’on a $\|x\|\leqslant \|x\|_u$ pour tout $x\in E$. En particulier, tout sous-espace de dom($u$) qui est fermé dans E est fermé dans $E_u$.

2) Si E et F sont des espaces hilbertiens, alors l’espace $E_u$ est un espace préhilbertien, puisque la norme sur $E_u$ provient de la forme hermitienne positive

$$
(x, y)\mapsto (x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

sur dom($u$).

#### Proposition 4 {#ts-iv-s4-prop-4 .statement tag=032U}

Soient E et F des espaces de Banach (resp. des espaces hilbertiens) et soit $u$ un opérateur partiel de E dans F. Alors $u$ est fermé si et seulement si l’espace normé $E_u$ est un espace de Banach (resp. un espace hilbertien).

Il suffit de traiter le cas des espaces de Banach. La norme de $E_u$ est obtenue, par transport de structure au moyen de l’application linéaire bijective $(x, y)\mapsto x$ de $\Gamma_u$ dans dom($u$), à partir de la norme obtenue par restriction au sous-espace $\Gamma_u$ de la norme $(x, y)\mapsto (\|x\|^2_E+\|y\|^2_F)^{1/2}$ sur l’espace de Banach $E\oplus F$. L’espace $E_u$ est donc un espace de Banach si et seulement si le sous-espace $\Gamma_u$ de $E\oplus F$ est fermé.

Si $u$ et $v$ sont des opérateurs partiels de E dans F et de F dans G, respectivement, et si $u$ est fermé, alors l’opérateur partiel $v\circ u$ n’est pas fermé en général, même si $v$ est continu (exercice 1 de IV, p. 344, c)). On a tout de même la condition suffisante suivante :

#### Lemme 2 {#ts-iv-s4-lem-2 .statement tag=032V}

Soient E, F et G des espaces normés sur K, l’espace F étant un espace de Banach. Soit $u$ un opérateur partiel fermé de E dans F et soit $v\in \mathscr{L}(F; G)$. S’il existe $C\in \mathbf{R}_+$ tel que

$$
\|u(x)\|\leqslant C(\|x\|+\|(v\circ u)(x)\|)
$$

pour tout $x\in$ dom($v\circ u$) $=$ dom($u$), c’est-à-dire, si l’application linéaire $x\mapsto u(x)$ de $E_{v\circ u}$ dans F est continue, alors $v\circ u$ est fermé.

Notons $w=v\circ u$. Soit $(x_n, w(x_n))_{n\in\mathbf{N}}$ une suite dans le graphe de $w$ qui converge dans $E\times G$. Soit $x$ la limite de la suite $(x_n)$. L’hypothèse implique que la suite $(u(x_n))_{n\in\mathbf{N}}$ est alors une suite de Cauchy dans F ; elle converge vers un élément $y$ de F. Puisque $u$ est fermé, on a donc $x\in$ dom($u$) et $y=u(x)$. Alors $w(x_n) =v(u(x_n))$ tend vers $v(y) =$ $v(u(x))$ puisque $v$ est continu, donc le graphe de $w$ est fermé.

Soient $u$ un opérateur partiel fermé sur un espace de Banach E et F un sous-espace de dom($u$). Si F est dense dans l’espace de Banach $E_u$, alors la réduction de $u$ à F est fermable, et sa fermeture est égale à $u$. On dit alors que F est un cœur pour $u$.

### 3. Exemples d’opérateurs partiels

Dans ce numéro, $K =\mathbf{R}$ ou $\mathbf{C}$.

#### Exemple 1 {#ts-iv-s4-n3-exa-1 .statement tag=032W}

Soit X un espace topologique localement compact et soit $\mu$ une mesure positive sur X. On fixe des éléments $p_1$ et $p_2$ de $[1,+\infty [$.

Soit $g$ une fonction $\mu$-mesurable sur X à valeurs dans K. Notons D le sous-espace de $\mathscr{L}_K^{p_1}(X, \mu)$ formé des fonctions $f$ dans $\mathscr{L}_K^{p_1}(X, \mu)$ telles que $gf\in \mathscr{L}_K^{p_2}(X, \mu)$. L’application linéaire de D dans $\mathscr{L}_K^{p_2}(X, \mu)$ définie par $f\mapsto gf$ détermine un opérateur partiel de $\mathscr{L}_K^{p_1}(X, \mu)$ dans $\mathscr{L}_K^{p_2}(X, \mu)$, que l’on note $m_g$.

Le sous-espace vectoriel des fonctions $\mu$-négligeables dans $\mathscr{L}_K^{p_1}(X, \mu)$ est contenu dans D, et l’image par $m_g$ d’une fonction $\mu$-négligeable est encore $\mu$-négligeable. On notera $\widetilde{m}_g$ l’opérateur partiel de $L^{p_1}_K(X, \mu)$ dans $L^{p_2}_K(X, \mu)$ déduit de $m_g$ par passage aux quotients. On dit que c’est l’opérateur de multiplication par $g$ de $L^{p_1}_K(X, \mu)$ dans $L^{p_2}_K(X, \mu)$. Des fonctions $g_1$ et $g_2$ localement égales $\mu$-presque partout définissent le même opérateur de multiplication.

#### Proposition 5 {#ts-iv-s4-prop-5 .statement tag=032X}

L’opérateur de multiplication $\widetilde{m}_g$ de $L^{p_1}_K(X, \mu)$ dans $L^{p_2}_K(X, \mu)$ est un opérateur fermé à domaine dense.

Démontrons d’abord que l’opérateur partiel $\widetilde{m}_g$ est fermé. Soit $(f_n, h_n)_{n\in\mathbf{N}}$ une suite dans $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ telle que la suite $(f_{\widetilde{n}},\widetilde{h}_n)$ des classes de $f_n$ et $h_n$ appartient au graphe de $\widetilde{m}_g$ et converge dans $L^{p_1}_K(X, \mu)\times L^{p_2}_K(X, \mu)$ quand $n$ tend vers l’infini. Soit $(f, h)$ un couple dans $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ tel que le couple $(\widetilde{f} ,\widetilde{h})$ de leurs classes est la limite de $(\widetilde{f}_n,\widetilde{h}_n)$.

Il existe une suite $(f_{n_k})_{k\in\mathbf{N}}$ extraite de la suite $(f_n)_n$ telle que $f_{n_k}(x)$ converge vers $f(x)$ pour $\mu$-presque tout $x$ (INT, IV, p. 131, § 3, n$^o4$, th. 3). Cela implique que $h_{n_k}(x) =g(x)f_{n_k}(x)$ converge $\mu$-presque partout vers $g(x)f(x)$. Par ailleurs la suite $(h_{n_k})$ converge vers $h$ dans l’espace $\mathscr{L}_K^{p_2}(X, \mu)$. Les fonctions $h$ et $gf$ sont donc égales $\mu$-presque partout (loc. cit.). Ainsi $\widetilde{f}$ appartient au domaine de $\widetilde{m}_g$ et $\widetilde{h}=\widetilde{m}_g(\widetilde{f})$. Cela démontre que $\widetilde{m}_g$ est fermé.

Démontrons que le domaine de $\widetilde{m}_g$ est dense dans $L^{p_1}_K(X, \mu)$. Il suffit de vérifier que les classes de fonctions $f\in \mathscr{K}(X; K)$ appartiennent à l’adhérence du domaine de $\widetilde{m}_g$ dans $L^{p_1}_K(X, \mu)$. Soit $f\in \mathscr{K}(X; K)$ et soit $\widetilde{f}$ sa classe dans $L^{p_1}_K(X, \mu)$. Pour tout entier $n\in \mathbf{N}$, notons $\varphi_n$ la fonction caractéristique de l’ensemble des éléments $x\in X$ tels que $|g(x)|\leqslant n$, et posons $f_n=f \varphi_n$. On a alors $|gf_n|\leqslant n|f|$, qui appartient à $\mathscr{L}_K^{p_2}(X, \mu)$, donc $f_n$ appartient au domaine de $\widetilde{m}_g$. Pour tout élément $x$ de X, la suite $(f_n(x))_{n\in\mathbf{N}}$ converge vers $f(x)$ quand $n\rightarrow +\infty$; de plus, on a $|f_n|\leqslant |f|$, qui appartient à $\mathscr{L}_K^{p_1}(X, \mu)$. D’après le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), la suite des classes de $f_n$ converge vers $\widetilde{f}$ dans $L^{p_1}_K(X, \mu)$. Ainsi, la classe de $f$ appartient à l’adhérence du domaine de $\widetilde{m}_g$.

Dans la proposition suivante, on suppose que $p_1=p_2= 2$.

#### Proposition 6 {#ts-iv-s4-prop-6 .statement tag=032Y}

a) Soit $g'$ une fonction $\mu$-mesurable sur X telle que $|g|\leqslant |g'|$. On a dom($\widetilde{m}_{g'}$)$\subset$ dom($\widetilde{m}_g$) et dom($\widetilde{m}_{g'}$) est un cœur de l’opérateur partiel $\widetilde{m}_g$;

b) Soit F un sous-espace de $\mathscr{L}_K^2(X, \mu)$ dont l’intersection avec $\mathscr{K}(X; K)$ est dense dans $\mathscr{K}(X; K)$ et dont l’image G dans $L^2_K(X, \mu)$ est contenue dans dom($\widetilde{m}_g$). Si $|g|^2$ est localement $\mu$-intégrable, alors $\mathscr{K}(X; K)$ est contenu dans le domaine de $\widetilde{m}_g$ et G est un cœur de $m_g$.

Démontrons a). Si $f\in \mathscr{L}_K^2(X, \mu)$ appartient au domaine de $m_{g'}$, de sorte que $f g'\in \mathscr{L}_K^2(X, \mu)$, l’hypothèse implique que $f g\in \mathscr{L}_K^2(X, \mu)$, d’où le résultat.

Démontrons que dom($\widetilde{m}_{g'}$) est un cœur de $\widetilde{m}_g$, c’est-à-dire que le domaine de $\widetilde{m}_{g'}$ est dense dans l’espace hilbertien $E_{\widetilde{m}_g}$. Soit $h\in \mathscr{L}_K^2(X, \mu)$

dont la classe $\widetilde{h}$ appartient à $E_{\widetilde{m}_g}$ et est orthogonale à dom($\widetilde{m}_{g'}$). Cela signifie que

$$
(\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh h'(1 +|g|^2)d\mu= 0
$$

pour toute fonction $h'\in \mathscr{L}_K^2(X, \mu)$ dont la classe $\widetilde{h}'$ appartient à dom($\widetilde{m}_{g'}$).

Soit C un sous-ensemble compact de X et soit $\varphi$ sa fonction caractéristique. Soit $n\in \mathbf{N}$. On note $\varphi_n$ la fonction caractéristique de l’ensemble $\mu$-intégrable $C_n$ des $x\in C$ tels que $|h(x)|\leqslant n$ et on pose $h'_n=\varphi_nh$. La classe de $h'_n$ appartient au domaine de $\widetilde{m}_{g'}$ puisque $|g'h'_n|\leqslant n\varphi$; il vient

$$
0 =\int_X\overline{h}h'_n(1 +|g|^2)d\mu=\int_X|h|^2\varphi_n(1 +|g|^2)d\mu
$$

Cela implique que $h$ est nulle pour $\mu$-presque tout $x\in C_n$ et donc, puisque $n$ est arbitraire, que $h$ est nulle pour $\mu$-presque tout $x\in C$. Il en résulte enfin que $h$ est nulle $\mu$-presque partout, puisque C est quelconque et que $h$ est modérée (INT, V, p. 9, § 1, n$^o3$, cor.).

Considérons maintenant l’assertion b). Comme $|g|^2$ est localement $\mu$-intégrable, la fonction $f g$ appartient à $\mathscr{L}_K^2(X, \mu)$ si $f\in \mathscr{K}(X; K)$, donc $\mathscr{K}(X; K)$ est contenu dans le domaine de $\widetilde{m}_g$.

Soit $h\in \mathscr{L}_K^2(X, \mu)$ dont la classe $\widetilde{h}$ appartient à $E_{m_g}$ et est orthogonal à G. On a alors

$$
0 = (\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh\overline{h}'(1 +|g|^2)d\mu
$$

pour tout $h'\in F$ de classe $\widetilde{h}'$. Compte tenu de l’hypothèse sur F, cela signifie que la mesure $h(1 +|g|^2)\cdot \mu$ est nulle, donc que $h$ est nulle $\mu$-presque partout puisque $h$ est modérée.

Soit $p$ un nombre réel $\geqslant 1$. Soit $h$ un élément de $\mathscr{L}_K^{\infty}(X, \mu)$. L’opérateur $\widetilde{m}_h$ de multiplication par $h$ est un endomorphisme de $L^p_K(X, \mu)$(IV, p. 186, n$^o5$). Supposons que l’ensemble Y des $x\in X$ tels que $h(x) = 0$ est localement $\mu$-négligeable. L’endomorphisme $\widetilde{m}_h$ est alors injectif (lemme 7 de IV, p. 186). Notons $h^{-1}$ la fonction sur X égale à 0 sur Y et à $x\mapsto 1/h(x)$ sur X- Y. L’opérateur partiel réciproque $\widetilde{m}^{-1}_h$ est l’opérateur de multiplication par $h^{-1}$ de $L^p_K(X, \mu)$ dans $L^p_K(X, \mu)$, c’est-à-dire que $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$. En effet, l’image de $\widetilde{m}_h$ est l’espace des classes des fonctions $g\in \mathscr{L}_K^p(X, \mu)$ de la forme $g=hf$ pour $f\in \mathscr{L}_K^p(X, \mu)$. Cette condition équivaut à $g(x)/h(x) =f(x)$ pour tout $x\in X$- Y et $g(x) = 0$ si $x\in Y$. Cela implique que le domaine de $\widetilde{m}^{-1}_h$ dans $L^p_K(X, \mu)$ est le domaine de $\widetilde{m}_{h^{-1}}$, et que l’égalité $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$ est valide.

Dans la suite, on notera parfois simplement $m_h$ l’opérateur partiel de multiplication par $h$ de $L^{p^1}_K(X, \mu)$ dans $L^{p_2}_K(X, \mu)$.

#### Exemple 2 {#ts-iv-s4-n3-exa-2 .statement tag=032Z}

Soient E un espace hilbertien sur K et $B = (e_i)_{i\in I}$ une base orthonormale de E. Soit $(\lambda_i)_{i\in I}$ une famille d’éléments de K. Soit D le sous-espace vectoriel de E formé des éléments $x\in E$ tels que la famille $(\lambda_i\langle e_i|x\rangle )_{i\in I}$ est de carré sommable dans K. L’espace D est dense dans E puisqu’il contient le vecteur $e_i$ pour tout $i\in I$. L’opérateur partiel $u$ de domaine D donné par

$$
x\mapsto \sum_{i\in I}\lambda_i\langle e_i|x\rangle e_i
$$

est appelé un opérateur partiel diagonal dans la base B, et $(\lambda_i)_{i\in I}$ est appelée la famille des valeurs propres de $u$.

L’opérateur $u$ est fermé. En effet, soit $(x_n, u(x_n))_{n\in\mathbf{N}}$ une suite d’éléments du graphe de $u$ qui converge dans $E\times E$, et soit $(x, y)$ sa limite. On a alors $\langle e_i|x_n\rangle  \rightarrow  \langle e_i|x\rangle$ pour tout $i\in I$ et

$$
\langle e_i|u(x_n)\rangle =\lambda_i\langle e_i|x_n\rangle  \rightarrow  \langle e_i|y\rangle
$$

pour tout $i\in I$. Par conséquent, $\lambda_i\langle e_i|x\rangle =\langle e_i|y\rangle$ pour tout $i\in I$, ce qui démontre que $x\in D$ et $u(x) =y$, c’est-à-dire que $u$ est fermé.

Cet exemple est en fait un cas particulier du précédent, appliqué à l’espace topologique X = I muni de la topologie discrète et de la mesure de comptage $\mu$, puisque E s’identifie à l’espace $\ell^2(I) = L^2(I, \mu)$ par l’application $x\mapsto (\langle e_i|x\rangle )_{i\in I}$ (EVT, V, p. 23, cor. 2) et $u$ s’identifie alors à l’opérateur de multiplication $m_{\lambda}$, où $\lambda$ est la fonction $i\mapsto \lambda_i$.

#### Exemple 3 {#ts-iv-s4-n3-exa-3 .statement tag=0330}

L’ensemble $\mathbf{N}_{\mathbf{R}}=\mathbf{N}\cup  \{\infty , \omega \}$ est muni de l’ordre total décrit dans VAR, R2, p. 10, tel que $n <\infty < \omega$ pour tout $n\in \mathbf{N}$. Soit $r\in \mathbf{N}_{\mathbf{R}}$. Soient $n\in \mathbf{N}$ et U un ouvert de $\mathbf{R}^n$. Soit $k\in \mathbf{N}$ tel que $k\leqslant r$. Soit $(n_{\alpha})_{|\alpha|\leqslant k}$ une famille d’éléments de $\mathscr{C}^r$(U), où les multi-indices considérés appartiennent à $\mathbf{N}^n$. La famille $(n_{\alpha})$ définit un opérateur différentiel scalaire D d’ordre $\leqslant k$ sur U (cf. VAR, R2, 14.1.6, 14.1.4). Pour tout entier $m$ tel que $k\leqslant m\leqslant r$, l’opérateur différentiel D définit une application linéaire de $C^m(U)$ dans $C^{m-k}(U)$ qui envoie $f\in C^m(U)$ sur

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}(f)
$$

La même formule définit une application linéaire continue de $\mathscr{D}(U)$ dans $\mathscr{D}'(U)$ (déf. 2 de IV, p. 208).

#### Définition 5 {#ts-iv-s4-def-5 .statement tag=0331}

Soit E un sous-espace vectoriel de $\mathscr{D}'(U)$ contenant $\mathscr{D}(U)$. On appelle opérateur différentiel associé à D sur E tout opérateur partiel sur E qui est une extension de l’opérateur partiel de domaine $\mathscr{D}(U)$ défini par $\varphi \mapsto D(\varphi )$.

Supposons par exemple que les coefficients $n_{\alpha}$ sont des fonctions bornées sur U. Soit $\mu$ la mesure de Lebesgue sur U. Si $p$ est un élément de $[1,+\infty [$, on peut alors définir un opérateur différentiel sur $L^p(U)$ associé à D dont le domaine est l’espace de Sobolev $W^{k,p}(U)$ (n$^o14$ de IV, p. 221), puisque dans ce cas on a $n_{\alpha}\partial^{\alpha}(f)\in L^p(U)$ pour tout $f\in W^{k,p}(U)$ et tout $|\alpha |\leqslant k$.

### 4. Adjoint

Dans ce numéro, K est l’un des corps $\mathbf{R}$ ou $\mathbf{C}$, et E et F désignent des espaces hilbertiens sur K.

Soit $u$ un opérateur à domaine dense de E dans F. Notons D le domaine de $u$. Pour $y\in F$, soit $\lambda_y$ la forme linéaire sur D telle que $\lambda_y(x) =\langle y|u(x)\rangle$ pour tout $x\in D$. On note $D^*$ l’ensemble des vecteurs $y\in F$ tels que $\lambda_y$ est continue sur D. C’est un sous-espace vectoriel de F. Soit $y\in D^*$; comme D est dense dans E, la forme linéaire $\lambda_y$ s’étend de manière unique en une forme linéaire continue sur E, que l’on note encore $\lambda_y$. D’après EVT, V, p. 15, th. 3, il existe un unique élément $u^*(y)$ dans E tel que $\lambda_y(x) =\langle u^*(y)|x\rangle$ pour tout $x\in E$. L’application $y\mapsto u^*(y)$ est linéaire de $D^*$ dans E.

#### Définition 6 {#ts-iv-s4-def-6 .statement tag=0332}

L’opérateur partiel de F dans E de domaine $D^*$ défini par $y\mapsto u^*(y)$ est appelé l’ adjoint de $u$. Il est noté $u^*$.

#### Remarque {#ts-iv-s4-n4-rem-9 .statement tag=0333}

On a donc $y\in D^*$ si et seulement s’il existe $c\in \mathbf{R}_+$ tel que $|\langle y|u(x)\rangle |\leqslant c\|x\|$ pour tout $x\in D$. L’élément $u^*(y)$ est alors caractérisé par la relation

$$
\langle y|u(x)\rangle =\langle u^*(y)|x\rangle \tag{1}
$$

pour tout $x\in D$. On a alors $|\langle y|u(x)\rangle |\leqslant \|u^*(y)\| \|x\|$ pour tout $x\in D$.

Dans le cas où $u$ est une application linéaire continue de E dans F, son adjoint au sens de la définition précédente coïncide avec l’adjoint défini dans EVT, V, p. 38, déf. 1, puisque $D^*$ est égal à F dans ce cas.

Soit $v\in \mathscr{P}(E; F)$ tel que $u\subset v$. On a alors $v^*\subset u^*$.

Soit $v\in \mathscr{P}(E; F)$ tel que $u+v$ est à domaine dense. L’opérateur partiel $v$ est alors à domaine dense et on a $u^*+v^*\subset (u+v)^*$. En général, il n’y a pas égalité (exercice 9 de IV, p. 347). Si $v\in \mathscr{L}(E; F)$, alors $u+v$ est à domaine dense et $(u+v)^*=u^*+v^*$. C’est le cas, par exemple, si F = E et si $v=\lambda 1_E$ où $\lambda \in K$.

Soit G un espace hilbertien sur K et soit $v\in \mathscr{P}(F; G)$ un opérateur à domaine dense. Si $v\circ u$ est à domaine dense, alors $u^*\circ v^*\subset (v\circ u)^*$. En général, il n’y a pas égalité (loc. cit.). Si $u$ (resp. $v)$ est un isomorphisme, alors $v\circ u$ est à domaine dense et on a $(v\circ u)^*=u^*\circ v^*$. C’est le cas, par exemple, si E = F (resp. F = G) et $u=\lambda 1_E$ (resp. $v=\lambda 1_F)$ où $\lambda \in K^*$.

On note $s$ l’isomorphisme isométrique d’espaces hilbertiens de $E\oplus F$ dans $F\oplus E$ défini par $s(x, y) = (-y, x)$ pour tout $(x, y)\in E\oplus F$.

#### Proposition 7 {#ts-iv-s4-prop-7 .statement tag=0334}

Soit $u$ un opérateur partiel à domaine dense de E dans F.

a) Le graphe de $u^*$ est égal à $s(\Gamma^{\circ}_u) =s(\Gamma_u)^{\circ}$;

b) L’opérateur partiel $u^*$ est fermé;

c) Le noyau de $u^*$ est l’orthogonal de l’image de $u$.

Notons $W =s(\Gamma_u)^{\circ}$. Comme l’application linéaire $s$ est unitaire, on a $W =s(\Gamma^{\circ}_u)$.

On a $(y, x)\in W$ si et seulement si

$$
\langle (y, x)|(-u(x'), x')\rangle = 0
$$

pour tout $x'\in$ dom($u$), c’est-à-dire si

$$
\langle y|u(x')\rangle =\langle x|x'\rangle
$$

pour tout $x'\in$ dom($u$). Lorsque $y\in$ dom($u^*$) et $x=u^*(y)$, cette propriété est vraie (cf. formule (1), p. 236). Réciproquement, si cette condition est valide, on en déduit que $|\langle y|u(x')\rangle |\leqslant \|x\| \|x'\|$ pour tout $x'\in$ dom($u$), ce qui entraîne que $y$ appartient à dom($u^*$); on a alors $u^*(y) =x$. Donc $W = \Gamma_{u^*}$.

L’opérateur $u^*$ est fermé, car l’espace $s(\Gamma_u)^{\circ}$ est fermé dans $F\oplus E$.

Démontrons l’assertion c). Si $y$ est orthogonal à l’image de $u$, la forme linéaire $\lambda_y:x\mapsto  \langle y|u(x)\rangle$ sur D est nulle, donc $y\in$ dom($u^*$) et $u^*(y) = 0$. Réciproquement, soit $y\in$ dom($u^*$). On a alors $u^*(y) = 0$ si et seulement si $y$ est orthogonal à $u(x)$ pour tout $x\in D$ (formule (1), p. 236).

#### Proposition 8 {#ts-iv-s4-prop-8 .statement tag=0335}

Soit $u$ un opérateur à domaine dense de E dans F. Alors $u^*$ est à domaine dense si et seulement si $u$ est fermable. Lorsque c’est le cas, la fermeture $\overline{u}$ de $u$ est égale à $u^{**}$, et l’adjoint de $\overline{u}$ est égal à $u^*$.

D’après la prop. 7, l’opérateur partiel $u^*$ est fermé. Supposons que le domaine $D^*$ de $u^*$ est dense dans F. Soit $u^{**}$ l’adjoint de $u^*$; c’est un opérateur partiel fermé de E dans F. Démontrons que $u\subset u^{**}$, ce qui impliquera que $u$ est fermable. Soit $x\in$ dom($u$). Par définition de $u^*$, les formes linéaires sur $D^*$ données par $y\mapsto  \langle x|u^*(y)\rangle$ et $y\mapsto  \langle u(x)|y\rangle$ sont égales ; on a donc $x\in$ dom($u^{**}$) et $u^{**}(x) =u(x)$, d’où l’assertion.

Réciproquement, supposons que $u$ est fermable ; on a $\Gamma_{\overline{u}}=\overline{\Gamma}_u$ (prop. 1 de IV, p. 228). Soit $y\in F$ un vecteur orthogonal à dom($u^*$). L’élément $(y,0)$ de $F\oplus E$ appartient alors à l’orthogonal du graphe de $u^*$. Or, d’après la prop. 7, a), on a

$$
\Gamma^{\circ}_{u^*}= (s(\Gamma_u)^{\circ})^{\circ}=s(\Gamma_u) =s(\Gamma_u)
$$

Il vient donc $(0, y)\in \Gamma_{\overline{u}}$, d’où $y=\overline{u}(0) = 0$. L’orthogonal de dom($u^*$) étant réduit à 0, l’espace dom($u^*$) est dense dans F.

Finalement, la prop. 7, appliquée à $u^*$, implique que

$$
\Gamma_{u^{**}}=s^{-1}(\Gamma^{\circ}_{u^*}) =s^{-1}(s(\Gamma^{\circ \circ}_u)) =\overline{\Gamma}_u
$$

donc $u^{**}=\overline{u}$, puis $\overline{u}^*= (u^*)^{**}=\overline{u^*}=u^*$ comme $u^*$ est fermé.

#### Corollaire {#ts-iv-s4-n4-cor-1 .statement tag=0336}

Si $u$ est un opérateur partiel fermé à domaine dense de E dans F, alors $u^*$ est à domaine dense et on a $u^{**}=u$.

#### Définition 7 {#ts-iv-s4-def-7 .statement tag=0337}

Soit $u$ un opérateur partiel sur E. On dit que $u$ est symétrique si $u$ est à domaine dense et si $u^*$ est une extension de $u$. On dit que $u$ est auto-adjoint si $u$ est à domaine dense et $u^*=u$. On dit que $u$ est essentiellement auto-adjoint s’il est fermable et si la fermeture $\overline{u}$ de $u$ est auto-adjointe.

On dit que $u$ est un opérateur partiel minoré si $u$ est symétrique et s’il existe un nombre réel $c$ tel que $\langle x|u(x)\rangle \geqslant c\|x\|^2$ pour tout $x$ appartenant au domaine de $u$. On dit alors que $c$ est un minorant de $u$. Si $c= 0$, on dit aussi que $u$ est un opérateur partiel positif.

On note $\mathscr{A}(E)$ l’ensemble des opérateurs partiels auto-adjoints sur E.

#### Remarque 1 {#ts-iv-s4-n4-rem-1 .statement tag=0338}

Pour qu’un opérateur $u$ à domaine dense sur E soit symétrique, il faut et il suffit que l’on ait

$$
\langle x|u(y)\rangle =\langle u(x)|y\rangle \tag{2}
$$

pour tout $(x, y)\in$ dom($u$)$^2$. Cette formule démontre en effet que le domaine de $u$ est contenu dans celui de $u^*$, puis que $u^*$ et $u$ coïncident sur le domaine de $u$. En particulier, il en résulte que $\langle x|u(x)\rangle  \in \mathbf{R}$ pour tout $x\in$ dom($u$).

Comme on le verra dans différents exemples, la formule (2) peut souvent être vérifiée par un calcul sans malice. Par contre, la détermination exacte du domaine de l’adjoint, qui permet seule de savoir si un opérateur symétrique est auto-adjoint ou non, peut être très délicate.

#### Remarque 2 {#ts-iv-s4-n4-rem-2 .statement tag=0339}

Un opérateur partiel auto-adjoint $u$ est essentiellement auto-adjoint (cf. prop. 8).

#### Remarque 3 {#ts-iv-s4-n4-rem-3 .statement tag=033A}

Soit $u$ un opérateur partiel symétrique sur E. L’opérateur $u$ est fermable (prop. 7, b)). Il vérifie dom($u$)$\subset$ dom($u^*$), et $u$ est auto-adjoint si et seulement si dom($u$) $=$ dom($u^*$). De plus, la fermeture $\overline{u}$ de $u$ est symétrique puisque $\overline{u}\subset u^*=\overline{u}^*$ (prop. 8).

#### Remarque 4 {#ts-iv-s4-n4-rem-4 .statement tag=033B}

Supposons $K =\mathbf{C}$. Soit $u\in \mathscr{P}(E; E)$ un opérateur partiel à domaine dense. La condition $\langle x|u(x)\rangle  \in \mathbf{R}$ pour tout $x\in$ dom($u$) implique que $u$ est symétrique (EVT, V, p. 2, remarque) ; en particulier, si $\langle x|u(x)\rangle  \in \mathbf{R}_+$ pour tout $x\in$ dom($u$), alors $u$ est positif.

#### Remarque 5 {#ts-iv-s4-n4-rem-5 .statement tag=033C}

Soient $u$ et $v$ des opérateurs partiels symétriques sur E. Si $u$ est auto-adjoint et si $u\subset v$, alors $v\subset v^*\subset u^*=u$, donc $u=v$.

#### Remarque 6 {#ts-iv-s4-n4-rem-6 .statement tag=033D}

Un opérateur partiel essentiellement auto-adjoint $u$ est symétrique, puisque $u\subset \overline{u}$ implique $\overline{u}=\overline{u}^*\subset u^*$, donc $u\subset u^*$.

#### Remarque 7 {#ts-iv-s4-n4-rem-7 .statement tag=033E}

Soient $u$ et $v$ des opérateurs partiels symétriques sur E. Si $u+v$ est à domaine dense, par exemple si $u$ ou $v$ appartient à $\mathscr{L}$ (E), alors $u+v$ est symétrique. En général, l’opérateur partiel $u+v$ n’est pas auto-adjoint, même si $u$ et $v$ le sont (exercice 9 de IV, p. 347).

#### Remarque 8 {#ts-iv-s4-n4-rem-8 .statement tag=033F}

Soit $u$ un opérateur partiel symétrique sur E. Un nombre réel $c$ est un minorant de $u$ si et seulement si l’opérateur $u-c\cdot 1_E$ est positif.

#### Lemme 3 {#ts-iv-s4-lem-3 .statement tag=033G}

Supposons que $K =\mathbf{R}$. Soit $u$ un opérateur partiel à domaine dense de E dans F.

a) L’adjoint de $u_{(\mathbf{C})}$ est $(u^*)_{(\mathbf{C})}$;

b) Supposons que E = F ; l’opérateur partiel $u$ est symétrique (resp. auto-adjoint) si et seulement si l’opérateur partiel $u_{(\mathbf{C})}$ est symétrique (resp. auto-adjoint).

Démontrons a). Soit $y\in F_{(\mathbf{C})}$ et écrivons $y=y_1+iy_2$ avec $y_1,y_2\in F$. Pour tous $(x_1, x_2)\in E\times E$, on a

$$
\langle u_{(\mathbf{C})}(x_1+ix_2)|y\rangle =\langle u(x_1)|y_1\rangle +i\langle u(x_1)|y_2\rangle
$$

$$
-i\langle u(x_2)|y_1\rangle +\langle u(x_2)|y_2\rangle
$$

Si $y\in$ dom($u^*$)$_{(\mathbf{C})}$, on en déduit que $y\in$ dom(($u_{(\mathbf{C})}$)$^*)$ et que $u^*_{(\mathbf{C})}(y) = (u_{(\mathbf{C})})^*(y)$, donc $u^*_{(\mathbf{C})}\subset (u_{(\mathbf{C})})^*$.

Réciproquement, supposons que $y$ est dans dom(($u_{(\mathbf{C})}$)$^*)$. Si on prend $x_2= 0$ (resp. $x_1= 0)$ dans la formule ci-dessus, on vérifie que $y_1\in$ dom($u^*$) (resp. que $y_2\in$ dom($u^*$)), d’où $y\in$ dom($u^*$)$_{(\mathbf{C})}$.

L’assertion a) implique que $u_{(\mathbf{C})}$ est symétrique (resp. auto-adjoint) si $u$ l’est.

Réciproquement, supposons que $u_{(\mathbf{C})}$ est symétrique. La relation $\langle u(x)|y\rangle =\langle x|u(y)\rangle$ pour tout $(x, y)\in$ dom($u_{(\mathbf{C})}$)$\times$ dom($u_{(\mathbf{C})}$) implique que $u$ est symétrique en prenant $x$ et $y$ dans le sous-espace dom($u$) de dom($u_{(\mathbf{C})}$). Si $u_{(\mathbf{C})}$ est auto-adjoint, ce qui précède démontre que $u$ est symétrique ; comme dom($u^*$) $=$ dom($u^*_{(\mathbf{C})}$)$\cap F$, l’assertion a) implique que dom($u^*$) $=$ dom($u_{(\mathbf{C})}$)$\cap F =$ dom($u$), donc $u$ est auto-adjoint.

### 5. Critères élémentaires pour les opérateurs auto-adjoints

#### Proposition 9 {#ts-iv-s4-prop-9 .statement tag=033H}

Soit $v\in \mathscr{L}(F; E)$ une application linéaire continue injective de F dans E dont l’image est dense dans E. L’adjoint de $v$ est une application linéaire continue injective de E dans F et on a $(v^*)^{-1}= (v^{-1})^*$. En particulier, si E = F, l’endomorphisme $v$ est hermitien si et seulement si l’opérateur partiel $v^{-1}$ est auto-adjoint.

L’opérateur partiel $v^{-1}$ est un opérateur fermé à domaine dense de E dans F (exemple 2 de IV, p. 228) et l’adjoint $v^*$ de $v$ est une application linéaire continue de E dans F ; elle est injective, puisque l’image de $v$ est dense dans E (EVT, V, p. 41, prop. 4). Soit $s$ (resp. $s')$ l’isomorphisme isométrique $(x, y)\mapsto (-y, x)$ de $E\oplus F$ sur $F\oplus E$ (resp. l’isomorphisme isométrique $(y, x)\mapsto (-x, y)$ de $F\oplus E$ sur $E\oplus F)$ et soit $\iota$ (resp. $\iota ')$ l’isomorphisme isométrique $(y, x)\mapsto (x, y)$ de $F\oplus E$ sur $E\oplus F$ (resp. l’isomorphisme isométrique $(x, y)\mapsto (y, x)$ de $E\oplus F$ sur $F\oplus E)$. On a alors $s\circ \iota =-\iota '\circ s'$, d’où

$$
\Gamma_{(v^{-1})^*}=s(\Gamma_{v^{-1}})^{\circ}=s(\iota (\Gamma_v))^{\circ}=-\iota '(s'(\Gamma_v))^{\circ}=-\iota '(\Gamma_{v^*}) = \Gamma_{(v^*)^{-1}}
$$

d’après la prop. 7 de IV, p. 236. La proposition en résulte.

#### Proposition 10 (Hellinger–Toeplitz) {#ts-iv-s4-prop-10 .statement tag=033I}

Soit $u$ un opérateur partiel symétrique sur l’espace hilbertien E. Si le domaine de $u$ est égal à E, alors $u\in \mathscr{L}(E)$ et $u$ est hermitien.

En effet, l’opérateur partiel $u$ est fermable (prop. 8 de IV, p. 237), et donc fermé puisque son domaine est E (IV, p. 228, remarque). On conclut alors en invoquant EVT, I, p. 19, cor. 5.

#### Corollaire {#ts-iv-s4-n5-cor-1 .statement tag=033J}

Soit $u$ un opérateur partiel symétrique sur E. Si l’opérateur partiel $u$ induit une application linéaire bijective de dom($u$) dans E, alors $u$ est auto-adjoint.

En effet, l’opérateur partiel $u^{-1}$ réciproque de $u$ est symétrique de domaine E (prop. 9), donc $u^{-1}$ est un élément auto-adjoint de $\mathscr{L}(E)$ (prop. 10), et $u$ est alors hermitien (prop. 9).

#### Proposition 11 {#ts-iv-s4-prop-11 .statement tag=033K}

Soit $u$ un opérateur partiel symétrique sur E et soit $\lambda \in \mathbf{C}$. Si $u+\lambda 1_E$ et $u+\lambda 1_E$ sont surjectifs, alors $u$ est auto-adjoint.

Il suffit de démontrer que dom($u^*$)$\subset$ dom($u$). Soit $x\in$ dom($u^*$). Il existe par hypothèse $y\in$ dom($u$) tel que $u(y) +\lambda y=u^*(x) +\lambda x$. Démontrons que $y=x$. Pour tout $z\in$ dom($u$), il vient

$$
\langle (u+\lambda 1_E)(z)|x\rangle =\langle z|(u^*+\overline{\lambda}1_E)(x)\rangle
$$

$$
=\langle z|(u+\overline{\lambda}1_E)(y)\rangle =\langle (u+\lambda 1_E)(z)|y\rangle
$$

puisque $u$ est symétrique. Comme l’opérateur $u+\lambda 1_E$ est surjectif, on a bien $y=x$, donc $x\in$ dom($u$).

Nous verrons plus loin (cf. prop. 17 de IV, p. 248) que si $\lambda \in \mathbf{C}-\mathbf{R}$, alors la réciproque est vraie.

#### Proposition 12 {#ts-iv-s4-prop-12 .statement tag=033L}

Soit $u$ un opérateur fermé à domaine dense de E dans F. L’opérateur partiel $u^*\circ u$ sur E est auto-adjoint et positif. Son domaine est un cœur pour $u$.

Notons $v$ l’opérateur partiel $1_E+u^*\circ u$. Son domaine est dom($u^*\circ u$), qui est contenu dans dom($u$). Pour tous $x\in$ dom($u$) et $y\in$ dom($v$), on a $u(y)\in$ dom($u^*$) et

$$
\langle x|v(y)\rangle =\langle x|y\rangle +\langle x|(u^*\circ u)(y)\rangle =\langle x|y\rangle +\langle u(x)|u(y)\rangle \tag{3}
$$

$$
\langle y|v(y)\rangle =\|y\|^2+\|u(y)\|^2 \tag{4}
$$

La formule (4) implique que l’opérateur partiel $v$ est injectif. Par ailleurs, d’après la prop. 7 de IV, p. 236, a), on a $F\oplus E = \Gamma_{u^*}\oplus s(\Gamma_u)$. Soit $x\in E$. Il existe $y'\in$ dom($u^*$) et $x'\in$ dom($u$) tels que

$$
(0, x) = (y', u^*(y')) + (-u(x'), x') = (y'-u(x'), x'+u^*(y'))
$$

On a donc $y'=u(x')$, d’où $x'\in$ dom($u^*\circ u$) $=$ dom($v$) et

$$
x=x'+u^*(y') =x'+ (u^*\circ u)(x') =v(x')
$$

L’opérateur partiel $v$ sur E est donc surjectif, et induit une application linéaire bijective de dom($v$) dans E.

Soit $x\in E$ orthogonal à dom($v$). Écrivons $x=v(x')$ où $x'\in$ dom($v$). D’après la formule (4), on obtient

$$
0 =\langle x'|x\rangle =\langle x'|v(x')\rangle =\|x'\|^2+\|u(x')\|^2
$$

d’où $x'= 0$, puis $x= 0$. Le domaine de $v$ est donc dense dans E.

L’opérateur partiel $v$ est à domaine dense ; il est bijectif et la formule (3) démontre qu’il est symétrique. On conclut que $v$ est auto-adjoint en appliquant le corollaire de la proposition 10. Par conséquent, $u^*\circ u=v-1_E$ est auto-adjoint. De plus, la formule

$$
\langle x|(u^*\circ u)(x)\rangle =\|u(x)\|^2
$$

pour tout $x\in$ dom($u^*\circ u$) implique que $u^*\circ u$ est positif.

Finalement, soit $y\in E_u$ orthogonal à dom($u^*\circ u$). Il existe un élément $x$ dans le domaine de $u^*\circ u$ tel que $y=v(x) =x+ (u^*\circ u)(x)$. On a alors $0 = (x|y)_u=\langle y|y\rangle$, d’où $y= 0$.

### 6. Opérateurs différentiels

Soient $n\in \mathbf{N}$ et U un ouvert de $\mathbf{R}^n$. On munit $\mathbf{R}^n$ et U de la mesure de Lebesgue notée $\mu$.

Soient $k\in \mathbf{N}$ et $h\in \mathbf{N}$ tels que $h\geqslant k$. Soit D un opérateur différentiel scalaire sur U d’ordre $\leqslant k$, à coefficients $(n_{\alpha})_{|\alpha|\leqslant k}$ de classe $C^h$ sur U. On suppose que pour tout $\alpha$ tel que $|\alpha |\leqslant k$ et tout $\beta$ tel que $0\leqslant \beta \leqslant \alpha$, la fonction $\partial^{\beta}n_{\alpha}$ est bornée sur U.

Soit $^tD$ l’opérateur différentiel scalaire sur U transposé de D (VAR, R2, 14.3.2) ; il est d’ordre $\leqslant k$ et de classe $C^{h-k}$; pour $\varphi \in \mathscr{D}$(U), on a

$$
^tD(\varphi ) =\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\partial^{\alpha}(\overline{n}_{\alpha}\varphi )
$$

(loc. cit.) ; en particulier, les coefficients de $^tD$ sont bornés sur U.

On note $D_-$ l’opérateur partiel sur $L^2(U)$ de domaine $\mathscr{D}(U)$ défini par

$$
\varphi \mapsto D(\varphi ) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}\varphi \tag{5}
$$

Soit $H_D$ l’espace des $f\in L^2(U)$ telles que la distribution

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}f
$$

appartient à $L^2(U)$; on note $D_+$ l’opérateur partiel de domaine $H_D$ défini par $f\mapsto D(f)$.

Puisqu’on a $\partial^{\alpha}f\in L^2(U)$ si $f\in H^k(U)$ et $|\alpha |\leqslant k$, l’espace de Sobolev $H^k(U)$ est contenu dans $H_D$; en général, ces espaces sont distincts.

On a $D_-\subset D_+$, et ce sont des opérateurs différentiels associés à D sur $L^2(U)$ (déf. 5 de IV, p. 235).

#### Proposition 13 {#ts-iv-s4-prop-13 .statement tag=033M}

Soit $u$ un opérateur partiel sur $L^2(U)$. Si que $D_-\subset u\subset D_+$, alors $u$ est fermable et $(^tD)_-\subset u^*\subset (^tD)_+$.

Soient $\varphi$ et $\psi$ dans $\mathscr{D}(U)$. On a alors

$$
\langle \varphi |D(\psi )\rangle =\sum_{|\alpha|\leqslant}\int_{kU}n_{\alpha}\varphi  \partial^{\alpha}\psi  d\mu
$$

$$
=\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}\varphi )|\psi \rangle =\langle^tD(\varphi )|\psi \rangle
$$

(cf. VAR, R2, 14.3.8). Puisque $\mathscr{D}(U)$ est dense dans $L^2(U)$ (prop. 4 de IV, p. 202), cela implique que $\varphi \in$ dom($u^*$) et $u^*(\varphi ) =^tD(\varphi )$. On a donc $(^tD)_-\subset u^*$; en particulier, $u^*$ est à domaine dense et $u$ est fermable (prop. 8 de IV, p. 237).

Soient $f\in$ dom($u^*$) et $\varphi \in \mathscr{D}(U)$. Puisque $\mathscr{D}(U)\subset$ dom($u$), la distribution associée à $u^*(f)$ vérifie

$$
\langle u^*(f), \varphi \rangle =\langle \overline{\varphi}|u^*(f)\rangle =\langle u(\overline{\varphi})|f\rangle
$$

Comme $D_-\subset u$, on calcule $u(\overline{\varphi})$ par la formule (5), d’où

$$
\langle u^*(f), \varphi \rangle =\sum_{\alpha}\langle n_{\alpha}\partial^{\alpha}\overline{\varphi}|f\rangle =\sum_{\alpha}\langle \partial^{\alpha}\overline{\varphi}|\overline{n}_{\alpha}f\rangle
$$

$$
=\sum_{\alpha}\langle \overline{n}_{\alpha}f, \partial^{\alpha}\varphi \rangle =\sum_{\alpha}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}f), \varphi \rangle =\langle^tD(f), \varphi \rangle
$$

Les distributions $u^*(f)$ et $^tD(f)$ sont donc égales ; la distribution $f$ appartient donc à $H_{_tD}$ et $u^*(f) =^tD(f)$, d’où $u^*\subset (^tD)_+$.

#### Remarque {#ts-iv-s4-n6-rem-1 .statement tag=033N}

La proposition signifie que l’adjoint d’un opérateur partiel $u$ tel que $D_-\subset u\subset D_+$ peut toujours se calculer au sens des distributions : les éléments $f$ du domaine de $u^*$ sont des éléments de $L^2(U)$ tels que la distribution $^tD(f)$ appartient à $L^2$(U), et on a $u^*(f) =^tD(f)$.

On dit que D est formellement symétrique si $^tD = D$ en tant qu’opérateur différentiel scalaire. Si c’est le cas, l’opérateur partiel $D_-$ est symétrique.

Considérons le cas particulier de l’opérateur différentiel scalaire d’ordre 2 défini par

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

On appelle laplacien sur U tout opérateur partiel $u$, auto-adjoint sur $L^2$(U), tel que $\Delta_-\subset u($cf. VAR, R2, 14.4.3, p. 83). Nous verrons plus loin (IV, p. 261, exemple) qu’il existe toujours au moins un laplacien sur $L^2(U)$; il peut en exister plus d’un (exercice 17 de IV, p. 358).

### 7. Spectre et résolvante

#### Lemme 4 {#ts-iv-s4-lem-4 .statement tag=033O}

Soit E un espace de Banach complexe et soit $u$ un opérateur partiel fermé injectif sur E tel que $u^{-1}\in \mathscr{L}(E)$. Soit $v\in \mathscr{L}(E)$ tel que $\|v\|<\|u^{-1}\|^{-1}$. Alors l’opérateur partiel $u+v$ est injectif, on a $(u+v)^{-1}\in \mathscr{L}(E)$ et

$$
(u+v)^{-1}=u^{-1}\circ \sum_{k=0}^{+\infty}(-vu^{-1})^k \tag{6}
$$

où la série est absolument convergente dans $\mathscr{L}(E)$. De plus, on a

$$
\|(u+v)^{-1}\|\leqslant \|u^{-1}\|_{-1}
$$

$$
1- \|v\| \|u\|
$$

Comme $\|v\| \|u^{-1}\|<1$, la série de terme général $(-vu^{-1})^k$ est absolument convergente dans $\mathscr{L}$ (E), et sa somme est l’inverse de l’endomorphisme $1_E+vu^{-1}$ (prop. 2 de I, p. 22). Par conséquent, l’opérateur partiel $(1_E+vu^{-1})\circ u=u+v($IV, p. 226, rem. vi) est injectif et l’opérateur partiel réciproque $(u+v)^{-1}=u^{-1}\circ (1_E+vu^{-1})^{-1}($IV, p. 226, rem. iii) appartient à $\mathscr{L}(E)$. Comme

$\|(1_E+vu^{-1})^{-1}\|\leqslant \sum^{+\infty}(\|v\| \|u^{-1}\|)^k=$ 1 $_{-1}$,

$$
1- \|v\| \|u\|
$$

$k=0$

le lemme est démontré.

#### Définition 8 {#ts-iv-s4-def-8 .statement tag=033P}

Soit $u$ un opérateur fermé à domaine dense sur un espace de Banach complexe E. L’ensemble résolvant de $u$ est l’ensemble des nombres complexes $\lambda$ tels que l’opérateur partiel $\lambda 1_E-u$ est injectif et son inverse $(\lambda 1_E-u)^{-1}$ appartient à $\mathscr{L}(E)$.

Le spectre de $u$, noté Sp($u$), est le complémentaire de l’ensemble résolvant dans $\mathbf{C}$.

Si $\lambda \in \mathbf{C}-$ Sp($u$), on note $R(u, \lambda )\in \mathscr{L}(E)$ l’inverse de $\lambda 1_E-u$. L’application de $\mathbf{C}-$ Sp($u$) dans $\mathscr{L}(E)$ qui à $\lambda$ associe $R(u, \lambda )$ est appelée la résolvante de $u$.

#### Remarque {#ts-iv-s4-n7-rem-1 .statement tag=033Q}

Soit E un espace de Banach complexe et soit $u$ un opérateur fermé à domaine dense sur E.

1) Si $u\in \mathscr{L}$ (E), son spectre coïncide avec le spectre de l’élément $u$ de l’algèbre $\mathscr{L}(E)$(I, p. 2, déf. 1).

2) Soit D le domaine de $u$. Pour tout $\lambda \in \mathbf{C}-$ Sp($u$), on a

$$
1_E= (\lambda 1_E-u)\circ R(u, \lambda ),1_D= R(u, \lambda )\circ (\lambda 1_E-u) \tag{7}
$$

De plus, pour $\lambda_1$ et $\lambda_2$ dans l’ensemble résolvant de $u$, on a

$$
R(u, \lambda_1)-R(u, \lambda_2) = (\lambda_2-\lambda_1)R(u, \lambda_2)\circ R(u, \lambda_1) \tag{8}
$$

$$
R(u, \lambda_1)\circ R(u, \lambda_2) = R(u, \lambda_2)\circ R(u, \lambda_1) \tag{9}
$$

En effet, on a

$$
R(u, \lambda_1)-R(u, \lambda_2) = R(u, \lambda_1)\circ 1_E-1_D\circ R(u, \lambda_2)
$$

Puisque $1_E= (\lambda_21_E-u)\circ R(u, \lambda_2)$ et $1_D= R(u, \lambda_1)\circ (\lambda_11_E-u)$, on obtient

$$
R(u, \lambda_1)-R(u, \lambda_2) =\lambda_2R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
-R(u, \lambda_1)\circ u\circ R(u, \lambda_2)-\lambda_1R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
+ R(u, \lambda_1)\circ u\circ R(u, \lambda_2)
$$

d’où la première formule. En échangeant le rôle de $\lambda_1$ et $\lambda_2$, on en déduit la seconde formule.

3) Soit $\lambda \in \mathbf{C}$. D’après le théorème du graphe fermé (EVT, I, p. 19, cor. 5), si l’application linéaire de dom($u$) dans E définie par $x\mapsto (\lambda 1_E-u)(x)$ est bijective, alors son inverse, dont le graphe est fermé, est continue de E dans E. Donc $\lambda$ appartient à l’ensemble résolvant de $u$ si et seulement si l’application $x\mapsto (\lambda 1_E-u)(x)$ de dom($u$) dans E est bijective.

4) Si $\lambda$ appartient au spectre de $u$, une des propriétés suivantes est valide :

(i) Le noyau de $\lambda 1_E-u$ n’est pas réduit à 0 ; on dit alors que $\lambda$ est une valeur propre de $u$, et que la dimension de Ker($\lambda 1_E-u$) est sa multiplicité ;

(ii) L’opérateur partiel $\lambda 1_E-u$ est injectif et son image n’est pas dense dans E ; on dit que $\lambda$ appartient au spectre résiduel de $u$;

(iii) L’opérateur partiel $\lambda 1_E-u$ est injectif, son image est dense dans E, mais $\lambda 1_E-u$ n’est pas surjectif ; on dit que $\lambda$ appartient au spectre continu de $u$.

5) Soit $\lambda$ un nombre complexe appartenant à l’ensemble résolvant de $u$. La résolvante $R(u, \lambda )$ est une application linéaire injective de E dans E ; son image est le domaine de $u$ et $u=\lambda 1_E-R(u, \lambda )^{-1}($cf. IV, p. 226). Inversement, cette propriété caractérise l’ensemble résolvant et la résolvante. Précisément, soit $\lambda \in \mathbf{C}$; s’il existe une application linéaire continue injective $w$ de E dans E telle que $u=\lambda 1_E-w^{-1}$, alors $\lambda$ appartient à l’ensemble résolvant de $u$ et $w= R(u, \lambda )$.

En particulier, si $v$ est un opérateur fermé à domaine dense sur E, et si $\lambda \in \mathbf{C}$ est un nombre complexe n’appartenant pas à Sp($u$)$\cup$ Sp($v$), alors l’égalité $R(u, \lambda ) = R(v, \lambda )$ implique que $u=v$.

6) On définit le spectre d’un opérateur partiel fermable $u$ comme le spectre de sa fermeture.

Il existe des opérateurs fermés dont le spectre est vide, ou dont le spectre est égal à $\mathbf{C}$ (exercice 12 de IV, p. 347).

Soient E un espace de Banach complexe et $u$ un opérateur fermé à domaine dense sur E. Si F est un espace de Banach complexe et si $v: E\rightarrow F$ est un isomorphisme, alors on a Sp($v\circ u\circ v^{-1}$) $=$ Sp($u$) et $R(v\circ u\circ v^{-1}, \lambda ) =v\circ R(u, \lambda )\circ v^{-1}$ pour tout $\lambda  /\in$ Sp($u$).

#### Proposition 14 {#ts-iv-s4-prop-14 .statement tag=033R}

Soit E un espace de Banach complexe. Soient $u$ un opérateur fermé à domaine dense sur E et U son ensemble résolvant.

a) Pour tout $\lambda \in U$, le disque ouvert dans $\mathbf{C}$ de centre $\lambda$ et de rayon $\|R(u, \lambda )\|^{-1}$ est contenu dans U ;

b) L’ensemble U est ouvert dans $\mathbf{C}$;

c) Supposons que Sp($u$) n’est pas vide. Soit $\lambda \in U$ et notons $\delta$ la distance dans $\mathbf{C}$ de $\lambda$ au spectre de $u$. On a $\delta  >0$ et $\|R(u, \lambda )\|\geqslant 1/\delta$;

d) L’application $\lambda \mapsto R(u, \lambda )$ est une application holomorphe de U dans $\mathscr{L}(E)$. Pour tout entier $k\in \mathbf{N}$ et tout $\lambda \in U$, on a

$\frac{\partial^k}{\partial \lambda^k}R(u, \lambda ) = (-1)^kk$!R($u, \lambda$ )$^{k+1}$.

Soit $\lambda \in U$. Pour tout $\mu\in \mathbf{C}$ tel que $\|(\mu-\lambda )1_E\|<\|R(u, \lambda )\|^{-1}$, le lemme 4 appliqué à l’opérateur partiel injectif $\lambda 1_E-u$ et à $v= (\mu-\lambda )1_E$ implique que l’opérateur partiel $\mu1_E-u=\lambda 1_E-u+v$ est injectif et a un inverse continu. Cela implique a). D’après loc. cit., on a également la formule

$$
R(u, \mu) = R(u, \lambda )\circ \sum_{k\in\mathbf{N}}(\lambda -\mu)^kR(u, \lambda )^k
$$

ce qui implique que la résolvante de $u$ est holomorphe dans U.

L’assertion b) résulte aussitôt de a). Si Sp($u$) est non vide, la distance de $\lambda$ à Sp($u$) est strictement positive (TG, IX, p. 13, prop. 2), d’où c).

La dernière partie de l’assertion d) est démontrée par récurrence sur $k$, le cas $k= 1$ étant conséquence de la formule (8), p. 245.

#### Proposition 15 {#ts-iv-s4-prop-15 .statement tag=033S}

Soient $u$ un opérateur fermé à domaine dense sur un espace de Banach complexe E et $\lambda$ un nombre complexe appartenant à l’ensemble résolvant de $u$.

a) Le sous-ensemble Sp(R($u, \lambda$ ))$-\{0\}$ de $\mathbf{C}$ est l’image du spectre de $u$ par l’application $\mu\mapsto (\lambda -\mu)^{-1}$ de $\mathbf{C}-\{\lambda \}$ dans $\mathbf{C}^*$;

b) Pour tout $\mu\not =\lambda$ dans $\mathbf{C}$, on a

Ker($\mu1_E-u$) $=$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda ))$.

Démontrons l’assertion a). Pour tout $\mu\not =\lambda$, on calcule

$$
\mu1_E-u= (\lambda -\mu) ((\lambda -\mu)^{-1}1_E-R(u, \lambda )) (\lambda 1_E-u)
$$

Puisque $\lambda  /\in$ Sp($u$) et $\mu\not =\lambda$, l’application linéaire $(\lambda -\mu)(\lambda 1_E-u)$ est une bijection de dom($u$) sur E. Par conséquent, cette formule implique que $\mu1_E-u$ est une bijection de dom($u$) sur E si et seulement si $(\lambda -\mu)^{-1}1_E-R(u, \lambda )$ est une bijection de E sur E, ce qui implique l’assertion.

Démontrons b). Si $\mu\not =\lambda$ et $x\in$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda ))$, on a $x\in$ dom($u$) et la formule $1_E= (\lambda 1_E-u)\circ R(u, \lambda )$ implique que $x\in$ Ker($\mu1_E-u$). Réciproquement, si $x\in$ Ker($\mu1_E-u$) et $\mu\not =\lambda$, la formule $1_{dom(u)}= R(u, \lambda )\circ (\lambda 1_E-u)$ implique $R(u, \lambda )(x) = (\lambda -\mu)^{-1}x$.

#### Proposition 16 {#ts-iv-s4-prop-16 .statement tag=033T}

Soit $u$ un opérateur fermé à domaine dense sur un espace hilbertien complexe E. Le spectre de $u^*$ est l’image du spectre de $u$ par la conjugaison complexe et, pour tout élément $\lambda$ de l’ensemble résolvant de $u$, on a $R(u, \lambda )^*= R(u^*, \lambda )$. En particulier, si $u$ est auto-adjoint, l’endomorphisme $R(u, \lambda )$ est normal pour tout $\lambda  /\in$ Sp($u$).

Soit $\lambda \in \mathbf{C}-$ Sp($u$) un élément de l’ensemble résolvant de $u$. On a $u=\lambda 1_E-R(u, \lambda )^{-1}$, donc

$$
u^*=\overline{\lambda}1_E-(R(u, \lambda )^{-1})^*=\overline{\lambda}1_E-(R(u, \lambda )^*)^{-1}
$$

(IV, p. 236 et prop. 9 de IV, p. 239). D’après la remarque 5, on en déduit que $\overline{\lambda}\in \mathbf{C}-$ Sp($u^*$) et que $R(u, \lambda )^*= R(u^*, \lambda )$. Par conséquent, le spectre de $u^*$ est contenu dans l’image de Sp($u$) par la conjugaison complexe. On obtient l’égalité en appliquant cette propriété à $u^*$, puisque $u^{**}=u$ (cor. de la prop. 8 de IV, p. 237). La dernière assertion résulte alors de la formule (9), p. 245.

#### Corollaire {#ts-iv-s4-n7-cor-1 .statement tag=033U}

Soit $u$ un opérateur partiel auto-adjoint sur un espace hilbertien complexe E. Si E n’est pas nul, alors le spectre de $u$ n’est pas vide.

Supposons que Sp($u$) est vide. Alors $u$ est injectif et $u^{-1}=-R(u,0)$ est un endomorphisme injectif de E tel que Sp($u^{-1}$)$\subset  \{0\}$ (prop. 15, a)), donc Sp($u^{-1}$) $=\{0\}($I, p. 26, cor. 1). Puisque $u^{-1}$ est normal (prop. 16), cela implique que $u^{-1}$ est nul (I, p. 110, exemple 1), ce qui est une contradiction.

#### Lemme 5 {#ts-iv-s4-lem-5 .statement tag=033V}

Soit E un espace hilbertien complexe et soit $u$ un opérateur partiel fermé à domaine dense sur E. Soit $\lambda \in \mathbf{C}$. Supposons qu’il existe un nombre réel $c >0$ tel que

(10) $\|u(x)-\lambda x\|\geqslant c\|x\|$ pour tout $x\in$ dom($u$),

(11) $\|u^*(x)-\lambda x\|\geqslant c\|x\|$ pour tout $x\in$ dom($u^*$).

Alors $\lambda$ appartient à l’ensemble résolvant de $u$ et $\|R(u, \lambda )\|\leqslant c^{-1}$.

L’hypothèse implique que $u-\lambda 1_E$ et $u^*-\overline{\lambda}1_E$ sont injectifs. Soit F l’image de $u-\lambda 1_E$. L’espace F est dense dans E, puisque son orthogonal est égal à Ker($u^*-\overline{\lambda}1_E$) (prop. 7, c) de IV, p. 236), qui est nul.

Démontrons que l’espace F est fermé. Soit $(x_n)_{n\in\mathbf{N}}$ une suite dans dom($u$) telle que la suite $(u(x_n)-\lambda x_n)_{n\in\mathbf{N}}$ converge vers $y\in F$. L’inégalité (10) implique que la suite $(x_n)_{n\in\mathbf{N}}$ est une suite de Cauchy dans E. Soit $x\in E$ sa limite. La suite $(x_n, u(x_n))$ converge vers $(x, y+\lambda x)$ dans $E\times E$; puisque le graphe de $u$ est fermé, on a donc $x\in$ dom($u$) et $u(x) =y+\lambda x$, ce qui démontre que $y\in F$.

On conclut que F = E. Ainsi, l’opérateur partiel $u-\lambda 1_E$ est bijectif, d’où $\lambda  /\in$ Sp($u$) (remarque 3). L’inégalité (10) implique alors que $\|R(u, \lambda )\|\leqslant c^{-1}$.

#### Proposition 17 {#ts-iv-s4-prop-17 .statement tag=033W}

Soit E un espace hilbertien complexe et soit $u$ un opérateur partiel auto-adjoint sur E.

a) Le spectre de $u$ est contenu dans $\mathbf{R}$;

b) Si $u$ est positif, alors le spectre de $u$ est contenu dans $\mathbf{R}_+$;

c) Supposons que E est non nul. Soient $\lambda  /\in$ Sp($u$) et $\delta  >0$ la distance de $\lambda$ au spectre de $u$. On a $\|R(u, \lambda )\|=\delta^{-1}$.

Soient $(a, b)\in \mathbf{R}\times \mathbf{R}$ et $\lambda =a+ib$. Soit $x\in$ dom($u$). Comme $u$ est auto-adjoint, on a $\langle x|u(x)\rangle  \in \mathbf{R}$, d’où

$$
\|u(x)-\lambda x\|^2=\|u(x)\|^2-2a\langle x|u(x)\rangle + (a^2+b^2)\|x\|^2
$$

$$
=\|u(x)-\lambda x\|^2
$$

Supposons que $b\not = 0$. On obtient alors

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2+b^2\|x\|^2
$$

$$
\geqslant b^2\|x\|^2
$$

D’après le lemme 5, on a donc $\lambda  /\in$ Sp($u$), d’où l’assertion a).

Supposons que $u$ est également positif. Si $b= 0$ et $a <0$, on obtient de même pour $x\in$ dom($u$) l’inégalité

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2\geqslant a^2\|x\|^2
$$

donc $\lambda  /\in$ Sp($u$) $($loc. cit.), ce qui démontre b).

Démontrons enfin c). D’après la prop. 16, la résolvante $R(u, \lambda )$ est un endomorphisme normal de E. Sa norme est donc égale à son rayon spectral (cor. 1 de I, p. 108), d’où

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(R(u,\lambda))}|\mu|$

(th. 1 de I, p. 24). Le spectre de $R(u, \lambda )$ ne peut être réduit à $\{0\}$, car dans ce cas on aurait $\|R(u, \lambda )\|= 0$, donc l’image dom($u$) de $R(u, \lambda )$ serait nulle, et E également. La prop. 15 implique donc que

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(u)}\frac{1}{|\lambda-\mu|}=\frac{1}{\delta}$.

#### Corollaire {#ts-iv-s4-n7-cor-2 .statement tag=033X}

Soit $u$ un opérateur auto-adjoint sur E.

a) Le spectre résiduel de $u$ est vide ;

b) Pour tous $\lambda \not =\mu$ dans $\mathbf{C}$, les espaces propres de $u$ relatifs à $\lambda$ et $\mu$ sont orthogonaux.

Démontrons a). Soit $\lambda$ appartenant au spectre de $u$; c’est un nombre réel (prop. 17). On a Ker($\lambda 1_E-u$) $=$ Im($\lambda 1_E-u$)$^{\circ}$ (prop. 7 de IV, p. 236), donc $\lambda$ n’est pas une valeur propre de $u$ si l’opérateur partiel $\lambda 1_E-u$ est d’image dense. Cela implique par définition que le spectre résiduel de $u$ est vide.

Démontrons b). D’après la proposition, on peut supposer que $\lambda$ et $\mu$ sont réels. Soient $x\in$ dom($u$) tel que $u(x) =\lambda x$ et $y\in$ dom($u$) tel que $u(y) =\mu y$. On a alors

$$
\lambda \langle x|y\rangle =\langle u(x)|y\rangle =\langle x|u(y)\rangle =\mu\langle x|y\rangle
$$

d’où $\langle x|y\rangle = 0$.

#### Remarque {#ts-iv-s4-n7-rem-2 .statement tag=033Y}

Si $u$ est un opérateur symétrique fermé non auto-adjoint, son spectre n’est pas contenu dans $\mathbf{R}($cf. cor. 10 de IV, p. 257 ci-dessous), et il est possible que les espaces propres de $u$ relatifs à $\lambda$ et $\overline{\lambda}$ ne soient pas orthogonaux (exercice 11 de IV, p. 347).

### 8. Pseudo-spectre

#### Définition 9 {#ts-iv-s4-def-9 .statement tag=033Z}

Soit E un espace de Banach complexe et soit $u$ un opérateur partiel fermé sur E. Soit $\varepsilon$ un nombre réel strictement positif. On appelle $\varepsilon$-pseudo-spectre de $u$ la réunion du spectre de $u$ et de l’ensemble des nombres complexes $\lambda$ appartenant à l’ensemble résolvant de $u$ tels que $\|R(u, \lambda )\|> \varepsilon^{-1}$. On note PSp$_{\varepsilon}(u)$ cet ensemble.

Certains auteurs définissent le $\varepsilon$-pseudo-spectre de $u$ comme l’ensemble $T_{\varepsilon}(u)$ réunion de Sp($u$) et de l’ensemble des $\lambda \in \mathbf{C}-$ Sp($u$) tels que $\|R(u, \lambda )\|\geqslant \varepsilon^{-1}$. L’adhérence de PSp$_{\varepsilon}(u)$ est contenue dans $T_{\varepsilon}(u)$, mais cette inclusion peut être stricte, même si E est un espace hilbertien (cf. exercices 18 de IV, p. 348 et 19 de IV, p. 349).

#### Proposition 18 {#ts-iv-s4-prop-18 .statement tag=0340}

Soient E un espace de Banach complexe et $u$ un opérateur partiel fermé sur E. Soit $\varepsilon \in \mathbf{R}^*_+$. L’ensemble PSp$_{\varepsilon}(u)$ est un ouvert de $\mathbf{C}$. Il n’est pas vide si E n’est pas nul.

Si E est nul, alors PSp$_{\varepsilon}(u)$ est vide. Supposons que E est non nul. D’après la prop. 14 de IV, p. 246, l’ensemble PSp$_{\varepsilon}(u)$ est un ouvert de $\mathbf{C}$.

L’ensemble PSp$_{\varepsilon}(u)$ n’est pas vide si le spectre de $u$ n’est pas vide. Si Sp($u$) est vide, alors le théorème de Liouville (VAR, R1, p. 29, 3.3.6) implique que la fonction holomorphe sur $\mathbf{C}$ définie par $\lambda \mapsto R(u, \lambda )$ n’est pas bornée, donc il existe $\lambda$ dans $\mathbf{C}$ tel que $\|R(u, \lambda )\|> \varepsilon^{-1}$.

#### Proposition 19 {#ts-iv-s4-prop-19 .statement tag=0341}

Soient E un espace de Banach complexe et $u$ un opérateur partiel fermé sur E. On a PSp$_{\varepsilon}(u)\subset$ PSp$_{\delta}(u)$ si $0< \varepsilon  < \delta$ et

$\bigcap_{\varepsilon\in\mathbf{R}^*_+}$ PSp$_{\varepsilon}(u) =$ Sp($u$).

La première assertion résulte de la définition. Pour la seconde, le spectre de $u$ est contenu dans PSp$_{\varepsilon}(u)$ pour tout $\varepsilon  >0$ par définition, et si $\lambda  /\in$ Sp($u$), alors $\lambda  /\in$ PSp$_{\varepsilon}(u)$ lorsque $\varepsilon  <\|R(u, \lambda )\|^{-1}$.

#### Proposition 20 {#ts-iv-s4-prop-20 .statement tag=0342}

Soient E un espace de Banach complexe et $u$ un opérateur partiel fermé sur E. Soit $\varepsilon \in \mathbf{R}^*_+$. Pour tout $\lambda \in \mathbf{C}$, les conditions suivantes sont équivalentes :

(i) On a $\lambda \in$ PSp$_{\varepsilon}(u)$;

(ii) Soit $\lambda \in$ Sp($u$), soit il existe $x\in$ dom($u$) tel que $\|x\|= 1$ et $\|(\lambda 1_E-u)(x)\|< \varepsilon$;

(iii) Il existe $v\in \mathscr{L}(E)$ tel que $\|v\|< \varepsilon$ et $\lambda \in$ Sp($u+v$).

On peut supposer que E est non nul. La condition (ii) est une reformulation de la définition, et donc de la condition (i).

Supposons que la condition (i) est vérifiée et démontrons (iii). Si $\lambda$ appartient au spectre de $u$, on peut prendre $v= 0$ dans (iii).

Supposons donc que $\lambda  /\in$ Sp($u$). Par définition de PSp$_{\varepsilon}(u)$, il existe $y\in E$ tel que $\|y\|= 1$ et $\|R(u, \lambda )y\|> \varepsilon^{-1}$. Posons $x= R(u, \lambda )y$. On a $x\not = 0$. D’après le théorème de Hahn–Banach (EVT, II, p. 67, cor. 2), la forme linéaire $\ell$ sur $\mathbf{C}x$ telle que $\ell (x) = 1$ admet un prolongement continu $\ell_1\in E'$ tel que $\|\ell_1\|=\|\ell \|$; on a donc $\|\ell_1\|=\|x\|^{-1}< \varepsilon$. Pour tout $e\in E$, posons $v(e) =\ell_1(e)y$. On a $v\in \mathscr{L}(E)$ et $v(x) =y$. Il vient $(u+v)x=u(x) +y=\lambda x$, donc $\lambda \in$ Sp($u+v$). Comme de plus $\|v\|=\|\ell_1\|< \varepsilon$, la condition (iii) est satisfaite.

Réciproquement, soit $v\in \mathscr{L}(E)$ tel que $\|v\|< \varepsilon$ et $\lambda \in$ Sp($u+v$). L’opérateur partiel $\lambda 1_E-(u+v)$ n’est donc pas injectif avec un inverse continu ; d’après le lemme 4 de IV, p. 243, appliqué à l’opérateur partiel injectif $\lambda 1_E-u$ et à $-v$, on a donc $\|v\|\geqslant \|R(u, \lambda )\|^{-1}$. Il en résulte que la condition (iii) implique (i).

#### Corollaire {#ts-iv-s4-n8-cor-1 .statement tag=0343}

Soient E un espace de Banach complexe et $u$ un opérateur partiel fermé sur E. Soit $\varepsilon  >0$.

a) Pour tout $v\in \mathscr{L}(E)$, on a PSp$_{\varepsilon}(u)\subset$ PSp$_{\varepsilon+\|v\|}(u+v)$;

b) Soient $\delta  >0$ et $D_{\delta}$ le disque ouvert de centre 0 et de rayon $\delta$ dans $\mathbf{C}$. On a PSp$_{\varepsilon}(u) + D_{\delta}\subset$ PSp$_{\varepsilon+\delta}(u)$.

Soit $\lambda \in$ PSp$_{\varepsilon}(u)$. Il existe un endomorphisme $w\in \mathscr{L}(E)$ tel que $\|w\|< \varepsilon$ et $\lambda \in$ Sp($u+w$) (prop. 20). Comme $u+w= (u+v)+(w-v)$ et $\|w-v\|< \varepsilon +\|v\|$, on a $\lambda \in$ PSp$_{\varepsilon+\|v\|}(u+v) ($loc. cit.).

Soit $\mu\in D_{\delta}$; on a $\lambda +\mu\in$ Sp($u+ (w+\mu1_E)$) et $\|w+\mu1_E\|< \varepsilon +\delta$, donc $\lambda +\mu\in$ PSp$_{\varepsilon+\delta}(u) ($loc. cit.).

#### Proposition 21 {#ts-iv-s4-prop-21 .statement tag=0344}

Soient E un espace de Banach complexe et $u$ un opérateur partiel fermé sur E. Soit $\varepsilon \in \mathbf{R}^*_+$. Toute composante connexe bornée de PSp$_{\varepsilon}(u)$ rencontre le spectre de $u$.

Soit U une composante connexe de PSp$_{\varepsilon}(u)$ qui ne rencontre pas Sp($u$). L’ensemble U est ouvert et fermé dans PSp$_{\varepsilon}(u)$, et son adhérence U dans $\mathbf{C}$ vérifie donc $U\cap$ PSp$_{\varepsilon}(u) = U$.

Comme Sp($u$) est contenu dans PSp$_{\varepsilon}(u)$ et U ne rencontre pas Sp($u$), cette égalité démontre que l’ensemble U est disjoint de Sp($u$), donc contenu dans l’ensemble résolvant de $u$. De plus, elle implique que l’ensemble $\overline{U}-$ U ne rencontre pas PSp$_{\varepsilon}(u)$.

On a donc $\|R(u, \lambda )\|\leqslant \varepsilon^{-1}$ pour tout $\lambda$ dans $\overline{U}-$ U, tandis que $\|R(u, \lambda )\|> \varepsilon^{-1}$ pour $\lambda \in U$. Si l’ensemble U est borné, son adhérence $\overline{U}$ est compacte et il existe $\lambda_0\in \overline{U}$ tel que $\|R(u, \lambda )\|\leqslant \|R(u, \lambda_0)\|$ pour $\lambda \in U$. Ce qui précède implique que $\lambda_0\in U$, ce qui contredit le principe du maximum (VAR, R1, p. 29, 3.3.7) puisque la résolvante de $u$ est holomorphe dans l’ensemble résolvant de $u$ (prop. 14 de IV, p. 246).

### 9. Opérateurs de multiplication

Soient X un espace localement compact et $\mu$ une mesure positive sur X. On considère les opérateurs de multiplication sur $L^2(X, \mu)$; ce sont des opérateurs fermés à domaine dense (prop. 5 de IV, p. 232). Pour toute fonction $\mu$-mesurable $g$ sur X, on notera $m_g$ l’opérateur partiel de multiplication par $g$ sur $L^2(X, \mu)$.

#### Proposition 22 {#ts-iv-s4-prop-22 .statement tag=0345}

Soit $g$ une fonction $\mu$-mesurable sur X.

a) Le spectre de $m_g$ est l’image $\mu$-essentielle S de $g$;

b) Soit $\lambda \in \mathbf{C}-$ Sp($m_g$). La résolvante $R(m_g, \lambda )$ est l’opérateur de multiplication $m_h$, où $h$ est la fonction sur X définie par $h(x) = 0$ si $g(x) =\lambda$ et $h(x) = (\lambda -g(x))^{-1}$ sinon.

Démontrons que $\mathbf{C}-$ S est contenu dans l’ensemble résolvant de $m_g$. Soit $\lambda \in \mathbf{C}-$ S. Il existe un voisinage ouvert U de $\lambda$ tel que le sous-ensemble $Y =\overset{-1}{g}(U)$ de X est localement $\mu$-négligeable. La fonction $k$ définie sur X par $k(x) = (\lambda -g(x))^{-1}$ si $x /\in Y$ et $k(x) = 0$ si $x\in Y$ appartient alors à $\mathscr{L}^{\infty}(X, \mu)$ (lemme 5 de IV, p. 184) ; l’opérateur de multiplication par $k$ est donc un endomorphisme de $L^2(X, \mu)$.

Comme $|gk|\leqslant 1 +|\lambda k|$, on a

$$
|gkf|\leqslant |f|+|\lambda kf|
$$

pour $f\in \mathscr{L}^2(X, \mu)$, ce qui implique que l’image de $m_k$ est contenue dans le domaine de $m_g$. Réciproquement, soit $f\in \mathscr{L}^2(X, \mu)$ dont la classe $\widetilde{f}$ appartient au domaine de $m_g$. En dehors de l’ensemble localement $\mu$-négligeable Y, on a $f(x) =k(x)(\lambda -g(x))f(x)$, donc $\widetilde{f}$ est dans l’image de $m_k$. La même formule prouve que $\lambda$ appartient à l’ensemble résolvant de $m_g$ et que $R(m_g, \lambda ) =m_k$. Comme l’ensemble Y est localement $\mu$-négligeable, l’opérateur de multiplication $m_k$ coïncide avec l’opérateur $m_h$ décrit dans l’assertion b).

Démontrons réciproquement que $\mathbf{C}-$ Sp($m_g$) est contenu dans $\mathbf{C}-$ S. Soit $\lambda \in \mathbf{C}-$ Sp($m_g$). Soit $M>\|R(m_g, \lambda )\|$ un nombre réel. Notons Y l’ensemble des $x\in X$ tels que $|\lambda -g(x)|<M^{-1}$. Démontrons que Y est localement $\mu$-négligeable, ce qui impliquera que $\lambda$ n’appartient pas à S, et conclura la démonstration.

Soit K un sous-ensemble compact de X. Soit $\varphi$ la fonction caractéristique de $Y\cap K$; c’est un élément de $\mathscr{L}^2(X, \mu)$, dont on note $\widetilde{\varphi}$ la classe dans $L^2(X, \mu)$. Soit $\psi$ une fonction dans $\mathscr{L}^2(X, \mu)$ dont la classe dans $L^2(X, \mu)$ est $R(m_g, \lambda )(\widetilde{\varphi})$. On a $R(m_g, \lambda )(\widetilde{\varphi})\in$ dom($m_g$) et $(\lambda -m_g)(R(m_g, \lambda )(\widetilde{\varphi})) =\widetilde{\varphi}$, donc $(\lambda -g(x))\psi (x) = 1$ pour $\mu$-presque tout $x\in Y\cap K$. Cela implique

$$
\|R(m_g, \lambda )\|^2\|\widetilde{\varphi}\|^2\geqslant \|R(m_g, \lambda )(\widetilde{\varphi})\|^2\geqslant M^2\mu(Y\cap K) = M^2\|\widetilde{\varphi}\|^2
$$

Au vu du choix de M, cela signifie que $\varphi$ est nulle $\mu$-presque partout. Ainsi, l’ensemble $Y\cap K$ est $\mu$-négligeable. L’ensemble Y est donc localement $\mu$-négligeable (INT, IV, p. 172, § 5, n$^o2$, prop. 5).

#### Proposition 23 {#ts-iv-s4-prop-23 .statement tag=0346}

Soit $g$ une fonction $\mu$-mesurable sur X. L’adjoint de l’opérateur de multiplication $m_g$ est $m_{\overline{g}}$.

Pour tout entier $n\geqslant$ 1, soit $\varphi_n$ la fonction caractéristique de l’ensemble des éléments $x\in$ X tels que $|g(x)|\leqslant n$, et soit $\widetilde{\varphi}_n$ sa classe dans $L^2(X, \mu)$. Soient $f\in \mathscr{L}^2(X, \mu)$ dont la classe $\widetilde{f}$ appartient à dom($m^*_g$) et $\psi$ une fonction dont la classe est $m^*_g(\widetilde{f})$.

Pour toute $h\in \mathscr{L}^2(X, \mu)$ dont la classe $\widetilde{h}$ appartient à dom($m_g$), on a également $\widetilde{h}\widetilde{\varphi}_n\in$ dom($m_g$), et donc $\langle \widetilde{f}|m_g(\widetilde{h}\widetilde{\varphi}_n)\rangle =\langle m^*_g(\widetilde{f})|\widetilde{h}\widetilde{\varphi}_n\rangle$. Cela entraîne l’égalité

$$
\int_X\overline{(f g-\psi)}\varphi_nh d\mu= 0
$$

Puisque le domaine de $m_g$ est dense dans $L^2(X, \mu)$, on en déduit que $(f g-\psi )\varphi_n$ est nulle $\mu$-presque partout. Puisque $n$ est arbitraire, cela signifie que $m^*_g(\widetilde{f})$ est la classe dans $L^2(X, \mu)$ de $f g$. En particulier, comme $m^*_g(\widetilde{f})\in L^2(X, \mu)$, on conclut que $f$ appartient au domaine de $m_{\overline{g}}$ et que $m^*_g(\widetilde{f}) =m_{\overline{g}}(\widetilde{f})$.

L’adjoint de $m_g$ est donc une extension de $m_{\overline{g}}$. De plus, on a

$$
\langle f|m_g(h)\rangle =\int_X\overline{f}\cdot (gh)d\mu=\int_Xf\overline{g}h d\mu
$$

pour tout $f\in L^2(X, \mu)$ et $h\in$ dom($m_g$), ce qui démontre que la forme linéaire $h\mapsto  \langle f|m_g(h)\rangle$ est continue lorsque $m_{\overline{g}}(f)g$ appartient à $L^2(X, \mu)$. Par conséquent le domaine de $m_{\overline{g}}$ est contenu dans celui de $m^*_g$, ce qui conclut la preuve.

#### Corollaire {#ts-iv-s4-n9-cor-1 .statement tag=0347}

Soit $g$ une fonction $\mu$-mesurable sur X. L’opérateur de multiplication $m_g$ sur $L^2(X, \mu)$ est auto-adjoint (resp. positif ) si et seulement si la fonction $g$ est localement $\mu$-presque partout à valeurs réelles (resp. localement $\mu$-presque partout positive).

La première assertion résulte de la proposition. Si $g$ est localement $\mu$-presque partout positive, on a $\langle f|m_g(f)\rangle =\int_Xg|f|^2d\mu\geqslant 0$ pour tout $f\in L^2(X, \mu)$, donc l’opérateur partiel $m_g$ est positif.

Réciproquement, si $m_g$ est positif, alors son spectre est contenu dans $\mathbf{R}_+$ (prop. 17 de IV, p. 248) ; comme il s’agit de l’image $\mu$-essentielle de $g$ (prop. 22, a)), cela signifie que $g$ est localement $\mu$-presque partout positive.

#### Lemme 6 {#ts-iv-s4-lem-6 .statement tag=0348}

Soient $g_1$ et $g_2$ des fonctions $\mu$-mesurables sur X.

a) L’opérateur partiel $m_{g_1}+m_{g_2}$ est fermable et sa fermeture est l’opérateur de multiplication $m_{g_1+g_2}$;

b) On a $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$;

c) Supposons que $g_1$ est bornée. On a alors $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$. Par ailleurs, le domaine de $m_{g_2}$ est contenu dans le domaine de $m_{g_1g_2}$, et $m_{g_1}\circ m_{g_2}$ est la réduction de $m_{g_1g_2}$ à dom($m_{g_2}$).

Il est élémentaire que $m_{g_1+g_2}$ est une extension de $m_{g_1}+m_{g_2}$; ce dernier opérateur est donc fermable, et $\overline{m_{g_1} + m_{g_2}}\subset m_{g_1+g_2}$.

Soit $f\in \mathscr{L}^2(X, \mu)$ tel que la fonction $h= (g_1+g_2)f$ appartient à $\mathscr{L}^2(X, \mu)$. Pour tout entier $n\geqslant 1$, notons $X_n$ l’ensemble des $x\in X$ tels que $|g_1(x)|+|g_2(x)|\leqslant n$ et $\varphi_n$ la fonction caractéristique de $X_n$. On a $\varphi_nf\in$ dom($m_{g_1}+m_{g_2}$). Comme $(\varphi_nf)(x)$ converge vers $f(x)$ pour tout $x\in X$ et que pour tout $n\in \mathbf{N}$, on a $|\varphi_nf|\leqslant |f|$ et $|(g_1+g_2)\varphi_nf|\leqslant$ $|(g_1+g_2)f|=|h|$, avec $h\in \mathscr{L}^2(X, \mu)$ par hypothèse, le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6) implique que la suite des couples de classes dans $L^2(X, \mu)\times L^2(X, \mu)$ de $(\varphi_nf,(g_1+g_2)\varphi_nf)$, qui appartiennent au graphe de $m_{g_1}+m_{g_2}$, converge vers le couple des classes de $(f, h)$ dans $L^2(X, \mu)$. La fermeture de $m_{g_1}+m_{g_2}$ est donc bien égale à $m_{g_1+g_2}$.

Il est élémentaire que $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$. Supposons que $g_1$ est bornée, de sorte que $m_{g_1}$ est une application linéaire continue sur $L^2(X, \mu)$. Alors le domaine de $m_{g_2}\circ m_{g_1}$ est l’ensemble des classes de fonctions $f\in \mathscr{L}^2(X, \mu)$ telles que $g_2(g_1f)\in \mathscr{L}^2(X, \mu)$, c’est-à-dire le domaine de $m_{g_1g_2}$. On a donc $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$.

Il est également élémentaire que dom($m_{g_1}\circ m_{g_2}$) $=$ dom($m_{g_2}$) est contenu dans dom($m_{g_1g_2}$), et que la réduction de $m_{g_1g_2}$ à cet espace est égale à $m_{g_1}\circ m_{g_2}$.

On se gardera de croire que $m_{g_1}\circ m_{g_2}=m_{g_1g_2}$ en général (exercice 10 de IV, p. 347). Néanmoins, on a le résultat partiel suivant :

#### Proposition 24 {#ts-iv-s4-prop-24 .statement tag=0349}

Soit $g$ une fonction $\mu$-mesurable sur X.

a) On a $m_{\overline{g}}\circ m_g=m_{|g|^2}$;

b) Pour tous entiers $k, \ell \in \mathbf{N}$, on a $m_{g^k\overline{g}^{\ell}}=m^k_gm^{\ell}_{\overline{g}}$.

On a $m_{\overline{g}}\circ m_g\subset m_{|g|^2}$ par le lemme 6. Inversement, on déduit de l’inégalité $|g|\leqslant 1 +|g|^2$ que dom($m_{|g|^2}$) $=$ dom($m_{\overline{g}}\circ m_g$), d’où la première assertion.

Soient $k, \ell \in \mathbf{N}$. On a $m^k_gm^{\ell}_{\overline{g}}\subset m_{g^k\overline{g}^{\ell}}($loc. cit.). Le domaine de $m^k_gm^{\ell}_{\overline{g}}$ est l’ensemble des classes dans $L^2(X, \mu)$ de fonctions $h\in \mathscr{L}^2(X, \mu)$ telles que $|g|^jh$ appartient à $\mathscr{L}^2(X, \mu)$ pour tout entier $j$ tel que $0\leqslant j\leqslant k+\ell$. Les inégalités

$$
|g^jh|\leqslant |h|+|g^{k+\ell}h|
$$

valides pour $0\leqslant j\leqslant k+\ell$, permettent de constater que dom($m^k_gm^{\ell}_{\overline{g}}$) est égal à dom($m_{g^k\overline{g}^{\ell}}$), d’où l’assertion b).

### 10. Extensions auto-adjointes d’un opérateur symétrique

Dans ce numéro, on se propose de classifier les extensions auto-adjointes des opérateurs symétriques sur un espace hilbertien complexe, et en particulier de trouver des conditions assurant l’existence d’une extension auto-adjointe d’un tel opérateur.

Soit E un espace hilbertien complexe. Pour tout opérateur partiel $u$ sur E, on écrira dans ce numéro $u+i$ et $u-i$ au lieu de $u+i1_E$ et $u-i1_E$.

Soit $u$ un opérateur fermé à domaine dense sur E. On rappelle (cf. définition 4 de IV, p. 230 et proposition 4 de IV, p. 230) que l’on note $E_u$ l’espace hilbertien dom($u$) muni de la forme hermitienne

$$
(x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

On note $\|x\|_u$ la norme d’un élément $x$ de l’espace hilbertien $E_u$. Tout sous-espace de dom($u$) qui est fermé dans E est fermé dans $E_u($IV, p. 230, remarque 1).

#### Définition 10 {#ts-iv-s4-def-10 .statement tag=034A}

Soit $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E. Soient $E_+=$ Ker($u^*-i$) et $E_-=$ Ker($u^*+i$). Le couple $(E_+,E_-)$ de sous-espaces de dom($u^*$) est appelé le couple de carence de $u$. Les sous-espaces $E_+$ et $E_-$ sont des sous-espaces fermés de E (prop. 3 de IV, p. 229). Le couple (dim(E$_+)$, dim(E$_-))$ des dimensions hilbertiennes de ces sous-espaces est appelé l’ indice de carence de $u$.

#### Proposition 25 {#ts-iv-s4-prop-25 .statement tag=034B}

Soit $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E. On a

Ker($u^*-i$)$^{\circ}=$ Im($u+i$),

Ker($u^*+i$)$^{\circ}=$ Im($u-i$).

D’après la prop. 7, c) de IV, p. 236, il suffit de démontrer que l’image de $u+i$ (resp. de $u-i)$ est fermée dans E. Puisque $u$ est symétrique, on a $\langle (u+i)(x)|(u+i)(y)\rangle = (x|y)_u$ pour tous $x$ et $y$ dans dom($u$). L’application $x\mapsto u(x) +ix$ de $E_u$ dans E est donc isométrique. Son image est fermée dans E (lemme 8 de I, p. 107). Puisqu’il s’agit aussi de l’image de $u+i$, celle-ci est fermée dans E. De même, l’image de $u-i$ est fermée dans E.

#### Lemme 7 {#ts-iv-s4-lem-7 .statement tag=034C}

Soient $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E et $v$ une extension symétrique fermée de $u$. Le domaine de $u$ est un sous-espace fermé de l’espace hilbertien $E_v$.

Comme $v$ est une extension de $u$, on a $(x|y)_v= (x|y)_u$ pour $x$ et $y$ dans dom($u$). L’injection canonique de $E_u$ dans $E_v$ est donc isométrique, et la conclusion en résulte (lemme 8 de I, p. 107).

#### Proposition 26 {#ts-iv-s4-prop-26 .statement tag=034D}

Soit $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E. Soit $(E_+,E_-)$ le couple de carence de $u$. Les espaces $E_+,E_-$ et dom($u$) sont des sous-espaces fermés et mutuellement orthogonaux de $E_{u^*}$ dont la somme hilbertienne est égale à $E_{u^*}$.

Puisque $u$ est symétrique, on a $u\subset u^*$, donc l’espace dom($u$) est fermé dans $E_{u^*}$ (lemme 7). Les sous-espaces $E_+$ et $E_-$ sont fermés dans E et contenus dans dom($u^*$), donc fermés dans $E_{u^*}$.

Soit $x\in E_+$. On a $u^*(x) =ix$, d’où $\langle x|u(y)\rangle =-i\langle x|y\rangle$ pour tout $y\in$ dom($u$). Par conséquent, pour tout $y\in$ dom($u$), on a

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =i(\langle x|u(y)\rangle  - \langle x|u^*(y)\rangle )= 0
$$

puisque $u$ est symétrique. Les espaces $E_+$ et dom($u$) sont donc orthogonaux dans $E_{u^*}$. De même, $E_-$ et dom($u$) sont orthogonaux dans $E_{u^*}$.

Soient $x\in E_+$ et $y\in E_-$. Alors

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle  - \langle x|y\rangle = 0
$$

donc $E_+$ et $E_-$ sont orthogonaux dans $E_{u^*}$.

Soit $x\in E_{u^*}$ orthogonal au sous-espace fermé dom($u$)$\oplus E_+\oplus E_-$. Pour tout $y\in$ dom($u$), on a $u^*(y) =u(y)$ puisque $u\subset u^*$, d’où

$$
0 = (x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle +\langle u^*(x)|u(y)\rangle
$$

Cela implique que $z=u^*(x)$ appartient au domaine de $u^*$ et vérifie $u^*(z) =-x$. Soit $x_-=z-ix$. C’est un élément de dom($u^*$) qui vérifie $u^*(x_-) =-x-iz=-ix_-$. Donc $x_-$ appartient à $E_-$. Mais, pour tout $w\in E_-$, on a

$$
-i\langle x_-|w\rangle =-i\langle z|w\rangle +\langle x|w\rangle
$$

$$
=\langle u^*(x)|u^*(w)\rangle +\langle x|w\rangle = (x|w)_{u^*}= 0
$$

Prenant $w=x_-$, on en déduit que $x_-= 0$, c’est-à-dire $z=ix$; comme $z=u^*(x)$, on a donc $x\in E_+$, d’où $x$ = 0 puisque $x$ est orthogonal à $E_+$ dans $E_{u^*}$. Ceci achève de démontrer que la somme directe dom($u$)$\oplus E_+\oplus E_-$ est égale à $E_{u^*}$.

#### Corollaire {#ts-iv-s4-n10-cor-1 .statement tag=034E}

Soit $u$ un opérateur symétrique fermé sur E. Alors $u$ est auto-adjoint si et seulement si l’indice de carence de $u$ est égal à $(0,0)$.

En effet, l’opérateur symétrique $u$ est auto-adjoint si et seulement si dom($u^*$) $=$ dom($u$); or la proposition démontre que dom($u^*$) est la somme hilbertienne de dom($u$) et des sous-espaces de carence de $u$.

Soit $u$ un opérateur partiel symétrique fermé. Le spectre de $u$ est contenu dans $\mathbf{R}$ si et seulement si $u$ est auto-adjoint. En effet, on sait que Sp($u$)$\subset \mathbf{R}$ si $u$ est auto-adjoint (prop. 17 de IV, p. 248) ; si $u$ n’est pas auto-adjoint, l’un des sous-espaces Ker($u^*+i$) ou Ker($u^*-i$) est non nul, donc l’image de $u+i$ ou de $u-i$ est un sous-espace propre de E (prop. 25 de IV, p. 256), de sorte que $i$ ou $-i$ appartient à Sp($u$).

#### Définition 11 {#ts-iv-s4-def-11 .statement tag=034F}

Soit $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E. Une condition au bord pour $u$ est une application linéaire partiellement isométrique (EVT, V, p. 41, déf. 3) de Ker($u^*-i$) dans Ker($u^*+i$).

Soient $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E et $b$ une condition au bord pour $u$. Soit I = Ker($b$)$^{\circ}$ le sous-espace initial de $b$. On note $u_b$ la réduction de $u^*$ au sous-espace de dom($u^*$) somme directe de dom($u$) et du graphe dans $E_+\oplus E_-$ de la restriction de $b$ à I. Comme $E_{u^*}=$ dom($u$)$\oplus E_+\oplus E_-$ (prop. 26), l’opérateur partiel $u_b$ est bien défini.

Autrement dit, le domaine de $u_b$ est l’espace des éléments $x\in E$ de la forme $x=x_0+y+b(y)$, où $x_0\in$ dom($u$) et $y$ appartient au sous-espace initial de $b$. On a alors $u_b(x_0+y+b(y)) =u(x_0) +iy-ib(y)$.

#### Théorème 1 (von Neumann) {#ts-iv-s4-thm-1 .statement tag=034G}

Soient $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E et $(E_+,E_-)$ son couple de carence.

a) Pour toute condition au bord $b$ pour $u$, l’opérateur partiel $u_b$ est une extension symétrique fermée de $u$;

b) L’application $b\mapsto u_b$ est une bijection de l’ensemble des conditions au bord pour $u$ sur l’ensemble des extensions symétriques fermées de $u$;

c) Pour toute condition au bord $b$ pour $u$, on a

Im($u_b+i$) $=$ Im($u+i$)$\oplus$ Im($b$)

Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Ker($b$)$^{\circ}$;

d) Pour toute condition au bord $b$ pour $u$, le couple de carence de $u_b$ est (Ker($b$), Ker($b^*$)).

Soit $b$ une condition au bord pour $u$ et $I\subset E_+$ son sous-espace initial. La restriction de $u^*$ à $\Gamma_{b|I}\subset E_+\oplus E_-$ est l’application linéaire continue définie par $x+b(x)\mapsto ix-ib(x)$ pour $x\in I$. Le graphe de $u_b$ est la somme directe du graphe de $u$ et du graphe de cette application linéaire ; il est donc fermé. L’opérateur fermé $u_b$ est une extension de $u$ telle que $u_b\subset u^*$.

Soient $\gamma_1$ et $\eta_1$ des éléments de I. Considérons les éléments

$$
\gamma =\gamma_1+b(\gamma_1),\eta =\eta_1+b(\eta_1)
$$

du graphe $\Gamma_{b|I}$. On calcule

$$
\langle \gamma |u^*(\eta )\rangle =i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )+i(\langle \gamma_1|\eta_1\rangle  - \langle b(\gamma_1)|b(\eta_1)\rangle )
$$

$$
=i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )
$$

puisque $b$ est isométrique sur I. On en déduit qu’on a

$$
\langle u^*(\gamma )|\eta \rangle =\langle \gamma |u^*(\eta )\rangle \tag{12}
$$

pour tous $\gamma$ et $\eta$ dans $\Gamma_{b|I}$.

Soient $x$ et $y$ des éléments de dom($u$)$,\gamma$ et $\eta$ des éléments de $\Gamma_{b|I}$. Il vient

$$
\langle x+\gamma |u_b(y+\eta )\rangle =\langle x|u(y)\rangle +\langle x|u^*(\eta )\rangle +\langle \gamma |u(y)\rangle +\langle \gamma |u^*(\eta )\rangle
$$

$$
=\langle u(x)|y\rangle +\langle u(x)|\eta \rangle +\langle u^*(\gamma )|y\rangle +\langle u^*(\gamma )|\eta \rangle
$$

$$
=\langle u_b(x+\gamma )|y+\eta \rangle
$$

où on a utilisé le fait que $u$ est symétrique et que $\gamma$ et $\eta$ appartiennent au domaine de $u^*$ ainsi que la formule (12). L’opérateur $u_b$ est donc une extension symétrique fermée de $u$. L’assertion a) est démontrée.

L’application $b\mapsto u_b$ est injective. En effet, une application partiellement isométrique de $E_+$ dans $E_-$ est déterminée de manière unique par son sous-espace initial et par sa restriction à celui-ci. Or le domaine de $u_b$ détermine le sous-espace initial I de $b$ et le graphe de la restriction de $b$ à I.

Démontrons que l’application $b\mapsto u_b$ est surjective. Soit $w$ une extension symétrique fermée de $u$. On a $w\subset w^*\subset u^*$. Le domaine de $w$ est donc un sous-espace de dom($u^*$) contenant dom($u$), et $w$ est la réduction de $u^*$ à ce sous-espace. Soit G l’intersection du domaine de $w$ et de $E_+\oplus E_-$. C’est un sous-espace fermé de $E_{u^*}$ (lemme 7) et on a dom($w$) $=$ dom($u$)$\oplus G$ d’après la proposition 26.

Soient $x\in E_+$ et $y\in E_-$ tels que $x+y\in G$. Puisque $w$ est symétrique, et que c’est la réduction de $u^*$ à dom($w$), on a

$$
\langle x+y|u^*(x+y)\rangle =\langle u^*(x+y)|x+y\rangle
$$

Cette égalité équivaut à

$$
\langle x|ix\rangle +\langle x| -iy\rangle +\langle y|ix\rangle +\langle y| -iy\rangle
$$

$$
=\langle ix|x\rangle +\langle ix|y\rangle +\langle -iy|x\rangle +\langle -iy|y\rangle
$$

c’est-à-dire à $\|x\|^2=\|y\|^2$. En particulier, la projection canonique $p_+: G\rightarrow E_+$ est injective et si I désigne son image, l’espace G est le graphe d’une application isométrique $b_0$ de I dans $E_-$. Pour $x$ dans I et $y$ dans $E_-$ tels que $x+y\in G$, on a

$$
\|x+y\|^2_{u^*}=\|x\|^2_{u^*}+\|y\|^2_{u^*}= 2(\|x\|^2+\|y\|^2)
$$

$$
= 4\|x\|^2= 4\|p_+(x+y)\|^2
$$

Ainsi, considérant G comme sous-espace fermé de l’espace hilbertien $E_{u^*}$, l’application $x\mapsto \frac{1}{2}p_+(x)$ de G dans I une isométrie. En particulier, I est fermé dans $E_+$ (lemme 8 de I, p. 107). Il existe alors une unique condition au bord $b$ pour $u$ dont I est l’espace initial et qui coïncide avec $b_0$ sur I. On a dom($w$) $=$ dom($u_b$), d’où $w=u_b$. Cela établit l’assertion b).

Démontrons les assertions c) et d). Soient $b$ une condition au bord pour $u$ et I son sous-espace initial. Pour $x_0\in$ dom($u$) et $y\in I$, on a

$$
u_b(x_0+y+b(y))-i(x_0+y+b(y)) = (u-i)(x_0)-2ib(y)
$$

On a Im($u-i$) $= E^{\circ}_-$ (prop. 25). Comme l’image de $b$ est contenue dans $E_-$, cette formule démontre que Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Im($b$). D’après loc. cit., on a donc Ker($u^*_b+i$) $= E_-\cap$ Im($b$)$^{\circ}=$ Ker($b^*$).

De manière analogue, on vérifie que Im($u_b+i$) $=$ Im($u+i$)$\oplus I$ et donc (loc. cit.) que Ker($u^*_b-i$) $= I^{\circ}\cap E_+=$ Ker($b$).

#### Corollaire 1 {#ts-iv-s4-thm-1-cor-1 .statement tag=034H}

Soit $u$ un opérateur symétrique fermé sur un espace hilbertien complexe E. L’application $b\mapsto u_b$ induit une bijection de l’ensemble des isométries de Ker($u^*-i$) sur Ker($u^*+i$) sur l’ensemble des extensions auto-adjointes de $u$. En particulier, il existe une extension auto-adjointe de $u$ si et seulement si les deux composantes de l’indice de carence de $u$ sont égales.

Cela découle du corollaire de la proposition 26 et du théorème, ainsi que de EVT, V, p. 25, cor. 2.

#### Corollaire 2 {#ts-iv-s4-thm-1-cor-2 .statement tag=034I}

Soit E un espace hilbertien réel. Soit $u$ un opérateur symétrique fermé sur E. L’opérateur partiel $u_{(\mathbf{C})}$ sur $E_{(\mathbf{C})}$ est symétrique et fermé, et admet au moins une extension auto-adjointe.

L’opérateur partiel $u_{(\mathbf{C})}$ est fermé et symétrique d’après la prop. 2 de IV, p. 228 et le lemme 3 de IV, p. 239. L’isomorphisme $\mathbf{R}$-linéaire $j$ de $E_{(\mathbf{C})}$ dans $E_{(\mathbf{C})}$ tel que $j(z\otimes x) =\overline{z}\otimes x$ pour tout $z\in \mathbf{C}$ et tout $x\in E$ induit un isomorphisme d’espaces hilbertiens de Ker($u^*_{(\mathbf{C})}-i$) dans Ker($u^*_{(\mathbf{C})}+i$) et on peut appliquer le corollaire 1.

#### Corollaire 3 {#ts-iv-s4-thm-1-cor-3 .statement tag=034J}

Soit $u$ un opérateur symétrique sur E. Les conditions suivantes sont équivalentes :

(i) L’opérateur $u$ est essentiellement auto-adjoint ;

(ii) Les espaces Ker($u^*+i$) et Ker($u^*-i$) sont nuls ;

(iii) Les espaces Im($u+i$) et Im($u-i$) sont denses dans E ;

(iv) L’opérateur symétrique partiel $u$ a une unique extension auto-adjointe.

Les conditions (ii) et (iii) sont équivalentes d’après la prop. 7, c) de IV, p. 236.

L’opérateur partiel $u$ est essentiellement auto-adjoint si et seulement si $\overline{u}$ est auto-adjoint, c’est-à-dire si Ker($\overline{u}^*-i$) $=$ Ker($\overline{u}^*+i$) $=\{0\}$ (cor. de la prop. 26). Comme $\overline{u}^*=u^*$ (prop. 8 de IV, p. 237), la condition (i) est donc équivalente à la condition (ii). De plus, le corollaire précédent démontre que (ii) implique que $u$ a une unique extension auto-adjointe, ce qui est la condition (iv).

Enfin, supposons que $u$ a une unique extension auto-adjointe $v$. Il en est alors de même de $\overline{u}$, puisque toute extension auto-adjointe de $\overline{u}$ en est une de $u$, donc est égale à $v$. D’après le corollaire précédent, les espaces Ker($\overline{u}^*+i$) et Ker($\overline{u}^*-i$) doivent être nuls, d’où la condition (ii) en utilisant encore $\overline{u}^*=u^*$.

#### Exemple {#ts-iv-s4-n10-exa-1 .statement tag=034K}

Soient U un ouvert de $\mathbf{R}^n$ muni de la mesure de Lebesgue $\mu$. Soit Δ l’opérateur différentiel scalaire

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

sur U. Notons $u$ l’opérateur partiel sur l’espace hilbertien réel $L^2_{\mathbf{R}}(U, \mu)$ de domaine $\mathscr{D}_{\mathbf{R}}(U) ($IV, p. 201, remarque) défini par $\varphi \mapsto  -\sum^n_{i=1}\partial_i^2\varphi$. On a $u_{(\mathbf{C})}= \Delta_-$, qui est un opérateur partiel fermable (prop. 13 de IV, p. 242) et symétrique (puisque Δ est formellement symétrique), donc $u$ est fermable et symétrique (proposition 2 de IV, p. 228 et lemme 3 de IV, p. 239). D’après le corollaire ci-dessus, il existe donc une extension auto-adjointe de $u_{(\mathbf{C})}$. C’est un laplacien sur U (IV, p. 243).

## EXERCICES {#ts-iv-s4-exercises}

Sauf mention du contraire, les espaces de Banach et les espaces hilbertiens ci-dessous sont supposés complexes.

See the [exercises for § 4](exercises/s4/).

[^1]: On prendra garde de ne pas confondre la notion de graphe considérée ici avec celle introduite dans TA, II, p. 155, déf. 1.
