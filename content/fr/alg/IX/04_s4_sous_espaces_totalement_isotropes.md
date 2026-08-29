---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 4
section_title: Sous-espaces totalement isotropes. Théorème de Witt
lang: fr
source: alg-ix-fr
pdf_pages: 0061-0077
extraction: ocr
subsections:
    - "no": 1
      title: Sous-espaces isotropes.
      page: 0
      pdf_page: 62
    - "no": 2
      title: Décomposition de Witt.
      page: 0
      pdf_page: 63
    - "no": 3
      title: Théorème de Witt.
      page: 0
      pdf_page: 69
statements: 17
exercises: 0
content_sha256: 14cb4de3331001e2cca71f8cafa3a3f182c71b7b91d8265d6f9b975bebdddf14
---

## § 4. Sous-espaces totalement isotropes. Théorème de Witt

Dans ce paragraphe on suppose, sauf mention expresse du contraire, que A est un corps. On désigne par Φ, soit une forme ε-hermitienne sur E (par rapport à l’antiautomorphisme involutif $λ \to \overline{λ}$ de A), soit la forme bilinéaire symétrique associée à une forme quadratique Q sur E (A étant supposé commutatif dans ce dernier cas).

### 1. Sous-espaces isotropes.

#### Définition 1 {#alg-ix-s4-def-1 .statement}

Etant donné un module E sur l’anneau A, un élément x de E est dit isotrope si $\Phi(x, x) = 0$. Un sous-module F de E est dit
    1) isotrope s’il existe un élément $x \neq 0$ de F orthogonal à F ;
    2) totalement isotrope si la restriction de $\Phi$ à F est nulle.

Lorsque le module E est muni d’une forme quadratique Q, on dira qu’un élément de E est isotrope (resp. qu’un sous-module de E est isotrope, ou totalement isotrope) si cet élément est isotrope (resp. si ce sous-module est isotrope, ou totalement isotrope) relativement à la forme bilinéaire associée à Q.

Un vecteur isotrope n’est autre qu’un vecteur orthogonal à lui-même. Dire qu’un sous-module F est isotrope signifie que $F \cap F^0 \neq \{0\}$, ou encore que la restriction de $\Phi$ à F est dégénérée ; un sous-module non isotrope G de E est donc un sous-module tel que la restriction de $\Phi$ à G est non dégénérée. Pour qu’un sous-module F de E soit totalement isotrope, il faut et il suffit que l’on ait $F \subset F^0$. Si F est un sous-module totalement isotrope de E, il en est de même de tout sous-module $F'$ contenu dans F. La somme d’une famille de sous-modules totalement isotropes et orthogonaux deux à deux est un sous-module totalement isotrope. L’ensemble des sous-modules totalement isotropes de E, ordonné par inclusion, est évidemment inductif ; il en résulte que tout sous-module totalement isotrope est contenu dans un sous-module totalement isotrope maximal.

#### Proposition 1 {#alg-ix-s4-prop-1 .statement}

On suppose que A est un corps. Soit F un sous-espace non isotrope de dimension finie de E ; alors E est somme directe de F et de $F^0$.

En effet, comme la restriction $\Phi'$ de $\Phi$ à F est non dégénérée par hypothèse, l’application $d_{\Phi'}$ de F dans son dual $F^*$ associée à droite à $\Phi'$ est injective, donc bijective puisque F et $F^*$ sont deux espaces de même dimension finie. Par suite, pour tout $y \in E$, il existe un élément $y_0$ et un seul de F tel que l’on ait $\Phi(x, y) = \Phi(x, y_0)$ pour tout $x \in F$, c’est-à-dire $y - y_0 \in F^0$ ; ceci prouve que E est somme directe de F et $F^0$.

#### Corollaire {#alg-ix-s4-n1-cor-1 .statement}

Si F est un sous-espace de dimension finie de E, et si Φ est non dégénérée, les conditions suivantes sont équivalentes :

a) F est non isotrope.
b) F^0 est non isotrope.
c) E est somme directe de F et F^0.

La prop. 1 montre en effet que a) implique c), et c) implique a) et b). Enfin, si F^0 est non isotrope, on a F ∩ F^0 ⊂ F^0 ∩ F^{00} = {0}; donc F est non isotrope, ce qui montre que b) implique a).

#### Définition 2 {#alg-ix-s4-def-2 .statement}

Soit Q une forme quadratique sur E. Un élément x de E est dit singulier (relativement à Q) si Q(x) = 0. Un sous-module F de E est dit :
1) singulier s’il existe un élément x ≠ 0 de F qui est singulier et orthogonal à F ;
2) totalement singulier si la restriction de Q à F est nulle.

Le noyau du module quadratique (E, Q) (§ 3, n° 4) est constitué par les éléments singuliers de E^0 ; pour qu’un sous-module F soit singulier, il faut et il suffit que son noyau soit ≠ {0}. Comme Φ(x, y) = Q(x + y) − Q(x) − Q(y), tout sous-module totalement singulier ≠ {0} est singulier. Comme Φ(x, x) = 2Q(x), tout vecteur singulier est isotrope et tout sous-module singulier (resp. totalement singulier) est isotrope (resp. totalement isotrope) ; la réciproque est vraie si A est un corps de caractéristique ≠ 2. Tout sous-module contenu dans un sous-module totalement singulier est lui-même totalement singulier. La somme d’une famille de sous-modules totalement singuliers et orthogonaux deux à deux est un sous-module totalement singulier. L’ensemble des sous-modules totalement singuliers de E, ordonné par inclusion, est inductif ; donc tout sous-module totalement singulier de E est contenu dans un sous-module totalement singulier maximal.

### 2. Décomposition de Witt.

Aux conventions déjà en vigueur depuis le début du présent paragraphe, nous ajouterons la suivante :

Bourbaki XXIV.

CONDITION (T). — Pour tout $x \in E$, il existe $\alpha \in A$ tel que $\Phi(x, x) = \alpha + \varepsilon \bar{\alpha}$.

Cette condition est toujours satisfaite lorsque $\Phi$ est alternée, ou lorsque $\varepsilon = 1$ et que $A$ est un corps de caractéristique $\neq 2$, en prenant alors $\alpha = \frac{1}{2} \Phi(x, x)$ (cf. exerc. 1 et 14).

#### Lemme 1 {#alg-ix-s4-lem-1 .statement}

