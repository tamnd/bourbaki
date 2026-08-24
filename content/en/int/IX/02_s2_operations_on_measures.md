---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 2
section_title: Operations on measures
lang: en
source: int-vii-ix
book_pages: INT IX.22-INT IX.41, INT IX.108
pdf_pages: 0204-0223, 0290-0290
extraction: ocr
subsections:
    - "no": 1
      title: Induced measure on a measurable subspace
      page: 22
      pdf_page: 204
    - "no": 2
      title: Measures defined by numerical densities
      page: 24
      pdf_page: 206
    - "no": 3
      title: Image of a measure
      page: 26
      pdf_page: 208
    - "no": 4
      title: Lifting of measures
      page: 29
      pdf_page: 211
    - "no": 5
      title: Product of two measures
      page: 31
      pdf_page: 213
    - "no": 6
      title: Integration with respect to the product of two measures
      page: 33
      pdf_page: 215
    - "no": 7
      title: A result on the disintegration of measures
      page: 37
      pdf_page: 219
statements: 38
exercises: 3
content_sha256: f05688e7f5e86ff2ea2066658769980a5ad9e44095245e34f9e9d06f1fa0ab07
---

## § 2. OPERATIONS ON MEASURES

As in the preceding section, $ T $ denotes a Hausdorff topological space, and $ \mu $ a measure on $ T $. Recall that all measures are assumed positive, absent mention to the contrary.

### 1. Induced measure on a measurable subspace

Let $ X $ be a subset of $ T $, and let $ \nu $ be the restriction of the mapping $ \mu : K \mapsto \mu_K $ to the set of compact subsets of $ X $; it is clear that $ \nu $ is a premeasure on $ X $. On the other hand, let $ x \in X $ and let $ V $ be an open neighborhood of $ x $ in $ T $ such that $ \mu^\bullet(V) < +\infty $; then

$$
\nu^\bullet(X \cap V) = \sup_{\substack{K \text{ compact} \\ K \subset X \cap V}} \mu^\bullet(K) \leq \mu^\bullet(V) < +\infty
$$

by *Remark 3* of §1, No. 2, so that $ \nu $ is a measure.

When $ X $ is not $ \mu $-measurable, the encumbrances $ \nu^\bullet $ and $ (\mu^\bullet)_X $ are not necessarily equal and the measure $ \nu $ presents no interest.

#### Definition 1 {#int-ix-s2-def-1 .statement}

*Let $ X $ be a $ \mu $-measurable subset of $ T $. The restriction of $ \mu : K \mapsto \mu_K $ to the set of compact subsets of $ X $ is called the measure induced by $ \mu $ on the subspace $ X $, and is denoted by $ \mu_X $ or $ \mu|X $.*

#### Proposition 1 {#int-ix-s2-prop-1 .statement}

*Let $ X $ be a $ \mu $-measurable subset of $ T $. The encumbrance $ (\mu_X)^\bullet $ is equal to the encumbrance $ (\mu^\bullet)_X $ induced by $ \mu^\bullet $ on $ X $ (§1, No. 1). In other words, $ (\mu_X)^\bullet(g) = \mu^\bullet(g^0) $ for every function $ g \in \mathcal{F}_+(X) $.

Let $ f \in \mathcal{F}_+(X) $ and let $ f^0 $ be the extension by 0 of $ f $ to $ T $. One has $ (\mu^\bullet)_X(f) = \mu^\bullet(f^0) = \sup_L \mu^\bullet(f^0 \varphi_L) $, where $ L $ runs over the set of compact subsets of $ T $ (§1, No. 2, Prop. 2); similarly $ (\mu_X)^\bullet(f) = \sup_K \mu_K^\bullet(f_K) = \sup_K \mu^\bullet(f^0 \varphi_K) $, where $ K $ runs over the set of compact subsets of $ X $. Thus it all comes down to showing that $ \mu^\bullet(f^0 \varphi_L) = \sup_K \mu^\bullet(f^0 \varphi_K) $ for every compact subset $ L $ of $ T $, where $ K $ runs over the set of compact subsets of $ L \cap X $. Now, let $ (K_n) $ be an increasing sequence of compact sets contained in $ L \cap X $, such that $ (L \cap X) - \bigcup_n K_n $ is locally $ \mu $-negligible (§1, No. 8, Prop. 11); $ f^0 $ being zero outside $ X $, $ f^0 \varphi_L $ is zero outside $ L \cap X $ hence is equal locally almost everywhere to the upper envelope of the sequence $ (f^0 \varphi_{K_n}) $. This implies that $ \mu^\bullet(f^0 \varphi_L) = \sup_n \mu^\bullet(f^0 \varphi_{K_n}) $, whence the desired result.*

#### Remark 1 {#int-ix-s2-n1-rem-1 .statement}

The relation $ (\mu_X)^\bullet = (\mu^\bullet)_X $ permits using the notation $ \mu_X^\bullet $ without ambiguity; we shall do so henceforth. The preceding Prop. 1 and Prop. 2 of §1, No. 2 show that the measures denoted $ \mu_K $ until now, for $ K $ compact, are indeed induced measures in the sense of Def. 1. Similarly, if $ T $ is locally compact, and if $ X $ is a locally compact subspace of $ T $, the above Prop. 1 and Prop. 1 of Ch. V, §7, No. 1 show that Def. 1 coincides with the definition of Ch. IV, §5, No. 7.

#### Remark 2 {#int-ix-s2-n1-rem-2 .statement}

Def. 1 may be extended to the case that $ \mu $ is a complex measure on $ T $. To show in this case that the premeasure $ \mu_X $ is a measure, it suffices to observe that $ |\mu_K| = |\mu|_K $ for every compact subset $ K $ of $ X $ (§1, No. 2).

By Prop. 1, a subset $ Y $ of $ X $ is $ \mu_X $-measurable (resp. locally $ \mu_X $-negligible) if and only if it is $ \mu $-measurable (resp. locally $ \mu $-negligible). If $ Y $ is $ \mu_X $-measurable, hence $ \mu $-measurable, the induced measures $ (\mu_X)_Y $ and $ \mu_Y $ are obviously equal by virtue of Prop. 1 (*transitivity of induced measures*).

