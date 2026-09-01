---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES ET INTÉGRALES
section: 3
section_title: Dérivées et intégrales de fonctions dépendant d'un paramètre
lang: fr
source: fvr-i-vii-fr
book_pages: FVR II.35-FVR II.38
pdf_pages: 0070-0081, 0087-0090
extraction: ocr
subsections:
    - "no": 1
      title: Intégrale d’une limite de fonctions dans un intervalle compact
      page: 18
      pdf_page: 70
    - "no": 2
      title: Intégrale d’une limite de fonctions dans un intervalle non compact
      page: 20
      pdf_page: 72
    - "no": 3
      title: Intégrales normalement convergentes
      page: 23
      pdf_page: 75
    - "no": 4
      title: Dérivée par rapport à un paramètre d’une intégrale dans un intervalle compact
      page: 24
      pdf_page: 76
    - "no": 5
      title: Dérivée par rapport à un paramètre d’une intégrale dans un intervalle non compact
      page: 26
      pdf_page: 78
    - "no": 6
      title: Interversion des intégrations
      page: 27
      pdf_page: 79
statements: 17
exercises: 10
content_sha256: 78e9b0c6439bb8e707e8de339dc250f725de8e22ef83030101571459ec119b77
---

## § 3. DÉRIVÉES ET INTÉGRALES DE FONCTIONS DÉPENDANT D’UN PARAMÈTRE

### 1. Intégrale d’une limite de fonctions dans un intervalle compact

Le th. 1 de II, p. 2, appliqué au cas particulier des primitives de fonctions réglées dans un intervalle compact, se traduit de la manière suivante dans la notation propre aux intégrales:

#### Proposition 1 {#fvr-ii-s3-prop-1 .statement}

Soient $A$ un ensemble filtré par un filtre $\mathfrak{F}$, $(f_\alpha)_{\alpha \in A}$ une famille de fonctions réglées dans un intervalle compact $I = (a, b)$; si les fonctions $f_\alpha$ convergent uniformément dans $I$ vers une fonction (réglée) $f$ suivant le filtre $\mathfrak{F}$, on a
$$
\lim_{\mathfrak{F}} \int_a^b f_\alpha(t) \, dt = \int_a^b f(t) \, dt.
$$
(1)

Deux corollaires de cette proposition sont importants dans les applications:

#### Corollaire 1 {#fvr-ii-s3-prop-1-cor-1 .statement}

Soit $(\mathbf{f}_n)$ une suite de fonctions réglées dans un intervalle compact $I = (a, b)$. Si la suite $(\mathbf{f}_n)$ converge uniformément dans $I$ vers une fonction (réglée) $\mathbf{f}$, on a
$$
\lim_{n \to \infty} \int_a^b \mathbf{f}_n(t) \, dt = \int_a^b \mathbf{f}(t) \, dt.
$$
(2)

En particulier, si une série dont le terme général $u_n$ est une fonction réglée dans $I$, converge uniformément vers $\mathbf{f}$ dans $I$, la série de terme général $\int_a^b u_n(t) dt$ est convergente et a pour somme $\int_a^b \mathbf{f}(t)dt$ (« intégration terme à terme d’une série uniformément convergente »).

#### Corollaire 2 {#fvr-ii-s3-prop-1-cor-2 .statement}

Soient $A$ une partie d’un espace topologique $F$, $\mathbf{f}$ une application de $I \times A$ dans un espace normé complet $E$ sur $\mathbf{R}$, telle que, pour tout $\alpha \in A$, la fonction $x \mapsto \mathbf{f}(x, \alpha)$ soit réglée dans $I$. Si les fonctions $x \mapsto \mathbf{f}(x, \alpha)$ convergent uniformément dans $I$ vers une fonction (réglée) $x \mapsto \mathbf{f}(x)$, lorsque $\alpha$ tend vers un point $\alpha_0 \in \overline{A}$ en restant dans $A$, on a
$$
\lim_{\alpha \to \alpha_0, \alpha \in A} \int_a^b \mathbf{f}(x, \alpha) \, dx = \int_a^b g(x) \, dx.
$$
(3)

En particulier:

#### Proposition 2 (« continuité d’une intégrale par rapport au paramètre ») {#fvr-ii-s3-prop-2 .statement}

Soient $F$ un espace compact, $I = (a, b)$ un intervalle compact de $\mathbf{R}$, $\mathbf{f}$ une application continue de $I \times F$ dans un espace normé complet $E$ sur $\mathbf{R}$; la fonction $h(\alpha) = \int_a^b \mathbf{f}(\alpha, x) \, dx$ est continue dans $F$.

En effet, comme $\mathbf{f}$ est uniformément continue dans l’espace compact $I \times F$, les fonctions $\mathbf{f}(\alpha, x)$ convergent uniformément vers $\mathbf{f}(x, \alpha_0)$ dans $I$, lorsque $\alpha$ tend vers un point quelconque $\alpha_0 \in F$.

