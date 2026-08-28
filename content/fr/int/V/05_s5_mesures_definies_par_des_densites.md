---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 5
section_title: Mesures définies par des densités numériques
lang: fr
source: int-v-fr
pdf_pages: 0046-0073, 0113-0123
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions localement intégrables
      page: 0
      pdf_page: 46
    - "no": 2
      title: Mesures définies par des densités numériques
      page: 0
      pdf_page: 48
    - "no": 3
      title: Intégration par rapport à une mesure définie par une densité
      page: 0
      pdf_page: 51
    - "no": 4
      title: Comportement du produit par rapport aux opérations usuelles
      page: 0
      pdf_page: 54
    - "no": 5
      title: Caractérisation des mesures de base $\mu$
      page: 0
      pdf_page: 57
    - "no": 6
      title: Mesures équivalentes
      page: 0
      pdf_page: 62
    - "no": 7
      title: Mesures étrangères
      page: 0
      pdf_page: 64
    - "no": 8
      title: '*Applications: I. Dualité des espaces* $L^p$'
      page: 0
      pdf_page: 66
    - "no": 9
      title: 'Applications: II. Fonctions de mesures'
      page: 0
      pdf_page: 70
    - "no": 10
      title: Mesures diffuses; mesures atomiques
      page: 0
      pdf_page: 72
statements: 48
exercises: 31
content_sha256: c6f935722c5425e83061430af4684c1cb286583577803e519dc328c98c47f944
---

## § 5. Mesures définies par des densités numériques

### 1. Fonctions localement intégrables

#### Proposition 1 {#int-v-s5-prop-1 .statement}

Soit $g$ une fonction définie localement presque partout dans T (pour la mesure positive $\mu$), à valeurs dans un espace de Banach F (resp. dans $\bar{\mathbf{R}}$). Les propriétés suivantes sont équivalentes:

a) Pour tout point $t \in T$, il existe un voisinage $V$ de $t$ tel que la fonction $g \varphi_V$ soit $\mu$-intégrable.

b) La fonction $g$ est $\mu$-mesurable et, pour tout ensemble compact $K \subset T$, on a $\int^* |g| \varphi_K d\mu < +\infty$.

c) Pour toute fonction numérique $h \in \mathcal{K}(T)$, $gh$ est $\mu$-intégrable.

Montrons que a) entraîne b); la fonction $g$ est en effet mesurable en vertu du principe de localisation (chap. IV, § 5, n° 2, prop. 4). D’autre part, pour tout $t \in K$, il existe par hypothèse un voisinage $V_t$ de $t$ dans $T$ tel que $g \varphi_{V_t}$ soit intégrable; on peut donc recouvrir $K$ par un nombre fini de voisinages $V_i (1 \leq i \leq n)$ tels que les fonctions $g \varphi_{V_i}$ soient intégrables. Comme

$$
|g| \varphi_K \leq \sum_{i=1}^n |g| \varphi_{V_i},
$$

on a $\int^* |g| \varphi_K d\mu < +\infty$.

En second lieu, b) entraîne c), car $gh$ est alors mesurable, et si $L$ est le support compact de $h$, on a $|gh| \leq \|h\| \cdot |g| \varphi_L$, donc $\int^* |gh| d\mu < +\infty$ par hypothèse; $gh$ est par suite intégrable en vertu du critère d’intégrabilité (chap. IV, § 5, n° 6, th. 5).

Enfin, c) entraîne a). En effet, pour tout $t \in T$, soit $V$ un voisinage compact de $t$. Il existe une application continue $h$ de $T$ dans $[0, 1]$, égale à 1 dans $V$ et à support compact (chap. III, 2e éd., § 1, n° 2, lemme 1); par hypothèse $gh$ est intégrable, donc il en est de même de $g \varphi_V = (gh) \varphi_V$ (chap. IV, § 5, n° 6, cor. 3 du th. 5).

#### Définition 1 {#int-v-s5-def-1 .statement}

On dit qu’une fonction $g$, définie localement presque partout dans $T$ (pour la mesure positive $\mu$), à valeurs dans un espace de Banach $F$ (resp. dans $\bar{\mathbf{R}}$) est localement intégrable pour $\mu$ (ou localement $\mu$-intégrable) si elle satisfait aux conditions $a), b), c)$ de la prop. 1. Si $\theta$ est une mesure complexe, on dit qu’une fonction $g$ définie localement $\theta$-presque partout est localement $\theta$-intégrable si elle est localement intégrable pour la mesure positive $|\theta|$.

Si $g$ est localement $\theta$-intégrable, toute fonction égale à $g$ localement presque partout est localement intégrable. Il est clair que la somme de deux fonctions localement intégrables est localement intégrable. Les fonctions à valeurs dans $F$, partout définies et localement intégrables pour $\theta$ forment un espace vectoriel noté $\mathcal{L}_{loc}^1(T, \theta; F)$; lorsque $F = \mathbf{R}$ ou $\mathbf{C}$, la mention de $F$ est souvent omise s’il n’y a pas d’ambiguïté. Cet espace sera toujours muni (sauf mention expresse du contraire) de la topologie définie par les semi-normes $g \mapsto \int |g \varphi_K| d|\theta|$, où $K$ parcourt l’ensemble des compacts de T. L’espace séparé associé, quotient de $\mathcal{L}_{\text{loc}}^1(T, \theta ; F)$ par le sous-espace $\mathcal{N}^\infty(F)$ des applications nulles localement presque partout, est noté $L_{\text{loc}}^1(T, \theta ; F)$. Les espaces $L_{\text{loc}}^1(T, \theta ; F)$ et $L_{\text{loc}}^1(T, |\theta| ; F)$ sont identiques.

On peut montrer que les espaces vectoriels topologiques qui viennent d’être définis sont complets (exerc. 31).

Toute fonction mesurable g essentiellement bornée dans tout ensemble compact est localement intégrable. Pour tout nombre $p$ tel que $1 \leq p \leq +\infty$, toute fonction $g \in \mathcal{L}_F^p$ est localement intégrable; en effet, pour toute fonction $h \in \mathscr{K}(T)$, $h$ appartient à $\mathcal{L}^q$ (où $q$ est l’exposant conjugué de $p$), donc $gh$ est intégrable (chap. IV, 2e éd., § 6, no 4, cor. 4 du th. 2).

Soient F, G, H trois espaces de Banach, et $(\mathbf{u}, \mathbf{v}) \mapsto \Phi(\mathbf{u}, \mathbf{v})$ une application bilinéaire continue de $F \times G$ dans H. Si $f$ est localement intégrable et prend ses valeurs dans F, et si $g \in \mathcal{L}_G^\infty$, $\Phi(f, g)$ est localement intégrable (chap. IV, § 6, no 4, cor. 1 du th. 2).

### 2. Mesures définies par des densités numériques

