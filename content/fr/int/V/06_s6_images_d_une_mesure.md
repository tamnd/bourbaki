---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 6
section_title: Images d'une mesure
lang: fr
source: int-v-fr
pdf_pages: 0073-0086, 0123-0128
extraction: ocr
subsections:
    - "no": 1
      title: '*Image d’une mesure positive*'
      page: 0
      pdf_page: 73
    - "no": 2
      title: Intégration par rapport à l’image d’une mesure positive
      page: 0
      pdf_page: 75
    - "no": 3
      title: Propriétés de l’image d’une mesure positive
      page: 0
      pdf_page: 77
    - "no": 4
      title: Image d’une mesure complexe
      page: 0
      pdf_page: 79
    - "no": 5
      title: 'Application: changement de variable dans l’intégrale de Lebesgue'
      page: 0
      pdf_page: 80
    - "no": 6
      title: Décomposition en tranches. Image réciproque d’une mesure par un homéomorphisme local
      page: 0
      pdf_page: 83
statements: 29
exercises: 22
content_sha256: ee8a61fda4c4bb0770ce4ab749dc8b1788e45276257a9a89a1cabdf019cf6e14
---

## § 6. — Images d’une mesure

### 1. *Image d’une mesure positive*

Soient X un espace localement compact, $\pi$ une application $\mu$-mesurable de T dans X. Dire que le couple $(\pi, 1)$ est $\mu$-adapté (\S 4, n° 1) équivaut à dire que pour toute fonction $f \in \mathcal{K}(X)$ la fonction $f \circ \pi$ est essentiellement $\mu$-intégrable.

#### Proposition 1 {#int-v-s6-prop-1 .statement}

*Soit $\pi$ une application $\mu$-mesurable de T dans un espace localement compact X. Les deux propriétés suivantes sont équivalentes :

a) pour toute fonction $f \in \mathcal{K}(X)$, $f \circ \pi$ est essentiellement $\mu$-intégrable ;

b) pour tout ensemble compact $K \subset X$, $\pi^{-1}(K)$ est essentiellement $\mu$-intégrable.

Nous venons de remarquer que a) entraîne que le couple $(\pi, 1)$ est $\mu$-adapté. Par suite (\S 4, n° 4, th. 2), pour tout ensemble compact $K \subset X$, la fonction $\varphi_K \circ \pi = \varphi_A$, où $A = \pi^{-1}(K)$, est essentiellement $\mu$-intégrable, autrement dit, a) entraîne b).

Inversement, supposons que $\pi^{-1}(K)$ soit essentiellement $\mu$-intégrable pour toute partie compacte K de X, et montrons que a) est vérifiée. Soit en effet S le support de $f$; comme S est compact, on a, par hypothèse, en posant $A = \pi^{-1}(S)$

$$
\int |f(\pi(t))| d\mu(t) \leq \|f\| \int \varphi_S(\pi(t)) d\mu(t) = \|f\| \int \varphi_A(t) d\mu(t) < +\infty.
$$

Comme $f \circ \pi$ est $\mu$-mesurable (chap. IV, § 5, n° 3, th. 1), on voit que $f \circ \pi$ est essentiellement $\mu$-intégrable ($\S 1, n° 3,$ prop. 9).

La propriété b) est évidemment équivalente à la propriété suivante (qui équivaut donc aussi à a)):
c) Pour tout point x de X, il existe un voisinage V de X tel que $\pi^{-1}(V)$ soit essentiellement $\mu$-intégrable.

#### Définition 1 {#int-v-s6-def-1 .statement}

Soit $\mu$ une mesure positive sur un espace localement compact T. On dit qu’une application $\pi$ de T dans un espace localement compact X est $\mu$-propre (ou propre pour la mesure $\mu$) si le couple $(\pi, 1)$ est $\mu$-adapté, c’est-à-dire ($\S 4, n° 1$) si $\pi$ est $\mu$-mesurable et satisfait aux conditions (équivalentes) de la prop. 1. La mesure $\int \varepsilon_{\pi(t)} d\mu(t)$ sur X s’appelle alors l’image de $\mu$ par $\pi$ et se note $\pi(\mu)$.

Si $v = \pi(\mu)$, on a donc, par définition, pour $f \in \mathcal{K}(X)$

$$
\int f(x) dv(x) = \int f(\pi(t)) d\mu(t).
$$

#### Remarque 1 {#int-v-s6-n1-rem-1 .statement}

Si $\mu$ est bornée (et en particulier si $\mu$ a un support compact), toute application $\mu$-mesurable de T dans X est $\mu$-propre (chap. IV, § 5, n° 3, th. 1 et n° 6, th. 5).
2) Si $\pi$ est $\mu$-mesurable et si, pour toute partie compacte K de X, $\pi^{-1}(K)$ est relativement compact, $\pi$ est $\mu$-propre (chap. IV, 2e éd., § 5, n° 5, prop. 7, et n° 6, th. 5); en particulier, toute application continue propre de T dans X (Top. gén., chap. I, 4e éd., § 10, n° 2, th. 1) est $\mu$-propre pour toute mesure positive $\mu$ sur T. Plus particulièrement, il en est ainsi de tout homéomorphisme $\pi$ de T sur X; la mesure $v = \pi(\mu)$ n’est autre alors que la mesure sur X transportée de $\mu$ par $\pi$ (chap. III, 2e éd., § 1, n° 3).
3) Supposons que la topologie de X admette une base dénombrable; alors toute application $\pi$ de T dans X qui vérifie

