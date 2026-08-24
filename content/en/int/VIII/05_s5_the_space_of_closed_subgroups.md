---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 5
section_title: The space of closed subgroups
lang: en
source: int-vii-ix
book_pages: INT VIII.73-INT VIII.74
pdf_pages: 0146-0159, 0173-0174
extraction: ocr
subsections:
    - "no": 1
      title: The space of Haar measures on the closed subgroups of G
      page: 46
      pdf_page: 146
    - "no": 2
      title: Semi-continuity of the volume of the homogeneous space
      page: 48
      pdf_page: 148
    - "no": 3
      title: The space of closed subgroups of G
      page: 51
      pdf_page: 151
    - "no": 4
      title: The case of groups without arbitrarily small finite subgroups
      page: 53
      pdf_page: 153
    - "no": 5
      title: The case of abelian groups
      page: 55
      pdf_page: 155
    - "no": 6
      title: Another interpretation of the topology of the space of closed subgroups
      page: 56
      pdf_page: 156
statements: 20
exercises: 6
content_sha256: df43a0eaeb027f0d65f04dd8a4fe236be3ba6c13fc86556941e52f7a5f9a53bb
---

## § 5. THE SPACE OF CLOSED SUBGROUPS

Throughout this section, G denotes a locally compact group and $ \mu $ a right Haar measure on G.

### 1. The space of Haar measures on the closed subgroups of G

#### Lemma 1 {#int-viii-s5-lem-1 .statement}

Let $ \alpha $ be a positive measure $ \neq 0 $ on G, S its support; the following two conditions are equivalent:
a) S is a closed subgroup of G and the measure induced by $ \alpha $ on S is a right Haar measure on S.
b) $ \delta(s)\alpha = \alpha $ for every $ s \in S $.
Moreover, when these conditions are satisfied, the set of $ t \in G $ such that $ \delta(t)\alpha = \alpha $ is equal to S.
It is clear that a) implies b); conversely, the relation b) implies that $ Sx = S $ for every $ x \in S $; in other words, the relations $ x \in S $ and $ y \in S $ imply that $ y \in Sx $, or again that $ yx^{-1} \in S $, and since S is nonempty, S is a closed subgroup of G. The set of $ t \in G $ such that $ St = S $ is then equal to S itself, whence the last assertion.

For the rest of the section, we denote by $ \Gamma $ the set of positive measures $ \neq 0 $ on G satisfying the conditions of Lemma 1, and for every $ \alpha \in \Gamma $ we denote by $ H_\alpha $ the closed subgroup of G that is the support of $ \alpha $.

#### Proposition 1 {#int-viii-s5-prop-1 .statement}

The set $ \Gamma $ is closed in the space $ \mathcal{M}_+(G) - \{0\} $ equipped with the vague topology.
We first prove the following lemmas:

#### Lemma 2 {#int-viii-s5-lem-2 .statement}

Let X be a locally compact space and for every measure $ \alpha \in \mathcal{M}_+(X) - \{0\} $, let $ S_\alpha $ be the support of $ \alpha $. Let $ \Phi $ be a filter on $ \mathcal{M}_+(X) - \{0\} $ that converges vaguely to a measure $ \alpha_0 \neq 0 $. Then, for every neighborhood V of a point s of the support of $ \alpha_0 $, there exists a set $ M \in \Phi $ such that, for every $ \alpha \in M $, one has $ V \cap S_\alpha \neq \varnothing $.
For, if $ \varphi \in \mathcal{K}_+(X) $ is a function with support contained in V and such that $ \int \varphi(x) d\alpha_0(x) > 0 $, by definition there exists a set $ M \in \Phi $ such that $ \int \varphi(x) d\alpha(x) > 0 $ for all $ \alpha \in M $, which implies $ V \cap S_\alpha \neq \varnothing $.

#### Lemma 3 {#int-viii-s5-lem-3 .statement}

Let E be a set filtered by a filter $ \Phi $, and let $ \xi \mapsto \alpha(\xi) $ be a mapping of E into $ \Gamma $ that converges vaguely with respect to $ \Phi $ to a measure $ \alpha_0 \neq 0 $. On the other hand, let $ \xi \mapsto t_\xi $ be a mapping of $ E $ into $ G $ such that $ t_\xi \in H_{\alpha(\xi)} $ for every $ \xi \in E $. If $ s $ is a cluster point of the mapping $ \xi \mapsto t_\xi $ with respect to $ \Phi $, then $ \delta(s)\alpha_0 = \alpha_0 $.

Replacing if necessary $ \Phi $ by a finer filter, we can suppose that $ s $ is a limit of $ \xi \mapsto t_\xi $ with respect to $ \Phi $; by Lemma 1, $ \delta(t_\xi)\alpha(\xi) = \alpha(\xi) $ for every $ \xi \in E $, and the conclusion follows from the continuity of the mapping $ (u, \lambda) \mapsto \delta(u)\lambda $ on $ G \times \mathcal{M}_+(G) $ (\S 3, No. 3, Prop. 13).

