---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 4
section_title: Produit d’espaces topologiques
lang: fr
source: top-i-iv-fr
book_pages: TG I.24-TG I.29, TG I.94-TG I.96
pdf_pages: 0036-0041, 0106-0108
extraction: ocr
subsections:
    - "no": 1
      title: Espaces produits
      page: 24
      pdf_page: 36
    - "no": 2
      title: Coupe d’un ensemble ouvert; coupe d’un ensemble fermé; projection d’un ensemble ouvert. Continuité partielle
      page: 26
      pdf_page: 38
    - "no": 3
      title: Adhérence dans un produit
      page: 27
      pdf_page: 39
    - "no": 4
      title: Limites projectives d’espaces topologiques
      page: 28
      pdf_page: 40
statements: 21
exercises: 10
content_sha256: c5e8bc3d0246c8dffd05dcc00a8d75345c75d23ad88acc1bae1dccf4b636ecd7
---

## § 4. PRODUIT D’ESPACES TOPOLOGIQUES

### 1. Espaces produits

#### Définition 1 {#top-i-s4-def-1 .statement}

Étant donnée une famille $(X_i)_{i \in I}$ d’espaces topologiques, on appelle espace produit de cette famille l’ensemble produit $X = \prod_{i \in I} X_i$ muni de la topologie produit des topologies des $X_i$ (I, p. 14, *Exemple III*). On dit que les $X_i$ ($i \in I$) sont les espaces facteurs de $X$.

En vertu de I, p. 12, prop. 4, la topologie produit sur $X$ a pour base l’ensemble $\mathfrak{B}$ des intersections finies d’ensembles de la forme $\overline{\mathrm{pr}}_i^{-1}(U_i)$, où $U_i$ est ouvert dans $X_i$; ces ensembles ne sont autres que les produits $\prod_{i \in I} A_i$, où $A_i$ est ouvert dans $X_i$ pour tout $i \in I$ et où $A_i = X_i$ sauf pour un nombre fini d’indices; nous donnerons à ces ensembles le nom d’ensembles élémentaires.

Si $\mathfrak{B}_i$ est une base de la topologie de $X_i$ (pour tout $i \in I$), il est clair que les ensembles élémentaires $\prod_{i \in I} A_i$ tels que $A_i \in \mathfrak{B}_i$ pour tout $i$ tel que $A_i \neq X_i$ forment encore une base de la topologie produit. Ceux de ces ensembles qui contiennent un point $x \in X$ forment par suite un système fondamental de voisinages de $x$ (I, p. 5, prop. 3).

Lorsque $I$ est un ensemble fini, la construction de la topologie produit à partir des topologies des $X_i$ se simplifie: les ensembles élémentaires sont simplement les produits $\prod_{i \in I} A_i$, où $A_i$ est une partie ouverte quelconque de $X_i$ pour tout $i \in I$ (cf. I. p. 95, exerc. 9).

#### Exemple {#top-i-s4-n1-exa-1 .statement}

*Le produit $\mathbf{R}^n$ de $n$ espaces identiques à la droite numérique $\mathbf{R}$ est appelé espace numérique à $n$ dimensions; $\mathbf{R}^2$ est aussi appelé plan numérique* (cf. VI, § 1, n° 1). *On définit de même, à partir de la droite rationnelle $\mathbf{Q}$, l’espace rationnel à $n$ dimensions $\mathbf{Q}^n$ (*plan rationnel* pour $n = 2$).

La topologie de l’espace $\mathbf{R}^n$ a pour base l’ensemble des produits de $n$ intervalles ouverts dans $\mathbf{R}$, ensembles qu’on appelle pavés ouverts à $n$ dimensions. Les pavés ouverts contenant un point $x \in \mathbf{R}^n$ forment un système fondamental de voisinages de ce point. On appelle de même pavés fermés à $n$ dimensions les produits de $n$ intervalles fermés dans $\mathbf{R}$. Les pavés fermés auxquels $x$ est intérieur forment encore un système fondamental de voisinages de $x$. On a des résultats analogues pour l’espace rationnel à $n$ dimensions.*

#### Proposition 1 {#top-i-s4-prop-1 .statement}

Soit $f = (f_i)$ une application d’un espace topologique $Y$ dans un espace produit $X = \prod_{i \in I} X_i$. Pour que $f$ soit continue en un point $a \in Y$, il faut et il suffit que, pour tout $i \in I$, $f_i$ soit continue au point $a$.

