---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 1
section_title: Semi-normes
lang: fr
source: evt-i-v-fr
pdf_pages: 0036-0042
extraction: ocr
subsections:
    - "no": 1
      title: Définition des semi-normes
      page: 0
      pdf_page: 36
    - "no": 2
      title: Topologies définies par des semi-normes
      page: 2
      pdf_page: 37
    - "no": 3
      title: Semi-normes dans les espaces quotients et les espaces produits
      page: 4
      pdf_page: 39
    - "no": 4
      title: Critères d’équicontinuité des applications multilinéaires pour les topologies définies par des semi-normes
      page: 6
      pdf_page: 41
statements: 18
exercises: 0
content_sha256: 1e2e0b5ae408b6adcab0d34e5f7da77d3e2ec59bbbb561a0eb07f1841fc382f4
---

## § 1. SEMI-NORMES

Dans tout ce paragraphe, $\mathbf{K}$ désigne un corps valué non discret.

### 1. Définition des semi-normes

#### Définition 1 {#evt-ii-s1-def-1 .statement}

Soit $E$ un espace vectoriel à gauche sur $\mathbf{K}$. On appelle semi-norme sur $E$ une application $p$ de $E$ dans $\mathbf{R}_+ = [0, +\infty[$, vérifiant les axiomes suivants :
(SN₁) Quels que soient $x \in E$ et $\lambda \in \mathbf{K}$, on a $p(\lambda x) = |\lambda| p(x)$.
(SN₂) Quels que soient $x, y$ dans $E$, on a $p(x + y) \leq p(x) + p(y)$.

On a l’inégalité :

$$
|p(x) - p(y)| \leq p(x - y)
$$

qui se déduit aussitôt des relations $p(x) \leq p(y) + p(x - y)$ et $p(y) \leq p(x) + p(y - x)$, puisque $p(y - x) = p(x - y)$.

#### Exemple 1 {#evt-ii-s1-n1-exa-1 .statement}

Une norme sur $E$ est une semi-norme $p$ telle que la relation $p(x) = 0$ entraîne $x = 0$ (I, p. 3).

#### Exemple 2 {#evt-ii-s1-n1-exa-2 .statement}

Pour toute forme linéaire $f$ sur $E$, la fonction $x \mapsto |f(x)|$ est une semi-norme sur $E$.

#### Exemple 3 {#evt-ii-s1-n1-exa-3 .statement}

Soient $p_i$ ($1 \leq i \leq n$) des semi-normes en nombre fini sur $E$; il est immédiat que $p'(x) = \sup_{1 \leq i \leq n} p_i(x)$ et $p''(x) = \sum_{i=1}^n \alpha_i p_i(x)$ (où les $\alpha_i$ sont $\geq 0$) sont encore des semi-normes sur $E$.

On appelle *ultra-semi-norme* sur E une application $p$ de E dans $\mathbf{R}_+$ qui vérifie (SN$_l$) et l’axiome suivant :

(SN$_{ll}'$) *Quels que soient* $x, y$ *dans* E, *on a* $p(x + y) \leq \sup(p(x), p(y))$.

Il est clair qu’une ultra-semi-norme est une semi-norme.

Dire que la valeur absolue sur K est *ultramétrique* (AC, VI, § 6, n° 2) signifie que c’est une ultra-semi-norme sur l’espace vectoriel à gauche $K_s$ qui n’est pas identiquement nulle.

#### Proposition 1 {#evt-ii-s1-prop-1 .statement}

*Soient* E *un espace vectoriel topologique à gauche sur* K, *p une semi-norme sur* E. *Les conditions suivantes sont équivalentes* :

a) *p est continue dans* E.
b) *p est continue au point* 0.
c) *p est uniformément continue*.
d) *Pour tout nombre réel* $\alpha > 0$, *l’ensemble* W$(p, \alpha)$ *des* $x \in E$ *tels que* $p(x) < \alpha$ *est ouvert dans* E.
e) *Il existe un nombre réel* $\alpha > 0$, *tel que* W$(p, \alpha)$ *soit un voisinage de* 0 *dans* E.
f) *Pour tout nombre réel* $\alpha > 0$, *l’ensemble* V$(p, \alpha)$ *des* $x \in E$ *tels que* $p(x) \leq \alpha$ *est un voisinage de* 0 *dans* E.

