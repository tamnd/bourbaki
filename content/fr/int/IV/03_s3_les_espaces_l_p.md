---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 3
section_title: Les espaces $L^p$
lang: fr
source: int-i-iv-fr
pdf_pages: 0127-0144, 0240-0240
extraction: ocr
subsections:
    - "no": 1
      title: L’inégalité de Minkowski
      page: 0
      pdf_page: 127
    - "no": 2
      title: Les semi-normes $N_p$
      page: 0
      pdf_page: 128
    - "no": 3
      title: Les espaces $\mathcal{F}_F^p$
      page: 0
      pdf_page: 130
    - "no": 4
      title: Fonctions de puissance $p$-ième intégrable
      page: 0
      pdf_page: 133
    - "no": 5
      title: Propriétés des fonctions de puissance p-ième intégrable
      page: 0
      pdf_page: 136
    - "no": 6
      title: Ensembles filtrants dans $L^p$ et suites croissantes dans $\mathcal{L}^p$
      page: 0
      pdf_page: 138
    - "no": 7
      title: Le théorème de Lebesgue
      page: 0
      pdf_page: 141
    - "no": 8
      title: Relations entre les espaces $\mathcal{L}_F^p (1 \leq p < + \infty)$.
      page: 0
      pdf_page: 143
statements: 41
exercises: 3
content_sha256: 61760e6cfcafeebf70f25c4fb21240e701896916261c808b88c7da4cffb6a768
---

## § 3. Les espaces $L^p$

### 1. L’inégalité de Minkowski

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$. Dans l’ensemble des fonctions numériques *positives* (finies ou non) définies dans X, la fonction $|\mu|^*(f)$ est positive, positivement homogène, croissante et convexe (§ 1, n° 3, prop. 10, 11 et 12).

#### Proposition 1 {#int-iv-s3-prop-1 .statement}

Pour tout nombre réel fini $p \geq 1$ et tout couple de fonctions positives $f, g$ (finies ou non) définies dans X, on a
$$(1)\quad (|\mu|^*((f + g)^p))^{1/p} \leq (|\mu|^*(f^p))^{1/p} + (|\mu|^*(g^p))^{1/p}$$
(inégalité de Minkowski).

En effet, l’inégalité (1) est évidente lorsque l’un des termes du second membre est égal à $+\infty$. Dans le cas contraire, $f$ et $g$ sont presque partout finies (§ 2, n° 3, prop. 7). Si $f_1$ et $g_1$ sont des fonctions finies et positives équivalentes à $f$ et $g$ respectivement, $f_1^p, g_1^p$ et $(f_1 + g_1)^p$ sont équivalentes à $f^p, g^p$ et $(f + g)^p$ respectivement, et comme deux fonctions positives équivalentes ont même intégrale supérieure (§ 2, n° 3, prop. 6), tout revient à démontrer l’inégalité (1) dans le cas où $f$ et $g$ sont des fonctions partout finies ; mais dans ce cas, l’inégalité est un cas particulier de l’inégalité de Minkowski générale démontrée au chap. I, n° 2, prop. 3.

Nous aurons encore à utiliser l’inégalité élémentaire suivante : si $p \geq 1$, quels que soient les nombres $a \geq 0, b \geq 0$, on a
$$(2)\quad a^p + b^p \leq (a + b)^p.$$

En effet, l’inégalité est évidente si $a = b = 0$ ou si l’un des nombres $a, b$ est $+\infty$ ; si $a, b$ sont finis et $a + b > 0$, elle s’écrit
$$\left(\frac{a}{a + b}\right)^p + \left(\frac{b}{a + b}\right)^p \leq 1,$$
et résulte de ce que $\left(\frac{a}{a + b}\right)^p \leq \frac{a}{a + b}$,
$$\left(\frac{b}{a + b}\right)^p \leq \frac{b}{a + b}$$
et $\frac{a}{a + b} + \frac{b}{a + b} = 1$.

### 2. Les semi-normes $N_p$

Dans tout ce qui suit, F désignera un espace vectoriel normé complet (espace de Banach) sur le corps $\mathbf{R}$ ou le corps $\mathbf{C}$ ; la norme d’un élément $z \in F$ se notera $|z|$. Etant donnée une application f d’un ensemble A dans F, on notera $|f|$ l’application $x \mapsto |f(x)|$ de A dans $\mathbf{R}_+$ (on aura soin d’observer que $|f|$ est une fonction numérique, et non un nombre).

#### Définition 1 {#int-iv-s3-def-1 .statement}

Soient X un espace localement compact, $\mu$ une mesure sur X. Pour toute application f de X dans un espace de Banach F, et tout nombre p tel que $1 \leq p < +\infty$, on désigne par $N_p(f, \mu)$, ou simplement par $N_p(f)$, le nombre positif $\left( \int^* |f|^p d|\mu| \right)^{1/p}$

On notera que le nombre $N_p(f)$ peut être égal à $+\infty$.

#### Proposition 2 {#int-iv-s3-prop-2 .statement}

Si f et g sont deux applications de X dans F, et $\alpha$ un scalaire quelconque $\neq 0$, on a, pour $1 \leq p < +\infty$,

(3)
$$
N_p(\alpha f) = |\alpha| N_p(f)
$$

(4)
$$
N_p(f + g) \leq N_p(f) + N_p(g).
$$

En effet, la relation (3) découle aussitôt de la déf. 1 et du fait que $|\mu|^*$ est positivement homogène ; d’autre part, comme $|f + g| \leq |f| + |g|$, l’inégalité (4) résulte de l’inégalité de Minkowski (1) et du fait que $|\mu|^*$ est croissante.

Nous étendrons la déf. 1 au cas des fonctions numériques finies ou non, définies dans X, en posant encore

$$
N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}
$$

pour une telle fonction $f$. On voit aussitôt que les relations (3) et (4) sont encore valables pour ces fonctions lorsque $f + g$ est définie dans X et $\alpha \neq 0$. En outre :

**Théorème 1** (théorème de convexité dénombrable). — Soit $(f_n)$ une suite de fonctions $\geq 0$ (finies ou non) définies dans X. Pour $1 \leq p < +\infty$, on a

(5)
$$
N_p \left( \sum_{n=1}^\infty f_n \right) \leq \sum_{n=1}^\infty N_p(f_n).
$$

Posons en effet $f = \sum_{n=1}^\infty f_n$; $f$ est l’enveloppe supérieure de la suite croissante des fonctions $g_n = \sum_{k=1}^n f_k$; la définition de $N_p(f)$ et le th. 3 du § 1, n° 3 montrent que $N_p(f) = \sup_n N_p(g_n)$. Mais on a $N_p(g_n) \leq \sum_{k=1}^n N_p(f_k)$ en vertu de la prop. 2, d’où l’inégalité (5).