Voici une application de cette proposition : la fonction $(x, \alpha) \mapsto x^\alpha$ est continue dans le produit $I \times J$, où $I = (a, b)$ est un intervalle compact tel que $0 < a < b$, $J$ un intervalle compact quelconque dans $\mathbf{R}$; on en conclut que $\int_a^b x^\alpha dx$ est une fonction continue de $\alpha$ dans $\mathbf{R}$; or, pour $\alpha$ rationnel et $\neq -1$, cette fonction est égale à $\frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$, et la fonction $\alpha \mapsto \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ est continue dans tout intervalle de $\mathbf{R}$ ne contenant pas $-1$; on a donc (prolongement des identités) $\int_a^b x^\alpha dx = \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ pour tout $\alpha$ réel et $\neq -1$; cela signifie encore que, pour tout $\alpha$ réel, la dérivée de $x^\alpha$ est $\alpha x^{\alpha-1}$ (cf. III, p. 4).

### 2. Intégrale d’une limite de fonctions dans un intervalle non compact

Le th. 1 de II, p. 2 s’applique à des fonctions plus générales que les fonctions réglées, puisqu’il suppose seulement que ces fonctions admettent des primitives. On voit donc en particulier que la prop. 1 de II, p. 19 s’applique encore lorsque, dans un intervalle $I \subset \mathbf{R}$, les fonctions $f_\alpha$ sont seulement supposées réglées par morceaux et admettant une intégrale dans $I$; toutefois, ce résultat suppose que soient vérifiées les deux autres hypothèses de la prop. 1, savoir : 1° $I$ est un intervalle borné ; 2° les $f_\alpha$ convergent uniformément dans $I$ vers $f$. La formule (1) de II, p. 19 peut être inexacte lorsque l’une de ces conditions cesse d’être remplie : il peut se faire alors que l’un ou l’autre des deux membres n’existe pas, ou qu’ils existent tous deux mais aient des valeurs distinctes.

