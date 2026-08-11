---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 10
section_title: Modules sur un anneau artinien
lang: fr
source: alg-viii-fr
book_pages: A VIII.169-A VIII.177
pdf_pages: 0175-0183
extraction: native
subsections:
    - "no": 1
      title: Radical d’un anneau artinien
      page: 169
      pdf_page: 175
    - "no": 2
      title: Modules sur un anneau artinien
      page: 170
      pdf_page: 176
    - "no": 3
      title: Modules projectifs sur un anneau artinien
      page: 171
      pdf_page: 177
statements: 12
exercises: 11
content_sha256: 55485906eea7d0089748b7d8faa05e77381c6f78f7ca1b7225c5d753c234b076
---

## § 10. MODULES SUR UN ANNEAU ARTINIEN

### 1. Radical d’un anneau artinien

#### Proposition 1 {#alg-viii-s10-prop-1 .statement tag=00C5}

Soit A un anneau artinien à gauche. Le radical $\mathfrak{r}$ de A est le plus grand idéal bilatère nilpotent de A et l’anneau $A/\mathfrak{r}$ est semi-simple.

On sait (VIII, p. 151, th. 1) que tout idéal bilatère nilpotent de A est contenu dans $\mathfrak{r}$. Prouvons que $\mathfrak{r}$ est nilpotent. Comme l’anneau A est artinien à gauche et que la suite des idéaux bilatères $\mathfrak{r}^n$ est décroissante, il existe un entier $p\geqslant 0$ tel qu’on ait $\mathfrak{r}^p=\mathfrak{r}^{p+1}$. Comme A est artinien, le A-module $A_s$ est de longueur finie (VIII, p. 5, th. 1) et donc noethérien. L’idéal à gauche $\mathfrak{r}^p$ est donc de type fini. D’après le lemme de Nakayama (th. 2 de VIII, p. 154), il en résulte que $\mathfrak{r}^p= 0$.

L’anneau $A/\mathfrak{r}$ est sans radical (VIII, p. 150, prop. 5) ; comme il est artinien à gauche, il est semi-simple (VIII, p. 150, prop. 4).

#### Corollaire 1 {#alg-viii-s10-prop-1-cor-1 .statement tag=00C6}

Pour qu’un anneau soit semi-simple, il faut et il suffit qu’il soit artinien à gauche et ne possède aucun idéal bilatère nilpotent autre que 0.

Un anneau semi-simple est artinien à gauche et sans radical (VIII, p. 150, prop. 4) ; il ne possède donc aucun idéal bilatère nilpotent autre que 0. La réciproque résulte de la prop. 1.

#### Corollaire 2 {#alg-viii-s10-prop-1-cor-2 .statement tag=00C7}

Dans un anneau artinien à gauche A, le radical se compose des éléments $x$ tels que ax soit nilpotent pour tout $a$ dans A.

Si A est artinien à gauche, le radical est un idéal bilatère nilpotent (prop. 1) ; tout nilidéal à gauche est contenu dans le radical d’après le théorème de Jacobson (VIII, p. 151, th. 1). Le corollaire 2 en résulte.

### 2. Modules sur un anneau artinien

#### Proposition 2 {#alg-viii-s10-prop-2 .statement tag=00C8}

Soit A un anneau artinien à gauche. Pour tout A-module M, les propriétés suivantes sont équivalentes :

(i) M est semi-simple ;

(ii) M est sans radical ;

(iii) M est annulé par le radical $\mathfrak{r}$ de A.

On sait que (i) implique (ii) (VIII, p.149, prop. 3). D’autre part, $\mathfrak{r}M$ est contenu dans le radical de M (VIII, p. 154, prop. 6) ; donc (ii) implique (iii).

