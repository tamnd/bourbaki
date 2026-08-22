---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 4
section_title: Modules semi-simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.51-A VIII.71
pdf_pages: 0062-0082
extraction: native+ocr
subsections:
    - "no": 1
      title: Modules semi-simples
      page: 51
      pdf_page: 62
    - "no": 2
      title: L’homomorphisme $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$
      page: 53
      pdf_page: 64
    - "no": 3
      title: Quelques opérations sur les modules
      page: 53
      pdf_page: 64
    - "no": 4
      title: Modules isotypiques
      page: 57
      pdf_page: 68
    - "no": 5
      title: Description d’un module isotypique
      page: 58
      pdf_page: 69
    - "no": 6
      title: Composants isotypiques d’un module
      page: 61
      pdf_page: 72
    - "no": 7
      title: Description d’un module semi-simple
      page: 65
      pdf_page: 76
    - "no": 8
      title: Multiplicités et longueurs dans les modules semi-simples
      page: 67
      pdf_page: 78
statements: 43
exercises: 8
content_sha256: a0d3722e19f6e8d76a5199d17801f010b5d51c55605ae7f5c68991a91330a6a5
---

## § 4. MODULES SEMI-SIMPLES

### 1. Modules semi-simples

#### Définition 1 {#alg-viii-s4-def-1 .statement tag=0040}

On dit qu’un module est semi-simple s’il est somme directe d’une famille de modules simples[^1].

On dit qu’un multimodule est semi-simple s’il est somme directe d’une famille de multimodules simples (cf. I, p. 36, déf. 7).

Un A-module M est semi-simple si et seulement s’il est semi-simple lorsqu’on le considère comme module sur l’anneau $A_M$ de ses homothéties.

#### Exemple 1 {#alg-viii-s4-n1-exa-1 .statement tag=0041}

Un module réduit à 0, un module simple, sont des modules semi-simples.

#### Exemple 2 {#alg-viii-s4-n1-exa-2 .statement tag=0042}

Si A est un corps, tout A-module est semi-simple d’après le th. 1 de II, p. 95. Cela montre qu’en général un module semi-simple se décompose de plusieurs manières comme somme directe de sous-modules simples (voir cependant le cor. 2 de VIII, p. 63).

#### Exemple 3 {#alg-viii-s4-n1-exa-3 .statement tag=0043}

Soit A un anneau principal et soit P un système représentatif d’éléments extrémaux de A (VII, p. 3). Soit M un A-module et, pour tout $\pi \in P$, soit $M(\pi )$ l’ensemble des $x\in M$ tels que $\pi x= 0$. D’après VII, p. 9, le A-module M est semi-simple si et seulement s’il est somme des sous-modules $M(\pi )$; il est alors somme directe de ces sous-modules. Cet exemple sera généralisé plus loin (VIII, p. 61).

Soient $A_1$ et $A_2$ des algèbres sur un anneau commutatif K. On a défini en III, p. 38, la notion de bimodule à gauche sur les algèbres $A_1$ et $A_2$, et montré que cette notion équivaut à celle de module à gauche sur l’anneau $A_1\otimes_KA_2$. On dira que M est un bimodule simple (resp. semi-simple, de type fini) si c’est un module simple (resp. semi-simple, de type fini) sur l’anneau $A_1\otimes_KA_2$.

#### Théorème 1 {#alg-viii-s4-thm-1 .statement tag=0044}

Soit M un module somme (non nécessairement directe) d’une famille $(S_i)_{i\in I}$ de sous-modules simples et soit N un sous-module de M. Il existe une partie J de I telle que M soit somme directe de la famille formée de N et des modules $S_j$ pour $j$ parcourant J.

Soit $\mathscr{S}$ l’ensemble des parties $I'$ de I telles que la somme de la famille formée des modules N et $S_i$, pour $i$ dans $I'$, soit directe. L’ensemble $\mathscr{S}$ est de caractère fini : pour qu’une partie J de I appartienne à $\mathscr{S}$, il faut et il suffit qu’il en soit de même de toute partie finie de J. Donc l’ensemble $\mathscr{S}$ possède un élément maximal J (E, III, p. 35). Posons $N'= N +\sum_{j\in J}S_j$. Soit $i$ dans I - J ; comme J est maximal dans $\mathscr{S}$, l’ensemble $J\cup  \{i\}$ n’appartient pas à $\mathscr{S}$, de sorte que $S_i\cap N'\not= 0$; comme $S_i$ est un module simple, on a $S_i\cap N'= S_i$. On a donc $S_i\subset N'$ pour tout $i\in I$, d’où $N'= M$. Cela achève la démonstration.

#### Corollaire 1 {#alg-viii-s4-thm-1-cor-1 .statement tag=0045}

Tout module somme d’une famille de modules simples est semi-simple.

Il suffit d’appliquer le th. 1 au cas où N est nul.

#### Corollaire 2 {#alg-viii-s4-thm-1-cor-2 .statement tag=0046}

Pour qu’un module M soit semi-simple, il faut et il suffit que tout sous-module de M soit facteur direct.

La condition est nécessaire d’après le th. 1.

Réciproquement, supposons que tout sous-module de M admette un supplémentaire. Soit $M'$ la somme des sous-modules simples de M et soit $M''$ un supplémentaire de $M'$ dans M. Supposons qu’on ait $M'\not= M$, d’où $M''\not= 0$. Soit N un sous-module monogène non nul de $M''$. D’après la prop. 3 de VIII, p. 45, il existe un sous-module maximal P de N. Soit Q un sous-module supplémentaire de P dans M. Alors $N\cap Q$ est un sous-module de N, supplémentaire de P dans N, donc isomorphe à $N/P$ (II, p. 20, prop. 13). Par suite $N\cap Q$ est un sous-module simple de $M''$, contrairement à la définition de $M'$.

On a donc $M'= M$ et le module M est semi-simple d’après le cor. 1.

#### Corollaire 3 {#alg-viii-s4-thm-1-cor-3 .statement tag=0047}

Soient M un module semi-simple et N un sous-module de M. Les modules N et $M/N$sont semi-simples. Plus précisément, si M est somme directe d’une famille $(S_i)_{i\in I}$ de modules simples, il existe une partie J de I telle que $M/N$ soit isomorphe à $\bigoplus_{j\in J}S_j$ et N à $\bigoplus_{i\in I-J}S_i$.

Choisissons J comme dans le th. 1. Le module $N'=\bigoplus_{j\in J}S_j$ est un supplémentaire de N dans M, il est donc isomorphe à $M/N$. De plus, les sous-modules N et $\bigoplus_{i\in I-J}S_i$ de M sont tous deux supplémentaires de $N'$ et donc isomorphes à $M/N'$.

#### Corollaire 4 {#alg-viii-s4-thm-1-cor-4 .statement tag=0048}

Soit M un module semi-simple. Pour que M soit simple, il faut et il suffit que l’anneau E des endomorphismes de M soit un corps.

Si M est simple, E est un corps d’après le cor. de la prop. 2 de VIII, p. 43.

Si E est un corps, le module M est indécomposable (VIII, p. 28, prop. 4, a)). Comme il est en outre semi-simple, il est simple.

#### Remarque {#alg-viii-s4-n1-rem-1 .statement tag=0049}

Soient K un corps commutatif algébriquement clos et A une K-algèbre. Soit M un A-module semi-simple qui est un espace vectoriel de dimension finie sur le corps K. Pour que M soit simple, il faut et il suffit que tout endomorphisme du A-module M soit de la forme $x\rightarrow \alpha x$ avec $\alpha$ dans K : c’est nécessaire d’après le th. 1 de VIII, p. 43, et suffisant d’après le cor. 4 ci-dessus.

### 2. L’homomorphisme $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$

