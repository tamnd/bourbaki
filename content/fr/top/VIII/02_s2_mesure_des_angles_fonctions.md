---
book: top
book_title: General Topology
chapter: VIII
chapter_title: NOMBRES COMPLEXES
section: 2
section_title: Mesure des angles; fonctions trigonométriques
lang: fr
source: top-v-x-fr
book_pages: TG VIII.7-TG VIII.15
pdf_pages: 0093-0101, 0111-0112
extraction: ocr
subsections:
    - "no": 1
      title: Le groupe multiplicatif U
      page: 7
      pdf_page: 93
    - "no": 2
      title: Angles de demi-droites
      page: 8
      pdf_page: 94
    - "no": 3
      title: Mesure des angles de demi-droites
      page: 10
      pdf_page: 96
    - "no": 4
      title: Fonctions trigonométriques
      page: 11
      pdf_page: 97
    - "no": 5
      title: Secteurs angulaires
      page: 13
      pdf_page: 99
    - "no": 6
      title: Angles de droites
      page: 14
      pdf_page: 100
statements: 5
exercises: 4
content_sha256: d20f42abcdd6aa338f831ed79ea60bd046d59840ad2df717ec1bef6f2d64d5ea
---

## § 2. MESURE DES ANGLES; FONCTIONS TRIGONOMÉTRIQUES

### 1. Le groupe multiplicatif U

#### Théorème 1 {#top-viii-s2-thm-1 .statement}

Le groupe topologique (multiplicatif) $\mathbf{U}$ des nombres complexes de valeur absolue 1 est isomorphe au groupe topologique (additif) $\mathbf{T}$ des nombres réels modulo 1.

En effet, $\mathbf{U} = S_1$ est compact et connexe, et possède un voisinage de l’élément neutre $+1$ homéomorphe à un intervalle ouvert de $\mathbf{R}$ (VI, p. 11, cor. 2); le théorème est donc une conséquence de la caractérisation topologique de $\mathbf{T}$ donnée dans V, p. 11, th. 2.

#### Corollaire {#top-viii-s2-n1-cor-1 .statement}

Le groupe multiplicatif $\mathbf{C}^*$ des nombres complexes $\neq 0$ est isomorphe au groupe $\mathbf{R} \times \mathbf{T}$ (cf. VIII, p. 4, prop. 1).

#### Remarque {#top-viii-s2-n1-rem-1 .statement}

L’isomorphie des groupes $\mathbf{C}^*$ et $\mathbf{R} \times \mathbf{T}$ entraîne l’existence des racines de toute « équation binôme » $z^n = a$ dans le corps $\mathbf{C}$; en s’appuyant sur cette propriété (et sur la compacité locale de $\mathbf{C}$) on peut obtenir une nouvelle démonstration du th. de d’Alembert-Gauss (VIII, p. 26, exerc. 2).

