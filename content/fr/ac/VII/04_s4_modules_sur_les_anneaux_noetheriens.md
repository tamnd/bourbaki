---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: Diviseurs
section: 4
section_title: Modules sur les anneaux noethériens intégralement clos
lang: fr
source: ac-v-vii-fr
pdf_pages: 0237-0274, 0299-0305
extraction: ocr
subsections:
    - "no": 1
      title: Réseaux
      page: 0
      pdf_page: 238
    - "no": 2
      title: Dualité; modules réflexifs
      page: 0
      pdf_page: 243
    - "no": 3
      title: Construction locale de modules réflexifs
      page: 0
      pdf_page: 248
    - "no": 4
      title: '*Pseudo-isomorphismes*'
      page: 0
      pdf_page: 250
    - "no": 5
      title: Diviseurs attachés aux modules de torsion
      page: 0
      pdf_page: 254
    - "no": 6
      title: Invariant relatif de deux réseaux
      page: 0
      pdf_page: 257
    - "no": 7
      title: Classes de diviseurs attachées aux modules de type fini
      page: 0
      pdf_page: 259
    - "no": 8
      title: Propriétés relatives aux extensions finies de l’anneau des scalaires
      page: 0
      pdf_page: 263
    - "no": 9
      title: Un théorème de réduction
      page: 0
      pdf_page: 269
    - "no": 10
      title: Modules sur les anneaux de Dedekind
      page: 0
      pdf_page: 272
statements: 81
exercises: 26
content_sha256: 38968e8a5882d97a8e9d5ea2e779cc29ed30e740da7a18f7a6473b7b37506c53
---

## § 4. Modules sur les anneaux noethériens intégralement clos

Dans tout ce paragraphe, A est un anneau commutatif intègre, de corps des fractions K. A partir du n° 2, on suppose en outre que A est noethérien et intégralement clos (donc un anneau de Krull (§ 1, n° 3, cor. du th. 2)); on note alors respectivement P(A), D(A) et C(A) l’ensemble des idéaux premiers de A de hauteur 1 ($§ 1, n° 6$), le groupe des diviseurs de A ($§ 1, n° 3$), et le groupe des classes de diviseurs de A ($§ 1, n° 10$), ces derniers étant notés additivement.

La méthode générale d’étude des modules de type fini sur un anneau noethérien intégralement clos A consiste à « localiser » les modules pour tous les idéaux premiers $p \in P(A)$ de hauteur 1 dans A; comme $A_p$ est alors un anneau de valuation discrète

### 1. Réseaux

#### Définition 1 {#ac-vii-s4-def-1 .statement}

Soit $V$ un espace vectoriel de dimension finie sur le corps $K$. On appelle réseau de $V$ par rapport à $A$ (ou simplement réseau de $V$) tout sous-$A$-module $M$ de $V$ vérifiant la condition suivante:

Il existe deux sous-$A$-modules libres $L_1, L_2$ de $V$ tels que $L_1 \subset M \subset L_2$ et que $\mathrm{rg}_A(L_1) = \mathrm{rg}_K(V)$.

#### Exemple 1 {#ac-vii-s4-n1-exa-1 .statement}

Si on prend $V = K$, les réseaux de $K$ ne sont autres que les idéaux fractionnaires $\neq (0)$ de $K$ ($§ 1$, n° 1, déf. 1).

#### Exemple 2 {#ac-vii-s4-n1-exa-2 .statement}

Si $\mathrm{rg}_K(V) = n$, tout sous-$A$-module libre $L$ de $V$ possède une base ayant au plus $n$ éléments, toute partie de $V$ libre sur $A$ étant libre sur $K$; pour que $L$ soit un réseau de $V$, il faut et il suffit que $L$ ait une base de $n$ éléments (autrement dit, que $\mathrm{rg}_A(L) = n$).

#### Exemple 3 {#ac-vii-s4-n1-exa-3 .statement}

Si $A$ est un anneau principal, tout réseau $M$ de $V$ est un $A$-module de type fini (puisque $A$ est noethérien) et sans torsion, donc est un $A$-module libre (*Alg.*, chap. VII, § 4, n° 3, cor. 2 du th. 2).

#### Proposition 1 {#ac-vii-s4-prop-1 .statement}

Pour qu’un sous-$A$-module $M$ de $V$ soit un réseau de $V$, il faut et il suffit que $KM = V$ et que $M$ soit contenu dans un sous-$A$-module de type fini de $V$.

Les conditions sont évidemment nécessaires, car un sous-$A$-module libre de $V$ ayant même rang que $V$ engendre $V$. Inversement, si $KM = V$, $M$ contient une base $(a_i)_{1 \leq i \leq n}$ de $V$ sur $K$, donc il contient le sous-$A$-module libre $L_1$ engendré par les $a_i$; d’autre part, si $M \subset M_1$, où $M_1$ est un sous-$A$-module de $V$ engendré par un nombre fini d’éléments $b_j$ et si $(e_i)_{1 \leq i \leq n}$ est une base de $V$ sur $K$, il existe un élément $s \neq 0$ de $A$ tel que chacun des $b_j$ soit combinaison linéaire des $s^{-1} e_i$ à coefficients *dans* $A$; si $L_2$ est le sous-$A$-module libre de $V$ engendré par les $s^{-1} e_i$, on a donc $M \subset L_2$.

#### Corollaire {#ac-vii-s4-n1-cor-1 .statement}

Supposons $A$ noethérien; pour qu’un sous-A-module $M$ de $V$ soit un réseau de $V$, il faut et il suffit que $KM = V$ et que $M$ soit de type fini.

#### Remarque 1 {#ac-vii-s4-n1-rem-1 .statement}

Rappelons que pour tout sous-A-module $M$ de $V$, l’application canonique $M \otimes_A K \to V$ est injective et a pour image $KM$ ($Alg.$, chap. II, 3e éd., § 7, n° 10, prop. 26); dire que $KM = V$ signifie donc que cette application est bijective.

#### Proposition 2 {#ac-vii-s4-prop-2 .statement}

Soient $M$ un réseau de $V$, $M_1$ un sous-A-module de $V$. S’il existe deux éléments $x, y$ de $K^*$ tels que $xM \subset M_1 \subset yM$, $M_1$ est un réseau de $V$; inversement, si $M_1$ est un réseau de $V$, il existe deux éléments $a, b$ non nuls de $A$ tels que $aM \subset M_1 \subset b^{-1}M$.

En effet, si $L_1, L_2$ sont deux réseaux libres de $V$ tels que $L_1 \subset M \subset L_2$, les relations $xM \subset M_1 \subset yM$ entraînent $xL_1 \subset M_1 \subset yL_2$ et $xL_1$ et $yL_2$ sont des réseaux libres; inversement, si $M_1$ est un réseau et $(e_i)_{1 \leq i \leq n}$ une base de $L_2$ sur $A$, la relation $KM_1 = V$ entraîne l’existence de $x = a/s \in K^*$ (où $a$ et $s$ sont des éléments non nuls de $A$) tel que $xe_i \in M_1$ pour tout $i$, d’où $xM \subset xL_2 \subset M_1$, et $a$ fortiori $aM \subset M_1$; échangeant les rôles de $M$ et $M_1$, on montre de même l’existence de $b \neq 0$ dans $A$ tel que $bM_1 \subset M$.

#### Proposition 3 {#ac-vii-s4-prop-3 .statement}

(i) Si $M_1,$ et $M_2$ sont des réseaux de $V$, il en est de même de $M_1 \cap M_2$ et de $M_1 + M_2$.

(ii) Si $W$ est un sous-espace vectoriel de $V$, et si $M$ est un réseau de $V$, $M \cap W$ est un réseau de $W$.

(iii) Soient $V, V_1, \ldots, V_k$ des espaces vectoriels de rang fini sur $K$, et soit $f : V_1 \times \cdots \times V_k \to V$ une application multilinéaire dont l’image engendre $V$. Si $M_i$ est un réseau de $V_i$ pour $1 \leq i \leq k$, le sous-A-module de $V$ engendré par $f(M_1 \times \cdots \times M_k)$ est un réseau de $V$.

(iv) Soient $V$ et $W$ deux espaces vectoriels de rang fini sur $K$, $M$ un réseau de $V$, $N$ un réseau de $W$. Le sous-A-module $N : M$ de $\operatorname{Hom}_K(V, W)$, formé des applications $K$-linéaires $f$ telles que $f(M) \subset N$, est un réseau de $\operatorname{Hom}_K(V, W)$.

(i) En vertu de la prop. 2, il existe $a$ et $b$ non nuls dans $A$ et tels que $aM_1 \subset M_2 \subset b^{-1}M_1$; on en conclut que $M_1 \cap M_2$ et $M_1 + M_2$ sont compris entre $aM_1$ et $b^{-1}M_1$, donc sont des réseaux en vertu de la prop. 2.

(ii) Soient S un supplémentaire de W dans V, L_w un réseau libre de W, L_s un réseau libre de S, de sorte que L = L_w ⊕ L_s est un réseau libre de V. Il existe donc x, y dans K* tels que xL ⊂ M ⊂ yL. On en déduit xL_w ⊂ M ∩ W ⊂ yL_w, ce qui montre que M ∩ W est un réseau de W (prop. 2).

(iii) Comme KM_i = V_i, il est clair par linéarité que f(M_1 × ... × M_k) engendre le K-espace vectoriel V; d’autre part, pour tout i, il existe un sous-A-module N_i de type fini de V_i tel que M_i ⊂ N_i; le sous-A-module N de V engendré par f(N_1 × ... × N_k) est de type fini et contient M, donc M est un réseau de V (prop. 1).

(iv) Soit P (resp. Q) un réseau libre de V (resp. W), contenant M (resp. contenu dans N); on a évidemment N : M ⊃ Q : P. Or il est immédiat que Q : P est isomorphe à Hom_A(P, Q), donc est un A-module libre de rang (rg_A P)(rg_A Q) (Alg., chap. II, 3e éd., § 1, n° 6, cor. 1 de la prop. 6), et par suite un réseau de Hom_K(V, W). De même, si P' (resp. Q') est un réseau libre de V (resp. W) contenu dans M (resp. contenant N), on a Q' : P' ⊃ N : M, et Q' : P' est un réseau de Hom_K(V, W); d’où la conclusion.

#### Remarque 2 {#ac-vii-s4-n1-rem-2 .statement}

La prop. 3, (i), montre que l’ensemble R(V) des réseaux de V est réticulé pour la relation d’inclusion; de plus, si M est un réseau fixe de V, les xM, où x parcourt K*, forment une partie de R(V) qui est à la fois coinitiale et cofinale (Ens., chap. III, 2e éd., § 1, n° 7).

#### Remarque 3 {#ac-vii-s4-n1-rem-3 .statement}

Avec les notations de la prop. 3, (iv), l’application canonique N : M → Hom_A(M, N) qui à toute application K-linéaire f ∈ N : M associe l’application A-linéaire de M dans N qui a même graphe que f|M, est bijective: en effet, toute application A-linéaire g : M → N se prolonge en une application K-linéaire g ⊗ 1 : M ⊗_A K → N ⊗_A K, et on a vu que M ⊗_A K et N ⊗_A K s’identifient respectivement à V et W.

En particulier, si l’on prend W = K, N = A, Hom_K(V, W) n’est autre que le K-espace vectoriel dual V* de V, et A : M s’identifie au A-module dual M* de M; nous ferons désormais cette identification et nous dirons que M* est le réseau dual de M: c’est donc l’ensemble des x* ∈ V* tels que ⟨x, x*⟩ ∈ A pour tout x ∈ M.

#### Corollaire {#ac-vii-s4-n1-cor-2 .statement}

Soient U, V, W trois espaces vectoriels de rang fini sur K, f : U × V → W une application K-bilinéaire non dégénérée à gauche (*Alg.*, chap. IX, § 1, n° 1, déf. 3). *Si $M$ est un réseau de $V$ et $N$ un réseau de $W$, l’ensemble $N :_f M$ des $x \in U$ tels que $f(x, y) \in N$ pour tout $y \in M$ est un réseau de $U$.*

Soit $s_f : U \to \operatorname{Hom}_K(V, W)$ l’application $K$-linéaire associée à gauche à $f$ (*Alg.*, chap. IX, *loc. cit.*), telle que $s_f(x)$ soit l’application linéaire $y \to f(x, y)$; rappelons que dire que $f$ est non dégénérée à gauche signifie que $s_f$ est *injective*. En vertu de la prop. 3, (iv), $N : M$ est un réseau de $\operatorname{Hom}_K(V, W)$; comme on a $N :_f M = s_f^{-1}(N : M)$ et que $s_f$ est injective, le corollaire résulte de la prop. 3, (ii).

#### Exemple 4 {#ac-vii-s4-n1-exa-4 .statement}

Soit $S$ une $K$-algèbre de rang fini (non nécessairement associative) ayant un élément unité; alors l’application bilinéaire $(x, y) \to xy$ de $S \times S$ dans $S$ est non dégénérée (à gauche et à droite). Si $M$ et $N$ sont des réseaux de $S$ par rapport à $A$, il en est de même de $M . N$ (prop. 3, (iii)) et de l’ensemble des $x \in S$ tels que $xM \subset N$ (cor. de la prop. 3). Notons qu’il existe une *sous-$A$-algèbre* de $S$ contenant l’élément unité de $S$ qui est un *réseau* de $S$; considérons en effet une base $(e_i)_{1 \leqslant i \leqslant n}$ de $S$ telle que $e_1$ soit l’élément unité de $S$, et soit $e_i e_j = \sum_k c_{ijk} e_k$ la table de multiplication de $S$ ($1 \leqslant i \leqslant n$, $1 \leqslant j \leqslant n$), de sorte que l’on a $c_{1jk} = \delta_{jk}$, $c_{i1k} = \delta_{ik}$ (symboles de Kronecker). Soit $s \in A$ non nul et tel que $c'_{ijk} = s . c_{ijk} \in A$ pour tout triplet d’indices $(i, j, k)$; si on pose $e'_i = se_i$ pour $i \geqslant 2$, on a $e'_i e'_j = sc'_{ij1} e_1 + \sum_{k \geqslant 2} c'_{ijk} e'_k$ pour $i \geqslant 2$ et $j \geqslant 2$; le réseau de $S$ ayant pour base $e_1$ et les $e'_i$ ($2 \leqslant i \leqslant n$) est une sous-$A$-algèbre de $S$ dont $e_1$ est l’élément unité.

#### Exemple 5 {#ac-vii-s4-n1-exa-5 .statement}

Soient $V$ un espace vectoriel de dimension finie sur $K$, $f$ une forme bilinéaire non dégénérée sur $V$. Si $M$ est un réseau de $V$, il résulte du cor. de la prop. 3 que l’ensemble $M_f^*$ des $x \in V$ tels que $f(x, y) \in A$ pour tout $y \in M$ est encore un réseau de $V$; si $s_f : V \to V^*$ est l’application linéaire associée à gauche à $f$ (qui est bijective), $s_f(M_f^*)$ n’est autre que le réseau dual $M^*$ de $M$.

