---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 2
section_title: REPRÉSENTATIONS DE TYPE RÉEL, COMPLEXE OU QUATERNIONIEN
appendix: true
lang: fr
source: lie-ix-fr
pdf_pages: 0106-0110
extraction: ocr
subsections:
    - "no": 1
      title: Représentations des algèbres réelles
      page: 0
      pdf_page: 106
    - "no": 2
      title: Représentations des groupes compacts
      page: 104
      pdf_page: 107
statements: 6
exercises: 0
content_sha256: adb80f7258da51f557ea84dd0c3de4fb1d1f67b32e6b291b0d3bf087cacd41eb
---

## APPENDICE 2

# Représentations de type réel, complexe ou quaternionien

### 1. Représentations des algèbres réelles

On note $\sigma$ l’automorphisme $\alpha \mapsto \overline{\alpha}$ de $\mathbf{C}$; si $W$ est un espace vectoriel complexe, on note $\overline{W}$ le $\mathbf{C}$-espace vectoriel $\sigma_*(W)$ (c’est-à-dire le groupe $W$ muni de la loi d’action $(\alpha, w) \mapsto \overline{\alpha}w$ pour $\alpha \in \mathbf{C}, w \in W$).

#### Proposition 1 {#lie-ix-a2-prop-1 .statement tag=01IS}

Soient $A$ une $\mathbf{R}$-algèbre (associative et unifère) et $V$ un $A$-module simple de dimension finie sur $\mathbf{R}$. On est alors dans l’un des trois cas suivants :

$\alpha)$ Le commutant de $V$ (A, VIII, § 5, no 1) est isomorphe à $\mathbf{R}$, et le $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ est simple ;
$\beta)$ le commutant de $V$ est isomorphe à $\mathbf{C}$; le $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ est somme directe de deux sous-$A_{(\mathbf{C})}$-modules simples non isomorphes, échangés par $\sigma \otimes 1_V$;
$\gamma)$ le commutant de $V$ est isomorphe à $\mathbf{H}$; le $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ est somme directe de deux sous-$A_{(\mathbf{C})}$-modules simples isomorphes échangés par $\sigma \otimes 1_V$.

Le commutant $E$ de $V$ est un corps, extension finie de $\mathbf{R}$ (A, VIII, § 3, no 2, prop. 2), donc isomorphe à $\mathbf{R}$, $\mathbf{C}$ ou $\mathbf{H}$ (A, VIII, § 15). Le $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ est semi-simple (A, VIII, § 11, no 4), et son commutant s’identifie à $\mathbf{C} \otimes_{\mathbf{R}} E$ (A, VIII, § 11, no 2, lemme 1).

Si $E$ est isomorphe à $\mathbf{R}$, le commutant de $V_{(\mathbf{C})}$ est isomorphe à $\mathbf{C}$, et $V_{(\mathbf{C})}$ est un $A_{(\mathbf{C})}$-module simple (A, VIII, § 11, no 4).

Si $E$ n’est pas isomorphe à $\mathbf{R}$, il contient un corps isomorphe à $\mathbf{C}$; on en déduit sur $V$ une structure de $A_{(\mathbf{C})}$-module, notée $V^c$. Alors $V^c$ est un $A_{(\mathbf{C})}$-module simple, et l’application $\mathbf{C}$-linéaire $\psi : V_{(\mathbf{C})} \to V^c \oplus \overline{V^c}$ telle que $\psi(\alpha \otimes v) = (\alpha v, \overline{\alpha} v)$ pour $\alpha \in \mathbf{C}, v \in V$, est un isomorphisme (A, V, p. 61, prop. 8). De plus $\sigma \otimes 1_V$ correspond par cet isomorphisme au $\mathbf{R}$-automorphisme $(v, v') \mapsto (v', v)$ de $V^c \oplus \overline{V^c}$, donc échange les sous-$A_{(\mathbf{C})}$-modules $\psi^{-1}(V^c)$ et $\psi^{-1}(\overline{V^c})$.