Comme $f_i = \mathrm{pr}_i \circ f$, cela n’est autre qu’un cas particulier de la prop. 4 de I, p. 12.

#### Corollaire 1 {#top-i-s4-prop-1-cor-1 .statement}

Soient $(X_i)_{i \in I}$, $(Y_i)_{i \in I}$ deux familles d’espaces topologiques ayant même ensemble d’indices. Pour tout $i \in I$, soit $f_i$ une application de $X_i$ dans $Y_i$. Pour que l’application produit $f : (x_i)$ de $(f_i(x_i)) \mapsto \prod_{i \in I} X_i$ dans $\prod_{i \in I} Y_i$ soit continue en un point $a = (a_i)$, il faut et il suffit que, pour tout $i \in I$, $f_i$ soit continue au point $a_i$.

En effet, $f$ s’écrit $x \mapsto (f_i(\mathrm{pr}_i x))$; la condition est donc suffisante en vertu de la prop. 1. Inversement, pour tout $\kappa \in I$, soit $g_\kappa$ l’application de $X_\kappa$ dans $\prod_{i \in I} X_i$ telle que $\mathrm{pr}_\kappa(g_\kappa(x_\kappa)) = x_\kappa$ et $\mathrm{pr}_i(g_\kappa(x_\kappa)) = a_i$ pour $i \neq \kappa$; $g_\kappa$ est continue au point $a_\kappa$ en vertu de la prop. 1; comme $f_\kappa = \mathrm{pr}_\kappa \circ f \circ g_\kappa$, on voit que si $f$ est continue au point $a$, $f_\kappa$ est continue au point $a_\kappa$.

#### Corollaire 2 {#top-i-s4-prop-1-cor-2 .statement}

Soient $X, Y$ deux espaces topologiques. Pour qu’une application $f : X \to Y$ soit continue, il faut et il suffit que l’application $g : x \mapsto (x, f(x))$ soit un homéomorphisme de $X$ sur le graphe $G$ de $f$ (considéré comme sous-espace de l’espace produit $X \times Y$).

Comme $f = \mathrm{pr}_2 \circ g$, la condition est suffisante. Elle est nécessaire, car si $f$ est continue, $g$ est bijective et continue (prop. 1) et son application réciproque est la restriction à $G$ de $\mathrm{pr}_1$, qui est continue (cf. E, IV, p. 18, critère CST 17).

#### Proposition 2 (associativité des produits topologiques) {#top-i-s4-prop-2 .statement}

Soient $(X_i)_{i \in I}$ une famille d’espaces topologiques, $(J_\kappa)_{\kappa \in K}$ une partition de l’ensemble $I$, et, pour tout $\kappa \in K$, soit $X'_\kappa = \prod_{i \in J_\kappa} X_i$ le produit des espaces $X_i$ pour $i \in J_\kappa$. L’application canonique (E, II, p. 35) de l’espace produit $\prod_{i \in I} X_i$ sur l’espace produit $\prod_{\kappa \in K} X'_\kappa$ est un homéomorphisme.

C’est un cas particulier de la transitivité des topologies initiales (I, p. 13, prop. 5; cf. E, IV, p. 17, critère CST 13).

On identifie le plus souvent les espaces produits $\prod_{i \in I} X_i$ et $\prod_{\kappa \in K} X'_\kappa$ au moyen de l’application canonique.

#### Corollaire {#top-i-s4-n1-cor-1 .statement}

Soit $\sigma$ une permutation de l’ensemble $\mathbf{I}$. L’application $(x_i) \mapsto (x_{\sigma(i)})$ est un homéomorphisme de $\prod_{i \in \mathbf{I}} X_i$ sur $\prod_{i \in \mathbf{I}} X_{\sigma(i)}$.

Il suffit, dans la prop. 2, de prendre $K = \mathbf{I}$ et $J_i = \{\sigma(i)\}$ pour tout $i \in \mathbf{I}$.

#### Proposition 3 {#top-i-s4-prop-3 .statement}

