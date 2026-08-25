---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 1
section_title: Dimension de Krull d’un anneau
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.81-AC VIII.83
pdf_pages: 0005-0017, 0085-0087
extraction: ocr
subsections:
    - "no": 1
      title: Dimension de Krull d’un espace topologique
      page: 0
      pdf_page: 5
    - "no": 2
      title: Codimension d’une partie fermée
      page: 4
      pdf_page: 8
    - "no": 3
      title: Dimension d’un anneau, hauteur d’un idéal
      page: 6
      pdf_page: 10
    - "no": 4
      title: Dimension d’un module de type fini
      page: 10
      pdf_page: 14
    - "no": 5
      title: Cycles associés à un module
      page: 11
      pdf_page: 15
statements: 48
exercises: 17
content_sha256: a122898c347ac2c94d8ed5475b416c6b8512da1b9ff8b449d3de15a3b1623dba
---

## § 1. DIMENSION DE KRULL D’UN ANNEAU

### 1. Dimension de Krull d’un espace topologique

#### Définition 1 {#ac-viii-s1-def-1 .statement}

Soit $ I $ un ensemble ordonné. Une partie finie non vide et totalement ordonnée de $ I $ est appelée une chaîne de $ I $. Soit $ c $ une chaîne de $ I $; le plus petit et le plus grand élément de $ c $ sont appelés les extrémités de $ c $. L’entier $ \mathrm{Card}(c) - 1 $ est appelé la longueur de $ c $. La relation d’inclusion dans l’ensemble des parties de $ I $ induit une relation d’ordre dans l’ensemble des chaînes de $ I $. Une chaîne $ c $ de $ I $ est dite saturée si elle est maximale parmi les chaînes de $ I $ ayant les mêmes extrémités que $ c $.

Pour désigner une chaîne c de longueur n, on écrira souvent : « la chaîne $ i_0 < \cdots < i_n $ », où les $ i_k $ sont les éléments de c indexés de façon strictement croissante par les entiers de 0 à n.

Soit X un espace topologique. On munit l’ensemble des parties fermées irréductibles de X (II, § 4, n° 1, déf. 1) de la relation d’ordre définie par l’inclusion. Lorsque l’on parlera d’une chaîne de parties fermées irréductibles de X, il s’agira toujours d’une chaîne au sens de cette relation d’ordre.

#### Définition 2 {#ac-viii-s1-def-2 .statement}

On appelle dimension de Krull de l’espace topologique X et on note dim kr(X) ou simplement dim(X) la borne supérieure dans $ \overline{\mathbf{R}} $ de l’ensemble des longueurs des chaînes de parties fermées irréductibles de X.
Pour tout point x de X, on appelle dimension de Krull de X en x et on note $ \dim_x(X) $ la borne inférieure des dimensions des voisinages ouverts de x.

On a $ \dim(\varnothing) = -\infty $. Par contre, si X n’est pas vide, l’adhérence de tout point de X est une partie fermée irréductible de X (II, § 4, n° 1, prop. 2) et la dimension de X est donc $ +\infty $ ou un entier positif. Supposons que X soit séparé et non vide ; alors toute partie irréductible de X est réduite à un point, et X est de dimension 0.
La définition de la dimension de Krull est donc dénuée d’intérêt pour les espaces séparés, mais elle est spécialement adaptée aux espaces topologiques rencontrés en Algèbre Commutative (spectres d’anneaux, \* schémas *, ...). Dans ce chapitre, aucune confusion n’est à craindre avec d’autres notions de dimension des espaces topologiques (par exemple, celle de Lebesgue), et nous dirons simplement « dimension » pour « dimension de Krull ».

#### Proposition 1 {#ac-viii-s1-prop-1 .statement}

Soit X un espace topologique.
a) Si Y est un sous-espace de X, on a $ \dim(Y) \leq \dim(X) $, et $ \dim_y(Y) \leq \dim_y(X) $ pour tout point y de Y.
b) Soient x un point de X et V un voisinage de x dans X. On a $ \dim_x(X) = \dim_x(V) $.
c) Soit $ (X_i)_{i \in I} $ une famille finie de parties fermées de X telle que $ X = \bigcup_{i \in I} X_i $. On a alors $ \dim(X) = \sup_{i \in I} \dim(X_i) $ et, pour tout point x de X, on a $ \dim_x(X) = \sup_{i \in J_x} \dim_x(X_i) $, où $ J_x $ désigne l’ensemble des $ i \in I $ tels que $ x \in X_i $.

Démontrons a). Si Z est une partie fermée irréductible de Y, son adhérence $ \overline{Z} $ dans X est irréductible (II, § 4, n° 1, prop. 2) et l’on a $ \overline{Z} \cap Y = Z $. Ainsi, toute chaîne c de parties fermées irréductibles de Y définit, par passage à l’adhérence dans X, une chaîne de parties fermées irréductibles de X, de même longueur que c. L’inégalité $ \dim(Y) \leq \dim(X) $ résulte de cela. Si U est une partie ouverte de X contenant un point y de Y, on a donc $ \dim(U \cap Y) \leq \dim(U) $, d’où $ \dim_y(Y) \leq \dim_y(X) $.
Démontrons b). On a par définition $ \dim_x(X) \leq \dim_x(V) $, et l’inégalité opposée résulte de a).
Démontrons c). Soit $ Z_0 \subset \ldots \subset Z_n $ une chaîne de parties fermées irréductibles de X. On a $ Z_n = \bigcup_{i \in I} (Z_n \cap X_i) $ et chacun des ensembles $ Z_n \cap X_i $ est fermé dans $ Z_n $;

comme I est fini, $ Z_n $ est contenu dans l’un des $ X_i $. Par suite, on a $ \dim(X) \leq \sup_{i} \dim(X_i) $, d’où l’égalité d’après *a*).

Soient maintenant $ x $ un point de $ X $ et $ n = \sup_{i \in J_x} \dim_x(X_i) $, où $ J_x $ est comme dans l’énoncé. On a $ \dim_x(X) \geq n $ d’après *a*), et, pour établir l’égalité, on peut supposer $ n $ fini. Pour tout $ i \in J_x $, soit $ U_i $ un voisinage ouvert de $ x $ dans $ X $, tel que $ \dim(U_i \cap X_i) \leq n $. Posons $ U = (\bigcap_{i \in J_x} U_i) \cap (\bigcap_{i \in I - J_x} \mathcal{C} X_i) $; l’ensemble $ U $ est ouvert dans $ X $. De plus, on a $ \dim(U) = \sup_{i \in J_x} \dim(U \cap X_i) \leq n $ d’après l’alinéa précédent, donc $ \dim_x(X) \leq n $.

