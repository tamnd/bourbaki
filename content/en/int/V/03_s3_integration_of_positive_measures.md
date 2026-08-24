---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 3
section_title: Integration of positive measures
lang: en
source: int-i-vi
book_pages: INT V.96-INT V.98
pdf_pages: 0270-0286, 0351-0353
extraction: ocr
subsections:
    - "no": 1
      title: Functions with values in a space of measures
      page: 0
      pdf_page: 270
    - "no": 2
      title: Superimposed integrals of positive functions
      page: 20
      pdf_page: 275
    - "no": 3
      title: Superimposed integrals of functions with values in a Banach space
      page: 24
      pdf_page: 279
    - "no": 4
      title: Universally measurable functions
      page: 25
      pdf_page: 280
    - "no": 5
      title: Diffusions
      page: 26
      pdf_page: 281
    - "no": 6
      title: Composition of bounded diffusions
      page: 29
      pdf_page: 284
statements: 30
exercises: 11
content_sha256: 5df5ceee4f3e12a558205316567b31117b43c3e350045788e46ec606a50f4590
---

## § 3. INTEGRATION OF POSITIVE MEASURES

### 1. Functions with values in a space of measures

Let $ X $ be a locally compact space, $ \mathcal{M}_+(X) $ the convex cone of positive measures on $ X $. Throughout the rest of this chapter, $ \mathcal{M}_+(X) $ will be equipped with the topology induced by the vague topology on $ \mathcal{M}(X) $ (Ch. III, §1, No. 9); thus, to say that a mapping $ \Lambda : t \mapsto \lambda_t $ of the locally compact space $ T $ into $ \mathcal{M}_+(X) $ is continuous means that, for every function $ f \in \mathcal{K}(X) $, the numerical function $ t \mapsto \lambda_t(f) $ is continuous. In this case we shall also say that $ \Lambda $ is vaguely continuous on $ T $. To say that a mapping $ \Lambda : t \mapsto \lambda_t $ is $ \mu $-measurable means that the set of compact subsets $ K $ of $ T $, such that the restriction of $ \Lambda $ to $ K $ is vaguely continuous, is

Let $ \Lambda : t \mapsto \lambda_t $ be a mapping of T into $ \mathcal{M}_+(X) $; we shall say that Λ is scalarly essentially integrable for the measure μ if, for every function $ f \in \mathcal{K}(X) $, the function $ t \mapsto \lambda_t(f) $ is essentially μ-integrable. If one sets $ \nu(f) = \int \lambda_t(f)\, d\mu(t) $, it is clear that ν is a positive linear form on $ \mathcal{K}(X) $, hence is a measure on X (Ch. III, §1, No. 5, Th. 1). We will say that ν is the integral of the function Λ with values in $ \mathcal{M}_+(X) $, and we will write $ \nu = \int \lambda_t\, d\mu(t) $.

The preceding definition is a special case of the concept of weak integral, which will be treated in a general manner in Ch. VI.

If $ f $ denotes an element of $ \mathcal{K}(X) $, the integral $ \int \lambda_t(f)\, d\mu(t) $ will also, by an abuse of notation, be denoted $ \int d\mu(t) \int f(x)\, d\lambda_t(x) $; the definition of the integral $ \nu = \int \lambda_t\, d\mu(t) $ may then be written

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

We shall make analogous abuses of notation in the sequel, for upper integrals, essential upper integrals, and integrals of functions with values in a Banach space.

#### Example 1 {#int-v-s3-n1-exa-1 .statement}

Suppose that T is a discrete space, and that μ is the measure on T defined by placing a mass +1 at each point of T (Ch. III, §1, No. 3). Let h be a function $ \geqslant 0 $ defined on T; since the function h is lower semi-continuous (even continuous) on T, $ \mu^*(h) = \mu^\bullet(h) = \sum_{t \in T} h(t) $ (Ch. IV, §1, No. 1, Example).

For the measure μ, the notions of integrable function and essentially integrable function are therefore identical. This being so, to say that a mapping $ t \mapsto \lambda_t $ of T into $ \mathcal{M}_+(X) $ is scalarly essentially μ-integrable amounts to saying that the family $ (\lambda_t)_{t \in T} $ is summable (§2, No. 1), and one then has $ \int \lambda_t\, d\mu(t) = \sum_{t \in T} \lambda_t $. Note that the mapping $ t \mapsto \lambda_t $ is vaguely continuous.

#### Example 2 {#int-v-s3-n1-exa-2 .statement}

The mapping $ t \mapsto \varepsilon_t $ of T into $ \mathcal{M}_+(T) $ is vaguely continuous, scalarly essentially μ-integrable for every positive measure μ on T, and one has $ \int \varepsilon_t\, d\mu(t) = \mu $.

#### Proposition 1 {#int-v-s3-prop-1 .statement}

Suppose that μ is the supremum of an increasing directed family $ (\mu_i)_{i \in I} $ of positive measures on T; in order that $ \Lambda : t \mapsto \lambda_t $ be scalarly essentially μ-integrable, it is necessary and sufficient that Λ be scalarly essentially $ \mu_i $-integrable for all $ i \in I $ and that the family $ (\int \lambda_t\, d\mu_i(t))_{i \in I} $ be bounded above in $ \mathcal{M}(X) $. One then has,

$$
\int \lambda_t\, d\mu(t) = \sup_{i \in I} \int \lambda_t\, d\mu_i(t).
$$

For, verifying that $ \Lambda $ is scalarly essentially integrable for a positive measure $ \eta $ on $ T $ comes down to verifying that $ t \mapsto \lambda_t(g) $ is $ \eta $-measurable and admits a finite essential upper integral, with respect to $ \eta $, for every function $ g \in \mathcal{H}_+(X) $. The proposition therefore follows at once from Prop. 11 of §1, No. 4 and its Corollary 2.

#### Corollary {#int-v-s3-n1-cor-1 .statement}

— *Suppose that $ \mu $ is the sum of a summable family $ (\mu_\alpha)_{\alpha \in A} $ of positive measures on $ T $; in order that $ \Lambda : t \mapsto \lambda_t $ be scalarly essentially $ \mu $-integrable, it is necessary and sufficient that $ \Lambda $ be scalarly essentially $ \mu_\alpha $-integrable for every $ \alpha \in A $ and that the family of measures $ \int \lambda_t d\mu_\alpha(t) $ be summable. One then has*

$$
\int \lambda_t d\mu(t) = \sum_{\alpha \in A} \int \lambda_t d\mu_\alpha(t).
$$

