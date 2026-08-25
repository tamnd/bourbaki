---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 6
section_title: The Hausdorff series
lang: en
source: lie-i-iii
pdf_pages: 0173-0182, 0219-0222
extraction: ocr
subsections:
    - "no": 1
      title: EXPONENTIAL AND LOGARITHM IN FILTERED ALGEBRAS
      page: 0
      pdf_page: 173
    - "no": 2
      title: HAUSDORFF GROUP
      page: 0
      pdf_page: 175
    - "no": 3
      title: LIE FORMAL POWER SERIES
      page: 0
      pdf_page: 176
    - "no": 4
      title: THE HAUSDORFF SERIES
      page: 0
      pdf_page: 178
    - "no": 5
      title: SUBSTITUTIONS IN THE HAUSDORFF SERIES
      page: 0
      pdf_page: 179
statements: 14
exercises: 3
content_sha256: a588e29717103254d7272a25b47f928b860d25d73c99158135d8f87332ab07da
---

## § 6. THE HAUSDORFF SERIES

*In this paragraph we assume that $ K $ is a field of characteristic 0.*

### 1. EXPONENTIAL AND LOGARITHM IN FILTERED ALGEBRAS

Let $ A $ be a unital associative algebra which is Hausdorff and complete under a real filtration $ (A_\alpha) $. We write $ m = A_0^+ = \bigcup_{\alpha > 0} A_\alpha $.

For $ x \in m $, the family $ (x^n/n!)_{n \in \mathbf{N}} $ is summable. We write

$$
e^x = \exp x = \sum_{n \geqslant 0} x^n/n!.
$$

Then $ \exp(x) \in 1 + m $ and the mapping $ \exp : m \to 1 + m $ is called the *exponential mapping* of $ A $.

For all $ y \in 1 + m $, the family $ ((-1)^{n-1}(y-1)^n/n)_{n \geqslant 1} $ is summable. We write

$$
\log y = \sum_{n \geqslant 1} (-1)^{n-1}(y-1)^n/n.
$$

Then $ \log y \in m $ and the mapping $ \log : 1 + m \to m $ is called the *logarithmic mapping* of $ A $.

#### Proposition 1 {#lie-ii-s6-prop-1 .statement}

*The exponential mapping is a homeomorphism of $ m $ onto $ 1 + m $ and the logarithmic mapping is the inverse homeomorphism.*

For $ x \in A_\alpha $, $ \frac{x^n}{n!} \in A_{n\alpha} $. It follows that the series defining the exponential converges uniformly on each of the sets $ A_\alpha $ for $ \alpha > 0 $; as $ A_\alpha $ is open in $ m $ and $ m = \bigcup_{\alpha > 0} A_\alpha $, the exponential mapping is continuous. It can be similarly shown that the logarithmic mapping is continuous.

Let $ e $ and $ l $ be the formal power series with no constant term

$$
e(X) = \sum_{n \geq 1} \frac{X^n}{n!}, \quad l(X) = \sum_{n \geq 1} (-1)^{n-1} X^n / n.
$$

We know (*Algebra*, Chapter IV, § 6, no. 9) that $ e(l(X)) = l(e(X)) = X $ on $ \hat{A}(\{X\}) = K[[X]] $. By substitution (§ 5, no. 1), we deduce that

$$
e(l(x)) = l(e(x)) = x
$$

for $ x \in m $; as

$$
\exp x = e(x) + 1, \quad \log(1 + x) = l(x)
$$

it follows immediately that

$$
\log \exp x = x, \quad \exp \log(1 + x) = 1 + x
$$

for $ x $ in $ m $, whence the proposition.

#### Remark {#lie-ii-s6-n1-rem-1 .statement}

(1) If $ x \in m, y \in m $ and $ x $ and $ y $ commute, then

$$
\exp(x + y) = \exp(x) \exp(y),
$$