#### Corollaire {#ac-viii-s1-n1-cor-1 .statement}

*a*) *La dimension de l’espace topologique $ X $ est la borne supérieure des dimensions de ses composantes irréductibles* (II, § 4, no 1, déf. 2).

*b*) *Soit $ x $ un point de $ X $. On a $ \dim_x(X) \geq \sup \dim_x(X_i) $, où $ X_i $ parcourt la famille des composantes irréductibles de $ X $ qui contiennent $ x $; il y a égalité si $ x $ possède un voisinage $ V $ qui n’a qu’un nombre fini de composantes irréductibles (ce qui est le cas par exemple si $ V $ est noethérien)*.

La première assertion est immédiate puisque les chaînes de parties fermées irréductibles de $ X $ sont les chaînes de parties fermées irréductibles des composantes irréductibles de $ X $ (II, § 4, no 1, prop. 5). L’inégalité $ \dim_x(X) \geq \sup_{i} \dim_x(X_i) $ résulte de la prop. 1, *a*). Soit $ V $ un voisinage de $ x $ qui ne possède qu’un nombre fini de composantes irréductibles, et soit $ (V_j)_{j \in J} $ la famille des composantes irréductibles de $ V $ qui contiennent $ x $. Il résulte de la prop. 1, *b*) et *c*) qu’on a
$$
\dim_x(X) = \dim_x(V) = \sup_{j \in J} \dim_x(V_j);
$$
on conclut en remarquant que chacun des $ V_j $ est contenu dans l’un des $ X_i $, $ i \in J_x $, et qu’on a par conséquent $ \sup_{j \in J} \dim_x(V_j) \leq \sup_{i \in J_x} \dim_x(X_i) $.

#### Proposition 2 {#ac-viii-s1-prop-2 .statement}

*Soit $ X $ un espace topologique. On a $ \dim(X) = \sup_{x \in X} \dim_x(X) $*.

En effet, on a par définition $ \dim(X) \geq \dim_x(X) $ pour tout $ x \in X $. D’autre part, si $ Z_0 \subset ... \subset Z_n $ est une chaîne de parties fermées irréductibles de $ X $, pour tout $ x \in Z_0 $ et tout voisinage ouvert $ U $ de $ x $, les ensembles $ Z_0 \cap U, ..., Z_n \cap U $ constituent une chaîne de parties fermées irréductibles de $ U $ (II, § 4, no 1, prop. 7). On a donc $ \dim_x(X) \geq n $, d’où $ \dim(X) \leq \sup_{x \in X} \dim_x(X) $.

#### Corollaire {#ac-viii-s1-n1-cor-2 .statement}

*Si $ (X_\alpha)_{\alpha \in A} $ est un recouvrement ouvert, ou un recouvrement fermé localement fini, d’un espace topologique $ X $, on a*
$$
\dim(X) = \sup_{\alpha \in A} \dim(X_\alpha).
$$

Il suffit de démontrer que, pour tout point $ x $ de $ X $, on a $ \dim_x(X) = \sup_{\alpha \in A_x} \dim_x(X_\alpha) $, où $ A_x $ est l’ensemble des $ \alpha \in A $ tels que $ x \in X_\alpha $. Ceci est clair dans le cas d’un recouvrement ouvert, et résulte de la prop. 1, c), dans le cas d’un recouvrement fermé localement fini.

### 2. Codimension d’une partie fermée

#### Définition 3 {#ac-viii-s1-def-3 .statement}

Soit X un espace topologique.

a) Si Y est une partie fermée irréductible de X, on appelle codimension de Y dans X la borne supérieure dans $ \overline{\mathbf{R}} $ des longueurs des chaînes de parties fermées irréductibles de X dont Y est le plus petit élément.

b) Si Y est une partie fermée de X, on appelle codimension de Y dans X, et on note $ \operatorname{codim}(Y, X) $ la borne inférieure dans $ \overline{\mathbf{R}} $ des codimensions, dans X, des composantes irréductibles de Y.

#### Remarque 1 {#ac-viii-s1-n2-rem-1 .statement}

La codimension d’une partie fermée Y de X est donc la borne inférieure des codimensions des parties fermées irréductibles de Y. On a $ \operatorname{codim}(\varnothing, X) = +\infty $ et, si X n’est pas vide, $ \operatorname{codim}(X, X) = 0 $. Toute partie fermée non vide de X contient une partie fermée irréductible (II, § 4, no 1, prop. 5); la codimension dans X d’une partie fermée Y est donc toujours un entier positif ou $ +\infty $; elle est nulle si et seulement si Y contient une composante irréductible de X.

#### Remarque 2 {#ac-viii-s1-n2-rem-2 .statement}

Si Y est une partie fermée non vide de X, on a $ \operatorname{codim}(Y, X) \leq \dim(X) $. On a $ \dim(X) = \sup_Y \operatorname{codim}(Y, X) $, où Y parcourt l’ensemble des parties fermées irréductibles de X. Si Y et Y’ sont deux parties fermées de X telles que $ Y' \subset Y $, on a $ \operatorname{codim}(Y, X) \leq \operatorname{codim}(Y', X) $.

#### Remarque 3 {#ac-viii-s1-n2-rem-3 .statement}

Soient Y une partie fermée de l’espace topologique X et $ (X_\alpha)_{\alpha \in A} $ (resp. $ (Y_\beta)_{\beta \in B} $) la famille des composantes irréductibles de X (resp. de Y). Pour tout $ \beta \in B $, notons $ A(\beta) $ l’ensemble des $ \alpha \in A $ tels que $ Y_\beta \subset X_\alpha $. Du fait que toute partie irréductible de X est contenue dans l’un des $ X_\alpha $ (II, § 4, no 1, prop. 5), il résulte de la déf. 3 que l’on a :

$$
\operatorname{codim}(Y, X) = \inf_{\beta \in B} \sup_{\alpha \in A(\beta)} \operatorname{codim}(Y_\beta, X_\alpha).
$$

#### Remarque 4 {#ac-viii-s1-n2-rem-4 .statement}

Soient $ (Y_i)_{i \in I} $ une famille finie de parties fermées de X et $ Y = \bigcup_{i \in I} Y_i $; on a

