---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 3
section_title: Formes hermitiennes et formes quadratiques
lang: fr
source: alg-ix-fr
pdf_pages: 0047-0061
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes et $\varepsilon$-hermitiennes.
      page: 0
      pdf_page: 47
    - "no": 2
      title: '*Modules sur une extension quadratique*.'
      page: 0
      pdf_page: 49
    - "no": 3
      title: Formes bilinéaires associées à une forme hermitienne.
      page: 0
      pdf_page: 50
    - "no": 4
      title: Formes quadratiques.
      page: 0
      pdf_page: 52
statements: 7
exercises: 0
content_sha256: c0d7c8b724352f8b0f88aedc95fe9241b73de923d6f20ae8f8560d6971352e3d
---

## § 3. Formes hermitiennes et formes quadratiques

Dans toute la suite de ce Chapitre, on désigne, sauf mention expresse du contraire, par A un anneau et par E un A-module à gauche. On suppose A muni d’un antiautomorphisme involutif J, noté $\alpha \to \overline{\alpha}$; on a donc $(\alpha + \beta) = \overline{\alpha} + \overline{\beta}$, $(\alpha \beta) = \overline{\beta} \cdot \overline{\alpha}$ et $\overline{\alpha} = \alpha$ quels que soient $\alpha, \beta$ dans A. Sauf mention expresse du contraire, les formes sesquilinéaires considérées sont sesquilinéaires à droite (§ 1, n° 2, déf. 4) pour cet antiautomorphisme.

### 1. Formes hermitiennes et $\varepsilon$-hermitiennes.

#### Définition 1 {#alg-ix-s3-def-1 .statement}

Soit $\varepsilon$ un élément du centre de A. Une forme sesquilinéaire $\Phi$ sur E telle que l’on ait $\Phi(x, y) = \varepsilon \overline{\Phi(y, x)}$ quel que soient $x$ et $y$ dans E s’appelle une forme $\varepsilon$-hermitienne. Une forme 1-hermitienne (resp. (−1)-hermitienne) est dite hermitienne (resp. antihermitienne).

Lorsque J est l’identité (ce qui implique que A est commutatif) une forme hermitienne (resp. antihermitienne) (pour J) n’est autre qu’une forme bilinéaire symétrique (resp. antisymétrique) (chap. III, § 5, n° 1, déf. 2). Rappelons qu’une forme bilinéaire alternée (chap. III, § 5, n° 2, déf. 4) est antisymétrique ; la réciproque est vraie si, dans A, la relation $2a = 0$ entraîne $a = 0$.

La relation d’orthogonalité ($§ 1, n° 3$) par rapport à une forme $\varepsilon$-hermitienne est évidemment symétrique (cf. exerc. 1).

Si $\alpha$ est un élément inversible de A, l’application $T : \lambda \to \alpha^{-1} \overline{\lambda} \alpha$ est un antiautomorphisme de A, et l’on vérifie aisément que la forme $\Phi \alpha$ est sesquilinéaire par rapport à T. Si, de plus, on a $\alpha = \overline{\alpha}$, alors T est involutif, et, si $\Phi$ est $\varepsilon$-hermitienne, $\Phi \alpha$ l’est aussi ; en effet on a
$$
(\lambda^T)^T = \alpha^{-1} (\overline{\alpha^{-1} \lambda \alpha}) \alpha = \alpha^{-1} \overline{\alpha} \lambda \overline{\alpha^{-1}} \alpha = \lambda
$$
$$
\Phi(y, x) \alpha = \varepsilon \overline{\Phi(x, y)} \alpha = \varepsilon (\Phi(x, y) \alpha)^T.
$$

En particulier, lorsque A est un corps, les éléments $\alpha$ du centre de A tels que $\overline{\alpha} = \alpha$ forment un sous-corps K de A, et les formes $\varepsilon$-hermitiennes sur E (pour J) forment un espace vectoriel sur K.

#### Remarque 1 {#alg-ix-s3-n1-rem-1 .statement}

Si $\Phi$ est une forme $\varepsilon$-hermitienne sur E, on a $\Phi(x, y) = \varepsilon \overline{\Phi(x, y)} \overline{\varepsilon}$ quels que soient $x, y$ dans E. Donc, si $\Phi$ prend des valeurs inversibles, on a $\varepsilon \overline{\varepsilon} = 1$.
2) S’il existe un élément inversible $i$ du centre de A tel que $\overline{i} = i \varepsilon$, alors, pour que $\Phi$ soit $\varepsilon$-hermitienne, il faut et il suffit que $i \Phi$ soit hermitienne.

