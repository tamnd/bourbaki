---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 1
section_title: Applications linéaires compactes
lang: fr
source: ts-iii-v-fr
book_pages: A III.2-A III.23, A III.103-A III.118
pdf_pages: 0016-0037, 0117-0132
extraction: native
subsections:
    - "no": 1
      title: Applications linéaires compactes
      page: 2
      pdf_page: 16
    - "no": 2
      title: Applications linéaires compactes et topologies faibles
      page: 6
      pdf_page: 20
    - "no": 3
      title: Transposition
      page: 8
      pdf_page: 22
    - "no": 4
      title: Le théorème de Leray–Schauder
      page: 10
      pdf_page: 24
    - "no": 5
      title: Sous-espaces invariants par un opérateur compact
      page: 12
      pdf_page: 26
    - "no": 6
      title: Espaces d’approximation
      page: 14
      pdf_page: 28
    - "no": 7
      title: Exemples d’espaces d’approximation
      page: 20
      pdf_page: 34
statements: 57
exercises: 37
content_sha256: 0bc9c89363bf7319df76daba8b9287747eb369c589204771fe6260d15b426793
---

## § 1. APPLICATIONS LINÉAIRES COMPACTES

### 1. Applications linéaires compactes

#### Définition 1 {#ts-iii-s1-def-1 .statement tag=02NY}

Soient E un espace vectoriel topologique et F un espace vectoriel topologique séparé. On dit qu’une application linéaire $u$ de E dans F est compacte s’il existe un voisinage V de 0 dans E tel que $u(V)$ soit une partie relativement compacte de F.

On note $\mathscr{L}^c(E; F)$ l’ensemble des applications linéaires compactes de E dans F ; on note aussi $\mathscr{L}^c(F)$ l’ensemble $\mathscr{L}^c(F; F)$.

#### Remarque 1 {#ts-iii-s1-n1-rem-1 .statement tag=02NZ}

Un voisinage de 0 dans E absorbe toute partie bornée de E ; l’image d’une partie bornée de E par une application linéaire compacte de E dans F est donc une partie relativement compacte de F.

#### Remarque 2 {#ts-iii-s1-n1-rem-2 .statement tag=02O0}

Soit E un espace semi-normé et soit B la boule unité de E. Pour qu’une application linéaire $u$ de E dans un espace vectoriel topologique séparé F soit compacte, il faut et il suffit que $u(B)$ soit une partie relativement compacte de F.

#### Remarque 3 {#ts-iii-s1-n1-rem-3 .statement tag=02O1}

Soit F un espace vectoriel topologique séparé. Pour qu’un sous-espace vectoriel E de F soit de dimension finie, il faut et il suffit que l’injection canonique de E dans F soit compacte (EVT, I, p. 15, th. 3).

#### Remarque 4 {#ts-iii-s1-n1-rem-4 .statement tag=02O2}

Pour tout espace vectoriel topologique E sur le corps $\mathbf{R}$, on note $E_{(\mathbf{C})}$ l’espace vectoriel topologique complexifié de E (EVT, II, p. 65). On identifie E à un sous-espace vectoriel topologique réel de $E_{(\mathbf{C})}$ par l’application $x\mapsto 1\otimes x$; l’espace vectoriel topologique réel sous-jacent à $E_{(\mathbf{C})}$ est alors somme directe topologique de E et $iE$.

Soit $u$ une application linéaire de E dans un espace vectoriel topologique séparé F sur $\mathbf{R}$. Notons $u_{(\mathbf{C})}$ l’application $\mathbf{C}$-linéaire de $E_{(\mathbf{C})}$ dans $F_{(\mathbf{C})}$ qui prolonge $u$. Les ensembles de la forme $V +iV$, où V est un voisinage de 0 dans E, forment un système fondamental de voisinages de 0 dans $E_{(\mathbf{C})}$. Pour que l’ensemble $u_{(\mathbf{C})}(V +iV) =u(V) +iu(V)$ soit relativement compact dans $F_{(\mathbf{C})}$, il faut et il suffit que $u(V)$ soit relativement compact dans F. Par suite, pour que l’application $\mathbf{C}$-linéaire $u_{(\mathbf{C})}$ soit compacte, il faut et il suffit que l’application $\mathbf{R}$-linéaire $u$ le soit.

Dans le même ordre d’idées, lorsque $v$ est une application $\mathbf{C}$-linéaire continue de $E_{(\mathbf{C})}$ dans un $\mathbf{C}$-espace vectoriel topologique G, pour que $v$ soit compacte il faut et il suffit que sa restriction à E soit compacte.

#### Remarque 5 {#ts-iii-s1-n1-rem-5 .statement tag=02O3}

Soient E un espace vectoriel topologique, F un espace vectoriel topologique séparé. Soit $F_1$ un sous-espace vectoriel fermé de F et soit $j$ l’injection canonique de $F_1$ dans F. Pour qu’une application linéaire $u$ de E dans $F_1$ soit compacte, il faut et il suffit que l’application linéaire $j\circ u$ de E dans F le soit.

#### Remarque 6 {#ts-iii-s1-n1-rem-6 .statement tag=02O4}

Soit $(G_i)_{i\in I}$ une famille d’espaces vectoriels topologiques séparés, et pour tout $i\in I$, soit $u_i$ une application linéaire compacte d’un espace vectoriel topologique E dans $G_i$. Si l’ensemble I est fini, ou si E est un espace semi-normé, l’application linéaire $x\mapsto (u_i(x))_{i\in I}$ de E dans $\prod_{i\in I}G_i$ est compacte (remarque 2 et TG, I, p. 63, th. 3).

#### Proposition 1 {#ts-iii-s1-prop-1 .statement tag=02O5}

Soient E un espace vectoriel topologique et F un espace vectoriel topologique séparé.

a) Toute application linéaire compacte de E dans F est continue ;

b) Toute application linéaire continue de rang fini de E dans F est compacte;

c) L’ensemble $\mathscr{L}^c(E; F)$ des applications linéaires compactes de E dans F est un sous-espace vectoriel de $\mathscr{L}(E; F)$.

Démontrons a). Soient $v: E\rightarrow F$ une application linéaire compacte et U un voisinage de 0 dans F. Choisissons un voisinage V de 0 dans E tel que $v(V)$ soit relativement compact dans F. Alors $v(V)$ est borné et il existe donc un nombre réel $\lambda  >0$ tel que l’ensemble $v(\lambda V)$ soit contenu dans U ; par suite, $v$ est continue.

Soit $u: E\rightarrow F$ une application linéaire continue de rang fini. Comme l’image $u(E)$ de $u$ est séparée et de dimension finie, il existe un voisinage compact A de 0 dans $u(E)$. L’ensemble $V =\overset{-1}{u}(A)$ est un voisinage de 0 dans E et l’on a $u(V)\subset A$, donc l’application linéaire $u$ est compacte. Cela prouve l’assertion b).

Soient $u_1$ et $u_2$ des applications linéaires compactes de E dans F. Soient $V_1$ et $V_2$ des voisinages de 0 dans E tels que les ensembles $u_1(V_1)$ et $u_2(V_2)$ soient relativement compacts dans F. Posons $V = V_1\cap V_2$ et $u=u_1+u_2$. Alors $u(V)$ est contenu dans $u_1(V_1) +u_2(V_2)$, donc est relativement compact dans F, et l’application linéaire $u$ est compacte. Il est immédiat que $\mathscr{L}^c(E; F)$ est stable par homothétie. Cela prouve que $\mathscr{L}^c(E; F)$ est un sous-espace vectoriel de $\mathscr{L}(E; F)$, d’où l’assertion c).

#### Proposition 2 {#ts-iii-s1-prop-2 .statement tag=02O6}

Soient E un espace semi-normé et F un espace vectoriel topologique séparé. On suppose que toute partie fermée bornée de F est complète. Alors le sous-espace vectoriel $\mathscr{L}^c(E; F)$ de $\mathscr{L}(E; F)$ est fermé pour la topologie de la convergence bornée.

