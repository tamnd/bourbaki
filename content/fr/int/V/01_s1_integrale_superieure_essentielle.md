---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 1
section_title: Intégrale supérieure essentielle
lang: fr
source: int-v-fr
pdf_pages: 0007-0017, 0108-0109
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’intégrale supérieure essentielle
      page: 0
      pdf_page: 7
    - "no": 2
      title: Fonctions et mesures modérées
      page: 0
      pdf_page: 9
    - "no": 3
      title: Fonctions essentiellement intégrables
      page: 0
      pdf_page: 12
    - "no": 4
      title: Une propriété spéciale à l’intégrale supérieure essentielle
      page: 0
      pdf_page: 16
statements: 25
exercises: 6
content_sha256: e66013f1e32478d647b682eb6d174db1b7187ad1d06d022eb0b6fe6869abede7
---

## § 1. Intégrale supérieure essentielle

### 1. Définition de l’intégrale supérieure essentielle

#### Définition 1 {#int-v-s1-def-1 .statement}

Pour toute fonction $f \in \mathcal{F}_+(T)$, on appelle intégrale supérieure essentielle de $f$ par rapport à $\mu$, et on note $\mu^*(f)$, la borne supérieure, finie ou non, de l’ensemble des nombres $\mu^*(f\varphi_K)$ où $K$ parcourt l’ensemble des parties compactes de $T$. Pour toute partie $A$ de $T$, on pose $\mu^*(A) = \mu^*(\varphi_A)$.

On utilise aussi les notations $\int^* f d\mu$, $\int^* f(t) d\mu(t)$, $\int^* f\mu$.
Comme $f\varphi_K \leq f$ pour toute partie compacte $K$ de $T$, on a
(1)
$$
\int^* f d\mu \leq \int^* f d\mu.
$$

On peut avoir $\mu^*(f) \neq \mu^*(f)$; en effet, la condition $\mu^*(f) = 0$ signifie que $f$ est négligeable tandis que la condition $\mu^*(f) = 0$ signifie que $f$ est localement négligeable (chap. IV, § 5, n° 2, prop. 5), et il peut exister des ensembles localement négligeables et non négligeables (chap. IV, § 1, exerc. 5).

L’application $\mu^*$ de $\mathcal{F}_+(T)$ dans $\bar{\mathbf{R}}$ coïncide avec $\mu$ sur $\mathcal{K}_+(T)$.
Il en résulte que deux mesures $\mu_1$ et $\mu_2$ telles que $\mu_1^* = \mu_2^*$ sont égales.

#### Proposition 1 {#int-v-s1-prop-1 .statement}

a) Si $f$ et $g$ sont deux fonctions numériques $\geq 0$, égales localement presque partout, on a $\mu^*(f) = \mu^*(g)$.
b) Si $f$ et $g$ sont deux fonctions numériques $\geq 0$, telles que $f \leq g$, on a $\mu^*(f) \leq \mu^*(g)$.
c) Si $f$ est une fonction numérique $\geq 0$, et $\alpha$ un nombre $\geq 0$, on a $\mu^*(\alpha f) = \alpha \mu^*(f)$.
d) Si $f$ et $g$ sont deux fonctions numériques $\geq 0$, on a $\mu^*(f + g) \leq \mu^*(f) + \mu^*(g)$.
e) Si $(f_n)_{n \in \mathbf{N}}$ est une suite croissante de fonctions numériques $\geq 0$, et si $f = \lim_{n \to \infty} f_n$, on a $\mu^*(f) = \lim_{n \to \infty} \mu^*(f_n)$.

Les propriétés a), b), c), d) se déduisent aussitôt des propriétés correspondantes de l’intégrale supérieure: a) de la proposition 6 du chap. IV, § 2, n° 3 et de la proposition 5 du chap. IV, § 5, n° 2; b), c), d) des propositions 10, 11, 12 du chap. IV, § 1, n° 3. Pour établir e), désignons par $\mathfrak{K}$ l’ensemble des parties compactes de T ; nous avons, d’après le théorème 3 du chap. IV, § 1, n° 3:

$$
\lim_{n \to \infty} \mu^*(f_n) = \sup_{n \in \mathbf{N}} \sup_{K \in \mathfrak{K}} \mu^*(f_n \varphi_K) = \sup_{K \in \mathfrak{K}} \sup_{n \in \mathbf{N}} \mu^*(f_n \varphi_K)
$$
$$
= \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K) = \mu^*(f).
$$

On a l’égalité dans la relation d) si $f$ et $g$ sont mesurables, d’après le cor. 4 du th. 5, chap. IV, § 5, n° 5. Plus généralement, on a le résultat suivant:

#### Proposition 2 {#int-v-s1-prop-2 .statement}

Soient $f, g, h$ trois éléments de $\mathcal{F}_+$; si $g$ et $h$ sont mesurables, on a:

(2)
$$
\int^* f(g + h)\, d\mu = \int^* fg\, d\mu + \int^* fh\, d\mu.
$$

On se ramène aussitôt à la démonstration de la formule analogue pour l’intégrale supérieure. Comme on a
$$
f(g + h) = fg + fh
$$
(avec la convention $0 \cdot (+\infty) = 0$), on a
$$
\int^* f(g + h)\, d\mu \leq \int^* fg\, d\mu + \int^* fh\, d\mu;
$$
il reste à établir l’inégalité inverse. Soit $u$ une fonction semi-continue inférieurement telle qu’on ait $u \geq f(g + h)$. Posons $v = \frac{u}{g + h}$ dans l’ensemble où $g + h > 0$, $v = +\infty$ dans l’ensemble où $g + h = 0$; on a $v \geq f$ et $u \geq v(g + h)$, d’où
$$
\int^* v(g + h)\, d\mu \leq \int^* u\, d\mu
$$
et par conséquent, $v$ étant mesurable (chap. IV, 2e éd., § 5, n° 6, cor. 4 du th. 5):
$$
\int^* fg\, d\mu + \int^* fh\, d\mu \leq \int^* vg\, d\mu + \int^* vh\, d\mu
$$
$$
= \int^* v(g + h)\, d\mu \leq \int^* u\, d\mu,
$$

ce qui entraîne l’inégalité cherchée, $\varepsilon$ étant arbitraire.

#### Corollaire {#int-v-s1-n1-cor-1 .statement}

Soient $f$ une fonction $\geqslant 0$, $(g_n)$ une suite de fonctions mesurables $\geqslant 0$; on a $\int^* f(\sum g_n) d\mu = \sum (\int^* fg_n d\mu)$.

Dans le cas d’une suite finie, c’est une conséquence immédiate de la prop. 2. Le cas d’une suite infinie s’en déduit au moyen de la prop. 1, e).

#### Proposition 3 {#int-v-s1-prop-3 .statement}

Pour tout nombre fini $\alpha \geqslant 0$ et tout couple de mesures $\mu, v$ sur $T$, on a
$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + v)^* = \mu^* + v^*.
$$
En outre, la relation $\mu \leqslant v$ entraîne $\mu^* \leqslant v^*$.

La démonstration est immédiate à partir de l’énoncé analogue du chapitre IV (§ 1, n° 3, prop. 15).

#### Proposition 4 {#int-v-s1-prop-4 .statement}

Pour toute fonction numérique $f \geqslant 0$, semi-continue inférieurement dans $T$, on a $\mu^*(f) = \mu^*(f)$.

En effet, soit $g$ une fonction de $\mathcal{K}_+(T)$ telle que $g \leqslant f$. Si $K$ est le support (compact) de $g$, on a $\mu(g) \leqslant \mu^*(f_{\varphi_K}) \leqslant \mu^*(f)$. Il en résulte, d’après la définition de l’intégrale supérieure, que $\mu^*(f) \leqslant \mu^*(f)$, donc $\mu^*(f) = \mu^*(f)$ (formule (1)).

### 2. Fonctions et mesures modérées

#### Proposition 5 {#int-v-s1-prop-5 .statement}