Soit $g$ une fonction numérique positive définie localement $\mu$-presque partout dans T, localement $\mu$-intégrable; l’ensemble des $t$ tels que $g(t) = +\infty$ est alors localement $\mu$-négligeable, car $g \varphi_K$ est $\mu$-intégrable pour tout compact K (chap. IV, § 2, no 3, prop. 7). Soit alors $g'$ une fonction localement intégrable positive et finie, égale à $g$ localement $\mu$-presque partout; posons $\lambda'_t = g'(t) \varepsilon_t$. L’application $t \mapsto \lambda'_t$ de T dans $\mathcal{M}_+(T)$ est vaguement $\mu$-mesurable et scalairement essentiellement intégrable (ou encore, le couple (I, $g'$), où I est l’application identique de T, est $\mu$-adapté); l’intégrale $\nu = \int \lambda'_t \, d\mu(t)$ ne dépend pas de la fonction $g'$, localement presque partout égale à $g$, utilisée dans la définition des mesures $\lambda'_t$. Cette mesure $\nu$ est définie par la condition

$$
\int f(t) \, d\nu(t) = \int f(t)g(t) \, d\mu(t) \quad \text{pour } f \in \mathscr{K}(T).
$$

Si maintenant $\theta$ est une mesure complexe, et si $u$ est une fonction complexe (ou une fonction à valeurs dans $\overline{\mathbf{R}}$) définie localement $\theta$-presque partout et localement intégrable pour $\theta$, on peut écrire

$$
\begin{align*}
\mu &= g_1 - g_2 + i(g_3 - g_4) \\
\theta &= \mu_1 - \mu_2 + i(\mu_3 - \mu_4).
\end{align*}
$$

$$
f \mapsto \int f(t)u(t)\ d\theta(t)
$$

sur $\mathcal{K}(T)$ est une mesure complexe.

#### Définition 2 {#int-v-s5-def-2 .statement}

*Soit $\theta$ une mesure complexe, et soit $u$ une fonction complexe (ou une fonction à valeurs dans $\bar{\mathbf{R}}$) définie localement $\theta$-presque partout et localement $\theta$-intégrable. On dit que la mesure complexe $f \mapsto \int fu\ d\theta$ sur $T$ est le produit de la mesure $\theta$ par la fonction $u$, ou la mesure de densité $u$ par rapport à $\theta$, et on la note $u . \theta$.

*Toute mesure complexe, produit d’une mesure positive $\mu$ par une fonction localement $\mu$-intégrable, est appelée mesure de base $\mu$.*

La relation $\eta = u . \theta$ s’écrit encore par convention

$$
d\eta(t) = u(t)\ d\theta(t).
$$

Lorsque $u$ est partout définie et continue, on retrouve la définition donnée au chap. III, 2e éd., § 1, n° 4. Il est clair que si $u_1$ et $u_2$ sont localement $\theta$-intégrables, on a $(u_1 + u_2) . \theta = u_1 . \theta + u_2 . \theta$. De même, si $\theta_1$ et $\theta_2$ sont deux mesures sur $T$, et si $u$ est une fonction localement intégrable pour $\theta_1$ et $\theta_2$, $u$ est localement intégrable pour $\theta_1 + \theta_2$ et on a $u . (\theta_1 + \theta_2) = u . \theta_1 + u . \theta_2$.

Nous nous bornerons désormais au cas des fonctions partout définies ; l’extension aux fonctions définies localement presque partout, toujours évidente, est laissée au lecteur.

La proposition suivante permet de ramener en grande partie le cas des mesures complexes à celui des mesures positives :

#### Proposition 2 {#int-v-s5-prop-2 .statement}

*Soient $\theta$ une mesure complexe, $u$ une fonction complexe localement $\theta$-intégrable ; on a*

$$(3)$$
$$
|u . \theta| = |u| . |\theta|
$$

Nous commencerons par un résultat auxiliaire :

*Lemme 1. — Soit $\theta$ une mesure complexe, et soit $f$ un élément de $\bar{\mathcal{L}}_c^1(T, \theta)$. On a alors

$$
\langle |\theta|, |f| \rangle = \sup_{c \in \mathscr{K}_1} |\langle \theta, cf \rangle| = \sup_{c \in \mathscr{B}_1} |\langle \theta, cf \rangle|
$$

où $\mathscr{K}_1$ (resp. $\mathscr{B}_1$) désigne l’ensemble des fonctions complexes c continues à support compact (resp. boréliennes) telles que $|c| \leq 1$.

Traitons d’abord le cas où $f \in \mathscr{K}(T; \mathbf{C})$. On a évidemment $\sup_{c \in \mathscr{K}_1} |\langle \theta, cf \rangle| \leq \sup_{c \in \mathscr{B}_1} |\langle \theta, cf \rangle| \leq \langle |\theta|, |f| \rangle$ (chap. IV, § 4, n° 2, prop. 2).

D’autre part, soit g un élément de $\mathscr{K}(T; \mathbf{C})$ tel que $|g| \leq |f|$; g est limite uniforme d’une suite $(g_n)$ d’éléments de $\mathscr{K}(T; \mathbf{C})$, dont les supports sont contenus dans l’ouvert U formé des t tels que $f(t) \neq 0$, et l’on peut évidemment supposer que $|g_n| \leq |f|$ pour tout n. Posons $c_n(t) = g_n(t)/f(t)$ pour $t \in U$, $c_n(t) = 0$ pour $t \notin U$; on a $c_n \in \mathscr{K}_1$, $g = \lim_{n \to \infty} c_n f$, donc $|\langle \theta, g \rangle| = \lim_{n \to \infty} |\langle \theta, c_n f \rangle|$, et finalement $\sup_{|g| \leq |f|, g \in \mathscr{K}(T; \mathbf{C})} |\langle \theta, g \rangle| \leq \sup_{c \in \mathscr{K}_1} |\langle \theta, cf \rangle|$. On conclut en remarquant que le premier membre de cette inégalité est égal à $\langle |\theta|, |f| \rangle$ (chap. III, 2e éd., § 1, n° 6, formule (12)).

Désignons ensuite par f un élément de $\bar{\mathcal{L}}_c^1(\theta)$, et montrons que (4) est encore vraie : il suffit de vérifier que les trois membres de cette relation dépendent continûment de f pour la topologie de $\bar{\mathcal{L}}_c^1(\theta)$, puisqu’ils coïncident sur le sous-espace dense $\mathscr{K}(T; \mathbf{C})$. Cela résulte aussitôt des inégalités suivantes, où f et $f'$ désignent des éléments de $\bar{\mathcal{L}}_c^1(\theta)$ :

$$
|\langle |\theta|, |f| \rangle - \langle |\theta|, |f'| \rangle| \leq \langle |\theta|, |f - f'| \rangle = N_1(f - f')
$$
$$
|\langle \theta, cf \rangle - \langle \theta, cf' \rangle| \leq \langle |\theta|, |c| |f - f'| \rangle \leq N_1(f - f')
$$

pour tout $c \in \mathscr{B}_1$. Le lemme est donc établi.

Passons à la démonstration de la proposition 2 : appliquons le lemme à la fonction uh, où h appartient à $\mathscr{K}_+(T)$. Il vient :

$$
\langle |\theta|, |uh| \rangle = \sup_{c \in \mathscr{K}_1} |\langle \theta, cuh \rangle| = \sup_{c \in \mathscr{K}_1} |\langle u . \theta, ch \rangle| = \langle |u . \theta|, h \rangle
$$

Mais le premier membre est aussi égal à

$$
\langle |\theta|, |u|h \rangle = \langle |u| . |\theta|, h \rangle.
$$

Les deux mesures $|u| . |\theta|$ et $|u . \theta|$ sont donc égales.

#### Corollaire {#int-v-s5-n2-cor-1 .statement}

Soient $g_1$ et $g_2$ deux fonctions numériques localement $\mu$-intégrables ; on a
$\inf(g_1 . \mu, g_2 . \mu) = \inf(g_1, g_2) . \mu$; $\sup(g_1 . \mu, g_2 . \mu) = \sup(g_1, g_2) . \mu$.

En particulier, si g est une fonction numérique localement $\mu$-intégrable, on a

$$
(g \cdot \mu)^+ = g^+ \cdot \mu; \quad (g \cdot \mu)^- = g^- \cdot \mu.
$$

Cela résulte aussitôt de la prop. 2 et des formules (6) du chap. II, § 1, n° 1.

### 3. Intégration par rapport à une mesure définie par une densité

Dans les énoncés de ce numéro, g désigne une fonction numérique positive, partout définie et localement $\mu$-intégrable, $\theta$ désigne une mesure complexe, et u une fonction complexe localement $\theta$-intégrable.

Les remarques du n° 2 montrent que les résultats du § 4 sont applicables à la mesure $v = g \cdot \mu = \int g(t) \varepsilon_t \, d\mu(t)$ (bien que la mesure $g(t) \varepsilon_t$ ne soit définie que si $g(t) \neq +\infty$). On obtient ainsi l’énoncé suivant:

#### Proposition 3 {#int-v-s5-prop-3 .statement}

Pour toute fonction numérique $f \geq 0$, définie dans T, on a

$$
\int^* f dv = \int^* (fg) \, d\mu
$$

Cela résulte du th. 1 du § 4, n° 2.

#### Corollaire 1 {#int-v-s5-prop-3-cor-1 .statement}

Pour qu’une fonction $\mathbf{f}$, à valeurs dans un espace de Banach ou dans $\bar{\mathbf{R}}$, soit localement négligeable pour la mesure $u \cdot \theta$, il faut et il suffit que $u \mathbf{f}$ soit localement négligeable pour $\theta$.

Dire que $\mathbf{f}$ (resp. $u \mathbf{f}$) est localement négligeable pour $u \cdot \theta$ (resp. pour $\theta$) équivaut à dire que $|\mathbf{f}|$ (resp. $|u| \cdot |\mathbf{f}|$) est localement négligeable pour $|u \cdot \theta|$ (resp. pour $|\theta|$). On est donc ramené, compte tenu de la prop. 2 du n° 2, au cas où $f, u, \theta$ sont positives ; l’énoncé résulte alors aussitôt de la prop. 3.

#### Corollaire 2 {#int-v-s5-prop-3-cor-2 .statement}

Soient $u_1$ et $u_2$ deux fonctions complexes localement $\theta$-intégrables. Pour que $u_1 \cdot \theta = u_2 \cdot \theta$, il faut et il suffit que $u_1$ et $u_2$ soient égales localement presque partout.

On se ramène aussitôt à montrer que $u \cdot \theta = 0$ entraîne $u(t) = 0$ localement presque partout ; mais $u \cdot \theta = 0$ signifie que la fonction 1 est localement négligeable pour la mesure $u . \theta$. On applique alors le corollaire 1.

#### Corollaire 3 {#int-v-s5-prop-3-cor-3 .statement}

Soit $u$ une fonction complexe localement intégrable pour la mesure positive $\mu$. Pour que $u . \mu$ soit une mesure positive, il faut et il suffit que $u(t) \geqslant 0$ localement presque partout.
En effet, $u . \mu$ est positive si et seulement si
$$
u . \mu = |u . \mu| = |u| . \mu
$$
(prop. 2), et cela équivaut à $u = |u|$ localement presque partout (cor. 2).

#### Proposition 4 {#int-v-s5-prop-4 .statement}

Pour qu’une application $f$ de $T$ dans un espace topologique $G$ soit mesurable pour la mesure $u . \theta$, il faut et il suffit que la restriction de $f$ à l’ensemble $\theta$-mesurable $S$ des $t$ tels que $u(t) \neq 0$ soit $\theta$-mesurable.
Lorsque $u$ et $\theta$ sont positives, cela résulte aussitôt de la prop. 3 du § 4, n° 3. Le résultat s’étend alors au cas où $u$ et $\theta$ sont complexes grâce à la prop. 2.

#### Corollaire {#int-v-s5-n3-cor-1 .statement}

Soit $f$ une fonction définie dans $T$, à valeurs dans un espace de Banach $F$ ou dans $\bar{\mathbf{R}}$. Pour que $f$ soit $(u . \theta)$-mesurable, il faut et il suffit que $uf$ soit $\theta$-mesurable.
En effet, $uf$ est le prolongement par 0 de $(uf)|_S$ à $T$.

#### Théorème 1 {#int-v-s5-thm-1 .statement}

Soit $f$ une fonction définie dans $T$, à valeurs dans un espace de Banach $F$ ou dans $\bar{\mathbf{R}}$. Pour que $f$ soit essentiellement intégrable pour la mesure $\eta = u . \theta$, il faut et il suffit que $uf$ soit essentiellement $\theta$-intégrable, et on a alors
$$
\int f \, d\eta = \int (uf) \, d\theta.
$$
Supposons en outre que $u$ soit continue et que $u(t) \neq 0$ pour tout $t \in T$; $f$ est alors intégrable pour la mesure $\eta$ si et seulement si $uf$ est intégrable pour $\theta$.
Le cas où $u$ et $\theta$ sont positives résulte aussitôt du th. 2 du § 4, n° 4. La première et la dernière assertion de l’énoncé s’en déduisent aussitôt, car $f$ est essentiellement intégrable (resp. intégrable) par rapport à $\eta = u . \theta$ si et seulement si elle est essentiellement intégrable (resp. intégrable) pour $|\eta| = |u| . |\theta|$.
Enfin, supposons que $f$ soit essentiellement intégrable pour $\eta$ (donc pour $|\eta|$); utilisons la décomposition (2): $f$ est essentiellement intégrable pour chacune des mesures $\eta_{ij} = g_i : \mu_j$ ($i = 1, 2, 3, 4, j = 1, 2, 3, 4$), car celles-ci sont majorées par $|\eta|$. On a

$$
\int \mathbf{f}\ d\eta_{ij} = \int g_i \mathbf{f}\ d\mu_j.
$$

La formule (6) s’en déduit immédiatement.

#### Corollaire {#int-v-s5-n3-cor-2 .statement}

Pour que la mesure $u.\theta$ soit bornée, il faut et il suffit que $u$ soit essentiellement $\theta$-intégrable.

#### Exemple {#int-v-s5-n3-exa-1 .statement}

Soit A une partie de T ; pour que $\varphi_A$ soit localement $\mu$-intégrable, il faut et il suffit que A soit $\mu$-mesurable. Supposant cette condition remplie, posons $v = \varphi_A . \mu$; pour toute fonction numérique $f \geqslant 0$ définie dans T, on a alors

$$
\int^\ast f dv = \int^\ast f \varphi_A\ d\mu,
$$

valeur que l’on note encore $\int_A^\ast f\ d\mu$ (cf. chap. IV, § 5, n° 6). Pour qu’une application $g$ de T dans un espace topologique G soit $v$-mesurable, il faut et il suffit que la restriction de $g$ à A soit $\mu$-mesurable. Pour qu’une application $\mathbf{f}$ de T dans un espace de Banach F ou dans $\bar{\mathbf{R}}$ soit essentiellement $v$-intégrable, il faut et il suffit que $\mathbf{f} \varphi_A$ soit essentiellement $\mu$-intégrable, et on a

$$
\int \mathbf{f}\ dv = \int \mathbf{f} \varphi_A\ d\mu,
$$

expression qu’on note encore $\int_A \mathbf{f}\ d\mu$. On notera que, si deux applications de T dans G (resp. F, $\bar{\mathbf{R}}$) coïncident dans A, pour que l’une d’elles soit $v$-mesurable (resp. essentiellement $v$-intégrable) il faut et il suffit que l’autre le soit. Si maintenant $g$ est une application dans G d’une partie quelconque $B \supset A$ de T, on dit que $g$ est $\mu$-mesurable dans A si un prolongement quelconque à T de la restriction de $g$ à A est $v$-mesurable, ce qui revient à dire que la restriction de $g$ à A est $\mu$-mesurable. On dit qu’une application $\mathbf{f}$ de B dans un espace de Banach F, ou dans $\bar{\mathbf{R}}$, est essentiellement $\mu$-intégrable dans A si un prolongement $\bar{\mathbf{f}}$ à T de la restriction de $\mathbf{f}$ à A est essentiellement $v$-intégrable ; on pose alors

$$
\int_A \mathbf{f}\ d\mu = \int_A \bar{\mathbf{f}} d\mu = \int \bar{\mathbf{f}} \varphi_A\ d\mu,
$$

et on dit que $\int_A \mathbf{f}\ d\mu$ est l’intégrale de $\mathbf{f}$ dans A (ou étendue à A).

Si $f$ est une fonction numérique $\geqslant 0$ définie dans $B \supset A$, on définit de même $\int_A^* f d\mu$ et $\int_A^\bullet f d\mu$. Enfin, on dit qu’une fonction numérique $g$ définie dans $B \supset A$ est *localement* $\mu$-intégrable *dans* $A$ si un prolongement $\bar{g}$ à $T$ de la restriction de $g$ à $A$ est localement $\nu$-intégrable : cela équivaut à dire que, pour toute partie compacte $K$ de $T$, $\bar{g} \varphi_{K \cap A}$ est $\mu$-intégrable.

### 4. Comportement du produit par rapport aux opérations usuelles

#### Proposition 5 {#int-v-s5-prop-5 .statement}

*Soit* $(\lambda_\alpha)_{\alpha \in A}$ *une famille de mesures positives sur* $T$, *filtrante pour la relation* $\leqslant$, *admettant dans* $\mathcal{M}(T)$ *une borne supérieure* $\lambda$. *Pour qu’une fonction numérique positive* $g$ *soit localement* $\lambda$-*intégrable*, *il faut et il suffit que* $g$ *soit localement* $\lambda_\alpha$*-intégrable pour tout* $\alpha \in A$, *et que la famille* $(g \cdot \lambda_\alpha)$ *soit majorée dans* $\mathcal{M}(T)$; *on a alors*

$$
g \cdot \lambda = \sup_{\alpha \in A} g \cdot \lambda_\alpha.
$$

Il est clair que la condition est nécessaire. Inversement, supposons que $g$ soit localement intégrable pour chaque mesure $\lambda_\alpha$, et que la famille $(g \cdot \lambda_\alpha)_{\alpha \in A}$ soit majorée ; désignons par $\lambda'$ sa borne supérieure. La fonction $g$ est alors $\lambda$-mesurable (§ 1, n° 4, cor. 2 de la prop. 11) ; on a de plus, pour toute fonction $h \in \mathscr{K}_+(T)$

$$
\int^\bullet (hg) \, d\lambda = \sup_{\alpha \in A} \int^\bullet (hg) \, d\lambda_\alpha = \sup_{\alpha \in A} \int^\bullet h \, d(g \cdot \lambda_\alpha) = \int^\bullet h \, d\lambda'
$$

(§ 1, n° 4, prop. 11). Cela entraîne d’abord que le premier membre est fini quel que soit $h$, de sorte que $g$ est localement $\lambda$-intégrable ; on peut donc remplacer le symbole $\int^\bullet$ par $\int$, et la formule s’écrit $\int h \, d(g \cdot \lambda) = \int h \, d\lambda'$. Il en résulte que $g \cdot \lambda = \lambda'$, et ceci achève la démonstration.

#### Corollaire {#int-v-s5-n4-cor-1 .statement}

*Supposons que* $\mu$ *soit la somme d’une famille* $(\mu_\alpha)_{\alpha \in A}$ *de mesures sur* $T$. *Pour qu’une fonction numérique positive* $g$ *définie dans* $T$ *soit localement* $\mu$*-intégrable*, *il faut et il suffit que* $g$ *soit localement* $\mu_\alpha$*-intégrable pour tout* $\alpha \in A$, *et que la famille* $(g \cdot \mu_\alpha)_{\alpha \in A}$ *soit sommable*. *On a dans ce cas*

$$(7)$$
$$
g \cdot \mu = \sum_{\alpha \in A} g \cdot \mu_\alpha.
$$

#### Proposition 6 {#int-v-s5-prop-6 .statement}

*Soit $(g_\alpha)_{\alpha \in A}$ une famille localement dénombrable de fonctions numériques positives localement $\mu$-intégrables définies dans $T$. Pour que la fonction $g = \sum_{\alpha \in A} g_\alpha$ soit localement $\mu$-intégrable, il faut et il suffit que la famille de mesures $(g_\alpha \cdot \mu)_{\alpha \in A}$ soit sommable, et on a dans ce cas*:

$$
g \cdot \mu = \sum_{\alpha \in A} g_\alpha \cdot \mu.
$$

Il est clair que $g$ est $\mu$-mesurable (chap. IV, 2e éd., § 5, n° 10, prop. 16). Pour que $g$ soit localement $\mu$-intégrable, il faut et il suffit par conséquent que $\mu^*(gf)$ soit fini pour tout $f \in \mathcal{H}_+(T)$. Or l’ensemble des $\alpha \in A$ tels que $g_\alpha f \neq 0$ étant dénombrable, on a $\mu^*(gf) = \sum_{\alpha \in A} \mu^*(g_\alpha f)$ (§ 1, n° 1, cor. de la prop. 2). Posons $v_\alpha = g_\alpha \cdot \mu$; la condition $\mu^*(gf) < +\infty$ équivaut à la condition $\sum_{\alpha \in A} v_\alpha(f) < +\infty$: autrement dit, $g$ est localement $\mu$-intégrable si et seulement si la famille $(v_\alpha)$ est sommable. Si l’on désigne alors par $v$ la somme de cette famille, le calcul précédent donne l’égalité $v(f) = \mu^*(gf)$, qui équivaut à (8).

#### Corollaire {#int-v-s5-n4-cor-2 .statement}

*Soit $(g_n)$ une suite de fonctions numériques localement $\mu$-intégrables, et telle que la suite des mesures $g_n \cdot \mu$ soit croissante. Pour que cette suite soit majorée dans l’espace vectoriel ordonné $\mathcal{M}(T)$ des mesures sur $T$, il faut et il suffit que la fonction $g = \sup g_n$ soit localement $\mu$-intégrable; la borne supérieure dans $\mathcal{M}(T)$ de la suite $(g_n \cdot \mu)$ est alors la mesure $g \cdot \mu$.

Il suffit d’appliquer la prop. 6 aux fonctions (positives localement presque partout) $g'_n = g_{n+1} - g_n$.

#### Proposition 7 {#int-v-s5-prop-7 .statement}

*Soit $X$ un espace localement compact dénombrable à l’infini, et soit $t \mapsto \lambda_t$ une application $\mu$-adéquate de $T$ dans $\mathcal{M}_+(X)$. Soit $g$ une fonction numérique positive définie dans $X$, localement intégrable pour la mesure $v = \int \lambda_t \, d\mu(t)$. L’ensemble des $t \in T$ tels que $g$ ne soit pas localement $\lambda_t$-intégrable est alors localement négligeable pour $\mu$, l’application $t \mapsto g . \lambda_t$ (définie localement $\mu$-presque partout) est $\mu$-adéquate, et on a:

$$
g . v = \int (g . \lambda_t) \, d\mu(t).
$$

Soit $(K_n)_{n \in \mathbf{N}}$ une suite croissante de compacts de $X$ dont les intérieurs recouvrent $X$; si $\eta$ est une mesure positive quelconque sur $X$, dire que $g$ est localement $\eta$-intégrable équivaut à dire que $g \varphi_{K_n}$ est $\eta$-intégrable pour tout $n$. Or soit $H_n$ l’ensemble des $t \in T$ tels que $g \varphi_{K_n}$ ne soit pas $\lambda_t$-intégrable, et soit $H = \bigcup_n H_n$; $H_n$ étant localement $\mu$-négligeable pour tout $n$ ($§ 3$, no 3, th. 1), il en est de même de $H$, ce qui établit la première assertion de l’énoncé. Quitte à remplacer $\lambda_t$ par 0 sur $H$ (ce qui ne change pas la mesure $v$), on peut supposer que $g$ est localement $\lambda_t$-intégrable pour tout $t \in T$. On a pour toute fonction positive $v$-mesurable $h$ définie dans $X$, d’après la prop. 3, et la prop. 5 du $§ 3$, no 2,

$$
\int^\bullet h \, d(g . v) = \int^\bullet (gh) \, dv = \int^\bullet d\mu(t) \int^\bullet (gh) \, d\lambda_t = \int^\bullet d\mu(t) \int^\bullet h \, d(g . \lambda_t).
$$

Cette formule et la prop. 5 du $§ 3$, no 2 montrent d’abord (en prenant $h \in \mathcal{K}_+(T)$) que l’application $t \mapsto g . \lambda_t$ est scalairement essentiellement $\mu$-intégrable, et que son intégrale est $g . v$; autrement dit, on a la relation (9). Ensuite, remplaçons $\mu$ par une mesure positive $\mu' \leq \mu$, et prenons pour $h$ une fonction semi-continue inférieurement positive : il résulte aussitôt de ces relations que $t \mapsto g . \lambda_t$ est $\mu$-adéquate ($§ 3$, no 1, déf. 1).

#### Proposition 8 {#int-v-s5-prop-8 .statement}

Soient $\theta$ une mesure complexe sur $T$, $g_1$ une fonction complexe localement $\theta$-intégrable, $\theta_1$ la mesure $g_1 . \theta$. Pour qu’une fonction complexe $g_2$ définie dans $T$ soit localement $\theta_1$-intégrable, il faut et il suffit que $g_2 g_1$ soit localement $\theta$-intégrable, et on a dans ce cas

$$
g_2 . \theta_1 = g_2 . (g_1 . \theta) = (g_2 g_1) . \theta
$$
(« formule d’associativité »).

D’après le cor. de la prop. 4, dire que $g_2$ est $\theta_1$-mesurable équivaut à dire que $g_2 g_1$ est $\theta$-mesurable. Supposons que cette condition soit satisfaite. On a, pour toute fonction $f \in \mathcal{K}_+(T)$, en vertu des propositions 2 et 3

$$
\int^\bullet |g_2| f d|\theta_1| = \int^\bullet |g_2| f |g_1| d|\theta| = \int^\bullet |g_2 g_1| f d|\theta|.
$$

Dire que $g_2$ est localement $\theta_1$-intégrable équivaut donc à dire que $g_2 g_1$ est localement $\theta$-intégrable. Cette condition étant supposée satisfaite, on a d’après le th. 1

$$
\int f d(g_2 \cdot \theta_1) = \int fg_2\, d\theta_1 = \int fg_2g_1\, d\theta = \int f d(g_2g_1 \cdot \theta)
$$

formule équivalente à (10).

### 5. Caractérisation des mesures de base $\mu$

**Théorème 2** (Lebesgue–Nikodym). — Soient $\mu$ et $\nu$ deux mesures positives sur $T$. Les propriétés suivantes sont équivalentes:

1) $\nu$ est une mesure de base $\mu$.
2) Tout ensemble localement $\mu$-négligeable est localement $\nu$-négligeable.
3) Tout compact $\mu$-négligeable est $\nu$-négligeable.

Il est clair que 1) entraîne 2) (cor. 1 de la prop. 3), et que 2) entraîne 3). Nous allons montrer que 3) entraîne 1). Notons d’abord que, si la condition 3) est remplie, tout ensemble $A$, universellement mesurable et localement $\mu$-négligeable, est localement $\nu$-négligeable ; on a en effet $\nu^*(A) = \sup \nu(K)$, $K$ parcourant l’ensemble des compacts contenus dans $A$ ($§ 1$, n° 3, prop. 10, a) et chap. IV, 2e éd., § 4, n° 6, cor. 2 du th. 4). Nous établirons ensuite deux lemmes.