#### Proposition 4 {#ac-vii-s4-prop-4 .statement}

*Soient $B$ un anneau commutatif intègre, $A$ un sous-anneau de $B$, $K$ et $L$ les corps des fractions respectifs de $A$ et de $B$. Soit $V$ un espace vectoriel de dimension finie sur $K$.*

(i) *Pour tout réseau $M$ de $V$ par rapport à $A$, l’image $BM$ de $M_{(B)} = M \otimes_A B$ dans $V_{(L)} = V \otimes_K L$ est un réseau de $V_{(L)}$ par rapport à $B$.*

(ii) Supposons de plus que B soit un A-module plat. Alors l’application canonique $M_{(B)} \to BM$ est bijective. Si en outre B est fidèlement plat, l’application qui, à tout réseau M de V par rapport à A, fait correspondre le réseau BM de $V_{(L)}$ par rapport à B, est injective.

(i) Comme $KM = V$, il est clair que $L.(BM) = V_{(L)}$; d’autre part M est contenu dans un sous-A-module de type fini $M_1$ de V, donc BM est contenu dans $BM_1$, qui est un B-module de type fini; d’où l’assertion (i) (prop. 1).

(ii) On a $V_{(L)} = V \otimes_K L = V \otimes_A L$ (chap. II, § 2, n° 7, prop. 18), et comme L est un B-module plat, c’est aussi un A-module plat (chap. I, § 2, n° 7, cor. 3 de la prop. 8). Comme B est un A-module plat, l’application canonique $M \otimes_A B \to V \otimes_A B$ est injective; d’autre part, V étant un K-module libre et K un A-module plat, V est un A-module plat (chap. I, § 2, n° 7, cor. 3 de la prop. 8), donc l’application canonique $V \otimes_A B \to V \otimes_A L$ est injective, ce qui établit la première assertion. Pour voir en outre que la relation $BM_1 = BM_2$ implique $M_1 = M_2$ pour deux réseaux $M_1, M_2$ de V par rapport à A lorsque B est un A-module fidèlement plat, notons d’abord que l’on a $BM_1 \cap BM_2 = B(M_1 \cap M_2)$ (chap. I, § 2, n° 6, prop. 6); on peut donc se borner au cas où $M_1 \subset M_2$, et notre assertion résulte alors du chap. I, § 3, n° 1, prop. 3, appliqué à l’injection canonique $M_1 \to M_2$.

#### Corollaire {#ac-vii-s4-n1-cor-3 .statement}

Supposons que A soit un anneau de valuation discrète. Soit $\hat{A}$ son complété, et soit $\hat{K}$ le corps des fractions de $\hat{A}$ (chap. VI, § 5, n° 3). L’application $\varphi$ qui, à tout réseau M de V, fait correspondre le réseau $\hat{A}M$ de $\hat{V} = V \otimes_K \hat{K}$ par rapport à $\hat{A}$, est bijective et son application réciproque fait correspondre à tout réseau $M'$ de $\hat{V}$ par rapport à $\hat{A}$ son intersection $M' \cap V$ (V étant canoniquement identifié à un sous-K-espace vectoriel de $\hat{V}$).

Si L est un réseau libre de V, les réseaux $aL$ (pour $a \in A$, $a \neq 0$) forment un système fondamental de voisinages de 0 pour une topologie $\mathcal{T}$ sur V (compatible avec sa structure de A-module), qui (lorsqu’on prend une base de L sur A) s’identifie à la topologie produit sur $K^n$; en vertu de la prop. 2, un système fondamental de voisinages de 0 pour $\mathcal{T}$ est encore formé de tous les réseaux de V par rapport à A ; il est clair que $\hat{V}$ est le complété de V pour $\mathcal{T}$. En outre, si m est l’idéal maximal de A, la topologie $\mathcal{T}$ induit sur tout réseau M de V par rapport à A la topologie m-adique puisque M est un A-module de type fini (chap. III, § 3, n° 2, th. 2), et $\hat{A}M$ est le complété de $M$ pour cette topologie (chap. III, § 2, n° 12, prop. 16); d’ailleurs, comme $M$ est ouvert (et par suite fermé) dans $V$, on a $\hat{A}M \cap V = M$, ce qui démontre à nouveau le fait que $\varphi$ est injective (qui découle directement de la prop. 4, (ii), puisque $\hat{A}$ est un $A$-module fidèlement plat). Enfin, si $M'$ est un réseau de $\hat{V}$ par rapport à $\hat{A}$, $M = M' \cap V$ est un réseau de $V$ par rapport à $A$, car tout élément de $\hat{A}$ est produit d’un élément de $A$ et d’un élément inversible de $\hat{A}$, donc il résulte de la prop. 2 qu’il existe $a, b$ dans $A - \{0\}$ tels que $a\hat{A}L \subset M' \subset b\hat{A}L$, d’où $aL \subset M' \cap V \subset bL$. En outre, $M'$ est ouvert dans $V$, et comme $V$ est dense dans $\hat{V}$, $M'$ est la complétion de $M' \cap V = M$; cela prouve que $\varphi$ est surjective, d’où le corollaire.

#### Exemple 6 {#ac-vii-s4-n1-exa-6 .statement}

Soient $S$ une partie multiplicative de $A$ ne contenant pas 0 ; appliquons la prop. 4 à $B = S^{-1}A$; on a alors $L = K, BM = S^{-1}M$; donc $S^{-1}M$ est un réseau de $V$ par rapport à $S^{-1}A$. En outre :

#### Proposition 5 {#ac-vii-s4-prop-5 .statement}

Soient $V, W$ deux espaces vectoriels de rang fini sur $K$, $M$ un réseau de $V$, $N$ un réseau de $W$. Si $M$ est de type fini, on a (avec les notations de la prop. 3):

(1) $$ S^{-1}(N : M) = S^{-1}N : S^{-1}M $$

dans $\mathrm{Hom}_K(V, W)$.

Il est clair que le premier membre de (1) est contenu dans le second. Réciproquement, soit $f \in S^{-1}N : S^{-1}M$, et soit $(x_i)_{1 \leq i \leq n}$ un système de générateurs de $M$. Il existe $s \in S$ tel que $f(x_i) \in s^{-1}N$ pour tout $i$, donc $sf \in N : M$, ce qui démontre la proposition.

### 2. Dualité; modules réflexifs

On rappelle qu’à partir de maintenant l’anneau $A$ est supposé noethérien et intégralement clos, et que l’on note $P(A)$ (ou simplement $P$) l’ensemble des idéaux premiers de hauteur 1 de $A$. Tout réseau par rapport à $A$ est un $A$-module de type fini (n° 1, cor. de la prop. 1).

Soient $V$ un espace vectoriel de rang fini sur $K$, $V^*$ son dual, $V^{**}$ son bidual; nous identifierons $V$ et $V^{**}$ au moyen de l’application canonique $c_V$ (Alg., chap. II, 3e éd., § 7, n° 5, th. 6). Soit $M$ un réseau de $V$; rappelons que le $A$-module dual $M^*$ de $M$ s’identifie canoniquement au réseau dual de $M$, ensemble des $x^* \in V^*$ tels que $\langle x, x^* \rangle \in A$ pour tout $x \in M$; le $A$-module bidual

M** de M est donc un réseau de V, qui contient M. En outre on a M*** = M*, car la relation M ⊂ M** entraîne (M**)* ⊂ M*, et on a d’autre part M* ⊂ (M*)** d’après ce qui précède (cf. Ens., chap. III, 2e éd., § 1, n° 5, prop. 2).

Si p est un idéal premier, la prop. 5 appliquée pour N = A donne la relation (M*)_p = (M_p)*, ce qui justifie la notation M_p* pour les deux membres.

#### Théorème 1 {#ac-vii-s4-thm-1 .statement}

Si M est un réseau de V, on a M* = $\bigcap_{p \in P} M_p^*$.

Il est clair que M* est contenu dans chacun des M_p*. Inversement, supposons que x* ∈ $\bigcap_{p \in P} M_p^*$; si x ∈ M, on a $\langle x, x^* \rangle \in \bigcap_{p \in P} A_p$, et comme A = $\bigcap_{p \in P} A_p$ (§ 1, n° 6, th. 4), on a bien x* ∈ M*.

#### Corollaire {#ac-vii-s4-n2-cor-1 .statement}

On a M** = $\bigcap_{p \in P} M_p$.

En effet, le th. 1 appliqué à M* montre que M** = $\bigcap_{p \in P} M_p^{**}$. Mais comme A_p est un anneau principal (§ 1, n° 6, th. 4), M_p est un A_p-module libre de type fini, donc M_p** s’identifie canoniquement à M_p (Alg., chap. II, 3e éd., § 2, n° 7, prop. 14), d’où le corollaire.

Pour un réseau quelconque M par rapport à A, l’application canonique c_M : M → M** (Alg., chap. II, 3e éd., § 2, n° 7) identifie un élément x ∈ M à lui-même, car x est l’unique élément y de V = V** tel que $\langle x, x^* \rangle = \langle y, x^* \rangle$ pour tout x* ∈ M*, puisque M* engendre V*. Nous dirons que M est réflexif si M** = M (loc. cit.). Comme on a vu plus haut que M* = (M*)**, on voit que le dual d’un réseau quelconque M est toujours réflexif.

#### Remarque 1 {#ac-vii-s4-n2-rem-1 .statement}

Soit M un A-module de type fini; il est immédiat que le dual M* de M, identifié à un sous-A-module de Hom_A(M, K), est un réseau du K-espace vectoriel Hom_A(M, K); en particulier, tout A-module réflexif de type fini est isomorphe à un réseau d’un K-espace vectoriel convenable.

#### Théorème 2 {#ac-vii-s4-thm-2 .statement}

Si M est un réseau de V, les conditions suivantes sont équivalentes:
a) M est réflexif.
b) $M = \bigcap_{p \in P} M_p$.
c) On a Ass(V/M) ⊂ P.

L’équivalence de a) et b) résulte du cor. du th. 1. Si b) est vérifiée, $V/M$ s’identifie canoniquement à un sous-A-module du produit $\prod_{p \in P} (V/M_p)$; mais en fait, il est contenu dans la *somme directe* $\bigoplus_{p \in P} (V/M_p)$: en effet, si $L \subset M$ est un réseau libre et $(e_i)_{1 \leq i \leq n}$ une base de $L$, chacune des coordonnées $x_i$ d’un point $x \in V$ par rapport à $(e_i)$ appartient à $A_p$ sauf pour un nombre fini de valeurs de $p$ (§ 1, n° 6, th. 4), donc $x \in L_p \subset M_p$ sauf pour un nombre fini de valeurs de $p \in P$. La relation $V/M \subset \bigoplus_{p \in P} (V/M_p)$ entraîne alors:

$$
\operatorname{Ass}(V/M) \subset \bigcup_{p \in P} \operatorname{Ass}(V/M_p).
$$

Comme $V/M_p$ est un $A_p$-module, un élément de $A - p$ ne peut annuler un élément $\neq 0$ de $V/M_p$, puisque les éléments de $A - p$ sont inversibles dans $A_p$; les éléments de $\operatorname{Ass}(V/M_p)$ sont donc contenus dans $p$ et sont $\neq 0$, puisque $V/M_p$ est un $A_p$-module de torsion; comme $p$ est de hauteur 1, on a nécessairement $\operatorname{Ass}(V/M_p) = \{p\}$ si $V/M_p \neq \{0\}$, et $\operatorname{Ass}(V/M_p) = \phi$ si $V/M_p = \{0\}$; donc $\operatorname{Ass}(V/M) \subset P$.

Enfin, si la condition c) est vérifiée, on a

$$
\operatorname{Ass}(M^{**}/M) \subset \operatorname{Ass}(V/M) \subset P.
$$

D’autre part, si $p \in P$, on a vu dans la démonstration du cor. du th. 1 que l’on a $M_p^{**} = M_p$, d’où $p \notin \operatorname{Ass}(M^{**}/M)$ (chap. IV, § 1, n° 3, cor. 1 de la prop. 7). On en conclut que l’on a $\operatorname{Ass}(M^{**}/M) = \phi$ d’où $M^{**} = M$ (chap. IV, § 1, n° 1, cor. 1 de la prop. 2).

#### Corollaire {#ac-vii-s4-n2-cor-2 .statement}

Soient $M, N$ deux réseaux de $V$ par rapport à $A$, *tels que* $N$ soit réflexif. *Pour que* $M \subset N$, *il faut et il suffit que*, *pour tout* $p \in P$, *on ait* $M_p \subset N_p$.

La condition est évidemment nécessaire, et si elle est remplie, on a $\bigcap_{p \in P} M_p \subset \bigcap_{p \in P} N_p = N$. Comme $M \subset M^{**} = \bigcap_{p \in P} M_p$, on a bien $M \subset N$.

#### Exemple 1 {#ac-vii-s4-n2-exa-1 .statement}

Tout réseau *libre* est réflexif.

#### Exemple 2 {#ac-vii-s4-n2-exa-2 .statement}

Prenons $V = K$. Pour qu’un idéal fractionnaire $a$ de $K$ soit un réseau réflexif, il faut et il suffit qu’il soit un *idéal divisoriel*, en vertu du critère b) du th. 2 et du § 1, n° 4, prop. 5 et 7.

#### Exemple 3 {#ac-vii-s4-n2-exa-3 .statement}

Soit $M$ un réseau par rapport à $A$; si $S$ est une partie multiplicative de $A$ ne contenant pas 0, la prop. 5 du n° 1 montre que $S^{-1}(M^*) = (S^{-1}M)^*$; si $M$ est réflexif, $S^{-1}M$ est donc un réseau réflexif par rapport à $S^{-1}A$.

#### Proposition 6 {#ac-vii-s4-prop-6 .statement}

(i) Si $M_1$ et $M_2$ sont des réseaux réflexifs de $V$, il en est de même de $M_1 \cap M_2$.

(ii) Si $W$ est un sous-espace vectoriel de $V$ et si $M$ est un réseau réflexif de $V$, $M \cap W$ est un réseau réflexif de $W$.

(iii) Soient $V, W$ deux espaces vectoriels de rang fini sur $K$, $M$ (resp. $N$) un réseau de $V$ (resp. $W$). Si $N$ est réflexif, le réseau $N : M$ de $\mathrm{Hom}_K(V, W)$ (n° 1, prop. 3) est réflexif.

(i) On a $(M_1 \cap M_2)_p = (M_1)_p \cap (M_2)_p$ pour tout $p \in P$ (chap. II, § 2, n° 4, th. 1). Si $M_1 = \bigcap_{p \in P} (M_1)_p$ et $M_2 = \bigcap_{p \in P} (M_2)_p$, on a donc $M_1 \cap M_2 = \bigcap_{p \in P} (M_1 \cap M_2)_p$, d’où la conclusion en vertu du th. 2.

(ii) De la même manière, on a $(M \cap W)_p = M_p \cap W_p = M_p \cap W$, d’où $M \cap W = \bigcap_{p \in P} (M \cap W)_p$, ce qui prouve (ii).