It follows immediately that every scalarly essentially $ \mu $-integrable mapping is also scalarly essentially $ \mu' $-integrable for every measure $ \mu' \leq \mu $.

In this section we shall limit ourselves to the study of scalarly essentially integrable mappings of $ T $ into $ \mathcal{M}_+(X) $ that have the property contemplated in the following definition:

#### Definition 1 {#int-v-s3-def-1 .statement}

— *Let $ X $ be a locally compact space, $ \Lambda : t \mapsto \lambda_t $ a scalarly essentially $ \mu $-integrable mapping of $ T $ into $ \mathcal{M}_+(X) $, and $ \nu $ the integral of $ \Lambda $.

We say that $ \Lambda $ is $ \mu $-pre-adequate if, for every lower semi-continuous function $ f \geq 0 $ defined on $ X $, the function $ t \mapsto \int^\bullet f d\lambda_t $ is $ \mu $-measurable on $ T $ and*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

*We say that $ \Lambda $ is $ \mu $-adequate (*) if $ \Lambda $ is $ \mu' $-pre-adequate for every positive measure $ \mu' \leq \mu $.*

It can be shown that if $ \Lambda $ is $ \mu $-pre-adequate and if the measure $ \nu = \int \lambda_t d\mu(t) $ is moderated—in particular if $ X $ is countable at infinity—then $ \Lambda $ is $ \mu $-adequate (Exer. 7); however, it is not known if these concepts are in general equivalent. In the statements in Nos. 2 and 3 below, the assertions preceded by an a) or a b) extend at once to pre-adequate mappings, whereas those preceded by a c) are valid only for adequate mappings.

(*) In the first edition, ' $ \mu $-adequate' mappings were defined to be the scalarly essentially $ \mu $-integrable and vaguely $ \mu $-measurable mappings. The definition given here is more general (Prop. 2 below).

The following proposition often permits one to verify that a given mapping is $ \mu $-adequate.

#### Proposition 2 {#int-v-s3-prop-2 .statement}

— Let $ \Lambda : t \mapsto \lambda_t $ be a scalarly essentially $ \mu $-integrable mapping of $ T $ into $ \mathcal{M}_+(X) $, and let $ \nu = \int \lambda_t \, d\mu(t) $.

a) *If $ \Lambda $ is vaguely continuous, then the mapping $ t \mapsto \lambda_t^\bullet(f) $ is lower semi-continuous for every lower semi-continuous function $ f \geqslant 0 $ defined on $ X $, $ \Lambda $ is $ \mu $-adequate, and we have the relation*

$$
\int^* f(x) \, d\nu(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

b) *If $ \Lambda $ is vaguely $ \mu $-measurable, then $ \Lambda $ is $ \mu $-adequate.*

c) *If the topology of $ X $ admits a countable base, then $ \Lambda $ is vaguely $ \mu $-measurable (hence also $ \mu $-adequate).*

Let $ f $ be a lower semi-continuous function $ \geqslant 0 $ defined on $ X $. Let $ F $ be the set, directed for the relation $ \leqslant $, of functions $ g \in \mathcal{K}(X) $ such that $ 0 \leqslant g \leqslant f $. For $ g \in F $, denote by $ h_g $ the function defined on $ T $ by $ h_g(t) = \lambda_t(g) $. Similarly, set

$$
h_f(t) = \lambda_t^*(f) = \lambda_t^\bullet(f) = \sup_{g \in F} h_g(t)
$$

(§1, No. 1, Prop. 4). Let us make the following hypothesis, weaker than that of a): assume only that the restriction of $ \Lambda $ to $ S $ is vaguely continuous, where $ S $ is a closed subset of $ T $ that contains the support of $ \mu $. For $ g \in F $, denote by $ \overline{h}_g $ the numerical function that coincides with $ h_g $ on $ S $ and has the value $ +\infty $ on $ C_S $. Set $ \overline{h}_f = \sup_{g \in F} \overline{h}_g $; then $ \overline{h}_f = h_f $ on $ S $. For every $ g \in F $, the function $ \overline{h}_g $ is lower semi-continuous; $ \overline{h}_f $ is therefore lower semi-continuous and, since the family $ (\overline{h}_g)_{g \in F} $ is directed,

$$
\mu^*(\overline{h}_f) = \sup_{g \in F} \mu^*(\overline{h}_g) = \sup_{g \in F} \mu^*(h_g) = \sup_{g \in F} \nu(g) = \nu^*(f)
$$

(Ch. IV, §1, No. 1, Th. 1 and §2, No. 3, Prop. 6). Since $ h_f = \overline{h}_f $ on $ S $, hence almost everywhere, this may also be written $ \mu^*(h_f) = \nu^*(f) $, an equality identical to (5). Similarly, $ f $ and $ \overline{h}_f $ being lower semi-continuous, the preceding relations yield the equality $ \mu^\bullet(\overline{h}_f) = \nu^\bullet(f) $ (§1, No. 1, Prop. 4); since $ \overline{h}_f = h_f $ on $ S $, it follows that $ \mu^\bullet(h_f) = \nu^\bullet(f) $ (§1, No. 1, Prop. 1), an equality identical to (4). The mapping $ \Lambda $ is therefore $ \mu $-pre-adequate; but one could have replaced everywhere in this argument $ \mu $ by $ \mu' \leqslant \mu $, and $ \nu $ by $ \nu' = \int \lambda_t \, d\mu'(t) $, because $ \Lambda $ is also scalarly essentially $ \mu' $-integrable and $ S $ contains the support of $ \mu' $. It follows from this that $ \Lambda $ is $ \mu $-adequate.

Suppose $ \Lambda $ is vaguely continuous; we may take $ S = T $; then $ h_f = \overline{h}_f $ is lower semi-continuous, which completes the proof of part a) of the statement.

Assume that $ \Lambda $ is vaguely $ \mu $-measurable and let us prove b). The set $ \mathcal{K} $ of compact subsets K of T such that the restriction of $ \Lambda $ to K is continuous being $ \mu $-dense (Ch. IV, §5, No. 10, Prop. 15), there exists a summable family $ (\mu_\alpha)_{\alpha \in A} $ of measures on T such that $ \mu = \sum_{\alpha \in A} \mu_\alpha $ and the support of each of the measures $ \mu_\alpha $ belongs to $ \mathcal{K} $ (§2, No. 3, Prop. 4). For every $ \alpha \in A $, the mapping $ \Lambda $ is scalarly essentially $ \mu_\alpha $-integrable, and we set $ \nu_\alpha = \int \lambda_t d\mu_\alpha(t) $; the family $ (\nu_\alpha) $ is summable, and its sum is equal to $ \nu $ (Cor. of Prop. 1). If $ f $ is a positive lower semi-continuous function defined on X, the first part of the proof, applied to the measures $ \mu_\alpha $ and the closed sets $ S_\alpha $, shows that:

$ 1^\circ $ $ h_f $ is $ \mu_\alpha $-measurable for every $ \alpha \in A $, hence is $ \mu $-measurable (§2, No. 2, Prop. 2), and

$ 2^\circ $ $ \int^* f(x) d\nu_\alpha(x) = \int^* d\mu_\alpha(t) \int^* f(x) d\lambda_t(x) $.

The formula (4) follows on summing over $ \alpha $ (§2, No. 2, Prop. 1). Applying the preceding argument to an arbitrary measure $ \mu' \leq \mu $ (which is legitimate, since $ \Lambda $ is scalarly essentially $ \mu' $-integrable and vaguely $ \mu' $-measurable, cf. §2, No. 2, Prop. 2), we conclude that $ \Lambda $ is $ \mu' $-pre-adequate, and b) is proved.

Finally, assuming that the topology of X admits a countable base, let us show that every scalarly essentially $ \mu $-integrable mapping $ \Lambda : t \mapsto \lambda_t $ of T into $ \mathcal{M}_+(X) $ is vaguely $ \mu $-measurable. This will result from the following lemma:

#### Lemma {#int-v-s3-n1-lem-1 .statement}

*Let X be a locally compact space having a countable base. Then, there exists in $ \mathcal{K}(X) $ a countable subset S having the following property: for every function $ f \in \mathcal{K}(X) $, there exist a sequence $ (f_n) $ of elements of S and a positive function $ \varphi \in S $ such that, for every number $ \varepsilon > 0 $, $ |f_n - f| \leq \varepsilon \varphi $ provided n is sufficiently large.*

Let $ X' $ be the Alexandroff compactification of X, which is a metrizable compact space (GT, IX, §2, No. 9, Prop. 16 and Cor.); we identify $ \mathcal{K}(X) $ with a subset of $ \mathcal{C}(X') $. Let $ S' $ be a countable dense subset of the Banach space $ \mathcal{C}(X') $ (GT, X, §3, No. 3, Th. 1); we can suppose that $ S' $ contains the constant function $ n $ for every $ n \in \mathbf{N} $. Let $ (U_n) $ be a sequence of relatively compact open sets in X, with union X, such that $ \overline{U}_n \subset U_{n+1} $ for all n (GT, I, §9, No. 9, Prop. 15), and let $ \varphi_n $ be a function in $ \mathcal{K}_+(X) $ equal to 1 on $ \overline{U}_n $. We denote by S the countable set of elements of $ \mathcal{K}(X) $ of the form $ \varphi_n g $ ($ n \in \mathbf{N}, g \in S' $). If $ f \in \mathcal{K}(X) $, let $ (g_n) $ be a sequence of elements of $ S' $ that converges uniformly to $ f $, and let k be an integer such that the support of $ f $ is contained in $ U_k $. Finally, let m be an integer that is an upper bound for the norms of the functions $ g_n $. The functions $ f_n = \varphi_k g_n $ belong to S and satisfy the statement, with $ \varphi = m \varphi_k $.

The lemma having been established, and the mapping $ t \mapsto \lambda_t(g) $ being essentially $ \mu $-integrable for every $ g \in S $, the mapping $ t \mapsto (\lambda_t(g))_{g \in S} $ of T into $ \mathbf{R}^S $ is $ \mu $-measurable (Ch. IV, §5, No. 3, Th. 1). The set $ \mathcal{K} $, of compact subsets K of T such that the restriction of this mapping to K is continuous, is therefore $ \mu $-dense, and it will suffice to show that the restriction of $ \Lambda $ to every $ K \in \mathcal{K} $ is continuous. Now, let $ f $ be any element of $ \mathcal{K}(X) $, $ f_n $ and $ \varphi $ elements of S satisfying the statement of the Lemma; the function $ t \mapsto \lambda_t(f) $ is then the uniform limit on K of the continuous functions $ t \mapsto \lambda_t(f_n) $; it is therefore continuous on K, and the proposition is proved.

### 2. Superimposed integrals of positive functions

For the rest of the section, absent express mention to the contrary, we shall denote by X a locally compact space, by $ \Lambda : t \mapsto \lambda_t $ a $ \mu $-adequate mapping of T into $ \mathcal{M}_+(X) $, and by $ \nu $ the integral of $ \Lambda $.

#### Proposition 3 {#int-v-s3-prop-3 .statement}

— Let f be a numerical function $ \geqslant 0 $ defined on X.
a) The following inequalities hold:

$$
\int^* f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

b) If $ \Lambda $ is vaguely continuous, then

$$
\int^* f(x)\, d\nu(x) \geqslant \int^* d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

c) If $ \lambda_t^\bullet(1) < +\infty $ locally $ \mu $-almost everywhere, then

$$
\int^\bullet f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) = \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

Let g be a lower semi-continuous function on X such that $ f \leqslant g $. For every $ t \in T $,

$$
\int^* f(x)\, d\lambda_t(x) \leqslant \int^* g(x)\, d\lambda_t(x),
$$

therefore, by (4) and Prop. 4 of §1,

$$
\int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \leqslant \int^\bullet d\mu(t) \int^* g(x)\, d\lambda_t(x) = \int^* g(x)\, d\nu(x).
$$

The first of the inequalities (6) then follows from the definition of $ \int^* f(x)\, d\nu(x) $ (Ch. IV, §1, No. 3, Def. 3), and the second follows immediately from it. The inequality (7) is proved in an analogous way if $ \Lambda $ is vaguely continuous, using (5) instead of (4).

