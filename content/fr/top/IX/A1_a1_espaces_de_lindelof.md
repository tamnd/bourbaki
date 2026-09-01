---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 1
section_title: Espaces de Lindelöf
appendix: true
lang: fr
source: top-v-x-fr
pdf_pages: 0195-0197
extraction: ocr
statements: 8
exercises: 0
content_sha256: 82bfed792246d4a3deff3f24ca86e0dd2545d6e631cac69468985fcbd6107a27
---

## APPENDICE 1

# ESPACES DE LINDELÖF

#### Définition 1 {#top-ix-a1-def-1 .statement}

On dit qu’un espace topologique $X$ (non nécessairement séparé) est un espace de Lindelöf si, de tout recouvrement ouvert de $X$, on peut extraire un recouvrement dénombrable de $X$.

#### Proposition 1 {#top-ix-a1-prop-1 .statement}

Soit $X$ un espace topologique.

(i) Si la topologie de $X$ admet une base dénombrable, $X$ est un espace de Lindelöf.

(ii) Soit $f : X \to Y$ une application continue de $X$ dans un espace topologique $Y$ (non nécessairement séparé). Si $X$ est un espace de Lindelöf, il en est de même du sous-espace $f(X)$ de $Y$.

(i) Soient $\mathcal{R}$ un recouvrement ouvert de $X$, $\mathcal{B}$ une base dénombrable de la topologie de $X$, $\mathcal{B}'$ l’ensemble des éléments $A \in \mathcal{B}$ tels qu’il existe un élément de $\mathcal{R}$ contenant $A$; $\mathcal{B}'$ est un recouvrement dénombrable de $X$, car tout $x \in X$ est contenu dans un ensemble $U \in \mathcal{R}$, et il existe ensuite $A \in \mathcal{B}$ tel que $x \in A \subset U$. Il existe alors une application $\Phi$ de $\mathcal{B}'$ dans $\mathcal{R}$ telle que l’on ait $A \subset \Phi(A)$ pour tout $A \in \mathcal{B}'$; il est clair que $\Phi(\mathcal{B}')$ est un recouvrement ouvert dénombrable de $X$ contenu dans $\mathcal{R}$.

(ii) Soit $(V_\lambda)_{\lambda \in L}$ une famille d’ensembles ouverts dans $Y$ formant un recouvrement de $f(X)$. Les ensembles $f^{-1}(V_\lambda)$ forment alors un recouvrement ouvert de $X$, et il existe par suite une partie dénombrable $J$ de $L$ telle que les ensembles ouverts $f^{-1}(V_\lambda)$ pour $\lambda \in J$ forment un recouvrement de $X$. Mais alors les ensembles $V_\lambda$ pour $\lambda \in J$ forment un recouvrement de $f(X)$, ce qui prouve que $f(X)$ est un espace de Lindelöf.

#### Corollaire {#top-ix-a1-n0-cor-1 .statement}

*Tout espace souslinien, et en particulier tout espace polonais ou lusinien, est un espace de Lindelöf.*

Cela résulte aussitôt de la prop. 1 précédente et de la définition des espaces sousliniens (IX, p. 59, déf. 2), puisqu’un espace polonais admet une base dénombrable.

#### Proposition 2 {#top-ix-a1-prop-2 .statement}

*Tout espace de Lindelöf régulier est paracompact.*

Soient $X$ un espace de Lindelöf régulier, et $\mathcal{R}$ un recouvrement ouvert de $X$. Pour tout $x \in X$, soit $U_x \in \mathcal{R}$ contenant $X$, et soit $V_x$ un voisinage ouvert de $x$ tel que $V_x \subset U_x$. Comme $X$ est un espace de Lindelöf, il existe une suite $(x_n)_{n \geq 0}$ de points de $X$ tels que les $V_{x_n}$ forment un recouvrement de $X$. Posons alors, pour tout entier $n \geq 0$, $W_n = U_{x_n} \cap \complement \left( \bigcup_{k < n} V_{x_k} \right)$. Les ensembles $W_n$ sont ouverts et forment un recouvrement de $X$ plus fin que $\mathcal{R}$. D’autre part, ce recouvrement est localement fini, car tout $x \in X$ appartient à un $V_{x_i}$ pour un $i$ au moins ; alors $V_{x_i}$ est un voisinage de $x$, qui ne rencontre aucun ensemble $W_n$ pour $n > i$.

#### Corollaire {#top-ix-a1-n0-cor-2 .statement}

*Tout espace souslinien régulier est paracompact* (et en particulier *normal* (IX, p. 49, prop. 4) et *a fortiori complètement régulier*).

#### Proposition 3 {#top-ix-a1-prop-3 .statement}

*Soit $X$ un espace topologique (non nécessairement séparé). Les propriétés suivantes sont équivalentes*:
a) *Tout sous-espace ouvert de $X$ est un espace de Lindelöf*.
b) *Tout ensemble de fonctions semi-continues inférieurement (resp. supérieurement) dans $X$ contient un sous-ensemble dénombrable qui admet la même enveloppe supérieure (resp. inférieure)*.