(iii) Comme $M$ est de type fini, il résulte du n° 1, prop. 5 que l’on a $(N : M)_p = N_p : M_p$; en outre, la relation $N = \bigcap_{p \in P} N_p$ entraîne:

$$
N : M = \bigcap_{p \in P} (N_p : M_p).
$$

En effet, si $f \in \bigcap_{p \in P} (N_p : M_p)$ et si $x \in M$, on a $f(x) \in \bigcap_{p \in P} N_p = N$, d’où $f \in N : M$; cela démontre que $N : M$ est réflexif.

#### Remarque 2 {#ac-vii-s4-n2-rem-2 .statement}

Si $M_1$ et $M_2$ sont des réseaux réflexifs de $V$, le réseau $M_1 + M_2$ n’est pas nécessairement réflexif (cf. § 1, exerc. 2).

#### Remarque 3 {#ac-vii-s4-n2-rem-3 .statement}

Si $M$ est un $A$-module de type fini, $T$ son sous-module de torsion, le dual $M^*$ de $M$ est le même que le dual de $M/T$, car pour toute forme linéaire $f$ sur $M$, l’image $f(T)$ est un sous-module de torsion de $A$, donc est nulle. Comme $M/T$ est isomorphe à un réseau d’un espace vectoriel sur $K$, on voit que le dual de tout $A$-module de type fini est réflexif.

#### Proposition 7 {#ac-vii-s4-prop-7 .statement}

Soit $0 \to M \to N \to Q \to 0$ une suite exacte de $A$-modules. On suppose que $N$ est de type fini et est sans torsion.

(i) Si $M$ est réflexif, on a $\mathrm{Ass}(Q) \subset P \cup \{\{0\}\}$ (autrement dit, tout idéal associé à $Q$ est, soit $(0)$, soit de hauteur 1).

(ii) Réciproquement, si $N$ est réflexif et si $\mathrm{Ass}(Q) \subset P \cup \{\{0\}\}$, alors $M$ est réflexif.

Comme $A$ est noethérien, $M$ est aussi de type fini ; si on pose $V = M_{(K)}, \ W = N_{(K)}, \ M$ (resp. $N$) s’identifie canoniquement à un réseau de V (resp. W) (n° 1, prop. 1). Considérons les deux suites exactes:

$$
0 \to V/M \to W/M \to W/V \to 0
$$
$$
0 \to Q \to W/M \to W/N \to 0.
$$

(i) On en déduit (chap. IV, § 1, n° 1, prop. 3):
$$
\operatorname{Ass}(Q) \subset \operatorname{Ass}(W/M) \subset \operatorname{Ass}(V/M) \cup \operatorname{Ass}(W/V).
$$
Si M est réflexif, on a $\operatorname{Ass}(V/M) \subset P$ (th. 2); d’autre part, il est clair que $\operatorname{Ass}(W/V)$ est, soit vide, soit réduit à $\{0\}$; d’où (i).

(ii) On a de même:
$$
\operatorname{Ass}(V/M) \subset \operatorname{Ass}(W/M) \subset \operatorname{Ass}(Q) \cup \operatorname{Ass}(W/N).
$$
Les hypothèses entraînent donc $\operatorname{Ass}(V/M) \subset P \cup \{\{0\}\}$. Mais $V/M$ est un A-module de torsion, donc $\{0\} \notin \operatorname{Ass}(V/M)$; le th. 2 montre alors que M est réflexif.

#### Proposition 8 {#ac-vii-s4-prop-8 .statement}

Soient R et S deux anneaux commutatifs, $\rho : R \to S$ un homomorphisme d’anneaux, M un R-module de type fini. On suppose que R est noethérien et que S est un R-module plat. Alors, si M est réflexif, il en est de même du S-module $M_{(S)} = M \otimes_R S$.

On sait (chap. I, § 2, n° 10, prop. 11) qu’il existe un isomorphisme canonique $\omega_M : (M^*)_{(S)} \to (M_{(S)})^*$, tel que
$$
\langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle = \rho(\langle x, x^* \rangle)
$$
pour $x \in M, x^* \in M^*$. Comme M est quotient d’un R-module libre L de type fini, $M^*$ est isomorphe à un sous-R-module du dual $L^*$, et $L^*$ est libre de type fini; puisque R est noethérien, $M^*$ est donc aussi un R-module de type fini, d’où un isomorphisme $\omega_{M^*} : (M^{**})_{(S)} \to ((M^*)_{(S)})^*$ tel que
$$
\langle x^* \otimes 1, \omega_{M^*}(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle)
$$
pour $x^* \in M^*$ et $x^{**} \in M^{**}$. D’autre part, on a un isomorphisme $' \omega_M : (M_{(S)})^{**} \to ((M^*)_{(S)})^*$, d’où par composition un isomorphisme canonique:
$$
\varphi = (' \omega_M^{-1}) \circ (\omega_{M^*}) : (M^{**})_{(S)} \to (M_{(S)})^{**}
$$
tel que l’on ait, avec les notations précédentes:
$$(1)\quad \langle \omega_M(x^* \otimes 1), \varphi(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle).$$
Considérons alors l’homomorphisme canonique $c_M : M \to M^{**},$ et montrons que l’homomorphisme composé :

(2) $\psi : M_{(S)} \xrightarrow{c_M \otimes 1} (M^{**})_{(S)} \to (M_{(S)})^{**}$

n’est autre que l’homomorphisme canonique $c_{M_{(S)}}$. Cela résulte aussitôt de (1) qui donne les relations :

$$
\langle \omega_M(x^* \otimes 1), \psi(x \otimes 1) \rangle = \rho(\langle x^*, c_M(x) \rangle) = \rho(\langle x, x^* \rangle)
= \langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle
$$

et du fait que les éléments $\omega_M(x^* \otimes 1)$ engendrent $(M_{(S)})^*$. Cela étant, l’hypothèse que $M$ est réflexif signifie que $c_M$ est bijectif, donc il en est de même de $c_M \otimes 1$, et par suite $\psi = c_{M_{(S)}}$ est bijectif, ce qui démontre la proposition.

### 3. Construction locale de modules réflexifs

Les notations et hypothèses sont celles du n° 2. On dira qu’une propriété a lieu « pour presque tout $p \in P$ » si l’ensemble des $p \in P$ pour lesquels elle n’est pas vraie est fini.

#### Théorème 3 {#ac-vii-s4-thm-3 .statement}

Soient $V$ un espace vectoriel de rang fini sur $K$, $M$ un réseau de $V$ par rapport à $A$.

(i) Soit $N$ un réseau de $V$ par rapport à $A$; alors, pour tout idéal premier $p$ de $A$, $N_p$ est un réseau de $V$ par rapport à $A_p$, et pour presque tout $p \in P$, on a $N_p = M_p$.

(ii) Réciproquement, supposons donné pour tout $p \in P$ un réseau $N(p)$ de $V$ par rapport à $A_p$ tel que $N(p) = M_p$ pour presque tout $p \in P$. Alors $N = \bigcap_{p \in P} N(p)$ est un réseau réflexif de $V$ par rapport à $A$, et c’est le seul réseau réflexif $N'$ de $V$ par rapport à $A$ tel que $N'_p = N(p)$ pour tout $p \in P$.

(i) La première assertion résulte du n° 1, prop. 4. En outre, il existe $x, y$ dans $K^*$ tels que $xN \subset M \subset yN$ (n° 1, prop. 2); on sait que pour presque tout $p \in P$, on a $v_p(x) = v_p(y) = 0$ (§ 1, n° 6, th. 4), ce qui montre que $x$ et $y$ sont inversibles dans $A_p$, donc $M_p = N_p$.

(ii) Quitte à remplacer $M$ par $x^{-1}M$ avec $x \neq 0$ dans $A$, on peut supposer que l’on a $N(p) \subset M_p$ pour tout $p \in P$. Soient $p_1, \ldots, p_h$ les éléments de $P$ tels que $N(p) = M_p$ pour $p$ distinct des $p_i$ ($1 \leq i \leq h$); posons :

$$
Q = M \cap N(p_1) \cap \ldots \cap N(p_h).
$$

Comme chacun des $N(p_i)$ contient un réseau libre par rapport à $A_{p_i}$, il contient *a fortiori* un réseau de $V$ par rapport à $A$, donc $Q$ contient un réseau de $V$ par rapport à $A$ (n° 1, prop. 3), et comme $Q$ est contenu dans $M$, $Q$ est un réseau par rapport à $A$. Pour prouver que $Q_p = N(p)$ pour tout $p \in P$, nous utiliserons le lemme suivant:

#### Lemme 1 {#ac-vii-s4-lem-1 .statement}

*Soient $p$ et $p'$ deux idéaux premiers de $A$ tels que (0) soit le seul idéal premier de $A$ contenu dans $p \cap p'$. Pour tout sous-A-module $E$ de $V$, on a alors $(E_p)_{p'} = \mathrm{K.E.}$*

Soit $S$ la partie multiplicative $(A - p)(A - p')$ de $A$; en vertu du chap. II, § 2, n° 3, prop. 7, on a $(E_p)_{p'} = S^{-1}E$. De plus, on a $A \subset S^{-1}A \subset K$; les idéaux premiers de $S^{-1}A$ correspondent aux idéaux premiers $q$ de $A$ tels que $q \cap S = \phi$ (chap. II, § 2, n° 5, prop. 11), et par hypothèse (0) est le seul idéal premier de $A$ ne rencontrant pas $S$; donc $S^{-1}A = K$ et $S^{-1}E = \mathrm{K.E.}$.

Revenons maintenant à la démonstration de (ii). Si $p \in P$ est distinct des $p_i$ ($1 \leq i \leq h$), le lemme 1 appliqué à $N(p_i)$ donne $(N(p_i))_p = ((N(p_i))_{p_i})_p = K \cdot N(p_i) = V$, puisque les $p_i$ et $p$ sont de hauteur 1. On a alors:

$$
Q_p = M_p \cap (N(p_1))_p \cap \ldots \cap (N(p_h))_p = M_p = N(p)
$$
(chap. II, § 2, n° 4). D’autre part, si $p$ est égal à $p_i$ ($1 \leq i \leq h$), on a $(N(p_i))_{p_j} = V$ pour $i \neq j$ par le même raisonnement que ci-dessus, et $(N(p_i))_{p_i} = N(p_i)$, d’où:

$$
Q_{p_i} = M_{p_i} \cap N(p_i) = N(p_i).
$$

On a donc prouvé que $Q_p = N(p)$ quel que soit $p \in P$. Alors $N = Q^{**} = \bigcap_{p \in P} Q_p$ est réflexif et vérifie les relations $N_p = Q_p = N(p)$ pour tout $p \in P$; la propriété d’unicité découle aussitôt du th. 2 du n° 2.

#### Remarque {#ac-vii-s4-n3-rem-1 .statement}

Soit $L$ un réseau libre de $V$ par rapport à $A$. Puisque $A_p$ est un anneau principal pour $p \in P$, $N(p)$ est un $A_p$-module libre de même rang que $L$, et il existe $u(p) \in \mathbf{GL}(V)$ tel que $u(p)(L_p) = N_p$; cette condition détermine d’ailleurs $u(p)$ à la multiplication à droite près par un élément de $\mathbf{GL}(L_p)$. La condition $N(p) = L_p$ pour presque tout $p \in P$ signifie que l’on doit avoir $u(p) \in \mathbf{GL}(L_p)$ pour presque tout $p \in P$. Les familles $(u(p))_{p \in P}$ vérifiant cette dernière propriété forment un groupe multiplicatif $\mathbf{GL}_a(V)$ contenant comme sous-groupe le produit $\prod_{p \in P} \mathbf{GL}(L_p)$.

Le th. 3 montre alors que *l’ensemble des réseaux réflexifs de $V$ est* canoniquement en correspondance biunivoque avec l’espace homogène $\mathrm{GL}_a(V)/\prod_{p \in P} \mathrm{GL}(L_p)$. Si on choisit une base $(e_i)_{1 \leq i \leq n}$ de $L$ sur $A$, $\mathrm{GL}(V)$ (resp. $\mathrm{GL}(L_p)$) s’identifie au groupe de matrices inversibles $\mathrm{GL}(n, K)$ (resp. $\mathrm{GL}(n, A_p)$) et le groupe $\mathrm{GL}_a(V)$ au groupe des systèmes de matrices d’ordre $n$, $(U(p))_{p \in P}$, tels que $U(p) \in \mathrm{GL}(n, K)$ pour tout $p \in P$ et $U(p) \in \mathrm{GL}(n, A_p)$ pour presque tout $p \in P$. Lorsque $A$ est un anneau de Dedekind, le groupe $\mathrm{GL}_a(V)$ s’identifie aussi au groupe $\mathrm{GL}(n, A)$, où $A$ est l’anneau des adèles restreints ($§ 2$, n° 4).

### 4. *Pseudo-isomorphismes*

Les notations et hypothèses sont celles des n°s 2 et 3.

#### Proposition 9 {#ac-vii-s4-prop-9 .statement}

Soit $M$ un $A$-module de type fini. Les conditions suivantes sont équivalentes:
a) $M_p = 0$ pour tout idéal premier $p$ de hauteur $\leq 1$.
b) L’annulateur $a$ de $M$ est un idéal $\neq (0)$, et on a $A : a = A$ ($A : a$ désignant, comme au $§ 1$, n° 1, l’ensemble des $x \in K$ tels que $xa \subset A$).

On sait (chap. II, $§ 2$, n° 2, cor. 2 de la prop. 4) que la condition $M_p = 0$ équivaut à $a \not\subset p$, donc à $aA_p = A_p$ (chap. II, $§ 2$, n° 5, Remarque); d’autre part, pour tout idéal entier $b \neq 0$ de $A$, la relation « $bA_p = A_p$ pour tout $p \in P$ » équivaut à div $b =$ div $A = 0$ dans $D(A)$ ($§ 1$, n° 4, prop. 7), ou encore à div($A : b$) = 0, et comme $A : b$ est divisoriel ($§ 1$, n° 1, prop. 1), cette relation est aussi équivalente à $A : b = A$. La proposition en résulte, en remarquant que dire que $a \not\subset p$ pour $p = (0)$ signifie que $a \neq (0)$.

#### Remarque 1 {#ac-vii-s4-n4-rem-1 .statement}

Les conditions équivalentes de la prop. 9 signifient aussi que Ass(M) ne contient aucun idéal premier de hauteur $\leq 1$. *On peut les interpréter en disant que Supp(M) est de codimension $\geq 2$ dans Spec(A).*

#### Définition 2 {#ac-vii-s4-def-2 .statement}

On dit qu’un $A$-module $M$ est pseudo-nul s’il est de type fini et s’il vérifie les conditions équivalentes de la prop. 9.

Cette définition, et la prop. 9, montrent qu’un $A$-module pseudo-nul est un $A$-module de torsion; la réciproque est inexacte.

#### Exemple 1 {#ac-vii-s4-n4-exa-1 .statement}