Par exemple, si $f_n$ est la fonction réglée dans $]0, 1[$, définie par $f_n(x) = n$ pour $0 < x < 1/n$, $f_n(x) = 0$ pour $1/n \leq x \leq 1$, la suite $(f_n)$ converge vers 0 uniformément dans tout intervalle compact contenu dans $]0, 1[$, mais non uniformément dans $]0, 1[$, et on a $\int_0^1 f_n(t) \, dt = 1$ pour tout $n$. On aurait un exemple où $\int_0^1 f_n(t) \, f$ ne tend vers aucune limite en remplaçant la suite $(f_n)$ précédente par la suite $((-1)^n f_n)$ qui converge encore uniformément vers 0 dans tout intervalle compact contenu dans $]0, 1[$.

D’autre part, dans l’intervalle non borné $I = (0, +\infty[$, soit $f_n$ la fonction réglée telle que $f_n(x) = 1/n$ pour $n^2 \leq x \leq (n+1)^2$ et $f_n(x) = 0$ pour toute autre valeur de $x$ dans $I$ ($n \geq 1$) ; la suite $(f_n)$ converge uniformément vers 0 dans $I$, mais l’intégrale $\int_0^{+\infty} f_n(t) \, dt = (2n+1)/n$ tend vers 2 lorsque $n$ croît indéfiniment.

En d’autres termes, lorsque $I$ est non borné, si on désigne par $\mathscr{F}$ l’espace vectoriel formé des fonctions $f$ réglées dans $I$, à valeurs dans $E$, et admettant une intégrale dans $I$, l’application $f \mapsto \int_I f(t) \, dt$ n’est pas continue lorsqu’on munit $\mathscr{F}$ de la topologie de la convergence uniforme dans $I$ (cf. II, p. 4, cor. 2).

Nous allons chercher des conditions suffisantes pour assurer la validité de la prop. 1, sous les hypothèses suivantes :
1° $I$ est un intervalle quelconque de $\mathbf{R}$, $f_\alpha$ est réglée dans $I$, et admet dans $I$ une intégrale ;
2° suivant le filtre $\mathfrak{F}$, la famille $(f_\alpha)$ converge uniformément vers $f$ dans tout intervalle compact contenu dans $I$.

Désignant alors par $\mathfrak{S}(I)$ l’ensemble ordonné filtrant des intervalles compacts contenus dans $I$ (II, p. 15), le premier membre de la formule (1) de II, p. 19 peut s’écrire $\lim_{J \in \mathfrak{S}(I)} (\lim_{\alpha \in J} \int_J f_\alpha(t) \, dt)$; d’autre part compte tenu de la prop. 1 (II, p. 19) et du fait que la famille $(f_\alpha)$ est uniformément convergente dans tout intervalle compact $J \subset I$, le second membre de (1) (II, p. 19) peut s’écrire $\lim_{J \in \mathfrak{S}(I)} (\lim_{\alpha \in J} \int_J f_\alpha(t) \, dt)$. On voit donc que la prop. 1 de II, p. 19 s’étendra lorsqu’on pourra intervertir les limites de l’application $(J, \alpha) \mapsto \int_J f_\alpha(t) \, dt$ suivant le filtre $\mathfrak{F}$, et suivant le filtre des sections $\Phi$ de l’ordonné filtrant $\mathfrak{S}(I)$. Or, nous connaissons une condition suffisante pour que cette interversion soit licite, savoir l’existence de la limite de l’application $(J, \alpha) \mapsto \int_J f_\alpha(t)\ dt$ suivant le *filtre produit* $\Phi \times \mathfrak{F}$ (TG, I, p. 58, cor. du th. 1). Nous allons transformer cette condition en une condition équivalente plus maniable.

En premier lieu, comme $E$ est complet, pour que $(J, \alpha) \mapsto \int_J f_\alpha(t)\ dt$ ait une limite suivant $\Phi \times \mathfrak{F}$, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe un intervalle compact $J_0 \subset I$ et un ensemble $M \in \mathfrak{F}$ tels que, quels que soient les éléments $\alpha, \beta$ de $M$ et l’intervalle compact $J \supset J_0$ contenu dans $I$, on ait

$$
\left\| \int_{J_0} f_\alpha(t)\ dt - \int_J f_\beta(t)\ dt \right\| \leq \varepsilon.
$$

Nous allons montrer d’autre part que cette condition est elle-même équivalente à la condition suivante: pour tout $\varepsilon > 0$, il existe un intervalle compact $J_0 \subset I$ et un ensemble $M \in \mathfrak{F}$ tels que, quels que soient $\alpha \in M$ et l’intervalle compact $J \supset J_0$ contenu dans $I$, on ait

$$
\left\| \int_{J_0} f_\alpha(t)\ dt - \int_J f_\alpha(t)\ dt \right\| \leq \varepsilon.
$$

Il est évident en effet que cette dernière condition est nécessaire; inversement, si elle est satisfaite, il existe (en vertu de la convergence uniforme de $(f_\alpha)$ dans tout intervalle compact) un ensemble $N \in \mathfrak{F}$ tel que, quels que soient $\alpha, \beta$ dans $N$, on ait

$$
\left\| \int_{J_0} f_\alpha(t)\ dt - \int_{J_0} f_\beta(t)\ dt \right\| \leq \varepsilon;
$$

et par suite, on a $\left\| \int_{J_0} f_\alpha(t)\ dt - \int_J f_\beta(t)\ dt \right\| \leq 2\varepsilon$ quels que soient $\alpha$ et $\beta$ dans $M \cap N \in \mathfrak{F}$ et quel que soit l’intervalle compact $J \supset J_0$.

Enfin, le lemme de II, p. 16 nous permet de mettre la dernière condition trouvée sous la forme équivalente suivante: *pour tout $\varepsilon > 0$, il existe un intervalle compact $J_0 \subset I$ et un ensemble $M \in \mathfrak{F}$ (dépendant de $\varepsilon$) tels que, pour tout intervalle compact $K \subset I$ n’ayant aucun point intérieur commun avec $J_0$, et tout $\alpha \in M$, on ait* $\left\| \int_K f_\alpha(t)\ dt \right\| \leq \varepsilon$.

Le plus souvent, on utilise une condition plus restrictive, obtenue en supposant, dans l’énoncé précédent, que l’ensemble $M$ *ne dépende pas de* $\varepsilon$:

#### Définition 1 {#fvr-ii-s3-def-1 .statement}

*On dit que l’intégrale* $\int_I f_\alpha(t)\ dt$ *est uniformément convergente pour* $\alpha \in A$ *(ou uniformément convergente dans* $A$*) si, pour tout* $\varepsilon > 0$, *il existe un intervalle compact* $J_0 \subset I$ *tel que, pour tout intervalle compact* $K \subset I$ *sans point intérieur commun avec* $J_0$, *et tout* $\alpha \in A$, *on ait*

$$
\left\| \int_K f_\alpha(t)\ dt \right\| \leq \varepsilon.
$$

Cette définition équivaut à dire que la famille des applications $\alpha \mapsto \int_I f_\alpha(t) \, dt$ est uniformément convergente dans $A$ (vers l’application $\alpha \mapsto \int_I f_\alpha(t) \, dt$) suivant le filtre des sections $\Phi$ de $\mathfrak{F}(I)$; chacune des intégrales $\int_I f_\alpha(t)$ est a fortiori convergente (la réciproque étant inexacte). En outre, d’après ce que nous venons de voir (ou d’après TG, X, p. 8, cor. 2):

#### Proposition 3 {#fvr-ii-s3-prop-3 .statement}

Soit $(\mathbf{f}_\alpha)$ une famille de fonctions réglées dans un intervalle $I$, telles que:
1° suivant le filtre $\mathfrak{F}$, la famille $(\mathbf{f}_\alpha)$ converge uniformément vers une fonction $\mathbf{f}$ (réglée dans $I$) dans tout intervalle compact contenu dans $I$; 2° l’intégrale $\int_I \mathbf{f}_\alpha(t) \, dt$ soit uniformément convergente pour tout $\alpha \in A$. Dans ces conditions, l’intégrale $\int_I \mathbf{f}(t) \, dt$ est convergente, et on a
$$
\lim_{\mathfrak{F}} \int_I \mathbf{f}_\alpha(t) \, dt = \int_I \mathbf{f}(t) \, dt.
$$
Les conditions de la prop. 3 sont remplies par exemple lorsque $I$ est un intervalle borné, que les $\mathbf{f}_\alpha$ sont uniformément bornées dans $I$, et convergent uniformément vers $\mathbf{f}$ dans tout intervalle compact contenu dans $I$; en effet, si $\| \mathbf{f}_\alpha(x) \| \leq h$ pour tout $x \in I$ et tout $\alpha$, et si $J_0$ est tel que la différence entre les longueurs de $I$ et de $J_0$ soit $\leq \varepsilon / h$, la condition (7) est vérifiée pour tout intervalle $K \subset I$ sans point intérieur commun avec $J_0$.

Comme pour la prop. 1 de II, p. 19, deux corollaires de la prop. 3 sont importants dans les applications:

#### Corollaire 1 {#fvr-ii-s3-prop-3-cor-1 .statement}

Soit $(\mathbf{f}_n)$ une suite de fonctions réglées dans un intervalle quelconque $I$, uniformément convergente vers une fonction $\mathbf{f}$ dans tout intervalle compact contenu dans $I$; si l’intégrale $\int_I \mathbf{f}_n(t) \, dt$ est uniformément convergente, l’intégrale $\int_I \mathbf{f}(t) \, dt$ est convergente, et on a
$$
\lim_{n \to \infty} \int_I \mathbf{f}_n(t) \, dt = \int_I \mathbf{f}(t) \, dt.
$$

#### Remarque {#fvr-ii-s3-n2-rem-1 .statement}

Les hypothèses faites dans ce corollaire sont suffisantes, mais non nécessaires pour la validité de la formule (9); nous généraliserons plus tard cette formule en même temps que la notion d’intégrale (voir INT, IV), et obtiendrons des conditions beaucoup moins restrictives.

#### Corollaire 2 {#fvr-ii-s3-prop-3-cor-2 .statement}

Soient $A$ une partie d’un espace topologique $F$, $\mathbf{f}$ une application de $I \times A$ dans un espace normé complet $E$ sur $\mathbf{R}$, telle que, pour tout $\alpha \in A$, la fonction $x \mapsto \mathbf{f}(x, \alpha)$ soit réglée dans $I$. Si, d’une part, les fonctions $x \mapsto \mathbf{f}(x, \alpha)$ convergent uniformément, dans tout intervalle compact contenu dans $I$, vers une fonction $x \mapsto \mathbf{f}(x)$, lorsque $\alpha$ tend vers $\alpha_0 \in \overline{A}$ en restant dans $A$; si, d’autre part, l’intégrale $\int_I \mathbf{f}(x, \alpha) \, dx$ est uniformément convergente dans $A$, alors l’intégrale $\int_I \mathbf{f}(x) \, dx$ est convergente, et on a
$$
\lim_{\alpha \to \alpha_0, \alpha \in A} \int_I \mathbf{f}(x, \alpha) \, dx = \int_I \mathbf{f}(x) \, dx.
$$

En particulier:

#### Proposition 4 (« continuité d’une intégrale impropre par rapport au paramètre ») {#fvr-ii-s3-prop-4 .statement}

Soient F un espace compact, I un intervalle quelconque de R, f une application continue de I × F dans un espace normé complet E sur R ; si l’intégrale h(α) = ∫_I f(x, α) dx est uniformément convergente dans F, elle est fonction continue de α dans F.

Compte tenu de la prop. 2 de II, p. 19, cette proposition résulte aussi de la continuité d’une limite uniforme de fonctions continues (TG, X, p. 9, th. 2).

### 3. Intégrales normalement convergentes

Soit (f_α)_{α∈A} une famille de fonctions réglées dans un intervalle quelconque I ⊂ R, à valeurs dans un espace normé complet E sur R. Supposons qu’il existe une fonction numérique finie g réglée dans I, telle que, pour tout x ∈ I et tout α ∈ A, on ait \|f_α(x)\| ≤ g(x) et que l’intégrale ∫_I g(t) dt soit convergente. Dans ces conditions, l’intégrale ∫_I f_α(t) dt est absolument et uniformément convergente dans A ; en effet, pour tout intervalle compact K contenu dans I, on a

$$
\left\| \int_K f_α(t) \, dt \right\| \leq \int_K g(t) \, dt
$$

et la convergence de l’intégrale ∫_I g(t) dt entraîne que, pour tout ε > 0, il existe un intervalle compact J ⊂ I tel que, pour tout intervalle compact K ⊂ I ne rencontrant pas J, on ait ∫_K g(t) dt ≤ ε. Lorsqu’il existe une fonction numérique g ayant les propriétés précédentes, on dit que l’intégrale ∫_I f_α(t) dt est normalement convergente dans A (cf. TG, X, p. 22).

Une intégrale peut être uniformément convergente dans A sans être normalement convergente. \* C’est ce qui se passe pour la suite (f_n) de fonctions numériques définies par les conditions f_n(x) = 1/x pour n ≤ x ≤ n + 1, f_n(x) = 0 pour les autres valeurs de x dans I = (1, +∞[. Il est immédiat que l’intégrale ∫_1^{+∞} f_n(t) dt est uniformément convergente, mais elle n’est pas normalement convergente, car la relation g(x) ≥ f_n(x) pour tout x ∈ I et tout n entraîne g(x) ≥ 1/x, et par suite l’intégrale de g dans I n’est pas convergente. \*

En particulier, considérons une série dont le terme général u_n est une fonction réglée dans l’intervalle I, et supposons que la série de terme général \|u_n(x)\| (qui est une fonction réglée dans I) converge uniformément dans tout intervalle compact contenu dans I, et soit telle que la série de terme général ∫_I \|u_n(t)\| dt soit convergente; alors (II, p. 16, prop. 2) la fonction (réglée) g(x), somme de la série de terme général \|u_n(x)\|, est telle que l’intégrale ∫_I g(t) dt soit convergente. Si on pose f_n = ∑_{p=1}^n u_p, l’intégrale ∫_I f_n(t) dt est normalement convergente, car on a

$$
\|f_n(x)\| \leq \sum_{p=1}^n \|u_p(x)\| \leq g(x)
$$

pour tout $x \in I$ et tout $n$; par suite, la somme $f$ de la série de terme général $u_n$ est une fonction réglée dans $I$ telle que l’intégrale $\int_I f(t)\, dt$ soit convergente, et on a

$$
\int_I f(t)\, dt = \sum_{n=1}^\infty \int_I u_n(t)\, dt
$$

(« intégration terme à terme d’une série dans un intervalle non compact »).

### 4. Dérivée par rapport à un paramètre d’une intégrale dans un intervalle compact

Soient $A$ un voisinage compact d’un point $x_0$ dans le corps $\mathbf{R}$ (resp. le corps $\mathbf{C}$), $I = [a,\ b]$ un intervalle *compact* dans $\mathbf{R}$, $f$ une application *continue* de $I \times A$ dans un espace normé complet $E$ sur $\mathbf{R}$ (resp. $\mathbf{C}$). On a vu (II, p. 19, prop. 2) que, dans ces conditions, $g(\alpha) = \int_a^b f(t,\ \alpha)\, dt$ est une fonction *continue* dans $A$. Cherchons des conditions *suffisantes* pour que $g$ admette une *dérivée* au point $x_0$. On a, pour $\alpha \neq x_0$

$$
\frac{g(\alpha) - g(x_0)}{\alpha - x_0} = \int_a^b \frac{f(t,\ \alpha) - f(t,\ x_0)}{\alpha - x_0}\, dt
$$

donc (II, p. 19, cor. 2), si les fonctions $x \mapsto \frac{f(x,\ \alpha) - f(x,\ x_0)}{\alpha - x_0}$ *convergent uniformément dans* $I$ vers une fonction (nécessairement continue) $x \mapsto h(x)$ lorsque $\alpha$ tend vers $x_0$ (en restant $\neq x_0$), $g$ admet une *dérivée* égale à $\int_a^b h(t)\, dt$ au point $x_0$; d’ailleurs, pour chaque $x \in I$, $\frac{f(x,\ \alpha) - f(x,\ x_0)}{\alpha - x_0}$ tend vers $h(x)$, donc $h(x)$ est la *dérivée* au point $x_0$ de l’application $\alpha \mapsto f(x,\ \alpha)$; nous désignerons cette *dérivée* (dite *dérivée partielle de* $f$ *par rapport à* $\alpha$) par la notation $f'_\alpha(x,\ x_0)$; les hypothèses faites entraînent donc que

$$
g'(\alpha_0) = \int_a^b f'_\alpha(t,\ x_0)\, dt.
$$

La proposition suivant donne une condition suffisante plus simple pour la validité de la formule (12):

#### Proposition 5 {#fvr-ii-s3-prop-5 .statement}

*On suppose que la dérivée partielle* $f'_\alpha(x,\ x)$ *existe pour tout* $x \in I$ *et tout* $\alpha$ *appartenant à un voisinage ouvert* $V$ *de* $x_0$, *et que, pour tout* $\alpha \in V$, *l’application* $x \mapsto f'_\alpha(x,\ \alpha)$ *soit réglée dans* $I$. *Dans ces conditions, si* $x \mapsto f'_\alpha(x,\ \alpha)$ *converge uniformément dans* $I$ *vers* $x \mapsto f'_\alpha(x,\ x_0)$ *lorsque* $\alpha$ *tend vers* $x_0$, *la fonction* $g(\alpha) = \int_a^b f(t,\ \alpha)\, dt$ *admet au point* $x_0$ *une dérivée donnée par la formule* (12).

En effet, pour tout $\varepsilon > 0$, il existe par hypothèse $r > 0$ tel que $|\alpha - x_0| \leq r$ entraîne $\| \mathbf{f}'_\alpha(x, \alpha) - \mathbf{f}'_\alpha(x, \alpha_0) \| \leq \varepsilon$ quel que soit $x \in I$. D’après les prop. 3 et 5 de I, p. 25, on a, pour $|\alpha - \alpha_0| \leq r$ ($\alpha \neq \alpha_0$) et pour tout $x \in I$

$$
\left\| \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0} - \mathbf{f}'_\alpha(x, \alpha_0) \right\| \leq \varepsilon
$$

ce qui prouve la convergence uniforme de $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ vers $\mathbf{f}'_\alpha(x, \alpha_0)$ dans $I$ lorsque $\alpha$ tend vers $\alpha_0$ (en restant $\neq \alpha_0$), et établit donc la formule (12).

#### Corollaire {#fvr-ii-s3-n4-cor-1 .statement}

*Si la dérivée partielle $\mathbf{f}'_\alpha(x, \alpha)$ existe dans $I \times V$ et est fonction continue de $(x, \alpha)$ dans cet ensemble, la fonction $g$ admet au point $\alpha_0$ une dérivée donnée par la formule (12).*

En effet, si $W$ est un voisinage compact de $\alpha_0$ contenu dans $V$, l’application $(x, \alpha) \mapsto \mathbf{f}'_\alpha(x, \alpha)$ est *uniformément continue* dans l’ensemble compact $I \times W$, donc $\mathbf{f}'_\alpha(x, \alpha)$ tend uniformément vers $\mathbf{f}'_\alpha(x, \alpha_0)$ dans $I$ lorsque $\alpha$ tend vers $\alpha_0$.

De la prop. 5, on déduit une proposition plus générale permettant de calculer la dérivée d’une intégrale lorsque, non seulement la fonction intégrée $\mathbf{f}$, mais aussi les limites d’intégration, dépendent du paramètre $\alpha$:

#### Proposition 6 {#fvr-ii-s3-prop-6 .statement}

*Les conditions de la prop. 5 étant supposées vérifiées, soient $a(\alpha), b(\alpha)$ deux fonctions définies dans $V$, à valeurs dans $I$; si les dérivées $a'(\alpha_0), b'(\alpha_0)$ existent et sont finies, la fonction $g(\alpha) = \int_{a(\alpha)}^{b(\alpha)} \mathbf{f}(t, \alpha) dt$ admet au point $\alpha_0$ une dérivée donnée par la formule*

$$
g'(\alpha_0) = \int_{a(\alpha_0)}^{b(\alpha_0)} \mathbf{f}'_\alpha(t, \alpha_0) \, dt + b'(\alpha_0) \mathbf{f}(b(\alpha_0), \alpha_0) - a'(\alpha_0) \mathbf{f}(a(\alpha_0), \alpha_0).
$$

En effet, pour tout $\alpha \in V$ distinct de $\alpha_0$, on peut écrire

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_{a(\alpha_0)}^{b(\alpha_0)} \frac{\mathbf{f}(t, \alpha) - \mathbf{f}(t, \alpha_0)}{\alpha - \alpha_0} \, dt + \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} \mathbf{f}(t, \alpha) \, dt
$$
$$
- \frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} \mathbf{f}(t, \alpha) \, dt.
$$

D’après la prop. 5 de II, p. 24, la première intégrale du second membre tend vers $\int_{a(\alpha_0)}^{b(\alpha_0)} \mathbf{f}'_\alpha(t, \alpha_0) \, dt$ lorsque $\alpha$ tend vers $\alpha_0$. Dans la seconde, nous allons remplacer $\mathbf{f}(t, \alpha)$ par $\mathbf{f}(b(\alpha_0), \alpha_0)$, et montrer que la différence tend vers 0. Posons $M = \mathrm{Max}(\|\mathbf{f}(b(\alpha_0), \alpha_0)\|, |b'(\alpha_0)| + 1)$; la fonction $b(\alpha)$ étant continue au point $\alpha_0$, et la fonction $\mathbf{f}$ continue au point $(b(\alpha_0), \alpha_0)$, pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, il existe $r > 0$ tel que la relation $|\alpha - \alpha_0| \leq r$ entraîne $\|\mathbf{f}(t, \alpha) - \mathbf{f}(b(\alpha_0), \alpha_0)\| \leq \varepsilon$ pour tout $t$ appartenant à l’intervalle d’extrémités $b(\alpha_0)$ et $b(\alpha)$; on peut aussi supposer que la relation $|\alpha - \alpha_0| \leq r$ entraîne $\left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} - b'(\alpha_0) \right| \leq \varepsilon$.

