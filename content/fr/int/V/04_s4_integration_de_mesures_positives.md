---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 4
section_title: Intégration de mesures positives ponctuelles
lang: fr
source: int-v-fr
pdf_pages: 0039-0046, 0112-0113
extraction: ocr
subsections:
    - "no": 1
      title: Familles de mesures ponctuelles
      page: 0
      pdf_page: 39
    - "no": 2
      title: Intégrales supérieures de fonctions positives par rapport à une intégrale de mesures ponctuelles
      page: 0
      pdf_page: 41
    - "no": 3
      title: Mesurabilité par rapport à une intégrale de mesures ponctuelles
      page: 0
      pdf_page: 44
    - "no": 4
      title: Intégration des fonctions à valeurs dans un espace de Banach, par rapport à une intégrale de mesures ponctuelles
      page: 0
      pdf_page: 45
statements: 10
exercises: 2
content_sha256: 4520a35e8834ab3eab243c8ddf3c3354879d36bad295c2c83aa8a23b63553243
---

## § 4. Intégration de mesures positives ponctuelles

### 1. Familles de mesures ponctuelles

Soient $X$ et $T$ deux espaces localement compacts, $\pi$ une application de $T$ dans $X$, $g$ une fonction numérique finie et $\geqslant 0$, définie dans $T$; ces deux fonctions définissent une application $t \mapsto \lambda_t = g(t) \varepsilon_{\pi(t)}$ de $T$ dans l’espace $\mathcal{M}(X)$ des mesures sur $X$, telle que pour tout $t \in T$, $\lambda_t$ soit une mesure ponctuelle (chap. III, 2e éd., §2, n° 4) ou soit égale à 0. Si $f$ est une fonction numérique $\geqslant 0$ définie dans $X$, on a $\int^* f(x) \, d\lambda_t(x) = \int^* f(x) \, d\lambda_t(x) = f(\pi(t))g(t)$ (rappelons qu’on a convenu de prendre ce produit égal à 0 lorsque $g(t) = 0$ et $f(\pi(t)) = +\infty$). Toute fonction (à valeurs dans un espace topologique) définie dans $X$, est $\lambda_t$-mesurable pour tout $t \in T$. Toute application $f$ de $X$ dans un espace de Banach $F$ est $\lambda_t$-intégrable pour tout $t \in T$ et on a $\int f(x) \, d\lambda_t(x) = f(\pi(t))g(t)$. Enfin, si $f$ est une fonction numérique quelconque définie dans $X$, pour que $f$ soit $\lambda_t$-intégrable, il faut et il suffit que $f(\pi(t))g(t)$ soit fini, et on a alors $\int f(x) \, d\lambda_t(x) = f(\pi(t))g(t)$.

#### Définition 1 {#int-v-s4-def-1 .statement}

Soit $\mu$ une mesure positive sur $T$. On dit que le couple $(\pi, g)$ est $\mu$-adapté si les conditions suivantes sont satisfaites :
1° Les fonctions $\pi$ et $g$ sont $\mu$-mesurables.
2° Pour toute fonction $f \in \mathcal{K}(X)$, l’application $t \mapsto f(\pi(t))g(t)$ est essentiellement $\mu$-intégrable.

#### Proposition 1 {#int-v-s4-prop-1 .statement}

Si le couple $(\pi, g)$ est $\mu$-adapté, l’application $\Lambda : t \mapsto \lambda_t = g(t) \varepsilon_{\pi(t)}$ de $T$ dans $\mathcal{M}_+(X)$ est scalairement essentiellement $\mu$-intégrable, vaguement $\mu$-mesurable et $\mu$-adéquate. Inversement, si $\Lambda$ est scalairement essentiellement $\mu$-intégrable et vaguement $\mu$-mesurable, la fonction $g$ est $\mu$-mesurable, et la restriction de $\pi$ à l’ensemble $S$ des $t \in T$ tels que $g(t) \neq 0$ est $\mu$-mesurable.

