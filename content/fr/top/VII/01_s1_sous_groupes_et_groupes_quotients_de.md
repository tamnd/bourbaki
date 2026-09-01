---
book: top
book_title: General Topology
chapter: VII
chapter_title: LES GROUPES ADDITIFS $\mathbf{R}^n$
section: 1
section_title: Sous-groupes et groupes quotients de $\mathbf{R}^n$
lang: fr
source: top-v-x-fr
pdf_pages: 0059-0069, 0077-0081
extraction: ocr
subsections:
    - "no": 1
      title: Sous-groupes discrets de $\mathbf{R}^n$
      page: 2
      pdf_page: 60
    - "no": 2
      title: Sous-groupes fermés de $\mathbf{R}^n$
      page: 4
      pdf_page: 62
    - "no": 3
      title: Sous-groupes associés
      page: 6
      pdf_page: 64
    - "no": 4
      title: Groupes quotients séparés de $\mathbf{R}^n$
      page: 8
      pdf_page: 66
    - "no": 5
      title: Sous-groupes et groupes quotients de $T^n$
      page: 9
      pdf_page: 67
    - "no": 6
      title: Fonctions périodiques
      page: 10
      pdf_page: 68
statements: 21
exercises: 18
content_sha256: f38793db3a278473815b0d0ed17a01360b4d00a057d0a76b992dcf699f875c0f
---

## § 1. SOUS-GROUPES ET GROUPES QUOTIENTS DE $\mathbf{R}^n$

Sur l’ensemble $\mathbf{R}^n$, nous aurons à considérer, dans ce paragraphe, d’une part sa structure de groupe *topologique* (additif), d’autre part sa structure d’*espace vectoriel* par rapport au corps $\mathbf{R}$ (VI, p. 2). Étant donnée une partie A de $\mathbf{R}^n$, nous envisagerons, tantôt le *sous-groupe* de $\mathbf{R}^n$ engendré par A (ensemble des combinaisons linéaires de points de A, à coefficients *entiers*), tantôt le *sous-espace vectoriel* engendré par A (ensemble des combinaisons linéaires de points de A, à coefficients *réels*) ; on aura soin de ne pas confondre ces deux notions. Conformément aux définitions données en Algèbre (A, II, p. 97), nous appellerons *rang* de A la *dimension* du sous-espace vectoriel V engendré par A ; dire que A est de rang $p$ équivaut donc à dire qu’il existe $p$ points $\mathbf{x}_i \in A$, formant un *système libre* par rapport au corps $\mathbf{R}$ (autrement dit, la relation $\sum_i t_i \mathbf{x}_i = 0$, où les $t_i$ sont *réels*, entraîne $t_i = 0$ pour tout $i$), et engendrant le $\mathbf{R}$-espace vectoriel V (ce qui veut dire que tout point de V est combinaison linéaire à coefficients réels des $\mathbf{x}_i$).

Dans ce qui suit interviendra aussi la notion de système de points de $\mathbf{R}^n$ *libre par rapport au corps* $\mathbf{Q}$ *des nombres rationnels* ; un tel système est une partie finie $(\mathbf{x}_i)$ de $\mathbf{R}^n$ telle que la relation $\sum_i r_i \mathbf{x}_i = 0$, où les $r_i$ sont *rationnels* (ou *entiers*, ce qui revient au même), entraîne $r_i = 0$ pour tout $i$. On aura soin de ne pas confondre cette notion et celle de système libre par rapport à $\mathbf{R}$; tout système libre par rapport à $\mathbf{R}$ est libre par rapport à $\mathbf{Q}$, mais la réciproque est inexacte ; par exemple, les nombres 1 et $\sqrt{2}$ forment dans $\mathbf{R}$ un système libre par rapport à $\mathbf{Q}$, mais non un système libre par rapport à $\mathbf{R}$; lorsque nous parlerons de *système libre* sans préciser, il s’agira toujours de système libre *par rapport à* $\mathbf{R}$. Il faut donc bien distinguer, sur $\mathbf{R}^n$, la structure d’espace vectoriel *par rapport à* $\mathbf{R}$ de la structure d’espace vectoriel *par rapport à* $\mathbf{Q}$; en particulier, le sous-espace vectoriel *par rapport à* $\mathbf{Q}$ engendré par une partie A de $\mathbf{R}^n$, est l’ensemble U des combinaisons linéaires de points de $A$, à coefficients rationnels; il est contenu dans le sous-espace vectoriel $V$ (par rapport à $\mathbf{R}$) engendré par $A$, mais en est en général distinct. La dimension de $U$ (*par rapport à* $\mathbf{Q}$) est appelé le *rang rationnel* de $A$; il est *au moins égal au rang* de $A$ défini ci-dessus (dimension de $V$ par rapport à $\mathbf{R}$); il peut être *infini* si $A$ est un ensemble infini, alors que le rang d’une partie non vide de $\mathbf{R}^n$ est toujours $\leq n$; en particulier, le rang rationnel d’une partie *non dénombrable* de $\mathbf{R}^n$ est toujours infini, puisqu’un espace vectoriel de dimension finie sur le corps $\mathbf{Q}$ est dénombrable.

Nous allons, dans ce paragraphe, déterminer tout d’abord la structure des *sous-groupes fermés* du groupe additif $\mathbf{R}^n$.

### 1. Sous-groupes discrets de $\mathbf{R}^n$

On a vu (V, p. 1, prop. 1) que les seuls sous-groupes fermés de $\mathbf{R}$, distincts de $\mathbf{R}$, sont les sous-groupes *discrets* de $\mathbf{R}$, engendrés par *un seul* élément. Nous allons commencer par étudier les sous-groupes *discrets* de $\mathbf{R}^n$.

