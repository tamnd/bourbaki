---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 6
section_title: Intégration dans les groupes de Lie compacts
lang: fr
source: lie-ix-fr
book_pages: LIE IX.52-LIE IX.65, LIE IX.121-LIE IX.125
pdf_pages: 0055-0068, 0124-0128
extraction: ocr
subsections:
    - "no": 1
      title: Produit de formes multilinéaires alternées
      page: 52
      pdf_page: 55
    - "no": 2
      title: La formule d’intégration de H. Weyl
      page: 53
      pdf_page: 56
    - "no": 3
      title: Intégration dans l’algèbre de Lie
      page: 58
      pdf_page: 61
    - "no": 4
      title: Intégration des sections d’un fibré vectoriel
      page: 60
      pdf_page: 63
    - "no": 5
      title: Formes différentielles invariantes
      page: 63
      pdf_page: 66
statements: 22
exercises: 13
content_sha256: 3ef3ff31a3b4ef0d382045164ef8504751835e3acd8e474862e866a76dedad0c
---

## § 6. INTÉGRATION DANS LES GROUPES DE LIE COMPACTS

On conserve les notations du § 4 ; on pose $w(G) = \mathrm{Card}\left(W_G(T)\right)$. On note $dg$ (resp. $dt$) la mesure de Haar sur $G$ (resp. $T$) de masse totale 1, et $n$ (resp. $r$) la dimension de $G$ (resp. $T$).

### 1. Produit de formes multilinéaires alternées

Soient $A$ un anneau commutatif et $M$ un $A$-module. Pour chaque entier $r \geqslant 0$, notons $\mathrm{Alt}^r(M)$ le $A$-module des formes $r$-linéaires alternées sur $M$; il s’identifie au dual du $A$-module $\Lambda^r(M)$ (A, III, p. 80, prop. 7). Soient $u \in \mathrm{Alt}^s(M)$ et $v \in \mathrm{Alt}^r(M)$; rappelons (A, III, p. 142, exemple 3) qu’on appelle produit alterné de $u$ et $v$ l’élément $u \wedge v$ de $\mathrm{Alt}^{s+r}(M)$ défini par

$$
(u \wedge v)(x_1, ..., x_{s+r}) = \sum_{\sigma \in S_{s,r}} \varepsilon_\sigma u(x_{\sigma(1)}, ..., x_{\sigma(s)})\ v(x_{\sigma(s+1)}, ..., x_{\sigma(s+r)}) ,
$$

où $S_{s,r}$ est le sous-ensemble du groupe symétrique $S_{s+r}$ formé des permutations dont les restrictions à $\{1, s\}$ et $\{s+1, s+r\}$ sont croissantes.

Soit maintenant

$$
0 \longrightarrow M' \overset{i}{\longrightarrow} M \overset{p}{\longrightarrow} M'' \longrightarrow 0
$$

une suite exacte de $A$-modules libres, de rangs respectifs $r, r+s$ et $s$.

#### Lemme 1 {#lie-ix-s6-lem-1 .statement tag=01EX}

Il existe une application $A$-bilinéaire de $\mathrm{Alt}^s(M'') \times \mathrm{Alt}^r(M')$ dans $\mathrm{Alt}^{s+r}(M)$, notée $(u, v) \mapsto u \cap v$, et caractérisée par l’une quelconque des deux propriétés suivantes :

a) Notons $u_1 \in \mathrm{Alt}^s(M)$ la forme $(x_1, ..., x_s) \mapsto u(p(x_1), ..., p(x_s))$, et soit $v_1 \in \mathrm{Alt}^r(M)$ une forme telle que $v_1(i(x'_1), ..., i(x'_r)) = v(x'_1, ..., x'_r)$ pour $x'_1, ..., x'_r$ dans $M'$; on a alors $u \cap v = u_1 \wedge v_1$.

b) Pour $x_1, ..., x_s$ dans $M$ et $x'_1, ..., x'_r$ dans $M'$, on a

$$
(u \cap v)(x_1, ..., x_s, i(x'_1), ..., i(x'_r)) = u(p(x_1), ..., p(x_s))\ v(x'_1, ..., x'_r) .
$$

L’application $\varphi : \mathrm{Alt}^s(M'') \otimes_A \mathrm{Alt}^r(M') \to \mathrm{Alt}^{s+r}(M)$ telle que $\varphi(u \otimes v) = u \cap v$ est un isomorphisme de $A$-modules libres de rang un.

L’existence d’une forme $v_1$ satisfaisant à la condition a) résulte de ce que $\Lambda^r(i)$ induit un isomorphisme de $\Lambda^r(M')$ sur un sous-module facteur direct de $\Lambda^r(M)$ (A, III, p. 78). Soit $v_1$ une telle forme; posons $u \cap v = u_1 \wedge v_1$. La formule (1) est alors satisfaite, puisque si l’on pose $i(x'_k) = x_{s+k}$ pour $1 \leq k \leq r$, le seul élément $\sigma$ de $S_{s,r}$ tel que $p(x_{\sigma(i)}) \neq 0$ pour $1 \leq i \leq s$ est la permutation identique. D’autre part la formule (1) détermine $u \cap v$ de manière unique : soient en effet $(e'_1, ..., e'_r)$ une base de $M'$, $(f''_1, ..., f''_s)$ une base de $M''$, et $f_1, ..., f_s$ des éléments de $M$ tels que $p(f_i) = f''_i$ pour $1 \leq i \leq s$. Alors $(f_1, ..., f_s, i(e'_1), ..., i(e'_r))$ est une base de $M$ (A, II, p. 27, prop. 21), et la formule (1) s’écrit

(2)
$$
(u \cap v)(f_1, ..., f_s, i(e'_1), ..., i(e'_r)) = u(f''_1, ..., f''_s)\ v(e'_1, ..., e'_r) ;
$$

or un élément de $Alt^{s+r}(M)$ est déterminé par sa valeur sur une base.

Il résulte de ce qui précède que chacune des conditions a) ou b) détermine le produit $u \cap v$ de manière unique ; il est clair que ce produit est bilinéaire. Enfin la dernière assertion du lemme résulte de la formule (2).

### 2. La formule d’intégration de H. Weyl

Soient $e$ l’élément neutre de $G$ et $\overline{e}$ sa classe dans $G/T$. Identifions l’espace tangent à $G$ en $e$ à $g$, l’espace tangent à $T$ en $e$ à $t$ et l’espace tangent à $G/T$ en $\overline{e}$ à $g/t$. Notons $(u, v) \mapsto u \cap v$ l’application $\mathbf{R}$-bilinéaire

$$
Alt^{n-r}(g/t) \times Alt^r(t) \to Alt^n(g)
$$

définie au numéro 1.