To prove Prop. 1 it suffices, by Lemma 1, to show that if a filter $ \Psi $ on $ \Gamma $ converges vaguely to a measure $ \alpha_0 \neq 0 $ and if $ s $ belongs to the support of $ \alpha_0 $, then $ \delta(s)\alpha_0 = \alpha_0 $. Now, for every neighborhood $ V $ of $ s $ in $ G $, there exists an $ M \in \Psi $ such that, for every $ \alpha \in M $, one has $ V \cap H_\alpha \neq \varnothing $, by Lemma 2. For every neighborhood $ V $ of $ s $ and every $ \alpha \in \Gamma $, let $ t_{V,\alpha} $ be a point of $ V \cap H_\alpha $ if $ V \cap H_\alpha \neq \varnothing $, and any point of $ H_\alpha $ in the contrary case; if $ \Theta $ is the section filter of the filter of neighborhoods of $ s $, and $ \Phi $ is the product filter $ \Theta \times \Psi $, then $ s $ is, by the foregoing, a cluster point of $ (V, \alpha) \mapsto t_{V,\alpha} $ with respect to $ \Phi $. Since, on the other hand, the mapping $ (V, \alpha) \mapsto \alpha $ has $ \alpha_0 $ as limit with respect to $ \Phi $, the proposition follows from Lemma 3.

#### Proposition 2 {#int-viii-s5-prop-2 .statement}

— Let $ \varphi $ be a function in $ \mathscr{K}_+(G) $ such that $ \varphi(e) > 0 $. Then the set $ \Gamma_\varphi $ of measures $ \alpha \in \Gamma $ such that $ \int \varphi(x)\,d\alpha(x) = 1 $ is compact for the vague topology.

The set $ \Gamma_\varphi $ is the intersection of $ \Gamma $ with the hyperplane of $ \mathcal{M}(G) $ formed by the $ \alpha $ such that $ \int \varphi(x)\,d\alpha(x) = 1 $; since this hyperplane is vaguely closed in $ \mathcal{M}(G) $ and does not contain 0, it follows from Prop. 1 that $ \Gamma_\varphi $ is vaguely closed in $ \mathcal{M}(G) $. It therefore suffices to show that for every compact subset $ K $ of $ G $, one has $ \sup_{\alpha \in \Gamma_\varphi} \alpha(K) < +\infty $ (Ch. III, §1, No. 9, Prop. 15). Now, let $ U $ be the open neighborhood of $ e $ in $ G $ defined by the inequality $ \varphi(x) > \varphi(e)/2 $; since $ 1 = \int \varphi(x)\,d\alpha(x) \geq \int_U \varphi(x)\,d\alpha(x) $ for $ \alpha \in \Gamma_\varphi $, one sees that, on setting $ c = 2/\varphi(e) $, one has $ \alpha(U) \leq c $ for every $ \alpha \in \Gamma_\varphi $. Let $ V $ be a symmetric open neighborhood of $ e $ in $ G $ such that $ V^2 \subset U $; let us show that $ \alpha(Vx) \leq c $ for every $ x \in G $ and every $ \alpha \in \Gamma_\varphi $. Indeed, this relation is trivial if $ Vx $ does not intersect the support $ H_\alpha $ of $ \alpha $; if, on the contrary, there exists an $ h \in Vx \cap H_\alpha $, then $ h = vx $ for some $ v \in V $, whence
$$
Vx = Vv^{-1}h \subset V^2h \subset Uh,
$$
and since $ \delta(h)\alpha = \alpha $, it follows that $ \alpha(Vx) \leq \alpha(Uh) = \alpha(U) \leq c $. Now let $ (x_i)_{1 \leq i \leq n} $ be a sequence of points of $ K $ such that the $ Vx_i $ form a covering of $ K $; it follows from the foregoing that $ \alpha(K) \leq \sum_{i=1}^n \alpha(Vx_i) \leq nc $ for every $ \alpha \in \Gamma_\varphi $; Q.E.D.

#### Proposition 3 {#int-viii-s5-prop-3 .statement}

— *Under the hypotheses of Prop. 2, the mapping* $ \alpha \mapsto \left( \langle \varphi, \alpha \rangle, \frac{\alpha}{\langle \varphi, \alpha \rangle} \right) $ *is a homeomorphism of* $ \Gamma $ *onto the product space* $ \mathbf{R}_+^* \times \Gamma_\varphi $.

Since the mapping $ \alpha \mapsto \langle \varphi, \alpha \rangle $ is vaguely continuous, it suffices to observe that $ \langle \varphi, \alpha \rangle \neq 0 $ for every measure $ \alpha \in \Gamma $, since $ e $ belongs to the support $ H_\alpha $ of $ \alpha $ and $ \varphi(e) > 0 $.

### 2. Semi-continuity of the volume of the homogeneous space

In this No., for every measure $ \alpha \in \Gamma $ we set

$$
Q_\alpha = G / H_\alpha ,
$$

and we denote by $ \pi_\alpha $ the canonical mapping $ G \to Q_\alpha $.

Let $ \Gamma^0 $ be the subset of $ \Gamma $ formed by the measures $ \alpha $ such that the subgroup $ H_\alpha $ of $ G $ is *unimodular*; the elements of $ \Gamma^0 $ are characterized by the fact that $ \alpha(f) = \alpha(\dot{f}) $ for every function $ f \in \mathcal{K}(G) $ (every function of $ \mathcal{K}(H_\alpha) $ being extendible to a function of $ \mathcal{K}(G) $ by Urysohn’s theorem); it follows that $ \Gamma^0 $ is a *closed* subset of $ \Gamma $. Recall that for every $ \alpha \in \Gamma^0 $, the quotient measure $ \mu_\alpha = \mu / \alpha $ on $ Q_\alpha $ is defined and is relatively invariant under $ G $ (Ch. VII, §2, No. 6, Th. 3); also recall that for every function $ f \in \mathcal{K}(G) $,

$$
\int_G f(x) d\mu(x) = \int_{Q_\alpha} d\mu_\alpha(\dot{x}) \int_{H_\alpha} f(xs) d\alpha(s) ,
$$

where $ \dot{x} = \pi_\alpha(x) $ is the canonical image of $ x \in G $ in $ Q_\alpha $.

