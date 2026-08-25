---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 6
section_title: Semi-simple Lie algebras
lang: en
source: lie-i-iii
pdf_pages: 0068-0086, 0120-0127
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 68
    - "no": 2
      title: SEMI-SIMPLICITY OF REPRESENTATIONS
      page: 0
      pdf_page: 69
    - "no": 3
      title: SEMI-SIMPLE ELEMENTS AND NILPOTENT ELEMENTS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 72
    - "no": 4
      title: REDUCTIVE LIE ALGEBRAS
      page: 0
      pdf_page: 74
    - "no": 5
      title: 'APPLICATION: A CRITERION FOR SEMI-SIMPLICITY OF REPRESENTATIONS'
      page: 0
      pdf_page: 76
    - "no": 6
      title: SUBALGEBRAS REDUCTIVE IN A LIE ALGEBRA
      page: 0
      pdf_page: 77
    - "no": 7
      title: EXAMPLES OF SEMI-SIMPLE LIE ALGEBRAS
      page: 0
      pdf_page: 78
    - "no": 8
      title: THE LEVI-MALCEV THEOREM
      page: 0
      pdf_page: 80
    - "no": 9
      title: THE INVARIANTS THEOREM
      page: 0
      pdf_page: 84
    - "no": 10
      title: CHANGE OF BASE FIELD
      page: 0
      pdf_page: 86
statements: 50
exercises: 27
content_sha256: ca11fbca171ac7274c26c58ce41a90b0164cd00d1507e007fcd9d059503138a2
---

## § 6. SEMI-SIMPLE LIE ALGEBRAS

*Recall that K denotes a field of characteristic 0 and that all Lie algebras are assumed to be finite-dimensional over K.*

### 1. DEFINITION OF SEMI-SIMPLE LIE ALGEBRAS

#### Definition 1 {#lie-i-s6-def-1 .statement}

*Let g be a Lie algebra. g is called semi-simple if and only if the only commutative ideal of g is {0}.*

#### Remark {#lie-i-s6-n1-rem-1 .statement}

(1) The algebra {0} is semi-simple. An algebra of dimension 1 or 2 is not semi-simple (cf. § 5, no. 1, Example 1). There exist semi-simple algebras of dimension 3 (cf. no. 7).

(2) A semi-simple algebra has zero centre and hence its adjoint representation is faithful.

(3) If $ g_1, \ldots, g_n $ are semi-simple, $ g = g_1 \times \cdots \times g_n $ is semi-simple: for if a is a commutative ideal of g, the projections of a onto $ g_1, \ldots, g_n $ reduce to {0}.

#### Theorem 1 {#lie-i-s6-thm-1 .statement}

*Let g be a Lie algebra. The following conditions are equivalent:*

(a) *g is semi-simple.*
(b) *The radical r of g is zero.*
(c) *The Killing form $ \beta $ of g is non-degenerate.*

*Moreover, a semi-simple Lie algebra is equal to its derived ideal.*

(a) $ \Rightarrow $ (b): for if $ r \neq \{0\} $, the last non-zero derived algebra of r is a commutative ideal of g.

(b) $ \Rightarrow $ (c): this follows from Proposition 5 (b) of § 5, no. 5 (which at the same time proves the last assertion of the theorem).

(c) $ \Rightarrow $ (a): this follows from Proposition 6 (b) of § 4, no. 4.

#### Corollary {#lie-i-s6-n1-cor-1 .statement}

*Let g be a semi-simple Lie algebra and $ \rho $ a representation of g on a finite-dimensional vector space V. Then $ \rho(g) \subset \mathfrak{sl}(V) $.*

The linear form $ x \mapsto \operatorname{Tr} \rho(x) $ ($ x \in g $) is zero when x is of the form $[y, z]$ ($ y \in g, z \in g $) and hence on $ \mathcal{D}g = g $.

#### Proposition 1 {#lie-i-s6-prop-1 .statement}

Let $ g $ be a semi-simple Lie algebra and $ \varphi $ a finite-dimensional faithful representation of $ g $. Then the bilinear form on $ g $ associated with $ \varphi $ is non-degenerate.

The orthogonal of $ g $ with respect to this form is a solvable ideal ($ \S 5 $, no. 4, Theorem 2) and hence is zero.

#### Corollary 1 {#lie-i-s6-prop-1-cor-1 .statement}

Let $ g $ be a Lie algebra, $ \beta $ its Killing form and $ a $ a semi-simple sub-algebra of $ g $. The orthogonal $ h $ of $ a $ with respect to $ \beta $ is a supplementary subspace of $ a $ in $ g $ and $[a, h] \subset h$. If $ a $ is an ideal of $ g $, so is $ h $, which is then the centralizer of $ a $ in $ g $.

Let $ \beta' $ be the restriction of $ \beta $ to $ a $: it is the bilinear form associated with the representation $ x \mapsto \operatorname{ad}_g x $ of $ a $ on the space $ g $. This representation is faithful and hence $ \beta' $ is non-degenerate (Proposition 1). Hence $ h $ is supplementary to $ a $ in $ g $. On the other hand, if $ x, y $ are in $ a $ and $ z \in h $, then

$$
\beta(x, [y, z]) = \beta([x, y], z) = 0,
$$

since $[x, y] \in a$, and hence $[y, z] \in h$, which proves that $[a, h] \subset h$. If $ a $ is an ideal of $ g $, we know that $ h $ is an ideal of $ g $ ($ \S 3 $, Proposition 7) and $ g $ is identified with $ a \times h $. As the centre of $ a $ is zero, the centralizer of $ a $ in $ g $ is $ h $.

#### Corollary 2 {#lie-i-s6-prop-1-cor-2 .statement}

Every extension of a semi-simple Lie algebra by a semi-simple Lie algebra is semi-simple and trivial.

This follows immediately from Corollary 1.

#### Corollary 3 {#lie-i-s6-prop-1-cor-3 .statement}

If $ g $ is semi-simple, every derivation of $ g $ is inner.

$ \operatorname{ad} g $ is isomorphic to $ g $ and hence semi-simple and is an ideal of the Lie algebra $ \delta $ of derivations of $ g $ ($ \S 1 $, Proposition 1). If $ D \in \delta $ commutes with the elements of $ \operatorname{ad} g $, then, for all $ x \in g $, $ \operatorname{ad} D(x) = [D, \operatorname{ad} x] = 0 $, whence $ D(x) = 0 $; hence $ D = 0 $. Corollary 3 then follows from Corollary 1.

### 2. SEMI-SIMPLICITY OF REPRESENTATIONS

#### Lemma 1 {#lie-i-s6-lem-1 .statement}

Let $ g $ be a semi-simple Lie algebra. The adjoint representation of $ g $ is semi-simple. Every ideal and every quotient algebra of $ g $ is semi-simple.

Let $ a $ be an ideal of $ g $. The orthogonal $ b $ of $ a $ in $ g $ with respect to the Killing form is an ideal of $ g $ and $ a \cap b $ is a commutative ideal ($ \S 3 $, no. 6, Proposition 7) and hence zero. Hence $ b $ is supplementary to $ a $ in $ g $. Moreover, as the Killing form of $ g $ is non-degenerate, so are its restrictions to $ a $ and $ b $ (*Algebra*, Chapter IX, $ \S 4 $, no. 1, Corollary to Proposition 1) and hence $ a $ and $ b $ are semi-simple (no. 1, Theorem 1 and $ \S 3 $, no. 6, Proposition 9).

#### Lemma 2 {#lie-i-s6-lem-2 .statement}

Let $ g $ be a Lie algebra. Then the following two conditions are equivalent:
(a) All finite-dimensional linear representations of $ g $ are semi-simple.
(b) Given a linear representation $ \varphi $ of $ g $ on a finite-dimensional vector space $ V $ and a vector subspace W of codimension 1 such that $ \rho(x)(V) \subset W $ for all $ x \in g $, there exists a supplementary line of W which is stable under $ \rho(g) $ (and hence annihilated by $ \rho(g) $).

Clearly (a) implies (b). Suppose that (b) holds. Let $ \sigma $ be a finite-dimensional representation of $ g $ on a vector space M and N a vector subspace which is stable under $ \sigma(g) $. Let $ \mu $ be the representation of $ g $ on $ \mathcal{L}(M) $ canonically derived from $ \sigma $ (\S 3, no. 3): recall that $ \mu(x) = \mathrm{ad}_{\mathcal{L}(M)} \rho(x) $. Let V (resp. W) be the subspace of $ \mathcal{L}(M) $ consisting of the linear mappings of M into N whose restriction to N is a homothety (resp. zero); then W is of codimension 1 in V and $ \mu(x)(V) \subset W $ for all $ x \in g $. By condition (b), there exists $ u \in V $ which is annihilated by $ \mu(x) $ for all $ x \in g $ and whose restriction to N is a non-zero homothety. By multiplying $ u $ by a suitable scalar, it can be assumed that $ u $ is a projector of M onto N. To say that $ \mu(x) \cdot u = 0 $ means that $ u $ is permutable with $ \sigma(x) $. Hence the kernel of $ u $ is a supplement of N in M which is stable under $ \sigma(x) $ for all $ x \in g $. Hence $ \sigma $ is semi-simple.

