---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 1
section_title: Spectres et caractères
lang: fr
source: ts-i-ii-fr
book_pages: TS I.1-TS I.15, TS I.153-TS I.154
pdf_pages: 0014-0028, 0166-0167
extraction: native
subsections:
    - "no": 1
      title: Algèbres unifères
      page: 1
      pdf_page: 14
    - "no": 2
      title: Spectre d’un élément dans une algèbre unifère
      page: 2
      pdf_page: 15
    - "no": 3
      title: Résolvante
      page: 3
      pdf_page: 16
    - "no": 4
      title: Spectre d’un élément dans une algèbre
      page: 4
      pdf_page: 17
    - "no": 5
      title: Sous-algèbres pleines
      page: 5
      pdf_page: 18
    - "no": 6
      title: Caractères d’une algèbre unifère commutative
      page: 6
      pdf_page: 19
    - "no": 7
      title: Cas des algèbres sans élément unité
      page: 9
      pdf_page: 22
    - "no": 8
      title: Idéaux primitifs
      page: 11
      pdf_page: 24
statements: 33
exercises: 8
content_sha256: 0c27f411f0ce6c8572cd94251b968e53245daa315b0cda2865409924ee87dc09
---

## § 1. SPECTRES ET CARACTÈRES

Dans ce paragraphe, la lettre K désigne un corps commutatif. Si E et F sont des K-espaces vectoriels, on note $E\otimes F = E\otimes_KF$.

### 1. Algèbres unifères