#### Lemme 2 {#int-v-s5-lem-2 .statement}

Soient $\alpha$ une mesure positive bornée sur $T$, $\beta$ une mesure réelle sur $T$ telle que $|\beta| \leq M \alpha$, où $M$ est une constante positive. Il existe alors une fonction réelle $u$, $\alpha$-intégrable, telle que $\beta = u \cdot \alpha$.

Soit $g$ un élément de l’espace $\mathcal{L}^2_{\mathbf{R}}(T, \alpha)$; $g$ est $\beta$-mesurable et on a $\int^* |g|^2\, d|\beta| \leq M \int^* |g|^2\, d\alpha < +\infty$. La fonction $g$ appartient donc à $\mathcal{L}^2(T, |\beta|)$, et aussi à $\mathcal{L}^1(T, |\beta|)$ puisque $\beta$ est bornée. On a d’après l’inégalité de Cauchy–Schwarz

$$
|\beta(g)|^2 \leq (\int |g| d|\beta|)^2 \leq (\int d|\beta|)(\int |g|^2\, d|\beta|) \leq M^2 \alpha(1)\alpha(|g|^2).
$$

L’application $g \mapsto \beta(g)$ est donc une forme linéaire continue sur $\mathcal{L}^2(T, \alpha)$. L’espace séparé associé à $\mathcal{L}^2(T, \alpha)$ étant un espace hilbertien, il existe alors (*Esp. Vect. Top.*, chap. V, § 1, th. 3) une fonction réelle $u \in \mathcal{L}^2(T, \alpha)$, donc appartenant aussi à $\mathcal{L}^1(T, \alpha)$, telle que $\beta(g) = \alpha(ug)$ pour tout $g \in \mathcal{L}^2(T, \alpha)$. En appliquant cette relation pour $g \in \mathcal{H}(T)$, on voit que $\beta = u \cdot \alpha$.