Si $A$ est un anneau de Dedekind, tout idéal premier de $A$ est de hauteur $\leq 1$; dire que $M$ est pseudo-nul signifie alors que $\operatorname{Supp}(M) = \phi$, donc que $M = 0$ (chap. II, § 4, n° 4).

#### Exemple 2 {#ac-vii-s4-n4-exa-2 .statement}

Soient $k$ un corps, $A = k[X, Y]$ l’anneau des polynômes sur $k$ à deux indéterminées ; si $m$ est l’idéal maximal $AX + AY$ de $A$, le $A$-module $A/m$ est pseudo-nul ; en effet, son annulateur $m$ n’est pas de hauteur $\leqslant 1$ puisqu’il contient les idéaux premiers principaux $AX$ et $AY$ et en est distinct ; on a donc $A : m = A$ ($§ 1$, n° 6, cor. 1 du th. 3).

#### Définition 3 {#ac-vii-s4-def-3 .statement}

Soient $M$ et $N$ deux $A$-modules, et $f : M \to N$ un homomorphisme. On dit que $f$ est pseudo-injectif (resp. pseudo-surjectif, pseudo-nul), si $\operatorname{Ker}(f)$ (resp. $\operatorname{Coker}(f)$, $\operatorname{Im}(f)$), est pseudo-nul ; on dit que $f$ est pseudo-bijectif s’il est à la fois pseudo-injectif et pseudo-surjectif.

On dit encore qu’un homomorphisme pseudo-bijectif est un pseudo-isomorphisme.

Supposons que $M$ et $N$ soient de type fini ; alors, pour que $f : M \to N$ soit pseudo-injectif (resp. pseudo-surjectif, pseudo-nul), il faut et il suffit que pour tout $p \in P \cup \{\{0\}\}$, $f_p : M_p \to N_p$ soit injectif (resp. surjectif, nul) ; cela résulte de la platitude du $A$-module $A_p$ (cf. chap. I, § 2, n° 3, Remarque 2).

#### Exemple 3 {#ac-vii-s4-n4-exa-3 .statement}

Soit $M$ un $A$-module sans torsion de type fini ; alors l’application canonique $c_M : M \to M^{**}$ de $M$ dans son bidual est un pseudo-isomorphisme. En effet, $M$ s’identifie à un réseau de $V = M \otimes_A K$ (n° 1, prop. 1) ; on a vu que $M_p = M_p^{**}$ pour tout $p \in P$ (n° 2, Exemple 2), et pour $p = 0$, $M_p$ et $M_p^{**}$ sont tous deux égaux à $V$.

#### Théorème 4 {#ac-vii-s4-thm-4 .statement}

Soient $E$ un $A$-module de type fini, $T$ le sous-module de torsion de $E$, et $M = E/T$. Il existe un pseudo-isomorphisme :

$$
f : E \to T \times M.
$$

Nous démontrerons d’abord deux lemmes.

#### Lemme 2 {#ac-vii-s4-lem-2 .statement}

Soit $(p_i)_{1 \leq i \leq k}$ une famille finie non vide d’idéaux premiers de $A$ de hauteur 1, et soit $S = \bigcap_i (A - p_i)$; alors l’anneau $S^{-1}A$ est principal.

En effet, $S^{-1}A$ est un anneau semi-local dont les idéaux maximaux sont les $m_i = p_i S^{-1}A$ pour $1 \leq i \leq k$, l’anneau local $(S^{-1}A)_{m_i}$ étant isomorphe à $A_{p_i}$ (chap. II, § 3, n° 5, prop. 17), donc un anneau de valuation discrète. L’anneau S^{-1}A est donc un anneau de Dedekind (§ 2, n° 2, th. 1, f)), et comme il est semi-local, il est principal (§ 2, n° 2, prop. 1).

#### Lemme 3 {#ac-vii-s4-lem-3 .statement}

Il existe un homomorphisme g : E → T dont la restriction à T est à la fois une homothétie et un pseudo-isomorphisme.

Soit a l’annulateur de T ; comme T est un A-module de torsion de type fini, on a a ≠ 0. Soient p_i (1 ≤ i ≤ k) les idéaux premiers de hauteur 1 contenant ·a (qui sont en nombre fini (§ 1, n° 6, th. 4)) ; si ce nombre est 0, T est pseudo-nul (prop. 9, a)), et on peut prendre g = 0. Sinon, soit S = \bigcap_i (A - p_i); en vertu du lemme 2, S^{-1}A est un anneau principal, donc S^{-1}M, qui est un S^{-1}A-module de type fini sans torsion, est libre (Alg., chap. VII, § 4, n° 3, cor. 2 du th. 2), et comme S^{-1}M = (S^{-1}E)/(S^{-1}T), S^{-1}T est facteur direct de S^{-1}E (Alg., chap. II, 3e éd., § 1, n° 11, prop. 21). Or, on a Hom_{S^{-1}A}(S^{-1}E, S^{-1}T) = S^{-1}\mathrm{Hom}_A(E, T) (chap. II, § 2, n° 7, prop. 19); donc il existe s_0 ∈ S et g_0 ∈ Hom_A(E, T) tel que s_0^{-1}g_0 soit un projecteur de S^{-1}E sur S^{-1}T. Si l’on note h_0 ∈ Hom_A(T, T) la restriction de g_0 à T, il existe par suite s_1 ∈ S tel que s_1h_0(x) = s_1s_0x pour tout x ∈ T; posant s = s_1s_0, g = s_1g, h = s_1h_0, h est donc l’homothétie de rapport s dans T et est la restriction de g à T. Reste à vérifier que h est un pseudo-isomorphisme. Or, si p = 0, ou si p ∈ P est distinct des p_i (1 ≤ i ≤ k), on a T_p = 0 (chap. II, § 4, n° 4, prop. 17), et h_p : T_p → T_p est un isomorphisme; si au contraire p est égal à l’un des p_i (1 ≤ i ≤ k), s est inversible dans A_{p_i}, et h_{p_i}, homothétie de rapport s dans T_{p_i}, est encore un isomorphisme, ce qui achève la démonstration du lemme 3.

Prouvons maintenant le th. 4. Soit g : E → T un homomorphisme vérifiant les propriétés du lemme 3; soit h la restriction de g à T, et soit π la projection canonique de E sur M. Montrons que l’homomorphisme f = (g, π) : E → T × M répond à la question. On a en effet le diagramme commutatif:

$$
\begin{array}{ccccccccc}
0 & \to & T & \longrightarrow & E & \longrightarrow & M & \to & 0 \\
& & \downarrow h & & \downarrow f & & \downarrow ^{1_M} & \\
0 & \to & T & \to & T \times M & \to & M & \to & 0
\end{array}
$$

où les lignes sont exactes. Le diagramme du serpent (chap. I,

$$
0 \to \mathrm{Ker}(h) \to \mathrm{Ker}(f) \to 0 \to \mathrm{Coker}(h) \to \mathrm{Coker}(f) \to 0
$$

donc $\mathrm{Ker}(f)$ est isomorphe à $\mathrm{Ker}(h)$ et $\mathrm{Coker}(f)$ à $\mathrm{Coker}(h)$. Comme $h$ est un pseudo-isomorphisme, il en est de même de $f$.

C.Q.F.D.

On peut dire qu’« à un pseudo-isomorphisme près », le th. 4 ramène l’étude des A-modules de type fini à celle des modules sans torsion, d’une part, et à celle des modules de torsion, d’autre part. En outre, on a vu ci-dessus (Exemple 3), qu’un module sans torsion est pseudo-isomorphe à son bidual, donc à un module réflexif. Quant aux modules de torsion, on a le résultat suivant, qui les détermine à un pseudo-isomorphisme près :

#### Théorème 5 {#ac-vii-s4-thm-5 .statement}

*Soit T un A-module de torsion de type fini. Il existe deux familles finies $(n_i)_{i \in I}$ et $(p_i)_{i \in I}$, où les $n_i$ sont des entiers $\geqslant 1$ et les $p_i$ des idéaux premiers de hauteur 1 de A, telles que si l’on pose $T' = \bigoplus_{i \in I} A/p_i^{n_i}$, il existe un pseudo-isomorphisme de T dans $T'$. De plus, les familles $(n_i)_{i \in I}$ et $(p_i)_{i \in I}$ ayant cette propriété sont uniques à une bijection près de l’ensemble d’indices, et les $p_i$ contiennent l’annulateur de T.*

*Unicité : Si $f : T \to T'$ est un pseudo-isomorphisme, et si $p \in P, f_p : T_p \to T'_p$ est un isomorphisme. Or, $T'_p$ est somme directe des $A_p/p^{n_i}A_p$, la somme étant étendue aux indices $i$ tels que $p_i = p$; les $p^{n_i}A_p$ sont donc les diviseurs élémentaires du $A_p$-module de torsion $T_p$ (*Alg.*, chap. VII, § 4, n° 7); leur unicité a été démontrée en *Alg.*, chap. VII, § 4, n° 7, prop. 7.*

*Existence : On peut se borner au cas où $T \neq 0$. Soient $a$ l’annulateur (non nul et distinct de A) de T, $p_i$ ($1 \leq i \leq k$) les idéaux premiers de hauteur 1 de A contenant $a$ (qui sont en nombre fini ($§ 1$, n° 6, th. 4)), et $S = \bigcap_i (A - p_i)$. L’anneau semi-local $A' = S^{-1}A$ est principal (lemme 2) et a pour idéaux maximaux les $m_i = p_iA'$; comme $S^{-1}T$ est un $A'$-module de torsion de type fini, il est isomorphe à une somme directe finie $\bigoplus_{j \in I} A'/m_{\varphi(j)}^{n_j}$, où $\varphi$ est une application d’un ensemble fini I dans $\{1, k\}$ (*Alg.*, chap. VII, § 4, n° 7, prop. 7); comme $A'/m_{\varphi(j)}^{n_j}$ est isomorphe à $S^{-1}(A/p_{\varphi(j)}^{n_j})$ (chap. II, § 2, n° 4), on a bien obtenu un A-module de torsion $T'$ du type cherché et un isomorphisme f_0 de S^{-1}T sur S^{-1}T'. Comme Hom_{S^{-1}A}(S^{-1}T, S^{-1}T') est égal à S^{-1}Hom_A(T, T') (chap. II, § 2, n° 7, prop. 19), il existe s \in S et un homomorphisme f : T \to T' tel que f_0 = s^{-1}f. Reste à montrer que f est un pseudo-isomorphisme : or, si p = 0 ou si p \in P est distinct des p_i, on a T_p = T'_p = 0 (chap. II, § 4, n° 4, prop. 17); si au contraire p est l’un des p_i (1 \leq i \leq k), s est inversible dans A_{p_i}, et comme f_{p_i} = s(f_0)_{p_i}, et que (f_0)_{p_i} est un isomorphisme de T_{p_i} = (S^{-1}T)_{m_i} sur T'_{p_i} = (S^{-1}T')_{m_i}, il en est de même de f_{p_i}.

C.Q.F.D.

#### Remarque 2 {#ac-vii-s4-n4-rem-2 .statement}

Dans l’énoncé du th. 5, on peut remplacer les modules A/p_i^{n_i} par A/p_i^{(n_i)} (§ 1, n° 4, prop. 8). En effet, pour tout p \in P, l’application canonique g : A/p^n \to A/p^{(n)} = A/(A \cap p^nA_p) est un pseudo-isomorphisme, car pour q \in P distinct de p, on a A_q/p^nA_q = A_q/p^{(n)}A_q = 0, et A_p/p^nA_p = A_p/p^{(n)}A_p.

\* Etant donnée une suite exacte de A-modules, E \to F \to G, si E et G sont pseudo-nuls, il en est de même de F, comme il résulte de la déf. 2 et du chap. II, § 2, n° 4, th. 1. Dans le langage des catégories, on peut donc dire que dans la catégorie C des A-modules, la sous-catégorie C' des modules pseudo-nuls est épaisse, et on peut alors définir la catégorie quotient C/C' : les objets de cette catégorie sont encore les A-modules, mais l’ensemble des morphismes de E dans F (pour E, F dans C/C') est la limite inductive de l’ensemble des groupes commutatifs Hom_A(E', F'), où E' (resp. F') parcourt l’ensemble des sous-modules de E (resp. l’ensemble des modules quotients F/F'' de F) tels que E/E' (resp. F'') soit pseudo-nul. On a bien entendu, pour tout couple de A-modules E, F, un homomorphisme canonique Hom_C(E, F) \to Hom_{C/C'}(E, F). Dire qu’un homomorphisme u \in Hom_A(E, F) est pseudo-nul (resp. pseudo-injectif, pseudo-surjectif, pseudo-bijectif) signifie que son image canonique dans Hom_{C/C'}(E, F) est nulle (resp. un monomorphisme, un épimorphisme, un isomorphisme).

### 5. Diviseurs attachés aux modules de torsion

Les notations et hypothèses sont celles des n°s 2, 3 et 4. Rappelons que D(A) (ou simplement D) désigne le groupe des diviseurs de A, noté additivement : on sait (§ 1, n° 3, th. 2) que D est le \mathbf{Z}-module libre engendré par les éléments de P.

Soit T un A-module de torsion de type fini. Pour tout $p \in P$, $T_p$ est un $A_p$-module de torsion de type fini, donc un module de longueur finie (chap. IV, § 2, n° 5, cor. 2 de la prop. 7); nous noterons $l_p(T)$ cette longueur. On a $T_p = 0$ pour tout $p$ ne contenant pas l’annulateur de T, donc pour presque tout $p$ ($§ 1$, n° 6, th. 4), ce qui justifie la définition suivante:

#### Définition 4 {#ac-vii-s4-def-4 .statement}

Si T est un A-module de torsion de type fini, on appelle contenu de T, et l’on note $\chi(T)$, le diviseur :

$$
\chi(T) = \sum_{p \in P} l_p(T) \cdot p.
$$

#### Proposition 10 {#ac-vii-s4-prop-10 .statement}

(i) Soit $0 \to T_1 \to T_2 \to T_3 \to 0$ une suite exacte de A-modules de torsion de type fini. On a alors :
$$
\chi(T_2) = \chi(T_1) + \chi(T_3).
$$
(ii) S’il existe un pseudo-isomorphisme $f : T_1 \to T_2$, on a $\chi(T_1) = \chi(T_2)$.
(iii) Pour que $\chi(T) = 0$, il faut et il suffit que T soit pseudo-nul.

Vu la déf. 4, il suffit de considérer pour chaque $p \in P$, les valeurs de $l_p$ pour les modules de torsion considérés. La propriété (i) résulte alors du chap. II, § 2, n° 4, th. 1 et de l’additivité des longueurs dans une suite exacte (Alg., chap. II, 3e éd., § 1, n° 10, prop. 16) et les propriétés (ii) et (iii) résultent aussitôt des définitions du n° 4.

#### Corollaire {#ac-vii-s4-n5-cor-1 .statement}

Soit $0 \to T_n \to T_{n-1} \to \cdots \to T_0 \to 0$ une suite exacte de A-modules de torsion de type fini. On a $\sum_{i=0}^n (-1)^i \chi(T_i) = 0$.

Vu le chap. II, § 2, n° 4, th. 1, cela résulte encore de la propriété analogue des $l_p$ (Alg., chap. II, 3e éd., § 1, n° 10, cor. 3 de la prop. 16).

Rappelons (chap. II, § 5, n° 4) que l’on peut parler de l’ensemble $F(A)$ des classes de A-modules de type fini pour la relation d’isomorphie; pour tout A-module M de type fini, on désigne par cl(M) l’élément correspondant de $F(A)$; nous désignerons par $T(A)$ la partie de $F(A)$ formée des classes de A-modules de torsion de type fini. Il est clair que $\chi$ définit une application de $T(A)$ dans D(A), notée encore $\chi$, telle que $\chi(\mathrm{cl}(T)) = \chi(T)$.

#### Proposition 11 {#ac-vii-s4-prop-11 .statement}

Soient G un groupe commutatif, noté additivement, et $\varphi : T(A) \to G$ une application; pour tout A-module *de torsion de type fini $T$, on pose encore, par abus de langage, $\varphi(T) = \varphi(\operatorname{cl}(T))$. On suppose vérifiées les conditions suivantes:*

1) *Si $0 \to T_1 \to T_2 \to T_3 \to 0$ est une suite exacte de $A$-modules de torsion de type fini, on a $\varphi(T_2) = \varphi(T_1) + \varphi(T_3)$.*

2) *Si $T$ est pseudo-nul, on a $\varphi(T) = 0$.*

*Il existe alors un homomorphisme $\theta : D(A) \to G$ et un seul tel que $\varphi = \theta \circ \chi$.*

Comme $\chi(A/\mathfrak{p}) = \mathfrak{p}$ pour tout $\mathfrak{p} \in P$, on doit avoir $\theta(\mathfrak{p}) = \varphi(A/\mathfrak{p})$ pour tout $\mathfrak{p} \in P$, ce qui prouve l’unicité de $\theta$, puisque les éléments de $P$ forment une base de $D(A)$. Inversement, soit $\theta$ l’homomorphisme de $D(A)$ dans $G$ tel que $\theta(\mathfrak{p}) = \varphi(A/\mathfrak{p})$ pour tout $\mathfrak{p} \in P$, et montrons qu’il répond à la question. Pour cela, posons $\psi(T) = \varphi(T) - \theta(\chi(T))$ pour tout $A$-module de torsion de type fini $T$; il est clair que les conditions 1) et 2) sont encore vérifiées lorsqu’on y remplace $\varphi$ par $\psi$. D’autre part, on a $\psi(A/\mathfrak{p}) = 0$ si $\mathfrak{p} \in P$; si $\mathfrak{p}$ est un idéal premier $\neq 0$ et non dans $P$, l’annulateur de $A/\mathfrak{p}$ n’est contenu dans aucun idéal de $P$, donc (n° 4, th. 5) $A/\mathfrak{p}$ est pseudo-nul, et par suite $\psi(A/\mathfrak{p}) = 0$. Cela étant, tout $A$-module de torsion de type fini $T$ admet une suite de composition dont les facteurs sont isomorphes à des $A$-modules de la forme $A/\mathfrak{p}$, avec $\mathfrak{p} \in \operatorname{Supp}(T)$ (chap. IV, § 1, n° 4, th. 1 et 2), donc $\mathfrak{p} \neq 0$ puisque $T$ est de torsion. Par récurrence sur la longueur de cette suite de composition, on en déduit (vu la propriété 1) pour $\psi$), que $\psi(T) = 0$.

