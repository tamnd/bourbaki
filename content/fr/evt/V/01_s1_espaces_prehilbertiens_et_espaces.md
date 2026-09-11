---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE)
section: 1
section_title: Espaces préhilbertiens et espaces hilbertiens
lang: fr
source: evt-i-v-fr
pdf_pages: 0263-0279, 0321-0331
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes
      page: 0
      pdf_page: 263
    - "no": 2
      title: Formes hermitiennes positives
      page: 2
      pdf_page: 264
    - "no": 3
      title: Espaces préhilbertiens
      page: 4
      pdf_page: 266
    - "no": 4
      title: Espaces hilbertiens
      page: 6
      pdf_page: 268
    - "no": 5
      title: Sous-ensembles convexes d’un espace préhilbertien
      page: 9
      pdf_page: 271
    - "no": 6
      title: Sous-espaces vectoriels et orthoprojecteurs
      page: 12
      pdf_page: 274
    - "no": 7
      title: Dual d’un espace hilbertien
      page: 15
      pdf_page: 277
statements: 43
exercises: 37
content_sha256: 88ed7fa78df6c58b1d4a1f24ee532cfa29c82661af302faa7086380f0c5393bd
---

## § 1. ESPACES PRÉHILBERTIENS ET ESPACES HILBERTIENS

### 1. Formes hermitiennes

Rappelons la définition suivante donnée en Algèbre (A, IX, § 2, no 1) :

#### Définition 1 {#evt-v-s1-def-1 .statement}

Soit E un espace vectoriel sur le corps K. On appelle forme hermitienne (à gauche) sur E toute application $f$ de $E \times E$ dans K satisfaisant aux conditions suivantes (pour $x_1, x_2, x, y_1, y_2, y$ dans E et $\lambda, \mu$ dans K) :

(1)
$$
\begin{cases}
f(x_1 + x_2, y) = f(x_1, y) + f(x_2, y) \\
f(x, y_1 + y_2) = f(x, y_1) + f(x, y_2)
\end{cases}
$$

(2)
$$
\begin{cases}
f(\lambda x, y) = \overline{\lambda} f(x, y) \\
f(x, \mu y) = \mu f(x, y)
\end{cases}
$$

(3)
$$
f(x, y) = \overline{f(y, x)} .
$$

Lorsque le corps K est égal à $\mathbf{R}$, la notion de forme hermitienne sur E se réduit à celle de forme bilinéaire symétrique sur $E \times E$ (A, III, p. 70).

On observera que la seconde condition (1) et la seconde condition (2) sont des conséquences des trois autres.

$^1$ Pour le lecteur qui s'intéresse spécialement aux espaces hilbertiens, on signale que seuls le no 7 du § 1 et le no 8 du § 4 dépendent des résultats des chapitres III et IV. Le lecteur pourra d'ailleurs à ce sujet se reporter au « Résumé des principales propriétés des espaces de Banach » qui figure à la fin de ce volume. Les seules références aux chapitres I et II concernent la définition d'un ensemble convexe et d'une semi-norme (II, p.1 et p.8), celle de somme directe topologique (I, p. 4 ), de famille totale et de famille topologiquement libre (I, p. 12).

De (1) et (2) on déduit aussitôt que

$$
f\left( \sum_j \lambda_j x_j, \sum_k \mu_k y_k \right) = \sum_{j,k} \overline{\lambda}_j \mu_k f(x_j, y_k) .
$$

En particulier, si E est de dimension finie, et si $(e_j)_{1 \leq j \leq n}$ est une base de E, on a,
pour $x = \sum_{j=1}^n \xi_j e_j$ et $y = \sum_{j=1}^n \eta_j e_j$,
$$
f(x, y) = \sum_{j,k} \alpha_{jk} \overline{\xi}_j \eta_k
$$
pour tout couple d’indices $j, k$; elle entraîne en particulier que les nombres $\alpha_{jj}$ sont réels.

D’après (3), le nombre $Q(x) = f(x, x)$ est réel pour tout $x \in E$. Par ailleurs, on établit aussitôt les formules suivantes, dites de *polarisation*

$$
4f(x, y) = \sum_{\varepsilon^2 = 1} \varepsilon Q(x + \varepsilon y) \quad \text{si } K = \mathbf{R},
$$
$$
4f(x, y) = \sum_{\varepsilon^4 = 1, \varepsilon \in \mathbf{C}} \varepsilon Q(x + \overline{\varepsilon} y) \quad \text{si } K = \mathbf{C}.
$$

#### Remarque {#evt-v-s1-n1-rem-1 .statement}

On notera que la formule (6) est valable pour toute forme *sesquilinéaire* sur $E \times E$ (c’est-à-dire toute fonction $f$ satisfaisant à (1) et (2), mais non nécessairement à (3)). Cette remarque montre que, lorsque $K = \mathbf{C}$, une forme sesquilinéaire $f$ telle que $f(x, x)$ soit réel pour tout $x \in E$ est nécessairement hermitienne : la relation (6) donne alors $\overline{f(y, x)} = f(x, y)$ puisque l’on a $y + \varepsilon x = \varepsilon (x + \overline{\varepsilon} y)$ et $Q(\varepsilon z) = Q(z)$ lorsque $\varepsilon^4 = 1$.

Des formules de polarisation, on tire en particulier :

#### Proposition 1 {#evt-v-s1-prop-1 .statement}

*Si $f$ est une forme hermitienne sur $E$, et $M$ un sous-espace vectoriel de $E$ tel que $f(x, x) = 0$ pour tout $x \in M$, on a aussi $f(x, y) = 0$ pour tout couple de points $x, y$ de $M$*.

Soit $f$ une forme hermitienne sur $E$; l’ensemble $N$ des $x \in E$ tels que $f(x, y) = 0$ pour tout $y \in E$ est un sous-espace vectoriel de $E$. Il résulte de (3) que, si $x_1 \equiv x_2$ (mod. $N$) et $y_1 \equiv y_2$ (mod. $N$), on a $f(x_1, y_1) = f(x_2, y_2)$; on définit donc sur l’espace quotient $E/N$ une forme sesquilinéaire $f$ en posant $f(\dot{x}, \dot{y}) = f(x, y)$ pour tout $x \in \dot{x}$ et tout $y \in \dot{y}$; il est clair que $f$ est hermitienne et que la relation «$f(\dot{x}, \dot{y}) = 0$ pour tout $\dot{y} \in E/N$» entraîne $\dot{x} = 0$ dans $E/N$, autrement dit (A, IX) $f$ est *séparante*. On dit que $f$ est la forme hermitienne séparante *associée* à $f$.

### 2. Formes hermitiennes positives

#### Définition 2 {#evt-v-s1-def-2 .statement}

*Soit $E$ un espace vectoriel sur le corps $K$. On dit qu’une forme hermitienne $f$ sur $E$ est positive si l’on a $f(x, x) \geq 0$ pour tout $x \in E$*.

Il est clair que les formes hermitiennes sur un espace vectoriel $E$ forment un espace vectoriel *sur le corps* $\mathbf{R}$ (mais non sur le corps $\mathbf{C}$ lorsque $K = \mathbf{C}$); dans cet espace, les formes hermitiennes positives constituent un *cône convexe pointé saillant* (II, p. 11) comme il résulte de la déf. 2 et de la prop. 1.

#### Proposition 2 {#evt-v-s1-prop-2 .statement}

Si $f$ est une forme hermitienne positive, on a

$$
|f(x, y)|^2 \leq f(x, x)\ f(y, y)
$$

quels que soient $x$ et $y$ dans $E$ (inégalité de Cauchy-Schwarz).

Supposons d’abord qu’on ait $f(y, y) \neq 0$. Pour tout $\xi \in K$, on a

$$
f(y, y)\ f(x + \xi y, x + \xi y) \geq 0
$$

ce qui s’écrit

$$
f(x, x)\ f(y, y) - |f(x, y)|^2 + (\overline{\xi} f(y, y) + \overline{f(x, y)}) (\overline{\xi} f(y, y) + f(x, y)) \geq 0 .
$$