#### Lemma 3 {#lie-i-s6-lem-3 .statement}

*Let g be a semi-simple Lie algebra, $ \rho $ a linear representation of g on a finite-dimensional vector space V and W a subspace of V of codimension 1 such that $ \rho(x)(V) \subset W $ for all $ x \in g $. Then there exists a supplementary line of W which is stable under $ \rho(g) $.*

For all $ x \in g $ let $ \sigma(x) $ be the restriction of $ \rho(x) $ to W. Suppose first that $ \sigma $ is simple. If $ \sigma = 0 $, then $ \rho(x)\rho(y) = 0 $ for all $ x, y $ in $ g $, hence $ \rho(g) = \rho(\mathcal{D}g) = \{0\} $ and our assertion is obvious. If $ \sigma \neq 0 $, let n be the kernel of $ \sigma $ and let m be a supplementary ideal of n in $ g $ (Lemma 1); then $ m \neq \{0\} $ and the restriction of $ \sigma $ to m is faithful; the restriction to m of the bilinear form associated with $ \sigma $ is non-degenerate (Proposition 1) and hence the Casimir element c associated with m and $ \sigma $ can be formed. By Proposition 12 of \S 3, no. 7, $ \sigma(c) $ is an automorphism of W. On the other hand, $ \rho(c)(V) \subset W $. Hence the kernel Z of $ \rho(c) $ is a supplementary line of W; since c belongs to the centre of the enveloping algebra of $ g $, $ \rho(c) $ is permutable with $ \rho(x) $ for all $ x \in g $ and hence Z is stable under $ \rho(g) $.

In the general case we argue by induction on the dimension of V. Let T be a minimal non-zero stable subspace of W. Let $ \rho' $ be the quotient representation on $ V' = V/T $. Then, for all $ x \in g $, $ \rho'(x)(V') \subset W' $, where $ W' = W/T $ is of codimension 1 in $ V' $. By the induction hypothesis there exists a line $ Z' $ which is supplementary to $ W' $ and stable under $ \rho'(g) $. Its inverse image Z in V is stable under $ \rho(g) $, contains T as subspace of codimension 1, $ Z \cap W = T $, and hence $ \rho(x)(Z) \subset T $ for all $ x \in g $. By what was proved above, there exists a supplementary line of T in Z which is stable under $ \rho(g) $; this line is supplementary to W in V, which completes the proof.

#### Theorem 2 (H. Weyl) {#lie-i-s6-thm-2 .statement}

*Every finite-dimensional linear representation of a semi-simple Lie algebra is completely reducible.*

This follows from Lemmas 2 and 3.

#### Definition 2 {#lie-i-s6-def-2 .statement}

*A Lie algebra g is called simple if the only ideals of g are {0} and g and if further g is non-commutative.*

A simple Lie algebra is semi-simple. The algebra {0} is not simple.

#### Proposition 2 {#lie-i-s6-prop-2 .statement}

*For a Lie algebra g to be semi-simple, it is necessary and sufficient that it be a product of simple algebras.*

The condition is sufficient (no. 1, Remark 3). Conversely, suppose that g is semi-simple. Since the adjoint representation of g is semi-simple, g is the direct sum of minimal non-zero ideals $ a_1, \ldots, a_m $. Then g is identified with the product algebra of the $ a_i $ (\S 1, no. 1). Every ideal of $ a_i $ is then an ideal of g and hence zero or equal to $ a_i $. On the other hand $ a_i $ is non-commutative. Hence the $ a_i $ are simple Lie algebras.

#### Corollary 1 {#lie-i-s6-prop-2-cor-1 .statement}

*A semi-simple Lie algebra is the product of its simple ideals $ g_i $. Every ideal of g is the product of certain of the $ g_i $.*

$ g = a_1 \times \cdots \times a_m $, where the $ a_i $ are simple. As the centre of $ a_i $ is zero, the centralizer of $ a_i $ in g is the product of the $ a_j $ for $ j \neq i $. Then let a be an ideal of g. If it does not contain $ a_i $, then $ a \cap a_i = \{0\} $, hence $[a, a_i] = \{0\}$ and a is contained in the product of the $ a_j $ for $ j \neq i $. It follows that a is the product of certain of the $ a_i $. Hence the simple ideals of g are precisely the $ a_i $.

The simple ideals of a semi-simple Lie algebra are called the *simple components* of g.

#### Corollary 2 {#lie-i-s6-prop-2-cor-2 .statement}

*Let g, $ g' $ be two Lie algebras, r and $ r' $ their radicals and f a homomorphism of g onto $ g' $. Then $ r' = f(r) $.*

As $ f(r) $ is solvable, $ f(r) \subset r' $. On the other hand, $ g/r $ is semi-simple (\S 5, no. 2, Proposition 3), hence $ g'/f(r) $, which is isomorphic to a quotient of $ g/r $, is semi-simple (Lemma 1) and hence $ f(r) \supset r' $ (\S 5, no. 2, Proposition 3).

#### Remark {#lie-i-s6-n2-rem-1 .statement}

(1) Theorem 2 admits a converse: if every finite-dimensional representation of g is semi-simple, g is semi-simple. For since the adjoint representation is semi-simple, every ideal of g admits a supplementary ideal and hence can be considered as a quotient of g. If g is not semi-simple then g admits a non-zero commutative quotient and therefore a quotient of dimension 1. Now the Lie algebra K of dimension 1 admits non-semi-simple representations, for example

$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

(2) Let g be a Lie algebra over K and $ \sigma $ a representation of g on a vector space M. On the other hand let $ f $ be a K-linear mapping of $ g $ into M such that:

$$
f([x, y]) = \sigma(x) \cdot f(y) - \sigma(y) \cdot f(x)
$$

for all $ x, y $ in $ g $. By § 1, no. 8, Example 2, being given $ \sigma $ and $ f $ is equivalent to being given a homomorphism $ x \mapsto (f(x), \sigma(x)) $ of $ g $ into $ \mathfrak{af}(M) $. On the other hand we have seen (loc. cit.) that the element $ (f(x), \sigma(x)) $ of $ \mathfrak{af}(M) $ is canonically identified with the element $ \rho(x) $ of $ \mathfrak{gl}(N) $ (where $ N = M \times K $) which induces $ \sigma(x) $ on M and maps the element $ (0, 1) $ of N to $ f(x) $. And $ \rho $ is then a representation of $ g $ on N such that $ \rho(x)(N) \subset M $ for all $ x \in g $.

Then, if $ g $ is semi-simple, there exists (Lemma 3) a line Z which is supplementary to M in N and annihilated by $ \rho(g) $. In other words, *there exists an element* $ m_0 \in M $ such that $ (-m_0, 1) \in N $ is annihilated by $ \rho(x) $, that is *such that*

$$
f(x) = \sigma(x) \cdot m_0
$$

*for all* $ x \in g $.

*Suppose that $ K = \mathbf{R} $. Let G be a connected Lie group with Lie algebra g. Consider an analytic homomorphism $ \phi $ of G into the affine group A of M corresponding to a homomorphism $ x \mapsto (f(x), \sigma(x)) $ of g into $ \mathfrak{af}(M) $. The above results can be interpreted by saying that if g is semi-simple $ \phi(G) $ leaves a point of M fixed. For let H be the set of elements of $ \mathbf{GL}(N) $ which leave stable all the linear varieties of N parallel to M. There exists (§ 1, no. 8, Example 2) a canonical isomorphism $ \psi $ of A onto H. Let Z be a supplementary line of M in N. To say that $ \rho(g) $ annihilates Z amounts to saying that $ (\psi \circ \phi)(G) $ leaves the points of Z fixed and hence (taking account of the definition of $ \psi $) that $ \phi(G) $ leaves fixed the projection onto M of the point of intersection of Z and $ M \times \{1\} $.*

### 3. SEMI-SIMPLE ELEMENTS AND NILPOTENT ELEMENTS IN SEMI-SIMPLE LIE ALGEBRAS

#### Proposition 3 {#lie-i-s6-prop-3 .statement}