#### Proposition 3 {#int-iv-s3-prop-3 .statement}

Si f et g sont deux applications équivalentes de X dans un espace de Banach F, on a $N_p(f - g) = 0$ pour $1 \leq p < +\infty$; réciproquement, si $N_p(f - g) = 0$ pour une valeur de $p \geq 1$, f et g sont équivalentes.

La proposition résulte aussitôt du th. 1 du § 2, n° 3.

Si f et g sont deux applications équivalentes de X dans F, on a $N_p(f) = N_p(g)$ pour tout $p \geq 1$ ($§ 2$, n° 3, prop. 6); $N_p(f)$ ne dépend donc que de la classe $\tilde{f}$ de f, et l’on pose par définition $N_p(\tilde{f}) = N_p(f)$. Comme les classes d’applications de X dans F forment un espace vectoriel ($§ 2$, n° 4), les relations (3) et (4) peuvent aussi s’écrire

$$
N_p(\alpha \tilde{f}) = |\alpha| N_p(\tilde{f})
$$
$$
N_p(\tilde{f} + \tilde{g}) \leq N_p(\tilde{f}) + N_p(\tilde{g}).
$$

On définit de même $N_p(\tilde{f})$ pour toute classe de fonctions numériques équivalentes (finies ou non).

On peut par suite définir $N_p(f)$ pour une fonction à valeurs dans F (resp. dans $\bar{\mathbf{R}}$) définie presque partout dans X, en posant $N_p(f) = N_p(\tilde{f})$; il est clair alors que les relations (3) et (4) sont encore valables (en supposant $\alpha \neq 0$ et $f + g$ définie presque partout, lorsqu’il s’agit de fonctions numériques, finies ou non).

Si $0 < p < 1$, on pose encore $N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}$, mais les inégalités (4) et (5) ne sont plus valables (cf. chap. I, exerc. 5 et chap. IV, § 6, exerc. 13).

### 3. Les espaces $\mathcal{F}_F^p$

Soient F un espace de Banach, $\mathcal{F}(X; F)$ (ou simplement $\mathcal{F}_F$) l’espace vectoriel de toutes les applications de X dans F. Pour $1 \leq p < +\infty$ nous désignerons par $\mathcal{F}^p(X, \mu; F)$ ou $\mathcal{F}_F^p(X, \mu)$, ou simplement $\mathcal{F}_F^p(\mu)$, ou $\mathcal{F}_F^p$ (si aucune confusion n’en résulte), l’ensemble des applications f de X dans F telles que $N_p(f) < +\infty$ (on écrit $\mathcal{F}^p$ au lieu de $\mathcal{F}_R^p$). Il est clair que $\mathcal{F}_F^p(|\mu|) = \mathcal{F}_F^p(\mu)$. Il résulte aussitôt de la prop. 2 du n° 2 que $\mathcal{F}_F^p$ est un sous-espace vectoriel de $\mathcal{F}_F$, et que $N_p(f)$ est une semi-norme sur cet espace. Nous supposerons toujours (sauf mention expresse du contraire) que $\mathcal{F}_F^p$ est muni de la topologie définie par cette semi-norme; nous dirons que cette topologie est la topologie de la convergence en moyenne d’ordre p (pour $p = 1$, on l’appelle simplement la topologie de la convergence en moyenne; pour $p = 2$, on dit aussi « topologie de la convergence en moyenne quadratique »). On dira qu’un filtre $\mathcal{G}$ sur $\mathcal{F}_F^p$ (resp. une suite $(f_n)$ d’éléments de $\mathcal{F}_F^p$), qui converge vers $f$ pour cette topologie converge en moyenne d’ordre $p$ vers $f$; cela signifie donc que $N_p(g - f)$ tend vers 0 suivant $\mathcal{G}$ (resp. que $N_p(f_n - f)$ tend vers 0 lorsque $n$ croît indéfiniment).

On étend aussitôt cette terminologie au cas où les fonctions $f_n$ et la fonction $f$ sont seulement définies presque partout (ou à valeurs dans $\bar{\mathbf{R}}$, définies et finies presque partout).

On notera que l’espace localement convexe $\mathcal{F}_F^p$ n’est pas séparé en général; l’adhérence de 0 dans cet espace est le sous-espace $\mathcal{N}_F$ des applications négligeables de $X$ dans $F$ (n° 1, prop. 3).

#### Remarque {#int-iv-s3-n3-rem-1 .statement}

Soit $F$ un espace de Banach sur le corps $\mathbf{C}$ des nombres complexes; alors, pour toute fonction $f \in \mathcal{F}_F^p$ et tout nombre complexe $\alpha$, $\alpha f$ appartient à $\mathcal{F}_F^p$, et l’on a $N_p(\alpha f) = |\alpha| N_p(f)$; en d’autres termes, $\mathcal{F}_F^p$ est aussi un espace vectoriel sur $\mathbf{C}$, et $N_p(f)$ une semi-norme sur cet espace vectoriel complexe (cf. Esp. vect. top., chap. II, 2e éd., § 1).

#### Proposition 4 {#int-iv-s3-prop-4 .statement}

Soit $\mathcal{B}$ une base de filtre sur $\mathcal{F}_F^p$. On suppose qu’il existe un ensemble compact $K \subset X$ tel que, pour toute partie $M \in \mathcal{B}$, toutes les applications $f \in M$ aient leur support dans $K$. Dans ces conditions, si $\mathcal{B}$ converge uniformément dans $X$ vers $f_0$, $f_0$ appartient à $\mathcal{F}_F^p$, et $\mathcal{B}$ converge en moyenne d’ordre $p$ vers $f_0$.

Il revient au même de dire que, sur l’ensemble des applications $f \in \mathcal{F}_F^p$ dont le support est contenu dans un ensemble compact fixe, la topologie de la convergence uniforme est plus fine que la topologie de la convergence en moyenne d’ordre $p$.

En effet, soit $h$ une application continue de $X$ dans $[0, 1]$, à support compact, égale à 1 dans $K$ (chap. III, § 1, n° 2, lemme 1). Pour tout $\varepsilon > 0$, il existe $M \in \mathcal{B}$ tel que, pour toute application $f \in M$, on ait $|f(x) - f_0(x)| \leq \varepsilon h(x)$ pour tout $x \in X$. On en déduit $N_p(f - f_0) \leq \varepsilon N_p(h)$, d’où la proposition.

#### Proposition 5 {#int-iv-s3-prop-5 .statement}

L’espace localement convexe $\mathcal{F}_F^p$ est complet.