since the family $ \left( \frac{x^i}{i!} \cdot \frac{y^j}{j!} \right)_{i,j \in \mathbf{N}} $ is summable (cf. *Algebra*, Chapter IV, § 6, no. 9, Proposition 11).

(2) As the series $ e $ and $ l $ are without constant term and $ A_\alpha $ is a closed ideal of $ A $, $ \exp A_\alpha \subset 1 + A_\alpha $ and $ \log(1 + A_\alpha) \subset A_\alpha $ whence $ \exp A_\alpha = 1 + A_\alpha $ and $ \log(1 + A_\alpha) = A_\alpha $ for $ \alpha > 0 $.

(3) Let $ B $ be a complete Hausdorff filtered unital associative algebra and $ n = \bigcup_{\alpha > 0} B_\alpha $. Let $ f $ be a continuous unital homomorphism of $ A $ into $ B $ such that $ f(m) \subset n $. Then $ f(\exp x) = \exp f(x) $ for $ x \in m $ and $ f(\log y) = \log f(y) $ for $ y \in 1 + m $; we show for example the first of these formulae:

$$
f(\exp x) = \sum_{n \geq 0} f(x^n)/n! = \sum_{n \geq 0} f(x)^n/n! = \exp f(x).
$$

(4) Let E be a unital associative algebra. If a is a nilpotent element of E, the family $ \left( \frac{a^n}{n!} \right)_{n \in \mathbf{N}} $ has finite support and we write $ \exp a = \sum_{n \geq 0} a^n / n! $. An element b is unipotent if $ b - 1 $ is nilpotent; then we write

$$
\log b = \sum_{n \geq 1} (-1)^{n-1} (b - 1)^n / n.
$$

We deduce from the relations $ e(l(X)) = l(e(X)) = X $ that the mapping $ a \mapsto \exp a $ is a bijection of the set of nilpotent elements of E onto the set of unipotent elements of E and that $ b \mapsto \log b $ is the inverse mapping.

### 2. HAUSDORFF GROUP

Let X be a set. We use the notation of § 5, nos. 1 and 2. The free Lie algebra L(X) is identified with its canonical image in A(X) (\S 3, no. 1, Theorem 1). We denote by $ \hat{L}(X) $ the closure of L(X) in $ \hat{A}(X) $, that is the set of elements of $ \hat{A}(X) $ of the form $ a = \sum_{n \geq 1} a_n $ such that $ a_n \in L^n(X) $ for all $ n \geq 0 $; this is filtered Lie subalgebra of $ \hat{A}(X) $.

#### Theorem 1 {#lie-ii-s6-thm-1 .statement}

*The restriction of the exponential mapping of $ \hat{A}(X) $ to $ \hat{L}(X) $ is a bijection of $ \hat{L}(X) $ onto a closed subgroup of the Magnus group $ \Gamma(X) $.*

We write $ A(X) = A, A^n(X) = A^n, \hat{A}(X) = \hat{A}, L^n(X) = L^n, \hat{L}(X) = \hat{L}, \Gamma(X) = \Gamma $. Let B be the algebra $ A \otimes A $ with the graduation of type $ \mathbf{N} $ defined by $ B^n = \sum_{i+j=n} A^i \otimes A^j $. Let $ \hat{B} = \prod_{n \geq 0} B^n $ be the associated complete filtered algebra (*Commutative Algebra*, Chapter III, § 2, no. 12, *Example* 1). The coproduct $ c : A \to A \otimes A $ defined in § 3, no. 1, Corollary 1 to Theorem 1 is graded of degree 0 and hence extends by continuity to a homomorphism $ \hat{c} : \hat{A} \to \hat{B} $ given by

$$
\hat{c}\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} c(a_n) \quad \text{for } a_n \in A^n.
$$

We also define continuous homomorphisms $ \delta' $ and $ \delta'' $ of $ \hat{A} $ into $ \hat{B} $ by

