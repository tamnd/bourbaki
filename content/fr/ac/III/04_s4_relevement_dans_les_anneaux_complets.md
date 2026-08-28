---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: Graduations, filtrations et topologies
section: 4
section_title: Relèvement dans les anneaux complets
lang: fr
source: ac-i-iv-fr
pdf_pages: 0250-0270, 0299-0303
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes fortement étrangers.
      page: 0
      pdf_page: 250
    - "no": 2
      title: Séries formelles restreintes.
      page: 0
      pdf_page: 253
    - "no": 3
      title: Le lemme de Hensel.
      page: 0
      pdf_page: 257
    - "no": 4
      title: Composition des systèmes de séries formelles.
      page: 0
      pdf_page: 261
    - "no": 5
      title: Systèmes d’équations dans les anneaux complets.
      page: 0
      pdf_page: 263
    - "no": 6
      title: Application aux décompositions d'anneaux.
      page: 0
      pdf_page: 269
statements: 27
exercises: 6
content_sha256: 3ae60667ac59c964ae5e4bcb3db2bbf1df89e8dee0dd6c9ccb80a1a716f90200
---

## § 4. Relèvement dans les anneaux complets.

### 1. Polynômes fortement étrangers.

Soit $R$ un anneau commutatif. On dit que deux éléments $x, y$ de $R$ sont fortement étrangers si les idéaux principaux $Rx$ et $Ry$ sont étrangers, autrement dit (chap. II, § 1, no 2) si $Rx + Ry = R$; il revient au même de dire qu’il existe deux éléments $a, b$ de $R$ tels que $ax + by = 1$.

#### Lemme 1 (« lemme d’Euclide ») {#ac-iii-s4-lem-1 .statement}

Soient x, y deux éléments fortement étrangers dans R ; si z ∈ R est tel que x divise yz, alors x divise z.

En effet, si $1 = ax + by$, on a $z = x(az) + (yz)b$.

Si x et y sont fortement étrangers dans R, on a
$$
Rxy = (Rx) \cap (Ry)
$$
(chap. II, § 1, no 2, prop. 5); si R est intègre, deux éléments fortement étrangers ont donc un ppcm égal à leur produit (Alg., chap. VI, § 1, no 8) et sont par suite étrangers au sens de Alg., chap. VI, § 1, no 12. Réciproquement, si R est un anneau principal, deux éléments étrangers sont aussi fortement étrangers, comme il résulte de l’identité de Bezout (Alg., chap. VII, § 1, no 2, th. 1).

Dans les anneaux de polynômes, on a le résultat suivant :

#### Proposition 1 {#ac-iii-s4-prop-1 .statement}

Soient A un anneau commutatif, P et P’ deux polynômes fortement étrangers dans A[X]. On suppose que P est unitaire et de degré s. Alors tout polynôme T dans A[X] s’écrit d’une manière et d’une seule sous la forme
$$
T = PQ + P’Q’
$$
avec $Q \in A[X]$, $Q’ \in A[X]$ et $\deg(Q’) < s$.

Si de plus on a $\deg(T) \leq t$ et $\deg(P’) \leq t - s$, alors $\deg(Q) \leq t - s$.

Comme P est unitaire, on a PR ≠ 0 pour tout polynôme R ≠ 0 de A[X] et dans ce cas on a $\deg(PR) = s + \deg(R)$.

Soit T un polynôme quelconque dans A[X]. Comme l’idéal engendré par P et P’ est A[X] tout entier, il existe des polynômes Q₁ et Q₁’ tels que $T = PQ_1 + P’Q_1’$; comme P est unitaire de degré s, la division euclidienne (Alg., chap. IV, § 1, no 5) montre qu’il existe deux polynômes Q’, Q’’ tels que $Q_1’ = PQ’’ + Q’$ avec $\deg(Q’) < s$; on en déduit donc
$$
T = PQ_1 + P’(PQ’’ + Q’) = PQ + P’Q’
$$
avec $Q = Q_1 + P’Q’’$. Pour démontrer l’unicité dans la formule (1), il suffit de prouver que les relations
$$
0 = PQ + P’Q’, \quad \deg(Q’) < s
$$