Soit $A$ une partie de $T$; les propriétés suivantes sont équivalentes:
a) L’ensemble $A$ est contenu dans la réunion d’une suite d’ouverts $\mu$-intégrables.
b) L’ensemble $A$ est contenu dans la réunion d’une suite d’ensembles $\mu$-intégrables.
c) L’ensemble $A$ est contenu dans la réunion d’une suite de compacts et d’un ensemble $\mu$-négligeable.

Il est clair que chacune des propriétés a) et c) entraîne b). Inversement, b) entraîne a), car tout ensemble de mesure extérieure finie est contenu dans un ouvert intégrable (chap. IV, § 1, n° 4, prop. 19), et b) entraîne c), car tout ensemble intégrable est réunion d’une suite de compacts et d’un ensemble négligeable (chap. IV, § 4, n° 6, cor. 2 du th. 4).

#### Définition 2 {#int-v-s1-def-2 .statement}

Une partie de $T$ est dite $\mu$-modérée si elle satisfait aux conditions équivalentes de la proposition 5. Une fonction définie sur T, à valeurs dans un espace vectoriel ou dans $\bar{\mathbf{R}}$, est dite $\mu$-modérée si elle est nulle dans le complémentaire d’une partie $\mu$-modérée de T. On dit que la mesure $\mu$ est modérée si T est un ensemble $\mu$-modéré.

Si $\mu$ est une mesure modérée, toute fonction sur T est $\mu$-modérée et toute partie de T est $\mu$-modérée.

#### Remarque 1 {#int-v-s1-n2-rem-1 .statement}

Si $\theta$ est une mesure complexe sur T, on dira qu’une fonction $f$ est $\theta$-modérée (resp. que $\theta$ est modérée) si $f$ est $|\theta|$-modérée (resp. si $|\theta|$ est modérée).

#### Remarque 2 {#int-v-s1-n2-rem-2 .statement}

Toute mesure bornée est modérée; si T est une réunion dénombrable de compacts, toute mesure sur T est modérée.

#### Remarque 3 {#int-v-s1-n2-rem-3 .statement}

Soit $(f_n)$ une suite de fonctions $\mu$-modérées à valeurs dans $\bar{\mathbf{R}}$. Pour chaque $n$, soit $U_n$ un ouvert, réunion dénombrable d’ouverts de mesure extérieure finie, tel que $f_n$ soit nulle hors de $U_n$. La fonction $s = \sum_{n \in \mathbf{N}} |f_n|$ est alors nulle hors de $\bigcup_{n \in \mathbf{N}} U_n$; elle est donc $\mu$-modérée, et il en est de même de toutes les fonctions majorées par $s$. Cela s’applique en particulier aux fonctions $\liminf_{n \to \infty} f_n$, $\limsup_{n \to \infty} f_n$ et $\sum_{n \in \mathbf{N}} f_n$ (si cette somme est définie).

#### Remarque 4 {#int-v-s1-n2-rem-4 .statement}

Une fonction égale presque partout à une fonction modérée est modérée.

#### Proposition 6 {#int-v-s1-prop-6 .statement}

Soit $f$ une fonction numérique positive définie dans T, $\mu$-mesurable et $\mu$-modérée. Il existe alors une suite $(h_n)_{n \in \mathbf{N}}$ d’éléments de $\mathcal{F}_+(T)$, dont la somme est égale à $f$, possédant les propriétés suivantes:

1) La fonction $h_0$ est $\mu$-négligeable.

2) Pour tout $n \geqslant 1$, il existe un compact $K_n$ tel que $h_n$ soit nulle hors de $K_n$, et que la restriction de $h_n$ à $K_n$ soit finie et continue.

Supposons que $f$ soit somme d’une suite $(f_n)$ de fonctions mesurables positives, dont chacune possède la propriété de l’énoncé; il est clair que $f$ la possède alors aussi. Posons

$$
f_n = \inf(f, n+1) - \inf(f, n)
$$

pour tout $n \in \mathbf{N}$; $f$ étant égale à la somme de la suite $(f_n)$, il nous suffira donc d’établir la proposition en supposant $f$ modérée et bornée. Désignons alors par A l’ensemble des $t \in T$ tels que $f(t) > 0$; A est mesurable et modéré, et il existe donc une suite $(A_n)$ d’ensembles intégrables, deux à deux disjoints, telle que