$$
\delta'\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (a_n \otimes 1), \qquad \delta''\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (1 \otimes a_n) \quad \text{for } a_n \in A^n.
$$

By Corollary 2 to Theorem 1 of § 3, no. 1, $ L^n $ is the set of $ a_n \in A^n $ such that $ c(a_n) = a_n \otimes 1 + 1 \otimes a_n $. It follows that $ \hat{L} $ is the set of $ a \in \hat{A} $ such that

$$
\hat{c}(a) = \delta'(a) + \delta''(a).
$$

Let $ \Delta $ be the set of $ b \in \hat{A} $ of constant term equal to 1 and satisfying the relation

$$
\hat{c}(b) = \delta'(b) \cdot \delta''(b),
$$

in other words, the set of $ b = \sum_{n \geq 0} b_n $ such that $ b_n \in \mathbf{A}^n $ for all $ n \geq 0 $, $ b_0 = 1 $ and $ c(b_n) = \sum_{i+j=n} b_i \otimes b_j $ for $ n \geq 0 $. The latter characterization shows that $ \Delta $ is a closed subset of $ \Gamma $; as $ \hat{\epsilon} $, $ \delta' $ and $ \delta'' $ are ring homomorphisms and every element of $ \delta'(\hat{\mathbf{A}}) $ commutes with every element of $ \delta''(\hat{\mathbf{A}}) $, the restrictions to $ \Gamma $ of the mappings $ c $ and $ \delta'\delta'' $ are group homomorphisms and $ \Delta $ is a subgroup of $ \Gamma $.

By Proposition 1 of no. 1, the exponential mapping of $ \hat{\mathbf{A}} $ is a bijection of the set $ \hat{\mathbf{A}}^+ $ of elements of $ \hat{\mathbf{A}} $ with no constant term onto $ \Gamma $. Let $ a \in \hat{\mathbf{A}}^+ $ and $ b = \exp a $. As $ \hat{\epsilon} $ is a continuous ring homomorphism,

$$
\hat{\epsilon}(b) = \hat{\epsilon}\left( \sum_{n \geq 0} a^n/n! \right) = \sum_{n \geq 0} \hat{\epsilon}(a)^n/n! = \exp \hat{\epsilon}(a).
$$

The relations

$$
\delta'(b) = \exp \delta'(a), \quad \delta''(b) = \exp \delta''(a)
$$

are proved similarly and, as $ \delta'(a) $ commutes with $ \delta''(a) $ (no. 1, Remark 1),

$$
\delta'(b) \delta''(b) = \exp (\delta'(a) + \delta''(a)).
$$

Therefore $ a $ satisfies (3) if and only if $ b $ satisfies (4), which proves the theorem.

#### Remark {#lie-ii-s6-n2-rem-1 .statement}

The above proof shows that $ \exp(\hat{\mathbf{L}}) $ is the subgroup $ \Delta $ of $ \Gamma $ consisting of the $ b $ satisfying (4).

Hence the group law of $ \Delta $ can be transported by the exponential mapping to $ \hat{\mathbf{L}} $. In other words, $ \hat{\mathbf{L}} $ is a complete topological group with the law of composition $ (a, b) \mapsto a \mathbin{\mathbf{h}} b $ given by

$$
a \mathbin{\mathbf{h}} b = \log(\exp a \cdot \exp b).
$$

The topological group thus obtained is called the *Hausdorff group* (derived from X relative to K).

Let $ g $ be the homomorphism of the free group $ F = F(X) $ into $ \Gamma $ such that $ g(x) = \exp x $ for $ x \in X $. As $ \exp x - 1 - x = \sum_{n \geq 2} x^n/n! $ is of order $ \geq 2 $, $ g $ is injective by Theorem 1 of § 5, no. 3. Therefore *the mapping $ \log \circ g $ is an injective homomorphism of $ F $ into the Hausdorff group which extends the canonical injection $ X \to \hat{\mathbf{L}}$*.

