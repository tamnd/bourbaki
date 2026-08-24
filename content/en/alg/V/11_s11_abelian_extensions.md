---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 11
section_title: Abelian extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.160-A V.166
pdf_pages: 0191-0207, 0274-0280
extraction: ocr
subsections:
    - "no": 1
      title: Abelian extensions and the abelian closure
      page: 77
      pdf_page: 191
    - "no": 2
      title: Roots of unity
      page: 78
      pdf_page: 192
    - "no": 3
      title: Primitive roots of unity
      page: 79
      pdf_page: 193
    - "no": 4
      title: Cyclotomic extensions
      page: 81
      pdf_page: 195
    - "no": 5
      title: Irreducibility of cyclotomic polynomials
      page: 83
      pdf_page: 197
    - "no": 6
      title: Cyclic extensions
      page: 85
      pdf_page: 199
    - "no": 7
      title: Duality of $ \mathbf{Z}/n\mathbf{Z} $-modules
      page: 86
      pdf_page: 200
    - "no": 8
      title: Kummer theory
      page: 88
      pdf_page: 202
    - "no": 9
      title: Artin-Schreier theory
      page: 91
      pdf_page: 205
statements: 45
exercises: 23
content_sha256: 6948c79032d0ed93f4abaa213981181a5d1932d82792a48541b5e6e181c59fa4
---

## § 11. ABELIAN EXTENSIONS

Throughout this paragraph K denotes a field.

### 1. Abelian extensions and the abelian closure

#### Definition 1 {#alg-v-s11-def-1 .statement}

— An extension E of K is said to be abelian if it is Galois and its Galois group is commutative.

Since every subgroup of a commutative group is normal, Cor. 4 of V, p. 68 shows that every subextension of an abelian extension is abelian.

#### Proposition 1 {#alg-v-s11-prop-1 .statement}

— Let E be a Galois extension of K and Γ its Galois group. Let A be the derived group of Γ (I, p. 10, Def. 4) and F the field of invariants of A. For a subextension L to E to be abelian it is necessary and sufficient that it should be contained in F.

Firstly we note that F is also the field of invariants of the closure $ \bar{\Delta} $ of A in Γ, and that $ \bar{\Delta} $ is a closed normal subgroup of Γ. By V, p. 68, Cor. 4, F is thus a Galois extension of K. Further, the Galois group of F over K is isomorphic to $ \Gamma / \bar{\Delta} $ and hence is commutative. Hence every subextension of F is abelian. Conversely let L be an abelian extension of K contained in E, and let Π be the Galois group of E over L. Since L is Galois, Π is a normal subgroup of Γ and the Galois group of L over K is isomorphic to $ \Gamma / \Pi $ (V, p. 68, Cor. 4). Therefore $ \Gamma / \Pi $ is commutative and Π contains A, whence $ L \subset F $.

#### Corollary {#alg-v-s11-n1-cor-1 .statement}

— Let E be an extension of K and let $ (E_i)_{i \in I} $ be a family of subextensions of E such that $ E = K \left( \bigcup_{i \in I} E_i \right) $. Suppose that each extension $ E_i $ is abelian, then the same is true of E.

In the first place E is a Galois extension of K (V, p. 57, Prop. 1). If the field F is defined as in Prop. 1, then we have $ E_i \subset F $ for all $ i \in I $, whence $ E = F $.