Soit $\mathfrak{R}$ l’ensemble des compacts K de T tels que $f|K$ soit continue ; $\mathfrak{R}$ étant $\mu$-dense (chap. IV, 2e éd., § 5, n° 10, prop. 15), L est réunion d’un ensemble négligeable N, et d’une suite $(K_n)_{n \geq 1}$ d’éléments de $\mathfrak{R}$ deux à deux disjoints (chap. IV, 2e éd., § 5, n° 8, déf. 6). Les fonctions $h_0 = f\varphi_N, h_n = f\varphi_{K_n}$ pour $n \geq 1$, satisfont alors aux conditions de l’énoncé.

La proposition suivante permet de ramener l’étude de l’intégrale supérieure à celle de l’intégrale supérieure essentielle.

#### Proposition 7 {#int-v-s1-prop-7 .statement}

Soit $f$ un élément de $\mathcal{F}_+(T)$.

1) *Si la fonction $f$ n’est pas $\mu$-modérée*, $\mu^*(f) = +\infty$.
2) *Si la fonction $f$ est $\mu$-modérée*, $\mu^*(f) = \mu^*(f)$.
3) *Si l’on a* $\mu^*(f) < +\infty$, *il existe une partie $\mu$-modérée* A, *réunion d’une suite de compacts de* T, *telle que* $f = f\varphi_A$ *localement presque partout*.

La première assertion résulte aussitôt du lemme 1 du chap. IV, 2e éd., § 5, n° 6. Pour établir la seconde, désignons par A une partie modérée, telle que $f$ soit nulle hors de A ; A est réunion d’un ensemble négligeable $A_0$ et d’une suite $(A_n)_{n \geq 1}$ d’ensembles compacts, que l’on peut supposer croissante. La fonction $f$ est alors presque partout égale à l’enveloppe supérieure des fonctions $f\varphi_{A_n}$ ($n \geq 1$), et l’on a donc (chap. IV, § 1, n° 3, th. 3 et § 2, n° 3, prop. 6)
$$
\mu^*(f) = \lim_{n \to \infty} \mu^*(f\varphi_{A_n}) \leq \mu^*(f);
$$
d’où l’égalité $\mu^*(f) = \mu^*(f)$ en vertu de la formule (1). Enfin, supposons que $\mu^*(f) < +\infty$ ; il existe une suite croissante $(A_n)$ de compacts telle que
$$
\mu^*(f) = \sup_n \mu^*(f\varphi_{A_n}).
$$
Posons $A = \bigcup_n A_n$ ; le second membre est égal à $\mu^*(f\varphi_A)$ (chap. IV, § 1, n° 3, th. 3), ou encore à $\mu^*(f\varphi_A)$ (d’après la prop. 1, ou d’après 2) ci dessus). Comme on a $\mu^*(f) = \mu^*(f\varphi_A) + \mu^*(f\varphi_{\mathbf{C}A})$ (prop. 2), on a $\mu^*(f\varphi_{\mathbf{C}A}) = 0$, et 3) en découle.

#### Corollaire 1 {#int-v-s1-prop-7-cor-1 .statement}

Pour que f soit négligeable, il faut et il suffit qu’elle soit localement négligeable et modérée.

#### Corollaire 2 {#int-v-s1-prop-7-cor-2 .statement}

Si $\mu$ est une mesure modérée (en particulier si $\mu$ est bornée, ou si T est dénombrable à l’infini), on a $\mu^* = \mu^*$.

#### Proposition 8 {#int-v-s1-prop-8 .statement}

a) Soit H un ensemble de fonctions $\geq 0$, semi-continues inférieurement, filtrant pour la relation $\leq$; on a alors:

$$
\mu^*(\sup_{h \in H} h) = \sup_{h \in H} \mu^*(h).
$$

b) Soit H un ensemble de fonctions $\geq 0$, semi-continues supérieurement, filtrant pour la relation $\geq$; s’il existe dans H une fonction $h_0$ telle que $\mu^*(h_0) < \infty$, on a:

$$
\mu^*(\inf_{h \in H} h) = \inf_{h \in H} \mu^*(h).
$$

