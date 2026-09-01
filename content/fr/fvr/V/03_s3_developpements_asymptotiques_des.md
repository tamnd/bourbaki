---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: ÉTUDE LOCALE DES FONCTIONS
section: 3
section_title: Développements asymptotiques des fonctions d'une variable réelle
lang: fr
source: fvr-i-vii-fr
book_pages: FVR V.18-FVR V.26
pdf_pages: 0223-0231, 0253-0254
extraction: ocr
subsections:
    - "no": 1
      title: 'Intégration des relations de comparaison: I. Relations faibles'
      page: 18
      pdf_page: 223
    - "no": 2
      title: 'Application : critères logarithmiques de convergence des intégrales'
      page: 19
      pdf_page: 224
    - "no": 3
      title: 'Intégration des relations de comparaison: II. Relations fortes'
      page: 20
      pdf_page: 225
    - "no": 4
      title: Dérivation des relations de comparaison
      page: 22
      pdf_page: 227
    - "no": 5
      title: Partie principale d’une primitive
      page: 23
      pdf_page: 228
    - "no": 6
      title: Développement asymptotique d’une primitive
      page: 25
      pdf_page: 230
statements: 22
exercises: 7
content_sha256: 20d29f65ab35a35f5a172f906fd69619f5e0f561f0080c86b52406bf3574f7b9
---

## § 3. DÉVELOPPEMENTS ASYMPTOTIQUES DES FONCTIONS D’UNE VARIABLE RÉELLE

Dans ce paragraphe, nous allons considérer seulement le cas où l’ensemble E est un intervalle ouvert de la droite achevée $\overline{\mathbf{R}}$, et $\mathfrak{F}$ une base de la trace sur E du filtre des voisinages de l’origine ou de l’extrémité $\alpha$ de E; en outre, nous étudierons surtout les fonctions numériques (finies) définies dans un ensemble de $\mathfrak{F}$ (dépendant de la fonction considérée). En utilisant au besoin l’un des changements de variables $x' = -x, x' = \frac{1}{x - \alpha}, x' = -\frac{1}{x - \alpha}$, on peut toujours se ramener au cas où E est un intervalle de la forme $]a, +\infty[$, et par suite où $\mathfrak{F}$ est formée des intervalles $]t, +\infty[$, où $t > a$. Nous nous bornerons donc en principe à ce dernier cas, et laisserons au lecteur le soin de traduire la plupart des propositions obtenues (au moyen des changements de variables précédents), sauf pour quelques résultats particulièrement importants.

Il nous sera commode de désigner, par abus de langage, les ensembles de $\mathfrak{F}$ sous le nom de « voisinages de $+\infty$ ».

### 1. Intégration des relations de comparaison: I. Relations faibles

#### Proposition 1 {#fvr-v-s3-prop-1 .statement}

