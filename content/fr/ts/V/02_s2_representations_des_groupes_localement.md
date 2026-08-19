---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 2
section_title: Représentations des groupes localement compacts
lang: fr
source: ts-iii-v-fr
book_pages: TS V.399-TS V.431, TS V.486-TS V.492
pdf_pages: 0412-0444, 0499-0505
extraction: native
subsections:
    - "no": 1
      title: Continuité de certaines représentations
      page: 399
      pdf_page: 412
    - "no": 2
      title: Extension de représentations à des espaces de mesures
      page: 400
      pdf_page: 413
    - "no": 3
      title: Critère de semi-simplicité
      page: 402
      pdf_page: 415
    - "no": 4
      title: Représentations régulières
      page: 405
      pdf_page: 418
    - "no": 5
      title: Fonctions équivariantes
      page: 407
      pdf_page: 420
    - "no": 6
      title: Représentations induites
      page: 415
      pdf_page: 428
    - "no": 7
      title: Cas d’un sous-groupe fermé central
      page: 416
      pdf_page: 429
    - "no": 8
      title: Représentations de carré intégrable
      page: 419
      pdf_page: 432
    - "no": 9
      title: Sous-représentations de la représentation régulière d’un groupe commutatif
      page: 425
      pdf_page: 438
    - "no": 10
      title: Représentations unitaires du groupe R
      page: 427
      pdf_page: 440
statements: 45
exercises: 20
content_sha256: eec3a032fa7b5e66f57c287f325099b4c057b4250ccf1d0461cd142a86adfd90
---

## § 2. REPRÉSENTATIONS DES GROUPES LOCALEMENT COMPACTS

Dans ce paragraphe, les espaces vectoriels sont sur le corps $K =\mathbf{R}$ ou $\mathbf{C}$. On note G un groupe localement compact muni d’une mesure de Haar à gauche $\mu$. On notera $\mathscr{L}^p(G) =\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ et $L^p(G) = L^p_{\mathbf{C}}(G, \mu)$ pour tout $p\in [1,+\infty ]$.

### 1. Continuité de certaines représentations

#### Proposition 1 {#ts-v-s2-prop-1 .statement tag=03A4}

Soit H un groupe localement compact. Soit $\varrho_1$ (resp. $\varrho_2)$ une représentation continue de G (resp. de H) dans un K-espace vectoriel localement convexe séparé $E_1$ (resp. $E_2)$. Notons F l’espace $\mathscr{L}(E_1; E_2)$ muni de la topologie de la convergence compacte. La représentation $\varrho$ de $G\times H$ dans F définie par $\varrho (g, h)u=\varrho_2(h)\circ u\circ \varrho_1(g^{-1})$ pour $(g, h)\in G\times H$ est continue.

Notons $\mathscr{L}_c(E_1; E_2)$ l’espace $\mathscr{L}(E_1; E_2)$ muni de la topologie de la convergence compacte. Soient $\mathfrak{F}_1$ (resp. $\mathfrak{F}_2,\mathfrak{F}_3)$ un filtre dans G convergeant vers $e$ (resp. un filtre dans $\mathscr{L}_c(E_1; E_2)$ convergeant vers 0, un filtre dans H convergeant vers $e)$. Comme G et H sont localement compacts, il existe des éléments $C\in \mathfrak{F}_1$ et $D\in \mathfrak{F}_3$ qui sont relativement compacts. L’ensemble $\varrho_1(C^{-1})$ est équicontinu dans $\mathscr{L}(E_1) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2, a$'))$. D’après la prop. 9 de EVT, III, p. 33 et la prop. 4 de EVT, III, p. 31, l’application définie par $(u, v)\mapsto u\circ v$ de $\mathscr{L}_c(E_1; E_2)\times \varrho_1(C^{-1})$ dans $\mathscr{L}_c(E_1; E_2)$ est continue. La base de filtre $\mathfrak{F}_2\circ \varrho_1(\mathfrak{F}^{-1}_1)$ converge donc vers 0 dans $\mathscr{L}_c(E_1; E_2)$. L’ensemble $\varrho_2(D)$ est équicontinu dans $\mathscr{L}(E_2) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2), et pour tout $x\in E_2$, l’ensemble $\varrho_2(D)x\subset E_2$ est relativement compact. Par conséquent, $\varrho_2(D)$ est relativement compact dans $\mathscr{L}(E_2)$ muni de la topologie de la convergence compacte (TG, X, p. 18, cor. 1). L’application définie par $(u, v)\mapsto u\circ v$ de $\overline{\varrho_2(D)}\times \mathscr{L}_c(E_1; E_2)$ dans $\mathscr{L}_c(E_1; E_2)$ est continue d’après la prop. 9 de EVT, III, p. 33 et la prop. 4 de EVT, III, p. 31. Donc la base de filtre $\varrho (\mathfrak{F}_1\times \mathfrak{F}_3)(\mathfrak{F}_2)$ converge vers 0 dans $\mathscr{L}_c(E_1; E_2)$. Cela entraîne l’assertion.

#### Corollaire {#ts-v-s2-n1-cor-1 .statement tag=03A5}

Soit $\varrho$ une représentation continue de G un K-espace vectoriel localement convexe séparé E. La représentation contragrédiente $\breve{\varrho}$ est continue lorsque $E'$ est muni de la topologie de la convergence compacte.

Cela résulte de la proposition en prenant $H =\{e\},\varrho_1=\varrho$ et $\varrho_2$ la représentation triviale sur K.

#### Remarque {#ts-v-s2-n1-rem-1 .statement tag=03A6}

La représentation contragrédiente n’est pas nécessairement continue lorsque $E'$ est muni de la topologie forte (cf. INT, VIII, p. 191, § 2, exercice 3, d)). On peut montrer qu’elle l’est si l’espace E est semi-réflexif (loc. cit., c)).

### 2. Extension de représentations à des espaces de mesures

Dans ce numéro, on suppose que $K =\mathbf{C}$.

Soit $\varrho$ une représentation linéaire continue de G dans un espace localement convexe séparé quasi-complet E. Notons $\mathscr{M}_c(G)$ l’espace des mesures à support compact sur G muni de la topologie de la convergence compacte ; c’est le dual de l’espace $\mathscr{C}(G)$. Pour toute mesure $\nu \in \mathscr{M}_c$(G), posons

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

C’est un élément de $\mathscr{L}(E)$. En particulier, on a $\varrho (\varepsilon_g) =\varrho (g)$ pour tout $g\in G$.

D’après INT, VIII, p. 136, § 2, n$^o6$, l’application $\nu \mapsto \varrho (\nu )$ est une application linéaire continue de $\mathscr{M}_c(G)$ dans l’espace $\mathscr{L}(E)$ muni de la topologie de la convergence compacte. D’après INT, VIII, p. 145, § 3, n$^o3$, prop. 11, c’est un morphisme d’algèbres unifères.

Soit $x\in E$. L’application de $\mathscr{M}_c(G)$ dans E définie par $\nu \mapsto \varrho (\nu )x$ est continue lorsque $\mathscr{M}_c(G)$ est muni de la topologie de la convergence compacte (INT, VI, p. 27, § 1, n$^o$ 7, prop. 16 et EVT, III, p. 31, prop. 4).

Pour $f\in \mathscr{L}^1(G)$ nulle en dehors d’une partie compacte de G, la mesure $f\cdot \mu$ est à support compact et l’on notera $\varrho^\mu(f)$, ou $\varrho (f)$ lorsqu’aucune ambiguïté n’est possible, l’endomorphisme $\varrho (f\cdot \mu)$ de E. Cet endomorphisme ne dépend que de la classe $\widetilde{f}$ de $f$ dans $L^1$(G), et on le notera aussi $\varrho^\mu(\widetilde{f})$ ou $\varrho (\widetilde{f})$.

De manière analogue, soit $\varrho$ une représentation linéaire continue et bornée de G dans un espace de Banach E. Pour toute mesure bornée $\nu \in \mathscr{M}^1$(G), on pose

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

D’après INT, VIII, loc. cit., l’application $\nu \mapsto \varrho (\nu )$ est un morphisme unifère continu d’algèbres de Banach de l’algèbre $\mathscr{M}^1(G)$ des mesures complexes bornées sur G dans l’algèbre de Banach $\mathscr{L}(E)$.

Soit $\rho$ la fonction $g\mapsto  \|\varrho (g)\|$ sur G ; l’algèbre notée $\mathscr{M}^{\rho}$ dans INT, VIII, p. 145, prop. 11 (dont les éléments sont les mesures $\nu$ telles que $\rho \in \mathscr{L}^1(\nu ))$ coïncide avec l’algèbre de Banach $\mathscr{M}^1(G)$. En effet, posons M = sup $\rho$. On a $M>0$ puisque $\rho (e) = 1$, et $M^{-1}\leqslant \rho \leqslant M$ puisque $\|\varrho (e)\|\leqslant \|\varrho (g)\| \|\varrho (g^{-1})\|$ pour tout $g\in G$; ainsi $\rho \in \mathscr{L}^1(\nu )$ si et seulement si $\nu$ est une mesure bornée.

Si $f\in \mathscr{L}^1$(G), on notera aussi $\varrho^\mu(f)$ ou simplement $\varrho (f)$ l’endomorphisme $\varrho (f\cdot \mu)$, et de même pour la classe $\widetilde{f}$ de $f$ dans $L^1(G)$.

#### Lemme 1 {#ts-v-s2-lem-1 .statement tag=03A7}

Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien E. L’application $\nu \mapsto \varrho (\nu )$ de $\mathscr{M}^1(G)$ dans $\mathscr{L}(E)$ est un morphisme unifère d’algèbres de Banach involutives.

D’après ce qui précède, il suffit de démontrer que le morphisme $\nu \mapsto \varrho (\nu )$ est involutif. Soit $\nu \in \mathscr{M}^1(G)$. La mesure $\nu^*$ est la mesure conjuguée de la mesure $\check{\nu}($I, p. 99, exemple 4). D’après la définition de la mesure conjuguée (INT, III, p. 52, § 1, n$^o5)$, on calcule

$$
\langle x|\varrho (\nu )y\rangle =\int\langle x|\varrho (g)y\rangle d\nu (g)
$$

$$
=\int^G_G\langle \varrho (g^{-1})x|y\rangle d\nu (g) =\int_G\langle \varrho (g)x|y\rangle d\check{\nu}(g)
$$

$$
=\int_G\langle y|\varrho (g)x\rangle d\nu^*(g) =\langle \varrho (\nu^*)x|y\rangle
$$

pour tous $x$ et $y$ dans E, d’où $\varrho (\nu )^*=\varrho (\nu^*)$.

Soit $\varrho$ une représentation linéaire continue (resp. continue et bornée) de G dans un espace localement convexe quasi-complet E (resp. un espace de Banach E). Si F est un sous-espace fermé de E définissant une sous-représentation $\varrho_F$ de $\varrho$, alors pour toute mesure $\nu \in \mathscr{M}_c(G)$ (resp. $\nu \in \mathscr{M}^1(G))$ l’application linéaire $\varrho (\nu )$ laisse stable le sous-espace F et coïncide avec $\varrho_F(\nu )$ sur F.

Réciproquement, soit $F\subset E$ un sous-espace fermé, stable par les applications linéaires $\varrho (f)$ pour toute fonction $f\in \mathscr{K}(G)$. Alors F définit une sous-représentation de $\varrho$ (INT, VIII, p. 139, § 2, n$^o7$, prop. 10).

Rappelons (A, VIII, p. 388) qu’une fonction $f: G\rightarrow \mathbf{C}$ est dite centrale si, pour tous $g$ et $h$ dans G, on a $f(gh) =f(hg)$. Cela revient à dire que $f$ est invariante par conjugaison.

#### Définition 1 {#ts-v-s2-def-1 .statement tag=03A8}

Une mesure bornée $\nu \in \mathscr{M}^1(G)$ est dite centrale si on a $\varepsilon_g*\nu =\nu *\varepsilon_g$ pour tout $g\in G$.

Si G est unimodulaire et $f\in \mathscr{C}(G)$ est $\mu$-intégrable, la mesure $f\cdot \mu$ est centrale si et seulement si $f$ est centrale.

Soit $\varrho$ une représentation continue bornée de G dans un espace de Banach E (resp. une représentation continue de G dans un espace localement convexe séparé quasi-complet E). Pour toute mesure centrale bornée $\nu$ sur G (resp. toute mesure centrale à support compact $\nu$ sur G), l’application linéaire $\varrho (\nu )$ est un G-morphisme de $\varrho$ dans $\varrho$. En effet, pour tout $g\in G$, on a

$$
\varrho (\nu )\varrho (g) =\varrho (\nu *\varepsilon_g) =\varrho (\varepsilon_g*\nu ) =\varrho (g)\varrho (\nu )
$$

### 3. Critère de semi-simplicité

#### Proposition 2 {#ts-v-s2-prop-2 .statement tag=03A9}

Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. Soit $\mathfrak{F}$ une base de filtre sur $\mathscr{M}_c(G)$ convergeant vers la mesure $\varepsilon_e$ pour la topologie de la convergence compacte. On suppose qu’il existe $M\in \mathfrak{F}$ tel que $\varrho (\nu )$ soit un endomorphisme compact de E pour tout $\nu \in M$.

La représentation unitaire $\varrho$ est alors semi-simple et toute représentation unitaire irréductible de G est de multiplicité finie dans $\varrho$.

Démontrons d’abord un lemme.

#### Lemme 2 {#ts-v-s2-lem-2 .statement tag=03AA}

Soit $\varrho_1$ une représentation unitaire non nulle de G isomorphe à une sous-représentation de $\varrho$. Il existe une mesure $\nu \in M$ telle que $\varrho_1(\check{\nu}*\nu )$ soit un endomorphisme compact hermitien non nul de l’espace de $\varrho_1$. En particulier, il existe un nombre réel $\lambda$ non nul tel que le sous-espace propre de $\varrho_1(\check{\nu}*\nu )$ relatif à $\lambda$ n’est pas nul.