D’après la formule de la moyenne (II, p. 12, formule (17)), on a donc

$$
\left\| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} \mathbf{f}(t, \alpha) \, dt - \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \mathbf{f}(b(\alpha_0), \alpha_0) \right\| \leq \left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \right| \varepsilon
$$

et par suite

$$
\left\| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} \mathbf{f}(t, \alpha) \, dt - b'(\alpha_0) \mathbf{f}(b(\alpha_0), \alpha_0) \right\| \leq 2M \varepsilon
$$

ce qui montre que $\frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} \mathbf{f}(t, \alpha) \, dt$ tend vers $b'(\alpha_0) \mathbf{f}(b(\alpha_0), \alpha_0)$. De la même manière, on montre que $\frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} \mathbf{f}(t, \alpha) \, dt$ tend vers $a'(\alpha_0) \mathbf{f}(a(\alpha_0), \alpha_0)$.

### 5. Dérivée par rapport à un paramètre d’une intégrale dans un intervalle non compact

L’ensemble V ayant la même signification que dans la prop. 5 de II, p. 24, supposons maintenant que I soit un intervalle quelconque de $\mathbf{R}$, $\mathbf{f}$ une application continue de $I \times V$ dans E; si l’intégrale $g(\alpha) = \int_I \mathbf{f}(t, \alpha) \, dt$ existe pour tout $\alpha \in V$ et est fonction continue de $\alpha$, la fonction $g$ n’a pas nécessairement au point $\alpha_0$ une dérivée égale à $\int_I \mathbf{f}'_\alpha(t, \alpha_0) \, dt$, même si $\mathbf{f}'_\alpha(x, \alpha)$ converge uniformément vers $\mathbf{f}'_\alpha(x, \alpha_0)$ dans tout intervalle compact contenu dans I, et si l’intégrale $\int_I \mathbf{f}'_\alpha(t, \alpha) \, dt$ existe pour tout $\alpha \in V$ (cf. II, p. 35, exerc. 3).

