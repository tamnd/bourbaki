---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 4
section_title: Fonctions et ensembles intégrables
lang: fr
source: int-i-iv-fr
pdf_pages: 0144-0173, 0240-0249
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement de l’intégrale
      page: 0
      pdf_page: 144
    - "no": 2
      title: Propriétés de l’intégrale
      page: 0
      pdf_page: 145
    - "no": 3
      title: Passages à la limite dans les intégrales
      page: 0
      pdf_page: 147
    - "no": 4
      title: Caractérisations des fonctions numériques intégrables
      page: 0
      pdf_page: 149
    - "no": 5
      title: Ensembles intégrables
      page: 0
      pdf_page: 153
    - "no": 6
      title: Critères d’intégrabilité d’un ensemble
      page: 0
      pdf_page: 155
    - "no": 7
      title: Caractérisation des mesures bornées
      page: 0
      pdf_page: 158
    - "no": 8
      title: Intégration par rapport à une mesure à support compact
      page: 0
      pdf_page: 160
    - "no": 9
      title: Clans et fonctions additives d’ensemble
      page: 0
      pdf_page: 163
    - "no": 10
      title: Approximation des fonctions continues par les fonctions étagées
      page: 0
      pdf_page: 166
    - "no": 11
      title: Prolongement d’une mesure définie sur une famille d’ensembles
      page: 0
      pdf_page: 167
statements: 62
exercises: 5
content_sha256: 3fcd4a66927194632d9fb1ddf6dc957e482b924a4f4a3e17d94933d48c0000ac
---

## § 4. Fonctions et ensembles intégrables

### 1. Prolongement de l’intégrale

Il résulte de la définition de l’espace $\mathcal{L}_F^p$ que le sous-espace $\mathcal{K}_F$ des fonctions continues à support compact est partout dense dans $\mathcal{L}_F^p$ (§ 3, n° 4, déf. 2). Toute fonction linéaire continue (pour la topologie de la convergence en moyenne d’ordre $p$), définie dans $\mathcal{K}_F$ et prenant ses valeurs dans un espace vectoriel topologique séparé et complet $G$, peut donc être prolongée par continuité de façon unique, en une fonction linéaire continue définie dans $\mathcal{L}_F^p$ et à valeurs dans $G$ (Top. gén., chap. II, 3e éd., § 3, n° 6, th. 2 et chap. III, § 3, prop. 3).

Or, pour toute fonction $f$ continue et à support compact, à valeurs dans l’espace de Banach $F$, nous avons défini (chap. III, § 3, n° 1) l’intégrale $\mu(f) = \int f\, d\mu$ par rapport à $\mu$, qui est un élément de $F$, et nous avons démontré (chap. III, § 3, n° 2, prop 5) l’inégalité

$$
\left| \int f\, d\mu \right| \leq \int |f|\, d|\mu| = N_1(f).
$$

Cette inégalité prouve que $f \mapsto \int f\, d\mu$ est une application linéaire de $\mathcal{K}_F$ dans $F$, continue pour la topologie de la convergence en moyenne dans $\mathcal{K}_F$. On peut donc la prolonger par continuité à l’espace $\mathcal{L}_F^1$ tout entier, et poser la définition suivante:

#### Définition 1 {#int-iv-s4-def-1 .statement}

On dit que les fonctions appartenant à $\mathcal{L}_F^1(X, \mu)$ sont intégrables pour la mesure $\mu$ (ou encore, sont $\mu$-intégrables). L’intégrale (par rapport à $\mu$) de la fonction intégrable $f$ est par définition la valeur pour $f$ du prolongement par continuité à $\mathcal{L}_F^1$ de l’application linéaire $g \mapsto \int g\, d\mu$ de $\mathcal{K}_F$ dans $F$; on la note encore $\mu(f)$ ou $\int f\, d\mu$, ou $\int f(x)\, d\mu(x)$ ou $\int f\mu$, ou $\int f(x)\mu(x)$.

Exemple — Soient X un espace discret, $\mu$ une mesure sur X et posons $\alpha(x) = \mu(\varphi_{\{x\}})$ pour tout $x \in X$. Les fonctions de $\mathcal{F}_F^1$ sont alors intégrables, autrement dit, $\mathcal{L}_F^1 = \mathcal{F}_F^1$; en outre, pour toute fonction $f \in \mathcal{L}_F^1$, on a

$$
\int f d\mu = \sum_{x \in X} \alpha(x)f(x).
$$

En effet, soit $f \in \mathcal{F}_F^1$; on a $|\mu|^*(|f|) = \sum_{x \in X} |\alpha(x)| \cdot |f(x)| < +\infty$ ($§ 1$, n° 3, Exemple); pour tout $\varepsilon > 0$, il existe une partie finie M de X telle que $\sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon$. La fonction g égale à f aux points $x \in M$ où f est finie, à 0 ailleurs, appartient à $\mathscr{K}(X; F)$ et l’on a, en vertu des conventions faites, $|\mu|^*(|f - g|) \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon$, ce qui prouve que $f \in \mathcal{L}_F^1$. D’autre part

$$
|\mu(g) - \sum_{x \in X} \alpha(x)f(x)| \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon
$$

d’où la seconde assertion.

En d’autres termes, les fonctions $\mu$-intégrables f sont celles pour lesquelles la famille $(\alpha(x)f(x))_{x \in X}$ est absolument sommable (Top. gén., chap. IX, § 3, n° 6), et l’intégrale $\int f d\mu$ est la somme de cette famille.

Comme $\mu(f)$ est continue dans $\mathcal{L}_F^1$ par définition et prend ses valeurs dans un espace séparé, on a $\mu(f) = 0$ pour toute fonction adhérente à 0 dans $\mathcal{L}_F^1$, c’est-à-dire négligeable ; si f et g sont deux fonctions intégrables équivalentes, on a $\mu(f) = \mu(g)$. En d’autres termes, la valeur de $\mu(f)$ ne dépend que de la classe $\tilde{f}$ de la fonction intégrable f ; on la note encore $\mu(\tilde{f})$, et la fonction $\tilde{f} \mapsto \mu(\tilde{f})$ est une application linéaire continue de $L_F^1$ dans F. Si une fonction f, à valeurs dans F, définie presque partout dans X, est équivalente à une fonction intégrable, on dit encore que f est intégrable, et on pose $\int f d\mu = \mu(\tilde{f})$; on définit de même une fonction intégrable à valeurs dans $\bar{\mathbf{R}}$, définie et finie presque partout, et son intégrale.

### 2. Propriétés de l’intégrale

#### Proposition 1 {#int-iv-s4-prop-1 .statement}

Pour toute fonction numérique $\mu$-intégrable positive $f$, on a

$$
\int f d|\mu| = \int^* f d|\mu| = N_1(f) \geq 0.
$$

En effet, $\int f d|\mu|$ et $N_1(f)$ sont continues dans $\mathcal{L}^1$ et égales pour toute fonction continue $f \geq 0$ à support compact; d’autre part, toute fonction $f \geq 0$ dans $\mathcal{L}^1$ est limite (au sens de la convergence en moyenne) d’une suite de fonctions $\geq 0$, continues et à support compact (§ 3, n° 5, prop. 11); d’où la proposition.

#### Corollaire 1 {#int-iv-s4-prop-1-cor-1 .statement}

Pour toute fonction intégrable $f \in \mathcal{L}_F^1$, $|f|$ est intégrable, et l’on a

$$
\int |f| d|\mu| = \int^* |f| d|\mu| = N_1(f).
$$

Nous ferons un usage fréquent de la prop. 1 et de son cor. 1, en remplaçant $\int^* f d|\mu|$ ou $N_1(f)$ par $\int f d|\mu|$ lorsqu’il s’agit d’une fonction intégrable $\geq 0$. Par exemple, pour que deux fonctions intégrables $f, g$ soient équivalentes, il faut et il suffit que

$$
\int |f - g| d|\mu| = 0.
$$

Rappelons que, pour qu’une fonction $f$ appartienne à $\mathcal{L}_F^p$, il faut et il suffit que la fonction $|f|^{p-1} \cdot f$ appartienne à $\mathcal{L}_F^1$ (§ 3, n° 8, cor 1. du th. 7), c’est-à-dire soit intégrable; cela explique la terminologie de « fonction de puissance $p$-ième intégrable ». En outre:

#### Corollaire 2 {#int-iv-s4-prop-1-cor-2 .statement}

Pour toute fonction $f \in \mathcal{L}_F^p$, la fonction numérique $|f|^p$ est intégrable, et l’on a

$$
N_p(f) = \left( \int |f|^p d|\mu| \right)^{1/p}.
$$

Cela résulte aussitôt de ce que $|f|$ appartient à $\mathcal{L}^p$ (§ 3, n° 5, prop. 11), et de la formule (2).

#### Proposition 2 {#int-iv-s4-prop-2 .statement}

Pour toute fonction intégrable $f$, on a

$$
\left| \int f d\mu \right| \leq \int |f| d|\mu|.
$$

Cela résulte aussitôt de l’inégalité (1) par passage à la limite, compte tenu de (3) et de la continuité de $N_1(f)$ dans $\mathcal{L}_F^1$.

#### Théorème 1 {#int-iv-s4-thm-1 .statement}

Soient $F$ et $G$ deux espaces de Banach, $u$ une application linéaire continue de $F$ dans $G$. Pour toute fonction intégrable $f$ à valeurs dans $F$, $u \circ f$ est intégrable et l’on a

$$
\int u(f(x)) d\mu(x) = u \left( \int f(x) d\mu(x) \right).
$$

Nous savons déjà que $u \circ f$ est intégrable (§ 3, n° 5, th. 4); la relation (6) étant valable pour $f \in \mathcal{K}_F$, s’étend à toute fonction intégrable $f$ par le principe de prolongement des identités : en effet, $f \mapsto u \circ f$ est continue pour la topologie de la convergence en moyenne, comme il résulte de l’inégalité $N_1(u \circ f) \leq \|u\| \cdot N_1(f)$.

#### Corollaire 1 {#int-iv-s4-thm-1-cor-1 .statement}

Soit $a'$ une forme linéaire continue sur $F$. Si $f$ est une fonction intégrable à valeurs dans $F$, la fonction numérique $\langle f, a' \rangle$ est intégrable, et l’on a
$$
\int \langle f(x), a' \rangle d\mu(x) = \left\langle \int f(x) d\mu(x), a' \right\rangle.
$$
Nous verrons au chap. VI, § 1, exerc. 7, 11 et 12 qu’il peut exister des fonctions $f$ à valeurs dans un espace de Banach $F$ de dimension infinie, telles que $\langle f, a' \rangle$ soit intégrable pour toute forme linéaire continue $a'$ sur $F$, sans que $f$ soit intégrable.

#### Corollaire 2 {#int-iv-s4-thm-1-cor-2 .statement}

Si les $a_k$ ($1 \leq k \leq n$) sont des vecteurs de $F$, et les $f_k$ ($1 \leq k \leq n$) des fonctions numériques intégrables, la fonction $f = \sum_{k=1}^n a_k f_k$ est intégrable, et l’on a
$$
\int \left( \sum_{k=1}^n a_k f_k \right) d\mu = \sum_{k=1}^n a_k \int f_k d\mu.
$$

### 3. Passages à la limite dans les intégrales

#### Proposition 3 {#int-iv-s4-prop-3 .statement}

Soit $\mathcal{B}$ une base de filtre sur $\mathcal{L}_F^1$. On suppose qu’il existe un ensemble compact $K \subset X$ tel que, pour toute partie $M \in \mathcal{B}$, toutes les fonctions $f \in M$ aient leur support dans $K$. Dans ces conditions, si $\mathcal{B}$ converge uniformément dans $X$ vers $f_0$, la fonction $f_0$ est intégrable, et l’on a
$$
\int f_0 d\mu = \lim_{\mathcal{B}} \int f d\mu.
$$
En effet, $\mathcal{B}$ converge en moyenne vers $f_0$ (§ 3, n° 3, prop. 4).

#### Proposition 4 {#int-iv-s4-prop-4 .statement}

Soit $(f_n)$ une suite croissante (resp. décroissante) de fonctions numériques intégrables. Pour que l’enveloppe supérieure (resp. inférieure) $f$ de cette suite soit intégrable, il faut et il suffit que $\sup_n \int f_n d|\mu| < +\infty$ (resp. $\inf_n \int f_n d|\mu| > -\infty$) et l’on a alors
$$
\int f d\mu = \lim_{n \to \infty} \int f_n d\mu.
$$

Bornons-nous à considérer une suite croissante. La suite des $g_n = f_n + f_1^-$ est croissante et formée de fonctions intégrables $\geqslant 0$; comme son enveloppe supérieure est $g = f + f_1^-$, la proposition résulte du th. 5 du § 3, n° 6.