An extension E of K is said to be an abelian closure of K if it is an abelian extension of K and every abelian extension of K is isomorphic to a subextension of E. Prop. 1 implies the existence of an abelian closure of K: for let $ K_s $ be a separable closure of K, with Galois group $ \Gamma $ and let $ (\overline{\Gamma}, \overline{\Gamma}) $ be the closure of the derived group of $ \Gamma $; denote by $ K_{ab} $ the field of invariants of $ (\overline{\Gamma}, \overline{\Gamma}) $; since every separable algebraic extension of K is isomorphic to a subextension of $ K_s $ (V, p. 45, Cor.). Prop. 1 shows that $ K_{ab} $ is an abelian closure of K. The Galois group of $ K_{ab} $ over K is canonically isomorphic to $ \Gamma / (\overline{\Gamma}, \overline{\Gamma}) $. Let us now show the uniqueness of abelian closures: let E, E' be two abelian closures of K; by definition there exist K-homomorphisms $ u : E \to E' $ and $ v : E' \to E $ and Prop. 1 (V, p. 52) implies that $ v(u(E)) = E $ and $ u(v(E')) = E' $, hence $ u $ is a K-isomorphism of E onto E'. Any other K-isomorphism of E onto E' is of the form $ u_1 = \sigma_0 \circ u $ with $ \sigma_0 \in \mathrm{Gal}(E'/K) $; since $ \mathrm{Gal}(E'/K) $ is commutative, the isomorphism $ \sigma \mapsto u \circ \sigma \circ u^{-1} $ of $ \mathrm{Gal}(E/K) $ onto $ \mathrm{Gal}(E'/K) $ is independent of $ u $; it is called the canonical isomorphism of $ \mathrm{Gal}(E/K) $ onto $ \mathrm{Gal}(E'/K) $.

### 2. Roots of unity

#### Definition 2 {#alg-v-s11-def-2 .statement}

*An element $ \zeta $ of K is said to be a root of unity if there exists an integer $ n > 0 $ such that $ \zeta^n = 1 $; for every integer $ n > 0 $ such that $ \zeta^n = 1 $, $ \zeta $ is called an n-th root of unity.*

It amounts to the same to say that the roots of unity are the elements of *finite order* of the multiplicative group $ K^* $ of non-zero elements of K (I, p. 51). The roots of unity form a subgroup $ \mu_\infty(K) $ of $ K^* $, the n-th roots form a subgroup $ \mu_n(K) $ of $ \mu_\infty(K) $. We have $ \mu_\infty(K) = \bigcup_{n \geq 1} \mu_n(K) $ and $ \mu_n(K) \subset \mu_m(K) $ if $ n $ divides $ m $. For every root of unity $ \zeta $ there exists a least integer $ n \geq 1 $ such that $ \zeta $ belongs to $ \mu_n(K) $, namely the order of $ \zeta $ in the group $ K^* $.

The group $ \mu_n(K) $, being the set of roots of the polynomial $ X^n - 1 $, is of finite order $ \leq n $. Let $ p $ be the characteristic of K. When $ p = 0 $, or when $ p \neq 0 $ and $ n $ is not divisible by $ p $, the derivative $ nX^{n-1} $ of $ X^n - 1 $ is relatively prime to $ X^n - 1 $ and so the polynomial $ X^n - 1 $ is then *separable*; if moreover K is algebraically closed, $ \mu_n(K) $ is thus a group of $ n $ elements.

Suppose that K is of non-zero characteristic $ p $ and let $ r \geq 0 $ be an integer; since the mapping $ x \mapsto x^{p^r} $ of K into K is injective, we have $ \mu_{np^r}(K) = \mu_n(K) $ for every integer $ n \geq 1 $.

We remark that a field may contain no n-th root of unity other than 1: this is the case for example with the prime fields $ \mathbf{Q} $ and $ \mathbf{F}_p $ for any odd integer $ n $.

#### Theorem 1 {#alg-v-s11-thm-1 .statement}

*Let $ p $ be the characteristic exponent of K and let $ n > 0 $ be an integer. Then the group $ \mu_n(K) $ of n-th roots of unity in K is cyclic and its order divides $ n $; when K is algebraically closed and $ n $ is prime to $ p $, the group $ \mu_n(K) $ is cyclic of order $ n $.*

It is enough to prove the first assertion of the theorem which is a consequence of the following more precise lemma:

#### Lemma 1 {#alg-v-s11-lem-1 .statement}

*Let G be a finite subgroup of $ K^* $ of order $ m $; then G is cyclic and we have $ G = \mu_m(K) $.*

Consider G as Z-module; we have $ mx = 0 $ for all $ x \in G $, hence the annihilator of G is an ideal of the form $ r\mathbf{Z} $, where the integer $ r \geq 1 $ divides $ m $. We thus have $ G \subset \mu_r(K) $. By Lemma 4 (V, p. 74) applied with $ A = \mathbf{Z} $ and $ M = G $ there exists an element $ x $ of G of order $ r $; let $ G' $ be the cyclic subgroup of G generated by $ x $. We have $ G' \subset \mu_r(K) $, Card $ (G') = r $ and Card $ \mu_r(K) \leq r $; therefore we have

G' = μ_r(K) ⊃ G and G is cyclic of order r, hence equal to μ_r(K). Since G has order m, we have m = r and the lemma follows.

#### Proposition 2 {#alg-v-s11-prop-2 .statement}

— Let K be algebraically closed and let p be its characteristic exponent. There exists an isomorphism of μ_∞(K) onto the group Q/Z[1/p].

We have denoted by Z[1/p] the subring of Q generated by 1/p, that is, the set of rational numbers of the form a/p^n with a ∈ Z and n ≥ 1; thus we have Z[1/p] = Z if K is of characteristic 0.

Let (v_n), be the strictly increasing sequence consisting of all the integers which are not divisible by p, if p ≠ 1; put X = v_1 v_2 ... v_n and denote by H_n the group of λ_n-th roots of unity; we have H_{n+1} ⊃ H_n and μ_∞(K) = U H_n. Since H_n is cyclic of order X, (Th. 1), there exists a sequence (a_n), of roots of unity such that a_n generates H_n and a_n = α_n^{v_n + 1}.

Further let β_n be the residue class mod Z[1/p] of 1/λ_n and let H'_n be the cyclic subgroup of Q/Z[1/p] generated by β_n. It is clear that β_n = v_{n+1} β_{n+1} and H'_n is of order λ_n because X is not divisible by p if p ≠ 1. Thus there exists for all n ≥ 1 an isomorphism φ_n : H_n → H'_n such that φ_n(α_n) = β_n and the relations α_n = α_{n+1}^{v_n + 1}, β_n = v_{n+1} β_{n+1}, show that φ_n+, extends φ_n. Finally there exists a unique isomorphism φ of μ_∞(K) onto Q/Z[1/p] extending the isomorphisms φ_n, that is, φ(α_n) = β_n for all n ≥ 1.

#### Remark 1 {#alg-v-s11-n2-rem-1 .statement}

When K is an algebraically closed field of characteristic 0, the group μ_∞(K) is thus isomorphic (not canonically) to Q/Z. *When K is the field C of complex numbers, we can write down an explicit such isomorphism: in effect the mapping x ↦ e^{2πix} is a homomorphism of Q into C* with kernel Z and image μ_∞(C); thus by passage to quotients it defines an isomorphism of Q/Z onto μ_∞(C).*

#### Remark 2 {#alg-v-s11-n2-rem-2 .statement}

The following result may be shown (cf. V, p. 165, Ex. 21): let G and H be two commutative groups all of whose elements are of finite order. Suppose that for every integer n ≥ 1, the equation nx = 0 has the same number of solutions, assumed finite in G and in H. Then the groups G and H are isomorphic. This provides a new proof of Prop. 2.

#### Remark 3 {#alg-v-s11-n2-rem-3 .statement}

For every prime number l put μ_{l∞}(K) = U μ_{ln}(K). When l is the characteristic p of K, we have μ_{p∞}(K) = {1}. From I, p. 80, Th. 4, we deduce that μ_∞(K) is a direct sum of the subgroups μ_{l∞}(K), where l runs over the set of all prime numbers distinct from p. For a given prime number l only two cases are possible: either μ_{l∞}(K) is finite and then μ_{l∞}(K) is isomorphic to Z/l^nZ for a suitable n (Th. 1), or μ_{l∞}(K) is infinite and then μ_{l∞}(K) is isomorphic to Z[l^{-1}]/Z (cf. Remark 2).

### 3. Primitive roots of unity

Let n ≥ 1 be an integer. By the Euler indicator of n, written φ(n), we understand the number of invertible elements of the ring Z/nZ of integers modulo n. By the next proposition $ \varphi(n) $ is also the number of integers $ k $ prime to $ n $ and such that $ 0 \leq k < n $.

#### Proposition 3 {#alg-v-s11-prop-3 .statement}

*Let $ k $ and $ n \geq 1 $ be two integers. Then the following assertions are equivalent*:

a) *the residue class of $ k $ mod $ n $ is invertible in the ring $ \mathbf{Z}/n\mathbf{Z} $;*
b) *the residue class of $ k $ mod $ n $ generates the cyclic group $ \mathbf{Z}/n\mathbf{Z} $;*
c) *the integers $ k $ and $ n $ are relatively prime* (*I*, p. 112).

Each of the conditions a) and b) means that there exists an integer $ x $ such that $ kx \equiv 1 \pmod{n} $, that is, there exist two integers $ x $ and $ y $ such that $ kx + ny = 1 $. This latter condition just means that $ k $ and $ n $ are relatively prime.

#### Corollary 1 {#alg-v-s11-prop-3-cor-1 .statement}

*Let $ G $ be a cyclic group of order $ n $ and let $ d $ be a divisor of $ n $. Then the number of elements of order $ d $ in $ G $ is equal to $ \varphi(d) $. In particular, $ \varphi(n) $ is the number of generators of $ G $.*

Since $ G $ is isomorphic to $ \mathbf{Z}/n\mathbf{Z} $, the number of generators of $ G $ is equal to $ \varphi(n) $ by Prop. 3. Let $ g $ be a generator of $ G $; then the elements $ h $ of $ G $ such that $ h^d = 1 $ constitute the subgroup $ H $ of $ G $ generated by $ g^{n/d} $; this group is cyclic of order $ d $ and the elements of order $ d $ of $ G $ are the generators of $ H $, hence their number is $ \varphi(d) $.

#### Corollary 2 {#alg-v-s11-prop-3-cor-2 .statement}

*For every integer $ n \geq 1 $, we have*
$$
\sum_{d \mid n} \varphi(d) = n,
$$
*where the integer $ d $ runs over the set of divisors > 0 of $ n $* ^1.

With the notation of Cor. 1, every element of $ G $ has a finite order which is a divisor $ d $ of $ n $ and for a fixed $ d $ there are $ \varphi(d) $ such elements.

The calculation of $ \varphi(n) $ is based on the two formulae:

(2) $ \varphi(mn) = \varphi(m)\varphi(n) $ if $ m $ and $ n $ are relatively prime ,
(3) $ \varphi(p^a) = p^{a-1}(p-1) $ ($ p $ prime, $ a \geq 1 $).

The first follows at once from the fact that the rings $ \mathbf{Z}/mn\mathbf{Z} $ and $ (\mathbf{Z}/m\mathbf{Z}) \times (\mathbf{Z}/n\mathbf{Z}) $ are isomorphic (*I*, p. 112), and that $ (A \times B)^* = A^* \times B^* $ for two rings $ A $ and $ B $. To prove (3) we note that the positive divisors of $ p^a $ are $ 1, p, p^2, \ldots, p^a $; hence the integer $ k $ has no common divisor with $ p^a $ other than $ 1 $ if and only if it is not divisible by $ p $; since there are $ p^a - 1 $ multiples of $ p $ between $ 0 $ and $ p^a - 1 $, we find indeed (3).

The formulae (2) and (3) show at once that
$$
\varphi(n) = n \prod_p (1 - 1/p),
$$
where $ p $ runs over the set of prime divisors of $ n $.

^1 The relation $ d \mid n $ between integers > 0 means « d divides n » (VI, p. 5).

An n-th root of unity is said to be primitive if it is of order $ n $; if there exists such a root $ \zeta $, the group $ \mu_n(K) $ is of order $ n $ and is generated by $ \zeta $. \* For example, the primitive n-th roots of unity in $ \mathbf{C} $ are the numbers $ e^{2\pi i k / n} $ with $ 0 \leq k < n $ and $ k $ prime to $ n $. \* Cor. 1 of Prop. 3 now implies the following result.