*Let M be a finite-dimensional vector space over K and $ g $ a semi-simple subalgebra of $ \mathfrak{gl}(M) $. Then $ g $ contains the semi-simple and nilpotent components of its elements.*

If $ K_1 $ is an extension of K, the Killing form of $ g_{(K_1)} $ is the extension to $ g_{(K_1)} $ of that of $ g $ (§ 3, no. 8) and hence is non-degenerate; therefore $ g_{(K_1)} $ is semi-simple. It therefore suffices to prove Proposition 3 when the base field is algebraically closed, which we shall henceforth assume to be the case.

For every subspace N of M, let $ g_N $ be the subalgebra of $ \mathfrak{gl}(M) $ consisting of the elements which leave N stable and whose restriction to N has trace zero. As $ g = \mathcal{D}g $, $ g \subset g_N $ if N is stable under $ g $. Then let $ g^* $ be the intersection of the normalizer of $ g $ in $ \mathfrak{gl}(M) $ and the algebras $ g_N $ where N runs through the set of subspaces of M which are stable under g. As the semi-simple (resp. nilpotent) component s (resp. n) of $ x \in gl(M) $ is a polynomial in x with no constant term and ad s (resp. ad n) is the semi-simple (resp. nilpotent) part of ad x ($ \S 5 $, no. 4, Lemma 2), clearly $ x \in g^* $ implies $ s \in g^* $ and $ n \in g^* $; it therefore suffices to show that $ g^* = g $. Since g is a semi-simple ideal of $ g^* $, $ g^* = a \times g $ (no. 1, Corollary 1 to Proposition 1). Let $ a \in a $ and let N be a subspace which is minimal among the non-zero subspaces of M which are stable under g. The restriction of a to N is a scalar multiple of the identity by Burnside’s Theorem, has trace zero by construction and hence is zero since K is of characteristic 0. As M is the direct sum of subspaces such as N, it follows that $ a = 0 $ and hence $ g^* = g $.

#### Corollary {#lie-i-s6-n3-cor-1 .statement}

An element x of g is a semi-simple (resp. nilpotent) endomorphism of M if and only if $ ad_g x $ is a semi-simple (resp. nilpotent) endomorphism of g.

Let s (resp. n) be the semi-simple (resp. nilpotent) component of $ x \in g $. Then $ s \in g $ and $ n \in g $ (Proposition 3). Then $ ad_g s $ (resp. $ ad_g n $) is the semi-simple (resp. nilpotent) component of $ ad_g x $, by Lemma 2 of $ \S 5 $, no. 4. If x is semi-simple (resp. nilpotent) so then is $ ad_g x $. If now $ ad_g x $ is semi-simple (resp. nilpotent), it is equal to $ ad_g s $ (resp. $ ad_g n $) and hence $ x = s $ (resp. $ x = n $) since the adjoint representation of g is faithful.

#### Definition 3 {#lie-i-s6-def-3 .statement}

Let g be a semi-simple Lie algebra. An element x of g is called semi-simple (resp. nilpotent) if, for every g-module M of finite dimension over K, $ x_M $ is a semi-simple (resp. nilpotent) endomorphism of M.

#### Proposition 4 {#lie-i-s6-prop-4 .statement}

Let g, g' be semi-simple Lie algebras and f a homomorphism of g into g'. If $ x \in g $ is semi-simple (resp. nilpotent), so is $ f(x) $. If f is surjective, every semi-simple (resp. nilpotent) element of g' is the image under f of a semi-simple (resp. nilpotent) element of g.

If $ \rho $ is a representation of g', $ \rho \circ f $ is a representation of g, whence the first assertion. If f is surjective, there exists a homomorphism g of g' into g such that $ f \circ g $ is the identity homomorphism of g' (no. 1, Corollary 2 to Proposition 1) and the second assertion then follows from the first.

#### Theorem 3 {#lie-i-s6-thm-3 .statement}

Let g be a semi-simple Lie algebra.

(a) Let $ x \in g $. If there exists a faithful representation $ \rho $ of g such that $ \rho(x) $ is a semi-simple (resp. nilpotent) endomorphism, then x is semi-simple (resp. nilpotent).

(b) Every element of g can be written uniquely as the sum of a semi-simple element and a nilpotent element which commute with one another.

Suppose that the hypothesis of (a) holds. Let $ \sigma $ be a representation of g, b the supplementary ideal of the kernel of $ \sigma $ and $ \alpha $ the projection of g onto b. Then $ ad_g x $ is semi-simple (resp. nilpotent) by the Corollary to Proposition 3 and hence $ ad_b \alpha(x) $ is semi-simple (resp. nilpotent). As $ \sigma(x) = \sigma(\alpha(x)) $, the first assertion follows from the Corollary to Proposition 3. The second result then follows from Proposition 3 applied to a faithful representation.

### 4. REDUCTIVE LIE ALGEBRAS

#### Definition 4 {#lie-i-s6-def-4 .statement}

*A Lie algebra is called reductive if its adjoint representation is semi-simple.*

#### Proposition 5 {#lie-i-s6-prop-5 .statement}

*Let $ g $ be a Lie algebra and $ r $ its radical. The following conditions are equivalent:*
(a) $ g $ is reductive.
(b) $ \mathcal{D}g $ is semi-simple.
(c) $ g $ is the product of a semi-simple algebra and a commutative algebra.
(d) $ g $ has a finite-dimensional representation such that the associated bilinear form is non-degenerate.
(e) $ g $ has a faithful semi-simple finite-dimensional representation.
(f) *The nilpotent radical of $ g $ is zero.*
(g) $ r $ is the centre of $ g $.

(a) $ \Rightarrow $ (b): if the adjoint representation of $ g $ is semi-simple, $ g $ is a direct sum of minimal non-zero ideals $ a_i $ and hence $ g $ is isomorphic to the product of the $ a_i $; and $ a_i $ has no ideals other than $ \{0\} $ and $ a_i $ and hence is simple or commutative of dimension 1. Therefore $ \mathcal{D}g $ is equal to the product of those $ a_i $ which are simple and hence is semi-simple.

(b) $ \Rightarrow $ (c): if $ \mathcal{D}g $ is semi-simple, $ g $ is isomorphic to the product of $ \mathcal{D}g $ by a Lie algebra $ h $ (no. 1, Corollary 1 to Proposition 1); $ h $ is isomorphic to $ g/\mathcal{D}g $ and hence is commutative.

(c) $ \Rightarrow $ (d): let $ g_1 $ and $ g_2 $ be two Lie algebras, $ \rho_i $ a finite-dimensional representation of $ g_i $ and $ \beta_i $ the bilinear form on $ g_i $ associated with $ \rho_i $ ($ i = 1, 2 $); $ \rho_1 $ and $ \rho_2 $ can be considered as representations of $ g = g_1 \times g_2 $; let $ \rho $ be their direct sum. Clearly the bilinear form on $ g $ associated with $ \rho $ is the direct sum of $ \beta_1 $ and $ \beta_2 $ and hence is non-degenerate if $ \beta_1 $ and $ \beta_2 $ are non-degenerate. Then to prove the implication (c) $ \Rightarrow $ (d) it suffices to consider the 2 following cases: (1) $ g $ is semi-simple; then the adjoint representation admits as associated form the Killing form, which is non-degenerate; (2) $ g = K $; then the identity representation of $ g $ on $ K $ has an associated bilinear form which is non-degenerate.

(d) $ \Rightarrow $ (e): let $ \rho $ be a finite-dimensional representation of $ g $ and $ \beta $ the associated bilinear form; by Proposition 4 of § 4, no. 3, there exists a finite-dimensional semi-simple representation $ \sigma $ of $ g $ such that the kernel $ n $ of $ \sigma $ is orthogonal to $ g $ with respect to $ \beta $. If $ \beta $ is non-degenerate, then $ n = \{0\} $ and hence $ \sigma $ is faithful.

(e) $ \Rightarrow $ (f): this is obvious.

(f) $ \Rightarrow $ (g): if the nilpotent radical of $ g $ is zero, $ \mathcal{D}g \cap r $ is zero ($ \S 5 $, no. 3, Theorem 1); as $[g, r] \subset \mathcal{D}g \cap r$, $ r $ is the centre of $ g $.

(g) ⇒ (a): if r is the centre of g, the adjoint representation of g is identified with a representation of g/r, which is a semi-simple Lie algebra (§ 5, no. 2, Proposition 3); this representation is therefore semi-simple (Theorem 2).

#### Remark {#lie-i-s6-n4-rem-1 .statement}

