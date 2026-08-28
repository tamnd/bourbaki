---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 9
section_title: Espaces affines et espaces projectifs
lang: fr
source: alg-i-iii-fr
book_pages: A II.126-A II.138, A II.200-A II.205
pdf_pages: 0303-0315, 0377-0382
extraction: ocr
subsections:
    - "no": 1
      title: Définition des espaces affines
      page: 126
      pdf_page: 303
    - "no": 2
      title: Calcul barycentrique
      page: 127
      pdf_page: 304
    - "no": 3
      title: Variétés linéaires affines
      page: 128
      pdf_page: 305
    - "no": 4
      title: Applications linéaires affines
      page: 130
      pdf_page: 307
    - "no": 5
      title: Définition des espaces projectifs
      page: 132
      pdf_page: 309
    - "no": 6
      title: Coordonnées homogènes
      page: 133
      pdf_page: 310
    - "no": 7
      title: Variétés linéaires projectives
      page: 133
      pdf_page: 310
    - "no": 8
      title: Complétion projective d’un espace affine
      page: 135
      pdf_page: 312
    - "no": 9
      title: Prolongement des fonctions rationnelles
      page: 136
      pdf_page: 313
    - "no": 10
      title: Applications linéaires projectives
      page: 136
      pdf_page: 313
    - "no": 11
      title: Structure d’espace projectif
      page: 138
      pdf_page: 315
statements: 12
exercises: 19
content_sha256: 1d7531690af2a3fe0e1c72b9ec9d09166704bcb341f6cfad216a6511a30de7f8
---

## § 9. ESPACES AFFINES ET ESPACES PROJECTIFS

### 1. Définition des espaces affines

#### Définition 1 {#alg-ii-s9-def-1 .statement}

Étant donné un espace vectoriel à gauche (resp. à droite) T sur un corps K, on appelle espace affine attaché à T tout ensemble homogène E du groupe additif T (I, p. 56) tel que O soit le seul opérateur de T laissant invariants tous les éléments de E (c’est-à-dire que T opère fidèlement et transitivement dans E). Dans ces conditions, T s’appelle l’espace des translations de E, et ses éléments s’appellent les translations de E (ou les vecteurs libres de E).

Dans ce qui suit, nous nous bornerons au cas où T est un espace vectoriel à gauche sur K. La dimension (sur K) de l’espace vectoriel des translations T d’un espace affine E s’appelle la dimension de E (sur K), et se note dim E ou dim_K E. Un espace affine de dimension un (resp. deux) s’appelle une droite affine (resp. un plan affine). Les éléments d’un espace affine sont encore qualifiés de points.

Dans les conditions de la déf. 1, pour t ∈ T et a ∈ E, nous noterons t + a ou a + t le transformé du point a par t. On a donc les relations

(1)
$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$
pour s ∈ T, t ∈ T, a ∈ E. L’application x ↦ x + t est une bijection de E sur lui-même, qu’on identifie à t. La déf. 1 entraîne en outre que, pour tout a ∈ E, l’application t ↦ t + a est une bijection de T sur E. Autrement dit, étant donnés deux points a, b de E, il existe une translation t et une seule telle que b = t + a; nous noterons cette translation b − a; on a donc les formules

(2)
$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a,
$$
$$
(c - b) + (b - a) = c - a
$$
pour a ∈ E, b ∈ E, c ∈ E. Si quatre points a, b, a', b' de E sont tels que b − a = b' − a', la formule
$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$
et la commutativité de l’addition dans T montrent que l’on a b' − b = a' − a.

Étant donné un point a ∈ E, l’application x ↦ x − a est une bijection de E sur T; quand on identifie E à T par cette application, on dit qu’on considère E comme espace vectoriel obtenu en prenant a pour origine dans E. Inversement, tout espace vectoriel T est canoniquement muni d’une structure d’espace affine attaché à T, à savoir la structure d’espace homogène correspondant au sous-groupe {0} de T (I, p. 59).

#### Remarque {#alg-ii-s9-n1-rem-1 .statement}

Les définitions de ce n°, et une partie des résultats qui suivent, s’étendent immédiatement au cas où, au lieu d’un espace vectoriel T, on considère un groupe commutatif à opérateurs quelconque T.

### 2. Calcul barycentrique

#### Proposition 1 {#alg-ii-s9-prop-1 .statement}

Soient (x_i)_{i \in I} une famille de points d’un espace affine E, et (\lambda_i)_{i \in I} une famille d’éléments de K, de support fini, telle que $\sum_{i \in I} \lambda_i = 1$ (resp. $\sum_{i \in I} \lambda_i = 0$). Si a est un point quelconque de E, le point x ∈ E défini par
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
(resp. le vecteur libre $\sum_{i \in I} \lambda_i (x_i - a)$) est indépendant du point a considéré.

En effet, si a' est un second point de E, on a
$$
\sum_{i} \lambda_i (x_i - a') = \sum_{i} \lambda_i ((x_i - a) + (a - a')) = \sum_{i} \lambda_i (x_i - a) + (\sum_{i} \lambda_i)(a - a').
$$

Si $\sum_i \lambda_i = 1$, on en déduit $\sum_i \lambda_i(x_i - a') = (x - a) + (a - a') = x - a'$; si $\sum_i \lambda_i = 0$, on a $\sum_i \lambda_i(x_i - a') = \sum_i \lambda_i(x_i - a)$; d’où la proposition.

Dans les conditions de la prop. 1, on note $\sum_{i \in I} \lambda_i x_i$ le point $x$ défini par $x - a = \sum_{i \in I} \lambda_i(x_i - a)$ (resp. le vecteur libre $\sum_{i \in I} \lambda_i(x_i - a)$).