#### Proposition 4 {#alg-v-s11-prop-4 .statement}

— Let $ n \geq 1 $ be an integer; suppose that there exist n n-th roots of unity in K (this is true for example if K is separably closed and $ n . 1, \neq 0 $). Then the number of primitive n-th roots of unity in K is equal to $ \varphi(n) $.

### 4. Cyclotomic extensions

Let $ p $ be the characteristic exponent of K and let $ n \geq 1 $ be an integer prime to $ p $; by a cyclotomic extension of level $ n $ over K we understand any splitting extension E of the polynomial $ X^n - 1 $ over K (V, p. 21). Since this polynomial is separable, E is a Galois extension of K, of finite degree (V, p. 57). There exists a primitive n-th root of unity in E ; if $ \zeta $ is such a root, then every n-th root of unity is a power of $ \zeta $, hence $ E = K(\zeta) $.

For the rest of this No. we shall choose a separable closure $ K_s $ of K. For every $ n \geq 1 $ prime to $ p $ the group $ \mu_n(K_s) $ is cyclic of order $ n $ and the field

$$
R_n(K) = K(\mu_n(K_s))
$$

is a cyclotomic extension of level $ n $ of K. We can consider $ \mu_n(K_s) $ as a free module of rank 1 over the ring $ \mathbf{Z}/n\mathbf{Z} $, and every element $ a $ of $ \mathrm{Gal}(K_s/K) $ induces an automorphism of $ \mu_n(K_s) $; there exists therefore a homomorphism $ \chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^* $ characterized by the formula $ u(\zeta) = \zeta^j $ for every n-th root of unity $ \zeta $ in $ K_s $, every $ u $ in $ \mathrm{Gal}(K_s/K) $ and every integer $ j $ in the residue class $ \chi_n(u) $ mod $ n $. Since $ R_n(K) = K(\mu_n(K_s)) $, the kernel of $ \chi_n $ is the subgroup $ \mathrm{Gal}(K_s/R_n(K)) $ of $ \mathrm{Gal}(K_s/K) $; hence we have $ \chi_n = \varphi_n \circ \psi_n $ where $ \psi_n $ is the restriction homomorphism of $ \mathrm{Gal}(K_s/K) $ over $ \mathrm{Gal}(R_n(K)/K) $ and $ \varphi_n $ is an injective homomorphism of $ \mathrm{Gal}(R_n(K)/K) $ in $ (\mathbf{Z}/n\mathbf{Z})^* $. In particular we have the following result :

#### Proposition 5 {#alg-v-s11-prop-5 .statement}

— For every integer $ n \geq 1 $ prime to $ p $ the extension $ R_n(K) $ of K is abelian of finite degree, its Galois group is isomorphic to a subgroup of $ (\mathbf{Z}/n\mathbf{Z})^* $ and its degree divides the order $ \varphi(n) $ of $ (\mathbf{Z}/n\mathbf{Z})^* $.

Let Q be an algebraic closure of the field Q of rational numbers, and let n be an integer. Then the cyclotomic polynomial $ \Phi_n $ of level $ n $ is defined by

$$
\Phi_n(X) = \prod_{\zeta \in S_n} (X - \zeta),
$$

where $ S_n $ is the set of primitive n-th roots of unity in $ Q $. The polynomial $ \Phi_n $ is of degree $ \varphi(n) $ (Prop. 4). It is clear that $ \Phi_n(X) $ is invariant under all automorphisms of $ \bar{\mathbf{Q}} $, and so belongs to $ \mathbf{Q}[X] $. Since every element $ \zeta $ of $ S_n $ is a root of the polynomial $ X^n - 1 $, the polynomial $ \Phi_n(X) $ divides $ X^n - 1 $, and the following lemma shows that $ \Phi_n(X) $ is a monic polynomial with integer coefficients.

#### Lemma 2 {#alg-v-s11-lem-2 .statement}

*Let f, g and h be monic polynomials in $ \mathbf{Q}[X] $ such that $ f = gh $. If f has integer coefficients, the same is true of g and h.*

Let $ a $ (resp. $ b $) be the least of the integers $ \alpha \geq 3 $ (resp. $ \beta \geq 1 $) such that $ \alpha g $ (resp. $ \beta h $) has integer coefficients; we put $ g' = ag $ and $ h' = bh $ and show by *reductio ad absurdum* that $ a = b = 1 $. If this were not so, there would be a prime divisor $ p $ of $ ab $. If $ u \in \mathbf{Z}[X] $, let us write $ \bar{u} $ for the polynomial with coefficients in the field $ \mathbf{F}_p $ obtained by reduction mod $ p $ of the coefficients of $ u $. We have $ g'h' = abf $, whence $ \bar{g}'\bar{h}' = 0 $; since the ring $ \mathbf{F}_p[X] $ is an integral domain (IV, p. 9, Prop. 8) we thus have $ \bar{g}' = 0 $ or $ \bar{h}' = 0 $. In other words, $ p $ divides all the coefficients of $ g' $ or all those if $ h' $ and this contradicts the hypothesis.

We have the relation

$$
X^n - 1 = \prod_{d|n} \Phi_d(X) .
$$

For we have $ X^n - 1 = \prod_{\zeta \in \mu_n(\mathbf{Q})} (X - \zeta) $ and the sets $ S_d $ for $ d $ dividing $ n $ form a partition of $ \mu_n(\mathbf{Q}) $.

The formula (6) determines $ \Phi_n(X) $ when we know $ \Phi_d(X) $ for all the divisors $ d < n $ of $ n $; since $ \Phi_1(X) = X - 1 $, we thus have a recursive procedure for calculating $ \Phi_n $. For example for prime $ p $ we have

$$
X^p - 1 = (X - 1)\Phi_p(X) ,
$$

whence

$$
\Phi_p(X) = X^{p-1} + X^{p-2} + \cdots + X + 1 ,
$$

and

$$
\Phi_{p^r+1}(X) = \Phi_p(X^{p^r}) \quad \text{for} \quad r \geq 0 .
$$

Let us list the values of the polynomials $ \Phi_n(X) $ for $ 1 \leq n \leq 12 $:

$$
\begin{align*}
\Phi_1(X) &= X - 1 \\
\Phi_2(X) &= X + 1 \\
\Phi_3(X) &= X^2 + X + 1 \\
\Phi_4(X) &= X^2 + 1 \\
\Phi_5(X) &= X^4 + X^3 + X^2 + X + 1 \\
\end{align*}
$$

$$
\Phi_6(X) = X^2 - X + 1
$$
$$
\Phi_7(X) = X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_8(X) = X^4 + 1
$$
$$
\Phi_9(X) = X^6 + X^3 + 1
$$
$$
\Phi_{10}(X) = X^4 - X^3 + X^2 - X + 1
$$
$$
\Phi_{11}(X) = X^{10} + X^9 + X^8 + X^7 + X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_{12}(X) = X^4 - X^2 + 1
$$

The values of $ \Phi_1, \Phi_2, \Phi_3, \Phi_4, \Phi_5, \Phi_7, \Phi_8, \Phi_9 $ and $ \Phi_{11} $ follow directly from (7); now we have $ \Phi_1 \Phi_2 \Phi_3 \Phi_6 = X^6 - 1 $ and $ \Phi_1 \Phi_2 \Phi_3 \Phi_4 \Phi_6 \Phi_{12} = X^{12} - 1 $, whence $ \Phi_4 \Phi_{12} = \frac{X^{12} - 1}{X^6 - 1} - X^6 + 1 $ and finally $ \Phi_{12} = \frac{X^6 + 1}{X^2 + 1} = X^4 - X^2 + 1 $. The cases $ n = 6 $ and $ n = 10 $ may be treated similarly.

#### Remark {#alg-v-s11-n4-rem-1 .statement}

