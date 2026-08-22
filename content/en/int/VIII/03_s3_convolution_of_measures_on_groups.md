---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 3
section_title: Convolution of measures on groups
lang: en
source: int-vii-ix
book_pages: INT VIII.18-INT VIII.24, INT VIII.61-INT VIII.65
pdf_pages: 0118-0124, 0161-0165
extraction: ocr
subsections:
    - "no": 1
      title: Algebras of measures
      page: 18
      pdf_page: 118
    - "no": 2
      title: The case of a group operating on a space
      page: 21
      pdf_page: 121
    - "no": 3
      title: Convolution and linear representations
      page: 22
      pdf_page: 122
statements: 16
exercises: 13
content_sha256: 770c50427b33153ec02eedab6fb35e27870c859fef0e164830e39a285e132540
---

## § 3. CONVOLUTION OF MEASURES ON GROUPS

### 1. Algebras of measures

Let G be a locally compact group. It will be understood, once and for all, that the measures $ \mu_1, \ldots, \mu_n $ on G are said to be convolvable if they are so for the mapping

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \cdots x_n;
$$

and it is by means of this mapping that the convolution product $ *_{i} \mu_i $ will always be taken. If $ s \in G, t \in G $, then

(1)
$$
\varepsilon_s * \varepsilon_t = \varepsilon_{st}.
$$

If $ s \in G $ and $ \mu \in \mathcal{M}(G) $, then

(2)
$$
\varepsilon_s * \mu = \gamma(s) \mu
$$
(3)
$$
\mu * \varepsilon_s = \delta(s^{-1}) \mu
$$

by §1, No. 1, Example 3. If G is abelian, to say that $ \mu_1 $ and $ \mu_2 $ are convolvable is equivalent to saying that $ \mu_2 $ and $ \mu_1 $ are convolvable, and one then has $ \mu_1 * \mu_2 = \mu_2 * \mu_1 $. When G is not abelian, it can happen that $ \mu_1 $ and $ \mu_2 $ are convolvable, without $ \mu_2 $ and $ \mu_1 $ being so (Exer. 12).

#### Proposition 1 {#int-viii-s3-prop-1 .statement}

— Let G be a locally compact group, $ \lambda, \mu, \nu $ measures $ \neq 0 $ on G.

(i) If $ \lambda, \mu, \nu $ are convolvable, then so are $ \lambda $ and $ \mu $, $ |\lambda| * |\mu| $ and $ \nu $, $ \mu $ and $ \nu $, $ \lambda $ and $ |\mu| * |\nu| $, and one has

$$
\lambda * \mu * \nu = (\lambda * \mu) * \nu = \lambda * (\mu * \nu).
$$

(ii) If $ \lambda $ and $ \mu $ are convolvable, as well as $ |\lambda| * |\mu| $ and $ \nu $, then $ \lambda, \mu, \nu $ are convolvable. Similarly if $ \mu $ and $ \nu $ are convolvable, as well as $ \lambda $ and $ |\mu| * |\nu| $.

This follows from Prop. 1 of §1, No. 2.

There can exist measures $ \lambda, \mu, \nu $ on G such that the convolution products $ \lambda * \mu $, $ (\lambda * \mu) * \nu $, $ \mu * \nu $, $ \lambda * (\mu * \nu) $ are all defined, and yet $ (\lambda * \mu) * \nu \neq \lambda * (\mu * \nu) $ (cf. Exer. 4).

Let $ \rho $ be a lower semi-continuous finite function $ > 0 $ on $ G $ such that $ \rho(st) \leq \rho(s)\rho(t) $ for all $ s, t $ in $ G $. We denote by $ \mathcal{M}^\rho(G) $ the vector space of measures $ \lambda $ on $ G $ such that $ \rho $ is $ \lambda $-integrable, and by $ \| \lambda \|_\rho $ (or simply $ \| \lambda \| $) the norm $ \int_G \rho(s) d|\lambda|(s) $ on this space. When $ \rho = 1 $, one recovers the set $ \mathcal{M}^1(G) $ of bounded measures on $ G $.