Soit $u$ un élément de $\mathscr{L}(E; F)$ adhérent à $\mathscr{L}^c(E; F)$ pour la topologie de la convergence bornée. Notons B la boule unité de E et V un voisinage de 0 dans F. Choisissons un voisinage W de 0 dans F tel que $W + W\subset V$. Il existe par hypothèse un élément $v$ de $\mathscr{L}^c(E; F)$ tel que $(u-v)(B)\subset W$. L’ensemble $v(B)$ étant relativement compact dans F, il existe une partie finie M de F telle que $v(B)\subset M + W$, d’où $u(B)\subset M + V$. Comme ceci vaut pour tout V, l’ensemble $u(B)$ est précompact dans F, donc son adhérence l’est également (TG, II, prop. 1, p. 30). Puisque celle-ci est fermée et bornée, elle est complète par l’hypothèse faite sur F, et par conséquent est compacte (TG, II, cor., p. 30). Il en résulte que $u(B)$ est relativement compact. Cela prouve que $u$ appartient à $\mathscr{L}^c(E; F)$.

Si F est localement convexe, l’hypothèse de la proposition signifie que F est quasi-complet (EVT, III, p. 8, déf. 6).

#### Corollaire {#ts-iii-s1-n1-cor-1 .statement tag=02O7}

Soient E et F des espaces de Banach. L’ensemble $\mathscr{L}^c(E; F)$ est un sous-espace vectoriel fermé de l’espace de Banach $\mathscr{L}(E; F)$. Il contient l’adhérence de l’espace $\mathscr{L}^f(E; F)$ des applications linéaires continues de rang fini de E dans F.

Cela résulte des propositions 1 et 2.

Il existe des espaces de Banach E et F tels que $\mathscr{L}^f(E; F)$ ne soit pas dense dans $\mathscr{L}^c(E; F) ($cf. remarque 6 de III, p. 16 et théorème 4 de III, p. 19, b)).

#### Proposition 3 {#ts-iii-s1-prop-3 .statement tag=02O8}

Soient $E_1$, E, F, $F_1$ des espaces vectoriels topologiques, F et $F_1$ étant supposés séparés. Soient $v: E_1\rightarrow E,u: E\rightarrow F$ et $w: F\rightarrow F_1$ des applications linéaires. Si $v$ et $w$ sont continues et $u$ compacte, alors $w\circ u\circ v$ est compacte.

Par hypothèse, il existe un voisinage V de 0 dans E tel que $u(V)$ soit relativement compact dans F. Posons $U =\overset{-1}{v}(V)$. Alors U est un voisinage de 0 dans $E_1$ et son image par $w\circ u\circ v$ est contenu dans $w(u$(V)), donc est relativement compact dans $F_1$. Par suite, l’application linéaire $w\circ u\circ v$ est compacte.

Soit E un espace vectoriel topologique séparé ; d’après les prop. 1 et 3$,\mathscr{L}^c(E)$ est un idéal bilatère de l’algèbre $\mathscr{L}(E)$. Lorsque E est un espace de Banach, $\mathscr{L}(E)$ est une algèbre de Banach et $\mathscr{L}^c(E)$ est un idéal bilatère fermé de $\mathscr{L}(E)$ (cor. de la prop. 2). C’est un idéal propre si E est de dimension infinie (cf. remarque 3, p. 2).

#### Corollaire {#ts-iii-s1-n1-cor-2 .statement tag=02O9}

Soit E un espace hilbertien. L’espace $\mathscr{L}^c(E)$ est un idéal bilatère auto-adjoint fermé de $\mathscr{L}(E)$. En particulier, c’est une algèbre stellaire.

En effet, l’espace $\mathscr{L}^c(E)$ est un idéal bilatère fermé, donc auto-adjoint, de $\mathscr{L}(E)$ (lemme 15 de I, p. 122).

#### Proposition 4 {#ts-iii-s1-prop-4 .statement tag=02OA}

Soient E un espace vectoriel topologique, $\widehat{E}$ son séparé complété et $j$ l’application canonique de E dans $\widehat{E}$. Soit $u$ une application linéaire compacte de E dans un espace vectoriel topologique séparé F. Il existe une unique application linéaire compacte $v$ de $\widehat{E}$ dans F telle que $u=v\circ j$.

Identifions F à un sous-espace vectoriel topologique de $\widehat{F}$ et notons $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ l’unique application linéaire continue telle que $\widehat{u}\circ j$ coïncide avec $u$ dans E. Comme $u$ est compacte, il existe un voisinage V de 0 dans E et une partie compacte A de F tels que $u(V)\subset A$. On a $\widehat{u}(j(V))\subset A$, d’où $\widehat{u}(j(V))\subset A$. Or $j(V)$ est un voisinage de 0 dans $\widehat{E}$ (TG, III, p. 24, prop. 7). Par suite, l’image de $\widehat{u}$ est contenue dans F et l’application linéaire continue $v:\widehat{E}\rightarrow F$ déduite de $\widehat{u}$ par passage au sous-espace est compacte. Comme $j(E)$ est dense dans $\widehat{E}$, l’application $v$ est l’unique application linéaire continue de $\widehat{E}$ dans F telle que $u=v\circ j$.

#### Proposition 5 {#ts-iii-s1-prop-5 .statement tag=02OB}

Soient E un espace localement convexe, F un espace vectoriel topologique séparé et $u$ une application linéaire compacte de E dans F. Il existe un espace de Banach G, une application linéaire continue $v$ de E dans G et une application linéaire compacte $w$ de G dans F tels que $u=w\circ v$.

Soit V un voisinage de 0 dans E tel que $u(V)$ soit relativement compact dans F. Soit $p$ une semi-norme continue sur E telle que V contienne la boule unité de $p$ (EVT, II, p. 26, cor.). Notons $E_p$ l’espace semi-normé obtenu en munissant E de la semi-norme $p$. L’application $u$ est une application linéaire compacte de $E_p$ dans F. Le séparé complété G de $E_p$ est un espace de Banach. Notons $v$ l’application linéaire canonique de $E_p$ dans G. D’après la prop. 4, il existe une application linéaire compacte $w: G\rightarrow F$ telle que $u=w\circ v$. D’autre part, $v$ est une application continue de E dans G car la topologie de E est plus fine que celle de $E_p$.

### 2. Applications linéaires compactes et topologies faibles

Soient E un espace localement convexe, $E'$ son dual. Rappelons que la topologie $\sigma (E,E')$ sur E s’appelle la topologie affaiblie sur E (EVT, IV, p. 4). Dans ce numéro, $E_{\sigma}$ désigne l’espace E muni de la topologie affaiblie.

#### Proposition 6 {#ts-iii-s1-prop-6 .statement tag=02OC}