En effet, supposons que le couple $(\pi, g)$ soit $\mu$-adapté; pour toute fonction $f \in \mathcal{K}(X)$, la fonction $t \mapsto \langle f, \lambda_t \rangle = f(\pi(t))g(t)$ est alors essentiellement $\mu$-intégrable. Montrons que $t \mapsto \lambda_t$ est vaguement $\mu$-mesurable. En effet, notons d’abord que, si $\pi$ et $g$ sont continues, l’application $t \mapsto \lambda_t$ est vaguement continue. Dans le cas général, l’ensemble des parties compactes $K$ de $T$ telles que les restrictions de $\pi$ et de $g$ à $K$ soient continues est $\mu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15); si $K$ est un tel ensemble, la restriction de $t \mapsto \lambda_t$ à $K$ est vaguement continue, d’où la première assertion de l’énoncé. La prop. 2 du § 3, n° 1, montre que $\Lambda$ est $\mu$-adéquate.

Inversement, supposons que $\Lambda$ soit scalairement essentiellement intégrable et vaguement $\mu$-mesurable; elle est alors $\mu$-adéquate (§ 3, n° 1, prop. 2). La fonction 1 étant semi-continue inférieurement dans $X$, la fonction $t \mapsto \lambda_t(1) = g(t)$ est $\mu$-mesurable (§ 3, déf. 1). L’ensemble $S$ est donc mesurable (chap. IV, 2e éd., § 5, n° 5, prop. 7). L’ensemble $R$ des compacts $K \subset S$ tels que $g|K$ soit continue et $\Lambda|K$ vaguement continue est $\mu$-dense dans $S$ (chap. IV, 2e éd., § 5, n° 10, prop. 15); si $K \in R$, la restriction à $K$ de l’application $t \mapsto \varepsilon_{\pi(t)} = \frac{1}{g(t)} \lambda_t$ est donc vaguement continue, et cela entraîne la continuité de $\pi|K$ (chap. III, 2e éd., § 1, n° 9, prop. 13). Comme $R$ est $\mu$-dense dans $S$, la restriction de $\pi$ à $S$ est mesurable.

Nous utiliserons le lemme suivant:

#### Lemme 1 {#int-v-s4-lem-1 .statement}

Soient $T$ et $X$ deux espaces topologiques, $\pi$ une application continue propre (Top. gén., chap. I, 4e éd., § 10, déf. 1) de $T$ dans $X$. Soit $g$ une fonction numérique semi-continue inférieurement, définie dans $T$. Pour tout $x \in X$, soit $f(x)$ la borne inférieure de la fonction $g(t)$ dans l’ensemble $\overline{\pi}^1(x)$ (borne inférieure égale à $+\infty$ si $\overline{\pi}^1(x) = \varnothing$; cf. Ens., chap. III, § 1, n° 9). Alors $f$ est semi-continue inférieurement dans $X$.

Pour tout nombre réel (fini) $a$, notons $B_a$ l’ensemble des $x \in X$ tels que $f(x) \leq a$, $A_a$ l’ensemble des $t \in T$ tels que $g(t) \leq a$; tout revient à montrer que $B_a$ est fermé (Top. gén., chap. IV, § 6, n° 2, prop. 1). Or $A_a$ est fermé (même réf.) et l’application propre $\pi$ est fermée (Top. gén., chap. I, 4e éd., § 10, n° 1, prop. 1); on est donc ramené à prouver que $\pi(A_a) = B_a$. La relation évidente

### 2. Intégrales supérieures de fonctions positives par rapport à une intégrale de mesures ponctuelles

Nous allons voir que, lorsque $(\pi, g)$ est un couple $\mu$-adapté, on peut préciser les résultats obtenus en appliquant les propositions du § 3 à la famille $t \mapsto \lambda_t = g(t) \varepsilon_{\pi(t)}$, qui est $\mu$-adéquate d’après la prop. 1.

#### Théorème 1 {#int-v-s4-thm-1 .statement}

Soit $(\pi, g)$ un couple $\mu$-adapté, et soit $\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t)$. Pour toute fonction numérique $f \geq 0$ définie dans $X$, on a

(1)
$$
\int^* f(x) \, d\nu(x) = \int^* f(\pi(t)) g(t) \, d\mu(t).
$$

A) Supposons d’abord que la mesure $\mu$ ait un support compact $K$, et que les restrictions à $K$ des fonctions $g$ et $\pi$ soient continues. On a, d’après la formule (4) du § 3, n° 1, $\nu^*(1) = \int_K g(t) \, d\mu(t) < +\infty$, de sorte que toutes les mesures qui interviennent dans la formule (1) sont bornées. On peut donc remplacer au premier membre $\int^*$ par $\int^*$. Compte tenu de la formule (6) du § 3, n° 2, tout revient à prouver que:

(2)
$$
\int^* f(x) \, d\nu(x) \leq \int^* f(\pi(t)) g(t) \, d\mu(t)
$$
où le symbole $\int^*$ au second membre peut à son tour être remplacé par $\int^*$. D’après la définition de l’intégrale supérieure, il suffit de vérifier l’inégalité

(3)
$$
\int^* f(x) \, d\nu(x) \leq \int^* h(t) \, d\mu(t)
$$
pour toute fonction $h$, semi-continue inférieurement dans $T$, majorant la fonction $t \mapsto f(\pi(t)) g(t)$. Or soit $\varepsilon$ un nombre $> 0$, et soit $u$ la fonction $(h + \varepsilon)/g$, qui est semi-continue inférieurement dans $K$. Si l’on a $t \in \bar{\pi}^1(\{x\}) \cap K$, on a $u(t) \geq f(x)$: c’est évident si $g(t) = 0$, car alors $u(t) = +\infty$; si $g(t) > 0$, on a
$$
u(t)g(t) = h(t) + \varepsilon \geq f(\pi(t))g(t) = f(x)g(t),
$$
d’où l’inégalité annoncée. Dans ces conditions soit $v(x)$, pour tout $x \in X$, la borne inférieure de $u(t)$ pour $t \in \pi^{-1}(\{x\}) \cap K$. La fonction $v$ majore $f$ d’après ce qui précède, elle est semi-continue inférieurement dans $X$ d’après le lemme 1 (appliqué à la restriction de $\pi$ à $K$); et on a $v(\pi(t))g(t) \leq h(t) + \varepsilon$ pour tout $t \in K$ (rappelons que le premier membre est nul par convention si $g(t) = 0$). Appliquons alors à $v$ la formule (4) du § 3, n° 1. Il vient:

(4)
$$
\int^* f(x)\ dv(x) \leq \int^* v(x)\ dv(x)
$$
$$
= \int^* v(\pi(t))g(t)\ d\mu(t) \leq \int_K^* (h(t) + \varepsilon)\ d\mu(t)
$$
$$
= \int_K^* h(t)\ d\mu(t) + \varepsilon\mu(1).
$$

La mesure $\mu$ étant bornée, et $\varepsilon$ étant arbitraire, l’inégalité (3) en résulte.

B) Passons maintenant au cas général. L’application $t \mapsto (\pi(t), g(t))$ de $T$ dans $X \times \mathbf{R}_+$ étant $\mu$-mesurable (chap. IV, § 5, n° 3, th. 1), l’ensemble $R$ des compacts $K$ de $T$ tels que les restrictions de $\pi$ et $g$ à $K$ soient continues est $\mu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15). D’après la prop. 4 du § 2, n° 3, $\mu$ est somme d’une famille sommable $(\mu_\alpha)_{\alpha \in A}$ de mesures portées par des éléments de $R$; le couple $(\pi, g)$ étant $\mu_\alpha$-adapté pour tout $\alpha \in A$, soit $v_\alpha$ la mesure $\int g(t)\varepsilon_{\pi(t)}\ d\mu_\alpha(t)$. On a alors d’après A)

(5)
$$
\int^* f(x)\ dv_\alpha(x) = \int^* f(\pi(t))g(t)\ d\mu_\alpha(t).
$$

Mais les $v_\alpha$ forment une famille sommable dont la somme est égale à $v$ (§ 3, n° 1, cor. de la prop. 1). On a donc d’après la prop. 1 du § 2, n° 1,

(6)
$$
\int^* f(x)\ dv(x) = \sum_{\alpha \in A} \int^* f(x)\ dv_\alpha(x).
$$

On a une relation analogue pour le second membre de (5), et (1) résulte donc de (5) par sommation sur $\alpha$.

#### Corollaire {#int-v-s4-n2-cor-1 .statement}

Pour qu’une partie $N$ de $X$ soit localement négligeable pour $v$, il faut et il suffit que l’intersection de $\pi^{-1}(N)$ et de l’ensemble des points $t \in T$ où $g(t) > 0$, soit localement négligeable pour $\mu$.

#### Proposition 2 {#int-v-s4-prop-2 .statement}