L’application $(y, x) \to \overline{\Phi(x, y)}$ étant sesquilinéaire pour J, pour que $\Phi$ soit $\varepsilon$-hermitienne, il faut et il suffit que l’on ait $\Phi(y, x) = \varepsilon \overline{\Phi(x, y)}$ lorsque $x$ et $y$ parcourent un système de générateurs de E. En particulier, si E admet une base finie $(e_i)_{1 \leq i \leq n}$, pour qu’une forme sesquilinéaire $\Phi$ sur E soit $\varepsilon$-hermitienne, il faut et il suffit que sa matrice $R = (\rho_{ij}) = (\Phi(e_i, e_j))$ vérifie les relations $\rho_{ji} = \varepsilon \overline{\rho_{ij}}$ quels que soient $i, j$, c’est-à-dire $'R = \varepsilon \overline{R}$ ; une matrice $R$ possédant cette propriété est dite $\varepsilon$-hermitienne. Lorsque $\varepsilon = 1$ (resp. $-1$) on dit que $R$ est hermitienne (resp. antihermitienne) relativement à l’antiautomorphisme J. Lorsque J est l’identité (donc A commutatif), une matrice hermitienne (resp. antihermitienne) $R$ est telle que $'R = R$ (resp. $'R = -R$) ; on dit alors que $R$ est une matrice symétrique (resp. antisymétrique). Pour que $\Phi$ soit une forme alternée, il faut et il suffit que sa matrice soit antisymétrique et, en outre, que les termes diagonaux de $R$ soient tous nuls ; une matrice possédant ces propriétés est dite alternée.

Soit $\Phi$ une forme sesquilinéaire sur $E$, et soient $s_\Phi$ et $d_\Phi$ les applications de $E$ dans $E^*$ associées à $\Phi$ à gauche et à droite ($\S 1$, n° 6). Pour que $\Phi$ soit $\varepsilon$-hermitienne, il faut et il suffit que $\langle x, s_\Phi(y) \rangle = \bar{\varepsilon} \langle x, d_\Phi(y) \rangle$ quels que soient les éléments $x, y$ de $E$, donc que $s_\Phi = \bar{\varepsilon} d_\Phi$, ou encore que $\langle x, d_\Phi(y) \rangle = \varepsilon \langle x, s_\Phi(y) \rangle$, donc que $d_\Phi = \varepsilon s_\Phi$.

Soit $\Phi$ une forme $\varepsilon$-hermitienne telle que l’application $d_\Phi$ de $E$ dans $E^*$ associée à droite à $\Phi$ soit bijective. Pour tout endomorphisme $u$ de $E$ on a alors
$$
u^{**} = \varepsilon \bar{\varepsilon} u.
$$
En effet, quels que soient les éléments $x$ et $y$ de $E$, on a
$$
\begin{align*}
\Phi(x, u^{**(y)}) &= \Phi(u^*(x), y) = \varepsilon \overline{\Phi(y, u^*(x))} = \varepsilon \overline{\Phi(u(y), x)} \\
&= \varepsilon \Phi(x, u(y)) \bar{\varepsilon} = \Phi(x, \varepsilon \bar{\varepsilon} u(y))
\end{align*}
$$
donc $u^{**(x)} = \varepsilon \bar{\varepsilon} u(x)$ puisque $\Phi$ est non dégénérée.

Si $\Phi$ est une forme $\varepsilon$-hermitienne telle que les applications $s_\Phi$ et $d_\Phi$ soient bijectives, alors la *forme inverse* $\widehat{\Phi}$ de $\Phi$ ($\S 1$, n° 7) *est une forme* $\bar{\varepsilon}$-hermitienne. En effet, en posant $s = s_\Phi$, $d = d_\Phi$ pour abréger, on déduit de $d = \varepsilon s$ que $s^{-1} = \bar{\varepsilon} d^{-1}$, $s$ étant semi-linéaire. Par suite, quels que soient $u, v$ dans $E$, on a
$$
\widehat{\Phi}(u, v) = \Phi(s^{-1}(u), d^{-1}(v)) = \bar{\varepsilon} \Phi(d^{-1}(u), d^{-1}(v)),
$$
d’où
$$
\widehat{\Phi}(v, u) = \bar{\varepsilon} \varepsilon \overline{\Phi(d^{-1}(u), d^{-1}(v))} = \bar{\varepsilon} \overline{\widehat{\Phi}(u, v)},
$$
puisque, $\varepsilon$ est dans le centre de $A$.

Enfin, lorsque l’anneau $A$ est commutatif, les prolongements canoniques d’une forme $\varepsilon$-hermitienne $\Phi$ aux puissances tensorielle et extérieure $\bigotimes^p E$ et $\wedge^p E$ de $E$ sont des formes $\varepsilon^p$-hermitiennes, comme il résulte aussitôt des formules (35) et (37) du $\S 1$, n° 9.

### 2. *Modules sur une extension quadratique*.

Soit $K$ un anneau commutatif. On prend pour $A$ l’extension quadratique $A = K(i)$ avec $i^2 = -1$, et pour $J$ l’automorphisme λ + iμ → λ − iμ ($\lambda \in K, \mu \in K$) (chap. II, § 7, n° 7). Si E est un A-module, nous noterons $E_0$ le K-module déduit de E par restriction de l’anneau des scalaires, et par j l’automorphisme $x \to ix$ de $E_0$; on a évidemment $j^2 = -I$, où I est l’application identique de $E_0$. Inversement soit $E_0$ un K-module et soit j un automorphisme de $E_0$ tel que $j^2 = -I$; l’application $\lambda + i\mu \to \lambda I + \mu j$ est évidemment un homomorphisme de A dans l’anneau $\mathcal{L}(E_0)$ des endomorphismes de $E_0$; on a donc défini sur $E_0$ une structure de A-module, pour laquelle on a

(2) $$(\lambda + i\mu)x = \lambda x + \mu j(x)$$ $(x \in E_0, \lambda \in K, \mu \in K).$

Si $E'$ est un autre A-module, $E'_0$ le K-module sous-jacent à $E'$, $j'$ l’automorphisme $x' \to ix'$ de $E'_0$, alors les applications A-linéaires f de E dans $E'$ ne sont autres que les applications K-linéaires de $E_0$ dans $E'_0$ telles que $f \circ j = j' \circ f$. En particulier, si l’on note $E^*$ et $(E_0)^*$ les duals respectifs de E et $E_0$, et si $f_1$ et $f_2$ sont deux applications de E dans K, pour que l’application $x \to f_1(x) + if_2(x)$ de E dans A soit A-linéaire, il faut et il suffit que $f_1$ et $f_2$ soient dans $(E_0)^*$ et que l’on ait $f_1 \circ j + i(f_2 \circ j) = if_1 - f_2$, c’est-à-dire $f_1 = f_2 \circ j$ et $f_1 \circ j = -f_2$. Comme j est un automorphisme de $E_0$ et que $j^2 = -I$, ces deux conditions sont équivalentes. En éliminant $f_1$ ou $f_2$, on voit que les formules

(3) $$f(x) = f_1(x) - if_1(j(x))$$
(4) $$f(x) = f_2(j(x)) + if_2(x)$$

$(x \in E,\ f \in E^*,\ f_1 \in (E_0)^*,\ f_2 \in (E_0)^*)$ établissent deux correspondances biunivoques entre $E^*$ et $(E_0)^*$.

### 3. Formes bilinéaires associées à une forme hermitienne.

Nous supposons encore ici que l’anneau A est l’extension quadratique $A = K(i)$ (où $i^2 = -1$) d’un anneau commutatif K, et que J est l’automorphisme $\lambda + i\mu \to \lambda - i\mu$ de A ($\lambda \in K, \mu \in K$). Soient E et $E'$ deux A-modules, $E_0$ et $E'_0$ les K-modules sous-jacents à E et $E'$, j et $j'$ les automorphismes $x \to ix$ et $x' \to ix'$ de E et $E'$ (cf. n° 2). Une forme K-bilinéaire $f$ sur $E_0 \times E'_0$ sera dite *invariante par j et $j'$* si l’on a

(5) $$f(j(x), j'(x')) = f(x, x')$$

pour $x \in E_0$ et $x' \in E'_0$. Remplaçant $x$ par $j(x)$, on voit que cette condition équivaut à

$$
f(x, j'(x')) = - f(j(x), x')
$$

quels que soient $x \in E_0$ et $x' \in E'_0$.

#### Proposition 1 {#alg-ix-s3-prop-1 .statement}

Soit $\Phi_1$ (resp. $\Phi_2$) une forme K-bilinéaire sur $E_0 \times E'_0$, invariante par $j$ et $j'$. L’application qui à $\Phi_1$ (resp. $\Phi_2$) fait correspondre l’application $\Phi$ de $E \times E'$ dans $A$ définie par

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$)