#### Proposition 4 {#int-viii-s5-prop-4 .statement}

— *Let* $ \Gamma^0 $ *be the set of measures* $ \alpha \in \Gamma $ *such that* $ H_\alpha $ *is unimodular, and for every* $ \alpha \in \Gamma^0 $ *set* $ \mu_\alpha = \mu / \alpha $; *then the mapping* $ \alpha \mapsto \| \mu_\alpha \| $ *of* $ \Gamma^0 $ *into* $ \overline{\mathbf{R}} $ *is lower semi-continuous for the vague topology*.

For every $ \alpha \in \Gamma^0 $ and every function $ f \in \mathcal{K}(G) $, set

$$
f_\alpha(\dot{x}) = \int_{H_\alpha} f(xs) d\alpha(s) = (f * \alpha)(x) ,
$$

where the convolution product is taken relative to the right Haar measure $ \mu $ and where one makes use of the fact that $ \dot{\alpha} = \alpha $ (\S 4, No. 4, formula (11)). We know (Ch. VII, §2, No. 1, Prop. 2) that the mapping $ f \mapsto f_\alpha $ of $ \mathcal{K}_+(G) $ into $ \mathcal{K}_+(Q_\alpha) $ is *surjective*; therefore, by (2),

$$
\| \mu_\alpha \| = \sup_{f \in \mathcal{K}_+(G), f \neq 0} \mu_\alpha(f_\alpha) / \| f_\alpha \| = \sup_{f \in \mathcal{K}_+(G), f \neq 0} \mu(f) / \| f_\alpha \|,
$$

where one has set

$$
\|f_\alpha\| = \sup_{\dot{x} \in Q_\alpha} |f_\alpha(\dot{x})| = \sup_{x \in G} |(f * \alpha)(x)| .
$$

To establish the proposition, it will suffice to show that, given $ f \in \mathcal{H}_+(G) $, the mapping $ \alpha \mapsto \|f_\alpha\| $ is vaguely continuous. Now, let K be the support of $ f $; the function $ f * \alpha $ has its support contained in $ KH_\alpha $ and is invariant on the right under $ H_\alpha $; consequently

$$
\|f_\alpha\| = \sup_{x \in K} |(f * \alpha)(x)| .
$$

The conclusion therefore follows from the fact that the mapping $ \alpha \mapsto f * \alpha $ of $ \mathcal{M}_+(G) $ equipped with the vague topology, into $ \mathcal{C}(G) $ equipped with the topology of compact convergence, is continuous (\S 4, No. 2, Remark 1).

Recall that if, for a measure $ \alpha \in \Gamma^0 $, $ \|\mu_\alpha\| $ is finite, then G is necessarily unimodular (Ch. VII, §2, No. 6, Cor. 3 of Th. 3).

#### Proposition 5 {#int-viii-s5-prop-5 .statement}

*Let g be a $ \mu $-integrable positive numerical function and let $ \Gamma^0(g) $ be the set of measures $ \alpha \in \Gamma^0 $ such that $ \int^* g(xs)\, d\alpha(s) \geq 1 $ for all $ x \in G $. Then the mapping $ \alpha \mapsto \|\mu_\alpha\| $ of $ \Gamma^0(g) $ into $ \overline{\mathbf{R}} $ is vaguely continuous.*

For every measure $ \alpha \in \Gamma^0(G) $, recall (Ch. VII, §2, No. 3, Prop. 5) that the function

$$
g_\alpha(\dot{x}) = \int_{H_\alpha} g(xs)\, d\alpha(s)
$$

is defined $ \mu_\alpha $-almost everywhere on $ Q_\alpha $, is $ \mu_\alpha $-integrable, and

$$
\int_G g(x)\, d\mu(x) = \int_{Q_\alpha} g_\alpha(\dot{x})\, d\mu_\alpha(\dot{x}) .
$$

In view of Prop. 4, it suffices to prove that, in $ \Gamma^0(g) $, $ \alpha \mapsto \|\mu_\alpha\| $ is *upper* semi-continuous. Fix a measure $ \alpha \in \Gamma^0(g) $, and let K be a compact subset of G. There exists on $ Q_\alpha $ a continuous function with compact support, taking its values in $[0, 1]$, equal to 1 on the compact set $ \pi_\alpha(K) $; since the mapping $ f \mapsto f_\alpha $ of $ \mathcal{H}_+(G) $ into $ \mathcal{H}_+(Q_\alpha) $ is surjective (Ch. VII, §2, No. 1, Prop. 2), one sees that there exists a function $ f \in \mathcal{H}_+(G) $ such that