Soient $X$ un ensemble, $(Y_i)_{i \in \mathbf{I}}$ une famille d’espaces topologiques, et pour chaque $i \in \mathbf{I}$, soit $f_i$ une application de $X$ dans $Y_i$. Soit $f$ l’application $x \mapsto (f_i(x))$ de $X$ dans $Y = \prod_{i \in \mathbf{I}} Y_i$, et soit $\mathcal{T}$ la topologie la moins fine sur $X$ rendant continues les $f_i$. Alors $\mathcal{T}$ est l’image réciproque par $f$ de la topologie induite sur $f(X)$ par la topologie produit sur $Y$.

C’est un autre cas particulier de la transitivité des topologies initiales (I, p. 13, prop. 5; cf. E, IV, p. 17, critère CST 15).

#### Corollaire {#top-i-s4-n1-cor-2 .statement}

Pour tout $i \in \mathbf{I}$, soit $A_i$ un sous-espace de $Y_i$. La topologie induite sur $A = \prod_{i \in \mathbf{I}} A_i$ par la topologie produit sur $\prod_{i \in \mathbf{I}} Y_i$ est la topologie produit des topologies des sous-espaces $A_i$.

Il suffit d’appliquer la prop. 3 aux fonctions $f_i = j_i \circ \mathrm{pr}_i$, $j_i$ étant l’injection canonique $A_i \to Y_i$ (cf. E, IV, p. 17, critère CST 14).

### 2. Coupe d’un ensemble ouvert; coupe d’un ensemble fermé; projection d’un ensemble ouvert. Continuité partielle

#### Proposition 4 {#top-i-s4-prop-4 .statement}

Soient $X_1, X_2$ deux espaces topologiques; pour tout $a_1 \in X_1$, l’application $x_2 \mapsto (a_1, x_2)$ est un homéomorphisme de $X_2$ sur le sous-espace $\{a_1\} \times X_2$ de $X_1 \times X_2$.

C’est un cas particulier du cor. 2 de I, p. 25, appliqué à la fonction constante $x_2 \mapsto a_1$.

L’application $x_2 \mapsto (a_1, x_2)$ est une section continue (I, p. 22) pour la relation d’équivalence $\mathrm{pr}_2 z = \mathrm{pr}_2 z'$ dans $X_1 \times X_2$; l’espace quotient de $X_1 \times X_2$ par cette relation d’équivalence est donc homéomorphe à $X_2$.

#### Corollaire {#top-i-s4-n2-cor-1 .statement}

La coupe $A(x_1)$ d’un ensemble ouvert (resp. fermé) $A$ du produit $X_1 \times X_2$, suivant un point quelconque $x_1 \in X_1$, est un ensemble ouvert (resp. fermé) dans $X_2$.

#### Proposition 5 {#top-i-s4-prop-5 .statement}

La projection sur un espace facteur d’un ensemble ouvert $U$ du produit $X_1 \times X_2$ est un ensemble ouvert.

En effet, on a par exemple $\mathrm{pr}_2 U = \bigcup_{x_1 \in X_1} U(x_1)$ et la proposition résulte du cor. de la prop. 4 et de l’axiome $(\mathrm{O}_1)$.

#### Remarque 1 {#top-i-s4-n2-rem-1 .statement}

La projection sur un espace facteur d’une partie fermée d’un espace produit $X_1 \times X_2$ peut fort bien ne pas être un ensemble fermé. Par exemple, dans le plan rationnel $\mathbf{Q}^2$, l’hyperbole d’équation $x_1 x_2 = 1$ est un ensemble fermé, mais ses projections sont toutes deux égales au complémentaire du point 0 dans $\mathbf{Q}$, ensemble qui n’est pas fermé.

#### Proposition 6 {#top-i-s4-prop-6 .statement}

Soient $X_1, X_2, Y$ trois espaces topologiques, $f$ une application de l’espace produit $X_1 \times X_2$ dans $Y$. Si $f$ est continue au point $(a_1, a_2)$, l’application partielle $x_2 \mapsto f(a_1, x_2)$ de $X_2$ dans $Y$ est continue au point $a_2$.

En effet cette application est composée de $f$ et de l’application $x_2 \mapsto (a_1, x_2)$; la proposition résulte donc de la prop. 4.

On exprime souvent la prop. 6 en disant qu’une fonction continue de deux arguments est continue par rapport à chacun d’eux.

#### Remarque 2 {#top-i-s4-n2-rem-2 .statement}

