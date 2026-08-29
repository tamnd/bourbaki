---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 2
section_title: Dimension des algèbres
lang: en
source: ac-viii-ix-fr
book_pages: AC VIII.13-AC VIII.23
pdf_pages: 0017-0027, 0088-0090
extraction: ocr
subsections:
    - "no": 1
      title: Dimension et platitude
      page: 13
      pdf_page: 17
    - "no": 2
      title: Dimension d’une algèbre de type fini
      page: 16
      pdf_page: 20
    - "no": 3
      title: Dimension d’une algèbre entière
      page: 0
      pdf_page: 21
    - "no": 4
      title: Algèbres de type fini sur un corps
      page: 19
      pdf_page: 23
statements: 32
exercises: 18
content_sha256: b8e1ebd3e2fd9776cb8144b9349cd361f182844488973d9c0ece34efe2b398d8
translated_from: content/fr/ac/VIII/02_s2_dimension_des_algebres.md
source_lang: fr
translation_method: machine
source_content_sha256: d7066e36706438d32a22f5ef08bd4e19a169b5d80d705a7389fcb171033cec0a
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-8df9cd5f
glossary_version: 34
glossary_terms_sha256: dbb8e41135a1f96dc128e6f6f522e621ec0981b0bd2bf5171e23db77934530d3
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. DIMENSION OF ALGEBRAS

### 1. Dimension and flatness

Let $\rho : A \to B$ be a homomorphism of rings. We denote by (PM) the following condition:
(PM) There exists a B-module N faithfully flat over A such that, for every prime ideal q of B, one has $N \otimes_B \kappa(q) \neq 0$.

#### Remark 1 {#ac-viii-s2-n1-rem-1 .statement}

The condition (PM) is satisfied when there exists a finitely generated B-module, faithfully flat over A and with support equal to Spec(B). This is the case, in particular, if the A-module B is faithfully flat.

#### Remark 2 {#ac-viii-s2-n1-rem-2 .statement}

The existence of a B-module N faithfully flat over A implies the injectivity of ρ (I, § 3, No. 5, prop. 8), and the surjectivity of the mapping “ρ : Spec(B) → Spec(A) (II, § 2, No. 5, cor. 4 to prop. 11).

#### Remark 3 {#ac-viii-s2-n1-rem-3 .statement}

Suppose that ρ : A → B is a local homomorphism of local rings and that there exists a B-module N flat over A and such that N ⊗_B κ(q) ≠ 0 for every prime ideal q of B. Then N is faithfully flat over A and ρ therefore has the property (PM): indeed we have N/m_B N = N ⊗_B κ(m_B) ≠ 0, hence N ≠ m_B N and fortiori N ≠ m_A N, and the conclusion follows from prop. 1 of I, § 3, No. 1.

#### Proposition 1 {#ac-viii-s2-prop-1 .statement}

Let ρ : A → B be a homomorphism of rings satisfying the condition (PM).

a) Let h : A → A′ be a homomorphism of rings. Then the homomorphism ρ′ : A′ → A′ ⊗_A B deduced from ρ satisfies the condition (PM).

b) Let q be a prime ideal of B and p = ρ^{-1}(q). The canonical homomorphism ρ_q : A_p → B_q satisfies the condition (PM).

c) Let q be a prime ideal of B and p = ρ^{-1}(q). For every prime ideal p′ of A contained in p, there exists a prime ideal q′ of B lying above p′ and contained in q.

Let N be a B-module faithfully flat over A and such that N ⊗_B κ(q) ≠ 0 for every prime ideal q of B.

Prove a). The A′-module N′ = A′ ⊗_A N is faithfully flat (I, § 3, No. 3, prop. 5); let q′ be a prime ideal of B′ = A′ ⊗_A B and q its inverse image in B. We have isomorphisms

$$ N' \otimes_{B'} \kappa(q') \to N \otimes_B \kappa(q') \to (N \otimes_B \kappa(q)) \otimes_{\kappa(q)} \kappa(q'); $$

as we have N ⊗_B κ(q) ≠ 0, we also have N′ ⊗_{B′} κ(q′) ≠ 0.

Prove b). According to props. 13 and 14 of II, § 3, No. 4, the A_p-module N_q is flat. On the other hand, let b′ be a prime ideal of B_q; it is of the form bB_q where b is a prime ideal of B contained in q (II, § 3, No. 1, prop. 3); we have N ⊗_B κ(b) ≠ 0 in view of the assumption made on N, and since N_q ⊗_{B_q} κ(b′) is isomorphic to N ⊗_B κ(b′), we have N_q ⊗_{B_q} κ(b′) ≠ 0. Remark 3 allows us to conclude.

Prove c). The local homomorphism ρ_q : A_p → B_q deduced from ρ satisfies the condition (PM) according to b). The mapping Spec(B_q) → Spec(A_p) is therefore surjective (Remark 2), which was to be proved.

#### Corollary {#ac-viii-s2-n1-cor-1 .statement}

