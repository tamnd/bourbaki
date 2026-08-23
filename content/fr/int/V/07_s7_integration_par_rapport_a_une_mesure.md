---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 7
section_title: Intégration par rapport à une mesure induite
lang: fr
source: int-v-fr
pdf_pages: 0086-0091, 0129-0130
extraction: ocr
subsections:
    - "no": 1
      title: Intégration par rapport à une mesure induite
      page: 0
      pdf_page: 86
    - "no": 2
      title: Propriétés des mesures induites
      page: 0
      pdf_page: 89
statements: 20
exercises: 11
content_sha256: d84ab1ef16df49f8161c815ab2cebe85a55ecbdee4b03955ed78a0fa77c73263
---

## § 7. Intégration par rapport à une mesure induite

### 1. Intégration par rapport à une mesure induite

Soient X un sous-espace localement compact de T, $ \mu $ une mesure positive sur T, $ \mu_X $ la mesure induite sur X par $ \mu $ (chap. IV, 2e éd., § 5, n° 7). Pour tout $ t \in T $, définissons une mesure $ \lambda_t $ sur X de la façon suivante : $ \lambda_t = \varepsilon_t $ si $ t \in T $, $ \lambda_t = 0 $ si $ t \in \mathbf{C}X $. Pour toute fonction numérique finie $ g $ définie dans $ X $, on a $ \int g(x)\ d\lambda_t(x) = g(t) $ si $ t \in X $ et $ \int g(x)\ d\lambda_t(x) = 0 $ si $ t \in \mathbf{C}X $. Si $ g $ est une fonction de $ \mathscr{H}(X) $, on a donc, par définition de $ \mu_X $

(1)
$$
\mu_X(g) = \int \langle g, \lambda_t \rangle\ d\mu(t).
$$

Cela signifie que l’on peut écrire

(2)
$$
\mu_X = \int \lambda_t\ d\mu(t)
$$
($ \S 3, n^\circ 1 $).

Définissons maintenant une application $ \pi $ de $ T $ dans $ X $ en posant $ \pi(t) = t $ pour $ t \in X $, et $ \pi(t) = t_0 $ pour $ t \in \mathbf{C}X $, $ t_0 $ étant un point arbitraire de $ X $; on peut écrire, pour tout $ t \in T $, $ \lambda_t = \varphi_X(t)\varepsilon_{\pi(t)} $. L’application $ \pi $ est $ \mu $-mesurable, car ses restrictions à $ X $ et à $ \mathbf{C}X $ le sont (chap. IV, 2e éd., $ \S 5 $, $ n^\circ 10 $, prop. 16); il en résulte aussitôt que le couple $ (\pi, \varphi_X) $ est $ \mu $-adapté ($ \S 4, n^\circ 1 $). On a par conséquent les résultats suivants:

#### Proposition 1 {#int-v-s7-prop-1 .statement}

*Pour toute fonction numérique $ g \geqslant 0 $ définie dans $ X $, on a*

(3)
$$
\int^* g\ d\mu_X = \int_X^* g\ d\mu
$$
(cf. $ \S 5, n^\circ 3 $, *Exemple*, pour la notation $ \int_X^* $).

Si on tient compte des remarques qui précèdent et de (2), la relation (3) résulte du th. 1 du $ \S 4 $.

#### Corollaire 1 {#int-v-s7-prop-1-cor-1 .statement}

*Pour toute partie $ B $ de $ X $, on a $ \mu_X^*(B) = \mu^*(B) $; pour que $ B $ soit localement $ \mu_X $-négligeable, il faut et il suffit que $ B $ soit localement $ \mu $-négligeable.*

#### Corollaire 2 {#int-v-s7-prop-1-cor-2 .statement}

*Soit $ M $ une partie de $ T $. Si $ \mu $ est concentrée sur $ M $, $ \mu_X $ est concentrée sur $ M \cap X $.*

#### Corollaire 3 {#int-v-s7-prop-1-cor-3 .statement}

*Pour que la mesure $ \mu_X $ soit nulle, il faut et il suffit que $ X $ soit localement $ \mu $-négligeable.*

#### Remarque {#int-v-s7-n1-rem-1 .statement}

Si $ S $ est le support de $ \mu $, $ S \cap X $ (qui est fermé dans $ X $) contient le support de $ \mu_X $ d’après le cor. 2, mais peut en être distinct. Par exemple, si $ \mu $ est une mesure diffuse et $ X $ un sous-espace réduit à un point, la mesure induite $ \mu_X $ est nulle, donc son support est vide. On notera cependant que le support de $ \mu_X $ est égal à $ S \cap X $ si $ X $ est ouvert dans $ T $.

#### Proposition 2 {#int-v-s7-prop-2 .statement}

Pour qu’une application $ g $ de $ X $ dans un espace topologique soit $ \mu_X $-mesurable, il faut et il suffit que $ g $ soit $ \mu $-mesurable dans $ X $ ($ \S 5 $, no 3, Exemple).
Cela résulte de la prop. 3 du $ \S 4 $.