On peut supposer que $\varrho_1$ est une sous-représentation de $\varrho$. Soit $E_1$ son espace. Pour toute mesure $\nu \in M$, l’endomorphisme $\varrho_1(\nu )$ est déduit de $\varrho (\nu )$ par passage aux sous-espaces. L’hypothèse et la prop. 3 de III, p. 5 impliquent donc que $\varrho_1(\nu )$ est compact.

Puisque $\mathfrak{F}$ converge vers la mesure $\varepsilon_e$ dans $\mathscr{M}_c(G)$ muni de la topologie de la convergence compacte et que l’espace $E_1$ n’est pas nul, il existe $\nu \in M$ telle que $v=\varrho_1(\nu )$ est un endomorphisme non nul de $E_1$ (cf. n$^o2$ de V, p. 400). L’endomorphisme $u=\varrho_1(\check{\nu}*\nu )$ est égal à $v^*\circ v$ (lemme 1 de V, p. 401) ; il est donc non nul (EVT, V, p. 39, prop. 2), hermitien et compact, puisque $v$ est compact.

Comme $u$ est hermitien et non nul, son spectre n’est pas réduit à zéro (exemple 1 de I, p. 110). Enfin, puisque $u$ est compact, tout $\lambda \in$ Sp($u$)$-\{0\}$ est une valeur propre de $u$ (prop. 2 de III, p. 83).

Démontrons maintenant la proposition.

Nous utiliserons la prop. 7 de V, p. 391 pour établir que $\varrho$ est semi-simple. Soit $\varrho_1$ une sous-représentation non nulle de $\varrho$ et $E_1\subset E$ son espace ; nous devons démontrer que $\varrho_1$ contient une sous-représentation irréductible.

Soit $\nu \in M$ tel que $u=\varrho_1(\check{\nu}*\nu )$ est un endomorphisme compact hermitien non nul de l’espace de $\varrho_1$, et soit $\lambda$ non nul tel que le sous-espace propre F de $u$ relatif à $\lambda$ est non nul (lemme 2). L’espace F est de dimension finie (prop. 5 de III, p. 90). Il existe une sous-représentation $\varrho_2$ de $\varrho_1$ sur un sous-espace $E_2$ de $E_1$ tel que $E_2\cap F$ est non nul et de dimension minimale. Soit $x$ un élément non nul de $E_2\cap F$, et soit $E_3$ la sous-représentation de $\varrho_1$ engendrée par $x$. On a alors $E_3\subset E_2$, d’où $E_3\cap F = E_2\cap F$ par minimalité de la dimension de $E_2\cap F$.

Démontrons que la représentation $E_3$ est irréductible. Soit $E_4\subset E_3$ un sous-espace fermé stable par G. On a $E_2\cap F = (E_4\cap F)\oplus (E^{\circ}_4\cap F)$, où $E^{\circ}_4$ désigne l’orthogonal de $E_4$ dans $E_3$ (en effet, si $y\in E_2\cap F$, soit $y_4\in E_4$ sa projection orthogonale sur $E_4$; puisque $E_4$ et $E^{\circ}_4$ sont stables par $u$, le vecteur $u(y_4)$ est la projection orthogonale de $u(y) =\lambda y$ sur $E_4$, d’où $u(y_4) =\lambda y_4$, ce qui signifie que $y_4\in E_4\cap F$, et l’assertion en résulte). La minimalité de la dimension de $E_2\cap F$ implique alors que, soit $E_4\cap F = E_2\cap F$, soit $E^{\circ}_4\cap F = E_2\cap F$. Dans le premier cas, on a $x\in E_4$, d’où $E_4= E_3$, et dans le second, on a $x\in E^{\circ}_4$, d’où $E^{\circ}_4= E_3$ et $E_4=\{0\}$. La représentation $E_3$ est donc irréductible.

On conclut d’après la prop. 7 de V, p. 391 que la représentation $\varrho$ est semi-simple.

Soit $\pi$ une représentation unitaire irréductible de G dont la multiplicité dans $\varrho$ est non nulle ; soit $E_{\pi}$ son espace. Il existe une mesure $\nu \in M$ et un nombre réel $\lambda$ non nul tels que $u=\pi (\check{\nu}*\nu )$ est un endomorphisme compact hermitien non nul de $E_{\pi}$ et que le sous-espace propre de $u$ relatif à $\lambda$ est non nul (lemme 2). Soit F le sous-espace propre de $v=\varrho (\check{\nu}*\nu )$ relatif à $\lambda$. Pour toute sous-représentation $E_1$ de E isomorphe à $\pi$, l’endomorphisme de $E_1$ déduit de $v$ par passage aux sous-espaces s’identifie à $u$, donc l’intersection de $E_1$ et de F n’est pas nulle. Ainsi, la multiplicité de $\pi$ dans $\varrho$ est inférieure à la dimension de l’espace F, qui est finie (prop. 5 de III, p. 90).

#### Exemple {#ts-v-s2-n3-exa-1 .statement tag=03AB}

On suppose que G est unimodulaire, par exemple que G est un groupe de Lie réel semi-simple. Soit $\Gamma \subset G$ un sous-groupe discret tel que le quotient $X = \Gamma \backslash G$ est compact. Le groupe G agit à droite par multiplication sur X. On note $\beta$ la mesure de comptage sur Γ et on pose $\widetilde{\mu}=\mu/\beta$ (INT, VII, p. 44, § 2, n$^o2$, déf. 1) ; c’est une mesure bornée G-invariante sur X.

Pour tout $f\in \mathscr{L}^2(X,\widetilde{\mu})$ et tout $g\in$ G, on définit la fonction $\varrho (g)f\in \mathscr{L}^2(X,\widetilde{\mu})$ par $\varrho (g)f(x) =f(x\cdot g)$. L’application $\varrho (g)$ est une application linéaire continue, qui induit par passage aux quotients une application unitaire sur $L^2(X,\widetilde{\mu})$, encore notée $\varrho (g)$. L’application $\varrho$ est une représentation unitaire de G dans $L^2(X,\widetilde{\mu})$ (INT, VII, p. 135, § 2, n$^o5$, prop. 8).

Soit $\varphi \in \mathscr{K}(G)$. Pour toutes parties compactes $L_1$ et $L_2$ de G, l’intersection T de Γ et de l’ensemble compact $L_1$Supp($\varphi$ )$L^{-1}_2$ est finie. Pour tout $(g, h)\in L_1\times L_2$, la série $\sum_{\gamma\in\Gamma}\varphi (g^{-1}\gamma h)$ coïncide avec la somme

finie $\sum_{\gamma\in T}\varphi (g^{-1}\gamma h)$. Puisque G est localement compact, la somme de

cette série, notée $k_{\varphi}(g, h)$, est une fonction continue sur $G\times G$.

Soit $g\in G$ et soit $(\gamma , \eta )\in \Gamma \times \Gamma$. On a $k_{\varphi}(\gamma g, \eta h) =k_{\varphi}(g, h)$, donc $k_{\varphi}$ définit par passage au quotient une fonction continue sur $X\times X$, que l’on note $\widetilde{k}_{\varphi}$. On a de plus $\widetilde{k}_{\varphi}\in \mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, puisque l’espace X est supposé compact.

On note $\dot{x}$ l’image dans X d’un élément $x$ de G par la projection canonique. Soit $\varphi \in \mathscr{K}(G)$. Pour $f\in \mathscr{L}^2(X,\widetilde{\mu})$ et $x\in G$, on a

$$
\varrho (\varphi )f( \dot{x}) =\int_G\varphi (g) (\varrho (g)f)( \dot{x})d\mu(g) =\int_G\varphi (g)f( \dot{x}\cdot g)d\mu(g)
$$

$$
=\int_G\varphi (x^{-1}y)f( \dot{y})d\mu(y) =\int_{\Gamma\backslash G}((\sum_{\gamma\in\Gamma}\varphi (x^{-1}\gamma y))f( \dot{y})d\widetilde{\mu}( \dot{y})
$$

(INT, VII, p. 46, § 2, n$^o3$, prop. 5). Comme $\widetilde{k}_{\varphi}$ appartient à l’espace $\mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, il en résulte que l’endomorphisme $\varrho (\varphi )$ de $L^2(X,\widetilde{\mu})$ coïncide avec l’endomorphisme de Hilbert–Schmidt de noyau $\widetilde{k}_{\varphi}$; cet endomorphisme est donc compact (cor. 1 de III, p. 33)

Il existe une suite $(\varphi_n)_{n\in\mathbf{N}}$ de fonctions dans $\mathscr{K}_+(G)$ d’intégrale 1 telle que $\varphi_n\cdot \mu$ converge vers $\varepsilon_e$ dans $\mathscr{M}_c(G)$ muni de la topologie de la convergence compacte (INT, VIII, p. 139, § 2, n$^o7$, cor. 2). La prop. 2 implique par conséquent que la représentation $\varrho$ est semi-simple et que les multiplicités des représentations unitaires irréductibles de G dans $\varrho$ sont finies.

Les représentations unitaires irréductibles de G dont la multiplicité dans $\varrho$ n’est pas nulle sont appelées représentations Γ-automorphes du groupe G.

### 4. Représentations régulières

Soient $p$ un nombre réel $\geqslant 1$ et $\mu'$ une mesure de Haar à droite sur G.

Pour tout $g\in G$ et toute fonction $f\in \mathscr{L}^p(G, \mu)$, on note $\boldsymbol{\gamma }^{(p)}_G(g)f$ la fonction $x\mapsto f(g^{-1}x)$ sur G. L’application $g\mapsto \boldsymbol{\gamma }^{(p)}_G(g)$ est une représentation linéaire continue de G dans $\mathscr{L}^p(G)$. Elle induit par passage aux quotients une représentation linéaire continue isométrique de G dans $L^p(G)$ (INT, VIII, p. 135, § 2, n$^o5$, prop. 8), notée $\boldsymbol{\gamma }^{(p)}_G$.

De même, pour tout $g\in G$ et toute fonction $f\in \mathscr{L}^p(G, \mu')$, on note $\boldsymbol{\delta }^{(p)}_G(g)f$ la fonction $x\mapsto f(xg)$ sur G. L’application $g\mapsto \boldsymbol{\delta }^{(p)}_G(g)$ est une représentation linéaire continue de G dans $\mathscr{L}^p(G, \mu')$. Elle induit par passage aux quotients une représentation linéaire continue isométrique de G dans $L^p(G, \mu') ($cf. INT, VIII, p. 136, § 2, n$^o5)$.

On dit que $\boldsymbol{\gamma }_G^{(p)}$ est la représentation régulière gauche de G dans $\mathscr{L}^p(G)$ ou $L^p(G)$ et que $\boldsymbol{\delta }^{(p)}_G$ est la représentation régulière droite de G dans $\mathscr{L}^p(G, \mu')$ ou $L^p(G, \mu')$.

#### Lemme 3 {#ts-v-s2-lem-3 .statement tag=03AC}

Soit $p$ un nombre réel $\geqslant 1$. La représentation régulière gauche (resp. droite) de G dans $L^p(G, \mu) ($resp. dans $L^p(G, \mu'))$ est fidèle.

Plus précisément, soit $q$ l’exposant conjugué de $p$ et soit $g$ un élément de G tel que $g\not =e$.

a) Il existe une fonction $\varphi \in \mathscr{K}(G)$, positive et non nulle dans $L^q(G, \mu)$, telle que $\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle = 0$;

b) Il existe une fonction $\varphi \in \mathscr{K}(G)$, positive et non nulle dans $L^q(G, \mu')$, telle que $\langle \varphi ,\boldsymbol{\delta }^{(p)}_G(g)\varphi \rangle = 0$.

Considérons le cas de la représentation régulière gauche $\boldsymbol{\gamma }^{(p)}_G$, celui de la représentation régulière droite étant similaire. L’assertion a) implique que $\boldsymbol{\gamma }^{(p)}_G$ est fidèle, car si $g\not =e$ est un élément de G, et si $\varphi$ est comme dans a), on a $\varphi \not =\boldsymbol{\gamma }^{(p)}_G(g)\varphi$ puisque $\langle \varphi , \varphi \rangle =\int_G\varphi^2>0$.

Démontrons donc a). Soit $g\not =e$ dans G. Soit C un voisinage compact symétrique de $e$ tel que $g /\in C^2$ et soit $\varphi \in \mathscr{K}(G)$ une fonction continue positive d’intégrale 1 à support contenu dans C ; la fonction $\varphi$ est non nulle dans $L^p(G, \mu)$. Comme $C\cap g^{-1}C =\emptyset$, on a

$$
\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle =\int_G\varphi (x)\varphi (g^{-1}x)d\mu(x) = 0
$$

Soit $\varrho$ une représentation continue et bornée de G dans un espace de Banach E. Pour tout $f\in L^1(G)$ (resp. $f'\in L^1(G, \mu'))$ et tout $g\in G$, on a

(1) $\varrho (g)\varrho (f\cdot \mu) =\varrho (\varepsilon_g*(f\cdot \mu)) =\varrho (\boldsymbol{\gamma }$[^1]$_G(g)f\cdot \mu)$,

(2) $\varrho (f'\cdot \mu')\varrho (g) =\varrho ((f'\cdot \mu')*\varepsilon_g) =\varrho (\boldsymbol{\delta }$[^1]$_G(g^{-1})f'\cdot \mu')$

(INT, VIII, p. 144, § 3, n$^o2$, formule (5)).

Supposons G unimodulaire, et posons $\mu'=\mu$. La représentation birégulière de G dans $\mathscr{L}^p(G)$ (resp. dans $L^p(G))$ est la représentation $\boldsymbol{\varrho }^{(p)}_G$ de $G\times G$ dans $\mathscr{L}^p(G)$ (resp. dans $L^p(G))$ telle que

$$
\boldsymbol{\varrho }_G^{(p)}(g_1, g_2) =\boldsymbol{\gamma }_G^{(p)}(g_1)\boldsymbol{\delta }_G^{(p)}(g_2) =\boldsymbol{\delta }_G^{(p)}(g_2)\boldsymbol{\gamma }_G^{(p)}(g_1)
$$