Soient E un espace localement convexe, F un espace localement convexe séparé, $u: E\rightarrow F$ une application linéaire compacte et B une partie bornée de E. La restriction de $u$ à B est une application continue de l’ensemble B, muni de la topologie induite par $\sigma (E,E')$, dans l’espace F.

L’application $u$ est une application linéaire continue de E dans F, et aussi de $E_{\sigma}$ dans $F_{\sigma}$. Sa restriction à B est donc une application continue de l’ensemble B, muni de la topologie induite par $\sigma (E,E')$, dans l’espace $F_{\sigma}$. Or l’ensemble $u(B)$ est contenu dans une partie compacte C de F (remarque 1 de III, p. 2) et l’espace $F_{\sigma}$ est séparé, de sorte que les topologies induites sur C par celles de F et de $F_{\sigma}$ coïncident. La proposition en résulte.

#### Corollaire {#ts-iii-s1-n2-cor-1 .statement tag=02OD}

Soit $(x_n)_{n\in\mathbf{N}}$ une suite de points de E, qui converge vers un point $x$ de E pour la topologie affaiblie. La suite $(u(x_n))_{n\in\mathbf{N}}$ converge dans F vers $u(x)$.

En effet, l’ensemble constitué du point $x$ et des points de la suite $(x_n)_{n\in\mathbf{N}}$ est une partie bornée de E (EVT, III, p. 3, cor. de la prop. 2).

#### Proposition 7 {#ts-iii-s1-prop-7 .statement tag=02OE}

Soient E un espace semi-normé, $E'$ son dual, B la boule unité de $E'$ et $u$ une application linéaire de $E'$ dans un espace localement convexe séparé F. Si la restriction de $u$ à B muni de la topologie induite par $\sigma (E',E)$ est continue, alors $u(B)$ est une partie compacte de F et $u$ est une application linéaire compacte du dual fort $E'_b$ de E dans F.

En effet l’ensemble B, muni de la topologie induite par $\sigma (E',E)$, est compact (EVT, III, p. 17, cor. 2).

#### Corollaire 1 {#ts-iii-s1-prop-7-cor-1 .statement tag=02OF}

Soit E un espace semi-normé de type dénombrable, soit $E'$ son dual et soit B la boule unité de $E'$. Soit $u$ une application linéaire de $E'$ dans un espace localement convexe séparé F. On suppose que pour toute suite $(x_n)_{n\in\mathbf{N}}$ d’éléments de B qui converge pour $\sigma (E',E)$ vers 0, la suite $(u(x_n))_{n\in\mathbf{N}}$ converge vers 0 dans F. Alors, $u(B)$ est une partie compacte de F et $u$ est une application linéaire compacte du dual fort $E'_b$ de E dans F.

En effet, la topologie induite sur B par $\sigma (E',E)$ est métrisable (EVT, III, p. 19, cor. 2). L’hypothèse du corollaire entraîne donc que la restriction de $u$ à B est une application continue de B dans F, lorsque B est muni de la topologie $\sigma (E',E)$, et le corollaire résulte de la proposition précédente.

#### Corollaire 2 {#ts-iii-s1-prop-7-cor-2 .statement tag=02OG}

Soient E un espace semi-normé et $\mathfrak{S}$ un ensemble de parties précompactes de E dont la réunion est dense dans E. Notons $E'_b$ le dual fort de E et $E'_{\mathfrak{S}}$ le dual de E muni de la $\mathfrak{S}$-topologie. L’espace $E'_{\mathfrak{S}}$ est séparé et l’application identique de $E'_b$ dans $E'_{\mathfrak{S}}$ est compacte.

L’espace $E'_{\mathfrak{S}}$ est séparé d’après TG, X, p. 8, prop. 7 ; sur la boule unité de $E'$, la $\mathfrak{S}$-topologie coïncide avec la topologie faible $\sigma (E',E)$ (EVT, III, p. 17, prop. 5), d’où le corollaire.

#### Exemple {#ts-iii-s1-n2-exa-1 .statement tag=02OH}

Soit E un espace semi-normé. L’application identique de $E'_b$ dans l’espace $E'$, muni de la topologie faible, de la topologie de la convergence compacte ou de la topologie de la convergence précompacte, est compacte.

#### Proposition 8 {#ts-iii-s1-prop-8 .statement tag=02OI}

Soient E un espace de Banach réflexif, B sa boule unité, F un espace localement convexe séparé et $u: E\rightarrow F$ une application linéaire. Les conditions suivantes sont équivalentes :

(i) L’application linéaire $u$ est compacte ;

(ii) L’ensemble $u(B)$ est une partie compacte de F ;

(iii) La restriction de $u$ à B est une application continue de l’ensemble B, muni de la topologie induite par $\sigma (E,E')$, dans F ;

(iv) Pour toute suite $(x_n)_{n\in\mathbf{N}}$ de points de B qui converge vers 0 pour la topologie $\sigma (E,E')$, la suite $(u(x_n))_{n\in\mathbf{N}}$ converge vers 0 dans F ;

(v) De toute suite infinie de points de $u(B)$, on peut extraire une suite qui converge dans F ;

(vi) Toute suite infinie de points de $u(B)$ a une valeur d’adhérence dans F.

Comme E est un espace réflexif, B est une partie compacte de $E_{\sigma}$ (EVT, IV, p. 17, prop. 6), donc (iii) implique (ii). La condition (ii) implique (i) par définition, et la condition (i) implique (iii) d’après la prop. 6. Il est également élémentaire que (iii) implique (iv) et que (v) implique (vi).

Nous allons maintenant démontrer que (iv) implique (v). Soit $(x_n)$ une suite infinie de points de B. Comme B est une partie compacte de $E_{\sigma}$, il existe d’après le théorème de $\breve{S}$mulian (EVT, IV, p. 36, th. 2) une suite $(y_n)$, extraite de la suite $(x_n)$, qui converge dans $E_{\sigma}$ vers une limite $y$. La suite $(y_n-y)$ est bornée dans $E_{\sigma}$, donc dans E (EVT, IV, p. 1, prop. 1) ; elle est donc contenue dans un ensemble homothétique de B. Si la condition (iv) est satisfaite, la suite $(u(y_n-y))$ converge vers 0 dans F, et $(u(y_n))$, qui est une suite extraite de $(u(x_n))$, converge vers $u(y)$. Cela prouve que (iv) implique (v).

Démontrons pour finir que (vi) implique (ii). Soit $j: F\rightarrow \widehat{F}$ l’injection canonique de F dans son complété. Sous l’hypothèse (vi), $u(B)$ est une partie précompacte de F (EVT, IV, p. 32, prop. 1), donc $j(u(B))$ est une partie relativement compacte de $\widehat{F}$ (TG, II, n$^{\circ}2$, p. 29) et $j\circ u$ est une application linéaire compacte. D’après l’équivalence déjà démontrée des conditions (i) et (ii), $j(u(B))$ est une partie compacte de $\widehat{F}$. Par suite, $u(B)$ est une partie compacte de F.

### 3. Transposition

Soient E un espace localement convexe et $E'$ son dual. Rappelons que l’on note $E'_b$ et $E'_c$ les espaces localement convexes obtenus en munissant l’espace vectoriel $E'$ de la topologie de la convergence bornée et de celle de la convergence compacte respectivement (EVT, III, p. 14). L’espace $E'_b$ est aussi appelé le dual fort de E (loc. cit., exemple 4).

#### Proposition 9 {#ts-iii-s1-prop-9 .statement tag=02OJ}

Soient E un espace localement convexe, F un espace localement convexe séparé et $u$ une application linéaire continue de E dans F.

a) Si l’application $u$ est compacte, alors sa transposée $^tu$ est une application linéaire compacte de $F'_c$ dans $E'_c$ et une application linéaire continue de $F'_c$ dans $E'_b$;

b) Supposons que l’espace E soit un espace semi-normé et que l’espace F soit quasi-complet. Si la transposée $^tu$ est une application continue de $F'_c$ dans $E'_b$, alors l’application linéaire $u$ est compacte.

Supposons d’abord que l’application linéaire $u$ est compacte. Il existe alors un voisinage V de 0 dans E dont l’image par $u$ est contenue dans une partie compacte C de F. De par sa définition (EVT, II, p. 47, déf. 2 et p. 68, déf. 1), le polaire $C^{\circ}$ de C est un voisinage de 0 dans $F'_c$ et l’on a $^tu(C^{\circ})\subset V^{\circ}$. Or $V^{\circ}$ est une partie équicontinue de $E'$, fermée pour la topologie faible, donc compacte dans $E'_c$ (EVT, III, p. 17, cor. 2 et prop. 5). Cela prouve que $^tu$ est une application linéaire compacte de $F'_c$ dans $E'_c$.

Conservons les hypothèses précédentes et soit U un voisinage de 0 dans $E'_b$. Il contient le polaire $A^{\circ}$ d’une partie bornée A de E. Comme l’application linéaire $u$ est compacte, l’ensemble $u(A)$ est relativement compact dans F (remarque 1 de III, p. 2), et $(^tu)^{-1}(A^{\circ}) =u(A)^{\circ}$ est un voisinage de 0 dans $F'_c$. Cela prouve que $^tu$ est une application linéaire continue de $F'_c$ dans $E'_b$.

Plaçons-nous maintenant sous les hypothèses de b) et notons B la boule unité de E. Le polaire $B^{\circ}$ de B est la boule unité de $E'_b$ et l’on a $(^tu)^{-1}(B^{\circ}) =u(B)^{\circ}$. Si $^tu$ est une application continue de $F'_c$ dans $E'_b$, l’ensemble $u(B)^{\circ}$ est donc un voisinage de 0 dans $F'_c$; il contient alors le polaire $C^{\circ}$ d’une partie compacte C de F. D’après le théorème des bipolaires (EVT, II, p. 49, cor. 3), l’ensemble $u(B)$ est contenu dans l’enveloppe fermée convexe de $C\cup  \{0\}$; celle-ci est compacte parce que l’espace F est quasi-complet (EVT, III, p. 8). Cela prouve que l’application linéaire $u$ est compacte.

#### Corollaire 1 (Schauder) {#ts-iii-s1-prop-9-cor-1 .statement tag=02OK}

Soient E un espace semi-normé, F un espace de Banach, $E'$ et $F'$ leurs duals forts respectifs et $u$ une application linéaire continue de E dans F. Les propriétés suivantes sont équivalentes :

(i) L’application linéaire $u$ de E dans F est compacte ;

(ii) L’application linéaire $^tu$ de $F'$ dans $E'$ est compacte ;

(iii) L’application linéaire $^tu$ de $F'_c$ dans $E'$ est continue.

L’équivalence de (i) et (iii) résulte de la prop. 9, a) et b) ; l’implication (iii)$\Rightarrow$(ii) provient du fait que l’application identique de $F'$ dans $F'_c$ est compacte (cor. de la prop. 7 de III, p. 7).