Rappelons (III, § 3, no 13, prop. 50) que l’application $\omega \mapsto \omega(e)$ est un isomorphisme de l’espace vectoriel des formes différentielles de degré $n$ (resp. $r$) sur $G$ (resp. $T$), invariantes à gauche, sur l’espace $Alt^n(g)$ (resp. $Alt^r(t)$). Observons d’ailleurs que, puisqu’un sous-groupe compact connexe de $\mathbf{R}^*$ est réduit à l’élément neutre, on a $\det \operatorname{Ad}\ g = 1$ pour tout $g \in G$, de sorte que les formes différentielles de degré $n$ invariantes à gauche sur $G$ sont aussi invariantes à droite et invariantes par automorphismes intérieurs (III, § 3, no 16, cor. à la prop. 54) : nous parlerons simplement dans la suite de formes différentielles invariantes sur $G$.

De même, il résulte de III, § 3, no 16, prop. 56 et de ce qui précède que l’application $\omega \mapsto \omega(\overline{e})$ est un isomorphisme de l’espace des formes différentielles de degré $n - r$ sur $G/T$, invariantes par $G$, sur l’espace $Alt^{n-r}(g/t)$.

Si $\omega_{G/T}$ est une forme différentielle de degré $n - r$ sur $G/T$, invariante par $G$, et $\omega_T$ une forme différentielle invariante de degré $r$ sur $T$, on note $\omega_{G/T} \cap \omega_T$ l’unique forme différentielle invariante de degré $n$ sur $G$ telle que

$$
(\omega_{G/T} \cap \omega_T)(e) = \omega_{G/T}(\overline{e}) \cap \omega_T(e) .
$$

Rappelons enfin qu’on note $f : (G/T) \times T \to G$ le morphisme de variétés déduit par passage au quotient de l’application $(g, t) \mapsto gtg^{-1}$ de $G \times T$ dans $G$ (§ 5, no 4).

Si $\alpha$ et $\beta$ sont des formes différentielles sur $G/T$ et $T$ respectivement, on note simplement $\alpha \wedge \beta$ la forme $\mathrm{pr}_1^*\alpha \wedge \mathrm{pr}_2^*\beta$ sur $(G/T) \times T$.

Pour $t \in T$, notons $\mathrm{Ad}_{g/t}(t)$ l’endomorphisme de $g/t$ déduit de $\mathrm{Ad}\ t$ par passage aux quotients. Posons

$$
\delta_G(t) = \det(\mathrm{Ad}_{g/t}(t) - 1) = \prod_{\alpha \in R(G, T)} (t^\alpha - 1).
$$

Soient $x \in t$ et $\alpha \in R(G, T)$; notons $\hat{\alpha}$ l’élément $(2\pi i)^{-1} \delta(\alpha)$ de $t^*$, de sorte qu’on a

$$
((\exp x)^\alpha - 1)\ ((\exp x)^{-\alpha} - 1) = (e^{2\pi i \hat{\alpha}(x)} - 1)\ (e^{-2\pi i \hat{\alpha}(x)} - 1) = 4 \sin^2 \pi \hat{\alpha}(x).
$$

Si $R_+(G, T)$ désigne l’ensemble des racines positives de $R(G, T)$ relativement à une base $B$, on a

$$
\delta_G(\exp x) = \prod_{\alpha \in R_+(G, T)} 4 \sin^2 \pi \hat{\alpha}(x),
$$

d’où en particulier $\delta_G(t) > 0$ pour tout $t \in T_r$. Remarquons aussi qu’on a $\delta_G(t) = \delta_G(t^{-1})$ pour $t \in T$.

#### Proposition 1 {#lie-ix-s6-prop-1 .statement tag=01EY}

*Soient $\omega_G, \omega_{G/T}$ et $\omega_T$ des formes différentielles invariantes sur $G, G/T$ et $T$ respectivement, de degrés respectifs $n, n-r$ et $r$. Si $\omega_G = \omega_{G/T} \cap \omega_T$, alors*

$$
f^*(\omega_G) = \omega_{G/T} \wedge \delta_G \omega_T.
$$

On peut évidemment supposer que $\omega_{G/T}$ et $\omega_T$ sont non nulles ; alors la forme différentielle $(u, t) \mapsto \omega_{G/T}(u) \wedge \omega_T(t)$ sur $(G/T) \times T$ est de degré $n$ et partout non nulle ; il existe donc une fonction numérique $\delta$ sur $(G/T) \times T$ telle que

$$
f^*(\omega_G)(u, t) = \delta(u, t)\ \omega_{G/T}(u) \wedge \omega_T(t).
$$

Observons maintenant que, pour $h \in G, u \in G/T, t \in T$, on a $f(h.u, t) = (\mathrm{Int}\ h)\ f(u, t)$ ; comme $\omega_G$ est invariante par automorphismes intérieurs, il en résulte aussitôt que $\delta(hu, t) = \delta(u, t)$, donc $\delta(u, t) = \delta(\overline{e}, t)$.

Notons $p : g \to g/t$ l’application de passage au quotient et $\varphi : g/t \to g$ l’application définie par

$$
\varphi(p(X)) = (\mathrm{Ad}\ t^{-1}) X - X \quad \text{pour } X \in g;
$$

rappelons (§ 5, no 4, lemme 4) que l’application tangente

$$
T_{(e,t)}(f) : T_e(G/T) \times T_t(T) \to T_t(G)
$$

applique $(z, tH)$ sur $t(\varphi(z) + H)$ pour $z \in g/t,\ H \in t$.

Soient $z_1, ..., z_{n-r}$ des éléments de $g/t$, $H_1, ..., H_r$ des éléments de $t$. On a