#### Corollaire {#int-v-s7-n1-cor-1 .statement}

Pour qu’une partie $ B $ de $ X $ soit $ \mu_X $-mesurable, il faut et il suffit que $ B $ soit $ \mu $-mesurable.

#### Théorème 1 {#int-v-s7-thm-1 .statement}

Soit $ g $ une fonction définie dans $ X $, à valeurs dans $ \bar{\mathbf{R}} $ ou dans un espace de Banach. Pour que $ g $ soit essentiellement $ \mu_X $-intégrable, il faut et il suffit que $ g $ soit essentiellement $ \mu $-intégrable dans $ X $ ($ \S 5 $, no 3, Exemple), et on a alors
$$
\int g\, d\mu_X = \int_X g\, d\mu.
$$
Cela résulte du th. 2 du $ \S 4 $.

#### Corollaire 1 {#int-v-s7-thm-1-cor-1 .statement}

Pour qu’une partie $ B $ de $ X $ soit essentiellement $ \mu_X $-intégrable, il faut et il suffit qu’elle soit essentiellement $ \mu $-intégrable, et on a $ \mu_X(B) = \mu(B) $.

#### Corollaire 2 {#int-v-s7-thm-1-cor-2 .statement}

Soit $ g $ une fonction complexe définie dans $ T $ et localement $ \mu $-intégrable; la restriction $ g_X $ de $ g $ à $ X $ est alors localement $ \mu_X $-intégrable, et on a
$$
(g \cdot \mu)_X = g_X \cdot \mu_X
$$
Cela résulte aussitôt du th. 1, appliqué aux fonctions $ fg $ ($ f \in \mathcal{H}(T; \mathbf{C}) $) et de la définition de la mesure induite par une mesure complexe sur $ X $ (chap. IV, 2e éd., $ \S 5 $, no 7).

#### Corollaire 3 {#int-v-s7-thm-1-cor-3 .statement}

Soit $ \theta $ une mesure complexe sur $ T $; on a
$$
|\theta|_X = |\theta_X|
$$
Posons en effet $ |\theta| = \mu $, et appliquons le cor. 2 en prenant pour $ g $ une fonction complexe de valeur absolue 1 telle que $ \theta = g \cdot \mu $ ($ \S 5 $, no 5, cor. 3 du th. 2); il vient $ \theta_X = g_X \cdot \mu_X $; mais $ g_X $ est une fonction de valeur absolue 1, et la formule (6) résulte de la prop. 2 du $ \S 5 $, no 2.

#### Remarque {#int-v-s7-n1-rem-2 .statement}

a) Le cor. 3 a déjà été démontré par une autre méthode (chap. IV, 2e éd., § 7, lemme 3).
    b) En vertu du cor. 3, les corollaires 1, 2, 3 de la prop. 1, la prop. 2, le théorème 1 et ses cor. 1, 2 s’étendent aussitôt à une mesure complexe.

#### Scholie {#int-v-s7-n1-sch-1 .statement}

Pour toute fonction f (resp. g) définie dans X (resp. dans T) à valeurs dans l’espace de Banach F ou dans $ \bar{\mathbf{R}} $, désignons par $ \zeta(f) $ (resp. par $ \rho(g) $) le prolongement par 0 de f à T (resp. la restriction de g à X). On a $ \zeta(\rho(g)) = \varphi_X \cdot g $, $ \rho(\zeta(f)) = f $. Désignons par $ \mu' $ la mesure $ \varphi_X \cdot \mu $ sur T. Pour tout $ p \in \{1, +\infty\} $, les propositions 1 et 2 entraînent que $ \zeta $ applique $ \mathcal{L}_F^p(X, \mu_X) $ dans $ \mathcal{L}_F^p(T, \mu') $, que $ \rho $ applique $ \mathcal{L}_F^p(T, \mu') $ sur $ \mathcal{L}_F^p(X, \mu_X) $, avec conservation de la norme dans les deux cas, et de l’intégrale pour $ p = 1 $ (th. 1); par passage aux espaces séparés associés, on obtient deux isomorphismes réciproques l’un de l’autre. De même, si l’on applique $ \zeta $ et $ \rho $ à des fonctions numériques positives, il y a conservation de l’intégrale supérieure essentielle (prop. 1). Si l’on convient donc d’identifier une fonction sur X à une fonction sur T nulle sur $ X - T $, et la mesure $ \mu_X $ à la mesure $ \mu' $, on ramène les problèmes concernant les mesures induites à des problèmes concernant les mesures définies par des densités, traités au § 5. Cette manière de raisonner s’applique d’ailleurs aussi aux mesures complexes, d’après le cor. 3 du th. 1.

### 2. Propriétés des mesures induites

#### Proposition 3 {#int-v-s7-prop-3 .statement}

Soient X un sous-espace localement compact de T, et $ \lambda $ une mesure complexe sur X. Les propriétés suivantes sont équivalentes:
    a) l’injection canonique $ i : X \to T $ est $ \lambda $-propre;
    b) pour tout compact K de T, $ K \cap X $ est essentiellement $ \lambda $-intégrable;
    c) tout point $ t \in T $ admet un voisinage V tel que $ V \cap X $ soit essentiellement $ \lambda $-intégrable;
    d) il existe une mesure $ \theta $ sur T telle que $ \theta_X = \lambda $.