Remark 3). — Let X be a $ \mu $-measurable subset of T. By Prop. 10 of §1, No. 8, applied to $ g = \varphi_X $, there exists a crushing $ (K_\alpha)_{\alpha \in A} $ of T such that for each $ \alpha \in A $, either $ K_\alpha \subset X $ or $ K_\alpha \subset \mathbf{C}X $. If one modifies the topology of T by the procedure of the Scholium of §1, No. 8, the space $ X' $ obtained by equipping X with the topology induced by $ T' $ is locally compact, and one knows how to associate to $ \mu $ (resp. to $ \mu_X $) a measure $ \mu' $ (resp. $ \nu $) on $ T' $ (resp. on $ X' $) that admits the same essential upper integral as $ \mu $ (resp. $ \mu_X $): this implies that $ \mu'_{X'} = \nu $. Since the locally negligible sets, measurable mappings, and essentially integrable functions with values in a Banach space, are the same for $ \mu $ and $ \mu' $, and for $ \mu_X $ and $ (\mu_X)' = \nu = \mu'_{X'} $, the theory of integration with respect to an induced measure reduces to that which was treated in Ch. V, §7 in the special case of locally compact spaces. We leave to the reader the task of transcribing the results.

### 2. Measures defined by numerical densities

#### Definition 2 {#int-ix-s2-def-2 .statement}

*A function f defined on T, with values in $ \overline{\mathbf{R}} $ or in a Banach space, is said to be locally $ \mu $-integrable if f is $ \mu $-measurable and every point $ x \in T $ admits a neighborhood V such that $ \mu^\bullet(|f|\varphi_V) < +\infty $.*

This definition coincides with the one given in Ch. V, §5, No. 1, in case T is locally compact.

Let $ f $ be a locally $ \mu $-integrable positive function; the mapping $ K \mapsto f_K \cdot \mu_K $ is a premeasure (Ch. V, §7, No. 1, Cor. 2 of Th. 1), which will be denoted $ f \cdot \mu $.

#### Proposition 2 {#int-ix-s2-prop-2 .statement}

*If f is a positive locally $ \mu $-integrable function, then, for every function $ g \in \mathcal{F}_+(T) $, one has the relation*

$$
(f \cdot \mu)^\bullet(g) = \mu^\bullet(fg).
$$

Indeed, for every compact set K in T,

$$
(f \cdot \mu)_K^\bullet(g_K) = (f_K \cdot \mu_K)^\bullet(g_K) = \mu_K^\bullet(f_K g_K) = \mu_K^\bullet((fg)_K),
$$

on using the definition of $ f \cdot \mu $ and Prop. 3 of Ch. V, §5, No. 3. Prop. 2 follows from this on passing to the supremum over K.

Now let $ x \in T $ and let V be a neighborhood of x such that $ \mu^\bullet(f \varphi_V) < +\infty $ (Def. 2); then $ (f \cdot \mu)^\bullet(V) = \mu^\bullet(f \varphi_V) < +\infty $, therefore $ f \cdot \mu $ is a measure.

#### Definition 3 {#int-ix-s2-def-3 .statement}

*Let f be a locally $ \mu $-integrable positive function. The measure $ f \cdot \mu : K \mapsto f_K \cdot \mu_K $ is called the measure with density f with respect* to $ \mu $, or the product measure of $ \mu $ by the function $ f $. Every measure of the form $ f \cdot \mu $, where $ f $ is positive and locally $ \mu $-integrable, is called a measure with base $ \mu $.

#### Remark 1 {#int-ix-s2-n2-rem-1 .statement}

The definition of $ f \cdot \mu $ extends to the case that $ f $ is a complex locally integrable function; one then has $ |f \cdot \mu| = |f| \cdot \mu $, which implies at once that $ f \cdot \mu $ is a measure, not just a premeasure. We retain the expression 'measures with base $ \mu $' to designate the complex measures so defined.

#### Remark 2 {#int-ix-s2-n2-rem-2 .statement}

Similarly, if $ \theta $ is a complex measure, $ f $ is said to be locally $ \theta $-integrable if it is locally $ |\theta| $-integrable, and one defines the measure $ f \cdot \theta : K \mapsto f_K \cdot \theta_K $. One has $ |f \cdot \theta| = |f| \cdot |\theta| $ (Ch. V, §5, No. 2, Prop. 2). In this No., we shall leave aside everything concerning non-positive measures.

#### Proposition 3 {#int-ix-s2-prop-3 .statement}

— Let $ \nu $ be a measure on T. For $ \nu $ to be of the form $ f \cdot \mu $, where $ f $ is a locally $ \mu $-integrable positive function, it is necessary and sufficient that every $ \mu $-negligible compact set be $ \nu $-negligible. If $ f' $ is a second locally $ \mu $-integrable function such that $ \nu = f' \cdot \mu $, then $ f = f' $ locally $ \mu $-almost everywhere.

The condition is obviously necessary (Prop. 2). Conversely, suppose that every $ \mu $-negligible compact set is $ \nu $-negligible. Let us introduce a crushing $ (K_\alpha)_{\alpha \in A} $ of T for the measure $ \mu + \nu $ and let us set $ N = T - \bigcup_{\alpha \in A} K_\alpha $. It is clear that $ (K_\alpha)_{\alpha \in A} $ is a crushing for $ \mu $ and for $ \nu $, and Prop. 9 of §1, No. 8 therefore implies the following relations for every $ g \in \mathcal{F}_+ $:

$$
\mu^\bullet(g) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(g_{K_\alpha}), \quad \nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}).
$$

Consider a compact set $ C \subset K_\alpha $ that is $ \mu_{K_\alpha} $-negligible; then $ C $ is locally $ \mu $-negligible, hence locally $ \nu $-negligible, and finally $ \nu_{K_\alpha} $-negligible by the definition of $ \nu $. It then follows from the Lebesgue–Nikodym theorem (Ch. V, §5, No. 5, Th. 2) that $ \nu_{K_\alpha} $ admits a density $ f_\alpha $ with respect to $ \mu_{K_\alpha} $. Let $ f $ be the function that coincides with $ f_\alpha $ on each of the sets $ K_\alpha $, and with 0 on $ N $; the function $ f $ is $ \mu $-measurable (Ch. IV, §5, No. 10, Prop. 16), and for every function $ g \in \mathcal{F}_+ $ one has, by the above relations and Prop. 3 of Ch. V, §5, No. 3,

$$
\nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_\alpha g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet((f g)_{K_\alpha}) = \mu^\bullet(f g).
$$

It then follows first of all that $ f $ is locally $ \mu $-integrable: if $ x $ is a point of T, and if $ V $ is a neighborhood of $ x $ such that $ \nu^\bullet(V) < +\infty $, then $ \mu^\bullet(f \varphi_V) < +\infty $. Next, Prop. 2 shows that the measures $ \nu $ and $ f \cdot \mu $ have the same essential upper integral. They are therefore equal (§1, No. 2, Cor. of Prop. 2). The uniqueness of $ f $ being obvious based on the case of compact spaces, the proposition is established.

Remark 3). — The theory of integration with respect to a measure $ \nu = f \cdot \mu $ reduces at once to the theory treated in Ch. V. For, let $ (K_\alpha)_{\alpha \in A} $ be a crushing of T for $ \mu $, hence for $ \nu $, and let $ T' $ be the locally compact space defined in the Scholium of §1, No. 8; we can associate to $ \mu $ (resp. to $ \nu $) a measure $ \mu' $ (resp. $ \nu' $) on $ T' $, in such a way that the measurable functions, the essentially integrable functions with values in a Banach space, and the essential upper integrals of positive functions, are the same for $ \mu $ and $ \mu' $ (resp. for $ \nu $ and $ \nu' $). The function $ f $ is therefore $ \mu' $-measurable; it is locally $ \mu' $-integrable, because $ T' $ is locally compact, and a compact subset of $ T' $ intersects only a finite number of the compact sets $ K_\alpha $ ($ \alpha \in A $). Finally, the relation $ \nu'^\bullet(g) = \nu^\bullet(g) = \mu^\bullet(fg) = \mu'^\bullet(fg) $ proves that $ \nu' = f \cdot \mu' $ (Ch. V, §5, No. 3, Prop. 3). We leave to the reader the task of transcribing the results of Ch. V, §5.

### 3. Image of a measure

#### Definition 4 {#int-ix-s2-def-4 .statement}

Let $ \pi $ be a mapping of T into a topological space X. One says that $ \pi $ is $ \mu $-proper if $ \pi $ is $ \mu $-measurable, and if every point x of X admits a neighborhood V such that $ \mu^\bullet(\overline{\pi}(V)) < +\infty $.

#### Remark 1 {#int-ix-s2-n3-rem-1 .statement}

When T and X are locally compact, this definition is equivalent to that of Ch. V, §6, No. 1.
2) A proper continuous mapping (GT, I, §10, No. 1, Def. 1) of T into X is $ \mu $-proper for every measure $ \mu $. For, let $ x \in X $; since $ \overline{\pi}(x) $ is compact (loc. cit., No. 2, Th. 1), the set $ \overline{\pi}(x) $ has an open neighborhood H such that $ \mu^\bullet(H) < +\infty $. Set $ V = X - \pi(T - H) $; since $ \pi $ is closed, V is open in X, contains x, and satisfies $ \overline{\pi}(V) \subset H $, whence $ \mu^\bullet(\overline{\pi}(V)) \leq \mu^\bullet(H) < +\infty $.
3) If $ \mu $ is bounded, every $ \mu $-measurable mapping of T into X is $ \mu $-proper.
4) If $ \theta $ is a complex measure on T, $ \pi $ is said to be $ \theta $-proper if $ \pi $ is proper for the positive measure $ |\theta| $.

#### Proposition 4 {#int-ix-s2-prop-4 .statement}

Let $ \pi $ be a $ \mu $-proper mapping of T into a topological space X. There exists one and only one measure $ \nu $ on X such that $ \nu^\bullet $ is equal to the image encumbrance $ \pi(\mu^\bullet) $ (§1, No. 1), in other words, such that $ \nu^\bullet(g) = \mu^\bullet(g \circ \pi) $ for all $ g \in \mathcal{F}_+(X) $.

Uniqueness is obvious (§1, No. 2, Cor. of Prop. 2). To establish existence, we shall first treat the case that $ \mu $ is carried by a compact set K, such that the restriction of $ \pi $ to K is continuous. Then $ L = \pi(K) $ is compact; let $ \pi' $ be the continuous mapping of K into L induced by $ \pi $, and let $ \nu' $ be the image measure $ \pi'(\mu_K) $ on L, $ \nu $ the measure on X defined by $ \nu' $ (§1, No. 3, Example 2). For every $ g \in \mathcal{F}_+(X) $,

$$
\nu^\bullet(g) = \nu'^\bullet(g_L) = \mu_K^\bullet(g_L \circ \pi') = \mu_K^\bullet((g \circ \pi)_K) = \mu^\bullet((g \circ \pi)_K^0) = \mu^\bullet(g \circ \pi)
$$

(we have used successively formula (3) of §1, No. 3; Prop. 2 of Ch. V, §6, No. 2; the definition of $ \mu_K^\bullet $; and the fact that $ \mu $ is carried by K). In other words, $ \nu^\bullet = \pi(\mu^\bullet) $.