$$
(f * \alpha)(x) = \int_G f(xs)\, d\alpha(s) \left\{ \begin{array}{ll}
\leq 1 & \text{for all } x \in G \\
= 1 & \text{for all } x \in K .
\end{array} \right.
$$

Since $ \beta \mapsto f * \beta $ is a continuous mapping of $ \mathcal{M}_+(G) $, equipped with the vague topology, into $ \mathcal{C}(G) $ equipped with the topology of compact convergence (\S 4, No. 2, Remark 1), one sees that for every $ \varepsilon > 0 $, the set $ U_\varepsilon $ of $ \beta \in \Gamma^0(G) $ such that
$$
f_\beta(\dot{x}) = \int_G f(xs)\, d\beta(s) > 1 - \varepsilon \quad \text{for all } x \in K
$$
is an open neighborhood of $ \alpha $ in $ \Gamma^0(g) $; for every $ \beta \in U_\varepsilon $, we then have, by virtue of the formula (2),
$$
(5) \quad \| \mu_\alpha \| \geq \int_G f(x)\, d\mu(x) = \int_{Q_\beta} f_\beta(\dot{x})\, d\mu_\beta(\dot{x}) \geq (1 - \varepsilon) \mu_\beta(\pi_\beta(K)).
$$
Given a number $ \varepsilon > 0 $, let us choose a function $ h \in \mathcal{K}_+(G) $ such that $ \int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon $, and let us take $ K = \mathrm{Supp}(h) $ in the foregoing. For every $ \beta \in \Gamma^0(g) $, by hypothesis $ g_\beta(\dot{x}) \geq 1 $ almost everywhere (for $ \mu_\beta $) in $ Q_\beta $, therefore
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{Q_\beta - \pi_\beta(K)} g_\beta(\dot{x})\, d\mu_\beta(\dot{x}) = \int_{G - KH_\beta} g(x)\, d\mu(x)
$$
by virtue of (4); since $ h $ is zero outside $ K $, and $ a fortiori $ outside $ KH_\beta $, it follows that
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{G - KH_\beta} |g(x) - h(x)|\, d\mu(x) \\
\leq \int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon;
$$
combining this result with (5), one sees that
$$
\| \mu_\beta \| \leq \varepsilon + \| \mu_\alpha \|/(1 - \varepsilon)
$$
when $ \beta \in U_\varepsilon $, which completes the proof.

#### Corollary 1 {#int-viii-s5-prop-5-cor-1 .statement}

— Let $ K $ be a compact subset of $ G $, $ V $ a symmetric compact neighborhood of $ e $ in $ G $, $ c $ a real number $ > 0 $. The restriction of the mapping $ \alpha \mapsto \| \mu_\alpha \| $ to the set of $ \alpha \in \Gamma^0 $ such that $ G = KH_\alpha $ and $ \alpha(V) \geq c $ is vaguely continuous.

For, let $ g \in \mathcal{K}_+(G) $ be a function such that $ g(x) \geq 1/c $ for $ x \in KV $. For every $ x \in K $,
$$
\int g(xs)\, d\alpha(s) \geq \int_V g(xs)\, d\alpha(s) \geq 1
$$

for $ \alpha $ satisfying the conditions of the statement; since, moreover, $ \pi_\alpha(K) = Q_\alpha $, one has $ \alpha \in \Gamma^0(g) $, whence the corollary.

#### Corollary 2 {#int-viii-s5-prop-5-cor-2 .statement}

*Let A be a $ \mu $-integrable subset of G. The restriction of the mapping $ \alpha \mapsto \| \mu_\alpha \| $ to the set $ N_A $ of normalized Haar measures of the discrete subgroups H of G such that $ G = AH $, is vaguely continuous.*

For $ a \in A $ and $ \alpha \in N_A $,

$$
\int \varphi_A(as)\ d\alpha(s) \geq \varphi_A(a) = 1,
$$

and since $ \pi_\alpha(A) = Q_\alpha $, one has $ N_A \subset \Gamma^0(\varphi_A) $, and the corollary therefore follows from Prop. 5.

### 3. The space of closed subgroups of G

Let us denote by $ \Sigma $ the set of *closed subgroups* of G; if one associates to each measure $ \alpha \in \Gamma $ the subgroup $ H_\alpha $ that is the support of $ \alpha $, one obtains a mapping (called canonical) of $ \Gamma $ into $ \Sigma $, which is clearly surjective and permits canonically identifying $ \Sigma $ with the set of orbits of the group of homotheties in $ \Gamma $ with ratio $ > 0 $. The set $ \Sigma $, equipped with the quotient topology of the vague topology on $ \Gamma $, is called *the space of closed subgroups* of G.

#### Theorem 1 {#int-viii-s5-thm-1 .statement}

*Let G be a locally compact group. The space $ \Sigma $ of closed subgroups of G is compact. Moreover, one has the following properties:*

(i) *The set $ \Sigma^0 $ of unimodular closed subgroups of G is closed in $ \Sigma $ (hence is compact).*

(ii) *If G is generated by a compact neighborhood of e, then the set $ \Sigma_c^0 $ of unimodular closed subgroups H of G such that the quotient space $ G/H $ is compact, is open in $ \Sigma^0 $ (hence is locally compact).*

(iii) *For every relatively compact open neighborhood U of e in G, the set $ D_U $ of discrete subgroups H of G such that $ H \cap U = \{e\} $ is closed in $ \Sigma^0 $ (hence is compact).*

It follows from Prop. 3 of No. 1 that $ \Sigma $ is homeomorphic to $ \Gamma_\varphi $, hence is compact by Prop. 2 of No. 1. Moreover, it was noted at the beginning of No. 2 that the set $ \Gamma^0 $ of measures $ \alpha \in \Gamma $ such that $ H_\alpha $ is unimodular is closed in $ \Gamma $; since $ \Gamma^0 $ is stable under the homotheties with ratio $ > 0 $, the image $ \Sigma^0 $ of $ \Gamma^0 $ in $ \Sigma $ is a closed subset of $ \Sigma $, which proves (i).

Property (ii) will be a consequence of the following proposition:

#### Proposition 6 {#int-viii-s5-prop-6 .statement}

*Suppose that the locally compact group G is generated by a compact neighborhood of e. Then the set $ \Gamma_c^0 $ of measures $ \alpha \in \Gamma^0 $* such that $ G/H_\alpha $ is compact is open in $ \Gamma^0 $, and the restriction to $ \Gamma_c^0 $ of the mapping $ \alpha \mapsto \| \mu_\alpha \| $ is vaguely continuous.

With the notations of Prop. 5 of No. 2, we have, for $ g \in \mathcal{K}_+(G) $,

$$
\Gamma^0(g) \subset \Gamma_c^0.
$$

For, if K is the support of $ g $, the relation $ \int g(xs)\, d\alpha(s) \geq 1 $ for all $ x \in G $ implies $ KH_\alpha = G $, the integral obviously being zero on the complement of $ KH_\alpha $, therefore $ G/H_\alpha = \pi_\alpha(K) $ is compact. Given a measure $ \alpha \in \Gamma_c^0 $, it will therefore suffice to define a function $ g \in \mathcal{K}_+(G) $ such that $ \Gamma^0(g) $ is a neighborhood of $ \alpha $ in $ \Gamma^0 $. Since $ G/H_\alpha $ is compact and the canonical mapping $ f \mapsto f_\alpha $ of $ \mathcal{K}_+(G) $ into $ \mathcal{K}_+(G/H_\alpha) $ is surjective (Ch. VII, §2, No. 2), there exists a function $ g \in \mathcal{K}_+(G) $ such that $ \int g(xs)\, d\alpha(s) = 2 $ for *every* $ x \in G $. Let K be the (compact) support of $ g $, L a symmetric compact neighborhood of e in G that generates G; the mapping $ \beta \mapsto g * \beta $ of $ \mathcal{M}_+(G) $ into $ \mathcal{C}(G) $ being vaguely continuous (\S4, No. 2, *Remark* 1), there exists a neighborhood W of $ \alpha $ in $ \Gamma^0 $ such that

$$
(g * \beta)(x) = \int g(xs)\, d\beta(s) \geq 1
$$

for all $ \beta \in W $ and $ x \in LK $. The first member of (7) being equal to zero outside $ KH_\beta $, the relation $ \beta \in W $ implies

$$
LK \subset KH_\beta,
$$

from which one deduces, by induction on $ n $, that $ L^n K \subset KH_\beta $ for every integer $ n > 0 $; since L generates G, we therefore have $ G = KH_\beta $ for every measure $ \beta \in W $, which proves that $ W \subset \Gamma_c^0 $. On the other hand, the first member of (7) being invariant on the right under $ H_\beta $, the inequality (7) is also valid for $ x \in LKH_\beta = G $; therefore $ W \subset \Gamma^0(g) $, which proves the proposition.

Finally, (iii) will be a consequence of the following proposition:

#### Proposition 7 {#int-viii-s5-prop-7 .statement}

*Let $ N \subset \Gamma^0 $ be the subspace of normalized Haar measures on the discrete subgroups of G, and for every relatively compact open neighborhood U of e in G, let $ N_U $ be the subset of N formed by the $ \alpha $ such that $ H_\alpha \cap U = \{e\} $. Then:
a) $ N_U $ is compact.
b) The interiors of the sets $ N_U $ in N form a covering of N, as U runs over the set of relatively compact open neighborhoods of e in G.
c) For a subset M of N to be relatively compact in N, it is necessary and sufficient that there exist a relatively compact open neighborhood U of e in G such that $ M \subset N_U $.*