For every integer $ m \geq 1 $ we denote by $ \hat{\mathbf{L}}_m $ the set of elements of order $ \geq m $ in $ \hat{\mathbf{L}} $ and by $ \Gamma_m $ the set of $ u \in \Gamma $ such that $ u - 1 $ is of order $ \geq m $. Then $ \hat{\mathbf{L}}_m = \exp(\Gamma_m) $ by Remark 2 of no. 1; as $ (\Gamma_m)_{m \geq 1} $ is an integral central filtration on $ \Gamma $ (§ 4, no. 5 Proposition 2), $ (\hat{\mathbf{L}}_m)_{m \geq 1} $ *is an integral central filtration on the group $ \hat{\mathbf{L}}$*.

### 3. LIE FORMAL POWER SERIES

#### Lemma 1 {#lie-ii-s6-lem-1 .statement}

*Let $ \mathfrak{g} $ be a filtered Lie algebra (§ 4, no. 1), $ (\mathfrak{g}_\alpha)_{\alpha \in \mathbf{R}} $ its filtration and let $ \alpha \in \mathbf{R} $. Let P be a homogeneous Lie polynomial of degree n in the indeterminates $ (\Gamma_i)_{i \in I} $ (§ 2, no. 4). Then $ P((a_i)) \in \mathfrak{g}_{n\alpha} $ for every family $ (a_i)_{i \in I} $ of elements of $ \mathfrak{g}_\alpha$*.

Every Lie polynomial of degree $ n \geqslant 2 $ is a finite sum of terms of the form $[Q, R]$ where $ Q $ and $ R $ are of degree $ < n $ and the sum their degrees is equal to $ n $ (\S 2, no. 7, Proposition 7). The lemma follows by induction on $ n $.

A *Lie formal power series*† (with coefficients in $ K $) *in the indeterminates* $ (T_i)_{i \in I} $ is any element of the Lie algebra $ \hat{L}((T_i)_{i \in I}) = \hat{L}(I) $. Such an element $ u $ can be written uniquely as the sum of a summable family $ (u_\nu)_{\nu \in \mathbf{N}^{(I)}} $ where $ u_\nu \in L^\nu(I) $.

Suppose that $ I $ is *finite*. Let $ g $ be a complete Hausdorff filtered Lie algebra such that $ g = \bigcup_{\alpha > 0} g_\alpha $; let $ t = (t_i)_{i \in I} $ be a family of elements of $ g $.

#### Proposition 2 {#lie-ii-s6-prop-2 .statement}

*The homomorphism* $ f_t : L(I) \to g $ *such that* $ f_t(T_i) = t_i $ (\S 2, no. 4) *can be extended by continuity to one and only one continuous homomorphism* $ \hat{f}_t $ *of* $ \hat{L}(I) $ *into* $ g $.

There exists $ \alpha > 0 $ such that $ t_i \in g_\alpha $ for all $ i \in I $; hence $ f_t(L^\nu(I)) \subset g_{|\nu| \wedge \alpha} $ for all $ \nu $ (Lemma 1), which implies the continuity of $ \hat{f}_t $.

If $ u \in \hat{L}(I) $, we write $ u((t_i)) = \hat{f}_t(u) $. In particular, taking $ g = \hat{L}(I) $, $ u = u((T_i)) $; in the general case, $ u((t_i)) $ is called the result of substituting the $ t_i $ for the $ T_i $ in the Lie formal power series $ u((T_i)) $. If $ u = \sum_{\nu \in \mathbf{N}^{(I)}} u_\nu $, where $ u_\nu \in L^\nu(X) $, the family $ (u_\nu((t_i)))_{\nu \in \mathbf{N}^{(I)}} $ is summable and
$$
u((t_i)) = \sum_{\nu \in \mathbf{N}^{I}} u_\nu((t_i)).
$$

