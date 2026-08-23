---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 8
section_title: Convergence de la série de Hausdorff (cas ultramétrique)
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0064-0069, 0090-0092
extraction: ocr
subsections:
    - "no": 1
      title: Majoration $ p $-adique des séries exp, log et H
      page: 0
      pdf_page: 64
    - "no": 2
      title: Algèbres de Lie normées
      page: 0
      pdf_page: 65
    - "no": 3
      title: Groupe défini par une algèbre de Lie normée complète
      page: 0
      pdf_page: 66
    - "no": 4
      title: Exponentielle dans les algèbres associatives normées complètes
      page: 0
      pdf_page: 67
statements: 9
exercises: 4
content_sha256: d3bd3f5080f5a761023fe77d33cd5cd81a5f28ede384d5a4918629b6ad89b68f
---

## § 8. Convergence de la série de Hausdorff (cas ultramétrique)

Dans ce paragraphe, on suppose que K est un corps valué complet non discret de caractéristique zéro, à valeur absolue ultramétrique. On désigne par $ p $ la caractéristique du corps résiduel de K (AC, VI, § 3, n° 2).

Si $ p \neq 0 $, on pose $ a = |p| $; on sait (AC, VI, § 6, n°s 2 et 3) que $ 0 < a < 1 $, et qu’il existe une valuation $ v $ de K à valeurs dans $ \mathbf{R} $, et une seule, dont la restriction à $ \mathbf{Q} $ est la valuation $ p $-adique $ v_p $, et qui est telle que $ |x| = a^{v(x)} $ pour tout $ x \in K $. On pose d’autre part:

$$
\theta = \frac{1}{p - 1}.
$$

Si $ p = 0 $, on désigne par $ a $ un nombre réel tel que $ 0 < a < 1 $, et par $ v $ une valuation de K à valeurs dans $ \mathbf{R} $ telle que $ |x| = a^{v(x)} $ pour tout $ x \in K $ (loc. cit.). On a $ v(x) = 0 $ pour $ x \in \mathbf{Q}^* $. On pose d’autre part:

$$
\theta = 0.
$$

### 1. Majoration $ p $-adique des séries exp, log et H

Dans ce numéro, on suppose $ p \neq 0 $.

#### Lemme 1 {#lie-ii-s8-lem-1 .statement}

Soit $ n $ un entier $ \geqslant 0 $, et soit $ n = n_0 + n_1 p + \cdots + n_k p^k $, avec $ 0 \leqslant n_i \leqslant p - 1 $, le développement $ p $-adique de $ n $. Soit $ S(n) = n_0 + n_1 + \cdots + n_k $. Alors

$$
v_p(n!) = \frac{n - S(n)}{p - 1}.
$$

En effet, on a $ v_p(n!) = \sum_{i=1}^n v_p(i) $, et le nombre d’entiers $ i $ compris entre 1 et $ n $ pour lesquels $ v_p(i) \geqslant j $ est égal à la partie entière $ [n/p^j] $ de $ n/p^j $. On a donc:

$$
v_p(n!) = \sum_{j \geqslant 0} j ([n/p^j] - [n/p^{j+1}]) = \sum_{j \geqslant 1} [n/p^j].
$$

Comme $ [n/p^j] = \sum_{i \geqslant j} n_i p^{i-j} $, le lemme en résulte.

#### Lemme 2 {#lie-ii-s8-lem-2 .statement}

On a $ v(n) \leqslant v(n!) \leqslant (n - 1)\theta $ et $ v(n) \leqslant (\log n)/(\log p) $ pour tout entier $ n \geqslant 1 $.

En effet $ v(n!) = v_p(n!) = (n - S(n))\theta \leqslant (n - 1)\theta $ d’après le lemme 1.
D’autre part, $ n \geqslant p^{v(n)} $, d’où $ v(n) \leqslant (\log n)/(\log p) $.

Soit $ I = \{U, V\} $ un ensemble à deux éléments, et soit

$$
H = \sum_{r,s \geqslant 0} H_{r,s}(U, V) \in \hat{L}_{\mathbf{Q}}(I)
$$