Soit $\Phi$ une forme $\varepsilon$-hermitienne vérifiant (T) (resp. la forme bilinéaire associée à une forme quadratique Q) sur $E$, et soit F un sous-espace totalement isotrope (resp. totalement singulier) de $E$, non réduit à 0. Pour tout $x \in E$ non orthogonal à F et tout $\alpha \in A$, il existe $y \in F$ tel que

$$
\Phi(x + y, x + y) = \alpha + \varepsilon \bar{\alpha} \quad (\text{resp. } Q(x + y) = \alpha).
$$

Posons en effet $\Phi(x, x) = \beta + \varepsilon \bar{\beta}$ (resp. $Q(x) = \beta$). Pour $y \in F$ on a alors $\Phi(x + y, x + y) = (\beta + \Phi(x, y)) + \varepsilon (\beta + \Phi(x, y))$ puisque $\Phi(y, y) = 0$ (resp. $Q(x + y) = \beta + \Phi(x, y)$ puisque $Q(y) = 0$). Comme $x$ n’est pas orthogonal à F, la fonction linéaire affine $y \to \Phi(x, y) + \beta$ sur F n’est pas constante ; elle prend donc la valeur $\alpha$ pour un certain élément $y$ de F, qui répond ainsi à la question.

On appelle décomposition de Witt de E toute décomposition de E en somme directe de trois sous-espaces F, F', G tels que F et F' soient totalement isotropes (resp. totalement singuliers) et que G soit non isotrope et soit orthogonal à $F + F'$; si E est de dimension finie, la matrice de $\Phi$ par rapport à une base de E adaptée à une décomposition de Witt de E se met sous la forme

$$
\begin{pmatrix}
0 & U & 0 \\
\varepsilon \overline{U} & 0 & 0 \\
0 & 0 & V
\end{pmatrix}
$$

(1)

On dit que $\Phi$ est une forme neutre si elle est non dégénérée et si E est de dimension finie et est somme directe de deux sous-espaces totalement isotropes (resp. totalement singuliers). La somme directe de deux formes neutres est une forme neutre.

#### Proposition 2 {#alg-ix-s4-prop-2 .statement}

Soit $\Phi$ une forme $\varepsilon$-hermitienne non dégénérée vérifiant (T) (resp. la forme bilinéaire associée à une forme quadratique non dégénérée Q), et soit F un sous-espace totalement isotrope (resp. totalement singulier) de dimension finie r.

a) Si $F'$ est un sous-espace totalement isotrope de dimension r tel que $F' \cap F^0 = \{0\}$, alors $F + F'$ est non isotrope et, pour toute base $(f_i)$ de F, il existe une base $(f'_i)$ de $F'$ telle que $\Phi(f_i, f'_j) = \delta_{ij}$ (indice de Kronecker) pour $i, j = 1, \ldots, r$.

b) Si G est un sous-espace totalement isotrope (resp. totalement singulier) de dimension $\leq r$ tel que $G \cap F^0 = \{0\}$, il existe un sous-espace totalement isotrope (resp. totalement singulier) $F' \supset G$ de dimension r tel que $F' \cap F^0 = \{0\}$.

Soit $\Psi$ la restriction de $\Phi$ à $F \times F'$; pour $x' \in F'$, la relation «$\Phi(x, x') = 0$ pour tout $x \in F$ » entraîne $x = 0$ puisque $F' \cap F^0 = \{0\}$. L’assertion a) résulte alors du cor. de la prop. 6 du § 1, n° 6, à l’exception du fait que $F + F'$ est non isotrope. Or le sous-espace $H = (F + F') \cap (F + F')^0$ est égal à $(F + F') \cap F^0 \cap {F'}^0$. Comme $F \subset F^0$, on a $(F + F') \cap F^0 = F + (F' \cap F^0) = F$, d’où $H = F \cap {F'}^0$; donc $H = \{0\}$ puisqu’on a vu que $\Psi$ est non dégénérée. Ceci prouve bien que $F + F'$ est non isotrope.

Pour démontrer b), nous procéderons par récurrence descendante sur $s = \dim G$. Il nous suffit ainsi de prouver que, si $s < r$, il existe un sous-espace totalement isotrope (resp. totalement singulier) $G'$ contenant G, de dimension $s + 1$, et tel que $G' \cap F^0 = \{0\}$. Comme $\dim G < \dim F$, la restriction de $\Phi$ à $F \times G$ est dégénérée, et comme $G \cap F^0$ est nul, $F \cap G^0$ est non nul. Si l’on avait alors $G + F^0 \supset G^0$, on en déduirait, en prenant les sous-espaces orthogonaux et en remarquant que $F = F^{00}$ et que $G = G^{00}$ ($§ 1$, n° 6, cor. 1 de la prop. 4), que $G^0 \cap F \subset G$, d’où

$$
G^0 \cap F \subset G \cap F \subset G \cap F^0 = \{0\},
$$

ce qui est impossible. Il existe alors un élément $x$ de $G^0$ tel que $x \notin G + F^0$; comme $F \subset F^0$, on peut ajouter à $x$ un vecteur de $G^0 \cap F$ sans modifier ces propriétés; comme $G^0 \cap F$ est totalement isotrope (resp. totalement singulier) et $\neq \{0\}$, le lemme 1 montre qu’on peut choisir $x$ isotrope (resp. singulier).

Alors le sous espace $G' = G + Ax$ est de dimension $s + 1$, et est totalement isotrope (resp. totalement singulier) ; de plus on a $G' \cap F^0 = \{0\}$ car, si $y = z + ax$ ($z \in G,\ a \in A$) est dans $F^0$, on a $a = 0$, car sinon $x \in F^0 + G$ contrairement au choix de $x$, d’où $y = z \in G \cap F^0 = \{0\}$ et $y = 0$. Par conséquent le sous-espace $G'$ répond à la question.

#### Corollaire 1 {#alg-ix-s4-prop-2-cor-1 .statement}

*Si F est un sous-espace totalement isotrope (resp. totalement singulier) de dimension r, il existe un sous-espace totalement isotrope (resp. totalement singulier) F' de dimension r tel que $F \cap F' = \{0\}$ et que $F + F'$ soit non isotrope.*

Il suffit de faire $G = \{0\}$ dans la prop. 2, b).

#### Corollaire 2 {#alg-ix-s4-prop-2-cor-2 .statement}

*Deux formes $\varepsilon$-hermitiennes neutres sur des espaces de même dimension sur A sont équivalentes.*

#### Remarque {#alg-ix-s4-n2-rem-1 .statement}