$$
f^*\omega_G(\overline{e}, t)(z_1, ..., z_{n-r}, tH_1, ..., tH_r)
$$
$$
= \omega_G(t)(t\varphi(z_1), ..., t\varphi(z_{n-r}), tH_1, ..., tH_r) \quad \text{d'après le calcul de } T_{(\overline{e}, t)}(f)
$$
$$
= \omega_G(e)(\varphi(z_1), ..., \varphi(z_{n-r}), H_1, ..., H_r) \quad \text{puisque } \omega_G \text{ est invariante}
$$
$$
= \omega_{G/T}(\overline{e})(p\varphi(z_1), ..., p\varphi(z_{n-r})), \omega_T(e)(H_1, ..., H_r) \quad (\text{n}^o 1, \text{lemme 1})
$$
$$
= \det(p\varphi)\omega_{G/T}(\overline{e})(z_1, ..., z_{n-r}).\omega_T(e)(H_1, ..., H_r)
$$
$$
= \delta_G(t)\omega_{G/T}(\overline{e})(z_1, ..., z_{n-r}).\omega_T(t)(tH_1, ..., tH_r) \quad \text{puisque } \omega_T \text{ est invariante}
$$
$$
= \delta_G(t)(\omega_{G/T} \wedge \omega_T)(\overline{e}, t)(z_1, ..., z_{n-r}, tH_1, ..., tH_r),
$$

d'où $f^*\omega_G(\overline{e}, t) = \delta_G(t)(\omega_{G/T} \wedge \omega_T)(\overline{e}, t)$; on a donc $\delta(\overline{e}, t) = \delta_G(t)$, d'où la proposition.

Munissons les variétés $G, T$ et $G/T$ des orientations définies par les formes $\omega_G, \omega_T$ et $\omega_{G/T}$ respectivement. Ces formes définissent alors des mesures invariantes sur $G, T$ et $G/T$ (III, § 3, n° 16, prop. 55 et 56), encore notées $\omega_G, \omega_T$ et $\omega_{G/T}$.

#### Lemme 2 {#lie-ix-s6-lem-2 .statement tag=01EZ}

*Si $\omega_G = \omega_{G/T} \cap \omega_T$, alors*

$$
\int_G \omega_G = \int_{G/T} \omega_{G/T} \cdot \int_T \omega_T.
$$

Notons $\pi$ le morphisme canonique de $G$ dans $G/T$. Soit $g \in G$, et soient $t_1, ..., t_{n-r}$ des éléments de $T_{\pi(g)}(G/T)$. Identifions la fibre $\pi^{-1}(\pi(g)) = gT$ à $T$ par la translation $\gamma(g)$. La relation $\omega_G = \omega_{G/T} \cap \omega_T$ entraîne alors l'égalité (VAR, R, 11.4.5) :

$$
\omega_G|_{(t_1, ..., t_{n-r})} = (\omega_{G/T}(t_1, ..., t_{n-r})) \omega_T.
$$

On a donc $\int_\pi \omega_G = \left( \int_T \omega_T \right) \omega_{G/T}$ (VAR, R, 11.4.6), et

$$
\int_G \omega_G = \int_{G/T} \int_\pi \omega_G = \int_T \omega_T \cdot \int_{G/T} \omega_{G/T} \quad \text{(VAR, R, 11.4.8)}.
$$

#### Lemme 3 {#lie-ix-s6-lem-3 .statement tag=01F0}

*L'image réciproque sur $(G/T) \times T_r$ de la mesure $dg$ sur $G_r$ par l'homéomorphisme local $f_r$ (INT, V, § 6, n° 6) est la mesure $\mu \otimes \delta_G dt$, où $\mu$ est l'unique mesure $G$-invariante sur $G/T$ de masse totale 1.*

Choisissons une forme différentielle invariante $\omega_T$ (resp. $\omega_{G/T}$) sur $T$ (resp. $G/T$) de degré maximum, telle que la mesure définie par $\omega_T$ (resp. $\omega_{G/T}$) soit égale à $dt$ (resp. $\mu$). Posons $\omega_G = \omega_{G/T} \cap \omega_T$. Le lemme 2 entraîne que la mesure définie par $\omega_G$ est égale à $dg$. Soit $U$ une partie ouverte de $(G/T) \times T_r$, telle que $f_r$ induise un isomorphisme de $U$ sur une partie ouverte $V$ de $G_r$. Soit $\varphi$ une fonction continue à support compact dans V ; notons encore $\varphi$ le prolongement de $\varphi$ à $G_r$, qui s’annule en dehors de V. On a

$$
\int_V \varphi dg = \int_V \varphi \omega_G = \int_U (\varphi \circ f_r) f_r^*(\omega_G)
$$
$$
= \int_U (\varphi \circ f_r) \omega_{G/T} \wedge \delta_G \omega_T \quad \text{(prop. 1)}
$$
$$
= \int_U (\varphi \circ f_r) d\mu \cdot \delta_G dt ,
$$

d’où le lemme.

**Théorème 1** (H. Weyl). — *La mesure dg sur G est l’image par l’application* $(g, t) \mapsto gtg^{-1}$ *de* $G \times T$ *dans* $G$ *de la mesure* $dg \otimes \frac{1}{w(G)} \delta_G dt$, où
$$
\delta_G(t) = \det(\mathrm{Ad}_{g/t}(t) - 1) = \prod_{\alpha \in R(G, T)} (t^\alpha - 1) .
$$

Il revient au même (INT, V, § 6, n° 3, prop. 4) de dire que $dg$ est l’image par l’application $f : (G/T) \times T \to G$ de la mesure $\mu \otimes \frac{1}{w(G)} \delta_G dt$.

Démontrons cette dernière assertion. Il résulte du § 5, n° 1 et de VAR, R, 10.1.3, c) que $G - G_r$ est négligeable dans $G$ et $T - T_r$ négligeable dans $T$. Par ailleurs l’application $f_r$ fait de $(G/T) \times T_r$ un revêtement principal de $G_r$, de groupe $W$ (§ 5, n° 4, prop. 4, b)). Le théorème résulte alors du lemme 3 et de INT, V, § 6, n° 6, prop. 11.

#### Corollaire 1 {#lie-ix-s6-lem-3-cor-1 .statement}

(i) *Soit* $\varphi$ *une fonction intégrable sur* $G$ *à valeurs dans un espace de Banach ou dans* $\overline{\mathbf{R}}$. *Pour presque tout* $t \in T$, *la fonction* $g \mapsto \varphi(gtg^{-1})$ *sur* $G$ *est intégrable pour* $dg$. *La fonction* $t \mapsto \delta_G(t) \int_G \varphi(gtg^{-1}) dg$ *est intégrable sur* $T$, *et l’on a*
$$
\int_G \varphi(g) dg = \frac{1}{w(G)} \int_T \left( \int_G \varphi(gtg^{-1}) dg \right) \delta_G(t) dt
$$
(*formule d’intégration de Hermann Weyl*).

(ii) *Soit* $\varphi$ *une fonction mesurable positive sur* $G$. *Pour presque tout* $t \in T$, *la fonction* $g \mapsto \varphi(gtg^{-1})$ *sur* $G$ *est mesurable*. *La fonction* $t \mapsto \int_G^* \varphi(gtg^{-1}) dg$ *sur* $T$ *est mesurable*, *et l’on a*
$$
\int_G^* \varphi(g) dg = \frac{1}{w(G)} \int_T^* \left( \int_G^* \varphi(gtg^{-1}) dg \right) \delta_G(t) dt .
$$

Puisque l’application $f$ se déduit par passage au quotient de l’application $(g, t) \mapsto gtg^{-1}$ de $G \times T$ dans $G$, il suffit d’appliquer INT, V, § 5, 6, 8 et INT, VII, § 2.

#### Corollaire 2 {#lie-ix-s6-lem-3-cor-2 .statement}

*Soit $\varphi$ une fonction centrale sur $G$ (c’est-à-dire telle que $\varphi(gh) = \varphi(hg)$ pour tous $g$ et $h$ dans $G$) à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$.
a) *Pour que $\varphi$ soit mesurable, il faut et il suffit que sa restriction à $T$ soit mesurable.*
b) *Pour que $\varphi$ soit intégrable, il faut et il suffit que la fonction $(\varphi|T)$ $\delta_G(t)$ soit intégrable sur $T$ et l’on a alors*

$$
\int_G \varphi(g) \, dg = \frac{1}{w(G)} \int_T \varphi(t) \, \delta_G(t) \, dt .
$$