Let $ \sigma $ be a continuous homomorphism of $ g $ into a complete Hausdorff filtered Lie algebra $ g' $ such that $ g' = \bigcup_{\alpha > 0} g'_\alpha $. For every *finite* family $ t = (t_i)_{i \in I} $ of elements of $ g $ and all $ u \in \hat{L}(I) $,
$$
\sigma(u((t_i))) = u((\sigma(t_i))),
$$
for the homomorphism $ \sigma \circ \hat{f}_t $ is continuous and maps $ T_i $ to $ \sigma(t_i) $ for $ i \in I $.

Let $ u = (u_j)_{j \in J} $ be a *finite* family of elements of $ \hat{L}(I) $ and let $ v \in \hat{L}(J) $; by substituting the $ u_j $ for the $ T_j $ in $ v $, we obtain an element $ w = v((u_j)_{j \in J}) $ of $ \hat{L}(I) $ denoted by $ v \circ u $. Then
$$
w((t_i)_{i \in I}) = v((u_j((t_i)_{i \in I}))_{j \in J})
$$
for every *finite* family $ t = (t_i)_{i \in I} $ of elements of $ g $, as is seen by operating with the continuous homomorphism $ \hat{f}_t $ on the equation $ w = v((u_j)_{j \in J}) $.

Let $ u = \sum_{\nu \in \mathbf{N}^{I}} u_\nu \in \hat{L}(I) $, where $ u_\nu \in L^\nu(I) $. The mapping $ \tilde{u} $ $ (t_i) \mapsto u((t_i)) $ of $ g^I $ into $ g $ is *continuous*: for in each of the open sets $ g_\alpha $ with $ \alpha > 0 $ the family of $ \tilde{u}_\alpha $ is uniformly summable and it suffices to prove that each $ \tilde{u}_\nu $ is continuous, which is immediate by induction on $ |\nu| $.

† A Lie formal power series is not in general a formal power series in the sense of *Algebra*, Chapter IV, § 6.

### 4. THE HAUSDORFF SERIES

Let {U, V} be a set with two elements.

#### Definition 1 {#lie-ii-s6-def-1 .statement}

*The element* $ H = U \circledast V = \log(\exp U \cdot \exp V) $ (no. 2) *of the Lie algebra* $ \hat{L}_\mathbf{Q}(\{U, V\}) $ *is called the Hausdorff series in the indeterminates* U *and* V.

We denote by $ H_n $ (resp. $ H_{r,s} $) the homogeneous component of H of total degree n (resp. multidegree $(r, s)$). Then

$$
H = \sum_{n \geq 0} H_n = \sum_{r, s \geq 0} H_{r,s}, \quad H_n = \sum_{r+s=n \atop r, s \geq 0} H_{r,s}.
$$

#### Theorem 2 {#lie-ii-s6-thm-2 .statement}

*If r and s are two positive integers such that* $ r + s \geq 1 $, *then* $ H_{r,s} = H'_{r,s} + H''_{r,s} $, *where*

$$
(r + s)H'_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s-1 \\ 1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} (V)
$$

$$
(r + s)H''_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) (U).
$$

In $ \hat{A}_\mathbf{Q}(\{U, V\}) $, $ \exp U \cdot \exp V = 1 + W $, where $ W = \sum_{r+s \geq 1} \frac{U^r V^s}{r! s!} $, whence

$$
H = \sum_{m \geq 1} (-1)^{m-1} W^m / m \text{ (no. 2)}, \text{ that is:}
$$

$$
H_{r,s} = \sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_m + s_m \geq 1}}
\prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!}.
$$

The linear mapping $ P_n $, defined by $ P_n(x_1, \ldots, x_n) = \frac{1}{n} \left( \prod_{i=1}^{n-1} (\mathrm{ad}\, x_i) \right)(x_n) $ for $ n \geq 1 $ and $ x_1, \ldots, x_n $ in $ \{U, V\} $, is a projector of $ A^n_\mathbf{Q}(\{U, V\}) $ onto $ L^n_\mathbf{Q}(\{U, V\}) $ (\S 3, no. 2, Corollary to Proposition 1); as $ H_{r,s} $ belongs to $ L^{r+s}_\mathbf{Q}(\{U, V\}) $, $ H_{r,s} = P_{r+s}(H_{r,s}) $. Now