En effet, les implications $c) \Rightarrow a) \Rightarrow b) \Rightarrow d) \Rightarrow e) \Rightarrow f) \Rightarrow c)$ sont immédiates, en vertu de l’inégalité (1) et de (SN$_l$).

#### Corollaire {#evt-ii-s1-n1-cor-1 .statement}

*Si* p *est une semi-norme continue dans* E *et q une semi-norme sur* E *telle que* $q \leq p$, *alors* q *est continue dans* E.

Lorsque $p$ est une *ultra-semi-norme* sur E, les ensembles W$(p, \alpha)$ et V$(p, \alpha)$ sont *à la fois ouverts et fermés*. En effet, on a vu que W$(p, \alpha)$ est ouvert ; si d’autre part z est adhérent à W$(p, \alpha)$, il y a un $y \in W(p, \alpha)$ tel que $p(y - z) < \alpha$, et on tire de (SN$_{ll}'$) que $p(z) < \alpha$, donc W$(p, \alpha)$ est fermé. D’autre part, V$(p, \alpha)$ est fermé puisque $p$ est continue ; en outre, si $p(x) \leq \alpha$ et $p(y) \leq \alpha$, on a $p(x + y) \leq \alpha$ en vertu de (SN$_{ll}'$), ce qui montre que V$(p, \alpha)$ est ouvert.

### 2. Topologies définies par des semi-normes

Soient E un espace vectoriel sur K, $p$ une semi-norme sur E ; pour tout $\alpha > 0$, soit V$(p, \alpha)$ l’ensemble des $x \in E$ tels que $p(x) \leq \alpha$. Il est clair que si $x \in V(p, \alpha)$ et si $\lambda \in K$ est tel que $|\lambda| \leq 1$, on a $\lambda x \in V(p, \alpha)$, autrement dit V$(p, \alpha)$ est *équilibré*. En outre, pour tout $x_0 \in E$, il existe un scalaire $\mu \in K$ non nul tel que $|\mu| \geq p(x_0) \alpha^{-1}$, donc $\mu^{-1} x_0 \in V(p, \alpha)$; autrement dit V$(p, \alpha)$ est *absorbant*. Enfin, il résulte de (SN$_{ll}$) que l’on a $V(p, \alpha/2) + V(p, \alpha/2) \subset V(p, \alpha)$, et de (SN$_l$) que pour tout scalaire $\lambda \neq 0$ dans K, on a $\lambda V(p, \alpha) = V(p, |\lambda| \alpha)$. On conclut de ces remarques, en vertu de I, p. 47, prop. 4, que lorsque $\alpha$ parcourt l’ensemble des nombres $> 0$ (ou seulement une suite de nombres $> 0$, tendant vers 0), les ensembles V$(p, \alpha)$ constituent un système fondamental de voisinages de 0 pour une topologie compatible avec la structure d’espace vectoriel de E ; on dit que cette topologie est *définie par la semi-norme* $p$. Un espace vectoriel E muni d’une telle topologie est appelé *espace semi-* normé. On notera que si $W(p, \alpha)$ est l’ensemble des $x \in E$ tels que $p(x) < \alpha$, les $W(p, \alpha)$ constituent (pour $\alpha > 0$, ou $\alpha$ parcourant seulement une suite de nombres $> 0$ tendant vers 0) un système fondamental de voisinages de 0 pour la topologie définie par $p$.