Comme l’espace séparé associé à $\mathcal{F}_F^p$ est un espace normé, il suffit de prouver que toute suite de Cauchy $(f_n)$ dans $\mathcal{F}_F^p$ a une limite pour la topologie de la convergence en moyenne d’ordre $p$

(Top. gén., chap. IX, § 2, n° 6, prop. 9). Par hypothèse, pour tout $\varepsilon > 0$, il existe un entier $m_0$ tel que les relations $m \geq m_0, n \geq m_0$ entraînent $N_p(f_n - f_m) \leq \varepsilon$. On peut donc définir par récurrence sur $k$ une suite strictement croissante $(n_k)$ d’entiers $\geq 0$ tels que l’on ait $N_p(f_{n_{k+1}} - f_{n_k}) \leq 2^{-k}$. Si nous montrons que la série de terme général $g_k = f_{n_{k+1}} - f_{n_k} (k \geq 1)$ est convergente en moyenne d’ordre $p$, elle aura une somme $g \in \mathcal{F}_F^p$, et $f = g + f_{n_1}$ sera limite de la suite $(f_{n_k})$ dans $\mathcal{F}_F^p$; $f$ sera alors valeur d’adhérence de la suite $(f_n)$; comme cette suite est une suite de Cauchy, elle aura pour limite $f$ et la prop. 5 sera démontrée (Top. gén., chap. II, 3e éd., § 3, n° 2, cor. 2 de la prop. 5).

La prop. 5 est donc conséquence de la proposition suivante:

#### Proposition 6 {#int-iv-s3-prop-6 .statement}

Soit $(f_n)$ une suite de fonctions de $\mathcal{F}_F^p$, telle que $\sum_{n=1}^\infty N_p(f_n) < +\infty$. Dans ces conditions, la série de terme général $f_n(x) \in F$ est absolument convergente presque partout dans $X$. Si l’on pose $f(x) = \sum_{n=1}^\infty f_n(x)$ aux points où la série converge, et $f(x) = 0$ ailleurs, la fonction $f$ appartient à $\mathcal{F}_F^p$ et est somme de la série de terme général $f_n$ (pour la topologie de la convergence en moyenne d’ordre $p$); de façon précise, on a, pour tout $n \geq 0$,

$$
N_p\left(f - \sum_{k=1}^n f_k\right) \leq \sum_{k=n+1}^\infty N_p(f_k).
$$

Considérons en effet la fonction positive (finie ou non) $g(x) = \sum_{n=1}^\infty |f_n(x)|$. D’après le th. de convexité dénombrable (n° 2, th. 1), on a $N_p(g) \leq \sum_{n=1}^\infty N_p(f_n) < +\infty$; donc $g$ est finie presque partout (§ 2, n° 3, prop. 7), ce qui signifie que la série de terme général $f_n(x)$ est absolument convergente presque partout. Comme $F$ est complet, cette série est convergente presque partout, et l’on a, pour tout $x \in X$, $|f(x)| \leq \sum_{n=1}^\infty |f_n(x)| = g(x)$, d’où

$$
N_p(f) \leq N_p(g) \leq \sum_{n=1}^\infty N_p(f_n) < +\infty,
$$
ce qui prouve que $f$ appartient

à $\mathcal{F}_F^p$. D’autre part, pour tout entier $n$, on a
$$
|f(x) - \sum_{k=1}^n f_k(x)| \leq \sum_{k=n+1}^\infty |f_k(x)|
$$
presque partout, d’où $N_p\left(f - \sum_{k=1}^n f_k\right) \leq \sum_{k=n+1}^\infty N_p(f_k)$. Par hypothèse la série de terme général $N_p(f_n)$ est convergente ; pour tout $\varepsilon > 0$, il existe donc un entier $n$ tel que $\sum_{k=n+1}^\infty N_p(f_k) \leq \varepsilon$, et l’inégalité (8) prouve que $f$ est somme de la série de terme général $f_n$, pour la topologie de la convergence en moyenne d’ordre $p$.

Les propositions 5 et 6 sont donc complètement démontrées.

### 4. Fonctions de puissance $p$-ième intégrable

L’espace vectoriel $\mathscr{K}(X; F)$ (que nous noterons simplement $\mathscr{K}_F$ si aucune confusion n’est à craindre), formé des applications continues et à support compact de $X$ dans $F$, est évidemment un sous-espace de chacun des espaces vectoriels $\mathcal{F}_F^p$.

#### Définition 2 {#int-iv-s3-def-2 .statement}

Etant donnés un espace localement compact $X$, une mesure $\mu$ sur $X$ et un espace de Banach $F$, on désigne par $\mathscr{L}_F^p(X, \mu)$ (ou simplement $\mathscr{L}_F^p(\mu)$, ou $\mathscr{L}_F^p$) l’adhérence, dans l’espace localement convexe $\mathcal{F}_F^p(X, \mu)$, de l’espace vectoriel $\mathscr{K}(X; F)$ des applications continues et à support compact de $X$ dans $F$. On note $L_F^p(X, \mu)$ (ou $L_F^p(\mu)$, ou $L_F^p$) l’espace séparé (normé) associé à $\mathscr{L}_F^p(X, \mu)$. On dit que les fonctions appartenant à $\mathscr{L}_F^p$ sont des fonctions de puissance $p$-ième intégrable (*).

On a évidemment $\mathscr{L}_F^p(X, |\mu|) = \mathscr{L}_F^p(X, \mu)$ et $L_F^p(X, |\mu|) = L_F^p(X, \mu)$.

On écrira $\mathscr{L}^p$ et $L^p$ au lieu de $\mathscr{L}_R^p$ et $L_R^p$ (ou de $\mathscr{L}_C^p$ et $L_C^p$ lorsque cela n’entraîne pas de confusion). Si $F$ est un espace de Banach complexe, $\mathscr{L}_F^p$ et $L_F^p$ sont munis d’une structure d’espace vectoriel topologique sur le corps $\mathbf{C}$ (n° 3, Remarque).

Il est clair que toute fonction de $\mathcal{F}_F^p$, équivalente à une fonction de $\mathscr{L}_F^p$, appartient à $\mathscr{L}_F^p$. Une fonction à valeurs dans $F$, et définie presque partout dans $X$, est encore dite de puissance $p$-ième intégrable si elle est équivalente à une fonction de $\mathscr{L}_F^p$; de même, une fonction à valeurs dans $\bar{R}$, définie et finie presque partout

(*) La justification de cette terminologie sera donnée au § 4, n° 2.

dans X, est dite de puissance p-ième intégrable si elle est équivalente à une fonction de $\mathcal{L}^p$.