On appelle algèbre unifère sur K un couple $(A, e)$ où A est une algèbre sur K à élément unité et $e$ l’élément unité de A. Comme $e$ est déterminé de manière unique par A, il nous arrivera de dire, par abus de langage, que A est une algèbre unifère. Si $(A, e)$ et $(A', e')$ sont des algèbres unifères, on appelle morphisme unifère de $(A, e)$ dans $(A', e')$ un morphisme $\varphi$ de A dans $A'$ tel que $\varphi (e) =e'$. Une sous-algèbre unifère de $(A, e)$ est un couple $(A', e)$, où $A'$ est une sous-algèbre de A contenant $e$.

On notera souvent 1 l’élément unité.

#### Lemme 1 {#ts-i-s1-lem-1 .statement tag=024R}

Soit A une algèbre. Pour tout idempotent $j$ de A, le sous-espace $jAj$ de A est l’ensemble des $x\in A$ tels que $xj=jx=x$. C’est une sous-algèbre de A qui admet l’élément unité $j$.

La preuve est élémentaire.

### 2. Spectre d’un élément dans une algèbre unifère

#### Définition 1 {#ts-i-s1-def-1 .statement tag=024S}

Soient A une algèbre unifère sur K et $e$ son élément unité. Pour tout $x\in A$, on appelle spectre de $x$ relativement à A l’ensemble des $\lambda \in K$ tels que $\lambda e-x$ ne soit pas inversible.

Le spectre de $x$ sera noté Sp$_A(x)$, ou Sp($x$) si aucune confusion n’en résulte. Le complémentaire de Sp$_A(x)$ dans K est appelé l’ensemble résolvant de $x$.

#### Remarque 1 {#ts-i-s1-n2-rem-1 .statement tag=024T}

Si $A =\{0\}$, on a Sp(0) $=\emptyset$.

#### Remarque 2 {#ts-i-s1-n2-rem-2 .statement tag=024U}

Si $A\not=\{0\}$, on a Sp($\lambda e$) $=\{\lambda \}$ pour tout $\lambda \in K$.

#### Remarque 3 {#ts-i-s1-n2-rem-3 .statement tag=024V}

Pour que $x\in A$ soit inversible, il faut et il suffit que $0\notin$ Sp($x$).

#### Remarque 4 {#ts-i-s1-n2-rem-4 .statement tag=024W}

Soit $R\in K(X)$ une fraction rationnelle et soit $x\in A$ un élément qui est substituable dans R, c’est-à-dire (A, IV, p. 20) qu’il existe P et $Q\in K[X]$ tels que $R = P/Q$ et $Q(x)$ est inversible ; on peut alors former l’élément $R(x) = P(x)\cdot Q(x)^{-1}= Q(x)^{-1}\cdot P(x)$ de A ; il ne dépend pas des choix de P et Q. On a $0\notin$ Q(Sp($x$)), de sorte que tout élément de Sp($x$) est substituable dans R.

On a R(Sp($x$))$\subset$ Sp(R($x$)). Soit en effet $\lambda \in$ Sp($x$) ; il existe un polynôme $P_1$ tel que $R(\lambda )-R(X) = (\lambda -X)P_1(X)/Q(X)$ ; alors, $R(\lambda )e-$ $R(x) = (\lambda e-x)(P_1(x)/Q(x))$, de sorte que $R(\lambda )-R(x)$ n’est pas inversible, donc $R(\lambda )\in$ Sp(R($x$)).

Inversement, supposons que le corps K est algébriquement clos. Supposons d’abord que R n’est pas constante et démontrons que l’on a Sp(R($x$)) $=$ R(Sp($x$)). Soit $\mu\in$ Sp(R($x$)). Comme R n’est pas constante, $P-\mu Q$ n’est pas le polynôme nul ; soit $\mu Q-P =\alpha \prod(\lambda_i-X)$ une décomposition en facteurs de degré 1, de sorte que $\mu e-R(x) =$ $\alpha \prod(\lambda_ie-x)Q(x)^{-1}$. Puisque $\mu e-R(x)$ n’est pas inversible, il existe $i$ tel que $\lambda_ie-x$ n’est pas inversible, donc $\lambda_i\in$ Sp($x$), puis $R(\lambda_i) =\mu\in$ R(Sp($x$)).

Lorsque R est constante, l’égalité Sp(R($x$)) $=$ R(Sp($x$)) vaut aussi, à condition que Sp($x$) soit non vide.

#### Remarque 5 {#ts-i-s1-n2-rem-5 .statement tag=024X}

Supposons que l’algèbre A soit non nulle. Soit $x\in A$ un élément nilpotent. Notons $n$ un entier tel que $x^n= 0$. Le spectre de $x^n$ est réduit à 0, donc il en est de même du spectre de $x$ d’après la remarque 4.

#### Remarque 6 {#ts-i-s1-n2-rem-6 .statement tag=024Y}

Soient A et B des algèbres unifères sur K et $\varphi : A\rightarrow B$ un morphisme unifère. Pour tout $x\in A$, on a Sp$_B(\varphi (x))\subset$ Sp$_A(x)$.

#### Remarque 7 {#ts-i-s1-n2-rem-7 .statement tag=024Z}

Soient A une algèbre unifère, R son radical (A, VIII, p. 150, déf. 2) et soit $\varphi$ le morphisme canonique de A sur $B = A/R$. Si $x\in A$, on a Sp$_B(\varphi (x)) =$ Sp$_A(x)$. En effet, il suffit de prouver que si $\varphi (x)$ est inversible dans B, alors $x$ est inversible dans A. Or, si $y\in A$ est tel que $\varphi (x)\varphi (y) =\varphi (y)\varphi (x) =\varphi (e)$, on a $xy\in e+ R,yx\in e+ R$, donc $xy$ et $yx$ sont inversibles (A, VIII, p. 151, th. 1) et par suite $x$ est inversible. En particulier, si $x\in R$, on a Sp$_A(x) =\{0\}$ si $A\not=\{0\}$.

#### Remarque 8 {#ts-i-s1-n2-rem-8 .statement tag=0250}

Soit $(B_i)_{i\in I}$ une famille d’algèbres unifères, avec $B_i= (A_i, e_i)$ pour $i\in I$. Posons $A =\prod_iA_i,e= (e_i)_{i\in I}$. Alors $(A, e)$ est une algèbre unifère appelée produit des $B_i$. Si $x= (x_i)_{i\in I}\in A$, on a Sp$_A(x) =\bigcup_i$ Sp$_{A_i}(x_i)$.

#### Exemple 1 {#ts-i-s1-n2-exa-1 .statement tag=0251}

Soit X un ensemble et soit $A = K^X$ l’algèbre des fonctions à valeurs dans K définies sur X. Le spectre d’un élément $f$ de A est l’ensemble des valeurs de $f$.

#### Exemple 2 {#ts-i-s1-n2-exa-2 .statement tag=0252}

Soit A une algèbre unifère de rang fini sur K. Pour que $x\in A$ soit inversible, il faut et il suffit que l’application linéaire $y\mapsto xy$ de A dans A soit de déterminant non nul. Il en résulte que le spectre de $x$ est l’ensemble des racines du polynôme caractéristique de $x$ (A, III, p. 110). Si A est l’algèbre des endomorphismes d’un espace vectoriel V de dimension finie sur K, le spectre de $x$ est donc l’ensemble des valeurs propres de $x$. Il n’en est pas toujours ainsi quand V est de dimension infinie (cf. I, p. 153, exercice 2).

### 3. Résolvante

#### Définition 2 {#ts-i-s1-def-2 .statement tag=0253}

Soient A une algèbre unifère sur K et $x\in A$. Pour tout $\lambda \in K$ - Sp($x$), on pose

$$
R(x, \lambda ) = (\lambda e-x)^{-1}
$$

L’application de K - Sp($x$) dans A donnée par $\lambda \mapsto R(x, \lambda )$ s’appelle la résolvante de $x$.

Pour $x$ fixé, les valeurs de $R(x, \lambda )$ sont deux à deux permutables. Si $\lambda , \mu\in K$, on a :

$$
(\lambda -\mu)e= (\lambda e-x)-(\mu e-x)
$$

donc, si $\lambda , \mu\in K$ - Sp($x$), on a la relation

$$
(\lambda -\mu)R(x, \lambda )R(x, \mu) = R(x, \mu)-R(x, \lambda ) \tag{1}
$$

Si $x, y\in A$ et $\lambda \in K$, on a :

$$
y-x= (\lambda e-x)-(\lambda e-y)
$$

donc, si $\lambda \in K$ - (Sp($x$)$\cup$ Sp($y$)), on a la relation

$$
R(y, \lambda )(y-x)R(x, \lambda ) = R(y, \lambda )-R(x, \lambda ) \tag{2}
$$

### 4. Spectre d’un élément dans une algèbre

Soit A une algèbre sur K. Rappelons (A, III, p. 4) qu’on définit sur l’espace vectoriel $\widetilde{A} = K\times A$ une structure d’algèbre telle que :

$$
(\lambda , a)(\mu, b) = (\lambda \mu, \lambda b+\mu a+ab)
$$

Soit $e= (1,0)$. Alors $(\widetilde{A}, e)$ est une algèbre unifère dite déduite de A par adjonction d’un élément unité. L’algèbre A s’identifie à l’idéal bilatère $\{0\} \times A$ de $\widetilde{A}$; l’algèbre A est commutative si et seulement si $\widetilde{A}$ l’est.

Si $A'$ est une seconde algèbre sur K, $(\widetilde{A}', e')$ l’algèbre unifère déduite de $A'$ par adjonction d’un élément unité, et $\varphi$ un morphisme de A dans $A'$, il existe un morphisme unifère et un seul de $(\widetilde{A}, e)$ dans $(\widetilde{A}', e')$ qui prolonge $\varphi$.

Soient A une algèbre sur K et $x\in$ A. On appelle spectre de $x$ relativement à A le spectre de $x$ relativement à l’algèbre unifère $\widetilde{A}$ déduite de A par adjonction d’un élément unité. Cet ensemble sera noté Sp$'_A(x)$, ou Sp$'(x)$ si aucune confusion n’en résulte. On a $0\in$ Sp$'_A(x)$ quel que soit $x\in A$.

Si $\varphi$ est un morphisme de A dans une algèbre B, on a Sp$'_B(\varphi (x))\subset$ Sp$'_A(x)$.

#### Remarque 1 {#ts-i-s1-n4-rem-1 .statement tag=0254}

Soit $(A,1)$ une algèbre unifère. Si $x\in A$, on a

Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. On vérifie en effet que $(e-1)\cdot A = A\cdot (e-1) = 0$, donc que $\widetilde{A}$ est l’algèbre unifère produit de A et de $K(e-1)$. Notre assertion résulte donc de la remarque 8 de I, p. 3.

#### Remarque 2 {#ts-i-s1-n4-rem-2 .statement tag=0255}

Il résulte de la remarque 1 que, si B est une algèbre sur K et si $x\in B$, on a :

Sp$'_B(x) =$ Sp$_{\widetilde{B}}(x) =$ Sp$_{\widetilde{B}}(x)\cup  \{0\}=$ Sp$'_{\widetilde{B}}(x)$.

#### Remarque 3 {#ts-i-s1-n4-rem-3 .statement tag=0256}

Si $x$ appartient au radical de A (A, VIII, p. 430, déf. 3), on a Sp$'_A(x) =\{0\}$. Ceci résulte de la remarque 7 de I, p. 3.

#### Proposition 1 {#ts-i-s1-prop-1 .statement tag=0257}

Soient A une algèbre et $x, y\in A$. On a Sp$'(xy) =$ Sp$'(yx)$.

En passant à $\widetilde{A}$, on se ramène au cas où A possède un élément unité $e$. Il suffit alors de prouver que, si $\lambda \not= 0$ est tel que $xy-\lambda e$ admette un inverse $u$, alors $yx-\lambda e$ est inversible. Posons $z=yux-e$. Puisque $xyu=\lambda u+e$, on a

$$
(yx-\lambda e)z=y(xyu)x-yx-\lambda yux+\lambda e
$$

$$
=y(\lambda u+e)x-yx-\lambda yux+\lambda e=\lambda e
$$

et de même $z(yx-\lambda e) =\lambda e$. Comme $\lambda \not= 0$, on voit que $yx-\lambda e$ est inversible.

Si A est une algèbre unifère et si $x, y\in A$, la proposition précédente entraîne que Sp($xy$)$\cup \{0\}=$ Sp($yx$)$\cup \{0\}$, mais on peut avoir Sp($xy$)$\not=$ Sp($yx$) (cf. I, p. 153, exerc. 3).

### 5. Sous-algèbres pleines

Soit A une algèbre unifère sur K.

#### Définition 3 {#ts-i-s1-def-3 .statement tag=0258}

On appelle sous-algèbre pleine de A une sous-algèbre unifère B telle que tout élément de B qui est inversible dans A soit inversible dans B.

Autrement dit, B est une sous-algèbre pleine de A si et seulement si Sp$_B(x) =$ Sp$_A(x)$ pour tout $x\in B$.

L’intersection d’une famille de sous-algèbres pleines de A est une sous-algèbre pleine de A.

Soit M une partie de A. L’intersection des sous-algèbres pleines de A contenant M est la plus petite sous-algèbre pleine de A contenant M ; on l’appelle la sous-algèbre pleine de A engendrée par M. Le commutant $M'$ de M dans A est une sous-algèbre pleine de A (car, si $x$ est inversible dans A et commute avec M, alors $x^{-1}$ commute avec M). Donc le bicommutant $M''$ de M est une sous-algèbre pleine de A qui contient la sous-algèbre pleine de A engendrée par M.

Si les éléments de M sont deux à deux permutables, on a $M\subset M'$ et $M''\subset M'''$; l’algèbre $M''$ est donc commutative et il en est alors de même de l’algèbre pleine engendrée par M.

Une sous-algèbre commutative maximale de A est une sous-algèbre pleine, car elle est égale à son commutant.

#### Lemme 2 {#ts-i-s1-lem-2 .statement tag=0259}

Soit $(x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments deux à deux permutables de A. La sous-algèbre pleine engendrée par $(x_{\lambda})$ est l’ensemble des éléments de la forme $R((x_{\lambda}))$, où $R\in K((X_{\lambda}))$ parcourt l’ensemble des fractions rationnelles dans lesquelles la famille $(x_{\lambda})$ est substituable.

Soit B la sous-algèbre pleine de A engendrée par la famille $(x_{\lambda})$, et notons $B_1$ l’ensemble des éléments de la forme $R((x_{\lambda}))$, où $R((X_{\lambda}))$ est une fraction rationnelle dans laquelle $(x_{\lambda})$ est substituable. Explicitement, $B_1$ est l’ensemble des éléments de A de la forme $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$, où $P,Q\in K[(X_{\lambda})]$ et $Q((x_{\lambda}))$ est inversible dans A. L’ensemble $B_1$ est une sous-algèbre unifère de A contenant la famille $(x_{\lambda})$. C’est une sous-algèbre pleine : si $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ est inversible dans A, alors $P((x_{\lambda}))$ est inversible dans A et l’inverse $Q((x_{\lambda}))P((x_{\lambda}))^{-1}$ de $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ appartient à $B_1$. On a donc $B\subset B_1$. D’autre part, si $P,Q\in K[(X_{\lambda})]$, et si $Q((x_{\lambda}))$ est inversible dans A, alors $P((x_{\lambda}))\in B$ et $Q((x_{\lambda}))\in B$, donc $Q((x_{\lambda}))^{-1}\in B$ et $P((x_{\lambda}))Q((x_{\lambda}))^{-1}\in B$, donc $B_1\subset B$.

### 6. Caractères d’une algèbre unifère commutative

#### Définition 4 {#ts-i-s1-def-4 .statement tag=025A}

Soit A une algèbre unifère commutative sur K. On appelle caractère unifère un morphisme unifère de A dans K.

Lorsqu’aucune confusion ne peut en résulter, on dira simplement caractère au lieu de caractère unifère. L’ensemble des caractères unifères de A est noté $\mathsf{X}(A)$. Si A est l’algèbre nulle, alors $\mathsf{X}(A)$ est vide.

Soient A et B des algèbres unifères commutatives sur K et $h$ un morphisme unifère de A dans B. L’application $\chi \mapsto \chi \circ h$ de $\mathsf{X}(B)$ dans $\mathsf{X}(A)$ se note $\mathsf{X}(h)$. Si $k$ est un morphisme de B dans une algèbre unifère commutative, on a $\mathsf{X}(k\circ h) =\mathsf{X}(h)\circ \mathsf{X}(k)$. L’application $\mathsf{X}$(Id$_A)$ est l’application identique de $\mathsf{X}(A)$.

Si $h$ est surjectif, $\mathsf{X}(h)$ est une bijection de $\mathsf{X}(B)$ sur l’ensemble des caractères de A qui s’annulent sur le noyau de $h$.

Soient $(A_1, e_1), . . . ,(A_n, e_n)$ des algèbres unifères commutatives sur K et soit A l’algèbre unifère $A_1\times  \cdots  \times A_n$, d’élément unité $(e_1, . . . , e_n)$. Pour tout $i$, identifions $A_i$ à un idéal de A et soit $\pi_i$ l’application canonique de A sur $A_i$. Alors $\mathsf{X}(\pi_i)$ est une bijection de $\mathsf{X}(A_i)$ sur l’ensemble $\mathsf{X}_i$ des caractères de A nuls sur $\prod_{j\not=i}A_j$. Les ensembles $\mathsf{X}_i$ sont deux à deux disjoints. D’autre part, soit $\chi \in \mathsf{X}(A)$. Puisque $1 =\sum\chi (e_i)$, il existe $i$ tel que $\chi (e_i)\not= 0$. Pour tout $j\not=i$ et tout $y\in A_j$, on a $\chi (e_i)\chi (y) =\chi (e_iy) =\chi (0) = 0$, donc $\chi (A_j) = 0$. Ainsi, $\chi$ s’annule sur $\prod_{j\not=i}A_j$, de sorte que $\mathsf{X}(A)$ est réunion des $\mathsf{X}_i$.

Soit B l’algèbre unifère $A_1\otimes  \cdots  \otimes A_n$. Notons $h_i$ le morphisme canonique $A_i\rightarrow B$. Alors

$$
\chi \mapsto (\chi \circ h_1, . . . , \chi \circ h_n)
$$

est une application de $\mathsf{X}(B)$ dans $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$, et

$$
(\chi_1, . . . , \chi_n)\mapsto \chi_1\otimes  \cdots  \otimes \chi_n
$$

est une application de $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$ dans $\mathsf{X}(B)$. On vérifie que ces applications sont des bijections réciproques l’une de l’autre, par lesquelles on identifiera $\mathsf{X}(B)$ à $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

Soit A une algèbre unifère commutative sur K. Soit Y l’ensemble des idéaux de codimension 1 de A. Pour tout $\chi \in \mathsf{X}(A)$, on a Ker($\chi$ )$\in Y$. L’application $\chi \mapsto$ Ker($\chi$ ) est une bijection de $\mathsf{X}(A)$ sur Y. En effet, si $I\in Y$, il existe un unique isomorphisme de la K-algèbre unifère $A/I$ sur K et le morphisme composé

$$
A\longrightarrow A/I\longrightarrow K
$$

est l’unique caractère de A de noyau I.

#### Définition 5 {#ts-i-s1-def-5 .statement tag=025B}

Soit A une algèbre unifère commutative sur K. Pour tout $x\in A$, on note $\mathscr{G}_A(x)$, ou simplement $\mathscr{G}(x)$, l’application $\chi \mapsto$ $\chi (x)$ de $\mathsf{X}(A)$ dans K. On l’appelle la transformée de Gelfand de $x$.

L’application $\mathscr{G}$ est un morphisme unifère de A dans l’algèbre unifère $K^{\mathsf{X}(A)}$ des applications de $\mathsf{X}(A)$ dans K. On l’appelle la transformation de Gelfand de A.

Si $x\in$ A, l’image de la transformée de Gelfand $\mathscr{G}_A(x)$ de $x$ est contenue dans Sp$_A(x)$. En effet, soit $\chi \in \mathsf{X}(A)$ ; puisque $\chi (x-\chi (x)e) =$ 0, l’élément $x-\chi (x)e$ n’est pas inversible.

Soient B une algèbre unifère commutative sur K et $h$ un morphisme unifère de A dans B ; alors $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ définit un morphisme unifère $h_*: K^{\mathsf{X}(A)}\rightarrow K^{\mathsf{X}(B)}$, et le diagramme :

$\mathscr{G}\leftarrow_A\mathsf{X}(A)$

A $\rightarrow K$ (3) $\rightarrow \leftarrow_h\rightarrow \leftarrow_{h_*}$

$\mathscr{G}\leftarrow_B\mathsf{X}(B)$

B $\rightarrow K$

est commutatif. En effet, pour tout $x\in A$ et tout $\chi \in \mathsf{X}(B)$, on a :

$$
\mathscr{G}_B(h(x))(\chi ) =\chi (h(x)) = (\chi \circ h)(x)
$$

$$
= (\mathsf{X}(h)(\chi ))(x)
$$

$$
=\mathscr{G}_A(x)(\mathsf{X}(h)(\chi )) \tag{4}
$$

$$
=h_*(\mathscr{G}_A(x))(\chi )
$$

Supposons maintenant que K soit un corps topologique. On munit alors $\mathsf{X}(A)$ de la topologie de la convergence simple sur A (cf. EVT, III, p. 14, exemple 1), et l’espace topologique $\mathsf{X}(A)$ s’appelle l’espace des caractères de A. La topologie de $\mathsf{X}(A)$ est donc la moins fine pour laquelle les fonctions $\mathscr{G}_A(x)$ pour $x\in A$ soient continues, et l’application $\chi \mapsto (\chi (a))_{a\in A}$ identifie l’espace $\mathsf{X}(A)$ avec une partie de $K^A$.

Lorsque K = $\mathbf{R}$ ou $\mathbf{C}$, cette topologie est la topologie induite sur $\mathsf{X}(A)\subset A^*$ par la topologie faible $\sigma (A^*,A)$ sur $A^*$ (EVT, II, p. 45, déf. 2) ; à ce titre, nous dirons aussi que c’est la topologie faible sur $\mathsf{X}(A)$.

Si $h$ est un morphisme unifère de A dans B, l’application $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ est continue. Si $h$ est surjectif, l’image de $\mathsf{X}(h)$, à savoir l’ensemble des caractères de A nuls sur le noyau de $h$, est fermée dans $\mathsf{X}(A)$ ; d’autre part, la topologie sur $\mathsf{X}(h)(\mathsf{X}(B))$ déduite de celle de $\mathsf{X}(B)$ par la bijection $\mathsf{X}(h)$ est la topologie de la convergence simple dans A, c’est-à-dire la topologie induite par celle de $\mathsf{X}(A)$ ; autrement dit, $\mathsf{X}(h)$ est un homéomorphisme de $\mathsf{X}(B)$ sur une partie fermée de $\mathsf{X}(A)$.

Si $A_1, . . . ,A_n$ sont des algèbres unifères commutatives sur K, l’espace $\mathsf{X}(A_1\times  \cdots  \times A_n)$ s’identifie ainsi à l’espace topologique somme de $\mathsf{X}(A_1), . . . ,\mathsf{X}(A_n)$. De même, $\mathsf{X}(A_1\otimes  \cdots  \otimes A_n)$ s’identifie à l’espace topologique produit $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

### 7. Cas des algèbres sans élément unité

#### Définition 6 {#ts-i-s1-def-6 .statement tag=025C}

Soit A une algèbre commutative sur K. On appelle caractère de A un morphisme d’algèbres de A dans K.

L’ensemble des caractères de A sera noté $\mathsf{X}'(A)$.

L’application nulle est un morphisme d’algèbres. Si A possède un élément unité $e$, un morphisme d’algèbres non nul de A dans K est unifère, c’est-à-dire est un caractère unifère de K au sens de la définition 4 : en effet, pour que $\chi \in \mathsf{X}'(A)$ soit non nul, il faut et il suffit que $\chi (e) = 1$.

On posera $\mathsf{X}(A) =\mathsf{X}'(A)-\{0\}$; d’après ce qui précède, la notation est compatible avec celle introduite lorsque A est unifère.

Si $h: A\rightarrow B$ est un morphisme d’algèbres commutatives, l’application $\chi \mapsto \chi \circ h$ est une application $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow \mathsf{X}'(A)$. Elle transforme 0 en 0. Si $k: B\rightarrow C$ est un morphisme d’algèbres commutatives, alors on a $\mathsf{X}'(k\circ h) =\mathsf{X}'(h)\circ \mathsf{X}'(k)$. Si $h$ est surjectif, $\mathsf{X}'(h)$ est une bijection de $\mathsf{X}'(B)$ sur l’ensemble des caractères de A nuls sur le noyau de $h$. Soient $A_1, . . . ,A_n$ des algèbres commutatives, $A = A_1\times  \cdots  \times A_n$ et $\pi : A\rightarrow A_i$ le morphisme canonique ; alors $\mathsf{X}'(\pi_i)$ est une bijection de $\mathsf{X}'(A_i)$ sur une partie $\mathsf{X}'_i$ de $\mathsf{X}'(A)$, à savoir l’ensemble des caractères de A nuls sur $\prod_{j\not=i}A_j$; on voit comme au n$^o6$ que $\mathsf{X}'(A)$ est réunion

des $\mathsf{X}'_i$; d’autre part, $\mathsf{X}'_i\cap \mathsf{X}'_j=\{0\}$ pour $i\not=j$; en particulier les $\mathsf{X}'_i-\{0\}$ forment une partition de $\mathsf{X}'(A)-\{0\}=\mathsf{X}(A)$.

Pour tout $x\in A$, soit $\mathscr{G}'_A(x)$, ou simplement $\mathscr{G}'(x)$, l’application $\chi \mapsto \chi (x)$ de $\mathsf{X}'(A)$ dans K. L’application $\mathscr{G}'$ est un morphisme de A dans l’algèbre $A_1$ des applications $\mathsf{X}'(A)\rightarrow K$ nulles en 0. Soient B une algèbre commutative, $B_1$ l’algèbre des applications $\mathsf{X}'(B)\rightarrow$ K nulles en 0, et $h$ un morphisme de A dans B; alors $\mathsf{X}'(h)$ définit un morphisme $h_1: A_1\rightarrow B_1$, et l’on a $h_1\circ \mathscr{G}'_A=\mathscr{G}'_B\circ h$. On note $\mathscr{G}_A(x)$, ou simplement $\mathscr{G}(x)$, la restriction de $\mathscr{G}'_A(x)$ à $\mathsf{X}(A)$ et on l’appelle transformée de Gelfand de $x$.

Soit $\widetilde{A}$ l’algèbre unifère déduite de A par adjonction d’un élément unité. Par restriction, tout caractère de $\widetilde{A}$ définit un caractère de A ; inversement, tout caractère de A se prolonge de manière unique en un caractère de $\widetilde{A}$. Cela définit une bijection canonique de $\mathsf{X}'(A)$ sur $\mathsf{X}(\widetilde{A})$, par laquelle on identifie ces deux ensembles. Le caractère 0 de A s’identifie à l’unique caractère de $\widetilde{A}$ de noyau A.

Si $x\in A$ et $\chi \in \mathsf{X}'(A)$, on a $\chi (x)\in$ Sp$_{\widetilde{A}}(x)$, donc $\chi (x)\in$ Sp$'_A(x)$.

#### Lemme 3 {#ts-i-s1-lem-3 .statement tag=025D}

L’application $\chi \mapsto$ Ker($\chi$ ) est une bijection de $\mathsf{X}(A)$ sur l’ensemble des idéaux réguliers de codimension 1 de A.

Rappelons (A, VIII, p. 426, déf. 1) qu’un idéal I de A est dit régulier si l’algèbre quotient $A/I$ admet un élément unité.

Démontrons le lemme. D’une part $\mathsf{X}(A)$ s’identifie à l’ensemble des caractères de $\widetilde{A}$ non nuls sur A. D’autre part, d’après A, VIII, p. 428, prop. 4, l’application $I\mapsto A\cap I$ est une bijection de l’ensemble des idéaux maximaux de $\widetilde{A}$ distincts de A sur l’ensemble des idéaux maximaux réguliers de A. Le lemme découle alors des résultats du n$^o6$.

Supposons maintenant que K soit un corps topologique. On munit alors $\mathsf{X}'(A)$ de la topologie de la convergence simple sur A ; la notation $\mathsf{X}'(A)$ désignera désormais l’espace topologique ainsi obtenu. Lorsque $K =\mathbf{R}$ ou $\mathbf{C}$, nous l’appelerons également topologie faible. Pour tout $x\in A$, la fonction $\mathscr{G}'_A(x)$ sur $\mathsf{X}'(A)$ est continue.

Si $h$ est un morphisme de A dans B, l’application $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow$ $\mathsf{X}'(A)$ est continue. Si $h$ est surjectif, $\mathsf{X}'(h)$ est un homéomorphisme de $\mathsf{X}'(B)$ sur son image et cette image est fermée dans $\mathsf{X}'(A)$.

Soit $A = A_1\times  \cdots  \times A_n$; avec les mêmes notations que plus haut, $\mathsf{X}'(\pi_i)$ est un homéomorphisme de $\mathsf{X}'(A_i)$ sur $\mathsf{X}'_i$ et $\mathsf{X}'_i$ est fermé dans $\mathsf{X}'(A)$. Donc $\mathsf{X}'_i-\{0\}$ est ouvert dans $\mathsf{X}'(A)$ ; les $\mathsf{X}'(\pi_i)$ définissent une application continue de l’espace somme S des $\mathsf{X}'(A_i)$ sur $\mathsf{X}'(A)$, et on vérifie immédiatement qu’une réunion de voisinages des points $0\in \mathsf{X}'(A_1), . . . ,0\in \mathsf{X}'(A_n)$ a pour image un voisinage de $0\in \mathsf{X}'(A)$ ; de tout ceci résulte que $\mathsf{X}'(A)$ s’identifie canoniquement à un espace quotient de S. En particulier, l’espace $\mathsf{X}(A)$ s’identifie à l’espace somme des $\mathsf{X}(A_i)$.

La bijection canonique de $\mathsf{X}'(A)$ sur $\mathsf{X}(\widetilde{A})$ est un homéomorphisme. Soient B une algèbre unifère sur K et $B'$ l’algèbre sous-jacente ; alors l’espace $\mathsf{X}(B)$ s’identifie au sous-espace $\mathsf{X}(B')$ de $\mathsf{X}'(B')$.

### 8. Idéaux primitifs

Soient A une algèbre sur K et E un espace vectoriel sur K. On appelle représentation de A dans E un morphisme de A dans l’algèbre $\mathscr{L}(E)$ des endomorphismes de E. Une représentation injective est dite fidèle. Soient $\pi_1$ et $\pi_2$ des représentations de A dans des espaces $E_1,E_2$. Un morphisme de $\pi_1$ dans $\pi_2$ est une application K-linéaire $u: E_1\rightarrow E_2$ telle que $u(\pi_1(a)x) =\pi_2(a)u(x)$ pour tous $a\in A$ et $x\in E_1$. Les représentations sont dites équivalentes s’il existe un morphisme de $\pi_1$ dans $\pi_2$ qui est un isomorphisme d’espaces vectoriels. Son inverse est alors un morphisme de $\pi_2$ dans $\pi_1$. Une représentation $\pi$ de A dans E est dite irréductible si $E\not=\{0\}$ et si les seuls sous-espaces vectoriels de E stables pour $\pi (A)$ sont $\{0\}$ et E.

#### Exemple {#ts-i-s1-n8-exa-1 .statement tag=025E}

L’application nulle de A dans $\mathscr{L}(E)$ est une représentation, dite triviale, de A. Elle est irréductible si seulement si E est de dimension 1.

#### Lemme 4 {#ts-i-s1-lem-4 .statement tag=025F}

Soit $\pi$ une représentation irréductible, non triviale, de A dans E. Pour tout élément $\xi$ non nul de E, on a $\pi (A)\xi = E$.

Le sous-espace $\pi (A)\xi$ de E est stable pour $\pi (A)$. Supposons qu’il soit nul. Le sous-espace non nul $K\xi$ de E serait alors stable par $\pi (A)$, et donc égal à E ; mais cela impliquerait que $\pi$ est la représentation nulle. On a donc $\pi (A)\xi = E$.

Soit $\pi$ une représentation irréductible, non triviale, de A dans E. D’après ce lemme, l’annulateur R de $\xi$ dans A est un idéal à gauche régulier (A, VIII, p. 425, n$^o1)$ de A, et la représentation $\pi$ est équivalente à la représentation définie par le A-pseudomodule $A/R$. Comme $\pi$ est irréductible, l’idéal R est un idéal à gauche maximal régulier.

#### Définition 7 {#ts-i-s1-def-7 .statement tag=025G}

Soit A une algèbre sur K. On appelle idéal primitif de A le noyau d’une représentation irréductible non triviale de A.

Si A est commutative, les idéaux primitifs de A sont les idéaux maximaux réguliers de A. En effet, les représentations irréductibles non triviales de A sont, à une équivalence près, les représentations $\pi_R$ définies par les A-pseudomodules $A/R$, où R est un idéal maximal régulier de A. Le noyau de $\pi_R$ contient R. Il lui est même égal puisque, d’après A, VIII, p. 426, prop. 2, la commutativité de A entraîne que $A/R$ est un corps. Donc Ker($\pi_R$) est maximal régulier.

#### Lemme 5 {#ts-i-s1-lem-5 .statement tag=025H}

Soit $\pi$ une représentation irréductible de A dans un espace vectoriel E sur K.

a) Soit I un idéal bilatère de A. Si $\pi (I)\not=\{0\}$, alors $\pi |I$ est irréductible;

b) Soient $I_1$ et $I_2$ des idéaux bilatères de A tels que $\pi (I_1)\not= 0$ et $\pi (I_2)\not= 0$. Alors $\pi (I_1I_2)\not= 0$.

L’ensemble des éléments de E annulés par $\pi (I)$ est stable pour $\pi (A)$ et distinct de E, donc égal à 0. Donc, si $\xi$ est un élément non nul de E, on a $\pi (I)\xi \not= 0$ ; comme $\pi (I)\xi$ est stable pour $\pi (A)$, on a $\pi (I)\xi = E$, ce qui prouve a). D’autre part, ce qui précède prouve que $\pi (I_2)E = E$, $\pi (I_1)\pi (I_2)E = E$, donc $\pi (I_1I_2)\not= 0$, d’où b).