Let us pass to the proof of (8). The mapping $ t \mapsto \lambda_t^*(1) $ is measurable, and finite locally $ \mu $-almost everywhere. The set $ \mathcal{K} $ of compact subsets of $ T $ such the restriction of $ t \mapsto \lambda_t^*(1) $ to $ K $ is finite and continuous is therefore $ \mu $-dense, and Prop. 4 of §2, No. 3 implies the existence of a summable family $ (\mu_\alpha)_{\alpha \in A} $ of positive measures, with supports belonging to $ \mathcal{K} $, such that $ \mu = \sum_{\alpha \in A} \mu_\alpha $. The mapping $ \Lambda $ is $ \mu_\alpha $-adequate for every $ \alpha \in A $; set $ \nu_\alpha = \int \lambda_t d\mu_\alpha(t) $. Prop. 1 shows that $ \nu = \sum_{\alpha \in A} \nu_\alpha $, and the relation (4), applied to the measure $ \mu_\alpha $ and the function 1, shows that $ \nu_\alpha $ is a bounded measure (because $ \lambda_t^*(1) $ is bounded on $ \operatorname{Supp}(\mu_\alpha) $). Let us then write the formula (6) for the measure $ \mu_\alpha $, replacing the symbol $ \int^* $ in the first member by $ \int^\bullet $, which is legitimate by Prop. 7 of §1; then

$$
\int^\bullet f(x) d\nu_\alpha(x) \geq \int^\bullet d\mu_\alpha(t) \int^* f(x) d\lambda_t(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x) d\lambda_t(x)
$$

(the last equality due to the fact that $ \lambda_t $ is bounded locally almost everywhere, and Prop. 7 of § 1). The inequality in (8) is then obtained by summing on $ \alpha $ (§2, No. 2, Prop. 1).

If no hypothesis analogous to that of c) is made, the inequality (8) may fail (Exer. 2).

#### Corollary 1 {#int-v-s3-prop-3-cor-1 .statement}

— *Let $ f $ be a function $ \geq 0 $ defined on $ X $, and let $ H $ be the set of $ t \in T $ such that $ f $ is not $ \lambda_t $-negligible.*
a) *If $ f $ $ \nu $-negligible, then $ H $ is locally $ \mu $-negligible.*
b) *If $ f $ is $ \nu $-negligible and $ \Lambda $ is vaguely continuous, then $ H $ is $ \mu $-negligible.*
c) *If $ f $ is locally $ \nu $-negligible and $ \lambda_t^\bullet(1) < +\infty $ locally $ \mu $-almost everywhere, then $ H $ is locally $ \mu $-negligible.*

#### Corollary 2 {#int-v-s3-prop-3-cor-2 .statement}

— *Let $ f $ be a function $ \geq 0 $ defined on $ X $, $ \nu $-measurable and $ \nu $-moderated. The set of $ t \in T $ such that $ f $ is not $ \lambda_t $-moderated is then locally $ \mu $-negligible (and even $ \mu $-negligible if $ \Lambda $ is vaguely continuous).*

For, $ f $ is the sum of a sequence of functions $ f_n \geq 0 $ such that $ f_n $ is zero outside a compact set $ K_n $ for $ n \geq 1 $, and $ f_0 $ is $ \nu $-negligible (§1, No. 2, Prop. 6); $ f_0 $ is then $ \lambda_t $-negligible except for $ t $ forming a set that is locally $ \mu $-negligible (and even $ \mu $-negligible, if $ \Lambda $ is vaguely continuous) by Cor. 1, and the statement then follows at once.

#### Proposition 4 {#int-v-s3-prop-4 .statement}

— *Let $ f $ be a $ \nu $-measurable function defined on $ X $, with values in a topological space $ G $, and let $ M $ be the set of $ t \in T $ such that $ f $ is not $ \lambda_t $-measurable.*
a) *Suppose that $ f $ is constant on the complement of a $ \nu $-moderated subset of $ X $; then $ M $ is locally $ \mu $-negligible.*

b) *Suppose that f is constant on the complement of a ν-moderated subset of X, and that Λ is vaguely continuous; then M is μ-negligible.*

c) *Suppose that $ \lambda_t^\bullet(1) < +\infty $ locally μ-almost everywhere; then M is locally μ-negligible.*

Let us first prove a) (resp. b)). Since every ν-integrable set is contained in a ν-integrable open set, the function f is constant on the complement B of a countable union of ν-integrable open sets. There exists a partition of X − B formed by a ν-negligible set N and a sequence $(K_n)$ of compact sets such that the restriction of f to each $K_n$ is continuous. Let S be the set of $t \in T$ such that N is not $\lambda_t$-negligible: S is locally μ-negligible (resp. μ-negligible) by Cor. 1 of Prop. 3. The sets $K_n, B, N$ are measurable for every measure on X, and the restriction of f to each of them is $\lambda_t$-measurable for every $t \notin S$. The function f is therefore $\lambda_t$-measurable for every $t \notin S$ (Ch. IV, §5, No. 10, Prop. 16).

To establish c), let us take up again the notations in the proof of Prop. 3; since f is ν-measurable, it is measurable for each of the measures $\nu_\alpha \leq \nu$. Now, these measures are bounded, hence moderated, and it follows from a) that M is locally $\mu_\alpha$-negligible for every $\alpha \in A$. This implies that M is locally μ-negligible (§2, No. 2, Cor. 2 of Prop. 1).

#### Proposition 5 {#int-v-s3-prop-5 .statement}

*Let f be a ν-measurable positive numerical function defined on X, and let N be the set of $t \in T$ such that f is not both $\lambda_t$-measurable and $\lambda_t$-moderated.*

a) *Suppose that f is ν-moderated. The set N is then locally μ-negligible, the function $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ is μ-measurable, and*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

b) *Suppose that f is ν-moderated, and that Λ is vaguely continuous. The set N is then μ-negligible, the function $t \mapsto \int^* f(x) d\lambda_t(x)$ is μ-measurable and μ-moderated, and*

$$
\int^* f(x) d\nu(x) = \int^* d\mu(t) \int^* f(x) d\lambda_t(x).
$$

c) *Suppose that $\lambda_t^\bullet(1) < +\infty$ locally μ-almost everywhere. The set N is then locally μ-negligible, the function $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ is μ-measurable, and (9) holds.*

Let us first prove a) (resp. b)), assuming that f is ν-moderated. The assertions concerning the set N have already been established (Prop. 4, and Cor. 2 of Prop. 3). By Prop. 6 of §1, No. 2, we may limit ourselves to proving a) (resp. b)) in each of the following special cases:

1) The function $ f $ is $ \nu $-negligible.
2) There exists a compact set $ K $ such that $ f $ is zero outside $ K $ and the restriction of $ f $ to $ K $ is continuous.

The special case 1) has already been treated (Cor. 1 of Prop. 3). To treat the second, we denote by $ G $ a $ \nu $-integrable open set containing $ K $, by $ M $ a constant upper bound for $ f $, by $ h $ the lower semi-continuous function $ M \varphi_G $, and by $ g $ the function $ h - f $. Since the function $ f $ is upper semi-continuous on $ X $, $ g $ is lower semi-continuous and positive. Moreover, $ f, g, h $ are $ \nu $-integrable.