Supposons que le A-module M soit annulé par $\mathfrak{r}$. On peut le considérer comme un module sur l’anneau $A/\mathfrak{r}$. Or l’anneau $A/\mathfrak{r}$ est semi-simple (VIII, p. 169, prop. 1) et tout module sur un anneau semi-simple est semi-simple (VIII, p. 134, prop. 4). Par suite, M est un module semi-simple sur l’anneau $A/\mathfrak{r}$ et a fortiori sur l’anneau A. Donc (iii) implique (i).

#### Corollaire {#alg-viii-s10-n2-cor-1 .statement tag=00C9}

Soit A un anneau artinien à gauche. Pour tout A-module M, le radical de M est égal à $\mathfrak{r}M$.

Le radical $\mathfrak{R}(M)$ de M contient $\mathfrak{r}M$ (VIII, p. 154, prop. 6). Par ailleurs, le A-module $M/\mathfrak{r}M$ est annulé par $\mathfrak{r}$; d’après la prop. 2, il est donc sans radical, et cela entraîne $\mathfrak{R}(M)\subset \mathfrak{r}M$ (VIII, p. 148, cor. 1, c)).

#### Proposition 3 {#alg-viii-s10-prop-3 .statement tag=00CA}

Soient A et B des anneaux et $f$ un homomorphisme de A dans B, tel que B soit engendré par la réunion de $f(A)$et du commutant $f(A)'$ de $f(A)$dans B. Soit M un B-module à gauche. On suppose que l’anneau A est artinien à gauche, ou que le A-module $f_*(M)$déduit de M par restriction des scalaires (II, p. 30) est de type fini. On a alors $\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$.

Soit S un B-module simple. Supposons que A soit artinien à gauche ou que le A-module $f_*(S)$ soit de type fini. Nous allons démontrer que $f_*(S)$ est sans radical. Pour tout $b\in f(A)'$, l’homothétie $b_S$ est un endomorphisme du A-module $f_*$(S), donc laisse stable $\mathfrak{R}_A(f_*(S))$ (VIII, p. 148, prop. 1). Comme B est engendré par $f(A)\cup f(A)'$, le radical $\mathfrak{R}_A(f_*(S))$ est un sous-B-module de S, donc égal à 0 ou S. Si $f_*(S)$ est un A-module de type fini, on a $\mathfrak{R}_A(f_*(S))\not=f_*(S)$ (VIII, p. 149, prop. 2). Si l’anneau A est artinien à gauche, on a $\mathfrak{R}_A(f_*(S)) =f(\mathfrak{r})S$, où $\mathfrak{r}$ est le radical de A (VIII, p. 170, cor. de la prop. 2) et comme $\mathfrak{r}$ est un idéal bilatère nilpotent de A (VIII, p. 169, prop. 1), on ne peut avoir $S =f(\mathfrak{r})S$. Dans les deux cas, on a donc $\mathfrak{R}_A(f_*(S)) = 0$.

Soit $u$ une application B-linéaire non nulle de M dans un B-module simple S. L’application $u$ est surjective ; par conséquent si $f_*(M)$ est de type fini, il en est de même de $f_*(S)$. Sous les hypothèses de la prop. 3, le A-module $f_*(S)$ est sans radical et $u$ est une application A-linéaire de $f_*(M)$ dans $f_*(S)$. Donc le noyau de $u$ contient $\mathfrak{R}_A(f_*(M))$ d’après la prop. 1 de VIII, p. 148. Comme $u$ est arbitraire, on a $\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$.

#### Corollaire {#alg-viii-s10-n2-cor-2 .statement tag=00CB}

Soient A un anneau commutatif et B une algèbre sur A. On suppose que l’anneau A est artinien ou que B est un A-module de type fini. On a alors $\mathfrak{R}(A)B\subset \mathfrak{R}(B)$.

D’après la prop. 3, le radical $\mathfrak{R}_A(B_s)$ est contenu dans $\mathfrak{R}_B(B_s)$, qui n’est autre que le radical de l’anneau B. Par ailleurs, on a $\mathfrak{R}(A)B\subset \mathfrak{R}_A(B_s)$ d’après la prop. 6 de VIII, p. 154, d’où le corollaire.