Let us now pass to the general case; by Props. 10 and 9 of §1, No. 8, $ \mu $ is the sum of a summable family $ (\mu_\alpha)_{\alpha \in A} $ of measures with compact support, such that the restriction of $ \pi $ to the support $ K_\alpha $ of $ \mu_\alpha $ is continuous for every $ \alpha \in A $. The special case treated above permits associating to each measure $ \mu_\alpha $ on T a measure $ \nu_\alpha $ on X such that $ \nu_\alpha^\bullet = \pi(\mu_\alpha^\bullet) $. Then, for $ g \in \mathcal{F}_+(X) $,

$$
\sum_{\alpha \in A} \nu_\alpha^\bullet(g) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi).
$$

The encumbrance $ \pi(\mu^\bullet) $ is locally bounded, since $ \pi $ is $ \mu $-proper; the family $ (\nu_\alpha)_{\alpha \in A} $ is therefore summable (§1, No. 7, Prop. 7), and its sum $ \nu $ satisfies the statement.

#### Definition 5 {#int-ix-s2-def-5 .statement}

*If $ \pi $ is a $ \mu $-proper mapping of T into a topological space X, the unique measure $ \nu $ on X such that $ \nu^\bullet(g) = \mu^\bullet(g \circ \pi) $ for all $ g \in \mathcal{F}_+(X) $ is called the image measure of $ \mu $ under $ \pi $, and is denoted $ \pi(\mu) $.*.

#### Example {#int-ix-s2-n3-exa-1 .statement}

— Let K be a compact subspace of T, i the canonical injection of K into T, and $ \lambda $ a measure on K; since i is continuous and $ \lambda $ is bounded, i is $ \lambda $-proper. Formula (3) of §1, No. 3 shows that the "measure on T defined by $ \lambda $" is the image measure $ i(\lambda) $.

*Remark 5).* — If $ \theta $ is a real measure and $ \pi $ is $ \theta $-proper, then $ \pi $ is proper for the measures $ \theta^+ $ and $ \theta^- $; one then sets $ \pi(\theta) = \pi(\theta^+) - \pi(\theta^-) $. If $ \theta $ is a complex measure and $ \pi $ is $ \theta $-proper, then $ \pi $ is proper for the real measures $ \Re(\theta) $ and $ \Im(\theta) $; one then sets

$$
\pi(\theta) = \pi(\Re(\theta)) + i \pi(\Im(\theta)).
$$

#### Proposition 5 {#int-ix-s2-prop-5 .statement}

*Let $ \pi $ be a $ \mu $-proper mapping of T into a topological space X, and let f be a mapping of X into a topological space F (Hausdorff or not). For f to be $ \pi(\mu) $-measurable, it is necessary and sufficient that $ f \circ \pi $ be $ \mu $-measurable.*

Let us take up again the proof of Prop. 4, and commence with the special case treated at the beginning, with the same notations; g is measurable for the measure $ \pi(\mu) = \nu $ if and only if $ g_L $ is $ \nu' $-measurable (§1, No. 5, *Example*); now, this is equivalent to saying that $ g_L \circ \pi' = (g \circ \pi)_K $ is $ \mu_K $-measurable (Ch. V, §6, No. 2, Prop. 3), and finally that $ g \circ \pi $ is $ \mu $-measurable (§1, No. 5, *Example*). Let us now pass to the general case, with the same notations as in the proof of Prop. 4; f is $ \nu $-measurable if and only if f is $ \nu_\alpha $-measurable for every $ \alpha \in A $ (§1, No. 7, Prop. 8), hence if and only if $ f \circ \pi $ is $ \mu_\alpha $-measurable for every $ \alpha \in A $ (the preceding special case) and finally if and only if $ f \circ \pi $ is $ \mu $-measurable ($ \S 1 $, No. 7, Prop. 8).

#### Corollary {#int-ix-s2-n3-cor-1 .statement}

— *Let X and Y be two topological spaces, $ \pi $ a $ \mu $-proper mapping of T into X, and $ \pi' $ a $ \pi(\mu) $-proper mapping of X into Y. The mapping $ \pi'' = \pi' \circ \pi $ is then $ \mu $-proper, and $ \pi''(\mu) = \pi'(\pi(\mu)) $ ('transitivity of images of measures').

For, $ \pi'' $ is $ \mu $-measurable (Prop. 5). Set $ \mu' = \pi(\mu) $; the image encumbrance $ \pi'(\mu'^\bullet) = \pi'(\pi(\mu^\bullet)) $ is obviously equal to $ \pi''(\mu^\bullet) $. Since it is locally bounded, $ \pi'' $ is $ \mu $-proper. The measures $ \pi''(\mu) $ and $ \pi'(\mu') $ then have the same essential upper integral, hence are equal.

#### Proposition 6 {#int-ix-s2-prop-6 .statement}

— *Let $ \pi $ be a $ \mu $-proper mapping of T into a topological space X, and let B be a $ \pi(\mu) $-measurable subset of X. Set $ A = \overline{\pi^{-1}(B)} $, and denote by $ \pi' $ the mapping of A into B that coincides with $ \pi $ on A. The set A is then $ \mu $-measurable, $ \pi_A $ and $ \pi' $ are $ \mu_A $-proper, and*

$$
(\pi(\mu))_B = (\pi_A(\mu_A))_B = \pi'(\mu_A).
$$

The set A is $ \mu $-measurable by Prop. 5 applied to $ \varphi_B $; the mapping $ \pi_A $ is clearly $ \mu_A $-measurable by the definition of induced measures (No. 1), and it follows that $ \pi' $ is measurable. Let $ f $ be an element of $ \mathscr{F}_+(B) $; denoting by zero exponents the extensions by 0 in X and in T, we have

$$
(\pi(\mu)_B)^\bullet(f) = \pi(\mu)^\bullet(f^0) = \mu^\bullet(f^0 \circ \pi) = \mu^\bullet((f \circ \pi')^0) = \mu_A^\bullet(f \circ \pi'),
$$

whence $ (\pi(\mu)_B)^\bullet = \pi'(\mu_A^\bullet) $. Since the encumbrance $ (\pi(\mu)_B)^\bullet $ is locally bounded, the same is true of $ \pi'(\mu_A^\bullet) $ and therefore $ \pi' $ is $ \mu_A $-proper. The measures $ \pi'(\mu_A) $ and $ (\pi(\mu))_B $ have the same essential upper integral, hence are equal. The other relation may be established in an analogous manner.

#### Proposition 7 {#int-ix-s2-prop-7 .statement}

— *Let T be a subspace of a topological space X, and let i be the injection of T into X.

a) *If $ \mu $ is a measure on T, and if i is $ \mu $-proper, then the measure $ i(\mu) $ is concentrated on T, and one has $ (i(\mu))_T = \mu $.

b) *If $ \lambda $ is a measure on X such that T is $ \lambda $-measurable, then i is $ \lambda_T $-proper, and $ i(\lambda_T) = \varphi_T \cdot \lambda $.

a) Set $ \nu = i(\mu) $; the relation $ \nu^\bullet(A) = \mu^\bullet(A \cap T) $, applied to $ A = X - T $, shows that $ \nu $ is concentrated on T. The relation $ \nu_T = \mu $ is a special case of the relation (2), on taking $ B = T = A $.

b) Let $ f $ be a positive function defined on X; setting $ \mu = \lambda_T $, one has $ \mu^\bullet(f \circ i) = \lambda_T^\bullet(f_T) = \lambda^\bullet(f \varphi_T) \leq \lambda^\bullet(f) $ (Prop. 1); it follows that i is $ \mu $-proper. On the other hand, $ \mu^\bullet(f \circ i) $ (resp. $ \lambda^\bullet(f \varphi_T) $) is the essential upper integral of $ f $ with respect to $ i(\mu) $ (resp. $ \varphi_T \cdot \lambda $). These two measures are therefore equal.