Démontrons pour conclure que la condition (ii) implique (i). Supposons que l’application linéaire $^tu: F'\rightarrow E'$ soit compacte. Il résulte de l’implication (i)$\Rightarrow$(ii), appliquée à $^tu$, que $^{tt}u$ est une application linéaire compacte de $E''$ dans $F''$. Notons $v$ l’application linéaire canonique de E dans $E''$; elle est continue. Comme F s’identifie à un sous-espace vectoriel fermé de $F''$ et que $u$ coïncide avec $^t(^tu)\circ v$ sur E, il résulte de la remarque 5 de III, p. 3 que l’application linéaire $u$ est compacte.

#### Corollaire 2 {#ts-iii-s1-prop-9-cor-2 .statement tag=02OL}

Soient E un espace semi-normé et F un espace de Banach de type dénombrable. Soit $u$ une application linéaire continue de E dans F. On suppose que pour toute suite $(y_n)$ d’éléments de $F'$ tendant faiblement vers 0, la suite $(^tu(y_n))$ tend fortement vers 0 dans $E'$. Alors l’application linéaire $u$ est compacte.

Notons $B'$ la boule unité de $F'$, munie de la topologie induite par la topologie $\sigma (F',F)$. Comme F est un espace de Banach de type dénombrable, $B'$ est un espace compact métrisable (EVT, III, p. 19, cor. 2). Sous l’hypothèse faite, la restriction de $^tu$ à $B'$ est une application continue de $B'$ dans $E'$ et $^tu(B')$ est une partie compacte de $E'$. D’après le cor. 1, l’application linéaire $u$ est compacte.

#### Remarque {#ts-iii-s1-n3-rem-1 .statement tag=02OM}

Soient E et F des espaces localement convexes séparés. La transposée d’une application linéaire compacte de E dans F n’est pas toujours une application linéaire compacte de $F'_b$ dans $E'_b($cf. III, p. 108, exercice 15).

### 4. Le théorème de Leray–Schauder

Le théorème suivant sera démontré dans TA, à paraître.

#### Théorème 1 (Brouwer) {#ts-iii-s1-thm-1 .statement tag=02ON}

Soit B une partie convexe compacte non vide d’un espace vectoriel normé de dimension finie. Toute application continue de B dans B possède un point fixe.

Nous allons en déduire le résultat suivant.

#### Théorème 2 (Leray–Schauder) {#ts-iii-s1-thm-2 .statement tag=02OO}

Soit X un espace topologique compact non vide, homéomorphe à une partie convexe d’un espace localement convexe. Toute application continue de X dans X possède un point fixe.

On peut supposer que X est une partie convexe d’un espace localement convexe E. Soient N l’adhérence de $\{0\}$ dans E et $\pi : E\rightarrow E/N$ la surjection canonique. Puisque X est un espace séparé, la restriction de $\pi$ à X est injective ; puisque X est compact, elle définit alors un homéomorphisme de X sur une partie convexe compacte non vide de l’espace localement convexe séparé $E/N$. Cela nous permet de supposer que l’espace E est séparé.

Soit $f: X\rightarrow X$ une application continue. L’application $h: X\rightarrow E$ définie par $h(x) =f(x)-x$ est continue ; comme X est compact, l’image $h(X)$ est fermée. Il suffit donc de prouver que 0 est adhérent à $h$(X), c’est-à-dire que pour tout voisinage ouvert convexe U de 0 dans E, il existe un point $b$ de X tel que $f(b)-b\in U$.

Soit U un voisinage convexe de 0 dans E. Pour tout $a\in X$, désignons par $V_a$ l’ensemble des éléments $x$ de X tels que $f(x)-f(a)\in U$. Il est ouvert dans X et contient $a$. Comme X est compact et non vide, il existe une partie finie non vide A de X telle que les ensembles $V_a$, pour $a\in A$, recouvrent X. Soit $(\varphi_a)_{a\in A}$ une partition continue de l’unité subordonnée au recouvrement $(V_a)_{a\in A}$ (TG, IX, p. 43, prop. 1 et p. 47, th. 3). Notons F le sous-espace vectoriel de E engendré par $f(A)$. Pour tout $x\in F\cap X$, posons

$$
g(x) =\sum_{a\in A}\varphi_a(x)f(a)
$$

On définit ainsi une application continue $g: F\cap X\rightarrow E$. Son image est contenue dans l’enveloppe convexe de $f$(A), donc dans $F\cap X$. Comme l’ensemble $F\cap X$ est une partie convexe compacte non vide d’un espace vectoriel de dimension finie, l’application $g$ possède un point fixe $b\in F\cap X$ d’après le théorème 1. On a

$$
f(b)-b=f(b)-g(b) =\sum_{a\in A}\varphi_a(b) (f(b)-f(a))
$$

Pour tout $a\in$ A tel que $\varphi_a(b)\not = 0$, on a $b\in V_a$ de sorte que $f(b)-f(a)\in U$. Comme U est convexe, on conclut que $f(b)-b\in U$, ce qui achève la démonstration.

### 5. Sous-espaces invariants par un opérateur compact

Le théorème suivant est à rapprocher du lemme de Schur (A, VIII, p. 43, cor. et V, p. 386, prop. 6) et du cor. 4 de I, p. 26.

#### Théorème 3 {#ts-iii-s1-thm-3 .statement tag=02OP}

Soient E un espace localement convexe séparé sur $\mathbf{C}$ et A une partie de $\mathscr{L}(E)$. Faisons les hypothèses suivantes :

(i) Il n’existe aucun sous-espace vectoriel fermé de E, distinct de $\{0\}$ et E, qui soit stable par A ;

(ii) L’ensemble A contient un endomorphisme compact non nul. Alors le commutant de A est réduit aux homothéties.

En remplaçant A par la sous-algèbre unifère de $\mathscr{L}(E)$ engendrée par A, on se ramène au cas où A est une sous-algèbre unifère de $\mathscr{L}(E)$. Soit alors $h$ un endomorphisme compact non nul de E appartenant à A.

#### Lemme 1 {#ts-iii-s1-lem-1 .statement tag=02OQ}

Il existe un élément $a$ de A tel que le noyau de $ha-1_E$ ne soit pas réduit à 0.

Il existe un élément $x_0$ de E tel que $h(x_0)\not = 0$. Soit V un voisinage fermé de $h(x_0)$ ne contenant pas 0. Comme l’endomorphisme $h$ est compact, on peut choisir un voisinage ouvert convexe U de $x_0$ tel que $h(U)$ soit une partie relativement compacte de V. L’adhérence C de $h(U)$ est donc une partie convexe compacte de E ; comme elle est contenue dans V, elle ne contient pas 0.

Soit $y$ un point de C. Notons $Ay$ l’ensemble des images de $y$ par les éléments de A. C’est un sous-espace vectoriel de E stable par A ; il est non nul car il contient $y$. D’après l’hypothèse (i) du théorème, l’ensemble $Ay$ est dense dans E. Il existe donc un élément $b$ de A tel que $b(y)\in U$. Comme l’ensemble C est compact, il existe une

$-1$

famille finie $(b_1, . . . , b_n)$ d’éléments de A tels que les ensembles $b_i(U)$ recouvrent C. Il existe une partition continue de l’unité $(\varphi_1, . . . , \varphi_n)$ sur C subordonnée à ce recouvrement (TG, IX, p. 47, th. 3). Définissons une application $f: C\rightarrow E$ en posant

$$
f(x) =\sum_{i=1}^n\varphi_i(x)b_i(x)
$$