Soient A un anneau, M un A-module et $(N_i)_{i\in I}$ une famille de A-modules. À tout élément $(u_i)$ de $\bigoplus_i$ Hom$_A(M,N_i)$, associons l’élément $m\rightarrow (u_i(m))$ de Hom$_A(M,\bigoplus_iN_i)$. On définit ainsi un homomorphisme canonique

$\varphi :\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$.

Il est clair que $\varphi$ est injectif. Soit $u$ un élément de Hom$_A(M,\bigoplus_iN_i)$. Pour que $u$ appartienne à l’image de $\varphi$, il faut et il suffit que l’ensemble des indices $i$ tels que pr$_i\circ u\not= 0$ soit fini. Cette condition est automatiquement satisfaite lorsque le module M est de type fini.

Par conséquent, si le module M est de type fini, l’homomorphisme $\varphi$ est bijectif.

### 3. Quelques opérations sur les modules

Soient A et B des anneaux et soit P un $(A$, B)-bimodule (II, p. 33). On va définir deux procédés dont l’un fait passer d’un B-module à gauche à un A-module à gauche et l’autre d’un A-module à gauche à un B-module à gauche. 3.1. L’opération $\mathscr{T}$. — Soit V un B-module à gauche. Notons $\mathscr{T}(V)$ le A-module à gauche $P\otimes_BV$ (II, p. 54). Sa loi d’action est donnée par la formule

$$
a(p\otimes v) = (ap)\otimes v \tag{1}
$$

pour $a\in A,p\in P$ et $v\in V$.

Soit $V'$ un B-module à gauche. Pour toute application B-linéaire $g$ de V dans $V'$, l’application $1_P\otimes g$ de $\mathscr{T}(V)$ dans $\mathscr{T}(V')$ est A-linéaire ; on la notera $\mathscr{T}(g)$. L’application $g\rightarrow \mathscr{T}(g)$ de Hom$_B(V,V')$ dans Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$ est $\mathbf{Z}$-linéaire et l’on a

$$
\mathscr{T}(1_V) = 1_{\mathscr{T}(V)},\mathscr{T}(g'\circ g) =\mathscr{T}(g')\circ \mathscr{T}(g) \tag{2}
$$

si $V, V', V''$ sont des B-modules à gauche et $g: V\rightarrow V',g': V'\rightarrow V''$ des applications B-linéaires. Le produit tensoriel commutant aux sommes directes, si V est la somme directe d’une famille de sous-modules $(V_i)_{i\in I}$, on peut identifier le A-module $\mathscr{T}(V)$ avec $\bigoplus_i\mathscr{T}(V_i)$.

3.2. L’opération $\mathscr{H}$. — Soit M un A-module à gauche. Notons $\mathscr{H}(M)$ le B-module à gauche Hom$_A(P,M)$ (II, p. 34). Sa loi d’action est donnée par la formule

$$
(bf)(p) =f(pb) \tag{3}
$$

pour $b\in B,f\in$ Hom$_A(P,M)$ et $p\in P$.

Soit $M'$ un A-module à gauche. Pour toute application A-linéaire $g$ de M dans $M'$, l’application Hom$_A(1_P, g)$ de $\mathscr{H}(M)$ dans $\mathscr{H}(M')$ est B-linéaire ; on la notera $\mathscr{H}(g)$. L’application $g\rightarrow \mathscr{H}(g)$ de Hom$_A(M,M')$ dans Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))$ est $\mathbf{Z}$-linéaire et l’on a

$$
\mathscr{H}(1_M) = 1_{\mathscr{H}(M)},\mathscr{H}(g'\circ g) =\mathscr{H}(g')\circ \mathscr{H}(g) \tag{4}
$$

si $M, M', M''$ sont des A-modules à gauche et $g: M\rightarrow M',g': M'\rightarrow M''$ des applications A-linéaires. Supposons en outre que P soit un A-module de type fini ; si M est la somme directe d’une famille de sous-modules $(M_i)_i$ alors on peut identifier $\mathscr{H}(M)$ à $\bigoplus_i\mathscr{H}(M_i)$ d’après VIII, p. 53.

3.3. Relations entre $\mathscr{T}$ et $\mathscr{H}$. — D’après la prop. 1 de II, p. 74, pour tout A-module à gauche M et tout B-module à gauche V, il existe un unique isomorphisme de groupes

(5) $\gamma :$ Hom$_A(\mathscr{T}(V),M)\longrightarrow$ Hom$_B(V,\mathscr{H}(M))$ caractérisé par la relation

(6)
$$(\gamma(h)(v))(p) = h(p \otimes v)$$

pour $ h \in \operatorname{Hom}_A(\mathscr{T}(V), M) $, $ v \in V $ et $ p \in P $. L’isomorphisme $ \gamma $ est appelé *isomorphisme d’adjonction*.

Soit $ M $ un A-module à gauche. Le A-module $ \mathscr{T}(\mathscr{H}(M)) $ n’est autre que le A-module $ P \otimes_B \operatorname{Hom}_A(P, M) $. En appliquant ce qui précède au B-module $ \mathscr{H}(M) $, l’application
$$\alpha_M = \gamma^{-1}(\operatorname{Id}_{\mathscr{H}(M)}) : \mathscr{T}(\mathscr{H}(M)) \longrightarrow M$$
est l’unique application satisfaisant à
(7)
$$\alpha_M(p \otimes f) = f(p)$$
pour $ p \in P $ et $ f \in \operatorname{Hom}_A(P, M) $. Nous dirons que $ \alpha_M $ est l’application A-linéaire canonique de $ \mathscr{T}(\mathscr{H}(M)) $ dans $ M $. Pour toute application A-linéaire $ g : M \to M' $, on a un diagramme commutatif

(I)
$$
\begin{array}{ccc}
\mathscr{T}(\mathscr{H}(M)) & \xrightarrow{\alpha_M} & M \\
\downarrow \mathscr{T}(\mathscr{H}(g)) & & \downarrow g \\
\mathscr{T}(\mathscr{H}(M')) & \xrightarrow{\alpha_{M'}} & M'.
\end{array}
$$