$(x \in E, x' \in E)$, est un isomorphisme du K-espace vectoriel des formes K-bilinéaires sur $E_0 \times E'_0$ invariantes par $j$ et $j'$ sur le K-espace vectoriel des formes sesquilinéaires sur $E \times E'$. Supposons de plus $E = E'$; pour que $\Phi$ soit hermitienne, il faut et il suffit que $\Phi_1$ soit symétrique (resp. que $\Phi_2$ soit antisymétrique) (cf. exerc. 4).

En effet toute application $\Phi$ de $E \times E'$ dans $A$ s’écrit, d’une manière et d’une seule, sous la forme $\Phi = \Phi_1 + i \Phi_2$, où $\Phi_1$ et $\Phi_2$ sont des applications de $E \times E'$ dans $K$. Pour que l’application partielle $x \to \Phi(x, x')$ soit A-linéaire, il faut et il suffit, d’après la formule (3) (resp. (4)) du n° 2, que $\Phi_1$ (resp. $\Phi_2$) soit K-linéaire en $x$ et que l’on ait

$$
\Phi(x, x') = \Phi_1(x, x') - i \Phi_1(j(x), x')
$$
(resp. $\Phi(x, x') = \Phi_2(j(x), x') + i \Phi_2(x, x')$).

De même, pour que $\overline{\Phi}(x, x')$ soit A-linéaire en $x'$, il faut et il suffit que $\Phi_1$ (resp. $\Phi_2$) soit K-linéaire en $x'$ et que l’on ait

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$).

Il en résulte immédiatement que, pour que $\Phi$ soit sesquilinéaire, il faut et il suffit qu’elle s’écrive sous l’une ou l’autre formes (9) et (11) (resp. (10) et (12)) avec $\Phi_1$ (resp. $\Phi_2$) K-bilinéaire invariante par $j$ et $j'$.

Il résulte de ceci que, pour qu’une forme sesquilinéaire $\Phi = \Phi_1 + i \Phi_2$ soit nulle, il faut et il suffit que $\Phi_1$ (resp. $\Phi_2$) soit nulle. Or, si $E = E'$, on a $\Phi(y, x) = \Phi_1(y, x) + i \Phi_2(y, x)$ et $\overline{\Phi(x, y)} = \Phi_1(x, y) - i \Phi_2(x, y)$; pour que ces deux expressions soient égales, autrement dit pour que $\Phi$ soit hermitienne, il faut et il suffit donc que $\Phi_1$ soit symétrique (resp. que $\Phi_2$ soit antisymétrique).

#### Remarque 1 {#alg-ix-s3-n3-rem-1 .statement}

Les formules (7) et (8) montrent que, si $x \in E$, pour que l’on ait $\Phi(x, x') = 0$ pour tout $x' \in E'$, il faut et il suffit que $\Phi_1(x, x') = 0$ (resp. $\Phi_2(x, x') = 0$) pour tout $x' \in E'$.
2) L’adjoint d’un endomorphisme $u$ de $E$ par rapport à $\Phi$ ($\S 1$, n° 8) est le même que l’adjoint de $u$ (considéré comme endomorphisme de $E_0$) par rapport à $\Phi_1$ (resp. $\Phi_2$).

### 4. Formes quadratiques.

#### Définition 2 {#alg-ix-s3-def-2 .statement}

On suppose l’anneau $A$ commutatif. On dit qu’une application $Q$ de $E$ dans $A$ est une forme quadratique sur $E$ si
1) l’on a $Q(\alpha x) = \alpha^2 Q(x)$ pour $\alpha \in A$ et $x \in E$;
2) l’application $\Phi : (x, y) \to Q(x + y) - Q(x) - Q(y)$ de $E \times E$ dans $A$ est une forme bilinéaire.
La forme bilinéaire $\Phi$ (qui est nécessairement symétrique) s’appelle la forme bilinéaire associée à $Q$. Si $\Phi$ est non dégénérée, on dit que $Q$ est non dégénérée.

Comme $Q(2x) = 4Q(x)$, il résulte aussitôt de 2) que l’on a
$$
\Phi(x, x) = 2Q(x).
$$
En particulier, si $A$ est un anneau de caractéristique 2, la forme $\Phi$ est alternée.

On dira que deux éléments (resp. deux sous-ensembles) de $E$ sont orthogonaux relativement à $Q$ s’ils sont orthogonaux relativement à la forme bilinéaire associée $\Phi$.

Soient $(x_i)_{i \in I}$ une famille d’éléments de $E$ et $(a_i)_{i \in I}$ une famille d’éléments de $A$ nuls sauf un nombre fini d’entre eux. Par récurrence sur le nombre des indices $i$ pour lesquels $a_i \neq 0$, on montre aisément que l’on a
$$
Q(\sum_i a_i x_i) = \sum_i a_i^2 Q(x_i) + \sum_{\{i, j\}} a_i a_j \Phi(x_i, x_j),
$$

la dernière sommation étant étendue aux sous-ensembles à deux éléments de I.

Pour toute forme bilinéaire $f$ sur $E \times E$, on définit une forme quadratique $Q$ en posant $Q(x) = f(x, x)$; la forme bilinéaire $\Phi$ associée à $Q$ est alors définie par $\Phi(x, y) = f(x, y) + f(y, x)$ pour $x, y$ dans $E$. De plus, si l’on suppose que le scalaire 2 a un inverse $\frac{1}{2}$ dans $A$, il existe une forme bilinéaire symétrique $f$ et une seule telle que $Q(x) = f(x, x)$, à savoir $f = \frac{1}{2} \Phi$; le discriminant de $f$ par rapport à un système $S = (x_1, \ldots, x_n)$ s’appelle aussi le discriminant de $Q$ par rapport à $S$. Il y a donc dans ce cas correspondance biunivoque entre les formes quadratiques et les formes bilinéaires symétriques sur $E$ (cf. exerc. 6).

Dans le cas d’un module libre, on a de plus le résultat suivant :

#### Proposition 2 {#alg-ix-s3-prop-2 .statement}

Supposons que $A$ soit commutatif et que $E$ admette une base $(e_i)_{i \in I}$. Alors, pour toute forme quadratique $Q$ sur $E$, il existe une forme bilinéaire $f$ sur $E \times E$ telle que $Q(x) = f(x, x)$ pour tout $x \in E$. Pour toute famille $(b_{ij})_{(i,j) \in I \times I}$ de scalaires tels que $b_{ij} = b_{ji}$ pour $(i, j) \in I \times I$, il existe une forme quadratique $Q$ et une seule telle que l’on ait

$$
Q(e_i) = b_{ii}, \quad \Phi(e_i, e_j) = b_{ij} \text{ pour } i \neq j,
$$

où $\Phi$ désigne la forme bilinéaire associée à $Q$; alors $Q$ est donnée par la formule

$$
Q(\sum_i a_i e_i) = \sum_{\{i,j\}} b_{ij} a_i a_j,
$$

la dernière sommation étant étendue aux sous-ensembles $\{i, j\}$ de $I$ ayant un ou deux éléments.

En effet, comme la formule (16) n’est qu’une transcription de la formule (14), l’unicité d’une forme quadratique $Q$ vérifiant (15) est démontrée. Pour démontrer son existence, remarquons d’abord qu’il existe une famille $(b'_{ij})$ d’éléments de $A$ telle que $b'_{ii} = b_{ii}$ et que $b'_{ij} + b'_{ji} = b_{ij}$ pour $i \neq j$; on obtient par exemple une telle famille en munissant $I$ d’une structure d’ensemble totalement ordonné (*Ens.*, chap. III, § 2, n° 3, th. 1) et en posant $b'_{ij} = b_{ij}$ pour $i < j$ et $b'_{ij} = 0$ pour $i > j$. Comme les $e_i$ forment une base de $E$, il existe une forme bilinéaire $f$ sur $E \times E$ telle que $f(e_i, e_j) = b'_{ij}$; en posant $Q'(x) = f(x, x)$ et en désignant par $\Phi'$ la forme bilinéaire associée à la forme quadratique $Q'$, on obtient $Q'(e_i) = b_{ii}$ et $\Phi'(e_i, e_j) = f(e_i, e_j) + f(e_j, e_i) = b_{ij}$. Ceci démontre notre seconde assertion. Quant à la première, elle en résulte aussitôt car, en vertu de l’unicité, si une forme quadratique $Q$ vérifie (15), on a $Q(x) = Q'(x) = f(x, x)$.

Le module $E$ muni de la structure définie par une forme quadratique $Q$ prend le nom de *module quadratique*. Un homomorphisme du module quadratique $(E, Q)$ dans un module quadratique $(E', Q')$ est une application linéaire $u$ de $E$ dans $E'$ telle que $Q = Q' \circ u$; si $\Phi$ et $\Phi'$ sont les formes bilinéaires associées à $Q$ et $Q'$, on a alors $\Phi(x, y) = \Phi'(u(x), u(y))$ pour $x \in E,\ y \in E$; autrement dit $\Phi'$ est l’image réciproque de $\Phi$ par $u$ (\S 1, n° 1). On dit que deux formes quadratiques $Q$ et $Q'$ sur deux $A$-modules $E$ et $E'$ sont *équivalentes* si les modules quadratiques correspondants sont isomorphes.

Soit $(E_i, Q_i)_{i \in I}$ une famille de modules quadratiques, et soit $E$ la somme directe des modules $E_i$. On appelle *somme directe externe* des modules quadratiques $(E_i, Q_i)$ le module quadratique obtenu en munissant $E$ de la forme quadratique $Q$ définie par $Q(\sum_i x_i) = \sum_i Q_i(x_i)$ pour $x_i \in E_i$. On dit aussi que la forme quadratique $Q$ est la *somme directe externe* des formes quadratiques $Q_i$.

Si les formes $Q_i$ sont non dégénérées, il en est de même de $Q$.

Soit $Q$ une forme quadratique sur le $A$-module $E$; si $F$ est un sous-module de $E$ et si $Q$ est constante sur chaque classe modulo $F$, l’application $\overline{Q}$ de $E/F$ dans $A$ déduite de $Q$ par passage au quotient est évidemment une forme quadratique, et l’application canonique de $E$ sur $E/F$ est un homomorphisme pour les structures de modules quadratiques. Pour que $Q$ soit constante sur chaque classe modulo $F$, il faut et il suffit que l’on ait $Q(x + y) = Q(x)$ pour $x \in E$ et $y \in F$, c’est-à-dire, en notant $\Phi$ la forme bilinéaire associée à $Q$, que l’on ait $Q(y) + \Phi(x, y) = 0$ pour $y \in F$ et $x \in E$. Faisant $x = 0$, on voit que l’on a $Q(y) = 0$ pour $y \in F$, et donc

$\Phi(x, y) = 0$ pour $x \in E$ et $y \in F$. Autrement dit, si l’on appelle noyau du module quadratique $(E, Q)$ l’ensemble $N$ des éléments $x$ de $E$ tels que $Q(x) = 0$ et $\Phi(x, z) = 0$ pour tout $z \in E$, pour que $Q$ soit constante sur chaque classe modulo $F$, il faut et il suffit que $F$ soit contenu dans le noyau $N$ de $(E, Q)$. On vérifie sans peine que $N$ est un sous-module de $E$. Pour que $Q$ soit constante sur chaque classe modulo $F$, il faut et il suffit donc que $F$ soit engendré par des éléments de $N$.

On voit aussitôt que le noyau du module quadratique $|E/N$ est $\{0\}$.

#### Proposition 3 {#alg-ix-s3-prop-3 .statement}

*Soit $h$ un homomorphisme de $A$ dans un anneau commutatif $A'$. Pour toute forme quadratique $Q$ sur le $A$-module $E$, il existe une forme quadratique $Q'$ et une seule sur le $A'$-module $A' \otimes_A E$ (chap. III, 2e éd., App. II, n° 10) telle que l’on ait*
$$
Q'(1 \otimes x) = h(Q(x))
$$
pour tout $x \in E$. *En outre la forme bilinéaire $\Phi'$ associée à $Q'$ s’obtient par extension de l’anneau des scalaires à partir de la forme bilinéaire $\Phi$ associée à $Q$*.

Montrons d’abord que, s’il existe une forme quadratique $Q'$ vérifiant (17), elle est unique et la forme bilinéaire $\Phi'$ associée à $Q'$ s’obtient par extension de l’anneau des scalaires à partir de la forme $\Phi$ associée à $Q$. En effet cette dernière assertion résulte de ce que l’on a
$$
\Phi'(1 \otimes x, 1 \otimes y) = Q'(1 \otimes x + 1 \otimes y) - Q'(1 \otimes x) - Q'(1 \otimes y)
= h(\Phi(x, y))
$$
pour $x \in E, y \in E$. La formule (14) montre alors que l’on a
$$
Q'(\sum_i a'_i \otimes x_i) = \sum_i a'_i{}^2 h(Q(x_i)) + \sum_{\{i, j\}} a'_i a'_j h(\Phi(x_i, x_j))
$$
pour $a'_i \in A'$ et $x_i \in E$, ce qui démontre l’unicité de $Q'$.

Pour montrer l’existence de $Q'$, nous supposerons d’abord que le module $E$ admet une base $(e_i)_{i \in I}$. Il existe alors des éléments $b_{ij}$ de $A$ tels que $b_{ij} = b_{ji}$ et que $Q(\sum_i a_i e_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$ pour $a_i \in A$ (prop. 2). Comme les éléments $1 \otimes_A e_i$ forment une base du

A'-module $A' \otimes_A E$, on définit une forme quadratique $Q'$ sur ce dernier module en posant
$$
Q'(\sum_i a'_i \otimes e_i) = \sum_{\{i,j\}} a'_i a'_j h(b_{ij})
$$
pour $a'_i \in A'$; d’où, pour $x = \sum_i a_i e_i \in E$
$$
Q'(1 \otimes x) = Q'(\sum_i h(a_i) \otimes e_i) = \sum_{\{i,j\}} h(a_i) h(a_j) h(b_{ij}) = h(Q(x)),
$$
ce qui démontre l’existence de $Q'$ dans ce cas.

Passons maintenant au cas général. Soient $(x_i)_{i \in I}$ un système de générateurs de $E$, $A^{(t)}$ le module des combinaisons linéaires formelles d’éléments de $I$ (chap. II, § 1, n° 8), et $(e_i)_{i \in I}$ la base canonique de $A^{(t)}$. L’application linéaire $u$ de $A^{(t)}$ dans $E$ définie par $u(e_i) = x_i$ est surjective puisque les éléments $x_i$ engendrent $E$. Il en résulte (chap. III, 2e éd., App. II, n° 5, prop. 4) que l’application $1 \otimes u$ de $A' \otimes A^{(t)}$ dans $A' \otimes E$ est surjective, et que son noyau $P'$ est engendré par les éléments de la forme $1 \otimes p$ avec $u(p) = 0$. Soit alors $Q'_1$ l’extension à $A' \otimes_A A^{(t)}$ de la forme quadratique $Q_1 = Q \circ u$ sur $A^{(t)}$. Si $p$ est un élément de $A^{(t)}$ tel que $u(p) = 0$, on a $Q'_1(1 \otimes p) = h(Q_1(p)) = 0$ et (en notant $\Phi'_1$ la forme bilinéaire associée à $Q'_1$) $\Phi'_1(1 \otimes p, 1 \otimes x) = h(\Phi(u(p), u(x))) = 0$ pour tout $x \in A^{(t)}$. Donc, si $u(p) = 0$ ($p \in A^{(t)}$), alors $1 \otimes p$ appartient au noyau du module quadratique $A' \otimes_A A^{(t)}$, et il existe par suite, comme on l’a vu plus haut, une forme quadratique $Q'$ sur $A' \otimes_A E$ telle que $Q'_1 = Q' \circ (1 \otimes u)$. Comme $u$ est surjective, on voit que $Q'$ vérifie la condition (17). CQFD.

La forme quadratique $Q'$, dont l’existence et l’unicité sont assurées par la prop. 3, est appelée l’extension de $Q$ à $A' \otimes_A E$ (par rapport à $h$). On dit aussi que $Q'$ s’obtient à partir de $Q$ par extension de l’anneau des scalaires.

Exercices. — 1) Soient $A$ un corps, $E$ un espace vectoriel à gauche sur $A$, $\Phi$ une forme sesquilinéaire sur $E$ (pour un antiautomorphisme $J$ de $A$). On suppose que le rang (fini ou infini) de $\Phi$ est $\geqslant 2$, et que les relations $\Phi(x, y) = 0$ et $\Phi(y, x) = 0$ sont équivalentes.
a) Montrer qu’il existe $\lambda \neq 0$ dans $A$ tel que l’on ait $\Phi(y, x) = \lambda (\Phi(x, y))^J$. (Utiliser l’exerc. 8 du § 1).
b) Montrer qu’il existe $\alpha \in A$ tel que la forme sesquilinéaire $\Phi \alpha$ (pour l’antiautomorphisme $\xi \to \alpha^{-1} \xi^J \alpha$) soit hermitienne ou alternée.

