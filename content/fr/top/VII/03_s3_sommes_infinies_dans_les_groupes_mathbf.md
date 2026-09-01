---
book: top
book_title: General Topology
chapter: VII
chapter_title: LES GROUPES ADDITIFS $\mathbf{R}^n$
section: 3
section_title: Sommes infinies dans les groupes $\mathbf{R}^n$
lang: fr
source: top-v-x-fr
pdf_pages: 0074-0077, 0083-0083
extraction: ocr
subsections:
    - "no": 1
      title: Familles sommables dans $\mathbf{R}^n$
      page: 0
      pdf_page: 74
    - "no": 2
      title: Séries dans $\mathbf{R}^n$
      page: 17
      pdf_page: 75
statements: 9
exercises: 2
content_sha256: 7dcf245f5701aa5188b28fcd4fa0b88da02ef48e1fe94d286b23948e2c36c69f
---

## § 3. SOMMES INFINIES DANS LES GROUPES $\mathbf{R}^n$

### 1. Familles sommables dans $\mathbf{R}^n$

Comme tout point de $\mathbf{R}^n$ possède un système fondamental *dénombrable* de voisinages, une famille $(\mathbf{x}_i)$ de points du groupe additif $\mathbf{R}^n$ ne peut être sommable que si l’ensemble des $i$ tels que $\mathbf{x}_i \neq 0$ est *dénombrable* (III, p. 38, corollaire), ce qui ramène essentiellement l’étude des familles sommables dans $\mathbf{R}^n$ à celle des *suites* sommables. Toutefois, pour les mêmes raisons que celles qui ont été exposées au sujet des familles sommables dans $\mathbf{R}$ (IV, p. 32), nous ne ferons, dans les énoncés qui suivent, aucune restriction sur la puissance de l’ensemble des indices.

#### Proposition 1 {#top-vii-s3-prop-1 .statement}

*Pour qu’une famille $(\mathbf{x}_i)_{i \in I}$ de points $\mathbf{x}_i = (x_{i,k})_{1 \leq k \leq n}$ de $\mathbf{R}^n$ soit sommable, il faut et il suffit que chacune des $n$ familles $(x_{i,k})_{i \in I}$ de nombres réels soit sommable dans $\mathbf{R}$.*

Cela résulte de la prop. 4 de III, p. 41.
Cette condition se transforme de la manière suivante:

#### Théorème 1 {#top-vii-s3-thm-1 .statement}

*Pour qu’une famille $(\mathbf{x}_i)_{i \in I}$ de points de $\mathbf{R}^n$ soit sommable, il faut et il suffit que la famille $(\|\mathbf{x}_i\|)$ des normes euclidiennes des $\mathbf{x}_i$ soit sommable dans $\mathbf{R}$.*

Cela résulte sans peine de la prop. 1, de la condition de sommabilité d’une famille de nombres réels (IV, p. 34, th. 3), des inégalités

$$
\sup_{1 \leq k \leq n} |x_{i,k}| \leq \|\mathbf{x}_i\| \leq \sum_{i=1}^n |x_{i,i}|,
$$

et du principe de comparaison (IV, p. 33, th. 2).

On peut procéder un peu autrement, en établissant d’abord la proposition suivante:

#### Proposition 2 {#top-vii-s3-prop-2 .statement}

*Pour toute famille finie $(\mathbf{x}_i)_{i \in I}$ de points de $\mathbf{R}^n$, on a*

(1)
$$
\sum_{i \in I} \|\mathbf{x}_i\| \leq 2n \cdot \sup_{J \subset I} \|\sum_{i \in J} \mathbf{x}_i\|.
$$

En effet, si $\mathbf{x}_i = (x_{ij})_{1 \leq j \leq n}$, on a $\|\mathbf{x}_i\| \leq \sum_{j=1}^n |x_{ij}|$, donc
$$
\sum_{i \in I} \|\mathbf{x}_i\| \leq \sum_{j=1}^n \left( \sum_{i \in I} |x_{ij}| \right).
$$
Or,
$$
\sum_{i \in I} |x_{ij}| = \sum_{i \in I} x_{ij}^+ + \sum_{i \in I} x_{ij}^-,
$$
et comme, pour toute partie $J$ de $I$, on a
$$
-\sum_{i \in I} x_{ij}^- \leq -\sum_{i \in J} x_{ij}^- \leq \sum_{i \in J} x_{ij} \leq \sum_{i \in J} x_{ij}^+ \leq \sum_{i \in I} x_{ij}^+,
$$
on en déduit
$$
\sum_{i \in I} |x_{ij}| \leq 2 \cdot \sup_{J \subset I} |\sum_{i \in J} x_{ij}|.
$$
Mais $|\sum_{i \in J} x_{ij}| \leq \|\sum_{i \in J} \mathbf{x}_i\|$, d’où l’inégalité (1).

D’autre part, le th. 1 équivaut à la proposition suivante (puisque $\mathbf{R}^n$ est un groupe complet): pour que la famille $(\mathbf{x}_t)$ satisfasse au critère de Cauchy (III, p. 38, th. 1), il faut et il suffit que la famille $(||\mathbf{x}_t||)$ satisfasse aussi à ce critère. Or l’inégalité du triangle montre que cette condition est suffisante, et l’inégalité (1) montre qu’elle est nécessaire.
En outre, on a l’inégalité
$$
\left| \sum_t \mathbf{x}_t \right| \leq \sum_t \left| \mathbf{x}_t \right|,
$$
qu’on déduit par passage à la limite de l’inégalité analogue pour les sommes partielles finies.