#### Lemme 3 {#int-v-s5-lem-3 .statement}

Supposons que la mesure positive $v$ soit telle que tout compact $\mu$-négligeable soit $v$-négligeable. Soit $\mathfrak{K}$ l’ensemble des compacts $K$ de $T$ possédant la propriété suivante :

(11) Il existe une constante $M \geq 0$ telle que $\varphi_K \cdot v \leq M \varphi_K \cdot \mu$.

L’ensemble $\mathfrak{K}$ est alors $\mu$-dense dans $T$.

Si $K$ satisfait à (11), et si $A$ est une partie borélienne contenue dans $K$, il résulte aussitôt de la prop. 8 que $\varphi_A \cdot v \leq M \varphi_A \cdot \mu$; on en déduit que la réunion de deux éléments $K, K'$ de $\mathfrak{K}$ appartient à $\mathfrak{K}$ car $\varphi_{K \cup K'} = \varphi_K + \varphi_A$, où $A = K' \cap C K$. Pour établir le lemme, il reste à prouver que tout compact $L$ tel que $\mu(L) > 0$ contient un compact $K \in \mathfrak{K}$ tel que $\mu(K) > 0$ (chap. IV, 2e éd., § 5, n° 8, prop. 12). Choisissons un nombre $M > v(L)/\mu(L)$, et appliquons le lemme 1 à la mesure positive bornée $\alpha = \varphi_L \cdot (v + M \mu)$ et à la mesure $\beta = \varphi_L \cdot (v - M \mu)$. Quitte à modifier la fonction $u$ telle que $\beta = u \cdot \alpha$ par une fonction qui lui est égale $\alpha$-presque partout, on peut supposer que $u$ est universellement mesurable (§ 3, n° 5, prop. 7), et nulle hors de $L$. L’ensemble $H$ des $t \in T$ tels que $u(t) < 0$, qui est contenu dans $L$, ne saurait être $\mu$-négligeable, car il serait alors $v$-négligeable (d’après la remarque faite au début de la démonstration du th. 2), donc $\alpha$-négligeable, et on aurait $\beta(L) > 0$, ce qui contredit le choix de $M$. Soit $K$ un compact contenu dans $H$, tel que $\mu(K) > 0$; montrons que $K \in \mathfrak{K}$, ce qui établira le lemme. On a d’après la prop. 8

$$
\varphi_K \cdot (v - M \mu) = \varphi_K \cdot \beta = \varphi_K \cdot (u \cdot \alpha) = (\varphi_K u) \cdot \alpha.
$$

La fonction $\varphi_K u$ est négative, et on a bien par conséquent $\varphi_K \cdot v \leq M \varphi_K \cdot \mu$.

Achevons alors la démonstration du théorème 2. On suppose la condition 3) vérifiée et on définit $K$ comme dans le lemme 3. Soit $(K_\alpha)_{\alpha \in A}$ une famille localement dénombrable d’éléments de $\mathfrak{K}$ deux à deux disjoints, telle que l’ensemble $N = T - \bigcup_{\alpha \in A} K_\alpha$ soit localement $\mu$-négligeable (chap. IV, 2e éd., § 5, n° 9, prop. 14); la famille $(K_\alpha)$ étant localement dénombrable, $N$ est universellement mesurable, et donc localement $v$-négligeable. Posons $\mu_\alpha = \varphi_{K_\alpha} \cdot \mu, \nu_\alpha = \varphi_{K_\alpha} \cdot v$; les fonctions $\varphi_{K_\alpha}$ formant une famille localement dénombrable, dont la somme est égale à 1 localement presque partout pour $\mu$ et pour $v$, la proposition 6 entraîne que $\mu = \sum_{\alpha \in A} \mu_\alpha, \nu = \sum_{\alpha \in A} \nu_\alpha$. D’autre part, par définition de $\mathfrak{K}$, il existe pour tout $\alpha$ une constante $M_\alpha$ telle que $\nu_\alpha \leq M_\alpha \mu_\alpha$; le lemme 2 entraîne donc l’existence d’une fonction $g_\alpha$, que l’on peut supposer nulle hors de $K_\alpha$ et positive (cor. 3 de la prop. 3), telle que $v_\alpha = g_\alpha \cdot \mu_\alpha$. On a donc (n° 4, prop. 8)
$$
v_\alpha = g_\alpha \cdot \mu_\alpha = g_\alpha \cdot (\varphi_{K_\alpha} \cdot \mu) = (g_\alpha \varphi_{K_\alpha}) \cdot \mu = g_\alpha \cdot \mu.
$$
Posons $g = \sum_{\alpha \in A} g_\alpha$; la famille $(g_\alpha)$ étant localement dénombrable, et la famille $(v_\alpha)$ étant sommable, la proposition 6 entraîne que g est localement $\mu$-intégrable, et que $v = g \cdot \mu$, ce qui établit le théorème.

#### Corollaire 1 {#int-v-s5-lem-3-cor-1 .statement}

Soit $\mathcal{N}$ un ensemble de mesures positives de base $\mu$, admettant dans $\mathcal{M}(T)$ une borne supérieure $v$; alors $v$ est une mesure de base $\mu$.

Le cor. de la prop. 2 permet de se ramener au cas où $\mathcal{N}$ est un ensemble filtrant croissant. On a alors, pour tout ensemble localement $\mu$-négligeable A, d’après la prop. 11 du § 1, n° 4,
$$
v^\bullet(A) = \sup_{\lambda \in \mathcal{N}} \lambda^\bullet(A) = 0.
$$
Le théorème 2 entraîne donc que $v$ est une mesure de base $\mu$.

#### Corollaire 2 {#int-v-s5-lem-3-cor-2 .statement}

Soit $v$ une mesure réelle sur T. Pour que $v$ appartienne à la bande engendrée par $\mu$ dans l’espace complètement réticulé $\mathcal{M}(T)$ (chap. II, § 1, n° 5), il faut et il suffit que $v$ soit une mesure de base $\mu$.

On se ramène aussitôt, en considérant $v^+$ et $v^-$, au cas d’une mesure $v$ positive (n° 2, cor. de la prop. 2). Posons alors $v_n = \inf(n\mu, v)$; $v$ appartient à la bande engendrée par $\mu$ si et seulement si $v = \sup_n v_n$ (chap. II, 2e éd., § 1, n° 5, cor. de la prop. 6). Or $v_n$, majorée par $n\mu$, est une mesure de base $\mu$ d’après le th. 2; la relation $v = \sup_n v_n$ entraîne donc que $v$ est une mesure de base $\mu$ (cor. 1). Inversement, supposons que $v$ soit une mesure de base $\mu : v = g \cdot \mu$, où $g$ est localement $\mu$-intégrable et positive. On a alors $v_n = \inf(g, n) \cdot \mu$ (cor. de la prop. 2), et il résulte aussitôt du théorème de Lebesgue (chap. IV, § 4, n° 3, prop. 4) que $v = \sup_n v_n$.

#### Corollaire 3 {#int-v-s5-lem-3-cor-3 .statement}

Soit $\theta$ une mesure complexe; il existe une fonction universellement mesurable $v$, telle que $|v| = 1$, et qu’on ait $\theta = v \cdot |\theta|, \ |\theta| = \bar{v} \cdot \theta$.

Posons en effet $\theta = \theta_1 - \theta_2 + i(\theta_3 - \theta_4)$, où $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta^-)$; les mesures positives $\theta_i$ ($i = 1, 2, 3, 4$), étant majorées par $|\theta|$ (chap. III, 2e éd., § 1, n° 6, formule (17)), sont des mesures de base $|\theta|$ d’après le théorème 2. Il en résulte qu’il existe une fonction localement $|\theta|$-intégrable $v$ telle que $\theta = v . |\theta|$. La proposition 2 donne alors la relation $|\theta| = |v| . |\theta|$, ce qui entraîne que $|v| = 1$ localement $|\theta|$-presque partout (cor. 2 de la prop. 3). On a enfin, d’après la prop. 8, $\bar{v} . \theta = (v \bar{v}) . |\theta| = |\theta|$. La fonction $v$ n’étant définie qu’à une fonction localement $|\theta|$-négligeable près, on peut supposer que $v$ est universellement mesurable (§ 3, n° 4, prop. 7) et que $|v| = 1$ partout.

Remarques — 1) Supposons que $\lambda$ soit une mesure positive, que $v$ soit une fonction $\lambda$-mesurable telle que $|v| = 1$ localement $\lambda$-presque partout (ce qui entraîne que $v$ est localement $\lambda$-intégrable), et qu’on ait $\theta = v . \lambda$. La prop. 2 montre aussitôt que $\lambda = |\theta|$; autrement dit, la propriété de l’énoncé précédent caractérise la mesure positive $|\theta|$.