$$
\operatorname{codim}(Y, X) = \inf_{i \in I} \operatorname{codim}(Y_i, X).
$$

En effet, toute composante irréductible de Y est contenue dans l’un des $ Y_i $.

#### Proposition 3 {#ac-viii-s1-prop-3 .statement}

Soit X un espace topologique.

a) Pour toute partie fermée non vide Y de X, on a

$$
\dim(Y) + \operatorname{codim}(Y, X) \leq \dim(X).
$$

b) Si Y, Z, T sont des parties fermées de X telles que $ Y \subset Z \subset T $, on a

$$
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) \leq \operatorname{codim}(Y, T).
$$

Il suffit de démontrer l’assertion $ a) $ dans le cas où $ \dim(X) $ est fini. Dans ce cas, $ \dim(Y) $ et $ \operatorname{codim}(Y, X) $ sont finis. Il existe une chaîne $ Y_0 \subset ... \subset Y_n $ de parties fermées irréductibles de $ Y $, de longueur $ n = \dim(Y) $ et une chaîne $ Y_n \subset ... \subset Y_{n+p} $ de parties fermées irréductibles de $ X $, de longueur $ p \geq \operatorname{codim}(Y, X) $. On en déduit que $ \dim(X) \geq n + p $, d’où $ a) $. Pour établir $ b) $, on peut supposer $ Y $ irréductible. Comme on a $ \operatorname{codim}(Y, Z) \leq \operatorname{codim}(Y, T) $, l’inégalité est démontrée si $ \operatorname{codim}(Y, Z) = +\infty $. Sinon, soit $ Z_0 $ une composante irréductible de $ Z $ contenant $ Y $ et telle que $ \operatorname{codim}(Y, Z) = \operatorname{codim}(Y, Z_0) $. On a $ \operatorname{codim}(Z, T) \leq \operatorname{codim}(Z_0, T) $, et on voit, comme ci-dessus, que $ \operatorname{codim}(Y, Z_0) + \operatorname{codim}(Z_0, T) \leq \operatorname{codim}(Y, T) $, d’où $ b) $.

#### Définition 4 {#ac-viii-s1-def-4 .statement}

Un espace topologique $ X $ est dit caténaire si, pour tout couple $ (Y, Z) $ de parties fermées irréductibles de $ X $ telles que $ Y \subset Z $, toute chaîne saturée de parties fermées irréductibles d’extrémités $ Y $ et $ Z $ est de longueur $ \operatorname{codim}(Y, Z) $.

Il revient au même de dire que, pour tout couple $ (Y, Z) $ de parties fermées irréductibles de $ X $ tel que $ \operatorname{codim}(Y, Z) $ soit fini, toutes les chaînes saturées d’extrémités $ Y $ et $ Z $ ont même longueur, et que, pour tout couple $ (Y, Z) $ tel que $ \operatorname{codim}(Y, Z) = +\infty $, il n’existe aucune chaîne saturée d’extrémités $ Y $ et $ Z $.

Tout sous-espace fermé d’un espace caténaire est caténaire. Pour qu’un espace soit caténaire, il faut et il suffit que ses composantes irréductibles le soient.

#### Proposition 4 {#ac-viii-s1-prop-4 .statement}

Soit $ X $ un espace topologique. Pour que $ X $ soit caténaire, il faut et il suffit que, pour tout triplet $ (Y, Z, T) $ de parties fermées irréductibles de $ X $ tel que $ Y \subset Z \subset T $, on ait :

$$
\operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)
$$

Supposons $ X $ caténaire. Compte tenu de la prop. 3, $ b) $, il suffit de démontrer la relation lorsque $ \operatorname{codim}(Y, Z) $ et $ \operatorname{codim}(Z, T) $ sont finis. En mettant bout à bout une chaîne saturée de parties fermées irréductibles d’extrémités $ Y $ et $ Z $, de longueur $ \operatorname{codim}(Y, Z) $, et une chaîne saturée de parties fermées irréductibles d’extrémités $ Z $ et $ T $, de longueur $ \operatorname{codim}(Z, T) $, on obtient une chaîne saturée d’extrémités $ Y $ et $ T $, de longueur $ \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) $. Mais, comme $ X $ est caténaire, cette longueur est nécessairement égale à $ \operatorname{codim}(Y, T) $.

Réciproquement, supposons que l’on ait $ \operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) $ quelles que soient les parties fermées irréductibles $ Y, Z, T $ de $ X $ telles que $ Y \subset Z \subset T $, et démontrons que $ X $ est caténaire. Pour cela, démontrons par récurrence sur l’entier $ n \geq 0 $ que, pour toute chaîne saturée $ Z_0 \subset ... \subset Z_n $ de parties fermées irréductibles de $ X $, on a $ \operatorname{codim}(Z_0, Z_n) = n $. Si $ n = 0 $, c’est clair. Soit $ n > 0 $, et supposons la propriété satisfaite pour les chaînes de longueur $ \leq n - 1 $. Si $ Z_0 \subset ... \subset Z_n $ est une chaîne saturée de longueur $ n $, alors $ Z_0 \subset ... \subset Z_{n-1} $ est une chaîne saturée de longueur $ n - 1 $, donc $ \operatorname{codim}(Z_0, Z_{n-1}) = n - 1 $. Vu l’hypothèse faite sur $ X $, on a $ \operatorname{codim}(Z_0, Z_n) = \operatorname{codim}(Z_0, Z_{n-1}) + \operatorname{codim}(Z_{n-1}, Z_n) = (n - 1) + 1 = n $.

#### Corollaire {#ac-viii-s1-n2-cor-1 .statement}

Soit X un espace topologique irréductible et de dimension finie. Pour que X soit caténaire, il faut et il suffit que, pour tout couple (Y, Z) de parties fermées irréductibles de X telles que Y ⊂ Z, on ait codim(Y, X) = codim(Y, Z) + codim(Z, X).

La condition est nécessaire d’après la prop. 4. Inversement, supposons-la vérifiée, et notons c(Z) l’entier codim(Z, X) pour toute partie fermée irréductible Z de X. Si Y, Z, T sont trois parties fermées irréductibles de X telles que Y ⊂ Z ⊂ T, on a
$$
\begin{align*}
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) &= (c(Y) - c(Z)) + (c(Z) - c(T)) \\
&= c(Y) - c(T) \\
&= \operatorname{codim}(Y, T),
\end{align*}
$$
et X est caténaire d’après la prop. 4.