#### Proposition 2 {#int-viii-s3-prop-2 .statement}

(i) *Any two elements of $ \mathcal{M}^\rho(G) $ are convolvable.*
(ii) *For convolution, and for the norm $ \| \lambda \| $, $ \mathcal{M}^\rho(G) $ is a complete normed algebra, admitting $ \varepsilon_e $ as unity element.*
(iii) $ \mathcal{C}'(G) $ *is a subalgebra of $ \mathcal{M}^\rho(G) $*.

Let $ \lambda, \mu $ be in $ \mathcal{M}^\rho(G) $, and let us show that $ \lambda $ and $ \mu $ are convolvable. Let $ f \in \mathcal{K}_+(G) $. Since $ \rho $ is $ > 0 $ and lower semi-continuous, there exists a constant $ k > 0 $ such that $ f \leq k\rho $. Then

$$
\int^* f(st) d|\lambda|(s) d|\mu|(t) \leq k \int^* \rho(st) d|\lambda|(s) d|\mu|(t)
$$
$$
\leq k \int^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= k \left( \int^* \rho(s) d|\lambda|(s) \right) \left( \int^* \rho(t) d|\mu|(t) \right)
$$

(Ch. V, §8, No. 3, Cor. 1 of Prop. 8). Therefore $ (s,t) \mapsto f(st) $ is $ (\lambda \otimes \mu) $-integrable, so that $ \lambda $ and $ \mu $ are convolvable. On the other hand, using Ch. V (§1, Prop. 4, §6, Prop. 2, §8, Cor. 1 of Prop. 8) and the fact that $ (s,t) \mapsto \rho(s)\rho(t) $ is lower semi-continuous in $ G \times G $, one has

$$
\int_G^* \rho(s) d|\lambda * \mu|(s) = \int_G^* \rho(s) d|\lambda * \mu|(s)
$$
$$
\leq \int_{G \times G}^* \rho(st) d|\lambda|(s) d|\mu|(t) \leq \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t) = \| \lambda \| \cdot \| \mu \|.
$$

One sees that $ \lambda * \mu \in \mathcal{M}^\rho(G) $ and that $ \| \lambda * \mu \| \leq \| \lambda \| \cdot \| \mu \| $. In view of Prop. 1, $ \mathcal{M}^\rho(G) $ is an algebra. The mapping $ \lambda \mapsto \rho \cdot \lambda $ is an isometric linear mapping $ \theta $ of $ \mathcal{M}^\rho(G) $ into $ \mathcal{M}^1(G) $; if $ \mu \in \mathcal{M}^1(G) $ then $ 1/\rho $, which is locally bounded and upper semi-continuous, is locally $ \mu $-integrable, and $ \rho $ is $ (1/\rho) \cdot \mu $-integrable, thus $ (1/\rho) \cdot \mu \in \mathcal{M}^\rho(G) $; this proves that $ \theta $ is surjective; therefore $ \mathcal{M}^\rho(G) $ is a complete normed algebra. Finally, it is clear that $ \varepsilon_e $ is a unity element for $ \mathcal{M}^\rho(G) $ and that $ \mathcal{C}'(G) $ is a subalgebra of $ \mathcal{M}^\rho(G) $ (§1, No. 4, Cor. of Prop. 5).

If $ \rho = 1 $, Prop. 2, (i) and (ii) also follow from §1, Prop. 2.

#### Proposition 3 {#int-viii-s3-prop-3 .statement}

*Let $ \mu_1, \ldots, \mu_n $ be measures on G. If all of the $ \mu_i $, except at most one, have compact support, then the $ \mu_i $ are convolvable.*