Let us then apply formula (4) (resp. (5)) to the lower semi-continuous functions $ h $ and $ g $. By subtraction, we see that the function

$$
t \mapsto \int^\bullet f(x)\, d\lambda_t(x) \quad (\text{resp. } \int^* f(x)\, d\lambda_t(x))
$$

is $ \mu $-measurable and that the formula (9) (resp. (10)) holds. Finally, under the hypothesis of b), the function $ t \mapsto \int^* f(x)\, d\lambda_t(x) $ has finite upper integral, hence is indeed $ \mu $-moderated.

To prove c), let us take up again the measures $ \mu_\alpha $ and $ \nu_\alpha $ of the proof of Prop. 3; since $ f $ is $ \nu_\alpha $-measurable and $ \nu_\alpha $-moderated, the assertion a) implies that $ t \mapsto \int^\bullet f(x)\, d\lambda_t(x) $ is $ \mu_\alpha $-measurable and that

$$
\int^\bullet f(x)\, d\nu_\alpha(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x)\, d\lambda_t(x).
$$

It remains only to sum on $ \alpha $, applying Props. 1 and 2 of §2, No. 2.

If $ f $ is not assumed to be $ \nu $-moderated, and if one does not make the assumption in c), then the relation (9) may not hold (Exer. 3).

#### Corollary {#int-v-s3-n2-cor-1 .statement}

— *Let $ \mathbf{f} $ be a function defined on $ X $, with values in a Banach space $ F $ or in $ \overline{\mathbf{R}} $, that is $ \nu $-measurable and $ \nu $-moderated. For $ \mathbf{f} $ to be $ \nu $-integrable, it is necessary and sufficient that*

$$
\int^\bullet d\mu(t) \int^\bullet |\mathbf{f}(x)|\, d\lambda_t(x) < +\infty.
$$

This follows at once from Prop. 5 and the criterion for integrability (Ch. IV, §5, No. 6, Th. 5).

### 3. Superimposed integrals of functions with values in a Banach space

#### Theorem 1 {#int-v-s3-thm-1 .statement}

— Let $ f $ be a function with values in a Banach space $ F $ or in $ \overline{\mathbf{R}} $, and let $ H $ be the set of $ t \in T $ for which $ f $ is not $ \lambda_t $-integrable.

a) *If $ f $ is $ \nu $-integrable, then $ H $ is locally $ \mu $-negligible, the function $ t \mapsto \int f(x)\, d\lambda_t(x) $ (defined for $ t \notin H $) is essentially $ \mu $-integrable, and*

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

b) *If $ f $ is $ \nu $-integrable and $ \Lambda $ is vaguely continuous, then $ H $ is moreover $ \mu $-negligible and the function $ t \mapsto \int f(x)\, d\lambda_t(x) $ (defined for $ t \notin H $) is $ \mu $-integrable.*

c) *If $ \lambda_t^*(1) < +\infty $ locally $ \mu $-almost everywhere, then the conclusions of a) remain true for $ f $ an essentially $ \nu $-integrable function.*

We are first going to establish a) (resp. b)). This statement is true when $ f $ is a positive numerical function (Prop. 5); if $ f $ is an integrable function with values in $ \overline{\mathbf{R}} $, this result may be applied to the positive functions $ f^+ $ and $ f^- $, and therefore extends at once to $ f $ by subtraction. It remains to treat the case of functions with values in $ F $. Let $ \mathcal{H} $ be the subspace of $ \mathcal{L}_F^1(\nu) $ formed by the linear combinations, with coefficients in $ F $, of the functions in $ \mathcal{K}(X) $; the result pertaining to real functions implies at once the validity of the statement for the elements of $ \mathcal{H} $. Now, $ \mathcal{H} $ is dense in $ \mathcal{L}_F^1(\nu) $; therefore, for every $ f \in \mathcal{L}_F^1(\nu) $, there exists a sequence $ (f_n) $ of elements of $ \mathcal{H} $ that has the following properties:

1) the sequence $ (f_n) $ converges to $ f $ in mean in $ \mathcal{L}_F^1(\nu) $, and $ \nu $-almost everywhere;
2) the function $ g = |f_0| + \sum_{n \in \mathbf{N}} |f_{n+1} - f_n| $ is such that $ \nu^*(g) < +\infty $ (Ch. IV, §3, No. 4, Th. 3).

Let $ N_1 $ be the set of $ t \in T $ such that $ \lambda_t^*(g) = +\infty $; $ N_1 $ is locally $ \mu $-negligible (resp. $ \mu $-negligible) by formula (6) (resp. (7)). For $ t \notin N_1 $, the $ f_n $ belong to $ \mathcal{L}_F^1(\lambda_t) $, the sequence $ (f_n) $ converges $ \lambda_t $-almost everywhere, as well as for the topology of convergence in mean in $ \mathcal{L}_F^1(\lambda_t) $ (Ch. IV, §3, No. 3, Prop. 6). Let $ M $ be set of $ x \in X $ such that $ f_n(x) $ does not converge to $ f(x) $: since $ M $ is $ \nu $-negligible, the set $ N_2 $ of $ t \in T $ such that $ M $ is not $ \lambda_t $-negligible is locally $ \mu $-negligible (resp. $ \mu $-negligible) by Cor. 1 of Prop. 3.

Suppose that $ t $ does not belong to $ N_1 \cup N_2 $; the sequence $ (f_n) $ converges in mean in $ \mathcal{L}_F^1(\lambda_t) $, and converges $ \lambda_t $-almost everywhere to $ f $. Therefore $ f \in \mathcal{L}_F^1(\lambda_t) $ and $ \int f\, d\lambda_t = \lim_{n \to \infty} \int f_n\, d\lambda_t $ (Ch. IV, §4, No. 1). The set $ H $ of the statement is thus contained in $ N_1 \cup N_2 $; it is therefore locally $ \mu $-negligible (resp. $ \mu $-negligible). On the other hand, the function $ t \mapsto \int f\, d\lambda_t $ is equal locally $ \mu $-almost everywhere to the limit of a sequence of $ \mu $-measurable functions; it is therefore $ \mu $-measurable. Finally, for every $ t \notin N_1 \cup N_2 $ and every $ n $, we have
$$
\left| \int f_n(x)\, d\lambda_t(x) \right| \leq \int^* g(x)\, d\lambda_t(x)
$$
by virtue of the inequality $ |f_n| \leq g $ and Prop. 2 of Ch. IV, §4, No. 2. Now, the function $ t \mapsto \int^* g(x)\, d\lambda_t(x) $ is essentially $ \mu $-integrable (resp. $ \mu $-integrable) by Prop. 5. We may therefore apply Lebesgue’s theorem, which yields
$$
\int d\mu(t) \int f(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int d\mu(t) \int f_n(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int f_n(x)\, d\nu(x).
$$
Since $ \int f_n(x)\, d\nu(x) $ tends to $ \int f(x)\, d\nu(x) $ as $ n $ tends to $ \infty $, by the hypotheses made on the sequence $ (f_n) $, the relation (11) follows and we have proved a) (resp. b)).