On retrouve ainsi en particulier la notation $b - a$ introduite dans II, p. 127. Lorsque $\sum_i \lambda_i = 1$, le point $x = \sum_i \lambda_i x_i$ s’appelle le *barycentre des points* $x_i$ *affectés des masses* $\lambda_i$.

Étant donnés $m$ points $a_1, \ldots, a_m$ de E, dont le nombre $m$ ne soit pas multiple de la caractéristique de $K$ (V, §1), le point $g = \sum_{i=1}^m \frac{1}{m} a_i$ s’appelle (par abus de langage) *le barycentre des points* $a_i$ ($1 \leq i \leq m$) (pour $m = 2$, on dit « milieu » au lieu de « barycentre »); il est caractérisé par la relation $\sum_{i=1}^m (a_i - g) = 0$.

### 3. Variétés linéaires affines

#### Définition 2 {#alg-ii-s9-def-2 .statement}

Étant donné un espace affine E, on dit qu’une partie V de E est une variété linéaire affine (ou simplement une variété linéaire ou un sous-espace affine de E) *si, pour toute famille* $(x_i)_{i \in I}$ *de points de* V, *et toute famille* $(\lambda_i)_{i \in I}$ *d’éléments de* K, *de support fini et telle que* $\sum_{i \in I} \lambda_i = 1$, *le barycentre* $\sum_{i \in I} \lambda_i x_i$ *appartient à* V.

Il revient au même de dire que la condition de la déf. 2 est vérifiée pour toute famille *finie* de points de V.

L’ensemble vide est une variété linéaire; toute intersection de variétés linéaires est une variété linéaire.

Soient V une partie non vide de E, a un point de V; la relation

$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$

signifie que $x$ est un barycentre $\sum_{i=1}^n \lambda_i x_i + (1 - \sum_{i=1}^n \lambda_i)a$ de la famille formée des $x_i$ et de $a$. Par suite:

#### Proposition 2 {#alg-ii-s9-prop-2 .statement}

Pour qu’une partie non vide V d’un espace affine E soit une variété linéaire, il faut et il suffit que V soit un sous-espace vectoriel pour la structure d’espace vectoriel de E obtenue en prenant un point de V comme origine.

En particulier, les variétés linéaires affines non vides d’un espace vectoriel T (considéré comme espace affine) ne sont autres que les *translatés* des sous-espaces vectoriels de T; les sous-espaces vectoriels de T sont donc les variétés linéaires contenant 0.

Soit V une variété linéaire non vide de l’espace affine E; l’ensemble des vecteurs libres $x - y$, où $x$ et $y$ parcourent V, est un sous-espace vectoriel D de l’espace des translations T de E, qu’on appelle la direction de V : en effet, si $a \in V$, on peut écrire
$$
x - y = (x - a) - (y - a),
$$
et notre assertion résulte de la prop. 2 de II, p. 128. Il est immédiat que D opère fidèlement et transitivement dans V, qui est donc canoniquement muni d’une structure d’espace affine attaché à D. Par dimension de la variété linéaire V, on entendra la dimension de V pour cette structure d’espace affine, c’est-à-dire la dimension de l’espace vectoriel D. Les variétés linéaires de dimension 0 sont les points de E; celles de dimension 1 (resp. 2) sont appelées les droites (resp. les plans) de E.

Tout vecteur $\neq 0$ appartenant à la direction d’une droite est appelé vecteur directeur de cette droite; ses composantes par rapport à une base de T forment ce qu’on appelle un système de paramètres directeurs de la droite considérée.

On appelle codimension d’une variété linéaire V dans E la codimension de sa direction D dans T; une variété linéaire de codimension 1 dans E s’appelle un hyperplan (affine) de E.

Deux variétés linéaires de même direction sont dites parallèles; il revient au même de dire qu’elles se déduisent l’une de l’autre par translation. Si V est une variété linéaire dans T (considéré comme espace affine), sa direction est la variété linéaire parallèle à V et contenant 0.

#### Proposition 3 {#alg-ii-s9-prop-3 .statement}

Étant donnée une famille $(a_i)_{i \in I}$ de points d’un espace affine E, l’ensemble V des barycentres $\sum_{i \in I} \lambda_i a_i \ ((\lambda_i) \text{ de support fini}, \sum_{i \in I} \lambda_i = 1)$ est une variété linéaire de E.

Si la famille $(a_i)$ est vide, on a $V = \varnothing$, à cause de la condition $\sum_i \lambda_i = 1$. On peut donc supposer la famille $(a_i)$ non vide, et dans ce cas la proposition est évidente, en prenant un des $a_i$ pour origine de E.

La variété V est évidemment la plus petite variété linéaire contenant les $a_i$; on dit qu’elle est engendrée par la famille $(a_i)$ et que cette famille est un système générateur de V.

Avec les notations de la prop. 3, et en supposant la famille $(a_i)$ non vide, pour que l’expression de tout point $x \in V$ sous la forme $x = \sum_i \lambda_i a_i$ soit unique, il faut et il suffit que, en désignant par $\kappa$ un indice quelconque de I, la famille des vecteurs $a_i - a_\kappa$, où $i$ parcourt l’ensemble des indices $\neq \kappa$, soit libre dans T. On dit alors que la famille $(a_i)_{i \in I}$ de points de E est affinement libre (ou que ses éléments forment un système affinement libre, ou sont affinement indépendants), et que $\lambda_i$ est la coordonnée barycentrique d’indice $i$ de $x$ par rapport à la famille affinement libre $(a_i)$.

On dit qu’une famille $(a_i)_{i \in I}$ de points de $E$ qui n’est pas affinement libre est *affinement liée*.