C’est une représentation linéaire continue (lemme 1 de V, p. 377). Elle vérifie

$$
(\boldsymbol{\varrho }_G^{(p)}(g_1, g_2)f)(x) =f(g_1^{-1}xg_2)
$$

pour tout $f\in \mathscr{L}^p$(G), tout $(g_1, g_2)\in G\times G$ et tout $x\in G$.

#### Remarque {#ts-v-s2-n4-rem-1 .statement tag=03AD}

La représentation birégulière de G dans $L^p(G, \mu)$ n’est pas nécessairement fidèle ; son noyau est l’image du centre de G par l’application $g\mapsto (g, g)$ (exercice 4 de V, p. 487).

Lorsque $p= 2$, la représentation régulière gauche $\boldsymbol{\gamma }$[^2]$_G$ de G dans l’espace hilbertien complexe $L^2(G, \mu)$ est unitaire, puisqu’elle est isométrique. De même, la représentation régulière droite $\boldsymbol{\delta }_G$[^2] dans $L^2(G, \mu')$ est unitaire.

On notera simplement $\boldsymbol{\gamma }_G=\boldsymbol{\gamma }$[^2]$_G$ et $\boldsymbol{\delta }_G=\boldsymbol{\delta }$[^2]$_G$, et on appellera ces représentations les représentations régulières gauche et droite de G.

Si G est unimodulaire, la représentation birégulière $\boldsymbol{\varrho }$[^2]$_G$ de $G\times G$ dans $L^2(G, \mu)$ est unitaire. On la notera simplement $\boldsymbol{\varrho }_G$.

#### Lemme 4 {#ts-v-s2-lem-4 .statement tag=03AE}

Soit $p$ un nombre réel $\geqslant 1$. Pour $f\in \mathscr{L}^1(G)$, l’application linéaire $\boldsymbol{\gamma }^{(p)}_G(f)$ coïncide avec l’endomorphisme de $L^p(G)$ défini par $\varphi \mapsto f*^\mu\varphi$.

Cela résulte de INT, VIII, p. 157, § 4, n$^o2$, prop. 6, compte tenu de la formule (14) de INT, VIII, p. 165.

#### Remarque {#ts-v-s2-n4-rem-2 .statement tag=03AF}

Rappelons que, pour toute fonction $f$ sur G, on définit la fonction $\check{f}$ sur G par $\check{f}(g) =f(g^{-1})$ pour tout $g\in G$ (INT, VII, p. 12, § 1, n$^o1$, formule (12)).

On vérifie que si $f\in \mathscr{L}^1$(G), l’application linéaire $u=\boldsymbol{\delta }^{(p)}_G(f)$ vérifie la relation

$$
u(\widecheck{\varphi}) =f*\check{\varphi}
$$

pour tout $\varphi \in L^p(G, \mu')$.

### 5. Fonctions équivariantes

Dans ce numéro, on fixe un sous-groupe fermé H de G. On note $\varpi$ la projection canonique de G dans $G/H$.

En sus de la mesure de Haar $\mu$ sur G, on fixe une mesure de Haar à gauche $\beta$ sur H.

D’après INT, VII, p. 56, § 2, n$^o5$, th. 2, il existe une fonction continue $\kappa : G\rightarrow \mathbf{R}_+^*$ telle que $\kappa (xh) = \Delta_H(h)\Delta_G(h)^{-1}\kappa (x)$ quel que soit $(x, h)\in G\times H$. On fixe une telle fonction $\kappa$. On note $\nu$ la mesure $(\kappa \cdot \mu)/\beta$ sur $G/H$; d’après loc. cit., c’est une mesure positive non nulle quasi-invariante par G. Son support est égal à $G/H$ (INT, VII, p. 10, § 1, n$^o1)$. D’après INT, VII, p. 43, § 2, n$^o2$, prop. 4, la mesure $\nu$ est l’unique mesure sur $G/H$ telle que la mesure $\nu^{\sharp}$ sur G soit égale à $\kappa \cdot \mu$. On munit l’espace $G/H$ de la mesure $\nu$ (de sorte qu’on note, par exemple, $\mathscr{L}^p(G/H) =\mathscr{L}^p(G/H, \nu ))$.

On dira qu’un ensemble $S\subset G$ est négligeable modulo H si $\varpi (S)$ est $\nu$-négligeable. Cette condition ne dépend pas du choix des mesures de Haar sur G et sur H. Elle implique que S est localement $\mu$-négligeable (INT, VII, p. 47, § 2, n$^o3$, prop. 6, a)). On dira qu’une propriété d’un élément de G est vraie presque partout modulo H si l’ensemble des éléments de G pour lesquels cette propriété ne vaut pas est négligeable modulo H.

Soit $\pi$ une représentation unitaire de H dans un espace hilbertien E. On note $\mathscr{F}_{\pi}(G)$ l’espace vectoriel des fonctions $f$ sur G à valeurs dans E telles que $f(xh) =\pi (h)f(x)$ pour tout $(x, h)\in G\times H$. On dit que les éléments de $\mathscr{F}_{\pi}(G)$ sont les fonctions $\pi$-équivariantes sur G.

L’espace $\mathscr{F}_1(G)$ associé à la représentation triviale de G sur $\mathbf{C}$ s’identifie à l’espace $\mathscr{F}(G/H)$ des fonctions à valeurs complexes sur $G/H$ par l’application $f\mapsto f\circ \varpi$ de $\mathscr{F}(G/H)$ dans $\mathscr{F}_1(G)$.

Pour toute fonction $f$ dans $\mathscr{F}_{\pi}$(G), la fonction $\|f\|$ appartient à $\mathscr{F}_1(G)$ puisque $\pi$ est unitaire. Ceci permet d’identifier $\|f\|$ à une fonction sur $G/H$, et on écrira par exemple $\|f(xH)\|$ pour la valeur de cette fonction en un élément $xH$ de $G/H$.

Une fonction $f$ de $\mathscr{F}_{\pi}(G)$ sera dite nulle en dehors d’un compact modulo H si $\|f\|$ est nulle en dehors d’une partie compacte de $G/H$. Il revient au même de dire qu’il existe une partie compacte K de G telle que $f$ est nulle en dehors de $K\cdot H$ (TG, III, p. 33, prop. 10).

On note $\mathscr{K}_{\pi}(G)$ l’espace des fonctions continues sur G appartenant à $\mathscr{F}_{\pi}(G)$ qui sont à support compact modulo H.

Un espace analogue à $\mathscr{K}_{\pi}(G)$ a été défini dans INT, VII, p. 39, §2, n$^o1$, lorsque $\pi$ est un homomorphisme continu de H dans $\mathbf{R}^*_+$.

Soit $p\in [1,+\infty [$. Pour tout $f\in \mathscr{F}_{\pi}$(G), on note

$$
N_p(f) =(\int_{G/H}^*\|f\|^pd\nu )^{1/p}
$$

C’est un nombre réel ou $+\infty$. On note $\mathscr{F}_{\pi}^p(G, \nu )$, ou simplement $\mathscr{F}_{\pi}^p$(G), le sous-espace des fonctions $f\in \mathscr{F}_{\pi}(G)$ telles que $N_p(f)$ est fini. L’espace $\mathscr{F}_{\pi}^p(G)$ muni de l’application $N_p$ est un espace semi-normé.

L’espace $\mathscr{K}_{\pi}(G)$ est contenu dans $\mathscr{F}_{\pi}^p(G)$. Son adhérence dans $\mathscr{F}_{\pi}^p(G)$ est notée $\mathscr{L}_{\pi}^p(G, \nu )$, ou simplement $\mathscr{L}_{\pi}^p(G)$; on dit que c’est l’espace des fonctions $\pi$-équivariantes sur G de puissance $p^e$ intégrable modulo H.

Les assertions de la proposition suivante sont, lorsque $\pi$ est la représentation triviale de dimension 1, conséquences de INT, IV, p. 128, § 3, n$^o3$, prop. 6 et p. 131, §3, n$^o4$, th. 3.

#### Proposition 3 {#ts-v-s2-prop-3 .statement tag=03AG}

a) Soit $(f_n)_{n\in\mathbf{N}}$ une suite dans $\mathscr{F}_{\pi}^p(G)$ telle que la série

$$
\sum_{n=0}^{+\infty}N_p(f_n)
$$

converge. Alors la série de terme général $f_n(g)$ est absolument convergente pour $g$ en dehors d’un ensemble T qui est négligeable modulo H. Soit $f$ la fonction sur G à valeurs dans E qui est égale à la somme de cette série sur G - T et égale à 0 sur T. On a alors $f\in \mathscr{F}_{\pi}^p(G)$ et la série de terme général $f_n$ converge vers $f$ dans l’espace $\mathscr{F}_{\pi}^p(G)$;

b) Soit $(f_n)$ une suite convergeant dans $\mathscr{L}_{\pi}^p(G)$ vers une fonction $f$. Il existe une suite $(f_{n_k})$ extraite de $(f_n)$ telle que $f_{n_k}(g)$ converge vers $f(g)$ pour tout $g$ en dehors d’un ensemble négligeable modulo H ;

c) Les espaces semi-normés $\mathscr{F}_{\pi}^p(G)$ et $\mathscr{L}_{\pi}^p(G)$ sont complets.

Dans l’assertion a), dire que la série de terme général $f_n$ converge vers $f$ dans l’espace $\mathscr{F}_{\pi}^p(G)$ signifie que la suite des sommes partielles $f_0+\cdots +f_n$ converge vers $f$ dans $\mathscr{F}_{\pi}^p(G)$. On dit alors aussi que $f$ est une somme de cette série.

Démontrons a). D’après la prop. 6 de INT, IV, p. 128, § 3, n$^o3$, il existe un ensemble $\nu$-négligeable $S\subset G/H$ tel que la série de terme général $\|f_n(gH)\|$ converge absolument pour $gH\in /S$. De plus, la fonction $h$ qui est égale à la somme de cette série pour $gH\in /S$ et qui est nulle pour $gH\in S$ vérifie $N_p(h)<+\infty$.

L’ensemble $T =\overset{-1}{\varpi}(S)$ est négligeable modulo H. Pour tout $g /\in T$, la série de terme général $f_n(g)$ est absolument convergente dans E. Définissons $f(g) =\sum f_n(g)$ pour $g /\in T$ et $f(g) = 0$ sinon. On a $f\in$ $\mathscr{F}_{\pi}(G)$. Notons que $\|f(gH)\|\leqslant h(gH)$ pour tout $g\in G$, d’où $N_p(f)\leqslant$ $N_p(h)<+\infty$. On a donc $f\in \mathscr{F}_{\pi}^p(G)$. De manière similaire, il vient

$$
N_p(f-\sum_{n=0}^kf_n)\leqslant \sum_{n=k+1}^{+\infty}N_p(f_n)
$$

pour tout $k\in \mathbf{N}$, donc la série $\sum f_n$ converge vers $f$ dans $\mathscr{F}_{\pi}^p(G)$. L’assertion a) est démontrée.

Démontrons b). La suite $(\|f_n-f\|)_{n\in\mathbf{N}}$ converge vers 0 dans l’espace $\mathscr{L}^p(G/H)$. D’après INT, IV, p. 131, § 4, n$^o3$, th. 3, il existe une suite extraite $(\|f_{n_k}-f\|)_{k\in\mathbf{N}}$ qui converge $\nu$-presque partout vers 0. La suite $(f_{n_k}(g))_{k\in\mathbf{N}}$ converge alors vers $f(g)$ pour tout $g$ en dehors d’un ensemble négligeable modulo H.

Démontrons finalement c). Soit $(f_n)_{n\in\mathbf{N}}$ une suite de Cauchy dans $\mathscr{F}_{\pi}^p(G)$. Il existe une suite strictement croissante d’entiers $(n_k)_{k\in\mathbf{N}}$ telle que $N_p(f_{n_{k+1}}-f_{n_k})\leqslant 2^{-k}$ pour tout $k\in \mathbf{N}$. Pour tout $k\in \mathbf{N}$, posons $h_k$ = $f_{n_{k+1}}-f_{n_k}\in \mathscr{F}_{\pi}^p(G)$. D’après a), la série de terme général $h_k$ converge dans $\mathscr{F}_{\pi}^p(G)$; notons $h$ sa somme. Pour tout $\ell \in \mathbf{N}$, il vient

$$
f_{n_0}+\sum_{k=0}^{\ell}h_k=f_{n_{\ell+1}}
$$

donc $f_{n_0}+h$ est valeur d’adhérence de la suite $(f_n)$. Celle-ci est donc convergente (TG, II, p. 14, cor. 2 de la prop. 5). Ainsi l’espace $\mathscr{F}_{\pi}^p(G)$ est complet ; comme l’espace $\mathscr{L}_{\pi}^p(G)$ est fermé dans $\mathscr{F}_{\pi}^p$(G), il est également complet.

#### Corollaire {#ts-v-s2-n5-cor-1 .statement tag=03AH}

Soit $(f_n)_{n\in\mathbf{N}}$ une suite de Cauchy dans $\mathscr{L}_{\pi}^p(G)$ et soit $f\in \mathscr{F}_{\pi}(G)$ tels que $f_n(g)$ converge vers $f(g)$ presque partout modulo H. Alors $f\in \mathscr{L}_{\pi}^p(G)$ et $(f_n)_{n\in\mathbf{N}}$ converge vers $f$ dans $\mathscr{L}_{\pi}^p(G)$.

En effet, la fonction $f$ coïncide presque partout modulo H avec la limite de la suite $(f_n)$ dans $\mathscr{L}_{\pi}^p(G)$.

On note $L^p_{\pi}(G)$ l’espace vectoriel topologique séparé normé associé à l’espace semi-normé $\mathscr{L}_{\pi}^p(G)$; c’est un espace de Banach.

Soit $f$ une fonction sur G à valeurs dans E. On note $S_f$ l’ensemble des $x\in G$ tels que la fonction $h\mapsto f(xh)$ sur H n’appartient pas à $\mathscr{L}_E^1(H)$. On a $S_f\cdot h= S_f$ pour tout $h\in H$.

