---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 1
section_title: Définition des nombres réels
lang: fr
source: top-i-iv-fr
pdf_pages: 0272-0277, 0316-0318
extraction: ocr
subsections:
    - "no": 1
      title: Le groupe ordonné des nombres rationnels
      page: 0
      pdf_page: 272
    - "no": 2
      title: La droite rationnelle
      page: 2
      pdf_page: 273
    - "no": 3
      title: La droite numérique et les nombres réels
      page: 3
      pdf_page: 274
    - "no": 4
      title: Propriétés des intervalles de $\mathbf{R}$
      page: 4
      pdf_page: 275
    - "no": 5
      title: Longueur d’un intervalle
      page: 5
      pdf_page: 276
    - "no": 6
      title: Structure uniforme additive de $\mathbf{R}$
      page: 5
      pdf_page: 276
statements: 10
exercises: 4
content_sha256: fd5df639616d82158cf8dca2be2e0311092966782b7f22cb8d09501aa2eff54e
---

## § 1. DÉFINITION DES NOMBRES RÉELS

### 1. Le groupe ordonné des nombres rationnels

On a défini en Algèbre (A, I, p. 112), la relation d’ordre $x \leq y$ dans l’ensemble $\mathbf{Q}$ des nombres rationnels; on a vu qu’elle fait de $\mathbf{Q}$ un ensemble totalement ordonné, et qu’elle est compatible avec la structure de groupe additif de $\mathbf{Q}$, c’est-à-dire (A, VI, § 1, n° 1) que, pour tout $z \in \mathbf{Q}$, la relation $x \leq y$ est équivalente à $x + z \leq y + z$ (ce qu’on énonce encore en disant que l’ordre est invariant par translation). Rappelons que l’on pose, dans $\mathbf{Q}$ (comme dans tout groupe totalement ordonné),

$$
x^+ = \sup(x, 0), \quad x^- = \sup(-x, 0) = (-x)^+, \quad |x| = \sup(x, -x);
$$

$|x|$ est appelé valeur absolue de $x$; on a

$$
x = x^+ - x^-, \quad |x| = x^+ + x^-
$$

et l’inégalité du triangle

(1)
$$
|x + y| \leq |x| + |y|,
$$

ainsi que l’inégalité

(2)
$$
||x| - |y|| \leq |x - y|
$$

qui en est une conséquence immédiate; on a de même

(3)
$$
|x^+ - y^+| \leq |x - y|.
$$

Les relations $x \geq 0, x = x^+, x^- = 0, |x| = x$ (resp. $x \leq 0, x = -x^-, x^+ = 0, |x| = -x$) sont équivalentes. La relation $|x| = 0$ est équivalente à $x = 0$; si a \geqslant 0, la relation $|x| \leqslant a$ est équivalente à $-a \leqslant x \leqslant a$, la relation $|x| \geqslant a$ à «$x \geqslant a$ ou $x \leqslant -a$ ». Quels que soient $x, y, z$ dans $\mathbf{Q}$, on a
$$
\text{(4)} \quad \sup(x, y) + z = \sup(x + z, y + z)
$$
$$
\text{(5)} \quad \inf(x, y) = -\sup(-x, -y)
$$
et, comme cas particuliers,
$$
\text{(6)} \quad \sup(x, y) = x + (y - x)^+ = x + (x - y)^-
$$
$$
\text{(7)} \quad \inf(x, y) = x - (y - x)^- = x - (x - y)^+.
$$
Enfin, on désigne par $\mathbf{Q}_+$ l’ensemble des nombres rationnels $\geqslant 0$; on a les relations
$$
\text{(8)} \quad \mathbf{Q}_+ + \mathbf{Q}_+ \subset \mathbf{Q}_+
$$
$$
\text{(9)} \quad \mathbf{Q}_+ \cap (-\mathbf{Q}_+) = \{0\}
$$
$$
\text{(10)} \quad \mathbf{Q}_+ \cup (-\mathbf{Q}_+) = \mathbf{Q}.
$$
La relation $x \leqslant y$ est équivalente à $y - x \in \mathbf{Q}_+$.
Nous allons, à l’aide de cette relation d’ordre, définir sur $\mathbf{Q}$ une topologie compatible avec sa structure de groupe additif.