Let F be a closed subset of Spec(A). If Y is an irreducible component of the inverse image of F by the mapping “ρ : Spec(B) → Spec(A), then the closure of “ρ(Y) is an irreducible component of F.

Let indeed a be an ideal of A such that F = V(a) and q the prime ideal of B such that Y = V(q). The inverse image by “ρ of F is the subset V(ρ(a)B) of Spec(B) and the closure of “ρ(Y) is the irreducible closed subset V(ρ^{-1}(q)) of Spec(A).

It is a matter of proving that if q is minimal among the prime ideals of B containing $\rho(a)$, then $\rho^{-1}(q)$ is minimal among the prime ideals of A containing a. Otherwise, there would exist a prime ideal $p'$ of A with $a \subset p' \subset \rho^{-1}(q)$ and $p' \neq \rho^{-1}(q)$; according to prop. 1, c), there would exist a prime ideal $q'$ of B such that $q' \subset q$ and $p' = \rho^{-1}(q')$, whence $\rho(a) \subset q' \subset q$ and $q' \neq q$ contrary to the assumption made on q.

#### Proposition 2 {#ac-viii-s2-prop-2 .statement}

Let $\rho : A \to B$ be a homomorphism of nonzero rings possessing the property (PM). One has the inequality

(1)
$$
\dim(B) \geq \dim(A) + \inf_{m \in S} \dim(B/mB)
$$
where S is the set of maximal ideals of A.

We know that $\dim(A) = \sup_{m \in S} \dim(A_m)$ (§ 1, No. 3, prop. 8). It is therefore enough to establish the inequality

(2)
$$
\dim(B) \geq \dim(A_m) + \dim(B/mB)
$$
for every maximal ideal m of A. In other words, it is a matter of proving the inequality

(3)
$$
\dim(B) \geq n + r
$$
if $p_0 \subset ... \subset p_n$ is a chain of prime ideals of A contained in m and $\overline{q}_0 \subset ... \subset \overline{q}_r$ is a chain of prime ideals of B/mB. For $0 \leq i \leq r$, there exists a prime ideal $q_{n+i}$ of B lying above m such that $\overline{q}_i = q_{n+i}/mB$, and $q_n \subset ... \subset q_{n+r}$ is a chain of prime ideals of B. Put $p'_i = p_i$ for $0 \leq i \leq n-1$ and $p'_n = m$, so that $p'_0 \subset ... \subset p'_n$ is a chain of prime ideals of A and q_n lies above $p'_n$. If $q_i$ is a prime ideal of B lying above $p'_i$ ($1 \leq i \leq n$), prop. 1, c) proves that there exists a prime ideal $q_{i-1}$ of B lying above $p'_{i-1}$ and contained in $q_i$. By descending induction, we thus construct a chain $q_0 \subset ... \subset q_n$ of prime ideals of B such that $q_i$ lies above $p_i$ for $0 \leq i \leq n$. As $q_0 \subset ... \subset q_{n+r}$ is a chain of prime ideals of B, we have proved the inequality (3).

#### Remark 4 {#ac-viii-s2-n1-rem-4 .statement}

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings satisfying condition (PM). We shall see later (§ 3, no 4, prop. 7) that in this case there is equality in (1). In the general case there may be strict inequality (p. 84, exercise 1).

#### Corollary {#ac-viii-s2-n1-cor-2 .statement}

For every ideal a of A, one has $\mathrm{ht}(a) \leq \mathrm{ht}(\rho(a)B)$.

Let q be a prime ideal of B containing $\rho(a)B$, and $p = \rho^{-1}(q)$. According to prop. 1, the local homomorphism $\rho_q : A_p \to B_q$ deduced from $\rho$ satisfies (PM), and we therefore have $\dim(A_p) \leq \dim(B_q)$ according to prop. 2. According to prop. 7 of § 7, no 3, we have $\mathrm{ht}(a) \leq \dim(A_p)$ since p contains a, whence $\mathrm{ht}(a) \leq \dim(B_q)$ for every prime ideal q of B containing $\rho(a)B$. The corollary then follows from loc. cit.

#### Lemma 1 {#ac-viii-s2-lem-1 .statement}

Let $\rho : A \to B$ be a homomorphism of rings and p a prime ideal of A. The continuous mapping $^a h : \mathrm{Spec}(B \otimes_A \kappa(p)) \to \mathrm{Spec}(B)$, associated with the canonical homomorphism $h : B \to B \otimes_A \kappa(p)$, *induces a homeomorphism of* $\mathrm{Spec}(B \otimes_A \kappa(p))$ *onto the subspace* $(\alpha\rho)^{-1}(p)$ *of* $\mathrm{Spec}(B)$ *formed by the prime ideals of* $B$ *lying above* $p$.

