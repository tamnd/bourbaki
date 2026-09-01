---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: ÉTUDE LOCALE DES FONCTIONS
section: 1
section_title: Comparaison des fonctions dans un ensemble filtré
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0206-0215, 0253-0253
extraction: ocr
subsections:
    - "no": 1
      title: 'Relations de comparaison: I. Relations faibles'
      page: 2
      pdf_page: 207
    - "no": 2
      title: 'Relations de comparaison: II. Relations fortes'
      page: 5
      pdf_page: 210
    - "no": 3
      title: Changement de variables
      page: 7
      pdf_page: 212
    - "no": 4
      title: Relations de comparaison entre fonctions strictement positives
      page: 7
      pdf_page: 212
    - "no": 5
      title: Notations
      page: 9
      pdf_page: 214
statements: 47
exercises: 3
content_sha256: 4b278b611edbc903d308f669178aefc79766c85334861544840988b827a56395
---

## § 1. COMPARAISON DES FONCTIONS DANS UN ENSEMBLE FILTRÉ

Soit E un ensemble, filtré par un filtre de base $\mathfrak{F}$ (TG, I, p. 36); dans ce chapitre, nous considérerons des fonctions dont l’ensemble de définition est une partie de E appartenant à la base de filtre $\mathfrak{F}$ (partie dépendant de la fonction considérée) et qui prennent leurs valeurs, soit dans le corps $\mathbf{R}$ des nombres réels, soit plus généralement dans un espace vectoriel normé sur un corps valué (TG, IX, p. 32).

Dans les applications, E sera le plus souvent une partie d’un espace numérique $\mathbf{R}^n$, ou de la droite achevée $\overline{\mathbf{R}}$, et $\mathfrak{F}$ la trace sur E du filtre des voisinages d’un point adhérent à E, ou encore le filtre des complémentaires des ensembles relativement compacts dans E (« voisinages du point à l’infini »).

Il ne suffira pas en général de savoir qu’une telle fonction tend vers une limite donnée suivant $\mathfrak{F}$ pour pouvoir traiter tous les problèmes de « passage à la limite suivant $\mathfrak{F}$ » où interviennent des expressions formées avec cette fonction.

Par exemple, lorsque la variable réelle x tend vers $+\infty$, les trois fonctions $x$, $x^2$ et $\sqrt{x}$ tendent toutes trois vers $+\infty$, mais, des expressions.

$$
(x+1)^2 - x^2,\quad (x+1) - x,\quad \sqrt{x+1} - \sqrt{x}
$$

la première tend vers $+\infty$, la seconde vers 1, la troisième vers 0.

Il importe donc de connaître, non seulement la valeur limite d’une fonction suivant $\mathfrak{F}$ (lorsque cette limite existe), mais encore la « manière » dont la fonction tend vers sa limite; en d’autres termes, on est amené à opérer une classification dans l’ensemble des fonctions qui tendent vers une même limite.

### 1. Relations de comparaison: I. Relations faibles

Nous désignerons dans ce qui suit par V un espace vectoriel normé sur un corps valué K, par $\mathcal{H}(\mathfrak{F}, V)$ l’ensemble des fonctions à valeurs dans V, dont chacune est définie dans une partie de E appartenant à la base de filtre $\mathfrak{F}$. Les relations que nous allons définir entre de telles fonctions ont un caractère local relatif au filtre de base $\mathfrak{F}$: nous allons préciser ce qu’il faut entendre par là. Si f et g sont deux fonctions de $\mathcal{H}(\mathfrak{F}, V)$, rappelons que la relation « il existe un ensemble Z $\in \mathfrak{F}$ tel que f et g soient définies et égales dans Z » est une relation d’équivalence R_\infty dans $\mathcal{H}(\mathfrak{F}, V)$ (TG, I, p. 44). Cela étant, nous dirons qu’une relation S où figure une fonction f de $\mathcal{H}(\mathfrak{F}, V)$ est de caractère local (suivant $\mathfrak{F}$) relativement à f, si elle est compatible (en f) avec la relation d’équivalence R_\infty (E, II, p. 42); on sait que, si $\tilde{f}$ est le germe de f suivant $\mathfrak{F}$, classe de f modulo R_\infty (élément de l’ensemble quotient $\mathcal{H}_\infty(\mathfrak{F}, V) = \mathcal{H}(\mathfrak{F}, V)/R_\infty$), on déduit de S, par passage au quotient, une relation entre $\tilde{f}$ et les autres arguments de S, et que réciproquement, toute relation de cette nature définit une relation de caractère local relativement à f.

#### Exemple {#fvr-v-s1-n1-exa-9 .statement}

Si f et g sont deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, la relation « il existe un ensemble X $\in \mathfrak{F}$ tel que f et g soient définies dans X, et que $f(t) \leq g(t)$ pour tout $t \in X$ » est de caractère local relativement à f et g. On note $\tilde{f} \leq \tilde{g}$ la relation obtenue en passant au quotient (pour f et g); on remarquera que si $\tilde{f} \leq \tilde{g}$, il existe une fonction $f_1 \in \tilde{f}$ et une fonction $g_1 \in \tilde{g}$, définies dans E tout entier, et telles que $f_1(t) \leq g_1(t)$ pour tout $t \in E$.

#### Remarque 1 {#fvr-v-s1-n1-rem-1 .statement}