L’assertion a), compte tenu de la prop. 4, est une répétition du théorème 1 du chap. IV, § 1, n° 1. Pour établir b), posons $\eta = \inf_{h \in H} h$, et soit $a$ un nombre $> 0$. Il existe un compact K tel que l’on ait (chap. IV, 2e éd., § 4, n° 4, cor. 1 de la prop. 5):

$$
\mu^*(h_0) - a \leq \mu^*(h_0 \varphi_K) = \mu(h_0 \varphi_K) \leq \mu^*(h_0).
$$

Les fonctions $h \varphi_K$, où $h$ parcourt H, forment un ensemble de fonctions semi-continues supérieurement, filtrant pour la relation $\geq$, et qui contient une fonction intégrable. On a donc (chap. IV, 2e éd., § 4, n° 4, cor. 2 de la prop. 5):

$$
\mu^*(\eta \varphi_K) = \inf_{h \in H} \mu^*(h \varphi_K).
$$

Mais on a (chap. IV, 2e éd., § 4, n° 4, cor. 1 de la prop. 5) $\mu^*(h_0 \varphi_{C_K}) \leq a$, d’où $\mu^*(h \varphi_{C_K}) \leq a$ pour toute fonction $h \in H$ majorée par $h_0$. On a donc finalement:

$$
\mu^*(\eta) \geq \mu^*(\eta \varphi_K) = \inf_{h \in H} \mu^*(h \varphi_K) \geq \inf_{h \in H} \mu^*(h) - a.
$$

L’inégalité $\mu^*(\eta) \leq \inf_{h \in H} \mu^*(h)$ étant évidente, et $a$ étant arbitraire, la proposition est établie.

### 3. Fonctions essentiellement intégrables

Soit F un espace de Banach réel; rappelons que les éléments des espaces $\mathcal{F}_F^p$ (chap. IV, § 3, n° 3) et $\mathcal{L}_F^p$ (chap. IV, § 3, n° 4, déf. 2) sont des fonctions $\mu$-modérées (chap. IV, 2e éd., § 5, n° 6, lemme 1); $\mathcal{N}_F$ désignant toujours l’espace des applications négligeables de T dans F, nous introduirons l’espace $\mathcal{N}_F^\infty$ des applications localement négligeables de T dans F.

#### Lemme 1 {#int-v-s1-lem-1 .statement}

Soient g et $g'$ deux applications $\mu$-modérées à valeurs dans F; si g et $g'$ sont égales localement presque partout à une même fonction f, on a $g = g'$ presque partout.

En effet, soit D l’ensemble des $t \in T$ tels que $g(t) \neq g'(t)$; D est localement négligeable et modéré, donc négligeable (cor. 1 de la prop. 7).

Nous désignerons par $\bar{\mathcal{F}}_F^p(T, \mu)$ (ou simplement $\bar{\mathcal{F}}_F^p(\mu)$, $\bar{\mathcal{F}}_F^p$, si aucune confusion n’en résulte) l’ensemble des applications f de T dans F, telles qu’il existe une fonction $g \in \mathcal{F}_F^p$ égale à f localement presque partout. Le nombre $N_p(g)$ ne dépendant que de f d’après le lemme 1, nous poserons $\overline{N}_p(f) = N_p(g)$. La fonction $\overline{N}_p$ est évidemment une semi-norme sur $\bar{\mathcal{F}}_F^p$, et nous supposerons toujours que $\bar{\mathcal{F}}_F^p$ est muni de la topologie définie par $\overline{N}_p$. L’adhérence de 0 pour cette topologie est l’espace $\mathcal{N}_F^\infty$; les relations $\bar{\mathcal{F}}_F^p = \mathcal{F}_F^p + \mathcal{N}_F^\infty$, $\mathcal{N}_F^\infty \cap \mathcal{F}_F^p = \mathcal{N}_F$ (lemme 1), montrent que l’espace normé $\bar{\mathcal{F}}_F^p / \mathcal{N}_F^\infty$ s’identifie canoniquement à $\mathcal{F}_F^p / \mathcal{N}_F$, qui est complet (chap. IV, § 3, n° 3, prop. 5); $\bar{\mathcal{F}}_F^p$ est donc lui-même complet.