Notons $p : G/T \times T \to T$ la seconde projection. On a $\varphi \circ f = (\varphi|T) \circ p$; par ailleurs, l’image par $p$ de la mesure $\mu \otimes \frac{1}{w(G)} \delta_G dt$ est $\frac{1}{w(G)} \delta_G dt$. Le corollaire résulte alors du th. 1 ci-dessus et du th. 1 de INT, V, § 6, n° 2, appliqués aux deux applications propres $f$ et $p$.

#### Corollaire 3 {#lie-ix-s6-lem-3-cor-3 .statement}

*Soient $H$ un sous-groupe fermé connexe de $G$ contenant $T$, $h$ son algèbre de Lie, et $dh$ la mesure de Haar sur $H$ de masse totale 1. Soit $\varphi$ une fonction centrale intégrable sur $G$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Alors la fonction $h \mapsto \varphi(h) \det(\mathrm{Ad}_{g/h}(h) - 1)$ est intégrable et centrale sur $H$ et l’on a :

$$
\int_G \varphi(g) \, dg = \frac{w(H)}{w(G)} \int_H \varphi(h) \det(\mathrm{Ad}_{g/h}(h) - 1) \, dh .
$$

En effet, la fonction $h \mapsto \varphi(h) \det(\mathrm{Ad}_{g/h}(h) - 1)$ est une fonction centrale sur $H$, dont la restriction à $T$ est la fonction $t \mapsto \varphi(t) \delta_G(t) \delta_H(t)^{-1}$. Le corollaire résulte donc du cor. 2 appliqué à $G$ et à $H$.

#### Remarque 1 {#lie-ix-s6-n2-rem-1 .statement tag=01F5}

Si l’on prend $\varphi = 1$ dans le cor. 3, on obtient

$$
\int_H \det(\mathrm{Ad}_{g/h}(h) - 1) \, dh = w(G)/w(H)
$$

et en particulier

$$
\int_T \delta_G(t) \, dt = w(G) .
$$

#### Remarque 2 {#lie-ix-s6-n2-rem-2 .statement tag=01F6}

Soit $v$ la mesure sur l’espace quotient $T/W$ définie par

$$
\int_{T/W} \psi(\tau) \, dv(\tau) = \frac{1}{w(G)} \int_T \psi(\pi(t)) \delta_G(t) \, dt ,
$$

où $\pi$ désigne la projection canonique de $T$ sur $T/W$. Le cor. 2 signifie que l’homéomorphisme $T/W \to G/\mathrm{Int}(G)$ ($§ 2$, no 5, cor. 1 à la prop. 5) transporte la mesure $v$ en l’image de la mesure $dg$ par la projection canonique $G \to G/\mathrm{Int}(G)$.

#### Remarque 3 {#lie-ix-s6-n2-rem-3 .statement tag=01F7}

Supposons $G$ simplement connexe. Soient $A$ une alcôve de $t$, et $dx$ la mesure de Haar sur $t$ telle que $\int_{\overline{A}} dx = 1$. Alors la mesure $v$ s’obtient aussi en transportant par l’homéomorphisme $\overline{A} \to T/W$ ($§ 5$, no 2, cor. 1 à la prop. 2) la mesure $\frac{1}{w(G)} \prod_{\alpha \in R_+(G,T)} 4 \sin^2 \pi \hat{\alpha}(x) \, dx$ sur $\overline{A}$.

#### Exemple {#lie-ix-s6-n2-exa-1 .statement tag=01F8}