Soient $V_i$ (1 $\leq i \leq n$) n espaces vectoriels normés sur K, $\varphi$ une fonction définie dans $V_1 \times V_2 \times \cdots \times V_n$, à valeurs dans V par passage aux quotients suivant R_\infty, la fonction $\varphi$ définit donc une application de
$$
\mathcal{H}_\infty(\mathfrak{F}, V_1) \times \cdots \times \mathcal{H}_\infty(\mathfrak{F}, V_n)
$$
dans $\mathcal{H}_\infty(\mathfrak{F}, V)$, que l’on notera le plus souvent $\varphi(\tilde{f}_1, \ldots, \tilde{f}_n)$ (TG, I xla, p. 45). Par exemple en prenant pour $\varphi$ les applications $(x, y) \mapsto x + y$ et $x \mapsto x\lambda$ ($\lambda \in K$), on définit ainsi, pour deux germes quelconques $\tilde{f}, \tilde{g}$ de $\mathcal{H}_\infty(\mathfrak{F}, V)$, les éléments $\tilde{f} + \tilde{g}$ et $\tilde{f}\lambda$ et on vérifie aussitôt que les lois de composition $(\tilde{f}, \tilde{g}) \mapsto \tilde{f} + \tilde{g}$ et $(\lambda, \tilde{f}) \mapsto \tilde{f}\lambda$ définissent sur $\mathcal{H}_\infty(\mathfrak{F}, V)$ une structure d’espace vectoriel sur le corps K; dans cet espace, $\tilde{0}$ est la classe formée des fonctions égales à 0 dans un ensemble de $\mathfrak{F}$, et $-\tilde{f}$ est la classe formée des fonctions égales à $-f$ dans un ensemble de $\mathfrak{F}$. De même, si V est une algèbre sur K, on définit sur $\mathcal{H}_\infty(\mathfrak{F}, V)$ une seconde loi de composition interne $(\tilde{f}, \tilde{g}) \mapsto \tilde{f}\tilde{g}$ en prenant $\varphi(x, y) = xy$; avec les deux lois précédentes, elle définit sur $\mathcal{H}_\infty(\mathfrak{F}, V)$ une structure d’algèbre sur le corps K; si V admet un élément unité e, $\mathcal{H}_\infty(\mathfrak{F}, V)$ admettra pour élément unité la classe $\tilde{e}$, formée des fonctions égales à e dans un ensemble de $\mathfrak{F}$; pour que $\tilde{f}$ soit inversible dans $\mathcal{H}_\infty(\mathfrak{F}, V)$, il faut et il suffit que, pour une fonction $f \in \tilde{f}$, il existe $Z \in \mathfrak{F}$ tel que $f(t)$ soit inversible dans V pour tout $t \in Z$ (auquel cas cette condition est vérifiée pour toute fonction de la classe $\tilde{f}$).

#### Remarque 2 {#fvr-v-s1-n1-rem-2 .statement}

Avec les mêmes notations, soit $\psi$ une application d’une partie de $\prod_{i=1}^n V_i$ dans V; nous désignerons par $\psi(f_1, f_2, \ldots, f_n)$ la fonction égale à $\psi(f_1(t), \ldots, f_n(t))$ en tout point $t \in E$ où les $f_i(t)$ sont définis et où le point $(f_i(t))$ appartient à l’ensemble où est définie $\psi^1$. Par exemple, $f + g$ est la fonction égale à $f(t) + g(t)$ en tout point $t \in E$ où $f$ et $g$ sont toutes deux définies. On observera que l’application $(\mathbf{f}, \mathbf{g}) \mapsto \mathbf{f} + \mathbf{g}$ n’est pas une loi de groupe dans $\mathcal{H}(\mathfrak{F}, V)$, car si $\mathbf{f}$ n’est pas définie dans $E$ tout entier, il n’existe pas de fonction $\mathbf{g} \in \mathcal{H}(\mathfrak{F}, V)$ telle que $\mathbf{f} + \mathbf{g} = 0$.

#### Définition 1 {#fvr-v-s1-def-1 .statement}

Étant données deux fonctions numériques $f, g$ appartenant à $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ et qui sont $\geqslant 0$ dans un ensemble de $\mathfrak{F}$, on dit que $f$ est dominée par $g$, ou que $g$ domine $f$ (suivant $\mathfrak{F}$), et on écrit $f \leqslant g$ ou $g \geqslant f$, s’il existe un ensemble $X \in \mathfrak{F}$ et un nombre $k > 0$ tels que $f(t) \leqslant k.g(t)$ pour tout $t \in X$ (autrement dit, s’il existe $k > 0$ tel que $\tilde{f} \leqslant k.\tilde{g}$).

Étant données deux espaces normés $V_1, V_2$, et deux fonctions $\mathbf{f}_1, \mathbf{f}_2$ appartenant respectivement à $\mathcal{H}(\mathfrak{F}, V_1)$ et $\mathcal{H}(\mathfrak{F}, V_2)$ on dit que $\mathbf{f}_1$ est dominée par $\mathbf{f}_2$ (suivant $\mathfrak{F}$) et on écrit $\mathbf{f}_1 \leqslant \mathbf{f}_2$ ou $\mathbf{f}_2 \geqslant \mathbf{f}_1$ si on a $\| \mathbf{f}_1 \| \leqslant \| \mathbf{f}_2 \|$.

La relation $\mathbf{f}_1 \leqslant \mathbf{f}_2$ est évidemment de caractère local en $\mathbf{f}_1$ et $\mathbf{f}_2$; elle est donc équivalente à la relation $\tilde{\mathbf{f}}_1 \leqslant \tilde{\mathbf{f}}_2$ qui s’en déduit par passage aux quotients. Lorsque $f$ et $g$ sont deux fonctions numériques, on aura soin de ne pas confondre les relations $\tilde{f} \leqslant \tilde{g}$ et $\tilde{f} \leqslant \tilde{g}$.

On notera que pour tout scalaire $\lambda \neq 0$, la relation $\mathbf{f}_1 \leqslant \mathbf{f}_2 \lambda$ est équivalente à $\mathbf{f}_1 \leqslant \mathbf{f}_2$. Si $\mathbf{f}_1 \leqslant \mathbf{f}_2$, il existe un ensemble $X \in \mathfrak{F}$ tel que, pour tout point $x \in X$ où $\mathbf{f}_2(x) = 0$, on ait $\mathbf{f}_1(x) = 0$.

#### Exemple 1 {#fvr-v-s1-n1-exa-1 .statement}

La relation $\mathbf{f} \leqslant 1$ signifie que $\mathbf{f}$ est bornée dans un ensemble de $\mathfrak{F}$.

#### Exemple 2 {#fvr-v-s1-n1-exa-2 .statement}