impliquent $Q = Q' = 0$. Or, si (2) est vérifiée, P divise – PQ = P'Q', et comme P et P' sont fortement étrangers, P divise Q' en vertu du lemme 1 ; si on avait $Q' \neq 0$, il existerait un polynôme S $\neq 0$ tel que $Q' = PS$, d'où $\deg(Q') = s + \deg(S) \geq s$, ce qui est contradictoire. On en conclut $Q' = 0$, d'où $PQ = 0$ et finalement $Q = 0$ d'après la remarque du début.

Enfin, supposons que l'on ait $\deg(T) \leq t$ et $\deg(P') \leq t - s$; le polynôme T étant mis sous la forme (1), on a
$$
\deg(P'Q') \leq \deg(P') + \deg(Q') < s + \deg(P') \leq t
$$
et par suite
$$
s + \deg(Q) = \deg(PQ) = \deg(T - P'Q') \leq t
$$
d'où $\deg(Q) \leq t - s$.

#### Exemple {#ac-iii-s4-n1-exa-1 .statement}

Pour qu'un polynôme $P \in A[X]$ soit fortement étranger à $X - a$ (où $a \in A$), il faut et il suffit que $P(a)$ soit *inversible* dans A. En effet, si P et $X - a$ sont fortement étrangers, il résulte de la prop. 1 qu'il existe $c \in A$ et un polynôme $Q \in A[X]$ tels que $cP + (X - a)Q = 1$, d'où $cP(a) = 1$ et $P(a)$ est inversible. Réciproquement, on a, par division euclidienne
$$
P = (X - a)R + P(a),
$$
et si $P(a) = b^{-1}$, où $b \in A$, on en déduit $1 = bP - b(X - a)R$, ce qui montre que P et $X - a$ sont fortement étrangers.

Soient A et B deux anneaux commutatifs, $f : A \to B$ un homomorphisme d'anneaux. Si $P = \sum_{i \geq 0} a_i X^i$ est une série formelle dans $A[[X]]$, on désignera par $\overline{f}(P)$ la série formelle $\sum_{i \geq 0} f(a_i) X^i$ dans $B[[X]]$. Si P est un polynôme, il en est de même de $\overline{f}(P)$, et si de plus P est unitaire, alors $\overline{f}(P)$ est unitaire de même degré que P. Enfin, il est clair que $P \to \overline{f}(P)$ est un homomorphisme de $A[[X]]$ dans $B[[X]]$ qui prolonge $f$ et applique X sur X. *La notation* $\overline{f}$ *sera constamment utilisée dans ce sens dans le reste de ce paragraphe.*

#### Proposition 2 {#ac-iii-s4-prop-2 .statement}

Soient A et B deux anneaux commutatifs, f un homomorphisme de A dans B, P, P' deux polynômes dans A[X]. Si P et P' sont fortement étrangers dans A[X], alors $\bar{f}(P)$ et $\bar{f}(P')$ sont fortement étrangers dans B[X]. La réciproque est vraie si f est surjectif, si son noyau est contenu dans le radical de A, et si P est unitaire.

Supposons P et P' fortement étrangers ; il existe donc des polynômes Q, Q' dans A[X] tels que PQ + P'Q' = 1 ; on en déduit $\bar{f}(P)\bar{f}(Q) + \bar{f}(P')\bar{f}(Q') = 1$, d'où la première assertion. Pour démontrer la seconde, désignons par α le noyau de f ; posons E = A[X], et soit F l'idéal de E engendré par P et P' ; comme f est surjectif et $\bar{f}(P)$ unitaire, la prop. 1 montre que pour tout polynôme T $\in$ A[X], il existe deux polynômes Q, Q' dans A[X] tels que $\bar{f}(T) = \bar{f}(P)\bar{f}(Q) + \bar{f}(P')\bar{f}(Q')$, d'où la relation E = F + αE. Or, E/F est un A-module de type fini, car tout polynôme est congru mod. P à un polynôme de degré < deg(P), P étant unitaire. Comme E/F = α(E/F) et que α est contenu dans le radical de A, le lemme de Nakayama montre que E/F = 0 (Alg., chap. VIII, § 6, no 3, cor. 2 de la prop. 6), ce qui signifie que P et P' sont fortement étrangers.

### 2. Séries formelles restreintes.

#### Définition 1 {#ac-iii-s4-def-1 .statement}

On dit qu'un anneau topologique commutatif A est linéairement topologisé (et que sa topologie est linéaire) s'il existe un système fondamental $\mathcal{B}$ de voisinages de 0 formé d'idéaux de A.

On notera que dans un tel anneau, les idéaux $\mathfrak{J} \in \mathcal{B}$ sont ouverts et fermés (Top. gén., chap. III, 3e éd., § 2, no 1, cor. de la prop. 4). Pour tout $\mathfrak{J} \in \mathcal{B}$, l'anneau topologique quotient $A/\mathfrak{J}$ est donc discret ; pour $\mathfrak{J} \in \mathcal{B}$, $\mathfrak{J}' \in \mathcal{B}$, $\mathfrak{J}' \subset \mathfrak{J}$, soit $h_{\mathfrak{J}\mathfrak{J}'} : A/\mathfrak{J}' \to A/\mathfrak{J}$ l'application canonique. On sait (Top. gén., chap. III, 3e éd., § 7, no 3) que $(A/\mathfrak{J}, f_{\mathfrak{J}\mathfrak{J}'})$ est un système projectif d'anneaux discrets (relatif à l'ensemble d'indices $\mathcal{B}$, ordonné filtrant par la relation $\supset$), dont la limite projective est un anneau topologique $\tilde{A}$ linéairement topologisé, séparé et complet ; en outre (loc. cit., prop. 2), on définit un morphisme strict $i : A \to \tilde{A}$, dont le noyau est l’adhérence de $\{0\}$ dans $A$, et l’image est partout dense dans $\tilde{A}$, de sorte que $\tilde{A}$ s’identifie canoniquement au séparé complété de $A$.

#### Définition 2 {#ac-iii-s4-def-2 .statement}

Étant donné un anneau topologique commutatif $A$, on dit qu’une série formelle $T = \sum_{(n_i)} c_{n_1 n_2 \ldots n_p} X_1^{n_1} X_2^{n_2} \ldots X_p^{n_p}$ de l’anneau $A[[X_1, \ldots, X_p]]$ est restreinte si, pour tout voisinage $V$ de 0 dans $A$, il n’y a qu’un nombre fini de coefficients $c_{n_1 \ldots n_p}$ n’appartenant pas à $V$ (autrement dit, la famille $(c_{n_1 \ldots n_p})$ tend vers 0 dans $A$ suivant le filtre des complémentaires des parties finies de $\mathbf{N}^p$).

Si $A$ est linéairement topologisé, les séries formelles restreintes dans $A[[X_1, \ldots, X_p]]$ forment un sous-anneau de $A[[X_1, \ldots, X_p]]$, que l’on note $A\{X_1, \ldots, X_p\}$ : en effet, si $T = \sum_{(n_i)} c_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}$, $T' = \sum_{(n_i)} c'_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}$ sont deux séries formelles restreintes, $\mathfrak{J}$ un voisinage de 0 dans $A$ qui est un idéal de $A$, il existe un entier $m$ tel que $c_{n_1 \ldots n_p} \in \mathfrak{J}$ et $c'_{n_1 \ldots n_p} \in \mathfrak{J}$ pour tout système $(n_1, \ldots, n_p)$ tel que $n_k \geq m$ pour un indice $k$ au moins ; or, si
$$
T'' = TT' = \sum_{(n_i)} c''_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p},
$$
on a $c''_{n_1 \ldots n_p} = \sum c_{r_1 \ldots r_p} c'_{s_1 \ldots s_p}$ pour tous les systèmes $(r_k), (s_k)$ tels que $r_k + s_k = n_k$ pour $1 \leq k \leq p$ ; on en conclut que si $n_k \geq 2m$, on a $r_k \geq m$ ou $s_k \geq m$, donc, puisque $\mathfrak{J}$ est un idéal, $c''_{n_1 \ldots n_p} \in \mathfrak{J}$ dès que $n_k \geq 2m$ pour un $k$ au moins, ce qui établit notre assertion. En outre, toute dérivée $\partial T / \partial X_i$ ($1 \leq i \leq p$) d’une série formelle restreinte est restreinte, comme il résulte aussitôt de la définition et du fait que les voisinages $\mathfrak{J} \in \mathcal{B}$ sont des sous-groupes additifs de $A$.

Lorsque $A$ est discret, l’anneau des séries formelles restreintes n’est autre que l’anneau des polynômes $A[X_1, \ldots, X_p]$.

Supposons toujours $A$ linéairement topologisé, et soit $\mathcal{B}$ un système fondamental de voisinages de 0 dans $A$ formé d’idéaux de $A$;

pour tout $\mathfrak{J} \in \mathcal{B}$, soit $p_{\mathfrak{J}} : A \to A/\mathfrak{J}$ l’homomorphisme canonique. Par définition, pour toute série formelle restreinte $T \in A\{X_1,...,X_p\}$, on a $\bar{p}_{\mathfrak{J}}(T) \in (A/\mathfrak{J})[X_1,...,X_p]$. Il est clair que

$$
((A/\mathfrak{J})[X_1,...,X_p], \overline{h}_{\mathfrak{J}\mathfrak{J}'})
$$

est un système projectif d’anneaux (relatif à l’ensemble d’indices filtrant $\mathcal{B}$) et que $(\bar{p}_{\mathfrak{J}})$ est un système projectif d’homomorphismes $A\{X_1,...,X_p\} \to (A/\mathfrak{J})[X_1,...,X_p]$; comme tout polynôme est une série formelle restreinte, $\bar{p}_{\mathfrak{J}}$ est surjectif ; son noyau $N_{\mathfrak{J}}$ est l’idéal de $A\{X_1,...,X_p\}$ formé des séries formelles restreintes dont tous les coefficients appartiennent à $\mathfrak{J}$; nous munirons $A\{X_1,...,X_n\}$ de la topologie (linéaire) dont les $N_{\mathfrak{J}}$ (pour $\mathfrak{J} \in \mathcal{B}$) forment un système fondamental de voisinages de 0 (topologie qui ne dépend évidemment que de celle de $A$). Alors, il résulte de Top. gén., chap. III, 3e éd., § 7, no 3, prop. 2, que

$$
\pi = \lim_{\leftarrow \mathfrak{J}} \bar{p}_{\mathfrak{J}} : A\{X_1,...,X_p\} \to \lim_{\leftarrow \mathfrak{J}} (A/\mathfrak{J})[X_1,...,X_p]
$$

est un morphisme strict, dont le noyau est l’adhérence de $\{0\}$ dans $A\{X_1,...,X_p\}$, et dont l’image est dense dans

$$
A' = \lim_{\leftarrow \mathfrak{J}} (A/\mathfrak{J})[X_1,...,X_p].
$$

#### Proposition 3 {#ac-iii-s4-prop-3 .statement}

Si l’anneau commutatif linéairement topologisé $A$ est séparé et complet, l’homomorphisme canonique $\pi$ est un isomorphisme d’anneaux topologiques.

En effet, pour tout $(n_1,...,n_p) \in \mathbf{N}^p$ et tout $\mathfrak{J} \in \mathcal{B}$, soit $\varphi_{n_1...n_p}^{\mathfrak{J}}$ l’application $(A/\mathfrak{J})[X_1,...,X_p] \to A/\mathfrak{J}$ qui à tout polynôme fait correspondre le coefficient de $X_1^{n_1}...X_p^{n_p}$ dans ce polynôme ; il est clair que les $\varphi_{n_1...n_p}^{\mathfrak{J}}$ forment un système projectif d’homomorphismes de $(A/\mathfrak{J})$-modules (relatif à l’ensemble ordonné $\mathcal{B}$), et comme $A$ s’identifie canoniquement à $\lim_{\leftarrow \mathfrak{J}} (A/\mathfrak{J})$ par hypothèse,

$$
\varphi_{n_1...n_p} = \lim_{\leftarrow \mathfrak{J}} \varphi_{n_1...n_p}^{\mathfrak{J}}
$$

est un $A$-homomorphisme continu de $A'$ dans $A$. Pour tout élément $S = (S_{\mathfrak{J}})_{\mathfrak{J} \in \mathcal{B}}$ de $A'$, nous allons voir que la série formelle $T = \sum_{(n_i)} \varphi_{n_1...n_p}(S) X_1^{n_1}...X_p^{n_p}$ est restreinte et telle que $\pi(T) = S$. En effet, pour tout $\mathfrak{J} \in \mathcal{B}$, et tout $\mathfrak{J}' \in \mathcal{B}$ tel que $\mathfrak{J}' \subset \mathfrak{J}$, la relation $\varphi_{n_1 \ldots n_p}^{\mathfrak{J}}(S_{\mathfrak{J}}) = 0$ entraîne
$$
\varphi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) \in \mathfrak{J}/\mathfrak{J}'
$$
comme $S_{\mathfrak{J}}$ est un polynôme, on voit que $\varphi_{n_1 \ldots n_p}(S) \in \mathfrak{J}$ sauf pour les $(n_1, \ldots, n_p)$ en nombre fini tels que $\varphi_{n_1 \ldots n_p}^{\mathfrak{J}}(S_{\mathfrak{J}}) \neq 0$, ce qui prouve notre première assertion ; la seconde résulte des définitions. Comme $A$ est séparé, l’intersection des $N_{\mathfrak{J}}$ est réduite à 0, donc $\pi$ est *bijectif*, ce qui achève la démonstration, puisque $\pi$ est un morphisme strict.

#### Proposition 4 {#ac-iii-s4-prop-4 .statement}

*Soient* $A, B$ *deux anneaux commutatifs linéairement topologisés*, $B$ *étant séparé et complet*, $u : A \to B$ *un homomorphisme continu*. *Pour toute famille* $b = (b_i)_{1 \leq i \leq p}$ *d’éléments de* $B$, *il existe un homomorphisme continu et un seul*
$$
\tilde{u} : A\{X_1, \ldots, X_p\} \to B
$$
*tel que* $\tilde{u}(a) = u(a)$ *pour tout* $a \in A$ *et* $\tilde{u}(X_i) = b_i$ *pour* $1 \leq i \leq p$.

Il existe en effet un homomorphisme $\varphi : A[X_1, \ldots, X_p] \to B$ et un seul tel que $\varphi(a) = u(a)$ pour $a \in A$ et $\varphi(X_i) = b_i$ pour $1 \leq i \leq p$. En outre, si $\mathfrak{H}$ est un voisinage de 0 dans $B$ qui est un idéal, $\tilde{u}^{-1}(\mathfrak{H}) = \mathfrak{J}$ est un idéal de $A$ qui est un voisinage de 0, et pour tout polynôme $P \in N_{\mathfrak{J}}$, il est clair que $\varphi(P) \in \mathfrak{H}$, donc $\varphi$ est continu. Comme $A[X_1, \ldots, X_p]$ est dense dans $A\{X_1, \ldots, X_p\}$, l’existence et l’unicité de $\tilde{u}$ résultent de *Top. gén.*, chap. III, 3e éd., § 3, no 3, prop. 5 et du principe de prolongement des identités.

Dans le cas particulier où $A = B$ et où $u$ est l’application identique on écrira $f(b_1, \ldots, b_p)$ ou $f(b)$ la valeur de $\tilde{u}(f)$ pour toute série formelle restreinte $f \in A\{X_1, \ldots, X_p\}$.

#### Remarque 1 {#ac-iii-s4-n2-rem-1 .statement}

La prop. 4 prouve que pour tout idéal *fermé* $a$ d’un anneau $A$ supposé séparé et complet, les relations $b_i \in a$ pour $1 \leq i \leq p$ entraînent $f(b_1, \ldots, b_p) \in a$ pour toute série formelle restreinte $f \in A\{X_1, \ldots, X_p\}$.

#### Remarque 2 {#ac-iii-s4-n2-rem-2 .statement}

Supposons $A$ linéairement topologisé ; soit $r$ un entier tel que $1 \leq r \leq p$, et munissons l’anneau $A\{X_1, \ldots, X_r\}$ de la topologie définie ci-dessus. Alors l’anneau topologique $A\{X_1, ..., X_p\}$ s’identifie à l’anneau des séries formelles restreintes

$$
(A\{X_1, ..., X_r\}\{X_{r+1}, ..., X_p\}
$$

comme il résulte aussitôt des définitions.

#### Remarque 3 {#ac-iii-s4-n2-rem-3 .statement}

Avec les notations de la Remarque 2, supposons en outre A séparé et complet, et écrivons toute série formelle restreinte $f \in A\{X_1, ..., X_p\}$ sous la forme

$$
f = \sum_{(n_i)} c_{n_{r+1}...n_p}(X_1, ..., X_r) X_{r+1}^{n_{r+1}} ... X_p^{n_p}
$$

où les $c_{n_{r+1}...n_p}$ sont des séries formelles restreintes. Pour tout système $x = (x_1, ..., x_r)$ d’éléments de A, soit

$$
b_{n_{r+1}...n_p} = c_{n_{r+1}...n_p}(x_1, ..., x_r).
$$

Il résulte aussitôt de la Remarque 1 que $\sum_{(n_i)} b_{n_{r+1}...n_p} X_{r+1}^{n_{r+1}} ... X_p^{n_p}$ est une série formelle *restreinte*, quel’on note $f(x_1, ..., x_r, X_{r+1}, ..., X_p)$; on dit qu’elle s’obtient en *substituant* les $x_i$ aux $X_i$ pour $1 \leq i \leq r$ dans $f$.

### 3. Le lemme de Hensel.

Dans un anneau topologique A, on dit qu’un élément $x$ est *topologiquement nilpotent* si 0 est une limite de la suite $(x^n)_{n \geq 0}$. Si A est un anneau commutatif *linéairement topologisé*, dire que $x \in A$ est topologiquement nilpotent signifie que pour tout idéal ouvert $\mathfrak{J}$ de A, l’image canonique de $x$ dans $A/\mathfrak{J}$ est un élément *nilpotent* de cet anneau. Si $r_\mathfrak{J}$ est le nilradical de $A/\mathfrak{J}$, il est clair que $(r_\mathfrak{J})$ est un système projectif de parties et l’ensemble t des éléments topologiquement nilpotents de A est l’image réciproque de $r = \lim_{\leftarrow \mathfrak{J}} r_\mathfrak{J}$ par l’homomorphisme canonique $A \to \lim_{\leftarrow \mathfrak{J}} A/\mathfrak{J}$; c’est donc un *idéal fermé* de A. Si en outre A est *séparé et complet*, cet idéal est contenu dans le radical de A, et pour qu’un élément $x \in A$ soit inversible, il faut et il suffit que sa classe mod. t soit inversible dans $A/t$ (\S 2, n° 13, lemme 3).

On notera que si A est un anneau, m un idéal bilatère de A, les éléments de m sont topologiquement nilpotents pour la topologie *m-adique*.

#### Théorème 1 (Hensel) {#ac-iii-s4-thm-1 .statement}

Soit $A$ un anneau commutatif linéairement topologisé, séparé et complet. Soit $m$ un idéal fermé de $A$, dont les éléments sont topologiquement nilpotents. Soient $B = A/m$ l’anneau topologique quotient, $\varphi : A \to B$ l’application canonique. Soient $R$ une série formelle restreinte dans $A\{X\}$, $\overline{P}$ un polynôme unitaire dans $B[X]$, $\overline{Q}$ une série formelle restreinte dans $B\{X\}$. On suppose que $\overline{\varphi}(R) = \overline{P}.\overline{Q}$ et que $\overline{P}$ et $\overline{Q}$ soient fortement étrangers dans $B\{X\}$. Alors il existe un couple $(P, Q)$ et un seul formé d’un polynôme unitaire $P \in A[X]$ et d’une série formelle restreinte $Q \in A\{X\}$ tel que

$$
(4) \quad R = P.Q, \qquad \overline{\varphi}(P) = \overline{P}, \qquad \overline{\varphi}(Q) = \overline{Q}.
$$

De plus $P$ et $Q$ sont fortement étrangers dans $A\{X\}$, et si $R$ est un polynôme, il en est de même de $Q$.

La démonstration se fait en quatre étapes. Dans les trois premières, on suppose que $A$ est discret, auquel cas $R$ et $\overline{Q}$ sont des polynômes.

1) $m^2 = 0$.

Soient $S, T$ deux polynômes de $A[X]$ tels que $S$ soit unitaire et que l’on ait $\overline{\varphi}(S) = \overline{P}, \overline{\varphi}(T) = \overline{Q}$; la prop. 2 du no 1 montre que $S$ et $T$ sont fortement étrangers ; donc (no 1, prop. 1) il existe un couple unique de polynômes $(S', T')$ de $A[X]$ tel que

$$
(5) \quad R - ST = ST' + TS' \quad \text{et} \quad \deg(S') < \deg(S) = \deg(\overline{P}).
$$

Les polynômes $P = S + S', Q = T + T'$ répondent alors à la question ; on a en effet

$$
(6) \quad \overline{P}.\overline{\varphi}(T') + \overline{Q}.\overline{\varphi}(S') = \overline{\varphi}(ST' + TS') = \overline{\varphi}(R - ST) = 0.
$$

Comme $\overline{P}$ est unitaire, $\overline{P}$ et $\overline{Q}$ fortement étrangers et

$$
\deg(\overline{\varphi}(S')) < \deg(\overline{P}),
$$

la prop. 1 du no 1 montre que $\overline{\varphi}(S') = \overline{\varphi}(T') = 0$, autrement dit les coefficients de $S'$ et $T'$ appartiennent à $m$, et la relation $m^2 = 0$ donne $PQ = ST + ST' + TS' = R$, ce qui vérifie les relations (4). Puisque $\overline{\varphi}(P) = \overline{P}$ et $\overline{\varphi}(Q) = \overline{Q}$, $P$ et $Q$ sont fortement étrangers (no 1, prop. 2) ; enfin, si $P_1, Q_1$ sont deux autres polynômes de $A[X]$ vérifiant (4) et tels que $P_1$ soit unitaire, on a nécessairement, en posant $S'_1 = P_1 - S, T'_1 = Q_1 - T, \deg(S'_1) < \deg(S)$ et $R - ST = ST'_1 + TS'_1$ puisque $S'_1$ et $T'_1$ ont leurs coefficients dans $m$; mais la prop. 1 prouve alors que $S' = S'_1$ et $T' = T'_1$, ce qui prouve l’unicité du couple $(P, Q)$.

2) $m$ est nilpotent.

Soit $n$ le plus petit entier tel que $m^n = 0$, et raisonnons par récurrence sur $n > 2$, le théorème étant démontré pour $n = 2$. Soient $A' = A/m^{n-1}$, $m' = m/m^{n-1}$; comme ${m'}^{n-1} = 0$, il existe un couple unique $(P', Q')$ de polynômes de $A'[X]$ tel que $P'$ soit unitaire, $R' = P'Q'$, $\bar{\psi}(P') = \bar{P}$ et $\bar{\psi}(Q') = \bar{Q}$, en désignant par $\psi$ l’homomorphisme canonique $A' \to A'/m' = B$, par $\theta$ l’homomorphisme canonique $A \to A'$ et en posant $R' = \bar{\theta}(R)$. D’autre part, comme $(m^{n-1})^2 = 0$, il existe un couple unique $(P, Q)$ de polynômes de $A[X]$ tel que $P$ soit unitaire et $R = PQ, \bar{\theta}(P) = P', \bar{\theta}(Q) = Q'$; comme $\varphi = \psi \circ \theta$, cela montre l’existence et l’unicité de $P$ et $Q$ vérifiant (4); en outre $P'$ et $Q'$ sont fortement étrangers par l’hypothèse de récurrence, donc il en est de même de $P$ et $Q$.

3) $A$ est discret.

On notera que dans ce cas $m$ n’est plus nécessairement nilpotent, mais c’est en tout cas un nilidéal par hypothèse. Soient $P_0, Q_0$ deux polynômes de $A[X]$ tels que $\bar{\varphi}(P_0) = \bar{P}, \bar{\varphi}(Q_0) = \bar{Q}$ et que $P_0$ soit unitaire. Considérons l’idéal $n$ de $A$ engendré par les coefficients de $R - P_0Q_0$; il est de type fini et contenu dans $m$, donc il est nilpotent (chap. II, § 2, no 6, prop. 15), et par définition, si $\psi : A \to A/n$ est l’application canonique, on a $\bar{\psi}(R) = \bar{\psi}(P_0)\bar{\psi}(Q_0)$. En outre, $\bar{\psi}(P_0)$ et $\bar{\psi}(Q_0)$ sont fortement étrangers, comme il résulte de l’hypothèse sur $\bar{P}$ et $\bar{Q}$ et de la prop. 2 du no 1 appliquée à l’homomorphisme canonique $A/n \to A/m$. En vertu du cas 2), il existe donc un couple $(P, Q)$ de polynômes de $A[X]$, tel que $P$ soit unitaire et que les relations (4) soient vérifiées. Le fait que $\bar{P}$ et $\bar{Q}$ sont fortement étrangers entraîne encore ici que $P$ et $Q$ sont fortement étrangers dans $A[X]$ en vertu du n° 1, prop. 2, car m est contenu dans le radical de A. Supposons enfin que P₁, Q₁ soient deux polynômes de A[X] vérifiant (4) et tels que P₁ soit unitaire, et soit n₁ l’idéal de type fini de A engendré par les coefficients de P − P₁ et les coefficients de Q − Q₁ ; comme n₁ est contenu dans m, il est nilpotent, et si ψ₁ : A → A/n₁ est l’application canonique on a $\bar{\psi}_1(P) = \bar{\psi}_1(P_1),\ \bar{\psi}_1(Q) = \bar{\psi}_1(Q_1)$; la propriété d’unicité du cas 2) entraîne donc P = P₁, Q = Q₁.

4) Cas général.

Soit $\mathcal{B}$ un système fondamental de voisinages de 0 dans A, formé d’idéaux de A. Pour tout $\mathfrak{J} \in \mathcal{B}$, soient $f_{\mathfrak{J}}$ l’application canonique $A \to A/\mathfrak{J}$, $\varphi_{\mathfrak{J}}$ l’application canonique

$$
A/\mathfrak{J} \to (A/\mathfrak{J})/((m + \mathfrak{J})/\mathfrak{J}) = A/(m + \mathfrak{J}),
$$

$g_{\mathfrak{J}}$ l’application canonique $B = A/m \to A/(m + \mathfrak{J})$, et posons $R_{\mathfrak{J}} = \bar{f}_{\mathfrak{J}}(R),\ \overline{P}_{\mathfrak{J}} = \bar{g}_{\mathfrak{J}}(\overline{P}),\ \overline{Q}_{\mathfrak{J}} = \bar{g}_{\mathfrak{J}}(\overline{Q})$. Comme chaque anneau $A/\mathfrak{J}$ est discret, on peut lui appliquer le cas 3), et on voit qu’il existe un couple unique $(P_{\mathfrak{J}}, Q_{\mathfrak{J}})$ de polynômes de $(A/\mathfrak{J})[X]$ tels que $P_{\mathfrak{J}}$ soit unitaire et $R_{\mathfrak{J}} = P_{\mathfrak{J}} Q_{\mathfrak{J}},\ \overline{\varphi}_{\mathfrak{J}}(P_{\mathfrak{J}}) = \overline{P}_{\mathfrak{J}},\ \overline{\varphi}_{\mathfrak{J}}(Q_{\mathfrak{J}}) = \overline{Q}_{\mathfrak{J}}$. L’unicité de ce couple entraîne que si $\mathfrak{J}' \subset \mathfrak{J},\ \mathfrak{J}' \in \mathcal{B}$, et si $f_{\mathfrak{J}\mathfrak{J}'} : A/\mathfrak{J}' \to A/\mathfrak{J}$ est l’application canonique, on a $P_{\mathfrak{J}} = \bar{f}_{\mathfrak{J}\mathfrak{J}'}(P_{\mathfrak{J}'}) , Q_{\mathfrak{J}} = \bar{f}_{\mathfrak{J}\mathfrak{J}'}(Q_{\mathfrak{J}'})$. Il résulte donc de l’identification canonique de $A\{X\}$ et de $\varprojlim_{\mathfrak{J}} (A/\mathfrak{J})[X]$ (n° 2, prop. 3) qu’il existe $P \in A\{X\}$ et $Q \in A\{X\}$ tels que $R = PQ$ et $\bar{f}_{\mathfrak{J}}(P) = P_{\mathfrak{J}},\ \bar{f}_{\mathfrak{J}}(Q) = Q_{\mathfrak{J}}$ pour tout $\mathfrak{J} \in \mathcal{B}$. En outre, on a $\bar{g}_{\mathfrak{J}}(\overline{P} - \overline{\varphi}(P)) = 0,\ \bar{g}_{\mathfrak{J}}(\overline{Q} - \overline{\varphi}(Q)) = 0$ pour tout $\mathfrak{J} \in \mathcal{B}$, ce qui signifie que pour tout $\mathfrak{J} \in \mathcal{B}$ les coefficients de $\overline{P} - \overline{\varphi}(P)$ et de $\overline{Q} - \overline{\varphi}(Q)$ appartiennent tous à $(m + \mathfrak{J})/m$. Mais comme m est fermé dans A, on a $\bigcap_{\mathfrak{J}} (m + \mathfrak{J}) = m$, d’où $\overline{P} = \overline{\varphi}(P),\ \overline{Q} = \overline{\varphi}(Q)$, et P et Q vérifient donc bien (4) ; en outre, comme les $P_{\mathfrak{J}}$ sont unitaires et de même degré, la série formelle restreinte P est un polynôme unitaire. Si $(P', Q')$ était un autre couple vérifiant (4) et tel que $P'$ soit un polynôme unitaire, on en déduirait que $R_{\mathfrak{J}} = \bar{f}_{\mathfrak{J}}(P')\bar{f}_{\mathfrak{J}}(Q'),\ \overline{\varphi}_{\mathfrak{J}}(\bar{f}_{\mathfrak{J}}(P')) = \overline{P}_{\mathfrak{J}}$ et $\overline{\varphi}_{\mathfrak{J}}(\bar{f}_{\mathfrak{J}}(Q')) = \overline{Q}_{\mathfrak{J}}$, et d’après l’unicité du cas 3), $\bar{f}_{\mathfrak{J}}(P') = P_{\mathfrak{J}},\ \bar{f}_{\mathfrak{J}}(Q') = Q_{\mathfrak{J}}$ pour tout $\mathfrak{J} \in \mathcal{B}$, ce qui entraîne $P = P'$ et $Q = Q'$. Montrons enfin que P et Q sont fortement étrangers ; en vertu du cas 3) et de la prop. 1 du no 1, pour tout $\mathcal{J} \in \mathcal{B}$, il existe un couple unique $(S_{\mathcal{J}}, T_{\mathcal{J}})$ de polynômes de $(A/\mathcal{J})[X]$ tels que

(7) $1 = P_{\mathcal{J}} S_{\mathcal{J}} + Q_{\mathcal{J}} T_{\mathcal{J}}$ et $\deg(T_{\mathcal{J}}) < \deg(P_{\mathcal{J}}) = \deg(\overline{P})$.

L’unicité de ce couple montre aussitôt que pour $\mathcal{J}' \in \mathcal{B}$, $\mathcal{J}' \subset \mathcal{J}$, on a $S_{\mathcal{J}} = \overline{f}_{\mathcal{J}\mathcal{J}'}(S_{\mathcal{J}'})$, $T_{\mathcal{J}} = \overline{f}_{\mathcal{J}\mathcal{J}'}(T_{\mathcal{J}'})$; compte tenu du no 2, prop. 3, on en conclut l’existence de deux séries formelles restreintes, $S, T$ de $A\{X\}$ telles que $S_{\mathcal{J}} = \overline{f}_{\mathcal{J}}(S)$, $T_{\mathcal{J}} = \overline{f}_{\mathcal{J}}(T)$ et $1 = PS + QT$.

