---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 1
section_title: Intégrale supérieure d'une fonction positive
lang: fr
source: int-i-iv-fr
pdf_pages: 0110-0120, 0238-0240
extraction: ocr
subsections:
    - "no": 1
      title: Intégrale supérieure d’une fonction positive semi-continue inférieurement
      page: 0
      pdf_page: 110
    - "no": 2
      title: Mesure extérieure d’un ensemble ouvert
      page: 0
      pdf_page: 113
    - "no": 3
      title: Intégrale supérieure d’une fonction positive
      page: 0
      pdf_page: 115
    - "no": 4
      title: Mesure extérieure d’un ensemble quelconque
      page: 0
      pdf_page: 119
statements: 35
exercises: 8
content_sha256: 5f9164258bd35e913c9b1ad80cf0b00b602f786cff5634e309986fe6cc189e46
---

## § 1. Intégrale supérieure d’une fonction positive

### 1. Intégrale supérieure d’une fonction positive semi-continue inférieurement

Soient X un espace localement compact, $\mu$ une mesure positive sur X ; on sait que $\mu$ est une fonction croissante dans l’ensemble réticulé $\mathcal{K}_+(X)$ (que nous noterons aussi $\mathcal{K}_+$).

Nous désignerons par $\mathcal{I}_+(X)$ (ou simplement $\mathcal{I}_+$) l’ensemble des fonctions numériques positives, finies ou non, et semi-continues inférieurement dans X. Rappelons que la somme d’une famille quelconque de fonctions de $\mathcal{I}_+$ appartient à $\mathcal{I}_+$; le produit d’une fonction de $\mathcal{I}_+$ par un nombre fini $\alpha > 0$ appartient à $\mathcal{I}_+$; l’enveloppe supérieure d’une famille quelconque de fonctions de $\mathcal{I}_+$ et l’enveloppe inférieure d’une famille finie de fonctions de $\mathcal{I}_+$ appartiennent aussi à $\mathcal{I}_+$ (Top. gén., chap. IV, § 6, n° 2, prop. 2 et th. 4). Nous utiliserons en outre le lemme suivant :

#### Lemme 1 {#int-iv-s1-lem-1 .statement}

Toute fonction $f \in \mathcal{I}_+$ est l’enveloppe supérieure de l’ensemble (filtrant pour la relation $\leqslant$) des fonctions $g \in \mathcal{K}_+$ telles que $g \leqslant f$.

En effet, pour tout $x \in X$ tel que $f(x) > 0$, et pour tout nombre réel fini $a$ tel que $0 < a < f(x)$, il existe par hypothèse un voisinage compact V de x tel que $f(y) \geq a$ dans V; d’autre part, il existe une fonction $g \in \mathcal{K}_+$, de support contenu dans V, égale à $a$ au point $x$ et $\leq a$ dans V (*Top. gén.*, chap. IX, § 1, n° 5, th. 2); on a donc $0 \leq g \leq f$ et $g(x) \geq a$, ce qui démontre le lemme.

#### Définition 1 {#int-iv-s1-def-1 .statement}

*Etant donnée une mesure positive $\mu$ sur X, on appelle intégrale supérieure d’une fonction $f \in \mathcal{J}_+$ (par rapport à $\mu$) le nombre positif (fini ou égal à $+\infty$)

$$
\mu^*(f) = \sup_{g \in \mathcal{K}_+, g \leq f} \mu(g).
$$

Pour toute fonction $f \in \mathcal{K}_+$, il est clair que $\mu^*(f) = \mu(f)$, autrement dit $\mu^*$ est un prolongement de $\mu$ à $\mathcal{J}_+$.

#### Exemple {#int-iv-s1-n1-exa-1 .statement}

Soient X un espace *discret*, $\mu$ une mesure positive sur X, et posons $\alpha(x) = \mu(\varphi_{\{x\}})$ pour tout $x \in X$. Toute fonction numérique $f$ définie dans X est alors continue; pour une telle fonction $f \geq 0$, on a $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$, en convenant de poser $\alpha(x)f(x) = 0$ lorsque $\alpha(x) = 0$ et $f(x) = +\infty$. En effet, on a