Pour toute fonction $\mathbf{f}$ de $\mathcal{H}(\mathfrak{F}, V)$ et tout scalaire $\lambda \neq 0$, on a $\mathbf{f} \leqslant \mathbf{f}\lambda$.

#### Exemple 3 {#fvr-v-s1-n1-exa-3 .statement}

Lorsque $x$ tend vers $+\infty$, on a $\sin^2 x \leqslant \sin x$.

#### Exemple 4 {#fvr-v-s1-n1-exa-4 .statement}

Lorsque $(x, y)$ tend vers $(0, 0)$ dans $\mathbf{R}^2$, on a
$$
xy \leqslant x^2 + y^2.
$$

Les propositions suivantes sont des conséquences immédiates de la déf. 1:

#### Proposition 1 {#fvr-v-s1-prop-1 .statement}

Si $f, g, h$ sont trois fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, les relations $f \leqslant g$ et $g \leqslant h$ entraînent $f \leqslant h$.

#### Proposition 2 {#fvr-v-s1-prop-2 .statement}

Soient $\mathbf{f}_1, \mathbf{f}_2$ deux fonctions de $\mathcal{H}(\mathfrak{F}, V)$ et $g$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. Les relations $\mathbf{f}_1 \leqslant g$ et $\mathbf{f}_2 \leqslant g$ entraînent $\mathbf{f}_1 + \mathbf{f}_2 \leqslant g$.

En outre:

#### Proposition 3 {#fvr-v-s1-prop-3 .statement}

Soient $V_1, V_2, V$ trois espaces normés sur un même corps valué, $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x} \cdot \mathbf{y}]$ une application bilinéaire continue de $V_1 \times V_2$ dans $V$. Si $\mathbf{f}_1$ et $\mathbf{f}_2$ sont des fonctions de $\mathcal{H}(\mathfrak{F}, V_1)$ et $\mathcal{H}(\mathfrak{F}, V_2)$ respectivement, $g_1, g_2$ deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ telles que $\mathbf{f}_1 \leqslant g_1$ et $\mathbf{f}_2 \leqslant g_2$, on a $[\mathbf{f}_1 \cdot \mathbf{f}_2] \leqslant g_1 g_2$.

En effet (TG, IX, p. 35, th.1), il existe un nombre $a > 0$ tel que $\| \mathbf{f}_1 \cdot \mathbf{f}_2 \| \leqslant a \| \mathbf{f}_1 \| \cdot \| \mathbf{f}_2 \|$.

1 En particulier, dans toute la suite, pour une fonction $\mathbf{f}$ de $\mathcal{H}(\mathfrak{F}, V)$, nous désignerons par $\| \mathbf{f} \|$ la fonction $t \mapsto \| \mathbf{f}(t) \|$, appartenant à $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ et définie dans le même ensemble que $\mathbf{f}$: nous signalons expressément que, dans ce chapitre, $\| \mathbf{f} \|$ est une fonction et non un nombre.

#### Corollaire {#fvr-v-s1-n1-cor-1 .statement}

Si V est une algèbre normée, $f_1, f_2$ deux fonctions de $\mathcal{H}(\mathfrak{F}, V)$, $g_1, g_2$ deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, les relations $f_1 \preccurlyeq g_1, f_2 \preccurlyeq g_2$ entraînent $f_1 f_2 \preccurlyeq g_1 g_2$.

La relation $\mathbf{f} \preccurlyeq \mathbf{g}$ entre fonctions de $\mathcal{H}(\mathfrak{F}, V)$ est transitive d’après la prop 1 ; comme elle est réflexive, la relation « $\mathbf{f} \preccurlyeq \mathbf{g}$ et $\mathbf{g} \preccurlyeq \mathbf{f}$ » est une relation d’équivalence dans $\mathcal{H}(\mathfrak{F}, V)$ (E, II, p. 40).

#### Définition 2 {#fvr-v-s1-def-2 .statement}

Étant données deux fonctions $\mathbf{f}, \mathbf{g}$ de $\mathcal{H}(\mathfrak{F}, V)$, on dit que $\mathbf{f}$ et $\mathbf{g}$ sont semblables (suivant $\mathfrak{F}$) et on écrit $\mathbf{f} \asymp \mathbf{g}$ si on a $\mathbf{f} \preccurlyeq \mathbf{g}$ et $\mathbf{g} \preccurlyeq \mathbf{f}$.

Pour tout scalaire $\lambda \neq 0$, la relation $\mathbf{f} \asymp \mathbf{g}$ est équivalente à $\mathbf{f} \asymp \mathbf{g} \lambda$. Elle entraîne l’existence d’un ensemble $X \in \mathfrak{F}$ tel que la partie de $X$ formée des points où $\mathbf{f}(x) = 0$ soit identique à la partie de $X$ formée des points où $\mathbf{g}(x) = 0$.

#### Exemple 5 {#fvr-v-s1-n1-exa-5 .statement}

Pour une fonction numérique $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$, la relation $f \asymp 1$ signifie qu’il existe deux nombres $a > 0, b > 0$ tels que $a \leq |f(x)| \leq b$ dans un ensemble de $\mathfrak{F}$, ou encore que la fonction $\log |f|$ est bornée dans un ensemble de $\mathfrak{F}$ : on dit alors que $f$ est logarithmiquement bornée dans un ensemble de $\mathfrak{F}$.

#### Exemple 6 {#fvr-v-s1-n1-exa-6 .statement}