#### Proposition 4 {#alg-ii-s9-prop-4 .statement}

*Pour qu’une famille non vide $(a_i)_{i \in I}$ de points d’un espace affine $E$ soit affinement liée, il faut et il suffit qu’il existe une famille $(\lambda_i)_{i \in I}$ d’éléments non tous nuls de $\mathbf{K}$, de support fini, telle que $\sum_{i \in I} \lambda_i = 0$ et $\sum_{i \in I} \lambda_i a_i = 0$.

En effet, étant donné un indice $\kappa \in I$, dire que la famille de vecteurs $(a_i - a_\kappa)$, où $i$ parcourt l’ensemble des indices $\neq \kappa$, est liée dans $T$, signifie qu’il existe une famille de scalaires $(\lambda_i)_{i \neq \kappa}$ non tous nuls, tels que $\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$, ce qui s’écrit aussi $\sum_{i \in I} \lambda_i a_i = 0$, avec $\lambda_\kappa = - \sum_{i \neq \kappa} \lambda_i$, autrement dit $\sum_{i \in I} \lambda_i = 0$.

#### Proposition 5 {#alg-ii-s9-prop-5 .statement}

*Pour qu’une famille non vide $(a_i)_{i \in I}$ de points d’un espace affine $E$ soit affinement libre, il faut et il suffit que, quel que soit l’indice $\kappa \in I$, $a_\kappa$ n’appartienne pas à la variété linéaire engendrée par les $a_i$ d’indice $\neq \kappa$.

La proposition est évidente si $I$ n’a qu’un seul élément. Sinon, en prenant pour origine dans $E$ un des $a_i$ d’indice $\neq \kappa$, la proposition résulte de II, p. 96, *Remarque*.

### 4. Applications linéaires affines

#### Définition 3 {#alg-ii-s9-def-3 .statement}

*Étant donnés deux espaces affines $E, E'$, attachés à deux espaces vectoriels, $T, T'$ sur un même corps $\mathbf{K}$, on dit qu’une application $u$ de $E$ dans $E'$ est une application linéaire affine (ou simplement une application affine) si, quelles que soient la famille $(x_i)_{i \in I}$ de points de $E$ et la famille $(\lambda_i)_{i \in I}$ de scalaires telle que $\sum_{i \in I} \lambda_i = 1$, on a*

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

#### Proposition 6 {#alg-ii-s9-prop-6 .statement}

*Soit $u$ une application affine de $E$ dans $E'$. Il existe une application linéaire $v$ et une seule de $T$ dans $T'$ telle que*

$$
u(x + t) = u(x) + v(t)
$$

*quels que soient* $x \in E, t \in T$.

En effet, soit $a$ un point quelconque de $E$. L’application

$$
t \mapsto u(a + t) - u(a)
$$

est une application linéaire $v_a$ de $T$ dans $T'$, car on peut écrire

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a
$$
$$
a + s + t = (a + s) + (a + t) - a
$$

et on tire de (3) que $v_a(\lambda t) = \lambda v_a(t)$ et $v_a(s + t) = v_a(s) + v_a(t)$. En outre, si b est un second point de E, on a $v_a = v_b$; en effet, la relation $(a + t) - a + b = b + t$ entraîne

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

c’est-à-dire $u(a + t) - u(a) = u(b + t) - u(b)$. D’où l’existence de $v$; l’unicité est immédiate.

On dit que $v$ est l’application linéaire de T dans $T'$ associée à $u$. Inversement, pour toute application linéaire $v$ de T dans $T'$ et tout couple de points $a \in E$, $a' \in E'$, on vérifie aussitôt que

$$
x \mapsto a' + v(x - a)
$$

est une application affine de E dans $E'$, dont $v$ est l’application linéaire associée. Dire que $u$ est une application affine de E dans $E'$ signifie donc encore que, si on prend comme origines dans E un point quelconque $a$ et dans $E'$ le point $u(a)$, $u$ est une application *linéaire* pour les deux espaces vectoriels ainsi obtenus.

Soient $E''$ un troisième espace affine, $T''$ son espace des translations, $u'$ une application affine de $E'$ dans $E''$, $v'$ l’application linéaire de $T'$ dans $T''$ associée à $u'$. Il est clair que $u' \circ u$ est une application affine de E dans $E''$; en outre, pour $a \in E$ et $t \in T$, on a

$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$

donc $v' \circ v$ est l’application linéaire de T dans $T''$ associée à $u' \circ u$. Pour qu’une application affine $u$ soit bijective, il faut et il suffit que l’application linéaire associée $v$ le soit, et $u^{-1}$ est alors une application affine, dont $v^{-1}$ est l’application linéaire associée.

En particulier, les bijections affines de E sur lui-même forment un groupe G, appelé *groupe affine* de E. L’application qui, à tout $u \in G$, fait correspondre l’application linéaire $v$ associée à $u$, est, d’après ce qui précède, un *homomorphisme* de G *sur le groupe linéaire* $\mathbf{GL}(T)$. Si $u$ est une translation $x \mapsto x + t$, $v$ est l’identité, et réciproquement. Donc, le noyau de l’homomorphisme précédent s’identifie au groupe T des translations de E, qui est par suite un *sous-groupe distingué* de G.

Si $u \in G$, l’automorphisme $t \mapsto utu^{-1}$ de T (où $t$ est identifié à la translation $x \mapsto x + t$) est l’application linéaire $v$ associée à $u$. En effet, pour $x \in E$ et $t \in T$, on a par définition

$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t),
$$

donc $utu^{-1} = v(t)$.