Reste à voir que si $R$ est un polynôme, il en est de même de $Q$. Or, les $Q_{\mathcal{J}}$ sont des polynômes par construction, et comme $P_{\mathcal{J}}$ est unitaire, la relation $R_{\mathcal{J}} = P_{\mathcal{J}} Q_{\mathcal{J}}$ entraîne

$$ \deg(Q_{\mathcal{J}}) \leq \deg(R_{\mathcal{J}}) \leq \deg(R) $$

pour tout $\mathcal{J} \in \mathcal{B}$; d’où aussitôt la conclusion par définition de $Q$.

C. Q. F. D.

### 4. Composition des systèmes de séries formelles.

Soit $A$ un anneau commutatif ; nous dirons qu’un système

(8) $f = (f_1, ..., f_p) \in (A[[X_1, ..., X_q]])^p$

de séries formelles en les $X_j$ ($1 \leq j \leq q$), à coefficients dans $A$, est sans terme constant s’il en est ainsi de tous les $f_j$. Pour tout système (8) de séries formelles et tout système

(9) $g = (g_1, ..., g_q) \in (A[[X_1, ..., X_r]])^q$

de $q$ séries formelles sans terme constant, nous désignerons par $f \circ g$ (ou $f(g)$) le système de séries formelles $f_j(g_1, ..., g_q)$ ($1 \leq j \leq p$) dans $(A[[X_1, ..., X_r]])^p$ (*Alg.*, chap. IV, § 5, no 5). Si