$$
P_{r+s} \left( \prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!} \right)
= \frac{1}{r+s} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} \frac{(\mathrm{ad}\, V)^{s_{m-1}}}{s_{m-1}!} (V)
$$

when $ s_m \geqslant 1 $ and

$$
(13)\quad P_{r+s}\left(\prod_{i=1}^{m} \frac{U r_i}{r_i!} \frac{V s_i}{s_i!}\right) = \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m-1}}{r_m!} \right)(U)
$$

when $ r_m \geqslant 1 $ and $ s_m = 0 $. Moreover, obviously $ (\mathrm{ad}\ t)^{p-1}.t = 0 $ if $ p \geqslant 2 $ and $ (\mathrm{ad}\ t)^0.t = t $. It follows that the two sides of (12) are zero when $ s_m \geqslant 2 $ and those of (13) are zero when $ r_m \geqslant 2 $. The theorem then follows since $ H'_{r,s} $ is the sum of the terms of type (12) and $ H''_{r,s} $ is the sum of the terms of type (13).

#### Remark {#lie-ii-s6-n4-rem-1 .statement}

(1) We have defined (\S 3, no. 2, Remark) a projector $ Q $ of $ A(X) $ onto $ L(X) $ such that $ Q(a^m) = 0 $ for $ a \in L(X) $ and $ m \geqslant 2 $ and $ Q(1) = 0 $. Then $ H = Q(\exp H) = Q(\exp U.\exp V) $, whence immediately

$$
(14)\quad H_{r,s} = Q \left( \frac{U^r V^s}{r! s!} \right) \quad \text{for } r + s \geqslant 1.
$$

(2) We have

$$
(15)\quad H(U, V) \equiv U + V + \frac{1}{2}[U, V] + \frac{1}{12}[U, [U, V]] \\
+ \frac{1}{12}[V, [V, U]] - \frac{1}{24}[U, [V, [U, V]]]
$$
modulo $ \sum_{n \geqslant 5} L^n(\{U, V\}) $.

(3) $ H_{0,n} = H_{n,0} = 0 $ for every integer $ n \neq 1 $, whence

$$
(16)\quad H(U, 0) = H(0, U) = U.
$$

On the other hand, as $ [U, -U] = 0 $,

$$
(17)\quad H(U, -U) = 0.
$$

### 5. SUBSTITUTIONS IN THE HAUSDORFF SERIES

As $ K $ is a field containing $ \mathbf{Q} $, the Hausdorff series can be considered as a Lie formal power series with coefficients in $ K $. Therefore, if $ g $ is a complete Hausdorff filtered Lie algebra with $ g = \bigcup_{\alpha > 0} g_\alpha $, then, for $ a, b $ in $ g $, $ a $ and $ b $ can be substituted for $ U $ and $ V $ in $ H $ (cf. no. 3 and \S 2, no. 5, Remark).

In particular, let $ A $ be a complete Hausdorff filtered unital associative algebra. We write $ m = \bigcup_{\alpha > 0} A_\alpha $ and $ m_\alpha = A_\alpha \cap m $ for $ \alpha \in \mathbf{R} $; hence $ m_\alpha = A_\alpha $ for $ \alpha > 0 $ and $ m_\alpha = m $ for $ \alpha \leqslant 0 $. With the bracket $ [a, b] = ab - ba $, $ m $ is a complete Hausdorff filtered Lie algebra, to which the above can be applied. With this notation, we have the following result which completes Proposition 1 of no. 1.

#### Proposition 3 {#lie-ii-s6-prop-3 .statement}