C.Q.F.D.

\* On peut, comme au n° 4, considérer la catégorie quotient $\mathcal{T}/\mathcal{T}'$ de la catégorie $\mathcal{T}$ des $A$-modules de torsion de type fini par la sous-catégorie épaisse $\mathcal{T}'$ des $A$-modules de torsion de type fini pseudo-nuls. Dans le langage des catégories abéliennes, la prop. 11 exprime alors que le *groupe de Grothendieck* de la catégorie abélienne $\mathcal{T}/\mathcal{T}'$ est canoniquement isomorphe à $D(A)$. \*

#### Proposition 12 {#ac-vii-s4-prop-12 .statement}

*Si $\mathfrak{a}$ est un idéal $\neq 0$ de $A$,*

$$
\chi(A/\mathfrak{a}) = \chi((A : \mathfrak{a})/A) = \operatorname{div} \mathfrak{a}.
$$

Soit $\mathfrak{p} \in P$. On a $\mathfrak{a}A_\mathfrak{p} = \mathfrak{p}^{n_\mathfrak{p}} A_\mathfrak{p}$ avec $n_\mathfrak{p} \geqslant 0$, puisque $A_\mathfrak{p}$ est un anneau de valuation discrète. Comme $(A/\mathfrak{a})_\mathfrak{p} = A_\mathfrak{p}/\mathfrak{a}A_\mathfrak{p}$, on a $l_\mathfrak{p}(A/\mathfrak{a}) = n_\mathfrak{p}$, d’où $\chi(A/\mathfrak{a}) = \sum_{\mathfrak{p} \in P} n_\mathfrak{p} \mathfrak{p} = \operatorname{div} \mathfrak{a}$ (§ 1, n° 4, prop. 7).

D’autre part, $(A : \mathfrak{a})_\mathfrak{p} = A_\mathfrak{p} : \mathfrak{a}A_\mathfrak{p} = \mathfrak{p}^{-n_\mathfrak{p}} A_\mathfrak{p}$, donc $l_\mathfrak{p}((A : \mathfrak{a})/A) = n_\mathfrak{p}$, et on conclut de la même façon.

### 6. Invariant relatif de deux réseaux

Les notations et hypothèses sont celles des n°s 2 à 5. Soient V un espace vectoriel de rang fini $n$ sur K, M un réseau de V par rapport à A. Soit W la puissance extérieure $\bigwedge^n V$, qui est un espace vectoriel de rang 1 sur K, et désignons par $M_W$ le réseau de W engendré par l’image de $M^n$ par l’application canonique $V^n \to \bigwedge^n V$ (n° 1, prop. 3, (iii)) ; on notera que $M_W$ n’est pas nécessairement isomorphe à $\bigwedge^n M$ (*Alg.*, chap. III, § 5, exerc. 9)). Si $e$ est une base de W sur K, on peut donc écrire $M_W = a . e$, où $a$ est un idéal fractionnaire $\neq 0$ de A.

Soit $M'$ un second réseau de V, et posons $M'_W = a' . e$, où $a'$ est un idéal fractionnaire $\neq 0$ de A ; le diviseur $\operatorname{div}(a) - \operatorname{div}(a')$ ne dépend pas du choix de la base $e$ de W, $a$ et $a'$ étant multipliés par un même élément de $K^*$ quand on change de base ; nous poserons $\chi(M, M') = \operatorname{div}(a) - \operatorname{div}(a')$ et nous dirons que ce diviseur est l’invariant relatif de $M'$ par rapport à M. Il est clair que si M, $M'$, $M''$ sont trois réseaux de V, on a :

(3) $\chi(M, M') + \chi(M', M'') + \chi(M'', M) = 0$

(4) $\chi(M, M') + \chi(M', M) = 0$.

Pour tout $p \in P$, il résulte aussitôt des définitions que l’on a $(M_W)_p = (M_p)_W$; en outre, $M_p$ étant alors un $A_p$-module libre puisque $A_p$ est principal, une base de $M_p$ sur $A_p$ est une base de V sur K, donc $(M_p)_W = \bigwedge^n (M_p)$ (chap. II, § 2, n° 8), et l’idéal fractionnaire $a_p = a A_p$ est principal. Si on pose $a_p = p^{n_p} A_p$, $a'_p = p^{n'_p} A_p$, on a donc :

$$
\chi(M, M') = \sum_{p \in P} (n_p - n'_p) . p,
$$

ce que l’on peut aussi écrire :

(5) $\chi(M, M') = \sum_{p \in P} \chi(M_p, M'_p)$

en identifiant $D(A_p)$ au sous-$\mathbf{Z}$-module de $D(A)$ engendré par $p$.

#### Proposition 13 {#ac-vii-s4-prop-13 .statement}

Soient M un réseau de V, u un K-auto-morphisme de V. Alors on a :

(6) $-\chi(M, u(M)) = \operatorname{div}(\det(u))$.

En effet, pour tout $p \in P$, on a alors $\bigwedge^n (u(M)_p) = \bigwedge^n (u(M_p))$; si $(e_i)_{1 \leq i \leq n}$ est une base de $M_p$, on a
$$
\bigwedge^n (M_p) = A_p \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n,
$$
et $\bigwedge^n (u(M_p)) = A_p \cdot \det(u)e_1 \wedge e_2 \wedge \cdots \wedge e_n$, d’où la proposition en vertu de la formule (5).

#### Proposition 14 {#ac-vii-s4-prop-14 .statement}