Now suppose that $ \lambda_t^\bullet(1) < +\infty $ locally $ \mu $-almost everywhere, and that $ g $ is an essentially $ \nu $-integrable function. Let $ f $ be a $ \nu $-integrable function such that $ g = f $ locally $ \nu $-almost everywhere (\S1, No. 3). Then $ g = f $ almost everywhere for $ \lambda_t $, except for $ t $ forming a locally $ \mu $-negligible set $ P $ (Cor. 1 c) of Prop. 3). Therefore $ \int g\, d\lambda_t = \int f\, d\lambda_t $ for all $ t \notin P \cup H $, and this completes the proof.

#### Remark {#int-v-s3-n3-rem-1 .statement}

Let $ \Lambda : t \mapsto \lambda_t $ be a $ \mu $-adequate mapping of $ T $ into $ \mathcal{M}_+(X) $. If a mapping $ \Lambda' : t \mapsto \lambda'_t $ of $ T $ into $ \mathcal{M}_+(X) $ is equal to $ \Lambda $ locally $ \mu $-almost everywhere, it follows at once from the definitions that $ \Lambda' $ is also $ \mu $-adequate, and that $ \Lambda $ and $ \Lambda' $ have the same integral. If now $ H : t \mapsto \eta_t $ is a function with values in $ \mathcal{M}_+(X) $, defined locally $ \mu $-almost everywhere, we shall again say that $ H $ is $ \mu $-adequate if it is equal locally $ \mu $-almost everywhere to a mapping $ \Lambda : t \mapsto \lambda_t $ that is everywhere defined and $ \mu $-adequate. We then set $ \int \eta_t\, d\mu(t) = \int \lambda_t\, d\mu(t) $, a definition that does not depend on the function $ \Lambda $ utilized. We leave to the reader the task of verifying that the propositions proved in the preceding Nos. extend to $ \mu $-adequate functions defined locally $ \mu $-almost everywhere.

### 4. Universally measurable functions

#### Definition 2 {#int-v-s3-def-2 .statement}

*A mapping f of T into a topological space F is said to be universally measurable if it is $ \mu $-measurable for every positive measure $ \mu $ on T.*

The subsets of T whose characteristic function is universally measurable are called universally measurable sets. They form a tribe on T (Ch. IV, §5, No. 4, Cor. 2 of Th. 2) that contains the Borel sets (same ref., Cor. 3), and the Souslin sets if T is metrizable (Ch. IV, §5, No. 1, Cor. 2 of Prop. 3). For a mapping $ f $ of T into a topological space F, metrizable and separable, to be universally measurable, it is necessary and sufficient that the inverse image under $ f $ of every closed ball in F be a universally measurable subset of T (Ch. IV, §5, No. 5, Th. 4).

#### Proposition 6 {#int-v-s3-prop-6 .statement}

*For a mapping $ f $ of T into a topological space F to be universally measurable, it is necessary and sufficient that $ f $ be measurable for every positive measure on T with compact support.*

The condition is obviously necessary; on the other hand it is sufficient, because every positive measure $ \mu $ is the sum of a family of measures with compact support (§2, No. 3, Prop. 4): the statement then follows from Prop. 2 of §2, No. 2.

#### Proposition 7 {#int-v-s3-prop-7 .statement}

*Let $ \mu $ be a positive measure on T, and let $ f $ be a $ \mu $-measurable mapping of T into a topological space F. Then, there exists a universally measurable mapping $ f' $ of T into F such that $ f = f' $ locally $ \mu $-almost everywhere.*

Let $ \mathcal{K} $ be the set of compact sets in T such that the restriction of $ f $ to K is continuous; since $ \mathcal{K} $ is $ \mu $-dense (Ch. IV, §5, No. 10, Prop. 15), there exists a locally countable family $ (K_i)_{i \in I} $ of pairwise disjoint elements of $ \mathcal{K} $ such that the set $ N = T - \bigcup_{i \in I} K_i $ is locally $ \mu $-negligible (Ch. IV, §5, No. 9, Prop. 14). Let $ x $ be an element of F; set

$$
f'(t) = f(t) \quad \text{if } t \in \bigcup_{i \in I} K_i,
$$
$$
f'(t) = x \quad \text{if } t \in N.
$$

The functions $ f $ and $ f' $ are equal locally $ \mu $-almost everywhere. On the other hand, $ N \cap K $ is a Borel subset of K for every compact set K in T, since the family $ (K_i) $ is locally countable. It follows that N is a universally measurable set, and that $ f' $ is a universally measurable function (Ch. IV, §5, No. 10, Prop. 16).

### 5. Diffusions

#### Definition 3 {#int-v-s3-def-3 .statement}

*Let X be a locally compact space, and let $ \Lambda : t \mapsto \lambda_t $ be a mapping of T into $ \mathcal{M}_+(X) $. The mapping $ \Lambda $ is said to be a diffusion* of T in X if Λ is adequate for every positive measure on T with compact support. The diffusion Λ is said to be bounded if all of the measures λ_t are bounded and $ \sup_{t \in T} \| \lambda_t \| < +\infty $; this quantity is then called the norm of Λ and is denoted $ \| \Lambda \| $.

The following proposition merely translates the definition:

#### Proposition 8 {#int-v-s3-prop-8 .statement}

— For a mapping $ \Lambda : t \mapsto \lambda_t $ of T into $ \mathcal{M}_+(X) $ to be a diffusion, it is necessary and sufficient that the following conditions be satisfied:
1) For every lower semi-continuous function $ f \geqslant 0 $ defined on X, the function $ t \mapsto \lambda_t^\bullet(f) $ is universally measurable on T.
2) For every function $ g \in \mathcal{K}_+(X) $, the function $ t \mapsto \lambda_t(g) $ is locally bounded in T.
3) For every lower semi-continuous function $ f \geqslant 0 $ defined on X and for every positive measure $ \mu $ on T with compact support, the following relation holds, where $ \nu $ denotes $ \int \lambda_t d\mu(t) $:

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