$$
\sum_{x \in X} \alpha(x)f(x) = \sup_M (\sum_{x \in M} \alpha(x)f(x)),
$$
où M parcourt l’ensemble des parties finies de X. S’il existe $x_0 \in X$ tel que $f(x_0) = +\infty$ et $\alpha(x_0) > 0$, on a $\sum_{x \in M} \alpha(x)f(x) = +\infty$ dès que $x_0 \in M$, et d’autre part, pour tout entier $n > 0$, on a $f \geq n \cdot \varphi_{\{x_0\}}$, donc $\mu^*(f) \geq n \alpha(x_0)$, et par suite $\mu^*(f) = +\infty$. Si au contraire $\alpha(x) = 0$ en tous les points où $f(x) = +\infty$, la fonction g égale à $f$ aux points $x \in M$ où $\alpha(x) > 0$, à 0 ailleurs, appartient à $\mathcal{K}_+$, et l’on a, en vertu des conventions faites, $\mu(g) = \sum_{x \in M} \alpha(x)f(x)$, ce qui prouve encore la relation $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$.

#### Proposition 1 {#int-iv-s1-prop-1 .statement}

*Pour tout nombre réel fini $\alpha > 0$ et toute fonction $f \in \mathcal{J}_+$, on a*

(1)
$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Proposition 2 {#int-iv-s1-prop-2 .statement}

*Sur l’ensemble $\mathcal{J}_+$, la fonction $\mu^*$ est croissante.*

Les démonstrations sont immédiates à partir de la déf. 1.

#### Théorème 1 {#int-iv-s1-thm-1 .statement}

*Soit H un ensemble non vide de fonctions de $\mathcal{J}_+$, filtrant pour la relation $\leq$. Pour toute mesure positive $\mu$ sur X, on a

(2) $$
\mu^*(\sup_{g \in H} g) = \sup_{g \in H} \mu^*(g) = \lim_{g \in H} \mu^*(g).
$$

Posons $f = \sup_{g \in H} g$. Nous démontrerons d’abord le théorème dans le cas particulier où les fonctions $g \in H$ et leur enveloppe supérieure $f$ appartiennent à $\mathcal{K}_+$. Il résulte alors du th. de Dini (*Top. gén.*, chap. X, 2e éd., § 4, n° 1, th. 1) que le filtre des sections de H converge *uniformément* vers $f$ dans toute partie compacte de X, et en particulier dans le support K de $f$. Comme $0 \leq g \leq f$ pour toute fonction $g \in H$, le support de toute fonction de H est contenu dans K ; mais par définition $\mu$ est continue dans l’espace vectoriel $\mathcal{K}(X, K; \mathbf{C})$ des fonctions continues à support contenu dans K, pour la topologie de la convergence uniforme ; d’où la relation (2) dans ce cas.

Passons au cas général. Il est clair que $\mu^*(g) \leq \mu^*(f)$ pour toute fonction $g \in H$. D’après la déf. 1, tout revient à montrer que, pour toute fonction $\psi \in \mathcal{K}_+$ telle que $\psi \leq f$, on a

$$
\mu(\psi) \leq \sup_{g \in H} \mu^*(g).
$$

Pour toute fonction $g \in H$, soit $\Phi_g$ l’ensemble des fonctions $\varphi \in \mathcal{K}_+$ telles que $\varphi \leq g$, et soit $\Phi$ la réunion des ensembles $\Phi_g$ lorsque g parcourt H ; comme H est filtrant, il en est de même de $\Phi$, et on a $f = \sup_{\varphi \in \Phi} \varphi$. Comme $\psi \leq f$, $\psi$ est l’enveloppe supérieure de l’ensemble des fonctions $\inf (\psi, \varphi)$ lorsque $\varphi$ parcourt $\Phi$ ; mais comme $\psi$ et les fonctions $\inf (\psi, \varphi)$ appartiennent à $\mathcal{K}_+$, la première partie de la démonstration prouve que $\mu(\psi) = \sup_{\varphi \in \Phi} \mu(\inf(\psi, \varphi))$. Or, chaque $\varphi \in \Phi$ appartient à un ensemble $\Phi_g$, donc

$$
\mu(\inf (\psi, \varphi)) \leq \mu(\varphi) \leq \mu^*(g) \leq \sup_{g \in H} \mu^*(g)
$$

d’où l’on déduit aussitôt que $\mu(\psi) \leq \sup_{g \in H} \mu^*(g)$. Nous avons donc prouvé que $\mu^*(f) = \sup_{g \in H} \mu^*(g)$; la relation $\mu^*(f) = \lim_{g \in H} \mu^*(g)$ est alors une conséquence du théorème de la limite monotone (*Top. gén.*, chap. IV, § 5, n° 2, th. 2).

#### Théorème 2 {#int-iv-s1-thm-2 .statement}

*Si $f_1$ et $f_2$ sont deux fonctions de $\mathcal{J}_+$, on a*

(3) $$
\mu^*(f_1 + f_2) = \mu^*(f_1) + \mu^*(f_2).
$$

En effet, lorsque $\varphi_1$ (resp. $\varphi_2$) parcourt l’ensemble des fonctions de $\mathcal{K}_+$ telles que $\varphi_1 \leq f_1$ (resp. $\varphi_2 \leq f_2$), les fonctions $\varphi_1 + \varphi_2$ forment un ensemble filtrant (pour $\leq$) dont l’enveloppe supérieure est $f_1 + f_2$. En vertu du th. 1, on a donc

$$
\mu^*(f_1 + f_2) = \sup \mu(\varphi_1 + \varphi_2) = \sup (\mu(\varphi_1) + \mu(\varphi_2)),
$$

$(\varphi_1, \varphi_2)$ parcourant l’ensemble des couples de fonctions de $\mathcal{K}_+$ telles que $\varphi_1 \leq f_1$ et $\varphi_2 \leq f_2$; comme on a

$$
\sup (\mu(\varphi_1) + \mu(\varphi_2)) = \sup \mu(\varphi_1) + \sup \mu(\varphi_2)
$$

(Top. gén., chap. IV, § 5, n° 7, cor. 2 de la prop. 12), le théorème est démontré.

#### Proposition 3 {#int-iv-s1-prop-3 .statement}

*Pour toute famille* $(f_i)_{i \in I}$ *de fonctions de* $\mathcal{I}_+$, *on a*

$$
\mu^*\left( \sum_{i \in I} f_i \right) = \sum_{i \in I} \mu^*(f_i).
$$

En effet, pour toute partie finie $J$ de $I$, il résulte du th. 2 (par récurrence sur le nombre d’éléments de $J$) que $\mu^*\left( \sum_{i \in J} f_i \right) = \sum_{i \in J} \mu^*(f_i)$; lorsque $J$ parcourt l’ensemble des parties finies de $I$, les fonctions $g_J = \sum_{i \in J} f_i$ appartiennent à $\mathcal{I}_+$ et forment un ensemble filtrant pour la relation $\leq$, dont l’enveloppe supérieure est la fonction $\sum_{i \in I} f_i$; la proposition résulte donc du th. 1.

#### Proposition 4 {#int-iv-s1-prop-4 .statement}

*Soit* $f$ *une fonction de* $\mathcal{I}_+$. *L’application* $\mu \mapsto \mu^*(f)$ *de l’ensemble* $\mathcal{M}_+(X)$ *des mesures positives sur* $X$, *dans la droite achevée* $\bar{\mathbf{R}}$, *est semi-continue inférieurement pour la topologie vague sur* $\mathcal{M}_+(X)$ *(chap. III, § 1, n° 9)*.

En effet, cette application est par définition l’enveloppe supérieure des applications $\mu \mapsto \mu(g)$, où $g$ parcourt l’ensemble des fonctions de $\mathcal{K}_+$ telles que $g \leq f$; et par définition de la topologie vague, les applications $\mu \mapsto \mu(g)$ sont continues dans $\mathcal{M}(X)$.

### 2. Mesure extérieure d’un ensemble ouvert

Etant donné un ensemble *ouvert* $G \subset X$, sa fonction caractéristique $\varphi_G$ est *semi-continue inférieurement* dans $X$ (*Top. gén.*, chap. IV, § 6, n° 2, cor. de la prop. 1). On peut donc poser la définition suivante:

#### Définition 2 {#int-iv-s1-def-2 .statement}

Etant donnée une mesure positive $\mu$ sur $X$, pour tout ensemble ouvert $G \subset X$, on appelle mesure extérieure de $G$, et l’on note $\mu^*(G)$, l’intégrale supérieure $\mu^*(\varphi_G)$.

La mesure extérieure d’un ensemble ouvert $G$ est donc un nombre $\geqslant 0$, fini ou égal à $+\infty$. On a $\mu^*(\emptyset) = 0$. En outre $\mu^*(X) = \| \mu \|$, comme le montre la formule (23) du chap. III, § 1, n° 8.

#### Proposition 5 {#int-iv-s1-prop-5 .statement}

La mesure extérieure d’un ensemble ouvert relativement compact $G$ est finie.

En effet, il existe alors une fonction $f \in \mathcal{K}_+$ telle que $\varphi_G \leqslant f$ (chap. III, § 1, n° 2, lemme 1), d’où
$$
\mu^*(G) = \mu^*(\varphi_G) \leqslant \mu^*(f) = \mu(f) < +\infty.
$$
Un ensemble ouvert de mesure extérieure finie n’est pas toujours relativement compact (exerc. 3).

#### Proposition 6 {#int-iv-s1-prop-6 .statement}

Si $G_1$ et $G_2$ sont deux ensembles ouverts tels que $G_1 \subset G_2$, on a $\mu^*(G_1) \leqslant \mu^*(G_2)$.

En effet, la relation $G_1 \subset G_2$ équivaut à $\varphi_{G_1} \leqslant \varphi_{G_2}$.

#### Proposition 7 {#int-iv-s1-prop-7 .statement}

Soit $\mathfrak{G}$ un ensemble de parties ouvertes de $X$, filtrant pour la relation $\subset$; on a
$$
\mu^*\left( \bigcup_{G \in \mathfrak{G}} G \right) = \sup_{G \in \mathfrak{G}} \mu^*(G).
$$
En effet, les fonctions $\varphi_G$ forment un ensemble filtrant (pour $\leqslant$) dans $\mathcal{J}_+$ et leur enveloppe supérieure est la fonction caractéristique de la réunion des ensembles $G \in \mathfrak{G}$; la proposition est donc une conséquence du th. 1.

#### Proposition 8 {#int-iv-s1-prop-8 .statement}

Soit $(G_i)_{i \in I}$ une famille quelconque d’ensembles ouverts; on a
$$
\mu^*\left( \bigcup_{i \in I} G_i \right) \leqslant \sum_{i \in I} \mu^*(G_i).
$$
En outre, si les $G_i$ sont deux à deux sans point commun, on a
$$
\mu^*\left( \bigcup_{i \in I} G_i \right) = \sum_{i \in I} \mu^*(G_i).
$$
En effet, si $G = \bigcup_{i \in I} G_i$, on a $\varphi_G = \sup_{i \in I} \varphi_{G_i} \leqslant \sum_{i \in I} \varphi_{G_i}$; lorsque les $G_i$ sont deux à deux sans point commun, $\varphi_G = \sum_{i \in I} \varphi_{G_i}$; la proposition est donc conséquence du th. 1 et de la prop. 3.

#### Exemple {#int-iv-s1-n2-exa-1 .statement}

Prenons $X = \mathbf{R}$, et soit $\mu$ la mesure de Lebesgue sur $\mathbf{R}$ (chap. III, § 1, n° 3); nous allons déterminer la mesure extérieure d’un intervalle ouvert $G = ]a, b[$ ($-\infty \leq a < b \leq +\infty$). Supposons d’abord $a$ et $b$ finis. Pour toute fonction de $f$ de $\mathscr{K}_+$ telle que $f \leq \varphi_G$, on a, d’après le th. de la moyenne,

$$
\int_{-\infty}^{+\infty} f(x) \, dx = \int_a^b f(x) \, dx \leq b - a,
$$

d’où $\mu^*(G) \leq b - a$. D’autre part, pour tout $\varepsilon > 0$, il existe une fonction $f \in \mathscr{K}_+$ telle que $f \leq \varphi_G$ et $f(x) = 1$ pour $a + \varepsilon \leq x \leq b - \varepsilon$; d’où $\mu^*(G) \geq b - a - 2\varepsilon$; comme $\varepsilon$ est arbitraire, on a

$$
\mu^*(G) = b - a;
$$

en d’autres termes, la mesure extérieure de $G$ est égale à sa longueur. Ce résultat s’étend aussitôt au cas où $G$ est un intervalle ouvert illimité, puisqu’il contient alors des intervalles ouverts bornés de longueur arbitrairement grande; on a donc dans ce cas $\mu^*(G) = +\infty$.

Soit maintenant $G$ un ensemble ouvert quelconque dans $\mathbf{R}$; $G$ est une réunion d’un ensemble dénombrable (fini ou infini) d’intervalles ouverts $]a_k, b_k[$, deux à deux sans point commun (Top. gén., chap. IV, § 2, n° 5, prop. 2); on a par suite

$$
\mu^*(G) = \sum_k (b_k - a_k)
$$

(prop. 8); autrement dit:

#### Proposition 9 {#int-iv-s1-prop-9 .statement}

Pour la mesure de Lebesgue sur $\mathbf{R}$, la mesure extérieure d’un ensemble ouvert dans $\mathbf{R}$ est égale à la somme des longueurs de ses composantes connexes.

On notera en particulier que si $G$ est un ensemble ouvert dans $\mathbf{R}$ tel que $\mu^*(G) = 0$, $G$ est vide.

### 3. Intégrale supérieure d’une fonction positive

Pour toute fonction numérique $f \geq 0$ (finie ou non) définie dans $X$, il existe des fonctions $h \in \mathscr{J}_+$ telles que $f \leq h$, ne serait-ce que la constante $+\infty$.

#### Définition 3 {#int-iv-s1-def-3 .statement}

Soit $\mu$ une mesure positive sur $X$; pour toute fonction numérique $f \geq 0$ (finie ou non) définie dans $X$, on appelle intégrale supérieure de $f$ (par rapport à $\mu$) le nombre positif (fini ou égal à $+\infty$)

$$
\mu^*(f) = \inf_{h \geq f, h \in \mathcal{I}_+} \mu^*(h).
$$

Lorsque $f \in \mathcal{I}_+$, le nombre $\mu^*(f)$ ainsi défini est égal à l’intégrale supérieure définie dans la déf. 1, puisque $\mu^*$ est croissante dans $\mathcal{I}_+$.

Au lieu de la notation $\mu^*(f)$, nous utiliserons aussi les notations $\int^* f d\mu$, $\int^* f(x) d\mu(x)$, $\int^* f\mu$ et $\int^* f(x)\mu(x)$.

#### Exemple {#int-iv-s1-n3-exa-1 .statement}

Si $X$ est un espace discret, $\mu$ une mesure positive sur $X$ et si l’on pose $\alpha(x) = \mu(\varphi_{\{x\}})$, on a $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$ pour toute fonction numérique $f \geq 0$ définie dans $X$, puisqu’une telle fonction est continue (n° 1, Exemple).

#### Proposition 10 {#int-iv-s1-prop-10 .statement}

Si $f$ et $g$ sont deux fonctions numériques $\geq 0$ définies dans $X$ et telles que $f \leq g$, on a $\mu^*(f) \leq \mu^*(g)$.

#### Proposition 11 {#int-iv-s1-prop-11 .statement}

Pour tout nombre réel fini $\alpha > 0$ et toute fonction numérique $f \geq 0$ définie dans $X$, on a

$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Proposition 12 {#int-iv-s1-prop-12 .statement}

Si $f_1$ et $f_2$ sont deux fonctions numériques $\geq 0$ définies dans $X$, on a

$$
\mu^*(f_1 + f_2) \leq \mu^*(f_1) + \mu^*(f_2).
$$

En effet, pour toute fonction $h_1 \in \mathcal{I}_+$ telle que $f_1 \leq h_1$ et toute fonction $h_2 \in \mathcal{I}_+$ telle que $f_2 \leq h_2$, on a, en vertu du th. 2,

$$
\mu^*(f_1 + f_2) \leq \mu^*(h_1 + h_2) = \mu^*(h_1) + \mu^*(h_2)
$$

d’où (Top. gén., chap. IV, § 5, n° 7, cor. 2 de la prop. 12)

$$
\mu^*(f_1 + f_2) \leq \inf_{h_1 \geq f_1, h_1 \in \mathcal{I}_+} \mu^*(h_1) + \inf_{h_2 \geq f_2, h_2 \in \mathcal{I}_+} \mu^*(h_2)
$$

ce qui n’est autre que l’inégalité (9).

Les prop. 10, 11 et 12 expriment que $\mu^*$ est une fonction croissante, positivement homogène et convexe dans l’ensemble des fonctions numériques $\geq 0$ définies dans $X$ (chap. I, n° 1). On notera que si $f_1$ et $f_2$ sont deux fonctions positives quelconques, les deux membres de (9) ne sont pas nécessairement égaux (§ 4, exerc. 8 d)); nous donnerons au § 5, n° 6 des conditions moyennant lesquelles l’égalité a lieu.

#### Théorème 3 {#int-iv-s1-thm-3 .statement}

Pour toute suite croissante $(f_n)$ de fonctions numériques $\geqslant 0$ définies dans E, on a

$$
\mu^*(\sup_n f_n) = \sup_n \mu^*(f_n).
$$

Comme chacune des fonctions $f_n$ est au plus égale à $\sup_n f_n$, tout revient à prouver que $\mu^*(\sup_n f_n) \leqslant \sup_n \mu^*(f_n)$; c’est évident si le second membre de cette inégalité est $+\infty$. Dans le cas contraire, on a $\mu^*(f_n) < +\infty$ pour tout $n$; nous allons montrer que, pour tout $\varepsilon > 0$, il existe une suite croissante $(g_n)$ de fonctions de $\mathcal{I}_+$ telle que $f_n \leqslant g_n$ et que $\mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon$. Si $g$ est l’enveloppe supérieure de la suite $(g_n)$, on aura $\mu^*(g) = \sup_n \mu^*(g_n)$ (n° 1, th. 1), d’où $\mu^*(g) \leqslant \sup \mu^*(f_n) + \varepsilon$; comme $\sup f_n \leqslant g$ et que $\varepsilon$ est arbitraire, le théorème sera démontré.

Par hypothèse, il existe une fonction $h_n \in \mathcal{I}_+$ telle que $f_n \leqslant h_n$ et que $\mu^*(f_n) \leqslant \mu^*(h_n) \leqslant \mu^*(f_n) + \frac{\varepsilon}{2^n}$; montrons que les fonctions $g_n = \sup(h_1, h_2, \ldots, h_n)$ répondent à la question. Elles appartiennent à $\mathcal{I}_+$, forment une suite croissante, et l’on a $f_n \leqslant g_n$ pour tout $n$; nous allons prouver qu’on a

$$
\mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon \left(1 - \frac{1}{2^n}\right).
$$

Raisonnons par récurrence sur $n$; le cas $n = 1$ est trivial. On a d’autre part $g_{n+1} = \sup(g_n, h_{n+1})$, $g_n \geqslant f_n$ et $h_{n+1} \geqslant f_{n+1} \geqslant f_n$, d’où $\inf(g_n, h_{n+1}) \geqslant f_n$; comme on a

$$
\inf(g_n, h_{n+1}) + \sup(g_n, h_{n+1}) = g_n + h_{n+1},
$$

il résulte du th. 2 du n° 1 que

$$
\mu^*(g_{n+1}) = \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(\inf(g_n, h_{n+1}))
$$
$$
\leqslant \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(f_n) \leqslant \mu^*(f_{n+1}) + \varepsilon \left(1 - \frac{1}{2^n}\right) + \frac{\varepsilon}{2^{n+1}}
$$
$$
= \mu^*(f_{n+1}) + \varepsilon \left(1 - \frac{1}{2^{n+1}}\right).
$$

C.Q.F.D.

#### Corollaire {#int-iv-s1-n3-cor-1 .statement}

Soit $\mathfrak{F}$ un ensemble de fonctions numériques $\geqslant 0$, filtrant pour la relation $\leqslant$ et tel qu’il existe une partie cofinale dénombrable $\mathfrak{G}$ de $\mathfrak{F}$ (Ens., chap. III, § 1, n° 7); on a
$$
\mu^*(\sup_{f \in \mathfrak{F}} f) = \sup_{f \in \mathfrak{F}} \mu^*(f).
$$
En effet, il existe une suite croissante de fonctions de $\mathfrak{G}$ ayant même enveloppe supérieure que $\mathfrak{F}$: si $(f_n)$ est la suite des fonctions de $\mathfrak{G}$, rangées dans un ordre quelconque, soit $(f_{n_k})$ une suite partielle définie par récurrence par les conditions $n_1 = 1$, $f_{n_{k+1}} \geqslant \sup(f_{n_k}, f_k)$; il est clair que cette suite partielle a les propriétés indiquées.

#### Remarque 1 {#int-iv-s1-n3-rem-1 .statement}

La relation (11) ne subsiste plus nécessairement lorsque $\mathfrak{F}$ est un ensemble filtrant non dénombrable de fonctions $\geqslant 0$ non semi-continues inférieurement. Prenons par exemple $X = \mathbf{R}$, $\mu$ étant la mesure de Lebesgue sur $\mathbf{R}$, et considérons l’ensemble filtrant (pour $\leqslant$) $\mathfrak{F}$ des fonctions caractéristiques $\varphi_M$ de toutes les parties finies $M$ de $\mathbf{R}$. On a $\mu^*(\varphi_M) = 0$ quel que soit l’ensemble fini $M$, car un point est contenu dans un intervalle ouvert de longueur arbitrairement petite, et la fonction caractéristique d’un ensemble réduit à un point a donc une intégrale supérieure nulle, en vertu de la déf. 3 et de la prop. 9 du n° 2. Mais l’enveloppe supérieure de $\mathfrak{F}$ est la fonction constante égale à 1 et l’on a $\mu^*(1) = +\infty$.

#### Remarque 2 {#int-iv-s1-n3-rem-2 .statement}

On observera que pour une suite décroissante $(f_n)$ de fonctions $\geqslant 0$, on n’a pas nécessairement $\mu^*(\inf_n f_n) = \inf_n \mu^*(f_n)$, même si $\mu^*(f_n) < +\infty$ pour tout $n$ (cf. § 4, exerc. 8 c)).