\* For every integer $ n > 0 $ a function $ \mu(n) $ is defined as follows: if $ n $ is divisible by the square of a prime number, we put $ \mu(n) = 0 $, otherwise $ \mu(n) = (-1)^h $ if $ n $ is the product of $ h $ distinct prime numbers (« Mobius function »). It may be shown that

$$
\Phi_n(X) = \prod_{d|n} (X^{n/d} - 1)^{\mu(d)},
$$

or more explicitly

$$
\Phi_n(X) = \prod_{p_1 < \ldots < p_h} (X^{n/p_1 \cdots p_h} - 1)^{(-1)^h}
$$

where $ (p_1, \ldots, p_h) $ runs over the set of all strictly increasing sequences of prime divisors of $ n $ (cf. Lie, II, p. 207, Ex. 1).

### 5. Irreducibility of cyclotomic polynomials

Let $ p $ be the characteristic exponent of $ K $ and let $ n $ be an integer prime top. We denote by $ \Phi_n \in K[X] $ the image of the polynomial with integer coefficients $ \Phi_n $ under the unique homomorphism of $ \mathbf{Z}[X] $ into $ K[X] $ which maps $ X $ to $ X $.

#### Lemma 3 {#alg-v-s11-lem-3 .statement}

*The roots of $ \Phi_n $ in $ K_s $ are the primitive $ n $-th roots of unity.*

Denote by $ S $, the set of roots of $ \Phi_n $ in $ K_s $. By Formula (6), the set $ \mu_n(K_s) $ is the union of the $ S_d $ for $ d $ dividing $ n $. Every primitive $ n $-th root of unity thus belongs to $ S_n $ and the lemma now follows from Prop. 4 (V, p. 81).

#### Proposition 6 {#alg-v-s11-prop-6 .statement}

— Let $ p $ be the characteristic exponent of $ K $ and let $ n \geq 1 $ be an integer prime to $ p $. For the polynomial $ \Phi_n(X) $ to be irreducible in $ K[X] $ it is necessary and sufficient that the homomorphism $ \chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^* $ should be surjective.

By Lemma 3 we have $ R_n(K) = K(\zeta) $ for each root $ \zeta $ of $ \Phi_n(X) $ and hence $ \Phi_n(X) $ is irreducible in $ K[X] $ if and only if the degree $ \varphi(n) $ of $ \Phi_n(X) $ is equal to $ [R_n(K):K] $. Further, the Galois group of $ R_n(K) $ over $ K $ is of order $ [R_n(K):K] $ and it is isomorphic to the subgroup of $ (\mathbf{Z}/n\mathbf{Z})^* $ which is the image of $ \chi_n $. Now Prop. 6 follows from the fact that $ (\mathbf{Z}/n\mathbf{Z})^* $ is of order $ \varphi(n) $.

#### Theorem 2 (Gauss) {#alg-v-s11-thm-2 .statement}

— Let $ Q $ be an algebraic closure of $ Q $ and let $ n \geq 1 $ be an integer.

a) The cyclotomic polynomial $ \Phi_n(X) $ is irreducible in $ Q[X] $.

b) The degree of $ R_n(Q) $ over $ Q $ is $ \varphi(n) $.

c) The homomorphism $ \chi_n $ of $ \mathrm{Gal}(\bar{Q}/Q) $ into $ (\mathbf{Z}/n\mathbf{Z})^* $ is surjective and defines by passage to quotients an isomorphism of $ \mathrm{Gal}(R_n(Q)/Q) $ onto $ (\mathbf{Z}/n\mathbf{Z})^* $.

Taking account of Prop. 6, we need only prove c). Every integer $ r $ prime to $ n $ is a product of prime numbers $ p_1, \ldots, p_s $ not dividing $ n $; so it is enough to show that for every prime number $ p $ not dividing $ n $, the mapping $ x \mapsto x^p $ of $ \mu_n(Q) $ into itself extends to an automorphism of $ R_n(Q) $. It suffices to prove that if $ \zeta $ is a primitive $ n $-th root of unity, the minimal polynomial $ f $ of $ \zeta $ over $ Q $ is equal to the minimal polynomial $ g $ of $ \zeta^p $ over $ Q $.

We shall assume that $ f \neq g $ and argue by contradiction. The polynomials $ f $ and $ g $ are monic irreducible in $ Q[X] $ and divide $ X^n - 1 $, so there exists $ u \in Q[X] $ such that $ X^n - 1 = fg u $ (IV, p. 13, Prop. 13). Lemma 2 (V, p. 82) shows that $ f, g $ and $ u $ have integer coefficients. Let us denote by $ \bar{v} $ the polynomial with coefficients in $ \mathbf{F}_p $ obtained from a polynomial $ v \in \mathbf{Z}[X] $ by reduction mod $ p $. We thus have $ X^n - 1 = \bar{f} \bar{g} \bar{u} $ in $ \mathbf{F}_p[X] $.

Further we have $ g(\zeta^p) = 0 $ and so $ g(X^p) $ is a multiple of $ f(X) $ in $ \mathbf{Q}[X] $. By Lemma 2 there exists $ h \in \mathbf{Z}[X] $ such that $ g(X^p) = f(X) \cdot h(X) $. Now we have $ v(X^p) = v(X)^p $ for every polynomial $ v \in \mathbf{F}_p[X] $. By reduction mod $ p $ we thus obtain $ \bar{g}^p = \bar{f} \bar{h} $. If $ v $ is an irreducible polynomial in $ \mathbf{F}_p[X] $ dividing $ \bar{f} $, it must then divide $ \bar{g} $. Since $ \bar{f} \bar{g} $ divides $ X^n - 1 $, we conclude that $ v^2 $ divides $ X^n - 1 $ in $ \mathbf{F}_p[X] $. This is absurd because the polynomial $ X^n - 1 $ is separable in $ \mathbf{F}_p[X] $.

It may be shown that for every abelian extension $ E $ of finite degree over $ Q $ there exists an integer $ n \geq 1 $ such that $ E $ is isomorphic to a subextension of $ R_n(Q) $. \* In other words, the field $ Q(\mu_{\infty}(C)) $ is an abelian closure of $ Q $. *(« Kronecker-Weber theorem »).

### 6. Cyclic extensions

#### Definition 3 {#alg-v-s11-def-3 .statement}

— *An extension E of K is said to be cyclic if it is Galois and its Galois group is cyclic.*

*Examples. — 1) Every Galois extension of prime degree is cyclic, because every finite group G of prime order $ p $ is cyclic (for every element $ x \neq 1 $ of G is of order $ p $, hence generates G).

2) Let $ F(X) = X^2 + aX + b $ be an irreducible polynomial in $ K[X] $. The only case where $ F(X) $ is not separable is that where $ K $ is of characteristic 2 and $ a = 0 $. We shall leave this case aside; let E be an extension of K generated by a root $ x $ of $ F(X) $. We have $[E : K] = 2$ and $ F(X) = (X - x)(X + a + x) $, hence E is a Galois extension of K. The Galois group of E over K is of order 2, hence cyclic.

3) Let $ \mathbf{F} $ be a field and $ \sigma $ an automorphism of finite order. The field E of invariants of $ \sigma $ is also the field of invariants of the cyclic group of order $ n $ generated by $ \sigma $, and hence (V, p. 66, Th. 3) F is a cyclic extension of degree $ n $ of E.

We know (I, p. 50) that every *subgroup* and every *quotient group* of a cyclic group is cyclic. Therefore (V, p. 68, Cor. 4), if E is a cyclic extension of a field K, of degree $ n $, then every subextension F of E is *cyclic over K*, and *E is cyclic over F*. For every divisor d of $ n $ there exists a unique subfield F of degree d over K contained in E : for in a cyclic group of order $ n $ there exists a unique subgroup of index d.

#### Theorem 3 (*Hilbert*) {#alg-v-s11-thm-3 .statement}

— *Let E be a cyclic extension of K and let a be a generator of the Galois group $ \Gamma $ of E over K.