Prenons pour $G$ le groupe $SU(2, \mathbf{C})$ et pour $T$ le sous-groupe des matrices diagonales ($§ 3$, no 6); on identifie $t$ à $\mathbf{R}$ par le choix de la base $\{ iH \}$ de $t$ (*loc. cit.*). Posons $A = ]0, \pi[$; c’est une alcôve de $t$. L’intervalle $\overline{A} = [0, \pi]$ s’identifie à l’espace des classes de conjugaison de $G$, l’élément $\theta$ de $\overline{A}$ correspondant à la classe de conjugaison de $\begin{pmatrix} e^{i\theta} & 0 \\ 0 & e^{-i\theta} \end{pmatrix}$. Soit $d\theta$ la mesure de Lebesgue sur $[0, \pi]$; il résulte de ce qui précède que la mesure sur $\overline{A}$ image de la mesure de Haar de $G$ est la mesure $\frac{2}{\pi} \sin^2 \theta d\theta$.

### 3. Intégration dans l’algèbre de Lie

#### Proposition 2 {#lie-ix-s6-prop-2 .statement tag=01F9}

*Soient $H$ un groupe de Lie (réel) de dimension $m$, $\mathfrak{h}$ son algèbre de Lie. Soit $\omega_H$ une forme différentielle invariante à droite de degré $m$ sur $H$, et soit $\omega_{\mathfrak{h}}$ la forme différentielle invariante par translation sur $\mathfrak{h}$, de degré $m$, qui coïncide à l’origine avec $\omega_H(e)$. On a*
$$
(\exp_H)^* \omega_H = \lambda_{\mathfrak{h}} \omega_{\mathfrak{h}}
$$
*où $\lambda_{\mathfrak{h}}$ est la fonction sur $\mathfrak{h}$, invariante sous $\mathrm{Ad}(H)$, telle que*
$$
\lambda_{\mathfrak{h}}(x) = \det \left( \sum_{p \geq 0} \frac{1}{(p+1)!} (\mathrm{ad}\ x)^p \right) \quad \text{pour} \quad x \in \mathfrak{h}.
$$
Soient $x, x_1, ..., x_m$ des éléments de $\mathfrak{h}$. On a
$$
(\exp^* \omega_H)_x(x_1, ..., x_m) = (\omega_H(\exp x)) \left( T_x(\exp)(x_1), ..., T_x(\exp)(x_m) \right).
$$
Notons $\varpi(x): \mathfrak{h} \to \mathfrak{h}$ la différentielle droite de l’exponentielle en $x$ (III, § 3, no 17, déf. 8); on a donc par définition :
$$
T_x(\exp)(y) (\exp x)^{-1} = \varpi(x).y \quad \text{pour tout} \quad y \in \mathfrak{h}.
$$
La forme $\omega_H$ étant invariante à droite, on obtient :
$$
(\omega_H(\exp x)) \left( T_x(\exp)(x_1), ..., T_x(\exp)(x_m) \right) = \omega_H(e) \left( \varpi(x).x_1, ..., \varpi(x).x_m \right)
$$
$$
= (\det \varpi(x)) \omega_{\mathfrak{h}}(x_1, ..., x_m);
$$

on a donc $\exp^*\omega_H = \lambda_h \omega_h$, avec $\lambda_h(x) = \det \varpi(x) = \det \frac{\exp \operatorname{ad} x - 1}{\operatorname{ad} x}$ (III, § 6, n° 4, prop. 12).

Soit $h \in H$; puisque $\operatorname{Ad} h$ est un automorphisme de $\mathfrak{h}$, on a
$$
\operatorname{ad}((\operatorname{Ad} h)(x)) = \operatorname{Ad} h \circ \operatorname{Ad} x \circ (\operatorname{Ad} h)^{-1},
$$
d’où $\lambda_h((\operatorname{Ad} h)(x)) = \lambda_h(x)$. La fonction $\lambda_h$ est donc invariante sous $\operatorname{Ad}(H)$; ceci achève de prouver la proposition.

#### Remarque {#lie-ix-s6-n3-rem-1 .statement tag=01FA}

Considérons la fonction $\lambda_g$ associée au groupe de Lie compact $G$; en vertu du § 2, n° 1, th. 1, il suffit pour la calculer de connaître ses valeurs sur $t$. Or, pour tout $x \in t$, l’endomorphisme $\operatorname{ad} x$ de $g$ est semi-simple, et admet pour valeurs propres 0 (avec multiplicité $r$), et, pour tout $\alpha \in R(G, T)$, $\delta(\alpha)(x)$ (avec multiplicité 1). On en déduit aussitôt
$$
\lambda_g(x) = \prod_{\alpha \in R(G, T)} \frac{e^{\delta(\alpha)(x)} - 1}{\delta(\alpha)(x)} = \frac{\delta_g(x)}{\pi_g(x)}
$$
avec $\delta_g(x) = \delta_G(\exp x)$ et $\pi_g(x) = \prod_{\alpha \in R(G, T)} \delta(\alpha)(x) = \det \operatorname{ad}_{g/t}(x)$.

Soient $\omega_{G/T}$ une forme différentielle invariante de degré $n - r$ sur $G/T$ et $\omega_t$ une forme différentielle de degré $r$ sur $t$ invariante par translation. Avec les notations du n° 1, on note $\omega_{G/T} \cap \omega_t$ l’unique forme différentielle $\omega_g$ de degré $n$ sur $g$, invariante par translation, telle que $\omega_g(0) = \omega_{G/T}(\overline{e}) \cap \omega_t(0)$.

Enfin, on désigne par $\psi : (G/T) \times t \to g$ le morphisme de variétés déduit par passage au quotient de l’application $(g, x) \mapsto (\operatorname{Ad} g)(x)$ de $G \times t$ dans $g$.

#### Proposition 3 {#lie-ix-s6-prop-3 .statement tag=01FB}

Soient $\omega_g, \omega_t, \omega_{G/T}$ des formes différentielles invariantes sur $g, t, G/T$ respectivement, de degrés respectifs $n, r, n - r$. Si $\omega_g = \omega_{G/T} \cap \omega_t$, on a :
$$
\psi^*\omega_g = \omega_{G/T} \wedge \pi_g \omega_t
$$
où $\pi_g$ est la fonction sur $t$ définie par $\pi_g(x) = \prod_{\alpha \in R(G, T)} \delta(\alpha)(x)$.

Notons $\omega_G$ (resp. $\omega_T$) la forme différentielle invariante de degré maximum sur $G$ (resp. $T$) qui coïncide à l’origine avec $\omega_g$ (resp. $\omega_t$). Considérons le diagramme commutatif
$$
\begin{array}{ccc}
(G/T) \times t & \xrightarrow{\psi} & g \\
\downarrow (\operatorname{Id}, \exp_T) & & \downarrow \exp_G \\
(G/T) \times T & \xrightarrow{f} & G
\end{array}
$$

Compte tenu de la prop. 1 du n° 2 et de la relation $\exp_T^*\omega_T = \omega_t$, on en déduit l’égalité
$$
\psi^*\exp_G^*\omega_G = \omega_{G/T} \wedge \delta_g \omega_t.
$$

D’après la prop. 2, on a $\psi^*\exp_G^*\omega_G = (\psi^*\lambda_g)\,\psi^*\omega_g$. Comme la fonction $\lambda_g$ est invariante sous $\mathrm{Ad}(G)$, on a

$$
(\psi^*\lambda_g)(\overline{g}, x) = \lambda_g(x) = \frac{\delta_g(x)}{\pi_g(x)} \quad \text{pour} \quad \overline{g} \in G/T, \quad x \in t.
$$

Il en résulte que les formes $\psi^*\omega_G(\overline{g}, x)$ et $\omega_{G/T}(\overline{g}) \wedge \pi_g(x)\,\omega_t(x)$ coïncident lorsque $\delta_g(x)$ est non nul, c’est-à-dire sur l’ouvert dense $(G/T) \times t_r$; elles sont donc égales, d’où la proposition.

Choisissons des formes différentielles invariantes de degré maximum $\omega_G$ sur $G$ et $\omega_T$ sur $T$, telles que $|\omega_G| = dg$ et $|\omega_T| = dt$; notons $\omega_g$ (resp. $\omega_t$) la forme différentielle invariante par translation sur $g$ (resp. $t$) qui coïncide avec $\omega_G(e)$ (resp. $\omega_T(e)$) à l’origine, et $dz$ (resp. $dx$) la mesure de Haar $|\omega_g|$ (resp. $|\omega_t|$). En raisonnant comme dans le n° 2, mutatis mutandis, on établit la proposition suivante :

#### Proposition 4 {#lie-ix-s6-prop-4 .statement tag=01FC}

*La mesure $dz$ sur $g$ est l’image par l’application propre $(g, x) \mapsto (\mathrm{Ad}\,g)(x)$ de $G \times t$ dans $g$ de la mesure $dg \otimes \frac{1}{w(G)} \pi_g dx$.*

Nous laissons au lecteur le soin d’énoncer et démontrer les analogues des cor. 1 à 3 et des remarques 1 à 3 du n° 2. Par exemple, soit $\varphi$ une fonction intégrable sur $g$ (à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$); on a

$$
\int_g \varphi(z)\,dz = \frac{1}{w(G)} \int_t \left( \int_G \varphi((\mathrm{Ad}\,g)\,x)\,dg \right) \pi_g(x)\,dx,
$$

et en particulier, si $\varphi$ est invariante sous $\mathrm{Ad}(G)$,

$$
\int_g \varphi(z)\,dz = \frac{1}{w(G)} \int_t \varphi(x)\,\pi_g(x)\,dx.
$$

### 4. Intégration des sections d’un fibré vectoriel

Dans ce numéro et le suivant, on désigne par $X$ une variété réelle de classe $C^r$ ($1 \leq r \leq \infty$), localement de dimension finie.

Soit $Y$ une variété de classe $C^r$. Si $r < \infty$, considérons l’application $f \mapsto j^r(f)$ de $\mathcal{C}^r(X; Y)$ dans $\mathcal{C}(X; J^r(X, Y))$ (VAR, R, 12.3.7). L’image réciproque par cette application de la topologie de la convergence compacte sur $\mathcal{C}(X; J^r(X, Y))$ est appelée *topologie de la $C^r$-convergence compacte* sur $\mathcal{C}^r(X; Y)$; c’est la borne supérieure des topologies de la $C^r$-convergence uniforme sur $K$ (VAR, R, 12.3.10), lorsque $K$ décrit l’ensemble des parties compactes de $X$.

Lorsque $r = \infty$, on appelle *topologie de la $C^\infty$-convergence compacte* sur $\mathcal{C}^\infty(X; Y)$ la borne supérieure des topologies de la $C^k$-convergence compacte, autrement dit la topologie la moins fine qui rende continues les injections canoniques $\mathcal{C}^\infty(X; Y) \to \mathcal{C}^k(X; Y)$, pour $0 \leq k < \infty$.

Soit E un fibré vectoriel réel de base X, de classe $C^r$, et soit $\mathcal{S}^r(X;E)$ l’espace vectoriel des sections de classe $C^r$ de E. On munira dans ce numéro $\mathcal{S}^r(X;E)$ de la topologie induite par la topologie de la $C^r$-convergence compacte sur $C^r(X;E)$, encore appelée topologie de la $C^r$-convergence compacte ; elle fait de $\mathcal{S}^r(X;E)$ un espace vectoriel topologique localement convexe séparé complet (cf. VAR, R, 15.3.1 et TS, à paraître).

Soient maintenant H un groupe de Lie, $m : H \times X \to X$ une loi d’opération à gauche de classe $C^r$; on pose $hx = m(h, x)$ pour $h \in H,\ x \in X$. Soit E un H-fibré vectoriel de base X, de classe $C^r$ (III, § 1, no 8, déf. 4). Pour $s \in \mathcal{S}^r(X;E)$ et $h \in H$, notons $^h s$ la section $x \mapsto h.s(h^{-1}x)$ de E ; l’application $(h, s) \mapsto ^h s$ est une loi d’opération de H dans l’espace $\mathcal{S}^r(X;E)$.

#### Lemme 4 {#lie-ix-s6-lem-4 .statement tag=01FD}

*La loi d’opération* $H \times \mathcal{S}^r(X;E) \to \mathcal{S}^r(X;E)$ *est continue*.

Compte tenu de la définition de la topologie de $\mathcal{S}^r(X;E)$ et de TG, X, p. 28, th. 3, il suffit de démontrer que pour tout entier $k \leq r$, l’application $f : H \times X \times \mathcal{S}^k(X;E) \to J^k(X;E)$ telle que $f(h, x, s) = j_x^k(^h s)$ est continue. Pour $h \in H$, notons $\tau_h$ (resp. $\theta_h$) l’automorphisme $x \mapsto hx$ de X (resp. de E). Définissons des applications
$$
f_1 : H \times X \to J^k(X, X) \\
f_2 : H \times E \to J^k(E, E) \\
g : H \times X \times \mathcal{S}^k(X;E) \to J^k(X, E)
$$
par $f_1(h, x) = j_x^k(\tau_h),\ f_2(h, v) = j_v^k(\theta_h),\ g(h, x, s) = j_{hx}^k(s)$. On a
$$
f(h, x, s) = f_2(h, s(h^{-1}x)) \circ g(h^{-1}, x, s) \circ f_1(h^{-1}, x),
$$
et il suffit par conséquent, d’après VAR, R, 12.3.6, de démontrer que $f_1,\ f_2$ et $g$ sont continues.

Or $g$ est l’application composée
$$
H \times X \times \mathcal{S}^k(X;E) \xrightarrow{(m,\mathrm{Id})} X \times \mathcal{S}^k(X;E) \xrightarrow{(\mathrm{Id},j^k)} X \times C(X;J^k(X,E)) \xrightarrow{\varepsilon} J^k(X;E)
$$
avec $\varepsilon(x, u) = u(x)$; l’application $\varepsilon$ étant continue (TG, X, p. 28, cor. 1), $g$ est continue.

Soit $(h_0, x_0) \in H \times X$; prouvons que $f_1$ est continue en $(h_0, x_0)$. Il existe des cartes $(U, \psi, F)$ et $(V, \chi, F')$ de X et un ouvert $\Omega$ de H tels que $x_0 \in U,\ h_0 \in \Omega$ et $m(\Omega \times U) \subset V$. En utilisant l’expression de $J^k(X,X)$ dans ces cartes, on est ramené à prouver, pour $1 \leq l \leq k$, la continuité en $(h_0, x_0)$ de l’application $(h, x) \mapsto \Delta_x^l(\tau_h)$ de $\Omega \times U$ dans $P_l(F;F')$, avec $\Delta_x^l(\tau_h)(v) = \frac{1}{l!} D^l \tau_h(x).v$ pour $v \in F$ (VAR, R, 12.2).

Or $D^l \tau_h(x)$ n’est autre que la dérivée partielle $l$-ième de $m(h, x)$ par rapport à $x$, qui est continue par hypothèse ; par conséquent $f_1$ est continue. On démontre de même que $f_2$ est continue, d’où le lemme.

#### Proposition 5 {#lie-ix-s6-prop-5 .statement tag=01FE}

*Supposons le groupe* H *compact et notons dh la mesure de Haar sur* H *de masse totale 1. Soit s une section de classe* $C^r$ *de* E. *Pour* $x \in X$, *notons* $s^\#$ l'intégrale vectorielle $\int_H^{h s} dh$. Alors $s^\#$ est une section de classe $C^r$ de $E$, invariante par $H$; pour $x \in X$, on a $s^\#(x) = \int_H h s(h^{-1} x) \, dh \in E_x$. L'endomorphisme $s \mapsto s^\#$ de $\mathscr{S}^r(X; E)$ est un projecteur sur le sous-espace des sections $H$-invariantes.

Considérons l'application $h \mapsto ^h s$ de $H$ dans $\mathscr{S}^r(X; E)$; elle est continue d'après le lemme 4. Puisque l'espace $\mathscr{S}^r(X; E)$ est séparé et complet, l'intégrale $s^\# = \int_H ^h s \, dh$ appartient à $\mathscr{S}^r(X; E)$ (INT, III, § 3, no 3, cor. 2). L'application linéaire $s \mapsto s(x)$ de $\mathscr{S}^r(X; E)$ dans $E_x$ étant continue, on a $s^\#(x) = \int_H ^h s(x) \, dh$ pour tout $x \in X$. Il est clair que $s^\#$ est invariante par $H$; si $s$ est une section $H$-invariante, on a $s^\# = s$, d'où la dernière assertion.

#### Corollaire 1 {#lie-ix-s6-prop-5-cor-1 .statement tag=01FF}

Soient $F$ un espace de Banach, $\rho : H \to \mathbf{GL}(F)$ une représentation linéaire analytique, $f \in \mathscr{C}^r(X; F)$. Pour $x \in X$, posons

$$
f^\#(x) = \int_H \rho(h) \cdot f(h^{-1} x) \, dh .
$$

Alors $f^\#$ est un morphisme de classe $C^r$ de $X$ dans $F$, compatible aux opérations de $H$; pour $x \in X$, on a (en notant $\tau_h$ l'automorphisme $x \mapsto hx$ de $X$)

$$
d_x f^\# = \int_H (\rho(h) \circ d_{h^{-1} x} f \circ T_x(\tau_{h^{-1}})) \, dh \in \mathcal{L}(T_x(X); F) .
$$

La première assertion résulte de la proposition appliquée au fibré $X \times F$, muni de la loi d'opération $(h; (x, f)) \mapsto (hx, \rho(h).f)$. La seconde s'obtient d'après INT, III, § 3, no 2, prop. 2, en appliquant à l'intégrale vectorielle $f^\#$ l'homomorphisme $d_x : \mathscr{C}^r(X; F) \to \mathcal{L}(T_x(X); F)$ qui est continu par définition de la topologie de la $C^r$-convergence compacte.

#### Corollaire 2 {#lie-ix-s6-prop-5-cor-2 .statement tag=01FG}

Soient $F$ un espace de Banach, $f \in \mathscr{C}^r(X; F)$; posons

$$
f^\#(x) = \int_H f(hx) \, dh
$$

pour $x \in X$. La fonction $f^\#$ est de classe $C^r$, et on a $f^\#(hx) = f^\#(x)$ pour $x \in X, h \in H$.

#### Corollaire 3 {#lie-ix-s6-prop-5-cor-3 .statement tag=01FH}

Soient $F$ un espace de Banach, $p$ un entier $\geqslant 0$, $^k \Omega^p(X; F)$ l'espace des formes différentielles de degré $p$ sur $X$, à valeurs dans $F$, de classe $C^k (2 \leq k + 1 \leq r)$. Pour $\omega \in ^k \Omega^p(X; F)$, posons $\omega^\# = \int_H \tau_h^* \omega \, dh$. Alors l'application $\omega \mapsto \omega^\#$ est un projecteur de $^k \Omega^p(X; F)$, dont l'image est le sous-espace des formes $H$-invariantes. On a $d(\omega^\#) = (d\omega)^\#$ pour tout $\omega \in ^k \Omega^p(X; F)$.

La première assertion résulte de la proposition appliquée au $H$-fibré vectoriel

Alt$^p$(T(X); F) (III, § 1, n° 8, exemples). Pour démontrer la seconde assertion, il suffit, compte tenu de INT, III, § 3, n° 2, prop. 2, de prouver que l’application $d : {}^k\Omega^p(X; F) \to {}^{k-1}\Omega^{p+1}(X; F)$ est continue lorsqu’on munit le premier espace (resp. le second) de la topologie de la $C^k$-convergence (resp. $C^{k-1}$-convergence) compacte. Or cela résulte aussitôt de la définition de ces topologies à l’aide de semi-normes (TS, à paraître) et du fait que $d$ est un opérateur différentiel d’ordre $\leqslant 1$ (VAR, R, 14.4.2).

### 5. Formes différentielles invariantes

Soit X une variété réelle de classe $C^\infty$ localement de dimension finie, et soit $(g, x) \mapsto gx$ une loi d’opération à gauche de classe $C^\infty$ du groupe de Lie compact connexe G dans X. Pour $g \in G$, on note $\tau_g$ l’automorphisme $x \mapsto gx$ de X. On désigne par $\Omega(X)$ l’algèbre des formes différentielles réelles de classe $C^\infty$ sur X (VAR, R, 8.3.1).

Pour tout élément $\xi$ de g, notons $D_\xi$ le champ de vecteurs sur X qui lui correspond (III, § 3, n° 5) et $\theta(\xi), i(\xi)$ les opérateurs correspondants sur $\Omega(X)$, de sorte qu’on a les formules (VAR, R, 8.4.5 et 8.4.7)

$$
\theta(\xi)\omega = d(i(\xi)\omega) + i(\xi)d\omega
$$
$$
\frac{d}{dt}(\tau_{\exp t\xi}^*\omega) = \tau_{\exp t\xi}^*(\theta(\xi)\omega).
$$

Une forme différentielle $\omega \in \Omega(X)$ est invariante si on a $\tau_g^*\omega = \omega$ pour tout $g \in G$; d’après la formule (16), il revient au même de dire qu’on a $\theta(\xi)\omega = 0$ pour tout $\xi \in g$. Notons $\Omega(X)^G$ l’espace des formes différentielles invariantes sur X ; si $\omega \in \Omega(X)^G$, on a $d\omega \in \Omega(X)^G$, de sorte que $\Omega(X)^G$ est un sous-complexe du complexe $(\Omega(X), d)$.

#### Théorème 2 {#lie-ix-s6-thm-2 .statement tag=01FI}

L’injection canonique $\iota : \Omega(X)^G \to \Omega(X)$ est un homotopisme de complexes (A, X, p. 33, déf. 5) ; l’application $\omega \mapsto \omega^\# = \int_G \tau_g^*\omega dg$ en est un homotopisme réciproque à homotopie près. En particulier, l’application $H(\iota) : H(\Omega(X)^G) \to H(\Omega(X))$ est bijective.

D’après le cor. 3 du n° 4, l’application $\omega \mapsto \omega^\#$ est un morphisme de complexes de $\Omega(X)$ dans $\Omega(X)^G$, qui induit l’identité sur le sous-complexe $\Omega(X)^G$ ; pour démontrer le théorème, il suffit donc de construire un homomorphisme $s : \Omega(X) \to \Omega(X)$, gradué de degré – 1, tel que

$$
\omega^\# - \omega = (d \circ s + s \circ d)(\omega) \quad \text{pour tout } \omega \in \Omega(X).
$$

D’après le lemme 1 de INT, IX, § 2, n° 4 et la remarque 1 du § 2, n° 2, il existe une mesure positive $d\xi$ sur g, à support compact, dont l’image par l’application exponentielle est égale à $dg$. Posons, pour $\omega \in \Omega(X)$,

$$
s(\omega) = \int_0^1 \left\{ \int_g \tau_{\exp t\xi}^*(i(\xi)\omega).d\xi \right\} dt ;
$$

il s'agit de montrer que la formule (17) est satisfaite. On vérifie comme dans la démonstration du cor. 1 (n° 4) la formule

$$
ds(\omega) = \int_0^1 \left\{ \int_g \tau_{\exp t\xi}^* d(i(\xi)\omega) \cdot d\xi \right\} dt .
$$

On déduit alors des formules (15) et (16) les égalités

$$
\begin{align*}
ds(\omega) + s(d\omega) &= \int_0^1 \left\{ \int_g \tau_{\exp t\xi}^* (d(i(\xi)\omega) + i(\xi)d\omega) \cdot d\xi \right\} dt \\
&= \int_0^1 \left\{ \int_g \tau_{\exp t\xi}^* (\theta(\xi)\omega) \cdot d\xi \right\} dt \\
&= \int_g \left\{ \int_0^1 \frac{d}{dt} (\tau_{\exp t\xi}^* \omega) \, dt \right\} d\xi \\
&= \int_g (\tau_{\exp \xi}^* \omega - \omega) \, d\xi \\
&= \omega^\# - \omega ,
\end{align*}
$$

d'où le th. 2.

Appliquons ce théorème dans le cas $X = G$, pour l'action de $G$ par translations à gauche. Rappelons (III, § 3, n° 13, prop. 50) qu'en associant à une forme différentielle sur $G$ sa valeur à l'élément neutre, on obtient un isomorphisme de $\Omega(G)^G$ sur l'algèbre graduée $\mathrm{Alt}(g)$ des formes multilinéaires alternées sur $g$. Identifions $\Omega(G)^G$ à $\mathrm{Alt}(g)$ par cet isomorphisme. L'opérateur $d$ est alors donné par la formule (III, § 3, n° 14, prop. 51)

$$
d\omega(a_1, ..., a_{p+1}) = \sum_{i < j} (-1)^{i+j} \omega([a_i, a_j], a_1, ..., a_{i-1}, a_{i+1}, ..., a_{j-1}, a_{j+1}, ..., a_{p+1})
$$

pour $\omega$ dans $\mathrm{Alt}^p(g)$ et $a_1, ..., a_{p+1}$ dans $g$.

Pour $\xi \in g$, soit $L_\xi$ le champ de vecteurs invariant à gauche qui lui correspond (défini au moyen de l'action de $G$ sur lui-même par translations à droite, cf. III, § 3, n° 6). Les opérateurs $\theta(L_\xi), i(L_\xi)$ commutent à l'action de $G$ sur $\Omega(G)$ définie par translation à gauche, donc induisent des opérateurs $\theta(\xi), i(\xi)$ de $\Omega(G)^G$; dans l'identification précédente, ceux-ci s'expriment par les formules (VAR, R, 8.3.2 et 8.4.2).

$$
\begin{align*}
(\theta(\xi)\omega)(a_1, ..., a_p) &= - \sum_i \omega(a_1, ..., a_{i-1}, [\xi, a_i], a_{i+1}, ..., a_p) \\
(i(\xi)\omega)(a_1, ..., a_{p-1}) &= \omega(\xi, a_1, ..., a_{p-1})
\end{align*}
$$

pour $\omega$ dans $\mathrm{Alt}^p(g)$ et $a_1, ..., a_p$ dans $g$.

Le sous-complexe $^G\Omega(G)^G$ des formes *biinvariantes* (III, § 3, n° 13) s’identifie au sous-complexe $\mathrm{Alt}(g)^G$ des formes multilinéaires alternées sur $g$ invariantes par la représentation adjointe (c’est-à-dire telles que $\theta(\xi)\ \omega = 0$ pour tout $\xi \in g$). On a donc un diagramme commutatif de complexes

$$
\begin{array}{ccc}
^G\Omega(G)^G & \to & \Omega(G)^G \to \Omega(G) \\
\downarrow & & \downarrow \\
\mathrm{Alt}(g)^G & \to & \mathrm{Alt}(g)
\end{array}
$$

(18)

où les flèches horizontales sont les injections canoniques, et les flèches verticales sont les isomorphismes induits par l’application $\omega \mapsto \omega(e)$.

**Corollaire 1. — a)** *Dans le diagramme (18), tous les morphismes sont des homotopismes.*

*b)* *Soit $\omega \in \mathrm{Alt}(g)$. Pour que $\omega$ appartienne à $\mathrm{Alt}(g)^G$, il faut et il suffit qu’on ait $d\omega = 0$ et $d(i(\xi)\ \omega) = 0$ pour tout $\xi \in g$. La différentielle du complexe $\mathrm{Alt}(g)^G$ est nulle.*