#### Proposition 13 {#int-iv-s1-prop-13 .statement}

Pour tout suite $(f_n)$ de fonctions numériques $\geqslant 0$, définies dans $X$, on a
$$
\mu^*\left( \sum_{n=1}^\infty f_n \right) \leqslant \sum_{n=1}^\infty \mu^*(f_n).
$$
Il suffit d’appliquer la relation (10) à la suite croissante des fonctions $g_n = \sum_{k=1}^n f_k$ en tenant compte de ce que, d’après (9), on a
$$
\mu^*(g_n) \leqslant \sum_{k=1}^n \mu^*(f_k).
$$
Au § 5, n° 6, nous donnerons des conditions moyennant lesquelles les deux membres de (12) sont égaux.

#### Proposition 14 (lemme de Fatou) {#int-iv-s1-prop-14 .statement}

Pour toute suite $(f_n)$ de fonctions numériques $\geqslant 0$, on a
$$
\mu^*(\lim_{n \to \infty} \inf f_n) \leqslant \lim_{n \to \infty} \inf \mu^*(f_n).
$$

En effet, pour tout entier $n$, posons $g_n = \inf_{p \geq 0} f_{n+p}$; la suite $(g_n)$ est croissante, et l’on a $\lim . \inf f_n = \sup_{n \to \infty} g_n$, d’où, en vertu de (10),
$$
\mu^*(\lim . \inf f_n) = \sup_{n \to \infty} \mu^*(g_n);
$$
mais comme $g_n \leq f_{n+p}$ pour $p \geq 0$, on a $\mu^*(g_n) \leq \mu^*(f_{n+p})$, d’où $\mu^*(g_n) \leq \inf_{p \geq 0} \mu^*(f_{n+p})$, et finalement
$$
\mu^*(\lim . \inf f_n) \leq \sup_{n \to \infty} (\inf_{p \geq 0} \mu^*(f_{n+p})) = \lim . \inf_{n \to \infty} \mu^*(f_n).
$$