Dans les conditions du corollaire 1, E est somme directe de $F + F'$ et de l’orthogonal de $F + F'$. On a donc une décomposition de Witt de E. D’après la prop. 2, a), il existe des bases de F et F’ telles que, dans la matrice (1) de $\Phi$, le bloc $U$ soit la matrice unité $1_r$.

#### Proposition 3 {#alg-ix-s4-prop-3 .statement}

*Soit $\Phi$ une forme $\varepsilon$-hermitienne non dégénérée vérifiant (T) (resp. la forme bilinéaire associée à une forme quadratique non dégénérée Q). Soient $F_1$ et $F_2$ deux sous-espaces totalement isotropes (resp. totalement singuliers) maximaux de E, l’un des deux étant de dimension finie. Posons $F = F_1 \cap F_2$. Soit $S_i \ (i = 1, 2)$ un supplémentaire de $F$ dans $F_i$; posons $S = S_1 + S_2$. Il existe alors deux sous-espaces G et H de E tels que
a) Les sous-espaces $G + F, S$ et H sont non isotropes et deux à deux orthogonaux ;
b) E est somme directe de F, S, G et H ;
c) Il n’y a aucun vecteur isotrope (resp. singulier) non nul dans H ;
d) G est totalement isotrope (resp. totalement singulier).
De plus $F_1$ et $F_2$ sont tous deux de dimensions finies et on a dim $F_1 = \dim F_2, \dim G = \dim F, \dim S_1 = \dim S_2, \operatorname{codim} H = 2 \dim F_1$.

Remarquons d’abord que, si $N$ est un sous-espace totalement isotrope (resp. totalement singulier) maximal, alors tout vecteur isotrope (resp. singulier) $x$ orthogonal à $N$ est un élément de $N$, car sinon $N + Ax$ contredirait le caractère maximal de $N$. Donc si, pour $i = 1,\ 2,\ x_i$ est un vecteur isotrope (resp. singulier) de $F_i^0$, on a $x_i \in F_i$. D’autre part, si $y$ est un élément de $S_1$ orthogonal à $S_2$, il est orthogonal à $F_1$ puisque $F_1$ est totalement isotrope, donc à $F$, et par suite à $F_2 = S_2 + F$. Comme $y$ est isotrope (resp. singulier) et qu’il est orthogonal à $F_2$, on a

$$
y \in S_1 \cap F_2 = S_1 \cap F_1 \cap F_2 = S_1 \cap F = \{0\}.
$$

On a donc $S_1 \cap S_2^0 = \{0\}$, et de même $S_2 \cap S_1^0 = \{0\}$. Comme l’un des deux sous-espaces $F_1, F_2$, par exemple $F_1$, est de dimension finie, $S_1$ est de dimension finie, donc $S_1^0$ est de codimension finie ($§ 1, \mathrm{n}^\circ 6, \mathrm{cor.\ 1\ de\ la\ prop.\ 4}$), et par conséquent $S_2$ est de dimension finie puisque $S_2 \cap S_1^0 = \{0\}$; de plus ceci montre que l’on a $\dim S_2 \leqslant \operatorname{codim} S_1^0 = \dim S_1$; de même $\dim S_1 \leqslant \dim S_2$, d’où $\dim S_1 = \dim S_2$. La prop. 2 a) montre alors que $S = S_1 + S_2$ est non isotrope.

Ceci étant, l’orthogonal $N$ de $S$ est non isotrope ($\mathrm{n}^\circ 1, \mathrm{cor.\ de\ la\ prop.\ 1}$) et contient $F$; le cor. 1 de la prop. 2 montre donc qu’il existe un sous-espace $G$ totalement isotrope (resp. totalement singulier) de $N$ tel que $\dim G = \dim F$, que $G \cap F = \{0\}$ et que $G + F$ soit non isotrope. Ainsi d) est vérifiée par $G$. On satisfera alors à a) et b) en prenant pour $H$ l’orthogonal de $G + F$ dans $N$. Quant à c), l’on remarque que, comme $H$ est orthogonal à $F_1 = S_1 + F$, il n’y a aucun vecteur isotrope (resp. singulier) non nul dans $H$ en vertu de ce qui a été remarqué au début de la démonstration et du fait que $H \cap F_1 = \{0\}$. Enfin certaines des assertions relatives aux dimensions ont été démontrées en cours de route ; les autres s’en déduisent trivialement.

#### Corollaire 1 {#alg-ix-s4-prop-3-cor-1 .statement}

Les hypothèses étant celles de la prop. 3, deux sous-espaces totalement isotropes (resp. totalement singuliers) maximaux de dimensions finies ont même dimension. Pour tout sous-espace totalement isotrope (resp. totalement singulier) maximal F de dimension finie, il en existe un autre F' tel que F ∩ F' = {0}, et dans ces conditions F + F' est non isotrope.

Si F ∩ F' = {0}, on aura G = {0} avec les notations de la prop. 3, et F + F' sera non isotrope. Les autres assertions résultent trivialement de la prop. 3 et du cor. 1 de la prop. 2.

#### Corollaire 2 {#alg-ix-s4-prop-3-cor-2 .statement}

Soit Q une forme quadratique non dégénérée sur un espace vectoriel E de dimension finie n sur un corps algébriquement clos A ; il existe alors une base (e_i)_{1 \leq i \leq n} de E telle que

(2)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} \qquad si\ n = 2\nu,
$$

(3)
$$
Q(\sum_{i=1}^{n} x_i e_i) = \sum_{i=1}^{\nu} x_i x_{i+\nu} + x_{2\nu+1}^2 \qquad si\ n = 2\nu + 1.
$$

Soient en effet F_1 et F_2 deux sous-espaces totalement singuliers maximaux tels que F_1 ∩ F_2 = {0} (cor. 1) et soit q leur dimension. On a alors G = {0} avec les notations de la prop. 3. Prenant une base (e_i)_{1 \leq i \leq q} de F_1 et une base (e_i)_{q+1 \leq i \leq 2q} de F_2 telles que Φ(e_i, e_{j+q}) = δ_{ij} pour i, j = 1, ..., q (prop. 2 a)), on voit qu’il suffit de montrer que dim H ≤ 1. Or, si x ∈ H, y ∈ H et si x ≠ 0, l’équation Q(y - ax) = Q(y) - aΦ(x, y) + a^2 Q(x) = 0 a au moins une solution a_0 puisque Q(x) ≠ 0, et l’on a y = a_0 x puisque tout vecteur singulier de H est nul.