#### Lemme 6 {#ts-i-s1-lem-6 .statement tag=025I}

Soient $I_1$ et $I_2$ des idéaux bilatères de A, I un idéal primitif de A. Si I contient $I_1I_2($en particulier, si I contient $I_1\cap I_2)$, alors I contient $I_1$ ou $I_2$.

Soit $\pi$ une représentation irréductible de noyau I. Si $I\not\supset I_1$ et $I\not\supset I_2$, le lemme 5, b) prouve que $\pi (I_1I_2)\not= 0$, d’où $I\not\supset I_1I_2$.

#### Lemme 7 {#ts-i-s1-lem-7 .statement tag=025J}

Supposons que A admette un élément unité. Soit I un idéal bilatère maximal de A. Alors I est un idéal primitif.

Il existe un idéal à gauche maximal R de A contenant I (A, I, p. 99, th. 1). Soit $\pi$ la représentation canonique de A dans $A/R$, qui est irréductible et non nulle. Comme IA $\subset R$, le noyau $I'$ de $\pi$ contient I, donc $I'= I$ et I est primitif.

Soit J(A) l’ensemble des idéaux primitifs de A. Pour toute partie M de A, nous noterons V(M) l’ensemble des idéaux primitifs de A contenant M; si I est l’idéal bilatère de A engendré par M, on a V(M) = V(I). Si M est réduit à un seul élément $x$, on écrira $V(x)$ au lieu de $V(\{x\})$. L’application $M\mapsto V(M)$ est décroissante pour les relations d’inclusion. On a :