la série de Hausdorff (\S 6, n° 4, déf. 1). Soient $ \mathbf{Z}_{(p)} $ l’anneau local de $ \mathbf{Z} $ relativement à l’idéal premier $ (p) $, et $ (e_b)_{b \in B} $ une base de $ L_{\mathbf{Z}_{(p)}}(\mathbf{I}) $ sur $ \mathbf{Z}_{(p)} $ (\S 2, n° 11, th. 1). C’est aussi une base de $ L_\mathbf{Q}(\mathbf{I}) $ sur $ \mathbf{Q} $.

#### Proposition 1 {#lie-ii-s8-prop-1 .statement}

*Soient r et s deux entiers $ \geqslant 0 $. Si $ H_{r,s} = \sum_{b \in B} \lambda_b e_b $, où $ \lambda_b \in \mathbf{Q} $, est la décomposition de $ H_{r,s} $ par rapport à la base $ (e_b)_{b \in B} $, on a*
$$
v_p(\lambda_b) \geqslant -(r + s - 1)\theta \quad \text{pour tout } b \in B.
$$
L’anneau $ A_{\mathbf{Z}_{(p)}}(\mathbf{I}) $ s’identifie au sous-$ \mathbf{Z}_{(p)} $-module de $ A_\mathbf{Q}(\mathbf{I}) $ engendré par les mots $ w \in Mo(\mathbf{I}) $. Comme $ L_{\mathbf{Z}_{(p)}}(\mathbf{I}) $ est facteur direct dans $ A_{\mathbf{Z}_{(p)}}(\mathbf{I}) $, on a
$$
L_{\mathbf{Z}_{(p)}}(\mathbf{I}) = A_{\mathbf{Z}_{(p)}}(\mathbf{I}) \cap L_\mathbf{Q}(\mathbf{I}).
$$
Soit $ f $ l’entier tel que $ f \leqslant (r + s - 1)\theta < f + 1 $. La relation (4) équivaut à $ v_p(\lambda_b) \geqslant -f $ pour tout $ b \in B $, c’est-à-dire à $ H_{r,s} \in p^{-f}L_{\mathbf{Z}_{(p)}}(\mathbf{I}) $. Or cela équivaut aussi, d’après (5), à $ H_{r,s} \in p^{-f}A_{\mathbf{Z}_{(p)}}(\mathbf{I}) $.

D’après la formule (11) du \S 6, n° 4, il suffit de montrer que, quel que soit l’entier $ m \geqslant 1 $ et quels que soient les entiers $ r_1, \ldots, r_m, s_1, \ldots, s_m $ tels que
$$
r_1 + \cdots + r_m = r, \qquad s_1 + \cdots + s_m = s,
$$
$$
r_i + s_i \geqslant 1 \quad \text{pour } 1 \leqslant i \leqslant m,
$$
on a
$$
v_p(m!r_1!\ldots r_m!s_1!\ldots s_m!) \leqslant f.
$$
Or, d’après le lemme 2, $ v_p(r_i!s_i!) \leqslant (r_i + s_i - 1)\theta $ et $ v_p(m!) \leqslant v_p(m!) \leqslant (m - 1)\theta $; le premier membre de (7) est donc majoré par $ \theta(m - 1 + \sum_{i=1}^m (r_i + s_i - 1)) = \theta(r + s - 1) $; comme c’est un entier, il est $ \leqslant f $, ce qui achève la démonstration.

### 2. Algèbres de Lie normées

#### Définition 1 {#lie-ii-s8-def-1 .statement}

*On appelle algèbre de Lie normée sur $ \mathbf{K} $ une algèbre de Lie munie d’une norme telle que*
$$
\|x + y\| \leqslant \sup(\|x\|, \|y\|)
$$
$$
\|[x, y]\| \leqslant \|x\| \cdot \|y\|
$$
*quels que soient x, y dans g.*

Dans tout le reste de ce paragraphe, on désigne par $ g $ une algèbre de Lie normée complète.