$$ h = (h_1, ..., h_r) \in (A[[X_1, ..., X_s]])^r $$

est un troisième système sans terme constant, on a

(10) $(f \circ g) \circ h = f \circ (g \circ h)$.

En effet, pour tout entier $m$, on a

$$ (f^{(m)} \circ g^{(m)}) \circ h^{(m)} = f^{(m)} \circ (g^{(m)} \circ h^{(m)}) $$

en désignant par $f^{(m)}, g^{(m)}, h^{(m)}$ les systèmes de polynômes formés des termes de degré total $\leq m$ dans les systèmes de séries formelles $f, g, h$. Mais il est clair que les termes de degré total $\leq m$ dans les séries de $(f \circ g) \circ h$ (resp. $f \circ (g \circ h)$) sont les mêmes que dans $(f^{(m)} \circ g^{(m)}) \circ h^{(m)}$ (resp. $f^{(m)} \circ (g^{(m)} \circ h^{(m)})$), d’où notre assertion.

Pour tout système (8), nous désignerons par $M_f$, ou $M_f(\mathbf{X})$, la matrice jacobienne $(\partial f_i / \partial X_j)$ ($1 \leq i \leq p, 1 \leq j \leq q$) où $i$ est l’indice des lignes et $j$ celui des colonnes ; pour deux systèmes (8) et (9), où $g$ est sans terme constant, on a