*c)* *L’espace vectoriel gradué $\mathrm{H}(\Omega(G))$ est isomorphe à $\mathrm{Alt}(g)^G$.*

Le théorème, appliqué à l’action de $G$ sur $G$ par translations à gauche (resp. à l’action $((g, h); x) \mapsto gxh^{-1}$ de $G \times G$ sur $G$) entraîne que l’injection canonique $\Omega(G)^G \to \Omega(G)$ (resp. $^G\Omega(G)^G \to \Omega(G)$) est un homotopisme ; compte tenu de A, X, p. 34, corollaire, l’assertion *a)* en résulte.

Démontrons *b)*. D’après la prop. 51 de III, § 3, n° 14, on a $d\alpha = - d\alpha$, c’est-à-dire $d\alpha = 0$, pour toute forme différentielle $\alpha$ sur $G$ qui est invariante à gauche et à droite. Si $\omega \in \mathrm{Alt}(g)^G$, on a donc $d\omega = 0$, et par conséquent $d(i(\xi)\ \omega) = \theta(\xi)\ \omega - i(\xi)\ d\omega = 0$. Inversement si $d\omega = 0$ et $d(i(\xi)\ \omega) = 0$, on a $\theta(\xi)\ \omega = 0$.

L’assertion *c)* résulte de *a)* et *b)*.