If a Lie algebra g can be decomposed as a product a × b of a commutative Lie algebra a and a semi-simple Lie algebra b, this decomposition is unique. More precisely, the centre of g is equal to the product of the centres of a and b and is hence equal to a. And $ \mathcal{D}g = \mathcal{D}a \times \mathcal{D}b = b $.

#### Corollary {#lie-i-s6-n4-cor-1 .statement}

(a) Every finite product of reductive algebras is a reductive algebra.
(b) If g is a reductive Lie algebra of centre c, every ideal of g is a direct factor, the product of its intersections with c and $ \mathcal{D}g $, and is a reductive Lie algebra.
(c) Every quotient of a reductive Lie algebra is a reductive Lie algebra.

Assertion (a) follows for example from condition (c) of Proposition 5.

Suppose that g is reductive. Let a be an ideal of g. Since the adjoint representation of g is semi-simple, a has a supplementary ideal b and g is identified with a × b. For all $ x \in g $, let $ \rho(x) $ be the restriction of $ \mathrm{ad}_g x $ to a. Then $ \rho $ is a semi-simple representation of g which is zero on b and defines on passing to the quotient the adjoint representation on a. Hence a is reductive. Similarly, g/a and b, which are isomorphic, are reductive. Finally, let d, d' be the centres of a and b; then $ a = d \times \mathcal{D}a, b = d' \times \mathcal{D}b, d \times d' = c, \mathcal{D}a \times \mathcal{D}b = \mathcal{D}g $; hence $ a = (a \cap c) + (a \cap \mathcal{D}g) $.

#### Proposition 6 {#lie-i-s6-prop-6 .statement}

Let g be a Lie algebra, r its radical and s its nilpotent radical.
(a) $ s = [g, r] = \mathcal{D}g \cap r $.
(b) s is the intersection of the orthogonals of g with respect to the bilinear forms associated with the finite-dimensional representations of g.

Clearly $ [g, r] \subset \mathcal{D}g \cap r $. Now $ \mathcal{D}g \cap r = s $ by Theorem 1 of § 5, no. 3. Let $ g' = g/[g, r] $ and f be the canonical homomorphism of g onto $ g' $; then $ f(r) $ is the radical $ r' $ of $ g' $ (Corollary 3 to Proposition 2, no. 2), hence $ [g', r'] = \{0\} $ and $ r' $ is the centre of $ g' $; therefore (Proposition 5) $ g' $ has a finite-dimensional faithful semi-simple representation, whence $ s \subset [g, r] $. This proves (a).

Let t be the intersection of the orthogonals of g with respect to the bilinear forms associated with the finite-dimensional representations of g. Then $ s \subset t $ (§ 4, no. 3, Proposition 4 (d)). On the other hand, $ g/s $ has a finite-dimensional faithful semi-simple representation and hence (Proposition 5) a finite-dimensional representation $ \rho $ such that the associated bilinear form is non-degenerate; considered as a representation of g, $ \rho $ has an associated bilinear form $ \beta $ on g and the orthogonal of g with respect to $ \beta $ is s, whence $ t \subset s $. Hence $ t = s $.

Even if $ s \neq \{0\} $ there may exist non-degenerate symmetric bilinear forms on g (Exercise 18 (c)). Such forms, of course, are not associated with any representation of g.

#### Corollary {#lie-i-s6-n4-cor-2 .statement}