The homomorphism $h$ is composed of the homomorphism of passing to the quotient of $B$ into $B/\rho(p)$ $B$ and of the canonical homomorphism of $B/\rho(p)$ $B$ into its ring of fractions $(\rho(A - p))^{-1}(B/\rho(p) \ B)$. According to the remark and the corollary to prop. 13 of II, § 4, no 3, $^a h$ therefore induces a homeomorphism of $\mathrm{Spec}(B \otimes_A \kappa(p))$ onto the subspace of $\mathrm{Spec}(B)$ formed by the prime ideals $q$ of $B$ which contain $\rho(p)$ and are disjoint from $\rho(A - p)$, that is to say which lie above $p$.

#### Remark 5 {#ac-viii-s2-n1-rem-5 .statement}

According to prop. 2 and Lemma 1, we therefore have, under the hypotheses of prop. 2, the inequality
$$
\dim(\mathrm{Spec}(B)) \geq \dim(\mathrm{Spec}(A)) + \inf_{p \in \mathrm{Spec}(A)} \dim(\alpha\rho^{-1}(p)) .
$$

### 2. Dimension of an algebra of finite type

#### Proposition 3 {#ac-viii-s2-prop-3 .statement}

*Let* $\rho : A \to B$ *be a homomorphism of rings*. *Put*
$n = \sup_{p \in \mathrm{Spec}(A)} \dim(B \otimes_A \kappa(p))$. *One has the inequality*
$$
\dim(B) + 1 \leq (\dim(A) + 1).(n + 1) .
$$

We may suppose $\dim(A) \neq -\infty$ and $n < +\infty$. Let $q_0 \subset ... \subset q_m$ be a chain of prime ideals of B; put $p_i = \rho^{-1}(q_i)$. The sequence of the $p_i$ is increasing, hence the set of its values has cardinal $\leq \dim(A) + 1$. For each $p \in \mathrm{Spec}(A)$, the set of the $q_j$ such that $p_j = p$ is a chain of the subset $^a\rho^{-1}(p)$ of $\mathrm{Spec}(B)$, hence has cardinal less than $\dim(B \otimes_A \kappa(p)) + 1$ (no 1, Lemma 1), and consequently less than or equal to $(n + 1)$. It follows that $m + 1 \leq (\dim(A) + 1)(n + 1)$, whence the proposition.

#### Remark 1 {#ac-viii-s2-n2-rem-1 .statement}

If the rings $A$ and $B$ are noetherian, we shall see below (§ 3, no 4, cor. 2 to prop. 7) that one has the inequality $\dim(B) \leq \dim(A) + n$, stronger than that of prop. 3.

#### Corollary 1 {#ac-viii-s2-prop-3-cor-1 .statement}

*Suppose that one has* $\dim(A) < +\infty$ *and that there exists an integer* $n$ *such that* $\dim(B \otimes_A \kappa(p)) \leq n$ *for every* $p \in \mathrm{Spec}(A)$. *Then one has* $\dim(B) < +\infty$.

#### Corollary 2 {#ac-viii-s2-prop-3-cor-2 .statement}

*Let* $A$ *be a ring and* $B = A[X]$ *the ring of polynomials in one indeterminate with coefficients in* $A$. *One has* :
$$
1 + \dim(A) \leq \dim(B) \leq 1 + 2\dim(A) .
$$

The first inequality has already been proved (§ 1, No. 3, example 4). Let us prove the second one. For every prime ideal $p$ of $A$, the ring $B \otimes_A \kappa(p)$, isomorphic to $\kappa(p)[X]$, is principal and is not a field, hence is of dimension 1 (§ 1, No. 3, example 2), and the inequality follows from prop. 3.

However, whatever the integers n and q with n + 1 ≤ q ≤ 2n + 1 may be, there exists a ring A of dimension n such that dim(A[X]) = q (see p. 84, exerc. 7).

#### Corollary 3 {#ac-viii-s2-prop-3-cor-3 .statement}

If A is of finite dimension, every nonzero finitely generated A-algebra is of finite dimension.

Indeed, one deduces from cor. 2, by induction on n, that the ring A[T₁, ..., Tₙ] is of finite dimension if A is of finite dimension; fortiori, every nonzero quotient of A[T₁, ..., Tₙ] is of finite dimension (§ 1, No. 3, prop. 6).

### 3. Dimension of an integral algebra

#### Lemma 2 {#ac-viii-s2-lem-2 .statement}

Let ρ : A → B be a homomorphism of rings such that, for every prime ideal p of A, the κ(p)-algebra B ⊗ₓₐ κ(p) is integral (V, § 1, No. 1, def. 2). Let q and q’ be two prime ideals of B such that q ⊂ q’ and q ≠ q’. Then ρ⁻¹(q) ≠ ρ⁻¹(q’).

Indeed, if q and q’ are over the same prime ideal p of A, one has dim(B ⊗ₓₐ κ(p)) ≥ 1 by Lemma 1 of No. 1, which contradicts the fact that dim(B ⊗ₓₐ κ(p)) ≤ 0 (§ 1, No. 3, example 6).

#### Theorem 1 {#ac-viii-s2-thm-1 .statement}

Let ρ : A → B be a homomorphism of rings making B an integral A-algebra.