Une condition suffisante pour que la formule (12) (II, p. 24) soit encore valable dans ce cas est donnée par la proposition suivante:

#### Proposition 7 {#fvr-ii-s3-prop-7 .statement}

*Soit I un intervalle quelconque de $\mathbf{R}$, $\mathbf{f}$ une fonction continue dans $I \times V$. On suppose que:
1° la dérivée partielle $\mathbf{f}'_\alpha(x, \alpha)$ existe pour tout $x \in I$ et tout $\alpha \in V$, et, pour tout $\alpha \in V$, l’application $x \mapsto \mathbf{f}'_\alpha(x, \alpha)$ est réglée dans I;
2° pour tout $\alpha \in V$, $\mathbf{f}'_\alpha(x, \beta)$ converge uniformément vers $\mathbf{f}'_\alpha(x, \alpha)$ dans tout intervalle compact contenu dans I, lorsque $\beta$ tend vers $\alpha$;
3° l’intégrale $\int_I \mathbf{f}'_\alpha(t, \alpha) \, dt$ est uniformément convergente dans V;
4° l’intégrale $\int_I \mathbf{f}(t, \alpha_0) \, dt$ est convergente.

Dans ces conditions, l’intégrale $g(\alpha) = \int_I \mathbf{f}(t, \alpha) \, dt$ est uniformément convergente dans V, et la fonction g admet en tout point de V une dérivée donnée par la formule*