Il se peut que toutes les applications partielles déterminées par une application $f : X_1 \times X_2 \to Y$ soient continues sans que $f$ soit continue dans $X_1 \times X_2$ (cf. IX, § 5, exerc. 21 et EVT, III, § 4, exerc. 4). *Par exemple, l’application $f$ du plan numérique $\mathbf{R}^2$ dans $\mathbf{R}$, définie par $f(x, y) = xy/(x^2 + y^2)$ pour $(x, y) \neq (0, 0)$ et $f(0, 0) = 0$, a toutes ses applications partielles continues, sans être continue au point $(0, 0)$, puisque $f(x, x) = \frac{1}{2}$ si $x \neq 0$.*

Si $g$ est une application de $X_1$ dans $Y$, continue en un point $a_1$, l’application $(x_1, x_2) \mapsto g(x_1)$ de $X_1 \times X_2$ dans $Y$ est continue en tout point $(a_1, x_2)$, car elle est composée de $g$ et de la projection sur $X_1$.

Les résultats de ce numéro s’étendent aisément à un produit quelconque $\prod_{i \in I} X_i$ d’espaces topologiques, en remarquant que ce produit est homéomorphe au produit $(\prod_{i \in J} X_i) \times (\prod_{i \in K} X_i)$ pour toute partition $(J, K)$ de $I$ (I, p. 25, prop. 2).

### 3. Adhérence dans un produit

#### Proposition 7 {#top-i-s4-prop-7 .statement}

Dans un espace produit $\prod_{i \in I} X_i$, l’adhérence d’un produit d’ensembles $\prod_{i \in I} A_i$ est identique au produit $\prod_{i \in I} \overline{A}_i$ de leurs adhérences.

En effet, supposons que $a = (a_i)$ soit adhérent à $\prod_i A_i$; pour tout $\kappa \in I$, $a_\kappa = \mathrm{pr}_\kappa a$ est adhérent à $A_\kappa$ en vertu de la continuité de $\mathrm{pr}_\kappa$ (I, p. 9, th. 1), donc $a \in \prod_i \overline{A}_i$. Réciproquement, soit $b = (b_i) \in \prod_i \overline{A}_i$ et soit $\prod_i V_i$ un ensemble élémentaire quelconque contenant $b$; pour tout $i \in I$, $V_i$ contient un point $x_i \in A_i$, donc $\prod_i V_i$ contient le point $(x_i) \in \prod_i A_i$, ce qui prouve que $b$ est adhérent à $\prod_i A_i$.

#### Corollaire {#top-i-s4-n3-cor-1 .statement}

Pour qu’un produit $\prod_i A_i$ d’ensembles non vides soit fermé dans l’espace $\prod_i X_i$, il faut et il suffit que, pour tout $i$, $A_i$ soit fermé dans $X_i$.

Rappelons que si $I$ est fini, un produit $\prod_{i \in I} A_i$ est ouvert lorsque, pour tout $i \in I$, $A_i$ est ouvert dans $X_i$; mais il n’en est pas de même lorsque $I$ est infini.

#### Proposition 8 {#top-i-s4-prop-8 .statement}

Soit $a = (a_i)$ un point d’un espace produit $X = \prod_{i \in I} X_i$; l’ensemble $D$ des points $x \in X$ tels que $\mathrm{pr}_i x = a_i$ sauf pour un nombre fini d’indices $i$, est partout dense dans $X$.

En effet, pour tout $x \in X$ et tout ensemble élémentaire $V = \prod_{i \in I} U_i$ contenant $x$, on a $U_i = X_i$ sauf pour les indices $i$ appartenant à une partie finie $J$ de $I$; prenons $y_i = x_i$ pour $i \in J$, $y_i = a_i$ pour $i \notin J$; il est clair que $y = (y_i) \in D$ et $y \in V$, d’où la proposition.

### 4. Limites projectives d’espaces topologiques