Le commutant $E_{(\mathbf{C})}$ de $V_{(\mathbf{C})}$ contient donc $\mathbf{C} \times \mathbf{C}$, opérant par homothéties sur $V^c \oplus \overline{V^c}$. Pour qu’il n’existe pas d’isomorphisme de $A_{(\mathbf{C})}$-modules de $V^c$ sur $\overline{V^c}$, il faut et il suffit que $E_{(\mathbf{C})}$ soit réduit à $\mathbf{C} \times \mathbf{C}$, c’est-à-dire que $E$ soit isomorphe à $\mathbf{C}$. Ceci achève la démonstration.

#### Proposition 2 {#lie-ix-a2-prop-2 .statement tag=01IT}

Soient $A$ une $\mathbf{R}$-algèbre (associative et unifère), et $W$ un $A_{(\mathbf{C})}$-module simple, de dimension finie sur $\mathbf{C}$. On est alors dans l’un des trois cas suivants :

a) Il existe un $A_{(\mathbf{C})}$-isomorphisme $\theta$ de $W$ sur $\overline{W}$, avec $\theta \circ \theta = 1_W$. Alors l’ensemble $V$ des points fixes de $\theta$ est une $\mathbf{R}$-structure sur $W$, et un $A$-module simple de commutant $\mathbf{R} \cdot 1_V$. De plus, $W_{[\mathbf{R}]}$ est somme directe de deux $A$-modules simples isomorphes.
b) Les $A_{(\mathbf{C})}$-modules $W$ et $\overline{W}$ ne sont pas isomorphes ; alors $W_{[\mathbf{R}]}$ est un $A$-module simple, de commutant $\mathbf{C} \cdot 1_W$.

c) Il existe un $A_{(C)}$-isomorphisme $\theta$ de $W$ sur $\overline{W}$, avec $\theta \circ \theta = -1_W$. Alors le $A$-module $W_{[R]}$ est simple, et son commutant est le corps $C.1_W \oplus C.\theta$, isomorphe à $H$.

L’espace vectoriel complexe $\mathrm{Hom}_{A_{(C)}}(W, W)$ est de dimension $\leqslant 1$ (A, VIII, § 3, n° 2); si $\theta \in \mathrm{Hom}_{A_{(C)}}(W, \overline{W})$, l’endomorphisme $\theta \circ \theta$ de $W$ est une homothétie, de rapport $\alpha \in C$. Pour tout $w \in W$, on a $\alpha \theta(w) = \theta \circ \theta \circ \theta(w) = \theta(\alpha w) = \overline{\alpha} \theta(w)$ de sorte que $\alpha$ est réel. Si $\theta' = \lambda \theta$, avec $\lambda \in C$, on a $\theta' \circ \theta' = |\lambda|^2 \theta \circ \theta$; une et une seule des trois possibilités suivantes est donc réalisée :

a) Il existe $\theta \in \mathrm{Hom}_{A_{(C)}}(W, \overline{W})$ avec $\theta \circ \theta = 1_W$;
b) $\mathrm{Hom}_{A_{(C)}}(W, \overline{W}) = \{0\}$;
c) Il existe $\theta \in \mathrm{Hom}_{A_{(C)}}(W, \overline{W})$ avec $\theta \circ \theta = -1_W$.

Dans le cas a), l’ensemble $V$ des points fixes de $\theta$ est une $R$-structure sur $W$ (A, V, p. 61, prop. 7); puisque $V_{(C)}$ est isomorphe à $W$, le $A$-module $V$ est simple, de commutant $R.1_V$ (prop. 1), et $W_{[R]}$ n’est pas simple.