En remplaçant $\xi$ par $-\overline{f(x, y)}/f(y, y)$ dans cette inégalité, on obtient (7). Raisonnement analogue si $f(x, x) \neq 0$.

Enfin, si $f(x, x) = f(y, y) = 0$, on a $f(x + \xi y, x + \xi y) \geq 0$ pour tout $\xi \in K$, ce qui s’écrit alors

$$
\xi f(x, y) + \overline{\xi f(x, y)} \geq 0 .
$$

Remplaçant $\xi$ par $-\overline{f(x, y)}$ dans cette inégalité, il vient $-2|f(x, y)|^2 \geq 0$, d’où $f(x, y) = 0$; on a encore (7) dans ce cas.

#### Corollaire 1 {#evt-v-s1-prop-2-cor-1 .statement}

Si $f$ est une forme hermitienne positive, l’ensemble $N$ des $x \in E$ tels que $f(x, x) = 0$ est identique au sous-espace vectoriel des $x \in E$ tels que $f(x, y) = 0$ pour tout $y \in E$.

#### Corollaire 2 {#evt-v-s1-prop-2-cor-2 .statement}

Pour qu’une forme hermitienne positive $f$ soit séparante, il faut et il suffit que la relation $x \neq 0$ entraîne $f(x, x) > 0$.

Cela résulte immédiatement du cor. 1.

Pour toute forme hermitienne positive $f$ sur $E$, la forme hermitienne séparante associée à $f$ (V, p. 2) est évidemment une forme hermitienne positive sur $E/N$.

#### Proposition 3 {#evt-v-s1-prop-3 .statement}

Soit $f$ une forme hermitienne positive sur $E$. Posons

$$
p(x) = f(x, x)^{1/2}
$$

pour tout $x \in E$. Alors $p$ est une semi-norme sur $E$, et c’est une norme si et seulement si $f$ est séparante.

Tout revient à prouver l’inégalité $p(x + y) \leq p(x) + p(y)$. Or, on a

$$
f(x + y, x + y) = f(x, x) + f(y, y) + f(x, y) + \overline{f(x, y)}
$$

et, d’après l’inégalité de Cauchy-Schwarz

$$
f(x + y, x + y) \leq f(x, x) + f(y, y) + 2(f(x, x)\ f(y, y))^{1/2}
$$
$$
= (f(x, x)^{1/2} + f(y, y)^{1/2})^2 .
$$

#### Remarque 1 {#evt-v-s1-n2-rem-1 .statement}

Supposons $f$ positive et séparante, et soient $x, y$ deux vecteurs $\neq 0$. La démonstration de l’inégalité de Cauchy-Schwarz montre que, si les deux membres de (7) sont égaux, il existe un scalaire $\xi$ tel que $f(x + \xi y, x + \xi y) = 0$ donc $x + \xi y = 0$, autrement dit, $x$ et $y$ sont linéairement dépendants ; la réciproque est immédiate. La démonstration de l’inégalité (8) montre alors que l’égalité $p(x + y) = p(x) + p(y)$ n’est possible que si $x$ et $y$ sont linéairement dépendants ; si $y = \lambda x$, l’égalité précédente s’écrit $|1 + \lambda| = 1 + |\lambda|$, et entraîne donc que $\lambda$ est réel et positif.

#### Remarque 2 {#evt-v-s1-n2-rem-2 .statement}

Soit $f$ une forme hermitienne positive sur $E$, et munissons $E$ de la semi-norme $x \mapsto f(x, x)^{1/2}$; si $\hat{f}$ est la forme hermitienne positive séparante associée à $f$, définie sur $E/N$, l’espace normé obtenu en munissant $E/N$ de la norme $x \mapsto \hat{f}(x, x)^{1/2}$ est l’espace normé associé à $E$ (II, p. 5).

#### Définition 3 {#evt-v-s1-def-3 .statement}

*Soit* $E$ *un espace vectoriel sur le corps* $K$. *On dit qu’une semi-norme* $p$ *sur* $E$ *est préhilbertienne s’il existe une forme hermitienne positive* $f$ *sur* $E$ *telle que* $p(x) = f(x, x)^{1/2}$ *pour tout* $x \in E$.

On notera que, pour une semi-norme $p$ sur $E$, il existe au plus une forme hermitienne positive $f$ telle que $p(x) = f(x, x)^{1/2}$ pour tout $x \in E$; cela résulte des formules de polarisation (V, p. 2).

### 3. Espaces préhilbertiens

#### Définition 4 {#evt-v-s1-def-4 .statement}

*On appelle espace préhilbertien un ensemble* $E$ *muni d’une structure d’espace vectoriel sur* $K$ *et d’une forme hermitienne positive. On dit que* $E$ *est un espace préhilbertien réel* (resp. *complexe*) *lorsque* $K = \mathbf{R}$ (resp. $K = \mathbf{C}$).

#### Exemple 1 {#evt-v-s1-n3-exa-1 .statement}

La forme $(\lambda, \mu) \mapsto \overline{\lambda} \mu$ définit sur $K$ une structure d’espace préhilbertien, dite *canonique*. Lorsque $K$ est considéré comme espace préhilbertien, il s’agit toujours, sauf mention expresse du contraire, de cette structure.

#### Exemple 2 {#evt-v-s1-n3-exa-2 .statement}

Soit $I$ un intervalle (borné ou non) de $\mathbf{R}$, et soit $E$ l’ensemble des fonctions réglées (FVR, II, p. 4) définies dans $I$, à valeurs dans $\mathbf{C}$ et à support compact. Il est clair que $E$ est un espace vectoriel sur $\mathbf{C}$; soit $f$ la forme sesquilinéaire $(x, y) \mapsto \int_I \overline{x(t)}\ y(t)\ dt$; il est immédiat que $f$ est une forme hermitienne positive sur $E$, et définit donc sur cet espace une structure d’espace préhilbertien.

#### Exemple 3 {#evt-v-s1-n3-exa-3 .statement}

Soit $n \geqslant 0$ un entier. Sur l’espace $K^n$, on définit une structure d’espace préhilbertien, au moyen de la forme hermitienne

$$
(x, y) \mapsto \sum_{j=1}^n \overline{x_j} y_j
$$

(pour $x = (x_1, \ldots, x_n)$ et $y = (y_1, \ldots, y_n)$). Lorsque $K = \mathbf{R}$, on retrouve le produit scalaire de deux vecteurs de $\mathbf{R}^n$ (TG, VI, p. 8).

#### Exemple 4 {#evt-v-s1-n3-exa-4 .statement}

\* Soit $\ell^2$ (ou $\ell^2(\mathbf{N})$) l’ensemble des suites $x = (x_n)_{n \in \mathbf{N}}$ d’éléments de $K$ telles que $\sum_{n=0}^\infty |x_n|^2$ soit fini. On montre que $\ell^2$ est un sous-espace vectoriel de $K^\mathbf{N}$ et l’on définit une structure d’espace préhilbertien sur $\ell^2$ au moyen de la forme hermitienne

$$
(x, y) \mapsto \sum_{n=0}^\infty \overline{x_n} y_n \quad (cf.\ V, p.18).
$$

#### Exemple 5 {#evt-v-s1-n3-exa-5 .statement}

Soient $E$ un espace préhilbertien réel, $f$ la forme bilinéaire symétrique correspondante sur $E$. Soit $E_{(c)}$ l’espace vectoriel complexifié de $E$; on identifie $E$ à un sous-ensemble de $E_{(c)}$ par l’application $x \mapsto 1 \otimes x$, de sorte que tout élément de $E_{(c)}$ s’écrit de manière unique sous la forme $x_1 + ix_2$ avec $x_1, x_2$ dans E. L’application $f$ s’étend de manière unique en une forme hermitienne $f_{(c)}$ sur $E_{(c)}$; on a
$$
f_{(c)}(x_1 + ix_2, y_1 + iy_2) = f(x_1, y_1) + f(x_2, y_2) + i(f(x_1, y_2) - f(x_2, y_1)) .
$$
En particulier, on a
$$
f_{(c)}(x_1 + ix_2, x_1 + ix_2) = f(x_1, x_1) + f(x_2, x_2) \geqslant 0 ,
$$
donc $f_{(c)}$ est positive. On dit que $E_{(c)}$, muni de $f_{(c)}$, est l’espace préhilbertien complexifié de E.