For, let $ S_i $ be the support of $ \mu_i $, and suppose that $ S_i $ is compact for $ i \neq i_0 $. Let K be a compact subset of G. The set of $ (x_1, \ldots, x_n) \in \prod_i S_i $ such that $ x_1 x_2 \cdots x_n \in K $ is compact, because the conditions $ x_i \in S_i $ for all $ i $, $ x_1 x_2 \cdots x_n \in K $ imply

$$
x_{i_0} \in S_{i_0-1}^{-1} \cdots S_1^{-1} K S_n^{-1} \cdots S_{i_0+1}^{-1} .
$$

Therefore the $ \mu_i $ are convolvable (§1, No. 4, Prop. 4).

#### Proposition 4 {#int-viii-s3-prop-4 .statement}

*The mapping $ (\lambda, \mu) \mapsto \lambda * \mu $ (resp. $ (\lambda, \mu) \mapsto \mu * \lambda $), where $ \lambda \in \mathcal{C}'(G) $, $ \mu \in \mathcal{M}(G) $, defines on $ \mathcal{M}(G) $ the structure of a left (resp. right) module over the algebra $ \mathcal{C}'(G) $.*

This follows from Props. 1 and 3.

#### Proposition 5 {#int-viii-s3-prop-5 .statement}

*Let $ \lambda $ be a left (resp. right) Haar measure on G, and $ \mu \in \mathcal{M}^1(G) $. Then $ \mu $ and $ \lambda $ (resp. $ \lambda $ and $ \mu $) are convolvable, and $ \mu * \lambda = \mu(1)\lambda $ (resp. $ \lambda * \mu = \mu(1)\lambda $).*

We can suppose that $ \mu \geqslant 0 $. Let $ f \in \mathcal{K}_+(G) $. When $ \lambda $ is a left Haar measure,

$$
\int^* d\mu(x) \int^* f(xy)\, d\lambda(y) = \int^* d\mu(x) \int f(y)\, d\lambda(y) = \lambda(f)\|\mu\| ,
$$

therefore the function $ (x, y) \mapsto f(xy) $ is $ (\mu \otimes \lambda) $-integrable, and its integral for $ \mu \otimes \lambda $ is $ \lambda(f)\|\mu\| $. One argues similarly when $ \lambda $ is a right Haar measure.

#### Proposition 6 {#int-viii-s3-prop-6 .statement}

*Let $ \mu $ and $ \nu $ be two convolvable measures on G. Let $ \chi $ be a continuous representation of G in $ \mathbf{C}^* $. Then $ \chi \cdot \mu $ and $ \chi \cdot \nu $ are convolvable and $ (\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu) $.*

Let $ f \in \mathcal{K}(G) $. Then $ f\chi \in \mathcal{K}(G) $, therefore the function

$$
(x, y) \mapsto f(xy)\chi(xy) = f(xy)\chi(x)\chi(y)
$$

on $ G \times G $ is integrable for $ \mu \otimes \nu $; therefore the function $ (x, y) \mapsto f(xy) $ is integrable for $ (\chi \cdot \mu) \otimes (\chi \cdot \nu) $; therefore $ \chi \cdot \mu $ and $ \chi \cdot \nu $ are convolvable. Moreover,

$$
\langle \chi \cdot \mu * \chi \cdot \nu, f \rangle = \int f(xy)\chi(x)\chi(y)\, d\mu(x)\, d\nu(y)
= \int (f\chi)(xy)\, d\mu(x)\, d\nu(y) = \langle \mu * \nu, \chi f \rangle ,
$$

whence $ (\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu) $.

#### Proposition 7 {#int-viii-s3-prop-7 .statement}

*Let G and G' be two locally compact groups, u a continuous representation of G in G', and $ \mu_1, \ldots, \mu_n $ measures on G, all $ \neq 0 $. Then the following assertions are equivalent:
(i) $ u $ is $ \mu_i $-proper for all i, and the measures $ u(|\mu_i|) $ are convolvable;
(ii) the $ \mu_i $ are convolvable and $ u $ is proper for $ *_{i}(|\mu_i|) $.
When these conditions are satisfied,