### 3. Modules projectifs sur un anneau artinien

#### Proposition 4 {#alg-viii-s10-prop-4 .statement tag=00CC}

Tout module sur un anneau artinien à gauche possède une couverture projective.

Soit A un anneau artinien à gauche et soit M un module sur A. Le radical $\mathfrak{r}$ de A est un idéal bilatère nilpotent et l’anneau $A/\mathfrak{r}$ est semi-simple (VIII, p. 169, prop. 1). Il s’ensuit que le $A/\mathfrak{r}$-module $M/\mathfrak{r}M$ est projectif ; l’assertion résulte alors de la prop. 11 de VIII, p. 160.

#### Proposition 5 {#alg-viii-s10-prop-5 .statement tag=00CD}

Soient A un anneau artinien à gauche et $\mathfrak{r}$ son radical.

a) Soit P un A-module projectif. Notons $u$ l’application canonique de P sur $P/\mathfrak{r}P$. Alors $(P, u)$est une couverture projective de $P/\mathfrak{r}P$. En particulier, le A-module P est de type fini si et seulement si $P/\mathfrak{r}P$l’est.

b) Soit M un module sur l’anneau $A/\mathfrak{r}$. Alors M, considéré comme A-module, possède une couverture projective. Si $(P, u)$est une telle couverture projective, $u$ induit par passage au quotient un isomorphisme de $P/\mathfrak{r}P$sur M. De plus, P est indécomposable si et seulement si M est simple.

c) Soient M et $M'$ des modules sur l’anneau $A/\mathfrak{r}$. Soient $(P, u)$et $(P', u')$des couvertures projectives des A-modules M et $M'$. Alors M et $M'$ sont isomorphes si et seulement si P et $P'$ le sont.

Le radical $\mathfrak{r}$ de A est un idéal bilatère nilpotent (VIII, p. 169, prop. 1). L’assertion a) résulte donc du cor. 1 de VIII, p. 159 et de la remarque 2 de VIII, p. 157.

Démontrons l’assertion b). L’existence d’une couverture projective $(P, u)$ de M résulte de la prop. 4 et l’isomorphisme de $P/\mathfrak{r}P$ avec M de la prop. 9 de VIII, p. 158. Comme l’anneau $A/\mathfrak{r}$ est semi-simple, un module sur cet anneau est indécomposable si et seulement s’il est simple. La dernière assertion découle alors du cor. 2 de VIII, p. 156.

Prouvons c). Soit $f$ un isomorphisme de P sur $P'$; il induit un isomorphisme $f$ de $P/\mathfrak{r}P$ sur $P'/\mathfrak{r}P'$, qui sont respectivement isomorphes à M et $M'$ d’après b). Donc M est isomorphe à $M'$. Réciproquement, tout isomorphisme $f$ de M sur $M'$ se relève en un isomorphisme $\widetilde{f}$ de P sur $P'$ tel que $f\circ u=u'\circ \widetilde{f}$ d’après la prop. 8 de VIII, p. 157.

#### Corollaire {#alg-viii-s10-n3-cor-1 .statement tag=00CE}

À toute classe P de A-modules projectifs, associons la classe $\varphi (P)$ du module $P/\mathfrak{r}P$sur l’anneau $A/\mathfrak{r}$. Toute classe de modules (resp. de modules de type fini) sur l’anneau $A/\mathfrak{r}$ est de la forme $\varphi (P)$pour une unique classe P de A-modules projectifs (resp. de A-modules projectifs de type fini).