#### Théorème 2 {#int-iv-s4-thm-2 .statement}

Soit $A$ un ensemble d’indices, filtré par un filtre $\mathfrak{F}$ à base dénombrable. Soit $(\mathbf{f}_\alpha)_{\alpha \in A}$ une famille de fonctions intégrables qui, suivant le filtre $\mathfrak{F}$, convergent simplement presque partout vers une fonction $\mathbf{f}$; s’il existe une fonction numérique $g \geqslant 0$ telle que $\int^* g \, d|\mu| < +\infty$, et que $|\mathbf{f}_\alpha(x)| \leqslant g(x)$ presque partout dans $X$ pour tout $\alpha \in A$, la fonction $\mathbf{f}$ est intégrable, et l’on a
$$
\int \mathbf{f} \, d\mu = \lim_{\mathfrak{F}} \int \mathbf{f}_\alpha \, d\mu.
$$
Le théorème résulte du th. de Lebesgue (§ 3, n° 7, cor. du th. 6) puisque, dans les conditions de l’énoncé, $\mathbf{f}_\alpha$ converge en moyenne vers $\mathbf{f}$ suivant $\mathfrak{F}$.

#### Corollaire 1 {#int-iv-s4-thm-2-cor-1 .statement}

Soient $\Omega$ un espace topologique, $t_0$ un point de $\Omega$ admettant un système fondamental dénombrable de voisinages, $\mathbf{f}$ une application de $X \times \Omega$ dans $F$, ayant les propriétés suivantes:
a) pour tout $t \in \Omega$, la fonction $x \mapsto \mathbf{f}(x, t)$ est intégrable;
b) pour tout $x \in X$, la fonction $t \mapsto \mathbf{f}(x, t)$ est continue en $t_0$;
c) il existe un voisinage $U$ de $t_0$ et une fonction numérique $g \geqslant 0$ définie dans $X$, telle que $\int^* g \, d|\mu| < +\infty$, et que $|\mathbf{f}(x, t)| \leqslant g(x)$ pour $x \in X$ et $t \in U$.
Dans ces conditions, l’application $t \mapsto \int \mathbf{f}(x, t) \, d\mu(x)$ de $\Omega$ dans $F$ est continue au point $t_0$.

#### Corollaire 2 {#int-iv-s4-thm-2-cor-2 .statement}

Soit $(\mathbf{f}_n)$ une suite de fonctions intégrables telle que la série de terme général $\mathbf{f}_n(x)$ converge presque partout; s’il existe une fonction $g \geqslant 0$ telle que $\int^* g \, d|\mu| < +\infty$, et que, pour tout entier $n$, on ait $\left| \sum_{k=1}^n \mathbf{f}_k(x) \right| \leqslant g(x)$ presque partout, alors la somme $\mathbf{f}(x)$ (définie presque partout) de la série de terme général $\mathbf{f}_n(x)$ est intégrable, et l’on a
$$
\int \mathbf{f} \, d\mu = \sum_{n=1}^\infty \int \mathbf{f}_n \, d\mu
$$
(« intégration terme à terme d’une série »).

### 4. Caractérisations des fonctions numériques intégrables

#### Proposition 5 {#int-iv-s4-prop-5 .statement}

Pour qu’une fonction numérique $f \geq 0$ (finie ou non) semi-continue inférieurement dans E, soit intégrable, il faut et il suffit que $\int^* f d|\mu| < +\infty$.

Tout revient à prouver que la condition est suffisante. La définition de $|\mu|^*(f)$ (§ 1, n° 1, déf. 1) prouve que, pour tout $\varepsilon > 0$, il existe une fonction continue $g \geq 0$, à support compact, telle que $g \leq f$ et $|\mu|^*(f) \leq |\mu|(g) + \varepsilon$. Mais $f - g$ est semi-continue inférieurement et $\geq 0$, donc (§ 1, n° 1, th. 2)
$$
|\mu|^*(f) = |\mu|(g) + |\mu|^*(f - g),
$$
autrement dit $N_1(f - g) = |\mu|^*(f - g) = |\mu|^*(f) - |\mu|(g) \leq \varepsilon$, ce qui prouve que $f$ est intégrable (§ 3, n° 3, prop. 7).

#### Corollaire 1 {#int-iv-s4-prop-5-cor-1 .statement}

Pour qu’une fonction numérique finie $f \geq 0$, semi-continue supérieurement dans X, soit intégrable, il faut et il suffit que $\int^* f d|\mu| < +\infty$.

En effet, si $|\mu|^*(f) < +\infty$, il existe une fonction $h$, semi-continue inférieurement, telle que $f \leq h$ et $|\mu|^*(h) < +\infty$; $h - f$ est définie partout et semi-continue inférieurement, et on a $|\mu|^*(h - f) \leq |\mu|^*(h) < +\infty$; donc $h - f$ est intégrable, et comme $f(x) = h(x) - (h(x) - f(x))$ presque partout, $f$ est intégrable.

#### Corollaire 2 {#int-iv-s4-prop-5-cor-2 .statement}

Soit H un ensemble non vide, filtrant pour la relation $\leq$ (resp. $\geq$) de fonctions numériques semi-continues inférieurement (resp. supérieurement) et intégrables; si
$$
\sup_{f \in H} \int f d|\mu| < +\infty
$$
(resp. $\inf_{f \in H} \int f d|\mu| > -\infty$), l’enveloppe supérieure (resp. inférieure) g de H est intégrable et l’on a
$$
\int g \, d\mu = \lim_{f \in H} \int f \, d\mu
$$
et $\int g \, d|\mu| = \sup_{f \in H} \int f d|\mu|$ (resp. $\int g \, d|\mu| = \inf_{f \in H} \int f d|\mu|$).

On peut se borner au cas des fonctions semi-continues inférieurement; les fonctions $f^+$ (resp. $f^-$), lorsque $f$ parcourt H, forment alors un ensemble filtrant pour $\leq$ (resp. $\geq$) de fonctions semi-continues inférieurement (resp. supérieurement) et $\geq 0$; l’enveloppe supérieure (resp. inférieure) des $f^+$ (resp. $f^-$) pour $f \in \mathrm{H}$, est égale à $g^+$ (resp. $g^-$). D’autre part, on peut remplacer $\mathrm{H}$ par une de ses sections (qui lui est cofinale), formée des $f \in \mathrm{H}$ qui sont $\geqslant f_0$, pour une fonction $f_0 \in \mathrm{H}$; on a alors $\int f^+ d|\mu| \leqslant \int f d|\mu| + \int f_0^- d|\mu|$; on voit ainsi qu’on est ramené à prouver les deux assertions du corollaire lorsque $\mathrm{H}$ est formé de fonctions positives. Si $\mathrm{H}$ est filtrant pour $\leqslant$ et formé de fonctions $\geqslant 0$, semi-continues inférieurement, on sait alors (§ 1, n° 1, th. 1) que
$$
|\mu|^*(g) = \sup_{f \in \mathrm{H}} |\mu|^*(f) = \sup_{f \in \mathrm{H}} \int f d|\mu| < +\infty,
$$
donc $g$, qui est semi-continue inférieurement, est intégrable en vertu de la prop. 5; on a $\int g d|\mu| = \lim_{f \in \mathrm{H}} \int f d|\mu|$, et comme $f \leqslant g$, $\lim_{f \in \mathrm{H}} \mathrm{N}_1(g - f) = 0$, ce qui montre que $f$ converge en moyenne vers $g$ suivant $\mathrm{H}$, et prouve donc le corollaire dans ce cas. Si $\mathrm{H}$ est filtrant pour $\geqslant$ et formé de fonctions $f$ semi-continues supérieurement et intégrables, telles que $0 \leqslant f \leqslant f_1$ avec $f_1 \in \mathrm{H}$, il existe une fonction $h$ semi-continue inférieurement et intégrable, telle que $f_1 \leqslant h$; on peut écrire $f = h - f'$, où $f'(x) = h(x) - f(x)$ lorsque $f(x) < +\infty$, et $f'(x) = 0$ dans le cas contraire. Il est clair que les $f'$ forment un ensemble filtrant pour $\leqslant$ de fonctions $\geqslant 0$, semi-continues inférieurement et intégrables, avec
$$
\int f' d|\mu| \leqslant \int h d|\mu| < +\infty;
$$
on peut leur appliquer ce qui a été démontré ci-dessus; si $g'$ est l’enveloppe supérieure des $f'$, $h$ et $g'$ sont finies presque partout, donc $h - g'$ est définie presque partout et égale à $g$ presque partout; on en tire aussitôt les conclusions du corollaire dans ce cas.

#### Corollaire 3 {#int-iv-s4-prop-5-cor-3 .statement}

Soit $f$ une fonction numérique bornée, semi-continue supérieurement dans $X$ et à support compact. Alors l’application $\mu \mapsto \int f d\mu$ est semi-continue supérieurement dans $\mathcal{M}_+(X)$ pour la topologie vague.

Si $h$ est une fonction de $\mathscr{K}_+(X)$ telle que $|f| \leqslant h$ (chap. III, § 1, n° 2, lemme 1), on a $0 \leqslant f + h \leqslant 2h$, et comme $f + h$ est semi-continue supérieurement, il résulte du cor. 1 que $f$ est $\mu$-intégrable pour toute mesure $\mu$ sur $X$. En outre, on a $\mu(f) = \mu(h) - \mu(h - f)$ et $h - f$ est une fonction semi-continue inférieurement et $\geqslant 0$. Comme l’application $\mu \mapsto \mu(h - f)$ est semi-continue inférieurement dans $\mathcal{M}_+(X)$ pour la topologie vague (§ 1, n° 1, prop. 4), cela démontre le corollaire.

#### Théorème 3 {#int-iv-s4-thm-3 .statement}

Pour qu’une fonction numérique $f \geq 0$ soit intégrable, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe une fonction semi-continue supérieurement $g \geq 0$, à valeurs finies et à support compact, et une fonction intégrable semi-continue inférieurement $h$, telles que $g \leq f \leq h$ et que $\int (h - g)\ d|\mu| \leq \varepsilon$.

La condition est suffisante d’après un critère général d’intégrabilité ($§ 3$, n° 4, prop. 8), la prop. 5 et son corollaire 1. Montrons que la condition est nécessaire. Si $f \geq 0$ est intégrable, pour tout $\varepsilon > 0$, il existe une fonction $u \geq 0$, continue et à support compact, telle que $N_1(f - u) \leq \varepsilon/4$. D’après la définition de $N_1$, cela entraîne qu’il existe une fonction $v \geq 0$, semi-continue inférieurement, telle que $\mu^*(v) \leq \varepsilon/2$ et $|f - u| \leq v$. On a donc $-v(x) \leq f(x) - u(x) \leq v(x)$ pour tout $x \in X$, et comme $u(x)$ est partout fini, on en déduit $(u(x) - v(x))^+ \leq f(x) \leq u(x) + v(x)$ pour tout $x \in X$. Les fonctions $g = (u - v)^+$ et $h = u + v$ répondent à la question.

#### Corollaire {#int-iv-s4-n4-cor-1 .statement}

Pour toute fonction numérique intégrable $f$ (resp. intégrable et $\geq 0$), il existe une suite croissante $(g_n)$ de fonctions semi-continues supérieurement et intégrables (resp. à valeurs finies, à supports compacts et intégrables), et une suite décroissante $(h_n)$ de fonctions semi-continues inférieurement et intégrables, telles que:

$1^\circ$ $g_n(x) \leq f(x) \leq h_n(x)$ pour tout $x \in X$ et tout entier $n$;
$2^\circ$ $f(x)$ est égale presque partout à l’enveloppe inférieure $h$ de la suite $(h_n)$ et à l’enveloppe supérieure $g$ de la suite $(g_n)$;
$3^\circ$ $\int f\ d\mu = \lim_{n \to \infty} \int g_n\ d\mu = \lim_{n \to \infty} \int h_n\ d\mu$.

Supposons d’abord $f \geq 0$. D’après le th. 3, pour tout $n$ il existe une fonction $v_n$, intégrable et semi-continue inférieurement, et une fonction $u_n$ semi-continue supérieurement, à valeurs finies et à support compact, telles que $u_n \leq f \leq v_n$ et $\int (v_n - u_n)\ d|\mu| \leq 1/n$; si on pose $g_n = \sup(u_1, u_2, \ldots, u_n)$ et $h_n = \inf(v_1, v_2, \ldots, v_n)$, les suites $(g_n)$ et $(h_n)$ répondent à la question. En effet, comme $g \leq f$, $g$ est intégrable en vertu de la prop. 4 du n° 3, et comme
$$
\int (f - g_n)\ d|\mu| \leq \int (v_n - u_n)\ d|\mu| \leq \frac{1}{n},
$$
on a $\int (f - g)\ d|\mu| = \lim_{n \to \infty} \int (f - g_n)\ d|\mu| = 0$ (n° 3, prop. 4), ce qui prouve que $f$ et $g$ sont équivalentes. On raisonne de même pour la suite $(h_n)$.