Soit $V$ un espace normé sur un corps valué non discret $K$, et soit $\mathbf{f}(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ un polynôme par rapport à $x \in K$, à coefficients dans $V$, tel que $a_0 \neq 0$. Pour tout vecteur $\mathbf{b} \neq 0$, on a $\mathbf{f}(x) \asymp \mathbf{b} x^n$ lorsque $|x|$ tend vers $+\infty$.

#### Exemple 7 {#fvr-v-s1-n1-exa-7 .statement}

Nous avons vu qu’on a $\sin^2 x \preccurlyeq \sin x$ lorsque $x$ tend vers $+\infty$, mais on n’a pas $\sin^2 x \asymp \sin x$, bien que ces deux fonctions s’annullent aux mêmes points.

#### Exemple 8 {#fvr-v-s1-n1-exa-8 .statement}

On a $x^2 + xy + y^2 \asymp x^2 + y^2$ lorsque $(x, y)$ tend vers $(0, 0)$ dans $\mathbf{R}^2$, mais non $xy \asymp x^2 + y^2$.

Il résulte aussitôt de la prop. 3 de V, p. 3, que si $f_1, f_2, g_1, g_2$ sont des fonctions de $\mathcal{H}(\mathfrak{F}, K)$ (K corps valué quelconque), les relations $f_1 \asymp g_1$ et $f_2 \asymp g_2$ entraînent $f_1 f_2 \asymp g_1 g_2$.

On notera par contre que les relations $f_1 \asymp g_1, f_2 \asymp g_2$ n’entraînent pas $f_1 + f_2 \asymp g_1 + g_2$, comme le montre l’exemple où $f_1(x) = g_1(x) = x^2, f_2(x) = -(x^2 + x), g_2(x) = -(x^2 - 1)$, $x$ réel tendant vers $+\infty$.

Les relations de comparaison $\mathbf{f} \preccurlyeq \mathbf{g}$, $\mathbf{f} \asymp \mathbf{g}$ sont dites relations faibles. On dit que deux fonctions $\mathbf{f}, \mathbf{g}$ de $\mathcal{H}(\mathfrak{F}, V)$ sont faiblement comparables si elles vérifient l’une (au moins) des deux relations $\mathbf{f} \preccurlyeq \mathbf{g} ; \mathbf{g} \preccurlyeq \mathbf{f}$.

#### Remarque 3 {#fvr-v-s1-n1-rem-3 .statement}

Deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ ne sont pas nécessairement faiblement comparables, comme le montre l’exemple des fonctions 1 et $x \sin x$ lorsque $x$ tend vers $+\infty$.

#### Remarque 4 {#fvr-v-s1-n1-rem-4 .statement}

Désignons par $R_0$ la relation $\mathbf{f} \asymp \mathbf{g}$ dans $(\mathcal{H}(\mathfrak{F}, V), \mathcal{H}_0(\mathfrak{F}, V))$, et par $\mathcal{H}_0(\mathfrak{F}, V)$ l’ensemble quotient $\mathcal{H}(\mathfrak{F}, V)/R_0$; on notera que la relation $R_\infty$ entraîne $R_0$. Par passage au quotient, la relation $\mathbf{f} \preccurlyeq \mathbf{g}$ donne, d’après la prop. 1 de V, p. 3, une relation d’ordre dans $\mathcal{H}_0(\mathfrak{F}, V)$ (E, III, p. 3) ; l’exemple qui précède prouve que $\mathcal{H}_0(\mathfrak{F}, V)$ n’est pas totalement ordonné par cette relation.

### 2. Relations de comparaison: II. Relations fortes

#### Définition 3 {#fvr-v-s1-def-3 .statement}

Étant données deux fonctions numériques $f, g$ appartenant à $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ et qui sont $\geqslant 0$ dans un ensemble de $\mathfrak{F}$, on dit que $f$ est négligeable devant $g$, ou que $g$ est prépondérante sur $f$ (suivant $\mathfrak{F}$), et on écrit $f \ll g$ ou $g \gg f$ si, pour tout $\varepsilon > 0$, il existe un ensemble $X \in \mathfrak{F}$ tel que $f(t) \leqslant \varepsilon g(t)$ pour tout $t \in X$.

Étant donnés deux espaces normés $V_1, V_2$, et deux fonctions $\mathbf{f}_1, \mathbf{f}_2$ appartenant respectivement à $\mathcal{H}(\mathfrak{F}, V_1)$ et $\mathcal{H}(\mathfrak{F}, V_2)$, on dit que $\mathbf{f}_1$ est négligeable devant $\mathbf{f}_2$ (suivant $\mathfrak{F}$) et on écrit $\mathbf{f}_1 \ll \mathbf{f}_2$ ou $\mathbf{f}_2 \gg \mathbf{f}_1$ si on a $\| \mathbf{f}_1 \| \ll \| \mathbf{f}_2 \|$.

Pour tout scalaire $\lambda \neq 0$, la relation $\mathbf{f}_1 \ll \mathbf{f}_2 \lambda$ est équivalente à $\mathbf{f}_1 \ll \mathbf{f}_2$. La relation $\mathbf{f}_1 \ll \mathbf{f}_2$ entraîne $\mathbf{f}_1 \ll \mathbf{f}_2$, mais ne lui est pas équivalente.

On notera que la relation $\mathbf{f}_1 \leqslant \mathbf{f}_2$ n’entraîne nullement la relation « $\mathbf{f}_1 \leqslant \mathbf{f}_2$ ou $\mathbf{f}_1 \asymp \mathbf{f}_2$ » : on a $\sin x \leqslant 1$ lorsque $x$ tend vers $+\infty$, mais aucune des relations $\sin x \leqslant 1$, $\sin x \asymp 1$ n’est vraie.

#### Exemple 1 {#fvr-v-s1-n2-exa-1 .statement}

La relation $\mathbf{f} \ll 1$ signifie que $\mathbf{f}$ tend vers 0 suivant $\mathfrak{F}$.

#### Exemple 2 {#fvr-v-s1-n2-exa-2 .statement}

Lorsque $\alpha$ et $\beta$ sont deux nombres réels tels que $\alpha < \beta$, on a $x^\alpha \ll x^\beta$ lorsque $x$ tend vers $+\infty$. De même, lorsque $m$ et $n$ sont deux entiers rationnels tels que $m < n$, on a $z^m \ll z^n$ lorsque le nombre complexe $z$ tend vers $\infty$.

#### Exemple 3 {#fvr-v-s1-n2-exa-3 .statement}

Lorsque $x$ tend vers $+\infty$, on a $x^n \ll e^x$ pour tout entier $n$ (III, p. 16).

#### Exemple 4 {#fvr-v-s1-n2-exa-4 .statement}

Dans $\mathbf{R}^2$, on a, lorsque $(x, y)$ tend vers $(0, 0)$
$$
x^2 + y^2 \ll |x| + |y|.
$$

Les propositions suivantes se déduisent immédiatement de la déf. 3:

#### Proposition 4 {#fvr-v-s1-prop-4 .statement}

Si $f, g, h$ sont trois fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, les relations $f \leqslant g$ et $g \ll h$ (resp. $f \ll g$ et $g \leqslant h$) entraînent $f \ll h$.

#### Proposition 5 {#fvr-v-s1-prop-5 .statement}

Soient $\mathbf{f}_1, \mathbf{f}_2$ deux fonctions de $\mathcal{H}(\mathfrak{F}, V)$, $g$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. Les relations $\mathbf{f}_1 \ll g$ et $\mathbf{f}_2 \ll g$ entraînent $\mathbf{f}_1 + \mathbf{f}_2 \ll g$.

D’autre part, le même raisonnement que pour la prop. 3 de V, p. 3, montre que:

#### Proposition 6 {#fvr-v-s1-prop-6 .statement}

Avec les notations de la prop. 3, les relations $\mathbf{f}_1 \ll g_1$ et $\mathbf{f}_2 \ll g_2$ (resp. $\mathbf{f}_1 \leqslant g_1$ et $\mathbf{f}_2 \leqslant g_2$) entraînent $[\mathbf{f}_1, \mathbf{f}_2] \ll g_1 g_2$.

La prop. 4 montre que la relation $\mathbf{f} \ll \mathbf{g}$ entre fonctions de $\mathcal{H}(\mathfrak{F}, V)$ est transitive; mais elle n’est pas réflexive: de façon précise, la relation $\mathbf{f} \ll \mathbf{f}$ entraîne que $\mathbf{f}$ est nulle dans un ensemble de $\mathfrak{F}$ (autrement dit, $\mathbf{f}$ est équivalente à 0 modulo $R_\infty$); en effet, pour un $\varepsilon$ tel que $0 < \varepsilon < 1$ il existe $X \in \mathfrak{F}$ tel que $\| \mathbf{f}(x) \| \leqslant \varepsilon \| \mathbf{f}(x) \|$ pour tout $x \in X$, ce qui n’est possible que si $\mathbf{f}(x) = 0$ pour tout $x \in X$. Il en résulte que la relation « $\mathbf{f} \ll \mathbf{g}$ et $\mathbf{g} \ll \mathbf{f}$ » est transitive et symétrique, mais non réflexive: ce n’est donc pas une relation d’équivalence (elle signifie qu’il existe un ensemble $X \in \mathfrak{F}$ tel que $\mathbf{f}(x) = \mathbf{g}(x) = 0$ pour tout $x \in X$).

#### Proposition 7 {#fvr-v-s1-prop-7 .statement}

Si $f$ et $g$ sont deux fonctions de $\mathcal{H}(\mathfrak{F}, V)$, la relation $f - g \ll f$ est équivalente à $f - g \ll g$.

En effet, $f - g \ll f$ signifie que, pour tout $\varepsilon > 0$, il existe $X \in \mathfrak{F}$ tel que $\|f(x) - g(x)\| \leq \varepsilon \|f(x)\|$ pour tout $x \in X$. On en tire $(1 - \varepsilon) \|f(x)\| \leq \|g(x)\|$, et par suite $f \preceq g$, d’où (p. 5, prop. 4) $f - g \ll g$.

#### Corollaire {#fvr-v-s1-n2-cor-1 .statement}

La relation $f - g \ll f$ est une relation d’équivalence dans $\mathcal{H}(\mathfrak{F}, V)$.

En effet, si $f - g \ll f$ et $g - h \ll g$, on a $f - g \ll g$, d’où (V, p. 5, prop. 5) $f - h \ll g$, et par suite, comme $g \preceq f$, $f - h \ll f$, ce qui montre que la relation considérée est transitive; elle est symétrique d’après la prop. 7 et est évidemment réflexive, d’où le corollaire.

#### Définition 4 {#fvr-v-s1-def-4 .statement}

Étant données deux fonctions $f, g$ de $\mathcal{H}(\mathfrak{F}, V)$, on dit que $f$ et $g$ sont équivalentes (suivant $\mathfrak{F}$) et on écrit $f \sim g$ si on a $f - g \ll f$.

La relation $f \sim g$ entraîne $f \succeq g$, mais ne lui est pas équivalente.

#### Exemple 5 {#fvr-v-s1-n2-exa-5 .statement}

Si $a$ est une fonction constante et $\neq 0$ dans $E$, la relation $f \sim a$ signifie que $f$ tend vers $a$ suivant $\mathfrak{F}$.

#### Exemple 6 {#fvr-v-s1-n2-exa-6 .statement}

Soit $V$ un espace normé sur un corps valué non discret $K$, et soit $f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ un polynôme par rapport à $x \in K$, à coefficients dans $V$, tel que $a_0 \neq 0$. On a $f(x) \sim a_0 x^n$ lorsque $|x|$ tend vers $+\infty$.

#### Exemple 7 {#fvr-v-s1-n2-exa-7 .statement}

Lorsque $x$ réel tend vers $+\infty$, on a $\left(1 + \frac{1}{x}\right) \sin x \sim \sin x$.

#### Exemple 8 {#fvr-v-s1-n2-exa-8 .statement}

Lorsque la variable complexe $z$ tend vers $0$, on a $e^z - 1 \sim z$. Plus généralement, si $V$ est un espace normé sur un corps valué $K$, $f$ une fonction définie dans un voisinage de $x_0 \in K$, à valeurs dans $V$, et admettant au point $x_0$ une dérivée $f'(x_0) \neq 0$, on a, lorsque $x$ tend vers $x_0$, $f(x) - f(x_0) \sim f'(x_0)(x - x_0)$ (I, p. 2, déf. 1).

#### Exemple 9 {#fvr-v-s1-n2-exa-9 .statement}

Lorsque $(x, y)$ tend vers $(0, 0)$ dans $\mathbf{R}^2$, on a
$$
\sqrt{\sin^2 x + \sin^2 y} \sim \sqrt{x^2 + y^2}.
$$

#### Exemple 10 {#fvr-v-s1-n2-exa-10 .statement}

Soit $f(x, y)$ un polynôme à coefficients réels par rapport à deux variables réelles $x, y$, n’ayant pas de terme constant. Si, lorsque $x$ tend vers $0$ en restant $> 0$, il existe une fonction $\varphi(x)$ continue dans un intervalle $(0, a)$ et telle que $\varphi(0) = 0$ et $f(x, \varphi(x)) = 0$ pour $0 \leq x \leq a$, on peut montrer qu’il existe un nombre rationnel $r$ et un nombre réel $\lambda \neq 0$ tels que $\varphi(x) \sim \lambda x^r$ (V, p. 48, exerc. 3).

#### Exemple 11 {#fvr-v-s1-n2-exa-11 .statement}

Pour tout $x > 0$, soit $\pi(x)$ le nombre des nombres premiers qui sont $\leq x$; on a démontré que, lorsque $x$ tend vers $+\infty$, on a $\pi(x) \sim x/\log x^2$.

#### Remarque {#fvr-v-s1-n2-rem-2 .statement}

On notera que la relation $f \sim g$ ne signifie nullement que la différence $f - g$ tende vers 0 suivant $\mathfrak{F}$; cette différence peut même être non bornée, comme le montre l’exemple $x^2 + x \sim x^2$, $x$ tendant vers $+\infty$.

#### Proposition 8 {#fvr-v-s1-prop-8 .statement}

Soient $K$ un corps valué, $f_1, f_2, g_1, g_2$ quatre fonctions de $\mathcal{H}(\mathfrak{F}, K)$; les relations $f_1 \sim g_1$ et $f_2 \sim g_2$ entraînent $f_1 f_2 \sim g_1 g_2$.

1 Voir par exemple A. E. Ingham, The distribution of prime numbers (Cambridge tracts, n° 30), Cambridge University Press, 1932.

En effet, on a $f_1 f_2 - g_1 g_2 = f_1 (f_2 - g_2) + (f_1 - g_1) g_2$; comme $f_1 \ll g_1$, $f_1 - g_1 \ll g_1$ et $f_2 - g_2 \ll g_2$, on a bien $f_1 f_2 - g_1 g_2 \ll g_1 g_2$ (V, p. 5, prop. 4 et 5).

Par contre, nous avons donné dans V, p. 4, un exemple où on avait $f_1 = g_1$, $f_2 \sim g_2$, mais où la relation $f_1 + f_2 \asymp g_1 + g_2$ n’était pas vraie (ni a fortiori
$$
f_1 + f_2 \sim g_1 + g_2.
$$

Les relations de comparaison $\mathbf{f} \ll \mathbf{g}$, $\mathbf{f} \sim \mathbf{g}$ sont dites relations fortes. Deux fonctions $\mathbf{f}, \mathbf{g}$ de $\mathcal{H}(\mathfrak{F}, V)$ sont dites comparables (ou fortement comparables lorsqu’on veut éviter des confusions possibles) si elles vérifient l’une des trois relations: $\mathbf{f} \ll \mathbf{g}$, $\mathbf{f} \gg \mathbf{g}$, ou « il existe $\lambda \neq 0$ tel que $\mathbf{f} \sim \mathbf{g} \lambda$ ».

#### Remarque 1 {#fvr-v-s1-n2-rem-1 .statement}

Deux fonctions peuvent être faiblement comparables sans être fortement comparables, par exemple les fonctions 1 et sin x lorsque x tend vers $+\infty$.
2) La définition des relations de comparaison $\mathbf{f}_1 \leqslant \mathbf{f}_2$ et $\mathbf{f}_1 \ll \mathbf{f}_2$ ne fait intervenir qu’en apparence les normes sur les espaces $V_1, V_2$ où $\mathbf{f}_1$ et $\mathbf{f}_2$ prennent respectivement leurs valeurs; elle ne dépend en réalité que des topologies de $V_1$ et $V_2$, car les relations $\mathbf{f}_1 \leqslant \mathbf{f}_2^2$ et $\mathbf{f}_1 \ll \mathbf{f}_2$ sont remplacées par des relations équivalentes lorsqu’on remplace la norme sur $V_1$ ou $V_2$ par une norme équivalente (TG, IX, p. 32, def. 7).

### 3. Changement de variables

Soit $\varphi$ une application d’un ensemble $E'$ dans $E$, telle que $\varphi^{-1}(\mathfrak{F})$ soit une base de filtre sur $E'$. Il est clair que si $\mathbf{f}_1, \mathbf{f}_2$ sont des fonctions de $\mathcal{H}(\mathfrak{F}, V_1)$ et $\mathcal{H}(\mathfrak{F}, V_2)$ respectivement, les fonctions $\mathbf{f}_1 \circ \varphi, \mathbf{f}_2 \circ \varphi$ appartiennent respectivement à $\mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_1)$ et $\mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_2)$, et que la relation $\mathbf{f}_1 \leqslant \mathbf{f}_2$ (resp. $\mathbf{f}_1 \ll \mathbf{f}_2$) est équivalente à $\mathbf{f}_1 \circ \varphi \leqslant \mathbf{f}_2 \circ \varphi$ (resp. $\mathbf{f}_1 \circ \varphi \ll \mathbf{f}_2 \circ \varphi$).