pour tout $x\in C$; c’est une application continue. Comme U est convexe et que $b_i(x)$ appartient à U lorsque $\varphi_i(x)$ n’est pas nul, on a $f(C)\subset U$ et $h(f(C))\subset C$. D’après le théorème de Leray–Schauder (th. 2 de III, p. 11), il existe un élément $x\in C$ tel que $h(f(x)) =x$. Posons alors

$$
a=\sum_{i=1}^n\varphi_i(x)b_i
$$

On a $h(a(x)) =h(f(x)) =x$ et $x$ est non nul puisque 0 n’appartient pas à C, donc le noyau de $ha-1_E$ n’est pas nul.

Terminons la démonstration du théorème 3. Soit $a$ un élément de A tel que le noyau T de $ha-1_E$ soit non nul (lemme 1). Notons $i$ l’injection canonique de T dans E. L’application linéaire $i$ est égale à $h\circ a\circ i$, elle est donc compacte. Ainsi la dimension de T est finie (remarque 3 de III, p. 2). Soit $u$ un élément de $\mathscr{L}(E)$ qui commute à A. Comme $u$ commute à $h\circ a$, on a $u(T)\subset T$. Comme T est de dimension finie non nulle sur le corps algébriquement clos $\mathbf{C}$, l’endomorphisme de T induit par $u$ admet une valeur propre $\lambda$.

Posons F = Ker($u-\lambda 1_E$). C’est un sous-espace vectoriel fermé non nul de E ; il est stable par A, puisque $u$ commute aux éléments de A. D’après l’hypothèse (i), on a F = E, d’où $u=\lambda 1_E$.

#### Corollaire 1 {#ts-iii-s1-lem-1-cor-1 .statement tag=02OR}

Conservons les hypothèses du théorème 3 et supposons de plus que les éléments de A soient deux à deux permutables. Alors E est de dimension 1 sur $\mathbf{C}$.

D’après l’hypothèse (ii) du théorème 3, l’espace E n’est pas nul. Il contient donc un sous-espace vectoriel F de dimension 1. Ce sous-espace est fermé car E est supposé séparé. D’après le th. 3, tout élément de A est une homothétie, donc stabilise F. Il résulte alors de l’hypothèse (i) du th. 3 que F est égal à E.

#### Corollaire 2 (Lomonosov) {#ts-iii-s1-lem-1-cor-2 .statement tag=02OS}

Soient E un espace localement convexe séparé de dimension au moins 2 sur le corps $\mathbf{C}$ et $u$ un endomorphisme de E. On suppose qu’il existe un endomorphisme compact $h\not = 0$ de E permutable à $u$. Il existe alors un sous-espace vectoriel fermé F de E, distinct de $\{0\}$ et de E, tel que $u(F)\subset F$.

En effet, le corollaire 1 montre que l’ensemble $A =\{u, h\}$ ne peut satisfaire à l’hypothèse (i) du théorème 3.

#### Corollaire 3 {#ts-iii-s1-lem-1-cor-3 .statement tag=02OT}

Soient E un espace localement convexe séparé sur le corps $\mathbf{C}$ et $u$ un endomorphisme compact de E. Si E est de dimension au moins 2, il existe un sous-espace vectoriel fermé F de E, distinct de $\{0\}$ et de E, tel que $u(F)\subset F$.

Le cas $u= 0$ est immédiat. Le cas $u\not = 0$ se déduit du cor. 2 en prenant $h=u$.

### 6. Espaces d’approximation

Étant donnés des espaces localement convexes E et F, rappelons (EVT, III, p. 14, exemple 2) que l’on note $\mathscr{L}_{pc}(E; F)$ l’espace localement convexe obtenu en munissant $\mathscr{L}(E; F)$ de la topologie de la convergence précompacte. On note aussi $\mathscr{L}_{pc}(E)$ l’espace localement convexe $\mathscr{L}_{pc}(E; E)$. Lorsque l’espace localement convexe E est séparé et quasi-complet (EVT, III, p. 8, déf. 6), la topologie de la convergence précompacte sur $\mathscr{L}(E; F)$ coïncide avec la topologie de la convergence compacte, puisque l’adhérence d’une partie précompacte de E est compacte (EVT, III, p. 8).

#### Définition 2 {#ts-iii-s1-def-2 .statement tag=02OU}

On dit qu’un espace localement convexe E possède la propriété d’approximation, ou encore est un espace d’approximation, si l’application identique $1_E$ de E est adhérente dans l’espace $\mathscr{L}_{pc}(E)$ à l’ensemble $\mathscr{L}^f(E)$ des endomorphismes continus de rang fini de E.

En particulier, tout espace localement convexe de dimension finie est un espace d’approximation.

#### Remarque 1 {#ts-iii-s1-n6-rem-1 .statement tag=02OV}

Pour que la somme directe topologique d’espaces localement convexes E et F soit un espace d’approximation, il faut et il suffit que E et F soient des espaces d’approximation.

#### Remarque 2 {#ts-iii-s1-n6-rem-2 .statement tag=02OW}

Soit E un espace localement convexe. Soient N l’adhérence de $\{0\}$ dans E et P un sous-espace supplémentaire algébrique de N dans E. Alors P est un supplémentaire topologique de N dans E, et est isomorphe à l’espace localement convexe $E/N$. L’espace N est un espace d’approximation. D’après la remarque 1, pour que E soit un espace d’approximation, il faut et il suffit que l’espace localement convexe séparé $E/N$ en soit un.

#### Remarque 3 {#ts-iii-s1-n6-rem-3 .statement tag=02OX}

Soient E un espace localement convexe, A une partie équicontinue de $\mathscr{L}^f(E)$ et T une partie totale de E. Si $1_E$ est adhérent à A pour la topologie de la convergence simple dans T, alors $1_E$ est adhérent à A dans $\mathscr{L}_{pc}(E)$ (EVT, III, p. 16, prop. 4 et p. 17, prop. 5), et E est un espace d’approximation.

#### Remarque 4 {#ts-iii-s1-n6-rem-4 .statement tag=02OY}

Soit E un espace localement convexe sur $\mathbf{C}$. Notons $E_0$ l’espace localement convexe sur $\mathbf{R}$ sous-jacent à E. Pour que E soit un espace d’approximation, il faut et il suffit que $E_0$ en soit un. En effet, la condition est nécessaire ; démontrons qu’elle est suffisante. Supposons donc que $E_0$ soit un espace d’approximation. Soient C une partie précompacte de E et U un voisinage convexe équilibré de 0 dans E. Posons $C'= C\cup iC$. Il existe une application $\mathbf{R}$-linéaire $u$ continue de rang fini de $E_0$ dans $E_0$ telle que $x-u(x)$ appartienne à U pour tout $x\in C'$. Posons $v(x) =^1_2(u(x)-iu(ix))$ pour tout $x$ dans E. On définit ainsi une application $\mathbf{C}$-linéaire continue de rang fini de E dans E. Pour tout $x\in C$, on a $x\in C',ix\in C'$ et $x-v(x) =^1_2(x-u(x))-_2^i(ix-u(ix))$, de sorte que $x-v(x)$ appartient à U. Cela prouve que E est un espace d’approximation.

#### Remarque 5 {#ts-iii-s1-n6-rem-5 .statement tag=02OZ}

Soit E un espace localement convexe sur $\mathbf{R}$. Pour que l’espace localement convexe complexifié $E_{(\mathbf{C})}$ de E soit un espace d’approximation, il faut et il suffit que E en soit un. Cela résulte des remarques 1 et 4, puisque l’espace localement convexe réel sous-jacent à $E_{(\mathbf{C})}$ est isomorphe à $E\times E$.

#### Proposition 10 {#ts-iii-s1-prop-10 .statement tag=02P0}

Soit E un espace hilbertien. Alors E est un espace d’approximation.

L’ensemble A des orthoprojecteurs de rang fini dans E est équicontinu. Soient $n\geqslant 1$ un entier et $(x_1, . . . , x_n)$ une famille d’éléments de E. Notons V le sous-espace vectoriel engendré par les $x_i$ et $p_V$ l’orthoprojecteur d’image V. On a $p_V(x_i) =x_i$ pour $1\leqslant i\leqslant n$. Cela entraîne que $1_E$ est adhérent à A pour la topologie de la convergence simple, et il en résulte que E est un espace d’approximation (remarque 3).