Il n’existe que deux isomorphismes distincts du groupe $\mathbf{T}$ sur le groupe $\mathbf{U}$; car si $g, g'$ sont deux isomorphismes de $\mathbf{T}$ sur $\mathbf{U}$, $h'$ l’isomorphisme réciproque de $g'$, $h' \circ g$ est un automorphisme de $\mathbf{T}$, donc (VII, p. 15, prop. 6) on a identiquement $g'(x) = g(x)$ ou $g'(x) = g(-x)$. On peut toujours supposer que l’isomorphisme $g$ est tel que $i$ soit l’image par $g$ de la classe (mod. 1) du point $\frac{1}{4}$; alors, en désignant par $\varphi$ l’homomorphisme canonique de $\mathbf{R}$ sur $\mathbf{T}$, tout morphisme strict du groupe additif $\mathbf{R}$ sur le groupe multiplicatif $\mathbf{U}$ est de la forme $x \mapsto g(\varphi(x/a))$, où $a$ est un nombre réel $\neq 0$ (VII, p. 14, prop. 4); on notera que l’intervalle $]-\lvert a \rvert/2, \lvert a \rvert/2[$ est le plus grand intervalle ouvert symétrique de $\mathbf{R}$ que ce morphisme strict applique d’une manière biunivoque sur image, et que l’on a $g(\varphi(\frac{1}{4})) = i$. Nous désignerons par $x \mapsto \mathbf{e}(x)$ l’homomorphisme $x \mapsto g(\varphi(x))$; tout morphisme strict de $\mathbf{R}$ sur $\mathbf{U}$ est donc de la forme $x \mapsto \mathbf{e}(x/a)$, où $a \neq 0$. La fonction $\mathbf{e}(x)$ est une fonction continue dans $\mathbf{R}$, à valeurs complexes, satisfaisant aux identités

(1) $$
|\mathbf{e}(x)| = 1,
$$
(2) $$
\mathbf{e}(x + y) = \mathbf{e}(x)\mathbf{e}(y),
$$
ainsi qu’aux relations
(3) $$
\mathbf{e}(0) = 1,\quad \mathbf{e}(\frac{1}{4}) = i,\quad \mathbf{e}(\frac{1}{2}) = -1,\quad \mathbf{e}(\frac{3}{4}) = -i,\quad \mathbf{e}(1) = 1.
$$
De (1) et (2) on tire les identités
(4) $$
\mathbf{e}(-x) = 1/\mathbf{e}(x) = \overline{\mathbf{e}(x)},
$$
et, de (2) et (3),
$$
\mathbf{e}(x + \frac{1}{4}) = i\mathbf{e}(x),\qquad \mathbf{e}(x + \frac{1}{2}) = -\mathbf{e}(x),\qquad \mathbf{e}(x + \frac{3}{4}) = -i\mathbf{e}(x),\qquad \mathbf{e}(x + 1) = \mathbf{e}(x).
$$
La fonction $\mathbf{e}(x)$ est périodique et 1 est période principale de cette fonction.

#### Remarque {#top-viii-s2-n1-rem-2 .statement}

L’application $x + iy \mapsto e^x \mathbf{e}(y)$ est un morphisme strict du groupe additif $\mathbf{C}$ sur le groupe multiplicatif $\mathbf{C}^*$, et sa restriction à un voisinage convenable de 0 est un isomorphisme local de $\mathbf{C}$ à $\mathbf{C}^*$. Par suite (VII, p. 14, remarque), tout morphisme strict de $\mathbf{C}$ sur $\mathbf{C}^*$ est de la forme $x + iy \mapsto e^{\alpha x + \beta y} \mathbf{e}(\gamma x + \delta y)$, où $\alpha, \beta, \gamma, \delta$ sont des nombres réels quelconques tels que $\alpha \delta - \beta \gamma \neq 0$. Nous verrons plus tard (FVR, III, § 1, n° 5) qu’il existe un seul de ces homomorphismes, qu’on note $z \mapsto e^z$, tel que $\lim_{z \to 0} (e^z - 1)/z = 1$; la restriction de cet homomorphisme à l’axe réel est identique à $e^x$ (d’où la notation).

### 2. Angles de demi-droites

Le corps $\mathbf{R}$ étant ordonné, nous orienterons le plan numérique $\mathbf{R}^2$ en prenant $\mathbf{e}_1 \wedge \mathbf{e}_2$ comme bivecteur positif ($\mathbf{e}_1, \mathbf{e}_2$ étant les vecteurs de la base canonique);

dans le plan numérique orienté $\mathbf{R}^2$ (identifié à $\mathbf{C}$ dans ce qui suit), on peut alors définir l’angle $(\Delta_1, \Delta_2)$ d’un couple quelconque $(\Delta_1, \Delta_2)$ de demi-droites.$^1$ L’ensemble $\mathcal{A}$ des angles de demi-droites est muni d’une structure de groupe commutatif (noté additivement), définie par

$$
(\Delta_1, \Delta_3) = (\Delta_1, \Delta_2) + (\Delta_2, \Delta_3),
$$

d’où en particulier, $(\Delta_1, \Delta_1) = 0, (\Delta_2, \Delta_1) = -(\Delta_1, \Delta_2)$.

L’angle plat $\overline{\omega}$ est la solution $\neq 0$ de l’équation $2\theta = 0$ dans $\mathcal{A}$; c’est l’angle que fait le demi-axe réel négatif avec le demi-axe réel positif.

Pour tout nombre complexe $z \neq 0$, on appelle amplitude de $z$, et l’on note $\mathrm{Am}(z)$, l’angle que fait avec le demi-axe réel positif la demi-droite d’origine 0 passant par $z$. L’application $z \mapsto \mathrm{Am}(z)$ est un homomorphisme du groupe multiplicatif $\mathbf{C}^*$ sur le groupe additif $\mathcal{A}$; on a donc

$$
\mathrm{Am}(zz') = \mathrm{Am}(z) + \mathrm{Am}(z') \quad \text{et} \quad \mathrm{Am}(\overline{z}) = \mathrm{Am}(z^{-1}) = -\mathrm{Am}(z).
$$

L’angle $\delta = \mathrm{Am}(i)$ s’appelle angle droit positif; c’est une des solutions, dans le groupe $\mathcal{A}$, de l’équation $2\theta = \overline{\omega}$, l’autre étant $-\delta = \delta + \overline{\omega}$.

L’homomorphisme $z \mapsto \mathrm{Am}(z)$, restreint au sous-groupe $\mathbf{U}$ de $\mathbf{C}^*$, est un isomorphisme de la structure de groupe de $\mathbf{U}$ sur celle de $\mathcal{A}$; si on transporte au groupe $\mathcal{A}$, par cet isomorphisme, la topologie de $\mathbf{U}$, $\mathcal{A}$ devient un groupe topologique compact, et l’homomorphisme $z \mapsto \mathrm{Am}(z)$ de $\mathbf{C}^*$ sur $\mathcal{A}$ est un morphisme strict du groupe topologique $\mathbf{C}^*$ sur le groupe topologique $\mathcal{A}$.

Désignons par $\theta \mapsto f(\theta)$ l’isomorphisme de $\mathcal{A}$ sur $\mathbf{U}$, réciproque de l’isomorphisme $z \mapsto \mathrm{Am}(z)$ de $\mathbf{U}$ sur $\mathcal{A}$. Par définition (A, IX, § 10, n° 3), $\Re(f(\theta))$ se note $\cos \theta$ et s’appelle cosinus de l’angle $\theta$, $\Im(f(\theta))$ se note $\sin \theta$ et s’appelle sinus de l’angle $\theta$. Ces fonctions sont continues dans le groupe topologique $\mathcal{A}$, et satisfont aux relations suivantes (*loc. cit.*), conséquences immédiates des définitions qui précèdent:

$$
\begin{align*}
\cos 0 &= 1, & \sin 0 &= 0, & \cos \overline{\omega} &= -1, & \sin \overline{\omega} &= 0, \\
\cos(-\theta) &= \cos \theta, & \sin(-\theta) &= -\sin \theta, \\
\cos(\theta + \theta') &= \cos \theta \cos \theta' - \sin \theta \sin \theta', \\
\sin(\theta + \theta') &= \sin \theta \cos \theta' + \sin \theta' \cos \theta, \\
\cos^2 \theta + \sin^2 \theta &= 1.
\end{align*}
$$

Par définition, la tangente $\mathrm{tg}(\theta)$ d’un angle $\theta \in \mathcal{A}$ est l’élément de $\tilde{\mathbf{R}}$, qui vaut $\sin \theta / \cos \theta$ lorsque $\theta \neq \delta$ et $\theta \neq -\delta$, et vaut $\infty$ lorsque $\theta = \delta$ ou $\theta = -\delta$.

\footnotetext{1 Rappelons (A, IX, § 10, n° 3) qu’on définit, dans l’ensemble des couples $(\Delta_1, \Delta_2)$ de demi-droites d’origine 0, une relation d’équivalence, en considérant deux couples $(\Delta_1, \Delta_2)$ et $(\Delta'_1, \Delta'_2)$ comme équivalents s’il existe une même rotation qui transforme $\Delta_1$ en $\Delta'_1$ et $\Delta_2$ en $\Delta'_2$; l’angle du couple $(\Delta_1, \Delta_2)$ (ou angle que fait $\Delta_2$ avec $\Delta_1$) est par définition la classe d’équivalence de ce couple.}

La fonction tg est une application continue de $\mathfrak{A}$ dans $\tilde{\mathbf{R}}$; on a $\operatorname{tg}(\theta + \overline{\omega}) = \operatorname{tg} \theta$. On appelle cotangente de $\theta$, et on note cotg $\theta$, l’élément de $\tilde{\mathbf{R}}$ égal à $1/\operatorname{tg} \theta$.

On notera que, si $\operatorname{Am}(z) = \theta$, on a $z = |z| (\cos \theta + i \sin \theta)$; cette expression s’appelle la forme trigonométrique du nombre complexe $z \neq 0$.

### 3. Mesure des angles de demi-droites

D’après le th. 1 de VIII, p. 7, le groupe topologique $\mathfrak{A}$ des angles de demi-droites est isomorphe à $\mathbf{T}$. Tout morphisme strict de $\mathbf{R}$ sur $\mathfrak{A}$ s’obtient en composant l’isomorphisme $z \mapsto \operatorname{Am}(z)$ de $\mathbf{U}$ sur $\mathfrak{A}$ et un morphisme strict de $\mathbf{R}$ sur $\mathbf{U}$; si l’on pose $\vartheta(x) = \operatorname{Am}(\mathbf{e}(x))$, tout morphisme strict de $\mathbf{R}$ sur $\mathfrak{A}$ est donc de la forme $x \mapsto \vartheta(x/a)$ ($a \neq 0$). Étant donné un nombre $a > 0$, fixé une fois pour toutes, tout angle $\theta$ correspond, par l’homomorphisme $x \mapsto \vartheta(x/a)$, à une classe de nombres réels modulo $a$ (élément de $\mathbf{R}/a\mathbf{Z}$) qu’on appelle la mesure de $\theta$ relativement à la base $a$; par abus de langage, tout nombre réel de cette classe est appelé une mesure de $\theta$; l’angle $\vartheta(x/a)$ est l’angle de mesure $x$ (relativement à la base $a$). Si $x$ est une mesure de $\theta$, $x'$ une mesure de $\theta'$ (relativement à la même base), $x + x'$ est une mesure de $\theta + \theta'$, $-x$ une mesure de $-\theta$. On appelle parfois mesure principale d’un angle (relativement à base $a$) celle de ses mesures qui appartient à l’intervalle $[0, a[$.

Choix d’une base $a$. — On se borne toujours à considérer des bases $a > 1$. À chaque $a > 1$ correspond un angle de demi-droites $\omega = \vartheta(1/a)$ dont la mesure principale est 1, et qu’on appelle unité d’angle relative à la base $a$; réciproquement, pour tout angle $\omega \neq 0$, il existe un $a > 1$ et un seul tel que $\vartheta(1/a) = \omega$, donc la donnée de l’unité d’angle $\omega$ détermine entièrement la base $a > 1$.
Lorsqu’on prend $a = 360$ l’unité d’angle correspondante s’appelle le degré.
En Analyse, on utilise la base $a$ définie par la condition
$$
\lim_{x \to 0} \frac{\mathbf{e}(x/a) - 1}{x} = i,
$$
nombre qu’on désigne par $2\pi$ (nous démontrerons plus tard (FVR, III, § 1, n° 3) l’existence d’un tel nombre et indiquerons comment on peut en calculer des valeurs approchées); l’unité d’angle correspondante est appelée radian. Avec la définition de $e^z$ pour $z$ complexe signalée ci-dessus, on a $\mathbf{e}(x) = e^{2\pi ix}$ pour tout $x \in \mathbf{R}$.

Une fois choisie une base $a$, lorsqu’on parle d’un angle de demi-droites, on entend le plus souvent une mesure de cet angle relativement à la base $a$; cet abus de langage n’a pas d’inconvénient si (comme c’est toujours le cas tant qu’on ne fait pas de calculs numériques) la base $a$ reste fixe dans les raisonnements, et si l’on se souvient que deux nombres réels congrus mod. $a$ correspondent au même angle de demi-droites.

Par exemple, ce qu’on entendra le plus souvent par amplitude d’un nombre complexe $z \neq 0$, sera une mesure en radians de cet angle, fixée par des conventions qui dépendront de la question étudiée; une fois ces conventions faites, on notera encore $\operatorname{Am}(z)$ la mesure de l’amplitude ainsi choisie.

### 4. Fonctions trigonométriques

Si on compose les fonctions cos θ, sin θ, tg θ, cotg θ (définies dans $\mathfrak{A}$) avec l’homomorphisme $x \mapsto \vartheta(x/a)$ de $\mathbf{R}$ sur $\mathfrak{A}$, les fonctions cos $\vartheta(x/a)$, sin $\vartheta(x/a)$, tg $\vartheta(x/a)$, cotg $\vartheta(x/a)$ ainsi obtenues s’appellent respectivement *cosinus*, *sinus*, *tangente* et *cotangente* du *nombre* $x$ relatifs à la base $a$, et se notent $\cos_a x$, $\sin_a x$, $\tg_a x$, et $\cotg_a x$. L’application $x \mapsto \cos_a x + i \sin_a x$ est composée de $\theta \mapsto \cos \theta + i \sin \theta$ et de $x \mapsto \vartheta(x/a)$, d’où, en vertu de la définition de cos θ et sin θ (VIII, p. 9), l’identité

$$
\mathbf{e}\left(\frac{x}{a}\right) = \cos_a x + i \sin_a x,
$$

qui équivaut à

$$
\cos_a x = \Re\left(\mathbf{e}\left(\frac{x}{a}\right)\right), \quad \sin_a x = \Im\left(\mathbf{e}\left(\frac{x}{a}\right)\right),
$$

et aussi, d’après (4), à

$$
\cos_a x = \frac{1}{2} \left( \mathbf{e}\left(\frac{x}{a}\right) + \mathbf{e}\left(-\frac{x}{a}\right) \right), \quad \sin_a x = \frac{1}{2i} \left( \mathbf{e}\left(\frac{x}{a}\right) - \mathbf{e}\left(-\frac{x}{a}\right) \right).
$$

On en conclut les identités

$$
\cos_b x = \cos_a \left( \frac{ax}{b} \right), \quad \sin_b x = \sin_a \left( \frac{ax}{b} \right).
$$

Lorsqu’on choisit la base $a = 2\pi$ dont il a été question plus haut on note simplement cos $x$, sin $x$, tg $x$, cotg $x$ les fonctions cos$_{2\pi} x$, sin$_{2\pi} x$, tg$_{2\pi} x$, cotg$_{2\pi} x$. Les formules (6) permettent d’ailleurs d’en déduire les valeurs des fonctions trigonométriques relatives à une base quelconque.

Les relations rappelées plus haut entre cosinus et sinus d’angles donnent évidemment les mêmes relations entre cosinus et sinus des *nombres* qui mesurent ces angles; en particulier, on a

$$
\begin{align*}
\cos_a(x + y) &= \cos_a x \cos_a y - \sin_a x \sin_a y, \\
\sin_a(x + y) &= \sin_a x \cos_a y + \sin_a y \cos_a x, \\
\cos_a(-x) &= \cos_a x, \quad \sin_a(-x) = -\sin_a x, \\
\cos_a^2 x + \sin_a^2 x &= 1.
\end{align*}
$$

Les fonctions cos$_a x$ et sin$_a x$ sont continues dans $\mathbf{R}$, et périodiques de période $a$; $a$ est d’ailleurs *période principale* de ces fonctions; en effet, la relation cos$_a x = \cos_a y$ entraîne sin$_a x = \sin_a y$ ou sin$_a x = -\sin_a y$, c’est-à-dire $\mathbf{e}(x/a) = \mathbf{e}(y/a)$ ou $\mathbf{e}(x/a) = \mathbf{e}(-y/a)$, donc $x \equiv y$ (mod. $a$) ou $x \equiv -y$ (mod. $a$); on voit de même que sin$_a x = \sin_a y$ est équivalente à $x \equiv y$ (mod. $a$) ou $x + y \equiv \frac{1}{2}a$ (mod. $a$).

Il résulte de ce qui précède que $\cos_a x$ ne prend jamais deux fois la même valeur dans l’intervalle $(0, \frac{1}{2}a)$; restreinte à cet intervalle, c’est donc une application *bijective* de cet intervalle sur l’intervalle $(-1, +1)$. Comme $\cos_a 0 = 1$, $\cos_a (\frac{1}{2}a) = -1$, $x \mapsto \cos_a x$ est une application *strictement décroissante* de $(0, \frac{1}{2}a)$ sur $(-1, 1)$ (IV, p. 9 et 10, th. 5 et *Remarque*). On a $\cos_a x = 0$ pour $x = a/4$, $\cos_a x > 0$ pour $0 \leq x < a/4$, $\cos_a x < 0$ pour $a/4 < x \leq a/2$. Comme $\cos_a(-x) = \cos_a x$, on en déduit la variation de $\cos_a x$ dans l’intervalle $(-\frac{1}{2}a, 0)$, puis dans tout $\mathbf{R}$ par périodicité (fig. 8). Comme $\sin_a x = -\cos_a(x + a/4)$, on en déduit la variation de $\sin_a x$ dans $\mathbf{R}$ (fig. 8).

![Figure 8](https://i.imgur.com/8zZzZzZ.png)

Figure 8

La fonction $\tg_a x$ est une application continue de $\mathbf{R}$ sur $\overline{\mathbf{R}}$; elle prend la valeur $\infty$ pour les valeurs $a/4 + k(a/2)$ ($k$ entier quelconque). Comme elle admet pour période $\frac{1}{2}a$, $\frac{1}{2}a$ en est une *période principale*. Dans l’intervalle $(0, a/4)$, $\sin_a x$ croît de 0 à 1, $\cos_a x$ décroît de 1 à 0, donc $\tg_a x$ est *strictement croissante* dans $(0, a/4)$, et applique $(0, a/4)$ sur $(0, +\infty)$; on en conclut que $\tg_a x$ est strictement croissante dans $]-a/4, +a/4[$, et est un homéomorphisme de cet intervalle sur $\mathbf{R}$ (fig. 9).

![Figure 9](https://i.imgur.com/8zZzZzZ.png)

Figure 9

### 5. Secteurs angulaires

Étant données deux demi-droites fermées distinctes $\Delta_1, \Delta_2$ d’origine 0, soit $x$ la mesure principale de l’angle $(\Delta_1, \Delta_2)$ (relative à une base $a$ choisie une fois pour toutes). La réunion des demi-droites fermées (resp. ouvertes) $\Delta$ d’origine 0 telles que la mesure principale $y$ de l’angle $(\Delta_1, \Delta)$ satisfasse à $0 \leq y \leq x$ (resp. $0 < y < x$) est identique au secteur angulaire fermé (resp. ouvert) S d’origine $\Delta_1$ et d’extrémité $\Delta_2$, défini en Algèbre (A, IX, § 10, n° 4).

![Figure 10](figure.png)

En effet, par une rotation, on peut toujours se ramener au cas où S ne contient pas la demi-droite passant par le point –1. Si $\alpha$ et $\beta$ sont les angles que font alors $\Delta_1$ et $\Delta_2$ respectivement avec le demi-axe réel positif, le secteur angulaire fermé S n’est autre (A, IX, § 10, n° 4, prop. 12) que la réunion des demi-droites fermées $\Delta$ faisant avec le demi-axe réel positif un angle $\theta$ tel que

$$
\tg \frac{\alpha}{2} \leq \tg \frac{\theta}{2} \leq \tg \frac{\beta}{2}.
$$

Or, si $u, v, t$ sont les mesures de $\alpha, \beta, \theta$ respectivement, contenues dans l’intervalle $] -a/2, +a/2[$, ces inégalités équivalent à $\tg_a u/2 \leq \tg_a t/2 \leq \tg_a v/2$, et comme $\tg_a x$ est une fonction croissante dans $] -a/4, +a/4[$, elles équivalent aussi à $u \leq t \leq v$ ou à $0 \leq t - u \leq v - u$; comme $x = v - u, y = t - u$, la proposition est démontrée pour les secteurs angulaires fermés; on raisonne de même pour les secteurs angulaires ouverts.

Un secteur angulaire fermé est un ensemble fermé dans $\mathbf{R}^2$; le secteur angulaire ouvert de même origine et même extrémité est son intérieur dans $\mathbf{R}^2$ (VI, p. 10, prop. 3). L’angle $(\Delta_1, \Delta_2)$ de mesure principale $x$, s’appelle l’ouverture du secteur S; S est dit saillant si $x < \frac{1}{2}a$, plat (ou demi-plan fermé) si $x = \frac{1}{2}a$, rentrant si $x > \frac{1}{2}a$; un secteur angulaire saillant est dit aigu si $x < a/4$, droit (ou quadrant) si $x = a/4$, obtus si $x > a/4$. La bissectrice du secteur S n’est autre que la demi-droite $\Delta$ faisant avec $\Delta_1$ un angle $y = \frac{1}{2}x$.

Deux demi-droites fermées distinctes $\Delta_1, \Delta_2$ définissent deux secteurs angulaires fermés : celui d’origine $\Delta_1$ et d’extrémité $\Delta_2$, et celui d’origine $\Delta_2$ et d’extrémité $\Delta_1$; leur réunion est le plan numérique $\mathbf{R}^2$, leur intersection est la réunion de $\Delta_1$ et $\Delta_2$.

### 6. Angles de droites

On a aussi défini en Algèbre (A, IX, § 10, n° 3) la notion d’angle d’un couple de deux droites dans un espace vectoriel à deux dimensions sur un corps ordonné maximal¹ ; cette définition s’applique en particulier au plan numérique $\mathbf{R}^2$. L’ensemble $\mathcal{A}_0$ des angles de droites est muni d’une structure de groupe commutatif (noté additivement), définie par

$$
(\widehat{D_1, D_3}) = (\widehat{D_1, D_2}) + (\widehat{D_2, D_3}),
$$

d’où en particulier

$$
(\widehat{D_1, D_1}) = 0, \qquad (\widehat{D_2, D_1}) = -(\widehat{D_1, D_2}).
$$

L’angle droit $\delta_0$ est la solution $\neq 0$ de l’équation $2\theta = 0$ dans $\mathcal{A}_0$; c’est l’angle que fait l’axe imaginaire avec l’axe réel.

On définit un homomorphisme canonique $\varphi$ du groupe $\mathcal{A}$ des angles de demi-droites sur le groupe $\mathcal{A}_0$ des angles de droites en faisant correspondre, à l’angle que fait une demi-droite $\Delta$ avec le demi-axe réel positif, l’angle que fait la droite D contenant $\Delta$ avec l’axe réel (A, IX, § 10, n° 1, cor. de la prop. 3); un angle de droites $\theta_0$ est l’image par $\varphi$ de deux angles de demi-droites $\theta, \theta + \overline{\omega}$; autrement dit, $\mathcal{A}_0$ est isomorphe au groupe quotient de $\mathcal{A}$ par le sous-groupe $\{0, \overline{\omega}\}$. Si on transporte à $\mathcal{A}_0$ la topologie du groupe quotient $\mathcal{A}/\{0, \overline{\omega}\}$ (par l’homomorphisme bijectif associé à $\varphi$), $\mathcal{A}_0$ devient un groupe topologique compact, $\varphi$ un morphisme strict de $\mathcal{A}$ sur $\mathcal{A}_0$.

Si on compose l’homomorphisme $\varphi$ de $\mathcal{A}$ sur $\mathcal{A}_0$ et l’homomorphisme $x \mapsto \vartheta(x/a)$ de $\mathbf{R}$ sur $\mathcal{A}$ on obtient un homomorphisme $x \mapsto \vartheta_0(x/a)$ de $\mathbf{R}$ sur $\mathcal{A}_0$; tout angle $\theta_0 \in \mathcal{A}_0$ correspond, par cet homomorphisme, à une classe de nombres réels mod. $\frac{1}{2}a$, qu’on appelle encore mesure de $\theta_0$ (relativement à la base $a$); par abus de langage, tout nombre de cette classe est aussi appelé une mesure de $\theta_0$, et celui qui appartient à $[0, a/2[$ la mesure principale de $\theta_0$; l’angle $\vartheta_0(x/a)$ est l’angle de droites de mesure $x$. Toute mesure de $\theta_0$ est aussi une mesure d’un des deux angles de demi-droites $\theta, \theta + \overline{\omega}$ dont $\theta_0$ est l’image par l’homomorphisme $\varphi$.

¹ Rappelons que, dans l’ensemble des couples $(D_1, D_2)$ de droites non isotropes, on définit une relation d’équivalence en considérant deux couples $(D_1, D_2)$ et $(D'_1, D'_2)$ comme équivalents, s’il existe une même similitude directe qui transforme $D_1$ en $D'_1$ et $D_2$ en $D'_2$; l’angle du couple $(D_1, D_2)$ est la classe d’équivalence de ce couple.

Ici encore, une fois choisie la base $a$, lorsqu’on parle d’un angle de droites, on entend le plus souvent, par abus de langage, une mesure de cet angle relativement à la base $a$.

#### Remarque {#top-viii-s2-n6-rem-1 .statement}

On définit un homomorphisme de $\mathbf{C}^*$ sur $\mathfrak{A}_0$ en faisant correspondre à tout nombre complexe $z \neq 0$ l’angle que fait la droite passant par 0 et $z$ avec l’axe réel; il est clair que cet homomorphisme est composé de $\varphi$ et de l’homomorphisme $z \mapsto \mathrm{Am}(z)$ de $\mathbf{C}^*$ sur $\mathfrak{A}$; c’est donc un morphisme strict du groupe topologique $\mathbf{C}^*$ sur le groupe topologique $\mathfrak{A}_0$, et la représentation bijective associée est un isomorphisme du groupe quotient $\mathbf{C}^*/\mathbf{R}^*$ sur $\mathfrak{A}_0$.

On sait (A, IX, § 10, no 3) que, si D désigne une droite faisant un angle $\theta_0$ avec l’axe réel, $(a, b)$ un couple de paramètres directeurs de D, la tangente de l’angle $\theta_0$ (qui se note encore $\tg \theta_0$) est l’élément $b/a$ de $\tilde{\mathbf{R}}$ ($= \infty$ si $a = 0$), qu’on appelle aussi la pente de la droite D. Si $\theta$ et $\theta + \overline{\omega}$ sont les deux angles de demi-droites dont $\theta_0$ est l’image par l’homomorphisme $\varphi$, on a $\tg \theta_0 = \tg \theta = \tg (\theta + \overline{\omega})$. L’application $\theta_0 \mapsto \tg \theta_0$ est un homéomorphisme de $\mathfrak{A}_0$ sur $\tilde{\mathbf{R}}$, car l’espace topologique $\mathbf{C}^*/\mathbf{R}^*$ n’est autre que la droite projective réelle $\mathbf{P}_1$, et l’on sait (VI, p. 16) que l’application qui fait correspondre à une droite (considérée comme point de $\mathbf{P}_1$) sa pente, est un homéomorphisme de $\mathbf{P}_1$ sur $\tilde{\mathbf{R}}$. Si maintenant on transporte à $\tilde{\mathbf{R}}$ la structure de groupe de $\mathfrak{A}_0$ par l’application $\theta_0 \mapsto \tg \theta_0$, on définit sur $\tilde{\mathbf{R}}$ une structure de groupe topologique commutatif, où le composé de deux éléments $t_1, t_2$ est $(t_1 + t_2)/(1 - t_1 t_2)$ quand $t_1$ et $t_2$ appartiennent à $\mathbf{R}$ et sont tels que $t_1 t_2 \neq 1$; pour les couples $(t_1, t_2)$ qui ne satisfont pas à ces conditions, le composé de $t_1$ et $t_2$ s’obtient en prolongeant par continuité la fonction $(x + y)/(1 - xy)$ à $\tilde{\mathbf{R}} \times \tilde{\mathbf{R}}$, et se note encore $(t_1 + t_2)/(1 - t_1 t_2)$.

Si $\theta$ est un angle de droites, on note souvent $2\theta$ le double commun des deux angles de demi-droites dont $\theta$ est l’image. L’application $\theta \mapsto 2\theta$ est un isomorphisme du groupe topologique $\mathfrak{A}_0$ des angles de droites sur le groupe topologique $\mathfrak{A}$ des angles de demi-droites, dont le composé avec la projection canonique de $\mathfrak{A}$ sur $\mathfrak{A}_0$ est la multiplication par l’entier 2 dans le groupe commutatif $\mathfrak{A}_a$. Avec cette notation, on a les formules suivantes (A, IX, pp. 75–83).

$$
\begin{align*}
\sin_a 2\theta &= 2 \tg_a \theta/(1 + \tg_a^2 \theta) \\
\cos_a 2\theta &= (1 - \tg_a^2 \theta)/(1 + \tg_a^2 \theta) \\
\tg_a 2\theta &= 2 \tg_a \theta/(1 - \tg_a^2 \theta),
\end{align*}
$$

qui sont des identités entre fonctions continues sur $\mathfrak{A}_0$ à valeurs dans $\tilde{\mathbf{R}}$ (VI, p. 16).

## EXERCICES {#top-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