Pour tout ensemble fini $ \mathbf{I} $, on définit comme au \S 7, n° 1, un homomorphisme continu $ u \mapsto \tilde{u} $ d’algèbres de Lie de $ \hat{L}(\mathbf{I}) $ dans $ \hat{P}(g^\mathbf{I}; g) $. On voit comme au \S 7 que si $ u = \sum_v u_v $, avec $ u_v \in L^v(\mathbf{I}) $ pour $ v \in \mathbf{N}^\mathbf{I} $, alors $ \tilde{u} = \sum_v \tilde{u}_v $, où $ \tilde{u}_v $ est l’application polynomiale $ (t_i)_{i \in \mathbf{I}} \mapsto u_v((t_i)) $ définie au \S 2, n° 4. La formule de composition (2) du \S 7, n° 1, reste valable.

### 3. Groupe défini par une algèbre de Lie normée complète

Soit $ H = \sum_{r \geq 0} H_{r,s} \in \hat{L}(\{U, V\}) $ la série de Hausdorff (\S 6, n° 4, déf. 1). Nous allons montrer que la série formelle à composantes continues correspondante

(10)
$$
\tilde{H} = \sum_{r,s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$
est convergente (VAR, R, 4.1.1).

Soient $ r \geq 0, s \geq 0 $, tels que $ r + s \neq 0 $ et soit $ \| \tilde{H}_{r,s} \| $ la norme du polynôme continu $ \tilde{H}_{r,s} $ (VAR, R, App., n° 2).

#### Lemme 3 {#lie-ii-s8-lem-3 .statement}

*On a*
$$
\| \tilde{H}_{r,s} \| \leq a^{-(r+s-1)\theta}.
$$

Soit B un ensemble de Hall relatif à I, et soit $ H_{r,s} = \sum_{b \in B} \lambda_b e_b $ la décomposition de $ H_{r,s} $ par rapport à la base correspondante de $ L(\{U, V\}) $. On a
(11)
$$
|\lambda_b| \leq a^{-(r+s-1)\theta}.
$$
En effet, cela est trivial pour $ p = 0 $, car $ \lambda_b \in \mathbf{Q} $; et cela résulte de la prop. 1 du n° 1 pour $ p \neq 0 $.

De plus, on a
(12)
$$
\| \tilde{e}_b \| \leq 1 \quad \text{pour } b \in B.
$$
En effet, montrons, plus généralement, par récurrence sur $ n $, que pour tout alternant $ b $ de degré $ n $ en les deux indéterminées U et V (\S 2, n° 6), on a $ \| \tilde{b} \| \leq 1 $. Si $ n = 1 $, $ \tilde{b} $ est une des projections de $ g \times g $ sur $ g $, donc est de norme $ \leq 1 $; si $ n > 1 $, il existe deux alternants $ b_1 $ et $ b_2 $ de degrés $ < n $, tels que $ b = [b_1, b_2] $. Comme l’application $ \gamma : (x, y) \mapsto [x, y] $ de $ g \times g \to g $ est bilinéaire de norme $ \leq 1 $, on a (VAR, R, App., n° 4)
(13)
$$
\| \tilde{b} \| = \| \gamma \circ (\tilde{b}_1, \tilde{b}_2) \| \leq \| \tilde{b}_1 \| \cdot \| \tilde{b}_2 \| \leq 1.
$$
Les relations (11) et (12) entraînent le lemme.

#### Proposition 2 {#lie-ii-s8-prop-2 .statement}

*La série formelle $ \tilde{H} $ est une série convergente* (VAR, R, 4.1.1). *Si G est la boule* $ \{ x \in g \mid \| x \| < a^\theta \} $, *le domaine de convergence strict de* $ \tilde{H} $ (VAR, R, 4.1.3) *contient* $ G \times G $.

En effet, si $ u $ et $ v $ sont deux nombres réels $ > 0 $ tels que $ u < a^\theta $ et $ v < a^\theta $, on a (lemme 3)
(14)
$$
\| \tilde{H}_{r,s} \| u^r v^s \leq a^\theta (u a^{-\theta})^r (v a^{-\theta})^s
$$
et $ \| \tilde{H}_{r,s} \| u^r v^s $ tend vers 0 lorsque $ r + s $ tend vers l’infini.

Notons $ h : G \times G \to g $ la fonction analytique (VAR, R, 4.2.4) définie par $ \tilde{H} $, c’est-à-dire par la formule
$$
(15) \quad h(x, y) = \sum_{r,s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r,s \geq 0} H_{r,s}(x, y) \quad \text{pour } (x, y) \in G \times G.
$$
Cette fonction s’appelle la fonction de Hausdorff de $ g $.
Soit $ (x, y) \in G \times G $. On a
$$
(16) \quad \| \tilde{H}_{r,s}(x, y) \| \leq \sup(\|x\|, \|y\|)
$$
$$
(17) \quad \| h(x, y) \| \leq \sup(\|x\|, \|y\|).
$$
En effet (17) résulte aussitôt de (16), et (16) est trivial pour $ r = s = 0 $; si $ r \geq 1 $, on a
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \| \tilde{H}_{r,s} \| \|x\|^r \|y\|^s \\
\leq \|x\| \left( \frac{\|x\|}{a^\theta} \right)^{r-1} \left( \frac{\|y\|}{a^\theta} \right)^s \\
\leq \|x\|;
$$
on raisonne de façon analogue si $ s \geq 1 $.
En particulier, $ \|h(x, y)\| < a^\theta $ pour $ (x, y) \in G \times G $.

#### Proposition 3 {#lie-ii-s8-prop-3 .statement}

Soit $ G $ la boule $ \{ x \in g \mid \|x\| < a^\theta \} $. L’application analytique $ h : G \times G \to G $ fait de $ G $ un groupe, dans lequel $ 0 $ est élément neutre et $ -x $ inverse de $ x $ pour tout $ x \in G $. De plus, si $ R $ est un nombre réel tel que $ 0 < R < a^\theta $, la boule $ \{ x \in g \mid \|x\| < R \} $ (resp. $ \{ x \in g \mid \|x\| \leq R \} $) est un sous-groupe ouvert de $ G $.
Comme $ H(U, -U) = 0 $ et $ H(0, U) = H(U, 0) = U $, on a $ h(x, -x) = 0 $ et $ h(0, x) = h(x, 0) = x $ pour tout $ x \in G $. Il ne reste donc qu’à démontrer la formule d’associativité
$$
(18) \quad h(h(x, y), z) = h(x, h(y, z)) \quad \text{pour } x, y, z \text{ dans } G.
$$
Comme on a
$$
H(H(U, V), W) = H(U, H(V, W))
$$
dans $ \hat{L}(\{U, V, W\}) $ (\S 6, n° 5, prop. 4), on a
$$
(19) \quad \tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H})
$$
dans $ \hat{P}(g \times g \times g; g) $ (n° 2), et (19) entraîne (18) d’après (16) et VAR, R, 4.1.5.
*Autrement dit (chap. III, § 1), G, muni de la fonction de Hausdorff, est un groupe de Lie.*