*Si $M, M'$ sont deux réseaux de $V$ tels que $M' \subset M, M/M'$ est un $A$-module de torsion de type fini, et l’on a*:
(7)
$$
\chi(M, M') = - \chi(M/M').
$$
En effet, il est clair que $M/M' \subset V/M'$ est un module de torsion de type fini; d’autre part, pour tout $p \in P$, on sait (*Alg.*, chap. VII, § 4, n° 2, th. 1) qu’il existe des bases $(e_i)_{1 \leq i \leq n}$ de $M_p$ et $(e'_i)_{1 \leq i \leq n}$ de $M'_p$ telles que $e'_i = \pi^{v_i} e_i$ pour $1 \leq i \leq n$ et des entiers $v_i \geq 0$, $\pi$ étant une uniformisante de $A_p$. On a donc (avec les notations introduites ci-dessus) $n'_p - n_p = \sum_{i=1}^n v_i$; et d’autre part, $(M/M')_p = M_p/M'_p$ est isomorphe au $A_p$-module de torsion $\bigoplus_{i=1}^n A_p / p^{v_i} A_p$, donc sa longueur est $\sum_{i=1}^n v_i$, ce qui démontre la proposition, vu (5) et la déf. 4 du n° 5.

#### Corollaire {#ac-vii-s4-n6-cor-1 .statement}

*Soient $L_1, L_2$ deux $A$-modules libres de même rang fini $n$ et soit $f : L_1 \to L_2$ un homomorphisme. Soit $U$ la matrice de $f$ par rapport à des bases de $L_1$ et de $L_2$. Pour que $\mathrm{Coker}(f)$ soit un $A$-module de torsion, il faut et il suffit que $\det(U) \neq 0$, et l’on a alors*:
(8)
$$
\chi(\mathrm{Coker}(f)) = \mathrm{div}(\det(U)).
$$
On peut considérer $L_1$ et $L_2$ comme des réseaux dans $V_1 = L_1 \otimes_A K$ et $V_2 = L_2 \otimes_A K$ respectivement, $f$ s’étendant en un $K$-homomorphisme $f_{(K)} : V_1 \to V_2$. On a alors $(\mathrm{Coker}(f))_{(K)} = \mathrm{Coker}(f_{(K)})$ et dire que $\mathrm{Coker}(f)$ est un $A$-module de torsion signifie que $\mathrm{Coker}(f_{(K)}) = 0$; or, il revient au même de dire que $f_{(K)}$ est surjectif ou que $\det(U) \neq 0$, d’où la première assertion. D’autre part, on peut écrire $f(L_1) = u(L_2)$, où $u$ est un endomorphisme de $L_2$ de déterminant $\det(U)$; comme $\mathrm{Coker}(f) = L_2 / u(L_2)$, la formule (8) résulte de (7) et (6).

#### Exemple {#ac-vii-s4-n6-exa-1 .statement}

Si $A = \mathbf{Z}$, le groupe des diviseurs de $A$ s’identifie au groupe multiplicatif $\mathbf{Q}_+^*$ des nombres rationnels $> 0$. Pour tout groupe commutatif fini T, $\chi(T)$ est l’ordre de T ; le corollaire précédent montre que l’ordre du groupe Coker(f) est égal à la valeur absolue de det(U) (cf. Alg., chap. VII, 2e éd., § 4, n° 7, cor. 3 du th. 3).

### 7. Classes de diviseurs attachées aux modules de type fini

Les notations et hypothèses sont celles des n°s 2 à 6. Rappelons que l’on note C(A) (ou simplement C) le groupe des classes de diviseurs de A, quotient de D(A) par le sous-groupe des diviseurs principaux. Pour tout diviseur $d \in D$, nous noterons $c(d)$ sa classe dans C.

#### Proposition 15 {#ac-vii-s4-prop-15 .statement}

Soit M un A-module de type fini. Il existe un sous-module libre L de M tel que $M/L$ soit un module de torsion, et l’élément $c(\chi(M/L))$ de C ne dépend pas du sous-module libre L choisi.

Posons $S = A - \{0\}$, et soit $V = S^{-1}M = M \otimes_A K$; si $n$ est le rang de V sur K, il existe $n$ éléments $e_i$ ($1 \leq i \leq n$) de M dont les images canoniques dans V forment une base de V; ces éléments sont évidemment linéairement indépendants dans M, donc engendrent un sous-module libre L de M tel que $S^{-1}(M/L) = S^{-1}M/S^{-1}L = 0$, de sorte que $M/L$ est un module de torsion.

Soit maintenant $L_1$ un second sous-module libre de M, de rang $n$. Puisque $S^{-1}L = S^{-1}L_1$, il existe $s \in S$ tel que $sL_1 \subset L$; on peut donc se borner à prouver que si $L_1 \subset L_2$ sont deux sous-modules libres de rang $n$ de M, on a $c(\chi(M/L_1)) = c(\chi(M/L_2))$. Or, on a $\chi(M/L_1) = \chi(M/L_2) + \chi(L_2/L_1)$, et il résulte du n° 6, cor. de la prop. 14, que $\chi(L_2/L_1)$ est un diviseur principal, donc

$$
c(\chi(L_2/L_1)) = 0.
$$

C.Q.F.D.

L’élément $c(\chi(M/L))$ sera noté $-c(M)$ dans ce qui suit ; nous dirons que $c(M)$ est la classe de diviseurs attachée à M.

#### Proposition 16 {#ac-vii-s4-prop-16 .statement}

(i) Soit $0 \to M_1 \xrightarrow{f} M_2 \xrightarrow{g} M_3 \to 0$ une suite exacte de A-modules de type fini. On a:

$$
c(M_2) = c(M_1) + c(M_3).
$$

(ii) S’il existe un pseudo-isomorphisme de $M_1$ dans $M_2$, on a $c(M_1) = c(M_2)$.

(iii) Si T est un module de torsion, on a $c(T) = -c(\chi(T))$.

(iv) Si $a \neq 0$ est un idéal fractionnaire de $K$, on a
$$
c(a) = c(\operatorname{div}(a)).
$$

(v) Si L est un A-module libre, on a $c(L) = 0$.

Pour prouver (i), considérons un sous-module libre $L_1$ (resp. $L_3$) de $M_1$ (resp. $M_3$) tel que $M_1/L_1$ (resp. $M_3/L_3$) soit un module de torsion. Puisque $L_3$ est libre et g surjectif, il existe dans $g^{-1}(L_3)$ un supplémentaire libre $L_{23}$ de $\operatorname{Ker}(g)$, isomorphe à $L_3$ ($Alg.$, chap. II, 3e éd., § 1, n° 11, prop. 21); mais $\operatorname{Ker}(g) = f(M_1)$ contient $f(L_1) = L_{12}$ qui est libre puisque $f$ est injectif. La somme $L_2 = L_{12} + L_{23}$ est directe, et $L_2$ est donc un sous-module libre de $M_2$. On a en outre le diagramme commutatif:

$$
\begin{array}{ccccccccc}
0 & \to & L_1 & \to & L_2 & \to & L_3 & \to & 0 \\
   &     & \downarrow &     & \downarrow &     & \downarrow &     & \\
0 & \to & M_1 & \xrightarrow{f} & M_2 & \xrightarrow{g} & M_3 & \to & 0
\end{array}
$$

où les lignes sont exactes et les flèches verticales des injections. On tire donc du diagramme du serpent (chap. I, § 1, n° 4, prop. 2) la suite exacte:

$$
0 \to M_1/L_1 \to M_2/L_2 \to M_3/L_3 \to 0.
$$

Comme $M_1/L_1$ et $M_3/L_3$ sont des modules de torsion, cette suite exacte montre d’abord qu’il en est de même de $M_2/L_2$, puis, en vertu de la prop. 10 du n° 5, que l’on a:

$$
\chi(M_2/L_2) = \chi(M_1/L_1) + \chi(M_3/L_3)
$$

ce qui démontre (i).

Les assertions (iii) et (v) sont évidentes sur la définition. Démontrons (ii). Soit donc $f : M_1 \to M_2$ un pseudo-isomorphisme, et soit $L_1$ un sous-module libre de $M_1$ tel que $M_1/L_1$ soit un module de torsion. Posons $L_2 = f(L_1)$; comme $\operatorname{Ker}(f)$ est pseudo-nul, c’est un module de torsion, donc $\operatorname{Ker}(f) \cap L_1 = 0$, et par suite $L_2$ est libre. Soit $\bar{f} : M_1/L_1 \to M_2/L_2$ l’homomorphisme déduit de $f$ par passage aux quotients; $\operatorname{Ker}(\bar{f})$ est isomorphe à $\operatorname{Ker}(f)$, et $\operatorname{Coker}(\bar{f})$ à $\operatorname{Coker}(f)$, donc $\bar{f}$ est un pseudo-isomorphisme; d’ailleurs $\operatorname{Coker}(\bar{f}) = M_2/f(M_1)$ est un module de torsion et il en est de même de $f(M_1)/L_2 = \bar{f}(M_1/L_1)$, donc $M_2/L_2$ est un module de torsion, et il résulte du n° 5, prop. 10, (ii) que l’on a $\chi(M_1/L_1) = \chi(M_2/L_2)$.

Reste enfin à prouver (iv). Soit $x \in K^*$ tel que $a \subset xA$. En considérant la suite exacte $0 \to a \to xA \to xA/a \to 0$, on a c(a) = c(xA) - c(xA/a) = -c(xA/a) d’après (i) et (v). Mais xA/a est isomorphe à A/x^{-1}a, d’où en vertu de (iii),

$$
c(xA/a) = -c(\chi(A/x^{-1}a)) = -c(\operatorname{div}(x^{-1}a)) = -c(\operatorname{div}(a))
$$
(n° 5, prop. 12). Ceci achève la démonstration.

Lorsque M est un réseau de V par rapport à A, on a $\chi(M/L) = -\chi(M, L)$ (n° 6, prop. 14); soient $(e_i)_{1 \leq i \leq n}$ une base de L, $e = e_1 \wedge e_2 \wedge \ldots \wedge e_n$ et $M_w = a.e$ (notation du n° 6); on a $\chi(M, L) = \operatorname{div}(a)$, d’où $c(M) = c(\operatorname{div}(a))$, ce qui généralise la prop. 16 (v).

#### Corollaire 1 {#ac-vii-s4-prop-16-cor-1 .statement}

Soit $0 \to M_n \xrightarrow{u} M_{n-1} \to \cdots \to M_0 \to 0$ une suite exacte de A-modules de type fini. On a alors

$$
\sum_{i=0}^n (-1)^i c(M_i) = 0.
$$

Raisonnons par récurrence sur $n$, le cas $n = 2$ étant la prop. 16, (i). Si $M'_{n-1} = \operatorname{Coker}(u)$, on a les deux suites exactes:

$$
\begin{align*}
0 &\to M_n \to M_{n-1} \to M'_{n-1} \to 0 \\
0 &\to M'_{n-1} \to M_{n-2} \to \cdots \to M_0 \to 0.
\end{align*}
$$

La première montre que $M'_{n-1}$ est de type fini, et l’hypothèse de récurrence donne

$$
(-1)^{n-1} c(M'_{n-1}) + \sum_{i=0}^{n-2} (-1)^i c(M_i) = 0
$$

et $c(M'_{n-1}) = c(M_{n-1}) - c(M_n)$,

d’où le corollaire.

On appelle résolution libre finie d’un A-module E une suite exacte:

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to E \to 0
$$

où les $L_i$ ($0 \leq i \leq n$) sont des A-modules libres de type fini.

#### Corollaire 2 {#ac-vii-s4-prop-16-cor-2 .statement}

Si un idéal fractionnaire divisoriel $a \neq 0$ de A admet une résolution libre finie, il est principal.

Appliquons en effet le cor. 1 à une résolution libre finie de $a$:

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to a \to 0.
$$

En vertu de la prop. 16 (v), il vient $c(a) = 0$, donc, en vertu de la prop. 16 (iv), $\operatorname{div}(a)$ est principal; comme $a$ est supposé être divisoriel, il est principal (§ 1, n° 1).

#### Corollaire 3 {#ac-vii-s4-prop-16-cor-3 .statement}

Si tout idéal divisoriel $\neq 0$ de $A$ admet une résolution libre finie, $A$ est factoriel.

C’est une conséquence immédiate du cor. 2 et du § 3, n° 1, déf. 1.

\* Nous verrons plus tard qu’un anneau local régulier vérifie l’hypothèse du cor. 3, donc est factoriel.*

Si $M$ est un $A$-module de type fini, nous noterons $r(M)$ son rang (rappelons que c’est le rang sur $K$ de $M_{(K)} = M \otimes_A K$); si $0 \to M_1 \to M_2 \to M_3 \to 0$ est une suite exacte de $A$-modules de type fini, la suite $0 \to (M_1)_{(K)} \to (M_2)_{(K)} \to (M_3)_{(K)} \to 0$ est encore exacte, donc $r(M_2) = r(M_1) + r(M_3)$. Nous poserons

$$
\gamma(M) = (r(M), c(M)) \in \mathbf{Z} \times C(A);
$$

$\gamma$ vérifie donc la propriété (i) de la prop. 16 et, si $M$ est pseudo-nul, $\gamma(M) = 0$ (puisque $M$ est de torsion). Il existe une application unique de $F(A)$ dans $\mathbf{Z} \times C(A)$ notée encore $\gamma$, telle que $\gamma(M) = \gamma(\mathrm{cl}(M))$ pour tout $A$-module $M$ de type fini. Nous allons voir que les propriétés précédentes caractérisent essentiellement $\gamma$:

#### Proposition 17 {#ac-vii-s4-prop-17 .statement}

Soient $G$ un groupe commutatif, noté additivement, et $\varphi$ une application de l’ensemble $F(A)$ des classes de $A$-modules de type fini dans $G$; pour tout $A$-module de type fini $M$, on pose encore, par abus de langage, $\varphi(M) = \varphi(\mathrm{cl}(M))$. On suppose vérifiées les conditions suivantes:

1) Si $0 \to M_1 \to M_2 \to M_3 \to 0$ est une suite exacte de $A$-modules de type fini, on a $\varphi(M_2) = \varphi(M_1) + \varphi(M_3)$.

2) Si $T$ est pseudo-nul, on a $\varphi(T) = 0$.

Il existe alors un homomorphisme $\theta : \mathbf{Z} \times C \to G$ et un seul tel que $\varphi = \theta \circ \gamma$.

En vertu de la prop. 16, (iv), tout élément de $N^* \times C$ est de la forme $(r(M), c(M))$ pour un $A$-module de type fini $M$ convenable; d’où l’unicité de $\theta$. Appliquons la prop. 11 du n° 5 à la restriction de $-\varphi$ à $T(A)$: il existe donc un homomorphisme $\theta_0 : D \to G$ tel que $-\varphi(T) = \theta_0(\chi(T))$ pour tout $A$-module de torsion $T$ de type fini. Soit $x$ un élément non nul de $A$; appliquant la propriété 1) à la suite exacte:

$$
0 \to A \xrightarrow{h_x} A \to A/xA \to 0
$$

où $h_x$ est la multiplication par $x$, il vient $\varphi(A/xA) = 0$, d’où θ₀(div(x)) = 0. Par passage au quotient, θ₀ définit donc un homomorphisme θ₁ : C → G et l’on a φ(T) = θ₁(c(T)) pour tout A-module de torsion T. Montrons alors que l’homomorphisme θ défini par θ(n, z) = n.φ(A) + θ₁(z) répond à la question. Pour cela, posons φ'(M) = φ(M) − θ(γ(M)) pour tout A-module M de type fini; il est clair que la condition 1) est encore vérifiée lorsqu’on y remplace φ par φ'. En outre, on a φ'(M) = 0 lorsque M est un module de torsion ou un module libre; mais comme pour tout A-module M de type fini, il existe un sous-module libre L de M tel que M/L soit un module de torsion (prop. 15), la propriété 1) montre que φ'(M) = 0 pour tout A-module M de type fini.

\* Dans le langage des catégories abéliennes, la prop. 17 montre que $\mathbf{Z} \times C(A)$ est canoniquement isomorphe au groupe de Grothendieck de la catégorie quotient $\mathcal{F}/\mathcal{F}'$, où $\mathcal{F}$ est la catégorie des A-modules de type fini, $\mathcal{F}'$ la sous-catégorie épaisse de $\mathcal{F}$ formée des modules pseudo-nuls. \*

### 8. Propriétés relatives aux extensions finies de l’anneau des scalaires

Dans ce n°, A et B désignent deux anneaux noethériens intégralement clos tels que $A \subset B$ et que B soit un A-module de type fini, K et L les corps des fractions de A et B respectivement. On écrira div_A, $\chi_A$, c_A, $\gamma_A$, r_A au lieu de div, $\chi$, c, $\gamma$, r respectivement lorsqu’il s’agira de A-modules, et on utilisera des notations analogues pour les B-modules.

On sait (§ 1, n° 10) que pour qu’un idéal premier $\mathfrak{P}$ de B soit de hauteur 1, il faut et il suffit que $p = \mathfrak{P} \cap A$ soit de hauteur 1; en outre (loc. cit., prop 14) pour $p \in P(A)$, il n’y a qu’un nombre fini d’idéaux premiers $\mathfrak{P} \in P(B)$ au-dessus de p. Pour abréger, nous noterons $\mathfrak{P}|p$ la relation « $\mathfrak{P}$ est au-dessus de $p$ » (c’est-à-dire $p = \mathfrak{P} \cap A$); nous noterons alors $e_{\mathfrak{P}/p}$ ou $e(\mathfrak{P}/p)$ l’indice de ramification $e(v_{\mathfrak{P}}/v_p)$ de la valuation $v_{\mathfrak{P}}$ par rapport à la valuation $v_p$ (chap. VI, § 8, n° 1) et $f_{\mathfrak{P}/p}$ ou $f(\mathfrak{P}/p)$ le degré résiduel $f(v_{\mathfrak{P}}/v_p)$ (loc. cit.); rappelons que les valuations discrètes $v_p$ et $v_{\mathfrak{P}}$ sont normées, et que $f_{\mathfrak{P}/p}$ est le degré du corps des fractions de $B/\mathfrak{P}$ sur le corps des fractions de $A/p$. Posons $n = r_A(B)$, où B est considéré comme A-module; on a donc par définition $n = [L : K]$, et, pour tout $p \in P(A)$, n est aussi le rang du $A_p$-module libre $B_{\mathfrak{P}}$ pour tout $\mathfrak{P}|p$. Il résulte donc du chap. VI,

(9)
$$
\sum_{\mathfrak{P}|p} e_{\mathfrak{P}/p} f_{\mathfrak{P}/p} = n.
$$

Cela étant, comme $D(A)$ et $D(B)$ sont des $\mathbf{Z}$-modules libres, on définit un homomorphisme croissant de groupes ordonnés $N : D(B) \to D(A)$ (aussi noté $N_{B/A}$), par la condition:

(10)
$$
N(\mathfrak{P}) = f_{\mathfrak{P}/p} \cdot p \quad \text{pour } \mathfrak{P} \in P(B), \text{ avec } p = \mathfrak{P} \cap A.
$$

On a d’autre part ($§ 1,$ n° 10, prop. 14) défini un homomorphisme croissant de groupes ordonnés $i : D(A) \to D(B)$ (aussi noté $i_{B/A}$), par la condition:

(11)
$$
i(p) = \sum_{\mathfrak{P}|p} e_{\mathfrak{P}/p} \cdot \mathfrak{P} \quad \text{pour } p \in P(A).
$$

Il est clair que pour toute famille $(d_i)$ (resp. $(d'_i)$) de diviseurs de $A$ (resp. $B$), on a:

(12)
$$
N(\sup(d'_i)) = \sup(N(d'_i)), \qquad N(\inf(d'_i)) = \inf(N(d'_i))
$$
(13)
$$
i(\sup(d_i)) = \sup(i(d_i)), \qquad i(\inf(d_i)) = \inf(i(d_i)).
$$

La formule (9) montre que l’on a:

(14)
$$
N \circ i = n \cdot 1_{D(A)}.
$$

Pour tout $a \in A$, on a ($§ 1,$ n° 10, prop. 14):

(15)
$$
i(\operatorname{div}_A(a)) = \operatorname{div}_B(a).
$$

On en déduit (grâce à (13)) que, pour tout idéal fractionnaire $a$ de $A$, on a aussi:

(16)
$$
i(\operatorname{div}_A(a)) = \operatorname{div}_B(aB).
$$

Pour tout élément $b \in B$, on sait (chap. V, $§ 1,$ n° 3, cor. de la prop. 11) que $N_{L/K}(b) \in A$; en outre (chap. VI, $§ 8,$ n° 5, formule (9)) on a:

(17)
$$
v_p(N_{L/K}(b)) = \sum_{\mathfrak{P}|p} f_{\mathfrak{P}/p} v_{\mathfrak{P}}(b)
$$
d’où:
(18)
$$
N(\operatorname{div}_B(b)) = \operatorname{div}_A(N_{L/K}(b)).
$$

Les formules (15) et (18) montrent que, par passage aux quotients, les homomorphismes $N$ et $i$ définissent des homomorphismes que l’on notera encore, par abus de langage:

$$
N : C(B) \to C(A), \qquad i : C(A) \to C(B).
$$

On notera que l’homomorphisme $i : C(A) \to C(B)$ n’est pas injectif en général ($§ 3$, exerc. 7).

Rappelons que pour tout B-module R, on note $R_{[A]}$ le A-module obtenu à partir de R par restriction des scalaires à A (*Alg.*, chap. II, 3\textsuperscript{e} éd., $§ 1$, no 13).

#### Proposition 18 {#ac-vii-s4-prop-18 .statement}

(i) *Pour que R soit un B-module pseudo-nul, il faut et il suffit que le A-module $R_{[A]}$ soit pseudo-nul.*

(ii) *Pour que R soit un B-module de torsion de type fini, il faut et il suffit que $R_{[A]}$ soit un A-module de torsion de type fini, et l’on a alors*:

$$
\chi_A(R_{[A]}) = N(\chi_B(R)).
$$

(iii) *Pour que R soit un B-module de type fini, il faut et il suffit que $R_{[A]}$ soit un A-module de type fini, et l’on a alors*:

$$
c_A(R_{[A]}) = N(c_B(R)) + r_B(R)c_A(B)
$$
$$
r_A(R_{[A]}) = n \cdot r_B(R) \quad \text{(on rappelle que } n = r_A(B)).
$$

Comme B est un A-module de type fini, pour que R soit un B-module de type fini, il faut et il suffit que $R_{[A]}$ soit un A-module de type fini. En outre, si b est l’annulateur de R, $b \cap A = a$ est l’annulateur de $R_{[A]}$; comme B est entier sur A, il n’y a pas d’autre idéal que 0 au-dessus de l’idéal 0 de A (chap. V, $§ 2$, no 1, cor. 1 de la prop. 1), donc il revient au même de dire que $a \neq 0$ ou que $b \neq 0$.

(i) En vertu de cette dernière remarque, on peut se borner au cas où R est un B-module de torsion. Si b est contenu dans un idéal premier $\mathfrak{P} \in P(B)$, a est contenu dans $\mathfrak{P} \cap A = p$, qui est de hauteur 1. Inversement, si a est contenu dans un idéal premier $p \in P(A)$, il existe un idéal premier $\mathfrak{P}$ de B qui contient b et est au-dessus de p (chap. V, $§ 2$, no 1, cor. 2 du th. 1). L’assertion (i) résulte de ces remarques et du no 4, déf. 2.

(ii) Pour tout B-module de torsion de type fini R, posons $\varphi(R) = \chi_A(R_{[A]})$; il est clair que (pour les B-modules de torsion de type fini) $\varphi$ vérifie les conditions 1) et 2) de la prop. 11 du no 5 (compte tenu de (i)). Il existe par suite un homomorphisme $\theta : D(B) \to D(A)$ tel que $\varphi(R) = \theta(\chi_B(R))$ pour tout B-module de torsion R de type fini. L’homomorphisme $\theta$ est déterminé par sa valeur pour tout B-module de la forme $B/\mathfrak{P}$ où $\mathfrak{P} \in P(B)$, puisque $\chi_B(B/\mathfrak{P}) = \mathfrak{P}$. Or, pour tout idéal premier $q \neq p = \mathfrak{P} \cap A$ dans $P(A)$, on a $p \not\subset q$, donc $(B/\mathfrak{P})_q = 0$. D’autre part, si on pose

S = A - p, $\mathfrak{P}. S^{-1}B$ est un idéal maximal de $S^{-1}B$ et $(B/\mathfrak{P})_p = S^{-1}B/\mathfrak{P}. S^{-1}B$ est isomorphe au corps des fractions de $B/\mathfrak{P}$ (chap. II, § 2, n° 5, prop. 11), c’est-à-dire au corps résiduel de $v_{\mathfrak{P}}$; sa longueur en tant que $A_p$-module est donc $f_{\mathfrak{P}/p}$; ce qui prouve que $\theta = N$ (n° 5, déf. 4).

(iii) Si T est le sous-module de torsion de R, $T_{[A]}$ est le sous-module de torsion de $R_{[A]}$, et $(R/T)_{[A]} = R_{[A]}/T_{[A]}$; pour prouver (21), on peut donc se borner au cas où R est sans torsion. Alors R est identifié à un sous-B-module de $R_{(L)}$, et contient une base $(e_i)_{1 \leq i \leq m}$ de $R_{(L)}$ sur L. Si $(b_j)_{1 \leq j \leq n}$ est une base de L sur K formée d’éléments de B, les $b_j e_i$ constituent une base de $R_{(L)}$ sur K, formée d’éléments de R, d’où (21). Soit d’autre part M un sous-B-module libre de R tel que $R/M$ soit un B-module de torsion; comme $M_{[A]}$ est somme directe de $r_B(R)$ A-modules isomorphes à B, on a (prop. 16, (i)) $c_A(M_{[A]}) = r_B(R).c_A(B)$. En outre, $c_A((R/M)_{[A]}) = -c_A(N(\chi_B(R/M)))$ en vertu de (19); mais par définition de l’homomorphisme $N : C(B) \to C(A)$, on a $c_A(N(d)) = N(c_B(d))$ pour tout $d \in D(B)$, et comme $c_B(\chi(R/M)) = -c_B(R)$ par définition, on a finalement $c_A((R/M)_{[A]}) = N(c_B(R))$; il suffit alors d’appliquer la prop. 16, (i) pour obtenir (20).

#### Proposition 19 {#ac-vii-s4-prop-19 .statement}

Soit R un B-module de type fini. Pour que R soit réflexif, il faut et il suffit que $R_{[A]}$ soit un A-module réflexif.

On a remarqué dans la démonstration de la prop. 18 que pour que R soit un B-module sans torsion, il faut et il suffit que $R_{[A]}$ soit un A-module sans torsion. On peut donc supposer que R est un réseau de $W = R \otimes_B L$ par rapport à B. Nous utiliserons le lemme suivant:

#### Lemme 4 {#ac-vii-s4-lem-4 .statement}

Soit W un espace vectoriel de rang fini sur L et soit R un réseau de W par rapport à B. Pour tout $p \in P(A)$, on a alors $(R_{[A]})_p = \bigcap_{\mathfrak{P}|p} R_{\mathfrak{P}}$.

En effet, si $S = A - p$, les idéaux premiers de l’anneau $S^{-1}B$ sont engendrés par les idéaux premiers de B ne rencontrant pas S, autrement dit les idéaux $\mathfrak{P}_i$ ($1 \leq i \leq m$) au-dessus de p et l’idéal (0); cela montre que $S^{-1}B$ est un anneau semi-local dont les idéaux maximaux sont les $m_i = \mathfrak{P}_i(S^{-1}B)$ pour $1 \leq i \leq m$; en outre l’anneau local $(S^{-1}B)_{m_i}$ est isomorphe à $B_{\mathfrak{P}_i}$ (chap. II, § 2, n° 5, prop. 11), donc est un anneau de valuation discrète. L’anneau $S^{-1}B$ est par suite un anneau de Dedekind (§ 2, n° 2, th. 1, f)), et comme il est semi-local, il est principal (§ 2, n° 2, prop. 1). Cela étant, $(R_{[A]})_p$ est égal à $S^{-1}R$, considéré comme $A_p$-module;