2) Si $|\theta| \leq a \mu$, où $\mu$ est une mesure positive et $a$ un nombre $\geq 0$, $\theta$ est une mesure de base $\mu$.

#### Corollaire 4 {#int-v-s5-lem-3-cor-4 .statement}

Soient $\rho$ et $\theta$ deux mesures complexes. Pour qu’il existe une fonction $u$, localement $\theta$-intégrable, telle que $\rho = u . \theta$, il faut et il suffit que tout compact $\theta$-négligeable soit $\rho$-négligeable.

Cette condition est évidemment nécessaire. Inversement, supposons que tout compact $\theta$-négligeable soit $\rho$-négligeable ; le théorème 2 entraîne l’existence d’une fonction localement $|\theta|$-intégrable $g$ telle que $|\rho| = g . |\theta|$. Le cor. 3 entraîne d’autre part l’existence d’une fonction $v_1$ (resp. $v_2$), de valeur absolue 1, mesurable pour la mesure $|\rho|$ (resp. $\theta$), telle que $\rho = v_1 . |\rho|$ (resp. $|\theta| = \bar{v}_2 . \theta$). D’après la prop. 8, on a alors $\rho = u . \theta$, où $u = v_1 g \bar{v}_2$.

#### Corollaire 5 {#int-v-s5-lem-3-cor-5 .statement}

Soient $\mu$ et $v$ deux mesures positives sur T. Les conditions 1), 2), 3) du th. 2 sont encore équivalentes aux suivantes:

4) Pour toute fonction numérique $f \geq 0$ $v$-intégrable et pour tout nombre $\varepsilon > 0$, il existe $\delta > 0$ tel que les relations $0 \leq h \leq f$ et $\int^* h \, d\mu \leq \delta$ entraînent $\int^* h \, dv < \varepsilon$.

5) Pour toute fonction $g \in \mathcal{K}_+(\mathrm{T})$ et tout nombre $\varepsilon > 0$, il existe $\delta > 0$ tel que, pour toute $h \in \mathcal{K}_+(\mathrm{T})$ majorée par $g$ et vérifiant $\int h \, d\mu \leq \delta$, on ait $\int h \, dv \leq \varepsilon$.

6) Pour tout ensemble compact $K \subset \mathrm{T}$ et tout nombre $\varepsilon > 0$, il existe $\delta > 0$ tel que les relations $A \subset K$ et $\mu^*(A) \leq \delta$ entraînent $v^*(A) \leq \varepsilon$.

Les implications 4) ⇒ 6) ⇒ 3) sont évidentes.

Supposons qu’il existe une fonction finie $k \geq 0$, universellement mesurable, localement $\mu$-intégrable, telle que $\nu = k . \mu$, et montrons que la condition 4) est remplie. Soient $f$ une fonction $\geq 0$, $\nu$-intégrable, et $\varepsilon > 0$. Pour tout entier $n \geq 0$, soit $A_n$ l’ensemble des $t \in T$ tels que $k(t) \geq n$. Les fonctions $f \varphi_{A_n}$ tendent simplement vers 0 en décroissant et sont majorées par $f$, donc il existe $N$ tel que $\int f \varphi_{A_N} d\nu \leq \varepsilon / 2$ (chap. IV, § 4, n° 3, prop. 4). Si $h$ est une fonction sur $T$ vérifiant $0 \leq h \leq f$ et $\int^* h \, d\mu \leq \varepsilon / 2N$, on a

$$
\nu^*(h) \leq \nu^*(h \varphi_{A_N}) + \nu^*(h(1 - \varphi_{A_N}))
$$

$$
\leq \nu^*(f \varphi_{A_N}) + \mu^*(h(1 - \varphi_{A_N})k) \leq \frac{\varepsilon}{2} + N \mu^*(h) \leq \varepsilon.
$$

On a ainsi prouvé que les conditions 4) et 6) sont équivalentes aux conditions du th. 2.

Il est clair que 4) entraîne 5). Enfin, si la condition 5) est remplie, $\nu$ appartient à la bande engendrée par $\mu$ (chap. II, § 2, n° 2, prop. 4), donc est de base $\mu$ (cor. 2).

#### Scholie {#int-v-s5-n5-sch-1 .statement}

Pour tout $\dot{f} \in L^1_{loc}(T, \mu ; \mathbf{B})$, posons $\varphi(\dot{f}) = f . \mu$, où $f \in \dot{f}$; l’application $\varphi$ est linéaire, croissante, injective (cor. 2 de la prop. 3), et admet pour image dans $\mathcal{M}(T)$ la bande $\mathbf{B}$ engendrée par $\mu$ (cor. 2 du th. 2). L’application $\varphi$ permet donc d’identifier $L^1_{loc}(T, \mu ; \mathbf{R})$ à un espace de mesures réelles sur $T$; comme tous les espaces $L^p_R(T, \mu)$ sont des sous-espaces de $L^1_{loc}(T, \mu ; \mathbf{R})$, ils peuvent eux aussi être identifiés à des sous-espaces de $\mathcal{M}(T)$. On a des considérations analogues pour les fonctions et mesures à valeurs complexes. On notera que l’application $\varphi$ envisagée ci-dessus est un isomorphisme des structures d’espace vectoriel ordonné de $L^1_{loc}$ et de $\mathbf{B}$, mais n’est évidemment pas un isomorphisme pour les structures d’espace vectoriel topologique de ces espaces.

Comme toute bande dans un espace complètement réticulé est elle-même un espace complètement réticulé (chap. II, § 1, n° 5), on voit que l’espace $L^1_{loc}$ est complètement réticulé; mais il convient de rappeler que la borne supérieure dans $L^1_{loc}$ d’une famille non dénombrable $(\dot{f}_\alpha)$ de classes d’équivalence n’est pas nécessairement identique à la classe de l’enveloppe supérieure des fonctions $f_\alpha$. Toutefois, nous avons vu que, pour une suite croissante $(f_n)$ de fonctions localement $\mu$-intégrables, dont l’enveloppe supérieure $f$ est localement $\mu$-intégrable, $f . \mu$ est la borne supérieure de la suite de mesures $(f_n . \mu)$ dans $\mathcal{M}(T)$ (cor. de la prop. 6).

Voici une conséquence intéressante du corollaire 3 du th. 2:

#### Proposition 9 {#int-v-s5-prop-9 .statement}

*Soit $\theta$ une mesure complexe bornée ; pour que $\theta$ soit une mesure positive, il faut et il suffit qu’on ait $\| \theta \| = \theta(1)$.*

Cette condition est évidemment nécessaire. Inversement, supposons qu’on ait $\| \theta \| = \int d\theta$, et désignons par $v$ une fonction $|\theta|$-mesurable, de valeur absolue 1, telle que $\theta = v . |\theta|$. Comme on a $\| \theta \| = \int d|\theta|$ (chap. III, 2e éd., § 1, n° 8, cor. 2 de la prop. 10), et $\int d\theta = \int v . d|\theta|$ (th. 1), l’hypothèse entraîne que $\int (1 - v) d|\theta| = 0$, et donc aussi que $\int \mathcal{R}(1 - v) d|\theta| = 0$. La fonction $\mathcal{R}(1 - v)$, étant positive, est donc nulle presque partout, ce qui entraîne que $v = 1$ presque partout, et achève la démonstration.

### 6. Mesures équivalentes

#### Proposition 10 {#int-v-s5-prop-10 .statement}

*Soient $\mu$ et $v$ deux mesures positives sur $T$. Les conditions suivantes sont équivalentes :

a) Les ensembles localement négligeables sont les mêmes pour $\mu$ et $v$.

b) Les bandes engendrées par $\mu$ et $v$ dans $\mathcal{M}(T)$ sont identiques.

c) On a $v = g . \mu$, où $g$ est localement $\mu$-intégrable et $g(t) > 0$ localement presque partout pour $\mu$.

Les conditions a) et b) sont équivalentes en vertu du cor. du th. 2 du n° 5. Si elles sont remplies, on a $v = g . \mu$ et $\mu = h . v$, où $g$ (resp. $h$) est positive et localement intégrable pour $\mu$ (resp. $v$). Donc (n° 4, prop. 8) $hg$ est localement $\mu$-intégrable, et on a $\mu = (hg) . \mu$. Il en résulte (n° 3, cor. 2 de la prop. 3) que $hg$ est égale à 1 localement presque partout pour $\mu$, de sorte que $g(t) > 0$ et $h(t) = 1/g(t)$ localement presque partout pour $\mu$. Réciproquement, supposons que $v = g . \mu$, avec $g(t) > 0$ localement presque partout pour $\mu$; comme $(1/g)g$ est définie localement presque partout et est localement $\mu$-intégrable, $1/g$ est localement $v$-intégrable et $(1/g) . v = \mu$ (n° 4, prop. 8).

#### Définition 3 {#int-v-s5-def-3 .statement}

*Sur un espace localement compact $T$, on dit que deux mesures complexes $\theta, \theta'$ sont équivalentes si les mesures $|\theta|$ et $|\theta'|$ satisfont aux conditions a), b), c) de la prop. 10.*

Pour que $\theta$ et $\theta'$ soient équivalentes, il faut et il suffit donc que $|\theta|$ et $|\theta'|$ le soient.

#### Remarque {#int-v-s5-n6-rem-1 .statement}

Si $\mu$ et $\nu$ sont deux mesures positives équivalentes, les fonctions mesurables définies dans $T$, à valeurs dans un espace topologique quelconque $G$, sont les mêmes pour $\mu$ et $\nu$, comme il résulte aussitôt de la prop. 4 du n° 3.

#### Proposition 11 {#int-v-s5-prop-11 .statement}

Soit $\mu$ une mesure positive sur $T$. Si $T$ est dénombrable à l’infini, il existe une fonction continue $h$ telle que $h(t) > 0$ pour tout $t \in T$ et que la mesure $\nu = h . \mu$ (équivalente à $\mu$) soit bornée.

En effet, soit $(K_n)$ une suite d’ensembles compacts formant un recouvrement de $T$, et pour tout $n$, soit $f_n$ une fonction de $\mathscr{K}(T)$ telle que $0 \leq f_n \leq 1$ et $f_n(t) = 1$ dans $K_n$ (chap. III, 2e éd., § 1, n° 2, lemme 1). Soit $(a_n)$ une suite de nombres $> 0$ telle que $\sum_n a_n < +\infty$; la série $h = \sum_n a_n f_n$ est alors normalement convergente dans $T$, et $h$ est par suite une fonction continue dans $T$, telle que $h(t) > 0$ pour tout $t \in T$, par construction. En posant $\nu = h . \mu$, on a alors (prop. 3 et chap. IV, § 1, n° 3, prop. 13)

$$
\nu^*(1) = \int^* h \, d\mu \leq \sum_n a_n \int f_n \, d\mu.
$$

En prenant par exemple $a_n = 2^{-n} (\int f_n \, d\mu)^{-1}$ lorsque $\int f_n \, d\mu > 1$, $a_n = 2^{-n}$ dans le cas contraire, on a $\sum_n a_n < +\infty$ et $\nu^*(1) < +\infty$, ce qui démontre la proposition.

#### Proposition 12 {#int-v-s5-prop-12 .statement}