$$
g'(\alpha) = \int_I \mathbf{f}'_\alpha(t, \alpha) \, dt.
$$

La convergence uniforme dans V de l’intégrale $\int_I \mathbf{f}'_\alpha(t, \alpha) \, dt$ signifie que la fonction $\alpha \mapsto \int_J f'_\alpha(t, \alpha) \, dt$ converge uniformément dans V suivant le filtre des sections $\Phi$ de l’ordonné filtrant $\mathfrak{t}(I)$ des intervalles compacts J contenus dans I. Posons $u_J(\alpha) = \int_J f(t, \alpha)dt$; les hypothèses montrent d’une part que $u_J(\alpha_0)$ a une limite suivant $\Phi$, et d’autre part, en vertu de la prop. 5 de II, p. 24, que $u'_J(\alpha) = \int_J f'_\alpha(t, \alpha) \, dt$ pour tout $\alpha \in V$. Nous pouvons donc appliquer le th. 1 de II, p. 2, aux fonctions $u_J$, le rôle de l’ensemble d’indices étant tenu ici par $\mathfrak{t}(I)$, celui du filtre sur cet ensemble par le filtre $\Phi$; la proposition en résulte aussitôt.

#### Remarque 1 {#fvr-ii-s3-n5-rem-1 .statement}