### 4. Exponentielle dans les algèbres associatives normées complètes
Dans ce n°, on désigne par A une algèbre associative unifière munie d’une norme $ x \mapsto \|x\| $ satisfaisant aux conditions:
$$
\begin{align*}
\|x + y\| &\leq \sup(\|x\|, \|y\|) \\
\|xy\| &\leq \|x\| \cdot \|y\| \\
\|1\| &= 1
\end{align*}
$$

Prenons $ I = \{ U \} $ et considérons les images $ \tilde{e} $ et $ \tilde{l} $ des séries $ e(U) = \sum_{n \geq 1} \frac{U^n}{n!} $ et
$$
l(U) = \sum_{n \geq 1} (-1)^{n-1} \frac{U^n}{n} \text{ dans } \hat{P}(A; A). \text{ On a:}
$$
(20)
$$
\left\| \left( \frac{U^n}{n!} \right)^{\sim} \right\| \leq a^{-(n-1)\theta}
$$
(21)
$$
\left\| \left( \frac{U^n}{n} \right)^{\sim} \right\| \leq a^{-\frac{\log n}{\log p}}
$$
d’après le lemme 2 du n° 1. Donc le rayon de convergence strict de la série $ \tilde{e} $ (resp. $ \tilde{l} $) est $ \geq a^\theta $ (resp. $ \geq 1 $) (VAR, R, 4.1.3). Pour $ R > 0 $, soit $ G_R = \{ x \in A \mid \|x\| < R \} $; posons $ G = G_{a^\theta} $. La série $ \tilde{e} $ (resp. $ \tilde{l} $) définit une application analytique $ e_A $ (resp. $ l_A $) de $ G $ (resp. $ G_1 $) dans $ A $. On posera:
(22)
$$
\exp_A(x) = 1 + e_A(x) = \sum_{n \geq 0} \frac{x^n}{n!} \quad \text{pour } x \in G
$$
(23)
$$
\log_A(x) = l_A(x-1) = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad \text{pour } x-1 \in G_1
$$
(on omet l’indice $ A $ quand aucune confusion n’est à craindre). Pour $ x \in G_R $ et $ n \geq 1 $, on a
(24)
$$
\left\| \frac{x^n}{n} \right\| \leq \left\| \frac{x^n}{n!} \right\| < R^n a^{-(n-1)\theta} = R \left( \frac{R}{a^\theta} \right)^{n-1}
$$
donc $ e_A(G_R) \subset G_R, l_A(G_R) \subset G_R $ pour $ R \leq a^\theta $.