Soit $(\mu_n)$ une suite de mesures positives bornées sur $T$; il existe une mesure positive bornée $\mu$ sur $T$ telle que la relation $\mu^*(N) = 0$ soit équivalente à « quel que soit $n$, $\mu_n^*(N) = 0$ »; chacune des mesures $\mu_n$ est de base $\mu$. En outre, si $\mu'$ est une seconde mesure positive sur $T$ ayant cette propriété, $\mu$ et $\mu'$ sont équivalentes.

La dernière partie de l’énoncé résulte aussitôt de la déf. 3. Pour démontrer l’existence de $\mu$, on peut se borner au cas où $\mu_n \neq 0$ pour tout $n$; la famille de mesures $\mu_n / 2^n \| \mu_n \|$ est alors sommable dans $\mathcal{M}(T)$, et sa somme $\mu$ est telle que $\| \mu \| \leq 1$. En outre, comme $\mu_n \leq 2^n \| \mu_n \| . \mu$, la relation $\mu(N) = 0$ entraîne $\mu_n(N) = 0$ pour tout $n$; inversement, si $N$ est un ensemble négligeable pour toutes les $\mu_n$, il est localement négligeable pour $\mu$ (§ 2, n° 2, cor. 2 de la prop. 1), et par suite $\mu$-négligeable puisque $\mu$ est bornée (§ 1, n° 2, cor. 2 de la prop. 7).

### 7. Mesures étrangères

Étant données deux mesures réelles $\rho, \sigma$ sur $T$, rappelons que l’on dit que $\rho$ et $\sigma$ sont étrangères si l’on à $\inf(|\rho|, |\sigma|) = 0$ dans $\mathcal{M}(T)$ (chap. II, § 1, n° 1). On sait que les mesures réelles étrangères à une mesure donnée forment une bande (chap. II, § 1, n° 5, th. 1). Cette définition s’étend aussitôt au cas des mesures complexes.

#### Définition 4 {#int-v-s5-def-4 .statement}

On dit qu’une mesure complexe $\theta$ sur $T$ est concentrée sur une partie $M$ de $T$, ou que $M$ porte $\theta$, si $\mathbf{C}M$ est localement négligeable pour $\theta$.

L’ensemble $M$ porte $\theta$ si et seulement s’il porte $|\theta|$. Il est équivalent de dire que $M$ porte $\theta$, ou que $M$ est $\theta$-mesurable et $\theta = \varphi_M \cdot \theta$. Si $\theta$ est concentrée sur $M$, toute mesure de base $|\theta|$ est concentrée sur $M$.

#### Proposition 13 {#int-v-s5-prop-13 .statement}

Pour que deux mesures complexes $\rho$ et $\sigma$ sur $T$ soient étrangères, il faut et il suffit qu’il existe dans $T$ deux ensembles $R$ et $S$ sans point commun, tels que $\rho$ soit concentrée sur $R$ et $\sigma$ sur $S$; $R$ et $S$ peuvent être supposés universellement mesurables.

Posons $\mu = |\rho|, v = |\sigma|, \lambda = \mu + v$; $\mu$ et $v$ étant majorées par $\lambda$, il existe deux fonctions localement $\lambda$-intégrables $u$ et $v$ (que l’on peut supposer universellement mesurables ($§ 3, \mathrm{n}^\circ 4$, prop. 7)) telles que $\mu = u \cdot \lambda, v = v \cdot \lambda$. On a alors

$$
\inf(|\rho|, |\sigma|) = \inf(\mu, v) = \inf(u, v) \cdot \lambda
$$

(n° 2, cor. de la prop. 2). Soit A (resp. B) l’ensemble des $t \in T$ tels que $u(t) > 0$ et $v(t) = 0$ (resp. $u(t) = 0$ et $v(t) > 0$). Si $\rho$ et $\sigma$ sont étrangères, on a $\inf(u, v) = 0$ localement $\lambda$-presque partout (n° 3, cor. 2 de la prop. 3), de sorte que les ensembles universellement mesurables disjoints A et B portent respectivement $\mu$ et $v$. Inversement, supposons que $\mu$ et $v$ soient portées respectivement par des ensembles disjoints $R$ et $S$; $\varphi_R$ est mesurable pour la mesure $\mu = u \cdot \lambda$, et $\mu = \varphi_R \cdot \mu$. D’après la prop. 8 du n° 4, la fonction $u' = u \varphi_R$ est $\lambda$-mesurable, et $\mu = u' \cdot \lambda$. De même, si $v' = v \varphi_S$, on a $v = v' \cdot \lambda$; on conclut en remarquant que $\inf(u', v') = 0$ (n° 2, cor de la prop. 2).

#### Corollaire 1 {#int-v-s5-prop-13-cor-1 .statement}

Pour toute mesure réelle $v$ sur $T$, il existe deux ensembles disjoints $M, N$ portant respectivement $v^+$ et $v^-$.

On aura soin de ne pas confondre la notion de support d’une mesure $v$, et celle d’ensemble où $v$ est concentrée. Le support $S$ de

On notera aussi que l’intersection des ensembles portant ν est l’ensemble des points t ∈ T tels que |ν|({t}) > 0, et peut être vide (par exemple dans le cas de la mesure de Lebesgue); il n’y a donc pas en général de plus petit ensemble portant ν.

#### Corollaire 2 {#int-v-s5-prop-13-cor-2 .statement}

Soient ρ et σ deux mesures complexes étrangères, et soient ρ′ et σ′ deux mesures complexes admettant des densités par rapport à ρ et à σ respectivement; ρ′ et σ′ sont alors étrangères.

#### Corollaire 3 {#int-v-s5-prop-13-cor-3 .statement}

Soient ρ et σ deux mesures complexes étrangères; on a alors |ρ + σ| = |ρ| + |σ|.

Désignons en effet par v (resp. w) une fonction universellement mesurable de valeur absolue 1 telle que ρ = v . |ρ| (resp. σ = w . |σ|) (cor. 3 du th. 2), par A un ensemble universellement mesurable portant ρ, tel que B = CA porte σ (prop. 13); on a alors aussi ρ + σ = (vφ_A + wφ_B) . (|ρ| + |σ|). La fonction vφ_A + wφ_B ayant une valeur absolue égale à 1, le corollaire résulte de la prop. 2.

#### Théorème 3 (Lebesgue) {#int-v-s5-thm-3 .statement}

Toute mesure complexe θ sur T peut s’écrire d’une seule manière sous la forme θ = g . μ + θ′, où g est localement μ-intégrable, et θ′ est une mesure étrangère à μ. On a alors |θ| = |g| . μ + |θ′|.

Lorsque θ est positive, ceci résulte aussitôt du th. de F. Riesz (chap. II, § 1, n° 5, th. 1) appliqué à l’espace complètement réticulé $\mathcal{M}(T)$ des mesures réelles sur T, et à la bande engendrée par μ dans cet espace, compte tenu du n° 5, cor. 2 du th. 2; de plus, θ′ et g . μ sont alors positives, ce qui entraîne que g est positive localement μ-presque partout (cor. 3 de la prop. 3). Pour traiter le cas où θ n’est pas positive, posons ν = |θ|, ν = f . μ + ν′ (où f est positive, et où ν′ et μ sont étrangères), et θ = v . ν, où v est une fonction universellement mesurable de valeur absolue 1 (cor. 3 du th. 2). Nous avons alors (prop. 8) θ = g . μ + θ′, avec g = vf (de sorte que |g| = f) et θ′ = v . ν′ (de sorte que |θ′| = ν′ d’après la prop. 2); les mesures θ′ et μ sont étrangères d’après le cor. 2 de la prop. 12. Il reste seulement à établir l’unicité de la décomposition. Supposons donc que $\theta = g . \mu + \theta' = g_1 . \mu + \theta'_1$, où $\theta_1$ et $\theta'_1$ sont étrangères à $\mu$; $|\theta' - \theta'_1|$ est majorée par $|\theta'| + |\theta'_1|$, donc $\theta' - \theta'_1$ est étrangère à $\mu$, et par conséquent aussi à $(g_1 - g) . \mu$. La relation $\theta' - \theta'_1 = (g_1 - g) . \mu$ entraîne alors que les deux membres sont nuls, ce qui prouve l’unicité.

Rappelons (th. 2, Scholie) que l’espace $L^1_{loc}(T, \mu; \mathbf{C})$ peut être identifié (au moyen de l’application $\dot{g} \mapsto g . \mu$) à un sous-espace de $\mathcal{M}_\mathbf{C}(T)$. Avec cette convention, le théorème 3 prend la forme suivante:

#### Corollaire {#int-v-s5-n7-cor-1 .statement}

*Il existe un projecteur* $p$ *de l’espace* $\mathcal{M}_\mathbf{C}(T)$ *sur l’espace* $L^1_{loc}(T, \mu; \mathbf{C})$, *dont le noyau* $\bar{p}^1(0)$ *est l’ensemble des mesures complexes étrangères à* $\mu$, *tel que*
$$
|\theta| = |p(\theta)| + |\theta - p(\theta)|, \qquad p(|\theta|) = |p(\theta)|
$$
*pour toute mesure complexe* $\theta$.

Si l’on restreint $p$ à l’ensemble des mesures bornées, on obtient un projecteur $p^1$ de l’espace $\mathcal{M}_\mathbf{C}^1(T)$ sur l’espace $L^1_\mathbf{C}(T, \mu)$; la relation $\| \theta \| = | \theta |(1)$ entraîne que $\| \theta \| = \| p^1(\theta) \| + \| \theta - p^1(\theta) \|$ pour toute mesure complexe bornée $\theta$.

### 8. *Applications: I. Dualité des espaces* $L^p$

Nous ne traiterons ici que le cas des espaces $L^p$ réels.

Rappelons que deux nombres $p, q$ tels que $1 \leq p \leq +\infty$, $1 \leq q \leq +\infty$, $1/p + 1/q = 1$, sont appelés des *exposants conjugués* (chap. IV, § 6, n° 4). Toute fonction $g \in \mathcal{L}^q$ définit une forme linéaire continue $\theta_g$ sur $L^p$, qu’on obtient par passage au quotient à partir de la forme linéaire $f \mapsto \int fg \, d\mu$ sur $\mathcal{L}^p$, et on a $N_q(g) = \| \theta_g \|$ (chap. IV, 2e éd., § 6, n° 4, cor. de la prop. 3). Par passage au quotient, on déduit donc de l’application $g \mapsto \theta_g$ une application linéaire isométrique $\varphi$ de $L^q$ dans le dual $(L^p)'$ de $L^p$. Nous allons montrer que, pour $1 \leq p < +\infty$, $\varphi$ applique $L^q$ *sur* $(L^p)'$, de sorte que nous pourrons désormais identifier l’espace de Banach $L^q$ à l’espace de Banach $(L^p)'$ par l’isomorphisme $\varphi$. En d’autres termes :

#### Théorème 4 {#int-v-s5-thm-4 .statement}

*Soient* $p$ *et* $q$ *deux exposants conjugués tels que* $1 \leq p < +\infty$. *Toute forme linéaire continue sur* $\mathcal{L}^p(T, \mu)$ *est du type* $f \mapsto \int fg \, d\mu$, *où* $g$ *est une fonction de* $\mathcal{L}^q(T, \mu)$ *dont la classe dans* $L^q$ *est bien déterminée.*

