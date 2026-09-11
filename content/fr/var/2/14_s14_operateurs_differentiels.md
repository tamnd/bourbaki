---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 14
section_title: Opérateurs différentiels
lang: fr
source: var-fr
pdf_pages: 0162-0173
extraction: ocr
subsections:
    - "no": 1
      title: Opérateurs différentiels
      page: 0
      pdf_page: 162
    - "no": 2
      title: Symboles
      page: 0
      pdf_page: 166
    - "no": 3
      title: Transposition
      page: 0
      pdf_page: 169
    - "no": 4
      title: Exemples
      page: 0
      pdf_page: 172
statements: 2
exercises: 0
content_sha256: 1392eb42732e48e986a4b120baebb41eb1413b70e59d35e31a21984b15deb2b5
---

## § 14. Opérateurs différentiels

Dans ce paragraphe, X désigne une variété localement de dimension finie de classe $C^r$, où $r \in \mathbf{N}_k$; on note E et F deux fibrés vectoriels de rang fini de classe $C^r$ et de base X.

Toutes les variétés et tous les fibrés vectoriels considérés sont supposés localement de dimension finie.

### 14.1. Opérateurs différentiels

### 14.1.1. Soit k un entier tel que $0 \leq k \leq r$, et soit $P^k(E)$ le fibré des jets de sections d’ordre k de E (12.6.1). Posons

$$
D^k(E,F)=\mathscr{L}(P^k(E);F).
$$

C’est un fibré vectoriel de base X et de classe $C^{r-k}$. Une section de ce fibré sur un ouvert U de X s’identifie à une application

$$
D:P^k(E)|U\longrightarrow F|U
$$

qui commute à la projection sur U et est linéaire sur chaque fibre ; une telle section est appelée un opérateur différentiel sur U, de type $E \rightarrow F$, et d’ordre $\leq k$. Soit $h \in \mathbf{N}_k \cup \{0\}$, avec $0 \leq h \leq r-k$. On note $\mathscr{D}^{k,h}_U(E,F)$ l’ensemble des opérateurs différentiels sur U, de type $E \rightarrow F$ et d’ordre $\leq k$, qui sont de classe $C^h$ (comme sections de $D^k(E,F)$, ou comme morphismes de $P^k(E)|U$ dans $F|U$, cela revient au même). Si $M=D^k(E,F)$, on a $\mathscr{D}^{k,h}_U(E,F)=\mathscr{F}^h_M(U)$; c’est un module sur $\mathscr{C}^h(U)$, cf. 7.4.1.

Si $0 \leq k' \leq k$, le morphisme $r^{k,k'}:P^k(E)\longrightarrow P^{k'}(E)$ (cf. 12.6.6) définit une injection de $D^{k'}(E,F)$ dans $D^k(E,F)$; tout opérateur différentiel d’ordre $\leq k'$ est ainsi identifié à un opérateur différentiel d’ordre $\leq k$. Un opérateur différentiel d’ordre $\leq k$ qui n’est pas d’ordre $\leq k-1$ est dit parfois d’ordre k. Si $h \in \mathbf{N}_k \cup \{0\}$ et $h \leq r-k$, et si U est un ouvert de X, on a :

$$
0 \subset \mathscr{D}^{0,h}_U(E,F) \subset \mathscr{D}^{1,h}_U(E,F) \subset \cdots \subset \mathscr{D}^{k,h}_U(E,F).
$$

Si $r=\infty$ ou $\omega$, on note $\mathscr{D}^{\omega,h}_U(E,F)$ la réunion des $\mathscr{D}^{k,h}_U(E,F)$ pour $k \geq 0$; un élément de cette réunion s’appelle un opérateur différentiel sur U d’ordre borné (de type $E \rightarrow F$, de classe $C^h$) ou parfois simplement un opérateur différentiel sur U.

### 14.1.2 (« Opérateurs d’ordre zéro »). On a $P^0(E)=E$ (12.5.1) et $D^0(E,F)=\mathscr{L}(E;F)$. Si U est ouvert dans X, et si $h \in \mathbf{N}_k \cup \{0\}$ et $h \leq r$, un élément de $\mathscr{D}^{0,h}_U(E,F)$ est un morphisme de classe $C^h$ de $E|U$ dans $F|U$.