Lorsqu’on n’a à considérer, sur un espace vectoriel E, qu’une seule structure d’espace préhilbertien, la valeur, pour un couple $(x, y)$ de points de E, de la forme hermitienne qui définit la structure considérée, se note $\langle x|y \rangle_E$ ou plus simplement $\langle x|y \rangle$ si aucune confusion n’est à craindre. Ce nombre s’appelle le produit scalaire $^1$ de x et de y (carré scalaire de x si $y = x$). Deux vecteurs $x, y$ sont dits orthogonaux si $\langle x|y \rangle = 0$. La fonction $x \mapsto \|x\| = \langle x|x \rangle^{1/2}$ est alors une semi-norme sur l’espace vectoriel E (V, p. 3); un espace préhilbertien est toujours considéré comme muni de cette semi-norme (et par suite aussi de la topologie et de la structure uniforme correspondantes).

Avec ces notations, dans un espace préhilbertien E, l’inégalité de Cauchy-Schwarz s’écrit
$$
|\langle x|y \rangle| \leqslant \|x\| \cdot \|y\| .
$$
Par suite, le produit scalaire est une forme sesquilinéaire continue sur $E \times E$ (II, p. 6, prop. 4).

Pour que E soit séparé, il faut et il suffit que $x \mapsto \|x\|$ soit une norme sur E, autrement dit que la forme hermitienne $(x, y) \mapsto \langle x|y \rangle$ soit positive et séparante; il revient au même de dire que $0$ est le seul vecteur de E orthogonal à lui-même.

Conformément aux définitions générales (E, IV, p. 6), un isomorphisme d’un espace préhilbertien E sur un espace préhilbertien F est une application linéaire bijective $u$ de E sur F telle que
$$
\langle u(x)|u(y) \rangle = \langle x|y \rangle
$$
quels que soient $x$ et $y$ dans E. On déduit de là $\|u(x)\| = \|x\|$ pour tout $x \in E$, et $u$ est évidemment un isomorphisme pour les structures d’espace vectoriel topologique de E et de F ; si E et F sont séparés, $u$ est une isométrie de E sur F. Réciproquement, si $u$ est une application linéaire bijective de E sur F, telle que $\|u(x)\| = \|x\|$ pour tout

$^1$ Il nous arrivera parfois d’écrire $(x|y)$ pour $\langle y|x \rangle$. Notons que la formule (4) de V, p. 2, prend les formes équivalentes :

$$(4\ bis)$$
$$
\langle \sum_i \lambda_i x_i | \sum_j \mu_j y_j \rangle = \sum_{i,j} \overline{\lambda}_i \mu_j \langle x_i | y_j \rangle .
$$

$$(4\ ter)$$
$$
(\sum_i \lambda_i x_i | \sum_j \mu_j y_j) = \sum_{i,j} \lambda_i \overline{\mu}_j \langle x_i | y_j \rangle .
$$

x ∈ E, les formules de polarisation (V, p. 2) montrent que u est un isomorphisme d’espaces préhilbertiens de E sur F.

Soient E un espace préhilbertien complexe, ⟨ x|y ⟩ le produit scalaire dans E. Sur l’ensemble E, on peut définir une seconde structure d’espace vectoriel par rapport à C, en gardant la même loi de groupe additif, et prenant comme loi de composition externe (λ, x) ↦ λ̄x (A, II, p. 30); pour cette structure d’espace vectoriel, (x, y) ↦ ⟨ y|x ⟩ est une forme hermitienne positive. L’espace préhilbertien E obtenu en munissant E de cette nouvelle structure d’espace vectoriel et de cette nouvelle forme hermitienne, est dit conjugué à l’espace E. Un isomorphisme u de E sur E est une application semi-linéaire de E sur lui-même (relative à l’automorphisme ξ ↦ ξ̄ de C) telle que ⟨ u(y)|u(x) ⟩ = ⟨ x|y ⟩ ou encore ⟨ u(x)|u(y) ⟩ = ⟨ x|y ⟩ (pour x, y dans E); on dit encore qu’une telle application est un semi-automorphisme de l’espace préhilbertien E.

Si E est un espace préhilbertien, M un sous-espace vectoriel de E, la restriction à M × M du produit scalaire ⟨ x|y ⟩ est une forme hermitienne positive sur M, qui définit donc sur M une structure d’espace préhilbertien; on dit que cette structure est induite par celle de E, ou encore que M est un sous-espace préhilbertien de E.

### 4. Espaces hilbertiens

#### Définition 5 {#evt-v-s1-def-5 .statement}

On appelle espace hilbertien (ou espace de Hilbert) un espace préhilbertien séparé et complet. On dit qu’une norme sur un espace vectoriel E (sur K) est hilbertienne si elle est préhilbertienne et si l’espace normé E est complet.

Si E est un espace hilbertien et M un sous-espace vectoriel fermé de E, la structure d’espace préhilbertien induite sur M est en fait une structure d’espace hilbertien. On dit dans ce cas que M, muni de la structure induite, est un sous-espace hilbertien de E.

#### Exemple 1 {#evt-v-s1-n4-exa-1 .statement}

Les espaces préhilbertiens définis dans les exemples 1, 3, 4 de V, p. 4, sont des espaces hilbertiens. Par contre, l’espace préhilbertien E défini dans l’exemple 2 n’est ni séparé, ni complet. Le complexifié d’un espace hilbertien est un espace hilbertien.

#### Exemple 2 {#evt-v-s1-n4-exa-2 .statement}

\* Soit X un espace topologique séparé et soit μ une mesure positive sur X. Notons L²(X, μ) l’espace formé des classes d’équivalence pour μ des fonctions de carré μ-intégrable sur X à valeurs dans C. C’est un espace hilbertien complexe, dont le produit scalaire est donné par

$$
\langle f|g \rangle = \int_X \overline{f(x)}\ g(x)\ d\mu(x) .
$$

#### Exemple 3 {#evt-v-s1-n4-exa-3 .statement}

\* Soit n ≥ 1 un entier et soit U un ouvert de Rⁿ. On note μ la mesure sur U induite par la mesure de Lebesgue sur Rⁿ, et l’on pose $\mathcal{H}^0 = L^2(U, \mu)$. On note $\mathcal{H}^1$ l’espace des fonctions $f \in \mathcal{H}^0$ ayant la propriété suivante : pour $1 \leq i \leq n$, il existe une fonction $g_i \in \mathcal{H}^0$ telle que

$$
\int_U g_i(x)\ h(x)\ d\mu(x) = - \int_U f(x)\ D_i h(x)\ d\mu(x)
$$

pour toute fonction h de classe $C^1$ à support compact dans U. La fonction $g_i$ est définie de manière unique (à l’équivalence pour μ près) et se note $D_i f$ ou $\partial f / \partial x_i$ (i-ième dérivée partielle). Par récurrence sur l’entier $s \geqslant 1$, on définit $\mathcal{H}^s$ comme l’ensemble des fonctions $f \in \mathcal{H}^1$ telles que $D_i f \in \mathcal{H}^{s-1}$ pour $1 \leqslant i \leqslant n$. On définit un produit scalaire sur $\mathcal{H}^s$ par la formule
$$
\langle f | g \rangle = \sum_{k=0}^s \sum_{1 \leqslant i_1 \leqslant \cdots \leqslant i_k \leqslant n} \int \overline{D_{i_1} \cdots D_{i_k} f} \cdot D_{i_1} \cdots D_{i_k} g d\mu .
$$
Alors $\mathcal{H}^s$ est un espace hilbertien complexe, qu’on appelle *espace de Sobolev* d’indice $s$.

#### Exemple 4 {#evt-v-s1-n4-exa-4 .statement}

\* Soit $X$ une variété différentielle de classe $C^r$ (avec $r \geqslant 1$), pure de dimension finie $n$. Soit $L$ le complémentaire, dans le fibré vectoriel $\Lambda^n T(X)$, de l’image de la section nulle. Pour tout nombre réel $\lambda \neq 0$, l’application $u \mapsto \lambda u$ de $\Lambda^n T(X)$ dans lui-même laisse stable $L$.