Si $f$ n’est pas positive, on peut appliquer à $f^+$ et $f^-$ ce qui précède, et il y a donc deux suites croissantes $(g'_n), (g''_n)$ de fonctions semi-continues supérieurement et intégrables, et deux suites décroissantes $(h'_n), (h''_n)$ de fonctions semi-continues inférieurement et intégrables telles que: 1° $g'_n \leq f^+ \leq h'_n,\ g''_n \leq -f^- \leq h''_n$; 2° $f^+$ (resp. $-f^-$) est égale presque partout à l’enveloppe supérieure des $g'_n$ et à l’enveloppe inférieure des $h'_n$ (resp. à l’enveloppe supérieure des $g''_n$ et à l’enveloppe inférieure des $h''_n$); 3°:

$$
\int f^+ d\mu = \lim_{n \to \infty} \int g'_n d\mu = \lim_{n \to \infty} \int h'_n d\mu,
$$
$$
-\int f^- d\mu = \lim_{n \to \infty} \int g''_n d\mu = \lim_{n \to \infty} \int h''_n d\mu.
$$

En outre, on peut supposer que les $g'_n$ et les $h''_n$ sont partout finies; alors il est clair que les suites des $g_n = g'_n + g''_n$ et $h_n = h'_n + h''_n$ répondent à la question.

#### Exemple {#int-iv-s4-n4-exa-1 .statement}

Pour toute mesure positive $\mu$ sur $\mathbf{R}$, toute fonction en escalier à support compact est $\mu$-intégrable; en effet, une fonction caractéristique d’intervalle ouvert (resp. fermé) est semi-continue inférieurement (resp. supérieurement), et toute fonction en escalier est combinaison linéaire de telles fonctions caractéristiques. On en déduit que si $\mathbf{f}$ est une fonction réglée dans $\mathbf{R}$ et à support compact (*Fonct. var. réelle*, chap. II, § 1, no 3), $\mathbf{f}$ est intégrable, car elle est limite uniforme d’une suite de fonctions en escalier $\mathbf{g}_n$ à support contenu dans un ensemble compact fixe (no 3, prop. 3); on a en outre $\int \mathbf{f}\, d\mu = \lim_{n \to \infty} \int \mathbf{g}_n\, d\mu$.

Si l’on prend en particulier pour $\mu$ la mesure de Lebesgue, on voit que pour toute fonction réglée $\mathbf{f}$ à support compact, l’intégrale $\int \mathbf{f}\, d\mu$ est égale à l’intégrale $\int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$ définie dans *Fonct. var. réelle*, chap. II, § 2, no 1.

#### Remarque 1 {#int-iv-s4-n4-rem-1 .statement}

Soit $\mathbf{f}$ une fonction réglée dans $\mathbf{R}$ et intégrable pour la mesure de Lebesgue $\mu$; alors $|\mathbf{f}|$ est aussi intégrable (no 2, cor. 1 de la prop. 1), et si l’on pose $I_n = (-n, +n)$, $|\mathbf{f}|$ est l’enveloppe supérieure de la suite croissante des fonctions réglées $|\mathbf{f}| \varphi_{I_n}$, donc $\int |\mathbf{f}|\, d\mu = \lim_{n \to \infty} \int_{-n}^{n} |\mathbf{f}(x)|\, dx$ d’après le th. 2 du no 3; donc l’intégrale $\int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$ est *absolument convergente* (*Fonct. var. réelle*, chap. II, § 2, no 3). En outre, $\int \mathbf{f}\, d\mu = \int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$ d’après le th. 2 du n° 3. Réciproquement, supposons que $\int_{-\infty}^{+\infty} f(x) dx$ soit absolument convergente; on a encore, en vertu du th. 2 du n° 3, $\int f d\mu = \int_{-\infty}^{+\infty} f(x) dx$. On notera que si l’intégrale $\int_{-\infty}^{+\infty} f(x) dx$ est convergente sans être absolument convergente, $f$ *n’est pas intégrable* pour la mesure de Lebesgue.

#### Remarque 2 {#int-iv-s4-n4-rem-2 .statement}

Appliquée à la mesure de Lebesgue et aux fonctions réglées, la prop. 3 du n° 3 redonne le théorème de passage à la limite pour les intégrales de fonctions réglées dans un intervalle compact (*Fonct. var. réelle*, chap. II, § 3, n° 1, prop. 1); pour les *suites* (ou les filtres à base dénombrable) de fonctions réglées, le th. 2 du n° 3 améliore beaucoup cette proposition, puisque, pour les fonctions réglées uniformément bornées dans un intervalle compact, il substitue la convergence *simple* à la convergence *uniforme* (cf. § 5, n° 4, th. 2). Mais en ce qui concerne le passage à la limite pour les intégrales *absolument convergentes* de fonctions réglées dans un intervalle non compact, on observera que les conditions du th. 2 du n° 3 impliquent que les intégrales considérées sont *uniformément convergentes* (au sens défini dans *Fonct. var. réelle*, chap. II, § 3, n° 2), et n’améliorent donc les conditions de convergence données au Livre IV (*loc. cit.*) qu’en ce qui concerne la convergence des fonctions $f_\alpha$ dans tout intervalle compact. Enfin, les conditions de passage à la limite données pour des intégrales de fonctions réglées *non absolument convergentes* restent en dehors de la théorie développée dans ce chapitre.

### 5. Ensembles intégrables

#### Définition 2 {#int-iv-s4-def-2 .statement}

*On dit qu’une partie* $A$ *d’un espace localement compact* $X$ *est intégrable pour une mesure* $\mu$ *sur* $X$ *(ou encore est* $\mu$*-intégrable*) si la fonction caractéristique* $\varphi_A$ *de* $A$ *est intégrable.* *Le nombre fini* $\mu(A) = \int \varphi_A d\mu$ *est appelé mesure de* $A$.

Pour tout ensemble intégrable $A$, on a $|\mu|(A) = |\mu|^*(A)$ (prop. 1); pour qu’un ensemble soit négligeable, il faut et il suffit qu’il soit de mesure nulle pour $|\mu|$.

#### Proposition 6 {#int-iv-s4-prop-6 .statement}

*La réunion d’une famille finie* $(A_i)_{1 \leq i \leq n}$ *d’ensembles intégrables est intégrable, et on a*
$$
|\mu|\left( \bigcup_{i=1}^n A_i \right) \leq \sum_{i=1}^n |\mu|(A_i).
$$
*En outre, si les* $A_i$ *sont deux à deux sans point commun, on a*
$$
\mu\left( \bigcup_{i=1}^n A_i \right) = \sum_{i=1}^n \mu(A_i).
$$

En effet, si $A = \bigcup_{i=1}^n A_i$, on a $\varphi_A = \sup \varphi_{A_i}$, donc (§ 3, n° 5, cor. de la prop. 12) si les $A_i$ sont intégrables, il en est de même de $A$; la relation (13) est un cas particulier de la relation analogue pour les mesures extérieures (§ 1, n° 4, prop. 18), compte tenu de la relation $|\mu|(A) = |\mu|^*(A)$; enfin, si les $A_i$ sont deux à deux sans point commun, on a $\varphi_A = \sum_{i=1}^n \varphi_{A_i}$; d’où (14).

#### Proposition 7 {#int-iv-s4-prop-7 .statement}

1° Si $A$ et $B$ sont deux ensembles intégrables tels que $B \subset A$, l’ensemble $C = A - B$ est intégrable, et on a
$$
\mu(C) = \mu(A) - \mu(B).
$$
2° *L’intersection d’une famille dénombrable d’ensembles intégrables est intégrable*.

La première partie résulte de ce que $\varphi_C = \varphi_A - \varphi_B$. D’autre part, si $(A_n)$ est une suite d’ensembles intégrables, et $A$ son intersection, on a $\varphi_A = \inf_n \varphi_{A_n}$, donc $A$ est intégrable (n° 3, prop. 4).

#### Corollaire {#int-iv-s4-n5-cor-1 .statement}

*Si $(A_n)$ est une suite décroissante d’ensembles intégrables, on a* $\mu\left( \bigcap_n A_n \right) = \lim_{n \to \infty} \mu(A_n)$.

En effet, si $A = \bigcap_n A_n$, $\varphi_A$ est l’enveloppe inférieure de la suite décroissante $(\varphi_{A_n})$ (n° 3, prop. 4).

#### Proposition 8 {#int-iv-s4-prop-8 .statement}

*Soit $(A_n)$ une suite croissante d’ensembles intégrables; pour que la réunion $A = \bigcup_n A_n$ soit intégrable, il faut et il suffit que* $\sup_n |\mu|(A_n) < +\infty$; *on a alors*
$$
\mu(A) = \lim_{n \to \infty} \mu(A_n).
$$
En effet, les $\varphi_{A_n}$ forment une suite croissante de fonctions intégrables, et $\varphi_A = \sup \varphi_{A_n}$; la proposition résulte donc de la prop. 4 du n° 3.

#### Corollaire {#int-iv-s4-n5-cor-2 .statement}

*Soit $(A_n)$ une suite d’ensembles intégrables telle que* $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$; *la réunion* $A = \bigcup_n A_n$ *est intégrable, et* on a
(17) $$ |\mu|\left(\bigcup_n A_n\right) \leq \sum_{n=1}^\infty |\mu|(A_n). $$
En effet, on a $\varphi_A = \sup_n \varphi_{A_n}$, et
$$ |\mu|^*(A) \leq \sum_{n=1}^\infty |\mu|^*(A_n) = \sum_{n=1}^\infty |\mu|(A_n) < +\infty $$
(§ 1, n° 4, prop. 18); A est donc intégrable (§ 3, n° 6, cor. 2 du th. 5) et comme $|\mu|(A) = |\mu|^*(A)$, on a bien (17).

#### Proposition 9 {#int-iv-s4-prop-9 .statement}

Soit $(A_n)$ une suite d’ensembles intégrables, deux à deux sans point commun, et telle que $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$; on a alors
(18)
$$
\mu\left(\bigcup_n A_n\right) = \sum_{n=1}^\infty \mu(A_n).
$$
En effet, si $A = \bigcup_n A_n$, on a $\varphi_A = \sum_{n=1}^\infty \varphi_{A_n}$ et la proposition résulte de (17) et du cor. 2 du th. 2 du n° 3.

On exprime encore la relation (18) en disant que la mesure $\mu$ est complètement additive dans l’ensemble des parties intégrables de X.

### 6. Critères d’intégrabilité d’un ensemble

#### Proposition 10 {#int-iv-s4-prop-10 .statement}

Pour qu’un ensemble A ouvert (resp. fermé) dans X soit intégrable, il faut et il suffit que $|\mu|^*(A) < +\infty$.
Comme $\varphi_A$ est alors semi-continue inférieurement (resp. supérieurement), la proposition résulte de la prop. 5 du n° 4 et de son corollaire 1.

#### Corollaire 1 {#int-iv-s4-prop-10-cor-1 .statement}

Tout ensemble compact est intégrable; tout ensemble ouvert relativement compact est intégrable.

#### Corollaire 2 {#int-iv-s4-prop-10-cor-2 .statement}

Pour toute mesure positive $\mu$ sur X, $A \mapsto \mu^*(A)$ est une capacité sur X (cf. Top. gén., chap. IX, 2e éd., § 6, n° 9, Exemple).

#### Exemple {#int-iv-s4-n6-exa-1 .statement}

