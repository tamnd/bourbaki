---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES ET INTÉGRALES
section: 2
section_title: Intégrales dans les intervalles non compacts
lang: fr
source: fvr-i-vii-fr
book_pages: FVR II.13-FVR II.18, FVR II.33-FVR II.35
pdf_pages: 0065-0070, 0085-0087
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une intégrale dans un intervalle non compact
      page: 13
      pdf_page: 65
    - "no": 2
      title: Intégrales de fonctions positives dans un intervalle non compact
      page: 16
      pdf_page: 68
    - "no": 3
      title: Intégrales absolument convergentes
      page: 18
      pdf_page: 70
statements: 10
exercises: 9
content_sha256: 2e3ce1ec4cd28d07427e7c5d21beaf54631c9beb95a004344a91eb9cc657feaa
---

## § 2. INTÉGRALES DANS LES INTERVALLES NON COMPACTS

### 1. Définition d’une intégrale dans un intervalle non compact

Soit $I$ un intervalle compact $(a, b)$ de la droite achevée $\overline{\mathbf{R}}$ ($a$ et $b$ pouvant donc être infinis); soit $\mathbf{f}$ une fonction définie dans $[a, b[$, prenant ses valeurs dans un espace normé complet $\mathbf{E}$ sur $\mathbf{R}$. Généralisant la déf. I de II, p. 1, nous dirons qu’une fonction $\mathbf{g}$, définie dans $[a, b[$, à valeurs dans $\mathbf{E}$, est une primitive de $\mathbf{f}$ si elle est continue dans $[a, b[$ (et en particulier aux extrémités $a, b$) et admet une dérivée égale à $\mathbf{f}(x)$ en tous les points du complémentaire par rapport à $[a, b[$ d’une partie dénombrable de cet intervalle.

Nous allons nous borner à considérer le cas suivant: il existe une suite finie strictement croissante $(c_i)_{0 \leq i \leq n}$ de points de $I = (a, b)$, telle que $c_0 = a, c_n = b$, et que $\mathbf{f}$ soit réglée dans chacun des intervalles ouverts $]c_i, c_{i+1}[$, mais non réglée dans tout intervalle ouvert contenant au moins un point $c_i$ intérieur à $I$; une telle fonction sera dite réglée par morceaux dans $[a, b[$. On notera qu’une fonction réglée dans $[a, b[$ est réglée par morceaux (en prenant $n = 1$ dans la définition précédente).

Si $\mathbf{f}$ admet une primitive $\mathbf{g}$ dans $I$ (au sens précisé ci-dessus), et si $a$ est un point de l’intervalle $]c_i, c_{i+1}[$ ($0 \leq i \leq n - 1$), on a, par hypothèse, pour tout $x$ appartenant à cet intervalle, $\mathbf{g}(x) - \mathbf{g}(a) = \int_a^x \mathbf{f}(t)dt$; $\mathbf{g}$ étant continue dans $I$ par hypothèse, on voit que $\int_a^x \mathbf{f}(t)dt$ doit tendre vers une limite dans $\mathbf{E}$ lorsque $x$ tend vers $c_i$ à droite et lorsque $x$ tend vers $c_{i+1}$ à gauche. Inversement, supposons que ces conditions soient vérifiées pour tout $t$, et soit $\mathbf{g}_i$ une primitive de $\mathbf{f}$ dans l’intervalle $]c_i, c_{i+1}[$ ($0 \leq i \leq n - 1$); on constate aussitôt que la fonction $\mathbf{g}$, définie dans le complémentaire par rapport à $I$ de l’ensemble des $c_i$, par la condition d’être à égale à $\mathbf{g}_i(x) + \sum_{k=1}^i (\mathbf{g}_{k-1}(c_k-) - \mathbf{g}_k(c_k+))$ dans $]c_i, c_{i+1}[$ pour $0 \leq i \leq n - 1$, est continue en tout point de $I$ distinct des $c_i$ et admet une limite en chacun de ces points; elle peut donc être prolongée par continuité en chacun des $c_i$, et la fonction prolongée est évidemment une primitive de $\mathbf{f}$ dans $I$. Il est clair en outre que toute autre primitive de $\mathbf{f}$ est de la forme $\mathbf{g} + \mathbf{a}$ ($\mathbf{a}$ élément de $E$).

#### Définition 1 {#fvr-ii-s2-def-1 .statement}

On dit qu’une fonction vectorielle $\mathbf{f}$ réglée par morceaux dans un intervalle $(a, b)$ de $\mathbf{R}$ admet une intégrale dans cet intervalle si $\mathbf{f}$ admet une primitive dans $(a, b)$; si $\mathbf{g}$ est une quelconque des primitives de $\mathbf{f}$ dans $(a, b)$, $x_0$ et $x$ deux points quelconques de $(a, b)$, on appelle intégrale de $\mathbf{f}$ de $x_0$ à $x$, et on note $\int_{x_0}^x \mathbf{f}(t)\ dt$ l’élément $\mathbf{g}(x) - \mathbf{g}(x_0)$.

Cette notion coïncide évidemment avec celle définie lorsque l’intervalle $(x_0, x)$ ne contient aucun des points $c_i$.

Les remarques qui précèdent la déf. 1 montrent que, pour que $\mathbf{f}$ ait une intégrale dans $]a, b[$, il faut et il suffit que sa restriction à chacun des intervalles $]c_i, c_{i+1}[$ admette une intégrale dans cet intervalle. Autrement dit, on est ramené au cas où $\mathbf{f}$ est réglée dans un intervalle non compact $I \subset \mathbf{R}$, d’extrémités $a, b$ ($a < b$), et où: 1° ou bien un des nombres $a, b$ (au moins) est infini; 2° ou bien $\mathbf{f}$ n’est pas réglée dans un intervalle compact contenant au moins un des points $a, b$ (les deux hypothèses ne s’excluant pas mutuellement). Pour que $\mathbf{f}$ ait une intégrale dans $I$, il faut et il suffit alors que l’intégrale $\int_x^y \mathbf{f}(t)dt$ tende vers une limite lorsque le point $(x, y)$ tend vers $(a, b) \in \overline{\mathbf{R}}^2$ en restant dans $I \times I$, et cette limite n’est autre que $\int_a^b \mathbf{f}(t)dt$ d’après la déf. 1. Par abus de langage, au lieu de dire que $\mathbf{f}$ a une intégrale dans $I$, on dit encore que l’intégrale $\int_a^b \mathbf{f}(t)dt$ est convergente.

#### Exemple 1 {#fvr-ii-s2-n1-exa-1 .statement}

L’intégrale $\int_1^{+\infty} dt/t^2$ est convergente et égale à 1, car
$$
\int_1^x \frac{dt}{t^2} = 1 - \frac{1}{x}.
$$
2) L’intégrale $\int_0^1 dt/\sqrt{t}$ est convergente et égale à 2, car
$$
\int_x^1 \frac{dt}{\sqrt{t}} = 2(1 - \sqrt{x}) \quad \text{pour } x > 0.
$$
3) Soit $(\mathbf{u}_n)_{n \leq 1}$ une suite infinie de points de $E$, et soit $\mathbf{f}$ la fonction en escalier définie dans l’intervalle $(1, +\infty)$ par les conditions: $\mathbf{f}(x) = \mathbf{u}_n$ pour $n \leq x < n + 1$. Pour que l’intégrale $\int_1^{+\infty} \mathbf{f}(t)dt$ soit convergente, il faut et il suffit que la série de terme général $\mathbf{u}_n$ soit convergente dans $E$; en effet, on a
$$
\int_1^n \mathbf{f}(t)\ dt = \sum_{p=1}^{n-1} \mathbf{u}_p,
$$
donc la condition est nécessaire; réciproquement, si la série de terme général $\mathbf{u}_n$ converge dans E, on a $\lim_{n \to \infty} u_n = 0$; or, si $n \leq x \leq n + 1$, on a $\int_1^n f(t) \, dt = \sum_{p=1}^{n-1} u_p + u_n(x - n)$, donc cette intégrale a pour limite $\sum_{n=1}^\infty u_n$ lorsque $x$ tend vers $+\infty$.

Il est immédiat que si une fonction $f$ réglée par morceaux admet une intégrale dans I, les formules (4) à (9) de II, p. 9 sont encore valables. De même, la formule (10) de II, p. 10 s’étend de la façon suivante : $f$ et $g$ sont supposées être des primitives de fonctions $f'$, $g'$ réglées dans ]$a, b$[, et on désigne par $[f.g]_a^b$ la limite (si elle existe) de $[f.g]_{x,y}^y$, lorsque $(x, y)$ tend vers $(a, b)$ (avec $a < x \leq y < b$) ; alors, si deux des expressions $[f.g]_a^b$, $\int_a^b [f(t).g'(t)] \, dt$, $\int_a^b [f'(t).g(t)] \, dt$ ont un sens, il en est de même de la troisième, et la formule (10) de II, p. 10 subsiste.

Enfin, soit $f$ une fonction numérique définie et continue dans $I = ]a, b[$, primitive d’une fonction $f'$ réglée dans ]$a, b$[; soit d’autre part $g$ une fonction vectorielle continue dans un intervalle ouvert $J$ contenant $f(I)$; si la fonction $g(f(x))f'(x)$ admet une intégrale dans $I$, et si $f$ tend vers une limite (finie ou non) aux points $a$ et $b$, $g$ admet une intégrale de $f(a+)$ à $f(b-)$, et on a la formule

$$
\int_a^b g(f(t))f'(t) \, dt = \int_{f(a+)}^{f(b-)} g(u) \, du.
$$

En effet, si $(x, y)$ tend vers $(a, b)$, $(f(x), f(y))$ tend vers $(f(a+), f(b-))$ par hypothèse ; il suffit donc d’appliquer la formule (12) de II, p. 11 entre $x$ et $y$ et de passer à la limite pour avoir (1).

Étant donnée une fonction $f$ réglée dans un intervalle non compact $I \subset \mathbf{R}$, d’extrémités $a$ et $b$ ($a < b$), la condition pour que $f$ ait une intégrale dans $I$ peut se présenter de la manière suivante. Les intervalles compacts $J \subset I$ forment un ensemble ordonné filtrant $\mathfrak{A}(I)$ pour la relation $\subset^1$, car si $[\alpha, \beta]$ et $[\gamma, \delta]$ sont deux intervalles compacts contenus dans $I$, et si on pose $\lambda = \min(\alpha, \gamma)$, $\mu = \max(\beta, \delta)$, l’intervalle $[\lambda, \mu]$ est contenu dans $I$ et contient les deux intervalles considérés. Pour tout intervalle compact $J = [\alpha, \beta]$ contenu dans $I$, posons alors

$$
\int_J f(t) \, dt = \int_\alpha^\beta f(t) \, dt;
$$

pour que $f$ admette une intégrale dans $I$, il faut et il suffit que l’application $J \mapsto \int_J f(t) \, dt$ ait une limite dans $E$ suivant l’ensemble ordonné filtrant $\mathfrak{A}(I)$; cette limite est alors l’intégrale $\int_I f(t) \, dt$, que nous noterons encore $\int_1 f(t) \, dt$.

1 Rappelons (E, III, p. 12) qu’un ensemble $\mathfrak{F}$ de parties de $I$ est filtrant pour la relation $\subset$ si, quels que soient $X \in \mathfrak{F}$, $Y \in \mathfrak{F}$ il existe $Z \in \mathfrak{F}$ tel que $X \subset Z$ et $Y \subset Z$. Si $S(X)$ désigne la partie de $\mathfrak{F}$ formée des $Y \in \mathfrak{F}$ tels que $U \supset X$, les $S(X)$ forment la base d’un filtre sur $\mathfrak{F}$, dit filtre des sections de $\mathfrak{F}$; la limite (si elle existe) d’une application $f$ de $\mathfrak{F}$ dans un espace topologique, suivant le filtre des sections de $\mathfrak{F}$, est encore dite limite de $f$ suivant l’ordonné filtrant $\mathfrak{F}$ (cf. TG, I, p. 49 et TG, IV, p. 18).

#### Proposition 1 (Critère de Cauchy pour les intégrales) {#fvr-ii-s2-prop-1 .statement}

Soit $f$ une fonction réglée dans un intervalle $I \subset \mathbf{R}$, de bornes $a$ et $b$ ($a < b$). Pour que l’intégrale $\int_a^b f(t)\ dt$ existe, il faut et il suffit que pour tout $\varepsilon > 0$, il existe un intervalle compact $J_0 = [\alpha, \beta]$ contenu dans $I$, tel que pour tout intervalle compact $K = (x, y)$ contenu dans $I$, et n’ayant aucun point intérieur commun avec $J_0$, on ait $\| \int_K f(t)\ dt \| \leq \varepsilon$.

En effet, comme $E$ est complet, le critère de Cauchy montre que, pour que l’intégrale $\int_I f(t)\ dt$ soit convergente, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un intervalle compact $J_0 = [\alpha, \beta]$ tel que, pour tout intervalle compact $J$ tel que $J_0 \subset J \subset I$, on ait $\| \int_J f(t)\ dt - \int_{J_0} f(t)\ dt \| \leq \varepsilon$. La proposition résultera donc du lemme suivant:

#### Lemme {#fvr-ii-s2-n1-lem-1 .statement}

Soit $J_0 = [\alpha, \beta]$ un intervalle compact contenu dans $I$. Pour qu’on ait $\| \int_J f(t)\ dt - \int_{J'} f(t)\ dt \| \leq \varepsilon$, pour tout couple d’intervalles compacts $J, J'$ contenus dans $I$ et contenant $J_0$, il faut que $\| \int_K f(t)\ dt \| \leq \varepsilon$, et il suffit que $\| \int_K f(t)\ dt \| \leq \varepsilon/2$, pour tout intervalle compact $K$ contenu dans $I$ et n’ayant aucun point intérieur commun avec $J_0$.

En effet, si pour $J_0 \subset J \subset I$ et $J_0 \subset J' \subset I$, on a
$$
\left\| \int_J f(t)\ dt - \int_{J'} f(t)\ dt \right\| \leq \varepsilon,
$$
on voit en particulier que, pour $x \leq y \leq \alpha$, ou pour $\beta \leq x \leq y$ ($x$ et $y$ dans $I$), on a $\| \int_x^y f(t)\ dt \| \leq \varepsilon$. Inversement, si $\| \int_K f(t)\ dt \| \leq \varepsilon/2$ pour tout intervalle compact $K \subset I$ tel que $K \cap J_0 = \varnothing$, et si $J = (x, y)$, $J' = (z, t)$ sont deux intervalles compacts contenus dans $I$ et contenant $J_0$, on a
$$
\left\| \int_J f(t)\ dt - \int_{J'} f(t)\ dt \right\| = \left\| \int_x^z f(t)\ dt + \int_z^t f(t)\ dt \right\| \leq \varepsilon,
$$
puisque
$$
x \leq \alpha \leq \beta \leq y \quad \text{et} \quad z \leq a \leq \beta \leq t.
$$

#### Exemple {#fvr-ii-s2-n1-exa-2 .statement}

Si l’intervalle $I$ est borné, et si $f$ est bornée dans $I$, l’intégrale $\int_I f(t)\ dt$ existe toujours, car d’après le th. de la moyenne, on a pour $y \leq \alpha \leq \beta \leq z$
$$
\left\| \int_y^\alpha f(t)\ dt \right\| \leq (\alpha - a) \sup_{x \in I} \| f(x) \|, \qquad \left\| \int_\beta^z f(t)\ dt \right\| \leq (b - \beta) \sup_{x \in I} \| f(x) \|
$$
et il suffit de prendre $\alpha - a$ et $b - \beta$ assez petits pour que le critère de Cauchy soit satisfait.

On notera que, dans ce cas, une primitive de $f$ dans $I$ n’a pas nécessairement de dérivée à droite (resp. à gauche) à l’origine (resp. l’extrémité) de $I$ (lorsque ce nombre est fini) contrairement à ce qui a lieu lorsque $I$ est compact et $f$ réglée dans $I$ (cf. II, p. 33, exerc. 1).

### 2. Intégrales de fonctions positives dans un intervalle non compact

#### Proposition 2 {#fvr-ii-s2-prop-2 .statement}

Soit $f$ une fonction numérique réglée et $\geq 0$ dans un intervalle $I \subset \mathbf{R}$, de bornes $a$ et $b$ ($a < b$). Pour que l’intégrale $\int_a^b f(t)\ dt$ existe, il faut et il suffit que l’ensemble des nombres $\int_J f(t) \, dt$ soit majoré, lorsque $J$ parcourt l’ensemble des intervalles compacts contenus dans $I$; l’intégrale $\int_a^b f(t) \, dt$ est alors la borne supérieure de l’ensemble des $\int_J f(t) \, dt$.

En effet, comme $f \geqslant 0$, la relation $J \subset J'$ entraîne
$$
\int_J f(t) \, dt \leqslant \int_{J'} f(t) \, dt;
$$
l’application $J \mapsto \int_J f(t) \, dt$ est donc croissante, et la proposition est une conséquence du théorème de la limite monotone (TG, IV, p. 18, th. 2).

Lorsque l’application $J \mapsto \int_J f(t) \, dt$ n’est pas bornée, elle a pour limite $+\infty$ suivant l’ordonné filtrant $\mathfrak{S}(I)$; on dit alors, par abuse de langage, que l’intégrale $\int_a^b f(t) \, dt$ est égale à $+\infty$. Les propriétés des intégrales établies au no 1 s’étendent (lorsqu’il s’agit de fonctions $\geqslant 0$) au cas où certaines des intégrales qui interviennent dans ces propriétés sont infinies, pourvu que les relations où elles figurent gardent un sens.

**Proposition 3 (principe de comparaison).** — *Soient $f$ et $g$ deux fonctions numériques réglées dans un intervalle $I \subset \mathbf{R}$, telles que $0 \leqslant f(x) \leqslant g(x)$ en tout point où $f$ et $g$ sont continues (cf. II, p. 11, prop. 6). Si l’intégrale de $g$ dans $I$ est convergente, il en est de même de l’intégrale de $f$ et on a $\int_I f(t) \, dt \leqslant \int_I g(t) \, dt$. En outre les deux intégrales ne peuvent être égales que si $f(x) = g(x)$ en tout point de $I$ où $f$ et $g$ sont continues.*

En effet, pour tout intervalle compact $J \subset I$, on a
$$
\int_J f(t) \, dt \leqslant \int_J g(t) \, dt;
$$
comme $\int_J g(t) \, dt \leqslant \int_I g(t) \, dt$, l’intégrale $\int_J f(t) \, dt$ est majorée, donc l’intégrale $\int_I f(t) \, dt$ est convergente; en outre, en passant à la limite, on a $\int_I f(t) \, dt \leqslant \int_I g(t) \, dt$. Supposons en outre que $f(x) < g(x)$ en un point $x \in I$ où $f$ et $g$ sont continues; il existe un intervalle compact $[c, d]$ contenu dans $I$, non réduit à un point et tel que $x \in [c, d]$; on a $\int_c^d f(t) \, dt < \int_c^d g(t) \, dt$ (II, p. 11, cor. 1), et comme d’autre part $\int_a^c f(t) \, dt \leqslant \int_a^c g(t) \, dt$ et $\int_d^b f(t) \, dt \leqslant \int_d^b g(t) \, dt$ d’après ce qui précède, on voit, en ajoutant membre à membre, qu’on a $\int_a^b f(t) \, dt < \int_a^b g(t) \, dt$.

Cette proposition fournit le moyen le plus fréquemment employé pour décider si une intégrale d’une fonction $f \geqslant 0$ est ou non convergente, en *comparant* $f$ à une fonction plus simple $g \geqslant 0$, dont on sait déjà si son intégrale est ou non convergente; nous verrons au chap. V comment peut se faire, dans les cas les plus usuels, la recherche de ces fonctions de comparaison, et nous en déduirons les critères d’application courante pour la convergence des intégrales et des séries.

### 3. Intégrales absolument convergentes

#### Définition 2 {#fvr-ii-s2-def-2 .statement}

On dit que l’intégrale d’une fonction $f$ réglée dans un intervalle $I \subset \mathbf{R}$ est absolument convergente, si l’intégrale de la fonction positive $\|f(x)\|$ est convergente.

#### Proposition 4 {#fvr-ii-s2-prop-4 .statement}

Si l’intégrale de $f$ dans $I$ est absolument convergente, elle est convergente, et on a
$$
\left\| \int_I f(t) \, dt \right\| \leq \int_I \|f(t)\| \, dt.
$$
En effet, pour tout intervalle compact $J \subset I$, on a (II, p. 12, formule (16))
$$
\left\| \int_J f(t) \, dt \right\| \leq \int_J \|f(t)\| \, dt.
$$
Si l’intégrale de la fonction positive $\|f(x)\|$ est convergente, pour tout $\varepsilon > 0$, il existe un intervalle compact $[\alpha, \beta]$ contenu dans $I$, tel que, pour tout intervalle compact $[x, y]$ contenu dans $I$ et n’ayant aucun point intérieur commun avec $[\alpha, \beta]$, on ait $\int_x^y \|f(t)\| \, dt \| \leq \varepsilon$ (II, p. 16, prop. 1); on en tire $\|\int_x^y f(t) \, dt\| \leq \varepsilon$, ce qui démontre la convergence de l’intégrale dans $I$ (II, p. 16, prop. 1); en passant à la limite dans (3), on en déduit alors l’intégalité (2).

#### Corollaire {#fvr-ii-s2-n3-cor-1 .statement}

Soient $E, F, G$ trois espaces normés complets sur $\mathbf{R}$, $(x, y) \mapsto [x, y]$ une application bilinéaire continue de $E \times F$ dans $G$. Soient $f, g$ deux fonctions réglées dans $I$, à valeurs dans $E$ et dans $F$ respectivement. Si $f$ est bornée dans $I$ et si l’intégrale de $g$ dans $I$ est absolument convergente, l’intégrale de $[f.g]$ dans $I$ est absolument convergente.

En effet, il existe un nombre $h > 0$ tel que l’on ait identiquement $\| [x.y] \| \leq h \|x\|.\|y\|$ (TG, IX, p. 35, th. 1); si on pose $= \sup_{x \in I} \|f(x)\|$, on a donc $\| [f(x).g(x)] \| \leq h k \|g(x)\|$ dans $I$; le principe de comparaison montre donc que l’intégrale de $[f.g]$ dans $I$ est absolument convergente, et on a, d’après (2),
$$
\left\| \int_I [f(t).g(t)] \, dt \right\| \leq h k \int_I \|g(t)\| \, dt.
$$

#### Remarque {#fvr-ii-s2-n3-rem-1 .statement}

Une intégrale peut être convergente sans l’être absolument; c’est ce que montre l’Exemple 3 de II, p. 14, lorsque la série de terme général $u_n$ est convergente sans être absolument convergente.

## EXERCICES {#fvr-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