### 2. La droite rationnelle

Considérons l’ensemble $\mathcal{F}$ des intervalles ouverts symétriques $]-a, +a[$, où $a$ parcourt l’ensemble des nombres rationnels $> 0$; nous allons montrer que $\mathcal{F}$ est un système fondamental de voisinages de $0$ dans une topologie compatible avec la structure de groupe additif de $\mathbf{Q}$.

Le groupe $\mathbf{Q}$ est commutatif, et l’axiome (GV$_{\mathrm{II}}'$) (III, p. 4) est évidemment vérifié; il suffit donc de voir que (GV$_{\mathrm{I}}'$) (III, p. 4) l’est aussi, autrement dit que, pour tout $a > 0$, il existe $b > 0$ tel que les conditions $|x| < b, |y| < b$ entraînent $|x + y| < a$; or, d’après l’inégalité du triangle, il suffit de prendre $b = a/2$.

#### Définition 1 {#top-iv-s1-def-1 .statement}

On appelle droite rationnelle l’espace topologique obtenu en munissant l’ensemble $\mathbf{Q}$ de la topologie de groupe dont un système fondamental de voisinages de $0$ est formé par les intervalles ouverts symétriques $]-a, +a[$ ($a > 0$).

Le groupe topologique $\mathbf{Q}$ ainsi défini est appelé groupe additif de la droite rationnelle.

Quel que soit le nombre rationnel $a > 0$, il existe un entier $n > 0$ tel que $1/n < a$; les intervalles ouverts $]-\frac{1}{n}, +\frac{1}{n}[$ ($n = 1, 2, \ldots$) forment donc un système fondamental de voisinages de $0$ sur la droite rationnelle.

On a un système fondamental de voisinages d’un point quelconque $x \in \mathbf{Q}$, en prenant les intervalles ouverts $]x - a, x + a[$, où $a$ parcourt l’ensemble des nombres rationnels $> 0$ (ou seulement l’ensemble des nombres $1/n$).

La définition 1 est donc équivalente à celle que nous avons donnée dans I, p. 4.

Pour tout couple $(a, b)$ tel que $a < b$, il existe $c \in \mathbf{Q}$ tel que $a < c < b$ (par exemple $c = (a + b)/2$); il en résulte que la droite rationnelle est un espace séparé et non discret.

Pour tout $a > 0$, soit $U_a$ l’ensemble des couples $(x, y)$ de $\mathbf{Q} \times \mathbf{Q}$ tels que $|x - y| < a$; lorsque $a$ parcourt l’ensemble des nombres rationnels $> 0$ (ou seulement l’ensemble des nombres $1/n$), les ensembles $U_a$ forment un système fondamental d’entourages de la structure uniforme du groupe additif $\mathbf{Q}$ de la droite rationnelle. Les relations (2) et (3) (IV, p. 1) montrent que $|x|$, $x^+$ et $x^-$ sont uniformément continues dans $\mathbf{Q}$. Il s’ensuit que les fonctions $\sup(x, y)$ et $\inf(x, y)$ sont uniformément continues dans $\mathbf{Q} \times \mathbf{Q}$.

### 3. La droite numérique et les nombres réels

#### Définition 2 {#top-iv-s1-def-2 .statement}

On désigne par $\mathbf{R}$ le groupe topologique complété du groupe additif $\mathbf{Q}$ de la droite rationnelle. Les éléments de $\mathbf{R}$ sont appelés nombres réels; en tant qu’espace topologique, $\mathbf{R}$ est appelé droite numérique; en tant que groupe topologique, on l’appelle groupe additif de la droite numérique.

On identifiera toujours $\mathbf{Q}$ avec le sous-groupe partout dense de $\mathbf{R}$, auquel il est canoniquement isomorphe; avec cette convention, tout nombre rationnel est un nombre réel. Tout nombre réel non rationnel est dit irrationnel; on a vu dans II, p. 15 qu’il en existe (on le verra d’une autre manière dans IV, p. 12; voir aussi IV, p. 47, exerc. 2); donc (III, p. 8, Remarque), l’ensemble $\mathbf{CQ}$ des nombres irrationnels est partout dense dans $\mathbf{R}$.

Nous allons voir qu’on peut prolonger à $\mathbf{R}$ la structure d’ordre de $\mathbf{Q}$, de manière que la structure d’ordre prolongée soit encore compatible avec la structure de groupe additif de $\mathbf{R}$:

#### Proposition 1 {#top-iv-s1-prop-1 .statement}

La relation $y - x \in \overline{\mathbf{Q}}_+$ est une relation d’ordre dans $\mathbf{R}$, qui fait de $\mathbf{R}$ un ensemble totalement ordonné, est compatible avec la structure de groupe additif de $\mathbf{R}$, et induit sur $\mathbf{Q}$ la relation d’ordre $x \leqslant y$.

Montrons d’abord que les relations $y - x \in \overline{\mathbf{Q}}_+$ et $z - y \in \overline{\mathbf{Q}}_+$ entraînent $z - x \in \overline{\mathbf{Q}}_+$; en effet, la fonction $x + y$ est continue dans $\mathbf{R} \times \mathbf{R}$; d’après (8) (IV, p. 2), on a donc $\overline{\mathbf{Q}}_+ + \overline{\mathbf{Q}}_+ \subset \overline{\mathbf{Q}}_+$ (I, p. 9, th. 1). En second lieu, on va voir que les relations $y - x \in \overline{\mathbf{Q}}_+$ et $x - y \in \overline{\mathbf{Q}}_+$ entraînent $x = y$, ce qui établit que $y - x \in \overline{\mathbf{Q}}_+$ est une relation d’ordre dans $\mathbf{R}$. Montrons pour cela que $\overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+) = \{0\}$; les fonctions $x \mapsto x^+$ et $x \mapsto x^-$ étant uniformément continues dans $\mathbf{Q}$, se prolongent par continuité dans $\mathbf{R}$ (II, p. 20, th. 2); soient $f$ et $g$ leurs prolongements respectifs. On a par prolongement $x = f(x) - g(x)$ quel que soit $x \in \mathbf{R}$; pour $x \in \overline{\mathbf{Q}}_+, g(x) = 0$; d’autre part, comme $-\overline{\mathbf{Q}}_+$ est l’adhérence de $-\mathbf{Q}_+$ d’après la continuité de $-x$, on a $f(x) = 0$ pour $x \in -\overline{\mathbf{Q}}_+$. Donc, pour $x \in \overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+)$, $f(x) = g(x) = 0$, d’où $x = 0$.