$$
M_{f \circ g} = (M_f(g)). M_g
$$

où $M_f(g)$ est la matrice dont les éléments s’obtiennent en substituant $g_j$ à $X_j$ ($1 \leq j \leq q$) dans chaque série élément de $M_f$; cette formule ne fait que traduire en effet la formule (9) d’Alg., chap. IV, § 5, n° 8. Nous noterons $M_f(0)$ la matrice des termes constants des éléments de $M_f$; on déduit donc de (11) que

$$
M_{f \circ g}(0) = M_f(0) . M_g(0).
$$

Étant donné un entier $n > 0$, nous poserons

$$
\mathbf{1}_n = \mathbf{X} = (X_1, ..., X_n) \in (A[[X_1, ..., X_n]])^n,
$$

qui sera considéré comme matrice à une colonne.

Pour tout système $f = (f_1, ..., f_n) \in (A[[X_1, ..., X_n]])^n$, $M_f$ est une matrice carrée d’ordre $n$; nous noterons $J_f$ ou $J_f(\mathbf{X})$ son déterminant, $J_f(0)$ le terme constant de $J_f$, égal à $\det(M_f(0))$; si $g = (g_1, ..., g_n)$ est un système sans terme constant dans $(A[[X_1, ..., X_n]])^n$, on a donc, d’après (11) et (12)

$$
J_{f \circ g} = J_f(g) . J_g
$$
$$
J_{f \circ g}(0) = J_f(0) J_g(0).
$$

#### Proposition 5 {#ac-iii-s4-prop-5 .statement}

*Soient A un anneau commutatif, $\hat{f} = (f_1, ..., f_n)$ un système sans terme constant de n séries de $A[[X_1, ..., X_n]]$. Supposons que $J_f(0)$ soit inversible dans A. Alors il existe un système sans terme constant $g = (g_1, ..., g_n)$ de n séries de $A[[X_1, ..., X_n]]$ tel que*

$$
f \circ g = \mathbf{1}_n.
$$

Ce système est unique et on a

(17) $g \circ f = 1_n$.

L’existence et l’unicité de $g$ résultent d’Alg., chap. IV, § 5, no 9, prop. 10, appliquée aux $n$ séries formelles

$$
f_i(Y_1, ..., Y_n) - X_i \quad (1 \leq i \leq n).
$$

Il résulte de (15) et (16) que l’on a $J_f(0)J_g(0) = 1$, donc $J_g(0)$ est aussi inversible. On en conclut l’existence d’un système $h = (h_1, ..., h_n)$ de $n$ séries sans terme constant de $A[[X_1, ..., X_n]]$ tel que $g \circ h = 1_n$; de cette relation et de (16) il résulte alors, grâce à (10), que $h = 1_n \circ h = (f \circ g) \circ h = f \circ (g \circ h) = f \circ 1_n = f$.