L’inverse
$$\gamma^{-1} : \operatorname{Hom}_B(V, \mathscr{H}(M)) \longrightarrow \operatorname{Hom}_A(\mathscr{T}(V), M)$$
de l’isomorphisme d’adjonction coïncide avec l’application $ f \mapsto \alpha_{M'} \circ \mathscr{T}(f) $. En effet, d’après (6) et (7) on a les relations
$$\gamma^{-1}(f)(p \otimes v) = (f(v))(p) = \alpha_{M'}(p \otimes f(v)) = \alpha_{M'} \circ \mathscr{T}(f)(p \otimes v)$$
pour tous $ f \in \operatorname{Hom}_B(V, \mathscr{H}(M)) $, $ v \in V $ et $ p \in P $.

Soit $ V $ un B-module. Le B-module $ \mathscr{H}(\mathscr{T}(V)) $ n’est autre que le B-module $ \operatorname{Hom}_A(P, P \otimes_B V) $. En appliquant (5) au A-module $ \mathscr{T}(V) $, l’application B-linéaire $ \beta_V = \gamma(\operatorname{Id}_{\mathscr{T}(V)}) $ de $ V $ dans $ \mathscr{H}(\mathscr{T}(V)) $ est caractérisée par la relation
(8)
$$\beta_V(v)(p) = p \otimes v$$
pour $ p \in P $ et $ v \in V $. Nous dirons que $ \beta_V $ est l’application B-linéaire canonique de $ V $ dans $ \mathscr{H}(\mathscr{T}(V)) $. Pour tout B-module $ V' $ et toute application B-linéaire $ g : V \to V' $, on a un diagramme commutatif

(II)

$$
\begin{array}{ccc}
V & \xrightarrow{\beta_V} & \mathcal{H}(\mathcal{T}(V)) \\
\downarrow g & & \downarrow \mathcal{H}(\mathcal{T}(g)) \\
V' & \xrightarrow{\beta_{V'}} & \mathcal{H}(\mathcal{T}(V')).
\end{array}
$$

Notons que le morphisme d’adjonction (5) coïncide avec l’application qui envoie $ u $ sur $ \mathcal{H}(u) \circ \beta_V $. En effet, des relations (6) et (8), on déduit les égalités

$$(\gamma(u)(v))(p) = u(p \otimes v) = u \circ (\beta_V(v))(p)$$

pour tous $ u \in \operatorname{Hom}_A(\mathcal{T}(V), M) $, $ v \in V $ et $ p \in P $.

#### Remarque 1 {#alg-viii-s4-n3-rem-1 .statement tag=004A}

Soient $ V $ et $ V' $ des $ B $-modules. L’isomorphisme d’adjonction

$$\gamma : \operatorname{Hom}_A(\mathcal{T}(V), \mathcal{T}(V')) \longrightarrow \operatorname{Hom}_B(V, \mathcal{H}(\mathcal{T}(V)))$$

vérifie la relation $ \gamma(\mathcal{T}(f)) = \beta_{V'} \circ f $ pour tout $ f \in \operatorname{Hom}_B(V, V') $, puisque

$$(\gamma(\mathcal{T}(f))(v))(p) = \mathcal{T}(f)(p \otimes v) = p \otimes f(v) = (\beta_{V'} \circ f)(v)(p).$$

Soient $ M $ et $ M' $ des $ A $-modules ; l’inverse de l’isomorphisme d’adjonction

$$\gamma^{-1} : \operatorname{Hom}_B(\mathcal{H}(M), \mathcal{H}(M')) \longrightarrow \operatorname{Hom}_A(\mathcal{T}(\mathcal{H}(M)), M')$$

vérifie la relation $ \gamma^{-1}(\mathcal{H}(u)) = u \circ \alpha_M $, pour tout $ u \in \operatorname{Hom}_B(M, M') $. En effet, on a les relations

$$\gamma^{-1}(\mathcal{H}(u))(p \otimes v) = (\mathcal{H}(u)(v))(p) = u(v(p)) = u \circ \alpha_M(p \otimes v)$$

pour tous $ u \in \operatorname{Hom}_B(M, M') $, $ v \in \mathcal{H}(M) $ et $ p \in P $.

#### Remarque 2 {#alg-viii-s4-n3-rem-2 .statement tag=004B}

Soit $ M $ un $ A $-module à gauche. Les applications $ B $-linéaires

$$\beta_{\mathcal{H}(M)} : \mathcal{H}(M) \to \mathcal{H}(\mathcal{T}(\mathcal{H}(M))) \quad \text{et} \quad \mathcal{H}(\alpha_M) : \mathcal{H}(\mathcal{T}(\mathcal{H}(M))) \to \mathcal{H}(M)$$

satisfont la relation $ \mathcal{H}(\alpha_M) \circ \beta_{\mathcal{H}(M)} = 1_{\mathcal{H}(M)} $. Elles ne sont pas bijectives en général.

Soit $ V $ un $ B $-module à gauche. Les applications $ A $-linéaires

$$\mathcal{T}(\beta_V) : \mathcal{T}(V) \to \mathcal{T}(\mathcal{H}(\mathcal{T}(V))) \quad \text{et} \quad \alpha_{\mathcal{T}(V)} : \mathcal{T}(\mathcal{H}(\mathcal{T}(V))) \to \mathcal{T}(V)$$

satisfont la relation $ \alpha_{\mathcal{T}(V)} \circ \mathcal{T}(\beta_V) = 1_{\mathcal{T}(V)} $. Elles ne sont pas bijectives en général.

#### Remarque 3 {#alg-viii-s4-n3-rem-3 .statement tag=004C}

Supposons que $ P $ soit de type fini en tant que $ A $-module. Soit $ M $ la somme directe d’une famille $ (M_i)_{i \in I} $ de $ A $-modules. Les $ A $-modules $ \mathcal{T}(\mathcal{H}(M)) $ et $ \bigoplus_i \mathcal{T}(\mathcal{H}(M_i)) $ sont canoniquement isomorphes. Lorsqu’on les identifie, $ \alpha_M $ s’identifie à $ \bigoplus_i \alpha_{M_i} $. De même, soit $ V $ la somme directe d’une famille $ (V_j)_{j \in J} $ de $ B $-modules. Le B-module $\mathscr{H}(\mathscr{T}(V))$ s’identifie à $\bigoplus_j\mathscr{H}(\mathscr{T}(V_j))$ et l’application linéaire $\beta_V$ à $\bigoplus_j\beta_{V_j}$.

### 4. Modules isotypiques

Soient A un anneau et S un A-module à gauche simple. Notons D l’anneau opposé de l’anneau des endomorphismes de S ; c’est un corps. Muni des actions de A et de D, S est un $(A$, D)-bimodule.

#### Proposition 1 {#alg-viii-s4-prop-1 .statement tag=004D}

Soit M un A-module. Les conditions suivantes sont équivalentes :

(i) Il existe un ensemble I tel que M soit isomorphe à $S^{(I)}$;

(ii) Le module M est somme directe d’une famille de sous-modules isomorphes à S ;

(iii) Le module M est somme d’une famille de sous-modules isomorphes à S ;

(iv) Il existe un espace vectoriel à gauche V sur le corps D tel que le A-module M soit isomorphe à $S\otimes_DV$.

L’équivalence de (i) et (ii) est immédiate et celle de (ii) et (iii) résulte du th. 1 de VIII, p. 52 appliqué au cas où N = 0. Tout espace vectoriel à gauche sur D est isomorphe à un espace vectoriel de la forme $D^{(I)}_s$, où I est un ensemble (II, p. 95, th. 1). Comme le produit tensoriel commute aux sommes directes, (i) équivaut à (iv).

#### Définition 2 {#alg-viii-s4-def-2 .statement tag=004E}

On dit qu’un A-module M est isotypique de type S s’il satisfait aux conditions équivalentes de la prop. 1. On dit que M est isotypique s’il existe un A-module simple T tel que M soit isotypique de type T.

Tout module isotypique est semi-simple.

#### Proposition 2 {#alg-viii-s4-prop-2 .statement tag=004F}

Si un module est somme de sous-modules isotypiques de type S, il est isotypique de type S. Les sous-modules et les modules quotients d’un module isotypique de type S sont isotypiques de type S.

La première assertion résulte des définitions, la seconde du cor. 3 de VIII, p. 52.

#### Remarque {#alg-viii-s4-n4-rem-1 .statement tag=004G}

Tout module isotypique non nul de type S possède un module quotient et un sous-module isomorphes à S ; par conséquent, si M et $M'$ sont des A-modules isotypiques non nuls de type S, le groupe Hom$_A(M,M')$ n’est pas réduit à 0.

#### Proposition 3 {#alg-viii-s4-prop-3 .statement tag=004H}

a) Soit M un A-module isotypique de type S. L’application A-linéaire $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$caractérisée par $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 55) est bijective.

b) Soit V un espace vectoriel à gauche sur le corps D. L’application D-linéaire $\beta_V: V\rightarrow$ Hom$_A(S,S\otimes_DV)$définie par $\beta_V(v)(s) =s\otimes v$ (VIII, p. 55) est bijective.

Notons $\mathscr{H}(M)$ le D-espace vectoriel à gauche Hom$_A(S,M)$. Le A-module M est par hypothèse somme directe d’une famille de sous-modules isomorphes à S. Le A-module S est monogène ; pour démontrer que l’application $\alpha_M$ est bijective, il suffit donc de considérer le cas où M = S (VIII, p. 56, remarque 3). Or $\mathscr{H}(S)$ n’est autre que le D-espace vectoriel $D_s$ et $\alpha_S$ n’est autre que l’isomorphisme $\iota : S\otimes_DD_s\rightarrow S$ défini par $\iota (s\otimes d) =sd$.

Il suffit de même, pour démontrer b), de considérer le cas où $V = D_s$. Or, comme l’application $\alpha_S$ est bijective, l’application $\beta_{D_s}=\beta_{\mathscr{H}(S)}$ l’est aussi (VIII, p. 56, remarque 2).

### 5. Description d’un module isotypique

Comme dans le numéro précédent, A désigne un anneau, S un A-module à gauche simple et D le corps End$_A(S)^o$. On considère S comme un $(A$, D)-bimodule.

#### Définition 3 {#alg-viii-s4-def-3 .statement tag=004I}

Soit M un A-module isotypique de type S. Une description de M relative à S est un couple $(V, \alpha )$, où V est un espace vectoriel à gauche sur le corps D et $\alpha : S\otimes_DV\rightarrow M$un isomorphisme de A-modules.

Tout A-module M isotypique de type S possède une description canonique : c’est le couple (Hom$_A(S,M), \alpha_M$) où $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$ est l’isomorphisme de A-modules caractérisée par $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 58, prop. 3 a)).

#### Théorème 2 {#alg-viii-s4-thm-2 .statement tag=004J}

Soient M un A-module isotypique de type S et $(V, \alpha )$une description de M. Notons $\mathscr{D}_D(V)$l’ensemble, ordonné par inclusion, des sous-D-espaces vectoriels de V et $\mathscr{D}_A(M)$celui des sous-A-modules de M. Identifions pour tout $W\in \mathscr{D}_D(V)$le A-module $S\otimes_DW$à son image canonique dans $S\otimes_DV$.

a) L’application $W\rightarrow \alpha (S\otimes_DW)$est un isomorphisme d’ensembles ordonnés de $\mathscr{D}_D(V)$sur $\mathscr{D}_A(M)$.

b) L’isomorphisme réciproque fait correspondre à un sous-module N de M le sous-espace vectoriel de V formé des éléments $v$ tels que $\alpha (s\otimes v)$appartienne à N pour tout $s\in S$.