Soit $x\in$ G - $S_f$. Comme $\pi$ est une représentation unitaire, la fonction $h\mapsto \pi (h)^*f(xh)$ est mesurable (comme composition de l’application $h\mapsto (h, f(xh))$ de H dans $H\times E$ qui est alors mesurable et de l’application continue $(g, x)\mapsto \pi (g)^*x$ de $H\times E$ dans E, cf. INT, IV, p. 174, § 5, n$^o3$, th. 1), et elle est intégrable sur H.

On définit une fonction $f^{\pi}$ sur G en posant

$$
f^{\pi}(x) =\int_H\pi (h)^*f(xh)d\beta (h) \tag{3}
$$

pour $x\in G$ - $S_f$ et $f^{\pi}(x) = 0$ si $x\in S_f$.

#### Proposition 4 {#ts-v-s2-prop-4 .statement tag=03AI}

Soit $f\in \mathscr{L}_E^1(G)$.

a) L’ensemble $S_f$ est négligeable modulo H et $f^{\pi}\in \mathscr{F}_{\pi}(G)$;

b) Soit C une partie compacte de G. Si $f$ est continue et à support contenu dans C, alors $S_f$ est vide, la fonction $f^{\pi}$ appartient à $\mathscr{K}_{\pi}(G)$ et son support est contenu dans $C\cdot H$.

La première partie de a) résulte de INT, VII, p. 57, § 2, n$^o5$, c). Soit $w\in H$. Si $x\in G$ - $S_f$, alors $xw\in G$ - $S_f$ et

$$
f^{\pi}(xw) =\int_H\pi (h)^*f(xwh)d\beta (h)
$$

$$
=\int_H\pi (w^{-1}y)^*f(xy)d\beta (y) =\pi (w)f^{\pi}(x)
$$

tandis que si $x\in S_f$, alors $f^{\pi}(xw) = 0 =\pi (w)^*f^{\pi}(x)$. La fonction $f^{\pi}$ appartient donc à $\mathscr{F}_{\pi}(G)$.

Supposons maintenant que $f$ est continue et à support contenu dans C. Pour tout $x\in G$, l’application $h\mapsto f(xh)$ appartient alors à $\mathscr{K}$ (H), donc est intégrable, ce qui démontre que $S_f=\emptyset$.

Démontrons que $f^{\pi}$ est continue. Soit $x\in G$. Soit U un voisinage ouvert relativement compact de $x$ dans G.

Pour tout $y\in U$, on a

$$
\|f^{\pi}(y)-f^{\pi}(x)\|\leqslant \int_H\|f(yh)-f(xh)\|d\beta (h)
$$

$$
=\int\|f(yh)-f(xh)\|d\beta (h)
$$

$H\cap (y^{-1}C\cup x^{-1}C)$

$\leqslant \beta (H\cap U^{-1}C)$ sup$_{h\in U^{-1}C}\|f(yh)-f(xh)\|$,

et la continuité de $f^{\pi}$ résulte alors de la continuité uniforme de $f$ sur G.

Enfin, si $x\in G$ vérifie $f^{\pi}(x)\not = 0$, il existe $h\in H$ tel que $f(xh)\not = 0$; ainsi $xh$ appartient à C et $x$ appartient à $C\cdot H$. Comme $C\cdot H$ est fermé dans G, on en conclut que le support de $f^{\pi}$ est inclus dans $C\cdot H$.

Soit C une partie compacte de G. Soit $u\in \mathscr{K}_+(G)$ une fonction telle que $u(x)>0$ pour tout $x\in C$. Soit $v$ la fonction sur G définie par

$$
v(x) =\int_Hu(xh)d\beta (h) \tag{4}
$$

pour tout $x\in G$; avec les notations précédentes, on a $v=u^1$, correspondant à la représentation triviale de dimension 1 de H. La fonction $v$ est continue et positive ; elle appartient à $\mathscr{F}_1$(G), son support est contenu dans Supp($u$)$\cdot H$ et on a

(5) $x$inf$_{\in C\cdot H}v(x)>0$

(INT, VII, p. 39–40, § 2, n$^o1$, prop. 1 et lemme 1, a)).

#### Lemme 5 {#ts-v-s2-lem-5 .statement tag=03AJ}

Soit $f\in \mathscr{F}_{\pi}(G)$ une fonction $\mu$-mesurable nulle en dehors de $C\cdot H$ telle que la fonction $\|f\|$ est $\nu$-intégrable sur $G/H$. Soit $s$ la fonction sur G à valeurs dans E telle que

$v(x)^{-1}f(x)$ si $x\in C\cdot H$

$$
s(x) =
$$

0 si $x\in G$ - $C\cdot H$.

a) La fonction $s$ est $\mu$-mesurable ; elle appartient à $\mathscr{F}_{\pi}(G)$ et est nulle en dehors de $C\cdot H$;

b) La fonction $us$ appartient à $\mathscr{L}^1(G)$ et $(us)^{\pi}=f$ presque partout modulo H.

La fonction $s$ est nulle en dehors de $C\cdot H$ par définition ; elle est $\mu$-mesurable puisque la fonction $f$ est $\mu$-mesurable et que $v(x)>0$ pour tout $x\in C\cdot H$ (INT, IV, p. 193, § 5, n$^o10$, prop. 16). On a $s\in \mathscr{F}_{\pi}(G)$ parce que $v\in \mathscr{F}_1(G)$.

La fonction $f$ est localement $\mu$-intégrable, puisque $\|f\|$ est une fonction $\nu$-intégrable (INT, VII, p. 47, § 2, n$^o3$, prop. 6, c), en notant que la mesure $\nu^{\sharp}=\kappa \cdot \mu$ est équivalente à $\mu)$, donc la fonction $s$ l’est également d’après la formule (5). La fonction $us$ est mesurable et nulle en dehors d’une partie compacte de G ; puisque $u$ est bornée, il en résulte que $us$ est $\mu$-intégrable.

Pour tout $x\in G$ - $S_{us}$, on a

$$
(us)^{\pi}(x) =\int_H\pi (h)^*(u(xh)s(xh))d\beta (h)
$$

$$
=\int_Hu(xh)s(x)d\beta (h) =v(x)s(x)
$$

puisque $s(xh) =\pi (h)s(x)$; la dernière assertion en résulte d’après la prop. 4, a).

Lorsque $H =\{e\}$ et $\pi$ est de dimension 1, la proposition suivante n’est autre que INT, IV, p. 184, § 5, n$^o6$, th. 5.

#### Proposition 5 {#ts-v-s2-prop-5 .statement tag=03AK}

Soit $p\in [1,+\infty [$. L’espace $\mathscr{L}_{\pi}^p(G)$ est l’espace des fonctions $f\in \mathscr{F}_{\pi}(G)$ telles que $f$ est $\mu$-mesurable et que la fonction $\|f\|$ appartient à $\mathscr{L}^p(G/H)$.

Soit $f\in \mathscr{L}_{\pi}^p(G)$. C’est la limite dans $\mathscr{L}_{\pi}^p(G)$ d’une suite d’éléments de $\mathscr{K}_{\pi}(G)$. D’après la prop. 3, b) et le théorème d’Egoroff (INT, IV, p. 175, § 5, n$^o4$, th. 2), la fonction $f$ est donc $\mu$-mesurable ; par conséquent, la fonction $\|f\|$ sur $G/H$ est $\nu$-mesurable (INT, VII, p. 47, § 2, n$^o3$, prop. 6, b)). Comme $N_p(f)$ est fini, la fonction $\|f\|$ appartient à $\mathscr{L}^p(G/H)$ (INT, IV, p. 184, § 5, n$^o6$, th. 5).

Démontrons l’assertion réciproque. Soit $f$ une fonction $\mu$-mesurable appartenant à $\mathscr{F}_{\pi}(G)$ telle que $\|f\| \in \mathscr{L}^p(G/H)$. Soit $\varepsilon  >0$. Démontrons qu’il existe $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ telle que

$$
N_p(f-\widetilde{f})^p=\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

ce qui conclura la démonstration.

Supposons d’abord qu’il existe une partie compacte C de G telle que $f$ est nulle en dehors de $C\cdot H$. Soit $u\in \mathscr{K}_+(G)$ une fonction telle que $u(x)>0$ pour tout $x\in C$ et définissons $v=u^1$ comme ci-dessus. Notons $\varphi$ la fonction caractéristique du support de $u$.

Soit $q$ l’exposant conjugué de $p$. Si $p= 1$, soit $w$ la fonction constante sur G égale à sup$_{x\in G}u(x)$. Si $p >1$, définissons

$$
w(x)=\left(\int_Hu(xh)^q\,d\beta(h)\right)^{1/q}
$$

pour tout $x\in G$. Dans tous les cas, la fonction $w$ est continue et positive ; elle appartient à $\mathscr{K}_1(G)$ (prop. 4 appliquée à la représentation triviale de dimension 1 et à la fonction $u^q)$ donc elle est bornée sur G. On pose W = sup$_{x\in G}w(x)$.

Soit $s$ la fonction sur G à valeurs dans E définie par le lemme 5 appliqué à $f$. Posons $g=\varphi s$. La fonction $g$ est $\mu$-mesurable, et vérifie $\|g\|\leqslant \|f\|/$ inf$_{x\in C\cdot H}v(x)$. Puisque $g$ est nulle en dehors du support de $u$ et que $\kappa$ est continue, on a $g\in \mathscr{L}_E^p(G, \kappa \cdot \mu)$. Soit $\widetilde{g}$ une fonction dans $\mathscr{K}_E(G)$ telle que

$$
\int^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon_p
$$

$_G$ W

On a $us=ug$, donc $f= (us)^{\pi}= (ug)^{\pi}$ presque partout modulo H (lemme 5, b)). Soit $\widetilde{f}= (u\widetilde{g})^{\pi}$; on a $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ (prop. 4, b)). Pour tout $x\in G$ - $S_{ug}$, on obtient

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|\leqslant \int_H^*u(xh)\|g(xh)-\widetilde{g}(xh)\|d\beta (h)
$$

d’où

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|^p\leqslant w(x)^p\int_H^*\|g(xh)-\widetilde{g}(xh)\|^pd\beta (h)
$$

grâce à l’inégalité de Hölder dans le cas $p >1$. Comme $S_{ug}$ est négligeable modulo H, il vient alors

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant W^p\int_{G/H}^*(\int_H^*\|g(xh)-\widetilde{g}(xh)\|d\beta (h))^pd\nu (xH)
$$

$$
= W^p\int_G^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon
$$

d’après INT, VII, p. 46, § 2, n$^o3$, prop. 5, b), qui est applicable car $g-\widetilde{g}$ est nulle en dehors d’une partie compacte de G. Cela implique la propriété demandée lorsque $f$ est nulle en dehors d’une partie compacte modulo H.

Considérons maintenant le cas général. Comme $\|f\| \in \mathscr{L}^p(G/H)$ par hypothèse, il existe une partie compacte L de $G/H$ telle que

$$
\int^*p\varepsilon
$$

$$
\|f\|d\nu \leqslant
$$

$(G/H)-L$ 2

(cf. INT, IV, p. 152, § 4, n$^o6$, th. 4). Soit $\varphi_L$ la fonction caractéristique de L et posons $f_L= (\varphi_L\circ \varpi )f$. On a

$$
\int^*p\int^*p\varepsilon
$$

$$
\|f-f_L\|d\nu =\|f\|d\nu \leqslant
$$

$G/H(G/H)-L$ 2

La fonction $f_L$ est $\mu$-mesurable et nulle en dehors d’un ensemble compact modulo H. Elle appartient à $\mathscr{L}_{\pi}^p$(G), donc d’après le cas précédent, il existe $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ telle que $N_p(f_L-\widetilde{f})\leqslant (\frac{\varepsilon}{2})^{1/p}$, d’où

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

comme désiré.

Considérons le cas $p= 2$. Pour $f_1$ et $f_2$ dans $\mathscr{F}_{\pi}$(G), la fonction $x\mapsto  \langle f_1(x)|f_2(x)\rangle$ appartient à $\mathscr{F}_1(G)$ puisque la représentation $\pi$ est unitaire, et définit donc par passage au quotient une fonction sur $G/H$, que l’on identifie comme précédemment à $\langle f_1|f_2\rangle$. On a la majoration $|\langle f_1|f_2\rangle |\leqslant \|f_1\|\|f_2\|$ dans $\mathscr{F}(G/H)$.

Si $f_1$ et $f_2$ appartiennent à $\mathscr{L}_{\pi}^2$(G), alors la fonction $\langle f_1|f_2\rangle$ appartient à $\mathscr{L}_1^1(G)$. En particulier, elle est intégrable sur $G/H$. L’application

$$
(f_1, f_2)\mapsto \int_{G/H}\langle f_1|f_2\rangle d\nu
$$

est une forme hermitienne positive sur $\mathscr{L}_{\pi}^2(G)$; la semi-norme associée est la semi-norme $N_2$. En particulier, l’espace $\mathscr{L}_{\pi}^2(G)$ est un espace préhilbertien et $L^2_{\pi}(G)$ est l’espace hilbertien associé à $\mathscr{L}_{\pi}^2(G)$.

### 6. Représentations induites

On garde les notations et conventions du numéro précédent concernant les mesures $\beta$ sur H et $\nu$ sur $G/H$, ainsi que la fonction $\kappa : G\rightarrow \mathbf{R}^*_+$.

Il existe une fonction continue $\eta$ de $G\times G/H$ dans $\mathbf{R}_+^*$ telle que

$$
\eta (x, yH) =\frac{\kappa(xy)}{\kappa(x)}
$$

pour tout $(x, y)\in G\times G$, et $\boldsymbol{\gamma }_{G/H}(x)\nu = (y\mapsto \eta (x^{-1}, y))\cdot \nu$ pour $x\in G$ (INT, VII, p. 56, § 2, n$^o5$, th. 2, c)).