a) For an element $ x \in E $ to satisfy $ N_{E/K}(x) = 1 $ it is necessary and sufficient that $ y \in E^* $ exist such that $ x = y / \sigma(y) $; every $ y_1 \in E^* $ with $ x = y_1 / \sigma(y_1) $ is then of the form $ \lambda y $ where $ \lambda \in K^* $.

b) For an element $ x \in E $ to satisfy $ \mathrm{Tr}_{E/K}(x) = 0 $ it is necessary and sufficient that $ z \in E $ exist with $ x = z - \sigma(z) $; then every $ z_1 \in E $ with $ x = z_1 - \sigma(z_1) $ is of the form $ z + \mu $, where $ \mu \in K $.

Let us first prove a lemma.*

#### Lemma 4 {#alg-v-s11-lem-4 .statement}

*Let $ \Gamma $ be a cyclic group of order $ n $, $ \sigma $ a generator of $ \Gamma $ and M a commutative group on which $ \Gamma $ operates according to the rule $ \gamma . (m + m') = \gamma . m + \gamma . m' $ for all $ \gamma \in \Gamma $ and $ m, m' \in M $. Let Z be the set of all mappings of $ \Gamma $ into M satisfying the relation*

$$
f(\tau \tau') = f(\tau) + \tau . f(\tau') \quad \text{for } \tau, \tau' \text{ in } \Gamma
$$

Put $ u(f) = f(a) $ for $ f \in Z $ and $ t(m) = \sum_{\tau \in \Gamma} \tau . m $ for $ m \in M $. Then the sequence

$$
0 \to Z \xrightarrow{u} M \xrightarrow{t} M
$$

is exact.

Let $ f \in \mathbf{Z} $; taking $ \tau = \tau' = 1 $ in (10) we find that $ f(1) = 0 $. Further, by induction on $ m \geqslant 0 $ we deduce the relation

$$
f(\sigma^m) = f(\sigma) + \sigma \cdot f(\sigma) + \cdots + \sigma^{m-2} \cdot f(\sigma) + \sigma^{m-1} \cdot f(\sigma)
$$

We have $ \sigma^n = 1 $, whence $ f(\sigma^n) = 0 $; the preceding relation with $ m = n $ is equivalent to the equality $ t(u(f)) = 0 $, whence $ \operatorname{Im}\ u \subset \operatorname{Ker}\ t $. Moreover, from (11) it follows that $ \operatorname{Ker}\ u = 0 $.

Let $ m \in M $ be such that $ t(m) = 0 $, that is, $ m + \sigma \cdot m + \cdots + \sigma^{n-1} \cdot m = 0 $. Let us define the mapping $ f $ of $ \Gamma $ into $ M $ by

$$
f(\sigma^j) = m + \sigma \cdot m + \cdots + \sigma^{j-2} \cdot m + \sigma^{j-1} \cdot m
$$

for $ 0 \leqslant j \leqslant n - 1 $. It may be left to the reader to establish the relation (10). We clearly have $ m = f(a) $, whence $ \operatorname{Im}\ u \supset \operatorname{Ker}\ t $.

With the lemma now proved, let us take $ y \in E^* $ and $ x = y/\sigma(y) $; we have $ N_{E/K}(\sigma(y)) = N_{E/K}(y) $, whence $ N_{E/K}(x) = 1 $. Conversely, let $ x $ in $ E^* $ be such that $ N_{E/K}(x) = 1 $; by Lemma 4, applied to $ M = E^* $, there exists a family of elements $ (c_\tau)_{\tau \in \Gamma} $ of $ E^* $ satisfying the relation $ c_{\tau \tau'} = c_\tau \cdot \tau(c_{\tau'}) $ for $ \tau, \tau' $ in $ \Gamma $ and $ c_\sigma = x $. By Cor. 1 of Prop. 9 (V, p. 65) there exists $ y \in E^* $ with $ c_\tau = y/\tau(y) $ for all $ \tau \in \Gamma $, whence in particular $ x = c_\sigma = y/\sigma(y) $. If $ y_1 \in E^* $ satisfies $ x = y_1/\sigma(y_1) $, then we have

$$
\sigma(y_1 y^{-1}) = y_1 y^{-1},
$$

hence $ y_1 y^{-1} $ belongs to $ K^* $ because $ a $ generates the Galois group of $ E $ over $ K $. This proves a).

The assertion b) follows in similar fashion from Cor. 2 of Prop. 9 (V, p. 65).

### 7. Duality of $ \mathbf{Z}/n\mathbf{Z} $-modules

In this No. we denote by $ n $ an integer $ > 0 $ and by $ T $ a cyclic group of order $ n $. A group $ G $ is said to be annihilated by $ n $ if $ g^n = 1 $ for all $ g \in G $; if moreover $ G $ is commutative, the group structure of $ G $ is underlying a unique $ \mathbf{Z}/n\mathbf{Z} $-module structure.

For every group $ G $ we denote by $ \operatorname{Hom}(G, T) $ the group of homomorphisms of $ G $ into $ T $; it is a commutative group annihilated by $ n $.

#### Proposition 7 {#alg-v-s11-prop-7 .statement}

— Let $ G $ be a commutative group annihilated by $ n $ and $ H $ a subgroup of $ G $. Then the restriction homomorphism $ \operatorname{Hom}(G, T) \to \operatorname{Hom}(H, T) $ is surjective.

For let $ f : H \to T $ be a homomorphism; we shall prove that there exists a homomorphism of $ G $ into $ T $ extending $ f $. Suppose first that $ G $ is cyclic, generated by an element $ g $ of order $ r $ dividing $ n $; denote by $ t $ a generator of $ T $. There exists a divisor s of r such that H is generated by $ g^s $ (I, p. 50, Prop. 19), and for every $ x \in \mathbf{Z} $ we have $ f(g^{sx}) = t^{ax} $, where a is an integer such that n divides $ ar/s $. Then $ a/s = (ar/ns)(n/r) $ is an integer and the homomorphism $ g^x \mapsto t^{(a/s)x} $, $ x \in \mathbf{Z} $, of G into T extends f. In the general case consider the set of pairs $(H', f')$ where $ H' $ is a subgroup of G containing H and $ f' $ is a homomorphism of $ H' $ into T extending $ f $, and let us order this set by the relation $(H', f') \leq (H'', f'')$ if $ H' \subset H'' $ and the restriction of $ f'' $ to $ H' $ is $ f' $. By Set Theory, III, p. 154, Def. 3 and Th. 2, this set has a maximal element $(H_1, f_1)$ and it suffices to prove that $ H_1 = G $; if this is not the case, there exists $ g \in G, g \notin H_1 $ and it is enough to prove that $ f_1 $ may be extended to a homomorphism T of the subgroup of G generated by $ H_1 $ and g. Now if C denotes the cyclic group generated by g, the restriction of $ f_1 $ to $ C \cap H_1 $ extends to a homomorphism $ f_2 $ of C into T and the homomorphism $ xy \mapsto f_1(x) f_2(y), x \in H_1, y \in C, $ of $ H_1C $ into T is the desired mapping.

#### Corollary 1 {#alg-v-s11-prop-7-cor-1 .statement}

— If G *is* a commutative group annihilated by *n*, and $ G \neq \{1\} $, then $ \mathrm{Hom}(G, T) \neq \{1\} $.

For it suffices to note that if H is a cyclic subgroup of G distinct from $\{1\}$, then $ \mathrm{Hom}(H, T) \neq \{1\} $, and to apply Prop. 7.

#### Corollary 2 {#alg-v-s11-prop-7-cor-2 .statement}

— If G *is* a *finite* commutative group annihilated by *n*, then the groups G and $ \mathrm{Hom}(G, T) $ have the same order.

If G is cyclic of order *r*, with generator g, then the mapping $ f \mapsto f(g) $ is a bijection of $ \mathrm{Hom}(G, T) $ onto the set of elements t of T such that $ t^r = 1 $, hence the assertion follows in this case. On the other hand, if H is a cyclic subgroup of G, we have $ \mathrm{Card}(G) = \mathrm{Card}(H) \cdot \mathrm{Card}(G/H) $; further, we have an exact sequence