Soient $a \in E$, et $G_a$ le sous-groupe de G formé des $u \in G$ tels que $u(a) = a$. Si on identifie E à T en prenant $a$ pour origine, $G_a$ s’identifie à $\mathbf{GL}(T)$. Tout $u \in G$ se met, d’une manière unique, sous la forme $u = t_1 u_1$ (resp. sous la forme $u = u_2 t_2$), où $u_1, u_2$ sont dans $G_a$ et $t_1, t_2$ dans T: en effet, posant $t_1 = u(a) - a$, on a $u^{-1} t_1 \in G_a$, d’où l’existence de $u_1$ et $t_1$; on obtient l’existence de $u_2$ et $t_2$ de manière analogue. L’unicité résulte du fait que $G_a \cap T$ se réduit à l’élément neutre de $G$. D’ailleurs
$$
t_1 u_1 = u_1 (u_1^{-1} t_1 u_1)
$$
d’où $u_2 = u_1, t_2 = u_1^{-1} t_1 u_1$. Enfin, les application linéaires associées à $u$ et $u_1$ sont les mêmes, donc, si on identifie comme plus haut $G_a$ à $\mathbf{GL}(T)$, $u_1$ est l’application linéaire de $T$ dans lui-même associée à $u$. On voit donc que $G$ est *produit semi-direct* de $G_a$ par $T$ (I, p 65.).

Soient $E, E'$ deux espaces affines sur $K$. L’image directe (resp. réciproque) d’une variété linéaire de $E$ (resp. $E'$) par une application affine $u$ de $E$ dans $E'$ est une variété linéaire de $E'$ (resp. $E$) ; le *rang* de $u$ est par définition la dimension de $u(E)$ ; il est égal au rang de l’application linéaire associée à $u$. Si $V, V'$ sont des variétés linéaires de même dimension finie $m$ dans $E, E'$ respectivement, il existe une application affine $u$ de $E$ dans $E'$ telle que $u(V) = V'$ : en prenant pour origines dans $E$ et $E'$ des points de $V$ et $V'$ respectivement, puis en prenant dans $E$ (resp. $E'$) une base dont les $m$ premiers vecteurs forment une base de $V$ (resp. $V'$), la proposition résulte aussitôt de II, p. 25, cor. 3.

Comme le corps $K$ est canoniquement muni d’une structure d’espace vectoriel à gauche (de dimension 1) sur $K$, il peut être considéré comme espace affine de dimension 1. Une application affine d’un espace affine $D$ (sur $K$) dans l’espace affine $K$ s’appelle encore une *fonction linéaire affine* (ou *fonction affine*). Si on prend pour origine dans $E$ un point $a$, toute fonction affine sur $E$ peut donc s’écrire d’une seule manière $x \mapsto \alpha + v(x)$, où $\alpha \in K$ et où $v$ est une forme linéaire sur l’espace vectoriel $E$ ainsi obtenu ; les fonctions affines sur $E$ forment donc un *espace vectoriel à droite sur $K$*, de dimension $1 + \dim E$. Si $u$ est une fonction affine non constante sur $E$, et $\lambda \in K$, l’ensemble des $x \in E$ satisfaisant à l’équation $u(x) = \lambda$ est un hyperplan ; réciproquement, pour tout hyperplan $H$ dans $E$, il existe une fonction affine $u_0$ sur $E$ telle que $H = \overline{u_0}(0)$, et toute fonction affine $u$ telle que $H = \overline{u}(0)$ est de la forme $u_0 \mu$, où $\mu \in K$ (II, p. 106, prop. 11). Si $u$ est une fonction affine non constante sur $E$, les hyperplans d’équations $u(x) = \alpha$ et $u(x) = \beta$ sont parallèles.

### 5. Définition des espaces projectifs

#### Définition 4 {#alg-ii-s9-def-4 .statement}

*Étant donné un espace vectoriel à gauche* (resp. *à droite*) $V$ *sur un corps* $K$, *on appelle espace projectif à gauche* (resp. *à droite*) *déduit de* $V$, *et on note* $\mathbf{P}(V)$, *le quotient du complémentaire* $V - \{0\}$ *de* $\{0\}$ *dans* $V$, *par la relation d’équivalence* $\Delta(V)$ : « *il existe* $\lambda \neq 0$ *dans* $K$ *tel que* $y = \lambda x$ (resp. $y = x \lambda$) » *entre* $x$ *et* $y$ *dans* $V - \{0\}$.

Lorsque $V = K_s^{n+1}$, on écrit encore $\mathbf{P}_n(K)$ au lieu de $\mathbf{P}(K_s^{n+1})$ et $\Delta_n(K)$ au lieu de $\Delta(V)$.

La déf. 4 s’exprime aussi en disant que $\mathbf{P}(V)$ est l’ensemble des droites (passant par 0) de V, privées de l’origine; $\mathbf{P}(V)$ s’identifie donc canoniquement à l’ensemble des droites (passant par 0) de V. Les éléments d’un espace projectif sont appelés points de cet espace.

Lorsque V est de dimension $n$, on appelle dimension de l’espace projectif $\mathbf{P}(V)$ l’entier $n - 1$ si $n$ est fini, et le cardinal $n$ dans le cas contraire; on note ce cardinal $\dim_K \mathbf{P}(V)$, ou $\dim \mathbf{P}(V)$. Ainsi, un espace projectif de dimension — 1 est vide, et un espace projectif de dimension 0 est réduit à un point. Un espace projectif de dimension 1 (resp. 2) s’appelle une droite projective (resp. un plan projectif).

Nous ne considérerons désormais que des espaces projectifs à gauche.

### 6. Coordonnées homogènes