Nous désignerons de même par $\bar{\mathcal{L}}_F^p(T, \mu)$ (ou $\bar{\mathcal{L}}_F^p(\mu)$, ou $\bar{\mathcal{L}}_F^p$) le sous-espace $\mathcal{L}_F^p + \mathcal{N}_F^\infty$ de $\bar{\mathcal{F}}_F^p$: on peut aussi caractériser $\bar{\mathcal{L}}_F^p$ comme le sous-espace de $\bar{\mathcal{F}}_F^p$ constitué par les applications mesurables (chap. IV, § 5, n° 6, th. 5). L’espace normé $\bar{\mathcal{L}}_F^p / \mathcal{N}_F^\infty$ s’identifie canoniquement à $L_F^p$; $\bar{\mathcal{L}}_F^p$ est donc complet. Ses éléments sont appelés fonctions de puissance p-ième essentiellement intégrable, cette terminologie étant justifiée par la proposition suivante:

#### Proposition 9 {#int-v-s1-prop-9 .statement}

Pour qu’une application f de T dans F appartienne à $\bar{\mathcal{F}}_F^p$ (resp. à $\bar{\mathcal{L}}_F^p$) il faut et il suffit que l’on ait (resp. que f soit mesurable et que l’on ait)

$$
\mu^*(|f|^p) < +\infty.
$$

On a alors $\overline{N}_p(f) = \mu^*(|f|^p))^{1/p}$.

On peut évidemment se limiter à l’assertion concernant $\bar{\mathcal{F}}_F^p$. Si f appartient à $\bar{\mathcal{F}}_F^p$, soit g une fonction appartenant à $\mathcal{F}_F^p$, égale à f localement presque partout; on a alors $|f|^p = |g|^p$ localement presque partout, donc $\mu^*(|f|^p) = \mu^*(|g|^p) = \mu^*(|g|^p) < +\infty$ (prop. 1, a) et prop. 7), et d’autre part, par définition de $\overline{N}_p$,

$$
\overline{N}_p(f) = N_p(g) = (\mu^*(|g|^p))^{1/p}.
$$

Inversement, supposons que l’on ait $\mu^*(|f|^p) < +\infty$; il existe alors un ensemble modéré $A$ tel que $f$ soit nulle localement presque partout dans $T - A$ (prop. 7). La fonction $f \varphi_A$, égale localement presque partout à $f$, est telle que $N_p(f \varphi_A) = \overline{N}_p(f) < +\infty$; elle appartient donc à $\mathcal{F}_F^p$, et on a $f \in \mathcal{F}_F^p$.

#### Corollaire {#int-v-s1-n3-cor-1 .statement}

Pour que $f$ appartienne à $\mathcal{L}_F^p$, il faut et il suffit que $f$ appartienne à $\overline{\mathcal{L}}_F^p$ et soit modérée.

#### Définition 3 {#int-v-s1-def-3 .statement}

Les éléments de $\overline{\mathcal{L}}_F^1$ sont appelés fonctions essentiellement $\mu$-intégrables à valeurs dans $F$. En composant l’application $\tilde{f} \mapsto \mu(\tilde{f})$ de $L_F^1$ dans $F$ avec l’application canonique de $\overline{\mathcal{L}}_F^1$ sur $L_F^1$, on obtient une application linéaire continue de $\overline{\mathcal{L}}_F^1$ dans $F$, qui prolonge l’application $f \mapsto \int f \, d\mu$ de $\mathcal{L}_F^1$ dans $F$. On note encore $\int f \, d\mu$ ou $\mu(f)$ la valeur de cette application pour $f \in \overline{\mathcal{L}}_F^1$, et on dit que cet élément est l’intégrale de $f$ par rapport à $\mu$.

Deux fonctions essentiellement intégrables et égales localement presque partout ont même intégrale. Pour toute fonction $f \geqslant 0$, finie et essentiellement intégrable, on a $\int^* f \, d\mu = \int f \, d\mu$. Si $A$ est un ensemble dont la fonction caractéristique est essentiellement intégrable, on dit que $A$ est un ensemble essentiellement $\mu$-intégrable; $\int \varphi_A \, d\mu$ se note aussi $\mu(A)$ et s’appelle encore la mesure de $A$.