#### Définition 3 {#alg-ix-s4-def-3 .statement}

On suppose que E est de dimension finie et que Φ est une forme ε-hermitienne non dégénérée vérifiant (T) (resp. la forme bilinéaire associée à une forme quadratique non dégénérée Q). On appelle indice de Φ (resp. Q) la dimension commune des sous-espaces totalement isotropes (resp. totalement singuliers) maximaux de E.

Si n est la dimension de E et ν l’indice de Φ (resp. Q), la prop. 3 montre que l’on a

(4)
$$
n \geq 2\nu.
$$

De plus, comme tout sous-espace totalement isotrope (resp. totalement singulier) est contenu dans un sous-espace totalement isotrope (resp. totalement singulier) maximal, les sous-espaces totalement isotropes (resp. totalement singuliers) qui sont maximaux sont ceux qui sont de dimension $v$. L’assertion que $\Phi$ (resp. Q) est d’indice 0 signifie que tout vecteur isotrope (resp. singulier) de E est nul. Dans un espace de dimension paire $n$, les formes neutres sont celles d’indice $\frac{1}{2}n$; il n’y a pas de forme neutre dans un espace de dimension impaire. La prop. 3 montre que toute forme est somme directe d’une forme neutre et d’une forme d’indice 0.

#### Proposition 4 {#alg-ix-s4-prop-4 .statement}

*Soit Q une forme quadratique non dégénérée sur E telle qu’il existe un vecteur $x \neq 0$ de E tel que $Q(x) = 0$. Pour tout élément a de A, il existe alors $y \in E$ tel que $Q(y) = a$.*

En effet, d’après le cor. 1 de la prop. 2, il existe un sous-espace $G = F + F'$ ($F, F'$: sous-espaces totalement singuliers de dimension 1) de E, de dimension 2, tel que la restriction de Q à G soit neutre. Si $\{ e, e' \}$ ($e \in F, e' \in F'$) est une base de G, on a
$$
Q(xe + x'e') = bxx' \quad (x \in A, x' \in A, b \in A, b \neq 0).
$$
Il suffit ainsi de prendre pour $y$ le vecteur $ae + b^{-1}e'$.

### 3. Théorème de Witt.

Étant donnés deux espaces vectoriels E, $E'$ sur A munis respectivement de deux formes sesquilinéaires $\Phi, \Phi'$ (resp. de deux formes quadratiques Q, $Q'$), on appelle *homomorphisme métrique* de E dans $E'$ toute application linéaire $u$ de E dans $E'$ telle que $\Phi'(u(x), u(y)) = \Phi(x, y)$ (resp. $Q'(u(x)) = Q(x)$) pour $x \in E, y \in E$. Si E et $E'$ ont même dimension finie et si $\Phi$ (resp. Q) est non dégénérée, tout homomorphisme métrique $u$ de E dans $E'$ est un isomorphisme, car $u(x) = 0$ implique $\Phi(x, y) = 0$ pour tout $y \in E$, donc $x = 0$; ainsi $u$ est injectif, donc bijectif puisque E et $E'$ ont même dimension finie.

**Théorème 1** (Witt). — *Soient E et $E'$ deux espaces vectoriels de dimensions finies, munis respectivement de deux formes $\varepsilon$-hermitiennes non dégénérées $\Phi$ et $\Phi'$ vérifiant la condition (T) du no 2* (resp. de deux formes quadratiques non dégénérées Q et Q'), et isomorphes pour ces structures. Etant donné un sous-espace quelconque F de E, tout homomorphisme métrique injectif de F dans E' se prolonge en un isomorphisme métrique de E sur E'.

En utilisant l’isomorphisme donné de E sur E', on voit qu’il suffit de montrer que tout homomorphisme métrique injectif u de F dans E se prolonge en un automorphisme métrique de E. Remarquons que si, pour i = 1, 2, F_i est un sous-espace de E et u_i un homomorphisme métrique de F_i dans E, tels que F_1 ∩ F_2 = {0} et que Φ(u_1(x_1), u_2(x_2)) = Φ(x_1, x_2) pour x_i ∈ F_i (i = 1, 2), alors l’homomorphisme ψ : x_1 + x_2 → u_1(x_1) + u_2(x_2) de F_1 + F_2 dans E qui prolonge u_1 et u_2 est métrique : en effet, quels que soient x_i, y_i dans F_i (i = 1, 2), le développement de chacune des expressions Φ(x_1 + x_2, y_1 + y_2) et Φ(u_1(x_1) + u_2(x_2), u_1(y_1) + u_2(y_2)) (resp. Q(x_1 + x_2) et Q(u_1(x_1) + u_2(x_2))) contient quatre (resp. trois) termes égaux chacun à chacun d’après les hypothèses faites. De plus, si u_1 et u_2 sont injectifs et si u_1(F_1) ∩ u_2(F_2) = {0}, alors ψ est injectif.

1) Démontrons d’abord le théorème de Witt dans le cas où l’ensemble des points invariants de u est un hyperplan U de F. L’ensemble des vecteurs de la forme u(x) − x avec x ∈ F est alors une droite D. Si F' est un sous-espace orthogonal à D tel que F' ∩ F = F' ∩ u(F) = {0}, on aura Φ(u(x), y) = Φ(x, y) pour x ∈ F et y ∈ F' ; notre remarque initiale s’applique donc à u et à l’application identique de F' dans E, montrant que u se prolonge à F + F' en laissant fixes les points de F' ; l’ensemble des vecteurs de la forme u(x) − x (x ∈ F + F') est encore la droite D. Or on a, pour x ∈ F, y ∈ F

(5) $\Phi(u(x), u(y) - y) = \Phi(u(x), u(y)) - \Phi(u(x), y) = \Phi(x - u(x), y)$,

ce qui, lorsque x ∈ U (c’est-à-dire lorsque u(x) = x), montre que x ∈ D^0 ; autrement dit on a U ⊂ D^0. Nous distinguerons deux cas :

a) $F \not\subset D^0$. La formule (5) montre que $u(F)$ n’est pas contenu dans $D^0$, donc $F \cap D^0 = u(F) \cap D^0 = U$. L’on peut alors prendre pour F' un supplémentaire de U dans D^0 ; comme F + F' contient l’hyperplan D^0 et en est distinct, on a F + F' = E, et on a trouvé dans ce cas le prolongement cherché de u à E.

b) F ⊂ D^0. La formule (5) montre que u(F) ⊂ D^0, et donc que

