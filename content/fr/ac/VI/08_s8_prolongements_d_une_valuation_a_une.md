---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 8
section_title: Prolongements d’une valuation à une extension algébrique
lang: fr
source: ac-v-vii-fr
pdf_pages: 0133-0151, 0183-0191
extraction: ocr
subsections:
    - "no": 1
      title: Indice de ramification. Degré résiduel
      page: 0
      pdf_page: 133
    - "no": 2
      title: Prolongement d’une valuation et complétion
      page: 0
      pdf_page: 136
    - "no": 3
      title: La relation $\sum_i e_i f_i \leq n$
      page: 0
      pdf_page: 138
    - "no": 4
      title: Indice initial de ramification
      page: 0
      pdf_page: 141
    - "no": 5
      title: La relation $\sum_i e_i f_i = n$
      page: 0
      pdf_page: 142
    - "no": 6
      title: Anneaux de valuation dans une extension algébrique
      page: 0
      pdf_page: 147
    - "no": 7
      title: Prolongement des valeurs absolues.
      page: 0
      pdf_page: 149
statements: 42
exercises: 22
content_sha256: 2bebe6600828f81de20f560173885512ca5f89218ee8866a421e03059969a264
---

## § 8. Prolongements d’une valuation à une extension algébrique.

### 1. Indice de ramification. Degré résiduel

Soient K un corps, L une extension de K, et A’ un anneau de valuation pour L. Comme on l’a vu au § 1, no 4, l’anneau $A = K \cap A'$ est un anneau de valuation pour K, et l’on a $m(A) = m(A') \cap K$. Si $\nu'$ est une valuation associée à $A'$, la restriction $\nu$ de $\nu'$ à K est une valuation de K associée à A;

le groupe des ordres $\Gamma_v$ de $\nu$ est un sous-groupe du groupe des ordres $\Gamma_{v'}$ de $\nu'$.

#### Définition 1 {#ac-vi-s8-def-1 .statement}

On appelle indice de ramification de $\nu'$ par rapport à $\nu$ (ou par rapport à $K$), et l’on note $e(\nu'/\nu)$, (ou $e(A'/A)$, ou parfois $e(L/K)$) l’indice $(\Gamma_{v'} : \Gamma_v)$.