Pour tout $W\in \mathscr{D}_D$(V), posons $\varphi (W) =\alpha (S\otimes_DW)$. Pour tout $N\in \mathscr{D}_A$(M), notons $\psi (N)$ l’ensemble des éléments $v\in V$ tels que $\alpha (s\otimes v)\in N$ pour tout $s\in S$. On définit ainsi deux applications $\varphi :\mathscr{D}_D(V)\rightarrow \mathscr{D}_A(M)$ et $\psi :\mathscr{D}_A(M)\rightarrow \mathscr{D}_D(V)$. Elles sont clairement croissantes.

Soit N un sous-module de M. Il est isotypique de type S (VIII, p. 57, prop. 2). Posons $W =\psi (N)$. D’après la prop. 3, b) de VIII, p. 58, les applications A-linéaires $h: S\rightarrow M$ ne sont autres que les applications $s\rightarrow \alpha (s\otimes v)$, où $v$ parcourt V. Celles dont l’image est contenue dans N sont les applications $s\rightarrow \alpha (s\otimes w)$, où $w$ parcourt W ; leurs images engendrent N, puisque N est isotypique de type S. On a donc $\alpha (S\otimes_DW) = N$, c’est-à-dire $\varphi (\psi (N)) = N$. Cela prouve que $\varphi \circ \psi$ est l’application identique de $\mathscr{D}_A(M)$. En particulier $\varphi$ est surjective et $\psi$ injective.

Pour terminer la démonstration, il suffit de prouver que l’application $\varphi$ est injective. Soient W et $W'$ des sous-espaces vectoriels de V tels que $\varphi (W) =\varphi (W')$. Les espaces vectoriels $S\otimes_DW$ et $S\otimes_DW'$ vus comme sous-espaces vectoriels de $S\otimes_DV$ coïncident. Choisissons une forme linéaire non nulle $f$ sur le D-espace vectoriel S et notons $g: S\otimes_DV\rightarrow V$ l’homomorphisme de groupes défini par $g(s\otimes v) =f(s)v$. On a $W =g(S\otimes_DW) =g(S\otimes_DW') = W'$, d’où l’injectivité de $\varphi$.

#### Remarque 1 {#alg-viii-s4-n5-rem-1 .statement tag=004K}

Soit M un A-module isotypique de type S et $(V, \alpha )$ une description de M. Alors M est de longueur finie si et seulement si V est de dimension finie et on a dans ce cas la relation

long$_A(M) =$ dim$_D(V)$.

#### Corollaire 1 {#alg-viii-s4-thm-2-cor-1 .statement tag=004L}

Soit M un A-module isotypique de type S. Pour tout sous-A-module N de M, identifions Hom$_A(S,N)$au sous-D-espace vectoriel de Hom$_A(S,M)$ formé des applications dont l’image est contenue dans N.

a) L’application $N\rightarrow$ Hom$_A(S,N)$est un isomorphisme d’ensembles ordonnés de $\mathscr{D}_A(M)$sur $\mathscr{D}_D$(Hom$_A(S,M)$).

b) La bijection réciproque associe à tout sous-espace vectoriel W de Hom$_A(S,M)$ le sous-module $\sum_{h\in W}h(S)$de M.

C’est une traduction du th. 2, lorsqu’on prend pour $(V, \alpha )$ la description canonique de M.

#### Corollaire 2 {#alg-viii-s4-thm-2-cor-2 .statement tag=004M}

Soient V un espace vectoriel à gauche sur D et $\mathscr{F}$ un ensemble d’endomorphismes de V. Pour qu’un sous-A-module de $S\otimes_DV$soit stable par tous les endomorphismes $1_S\otimes u$, où $u$ parcourt $\mathscr{F}$, il faut et il suffit qu’il soit de la forme $S\otimes_DW$, où W est un sous-espace vectoriel de V stable par tous les endomorphismes appartenant à $\mathscr{F}$.

En effet, d’après le th. 2, tout sous-A-module N de S $ \otimes_D V $ est égal à S $ \otimes_D W $, où W est le sous-espace vectoriel de V formé des éléments $ v $ tels que $ s \otimes v $ appartienne à N pour tout $ s \in S $.

#### Théorème 3 {#alg-viii-s4-thm-3 .statement tag=004N}

Soient M et M' des A-modules isotypiques de type S. Soient (V, $ \alpha $) et (V', $ \alpha' $) des descriptions de M et M' respectivement. Pour toute application D-linéaire $ f : V \to V' $, Notons $ \tilde{f} : M \to M' $ l’unique application A-linéaire rendant commutatif le diagramme

$$
\begin{array}{ccc}
S \otimes_D V & \xrightarrow{\alpha} & M \\
| & & | \\
S \otimes_D V' & \xrightarrow{\alpha'} & M'.
\end{array}
$$

L’application $ f \mapsto \tilde{f} $ de $ \operatorname{Hom}_D(V, V') $ dans $ \operatorname{Hom}_A(M, M') $ est un isomorphisme de groupes.

Il nous suffit de démontrer que l’application $ \mathbf{Z}$-linéaire $ u \mapsto 1_S \otimes u $ de $ \operatorname{Hom}_D(V, V') $ dans $ \operatorname{Hom}_A(S \otimes_D V, S \otimes_D V') $ est bijective. En reprenant les notations du n°3 appliqué au (A, D)-bimodule S, cela revient à montrer que l’application
$$
\mathscr{T} : \operatorname{Hom}_D(V, V') \longrightarrow \operatorname{Hom}_A(\mathscr{T}(V), \mathscr{T}(V'))
$$
est bijective. Mais d’après la remarque 1 de VIII, p. 56, comme l’isomorphisme d’adjonction (VIII, p. 54) est bijectif, cela revient à montrer que l’application qui envoie $ u $ sur $ \beta_{V'} \circ u $ est bijective, ce qui résulte du fait que l’application D-linéaire $ \beta_{V'} $ est bijective (VIII, p. 58, prop. 3 b)).