Pour la mesure de Lebesgue $\mu$ sur $\mathbf{R}$, il résulte de la prop. 10 que tout intervalle ouvert borné $]a, b[$ est intégrable et a pour mesure $b - a$ (§ 1, n° 2, prop. 9). Comme tout ensemble réduit à un point est négligeable pour la mesure de Lebesgue, on déduit de là que tous les intervalles d’extrémités $a$ et $b$ ont même mesure $b - a$.

#### Proposition 11 {#int-iv-s4-prop-11 .statement}

*Soit $\mathcal{G}$ un ensemble, filtrant pour la relation $\subset$, d’ensembles ouverts intégrables de $X$; pour que $A = \bigcup_{G \in \mathcal{G}} G$ soit intégrable, il faut et il suffit que $\sup_{G \in \mathcal{G}} |\mu|(G) < +\infty$, et l’on a alors $\mu(A) = \lim_{\mathcal{G}} \mu(G)$ et $|\mu|(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$.*

On sait en effet que $|\mu|^*(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$ (§ 1, n° 2, prop. 7); la proposition résulte donc de la prop. 10.

#### Corollaire {#int-iv-s4-n6-cor-1 .statement}

*Soit $\mathfrak{F}$ un ensemble, filtrant pour la relation $\supset$, d’ensembles fermés intégrables dans $E$; l’ensemble fermé $B = \bigcap_{H \in \mathfrak{F}} H$ est intégrable, et l’on a $\mu(B) = \lim_{\mathfrak{F}} \mu(H)$ et $|\mu|(B) = \inf_{H \in \mathfrak{F}} |\mu|(H)$.*

En effet, soit $H_0$ un ensemble de $\mathfrak{F}$; comme $H_0$ est intégrable, il est contenu dans un ensemble ouvert intégrable $U$ (§ 1, n° 4, prop. 19); les ensembles ouverts $U \cap \overline{CH}$ forment un ensemble filtrant pour la relation $\subset$, contenus dans $U$ et dont la réunion est $U \cap \overline{CB}$; on est donc ramené à la prop. 11.

#### Théorème 4 {#int-iv-s4-thm-4 .statement}

*Pour qu’un ensemble $A$ soit intégrable, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un ensemble ouvert intégrable $G$ et un ensemble compact $K$, tels que $K \subset A \subset G$ et que*

$$
|\mu|(G - K) = |\mu|(G) - |\mu|(K) \leq \varepsilon.
$$

a) La condition est *suffisante*, car elle signifie que $\varphi_K \leq \varphi_A \leq \varphi_G$ et $\int (\varphi_G - \varphi_K) d|\mu| \leq \varepsilon$; comme $\varphi_G$ et $\varphi_K$ sont intégrables, il en est de même de $\varphi_A$ (§ 3, n° 4, prop. 8).

b) La condition est *nécessaire*. Si $A$ est intégrable, il existe un ensemble ouvert $G \supset A$, tel que $|\mu|^*(G)$ soit arbitrairement voisin de $|\mu|^*(A) = |\mu|(A)$ (§ 1, n° 4, prop. 19); tout revient donc à prouver que, pour tout $\varepsilon > 0$, il existe un ensemble compact $K \subset A$ tel que $|\mu|(A) - |\mu|(K) \leq \varepsilon$. Comme $\varphi_A$ est intégrable, il existe une fonction $f \geq 0$, semi-continue supérieurement et à support compact $S$, telle que $f \leq \varphi_A$ et $\int (\varphi_A - f) d|\mu| \leq \frac{\varepsilon}{2}$ (th. 3, n° 4). Soit $\delta > 0$ un nombre arbitraire, et soit $K$ l’ensemble des points $x \in E$ tels que $f(x) \geq \delta$; $K$ est fermé et contenu dans $S$, donc *compact*, et comme

S ⊂ A, on a K ⊂ A. L’ensemble B = A − K est intégrable, et on a $f \leq \varphi_K + \delta \varphi_B$, d’où

$$
\int f d|\mu| \leq |\mu|(K) + \delta . |\mu|(B) \leq |\mu|(K) + \delta . |\mu|(A),
$$

et finalement

$$
|\mu|(A) \leq \int f d|\mu| + \frac{\varepsilon}{2} \leq |\mu|(K) + \delta . |\mu|(A) + \frac{\varepsilon}{2},
$$

ce qui achève la démonstration, puisque $\delta$ est arbitraire.

#### Corollaire 1 {#int-iv-s4-thm-4-cor-1 .statement}

Pour qu’un ensemble A soit intégrable, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un ensemble compact $K \subset A$ tel que $|\mu|^*(A - K) \leq \varepsilon$. La mesure $|\mu|(A)$ est alors la borne supérieure de l’ensemble des mesures $|\mu|(K)$ des ensembles compacts $K \subset A$.

La condition est nécessaire, car si G et K satisfont aux conditions du th. 4, on a

$$
|\mu|^*(A - K) \leq |\mu|^*(G - K) \leq \varepsilon.
$$

La condition est suffisante, car elle exprime que, pour la topologie de la convergence en moyenne, $\varphi_A$ est adhérente à l’ensemble des fonctions intégrables $\varphi_K$ (K partie compacte arbitraire de A).

#### Corollaire 2 {#int-iv-s4-thm-4-cor-2 .statement}

Pour tout ensemble intégrable A, il existe :

1° un ensemble $A_1 \supset A$, intersection dénombrable d’ensembles ouverts intégrables, et tel que $A_1 - A$ soit négligeable ;
2° un ensemble $A_2 \subset A$, réunion dénombrable d’ensembles compacts deux à deux sans point commun et tel que $A - A_2$ soit négligeable.

1° Pour tout entier n, il existe un ensemble ouvert intégrable $G_n$ tel que $|\mu|(G_n) - |\mu|(A) \leq \frac{1}{n}$; si $A_1$ est l’intersection des $G_n$, on a $|\mu|(A_1) = |\mu|(A)$ (n° 5, cor. de la prop. 7), donc $A_1 - A$ est négligeable.

2° Définissons les ensembles compacts $K_n$ par récurrence de la façon suivante : $K_1 \subset A$ et $|\mu|(A - K_1) \leq 1$; $K_n \subset A - \left( \bigcup_{i=1}^{n-1} K_i \right)$, et $|\mu|(A \cap C \left( \bigcup_{i=1}^{n-1} K_i \right) \cap C K_n) \leq \frac{1}{n}$ pour $n > 1$ (th. 4); si $A_2$ est la réunion des $K_n$, on a $|\mu|(A_2) = |\mu|(A)$ (n° 5, prop. 8), donc $A - A_2$ est négligeable.

#### Corollaire 3 {#int-iv-s4-thm-4-cor-3 .statement}

Tout ensemble de mesure extérieure finie est contenu dans la réunion d’un ensemble négligeable et d’une famille dénombrable d’ensembles compacts, deux à deux sans point commun, dont la somme des mesures est finie.

Il suffit d’appliquer le cor. 2 à un ensemble ouvert intégrable contenant l’ensemble donné.

#### Corollaire 4 {#int-iv-s4-thm-4-cor-4 .statement}

Pour tout ensemble ouvert $U$ dans $E$, $|\mu|^*(U)$ est la borne supérieure des mesures $|\mu|(K)$ des ensembles compacts $K \subset U$.

C’est immédiat si $|\mu|^*(U) < +\infty$ en raison du th. 4. Si $|\mu|^*(U) = +\infty$, pour tout entier $n$, il existe par hypothèse une fonction $f \in \mathcal{K}_+$ telle que $f \leq \varphi_U$ et $|\mu|(f) \geq n$. Si $K$ est le support compact de $f$, on a $f \leq \varphi_K \leq \varphi_U$, d’où $|\mu|(K) \geq n$, ce qui démontre le corollaire.

On notera que $|\mu|^*(U)$ est aussi la borne supérieure des mesures $|\mu|(G)$ des ensembles ouverts relativement compacts tels que $\bar{G} \subset U$. En effet, si $K$ est un ensemble compact contenu dans $U$, pour tout $x \in K$, il existe un voisinage ouvert relativement compact $V$ de $x$ tel que $\bar{V} \subset U$. En recouvrant $K$ par un nombre fini de ces voisinages, leur réunion $G$ est un ensemble ouvert relativement compact tel que $\bar{G} \subset U$ et $K \subset G$, d’où
$$
\mu(K) \leq |\mu|(G) \leq |\mu|^*(U).
$$

### 7. Caractérisation des mesures bornées

#### Proposition 12 {#int-iv-s4-prop-12 .statement}

Pour qu’une mesure $\mu$ sur un espace localement compact $X$ soit bornée (chap. III, § 1, n° 8), il faut et il suffit que $X$ soit un ensemble intégrable pour $\mu$ (ou, ce qui revient au même, que toute fonction constante finie soit intégrable); on a alors
$$
\| \mu \| = |\mu|(X) = \int d|\mu|.
$$
En effet, on a vu que $|\mu|^*(X) = \| \mu \|$ (§ 1, n° 2); la proposition résulte donc de la prop. 10 du n° 6.

Pour toute mesure bornée $\mu$, on dit encore que $\mu(X)$ est la masse totale de $\mu$.

Il résulte du th. 4 n° 5 que si $\mu$ est une mesure bornée, pour tout $\varepsilon > 0$, il existe un ensemble compact $K$ tel que $|\mu|(C K) \leq \varepsilon$.

#### Proposition 13 {#int-iv-s4-prop-13 .statement}

Soit $\mu$ une mesure bornée sur $X$. Soit $\mathcal{B}$ une base de filtre sur $\mathcal{L}_F^p$, ayant les propriétés suivantes :
1° il existe un ensemble $M \in \mathcal{B}$ tel que les fonctions $f \in M$ soient uniformément bornées dans $X$;
2° $\mathcal{B}$ converge uniformément dans toute partie compacte de $X$ vers une fonction $f_0$.
Dans ces conditions, $f_0$ appartient à $\mathcal{L}_F^p$ et $\mathcal{B}$ converge en moyenne d’ordre $p$ vers $f_0$.
Remarquons d’abord que si $|f(x)| \leq a$ pour tout $x \in X$ et toute fonction $f \in M$, on a aussi $|f_0(x)| \leq a$ pour tout $x \in X$. Cela étant, pour tout $\varepsilon > 0$, il existe un ensemble compact $K$ tel que $|\mu|(C K) \leq \varepsilon^p$ et un ensemble $N \in \mathcal{B}$ tel que, pour toute fonction $f \in N$, on ait $|f(x) - f_0(x)| \leq \varepsilon(|\mu|(K))^{-1/p}$ pour tout $x \in K$. Or, on peut écrire
$$
f - f_0 = (f - f_0)\varphi_K + (f - f_0)\varphi_{C K};
$$
il résulte de ce qui précède que, si $f \in M \cap N$, on a $N_p((f - f_0)\varphi_K) \leq \varepsilon$ et $N_p((f - f_0)\varphi_{C K}) \leq 2a\varepsilon$, d’où $N_p(f - f_0) \leq (2a + 1)\varepsilon$, ce qui démontre la proposition.

#### Corollaire {#int-iv-s4-n7-cor-1 .statement}

Pour une mesure $\mu$ bornée sur $X$, toute application $f$ continue et bornée de $X$ dans $F$ appartient à chacun des $\mathcal{L}_F^p (1 \leq p < +\infty)$.
En effet, pour toute partie compacte $K$ de $X$, soit $M_K$ l’ensemble des applications de $X$ dans $F$ de la forme $h f$, où $h$ est une application continue de $X$ dans $\{0, 1\}$ égale à 1 dans $K$ et à support compact. Il est clair que les ensembles $M_K$ forment dans $\mathcal{L}_F^p$ une base de filtre $\mathcal{B}$, que les fonctions appartenant à $M_K$ sont uniformément bornées, et que $\mathcal{B}$ converge uniformément vers $f$ dans toute partie compacte de $X$, d’où le corollaire.

En particulier, la fonction $f$ est intégrable, et son intégrale $\int f \, d\mu$ est la limite suivant $\mathcal{B}$ des intégrales $\int h f \, d\mu$.

Nous retrouverons le cor. de la prop. 13 comme conséquence d’un critère général d’intégrabilité au § 5, n° 6.

Avec les notations du chap. III, § 1, n° 2, on a $|f| \leq \|f\| . 1$ pour toute fonction $f \in \mathcal{C}^b(X; F)$, d’où, en vertu des formules (3) et (4) du n° 2,

(19)
$$
N_p(f) \leq \|f\| \cdot N_p(1) = \|f\| \cdot \|\mu\|^{1/p}.
$$

En particulier, pour $p = 1$, la formule (5) du n° 2 donne

(20)
$$
|\int f d\mu| \leq \|f\| \cdot \|\mu\|
$$

et par suite l’application $f \mapsto \int f d\mu$ est continue dans l’espace de Banach $C^b(X; F)$; sa restriction à l’adhérence $C^0(X; F)$ de $\mathcal{K}(X; F)$ dans $C^b(X; F)$, espace des fonctions continues tendant vers 0 au point à l’infini (chap. III, § 1, n° 2, prop. 3), est donc le prolongement par continuité de l’intégrale à $C^0(X; F)$.

### 8. Intégration par rapport à une mesure à support compact

Soit $\mu$ une mesure sur $X$ dont le support $S = \mathrm{Supp}(\mu)$ est compact ; l’ensemble ouvert $X - S$ est négligeable (§ 2, n° 5, prop. 2). Pour toute fonction $f$ à valeurs dans un espace vectoriel $F$ ou dans $\bar{\mathbf{R}}$, les fonctions $f$ et $f \varphi_S$ sont donc équivalentes (§ 2, n° 4) ; pour que $f$ soit $\mu$-intégrable (lorsque $F$ est un espace de Banach), il faut et il suffit donc que $f \varphi_S$ le soit, et l’on a (n° 1)

(21)
$$
\int f d\mu = \int f \varphi_S d\mu.
$$

Si de plus $f$ est bornée dans $S$, il résulte de (20) que l’on a

(22)
$$
|\int f d\mu| \leq \|\mu\| \cdot \sup_{x \in S} |f(x)|.
$$

En particulier si $f$ est continue dans $X$, $f$ est $\mu$-intégrable puisque $fh \in \mathcal{K}(X; F)$ pour toute fonction $h \in \mathcal{K}(X; \mathbf{R})$ égale à 1 dans $S$ (chap. III, § 1, n° 2, lemme 1). Plus précisément :

#### Proposition 14 {#int-iv-s4-prop-14 .statement}

Soient $X$ un espace localement compact, $F$ un espace de Banach non réduit à 0 ; on munit l’espace $C(X; F)$ de toutes les applications continues de $X$ dans $F$ de la topologie de la convergence compacte. Pour qu’une mesure $\mu$ sur $X$ soit telle que l’application linéaire $f \mapsto \int f d\mu$ de $\mathcal{K}(X; F)$ dans $X$ se prolonge en une application linéaire continue de $C(X; F)$ dans $F$, il faut et il suffit que $\mathrm{Supp}(\mu)$ soit compact ; un tel prolongement est unique et coïncide avec l’intégrale définie au n° 1.

On vient de voir en effet que si $\mu$ a un support compact, l’intégrale $\int f d\mu$ est définie pour toute fonction $f \in C(X; F)$ et que l’application $f \mapsto \int f d\mu$ de $C(X; F)$ dans $F$ est continue pour la topologie de la convergence compacte. Inversement, supposons que $f \mapsto \int f\, d\mu$ soit continue *dans* $\mathcal{K}(X; F)$ pour la topologie de la convergence compacte. Il y a alors un ensemble compact $K \subset X$ et un nombre $a > 0$ tels que $|\mu(f)| \leq a \cdot \sup_{x \in K} |f(x)|$ pour toute fonction $f \in \mathcal{K}(X; F)$; en particulier, si le support de $g \in \mathcal{K}(X; F)$ ne rencontre pas $K$, on a $\mu(g) = 0$. Prenant $g = h a$, où $a \neq 0$ est un vecteur de $F$ et $h \in \mathcal{K}(X; C)$, on voit que $\mu(h) = 0$ pour toute fonction $h \in \mathcal{K}(X; C)$ dont le support ne rencontre pas $K$, ce qui prouve que $\operatorname{Supp}(\mu) \subset K$. Enfin, l’unicité du prolongement résulte de ce que $\mathcal{K}(X; F)$ est *dense* dans $\mathcal{C}(X; F)$ pour la topologie de la convergence compacte (chap. III, § 1, no 2, prop. 4).

La prop. 14 permet d’identifier une mesure à support compact sur $X$ à son prolongement continu à $\mathcal{C}(X; C)$. L’ensemble des mesures à support compact sur $X$ s’identifie donc au *dual* $\mathcal{C}'(X; C)$ de l’espace localement convexe séparé $\mathcal{C}(X; C)$. Rappelons que $\mathcal{C}(X; C)$ est *complet* (*Top. gén.*, chap. X, 2e éd., § 1, no 6, cor. 3 du th. 2); mais il n’est pas nécessairement tonnelé (exerc. 17). Toutefois, si $X$ est *dénombrable à l’infini*, donc réunion d’une suite croissante d’ensembles compacts $K_n$ tels que $K_n \subset \dot{K}_{n+1}$, alors la topologie de $\mathcal{C}(X; C)$ peut être définie par la famille dénombrable de semi-normes $p_n(f) = \sup_{x \in K_n} |f(x)|$, donc $\mathcal{C}(X; C)$ est un *espace de Fréchet* dans ce cas. Par suite, pour tout recouvrement $\mathfrak{S}$ de $\mathcal{C}(X; C)$ par des ensembles bornés, l’espace $\mathcal{C}'(X; C)$ est alors *quasi-complet* pour la $\mathfrak{S}$-topologie (*Esp. vect. top.*, chap. III, § 3, no 7, cor. 2 du th. 4).

Nous considérerons surtout sur $\mathcal{C}'(X; C)$ la topologie de la *convergence compacte* (topologie de la convergence uniforme dans les parties compactes de $\mathcal{C}(X; C)$). Rappelons que les parties relativement compactes $H$ de $\mathcal{C}(X; C)$ sont caractérisées par les propriétés suivantes (*Top. gén.*, chap. X, 2e éd., § 2, no 5, cor. 3 du th. 2):
1° $H$ est équicontinue ;
2° pour tout $x \in X$, l’ensemble $H(x)$ des $f(x)$, où $f$ parcourt $H$, est borné dans $C$.

#### Proposition 15 {#int-iv-s4-prop-15 .statement}

*Soient* $X$ *un espace localement compact et, pour tout* $x \in X$, *soit* $\varepsilon_x$ *la mesure de Dirac au point* $x$. *L’application* $x \mapsto \varepsilon_x$ *de* $X$ *dans* $\mathcal{C}'(X; C)$ *est continue pour la topologie de la convergence compacte sur* $\mathcal{C}'(X; C)$.

Considérons un voisinage de $\varepsilon_{x_0}$ dans $\mathcal{C}'(X; C)$ pour cette topologie, que l’on peut supposer défini en prenant un nombre δ > 0, une partie compacte H de $\mathcal{C}(X; \mathbf{C})$ et en considérant l’ensemble des mesures $\mu$ sur X telles que $|\mu(f) - \varepsilon_{x_0}(f)| \leq \delta$ pour toute fonction $f \in H$. Comme H est équicontinue, il existe un voisinage U de $x_0$ dans X tel que la relation $f \in H$ entraîne $|f(x) - f(x_0)| \leq \delta$ pour tout $x \in U$, ce qui s’écrit aussi

$$
|\varepsilon_x(f) - \varepsilon_{x_0}(f)| \leq \delta,
$$

et prouve la proposition.

#### Proposition 16 {#int-iv-s4-prop-16 .statement}

*Soient K une partie compacte de X, L l’espace vectoriel des mesures $\mu$ sur X de support contenu dans K. Sur L, les topologies induites par la topologie $\mathcal{T}$ de la convergence compacte sur $\mathcal{C}'(X; \mathbf{C})$ et la topologie $\mathcal{T}'$ de la convergence strictement compacte sur $\mathcal{M}(X; \mathbf{C})$ (chap. III, § 1, n° 10) coïncident.*

Il est clair que sur L, la topologie induite par $\mathcal{T}$ est plus fine que la topologie induite par $\mathcal{T}'$. Inversement, soient H une partie compacte de $\mathcal{C}(X; \mathbf{C})$, h une fonction de $\mathcal{K}(X; \mathbf{C})$ égale à 1 dans K. Il est clair que l’ensemble H’ des fonctions $fh$, où $f$ parcourt H, est strictement compact dans $\mathcal{K}(X; \mathbf{C})$, et, pour toute mesure $\mu \in L$, on a $\mu(f) = \mu(fh)$ pour toute fonction $f \in H$, d’où la conclusion.

#### Corollaire 1 {#int-iv-s4-prop-16-cor-1 .statement}

*Pour toute partie compacte K de X et tout nombre $a > 0$, l’ensemble B des mesures $\mu$ sur X telles que $\mathrm{Supp}(\mu) \subset K$ et $\| \mu \| \leq a$ est une partie équicontinue de $\mathcal{C}'(X; \mathbf{C})$, qui est compacte pour la topologie $\mathcal{T}$ de la convergence compacte.*

En effet, soit H une partie de $\mathcal{C}(X; \mathbf{C})$, formée de fonctions uniformément bornées dans K ; il existe un nombre $c > 0$ tel que $|\mu(f)| \leq c.\| \mu \| \leq ac$ pour toute fonction $f \in H$ et toute mesure $\mu \in B$, en vertu de (22) ; on a donc $B \subset acH^0$ dans le dual $\mathcal{C}'(X; \mathbf{C})$ de $\mathcal{C}(X; \mathbf{C})$, ce qui prouve l’équicontinuité de B ; le fait que B est compact pour $\mathcal{T}$ résulte de ce que, sur B, $\mathcal{T}$ et la topologie vague induisent la même topologie (prop. 16 et chap. III, § 1, n° 10, prop. 17) et du fait que B est vaguement compact (chap. III, § 1, n° 9, cor. 2 de la prop. 15 et § 2, n° 2, prop. 6).

#### Corollaire 2 {#int-iv-s4-prop-16-cor-2 .statement}

*Toute mesure à support compact (resp. positive à support compact) $\mu$ est adhérente dans $\mathcal{C}'(X; \mathbf{C})$, pour la topologie $\mathcal{T}$ de la convergence compacte, à l’ensemble des mesures (resp. des mesures positives) dont le support est fini et contenu dans $\mathrm{Supp}(\mu)$ et dont la norme est égale à $\| \mu \|$.*

En effet, sur l’ensemble B des mesures $\nu$ telles que
$$
\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu) \quad \text{et} \quad \| \nu \| \leq \| \mu \|,
$$
la topologie induite par la topologie vague est identique à la topologie induite par $\mathcal{T}$, et le corollaire résulte donc du chap. III, § 2, n° 4, cor. 2 et 3 du th. 1.