Cet indice est un entier naturel, ou $+\infty$. Lorsque $\nu'_0$ est une valuation équivalente à $\nu'$, on dira encore que $e(\nu'/\nu)$ est l’indice de ramification de $\nu'_0$ par rapport à $\nu$. Si $e(\nu'/\nu) = 1$, on dit que $\nu'$ est non ramifiée par rapport à $\nu$.

D’autre part le corps résiduel $\kappa(A)$ de $\nu$ s’identifie à un sous-corps du corps résiduel $\kappa(A')$ de $\nu'$.

#### Définition 2 {#ac-vi-s8-def-2 .statement}

On appelle degré résiduel de $\nu'$ par rapport à $\nu$ (ou par rapport à $K$), et l’on note $f(\nu'/\nu)$ (ou $f(A'/A)$, ou parfois $f(L/K)$), le degré $[\kappa(A') : \kappa(A)]$.

Ce degré est un entier naturel, ou bien $+\infty$.

#### Lemme 1 {#ac-vi-s8-lem-1 .statement}

Soient $K, K', K''$ trois corps tels que $K \subset K' \subset K''$; $\nu''$ une valuation de $K''$, $\nu$ et $\nu'$ ses restrictions à $K$ et $K'$. On a les relations :

(1) $e(\nu''/\nu) = e(\nu''/\nu')e(\nu'/\nu)$, $f(\nu''/\nu) = f(\nu''/\nu')f(\nu'/\nu)$.

C’est évident.

#### Lemme 2 {#ac-vi-s8-lem-2 .statement}

Soient $K$ un corps, $L$ une extension de degré fini $n$ de $K$, $\nu'$ une valuation de $L$, et $\nu$ sa restriction à $K$. On a l’inégalité

(2) $e(\nu'/\nu)f(\nu'/\nu) \leq n;$

en particulier $e(\nu'/\nu)$ et $f(\nu'/\nu)$ sont finis.

En effet, prenons des entiers naturels $r$ et $s$ respectivement inférieurs à $e(\nu'/\nu)$ et $f(\nu'/\nu)$. Il suffit de montrer qu’on a $rs \leq n$. Vu la définition de $r$, il existe des éléments $x_i$ de $L$ ($1 \leq i \leq r$) tels que $\nu'(x_i) \equiv \nu'(x_j)$ (mod. $\Gamma_v$) pour $i \neq j$. Vu la définition de $s$, il existe des éléments $y_k$ ($1 \leq k \leq s$) de l’anneau $A'$ de $\nu'$ dont les images canoniques $\overline{y}_k$ dans $\kappa(A')$ sont linéairement indépendantes sur $\kappa(A)$; on a évidemment $\nu'(y_k) = 0$ pour tout $k$. Nous allons montrer que les $rs$ éléments $x_iy_k$ sont linéairement indépendants sur $K$, ce qui établira bien l’inégalité $rs \leq n$.

Supposons donc qu’il existe une relation linéaire non triviale de la forme

(3) $$
\sum_{i,k} a_{ik} x_i y_k = 0 \quad (a_{ik} \in K).
$$

Choisissons les indices $j, m$ de sorte que
$$
\nu'(a_{jm} x_j y_m) \leq \nu'(a_{ik} x_i y_k)
$$
pour tout couple $(i, k)$; on a alors $a_{jm} \neq 0$. Si $i \neq j$, on ne peut avoir $\nu'(a_{ik} x_i y_k) = \nu'(a_{jm} x_j y_m)$ car ceci entraînerait
$$
\nu'(x_i) - \nu'(x_j) = \nu'(a_{jm}) - \nu'(a_{ik}) \in \Gamma_v,
$$
contrairement au choix des $x_i$. En multipliant (3) par $(a_{jm} x_j)^{-1}$, on obtient une relation de la forme
$$
\sum_k b_k y_k + z = 0, \quad \text{où} \quad b_k = \frac{a_{jk} x_j}{a_{jm} x_j} \in A', \quad z \in A'
$$
et $\nu'(b_k) \geq 0,\ \nu'(z) > 0$. D’où, dans $\kappa(A')$, une relation de la forme $\sum_k \overline{b_k} \overline{y_k} = 0$. Comme $b_m = 1$, ceci contredit l’hypothèse faite sur $y_k$.

#### Proposition 1 {#ac-vi-s8-prop-1 .statement}

*Soient K un corps, L une extension algébrique de K, $\nu'$ une valuation de L, $\nu$ sa restriction à K, A et A' les anneaux de $\nu$ et $\nu'$. Alors $\Gamma_{v'}/\Gamma_v$ est un groupe de torsion, et $\kappa(A')$ est une extension algébrique de $\kappa(A)$*.

Soit en effet $(L_\alpha)$ la famille des sous-extensions de degré fini de L; posons $\Gamma_\alpha = \nu'(L_\alpha^*)$. Le groupe $\Gamma_{v'}$ est réunion de la famille filtrante croissante formée par les $\Gamma_\alpha$; comme les groupes $\Gamma_\alpha/\Gamma_v$ sont finis (lemme 2), $\Gamma_{v'}/\Gamma_v$ est un groupe de torsion. On raisonne de même pour prouver que $\kappa(A')$ est une extension algébrique de $\kappa(A)$.

#### Corollaire 1 {#ac-vi-s8-prop-1-cor-1 .statement}

*La hauteur de $\nu'$ est égale à celle de $\nu$*.

Ceci résulte en effet de la prop. 1 et du lemme suivant:

#### Lemme 3 {#ac-vi-s8-lem-3 .statement}

*Soient G' un groupe totalement ordonné, G un sous-groupe de G' et $\mathfrak{S}'$ (resp. $\mathfrak{S}$) l’ensemble des sous-groupes isolés de G' (resp. G). L’application $H' \to H' \cap G$ applique $\mathfrak{S}'$ sur $\mathfrak{S}$. Cette application est bijective si $G'/G$ est un groupe de torsion*.

Il est clair que $H' \in \mathfrak{S}'$ implique $H' \cap G \in \mathfrak{S}$. Soit maintenant $H \in \mathfrak{S}$; notons $H'$ l’ensemble des $x' \in G'$ tels qu’il existe $h \in H$

C.Q.F.D.

#### Corollaire 2 {#ac-vi-s8-lem-3-cor-2 .statement}

Pour que $\varphi'$ soit impropre (resp. de hauteur 1), il faut et il suffit que $\varphi$ soit impropre (resp. de hauteur 1).

#### Corollaire 3 {#ac-vi-s8-lem-3-cor-3 .statement}

Supposons que $L$ soit une extension de degré fini de $K$. Pour que $\varphi'$ soit discrète, il faut et il suffit que $\varphi$ soit discrète.

Si $\varphi'$ est discrète, $\Gamma_v$ est isomorphe à un sous-groupe non nul de $\mathbf{Z}$ (cor. 2), donc à $\mathbf{Z}$. Réciproquement, si $\varphi$ est discrète, $\Gamma_v$ est isomorphe à $\mathbf{Z}$, et $\Gamma_{v'}/\Gamma_v$ est un groupe fini (lemme 2); donc $\Gamma_{v'}$ est un groupe commutatif de type fini, de rang 1, et sans torsion; par conséquent il est isomorphe à $\mathbf{Z}$.

### 2. Prolongement d’une valuation et complétion

#### Définition 3 {#ac-vi-s8-def-3 .statement}

Soient $K$ un corps, $\varphi$ une valuation de $K$, et $L$ une extension de $K$. On appelle système complet de prolongements de $\varphi$ à $L$ une famille $(\varphi'_i)_{i \in I}$ de valuations de $L$ prolongeant $\varphi$, telle que toute valuation de $L$ prolongeant $\varphi$ soit équivalente à une $\varphi'_i$ et à une seule.

#### Proposition 2 {#ac-vi-s8-prop-2 .statement}

Soient $K$ un corps, $\varphi$ une valuation de $K$, $\hat{K}$ le complété de $K$ pour $\varphi$, $\hat{\varphi}$ le prolongement continu de $\varphi$ à $\hat{K}$, et $L$ une extension de degré fini $n$ de $K$.

a) Soit $\varphi'$ une valuation de $L$ prolongeant $\varphi$; notons $\hat{L}_{v'}$ le complété de $L$ pour $\varphi'$ et $\hat{\varphi}'$ le prolongement continu de $\varphi'$ à $\hat{L}_{v'}$; en identifiant $\hat{K}$ à l’adhérence de $K$ dans $\hat{L}_{v'}$, on a

$$
(4) \quad e(\hat{\varphi}'/\hat{\varphi}) = e(\varphi'/\varphi), \quad f(\hat{\varphi}'/\hat{\varphi}) = f(\varphi'/\varphi),
$$
$$
(5) \quad [\hat{L}_{v'} : \hat{K}] \leq n,
$$
$$
(6) \quad e(\varphi'/\varphi)f(\varphi'/\varphi) \leq [\hat{L}_{v'} : \hat{K}]
$$

b) Tout ensemble de valuations deux à deux indépendantes de L prolongeant une valuation non impropre $\nu$ est fini. Notons $\nu'_1, \ldots, \nu'_s$ des valuations deux à deux indépendantes de L prolongeant $\nu$, telles que toute valuation de L prolongeant $\nu$ soit dépendante de l’une des $\nu'_i$; soient $L_i$ le corps L muni de la topologie définie par $\nu'_i$, $\hat{L}_i$ son complété; posons $n_i = [\hat{L}_i : \hat{K}]$. Alors l’application canonique $\varphi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i$ (prolongeant par continuité l’application diagonale $L \to \prod_{i=1}^s L_i$) est surjective, son noyau est le radical de $\hat{K} \otimes_K L$, et l’on a

$$
\sum_{i=1}^s n_i \leq n.
$$

(7)

Démontrons d’abord a). On peut supposer $\nu$ non impropre. Comme $\nu$ et $\hat{\nu}$ (resp. $\nu'$ et $\hat{\nu}'$) ont même groupe des ordres et même corps résiduel (§ 5, no 3, prop. 5, b) et f)), (4) est vraie. On en déduit (6) au moyen du lemme 2. Enfin le sous-$\hat{K}$-espace vectoriel de $\hat{L}_{\nu'}$ engendré par L est fermé (§ 5, no 2, cor. de la prop. 4) et partout dense, donc égal à $\hat{L}_{\nu'}$; ceci démontre (5).

Passons à b). On peut encore supposer $\nu$ non impropre. Soit $(\nu'_1, \ldots, \nu'_r)$ une famille finie quelconque de valuations deux à deux indépendantes de L prolongeant $\nu$. L’image de L dans $\prod_{i=1}^r L_i$ par l’application diagonale est partout dense (§ 7, no 2, th. 1) et $\prod_{i=1}^r L_i$ est dense dans $\prod_{i=1}^r \hat{L}_i$. Donc l’image canonique de $\hat{K} \otimes_K L$ dans $\prod_{i=1}^r \hat{L}_i$ est partout dense. D’autre part cette image est un sous-$\hat{K}$-espace vectoriel de $\prod_{i=1}^r \hat{L}_i$; comme $\prod_{i=1}^r \hat{L}_i$ est de dimension finie sur $\hat{K}$ d’après (5), l’image de $\hat{K} \otimes_K L$ est fermée (§ 5, no 2, cor. de la prop. 4), donc égale à $\prod_{i=1}^r \hat{L}_i$. Comme la dimension de $\hat{K} \otimes_K L$ sur $\hat{K}$ est $n$, on a $\sum_{i=1}^r n_i \leq n$. Ceci montre en particulier que l’entier $r$ est majoré par $n$, et démontre la première assertion de b).