Tout d’abord, le sous-groupe de $\mathbf{R}^n$ engendré par $p$ vecteurs ($p \leq n$) de la base canonique (VI, p. 3) de $\mathbf{R}^n$, est un groupe discret isomorphe au groupe produit $\mathbf{Z}^p$ de $p$ groupes identiques à $\mathbf{Z}$. Plus généralement, considérons le sous-groupe $G$ engendré par $p$ points $a_i$ ($1 \leq i \leq p$) formant un système *libre*; il existe une application linéaire bijective de $\mathbf{R}^n$ sur lui-même transformant $a_i$ en $e_i$ ($1 \leq i \leq p$); une telle application étant un automorphisme du groupe topologique $\mathbf{R}^n$, $G$ est un groupe topologique isomorphe au sous-groupe engendré par les $e_i$ ($1 \leq i \leq p$), et c’est par suite un sous-groupe *discret* de rang $p$ isomorphe à $\mathbf{Z}^p$.

La structure du groupe $\mathbf{Z}^p$, et par suite du groupe $G$, a été étudiée en Algèbre (A, VII, §§ 3 et 4); rappelons les principaux résultats de cette étude. Les *bases* de $G$ par rapport à l’anneau $\mathbf{Z}$ sont les systèmes de $p$ points $b_i = \sum_{j=1}^p r_{ij} a_j$, où les $r_{ij}$ sont des entiers tels que le déterminant $\det(r_{ij})$ soit égal à $+1$ ou à $-1$. Tout *sous-groupe* $H$ de $G$ est discret et de rang $q \leq p$; en outre, pour un sous-groupe donné $H$ de rang $q$, il existe un système libre de $p$ points $b_i$ ($1 \leq i \leq p$) engendrant $G$, et un système de $q$ points $c_i$ ($1 \leq i \leq q$) engendrant $H$, tels que, pour $1 \leq i \leq q$, on ait $c_i = e_i b_i$, où les $e_i$ sont des entiers (les *facteurs invariants* de $H$ par rapport à $G$) tels que $e_{i+1} \equiv 0$ (mod. $e_i$) pour $1 \leq i \leq q-1$. Le groupe quotient $G/H$ est un groupe discret, isomorphe au produit $\mathbf{Z}^{p-q} \times F$, où $F$ est un groupe abélien *fini*, produit direct de $q$ groupes cycliques d’ordres respectifs $\ell_1, \ell_2, \ldots, \ell_q$.

Nous allons maintenant montrer que les sous-groupes discrets de $\mathbf{R}^n$ que nous venons de considérer sont les *seuls*.

#### Proposition 1 {#top-vii-s1-prop-1 .statement}

*Soient* $G$ *un sous-groupe discret de* $\mathbf{R}^n$, *de rang* $p$, $(a_i)_{1 \leq i \leq p}$ *un système libre de* $p$ *points de* $G$, $P$ *le parallélétope fermé de centre* $0$, *construit sur les vecteurs* $a_i$ (VI, p. 3); alors l’ensemble $G \cap P$ est fini et engendre $G$, et tout point de $G$ est une combinaison linéaire des $a_i$ à coefficients rationnels.

En effet, $G \cap P$ est compact et discret, donc fini. Soit $x$ un point quelconque de $G$; il est égal à une combinaison linéaire $\sum_{i=1}^p t_i a_i$ à coefficients réels des $a_i$. Pour tout entier $m > 0$, considérons le point

$$
z_m = m x - \sum_{i=1}^p [m t_i] a_i = \sum_{i=1}^p (m t_i - [m t_i]) a_i^1;
$$

il appartient à $G$, et comme $0 \leq m t_i - [m t_i] < 1$, il est contenu dans $P$. On en déduit tout d’abord que $x = z_1 + \sum_{i=1}^p [t_i] a_i$, donc $G$ est engendré par $G \cap P$. D’autre part, comme $G \cap P$ est fini, il existe deux entiers distincts $h, k$ tels que $z_h = z_k$, ce qui entraîne $(h - k) t_i = [h t_i] - [k t_i]$ pour $1 \leq i \leq p$; donc les $t_i$ sont rationnels.

#### Corollaire {#top-vii-s1-n1-cor-1 .statement}

Soient $(a_i)_{1 \leq i \leq p}$ un système libre de $p$ points de $\mathbf{R}^n$ et $b = \sum_{i=1}^p t_i a_i$ une combinaison linéaire à coefficients réels des $a_i$. Pour que le sous-groupe $G$ de $\mathbf{R}^n$ engendré par les $p + 1$ points $a_i$ ($1 \leq i \leq p$) et $b$ soit discret, il faut et il suffit que les nombres $t_i$ soient rationnels.

La prop. 1 montre que la condition est nécessaire. Elle est suffisante, car si elle est remplie, on peut écrire $t_i = m_i / d$, où $d$ et les $m_i$ sont entiers ($1 \leq i \leq p$); $b$ est donc combinaison linéaire à coefficients entiers des $p$ points $(1/d) a_i$, d’où résulte que $G$ est un sous-groupe du groupe discret engendré par ces $p$ points, et par suite est lui-même discret.

On peut encore exprimer le résultat de la prop. 1 de la façon suivante: si $q$ points $x_i$ ($1 \leq i \leq q$) d’un sous-groupe discret $G$ de $\mathbf{R}^n$ forment un système lié par rapport à $\mathbf{R}$, ils forment aussi un système lié par rapport à $\mathbf{Q}$. On en conclut aussitôt que le rang rationnel d’un sous-groupe discret de $\mathbf{R}^n$ est égal à son rang.

Le corollaire de la prop. 1, appliqué au cas où les $a_i$ sont les $n$ vecteurs $e_i$ de la base canonique, donne la proposition suivante:

#### Proposition 2 (Kronecker) {#top-vii-s1-prop-2 .statement}