D’autres exemples d’espaces d’approximation seront donnés dans le n$^o7$ de III, p. 20.

#### Lemme 2 {#ts-iii-s1-lem-2 .statement tag=02P1}

Soit E un espace localement convexe. Alors E est un espace d’approximation si et seulement si, pour toute partie précompacte C de E et tout voisinage U de 0 dans E, il existe un entier $n\geqslant 0$, des éléments $e_1, . . . , e_n$ de E, et des formes linéaires continues $f_1, . . . , f_n$ sur E, tels que $x-\sum^n_{i=1}f_i(x)e_i$ appartienne à U pour tout $x\in C$.

La définition de la topologie de la convergence précompacte montre que la condition est suffisante. Inversement, supposons que E soit un espace d’approximation. Soit P un espace supplémentaire topologique dans E de l’adhérence de $\{0\}($cf. remarque 2). L’ensemble A des $u\in \mathscr{L}^f(E)$ tels que $u(E)\subset P$ est alors dense dans $\mathscr{L}^f(E)$. Comme P est séparé, tout élément $u$ de A est de la forme $x\mapsto \sum^n_{i=1}f_i(x)e_i$, où $n\in \mathbf{N},e_1, . . . , e_n$ sont des éléments de E et $f_1, . . . , f_n$ des formes linéaires continues sur E (EVT, I, p. 14, th. 2). Cela prouve que la condition est nécessaire.

#### Remarque 6 {#ts-iii-s1-n6-rem-6 .statement tag=02P2}

Il existe des espaces de Banach qui ne possèdent pas la propriété d’approximation, comme l’a démontré P. Enflo (A counterexample to the approximation problem in Banach spaces, Acta Math. 130 (1973), p. 309–317 ; cf. exercice 25 de III, p. 112). Cela répondait à une question de S. Banach (Théorie des opérations linéaires, Monografje Matematyczne I, Warszawa, 1932, remarques au chapitre VI, §1). Voir aussi la remarque p. 21.

#### Proposition 11 {#ts-iii-s1-prop-11 .statement tag=02P3}

Soient E et F des espaces localement convexes. Supposons que E soit un espace d’approximation.

a) L’ensemble $\mathscr{L}^f(E; F)$ est dense dans $\mathscr{L}_{pc}(E; F)$;

b) L’ensemble $\mathscr{L}^f(F; E)$ est dense dans $\mathscr{L}_{pc}(F; E)$;

c) Soient $\mathfrak{S}$ un ensemble de parties bornées de F et $u\in \mathscr{L}(F; E)$. Supposons que l’image par $u$ de toute partie de F appartenant à $\mathfrak{S}$ soit précompacte. Alors $u$ est adhérent à $\mathscr{L}^f(F; E)$ pour la $\mathfrak{S}$-topologie (EVT, III, p. 13).

Soit $v$ un élément de $\mathscr{L}(E; F)$. L’application $\varphi :w\mapsto v\circ w$ de $\mathscr{L}_{pc}(E)$ dans $\mathscr{L}_{pc}(E; F)$ est continue (TG, X, p. 5, prop. 3). On a $\varphi (1_E) =v$ et $\varphi (\mathscr{L}^f(E))\subset \mathscr{L}^f(E; F)$, donc $v$ est adhérent à $\mathscr{L}^f(E; F)$ dans $\mathscr{L}_{pc}(E; F)$. Cela prouve a).

De même, sous les hypothèses de c), l’application $\psi :w\mapsto w\circ u$ de $\mathscr{L}_{pc}(E)$ dans $\mathscr{L}_{\mathfrak{S}}(F; E)$ est continue (loc. cit.). On a $\psi (1_E) =u$ et $\psi (\mathscr{L}^f(E))\subset \mathscr{L}^f(F; E)$, donc $u$ est adhérent à $\mathscr{L}^f(F; E)$ dans $\mathscr{L}_{\mathfrak{S}}(F; E)$.

L’image d’une partie précompacte de F par une application linéaire continue de F dans E est précompacte, donc b) résulte de c).

#### Corollaire {#ts-iii-s1-n6-cor-1 .statement tag=02P4}

Soient E un espace d’approximation séparé et F un espace localement convexe. Toute application linéaire compacte de F dans E est adhérente à $\mathscr{L}^f(F; E)$ dans l’espace $\mathscr{L}(F; E)$ muni de la topologie de la convergence bornée.

Cela résulte de la prop. 11, c), car l’image d’une partie bornée de F par une application linéaire compacte de F dans E est relativement compacte dans E (remarque 1 de III, p. 2), donc précompacte.

#### Proposition 12 {#ts-iii-s1-prop-12 .statement tag=02P5}

Soient E un espace localement convexe, I un ensemble, et pour chaque $i\in I$, soient $F_i$ un espace localement convexe et $v_i: E\rightarrow F_i$ une application linéaire continue d’image dense. Supposons que pour tout voisinage U de 0 dans E, il existe $i\in I$ et un voisinage V de 0 dans $F_i$ tels que $\overset{-1}{v_{i}}(V)\subset U$. Si les $F_i$ sont des espaces d’approximation, alors E en est un également.

Soient A une partie précompacte de E et U un voisinage de 0 dans E. Il existe par hypothèse $i\in I$ et une semi-norme continue $p$ sur $F_i$ tels que U contienne $(p\circ v_i)^{-1}([0,1])$. Posons $F = F_i,v=v_i$ et $B =v$(A), et supposons que F soit un espace d’approximation. L’ensemble B est précompact dans F. Il existe donc (lemme 2) un entier $n\geqslant 1$, des éléments $y_1, . . . , y_n$ de F et des formes linéaires continues $f_1, . . . , f_n$ sur F, tels que l’on ait, pour tout $y\in B$,

$^n$ 1

$$
py-\sum f_j(y)y_j\leqslant
$$

2

$j=1$

Comme B est borné (EVT, III, p. 3, prop. 2), il existe un nombre réel $M>0$ tel que $|f_j(y)|\leqslant M$ pour tout $j$ tel que $1\leqslant j\leqslant n$ et tout $y\in B$. De plus, puisque $v(E)$ est dense dans F, il existe, pour chaque entier $j$ tel que $1\leqslant j\leqslant n$, un élément $x_j$ de E tel que $p(y_j-v(x_j))\leqslant (2nM)^{-1}$. L’application linéaire

$$
u:x\longmapsto \sum_{j=1}^nf_j(v(x))x_j
$$

appartient à $\mathscr{L}^f(E)$. Pour tout $x\in A$, on a

$$
v(x-u(x)) =v(x)-\sum_{j=1}^nf_j(v(x))y_j+\sum_{j=1}^nf_j(v(x))(y_j-v(x_j))
$$

d’où $p(v(x-u(x)))\leqslant^1_2+_{2nM}^{nM}= 1$, et par suite $x-u(x)\in U$. La proposition en résulte.

#### Corollaire 1 {#ts-iii-s1-prop-12-cor-1 .statement tag=02P6}

Un sous-espace vectoriel dense d’un espace d’approximation est un espace d’approximation.

#### Corollaire 2 {#ts-iii-s1-prop-12-cor-2 .statement tag=02P7}

Si le séparé complété d’un espace localement convexe E est un espace d’approximation, alors E est un espace d’approximation.

#### Corollaire 3 {#ts-iii-s1-prop-12-cor-3 .statement tag=02P8}

Le produit d’une famille d’espaces d’approximation est un espace d’approximation.

Soit en effet $(E_i)_{i\in I}$ une famille d’espaces d’approximation. Pour toute partie finie J de I, posons $E_J=\prod_{i\in J}E_i$ et notons $v_J$ l’application canonique de $E =\prod_{i\in I}E_i$ dans $E_J$. L’espace localement convexe $E_J$ est un espace d’approximation (remarque 1). Le corollaire résulte alors de la prop. 12 appliquée à l’espace localement convexe E, à la famille $(E_J)$ d’espaces localement convexes et aux applications linéaires continues $v_J: E\rightarrow E_J$.

#### Corollaire 4 {#ts-iii-s1-prop-12-cor-4 .statement tag=02P9}

Soit E un espace localement convexe. Si toute semi-norme continue sur E est majorée par une semi-norme continue préhilbertienne, alors E est un espace d’approximation.