Soient V un espace vectoriel de dimension finie $n + 1$ sur K, $\mathbf{P}(V)$ l’espace projectif de dimension $n$ déduit de V, $(e_i)_{0 \leq i \leq n}$ une base de V. Désignons par $\pi$ l’application canonique de $V - \{0\}$ sur l’ensemble quotient $\mathbf{P}(V)$. Pour tout point $x = \sum_{i=0}^n \xi_i e_i$ de $V - \{0\}$, on dit que $(\xi_0, \xi_1, \ldots, \xi_n)$ est un système de coordonnées homogènes du point $\pi(x)$ par rapport à la base $(e_i)$ de V. Tout système $(\xi_i)$ de $n + 1$ éléments non tous nuls de K est donc un système de coordonnées homogènes d’un point de $\mathbf{P}(V)$ par rapport à $(e_i)$; pour que deux tels systèmes $(\xi_i), (\xi'_i)$ soient des systèmes de coordonnées homogènes d’un même point de $\mathbf{P}(V)$ par rapport à la même base $(e_i)$, il faut et il suffit qu’il existe un élément $\lambda \neq 0$ de K tel que $\xi'_i = \lambda \xi_i$ pour $0 \leq i \leq n$.

On généralise aussitôt cette définition au cas où V est de dimension infinie.

Étant donnée une seconde base $(\bar{e}_i)$ de V, telle que $e_i = \sum_{j=0}^n \alpha_{ij} \bar{e}_j$ ($0 \leq i \leq n$), et un système $(\xi_i)$ de coordonnées homogènes de $\pi(x)$ par rapport à la base $(e_i)$, pour qu’un système $(\bar{\xi}_i)$ de $n + 1$ éléments de K soit un système de coordonnées homogènes de $\pi(x)$ par rapport à la base $(\bar{e}_i)$, il faut et il suffit qu’il existe $\lambda \neq 0$ dans K, tel que l’on ait

$$
\lambda \bar{\xi}_i = \sum_{j=0}^n \xi_j \alpha_{ji} \quad \text{pour } 0 \leq i \leq n.
$$

En particulier, si $e_i = \gamma_i \bar{e}_i$, avec $\gamma_i \neq 0$ ($0 \leq i \leq n$), on a $\bar{\xi}_i = \mu \xi_i \gamma_i$, où $\mu \neq 0$.

### 7. Variétés linéaires projectives

Soit W un sous-espace vectoriel d’un espace vectoriel V; l’image canonique de $W - \{0\}$ dans l’espace projectif $\mathbf{P}(V)$ déduit de V, est appelée une variété linéaire projective (ou simplement une variété linéaire lorsque aucune confusion n’est à craindre); comme la relation d’équivalence $\Delta(W)$ dans $W - \{0\}$ est induite par la relation $\Delta(V)$, on peut identifier la variété linéaire projective image de $W - \{0\}$ dans $\mathbf{P}(V)$ avec l’espace projectif $\mathbf{P}(W)$ déduit de W, et parler par suite de la dimension d’une telle variété. Dans un espace projectif $\mathbf{P}(V)$, l’image canonique d’un hyperplan (privé de l’origine) de $V$ est une variété linéaire appelée *hyperplan projectif* (ou simplement *hyperplan*) ; si $\mathbf{P}(V)$ est de dimension finie $n$, les hyperplans dans $\mathbf{P}(V)$ sont les variétés linéaires de dimension $n - 1$.

Toute proposition relative aux sous-espaces vectoriels d’un espace vectoriel se traduit en une proposition relative aux variétés linéaires projectives. Par exemple, si un espace projectif $\mathbf{P}(V)$ est de dimension finie $n$, et si $(e_i)_{0 \leq i \leq n}$ est une base de $V$, toute variété linéaire $L \subset \mathbf{P}(V)$, de dimension $r$, peut être définie par un système de $n - r$ équations linéaires homogènes

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \quad (1 \leq j \leq n - r)
$$

entre les coordonnées homogènes $\xi_i$ ($0 \leq i \leq n$) d’un point de $\mathbf{P}(V)$ par rapport à la base $(e_i)$, les premiers membres de (4) étant des formes linéaires indépendantes sur $V$. En particulier, un hyperplan projectif est défini par une seule équation linéaire homogène à coefficients non tous nuls. Inversement, les points de $\mathbf{P}(V)$ satisfaisant à un système arbitraire d’équations linéaires et homogènes par rapport aux $\xi_i$ forment une variété linéaire $L$; si le système considéré se compose de $k \leq n + 1$ équations, $L$ est de dimension $\geq n - k$.

Toute intersection de variétés linéaires de $\mathbf{P}(V)$ est une variété linéaire; pour toute partie $A$ de $\mathbf{P}(V)$, il existe une plus petite variété linéaire $L$ contenant $A$; on dit que c’est la variété linéaire *engendrée par* $A$ ou que $A$ est un *système générateur* de $L$; si $W$ est le sous-espace vectoriel de $V$ engendré par $\pi^{-1}(A)$, on a $L = \mathbf{P}(W)$.

Si $L$ et $M$ sont deux variétés linéaires quelconques dans $\mathbf{P}(V)$, $N$ la variété linéaire engendrée par $L \cup M$, on a (II, p. 99, cor. 3)

$$
\dim L + \dim M = \dim(L \cap M) + \dim N.
$$

En particulier, si $\mathbf{P}(V)$ est de dimension finie et si $\dim L + \dim M \geq \dim \mathbf{P}(V)$, on déduit de (5) que $L \cap M$ n’est pas vide.

Soient $(x_i), (y_i)$ deux familles de points de l’espace vectoriel $V$ ayant même ensemble d’indices, telles que $y_i = \lambda_i x_i$, où $\lambda_i \neq 0$, pour tout $i$. Si la famille $(x_i)$ est libre, il en est de même de $(y_i)$, et réciproquement; on dit alors que la famille des points $\pi(x_i)$ de $\mathbf{P}(V)$ est *projectivement libre* (ou simplement *libre*). Il revient au même de dire que, pour tout indice $\kappa$, le point $\pi(x_\kappa)$ n’appartient pas à la variété linéaire engendrée par les $\pi(x_i)$ pour $i \neq \kappa$. Une famille de points de $\mathbf{P}(V)$ qui n’est pas projectivement libre est dite *projectivement liée* (ou simplement *liée*).

Pour qu’une famille $(x_i)$ de points de $V - \{0\}$ soit telle que la famille $(\pi(x_i))$ soit projectivement libre et engendre $\mathbf{P}(V)$, il faut et il suffit que $(x_i)$ soit une base de $V$. Si $\mathbf{P}(V)$ est de dimension $n$, le nombre d’éléments d’une telle famille est donc $n + 1$. On notera que la donnée d’une telle famille $(\pi(x_i))$ dans $\mathbf{P}(V)$ ne détermine pas (même à un facteur à gauche près) les coordonnées homogènes d’un point donné de $\mathbf{P}(V)$ par rapport à une base $(y_i)$ de V telle que $\pi(y_i) = \pi(x_i)$ pour tout $i$ (cf. II, p. 133).

### 8. Complétion projective d’un espace affine

Soit V un espace vectoriel (à gauche) sur un corps K, et considérons l’espace vectoriel $K_s \times V$ sur K ; on dit que l’espace projectif $\mathbf{P}(K_s \times V)$ est l’espace projectif canoniquement associé à l’espace vectoriel V. Si V est de dimension $n$, $\mathbf{P}(K_s \times V)$ est de même dimension $n$. Considérons, dans $K_s \times V$, l’hyperplan affine $V_1 = \{1\} \times V$, dont la direction (II, p. 129) est le sous-espace $V_0 = \{0\} \times V$; si une droite (passant par 0) de $K_s \times V$ n’est pas contenue dans $V_0$, elle contient un point $(\alpha, x)$ avec $\alpha \neq 0$ et $x \in V$, donc elle contient aussi le point $\alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x)$ de $V_1$; la réciproque est immédiate, et on voit qu’il y a correspondance biunivoque entre les points de $V_1$ et les droites (passant par 0) de $K_s \times V$ non contenues dans $V_0$, chacune de ces dernières rencontrant $V_1$ en un point et un seul. On en déduit que l’application $x \mapsto \varphi(x) = \pi(1, x)$ est une injection (dite canonique) de V dans l’espace projectif $\mathbf{P}(K_s \times V)$; on identifie souvent V à son image par cette injection. Le complémentaire de $\varphi(V)$ dans $\mathbf{P}(K_s \times V)$ est l’hyperplan projectif $\mathbf{P}(V_0)$, dit hyperplan à l’infini de $\mathbf{P}(K_s \times V)$ (ou de V, par abus de langage); ses points sont encore dits « points à l’infini » de $\mathbf{P}(K_s \times V)$ (ou de V). Si $(a_i)$ est une base de V, et si on prend pour $K_s \times V$ la base formée des éléments $e_i = (0, a_i)$ et de l’élément $e_\omega = (1, 0)$, les points à l’infini de $\mathbf{P}(K_s \times V)$ sont ceux dont la coordonnée homogène d’indice $\omega$ est 0.