14.1.3 (« Affaiblissement de structure »). Supposons $K = \mathbf{R}$, et soit $r' \in \mathbf{N}_\mathbf{R}$ avec $r' \leq r$. Soient $X', E'$ et $F'$ la variété et les fibrés vectoriels de classe $C^{r'}$ obtenus par affaiblissement de structure à partir de $X, E,$ et $F$ respectivement. Soit $k$ un entier tel que $0 \leq k \leq r'$. Alors $P^k(E')$ est le fibré de classe $C^{r'-k}$ déduit de $P^k(E)$ par affaiblissement de structure, et l’on a un résultat analogue pour $D^k(E', F')$. En particulier, si $U$ est ouvert dans $X$, et si $0 \leq h \leq r - k'$, on a $\mathscr{D}_U^{k',h}(E', F') = \mathscr{D}_U^{k,h}(E, F)$.

14.1.4. Soit $D$ un opérateur différentiel sur $X$, de type $E \to F$, d’ordre $\leq k$ (où $0 \leq k \leq r$). Soit $U$ un ouvert de $X$, et soit $s$ une section, de classe $C^m$, de $E$ sur $U$, avec $m \in \mathbf{N}_K \cup \{0\}$ et $k \leq m \leq r$. Alors $j^k(s)$ est une section de classe $C^{m-k}$ de $P^k(E)$ sur $U$ (12.6.1); son image par $D$ est notée $D_U(s)$, ou $D(s)$. C’est une section de $F|U$. Supposons $D$ de classe $C^h$, où $h = m - k$. Alors $D_U(s)$ est de classe $C^h$, et les applications
$$
D_U : \mathscr{S}_E^m(U) \to \mathscr{S}_F^h(U)
$$
ainsi obtenues jouissent des propriétés suivantes:

(1) $D_U$ est $K$-linéaire.
(2) Pour tout $s \in \mathscr{S}_E^m(U)$ et tout ouvert $V$ de $U$, on a $D_V(s|V) = D_U(s)|V$.
(3) Pour tout $s \in \mathscr{S}_E^m(U)$ et tout $x \in U$ tels que $j_x^k(s) = 0$, on a $D_U(s)(x) = 0$.
(3') Pour tout système de coordonnées $\xi = (\xi^1, \ldots, \xi^n)$ dans $U$ et tout repère $s = (s_1, \ldots, s_d)$ de $E$ sur $U$ (7.4.4), il existe des sections $n_{i,\alpha} (1 \leq i \leq d, \alpha \in \mathbf{N}^n, |\alpha| \leq k)$ de $F$ sur $U$, de classe $C^h$ et telles que, pour toute famille $(f_i)_{1 \leq i \leq d}$ d’éléments de $\mathscr{C}^m(U)$, on ait
$$
D_U \left( \sum_{1 \leq i \leq d} f_i . s_i \right) = \sum_{1 \leq i \leq d, |\alpha| \leq k} \Delta_\xi^\alpha(f_i) . n_{i,\alpha}, \quad \text{(cf. 13.2.6).}
$$
(4) Pour toute fonction $f \in \mathscr{C}^m(U)$ et toute application $\theta$ de $\mathscr{S}_U^m(E)$ dans $\mathscr{S}_U^h(F)$, notons $\operatorname{ad}(f)\theta$ l’application
$$
s \mapsto f . \theta(s) - \theta(f.s)
$$
de $\mathscr{S}_U^m(E)$ dans $\mathscr{S}_U^h(F)$. Alors, pour toute fonction $f \in \mathscr{C}^m(U)$, il existe un opérateur différentiel $L$ sur $U$, de type $E \to F$, d’ordre $\leq k - 1$ et de classe $C^h$ tel que
$$
(\operatorname{ad}(f)D_U)(s) = L_U(s) \quad \text{pour tout } s \in \mathscr{S}_U^m(E).
$$
(5) On a
$$
\operatorname{ad}(f_0) \ldots \operatorname{ad}(f_k) D_U = 0 \quad \text{quels que soient } f_0, \ldots, f_k \text{ dans } \mathscr{C}^m(U).
$$
Si l’on pose $I = \{0, \ldots, k\}$ et $f_H = \prod_{i \in H} f_i$ pour toute partie $H$ de $I$, la relation précédente équivaut à:
$$
\sum_{H \subset I} (-1)^{\operatorname{Card}(H)} f_H . D_U(f_{I-H}.s) = 0
$$
quelles que soient $f_0, \ldots, f_k$ dans $\mathscr{C}^m(U)$ et $s$ dans $\mathscr{S}_E^m(U)$.

14.1.5 (« Caractérisation des opérateurs différentiels »). Soient $k, m$ et $h = m - k$ comme dans 14.1.4. Pour tout ouvert $U$ de $X$, soit $D_U$ une application de $\mathscr{S}_E^m(U)$ dans $\mathscr{S}_F^h(U)$. Supposons que les conditions 1, 2, 3 (resp. 1, 2, 3’) de 14.1.4 soient vérifiées pour toute partie ouverte U de X. Il existe alors un élément D de $\mathscr{D}_X^{k,h}(E, F)$ et un seul tel que les $D_U$ soient les applications correspondantes.$^{(1)}$ Dans ce qui suit, on identifie D à la famille des $D_U$.

Lorsque $m = \infty$ ou $\omega$, on a $h = m$ et l’on peut remplacer les conditions (3) et (3') par l’une des conditions (4) et (5).

14.1.6 (« Opérateurs scalaires »). Supposons que E et F soient égaux au fibré trivial $K_X$. Un opérateur différentiel de type $E \to F$ s’appelle alors un opérateur différentiel *scalaire* ou simplement un opérateur différentiel ; s’il est d’ordre $\leq k$, c’est une section du fibré $\mathscr{L}(P^k(X); K_X) = P^k(X)^*$, *dual* du fibré $P^k(X)$; en utilisant l’isomorphisme
$$
i^{-1} : P^k(X)^* \to T^{(k)}(X) \quad (\text{cf. } 13.2.5),
$$
on voit qu’un opérateur différentiel scalaire d’ordre $\leq k$ s’identifie à une *section* du fibré vectoriel $T^{(k)}(X)$, i.e. à un *champ de distributions ponctuelles d’ordre* $\leq k$.

Prenons en particulier pour X un ouvert de $K^n$, où n est un entier $\geq 0$. Les champs de distributions ponctuelles
$$
\Delta^\alpha : x \mapsto \Delta_x^\alpha \quad (\text{cf. } 13.2.6)
$$
sont des opérateurs différentiels scalaires de classe $C^\omega$. Pour tout $h \in N_K$, les $\Delta^\alpha$ pour $(|\alpha| \leq k)$ forment une *base* du $C^h(X)$-module $\mathscr{D}_X^{k,h}(K_X, K_X)$.

14.1.7 (« Opérateurs différentiels complexes sur une variété réelle »). Supposons $K = \mathbf{R}$ et que les fibrés vectoriels E et F soient munis de *structures complexes* (8.8.1) ; soit k un entier tel que $0 \leq k \leq r$. Le fibré $P^k(E)$ est alors muni d’une structure complexe (12.6.3) ; le fibré $\mathscr{L}_c(P^k(E); F)$ (7.8.5) des applications linéaires *complexes* de $P^k(E)$ dans F est un sous-fibré vectoriel de $\mathscr{L}(P^k(E); F) = D^k(E, F)$; on le note $D_c^k(E, F)$. Une section de $D_c^k(E, F)$ est appelée un opérateur différentiel *complexe*, de type $E \to F$ et d’ordre $\leq k$. Si $h \in N_K$ et $h \leq r - k$, et si U est un ouvert de X, on note de même $\mathscr{D}_U^{k,h}(E, F)_c$ l’espace des sections de classe $C^h$ de $D_c^k(E, F)$ sur U ; c’est un C-espace vectoriel. Les autres définitions et résultats de ce paragraphe s’étendent de manière analogue aux opérateurs différentiels complexes ; nous en laissons la formulation au lecteur.

14.1.8 (« Composition »). Soit G un fibré vectoriel de classe $C^r$ et de base X. Soient $k'$ et $k''$ des entiers positifs de somme $k \leq r$, et soit $D'$ (resp. $D''$) un opérateur différentiel sur X, de type $E \to F$ (resp. de type $F \to G$), d’ordre $\leq k'$ (resp. $\leq k''$). Supposons $D' : P^{k'}(E) \to F$ de classe $C^{h'}$, avec $h' \in N_K \cup \{0\}$ et $k'' \leq h' \leq r - k'$; l’application
$$
D'_* = P^{k''}(D') : P^{k''}(P^{k'}(E)) \to P^{k''}(F)
$$
est de classe $C^{h'-k''}$ (12.6.3). Soit $\beta$ l’homomorphisme canonique de $P^{k}(E)$ dans $P^{k''}(P^{k'}(E))$, cf. 12.6.5. En composant les applications
$$
P^k(E) \xrightarrow{\beta} P^{k''}(P^{k'}(E)) \xrightarrow{D'_*} P^{k''}(F) \xrightarrow{D''} G,
$$
on obtient un opérateur différentiel de type $E \to G$ et d’ordre $\leq k$. Cet opérateur est dit le *composé* de $D''$ et $D'$; on le note $D'' \circ D'$.

$^1$ Il suffit d’ailleurs que la condition (3') soit vérifiée pour une famille $(\xi_\lambda)$ de systèmes de coordonnées et une famille de repères $(s_\lambda)$ dont les domaines recouvrent X.

Si U est un ouvert de X, et si s ∈ $\mathscr{S}_E^{k}(U)$, on a
$$
(D'' \circ D')(s) = D''(D'(s))
$$
(où les deux membres sont des sections de G sur U); cela justifie la terminologie et la notation adoptées.

Supposons maintenant D'' de classe $C^{h''}$, avec $h'' \in \mathbf{N}_K \cup \{0\}$ et $h'' \leq r - k''$. Alors $D'' \circ D'$ est de classe $C^h$, avec $h = \inf(h' - k'', h'')$.

Supposons que l’on ait $E = F = G$, et que $k' \leq h''$, auquel cas $D' \circ D''$ est défini. Alors $D' \circ D'' - D'' \circ D'$ est un opérateur différentiel de type $E \to E$ et d’ordre $\leq k - 1$; on le note $[D', D'']$.

14.1.9 (« Associativité »). Les notations et hypothèses étant celles de 14.1.8, soit H un fibré vectoriel de classe $C^r$ et de base X, et soit $D'''$ un opérateur différentiel sur X, de type $G \to H$ et d’ordre $\leq k'''$, avec $k' + k'' + k''' \leq r$. On suppose que $D'$ est de classe $C^{h'}$, avec $h' \in \mathbf{N}_K \cup \{0\}$ et $k'' + k''' \leq h' \leq r - k'$ et que $D''$ est de classe $C^{h''}$, avec $h'' \in \mathbf{N}_K \cup \{0\}$ et $k''' \leq h'' \leq r - k''$. Alors les composés
$$
D''' \circ (D'' \circ D') \quad \text{et} \quad (D''' \circ D'') \circ D'
$$
sont définis et sont égaux.

14.1.10. Exemples

a) Soit U un ouvert de X, soit $D \in \mathscr{D}_U^{k,h}(E, F)$ avec $h \in \mathbf{N}_K \cup \{0\}$ et $h \leq r - k$, et soit $f \in \mathscr{C}^{h+k}(U)$ (resp. $f \in \mathscr{C}^h(U)$). La multiplication par f dans E (resp. F) est un opérateur différentiel sur U d’ordre $\leq 0$, et de type $E \to E$ (resp. $F \to F$), cf. 14.1.2. Les composés $D \circ f$ et $f \circ D$ sont définis et appartiennent à $\mathscr{D}_U^{k,h}(E; F)$; on pose
$$
\operatorname{ad}(f)D = f \circ D - D \circ f \in \mathscr{D}_U^{k-1,h}(E, F),
$$
cf. 14.1.4, (4). On munit ainsi $\mathscr{D}_U^{k,h}(E, F)$ d’une structure de $\mathscr{C}^{h+k}(U)$-module à droite (resp. de $\mathscr{C}^h(U)$-module à gauche). La structure de module à gauche coïncide avec celle de 14.1.1.

b) Supposons $r = \infty$ ou $r = \omega$. Les opérateurs différentiels de type $E \to E$ et de classe $C^r$ forment une K-algèbre associative à élément unité.

c) Prenons pour X un ouvert de $K^n$. Les opérateurs différentiels scalaires $\Delta^\alpha$ (14.1.6) vérifient les formules
$$
\Delta^\alpha \circ \Delta^\beta = ((\alpha, \beta)) \Delta^{\alpha+\beta}.
$$
Ils commutent entre eux. Notons $D_i$ l’opérateur $\Delta^{\varepsilon_i}$ (« i-ème dérivée partielle »). Si K est de caractéristique 0, on a
$$
\Delta^\alpha = \frac{1}{\alpha!} D_1^{\alpha_1} \ldots D_n^{\alpha_n}.
$$
Si K est de caractéristique $p \neq 0$, on a $D_i^p = 0$ pour tout $i$.

14.1.11 (« Opérateurs multidifférentiels »). Soient $E_1, \ldots, E_n$ des espaces fibrés vectoriels de classe $C^r$ et de base X, et soient $k, k_1, \ldots, k_n$ des entiers appartenant à $[0, r]$. Posons
$$
L(k_1, \ldots, k_n) = \mathscr{L}(P^{k_1}(E_1) \otimes \cdots \otimes P^{k_n}(E_n); F).
$$

Si $k_i \leq k$ pour tout $i$, les projections $r^{k_i, k_i} : P^k(E_i) \to P^{k_i}(E_i)$ permettent d’identifier le fibré $L(k_1, \ldots, k_n)$ à un sous-fibré du fibré $L(k) = L(k, \ldots, k)$. Il existe un plus petit sous-fibré $M(k)$ de $L(k)$ contenant tous les sous-fibrés $L(k_1, \ldots, k_n)$, pour $k_1 + \cdots + k_n = k$. Une section $H$ de $M(k)$ est appelée un opérateur $n$-différentiel (ou multidifférentiel) de type $(E_1, \ldots, E_n) \to F$ et d’ordre $\leq k$. Si $s_i$ ($1 \leq i \leq n$) est une section de classe $C^m$ ($m \in \mathbf{N}_K, m \geq k$) de $E_i$ sur un ouvert $U$ de $X$, on définit $H_U(s_1, \ldots, s_n) = H(s_1, \ldots, s_n)$ comme l’image par $H$ de la section $j^k(s_1) \otimes \cdots \otimes j^k(s_n)$ du fibré
$$
P^k(E_1) \otimes \cdots \otimes P^k(E_n).
$$
C’est une section de $F|U$. Si $H$ est de classe $C^h$, cette section est de classe $C^p$ avec $p = \inf(m - k, h)$.

Lorsque $E_1, \ldots, E_n$ et $F$ sont égaux à $K_X$, on dit que $H$ est un opérateur $n$-différentiel (ou multidifférentiel) scalaire.

#### Exemple {#var-2-s14-n1-exa-1 .statement}

Soient $J$ un ensemble fini, $X$ un ouvert de $K^J$. Soit $H$ un opérateur $n$-différentiel scalaire d’ordre $\leq k$ sur $X$. Il existe une famille unique de fonctions scalaires
$$
c(\alpha(1), \ldots, \alpha(n))_{(\alpha(1), \ldots, \alpha(n)) \in \mathbf{N}^J}, \quad \sum_{i=1}^n |\alpha(i)| \leq k
$$
sur $X$ telles que
$$
H_X(f_1, \ldots, f_n) = \sum_{\alpha(1), \ldots, \alpha(n)} c(\alpha(1), \ldots, \alpha(n)) \Delta^{\alpha(1)}(f_1) \ldots \Delta^{\alpha(n)}(f_n)
$$
pour toute famille $(f_1, \ldots, f_n)$ de fonctions de classe $C^k$ sur $X$. Pour que $H$ soit de classe $C^h$, il faut et il suffit que les fonctions $c(\alpha(1), \ldots, \alpha(n))$ soient de classe $C^h$.

### 14.2. Symboles

14.2.1. Soit $k$ un entier positif $\leq r$. Considérons la suite exacte
$$
0 \to P_k(T(X); E) \xrightarrow{i'} P^k(E) \xrightarrow{j'} P^{k-1}(E) \to 0
$$
du n° 12.6.8, où l’on a posé $j = r^{k, k-1}$. En appliquant le foncteur vectoriel $M \mapsto \mathscr{L}(M; F)$ à cette suite, on obtient la suite exacte
$$
0 \to \mathscr{L}(P^{k-1}(E); F) \xrightarrow{j''} \mathscr{L}(P^k(E); F) \xrightarrow{\sigma_k} \mathscr{L}(P_k(T(X); E); F) \to 0
$$
que l’on peut écrire:
$$
0 \to D^{k-1}(E, F) \xrightarrow{j''} D^k(E, F) \xrightarrow{\sigma_k} S^k(E, F) \to 0
$$
en posant
$$
S^k(E, F) = \mathscr{L}(P_k(T(X); E); F).
$$
L’homomorphisme $j' = \mathscr{L}(j; \mathrm{Id}_F)$ est l’inclusion canonique de $D^{k-1}(E, F)$ dans $D^k(E, F)$; l’homomorphisme $\sigma_k$ est égal par définition à $\mathscr{L}(i; \mathrm{Id}_F)$. Si $D$ est un opérateur différentiel de type $E \to F$ et d’ordre $\leq k$, son image par $\sigma_k$ est une section $\sigma_k(D)$ de $S^k(E, F)$ que l’on appelle le $k$-symbole (ou simplement le symbole) de $D$; on a $\sigma_k(D) = 0$ si et seulement si $D$ est d’ordre $\leq k-1$. Si $D$ est de classe $C^h$, il en est de même de son symbole.

14.2.2 (« Identifications du fibré des symboles »). On peut écrire le fibré $S^k(E, F) = \mathscr{L}(P_k(T(X); E); F)$ de diverses manières. Tout d’abord, si $x \in X$, un élément de $P_k(T_x(X); E_x)$ s’identifie (13.1.2) à un élément de $\mathscr{L}(TS^k(T_x(X)); E_x)$. On obtient ainsi des identifications de fibrés vectoriels

$$
P_k(T(X); E) = \mathscr{L}(TS^k(T(X)); E) = (TS^k(T(X)))* \otimes E
$$

et, en appliquant le foncteur vectoriel $M \mapsto \mathscr{L}(M; F) = M^* \otimes F$, on obtient:

$$
S^k(E, F) = TS^k(T(X)) \otimes E^* \otimes F = TS^k(T(X)) \otimes \mathscr{L}(E; F).
$$

On peut encore transformer l’expression précédente. Si $M$ et $N$ sont deux fibrés vectoriels, notons $\mathrm{Sym}^k(M; N)$ le sous-fibré de $\mathscr{L}(M, \ldots, M; N)$ formé des applications $k$-linéaires symétriques. On a un isomorphisme canonique

$$
\mathrm{Sym}^k(M; N) \to \mathrm{Sym}^k(M; K_X) \otimes N;
$$

d’autre part, la dualité entre $\otimes^k M$ et $\otimes^k M^*$ identifie $\mathrm{Sym}^k(M; K_X)$ à $TS^k(M^*)$. On obtient ainsi une identification

$$
\mathrm{Sym}^k(M; N) = TS^k(M^*) \otimes N.
$$

En appliquant cette formule à $M = T(X)^*$ et $N = \mathscr{L}(E; F)$, on a:

$$
S^k(E, F) = TS^k(T(X)) \otimes \mathscr{L}(E; F) = \mathrm{Sym}^k(T(X)^*; \mathscr{L}(E; F)).
$$

Supposons $K$ de caractéristique 0 ou $> k$. Si $u$ est une application $k$-linéaire symétrique, notons $\tilde{u}$ l’application polynomiale

$$
x \mapsto \frac{1}{k!} u(x, \ldots, x)
$$

correspondante. L’application $u \mapsto \tilde{u}$ définit un isomorphisme

$$
S^k(E, F) = \mathrm{Sym}^k(T(X)^*, \mathscr{L}(E; F)) \to P_k(T(X)^*; \mathscr{L}(E; F)).
$$

Ainsi, tout élément $\sigma$ de $S^k(E, F)_x$, avec $x \in X$, peut être identifié à une application polynomiale homogène $\tilde{\sigma}$ de degré $k$ de $T_x(X)^*$ dans $\mathscr{L}(E_x; F_x)$.

14.2.3 (« Calcul du symbole d’un opérateur différentiel »). Soit $x \in X$ et soit $D$ un opérateur différentiel de type $E \to F$, d’ordre $\leq k$, défini dans un voisinage ouvert de $x$ et de classe $C^{r-k}$. On va expliciter la valeur $\sigma_k(D)(x)$ du symbole de $D$ en $x$. Considérons-le comme élément de $\mathrm{Sym}^k(T_x(X)^*; \mathscr{L}(E_x; F_x))$ (cf. 14.2.2). Soient $\omega_1, \ldots, \omega_k$ des covecteurs en $x$ et choisissons des fonctions $f_1, \ldots, f_k$ de classe $C^r$ dans un voisinage ouvert $U$ de $x$ telles que $d_x f_i = \omega_i$ pour $i = 1, \ldots, k$. Posons

$$
D' = (-1)^k \mathrm{ad}\,(f_k) \ldots \mathrm{ad}(f_1)D \quad (\text{cf. } 14.1.10, a).
$$

L’opérateur $D'$ est d’ordre $\leq 0$; c’est une section de $\mathscr{L}(E; F)|U$. La valeur de $D'$ en $x$ est un élément $\lambda(\omega_1, \ldots, \omega_k)$ de $\mathscr{L}(E_x; F_x)$ qui ne dépend que de $(\omega_1, \ldots, \omega_k)$. L’application $\lambda$ ainsi définie est symétrique. *Elle est égale au symbole $\sigma_k(D)(x)$ de $D$ en $x$*.

Supposons $K = \mathbf{R}$ ou $\mathbf{C}$, et explicitons $\sigma_k(D)(x)$ considéré comme application polynomiale homogène de degré $k$ de $T_x(X)^*$ dans $\mathscr{L}(E_x; F_x)$ (cf. 14.2.2). Soient $\omega \in T_x(X)^*$ et $v \in E_x$; choisissons une fonction $f$ de classe $C^r$ dans un voisinage ouvert U de x telle que $d_x f = \omega$, et une section s de classe $C^r$ de E dans U telle que $s(x) = v$. Il existe une famille $(\varphi_0, \varphi_1, \ldots, \varphi_k)$ de sections de F dans U et une seule telle que
$$
e^{-tf} D(e^{tf}s) = \sum_{j=0}^k t^j \varphi_j \quad \text{pour tout } t \in K.
$$
Alors, $\varphi_k(x)$ ne dépend pas du choix de f et s telles que $d_x f = \omega, v(x) = s$; l’application $v \mapsto \varphi_k(x)$ est un élément $\lambda(\omega)$ de $\mathscr{L}(E_x; F_x)$, et $\lambda$ est une application polynomiale homogène de degré k de $T_x(X)^*$ dans $\mathscr{L}(E_x; F_x)$. *Cette application est égale au symbole $\sigma_k(D)(x)$ de D en x.*

14.2.4 (« Le cas scalaire »). Prenons $E = F = K_X$, auquel cas on identifie $D^k(E, F)$ au fibré $T^{(k)}(X)$ des distributions ponctuelles d’ordre $\leq k$, cf. 14.1.6. On a
$$
S^k(E, F) = TS^k(T(X))
$$
et le symbole
$$
\sigma_k : T^{(k)}(X) \to TS^k(T(X))
$$
n’est autre que le composé
$$
T^{(k)}(X) \to T^{(k)}(X)/T^{(k-1)}(X) \xrightarrow{i_k} TS^k(T(X)),
$$
où $i_k$ est l’isomorphisme défini en 13.3.2.

Prenons par exemple pour X un ouvert de $K^n$, et soit $\{e_1, \ldots, e_n\}$ la base canonique de $K^n$ (identifié aux espaces tangents $T_x(X)$). Si $\alpha \in \mathbf{N}^n$ est tel que $|\alpha| \leq k$, le symbole de l’opérateur $\Delta^\alpha$ est donné par les formules (cf. 13.3.3):
$$
\begin{aligned}
\sigma_k(\Delta^\alpha)(x) &= 0 & \text{si } |\alpha| < k \\
\sigma_k(\Delta^\alpha)(x) &= \gamma_{\alpha_1}(e_1) \cdots \gamma_{\alpha_n}(e_n) & \text{si } |\alpha| = k,
\end{aligned}
$$
le produit des $\gamma_{\alpha_i}(e_i)$ étant le *produit symétrique*, cf. 13.2.6 et 13.3.3.

14.2.5 (« Symbole d’un composé »). Les notations et hypothèses sont celles de 14.1.8. La composition des applications linéaires définit un accouplement
$$
\mathscr{L}(F; G) \times \mathscr{L}(E; F) \to \mathscr{L}(E; G).
$$
D’autre part, l’opération de *produit symétrique* définit un accouplement
$$
TS^{k''}(T(X)) \times TS^{k'}(T(X)) \to TS^k(T(X)).
$$
Comme on a
$$
\begin{aligned}
S^{k''}(F, G) &= TS^{k''}(T(X)) \otimes \mathscr{L}(F; G) \\
S^{k'}(E, F) &= TS^{k'}(T(X)) \otimes \mathscr{L}(E; F) \\
S^k(E, G) &= TS^k(T(X)) \otimes \mathscr{L}(E; G)
\end{aligned}
$$
cf. 14.2.2,
on déduit de là, par produit tensoriel, un accouplement
(*) $$
S^{k''}(F, G) \times S^{k'}(E, F) \to S^k(E, G).
$$
On a alors la formule
$$
\sigma_k(D'' \circ D') = \sigma_{k''}(D'') \cdot \sigma_{k'}(D'),
$$

où le produit figurant dans le terme de droite est défini par l’accouplement (*) ci-dessus.

Supposons maintenant K de caractéristique zéro, et soit $x \in X$. Notons $\sigma$ (resp. $\sigma', \sigma''$) le k-symbole (resp. le $k'$-symbole, le $k''$-symbole) de $D'' \circ D'$ (resp. $D', D''$) en $x$. Pour tout $\omega \in T_x(X)^*$, on a alors (avec les notations de la fin de 14.2.2):

$$
\tilde{\sigma}(\omega) \in \mathscr{L}(E_x; G_x), \quad \tilde{\sigma}'(\omega) \in \mathscr{L}(E_x; F_x), \quad \tilde{\sigma}''(\omega) \in \mathscr{L}(F_x; G_x)
$$

et

$$
\tilde{\sigma}(\omega) = \tilde{\sigma}''(\omega) \circ \tilde{\sigma}'(\omega).
$$

**14.3. Transposition**

Dans ce n°, on suppose que X est pure de dimension $n$.

### 14.3. Transposition

14.3.1. Soit $\Omega = \det(T(X)^*)$, cf. 7.9.9 ; c’est un fibré vectoriel de rang 1 en chaque point, de base X, et de classe $C^{r-1}$. On a

$$
\Omega = \wedge^n T(X)^* = \mathrm{Alt}^n(T(X); K_X).
$$

Soit M un fibré vectoriel de base X. On pose

$$
\tilde{M} = \mathscr{L}(M; \Omega) = M^* \otimes \Omega.
$$

[^1]

Si M est de classe $C^n$, avec $h \in N_K \cup \{0\}$ et $h \leq r - 1$, il en est de même de $\tilde{M}$. L’application canonique de M dans $\tilde{M} = \mathscr{L}(\mathscr{L}(M; \Omega); \Omega)$ est un isomorphisme ; on l’utilise pour identifier M à $\tilde{M}$.

14.3.2 (« Définition du transposé »). Soit $k$ un entier positif $\leq r - 1$, et soit D un opérateur différentiel sur X, de type $E \to F$, d’ordre $\leq k$, et de classe $C^n$, avec $h \in N_K \cup \{0\}$ et $k \leq h \leq r - k$. Il existe alors un opérateur différentiel $^tD$ sur X, de type $\bar{F} \to \bar{E}$ et d’ordre $\leq k$, jouissant de la propriété suivante :

Soit $\xi = (\xi^1, \ldots, \xi^n)$ un système de coordonnées dans un ouvert U de X et soit $s = (s_i)_{1 \leq i \leq e}$ (resp. $t = (t_j)_{1 \leq j \leq f}$) un repère de E (resp. de F) sur U. Soit $(s_i^*)$ (resp. $(t_j^*)$) le repère de $E^*$ (resp. de $F^*$) tel que $\langle s_i, s_j^* \rangle = \delta_{ij}$ (resp. $\langle t_i, t_j^* \rangle = \delta_{ij}$), et soit $(\tilde{s}_i)$ (resp. $(\tilde{t}_j)$) le repère de $\bar{E}$ (resp. $\bar{F}$) sur U obtenu en formant le produit tensoriel de $(s_i^*)$ (resp. de $(t_j^*)$) avec le repère $\omega = d\xi^1 \wedge \cdots \wedge d\xi^n$ de $\Omega$. Soient $c_{\alpha}^{ij}$ ($1 \leq i \leq e$, $1 \leq j \leq f$, $|\alpha| \leq k$) les fonctions de classe $C^n$ sur U telles que l’on ait

$$
D \left( \sum_i f_i s_i \right) = \sum_{i,j,\alpha} c_{\alpha}^{ij} \Delta_{\xi}^{\alpha}(f_i) \cdot t_j
$$

quelles que soient les fonctions $f_i$ dans $C^{h+k}(U)$, cf. 14.1.4, (3'). On a alors

$$
{}^tD \left( \sum_j g_j \tilde{t}_j \right) = \sum_{i,j,\alpha} (-1)^{|\alpha|} \Delta_{\xi}^{\alpha}(c_{\alpha}^{ij} g_j) \tilde{s}_i
$$

quelles que soient les fonctions $g_j$ dans $C^{h+k}(U)$.

80
VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES § 14

La propriété précédente (qui doit être vérifiée quels que soient $\xi$, $s$ et $t$) détermine $^{t}D$ de façon unique.[^2] L'opérateur $^{t}D$ est appelé le transposé de $D$; il est de classe $C^{h-k}$. Si $h\geq 2k$, le transposé de $^{t}D$ est défini et égal à $D$ (compte tenu des identifications de $\widetilde{E}$ et $\widetilde{F}$ avec $E$ et $F$ respectivement).

L'application $D\mapsto{}^{t}D$ est $K$-linéaire. Si $k=0$, i.e. si $D$ est un morphisme de $E$ dans $F$, $^{t}D$ est le morphisme $\mathscr{L}(D;\operatorname{Id}_{\Omega})$ de $\widetilde{F}$ dans $\widetilde{E}$.

Le symbole de $^{t}D$ se déduit du symbole de $D$ au moyen de l'isomorphisme

$$
\operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(E;F)\longrightarrow \operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(\widetilde{F};\widetilde{E})
$$

qui est le produit tensoriel de l'automorphisme $(-1)^k$ de $\operatorname{TS}^{k}(T(X))$ et de l'isomorphisme $u\mapsto\mathscr{L}(u;\operatorname{Id}_{\Omega})$ de $\mathscr{L}(E;F)$ sur $\mathscr{L}(\widetilde{F};\widetilde{E})$.

### 14.3.3 («Transposé d'un composé»). Les notations et hypothèses étant celles de 14.1.8, supposons que $D'$ soit de classe $C^{h'}$ et $D''$ de classe $C^{h''}$ avec $h',h''$ dans $\mathbf{N}_K\cup\{0\}$, $h'\geq k'+2k''$ et $h''\geq k''+2k'$.

Alors les transposés de $D'$, $D''$ et $D''\circ D'$ sont définis, ainsi que le composé de $^{t}D'$ et $^{t}D''$, et l'on a

$$
^{t}(D''\circ D')={}^{t}D'\circ{}^{t}D''.
$$

En particulier, les hypothèses et notations étant celles de 14.3.2, et $f$ étant une fonction de classe $C^{h'}$ sur $X$ avec $2k\leq h'$, on a $^{t}(D\circ f)=f\circ{}^{t}D$.

#### Exemple {#var-2-s14-n3-exa-1 .statement}

Prenons pour $X$ un ouvert de $K^n$, notons $\xi^1,\ldots,\xi^n$ les fonctions coordonnées sur $X$ et identifions $\Omega$ à $K_X$ au moyen du repère $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$. Si $E=F=K_X$, on a

$$
\widetilde{E}=\widetilde{F}=\mathscr{L}(K_X;\Omega)=\mathscr{L}(K_X;K_X)=K_X,
$$

et l'opération $D\mapsto{}^{t}D$ transforme opérateurs différentiels scalaires en opérateurs différentiels scalaires. On a, par exemple

$$
{}^{t}(\Delta^\alpha)=(-1)^{|\alpha|}\Delta^\alpha\qquad\text{pour tout }\alpha\in\mathbf{N}^n.
$$

Si $r$ est infini, la transposition est un anti-automorphisme de l'algèbre $\mathscr{D}^{\infty}_{K_X}(K_X,K_X)$.

### 14.3.4. Soit $k$ un entier positif tel que $K$ soit de caractéristique $0$ ou $>k$. Soit $\Omega_1$ le fibré vectoriel $\bigwedge^{n-1}T(X)^*=\mathscr{L}(T(X);K_X)$. Les notations et hypothèses étant celles de 14.3.2, soit en outre $D'$ un opérateur différentiel sur $X$, de $\widetilde{F}\rightarrow\widetilde{E}$, d'ordre $\leq k$; on appelle opérateur de Green pour $(D,D')$ tout opérateur multidifférentiel $G$ (cf. 14.1.11) de type $(E,\widetilde{F})\rightarrow\Omega_1$, d'ordre $\leq k-1$[^3] et de classe $C^h$ (avec $h\geq1$), tel que l'on ait l'identité

(1)

$$
\langle D(u),v\rangle-\langle u,D'(v)\rangle=d(G(u,v))
$$

quels que soient l'ouvert $U$ de $X$ et les éléments $u\in\mathscr{S}^k_E(U)$, $v\in\mathscr{S}^k_F(U)$. Précisons que, dans cette formule, $d$ désigne la différentiation extérieure (8.3.5) et $\langle D(u),v\rangle$ (resp.

$\langle u, D'(v) \rangle$) désigne la section de $\Omega$ sur $U$ obtenue à partir du couple $(D(u), v)$ (resp. du couple $(u, D'(v))$) par l’accouplement canonique de $F \times \tilde{F}$ (resp. de $E \times \tilde{E}$) dans $\Omega$. L’existence de $G$ implique $D' = {}^tD$; on dit aussi que $G$ est un opérateur de Green pour $D$.

14.3.5. Soit $D$ un opérateur différentiel sur $X$, de type $E \to F$, d’ordre $\leq k$, de classe $C^h$ avec $h \in N_K$ et $k \leq h \leq r - k$. Il existe un opérateur de Green de classe $C^{h-k+1}$ pour $D$ dans chacun des cas suivants:

a) $K = \mathbf{R}$, $r = \infty$ et $X$ est paracompacte.
b) $K$ est de caractéristique $0$ ou $> k$, $X$ est isomorphe à un ouvert d’un espace $K^n$, et les fibrés $E$ et $F$ sont isomorphes à des fibrés triviaux.
c) L’opérateur $D$ est d’ordre $\leq 1$ (cf. 14.3.7).

14.3.6. On conserve les hypothèses et notations de 14.3.3. Si $G'$ (resp. $G''$) est un opérateur de Green pour $D'$ (resp. $D''$), il existe un opérateur de Green $H$ pour $D'' \circ D'$ et un seul tel que l’on ait

$$
H(u, v) = G''(D'(u), v) + G'(u, {}^tD''(v))
$$

quels que soient l’ouvert $U$ de $X$ et les éléments $u \in \mathscr{S}_E^k(U)$ et $v \in \mathscr{S}_{\tilde{G}}^k(U)$.

14.3.7. On a $S^1(E, F) = T(X) \otimes E^* \otimes F$ (cf. 14.2.2). D’autre part, le produit intérieur droit $(\xi, \omega) \mapsto i(\xi)\omega$ (cf. A, III, p. 158) définit un isomorphisme de $T(X) \otimes \Omega$ sur $\Omega_1$; par produit tensoriel avec le dual $\Omega^*$ de $\Omega$, on obtient ainsi un isomorphisme de $T(X)$ sur $\Omega^* \otimes \Omega_1$, d’où des identifications de fibrés vectoriels

$$
\begin{align*}
S^1(E, F) &= \Omega^* \otimes \Omega_1 \otimes E^* \otimes F = (E \otimes F^* \otimes \Omega)^* \otimes \Omega_1 \\
&= (E \otimes \tilde{F})^* \otimes \Omega_1 = \mathscr{L}(E \otimes \tilde{F}; \Omega_1).
\end{align*}
$$

Cela posé, soit $D$ un opérateur différentiel sur $X$, de type $E \to F$, d’ordre $\leq 1$, de classe $C^h$ avec $h \in N_K \cup \{0\}$ et $h \leq r - 1$. Il existe un unique opérateur de Green pour $D$; il est d’ordre $0$; c’est un morphisme de classe $C^h$ de $E \otimes \tilde{F}$ dans $\Omega_1$, et il se déduit du symbole de $D$ par l’identification précédente.

14.3.8. Supposons que l’on ait $K = \mathbf{R}$, que $X$ soit séparée et orientée (10.2.4) et soit $A$ une pièce fermée (11.1.2) de $X$. Munissons $A$ de l’orientation induite par celle de $X$, et $\partial A$ de l’orientation correspondante (11.2.1). Soient $k$ un entier tel que $2k \leq r$, $D$ un opérateur différentiel sur $X$, de type $E \to F$, d’ordre $\leq k$ et de classe $C^k$. Soit $G$ un opérateur de Green pour $D$. Soient $U$ un ouvert de $X$, $u \in \mathscr{S}_E^k(U)$, $v \in \mathscr{S}_{\tilde{F}}^k(U)$ et supposons que les supports de $u$ et de $v$ rencontrent $A$ suivant un compact. On a alors

$$
\int_A \langle D(u), v \rangle - \int_A \langle u, {}^tD(v) \rangle = \int_{\partial A} G(u, v)
$$

(*formule de Green*). En particulier, si $\partial A = \varnothing$, on a

$$
\int_A \langle D(u), v \rangle = \int_A \langle u, {}^tD(v) \rangle.
$$

### 14.4. Exemples

On suppose X pure de dimension finie n. On la suppose aussi munie d'une structure de variété de classe C^{r+1} compatible avec la structure de classe C^r donnée.

14.4.1 (« Transformations infinitésimales »). Soit $\tau$ un foncteur vectoriel en dimension finie pour les isomorphismes, de classe C^r ; on suppose que, pour tout espace vectoriel V de dimension finie, $\tau(V)$ est de dimension finie. On note E_{\tau} le fibré vectoriel $\tau(T(X))$; il est de classe C^r.

Soit $\xi$ un champ de vecteurs de classe C^r sur X. Il existe un opérateur différentiel D de type $E_{\tau} \to E_{\tau}$ et d'ordre $\leq 1$ tel que

$$
D_U(s) = \theta_{\xi}.s
$$

pour tout ouvert U de X et tout $s \in \mathscr{S}_{E_{\tau}}(U)$, cf. 8.4.3. Un tel opérateur D est unique; on le note $(\theta_{\xi})_{\tau}$ ou simplement $\theta_{\xi}$. Son symbole est la section $\xi \otimes \mathrm{Id}_{E_{\tau}}$ du fibré vectoriel

$$
S^1(E_{\tau}, E_{\tau}) = T(X) \otimes \mathscr{L}(E_{\tau}; E_{\tau}).
$$

Si V est un K-espace vectoriel de dimension finie, posons

$$
\tilde{\tau}(V) = \mathscr{L}(\tau(V); \mathrm{Alt}^n(V; K)) = \tau(V)^* \otimes \wedge^n V^*,
$$

et si $u : V_1 \to V_2$ est un isomorphisme, définissons $\tilde{\tau}(u) : \tilde{\tau}(V_1) \to \tilde{\tau}(V_2)$ par transport de structure. On obtient ainsi un foncteur vectoriel en dimension finie $\tilde{\tau}$. Le fibré $E_{\tilde{\tau}} = \tilde{\tau}(T(X))$ s'identifie de manière évidente au fibré $(E_{\tau})^*$; le transposé de $(\theta_{\xi})_{\tau}$ est $-(\theta_{\xi})_{\tilde{\tau}}$ et la formule (1) du n° 14.3.4 prend la forme

$$
\langle \theta_{\xi}.u, v \rangle + \langle u, \theta_{\xi}.v \rangle = d(i(\xi)(u.v)).
$$

14.4.2 (« Différentielle extérieure »). Pour tout entier $p \geq 0$ on pose

$$
\Omega^p = \mathrm{Alt}^p(T(X); K_X).
$$

Il existe un opérateur différentiel D de type $\Omega^p \to \Omega^{p+1}$ et d'ordre $\leq 1$ tel que

$$
D_U(\omega) = d\omega
$$

pour tout ouvert U de X et tout $\omega \in \mathscr{S}_{\Omega^p}(U)$. Un tel opérateur D est unique; on le note d (ou $d_p$ si l'on tient à préciser l'entier p).

Son symbole est l'élément de $S^1(\Omega^p, \Omega^{p+1})$ obtenu de la manière suivante: on a tout d'abord

$$
S^1(\Omega^p, \Omega^{p+1}) = T(X) \otimes \mathscr{L}(\Omega^p; \Omega^{p+1})
$$
$$
= \mathscr{L}(\Omega^1; \mathscr{L}(\Omega^p; \Omega^{p+1})) = \mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1}),
$$

où $\mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1})$ désigne le fibré des applications bilinéaires de $\Omega^1 \times \Omega^p$ dans $\Omega^{p+1}$. Or le produit extérieur $(\alpha, \beta) \mapsto \alpha \wedge \beta$ définit une section canonique de ce dernier fibré; cette section est le symbole de $d_p$.