(Remarquer d’abord que l’on a $\xi^{J^2} = \lambda^{-1} \xi \lambda^{-J}$ et $\lambda \lambda^J = \lambda^J \lambda = 1$. Distinguer ensuite deux cas suivant que $\xi + \xi^J \lambda^{-1} = 0$ pour tout $\xi \in A$ ou non ; dans le second cas, montrer que tout élément $\neq 0$ de la forme $\alpha = \xi + \xi^J \lambda^{-1}$ répond à la question).

2) Soit $\Phi$ une forme sesquilinéaire $\varepsilon$-hermitienne sur un espace vectoriel $E$ de dimension finie sur un corps $A$.

a) Montrer que pour tout sous-espace vectoriel $M$ de $E$, on a $(M^0)^0 = M + E^0$ et $\dim M^0 + \dim M = \dim E + \dim (M \cap E^0)$.

b) Si $M_1, M_2$ sont deux sous-espaces vectoriels de $E$, montrer que l’on a $\dim (M_1 \cap M_2^0) + \dim (M_2 + M_1^0) = \dim E + \dim (M_1 \cap E^0)$ (considérer l’application canonique de $E$ sur $E/E^0$).

3) Soient $K$ un anneau commutatif, $f$ un polynôme unitaire de $K[X]$, de degré $n \geqslant 1$; soit $A$ l’algèbre quotient $K[X]/(f)$ admettant pour base sur $K$ les éléments $1, \xi, \xi^2, \ldots, \xi^{n-1}$ (chap. IV, § 1, no 5, prop. 4). Montrer que la donnée d’un $A$-module $E$ équivaut à la donnée d’un $K$-module $E_0$ et d’un $K$-endomorphisme $j$ de $E_0$ tel que $f(j) = 0$. Pour tout $u \in E^*$, on pose $u(x) = \sum_{k=0}^{n-1} u_k(x) \xi^k$; montrer que si $\alpha_0 = f(0)$ est inversible dans $K$, l’application $u \to u_0$ est un $K$-isomorphisme de $E^*$ sur $(E_0)^*$, dont on explicitera l’isomorphisme réciproque.