Soient $\theta_1, \theta_2, \ldots, \theta_n$ des nombres réels. Les conditions suivantes sont équivalentes:
a) pour tout $\varepsilon > 0$, il existe un entier $q$ et $n$ entiers $p_i$ ($1 \leq i \leq n$) tels que
$$
|q \theta_i - p_i| \leq \varepsilon \quad \text{pour } 1 \leq i \leq n,
$$
un au moins des premiers membres de ces inégalités n’étant pas nul;
b) l’un au moins des $\theta_i$ est irrationnel.

1 On rappelle (IV, p. 41) que pour tout nombre réel $x$, $[x]$ est la partie entière de $x$, c’est-à-dire le plus grand entier rationnel qui soit $\leq x$.

#### Théorème 1 {#top-vii-s1-thm-1 .statement}

*Tout sous-groupe discret* G de $\mathbf{R}^n$, de rang égal à p, est engendré par un système libre de p points.

D’après les propriétés des groupes isomorphes à $\mathbf{Z}^p$ rappelées plus haut, il suffira de montrer que G est *sous-groupe* d’un groupe discret engendré par un système libre de p points. Or, comme G est de rang p, il existe un système libre de p points $\mathbf{a}_i$ ($1 \leq i \leq p$) de G tel que tout $\mathbf{x} \in G$ soit égal à une combinaison linéaire $\sum_{i=1}^p t_i \mathbf{a}_i$ à coefficients réels des $\mathbf{a}_i$; G étant discret, la prop. 1 (VII, p. 2) montre que les $t_i$ sont *rationnels* et que G est engendré par un nombre *fini* de points; ces points étant combinaisons linéaires des $\mathbf{a}_i$ à coefficients rationnels, il existe un entier d tel qu’ils soient combinaisons linéaires à coefficients *entiers* des p points $(1/d)\mathbf{a}_i = \mathbf{a}'_i$; il en résulte que G est un sous-groupe du groupe engendré par les $\mathbf{a}'_i$.

On peut démontrer le th. 1 sans faire appel à la théorie des facteurs invariants (cf. VII, p. 19, exerc. 1).
Les sous-groupes discrets de $\mathbf{R}^n$ qui sont de rang n sont encore appelés des *réseaux* dans $\mathbf{R}^n$.

### 2. Sous-groupes fermés de $\mathbf{R}^n$

Nous connaissons déjà deux sortes de sous-groupes fermés de $\mathbf{R}^n$; d’une part, les *sous-espaces vectoriels de* $\mathbf{R}^n$, qui sont isomorphes aux groupes $\mathbf{R}^p$ ($p \leq n$); d’autre part, les sous-groupes *discrets* (III, p. 7, prop. 5), qui sont isomorphes aux groupes $\mathbf{Z}^q$ ($q \leq n$) comme nous venons de le voir. Nous allons déterminer la structure d’un sous-groupe fermé *quelconque* de $\mathbf{R}^n$ en montrant qu’un tel sous-groupe est isomorphe à un *produit* de la forme $\mathbf{R}^p \times \mathbf{Z}^q$ ($0 \leq p + q \leq n$).

Nous nous appuierons sur la proposition suivante:

#### Proposition 3 {#top-vii-s1-prop-3 .statement}

*Tout sous-groupe fermé non discret de* $\mathbf{R}^n$ *contient une droite passant par* 0.

