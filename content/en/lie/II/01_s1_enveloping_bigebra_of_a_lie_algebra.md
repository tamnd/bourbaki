---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 1
section_title: Enveloping bigebra of a Lie algebra
lang: en
source: lie-i-iii
pdf_pages: 0129-0140, 0196-0199
extraction: ocr
subsections:
    - "no": 1
      title: PRIMITIVE ELEMENTS OF A COGEBRA
      page: 0
      pdf_page: 129
    - "no": 2
      title: PRIMITIVE ELEMENTS OF A BIGEBRA
      page: 0
      pdf_page: 131
    - "no": 3
      title: FILTERED BIGEBRAS
      page: 0
      pdf_page: 132
    - "no": 4
      title: ENVELOPING BIGEBRA OF A LIE ALGEBRA
      page: 0
      pdf_page: 133
    - "no": 5
      title: STRUCTURE OF THE COGEBRA U(g) IN CHARACTERISTIC 0
      page: 0
      pdf_page: 134
    - "no": 6
      title: STRUCTURE OF FILTERED BIGEBRAS IN CHARACTERISTIC 0
      page: 0
      pdf_page: 137
statements: 24
exercises: 11
content_sha256: 2809a9ef30dc6d5e712bfdcb8c630966d7bcdf41020c5af1ebbaf978ef021eac
---

## § 1. ENVELOPING BIGEBRA OF A LIE ALGEBRA

Throughout this paragraph, g will denote a Lie algebra over K, U(g) or simply U its enveloping algebra (Chapter I, § 2, no. 1), σ the canonical mapping of g into U(g) (loc. cit.) and (U_n)_{n \geq 0} the canonical filtration of U (loc. cit., no. 6).

### 1. PRIMITIVE ELEMENTS OF A COGEBRA

Throughout this no. we consider a cogebra E (Algebra, Chapter III, § 11, no. 1) with coproduct
$$
c : E \to E \otimes E
$$
and counit ε (loc. cit., no. 2). Recall that ε is a linear form on the K-module E such that (with the canonical identification of E \otimes K and K \otimes E with E):
$$
\mathrm{Id}_E = (\varepsilon \otimes \mathrm{Id}_E) \circ c = (\mathrm{Id}_E \otimes \varepsilon) \circ c.
$$
Let E^+ denote the kernel of ε and let u be an element of E such that
$$
c(u) = u \otimes u \quad \text{and} \quad \varepsilon(u) = 1.
$$

† The results of Chapters II and III depend on the first six books, on Lie groups and Lie Algebras, Chapter I, on Commutative Algebra and on Differentiable and Analytic Manifolds, Summary of Results; no. 9 of § 6 of Chapter III depends also on Spectral Theories, Chapter I.

The K-module E is the direct sum of $ E^+ $ and the submodule $ K.u $ which is free with basis $ u $; let $ \pi_u : E \to E^+ $ and $ \eta_u : E \to K.u $ denote the projectors associated with this decomposition. Then

(1)
$$
\pi_u(x) = x - \varepsilon(x).u, \qquad \eta_u(x) = \varepsilon(x).u.
$$

#### Definition 1 {#lie-ii-s1-def-1 .statement}

*An element $ x $ of $ E $ is called u-primitive if*

(2)
$$
c(x) = x \otimes u + u \otimes x.
$$

The $ u $-primitive elements of $ E $ form a submodule of $ E $, denoted by $ P_u(E) $.

#### Proposition 1 {#lie-ii-s1-prop-1 .statement}

*Every u-primitive element of $ E $ belongs to $ E^+ $.*
(2) implies $ x = \varepsilon(x).u + \varepsilon(u).x = \varepsilon(x).u + x, $ whence $ \varepsilon(x) = 0 $.

#### Remark {#lie-ii-s1-n1-rem-1 .statement}