Conservons les notations du th. 3. Soit $ M'' $ un A-module isotypique de type S et soit $ (V'', \alpha'') $ une description de $ M'' $. Pour tout $ f \in \operatorname{Hom}_D(V, V') $ et tout $ g $ appartenant à $ \operatorname{Hom}_D(V', V'') $, on a $ \widetilde{g \circ f} = \widetilde{g} \circ \widetilde{f} $. En particulier, pour $ M = M', V = V' $ et $ \alpha = \alpha' $, l’application $ f \mapsto \tilde{f} $ de $ \operatorname{End}_D(V) $ dans $ \operatorname{End}_A(M) $ est un isomorphisme d’anneaux.

#### Remarque 2 {#alg-viii-s4-n5-rem-2 .statement tag=004O}

Soit M un A-module isotypique de type S et soit $ (V, \alpha) $ une description de M. Soit B un sous-anneau de l’anneau $ \operatorname{End}_A(M)^o $. L’isomorphisme d’anneaux de $ \operatorname{End}_D(V)^o $ sur $ \operatorname{End}_A(M)^o $ munit V d’une structure de (D, B)-bimodule de sorte que $ \alpha $ est un isomorphisme de (A, B)-bimodules. Il existe un isomorphisme de l’ensemble des sous-(D, B)-bimodules de V, ordonnés par l’inclusion sur celui des sous-(A, B)-bimodules de M (VIII, p. 58, th. 2 et VIII, p. 59, cor. 2).

#### Corollaire {#alg-viii-s4-n5-cor-1 .statement tag=004P}

Soient M, M' des A-modules isotypiques de type S. L’application $ u \mapsto \operatorname{Hom}(1_S, u) $ de $ \operatorname{Hom}_A(M, M') $ dans $ \operatorname{Hom}_D(\operatorname{Hom}_A(S, M), \operatorname{Hom}_A(S, M')) $ est un isomorphisme de groupes. Lorsque M est égal à $M'$, c’est un isomorphisme d’anneaux de End$_A(M)$sur End$_D$(Hom$_A(S,M)$).

Compte tenu de la commutativité du diagramme (I) de VIII, p. 55 ce corollaire résulte du th. 3, appliqué aux descriptions canoniques de M et $M'$.

### 6. Composants isotypiques d’un module

#### Définition 4 {#alg-viii-s4-def-4 .statement tag=004Q}

Soient A un anneau, M un A-module et S un A-module simple. On appelle composant isotypique de type S de M, et l’on note $M_S$, la somme des sous-modules de M isomorphes à S.

Il est clair que $M_S$ est le plus grand sous-module de M qui soit isotypique de type S. Comme tout sous-module de $M_S$ est isotypique de type S (VIII, p. 57, prop. 2), on a $N_S= M_S\cap N$ pour tout sous-module N de M.

Si $S'$ est un A-module simple isomorphe à S, on a évidemment $M_S= M_{S'}$, donc $M_S$ ne dépend que de la classe de S (VIII, p. 47).

Soit M un A-module. Il existe un plus grand sous-module semi-simple de M, qu’on appelle le socle de M ; c’est la somme des sous-modules simples de M, et aussi la somme des composants isotypiques de M. En particulier, M est semi-simple si et seulement s’il est égal à son socle.

#### Proposition 4 {#alg-viii-s4-prop-4 .statement tag=004R}

Soit A un anneau. Désignons par $\mathscr{S}$ l’ensemble des classes de A-modules simples. Soit M un A-module semi-simple.

a) Le module M est somme directe de la famille $(M_{\lambda})_{\lambda\in\mathscr{S}}$ de ses composants isotypiques.

b) Supposons que M soit somme directe d’une famille $(N_i)_{i\in I}$ de sous-modules simples. Pour tout $\lambda \in \mathscr{S}$, soit $I(\lambda )$l’ensemble des indices $i\in I$tels que $N_i$ soit de classe $\lambda$. On a $M_{\lambda}=\bigoplus_{i\in I(\lambda)}N_i$.

c) Si M est de type fini, l’ensemble des $\lambda \in \mathscr{S}$ tels que $M_{\lambda}\not= 0$est fini.

d) Pour tout sous-module N de M, et tout $\lambda \in \mathscr{S}$, on a $N_{\lambda}= N\cap M_{\lambda}$ et $(M/N)_{\lambda}= (M_{\lambda}+ N)/N$.

Comme M est semi-simple, il est somme de la famille $(M_{\lambda})_{\lambda\in\mathscr{S}}$, prouvons que cette somme est directe. Soit $\lambda \in \mathscr{S}$. Notons $M'_{\lambda}$ la somme de la famille $(M_{\mu})_{\mu\in\mathscr{S}-\{\lambda\}}$. Le module $M'_{\lambda}$ est somme directe d’une famille de modules simples non isomorphes à $\lambda$ (VIII, p. 52, th. 1). D’après le cor. 3 du th. 1 de VIII, p. 52, $M'_{\lambda}$ ne contient aucun sous-module simple de classe $\lambda$. On a donc $M_{\lambda}\cap M'_{\lambda}= 0$. L’assertion a) est donc démontrée. Par construction, on a $M_{\lambda}\supset \bigoplus_{i\in I(\lambda)}N_i$, l’assertion b) résulte alors de II, p. 18, remarque 1.

L’assertion c) résulte de a) et de (II, p. 29, prop. 23).

Soit N un sous-module de M et $\lambda \in \mathscr{S}$. Le composant isotypique $N_{\lambda}$ de N est contenu dans $M_{\lambda}$ et $M_{\lambda}\cap N\subset N_{\lambda}$. L’intersection $N\cap M_{\lambda}$ est donc le composant isotypique de type $\lambda$ de N.

Pour tout $\lambda \in S$, le module $M_{\lambda}+ N/N$ est isomorphe à $M_{\lambda}/(M_{\lambda}\cap N)$. Il est donc isotypique de type $\lambda$ et contenu dans $(M/N)_{\lambda}$. La dernière assertion résulte alors de a) et de II, p. 18, remarque 1.

#### Corollaire {#alg-viii-s4-n6-cor-1 .statement tag=004S}

Soit A un anneau et $\mathscr{S}$ l’ensemble des classes de A-modules simples. Soit M un A-module semi-simple et N un sous-module de M. Alors on a $N =\bigoplus_{\lambda\in\mathscr{S}}N\cap M_{\lambda}$ et $M/N =\bigoplus_{\lambda\in\mathscr{S}}(M_{\lambda}+ N)/N$.

Comme N et $M/N$ sont semi-simple (VIII, p. 52, cor. 3), le corollaire résulte de la prop. 4 d).

On appelle support d’un A-module semi-simple M l’ensemble des classes $\lambda$ de A-modules simples telles que le composant isotypique de M de type $\lambda$ soit non nul. Le support d’un A-module semi-simple de type fini est fini.

#### Proposition 5 {#alg-viii-s4-prop-5 .statement tag=004T}

Soit A un anneau et soit $\mathscr{S}$ l’ensemble des classes de A-modules simples. Soient M et N des A-modules.

a) Soit $f: M\rightarrow N$un homomorphisme. Pour tout $\lambda \in \mathscr{S},f$ induit un homomorphisme $f_{\lambda}$ de $M_{\lambda}$ dans $N_{\lambda}$;si M est semi-simple et $f$ surjectif, chacun des homomorphismes $f_{\lambda}$ est surjectif.