*Soient $\pi$ une application continue et propre* (Top. gén., chap. I, 4e éd., § 10, n° 1) *de T dans X, g une fonction numérique finie et continue dans T, telle que $g(t) > 0$ pour tout $t \in T$. Alors le couple $(\pi, g)$ est $\mu$-adapté, et si on pose*

$$
\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t),
$$

*on a, pour toute fonction numérique $f \geqslant 0$ définie dans X,

$$
\int^* f(x) \, dv(x) = \int^* f(\pi(t))g(t) \, d\mu(t).
$$

Il est clair que $\pi$ et $g$ sont $\mu$-mesurables ; en outre, pour toute fonction $\psi \in \mathcal{K}(X)$, $\psi \circ \pi$ est continue et à support compact, puisque $\pi$ est propre ; le couple $(\pi, g)$ est donc $\mu$-adapté, et en outre l’application $t \to g(t)\varepsilon_{\pi(t)}$ est *vaguement continue*.

Soit $h$ une fonction semi-continue inférieurement dans $T$, telle que $f(\pi(t))g(t) \leqslant h(t)$ pour tout $t \in T$. Nous allons montrer que

$$
\int^* f(x) \, dv(x) \leqslant \int^* h(t) \, d\mu(t).
$$

Par définition de l’intégrale supérieure, il en résultera l’inégalité

$$
\int^* f(x) \, dv(x) \leqslant \int^* f(\pi(t))g(t) \, d\mu(t)
$$

ce qui, joint à l’inégalité (7) du § 3, n° 2, démontrera (7).

Pour démontrer (8), définissons dans X une fonction $\bar{f}$ de la façon suivante : $\bar{f}(x)$ est la borne inférieure de $h(t)/g(t)$ dans l’ensemble $\overline{\pi}^1(x)$ (borne inférieure égale à $+\infty$ si $\overline{\pi}^1(x) = \varnothing$). La fonction $\bar{f}$ possède les propriétés suivantes :

1° $\bar{f}(x) \geqslant f(x)$ pour tout $x \in X$ (puisque $g(t) > 0$ pour tout $t \in T$).
2° $\bar{f}(\pi(t))g(t) \leqslant h(t)$ pour tout $t \in T$.
3° La fonction $\bar{f}$ est semi-continue inférieurement, en vertu du lemme 1, la fonction $h/g$ étant semi-continue inférieurement dans $T$.

On a par suite, compte tenu de la prop. 2a) du § 3, n° 1 :

$$
\int^* f(x) \, dv(x) \leqslant \int^* \bar{f}(x) \, dv(x) = \int^* \bar{f}(\pi(t))g(t) \, d\mu(t) \leqslant \int^* h(t) \, d\mu(t)
$$

ce qui établit (8), et achève la démonstration.

### 3. Mesurabilité par rapport à une intégrale de mesures ponctuelles

#### Proposition 3 {#int-v-s4-prop-3 .statement}

Soit $(\pi, g)$ un couple $\mu$-adapté, et soit $\nu = \int g(t) \varepsilon_{\pi(t)} d\mu(t)$. Soient $f$ une application de $X$ dans un espace topologique $G$, $S$ l’ensemble ($\mu$-mesurable) des points $t \in T$ tels que $g(t) > 0$. Pour que $f$ soit $\nu$-mesurable, il faut et il suffit que la restriction de $f \circ \pi$ à $S$ soit $\mu$-mesurable.

Supposons d’abord que $f$ soit $\nu$-mesurable. Par hypothèse, l’ensemble $\mathfrak{K}$ des parties compactes $K$ de $S$ telles que la restriction de $\pi$ à $K$ soit continue, est $\mu$-dense dans $S$ (chap. IV, 2e éd., § 5, n° 10, prop. 15). Pour montrer que la restriction à $S$ de $f \circ \pi$ est $\mu$-mesurable, il suffit donc de prouver que, pour tout $K \in \mathfrak{K}$, l’ensemble des parties compactes $H$ de $K$, telles que la restriction de $f \circ \pi$ à $H$ soit continue, est $\mu$-dense dans $K$ (chap. IV, 2e éd., § 5, n° 8, prop. 13). Mais par hypothèse, il existe une partition de l’ensemble compact $\pi(K)$ formée d’un ensemble $\nu$-négligeable $N$ et d’une suite d’ensembles compacts $(C_n)$ tels que la restriction de $f$ à chacun des $C_n$ soit continue. Dans ces conditions, $K \cap \overline{\pi}^{-1}(N)$ et les ensembles $K \cap \overline{\pi}^{-1}(C_n)$ forment une partition de $K$; mais $K \cap \overline{\pi}^{-1}(N)$ est $\mu$-négligeable en vertu du cor. du th. 1 du n° 2, les ensembles $K \cap \overline{\pi}^{-1}(C_n)$ sont compacts et la restriction de $f \circ \pi$ à chacun de ces derniers est continue, ce qui prouve que la restriction à $S$ de $f \circ \pi$ est $\mu$-mesurable.