Si maintenant $\Gamma$ est un ensemble de semi-normes sur $E$, la *borne supérieure* des topologies définies par les semi-normes $p \in \Gamma$ est encore compatible avec la structure d’espace vectoriel (I, p. 11, cor. 4). On a un système fondamental de voisinages de 0 pour cette topologie en considérant les intersections finies $\bigcap_i V(p_i, \alpha_i)$ avec $p_i \in \Gamma$ et $\alpha_i > 0$. On dit que cette topologie est *définie par l’ensemble $\Gamma$ de semi-normes*. C’est la topologie *la moins fine* sur $E$ parmi celles qui sont invariantes par toute translation et qui rendent continues les semi-normes $p \in \Gamma$.

Soit $E$ un espace vectoriel topologique sur $K$; on dit qu’un ensemble $\Gamma$ de semi-normes sur $E$ est un *système fondamental de semi-normes* si la topologie de $E$ est égale à la topologie définie par $\Gamma$.

Soit $E$ un espace vectoriel sur $K$, muni de la topologie définie par un ensemble de semi-normes $\Gamma$. Pour toute semi-norme $p$, on a $p(x - z) \leq p(x - y) + p(y - z)$, ce qui montre que la fonction $(x, y) \mapsto p(x - y)$ est un *écart* sur $E$ (TG, IX, p. 1); il résulte des définitions que l’ensemble de ces écarts, lorsque $p$ parcourt $\Gamma$, définit la structure uniforme de l’espace vectoriel topologique $E$.

#### Remarque 1 {#evt-ii-s1-n2-rem-1 .statement}

La topologie définie par un ensemble *fini* de semi-normes $p_i$ sur $E$ ($1 \leq i \leq n$) peut être définie par la *seule* semi-norme $p = \sup_{1 \leq i \leq n} p_i$. Par contre une topologie définie par un ensemble infini de semi-normes ne peut en général être définie par une seule semi-norme (III, p. 38, exerc. 2).

#### Remarque 2 {#evt-ii-s1-n2-rem-2 .statement}

Soit $(\mathcal{T}_\nu)_{\nu \in I}$ une famille de topologies sur un espace vectoriel $E$ sur $K$, dont chacune est définie par un ensemble $\Gamma_\nu$ de semi-normes. Alors la topologie définie par l’ensemble de semi-normes $\Gamma = \bigcup_{\nu \in I} \Gamma_\nu$ est la borne supérieure des topologies $\mathcal{T}_\nu$.

#### Remarque 3 {#evt-ii-s1-n2-rem-3 .statement}

La relation « il existe $\lambda > 0$ tel que $p \leq \lambda q$ » entre deux semi-normes $p, q$ sur $E$ est une relation de préordre. Si $\Gamma_0$ est un ensemble de semi-normes *filtrant croissant* pour cette relation de préordre, on obtient un système fondamental de voisinages de 0 pour la topologie définie par $\Gamma_0$ en prenant l’ensemble des $V(p, \alpha)$, où $p \in \Gamma_0$ et $\alpha > 0$. Si $\Gamma$ est un ensemble quelconque de semi-normes sur $E$, on obtient un ensemble filtrant de semi-normes définissant la même topologie que $\Gamma$ en prenant l’ensemble $\Gamma_0$ des enveloppes supérieures de toutes les familles finies de semi-normes appartenant à $\Gamma$.

#### Remarque 4 {#evt-ii-s1-n2-rem-4 .statement}

Même si $K = \mathbf{R}$, la topologie d’un espace vectoriel topologique sur $K$ ne peut pas toujours être définie par un ensemble de semi-normes (*cf.* II, p. 26).

#### Exemple {#evt-ii-s1-n2-exa-1 .statement}

Soit $\mathscr{C}^\infty(\mathbf{R})$ l’espace vectoriel sur $\mathbf{R}$ des fonctions numériques indéfiniment dérivables dans $\mathbf{R}$. Pour toute fonction $f \in \mathscr{C}^\infty(\mathbf{R})$ et tout couple d’entiers $n \geq 0$, $m \geq 1$, posons :