Soit $\mathscr{P}$ l’ensemble des semi-normes préhilbertiennes continues sur E. Pour chaque $p\in \mathscr{P}$, l’hypothèse implique que l’espace semi-normé $E_p$ obtenu en munissant E de la semi-norme $p$ est un espace d’approximation (corollaire 2 et proposition 10), et l’application identique de E dans $E_p$ est continue. Le corollaire résulte donc de la proposition 12.

#### Lemme 3 {#ts-iii-s1-lem-3 .statement tag=02PA}

Soient E un espace localement convexe métrisable et $(x_n)_{n\in\mathbf{N}}$ une suite d’éléments de E convergeant vers 0. Il existe une suite $(y_n)_{n\in\mathbf{N}}$ d’éléments de E convergeant vers 0 et une suite $(\lambda_n)_{n\in\mathbf{N}}$ d’éléments de l’intervalle $[0,1]$ convergeant vers 0 telles que l’on ait $x_n=\lambda_ny_n$ pour tout $n\in \mathbf{N}$.

Puisque E est métrisable, il existe un système fondamental $(V_m)_{m\in\mathbf{N}}$ de voisinages équilibrés de 0 dans E tel que $V_0= E$ et $2^{m+1}V_{m+1}\subset V_m$ pour tout $m\geqslant 0$. Puisque $(x_n)$ converge vers 0, il existe une suite strictement croissante $(N_m)_{m\in\mathbf{N}}$ d’entiers telle que $N_0= 0$ et telle que, pour tout $m\geqslant 0$, on ait $x_n\in V_m$ pour $n\geqslant N_m$. Pour tout entier $n\geqslant 0$, il existe un unique entier $m\geqslant 0$ tel que $N_m\leqslant n <N_{m+1}$, et on pose alors $\lambda_n= 2^{-m}$ et $y_n= 2^mx_n$. La suite $(\lambda_n)$ ainsi définie converge vers 0. De plus, comme $y_n\in V_m$ pour $n\geqslant N_{m+1}$, la suite $(y_n)$ converge vers 0 dans E. Enfin, on a $x_n=\lambda_ny_n$ pour tout $n$.

Rappelons (EVT, II, p. 28) que si E est un espace vectoriel et L une partie convexe équilibrée de E, on note $E_L$ le sous-espace vectoriel de E engendré par L, muni de la semi-norme dont la boule unité est L. Lorsque l’ensemble L ne contient aucune droite, cette semi-norme est une norme.

#### Lemme 4 {#ts-iii-s1-lem-4 .statement tag=02PB}

Soient E un espace de Fréchet et A une partie compacte de E. Il existe une partie compacte convexe équilibrée L de E contenant A telle que les topologies induites sur A par celles de E et de $E_L$ coïncident.

L’ensemble A est contenu dans l’enveloppe fermée convexe équilibrée de l’ensemble des points d’une suite $(x_n)_{n\in\mathbf{N}}$ d’éléments de E convergeant vers 0 (EVT, IV, p. 24, cor. 1). Soient $(y_n)_{n\in\mathbf{N}}$ et $(\lambda_n)_{n\in\mathbf{N}}$ des suites satisfaisant aux conclusions du lemme 3. L’enveloppe fermée convexe équilibrée L des points de la suite $(y_n)$ contient A et est une partie compacte de E (EVT, III, p. 8). Par suite, $E_L$ est un espace de Banach (EVT, III, p. 8, cor.). Dans cet espace de Banach, la norme de $x_n$ est majorée par $\lambda_n$, donc la suite $(x_n)$ tend vers 0. L’enveloppe fermée convexe équilibrée $\widetilde{A}$ de la suite $(x_n)$ dans $E_L$ est une partie compacte de $E_L$ (EVT, III, p. 8). Comme L est une partie bornée de E, l’injection canonique de $E_L$ dans E est continue. Les topologies induites sur $\widetilde{A}$ par celles de $E_L$ et de E coïncident, et $\widetilde{A}$ est une partie compacte, donc fermée, de E. Puisque l’ensemble $\widetilde{A}$ est convexe, équilibré et contient la suite $(x_n)$, il contient A. Ceci achève la démonstration.

#### Théorème 4 {#ts-iii-s1-thm-4 .statement tag=02PC}

Soit E un espace de Fréchet.

a) Supposons que E soit un espace d’approximation. Alors, pour tout espace semi-normé F, l’espace $\mathscr{L}^f(F; E)$ est dense dans $\mathscr{L}^c(F; E)$ pour la topologie de la convergence bornée ;

b) Inversement, supposons que pour tout espace de Banach F, toute application linéaire compacte de F dans E soit adhérente à $\mathscr{L}^f(F; E)$ pour la topologie de la convergence bornée. Alors E est un espace d’approximation.

Soit F un espace semi-normé. L’adhérence de $\mathscr{L}^f(F; E)$ dans $\mathscr{L}(F; E)$ est contenue dans $\mathscr{L}^c(F; E)$ (prop. 1 et 2 de III, p. 4). Elle est égale à $\mathscr{L}^c(F; E)$ si E est un espace d’approximation d’après le cor. de la prop. 11. Cela prouve l’assertion a).

Supposons satisfaite l’hypothèse de b). Soit $\varepsilon  >0$ un nombre réel. Soient A une partie compacte de E et $p$ une semi-norme continue sur E. Soit L une partie compacte convexe équilibrée de E telle que A soit une partie compacte de l’espace normé $E_L$ (lemme 4). L’injection canonique $j: E_L\rightarrow E$ est compacte et $E_L$ est un espace de Banach (EVT, III, p. 8, cor.). Il existe donc par hypothèse un entier $n\geqslant 1$, des éléments $e_1, . . . , e_n$ de E, et des formes linéaires continues $\ell_1, . . . , \ell_n$ sur $E_L$, tels que l’application $v$ de $E_L$ dans E définie par $v(x) =\sum^n_{i=1}\ell_i(x)e_i$ vérifie $p(x-v(x))\leqslant^{\varepsilon}_2$ pour $x\in A$. L’image de $^tj: E'\rightarrow (E_L)'$ est dense dans $(E_L)'$ pour la topologie faible (EVT, IV, p. 6, prop. 5). Sur $(E_L)'$ la topologie de la convergence compacte est compatible avec la dualité entre $(E_L)'$ et $E_L$ (EVT, IV, p. 3, exemple). Donc $^tj(E')$ est dense dans $(E_L)'$ pour la topologie de la convergence compacte (EVT, IV, p. 1, prop. 1), et il existe des formes linéaires continues $f_1, . . . , f_n$ sur E telles que

$$
|\ell_i(x)-f_i(x)|p(e_i)\leqslant_{2n}^{\varepsilon}
$$

pour $x\in A$ et $1\leqslant i\leqslant n$. L’endomorphisme $u:x\mapsto \sum^n_{i=1}f_i(x)e_i$ de E appartient à $\mathscr{L}^f(E)$ et pour tout $x\in A$, on a

$$
\varepsilon \varepsilon
$$

$$
p(x-u(x))\leqslant p(x-v(x)) +p(v(x)-u(x))\leqslant +n\times =\varepsilon
$$

2 $2n$

Il résulte de cela que $1_E$ est adhérent à $\mathscr{L}^f(E)$ pour la topologie de la convergence compacte. Or celle-ci coïncide avec la topologie de la convergence précompacte car E est complet. Donc E est un espace d’approximation.

### 7. Exemples d’espaces d’approximation

Rappelons que tout espace hilbertien est un espace d’approximation (III, p. 15, prop. 10). Ce numéro donne d’autres exemples.

Si X est un espace localement compact, on note $\mathscr{C}_0(X; K)$, ou simplement $\mathscr{C}_0$(X), l’espace de Banach des fonctions continues de X dans K tendant vers 0 à l’infini, muni de la norme définie par $\|f\|=$ sup$_{x\in X}|f(x)|$ pour $f\in \mathscr{C}_0(X)$. Lorsque X est compact, cet espace coïncide avec l’espace $\mathscr{C}(X)$ des fonctions continues de X dans K.

#### Lemme 5 {#ts-iii-s1-lem-5 .statement tag=02PD}

Soient X un espace topologique compact, F un sous-ensemble fini de $\mathscr{C}(X)$ et $\varepsilon  >0$ un nombre réel.