Soit $p\in [1,+\infty [$ et soit $\pi$ une représentation unitaire de H dans un espace hilbertien complexe E.

#### Lemme 6 {#ts-v-s2-lem-6 .statement tag=03AL}

Soit $f\in \mathscr{K}_{\overline{\pi}}(G)$. Pour tout $g\in G$, la fonction

$$
\widetilde{f}:x\mapsto \eta (g^{-1}, xH)^{1/p}f(g^{-1}x)
$$

de G dans E appartient à $\mathscr{K}_{\overline{\pi}}(G)$ et vérifie $N_p(\widetilde{f}) = N_p(f)$.

On vérifie sans peine que $\widetilde{f}\in \mathscr{K}_{\overline{\pi}}(G)$. Comme

$$
N_p(\widetilde{f})^p=\int_{G/H}^*\|\widetilde{f}\|^pd\nu =\int_{G/H}^*\gamma_{G/H}(g)(\|f\|^p)(y)\eta (g^{-1}, y)d\nu (y)
$$

et que $(y\mapsto \eta (g^{-1}, y))\cdot \nu =\boldsymbol{\gamma }_{G/H}(g)\nu$, on obtient $N_p(\widetilde{f}) = N_p(f)$.

Il résulte de ce lemme qu’il existe une représentation continue et isométrique $\widetilde{\pi}$ de G dans $L^p_{\overline{\pi}}(G)$ telle que pour $f\in \mathscr{K}_{\pi}(G)$ et $g\in G$, l’élément $\widetilde{\pi}(g)f$ soit la classe de la fonction $\widetilde{f}$ définie ci-dessus. Si $p= 2$, alors cette représentation est unitaire.

#### Définition 2 {#ts-v-s2-def-2 .statement tag=03AM}

On dit que la représentation unitaire de G dans l’espace $L^2_{\overline{\pi}}(G)$ ainsi définie est la représentation unitaire de G induite par la représentation $\pi$ de H relativement à $\kappa$. On la note Ind$^G_H(\pi , \kappa )$, ou simplement Ind$^G_H(\pi )$.

#### Remarque 1 {#ts-v-s2-n6-rem-1 .statement tag=03AN}

Soit $\varrho$ une représentation unitaire de H dans un espace hilbertien complexe F et soit $u:\pi \rightarrow \varrho$ un H-morphisme. Pour toute fonction $f\in \mathscr{K}_{\overline{\pi}}$(G), notons $v(f)$ la fonction $g\mapsto u(f(g))$ de G dans F ; elle appartient à $\mathscr{K}_{\overline{\varrho}}(G)$ et vérifie $N_p(v(f))\leqslant \|u\|N_p(f)$. L’application linéaire de $\mathscr{K}_{\overline{\pi}}(G)$ dans $\mathscr{K}_{\overline{\varrho}}(G)$ qui à $f$ associe $v(f)$ s’étend donc en un H-morphisme continu de Ind$^G_H(\pi )$ dans Ind$^G_H(\varrho )$ qui est noté Ind$^G_H(u)$. On a Ind$^G_H(1_{\pi}) = 1_{Ind^G_H(\pi)}$. Soit $\sigma$ une représentation unitaire de H et soit $v:\varrho \rightarrow \sigma$ un H-morphisme ; on a Ind$^G_H(v\circ u) =$ Ind$^G_H(v)\circ$ Ind$^G_H(u)$.

*Autrement dit, la construction qui à $\pi$ associe Ind$^G_H(\pi )$ et à $u$ associe Ind$^G_H(u)$ est un foncteur de la catégorie des représentations unitaires de H dans celle des représentations unitaires de G (cf. CAT, I, § 2, en préparation).*

#### Remarque 2 {#ts-v-s2-n6-rem-2 .statement tag=03AO}

Soit $\kappa ': G\rightarrow \mathbf{R}_+^*$ telle que

$$
\frac{\kappa'(xh)}{\kappa^'(x)}=\frac{\Delta_H(h)}{\Delta_G(h)}=\frac{\kappa(xh)}{\kappa(x)}
$$

pour tout $(x, h)\in G\times H$. Soit $\nu '$ la mesure quasi-invariante $(\kappa '\cdot \mu)/\beta$ sur $G/H$. La fonction $\kappa '\kappa^{-1}$ définit par passage aux quotients une fonction continue $\xi : G/H\rightarrow \mathbf{R}_+^*$ telle que $\nu '=\xi \cdot \nu$. L’endomorphisme $\alpha$ de $\mathscr{K}_{\pi}(G)$ défini par $f\mapsto (\kappa '\kappa^{-1})^{1/p}f$ vérifie

$$
\int_{G/H}^*\|f\|^pd\nu '=\int_{G/H}^*\|\alpha (f)\|^pd\nu
$$

et permet d’identifier les espaces $\mathscr{L}_{\pi}^p(G, \nu ')$ et $\mathscr{L}_{\pi}^p(G, \nu )$, ainsi que les espaces $L^p_{\pi}(G, \nu ')$ et $L^p_{\pi}(G, \nu )$. De plus, $\alpha$ induit un isomorphisme isométrique des représentations Ind$^G_H(\pi , \kappa ')$ et Ind$^G_H(\pi , \kappa )$.

### 7. Cas d’un sous-groupe fermé central

Dans ce numéro, on suppose que le groupe G est unimodulaire.

On considère un sous-groupe fermé Z du centre de G, et on note $dz$ une mesure de Haar sur Z. On munit le groupe quotient $G/Z$ de la mesure de Haar $\nu =\mu/dz$. Soit $\chi$ un caractère unitaire de Z. Le groupe quotient $G/Z$ est unimodulaire d’après INT, VII, p. 61, § 2, n$^o7$, cor. de la prop. 11.

#### Lemme 7 {#ts-v-s2-lem-7 .statement tag=03AP}

On a

$$
N_1(\check{f}) = N_1(f),\langle f_1|f_2\rangle =\langle \check{f}_1|\check{f}_2\rangle \tag{6}
$$

pour tout $f\in \mathscr{F}_{\chi}(G)$ et tous $f_1$ et $f_2$ dans $\mathscr{L}_{\chi}^2(G)$.

Ces formules sont conséquences des définitions.

Pour tout $g\in G$ et tout $f\in \mathscr{F}_{\chi}$(G), les fonctions $x\mapsto f(g^{-1}x)$ et $x\mapsto f(xg)$ appartiennent à $\mathscr{F}_{\chi}(G)$. On les note respectivement $\boldsymbol{\gamma }_{G,\chi}(g)f$ et $\boldsymbol{\delta }_{G,\chi}(g)f$. Les applications $\boldsymbol{\gamma }_{G,\chi}$ et $\boldsymbol{\delta }_{G,\chi}$ sont des représentations linéaires de G dans $\mathscr{F}_{\chi}(G)$. Pour tout $z\in Z$, on a

$$
\boldsymbol{\gamma }_{G,\chi}(gz) =\overline{\chi(z)}\boldsymbol{\gamma }_{G,\chi}(g),\boldsymbol{\delta }_{G,\chi}(gz) =\chi (z)\boldsymbol{\delta }_{G,\chi}(g) \tag{7}
$$

Soient $f\in \mathscr{F}_{\chi}(G)$ et $g\in G$; on a

$$
|\boldsymbol{\gamma }_{G,\chi}(g)f|=\boldsymbol{\gamma }_{G/Z}(gZ)|f|,|\boldsymbol{\delta }_{G,\chi}(g)f|=\boldsymbol{\delta }_{G/Z}(gZ)|f| \tag{8}
$$

où toutes les fonctions apparaissant dans ces égalités sont identifiées à des fonctions sur $G/Z$.

Le sous-espace $\mathscr{K}_{\chi}(G)$ de $\mathscr{F}_{\chi}(G)$ est stable par $\boldsymbol{\gamma }_{G,\chi}$ et $\boldsymbol{\delta }_{G,\chi}$. Soit $p$ un nombre réel $\geqslant 1$. Les formules (8) impliquent que les représentations $\boldsymbol{\gamma }_{G,\chi}$ et $\boldsymbol{\delta }_{G,\chi}$, restreintes à $\mathscr{K}_{\chi}$(G), s’étendent en des représentations linéaires continues et isométriques de G dans $\mathscr{L}_{\chi}^p$(G), qui seront

notées $\boldsymbol{\gamma }^{(p)}_{G,\chi}$ et $\boldsymbol{\delta }^{(p)}_{G,\chi}$. Par passage aux quotients, ces représentations définissent également des représentations isométriques de G dans $L^p_{\chi}$(G), notées de la même manière.

Les représentations $\boldsymbol{\gamma }_G$[^2]$_{,\chi}$ et $\boldsymbol{\delta }_G$[^2]$_{,\chi}$ dans $L_{\chi}^2(G)$ sont unitaires, et seront notées simplement $\boldsymbol{\gamma }_{G,\chi}$ et $\boldsymbol{\delta }_{G,\chi}$, respectivement, lorsqu’aucune confusion avec les représentations dans $\mathscr{F}_{\chi}(G)$ ne sera possible. On note aussi $\boldsymbol{\varrho }_{G,\chi}$ la représentation continue de $G\times G$ dans $\mathscr{L}_{\chi}^2(G)$ ou $L^2_{\chi}(G)$ définie par

$$
\boldsymbol{\varrho }_{G,\chi}(g, h) =\boldsymbol{\gamma }_{G,\chi}(g)\circ \boldsymbol{\delta }_{G,\chi}(h) =\boldsymbol{\delta }_{G,\chi}(h)\circ \boldsymbol{\gamma }_{G,\chi}(g)
$$

pour tout $(g, h)\in G\times G ($cf. lemme 1 de V, p. 377).

La représentation $\boldsymbol{\gamma }_{G,\chi}$ sur $L^2_{\chi}(G)$ n’est autre que la représentation induite Ind$^G_Z(\overline{\chi})$.

Lorsque $Z =\{e\}$, le lemme suivant résulte de INT, VIII, p. 166, § 4, n$^o5$, prop. 12, puisque G est unimodulaire.

#### Lemme 8 {#ts-v-s2-lem-8 .statement tag=03AQ}

Soient $f_1\in \mathscr{K}_{\chi}(G)$ et $f_2\in \mathscr{L}_{\chi}^2(G)$.

a) La fonction $f$ sur G définie par $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ pour tout $g\in G$ appartient à $\mathscr{L}_{\overline{\chi}}^2(G)$ et vérifie $N_2(f)\leqslant N_1(f_1)N_2(f_2)$;

b) La fonction $f$ sur G définie par $f(g) =\langle f_1|\boldsymbol{\delta }_{G,\chi}(g)f_2\rangle$ pour tout $g\in G$ appartient à $\mathscr{L}_{\chi}^2(G)$ et vérifie $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Démontrons a), la preuve de l’assertion b) étant similaire. La fonction $f$ est continue, donc $\mu$-mesurable. Pour tout $z\in Z$ et tout $g\in G$, on a

$$
f(gz) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(gz)f_2\rangle =\overline{\chi(z)}\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

(formule (7), p. 417), donc $f\in \mathscr{F}_{\overline{\chi}}(G)$. La prop. 5 de V, p. 413 implique qu’il suffit maintenant de démontrer que $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Supposons d’abord que $f_2$ appartient à $\mathscr{K}_{\chi}(G)$. Pour tout $g\in G$, on a par définition

$$
f(g) =\int_{G/Z}\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2d\nu
$$

où la fonction $\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2$ est identifiée à une fonction sur $G/Z$.

Définissons une fonction $f_3$ sur G en posant $f_3(g) = 0$ si $f_1(g) = 0$ et $f_3(g) =f_1(g)|f_1(g)|^{-1/2}$ sinon. La fonction $f_3$ appartient à $\mathscr{F}_{\chi}(G)$ et vérifie $f_1=|f_1|^{1/2}f_3$; elle est $\mu$-mesurable et nulle en dehors d’un compact modulo Z, puisque $f_1$ l’est. Comme $|f_1|^{1/2}\in \mathscr{K}_1$(G), il vient

$$
\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2=|f_1|^{1/2}\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2
$$

$$
|\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2|=|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|
$$

pour tout $g\in G$.

Soit $g\in G$. D’après l’inégalité de Cauchy–Schwarz, on a

$$
|f(g)|^2\leqslant (\int_{G/Z}|f_1|^{1/2}|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|d\nu )^2
$$

$$
\leqslant (\int_{G/Z}|f_1|d\nu )(\int_{G/Z}|f_3|^2|\boldsymbol{\gamma }_{G,\chi}(g)f_2|^2d\nu )
$$

Comme on a $|f_3|^2=|f_1|$ dans $\mathscr{K}(G/Z)$, on en déduit en intégrant sur $G/Z$ que

$$
\int_{G/Z}|f(g)|^2d\nu (g)\leqslant N_1(f_1)\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

La fonction sur $G/Z\times G/Z$ déduite de la fonction

$$
(g, x)\mapsto  |f_1(x)| |f_2(g^{-1}x)|^2
$$

par passage aux quotients est $(\nu \otimes \nu$)-mesurable et à support compact, donc elle est $(\nu \otimes \nu$)-modérée (INT, V, p. 4, § 5, n$^o2$, déf. 2). D’après la prop. 7 de INT, V, p. 93, § 8, n$^o3$, il vient

$$
\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

$$
=\int_{G/Z}|f_1(x)|(\int_{G/Z}|f_2(g^{-1}x)|^2d\nu (g))d\nu (x) = N_1(f_1)N_2(f_2)^2
$$

Par conséquent, on a $N_2(f)^2\leqslant N_1(f_1)^2N_2(f_2)^2$, ce qui établit la propriété demandée dans ce cas.