D ⊂ D^0 ; la droite D est donc isotrope (resp. singulière, car on a Q(u(x) − x) = Q(u(x)) − Φ(x, u(x)) + Q(x) = 2Q(x) − Φ(x, x) = 0 pour x ∈ F). Nous allons montrer que, dans ces conditions, il existe un sous-espace F' de D^0 qui est supplémentaire de F et de u(F) dans D^0. C’est immédiat si F = u(F). Sinon, soient x et y des vecteurs tels que x ∈ F, x ∉ U, y ∈ u(F), y ∉ U ; on a alors F = U + Ax, u(F) = U + Ay, et F ne contient pas x + y sinon y = (x + y) − x appartiendrait à F ∩ u(F) = U ; on voit de même que x + y n’appartient pas à u(F) ; ainsi la droite A(x + y) est supplémentaire de F et de u(F) dans le sous-espace F + u(F) ; il suffit alors de poser F' = A(x + y) + G où G est un supplémentaire de F + u(F) dans D^0. Ceci étant, on a F + F' = u(F) + F' = D^0, et, dans ce cas, ce qui a été dit au début de 1) montre qu’il existe un prolongement de u à l’hyperplan D^0 de E, et que D^0 est stable pour ce prolongement.

On est donc ramené au cas où F est l’hyperplan D^0 et où u est un automorphisme de F. Démontrons que, pour tout z ∈ E, il existe z' ∈ E tel que

(6)
$$
\Phi(u(x), z') = \Phi(x, z)
$$
pour tout x ∈ F ; en effet la forme linéaire x → Φ(u^{-1}(x), z) sur F est restriction d’une forme linéaire sur E, forme qui est du type x → Φ(x, z') puisque Φ est non dégénérée ; donc (6) est valable. De plus, si z ∉ F, il existe un vecteur z' ∈ E vérifiant (6) et tel que Φ(z', z') = Φ(z, z) (resp. Q(z') = Q(z)) : en effet la formule (6) reste valable si l’on ajoute à z' un élément u(y) − y (y ∈ F) de D puisque F = D^0, et le lemme 1 du no 2 permet de conclure puisque z n’est pas orthogonal à D. Notre remarque initiale montre alors qu’il existe un homomorphisme métrique ϕ de F + Az = E dans E qui prolonge u et qui transforme z en z'. Puisque Φ est non dégénérée, ϕ est l’automorphisme métrique de E cherché.

2) Dans le cas général, nous raisonnons par récurrence sur r = dim F. Le cas r = 0 est trivial. Soit alors r > 0, c’est-à-dire F ≠ {0}, et soit U un hyperplan de F. La restriction u_0 de u à U se prolonge, d’après l’hypothèse de récurrence, en un automorphisme métrique ϕ_0 de E. Si ϕ_0 prolonge u, le théorème est démontré. Sinon U est l’ensemble des éléments invariants, par v_0^{-1}u, et il existe , d’après 1), un automorphisme métrique v_1 de E prolongeant v_0^{-1}u. L’automorphisme v_0v_1 est alors le prolongement cherché de u. CQFD.

#### Corollaire 1 {#alg-ix-s4-prop-4-cor-1 .statement}

Soient, pour i = 1, 2, E_i un espace vectoriel de dimension finie, Φ_i une forme ε-hermitienne non dégénérée sur E_i vérifiant (T) (resp. Q_i une forme quadratique non dégénérée sur E_i), E'_i et E''_i deux sous-espaces orthogonaux de E_i dont E_i soit somme directe. Si les formes Φ_1 et Φ_2 (resp. Q_1 et Q_2) sont équivalentes, et si leurs restrictions à E'_1 et E'_2 sont équivalentes, il en est de même de leurs restrictions à E''_1 et E''_2.

En effet, soit u un isomorphisme métrique de E'_1 sur E'_2. D’après le th. 1, u se prolonge en un isomorphisme métrique ϕ de E_1 sur E_2. Comme Φ_i est non dégénérée, E''_i est l’orthogonal de E'_i dans E_i, donc ϕ applique E''_1 sur E''_2. CQFD.

#### Corollaire 2 {#alg-ix-s4-prop-4-cor-2 .statement}

Les hypothèses étant celles du th. 1, le groupe des automorphismes métriques de E permuté transitiivement les sous-espaces totalement isotropes (resp. totalement singuliers) de dimension donnée de E. De plus, si F est un sous-espace totalement isotrope (resp. totalement singulier) de E, toute application linéaire bijective de F sur F est induite par un automorphisme métrique de E.

#### Corollaire 3 {#alg-ix-s4-prop-4-cor-3 .statement}

Soit Q une forme quadratique non dégénérée sur un espace vectoriel E de dimension finie sur un corps algébriquement clos A. Le groupe des automorphismes métriques de E permuté transitiivement les sous-espaces non isotropes de dimension donnée de E.

Ceci résulte immédiatement du th. 1 et du cor. 2 de la prop. 3.

Exercices. — 1) a) Soient K un corps de caractéristique 2, J : ξ → ¯ξ un antiautomorphisme involutif de K, Z le centre de K. Montrer que si la restriction de J à Z n’est pas l’identité, tout élément μ de K tel que ¯μ = μ est de la forme λ + ¯λ (remarquer qu’il y a un élément ρ ≠ 0 dans Z qui s’écrit sous la forme ζ + ¯ζ, avec ζ ∈ Z) ; toute forme hermitienne sur un espace vectoriel sur K satisfait alors à la condition (T).

b) Donner des exemples de corps de caractéristique 2, admettant un antiautomorphisme involutif ξ → ¯ξ distinct de l’application identique, et pour lequel il y ait des éléments $\mu = \bar{\mu}$ qui ne sont pas de la forme $\lambda + \bar{\lambda}$ (cf. chap. VIII, § 11, exerc. 4).

2) Soient A un corps, E un espace vectoriel sur A, $\Phi$ (resp. Q) une forme $\varepsilon$-hermitienne non dégénérée sur E, vérifiant la condition (T) (resp. une forme quadratique non dégénérée sur E, $\Phi$ désignant alors la forme bilinéaire symétrique associée à Q).

a) Montrer que pour qu’un plan $P \subset E$ soit isotrope (resp. singulier) et non totalement isotrope (resp. non totalement singulier), il faut et il suffit qu’il ne contienne qu’une seule droite isotrope (resp. singulière) (cf. exerc. 14 e)).