Soient $I$ un ensemble préordonné (non nécessairement filtrant), la relation de préordre dans $I$ étant notée $\alpha \leq \beta$. Pour tout $\alpha \in I$, soit $X_\alpha$ un espace topologique, et pour $\alpha \leq \beta$, soit $f_{\alpha \beta}$ une application de $X_\beta$ dans $X_\alpha$. Nous dirons que $(X_\alpha, f_{\alpha \beta})$ est un système projectif d’espaces topologiques si : 1° $(X_\alpha, f_{\alpha \beta})$ est un système projectif d’ensembles (E, III, p. 52); 2° pour $\alpha \leq \beta, f_{\alpha \beta}$ est une application continue. Soient $X$ l’ensemble $\lim_{\leftarrow} X_\alpha$, et pour tout $\alpha \in I$, soit $f_\alpha$ l’application canonique $X \to X_\alpha$; nous dirons que sur $X$ la topologie la moins fine rendant continues les $f_\alpha$ est la limite projective (pour les $f_{\alpha \beta}$) des topologies des $X_\alpha$, et que l’ensemble $X$, muni de cette topologie, est la limite projective du système projectif d’espaces topologiques $(X_\alpha, f_{\alpha \beta})$: lorsque nous parlerons de $\lim_{\leftarrow} X_\alpha$ comme d’un espace topologique, il sera toujours sous-entendu, sauf mention expresse du contraire, que la topologie de cet espace est la limite projective des topologies des $X_\alpha$.

On sait que l’ensemble $X$ est la partie du produit $\prod_{\alpha \in I} X_\alpha$ formée des points $x$ tels que
(1)
$$
\mathrm{pr}_\alpha x = f_{\alpha \beta}(\mathrm{pr}_\beta x)
$$
pour $\alpha \leq \beta$. Il résulte de la prop. 3 de I, p. 26 que, sur $X$, la topologie limite projective des topologies des $X_\alpha$ est identique à la topologie induite par la topologie de l’espace produit $\prod_{\alpha \in I} X_\alpha$. Si, pour tout $\alpha \in I$, $Y_\alpha$ est un sous-espace de $X_\alpha$, de sorte que les $Y_\alpha$ forment un système projectif de parties des $X_\alpha$ (E, III, p. 54), il est clair que l’espace topologique $\lim_{\leftarrow} Y_\alpha$ est un sous-espace de $\lim_{\leftarrow} X_\alpha$.

Soit $(X'_\alpha, f'_{\alpha \beta})$ un second système projectif d’espaces topologiques ayant même ensemble d’indices $I$, et pour tout $\alpha \in I$, soit $u_\alpha : X_\alpha \to X'_\alpha$ une application continue, telle que $(u_\alpha)$ soit un système projectif d’applications (E III, p. 54); alors $u = \lim_{\leftarrow} u_\alpha$ est une application continue de $X = \lim_{\leftarrow} X_\alpha$ dans $X' = \lim_{\leftarrow} X'_\alpha$. En effet, si $f'_\alpha$ est l’application canonique $X' \to X'_\alpha$, on a $f'_\alpha \circ u = u_\alpha \circ f_\alpha$, donc $f'_\alpha \circ u$ est continue pour tout $\alpha \in I$, et notre assertion résulte de la prop. 4 de I, p. 12.

Enfin, supposons $I$ filtrant à droite, et soit $J$ une partie cofinale de $I$; soit $Z$ la limite projective du système projectif $(X_\alpha, f_{\alpha \beta})_{\alpha \in J, \beta \in J}$ d’espaces topologiques.

Alors la bijection canonique $g : X \to Z$ (E, III, p. 55, prop. 3) est un homéomorphisme. En effet, pour tout $\lambda \in J$, on a $\mathrm{pr}_\lambda(g(x)) = \mathrm{pr}_\lambda x$, donc $g$ est continue (I, p. 25, prop. 1); inversement, soit $h$ la bijection réciproque de $g$; pour tout $\alpha \in I$, il existe $\lambda \in J$ tel que $\alpha \leq \lambda$ et on a donc $\mathrm{pr}_\alpha(h(z)) = f_{\alpha \lambda}(\mathrm{pr}_\lambda z)$, ce qui montre la continuité de $h$ (I, p. 25, prop. 1), vu l’hypothèse sur les $f_{\alpha \beta}$.

#### Proposition 9 {#top-i-s4-prop-9 .statement}

Soit $I$ un ensemble préordonné filtrant à droite. Soient $(X_\alpha, f_{\alpha \beta})$ un système projectif d’espaces topologiques ayant $I$ pour ensemble d’indices, $X = \lim_{\leftarrow} X_\alpha$, $J$ une partie cofinale de $I$. La famille des ensembles $f_\alpha^{-1}(U_\alpha)$, où $\alpha$ parcourt $J$, où $f_\alpha$ est l’application canonique $X \to X_\alpha$, et où, pour chaque $\alpha \in J$, $U_\alpha$ parcourt une base $\mathcal{B}_\alpha$ de la topologie de $X_\alpha$, est une base de la topologie de $X$.