a) Let M be a finitely generated A-module. Then one has dim_B(M ⊗ₓₐ B) ≤ dim_A(M). In particular, one has dim(B) ≤ dim(A). If the mapping “ρ : Spec(B) → Spec(A) is surjective, for example (V, § 2, No. 1, th. 1) if ρ is injective, one has dim_B(M ⊗ₓₐ B) = dim_A(M), and in particular dim(B) = dim(A).

b) Let b be an ideal of B and a = ρ⁻¹(b) its inverse image in A. One has ht(b) ≤ ht(a) and dim(B/b) = dim(A/a). If “ρ : Spec B → Spec A is surjective, one has ht(aB) ≤ ht(a) for every ideal a of A.

c) Suppose that B is finite over A and let N be a finitely generated B-module. Then one has dim_B(N) = dim_A(N). In particular, one has dim(B) = dim_A(B).

Let us prove a). By prop. 5 of V, § 1, No. 1, the κ(p)-algebra B ⊗ₓₐ κ(p) is integral for every prime ideal p of A. Let q₀ ⊂ ... ⊂ qₘ be a chain of prime ideals of B; by Lemma 2, the ideals pᵢ = ρ⁻¹(qᵢ) are pairwise distinct, hence p₀ ⊂ ... ⊂ pₘ is a chain of prime ideals of A, whence m ≤ dim(A). Hence dim(B) ≤ dim(A).

Suppose now that the mapping “ρ is surjective. Let p₀ ⊂ ... ⊂ pₙ be a chain of prime ideals of A; there exists therefore a prime ideal q₀ of B over p₀. By cor. 2 to the first existence theorem (V, § 2, No. 1, th. 1), one can construct, by induction on n, a chain q₀ ⊂ ... ⊂ qₙ of prime ideals of B such that qᵢ is over pᵢ for 0 ≤ i ≤ n. Hence n ≤ dim(B) and consequently dim(A) ≤ dim(B).

This proves $a$ in the case where $M = A$. In the general case, let $a$ be the annihilator of $M$, so that the support of $M$ is identified with $\operatorname{Spec}(A/a)$, and one has $\dim_A(M) = \dim(A/a)$. By II, § 4, No. 4, prop. 19, the support of $M \otimes_A B$ is the inverse image by $^a\rho$ of the support of $M$, hence is identified with $\operatorname{Spec}(B/\rho(a) B)$, and one has $\dim_B(M \otimes_A B) = \dim(B/\rho(a) B)$. It remains to observe that the homomorphism $\rho': A/a \to B/\rho(a) B$ deduced from $\rho$ makes $B/\rho(a) B$ an $(A/a)$-algebra integral, and that “$\rho'$ is surjective when $^a\rho$ is so.

Let us prove $b$. By prop. 7 of § 1, No. 3, it suffices to prove that $\operatorname{ht}(b) \leq \dim(A_p)$ for every prime ideal $p$ of $A$ containing $a$; let $p$ be such an ideal. By V, § 2, No. 1, cor. 2 to th. 1, there exists a prime ideal $q$ of $B$ over $p$ and containing $b$, and one has $\operatorname{ht}(b) \leq \dim(B_q)$ by prop. 7 of § 1, No. 3.

Now $B_q$ identifies with a ring of fractions of the $A_p$-algebra $B \otimes_A A_p$, whence
$$
\dim(B_q) \leq \dim(B \otimes_A A_p) \leq \dim(A_p)
$$
by Prop. 6 of § 1, No. 3 and the assertion $a$ above. We have thus proved the inequality $\operatorname{ht}(b) \leq \operatorname{ht}(a)$. Moreover, the homomorphism from $A/a$ into $B/b$ deduced from $\rho$ is injective and makes $B/b$ an $(A/a)$-algebra which is integral; we therefore have $\dim(B/b) = \dim(A/a)$ by $a$. Suppose “$\rho$ is surjective and let $a$ be an ideal of $A$ and $p$ a prime ideal of $A$ containing $a$. There exists by assumption a prime ideal $q$ of $B$ lying above $p$. We have $aB \subset q$, whence $\operatorname{ht}(aB) \leq \operatorname{ht}(q) \leq \operatorname{ht}(p)$ by what precedes. Passing to the greatest lower bound, we obtain $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$.

Finally, $c$ follows from $b$ applied to the annihilator $b$ of $N$.

#### Theorem 2 {#ac-viii-s2-thm-2 .statement}

Let $A$ be an integrally closed ring, and $B$ a ring containing $A$, integral over $A$. Assume that $B$ is a torsion-free $A$-module. For every ideal $a$ of $A$, one has $\operatorname{ht}(a) = \operatorname{ht}(aB)$. Let $b$ be an ideal of $B$ and $a = b \cap A$; one then has $\operatorname{ht}(a) = \operatorname{ht}(b)$.