D’après (10) (IV, p. 2), on a $\overline{\mathbf{Q}}_+ \cup (-\overline{\mathbf{Q}}_+) = \mathbf{R}$, donc $\mathbf{R}$ est totalement ordonné par la relation d’ordre $y - x \in \overline{\mathbf{Q}}_+$.

En outre, comme les relations $y - x \in \overline{\mathbf{Q}}_+$ et $(y + z) - (x + z) \in \overline{\mathbf{Q}}_+$ sont équivalentes, la relation d’ordre $y - x \in \overline{\mathbf{Q}}_+$ est bien compatible avec la structure de groupe additif de $\mathbf{R}$.

Enfin, si $x$ et $y$ appartiennent à $\mathbf{Q}$, les relations $y - x \in \overline{\mathbf{Q}}_+$ et $y - x \in \mathbf{Q}_+$ sont équivalentes, ce qui achève la démonstration, en prouvant que la relation d’ordre $y - x \in \overline{\mathbf{Q}}_+$ induit sur $\mathbf{Q}$ la relation $x \leq y$; on la notera encore $x \leq y$.

L’ensemble $\overline{\mathbf{Q}}_+$ est identique à l’ensemble des $x \geq 0$ dans $\mathbf{R}$; on l’écrira $\mathbf{R}_+$; c’est un ensemble fermé. On désignera par $\mathbf{R}_+^*$ l’ensemble des $x > 0$; c’est le complémentaire de $-\mathbf{R}_+$, donc c’est un ensemble ouvert dans $\mathbf{R}$.

### 4. Propriétés des intervalles de $\mathbf{R}$

#### Proposition 2 {#top-iv-s1-prop-2 .statement}