#### Proposition 5 {#ac-viii-s1-prop-5 .statement}

Soit X un espace topologique de dimension finie. Supposons que toutes les chaînes maximales de parties fermées irréductibles de X aient même longueur. Alors X est caténaire ; pour toute partie fermée irréductible Z de X, on a
$$
\operatorname{codim}(Z, X) = \dim(X) - \dim(Z);
$$
pour tout couple (Y, Z) de parties fermées irréductibles de X tel que Y ⊂ Z, on a
$$
\operatorname{codim}(Y, Z) = \dim(Z) - \dim(Y).
$$

Soient Y et Z deux parties fermées irréductibles de X telles que Y ⊂ Z. Soient Y_0 ⊂ ... ⊂ Y_p une chaîne telle que Y_p = Y et p = \dim(Y), Z_0 ⊂ ... ⊂ Z_q une chaîne telle que Z_0 = Z et q = \operatorname{codim}(Z, X). Pour toute chaîne saturée T_0 ⊂ ... ⊂ T_r telle que T_0 = Y et T_r = Z, la chaîne
$$
Y_0 \subset ... \subset Y_{p-1} \subset T_0 \subset ... \subset T_r \subset Z_1 ... \subset Z_q
$$
est maximale, et de longueur p + q + r ; d’après l’hypothèse faite sur X, on a donc p + q + r = \dim(X), soit r = \dim(X) - \dim(Y) - \operatorname{codim}(Z, X). Il en résulte que X est caténaire et que, pour Y et Z comme ci-dessus, on a
$$
\dim(Y) + \operatorname{codim}(Y, Z) = \dim(X) - \operatorname{codim}(Z, X).
$$
Prenant Y = Z, on voit que le second membre est égal à \dim(Z), d’où la proposition.

### 3. Dimension d’un anneau, hauteur d’un idéal

#### Définition 5 {#ac-viii-s1-def-5 .statement}

On appelle dimension de Krull, ou simplement dimension, d’un anneau (commutatif) A et l’on note \dim(A), la dimension de Krull de l’espace topologique Spec(A) (II, § 4, n° 3, déf. 4). Si p est un idéal premier de A, on appelle dimension de A en p, et on note \dim_p(A), le nombre \dim_p(\operatorname{Spec}(A)).

L’application $ p \mapsto V(p) $ est une bijection décroissante de l’ensemble des idéaux premiers de $ A $ sur l’ensemble des parties fermées irréductibles de $ \mathrm{Spec}(A) $ (*loc. cit.*, cor. 2 à la prop. 14). *La dimension de $ A $ est donc la borne supérieure de l’ensemble des longueurs des chaînes d’idéaux premiers de $ A $* ; elle est égale à $ -\infty, +\infty $ ou à un entier positif.

Soit $ p \in \mathrm{Spec}(A) $; les ensembles $ \mathrm{Spec}(A)_f $, où $ f $ parcourt $ A $, forment une base de la topologie de $ \mathrm{Spec}(A) $, et $ p $ appartient à l’ouvert $ \mathrm{Spec}(A)_f $ si et seulement si $ f $ n’appartient pas à $ p $. Par conséquent, $ \dim_p(A) $ est la borne inférieure des nombres $ \dim(A_f) $, où $ f $ parcourt $ A - p $ (II, § 5, no 1, prop. 1).

#### Exemple 1 {#ac-viii-s1-n3-exa-1 .statement}

On a $ \dim(A) < 0 $ si et seulement si $ A $ est réduit à 0. Pour que l’on ait $ \dim(A) \leqslant 0 $, il faut et il suffit que tout idéal premier de $ A $ soit maximal. Les anneaux intègres de dimension 0 sont les corps. Un anneau noethérien est de dimension $ \leqslant 0 $ si et seulement s’il est artinien (IV, § 2, no 5, prop. 9).

#### Exemple 2 {#ac-viii-s1-n3-exa-2 .statement}

Les anneaux de Dedekind sont les anneaux noethériens intégralement clos de dimension $ \leqslant 1 $ (VII, § 2, no 2, th. 1). Plus généralement, d’après V, § 1, no 2, cor. 2 à la prop. 9, un anneau est un produit fini d’anneaux de Dedekind si et seulement s’il est noethérien, réduit, intégralement fermé dans son anneau total des fractions, et de dimension $ \leqslant 1 $.

#### Exemple 3 {#ac-viii-s1-n3-exa-3 .statement}

Si $ A $ est un anneau de valuation (VI, § 1, no 2, déf. 2), sa dimension est égale à la hauteur de la valuation (VI, § 4, no 4, prop. 5).

#### Exemple 4 {#ac-viii-s1-n3-exa-4 .statement}

Soit $ A $ un anneau. On a
$$
\dim(A[X]) \geqslant \dim(A) + 1 .
$$
En effet, si $ p_0 \subset ... \subset p_n $ est une chaîne d’idéaux premiers de $ A $, de longueur $ n $, on obtient une chaîne $ p'_0 \subset ... \subset p'_{n+1} $ d’idéaux premiers de $ A[X] $, de longueur $ n + 1 $, en posant $ p'_i = p_i A[X] $ pour $ 0 \leq i \leq n $, et $ p'_{n+1} = p_n A[X] + XA[X] $.

Par le même raisonnement, on prouve l’inégalité $ \dim(A[[X]]) \geqslant \dim(A) + 1 $. On en déduit par récurrence les inégalités
$$
\dim(A[X_1, ..., X_n]) \geqslant \dim(A) + n ,
$$
$$
\dim(A[[X_1, ..., X_n]]) \geqslant \dim(A) + n .
$$

Nous démontrerons plus loin (§ 3, no 4, cor. 3 de la prop. 7 et cor. 3 de la prop. 8) que l’on a égalité dans les deux formules précédentes lorsque $ A $ est noethérien.

#### Exemple 5 {#ac-viii-s1-n3-exa-5 .statement}

Soit $ X $ une variété analytique complexe. Si $ X $ est de dimension complexe $ n $ en un point $ x $ de $ X $, l’anneau local des germes en $ x $ de fonctions analytiques sur $ X $ est de dimension $ n $. \*

#### Exemple 6 {#ac-viii-s1-n3-exa-6 .statement}