Inversement, supposons qu’il en soit ainsi; pour montrer que $f$ est $\nu$-mesurable, il suffit de prouver que l’ensemble $\mathfrak{L}$ des parties compactes $L$ de $X$, telles que la restriction de $f$ à $L$ soit continue, est $\nu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15). Soit $N$ une partie de $X$ telle que $N \cap L$ soit $\nu$-négligeable pour tout $L \in \mathfrak{L}$, et montrons que $N$ est localement $\nu$-négligeable. Pour cela, nous devons montrer que $\overline{\pi}^{-1}(N) \cap S$ est localement $\mu$-négligeable (cor. du th. 1 du n° 2). Or, l’ensemble $\mathfrak{H}$ des parties compactes $H$ de $S$, telles que les restrictions à $H$ de $\pi$ et de $f \circ \pi$ soient continues, est par hypothèse $\mu$-dense dans $S$ (chap. IV, 2 éd., § 5, n° 10, prop. 15). Il nous suffit donc de prouver que $\overline{\pi}^{-1}(N) \cap H$ est $\mu$-négligeable pour tout $H \in \mathfrak{H}$. Or, $\pi(H)$ est compact et peut être identifié à l’espace quotient de $H$ par la relation d’équivalence $\pi(t) = \pi(t')$, $\pi$ étant identifiée à l’application canonique de $H$ sur cet espace quotient (Top. gén., chap. I, 4e éd., § 5, n° 2, prop. 3). Comme la restriction de $f \circ \pi$ à $H$ est continue, la restriction de $f$ à $\pi(H)$ est donc continue, autrement dit $\pi(H) \in \mathfrak{L}$, et par suite $N \cap \pi(H)$ est $\nu$-négligeable. En vertu du cor. du th. 1 du n° 2, $\bar{\pi}^1(N \cap \pi(H)) \cap S$ est localement $\mu$-négligeable ; il en est donc de même de l’ensemble

$$
H \cap \bar{\pi}^1(N) \subset \bar{\pi}^1(N \cap \pi(H)) \cap S ;
$$

mais comme $H$ est compact, $H \cap \bar{\pi}^1(N)$ est $\mu$-négligeable, ce qui achève la démonstration.

#### Remarque {#int-v-s4-n3-rem-1 .statement}

Si $f$ est une application de $X$ dans un espace de Banach $F$, il revient au même de dire que la restriction de $f \circ \pi$ à $S$ est $\mu$-mesurable, ou que la fonction $(f \circ \pi)g$ (définie dans $T$) est $\mu$-mesurable, puisque $g$ est $\mu$-mesurable, ne s’annule pas dans $S$, et est nulle dans $T - S$ (chap. IV, 2e éd., § 5, n° 10, prop. 15).

### 4. Intégration des fonctions à valeurs dans un espace de Banach, par rapport à une intégrale de mesures ponctuelles

#### Théorème 2 {#int-v-s4-thm-2 .statement}

Soit $(\pi, g)$ un couple $\mu$-adapté, et soit $\nu = \int g(t)\varepsilon_{\pi(t)} d\mu(t)$. Soit $f$ une fonction définie dans $X$, à valeurs dans un espace de Banach $F$ ou dans $\bar{R}$. Pour que $f$ soit essentiellement $\nu$-intégrable, il faut et il suffit que $t \mapsto f(\pi(t))g(t)$ soit essentiellement $\mu$-intégrable, et on a alors

$$
\int f(x) \, d\nu(x) = \int f(\pi(t))g(t) \, d\mu(t).
$$

Supposons en outre que $\pi$ soit continue et propre, et que $g$ soit continue et telle que $g(t) > 0$ pour tout $t \in T$. Alors, pour que $f$ soit $\nu$-intégrable, il faut et il suffit que $t \mapsto f(\pi(t))g(t)$ soit $\mu$-intégrable.

A) Nous commencerons par traiter le cas où la mesure $\mu$ est portée par un compact $K$, sur lequel $g$ est bornée. Les mesures $\mu$ et $\nu$ sont alors bornées, et on peut remplacer dans l’énoncé « essentiellement intégrable » par « intégrable ». Supposons que $f$ soit $\nu$-intégrable : la fonction $f(\pi(t))g(t)$ est alors $\mu$-intégrable, et la relation (9) est vérifiée, d’après le th. 1 du § 3, n° 3. Inversement, supposons que $f(\pi(t))g(t)$ soit $\mu$-intégrable : $f$ est alors $\nu$-mesurable (n° 3, prop. 3 et Remarque), et on a