Soient M une variété linéaire affine dans V (II, p. 128), D sa direction; l’image canonique $\varphi(M)$ de M dans $\mathbf{P}(K_s \times V)$ est contenue dans l’image canonique $\overline{M} = \pi(M_2)$ du sous-espace vectoriel $M_2$ de $K_s \times V$ engendré par la variété linéaire affine $M_1 = \{1\} \times M$ de $K_s \times V$. Plus précisément, si $(a_i)$ est un système affinement libre de M engendrant M, les éléments $(1, a_i)$ forment une base de $M_2$, et par suite $\overline{M}$ n’est autre que la variété linéaire projective engendrée par $\varphi(M)$; si M est de dimension finie, $\overline{M}$ a même dimension que M. Le complémentaire de $\varphi(M)$ dans $\overline{M}$ est l’intersection de $\overline{M}$ et de l’hyperplan à l’infini, et est égal à l’image canonique $\pi(M_0)$, où $M_0 = \{0\} \times D$.

Réciproquement, soit N une variété linéaire projective non contenue dans l’hyperplan à l’infini et soit $R = \pi^{-1}(N)$; $R \cap V_1$ est une variété linéaire affine de $K_s \times V$, de la forme $\{1\} \times M$, où M est une variété linéaire affine de V, et on voit aussitôt que N est la variété linéaire projective $\overline{M}$ engendrée par $\varphi(M)$.

Il y a donc correspondance biunivoque entre variétés linéaires affines de V et variétés linéaires projectives de $\mathbf{P}(K_s \times V)$ non contenues dans l’hyperplan à l’infini; pour que deux variétés linéaires affines de V soient parallèles, il faut et il suffit que les variétés linéaires projectives qu’elles engendrent aient même intersection avec l’hyperplan à l’infini (ce qu’on exprime parfois en disant que les deux variétés linéaires affines considérées ont mêmes points à l’infini).

### 9. Prolongement des fonctions rationnelles