$$
V(\emptyset ) = J(A),V(A) =\emptyset \tag{5}
$$

$$
V(\bigcup_{i\in I}M_i)= V(\sum_{i\in I}M_i)=\bigcap_{i\in I}V(M_i) \tag{6}
$$

pour toute famille $(M_i)_{i\in I}$ de parties de A. D’autre part, d’après le lemme 6,

$$
V(I_1\cap I_2) = V(I_1I_2) = V(I_1)\cup V(I_2) \tag{7}
$$

pour tous idéaux bilatères $I_1,I_2$ de A. Les formules (5) à (7) démontrent que les parties V(M) de J(A) sont les parties fermées d’une topologie appellée la topologie de Jacobson sur J(A).

Soit T une partie de J(A) et soit Υ(T) l’intersection des éléments de T, de sorte que Υ(T) est un idéal bilatère de A. Alors l’adhérence de T dans J(A) est la plus petite partie fermée de J(A) contenant T, c’est-à-dire V(Υ(T)). En particulier, T est fermée si et seulement si T = V(Υ(T)).

#### Proposition 2 {#ts-i-s1-prop-2 .statement tag=025K}

Soient $I_1$ et $I_2$ des points distincts de J(A). Alors l’un de ces deux points est non adhérent à l’autre.

En effet, on a par exemple $I_1\not\subset I_2$. L’ensemble $V(I_1)$ des $I\in J(A)$ tels que $I_1\subset I$ est fermé dans J(A), et il contient $I_1$ mais pas $I_2$.