Considérons le cas général. Notons $u$ l’application linéaire de $\mathscr{K}_{\chi}(G)$ dans $\mathscr{L}_{\overline{\chi}}^2(G)$ qui à $f_2$ associe $f$. Soit $f_2\in \mathscr{L}_{\chi}^2(G)$ et soit $(f_{2,n})_{n\in\mathbf{N}}$ une suite dans $\mathscr{K}_{\chi}(G)$ qui converge vers $f_2$ dans $\mathscr{L}_{\chi}^2(G)$. Soit $f_n=u(f_{2,n})$; la suite $(f_n)_{n\in\mathbf{N}}$ est de Cauchy dans $\mathscr{L}_{\overline{\chi}}^2(G)$ puisque le cas précédent implique que $N_2(f_n-f_m)\leqslant N_1(f_1)N_2(f_{2,n}-f_{2,m})$ pour tous $n$ et $m$ dans $\mathbf{N}$. Soit $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ telle que $(f_n)$ converge vers $f$ (prop. 3, c) de V, p. 409). Comme $N_2(f_n)\leqslant N_1(f_1)N_2(f_{2,n})$ pour tout $n\in \mathbf{N}$, il vient $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Il existe une suite extraite $(f_{n_k})_{k\in\mathbf{N}}$ telle que $f_{n_k}(g)$ converge vers $f(g)$ pour tout $g\in G$ en dehors d’une partie de G négligeable modulo Z (loc. cit., b)). Mais par ailleurs, pour tout $g\in G$, on a

$$
f_{n_k}(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_{2,n_k}\rangle  \rightarrow  \langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

Par conséquent, on a $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ pour tout $g$ en dehors d’une partie de G négligeable modulo Z. Puisque $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ et que $N_2(f)\leqslant N_1(f_1)N_2(f_2)$, le lemme est démontré.

### 8. Représentations de carré intégrable

Dans ce numéro, les espaces hilbertiens considérés sont complexes. On suppose que G est unimodulaire et on note C son centre. Pour tout sous-groupe fermé Z de C, on note $\beta_Z$ une mesure de Haar sur Z, et on munit $G/Z$ de la mesure de Haar $\nu_Z=\mu/\beta_Z$ (INT, VII, p. 44, § 2, n$^o2$, déf. 1).

Soient $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E et $\chi \in \widehat{C}$ son caractère central (déf. 6 de V, p. 390). Pour tous $x$ et $y$ dans E, on note $f_{x,y}$ le coefficient matriciel $g\mapsto  \langle x|\pi (g)y\rangle$; c’est une fonction continue sur G à valeurs complexes.

Soient $x$ et $y$ dans E. Pour $z\in C$ et $g\in G$, on a

$$
f_{x,y}(zg) =\langle x|\pi (zg)y\rangle =\langle x|\chi (z)\pi (g)y\rangle =\chi (z)f_{x,y}(g) \tag{9}
$$

donc $f_{x,y}$ appartient à l’espace $\mathscr{F}_{\chi}(G) ($V, p. 408). De plus, pour tout $(g_1, h_1)\in G\times G$ et tout $g\in G$, on a

$$
f_{\pi(g_1)x,\pi(h_1)y}(g) =\langle \pi (g_1)x|\pi (g)\pi (h_1)y\rangle =f_{x,y}(g_1^{-1}gh_1) \tag{10}
$$

La relation (9) justifie la définition qui suit.

#### Définition 3 {#ts-v-s2-def-3 .statement tag=03AR}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. On dit que $\pi$ est de carré intégrable modulo le centre si la fonction sur $G/C$ déduite de la fonction $|f_{x,y}|$ par passage au quotient appartient à $\mathscr{L}^2(G/C)$ pour tout $(x, y)\in E\times E$.

Cette condition ne dépend pas du choix d’une mesure de Haar sur $G/C$.

Si les coefficients matriciels de $\pi$ appartiennent à $\mathscr{L}^2$(G), on dit que $\pi$ est de carré intégrable ; l’existence d’une représentation unitaire irréductible de G de carré intégrable implique que le centre de G est compact (exercice 5 de V, p. 487).

Il existe des groupes G qui n’admettent aucune représentation de carré intégrable, même modulo le centre (cf. exercice 32 de V, p. 516).

#### Proposition 6 {#ts-v-s2-prop-6 .statement tag=03AS}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. Soit $\chi$ le caractère central de $\pi$. Alors $\pi$ est de carré intégrable modulo le centre si et seulement s’il existe des éléments non nuls $x_0$ et $y_0$ de E tels que la fonction sur $G/C$ déduite de $|f_{x_0,y_0}|$ par passage au quotient appartient à $\mathscr{L}^2(G/C)$.

Supposons qu’il existe des éléments $x_0$ et $y_0$ non nuls de E tels que $|f_{x_0,y_0}| \in \mathscr{L}^2(G/C)$. Il suffit de démontrer que $\pi$ est alors de carré intégrable modulo le centre.

Soit F l’ensemble des éléments $x\in E$ tels que $|f_{x,y_0}|$ appartient à $\mathscr{L}^2(G/C)$. C’est un sous-espace vectoriel de E ; il contient $x_0$, donc n’est pas nul. La relation (10) ci-dessus implique que F est stable par $\pi$; comme la représentation $\pi$ est irréductible, l’espace F est donc dense dans E.

Soit $x\in F$. Puisque $f_{x,y_0}$ appartient à $\mathscr{F}_{\chi}(G)$ et est $\mu$-mesurable, et que $|f_{x,y_0}| \in \mathscr{L}^2(G/C)$, on a $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ (prop. 5 de V, p. 413 appliquée à Z = C). Notons $u$ l’opérateur partiel de E dans $L^2_{\chi}(G)$ dont le domaine est F et qui associe à $x\in F$ la classe de $f_{x,y_0}$ dans $L^2_{\chi}(G)$.

Démontrons que l’opérateur partiel $u$ est fermé. Soit $(x_n, u(x_n))_{n\in\mathbf{N}}$ une suite d’éléments du graphe de $u$ qui converge dans $E\times L^2_{\chi}(G)$. Soit $x$ la limite de $(x_n)$ et soit $f\in \mathscr{L}_{\chi}^2(G)$ une fonction dont la classe est la limite de la suite $(u(x_n))$.

La fonction $u(x_n)$ est la classe du coefficient matriciel $f_{x_n,y_0}$. Pour tout $g\in G$, on a

$$
f_{x_n,y_0}(g) =\langle x_n|\pi (g)y_0\rangle  \rightarrow  \langle x|\pi (g)y_0\rangle =f_{x,y_0}(g)
$$

quand $n\rightarrow +\infty$. On a donc $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ et $f=f_{x_0,y}$ presque partout modulo C (cor. de la prop. 3 de V, p. 409) ; cela signifie que $u(x)$ est la classe de $f$ dans $L^2_{\chi}(G)$. On a donc démontré que $u$ est fermé.

Le domaine F de $u$ est stable par $\pi$, et la relation (10) démontre que $u$ vérifie $u\circ \pi (g) =\boldsymbol{\gamma }_{G,\chi}(g)\circ u$ pour tout $g\in G$. On a par conséquent aussi l’égalité $u^*\circ \boldsymbol{\gamma }_{G,\chi}(g) =\pi (g)\circ u^*$ pour tout $g\in G$ (lemme 6 de V, p. 381), d’où $(u^*\circ u)\circ \pi (g) =\pi (g)\circ (u^*\circ u)$. Or l’opérateur partiel $u^*\circ u$ est auto-adjoint (prop. 12 de IV, p. 241), et en particulier fermé (prop. 7 de IV, p. 236), donc le cor. 1 de V, p. 387 implique que le domaine de $u^*\circ u$ est égal à E. A fortiori, on a F = E, c’est-à-dire que la fonction $|f_{x,y_0}|$ appartient à $\mathscr{L}^2(G/C)$ pour tout $x\in E$.

Soient $(x, y)\in E\times E$. On a $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$. On démontre mutatis mutandis, en utilisant la représentation $\boldsymbol{\delta }_{G,\chi}$ au lieu de $\boldsymbol{\gamma }_{G,\chi}$, que l’ensemble des $y\in E$ tels que la fonction $|f_{x,y}|$ appartient à $\mathscr{L}^2(G/C)$ est égal à E. La proposition en résulte.

Dans la suite de ce numéro, on fixe un sous-groupe fermé Z de C tel que $C/Z$ est compact.

#### Lemme 9 {#ts-v-s2-lem-9 .statement tag=03AT}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E qui est de carré intégrable modulo le centre. Soit $\chi$ la restriction à Z du caractère central de $\pi$. Pour tous $x$ et $y$ dans E, on a $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$.

La fonction $f_{x,y}$ est continue donc $\mu$-mesurable. On a $f_{x,y}\in \mathscr{F}_{\chi}(G)$ d’après la formule (9), p. 420. De plus, d’après INT, VII, p. 64, § 2, n$^o8$, cor. 1, c), on a $N_2(f_{x,y})<+\infty$ puisque $C/Z$ est compact et que $|f_{x,y}| \in \mathscr{L}^2(G/C)$. L’assertion résulte donc de la proposition 5 de V, p. 413.

#### Proposition 7 {#ts-v-s2-prop-7 .statement tag=03AU}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E qui est de carré intégrable modulo le centre. Soit $\chi$ la restriction à Z du caractère central de $\pi$.

Il existe un nombre réel $c >0$ et un unique $(G\times G)$-morphisme isométrique $w$ de la représentation unitaire $\overline{\pi}\boxtimes \pi$ dans $L^2_{\chi}(G)$ tels que, pour tout $(x, y)\in \overline{E}\times E$, l’élément $w(x\otimes y)$ est la classe dans $L^2_{\chi}(G)$ de la fonction $c^{1/2}f_{x,y}$.

Pour tout $(x, y)\in E\times E$, on a $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$ (lemme 9). Notons $v$ l’unique application linéaire de $E\otimes E$ dans $L^2_{\chi}(G)$ telle que $v(x\otimes y)$ est la classe de $f_{x,y}$ pour tout $(x, y)\in E\times E$.

Nous démontrerons ci-dessous le lemme suivant.

#### Lemme 10 {#ts-v-s2-lem-10 .statement tag=03AV}

Il existe un nombre réel $c >0$ tel que l’application linéaire $w=c^{1/2}v$ est isométrique.

Ce lemme étant supposé valide, remarquons que la formule (10), p. 420, s’écrit

$$
v(\overline{\pi}(g_1)x\otimes \pi (h_1)y) =\boldsymbol{\varrho }_{G,\chi}(g_1, h_1)v(x\otimes y) \tag{11}
$$

pour tout $(g_1, h_1)\in G\times G$ et tout $(x, y)\in \overline{E}\times E$. L’application linéaire isométrique $w$ de $E\otimes E$ dans $L^2_{\chi}(G)$ admet un prolongement continu, encore noté $w$, à $E\widehat{\otimes}_2E$. Par continuité et linéarité, la formule (11) implique que $w$ est un $(G\times$ G)-morphisme de $\overline{\pi}\boxtimes \pi$ dans $L^2_{\chi}$(G), ce qui conclut la démonstration de la proposition.

Démontrons le lemme. Pour tout $x\in E$, on note $u_x$ l’application linéaire $y\mapsto v(x\otimes y) =f_{x,y}$ de E dans $L^2_{\chi}(G)$. On a $u_x\in$ Hom$_G(\pi ,\boldsymbol{\gamma }_{G,\chi})$ (formule (10)). D’après le cor. 5 de V, p. 388, il existe un nombre réel $\lambda_x\geqslant 0$ tel que $\lambda_xu_x$ est isométrique.

Soient $x$ et $y$ dans E. On a

$$
\|f_{x,y}\|^2=\int_{G/Z}\overline{f}_{x,y}f_{x,y}d\nu_Z=\int_{G/Z}\overline{\check{f}}_{x,y}\check{f}_{x,y}d\nu_Z
$$

puisque $G/Z$ est unimodulaire (lemme 7 de V, p. 417). En notant que $\check{f}_{x,y}=f_{y,x}$, on obtient

$$
\lambda_x\|y\|^2=\|f_{x,y}\|^2=\int_{G/Z}f_{y,x}\overline{f}_{y,x}d\nu_Z=\|f_{y,x}\|^2=\lambda_y\|x\|^2
$$

Cela signifie que le nombre réel positif $\lambda_x/\|x\|^2$ est indépendant du choix de l’élément non nul $x$ de E. Il est strictement positif puisque, pour tout $x$ non nul, la fonction $f_{x,x}$ est continue et prend la valeur $\|x\|^2>0$ en $e$, d’où $\|u_x(x)\|=\|f_{x,x}\|>0$. Notons $c^{-1}$ ce nombre réel.

Pour tout $(x, y)\in E\times E$, il vient

$$
\|v(x\otimes y)\|^2=\|f_{x,y}\|^2=\lambda_x\|y\|^2=c^{-1}\|x\|^2\|y\|^2=c^{-1}\|x\otimes y\|^2
$$

En utilisant EVT, V, p. 29, cor. 1, on en déduit que l’application linéaire $w=c^{1/2}v$ de $E\widehat{\otimes}_2E$ dans $L^2_{\chi}(G)$ est isométrique, comme désiré.

#### Corollaire {#ts-v-s2-n8-cor-1 .statement tag=03AW}

Soit $\pi$ une représentation unitaire irréductible de G et soit $\chi$ la restriction à Z de son caractère central. La représentation $\pi$ est de carré intégrable modulo le centre si et seulement si elle est isomorphe à une sous-représentation de la représentation $\boldsymbol{\gamma }_{G,\chi}$ de G dans $L^2_{\overline{\chi}}(G)$ (resp. de la représentation $\boldsymbol{\delta }_{G,\chi}$ de G dans $L^2_{\chi}(G))$.

Démontrons l’assertion concernant $\boldsymbol{\gamma }_{G,\chi}$, la seconde étant démontrée de manière similaire.

Supposons d’abord qu’il existe une sous-représentation E de la représentation $\boldsymbol{\gamma }_{G,\chi}$ isomorphe à $\pi$. Comme l’espace E n’est pas nul, il existe une fonction $f_1\in \mathscr{K}_{\overline{\chi}}(G)$ dont la classe $\widetilde{f}_1$ n’est pas orthogonale à E. On a $f_1\in \mathscr{L}_{\overline{\chi}}^1(G)$. Notons $\widetilde{f}_{1,E}$ la projection orthogonale de $\widetilde{f}_1$ sur E ; c’est un élément non nul de E. Soit par ailleurs $\widetilde{f}_2\in E$ non nulle. L’application $h:g\mapsto  \langle \widetilde{f}_{1,E}|\boldsymbol{\gamma }_{G,\chi}(g)\widetilde{f}_2\rangle$ est un coefficient matriciel de $\pi$. Pour tout $g\in G$, on a $h(g) =\langle \widetilde{f}_1|\boldsymbol{\gamma }_{G\overline{,\chi}}(g)\widetilde{f}_2\rangle$ puisque $\widetilde{f}_1-\widetilde{f}_{1,E}$ est orthogonale à E. D’après le lemme 8 de V, p. 418, la fonction $h$ appartient à $\mathscr{L}_{\chi}^2$(G), donc la proposition 6 implique que $\pi$ est de carré intégrable modulo le centre.