$$
\{1\} \to \mathrm{Hom}(G/H, T) \to \mathrm{Hom}(G, T) \to \mathrm{Hom}(H, T) \to \{1\}
$$

(II, p. 227, Th. 1 and Prop. 7 above), hence

$$
\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(\mathrm{Hom}(H, T)) \cdot \mathrm{Card}(\mathrm{Hom}(G/H, T)).
$$

Since $ \mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H) $, it comes to the same to prove the corollary for G or for $ G/H $. Now the result follows by induction on $ \mathrm{Card}(G) $.

Now let G and H be two groups and $ f : G \times H \to T $ a bimultiplicative mapping, that is, such that for any $ g, g' \in G, h, h' \in H $ we have

$$
f(gg', h) = f(g, h) f(g', h), \quad f(g, hh') = f(g, h) f(g, h')
$$

We define group homomorphisms

$$
s_f : G \to \mathrm{Hom}(H, T), \quad d_f : H \to \mathrm{Hom}(G, T),
$$

by $ s_f(g)(h) = d_f(h)(g) = f(g, h) $ (cf. II, p. 268, Cor. to Prop. 1, when G and H are commutative).

#### Proposition 8 {#alg-v-s11-prop-8 .statement}

— *Suppose that G and H are commutative and annihilated by n. If s_f is bijective and H is finite, then d_f is bijective and we have Card(G) = Card(H).*

If s_f is bijective and H is finite, we have by Cor. 2 to Prop. 7 the relation Card(G) = Card(Hom(H, T)) = Card(H), hence Card(G) is finite and by another application of the Corollary, Card(Hom(G, T)) = Card(H). So it is enough to prove that d_f is injective. Now if h \in \mathrm{Ker}(d_f), we have f(g, h) = 1 for all g \in G, hence since s_f is bijective, \varphi(h) = 1 for all \varphi \in \mathrm{Hom}(H, T); by Prop. 7 this implies \mathrm{Hom}(\mathrm{Ker}(d_f), T) = \{1\}, hence \mathrm{Ker}(d_f) = \{1\} by Cor. 1 to Prop. 7.

### 8. Kummer theory

In this No. we denote by $ n $ an integer > 0, and we shall suppose that $ \mu_n(K) $ has $ n $ elements; by V, p. 78 this means also that $ n $ is prime to the characteristic exponent of K and that all the n-th roots of unity in an algebraic closure $ \Omega $ of K lie in K.

We shall say that an extension L of K is *abelian of exponent dividing n* if it is abelian (V, p. 77, Def. 1) and its Galois group Gal(L/K) is annihilated by $ n $ (V, p. 86).

Let A be a subset of $ K^* $; we denote by $ K(A^{1/n}) $ the subextension of $ \Omega $ generated by all $ 0 \in \Omega $ such that $ \theta^n \in A $.

#### Lemma 5 {#alg-v-s11-lem-5 .statement}

— *$ K(A^{1/n}) $ is an abelian extension of K of exponent dividing n.*

Since the polynomials $ X^n - a, a \in A $ are separable over K, $ L = K(A^{1/n}) $ is a separable, hence a Galois extension of K. Let $ \sigma \in \mathrm{Gal}(L/K) $ and let $ 0 \in \Omega $ be such that $ \theta^n \in A $. We have $ \sigma(\theta)^n = \theta^n $; hence there exists $ \zeta \in \mu_n(\Omega) = \mu_n(K) $ such that $ \sigma(\theta) = \zeta \theta $; this implies that $ \sigma^n(\theta) = \zeta^n \theta = 0 $, whence $ \sigma^n = 1 $. If $ \sigma' $ is another element of $ \mathrm{Gal}(L/K) $ there exists $ \zeta' \in \mu_n(K) $ such that $ \sigma'(\theta) = \zeta' \theta $, whence $ \sigma'\sigma(\theta) = \zeta \zeta' \theta = \sigma\sigma'(\theta) $ and so $ \sigma'\sigma = \sigma\sigma' $.

#### Lemma 6 {#alg-v-s11-lem-6 .statement}

— *Let L be a Galois extension of K. There exists a unique mapping $ (\sigma, a) \mapsto \langle \sigma, a \rangle $ of $ \mathrm{Gal}(L/K) \times ((L^n \cap K^*)/K^{*n}) $ into $ \mu_n(K) $ such that for every $ \sigma \in \mathrm{Gal}(L/K) $ and every element $ 0 \in L^* $ such that $ \theta^n \in K $ we have, on denoting by $ \overline{\theta^n} $ the residue class of $ \theta^n $ mod $ K^{*n} $:*

$$
\langle \sigma, \overline{\theta^n} \rangle = \sigma(\theta)/\theta
$$

*This mapping is bimultiplicative.*

In effect the right-hand side of (13) is an n-th root of unity which only depends on the residue class mod $ K^{*n} $ of $ \theta^n $; this proves the first assertion. The second assertion is verified without difficulty.

For every Galois extension L of K let us write

$$
k_L : (L^n \cap K^*)/K^{*n} \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mu_n(K)) ,
$$
$$
k'_L : \mathrm{Gal}(L/K) \to \mathrm{Hom}((L^n \cap K^*)/K^{*n}, \mu_n(K)) ,
$$

for the homomorphisms derived from the above bimultiplicative mapping (V, p. 87).

#### Proposition 9 {#alg-v-s11-prop-9 .statement}

*For every Galois extension of finite degree L of K, the homomorphism $ k_L $ is bijective.*

Let $ 0 \in L^* $ be such that $ 0^n \in K $ and the residue class of $ 0^n \mod K^{*n} $ belongs to the kernel of $ k_L $. For every $ \sigma \in \mathrm{Gal}(L/K) $ we have by definition $ \sigma(\theta) = 0 $; hence $ 0 \in K^* $ and $ \theta^n \in K^{*n} $. This proves the injectivity of $ k_L $. Now let $ f : \mathrm{Gal}(L/K) \to \mu_n(K) $ be a homomorphism; for all $ \sigma, \tau \in \mathrm{Gal}(L/K) $ we have

$$
f(\sigma \tau) = f(\sigma) f(\tau) = f(\sigma) \cdot \sigma f(\tau) , \quad f(\sigma)^n = 1 .
$$

By V, p. 65, Cor. 1 there exists $ 0 \in L^* $ such that $ f(\sigma) = \sigma(\theta)/\theta $ for all $ \sigma \in \mathrm{Gal}(L/K) $; since $ f(\sigma)^n = 1 $, we have $ \sigma(\theta^n) = 0^n $ for all $ \sigma \in \mathrm{Gal}(L/K) $, hence $ 0^n \in K^* $; if $ a $ is the residue class of $ \theta^n \mod K^{*n} $, we have by definition $ f(\sigma) = \langle \sigma, a \rangle $ for $ \sigma \in \mathrm{Gal}(L/K) $, hence $ f = k_L(a) $.

#### Corollary {#alg-v-s11-n8-cor-1 .statement}

*If L is a Galois extension of K, the homomorphism $ k_L $ is injective and its image is the group $ \mathrm{Hom}_c(\mathrm{Gal}(L/K), \mu_n(K)) $ of continuous homomorphisms of the topological group $ \mathrm{Gal}(L/K) $ into the discrete group $ \mu_n(K) $.*

This follows at once from what has been said, using the fact that L is an increasing directed union of Galois extensions $ L_i $ of finite degree and that the homomorphism of $ \mathrm{Gal}(L/K) $ into $ \mu_n(K) $ is continuous if and only if it can be factored through one of the quotients $ \mathrm{Gal}(L_i/K) $ of $ \mathrm{Gal}(L/K) $.

#### Theorem 4 {#alg-v-s11-thm-4 .statement}