Soient $ k $ un corps et $ A $ une $ k $-algèbre entière non nulle. Alors on a $ \dim(A) = 0 $. Cela résulte du cor. 1 à la prop. 1 de V, § 2, no 1, et du fait que $ \dim(k) = 0 $.

#### Exemple 7 {#ac-viii-s1-n3-exa-7 .statement}

Si $ \mathfrak{n} $ est un nilidéal de $ A $, $ \mathrm{Spec}(A) $ est homéomorphe à $ \mathrm{Spec}(A/\mathfrak{n}) $ (II, § 4, no 3, remarque). On a donc $ \dim(A/\mathfrak{n}) = \dim(A) $; en particulier, on a $ \dim(A) = \dim(A_{\mathrm{red}}) $ où $ A_{\mathrm{red}} $ est le quotient de l’anneau $ A $ par son nilradical.

#### Exemple 8 {#ac-viii-s1-n3-exa-8 .statement}

Il existe des anneaux noethériens de dimension infinie (p. 83, exerc. 13). Nous verrons ci-dessous (§ 3, n° 1, cor. 1 à la prop. 2) que tout anneau local noethérien est de dimension finie.

#### Proposition 6 {#ac-viii-s1-prop-6 .statement}

Soit A un anneau.
a) Si a est un idéal de A, on a dim(A/a) $ \leq $ dim(A).
b) Si S est une partie multiplicative de A, on a dim(S$^{-1}$A) $ \leq $ dim(A).
c) On a dim(A) = sup dim(A/p), où p parcourt l’ensemble des idéaux premiers minimaux de A.
d) Si A n’a qu’un nombre fini d’idéaux premiers minimaux (par exemple si A est noethérien (II, § 4, n° 3, cor. 3 à la prop. 14)) et si p est un idéal premier de A, on a
$$
\dim_p(A) = \sup_q \dim_{p/q}(A/q),
$$
où q parcourt l’ensemble des idéaux premiers minimaux de A contenus dans p.
e) Soit a un idéal de A qui n’est contenu dans aucun idéal premier minimal de A ; on a alors dim(A) $ \geq $ dim(A/a) + 1. En particulier, si A est intègre, on a dim(A) $ \geq $ dim(A/a) + 1 pour tout idéal non nul a de A.

D’après la remarque de II, § 4, n° 3, si a est un idéal de A, l’espace topologique Spec(A/a) est homéomorphe au sous-espace fermé V(a) de Spec(A). L’assertion a) résulte de cela et de la prop. 1, a) du n° 1. L’assertion b) résulte de loc. cit., corollaire à la prop. 13. D’après loc. cit., cor. 2 à la prop. 14, les composantes irréductibles de Spec(A) sont homéomorphes aux espaces Spec(A/p), où p est un idéal premier minimal de A, et l’assertion c) résulte du corollaire de la prop. 1 du n° 1. Sous l’hypothèse de d ), l’espace Spec(A) n’a qu’un nombre fini de composantes irréductibles ; les composantes irréductibles de Spec(A) contenant p sont les ensembles V(q), où q est un idéal premier minimal contenu dans p. L’assertion d) résulte alors du cor., b) de la prop. 1 du n° 1.

Démontrons enfin e). Il s’agit de prouver que, pour toute chaîne $ p_0 \subset ... \subset p_n $ d’idéaux premiers de A telle que $ a \subset p_0 $, on a dim(A) $ \geq n + 1 $. Vu l’hypothèse faite sur a, il existe un idéal premier $ p_{-1} $ de A contenu dans $ p_0 $, distinct de $ p_0 $, et $ p_{-1} \subset p_0 \subset ... \subset p_n $ est une chaîne d’idéaux premiers de A, de longueur $ n + 1 $.

#### Remarque 1 {#ac-viii-s1-n3-rem-1 .statement}

Soit $ \rho : A \to B $ un homomorphisme d’anneaux. Alors dim(B) est la borne supérieure des nombres dim(B/$ \rho(p) $.B), où p parcourt l’ensemble des idéaux premiers minimaux de A : en effet, pour tout idéal premier minimal q de B, il existe un idéal premier minimal p de A contenu dans $ \rho^{-1}(q) $ (II, § 2, n° 6, lemme 2) et l’on a
$$
\dim(B/q) \leq \dim(B/\rho(p).B) \leq \dim(B)
$$
par la prop. 6, a) ; on conclut par la prop. 6, c).

#### Définition 6 {#ac-viii-s1-def-6 .statement}

Soit a un idéal d’un anneau A. La codimension de V(a) dans Spec(A) est appelée hauteur de l’idéal a et notée ht(a).

Supposons A intègre. Alors les idéaux premiers de hauteur 1 de A au sens de la déf. 4 de VII, § 1, n° 6, sont les idéaux premiers de hauteur 1 au sens de la définition ci-dessus.

#### Proposition 7 {#ac-viii-s1-prop-7 .statement}

a) La hauteur d’un idéal premier p de A est la borne supérieure des longueurs des chaînes d’idéaux premiers $ p_0 \subset ... \subset p_n $ telles que $ p_n = p $.

b) Soient p un idéal premier de A et a un idéal de A. Alors on a $ \dim(A_p/aA_p) = -\infty $ si a n’est pas contenu dans p et $ \dim(A_p/aA_p) = \operatorname{codim}(V(p), V(a)) $ si a est contenu dans p. En particulier, si p est un idéal premier de A, on a $ \dim(A_p) = \operatorname{ht}(p) $.

c) Si a est un idéal de A, on a $ \operatorname{ht}(a) = \inf_{p} \operatorname{ht}(p) = \inf_{p} \dim(A_p) $ où p parcourt l’ensemble des idéaux premiers de A contenant a.

L’assertion a) est la traduction de la déf. 3, a) du n° 2. L’assertion b) résulte du fait que l’application $ q \mapsto q(A_p/aA_p) $ est un isomorphisme croissant de l’ensemble des idéaux premiers q de A tels que $ a \subset q \subset p $ sur l’ensemble des idéaux premiers de l’anneau local $ A_p/aA_p $ (II, § 2, n° 5, prop. 11). Soit a un idéal de A ; les parties fermées irréductibles de $ V(a) $ sont les ensembles $ V(p) $, où p est un idéal premier de A contenant a. L’assertion c) résulte donc de la remarque 1 du n° 2.

#### Corollaire {#ac-viii-s1-n3-cor-1 .statement}

Soient p un idéal premier de A et S une partie multiplicative de A ne rencontrant pas p. Alors $ \operatorname{ht}(p) = \operatorname{ht}(S^{-1}p) $.