Soit $\rho$ l’application canonique de $A$ dans $B$. Soient $a$ un idéal de $A$. Si $a = A$, la première égalité est claire. Supposons $a \neq A$. Comme $\rho$ est injectif, $^a\rho$ est surjectif (V, § 2, No. 1, Theorem 1). Par suite $aB \neq B$. Soit alors $q$ un idéal premier de $B$ contenant $aB$. Posons $p = q \cap A$. On a $a \subset p$, d’où $\operatorname{ht}(a) \leq \operatorname{ht}(p)$. Soit $p_0 \subset ... \subset p_n$ une chaîne d’idéaux premiers de $A$ avec $p_n = p$. D’après le deuxième théorème d’existence (V, § 2, No. 4, Theorem 3), on construit par récurrence une chaîne $q_0 \subset ... \subset q_n$ d’idéaux premiers de $B$ telle que $q_n = q$ et $q_i$ soit au-dessus de $p_i$ pour $0 \leq i \leq n$. On a $n \leq \operatorname{ht}(q)$, d’où $\operatorname{ht}(a) \leq \operatorname{ht}(q)$. En passant à la borne inférieure on obtient $\operatorname{ht}(a) \leq \operatorname{ht}(aB)$ ($§ 1$, No. 3, Prop. 7). L’inégalité $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$ résulte du Theorem 1, d’où la première equality. Soit $b$ un idéal de $B$. Posons $a = \rho^{-1}(b)$. On a $aB \subset b$, d’où $\operatorname{ht}(a) = \operatorname{ht}(aB) \leq \operatorname{ht}(b)$. L’inégalité $\operatorname{ht}(b) \leq \operatorname{ht}(a)$ résulte du Theorem 1, d’où le theorem.

#### Remark {#ac-viii-s2-n3-rem-1 .statement}

Soient $A$ un anneau intègre et $B$ un anneau contenant $A$, entier sur $A$. Soit $p$ un idéal premier de $A$ tel que la clôture intégrale de $A_p$ soit un anneau local. On peut démontrer que, pour tout idéal premier $q$ de $B$ au-dessus de $p$, on a $\operatorname{ht}(p) = \operatorname{ht}(q)$ (p. 85, Exer. 9) lorsque $B$ est intègre.

### 4. Algebras of finite type over a field

Dans ce numéro, $k$ désigne un field.

#### Lemma 3 {#ac-viii-s2-lem-3 .statement}

Let $A$ be a $k$-algebra of finite type and $p_0 \subset ... \subset p_m$ a maximal chain of prime ideals of $A$. There exists an integer $n \geq m$, a sequence $(x_1, ..., x_n)$ of elements of $A$, algebraically free over $k$ (A, IV, p. 4), and such that :
a) $A$ is entire over the ring $B = k[x_1, ..., x_n]$;
b) for every $j$ such that $0 \leq j \leq m$, the ideal $p_j \cap B$ is generated by the $x_k$ with $1 \leq k \leq n - m + j$.

According to the normalization lemma (V, § 3, No. 1, th. 1), there exists an integer $n \geq 0$, a finite sequence $(x_1, ..., x_n)$ of elements of $A$ algebraically free and an increasing sequence $(h(j))_{0 \leq j \leq m}$ of integers $\leq n$ such that the ideal $p_j \cap B$ is equal to the prime ideal $q_j$ of $B$ generated by the $x_k$ with $1 \leq k \leq h(j)$, and that $A$ is entire over the ring $B$. Let $j$ be an integer such that $0 \leq j < m$. By passing to quotients, one deduces from the canonical injection of $B$ into $A$ an injective homomorphism of $B/q_j$ into $A/p_j$ which makes $A/p_j$ a finite $(B/q_j)$-algebra. Since the ring $B/q_j$ is isomorphic to an algebra of polynomials in $n - h(j)$ indeterminates over $k$, it is integrally closed (V, § 1, No. 3, Cor. 3 of Prop. 13). According to th. 2 of No. 3, one therefore has

$$
1 = \mathrm{ht}(p_{j+1}/p_j) = \mathrm{ht}(q_{j+1}/q_j) \geq h(j+1) - h(j) .
$$

It follows that one has $h(j+1) \leq h(j) + 1$ and $q_{j+1} \neq q_j$, whence $h(j+1) = h(j) + 1$. But one has $h(m) = n$ since $q_m$ is maximal (V, § 2, No. 1, Prop. 1), whence finally $h(j) = n - m + j$.

#### Theorem 3 {#ac-viii-s2-thm-3 .statement}

Let $A$ be a $k$-algebra of finite type.
a) For every minimal prime ideal $p$ of $A$, all maximal chains of prime ideals of $A$ with origin $p$ have length the integer $\deg.\mathrm{tr}_k \kappa(p)$.
b) The ring $A$ is catenary and its dimension is the supremum of the integers $\deg.\mathrm{tr}_k \kappa(p)$, where $p$ runs through the minimal prime ideals of $A$.
c) If $A$ is integral, then all maximal chains of prime ideals of $A$ have the same length, and the dimension of $A$ is the degree of transcendence over $k$ of the field of fractions of $A$.