Les fonctions de $\mathcal{L}_F^p$ (resp. de $\mathcal{L}^p$) sont donc les fonctions de puissance p-ième intégrable qui sont définies dans X tout entier (resp. définies et finies dans X tout entier). Dans ce paragraphe et le suivant, la plupart des propositions démontrées pour les fonctions de $\mathcal{L}_F^p$ (resp. $\mathcal{L}^p$) s’étendent immédiatement aux fonctions de puissance p-ième intégrable qui ne sont pas partout définies (resp. qui ne sont pas partout définies et finies); nous laisserons le plus souvent au lecteur le soin de formuler et de démontrer ces résultats.

#### Remarque 1 {#int-iv-s3-n4-rem-1 .statement}

Comme on l’a déjà signalé (§ 2, n° 5) les fonctions de puissance p-ième intégrable, à valeurs dans F, ne forment pas un espace vectoriel en général.

#### Remarque 2 {#int-iv-s3-n4-rem-2 .statement}

En général, l’espace $\mathcal{F}_F^p$ est distinct du sous-espace $\mathcal{L}_F^p$ (§ 4, exerc. 8).

La déf. 2 donne aussitôt le critère suivant:

#### Proposition 7 {#int-iv-s3-prop-7 .statement}

Pour qu’une fonction f appartienne à $\mathcal{L}_F^p$, il faut et il suffit que, pour tout $\varepsilon > 0$, il existe une fonction g, continue et à support compact, telle que $N_p(f - g) \leq \varepsilon$.

En d’autres termes, les fonctions de $\mathcal{L}_F^p$ sont les limites de suites de fonctions continues à support compact, pour la topologie de la convergence en moyenne d’ordre p.

#### Proposition 8 {#int-iv-s3-prop-8 .statement}

Soit f une fonction numérique (finie ou non) définie presque partout; si, pour tout $\varepsilon > 0$, il existe deux fonctions g, h de puissance p-ième intégrable, telles que $g \leq f \leq h$ presque partout et que $N_p(h - g) \leq \varepsilon$, f est de puissance p-ième intégrable.

En effet, f est finie presque partout, et

$$
N_p(f - g) \leq N_p(h - g) \leq \varepsilon;
$$

la prop. 7 montre donc que f est de puissance p-ième intégrable.

Comme, par définition, $\mathcal{L}_F^p$ est un sous-espace fermé de $\mathcal{F}_F^p$, et que ce dernier est complet (n° 3, prop. 5), on a le résultat suivant (Top. gén., chap. II, 3e éd., § 3, n° 4, prop. 8):

#### Théorème 2 {#int-iv-s3-thm-2 .statement}

L’espace $\mathcal{L}_F^p$ est complet; l’espace $\mathbf{L}_F^p$ est un espace de Banach.

Dans l’espace $L_F^p$, la norme $N_p(\tilde{f})$ d’une classe se note encore $\| \tilde{f} \|_p$.

On peut préciser le th. 2 de la façon suivante :

#### Théorème 3 {#int-iv-s3-thm-3 .statement}

Soit $(f_n)$ une suite de Cauchy dans l’espace $\mathcal{L}_F^p$; il existe une suite $(f_{n_k})$ extraite de $(f_n)$, ayant les propriétés suivantes :
1° la série de terme général $N_p(f_{n_{k+1}} - f_{n_k})$ est convergente ;
2° la série de terme général $f_{n_{k+1}}(x) - f_{n_k}(x)$ est absolument convergente presque partout ;
3° si $f$ est une fonction définie dans $X$ et égale presque partout à la limite de la suite $(f_{n_k}(x))$, $f$ appartient à $\mathcal{L}_F^p$ et la suite $(f_n)$ converge en moyenne d’ordre $p$ vers $f$;
4° il existe une fonction $g \geqslant 0$ semi-continue inférieurement, telle que $N_p(g) < +\infty$ et que, pour tout $k$, on ait $|f_{n_k}(x)| \leqslant g(x)$ pour tout $x \in X$.

Comme dans la démonstration de la prop. 5 du n° 3, il suffit de définir la suite $(n_k)$ par récurrence de sorte que

$$
N_p(f_{n_{k+1}} - f_{n_k}) \leqslant 2^{-k};
$$

les parties 2° et 3° résultent alors de la prop. 6 du n° 3 et du fait que $\mathcal{L}_F^p$ est fermé dans $\mathcal{F}_F^p$. D’autre part, si $h(x)$ est somme de la série de terme général $|f_{n_{k+1}}(x) - f_{n_k}(x)|$, le th. 1 du n° 2 montre que $N_p(h) < +\infty$; par définition de $|\mu|^*$, il existe donc une fonction semi-continue inférieurement $g \geqslant h + |f_{n_1}|$ telle que

$$
N_p(g) < +\infty,
$$

ce qui achève la démonstration.

#### Corollaire 1 {#int-iv-s3-thm-3-cor-1 .statement}

Si une suite de Cauchy $(f_n)$ dans l’espace $\mathcal{L}_F^p$ est telle que la suite $(f_n(x))$ converge presque partout vers $f(x)$, $f$ est de puissance $p$-ième intégrable, et la suite $(f_n)$ converge en moyenne d’ordre $p$ vers $f$.

En effet, il existe une suite $(f_{n_k})$ extraite de $(f_n)$ telle que $(f_{n_k}(x))$ converge presque partout vers $g(x)$, où $g$ est une fonction de $\mathcal{L}_F^p$ telle que $(f_n)$ converge en moyenne d’ordre $p$ vers $g$. Les hypothèses entraînent donc que $f(x) = g(x)$ presque partout, d’où le corollaire.

#### Corollaire 2 {#int-iv-s3-thm-3-cor-2 .statement}

Soit $\mathcal{E}$ un ensemble partout dense dans $\mathcal{L}_F^p$. Pour toute fonction $f \in \mathcal{L}_F^p$, il existe une suite $(g_n)$ de fonctions de $\mathcal{E}$ possédant les propriétés suivantes :

- 1° la suite $(g_n)$ converge en moyenne d’ordre $p$ vers $f$;
  2° pour presque tout $x \in X$, la suite $(g_n(x))$ converge vers $f(x)$.
  En effet, comme l’espace $L^p_F$ est métrisable, il existe une suite de Cauchy $(f_n)$ dans $\mathcal{L}_F^p$ formée de fonctions de $\mathcal{E}$ et convergente en moyenne d’ordre $p$ vers $f$ (*Top. gén.*, chap. IX, § 2, n° 6, prop. 8); il suffit d’appliquer à cette suite le th. 3.

  Le cor. 2 s’applique en particulier au cas où on prend pour $\mathcal{E}$ l’espace $\mathcal{K}_F$ des *fonctions continues à support compact*.

  *Remarques.* — 1) Une suite de Cauchy $(f_n)$ dans $\mathcal{L}_F^p$ peut être telle que la suite $(f_n(x))$ ne soit convergente en *aucun point de* $X$ (exerc. 1).
    2) Si $f$ appartient à $\mathcal{L}_F^p$, il n’est pas toujours possible de trouver une suite $(f_n)$ de fonctions continues à support compact telle que la suite $(f_n(x))$ converge *partout* dans $X$ vers une fonction égale presque partout à $f(x)$ (§ 4, exerc. 4 c)).