Let $ g, g' $ be Lie algebras, $ s $ (resp. $ s' $) the nilpotent radical of $ g $ (resp. $ g' $) and $ f $ a homomorphism of $ g $ onto $ g' $.
(a) Then $ s' = f(s) $.
(b) $ g' $ is reductive if and only if the kernel of $ f $ contains $ s $.

If $ r, r' $ are the radicals of $ g, g' $, then $ s' = [g', r'] = [f(g), f(r)] = f([g, r]) = f(s) $. Assertion (b) is an immediate consequence of (a).

### 5. APPLICATION: A CRITERION FOR SEMI-SIMPLICITY OF REPRESENTATIONS

#### Theorem 4 {#lie-i-s6-thm-4 .statement}

Let $ g $ be a Lie algebra, $ r $ its radical, $ \rho $ a finite-dimensional representation of $ g $, $ g' = \rho(g) $ and $ r' = \rho(r) $. Then the following conditions are equivalent:
(a) $ \rho $ is semi-simple;
(b) $ g' $ is reductive and its centre consists of semi-simple endomorphisms;
(c) $ r' $ consists of semi-simple endomorphisms;
(d) the restriction of $ \rho $ to $ r $ is semi-simple.

(a) $ \Rightarrow $ (b): if $ \rho $ is semi-simple, $ g' $ is reductive (Proposition 5); the associative algebra generated by 1 and $ g' $ is semi-simple (\emph{Algebra}, Chapter VIII, § 5, no. 1, Proposition 3), hence its centre is semi-simple (\emph{loc. cit.}, § 5, no. 4, Proposition 12) and hence the elements of this centre are semi-simple (\emph{loc. cit.}, § 9, no. 1, Proposition 2).

(b) $ \Rightarrow $ (c): if $ g' $ is reductive, its centre is equal to its radical, that is $ r' $, whence the implication (b) $ \Rightarrow $ (c).

(c) $ \Rightarrow $ (d): suppose that $ r' $ consists of semi-simple endomorphisms. As $ [g', r'] $ consists of nilpotent endomorphisms (no. 4, Proposition 6), $ [g', r'] = \{0\} $. Then the implication (c) $ \Rightarrow $ (d) follows from \emph{Algebra}, Chapter VIII, § 9, no. 2, Theorem 1.

(d) $ \Rightarrow $ (a): let $ s $ be the nilpotent radical of $ g $ and $ \rho' $ the restriction of $ \rho $ to $ r $. The elements of $ \rho(s) $ are nilpotent and hence $ s $ is contained in the largest nilpotency ideal of $ \rho' $. As $ \rho' $ is semi-simple, $ \rho'(s) = \{0\} $ and $ g' $ is reductive (Corollary to Proposition 6), so that $ g' = a' \times r' $ with $ a' $ semi-simple (Proposition 5). Let $ A' $ (resp. $ R' $) be the associative algebra generated by 1 and $ a' $ (resp. $ r' $). It is semi-simple (\emph{Algebra}, Chapter VIII, § 5, no. 1, Proposition 3), hence $ A' \otimes_K R' $ is semi-simple (\emph{loc. cit.}, § 7, no. 6, Corollary 4 to Theorem 3) and hence the associative algebra generated by 1 and $ g' $, which is a quotient of $ A' \otimes_K R' $, is semi-simple, which proves that $ \rho $ is semi-simple.

#### Corollary 1 {#lie-i-s6-thm-4-cor-1 .statement}

Let $ g $ be a Lie algebra and $ \rho $ and $ \rho' $ two finite-dimensional semi-simple representations of $ g $. Then the tensor product of $ \rho $ and $ \rho' $ is semi-simple.

Let $ r $ be the radical of $ g $. For $ x \in r $, $ \rho(x) $ and $ \rho'(x) $ are semi-simple (Theorem 4), hence $ \rho(x) \otimes 1 + 1 \otimes \rho'(x) $ is semi-simple (\emph{Algebra}, Chapter VIII, § 9, Corollary to Theorem 1) and hence the tensor product of $ \rho $ and $ \rho' $ is semi-simple (Theorem 4).

#### Corollary 2 {#lie-i-s6-thm-4-cor-2 .statement}

Let $ g $ be a Lie algebra, $ \rho $ a semi-simple representation of $ g $ on a finite-dimensional vector space $ V $, $ T $ and $ S $ the tensor and symmetric algebras of $ V $ and $ \sigma_T $, $ \sigma_S $ the representations of $ g $ on $ T $ and $ S $ canonically derived from $ \rho $. Then $ \sigma_T $ and $ \sigma_S $ are semi-simple and, more precisely, direct sums of finite-dimensional simple representations.

Let $ T^n $ be the subspace of $ T $ consisting of the homogeneous tensors of order $ n $. This subspace is stable under $ \sigma_T $ and the representation defined by $ \sigma_T $ on $ T^n $ is semi-simple (Corollary 1). Hence the corollary for $ \sigma_T $ and therefore for $ \sigma_S $, which is a quotient representation of $ \sigma_T $.

#### Corollary 3 {#lie-i-s6-thm-4-cor-3 .statement}

Let $ g $ be a Lie algebra and $ \rho $ and $ \rho' $ two finite-dimensional semi-simple representations of $ g $ on spaces $ M $ and $ M' $. Then the representation of $ g $ on $ \mathcal{L}_K(M, M') $ canonically derived from $ \rho $ and $ \rho' $ is semi-simple.

The $ g $-module $ \mathcal{L}_K(M, M') $ is canonically identified with the $ g $-module $ M^* \otimes_K M' $ (\S 3, no. 3, Proposition 4), so that Corollary 3 follows from Corollary 1.

#### Corollary 4 {#lie-i-s6-thm-4-cor-4 .statement}

Let $ g $ be a Lie algebra, $ a $ an ideal of $ g $ and $ \rho $ a semi-simple representation of $ g $.
(a) The restriction $ \rho' $ of $ \rho $ to $ a $ is semi-simple.
(b) If $ \rho $ is simple, $ \rho' $ is a sum of simple representations isomorphic to one another.

Passing to the quotient by the kernel of $ \rho $, $ \rho $ can be assumed to be faithful. Then $ g $ is reductive. Let $ g = g_1 \times g_2 $, where $ g_1 $ is the centre of $ g $ and $ g_2 $ is semi-simple. Then $ a = a_1 \times a_2 $, where $ a_1 \subset g_1 $, $ a_2 \subset g_2 $ and $ a_1 $ is the centre of $ a $. The elements of $ \rho(g_1) $, and in particular those of $ \rho(a_1) $, are semi-simple (Theorem 4) and hence $ \rho' $ is semi-simple (Theorem 4). Hence (a). Assertion (b) follows from (a), using \S 3, no. 1, Corollary to Proposition 1.

### 6. SUBALGEBRAS REDUCTIVE IN A LIE ALGEBRA

#### Definition 5 {#lie-i-s6-def-5 .statement}

Let $ g $ be a Lie algebra and $ h $ a Lie subalgebra of $ g $. $ h $ is called reductive in $ g $ if the representation $ x \mapsto \operatorname{ad}_g x $ of $ h $ is semi-simple.

This representation admits as subrepresentation the adjoint representation of $ h $. Hence, if $ h $ is reductive in $ g $, $ h $ is reductive. On the other hand, to say that a Lie algebra is reductive in itself is equivalent to saying that it is reductive.

#### Proposition 7 {#lie-i-s6-prop-7 .statement}

Let $ g $ be a Lie algebra, $ h $ a subalgebra reductive in $ g $, $ \rho $ a representation of $ g $ on a vector space $ V $ and $ W $ the sum of the finite-dimensional subspaces of $ V $ which are simple $ h $-modules. Then $ W $ is stable under $ \rho(g) $.

Let $ W_0 $ be a finite-dimensional simple sub-$ h $-module of $ V $. We need to prove that $ \rho(x)(W_0) \subset W $ for all $ x \in g $. Let $ M $ denote the vector space $ g $ considered as an $ h $-module by means of the representation $ x \mapsto \operatorname{ad}_g x $ of $ h $ on $ g $. Then $ M \otimes_K W_0 $ is a semi-simple $ h $-module (Corollary 1 to Theorem 4). Let $ \theta $ be the K-linear mapping of $ M \otimes_K W_0 $ into V defined by $ \theta(x \otimes w) = \rho(x)w $. This is an $ \mathfrak{h} $-module homomorphism, for if $ y \in \mathfrak{h} $ then:

$$
\begin{align*}
\theta([y, x] \otimes w + x \otimes \rho(y)w) &= \rho([y, x])w + \rho(x)\rho(y)w \\
&= \rho(y)\rho(x)w = \rho(y)\theta(x \otimes w).
\end{align*}
$$

Hence $ \theta(M \otimes_K W_0) $ is a finite-dimensional semi-simple $ \mathfrak{h} $-module. Hence $ \theta(M \otimes_K W_0) \subset W $, that is $ \rho(x)(W_0) \subset W $ for all $ x \in g $.

#### Corollary 1 {#lie-i-s6-prop-7-cor-1 .statement}

*Let $ g $ be a Lie algebra, $ \mathfrak{h} $ a subalgebra reductive in $ g $ and $ \rho $ a finite-dimensional semi-simple representation of $ g $. Then the restriction of $ \rho $ to $ \mathfrak{h} $ is semi-simple.*

It suffices to consider the case where $ \rho $ is simple. We adopt the notation V, W of Proposition 4. Let $ W_1 $ be a subspace of V minimal among the non-zero subspaces stable under $ \rho(\mathfrak{h}) $. Then $ W_1 \subset W $, hence $ W \neq \{0\} $ and hence $ W = V $.

#### Corollary 2 {#lie-i-s6-prop-7-cor-2 .statement}

*Let $ g $ be a Lie algebra, $ \mathfrak{h} $ a subalgebra reductive in $ g $ and $ \mathfrak{k} $ a subalgebra of $ \mathfrak{h} $ reductive in $ \mathfrak{h} $. Then $ \mathfrak{k} $ is reductive in $ g $.*

The representation $ x \mapsto \mathrm{ad}_g x $ of $ \mathfrak{h} $ on $ g $ is semi-simple and hence its restriction to $ \mathfrak{k} $ is semi-simple (Corollary 1).

### 7. EXAMPLES OF SEMI-SIMPLE LIE ALGEBRAS

#### Proposition 8 {#lie-i-s6-prop-8 .statement}

*Let $ V $ be a finite-dimensional vector space. Then $ \mathrm{gl}(V) $ is reductive. Its centre is the set of homotheties of $ V $, its derived algebra is $ \mathrm{sl}(V) $ and the latter is semi-simple.*

The identity representation of $ \mathrm{gl}(V) $ is simple, hence $ \mathrm{gl}(V) $ is reductive and therefore $ \mathrm{gl}(V) $ is the direct sum of its centre $ c $ and its derived algebra $ \mathcal{D}(\mathrm{gl}(V)) $. The centre $ c $ is the set of homotheties (*Algebra*, Chapter II, § 2, no. 5, Corollary 1 to Proposition 5). Clearly $ \mathcal{D}(\mathrm{gl}(V)) \subset \mathrm{sl}(V) $. As $ \mathrm{sl}(V) \cap c = \{0\} $, $ \mathcal{D}(\mathrm{gl}(V)) = \mathrm{sl}(V) $. Hence $ \mathrm{sl}(V) $ is semi-simple.

#### Example {#lie-i-s6-n7-exa-1 .statement}

We identify $ \mathrm{sl}(K^2) $ with the Lie algebra of matrices of order 2 and trace zero. We write

$$
X = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} \quad Y = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} \quad H = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

Then $ X, Y, H $ form a basis of $ \mathrm{sl}(K^2) $ and

$$
[H, X] = 2X \qquad [H, Y] = -2Y \qquad [X, Y] = H.
$$

As an algebra of dimension 1 or 2 is not semi-simple (no. 1, *Remark 1*), $ \mathrm{sl}(K^2) $ is simple. In fact, $ \mathrm{sl}(V) $ is simple for $ \dim V \geq 2 $, as we shall see later (cf. also Exercises 21 and 24).

#### Proposition 9 {#lie-i-s6-prop-9 .statement}

Let V be a vector space of finite dimension n over K and β a non-degenerate symmetric (resp. alternating) bilinear form on V. Let g be the Lie algebra consisting of the x ∈ gl(V) such that β(xm, m') + β(m, xm') = 0 for all m, m' in V. Then g is reductive; g is even semi-simple except in the case where β is symmetric and n = 2.

For all u ∈ gl(V) let u* denote its adjoint relative to β; then Tr(u) = Tr(u*) by Proposition 7 of Algebra, Chapter IX, § 1, no. 8. The condition

$$
\beta(um, m') + \beta(m, um') = 0
$$

for all m, m' in V means that $ u + u^* = 0 $. In particular, if $ v \in \mathrm{gl}(V) $ then $ (v - v^*)^* = v^* - v $ and hence $ v - v^* \in g $. Then let u be an element of g orthogonal to g with respect to the bilinear form φ associated with the identity representation of g. For all $ v \in \mathrm{gl}(V) $, $ \mathrm{Tr}\,u(v - v^*) = 0 $, hence

$$
\mathrm{Tr}(uv) = \mathrm{Tr}(uv^*) = \mathrm{Tr}(uv^*)^* = \mathrm{Tr}(vu^*) = -\mathrm{Tr}(vu) = -\mathrm{Tr}(uw)
$$

and hence $ \mathrm{Tr}(uw) = 0 $. It follows that $ u = 0 $, so that φ is non-degenerate. Hence g is reductive (Proposition 5). It remains to show that the centre of g is zero (except when β is symmetric and $ n = 2 $). By extending the base field, we can assume that K is algebraically closed.

(a) When β is symmetric, it can be identified with the bilinear form on $ K^n $ with matrix $ I_n $ with respect to the canonical basis (Algebra, Chapter IX, § 6, Corollary 1 to Theorem 1). Under these conditions g is identified with the Lie algebra of skew-symmetric matrices ($ \S 3 $, no. 4, Example 1). Let $ U = (u_{ij}) \in g $; we use the fact that U commutes with the matrix $ (v_{ij}) \in g $ all of whose elements are zero except $ v_{i_0j_0} $ and $ v_{j_0i_0} $ ($ i_0 \neq j_0 $) which are equal respectively to 1 and −1. We find that $ u_{i_0j} = u_{j_0i} = u_{i_0} = u_{j_0} = 0 $ for $ i \neq i_0, j_0 $ and $ j \neq i_0, j_0 $. If $ n > 2 $, there exist, for all distinct indices $ i_0 $ and $ j $, distinct indices i and $ j_0 $ such that $ i \neq i_0, j_0 \neq j, j_0 \neq i_0 $; hence $ u_{i_0j} = 0 $. This proves that an element of the centre of g is zero.

(b) When β is alternating and $ n = 2m $, β can be identified with the bilinear form on $ K^{2m} $ with matrix $ \begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix} $ with respect to the canonical basis (Algebra, Chapter IX, § 5, Corollary 1 to Theorem 1). Under these conditions g is identified with the Lie algebra of matrices of the form $ U = \begin{pmatrix} A & B \\ C & D \end{pmatrix} $ where $ D = -{}^tA $, B and C are symmetric ($ A, B, C, D $ in $ \mathbf{M}_m(K) $) ($ \S 3 $, no. 4, Example 1). We use first the fact that U commutes with the matrix $ \begin{pmatrix} X & 0 \\ 0 & -{}^tX \end{pmatrix} $, where $ X \in \mathbf{M}_m(K) $. Then $ AX = XA, CX = -{}^tXC, XB = -B\cdot{}^tX $; as these equalities must hold for all X, it follows that A is a scalar matrix $ \lambda I_m $. We now use the fact that U commutes with the matrix $ \begin{pmatrix} 0 & Y \\ 0 & 0 \end{pmatrix} $, where

Y is a symmetric matrix of $ \mathbf{M}_m(\mathbf{K}) $. Then $ \lambda Y = YC = CY = 0 $. This proves first that $ \lambda = 0 $. Moreover, for all $ X \in \mathbf{M}_m(\mathbf{K}) $, $ X + {}^tX $ is symmetric and hence $ XC = -{}^tXC $. Using the equation $ CX = -{}^tXC $ obtained above, we see that $ C $ commutes with every element of $ \mathbf{M}_m(\mathbf{K}) $ and hence that $ C $ is a scalar matrix, necessarily zero since $ YC = 0 $. It is similarly shown that $ B = 0 $.

For $ \beta $ symmetric and $ n = 2 $, $ g $ is of dimension 1 and hence commutative. For the other cases cf. Exercises 25 and 26.

### 8. THE LEVI-MALCEV THEOREM

Let E be a complete normed vector space over $ \mathbf{R} $ and $ u $ a continuous endomorphism of E. We have seen (Functions of a real variable, Chapter IV, § 2, no. 6) that the sequence $ \frac{u^n}{n!} $ is summable in $ \mathcal{L}(E) $ and we wrote

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

Now let E be a vector space over the field K and $ u $ a nilpotent endomorphism of E. The series $ \sum_{n=0}^\infty \frac{u^n}{n!} $ has only a finite number of non-zero terms and we can therefore write

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

This definition agrees with the above if $ K = \mathbf{R} $ and if E is complete and normed. If $ v $ is another nilpotent endomorphism of E which commutes with $ u $, then:

$$
e^{u+v} = \left( \sum_{n=0}^\infty \frac{u^n}{n!} \right) \left( \sum_{p=0}^\infty \frac{v^p}{p!} \right) = \sum_{n,p=0}^\infty \frac{u^n v^p}{n! p!}
$$
$$
= \sum_{q=0}^\infty \frac{1}{q!} \left( \sum_{n+p=q} \binom{q}{n} u^n v^p \right) = \sum_{q=0}^\infty \frac{1}{q!} (u+v)^q = e^{u+v}.
$$

In particular, $ e^u e^{-u} = e^{-u} e^u = e^0 = 1 $ and hence $ e^u $ is always an automorphism of E.

If further E is a (not necessarily associative) algebra and $ u $ is a (nilpotent) derivation of E, then $ e^u $ is an automorphism of the algebra E. For if $ x, y \in E $ then

$$
u^p(xy) = \sum_{r+s=p} \binom{p}{r} u^r(x) u^s(y)
$$

for every integer $ p \geqslant 0 $ (Leibniz’s formula). It follows that

$$
e^{u}(xy) = \sum_{p \geqslant 0} \frac{1}{p!} u^p(xy) = \sum_{p \geqslant 0} \sum_{r+s=p} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!}
$$

$$
= \sum_{r,s=0}^{\infty} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!} = e^{u}(x)e^{u}(y)
$$