Prenons maintenant $(\nu'_1, \ldots, \nu'_s)$ comme dans l’énoncé. La surjectivité de $\varphi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i$ et la relation (7) ont déjà

#### Corollaire 1 {#ac-vi-s8-prop-2-cor-1 .statement}

*Si $K$ est complet pour $\nu$, et si $\nu$ est non impropre, deux valuations de $L$ prolongeant $\nu$ sont dépendantes.* En effet, on a $\hat{K} \otimes_K L = L$.

#### Corollaire 2 {#ac-vi-s8-prop-2-cor-2 .statement}

*Si $\hat{K}$ ou $L$ est séparable sur $K$, l’application canonique $\varphi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i$ est un isomorphisme.* En effet le radical de $\hat{K} \otimes_K L$ est alors nul (*Alg.*, chap. VIII, § 7, no 3, th. 1).

#### Remarque {#ac-vi-s8-n2-rem-1 .statement}

La prop. 2, b) montre que toute *extension composée* de $\hat{K}$ et $L$ sur $K$ (*Alg.*, chap. VIII, § 8) est isomorphe à l’un des complétés $\hat{L}_i$, et que ceux-ci sont des extensions composées deux à deux non isomorphes.

### 3. La relation $\sum_i e_i f_i \leq n$

Soient $K$ un corps, $\nu$ une valuation de $K$, et $L$ une extension de degré fini $n$ de $K$. Soient $(\nu'_1, \ldots, \nu'_r)$ des valuations deux à deux *inéquivalentes* de $L$ prolongeant $\nu$; si elles sont *indépendantes* (ce qui est toujours le cas si $\nu$ est de hauteur 1), on a $\sum_{i=1}^r e(\nu'_i/\nu)f(\nu'_i/\nu) \leq n$ en vertu de la prop. 2 (formules (6)) et (7)). Nous allons voir que ce résultat est vrai dans le cas général. De façon précise :

#### Théorème 1 {#ac-vi-s8-thm-1 .statement}

Soient K un corps, $\varphi$ une valuation de K, et L une extension de degré fini n de K. Alors :
a) Tout système complet $(\varphi'_i)_{i \in I}$ de prolongements de $\varphi$ à L est fini.
b) On a $\sum_{i \in I} e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n$, et a fortiori Card(I) $\leq n$.
c) Les anneaux des $\varphi'_i$ sont deux à deux non comparables pour la relation d’inclusion.

Le théorème étant trivial si $\varphi$ est impropre, nous supposerons $\varphi$ non impropre. Soit $(\varphi'_1, \ldots, \varphi'_s)$ une famille finie quelconque de valuations deux à deux inéquivalentes de L prolongeant $\varphi$.

Nous allons d’abord prouver que $\sum_{i=1}^s e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n$. Ceci démontrera a) et b).

Nous raisonnons par récurrence sur s, et supposerons donc notre inégalité établie dans le cas de 0, 1, ..., s—1 valuations. Nous distinguons 2 cas.

1) Supposons qu’il existe au moins deux valuations $\varphi'_i$ indépendantes. Il existe alors (§ 7, no 2, Remarque 1), une partition $\{1, s\} = I_1 \cup \cdots \cup I_t$ de $\{1, s\}$ telle que :
(i) pour que $\varphi'_i$ et $\varphi'_j$ soient dépendantes, il faut et il suffit que i et j appartiennent à un même $I_k$;
(ii) Card$(I_k) < s$ pour tout k.

Choisissons dans chaque $I_k$ un indice $i(k)$. Notons $\hat{L}_{i(k)}$ le complété de L pour $\varphi'_{i(k)}$, et posons $n(k) = [\hat{L}_{i(k)} : \hat{K}]$. Pour tout $i \in I_k$, $\varphi'_i$ définit sur L la même topologie que $\varphi'_{i(k)}$ (§ 7, no 2, prop. 3)), donc se prolonge en une valuation $\hat{\varphi}'_i$ de $\hat{L}_{i(k)}$ dont la restriction à $\hat{K}$ est $\hat{\varphi}$. Puisque les $\varphi'_i$ pour $i \in I_k$ sont deux à deux inéquivalentes, il en est de même des $\hat{\varphi}'_i$. L’hypothèse de récurrence appliquée au couple $(\hat{K}, \hat{L}_{i(k)})$ montre, en vertu de la prop. 2, a), formule (4), que l’on a $\sum_{i \in I_k} e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n(k)$. Comme $\sum_{k=1}^t n(k) \leq n$ (prop. 2, b), formule (7)), on a bien $\sum_{i=1}^s e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n$.

2) Passons au cas où deux quelconques des $\varphi'_i$ sont dépendantes. Soit $A'_i$ l’anneau de $\varphi'_i (1 \leq i \leq s)$; en notant A l’anneau de $\varphi$, on a $A'_i \cap K = A$ pour tout i. Soit B' le sous-anneau de L engendré par $A'_1, \ldots, A'_s$; posons $B = B' \cap K$: on a $B \supset A$. Alors B est l’anneau d’une valuation $\omega$ de $K$, et $B'$ l’anneau d’une valuation non impropre $\omega'$ de $L$ prolongeant $\omega$ ($§ 7$, n° 2, prop. 4); le corps $\kappa(B')$ est une extension de degré $f(\omega'/\omega)$ de $\kappa(B)$. Considérons les images canoniques $\overline{A'_i}$, $\overline{A}$ de $A'_i$ et $A$ dans $\kappa(B')$; alors $\overline{A}$ est l’anneau d’une valuation $\bar{\nu}$ de $\kappa(B)$, et les $\overline{A'_i}$ sont les anneaux de valuations $\bar{\nu}'_i$ de $\kappa(B')$ prolongeant $\bar{\nu}$. Comme les $A'_i$ engendrent $B'$, les $\overline{A'_i}$ engendrent $\kappa(B')$, donc les $\bar{\nu}'_i$ ne sont pas toutes dépendantes ($§ 7$, n° 2, prop. 4). D’après la première partie de la démonstration, on a