*a) The mapping $ H \mapsto K(H^{1/n}) $ is an inclusion preserving bijection of the set of subgroups of $ K^* $ containing $ K^{*n} $ onto the set of abelian subextensions of exponent dividing n of $ \Omega $. The inverse mapping is $ L \mapsto L'' \cap K^* $.

b) For every subgroup H of $ K^* $ containing $ K^{*n} $ the homomorphism

$$
k' : \mathrm{Gal}(K(H^{1/n})/K) \to \mathrm{Hom}(H/K^{*n}, \mu_n(K))
$$

is bijective, and it is a homeomorphism when the group $ \mathrm{Hom}(H/K^{*n}, \mu_n(K)) $ is equipped with the topology of simple convergence.

c) Let H be a subgroup of $ K^* $ containing $ K^{*"n} $. For every $ a \in H/K^{*n} $ let $ \theta_a $ be an element of $ \Omega $ such that $ \theta_a^n $ is a representative of a in H. Then the $ \theta_a, a \in H/K^{*n} $, form a basis of the vector K-space $ K(H^{1/n}) $. In particular,

$$
[K(H^{1/n}):K] = (H:K^{*"n}) .
$$

A) For every abelian extension L of K of exponent dividing n let us put $ H_L = L'' \cap K^* $. If $ [L:K] $ is finite, the homomorphism $ k'_L $ of $ \mathrm{Gal}(L/K) $ into $ \mathrm{Hom}(H_L, \mu_n(K)) $ is bijective by Prop. 9 and V, p. 88, Prop. 8.

Since every abelian extension of K of exponent dividing $ n $ is an increasing directed union of abelian subextensions of finite degree of exponent dividing $ n $, we deduce by passage to inverse limits that $ k'_L $ is a homeomorphism of topological groups for every abelian extension L of K dividing n.

B) Let L be an abelian extension of finite degree, of exponent dividing $ n $, of K, and let $ L' = K(H_L^{1/n}) $; this is a subextension of L ; moreover $ H_{L'} $ contains $ H_L $ and so is equal to it. Since the homomorphisms $ k'_L $ and $ k'_{L'} $ are bijective by A) and $ H_L = H_{L'} $, the groups Gal$(L/K)$ and Gal$(L'/K)$ have the same order and so are equal. This shows that $ L' = L $, and hence that $ L = K(H_L^{1/n}) $. If L is an abelian extension of exponent dividing $ n $ of K, we have $ K(H_L^{1/n}) = L $, because $ K(H_L^{1/n}) $ is a subextension of L which contains every subextension of finite degree of L.

C) Let H be a subgroup of $ K^* $ containing $ K^{*n} $; put $ L = K(H^{1/n}) $, then this is an abelian extension of K of exponent dividing $ n $ (V, p. 88, Lemma 5). We have $ H \subset H_L $, whence we obtain an exact sequence of commutative groups annihilated by $ n $

$$
\{1\} \to H/K^{*n} \to H_L/K^{*n} \to H_L/H \to \{1\}.
$$

From this we obtain an exact sequence

$$
\{1\} \to \operatorname{Hom}(H_L/H, \mu_n(K)) \to \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) \xrightarrow{\iota} \operatorname{Hom}(H/K^{*n}, \mu_n(K)),
$$

where $ \iota $ is the restriction homomorphism.

If we identify $ \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) $ with Gal$(L/K)$ by means of the isomorphism $ k'_L $, the kernel of $ \iota $ is identified with the set of $ \sigma \in \operatorname{Gal}(L/K) $ such that $ \sigma(\theta) = \theta $ for all $ \theta \in H^{1/n} $. It follows that $ \iota $ is injective, hence $ \operatorname{Hom}(H_L/H, \mu_n(K)) $ is reduced to (1) ; by Cor. 1 of V, p. 87 we thus have $ H = H_L $. This completes the proof of a) and b).

D) Let us prove c). If $ a, b \in H $, we have $ \theta_a \theta_b / \theta_{ab} \in K $. It follows that the vector subspace of $ K(H^{1/n}) $ generated by the $ \theta_a $ is stable under multiplication and so coincides with $ K(H^{1/n}) $. It only remains to show that the $ \theta_a $ are linearly independent ; to do this we may evidently assume that $ H/K^{*n} $ is finite ; then $[K(H^{1/n}) : K] = (\operatorname{Gal}(K(H^{1/n})/K) : \{1\}) = (H : K^{*n})$ by b) and Cor. 2 of V, p. 87 ; since the number of $ \theta_a $ is equal to $ (H : K^{*n}) $ and they generate the vector K-space $ K(H^{1/n}) $, they are linearly independent.

#### Example 1 {#alg-v-s11-n8-exa-1 .statement}

There exists a largest abelian extension of exponent dividing $ n $ of K, contained in $ \Omega $ ; it is obtained by adjoining to K the n-th roots of all its elements ; its Galois group may be identified with $ \operatorname{Hom}(K^*/K^{*n}, \mu_n(K)) $, hence also with $ \operatorname{Hom}(K^*, \mu_n(K)) $.

#### Example 2 {#alg-v-s11-n8-exa-2 .statement}

Let us take $ K = \mathbf{Q} $ and $ n = 2 $. Then $ \mathbf{Q}^*/\mathbf{Q}^{*2} $ is a vector $ \mathbf{F}_2 $-space having as a basis the union of $\{-1\}$ and the set of all prime numbers. The largest abelian extension of exponent 2 of Q contained in $ \mathbf{C} $ is thus the subfield $ \mathbf{Q}(i, \sqrt{2}, \sqrt{3}, \sqrt{5}, \ldots) $ of $ \mathbf{C} $. Its Galois group consists of all the automorphisms obtained by multiplying each of the elements $ i,\ \sqrt{2},\ \sqrt{3},\ \sqrt{5} $ etc. by $ \pm 1 $. \*

#### Example 3 {#alg-v-s11-n8-exa-3 .statement}

Let L be a cyclic extension of K of degree $ n $; then the group $ (L^n \cap K^*)/K^{*n} $ is cyclic of order $ n $. If $ a \in K^* $ is such that the residue class of $ a $ mod $ K^{*n} $ is a generator of this group, then L is K-isomorphic to $ K[X]/(X^n - a) $ and the group $ \mathrm{Gal}(L/K) $ consists of the $ n $ automorphisms mapping $ X $ to $ \zeta X $, $ \zeta \in \mu_n(K) $.

#### Example 4 {#alg-v-s11-n8-exa-4 .statement}

Conversely let $ a \in K^* $ and let $ r $ be the least integer $ > 0 $ such that $ a' \in K^{*n} $; then the subfield $ L $ of $ \Omega $ generated by the roots of the polynomial $ X^n - a $ is a cyclic extension of $ K $ of degree $ r $. In particular, $ X^n - a $ is irreducible if and only if $ r = n $.

#### Remark {#alg-v-s11-n8-rem-1 .statement}

Let $ a \in K^* $ and let r be the least integer $ > 0 $ such that $ a' \in K^n $. Let B be the set of roots in K of the polynomial $ X^{n/r} - a $; then we have