¶ 4) a) Soient $A$ un anneau (commutatif ou non), $\sigma$ un automorphisme de $A$ tel qu’il existe un élément inversible $\gamma \in A$ vérifiant $\gamma^\sigma = \gamma$, et tel que l’on ait $\xi^{\sigma^2} = \gamma \xi \gamma^{-1}$ pour tout $\xi \in A$. Soit $B$ un $A$-module à gauche ayant une base de deux éléments $(e_1, e_2)$; montrer qu’on définit sur $B$ une structure d’anneau en prenant comme multiplication dans $B$ la loi de composition

$$
(\xi e_1 + \eta e_2)(\xi' e_1 + \eta' e_2) = (\xi \xi' + \eta \eta' \gamma) e_1 + (\eta \xi'^\sigma + \xi \eta') e_2.
$$

Pour cette structure d’anneau, $e_1$ est élément unité (qu’on identifie avec l’élément unité 1 de $A$); si on pose $e_2 = \rho$, on a $\rho^2 = \gamma$ et $\rho \xi = \xi^\sigma \rho$ pour tout $\xi \in A$; en outre, $B$ est un $A$-module à droite, dont 1 et $\rho$ forment une base. Si $A$ est un corps, une condition nécessaire et suffisante pour que $B$ soit un corps est que $\gamma$ ne soit pas de la forme $\lambda^\sigma \lambda$ (où $\lambda \in A$). (Cf. chap. VIII, § 12, exerc. 8).