$$
\sum_{i=1}^{s} e(\bar{\nu}'_i/\bar{\nu}) f(\bar{\nu}'_i/\bar{\nu}) \leq [\kappa(B') : \kappa(B)] = f(\omega'/\omega)
$$

donc

$$
\sum_{i=1}^{s} e(\omega'/\omega) e(\bar{\nu}'_i/\bar{\nu}) f(\bar{\nu}'_i/\bar{\nu}) \leq e(\omega'/\omega) f(\omega'/\omega) \leq n \quad (\text{n° 1, lemme 1}).
$$

La démonstration de a) et b) sera donc terminée si nous prouvons que l’on a

$$(8)$$
$$
f(\bar{\nu}'_i/\bar{\nu}) = f(\nu'_i/\nu), \quad e(\omega'/\omega) e(\bar{\nu}'_i/\bar{\nu}) = e(\nu'_i/\nu).
$$

Remarquons, pour cela, que $\nu$ et $\bar{\nu}$ (resp. $\nu'_i$ et $\bar{\nu}'_i$) ont même corps résiduel ($§ 4$, n° 1, cor. de la prop. 2); ceci prouve la première égalité. Pour la seconde on a, en vertu de la Remarque du $§ 4$, n° 3, le diagramme commutatif suivant, où les lignes sont des suites exactes, et où les flèches verticales représentent les injections canoniques:

$$
\begin{array}{ccccccccc}
0 & \to & \Gamma_{\bar{\nu}}^- & \to & \Gamma_{\nu} & \to & \Gamma_w & \to & 0 \\
& & \downarrow & & \downarrow & & \downarrow & & \\
0 & \to & \Gamma_{\nu_i'}^- & \to & \Gamma_{\nu_i'} & \to & \Gamma_{w'} & \to & 0.
\end{array}
$$

On en déduit, ce qui démontre la seconde formule (8), qu’on a une suite exacte

$$
0 \to \Gamma_{\nu_i'}^-/\Gamma_{\bar{\nu}}^- \to \Gamma_{\nu_i'}/\Gamma_{\nu} \to \Gamma_{w'}/\Gamma_w \to 0
$$

en vertu du chap. I, $§ 1$, n° 4, prop. 2.

Pour terminer la démonstration du th. 1, il reste à prouver c). Si l’anneau de $\nu'_i$ contient celui de $\nu'_j$, $\Gamma_{\nu_i'}$ s’identifie à un groupe quotient $\Gamma_{\nu_j'}/H$, $H$ étant un sous-groupe isolé ($§ 4$, n° 3). Comme l’application canonique composée $\Gamma_{\nu} \to \Gamma_{\nu_j'} \to \Gamma_{\nu_j'}/H = \Gamma_{\nu_i'}$ est injective, on a $H \cap \Gamma_{\nu} = \{0\}$, d’où $H = \{0\}$ (lemme 3, n° 1). Alors $\nu'_i$ et $\nu'_j$ sont équivalentes, d’où $i = j$.

#### Remarque {#ac-vi-s8-n3-rem-1 .statement}

L’intersection C des anneaux $A'_i$ des valuations $\nu'_i (i \in I)$ est la fermeture intégrale de A dans L ($§ 1, n^o 3$, cor. 3 du th. 3); il résulte en outre de c) et du $§ 7, n^o 1$, prop. 1 et 2, que C est un anneau semi-local, que ses idéaux maximaux sont les intersections $m_i = C \cap m(A'_i)$ et que $A'_i = C_{m_i}$ pour tout $i \in I$.

### 4. Indice initial de ramification

#### Définition 4 {#ac-vi-s8-def-4 .statement}

Soient G un groupe commutatif totalement ordonné, et H un sous-groupe d’indice fini de G. On appelle indice initial de H dans G, et l’on note $\varepsilon(G, H)$, le nombre des sous-ensembles majeurs de G formés d’éléments strictement positifs, et contenant tous les éléments $> 0$ de H.

Cet indice initial est un entier naturel, en vertu de la proposition suivante :

#### Proposition 3 {#ac-vi-s8-prop-3 .statement}

Les hypothèses sont celles de la déf. 4. Si l’ensemble des éléments strictement positifs de G n’a pas de plus petit élément, on a $\varepsilon(G, H) = 1$ quel que soit H. S’il existe un plus petit élément $> 0$ de G, et si l’on note G’ le sous-groupe qu’il engendre, on a $\varepsilon(G, H) = (G' : (G' \cap H))$.

Dans le premier cas, soit x un élément $> 0$ de G. L’ensemble des $y \in G$ tels que $0 < y < x$ est infini, donc il existe deux éléments de cet ensemble qui sont distincts et congrus modulo H; leur différence est un élément z ’de H tel que $0 < z < x$. Donc tout sous-ensemble majeur qui contient tous les éléments strictement positifs de H contient x, donc tous les éléments $> 0$ de G.

Dans le second cas, soit x le plus petit élément $> 0$ de G, et soit n le plus petit entier $> 0$ tel que $nx \in H$. Il est clair que $n = (G' : (G' \cap H))$. D’autre part, en notant M(y) l’ensemble des $z \in G$ tels que $y \leq z (y \in G)$, on voit aussitôt que les ensembles majeurs de la déf. 4 ne sont autres que M(x), M(2x), ..., M(nx).

C.Q.F.D.

#### Corollaire {#ac-vi-s8-n4-cor-1 .statement}

L’indice initial $\varepsilon(G, H)$ divise l’indice $(G : H)$, et lui est égal si G est isomorphe à $\mathbf{Z}$.
En particulier, on a $\varepsilon(G, H) \leq (G : H)$.

#### Définition 5 {#ac-vi-s8-def-5 .statement}

Soient K un corps, L une extension de degré fini de K, $\omega$ une valuation de L, $\nu$ sa restriction à K,

Γ_w et Γ_v leurs groupes des ordres. On appelle indice initial de ramification de ω par rapport à ν (ou par rapport à K) et l’on note ε(ω/ν), l’indice initial de Γ_v dans Γ_w.

D’après le corollaire ci-dessus, ε(ω/ν) divise e(ω/ν), avec égalité dans le cas d’une valuation discrète.

#### Proposition 4 {#ac-vi-s8-prop-4 .statement}

Les hypothèses sont celles de la déf. 5. Soient A et m (resp. A' et m') l’anneau et l’idéal de la valuation ν (resp. ω). On a

$$ [A'/mA': A/m] = \varepsilon(\omega/\nu)f(\omega/\nu). $$

Les idéaux de A' contenant mA' et distincts de A' correspondent en effet aux sous-ensembles majeurs de Γ_w formés d’éléments > 0 et contenant les éléments > 0 de Γ_v (§ 3, n° 5, cor. de la prop. 7). Ils sont donc en nombre égal à ε(ω/ν), et, comme ils forment un ensemble totalement ordonné par inclusion, ce nombre est égal à la longueur de l’anneau quotient A'/mA'. Or un module de longueur 1 sur A' est un espace vectoriel de dimension 1 sur A'/m', donc un module de longueur f(ω/ν) sur A; donc, comme A'/mA' est de longueur ε(ω/ν) sur A', il est de longueur ε(ω/ν)f(ω/ν) sur A, c’est-à-dire sur A/m. C.Q.F.D.

### 5. La relation $\sum_i e_i f_i = n$

#### Proposition 5 {#ac-vi-s8-prop-5 .statement}

Soient K un corps, ν une valuation de K, A son anneau, m son idéal, L une extension de degré fini n de K, B la fermeture intégrale de A dans L, et (ν'_i)_{1 \leq i \leq s} un système complet de prolongements de ν à L. On a alors

$$ [B/mB : A/m] = \sum_{i=1}^s \varepsilon(\nu'_i/\nu)f(\nu'_i/\nu). $$

Soit A_i l’anneau de ν'_i; on a A_i = B_{m_i}, où m_i parcourt la famille des idéaux maximaux de B (n° 3, Remarque). Soit q_i le saturé de mB par rapport à m_i (Chap. II, § 2, n° 4). D’après le Chap. V, cor. 3 de la prop. 1, n° 1, § 2, l’homomorphisme canonique B/mB → $\prod_{i=1}^s B/q_i$ est un isomorphisme, et m_i est le seul idéal maximal de B contenant q_i. Donc B/q_i est canoniquement isomorphe à (B/q_i)_{m_i} (Chap. II, § 3, n° 3, prop. 8), c’est-à-dire à $B_{m_i}/mB_{m_i} = A_i/mA_i$. On a donc un isomorphisme canonique $B/mB \to \prod_{i=1}^s A_i/mA_i$, d’où le résultat en vertu de la prop. 4 du no 4.

#### Corollaire {#ac-vi-s8-n5-cor-1 .statement}

Avec les mêmes hypothèses et notations, on a

$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(\varphi'_i/\varphi)f(\varphi'_i/\varphi') \leq \sum_{i=1}^s e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n.
$$

On sait en effet qu’on a $\varepsilon(\varphi'_i/\varphi) \leq e(\varphi'_i/\varphi)$ (no 4, cor. de la prop. 3) et $\sum_{i=1}^s e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) \leq n$ (no 3, th. 1).

#### Théorème 2 {#ac-vi-s8-thm-2 .statement}

Les hypothèses et notations étant celles de la prop. 5, les conditions suivantes sont équivalentes:

a) B est un A-module de type fini;
b) B est un A-module libre;
c) on a $[B/mB : A/m] = n;$
d) on a $\sum_{i=1}^n e(\varphi'_i/\varphi)f(\varphi'_i/\varphi) = n,$ et $\varepsilon(\varphi'_i/\varphi) = e(\varphi'_i/\varphi)$ pour tout i.