$$
*_{i} u(\mu_i) = u(*_{i} \mu_i).
$$

This follows from §1, No. 2, Cor. of Prop. 1.

#### Corollary {#int-viii-s3-n1-cor-1 .statement}

*Let G be a locally compact group, $ \mu_1, \ldots, \mu_n $ measures on G. For the sequence $ (\mu_i)_{1 \leq i \leq n} $ to be convolvable, it is necessary and sufficient that the sequence $ (\check{\mu}_{n-i})_{0 \leq i \leq n-1} $ be so, in which case*

$$
(\mu_1 * \cdots * \mu_n)^{\vee} = \check{\mu}_n * \cdots * \check{\mu}_1.
$$

This follows from Prop. 7 on considering the isomorphism $ x \mapsto x^{-1} $ of G onto the opposite group.

### 2. The case of a group operating on a space

Let X be a locally compact space on which a locally compact group G operates on the left continuously by

$$
(s, x) \mapsto s \cdot x.
$$

If $ \mu_1, \ldots, \mu_n $ are measures on G and $ \nu $ is a measure on X, these will be said to be convolvable if they are so for the mapping $ (s_1, \ldots, s_n, x) \mapsto s_1 \cdots s_n x $ of $ G^n \times X $ into X, and their convolution product is to be understood in the sense of this mapping.

If $ s \in G $ and $ x \in X $, then

(4)
$$
\varepsilon_s * \varepsilon_x = \varepsilon_{sx}.
$$

If $ s \in G $ and $ \mu \in \mathcal{M}(X) $, then

(5)
$$
\varepsilon_s * \mu = \gamma(s)\mu
$$
by §1, No. 1, Example 3.

#### Proposition 8 {#int-viii-s3-prop-8 .statement}

— Let $ \mu $ be a measure on $ G $, $ \nu $ a measure on $ X $.
(i) If $ \mu $ has compact support, then $ \mu $ and $ \nu $ are convolvable.
(ii) If $ \nu $ has compact support, and if $ G $ operates properly in $ X $, then $ \mu $ and $ \nu $ are convolvable.
This follows from Prop. 4 of §1, No. 4.

#### Proposition 9 {#int-viii-s3-prop-9 .statement}

— For convolution, $ \mathcal{M}^1(X) $ is a left module over $ \mathcal{M}^1(G) $, while $ \mathcal{M}(X) $ and $ \mathcal{C}'(X) $ are left modules over $ \mathcal{C}'(G) $.
This follows from Prop. 8, and from §1, Props. 1, 3 and the Cor. of Prop. 5.

#### Proposition 10 {#int-viii-s3-prop-10 .statement}

— Let $ \mu $ be a measure on $ G $, $ \nu $ a measure on $ X $, $ \mu $ and $ \nu $ being convolvable. Suppose in addition that there exists a positive measure $ \beta $ on $ X $ such that $ \gamma(s)\nu $ has base $ \beta $ for every $ s \in G $. Then $ \mu * \nu $ has base $ \beta $.
Let $ K $ be a $ \beta $-negligible compact subset of $ X $. Then $ K $ is $ \gamma(s)|\nu| $-negligible for every $ s \in G $. Now,
$$
|\mu| * |\nu| = \int_G (\varepsilon_s * |\nu|) d|\mu|(s)
$$
(§1, No. 5, Prop. 7), and the mapping $ s \mapsto \varepsilon_s * |\nu| $ is vaguely continuous (§2, Prop. 6). Therefore $ K $ is $ |\mu| * |\nu| $-negligible by Ch. V, §3, No. 3, Th. 1. Therefore $ |\mu| * |\nu| $ has base $ \beta $ (Ch. V, §5, No. 5, Th. 2).

### 3. Convolution and linear representations

#### Proposition 11 {#int-viii-s3-prop-11 .statement}