Cela résulte de la prop. 7, a), et de II, § 2, n° 5, prop. 11.

#### Proposition 8 {#ac-viii-s1-prop-8 .statement}

Soit A un anneau.

a) On a $ \dim(A) = \sup_m \dim(A_m) = \sup_m \operatorname{ht}(m) $, où m parcourt l’ensemble des idéaux maximaux (resp. premiers) de A.

b) Soient b un idéal de A distinct de A et a un idéal de A contenu dans b. Alors on a $ \operatorname{codim}(V(b), V(a)) + \dim(A/b) \leq \dim(A/a) $. En particulier, pour tout idéal b de A distinct de A, on a l’inégalité $ \operatorname{ht}(b) + \dim(A/b) \leq \dim(A) $.

La première assertion résulte de la remarque 2 du n° 2 et de la prop. 7, b). La seconde résulte de la prop. 3, a) du n° 2 et des relations $ \dim(A/b) = \dim(V(b)) $, $ \dim(A/a) = \dim(V(a)) $.

#### Définition 7 {#ac-viii-s1-def-7 .statement}

On dit qu’un anneau A est caténaire si l’espace topologique Spec(A) est caténaire (n° 2, déf. 4).

Cela signifie donc que, pour tout couple (p, q) d’idéaux premiers de A tel que $ q \subset p $, toutes les chaînes saturées d’idéaux premiers de A d’extrémités p et q ont pour longueur $ \operatorname{codim}(V(p), V(q)) = \dim(A_p/qA_p) $.

#### Remarque 2 {#ac-viii-s1-n3-rem-2 .statement}

Tout anneau quotient d’un anneau caténaire est caténaire. Pour que l’anneau A soit caténaire, il faut et il suffit que, pour tout idéal premier p de A, l’anneau $ A_p $ soit caténaire.

#### Remarque 3 {#ac-viii-s1-n3-rem-3 .statement}

D’après la prop. 7, b) et la prop. 4 du n° 2, l’anneau A est caténaire si et seulement si, pour tout triplet (p, q, r) d’idéaux premiers de A tel que $ r \subset q \subset p $, on a dim(A_p/qA_p) + dim(A_q/rA_q) = dim(A_p/rA_p). Si A est intègre et de dimension finie, alors A est caténaire si et seulement si on a ht(q) + dim(A_p/qA_p) = ht(p) pour tout couple (p, q) d’idéaux premiers de A tel que q ⊂ p. En effet, l’espace topologique Spec(A) est alors irréductible et de dimension finie, et on applique le corollaire à la prop. 4 du n° 2.

#### Remarque 4 {#ac-viii-s1-n3-rem-4 .statement}

Soit A un anneau de dimension finie, dont toutes les chaînes maximales d’idéaux premiers ont même longueur. Alors A est caténaire, on a ht(p) + dim(A/p) = dim(A) pour tout idéal premier p de A, et dim(A_p/qA_p) + dim(A/p) = dim(A/q) pour tout couple (p, q) d’idéaux premiers de A tel que q ⊂ p (n° 2, prop. 5).

#### Remarque 5 {#ac-viii-s1-n3-rem-5 .statement}

Nous verrons au § 2, n° 4, que toute algèbre de type fini sur un corps est un anneau caténaire. Il existe des anneaux locaux noethériens qui ne sont pas caténaires (p. 83, exerc. 16).

### 4. Dimension d’un module de type fini

#### Définition 8 {#ac-viii-s1-def-8 .statement}

Soient A un anneau et M un A-module de type fini. On appelle dimension de Krull (ou simplement dimension $ ^1 $) du A-module M et on note $ \dim_A(M) $ (ou $ \dim(M) $ s’il n’y a pas d’ambiguïté) la dimension de Krull du support de M (II, § 4, n° 4, déf. 5).

Le support du A-module A est Spec(A); la dimension du A-module A est donc égale à la dimension de l’anneau A.

Soient M un A-module de type fini et α son annulateur ; on a

$$
\operatorname{Supp}(M) = V(\alpha) = \operatorname{Supp}(A/\alpha)
$$

(II, § 4, n° 4, prop. 17). Par suite coïncident la dimension du A-module M, la dimension du A-module A/α, la dimension de l’anneau A/α et la dimension du (A/α)-module M ; c’est la borne supérieure de l’ensemble des longueurs des chaînes $ p_0 \subset ... \subset p_n $ d’idéaux premiers de A telles que $ \alpha \subset p_0 $. D’après la prop. 6, c) du n° 3, la dimension de M est aussi la borne supérieure des dimensions des anneaux (ou des A-modules) A/p, où p parcourt l’ensemble des idéaux premiers de A, minimaux parmi ceux qui contiennent α.

#### Remarque 1 {#ac-viii-s1-n4-rem-1 .statement}

Soient A un anneau noethérien et M un A-module de type fini. Il est équivalent de dire que $ \dim_A(M) \leq 0 $, ou que les éléments de Supp(M) sont des idéaux maximaux de A, ou que M est de longueur finie (IV, § 2, n° 5, prop. 7).

#### Remarque 2 {#ac-viii-s1-n4-rem-2 .statement}

Si M est un module de type fini sur un anneau noethérien A, $ \dim_A(M) $ est la borne supérieure des nombres $ \dim(A/p) $, où p parcourt l’ensemble $ \operatorname{Ass}_A(M) $ des idéaux premiers de A associés à M (IV, § 1, n° 4, th. 2).

1 Si A est un corps, la dimension de Krull de M est $ \leq 0 $. Il y aura lieu de ne pas confondre la dimension de Krull de M et la dimension (ou rang) de l’espace vectoriel M sur le corps A (A, II, p. 97, déf. 1).

#### Proposition 9 {#ac-viii-s1-prop-9 .statement}

Soient $ A $ un anneau et $ M $ un $ A $-module de type fini.

a) Pour tout $ p \in \mathrm{Supp}(M) $, on a $ \dim_{A_p}(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M)) $.

b) $ \dim_A(M) $ est la borne supérieure des $ \dim_{A_p}(M_p) $, où $ p $ parcourt $ \mathrm{Spec}(A) $ (resp. où $ p $ parcourt l’ensemble des idéaux maximaux de $ A $ appartenant à $ \mathrm{Supp}(M) $).

c) Soit $ M' $ un sous-module de type fini de $ M $; alors