L’équivalence de a) et b) résulte du lemme 1, § 3, no 6. Il est clair que b) implique c) (Alg., chap. II, 3e éd., § 1, no 5, formule (19)). L’équivalence de c) et d) résulte du cor. de la prop. 5. Reste à voir que c) implique b).

De façon générale, si M est un A-module, nous noterons V(M) l’espace vectoriel $M/mM$ sur $A/m$. L’hypothèse c) signifie que $\dim(V(B)) = n$. Soient $x_1, \ldots, x_n$ des éléments de B dont les images canoniques dans V(B) forment une base de V(B), et soit $L \subset B$ le sous-A-module qu’ils engendrent. Comme L est sans torsion et de type fini, il est libre (§ 3, no 6, lemme 1). Nous allons voir que $B = L$. Soit $y \in B$; posons $M = L + Ay$; c’est encore un A-module libre. Les injections canoniques $L \to M \to B$ donnent des homomorphismes canoniques $V(L) \to V(M) \to V(B)$. Comme les rangs de L et M sont $\leq n$, il en est de même des dimensions de V(L) et V(M). Or, par hypothèse, $V(L) \to V(B)$ est surjectif, et V(B) est de dimension $n$, donc V(L) et V(M) sont de dimension $n$, et $V(L) \to V(M)$ est surjectif. Comme M est de type fini, $L \to M$ est surjectif (Chap. II, § 3, no 2, cor. 1 de la prop. 4), d’où $L = M, \ y \in L$ et $B = L$. Donc B est libre.

C.Q.F.D.

#### Remarque 1 {#ac-vi-s8-n5-rem-1 .statement}

Lorsque $\nu$ est discrète, on a $\varepsilon(\nu_i'/\nu) = e(\nu_i'/\nu)$ (no 4), et la condition d) se réduit à $\sum_{i=1}^s e(\nu_i'/\nu)f(\nu_i'/\nu) = n.$

#### Corollaire 1 {#ac-vi-s8-thm-2-cor-1 .statement}

Avec les mêmes hypothèses et notations, on suppose de plus $\nu$ discrète et $\mathbf{L}$ séparable. Alors

$$
\sum_{i=1}^s e(\nu_i'/\nu)f(\nu_i'/\nu) = n.
$$

En effet la fermeture intégrale $B$ de $A$ est alors un $A$-module libre de rang $n$, puisque $A$ est principal (Chap. V, § 1, no 6, cor. 2 de la prop. 18).

#### Corollaire 2 {#ac-vi-s8-thm-2-cor-2 .statement}