### 9. Clans et fonctions additives d’ensemble

#### Définition 3 {#int-iv-s4-def-3 .statement}

On dit qu’un ensemble non vide $\Phi$ de parties d’un ensemble A est un clan s’il existe une algèbre $\mathcal{A}$ (sur $\mathbf{R}$) formée de fonctions numériques finies, définies dans A, telle que les relations $M \in \Phi$ et $\varphi_M \in \mathcal{A}$ soient équivalentes.

#### Exemple {#int-iv-s4-n9-exa-1 .statement}

Si $\mu$ est une mesure sur un espace localement compact X, les combinaisons linéaires à coefficients réels de fonctions caractéristiques d’ensembles intégrables forment une algèbre $\mathcal{A}$, car pour deux ensembles intégrables M, N,
$$
\varphi_M \varphi_N = \varphi_{M \cap N}
$$
est intégrable (n° 5, prop. 7); il résulte alors des déf. 2 et 3 que l’ensemble des parties intégrables de X est un clan.

#### Proposition 17 {#int-iv-s4-prop-17 .statement}

Pour qu’un ensemble non vide $\Phi$ de parties d’un ensemble A soit un clan, il faut et il suffit qu’il satisfasse à la condition suivante:
(CL) Pour tout couple d’ensembles M, N appartenant à $\Phi$, les ensembles $M \cup N$ et $M \cap \mathbf{C} N$ appartiennent à $\Phi$.

La condition est nécessaire, en vertu des relations
$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N, \qquad \varphi_{M \cap \mathbf{C} N} = \varphi_M - \varphi_M \varphi_N.
$$

Pour montrer qu’elle est suffisante, remarquons d’abord qu’elle entraîne que, pour deux ensembles quelconques M, N de $\Phi$, $M \cap N$ appartient à $\Phi$, puisque $M \cap N = M \cap (\mathbf{C}(M \cap \mathbf{C} N))$. Soit alors $\mathcal{E}(\Phi)$ l’ensemble des combinaisons linéaires à coefficients réels de fonctions caractéristiques d’ensembles de $\Phi$. Comme $\varphi_M \varphi_N = \varphi_{M \cap N}$, $\mathcal{E}(\Phi)$ est une algèbre. Tout revient à montrer que, si M est une partie de A telle que $\varphi_M = \sum_i c_i \varphi_{M_i}$, où les $M_i \in \Phi$, on a $M \in \Phi$.

Cela va résulter du lemme suivant:

#### Lemme 1 {#int-iv-s4-lem-1 .statement}

Soit $\Phi$ un ensemble non vide de parties de A satisfaisant à l’axiome (CL). Etant donnée une famille finie $(M_i)_{1 \leq i \leq n}$ d’ensembles de $\Phi$, il existe une famille finie $(N_j)_{1 \leq j \leq m}$ d’ensembles de $\Phi$, deux à deux sans point commun, telle que chacun des $M_i$ soit réunion d’un certain nombre des $N_j$.

En effet, considérons les $2^n - 1$ ensembles de la forme $\bigcap_{i=1}^n P_i$, où $P_i = M_i$ pour certains indices $i$, $P_i = \bigcup M_i$ pour les autres, un au moins des $P_i$ étant égal à $M_i$. Soit $(N_j)_{1 \leq j \leq m}$ la suite de ces ensembles rangés dans un certain ordre ; ils sont deux à deux sans point commun, et appartiennent à $\Phi$; d’autre part, tout ensemble $M_k$ est réunion des ensembles $N_j = \bigcap_{i=1}^n P_i$ correspondant aux familles $(P_i)$ telles que $P_k = M_k$, ce qui démontre le lemme.