Soit $\alpha$ un nombre complexe. On appelle *densité d’ordre* $\alpha$ sur $X$ une fonction $\omega$ sur $L$, à valeurs complexes, telle que l’on ait $\omega(\lambda u) = |\lambda|^{\alpha} \omega(u)$ pour $u \in L$ et $\lambda$ réel non nul. On dit qu’une densité $\omega$ d’ordre 1 est *localement intégrable* s’il existe un recouvrement ouvert $(U_i)_{i \in I}$ de $X$, et pour chaque $i \in I$ un système de coordonnées $\xi_i = (\xi_i^1, \ldots, \xi_i^n)$ dans $U_i$ et une fonction $f_i$ à valeurs complexes sur $\xi_i(U_i)$ satisfaisant aux conditions suivantes :

a) La fonction $f_i$ est localement intégrable sur l’ouvert $\xi_i(U_i)$ de $\mathbf{R}^n$ par rapport à la mesure de Lebesgue $\mu$;
b) soit $x \in U_i$; si $(\partial_{1,i,x}, \ldots, \partial_{n,i,x})$ est la base de $T_x X$ associée au système de coordonnées $(\xi_i^1, \ldots, \xi_i^n)$ dans $U_i$, on a
$$
\omega(\partial_{1,i,x} \wedge \cdots \wedge \partial_{n,i,x}) = f_i(\xi_i^1(x), \ldots, \xi_i^n(x)) .
$$
Il existe alors sur $X$ une mesure $\tilde{\omega}$ et une seule telle que pour tout $i \in I$, l’image par $\xi_i$ de la restriction de $\tilde{\omega}$ à $U_i$ soit égale à la mesure $f_i \cdot \mu$ (*cf.* VAR, R, 10.4.3).

Soit $\mathcal{V}$ (resp. $\mathcal{N}$) l’espace vectoriel des densités $\omega$ d’ordre 1/2 telles que la mesure associée à la densité $|\omega|^2$ d’ordre 1 soit bornée (resp. nulle). Soient $\omega_1$ et $\omega_2$ dans $\mathcal{V}$; alors $\omega = \overline{\omega}_1 \omega_2$ est une densité d’ordre 1, et la mesure $\tilde{\omega}$ associée à $\omega$ est bornée ; le nombre $\int_X \tilde{\omega}$ ne dépend que des classes $\dot{\omega}_1$ et $\dot{\omega}_2$ de $\omega_1$ et $\omega_2$ modulo $\mathcal{N}$ et se note $\langle \omega_1 | \omega_2 \rangle$ ou $\langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$. Alors l’application $(\dot{\omega}_1, \dot{\omega}_2) \mapsto \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$ munit l’espace vectoriel $\Omega_{1/2}(X) = \mathcal{V}/\mathcal{N}$ d’une structure d’espace hilbertien complexe.

#### Exemple 5 {#evt-v-s1-n4-exa-5 .statement}

\* Soit $D$ le disque ouvert de centre 0 et rayon 1 dans $\mathbf{C}$. L’espace de Hardy $H^2(D)$ se compose des fonctions holomorphes $f : D \to \mathbf{C}$ pour lesquelles on a
$$
\sup_{0 < R < 1} \int_0^1 |f(R \cdot e(\theta))|^2 \, d\theta < + \infty .
$$
Si $f_1$ et $f_2$ appartiennent à $H^2(D)$, la limite
$$
\langle f_1 | f_2 \rangle = \lim_{R \to 1} \int_0^1 \overline{f_1(R \cdot e(\theta))} \cdot f_2(R \cdot e(\theta)) \, d\theta
$$
existe ; l’application $(f_1, f_2) \mapsto \langle f_1 | f_2 \rangle$ munit l’espace vectoriel $H^2(D)$ d’une structure d’espace hilbertien complexe.

Pour qu’une fonction $f : D \to \mathbf{C}$ appartienne à $H^2(D)$, il faut et il suffit qu’il existe une suite $(a_n)_{n \in \mathbf{N}}$ de nombres complexes telle que $\sum_{n=0}^\infty |a_n|^2 < + \infty$ et que
$$
f(z) = \sum_{n=0}^\infty a_n z^n
$$
pour tout $z \in D$. On a alors $\|f\|^2 = \sum_{n=0}^\infty |a_n|^2$, d’où un isomorphisme de $H^2(D)$ avec l’espace hilbertien $\ell^2$ (V, p. 4).

Tout espace préhilbertien séparé est isomorphe à un sous-espace partout dense d’un espace hilbertien déterminé à un isomorphisme près ; de façon précise :

#### Proposition 4 {#evt-v-s1-prop-4 .statement}

Soient E un espace préhilbertien séparé, $\hat{E}$ l’espace normé complété de E (TG, IX, p. 33). Le produit scalaire $(x, y) \mapsto \langle x|y \rangle$ se prolonge par continuité en une forme hermitienne positive et séparante sur $\hat{E}$, qui définit sur $\hat{E}$ une structure d’espace hilbertien.

L’existence du prolongement de $(x, y) \mapsto \langle x|y \rangle$ à $\hat{E} \times \hat{E}$ résulte de la continuité de cette forme sesquilinéaire dans $E \times E$ (TG, III, p. 50, th. 1). En outre, ce prolongement, que nous noterons aussi $(x, y) \mapsto \langle x|y \rangle$, est une forme hermitienne et satisfait à la relation $\langle x|x \rangle = \|x\|^2$, en vertu du principe de prolongement des identités ($\|x\|$ désignant la norme sur $\hat{E}$ obtenue en prolongeant par continuité la norme sur E) ; cela prouve que la relation $\langle x|x \rangle = 0$ entraîne $x = 0$ dans $\hat{E}$, donc que la forme $(x, y) \mapsto \langle x|y \rangle$ est positive et séparante, et définit par suite sur $\hat{E}$ une structure d’espace hilbertien.

On dit que cet espace hilbertien est le complété de l’espace préhilbertien séparé E.

\* Exemple 6. — Soit U un ouvert de $\mathbf{R}^n$ ($n \geqslant 1$). Soit $\mathcal{C}_0^1(U)$ l’espace vectoriel des fonctions de classe $C^1$ à support compact dans U. On définit sur $\mathcal{C}_0^1(U)$ une structure d’espace préhilbertien séparé dont le produit scalaire est donné par

$$
\langle f|g \rangle = \sum_{i=1}^n \int_U \overline{D_i f(x)} \cdot D_i g(x) \, dx .
$$

Cet espace préhilbertien n’est pas complet. Son complété s’appelle l’espace de Dirichlet associé à U. \*

#### Corollaire {#evt-v-s1-n4-cor-1 .statement}

Soient V un espace vectoriel sur K et f une forme hermitienne positive sur V.

a) Il existe un espace de Hilbert E et une application linéaire $u : V \to E$ tels que $f(x, y) = \langle u(x)|u(y) \rangle$ pour $x, y$ dans V, et que $u(V)$ soit dense dans E.

b) Si deux couples $(E_i, u_i)$ satisfont aux conditions analogues à a), il existe un unique isomorphisme $\varphi$ de l’espace de Hilbert $E_1$ sur l’espace de Hilbert $E_2$ tel que $u_2 = \varphi \circ u_1$.

Soit N l’ensemble des $x \in V$ tels que $f(x, x) = 0$. Sur l’espace $V/N$, on définit une forme hermitienne positive et séparante par $\langle \dot{x}|\dot{y} \rangle = f(x, y)$ pour $x \in \dot{x}$ et $y \in \dot{y}$. Soient E l’espace hilbertien complété de $V/N$ et $u$ l’application $x \mapsto x + N$ de V dans E. Alors les conditions de a) sont remplies.

Sous les hypothèses de b), N est égal au noyau de $u_1$ et à celui de $u_2$. Il existe donc une application linéaire bijective $\varphi_0$ de $u_1(V)$ sur $u_2(V)$ telle que $u_2(x) = \varphi_0(u_1(x))$ pour tout $x \in V$. On vérifie aussitôt que $\varphi_0$ est un isomorphisme d’espaces préhilbertiens, donc une isométrie. Comme $u_i(V)$ est dense dans $E_i$ pour $i = 1, 2$, $\varphi_0$ se prolonge de manière unique en une isométrie $\varphi$ de $E_1$ sur $E_2$, d’où b).