b) Soit $J$ un antiautomorphisme involutif de $A$. On suppose qu’il existe un élément inversible $\delta \in A$ satisfaisant aux conditions suivantes :

(1) $\delta^J = \delta, \quad \delta^\sigma \delta = \gamma \gamma^J, \quad (\xi^J)^\sigma = \delta (\xi^\sigma)^J \delta^{-1}$ pour tout $\xi \in A$.

Montrer qu’on peut alors prolonger $J$ en un antiautomorphisme involutif de $B$ (noté encore $J$) en posant

(2) $$ (\xi + \eta \rho)^J = \xi^J + \gamma^{-1} \delta^\sigma (\eta^J)^\sigma \rho. $$

Si en outre $A$ et $B$ sont des corps et si $\sigma$ n’est pas un automorphisme intérieur, montrer que les conditions (1) sont nécessaires pour l’existence d’un prolongement de $J$ en un antiautomorphisme involutif de $B$ (en posant $\rho^J = \alpha + \beta \rho$, avec $\alpha, \beta$ dans $A$, montrer qu’on a nécessairement $\alpha = 0$, en écrivant la condition $(\rho \xi)^J = \xi^J \rho^J$ pour tout $\xi \in A$).

c) On suppose les conditions (1) vérifiées et l’antiautomorphisme involutif J prolongé à B par (2). Soient F un B-module unitaire, E le A-module unitaire déduit de F par restriction à A de l’anneau des scalaires ; l’application $j : x \to \rho x$ est alors une application semi-linéaire bijective de E sur lui-même, relative à l’automorphisme $\sigma$ de A et telle que $j^2(x) = \gamma x$. Soit $\Phi$ une forme hermitienne sur F (pour J) ; pour $x \in E$, $y \in E$, posons $\Phi(x, y) = \Phi_1(x, y) + \Phi_2(x, y)\rho$, où $\Phi_1(x, y) \in A$, $\Phi_2(x, y) \in A$. Montrer que $\Phi_1$ est une forme hermitienne sur E (pour J), telle que
$$
\Phi_1(j(x), j(y)) = (\Phi_1(x, y))^{\sigma \delta};
$$
on a $\Phi_2(x, y) = \Phi_1(x, j(y))\delta^{-1}$, $\Phi_2$ est une forme sesquilinéaire sur E pour l’antiautomorphisme (en général non involutif) $\xi \to (\xi^J)^{\sigma}$, telle que
$$
\Phi_2(j(x), j(y)) = (\Phi_2(x, y))^{\sigma \delta^{\sigma}}
$$
et
$$
\Phi_2(y, x) = \gamma^J \delta^{-1}((\Phi_2(x, y))^J)^{\sigma}.
$$

Réciproques. Pour que $\Phi$ soit non dégénérée, il faut et il suffit que $\Phi_1$ ou $\Phi_2$ soit non dégénérée. Cas particulier où B est une algèbre de quaternions sur un anneau commutatif K, correspondant à une couple $(\alpha, \beta)$ d’éléments de K, $\beta$ étant inversible, A la sous-algèbre $K + Ku$ de B, et J et $\sigma$ l’application $\xi \to \bar{\xi}$ (chap. II, § 7, no 8).

d) Soit $u$ un automorphisme du A-module E. Pour que $u$ soit un automorphisme du B-module F, laissant invariante la forme $\Phi$, il faut et il suffit que $u$ satisfasse à deux quelconques des trois conditions suivantes :
1° $u$ laisse invariante $\Phi_1$;
2° $u$ laisse invariante $\Phi_2$;
3° $u$ permuté avec $j$.