whence our assertion.

Now let $ g $ be a Lie algebra. If $ x $ belongs to the nilpotent radical of $ g $, the derivation $ \mathrm{ad}_g x $ of $ g $ is nilpotent. We can therefore make the following definition:

#### Definition 6 {#lie-i-s6-def-6 .statement}

*A special automorphism of $ g $ is an automorphism of $ g $ of the form $ e^{\mathrm{ad}\, x} $, where $ x $ is in the nilpotent radical of $ g $.*

Clearly a special automorphism leaves every ideal of $ g $ stable.

#### Definition 7 {#lie-i-s6-def-7 .statement}

*Let $ g $ be a Lie algebra and $ r $ its radical. A Levi subalgebra of $ g $ is any subalgebra of $ g $ supplementary to $ r $.*

A Levi subalgebra is isomorphic to $ g/r $ and hence is semi-simple. As a semi-simple subalgebra has only 0 in common with $ r $, every semi-simple subalgebra $ h $ such that $ g = r + h $ is a Levi subalgebra; consequently the image of a Levi subalgebra under a surjective homomorphism is a Levi subalgebra.

#### Theorem 5 (Levi–Malcev) {#lie-i-s6-thm-5 .statement}

*A Lie algebra $ g $ always has a Levi subalgebra $ s $. Every Levi subalgebra of $ g $ is the image of $ s $ under a special automorphism.*

Let $ r $ denote the radical of $ g $. We first treat two special cases.

(a) $[g, r] = \{0\}$.

By Proposition 5, $ g $ is then the product of its centre $ r $ by $ \mathcal{D}g $ which is semi-simple. Hence $ \mathcal{D}g $ is a Levi subalgebra. Moreover, if $ s' $ is a semi-simple subalgebra, then $ s' = \mathcal{D}s' $ (Theorem 1), hence $ s' \subset \mathcal{D}g $ and $ \mathcal{D}g $ is the unique Levi subalgebra of $ g $.

(b) $[g, r] \neq \{0\}$ and the only ideals of $ g $ contained in $ r $ are $ \{0\} $ and $ r $.

Then $[g, r] = r,\ [r, r] = \{0\}$ and the centre of $ g $ is zero. Let $ M $ (resp. $ N $) be the subspace of $ \mathcal{L}(g) $ consisting of the linear mappings of $ g $ into $ r $ whose restriction to $ r $ is a homothety (resp. zero); $ N $ is therefore of codimension 1 in $ M $. For $ m \in M $, let $ \lambda(m) $ denote the ratio of the homothety of $ r $ defined by $ m $. Let $ \sigma $ be the representation of $ g $ on $ \mathcal{L}(g) $ canonically derived from the adjoint representation; recall that $ \sigma(x).u = [\mathrm{ad}_g x, u] $ for all $ x \in g $ and all $ u \in \mathcal{L}(g) $.

Clearly $ \sigma(x)(M) \subset N $ for all $ x \in g $. Moreover, if $ x \in r, y \in g $ and $ u \in M $, then
$$
(\sigma(x).u)(y) = [x, u(y)] - u([x, y]) = -\lambda(u)[x, y]
$$
since $[r, r] = \{0\}$; and (4) can be written:
$$
(x).u = -\mathrm{ad}(\lambda(u).x).
$$