On dit que l’espace hilbertien E est le séparé-complété de V (pour la forme $f$).

#### Exemple 7 {#evt-v-s1-n4-exa-7 .statement}

Soient G un groupe (d’élément unité noté 1) et $\pi$ un homomorphisme de G dans le groupe des automorphismes d’un espace hilbertien complexe E ; on dit encore que $\pi$ est une *représentation unitaire* de $G$ dans $E$. Soit $a \in E$; on pose
$$
\varphi(x) = \langle a | \pi(x) \cdot a \rangle
$$
pour tout $x \in G$. Alors $\varphi : G \to \mathbf{C}$ est de *type positif*, autrement dit satisfait à la relation :

(TP) *Quels que soient* $\lambda_1, \ldots, \lambda_n$ *dans* $\mathbf{C}$ *et* $x_1, \ldots, x_n$ *dans* $G$, *on a*
$$
\sum_{i,j=1}^n \overline{\lambda_i} \lambda_j \varphi(x_i^{-1} x_j) \geqslant 0 .
$$
En effet, le premier membre de (11) n’est autre que $\| \sum_{i=1}^n \lambda_i \pi(x_i) \cdot a \| ^2$.

Réciproquement, soit $\varphi$ une fonction de type positif sur $G$. Soit $C^{(G)}$ l’espace vectoriel des fonctions à support fini sur $G$. On définit une forme hermitienne $\Phi$ sur $C^{(G)}$ par
$$
\Phi(u, v) = \sum_{x,y \in G} \overline{u(x)} \ v(y) \ \varphi(x^{-1} y)
$$
et la relation (TP) exprime que $\Phi$ est positive. D’après le corollaire de la prop. 4, il existe un espace hilbertien $E$ et une application linéaire $\rho : C^{(G)} \to E$, d’image dense, telle que
$$
\Phi(u, v) = \langle \rho(u) | \rho(v) \rangle \quad \text{pour } u, v \text{ dans } C^{(G)} .
$$
Pour tout $x \in G$, soit $\gamma_x$ la translation à gauche par $x$ dans $C^{(G)}$ définie par $\gamma_x u(y) = u(x^{-1} y)$ pour $u \in C^{(G)}$ et $y \in G$. On a $\Phi(\gamma_x u, \gamma_x v) = \Phi(u, v)$. Appliquons alors l’assertion b) du corollaire de la prop. 4 à $\rho$ et $\rho \circ \gamma_x$ : il existe un unique automorphisme $\pi(x)$ de l’espace hilbertien $E$ tel que $\rho \circ \gamma_x = \pi(x) \circ \rho$. On voit aussitôt que $\pi$ est un homomorphisme de $G$ dans le groupe des automorphismes de $E$.
Soit $\delta$ l’élément de $C^{(G)}$ défini par $\delta(1) = 1, \delta(x) = 0$ pour $x \neq 1$ dans $G$. On a $u = \sum_{x \in G} u(x) \cdot \gamma_x \delta$ pour tout $u \in C^{(G)}$, d’où $\rho(u) = \sum_{x \in G} u(x) \pi(x) \cdot a$, en posant $a = \rho(\delta)$.
Les formules (12) et (13) entraînent aussitôt $\varphi(x) = \langle a | \pi(x) \cdot a \rangle$ pour tout $x \in G$. On remarquera que l’ensemble des vecteurs $\pi(x) \cdot a$, pour $x \in G$, est total dans $E$.

### 5. Sous-ensembles convexes d’un espace préhilbertien

Si l’on calcule $\| x - y \| ^2 = \langle x - y | x - y \rangle$ et $\| x + y \| ^2 = \langle x + y | x + y \rangle$ pour deux points quelconques $x, y$ d’un espace préhilbertien $E$, on vérifie aussitôt l’« identité de la médiane »
$$
\| \frac{1}{2}(x + y) \| ^2 + \| \frac{1}{2}(x - y) \| ^2 = \frac{1}{2} (\| x \| ^2 + \| y \| ^2) .
$$
On déduit de cette identité la proposition suivante :