Inversement, si $W_{[R]}$ n’est pas simple, soit $V$ un sous-$A$-module simple de $W_{[R]}$; puisque le $A_{(C)}$-module $W$ est simple, on a $V + iV = W$ et $V \cap iV = \{0\}$, c’est-à-dire $W = V \oplus iV$. Ainsi $V$ est une $R$-structure sur $W$, et l’isomorphisme $\theta$ de $W$ sur $\overline{W}$ tel que $\theta(v + iv') = v - iv'$ pour $v$ et $v'$ dans $V$ satisfait à $\theta \circ \theta = 1_W$.

Par conséquent, dans les cas b) et c), le $A$-module $W_{[R]}$ est simple ; d’après la prop. 1, son commutant $E$ est isomorphe à $C$ dans le cas b), et à $H$ dans le cas c). De plus il est clair que $E$ contient $C.1_W$, et $C.\theta$ dans le cas c), d’où la proposition.

Sous les hypothèses de la proposition, on dit que le $A_{(C)}$-module $W$ est de type réel, complexe ou quaternionien (relativement à $A$) suivant qu’on est dans le cas a), b) ou c) respectivement.

Pour $K = R$ ou $C$, notons $\mathfrak{S}_K(A)$ l’ensemble des classes de $A_{(K)}$-modules simples, de dimension finie sur $K$. Le groupe $\Gamma = \mathrm{Gal}(C/R)$ opère sur $\mathfrak{S}_C(A)$; les deux propositions précédentes établissent une correspondance bijective entre $\mathfrak{S}_R(A)$ et l’ensemble quotient $\mathfrak{S}_C(A)/\Gamma$.

### 2. Représentations des groupes compacts

Soit $G$ un groupe topologique compact, et soit $\rho : G \to \mathrm{GL}(W)$ une représentation continue de $G$ dans un espace vectoriel complexe de dimension finie. On dira que $\rho$ est irréductible de type réel, complexe ou quaternionien s’il en est ainsi du $C^{(G)}$-module $W$ (relativement à l’algèbre $A = R^{(G)}$). Soit $H$ une forme hermitienne positive séparante sur $W$, invariante par $G$.

#### Proposition 3 {#lie-ix-a2-prop-3 .statement tag=01IU}

Supposons $\rho$ irréductible.

a) La représentation $\rho$ est de type réel si et seulement s’il existe une forme bilinéaire symétrique $B$ non nulle sur $W$, invariante par $G$. Dans ce cas la forme $B$ est séparante ; l’ensemble $V$ des $w \in W$ tels que $H(w, x) = B(w, x)$ pour tout $x \in W$ est une $R$-structure sur $W$ invariante par $G$.

b) La représentation $\rho$ est de type complexe si et seulement s’il n’existe pas de forme bilinéaire non nulle sur $W$ invariante par $G$.

c) La représentation $\rho$ est de type quaternionien si et seulement s'il existe une forme bilinéaire alternée non nulle sur $W$, invariante par $G$; une telle forme est nécessairement séparante.

Pour $\theta \in \mathrm{Hom}_{\mathbf{C}(G)}(W, \overline{W})$ et $x, y \in W$, posons $B_\theta(x, y) = H(\theta x, y)$. Alors $B_\theta$ est une forme bilinéaire sur $W$, invariante par $G$, séparante si $\theta$ est non nul. Notons $\mathcal{B}(W)^G$ l'espace des formes bilinéaires sur $W$ invariantes par $G$; l'application $\theta \mapsto B_\theta$ de $\mathrm{Hom}_{\mathbf{C}(G)}(W, \overline{W})$ sur $\mathcal{B}(W)^G$ est un isomorphisme de $\mathbf{C}$-espaces vectoriels. Ceci entraîne, en particulier, l'assertion $b$.

Soit $\theta$ un $\mathbf{C}^{(G)}$-isomorphisme de $W$ sur $\overline{W}$ tel que $\theta \circ \theta = \alpha_w$, avec $\alpha \in \{ -1, +1 \}$ (prop. 2); puisque $\mathcal{B}(W)^G$ est de dimension 1, il existe $\varepsilon \in \mathbf{C}$ tel que

$$
B_\theta(y, x) = \varepsilon B_\theta(x, y) \quad \text{quels que soient } x, y \text{ dans } W .
$$

On obtient en itérant $B_\theta(y, x) = \varepsilon B_\theta(x, y) = \varepsilon^2 B_\theta(y, x)$, d'où $\varepsilon^2 = 1$ et $\varepsilon \in \{ -1, +1 \}$.