#### Proposition 4 {#lie-ii-s8-prop-4 .statement}

*Soit $ R $ un nombre réel tel que $ 0 < R \leq a^\theta $. L’application $ \exp_A $ définit un isomorphisme analytique de $ G_R $ sur $ 1 + G_R $, et l’isomorphisme réciproque est la restriction de $ \log_A $ à $ 1 + G_R $.*

On a $ e(l(X)) = l(e(X)) = X $. D’après (20), (21), et VAR, R, 4.1.5, on en déduit que $ e_A(l_A(x)) = l_A(e_A(x)) $ pour $ x \in G_R $. Donc
$$
\begin{align*}
\exp_A(\log_A x) &= x & \text{pour } x \in 1 + G_R \\
\log_A(\exp_A x) &= x & \text{pour } x \in G_R
\end{align*}
$$
ce qui achève la démonstration.

Si on munit $ A $ du crochet $ [x, y] = xy - yx $, $ A $ devient une algèbre de Lie normée complète, car $ \|xy - yx\| \leq \sup(\|xy\|, \|yx\|) \leq \|x\| \cdot \|y\| $. La prop. 2 du n° 3 entraîne que le domaine de convergence strict de $ \tilde{H} $ contient $ G \times G $, et $ \tilde{H} $ définit donc une fonction analytique $ h : G \times G \to A $; on a
(25)
$$
h(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y).
$$

#### Proposition 5 {#lie-ii-s8-prop-5 .statement}

Pour $ x, y $ dans $ G $, on a

$$
\exp_A x \cdot \exp_A y = \exp_A h(x, y).
$$

En effet, on a $ e^U e^V = e^{H(U, V)} $, donc

$$
m \circ (1 + \tilde{\epsilon}, 1 + \tilde{\epsilon}) = (1 + \tilde{\epsilon}) \circ \tilde{H}
$$

dans $ \tilde{H}(A \times A; A) $ (en désignant par $ m $ la multiplication de $ A $). La proposition résulte alors de la prop. 2, du lemme 3, et de VAR, R, 4.1.5.

## EXERCICES {#lie-ii-s8-exercises}

On suppose que la caractéristique résiduelle $ p $ du corps $ K $ est $ > 0 $. On note $ \mathfrak{o}_K $ l’anneau de la valuation $ v $ de $ K $.

See the [exercises for § 8](exercises/s8/).