![Diagram showing sets B', B, and A with points x and y](https://i.imgur.com/3Q5z5QG.png)

Fig. 1.

#### Proposition 5 {#evt-v-s1-prop-5 .statement}

Soit E un espace préhilbertien. Soient d un nombre réel > 0, δ un nombre réel tel que 0 ≤ δ < d. Soient B et B' les parties de E définies par \|x\| < d, \|x\| ≤ d + δ respectivement, et soit A un ensemble convexe contenu dans B' − B. Pour tout couple de points x, y de A, on a alors \|x − y\| ≤ \sqrt{12dδ} (fig. 1).

En effet, on a $\frac{1}{2}(x + y) \in A$, donc $\left\| \frac{1}{2}(x + y) \right\| \geq d$; on tire alors de (14) l’inégalité

$$
\left\| \frac{1}{2}(x - y) \right\|^2 = \frac{1}{2}(\|x\|^2 + \|y\|^2) - \left\| \frac{1}{2}(x + y) \right\|^2 \leq (d + \delta)^2 - d^2 \leq 3d\delta
$$

d’où la proposition.

#### Théorème 1 {#evt-v-s1-thm-1 .statement}

Soient E un espace préhilbertien, H une partie convexe non vide de E telle que H soit un sous-espace uniforme séparé et complet de E. Pour tout $x \in E$, il existe un point $p_H(x)$ de H et un seul tel que $\|x - p_H(x)\| = \inf_{y \in H} \|x - y\|$. L’élément $p_H(x)$ de H est aussi l’unique élément a de H satisfaisant à la relation $^1$

(15)
$$
\Re \langle x - a | y - a \rangle \leq 0
$$
pour tout $y \in H$.

![Figure 2](https://i.imgur.com/3Q5z5QG.png)

Fig. 2.

Posons $d = \inf_{y \in H} \|x - y\|$, et pour tout entier $n > 0$, soit $H_n$ l’ensemble des points $y$ de H tels que $\|x - y\| \leq d + n^{-1}$. L’ensemble $H_n$ est fermé dans H, convexe et non vide, et son diamètre est majoré par $\sqrt{12d/n}$ pour tout $n$ assez grand d’après la prop. 5. La suite $(H_n)_{n \geq 1}$ étant décroissante, et l’ensemble H étant supposé séparé et complet, la base de filtre de Cauchy $(H_n)_{n \geq 1}$ converge vers un point $p_H(x)$ de H ; on a $\{ p_H(x) \} = \bigcap_{n \geq 1} H_n$, donc $p_H(x)$ est l’unique point a de H tel que $\|x - a\| = d$.

Soit $y \in H$; comme H est convexe, le point $z(\lambda) = p_H(x) + \lambda(y - p_H(x))$ de E appartient à H pour tout nombre réel $\lambda$ tel que $0 < \lambda < 1$. On a donc $\|x - z(\lambda)\|^2 \geq \|x - p_H(x)\|^2$ pour $0 < \lambda < 1$, d’où

$$
\Re \langle x - p_H(x) | y - p_H(x) \rangle = \lim_{\lambda \to 0} \frac{1}{2\lambda} \left\{ \|x - p_H(x)\|^2 - \|x - z(\lambda)\|^2 \right\} \leq 0 .
$$

$^1$ On rappelle (TG, VIII, p. 2) que $\Re(z)$ désigne la partie réelle du nombre complexe z ; on a $\Re(z) = z$ si z est réel.

Réciproquement, soit $a$ un point de $H$ tel que l’on ait $\mathcal{R} \langle x - a | y - a \rangle \leq 0$ pour tout $y \in H$. Pour tout $y \in H$, on a donc

$$
\|x - y\|^2 = \|x - a\|^2 + \|y - a\|^2 - 2\mathcal{R} \langle x - a | y - a \rangle \geq \|x - a\|^2,
$$

d’où $\|x - a\| = d$ et finalement $a = p_H(x)$ d’après la première partie de la démonstration.

L’application $p_H$ de $E$ dans $H$ sera appelée dans la suite la *projection* de $E$ sur $H$. On remarquera que l’on a $p_H(x) = x$ pour tout $x \in H$.

La première partie du th. 1 est valable sous des hypothèses plus générales sur l’espace $E$ (V, p. 66, exerc. 31).

La démonstration du th. 1 établit entre autres la propriété suivante :

#### Corollaire 1 {#evt-v-s1-thm-1-cor-1 .statement}

*Soient $I$ un ensemble filtré par un filtre $\mathfrak{F}$ et $(y_i)_{i \in I}$ une famille de points de $H$. Soit $x \in E$. On suppose que l’on a*

$$
\lim_{i, \mathfrak{F}} \|x - y_i\| = \inf_{z \in H} \|x - z\|.
$$

*Alors $y_i$ tend vers $p_H(x)$ suivant le filtre $\mathfrak{F}$.*

#### Corollaire 2 {#evt-v-s1-thm-1-cor-2 .statement}

*Quels que soient $x, y$ dans $E$, on a*

$$
\|p_H(x) - p_H(y)\| \leq \|x - y\|.
$$

*En particulier, l’application $p_H$ de $E$ dans $H$ est continue.*

Soient $x, y$ deux points de $E$. Posons $a = p_H(x) - x,\ b = p_H(y) - p_H(x),\ c = y - p_H(y)$. D’après la formule (15) (V, p. 10), on a $\mathcal{R} \langle a | b \rangle \geq 0$ et $\mathcal{R} \langle c | b \rangle \geq 0$. On a $a + b + c = y - x$, d’où

$$
\begin{align*}
\|x - y\|^2 &= \|a + b + c\|^2 = \|b\|^2 + \|a + c\|^2 + 2\mathcal{R} \langle a | b \rangle + 2\mathcal{R} \langle c | b \rangle \\
&\geq \|b\|^2 = \|p_H(x) - p_H(y)\|^2.
\end{align*}
$$

Ceci prouve le cor. 2.

#### Proposition 6 {#evt-v-s1-prop-6 .statement}

*Soit $E$ un espace préhilbertien et soit $\Phi$ un ensemble non vide, filtrant décroissant de parties convexes non vides, séparées et complètes de $E$. Pour tout $x \in E$ et toute partie $H$ de $E$, posons $d(x, H) = \inf_{z \in H} \|x - z\|$. Pour que l’intersection $M$ des ensembles $H$ appartenant à $\Phi$ soit non vide, il faut et il suffit qu’il existe $x_0$ dans $E$ tel que $\sup_{H \in \Phi} d(x_0, H)$ soit fini. Pour tout $x \in E$, on a alors $p_M(x) = \lim_{H \in \Phi} p_H(x)$ (limite suivant l’ensemble filtrant $\Phi$).

Si $M$ est non vide, on a $d(x, H) \leq d(x, M)$ pour tout $H \in \Phi$ et tout $x \in E$.
Réciproquement, supposons qu’il existe un point $x_0$ de $E$ et un nombre réel

C ≥ 0 tels que $d(x_0, H) \leq C$ pour tout $H \in \Phi$. Soit $x \in E$; on a alors
$$
d(x, H) \leq \|x - x_0\| + C \text{ pour tout } H \in \Phi,
$$
donc le nombre $d = \sup_{H \in \Phi} d(x, H)$ est fini. Soit B l’ensemble des $z \in E$ tels que $\|x - z\| \leq d$. Comme B est convexe et fermé dans E, les ensembles $H \cap B$, pour H parcourant $\Phi$, sont convexes, séparés et complets. Soit $\varepsilon > 0$; il existe un ensemble $H \in \Phi$ tel que $d(x, H) \geq d - \varepsilon$, et si $\varepsilon < d/2$, le diamètre de $H \cap B$ est majoré par $\sqrt{12\varepsilon(d - \varepsilon)}$ d’après la prop. 5 (V, p. 10). Autrement dit, pour tout $H_0 \in \Phi$, les ensembles fermés $H \cap B$, pour $H \in \Phi$ et $H \subset H_0$, forment une base de filtre de Cauchy sur l’espace séparé et complet $H_0$. L’intersection des ensembles $H \cap B$ (pour $H \in \Phi$) est donc réduite à un point $y$. On a $y \in M$ et $\|x - y\| = d = d(x, M)$. Comme M est fermé dans $H_0$, c’est un ensemble convexe, séparé et complet dans E et l’on a donc $y = p_M(x)$. Pour tout $H \in \Phi$, on a $p_H(x) \in H \cap B$, d’où $p_M(x) = \lim_{H \in \Phi} p_H(x)$.

#### Proposition 7 {#evt-v-s1-prop-7 .statement}

*Soit E un espace préhilbertien séparé et soit $\Psi$ un ensemble non vide, filtrant croissant de parties convexes, complètes et non vides de E. Posons $A = \bigcup_{H \in \Psi} H$ et supposons que l’adhérence N de A soit complète. Alors N est convexe et l’on a $p_N(x) = \lim_{H \in \Psi} p_H(x)$ pour tout $x \in E$.*

Il est clair que A est convexe, donc son adhérence N est convexe (II, p. 14). Avec les notations de la prop. 6, on a $d(x, N) = \inf_{H \in \Psi} d(x, H)$, et par suite $d(x, N)$ est la limite de $d(x, H)$ suivant le filtre des sections de $\Psi$. Comme on a $p_H(x) \in H$ et $\lim_{H \in \Psi} \|x - p_H(x)\| = \lim_{H \in \Psi} d(x, H) = d(x, N)$, il résulte du cor. 1 de V, p. 11 que $p_H(x)$ tend suivant le filtre des sections de $\Psi$ vers la projection $p_N(x)$ de x sur N.

### 6. Sous-espaces vectoriels et orthoprojecteurs

Soit E un espace préhilbertien. Rappelons que deux vecteurs $x$ et $y$ de E sont dits *orthogonaux* si l’on a $\langle x | y \rangle = 0$; on a alors
$$
\|x + y\|^2 = \|x\|^2 + \|y\|^2
$$
(« th. de Pythagore »).

Soit A une partie de E. On dit qu’un vecteur $x$ de E est *orthogonal* à A s’il est orthogonal à tout vecteur de A. L’ensemble des vecteurs orthogonaux à A est un sous-espace vectoriel fermé de E, noté $A^\circ$ et appelé (par abus de langage) l’*orthogonal* de A.

Soient A et B deux parties de E. On dit que A et B sont *orthogonales* si tout vecteur de A est orthogonal à tout vecteur de B. Il revient au même de dire que l’on a $A \subset B^\circ$, ou encore $B \subset A^\circ$. Si E est séparé et si A et B sont *orthogonales*, alors $A \cap B$ est vide ou réduit à 0 puisque 0 est le seul vecteur de E orthogonal à lui-même.

#### Théorème 2 {#evt-v-s1-thm-2 .statement}

Soient E un espace préhilbertien et M un sous-espace vectoriel de E, qui est séparé et complet. Alors E est somme directe topologique de M et du sous-espace $M^\circ$ orthogonal de M. Le projecteur de E sur M associé à la décomposition $E = M \oplus M^\circ$ est la projection $p_M$ de E sur M définie dans le th. 1 (V, p. 10).

Montrons d’abord que $x - p_M(x)$ appartient à $M^\circ$ pour tout $x \in E$. En effet, soit $y \in M$. Pour tout scalaire $\lambda \in K$, le vecteur $p_M(x) + \lambda y$ appartient à M ; d’après la formule (15) (V, p. 10), on a donc

$$
\mathcal{R}(\lambda \langle x - p_M(x)|y \rangle) \leq 0
$$

pour tout $\lambda \in K$. Si l’on prend en particulier $\lambda = \overline{\langle x - p_M(x)|y \rangle}$, on en conclut $\langle x - p_M(x)|y \rangle = 0$, d’où notre assertion.

Comme M est séparé, 0 est le seul vecteur de M orthogonal à lui-même, d’où $M \cap M^\circ = \{0\}$. Pour tout $x \in E$, on a $p_M(x) \in M$ et $x - p_M(x) \in M^\circ$. Par suite, E est somme directe de M et $M^\circ$, et $p_M$ est le projecteur de E sur M de noyau $M^\circ$. Comme $p_M$ est une application continue de E dans M (V, p. 11, cor. 2), il résulte de TG, III, p. 46 que E est somme directe topologique de M et $M^\circ$.

#### Corollaire {#evt-v-s1-n6-cor-1 .statement}

Soient E un espace préhilbertien séparé et M un sous-espace vectoriel de dimension finie de E. Alors E est somme directe de M et de $M^\circ$.

Puisque E est séparé, il en est de même de M ; comme M est de dimension finie, il est donc complet (I, p. 14). Il suffit donc d’appliquer le th. 2.

Avec les notations du th. 2, on dit que $M^\circ$ est le supplémentaire orthogonal de M et que $p_M$ est l’orthoprojecteur (ou le projecteur orthogonal, ou par abus de langage le projecteur) de E sur M ; si x est un vecteur de E, le vecteur $p_M(x)$ de M s’appelle aussi la projection orthogonale de x sur M. Notons que $p_M$ est une application linéaire continue de E sur M et que l’on a $\|p_M\| = 1$ d’après le cor. 2 de V, p. 11, sauf dans le cas où $M = \{0\}$ où l’on a $p_M = 0$.

Il résulte aussitôt du th. de Pythagore que l’application canonique $\psi$ de E/M sur $M^\circ$ déduite de la décomposition en somme directe $E = M \oplus M^\circ$ est isométrique si l’on munit E/M de la semi-norme quotient de celle de E (II, p. 4). Nous munirons toujours E/M de la structure d’espace préhilbertien pour laquelle $\psi$ est un isomorphisme d’espaces préhilbertiens ; la semi-norme quotient sur E/M est alors déduite de cette structure préhilbertienne.

Nous utiliserons le plus souvent les résultats précédents lorsque E est un espace hilbertien et M un sous-espace vectoriel fermé de E. Dans ce cas, $M^\circ$ est un sous-espace vectoriel fermé de E, et l’on a $p_{M^\circ} = 1 - p_M$ et $(M^\circ)^\circ = M$.

#### Proposition 8 {#evt-v-s1-prop-8 .statement}

Soient E un espace hilbertien, M un sous-espace vectoriel fermé de E, I un ensemble ordonné filtrant non vide et $(M_i)_{i \in I}$ une famille de sous-espaces vectoriels fermés de E. On suppose, ou bien que l’application $i \mapsto M_i$ est croissante et que M est l’adhérence de $\bigcup_{i \in I} M_i$, ou bien que l’application $i \mapsto M_i$ est décroissante et que l’on a $M = \bigcap_{i \in I} M_i$. On a alors $p_M(x) = \lim_{i \in I} p_{M_i}(x)$ pour tout $x \in E$.

La prop. 8 résulte aussitôt des prop. 6 (V, p. 11) et 7 (V, p. 12).

#### Proposition 9 {#evt-v-s1-prop-9 .statement}

Soient E un espace hilbertien et M, N deux sous-espaces vectoriels fermés de E.

a) Les conditions suivantes sont équivalentes :

(i) on a $p_M p_N = p_N p_M$;
(ii) si $x \in M$ est orthogonal à $M \cap N$ et si $y \in N$ est orthogonal à $M \cap N$, alors $x$ et $y$ sont orthogonaux ;
(iii) tout vecteur de $M$ orthogonal à $M \cap N$ est orthogonal à $N$;
(iv) on a $M = (M \cap N) + (M \cap N^\circ)$.

b) Si les conditions équivalentes de a) sont remplies, on a $p_{M \cap N} = p_M p_N$, le sous-espace vectoriel $M + N$ de E est fermé et l’on a $p_{M+N} = p_M + p_N - p_M p_N$.