### 4. Relations de comparaison entre fonctions strictement positives

Soit $g$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, strictement positive dans un ensemble de $\mathfrak{F}$. Les relations de comparaison où figure $g$ peuvent alors se formuler d’une autre manière: la relation $\mathbf{f} \ll g$ équivaut à dire que la fonction $\| \mathbf{f} \|/g$ (qui est définie dans un ensemble de $\mathfrak{F}$) est bornée dans un ensemble de $\mathfrak{F}$; la relation $\mathbf{f} \ll g$ équivaut à dire que $\| \mathbf{f} \|/g$ tend vers 0 suivant $\mathfrak{F}$. Si $f$ est une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, la relation $f \asymp g$ signifie que $f/g$ est logarithmiquement bornée dans un ensemble de $\mathfrak{F}$, et la relation $f \sim g$, que $f/g$ tend vers 1 suivant $\mathfrak{F}$. Si $f$ est une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ positive dans un ensemble de $\mathfrak{F}$, dire que $f$ et $g$ sont comparables signifie donc que $f/g$ tend vers une limite (finie ou égale à $+\infty$) suivant $\mathfrak{F}$.

#### Proposition 9 {#fvr-v-s1-prop-9 .statement}

Soient f et g deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ strictement positives dans un ensemble de $\mathfrak{F}$. Pour que f et g soient comparables, il faut et il suffit que pour tout nombre $t \geqslant 0$, sauf un au plus, la fonction $f - tg$ garde un signe constant$^1$ dans un ensemble de $\mathfrak{F}$.