### 2. Intégration par rapport à l’image d’une mesure positive

Soit $\pi$ une application $\mu$-propre de T dans X, et soit $\nu = \pi(\mu)$. En appliquant les résultats du § 4, on obtient les énoncés suivants :

#### Proposition 2 {#int-v-s6-prop-2 .statement}

Pour toute fonction numérique $f \geqslant 0$ définie dans X, on a

$$
\int^\ast f(x)\, d\nu(x) = \int^\ast f(\pi(t))\, d\mu(t).
$$

(2)

Cela résulte du th. 1 du § 4, n° 2.

#### Corollaire 1 {#int-v-s6-prop-2-cor-1 .statement}

Pour toute partie A de X, on a

$$
\nu^\ast(A) = \mu^\ast(\overline{\pi^{-1}(A)}).
$$

#### Corollaire 2 {#int-v-s6-prop-2-cor-2 .statement}

Pour qu’une partie A de X soit localement négligeable pour $\nu$, il faut et il suffit que $\overline{\pi^{-1}(A)}$ soit localement négligeable pour $\mu$.

#### Corollaire 3 {#int-v-s6-prop-2-cor-3 .statement}

Si la mesure $\mu$ est concentrée sur un ensemble M, $\pi(\mu)$ est concentrée sur $\pi(M)$.
En effet, si $N = X - \pi(M)$, $\overline{\pi^{-1}(N)}$ ne rencontre pas M, donc est localement $\mu$-négligeable, et par suite (cor. 2) N est localement $\nu$-négligeable.

#### Corollaire 4 {#int-v-s6-prop-2-cor-4 .statement}

Soit S le support de $\mu$. Si $\pi$ est continue, le support de $\pi(\mu)$ est $\overline{\pi(S)}$.
En effet, il résulte du cor. 3 que $\pi(\mu)$ est concentrée sur $\pi(S)$, donc, si $S'$ est le support de $\pi(\mu)$, on a $S' \subset \overline{\pi(S)}$. D’autre part, $
\overline{\pi}^{-1}(X - S')$ est un ensemble ouvert localement $\mu$-négligeable (cor. 2), donc $\mu$-négligeable (chap. IV, § 5, n° 2, cor. 2 de la prop. 5).

On a donc $\overline{\pi}^{-1}(X - S') \subset T - S$ et par suite $\pi(S) \subset S'$, ce qui démontre le corollaire.

#### Proposition 3 {#int-v-s6-prop-3 .statement}

*Pour qu’une application $f$ de $X$ dans un espace topologique $G$ soit $\nu$-mesurable, il faut et il suffit que $f \circ \pi$ soit $\mu$-mesurable.*

C’est une conséquence immédiate de la prop. 3 du § 4, n° 3.

#### Corollaire {#int-v-s6-n2-cor-1 .statement}

*Pour qu’une partie $A$ de $X$ soit $\nu$-mesurable, il faut et il suffit que $\overline{\pi}^{-1}(A)$ soit $\mu$-mesurable.*

Par contre, l’image par $\pi$ d’une partie $\mu$-mesurable $M$ de $T$ n’est pas nécessairement $\nu$-mesurable, même si $\pi$ est continue et $M$ $\mu$-négligeable (exerc. 7 et § 8, exerc. 1).

#### Théorème 1 {#int-v-s6-thm-1 .statement}

*Soit $f$ une fonction définie dans $X$, à valeurs dans $\bar{\mathbf{R}}$ ou dans un espace de Banach $F$. Pour que $f$ soit essentiellement $\nu$-intégrable, il faut et il suffit que $f \circ \pi$ soit essentiellement $\mu$-intégrable, et l’on a alors*

$$
\int f(x)\ dv(x) = \int f(\pi(t))\ d\mu(t).
$$

Supposons en outre que $\pi$ soit continue et propre. *Pour que $f$ soit $\nu$-intégrable, il faut et il suffit alors que $f \circ \pi$ soit $\mu$-intégrable.*

Il suffit d’appliquer le th. 2 du § 4, n° 4.

#### Corollaire {#int-v-s6-n2-cor-2 .statement}

*Pour qu’une partie $A$ de $X$ soit essentiellement $\nu$-intégrable, il faut et il suffit que $\overline{\pi}^{-1}(A)$ soit essentiellement $\mu$-intégrable, et on a alors $\nu(A) = \mu(\overline{\pi}^{-1}(A))$.*

En particulier, pour tout ensemble compact $K \subset X$, on a $\nu(K) = \mu(\overline{\pi}^{-1}(K))$. Il résulte de là et du cor. 3 de la prop. 2 que, si $\mu$ est *atomique* ($\S 5$, n° 10), il en est de même de $\pi(\mu) = \nu$. En effet, soit $M$ l’ensemble des $t \in T$ tels que $\mu(\{t\}) \neq 0$; comme $\mu$ est portée par $M$, $\nu$ est portée par $\pi(M)$; en outre, pour tout $x \in \pi(M)$, on a $\nu(\{x\}) = \mu(\overline{\pi}^{-1}(x)) > 0$, puisque $\overline{\pi}^{-1}(x)$ contient au moins un point de $M$. Donc $\nu$ est atomique ($\S 5$, n° 10, prop. 15).

### 3. Propriétés de l’image d’une mesure positive

#### Proposition 4 {#int-v-s6-prop-4 .statement}

Soient T, T', T'' trois espaces localement compacts, μ une mesure positive sur T, π une application μ-mesurable de T dans T', π' une application de T' dans T'', et π'' = π' ∘ π.

a) Supposons que π soit μ-propre et soit μ' = π(μ). Pour que π' soit μ'-propre, il faut et il suffit que π'' soit μ-propre, et on a alors π''(μ) = π'(π(μ)) (« transivité de l’image d’une mesure »).

b) Supposons que π' soit continue, et que π'' soit μ-propre ; π est alors μ-propre, π' est π(μ)-propre, et on a π''(μ) = π'(π(μ)).