Since $ D_U $ is the image of $ N_U $ under the canonical continuous mapping $ \Gamma \to \Sigma $, the assertion (iii) of Th. 1 will result at once from Prop. 7 a).

To prove Prop. 7, we observe that $ N_U $ can be defined as the subset of $ \Gamma^0 $ formed by the $ \alpha $ such that both

$$
\alpha(\{e\}) \geq 1 \quad \text{and} \quad \alpha(U) \leq 1.
$$

Now, if $ A $ is compact (resp. open and relatively compact) in $ G $, then the mapping $ \alpha \mapsto \alpha(A) $ of $ \mathcal{M}_+(G) $ into $ \mathbf{R} $ is upper (resp. lower) semi-continuous for the vague topology (Ch. IV, §4, No. 4, Cor. 3 of Prop. 5 and loc. cit., §1, No. 1, Prop. 4); we thus see that $ N_U $ is a closed subset of $ \Gamma^0 $. Moreover, let $ \varphi \in \mathcal{K}_+(G) $ be a function such that $ \varphi(e) = 1 $ and $ \varphi(x) = 0 $ on $ G - U $; it is clear that $ \int \varphi(x) d\alpha(x) = 1 $ for all $ \alpha \in N_U $; Prop. 2 of No. 1 therefore shows that $ N_U $ is a compact set, which proves a). On the other hand let $ V $ be a relatively compact open neighborhood of $ e $ in $ G $ such that $ \overline{V} \subset U $, and let $ \varphi \in \mathcal{K}_+(G) $, with support contained in $ U $ and such that $ \varphi(x) = 1 $ on $ V $. Then $ \alpha(\varphi) = 1 $ for $ \alpha \in N_U $, therefore there exists a neighborhood $ W $ of $ \alpha $ in $ N $ such that $ \beta(\varphi) < 2 $ for $ \beta \in W $; it is then clear that $ W \subset N_V $, therefore $ N_V $ is a neighborhood of $ N_U $. Since the $ N_U $ cover $ N $, this proves b). Finally, every compact subset $ M $ of $ N $ is contained in a finite union of sets $ N_{U_i} $ ($ 1 \leq i \leq n $), and since $ \bigcup_i N_{U_i} \subset N_U $, where $ U = \bigcap_i U_i $, this proves c).

#### Corollary {#int-viii-s5-n3-cor-1 .statement}

— *The subspace* $ N $ *of* $ \Gamma^0 $ *is locally compact*.

### 4. The case of groups without arbitrarily small finite subgroups

#### Theorem 2 {#int-viii-s5-thm-2 .statement}