As the centre of $ g $ is zero, the mapping $ x \mapsto \mathrm{ad}_g x $ defines a bijection $ \phi $ of $ r $ onto a subspace $ P $ of $ \mathcal{L}(g) $. This subspace is stable under $ \sigma(g) $ and contained in $ N $ since $ r $ is a commutative ideal and (5) shows that $ \sigma(x)(M) \subset P $ for $ x \in r $. The representation of $ g $ on $ M/P = V $ derived from $ \sigma $ is therefore zero on $ r $ and defines a representation $ \sigma' $ of the semi-simple algebra $ g/r $ on $ V $. For all $ y \in g/r $, the space $ \sigma'(y)(V) $ is contained in $ N/P $, which is of codimension 1 in $ V $. Consequently (no. 2, Lemma 3) there exists $ u_0 \in M $ such that $ \lambda(u_0) = -1 $ and $ \sigma(x).u_0 \in P $ for all $ x \in g $. The mapping $ x \mapsto \phi^{-1}(\sigma(x).u_0) $ is a linear mapping of $ g $ into $ r $. By (5) its restriction to $ r $ is the identity mapping of $ r $. Hence its kernel is a subspace $ s $ of $ g $ supplementary to $ r $ in $ g $. As $ s $ is the set of $ x \in g $ such that $ \sigma(x).u_0 = 0 $, $ s $ is a subalgebra of $ g $ and therefore a Levi subalgebra of $ g $.

Let $ s' $ be another Levi subalgebra. For all $ x \in s' $, let $ h(x) $ be the unique element of $ r $ such that $ x + h(x) \in s $. Since $ s $ is a subalgebra and $ r $ is commutative, for $ x, y $ in $ s' $:
$$
[x + h(x), y + h(y)] = [x, y] + [x, h(y)] + [h(x), y] \in s
$$
hence
$$
h([x, y]) = (\mathrm{ad}\, x).h(y) - (\mathrm{ad}\, y).h(x).
$$
By Remark 2 of no. 2, there exists $ a \in r $ such that $ h(x) = -[x, a] $ for all $ x \in s' $. Then:
$$
x + h(x) = x + [a, x] = (1 + \mathrm{ad}\, a).x.
$$
As $ r $ is commutative, $ (\mathrm{ad}\, a)^2 = 0 $ and hence $ 1 + \mathrm{ad}\, a = e^{\mathrm{ad}\, a} $. As $ r = [g, r] $, $ e^{\mathrm{ad}\, a} $ is a special automorphism of $ g $. By (6) this special automorphism maps $ s' $ to $ s $.

(c) General case:

We argue by induction on the dimension $ n $ of the radical. There is nothing to prove if $ n = 0 $ and hence it can be assumed that the theorem holds for Lie algebras whose radical is of dimension $ < \dim r $. By (a) it suffices to consider the case where $[g, r] \neq \{0\}$. As $[g, r]$ is nilpotent (no. 4, Proposition 6), its centre $ c $ is $ \neq \{0\} $. Let $ m $ be a minimal non-zero ideal of $ g $ contained in $ c $. If $ m = r $, we have case (b). Therefore let $ m \neq r $ and let $ f $ be the canonical mapping of $ g $ onto $ g' = g/m $. The radical of $ g' $ is $ r' = r/m $. By the induction hypothesis, $ g' $ has a Levi subalgebra $ l' $. Then $ b = f(l') $ is a subalgebra of g containing m such that h/m = h' is semi-simple and hence having m as radical. By the induction hypothesis h = m + s where s is a semi-simple subalgebra. Then the equality g' = r' + h' implies g = r + h = r + m + s = r + s and hence s is a Levi subalgebra of g.

Let s' be another Levi subalgebra of g. Then f(s) and f(s') are two Levi subalgebras of g' and there exists by the induction hypothesis a' ∈ [g', r'] such that e^{ad\alpha'}(f(s')) = f(s). If a ∈ [g, r] is such that f(a) = a', it follows that:

s_1 = e^{ada}(s') \subset m + s = h.

Then s_1 and s are two Levi subalgebras of h and by the induction hypothesis there exists b ∈ m such that e^{adb}(s_1) = s. Hence s = e^{adb}.e^{ada}(s'). Finally, as m is in the centre of [g, r], e^{adb}.e^{ada} = e^{ad(b+a)} and b + a ∈ [g, r], which completes the proof.

#### Corollary 1 {#lie-i-s6-thm-5-cor-1 .statement}

Let s be a Levi subalgebra of g and h a semi-simple subalgebra of g.
(a) There exists a special automorphism of g mapping h onto a subalgebra of s.
(b) h is contained in a Levi subalgebra of g.

Let r be the radical of g and a = h + r, which is a subalgebra of g. Then a/r is semi-simple and r is solvable, hence r is the radical of a and h is a Levi subalgebra of a. On the other hand, a ∩ s = h' is a supplementary subalgebra to r in a and hence also a Levi subalgebra of a. Then there exists (Theorem 5) a ∈ [a, r] such that e^{ada} maps h onto h'. Now a ∈ [g, r]; e^{ada} maps h onto a subalgebra of s and e^{-ada}(s) is a Levi subalgebra of g containing h.

#### Corollary 2 {#lie-i-s6-thm-5-cor-2 .statement}

For a subalgebra h of g to be a Levi subalgebra of g, it is necessary and sufficient that h be a maximal semi-simple subalgebra of g.

This follows immediately from Corollary 1.

#### Corollary 3 {#lie-i-s6-thm-5-cor-3 .statement}

Let g be a Lie algebra and m an ideal of g such that g/m is semi-simple. Then g contains a subalgebra supplementary to m in g. In other words, every extension of a semi-simple Lie algebra is inessential.

Let s be a Levi subalgebra of g (Theorem 5). Its canonical image in g/m is a Levi subalgebra and therefore equal to g/m, hence g = s + m. Then an ideal of s supplementary in s to the ideal m ∩ s is a subalgebra of g supplementary to m in g.

#### Corollary 4 {#lie-i-s6-thm-5-cor-4 .statement}

Let g be a Lie algebra, r its radical, s a Levi subalgebra of g and m an ideal of g. Then m is the direct sum of m ∩ r which is its radical and m ∩ s which is a Levi subalgebra of m.

We know that m ∩ s is the radical of m (§ 5, no. 5, Corollary 3 to Proposition 5). Let h be a Levi subalgebra of m and s' a Levi subalgebra of g containing h (Corollary 1). The algebra m ∩ s' is an ideal of s', is therefore semi-simple, and contains h and is therefore equal to h. Hence m is the direct sum of $ m \cap r $ and $ m \cap s' $. There exists a special automorphism mapping $ s' $ onto $ s $; this automorphism leaves $ r $ and $ m $ invariant; hence $ m $ is the direct sum of $ m \cap r $ and $ m \cap s $ and $ m \cap s $ is a Levi subalgebra of $ m $.

### 9. THE INVARIANTS THEOREM

Let $ g $ be a Lie algebra and $ \rho $ a representation of $ g $ on a vector space $ M $. For every class $ \delta $ of simple representations of $ g $ let $ M_\delta $ be the isotypical component of $ M $ of species $ \delta $. The subspace $ M_0 $ of invariant elements of $ M $ is just $ M_{\delta_0} $, where $ \delta_0 $ denotes the class of the zero representation of $ g $ on a space of dimension 1.

#### Lemma 4 {#lie-i-s6-lem-4 .statement}

*Let $ \rho, \sigma, \tau $ be representations of $ g $ on vector spaces $ M, N, P $. Suppose that we are given a $ K $-bilinear mapping $ (m, n) \mapsto m.n $ of $ M \times N $ into $ P $ such that*

$$
(\rho(x)m).n + m.(\sigma(x)n) = \tau(x)(m.n)
$$

*for all $ m \in M, n \in N, x \in g $.*

(a) *If $ m_0 \in M_0 $, the mapping $ n \mapsto m_0.n $ is a $ g $-module homomorphism.*

(b) *If $ n \in N_\delta $, then $ m_0.n \in P_\delta $.*

(c) *If $ M $ is a (not necessarily associative) algebra and the $ \rho(x) $ are derivations of $ M $, $ M_0 $ is a subalgebra of $ M $ and each $ M_\delta $ is a right and left $ M_0 $-module.*

For $ m_0 \in M_0, n \in N $ and $ x \in g $,

$$
\tau(x)(m_0.n) = m_0.(\sigma(x)n),
$$

whence (a). Assertion (b) follows from (a) (*Algebra*, Chapter VIII, § 3, no. 4, Proposition 10). If $ N = P = M $ and $ \sigma = \tau = \rho $, assertion (b) gives assertion (c) as a special case.

#### Lemma 5 {#lie-i-s6-lem-5 .statement}

*Suppose further that $ \sigma $ and $ \tau $ are semi-simple and hence $ N $ (resp. $ P $) is the direct sum of the $ N_\delta $ (resp. $ P_\delta $). For all $ n \in N $ (resp. $ p \in P $), let $ n^\natural $ (resp. $ p^\natural $) be its component in $ N_0 $ (resp. $ P_0 $). Let $ m_0 \in M_0 $. Then for all $ n \in N $, $ (m_0.n)^\natural = m_0.n^\natural $.*

By linearity it suffices to consider the case where $ n \in N_\delta $. If $ \delta \neq \delta_0 $, $ n^\natural = 0 $ and $ m_0.n \in P_\delta $ (Lemma 4), hence $ (m_0.n)^\natural = 0 = m_0.n^\natural $. If $ \delta = \delta_0 $, $ n^\natural = n $ and $ m_0.n \in P_0 $ (Lemma 4), hence $ (m_0.n)^\natural = m_0.n = m_0.n^\natural $.

#### Theorem 6 {#lie-i-s6-thm-6 .statement}

*Let $ g $ be a Lie algebra, $ V $ a semi-simple $ g $-module of finite dimension over $ K $, $ S $ the symmetric algebra of $ V $ and $ x_S $ the derivation of $ S $ which extends $ x_V $ (so that $ x \mapsto x_S $ is a representation of $ g $ on $ S $).*

(a) *The algebra $ S_0 $ of invariants of $ S $ is generated by a finite number of elements.*

(b) *For every class $ \delta $ of simple representations of $ g $ of finite dimension over $ K $, let $ S_\delta $ be the isotypical component of $ S $ of species $ \delta $. Then $ S_\delta $ is a finitely generated $ S_0 $-module.*

Let $ \overline{S} \subset S $ be the ideal of elements of $ S $ with no constant term. Let $ I $ be the ideal of $ S $ generated by $ S_0 \cap \overline{S} $ and let $ (s_1, s_2, \ldots, s_p) $ be a finite system of generators of the ideal I (Commutative Algebra, Chapter III, § 3). It can be assumed that the s_i belong to S_0 ∩ S̄ and are homogeneous (the x_S preserve degrees and hence each S_δ is a graded submodule). Let S_1 be the subalgebra of S generated by 1 and the s_i. Then S_1 ⊂ S_0. We show that S_1 = S_0. For this we prove that every homogeneous element s of S_0 is in S_1, arguing by induction on the degree n of s. If n = 0, our assertion is obvious. Suppose therefore n > 0 and that our assertion has been proved when the degree of s is < n. As s ∈ I, s = $ \sum_{i=1}^{p} s_i s'_i $, where the s'_i are elements of S which can be assumed to be homogeneous, with deg(s'_i) = deg(s) − deg(s_i) < n. Lemma 5 can be applied, as the g-module S is semi-simple (no. 5, Corollary 2 to Theorem 4); in the notation of this lemma,

$$
s = s^{\natural} = \sum_{i=1}^{p} (s_i s'_i)^{\natural} = \sum_{i=1}^{p} s_i {s'_i}^{\natural}.
$$

The {s'_i}^{\natural} are elements of S_0 which are homogeneous and of degree < n (since each S_δ is a graded submodule). Hence they are in S_1 by the induction hypothesis. Hence s ∈ S_1, which proves (a).

We now consider a simple representation of g of class δ on a finite-dimensional space M. Let L = $ \mathcal{L}_K(M, S) $. For all s ∈ S and all f ∈ L, let sf be the element of L defined by (sf)(m) = s.f(m) (m ∈ M); an S-module structure is thus defined on L; as M is finite-dimensional over K, clearly L is a finitely generated S-module and hence a Noetherian S-module since the ring S is Noetherian. On the other hand, L has a canonical g-module structure. For every integer n ≥ 0 let S^n be the set of homogeneous elements of S of degree n; then the g-module $ \mathcal{L}_K(M, S^n) $ is semi-simple (no. 5, Corollary 3 to Theorem 4) and hence the g-module L is semi-simple. Moreover, for s ∈ S, f ∈ L, x ∈ g and m ∈ M,

$$
(x_L(sf))(m) = x_S((sf)(m)) - (sf)(x_M m)
= x_S(s.f(m)) - s.f(x_M m)
= (x_S s).f(m) + s.(x_S f(m)) - s.f(x_M m)
= ((x_S s)f)(m) + (s(x_L f))(m)
$$

and hence $ x_L(sf) = (x_S s)f + s(x_L f) $. We can therefore apply Lemma 5.

The subset L_0 of invariant elements of L is just the set of homomorphisms of the g-module M into the g-module S. Hence, if φ denotes the canonical homomorphism of M ⊗_K L onto S, $ \phi(M \otimes_K L_0) = S_\delta $. As φ is obviously an S-module homomorphism, it suffices to show that L_0 is a finitely generated S_0-module. Let J be the sub-S-module of L generated by L_0. Since L is a Noetherian S-module, there exists a finite sequence (f_1, ..., f_q) of elements of L_0 generating the S-module J. Let L_1 be the S_0-module generated by f_1, \ldots, f_q. Then L_1 \subset L_0. On the other hand, if f \in L_0, then $ f = \sum_{i=1}^q s_i f_i $ with $ s_i \in S $ for all $ i $ and hence by Lemma 5 whose notation we adopt:

$$
f = f^\mathfrak{h} = \left( \sum_{i=1}^q s_i f_i \right)^\mathfrak{h} = \sum_{i=1}^q s_i^\mathfrak{h} f_i \in L_1.
$$

Hence $ L_0 = L_1 $, so that $ L_0 $ is a finite generated $ S_0 $-module.

### 10. CHANGE OF BASE FIELD

Let $ K_1 $ be a commutative extension of $ K $. For a Lie algebra $ g $ over $ K $ to be semi-simple, it is necessary and sufficient that $ g_{(K_1)} $ be semi-simple; for the Killing form $ \beta_1 $ of $ g_{(K_1)} $ is derived from the Killing form $ \beta $ of $ g $ by extending the base field from $ K $ to $ K_1 $; hence $ \beta_1 $ is non-degenerate if and only if $ \beta $ is non-degenerate (*Algebra*, Chapter IX, § 1, no. 4, Corollary to Proposition 3).

If $ g_{(K_1)} $ is simple, $ g $ is semi-simple by the above and cannot be a product of two non-zero ideals, hence $ g $ is simple. On the other hand if $ g $ is simple $ g_{(K_1)} $ (which is semi-simple) may be not simple (Exercises 17 and 26 (b)).

Let $ g $ be a Lie algebra and $ r $ its radical. Then $ r_{(K_1)} $ is the radical of $ g_{(K_1)} $ (\S 5, no. 6). Therefore, if $ s $ denotes the nilpotent radical of $ g $, the nilpotent radical of $ g_{(K_1)} $ is $ [g_{(K_1)}, r_{(K_1)}] = [g, r]_{(K_1)} = s_{(K_1)} $. It follows that $ g $ is reductive if and only if $ g_{(K_1)} $ is reductive.

Let $ g $ be a Lie algebra and $ h $ a subalgebra. Recall that a representation of $ h $ is semi-simple if and only if the representation of $ h_{(K_1)} $ derived by extending the base field to $ K_1 $ is semi-simple. Hence $ h $ is reductive in $ g $ if and only if $ h_{(K_1)} $ is reductive in $ g_{(K_1)} $.

Now let $ K_0 $ be a subfield of $ K $ such that $ [K : K_0] $ is finite. Let $ g $ be a Lie algebra and $ g_0 $ the (finite-dimensional) Lie algebra derived from $ g $ by restricting the base field from $ K $ to $ K_0 $. Every commutative ideal of $ g $ is a commutative ideal of $ g_0 $; conversely, if $ a_0 $ is a commutative ideal of $ g_0 $ the smallest vector subspace over $ K $ of $ g $ containing $ a_0 $ is a commutative ideal of $ g $; hence $ g $ is semi-simple if and only if $ g_0 $ is semi-simple. If $ g_0 $ is simple, clearly $ g $ is simple. Conversely, suppose that $ g $ is simple. We show that $ g_0 $ is simple. Let $ a_0 $ be a simple component of $ g_0 $. For all $ \lambda \in K^* $, $ \lambda a_0 $ is an ideal of $ g_0 $ and

$$
[a_0, \lambda a_0] = \lambda [a_0, a_0] = \lambda a_0 \neq \{0\},
$$

hence $ \lambda a_0 \supset a_0 $ and therefore $ \lambda a_0 = a_0 $ since $ \dim_{K_0}(\lambda a_0) = \dim_{K_0} a_0 $. Now the vector subspace of $ g $ generated by $ a_0 $ is a non-zero ideal of $ g $ and hence is the whole of $ g $. Hence $ g = a_0 $, which proves our assertion.

### Exercises {#lie-i-s6-exercises}

The conventions of § 6 remain valid unless otherwise mentioned.

See the [exercises for § 6](exercises/s6/).