Ce lemme étant établi, toute fonction de la forme $\sum_{i=1}^n c_i \varphi_{M_i}$, où $M_i \in \Phi$, peut s’écrire sous la forme $\sum_{j=1}^m d_j \varphi_{N_j}$, où les $N_j$ appartiennent à $\Phi$ et sont deux à deux sans point commun; si $\varphi_M = \sum_{j=1}^m d_j \varphi_{N_j}$, on a nécessairement $d_j = 0$ ou $d_j = 1$ pour chaque indice $j$, donc $M$ est réunion d’un certain nombre des $N_j$, et par suite appartient à $\Phi$.

Tout clan $\Phi$ de parties de $A$ contient la partie vide $\emptyset$ de $A$; en effet, il existe au moins une partie $M \in \Phi$, donc $M - M = \emptyset$ appartient à $\Phi$. On notera d’ailleurs que l’ensemble de parties de $A$ réduit à la seule partie $\emptyset$ est un clan.

#### Définition 4 {#int-iv-s4-def-4 .statement}

Etant donné un clan $\Phi$ de parties d’un ensemble $A$, et un espace de Banach $F$, on appelle fonction étagée sur les ensembles de $\Phi$ (ou fonction $\Phi$-étagée), à valeurs dans $F$, toute fonction de la forme $\sum_i a_i \varphi_{M_i}$, où les $a_i$ appartiennent à $F$, et les $M_i$ à $\Phi$.

Il est clair que l’ensemble $\mathscr{E}_F(\Phi)$ des fonctions $\Phi$-étagées à valeurs dans $F$, est un espace vectoriel sur $\mathbf{R}$ ou $\mathbf{C}$. Nous venons de voir dans la prop. 17 que l’ensemble $\mathscr{E}(\Phi)$ des fonctions numériques finies $\Phi$-étagées est une algèbre sur $\mathbf{R}$; c’est aussi le sous-espace vectoriel de $\mathbf{R}^A$ engendré par les fonctions caractéristiques des ensembles de $\Phi$.

Toute fonction de $\mathcal{E}_F(\Phi)$ peut s’écrire $f = \sum_j c_j \varphi_{N_j}$, où les $N_j \in \Phi$ sont deux à deux sans point commun, en raison du lemme 1 ; on en déduit que $|f| = \sum_j |c_j| \varphi_{N_j}$ appartient à $\mathcal{E}(\Phi)$. En particulier, $\mathcal{E}(\Phi)$ est un espace de Riesz, l’enveloppe supérieure de deux fonctions de $\mathcal{E}(\Phi)$ appartenant à $\mathcal{E}(\Phi)$.

#### Remarque {#int-iv-s4-n9-rem-1 .statement}

On voit aisément que la déf. 4 est équivalente à la suivante : une fonction $\Phi$-étagée à valeurs dans $F$ est une fonction $f$ qui ne prend qu’un nombre fini de valeurs et qui est telle que, pour tout $a \neq 0$ dans $F$, l’ensemble $\overline{f(a)}$ appartienne à $\Phi$.

#### Définition 5 {#int-iv-s4-def-5 .statement}

On dit qu’une fonction numérique finie $\lambda$, définie dans un clan $\Phi$ de parties d’un ensemble $A$, est additive, si, pour tout couple d’ensembles $M, N$ sans point commun et appartenant à $\Phi$, on a $\lambda(M \cup N) = \lambda(M) + \lambda(N)$.

Il résulte en particulier de cette définition que $\lambda(\emptyset) = 0$.

#### Proposition 18 {#int-iv-s4-prop-18 .statement}

Soit $\lambda$ une fonction additive d’ensemble, définie dans un clan $\Phi$. Il existe une forme linéaire et une seule (notée encore $\lambda$) sur l’espace vectoriel $\mathcal{E}(\Phi)$ des fonctions $\Phi$-étagées numériques finies, telle que $\lambda(\varphi_M) = \lambda(M)$ pour tout ensemble $M \in \Phi$; en outre, si $\lambda(M) \geq 0$ pour tout $M \in \Phi$, $\lambda$ est une forme linéaire positive sur $\mathcal{E}(\Phi)$.

L’unicité de la forme linéaire $\lambda$ est évidente, puisque les fonctions caractéristiques d’ensembles de $\Phi$ engendrent l’espace vectoriel $\mathcal{E}(\Phi)$. Pour prouver l’existence de $\lambda$, il suffit de prouver que la relation $\sum_i c_i \varphi_{M_i} = 0$, où les $M_i$ sont des ensembles non vides appartenant à $\Phi$, entraîne $\sum_i c_i \lambda(M_i) = 0$. Or, en vertu du lemme 1, il existe une famille finie $(N_j)$ d’ensembles non vides de $\Phi$, deux à deux sans point commun, telle que pour chaque indice $i$, on ait $\varphi_{M_i} = \sum_j a_{ij} \varphi_{N_j}$, avec $a_{ij} = 0$ ou $a_{ij} = 1$. La relation $\sum_i c_i \varphi_{M_i} = 0$, qui s’écrit $\sum_j \left( \sum_i c_i a_{ij} \right) \varphi_{N_j} = 0$, entraîne donc $\sum_i c_i a_{ij} = 0$ pour tout indice $j$. En vertu de la déf. 5, on a alors

$$
\sum_i c_i \lambda(M_i) = \sum_j \left( \sum_i c_i a_{ij} \right) \lambda(N_j) = 0,
$$

ce qui démontre l’existence de $\lambda$. Supposons enfin que $\lambda(M) \geq 0$ pour tout $M \in \Phi$; pour toute fonction $f \in \mathcal{E}(\Phi)$, on peut écrire $f = \sum_i c_i \varphi_{M_i}$, où les $M_i \in \Phi$ sont deux à deux sans point commun; si $f \geqslant 0$, on a donc $c_i \geqslant 0$ pour tout indice $i$ tel que $M_i$ soit non vide, d’où $\lambda(f) = \sum_i c_i \lambda(M_i) \geqslant 0$.

### 10. Approximation des fonctions continues par les fonctions étagées

#### Proposition 19 {#int-iv-s4-prop-19 .statement}

*Soient X un espace localement compact, $\Phi$ un clan de parties de X, contenant l’ensemble des parties compactes de X. Pour toute application continue $f$ de X dans un espace de Banach F (resp. toute fonction numérique $f$ finie, continue et $\geqslant 0$ dans X), à support compact K, il existe une suite $(g_n)$ de fonctions de $\mathcal{E}_F(\Phi)$, dont le support est contenu dans K (resp. une suite $(g_n)$ de fonctions de $\mathcal{E}(\Phi)$, telle que $0 \leqslant g_n \leqslant f$ pour tout n), qui converge uniformément vers $f$ (resp. $f$).

En effet, comme $f$ est uniformément continue dans K, on peut recouvrir K par un nombre fini d’ensembles compacts $M_i$ ($1 \leqslant i \leqslant m$) tels que l’oscillation de $f$ dans chacun des $M_i$ soit $\leqslant 1/n$. Comme les $M_i$ et K appartiennent à $\Phi$, il existe une partition de K en ensembles $N_j \in \Phi$ tels que chacun des ensembles $M_i \cap K$ soit réunion d’un certain nombre des $N_j$ (n° 9, lemme 1). Soit $a_j$ un élément de F tel que $|f(x) - a_j| \leqslant 1/n$ dans $N_j$. Si on pose $g_n = \sum_j a_j \varphi_{N_j}$, on a $|f - g_n| \leqslant 1/n$, d’où la proposition dans ce cas. On raisonne de même pour une fonction continue numérique $f$, en prenant $a_j = \inf_{x \in N_j} f(x)$, et $g_n = \sum_j a_j \varphi_{N_j}$.

#### Corollaire 1 {#int-iv-s4-prop-19-cor-1 .statement}

*Soit $\mu$ une mesure positive sur X; l’espace $\mathcal{E}_F(\Phi)$ est partout dense dans chacun des espaces $\mathcal{L}_F^p$ ($1 \leqslant p < +\infty$).

En effet, il résulte de la prop. 19 et du critère de convergence en moyenne pour les limites uniformes de fonctions à support compact ($§ 3$, n° 3, prop. 4) que $\mathcal{E}_F(\Phi)$ est dense, pour la topologie de la convergence en moyenne d’ordre $p$, dans l’adhérence de l’espace $\mathcal{K}_F$ des fonctions continues à support compact; d’où le corollaire.

#### Corollaire 2 {#int-iv-s4-prop-19-cor-2 .statement}

*Pour toute partie fermée S de X, toute fonction $f \in \mathcal{K}(X, S; \mathbf{C})$ est limite uniforme de combinaisons linéaires $\sum_i \lambda_i \varphi_{K_i}$, où les $\lambda_i$ appartiennent à $\mathbf{C}$ et les $K_i$ sont des parties compactes de S.*

En effet, l’ensemble $\mathcal{A}$ des combinaisons linéaires considérées est une $\mathbf{C}$-algèbre. Soit $\Phi$ l’ensemble des parties $M$ de $X$ telles que $\varphi_M \in \mathcal{A}$; $\Phi$ est donc un *clan* dont tous les éléments sont des parties de $S$, contenant les parties compactes de $S$, et l’on a $\mathcal{E}_c(\Phi) \subset \mathcal{A}$. Il suffit alors d’appliquer la prop. 19 à l’espace localement compact $S$ et au clan $\Phi$.

#### Corollaire 3 {#int-iv-s4-prop-19-cor-3 .statement}

*Si $\mu$ et $\nu$ sont deux mesures sur $X$ telles que $\mu(K) = \nu(K)$ pour toute partie compacte $K$ de $X$, on a $\mu = \nu$.*
En effet, il résulte du cor. 2 et de la définition d’une mesure que pour toute partie compacte $S$ de $X$, $\mu$ et $\nu$ prennent les mêmes valeurs dans $\mathscr{K}(X, S ; \mathbf{C})$.

### 11. Prolongement d’une mesure définie sur une famille d’ensembles

Soit $\Phi$ un ensemble non vide de parties d’un espace localement compact $X$. Etant donnée une fonction numérique finie $M \mapsto \alpha(M)$, définie et $\geqslant 0$ dans $\Phi$, nous nous proposons de chercher à quelles conditions il existe une mesure positive $\mu$ sur $X$ telle que les ensembles de $\Phi$ soient $\mu$-intégrables et que l’on ait $\mu(M) = \alpha(M)$ pour tout $M \in \Phi$. Nous nous bornerons à considérer le cas où l’ensemble $\Phi$ satisfait aux conditions suivantes :
*(PC$_1$)* *La réunion et l’intersection de deux ensembles de $\Phi$ appartiennent à $\Phi$.*
*(PC$_2$)* *Pour tout couple formé d’un ensemble compact $K$ et d’un ensemble ouvert $U$ dans $X$, tels que $K \subset U$, il existe un ensemble $M \in \Phi$ tel que $K \subset M \subset U$.*

On notera que la condition (PC$_2$) implique que $\emptyset \in \Phi$, en prenant $K = U = \emptyset$. Mais l’ensemble $\Phi$ n’est pas nécessairement un clan : par exemple, l’ensemble des parties compactes de $X$ vérifie les conditions (PC$_1$) et (PC$_2$), mais n’est pas un clan en général, car si $M$ et $N$ sont compacts, il n’en est pas de même de $M \cap C N$ en général.

Nous supposerons en outre que la fonction $\alpha$, définie dans $\Phi$, vérifie les conditions suivantes (évidemment nécessaires pour que le problème ait une solution) :

*(PM$_1$)* *La relation $M \subset N$ entraîne $\alpha(M) \leqslant \alpha(N)$.*
*(PM$_2$)* *Quels que soient $M$ et $N$ dans $\Phi$, $\alpha(M \cup N) \leqslant \alpha(M) + \alpha(N)$.*
*(PM$_3$)* *La relation $M \cap N = \emptyset$ entraîne $\alpha(M \cup N) = \alpha(M) + \alpha(N)$.*

En prenant $N = \emptyset$ dans la condition (PM$_3$), on en déduit que $\alpha(\emptyset) = 0$; la condition (PM$_1$) montre alors que $\alpha(M) \geqslant 0$ pour tout $M \in \Phi$.

#### Théorème 5 {#int-iv-s4-thm-5 .statement}