Montrons que $|v|(|f|) \leq a \cdot N_p(f)$ pour toute fonction $f$ de $\mathscr{K}(T)$. Il suffit de prouver cette formule pour $f \geq 0$. Or, pour toute fonction $\psi$ de $\mathscr{K}(T)$ telle que $|\psi| \leq f$, on a
$$
|v(\psi)| \leq a \cdot N_p(\psi) \leq a \cdot N_p(f);
$$
notre assertion résulte de l’expression de la valeur absolue d’une mesure donnée au chap. III, 2e éd., § 1, n° 6, formule (12). La relation $|v|(|f|) \leq a(\mu(|f|^p))^{1/p}$ s’étend aussitôt au cas où $f$ est la fonction caractéristique d’un compact, grâce à un passage à l’enveloppe inférieure, et entraîne alors que tout compact $\mu$-négligeable est $v$-négligeable, de sorte que $v$ est une mesure de base $\mu$ (n° 5, th. 2).

Il existe donc une fonction positive localement $\mu$-intégrable $h_1$ telle que $|v|(f) = \int f h_1 \, d\mu$ pour toute fonction $f \in \mathscr{K}(T)$. Montrons que $h_1$ est localement presque partout égale à une fonction de $\mathcal{L}^q$. Si la fonction $f \geq 0$ de $\mathscr{K}(T)$ est telle que $N_p(f) \leq 1$, on a $\int f h_1 \, d\mu = |v|(f) \leq a$. Pour toute application continue $f_0$ de $T$ dans $[0, 1]$, à support compact, on a donc $\sup \int (f_0 h_1) f \, d\mu \leq a$ lorsque $f$ parcourt l’ensemble des fonctions $\geq 0$ de $\mathscr{K}(T)$ telles que $N_p(f) \leq 1$. D’après la formule (11) du chap. IV, § 6, n° 4, on en déduit que $N_q(f_0 h_1) \leq a$. De là résulte que $\sup_K N_q(\varphi_K h_1) \leq a$ lorsque $K$ parcourt l’ensemble des parties compactes de $T$, et cela prouve notre assertion (§ 1, prop. 9).

Soit $v$ une fonction (réelle) de valeur absolue 1 universellement mesurable, telle que $v = v \cdot |v|$ (cor. 3 du th. 2), et soit $g = v h_1$; on a $v = g \cdot \mu$, et $g$ appartient à $\mathcal{L}^q$. On a, pour toute fonction $f \in \mathscr{K}(T), \theta(f) = v(f) = \int f g \, d\mu$. Autrement dit, les formes linéaires continues $\theta$ et $\theta_g$ coïncident dans $\mathscr{K}(T)$; elles sont donc égales dans $\mathcal{L}^p$, puisque $\mathscr{K}(T)$ est partout dense dans $\mathcal{L}^p$, et cela achève la démonstration.

#### Corollaire {#int-v-s5-n8-cor-1 .statement}

Pour tout nombre $p$ tel que $1 < p < \infty$, l’espace de Banach $L^p(T, \mu)$ est réflexif.

En général, le dual de $L^\infty$ n’est pas isomorphe à $L^1$, et par suite $L^1$ et $L^\infty$ ne sont pas réflexifs (exerc. 10). Nous allons caractériser les formes linéaires continues sur $L^\infty$ qui proviennent, par passage au quotient, d’une forme linéaire $f \mapsto \int fg\, d\mu$ sur $\mathcal{L}^\infty$, où $g \in \mathcal{L}^1$.

L’espace vectoriel ordonné $L^\infty(T, \mu)$, qui est un sous-espace de $L^1_{loc}(T, \mu)$, est complètement réticulé; en effet, si $(f_\alpha)$ est une famille de fonctions positives de $\mathcal{L}^\infty$, dont l’ensemble des classes $(\dot{f}_\alpha)$ est majoré dans $L^\infty$, il existe $a \geq 0$ tel que $N_\infty(f_\alpha) \leq a$ pour tout $\alpha$. Comme $L^1_{loc}(T, \mu)$ est complètement réticulé, la famille $(\dot{f}_\alpha)$ admet une borne supérieure $\dot{h}$ dans $L^1_{loc}(T, \mu)$; mais comme $\dot{a} \geq \dot{f}_\alpha$ pour tout $\alpha$, on a $\dot{h} \leq \dot{a}$, et par suite $N_\infty(h) \leq a$, d’où notre assertion.

#### Proposition 14 {#int-v-s5-prop-14 .statement}

Pour qu’une forme linéaire positive $\theta$ sur $\mathcal{L}^\infty$ soit du type $f \mapsto \int fg\, d\mu$, où $g \in \mathcal{L}^1$, il faut et il suffit que, pour toute famille filtrante croissante $(f_\alpha)_{\alpha \in A}$ de fonctions positives de $\mathcal{L}^\infty$, dont l’ensemble des classes $(\dot{f}_\alpha)_{\alpha \in A}$ est majoré dans $L^\infty$ et admet $\dot{h}$ comme borne supérieure dans cet espace, on ait
$$
\dot{\theta}(h) = \sup_{\alpha \in A} \dot{\theta}(f_\alpha).
$$

Montrons d’abord que la condition est nécessaire. En effet, la mesure $h.\mu$ est la borne supérieure dans $\mathcal{M}(T)$ de l’ensemble des mesures $f_\alpha.\mu$ (n° 5, Scholie); donc (chap. II, § 2, n° 2), pour toute fonction $\varphi \geq 0$ de $\mathscr{K}(T)$, on a $\int h\varphi\, d\mu = \sup_{\alpha \in A} \int f_\alpha \varphi\, d\mu$. Si maintenant $a$ est un nombre $\geq 0$ tel que $N_\infty(f_\alpha) \leq a$ pour tout $\alpha \in A$ (ce qui entraîne $N_\infty(h) \leq a$), pour tout $\varepsilon > 0$, il existe $\varphi \in \mathscr{K}(T)$ telle que $\varphi \geq 0$ et $N_1(g - \varphi) \leq \varepsilon$, d’où l’on tire $\int |f_\alpha|g - \varphi|\, d\mu \leq a\varepsilon$ pour tout $\alpha \in A$, et $\int h|g - \varphi|\, d\mu \leq a\varepsilon$. Comme $\sup_{\alpha \in A} \int f_\alpha g\, d\mu \leq \int hg\, d\mu$, cela prouve que les deux membres de cette inégalité sont égaux.

Pour établir que la condition est suffisante, nous utiliserons le lemme suivant :

#### Lemme 4 {#int-v-s5-lem-4 .statement}

1° Soit $f$ une fonction positive semi-continue inférieurement et bornée dans T. Alors sa classe $\dot{f}$ dans $L^\infty$ est la borne supérieure de l’ensemble des classes $\varphi$, où $\varphi$ parcourt l’ensemble des fonctions de $\mathscr{K}(T)$ telles que $0 \leq \varphi \leq f$.

2° Soit $f$ une fonction positive mesurable et bornée dans T. Alors sa classe $\dot{f}$ dans $L^\infty$ est la borne inférieure de l’ensemble des classes $\psi$, où $\psi$ parcourt l’ensemble des fonctions semi-continues inférieurement et bornées dans T, qui sont $\geq f$.

1° Soit $f'$ une fonction de $\mathcal{L}^\infty$ telle que $\dot{f}'$ soit la borne supérieure dans $L^\infty$ de l’ensemble des classes $\varphi$ des fonctions $\varphi$ de $\mathscr{K}(T)$ telles que $0 \leq \varphi \leq f$; on a évidemment $\dot{f}' \leq \dot{f}$. Soit U une partie ouverte relativement compacte de T; pour toute fonction $h$ de $\mathscr{K}(T)$ telle que $0 \leq h \leq f \varphi_U$, on a, par définition, $h(t) \leq f'(t)$ localement presque partout, donc $h(t) \leq f'(t)\varphi_U(t)$ presque partout; on en conclut que $\int h\,d\mu \leq \int f'\varphi_U\,d\mu$. Mais puisque $f\varphi_U$ est semi-continue inférieurement, $\int f\varphi_U\,d\mu = \sup \int h\,d\mu$, où $h$ parcourt l’ensemble des fonctions de $\mathscr{K}(T)$ telles que $0 \leq h \leq f\varphi_U$ (chap. IV, § 1, n° 1, déf. 1); on a donc

$$
\int f\varphi_U\,d\mu \leq \int f'\varphi_U\,d\mu,
$$

et comme $f'\varphi_U \leq f\varphi_U$ presque partout, on a nécessairement $f\varphi_U = f'\varphi_U$ presque partout, d’où $f = f'$ localement presque partout.

2° Soit $f'$ une fonction de $\mathcal{L}^\infty$ telle que $\dot{f}'$ soit la borne inférieure dans $L^\infty$ de l’ensemble des classes $\psi$ des fonctions $\psi$ semi-continues inférieurement, bornées et $\geq f$; on a $\dot{f}' \geq \dot{f}$. Soit K une partie compacte de T; pour toute fonction $h$, semi-continue inférieurement, bornée et majorant $f\varphi_K$, soit $\bar{h}$ la fonction égale à $h$ dans K, à $\|f\| + \|h\|$ dans $T - K$. Alors $\bar{h}$ est semi-continue inférieurement et $\geq f$, donc par définition $\bar{h}(t) \geq f'(t)$ localement presque partout; on en conclut que $h(t) \geq f'(t)\varphi_K(t)$ presque partout, d’où $\int h\,d\mu \geq \int f'\varphi_K\,d\mu$. Mais $\int f\varphi_K\,d\mu = \inf \int h\,d\mu$, où $h$ parcourt l’ensemble des fonctions semi-continues inférieurement, bornées et majorant $f\varphi_K$ (chap. IV, § 1, n° 3, déf. 3); on a donc

$$
\int f\varphi_K\,d\mu \geq \int f'\varphi_K\,d\mu,
$$

et comme $f\varphi_K \leq f'\varphi_K$ presque partout, on a nécessairement $f\varphi_K = f'\varphi_K$ presque partout, d’où $f = f'$ localement presque partout.

Ce lemme étant démontré, soit $\theta$ une forme linéaire positive sur $\mathcal{L}^\infty$ satisfaisant à la condition de l’énoncé de la prop. 14. La restriction de $\theta$ à l’espace $\mathscr{K}(T)$ est une mesure positive $\nu$ sur T. Nous allons montrer que, pour toute fonction positive $f \in \mathcal{L}^\infty(T, \mu)$, on a $\theta(f) = \nu^*(f)$. Supposons d’abord que $f$ soit semi-continue inférieurement (et bornée); d’après le lemme 4, $f$ est la borne supérieure de l’ensemble filtrant croissant des classes $\varphi$, où $\varphi$ parcourt l’ensemble filtrant $\Phi$ des fonctions de $\mathscr{K}(T)$ telles que $0 \leq \varphi \leq f$. Comme par hypothèse $\theta(f) = \sup_{\varphi \in \Phi} \theta(\varphi)$, et que $\nu^*(f) = \sup_{\varphi \in \Phi} \nu(\varphi)$ par définition, notre assertion est démontrée dans ce cas. Supposons en second lieu que $f$ soit $\mu$-mesurable et bornée; on a alors, par définition, $\nu^*(f) = \inf_{\psi \in \Psi} \nu^*(\psi)$, où $\psi$ parcourt l’ensemble filtrant décroissant $\Psi$ des fonctions semi-continues inférieurement, bornées et $\geq f$. Si $a \geq \|f\|$, en appliquant l’hypothèse de l’énoncé à l’ensemble filtrant croissant des classes des fonctions $a - \psi$, où $\psi \in \Psi$ et $\psi \leq a$, on voit, en vertu du lemme, que l’on a $\theta(f) = \inf_{\psi \in \Psi} \theta(\psi)$, et on a donc bien $\theta(f) = \nu^*(f)$. En particulier, pour toute fonction $\mu$-négligeable $f \geq 0$, on a $\theta(f) = 0$, donc $\nu^*(f) = 0$, et par suite (n° 5, th. 2) $\nu$ est une mesure de base $\mu$; en outre, $\nu^*(1) = \theta(1) < +\infty$, et par suite (cor. du th. 1) $\nu = g \cdot \mu$, où $g \in \mathcal{L}^1(T, \mu)$. Enfin, toute fonction $\mu$-mesurable étant $\nu$-mesurable, toute fonction positive $f \in \mathcal{L}^\infty(T, \mu)$ est $\nu$-intégrable, et on a $\int fg \, d\mu = \nu^*(f) = \theta(f)$, ce qui achève la démonstration.