Les conditions 1° et 2° de la prop. 7 sont remplies a fortiori lorsque $f'_\alpha(x, \alpha)$ est fonction continue de $(x, \alpha)$ dans $I \times V$.
2) Lorsque, dans une intégrale $\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt$, les extrémités de l’intervalle d’intégration sont des fonctions finies du paramètre, l’étude de cette intégrale en fonction de $\alpha$ peut se rattacher à celle d’une intégrale dans $[0, 1]$; en effet, par le changement de variable $t = a(\alpha)(1-u) + b(\alpha)u$, on a
$$
\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt = \int_0^1 f(a(\alpha)(1-u) + b(\alpha)u, \alpha)(b(\alpha) - a(\alpha)) \, du.
$$

### 6. Interversion des intégrations

Soient $I = [a, b]$ et $A = [c, d]$ deux intervalles compacts de $\mathbf{R}$; soit $f$ une fonction continue dans $I \times A$, à valeurs dans un espace normé complet $E$ sur $\mathbf{R}$; d’après la prop. 2 de II, p. 19, $\int_a^b f(x, \alpha) \, dx$ est fonction continue de $\alpha$ dans $A$; son intégrale $\int_c^d (\int_a^b f(x, \alpha) \, dx) d\alpha$ se note aussi, pour simplifier $\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx$.