c) On a $p_M p_N = 0$ si et seulement si $M$ est orthogonal à $N$. S’il en est ainsi, le sous-espace vectoriel $M + N$ de E est fermé et l’on a $p_{M+N} = p_M + p_N$.

Posons $L = M \cap N$, $M_1 = M \cap L^\circ$ et $N_1 = N \cap L^\circ$. La condition (ii) signifie que $M_1$ et $N_1$ sont orthogonaux, et (iii) signifie que $M_1$ et $N$ sont orthogonaux. Comme on a $N = N_1 + L$ et que $M_1$ est orthogonal à $L$, on a prouvé l’équivalence de (ii) et (iii). Si la condition (iii) est satisfaite, on a $M_1 = M \cap N^\circ$ et comme on a $M = L + M_1$, la condition (iv) est remplie. Réciproquement, de (iv) on déduit $M_1 = M \cap N^\circ$ puisque les sous-espaces $M \cap N$ et $M \cap N^\circ$ de $M$ sont orthogonaux, et par suite $M_1 \subset N^\circ$, c’est-à-dire la relation (iii).

Supposons la condition (iv) satisfaite. Il est immédiat que l’on a $p_N(y) = p_L(y)$ pour tout $y \in M$ et par conséquent $p_N p_M(x) = p_L p_M(x)$ pour tout $x \in E$. Mais, pour tout $x \in E$, le vecteur $p_L p_M(x)$ appartient à $L$, et le vecteur
$$
x - p_L p_M(x) = (x - p_M(x)) + (p_M(x) - p_L(p_M(x)))
$$
appartient à $M^\circ + L^\circ = L^\circ$; on a donc $p_L p_M(x) = p_L(x)$. Finalement, on a $p_N p_M = p_L p_M = p_L$. Comme la condition (ii) est équivalente à (iv) et qu’elle est symétrique en $M$ et $N$, on a aussi $p_M p_N = p_L$. On a finalement $p_M p_N = p_N p_M = p_{M \cap N}$, d’où (i).

Réciproquement, supposons la condition (i) satisfaite. Soit $x \in M$; on a
$$
p_M(p_N(x)) = p_N(p_M(x)) = p_N(x)
$$
d’où $p_N(x) \in M$. On en déduit $x - p_N(x) \in M$, donc $x$ est la somme d’un élément $p_N(x)$ de $M \cap N$ et d’un élément $x - p_N(x)$ de $M \cap N^\circ$, d’où (iv).

On a donc prouvé a) et la première partie de b). Supposons que $p_M$ et $p_N$ commutent et posons $q = p_M + p_N - p_M p_N$; comme $p_M$ et $p_N$ sont des idempotents de l’algèbre $\mathcal{L}(E)$, il en est de même de $q$; par suite (TG, III, p. 47), l’image de $q$ est un sous-espace vectoriel fermé de $E$. Il est clair que l’image de $q$ est contenue dans $M + N$; par ailleurs, on a $p_N(x) = x$, d’où $q(x) = x$ pour tout $x \in N$; comme on a aussi $q = p_M + p_N - p_N p_M$, on a de même $q(x) = x$ pour tout $x \in M$. En conclusion, l’image de $q$ est égale à $M + N$. L’orthogonal de $M + N$ est égal à $M^\circ \cap N^\circ$, et le noyau de $q$ contient évidemment $M^\circ \cap N^\circ$, d’où $q = p_{M+N}$. Ceci prouve b).

On a $p_M p_N = 0$ si et seulement si l’image $N$ de $p_N$ est contenue dans le noyau $M^\circ$ de $p_M$, c’est-à-dire si et seulement si $M$ est orthogonal à $N$. Le reste de l’assertion c) est alors un cas particulier de b).

#### Remarque {#evt-v-s1-n6-rem-1 .statement}

Soient E un espace hilbertien et M, N deux sous-espaces vectoriels fermés de E. La relation $M \subset N$ équivaut à l’orthogonalité de M et $N^\circ$, c’est-à-dire à la relation $p_M p_{N^\circ} = 0$ d’après la prop. 9, c). Comme on a $p_{N^\circ} = 1 - p_N$, on conclut que les relations $M \subset N$ et $p_M = p_M p_N$ sont équivalentes (« th. des trois perpendiculaires », cf. fig. 3).