On conclut de la prop. 14 que les formes linéaires sur $\mathcal{L}^\infty$ du type $f \mapsto \int fg \, d\mu$, où $g \in \mathcal{L}^1$, sont les différences $\theta_1 - \theta_2$, où $\theta_1$ et $\theta_2$ sont des formes linéaires positives satisfaisant à la condition de la prop. 14.

### 9. Applications: II. Fonctions de mesures

Soient $\mu_1, \mu_2, \ldots, \mu_n$ des mesures réelles sur T, et $u(x_1, \ldots, x_n)$ une fonction numérique finie, définie dans $\mathbf{R}^n$, et positivement homogène (c’est-à-dire (chap. I, § 1, n° 1) telle que

$$
u(\alpha x_1, \ldots, \alpha x_n) = \alpha u(x_1, \ldots, x_n)
$$

pour tout scalaire $\alpha \geq 0$. Il existe des mesures positives $\lambda$ sur T telles que $|\mu_i| \leq \lambda$ pour $1 \leq i \leq n$ (par exemple la somme

$$
\sum_{i=1}^{n} |\mu_i|). \text{ Soient } \lambda, \lambda' \text{ deux telles mesures sur T. On peut écrire } \mu_i = f_i \cdot \lambda = f'_i \cdot \lambda', \text{ où } f_i \text{ (resp. } f'_i) \text{ est mesurable et essentiellement bornée pour la mesure } \lambda \text{ (resp. } \lambda') \text{ (n° 5, th. 2). Nous allons établir le résultat suivant: pour que la fonction numérique } u(f_1, \ldots, f_n) \text{ soit localement intégrable pour } \lambda, \text{ il faut et il suffit que la fonction } u(f'_1, \ldots, f'_n) \text{ soit localement intégrable pour } \lambda', \text{ et on a alors}
$$
$$
u(f_1, \ldots, f_n) \cdot \lambda = u(f'_1, \ldots, f'_n) \cdot \lambda'.
$$
Comme on a $|\mu_i| \leq \inf(\lambda, \lambda')$, on peut se borner au cas où $\lambda \leq \lambda'$. On a alors $\lambda = g \cdot \lambda'$, où $g$ est une fonction $\lambda'$-mesurable telle que $0 \leq g \leq 1$ (n° 5, th. 2); d’où (n° 4, prop. 8)
$$
\mu_i = f_i \cdot (g \cdot \lambda') = (f_i g) \cdot \lambda';
$$
on en conclut (n° 3, cor. 2 de la prop. 3) que $f_i g$ est égale à $f'_i$ localement presque partout pour $\lambda'$. Par suite, on a, d’après (12),
$$
u(f'_1, \ldots, f'_n) = u(f_1 g, \ldots, f_n g) = u(f_1, \ldots, f_n) g
$$
localement presque partout pour $\lambda'$. Pour que $u(f'_1, \ldots, f'_n)$ soit localement $\lambda'$-intégrable, il faut et il suffit par conséquent que $u(f_1, \ldots, f_n) g$ soit localement intégrable pour $\lambda'$, donc (n° 4, prop. 8) que $u(f_1, \ldots, f_n)$ soit localement intégrable pour $\lambda$; et l’on a (n° 4, prop. 8)
$$
u(f'_1, \ldots, f'_n) \cdot \lambda' = (u(f_1, \ldots, f_n) g) \cdot \lambda' = u(f_1, \ldots, f_n) \cdot \lambda.
$$
La mesure $u(f_1, \ldots, f_n) \cdot \lambda$ ne dépend donc que des mesures $\mu_1, \ldots, \mu_n$ et de la fonction $u$; aussi la note-t-on $u(\mu_1, \ldots, \mu_n)$. Cette mesure est par suite définie lorsque $u$ est une fonction positivement homogène telle que, pour une mesure positive $\lambda$ majorant toutes les $|\mu_i|$, $u(f_1, \ldots, f_n)$ soit localement $\lambda$-intégrable, en désignant par $f_i$ la densité de $\mu_i$ par rapport à $\lambda$. On notera que cette condition est remplie lorsque $u$ est positivement homogène et continue: on a en effet alors
$$
|u(x_1, \ldots, x_n)| \leq a(|x_1| + |x_2| + \ldots + |x_n|)
$$
$(u$ étant bornée dans un voisinage assez petit de $(0, \ldots, 0))$, et comme $u(f_1, \ldots, f_n)$ est $\lambda$-mesurable (chap. IV, § 5, n° 3, th. 1), elle est localement $\lambda$-intégrable en vertu du critère d’intégrabilité (chap. IV, § 5, n° 6, th. 5).

Soient $u_1, \ldots, u_p$ des fonctions numériques positivement homogènes définies dans $\mathbf{R}^n$, et telles que les $p$ fonctions $g_k = u_k(f_1, \ldots, f_n)$ ($1 \leq k \leq p$) soient localement $\lambda$-intégrables. Soit $v$ une fonction numérique positivement homogène définie dans $\mathbf{R}^p$, et telle que $v(g_1, \ldots, g_p)$ soit localement $\lambda$-intégrable. Posons

$$
w(x_1, \ldots, x_n) = v(u_1(x_1, \ldots, x_n), \ldots, u_p(x_1, \ldots, x_n)).
$$

Alors la fonction $w$ est positivement homogène, $w(f_1, \ldots, f_n)$ est localement $\lambda$-intégrable, et on a par définition

$$
w(\mu_1, \ldots, \mu_n) = v(u_1(\mu_1, \ldots, \mu_n), \ldots, u_p(\mu_1, \ldots; \mu_n)).
$$

Dans le cas particulier des fonctions $x^+, x^-, |x|, x + y, \inf(x, y), \sup(x, y)$, les mesures définies par le procédé qui vient d’être décrit coïncident respectivement avec celles qui ont été notées $\mu^+, \mu^-, |\mu|, \mu + \nu, \inf(\mu, \nu), \sup(\mu, \nu)$; cela résulte aussitôt du cor. de la prop. 2 du n° 2. Si $\mu$ et $\nu$ sont deux mesures réelles, et $\theta = \mu + i \nu$, on a $|\theta| = \sqrt{\mu^2 + \nu^2}$; en effet, soient $\lambda$ une mesure $\geqslant 0$ majorant $|\mu|$ et $|\nu|$, et $f, g$ des fonctions localement $\lambda$-intégrables telles que $\mu = f \cdot \lambda, \nu = g \cdot \lambda$; on a

$$
\sqrt{\mu^2 + \nu^2} = \sqrt{f^2 + g^2} \cdot \lambda,
$$
$\theta = (f + ig) \cdot \lambda$, donc (n° 2, prop. 2) $|\theta| = \sqrt{f^2 + g^2} \cdot \lambda$.

On peut appliquer cette méthode à la fonction positivement homogène $(x_1^2 + \ldots + x_n^2)^{1/2}$, pour définir la longueur d’une courbe dans $\mathbf{R}^n$.

### 10. Mesures diffuses; mesures atomiques

#### Définition 5 {#int-v-s5-def-5 .statement}

On dit qu’une mesure $\theta$ sur $T$ est diffuse si, pour tout $t \in T$, on a $|\theta|(\{t\}) = 0$.

#### Exemple {#int-v-s5-n10-exa-1 .statement}

La mesure de Lebesgue sur $\mathbf{R}$ est diffuse (chap. IV, § 1, n° 3, Remarque 1).

Dire que $\theta$ est une mesure diffuse sur $T$ revient à dire que tout ensemble de complémentaire fini porte $|\theta|$, ou encore que $|\theta|$ est étrangère à toute mesure ponctuelle. Les mesures réelles diffuses forment donc une bande dans $\mathcal{M}(T)$ (chap. II, § 1, n° 5, th. 1).

Rappelons (chap. III, 2e éd., § 1, n° 3) qu’une mesure complexe $\rho$ sur $T$ est dite atomique si elle est de la forme $\sum_{t \in T} \alpha(t) \varepsilon_t$, où $\alpha$ est une fonction complexe sur $T$, telle que $\sum_{t \in K} |\alpha(t)| < +\infty$ pour tout compact K de T, ce qui exprime que la famille $(\alpha(t)\varepsilon_t)_{t\in T}$ est sommable (§ 2, n° 1, remarque 2). Il résulte alors de la remarque suivant le cor. 3 du th. 2 du n° 5 que $|\rho| = \sum_{t\in T} |\alpha(t)|\varepsilon_t$. La fonction $\alpha$ qui intervient dans ces formules est uniquement déterminée, car $\alpha(t) = \rho(\{t\})$. Une mesure atomique et une mesure diffuse sont étrangères.

#### Proposition 15 {#int-v-s5-prop-15 .statement}

*Toute mesure complexe $\sigma$ sur $T$ peut s’écrire d’une seule manière sous la forme $\rho + \theta$, où $\rho$ est une mesure atomique, $\theta$ une mesure diffuse ; on a alors $|\sigma| = |\rho| + |\theta|$*.

L’unicité de la décomposition est évidente, car $\rho$ étant atomique, et $\theta$ diffuse, on doit avoir $\rho = \sum_{t\in T} \rho(\{t\})\varepsilon_t = \sum_{t\in T} \sigma(\{t\})\varepsilon_t$, et $\theta = \sigma - \rho$. Pour établir l’existence, il suffit de remarquer que $\sum_{t\in K} |\sigma(\{t\})| \leq |\sigma|(K) < +\infty$ pour tout compact K, de sorte que l’on peut poser $\sum_{t\in T} \sigma(\{t\})\varepsilon_t = \rho$. La mesure $\sigma - \rho$ est évidemment diffuse, et la relation $|\sigma| = |\rho| + |\sigma - \rho|$ résulte aussitôt du cor. 3 de la prop. 13 du n° 8.

On notera que cette démonstration prouve que si $\sigma$ est portée par un ensemble M et si $|\sigma|(\{t\}) > 0$ pour tout $t \in M$, $\sigma$ est *atomique*.

## EXERCICES {#int-v-s5-exercises}

See the [exercises for § 5](exercises/s5/).