Si on applique les résultats du n° 8 à l’espace vectoriel $V = K_s$, de dimension 1, on voit qu’il existe une injection canonique $\varphi$ de $K_s$ dans la droite projective $P_1(K) = P(K_s \times K_s)$; pour tout $\xi \in K$, $\varphi(\xi)$ est le point de coordonnées homogènes $(1, \xi)$ par rapport à la base canonique (II, p. 25) de $K_s \times K_s$. Le complémentaire de $\varphi(K)$ dans $P_1(K)$ est réduit au point de coordonnées homogènes $(0, 1)$ par rapport à la base précédente; on l’appelle le « point à l’infini ». On dit parfois que $P_1(K)$ est le corps projectif associé à $K$ et on le note $\tilde{K}$, le point à l’infini de $\tilde{K}$ étant noté $\infty$.

\* Considérons en particulier le cas où $K$ est un corps commutatif, et soit $f \in K(X)$ une fraction rationnelle à une indéterminée sur $K$ (IV, § 4); si $f \neq 0$, on peut écrire d’une seule manière $f = \alpha p/q$, où $\alpha \in K^*$ et $p$ et $q$ sont deux polynômes unitaires étrangers (VII, § 1); soient $m$ et $n$ leurs degrés respectifs, et posons $r = \sup(m, n)$. Posons $p_1(T, X) = \operatorname{Tr} p(X/T)$, $q_1(T, X) = \operatorname{Tr} q(X/T)$; $p_1$ et $q_1$ sont deux polynômes homogènes de degré $r$ sur $K$, tels que $p(X) = p_1(1, X)$, $q(X) = q_1(1, X)$. Cela étant, pour tout élément $\xi \in K$ qui n’est pas un zéro de $q(X)$, $f(\xi) = \alpha p(\xi)/q(\xi)$ est défini, et peut s’écrire

$$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$

pour tout $\lambda \neq 0$ dans $K$. Considérons alors l’application

$$
(\eta, \xi) \mapsto (q_1(\eta, \xi), \alpha p_1(\eta, \xi))
$$

de $K^2$ dans lui-même; elle est compatible avec la relation d’équivalence $\Delta(K^2)$ et définit par suite, par passage aux quotients, une application $\tilde{f}$ de $\tilde{K}$ dans lui-même, qui coïncide avec $\xi \mapsto f(\xi)$ aux points où cette fonction rationnelle est définie; on dit, par abus de langage, que $\tilde{f}$ est le prolongement canonique de $f$ à $\tilde{K}$.

Par exemple, si $f = 1/X$, on a $\tilde{f}(0) = \infty$ et $\tilde{f}(\infty) = 0$; si $f = (aX + b)/(cX + d)$ avec $ad - bc \neq 0$, on a $\tilde{f}(-d/c) = \infty$, $\tilde{f}(\infty) = a/c$ si $c \neq 0$, $\tilde{f}(\infty) = \infty$ si $c = 0$. Si $f = a_0 X^n + \cdots + a_n$ est un polynôme de degré $n > 0$, on a $\tilde{f}(\infty) = \infty$.*

### 10. Applications linéaires projectives