Soient A un anneau artinien à gauche et $\mathfrak{r}$ son radical. Notons $\mathscr{S}$ l’ensemble des classes de A-modules simples ; il est fini (VIII, p. 47). D’après la prop. 2 de VIII, p. 170, il s’identifie canoniquement à l’ensemble des classes de modules simples sur l’anneau semi-simple $A/\mathfrak{r}$. Pour tout $\lambda \in \mathscr{S}$, notons $S_{\lambda}$ un A-module simple de classe $\lambda$ et choisissons une couverture projective $(P_{\lambda}, u_{\lambda})$ de $S_{\lambda}$ (VIII, p. 171, prop. 4). D’après la prop. 5, le A-module $P_{\lambda}$ est projectif et indécomposable et $u_{\lambda}$ définit un isomorphisme de $P_{\lambda}/\mathfrak{r}P_{\lambda}$ sur $S_{\lambda}$. De plus, si P est un A-module projectif et indécomposable, il existe un unique $\lambda \in \mathscr{S}$ tel que P soit isomorphe à $P_{\lambda}:$ c’est l’unique $\lambda \in \mathscr{S}$ tel que $P/\mathfrak{r}P$ soit isomorphe à $S_{\lambda}$.

#### Proposition 6 {#alg-viii-s10-prop-6 .statement tag=00CF}

Soient A un anneau artinien à gauche et $\mathfrak{r}$ son radical. Soit P un A-module projectif.

a) Le A-module $P = P/\mathfrak{r}P$est semi-simple et le A-module P est isomorphe à $\bigoplus\lambda \in \mathscr{S}P([P:\lambda \lambda ])$.

b) Soit $(Q_i)_{i\in I}$ une famille de sous-modules projectifs indécomposables de P dont P est la somme directe. Alors pour tout $\lambda \in \mathscr{S}$, le cardinal de l’ensemble $I(\lambda )$des $i\in I$tels que $Q_i$ soit isomorphe à $P_{\lambda}$ est égal à $[P :\lambda ]$.

Le fait que P soit semi-simple résulte de la prop. 2 (VIII, p. 170). Le A-module $Q =\oplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ est projectif, et comme $P_{\lambda}/\mathfrak{r}P_{\lambda}$ est isomorphe à $S_{\lambda}, Q/\mathfrak{r}Q$ est isomorphe à $\oplus_{\lambda\in\mathscr{S}}S^{([P:\lambda])}_{\lambda}$, c’est-à-dire à $P = P/\mathfrak{r}P$. D’après la prop. 5, les A-modules P et Q sont isomorphes.

Supposons donnée une famille $(Q_i)_{i\in I}$ de sous-modules projectifs et indécomposables, dont P soit somme directe. Pour tout $i\in I$, le A-module $Q_i/\mathfrak{r}Q_i$ est simple d’après la prop. 5. Pour $\lambda \in \mathscr{S}$, notons $I(\lambda )$ l’ensemble des $i\in I$ tels que $Q_i/\mathfrak{r}Q_i$ soit isomorphe à $S_{\lambda}$, donc à $P_{\lambda}/\mathfrak{r}P_{\lambda}$; c’est aussi l’ensemble des $i\in I$ tels que $Q_i$ soit isomorphe à $P_{\lambda}$. Comme $P = P/\mathfrak{r}P$ est somme directe de la famille $(Q_i/\mathfrak{r}Q_i)_{i\in I}$, on a Card(I($\lambda$ )) $= [P :\lambda ]$ d’après le th. 1 de VIII, p. 29.

#### Exemple {#alg-viii-s10-n3-exa-1 .statement tag=00CG}

Prenons P égal à $A_s$. Pour tout $\lambda \in \mathscr{S}$, notons $D_{\lambda}$ le corps opposé du commutant du A-module simple $S_{\lambda}$ et $m(\lambda )$ la dimension de $S_{\lambda}$ considéré comme espace vectoriel à droite sur le corps $D_{\lambda}$. On sait que $m(\lambda )$ est égale à la multiplicité $[A_s/\mathfrak{r}A_s:\lambda ]$ (VIII, p. 139, prop. 11). Par conséquent, le A-module $A_s$ est isomorphe à $\oplus_{\lambda\in\mathscr{S}}P^{m(\lambda)}_{\lambda}$.

## EXERCICES {#alg-viii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