La condition est nécessaire. En effet, si $f \ll g$, on a $f - tg \sim -tg$ sauf pour $t = 0$, donc $f - tg$ est strictement négative dans un ensemble de $\mathfrak{F}$, sauf pour $t = 0$; si $f \gg g$, $f - tg$ est strictement positive dans un ensemble de $\mathfrak{F}$ pour tout $t$; enfin, si $f \sim k.g$ ($k$ constante > 0), $f - tg \sim (k - t)g$ sauf pour $t = k$, donc, sauf peut-être pour $t = k$, $f - tg$ a le signe de $k - t$ dans un ensemble de $\mathfrak{F}$.

La condition est suffisante. En effet, supposons que le rapport $f/g$ ait deux valeurs d’adhérence distinctes $\alpha < \beta$ suivant $\mathfrak{F}$. Pour tout nombre $t$ tel que $\alpha < t < \beta$, il existe alors dans tout ensemble $X \in \mathfrak{F}$, deux points $x_1, x_2$ tels que $f(x_1)/g(x_1) < t$ et $f(x_2)/g(x_2) > t$; donc $f(x) - tg(x)$ ne garde pas un signe constant dans $X$; nous arrivons à une conclusion incompatible avec l’hypothèse. Il s’ensuit que $f/g$ n’a qu’une seule valeur d’adhérence (finie ou infinie) suivant le filtre de base $\mathfrak{F}$, et par suite (TG, I, p. 60, corollaire) a pour limite cette valeur suivant $\mathfrak{F}$.