Soient $K$ un corps, $\nu$ une valuation discrète de $K$ pour laquelle $K$ est complet, et $\mathbf{L}$ une extension de degré fini $n$ de $K$. Alors $\nu$ admet un prolongement $\nu'$ et un seul à $\mathbf{L}$ (à une équivalence près), l’anneau $A'$ de $\nu'$ est un module libre de type fini sur l’anneau $A$ de $\nu$, et l’on a $e(\nu'/\nu)f(\nu'/\nu) = n$.

En effet, tous les prolongements de $\nu$ à $\mathbf{L}$ sont dépendants (no 2, cor. de la prop. 2); puisqu’ils sont discrets (no 1, cor. 3 de la prop. 1), ils sont par conséquent équivalents ($§ 4$, no 5, prop. 6, c)). Ceci démontre l’unicité de $\nu'$. La fermeture intégrale de $A$ dans $\mathbf{L}$ est donc $A'$ ($§ 1$, no 3, cor. 3 du th. 3). Comme $\nu$ est discrète, la topologie induite sur $A$ par celle de $K$ est la topologie $m$-adique (où $m = m(A)$); l’anneau $A$ est complet, car il est fermé dans $K$. On en conclut que, puisque $A'/mA'$ est un $(A/m)$-espace vectoriel de dimension finie (no 4, prop. 4), $A'$ est un $A$-module de type fini (chap. III, § 2; no 9, cor. 3 de la prop. 12). Il est donc libre et l’on a $e(\nu'/\nu)f(\nu'/\nu) = n$ en vertu du th. 2.

#### Corollaire 3 {#ac-vi-s8-thm-2-cor-3 .statement}

Supposons que $\nu$ soit de hauteur 1 et que les conditions équivalentes du th. 2 soient vérifiées; si $\hat{\mathbf{L}}_i$ est le complété de $\mathbf{L}$ pour $\nu_i'$, le degré $n_i = [\hat{\mathbf{L}}_i : \hat{K}]$ est égal à $e(\nu_i'/\nu)f(\nu_i'/\nu)$ pour tout $i$ et l’homomorphisme canonique

$$
\varphi : \hat{K} \otimes_K \mathbf{L} \to \prod_{i=1}^s \hat{\mathbf{L}}_i
$$

(no 2, prop. 2) est bijectif. Pour tout $x \in \mathbf{L}$, le polynôme caractéristique $\mathrm{Pc}_{L/K}(x; X)$ est égal au produit des polynômes caractéristiques $\mathrm{Pc}_{\hat{L}_i/\hat{K}}(x; X)$ ($1 \leq i \leq s$); en particulier, on a

$$
\left\{
\begin{aligned}
\mathrm{Tr}_{L/K}(x) &= \sum_{i=1}^s \mathrm{Tr}_{\hat{L}_i/\hat{K}}(x) \\
\mathrm{N}_{L/K}(x) &= \prod_{i=1}^s \mathrm{N}_{\hat{L}_i/\hat{K}}(x) \\
\varphi(\mathrm{N}_{L/K}(x)) &= \sum_{i=1}^s n_i \varphi_i'(x).
\end{aligned}
\right.
$$

(La dernière relation (9) a un sens, car on peut évidemment supposer que les $\varphi_i'$, qui sont de hauteur 1 en vertu du cor. 2 de la prop. 1 du no 1, prennent, ainsi que $\varphi$, leurs valeurs dans un sous-groupe de $\mathbf{R}$.

Comme les $\varphi_i'$ sont deux à deux inéquivalentes et de hauteur 1, elles sont indépendantes, et la prop. 2 du no 2 montre donc que l’on a $e(\varphi_i'/\varphi)f(\varphi_i'/\varphi) \leq n_i$ pour tout $i$, et $\sum_{i=1}^s n_i \leq n$. La première assertion résulte donc de ces inégalités et de la relation $\sum_{i=1}^s e(\varphi_i'/\varphi)f(\varphi_i'/\varphi) = n$. Par l’isomorphisme $\varphi$, l’endomorphisme $z \to z(1 \otimes x)$ de $\hat{K} \otimes_K L$ (pour $x \in L$) se transporte en l’endomorphisme de $\prod_{i=1}^s \hat{L}_i$ laissant stable chacun des facteurs et se réduisant dans chaque facteur à la multiplication par $x$ (L étant plongé canoniquement dans son complété $\hat{L}_i$); d’où l’assertion relative au polynôme caractéristique de $x$ et les deux premières formules (9). Enfin, soit E une extension quasi-galoisienne de $\hat{K}$ de degré fini, contenant $\hat{L}_i$; comme $\hat{K}$ est complet et $\hat{\varphi}$ de hauteur 1, il n’existe (à une équivalence près) qu’une seule valuation $\varphi$ sur E prolongeant $\hat{\varphi}$ (no 2, cor. 1 de la prop. 2); pour tout $\hat{K}$-automorphisme $\sigma$ de E, on a donc $\varphi(\sigma(x)) = \varphi_i'(x)$. Par suite $\hat{\varphi}(\mathrm{N}_{\hat{L}_i/\hat{K}}(x)) = n_i \varphi_i'(x)$ (Alg., chap. VIII, § 12, no 2, formule (15)), ce qui prouve la troisième formule (9).

#### Corollaire 4 {#ac-vi-s8-thm-2-cor-4 .statement}

Sous les hypothèses du cor. 3, si L est une extension séparable de K, chacun des $\hat{L}_i$ est une extension séparable de $\hat{K}$. Si de plus L est une extension galoisienne de K, de groupe de Galois $G_f$, et si $G_i$ désigne le groupe de décomposition de l’idéal de $\varphi_i'$ dans B (chap. V, § 2, no 2, déf. 2), alors $\hat{L}_i$ est une extension galoisienne de $\hat{K}$, dont le groupe de Galois est isomorphe à $G_i$.

$$
\operatorname{Card}(G_i) = n/s \leq n_i,
$$

et d’autre part $n = sn_i$ en vertu du cor. 3; cela prouve que $\hat{L}_i$ est une extension galoisienne de $\hat{K}$ et que les prolongements par continuité des automorphismes $\sigma \in G_i$ sont les seuls $\hat{K}$-automorphismes de $\hat{L}_i$.

#### Remarque 2 {#ac-vi-s8-n5-rem-2 .statement}

Une partie des résultats précédents s’étend au cas des valuations sur un corps $K$ non nécessairement commutatif (cf. § 3, no 1). Soit $L$ un surcorps de $K$, et soient $\varphi'$ une valuation sur $L$, $\varphi$ sa restriction à $K$, $A'$ et $A$ les anneaux respectifs des valuations $\varphi'$ et $\varphi$; on définit alors l’indice de ramification $e(\varphi'/\varphi)$ comme au no 1; d’autre part, $\kappa(A)$ s’identifie à un sous-corps de $\kappa(A')$, et l’on appelle rang résiduel (à gauche) de $\varphi'$ par rapport à $\varphi$ le nombre $f(\varphi'/\varphi)$ égal à la dimension du $\kappa(A)$-espace vectoriel à gauche $\kappa(A')$, lorsque cette dimension est finie, et $+\infty$ dans le cas contraire. Alors, si $L$ est un $K$-espace vectoriel à gauche de dimension finie $n$, le lemme 2 du no 1 et sa démonstration subsistent sans changement. En outre, si $K$ est complet pour $\varphi$, les assertions du cor. 2 du th. 2 du no 5 (autres que l’existence de $\varphi'$) sont encore valables ($n$ désignant la dimension de $L$ comme $K$-espace vectoriel à gauche) avec la démonstration suivante:

En premier lieu la topologie définie par $\varphi'$ sur $L$ est séparée et compatible avec sa structure de $K$-espace vectoriel à gauche, donc deux prolongements de $\varphi$ à $L$ donnent sur $L$ la même topologie ($§ 5$, no 2, prop. 4), ce qui prouve que ces prolongements sont les mêmes à une équivalence près ($§ 6$, no 2). Montrons ensuite que si $m = m(A)$, $A'/mA'$ est un $(A/m)$-espace vectoriel à gauche

### 6. Anneaux de valuation dans une extension algébrique

#### Proposition 6 {#ac-vi-s8-prop-6 .statement}

Soient $K$ un corps, $\nu$ une valuation de $K$, $A$ son anneau, $L$ une extension algébrique de $K$, $A'$ la fermeture intégrale de $A$ dans $L$. Soient $\mathcal{B}$ l’ensemble des anneaux des valuations de $L$ qui prolongent $\nu$, $\mathcal{M}'$ l’ensemble des idéaux maximaux de $A'$. Alors l’application $V \to m(V) \cap A'$ est une bijection de $\mathcal{B}$ sur $\mathcal{M}'$, et $m' \to A'_{m'}$ est la bijection réciproque.

Tout idéal maximal $m'$ de $A'$ est tel que $m' \cap A$ soit l’idéal maximal $m$ de $A$ (chap. V, § 2, no 1, prop. 1), et $A'_{m'}$ est dominé par un anneau de valuation $V$ de $L$ (qui est donc l’anneau d’une valuation de $L$ prolongeant $\nu$) ($§ 1$, no 2, cor. du th. 2). Le corps $L$ est réunion de la famille filtrante des sous-extensions $K_\alpha$ de $L$ qui sont de degré fini sur $K$, et il suffira, pour voir que $V = A'_{m'}$, de prouver que $V \cap K_\alpha = A'_{m'} \cap K_\alpha$ pour tout $\alpha$. Or, si on pose $A'_\alpha = A' \cap K_\alpha$, $A'_\alpha$ est la fermeture intégrale de $A$ dans $K_\alpha$, donc est intersection des anneaux des valuations de $K_\alpha$ qui prolongent $\nu$, et ces anneaux $V_{i\alpha}$ sont en nombre fini et sont les anneaux locaux $(A'_\alpha)_{m'_{i\alpha}}$ de $A'_\alpha (1 \leq i \leq n)$, où les $m'_{i\alpha}$ sont les idéaux maximaux distincts de $A'_\alpha$ (no 3, Remarque); mais $m' \cap A'_\alpha$ est un des $m'_{i\alpha}$ et $V \cap K_\alpha$ est donc égal à l’anneau local correspondant $(A'_\alpha)_{m'_{i\alpha}} \subset A'_{m'}$, ce qui achève de montrer que

C.Q.F.D.

#### Proposition 7 {#ac-vi-s8-prop-7 .statement}

Soient K un corps, L une extension quasi-galoisienne de K, $f$ et $f'$ des places de L à valeurs dans un même corps F. On suppose que les restrictions de $f$ et $f'$ à K coïncident. Il existe alors un K-automorphisme s de L tel que $f' = f \circ s$.

Soit en effet A l’anneau de la place de K restriction commune de $f$ et $f'$. Les anneaux de $f$ et $f'$ contiennent la fermeture intégrale $A'$ de A dans L (§ 1, n° 3, cor. 3 du th. 3), donc (chap. V, § 2, n° 3, cor. 1 de la prop. 6), il existe un K-automorphisme s de L tel que les restrictions de $f'$ et de $f \circ s$ à $A'$ soient égales; si $m'$ est le noyau commun de ces restrictions, $m' \cap A$ est l’idéal maximal de A, donc $m'$ est un idéal maximal de $A'$ et les places $f'$ et $f \circ s$ coïncident dans l’anneau $A'_{m'}$; mais en vertu de la prop. 6, le seul anneau de valuation de L dominant $A'_{m'}$ est l’anneau $A'_{m'}$ lui-même, donc les anneaux des places $f'$ et $f \circ s$ sont les mêmes.

C.Q.F.D.

#### Corollaire 1 {#ac-vi-s8-prop-7-cor-1 .statement}

Soient K un corps, $\nu$ une valuation de K, L une extension quasi-galoisienne de K, et $\nu', \nu''$ deux extensions de $\nu$ à L. Il existe alors un K-automorphisme s de L tel que $\nu''$ soit équivalente à $\nu' \circ s$.

Soient $f'$ et $f''$ des places de K associées à $\nu'$ et $\nu''$; en les remplaçant au besoin par des places équivalentes, on peut supposer qu’elles prennent toutes deux leurs valeurs dans la clôture algébrique du corps résiduel de $\nu$ (n° 1, prop. 1). Il existe alors un K-automorphisme s de L tel que $f'' = f' \circ s$ (prop. 7); ainsi $\nu''$ est équivalente à $\nu' \circ s$ en vertu de la correspondance entre places et valuations (§ 3, n° 3).

#### Corollaire 2 {#ac-vi-s8-prop-7-cor-2 .statement}

Soient K un corps, $f$ une place (resp. $\nu$ une valuation) de K, et L une extension radicielle de K. Alors toutes les extensions de $f$ (resp. $\nu$) à L sont équivalentes.

En effet L est une extension quasi-galoisienne, et son seul automorphisme est l’identité. Le cor. 2 résulte donc de la prop. 7 (resp. du cor. 1).

#### Proposition 8 {#ac-vi-s8-prop-8 .statement}

Soient K un corps, $\nu$ une valuation de K, L une extension quasi-galoisienne de degré fini n de K, et $(v'_i)_{1 \leq i \leq g}$ un système complet de prolongements de $v$ à L. Alors $e(v'_i/v)$ et $f(v'_i/v)$ ont des valeurs $e$ et $f$ indépendantes de $i$. On a $efg \leq n$. Si la fermeture intégrale dans L de l’anneau A de $v$ est un A-module de type fini, on a $efg = n$.

Ceci résulte aussitôt des th. 1 (no 3) et 2 (no 5).

### 7. Prolongement des valeurs absolues.

#### Proposition 9 {#ac-vi-s8-prop-9 .statement}

Soient K un corps, L une extension algébrique de K, et $f$ une valeur absolue sur K. Alors $f$ se prolonge en une valeur absolue sur L.

Supposons d’abord qu’il existe une valuation $v$ de K à valeurs réelles telle que $f(x) = e^{-v(x)}$. Il existe une valuation $v'$ de L dont la restriction à K est équivalente à $v$ (§ 3, no 3, prop. 5). Alors $v'$ est de hauteur 0 ou 1 (no 1, cor. 2 de la prop. 1), donc peut être supposée à valeurs réelles. La restriction de l’application $x \to e^{-v'(x)}$ à K est une valeur absolue équivalente à $f$, donc de la forme $f^s$ avec $s > 0$ (Top. gén., chap. IX, § 3, no 2, prop. 5). On en conclut que

$$
x \to e^{-v'(x)/s}
$$

est une valeur absolue sur L prolongeant $f$.

Supposons maintenant $f$ non ultramétrique. Alors K s’identifie à un sous-corps de C de manière que $f(x) = |x|^s$ où $0 \leq s \leq 1$ (§ 6, no 4, th. 2). Comme C est algébriquement clos, L s’identifie à un sous-corps de C, et la valeur absolue $x \to |x|^s$ prolonge $f$.

#### Proposition 10 {#ac-vi-s8-prop-10 .statement}

Soient K un corps, $f$ une valeur absolue sur K telle que K soit complet et non discret pour $f$, et L une extension algébrique de K. Alors $f$ se prolonge de manière unique en une valeur absolue $f'$ sur L, et si L est de degré fini $n$, on a $f'(x) = (f(\mathrm{N}_{L/K}(x)))^{1/n}$ pour tout $x \in L$.

L’existence de $f'$ résulte de la prop. 9, et son unicité (sur toute sous-extension de degré fini de L, donc sur L tout entier) du lemme 2 du § 6, no 4. Soit $f'$ l’unique prolongement de $f$ à la clôture algébrique de K, et supposons L de degré fini $n$. On sait que $\mathrm{N}_{L/K}(x) = \prod_{i=1}^n x_i$, où chaque $x_i$ est conjugué de $x$ sur K (Alg., chap. VIII, § 12, no 2, prop. 4). Vu l’unicité de $f'$, on a $f'(x_i) = f'(x)$ pour tout $i$, d’où la formule annoncée.

#### Proposition 11 {#ac-vi-s8-prop-11 .statement}

Soient K un corps, f une valeur absolue non ultramétrique sur K, $\hat{K}$ le complété de K pour f, $\hat{f}$ le prolongement continu de f à $\hat{K}$, et L une extension de degré fini n de K.

a) Soit $f'$ une valeur absolue de L prolongeant f; notons $\hat{L}_{f'}$ le complété de L pour $f'$, et identifions $\hat{K}$ à l’adhérence de K dans $\hat{L}_{f'}$; on a $[\hat{L}_{f'} : \hat{K}] \leq n$.

b) Les valeurs absolues de L prolongeant f sont en nombre fini. Si on les note $f'_1, \ldots, f'_s$, et si l’on désigne par $\hat{L}_i$ le complété de L pour $f'_i$, l’application canonique $\hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i$ est un isomorphisme, et l’on a

$$
\sum_{i=1}^s [\hat{L}_i : \hat{K}] = n.
$$

La démonstration est la même que celle des assertions analogues de la prop. 2 (no 2). On remplace les références

§ 7, no 2, th. 1; § 5, no 2, cor. de la prop. 4

par les suivantes:

§ 7, no 3, th. 2; Esp. Vect. Top., chap. I, § 2, no 3, cor. 1 du th. 2.

On observe que deux prolongements de f à L qui définissent la même topologie sont égaux (Top. gén., chap. IX, § 3, no 2, prop. 5). Enfin, comme f est non ultramétrique, K est de caractéristique 0, donc le radical de $\hat{K} \otimes_K L$ est nul.

#### Remarque 1 {#ac-vi-s8-n7-rem-1 .statement}

La prop. 11 b) montre que toute extension composée de $\hat{K}$ et L sur K est isomorphe à l’un des complétés $\hat{L}_i$, et que ceux-ci sont des extensions composées deux à deux non isomorphes.

#### Remarque 2 {#ac-vi-s8-n7-rem-2 .statement}

Nous savons que les complétés $\hat{K}$ et $\hat{L}_i$ sont isomorphes à $\mathbf{R}$ ou $\mathbf{C}$ (§ 6, no 4, th. 2). Lorsque $\hat{K}$ est isomorphe à $\mathbf{C}$, il en est de même de $\hat{L}_i$ pour tout i, et (10) montre que le nombre des prolongements $f'_i$ est égal à n. Lorsque $\hat{K}$ est isomorphe à $\mathbf{R}$ (par exemple lorsque $K = \mathbf{Q}$), notons $r_1$ (resp. $r_2$) le nombre d’indices i tels que $\hat{L}_i$ soit isomorphe à $\mathbf{R}$ (resp. $\mathbf{C}$); alors (10) s’écrit:

$$
r_1 + 2r_2 = n.
$$

#### Proposition 12 {#ac-vi-s8-prop-12 .statement}

Soient K un corps, f une valeur absolue sur K, L une extension quasi-galoisienne de K, f' et f'' deux prolongements de f à L. Il existe alors un K-automorphisme s de L tel que f'' = f' o s.

Lorsque f est ultramétrique, le cor. 1 de la prop. 7 (n° 6) montre qu’il existe un K-automorphisme s de L tel que f'' et f' o s soient des valeurs absolues équivalentes; il existe alors un nombre réel a > 0 tel que f''(x) = (f'(s(x)))^a pour tout x ∈ L. Si f est non impropre, on prend x ∈ K* tel que f(x) ≠ 1, ce qui montre que a = 1. Si f est impropre, il en est de même de f' et f'' (cor. 2 de la prop. 1, n° 1), et l’on peut prendre pour s l’automorphisme identique.

Si f est non ultramétrique, il existe des Q-isomorphismes u', u'' de L sur des sous-corps de C et des exposants réels a' > 0, a'' > 0 tels que f'(x) = |u'(x)|^{a'} et f''(x) = |u''(x)|^{a''} pour tout x ∈ L (§ 6, n° 4, th. 2). Prenant x = 2, on voit que a' = a''. Les restrictions de u' et u'' à K se prolongent par continuité en des isomorphismes u_1 et u_2 de $\hat{K}$ sur R (resp. C). Alors u_2 o u_1^{-1} est un automorphisme du corps valué R (resp. C), et est donc l’identité (resp. l’identité ou l’automorphisme c : ζ → $\bar{\zeta}$). En remplaçant au besoin u' par c o u', on voit que l’on peut supposer que les restrictions de u' et u'' à K coïncident. Identifiant K à un sous-corps de C au moyen de cette commune restriction, u' et u'' sont des K-isomorphismes de L sur des sous-corps de C. Comme L est extension quasi-galoisienne de K, il existe un K-automorphisme s de L tel que u'' = u' o s; puisque a' = a'', on en déduit aussitôt que f'' = f' o s.

C.Q.F.D.

#### Remarque 3 {#ac-vi-s8-n7-rem-3 .statement}

Lorsque $\hat{K}$ est isomorphe à R, la prop. 12 montre que tous les complétés $\hat{L}_i$ de L (notations de la prop. 11) sont isomorphes entre eux. Ainsi, avec les notations de la Remarque 2) ci-dessus, on a, soit r_1 = n et r_2 = 0, soit r_1 = 0 et 2r_2 = n.

## EXERCICES {#ac-vi-s8-exercises}

See the [exercises for § 8](exercises/s8/).