*Remark 6).* — Let $ \pi $ be a $ \mu $-proper mapping of $ T $ into a topological space $ X $. One reduces the theory of integration with respect to the image measure $ \nu = \pi(\mu) $ to the theory treated in Ch. V, §6, in the following way. Let $ (K_\alpha)_{\alpha \in A} $ (resp. $ (L_\beta)_{\beta \in B} $) be a crushing of $ T $ (resp. of $ X $) for $ \mu $ (resp. for $ \nu $), and set $ N = T - \bigcup_{\alpha \in A} K_\alpha,\ P = X - \bigcup_{\beta \in B} L_\beta $. We can suppose that the restriction of $ \pi $ to each $ K_\alpha $ is continuous (§1, No. 8, Prop. 10). Let $ T', X' $ be the locally compact spaces constructed as in the Scholium of §1, No. 8 and let $ \mu' $ and $ \nu' $ be the measures on these spaces associated with $ \mu $ and $ \nu $. The topology of $ T' $ being the sum of the topologies of the subspaces $ K_\alpha $ and the discrete topology on $ N $, $ \pi $ is a continuous mapping of $ T' $ into $ X $ and the relation $ \mu'^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g) $ (for $ g \in \mathcal{F}_+(X) $) shows that $ \pi $ is $ \mu' $-proper and that $ \pi(\mu') = \nu $. On the other hand, the identity mapping $ i $ of $ X $ onto $ X' $ is $ \nu $-proper, and $ i(\nu) = \nu' $. It follows that $ \pi $ is a $ \mu' $-proper mapping of $ T' $ into $ X' $, and that the image of $ \mu' $ under $ \pi $ is $ \nu' $ (Cor. of Prop. 5). We leave to the reader the task of transcribing the results of Ch. V, §6.

### 4. Lifting of measures

#### Proposition 8 {#int-ix-s2-prop-8 .statement}

*Let $ T $ and $ X $ be two topological spaces, $ \pi $ a mapping of $ T $ into $ X $.

a) Let $ \nu $ be a bounded measure on $ X $. In order that there exist a measure $ \mu $ on $ T $ such that $ \pi $ is $ \mu $-proper and $ \pi(\mu) = \nu $, it is necessary and sufficient that there exist, for every number $ \varepsilon > 0 $, a compact set $ K_\varepsilon \subset T $ such that the restriction of $ \pi $ to $ K_\varepsilon $ is continuous and $ \nu^\bullet(X - \pi(K_\varepsilon)) < \varepsilon $.

b) Suppose that $ \pi $ is injective; let $ \mu $ and $ \mu' $ be two measures on $ T $, such that $ \pi $ is proper for $ \mu $ and $ \mu' $, and such that $ \pi(\mu) = \pi(\mu') $. Then $ \mu = \mu' $.

The condition stated in *a)* is necessary. For, if $ \pi $ is $ \mu $-proper and $ \pi(\mu) = \nu $, the relation $ \mu^\bullet(1) = \nu^\bullet(1) < +\infty $ implies that $ \mu $ is bounded. Prop. 2 of §1, No. 2, applied to the function 1, implies the existence of a compact subset $ K $ of $ T $ such that $ \mu^\bullet(T - K) < \varepsilon/2 $. Since $ \pi $ is $ \mu $-measurable, there exists a compact set $ K_\varepsilon \subset K $ such that the restriction of $ \pi $ to $ K_\varepsilon $ is continuous, and such that $ \mu^\bullet(K - K_\varepsilon) < \varepsilon/2 $. Then (No. 3, Prop. 4)

$$
\nu^\bullet(X - \pi(K_\varepsilon)) = \mu^\bullet(T - \overline{\pi}^{-1}(\pi(K_\varepsilon))) < \varepsilon.
$$

To show that the condition is sufficient, we first treat a special case.

#### Lemma 1 {#int-ix-s2-lem-1 .statement}

Let U and V be two compact spaces, h a continuous mapping of U onto V. The mapping $ \lambda \mapsto h(\lambda) $ of $ \mathcal{M}_+(U) $ into $ \mathcal{M}_+(V) $ is then surjective.

For, let a be the linear mapping $ f \mapsto f \circ h $ of $ \mathcal{C}(V) $ into $ \mathcal{C}(U) $; since h is surjective, a is an isometry of $ \mathcal{C}(V) $ onto a subspace H of $ \mathcal{C}(U) $. Let $ \theta $ be a positive measure on V; then $ \theta \circ a^{-1} $ is a continuous linear form on H, which is extendible to a linear form $ \eta $ on $ \mathcal{C}(U) $ with the same norm, by virtue of the Hahn–Banach theorem (TVS, II, §3, No. 2, Cor. 3 of Th. 1); $ \eta $ is then a measure on U, and $ \theta(f) = \eta(f \circ h) $ for all $ f \in \mathcal{C}(V) $, so that $ \theta = h(\eta) $. Finally, $ \theta(1) = \| \theta \| = \| \eta \| $, and $ \theta(1) = \eta(1) $, so that $ \eta $ is positive (Ch. V, §5, No. 5, Prop. 9).

Let us now prove the sufficiency of the condition stated in a). The condition implies the existence of a sequence $ (K_n)_{n \geq 1} $ of compact subsets of T, such that the restriction of $ \pi $ to each $ K_n $ is continuous, and such that, for every $ n $, $ \nu^\bullet(X - \pi(K_n)) < 1/n $. The sequence $ (K_n) $ can be assumed to be increasing. Set $ L_n = \pi(K_n) $ and denote by $ \nu'_n $ the measure $ \varphi_{L_n - L_{n-1}} \cdot \nu_{L_n} $ on $ L_n $, with the convention $ L_0 = \varnothing $.

The restriction $ \pi_{K_n} $ being continuous, there exists a measure $ \mu'_n $ on $ K_n $ such that $ \pi_{K_n}(\mu'_n) = \nu'_n $ (Lemma 1). Let $ \mu_n $ be the image of $ \mu'_n $ under the canonical injection of $ K_n $ into T, and let g be an element of $ \mathcal{F}_+(X) $. Using successively the fact that $ \nu $ is concentrated on $ \bigcup L_n $, Prop. 4 of §1, No. 5; Prop. 2 of §1, No. 2; Prop. 4 of No. 3, and finally Prop. 7 of No. 3, we have

$$
\nu^\bullet(g) = \sum_n \nu^\bullet(\varphi_{L_n - L_{n-1}} g) = \sum_n \nu'_n \bullet (g_{L_n}) = \sum_n \mu'_n \bullet (g_{L_n} \circ \pi_{K_n})
$$
$$
= \sum_n \mu'_n \bullet ((g \circ \pi)_{K_n}) = \sum_n \mu_n^\bullet (g \circ \pi).
$$

Taking $ g = 1 $ in this formula, one sees that the family $ (\mu_n) $ is summable and that its sum is a bounded measure $ \mu $ (§1, No. 7, Prop. 7). By Prop. 5 of No. 3, the mapping $ \pi $ is $ \mu_n $-measurable for all $ n $, because $ \pi_{K_n} $ is continuous, hence $ \mu'_n $-measurable; it follows that $ \pi $ is $ \mu $-measurable (§1, No. 7, Prop. 8), hence $ \mu $-proper since $ \mu $ is bounded. The above relations then prove that the measures $ \pi(\mu) $ and $ \nu $ have the same essential upper integral, hence are equal (§1, No. 2, Cor. of Prop. 2).

Finally, let us assume that $ \pi $ is injective, and let us prove b). Let f be an element of $ \mathcal{F}_+(T) $; since $ \pi $ is injective, there exists a function $ g \in \mathcal{F}_+(X) $ such that $ f = g \circ \pi $ and, setting $ \nu = \pi(\mu) = \pi(\mu') $, by Prop. 4 of No. 3 we have

$$
\mu^\bullet(f) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g) = \mu'^\bullet(g \circ \pi) = \mu'^\bullet(f).
$$

The two measures $ \mu $ and $ \mu' $ thus have the same essential upper integral, which implies their equality (\$1, No. 2, Cor. of Prop. 2).

#### Remark {#int-ix-s2-n4-rem-1 .statement}

Suppose that $ \pi $ is injective. Let $ \theta $ be a complex measure such that $ \pi $ is $ \theta $-proper and $ \pi(\theta) = 0 $; then $ \theta = 0 $. Indeed, by separating $ \theta $ into its real and imaginary parts, one can reduce to the case that $ \theta $ is real. We then have $ \pi(\theta^+) = \pi(\theta^-) $, therefore $ \theta^+ = \theta^- $ (Prop. 8), and finally $ \theta = 0 $.

Here is an important case where condition $ a) $ of Prop. 8 is always satisfied.

#### Proposition 9 {#int-ix-s2-prop-9 .statement}

— *Let T be a Souslin space* (GT, IX, §6, No. 2, Def. 2), *X a Hausdorff space*, $ \pi $ *a continuous mapping of T onto X*, and $ \nu $ *a bounded measure on X*. *Then there exists a bounded measure $ \mu $ on T such that $ \pi(\mu) = \nu $*.

The hypotheses obviously imply that X is a Souslin space.