#### Remarque {#lie-ix-s6-n5-rem-1 .statement tag=01FK}

Considérons les sous-complexes $Z(\Omega(G))$ et $B(\Omega(G))$ de $\Omega(G)$ (A, X, p. 25). Il résulte de la formule donnant la différentielle du produit de deux formes (VAR, R, 8.3.5) que $Z(\Omega(G))$ est une sous-algèbre de $\Omega(G)$ et que $B(\Omega(G))$ est un idéal de $Z(\Omega(G))$; par conséquent le produit extérieur induit sur $\mathrm{H}(\Omega(G))$ une structure d’algèbre graduée. On déduit alors de ce qui précède un isomorphisme d’algèbres graduées $\mathrm{H}(\Omega(G)) \to \mathrm{Alt}(g)^G$.

Soit $H$ un sous-groupe fermé de $G$; appliquons maintenant le th. 2 à $X = G/H$. D’après III, § 1, n° 8, cor. 1 à la prop. 17, les formes différentielles $G$-invariantes sur $G/H$ s’identifient aux éléments $H$-invariants de $\mathrm{Alt}(T_e(G/H))$, c’est-à-dire encore aux éléments de $\mathrm{Alt}(g)$ qui sont $H$-invariants et annulés par les opérateurs $i(\xi)$ pour tout $\xi \in L(H)$. Par suite :

**Corollaire 2. — Soit $H$ un sous-groupe fermé de $G$.**

*a)* *L’injection canonique $\Omega(G/H)^G \to \Omega(G/H)$ est un homotopisme.*

*b)* *Le complexe $\Omega(G/H)^G$ s’identifie au sous-complexe de $\mathrm{Alt}(g)$ formé des éléments $\omega$ de $\mathrm{Alt}(g)$ qui sont invariants pour la représentation adjointe de $H$ et tels que $i(\xi)\ \omega = 0$ pour tout $\xi \in L(H)$. Si en outre $H$ est connexe, ce sous-complexe est formé des $\omega \in \mathrm{Alt}(g)$ tels que $\theta(\xi)\ \omega = 0$ et $i(\xi)\ \omega = 0$ pour tout $\xi \in L(H)$.*

## EXERCICES {#lie-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