Si une fonction $f$, à valeurs dans $F$, est définie localement presque partout dans $T$, on dit encore que $f$ est essentiellement intégrable si elle est égale, localement presque partout, à une fonction $f_1$ partout définie et intégrable; on pose alors

$$
\int f \, d\mu = \int f_1 \, d\mu,
$$

et cette définition ne dépend pas de la fonction intégrable $f_1$ partout définie et localement presque partout égale à $f$ (lemme 1). On définit de même la notion de fonction essentiellement intégrable pour les fonctions à valeurs dans $\mathbf{R}$, définies et finies localement presque partout.

$$
|\int f\,d\mu| \leq \int |f|\,d\mu
$$

valable pour toute fonction essentiellement intégrable $f$ à valeurs dans un espace de Banach.

#### Proposition 10 {#int-v-s1-prop-10 .statement}

*Soit $\mathfrak{R}$ un ensemble $\mu$-dense de parties compactes de $T$.*

a) *Si $f$ est une fonction numérique $\geq 0$, on a*:

$$
\mu^*(f) = \sup_{K \in \mathfrak{R}} \mu^*(f \varphi_K).
$$

b) *Si $f$ est une fonction à valeurs dans un espace de Banach $F$, essentiellement intégrable, on a*:

$$
\int f\,d\mu = \lim_{\mathfrak{R}} \int f \varphi_K\,d\mu
$$

*la limite étant prise suivant l’ensemble filtrant (pour $\subset$) $\mathfrak{R}$.*

Pour établir a), il suffit de montrer que pour toute partie compacte $L$ de $T$, on a $\int^* f \varphi_L\,d\mu = \sup_K \int^* f \varphi_K\,d\mu$, où $K$ parcourt l’ensemble des parties de $L$ appartenant à $\mathfrak{R}$. Comme $L$ est réunion d’un ensemble négligeable et d’une suite croissante ($K_n$) d’éléments de $\mathfrak{R}$ (chap. IV, 2e éd., § 5, n° 8, prop. 12), cela résulte du théorème de passage à la limite dans les intégrales supérieures (chap. IV, § 1, n° 3, th. 3).

Supposons maintenant que $f$ appartienne à $\overline{\mathcal{L}}_F^1$; soit $\varepsilon$ un nombre $> 0$, et soit $K$ un élément de $\mathfrak{R}$ tel que

$$
\int |f|\varphi_K\,d\mu \geq \int |f|\,d\mu - \varepsilon
$$

(il en existe d’après a)). On a alors pour tout compact $H$ contenant $K$:

$$
\left| \int f\,d\mu - \int f \varphi_H\,d\mu \right| \leq \int |f|\varphi_{\mathbf{C}_H}\,d\mu \leq \int |f|\varphi_{\mathbf{C}_K}\,d\mu \leq \varepsilon.
$$

*Extension aux espaces de Banach et aux mesures complexes.* Soit $F$ un espace de Banach complexe; par abus de notation, nous désignerons encore par $F$ l’espace de Banach réel sous-jacent à $F$. L’espace de Banach $\overline{\mathcal{L}}_F^p(T, \mu)$ peut alors être muni d’une structure d’espace de Banach complexe naturelle, et il conviendra de préciser si l’on utilise la structure réelle ou complexe de cet espace. Dans ce chapitre, et sauf mention expresse du contraire, il s’agira toujours de la structure réelle.

Soit $\theta$ une mesure complexe ; on posera $\mathcal{L}_F^p(T, \theta) = \mathcal{L}_F^p(T, |\theta|)$; si F est un espace de Banach complexe, il y a lieu de faire les mêmes remarques que ci-dessus. En particulier, une fonction $f$ à valeurs dans F sera dite essentiellement intégrable pour $\theta$ si elle est essentiellement intégrable pour $|\theta|$. L’assertion b) de la prop. 10 s’étend aussitôt aux mesures complexes.

### 4. Une propriété spéciale à l’intégrale supérieure essentielle