Sous les hypothèses de a), pour que π'' soit μ-mesurable, il faut et il suffit que π' soit μ'-mesurable (n° 2, prop. 3). D’autre part, si K est une partie compacte de T'', on a ${\pi''}^{-1}(K) = {\pi'}^{-1}(\pi'(K))$; pour que ${\pi''}^{-1}(K)$ soit essentiellement μ-intégrable, il faut et il suffit que ${\pi'}^{-1}(K)$ soit essentiellement μ'-intégrable, en vertu du cor. du th. 1. Enfin, si π'' est μ-propre, en posant $\mu'' = \pi''(\mu)$, on a, pour toute fonction $f \in \mathcal{K}(T'')$,

$$
\int f(t'')\,d\mu''(t'') = \int f(\pi''(t))\,d\mu(t)
$$
$$
= \int f(\pi'(\pi(t)))\,d\mu(t) = \int f(\pi'(t'))\,d\mu'(t')
$$

en vertu du th. 1 du n° 2, ce qui achève la démonstration de a).

Sous les hypothèses de b), soit K' une partie compacte de T'. Alors $K'' = \pi'(K')$ est compact, donc ${\pi''}^{-1}(K'')$ est essentiellement μ-intégrable, donc ${\pi'}^{-1}(K') \subset {\pi''}^{-1}(K'')$ est essentiellement μ-intégrable (chap. IV, 2e éd., § 5, n° 5, prop. 7), de sorte que π est μ-propre. On achève alors en appliquant la partie a) de l’énoncé.

#### Corollaire {#int-v-s6-n3-cor-1 .statement}