*If $ a \in m, b \in m $, then $ \exp H(a, b) = \exp a . \exp b $.*

Let $ a, b $ be in $ m $; there exists $ \alpha > 0 $ such that $ a \in A_\alpha $ and $ b \in A_\alpha $. Then there exists a continuous homomorphism $ \theta $ of the Magnus algebra $ \hat{A}(\{U, V\}) $ into $ A $ mapping $ U $ to $ a $ and $ V $ to $ b $ (\S 5, no. 1, Proposition 1).

The restriction of $ \theta $ to $ \hat{L}(\{U, V\}) $ is a continuous homomorphism of Lie algebras of $ L(\{U, V\}) $ into $ m $ which maps $ U $ (resp. $ V $) to $ a $ (resp. $ b $). By formula (6) of no. 3, therefore $ \theta(H) = H(a, b) $. It then suffices to apply the continuous homomorphism $ \theta $ to the two sides of the relation
$$
\exp H(U, V) = \exp U . \exp V
$$
taking account of *Remark 3* of no. 1.

#### Remark 1 {#lie-ii-s6-n5-rem-1 .statement}

If $ a $ and $ b $ commute, then $ H_{r,s}(a, b) = 0 $ for $ r + s \geq 2 $, for every homogeneous Lie polynomial of degree $ \geq 2 $ is zero at $ (a, b) $. Then $ H(a, b) = a + b $ and Proposition 3 recovers the formula
$$
\exp(a + b) = \exp a . \exp b.
$$

#### Proposition 4 {#lie-ii-s6-prop-4 .statement}

*Let $ g $ be a complete Hausdorff filtered Lie algebra such that $ g = \bigcup_{\alpha > 0} g_\alpha $. The mapping $ (a, b) \mapsto H(a, b) $ is a group law on $ g $ compatible with the topology on $ g $ under which $ 0 $ is the identity element and $ -a $ is the inverse of $ a $ for all $ a \in g $.*

The mapping $ (a, b) \mapsto H(a, b) $ of $ g \times g $ into $ g $ is continuous (no. 3); as the mapping $ a \mapsto -a $ is obviously continuous, it suffices to prove the relations
$$
\begin{align*}
(18) \quad & H(H(a, b), c) = H(a, H(b, c)) \\
(19) \quad & H(a, -a) = 0 \\
(20) \quad & H(a, 0) = H(0, a) = a
\end{align*}
$$
for $ a, b, c $ in $ g $. By formula (7) of no. 3, it suffices to prove these formulae when $ a, b, c $ are three indeterminates and $ g = \hat{L}(\{a, b, c\}) $. Now the restriction of the exponential mapping to $ \hat{L}(\{a, b, c\}) $ is an injection into the Magnus algebra $ \hat{A}(\{a, b, c\}) $ and by Proposition 3:
$$
\begin{align*}
\exp H(H(a, b), c) &= \exp H(a, b) . \exp c = \exp a . \exp b . \exp c \\
\exp H(a, H(b, c)) &= \exp a . \exp H(b, c) = \exp a . \exp b . \exp c \\
\exp H(a, -a) &= \exp a . \exp(-a) = \exp(a - a) = \exp 0 \\
\exp H(a, 0) &= \exp a . \exp 0 = \exp a \\
\exp H(0, a) &= \exp 0 . \exp a = \exp a.
\end{align*}
$$
This establishes relations (18) to (20).

#### Remark {#lie-ii-s6-n5-rem-2 .statement}

(2) Take $ g $ to be the Lie algebra $ \hat{L}(X) $. The group law introduced in the above proposition coincides with the law defined in no. 2. In other words,
$$
a \mathbin{\mathbf{h}} b = H(a, b) \quad \text{for } a, b \text{ in } \hat{L}(X);
$$
thus the Hausdorff group law is given by the Hausdorff series.