d’après ce qui précède, S^{-1}R est un réseau libre de W par rapport à S^{-1}B et on peut par suite lui appliquer le th. 2 du n° 2, qui donne S^{-1}R = \bigcap_i (S^{-1}R)_{m_i} : mais (S^{-1}R)_{m_i} = R_{\mathfrak{p}_i}, ce qui prouve le lemme.

Revenant à la démonstration de la prop. 19, on a, en vertu du lemme 4, $\bigcap_{\mathfrak{p} \in P(B)} R_{\mathfrak{p}} = \bigcap_{p \in P(A)} (R_{[A]})_p$, et la conclusion résulte du n° 2, th. 2.

#### Corollaire {#ac-vii-s4-n8-cor-1 .statement}

L’anneau B est un A-module réflexif.

#### Proposition 20 {#ac-vii-s4-prop-20 .statement}

(i) Pour qu’un A-module de type fini M soit pseudo-nul, il faut et il suffit que M \otimes_A B soit un B-module pseudo-nul.

(ii) Si M est un A-module de torsion de type fini, M \otimes_A B est un B-module de torsion de type fini, et l’on a:

(22)
$$ \chi_B(M \otimes_A B) = i(\chi_A(M)). $$

(iii) Si M est un A-module de type fini, M \otimes_A B est un B-module de type fini, et l’on a:

(23)
$$ c_B(M \otimes_A B) = i(c_A(M)) $$
(24)
$$ r_B(M \otimes_A B) = r_A(M). $$

(i) Soient $\mathfrak{p}$ un idéal premier de B, $p = \mathfrak{p} \cap A$; on a $(M \otimes_A B)_\mathfrak{p} = M \otimes_A B_\mathfrak{p}$ (chap. II, § 2, n° 7, prop. 18), et d’autre part $M \otimes_A B_\mathfrak{p} = (M \otimes_A A_p) \otimes_{A_p} B_\mathfrak{p} = M_p \otimes_{A_p} B_\mathfrak{p}$; la relation $M_p = 0$ est donc équivalente à $(M \otimes_A B)_\mathfrak{p} = 0$ (chap. II, § 4, n° 4, lemme 4). Il suffit d’appliquer cette remarque à l’idéal $\mathfrak{p} = (0)$ et aux idéaux $\mathfrak{p} \in P(B)$ pour prouver (i), compte tenu du n° 4, déf. 2.

Pour prouver (ii), nous utiliserons le lemme suivant:

#### Lemme 5 {#ac-vii-s4-lem-5 .statement}

Soient M_1, M_2 deux A-modules de type fini, f : M_1 \to M_2 un homomorphisme injectif. Alors le noyau de $f \otimes 1_B : M_1 \otimes_A B \to M_2 \otimes_A B$ est pseudo-nul.

Soit p un idéal premier de A de hauteur $\leq 1$. On a $(M_i \otimes_A B)_p = (M_i)_p \otimes_{A_p} B_p$ ($i = 1, 2$) (chap. II, § 2, n° 7, prop. 18) et $(f \otimes 1_B)_p = f_p \otimes 1_{B_p}$; l’hypothèse que f est injectif entraîne qu’il en est de même de $f_p$ (chap. II, § 2, n° 4, th. 1); d’autre part, vu le choix de p, $A_p$ est un anneau principal et $B_p$ un $A_p$-module sans torsion de type fini, donc libre; on en conclut que $f_p \otimes 1_{B_p}$ est lui aussi injectif. Si I = Ker(f \otimes 1), on a $I_p = \mathrm{Ker}((f \otimes 1)_p)$ (chap. II, § 2, n° 4, th. 1); on a donc $I_p = 0$, d’où *a fortiori* $I_{\mathfrak{P}} = (I_p)_{\mathfrak{P}} = 0$ pour $\mathfrak{P}|p$, ce qui prouve le lemme (n° 4, déf. 2).

Revenons à la démonstration de (ii). Pour tout A-module de torsion de type fini M, posons $\varphi(M) = \chi_B(M \otimes_A B)$; il résulte de (i) que si M est pseudo-nul, on a $\varphi(M) = 0$. D’autre part, considérons une suite exacte de A-modules de torsion de type fini :

$$
0 \to M_1 \to M_2 \to M_3 \to 0.
$$

Il résulte du lemme 4 que l’on a une suite exacte de B-modules :

$$
0 \to I \to M_1 \otimes_A B \to M_2 \otimes_A B \to M_3 \otimes_A B \to 0
$$

où I est pseudo-nul. En utilisant le n° 5, cor. de la prop. 10, on a donc $\varphi(M_2) = \varphi(M_1) + \varphi(M_3)$. On conclut donc de la prop. 11 du n° 5 qu’il existe un homomorphisme $\theta : D(A) \to D(B)$ tel que $\varphi(M) = \theta(\chi_A(M))$ pour tout A-module de torsion de type fini M. Pour prouver que $\theta = i$, il suffit de montrer que $\varphi(A/p) = i(p)$ pour tout $p \in P(A)$; or on a $(A/p) \otimes_A B = B/pB$, et pour tout $\mathfrak{P} \in P(B)$, $(B/pB)_{\mathfrak{P}} = B_{\mathfrak{P}}/pB_{\mathfrak{P}}$; ce dernier module est 0 si $\mathfrak{P}$ n’est pas au-dessus de p ; si au contraire $\mathfrak{P}|p$, $B_{\mathfrak{P}}/pB_{\mathfrak{P}}$ est un $B_{\mathfrak{P}}$-module de longueur $e(\mathfrak{P}/p)$ par définition de l’indice de ramification (chap. VI, § 8, n° 1); on a donc $\chi_B(B/pB) = \sum_{\mathfrak{P}|p} e_{\mathfrak{P}/p} \cdot \mathfrak{P} = i(p)$, ce qui achève de prouver (ii).

La formule (24) est immédiate, car

$$
(M \otimes_A B) \otimes_B L = M \otimes_A L = (M \otimes_A K) \otimes_K L
$$

et le rang sur L de $(M \otimes_A K) \otimes_K L$ est égal au rang sur K de $M \otimes_A K$. Pour démontrer (23), considérons un sous-module libre H de M tel que Q = M/H soit un A-module de torsion. Appliquant comme ci-dessus le lemme 4, on a une suite exacte de B-modules :

$$
0 \to I \to H \otimes_A B \to M \otimes_A B \to Q \otimes_A B \to 0
$$

où I est pseudo-nul. Il résulte donc du n° 7, prop. 16, (ii) et (v) et cor. 1 de la prop. 16, que l’on a

$$
c_B(M \otimes_A B) = c_B(Q \otimes_A B) = -c_B(\chi_B(Q \otimes_A B)) = -c_B(i(\chi_A(Q)))
$$

en vertu de (ii); mais par définition de l’homomorphisme $i : C(A) \to C(B)$ on a $c_B(i(\chi_A(Q))) = i(c_A(\chi_A(Q))) = -i(c_A(M))$, ce qui achève de prouver (23).

#### Remarque 1 {#ac-vii-s4-n8-rem-1 .statement}

Si M est un A-module réflexif, $M \otimes_A B$ n’est pas nécessairement réflexif (exerc. 6). Il en est toutefois ainsi lorsque B est un A-module *plat* (n° 2, prop. 8).

#### Remarque 2 {#ac-vii-s4-n8-rem-2 .statement}

Soit C un troisième anneau noethérien intégralement clos, tel que B ⊂ C et que C soit un B-module de type fini (donc aussi un A-module de type fini). On a alors les formules de transitivité:

(25) $N_{C/A} = N_{B/A} \circ N_{C/B}$,

(26) $i_{C/A} = i_{C/B} \circ i_{B/A}$

qui résultent immédiatement des formules de transitivité pour les indices de ramification et les degrés résiduels (chap. VI, § 8, n° 1, lemme 1).

### 9. Un théorème de réduction

Les notations et hypothèses sont de nouveau celles des n°s 2 à 7.

#### Lemme 6 {#ac-vii-s4-lem-6 .statement}