— Let $ G $ be a locally compact group, $ E $ a quasi-complete locally convex space, $ U $ a continuous representation of $ G $ in $ E $.
(i) If $ \lambda \in \mathcal{C}'(G) $, $ \mu \in \mathcal{C}'(G) $, then $ U(\lambda * \mu) = U(\lambda)U(\mu) $.
(ii) Suppose that $ E $ is a Banach space, and let $ \rho(s) = \|U(s)\| $ for $ s \in G $. If $ \lambda \in \mathcal{M}^\rho(G) $, $ \mu \in \mathcal{M}^\rho(G) $, then $ U(\lambda * \mu) = U(\lambda)U(\mu) $.
Let $ \lambda, \mu $ be in $ \mathcal{C}'(G) $. For any $ x \in E $ one has, by applying notably Props. 1 and 4 of Ch. VI, §1, No. 1,
$$
U(\lambda * \mu)x = \int_G U(s)x\, d(\lambda * \mu)(s)
$$
$$
= \int_{G \times G} U(st)x\, d\lambda(s)\, d\mu(t) = \int_{G \times G} U(s)U(t)x\, d\lambda(s)\, d\mu(t)
$$
$$
= \int_G U(\lambda)U(t)x\, d\mu(t) = U(\lambda) \int_G U(t)x\, d\mu(t) = U(\lambda)U(\mu)x ,
$$
whence (i). An analogous argument may be applied in case (ii).

With G still a locally compact group, let us assume that G operates continuously on the left in a locally compact space X. This defines (§2, No. 4) a continuous linear representation $ \gamma $ of G in $ \mathcal{M}(X) $ (equipped with the topology of compact convergence in $ \mathcal{H}(X) $).

#### Proposition 12 {#int-viii-s3-prop-12 .statement}

*If $ \lambda \in \mathcal{C}'(G) $ and $ \mu \in \mathcal{M}(X) $, then*

$$
\gamma(\lambda)\mu = \lambda * \mu.
$$

By Prop. 7 of §1, No. 5,

$$
\lambda * \mu = \int_G (\varepsilon_s * \mu) d\lambda(s).
$$

Now, $ \varepsilon_s * \mu = \gamma(s)\mu $ (No. 2, formula (5)) and

$$
\int_G (\gamma(s)\mu) d\lambda(s) = \gamma(\lambda)\mu
$$

by the definition of $ \gamma(\lambda) $.

#### Corollary {#int-viii-s3-n3-cor-1 .statement}

*The mapping $ (\lambda, \mu) \mapsto \lambda * \mu $ of $ \mathcal{C}'(G) \times \mathcal{M}(X) $ into $ \mathcal{M}(X) $ is hypocontinuous relative to the equicontinuous subsets of $ \mathcal{C}'(G) $ and the compact subsets of $ \mathcal{M}(X) $ ($ \mathcal{C}'(G) $ and $ \mathcal{M}(X) $ being equipped with the topology of compact convergence in $ \mathcal{C}(G) $ and $ \mathcal{H}(X) $, respectively).*

For, $ \mathcal{M}(X) $, equipped with the topology of compact convergence in $ \mathcal{H}(X) $, is quasi-complete. Therefore the mapping $ (\lambda, \mu) \mapsto \gamma(\lambda)\mu $ of $ \mathcal{C}'(G) \times \mathcal{M}(X) $ into $ \mathcal{M}(X) $ is hypocontinuous relative to the equicontinuous subsets of $ \mathcal{C}'(G) $ and the compact subsets of $ \mathcal{M}(X) $ (§2, No. 6). It then suffices to apply Prop. 12.

#### Remark {#int-viii-s3-n3-rem-1 .statement}

— 1) Let $ \lambda_0 \in \mathcal{C}'(G) $. The mapping $ \mu \mapsto \lambda_0 * \mu $ of $ \mathcal{M}(X) $ into $ \mathcal{M}(X) $ is vaguely continuous. For, let $ f \in \mathcal{H}(X) $. One has

$$
\langle \lambda_0 * \mu, f \rangle = \int f(sx) d\lambda_0(s) d\mu(x) = \langle \mu, g \rangle,
$$