#### Proposition 10 {#fvr-v-s1-prop-10 .statement}

Soient f et g deux fonctions de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ strictement positives dans un ensemble de $\mathfrak{F}$; pour tout $\alpha$ réel et $\neq 0$, la relation $f \asymp g$ (resp. $f \sim g$) est équivalente à $f^\alpha \asymp g^\alpha$ (resp. $f^\alpha \sim g^\alpha$); si $\alpha > 0$, la relation $f \ll g$ (resp. $f \ll g$) est équivalente à $f^\alpha \ll g^\alpha$ (resp. $f^\alpha \ll g^\alpha$); si $\alpha < 0$, elle est équivalente à $f^\alpha \gg g^\alpha$ (resp. $f^\alpha \gg g^\alpha$).

Les démonstrations sont immédiates.

On notera que dans $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, l’ensemble $\Gamma$ des fonctions strictement positives dans un ensemble de $\mathfrak{F}$ est tel que $\Gamma/\mathbf{R}_+$ soit un groupe multiplicatif $\Gamma_\infty$ dans $\mathcal{H}_\infty(\mathfrak{F}, \mathbf{R})$; $\Gamma/\mathbf{R}_0$ est identique au groupe quotient de $\Gamma_\infty$ par le sous-groupe des classes (mod. $\mathbf{R}_+$) des fonctions de $\Gamma$ logarithmiquement bornées; sur $\Gamma/\mathbf{R}_0$, la relation d’ordre déduite de la relation $f \ll g$ par passage aux quotients est compatible avec la structure de groupe de $\Gamma/\mathbf{R}_0$, et en fait donc un groupe ordonné.

#### Proposition 11 {#fvr-v-s1-prop-11 .statement}

Soit g une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ telle que $\lim_{x \to \mathfrak{F}} g = +\infty$; la relation $f \ll g$ entraîne $e^f \ll e^g$; la relation $f \sim g$ entraîne $\log f \sim \log g$.

En effet, si $f \ll g, f - g = g \left( \frac{f}{g} - 1 \right)$ tend vers $-\infty$ suivant $\mathfrak{F}$. De même, si $f \sim g$, on a $\log f = \log g + \log \frac{f}{g}$, donc $\log f - \log g$ tend vers 0, et il en est de même de $\frac{\log f}{\log g} - 1 = \frac{\log f - \log g}{\log g}$.

Par contre, on notera que la relation $f \sim g$ n’entraîne pas $e^f \sim e^g$, ni même $e^f \asymp e^g$, comme le montre l’exemple où $f(x) = x^2, g(x) = x^2 + x$, $x$ tendant vers $+\infty$; de même, la relation $f \ll g$ n’entraîne pas $\log f \ll \log g$, comme le montre l’exemple où $f(x) = x, g(x) = x^2, x$ tendant vers $+\infty$.

$^1$ On rappelle qu’on a défini le signe $\operatorname{sgn} x$ d’un nombre réel $x$ comme égal à $+1$ si $x > 0$, à $-1$ si $x < 0$, à 0 si $x = 0$ (TG, IV, p. 12). Dire qu’une fonction numérique garde un signe constant dans un ensemble signifie donc, soit qu’elle est $> 0$ en tout point de cet ensemble, soit qu’elle est $< 0$ en tout point de l’ensemble, soit enfin qu’elle est identiquement nulle dans l’ensemble.

#### Définition 5 {#fvr-v-s1-def-5 .statement}

Soit g une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, strictement positive dans un ensemble de $\mathfrak{F}$, et telle que $\lim_{\mathfrak{F}} g = 0$ ou $\lim_{\mathfrak{F}} g = +\infty$. On dit qu’une fonction $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ est d’ordre $\varphi$ (fini ou infini) par rapport à g si on a $\lim_{\mathfrak{F}} \log (|f|/|\log g|) = \varphi$.