Let us consider the set function $ c : A \mapsto \nu^\bullet(\pi(A)) $ on $ \mathfrak{P}(T) $. The relation $ A \subset B $ implies $ c(A) \leq c(B) $; if $ (A_n) $ is an increasing sequence of subsets of T, and if $ A = \bigcup_{n \in \mathbf{N}} A_n $, then $ c(A) = \sup_n c(A_n) $ from the fact that $ \nu^\bullet $ is an encumbrance. Finally, let $ A \subset T $ and let $ \varepsilon $ be a number $ > 0 $; choose an open subset G of X containing $ \pi(A) $, such that $ \nu^\bullet(G) \leq \nu^\bullet(\pi(A)) + \varepsilon $ (\$1, No. 9, Prop. 13); the open subset $ H = \overline{\pi^{-1}(G)} $ of T contains A, and $ c(H) \leq c(A) + \varepsilon $. The function c is therefore a right-continuous capacity on T (TG, IX, §6, No. 10, Def. 9)(1) and the theorem on capacitability (*loc. cit.*, Th. 6) implies the equality $ c(T) = \sup_K c(K) $, where K runs over the set of compact subsets of T. Prop. 8 then implies the existence of the desired measure $ \mu $.

### 5. Product of two measures

Let S and T be two topological spaces, equipped respectively with two (positive) premeasures $ \lambda $ and $ \mu $, and let X be the product space $ S \times T $. Let K be a compact subset of X; let us denote by A and B the projections of K on S and T respectively, and set

$$
\nu_K = (\lambda_A \otimes \mu_B)_K .
$$

We thus define a premeasure on X. For, let L be a compact subset of X containing K, and let C and D be its two projections; then $ A \subset C $, $ B \subset D $,

(1) A capacity $ f $ on T is said to be right-continuous if, for every compact set K in T, $ f(K) = \inf_U f(U) $ as U runs over the open sets $ U \supset K $. This concept is not defined in GT, translated from an earlier edition of Ch. IX.

consequently, using the transitivity of induced measures, and Prop. 12 of Ch. V, §8, No. 5, we have

$$
(\nu_L)_K = ((\lambda_C \otimes \mu_D)_L)_K = (\lambda_C \otimes \mu_D)_K \\
= ((\lambda_C \otimes \mu_D)_{A \times B})_K = (\lambda_A \otimes \mu_B)_K = \nu_K .
$$

#### Definition 6 {#int-ix-s2-def-6 .statement}

*The premeasure $ \nu $ defined by (3) is called the product premeasure of $ \lambda $ and $ \mu $, and is denoted $ \lambda \otimes \mu $.*

This definition obviously extends to the case that $ \lambda $ and $ \mu $ are complex premeasures, and one then has $ |\lambda \otimes \mu| = |\lambda| \otimes |\mu| $ (Ch. III, §4, No. 2, Prop. 3 and Ch. IV, §5, No. 7, Lemma 3).

We conserve the notations of Ch. III, §4 and Ch. V, §8 relative to products of measures and to iterated integrals. In particular, if $ f $ and $ g $ are two functions defined respectively on $ S $ and $ T $, with values in $ \overline{\mathbf{R}}_+ $ or in $ \mathbf{C} $, the function $ (s, t) \mapsto f(s)g(t) $ on $ S \times T $ will be denoted $ f \otimes g $.

#### Proposition 10 {#int-ix-s2-prop-10 .statement}

*Let $ \nu $ be the product premeasure of $ \lambda $ and $ \mu $; for every function $ f \in \mathcal{F}_+(S) $ and every function $ g \in \mathcal{F}_+(T) $,*

$$
\nu^\bullet(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g) .
$$

*The premeasure $ \nu $ is the only premeasure on $ S \times T $ that satisfies (4).*

As $ K $ (resp. $ L $) runs over the set of compact subsets of $ S $ (resp. of $ T $), we have

$$
\begin{align*}
\nu^\bullet(f \otimes g) &= \sup_{K,L} \nu^\bullet_{K \times L}((f \otimes g)_{K \times L}) = \sup_{K,L} (\lambda_K \otimes \mu_L)^\bullet(f_K \otimes g_L) \\
&= \sup_{K,L} \lambda_K^\bullet(f_K) \cdot \mu_L^\bullet(g_L) = (\sup_K \lambda_K^\bullet(f_K)) (\sup_L \mu_L^\bullet(g_L)) \\
&= \lambda^\bullet(f)\mu^\bullet(g)
\end{align*}
$$

by Prop. 8 of Ch. V, §8, No. 3.

Let $ \eta $ be a second premeasure on $ S \times T $ satisfying (4), and let $ K $ and $ L $ be compact subsets of $ S $ and $ T $ respectively, $ f $ and $ g $ elements of $ \mathcal{F}_+(K) $ and $ \mathcal{F}_+(L) $ respectively. One has the relation $ (f \otimes g)^0 = f^0 \otimes g^0 $ between the extensions by 0, therefore (§1, No. 2, Prop. 2)

$$
\eta^\bullet_{K \times L}(f \otimes g) = \eta^\bullet((f \otimes g)^0) = \eta^\bullet(f^0 \otimes g^0) \\
= \lambda^\bullet(f^0)\mu^\bullet(g^0) = \lambda_K^\bullet(f)\mu_L^\bullet(g) .
$$

In particular, if one takes $ f \in \mathcal{K}_+(K) $, $ g \in \mathcal{K}_+(L) $, one sees that $ \eta_{K \times L} $ has the characteristic property of the product measure $ \lambda_K \otimes \mu_L $ (Ch. III, §4, No. 1, Th. 1). Therefore $ \eta_{K \times L} = \nu_{K \times L} $; since every compact subset of $ S \times T $ is contained in a set of the form $ K \times L $, the transitivity of induced measures implies that $ \eta = \nu $.

#### Corollary 1 {#int-ix-s2-prop-10-cor-1 .statement}

— *If $ \lambda $ and $ \mu $ are measures, then $ \nu $ is a measure.*

For, let $ x = (s, t) $ be a point of $ X $, and let $ U $ and $ V $ be neighborhoods of $ s, t $ respectively, such that $ \lambda^\bullet(U) < +\infty $, $ \mu^\bullet(V) < +\infty $; the set $ U \times V $ is a neighborhood of $ x $, and $ \nu^\bullet(U \times V) = \lambda^\bullet(U)\mu^\bullet(V) < +\infty $ by (4); the encumbrance $ \nu^\bullet $ is thus locally bounded, and the premeasure $ \nu $ is a measure.

This result extends at once to complex measures.

#### Corollary 2 {#int-ix-s2-prop-10-cor-2 .statement}

— *If $ A $ is a subset of $ S $ locally negligible for $ \lambda $, then $ A \times T $ is locally $ \nu $-negligible.*

#### Corollary 3 {#int-ix-s2-prop-10-cor-3 .statement}

— *Suppose that $ \lambda $ (resp. $ \mu $) is the sum of a summable family $ (\lambda_\alpha)_{\alpha \in A} $ (resp. $ (\mu_\beta)_{\beta \in B} $) of measures on $ S $ (resp. $ T $). The family $ (\lambda_\alpha \otimes \mu_\beta)_{(\alpha, \beta) \in A \times B} $ is then summable, and its sum is $ \lambda \otimes \mu $.*

For, let $ p $ be the encumbrance $ \sum_{\alpha, \beta} (\lambda_\alpha \otimes \mu_\beta)^\bullet $; if $ f \in \mathcal{F}_+(S) $ and $ g \in \mathcal{F}_+(T) $, then obviously $ p(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g) $. The proof of Cor. 1 then shows that $ p $ is locally bounded, so that the family $ (\lambda_\alpha \otimes \mu_\beta) $ is summable (\S 1, No. 7, Prop. 7). Its sum $ \eta $ then satisfies $ \eta^\bullet = p $ (\S 1, No. 7, Prop. 7), and Prop. 10 implies $ \eta = \nu $.

### 6. Integration with respect to the product of two measures

*Throughout this No., $ \lambda $ and $ \mu $ denote measures on $ S $ and $ T $, respectively, and $ \nu $ denotes the product measure $ \lambda \otimes \mu $ on $ S \times T $. In addition, if $ f $ is a positive function on $ S \times T $, for every $ s \in S $ we denote by $ f_s $ the function $ t \mapsto f(s, t) $ on $ T $, and by $ I_f $ the function $ s \mapsto \mu^\bullet(f_s) $ on $ S $.*

#### Lemma 2 {#int-ix-s2-lem-2 .statement}

*Let $ f $ be a $ \nu $-measurable positive function on $ S \times T $; for every compact subset $ L $ of $ T $, let $ I_f^L $ be the function $ s \mapsto \mu^\bullet(f_s \varphi_L) $ on $ S $. Then the function $ I_f^L $ is $ \lambda $-measurable, and*

$$
(5) \quad I_f = \sup_L I_f^L
$$
$$
(6) \quad \nu^\bullet(f) = \sup_L \lambda^\bullet(I_f^L),
$$

*where $ L $ runs over the set of compact subsets of $ T $.*