Le résultat suivant sera fréquemment utilisé dans la suite. On ne peut pas remplacer dans l’énoncé les intégrales supérieures essentielles par des intégrales supérieures ordinaires (voir l’exerc. 4).

#### Proposition 11 {#int-v-s1-prop-11 .statement}

Soit $(\lambda_\alpha)_{\alpha \in A}$ une famille de mesures positives sur T, filtrante pour la relation $\leq$ et admettant dans $\mathcal{M}(T)$ une borne supérieure $\lambda$. On a alors pour toute fonction numérique $f \geq 0$

$$
\lambda^\bullet(f) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Lorsque $f$ appartient à $\mathcal{K}(T)$, cette relation se réduit à la définition de la borne supérieure d’un ensemble filtrant dans $\mathcal{M}(T)$ (chap. II, § 2, n° 2, lemme 1). Supposons ensuite que $f$ soit majorée par une fonction $g \in \mathcal{K}_+$ (autrement dit, que $f$ soit bornée et nulle hors d’un compact K); soit $\alpha$ un indice tel que l’on ait $\lambda_\alpha(g) \geq \lambda(g) - \varepsilon$, où $\varepsilon$ est un nombre $> 0$; la mesure $\nu = \lambda - \lambda_\alpha$ étant positive, on a $\nu^\ast(f) \leq \nu(g) \leq \varepsilon$, ou $\lambda_\alpha^\ast(f) \geq \lambda^\ast(f) - \varepsilon$ (chap. IV, § 1, n° 3, prop. 15). Il en résulte ($\varepsilon$ étant arbitraire) que le second membre de (6) majore le premier ; l’inégalité inverse étant évidente, (6) est établie dans le cas particulier envisagé. Supposons ensuite que $f$ soit nulle hors de K, mais non nécessairement bornée, et posons $f_n = \inf(f, n)$ pour tout entier $n$. On a :

$$
\lambda^\bullet(f) = \sup_{n \in \mathbf{N}} \lambda^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \sup_{n \in \mathbf{N}} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Enfin, si l’on ne fait plus aucune restriction sur $f$, on a, en désignant par $\mathfrak{R}$ l’ensemble des parties compactes de T,

$$
\lambda^\bullet(f) = \sup_{K \in \mathfrak{R}} \lambda^\bullet(f \varphi_K) = \sup_{K \in \mathfrak{R}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f \varphi_K)
$$
$$
= \sup_{\alpha \in A} \sup_{K \in \mathfrak{R}} \lambda_\alpha^\bullet(f \varphi_K) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

#### Corollaire 1 {#int-v-s1-prop-11-cor-1 .statement}

Pour qu’une partie N de T soit localement $\lambda$-négligeable, il faut et il suffit que N soit localement $\lambda_\alpha$-négligeable pour tout $\alpha \in A$.

#### Corollaire 2 {#int-v-s1-prop-11-cor-2 .statement}

Pour qu’une application g de T dans un espace topologique G soit $\lambda$-mesurable, il faut et il suffit qu’elle soit $\lambda_\alpha$-mesurable pour tout $\alpha \in A$.

La condition est évidemment nécessaire, car $\lambda_\alpha \leq \lambda$ pour tout $\alpha$ (chap. IV, § 1, n° 3, prop. 15). Inversement, supposons que g soit $\lambda_\alpha$-mesurable pour tout $\alpha$, désignons par $\mathfrak{K}$ l’ensemble des compacts K de T tels que $g|K$ soit continue, et soit L un compact tel que $L \cap K$ soit $\lambda$-négligeable pour tout $K \in \mathfrak{K}$. L’ensemble $\mathfrak{K}$ étant $\lambda_\alpha$-dense, L est $\lambda_\alpha$-négligeable pour tout $\alpha$ (chap. IV, 2e éd., § 5, n° 8, prop. 12), donc $\lambda$-négligeable (cor. 1). Il en résulte que $\mathfrak{K}$ est $\lambda$-dense, et que g est $\lambda$-mesurable (chap. IV, 2e éd., § 5, n° 10, prop. 15).

## EXERCICES {#int-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