### 5. Propriétés des fonctions de puissance p-ième intégrable

#### Théorème 4 {#int-iv-s3-thm-4 .statement}

*Soient F et G deux espaces de Banach, u une application linéaire continue de F dans G. Pour toute fonction f $\in \mathcal{L}_F^p$, la fonction composée u $\circ$ f appartient à $\mathcal{L}_G^p$*.
  En effet, soit $f \in \mathcal{L}_F^p$; pour tout $\varepsilon > 0$, il existe une fonction $g \in \mathcal{K}_F$ telle que $N_p(f - g) \leq \varepsilon$; comme on a
  $$
  |u \circ f - u \circ g| \leq \|u\| \cdot |f - g|,
  $$
  on a $N_p(u \circ f - u \circ g) \leq \|u\| \cdot N_p(f - g) \leq \varepsilon \|u\|$, et comme $u \circ g$ est continue et à support compact, le théorème est démontré.

#### Corollaire 1 {#int-iv-s3-thm-4-cor-1 .statement}

*Soit a' une forme linéaire continue sur F; si f $\in \mathcal{L}_F^p$, la fonction numérique $x \mapsto \langle f(x), a' \rangle$ (qu’on note $\langle f, a' \rangle$) appartient à $\mathcal{L}^p$*.

#### Corollaire 2 {#int-iv-s3-thm-4-cor-2 .statement}

*Etant donnés n points $a_k$ de F $(1 \leq k \leq n)$, et n fonctions numériques $f_k$ $(1 \leq k \leq n)$ appartenant à $\mathcal{L}^p$, la fonction $f = \sum_{k=1}^n a_k f_k$ appartient à $\mathcal{L}_F^p$*.
  Cela résulte de ce que l’application $t \mapsto at$ de $\mathbf{R}$ dans F est continue.

#### Proposition 9 {#int-iv-s3-prop-9 .statement}

Soit F un espace vectoriel de dimension n sur $\mathbf{R}$, et soit $(e_k)_{1 \leq k \leq n}$ une base de F. Pour qu’une fonction $f = \sum_{k=1}^n e_k f_k$ appartienne à $\mathcal{L}_F^p$, il faut et il suffit que chacune des fonctions numériques $f_k$ appartienne à $\mathcal{L}^p$.

Cela résulte aussitôt des cor. 1 et 2 du th. 4.

#### Proposition 10 {#int-iv-s3-prop-10 .statement}

Dans l’espace $\mathcal{L}_F^p$, le sous-espace vectoriel formé des combinaisons linéaires (finies) $\sum_k a_k f_k$, où $a_k \in F$ et où les $f_k$ sont des fonctions numériques continues à support compact, est partout dense (pour la topologie de la convergence en moyenne d’ordre p).

En effet, l’ensemble $\mathcal{K}_F$ des applications continues et à support compact de X dans F est partout dense dans $\mathcal{L}_F^p$ par définition. D’autre part, toute fonction $g \in \mathcal{K}_F$ peut être approchée uniformément par des fonctions de la forme $\sum_k a_k f_k$, où les $f_k$ sont continues et à support contenu dans un voisinage compact fixe du support de g (chap. III, § 1, n° 2, lemme 2); il en résulte (n° 3, prop. 4) que g est adhérente dans $\mathcal{L}_F^p$ à l’ensemble des $\sum_k a_k f_k$, d’où la proposition.

#### Proposition 11 {#int-iv-s3-prop-11 .statement}

Si une fonction $f$ appartient à $\mathcal{L}_F^p$, la fonction $|f|$ appartient à $\mathcal{L}^p$, et l’application $f \mapsto |f|$ de $\mathcal{L}_F^p$ dans $\mathcal{L}^p$ est uniformément continue (pour la topologie de la convergence en moyenne d’ordre p).

En effet, pour tout $\varepsilon > 0$, il existe une fonction g continue et à support compact, telle que $N_p(f - g) \leq \varepsilon$; comme
$$
||f| - |g|| \leq |f - g|,
$$
on a $N_p(|f| - |g|) \leq \varepsilon$, ce qui prouve que $|f| \in \mathcal{L}^p$. D’autre part, si $f_1, f_2$ sont deux fonctions de $\mathcal{L}_F^p$, on a $N_p(|f_1| - |f_2|) \leq N_p(f_1 - f_2)$, ce qui montre que $f \mapsto |f|$ est une application uniformément continue.

#### Proposition 12 {#int-iv-s3-prop-12 .statement}

Pour qu’une fonction numérique $f$ appartienne à $\mathcal{L}^p$, il faut et il suffit que chacune des fonctions $f^+$ et $f^-$ appartienne à $\mathcal{L}^p$.

La condition est suffisante, puisque $f = f^+ - f^-$; elle est nécessaire, puisque si $f \in \mathcal{L}^p$, on a $|f| \in \mathcal{L}^p$ (prop. 11).

#### Corollaire {#int-iv-s3-n5-cor-1 .statement}

L’enveloppe supérieure (resp. inférieure) d’une famille finie de fonctions de $\mathcal{L}^p$ appartient à $\mathcal{L}^p$.

### 6. Ensembles filtrants dans $L^p$ et suites croissantes dans $\mathcal{L}^p$

Nous avons défini (§ 2, n° 6) une relation d’ordre $\tilde{f} \leq \tilde{g}$ dans l’ensemble $\tilde{\mathcal{F}}$ des classes d’équivalence des fonctions numériques définies et finies presque partout dans $X$; muni de cette relation d’ordre et de sa structure d’espace vectoriel, $\tilde{\mathcal{F}}$ est un espace de Riesz. Le cor. de la prop. 12 du n° 5 montre que, si $\tilde{f}$ et $\tilde{g}$ sont deux éléments du sous-espace $L^p$ de $\tilde{\mathcal{F}}$, la borne supérieure $\sup (\tilde{f}, \tilde{g})$ de $\tilde{f}$ et $\tilde{g}$ dans $\tilde{\mathcal{F}}$ (qui est la classe de chacune des fonctions $\sup(f, g)$ où $f \in \tilde{f}$ et $g \in \tilde{g}$) appartient à $L^p$; cela prouve en particulier que $L^p$, muni de la relation d’ordre induite par celle de $\tilde{\mathcal{F}}$, est un espace de Riesz.

#### Proposition 13 {#int-iv-s3-prop-13 .statement}

Dans l’espace de Riesz $L^p$, muni de la topologie définie par la norme $\| \tilde{f} \|_p$, l’application $\tilde{f} \mapsto |\tilde{f}|$ est uniformément continue, et l’ensemble des éléments $\tilde{f} \geq 0$ est fermé.

La première partie de la proposition résulte aussitôt de la prop. 11 du n° 5; comme l’ensemble des $\tilde{f} \geq 0$ est aussi l’ensemble des $\tilde{f}$ tels que $|\tilde{f}| = \tilde{f}$, il est fermé, puisque $\tilde{f} \mapsto |\tilde{f}|$ est une application continue et que $L^p$ est séparé.

On voit donc que, sur $L^p$, la topologie définie par la norme $\| \tilde{f} \|_p$ est compatible avec la structure d’espace vectoriel ordonné de $L^p$ (Esp. vect. top., chap. II, 2e éd., § 2, n° 7).

#### Proposition 14 {#int-iv-s3-prop-14 .statement}

Soit $H$ une partie de l’espace de Riesz $L^p$, formée de classes $\geq 0$, et filtrante pour la relation $\leq$. Pour que $H$ ait une borne supérieure dans $L^p$, il faut et il suffit que
$$
\sup_{\tilde{f} \in H} \| \tilde{f} \|_p < +\infty.
$$
La borne supérieure de $H$ dans $L^p$ est alors la limite (dans l’espace de Banach $L^p$) du filtre des sections de $H$.

La condition est évidemment nécessaire, puisque $\tilde{f} \mapsto \| \tilde{f} \|_p$ est une fonction croissante dans l’ensemble des éléments $\geq 0$ de $L^p$. Pour voir qu’elle est suffisante, remarquons d’abord qu’elle entraîne que l’image de $H$ par l’application $\tilde{f} \mapsto \| \tilde{f} \|_p$ a une limite dans $\mathbf{R}$, en vertu du th. de la limite monotone; l’image du filtre des sections $\mathfrak{F}$ de $H$ par cette application est donc une base de filtre de Cauchy dans $\mathbf{R}$. La démonstration sera achevée si nous montrons que $\mathfrak{F}$ lui-même est une base de filtre de Cauchy sur $L^p$; en effet, $\mathfrak{F}$ convergera alors dans $L^p$, puisque $L^p$ est complet (n° 4, prop. 7), et la proposition résultera de *Esp. vect. top.*, chap. II, 2e éd., § 2, n° 7, prop. 18.

Pour voir que $\mathfrak{F}$ est une base de filtre de Cauchy, nous utiliserons le lemme suivant:

#### Lemme {#int-iv-s3-n6-lem-1 .statement}

*Si $f$ et $g$ sont deux fonctions de $\mathcal{L}^p$ telles que $0 \leq f \leq g$, on a*

$$
(\mathrm{N}_p(g - f))^p \leq (\mathrm{N}_p(g))^p - (\mathrm{N}_p(f))^p.
$$

En effet, lorsque $f$ et $g$ sont continues à support compact, la relation (9) s’écrit

$$
\int (g - f)^p d|\mu| \leq \int g^p d|\mu| - \int f^p d|\mu|
$$

et est alors conséquence de l’inégalité élémentaire $(g - f)^p \leq g^p - f^p$ (n° 1, formule (2)). Pour passer de là au cas général, il suffit de remarquer que les deux membres de (9) sont des fonctions continues dans $\mathcal{L}^p \times \mathcal{L}^p$, et que toute fonction $f \geq 0$ de $\mathcal{L}^p$ est limite (pour la convergence en moyenne d’ordre $p$) d’une suite de fonctions $\geq 0$ continues et à support compact, en raison de la continuité de l’application $g \mapsto |g|$ dans $\mathcal{L}^p$ (prop. 11).

Ce lemme étant établi, pour tout $\varepsilon > 0$, il existe par hypothèse un $\tilde{f} \in \mathrm{H}$ tel que, pour tout $\tilde{g} \geq \tilde{f}$ appartenant à $\mathrm{H}$, on ait $(\|\tilde{g}\|_p)^p - (\|\tilde{f}\|_p)^p \leq \varepsilon$; on en déduit $(\|\tilde{g} - \tilde{f}\|_p)^p \leq \varepsilon$; donc, si $\tilde{g}_1$ et $\tilde{g}_2$ sont deux éléments $\geq \tilde{f}$ dans $\mathrm{H}$, on a $\|\tilde{g}_1 - \tilde{g}_2\|_p \leq 2\varepsilon^{1/p}$, ce qui prouve que $\mathfrak{F}$ est une base de filtre de Cauchy sur $L^p$, et achève la démonstration de la prop. 14.

#### Corollaire 1 {#int-iv-s3-prop-14-cor-1 .statement}

*Si $\tilde{g}$ est la borne supérieure de $\mathrm{H}$ dans $L^p$, on a*

$$
\|\tilde{g}\|_p = \lim_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p = \sup_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p.
$$

Cela résulte de la continuité de la norme $\|\tilde{f}\|_p$ dans $L^p$, et du th. de la limite monotone.

#### Corollaire 2 {#int-iv-s3-prop-14-cor-2 .statement}

*L’espace de Riesz $L^p$ est complètement réticulé.*

En effet, tout ensemble $\mathrm{H}$ filtrant (pour la relation $\leq$) dans $L^p$ formé de classes $\geq 0$, et majoré dans $L^p$, admet une borne supérieure : car si $\tilde{h}$ est un majorant de $\mathrm{H}$ dans $L^p$, on a $\|\tilde{f}\|_p \leq \|\tilde{h}\|_p$ pour tout $\tilde{f} \in \mathrm{H}$, et la prop. 14 s’applique. Cela démontre le corollaire (chap. II, § 1, n° 3, prop. 1).

Les conclusions de la prop. 14 ne subsistent plus lorsqu’on les formule pour les fonctions de $\mathcal{L}^p$, et non plus pour leurs classes. De façon précise, si $M$ est une partie de $\mathcal{L}^p$, formée de fonctions $\geqslant 0$, filtrante pour la relation $\leqslant$, et telle que $\sup_{f \in M} N_p(f) < +\infty$, la classe de l’enveloppe supérieure $g$ de $M$ n’est pas nécessairement identique à la borne supérieure dans $L^p$ des classes des fonctions $f \in M$; en particulier, $g$ n’est pas nécessairement de puissance $p$-ième intégrable, et même lorsque $g \in \mathcal{L}^p$, $N_p(g)$ peut être distinct de $\sup_{f \in M} N_p(f)$ (cf. § 1, n° 3, Remarque 1 suivant le th. 3).

On a toutefois le théorème suivant:

#### Théorème 5 {#int-iv-s3-thm-5 .statement}

Soit $(f_n)$ une suite croissante de fonctions $\geqslant 0$ de $\mathcal{L}^p$. Pour que l’enveloppe supérieure $f$ de cette suite soit de puissance $p$-ième intégrable, il faut et il suffit que $\sup_n N_p(f_n) < +\infty$. Alors la suite $(f_n)$ converge en moyenne d’ordre $p$ vers $f$ et l’on a

$$
N_p(f) = \sup_n N_p(f_n) = \lim_{n \to \infty} N_p(f_n).
$$

La condition étant évidemment nécessaire, tout revient à prouver qu’elle est suffisante. Or, si elle est remplie, la prop. 14 montre que la suite $(\tilde{f}_n)$ est une suite de Cauchy dans $L^p$, donc la suite $(f_n)$ est une suite de Cauchy dans $\mathcal{L}^p$; comme $f_n(x)$ tend vers $f(x)$ pour tout $x \in X$, $f$ est de puissance $p$-ième intégrable et est la limite de la suite $(f_n)$ pour la topologie de la convergence en moyenne d’ordre $p$ (n° 4, cor. 1 du th. 3). Donc $N_p(f_n)$ tend vers $N_p(f)$ puisque $N_p$ est une fonction continue sur $\mathcal{L}^p$.

#### Corollaire 1 {#int-iv-s3-thm-5-cor-1 .statement}

Soit $(f_n)$ une suite décroissante de fonctions $\geqslant 0$ de $\mathcal{L}^p$; l’enveloppe inférieure $f$ de cette suite appartient à $\mathcal{L}^p$, la suite $(f_n)$ converge en moyenne d’ordre $p$ vers $f$, et l’on a

$$
N_p(f) = \lim_{n \to \infty} N_p(f_n) = \inf_n N_p(f_n).
$$

Les deux premières assertions résultent du th. 5 appliqué à la suite croissante et majorée des $g_n = f_1 - f_n$; le reste est ensuite évident.

#### Corollaire 2 {#int-iv-s3-thm-5-cor-2 .statement}

Soit $(f_n)$ une suite de fonctions de $\mathcal{L}^p$. Pour que l’enveloppe supérieure $f$ de la suite $(f_n)$ soit de puissance $p$-ième intégrable, il faut et il suffit qu’il existe une fonction $g \geq 0$ telle que $\int^* g^p d|\mu| < +\infty$ et que $f_n \leq g$ pour tout $n$.

La condition est évidemment nécessaire, en prenant $g = f^+$. Inversement, supposons-la vérifiée, et posons $g_n = \sup_{k \leq n} f_k$; la suite $(g_n)$ est croissante et formée de fonctions de puissance $p$-ième intégrable (n° 5, cor. de la prop. 12). La suite croissante des fonctions positives $h_n = g_n + g_1^-$ satisfait aux conditions du th. 5, puisque $N_p(h_n) \leq N_p(g + g_1^-) < +\infty$; l’enveloppe supérieure $\sup_n h_n$ est donc de puissance $p$-ième intégrable, et il en est de même de $f = \sup_n h_n - g_1^-$.

#### Corollaire 3 {#int-iv-s3-thm-5-cor-3 .statement}

Soient $A$ un ensemble dénombrable, $\mathcal{F}$ un filtre sur $A$ ayant une base dénombrable, $(f_\alpha)_{\alpha \in A}$ une famille de fonctions $\geq 0$ de $\mathcal{L}^p$. On suppose qu’il existe une fonction $g \geq 0$ telle que $N_p(g) < +\infty$ et $f_\alpha \leq g$ pour tout $\alpha \in A$; alors la fonction $\lim . \sup_{\mathcal{F}} f_\alpha$ est de puissance $p$-ième intégrable, et l’on a

(12) $$
\lim . \sup_{\mathcal{F}} N_p(f_\alpha) \leq N_p(\lim . \sup_{\mathcal{F}} f_\alpha).
$$

En effet, soit $(A_n)$ une base décroissante de $\mathcal{F}$, et posons $g_n = \sup_{\alpha \in A_n} f_\alpha$; comme $A_n$ est un ensemble dénombrable, il résulte du cor. 2 que $g_n$ est de puissance $p$-ième intégrable; on a d’autre part $N_p(g_n) \geq \sup_{\alpha \in A_n} N_p(f_\alpha)$. Cela étant, $\lim . \sup_{\mathcal{F}} f_\alpha$ est l’enveloppe inférieure de la suite décroissante $(g_n)$; donc $\lim . \sup_{\mathcal{F}} f_\alpha$ est de puissance $p$-ième intégrable en vertu du cor. 1, et l’on a

$$
N_p(\lim . \sup_{\mathcal{F}} f_\alpha) = N_p(\inf_n g_n) = \lim_{n \to \infty} N_p(g_n) \geq \lim_{n \to \infty} (\sup_{\alpha \in A_n} N_p(f_\alpha)) \\
= \lim . \sup_{\mathcal{F}} N_p(f_\alpha).
$$

### 7. Le théorème de Lebesgue

#### Théorème 6 (Lebesgue) {#int-iv-s3-thm-6 .statement}

Soient $F$ un espace de Banach, $(f_n)$ une suite de fonctions de $\mathcal{L}_F^p$ telles que : 1° la suite $(f_n(x))$ converge presque partout vers une limite $f(x) \in F$; 2° il existe une fonction numérique $g \geq 0$ tel que $\int^* g^p d|\mu| < +\infty$ et $|f_n(x)| \leq g(x)$ presque partout dans X, pour tout entier n. Alors la fonction f (définie presque partout) est de puissance p-ième intégrable, et la suite (f_n) converge en moyenne d’ordre p vers f.

Considérons la suite «double» de fonctions numériques $g_{mn} = |f_m - f_n|$, qui appartiennent à $\mathcal{L}^p$ (n° 5, prop. 11); par hypothèse, on a $\lim_{m \to \infty, n \to \infty} g_{mn}(x) = 0$ presque partout, et d’autre part $|g_{mn}(x)| \leq 2g(x)$ presque partout; par application à cette suite double du cor. 3 du th. 5 du n° 6, on a

$$
\lim_{m \to \infty, n \to \infty} \sup N_p(f_m - f_n) \leq N_p(0) = 0
$$

et comme $N_p(f_m - f_n) \geq 0$, cela entraîne

$$
\lim_{m \to \infty, n \to \infty} N_p(f_m - f_n) = 0;
$$

autrement dit, la suite $(f_n)$ est une suite de Cauchy dans $\mathcal{L}_F^p$. Le théorème résulte donc du cor. 1 du th. 3 du n° 4.

#### Corollaire {#int-iv-s3-n7-cor-1 .statement}

Soit A un ensemble d’indices, filtré par un filtre $\mathfrak{F}$ ayant une base dénombrable. Si $(f_\alpha)_{\alpha \in A}$ est une famille de fonctions de $\mathcal{L}_F^p$ qui, suivant le filtre $\mathfrak{F}$, convergent simplement presque partout vers une fonction f, et si en outre il existe une fonction numérique $g \geq 0$ telle que $\int^* g^p d|\mu| < +\infty$ et $|f_\alpha(x)| \leq g(x)$ presque partout dans X pour tout $\alpha \in A$, alors la fonction f est de puissance p-ième intégrable, et $f_\alpha$ tend en moyenne d’ordre p vers f suivant le filtre $\mathfrak{F}$.

En effet, soit $(A_n)$ une base dénombrable décroissante de $\mathfrak{F}$, et soit $\alpha_n$ un élément quelconque de $A_n$; la suite $(f_{\alpha_n})$ converge simplement vers f presque partout dans X, donc le th. 6 montre que f est de puissance p-ième intégrable et que $\lim_{n \to \infty} N_p(f - f_{\alpha_n}) = 0$.

Comme $\mathfrak{F}$ est le filtre intersection des filtres élémentaires associés à toutes les suites $(\alpha_n)$ (Top. gén., chap. I, 3e éd., § 6, n° 8, prop. 11), $\lim_{\mathfrak{F}} N_p(f - f_\alpha)$ existe et est égale à la limite commune 0 de toutes les suites $(N_p(f - f_{\alpha_n}))$.

#### Remarque 1 {#int-iv-s3-n7-rem-1 .statement}

Le th. 6 ne subsiste pas si on remplace l’hypothèse $|f_n| \leq g$ (avec $N_p(g) < +\infty$) par l’hypothèse plus faible $\sup_n N_p(f_n) < +\infty$. Supposons par exemple que $\mu$ soit la mesure de Lebesgue sur $\mathbf{R}$; définissons les fonctions continues $f_n$ de la manière suivante: $f_n(x) = 0$ pour $x \leq 0$ et $x \geq \frac{2}{n}$, $f_n\left(\frac{1}{n}\right) = n$, f_n étant linéaire dans les intervalles $\left(0, \frac{1}{n}\right)$ et $\left(\frac{1}{n}, \frac{2}{n}\right)$. On a
$$
\lim_{n \to \infty} f_n(x) = 0 \text{ pour tout } x \in \mathbf{R}, \text{ mais } N_1(f_n) = 1 \text{ pour tout } n
$$
(cf. § 5, exerc. 12).

#### Remarque 2 {#int-iv-s3-n7-rem-2 .statement}

Le cor. du th. 6 ne subsiste pas si on ne suppose plus que le filtre $\mathcal{F}$ ait une base dénombrable (cf. § 1, no 3, Remarque 1 suivant le th. 3).

### 8. Relations entre les espaces $\mathcal{L}_F^p (1 \leq p < + \infty)$.

Pour tout nombre $\alpha > 0$, l’application $z \mapsto |z|^{\alpha - 1} . z$ est définie et continue dans le complémentaire de 0 dans $F$; en outre, comme $||z|^{\alpha - 1} . z| = |z|^{\alpha}$, cette fonction tend vers 0 avec $z$, et on peut donc la prolonger par continuité au point 0 en lui donnant la valeur 0 en ce point, même si $\alpha < 1$.

#### Théorème 7 {#int-iv-s3-thm-7 .statement}

Soient $p$ et $q$ deux nombres réels tels que $1 \leq p < + \infty, 1 \leq q < + \infty$. Si une fonction $f$ appartient à $\mathcal{L}_F^p$, la fonction $|f|^{(p/q) - 1} . f$ appartient à $\mathcal{L}_F^q$, et réciproquement.

Par hypothèse, il existe une suite $(f_n)$ de fonctions continues à support compact telles que $\sum_{n=1}^{\infty} N_p(f_n) < + \infty$ et $f(x) = \sum_{n=1}^{\infty} f_n(x)$ presque partout (no 4, th. 3). Posons
$$
g_n = |f_1 + f_2 + \cdots + f_n|^{(p/q) - 1} . (f_1 + f_2 + \cdots + f_n);
$$
la fonction $g_n$ est continue et à support compact; d’autre part, on a $|g_n|^q = |f_1 + f_2 + \cdots + f_n|^p \leq \left( \sum_{n=1}^{\infty} |f_n| \right)^p = h^q$, où la fonction numérique $h \geq 0$ (finie ou non) vérifie l’inégalité
$$
(N_q(h))^q = \left( N_p \left( \sum_{n=1}^{\infty} |f_n| \right) \right)^p \leq \left( \sum_{n=1}^{\infty} N_p(f_n) \right)^p < + \infty
$$
en vertu du th. de convexité dénombrable. En outre, $g_n(x)$ tend presque partout vers $g(x) = |f(x)|^{(p/q) - 1} . f(x)$, donc le th. de Lebesgue montre que $g \in \mathcal{L}_F^q$. La réciproque est immédiate, puisque $f = |g|^{(q/p) - 1} . g$.

On peut montrer que l’application $f \mapsto |f|^{p/q - 1} . f$ est un homéomorphisme de $\mathcal{L}_F^p$ sur $\mathcal{L}_F^q$ (§ 6, exerc. 10).

#### Corollaire 1 {#int-iv-s3-thm-7-cor-1 .statement}

Pour qu’une fonction $f$ appartienne à $\mathcal{L}_F^p$, il faut et il suffit que la fonction $|f|^{p-1} \cdot f$ appartienne à $\mathcal{L}_F^1$.

#### Corollaire 2 {#int-iv-s3-thm-7-cor-2 .statement}

Pour qu’une fonction numérique positive $f$ appartienne à $\mathcal{L}^p$, il faut et il suffit que $f^p$ appartienne à $\mathcal{L}^1$.

On notera que si $f$ est une fonction numérique de signe quelconque telle que $|f|^p$ appartienne à $\mathcal{L}^1$, $f$ n’appartient pas nécessairement à $\mathcal{L}^p$ (cf. § 4, exerc. 8).

## EXERCICES {#int-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