Suppose $A$ is integral and consider a maximal chain $p_0 \subset ... \subset p_m$ of prime ideals of $A$. We have $p_0 = 0$. We deduce then from Lemma 3 the existence of an injective homomorphism $\varphi : k[X_1, ..., X_m] \to A$ of $k$-algebras which makes $A$ a finite $k[X_1, ..., X_m]$-algebra. Consequently, the degree of transcendence over $k$ of the field of fractions of $A$ is equal to $m$, whence c). Assertion a) follows from assertion c) applied to the ring $A/p$ and assertion b) is an immediate consequence of a) and Prop. 5 of § 1, No. 2.

#### Corollary 1 {#ac-viii-s2-thm-3-cor-1 .statement}

Let $n$ be a positive integer. We have

$$
\dim(k[X_1, ..., X_n]) = n .
$$

For a finite type k-algebra A to have dimension n, it is necessary and sufficient that there exist an injective k-homomorphism $\varphi : k[X_1, ..., X_n] \to A$ making A a finite algebra over $k[X_1, ..., X_n]$.

This follows from th. 3, from the normalization lemma (V, § 3, No. 1, th. 1) and from th. 1, a) of No. 3.

#### Corollary 2 {#ac-viii-s2-thm-3-cor-2 .statement}

Let A be an integral k-algebra of finite type. For every prime ideal p of A, we have

$$
\operatorname{ht}(p) = \dim(A_p) = \dim(A) - \dim(A/p)
$$
$$
= \dim(A) - \deg.\operatorname{tr}_k\kappa(p).
$$

In particular, we have $\operatorname{ht}(m) = \dim(A_m) = \dim(A)$ for every maximal ideal m of A.

This follows from th. 3 and Remark 4 of § 1, No. 3.

#### Corollary 3 {#ac-viii-s2-thm-3-cor-3 .statement}

Let A be a k-algebra of finite type and let f be an element of A which belongs to no minimal prime ideal of A (for example an element of A which is not a divisor of zero, cf. IV, § 1, No. 1, Cor. 3 to Prop. 2 and No. 3, Cor. 1 to Prop. 7). We have $\dim(A) = \dim(A_f)$.

The mapping $p \mapsto pA_f$ is a bijection of the set of minimal prime ideals of A onto the set of minimal prime ideals of $A_f$. Moreover the rings $A/p$ and $A_f/pA_f = (A/p)_f$ have the same field of fractions. It is therefore sufficient to apply th. 3, b).

#### Corollary 4 {#ac-viii-s2-thm-3-cor-4 .statement}

Let A be a k-algebra of finite type and let p be a prime ideal of A.

a) In order that p be maximal, it is necessary and sufficient that the field of fractions of $A/p$ be a finite extension of k.

b) Let $f \in A - p$; the ideal p is a maximal ideal of A if and only if $pA_f$ is a maximal ideal of $A_f$.

If p is a maximal ideal of A, then $A/p$ is a field, hence a ring of dimension 0; it is a finite type extension of k whose degree of transcendence is 0 (th. 3, c)), it is therefore a finite extension of k. Conversely, if the field of fractions of $A/p$ is a finite extension of k, we have $\dim(A/p) = 0$ hence p is maximal. Assertion b) follows from assertion a), taking into account that $A/p$ and $A_f/pA_f$ have the same field of fractions.

Assertion a) of Cor. 4 is a form of the theorem of zeros (V, § 3, No. 3, Prop. 1).

#### Corollary 5 {#ac-viii-s2-thm-3-cor-5 .statement}

Let A be a k-algebra of finite type, p a prime ideal of A and $(\mathfrak{p}_i)_{i \in I}$ the family of minimal prime ideals of A contained in p. We have:

$$
\dim_p(A) = \sup_{i \in I} \dim(A/\mathfrak{p}_i)
$$
$$
= \dim(A_p) + \dim(A/p)
$$
$$
= \dim(A_p) + \deg.\operatorname{tr}_k\kappa(p).
$$

We have $\dim_p(A) = \sup_{i \in I} \dim_{p/p_i}(A/p_i)$ (§ 1, No. 3, Prop. 6). But, according to Cor. 3, we have $\dim_{p/p_i}(A/p_i) = \dim(A/p_i)$, whence the first equality. According to Cor. 2, we have $\dim(A/p_i) = \dim((A/p_i)_p) + \dim(A/p)$. The second equality of the corollary therefore follows from the fact that $\dim(A_p) = \sup_{i \in I} \dim((A/p_i)_p)$ and the third from th. 3.

Thus $\dim_p(A)$ is the supremum of the lengths of the chains of prime ideals of $A$ of which $p$ is an element.

#### Corollary 6 {#ac-viii-s2-thm-3-cor-6 .statement}

*Let A be a finitely generated k-algebra not reduced to 0, and let n be an integer $\geqslant 0$. The following conditions are equivalent:*

a) *For every $p \in \operatorname{Ass}(A)$, one has $\dim(A/p) = n$.*

b) *Every associated prime ideal of A is minimal and all the irreducible components of Spec(A) have dimension n.*