$$
X^n - a = \prod_{b \in B} (X' - b),
$$

by substitution of $ X' $ for T in the relation $ T^{n/r} - a = \Pi (T - b) $. By Example 4 each of the polynomials $ X' - b $ is irreducible, so that (14) is the decomposition of $ X^n - a $ into irreducible polynomials in $ K[X] $.

### 9. Artin-Schreier theory

In this No. we shall use $ p $ to denote a prime number and assume that K is of characteristic $ p $. We denote by $ \Omega $ an algebraic closure of K and by $ \varphi $ the endomorphism of the additive group of $ \Omega $ defined by

$$
\varphi(x) = x^p - x.
$$

By V, p. 93 the kernel of $ \varphi $ is the prime subfield $ \mathbf{F}_p $ of $ K $. For every subset $ A $ of K we denote by $ K(\varphi^{-1}(A)) $ the subextension of $ \Omega $ generated by all $ x \in \Omega $ such that $ \varphi(x) \in A $.

#### Lemma 7 {#alg-v-s11-lem-7 .statement}

$ K(\varphi^{-1}(A)) $ is an abelian extension of $ K $ of exponent dividing $ p $.

Since the polynomials $ \varphi - a = X^p - X - a,\ a \in A $ are separable over $ K $, the extension $ L = K(\varphi^{-1}(A)) $ is Galois. Let $ a \in \mathrm{Gal}(L/K) $ and $ x \in \varphi^{-1}(A) $; we have $ \varphi(\sigma(x)) = \varphi(x) $, hence $ \sigma(x) - x \in \mathbf{F}_p $, that is, $ \sigma(x) = x + i,\ i \in \mathbf{F}_p $. This implies that $ \sigma^p(x) = x + pi = x $, hence $ u^p = 1 $; similarly if $ a' \in \mathrm{Gal}(L/K) $ and $ \sigma'(x) = x + j $, then we have $ \sigma \circ \sigma'(x) = x + i + j = a' \circ \sigma(x) $, so $ \sigma \circ \sigma' = \sigma' \circ \sigma $.

#### Lemma 8 {#alg-v-s11-lem-8 .statement}

Let L be a Galois extension of K. There exists a unique mapping $ (\sigma, a) \mapsto [a, a') $ of $ \mathrm{Gal}(L/K) \times ((\varphi(L) \cap K)/\varphi(K)) $ into $ \mathbf{F}_p $ such that for all $ \sigma \in \mathrm{Gal}(L/K) $ and every element $ x \in L $ such that $ \varphi(x) \in K $ we have, on denoting by $ \overline{\varphi(x)} $ the residue class of $ \varphi(x) $ mod $ \varphi(K) $,

$$
[\sigma, \overline{\varphi(x)}] = \sigma(x) - x.
$$

This mapping is Z-bilinear (for $ \sigma, \tau \in \mathrm{Gal}(L/K) $, $ a, b \in (\mathcal{P}(L) \cap K)/\mathcal{P}(K) $, we have $ [\sigma \tau, a) = [\sigma, a) + [\tau, a) $, $ [\sigma, a + b) = [\sigma, a) + [a, b) $).

For the right-hand side of (15) is an element of $ \mathbf{F}_p $ which depends only on the residue class of $ \mathcal{P}(x) \mod \mathcal{P}(K) $; this proves the first assertion; the second may be verified without difficulty.

For every Galois extension $ L $ of $ K $ let us write

$$
a_ : (\mathcal{P}(L) \cap K)/\mathcal{P}(K) \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mathbf{F}_p)
$$
$$
a_L' : \mathrm{Gal}(L/K) \to \mathrm{Hom}((\mathcal{P}(L) \cap K)/\mathcal{P}(K), \mathbf{F}_p)
$$

for the homomorphisms obtained from the above Z-bilinear mapping (V, p. 87).

#### Proposition 10 {#alg-v-s11-prop-10 .statement}

*For every Galois extension $ L $ of finite degree of $ K $, the homomorphism $ a_ $ is bijective.*

Let $ x \in L $ be such that $ \mathcal{P}(x) \in K $ and the residue class of $ \mathcal{P}(x) \mod \mathcal{P}(K) $ lies in the kernel of $ a_ $. For every $ \sigma \in \mathrm{Gal}(L/K) $ we have by definition $ \sigma(x) = x $; hence $ x \in K $ and $ \mathcal{P}(x) \in \mathcal{P}(K) $. This proves the injectivity of $ a_ $. Now let $ f : \mathrm{Gal}(L/K) \to \mathbf{F}_p $ be a homomorphism; for all $ \sigma, \tau \in \mathrm{Gal}(L/K) $ we have

$$
f(\sigma \tau) = f(\sigma) + \sigma(f(\tau)), \quad f(\sigma) \in \mathbf{F}_p.
$$

By V, p. 65, Cor. 2 there exists $ x \in L $ such that $ f(u) = \sigma(x) - x $ for all $ o \in \mathrm{Gal}(L/K) $. Since $ f(o) \in \mathbf{F}_p $ we have $ \mathcal{P}(\sigma(x)) = \mathcal{P}(x) $, hence $ \sigma(\mathcal{P}(x)) = \mathcal{P}(x) $ for all $ a \in \mathrm{Gal}(L/K) $ and $ \mathcal{P}(x) \in K $. If $ a $ is the residue class of $ \mathcal{P}(x) \mod \mathcal{P}(K) $, we have $ f(\sigma) = [\sigma, a) $, so $ f = a_L(a) $.

#### Corollary {#alg-v-s11-n9-cor-1 .statement}

*If $ L $ is a Galois extension of $ K $, the homomorphism $ a_ $ is injective and its image is the group $ \mathrm{Hom}_c(\mathrm{Gal}(L/K), \mathbf{F}_p) $ of continuous homomorphisms of the topological group $ \mathrm{Gal}(L/K) $ into the discrete group $ \mathbf{F}_p $.*

This is proved in the same way as the Cor. of Prop. 9, V, p. 89.

#### Theorem 5 {#alg-v-s11-thm-5 .statement}

*a) The mapping $ A \mapsto K(\mathcal{P}^{-1}(A)) $ is a bijection of the set of subgroups of $ K $ containing $ \mathcal{P}(K) $ onto the set of abelian subextensions of exponent dividing $ p $ in $ \Omega $. The inverse mapping is $ L \mapsto \mathcal{P}(L) \cap K $.
b) For every subgroup $ A $ of $ K $ containing $ \mathcal{P}(K) $, the homomorphism

$$
a' : \mathrm{Gal}(K(\mathcal{P}^{-1}(A))/K) \to \mathrm{Hom}(A/\mathcal{P}(K), \mathbf{F}_p)
$$

is bijective, and it is a homeomorphism when $ \mathrm{Hom}(A/\mathcal{P}(K), \mathbf{F}_p) $ is equipped with the topology of simple convergence.
c) Let $ A $ be a subgroup of $ K $ containing $ \mathcal{P}(K) $ and let $ B $ be a basis of the vector $ \mathbf{F}_p $-space $ A/\mathcal{P}(K) $. For each $ a \in B $ let $ x_a $ be an element of $ \Omega $ such that $ \mathcal{P}(x_a) $ is a representative of $ a $ in $ A $. Then the monomials $ x^\alpha = \prod_{a \in B} x_a^{\alpha(a)} $ with a = (\alpha(a)) in N^{(B)} such that 0 \leq \alpha(a) < p for each a \in B form a basis of the vector K-space K(\mathfrak{p}^{-1}(A)). In particular we have [K(\mathfrak{p}^{-1}(A)):K] = (A:\mathfrak{p}(K)).

Th. 5 is proved in the same way as Th. 4 (V, p. 89) mutatis mutandis.

#### Example 1 {#alg-v-s11-n9-exa-1 .statement}

There exists a greatest abelian extension of K of exponent dividing p, contained in \Omega; it is K(B^1(K)), its Galois group may be identified with Horn(K/\mathfrak{p}(K),\mathbf{F}_p).

#### Example 2 {#alg-v-s11-n9-exa-2 .statement}

Let L be a cyclic extension of K of degree p; then the group (\mathfrak{p}(L) \cap K)/\mathfrak{p}(K) is cyclic of order p. If a \in K is such that the residue class of a mod \mathfrak{p}(K) is a generator of this group, then L is K-isomorphic to K[X]/(X^p - X - a) and the Galois group Gal(L/K) consists of the p automorphisms mapping X to X + i, i \in \mathbf{F}_p.

#### Example 3 {#alg-v-s11-n9-exa-3 .statement}

Conversely, if a \in K - \mathfrak{p}(K), then the polynomial X^p - X - a is irreducible and the subfield L of \Omega generated by its roots is a cyclic extension of K of degree p. If a \in \mathfrak{p}(K), then X^p - X - a = \prod_{a \in \mathfrak{p}^{-1}(a)} (X - \alpha).

### Exercises {#alg-v-s11-exercises}

See the [exercises for § 11](exercises/s11/).