Montrons d’abord que b) entraîne a). Soit $U$ un sous-espace ouvert de $X$, et soit $(U_\lambda)_{\lambda \in L}$ une famille d’ensembles ouverts dans $U$ (donc dans $X$) recouvrant $U$. Les fonctions $\varphi_{U_\lambda}$ étant semi-continues inférieurement dans $X$, il existe une partie dénombrable $J$ de $L$ telle que la famille $(\varphi_{U_\lambda})_{\lambda \in J}$ ait même enveloppe supérieure $\varphi_U$ que la famille $(\varphi_{U_\lambda})_{\lambda \in L}$. On a par suite $U = \bigcup_{\lambda \in J} U_\lambda$, et $U$ est un espace de Lindelöf.

Prouvons maintenant que a) entraîne b). Soient $\mathcal{F}$ un ensemble de fonctions semi-continues inférieurement dans $X$, et $s$ l’enveloppe supérieure de $\mathcal{F}$. Soit $D$ une partie dénombrable dense de $\overline{\mathbf{R}}$. Pour toute fonction $f \in \mathcal{F}$ et tout nombre $d \in D$, soit $U_{f,d}$ l’ensemble ouvert des $x \in X$ tels que $f(x) > d$ (IV, p. 29). Par hypothèse, il existe une partie dénombrable $\mathcal{F}_d'$ de $\mathcal{F}$ telle que

$$
\bigcup_{f \in \mathcal{F}} U_{f,d} = \bigcup_{f \in \mathcal{F}_d'} U_{f,d}.
$$

Posons $\mathcal{F}' = \bigcup_{d \in D} \mathcal{F}'_d$, et désignons par $s'$ l’enveloppe supérieure de $\mathcal{F}'$. On a évidemment $s \geqslant s'$; d’autre part, soit $x$ un point de $X$, et soit $d$ un élément de $D$ tel que $s(x) > d$; il existe une fonction $f \in \mathcal{F}$ telle que $f(x) > d$; on a donc $x \in U_{f,d}$, et il existe une fonction $f' \in \mathcal{F}'_d$ telle que $x \in U_{f',d}$. Par suite, on a aussi $s'(x) > d$, d’où l’inégalité $s' \geqslant s$, et finalement $s' = s$. Comme $\mathcal{F}'$ est dénombrable, l’assertion est établie pour les fonctions semi-continues inférieurement; le cas des fonctions semi-continues supérieurement s’y ramène par changement de signe.

#### Corollaire 1 {#top-ix-a1-prop-3-cor-1 .statement}

*Soient $X$ un espace souslinien régulier, $H$ un ensemble de fonctions numériques continues dans $X$, qui sépare les points de $X$* (IX, p. 9, déf. 5). *Il existe alors une partie dénombrable $H'$ de $H$ qui sépare les points de $X$*.

En effet, $X \times X$ est un espace souslinien (IX, p. 60, prop. 7); il en est de même de tout sous-espace ouvert de $X \times X$ (IX, p. 59, prop. 5), qui est donc un espace de Lindelöf (IX, p. 76, corollaire). À toute fonction $h \in H$, associons l’ensemble fermé $F_h$ des couples $(x, y) \in X \times X$ tels que $h(x) = h(y)$. En vertu de la prop. 3, il existe une partie dénombrable $H'$ de $H$ telle que l’on ait $\bigcap_{h \in H'} F_h = \bigcap_{h \in H} F_h$. Mais par hypothèse le second membre est la diagonale de $X \times X$; il en est donc de même du premier, et par suite $H'$ sépare les points de $X$.

#### Corollaire 2 {#top-ix-a1-prop-3-cor-2 .statement}

*Tout espace compact souslinien est métrisable*.

Soient $X$ un espace compact souslinien, $I$ l’intervalle $[0, 1]$ de $\mathbf{R}$, $H$ l’ensemble des applications continues de $X$ dans $I$. Comme $X$ est complètement régulier, $H$ sépare les points de $X$, et le cor. 1 entraîne l’existence d’une suite $(f_n)$ d’éléments de $H$ qui sépare les points de $X$. Mais alors l’application $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ de $X$ dans $I^\mathbf{N}$, continue et injective, est un homéomorphisme de l’espace compact $X$ sur un sous-espace de $I^\mathbf{N}$; cela prouve que $X$ est métrisable.