On notera que si $f$ est d’ordre $\varphi$ par rapport à $g$, $f$ est d’ordre $-\varphi$ par rapport à $1/g$; on peut donc considérer uniquement le cas où $g(x)$ tend vers $+\infty$ suivant $\mathfrak{F}$.

#### Proposition 12 {#fvr-v-s1-prop-12 .statement}

Soit $g$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ telle que $\lim_{\mathfrak{F}} g = +\infty$; soit $f$ une fonction de $\mathcal{H}(\mathfrak{F}, \mathbf{R})$.

a) Pour que $f$ soit d’ordre $+\infty$ par rapport à $g$, il faut et il suffit que $f \gg g^\alpha$ pour tout $\alpha \geqslant 0$.

b) Pour que $f$ soit d’ordre $-\infty$ par rapport à $g$, il faut et il suffit que $f \ll g^{-\alpha}$ pour tout $\alpha > 0$.

c) Pour que $f$ soit d’ordre fini et égal à $\varphi$ par rapport à $g$, il faut et il suffit que, pour tout $\varepsilon > 0$, on ait $g^{\varphi-\varepsilon} \ll f \ll g^{\varphi+\varepsilon}$.

Démontrons par exemple c). Si l’ordre de $f$ par rapport à $g$ est $\varphi$, pour tout $\varepsilon > 0$, il existe un ensemble $M \in \mathfrak{F}$, tel que, pour tout $x \in M$, on ait
$$
\left( \varphi - \frac{\varepsilon}{2} \right) \log g(x) \leqslant \log |f(x)| \leqslant \left( \varphi + \frac{\varepsilon}{2} \right) \log g(x),
$$
ou encore $(g(x))^{\varphi-\frac{\varepsilon}{2}} \leqslant |f(x)| \leqslant (g(x))^{\varphi+\frac{\varepsilon}{2}}$; comme $\lim_{\mathfrak{F}} g = +\infty$, on a donc $g^{\varphi-\varepsilon} \ll f \ll g^{\varphi+\varepsilon}$ pour tout $\varepsilon > 0$; la réciproque est immédiate. Les démonstrations de a) et b) sont analogues.

On notera que si $f$ est d’ordre fini $\varphi$ par rapport à $g$, $fg^{-\varphi}$ est d’ordre 0 par rapport à $g$, et réciproquement; si $f_1$ (resp. $f_2$) est d’ordre $\rho_1$ (resp. $\rho_2$) par rapport à $g$, et si $\rho_1 + \rho_2$ est défini, $f_1 f_2$ est d’ordre $\rho_1 + \rho_2$ par rapport à $g$.

#### Remarque 1 {#fvr-v-s1-n4-rem-1 .statement}

On observera que lorsque $f$ est d’ordre fini $\varphi$ par rapport à $g$, le rapport $f/g^\varphi$ ne tend pas nécessairement vers une limite; par exemple, toute fonction logarithmiquement bornée est d’ordre 0 par rapport à $g$, mais n’a pas nécessairement de limite suivant $\mathfrak{F}$.

#### Remarque 2 {#fvr-v-s1-n4-rem-2 .statement}

Une fonction $f$ définie dans un ensemble de $\mathfrak{F}$ n’a pas nécessairement un ordre déterminé (fini ou non) par rapport à $g$, car les fonctions ayant un ordre déterminé par rapport à $g$ sont comparables à toutes les puissances de $g$, sauf une au plus. Or, $f$ n’a pas nécessairement cette propriété, comme on le voit sur l’exemple $g(x) = x$, $f(x) = 1 + x^2 \sin^2 x$ (x tendant vers $+\infty$). Dans cet exemple, $f$ est comparable à $g^\alpha$ pour $\alpha < 0$ et $\alpha > 2$; si on prenait $f(x) = e^x \sin^2 x + e^{-x} \cos^2 x$, $f$ ne serait comparable à aucune puissance (positive ou négative) de $g$.

### 5. Notations

Étant donnée une fonction numérique $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$, il est souvent commode, dans une formule, de noter $O(f)$ une fonction dominée par $f$, et $o(f)$ une fonction négligeable devant $f$. Lorsque, dans une démonstration, interviennent plusieurs fonctions dominées par une même fonction $f$ (resp. négligeables devant $f$), on les notera $O_1(f), O_2(f)$, etc. (resp. $o_1(f), o_2(f)$, etc.).

Beaucoup d’auteurs notent indistinctement $O(f)$ (resp. $o(f)$) toutes les fonctions intervenant dans une démonstration et dominées par $f$ (resp. négligeables devant $f$), par un abus de langage qui n’est pas sans créer des risques de confusion.

Avec ces notations, les prop. 1, 2, 3 (V, p. 3) se traduisent comme suit: si $g = O_1(f)$ et $h = O(g)$, alors $h = O_2(f)$; on peut écrire

(1)
$$
\sum_{i=1}^n \lambda_i O_i(f) = O_{n+1}(f) \quad (\lambda_i \text{ scalaires})
$$
(2)
$$
O(f)O(g) = O(fg).
$$

De même, la prop. 4 (V, p. 5) montre que si $g = O_1(f)$ et $h = o(g)$ (resp. $g = o_1(f)$ et $h = O(g)$), on a $h = o_2(f)$, et les prop. 5 et 6 (V, p. 5) s’expriment sous la forme

(3)
$$
\sum_{i=1}^n \lambda_i o_i(f) = o_{n+1}(f) \quad (\lambda_i \text{ scalaires})
$$
(4)
$$
o(f)o(g) = o(fg).
$$

La relation $f \sim g$ équivaut à $f = g + o(g)$. La notation $O(1)$ (resp. $o(1)$) désigne une fonction bornée dans un ensemble de $\mathfrak{F}$ (resp. une fonction tendant vers 0 suivant $\mathfrak{F}$).

## EXERCICES {#fvr-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