#### Corollaire {#int-iv-s1-n3-cor-2 .statement}

Soit $(f_n)$ une suite de fonctions numériques $\geq 0$ telle que, pour tout $x \in X$, $\lim_{n \to \infty} f_n(x) = +\infty$. Si la mesure $\mu$ n’est pas nulle, on a $\lim_{n \to \infty} \mu^*(f_n) = +\infty$.

En effet, si $f_0$ est la fonction constante égale à $+\infty$, $f_0$ est l’enveloppe supérieure de toutes les fonctions de $\mathcal{K}_+$, et comme $\mu \neq 0$, on a $\mu^*(f_0) > 0$; mais comme $f_0 = \alpha f_0$ pour tout $\alpha > 0$, on a nécessairement $\mu^*(f_0) = +\infty$ (prop. 11). L’inégalité (13) montre alors que $\mu^*(f_n)$ tend vers $+\infty$ avec $n$.

#### Proposition 15 {#int-iv-s1-prop-15 .statement}

Pour tout scalaire $\alpha > 0$ et tout couple de mesures positives $\mu, \nu$ sur $X$, on a
$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + \nu)^* = \mu^* + \nu^*.
$$
En outre, la relation $\mu \leq \nu$ entraîne $\mu^* \leq \nu^*$.

Démontrons la relation (15). Posons $\lambda = \mu + \nu$; on a donc $\lambda(f) = \mu(f) + \nu(f)$ pour $f \in \mathcal{K}_+$; pour $f \in \mathcal{J}_+$, la valeur de $\lambda^*(f)$ (resp. $\mu^*(f)$, $\nu^*(f)$) est la limite de $\lambda(g)$ (resp. $\mu(g)$, $\nu(g)$) lorsque $g$ parcourt l’ensemble filtrant (pour $\leq$) des $g \in \mathcal{K}_+$ telles que $g \leq f$; on a donc $\lambda^*(f) = \mu^*(f) + \nu^*(f)$. Enfin, si $f$ est une fonction $\geq 0$ quelconque définie dans $X$, $\lambda^*(f)$ (resp. $\mu^*(f)$, $\nu^*(f)$) est la limite de $\lambda^*(h)$ (resp. $\mu^*(h)$, $\nu^*(h)$) lorsque $h$ parcourt l’ensemble filtrant (pour $\geq$) des fonctions $h \in \mathcal{J}_+$ telles que $h \geq f$; on a donc encore, par passage à la limite, $\lambda^*(f) = \mu^*(f) + \nu^*(f)$, ce qui démontre (15). On établit de même la relation (14). Enfin, si $\mu \leq \nu$, on peut écrire $\nu = \mu + (\nu - \mu)$, où $\nu - \mu \geq 0$, donc $\nu^* = \mu^* + (\nu - \mu)^*$, ce qui montre que $\mu^* \leq \nu^*$.