La prop. 5 et les formules (10) et (15) montrent que pour la loi de composition $(f, g) \to f \circ g$, l’ensemble des systèmes $f = (f_1, ..., f_n)$ de $n$ séries sans terme constant de $A[[X_1, ..., X_n]]$ pour lesquels $J_f(0)$ est inversible dans $A$, est un groupe.

### 5. Systèmes d’équations dans les anneaux complets.

Pour abréger, nous dirons dans ce qui suit qu’un anneau $A$ satisfait aux conditions de Hensel s’il est commutatif, linéairement topologisé, séparé et complet ; étant donné un idéal $m$ dans un tel anneau, nous dirons que $m$ (ou le couple $(\Lambda, m)$) satisfait aux conditions de Hensel si $m$ est fermé dans $A$ et si ses éléments sont topologiquement nilpotents. L’idéal $t$ de $A$ formé de tous les éléments topologiquement nilpotents satisfait aux conditions de Hensel (no 3).

En particulier, si $A$ est un anneau commutatif, $m$ un idéal de $A$, et si $A$ est séparé et complet pour la topologie $m$-adique, le couple $(A, m)$ satisfait aux conditions de Hensel.

#### Proposition 6 {#ac-iii-s4-prop-6 .statement}

Soient $A$ un anneau commutatif, $B$ un anneau satisfaisant aux conditions de Hensel, $u : A \to B$ un homomorphisme. Pour toute famille $x = (x_1, ..., x_n)$ d’éléments topologiquement nilpotents de $B$, il existe un homomorphisme $\tilde{u}$ et un seul de $A[[X_1, ..., X_n]]$ dans $B$ tel que $\tilde{u}(a) = u(a)$ pour tout $a \in A$ et $\tilde{u}(X_i) = x_i$ pour $1 \leq i \leq n$. En outre, si $m$ désigne l’idéal des séries sans terme constant dans $A[[X_1, ..., X_n]]$, $\tilde{u}$ est continu pour la topologie m-adique.

Soit $\alpha$ l’idéal de type fini engendré dans B par les $x_i (1 \leq i \leq n)$; pour tout idéal ouvert $\mathfrak{H}$ de B, les images des $x_i$ dans $B/\mathfrak{H}$ sont nilpotentes, donc l’idéal $(\alpha + \mathfrak{H})/\mathfrak{H}$ est nilpotent dans $B/\mathfrak{H}$, et il existe un entier $k$ tel que, pour $\sum_{i=1}^n p_i \geq k$ on ait $x_1^{p_1} ... x_n^{p_n} \in \mathfrak{H}$. Comme tout élément de $m^k$ est somme finie de séries formelles de la forme $X_1^{p_1} ... X_n^{p_n} g(X_1, ..., X_n)$, où $\sum_{i=1}^n p_i \geq k$, on voit que si $\tilde{u}$ répond à la question, on a $\tilde{u}(m^k) \subset \mathfrak{H}$, ce qui prouve la continuité de $\tilde{u}$. Il existe évidemment un homomorphisme $\varphi : A[X_1, ..., X_n] \to B$ et un seul tel que $\varphi(a) = u(a)$ pour $a \in A$ et $\varphi(X_i) = x_i$ pour $1 \leq i \leq n$, et le raisonnement précédent montre que $\varphi$ est continu pour la topologie induite sur $A[X_1, ..., X_n]$ par la topologie m-adique. Comme $A[X_1, ..., X_n]$ est dense dans $A[[X_1, ..., X_n]]$ pour la topologie m-adique et que B est séparé et complet, cela achève de prouver l’existence et l’unicité de $\tilde{u}$.

On notera que cette proposition redonne comme cas particulier le (i) de la prop. 11 du § 2, no 9.

Lorsque A est lui-même linéairement topologisé, la restriction de $\tilde{u}$ à $A\{X_1, ..., X_n\}$ coïncide avec l’homomorphisme défini à partir de $u$ dans la prop. 4 du no 2. Cela résulte aussitôt de ce que $A[X_1, ..., X_n]$ est dense dans $A\{X_1, ..., X_n\}$ quand on munit cet anneau de la topologie ayant pour système fondamental de voisinages de 0 les idéaux $m^k \cap N_S$ (avec les notations du no 2 ; cette topologie est la borne supérieure de la topologie induite sur $A\{X_1, ..., X_n\}$ par la topologie m-adique de $A[[X_1, ..., X_n]]$, et de la topologie définie au no 2).

Lorsque B = A et que $u$ est l’application identique, nous noterons $f(x_1, ..., x_n)$ ou $f(\mathbf{x})$ l’élément $\tilde{u}(f)$ pour toute série formelle $f \in A[[X_1, ..., X_n]]$; pour tout système $\mathbf{f} = (f_1, ..., f_r)$ de séries formelles de $A[[X_1, ..., X_n]]$, on notera $\mathbf{f}(\mathbf{x})$ l’élément $(f_1(\mathbf{x}), ..., f_r(\mathbf{x}))$ de $A^r$ et on dit qu’il s’obtient en substituant les $x_i$ aux $X_i$ dans $\mathbf{f}$. Si $n \leq m$ et si F est une série formelle de $A[[X_1, ..., X_m]]$, on peut considérer F comme une série formelle en $X_{n+1}, \ldots, X_m$ à coefficients dans $\Lambda[[X_1, \ldots, X_n]]$; on note $F(x_1, \ldots, x_n, X_{n+1}, \ldots, X_m)$ la série formelle de $\Lambda[[X_{n+1}, \ldots, X_m]]$ obtenue en substituant les $x_i$ aux $X_i$ dans les coefficients de F, pour $1 \leq i \leq n$.

Prenons pour B un anneau de séries formelles $\Lambda[[X_1, \ldots, X_r]]$, et soit $\mathfrak{n}$ l’idéal des séries de B sans terme constant, de sorte que $(B, \mathfrak{n})$ satisfait aux conditions de Hensel ($§\ 2$, no 6, cor. de la prop. 6). On peut appliquer la prop. 6 en prenant pour les $x_i \in B$ des séries sans terme constant ; alors, pour toute série $f \in \Lambda[[X_1, \ldots, X_n]]$, $\tilde{u}(f)$ n’est autre que la série formelle $f(x_1, \ldots, x_n)$ définie en Alg., chap. IV, $§\ 5$, no 5. C’est évident si $f$ est un polynôme et on en déduit la proposition dans le cas général en remarquant que $f \to f(x_1, \ldots, x_n)$ est continue dans $\Lambda[[X_1, \ldots, X_n]]$ pour la topologie $m$-adique.

#### Corollaire {#ac-iii-s4-n5-cor-1 .statement}

Soient $\Lambda$ un anneau satisfaisant aux conditions de Hensel, $\mathbf{x} = (x_1, \ldots, x_n)$ une famille d’éléments topologiquement nilpotents dans $\Lambda$. Soient $g = (g_1, \ldots, g_q)$ un système sans terme constant de séries de $\Lambda[[X_1, \ldots, X_n]]$, $\mathbf{f} = (f_1, \ldots, f_p)$ un système de séries formelles de $\Lambda[[X_1, \ldots, X_q]]$. Alors $g(\mathbf{x}) = (g_1(\mathbf{x}), \ldots, g_q(\mathbf{x}))$ est une famille d’éléments topologiquement nilpotents de $\Lambda$ et on a
$$(18)$$
$$(\mathbf{f} \circ g)(\mathbf{x}) = \mathbf{f}(g(\mathbf{x})).$$

Le fait que les $g_i(\mathbf{x})$ sont topologiquement nilpotents résulte aussitôt de la prop. 6 et du fait que dans $\Lambda$ l’idéal des éléments topologiquement nilpotents est fermé. La relation (18) est évidente lorsque les $f_j$ sont des polynômes ; d’autre part, si $m$ et $m'$ sont les idéaux des séries sans terme constant dans $\Lambda[[X_1, \ldots, X_q]]$ et dans $\Lambda[[X_1, \ldots, X_n]]$ respectivement, il est clair que la relation $f \in m^k$ entraîne $f(g_1, \ldots, g_q) \in {m'}^k$. Les deux membres de (18) sont donc fonctions continues de $\mathbf{f}$ dans $(\Lambda[[X_1, \ldots, X_q]])^p$ quand on munit $\Lambda[[X_1, \ldots, X_q]]$ de la topologie $m$-adique, en vertu de la remarque précédente et de la prop. 6 ; d’où la relation (18).