Soient T et T' deux espaces localement compacts, μ une mesure positive sur T, π une application bijective de T sur T', ${\pi'}^{-1}$ l’application réciproque. Supposons que π soit μ-propre, et soit $\mu' = \pi(\mu)$. Alors ${\pi'}^{-1}$ est μ'-propre et on a ${\pi'}^{-1}(\pi(\mu)) = \mu$.

#### Proposition 5 {#int-v-s6-prop-5 .statement}

Soient T et X deux espaces localement compacts, μ une mesure positive sur T, π une application μ-propre de T dans X, g une fonction numérique finie et $\geq 0$, définie dans X et telle que $g \circ \pi$ soit localement intégrable pour μ. Pour que g soit localement intégrable pour $\pi(\mu)$, il faut et il suffit que π soit propre pour la mesure $(g \circ \pi) . \mu$, et on a alors

$$
\pi((g \circ \pi) . \mu) = g . \pi(\mu).
$$

$$
\int fg\, d\nu = \int f(\pi(t))g(\pi(t))\, d\mu(t) = \int f(\pi(t))\, d\rho(t)
$$

(n° 2, th. 1 et § 5, th. 1), ce qui prouve la relation (4).

#### Proposition 6 {#int-v-s6-prop-6 .statement}

Soient $T$ et $X$ deux espaces localement compacts, $(\lambda_\alpha)_{\alpha \in A}$ une famille de mesures positives sur $T$, filtrante pour la relation $\leqslant$, admettant dans $\mathcal{M}(T)$ une borne supérieure $\mu$. Pour qu’une application de $T$ dans $X$ soit $\mu$-propre, il faut et il suffit qu’elle soit $\lambda_\alpha$-propre pour tout $\alpha \in A$, et que la famille $(\pi(\lambda_\alpha))_{\alpha \in A}$ soit majorée dans $\mathcal{M}(X)$. Dans ce cas, on a

(5)
$$
\pi(\mu) = \sup_\alpha \pi(\lambda_\alpha).
$$

Pour que $\pi$ soit $\mu$-mesurable, il faut et il suffit que $\pi$ soit $\lambda_\alpha$-mesurable pour tout $\alpha \in A$ (§1, n° 4, cor. 2 de la prop. 11). Supposons cette condition satisfaite; dire que $\pi$ est $\mu$-propre équivaut alors à dire qu’on a, pour toute fonction $f \in \mathcal{K}_+(T)$,

$$
\mu^*(f \circ \pi) < +\infty.
$$

Or on a

$$
\int^\ast (f \circ \pi)\, d\mu = \sup_\alpha \int^\ast (f \circ \pi)\, d\lambda_\alpha = \sup_\alpha \int^\ast f\, d(\pi(\lambda_\alpha))
$$

(§ 1, n° 4, prop. 11); le premier membre est donc fini pour toute $f \in \mathcal{K}_+(T)$ si et seulement si la famille $(\pi(\lambda_\alpha))$ admet une borne supérieure $\theta$ dans $\mathcal{M}(X)$, et on a alors $\int (f \circ \pi)\, d\mu = \int f\, d\theta$, relation équivalente à (5).

#### Corollaire 1 {#int-v-s6-prop-6-cor-1 .statement}

Soit $(\mu_\alpha)_{\alpha \in A}$ une famille sommable de mesures positives sur $T$, telle que $\mu = \sum_{\alpha \in A} \mu_\alpha$; pour qu’une application $\pi$ de $T$ dans un espace localement compact $X$ soit $\mu$-propre, il faut et il suffit qu’elle soit $\mu_\alpha$-propre pour tout $\alpha \in A$, et que la famille

$(\pi(\mu_\alpha))_{\alpha \in \Lambda}$ soit sommable. On a dans ce cas
$$(6)$$
$$
\pi(\mu) = \sum_{\alpha \in \Lambda} \pi(\mu_\alpha).
$$

#### Corollaire 2 {#int-v-s6-prop-6-cor-2 .statement}

Soient $T$ et $X$ deux espaces localement compacts, $(\lambda_i)_{1 \leq i \leq n}$ une suite finie de mesures positives sur $T$, et soit $\mu = \sum_{i=1}^n \lambda_i$. Pour qu’une application $\pi$ de $T$ dans $X$ soit $\mu$-propre, il faut et il suffit qu’elle soit $\lambda_i$-propre pour chaque indice $i$, et on a alors
$$
\sum_{i=1}^n \pi(\lambda_i) = \pi\left( \sum_{i=1}^n \lambda_i \right).
$$

### 4. Image d’une mesure complexe

Soit $\theta$ une mesure complexe sur $T$, et soit $\pi$ une application de $T$ dans un espace localement compact $X$ : supposons que $\pi$ soit $\theta$-mesurable, et que pour chaque $f \in \mathcal{K}(X; \mathbf{C})$, $f \circ \pi$ soit essentiellement $\theta$-intégrable. Comme il est équivalent de dire qu’une fonction est mesurable (resp. essentiellement intégrable) par rapport à $\theta$ ou par rapport à $|\theta|$, cela signifie que $\pi$ est $|\theta|$-propre. Si $f \in \mathcal{K}(X; \mathbf{C})$, on a
$$(7)$$
$$
\left| \int (f \circ \pi) \, d\theta \right| \leq \int (|f| \circ \pi) \, d|\theta|;
$$
il en résulte aussitôt que la forme linéaire $f \mapsto \int (f \circ \pi) \, d\theta$ sur $\mathcal{K}(X; \mathbf{C})$ est une mesure complexe sur $X$ (chap. III, 2e éd., § 1, no 3, prop. 6), et on peut poser la définition suivante:

#### Définition 2 {#int-v-s6-def-2 .statement}

Soit $\theta$ une mesure complexe sur un espace localement compact $T$. On dit qu’une application $\pi$ de $T$ dans un espace localement compact $X$ est $\theta$-propre si elle est $|\theta|$-propre. La mesure $f \mapsto \int (f \circ \pi) \, d\theta$ s’appelle alors l’image de $\theta$ par $\pi$ et se note $\pi(\theta)$.

La relation (7) se met alors sous la forme:
$$(8)$$
$$
|\pi(\theta)| \leq \pi(|\theta|).
$$

La mesure $\pi(\theta)$ peut être nulle sans que $\theta$ le soit, comme on le voit immédiatement en prenant pour $T$ un espace réduit à deux points $a, b$, pour $\theta$ la mesure $\varepsilon_a - \varepsilon_b$, pour $\pi$ une application constante.

Soient $\theta$ et $\theta'$ deux mesures complexes sur $T$; si $\pi$ est $\theta$-propre et $\theta'$-propre, il résulte du cor. 2 de la prop. 6 que $\pi$ est $(\theta + \theta')$-propre, car on a $|\theta + \theta'| \leq |\theta| + |\theta'|$, et on a évidemment $\pi(\theta + \theta') = \pi(\theta) + \pi(\theta')$.

En particulier, si $\theta$ est une mesure réelle, et si $\pi$ est $\theta$-propre, on a

$$
\pi(\theta) = \pi(\theta^+) - \pi(\theta)^-.
$$

Plusieurs résultats établis plus haut s’étendent aussitôt aux mesures complexes; nous citerons les plus importants.

#### Proposition 7 {#int-v-s6-prop-7 .statement}

*Soient $\theta$ une mesure complexe sur $T$, $\pi$ une application $\theta$-propre de $T$ dans un espace localement compact $X$, $\nu$ la mesure image $\pi(\theta)$.*

a) *Soit $A$ une partie de $X$; si $\overline{\pi}^1(A)$ est localement $\theta$-négligeable, $A$ est localement $\nu$-négligeable.*

b) *Soit $f$ une application de $X$ dans un espace topologique; si $f \circ \pi$ est $\theta$-mesurable, $f$ est $\nu$-mesurable.*

c) *Soit $f$ une fonction définie dans $X$, à valeurs dans un espace de Banach $F$; si $f \circ \pi$ est essentiellement $\theta$-intégrable, $f$ est essentiellement $\nu$-intégrable et on a*

$$
\int f(\pi(t))\ d\theta(t) = \int f(x)\ d\nu(x).
$$

Compte tenu de la formule (8), ces résultats se déduisent du cor. 2 de la prop. 2, de la prop. 3, et du th. 1 du n° 2.

### 5. Application: changement de variable dans l’intégrale de Lebesgue

Soient $I$ un intervalle (borné ou non) de $\mathbf{R}$, $a$ son origine, $b$ son extrémité dans $\bar{R}$, $\mu$ la mesure de Lebesgue dans $I$. Pour toute fonction $\mu$-intégrable $f$ et tout intervalle $H \subset I$, d’origine $\alpha$ et d’extrémité $\beta$, nous écrirons $\int_{\alpha}^{\beta} f(t)\ dt$ au lieu de $\int_H f(t)\ dt = \int_H f\ d\mu$, et nous poserons $\int_{\beta}^{\alpha} f(t)\ dt = - \int_{\alpha}^{\beta} f(t)\ dt$; la signification ainsi donnée à ces symboles coïncide avec celle qui leur a été attribuée dans *Fonct. var. réelle*, chap. II, §§ 1 et 2, lorsque $f$ est une fonction réglée à support compact (chap. IV, § 4, n° 4, *Exemple*).

Soient $g$ une fonction numérique définie dans $I$ et *localement* $\mu$-intégrable, $x_0$ un point de $I$; pour tout $x \in I$, posons

$$
G(x) = c + \int_{x_0}^{x} g(t)\, dt \tag{11}
$$
*(c constante)*.

La fonction numérique $G$ est *continue* dans $I$; cela résulte aussitôt du th. de Lebesgue (chap. IV, § 4, n° 3, cor. 1 du th. 2), car le produit de $g$ et de la fonction caractéristique de l’intervalle d’extrémités $x$ et $x + h$ tend vers une fonction négligeable lorsque $h$ tend vers 0. Donc $G(I)$ est un *intervalle* de $\mathbf{R}$. Dans tout ce n°, on considérera $G$ comme une application de $I$ sur l’espace localement compact $G(I)$. On désignera par $\lambda$ la mesure $g . \mu$ sur $I$.

Supposons d’abord que $g$ soit $\mu$-intégrable. Alors, le même raisonnement que ci-dessus montre que les limites $G(a+)$ et $G(b-)$ existent et sont *finies*; en outre, la mesure $|\lambda|$ est *bornée* ($\S 5$, n° 3, cor. du th. 1), et l’application $G$ de $I$ dans $G(I)$ est *$\lambda$-propre*.

#### Proposition 8 {#int-v-s6-prop-8 .statement}

*Supposons* $g$ $\mu$-intégrable. *Si* $J$ *désigne l’intervalle ouvert de* $\mathbf{R}$ *d’extrémités* $G(a+)$ *et* $G(b-)$, *l’image par* $G$ *de la mesure* $g . \mu$ *est la mesure* $\varphi_J . \nu$ *si* $G(a+) \leq G(b-)$ *et la mesure* $-\varphi_J . \nu$ *si* $G(a+) \geq G(b-)$ (*$\nu$ désignant la mesure de Lebesgue sur* $G(I)$).

Il suffit de prouver que, pour toute fonction $f \in \mathcal{K}(G(I))$, on a

$$
\int_{G(a+)}^{G(b-)} f(\xi)\, d\xi = \int_a^b f(G(t))g(t)\, dt. \tag{12}
$$

Or, cette formule a déjà été démontrée lorsque $g \in \mathcal{K}(I)$ (*Fonct. var. réelle*, chap. II, § 2, n° 1, formule (1)). Passons au cas général; il existe une suite $(g_n)$ de fonctions de $\mathcal{K}(I)$ telle que: 1° la suite $(g_n(t))$ tende vers $g(t)$ presque partout dans $I$; 2° il existe une fonction $\mu$-intégrable $h \geq 0$ telle que $|g_n| \leq h$ pour tout $n$ (chap. IV, § 3, n° 4, th. 3). Il résulte aussitôt du th. de Lebesgue que, si on pose $G_n(x) = c + \int_{x_0}^x g_n(t)\, dt$, la suite $(G_n)$ converge *uniformément* vers $G$ dans $I$, et que les nombres $G_n(a+)$ et $G_n(b-)$ tendent respectivement vers $G(a+)$ et $G(b-)$. Soit $f'$ une fonction de $\mathcal{K}(\mathbf{R})$ prolongeant $f$; ce qui précède prouve que $f'(G_n(t))$ tend vers $f'(G(t)) = f(G(t))$ pour tout $t \in I$; appliquant le th. de

Lebesgue, on voit que la formule (12) résulte de la formule

$$
\int_{G_n(a+)}^{G_n(b-)} f'(\xi)\, d\xi = \int_a^b f'(G_n(t))g_n(t)\, dt
$$

par passage à la limite.

#### Corollaire {#int-v-s6-n5-cor-1 .statement}

Si une fonction $f$ définie dans $G(I)$, à valeurs dans $\bar{\mathbf{R}}$ ou dans un espace de Banach, est telle que la fonction $t \mapsto f(G(t))g(t)$ soit intégrable dans $I$ pour la mesure de Lebesgue, alors $f$ est intégrable dans $J$ pour la mesure de Lebesgue et on a (formule du changement de variable dans l’intégrale de Lebesgue)

(13)
$$
\int_{G(a+)}^{G(b-)} f(\xi)\, d\xi = \int_a^b f(G(t))g(t)\, dt.
$$

En effet, $f(G(t))$ est intégrable pour la mesure $|g|\cdot \mu$, donc aussi pour les mesures $g^+\cdot \mu$ et $g^-\cdot \mu$; il résulte du th. 1 (n° 2) que $f$ est intégrable pour les mesures images $G(g^+\cdot \mu)$ et $G(g^-\cdot \mu)$, donc aussi pour la mesure $\varphi_j\cdot v$ et que l’on a (13), compte tenu de la prop. 8 et de la formule (9).

Il peut se faire que $f$ soit intégrable dans $J$ pour la mesure de Lebesgue, mais que $t \mapsto f(G(t))g(t)$ ne soit pas intégrable dans $I$ pour la mesure de Lebesgue (exerc. 10).

Supposons maintenant que $g$ garde presque partout un signe constant (et soit localement $\mu$-intégrable); on peut par exemple supposer $g(t) \geq 0$ presque partout dans $I$. Alors $G$ est une fonction continue croissante dans $I$, donc $G(a+)$ et $G(b-)$ existent (mais peuvent être infinis). En outre, $G$ est une application $\lambda$-propre de $I$ dans $G(I)$: en effet, si $G(b-) \in G(I)$, il y a un $x_1 \geq x_0$ tel que $G$ soit constant pour $x \geq x_1$, et alors l’image réciproque par $G$ de l’intervalle compact $[G(x_0), G(b-)]$ est $\lambda$-intégrable; si au contraire $G(b-) \notin G(I)$, l’image réciproque par $G$ de tout intervalle compact d’origine $G(x_0)$, contenu dans $G(I)$, est un intervalle compact. On raisonne de même pour les intervalles compacts d’extrémité $G(x_0)$, d’où notre assertion. En outre:

#### Proposition 9 {#int-v-s6-prop-9 .statement}

Supposons $g \geq 0$ et localement $\mu$-intégrable. Alors, l’image par $G$ de la mesure positive $g\cdot \mu$ est la mesure de Lebesgue sur $G(I)$. Pour qu’une fonction $f$, définie dans $G(I)$, à valeurs dans $\bar{\mathbf{R}}$ ou dans un espace de Banach, soit intégrable dans $G(I)$ pour la mesure de Lebesgue, il faut et il suffit que la fonction t \mapsto f(G(t))g(t) soit intégrable dans I pour la mesure de Lebesgue, et on a la relation (13).

La première partie de l’énoncé résulte de ce que la formule (12) est valable pour toute fonction $f \in \mathscr{K}(G(I))$; en effet, le support de la fonction $t \mapsto f(G(t))$ est contenue dans un intervalle $K \subset I$ dans lequel $g$ est intégrable, en vertu des remarques faites ci-dessus, et il suffit d’appliquer à $K$ la prop. 8. La seconde partie est conséquence du th. 1 du n° 2.

### 6. Décomposition en tranches. Image réciproque d’une mesure par un homéomorphisme local

Soient $X$ un espace localement compact, $\pi$ une application de $X$ dans un espace localement compact $T$, $\mu$ une mesure positive sur $T$, $\Lambda : t \mapsto \lambda_t$ une application scalairement essentiellement $\mu$-intégrable et vaguement $\mu$-mesurable de $T$ dans $\mathcal{M}_+(X)$. Soit $v = \int \lambda_t\, d\mu(t)$. Si $\lambda_t$ est portée par $\bar{\pi}^1(t)$ pour tout $t \in T$, on dit que l’égalité $v = \int \lambda_t\, d\mu(t)$ est une décomposition en tranches (ou une désintégration) de $v$ relativement à $\pi$. Cette notion sera étudiée de manière détaillée au chap. VI.

#### Proposition 10 {#int-v-s6-prop-10 .statement}

On conserve les notations ci-dessus, et on suppose que $\pi$ est $v$-mesurable. Soit $g$ la fonction $t \mapsto \lambda_t^*(1)$ sur $T$. Pour que $\pi$ soit $v$-propre, il faut et il suffit que $g$ soit localement $\mu$-intégrable, et on a dans ce cas

$$
\pi(v) = g \cdot \mu.
$$

Nous commencerons par raisonner en supposant que $g$ est finie localement $\mu$-presque partout; nous nous débarrasserons de cette hypothèse auxiliaire à la fin de la démonstration. Comme $\pi$ est $v$-mesurable par hypothèse, dire que $\pi$ est $v$-propre équivaut à dire que $v^*(f \circ \pi) < +\infty$ pour toute fonction $f \in \mathscr{K}_+(T)$; $g$ étant finie localement presque partout, on est dans les conditions d’application de l’assertion c), prop. 5 du § 3, n° 2. On a donc