### 4. Mesure extérieure d’un ensemble quelconque

#### Définition 4 {#int-iv-s1-def-4 .statement}

Soit $\mu$ une mesure positive sur $X$; pour toute partie $A$ de $X$, on appelle mesure extérieure de $A$ (pour la mesure $\mu$), et on note $\mu^*(A)$, l’intégrale supérieure $\mu^*(\varphi_A)$.

La mesure extérieure d’un ensemble est donc un nombre $\geq 0$, fini ou égal à $+\infty$, qui coïncide pour les ensembles ouverts avec la mesure extérieure définie dans la déf. 2 du n° 2.

#### Proposition 16 {#int-iv-s1-prop-16 .statement}

*Si A et B sont deux parties de X telles que $A \subset B$, on a $\mu^*(A) \leq \mu^*(B)$.*

#### Corollaire {#int-iv-s1-n4-cor-1 .statement}

*Tout ensemble relativement compact dans X est de mesure extérieure finie.*
En effet, un tel ensemble est contenu dans un ensemble ouvert relativement compact (*Top. gén.*, chap. I, 3e éd., § 9, n° 7, prop. 10), dont la mesure extérieure est finie (n° 2, prop. 5).

#### Proposition 17 {#int-iv-s1-prop-17 .statement}

*Si $(A_n)$ est une suite croissante de parties de X, on a*
$$
\mu^*\left( \bigcup_n A_n \right) = \sup_n \mu^*(A_n).
$$