Réciproquement, supposons que $\pi$ est de carré intégrable modulo le centre. Soit $x_0\in E$ un vecteur non nul. D’après la prop. 7 et la formule (10), l’application $y\mapsto \check{f}_{x_0,y}$ est un G-morphisme injectif de $\pi$ dans $\boldsymbol{\gamma }_{G,\chi}$.

#### Définition 4 {#ts-v-s2-def-4 .statement tag=03AX}

Soit Z un sous-groupe fermé de C tel que $C/Z$ est compact. Soit $\pi$ une représentation unitaire irréductible de G qui est de carré intégrable modulo le centre. L’unique nombre réel $c >0$ qui vérifie la propriété de la proposition 7 est appelé le degré formel de $\pi$ relatif à Z. On le note $c_Z(\pi )$.

Le degré formel dépend du choix de la mesure de Haar sur Z. Si la mesure de Haar $\beta_Z$ sur Z est multipliée par un nombre réel $t >0$, alors la mesure $\nu_Z=\mu/\beta_Z$ sur $G/Z$ est multipliée par $t^{-1}$, et le degré formel de $\pi$ est multiplié par $t$.

Le degré formel est caractérisé par la propriété suivante :

#### Proposition 8 (Relations d’orthogonalité) {#ts-v-s2-prop-8 .statement tag=03AY}

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E qui est de carré intégrable modulo le centre. On a

$$
c_Z(\pi )\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle x|y\rangle \langle x'|y'\rangle
$$

pour tout $(x, y, x', y')\in E^4$.

Notons $w$ le morphisme de la prop. 7. On a

$$
\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle f_{x,x'}|f_{y,y'}\rangle
$$

et d’après loc. cit., il vient

$$
\langle f_{x,x'}|f_{y,y'}\rangle =\frac{1}{c_Z(\pi)}\langle w(x\otimes x')|w(y\otimes y')\rangle
$$

$$
=\frac{1}{c_Z(\pi)}\langle x\otimes x'|y\otimes y'\rangle =\frac{1}{c_Z(\pi)}\langle x|y\rangle_{\overline{E}}\langle x'|y'\rangle_E
$$

d’où le résultat.

En complément de la proposition précédente, on a aussi les relations suivantes pour des représentations irréductibles de carré intégrable non isomorphes.

#### Proposition 9 {#ts-v-s2-prop-9 .statement tag=03AZ}

Soient $\pi_1$ et $\pi_2$ des représentations unitaires irréductibles non isomorphes de G dans des espaces hilbertiens $E_1$ et $E_2$. On suppose que $\pi_1$ et $\pi_2$ sont de carré intégrable modulo le centre et que les restrictions à Z de leurs caractères centraux coïncident. Alors

$$
\int_{G/Z}\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\nu_Z(g) = 0
$$

pour tout $(x, x', y, y')\in E^2_1\times E^2_2$.

Pour $i= 1, 2$, notons $w_i$ le morphisme de la proposition 7 pour la représentation $\pi_i$. D’après le lemme 8, b) de V, p. 384 et l’assertion b) de la proposition 8 de V, p. 394, l’image de $w_i$ est contenue dans la composante $\pi_i$-isotypique de $\boldsymbol{\delta }_{G,\chi}$. D’après l’assertion a) de loc. cit., l’image de $w_1$ est donc orthogonale à l’image de $w_2$. Par conséquent, il vient $\langle w_1(x\otimes x')|w_2(y\otimes y')\rangle = 0$ pour tout $(x, x', y, y')\in E^2_1\times E^2_2$, ce qui est la formule demandée.

#### Remarque {#ts-v-s2-n8-rem-1 .statement tag=03B0}

Les relations d’orthogonalité des prop. 8 et 9 généralisent celles de A, VIII, p. 399 (voir aussi le cas où G est compact dans le § 2 de V, p. 457).

### 9. Sous-représentations de la représentation régulière d’un groupe commutatif

Dans ce numéro, G est un groupe localement compact commutatif et $\mu$ une mesure de Haar sur G. On note $\widehat{G}$ le groupe dual de G (déf. 2 de II, p. 201) et $\widehat{\mu}$ la mesure de Haar duale de $\mu$ sur $\widehat{G}$ (déf. 4 de II, p. 214). Les notions de mesurabilité seront toujours relatives à $\mu$ et $\widehat{\mu}$.

On se propose de déterminer toutes les sous-représentations de la représentation régulière gauche $\boldsymbol{\gamma }_G$ de G dans $L^2(G, \mu)$. Comme G est commutatif, on a d’ailleurs $\boldsymbol{\delta }_G(g) =\boldsymbol{\gamma }_G(g^{-1})$, donc ces sous-représentations sont aussi les sous-représentations de la représentation régulière droite.

Pour toute partie mesurable M de $\widehat{G}$, on note $E_M$ l’ensemble des $f\in L^2(G, \mu)$ telles que la transformée de Fourier $\mathscr{F}_G(f)$ est nulle presque partout sur M (cf. n$^o3$ de II, p. 210). C’est le noyau de l’application linéaire continue $f\mapsto \varphi_M\mathscr{F}_G(f)$ de $L^2(G, \mu)$ dans $L^2(\widehat{G},\widehat{\mu})$, où $\varphi_M$ désigne la fonction caractéristique de M (cf. th. 1 de II, p. 215), et c’est donc un sous-espace fermé dans $L^2(G, \mu)$.

On dit que des parties mesurables M et N de $\widehat{G}$ sont égales à un ensemble localement négligeable près si $(M\cup N)$- $(M\cap N)$ est localement négligeable. De manière équivalente, des parties mesurables M et N sont égales à un ensemble localement négligeable près si et seulement si les fonctions caractéristiques de M et N sont égales dans $L^{\infty}(\widehat{G},\widehat{\mu})$.

#### Proposition 10 {#ts-v-s2-prop-10 .statement tag=03B1}

a) Soit M une partie mesurable de $\widehat{G}$. L’espace $E_M$ est une sous-représentation de la représentation $\boldsymbol{\gamma }_G$;

b) Soient M et N des parties mesurables de $\widehat{G}$. On a $E_M= E_N$ si et seulement si M et N sont égales à un ensemble localement négligeable près;

c) Toute sous-représentation de $\boldsymbol{\gamma }_G$ est de la forme $E_M$ pour une partie mesurable M de $\widehat{G}$.

Soit $\eta$ l’application canonique de G dans $\widehat{\widehat{G}} ($cf. II, p. 216, remarque 1). Comme $E_M$ est fermé, l’assertion a) découle des formules

$$
\boldsymbol{\gamma }_G(x)(f) =\varepsilon_x*f,\mathscr{F}_G(\varepsilon_x*f) =\eta (x)\mathscr{F}_G(f)
$$

pour $x\in G$ et $f\in L^2(G, \mu)$.

Soient M et N des parties mesurables égales à un ensemble localement négligeable près. Comme $\varphi_M$ est alors égale à $\varphi_N$ dans $L^{\infty}(\widehat{G},\widehat{\mu})$, cette condition implique que $E_M= E_N$.

Supposons réciproquement que M et N ne sont pas égales à un ensemble localement négligeable près. Quitte éventuellement à échanger le rôle de M et N, il existe alors un sous-ensemble compact K tel que l’ensemble $L = K\cap (M$ - $(M\cap N))$ n’est pas négligeable. Soit $\varphi_L\in L^2(\widehat{G},\widehat{\mu})$ la classe de la fonction caractéristique de L, et posons $f=\overline{\mathscr{F}}_{\widehat{G}}(\varphi_L)\in L^2(G, \mu)$; on a $\mathscr{F}_G(f) =\varphi_L$ (cor. du th. 2 de II, p. 220). Alors $f$ appartient à $E_N$, puisque $L\cap N$ est vide, mais pas à $E_M$, puisque $\varphi_M\mathscr{F}(f) =\varphi_M\varphi_L=\varphi_L$. On a donc $E_M\not = E_N$, ce qui prouve b).

Soit maintenant E une sous-représentation de $\boldsymbol{\gamma }_G$. Soit $p_E$ l’orthoprojecteur de $L^2(G, \mu)$ d’image E et soit $q_E=\mathscr{F}_G\circ p_E\circ \mathscr{F}_G^{-1}$. Le projecteur $p_E$ appartient à Hom$_G(\boldsymbol{\gamma }_G,\boldsymbol{\gamma }_G)$ (prop. 4 de V, p. 383), donc il commute avec $\boldsymbol{\gamma }_G(f)$ pour tout $f\in L^1(G, \mu) ($cf. V, p. 401). Cela signifie qu’il commute avec les endomorphismes $\varphi \mapsto f*\varphi$ pour $f\in L^1(G, \mu)$ (lemme 4 de V, p. 407). Par conséquent, l’endomorphisme $q_E$ de $L^2(\widehat{G},\widehat{\mu})$ commute avec l’endomorphisme de multiplication par $g$ pour toute fonction $g\in \mathscr{C}_0(\widehat{G})$ appartenant à l’image de la transformation de Fourier de $L^1(G, \mu)$ dans $\mathscr{C}_0(\widehat{G})$ (prop. 14 de II, p. 223). Puisque l’image de la transformation de Fourier est dense dans $\mathscr{C}_0(\widehat{G})$ (corollaire de la prop. 5 de II, p. 209), la continuité du morphisme $g\mapsto m_g$ implique que $q_E$ commute avec $m_g$ pour toute fonction $g\in \mathscr{C}_0(\widehat{G})$.

D’après le corollaire de la proposition 7 de IV, p. 188, il existe donc une fonction $\varphi \in \mathscr{L}^{\infty}(\widehat{G},\widehat{\mu})$ telle que $q_E=m_{\varphi}$. Comme $q_E=q^2_E$, on a $m_{\varphi}=m^2_{\varphi}=m_{\varphi^2}$, d’où $\varphi =\varphi^2$ dans $L^{\infty}(\widehat{G},\widehat{\mu})$ (prop. 5 de IV, p. 186) ; cela signifie que $\varphi$ est égale dans $L^{\infty}(\widehat{G},\widehat{\mu})$ à la classe de la fonction caractéristique d’un sous-ensemble mesurable N de $\widehat{G}$. Posons $M =\widehat{G}-$ N. Soit $f\in L^2(G, \mu)$. On a $f\in E$ si et seulement si $p_E(f) =f$, si et seulement si $\varphi \mathscr{F}_G(f) =\mathscr{F}_G(f)$, ce qui équivaut à $f\in E_M$.

#### Remarque {#ts-v-s2-n9-rem-1 .statement tag=03B2}

Soit $\chi$ un caractère de G. Si G n’est pas compact, la composante $\chi$-isotypique de la représentation régulière de G dans $L^2(G)$ est triviale. Si G est compact, la composante $\chi$-isotypique de la représentation régulière de G est de dimension 1 et la fonction $\chi \in L^2(G)$ en est une base.

### 10. Représentations unitaires du groupe R

Dans ce numéro, E désigne un espace hilbertien complexe. On munit le groupe $\mathbf{R}$ de la mesure de Lebesgue.

#### Lemme 11 {#ts-v-s2-lem-11 .statement tag=03B3}

Soit $u$ un opérateur partiel auto-adjoint sur E. Pour $t\in \mathbf{R}$, posons $\varrho (t) =e^{itu}\in \mathscr{L}(E)$. Alors l’application $\varrho$ est une représentation unitaire de $\mathbf{R}$.

L’opérateur $\varrho (t)$ est défini par le calcul fonctionnel universellement mesurable (déf. 5 de IV, p. 272) ; c’est un endomorphisme de E puisque la fonction $x\mapsto e^{itx}$ est bornée sur Sp($u$) (prop. 5, a) de IV, p. 275).

D’après la prop. 5 de IV, p. 275, on a $\varrho (0) = 1_E,\varrho (t)^*=\varrho (-t)$ pour tout $t\in \mathbf{R}$ et $\varrho (t_1+t_2) =\varrho (t_1)\varrho (t_2)$ pour tous $t_1$ et $t_2$ dans $\mathbf{R}$. En particulier, l’endomorphisme $\varrho (t)$ est unitaire pour tout $t\in \mathbf{R}$. Pour tout $x\in E$, l’application de $\mathbf{R}$ dans E définie par $x\mapsto \varrho (t)x$ est continue en $t= 0$ d’après la prop. 6 de IV, p. 276, donc $\varrho$ est une représentation unitaire de $\mathbf{R}$ dans E (V, p. 380, lemme 4).

#### Lemme 12 {#ts-v-s2-lem-12 .statement tag=03B4}

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$ dans E. Soit D l’ensemble des éléments $x$ de E tels que l’application $\psi_x:t\mapsto \varrho (t)x$ est dérivable en 0. L’application $u$ de D dans E donnée par $x\mapsto i^{-1}\psi '_x(0)$ définit un opérateur partiel symétrique sur E.

Soient $f\in \mathscr{D}(\mathbf{R})$ et $x\in E$. Posons $y=\varrho (f)x$. Pour tout $h\in \mathbf{R}$, on a

$$
\psi_y(h) =\varrho (h)\varrho (f)x=\varrho (f)\varrho (h)x
$$

$$
=\int_{\mathbf{R}}f(t)\varrho (t+h)x dt=\int_{\mathbf{R}}f(t-h)\psi_x(t)dt
$$