Suppose that $ \Lambda $ is a diffusion. The condition 1) is then satisfied by the definition of adequate mappings (No. 1, Def. 1) and Prop. 6; the condition 3) is satisfied by formula (4), since $ \Lambda $ is $ \mu $-adequate. Let $ g \in \mathcal{K}_+(X) $ and let $ u $ be the function $ t \mapsto \lambda_t(g) $ (universally measurable, by 1)); suppose that $ u $ is not locally bounded. There would then exist a compact set K such that $ u $ is not bounded on K, hence there would exist a sequence $ (t_n) $ of elements of K such that $ u(t_n) \geqslant n^2 $ for all $ n \geqslant 1 $; then $ u $ is not integrable for the measure $ \mu = \sum_{n \geqslant 1} \frac{1}{n^2} \varepsilon_{t_n} $ with compact support, contrary to the hypothesis on $ \Lambda $, which implies that $ t \mapsto \lambda_t(g) $ is integrable for every positive measure with compact support. The above three conditions are thus necessary. Conversely, the conditions 1) and 2) imply that $ \Lambda $ is scalarly essentially $ \mu $-integrable for every measure $ \mu $ with compact support. Since every measure $ \mu' \geqslant 0 $ that is bounded above by a measure $ \mu $ with compact support also has compact support, the conditions 1) and 3) express that $ \Lambda $ is $ \mu $-adequate for every positive measure with compact support, which is indeed the sought-for result.

#### Proposition 9 {#int-v-s3-prop-9 .statement}

— Let $ \Lambda : t \mapsto \lambda_t $ be a mapping of T into $ \mathcal{M}_+(X) $, such that the function $ t \mapsto \lambda_t(g) $ is universally measurable and locally bounded in T for every $ g \in \mathcal{K}_+(X) $. One can affirm that $ \Lambda $ is a diffusion in each of the following cases:

a) *the topology of X admits a countable base*;
b) *Λ is universally measurable for the vague topology*.

For, let $ μ $ be a positive measure on $ T $ with compact support; the mapping $ Λ $ is scalarly essentially $ μ $-integrable, hence $ μ $-adequate if either a) or b) is satisfied (No. 1, Prop. 2).

For the rest of this section, we shall adopt the following notations: we will denote by $ ⟨η, h⟩ $ the upper essential integral, for a positive measure $ η $, of a positive $ η $-measurable function $ h $. The mapping $ Λ : t ↦ λ_t $ will be a diffusion of $ T $ in $ X $. If $ f $ is a positive universally measurable function defined on $ X $, we shall denote by $ Λf $ the mapping $ t ↦ λ_t^*(f) $. If $ μ $ is a positive measure on $ T $ such that $ Λ $ is scalarly essentially $ μ $-integrable, we shall denote by $ μΛ $ the measure $ ∫ λ_t dμ(t) $. The definition of the integral then takes the form

$$
⟨μΛ, f⟩ = ⟨μ, Λf⟩ \quad \text{for } f ∈ \mathcal{K}_+(X).
$$

We shall say that a positive measure $ μ $ on $ T $ *belongs to the domain of $ Λ $* if $ Λ $ is $ μ $-adequate: this amounts to saying (in view of Prop. 8) that $ Λ $ is scalarly essentially $ μ $-integrable and $ ⟨μ'Λ, f⟩ = ⟨μ', Λf⟩ $ for every positive measure $ μ' ≤ μ $ and every lower semi-continuous positive function $ f $.

#### Proposition 10 {#int-v-s3-prop-10 .statement}

*Let $ f, g $ be two positive universally measurable functions on $ X $, let $ a $ be a number $ ≥ 0 $, and let $ μ $ and $ ν $ be two positive measures on $ T $. Then:*

a) $ Λ(f + g) = Λf + Λg $, $ Λ(af) = aΛf $.
b) *If $ μ $ and $ ν $ belong to the domain of $ Λ $, then so do $ μ + ν $ and $ aμ $, and one has* $ (μ + ν)Λ = μΛ + νΛ $, $ (aμ)Λ = a(μΛ) $.

The only non-obvious point is that $ μ + ν $ belongs to the domain of $ Λ $, which is treated by observing that every positive measure bounded above by $ μ + ν $ is of the form $ μ' + ν' $, where $ μ' ≤ μ $, $ ν' ≤ ν $ (the 'decomposition lemma', Ch. II, §1, No. 1). See also the next proposition.

#### Proposition 11 {#int-v-s3-prop-11 .statement}

*For a positive measure $ μ $ on $ T $ to belong to the domain of $ Λ $, it is necessary and sufficient that $ Λ $ be scalarly essentially $ μ $-integrable.*

This condition is obviously necessary. Conversely, suppose it is satisfied, and let $ f $ be a lower semi-continuous positive function defined on $ X $. The function $ Λf $ is universally measurable, hence $ μ $-measurable. We are going to prove that $ ⟨μ, Λf⟩ = ⟨μΛ, f⟩ $; since this equality will also be valid for every positive measure $ μ' ≤ μ $, because $ Λ $ is also scalarly essentially $ μ' $-integrable, it will follow that $ Λ $ is $ μ $-adequate.

Let $ (\mu_i)_{i∈I} $ be a summable family of positive measures with compact support, such that $ μ = ∑_{i∈I} μ_i $ (§2, No. 3, Prop. 4); the family of measures $ \mu_i \Lambda $ is then summable, and $ \mu \Lambda = \sum_{i \in I} \mu_i \Lambda $ (No. 1, Cor. of Prop. 1). Consequently $ \langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle $ (\S 2, No. 2, Prop. 1); but $ \Lambda $ is $ \mu_i $-adequate, thus $ \langle \mu_i \Lambda, f \rangle = \langle \mu_i, \Lambda f \rangle $. Again applying Prop. 1 of \S 2, we obtain the sought-for equality:

$$
\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i, \Lambda f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### Corollary 1 {#int-v-s3-prop-11-cor-1 .statement}

— *If $ \Lambda $ is a bounded diffusion, then every bounded positive measure $ \mu $ belongs to the domain of $ \Lambda $, and $ \| \mu \Lambda \| \leq \| \mu \| \| \Lambda \| $.*

#### Corollary 2 {#int-v-s3-prop-11-cor-2 .statement}