c) *There exists an injective k-homomorphism $\varphi : k[X_1, ..., X_n] \to A$ making A a $k[X_1, ..., X_n]$-module of finite type without torsion.*

The equivalence of a) and b) is immediate. Let us show that a) implies c). According to b), the ring A has dimension n and there therefore exists (cor. 1) an injective k-homomorphism $\varphi : k[X_1, ..., X_n] \to A$ making A a $k[X_1, ..., X_n]$-module of finite type. For every prime ideal $p \in \operatorname{Ass}(A)$, the ring $A/p$ is then integral over $k[X_1, ..., X_n]$, and we therefore have $n = \dim(A/p) = \dim(k[X_1, ..., X_n]/\varphi^{-1}(p))$ by th. 1, a) of no. 3, whence $\varphi^{-1}(p) = 0$. The image by the injective homomorphism $\varphi$ of a nonzero element of $k[X_1, ..., X_n]$ is not a zero divisor in A (IV, § 1, no. 1, cor. 3 to prop. 2), whence c).

Conversely, suppose that condition c) is satisfied. For every prime ideal $p \in \operatorname{Ass}(A)$, the homomorphism $k[X_1, ..., X_n] \to A/p$ deduced from $\varphi$ is injective (*loc. cit.*). We therefore have $\dim(A/p) = n$ by cor. 1.

#### Remark 1 {#ac-viii-s2-n4-rem-1 .statement}

By cor. 5, the conditions a), b), c) of cor. 6 imply that one has $\dim_p(A) = \dim(A)$ for every prime ideal $p$ of A.

#### Proposition 4 {#ac-viii-s2-prop-4 .statement}

*Let A and B be two finitely generated k-algebras and $\rho : A \to B$ an algebra homomorphism. Suppose that A is integral and that the A-module B is without torsion, and denote by K the field of fractions of A. One has*

$$
\dim(B) = \dim(A) + \dim(B \otimes_A K).
$$

Suppose first that B is integral. The algebra $B \otimes_A K$ is then a ring of fractions of B defined by a multiplicative subset not containing 0. It therefore has as its field of fractions the field of fractions L of B. By th. 3, one has

$$
\dim(B) = \deg.\mathrm{tr}_k L,\quad \dim(A) = \deg.\mathrm{tr}_k K,
$$
$$
\dim(B \otimes_A K) = \deg.\mathrm{tr}_K L.
$$

Now, by the corollary of A, V, p. 106

$$
\deg.\mathrm{tr}_k L = \deg.\mathrm{tr}_K L + \deg.\mathrm{tr}_k K,
$$

whence the result in this case.

Let us pass to the general case. Every minimal prime ideal $p$ of $B$ is formed of zero divisors in $B$, and is therefore above the ideal 0 of $A$. It follows that the mapping $p \mapsto p . (B \otimes_A K)$ is a bijection from the set of minimal prime ideals of $B$ onto the set of minimal prime ideals of $B \otimes_A K$. The proposition therefore follows from the first part of the proof and from prop. 6, c) of § 1, no 3.

#### Corollary {#ac-viii-s2-n4-cor-1 .statement}

*Let $\rho : A \to B$ be an injective homomorphism of finitely generated k-algebras.* *One has* $\dim(A) \leq \dim(B)$.

Indeed, let $p$ be a minimal prime ideal of $A$ such that $\dim(A) = \dim(A/p)$. There exists a prime ideal $q$ of $B$ above $p$ (II, § 2, no 6, prop. 16). By prop. 4 applied to $A/p$ and $B/q$, one has $\dim(A) = \dim(A/p) \leq \dim(B/q) \leq \dim(B)$, whence the corollary.

*Lemma 4. — Let $A$ and $B$ be two integral k-algebras, $M$ an $A$-module without torsion, $N$ a $B$-module without torsion. If the ring $A \otimes_k B$ is integral, then $M \otimes_k N$ is a module without torsion over $A \otimes_k B$.*

Let $K$ (resp. $L$) be the field of fractions of $A$ (resp. $B$). There exists a set $I$ (resp. $J$) such that $M$ (resp. $N$) is isomorphic to a submodule of $K^{(I)}$ (resp. $L^{(J)}$). The $(A \otimes_k B)$-module $M \otimes_k N$ is therefore isomorphic to a submodule of $K^{(I)} \otimes_k L^{(J)}$, which is isomorphic to $(K \otimes_k L)^{(I \times J)}$. Since $K \otimes_k L$ is a ring of fractions of the integral ring $A \otimes_k B$, it is a torsion-free module over $A \otimes_k B$, whence the lemma.

*PROPOSITION 5. — Let $k'$ be an extension of $k$, $A$ a k-algebra of finite type and $B$ a $k'$-algebra of finite type.

a) *The $k'$-algebra $A \otimes_k B$ is of finite type and one has*
$$
\dim(A \otimes_k B) = \dim(A) + \dim(B).
$$