Soit $\Phi$ un ensemble de parties d’un espace localement compact $X$, satisfaisant à $(\mathrm{PC}_I)$ et $(\mathrm{PC}_{II})$, et soit $\alpha$ une fonction numérique finie, définie dans $\Phi$, satisfaisant aux conditions $(\mathrm{PM}_I)$, $(\mathrm{PM}_{II})$ et $(\mathrm{PM}_{III})$. Pour qu’il existe une mesure positive $\mu$ sur $X$, telle que les ensembles de $\Phi$ soient $\mu$-intégrables et que l’on ait $\mu(M) = \alpha(M)$ pour tout $M \in \Phi$, il faut et il suffit que $\alpha$ vérifie en outre la condition suivante :

$(\mathrm{PM}_{IV})$ Pour tout $\varepsilon > 0$ et tout $M \in \Phi$, il existe un ensemble compact $K \subset M$ et un ensemble ouvert $U \supset M$, tels que, pour tout ensemble $N \in \Phi$ satisfaisant à la relation $K \subset N \subset U$, on ait $|\alpha(N) - \alpha(M)| \leq \varepsilon$.

En outre, si la condition $(\mathrm{PM}_{IV})$ est remplie, la mesure $\mu$ est unique ; pour tout ensemble compact $K$, on a $\mu(K) = \inf_{M \in \Phi, M \supseteq K} \alpha(M)$; pour tout ensemble ouvert $U$, on a $\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$.

On notera que la condition $(\mathrm{PM}_{IV})$ est équivalente à la conjonction des deux suivantes :