$$
p_{n,m}(f) = \sup_{-m \leq t \leq m} |f^{(n)}(t)|
$$

avec $f^{(0)} = f$. Il est immédiat que les $p_{n,m}$ sont des semi-normes sur $\mathscr{C}^\infty(\mathbf{R})$. Pour que des fonctions $f_\alpha$ convergent vers 0 (suivant un filtre $\mathfrak{F}$ sur l’ensemble des indices) dans $\mathscr{C}^\infty(\mathbf{R})$ pour la topologie $\mathcal{T}$ définie par les semi-normes $p_{n,m}$, il faut et il suffit que, pour tout entier $n \geq 0$, les fonctions $f_\alpha^{(n)}$ tendent vers 0 (suivant $\mathfrak{F}$) *uniformément dans toute partie compacte de* $\mathbf{R}$. On dit que $\mathcal{T}$ est la *topologie de la convergence compacte pour les fonctions* $f \in \mathscr{C}^\infty(\mathbf{R})$ *et toutes leurs dérivées* (*cf.* III, p. 9).

#### Proposition 2 {#evt-ii-s1-prop-2 .statement}

Soient $\Gamma$ un ensemble de semi-normes sur un espace vectoriel $E$, $\mathcal{T}$ la topologie sur $E$ définie par $\Gamma$.

(i) L’adhérence de $\{0\}$ dans $E$ pour $\mathcal{T}$ est l’ensemble des $x \in E$ tels que $p(x) = 0$ pour toute semi-norme $p \in \Gamma$.

(ii) Si $\mathcal{T}$ est séparée et si $\Gamma$ est dénombrable, $\mathcal{T}$ est métrisable.

La proposition résulte aussitôt des définitions et de TG, IX, p. 15, cor. 1.

On notera que si $\mathcal{T}$ est métrisable, $\mathcal{T}$ ne peut pas toujours être définie par une seule norme ; c’est le cas de l’exemple donné ci-dessus (*cf.* IV, p. 18, *Exemple 4*).

Soit $E$ un espace vectoriel sur $K$, muni de la topologie définie par un ensemble de semi-normes $\Gamma$. Soit $\hat{E}$ le séparé complété de $E$ (I, p. 6), et soit $\hat{\Gamma}$ l’ensemble des applications $\hat{p}$ de $\hat{E}$ dans $\mathbf{R}_+$, où $p$ parcourt $\Gamma$ (TG, II, p. 24, prop. 15). En vertu du principe de prolongement des inégalités, les fonctions $\hat{p} \in \hat{\Gamma}$ sont des semi-normes sur $\hat{E}$, et les fonctions $\hat{p}(x - y)$ forment un ensemble d’écarts définissant la structure uniforme de $\hat{E}$ (TG, IX, p. 5, prop. 1). On voit donc que $\hat{\Gamma}$ est un ensemble fondamental de semi-normes définissant la topologie de $\hat{E}$.

### 3. Semi-normes dans les espaces quotients et les espaces produits

Soit $E$ un espace vectoriel topologique sur $K$, dont la topologie est définié par un ensemble $\Gamma$ de semi-normes. Il est clair que les restrictions des semi-normes de $\Gamma$ à un sous-espace vectoriel $M$ de $E$ définissent la topologie induite sur $M$ par celle de $E$.

Soit $\varphi$ l’application canonique de $E$ sur l’espace vectoriel quotient $E/M$. Montrons que, pour toute semi-norme $p$ sur $E$, la fonction

$$
\dot{p}(z) = \inf_{\varphi(x) = z} p(x)
$$

est une *semi-norme* sur $E/M$. En effet, il est clair que $\dot{p}$ vérifie la condition (SN$_I$) ; d’autre part, si $z', z''$ sont deux vecteurs de $E/M$, on a :