#### Proposition 3 {#ts-i-s1-prop-3 .statement tag=025L}

Soit $I\in J(A)$. Pour que $\{I\}$ soit fermé dans J(A), il faut et il suffit que I soit un idéal primitif maximal.

En effet, l’adhérence de $\{I\}$ se compose des idéaux primitifs de A contenant I.

La relation

« $\pi_1,\pi_2$ sont des représentations de A, qui sont isomorphes »

est une relation d’équivalence par rapport à $\pi_1$ et $\pi_2$. Pour toute représentation $\pi$ de A, on notera cl($\pi$ ) la classe d’équivalence de $\pi$, qui est donc une représentation de A isomorphe à $\pi$, telle que deux représentations $\pi_1$ et $\pi_2$ sont isomorphes si et seulement si cl($\pi_1$) $=$ cl($\pi_2$). On dit que cl($\pi$ ) est la classe de $\pi$.

Soit $\mathfrak{c}$ le cardinal de A. Soit $\pi$ une représentation irréductible non nulle de A dans un K-espace vectoriel E. Soit $\xi$ un élément non nul de E. Puisque $\pi (A)\xi = E$ (lemme 4), la dimension de E est $\leqslant \mathfrak{c}$ (A, II, p. 97, corollaire). La relation

« $\lambda$ est une classe de représentations irréductibles de A