— *Let* $ G $ *be a locally compact group satisfying the following condition*:
(L) *There exists a neighborhood of* $ e $ *in* $ G $ *that contains no finite subgroup of* $ G $ *not reduced to* $ e $.
*The following properties then hold*:
(i) *The set* $ D $ *of discrete subgroups of* $ G $ *is locally closed in* $ \Sigma $ *(which is equivalent to saying that it is locally compact)*.
(ii) *For a closed subset* $ A $ *of* $ D $ *to be compact, it is necessary and sufficient that there exist a neighborhood* $ U $ *of* $ e $ *in* $ G $ *such that* $ H \cap U = \{e\} $ *for every subgroup* $ H \in A $.
(iii) *If in addition* $ G $ *is generated by a compact neighborhood of* $ e $, *then the set* $ D_c $ *of discrete subgroups* $ H $ *of* $ G $ *such that* $ G/H $ *is compact is locally closed in* $ \Sigma $ *(hence is locally compact)*.

We have $ D_c = D \cap \Sigma_c^0 $, therefore (iii) is a consequence of (i), and Th. 1 (ii) of No. 3.

With the notations of No. 3, Prop. 7, it suffices, for proving (i) and (ii), to prove that:

#### Proposition 8 {#int-viii-s5-prop-8 .statement}

*The canonical bijection of N onto D is a homeomorphism.*

Now, if $ \Gamma_d $ is the set of Haar measures on the discrete subgroups of $ G $, then $ D $ is canonically homeomorphic to the space of orbits of the group of homotheties in $ \Gamma_d $ with ratio $ > 0 $ (GT, I, §5, No. 2, Prop. 4). It therefore suffices to prove that the canonical mapping $ \alpha \mapsto (\alpha(\{e\}), \alpha/\alpha(\{e\})) $ of $ \Gamma_d $ onto $ \mathbf{R}_+^* \times \mathbf{N} $ is a *homeomorphism*, which will result from the following lemma:

#### Lemma 4 {#int-viii-s5-lem-4 .statement}

*If the group G satisfies the condition (L), the mapping $ \alpha \mapsto \alpha(\{e\}) $ of $ \Gamma_d $ into $ \mathbf{R}_+^* $ is vaguely continuous.*

Let us consider a measure $ \alpha \in \Gamma_d $; let $ V_0 $ be a relatively compact open neighborhood of $ e $ in $ G $ such that $ H_\alpha \cap V_0 = \{e\} $ and such that there exists no finite subgroup of $ G $ contained in $ V_0 $ and not reduced to $ e $. Let $ V $ be a symmetric compact neighborhood of $ e $ such that $ V^3 \subset V_0 $, and let $ U $ be a symmetric neighborhood of $ e $ such that $ U^2 \subset V $. Let $ \varphi $ (resp. $ \psi $) be a function in $ \mathcal{H}_+(G) $, with values in $[0, 1]$, equal to 1 on $ V^3 $ (resp. at the point $ e $) and with support contained in $ V_0 $ (resp. in $ U $). The set of measures $ \beta \in \Gamma_d $ such that $ |\beta(\varphi) - \alpha(\varphi)| \leq \varepsilon $ and $ |\beta(\psi) - \alpha(\psi)| \leq \varepsilon $ is a neighborhood $ W $ of $ \alpha $. We propose to show that, provided $ \varepsilon $ is taken to be sufficiently small, $ H_\beta \cap V = \{e\} $ *for every* $ \beta \in W $; it will then follow that $ \beta(\psi) = \beta(\{e\}) $, hence that $ |\beta(\{e\}) - \alpha(\{e\})| \leq \varepsilon $, which will prove the lemma.

It will suffice to show that, for $ \beta \in W $,

$$
(V^2 - V) \cap H_\beta = \varnothing.
$$

For, suppose that this point is established: then, for $ x $ and $ y $ in $ V \cap H_\beta $, one has $ xy^{-1} \in V^2 \cap H_\beta $; but, by virtue of (8), this implies $ xy^{-1} \in V \cap H_\beta $; in other words, $ V \cap H_\beta $ is a *subgroup* of $ G $, which is obviously discrete and compact, hence finite; but then, by the choice of $ V_0 $, this implies that indeed $ V \cap H_\beta = \{e\} $.

Let us argue by contradiction and so assume that there exists a point $ z $ of $ V^2 - V $ that belongs to $ H_\beta $; by the choice of $ U $ and $ V $, we have $ \psi(sz^{-1}) + \psi(s) \leq \varphi(s) $ in $ G $, the relation $ z \notin U^2 $ implying $ Uz \cap U = \varnothing $. Since

$$
\int \psi(sz^{-1})\, d\beta(s) = \int \psi(s)\, d\beta(s),
$$

it follows that $ 2\beta(\psi) \leq \beta(\varphi) \leq \alpha(\varphi) + \varepsilon $; but we also have
$$
\beta(\psi) \geq \alpha(\psi) - \varepsilon,
$$
and by construction $ \alpha(\varphi) = \alpha(\psi) = \alpha(\{e\}) $. We thus arrive at a contradiction by taking $ \varepsilon < \alpha(\{e\})/3 $. Q.E.D.

In graphic terms, a group $ G $ satisfying the condition (L) is said to *not have arbitrarily small finite subgroups.* It can be shown that every Lie group satisfies the condition (L); but this condition is not characteristic of Lie groups; for example, the multiplicative group of $ p $-adic integers congruent to 1 mod $ p $ satisfies (L).*

### 5. The case of abelian groups