En effet, soit $(\mathbf{x}_p)_{p \in \mathbf{N}}$ une suite infinie de points de G, tels que $\mathbf{x}_p \neq 0$ et $\lim_{p \to \infty} \mathbf{x}_p = 0$; une telle suite existe d’après l’hypothèse. Soit P un cube ouvert de centre 0 contenant les $\mathbf{x}_p$. Désignons par $k_p$ le plus grand les entiers $h > 0$ tels que $h \mathbf{x}_p \in P$ (comme P est un pavé borné et $\mathbf{x}_p \neq 0$, l’existence de $k_p$ résulte de l’axiome d’Archimède). Les points $k_p \mathbf{x}_p$ appartiennent à l’ensemble compact $\overline{P}$; la suite $(k_p \mathbf{x}_p)_{p \in \mathbf{N}}$ a donc une valeur d’adhérence $\mathbf{a} \in \overline{P}$. D’ailleurs, si $\|k_p \mathbf{x}_p - \mathbf{a}\| \leq \varepsilon$, on a $\|(k_p + 1) \mathbf{x}_p - \mathbf{a}\| \leq \varepsilon + \|\mathbf{x}_p\|$, et comme $\lim_{p \to \infty} \mathbf{x}_p = 0$, $\mathbf{a}$ est aussi valeur d’adhérence de la suite $((k_p + 1) \mathbf{x}_p)$, dont les points appartiennent à l’ensemble fermé $\mathcal{C} P$, d’après la définition de $k_p$; on a donc $\mathbf{a} \in \overline{P} \cap \mathcal{C} P$ (frontière de P, fig. 5), ce qui entraîne $\mathbf{a} \neq 0$; en outre, comme G est fermé, $\mathbf{a} \in G$. Soit alors t un nombre réel quelconque; comme $|t k_p - [t k_p]| < 1$ la relation $\|k_p x_p - a\| \leq \varepsilon$ entraîne $\|[(tk_p)x_p - ta\| \leq |t|\varepsilon + \|x_p\|$; comme $\lim_{p \to \infty} x_p = 0$, $ta$ est valeur d’adhérence de la suite $[tk_p]x_p$; les points de cette suite appartenant à $G$, on a $ta \in G$, puisque $G$ est fermé. La proposition est ainsi démontrée.

![Figure 5](https://i.imgur.com/5zXzX.png)
Figure 5

![Figure 6](https://i.imgur.com/5zXzX.png)
Figure 6

#### Théorème 2 {#top-vii-s1-thm-2 .statement}

*Soit $G$ un sous-groupe fermé de $\mathbf{R}^n$, de rang $r$ ($0 \leq r \leq n$); il existe un plus grand sous-espace vectoriel $V$ contenu dans $G$; pour tout espace vectoriel $W$ supplémentaire de $V$, $W \cap G$ est discret, et $G$ est somme directe de $V$ et de $W \cap G$.*

Démontrons d’abord l’existence de $V$ en prouvant que la réunion des droites contenues dans $G$ et passant par $0$ est un sous-espace vectoriel: en effet, le sous-espace vectoriel engendré par la réunion de ces droites est identique au sous-groupe engendré par cette réunion. Le groupe $G$ est *somme directe* de $V$ et de $W \cap G$, car pour tout $x \in G$, on a $x = y + z$, avec $y \in V$, $z \in W$; comme $V \subset G$, on a $z = x - y \in G$, donc $z \in W \cap G$. Reste à prouver que $W \cap G$ est *discret*; cela résulte de la prop. 3 (VII, p. 4), car $W \cap G$ est un sous-groupe fermé, et ne contient aucune droite, en vertu de la définition de $V$.

D’une manière imagée, lorsque $G \neq V$, on peut dire que $G$ est la réunion d’une infinité dénombrable de variétés linéaires *parallèles à* $V$, passant par les points du groupe discret $W \cap G$ (fig. 6).

Si $p$ est la dimension du sous-espace vectoriel $V$, on a $p \leq r$, et $W \cap G$ est un sous-groupe discret de rang $r - p$.

#### Corollaire 1 {#top-vii-s1-thm-2-cor-1 .statement}

*Il existe une base $(a_i)_{1 \leq i \leq n}$ de $\mathbf{R}^n$, telle que $a_i \in G$ pour $1 \leq i \leq r$, $a_i \in V$ pour $1 \leq i \leq p$, et que $G$ soit identique à l’ensemble des points*
$$
\sum_{i=1}^{p} t_i a_i + \sum_{j=p+1}^{r} n_j a_j,
$$
*où les $t_i$ prennent toutes les valeurs réelles, les $n_j$ toutes les valeurs entières.*
Cela résulte du th. 2, et du th. 1 de VII, p. 4 appliqué au groupe discret $W \cap G$.

#### Corollaire 2 {#top-vii-s1-thm-2-cor-2 .statement}

Il existe un automorphisme de $\mathbf{R}^n$ qui applique $G$ sur le groupe $G'$, isomorphe à $\mathbf{R}^p \times \mathbf{Z}^{r-p}$, somme directe du sous-espace vectoriel engendré par $e_1, e_2, \ldots, e_p$ et du sous-groupe additif (discret) engendré par $e_{p+1}, e_{p+2}, \ldots, e_r$.

C’est une conséquence immédiate du cor. 1.

Le cor. 2 du th. 2 montre qu’un sous-groupe fermé $G$ de $\mathbf{R}^n$ est entièrement déterminé, à isomorphisme près, par la donnée de deux entiers $\geqslant 0$: son rang que nous noterons $r(G)$, et la dimension du plus grand sous-espace vectoriel contenu dans $G$, nombre que nous noterons $d(G)$ et appellerons *dimension* du sous-groupe $G$; les seules conditions que doivent remplir ces deux entiers sont les inégalités $0 \leqslant d(G) \leqslant r(G) \leqslant n$.

### 3. Sous-groupes associés

Soit $G$ un sous-groupe quelconque (fermé ou non) de $\mathbf{R}^n$. Considérons l’ensemble $G^*$ des points $u = (u_i)$ de $\mathbf{R}^n$ tels que, pour *tout* point $x = (x_i) \in G$, le nombre $(u \mid x) = \sum_{i=1}^n u_i x_i$ soit un *entier*. Il est immédiat que $G^*$ est un *sous-groupe* de $\mathbf{R}^n$; on dit que c’est le sous-groupe *associé* à $G$. Si $G$ et $H$ sont deux sous-groupes de $\mathbf{R}^n$ tels que $H \subset G$, il est clair que $G^* \subset H^*$.

#### Proposition 4 {#top-vii-s1-prop-4 .statement}

*Le sous-groupe* $G^*$ *associé à un sous-groupe* $G$ *de* $\mathbf{R}^n$ *est fermé*, et on a $(\overline{G})^* = G^*$.

En effet, si pour tout $x \in G$, on pose $f_x(u) = (u \mid x)$, $f_x$ est une forme linéaire, donc continue; comme $G^*$ est l’intersection des ensembles $f_x^{-1}(\mathbf{Z})$ lorsque $x$ parcourt $G$, et que chacun de ces ensembles est fermé, $G^*$ est fermé. D’autre part, si $u \in G^*$, on a $(u \mid x) \in \mathbf{Z}$ pour tout $x \in G$, donc, puisque $\mathbf{Z}$ est fermé dans $\mathbf{R}$, $(u \mid y) \in \mathbf{Z}$ pour tout point $y$ adhérent à $G$; autrement dit, $u \in (\overline{G})^*$; comme d’autre part $(\overline{G})^* \subset G^*$, on a $(\overline{G})^* = G^*$.

Étudions la structure de $G^*$ lorsque $G$ est *fermé*. D’après VII, p. 5, cor. 1, il existe une base $(a_i)_{1 \leqslant i \leqslant n}$ de $\mathbf{R}^n$, telle que $G$ soit identique à l’ensemble des points $x = \sum_{i=1}^p t_i a_i + \sum_{j=p+1}^{p+q} n_j a_j$, où les $t_i$ prennent toutes les valeurs réelles, les $n_j$ toutes les valeurs entières. Pour que $(u \mid x)$ soit entier pour *tous* ces points $x$, il faut et il suffit que $(u \mid a_i) = 0$ pour $1 \leqslant i \leqslant p$, et que $(u \mid a_i)$ soit entier pour $p+1 \leqslant i \leqslant p+q$. Désignons par $(a'_i)_{1 \leqslant i \leqslant n}$ la base de $\mathbf{R}^n$ telle que $(a'_i \mid a_j) = 0$ pour $i \neq j$, $(a'_i \mid a_i) = 1$ pour tout $i$ (A, IX, §1, n° 6); si l’on pose $u = \sum_{i=1}^n u_i a_i$, on voit que les points $u \in G^*$ sont caractérisés par les conditions: $u_i = 0$ pour $1 \leqslant i \leqslant p$, et $u$ entier pour $p+1 \leqslant i \leqslant p+q$; donc $G^*$ est somme directe du sous-espace vectoriel $W$ ayant pour base les $a'_i$ d’indice tel que $p+q+1 \leqslant i \leqslant n$, et du sous-groupe discret engendré par les $a'_i$ d’indice tel que $p+1 \leqslant i \leqslant p+q$.

Autrement dit:
**Proposition 5.** — *Pour tout sous-groupe fermé G de $\mathbf{R}^n$, on a $r(G^*) = n - d(G)$, et $d(G^*) = n - r(G)$.*

Appliquons le même raisonnement à $G^*$; en remarquant que la base duale de $(\mathbf{a}_i')$ est $(\mathbf{a}_i)$, on voit que:

#### Proposition 6 {#top-vii-s1-prop-6 .statement}

*Pour tout sous-groupe G de $\mathbf{R}^n$, on a $(G^*)^* = \overline{G}$.*

#### Corollaire {#top-vii-s1-n3-cor-1 .statement}

*Pour qu’un point $\mathbf{x}$ soit adhérent à un sous-groupe G de $\mathbf{R}^n$, il faut et il suffit que $(\mathbf{u} \mid \mathbf{x})$ soit entier pour tout $\mathbf{u} \in \mathbf{R}^n$ tel que $(\mathbf{u} \mid \mathbf{y})$ soit entier pour tout $\mathbf{y} \in G$.*

Appliquons cette caractérisation des points adhérents à un sous-groupe G, au cas du sous-groupe G engendré par les $n$ vecteurs $\mathbf{e}_j$ de la base canonique $(1 \leq j \leq n)$, et par un nombre quelconque $m$ de points $\mathbf{a}_i$ $(1 \leq i \leq m)$ de $\mathbf{R}^n$. Dire que $(\mathbf{u} \mid \mathbf{e}_j)$ est entier pour $1 \leq j \leq n$ signifie que les $n$ coordonnées de $\mathbf{u}$ sont entières; donc:

**Proposition 7 (Kronecker).** — *Soient $\mathbf{a}_i = (a_{ji})$ $(1 \leq i \leq m, 1 \leq j \leq n)$ m points de $\mathbf{R}^n$, $\mathbf{b} = (b_j)$ $(1 \leq j \leq n)$ un point de $\mathbf{R}^n$. Afin que, pour tout $\varepsilon > 0$, il existe m entiers $q_i$ $(1 \leq i \leq m)$ et n entiers $p_j$ $(1 \leq j \leq n)$ tels que*
$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - b_j| \leq \varepsilon \quad \text{pour } 1 \leq j \leq n,
$$
*il faut et il suffit que, pour toute suite finie $(r_j)$ $(1 \leq j \leq n)$ de n entiers telle que les m nombres $\sum_{j=1}^n a_{ij} r_j$ $(1 \leq i \leq m)$ soient tous entiers, le nombre $\sum_{j=1}^n b_j r_j$ soit aussi entier.*

#### Corollaire 1 {#top-vii-s1-prop-6-cor-1 .statement}

*Afin que, pour tout $\mathbf{x} = (x_j)$ $(1 \leq j \leq n)$ et tout $\varepsilon > 0$, il existe m entiers $q_i$ $(1 \leq i \leq m)$ et n entiers $p_j$ $(1 \leq j \leq n)$ tels que*
$$
|q_1 a_{1j} + q_2 a_{2j} + \cdots + q_m a_{mj} - p_j - x_j| \leq \varepsilon \quad \text{pour } 1 \leq j \leq n,
$$
*il faut et il suffit qu’il n’existe aucune suite finie $(r_j)$ de n entiers non tous nuls, telle que chacun des m nombres $\sum_{j=1}^n a_{ij} r_j$ soit entier.*

En effet, si G est dense dans $\mathbf{R}^n$, c’est-à-dire si $\overline{G} = \mathbf{R}^n$, $G^*$ est réduit à 0, et réciproquement.

En particulier, pour $m = 1$:

#### Corollaire 2 {#top-vii-s1-prop-6-cor-2 .statement}

*Soient $\theta_1, \theta_2, \ldots, \theta_n$ n nombres réels. Afin que, quels que soient les n nombres réels $x_1, x_2, \ldots, x_n$ et le nombre $\varepsilon > 0$, il existe un entier q et n entiers $p_j$ tels que*
$$
|q \theta_j - p_j - x_j| \leq \varepsilon \quad \text{pour } 1 \leq j \leq n,
$$
*il faut et il suffit qu’il n’existe aucune relation de la forme $\sum_{j=1}^n r_j \theta_j = h$, où les $r_j$ sont n entiers non tous nuls, et h un entier (condition qui entraîne, en particulier, que les $\theta_j$, ainsi que les rapports $\theta_j / \theta_k$ pour $j \neq k$, doivent être *irrationnels*).*

On peut interpréter ce résultat de la façon suivante: pour tout entier $q \in \mathbf{Z}$, désignons par $\mathbf{x}_q$ le point de coordonnées $q\theta_j - [q\theta_j]$ ($1 \leq j \leq n$); alors le cor. 2 donne une condition nécessaire et suffisante pour que l’ensemble des $\mathbf{x}_q$ soit dense dans le cube produit des intervalles $(0, 1)$ des espaces facteurs de $\mathbf{R}^n$.

#### Proposition 8 {#top-vii-s1-prop-8 .statement}

*Quels que soient les sous-groupes fermés* $G_1, G_2$ de $\mathbf{R}^n$, *on a*
$$
(G_1 + G_2)^* = G_1^* \cap G_2^*,
$$
*et*
$$
(G_1 \cap G_2)^* = \overline{G_1^* + G_2^*}.
$$

En effet, pour que $(\mathbf{u} \mid \mathbf{x} + \mathbf{y})$ soit entier quels que soient $\mathbf{x} \in G_1$ et $\mathbf{y} \in G_2$, il faut et il suffit que $(\mathbf{u} \mid \mathbf{x})$ soit entier pour tout $\mathbf{x} \in G_1$ et que $(\mathbf{u} \mid \mathbf{y})$ soit entier pour tout $\mathbf{y} \in G_2$, en raison de la relation $(\mathbf{u} \mid \mathbf{x} + \mathbf{y}) = (\mathbf{u} \mid \mathbf{x}) + (\mathbf{u} \mid \mathbf{y})$; on a donc $(G_1 + G_2)^* = G_1^* \cap G_2^*$ pour tout couple de sous-groupes $G_1, G_2$ de $\mathbf{R}^n$. Si maintenant on suppose $G_1$ et $G_2$ fermés, on a $(G_1^* + G_2^*)^* = G_1 \cap G_2$ d’après la prop. 6 (VII, p. 7), d’où, en prenant les groupes associés, et appliquant de nouveau la prop. 6, $(G_1 \cap G_2)^* = \overline{G_1^* + G_2^*}$.

#### Remarque {#top-vii-s1-n3-rem-1 .statement}

Soient $G_1, G_2$ deux *réseaux* de $\mathbf{R}^n$ (n° 1) tels que $G_2 \subset G_1$; alors (VII, p. 7, prop. 5) $G_1^*$ et $G_2^*$ sont des *réseaux* de $\mathbf{R}^n$ tels que $G_1^* \subset G_2^*$. On a vu (VII, p. 2, prop. 1) qu’il existe un entier $m > 0$ tel que $mG_1 \subset G_2$. Pour $\mathbf{x} \in G_1$ et $\mathbf{u} \in G_2^*$, on a donc $m(\mathbf{u} \mid \mathbf{x}) \in \mathbf{Z}$, donc $(\mathbf{u} \mid \mathbf{x}) \in \mathbf{Q}$. En outre, si $\mathbf{x} \in G_2$ et $\mathbf{u} \in G_2^*$, ou si $\mathbf{x} \in G_1$ et $\mathbf{u} \in G_1^*$, on a par définition $(\mathbf{u} \mid \mathbf{x}) \in \mathbf{Z}$. On en déduit que, par passage aux quotients, l’application $\mathbf{Z}$-bilinéaire $(\mathbf{x}, \mathbf{u}) \to (\mathbf{u} \mid \mathbf{x})$ de $G_1 \times G_2^*$ dans $\mathbf{Q}$ définit une application $\mathbf{Z}$-bilinéaire B de $(G_1/G_2) \times (G_2^*/G_1^*)$ dans $\mathbf{Q}/\mathbf{Z}$. En outre, il est clair que si $\overline{\mathbf{x}}_0 \in G_1/G_2$ (resp. $\overline{\mathbf{u}}_0 \in G_2^*/G_1^*$) est tel que, pour *tout* $\overline{\mathbf{u}} \in G_2^*/G_1^*$ (resp. pour *tout* $\overline{\mathbf{x}} \in G_1/G_2$), on ait $B(\overline{\mathbf{x}}_0, \overline{\mathbf{u}}) = 0$ (resp. $B(\overline{\mathbf{x}}, \overline{\mathbf{u}}_0) = 0$) on a nécessairement $\overline{\mathbf{x}}_0 = 0$ (resp. $\overline{\mathbf{u}}_0 = 0$). On en conclut qu’il existe une *bijection* $\mathbf{Z}$-linéaire $h$ de $G_2^*/G_1^*$ sur $D(G_1/G_2)$ (avec les notations de A, VII, § 4, n° 8) telle que $\langle \overline{\mathbf{x}}, h(\overline{\mathbf{u}}) \rangle = B(\overline{\mathbf{x}}, \overline{\mathbf{u}})$ pour $\overline{\mathbf{x}} \in G_1/G_2$ et $\overline{\mathbf{u}} \in G_2^*/G_1^*$ (*loc. cit.*); en particulier, les groupes finis $G_1/G_2$ et $G_2^*/G_1^*$ sont *isomorphes*.

### 4. Groupes quotients séparés de $\mathbf{R}^n$

Tout groupe quotient séparé de $\mathbf{R}^n$ est de la forme $\mathbf{R}^n/H$, où $H$ est un sous-groupe *fermé* de $\mathbf{R}^n$ (III, p. 13, prop. 18). D’après le cor. 2 de VII, p. 6, il existe un automorphisme $f$ de $\mathbf{R}^n$ transformant $H$ en un sous-groupe $H'$, somme directe d’un sous-espace vectoriel engendré par $p$ des vecteurs $\mathbf{e}_i$ de la base canonique, et du groupe discret engendré par $q$ des $n - p$ vecteurs $\mathbf{e}_i$ restants ($0 \leq p + q \leq n$). Par passage aux quotients, $f$ donne un isomorphisme de $\mathbf{R}^n/H$ sur $\mathbf{R}^n/H'$ (III, p. 17, *Remarque 3*); or, $\mathbf{R}^n/H'$ est isomorphe à $\mathbf{R}^{n-p-q} \times \mathbf{T}^q$ (III, p. 18, corollaire). Donc:

#### Proposition 9 {#top-vii-s1-prop-9 .statement}

*Tout groupe quotient séparé de* $\mathbf{R}^n$ *est isomorphe à un groupe produit* $\mathbf{R}^h \times \mathbf{T}^k$ ($0 \leq h + k \leq n$).

L’espace produit $T^n$ (et, par abus de langage, le groupe topologique $T^n$) est appelé tore à n dimensions; d’après la prop. 4 de V, p. 2, c’est un espace compact, connexe et localement connexe.

En outre, si on désigne par C un cube fermé de côté 1 dans $\mathbf{R}^n$, $T^n$ est homéomorphe à l’espace quotient de C par la relation d’équivalence: « quel que soit i, $x_i \equiv y_i \pmod{1}$ » entre les points $\mathbf{x} = (x_i)$ et $\mathbf{y} = (y_i)$ de C. De façon plus imagée on dit que $T^n$ provient du cube C par « identification des faces opposées ».

#### Proposition 10 {#top-vii-s1-prop-10 .statement}

*Le groupe topologique $T^n$ est localement isomorphe à $\mathbf{R}^n$.* En effet, $T^n = (\mathbf{R}/\mathbf{Z})^n$ est isomorphe à $\mathbf{R}^n/\mathbf{Z}^n$ (III, p. 18, corollaire) et $\mathbf{Z}^n$ est un sous-groupe discret de $\mathbf{R}^n$ d’où la conclusion (III, p. 13, prop. 19).

Il en résulte que les groupes $\mathbf{R}^p \times T^{n-p}$ sont localement isomorphes à $\mathbf{R}^n$ pour $0 \leq p \leq n$; nous verrons dans VII, p. 13, que ce sont les seuls groupes connexes ayant cette propriété.

#### Proposition 11 {#top-vii-s1-prop-11 .statement}

*Tout sous-groupe fermé de $\mathbf{T}$, distinct de $\mathbf{T}$, est un groupe cyclique fini. Pour tout entier $n > 0$, $\mathbf{T}$ contient un sous-groupe d’ordre $n$ et un seul, qui est l’ensemble des éléments de $\mathbf{T}$ dont l’ordre divise $n$. Tout groupe quotient séparé de $\mathbf{T}$, non réduit à l’élément neutre, est isomorphe à $\mathbf{T}$.*

Soit $f : \mathbf{R} \to \mathbf{T}$ l’homomorphisme canonique. Les sous-groupes fermés de $\mathbf{T}$ sont les $f(H)$, où H est un sous-groupe fermé de $\mathbf{R}$ contenant $\mathbf{Z}$. D’après VII, p. 5, cor. 1 du th. 2, on a soit $H = \mathbf{R}$, c’est-à-dire $f(H) = \mathbf{T}$, soit $H = (1/n)\mathbf{Z}$, où $n$ est un entier $> 0$, auquel cas $f(H)$ est cyclique d’ordre $n$ et est l’ensemble des éléments de $\mathbf{T}$ dont l’ordre divise $n$. La dernière assertion résulte de l’existence d’un isomorphisme de $\mathbf{R}/H$ sur $\mathbf{T}/f(H)$.

Il résulte notamment de ce qui précède que $T^n$ et $T^m$ ne peuvent être algébriquement isomorphes que si $n = m$. En effet, $T^n$ possède $2^n - 1$ points d’ordre 2 et $2^n - 1 \neq 2^m - 1$ si $n \neq m$.

Tout groupe quotient séparé de $T^n$ est compact; il est donc isomorphe à un groupe quotient compact de $\mathbf{R}^n$, donc à un groupe $T^k$, $0 \leq k \leq n$ (VII, p. 8, prop. 9).

### 5. Sous-groupes et groupes quotients de $T^n$

Identifions $T^n$ et $\mathbf{R}^n/\mathbf{Z}^n$, et soit $\varphi$ l’homomorphisme canonique de $\mathbf{R}^n$ sur $\mathbf{R}^n/\mathbf{Z}^n$; tout sous-groupe de $T^n$ est de la forme $G = \varphi(H)$, H étant un sous-groupe de $\mathbf{R}^n$ contenant $\mathbf{Z}^n$ (A, I, p. 37), et est isomorphe à $H/\mathbf{Z}^n$ (III, p. 14, prop. 20); pour que G soit fermé dans $T^n$, il faut et il suffit que H soit fermé dans $\mathbf{R}^n$ (I, p. 21). Pour chercher les sous-groupes fermés de $T^n$, nous sommes donc ramenés à déterminer les sous-groupes fermés H de $\mathbf{R}^n$ tels que $H \supset \mathbf{Z}^n$; nous allons utiliser la prop. 6 de VII, p. 7, et déterminer d’abord le sous-groupe $H^*$ associé à un tel sous-groupe. Comme $\mathbf{Z}^n$ est son propre associé, on a $H^* \subset \mathbf{Z}^n$; par suite (VII, p. 2), il existe une base $(\mathbf{a}_i)$ ($1 \leq i \leq n$) de $\mathbf{R}^n$ engendrant $\mathbf{Z}^n$, et une base de $H^*$ (par rapport à l’anneau $\mathbf{Z}$) formée de $p$ points $\mathbf{b}_i$ ($1 \leq i \leq p$) tels que $\mathbf{b}_i = e_i \mathbf{a}_i$ pour $1 \leq i \leq p$, les $e_i$ étant des entiers qui satisfont à $e_{i+1} \equiv 0$ (mod. $e_i$) pour $1 \leq i \leq p - 1$. Soit $(\mathbf{a}'_i)$ la base duale de $(\mathbf{a}_i)$; pour que $\mathbf{u} = \sum_{i=1}^n u_i \mathbf{a}'_i$ appartienne à $(H^*)^* = H$, il faut et il suffit que $u_i e_i$ soit entier pour $1 \leq i \leq p$; autrement dit, $H$ est somme directe du sous-espace vectoriel $V$ engendré par $\mathbf{a}'_{p+1}, \ldots, \mathbf{a}'_n$, et du sous-groupe discret $K$ engendré par les $p$ points $(1/e_i) \mathbf{a}'_i$ ($1 \leq i \leq p$); d’autre part, $\mathbf{Z}^n$ est somme directe de $V \cap \mathbf{Z}^n$ et de $K \cap \mathbf{Z}^n$, puisque les $\mathbf{a}'_i$ ($1 \leq i \leq n$) engendrent $\mathbf{Z}^n$. Le groupe quotient $H/\mathbf{Z}^n$ est donc isomorphe à $(V/(V \cap \mathbf{Z}^n)) \times (K/(K \cap \mathbf{Z}^n))$ (III, p. 18, corollaire); $V/(V \cap \mathbf{Z}^n)$ est isomorphe à $\mathbf{T}^{n-p}$, et $K/(K \cap \mathbf{Z}^n)$ est un groupe *fini*, somme directe de $p$ groupes cycliques d’ordres respectifs $e_i$ ($1 \leq i \leq p$) (VII, p. 2).

En résumé:

#### Proposition 12 {#top-vii-s1-prop-12 .statement}

*Soient T un groupe topologique isomorphe à $\mathbf{T}^n$ et G un sous-groupe fermé de T. Il existe un isomorphisme de groupes topologiques f de T sur $\mathbf{T}^n$ et des sous-groupes fermés $G_1, \ldots, G_n$ de T tels que $f(G) = G_1 \times \cdots \times G_n$.*

#### Remarque {#top-vii-s1-n5-rem-1 .statement}

Il résulte notamment des prop. 11 et 12 qu’un sous-groupe fermé $G$ de $\mathbf{T}^n$ est le produit direct de sa composante neutre $G^0$, qui est isomorphe à un groupe $\mathbf{T}^h$ ($0 \leq h \leq n$), et d’un sous-groupe fini (qui est produit de $n - h$ sous-groupes cycliques, éventuellement réduits à l’élément neutre).

### 6. Fonctions périodiques

#### Définition 1 {#top-vii-s1-def-1 .statement}

*On dit qu’une fonction f, définie dans $\mathbf{R}^n$, et prenant ses valeurs dans un ensemble quelconque E, est périodique s’il existe un point $\mathbf{a} \neq 0$ de $\mathbf{R}^n$ tel que*

$$
f(\mathbf{x} + \mathbf{a}) = f(\mathbf{x})
$$

*quel que soit $\mathbf{x} \in \mathbf{R}^n$.* Si f est périodique, tout point $\mathbf{a} \in \mathbf{R}^n$ pour lequel la relation (1) est une identité en $\mathbf{x}$, est appelé une période de f.

L’ensemble G des périodes d’une fonction périodique f est évidemment un *sous-groupe* (non réduit à 0 par hypothèse) du groupe additif $\mathbf{R}^n$. Lorsque f est une application périodique *continue* de $\mathbf{R}^n$ dans un espace topologique *séparé* E, son groupe des périodes G est *fermé*. En effet, si $G_x$ désigne l’ensemble des $\mathbf{a} \in \mathbf{R}^n$ tels que $f(\mathbf{x} + \mathbf{a}) = f(\mathbf{x})$ pour *un point donné* $\mathbf{x} \in \mathbf{R}^n$, G est l’intersection des $G_x$ lorsque $\mathbf{x}$ parcourt $\mathbf{R}^n$, et chacun des $G_x$ est *fermé* (I, p. 53, prop. 2). Soit alors V le plus grand sous-espace vectoriel contenu dans G (VII, p. 5, th. 2); la fonction f est *constante* dans toute classe mod. V; si W désigne un sous-espace vectoriel supplémentaire de V, f est déterminée par sa restriction à W. Autrement dit (W étant un groupe topologique isomorphe à un $\mathbf{R}^p$), l’étude des fonctions périodiques continues dans $\mathbf{R}^n$ se ramène à l’étude de celles de ces fonctions $f$ dont le groupe des périodes $G$ est discret; si ce groupe est de rang $q$, on dit que $f$ est une fonction $q$ fois périodique, et tout système libre de $q$ points engendrant $G$ est appelé un système principal de périodes de $f$.

Si $(\mathbf{a}_i)$ et $(\mathbf{b}_i)$ sont deux systèmes principaux de périodes de $f$, on a vu (VII, p. 2) que chacun d’eux se déduit de l’autre par une transformation linéaire à coefficients entiers, de déterminant $+1$ ou $-1$.

Soit $\varphi$ l’application canonique de $\mathbf{R}^n$ sur $\mathbf{R}^n/G$; à toute application $g$ de $\mathbf{R}^n/G$ dans un ensemble $E$ correspond la fonction $\dot{g} = g \circ \varphi$, qui est une application périodique de $\mathbf{R}^n$ dans $E$, ayant un groupe de périodes qui contient $G$; et réciproquement, toute application de $\mathbf{R}^n$ dans $E$, admettant un groupe de périodes qui contient $G$, est de cette forme, puisqu’elle est compatible avec la relation $x \equiv y$ (mod. $G$) (E, II, p. 44). On définit ainsi une application bijective $g \mapsto \dot{g}$ de l’ensemble des applications de $\mathbf{R}^n/G$ dans $E$, sur l’ensemble des applications de $\mathbf{R}^n$ dans $E$ dont le groupe de périodes contient $G$. Pour que $\dot{g}$ soit continue (lorsque $E$ est un espace topologique) il faut et il suffit que $g$ le soit (I, p. 21, prop. 6).

## EXERCICES {#top-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