$$
\int^\ast (f \circ \pi)\, dv = \int^\ast d\mu(t) \int^\ast (f \circ \pi)\, d\lambda_t = \int^\ast f(t)g(t)\, d\mu(t),
$$

du fait que $\lambda_t$ est concentrée sur $\bar{\pi}^1(t)$. On sait que $g$ est $\mu$-mesurable, puisque $\Lambda$ est $\mu$-adéquate (\S 3, n° 1, déf. 1). Dire que le premier membre est fini pour toute $f \in \mathscr{K}_+(T)$ équivaut donc à dire que $g$ est localement $\mu$-intégrable (\S 5, prop. 1), et (14) résulte aussitôt dans ce cas des relations ci-dessus.

Il nous reste donc seulement à éliminer l’hypothèse auxiliaire. Si g est localement $\mu$-intégrable, g est finie localement $\mu$-presque partout, et l’hypothèse est bien satisfaite. Supposons que $\pi$ soit $\nu$-propre, et montrons que g est finie localement presque partout. Soit $\mathfrak{R}$ l’ensemble $\mu$-dense des compacts K tels que $\Lambda|K$ soit vaguement continue; comme g est $\mu$-mesurable, on est ramené à montrer que tout compact $K \in \mathfrak{R}$, tel que $g|K = +\infty$, est $\mu$-négligeable. Or soit $\mathcal{H}$ l’ensemble des fonctions $h \in \mathcal{K}_+(X)$ telles que $h \leq 1$; posons $g_h(t) = \lambda_t(h)$, désignons par $\Lambda_h$ l’application $\mu$-adéquate $t \mapsto h \cdot \lambda_t$, par $\nu_h$ l’intégrale de $\Lambda_h$, par $f$ un élément de $\mathcal{K}_+(T)$ tel que $f \geq \varphi_K$. Si nous appliquons la formule (14) à $\Lambda_h$, qui satisfait à l’hypothèse auxiliaire, nous obtenons:

$$
\int (f \circ \pi) \, d\nu \geq \int (f \circ \pi) \, d\nu_h = \int fg_h \, d\mu.
$$

Mais les fonctions $fg_h|K$ forment un ensemble filtrant croissant de fonctions continues sur K, dont l’enveloppe supérieure vaut $+\infty$: d’après le th. de Dini (Top. gén., chap. X, 2e éd., § 4, n° 1, th. 1), on peut choisir h de telle sorte que $fg_h|K$ soit supérieure à un nombre positif arbitraire n, et il vient $\int (f \circ \pi) \, d\nu \geq n \mu(K)$. Le premier membre étant fini du fait que $\pi$ est $\nu$-propre, on en déduit que $\mu(K) = 0$.

#### Corollaire 1 {#int-v-s6-prop-10-cor-1 .statement}

Supposons que $\pi$ soit $\nu$-mesurable.

a) Si $N \subset T$ est localement $\mu$-négligeable, $\bar{\pi}^{-1}(N)$ est localement $\nu$-négligeable.

b) Si $f$ est une application $\mu$-mesurable de T dans un espace topologique G, $f \circ \pi$ est $\nu$-mesurable.

Reprenons les notations $\Lambda_h$, $\nu_h$, $g_h$ de la fin de la démonstration précédente: $\nu_h$ étant une mesure bornée pour tout $h \in \mathcal{H}$, $\pi$ est $\nu_h$-propre, $g_h$ est localement $\mu$-intégrable, et $\pi(\nu_h) = g_h \cdot \mu$, mesure de base $\mu$. Il en résulte que N est localement négligeable (resp. que $f$ est mesurable) pour la mesure $\pi(\nu_h)$ ($\S 5$, n° 3, cor. 1 de la prop. 3 et cor. de la prop. 4). Par conséquent, $\bar{\pi}^{-1}(N)$ est localement négligeable (resp. $f \circ \pi$ est mesurable) pour la mesure $\nu_h$ (cor. 2 de la prop. 2, resp. prop. 3). On remarque enfin que les mesures $\nu_h$ forment une famille filtrante croissante de mesures positives, dont la borne supérieure est $\nu$ ($\S 3$, n° 1, prop. 1), et on applique le cor. 1 (resp. 2) de la prop. 11 du $\S 1$, n° 4.