$$
\int^\ast |f(x)| \, d\nu(x) = \int^\ast |f(\pi(t))|g(t) \, d\mu(t) < +\infty
$$

(n° 2, th. 1) : $f$ est donc essentiellement $\nu$-intégrable ($\S 1$, n° 3, prop. 9), donc $\nu$-intégrable. Le th. 1 du $\S 3$, n° 3 entraîne alors (9).

B) Passons au cas général. Soit $\mathcal{K}$ l’ensemble des parties compactes $K$ de $T$ telles que $g|K$ soit continue : $\mathcal{K}$ est $\mu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15), et la mesure $\mu$ est donc somme d’une famille $(\mu_\alpha)_{\alpha \in A}$ de mesures portées par des éléments de $\mathfrak{R}$ (§ 2, n° 3, prop. 4). Le couple $(g, \pi)$ est évidemment $\mu_\alpha$-adapté pour tout $\alpha \in A$, et la mesure $\nu$ est somme de la famille des mesures $\nu_\alpha = \int \varepsilon_{\pi(t)} g(t) \, d\mu_\alpha(t)$ (§ 3, n° 1, prop. 12). Le raisonnement de A) s’appliquant aux mesures $\mu_\alpha, \nu_\alpha$, la première partie de l’énoncé résulte alors de la prop. 3 du § 2, n° 2.

Pour que la fonction $f$ (resp. $t \mapsto f(\pi(t))g(t)$) soit intégrable pour $\nu$ (resp. pour $\mu$), il faut et il suffit qu’elle soit essentiellement intégrable, et qu’on ait

$$
\int^* |f(x)| \, d\nu(x) < +\infty \quad \text{(resp. } \int^* |f(\pi(t))|g(t) \, d\mu(t) < +\infty \text{)}.
$$

La seconde partie de l’énoncé résulte donc de la première partie, et de la proposition 2.

#### Remarque {#int-v-s4-n4-rem-1 .statement}

Soient $(\pi, g)$ un couple $\mu$-adapté, $\pi'$ une application de T dans X, $g'$ une fonction numérique finie et $\geqslant 0$ définie dans T, telles que $\pi'$ (resp. $g'$) soit égale à $\pi$ (resp. $g$) localement presque partout pour $\mu$. Alors le couple $(\pi', g')$ est $\mu$-adapté, les mesures $\lambda_t = g(t)\varepsilon_{\pi(t)}$ et $\lambda'_t = g'(t)\varepsilon_{\pi'(t)}$ sont égales localement presque partout, et on a $\int g(t)\varepsilon_{\pi(t)} \, d\mu(t) = \int g'(t)\varepsilon_{\pi'(t)} \, d\mu(t)$. Si maintenant $\pi'$ et $g'$ sont seulement définies localement presque partout (pour $\mu$), et s’il existe un couple $\mu$-adapté $(\pi, g)$ tel que $\pi'$ (resp. $g'$) soit égale à $\pi$ (resp. $g$) localement presque partout, on dit encore que le couple $(\pi', g')$ est $\mu$-adapté, et on pose alors

$$
\int g'(t)\varepsilon_{\pi'(t)} \, d\mu(t) = \int g(t)\varepsilon_{\pi(t)} \, d\mu(t)
$$

(cf. § 3, n° 3, Remarque). Les énoncés des th. 1 et 2 et de la prop. 3 restent valables lorsqu’on suppose seulement $\pi$ et $g$ définis localement presque partout.

## EXERCICES {#int-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