(3) Let $ g $ be a Lie algebra with the integral filtration ($ \mathcal{C}^n g $) defined by the lower central series. Suppose that there exists $ m \geq 1 $ such that $ \mathcal{C}^m g = \{0\} $. With the topology derived from the filtration $ (\mathcal{C}^n g)_{n \geq 1} $, the Lie algebra $ g $ is Hausdorff, complete and even discrete. Then $ P(a_1, \ldots, a_r) = 0 $ for $ a_1, \ldots, a_r $ in $ g $ and for every homogeneous Lie polynomial $ P $ of degree $ \geq m $; in particular, $ H_{r,s}(a, b) = 0 $ for $ r + s \geq m $ and the series $ H(a, b) = \sum_{r,s} H_{r,s}(a, b) $ has only a finite number of non-zero terms. The group law $ (a, b) \mapsto H(a, b) $ on $ g $ is then a polynomial mapping (\$ 2, no. 4).

#### Proposition 5 {#lie-ii-s6-prop-5 .statement}

*Let $ K_{r,s} $ be the component of $ H(U + V, -U) $ of multidegree $ (r, s) $. Then*
$$
K_{n,1}(U, V) = \frac{1}{(n+1)!} (\operatorname{ad} U)^n(V) \quad \text{for } n \geq 0.
$$

We write $ K(U, V) = H(U + V, -U) $, $ K_1(U, V) = \sum_{n \geq 0} K_{n,1}(U, V) $. We denote by L (resp. R) left (resp. right) multiplication by $ U $ on $ \hat{A}(\{U, V\}) $.

We can write
$$
e^{U}V e^{-U} = \sum_{p, q} \frac{U^p}{p!} V \frac{(-U)^q}{q!}
= \sum_{n \geq 0} \frac{1}{n!} \left( \sum_{p+q=n} \frac{n!}{p!q!} (L^p(-R)^q) \cdot V \right)
= \sum_{n \geq 0} \frac{1}{n!} (L - R)^n V
$$
and therefore
$$
e^{U}V e^{-U} = \sum_{n \geq 0} \frac{1}{n!} (\operatorname{ad} U)^n V.
$$
We now calculate modulo the ideal $ \sum_{m \geq 0} \sum_{n \geq 2} A^{m,n}(\{U, V\}) $ of $ A(\{U, V\}) $. For all $ n \geq 1 $,
$$
(U + V)^n \equiv U^n + \sum_{i=1}^{n-1} U^i V U^{n-1-i}
$$
whence
$$
(\operatorname{ad} U)(U + V)^n \equiv ((L - R) \sum_{i=1}^{n-1} L^i R^{n-i}) \cdot V \\
\equiv (L^n - R^n) \cdot V \\
\equiv U^n V - V U^n.
$$
Therefore
$$
(\operatorname{ad} U) \cdot e^{U+V} \equiv e^{U}V - V e^{U}
$$
summing over $ n $.

On the other hand, $ K_1(U, V) \equiv K(U, V) $ and $ e^{K_1(U, V)} \equiv 1 + K_1(U, V) $ and hence
$$
K_1 \equiv e^K - 1 \equiv e^{U+V}e^{-U} - 1
$$
by Proposition 3. We deduce that
$$
\begin{align*}
(\mathrm{ad}\ U)K_1 &\equiv Ue^{U+V}e^{-U} - e^{U+V}e^{-U}U \\
&\equiv (e^{UV} - Ve^U)e^{-U} \quad \text{(by (23))} \\
&\equiv e^{UV}e^{-U} - V \\
&\equiv \sum_{n \geq 1} \frac{1}{n!} (\mathrm{ad}\ U)^n V \quad \text{(by (22))} \\
&\equiv (\mathrm{ad}\ U)\left( \sum_{n \geq 0} \frac{(\mathrm{ad}\ U)^n}{(n+1)!} V \right).
\end{align*}
$$
It then suffices to apply the *Remark* of § 2, no. 11.

### Exercises {#lie-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