#### Proposition 18 {#int-iv-s1-prop-18 .statement}

*Pour toute suite $(A_n)$ de parties de X, on a*
$$
\mu^*\left( \bigcup_n A_n \right) \leq \sum_n \mu^*(A_n).
$$
Ces propositions sont les traductions des prop. 10 et 13 et du th. 3 du n° 3 pour les fonctions caractéristiques d’ensembles.

#### Proposition 19 {#int-iv-s1-prop-19 .statement}

*Pour toute partie A de X, $\mu^*(A)$ est la borne inférieure des mesures extérieures des ensembles ouverts contenant A.*
La proposition est évidente si $\mu^*(A) = +\infty$. Dans le cas contraire, pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, il existe une fonction $f \in \mathcal{J}_+$ telle que $\varphi_A \leq f$ et $\mu^*(A) \leq \mu^*(f) \leq \mu^*(A) + \varepsilon$. Soit G l’ensemble des $x \in X$ tels que $f(x) > 1 - \varepsilon$. Comme $f$ est semi-continue inférieurement, G est ouvert (*Top. gén.*, chap. IV, § 6, n° 2, prop. 1) et contient A ; on a d’autre part $f \geq (1 - \varepsilon)\varphi_G$, d’où
$$
\mu^*(G) \leq \frac{1}{1 - \varepsilon} \mu^*(f) \leq \frac{1}{1 - \varepsilon} (\mu^*(A) + \varepsilon);
$$
comme $\varepsilon$ est arbitraire, on voit que $\mu^*(G)$ diffère d’aussi peu qu’on veut de $\mu^*(A)$, d’où la proposition.

## EXERCICES {#int-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