b) Supposons M semi-simple. L’application $f\rightarrow (f_{\lambda})_{\lambda\in\mathscr{S}}$ est un isomorphisme de groupes de Hom$_A(M,N)$sur $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(M_{\lambda},N_{\lambda})$. Lorsque M est égal à N, c’est un isomorphisme d’anneaux de End$_A(M)$sur $\prod_{\lambda\in\mathscr{S}}$ End$_A(M_{\lambda})$.

Pour tout $\lambda \in \mathscr{S}$, le sous-module $f(M_{\lambda})$ de N est isomorphe à un quotient d’un module isotypique de type $\lambda$; il est donc isotypique de type $\lambda$, et par suite, contenu dans $N_{\lambda}$.

Supposons que M soit semi-simple et $f$ surjectif. Alors $f$ induit un isomorphisme de $M/$ Ker($f$) sur N qui envoie $(M_{\lambda}+$ Ker($f$))$/$ Ker($f$) sur $f(M_{\lambda})$. D’apres la prop. 4 de VIII, p. 61, $N_{\lambda}=f(M_{\lambda})$ ce qui termine la démonstration de a).

L’application considérée dans b) est clairement un homomorphisme de groupes et c’est un homomorphisme d’anneaux lorsque M est égal à N. Soit $(f_{\lambda})_{\lambda\in\mathscr{S}}$ un élément de $\prod_{\lambda\in\mathscr{S}}$ Hom(M$_{\lambda},N_{\lambda}$). Son unique antécédent par l’application de b) est l’homomorphisme $f: M\rightarrow N$ défini par

$$
f((\sum_{\lambda\in\mathscr{S}}x_{\lambda})=\sum_{\lambda\in\mathscr{S}}f_{\lambda}(x_{\lambda})
$$

pour tout $(x_{\lambda})_{\lambda\in\mathscr{S}}\in \bigoplus_{\lambda}M_{\lambda}$.

#### Remarque {#alg-viii-s4-n6-rem-1 .statement tag=004U}

Soient A et B des anneaux. Soit M un $(A$, B)-bimodule. Il résulte de la prop. 5 que les composants isotypiques du A-module M sont des sous-bimodules de M. Cela s’applique en particulier lorsque M est un A-module et B l’anneau opposé de End$_A(M)$.

#### Exemple {#alg-viii-s4-n6-exa-1 .statement tag=004V}

Examinons le cas où l’anneau A est commutatif. L’application qui envoie un idéal maximal $\mathfrak{m}$ sur cl(A$/\mathfrak{m}$) est une bijection de l’ensemble des idéaux maximaux de A sur l’ensemble $\mathscr{S}$ des classes de A-modules simples (VIII, p. 47). La bijection réciproque associe à $\lambda$ son annulateur $\mathfrak{m}_{\lambda}$.

Soit N un A-module. Pour tout $\lambda \in \mathscr{S}$, le composant isotypique $M_{\lambda}$ de M est formé des éléments annulés par $\mathfrak{m}_{\lambda}$ et l’on peut considérer $M_{\lambda}$ comme un espace vectoriel sur le corps $A/\mathfrak{m}_{\lambda}$. Si M est semi-simple et si N est un autre A-module, on déduit de la prop. 5 un isomorphisme de groupes de Hom$_A(M,N)$ sur $\prod_{\lambda\in\mathscr{S}}$ Hom$_{A/\mathfrak{m}_{\lambda}}(M_{\lambda},N_{\lambda})$.

#### Corollaire 1 {#alg-viii-s4-prop-5-cor-1 .statement tag=004W}

Soient M un A-module semi-simple et N un sous-module de M. Les conditions suivantes sont équivalentes :

(i) Il existe un unique sous-module supplémentaire de N dans M ;

(ii) On a Hom$_A(M/N,N) = 0$;

(iii) Il existe une partie Λ de $\mathscr{S}$ telle que $N =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$.

Choisissons un sous-module $N'$ supplémentaire de N dans M (VIII, p. 52, cor. 2) ; si l’on identifie M à $N'\times N$, les sous-modules de M supplémentaires de N sont les graphes des applications A-linéaires de $N'$ dans N ; comme $N'$ est isomorphe à $M/N$, on a prouvé l’équivalence des propriétés (i) et (ii). D’après la prop. 5, b), le groupe Hom$_A(N',N)$ est isomorphe au groupe $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(N'_{\lambda},N_{\lambda})$. Il est nul si et seulement si, pour tout $\lambda \in \mathscr{S}$, on a $N_{\lambda}= 0$ ou $N'_{\lambda}= 0$ (VIII, p. 57, remarque), c’est-à-dire $N_{\lambda}= 0$ ou $N_{\lambda}= M_{\lambda}$. Cela prouve l’équivalence des conditions (ii) et (iii).

#### Corollaire 2 {#alg-viii-s4-prop-5-cor-2 .statement tag=00R0}

Soit M un A-module. Les deux conditions suivantes sont équivalentes :

(i) Tout sous-module de M admet un unique sous-module supplémentaire.

(ii) M est somme directe d’une famille $(S_i)_{i\in I}$ de modules simples, deux à deux non isomorphes. Supposons que M vérifie ces conditions. Alors, pour tout sous-module N de M, il existe une unique partie J de I telle qu’on ait $N =\bigoplus_{j\in J}S_j$ et tout sous-module simple de M est égal à l’un des $S_i$.

Chacune des propriétés (i) et (ii) entraîne que M est semi-simple.

Supposons la condition (i) satisfaite. Soit $\lambda \in \mathscr{S}$. D’après l’équivalence de (i) et (iii) dans le cor. 1, tout sous-module de $M_{\lambda}$ est nul ou égal à $M_{\lambda}$. Par suite, $M_{\lambda}$ est nul ou simple et (ii) résulte de ce que M est somme directe de la famille $(M_{\lambda})_{\lambda\in\mathscr{S}}$.

Inversement, si la condition (ii) est satisfaite, $M_{\lambda}$ est nul ou simple pour tout $\lambda \in \mathscr{S}$; si N est un sous-module de M, alors $N\cap M_{\lambda}$ est égal à 0 ou $M_{\lambda}$ pour tout $\lambda \in \mathscr{S}$; comme on a $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 62, cor.), le sous-module N satisfait à la condition (iii) du cor. 1, donc admet un unique sous-module supplémentaire dans M. Cela prouve que (ii) implique (i), ainsi que les dernières assertions du corollaire.

Soient M un A-module et S un A-module simple. Notons D l’anneau opposé du corps End$_A(S)$ et considérons S comme un $(A$, D)-bimodule. Alors Hom$_A(S,M)$ est un espace vectoriel à gauche sur D et Hom$_A(M,S)$ un espace vectoriel à droite sur D. Le dual du D-espace vectoriel à gauche Hom$_A(S,M)$ est un espace vectoriel à droite sur D (II, p. 40, déf. 2). Pour tout $u\in$ Hom$_A(M,S)$, l’application $h(u) :v\rightarrow u\circ v$ de Hom$_A(S,M)$ dans Hom$_A(S,S) = D$ est une forme linéaire sur le D-espace vectoriel à gauche Hom$_A(S,M)$.

#### Proposition 6 {#alg-viii-s4-prop-6 .statement tag=004X}

Conservons les notations ci-dessus et supposons le A-module M semi-simple. L’application $u\rightarrow h(u)$du D-espace vectoriel à droite Hom$_A(M,S)$ dans le dual du D-espace vectoriel à gauche Hom$_A(S,M)$est D-linéaire et bijective.

Soient $u\in$ Hom$_A(M,S),v\in$ Hom$_A(S,M)$ et $d\in D$. On a

$$
h(ud)(v) =h(d\circ u)(v) =d\circ u\circ v=d\circ (h(u)(v)) =h(u)(v)d
$$