Si ces conditions équivalentes sont satisfaites, on a avec la notation de d),

$$
(i(\lambda))_X = \lambda \quad \text{et} \quad i(\lambda) = i(\theta_X) = \varphi_X \cdot \theta.
$$

L’injection i étant continue, l’équivalence des propriétés a), b) et c) résulte de la prop. 1 du § 6, et de la remarque qui la suit,

$$
\int g\, d(i(\lambda))_X = \int g'\, d(i(\lambda)) = \int (g' \circ i)\, d\lambda = \int g\, d\lambda.
$$

Cela achève de prouver l’équivalence des quatre propriétés. Si $\lambda = \theta_X$, et si $g \in \mathscr{H}(T; \mathbf{C})$, on a

$$
\int g\, d(i(\theta_X)) = \int (g \circ i)\, d(\theta_X) = \int g \varphi_X\, d\theta,
$$

car $g \varphi_X$ est le prolongement par 0 de $g \circ i$ à $T$. Cela prouve la seconde formule (7).

#### Corollaire 1 {#int-v-s7-prop-3-cor-1 .statement}

Si $X$ est fermé, toute mesure complexe $\lambda$ sur $X$ est induite par une mesure sur $T$.

En effet, si $K$ est un compact de $T$, $K \cap X$ est alors compact, donc $\lambda$-intégrable.

#### Corollaire 2 {#int-v-s7-prop-3-cor-2 .statement}

Soient $\theta$ une mesure complexe sur $T$, $\pi$ une application $\theta$-propre de $T$ dans un espace localement compact $Y$, et $\pi_X$ sa restriction à $X$. Alors $\pi_X$ est $\theta_X$-propre, et on a $\pi_X(\theta_X) = \pi(\varphi_X \cdot \theta)$.

En effet, on a $\pi_X = \pi \circ i$, où $i$ est l’injection canonique $X \to T$. Lorsque $\theta$ est positive le corollaire se déduit donc de la prop. 3 et de la transitivité des mesures images ($§ 6$, n° 3, prop. 4). Le cas d’une mesure complexe non positive en résulte par linéarité.

#### Proposition 4 {#int-v-s7-prop-4 .statement}

Soient $X$ et $Y$ deux sous-espaces localement compacts de $T$, tels que $Y \subset X$. Si $\theta$ est une mesure complexe sur $T$, la mesure $(\theta_X)_Y$ induite par $\theta_X$ sur $Y$ est égale à $\theta_Y$ (« transitivité des mesures induites »).

Il suffit de remarquer que, si $g$ est un élément de $\mathscr{H}(Y; \mathbf{C})$, le prolongement par 0 de $g$ à $T$ s’obtient en prolongeant par 0 le prolongement par 0 de $g$ à $X$, ou encore, en utilisant les identifications du Scholie, que $\varphi_Y \cdot \theta = \varphi_Y(\varphi_X \cdot \theta)$ ($§ 5$, n° 4, prop. 8).

#### Proposition 5 {#int-v-s7-prop-5 .statement}

Soit $(\lambda_\alpha)_{\alpha \in A}$ une famille filtrante croissante de mesures positives sur $T$, admettant une borne supérieure $\lambda$, et soit $X$ un sous-espace localement compact de $T$. La famille des mesures induites $\lambda_\alpha|X$ est alors majorée dans $\mathcal{M}(X)$, et on a
$$
\sup_{\alpha \in A} (\lambda_\alpha|X) = \lambda|X.
$$
Compte tenu des identifications du Scholie, cette proposition est un cas particulier de la prop. 5 du § 5, n° 4.

#### Corollaire {#int-v-s7-n2-cor-1 .statement}

Soit $(\mu_i)_{i \in I}$ une famille sommable de mesures positives sur $T$, de somme $\mu$. La famille des mesures induites $\mu_i|X$ est alors sommable, et on a
$$
\sum_{i \in I} (\mu_i|X) = \mu|X.
$$

#### Proposition 6 {#int-v-s7-prop-6 .statement}

Soit $\Lambda : t \mapsto \lambda_t$ une application $\mu$-adéquate de $T$ dans $\mathcal{M}_+(X)$, où $X$ est un espace localement compact dénombrable à l’infini, et soit $Y$ un sous-espace localement compact de $X$. Posons $\int \lambda_t d\mu(t) = v$. L’application $t \mapsto \lambda_t|Y$ de $T$ dans $\mathcal{M}_+(Y)$ est alors $\mu$-adéquate, et on a
$$
\int (\lambda_t|Y) d\mu(t) = v|Y.
$$
Compte tenu des identifications du Scholie, cette proposition est un cas particulier de la prop. 7 du § 5, n° 4.

## EXERCICES {#int-v-s7-exercises}

See the [exercises for § 7](exercises/s7/).