Let $ G $ be a locally compact group, $ N \subset \Gamma^0 $ the subspace of normalized Haar measures on the discrete subgroups of $ G $, and $ N_c $ the subset of $ N $ corresponding to the discrete subgroups $ H $ of $ G $ such that $ G/H $ is *compact*; thus $ N_c = N \cap \Gamma_c^0 $ in the notations of No. 3, Prop. 6; and if the group $ G $ is generated by a compact neighborhood of $ e $, it follows from No. 3, Prop. 6 that $ N_c $ is *open* in $ N $ (hence is *locally compact* by No. 3, Cor. of Prop. 7) and that the restriction to $ N_c $ of the mapping $ \alpha \mapsto \| \mu_\alpha \| $ is *vaguely continuous*.

#### Proposition 9 {#int-viii-s5-prop-9 .statement}

*Let $ G $ be a locally compact abelian group, generated by a compact neighborhood of $ e $. For a subset $ A $ of $ N_c $ to be relatively compact in $ N_c $, it is necessary and sufficient that it satisfy the following two conditions:*

(i) *There exists an open neighborhood $ U $ of $ e $ in $ G $ such that $ H_\alpha \cap U = \{e\} $ for all $ \alpha \in A $.*

(ii) *There exists a constant $ k $ such that $ \mu_\alpha(G/H_\alpha) \leq k $ for all $ \alpha \in A $.*

If $ A \subset N_c $ is relatively compact in $ N_c $, it is *a fortiori* so in $ N $, and the necessity of the conditions (i) and (ii) therefore follows from No. 3, Props. 6 and 7 (without assuming $ G $ to be abelian). Conversely, suppose that $ A \subset N_c $ satisfies these conditions; if $ \overline{A} $ is the closure of $ A $ *in* $ N $, then $ \overline{A} $ is compact by virtue of No. 3, Prop. 7; moreover, since $ \alpha \mapsto \| \mu_\alpha \| $ is lower semi-continuous on $ \Gamma^0 $ for the vague topology (No. 2, Prop. 4), the condition (ii) implies that one also has $ \| \mu_\alpha \| \leq k $ for all $ \alpha \in \overline{A} $. Now, since $ G $ is abelian, $ \mu_\alpha = \mu/\alpha $ is a Haar measure on the group $ G/H_\alpha $, and $ G/H_\alpha $ is therefore compact for every $ \alpha \in \overline{A} $ (Ch. VII, §1, No. 2, Prop. 2). This means that $ \overline{A} \subset N_c $, thus $ A $ is relatively compact in $ N_c $.

#### Corollary {#int-viii-s5-n5-cor-1 .statement}

*Let $ G $ be a locally compact abelian group, generated by a compact neighborhood of $ e $ and satisfying the condition (L) of No. 4.*

Let $ D_c $ be the set of discrete subgroups $ H $ of $ G $ such that $ G/H $ is compact, and, for every $ H \in D_c $, let $ v(H) $ be the total mass $ \mu_\alpha(G/H) $, where $ \mu_\alpha $ is the quotient measure of $ \mu $ by the normalized Haar measure $ \alpha $ of $ H $. For a subset $ A $ of the space $ D_c $ to be relatively compact in $ D_c $, it is necessary and sufficient that it satisfy the following two conditions:

(i) There exists an open neighborhood $ U $ of $ e $ in $ G $ such that $ H \cap U = \{e\} $ for all $ H \in A $.

(ii) There exists a constant $ k $ such that $ v(H) \leq k $ for all $ H \in A $.

Taking into account Prop. 9, this follows at once from the fact that $ D_c $ is the image of $ N_c $ under the canonical bijection of $ N $ onto $ D $, and the fact that, under the hypotheses made, this bijection is a homeomorphism (No. 4, Prop. 8).

#### Example {#int-viii-s5-n5-exa-1 .statement}

Let us take $ G = \mathbf{R}^n $ and for $ \mu $ the Lebesgue measure; all of the hypotheses of the Cor. of Prop. 9 are satisfied. The discrete subgroups $ H $ of $ G $ such that $ G/H $ is compact are none other than the discrete subgroups of *rank* $ n $ (GT, VII, §1, No. 1, Th. 1); such a subgroup $ H $ is generated by a basis $ (a_i)_{1 \leq i \leq n} $ of $ \mathbf{R}^n $, and

$$
v(H) = |\det(a_1, \ldots, a_n)|
$$

(the determinant being taken with respect to the canonical basis of $ \mathbf{R}^n $) (Ch. VII, §2, No. 10, Th. 4). The space $ D_c $ can be interpreted here in the following way: every subgroup $ H \in D_c $ is the transform $ g \cdot \mathbf{Z}^n $ of the subgroup $ \mathbf{Z}^n $ by an element $ g \in \mathbf{GL}(n, \mathbf{R}) $, and the subgroup of $ \mathbf{GL}(n, \mathbf{R}) $ leaving $ \mathbf{Z}^n $ stable may be identified with $ \mathbf{GL}(n, \mathbf{Z}) $. Consequently $ D_c $ may be canonically identified, as a (non-topological) homogeneous space, with $ \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}) $. On the other hand, $ \mathbf{GL}(n, \mathbf{R}) $ operates continuously in $ \mathbf{R}^n $, hence also in $ \mathcal{M}_+(\mathbf{R}^n) $ for the vague topology (§3, No. 3, Prop. 13), hence in the subspace $ N_c $ of $ \mathcal{M}_+(\mathbf{R}^n) $; moreover, the canonical homeomorphism (No. 4, Prop. 8) of $ N_c $ onto $ D_c $ is compatible with the laws of operation of $ \mathbf{GL}(n, \mathbf{R}) $. Since $ \mathbf{GL}(n, \mathbf{R}) $ is countable at infinity and $ D_c $ is locally compact, the bijection of $ \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}) $ onto $ D_c $ defined above is a *homeomorphism* (Ch. VII, App. I, Lemma 2). The Cor. of Prop. 9 therefore gives a criterion for compactness in the homogeneous space $ \mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z}) $.