Dans ce qui suit, pour un anneau $\Lambda$ et un idéal $m$ de $\Lambda$, nous noterons $m^{x^n}$ l’ensemble produit $\prod_{i=1}^n m_i$ dans $\Lambda^n$, avec $m_i = m$ pour $1 \leq i \leq n$, pour éviter toute confusion.

#### Proposition 7 {#ac-iii-s4-prop-7 .statement}

Soient $A$ un anneau, $m$ un idéal de $A$ tels que le couple $(A, m)$ satisfasse aux conditions de Hensel. Soit $f = (f_1, ..., f_n)$ un système sans terme constant de séries de $A[[X_1, ..., X_n]]$ tel que $J_f(0)$ soit inversible dans $A$. Alors, pour tout $x \in m^{x^n}$, on a $f(x) \in m^{x^n}$, et $x \to f(x)$ est une bijection de $m^{x^n}$ sur lui-même, la bijection réciproque étant $x \to g(x)$, où $g$ est donné par la relation (16) du no 4.

Le fait que $f(x) \in m^{x^n}$ est évident lorsque les $f_i$ sont des polynômes et résulte en général de la prop. 6 et de ce que $m$ est fermé dans $A$. Les autres assertions de la proposition sont alors des conséquences immédiates de (16), (17) et (18).

#### Corollaire {#ac-iii-s4-n5-cor-2 .statement}

Soit $q$ un idéal fermé de $A$ contenu dans $m$. Alors la relation $x \equiv x' \pmod{q^{x^n}}$ est équivalente à $f(x) \equiv f(x') \pmod{q^{x^n}}$.

En effet, pour toute série formelle $f \in A[[X_1, ..., X_n]]$, on a
$$
f(X_1, ..., X_n) - f(Y_1, ..., Y_n) = \sum_{i=1}^n (X_i - Y_i) h_i(X_1, ..., X_n, Y_1, ..., Y_n)
$$
où les $h_i$ appartiennent à $A[[X_1, ..., X_n, Y_1, ..., Y_n]]$ (Alg., chap. IV, § 5, no 8, prop. 9); on en déduit aussitôt que la relation $x \equiv x' \pmod{q^{x^n}}$ entraîne $f(x) \equiv f(x') \pmod{q^{x^n}}$. La réciproque s’obtient en remplaçant $f$ par son « inverse » $g$.

#### Théorème 2 {#ac-iii-s4-thm-2 .statement}

Soient $A$ un anneau, $m$ un idéal de $A$ tels que le couple $(A, m)$ satisfasse aux conditions de Hensel. Soit $f = (f_1, ..., f_n)$ un système de $n$ éléments de $A \{ X_1, ..., X_n \}$ et soit $a \in A^n$; posons $J_f(a) = e$. Il existe un système $g = (g_1, ..., g_n)$ de séries formelles restreintes sans terme constant dans $A \{ X_1, ..., X_n \}$, telles que :
(i) $M_g(0) = I_n$ (matrice unité).
(ii) Pour tout $x \in A^n$, on a
$$
f(a + ex) = f(a) + M_f(a) \cdot eg(x).
$$
(iii) Soit $h = (h_1, ..., h_n)$ le système de séries formelles sans terme constant (non nécessairement restreintes) tel que $g \circ h = 1_n$ (prop. 5). Pour tout $y \in m^{x^n}$, on a
$$
f(a + eh(y)) = f(a) + M_f(a) \cdot ey.
$$

Pour toute série formelle $f \in A[[X_1, ..., X_n]]$, on a
$$
(21) \quad f(\mathbf{X} + \mathbf{Y}) = f(\mathbf{X}) + M_f(\mathbf{X}) \cdot \mathbf{Y} + \sum_{1 \leq i \leq j \leq n} G_{ij}(\mathbf{X}, \mathbf{Y}) Y_i Y_j
$$
où les $G_{ij}$ sont des séries formelles bien déterminées dans $A[[X_1, ..., X_n, Y_j, ..., Y_n]]$. Si $f$ est restreinte, il en est de même des éléments de $M_f$ et des $G_{ij}$, car ces séries formelles sont des polynômes lorsque $f$ est un polynôme, et il résulte de leur unicité que pour tout idéal ouvert $\mathfrak{J}$ de $A$, en désignant par $p_\mathfrak{J} : A \to A/\mathfrak{J}$ l’application canonique, l’image de $G_{ij}$ par $\bar{p}_\mathfrak{J}$ est le coefficient de $Y_i Y_j$ dans $\bar{p}_\mathfrak{J}(F)$ où $F$ est la série formelle $f(\mathbf{X} + \mathbf{Y})$ dans $A[[X_1, ..., X_n, Y_1, ..., Y_n]]$; d’où notre assertion.

Cela étant, en écrivant la formule (21) pour chaque série $f_i$ ($1 \leq i \leq n$), on obtient, pour tout $\mathbf{x} \in A^n$ (no 2, prop. 4)
$$
(22) \quad \mathbf{f}(a + e \mathbf{x}) = \mathbf{f}(a) + M_i(a) \cdot e \mathbf{x} + e^2 r(\mathbf{x})
$$
où $r = (r_1, ..., r_n)$ est un système de séries formelles restreintes dont chacune est d’ordre total $\geq 2$. Il résulte des formules (18) de Alg., chap. III, 2e éd., § 6, no 5 qu’il existe une matrice carrée $M' \in \mathbf{M}_n(A)$ telle que
$$
(23) \quad M_i(a) \cdot M' = e I_n,
$$
d’où en portant dans (22)
$$
(24) \quad \mathbf{f}(a + e \mathbf{x}) = \mathbf{f}(a) + M_i(a) \cdot e \mathbf{x} + M_i(a) M' \cdot e r(\mathbf{x}).
$$
En posant $g = 1_n + M' \cdot r$, on voit que $g$ vérifie les conditions (i) et (ii) ; il suffit ensuite de remplacer $\mathbf{x}$ par $h(y)$ pour obtenir (iii).

#### Corollaire 1 {#ac-iii-s4-thm-2-cor-1 .statement}