![Diagram showing orthogonal projections and subspaces](fig_3.png)

Fig. 3.

### 7. Dual d’un espace hilbertien

#### Théorème 3 {#evt-v-s1-thm-3 .statement}

Soit E un espace hilbertien. Pour tout $x \in E$, soit $x^*$ la forme linéaire continue $y \mapsto \langle x | y \rangle$ sur E ; l’application $x \mapsto x^*$ est une application semi-linéaire (pour l’automorphisme $\xi \mapsto \overline{\xi}$) bijective de E sur son dual $E'$, et une isométrie de l’espace normé E sur l’espace normé $E'$.

En effet, l’application $x \mapsto x^*$ est semi-linéaire d’après (2) (V, p. 1), et, en vertu de l’inégalité de Cauchy-Schwarz, on a $\|x^*\| = \sup_{\|y\| \leq 1} |\langle x | y \rangle| = \|x\|$, donc $x \mapsto x^*$ est une isométrie de E dans $E'$, et en particulier est injective. Pour achever la démonstration, il faut prouver que pour tout $x' \neq 0$ dans $E'$, il existe $x \in E$ tel que $x' = x^*$. Or l’hyperplan $H = \mathrm{Ker}\, x'$ est fermé dans E ; son orthogonal est une droite D. Soit $b$ un élément non nul de D ; le noyau de la forme linéaire $b^*$ est égal à H et il existe donc un scalaire $\lambda \neq 0$ tel que $x' = \lambda \cdot b^* = (\overline{\lambda} \cdot b)^*$.

C.Q.F.D.

L’application $x \mapsto x^*$ de E sur son dual $E'$ est dite canonique. L’application réciproque de $E'$ sur E est aussi dite canonique et se note $x' \mapsto {x'}^*$. On a donc

$$
\langle x | y \rangle = \langle y, x^* \rangle, \quad \langle x, x' \rangle = \langle {x'}^* | x \rangle
$$

pour $x, y$ dans E et $x'$ dans $E'$. On a aussi $(x^*)^* = x$ pour $x \in E$.

Lorsque $K = \mathbf{R}$, l’application $x \mapsto x^*$ est linéaire. On transportera à $E'$ le produit scalaire de E par cette application. Lorsque $K = \mathbf{C}$, on peut considérer l’application $x \mapsto x^*$ comme un isomorphisme de l’espace vectoriel $\overline{E}$ conjugué de E sur $E'$ (V, p. 6). On transportera à $E'$ le produit scalaire de $\overline{E}$ par cette application.

Dans les deux cas considérés, E' est un espace hilbertien, et l’on a les formules

$$
\langle x^*|y^*\rangle = \overline{\langle x|y\rangle}, \quad \langle x'|x'\rangle = \|x'\|^2
$$

pour $x, y$ dans $E$ et $x'$ dans $E'$.

Il revient au même de dire que le vecteur $x \in E$ est orthogonal à un vecteur $y \in E$, ou de dire que la forme linéaire $x^* \in E'$ est orthogonale à $y$ au sens défini en II, p. 44 (ce qui justifie l’emploi du mot « orthogonal » dans les deux cas). Si M est un sous-espace vectoriel fermé de E, le sous-espace $M^\circ$ orthogonal à M dans $E'$ (II, p. 48) est l’image par $x \mapsto x^*$ de l’orthogonal de M dans E, défini en V, p. 12 (ce qui justifie l’emploi de la notation $M^\circ$ dans les deux cas).

#### Corollaire 1 {#evt-v-s1-thm-3-cor-1 .statement}

*Pour qu’une famille $(x_i)_{i \in I}$ de points d’un espace hilbertien E soit totale, il faut et il suffit que pour $y \in E$, les relations $\langle x_i|y\rangle = 0$ pour tout indice $i \in I$ entraînent $y = 0$.*

En effet, cela exprime que 0 est le seul vecteur de $E'$ orthogonal aux $x_i$ (II, p. 46 et IV, p. 1).

#### Corollaire 2 {#evt-v-s1-thm-3-cor-2 .statement}

*Soient E et F deux espaces hilbertiens. Pour $u \in \mathcal{L}(E; F)$, $x \in E$ et $y \in F$, posons*

$$(18)$$
$$
\Phi_u(y, x) = \langle y|u(x)\rangle .
$$

*L’application $u \mapsto \Phi_u$ est un isomorphisme de l’espace de Banach $\mathcal{L}(E; F)$ sur l’espace des formes sesquilinéaires $^1$ continues sur $F \times E$, muni de la norme*

$$(19)$$
$$
\|f\| = \sup_{\substack{x \in E, y \in F \\ \|x\| \leq 1, \|y\| \leq 1}} |f(y, x)| .
$$

Il est clair que $\Phi_u$ est sesquilinéaire et continue pour tout $u \in \mathcal{L}(E; F)$. Inversement, soit $f$ une forme sesquilinéaire continue sur $F \times E$. Pour tout $x \in E$, l’application $y \mapsto f(y, x)$ est une forme linéaire continue sur l’espace hilbertien F. D’après le th. 3, il existe donc pour tout $x \in E$, un unique élément $u(x)$ de F tel que l’on ait $f(y, x) = \langle u(x)|y\rangle$ pour tout $y \in F$. L’application $u : x \mapsto u(x)$ de E dans F est linéaire et l’on a

$$
\begin{align*}
\|f\| &= \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |f(y, x)| = \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |\langle y|u(x)\rangle| \\
&= \sup_{\|x\| \leq 1} \|u(x)\| ;
\end{align*}
$$

donc $u$ appartient à $\mathcal{L}(E; F)$, on a $f = \Phi_u$ et $\|u\| = \|f\|$. D’où le cor. 2.

L’application canonique de E dans son bidual $E''$ (IV, p. 14) applique E *sur* $E''$, autrement dit (IV, p. 16), E est un espace de Banach *réflexif*. En effet, si E est un espace hilbertien réel (resp. complexe), l’application canonique $\varphi$ de $E'$ sur E est un

$^1$ Rappelons (A, IX, § 1, n° 5) qu’une forme sesquilinéaire (à gauche) $f$ sur $F \times E$ est une application de $F \times E$ dans $K$ qui satisfait aux relations (1) et (2) de V, p. 1.

isomorphisme de l’espace normé E′ sur E (resp. sur l’espace $\overline{E}$ conjugué de E); appliquant le th. 3 à E (resp. $\overline{E}$), on voit que toute forme linéaire continue sur l’espace normé E′ est de la forme $x' \mapsto \langle \varphi(x')|x \rangle = \langle x, x' \rangle$ avec $x \in E$, d’où notre assertion.

Par suite (IV, p. 17, prop. 6) :

#### Théorème 4 {#evt-v-s1-thm-4 .statement}

*Dans un espace hilbertien E, la boule unité est faiblement compacte.*

#### Proposition 10 {#evt-v-s1-prop-10 .statement}

*Si, dans un espace hilbertien E, un filtre $\mathcal{F}$ converge faiblement vers $x_0$, et si en outre $\lim_{\mathcal{F}} \|x\| = \|x_0\|$, alors $\mathcal{F}$ converge vers $x_0$ pour la topologie initiale de E.*

En effet, $\|x - x_0\|^2 = \|x\|^2 - 2\Re \langle x|x_0 \rangle + \|x_0\|^2$. Comme $\langle x|x_0 \rangle$ tend par hypothèse vers $\|x_0\|^2$ suivant $\mathcal{F}$, et que $\|x\|$ tend vers $\|x_0\|$ suivant $\mathcal{F}$, $\|x - x_0\|$ tend vers 0 suivant $\mathcal{F}$, d’où la proposition.

#### Remarque {#evt-v-s1-n7-rem-1 .statement}

Si E est un espace préhilbertien séparé et $\hat{E}$ l’espace hilbertien complété de E, on sait (III, p. 16) que le dual E′ de E s’identifie au dual de $\hat{E}$; il résulte du th. 3 (V, p. 15) que toute forme linéaire continue sur E s’écrit d’une seule manière $x \mapsto \langle a|x \rangle$, où $a \in \hat{E}$.

## EXERCICES {#evt-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