Cela prouve que l’application $h$ est D-linéaire. Elle n’est autre que l’application donnée par $u\rightarrow$ Hom(1$_S, u$) de Hom$_A(M,S)$ dans Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,S)$). Pour démontrer qu’elle est bijective, il suffit d’après la prop. 5, b) de VIII, p. 62, de traiter le cas où le A-module M est isotypique de type S et on peut alors appliquer le cor. de VIII, p. 60.

### 7. Description d’un module semi-simple

Jusqu’à la fin de ce paragraphe, on note A un anneau et $\mathscr{S}$ l’ensemble des classes de A-modules simples. Pour tout $\lambda \in \mathscr{S}$, on choisit un module simple $S_{\lambda}$ de classe $\lambda$ (par exemple $S_{\lambda}=\lambda$ ) et l’on note $D_{\lambda}$ l’anneau opposé du corps des endomorphismes de $S_{\lambda}$; on considère $S_{\lambda}$ comme un $(A,D_{\lambda}$)-bimodule.

Soit M un A-module. Pour tout $\lambda \in \mathscr{S}$, Hom$_A(S_{\lambda},M)$ est un espace vectoriel à gauche sur le corps $D_{\lambda}$. D’après VIII, p. 55 et II, p. 12, prop. 6, il existe une unique application A-linéaire, dite canonique,

$\alpha_M:\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))\rightarrow M$

satisfaisant à la relation

$$
\alpha_M(s\otimes f) =f(s) \tag{10}
$$

pour $\lambda \in \mathscr{S},s\in S_{\lambda}$, et $f\in$ Hom$_A(S_{\lambda},M)$. Si l’on munit $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))$ et M de leur structure de End$_A$(M)-module naturelle, l’application$\alpha_M$ est End$_A(M)$-linéaire.

#### Proposition 7 {#alg-viii-s4-prop-7 .statement tag=004Y}

Soit M un A-module. L’application canonique $\alpha_M$ est injective. Pour tout $\lambda \in \mathscr{S}$, l’image par $\alpha_M$ de $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$est le composant isotypique de M de type $\lambda$. L’image de $\alpha_M$ est le socle de M. Le A-module M est semi-simple si et seulement si l’application $\alpha_M$ est bijective.

Soit $\lambda \in \mathscr{S}$. Notons $M_{\lambda}$ le composant isotypique de M de type $\lambda$. Toute application A-linéaire de $S_{\lambda}$ dans M prend ses valeurs dans $M_{\lambda}$ (VIII, p. 62, prop. 5). Par suite, d’après la prop. 3, a) de VIII, p. 58, l’application $\alpha_M$ induit une bijection de $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ sur $M_{\lambda}$. La proposition en résulte, puisque le socle de M est somme directe de la famille $(M_{\lambda})_{\lambda\in\mathscr{S}}$, et que le module M est semi-simple si et seulement s’il est égal à son socle.

#### Définition 5 {#alg-viii-s4-def-5 .statement tag=004Z}

Soit M un A-module semi-simple. Une description de M (relative à la famille $(S_{\lambda})_{\lambda\in\mathscr{S}}$)est un couple $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$, où $V_{\lambda}$ est un espace vectoriel à gauche sur le corps $D_{\lambda}$ pour chaque $\lambda \in \mathscr{S}$ et où $\alpha :\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})\rightarrow M$est un isomorphisme de A-modules.

Tout A-module semi-simple M possède d’après la prop. 7 une description canonique : c’est le couple ((Hom$_A(S_{\lambda},M)$)$_{\lambda\in\mathscr{S}}, \alpha_M$) où $\alpha_M$ est l’application A-linéaire définie par la formule (10).

#### Proposition 8 {#alg-viii-s4-prop-8 .statement tag=0050}

Soient M un A-module semi-simple et $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$une description de M.

a) Pour tout $\lambda \in \mathscr{S},\alpha$ induit un isomorphisme du A-module $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ sur le composant isotypique de M de type $\lambda$.

b) Pour tout $\lambda \in \mathscr{S}$, l’application $\beta_{\lambda}: V_{\lambda}\rightarrow$ Hom$_A(S_{\lambda},M)$définie par $\beta_{\lambda}(v)(s) =\alpha (s\otimes v)$est $D_{\lambda}$-linéaire et bijective.

c) Soit N un sous-module de M. Il existe une unique famille $(W_{\lambda})_{\lambda\in\mathscr{S}}$ vérifiant $: W_{\lambda}$ est un sous-$D_{\lambda}$-espace vectoriel de $V_{\lambda}$ pour tout $\lambda \in \mathscr{S}$ et N est l’image par $\alpha$ du module $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$identifié à son image canonique dans le module $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$. Pour tout $\lambda \in \mathscr{S}, W_{\lambda}$ est l’ensemble des éléments $v\in V_{\lambda}$ tels que $\alpha (s\otimes v)$appartienne à N pour tout $s\in S_{\lambda}$.

Le A-module $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ est isotypique de type $\lambda$ pour tout $\lambda \in \mathscr{S}$. L’assertion a) résulte alors du fait que $\alpha$ est un isomorphisme et du fait que M est la somme directe de la famille $(M_{\lambda})_{\lambda\in\mathscr{S}}$ (VIII, p. 61, prop. 4 a)).

Soit $\lambda \in \mathscr{S}$. Notons $\alpha_{\lambda}: S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}\rightarrow M$ la restriction de $\alpha$ à $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$. Avec les notations du n$^o3$ appliquées au $(A,D_{\lambda}$)-bimodule $S_{\lambda}$,

$$
\beta_{\lambda}=\gamma (\alpha_{\lambda}) =\mathscr{H}(\alpha_{\lambda})\circ \beta_{V_{\lambda}}
$$

où la dernière égalité résulte de VIII, p. 56. Donc $\beta_{\lambda}$ est la composée de l’homomorphisme $D_{\lambda}$-linéaire $\mathscr{H}(\alpha_{\lambda})$ et de $\beta_{V_{\lambda}}$. L’assertion b) résulte alors de la prop. 3, b) de VIII, p. 58.

Soit N un sous-module de M. On a $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 62, cor.), donc c) résulte du th. 2 de VIII, p. 58.

#### Corollaire {#alg-viii-s4-n7-cor-1 .statement tag=0051}

Soit M un A-module semi-simple. Pour tout sous-module N de M et tout élément $\lambda$ de $\mathscr{S}$, identifions Hom$_A(S_{\lambda},N)$au sous-$D_{\lambda}$-espace vectoriel de Hom$_A(S_{\lambda},M)$formé des applications dont l’image est contenue dans N.

a) L’application $N\rightarrow$ (Hom$_A(S_{\lambda},N)$)$_{\lambda\in\mathscr{S}}$ est une bijection de l’ensemble des sous-A-modules de M sur l’ensemble des familles $(W_{\lambda})_{\lambda\in\mathscr{S}}$ telles que, pour tout $\lambda \in \mathscr{S}, W_{\lambda}$ soit un sous-$D_{\lambda}$-espace vectoriel de Hom$_A(S_{\lambda},M)$.

b) La bijection réciproque associe à une famille $(W_{\lambda})_{\lambda\in\mathscr{S}}$ le sous-A-module $\sum_{\lambda\in\mathscr{S}}\sum_{w\in W_{\lambda}}w(S_{\lambda})$de M.

C’est une traduction de la prop. 8 c) appliquée à la description canonique de M.

#### Proposition 9 {#alg-viii-s4-prop-9 .statement tag=0052}

Soient M et $M'$ des A-modules semi-simples et soient $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$et $((V'_{\lambda})_{\lambda\in\mathscr{S}}, \alpha ')$des descriptions de M et $M'$ respectivement. Pour toute famille $\boldsymbol{f}= (f_{\lambda})_{\lambda\in\mathscr{S}}$ de $\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V'_{\lambda})$, il existe une unique application A-linéaire $ \varphi(f) \in \operatorname{Hom}_A(M, M') $ rendant commutatif le diagramme