On sait (I, p. 12) que les intersections finies d’ensembles de la forme $f_\alpha^{-1}(U_\alpha)$ ($\alpha \in I$, $U_\alpha$ ouvert dans $X_\alpha$) forment une base de la topologie de $X$. Si $(\alpha_i)_{1 \leq i \leq n}$ est une famille finie d’indices de $I$, il existe $\gamma \in J$ tel que $\alpha_i \leq \gamma$ pour $1 \leq i \leq n$, donc $f_{\alpha_i} = f_{\alpha_i \gamma} \circ f_\gamma$, et si l’on pose $V_\gamma = \bigcap_i f_{\alpha_i \gamma}^{-1}(U_{\alpha_i})$, on a $f_\gamma(V_\gamma) = \bigcap_i f_{\alpha_i}^{-1}(U_{\alpha_i})$; mais $V_\gamma$ est ouvert, donc réunion d’ensembles de $\mathcal{B}_\gamma$, d’où la proposition.

#### Corollaire {#top-i-s4-n4-cor-1 .statement}

Supposons $I$ filtrant. Soit $A$ une partie de $X = \lim_{\leftarrow} X_\alpha$, et pour tout $\alpha \in I$, posons $A_\alpha = f_\alpha(A)$. Alors:
(i) Les $A_\alpha$ (resp. les $\overline{A}_\alpha$) forment un système projectif de parties des $X_\alpha$ et l’on a $\overline{A} = \bigcap_\alpha f_\alpha^{-1}(\overline{A}_\alpha) = \lim_{\leftarrow} \overline{A}_\alpha$.
(ii) Si $A$ est fermé dans $X$, on a $A = \lim_{\leftarrow} A_\alpha = \lim_{\leftarrow} \overline{A}_\alpha$.

La première assertion de (i) résulte des relations $f_\alpha = f_{\alpha \beta} \circ f_\beta$ pour $\alpha \leq \beta$ et de ce que les $f_{\alpha \beta}$ sont continues (I, p. 9, th. 1). Posons $A' = \bigcap_\alpha f_\alpha^{-1}(\overline{A}_\alpha)$; il est clair que $A'$ est fermé et contient $A$, donc $\overline{A} \subset A'$. Inversement, soit $x \in A'$ et montrons que $x$ est adhérent à $A$. En vertu de la prop. 9, il suffit de prouver que tout voisinage de $x$ qui est de la forme $f_\alpha^{-1}(U_\alpha)$, avec $\alpha \in I$ et $U_\alpha$ ouvert dans $X_\alpha$, rencontre $A$. Or on a par hypothèse $f_\alpha(x) \in U_\alpha$, et comme $f_\alpha(x) \in \overline{A}_\alpha$, on a $U_\alpha \cap A_\alpha \neq \varnothing$, ce qui signifie que $A \cap f_\alpha^{-1}(U_\alpha)$ n’est pas vide.

Pour établir (ii), il suffit de remarquer que, sans hypothèse sur $A$, on a $A \subset \lim_{\leftarrow} A_\alpha \subset \lim_{\leftarrow} \overline{A}_\alpha$; si $A$ est fermé, il résulte de (i) que $A = \lim_{\leftarrow} \overline{A}_\alpha$, d’où (ii).

#### Exemple {#top-i-s4-n4-exa-1 .statement}

Soit $(X_\alpha)_{\alpha \in I}$ une famille filtrante (pour $\supseteq$) de parties d’un ensemble $Y$, et pour chaque $\alpha \in I$, soit $\mathcal{T}_\alpha$ une topologie sur $X_\alpha$, telle que pour $\alpha \leq \beta$, $\mathcal{T}_\beta$ soit plus fine que la topologie induite sur $X_\beta$ par $\mathcal{T}_\alpha$. Alors, si l’on prend pour $f_{\alpha \beta}$ l’injection canonique $X_\beta \to X_\alpha$ pour $\alpha \leq \beta$, $\lim_{\leftarrow} X_\alpha$ s’identifie canoniquement à l’intersection $X$ des $X_\alpha$ muni de la topologie borne supérieure (I, p. 13, Exemple II) des topologies induites sur $X$ par les $\mathcal{T}_\alpha$.

## EXERCICES {#top-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