— *Suppose that $ \mu $ is the sum of a summable family $ (\mu_\alpha)_{\alpha \in A} $ of positive measures belonging to the domain of $ \Lambda $. For $ \mu $ to belong to the domain of $ \Lambda $, it is necessary and sufficient that the family of measures $ \mu_\alpha \Lambda $ be summable, in which case $ \mu \Lambda = \sum_{\alpha \in A} \mu_\alpha \Lambda $.*

It suffices to apply the Corollary of Prop. 1 of No. 1.

Proposition 5, expressed in the language of diffusions, takes the following form:

#### Proposition 12 {#int-v-s3-prop-12 .statement}

— *Let $ \mu $ be a positive measure on $ T $ that belongs to the domain of $ \Lambda $, and let $ f $ be a universally measurable function $ \geq 0 $ defined on $ X $. If $ f $ is moderated for the measure $ \mu \Lambda $, or if the measures $ \lambda_t $ are bounded, then the function $ \Lambda f $ is $ \mu $-measurable and*

$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### Corollary {#int-v-s3-n5-cor-1 .statement}

— *If $ X $ is countable at infinity, or if the measures $ \lambda_t $ are bounded, then the function $ \Lambda f $ is universally measurable on $ T $ for every universally measurable function $ f \geq 0 $ defined on $ X $, and (13) holds.*

### 6. Composition of bounded diffusions

#### Proposition 13 {#int-v-s3-prop-13 .statement}

— *Let $ T, X, Y $ be three locally compact spaces, $ \Lambda : t \mapsto \lambda_t $ a bounded diffusion of $ T $ in $ X $, and $ H : x \mapsto \eta_x $ a bounded diffusion of $ X $ in $ Y $. The mapping $ t \mapsto \lambda_t H $ is then a bounded diffusion of $ T $ in $ Y $, which is denoted by $ \Lambda H $, and*

$$
\| \Lambda H \| \leq \| \Lambda \| \| H \|.
$$

*Let $ f $ be a universally measurable function $ \geq 0 $ defined on $ Y $, and $ \mu $ a measure on $ T $. Suppose that $ \mu $ belongs to the domain of $ \Lambda $, and that* μΛ belongs to the domain of H; then μ belongs to the domain of ΛH, and

$$
\langle \mu(\Lambda H), f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda Hf \rangle;
$$
(15)
$$
(\mu \Lambda)H = \mu(\Lambda H); \quad \Lambda(Hf) = (\Lambda H)f.
$$

Set $ \gamma_t = \lambda_t H $; we shall denote by $ \Gamma $ the mapping $ \Lambda H $ of T into $ \mathcal{M}_+(Y) $, and by $ \Gamma f $ the function $ t \mapsto \langle \gamma_t, f \rangle $ (an abuse of notation, since we do not yet know whether $ \Gamma $ is a diffusion). Then $ \langle \gamma_t, f \rangle = \langle \lambda_t H, f \rangle = \langle \lambda_t, Hf \rangle $ by (13); since the function $ Hf $ is positive and universally measurable on X (Cor. of Prop. 12), it follows first of all that $ \Gamma f = \Lambda(Hf) $, and then that $ \Gamma f $ is universally measurable on T (same reference). It is clear that all of the measures $ \gamma_t $ have total mass at most equal to $ \| \Lambda \| \| H \| $. Consequently $ \Gamma g $ is universally measurable and bounded for every function $ g \in \mathcal{K}_+(Y) $; $ \Gamma $ is therefore scalarly essentially integrable for every bounded measure on T, and in particular for every measure with compact support. More generally, if $ \mu $ is a measure in the domain of $ \Lambda $, such that $ \mu \Lambda $ belongs to the domain of H, then, for $ g \in \mathcal{K}_+(Y) $,

$$
\langle \mu, \Gamma g \rangle = \langle \mu, \Lambda(Hg) \rangle = \langle \mu \Lambda, Hg \rangle = \langle (\mu \Lambda)H, g \rangle.
$$

Since the last quantity is finite, we see that $ \Gamma $ is scalarly essentially $ \mu $-integrable. Let us denote by $ \mu \Gamma $ the integral $ \int \gamma_t d\mu(t) $ (an abuse of notation, since we do not yet know whether $ \Gamma $ is a diffusion). The preceding relations may then be written

$$
\langle \mu \Gamma, g \rangle = \langle (\mu \Lambda)H, g \rangle,
$$

or also $ \mu \Gamma = (\mu \Lambda)H $ since $ g $ is arbitrary in $ \mathcal{K}_+(Y) $.

Consider anew the universally measurable function $ f \geqslant 0 $. We have

$$
\langle \mu \Gamma, f \rangle = \langle (\mu \Lambda)H, f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda(Hf) \rangle = \langle \mu, \Gamma f \rangle.
$$

When $ f $ is lower semi-continuous and $ \mu $ runs over the set of positive measures with compact support, these relations express that $ \Gamma $ is a diffusion of T in Y. The assertion then does no more than make explicit the relations obtained in the course of the above proof.

#### Definition 4 {#int-v-s3-def-4 .statement}

*The notations being those of Proposition 13, the diffusion $ \Lambda H $ is called the composed diffusion (or the composition) of the bounded diffusions H and $ \Lambda $.*

Let $ X_1, X_2, X_3, X_4 $ be four locally compact spaces, and $ \Lambda_1, \Lambda_2, \Lambda_3 $ three bounded diffusions, of $ X_1 $ in $ X_2 $, $ X_2 $ in $ X_3 $, $ X_3 $ in $ X_4 $, respectively. It follows at once from Prop. 13 that

$$
(\Lambda_1 \Lambda_2) \Lambda_3 = \Lambda_1 (\Lambda_2 \Lambda_3).
$$

We will therefore use these notations without parentheses for the composition of diffusions.

#### Example {#int-v-s3-n6-exa-1 .statement}

Let $ u $ be a universally measurable mapping of T into X, and $ v $ a universally measurable mapping of X into Y; by Prop. 2 b), one defines diffusions $ \Lambda $ and $ H $ by the formulas

$$
\lambda_t = \varepsilon_{u(t)}, \quad \eta_x = \varepsilon_{v(x)};
$$

the diffusion $ \Gamma = \Lambda H $ is then given by

$$
\gamma_t = \varepsilon_{(vou)(t)}.
$$

One is therefore careful to note that the order of composition of diffusions is the opposite of the usual order of the composition of functions.

### Exercises {#int-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