b) *Let $r$ be a prime ideal of $A \otimes_k B$; let $p$ (resp. $q$) denote the inverse image of $r$ in $A$ (resp. $B$). One has*
$$
\dim_r(A \otimes_k B) = \dim_p(A) + \dim_q(B).
$$

Put $n = \dim(A)$ and $m = \dim(B)$. By Cor. 1 to Theorem 3 there exist injective algebra homomorphisms $\varphi : k[X_1, ..., X_n] \to A$ and $\psi : k'[Y_1, ..., Y_m] \to B$ making $A$ and $B$ respectively finite algebras over $k[X_1, ..., X_n]$ and $k'[Y_1, ..., Y_m]$. The homomorphism $\varphi \otimes \psi$ is then injective and makes $A \otimes_k B$ into a finite algebra over the $k'$-algebra $k[X_1, ..., X_n] \otimes_k k'[Y_1, ..., Y_m]$, which is identified with $k'[X_1, ..., X_n, Y_1, ..., Y_m]$. Therefore $\dim(A \otimes_k B) = n + m$ by Cor. 1 to Theorem 3, which proves a).

Let us remark that when $A$ and $B$ are integral, $A \otimes_k B$ is a torsion-free $k'[X_1, ..., X_n, Y_1, ..., Y_m]$-module by Lemma 4, and that therefore one has
$$
\dim_r(A \otimes_k B) = n + m = \dim(A) + \dim(B)
$$
for every prime ideal $r$ of $A \otimes_k B$ by Remark 1.

Prove now b). Let $r_0$ be a minimal prime ideal of $A \otimes_k B$ contained in $r$, and denote by $p_0$ (resp. $q_0$) the inverse image of $r_0$ in $A$ (resp. $B$). The ring

(A \otimes_k B)/r_0 is isomorphic to a quotient of the ring (A/p_0) \otimes_k (B/q_0). We have therefore, by $a$,

$$
\dim((A \otimes_k B)/r_0) \leq \dim(A/p_0) + \dim(B/q_0).
$$

Applying cor. 5 to th. 3, we deduce the inequality

$$
\dim_r(A \otimes_k B) \leq \dim_p(A) + \dim_q(B).
$$

Conversely, let $p_0$ (resp. $q_0$) be a minimal prime ideal of A (resp. B) contained in $p$ (resp. q). According to the remark made above, we have

$$
\dim(A/p_0) + \dim(B/q_0) = \dim_{\overline{r}}((A/p_0) \otimes_k (B/q_0))
$$

where $\overline{r}$ is the image of r by the canonical surjection $A \otimes_k B \to (A/p_0) \otimes_k (B/q_0)$. The second member of the preceding equality is obviously less than $\dim_r(A \otimes_k B)$. Applying cor. 5 to th. 3, we deduce the inequality

$$
\dim_p(A) + \dim_q(B) \leq \dim_r(A \otimes_k B),
$$

which completes the proof.

#### Corollary {#ac-viii-s2-n4-cor-2 .statement}

*Let A be a finitely generated k-algebra, k' an extension of k, and A' the k'-algebra A \otimes_k k'.*

a) *We have* $\dim(A') = \dim(A)$.

b) *Let p' be a prime ideal of A' and p its inverse image in A; we have* $\dim_{p'}(A') = \dim_p(A)$.

c) *Let p' be a minimal prime ideal of A' and p its inverse image in A. Then p is minimal and we have* $\dim(A'/p') = \dim(A/p)$.

The assertions a) and b) follow from prop. 5 by taking $B = k'$. Let us prove c). The ideal p is minimal (No. 1, prop. 1) and we have

$$
\dim(A'/p') = \dim_{p'}(A') = \dim_p(A) = \dim(A/p).
$$

#### Remark 2 {#ac-viii-s2-n4-rem-2 .statement}

*Suppose that the extension k' of k is radicial. Then the canonical mapping $f : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ is a homeomorphism.*

Let indeed $p \in \mathrm{Spec}(A)$. By Lemma 1 of No. 1, the space $f^{-1}(\{p\})$ is homeomorphic to $\mathrm{Spec}(\kappa(p) \otimes_k k')$. Now the set a of nilpotent elements of $\kappa(p) \otimes_k k'$ is a prime ideal (A, V, p. 134, corollary) and the quotient ring $(\kappa(p) \otimes_k k')/a$, integral and finite over $\kappa(p)$, is a field (A, V, p. 16, cor. 1 and p. 10, prop. 1). Consequently $f^{-1}(\{p\})$ is reduced to one element. It follows that the mapping $f$ is an increasing bijection of $\mathrm{Spec}(A')$ onto $\mathrm{Spec}(A)$, these two sets being ordered by inclusion of the prime ideals, and hence induces a bijection between the irreducible closed subsets of $\mathrm{Spec}(A)$ and those of $\mathrm{Spec}(A')$. Since the closed subsets of $\mathrm{Spec}(A)$ (resp. $\mathrm{Spec}(A')$) are finite unions of irreducible closed subsets, $f$ is a homeomorphism.

For a generalization, see exerc. 24, p. 98.

## EXERCISES {#ac-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