#### Proposition 8 {#fvr-ii-s3-prop-8 .statement}

Si $f$ est continue dans $I \times A$, on a
$$
\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx = \int_a^b dx \int_c^d f(x, \alpha) \, d\alpha
$$
(« formule d’interversion des intégrations »).

Nous allons montrer que, pour tout $y \in A$, on a
$$
\int_c^y d\alpha \int_a^b f(x, \alpha) \, dx = \int_a^b dx \int_c^y f(x, \alpha) \, d\alpha.
$$

Comme les deux membres de (16) sont des fonctions de $y$ égales pour $y = c$, il suffira de prouver qu’elles sont dérivables dans $]c, d[$ et que leurs dérivées sont égales en tout point de cet intervalle. Si on pose $g(\alpha) = \int_a^b f(x, \alpha) \, dx$, $h(x, y) = \int_c^y f(x, \alpha) \, dx$, la relation (16) s’écrit
$$
\int_c^y g(\alpha) \, d\alpha = \int_a^b h(x, y) \, dx.
$$

Or, la dérivée du premier membre par rapport à $y$ est $g(y)$, celle du second est $\int_a^b h_y'(x, y) \, dx$ d’après II, p. 25, corollaire, puisque $h_y'(x, y) = f(x, y)$ est continue dans $I \times A$; les deux expressions ainsi obtenues sont bien identiques.

Supposons maintenant que $A = [c, d]$ soit un intervalle *compact* dans $\mathbf{R}$, $I$ un intervalle *quelconque* dans $\mathbf{R}$; soit $\mathbf{f}$ une fonction continue dans $I \times A$, à valeurs dans $E$, telle que l’intégrale $\mathbf{f}(\alpha) = \int_I \mathbf{f}(t, \alpha) \, dt$ soit convergente pour tout $\alpha \in A$; même si $g(\alpha)$ est continue dans $A$, on ne peut pas toujours intervertir les intégrations dans l’intégrale $\int_c^d d\alpha \int_I \mathbf{f}(t, \alpha) \, dt$, car l’intégrale $\int_I dt \int_c^d \mathbf{f}(t, \alpha) \, d\alpha$ peut ne pas exister, ou être distincte de l’intégrale $\int_c^d d\alpha \int_I \mathbf{f}(t, \alpha) \, dt$ (cf. II, p. 36, exerc. 7). On a toutefois le résultat suivant:

#### Proposition 9 {#fvr-ii-s3-prop-9 .statement}

*Si la fonction* $\mathbf{f}$ *est continue dans* $I \times A$, *et si l’intégrale* $\int_I \mathbf{f}(t, \alpha) \, dt$ *est uniformément convergente dans* $A$, *l’intégrale* $\int_I dt \int_c^d \mathbf{f}(t, \alpha) \, d\alpha$ *est convergente*, *et on a*
$$
\int_c^d d\alpha \int_I \mathbf{f}(t, \alpha) \, dt = \int_I dt \int_c^d \mathbf{f}(t, \alpha) \, d\alpha.
$$
(17)

Pour tout intervalle compact $J$ contenu dans $I$, posons $u_J(\alpha) = \int_J \mathbf{f}(t, \alpha) \, dt$. L’hypothèse entraîne que suivant le filtre des sections $\Phi$ de l’ordonné filtrant $k(I)$, la fonction continue $u_J$ converge uniformément dans $A$ vers $\int_I \mathbf{f}(t, \alpha) \, dt$; donc (II, p. 19, prop. 1), $\int_c^d d\alpha \int_J \mathbf{f}(t, \alpha) \, dt$ a pour limite $\int_c^d d\alpha \int_I \mathbf{f}(t, \alpha) \, dt$ suivant $\Phi$; mais, d’après la prop. 8 (II, p. 27), on a
$$
\int_c^d d\alpha \int_J \mathbf{f}(t, \alpha) \, dt = \int_J dt \int_c^d \mathbf{f}(t, \alpha) \, d\alpha.
$$
(18)

Le résultat précédent signifie donc que l’intégrale $\int_I dt \int_c^d \mathbf{f}(t, \alpha) \, d\alpha$ est convergente, et en passant à la limite suivant $\Phi$ dans la relation (18), on obtient (17).

Exercises

## EXERCICES {#fvr-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