b) On suppose que dim $E \geqslant 3$, et qu’il existe dans E des vecteurs isotropes $\neq 0$. Montrer que si P est un plan non totalement isotrope dans E, il existe un sous-espace vectoriel non isotrope $V \subset E$, de dimension 3, contenant des vecteurs isotropes $\neq 0$, et tel que $P \subset V$.

3) Les hypothèses étant les mêmes que dans l’exerc. 2, montrer que si dim $E \geqslant 3$, toute droite isotrope dans E est intersection de deux plans non isotropes.

4) Les hypothèses sont celles de l’exerc. 2, et on suppose en outre que E est de dimension finie.

a) Si l’indice $\nu$ de $\Phi$ (resp. Q) est $\geqslant 1$, montrer que pour tout vecteur isotrope (resp. singulier) $a \neq 0$ dans E, il existe une base $(e_i)$ de E formée de vecteurs isotropes (resp. singuliers), telle que $e_1 = a$ (cf. exerc. 14 e)).

b) Soient V, W deux sous-espaces totalement isotropes (resp. totalement singuliers) de même dimension $r \leqslant \nu$; montrer qu’il existe deux sous-espaces totalement isotropes (resp. totalement singuliers) maximaux $V_1, W_1$, tels que $V \subset V_1, W \subset W_1$, et $V_1 \cap W_1 = V \cap W$. (Si $U = V \cap W$, raisonner dans $U^0/U$).

c) Soient V, W, $V_1, W_1$ quatre sous-espaces totalement isotropes (resp. totalement singuliers) de même dimension, tels que $V + W$ et $V_1 + W_1$ soient non isotropes. Montrer qu’il existe un automorphisme métrique $u$ de E tel que $u(V) = V_1$ et $u(W) = W_1$.

d) Soient $f$ une forme linéaire sur E, $\alpha$ un élément de A de la forme $\lambda + \varepsilon \bar{\lambda}$ (resp. un élément de $\Lambda$). On considère la forme sesquilinéaire sur E

$$
(x, y) \to \Phi_1(x, y) = \Phi(x, y) + f(x)\overline{\alpha f(y)}
$$

(resp. la forme quadratique

$$
x \to Q_1(x) = Q(x) + \alpha(f(x))^2).
$$

Montrer que si $\Phi_1$ (resp. $Q_1$) est non dégénérée et si $\nu_1$ désigne son indice, on a $|\nu_1 - \nu| \leqslant 1$.

5) a) Soient B un anneau, $\xi \to \bar{\xi}$ un antiautomorphisme involutif de B, $\varepsilon$ un élément du centre de B tel que $\varepsilon \bar{\varepsilon} = 1$. Montrer que si $\beta$ est un élément inversible de B tel que $\beta + \varepsilon \bar{\beta} \neq 0$, il existe un élément inversible $\mu \neq 1$ dans B, tel que $\mu(\beta + \varepsilon \bar{\beta})\mu = \beta + \varepsilon \bar{\beta}$. (Montrer qu’on peut prendre $\mu$ tel que $\mu \beta \bar{\mu} = \beta$).

b) Soient A un corps, E un espace vectoriel sur A, $\Phi$ une forme sesquilinéaire $\varepsilon$-hermitienne non dégénérée sur $E$, satisfaisant à (T). Montrer que si $\Phi$ n’est pas alternée, pour tout hyperplan non isotrope $H$ de $E$, il existe un automorphisme métrique de $E$, distinct de l’identité, laissant invariant tout élément de $H$ (utiliser $a$).

6) Les hypothèses étant celles de l’exerc. 2, soit $a$ un vecteur isotrope $\neq 0$ dans $E$ (resp. un vecteur isotrope non singulier (on notera que de tels vecteurs n’existent que si $A$ est de caractéristique 2)). Soit $\lambda \in A$ tel que $\lambda + \varepsilon \bar{\lambda} = 0$ (resp. $\lambda = (Q(a))^{-1}$) ; montrer que la transvection $x \to x + \Phi(x, a)\lambda a$ (chap. II, § 6, exerc. 7) est un automorphisme métrique de $E$; réciproque.

7) Les hypothèses étant celles de l’exerc. 2, soit $G$ le groupe des automorphismes métriques de $E$. Montrer que les seules bijections semi-linéaires de $E$ sur lui-même qui permutent avec tous les éléments de $G$ sont les homothéties de $E$, sauf dans les trois cas suivants : dim $E = 2$, $G$ est le groupe des automorphismes métriques correspondant à une forme quadratique d’indice 1 sur $E$, et $A$ est l’un des trois corps $\mathbf{F}_2, \mathbf{F}_3$ ou $\mathbf{F}_4$. (Utiliser les exerc. 5, 6 et 3 ; examiner à part le cas d’une forme quadratique sur un espace vectoriel de dimension 2).

*8) Soient $A$ un corps, $E$ un espace vectoriel de dimension finie $> 0$ sur $A$, $\Phi$ une forme sesquilinéaire $\varepsilon$-hermitienne non dégénérée sur $E$, satisfaisant à (T). Soit $M(\Phi)$ le groupe des multiplicateurs des similitudes de $E$ pour $\Phi$ ($§ 6, \mathrm{n}^o\ 5$).

a) Soient $V_1, V_2$ deux sous-espaces vectoriels de $E$, de même dimension, et soient $\Phi_1, \Phi_2$ les restrictions de $\Phi$ à $V_1, V_2$ respectivement. Pour qu’il existe une similitude $u$ telle que $u(V_1) = V_2$, il faut et il suffit qu’il existe $\alpha \in M(\Phi)$ tel que $\Phi_2$ soit équivalente à $\alpha \Phi_1$ (utiliser le th. de Witt).

b) Soit $(F, F', G)$ une décomposition de Witt de $E$ ($\mathrm{n}^o\ 2$), et soit $\Phi_0$ la restriction de $\Phi$ au sous-espace non isotrope $G$. Montrer que l’on a $M(\Phi) = M(\Phi_0)$ si $G \neq \{0\}$. (Utiliser le th. de Witt et la prop. 2 du $\mathrm{n}^o\ 2$).

c) Montrer que si l’indice $v$ de $\Phi$ est tel que dim $E = 2v$, $M(\Phi)$ est le groupe des éléments $\zeta \neq 0$ du centre de $A$ tels que $\bar{\zeta} = \zeta$. Si dim $E = 2v + 1$, $M(\Phi)$ est le groupe des éléments de la forme $\rho \bar{\rho}$, où $\rho$ parcourt le groupe multiplicatif des éléments $\neq 0$ du centre de $A$ (utiliser le th. de Witt). (Cf. § 10, exerc. 18).*