#### Corollaire {#top-vii-s3-n1-cor-1 .statement}

*Pour qu’une famille $(\mathbf{x}_t)$ de points de $\mathbf{R}^n$ soit sommable, il faut et il suffit que l’ensemble des sommes partielles finies de cette famille soit borné dans $\mathbf{R}^n$.*
D’après le th. 1 (VII, p. 16) et l’inégalité du triangle, cette condition est nécessaire; elle est suffisante d’après l’inégalité (1) et le th. 1.

#### Proposition 3 {#top-vii-s3-prop-3 .statement}

*Soient $(\mathbf{x}_\lambda)_{\lambda \in L}$ une famille sommable de points de $\mathbf{R}^m$, $(\mathbf{y}_\mu)_{\mu \in M}$ une famille sommable de points de $\mathbf{R}^n$, $f$ une application bilinéaire de $\mathbf{R}^m \times \mathbf{R}^n$ dans $\mathbf{R}^p$. La famille $(f(\mathbf{x}_\lambda, \mathbf{y}_\mu))_{(\lambda, \mu) \in L \times M}$ est sommable, et l’on a*
$$
\sum_{(\lambda, \mu) \in L \times M} f(\mathbf{x}_\lambda, \mathbf{y}_\mu) = f\left( \sum_{\lambda \in L} \mathbf{x}_\lambda, \sum_{\mu \in M} \mathbf{y}_\mu \right).
$$
Pour montrer que la famille des $f(\mathbf{x}_\lambda, \mathbf{y}_\mu)$ est sommable, il suffit (VII, p. 16, prop. 1) d’établir que chacune des $p$ familles formées par les coordonnées des $f(\mathbf{x}_\lambda, \mathbf{y}_\mu)$ dans $\mathbf{R}^n$ est sommable; autrement dit, on peut se limiter au cas où $f$ est une *forme* bilinéaire; mais, pour une telle forme $f$, on a $f(\mathbf{x}, \mathbf{y}) = \sum_{i,j} a_{ij} x_i y_j$, donc on est ramené au cas où $f(\mathbf{x}, \mathbf{y}) = x_i y_j$, et dans ce cas la proposition a déjà été démontrée (IV, p. 35, prop. 1).

En spécialisant la fonction $f$, on a en particulier les corollaires suivants:

#### Corollaire 1 {#top-vii-s3-prop-3-cor-1 .statement}

*Si $(a_\lambda)_{\lambda \in L}$ est une famille sommable de nombres réels, $(\mathbf{x}_\mu)_{\mu \in M}$ une famille sommable de points de $\mathbf{R}^n$, la famille $(a_\lambda \mathbf{x}_\mu)_{(\lambda, \mu) \in L \times M}$ est sommable, et l’on a*
$$
\sum_{(\lambda, \mu) \in L \times M} a_\lambda \mathbf{x}_\mu = \left( \sum_{\lambda \in L} a_\lambda \right) \left( \sum_{\mu \in M} \mathbf{x}_\mu \right).
$$

#### Corollaire 2 {#top-vii-s3-prop-3-cor-2 .statement}

*Si $(\mathbf{x}_\lambda)_{\lambda \in L}$ et $(\mathbf{y}_\mu)_{\mu \in M}$ sont deux familles sommables de points de $\mathbf{R}^n$, la famille $(\mathbf{x}_\lambda \mid \mathbf{y}_\mu)$ (cf. VI, p. 8) est sommable dans $\mathbf{R}$, et l’on a*
$$
\sum_{(\lambda, \mu) \in L \times M} (\mathbf{x}_\lambda \mid \mathbf{y}_\mu) = \left( \sum_{\lambda \in L} \mathbf{x}_\lambda \mid \sum_{\mu \in M} \mathbf{y}_\mu \right).
$$

### 2. Séries dans $\mathbf{R}^n$

Pour qu’une série de terme général $\mathbf{x}_m = (x_{mi})_{1 \leq i \leq n}$ soit convergente dans $\mathbf{R}^n$, il faut et il suffit évidemment que chacune des $n$ séries $(x_{mi})_{m \in \mathbf{N}}$ soit convergente dans $\mathbf{R}$.

#### Définition 1 {#top-vii-s3-def-1 .statement}

Une série de points de $\mathbf{R}^n$ est dite absolument convergente si la série des normes euclidiennes de ses termes est convergente.

#### Proposition 4 {#top-vii-s3-prop-4 .statement}

Pour qu’une série de points de $\mathbf{R}^n$, soit commutativement convergente, il faut et il suffit qu’elle soit absolument convergente.

C’est une conséquence de la prop. 9 de III, p. 44, et du th. 1 (VII, p. 16).

Les exemples de IV, p. 38, montrent que, dans $\mathbf{R}^n$, une série peut être convergente sans être absolument convergente.

Exercises

## EXERCICES {#top-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