$(\mathrm{PM}'_{IV})$ Pour tout $\varepsilon > 0$ et tout $M \in \Phi$, il existe un ensemble ouvert $U \supset M$ tel que, pour tout $N \in \Phi$ contenu dans $U$, on ait $\alpha(N) \leq \alpha(M) + \varepsilon$.

$(\mathrm{PM}''_{IV})$ Pour tout $\varepsilon > 0$ et tout $M \in \Phi$, il existe un ensemble compact $K \subset M$ tel que, pour tout $N \in \Phi$ contenant $K$, on ait $\alpha(N) \geq \alpha(M) - \varepsilon$.

En effet, il est évident que $(\mathrm{PM}'_{IV})$ et $(\mathrm{PM}''_{IV})$ entraînent $(\mathrm{PM}_{IV})$. Inversement, montrons par exemple que $(\mathrm{PM}_{IV})$ entraîne $(\mathrm{PM}'_{IV})$ : soient $K$ un ensemble compact, $U$ un ensemble ouvert, tels que $K \subset M \subset U$ et que $|\alpha(P) - \alpha(M)| \leq \varepsilon$ pour tout $P \in \Phi$ tel que $K \subset P \subset U$. Alors, si $N \in \Phi$ et $N \subset U$, $M \cup N$ appartient à $\Phi$ et

$$
K \subset (M \cup N) \subset U,
$$

d’où $\alpha(M \cup N) \leq \alpha(M) + \varepsilon$, et *a fortiori* $\alpha(N) \leq \alpha(M) + \varepsilon$.

Lorsque l’ensemble $\Phi$, satisfaisant à $(\mathrm{PC}_I)$ et $(\mathrm{PC}_{II})$, est formé d’ensembles *compacts*, la condition $(\mathrm{PM}''_{IV})$ est vérifiée d’elle-même, et $(\mathrm{PM}_{IV})$ est alors équivalente à $(\mathrm{PM}'_{IV})$.

La condition $(\mathrm{PM}_{IV})$ est *nécessaire* : cela résulte aussitôt du th. 4 du n° 6 sur l’« approximation » d’un ensemble intégrable par un ensemble compact et un ensemble ouvert. Pour démontrer les autres assertions du théorème nous procéderons en plusieurs étapes.

1° Définition d’une topologie sur $\mathfrak{P}(X)$.

Pour tout couple $(K, U)$ formé d’un ensemble compact $K$ et d’un ensemble ouvert $U$ dans $X$, désignons par $I(K, U)$ l’ensemble des parties $M \subset X$ telles que $K \subset M \subset U$; pour que $I(K, U)$ ne soit pas vide, il faut et il suffit que $K \subset U$. Si $(K', U')$ est un second couple formé d’un ensemble compact $K'$ et d’un ensemble ouvert $U'$, on a

$$
I(K, U) \cap I(K', U') = I(K \cup K', U \cap U').
$$

Soit $\mathcal{T}$ la topologie sur $\mathfrak{P}(X)$ engendrée par l’ensemble des parties $I(K, U)$ lorsque $K$ parcourt l’ensemble des parties compactes de $X$, et $U$ l’ensemble des parties ouvertes de $X$; d’après ce qui précède, les $I(K, U)$ forment une base de la topologie $\mathcal{T}$ (*Top. gén.*, chap. I, 3e éd., § 1, n° 3).

On notera que la définition de $\mathcal{T}$ entraîne que, dans $\mathfrak{P}(X)$, l’ensemble des parties compactes de $X$ est *partout dense*. La condition (PC$_{\text{II}}$) exprime que $\Phi$ est *dense* dans $\mathfrak{P}(X)$, et la condition (PM$_{\text{IV}}$) exprime que la fonction $\alpha$ est *continue* dans $\Phi$, pour la topologie induite par $\mathcal{T}$. Enfin, le th. 4 exprime que la fonction $M \mapsto \mu(M)$ est *continue* dans le clan des ensembles $\mu$-intégrables, pour la topologie induite par $\mathcal{T}$.

*2° Unicité de $\mu$*

Désignons par $\bar{\Phi}$ l’ensemble des parties $M \subset X$ telles que $\alpha(N)$ tende vers une limite finie lorsque $N$ tend vers $M$ (pour la topologie $\mathcal{T}$) en restant dans $\Phi$; on peut alors prolonger d’une seule manière $\alpha$ en une application *continue* $\bar{\alpha}$ de $\bar{\Phi}$ dans $\mathbf{R}$ (*Top. gén.*, chap. I, 3e éd., § 8, n° 5, th. 1). S’il existe une mesure $\mu$ répondant à la question, les remarques faites ci-dessus prouvent que le clan $\Psi$ des ensembles $\mu$-intégrables est contenu dans $\bar{\Phi}$, et que $\mu(M) = \bar{\alpha}(M)$ pour tout $M \in \Psi$; cette relation a lieu en particulier pour toute partie compacte $M$ de $X$, ce qui prouve l’unicité de $\mu$ (cor. 2 de la prop. 19).

*3° Prolongement de $\alpha$ aux ensembles compacts.*

Sans supposer l’existence de $\mu$, nous allons maintenant étudier l’ensemble $\bar{\Phi}$ et le prolongement $\bar{\alpha}$ de $\alpha$ à $\bar{\Phi}$. Montrons en premier lieu que tout ensemble compact $K$ appartient à $\bar{\Phi}$, et que l’on a $\bar{\alpha}(K) = \inf_{P \in \Phi, P \supset K} \alpha(P)$. Posons $a = \inf_{P \in \Phi, P \supset K} \alpha(P)$; pour tout $\varepsilon > 0$, il existe $M \in \Phi$ tel que $K \subset M$ et $\alpha(M) \leq a + \varepsilon$. D’après (PM$_{\text{IV}}$), il existe un ensemble ouvert $U \supset M$ tel que, pour tout $N \in \Phi$ contenu dans $U$, on ait $\alpha(N) \leq \alpha(M) + \varepsilon \leq a + 2\varepsilon$; pour tout $N \in \Phi$ tel que $K \subset N \subset U$, on a donc $a \leq \alpha(N) \leq a + 2\varepsilon$, ce qui, en vertu des définitions, montre que $K \in \bar{\Phi}$ et $\bar{\alpha}(K) = a$.

Ce résultat prouve aussitôt que si $K_1$ et $K_2$ sont deux ensembles compacts tels que $K_1 \subset K_2$, on a $\bar{\alpha}(K_1) \leq \bar{\alpha}(K_2)$. Si $K_1$ et $K_2$ sont deux ensembles compacts quelconques, on a $\bar{\alpha}(K_1 \cup K_2) \leq \bar{\alpha}(K_1) + \bar{\alpha}(K_2)$ d’après (PM$_{\text{II}}$). Nous allons voir en outre que si $K_1$ et $K_2$ ne se rencontrent pas, on a $\bar{\alpha}(K_1 \cup K_2) = \bar{\alpha}(K_1) + \bar{\alpha}(K_2)$. En effet, il existe alors deux ensembles ouverts sans point commun $U_1, U_2$ tels que $K_1 \subset U_1, K_2 \subset U_2$ (*Top. gén.*, chap. II, 3e éd., § 4, prop. 4). Il existe donc aussi, d’après (PC$_{\text{II}}$), deux ensembles $M_1 \in \Phi, M_2 \in \Phi$, tels que $K_1 \subset M_1 \subset U_1$ et $K_2 \subset M_2 \subset U_2$. Soit alors $P$ un ensemble quelconque de $\Phi$ contenant $K_1 \cup K_2$; la réunion des deux ensembles $P \cap M_1$ et $P \cap M_2$ appartient à $\Phi$ d’après (PC$_{\text{I}}$), et comme ces deux ensembles ne se rencontrent pas, on a, en appliquant (PM$_{\text{I}}$) et (PM$_{\text{III}}$),

$$
\alpha(P) \geq \alpha(P \cap M_1) + \alpha(P \cap M_2) \geq \bar{\alpha}(K_1) + \bar{\alpha}(K_2),
$$

ce qui établit notre assertion.

*4° Prolongement de $\alpha$ aux ensembles ouverts.*

Nous allons voir maintenant que, pour qu’un ensemble ouvert U appartenne à $\bar{\Phi}$, il faut et il suffit que, lorsque K parcourt l’ensemble des parties compactes de U, la borne supérieure des nombres $\bar{\alpha}(K)$ soit finie ; en outre, $\bar{\alpha}(U)$ est alors égal à cette borne supérieure.

En effet, soit U un ensemble ouvert appartenant à $\bar{\Phi}$; pour tout $\varepsilon > 0$ il existe un ensemble compact $K \subset U$ tel que, pour tout ensemble $M \in \Phi$ vérifiant $K \subset M \subset U$, on ait $|\bar{\alpha}(U) - \alpha(M)| \leq \varepsilon$; d’où

$$
|\bar{\alpha}(U) - \bar{\alpha}(K)| \leq \varepsilon;
$$

d’autre part, si $K'$ est un ensemble compact quelconque contenu dans U, on a $K \subset K \cup K' \subset U$, d’où $|\bar{\alpha}(U) - \bar{\alpha}(K \cup K')| \leq \varepsilon$ et par suite $\bar{\alpha}(U) \geq \bar{\alpha}(K \cup K') - \varepsilon \geq \bar{\alpha}(K') - \varepsilon$; $\bar{\alpha}(U)$ est donc bien égal à la borne supérieure des nombres $\bar{\alpha}(K)$ lorsque K parcourt l’ensemble des parties compactes de U.

Inversement, soit U un ensemble ouvert tel que $b = \sup_{K \subset U} \bar{\alpha}(K) < +\infty$ (K parcourant l’ensemble des parties compactes de U), et montrons que $U \in \bar{\Phi}$. Pour tout $\varepsilon > 0$, il existe un ensemble compact $K \subset U$ tel que $b - \varepsilon \leq \bar{\alpha}(K) \leq b$; d’après (PM$_{IV}$), pour tout ensemble $M \in \Phi$ tel que

$$
K \subset M \subset U,
$$

il existe un ensemble compact $K' \subset M$ tel que

$$
\alpha(M) \leq \bar{\alpha}(K') + \varepsilon \leq b + \varepsilon;
$$

on a donc $b - \varepsilon \leq \alpha(M) \leq b + \varepsilon$, ce qui prouve que $U \in \bar{\Phi}$.

De cette caractérisation des ensembles ouverts $U \in \bar{\Phi}$, et de $\bar{\alpha}(U)$, il résulte d’abord que, si $U_1$ et $U_2$ sont deux ensembles ouverts tels que $U_1 \subset U_2$ et $U_2 \in \bar{\Phi}$, alors $U_1 \in \bar{\Phi}$ et $\bar{\alpha}(U_1) \leq \bar{\alpha}(U_2)$. D’autre part, si $U_1$ et $U_2$ sont deux ensembles ouverts appartenant à $\bar{\Phi}$, il en est de même de $U_1 \cup U_2$ et on a $\bar{\alpha}(U_1 \cup U_2) \leq \bar{\alpha}(U_1) + \bar{\alpha}(U_2)$. En effet, soit K un ensemble compact quelconque contenu dans $U_1 \cup U_2$; pour tout point $x \in K$, il existe un voisinage compact de x contenu dans $U_1$ ou dans $U_2$; on peut donc recouvrir K par un nombre fini de ces voisinages ; si $K_1$ (resp. $K_2$) est la réunion de ceux qui sont contenus dans $U_1$ (resp. $U_2$), on a $K \subset K_1 \cup K_2$, d’où

$$
\bar{\alpha}(K) \leq \bar{\alpha}(K_1 \cup K_2) \leq \bar{\alpha}(K_1) + \bar{\alpha}(K_2) \leq \bar{\alpha}(U_1) + \bar{\alpha}(U_2),
$$

ce qui établit la propriété annoncée.

**5° Propriétés de $\bar{\Phi}$ et de $\bar{\alpha}$.**

La définition de $\bar{\Phi}$ et de $\bar{\alpha}$ peut maintenant se transformer comme suit (compte tenu de (PC$_{II}$)) : pour que $M \in \bar{\Phi}$, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un ensemble compact K et un ensemble ouvert $U \in \bar{\Phi}$, tels que $K \subset M \subset U$ et $\bar{\alpha}(U) - \bar{\alpha}(K) \leq \varepsilon$; $\bar{\alpha}(M)$ est en outre la *borne inférieure* des $\bar{\alpha}(U)$ pour les ensembles ouverts $U \in \bar{\Phi}$ contenant M, et la *borne supérieure* des $\bar{\alpha}(K)$ pour les ensembles compacts $K \subset M$.

Nous allons déduire d’abord de là que, si $M_1$, $M_2$ et $M_1 \cup M_2$ appartiennent à $\bar{\Phi}$, on a $\bar{\alpha}(M_1 \cup M_2) \leq \bar{\alpha}(M_1) + \bar{\alpha}(M_2)$. En effet, si $U_1$ et

U_2 sont deux ensembles ouverts de $\bar{\Phi}$ contenant respectivement $M_1$ et $M_2$ et tels que $\bar{\alpha}(U_1) \leq \bar{\alpha}(M_1) + \varepsilon$ et $\bar{\alpha}(U_2) \leq \bar{\alpha}(M_2) + \varepsilon$, alors $U_1 \cup U_2$ appartient à $\bar{\Phi}$, contient $M_1 \cup M_2$, et par suite

$$
\bar{\alpha}(M_1 \cup M_2) \leq \bar{\alpha}(U_1 \cup U_2) \leq \bar{\alpha}(U_1) + \bar{\alpha}(U_2) \leq \bar{\alpha}(M_1) + \bar{\alpha}(M_2) + 2\varepsilon,
$$

d’où notre assertion.

Montrons ensuite que, si $K$ est un ensemble compact et $U$ un ensemble ouvert de $\bar{\Phi}$ tel que $K \subset U$, on a $\bar{\alpha}(U - K) = \bar{\alpha}(U) - \bar{\alpha}(K)$. D’après ce qui précède, on a $\bar{\alpha}(U) \leq \bar{\alpha}(K) + \bar{\alpha}(U - K)$. D’autre part, pour tout ensemble compact $K' \subset U - K$, on a

$$
\bar{\alpha}(K \cup K') = \bar{\alpha}(K) + \bar{\alpha}(K') \leq \bar{\alpha}(U);
$$

comme $U - K$ est ouvert et appartient à $\bar{\Phi}$, $\bar{\alpha}(U - K)$ est la borne supérieure des $\bar{\alpha}(K')$, ce qui montre que $\bar{\alpha}(K) + \bar{\alpha}(U - K) \leq \bar{\alpha}(U)$.

La définition de $\bar{\Phi}$ s’exprime donc encore de la façon suivante : pour que $M \in \bar{\Phi}$, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un ensemble compact $K$ et un ensemble ouvert $U \in \bar{\Phi}$ tels que $K \subset M \subset U$ et $\bar{\alpha}(U - K) \leq \varepsilon$.

Nous sommes maintenant en mesure de prouver que $\bar{\Phi}$ est un clan et $\bar{\alpha}$ une fonction additive d’ensemble dans $\bar{\Phi}$. En premier lieu, montrons que, si $M$ et $N$ appartiennent à $\bar{\Phi}$, il en est de même de $M \cap \mathbf{C}N$ et de $M \cup N$. Par hypothèse, pour tout $\varepsilon > 0$, il existe deux ensembles compacts $K, K'$ et deux ensembles ouverts, $U, U'$ de $\bar{\Phi}$ tels que $K \subset M \subset U, K' \subset N \subset U', \bar{\alpha}(U - K) \leq \varepsilon, \bar{\alpha}(U' - K') \leq \varepsilon$. L’ensemble $K'' = K \cap \mathbf{C}U'$ est compact, l’ensemble $U'' = U \cap \mathbf{C}K'$ est ouvert et appartient à $\bar{\Phi}$, et on a $K'' \subset M \cap \mathbf{C}N \subset U''$; d’autre part, $U'' - K''$ est contenu dans la réunion de $U \cap \mathbf{C}K$ et $U' \cap \mathbf{C}K'$, d’où $\bar{\alpha}(U'' - K'') \leq 2\varepsilon$, ce qui prouve que $M \cap \mathbf{C}N \in \bar{\Phi}$. De même, $U_1 = U \cup U'$ est ouvert et appartient à $\bar{\Phi}$, $K_1 = K \cup K'$ est compact, et on a $K_1 \subset M \cup N \subset U_1$; d’autre part, $U_1 - K_1$ est contenu dans la réunion de $U - K$ et de $U' - K'$, d’où encore $\bar{\alpha}(U_1 - K_1) \leq 2\varepsilon$, et $M \cup N$ appartient à $\bar{\Phi}$. Enfin, si $M$ et $N$ ne se rencontrent pas, on a

$$
\bar{\alpha}(K_1) = \bar{\alpha}(K) + \bar{\alpha}(K') \geq \bar{\alpha}(M) + \bar{\alpha}(N) - 2\varepsilon,
$$

et par suite $\bar{\alpha}(M \cup N) \geq \bar{\alpha}(M) + \bar{\alpha}(N) - 2\varepsilon$; comme $\varepsilon$ est arbitraire on a $\bar{\alpha}(M \cup N) = \bar{\alpha}(M) + \bar{\alpha}(N)$.

6° Existence de la mesure $\mu$.

En vertu de la prop. 18 du n° 9, il existe une forme linéaire positive $\beta$ et une seule sur l’espace vectoriel $\mathcal{E}(\bar{\Phi})$ des fonctions $\bar{\Phi}$-étagées, telle que $\beta(\varphi_M) = \bar{\alpha}(M)$ pour tout $M \in \bar{\Phi}$. Pour toute partie compacte $K$ de $X$, désignons par $\mathcal{G}(K)$ l’espace des limites uniformes de fonctions de $\mathcal{E}(\bar{\Phi})$ dont le support est contenu dans $K$. Comme $\beta$ est positive, on a $|\beta(f)| \leq \bar{\alpha}(K) \cdot \|f\|$ pour toute fonction $f \in \mathcal{E}(\bar{\Phi})$ dont le support est contenu dans $K$; la restriction de $\beta$ à l’espace de ces fonctions est une forme linéaire continue pour la topologie de la convergence uniforme ; elle se prolonge donc en une forme linéaire continue positive $\bar{\beta}_K$ sur $\mathcal{G}(K)$. En outre, si $K$ et $K_1$ sont deux ensembles compacts tels que

K ⊂ K₁, la restriction de $\bar{\beta}_{K_1}$ à $\mathcal{G}(K)$ est identique à $\bar{\beta}_K$, donc il existe une forme linéaire positive $\bar{\beta}$ sur la réunion $\mathcal{G}$ des $\mathcal{G}(K)$, qui prolonge chacune des formes $\bar{\beta}_K$.

Or, comme tout ensemble compact appartient à $\bar{\Phi}$, l’espace $\mathcal{H}$ des fonctions numériques continues et à support compact est un sous-espace de $\mathcal{G}$ (n° 10, prop. 19); la restriction à $\mathcal{H}$ de la forme linéaire positive $\bar{\beta}$ est donc une mesure positive $\mu$. Montrons que pour tout ensemble compact K, on a $\mu(K) = \bar{\alpha}(K)$. Pour tout $\varepsilon > 0$, il existe un ensemble ouvert $U \in \bar{\Phi}$ tel que $K \subset U$, $\mu(U) \leq \mu(K) + \varepsilon$ et $\bar{\alpha}(U) \leq \bar{\alpha}(K) + \varepsilon$. Soit $f$ une application continue de X dans $[0, 1]$ dont le support est contenu dans U et telle que $f(x) = 1$ dans K (chap. III, § 1, n° 2, lemme 1). On a $\mu(K) \leq \mu(f) \leq \mu(U) \leq \mu(K) + \varepsilon$, et d’autre part

$$
\bar{\alpha}(K) = \beta(\varphi_K) \leq \bar{\beta}(f) \leq \beta(\varphi_U) = \bar{\alpha}(U) \leq \bar{\alpha}(K) + \varepsilon;
$$

comme $\mu(f) = \bar{\beta}(f)$, on voit que $|\mu(K) - \bar{\alpha}(K)| \leq \varepsilon$, et comme $\varepsilon$ est arbitraire, $\mu(K) = \bar{\alpha}(K)$.

La caractérisation des ensembles ouverts appartenant à $\bar{\Phi}$, jointe au cor. 4 du th. 4 du n° 6, montre alors que les ensembles ouverts appartenant à $\bar{\Phi}$ ne sont autres que les ensembles ouverts $\mu$-intégrables, et que, pour un tel ensemble U, on a $\mu(U) = \bar{\alpha}(U)$. Le th. 4 du n° 6 et la caractérisation des ensembles de $\bar{\Phi}$ donnée au 5° montrent ensuite que les ensembles $\mu$-intégrables sont les ensembles de $\bar{\Phi}$, et que, pour un tel ensemble M, on a $\mu(M) = \bar{\alpha}(M)$. Enfin, le fait que $\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$ pour tout ensemble ouvert U résulte aussitôt de (PC₂) et du cor. 4 du th. 4 du n° 6.

Le théorème 5 est ainsi complètement démontré.

#### Corollaire {#int-iv-s4-n11-cor-1 .statement}

Soient X un espace localement compact à base dénombrable, $\Psi$ l’ensemble des parties boréliennes de X, $\beta$ une application de $\Psi$ dans $[0, +\infty]$ satisfaisant aux conditions suivantes:

(i) Si $(B_1, B_2, \ldots)$ est une suite de parties boréliennes de X deux à deux disjointes, on a $\beta(B_1 \cup B_2 \cup \ldots) = \beta(B_1) + \beta(B_2) + \ldots$

(ii) Si B est une partie compacte de X, on a $\beta(B) < +\infty$.

Alors il existe une mesure positive $\mu$ sur X et une seule telle que $\beta(B) = \mu^*(B)$ pour tout $B \in \Psi$.

Soient $\Phi$ l’ensemble des parties compactes de X et $\alpha$ la restriction de $\beta$ à $\Phi$. Alors les conditions (PC₁), (PC₂), (PM₁), (PM₂), (PM₃), (PM₄) sont satisfaites. Soient K une partie compacte de X, et $\varepsilon > 0$. Alors K est l’intersection d’une suite décroissante $(U_1, U_2, \ldots)$ de parties ouvertes relativement compactes de X (Top. gén., chap. IX, 2e éd., § 2, n° 5, prop. 7).

On a $\sum_{n=1}^{+\infty} \beta(U_n - U_{n+1}) = \beta(U_1 - K) < +\infty$, donc

$$
\beta(U_n) - \beta(K) = \beta(U_n - K) = \sum_{p=n}^{+\infty} \beta(U_p - U_{p+1})
$$

tend vers 0 quand n tend vers $+\infty$. Ceci prouve que la condition (PM₄) est satisfaite. D’après le th. 5, il existe une mesure positive $\mu$ sur X telle que $\mu(K) = \alpha(K)$ pour toute partie compacte K de X. Comme toute partie ouverte U de X est réunion d’une suite croissante de parties compactes, on a $\mu^*(U) = \beta(U)$. Soit L une partie compacte de X. D’après la prop. 7 du n° 5, les parties $\mu$-intégrables de L forment une tribu de parties de L. Donc, si B est un élément de $\Psi$ contenu dans L, B est $\mu$-intégrable; pour tout $\varepsilon > 0$, il existe alors une partie compacte K et une partie ouverte U de X telles que $K \subset B \subset U$, $\mu^*(U) - \mu(K) \leq \varepsilon$ (n° 6, th. 4). Comme $\beta(U) = \mu^*(U)$ et $\beta(K) = \mu(K)$, on voit que $|\mu^*(B) - \beta(B)| \leq 2\varepsilon$. Donc $\beta(B) = \mu^*(B)$. Enfin, toute partie borélienne C de X est réunion d’une suite de parties boréliennes relativement compactes deux à deux disjointes, d’où $\beta(C) = \mu^*(C)$. L’unicité de $\mu$ résulte aussitôt du th. 5.

## EXERCICES {#int-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