Soient $A$ un anneau, $m$ un idéal de $A$ tels que le couple $(A, m)$ satisfasse aux conditions de Hensel. Soient $f \in A\{X\}$, $a \in A$, et posons $e = f'(a)$. Si $f(a) \equiv 0$ (mod. $e^2 m$), alors il existe $b \in A$ tel que $f(b) = 0$ et $b \equiv a$ (mod. $e m$). Si $b'$ est un second élément de $A$ tel que $f(b') = 0$ et $b' \equiv a$ (mod. $e m$), on a $e(b - b') = 0$. En particulier, $b$ est unique si $e$ n’est pas diviseur de zéro dans $A$.

En effet, soit $f(a) = e^2 c$ avec $c \in m$ ; la formule (20) pour $n = 1$ donne $f(a + e h(y)) = e^2 (c + y)$ et il suffit donc de prendre $y = -c$, $b = a + e h(-c)$. En outre si $b = a + e x$, $b' =$ a + ex', x \in m, x' \in m, f(b) = f(b') = 0, on déduit de (19) que $e^2(g(x) - g(x')) = 0$. Comme $g(X) - g(Y) = (X - Y)u(X, Y)$, où $u$ est restreinte et $u(0, 0) = 1$, on a $g(x) - g(x') = (x - x')v$, où $v \in A$ est inversible, car, $m$ étant fermé, on a $v - 1 = u(x, x') - 1 \in m$ et $m$ est contenu dans le radical de $A$; d'où la relation $e(b - b') = 0$.

#### Remarque {#ac-iii-s4-n5-rem-1 .statement}

Le corollaire s’applique notamment lorsque $e$ est inversible dans $A$; on peut alors déduire aussi l’existence de $b$ du th. de Hensel, car l’image canonique de $f(X)$ dans $(A/m)\{X\}$ est de la forme $(X - \alpha)f_1(X)$, $X - \alpha$ et $f_1(X)$ étant fortement étrangers, car $f_1(x) = f'(x)$ est l’image de $e$ (no 1, Exemple).

#### Exemple 1 {#ac-iii-s4-n5-exa-1 .statement}

Soient $p$ un nombre premier $\neq 2$ et $n$ un entier dont la classe mod. $p$ soit un carré $\neq 0$ dans le corps premier $\mathbf{F}_p$. Si $\mathbf{Z}_p$ est l’anneau des entiers $p$-adiques ($\S$ 2, no 12, Exemple 3), l’application du cor. 1 au polynôme $X^2 - n$ montre que $n$ est un carré dans $\mathbf{Z}_p$; par exemple 7 est un carré dans $\mathbf{Z}_3$.

#### Exemple 2 {#ac-iii-s4-n5-exa-2 .statement}

Soit $A = K[[Y]]$ l’anneau des séries formelles à une indéterminée à coefficients dans un corps commutatif $K$; muni de la topologie (Y)-adique, l’anneau $A$ est séparé et complet ($\S$ 2, no 6, cor. de la prop. 6) et l’application $f(Y) \to f(0)$ définit par passage au quotient un isomorphisme de $A/(Y)$ sur le corps $K$. En vertu du cor. 1, si $F(Y, X)$ est un polynôme en $X$ à coefficients dans $A$, et si $a$ est une racine simple de $F(0, X)$ dans $K$, il existe une série formelle et une seule $f(Y)$ telle que $f(0) = a$ et $F(Y, f(Y)) = 0$.

#### Corollaire 2 {#ac-iii-s4-thm-2-cor-2 .statement}

Soient $A$ un anneau, $m$ un idéal de $A$ tels que le couple $(A, m)$ satisfasse aux conditions de Hensel. Soient $r, n$ des entiers tels que $0 \leq r < n$, $f = (f_{r+1}, ..., f_n)$ un système de $n - r$ éléments de $A \{X_1, ..., X_n\}$; désignons par $J^{(n-r)}_i(\mathbf{X})$ le mineur de $M_f(\mathbf{X})$ formé des colonnes d’indice $j$ tel que $r + 1 \leq j \leq n$. Soit $a \in A^n$ tel que $J^{(n-r)}_i(a)$ soit inversible dans $A$ et que l’on ait $f(a) \equiv 0$ (mod. $m^{x(n-r)}$). Alors il existe un $\mathbf{x} = (x_1, ..., x_n) \in A^n$ et un seul tel que $x_k = a_k$ pour $1 \leq k \leq r$, $\mathbf{x} \equiv a$ (mod. $m^{x^n}$) et $f(\mathbf{x}) = 0$.

En substituant $a_k$ à $X_k$ pour $1 \leq k \leq r$ dans les $f_t$ (no 2, Remarque 3) on voit aussitôt qu’on peut se restreindre au cas où r = 0 pour prouver le corollaire. Le th. 2 et la prop. 7 montrent alors que f définit une bijection de $a + m^{x^n}$ sur $f(a) + m^{x^n} = m^{x^n}$; le corollaire résulte de ce que $0 \in m^{x^n}$.

#### Corollaire 3 {#ac-iii-s4-thm-2-cor-3 .statement}

Les notations étant celles du cor. 2, soit $a \in A^n$; posons $e = J_i^{(n-r)}(a)$ (non nécessairement inversible dans A) et supposons que l'on ait $f(a) \equiv 0$ (mod. $e^2 m^{x(n-r)}$). Alors il existe $n - r$ séries formelles $\varphi_i$ de $A[[X_1, ..., X_r]]$ ($r + 1 \leq i \leq n$) à terme constant dans $m$, telles que, pour tout $t = (t_1, ..., t_r) \in m^{x^r}$, on ait

$$
f_i(a_1 + e^2 t_1, ..., a_r + e^2 t_r, a_{r+1} + e \varphi_{r+1}(t), ..., a_n + e \varphi_n(t)) = 0
$$

pour $r + 1 \leq i \leq n$.

Pour $1 \leq i \leq r$, posons $f_i(X) = X_i - a_i$, et soit $u = (f_1, ..., f_n)$; on a $J_u(a) = e$ et le th. 2 est applicable au système u. Avec les notations du th. 2, il résulte des définitions précédentes que $eg_i(X) = eX_i$ pour $1 \leq i \leq r$, d'où $eh_i(X) = eX_i$ pour $1 \leq i \leq r$; en outre, si $M' \in \mathbf{M}_n(A)$ est telle que $M_u(a).M' = eI_n$, $M'$ est de la forme

$$
\begin{pmatrix}
eI_r & 0 \\
* & *
\end{pmatrix}.
$$

Remplaçant y par $M'.z$ (avec $z = (z_1, ..., z_n) \in m^{x^n}$), dans la formule (20), on obtient

$$
\begin{align*}
f_i(a_1 + e^2 z_1, ..., a_r + e^2 z_r, a_{r+1} + e h_{r+1}(M'.z), ..., a_n + e h_n(M'.z)) \\
= f_i(a) + e^2 z_i \quad \text{pour } 1 \leq i \leq n.
\end{align*}
$$

Par hypothèse, on a $f_j(a) = e^2 b_j$ avec $b_j \in m$ pour $r + 1 \leq j \leq n$. Posons $\psi_j(X_1, ..., X_n) = h_j(M'.X)$, et

$$
\varphi_j(X_1, ..., X_r) = \psi_j(X_1, ..., X_r, -b_{r+1}, ..., -b_n)
$$

pour $r + 1 \leq j \leq n$. Pour $r + 1 \leq i \leq n$, en substituant $t_j$ à $z_j$ pour $1 \leq j \leq r$ et $-b_j$ à $z_j$ pour $r + 1 \leq j \leq n$ dans (26), on obtient les relations (25) pour tout $t \in m^{x^r}$.

### 6. Application aux décompositions d'anneaux.

#### Lemme 2 {#ac-iii-s4-lem-2 .statement}

Soient A un anneau, m un idéal de A tels que le couple $(A, m)$ satisfasse aux conditions de Hensel. Soient B l'anneau quotient $A/m$, $\pi : A \to B$ l'homomorphisme canonique. Pour tout idempotent c de B, il existe un idempotent e ∈ A et un seul tel que π(e) = c.

Soit a ∈ A tel que π(a) = c ; on peut appliquer le cor. 1 du th. 2 du n° 5 au polynôme f(X) = X² − X de A[X] et à l’élément a ∈ A. On a f'(a) = 2a − 1, et comme π(2a − 1) = 2c − 1 et (2c − 1)² = 1 dans B, 2c − 1 est inversible dans B, donc 2a − 1 est inversible dans A (§ 2, n° 13, lemme 3). Comme f(a) ∈ m, le cor. 1 du th. 2 du n° 5 donne aussitôt l’existence et l’unicité de e.

#### Proposition 8 {#ac-iii-s4-prop-8 .statement}

Soient A un anneau, m un idéal de A tels que le couple (A, m) satisfasse aux conditions de Hensel. Soient B l’anneau quotient A/m, π : A → B l’homomorphisme canonique. Si B est composé direct d’une famille finie (b_i)_{i∈I} d’idéaux, il existe une famille et une seule (α_i)_{i∈I} d’idéaux de A telle que π(α_i) = b_i pour tout i ∈ I et que A soit composé direct de la famille (α_i).

Soit 1 = ∑_{i} c_i où c_i ∈ b_i pour tout i ; les c_i sont des idempotents de B tels que c_i c_j = 0 pour i ≠ j. En vertu du lemme 2, il existe donc des idempotents e_i de A (i ∈ I) tels que π(e_i) = c_i pour tout i ; comme e_i e_j est un idempotent tel que π(e_i e_j) = c_i c_j = 0 pour i ≠ j, on a e_i e_j = 0 pour i ≠ j (lemme 2) ; comme 1 − ∑_{i} e_i est un idempotent tel que π(1 − ∑_{i} e_i) = 1 − ∑_{i} c_i = 0, on a de même 1 = ∑_{i} e_i. Il en résulte que A est composé direct des idéaux α_i = e_i A et que π(α_i) = π(e_i)B = b_i.

Il reste à démontrer l’unicité d’une telle décomposition. Or, supposons A composé direct d’une seconde famille (α'_i)_{i∈I} d’idéaux avec π(α'_i) = b_i pour tout i ; on a alors 1 = ∑_{i} e'_i avec e'_i ∈ α'_i, d’où, dans B, 1 = ∑_{i} π(e'_i). avec π(e'_i) ∈ b_i, ce qui entraîne π(e'_i) = c_i ; comme e'_i et e_i sont des idempotents, on a nécessairement e'_i = e_i (lemme 2), ce qui achève la démonstration.

#### Remarque {#ac-iii-s4-n6-rem-1 .statement}

La prop. 8 redonne la structure d’un anneau semi-local A séparé et complet pour la topologie r-adique (r radical de A), déjà obtenue comme conséquence du § 2, n° 13, cor. de la prop. 19.

## EXERCICES {#ac-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