We first note that the inclusion $ L \subset L' $ implies $ I_f^L \leq I_f^{L'} $; on the other hand, $ I_f^L(s) = \mu_L^\bullet((f_s)_L) $ for all $ s \in S $. Formula (5) is therefore an immediate consequence of the definition of the encumbrance $ \mu^\bullet $ given in

§1, No. 2. If K is a compact subset of S, and L a compact subset of T, then $ \nu_{K \times L} = \lambda_K \otimes \mu_L $ by construction, and Prop. 7 of Ch. V, §8, No. 3 implies the relation

$$
\nu^\bullet(f \varphi_{K \times L}) = \lambda_K^\bullet((I_f^L)_K).
$$

Moreover, every compact subset of $ S \times T $ is contained in a compact set of the form $ K \times L $; passing to the upper envelope over all K and L in the preceding formula, we therefore obtain

$$
\nu^\bullet(f) = \sup_L \sup_K \lambda_K^\bullet((I_f^L)_K) = \sup_L \lambda^\bullet(I_f^L),
$$

namely (6).

Finally, Prop. 7 of Ch. V, §8, No. 3 implies that the restriction of $ I_f^L $ to every compact subset K of S is $ \lambda_K $-measurable; this is equivalent to saying that $ I_f^L $ is $ \lambda $-measurable.

#### Proposition 11 {#int-ix-s2-prop-11 .statement}

*Let f be a lower semi-continuous function $ \geqslant 0 $ defined on $ X = S \times T $.*

a) *The function $ f_s : t \mapsto f(s, t) $ is lower semi-continuous on T for every $ s \in S $.*

b) *The function $ I_f : s \mapsto \int^\bullet f(s, t) d\mu(t) $ is lower semi-continuous on S, and*

$$
\iint_X^\bullet f(s, t) d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) d\mu(t).
$$

The property *a)* is obvious, since the mapping $ t \mapsto f(s, t) $ of T into $ \overline{\mathbf{R}} $ is the composition of $ f $ with the continuous mapping $ t \mapsto (s, t) $ of T into X. To establish *b)*, we will make use of a lemma:

#### Lemma 3 {#int-ix-s2-lem-3 .statement}

— *Let X be a topological space (Hausdorff or not), f a lower semi-continuous function $ \geqslant 0 $ defined on X; then f is the limit of an increasing sequence $ (f_n)_{n \in \mathbf{N}} $ of lower semi-continuous functions on X, such that each function $ f_n $ is a linear combination, with positive coefficients, of characteristic functions of open sets.*

Given two integers $ k \geqslant 1 $ and $ n \geqslant 1 $, let us denote by $ J_{kn} $ the characteristic function of the interval $ ]k/2^n, +\infty] $ of $ \overline{\mathbf{R}} $. For every $ x \in \overline{\mathbf{R}}_+ $, set

$$
u_n(x) = 2^{-n} \sum_{k=1}^{n \cdot 2^n} J_{kn}(x);
$$

it is immediate that the sequence $ (u_n(x))_{n \geqslant 1} $ is increasing and admits x as limit. The sequence of functions $ f_n = u_n \circ f $ is therefore increasing and converges to $ f $, and one has $ f_n = 2^{-n} \sum_{k=1}^{n \cdot 2^n} \varphi_{U(k,n)} $,
where $ U(k,n) $ is the open set $ f^{-1}([k/2^n, +\infty]) $ of $ X $.

Let us pass to the proof of $ b) $. The function $ I_f $ being the upper envelope of the increasing directed family of functions $ I_f^L $, where $ L $ runs over the set of compact subsets of $ T $ (Lemma 2), it will suffice to show that the functions $ I_f^L $ are lower semi-continuous; the formula (9) may then be deduced from (6) by passing to the upper envelope over $ L $ (\$1, No. 6, Prop. 5).

Thus let $ \mathcal{H} $ be the set of positive lower semi-continuous functions $ f $ on $ S \times T $ such that $ I_f^L $ is lower semi-continuous for every compact subset $ L $ of $ T $. By Prop. 5 of \$1, No. 6, the supremum of every increasing directed set of elements of $ \mathcal{H} $ belongs to $ \mathcal{H} $. By Lemma 3, it will therefore suffice to prove that the characteristic function of an open set $ W $ of $ S \times T $ belongs to $ \mathcal{H} $. Moreover, by the definition of the product topology on $ S \times T $, the open set $ W $ is the union of an increasing directed family $ (W_\alpha)_{\alpha \in A} $ of open sets of the form
$$
W = \bigcup_{1 \leq i \leq n} (U_i \times V_i),
$$
where the $ U_i $ are open in $ S $ and the $ V_i $ are open in $ T $; by the remarks made above, it will suffice to show that the characteristic function of such an open set belongs to $ \mathcal{H} $. Let then $ s \in S $, and let $ U $ be the intersection of the family (possibly empty) formed by the open sets $ U_i $ containing $ s $; one sees immediately that $ \varphi_W(s,t) \leq \varphi_W(s',t) $ for all $ s' \in U $ and $ t \in T $, whence, by integration, $ I_{\varphi_W}^L(s) \leq I_{\varphi_W}^L(s') $ for all $ s' \in U $. Consequently $ I_{\varphi_W}^L $ is lower semi-continuous, and the proposition is established.

#### Corollary 1 {#int-ix-s2-lem-3-cor-1 .statement}

*Let $ f $ be a positive numerical function defined on $ X = S \times T $; then*
$$
\iint_X^* f(s,t)\, d\nu(s,t) \geq \int_S^* d\lambda(s) \int_T^* f(s,t)\, d\mu(t).
$$

For, let $ g $ be a lower semi-continuous function on $ X $ such that $ g \geq f $; by Prop. 11,
$$
\iint_X^* g(s,t)\, d\nu(s,t) = \iint^* g(s,t)\, d\nu(s,t) = \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t)
$$
$$
= \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t) \geq \int^* d\lambda(s) \int^* f(s,t)\, d\mu(t).
$$
The inequality (10) is obtained by passing to the lower envelope over $ g $.

#### Corollary 2 {#int-ix-s2-lem-3-cor-2 .statement}

— Let $ f $ be a numerical function defined on $ S \times T $ and $ \nu $-negligible. Then the function $ f_s : t \mapsto f(s, t) $ is $ \mu $-negligible for $ \lambda $-almost every $ s \in S $.

#### Proposition 12 {#int-ix-s2-prop-12 .statement}

— Let $ f $ be a $ \nu $-measurable positive function defined on $ X = S \times T $. Assume that $ f $ is $ \nu $-moderated (resp. that $ \mu $ is moderated). Then:
a) The set $ N $ of $ s \in S $ such that the function $ f_s : t \mapsto f(s, t) $ is not $ \mu $-measurable is negligible (resp. locally negligible) for $ \lambda $.
b) The mapping $ s \mapsto \int^\bullet f(s, t) \, d\mu(t) $ is $ \lambda $-measurable, and

$$
\iint_X^\bullet f(s, t) \, d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) \, d\mu(t).
$$

We begin by establishing b) when $ f $ is $ \nu $-moderated. By Lemma 2, this part of the statement is valid when there exists a compact subset $ L $ of $ T $ such that $ f $ is zero outside $ S \times L $; for, in this case $ I_f = I_f^{L'} $ for every compact subset $ L' $ of $ T $ containing $ L $, and formula (11) reduces to (6). In particular, b) is established for a function $ f $ that is zero outside a compact subset of $ S \times T $. On the other hand, Cor. 1 of Prop. 11 implies that b) is true when $ f $ is $ \nu $-negligible. Since every $ \nu $-moderated function is the sum of a $ \nu $-negligible function and a sequence of functions with compact support (\S 1, No. 9, Cor. 3 of Prop. 14), the assertion b) is true when $ f $ is $ \nu $-moderated.

Similarly, the assertion b) is obvious when $ \mu $ is carried by a compact subset $ L $ of $ T $ (Lemma 2). Suppose that $ \mu $ is moderated; then there exists a sequence $ (\mu_n)_{n \in \mathbf{N}} $ of measures on $ T $ with compact support, such that $ \mu = \sum_n \mu_n $ (\S 1, No. 9, Cor. 5 of Prop. 14), whence $ \nu = \sum_n \lambda \otimes \mu_n $ (No. 5, Cor. 3 of Prop. 10). The assertion b), being valid for each of the measures $ \nu_n = \lambda \otimes \mu_n $, is also valid for $ \nu = \sum_n \nu_n $.