$$
\begin{array}{ccc}
\bigoplus_{\lambda \in \mathscr{I}} (S_\lambda \otimes_{D_\lambda} V_\lambda) & \xrightarrow{\alpha} & M \\
\downarrow & & \downarrow \varphi(f) \\
\bigoplus_{\lambda \in \mathscr{I}} (1_{S_\lambda} \otimes f_\lambda) & & \\
& & \\
\bigoplus_{\lambda \in \mathscr{I}} (S_\lambda \otimes_{D_\lambda} V'_\lambda) & \xrightarrow{\alpha'} & M'.
\end{array}
$$

L’application $ \varphi : \prod_{\lambda \in \mathscr{I}} \operatorname{Hom}_{D_\lambda}(V_\lambda, V'_\lambda) \to \operatorname{Hom}_A(M, M') $ ainsi définie est un isomorphisme de groupes. Lorsque l’on a $ M = M' $, $ V_\lambda = V'_\lambda $ pour tout $ \lambda \in \mathscr{I} $ et $ \alpha = \alpha' $, l’application $ \varphi $ est un isomorphisme d’anneaux de $ \prod_{\lambda \in \mathscr{I}} \operatorname{End}_{D_\lambda}(V_\lambda) $ sur $ \operatorname{End}_A(M) $.

Compte tenu de la description des composants isotypiques de $ M $ et $ M' $ donnée dans la prop. 8 a), cela résulte du th. 3 de VIII, p. 60 et de la prop. 5, b) de VIII, p. 62.

#### Corollaire {#alg-viii-s4-n7-cor-2 .statement tag=0053}

Soient $ M $ un $ A $-module semi-simple et $ M' $ un $ A $-module. L’application $ u \mapsto (\operatorname{Hom}(1_{S_\lambda}, u))_{\lambda \in \mathscr{I}} $ de $ \operatorname{Hom}_A(M, M') $ dans

$$
\prod_{\lambda \in \mathscr{I}} \operatorname{Hom}_{D_\lambda}(\operatorname{Hom}_A(S_\lambda, M), \operatorname{Hom}_A(S_\lambda, M'))
$$

est un isomorphisme de groupes. Lorsque $ M' $ est égal à $ M $, c’est un isomorphisme de l’anneau $ \operatorname{End}_A(M) $ sur l’anneau $ \prod_{\lambda \in \mathscr{I}} \operatorname{End}_{D_\lambda}(\operatorname{Hom}_A(S_\lambda, M)) $.

C’est une traduction de la proposition 9 appliquée aux descriptions canoniques de $ M $ et du socle de $ M' $.

### 8. Multiplicités et longueurs dans les modules semi-simples

#### Proposition 10 {#alg-viii-s4-prop-10 .statement tag=0054}

Soit $ M $ un $ A $-module semi-simple. Soit $ (M_i)_{i \in I} $ une famille de sous-modules simples dont $ M $ est somme directe. Les propriétés suivantes sont équivalentes :

(i) $ M $ est de longueur finie ;
(ii) $ M $ est artinien ;
(iii) $ M $ est noethérien ;
(iv) $ M $ est de type fini ;
(v) $ I $ est fini.

Si $ M $ satisfait à ces propriétés, la longueur de $ M $ est égale au cardinal de $ I $.

Si l’ensemble $ I $ est fini, $ M $ possède les propriétés (i) , (ii) , (iii) et (iv). Supposons l’ensemble $ I $ infini. D’après l’exemple 2 de VIII, p. 2, le module $ M $ n’est ni artinien, ni noethérien ; comme tout module de longueur finie est artinien et noethérien (VIII, p. 2, prop. 1), M n’est pas davantage de longueur finie. Enfin, tout élément de M appartient à la somme d’un nombre fini de sous-modules $M_i$, donc M n’est pas de type fini. Cela prouve l’équivalence des conditions (i) à (v). Si celles-ci sont satisfaites, on a long(M) $=\sum_{i\in I}$ long(M$_i$) $=$ Card(I) (II, p.23, cor. 5).

#### Proposition 11 {#alg-viii-s4-prop-11 .statement tag=0055}

Soit M un A-module semi-simple, somme directe d’une famille $(M_i)_{i\in I}$ de sous-modules simples. Pour tout $\lambda \in \mathscr{S}$, on note $I(\lambda )$l’ensemble des indices $i\in I$tels que $M_i$ soit de classe $\lambda$. Le cardinal de $I(\lambda )$est égal à la dimension du $D_{\lambda}$-espace vectoriel à gauche Hom$_A(S_{\lambda},M)$.

Le composant isotypique de type $\lambda$ de A est isomorphe à $S^{(I(\lambda))}_{\lambda}$ (VIII, p. 61, prop. 4 b)). Le $D_{\lambda}$-espace vectoriel Hom$_A(S_{\lambda},M)$ s’identifie à Hom$_A(S_{\lambda},M_{\lambda})$, donc est isomorphe à $D^{(I(\lambda))}_{\lambda}$ (VIII, p. 53). Cela prouve la proposition.

Tout module simple est primordial (VIII, p. 41), donc tout module semi-simple est semi-primordial. Soit M un A-module semi-simple et soit $\lambda \in \mathscr{S}$. On appelle multiplicité de $\lambda$ dans M la multiplicité primordiale $[M :\lambda ]$ de $\lambda$ dans M définie en VIII, p. 32. La prop. 11 se traduit par l’égalité

(11) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$).

Plus généralement, si $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ est une description de M, alors $[M :\lambda ]$ est égal à dim$_{D_{\lambda}}(V_{\lambda})$. D’après la prop. 6 de VIII, p. 64, on a aussi

(12) $[M :\lambda ] =$ dim$_{D_{\lambda}}$(Hom$_A(M,S_{\lambda})$)

lorsque la multiplicité $[M :\lambda ]$ est finie. Pour que des A-modules semi-simples M et $M'$ soient isomorphes, il faut et il suffit qu’on ait $[M :\lambda ] = [M':\lambda ]$ pour tout $\lambda \in \mathscr{S}$.

Soit M un A-module semi-simple. Il existe un cardinal $\mathbf{I}$possédant la propriété suivante : pour toute décomposition $M =\bigoplus_{i\in I}M_i$ de M en somme directe de modules simples, le cardinal de I est égal à $\mathbf{I}$(VIII, p. 32, cor. 2). Ce cardinal est appelé la longueur du A-module semi-simple M, et noté long$_A(M)$ ou long(M). Lorsque M est de longueur finie cette définition est compatible avec celle de II, p. 21, d’après la prop. 10.

Les A-modules simples sont les A-modules semi-simples de longueur 1, et l’on a la formule

(13) long$_A(\bigoplus_{j\in J}M_j)=\sum_{j\in J}$ long$_A(M_j)$ pour toute famille $(M_j)_{j\in J}$ de A-modules semi-simples. D’après la prop. 11, on a (14) long$_A(M) =\sum_{\lambda\in\mathscr{S}}$ dim$_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$.

En appliquant cette formule à $M_{\lambda}$, on obtient $[M :\lambda ] =$ long$_A(M_{\lambda})$ pour tout $\lambda \in \mathscr{S}$.

Lorsque A est un corps, les A-modules simples sont les espaces vectoriels de dimension 1 ; tout A-module est alors semi-simple (II, p. 95, th. 1) et sa longueur n’est autre que sa dimension en tant qu’espace vectoriel sur A (II, p. 97) .

## EXERCICES {#alg-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).

[^1]: D’après le cor. 2 de VIII, p. 52, cette définition coïncide avec celle donnée en VII, p. 9.