#### Corollaire 2 {#int-v-s6-prop-10-cor-2 .statement}

Supposons que $\pi$ soit $v$-propre; soit $f$ une application définie dans $T$, à valeurs dans un espace de Banach ou dans $\bar{\mathbf{R}}$. Pour que $f \circ \pi$ soit essentiellement $v$-intégrable, il faut et il suffit que $gf$ soit essentiellement $\mu$-intégrable.

Cela résulte immédiatement, compte tenu de la prop. 10, du th. 1 du § 5, n° 3 et du th. 1 du n° 2.

#### Exemple {#int-v-s6-n6-exa-1 .statement}

Soient $X$ et $T$ deux espaces localement compacts, et soit $\pi$ un homéomorphisme local de $X$ dans $T$. Autrement dit (Top. gén., chap. XI), nous supposons que tout point $x \in X$ admet un voisinage $V$ tel que $\pi|V$ soit un homéomorphisme de $V$ sur un voisinage de $\pi(x)$; quitte à remplacer $V$ par un voisinage ouvert relativement compact $W$ de $x$ tel que $\overline{W} \subset V$, on en déduit que l’ensemble $\mathcal{U}$ des ouverts relativement compacts $U$ de $X$, tels que $\pi|\overline{U}$ soit un homéomorphisme de $\overline{U}$ sur son image, est un recouvrement ouvert de $X$. Soit alors $\mu$ une mesure positive sur $T$; si $U$ est un élément de $\mathcal{U}$, $\pi(U)$ est un ouvert de l’espace compact $\pi(\overline{U})$, donc un sous-espace localement compact de $T$, et on sait définir la mesure $\mu|\pi(U)$ induite par $\mu$ sur $\pi(U)$ (chap. IV, 2e éd., § 5, n° 7). Soit $\nu_U$ l’image de $\mu|\pi(U)$ par l’homéomorphisme réciproque de $\pi|U$; nous allons montrer qu’il existe sur $X$ une mesure $\nu$ et une seule qui induit la mesure $\nu_U$ sur tout ouvert $U \in \mathcal{U}$. Cette mesure est appelée l’image réciproque de $\mu$ par l’homéomorphisme local $\pi$, et notée $\overline{\pi}^1(\mu)$.