Pour déterminer le transposé de $d_p$, on remarque d'abord que le produit extérieur définit un accouplement $\Omega^p \times \Omega^{n-p} \to \Omega^n = \Omega$ qui permet d'identifier $(\Omega^p)^*$ à $\Omega^{n-p}$. On identifie de la même manière $(\Omega^{p+1})^*$ à $\Omega^{n-p-1}$. Avec ces conventions, le transposé de $d_p$ est $(-1)^{p+1} d_{n-p-1}$ et l'opérateur de Green correspondant, de type

$(\Omega^p,\Omega^{n-p-1})\longrightarrow\Omega_1=\Omega^{n-1}$, est simplement le produit extérieur (sur chaque fibre).

### 14.4.3 (« Laplacien »).

On prend $K=\mathbf{R}$, $r=\infty$, $X=\mathbf{R}^n$, $E=F=K_X$; on note $\xi^i$ $(1\leq i\leq n)$ les fonctions coordonnées sur $X$; on pose $D_i=\partial/\partial\xi^i$, et $L=\sum_{i=1}^n D_i^2$. L'opérateur $L$ est un opérateur différentiel scalaire d'ordre $\leq 2$. Si l'on identifie $\Omega$ à $K_X$ grâce au repère $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$, on a $\tilde E=\tilde F=K_X$ (cf. 14.3.3, exemple) et $\tilde L=L$.