5) Soient A un anneau commutatif, E un A-module, $(x_i)_{i \in I}$ un système de générateurs de E ; soit R le sous-module du module $A^{(1)}$ formé des éléments $(y_i)_{i \in I}$ tels que $\sum_i y_i x_i = 0$, et soit $(a_{\lambda})_{\lambda \in L}$ un système de générateurs de R (avec $a_{\lambda} = (a_{\lambda i})_{i \in I}$). Soit $(b_{ij})$ une famille d’éléments de A $(i \in I, j \in I)$. Pour qu’il existe une forme quadratique Q telle que $Q(x_i) = b_{ii}$ et $\Phi(x_i, x_j) = b_{ij}$ pour $i \neq j$ ($\Phi$ désignant la forme bilinéaire associée à Q), il faut et il suffit que $b_{ij} = b_{ji}$ quels que soient $i, j$ dans I, et que, quels que soient $\lambda \in L$ et $i \in I$, on ait
$$
\sum_{\{i, j\}} b_{ij} a_{\lambda i} a_{\lambda j} = \sum_{j \neq i} b_{ij} a_{\lambda j} + 2b_{ii} a_{\lambda i} = 0;
$$
on a alors $Q(\sum a_i x_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$. En déduire une nouvelle démonstration de la prop. 3 du no 4. (Remarquer que les $x'_i = 1 \otimes x_i$ forment un système de générateurs de $A' \otimes_A E$, et que le $A'$-module $A' \otimes_A E$ est isomorphe à $A'^{(1)}/R'$, où $A'^{(1)}$ est identifié à $A' \otimes_A A^{(1)}$ et $R'$ est engendré par l’image de R par l’application canonique de $A^{(1)}$ dans $A'^{(1)}$.

6) Soient $A$ un anneau commutatif de caractéristique 2, $E$ un $A$-module libre, $\mathcal{A}$ (resp. $\mathcal{S}$, $\mathcal{Q}$) le $A$-module des formes bilinéaires alternées (resp. bilinéaires symétriques, quadratiques) sur $E$. On a $\mathcal{A} \subset \mathcal{S}$; on définit en outre une application linéaire $\omega$ de $\mathcal{S}$ dans $\mathcal{Q}$, et une application linéaire $\theta$ de $\mathcal{Q}$ dans $\mathcal{A}$ de la façon suivante : pour toute forme bilinéaire $\Phi \in \mathcal{S}$, $\omega(\Phi)$ est la forme quadratique $x \to \Phi(x, x)$, et pour toute forme quadratique $Q \in \mathcal{Q}$, $\theta(Q)$ est la forme bilinéaire associée à $Q$, qui est alternée. Montrer que $\omega(0) = \mathcal{A}$, $\theta(\mathcal{Q}) = \mathcal{A}$ et $\theta(0) = \omega(\mathcal{S})$.

¶ 7) Soient $A$ un anneau commutatif, $E, F$ deux $A$-modules. On dit qu’une application $Q$ de $E$ dans $F$ est *quadratique* si elle satisfait aux conditions suivantes : $1^\circ$ $Q(\alpha x) = \alpha^2 Q(x)$ pour $\alpha \in A, x \in E$; $2^\circ$ l’application $(x, y) \to Q(x + y) - Q(x) - Q(y)$ de $E \times E$ dans $F$ est bilinéaire. Si $f$ est une application linéaire d’un $A$-module $E_1$ dans $E$, $Q \circ f$ est une application quadratique de $E_1$ dans $F$.

$a)$ Soient $E$ un $A$-module, $A^{(E)}$ le module des combinaisons linéaires formelles des éléments de $E$ à coefficients dans $A$ (chap. II, § 1, no 8), et pour tout $x \in E$, soit $\varepsilon_x$ l’élément correspondant de la base canonique de $A^{(E)}$. Soit $\Gamma^2(E)$ le quotient de $A^{(E)} \times (E \otimes_A E)$ par le sous-module $R$ engendré par les éléments $(\varepsilon_{x+y} - \varepsilon_x - \varepsilon_y, -x \otimes y)$ et $(\varepsilon_{\lambda x} - \lambda^2 \varepsilon_x, 0)$, pour $x \in E, y \in E, \lambda \in A$. Pour tout $x \in E$, on pose $\gamma(x) = \varphi(\varepsilon_x, 0)$, en désignant par $\varphi$ l’application canonique de $A^{(E)} \times (E \otimes E)$ sur $\Gamma^2(E)$; on dit que $\gamma$ est l'*application canonique* de $E$ dans $\Gamma^2(E)$. Montrer que $\gamma$ est une application quadratique de $E$ dans $\Gamma^2(E)$ et que, pour toute application quadratique $Q$ de $E$ dans un $A$-module $F$, il existe une application *linéaire* et une seule $q$ de $\Gamma^2(E)$ dans $F$ telle que $Q = q \circ \gamma$ (en d’autres termes, $(\Gamma^2(E), \gamma)$ est solution d’un problème d’application universelle ; cf. *Ens.*, chap. IV, § 3).

Pour tout couple de $A$-modules $E, E'$ et toute application linéaire $f$ de $E$ dans $E'$, montrer que, si $\gamma'$ désigne l’application canonique de $E'$ dans $\Gamma^2(E')$, il existe une et une seule application linéaire $\bar{f}$ de $\Gamma^2(E)$ dans $\Gamma^2(E')$ telle que $\gamma' \circ f = \bar{f} \circ \gamma$.

$b)$ On suppose que $E$ est somme directe de deux sous-modules $M, N$. Définir un isomorphisme canonique de $\Gamma^2(E)$ sur la somme directe des modules $\Gamma^2(M), \Gamma^2(N)$ et $M \otimes N$ (montrer que cette somme directe est solution du même problème d’application universelle que $\Gamma^2(E)$).

$c)$ Soient $F$ un sous-module de $E$, $j$ l’injection canonique de $F$ dans $E$. Définir un isomorphisme canonique de $\Gamma^2(E/F)$ sur

$$
\Gamma^2(E)/(\bar{j}(\Gamma^2(F)) + \psi(E \times F)),
$$

où $\psi(x, y) = \varphi(0, x \otimes j(y))$ pour $x \in E, y \in F$. (Même méthode).