Let us prove a); denote by $ N $ the set of $ s \in S $ such that $ f_s $ is not $ \mu $-measurable; for every compact subset $ L $ of $ T $, similarly denote by $ N_L $ the set of $ s \in S $ such that $ f_s \varphi_L $ is not $ \mu $-measurable. If $ K $ and $ L $ are compact sets in $ S $ and $ T $ respectively, then $ f_{K \times L} $ is measurable with respect to the measure $ \nu_{K \times L} = \lambda_K \otimes \mu_L $, and Prop. 2 of Ch. V, \S 8, No. 2 shows that the set $ N_L $ is locally negligible for $ \lambda_K $; since $ K $ is arbitrary, $ N_L $ is locally $ \lambda $-negligible.

Suppose that $ f $ is zero outside a compact set of the form $ K \times L $; then $ N = N_L $, and $ N $ is contained in $ K $; it follows that $ N $ is $ \lambda $-negligible. Similarly, if $ f $ is $ \nu $-negligible, Cor. 2 of Prop. 11 implies that $ N $ is $ \lambda $-negligible. The case that $ f $ is $ \nu $-moderated can then be treated as above, on combining the preceding two cases.

Suppose that $ \mu $ is carried by a compact subset $ L $ of $ T $; then $ N = N_L $ again, therefore $ N $ is locally $ \lambda $-negligible. Since every moderated measure is the sum of a sequence of measures with compact support ($ \S 1 $, No. 9, Cor. 5 of Prop. 14), this result extends at once to the case that $ \mu $ is moderated, on using Prop. 8 of $ \S 1 $, No. 7.

#### Remark {#int-ix-s2-n6-rem-1 .statement}

— Let $ (K_\alpha)_{\alpha \in A} $ be a crushing of $ S $ for $ \lambda $ and let $ M = S - \bigcup_{\alpha \in A} K_\alpha $; define in an analogous way $ (L_\beta)_{\beta \in B} $ and $ N $ for the measure $ \mu $ on $ T $. We denote by $ S' $ the locally compact space that is the sum of the subspaces $ K_\alpha $ of $ S $ and the *discrete* space $ M $; the space $ T' $ is defined analogously, and we set $ X' = S' \times T' $. The locally compact space $ X' $ is the sum of the family $ (K_\alpha \times L_\beta)_{(\alpha, \beta) \in A \times B} $ of compact subspaces of $ X $ and the subspace $ P = (M \times T) \cup (S \times N) $ that is a locally $ \nu $-negligible subset of $ X $ (one observes that $ P $ is in general not a discrete space). We saw in the *Scholium* of $ \S 1 $, No. 8 that there exists a measure $ \lambda' $ on $ S' $ such that the measurable functions, the essential upper integral of positive functions, the essentially integrable functions and their integrals, are the same for $ \lambda $ and $ \lambda' $. We associate the measure $ \mu' $ on $ T' $ with $ \mu $, and the measure $ \nu' $ on $ X' $ with $ \nu $, in conformity with the cited Scholium; one sees immediately that $ \nu'^\bullet(f \otimes g) = \lambda'^\bullet(f) \mu'^\bullet(g) $ for $ f \in \mathcal{F}_+(S) $ and $ g \in \mathcal{F}_+(T) $; therefore $ \nu' = \lambda' \otimes \mu' $ by Prop. 10 of No. 5. Since the topology of $ X' $ is finer than that of $ X $, every $ \nu $-moderated function is $ \nu' $-moderated. This procedure permits extending without new proof the Lebesgue–Fubini theorem (Ch. V, $ \S 8 $, No. 4, Th. 1) to the present situation.

### 7. A result on the disintegration of measures

#### Proposition 13 {#int-ix-s2-prop-13 .statement}

*Let $ X $ be a topological space, $ \nu $ a moderated measure on $ X $, $ p $ a $ \nu $-proper mapping of $ X $ into a topological space $ T $, and $ \mu = p(\nu) $. Assume that every compact subspace of $ X $ is metrizable. Then there exists a mapping $ t \mapsto \lambda_t $ of $ T $ into $ \mathcal{M}_+(X) $ having the following properties:

a) for every $ t \in T $, the measure $ \lambda_t $ is carried by $ \overline{p}^{-1}(t) $;
b) for every universally measurable$^{(1)}$ positive function $ f $ on $ X $, the function $ t \mapsto \lambda_t^\bullet(f) $ is universally measurable on $ T $ and*

$$
\int_X f(x)\, d\nu(x) = \int_T d\mu(t) \int_X f(x)\, d\lambda_t(x);
$$

\footnotetext{(1) A mapping of a topological space $ X $ into a topological space $ Y $ is said to be *universally measurable* if it is $ \mu $-measurable for every measure $ \mu $ on $ X $ (cf. Ch. V, $ \S 3 $, No. 4).}

c) the set of $ t \in T $ such that $ \lambda_t(1) \neq 1 $ is locally $ \mu $-negligible.
Moreover, if $ t \mapsto \lambda'_t $ is a mapping of $ T $ into $ \mathcal{M}_+(X) $ satisfying the conditions a) and b), the set of $ t \in T $ such that $ \lambda_t \neq \lambda'_t $ is locally $ \mu $-negligible.
We will need an auxiliary result:

#### Lemma 4 {#int-ix-s2-lem-4 .statement}

Let $ X $ be a topological space, $ \nu $ a measure on $ X $, and $ f $ a $ \nu $-measurable mapping of $ X $ into a topological space $ F $ (Hausdorff or not). There exists a universally measurable mapping $ f' $ of $ X $ into $ F $, equal to $ f $ locally $ \nu $-almost everywhere.

The proof is identical to that of Prop. 7 of Ch. V, §3, No. 4, on taking into account Prop. 10 of §1, No. 8.

Let us pass to the proof of Prop. 13.
A) Suppose that $ X $ is compact and metrizable and that $ p $ is continuous and surjective:
The space $ T $ is then compact and metrizable (GT, IX, §2, No. 10). By Th. 1 of Ch. VI, §3, No. 1, there exists a mapping $ H : t \mapsto \eta_t $ of $ T $ into $ \mathcal{M}_+(X) $, vaguely $ \mu $-measurable and scalarly essentially $ \mu $-integrable, such that $ \nu = \int_T \eta_t \, d\mu(t) $ and such that $ \eta_t $ has total mass 1 and is carried by $ \overline{p}(t) $ for every $ t \in T $. Let $ (S_n)_{n \in \mathbf{N}} $ be a crushing of $ T $ for $ \mu $, such that the restriction of $ H $ to each of the sets $ S_n $ is continuous (§1, No. 8, Props. 10 and 11); we denote by $ \Lambda : t \mapsto \lambda_t $ the mapping of $ T $ into $ \mathcal{M}_+(X) $ that is equal to $ H $ on $ S = \bigcup_{n \in \mathbf{N}} S_n $ and to 0 on $ T - S $. It is clear that $ \nu = \int_T \lambda_t \, d\mu(t) $ and that $ \Lambda $ satisfies condition a) of the statement.
Let $ \theta $ be a measure on $ T $; the mapping $ \Lambda $ is vaguely $ \theta $-measurable and scalarly essentially $ \theta $-integrable, hence also $ \theta $-adequate (Ch. V, §3, No. 1, Prop. 2 b)). Let $ f $ be a universally measurable positive function on $ X $; by Prop. 5 of Ch. V, §3, No. 2 applied to $ \int \lambda_t \, d\theta(t) $, the mapping $ t \mapsto \lambda_t^\bullet(f) $ is $ \theta $-measurable, hence universally measurable in view of the arbitrariness of $ \theta $.
The formula (12) results from Prop. 5 of Ch. V, §3, No. 2.
B) Suppose that there exists a compact subset $ X' $ of $ X $ carrying the measure $ \nu $ and such that $ p_{X'} $ is continuous:
Set $ T' = p(X') $, and $ p' = p_{X'} $; let us denote by $ \nu' $ the measure $ \nu_{X'} $, and by $ \mu' $ the image measure $ p'(\nu') $ on $ T' $. Since $ p' $ is continuous and surjective and since $ X' $ is compact and metrizable, by A) there exists a mapping $ \Lambda' : t' \mapsto \lambda'_{t'} $ of $ T' $ into $ \mathcal{M}_+(X') $ satisfying the following conditions:
a') for every $ t' \in T' $, the measure $ \lambda'_{t'} $ is carried by $ X' \cap \overline{p}'(t') $;
b') for every universally measurable positive function $ f' $ on $ X' $, the function $ t' \mapsto \lambda'_{t'}^\bullet(f') $ is universally measurable on $ T' $ and
$$
\int_{X'} f'(x') \, d\nu'(x') = \int_{T'} d\mu'(t') \int_{X'} f'(x') \, d\lambda'_{t'}(x').
$$

Let $ t \in T $; if $ t $ belongs to $ T' $, let us denote by $ \lambda_t $ the image of $ \lambda'_t $ under the canonical injection of $ X' $ into $ X $, and if $ t $ belongs to $ T - T' $ we set $ \lambda_t = 0 $. The reader will verify without difficulty that the mapping $ t \mapsto \lambda_t $ satisfies the conditions $ a) $ and $ b) $ of the statement.

C) *Existence in the general case*:

The measure $ \nu $ on $ X $ being moderated, we may choose a covering $ (U_m)_{m \in \mathbf{N}} $ of $ X $ consisting of $ \nu $-integrable open sets. Let in addition $ (X_n)_{n \in \mathbf{N}} $ be a $ \nu $-crushing of $ X $ such that the restriction of $ p $ to each set $ X_n $ is continuous (\S 1, No. 8, Props. 10 and 11); denote by $ \nu_n $ the measure $ \varphi_{X_n} \cdot \nu $ on $ X $ and by $ \mu_n $ its image under $ p $. By B) there exists, for every integer $ n \in \mathbf{N} $, a mapping $ t \mapsto \alpha^n_t $ of $ T $ into $ \mathcal{M}_+(X) $ satisfying the following conditions:

$ a'') $ The measure $ \alpha^n_t $ is carried by $ \overline{p}(t) $ for all $ t \in T $.

$ b'') $ If $ f $ is a universally measurable positive function on $ X $, the positive function $ t \mapsto (\alpha^n_t)^*(f) $ on $ T $ is universally measurable and

$$
\int_X f(x)\, d\nu_n(x) = \int_T d\mu_n(t) \int_X f(x)\, d\alpha^n_t(x).
$$

One has $ \nu = \sum_{n \in \mathbf{N}} \nu_n $ and $ \mu = \sum_{n \in \mathbf{N}} \mu_n $; it follows immediately from Prop. 3 of No. 2 and the above Lemma 4 that there exists a sequence $ (g_n)_{n \in \mathbf{N}} $ of universally measurable positive functions on $ T $ such that $ \mu_n = g_n \cdot \mu $ for all $ n \in \mathbf{N} $ and such that $ \sum_{n \in \mathbf{N}} g_n = 1 $. For every $ t \in T $, let us denote by $ \beta^n_t $ the measure $ g_n(t) \cdot \alpha^n_t $ on $ X $ and by $ q_t $ the encumbrance $ \sum_{n \in \mathbf{N}} (\beta^n_t)^* $ on $ X $. Let $ f $ be a universally measurable positive function on $ X $; using Prop. 2 of No. 2 and summing over $ n $ in (13), we obtain

$$
\int_X f(x)\, d\nu(x) = \int_T q_t(f)\, d\mu(t);
$$

it is moreover clear that the function $ t \mapsto q_t(f) $ on $ T $ is universally measurable.

For every $ m \in \mathbf{N} $, let $ E_m $ be the set of $ t \in T $ such that $ q_t(U_m) = +\infty $; the set $ E_m $ is universally measurable because this is true of the mapping $ t \mapsto q_t(U_m) $, and $ E_m $ is locally $ \mu $-negligible by the formula (14) applied to $ f = \varphi_{U_m} $, since $ \nu^*(U_m) $ is finite. The set $ E = \bigcup_{m \in \mathbf{N}} E_m $ is therefore universally measurable and locally $ \mu $-negligible. We set $ \lambda_t = 0 $ for $ t \in E $. Moreover, let $ t \in T - E $; the encumbrance $ q_t $ is locally bounded since the open sets $ U_m $ cover $ X $ and since $ q_t(U_m) $ is finite; by Prop. 7 of \S 1, No. 7, there exists a measure $ \lambda_t $ on $ X $ such that $ q_t = \lambda_t^* $ and $ \lambda_t = \sum_{n \in \mathbf{N}} \beta^n_t $. It is immediate that the mapping $ t \mapsto \lambda_t $ satisfies the conditions $ a) $ and $ b) $ of the statement.

D) *Proof of c)*:
Let $ f $ be a universally measurable function on $ X $ that is positive and bounded; we are going to show that the universally measurable function $ h_f : t \mapsto \lambda_t^\bullet(f) $ on $ T $ is a density for the measure $ \mu_f = p(f \cdot \nu) $ with respect to $ \mu = p(\nu) $. Let $ K $ be a compact subset of $ T $ and let $ A = \overline{p}^{-1}(K) $. For every $ t \in T $, the measure $ \lambda_t $ is carried by $ \overline{p}^{-1}(t) $; if $ t $ belongs to $ K $ then $ \overline{p}^{-1}(t) \subset A $, whence $ \lambda_t^\bullet(f \varphi_A) = \lambda_t^\bullet(f) $; on the other hand, if $ t $ belongs to $ T - K $ then $ \overline{p}^{-1}(t) \subset X - A $, whence $ \lambda_t^\bullet(f \varphi_A) = 0 $. Applying the formula (12) to $ f \cdot \varphi_A $,$^{(1)}$ we obtain

$$
\mu_f(K) = \int_A^\bullet f(x)\, d\nu(x) = \int_K^\bullet d\mu(t) \int_X^\bullet f(x)\, d\lambda_t(x) = \int_K^\bullet h_f(t)\, d\mu(t),
$$

which establishes the relation $ \mu_f = h_f \cdot \mu $.

Letting $ f = 1 $, one sees that the function $ h_1 : t \mapsto \| \lambda_t \| $ is a density of the measure $ \mu_1 = \mu $ with respect to $ \mu $, hence is equal to 1 locally $ \mu $-almost everywhere in $ T $.

E) *Uniqueness*:
Let $ t \mapsto \lambda_t^i $ (for $ i = 1, 2 $) be two mappings of $ T $ into $ \mathcal{M}_+(X) $ satisfying the conditions $ a) $ and $ b) $ of the statement. As in C), choose a $ \mu $-crushing $ (X_n)_{n \in \mathbf{N}} $ of $ X $ such that $ p_{X_n} $ is continuous for every $ n \in \mathbf{N} $, and set $ N = X - \bigcup_{n \in \mathbf{N}} X_n $. For every integer $ n \in \mathbf{N} $, choose a countable set $ D_n $ of positive functions on $ X $, zero outside $ X_n $, whose restrictions to $ X_n $ form a dense set in the normed space $ \mathcal{C}(X_n) $ (apply Th. 1 of GT, X, §3, No. 3 to the metrizable compact space $ X_n $). We set $ D = \bigcup_{n \in \mathbf{N}} D_n $.

Let $ f \in D $; by D), the functions $ t \mapsto (\lambda_t^1)^\bullet(f) $ and $ t \mapsto (\lambda_t^2)^\bullet(f) $ are densities of the measure $ \mu_f $ with respect to $ \mu $, and so there exists a locally $ \mu $-negligible set $ E_f $ in $ T $ such that $ (\lambda_t^1)^\bullet(f) = (\lambda_t^2)^\bullet(f) $ for $ t \in T - E_f $. Moreover, by (12), the set $ F_i $ of $ t \in T $ such that $ (\lambda_t^i)^\bullet(N) \neq 0 $ is locally $ \mu $-negligible for $ i = 1, 2 $. Since $ D $ is countable, the set $ G = (\bigcup_{f \in D} E_f) \cup F_1 \cup F_2 $ is locally $ \mu $-negligible; for $ t \in T - G $, we have $ (\lambda_t^1)^\bullet(N) = (\lambda_t^2)^\bullet(N) = 0 $ and $ (\lambda_t^1)_{X_n} = (\lambda_t^2)_{X_n} $, whence $ \lambda_t^1 = \lambda_t^2 $ by Prop. 9 of §1, No. 8.

Q.E.D.

#### Remark {#int-ix-s2-n7-rem-1 .statement}

— 1) If $ X $ is a Souslin space, then every compact subspace of $ X $ is a Souslin space, hence is metrizable (TG, IX, Appendix I, Cor. 2 of Prop. 3),$^{(2)}$

(1) In case $ f \cdot \varphi_A $ is not universally measurable, make use of *Remark 2*) below.
(2) This result does not appear in GT (cf. the footnote to *Remark 1* of §1, No. 9).

and every measure on X is moderated (\S 1, No. 9, Remark 1). By Prop. 13, every measure $ \nu $ on X therefore admits a disintegration with respect to every $ \nu $-proper mapping.

2) With the notations of Prop. 13, let $ f $ be a positive $ \nu $-measurable function. One can prove, as in Ch. V, \S 3, No. 2, Prop. 5, that the set of $ t \in T $ such that $ f $ is not $ \lambda_t $-measurable is locally $ \mu $-negligible, that $ t \mapsto \lambda_t^\bullet(f) $ is $ \mu $-measurable, and that the relation (12) again holds.

### Exercises {#int-ix-s2-exercises}

See the [exercises for § 2](exercises/s2/).