$$
\dim_A(M) = \sup(\dim_A(M'), \dim_A(M/M')) .
$$

a) Soit $ a $ l’annulateur de $ M $; alors l’annulateur du $ A_p $-module $ M_p $ est $ aA_p $ (II, § 2, n° 4, formule (9)), d’où $ \dim_{A_p}(M_p) = \dim(A_p/aA_p) $. On conclut par la prop. 7, b) du n° 3.

b) Cela résulte aussitôt de $ a) $ et du fait que $ \dim_{A_p}(M_p) = -\infty $ si $ p $ n’appartient pas à $ \mathrm{Supp}(M) $.

c) On a $ \mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M') $ (II, § 4, n° 4, prop. 16), et on applique la prop. 1 du n° 1.

#### Remarque 3 {#ac-viii-s1-n4-rem-3 .statement}

Sous les conditions de la prop. 9, c), on a $ \mathrm{codim}(\mathrm{Supp}(M), \mathrm{Spec}(A)) = \inf(\mathrm{codim}(\mathrm{Supp}(M'), \mathrm{Spec}(A)), \mathrm{codim}(\mathrm{Supp}(M/M'), \mathrm{Spec}(A))) $. Cela résulte de la formule $ \mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M') $ et de la remarque 4 du n° 2.

### 5. Cycles associés à un module

Dans ce numéro, on note $ A $ un anneau noethérien.

Soit $ Z(A) $ le $ \mathbf{Z} $-module libre de base l’ensemble des parties fermées irréductibles de $ \mathrm{Spec}(A) $; pour toute partie fermée irréductible $ Y $ de $ \mathrm{Spec}(A) $, on note $ [Y] $ l’élément correspondant de $ Z(A) $. Les éléments de $ Z(A) $ s’appellent parfois des cycles.

Soit $ M $ un $ A $-module de type fini. Pour tout idéal premier $ p $ de $ A $ qui est un élément minimal de $ \mathrm{Supp}(M) $, on a $ 0 < \mathrm{long}_{A_p}(M_p) < \infty $ (IV, § 2, n° 5, cor. 2 à la prop. 7 et § 1, n° 4, th. 2); on pose

$$
z(M) = \sum_p \mathrm{long}_{A_p}(M_p).[V(p)] ,
$$

où $ p $ parcourt l’ensemble fini des idéaux premiers minimaux de $ \mathrm{Supp}(M) $.

#### Remarque {#ac-viii-s1-n5-rem-1 .statement}

Pour tout $ p \in \mathrm{Spec}(A) $, on a $ z(A/p) = [V(p)] $. Plus généralement, soit $ M $ un $ A $-module de type fini, et soit $ (M_i)_{0 \leq i \leq n} $ une suite de composition de $ M $ telle que pour $ 0 \leq i \leq n-1 $, le module $ M_i/M_{i+1} $ soit isomorphe à $ A/p_i $, où $ p_i $ est un idéal premier de $ A $ (cf. IV, § 1, n° 4, th. 1); alors on a $ z(M) = \sum_{i \in J} [V(p_i)] $, où $ J $ est la partie de $ I $ formée des $ i $ tels que $ p_i $ soit un élément minimal de $ \{ p_0, ..., p_{n-1} \} $ (IV, § 1, n° 4, th. 2 et § 2, n° 5, remarque 1).

Pour tout entier $ d $, notons $ Z_{\leq d} $ (resp. $ Z_d $, resp. $ Z^{>d} $, resp. $ Z^d $) le sous-$ \mathbf{Z} $-module de $ Z(A) $ engendré par les éléments $ [V(p)] $ où $ p $ est un idéal premier de $ A $ tel que $ \dim(A/p) \leq d $ (resp. $ \dim(A/p) = d $, resp. $ \mathrm{ht}(p) \geq d $, resp. $ \mathrm{ht}(p) = d $). On dit que les éléments de $ Z_d $ (resp. $ Z^d $) sont les cycles de dimension $ d $ (resp. de codimension $ d $). On a évidemment
$$
Z_{\leq d} = Z_{\leq d-1} \oplus Z_d,\quad Z^{>d} = Z^{>d+1} \oplus Z^d.
$$
Soit par ailleurs $ C $ l’ensemble des classes de $ A $-modules de type fini (A, VIII, § 3, n° 5), et pour chaque entier $ d $, soit $ C_{\leq d} $ (resp. $ C^{>d} $) la partie de $ C $ formée des classes de $ A $-modules de type fini de dimension $ \leq d $ (resp. dont le support est de codimension $ \geq d $ dans $ \mathrm{Spec}(A) $).

#### Lemme 1 {#ac-viii-s1-lem-1 .statement}

*Soient $ M $ un $ A $-module de type fini et $ d $ un entier.*
  *a*) *Pour que $ M $ soit de type $ C_{\leq d} $, il faut et il suffit que $ z(M) \in Z_{\leq d} $; la projection $ z_d(M) $ de $ z(M) $ sur $ Z_d $ parallèlement à $ Z_{\leq d-1} $ est alors donnée par*