*9) Soient $A$ un corps commutatif, $E$ un espace vectoriel sur $A$, $Q$ une forme quadratique non dégénérée sur $E$. On appelle similitude pour $Q$ tout automorphisme $u$ de $E$ tel qu’il existe un élément $\alpha \neq 0$ de $A$ pour lequel $Q(u(x)) = \alpha Q(x)$ quel que soit $x \in E$; $u$ est alors aussi une similitude pour la forme bilinéaire associée à $Q$. En supposant la dimension de $E$ finie et $> 0$, énoncer et démontrer pour les similitudes relatives à $Q$ les analogues des résultats de l’exerc. 8.*

*10) Soient $A$ un corps, $E$ un espace vectoriel sur $A$ de dimension $> 2$, $\Phi_1$ (resp. $\Phi_2$) une forme sesquilinéaire non dégénérée $\varepsilon_1$-hermitienne (resp. $\varepsilon_2$-hermitienne) sur $E$ pour un antiautomorphisme involutif $J_1$ (resp. $J_2$) de $A$, vérifiant la condition (T). Montrer que si le groupe des automorphismes métriques de $E$ pour $\Phi_1$ est un sous-groupe du groupe des similitudes pour $\Phi_2$, il existe $\alpha \in A$ tel que $\Phi_2 = \Phi_1 \alpha$ (utiliser les exerc. 5 b) et 6).

Démontrer la propriété analogue lorsque A est supposé commutatif, et que $\Phi_1$ et $\Phi_2$ sont remplacées dans l’énoncé par deux formes quadratiques non dégénérées $Q_1, Q_2$ sur E.*

11) Soient A un anneau, J un antiautomorphisme involutif de A, E un A-module admettant une base finie $(e_i)$, $\Phi$ une forme $\varepsilon$-hermitienne non dégénérée sur E, R la matrice de $\Phi$ par rapport à $(e_i)$; le groupe des automorphismes métriques de $\Phi$ s’identifie au groupe G des matrices inversibles U telles que $^tU . R . U^j = R$.

a) On suppose qu’il existe une matrice P telle que $R = ^tP + \varepsilon P^j$. Montrer que pour toute matrice S telle que $^tS + \varepsilon S^j = 0$, et que $P + S$ soit inversible, $U = (^tP^j - \varepsilon^j S)^{-1}(P + S)$ appartient à G, et $\varepsilon I + U$ est inversible. Réciproque (montrer que pour toute matrice $U \in G$ telle que $\varepsilon I + U$ soit inversible, on a

$$
\varepsilon(\varepsilon I + ^tU)^{-1}R + \varepsilon^j R (\varepsilon^j I + U^j)^{-1} = R.
$$

b) Montrer que la condition de a) est vérifiée lorsque $\Phi$ satisfait à la condition (T). Cas où dans A l’équation $2\xi = \alpha$ admet une solution et une seule pour tout $\alpha \in A$.

¶ 12) Soient A un corps commutatif, E un espace vectoriel de dimension finie n sur A, $\Phi$ une forme sesquilinéaire $\varepsilon$-hermitienne non dégénérée sur E.

a) Soit u un endomorphisme de E ; montrer que si les $r_i (1 \leq i \leq m)$ sont les invariants de similitude de u (chap. VII, § 5, no 1, déf. 1), les invariants de similitude de l’adjoint $u^*$ de u par rapport à $\Phi$ sont les polynômes $\bar{r}_i (1 \leq i \leq m)$, où $\bar{r}_i$ se déduit de $r_i$ en appliquant à chaque coefficient l’automorphisme J (cf. chap. VII, § 5, exerc. 2). Pour tout polynôme unitaire irréductible $p \in A[X]$ divisant le polynôme minimal de u, soit $F_k(u, p)$ le noyau de $(p(u))^k$ dans E, et soit $F(u, p)$ la réunion des $F_k(u, p)$ pour tous les entiers $k > 0$. Montrer que si p et q sont deux polynômes unitaires irréductibles distincts divisant le polynôme minimal de u, les sous-espaces $F(u, p)$ et $F(u^*, \bar{q})$ sont orthogonaux (utiliser l’identité de Bezout). Enfin, si G est un sous-espace vectoriel de E tel que $u(G) \subset G$, on a $u^*(G^0) \subset G^0$.

b) On suppose que $uu^* = u^*u$ (cas où on dit que u est un endomorphisme normal pour $\Phi$; cf. § 7, no 3); montrer que l’on a alors $u^*(F_k(u, p)) \subset F_k(u, p)$ pour tout k, et par suite $u^*(F(u, p)) \subset F(u, p)$. Si on pose $G(p, \bar{q}) = F(u, p) \cap F(u^*, \bar{q})$, montrer que E est somme directe des sous-espaces $G(p, \bar{q})$, et que $G(p, \bar{q})$ et $G(p_1, \bar{q}_1)$ sont orthogonaux si $p \neq q_1$ ou si $p_1 \neq q$; en particulier $G(p, \bar{q})$ est totalement isotrope si $p \neq q$. Montrer que $G(p, \bar{p})$ est réduit à 0 ou non isotrope, et que si $p \neq q$, aucun vecteur non nul de $G(p, \bar{q})$ n’est orthogonal à $G(q, \bar{p})$ (utiliser le fait que $\Phi$ est non dégénérée); en déduire que si $p \neq q$, $G(p, \bar{q})$ et $G(q, \bar{p})$ sont des sous-espaces totalement isotropes de même dimension, et que $G(p, \bar{q}) + G(q, \bar{p})$ est non isotrope.