Soient $V, V'$ deux espaces vectoriels à gauche sur un corps $K$, $f$ une application linéaire de $V$ dans $V'$, $N = \overline{f}(0)$ son noyau. Il est immédiat que l’image par $f$ d’une droite (passant par 0) de $V$ non contenue dans $N$ est une droite (passant par 0) de $V'$; donc, par passage aux quotients, $f$ définit une application $g$ de $P(V) - P(N)$ dans $P(V')$. Une telle application est dite application linéaire projective (ou simplement application projective); bien qu’elle soit définie dans $P(V) - P(N)$ et non dans $P(V)$ tout entier (lorsque $N \neq \{0\}$), on dira par abus de langage que $g$ est une application projective de $P(V)$ dans $P(V')$. La variété linéaire projective $P(N)$, où $g$ n’est pas définie, est appelée le centre de $g$.

On notera que, lorsque $g$ est définie dans $\mathbf{P}(V)$ tout entier (c’est-à-dire lorsque $N = \{0\}$), $g$ est une injection de $\mathbf{P}(V)$ dans $\mathbf{P}(V')$.

Lorsqu’on s’est donné des bases $(a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M}$ dans $V$ et $V'$ respectivement, une application projective de $\mathbf{P}(V)$ dans $\mathbf{P}(V')$ fait correspondre à un point de $\mathbf{P}(V)$ de coordonnées homogènes $\xi_\lambda \ (\lambda \in L)$ un point de $\mathbf{P}(V')$ admettant un système de coordonnées homogènes $\eta_\mu \ (\mu \in M)$ de la forme

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

Le centre de $g$ est la variété linéaire définie par les équations

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

Si $C$ est le centre de $g$, et $M$ une variété linéaire de $\mathbf{P}(V)$, l’image par $g$ de $M - (M \cap C)$ est une variété linéaire de $\mathbf{P}(V')$, que l’on désigne (par abus de langage) par $g(M)$. On a

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

(II, p. 101, formule (12)). Si $M'$ est une variété linéaire de $\mathbf{P}(V')$, $\overline{g}^1(M') \cup C$ est une variété linéaire de $\mathbf{P}(V)$, et on a

$$
\dim(\overline{g}^1(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

On dit, par abus de langage, que $\overline{g}^1(M') \cup C$ est l’image réciproque de $M'$ par $g$.

Comme les valeurs prises par une application linéaire sur une base $(e_i)$ de $V$ peuvent être choisies arbitrairement dans $V'$, on voit qu’il existe une application projective de $\mathbf{P}(V)$ dans $\mathbf{P}(V')$ prenant des valeurs arbitraires aux points $\pi(e_i)$. Mais (même lorsque $g$ est partout définie) la donnée des éléments $g(\pi(e_i))$ ne détermine pas $g$ de façon unique (II, p. 202, exerc. 10).

La composée de deux applications projectives qui sont des bijections est une application projective; il en est de même de l’application réciproque d’une telle bijection. Les applications projectives bijectives d’un espace projectif $\mathbf{P}(V)$ sur lui-même forment donc un groupe, appelé groupe projectif de $\mathbf{P}(V)$, et noté $\mathbf{PGL}(V)$; on écrit $\mathbf{PGL}_n(K)$ ou $\mathbf{PGL}(n, K)$ au lieu de $\mathbf{PGL}(K_s^n)$.

#### Remarque {#alg-ii-s9-n10-rem-1 .statement}

Dans un espace projectif $\mathbf{P}(V)$ sur un corps $K$, soit $H = \mathbf{P}(W)$ un hyperplan. Il existe une application linéaire bijective $f$ de $V$ sur $K_s \times W$ telle que $f(W) = W$; soit $g$ l’application projective obtenue à partir de $f$ par passage aux quotients. On a vu (II, p. 135) qu’on peut identifier le complémentaire de $\mathbf{P}(W)$ dans $\mathbf{P}(K_s \times W)$ à un espace affine, dont $W$ est l’espace des translations. Lorsqu’on identifie $\mathbf{P}(V)$ à $\mathbf{P}(K_s \times W)$ au moyen de $g$, on dit qu’on a pris $H$ pour hyperplan à l’infini dans $\mathbf{P}(V)$; le complémentaire de $H$ dans $\mathbf{P}(V)$ est alors identifié à un espace affine dont $W$ est l’espace des translations.

### 11. Structure d’espace projectif

Étant donnés un ensemble E et un corps K, une structure d’espace projectif (à gauche) sur E, par rapport au corps K, est définie par la donnée d’un ensemble non vide Φ de bijections de parties de l’espace projectif $\mathbf{P}(K_s^{(E)})$ sur E, satisfaisant aux axiomes suivants:

(EP_I) L’ensemble de définition de toute application $f \in \Phi$ est une variété linéaire de $\mathbf{P}(K_s^{(E)})$.

(EP_{II}) Pour tout couple d’éléments $f, g$ de $\Phi$, définis respectivement dans les variétés linéaires $\mathbf{P}(V)$ et $\mathbf{P}(W)$, la bijection $h = g^{-1} \circ f$ de $\mathbf{P}(V)$ sur $\mathbf{P}(W)$ est une application projective.

(EP_{III}) Inversement, si $f \in \Phi$ est définie dans la variété linéaire $\mathbf{P}(V)$, et si $h$ est une application projective bijective de $\mathbf{P}(V)$ sur une variété linéaire $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, on a $f \circ h^{-1} \in \Phi$.

Soient E un ensemble, $(V_\lambda)_{\lambda \in L}$ une famille d’espaces vectoriels sur K, et supposons donnée pour chaque $\lambda \in L$ une bijection $f_\lambda$ de $\mathbf{P}(V_\lambda)$ sur E, telle que, pour tout couple d’indices $\lambda, \mu, f_\lambda^{-1} \circ f_\mu$ soit une application projective de $\mathbf{P}(V_\mu)$ sur $\mathbf{P}(V_\lambda)$. On peut alors définir sur E une structure d’espace projectif par rapport à K, de la façon suivante: soit $(e_i)_{i \in I}$ une base d’un espace $V_\lambda$ et posons $a_i = f_\lambda(\pi(e_i))$; soit $b_i$ l’élément d’indice $a_i$ dans la base canonique de $K_s^{(E)}$ (II, p. 25). La relation $i \neq \kappa$ entraîne $b_i \neq b_\kappa$ en vertu de l’hypothèse que $f_\lambda$ est bijective; donc les $b_i$ forment une base d’un sous-espace vectoriel $W_0$ de $K_s^{(E)}$, et il existe par suite une application projective bijective $h$ de $\mathbf{P}(W_0)$ sur $\mathbf{P}(V_\lambda)$ telle que $h(\pi(b_i)) = \pi(e_i)$ pour tout $i \in I$. Si on prend pour $\Phi$ l’ensemble de toutes les applications $f_\lambda \circ h \circ g^{-1}$, où $g$ parcourt l’ensemble de toutes les applications projectives bijectives de $\mathbf{P}(W_0)$ sur des variétés linéaires $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, on vérifie aussitôt que $\Phi$ satisfait aux axiomes (EP_I), (EP_{II}) et (EP_{III}). Il est immédiat en outre que $\Phi$ ne dépend, ni du choix de l’indice $\lambda \in L$, ni du choix d’une base $(e_i)$ dans $V_\lambda$, ni du choix de $h$.

En particulier (en prenant L réduit à un seul élément), tout espace projectif $\mathbf{P}(V)$ déduit d’un espace vectoriel V (II, p. 132, déf. 4) est ainsi muni d’une « structure d’espace projectif » bien déterminée, au sens de la définition donnée dans ce n°. On peut donc appeler espace projectif tout ensemble muni d’une structure d’espace projectif.

Les notations restant les mêmes, une variété linéaire dans l’espace projectif E est une partie M de E telle que, pour une bijection $f \in \Phi$ au moins, définie dans $\mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)})$, $\overline{f^{-1}}(M)$ soit une variété linéaire dans $\mathbf{P}(V)$ au sens de II, p. 133 (cette propriété est alors vérifiée pour toute $f \in \Phi$). Il résulte de ce qui précède que toute variété linéaire dans un espace projectif est canoniquement munie d’un structure d’espace projectif.

On dit que l’espace projectif E est de dimension n si, pour toute $f \in \Phi$, $\overline{f^{-1}}(E)$ est une variété linéaire de dimension n (il suffit que cela soit vérifié pour une application $f \in \Phi$).

## EXERCICES {#alg-ii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