Pour $1\leq i\leq n$, posons $\omega_i=(-1)^{i-1}d\xi^1\wedge\cdots\wedge d\xi^{i-1}\wedge d\xi^{i+1}\wedge\cdots\wedge d\xi^n$. Les $\omega_i$ forment un repère de $\Omega_1=\Omega^{n-1}$. Si $f\in\mathscr C^1(X)$, notons $\operatorname{grad}(f)$ la section $\sum_{i=1}^n D_i(f)\omega_i$ de $\Omega_1$. Il existe un opérateur de Green $G$ pour $L$ tel que l'on ait

$$G(u,v)=v.\operatorname{grad}(u)-u.\operatorname{grad}(v)$$

pour tout ouvert $U$ de $X$ et $u,v$ dans $\mathscr C^1(U)$.

En particulier, soit $A$ une pièce compacte de $\mathbf{R}^n$. Orientons $\mathbf{R}^n$, munissons $A$ de l'orientation induite par celle de $\mathbf{R}^n$ et $\partial A$ de l'orientation correspondante (11.2.1). On a

$$\int_A(Lu).v\omega-\int_Au.(Lv)\omega=\int_{\partial A}(v.\operatorname{grad}(u)-u.\operatorname{grad}(v))$$

pour $u,v$ dans $\mathscr C^1(X)$.

[^1]: On aura soin de ne pas confondre $\tilde{M}$ avec le revêtement de M défini en 10.2.4 et noté de la même manière.
[^2]: En fait, il suffit de vérifier la propriété en question pour des triplets $(\xi^\lambda,s^\lambda,t^\lambda)$ tels que les domaines des $\xi^\lambda$ recouvrent $X$.
[^3]: Lorsque $k=0$, on convient que cela signifie que $G=0$.