$$
\begin{align*}
\inf_{\varphi(x) = z' + z''} p(x) &\leq \inf_{\varphi(x') = z', \varphi(x'') = z''} p(x' + x'') \\
&\leq \inf_{\varphi(x') = z', \varphi(x'') = z''} (p(x') + p(x'')) \\
&= \inf_{\varphi(x') = z'} p(x') + \inf_{\varphi(x'') = z''} p(x'')
\end{align*}
$$

ce qui montre que $\dot{p}$ vérifie (SN$_{II}$). On dit que $\dot{p}$ est la *semi-norme quotient* de $p$ par $M$.

On notera que le même raisonnement prouve que si $p$ est une *ultra-semi-norme*, il en est de même de $\dot{p}$.

Cela étant, on a, pour tout $\alpha > 0$ (avec les notations du no 2) :

$$
\varphi(\mathrm{W}(p, \alpha)) = \mathrm{W}(\dot{p}, \alpha) .
$$

En effet, dire que $\dot{p}(z) < \alpha$ signifie qu’il existe $x \in E$ tel que $\varphi(x) = z$ et $p(x) < \alpha$, d’où la relation (4).

On conclut de là que si l’ensemble $\Gamma$ de semi-normes est filtrant (II, p. 3, Remarque 3), alors la topologie quotient sur $E/M$ est définie par l’ensemble des semi-normes $\dot{p}$, lorsque $p$ parcourt $\Gamma$.

Si $N$ est l’adhérence de 0 dans $E$, la topologie de $E/N$ est définie par les semi-normes quotients $\dot{p}$ où $p$ parcourt $\Gamma$ (même si $\Gamma$ n’est pas filtrant); on a ici $\dot{p}(\dot{x}) = p(x)$ pour tout $x$ appartenant à une classe $\dot{x}$ mod. $N$. On notera que $E/N$ n’est autre que l’espace séparé associé à $E$ (I, p. 4).

Soient $E$ un espace vectoriel sur $K$, $(E_i)_{i \in I}$ une famille d’espaces vectoriels sur $K$, $E_i$ étant muni d’une topologie $\mathcal{T}_i$ définie par un ensemble de semi-normes $\Gamma_i$. Pour chaque $i \in I$, soit $f_i$ une application linéaire de $E$ dans $E_i$; il est clair que lorsque $p_i$ parcourt l’ensemble $\Gamma_i$, les $p_i \circ f_i$ forment un ensemble $\Gamma'_i$ de semi-normes sur $E$. La topologie $\mathcal{T}$ sur $E$, définie comme étant la moins fine de celles rendant continues toutes les applications $f_i$ (I, p. 9) est alors définie par l’ensemble de semi-normes $\Gamma' = \bigcup_{i \in I} \Gamma'_i$, comme il résulte de la définition des voisinages de 0 pour $\mathcal{T}$ (TG, I, p. 12, prop. 4).

Si les $p_i$ sont des ultra-semi-normes, il en est de même des $p_i \circ f_i$.

Soit $E$ un espace vectoriel sur $K$, muni d’une topologie $\mathcal{T}$ définie par une famille de semi-normes $(p_i)_{i \in I}$; pour tout $i \in I$, soit $\mathcal{T}_i$ la topologie définie par la seule semi-norme $p_i$, et notons $E_i$ l’espace obtenu en munissant $E$ de $p_i$. Alors la topologie $\mathcal{T}$ est l’image réciproque par l’application diagonale $\Delta : E \to \prod_{i \in I} E_i$ de la topologie produit sur $\prod_{i \in I} E_i$ (I, p. 9, prop. 7). Pour tout $i \in I$, désignons par $N_i$ l’adhérence de 0 dans $E_i$, par $F_i = E_i / N_i$ l’espace normé défini par la norme $\dot{p}_i$ correspondant à $p_i$ (II, p. 4, formule (3)); si $\varphi_i : E_i \to F_i$ est l’application canonique, et $\varphi : (x_i) \mapsto (\varphi_i(x_i))$ l’application produit, on sait que la topologie produit sur $\prod_{i \in I} E_i$ est l’image réciproque par $\varphi$ de la topologie produit sur $\prod_{i \in I} F_i$ (TG, II, p. 26, prop. 18); la topologie $\mathcal{T}$ est donc l’image réciproque par l’application composée $\varphi \circ \Delta$ de la topologie produit sur $\prod_{i \in I} F_i$. Si en particulier $\mathcal{T}$ est séparée, il résulte de II, p. 4, prop. 2 que l’application $\varphi \circ \Delta$ est injective, donc :

#### Proposition 3 {#evt-ii-s1-prop-3 .statement}

Tout espace vectoriel topologique séparé $E$ sur $K$, dont la topologie est définie par un ensemble de semi-normes, est isomorphe à un sous-espace d’un produit d’espaces de Banach.

Si de plus la topologie de $E$ est définie par une famille dénombrable de semi-normes, $E$ est métrisable (I, p. 16).

### 4. Critères d’équicontinuité des applications multilinéaires pour les topologies définies par des semi-normes

#### Proposition 4 {#evt-ii-s1-prop-4 .statement}

Soient $E_i$ ($1 \leq i \leq n$) et $F$ des espaces vectoriels topologiques sur $K$; on suppose que pour tout $i$, la topologie de $E_i$ est définie par un ensemble filtrant de semi-normes $\Gamma_i$ et que la topologie de $F$ est définie par un ensemble de semi-normes $\Gamma$.

Pour qu’un ensemble $H$ d’applications multilinéaires de $\prod_{i=1}^n E_i$ dans $F$ soit équicontinu, il faut et il suffit que, pour toute semi-norme $q \in \Gamma$, il existe pour chaque indice $i$ une semi-norme $p_i \in \Gamma_i$, ainsi qu’un nombre $a > 0$, tels que l’on ait, pour toute fonction $u \in H$ et tout point $(x_i) \in \prod_{i=1}^n E_i$,

$$
q(u(x_1, x_2, \ldots, x_n)) \leq a \cdot p_1(x_1) \, p_2(x_2) \cdots p_n(x_n) .
$$

La condition est suffisante, car si elle est vérifiée, $H$ est équicontinu au point $(0, 0, \ldots, 0)$, donc partout (I, p. 9, prop. 6).

Montrons que la condition est nécessaire. Par hypothèse, pour toute semi-norme $q \in \Gamma$ et tout nombre $\beta > 0$, il existe $n$ nombres $\alpha_i > 0$ ($1 \leq i \leq n$) et, pour chaque indice $i$, une semi-norme $p_i \in \Gamma_i$, tels que les relations $p_i(x_i) \leq \alpha_i$ pour $1 \leq i \leq n$ entraînent $q(u(x_1, x_2, \ldots, x_n)) \leq \beta$ pour toute fonction $u \in H$. Comme $K$ est non discret, on peut même supposer que l’on a, pour tout $i$, $\alpha_i = |\lambda_i| < 1$ où $\lambda_i \in K$.

Soit alors $(x_1, \ldots, x_n)$ un point quelconque de $\prod_{i=1}^n E_i$, et pour chaque indice $i$, soit $m_i \in \mathbf{Z}$ un entier tel que $p_i(x_i) \leq |\lambda_i|^{m_i + 1}$; cela s’écrit aussi $p_i(\lambda_i^{-m_i} x_i) \leq |\lambda_i|$ ($1 \leq i \leq n$), donc on a par hypothèse :

$$
q(u(x_1, x_2, \ldots, x_n)) \leq \beta |\lambda_1|^{m_1} |\lambda_2|^{m_2} \cdots |\lambda_n|^{m_n} .
$$

Supposons d’abord que l’un des $p_i(x_i)$ soit nul. Alors, on peut prendre $m_i \in \mathbf{N}$ arbitrairement grand, donc

$$
q(u(x_1, x_2, \ldots, x_n)) = 0 .
$$

Si au contraire tous les $p_i(x_i)$ sont $\neq 0$, prenons pour chaque $i$ l’entier $m_i$ tel que $|\lambda_i|^{m_i + 2} < p_i(x_i) \leq |\lambda_i|^{m_i + 1}$; alors on a

$$
|\lambda_i|^{m_i} < |\lambda_i|^{-2} p_i(x_i) ,
$$

d’où en vertu de (6), la relation (5) avec $a = \beta (|\lambda_1| \cdot |\lambda_2| \cdots |\lambda_n|)^{-2}$.

C.Q.F.D.

#### Corollaire {#evt-ii-s1-n4-cor-1 .statement}

Pour que $H$ soit équicontinu, il faut et il suffit que, pour toute semi-norme $q \in \Gamma$, il existe un voisinage de 0 dans $\prod_{i=1}^n E_i$ dans lequel les fonctions $q \circ u$, pour $u \in H$, soient uniformément bornées.

La condition est évidemment nécessaire, et la démonstration de la prop. 4 montre qu’elle entraîne une inégalité de la forme (5) pour tout $u \in \mathrm{H}$, donc l’équicontinuité de $\mathrm{H}$.

Nous expliciterons le cas particulier de la prop. 4 relatif aux applications linéaires :

#### Proposition 5 {#evt-ii-s1-prop-5 .statement}

Soient $E, F$ deux espaces vectoriels topologiques sur un corps valué non discret $K$; on suppose que la topologie de $E$ (resp. $F$) est définie par un ensemble $\Gamma$ (resp. $\Gamma'$) de semi-normes. Soit $\mathrm{H}$ un ensemble d’applications linéaires de $E$ dans $F$. Les conditions suivantes sont équivalentes :
a) $\mathrm{H}$ est équicontinu.
b) Pour toute semi-norme $q \in \Gamma'$, il existe une famille finie $(p_i)_{1 \leq i \leq n}$ de semi-normes appartenant à $\Gamma$ et un nombre $a > 0$ tels que l’on ait, pour tout $x \in E$ et toute $u \in \mathrm{H}$,
$$
q(u(x)) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) .
$$
c) Pour toute semi-norme $q \in \Gamma'$, $\sup_{u \in \mathrm{H}} (q \circ u)$ est une semi-norme continue sur $E$.

#### Corollaire 1 {#evt-ii-s1-prop-5-cor-1 .statement}

Soient $E$ un espace vectoriel sur $K$, $\mathcal{T}, \mathcal{T}'$ deux topologies sur $E$ définies respectivement par deux ensembles $\Gamma, \Gamma'$ de semi-normes. Pour que $\mathcal{T}$ soit plus fine que $\mathcal{T}'$, il faut et il suffit que, pour toute semi-norme $q \in \Gamma'$, il existe une famille finie $(p_i)_{1 \leq i \leq n}$ de semi-normes appartenant à $\Gamma$ et un nombre $a > 0$ tels que l’on ait $q(x) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x)$ pour tout $x \in E$.
En effet, cela exprime que l’application identique de $E$ muni de $\mathcal{T}$, sur $E$ muni de $\mathcal{T}'$, est continue.

#### Corollaire 2 {#evt-ii-s1-prop-5-cor-2 .statement}

Soit $E$ un espace vectoriel topologique sur $K$, dont la topologie $\mathcal{T}$ est définie par un ensemble filtrant $\Gamma$ de semi-normes; pour toute semi-norme $p \in \Gamma$, soit $E_p$ l’espace obtenu en munissant $E$ de $p$. L’ensemble $E'$ des formes linéaires sur $E$ continues pour $\mathcal{T}$ est réunion des ensembles $E'_p$, où $E'_p$ est l’ensemble des formes linéaires continues dans $E_p$ ($p \in \Gamma$).