If $ x \in E $ and $ c(x) = x' \otimes u + u \otimes x'' $, where $ x', x'' $ are in $ E^+ $, then $ x = \varepsilon(x').u + \varepsilon(u).x'' = x'' $; similarly $ x = x' $ and $ x $ is $ u $-primitive.

For all $ x \in E^+ $, we write

(3)
$$
c_u^+(x) = c(x) - x \otimes u - u \otimes x.
$$

#### Proposition 2 {#lie-ii-s1-prop-2 .statement}

*We have*

(4)
$$
(\pi_u \otimes \pi_u) \circ c = c_u^+ \circ \pi_u.
$$

Let $ x $ be in $ E $; then
$$
\begin{align*}
(\pi_u \circ \pi_u)(c(x)) &= ((1 - \eta_u) \otimes (1 - \eta_u))(c(x)) \\
&= c(x) - (1 \otimes \eta_u)(c(x)) - (\eta_u \otimes 1)(c(x)) + (\eta_u \otimes \eta_u)(c(x)).
\end{align*}
$$
As $ \varepsilon $ is counit of $ E $,
$$
(1 \otimes \eta_u)(c(x)) = x \otimes u, \qquad (\eta_u \otimes 1)(c(x)) = u \otimes x
$$
whence
$$
(\eta_u \otimes \eta_u)(c(x)) = (\eta_u \otimes 1)((1 \otimes \eta_u)(c(x))) = \varepsilon(x).u \otimes u;
$$
from this we conclude
$$
(\pi_u \otimes \pi_u)(c(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u.
$$
On the other hand,
$$
c_u^+(\pi_u(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u,
$$
whence formula (4).

As $ E^+ $ is a direct factor submodule of $ E $, $ E^+ \otimes E^+ $ can be identified with a direct factor submodule of $ E \otimes E $. With this identification, $ \pi_u \otimes \pi_u $ is a projector of $ E \otimes E $ onto $ E^+ \otimes E^+ $. By formula (4), $ c_u^+ $ maps $ E^+ $ into $ E^+ \otimes E^+ $ and $ \pi_u $ is a morphism of the cogebras $ (E, c) $ into the cogebras $ (E^+, c_u^+) $.

#### Proposition 3 {#lie-ii-s1-prop-3 .statement}

*If the cogebras* $(E, c)$ *is coassociative* (resp. cocommutative) (*Algebra*, Chapter III, § 11, no. 2), *so is the cogebras* $(E^+, c_u^+)$.

This follows from the following lemma:

#### Lemma 1 {#lie-ii-s1-lem-1 .statement}

*Let* $\pi : E \to E'$ *be a surjective cogebras morphism. If* $E$ *is coassociative* (resp. cocommutative), *so is* $E'$.

Let $B$ be an associative $K$-algebra; the mapping $f \mapsto f \circ \pi$ is an *injective* algebra homomorphism of $\mathrm{Hom}_K(E', B)$ into $\mathrm{Hom}_K(E, B)$. It then suffices to apply Proposition 1 (resp. Proposition 2) of *Algebra*, Chapter III, § 11, no. 2.

### 2. PRIMITIVE ELEMENTS OF A BIGEBRA

Let $E$ be a *bigebra* (*Algebra*, Chapter III, § 11, no. 4), $c$ its coproduct, $\varepsilon$ its counit and $1$ its unit element. As $\varepsilon(1) = 1$ and $c(1) = 1 \otimes 1$, the results of the previous no. can be applied with $u = 1$. The 1-primitive elements of $E$ (no. 1, Definition 1) are simply called *primitive* (cf. *Algebra*, Chapter III; § 11, no. 8), that is the elements $x$ of $E$ such that

$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

We write simply $\pi$, $\eta$, $P(E)$, $c^+$ instead of $\pi_1$, $\eta_1$, $P_1(E)$, $c_1^+$.

#### Proposition 4 {#lie-ii-s1-prop-4 .statement}

*The set* $P(E)$ *of primitive elements of* $E$ *is a Lie subalgebra of* $E$.

If $x, y$ are in $P(E)$, then
$$
\begin{align*}
c(xy) &= c(x)c(y) = (x \otimes 1 + 1 \otimes x)(y \otimes 1 + 1 \otimes y) \\
&= xy \otimes 1 + 1 \otimes xy + x \otimes y + y \otimes x,
\end{align*}
$$
whence
$$
c([x, y]) = [x, y] \otimes 1 + 1 \otimes [x, y].
$$

#### Proposition 5 {#lie-ii-s1-prop-5 .statement}

*Let* $f : E \to E'$ *be a bigebra morphism. If* $x$ *is a primitive element of* $E$, *then* $f(x)$ *is a primitive element of* $E'$ *and the restriction of* $f$ *to* $P(E)$ *is a Lie algebra homomorphism* $P(f) : P(E) \to P(E')$.

Let $c$ (resp. $c'$) be the coproduct of $E$ (resp. $E'$). Since $f$ is a cogebras morphism $c' \circ f = (f \otimes f) \circ c$, whence
$$
\begin{align*}
c'(f(x)) &= (f \otimes f)(c(x)) = (f \otimes f)(x \otimes 1 + 1 \otimes x) \\
&= f(x) \otimes 1 + 1 \otimes f(x),
\end{align*}
$$
for $x$ primitive. Hence $f$ maps $P(E)$ into $P(E')$ and $f([x, y]) = [f(x), f(y)]$ since $f$ is an algebra homomorphism.

#### Remark {#lie-ii-s1-n2-rem-1 .statement}

(1) Let $p$ be a prime number such that $p \cdot 1 = 0$ in $K$. The binomial formula and the congruences $\binom{p}{i} \equiv 0 \pmod{p}$ for $1 \leq i \leq p - 1$ imply that

P(E) is stable under the mapping $ x \mapsto x^p $.

(2) By definition, the diagram

$$
0 \longrightarrow P(E) \longrightarrow E^+ \xrightarrow{c^+} E^+ \otimes E^+
$$

is an exact sequence. If $ K' $ is a commutative ring and $ \rho : K \to K' $ a ring homomorphism, $ \rho^*(E) = E \otimes_K K' $ is a $ K' $-bigebra and the inclusion $ P(E) \to E $ defines a homomorphism of Lie $ K' $-algebras

$$
\alpha : P(E) \otimes_K K' \to P(E \otimes_K K').
$$

If $ K' $ is flat over $ K $ (Commutative Algebra, Chapter I, § 2, no. 3, Definition 2), it follows from loc. cit. that the diagram

$$
0 \longrightarrow P(E) \otimes_K K' \longrightarrow E^+ \otimes_K K' \xrightarrow{c^+ \otimes_K \mathrm{Id}_{K'}} (E^+ \otimes_K K') \otimes_{K'} (E^+ \otimes_K K')
$$

is an exact sequence, which implies that $ \alpha $ is an isomorphism.

### 3. FILTERED BIGEBRAS

#### Definition 2 {#lie-ii-s1-def-2 .statement}

Let $ E $ be a bigebra with coproduct $ c $. A filtration compatible with the bigebra structure on $ E $ is an increasing sequence $ (E_n)_{n \geq 0} $ of submodules of $ E $ such that

$$
\begin{align*}
E_0 &= K.1, \quad E = \bigcup_{n \geq 0} E_n \\
E_m \cdot E_n &\subset E_{m+n} \quad \text{for } m \geq 0, n \geq 0 \\
c(E_n) &\subset \sum_{i+j=n} \operatorname{Im}(E_i \otimes E_j) \quad \text{for } n \geq 0.\dagger
\end{align*}
$$

A bigebra with a filtration compatible with its bigebra structure is called a filtered bigebra.

#### Example {#lie-ii-s1-n3-exa-1 .statement}

Let $ E $ be a graded bigebra (Algebra, Chapter III, § 11, no. 4, Definition 3) and $ (E^n)_{n \geq 0} $ its graduation. We write $ E_n = \sum_{i=0}^n E^i $. The sequence $ (E_n) $ is a filtration compatible with the bigebra structure on $ E $.

#### Proposition 6 {#lie-ii-s1-prop-6 .statement}

Let $ E $ be a filtered bigebra and $ (E_n)_{n \geq 0} $ its filtration. For every integer $ n \geq 0 $, let $ E_n^+ = E_n \cap E^+ $. Then $ E_0^+ = \{0\} $ and

$$
c^+(E_n^+) \subset \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-1}^+) \quad \text{for } n \geq 0.\dagger
$$

As $ E_0 = K.1, E_0^+ = 0 $. If $ x \in E_n, \pi(x) = x - \varepsilon(x).1 $ (formula (1)), whence $ \pi(x) \in E_n^+ $ and $ \pi(E_n) \subset E_n^+ $. It follows that $ \pi \otimes \pi $ maps $ \operatorname{Im}(E_i \otimes E_j) $ into

\dagger If A and B are two submodules of E, we denote by $ \operatorname{Im}(A \otimes B) $ the image of the canonical mapping $ A \otimes B \to E \otimes E $.

Im(E_i^+ \otimes E_j^+) \text{ for } i \geq 0, j \geq 0. \text{ As } c^+ = (\pi \otimes \pi) \circ c \text{ in } E^+ \text{ (no. 1, Proposition 2), by (6)}

$$
c^+(E_n^+) \subset \sum_{i=0}^n \operatorname{Im}(E_i^+ \otimes E_{n-i}^+) = \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-i}^+).
$$

#### Corollary {#lie-ii-s1-n3-cor-1 .statement}

*The elements of* $ E_1^+ $ *are primitive.*
If $ x \in E_1^+ $, then $ c^+(x) = 0 $ by (7), whence (5).

### 4. ENVELOPING BIGEBRA OF A LIE ALGEBRA

Recall that $ g $ denotes a Lie algebra and $ U $ its enveloping algebra, with its canonical filtration $ (U_n)_{n \geq 0} $.

#### Proposition 7 {#lie-ii-s1-prop-7 .statement}

*There exists on the algebra* $ U $ *one and only one coproduct* $ c $ *which makes* $ U $ *into a bigebra such that the elements of* $ \sigma(g) $ *are primitive. The bigebra* $ (U, c) $ *is cocommutative; its counit is the linear form* $ \varepsilon $ *such that the constant term (Chapter I, § 2, no. 1) of every element* $ x $ *of* $ U $ *is* $ \varepsilon(x) . 1 $. *The canonical filtration* $ (U_n)_{n \geq 0} $ *of* $ U $ *is compatible with this bigebra structure.*

(a) Let $ x \in g $; we write $ c_0(x) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x) \in U \otimes U $. If $ x, y $ are in $ g $, then
$$
c_0(x)c_0(y) = (\sigma(x)\sigma(y)) \otimes 1 + 1 \otimes (\sigma(x)\sigma(y)) + \sigma(x) \otimes \sigma(y) + \sigma(y) \otimes \sigma(x),
$$
whence
$$
[c_0(x), c_0(y)] = c_0([x, y]).
$$
By the universal property of $ U $ (Chapter I, § 2, no. 1, Proposition 1), there exists one and only one unital algebra homomorphism
$$
c : U \to U \otimes U
$$
such that $ c(\sigma(x)) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x) $ for $ x \in g $. This proves the uniqueness assertion of Proposition 7.

(b) *We show that* $ c $ *is coassociative.* The linear mappings $ c' $ and $ c'' $ of $ U $ into $ U \otimes U \otimes U $ defined by
$$
c' = (c \otimes \mathrm{Id}_U) \circ c \quad \text{and} \quad c'' = (\mathrm{Id}_U \otimes c) \circ c
$$
are unital algebra homomorphisms which coincide on $ \sigma(g) $ since, for $ a \in \sigma(g) $,
$$
c'(a) = a \otimes 1 \otimes 1 + 1 \otimes a \otimes 1 + 1 \otimes 1 \otimes a = c''(a),
$$
whence the result.

(c) *We show that* $ c $ *is cocommutative.* Let $ \tau $ be the automorphism of $ U \otimes U $ such that $ \tau(a \otimes b) = b \otimes a $ for $ a, b $ in $ U $. The mappings $ \tau \circ c $ and $ c $ of $ U $ into $ U \otimes U $ are unital algebra homomorphisms which coincide on $ \sigma(g) $, whence the result.

(d) *We show that* $ \varepsilon $ *is a counit for* $ c $. The mappings $ (\mathrm{Id}_U \otimes \varepsilon) \circ c $ and (ε ⊗ Id_U) ∘ c, of U into U are unital algebra homomorphisms which coincide with Id_U on σ(g).

(e) We know that U_0 = K . 1, U_n ⊂ U_{n+1}, U = ⋃_{n ≥ 0} U_n and U_n · U_m ⊂ U_{n+m} (Chapter I, § 2, no. 6). Let a_1, ..., a_n be in σ(g). Then

$$
c(a_1 ... a_n) = \prod_{i=1}^n c(a_i) = \prod_{i=1}^n (a_i ⊗ 1 + 1 ⊗ a_i)
$$
$$
= \sum_{i=0}^n \sum_{α ∈ I(i)} (a_{α(1)} ... a_{α(i)}) ⊗ (a_{α(i+1)} ... a_{α(n)}),
$$

where I(i) denotes the set of permutations of {1, n} which are increasing in each of the intervals {1, i} and {i + 1, n}. As U_n is the K-module generated by the products of at most n elements of σ(g), formula (8) implies that the filtration (U_n) is compatible with the bigebra structure of (U, c).

#### Definition 3 {#lie-ii-s1-def-3 .statement}

*The bigebra* (U, c) *is called the* enveloping bigebra *of the Lie algebra* g.

#### Proposition 8 {#lie-ii-s1-prop-8 .statement}

*Let E be a bigebra with coproduct denoted by c_E and let h be a Lie algebra homomorphism of g into P(E)* (no. 2, Proposition 4). *The unital algebra homomorphism f : U → E such that f(σ(x)) = h(x) for all x ∈ g is a bigebra morphism.*

We show that (f ⊗ f) ∘ c = c_E ∘ f. These are two unital algebra homomorphisms of U into E ⊗ E and, for a ∈ σ(g),

$$(f ⊗ f)(c(a)) = f(a) ⊗ 1 + 1 ⊗ f(a) = c_E(f(a))$$

since f(a) ∈ P(E). Similarly if ε_E is the counit of E, ε_E ∘ f is a unital algebra homomorphism U → K which is zero on σ(g) (no. 1, Proposition 1) and therefore coincides with ε.

It follows from Propositions 5 and 8 that the mapping f ↦ f ∘ σ defines a one-to-one correspondence between bigebra homomorphisms U(g) → E and Lie algebra homomorphisms g → P(E).

#### Corollary {#lie-ii-s1-n4-cor-1 .statement}

*Let g_i (i = 1, 2) be a Lie algebra, U(g_i) its enveloping bigebra and σ_i : g_i → U(g_i) the canonical mapping. For every Lie algebra homomorphism h : g_1 → g_2, the unital algebra homomorphism U(h) : U(g_1) → U(g_2) such that U(h) ∘ σ_1 = σ_2 ∘ h (Chapter I, § 2, no. 1) is a bigebra morphism.*

### 5. STRUCTURE OF THE COGEBRA U(g) IN CHARACTERISTIC 0

In this no., K will be assumed to be a field of characteristic 0.

Let S(g) be the symmetric algebra of the vector space g, c_S its coproduct (Algebra, Chapter III, § 11, no. 1, Example 6) and η the canonical isomorphism of the vector space $ S(\mathfrak{g}) $ onto the vector space $ U $ (Chapter I, § 2, no. 7). Recall that if $ x_1, \ldots, x_n $ are in $ \mathfrak{g} $, then

$$
\eta(x_1 \ldots x_n) = \frac{1}{n!} \sum_{\tau \in \mathfrak{S}_n} \sigma(x_{\tau(1)}) \ldots \sigma(x_{\tau(n)}).
$$

In particular, for $ x \in \mathfrak{g} $ and $ n \geq 0 $,

$$
\eta(x^n) = \sigma(x)^n.
$$

Note that by *Algebra*, Chapter III, § 6, no. 1, *Remark 3*, $ \eta $ is the unique linear mapping of $ S(\mathfrak{g}) $ into $ U $ satisfying condition (10).

#### Proposition 9 {#lie-ii-s1-prop-9 .statement}

*For every integer $ n \geq 0 $, let $ U^n $ be the vector subspace of $ U $ generated by the $ \sigma(x)^n $ for $ x \in \mathfrak{g} $.*

(a) *The sequence $ (U^n)_{n \geq 0} $ is a graduation of the vector space $ U $ compatible with its cogebra structure.*

*Let $ U $ be given the graduation $ (U^n) $.*

(b) *The canonical mapping $ \eta : S(\mathfrak{g}) \to U $ is an isomorphism of graded cogebras.*

Let $ x \in \mathfrak{g} $ and $ n \in \mathbf{N} $. Then

$$
c_S(x^n) = c_S(x)^n = (x \otimes 1 + 1 \otimes x)^n = \sum_{i=0}^n \binom{n}{i} x^i \otimes x^{n-i}
$$

since $ c_S $ is an algebra homomorphism. Similarly, by (10),

$$
c(\eta(x^n)) = c(\sigma(x)^n) = c(\sigma(x))^n = (\sigma(x) \otimes 1 + 1 \otimes \sigma(x))^n
$$
$$
= \sum_{i=0}^n \binom{n}{i} \sigma(x)^i \otimes \sigma(x)^{n-i} = \sum_{i=0}^n \binom{n}{i} \eta(x^i) \otimes \eta(x^{n-i}),
$$

whence

$$
(\eta \otimes \eta)(c_S(x^n)) = c(\eta(x^n)).
$$

As the $ x^n $, for $ x \in \mathfrak{g} $ and $ n \in \mathbf{N} $, generate the vector space $ S(\mathfrak{g}) $, $ (\eta \otimes \eta) \circ c_S = c \circ \eta $ and $ \eta $ is a cogebra isomorphism.

On the other hand, formula (10) shows that $ \eta(S^n(\mathfrak{g})) = U^n $, which completes the proof of (a) and (b) taking account of the fact that the graduation of $ S(\mathfrak{g}) $ is compatible with its cogebra structure.

The graduation $ (U^n)_{n \geq 0} $ of $ U $ is called the *canonical graduation*.

#### Corollary {#lie-ii-s1-n5-cor-1 .statement}

*The canonical mapping $ \sigma $ defines an isomorphism of $ \mathfrak{g} $ onto the Lie algebra $ P(U) $ of primitive elements of $ U $.*

As $ c^+ $ is a graded homomorphism of degree 0,

$$
P(U) = \sum_{n \geq 1} (P(U) \cap U^n).
$$

It suffices to prove that if $ n > 1 $ and $ a \in U^n $ is primitive, then $ a = 0 $. Now $ a $ can be written as $ \sum_i \lambda_i a_i^n $, where $ \lambda_i \in K $, $ a_i \in \sigma(g) $. By (12), the term of bi-degree $ (1, n-1) $ in $ c^+(a) $ is $ n \sum_i \lambda_i a_i \otimes a_i^{n-1} $. Hence $ \sum_i \lambda_i a_i \otimes a_i^{n-1} = 0 $. If $ \mu : U \otimes U \to U $ is the linear mapping defined by multiplication on $ U $, then
$$
a = \sum_i \lambda_i a_i^n = \mu \left( \sum_i \lambda_i a_i \otimes a_i^{n-1} \right) = 0.
$$

#### Remark {#lie-ii-s1-n5-rem-1 .statement}

(1) $ U_n = \sum_{i=0}^n U^i $ (Chapter I, § 2, no. 7, Corollary 4 to Theorem 1).

(2) The mapping $ \eta $ is the unique morphism of graded cogebras of $ S(g) $ into $ U $ such that $ \eta(1) = 1 $ and $ \eta(x) = \sigma(x) $ for $ x \in g $. For if $ \eta' $ is a morphism satisfying these conditions, we prove by induction on $ n $ that $ \eta'(x^n) = \eta(x^n) $ for $ x \in g $ and $ n > 1 $. As $ c_S^+(x^n) = \sum_{i=1}^{n-1} \binom{n}{i} x^i \otimes x^{n-i} $ by (3) and (11),
$$
(\eta \otimes \eta)(c_S^+(x^n)) = (\eta' \otimes \eta')(c_S^+(x^n))
$$
by the induction hypothesis. It follows that $ c^+(\eta(x^n)) = c^+(\eta'(x^n)) $; it follows that $ \eta(x^n) - \eta'(x^n) $ is a primitive element of degree $ n $ and hence is zero (Corollary to Proposition 9).

(3) Let $ \psi $ be the canonical isomorphism of the bigebra $ TS(g) $ onto the bigebra $ S(g) $ (Algebra, Chapter IV, § 5, Corollary 1 to Proposition 12). The mapping
$$
\eta \circ \psi : TS(g) \to U
$$
is called canonical. It is the unique morphism $ \eta' $ of graded cogebras of $ TS(g) $ into $ U $ such that $ \eta'(1) = 1 $ and $ \eta'(x) = \sigma(x) $ for all $ x \in g $.

(4) Let $ V $ be a vector space. The primitive elements of the bigebra $ S(V) $ are the elements of degree 1. This follows from the Corollary to Proposition 9 applied to the commutative Lie algebra $ V $.

Let $ (e_i)_{i \in I} $ be a basis of the vector $ K $-space $ g $, where the indexing set $ I $ is totally ordered. For all $ \alpha \in \mathbf{N}^{(I)} $, we write
$$
e_\alpha = \prod_{i \in I} \frac{\sigma(e_i)^{\alpha(i)}}{\alpha(i)!}.
$$
The $ e_\alpha $, for $ |\alpha| \leq n $, form a basis of the vector $ K $-space $ U_n $ (Chapter I, § 2, no. 7, Corollary 3 to Theorem 1). Then
$$
e_0 = 1, \quad e_{e_i} = \sigma(e_i) \quad \text{for } i \in I.
$$

As the graded algebra associated with the filtered algebra U is commutative (loc. cit., Theorem 1), for $ \alpha, \beta $ in $ \mathbf{N}^{(\Omega)} $,

$$
e_{\alpha} \cdot e_{\beta} \equiv ((\alpha, \beta)) \cdot e_{\alpha + \beta} \mod U_{|\alpha| + |\beta| - 1}.
$$

where

$$
((\alpha, \beta)) = \prod_{i \in I} \frac{(\alpha(i) + \beta(i))!}{\alpha(i)! \beta(i)!}.
$$

On the other hand, we have immediately

$$
\varepsilon(e_0) = 1, \quad \varepsilon(e_{\alpha}) = 0 \quad \text{for } |\alpha| \geq 1.
$$

Finally, formula (12) implies that, for $ \alpha \in \mathbf{N}^{(\Omega)} $,

$$
c(e_{\alpha}) = \sum_{\beta + \gamma = \alpha} e_{\beta} \otimes e_{\gamma}.
$$

This formula allows us to determine the algebra $ U' = \mathrm{Hom}(U, K) $ dual to the cogebra U (Algebra, Chapter III, § 11, no. 2). For let $ K[[X_i]]_{i \in I} $ be the algebra of formal power series in indeterminates $ (X_i)_{i \in I} $ (cf. Algebra, Chapter III, § 2, no. 11); if $ \lambda \in U' $, let $ f_{\lambda} $ denote the formal power series

$$
f_{\lambda} = \sum_{\alpha} \langle \lambda, e_{\alpha} \rangle X^{\alpha}, \quad \text{where } X^{\alpha} = \prod_{i \in I} X_i^{\alpha(i)}
$$

and the summation index $ \alpha $ runs through $ \mathbf{N}^{(\Omega)} $.

#### Proposition 10 {#lie-ii-s1-prop-10 .statement}

*The mapping* $ \lambda \mapsto f_{\lambda} $ *is an isomorphism of the algebra* $ U' $ *onto the algebra of formal power series* $ K[[X_i]]_{i \in I} $.

Because $ (e_{\alpha}) $ is a basis of U, the mapping $ \lambda \mapsto f_{\lambda} $ is K-linear and bijective. On the other hand, for $ \lambda, \mu $ in $ U' $,

$$
\begin{align*}
f_{\lambda \mu} &= \sum_{\alpha} \langle \lambda \mu, e_{\alpha} \rangle X^{\alpha} = \sum_{\alpha} \langle \lambda \otimes \mu, c(e_{\alpha}) \rangle X^{\alpha} \\
&= \sum_{\alpha} \langle \lambda \otimes \mu, \sum_{\beta + \gamma = \alpha} e_{\beta} \otimes e_{\gamma} \rangle X^{\alpha} \tag{by (16)} \\
&= \sum_{\beta, \gamma} \langle \lambda, e_{\beta} \rangle \langle \mu, e_{\gamma} \rangle X^{\beta + \gamma} = f_{\lambda} f_{\mu},
\end{align*}
$$

which shows that $ \lambda \mapsto f_{\lambda} $ is an *algebra* isomorphism and completes the proof.

### 6. STRUCTURE OF FILTERED BIGEBRAS IN CHARACTERISTIC 0

In this no. we continue to assume that K is a *field of characteristic 0*.

If E is a bigebra, the canonical injection $ P(E) \to E $ can be extended to a bigebra morphism $ f_E : U(P(E)) \to E $ (no. 4, Proposition 8).

#### Theorem 1 {#lie-ii-s1-thm-1 .statement}

Let E be a cocommutative bigebra.
(a) The bigebra morphism $ f_E : U(P(E)) \to E $ is injective.
(b) If there exists on E a filtration compatible with its bigebra structure (no. 3, Definition 2), the morphism $ f_E $ is an isomorphism.
(In case (b), the bigebra E is therefore identified with the enveloping bigebra of the Lie algebra of its primitive elements.)
Let $ c_E $ (resp. $ \varepsilon_E $) be the coproduct (resp. counit) of E. We write $ g = P(E) $; let $ (e_i)_{i \in I} $ be a basis of the vector K-space g, where the indexing set I is totally ordered, and let $ (e_\alpha)_{\alpha \in \mathbf{N}^{(1)}} $ be the basis introduced in the preceding no. We write $ X_\alpha = f_E(e_\alpha) $ for $ \alpha \in \mathbf{N}^{(1)} $. By (15) and (16), we have:
$$
\varepsilon_E(X_0) = 1, \quad \varepsilon_E(X_\alpha) = 0 \quad \text{for } |\alpha| \geq 1,
$$
$$
c_E(X_\alpha) = \sum_{\beta + \gamma = \alpha} X_\beta \otimes X_\gamma \quad \text{for } \alpha \in \mathbf{N}^{(1)},
$$
since $ f_E $ is a cogebra morphism.
We show that $ f_E $ is injective. This results from the following lemma:

#### Lemma 2 {#lie-ii-s1-lem-2 .statement}

Let V be a vector space, E a cogebra and $ f : S(V) \to E $ a cogebra morphism. If the restriction of f to $ S^0(V) + S^1(V) $ is injective, then f is injective.
Let $ n \geq 0 $; we write $ S_n = \sum_{i \geq n} S^i(V) $ and $ c_S $ for the coproduct of $ S(V) $ and show by induction on n that $ f | S_n $ is injective. Since the assertion is trivial for $ n = 0 $ and $ n = 1 $, we assume that $ n \geq 2 $ and let $ u \in S_n $ be such that $ f(u) = 0 $. Then
$$
0 = c_E(f(u)) = (f \otimes f)(c_S(u))
= f(u) \otimes 1 + 1 \otimes f(u) + (f \otimes f)(c_S^+(u))
= (f \otimes f)(c_S^+(u)).
$$
As $ c_S^+(u) \in S_{n-1} \otimes S_{n-1} $, by (11) the induction hypothesis shows that u is a primitive element of $ S(V) $, hence is of degree 1 (no. 5, Remark 4) and hence is zero, since $ f | S^1(V) $ is injective.
It follows in particular that the family $ (X_\alpha) $ is free.
We show that $ f_E $ is surjective if E has a filtration compatible with its bigebra structure. Let $ (E_n)_{n \geq 0} $ be such a filtration and write $ E_n^+ = E_n \cap \mathrm{Ker}(\varepsilon_E) $. We show by induction on n that $ E_n^+ $ is contained in the image of $ f_E $. As $ E = K.1 + \bigcup_{n \geq 0} E_n^+ $, this will imply the surjectivity of $ f_E $. The assertion is trivial for $ n = 0 $ and follows from the Corollary to Proposition 6 of no. 3 for $ n = 1 $; suppose henceforth that $ n \geq 2 $ and let $ x \in E_n^+ $. By Proposition 6 of no. 3,
$$
c_E^+(x) \in \sum_{i=1}^{n-1} E_i^+ \otimes E_{n-i}^+
$$

and by the induction hypothesis there exist scalars $ \lambda_{\alpha, \beta} $, where $ \alpha, \beta $ are in $ \mathbf{N}^{(\Omega)} $, which are zero except for a finite number, such that

(19)
$$
c_E^+ (x) = \sum_{\alpha, \beta \neq 0} \lambda_{\alpha, \beta} X_\alpha \otimes X_\beta.
$$

Hence by formula (18)

$$
(c_E^+ \otimes \mathrm{Id}_E)(c_E^+ (x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha + \beta, \gamma} X_\alpha \otimes X_\beta \otimes X_\gamma
$$
$$
(\mathrm{Id}_E \otimes c_E^+)(c_E^+ (x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha, \beta + \gamma} X_\alpha \otimes X_\beta \otimes X_\gamma.
$$

By Proposition 3 of no. 1 and the linear independence of the $ X_\alpha $ it follows that

(20)
$$
\lambda_{\alpha + \beta, \gamma} = \lambda_{\alpha, \beta + \gamma} \quad \text{for } \alpha, \beta, \gamma \text{ in } \mathbf{N}^{(\Omega)} - \{0\}.
$$

On the other hand, the coproduct $ c_E $ is cocommutative; the same argument as above implies

(21)
$$
\lambda_{\alpha, \beta} = \lambda_{\beta, \alpha} \quad \text{for } \alpha, \beta \text{ in } \mathbf{N}^{(\Omega)} - \{0\}.
$$

Suppose that there exists a family of scalars $ (\mu_\alpha) $ with $ |\alpha| \geq 2 $, such that

(22)
$$
\mu_{\alpha + \beta} = \lambda_{\alpha, \beta} \quad \text{for } \alpha, \beta \text{ in } \mathbf{N}^{(\Omega)} - \{0\}.
$$

Then
$$
c_E^+ (x) = \sum_{\alpha, \beta \neq 0} \mu_{\alpha + \beta} X_\alpha \otimes X_\beta = \sum_{|\gamma| \geq 2} \mu_\gamma c_E^+ (X_\gamma)
$$
by formula (18), hence $ y = x - \sum_{|\gamma| \geq 2} \mu_\gamma X_\gamma $ is primitive and hence belongs to $ P(E) \subset \mathrm{Im}(f_E) $. Hence
$$
x = y + \sum_{|\gamma| \geq 2} \mu_\gamma f_E(e_\gamma) \in \mathrm{Im}(f_E).
$$

The proof will therefore be complete when we have proved the following lemma:

#### Lemma 3 {#lie-ii-s1-lem-3 .statement}

*If a family of scalars* $ (\lambda_{\alpha, \beta}) $ *of finite support* (with $ \alpha, \beta $ in $ \mathbf{N}^{(\Omega)} - \{0\} $) *satisfies relations* (20) *and* (21), *there exists a family* $ (\mu_\alpha)_{|\alpha| \geq 2} $ *of finite support such that* $ \mu_{\alpha + \beta} = \lambda_{\alpha, \beta} $ *for* $ \alpha, \beta $ *non-zero*.

It suffices to prove that

(23)
$$
\alpha + \beta = \gamma + \delta
$$

implies $ \lambda_{\alpha, \beta} = \lambda_{\gamma, \delta} $ for $ \alpha, \beta, \gamma, \delta $ non-zero. By Riesz's Decomposition Lemma (*Algebra*, Chapter VI, § 1, no. 10, Theorem 1) there exist $ \pi, \rho, \sigma, \tau $ in $ \mathbf{N}^{(\Omega)} $ such that
$$
\alpha = \pi + \sigma, \qquad \beta = \rho + \tau, \qquad \gamma = \pi + \rho, \qquad \delta = \sigma + \tau.
$$

Suppose $ \pi \neq 0 $; as $ \sigma + \beta = \rho + \delta $, relation (20) implies
$$
\lambda_{\alpha, \beta} = \lambda_{\pi + \sigma, \beta} = \lambda_{\pi, \sigma + \beta} = \lambda_{\pi, \rho + \delta} = \lambda_{\pi + \rho, \delta} = \lambda_{\gamma, \delta}.
$$
If on the other hand $ \pi = 0 $, then $ \beta = \gamma + \tau $ and $ \delta = \alpha + \tau $, whence
$$
\lambda_{\alpha, \beta} = \lambda_{\alpha, \gamma + \tau} = \lambda_{\alpha + \tau, \gamma} = \lambda_{\delta, \gamma}
$$
by (20), but also $ \lambda_{\delta, \gamma} = \lambda_{\gamma, \delta} $ by (21), whence $ \lambda_{\alpha, \beta} = \lambda_{\gamma, \delta} $.

### Exercises {#lie-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