On a par ailleurs, pour $x$ dans $W$,

$$
H(\theta x, \theta x) = B_\theta(x, \theta x) = \varepsilon B_\theta(\theta x, x) = \varepsilon H(\theta \circ \theta(x), x) = \varepsilon \alpha H(x, x)
$$

d'où $\varepsilon \alpha > 0$ puisque $H$ est positive, c'est-à-dire $\varepsilon = \alpha$. Les assertions a) et c) résultent alors de la prop. 2.

Notons $dg$ la mesure de Haar de masse totale 1 sur $G$.

#### Lemme 1 {#lie-ix-a2-lem-1 .statement tag=01IV}

Soit $W^G$ le sous-espace de $W$ formé des éléments invariants par $G$. L'endomorphisme $\int_G \rho(g) \, dg$ de $W$ est un projecteur d'image $W^G$, compatible aux opérations de $G$. On a en particulier

$$
\dim W^G = \int_G \mathrm{Tr} \, \rho(g) \, dg .
$$

Posons $p = \int_G \rho(g) \, dg$; on a, pour $h \in G$,

$$
\rho(h) \circ p = \int_G \rho(hg) \, dg = \int_G \rho(g) \, dg = p
$$

et de même $p \circ \rho(h) = p$. Ainsi $p$ est compatible aux opérations de $G$, et son image est contenue dans $W^G$. Si $w \in W^G$, on a $p(w) = \int_G \rho(g)w \, dg = w$, d'où le lemme.

#### Lemme 2 {#lie-ix-a2-lem-2 .statement tag=01IW}

Soit $u$ un endomorphisme d'un espace vectoriel $E$ de dimension finie sur un corps $K$. On a

$$
\mathrm{Tr} \, u^2 = \mathrm{Tr} \, S^2(u) - \mathrm{Tr} \, \Lambda^2(u) .
$$

Soit $\chi_u(X) = \prod_{i=1}^n (X - \alpha_i)$ une décomposition en facteurs linéaires du polynôme caractéristique de $u$ dans une extension convenable de $K$. On a $\operatorname{Tr} u^2 = \sum_i \alpha_i^2$, $\operatorname{Tr} \Lambda^2(u) = \sum_{i < j} \alpha_i \alpha_j$, $\operatorname{Tr} S^2(u) = \sum_{i \leq j} \alpha_i \alpha_j$ (*cf.* A, VII, p. 37, cor. 3), d’où le résultat.

#### Proposition 4 {#lie-ix-a2-prop-4 .statement tag=01IX}

*Supposons $\rho$ irréductible. Pour que $\rho$ soit de type réel (resp. complexe, resp. quaternionien), il faut et il suffit que l’intégrale* $\int_G \operatorname{Tr} \rho(g^2) \, dg$ *soit égale à* 1 *(resp. 0, resp. — 1).*

Notons $\check{\rho}$ la représentation contragrédiente de $\rho$ dans $W^*$ (définie par $\check{\rho}(g) = {}^t\rho(g^{-1})$). En appliquant le lemme 2 à $\check{\rho}(g)$ et en intégrant sur $G$, on obtient

$$
\int_G \operatorname{Tr} \rho(g^2) \, dg = \int_G \operatorname{Tr} {}^t\rho(g^{-2}) \, dg = \int_G \operatorname{Tr} S^2(\check{\rho}(g)) \, dg - \int_G \operatorname{Tr} \Lambda^2(\check{\rho}(g)) \, dg
$$

d’où, d’après le lemme 1,

$$
\int_G \operatorname{Tr} \rho(g^2) \, dg = \dim(S^2W^*)^G - \dim(\Lambda^2W^*)^G.
$$

Or $S^2W^*$ (resp. $\Lambda^2W^*$) s’identifie à l’espace des formes bilinéaires symétriques (resp. alternées) sur $W$. La proposition résulte donc aussitôt de la prop. 3.

Exercises