La fonction de $\mathbf{R}^2$ dans $\mathbf{C}$ définie par $(t, h)\mapsto f(t-h)$ est indéfiniment dérivable ; sa dérivée par rapport à $h$ est la fonction définie par $(t, h)\mapsto$ $-f'(t-h)$, qui est bornée par $\|f'\|_{\infty}$. Lorsque $h= 0$, cette dérivée est nulle pour $t$ en dehors d’un ensemble compact. Comme $\|\psi_x(t)\|=\|x\|$ pour tout $t$, on déduit de la prop. 2 de IV, p. 197 que la fonction $\psi_y$ est dérivable en 0 et que sa dérivée est donnée par

$$
\psi '_y(0) =-\int_{\mathbf{R}}f'(t)\psi_x(t)dt=-\varrho (f')x
$$

On a donc $y\in D$. Comme l’espace $\mathscr{D}(\mathbf{R})$ est dense dans $L^1(\mathbf{R})$ (prop. 4 de IV, p. 202) on déduit de INT, VIII, p. 139, § 2, n$^o7$, prop. 10 que l’espace D est dense dans E.

Soient $x_1$ et $x_2$ dans D. On calcule

$$
i
$$

$\langle u(x_1)|x_2\rangle =$ lim $\langle (\varrho (h)-1_E)x_1|x_2\rangle$

$$
_{h\rightarrow 0}h
$$

$$
i
$$

= lim $\langle x_1|(\varrho (-h)-1_E)x_2\rangle =\langle x_1|u(x_2)\rangle$.

$$
_{h\rightarrow 0}h
$$

Par conséquent, l’opérateur partiel $u$ est symétrique.

#### Définition 5 {#ts-v-s2-def-5 .statement tag=03B5}

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$ dans E. L’opérateur partiel symétrique défini dans le lemme 12 est appelé le générateur infinitésimal de $\varrho$.

#### Théorème 1 (Stone) {#ts-v-s2-thm-1 .statement tag=03B6}

L’application $\sigma$ qui à une représentation unitaire $\varrho$ de $\mathbf{R}$ dans E associe son générateur infinitésimal $u$ définit une bijection de l’ensemble des représentations unitaires de $\mathbf{R}$ dans E dans l’ensemble des opérateurs partiels auto-adjoints sur E. La bijection réciproque $\tau$ associe à un opérateur partiel auto-adjoint la représentation unitaire $t\mapsto e^{itu}$.

Démontrons d’abord quelques lemmes.

#### Lemme 13 {#ts-v-s2-lem-13 .statement tag=03B7}

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$ dans E et soit $u$ son générateur infinitésimal.

a) Le domaine de $u$ est l’ensemble des $x\in E$ tels que l’application $\psi_x:t\mapsto \varrho (t)x$ est dérivable sur $\mathbf{R}$;

b) Pour tout $t\in \mathbf{R}$ et tout $x\in$ dom($u$), on a $\varrho (t)x\in$ dom($u$) et $\psi '_x(t) =iu(\varrho (t)x)$;

c) L’opérateur partiel $u$ est essentiellement auto-adjoint.

Pour tout $x\in E$, notons $\psi_x$ l’application de $\mathbf{R}$ dans E définie par $\psi_x(t) =\varrho (t)x$. Pour tout $t\in \mathbf{R}$ et tout $h\in \mathbf{R}$, on a

$$
\psi_x(t+h)-\psi_x(t) =\varrho (t)(\psi_x(h)-\psi_x(0))
$$

ce qui démontre que dom($u$) est l’espace des éléments $x\in E$ tels que $\psi_x$ est dérivable sur $\mathbf{R}$ et établit que $\psi '_x(t) =\varrho (t)\psi '_x(0) =i\varrho (t)(u(x))$ pour tout $t\in \mathbf{R}$.

Soient $x\in$ E et $t\in \mathbf{R}$. On a $\psi_{\varrho(t)x}(s) =\psi_x(s+t)$ pour tout $s\in \mathbf{R}$. Par conséquent, on a $\varrho (t)x\in$ dom($u$) si $x\in$ dom($u$), et de plus $u(\varrho (t)x) =i^{-1}\psi '_x(t) =\varrho (t)u(x)$ d’après a). On obtient alors l’assertion b).

Démontrons c). Soit $x\in$ Ker($u^*-i1_E$). Démontrons que $x= 0$. Soit $y\in$ dom($u$), et soit $f$ la fonction sur $\mathbf{R}$ définie par $f(t) =\langle \psi_y(t)|x\rangle$ pour $t\in \mathbf{R}$. La fonction $f$ est bornée puisque $\|\psi_y(t)\|=\|y\|$ pour tout $t\in \mathbf{R}$; elle est dérivable dans $\mathbf{R}$ et, pour tout $t\in \mathbf{R}$, l’assertion b) implique

$$
f'(t) =\langle \psi '_y(t)|x\rangle =\langle iu(\varrho (t)y)|x\rangle
$$

$$
=-i\langle \varrho (t)y|u^*(x)\rangle =-i\langle \psi_y(t)|ix\rangle =f(t)
$$

puisque $u^*(x) =ix$. On a donc $f(t) =f(0)e^t$ pour tout $t\in \mathbf{R}$ (FVR, IV, p. 27). Puisque $f$ est bornée, la fonction $f$ est nulle et, en particulier, on a $\langle y|x\rangle =f(0) = 0$. Comme l’espace dom($u$) est dense dans E, on conclut que $x= 0$. De même, on démontre que Ker($u^*+i1_E$) est réduit à 0. D’après le cor. 3 de IV, p. 261, l’opérateur partiel $u$ est donc essentiellement auto-adjoint.

#### Lemme 14 {#ts-v-s2-lem-14 .statement tag=03B8}

Soit $u$ un opérateur partiel auto-adjoint sur E et soit $\varrho (t) =e^{itu}$ la représentation unitaire de $\mathbf{R}$ définie par $u$. Le générateur infinitésimal de $\varrho$ est égal à $u$.

Soit $x\in$ dom($u$). Posons $\psi_x(t) =\varrho (t)x$ pour tout $t\in \mathbf{R}$. Pour tout nombre réel $h$ non nul, on a

$$
\frac{1}{h}(\psi_x(t+h)-\psi_x(t)) =(\frac{1}{h}(e^{ihu}-1_E))e^{itu}x=(\frac{1}{h}(e^{ihu}-1_E))\varrho (t)x
$$

Lorsque $h$ tend vers 0, on a

1 $_{iht}$

$$
(e-1)\rightarrow it
$$

$$
h
$$

pour tout $t\in \mathbf{R}$. De plus,

$$
|\frac{1}{h}(e^{iht}-1)|=|t||\frac{1}{h}\int_0^he^{its}ds|\leqslant |t|
$$

Il résulte alors de la prop. 6 de IV, p. 276 que la fonction $\psi_x$ est dérivable sur $\mathbf{R}$ et vérifie $\psi '_x(t) =iu(\varrho (t)x)$ pour tout $t\in \mathbf{R}$. Par conséquent, le domaine de $u$ est inclus dans l’ensemble des $x\in E$ tels que $\psi_x$ est dérivable en 0 et qu’on a alors $\psi '_x(0) =iu(x)$. Cela signifie par définition que le générateur infinitésimal de $\varrho$ est une extension de $u$. Ces deux opérateurs sont donc égaux puisqu’ils sont symétriques et que $u$ est auto-adjoint (IV, p. 238, remarque 5).

#### Lemme 15 {#ts-v-s2-lem-15 .statement tag=03B9}

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$ dans E. Alors le générateur infinitésimal $u$ de $\varrho$ est auto-adjoint et $\varrho (t) =e^{itu}$ pour tout $t\in \mathbf{R}$.

D’après le lemme 13, c), l’opérateur partiel $u$ est essentiellement auto-adjoint. Sa fermeture $\overline{u}$ est donc un opérateur auto-adjoint. Notons $\pi$ la représentation unitaire de $\mathbf{R}$ définie par $\pi (t) =e^{itu}$ (lemme 11).

Pour tout $x\in E$, notons $\psi_x$ (resp. $\widetilde{\psi}_x)$ l’application de $\mathbf{R}$ dans E définie par $\psi_x(t) =\varrho (t)x$ (resp. par $\widetilde{\psi}_x(t) =\pi (t)x)$.

D’après le lemme 13, a) et b), l’espace dom($u$) est le sous-espace de E formé des éléments $x\in E$ tels que l’application $\psi_x$ est dérivable sur $\mathbf{R}$, et pour tout $x\in$ dom($u$) et tout $t\in \mathbf{R}$, on a $\psi '_x(t) =iu(\psi_x(t))$. De même, l’espace dom($\overline{u}$) est le sous-espace de E formé des éléments $x\in E$ tels que l’application $\widetilde{\psi}_x$ est dérivable sur $\mathbf{R}$, et pour tout $x\in$ dom($\overline{u}$) et tout $t\in \mathbf{R}$, on a $\widetilde{\psi}'_x(t) =iu(\widetilde{\psi}_x(t))$.

Soit $x\in$ dom($u$)$\subset$ dom($\overline{u}$). Posons $f=\psi_x-\widetilde{\psi}_x$. C’est une fonction dérivable de $\mathbf{R}$ dans E. Pour tout $t\in \mathbf{R}$, il vient

$$
f'(t) =iu(\psi_x(t))-iu(\widetilde{\psi}_x(t)) =iu(f(t))
$$

puisque $\psi_x(t)\in$ dom($u$) et $u\subset \overline{u}$. Posons $g=\|f\|^2$; c’est une application dérivable de $\mathbf{R}$ dans $\mathbf{R}$ telle que $g(0) = 0$. Pour $t\in \mathbf{R}$, on obtient d’après FVR, I, p. 28, prop. 2

$$
g'(t) =\langle f'(t)|f(t)\rangle +\langle f(t)|f'(t)\rangle
$$

$$
=\langle iu(f(t))|f(t)\rangle +\langle f(t)|iu(f(t))\rangle = 0
$$

puisque $\overline{u}$ est auto-adjoint. On a donc $f= 0$, d’où $\varrho (t)x=\pi (t)x$ pour tout $t\in \mathbf{R}$. Les endomorphismes continus $\varrho (t)$ et $\pi (t)$ de E coïncident sur dom($u$), et sont donc égaux pour tout $t\in \mathbf{R}$. Ainsi, on a $\pi =\varrho$; comme $\overline{u}$ est le générateur infinitésimal de $\pi$ (lemme. 14), on a $\overline{u}=u$, ce qui démontre que $u$ est auto-adjoint.

Nous pouvons maintenant démontrer le th. 1.

Les applications $\sigma$ et $\tau$ sont bien définies (lemme 15 et lemme 11, respectivement).

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$. Notons $u$ son générateur infinitésimal. La relation $\varrho (t) =e^{itu}$ pour tout $t\in \mathbf{R}$ (lemme 15) démontre que $\tau \circ \sigma$ est l’application identique.

Soit $u$ un opérateur partiel auto-adjoint sur E. Le lemme 14 démontre que le générateur infinitésimal de la représentation unitaire $t\mapsto e^{itu}$ est égal à $u$, donc $\sigma \circ \tau$ est l’application identique.

Soit $u$ un opérateur partiel auto-adjoint sur E et soit $\varrho (t) =e^{itu}$ pour $t\in \mathbf{R}$ la représentation unitaire de $\mathbf{R}$ dans E qui lui est associée. Soit $x\in$ dom($u$). L’équation $\partial_t\varrho (t)x=iu(\varrho (t)x)$ qui est alors satisfaite (lemme 13, b)) est appelée l’équation de Schrödinger.

#### Corollaire {#ts-v-s2-n10-cor-1 .statement tag=03BA}

Soit $\varrho$ une représentation unitaire de $\mathbf{R}$ dans un espace hilbertien E. Il existe un espace localement compact X, une mesure positive $\mu$ sur X et une fonction continue $g$ sur X à valeurs réelles tels que $\varrho$ est isomorphe à la représentation $\pi$ de $\mathbf{R}$ dans $L^2(X, \mu)$ définie par $\pi (t)f=e^{itg}f$ pour tout $t\in \mathbf{R}$ et tout $f\in L^2(X, \mu)$.

Soit $u$ l’opérateur auto-adjoint sur E tel que $\varrho (t) =e^{itu}$ pour tout $t\in \mathbf{R}$ (théorème 1). Il existe un espace localement compact X, une mesure positive $\mu$ sur X, un isomorphisme isométrique $\theta$ de $L^2(X, \mu)$ sur E et une fonction continue $g$ sur X à valeurs réelles tels que $u=\theta \circ m_g\circ \theta^{-1}$ (th. 1 de IV, p. 266). L’assertion résulte de la formule $e^{itu}=\theta \circ e^{itm_g}\circ \theta^{-1}=\theta \circ m_{e^{itg}}\circ \theta^{-1}$ (lemme 4 de IV, p. 269).

#### Remarque {#ts-v-s2-n10-rem-1 .statement tag=03BB}

Supposons que $u$ est un endomorphisme de E. La représentation unitaire de $\mathbf{R}$ dans E définie par $\varrho (t) =e^{itu}$ vérifie alors l’inégalité $\|\varrho (t)-1_E\|\leqslant |t| \|u\|$ pour tout $t\in \mathbf{R}$, et l’application $\varrho$ de $\mathbf{R}$ dans l’espace de Banach $\mathscr{L}(E)$ est l’unique solution de l’équation différentielle linéaire

$$
1d\varrho
$$

$$
=u\circ \varrho
$$

$$
idt
$$

(cf. FVR, IV, p. 26, §6).

#### Exemple {#ts-v-s2-n10-exa-1 .statement tag=03BC}

Soit $\varrho$ la représentation régulière de $\mathbf{R}$ dans $L^2(\mathbf{R})$. Le générateur infinitésimal de $\varrho$ est la fermeture de l’opérateur différentiel de domaine $\mathscr{D}(\mathbf{R})$ défini par $f\mapsto  -if'$.

## EXERCICES {#ts-v-s2-exercises}

Dans les exercices de ce paragraphe, sauf mention du contraire, G désigne un groupe topologique localement compact, muni d’une mesure de Haar à gauche qui est notée $\mu$.

See the [exercises for § 2](exercises/s2/).