$$
z_d(M) = \sum_{\dim(A/p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$
  *b*) *Pour que $ M $ soit de type $ C^{>d} $, il faut et il suffit que $ z(M) \in Z^{>d} $; la projection $ z^d(M) $ de $ z(M) $ sur $ Z^d $ parallèlement à $ Z^{>d+1} $ est alors donnée par*
$$
z^d(M) = \sum_{\mathrm{ht}(p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$

Pour que $ M $ soit de type $ C_{\leq d} $, c’est-à-dire de dimension $ \leq d $, il faut et il suffit que pour tout idéal premier minimal $ p $ de $ \mathrm{Supp}(M) $, on ait $ \dim(A/p) \leq d $, ce qui signifie que $ z(M) \in Z_{\leq d} $. Supposons qu’on ait $ \dim(M) \leq d $, et soit $ p \in \mathrm{Spec}(A) $ tel que $ \dim(A/p) = d $; alors, ou bien $ p \notin \mathrm{Supp}(M) $ et donc $ M_p = 0 $, ou bien $ p \in \mathrm{Supp}(M) $, et $ p $ est un élément minimal de $ \mathrm{Supp}(M) $; le coefficient de $ [V(p)] $ dans $ z(M) $ est dans les deux cas $ \mathrm{long}_{A_p}(M_p) $, d’où *a)*. La partie *b)* se démontre de façon analogue ; on notera qu’un module $ M $ de type fini est de type $ C^{>d} $ si et seulement si l’on a $ M_p = 0 $ pour tout idéal premier $ p $ de hauteur $ < d $.

D’après la prop. 9, *c)* et la remarque 3 du n° 4, les ensembles $ C_{\leq d} $ et $ C^{>d} $ sont héréditaires (A, VIII, § 10, n° 1, déf. 1), et l’on peut considérer les groupes de Grothendieck $ K(C_{\leq d}) $ et $ K(C^{>d}) $ correspondants (*loc. cit.*, n° 2); pour tout $ A $-module $ M $ de type $ C_{\leq d} $ (resp. $ C^{>d} $), notons $ [M]_{\leq d} $ (resp. $ [M]^{>d} $) l’élément associé dans $ K(C_{\leq d}) $ (resp. $ K(C^{>d}) $). D’après le lemme 1, les fonctions $ z_d $ et $ z^d $ sont additives ; il existe donc (*loc. cit.*, prop. 3) des homomorphismes
$$
\zeta_d : K(C_{\leq d}) \to Z_d,\quad \zeta^d : K(C^{>d}) \to Z^d
$$
tels que $ \zeta_d([M]_{\leq d}) = z_d(M) $ pour tout $ A $-module $ M $ de type $ C_{\leq d} $ et $ \zeta^d([N]^{>d}) = z^d(N) $ pour tout $ A $-module $ N $ de type $ C^{>d} $. Par ailleurs, puisque $ C_{\leq d-1} \subset C_{\leq d} $ et $ C^{>d+1} \subset C^{>d} $, on a des homomorphismes canoniques
$$
i_d : K(C_{\leq d-1}) \to K(C_{\leq d})\quad \text{et}\quad i^d : K(C^{>d+1}) \to K(C^{>d}).
$$
Avec ces notations :

#### Proposition 10 {#ac-viii-s1-prop-10 .statement}

Les suites de $ \mathbf{Z} $-modules et d’homomorphismes

$$
\begin{array}{cccccc}
K(\mathcal{C}_{\leq d-1}) & \xrightarrow{i_d} & K(\mathcal{C}_{\leq d}) & \xrightarrow{\zeta_d} & Z_d & \longrightarrow 0 \\
K(\mathcal{C}^{>d+1}) & \xrightarrow{i_d} & K(\mathcal{C}^{>d}) & \xrightarrow{\zeta_d} & Z^d & \longrightarrow 0
\end{array}
$$

sont exactes.

On a $ \zeta_d \circ i_d = 0 $ d’après le lemme 1. Pour tout $ p \in \mathrm{Spec}(A) $ tel que $ \dim(A/p) = d $, on a $ \zeta_d([A/p]_{\leq d}) = z_d(A/p) = [V(p)] $, donc l’homomorphisme $ \zeta_d $ est surjectif. D’après IV, § 1, no 4, th. 1, $ K(\mathcal{C}_{\leq d}) $ est engendré par les $ [A/p]_{\leq d} $, où $ p \in \mathrm{Spec}(A) $ et $ \dim(A/p) \leq d $; par conséquent, tout élément $ \xi $ de $ K(\mathcal{C}_{\leq d}) $ peut s’écrire $ \xi = i_d(\eta) + \sum_{i=1}^k n_i[A/p_i]_{\leq d} $, avec $ \eta \in K(\mathcal{C}_{\leq d-1}) $, $ n_i \in \mathbf{Z} $ et $ \dim(A/p_i) = d $ pour $ 1 \leq i \leq k $; on a $ \zeta_d(\xi) = \sum_{i=1}^k n_i[V(p_i)] $ et par conséquent $ \zeta_d(\xi) = 0 $ implique $ \xi = i_d(\eta) \in \mathrm{Im}(i_d) $, d’où $ \mathrm{Ker}(\zeta_d) = \mathrm{Im}(i_d) $.

On raisonne de même pour la seconde suite.

#### Exemple 1 {#ac-viii-s1-n5-exa-1 .statement}

Supposons A noethérien et intègre. Alors on a $ Z^0 = \mathbf{Z}.[\mathrm{Spec}(A)] $; on a $ \mathcal{C}^{>0} = \mathcal{C} $ et $ z^0(M) = \mathrm{rg}(M).[Spec(A)] $. Les modules de type $ \mathcal{C}^{>1} $ sont donc les modules de torsion.

#### Exemple 2 {#ac-viii-s1-n5-exa-2 .statement}

Supposons A noethérien et intégralement clos. Alors $ Z^1 $ s’identifie au groupe $ D(A) $ des diviseurs de A introduit au chapitre VII (§ 1, no 3, th. 2, et no 6, th. 3). Les modules de type $ \mathcal{C}^{>2} $ sont les modules pseudo-nuls (VII, § 4, no 4, déf. 2); si M est un module de torsion de type fini, alors $ z^1(M) \in Z^1 = D(A) $ est le contenu $ \chi(M) $ de M (VII, § 4, no 5, déf. 4). Les prop. 10 et 11 de loc. cit. sont donc équivalentes à l’exactitude de la suite $ K(\mathcal{C}^{>2}) \to K(\mathcal{C}^{>1}) \to Z^1 \to 0 $.

#### Exemple 3 {#ac-viii-s1-n5-exa-3 .statement}

Les modules de type $ \mathcal{C}_{\leq 0} $ sont les modules de dimension $ \leq 0 $, c’est-à-dire les modules de longueur finie (no 4, remarque 1). On a $ \mathrm{long}_A(M) = \varepsilon(z_0(M)) $ pour tout A-module de longueur finie M, où $ \varepsilon : Z_0 \to \mathbf{Z} $ associe à la combinaison linéaire $ \sum_m n_m[V(m)] $ l’entier $ \sum_m n_m $ (IV, § 2, no 5, corollaire à la prop. 8).

#### Exemple 4 {#ac-viii-s1-n5-exa-4 .statement}

Supposons A intègre et de dimension finie. Posons $ d = \dim(A) $. Alors on a $ \mathcal{C}_{\leq d} = \mathcal{C} $, $ Z_d = \mathbf{Z}.[\mathrm{Spec}(A)] = Z^0 $, $ z_d(M) = \mathrm{rg}(M).[Spec(A)] = z^0(M) $, et les modules de type $ \mathcal{C}_{\leq d-1} $ sont les modules de torsion.

## EXERCICES {#ac-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