Soient R un anneau commutatif, $p_i$ ($1 \leqslant i \leqslant n$) des idéaux premiers de R, deux à deux distincts.

(i) Pour $1 \leqslant i \leqslant n$, soit $H_i$ une partie de $R/p_i$ vérifiant la condition suivante: il n’existe aucun élément $\alpha_i \in R/p_i$ tel que $\alpha_i + H_i$ contienne un idéal $\neq 0$ de $R/p_i$. Alors il existe $a \in R$ tel que, pour $1 \leqslant i \leqslant n$, l’image canonique de a dans $R/p_i$ n’appartienne pas à $H_i$.

(ii) Si Card($H_i$) < Card($R/p_i$), les $H_i$ vérifient la condition de (i).

(i) Raisonnons par récurrence sur n, le cas $n = 0$ étant trivial. Soit donc $n \geqslant 1$. Quitte à faire une permutation sur les indices i, on peut supposer que $p_1$ est minimal parmi les $p_i$ et par suite, pour $2 \leqslant i \leqslant n$, il existe $c_i \in p_i$ tel que $c_i \notin p_1$. En vertu de l’hypothèse de récurrence, il existe $b \in R$ tel que l’image canonique de b dans $R/p_i$ n’appartienne pas à $H_i$ pour $2 \leqslant i \leqslant n$. Pour tout $x \in R$, posons $a_x = b + x c_2 c_3 \cdots c_n$; comme $c_i \in p_i$, on a évidemment $a_x \equiv b$ (mod. $p_i$) pour $2 \leqslant i \leqslant n$. Il suffit donc de prouver qu’il existe $x \in R$ tel que l’image canonique de $a_x$ dans $R/p_1$ n’appartienne pas à $H_1$. Or, l’ensemble des images canoniques des $a_x$ dans $R/p_1$, lorsque x parcourt R, n’est autre que $\beta + c$, où $\beta$ est l’image canonique de b et c l’idéal de $R/p_1$ engendré par l’image canonique de $c_2 c_3 \cdots c_n$; en vertu du choix des $c_i$, on a $c \neq 0$ puisque $R/p_1$ est intègre, et l’hypothèse sur $H_1$ entraîne l’existence d’un x répondant à la question.

(ii) Comme $R/p_i$ est intègre, tout idéal $\neq 0$ de $R/p_i$ a un cardinal égal à celui de $R/p_i$, et il en est de même de tout translaté d’un idéal par un élément de $R/p_i$, d’où la conclusion.

#### Théorème 6 {#ac-vii-s4-thm-6 .statement}

Soit $M$ un $A$-module sans torsion de type fini. Il existe un sous-module libre $L$ de $M$ tel que $M/L$ soit isomorphe à un idéal de $A$.

Nous désignerons par $n$ le rang de $M$ (rang de $V = M \otimes_A K$ sur $K$) et nous considérerons $M$ comme un réseau de $V$ par rapport à $A$. Alors pour tout $p \in P(A)$, $M_p$ est un réseau de $V$ par rapport à $A_p$ (n° 1, Exemple 6), et comme $A_p$ est un anneau principal, $M_p$ est un $A_p$-module libre de rang $n$. Nous poserons :

$$
M(p) = M_p / pM_p.
$$

Nous désignerons par $k(p)$ le corps des fractions de $A/p$ (isomorphe au corps résiduel de $A_p$); $M(p) = M \otimes_A k(p)$ est donc un espace vectoriel de rang $n$ sur $k(p)$. Pour tout $x \in M$, nous noterons $x(p)$ l’image canonique de $x$ dans $M(p)$.

#### Lemme 7 {#ac-vii-s4-lem-7 .statement}

Soient $x_i$ ($1 \leq i \leq m$) des éléments de $M$ linéairement indépendants (sur $A$ ou sur $K$, ce qui revient au même), et soit $L$ le sous-A-module de $M$ engendré par les $x_i$. Alors, pour presque tout $p \in P$, les $x_i(p) \in M(p)$ sont linéairement indépendants sur $k(p)$; pour qu’ils soient linéairement indépendants sur $k(p)$ pour tout $p \in P$, il faut et il suffit que $M/L$ soit sans torsion.

Soient $x_{m+1}, \ldots, x_n$ des éléments de $M$ qui, avec $x_1, \ldots, x_m$, forment une base de $V$, et soit $N$ le sous-A-module libre de $M$ engendré par les $x_i$ ($1 \leq i \leq n$). Il résulte du n° 3, th. 3 que l’on a $N_p = M_p$ pour presque tout $p \in P$; comme $x_1(p), \ldots, x_n(p)$ forment une base de $N(p)$ sur $k(p)$, cela établit la première assertion.

Si $M/L$ est sans torsion, il en est de même de $(M/L)_p = M_p / L_p$ pour tout $p \in P$ (n° 1, Exemple 6), et comme $A_p$ est principal, $M_p / L_p$ est libre. Par suite, $M_p$ est somme directe de $L_p$ et d’un $A_p$-module libre $E$ de rang $n - m$; donc $M(p)$ est somme directe de $L(p)$ et du $k(p)$-espace vectoriel $E/pE$, de rang $n - m$; par suite $L(p)$ est de rang $m$, et comme il est engendré par les $x_i(p)$ ($1 \leq i \leq m$), ces derniers sont linéairement indépendants.

Inversement, supposons que les $x_i(p)$ ($1 \leq i \leq m$), soient linéairement indépendants sur $k(p)$ pour tout $p \in P$. Alors $L_p$ est facteur direct de $M_p$ pour tout $p$ (chap. II, § 3, n° 2, cor. 1 de la prop. 5), et par suite $M_p / L_p = (M/L)_p$ est sans torsion pour tout $p \in P$. On en conclut que $P \cap \operatorname{Ass}(M/L) = \phi$ en vertu du chap. IV, § 1, n° 2, cor. de la prop. 5. Mais comme $L$ est réflexif, il résulte du n° 2, prop. 7, (i), que le seul idéal premier qui puisse appartenir à $\operatorname{Ass}(M/L)$ est l’idéal (0); donc $M/L$ est sans torsion.

#### Lemme 8 {#ac-vii-s4-lem-8 .statement}

Supposons que le rang n de M soit $\geqslant 2$; alors il existe un élément $x \neq 0$ de M tel que $M/Ax$ soit sans torsion.

Soit $y \neq 0$ un élément de M. En vertu du lemme 7, l’ensemble Y des $p \in P$ tels que $y(p) = 0$ est fini. Si $Y = \phi$, il résulte du lemme 7, appliqué à la suite $(x_i)$ formée du seul élément y, que $M/Ay$ est sans torsion. Supposons donc $Y \neq \phi$, et posons $S = \bigcap_{p \in Y} (A - p)$; on sait (n° 4, lemme 2) que $S^{-1}A$ est un anneau principal semi-local, dont les idéaux maximaux sont les $pS^{-1}A$, où $p \in Y$, les anneaux locaux correspondants étant les $A_p$. On a donc

$$
S^{-1}A/pS^{-1}A = k(p),
$$

d’où

$$
S^{-1}M/pS^{-1}M = (M/pM) \otimes_A S^{-1}A = M \otimes_A ((A/p) \otimes_A S^{-1}A)
$$
$$
= M \otimes_A k(p) = M(p)
$$

pour tout $p \in Y$. En vertu du chap. II, § 1, n° 2, prop. 6, il existe un élément $z/s \in S^{-1}M$ ($z \in M, s \in S$) dont les images canoniques dans les $M(p)$ pour $p \in Y$ sont toutes $\neq 0$. Par définition de S, on a donc $z(p) \neq 0$ pour tout $p \in Y$. On peut en outre supposer que y et z sont linéairement indépendants sur K. En effet, dans le cas contraire, considérons un élément $t \in M$ linéairement indépendant de y (il en existe puisque $n \geqslant 2$); prenons d’autre part un élément $a \neq 0$ appartenant à $\bigcap_{p \in Y} p$ (qui n’est pas réduit à 0 puisque A est intègre), et posons $z' = z + at$: il est clair que y et $z'$ sont linéairement indépendants sur K et que l’on a $z'(p) = z(p) \neq 0$ pour tout $p \in Y$.

Supposant donc y et z linéairement indépendants sur K, soit Z l’ensemble des $p \in P - Y$ tels que $y(p)$ et $z(p)$ soient linéairement dépendants sur $k(p)$; il résulte du lemme 7 que cet ensemble est fini. Pour tout $p \in Z$, on peut donc écrire $z(p) = \lambda(p)y(p)$ avec $\lambda(p) \in k(p)$. Or, on a Card(A/p) $\geqslant 2$ pour tout $p \in P$; il résulte donc du lemme 6 qu’il existe $b \in A$ tel que, pour tout $p \in Z$, l’image canonique de b dans $A/p$ soit distincte de $\lambda(p)$. Montrons alors que l’élément $x = z - by$ répond à la question; il suffit (en vertu du lemme 7 appliqué pour $m = 1$), de vérifier que $x(p) \neq 0$ pour tout $p \in P$. Or:

— si $p \in Y$, on a $x(p) \neq 0$ par construction;
— si $p \in Z$, on a $x(p) = \mu_p \cdot y(p)$ avec $\mu_p \neq 0$ en vertu du choix de b, donc $x(p) \neq 0$ puisque $y(p) \neq 0$;

—si $p \in P - (Y \cup Z)$, $y(p)$ et $z(p)$ sont linéairement indépendants, donc $x(p) \neq 0$.

Ces lemmes étant établis, passons à la démonstration du th. 6. Raisonnons par récurrence sur $n$, le cas $n \leq 1$ étant trivial puisque $M$ lui-même est alors isomorphe à un idéal de $A$. Supposons donc $n \geq 2$; en vertu du lemme 8, il existe un sous-module libre $L_0$ de $M$, de rang 1, tel que $M/L_0$ soit sans torsion ; $M/L_0$ est donc de rang $n - 1$. En vertu de l’hypothèse de récurrence, il y a donc un sous-module libre $L_1$ de $M/L_0$ tel que $(M/L_0)/L_1$ soit isomorphe à un idéal de $A$. Soit $L$ l’image réciproque de $L_1$ dans $M$; $L/L_0$ est isomorphe à $L_1$, et puisque $L_1$ est libre, $L$ est isomorphe à $L_0 \oplus L_1$ (*Alg.*, chap. II, 3e éd., § 1, no 11, prop. 21), donc libre; comme $M/L$ est isomorphe à $(M/L_0)/L_1$, le théorème est démontré.

#### Remarque {#ac-vii-s4-n9-rem-1 .statement}

Si $M$ est réflexif, il n’en est pas nécessairement de même de $M/L$ (exerc. 9).

### 10. Modules sur les anneaux de Dedekind

On suppose maintenant que $A$ soit un *anneau de Dedekind*; on sait alors que les idéaux $p \in P$ sont *maximaux* et que ce sont les seuls idéaux premiers $\neq 0$ de $A$ (§ 2, no 1); le groupe $D(A)$ s’identifie au groupe $I(A)$ des idéaux fractionnaires $\neq 0$ de $A$.

#### Proposition 21 {#ac-vii-s4-prop-21 .statement}

*Soit $A$ un anneau de Dedekind. Tout $A$-module pseudo-nul est nul. Tout homomorphisme pseudo-injectif (resp. pseudo-surjectif, pseudo-bijectif, pseudo-nul) de $A$-modules est injectif (resp. surjectif, bijectif, nul).*

Le première assertion a déjà été démontrée (no 4, Exemple 1); les autres s’en déduisent immédiatement.

#### Proposition 22 {#ac-vii-s4-prop-22 .statement}

*Soient $A$ un anneau de Dedekind, $M$ un $A$-module de type fini. Les propriétés suivantes sont équivalentes:*
a) $M$ est sans torsion.
b) $M$ est réflexif.
c) $M$ est projectif.

On sait déjà (sans hypothèse sur l’anneau intègre $A$) que b) implique a) (no 2, Remarque 1) et que c) implique b) (*Alg.*, chap. II, 3e éd., § 2, n° 7, cor. 4 de la prop. 14). Si M est sans torsion, il s’identifie à un réseau de V = M ⊗_A K par rapport à A ; M_p est donc un A_p-module libre pour tout idéal maximal p ∈ P, puisque A_p est principal. La conclusion résulte alors du chap. II, § 5, n° 2, th. 1, b).

#### Corollaire {#ac-vii-s4-n10-cor-1 .statement}

Soit M un A-module de type fini, et soit T son sous-module de torsion. Alors T est facteur direct dans M.
En effet, comme M/T est sans torsion et de type fini, il est projectif en vertu de la prop. 22, et le corollaire résulte donc d’Alg., chap. II, 3e éd., § 2, n° 2, prop. 4.

#### Proposition 23 {#ac-vii-s4-prop-23 .statement}

Soient A un anneau de Dedekind, T un A-module de torsion de type fini. Il existe deux familles finies (n_i)_{i∈I} et (p_i)_{i∈I}, où les n_i sont des entiers ≥ 1 et les p_i des éléments de P, telles que T soit isomorphe à la somme directe $\bigoplus_{i∈I} (A/p_i^{n_i})$. De plus, les familles (n_i)_{i∈I} et (p_i)_{i∈I} sont uniques à une bijection près de l’ensemble d’indices.
Cela résulte du n° 4, th. 5, compte tenu du fait qu’un pseudo-isomorphisme est ici un isomorphisme.

#### Proposition 24 {#ac-vii-s4-prop-24 .statement}

Soient A un anneau de Dedekind, M un A-module sans torsion de type fini, de rang n ≥ 1. Il existe alors un idéal 𝔅 ≠ 0 de A tel que M soit isomorphe à la somme directe des modules A^{n−1} et 𝔅. De plus, la classe de l’idéal 𝔅 est déterminée de manière unique par cette condition.
Le th. 6 du n° 9 montre qu’il existe un sous-module libre L de M tel que M/L soit isomorphe à un idéal a de A. Si a = 0, on prend 𝔅 = A. Dans le cas contraire, a est de rang 1, donc L = A^{n−1}, et a est un module projectif (prop. 22); M est par suite isomorphe à la somme directe de L et de a (Alg., chap. II, 3e éd., § 2, n° 2, prop. 4), ce qui prouve la première partie de la proposition. En outre, il résulte du n° 7, prop. 16, (i), (iv) et (v), que l’on a c(M) = c(𝔅), d’où l’unicité de la classe de 𝔅.

#### Remarque 1 {#ac-vii-s4-n10-rem-1 .statement}

Les prop. 23, 24 et le cor. de la prop. 22 déterminent complètement la structure des A-modules de type fini. La prop. 24 montre qu’un A-module sans torsion de type fini est déterminé à un isomorphisme près par son rang et par la classe de diviseurs qui lui est attachée.

#### Remarque 2 {#ac-vii-s4-n10-rem-2 .statement}

On peut montrer que sur un anneau de Dedekind, un module projectif qui n’est pas de type fini est nécessairement libre (exerc. 21) et que tout sous-module d’un module projectif est projectif (exerc. 20).

## EXERCICES {#ac-vii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