Tout intervalle fermé (resp. ouvert) de $\mathbf{R}$, est un ensemble fermé (resp. ouvert) dans $\mathbf{R}$.

En effet, les ensembles $\{a, \rightarrow[ = a + \mathbf{R}_+ \text{ et } ]\leftarrow, a\} = a - \mathbf{R}_+$ se déduisent par translation de $\mathbf{R}_+$ et $-\mathbf{R}_+$ respectivement, donc (III, p. 2) sont fermés; les ensembles $]\leftarrow, a[$ et $]a, \rightarrow[$, qui en sont les complémentaires respectifs, sont ouverts; enfin, l’intervalle fermé $[a, b]$ (resp. l’intervalle ouvert $]a, b[$), intersection de $\{a, \rightarrow[$ et $]\leftarrow, b\}$ (resp. de $]a, \rightarrow[$ et $]\leftarrow, b[$) est un ensemble fermé (resp. ouvert).

Les intervalles fermés $[-a, +a]$ ($a > 0$) de $\mathbf{R}$ sont donc des voisinages de 0; montrons qu’ils forment un système fondamental de voisinages de 0 lorsque $a$ parcourt $\mathbf{R}_+^*$. Il suffit d’établir la proposition suivante:

#### Proposition 3 {#top-iv-s1-prop-3 .statement}

Lorsque $r$ parcourt l’ensemble des nombres rationnels $> 0$, les intervalles $S_r = (-r, +r)$ de $\mathbf{R}$ forment un système fondamental de voisinages de 0.

En effet (III, p. 24, prop. 7), on obtient un système fondamental de voisinages de 0 dans $\mathbf{R}$ en prenant les adhérences, dans $\mathbf{R}$, des intervalles $S_r \cap \mathbf{Q} = (-r, +r)$ de $\mathbf{Q}$. La proposition sera démontrée si on établit que $S_r$ est l’adhérence de $S_r \cap \mathbf{Q}$. Or, $S_r$ est fermé dans $\mathbf{R}$; il suffit donc de montrer que, si $x$ est un nombre réel tel que $-r < x < r$, $x$ est adhérent à $S_r \cap \mathbf{Q}$. Or, $]-r, +r[$ est un ensemble ouvert dans $\mathbf{R}$, donc, pour tout voisinage assez petit $V$ de 0 dans $\mathbf{R}$, $x + V \subset ]-r, +r[$; mais, comme $\mathbf{Q}$ est partout dense dans $\mathbf{R}$, il existe un nombre rationnel $r' \in x + V$, et on a donc $-r < r' < r$, c’est-à-dire $r' \in S_r \cap \mathbf{Q}$.

#### Corollaire {#top-iv-s1-n4-cor-1 .statement}

Tout point de la droite numérique possède un système fondamental dénombrable de voisinages.

#### Proposition 4 {#top-iv-s1-prop-4 .statement}

Pour tout couple $(x, y)$ de nombres réels tels que $x < y$, il existe un nombre rationnel $r$ tel que $x < r < y$.

Comme $\mathbf{Q}$ est partout dense dans $\mathbf{R}$, il suffit de voir que $]x, y[$ n’est pas vide;

par translation, on se ramène au cas où $x = 0, y > 0$. Or, $\mathbf{R}$ étant un espace séparé, il existe, d’après la prop. 3, un nombre rationnel $r > 0$ tel que $y \notin (-r, +r)$, ce qui entraîne $0 < r < y$.

#### Proposition 5 {#top-iv-s1-prop-5 .statement}

*Soit I un intervalle quelconque de $\mathbf{R}$. La topologie induite sur I par celle de $\mathbf{R}$ est engendrée par l’ensemble des intervalles ouverts de I* (I étant considéré comme ensemble totalement ordonné par la relation $x \leq y$).

Tout intervalle ouvert de I est la trace sur I d’un intervalle ouvert de $\mathbf{R}$: c’est évident pour un intervalle borné; et l’intervalle illimité $]a, \rightarrow[$ de I est la trace de l’intervalle illimité $]a, \rightarrow[$ de $\mathbf{R}$. On peut donc se borner au cas où $I = \mathbf{R}$; mais alors, la proposition résulte de la prop. 3, car tout voisinage d’un point $x \in \mathbf{R}$ contient un intervalle ouvert $]x - a, x + a[$.

#### Remarque {#top-iv-s1-n4-rem-1 .statement}

Si A est une partie *partout dense* de $\mathbf{R}$, la topologie de $\mathbf{R}$ est encore engendrée par l’ensemble des intervalles ouverts dont les extrémités appartiennent à A. En effet, si $]x - a, x + a[$ est un intervalle ouvert contenant x, il existe deux points $y, z$ de A tels que $x - a < y < x < z < x + a$; donc $]y, z[$ contient x et est contenu dans $]x - a, x + a[$. Ce raisonnement montre même que les intervalles considérés forment une *base* (I, p. 5) de la topologie de $\mathbf{R}$. En particulier, si on prend $A = \mathbf{Q}$, on voit que la topologie de $\mathbf{R}$ a une *base dénombrable*.

### 5. Longueur d’un intervalle

#### Définition 3 {#top-iv-s1-def-3 .statement}

*On appelle longueur d’un intervalle borné d’origine a et d’extrémité b, le nombre réel positif $b - a$*.

Tout intervalle borné contenant plus d’un point a donc une longueur $> 0$. Si $a \leq b$, les quatre intervalles $[a, b]$, $]a, b[$, $[a, b[$, $]a, b]$ ont même longueur. Un intervalle d’extrémités $a + c$ et $b + c$ a même longueur que l’intervalle d’extrémités $a$ et $b$: en d’autres termes, *la longueur d’un intervalle est invariante par translation*.

Si $a \leq c \leq d \leq b$, on a $d - c \leq b - a$; donc, si un intervalle borné I est contenu dans un intervalle borné I’, la longueur de I est inférieure à celle de I’.

Si n intervalles ouverts, $I_1, I_2, \ldots, I_n$ sans point commun deux à deux, sont contenus dans l’intervalle $(a, b)$ ($a < b$), on voit aisément, par récurrence sur n, que, si $I_k = ]c_k, d_k[$, il existe une permutation $\sigma$ des indices $k$ ($1 \leq k \leq n$) telle que l’on ait $d_{\sigma(k)} \leq c_{\sigma(k+1)}$ pour $1 \leq k \leq n - 1$. Il en résulte immédiatement que la somme des longueurs des intervalles $I_k$ est au plus égale à la longueur de $(a, b)$; elle ne peut lui être égale que si $c_{\sigma(1)} = a, d_{\sigma(n)} = b$ et $d_{\sigma(k)} = c_{\sigma(k+1)}$ pour $1 \leq k \leq n - 1$.

### 6. Structure uniforme additive de $\mathbf{R}$

Le groupe $\mathbf{R}$ étant totalement ordonné, les fonctions $x^+, x^-$ et $|x|$ sont définies dans $\mathbf{R}$ de la même manière que dans $\mathbf{Q}$ et satisfont à toutes les relations rappelées ci-dessus pour $\mathbf{Q}$, notamment aux relations (1) à (7) (IV, p. 1 et 2). Soit $a$ un nombre réel $> 0$, et $U_a$ l’ensemble des couples $(x, y) \in \mathbf{R} \times \mathbf{R}$ tels que $|x - y| < a$; lorsque $a$ parcourt l’ensemble des nombres réels $> 0$ (ou seulement l’ensemble des nombres $1/n$), les ensembles $U_a$ forment un *système fondamental d’entourages* de la structure uniforme du groupe additif $\mathbf{R}$ de la droite numérique (dite encore *structure uniforme additive de la droite numérique*).

Les fonctions $|x|$, $x^+$ et $x^-$ sont *uniformément continues* dans $\mathbf{R}$, les fonctions $\sup(x, y)$ et $\inf(x, y)$ *uniformément continues* dans $\mathbf{R} \times \mathbf{R}$; ces fonctions sont donc identiques à celles qu’on obtient en *prolongeant par continuité* les fonctions de même nom définies dans $\mathbf{Q}$ et dans $\mathbf{Q} \times \mathbf{Q}$ respectivement.

## EXERCICES {#top-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