L’unicité de $\nu$ résulte aussitôt du principe de localisation (chap. III, 2e éd., § 2, n° 1, cor. de la prop. 1). Pour établir l’existence notons que si $t \in T$, tout point $x \in \overline{\pi}^1(t)$ admet un voisinage qui ne rencontre $\overline{\pi}^1(t)$ qu’au point $x$, de sorte que $\overline{\pi}^1(t)$ est un sous-espace discret de $X$, et que la famille $(\varepsilon_x)_{x \in \overline{\pi}^1(t)}$ est sommable; désignons par $\lambda_t$ sa somme. Montrons ensuite que l’application $t \mapsto \lambda_t$ est scalairement essentiellement $\mu$-intégrable, et que son intégrale $\nu = \int \lambda_t \, d\mu(t)$ est l’image réciproque cherchée. Cela résultera aussitôt du lemme suivant:

#### Lemme 1 {#int-v-s6-lem-1 .statement}

a) Soit $f$ un élément de $\mathscr{K}_+(X)$; la fonction $t \mapsto \lambda_t(f)$ est positive, semi-continue supérieurement, à support compact, et sa restriction à $\pi(X)$ est continue.

b) Soient $U$ un élément de $\mathcal{U}$, $\nu$ l’intégrale de la fonction scalairement essentiellement $\mu$-intégrable $t \mapsto \lambda_t$; l’image de la mesure $\nu|U$ par $\pi|U$ est égale à $\mu|\pi(U)$,

Pour établir a), on peut se ramener au moyen d’une partition de l’unité (chap. III, 2e éd., § 1, n° 2, lemme 1) au cas où le support S de f est contenu dans un ouvert $U \in \mathcal{U}$. Soit g l’application $t \mapsto \lambda_t(f) ; \pi|U$ étant un homéomorphisme, $g|\pi(U)$ appartient à $\mathscr{K}_+(\pi(U))$, et par suite ($\pi(U)$ étant un ouvert de $\pi(X)$) la restriction de g à $\pi(X)$ est continue. Comme g est positive et que la restriction de g au compact $\pi(S)$ est continue, on voit que g est semi-continue supérieurement dans T. On en déduit que g est $\mu$-intégrable.

Pour établir b), désignons par g un élément de $\mathscr{K}(\pi(U))$, par $g^\circ$ son prolongement par 0 à T, par f la fonction $g \circ (\pi|U)$, par $f^\circ$ la prolongement par 0 de f à X. L’assertion b) équivaut à l’égalité $\int g^\circ d\mu = \int f^\circ dv$. Mais on a $f \in \mathscr{K}(U)$, donc $f^\circ \in \mathscr{K}(X)$, et la seconde intégrale est donc égale à $\int \lambda_t(f^\circ) d\mu(t)$. On a enfin $\lambda_t(f^\circ) = g^\circ(t)$, ce qui achève la démonstration.

Notons maintenant que $\pi(X)$ est ouvert dans T, donc $\mu$-mesurable ; l’application $\Lambda : t \mapsto \lambda_t$ est vaguement $\mu$-mesurable, car sa restriction à chacun des ensembles $\pi(X)$ et $\mathbf{C}\pi(X)$ est vaguement continue. Dans ces conditions, la formule $\bar{\pi}^1(\mu) = \int \lambda_t d\mu(t)$ définit une décomposition en tranches de $\bar{\pi}^1(\mu)$ relativement à $\pi$, et la prop. 10 nous donne le résultat suivant :

#### Proposition 11 {#int-v-s6-prop-11 .statement}

Soit $\pi$ un homéomorphisme local d’un espace localement compact X dans un espace localement compact T, et soit $\mu$ une mesure positive sur T. Soit n la fonction numérique qui associe à tout $t \in T$ le nombre des éléments de $\bar{\pi}^1(t)$, si ce nombre est fini, ou $+\infty$ dans le cas contraire. Pour que $\pi$ soit $\bar{\pi}^1(\mu)$-propre, il faut et il suffit que n soit localement $\mu$-intégrable, et on a dans ce cas
$$
\pi(\bar{\pi}^1(\mu)) = n \cdot \mu.
$$

## EXERCICES {#int-v-s6-exercises}

See the [exercises for § 6](exercises/s6/).