dans un K-espace vectoriel de dimension $\leqslant \mathfrak{c}$ »

est collectivisante en $\lambda$ (E, II, p. 3). En effet, tout espace vectoriel de dimension $\leqslant \mathfrak{c}$ est isomorphe à un espace $K^B$ où B est une partie de A (A, II, p. 25, déf. 10), et l’assertion résulte alors de E, II, p. 47.

On note $\widehat{A}$ l’ensemble des classes de représentations irréductibles, non triviales, de A. D’après ce qui précède, pour toute représentation irréductible non triviale $\pi$ de A, il existe une unique représentation $\widehat{\pi}\in \widehat{A}$ qui est isomorphe à $\pi$.

L’application de $\widehat{A}$ dans J(A) qui associe à $\pi$ son noyau est surjective. Si A est commutative, il résulte du fait que les idéaux primitifs sont les idéaux maximaux réguliers que cette application est une bijection.

On munit $\widehat{A}$ de la topologie image réciproque de celle de J(A) par l’application $\widehat{A}\rightarrow J(A)$.

#### Proposition 4 {#ts-i-s1-prop-4 .statement tag=025M}

Si A possède un élément unité, les espaces J(A) et $\widehat{A}$ sont quasi-compacts.

Il suffit de faire la démonstration pour J(A). Soit $(T_j)$ une famille de parties fermées de J(A) dont l”intersection est vide. Si la somme $\sum_j\Upsilon (T_j)$ était différente de A, alors cette somme serait contenue dans un idéal bilatère maximal I. L’idéal I serait primitif (lemme 7) ; comme la partie $T_j$ est fermée, donc égale à $V(\Upsilon (T_j))$, on aurait $I\in T_j$ pour tout $j$, ce qui contredit l’hypothèse. Ainsi on a $\sum_j\Upsilon (T_j) = A$, et donc on peut écrire $1 =x_1+\cdots +x_n$ avec $n\geqslant 1$ et $x_i\in \Upsilon (T_{j_i})$ pour tout $i$. Ceci entraîne que $\Upsilon (T_{j_1})+\cdots +\Upsilon (T_{j_n}) = A$, d’où $T_{j_1}\cap  \cdots  \cap T_{j_n}=\emptyset$.