Dans un intervalle $]a, +\infty[$, soient $\mathbf{f}$ une fonction vectorielle réglée, g une fonction réglée $\geqslant 0$ et telle que $\int_a^{+\infty} g(t)\ dt > 0$. La relation $\mathbf{f} \preccurlyeq g$ pour $x$ tendant vers $+\infty$ entraîne $\int_a^x \mathbf{f}(t)\ dt \preccurlyeq \int_a^x g(t)\ dt$. Si l’intégrale $\int_a^{+\infty} g(t)\ dt$ est convergente, l’intégrale $\int_a^{+\infty} \mathbf{f}(t)\ dt$ est absolument convergente.

En effet, il existe par hypothèse $b \geqslant a$ et un nombre $c' > 0$ tels que
$$
\| \mathbf{f}(x) \| \leqslant c'(g(x)) \quad \text{pour } x \geqslant b,
$$
d’où
$$
\left\| \int_b^x \mathbf{f}(t)\ dt \right\| \leqslant \int_b^x \| \mathbf{f}(t) \| \ dt \leqslant c' \int_b^x g(t)\ dt;
$$
comme d’autre part, on peut supposer $b$ assez grand pour que $\int_a^b g(t)\ dt > 0$, il existe $c'' > 0$ tel que $\left\| \int_a^b \mathbf{f}(t)\ dt \right\| \leqslant c'' \int_a^b g(t)\ dt$; en posant $c = \max (c', c'')$, on a donc, pour tout $x \geqslant b$,
$$
\left\| \int_a^x \mathbf{f}(t)\ dt \right\| \leqslant c \int_a^x g(t)\ dt,
$$
d’où la proposition.

#### Corollaire 1 {#fvr-v-s3-prop-1-cor-1 .statement}

Si $f$ et $g$ sont des fonctions réglées $\geqslant 0$ dans l’intervalle $]a, +\infty[$, telles que $f \succeq g$, et si $\int_a^{+\infty} g(t)\ dt = +\infty$, on a $\int_a^{+\infty} f(t)\ dt = +\infty$.

#### Corollaire 2 {#fvr-v-s3-prop-1-cor-2 .statement}

Si $f$ et $g$ sont $\geqslant 0$ et non identiquement nulles dans $[a, +\infty[$ et telles que $f \asymp g$, on a $\int_a^x f(t)\ dt \asymp \int_a^x g(t)\ dt$.

### 2. Application : critères logarithmiques de convergence des intégrales

Par un choix convenable de la fonction $g$, on peut déduire de la prop. 1 de V, p. 18, et de son cor. 1 des critères permettant d’affirmer que l’intégrale $\int_a^{+\infty} f(t)\ dt$ d’une fonction $f \geqslant 0$ est convergente ou infinie : il suffit de choisir pour $g$ une fonction dont on connaît une primitive. En particulier, comme $x^\mu$ a pour primitive $\frac{x^{\mu+1}}{\mu+1}$ lorsque $\mu \neq -1$, et log $x$ lorsque $\mu = -1$, on a le critère suivant :

#### Proposition 2 (« critère logarithmique d’ordre 0 ») {#fvr-v-s3-prop-2 .statement}

Soit $f$ une fonction réglée $\geqslant 0$ dans l’intervalle $[a, +\infty[$; si $f(x) \leqslant x^\mu$ pour un $\mu < -1$, l’intégrale $\int_a^{+\infty} f(t)\ dt$ est convergente ; si $f(x) \geqslant x^\mu$ pour un $\mu \geqslant -1$, l’intégrale $\int_a^{+\infty} f(t)\ dt$ est infinie.

Ce critère ne permet pas de conclure lorsque $1/x^{1+\alpha} \ll f(x) \ll 1/x$ pour tout exposant $\alpha > 0$, par exemple pour $f(x) = 1/x(\log x)^\mu$ ($\mu > 0$). Mais dans ce dernier cas, $f$ a pour primitive $\frac{1}{1-\mu} (\log x)^{1-\mu}$ si $\mu \neq 1$ et log log $x$ si $\mu = 1$. Par suite :

#### Proposition 3 (« critère logarithmique d’ordre 1 ») {#fvr-v-s3-prop-3 .statement}

Soit $f$ une fonction réglée $\geqslant 0$ dans l’intervalle $[a, +\infty[$; si $f(x) \leqslant 1/x(\log x)^\mu$ pour un $\mu > 1$, l’intégrale $\int_a^{+\infty} f(t)\ dt$ est convergente ; si $f(x) \geqslant 1/x(\log x)^\mu$ pour un $\mu \leqslant 1$, l’intégrale $\int_a^{+\infty} f(t)\ dt$ est infinie.

De façon générale, désignons par $l_n(x)$, pour tout entier $n \geqslant 0$, la fonction définie par récurrence (pour $x$ assez grand) par les relations $l_0(x) = x$, $l_n(x) = \log(l_{n-1}(x))$ pour $n \geqslant 1$ ; on dit que $l_n(x)$ est le $n$-ème logarithme itéré de $x$ (cf. Appendix). On vérifie aussitôt que $\frac{1}{1-\mu} (l_n(x))^{1-\mu}$ est une primitive de

$$
\frac{1}{x.l_1(x).l_2(x)\ldots l_{n-1}(x)\ (l_n(x))^\mu}
$$

pour $\mu \neq 1$, et $l_{n+1}(x)$ une primitive de

$$
\frac{1}{x.l_1(x).l_2(x)\ldots l_{n-1}(x).l_n(x)}
$$

Par suite :

#### Proposition 4 (« critère logarithmique d’ordre $n$ ») {#fvr-v-s3-prop-4 .statement}

Soit $f$ une fonction réglée $\geqslant 0$ dans l’intervalle $[a, +\infty[$; si $f(x) \leqslant \frac{1}{x.l_1(x).l_2(x)\ldots l_{n-1}(x)\ (l_n(x))^\mu}$ pour un $\mu > 1$, l’intégrale $\int_a^{+\infty} f(t) \, dt$ est convergente; si $f(x) \geqslant \frac{1}{x.l_1(x)\ldots l_{n-1}(x).(l_n(x))^{\mu}}$ pour un $\mu \leqslant 1$, l’intégrale $\int_a^{+\infty} f(t) \, dt$ est infinie.

Chaque critère logarithmique est donc applicable à des fonctions pour lesquelles les critères d’ordre inférieur ne peuvent donner de conclusion (cf. V, p. 52, exerc. 5 b) et V, p. 53, exerc. 8).

En raison de son utilité, nous traduirons le critère d’ordre 0 pour les intégrales $\int_a^a f(t) \, dt$, où $f$ est réglée et $\geqslant 0$ dans l’intervalle non compact $]\alpha, a]$:

**Proposition 5** (« critère logarithmique d’ordre 0 »). — Si, au voisinage de $\alpha$, on a $f(x) \leqslant 1/(x-\alpha)^{\mu}$ pour un $\mu < 1$, l’intégrale $\int_a^a f(t) \, dt$ est convergente; si $f(x) \geqslant 1/(x-\alpha)^{\mu}$ pour un $\mu \geqslant 1$, l’intégrale $\int_a^a f(t) \, dt$ est infinie.

Nous laissons au lecteur le soin de traduire de même le critère logarithmique d’ordre $n$.

L’application des critères logarithmiques est immédiate si on sait obtenir une partie principale de $f$ par rapport à une échelle de comparaison contenant les fonctions qui interviennent dans ces critères: si $f_1$ est cette partie principale, l’intégrale $\int_a^{+\infty} f(t) \, dt$ est convergente ou infinie en même temps que $\int_a^{+\infty} f_1(t) \, dt$, et pour cette dernière intégrale, l’application des critères logarithmiques est immédiate.

#### Exemple 1 {#fvr-v-s3-n2-exa-1 .statement}

La fonction $t^p(1-t)^q$ est non bornée dans $]0,1[$ lorsque $p < 0$ ou $q < 0$; d’après les critères logarithmiques d’ordre 0 appliqués au voisinage des points 0 et 1, pour que l’intégrale $\int_0^1 t^p(1-t)^q \, dt$ converge, il faut et il suffit que $p > -1$ et $q > -1$. Lorsqu’il en est ainsi, cette intégrale est dite intégrale eulérienne de première espèce et notée $B(p+1,q+1)$ (cf. VII, p. 8).

#### Exemple 2 {#fvr-v-s3-n2-exa-2 .statement}

Considérons l’intégrale $\int_0^{\infty} t^{x-1}e^{-t} \, dt$. Comme $e^{-t} \sim 1$ au voisinage de 0, pour que cette intégrale converge, il faut que $x > 0$; cette condition est aussi suffisante car au voisinage de $+\infty$, on a $e^{-t} \ll t^{-\mu}$ quel que soit $\mu > 0$. Lorsque $x > 0$, l’intégrale est dite intégrale eulérienne de seconde espèce et notée $\Gamma(x)$ (cf. VII, p. 7).

### 3. Intégration des relations de comparaison: II. Relations fortes

#### Proposition 6 {#fvr-v-s3-prop-6 .statement}

Soient $\mathbf{f}$ une fonction vectorielle réglée, $g$ une fonction numérique réglée et $\geqslant 0$ dans $]a, +\infty[$.

1° Si l’intégrale $\int_a^{+\infty} g(t)dt$ est convergente, la relation $\mathbf{f} \ll g$ (resp. $\mathbf{f} \sim c g$, où $c$ est constant) entraîne $\int_x^{+\infty} \mathbf{f}(t) \, dt \ll \int_x^{+\infty} g(t) \, dt$ (resp. $\int_x^{+\infty} \mathbf{f}(t) \, dt \sim c \int_x^{+\infty} g(t) \, dt$).

2° Si l’intégrale $\int_a^{+\infty} g(t) \, dt$ est infinie, la relation $\mathbf{f} \ll g$ (resp. $\mathbf{f} \sim c g$) entraîne

$$ \int_{\alpha}^{\infty} \mathbf{f}(t) \, dt \ll \int_{\beta}^{\infty} g(t) \, dt \quad \text{(resp. } \int_{\alpha}^{\infty} \mathbf{f}(t) \, dt \sim c \int_{\beta}^{\infty} g(t) \, dt,\text{)} $$

quels que soient $\alpha$ et $\beta$ dans $]a, +\infty[$.

Il suffit de démontrer la proposition concernant la relation $f \ll g$, puisque, si $c \neq 0$, la relation $f \sim cg$ est équivalente à $f - cg \ll g$.

La première partie est une conséquence immédiate du théorème de la moyenne, car si on a $\|f(x)\| \leq \varepsilon g(x)$ pour $x \geq x_0$, on en tire
$$
\left\| \int_x^{+\infty} f(t) \, dt \right\| \leq \int_x^{+\infty} \|f(t)\| \, dt \leq \varepsilon \int_x^{+\infty} g(t) \, dt \quad \text{pour } x \geq x_0.
$$
En second lieu, supposons que $\int_a^{+\infty} g(t) \, dt = +\infty$. Si $\|f(x)\| \leq \varepsilon g(x)$ pour $x \geq x_0 \geq \max(\alpha, \beta)$, on a
$$
\int_\alpha^\infty \|f(t)\| \, dt = \int_\alpha^{x_0} \|f(t)\| \, dt + \int_{x_0}^\infty \|f(t)\| \, dt \leq \int_\alpha^{x_0} \|f(t)\| \, dt + \varepsilon \int_{x_0}^\infty g(t) \, dt
$$
$$
= \varepsilon \int_\beta^\infty g(t) \, dt + \left( \int_\alpha^{x_0} \|f(t)\| \, dt - \varepsilon \int_\beta^{x_0} g(t) \, dt \right).
$$
Or, il existe $x_1 \geq x_0$ tel que pour tout $x \geq x_1$
$$
\left| \int_\alpha^{x_0} \|f(t)\| \, dt - \varepsilon \int_\beta^{x_0} g(t) \, dt \right| \leq \varepsilon \int_\beta^\infty g(t) \, dt
$$
d’où, pour $x \geq x_1$
$$
\left\| \int_\alpha^\infty f(t) \, dt \right\| \leq \int_\alpha^\infty \|f(t)\| \, dt \leq 2\varepsilon \int_\beta^\infty g(t) \, dt
$$
ce qui achève la démonstration, $\varepsilon > 0$ étant arbitraire.

En d’autres termes, on peut intégrer les deux membres d’une relation forte $f \ll g$, $f \sim ag$, lorsque $g$ est positive dans un intervalle $(a, +\infty)$, sans que la relation cesse d’avoir lieu entre les primitives des deux membres, pourvu qu’on ait soin d’intégrer de $x$ à $+\infty$ si $\int_a^{+\infty} g(t) \, dt$ est convergente et de $\alpha$ à $x$ ($\alpha$ quelconque dans $(a, +\infty)$) dans le cas contraire.

On notera que les prop. 1 (V, p. 18) et 6 (V, p. 20) sont encore valables lorsque $\mathfrak{F}$ est la base de filtre formée de la trace des intervalles $(t, +\infty)$ (où $t > a$) sur le complémentaire d’un ensemble dénombrable (cf. I, p. 23, th. 2).

#### Exemple 1 {#fvr-v-s3-n3-exa-1 .statement}

En appliquant la prop. 6 de V, p. 20, à la relation $1/x \ll x^{\alpha-1}$ où $\alpha > 0$, on retrouve la relation $\log x \ll x^\alpha$ pour tout $\alpha > 0$, équivalente à la relation $y^{1/\alpha} \ll e^y$ démontrée dans III, p. 16.

#### Exemple 2 {#fvr-v-s3-n3-exa-2 .statement}

On a $\left( \frac{e^x}{x} \right)' = \frac{e^x}{x} \left( 1 - \frac{1}{x} \right) \sim e^x/x$; comme $e^x/x$ tend vers $+\infty$ avec $x$, on déduit de la prop. 6 de V, p. 20, que $\int_1^x \frac{e^t}{t} \, dt \sim e^x/x$.

#### Remarque {#fvr-v-s3-n3-rem-1 .statement}

Lorsque $g$ n’est pas supposée rester $\geq 0$ dans un intervalle $(a, +\infty)$ (ou rester $\leq 0$ dans un tel intervalle), et que $\int_a^{+\infty} g(t) \, dt$ n’est pas convergente, la relation $f \sim g$ n’entraîne pas nécessairement $\int_a^\infty f(t) \, dt \sim \int_a^\infty g(t) \, dt$, comme le montre l’exemple où $g(x) = \sin x$ et $f(x) = \left( 1 + \frac{\sin x}{x} \right) \sin x$; on a en effet
$$
\int_{n\pi}^{(n+1)\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{(n+1)\pi} \int_0^\pi \sin^2 t \, dt \geq \frac{1}{2} \int_{n+1}^{n+2} \frac{dt}{t},
$$

d’où

$$
\int_{\pi}^{n\pi} \frac{\sin^2 t}{t} dt \geq \frac{1}{2} \int_{2}^{n+1} \frac{dt}{t}
$$

et l’intégrale $\int_{1}^{\infty} dt/t$ est infinie, alors que $\int_{\frac{\pi}{2}}^{\infty} g(t) \, dt = -\cos x$ reste bornée (cf. V, p. 49, exerc. 4).

### 4. Dérivation des relations de comparaison

Les propositions 1 (V, p. 18) et 6 (V, p. 20) n’admettent pas de réciproque : l’existence d’une relation de comparaison $f \leq g$, $f \ll g$, $f \sim cg$ entre deux fonctions dérivables au voisinage de $+\infty$ n’entraîne pas nécessairement la même relation de comparaison entre leurs dérivées, même lorsqu’il s’agit de relations de comparaison entre fonctions numériques et monotones $f$ et $g$.

Par exemple, la fonction $x^2 + x \sin x + \cos x$ est monotone et équivalente à $x^2$, mais sa dérivée $x(2 + \cos x)$ n’est pas équivalente à $2x$.

Par contre, on peut dériver des relations de comparaison lorsqu’on suppose a priori que les dérivées des fonctions considérées sont comparables (V, p. 7). De façon générale, nous dirons que deux fonctions numériques $f, g$, définies dans un intervalle $[a, +\infty[$, sont comparables d’ordre $k$ au voisinage de $+\infty$ si, dans un voisinage de $+\infty$, elles admettent une dérivée $k$-ème réglée sauf en une infinité dénombrable de points, et si, dans ce voisinage, $f^{(k)}$ et $g^{(k)}$ gardent un signe constant (dans l’ensemble où elles sont définies), et sont comparables.

On convient de dire que deux fonctions numériques comparables (V, p. 7) sont comparables d’ordre 0.

#### Proposition 7 {#fvr-v-s3-prop-7 .statement}

Si deux fonctions numériques $f, g$, sont comparables d’ordre 1, elles sont comparables ; en outre, la relation $f \ll g$ (resp. $f \sim cg, c$ constante) entraîne $f' \ll g'$ (resp. $f' \sim cg'$) sauf si $g$ est équivalente à une constante $\neq 0$.

En effet, comme $f'$ et $g'$ gardent un signe constant dans un intervalle $]x_0, +\infty[$, $f$ et $g$ sont monotones dans cet intervalle, donc tendent vers une limite finie ou infinie lorsque $x$ tend vers $+\infty$. Il est évident que $f$ et $g$ sont comparables lorsque $x$ tend vers $+\infty$, si une de ces limites est finie et $\neq 0$, ou si l’une est nulle et l’autre infinie. Si $f$ et $g$ tendent toutes deux vers 0, on peut écrire $f(x) = -\int_x^{+\infty} f'(t) dt, g(x) = -\int_x^{+\infty} g'(t) dt$; comme $f'$ et $g'$ sont comparables, il en est de même de $f$ et $g$ et la relation de comparaison entre $f$ et $g$ est la même que celle qui existe entre $f'$ et $g'$, d’après la prop. 6 (V, p. 20). De même, si $f$ et $g$ ont toutes deux un elimite infinie, on a $f(x) = f(x_0) + \int_{x_0}^x f'(t) dt, g(x) = g(x_0) + \int_{x_0}^x g'(t) dt$; la prop. 6 (V, p. 20) montre de nouveau que $f$ et $g$ sont comparables et que la relation de comparaison entre $f$ et $g$ est la même que celle qui existe entre $f'$ et $g'$. Pour achever de démontrer la proposition, il reste à considérer le cas où $g$ tend vers $\pm \infty$ et $f$ vers une constante ; alors on ne peut avoir $f' \gg g'$, car on déduirait de la prop. 1 (V, p. 18) que l’intégrale $\int_{x_0}^\infty g'(t)\,dt$ serait convergente; comme $f'$ et $g'$ sont supposées comparables, on a nécessairement $f' \ll g'$.

#### Corollaire {#fvr-v-s3-n4-cor-1 .statement}

Si deux fonctions numériques $f, g$ sont comparables d’ordre $k \geqslant 1$, elles sont comparables d’ordre $p$ pour $0 \leqslant p \leqslant k$; en outre, la relation $f \ll g$ (resp. $f \sim cg$) entraîne $f^{(k)} \ll g^{(k)}$ (resp. $f^{(k)} \sim cg^{(k)}$) sauf lorsque l’une des dérivées $g^{(p)}$ ($0 \leqslant p \leqslant k - 1$) est équivalente à une constante $\neq 0$.

En effet, comme $f^{(k)}$ et $g^{(k)}$ gardent un signe constant dans un intervalle $[x_0, +\infty[$, $f^{(k-1)}$ et $g^{(k-1)}$ sont monotones dans cet intervalle, donc gardent un signe constant au voisinage de $+\infty$; en outre, la prop. 7 de V, p. 22, montre que $f^{(k-1)}$ et $g^{(k-1)}$ sont comparables, donc le corollaire résulte de la prop. 7 appliquée par récurrence sur $k$.

#### Remarque 1 {#fvr-v-s3-n4-rem-1 .statement}

La restriction de l’énoncé de la prop. 7 concernant $g$ est essentielle. Par exemple, on a $1/x \ll 1 + \frac{1}{x}$ bien que les dérivées des deux membres soient équivalentes; de même $1 + \frac{1}{x} \sim 1 + \frac{1}{x^2}$, mais $1/x^2 \gg 2/x^3$.

#### Remarque 2 {#fvr-v-s3-n4-rem-2 .statement}

Si $f$ et $g$ sont comparables d’ordre $k$, une fonction $f_1$ équivalente à $f$ n’est pas nécessairement comparable d’ordre $k$ à $g$; elle l’est toutefois si on suppose que $f_1$ est comparable d’ordre $k$ à $f$ et qu’aucune des dérivées $f^{(p)}$ ($0 \leqslant p \leqslant k - 1$) n’est équivalente à une constante $\neq 0$.

#### Remarque 3 {#fvr-v-s3-n4-rem-3 .statement}

Si $f$ et $g$ sont comparables d’ordre $k$, il n’en pas nécessairement de même de $hf$ et $hg$, même pour une fonction monotone $h$ aussi simple que $h(x) = x$ (V, p. 49, exerc. 3); de même, $1/f$ et $1/g$ ne sont pas nécessairement comparables d’ordre $k$ (V, p. 48, exerc. 1).

### 5. Partie principale d’une primitive

Soit $f$ une fonction numérique réglée $\neq 0$ et gardant un signe constant dans un intervalle $[a, +\infty[$; la proposition suivante permet dans certains cas d’obtenir une partie principale simple de la primitive $\int_x^{+\infty} f(t)\,dt$ si $\int_a^{+\infty} f(t)\,dt$ est convergente, et de la primitive $\int_a^x f(t)\,dt$ si l’intégrale $\int_a^{+\infty} f(t)\,dt$ est infinie:

#### Proposition 8 {#fvr-v-s3-prop-8 .statement}

On pose $F(x) = \int_x^{+\infty} f(t)\,dt$ si $\int_a^{+\infty} f(t)\,dt$ est convergente, $F(x) = \int_a^x f(t)\,dt$ si $\int_a^{+\infty} f(t)\,dt$ est infinie. On suppose que $\log |f|$ et $\log x$ sont comparables d’ordre 1.

1° Si $f$ est d’ordre fini $\mu \neq -1$ par rapport à $x$, on a
$$
F(x) \sim \frac{1}{|\mu + 1|}\, x f(x).
$$
(1)

2° Si $f$ est d’ordre infini par rapport à $x$ et si $f/f'$ et $x$ sont comparables d’ordre 1, on a
$$
F(x) \sim \frac{(f(x))^2}{|f'(x)|}.
$$
(2)

On notera que l’hypothèse entraîne que $f(x)$ a un ordre déterminé par rapport à $x$ (V, p. 9).

§ 3

1° Si $f$ est d'ordre $\mu \neq 0$ par rapport à $x$, on a $\log |f| \sim \mu \log x$, donc, comme $\log |f|$ et $\log x$ sont comparables d'ordre 1, on a d'après la prop. 7 de V, p. 22, $f'/f \sim \mu/x$, ou $x f' \sim \mu f$. Si $\mu > -1$, on a $f(x) \gg x^{\mu-\varepsilon}$ pour tout $\varepsilon > 0$, donc (V, p. 19, prop. 2) l'intégrale $\int_a^{+\infty} f(t)\,dt$ est infinie. On peut écrire $F(x) = \int_a^x f(t)\,dt = x f(x) - a f(a) - \int_a^x t f'(t)\,dt$, ou encore
$$
\int_a^x (f(t) + t f'(t))\,dt = x f(x) - a f(a);
$$
comme $\mu \neq -1, f(x) + x f'(x) \sim (\mu + 1) f(x)$, donc (V, p. 20, prop. 6)
$$
\int_a^x (f(t) + t f'(t))\,dt \sim (\mu + 1) F(x),
$$
ce qui démontre dans ce cas la relation (1). Si $\mu = 0$, on a de même $x f'(x) \ll f(x)$, ce qui donne encore $f(x) + x f'(x) \sim f(x)$. On raisonne de manière analogue lorsque $\mu < -1$, cas où $\int_a^{+\infty} f(t)\,dt$ est convergente.

2° Si $f$ est d'ordre $+\infty$ par rapport à $x$, on a $\log |f| \gg \log x$, donc (V, p. 22, prop. 7) $f'/f \gg 1/x$, ou encore, en posant $g(x) = f(x)/f'(x)$, $g(x) \ll x$; en outre, comme $f(x) \gg x^\alpha$ pour tout $\alpha > 0$, l'intégrale $\int_a^{+\infty} f(t)\,dt$ est infinie. On peut écrire
$$
F(x) = \int_a^x f(t)\,dt = \int_a^x g(t) f'(t)\,dt = g(x) f(x) - g(a) f(a) - \int_a^x f(t) g'(t)\,dt;
$$
comme $g$ et $x$ sont comparables d'ordre 1, de la relation $g(x) \ll x$ on déduit (V, p. 22, prop. 7) $g'(x) \ll 1$, donc $f g' \ll f$, et par suite (V, p. 20, prop. 6)
$$
\int_a^x f(t) g'(t)\,dt \ll F(x),
$$
ce qui établit la relation (2). Démonstration analogue lorsque $f$ est d'ordre $-\infty$ par rapport à $x$, cas où $\int_a^{+\infty} f(t)\,dt$ est convergente.

Soit $\mathscr{E}$ une échelle de comparaison (pour $x$ réel tendant vers $+\infty$) formée de fonctions numériques non nulles et de signe constant au voisinage de $+\infty$, telle que $x \in \mathscr{E}$ et que le produit et le quotient de deux fonctions de $\mathscr{E}$ appartiennent encore à $\mathscr{E}$ (V, p. 11 et p. 14). Si une fonction réglée $f$ de signe constant au voisinage de $+\infty$ admet une partie principale $c g$ par rapport à $\mathscr{E}$, $\int_a^{+\infty} f(t)\,dt$ (resp. $\int_a^x f(t) dt$ suivant le cas) sera équivalente à $c \int_a^{+\infty} g(t)\,dt$ (resp. $c \int_a^x g(t)\,dt$); si la fonction $g$ satisfait aux conditions de la prop. 8 de V, p. 23, et si (lorsque la formule (2) de V, p. 23, s'applique) on connaît une partie principale de $g'$ relativement à $\mathscr{E}$, on aura ainsi une partie principale de $\int_a^{+\infty} f(t)\,dt$ (resp. $\int_a^x f(t)\,dt$) relativement à $\mathscr{E}$.

#### Exemple 1 {#fvr-v-s3-n5-exa-1 .statement}

La fonction $1/\log x$ est d’ordre 0 par rapport à $x$, et satisfait aux conditions de la prop. 8 de V, p. 23; donc
$$
\int_a^x \frac{dt}{\log t} \sim \frac{x}{\log x}.
$$
2) La fonction $e^{x^2}$ est d’ordre $+\infty$ par rapport à $x$ et satisfait aux conditions de la prop. 8, donc
$$
\int_a^x e^{t^2} dt \sim \frac{1}{2x} e^{x^2}.
$$
Dans l’Appendice (V, p. 41), nous définirons un ensemble de fonctions auxquelles les prop. 7 et 8 sont toujours applicables.

#### Remarque {#fvr-v-s3-n5-rem-1 .statement}

La prop. 8 n’est pas directement applicable à une fonction $f$ d’ordre –1 par rapport à $x$. Mais on peut alors écrire $f(x) = f_1(x)/x$, $f_1$ étant d’ordre 0 par rapport à $x$. Supposons par exemple que $\int_a^{+\infty} f(t) \, dt$ soit infini; alors
$$
F(x) = \int_a^x f(t) \, dt = \int_a^x \frac{1}{t} f_1(t) \, dt = \int_{\log a}^{\log x} f_1(e^u) \, du.
$$
Si la fonction $f_1(e^y)$ satisfait aux conditions de la prop. 8 et a un ordre $\neq -1$ par rapport à $y$ (c’est-à-dire si $f_1(x)$ a un ordre $\neq -1$ par rapport à $\log x$), les formules (1) et (2) permettront encore d’obtenir une partie principale de $F(x)$. Par exemple, soit $f(x) = \frac{\exp (\sqrt{\log x})}{x \log x}$; comme $\exp (\sqrt{\log x})$ est d’ordre 0 par rapport à $x$, $f$ est d’ordre –1; on a ici $f_1(e^y) = e^{\sqrt{y}}/y$ et cette fonction est d’ordre $+\infty$ par rapport à $y$; la prop. 8 lui est applicable et donne $\int_a^y e^{\sqrt{u}}/u \, du \sim 2e^{\sqrt{y}}/\sqrt{y}$; en revenant à la variable $x$, il vient donc $\int_a^x \frac{\exp (\sqrt{\log t})}{t \log t} \, dt \sim \frac{2 \exp (\sqrt{\log x})}{\sqrt{\log x}}$.

### 6. Développement asymptotique d’une primitive

Soit $\mathcal{E}$ une échelle de comparaison au voisinage de $+\infty$ formée de fonctions numériques $\neq 0$ et de signe constant au voisinage de $+\infty$; soit $\mathbf{f}$ une fonction vectorielle réglée définie dans un intervalle $]a, +\infty[$, à valeurs dans un espace normé complet $E$, et admettant un développement asymptotique
$$
\mathbf{f} = \sum_{\lambda < \alpha} a_\lambda g_\lambda + \mathbf{r}_\alpha
$$
à la précision $g_\alpha$, par rapport à $\mathcal{E}$. Supposons en outre que toute primitive $\int_a^x g(t) \, dt$ d’une fonction $g \in \mathcal{E}$ admette un développement asymptotique par rapport à $\mathcal{E}$. Dans ces conditions, nous allons voir qu’on peut obtenir un développement asymptotique de $F(x) = \int_a^x \mathbf{f}(t) \, dt$ relativement à $\mathcal{E}$. Distinguons deux cas:
1° $\int_a^{+\infty} g_\alpha(t) \, dt$ est infini; alors (V, p. 20, prop. 6), on a $\int_a^x \mathbf{r}_\alpha(t) \, dt \ll \int_a^x g_\alpha(t) \, dt$; par hypothèse, on peut obtenir un développement asymptotique de $\sum_{\lambda < \alpha} a_\lambda \int_a^x g_\lambda(t) \, dt$ à une certaine précision $g_\rho$ (V, p. 12); si $c g_\sigma$ est la partie principale de $\int_a^x g_\alpha(t) dt$, on aura donc un développement asymptotique de $\int_a^x \mathbf{f}(t) \, dt$ à la précision $g_{\min(\rho, \sigma)}$, dont tous les termes ont des normes croissant indéfiniment.

2° $\int_a^{+\infty} g_\alpha(t) \, dt$ est convergente; soit $\beta$ alors le plus petit des indices $\lambda \leq \alpha$ tels que $a_\lambda \neq 0$ et que $\int_a^{+\infty} g_\lambda(t) dt$ soit convergente; l’intégrale
$$
C = \int_a^{+\infty} (f(t) - \sum_{\lambda < \beta} a_\lambda g_\lambda(t)) \, dt
$$
est alors convergente, et on peut écrire
$$
F(x) = \sum_{\lambda < \beta} a_\lambda \int_a^x g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda < \alpha} a_\lambda \int_x^{+\infty} g_\lambda(t) \, dt - \int_x^{+\infty} r_\alpha(t) \, dt.
$$
On a alors $\int_x^{+\infty} r_\alpha(t) \, dt \ll \int_x^{+\infty} g_\alpha(t) \, dt$; si $c g_\sigma$ est la partie principale de $\int_x^{+\infty} g_\sigma(t) dt$, et si on a un développement asymptotique de
$$
\sum_{\lambda < \beta} a_\lambda \int_a^x g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda < \alpha} a_\lambda \int_x^{+\infty} g_\lambda(t) \, dt
$$
à la précision $g_\sigma$, on aura de la sorte un développement asymptotique de $F$ à la précision $g_{\min(\sigma, \alpha)}$.

Tout revient donc à trouver des développements asymptotiques par rapport à $\mathcal{E}$ de primitives de fonctions de $\mathcal{E}$. Nous avons vu comment, moyennant certaines hypothèses sur $\mathcal{E}$, la prop. 8 de V, p. 23 donne la partie principale d’une telle primitive. En outre, la démonstration de la prop. 8 donne l’expression de la différence des deux membres de la formule (1) (resp. (2)) de V, p. 23, sous forme d’une primitive de la fonction $\frac{1}{|\mu + 1|} (x f'(x) + f(x)) - f(x)$ (resp. $f(x) g'(x)$), avec $g = f/f'$; en formant la partie principale de cette nouvelle primitive, ainsi qu’un développement asymptotique du second membre de (1) (resp. (2)), on obtiendra le second terme du développement cherché (voir V, p. 36–43).

#### Exemple 1 {#fvr-v-s3-n6-exa-1 .statement}

Soit $f(x) = 1/\log x$ ($x > 1$); on a vu que $\int_a^x dt/\log t \sim x/\log x$, et la différence $\int_a^x \frac{dt}{\log t} - \frac{x}{\log x}$ est une primitive de $1/(\log x)^2$; on peut de nouveau appliquer à cette fonction la prop. 8, qui donne $\int_a^x dt/(\log t)^2 \sim x/(\log x)^2$. Par récurrence, on obtient ainsi le développement
$$
\int_a^x \frac{dt}{\log t} = \frac{x}{\log x} + \frac{x}{(\log x)^2} + \frac{2x}{(\log x)^3} + \cdots + (n-1)! \frac{x}{(\log x)^n} + o\left( \frac{x}{(\log x)^n} \right).
$$
On notera que, quel que soit $n$, tous les termes de ce développement tendent vers $+\infty$ avec $x$.

#### Exemple 2 {#fvr-v-s3-n6-exa-2 .statement}

Soit $f(x) = \frac{e^x}{x^2 + 1}$; on peut écrire $f(x) = \frac{e^x}{x^2} - \frac{e^x}{x^4} + o_1\left( \frac{e^x}{x^4} \right)$. La prop. 8 donne les développements
$$
\int_a^x \frac{e^t}{t^2} \, dt = \frac{e^x}{x^2} + \frac{2e^x}{x^3} + \frac{6e^x}{x^4} + o_2\left( \frac{e^x}{x^4} \right)
$$
$$
\int_a^x \frac{e^t}{t^4} \, dt = \frac{e^x}{x^4} + o_3\left( \frac{e^x}{x^4} \right)
$$
d’où par addition
$$
\int_a^x \frac{e^t}{t^2 + 1} \, dt = \frac{e^x}{x^2} + 2 \frac{e^x}{x^3} + 5 \frac{e^x}{x^4} + o_4\left( \frac{e^x}{x^4} \right)
$$

## EXERCICES {#fvr-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