where $ g(x) = \int f(sx) d\lambda_0(s) $. Now, $ g $ is continuous (Ch. VII, §1, No. 1, Lemma 1). On the other hand, let S be the support of $ \lambda_0 $ and K that of $ f $. The conditions $ sx \in K $ and $ s \in S $ imply $ x \in S^{-1}K $; therefore the support of $ g $ is contained in $ S^{-1}K $, so that $ g \in \mathcal{H}(X) $. Then $ \langle \lambda_0 * \mu, f \rangle = \langle \mu, g \rangle $ is a vaguely continuous function of $ \mu $, which proves our assertion.

2) Let $ \mu_0 \in \mathcal{M}(X) $. The mapping $ \lambda \mapsto \lambda * \mu_0 $ of $ \mathcal{C}'(G) $ into $ \mathcal{M}(X) $ is continuous for the topologies $ \sigma(\mathcal{C}'(G), \mathcal{C}(G)) $ and $ \sigma(\mathcal{M}(X), \mathcal{H}(X)) $. For, let $ f \in \mathcal{K}(X) $. Setting $ h(s) = \int f(sx)\, d\mu_0(x) $, we have $ \langle f, \lambda * \mu_0 \rangle = \langle h, \lambda \rangle $, and $ h \in \mathcal{C}(G) $ (Ch. VII, §1, No. 1, Lemma 1).

#### Proposition 13 {#int-viii-s3-prop-13 .statement}

*The mapping* $ (s, \mu) \mapsto \gamma(s)\mu $ *of* $ G \times \mathcal{M}_+(X) $ *into* $ \mathcal{M}_+(X) $ *is continuous when the set* $ \mathcal{M}_+(X) $ *of positive measures on* $ X $ *is equipped with the vague topology*.

Since $ \gamma(s)\mu = \gamma(ss_0^{-1})\gamma(s_0)\mu $, it follows from *Remark 1* that it suffices to prove the continuity of the mapping under consideration at a point of the form $ (e, \mu_0) $ with $ \mu_0 \in \mathcal{M}_+(X) $. Given a function $ f \in \mathcal{K}(X) $ and a number $ \varepsilon > 0 $, it is thus a matter of showing that there exist a neighborhood U of e in G and a neighborhood W of $ \mu_0 $ in $ \mathcal{M}_+(X) $ such that the relations $ s \in U, \mu \in W $ imply

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon .
$$

Let V be a compact neighborhood of the support K of $ f $ in X, and let $ \varphi \in \mathcal{K}_+(X) $ be such that $ \varphi(x) = 1 $ on V; there exists a neighborhood $ W_0 $ of $ \mu_0 $ in $ \mathcal{M}_+(X) $ such that $ a = \sup_{\mu \in W_0} \mu(V) $ is finite: it suffices to take for $ W_0 $ the set of $ \mu \in \mathcal{M}_+(X) $ such that $ |\langle \varphi, \mu - \mu_0 \rangle| \leq 1 $. Since the mapping $ (s, x) \mapsto sx $ is continuous, there is, on the other hand, a compact neighborhood $ U_0 $ of e in G such that $ sK \subset V $ for all $ s \in U_0 $; the function $ (s, x) \mapsto f(sx) $ is then uniformly continuous in $ U_0 \times V $ and so there is a neighborhood $ U \subset U_0 $ of e such that $ |f(sx) - f(x)| \leq \varepsilon / 2a $ for all $ s \in U $ and $ x \in V $. For $ s \in U $ and $ \mu \in W_0 $, we therefore have

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu(x) \right| \leq \varepsilon / 2 ;
$$

if $ W \subset W_0 $ is the neighborhood of $ \mu_0 $ in $ \mathcal{M}_+(X) $ formed by the measures $ \mu \in W_0 $ such that $ \left| \int f(x)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon / 2 $, U and W meet the requirements.

### Exercises {#int-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