### 6. Another interpretation of the topology of the space of closed subgroups

Let $ \mathfrak{F} $ be the set of closed subsets of $ G $; one defines a *Hausdorff uniform structure* on $ \mathfrak{F} $ in the following way: for every compact subset $ K $ of $ G $ and every neighborhood $ V $ of $ e $ in $ G $, let $ P(K, V) $ be the set of pairs $ (X, Y) $ of elements of $ \mathcal{F} $ such that both

$$
(9) \quad X \cap K \subset VY \quad \text{and} \quad Y \cap K \subset VX.
$$

Let us show that the set of $ P(K, V) $ is a fundamental system of entourages for a Hausdorff uniform structure $ \mathcal{U} $ on $ \mathcal{F} $. The axioms $ (U'_I) $ and $ (U'_{II}) $ of GT, II, §1, No. 1 are obviously satisfied; moreover, the relations $ K \subset K' $ and $ V' \subset V $ imply $ P(K', V') \subset P(K, V) $; to verify $ (U'_{III}) $, one can therefore limit oneself to the case that $ V $ is a symmetric compact neighborhood of $ e $, so that $ VK $ is compact. Suppose that $ (X, Y) \in P(VK, V) $ and $ (Y, Z) \in P(VK, V) $; then $ X \cap K \subset X \cap VK \subset VY $, and if $ y \in Y $ is such that $ vy \in K $ for some $ v \in V $, then necessarily $ y \in VK $, therefore

$$
X \cap K \subset V(Y \cap VK);
$$

on the other hand, $ Y \cap VK \subset VZ $, whence $ X \cap K \subset V^2Z $, and one shows similarly that $ Z \cap K \subset V^2X $, which proves $ (U'_{III}) $. Finally, if $ X, Y $ are two distinct elements of $ \mathcal{F} $, there exists for example a point $ a \in X $ such that $ a \notin Y $, hence a symmetric compact neighborhood $ V $ of $ e $ such that $ Va \cap Y = \varnothing $, that is, $ a \notin VY $; *a fortiori* $ (X, Y) \notin P(Va, V) $, which completes the proof of our assertion.

This established, let us consider on the set $ \Sigma $ of closed subgroups of $ G $ the topology $ \mathcal{T} $ induced by the topology of the uniform space $ \mathcal{F} $ just defined. We shall see that this topology is *identical to the topology defined in No. 3*. It will suffice to prove that the mapping $ \alpha \mapsto H_\alpha $ of $ \Gamma $ into $ \Sigma $ is *continuous* when $ \Sigma $ is equipped with the topology $ \mathcal{T} $: for, the same will then be true of the restriction of this mapping to $ \Gamma_\varphi $ (with notations as in No. 1, Prop. 2), which is bijective; but since $ \Gamma_\varphi $ is compact and the topology $ \mathcal{T} $ is separated, the mapping $ \alpha \mapsto H_\alpha $ of $ \Gamma_\varphi $ into $ \Sigma $ will then be a homeomorphism.

Thus let $ \alpha_0 $ be a point of $ \Gamma $ and let $ \Phi $ be a filter on $ \Gamma $ that converges to $ \alpha_0 $; we are to show that, with respect to $ \Phi $, $ H_\alpha $ tends to $ H_{\alpha_0} $ for the topology $ \mathcal{T} $. Let $ K $ be a compact subset of $ G $, $ V $ a symmetric compact neighborhood of $ e $ in $ G $; for every $ x \in H_{\alpha_0} \cap K $, there exists a set $ M(x) \in \Phi $ such that for every $ \alpha \in M(x) $, one has $ Vx \cap H_\alpha \neq \varnothing $ (No. 1, Lemma 2), whence $ Vx \subset V^2H_\alpha $; on covering $ H_{\alpha_0} \cap K $ by a finite number of sets $ Vx_i $, one sees that if $ M = \bigcap_i M(x_i) $, then $ H_{\alpha_0} \cap K \subset V^2H_\alpha $ for every $ \alpha \in M $.

Conversely, suppose that there existed an open neighborhood $ U $ of $ e $ in $ G $ such that, for every set $ L \in \Phi $, there is at least one $ \alpha \in L $ for which $ H_\alpha \cap K \not\subset UH_{\alpha_0} $; if $ \omega(L) $ is the set of $ \alpha \in L $ having this property, the $ \omega(L) $ would form a base of a filter $ \Phi' $ on $ \Gamma $ finer than $ \Phi $, and, for every $ \alpha $ belonging to the union $ E $ of the $ \omega(L) $ for $ L \in \Phi $, there would exist a t_\alpha \in H_\alpha \cap K \text{ not belonging to } UH_{\alpha_0}; \text{ for } \alpha \notin E, \text{ take for } t_\alpha \text{ any point of } H_\alpha. \text{ Since } K \cap C(UH_{\alpha_0}) \text{ is compact, there would exist a cluster point } s \text{ of } \alpha \mapsto t_\alpha \text{ with respect to } \Phi', \text{ belonging to } K \cap C(UH_{\alpha_0}); \text{ but since } \Phi' \text{ converges to } \alpha_0 \text{ in } \Gamma, \text{ this contradicts Lemma 3 of No. 1.}

Exercises

### Exercises {#int-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