c) On suppose que J n’est pas l’identité ou que A n’est pas de caractéristique 2, et que $u^* = u$. Soit $\mathcal{M}$ l’ensemble des sous-espaces non isotropes $M \subset G(p, \bar{p})$, stables pour u (donc sous-modules du $A[X]$-module $E_u$ (chap. VII, § 5, no 1)). Montrer que si $M$ est un élément minimal de $\mathfrak{M}$, $M$ est un sous-module *indécomposable* de $E_u$ (chap. VII, § 4, no 7). (Supposer que $M$ soit somme directe d’un sous-module indécomposable $M_1$ et d’un sous-module $M_2 \neq \{0\}$, les polynômes minimaux $p^h$ et $p^k$ des restrictions de $u$ à $M_1$ et $M_2$ respectivement étant tels que $h \geq k$. Remarquer alors que $M_1$ est nécessairement isotrope et que tout $z \neq 0$ dans $M_1$ tel que $p(u).z = 0$ est orthogonal à $M_1$ (utiliser le fait que tout sous-module de $M_1$ est monogène) ; écrire que $z = (p(u))^{h-1}.x$ et que $z$ n’est pas orthogonal à $M_2$, et en déduire qu’on a nécessairement $k = h$. Montrer ensuite qu’il existe un sous-module indécomposable $N_2$ de $M_2$ tel que $p^h$ soit le polynôme minimal de la restriction de $u$ à $N_2$, et que $M_1 + N_2$ soit non isotrope ; en conclure que $M_2 = N_2$. Enfin, si $y \in M_2$ n’est pas orthogonal à $z$, considérer le sous-module $P$ de $M$ engendré par $w = x + \lambda y$, où $\lambda \in \mathbf{A}$, et montrer qu’on peut prendre $\lambda$ tel que $P$ soit non isotrope, en prouvant qu’on a $\Phi((p(u))^{h-1}.w, w) \neq 0$; ce qui aboutit à une contradiction).

d) Déduire de c) que $G(p, \overline{p})$ est somme directe de sous-modules indécomposables $H_i$, deux à deux orthogonaux. Si $p^h$ est le polynôme minimal de la restriction de $u$ à $H_i$, et si $d$ est le degré de $p$, montrer qu’il existe dans $H_i$ un sous-espace totalement isotrope de dimension $d.[h/2]$. Cas où $E$ ne contient aucun vecteur isotrope $\neq 0$ (cf. § 7, no 3).

e) Enoncer et démontrer les propriétés analogues à celles de c) et d) lorsqu’on a $u^* = -u$ ou $u^*u = 1$.

f) Donner un exemple où $n = 4$, $\Phi$ est symétrique et d’indice 2, $p = \overline{p} = X - 1$, $u$ est normal, $E = G(p, \overline{p})$, mais $E$ n’est pas somme directe de sous-modules minimaux de $\mathfrak{M}$, et où il existe un vecteur propre de $u$ qui n’est pas vecteur propre de $u^*$ (cf. § 7, no 3).

13) Les hypothèses sont celles de l’exerc. 2, et on suppose en outre que $E$ admette une base dénombrable $(e_n)$. Soit $F$ un sous-espace totalement isotrope (resp. totalement singulier) de $E$ tel que $F^{00} = F$; montrer qu’il existe un sous-espace totalement isotrope (resp. totalement singulier) $F'$ tel que : $1^\circ \ F \cap F' = \{0\}$; $2^\circ$ il existe une base $(a_m)_{m \in I}$ de $F$ et une base $(a'_m)_{m \in I}$ de $F'$ (l’intervalle de $\mathbf{N}$ d’origine 0) telles que $\Phi(a_i, a'_j) = \delta_{ij}$ pour tout couple d’indices ; $3^\circ$ $(F + F')^{00} = F + F'$ et $E$ est somme directe de $F + F'$ et de $G = (F + F')^0$. (Former par récurrence une suite croissante $(L_n)$ de sous-espaces non isotropes, de réunion $E$, tels que $\dim L_{n+1} - \dim L_n = 2$, et appliquer la prop. 2 du no 2 à chacun des $L_n$; pour former cette suite, on considérera, pour tout $n$, le plus petit entier $k$ tel que $e_k \notin L_n$, et on utilisera l’exerc. 9 b) du § 1).

14) Soient $A$ un corps de caractéristique 2, $E$ un espace vectoriel de dimension finie $n$ sur $A$, $\Phi$ une forme hermitienne non dégénérée sur $E$, ne satisfaisant pas nécessairement à la condition (T).

a) Montrer que l’ensemble $V$ des $x \in E$ tels que $\Phi(x, x)$ soit de la forme $\alpha + \overline{\alpha}$ est un sous-espace vectoriel de $E$.

b) Soient $V_1 = V \cap V^0$, $q = \dim V_1$, $V_2$ un supplémentaire de $V_1$ par rapport à $V$, $V_3$ un supplémentaire de $V_1$ par rapport à $V^0$. Montrer qu’il existe une base $(e_i)_{1 \leq i \leq 2q}$ de $(V_2 + V_3)^0 = V_2^0 \cap V_3^0$ telle que les vecteurs $e_1, \ldots, e_q$ forment une base de $V_1$ et que l’on ait $\Phi(e_i, e_{q+j}) = \delta_{ij}$ pour $1 \leq i \leq q, 1 \leq j \leq q$.

c) Soit $G(\Phi)$ le groupe des automorphismes métriques de $E$ (pour $\Phi$). Montrer que pour tout $u \in G(\Phi)$, on a $u(x) = x$ pour tout $x \in V^0$.

d) Pour tout $u \in G(\Phi)$, on a $u(V) = V$; soit $u_v$ la restriction de $u$ à $V$, et soit $G_v$ le groupe formé par les $u_v$. Montrer que : $1^o$ le noyau de l’homomorphisme $u \to u_v$ de $G(\Phi)$ sur $G_v$ est commutatif ; $2^o$ si $\Phi_2$ est la restriction de $\Phi$ à $V_2$ et $G(\Phi_2)$ le groupe des automorphismes métriques de $V_2$ pour $\Phi_2$, il existe un homomorphisme de $G_v$ sur $G(\Phi_2)$ dont le noyau est commutatif (utiliser $b$ et $c$).

e) On suppose que $A$ est commutatif et $J$ est l’identité ; soient $E$ un espace vectoriel de dimension 3 sur $A$, $(e_i)_{1 \leq i \leq 3}$ une base de $E$, $\Phi$ la forme symétrique non dégénérée sur $E$ dont la matrice par rapport à $(e_i)$ est

$$
\begin{pmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0
\end{pmatrix}.
$$

Montrer que tous les vecteurs isotropes dans $E$ sont contenus dans l’hyperplan engendré par $e_2$ et $e_3$ (cf. exerc. 4 a)). Donner un exemple de plan non isotrope mais ne contenant qu’une seule droite isotrope (cf. exerc. 2 a)). Montrer qu’il n’existe aucun automorphisme $u \in G(\Phi)$ tel que $u(e_1) = e_1 + e_2$, bien que l’on ait $\Phi(e_1, e_1) = \Phi(e_1 + e_2, e_1 + e_2)$.