$d)$ Soient $A'$ un anneau commutatif, $h$ un homomorphisme de $A$ dans $A'$. Définir un isomorphisme canonique de $\Gamma^2(A' \otimes_A E)$ sur $A' \otimes_A \Gamma^2(E)$ (même méthode).

$e)$ Il existe une application linéaire et une seule $s$ de $\Gamma^2(E)$ dans $E \otimes E$ telle que $s(\gamma(x)) = x \otimes x$ pour tout $x \in E$; montrer que si $E$ est un module libre, s est un isomorphisme sur le sous-module des tenseurs symétriques d’ordre 2 sur E.

f) On suppose que $A = \mathbf{Z}$ et que E est un groupe cyclique fini d’ordre n. Montrer que $\Gamma^2(E)$ est un groupe cyclique d’ordre n si n est impair, d’ordre $2n$ si n est pair. (Remarquer d’abord que si a est un générateur de E, $\gamma(a)$ est un générateur de $\Gamma^2(E)$, et que $\gamma(-ha) = \gamma(ha)$ pour tout entier h ; déduire de là que si n est impair, $n\gamma(a) = 0$ en prenant $h = (n-1)/2$; montrer de même que $2n\gamma(a) = 0$ si n est pair. Prouver enfin que si n est impair (resp. pair), il existe une application quadratique Q de E dans un groupe cyclique d’ordre n (resp. $2n$) appliquant a sur un générateur de ce groupe).

8) Soient A un corps commutatif, E, F deux espaces vectoriels sur A. Soit g une application de E dans F, telle qu’il existe trois applications $a, b, c$ de $E \times E$ dans F, satisfaisant à l’identité

$$
g(\lambda x + \mu y) = \lambda^2 a(x, y) + \lambda \mu b(x, y) + \mu^2 c(x, y)
$$

quels que soient $x, y$ dans E, $\lambda, \mu$ dans A.

a) Montrer que l’on a $a(x, y) = g(x), c(x, y) = g(y), b(y, x) = b(x, y)$ et $b(\lambda x, y) = \lambda b(x, y)$; en outre, si on pose

$$
d(x, y, z) = b(x + y, z) - b(x, z) - b(y, z)
$$

montrer que l’on a $d(x, y, z) = d(y, z, x) = d(z, x, y)$ et en conclure que $d(\lambda x, \mu y, v z) = \lambda \mu v d(x, y, z)$.

b) Déduire de a) que si $A \neq \mathbf{F}_2$, on a nécessairement $d(x, y, z) = 0$ et par suite que g est une application quadratique (exerc. 7). Au contraire, si $A = \mathbf{F}_2$ et si dim E $\geqslant 3$, montrer qu’il existe des applications g de E dans A, satisfaisant à (4) et pour lesquelles $d(x, y, z)$ ne soit pas identiquement nul.

9) Soient A un anneau commutatif, E un A-module ayant une base de n éléments, $\Phi$ une forme bilinéaire symétrique sur E. Soient e un élément de $\bigwedge^n E$ formant une base de ce module, $\Delta$ le discriminant de $\Phi$ par rapport à e, $\varphi_p$ l’isomorphisme canonique de $\bigwedge^p E$ sur $\bigwedge^{n-p} E^*$ relatif à e (chap. III, § 8, no 5). Pour $x \in \bigwedge^p E$, soit $d_{(p)}(x) = \varphi_{n-p}^{-1}(d_{\Phi_{(p)}}(x))$; montrer que l’application $d_{(p)}$ de $\bigwedge^p E$ dans $\bigwedge^{n-p} E$ possède les propriétés suivantes :

a) Pour tout $x \in \bigwedge^p E$, $d_{(n-p)}(d_{(p)}(x)) = (-1)^{p(n-p)} \Delta x$.

b) Pour tout couple d’éléments $x, y$ de $\bigwedge^p E$, on a

$$
x \wedge d_{(p)}(y) = \Phi_{(p)}(x, y)e \quad \text{et} \quad \Phi_{(n-p)}(d_{(p)}(x), d_{(p)}(y)) = \Delta \Phi_{(p)}(x, y).
$$

c) On suppose en outre que A soit un corps et que $\Phi$ soit non dégénérée. Alors, si x est un p-vecteur décomposable $\neq 0$ correspondant à un sous-espace F de E (chap. III, § 7, no 3), $d_{(p)}(x)$ est un $(n-p)$-vecteur décomposable $\neq 0$ correspondant au sous-espace $F^0$ orthogonal à F.

d) Étendre les résultats précédents au cas où (A étant un anneau commutatif), Φ est une forme sesquilinéaire ε-hermitienne pour un automorphisme involutif J ≠ 1 de A.

10) a) Soient A un anneau commutatif, E un A-module ayant une base de 3 éléments, Φ une forme bilinéaire symétrique sur E. Avec les notations de l’exerc. 9, pour deux éléments quelconques x, y de E, on pose $x \overline{\wedge} y = d_{(2)}(x \wedge y)$, et on dit que cet élément est le produit vectoriel de x et de y (relativement à Φ et à la base e de $\bigwedge^3 E$). Montrer que $(x, y) \to x \overline{\wedge} y$ est une application bilinéaire alternée de $E \times E$ dans E, et que $x \overline{\wedge} y$ est orthogonal à x et à y.

b) Soient α, β deux éléments inversibles de A, B l’algèbre de quaternions sur A correspondant au couple ($α, β$) (chap. II, § 7, n° 8), 1, u, v, ω la base canonique de B sur A ; soit E le sous-module de B ayant pour base u, v, ω. Montrer que si x, y sont deux quaternions appartenant à E, on a
$$
xy = \Phi(x, y) + x \overline{\wedge} y
$$
où Φ est une forme bilinéaire symétrique sur E, telle que les applications linéaires associées à Φ soient bijectives, et $x \overline{\wedge} y$ est le produit vectoriel de x et de y relatif à la forme Φ et à la base $α^{-1}β^{-1}u \wedge v \wedge ω$ de $\bigwedge^3 E$.

11) Soit Φ une forme sesquilinéaire ε-hermitienne non dégénérée sur un espace vectoriel E de dimension finie. On dit qu’un sous-espace vectoriel M de E est faiblement orthogonal à un sous-espace vectoriel N (relativement à Φ) si l’un des deux sous-espaces M, N° contient l’autre.

a) Montrer que la relation « M est faiblement orthogonal à N » est symétrique.

b) Si M et N sont faiblement orthogonaux, M° et N° sont faiblement orthogonaux.

c) Si M et N sont faiblement orthogonaux et si $M \cap N = \{0\}$, M et N sont orthogonaux.