Supposons l’algèbre A commutative et unifère. La topologie de Jacobson sur J(A) est la topologie induite sur J(A) par la topologie de Zariski du spectre premier de A (AC, II, déf. 4, p. 125).

Supposons que A est commutative et que K est un corps topologique. L’isomorphisme canonique de K sur $\mathscr{L}(K)$ permet d’identifier un élément de $\mathsf{X}(A)$ à une représentation de A dans l’espace vectoriel K, ce qui définit une application injective de $\mathsf{X}(A)$ dans $\widehat{A}$. On peut donc identifier $\mathsf{X}(A)$ à une partie de $\widehat{A}$.

#### Proposition 5 {#ts-i-s1-prop-5 .statement tag=025N}

La topologie induite sur $\mathsf{X}(A)$ par celle de $\widehat{A}$ est moins fine que la topologie de $\mathsf{X}(A)$.

En effet, soit T une partie fermée de $\widehat{A}$. Alors T est l’ensemble des $\pi \in \widehat{A}$ dont le noyau contient une partie M de A. Donc $T\cap \mathsf{X}(A)$ est l’ensemble des $\chi \in \mathsf{X}(A)$ qui s’annulent sur M, c’est-à-dire une partie fermée de $\mathsf{X}(A)$. D’où la proposition.

En général, la topologie de $\mathsf{X}(A)$ ne coïncide pas avec la topologie induite par la topologie de $\widehat{A}($cf. I, p. 193, exercice 6, c)).

## EXERCICES {#ts-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