Il existe un sous-ensemble fini $X_0\subset X$ et une application linéaire $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ de norme $\leqslant 1$ tels que $\|u(f|X_0)-f\|\leqslant \varepsilon$ pour tout $f\in F$.

Puisque l’ensemble F est une partie équicontinue de $\mathscr{C}$ (X), il existe un recouvrement fini $(U_i)_{i\in I}$ de X tel que, pour tout $i\in I$ et tout $f\in F$, le diamètre de $f(U_i)$ soit $\leqslant \varepsilon$. Pour $i$ dans I, choisissons un point $x_i$ de $U_i$, et notons $X_0$ l’ensemble fini des $x_i$ pour $i\in I$.

Soit $(\varphi_i)_{i\in I}$ une partition continue de l’unité subordonnée à $(U_i)_{i\in I}$ (TG, IX, p. 47, th. 3). Définissons une application linéaire $u$ de $\mathscr{C}(X_0)$ dans $\mathscr{C}(X)$ en posant

$$
u(g) =\sum_{i\in I}g(x_i)\varphi_i
$$

pour tout $g\in \mathscr{C}(X_0)$. L’application linéaire $u$ est de norme $\leqslant 1$ et vérifie $\|u(f|X_0)-f\|\leqslant \varepsilon$ pour tout $f$ dans F, d’où l’assertion.

#### Proposition 13 {#ts-iii-s1-prop-13 .statement tag=02PE}

Soit X un espace topologique localement compact. L’espace de Banach $\mathscr{C}_0(X)$ est un espace d’approximation.

Supposons d’abord X compact. Soit $A\subset \mathscr{L}^f(\mathscr{C}(X))$ l’ensemble des applications de la forme $f\mapsto u(f|X_0)$, où $X_0$ est un sous-ensemble fini de X et $u:\mathscr{C}(X_0)\rightarrow \mathscr{C}(X)$ une application linéaire de norme $\leqslant 1$. L’ensemble A est équicontinu. Par le lemme 5, l’application identique de $\mathscr{C}(X)$ est adhérente à A pour la topologie de la convergence simple sur $\mathscr{C}(X)$. La proposition résulte alors de la remarque 3 de III, p. 14.

Passons au cas général. Soient Y le compactifié d’Alexandroff de X et $\omega$ le point à l’infini de Y (TG, I, p. 67). Identifions $\mathscr{C}_0(X)$ à l’ensemble des éléments de $\mathscr{C}(Y)$ nuls en $\omega$. Alors $\mathscr{C}(Y)$ est somme directe topologique de $\mathscr{C}_0(X)$ et de l’espace vectoriel des applications constantes sur Y. Comme $\mathscr{C}(Y)$ est un espace d’approximation d’après ce qui précède, l’espace $\mathscr{C}_0(X)$ est un espace d’approximation (remarque 1 de III, p. 14).

#### Corollaire {#ts-iii-s1-n7-cor-1 .statement tag=02PF}

Toute algèbre stellaire commutative est un espace d’approximation.

En effet, une telle algèbre est isomorphe à l’algèbre des fonctions continues tendant vers 0 à l’infini sur un espace localement compact (I, p. 108, th. 1).

#### Remarque {#ts-iii-s1-n7-rem-1 .statement tag=02PG}

Si E est un espace hilbertien de dimension infinie, l’algèbre stellaire $\mathscr{L}(E)$ n’a pas la propriété d’approximation (A. Szankowski, $\mathscr{B}(H)$ does not have the approximation property, Acta Math. 147 (1981), p. 89–108).

#### Lemme 6 {#ts-iii-s1-lem-6 .statement tag=02PH}

Soit X un espace topologique localement compact. Soit $\mu$ une mesure positive sur X et $p\in [1,+\infty [$. Soient F un sous-ensemble fini de $L^p_K(X, \mu)$ et $\varepsilon  >0$ un nombre réel.

Il existe un projecteur de rang fini $u$ de $L^p_K(X, \mu)$ de norme $\leqslant 1$ tel que $\|u(f)-f\|\leqslant \varepsilon$ pour tout $f$ dans F.

Soit $\mathscr{P}$ l’ensemble des partitions finies $\pi = (K_1, . . . ,K_n,H)$ de X, où $n\geqslant 1$ est un entier et $K_1, . . . ,K_n$ sont des parties intégrables et de mesure non nulle de X. Pour toute partition $\pi = (K_1, . . . ,K_n,H)\in \mathscr{P}$, on définit un endomorphisme $v_{\pi}$ de $\mathscr{L}^p(X, \mu)$ en posant

$^n$ 1 $\int$

$$
v_{\pi}(f) =\sum f d\mu\varphi_{K_i}
$$

$$
\mu(K_i)_{K_i}
$$

$i=1$

pour $f\in \mathscr{L}_K^p(X, \mu)$, où $\varphi_{K_i}$ est la fonction caractéristique de $K_i$. L’application $v_{\pi}$ induit, par passage aux quotients, un projecteur $u_{\pi}$ de $L^p_K(X, \mu)$. On vérifie aisément que l’image de $u_{\pi}$ est l’espace des classes de fonctions $f\in \mathscr{L}_K^p(X, \mu)$ telles que $f$ est nulle sur H et constante sur $K_i$ pour $1\leqslant i\leqslant n$.

Démontrons que $\|u_{\pi}\|\leqslant 1$. Pour $f\in \mathscr{L}_K^p(X, \mu)$, on a

$n\int p$

$\|u_{\pi}(f)\|^p_p=\sum\mu(K_i)^{1-p}f d\mu$.

$i=1K_i$

D’après l’inégalité de Hölder (INT, IV, p. 208, § 6, n$^o4$, th. 2), on a pour tout $i$ l’inégalité

$\int p\int$

$f d\mu\leqslant \mu(K_i)^{p-1}|f|^pd\mu$,

$K_iK_i$

d’où $\|u_{\pi}(f)\|_p\leqslant \|f\|_p$.

Soit $\mathscr{E}$ l’ensemble des classes dans $L^p_K(X, \mu)$ des fonctions intégrables sur X qui ne prennent qu’un nombre fini de valeurs. Comme $\mathscr{E}$ est dense dans $L^p_K(X, \mu)$ (INT, IV, p. 162, §4, n$^o10$, cor. 1), il existe un ensemble fini $F'$ de $\mathscr{E}$ tel que tout élément de F soit à distance au plus $\varepsilon$ d’un élément de $F'$. En considérant la partition finie $\pi$ formée par les ensembles de mesure non nulle où l’application $x\mapsto (f(x))_{f\in F'}$ prend une valeur donnée, on voit qu’il existe un élément $\pi$ de $\mathscr{P}$ tel que $u_{\pi}(f) =f$ pour tout $f$ dans $F'$. Le projecteur $u_{\pi}$ a donc les propriétés requises.

#### Proposition 14 {#ts-iii-s1-prop-14 .statement tag=02PI}

Soient X un espace topologique localement compact, $\mu$ une mesure positive sur X, et $p\in [1,+\infty ]$. L’espace $L^p_K(X, \mu)$ est un espace d’approximation.

Si $p= +\infty$, alors l’espace $L^{\infty}_{\mathbf{C}}(X, \mu)$ est une algèbre stellaire commutative (exemple 4 de I, p. 103), donc un espace d’approximation (cor. de la prop. 13), et il en est de même de $L^{\infty}_{\mathbf{R}}(X, \mu)$ d’après la remarque 5 de III, p. 15.

Supposons que $p$ est fini. Soit $A\subset \mathscr{L}^f(L^p_K(X, \mu))$ l’ensemble des projecteurs de rang fini et norme $\leqslant 1$. Par le lemme 6, l’application identique de $L^p_K(X, \mu)$ est adhérente à A pour la topologie de la convergence simple, et la proposition résulte alors de la remarque 3 de III, p. 14.

## EXERCICES {#ts-iii-s1-exercises}

Dans les exercices 1 à 5 exclusivement K désigne un corps valué complet non archimédien et non discret, dont on note $x\mapsto  |x|$ la valuation. On note aussi $G\subset \mathbf{R}^*_+$ l’image de $K^*$ par l’application $x\mapsto  |x|$. Les espaces de Banach considérés sont des espaces de Banach sur K.

See the [exercises for § 1](exercises/s1/).
