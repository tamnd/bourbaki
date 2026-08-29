---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 4
section_title: Anneaux réguliers
lang: en
source: ac-x-fr
pdf_pages: 0052-0060, 0161-0164
extraction: ocr
subsections:
    - "no": 1
      title: Propriétés homologiques élémentaires des anneaux locaux réguliers
      page: 0
      pdf_page: 52
    - "no": 2
      title: Caractérisation homologique des anneaux noethériens réguliers
      page: 54
      pdf_page: 53
    - "no": 3
      title: Anneaux réguliers et algèbres finies
      page: 0
      pdf_page: 56
    - "no": 4
      title: Anneaux présentables
      page: 0
      pdf_page: 57
    - "no": 5
      title: Anneaux réguliers et extensions plates
      page: 59
      pdf_page: 58
statements: 29
exercises: 13
content_sha256: 3a9b79f63014ef951b00ee573dd100216a0d16c92c7c07a16d7c538bfed42cbf
translated_from: content/fr/ac/X/04_s4_anneaux_reguliers.md
source_lang: fr
translation_method: machine
source_content_sha256: 1cb4ee83cd3848ac9878b8d74c05d2ee772f02b46e916425c5ae49647a84ed0f
translation_model: gpt-5.4
translation_run: translate-en-mt-0c057ba2
glossary_version: 34
glossary_terms_sha256: e8466bc4abad38235d18e98757580148b32296eb937f66cb0d1d2f6d3027202d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. REGULAR RINGS

### 1. Elementary Homological Properties of Regular Local Rings

#### Proposition 1 {#ac-x-s4-prop-1 .statement}

Let $A$ be a regular noetherian local ring and $n$ its dimension. Then $\mathrm{dh}(A) = n$ and, for every integer $i \geqslant 0$,

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \binom{n}{i}.
$$

Let $x = (x_1, \ldots, x_n)$ be a system of coordinates of $A$ (VIII, § 5, No. 1, def. 1). The sequence $x$ generates $m_A$ and is completely secant for $A$ (loc. cit., No. 2, th. 1). The Koszul complex $K_\bullet(x, A)$ is a free resolution of $\kappa_A$ (A, X, p. 159, remark 3), whose differential is zero modulo $m_A$. Hence, for every integer $i \geqslant 0$, one has (§ 3, No. 3, formula (1))

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \mathrm{rg}_A(K_i(x, A)) = \binom{n}{i}.
$$

It then follows from cor. 1 of prop. 4 of No. 3, § 3 that $\mathrm{dh}(A) = n$.

#### Proposition 2 {#ac-x-s4-prop-2 .statement}

A regular noetherian local ring is factorial.

By prop. 1, every finitely generated module over a regular noetherian local ring admits a projective resolution of finite length by finitely generated projective modules, hence free modules (II, § 3, No. 2, cor. 2 of prop. 5). It then follows from VII, § 4, No. 7, cor. 3 of prop. 16 that such a ring is factorial.

#### Proposition 3 {#ac-x-s4-prop-3 .statement}

Let $A$ be a regular noetherian local ring and $M$ a nonzero finitely generated $A$-module. Its projective dimension is finite, and one has

$$
\mathrm{dp}_A(M) + \mathrm{prof}_A(M) = \dim(A).
$$

In fact, $M$ has finite projective dimension (prop. 1), and one has $\mathrm{prof}(A) = \dim(A)$ since $A$ is a Macaulay ring (§ 2, No. 5, example 7). One then applies th. 1 of § 3, No. 5.

#### Corollary 1 {#ac-x-s4-prop-3-cor-1 .statement}

One has $\mathrm{dp}_A(M) \geqslant \dim(A) - \dim(M)$; for equality to hold, it is necessary and sufficient that $M$ be a Macaulay module.

#### Corollary 2 {#ac-x-s4-prop-3-cor-2 .statement}

For the $A$-module $M$ to be free, it is necessary and sufficient that it be a Macaulay module and of dimension $\dim(A)$, or again that it be of depth $\geqslant \dim(A)$.

#### Corollary 3 {#ac-x-s4-prop-3-cor-3 .statement}

Every finitely generated reflexive module over a regular noetherian local ring of dimension 2 is free.

In fact, a regular noetherian local ring is integrally closed (VIII, § 5, No. 2, cor. 1 of th. 1). Corollary 3 therefore follows from corollary 2 and § 1, No. 10, prop. 16.

#### Corollary 4 {#ac-x-s4-prop-3-cor-4 .statement}

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings. Suppose that $A$ is regular and that $\rho$ makes $B$ into a finitely generated $A$-module. Then $dp_A(B) \geq \dim(A) - \dim(B)$. For $B$ to be a Macaulay ring, it is necessary and sufficient that one have $dp_A(B) = \dim(A) - \dim(B)$. For $B$ to be a Macaulay ring of dimension equal to $\dim(A)$, it is necessary and sufficient that the $A$-module $B$ be free.

In fact, one has $\dim(B) = \dim_A(B)$ (VIII, § 2, No. 3, th. 1); moreover, $B$ is a Macaulay ring if and only if it is a Macaulay $A$-module (§ 2, No. 6, prop. 8). It is therefore enough to apply corollaries 1 and 2.

#### Remark {#ac-x-s4-n1-rem-1 .statement}

Corollary 4 makes it possible to characterize Macaulay local rings in several important cases. Let $A$ be a noetherian local ring; it is a Macaulay ring if and only if the same is true of $\hat{A}$ (§ 2, No. 7, cor. 4 of prop. 9). Henceforth suppose the local ring $A$ complete, and put $d = \dim(A)$.

a) Suppose that $A$ possesses a subfield. Then it possesses a coefficient subfield $K$ (IX, § 3, No. 3), and there exists a formal power series algebra $E = K[[T_1, \ldots, T_n]]$ and a surjective homomorphism of $K$-algebras $E \to A$ (*loc. cit.*); there also exists a formal power series algebra $E' = K[[T_1, \ldots, T_d]]$ and an injective local homomorphism of $K$-algebras $E' \to A$ such that $A$ is a finite algebra over $E'$ (*loc. cit.*). The following properties are equivalent :

(i) $A$ is a Macaulay ring;
(ii) $dp_E(A) = n - d$;
(iii) $A$ is a free $E'$-module.

b) Suppose that the residue field of $A$ is of characteristic $p > 0$. There exists a $p$-ring of length $+\infty$, with residue field $\kappa_A$ (IX, § 2, No. 3, prop. 5). Let $C$ be such a ring; there exists a formal power series algebra $E = C[[T_1, \ldots, T_n]]$ and a surjective homomorphism $\rho : E \to A$ (IX, § 2, No. 5, th. 3). The following properties are equivalent:

(i) $A$ is a Macaulay ring;
(ii) $dp_E(A) = n + 1 - d$.

Suppose moreover that $p1_A$ is not a zero divisor in $A$; then there exists a formal power series algebra $E' = K[[T_1, \ldots, T_{d-1}]]$ and an injective local homomorphism of $K$-algebras $E' \to A$ such that $A$ is a finite algebra over $E'$ (*loc. cit.*). The local ring $E'$ is regular, of dimension $n + 1$ (VIII, § 5, No. 5, example 2). The preceding conditions are also equivalent to

(iii) $A$ is a free $E'$-module.

For analogous results in the case of modules, see § 5, No. 5.

### 2. Homological Characterization of Regular Noetherian Rings

#### Theorem 1 (Serre) {#ac-x-s4-thm-1 .statement}

A noetherian local ring is regular if and only if its homological dimension is finite.

We have seen that a regular noetherian local ring is of finite homological dimension (prop. 1).

Conversely, let $A$ be a noetherian local ring of finite homological dimension $n$; by § 3, No. 3, Corollary 2 of Proposition 4 and No. 5, Theorem 1, one has
$$
n = \mathrm{dh}(A) = \mathrm{dp}_A(\kappa_A) = \mathrm{prof}(A) .
$$
If $n = 0$, the $A$-module $\kappa_A$ is free, hence $m_A = 0$ and $A$ is a field. Suppose $n > 0$ and argue by induction on $n$. Since $\mathrm{prof}(A) > 0$, the ideal $m_A$ is not associated to $A$ (§ 1, No. 1, Remark 2), hence is not contained in the union of $m_A^2$ and the ideals associated to $A$ (II, $§ 1$, No. 1, Proposition 2). Consequently (IV, $§ 1$, No. 1, Corollary 2 of Proposition 2), one can find an element $x$ of $m_A - m_A^2$ such that the homothety $x_A$ is injective. Let $B$ denote the noetherian local ring $A/xA$ and consider the sequence of $A$-modules
$$
0 \to \kappa_A \xrightarrow{i} m_A/xm_A \xrightarrow{p} m_B \to 0
$$
where the mapping $i$ is deduced by passing to quotients from the mapping $a \mapsto ax$ of $A$ into $m_A$, and where $p$ is the canonical surjection; it is exact. Since the class of $x$ in the $\kappa_A$-vector space $m_A/m_A^2$ is non-zero, there exists an $A$-linear mapping $\phi : m_A \to \kappa_A$ with $\phi(x) = 1$; by passing to the quotient, one deduces from $\phi$ a retraction of $i$, so that the preceding exact sequence is split. This implies the relations
$$
\mathrm{dp}_B(m_B) \leq \mathrm{dp}_B(m_A/xm_A) = \mathrm{dp}_A(m_A) < +\infty
$$
(Corollary 2 of Proposition 7 of § 3, No. 4 and $\Lambda$, X, p. 135, Corollary 1). Corollary 2 of loc. cit. applied to the exact sequence of $B$-modules $0 \to m_B \to B \to \kappa_B \to 0$ implies $\mathrm{dp}_B(\kappa_B) < +\infty$. The ring $B$ is therefore of finite homological dimension (§ 3, No. 3, Corollary 2 of Proposition 4), and of depth $n - 1$ (§ 1, No. 4, Proposition 7 and No. 3, Corollary of Proposition 4). It follows from the induction hypothesis that $B$ is regular, hence that $A$ is regular (VIII, $§ 5$, No. 3, Corollary 1 of Proposition 2).

Consequently, if $A$ is a noetherian local ring, there is an equivalence between the following three properties:
(i) $A$ is regular;
(ii) the $A$-module $\kappa_A$ is of finite projective dimension;
(iii) every finitely generated $A$-module is of projective dimension $< +\infty$.

#### Definition 1 {#ac-x-s4-def-1 .statement}

One says that a ring $A$ is regular if it is noetherian and if the local ring $A_m$ is regular for every maximal ideal $m$ of $A$.

#### Proposition 4 {#ac-x-s4-prop-4 .statement}

Let $A$ be a noetherian ring. The following conditions are equivalent:
(i) $A$ is regular;
(ii) every finitely generated $A$-module has projective dimension $< +\infty$;
(iii) for every maximal ideal $m$ of $A$, the projective dimension of $A/m$ is finite;
(iv) for every prime ideal $p$ of $A$, the local ring $A_p$ is regular.

Let us prove that (i) implies (ii). Let $M$ be a finitely generated $A$-module. Under hypothesis (i), one has $\mathrm{dp}_{A_m}(M_m) \leq \mathrm{dh}(A_m) < +\infty$ for every maximal ideal $m$ of $A$ (No. 1, prop. 1); therefore $M$ has projective dimension $< +\infty$ ($§ 3$, No. 2, cor. 2 of prop. 3), whence (ii).

#### Example 1 {#ac-x-s4-n2-exa-1 .statement}

If the ring $A$ is regular, the ring of fractions $S^{-1}A$ is regular for every multiplicative subset $S$ of $A$: this follows for example from characterization (iii) above.

#### Example 2 {#ac-x-s4-n2-exa-2 .statement}

In order that a ring be regular, it is necessary and sufficient that it be isomorphic to the product of a finite family of integral regular rings; this follows in fact from the fact that every regular ring is locally integral ($§ 1$, No. 8), since regular local rings are integral.

#### Example 3 {#ac-x-s4-n2-exa-3 .statement}

The integral regular rings of dimension $\leq 1$ are the Dedekind rings (VIII, $§ 5$, No. 1, example 1 and VII, $§ 2$, No. 2, theorem 1).

#### Corollary 1 {#ac-x-s4-prop-4-cor-1 .statement}

*Let $A$ be a noetherian ring. The following conditions are equivalent*:

(i) *one has* $\mathrm{dh}(A) < +\infty$ ;
(ii) *$A$ is regular and one has* $\dim(A) < +\infty$.

*If these conditions are satisfied, one has* $\dim(A) = \mathrm{dh}(A)$.

If the ring $A$ is regular, one has for every maximal ideal $m$ of $A$ the equality $\dim(A_m) = \mathrm{dh}(A_m)$ (No. 1, prop. 1), and therefore

$$
\mathrm{dh}(A) = \sup_m \mathrm{dh}(A_m) = \sup_m \dim(A_m) = \dim A
$$

($§ 3$, No. 2, prop. 3 and VIII, $§ 1$, No. 3, prop. 8). On the other hand, if $\mathrm{dh}(A) < +\infty$, the ring $A$ is regular by prop. 4. The corollary follows.

There exist regular noetherian rings of infinite dimension (VIII, $§ 5$, exerc. 6).

#### Corollary 2 {#ac-x-s4-prop-4-cor-2 .statement}

*A regular ring is normal, Gorenstein and Macaulay.*

In fact, a regular local ring is integrally closed (VIII, $§ 5$, No. 2, cor. 1 of th. 1), Gorenstein ($§ 3$, No. 9, example 4) and Macaulay ($§ 2$, No. 5, example 6).

#### Corollary 3 {#ac-x-s4-prop-4-cor-3 .statement}

*Let $A$ be a noetherian ring, $J$ an ideal of $A$ and $\hat{A}$ the separated completion of $A$ for the $J$-adic topology.*

a) *In order that the ring $\hat{A}$ be regular, it is necessary and sufficient that, for every maximal ideal $m$ of $A$ containing $J$, the ring $A_m$ be regular.*

b) *If the ring $A$ is regular, the ring $\hat{A}$ is regular. If the ring $\hat{A}$ is regular and the ideal $J$ contained in the radical of $A$, the ring $\Lambda$ is regular.*

#### Corollary 4 {#ac-x-s4-prop-4-cor-4 .statement}

*Let $A$ be a regular ring and $P$ a finitely generated projective $A$-module. The symmetric algebra $S_A(P)$ is a regular ring.*

Let $p$ be a prime ideal of $S_A(P)$ and $q$ its inverse image in $A$. The local ring $S_A(P)_p$ is a ring of fractions of the ring $S_A(P)_q$, which is isomorphic to $S_{A_q}(P_q)$ (A, III, p. 72, prop. 7); it is enough to prove that the latter is regular. This reduces us to the case where $A$ is local; but then $P$ is free of finite type. By prop. 1 of No. 1 and A, X, p. 143, cor. 1, one has $dh(S_A(P)) = dh(A) + rg_A(P) < +\infty$, and $S_A(P)$ is regular by prop. 4.

#### Corollary 5 {#ac-x-s4-prop-4-cor-5 .statement}

*Let $A$ be a regular ring, and $(T_i)_{i \in I}$ a finite family of indeterminates. The polynomial ring $A[(T_i)_{i \in I}]$ and the ring of formal series $A[[T_i]_{i \in I}]$ are regular.*

This follows from cor. 4 and cor. 3 b).

### 3. Regular Rings and Finite Algebras

#### Proposition 5 {#ac-x-s4-prop-5 .statement}

*Let $\rho : A \to B$ be a homomorphism of noetherian rings and $N$ a $B$-module. Suppose that
a) the ring $A$ is regular,
b) $N$ is a finitely generated $A$-module,
c) the $B$-module $N$ is Cohen-Macaulay,
d) every minimal prime ideal of $\mathrm{Supp}_B(N)$ lies over a minimal prime ideal of $A$.
Then $N$ is a projective $A$-module (of finite type).*

The point is to prove that, for every maximal ideal $m$ of $A$, the $A_m$-module $N_m$ is free (II, § 5, No. 2, th. 1). The $A$-module $B/\mathrm{Ann}_B(N)$ is a submodule of the finitely generated $A$-module $\mathrm{End}_A(N)$, and is therefore finitely generated. If one replaces $B$ by $B/\mathrm{Ann}_B(N)$, the hypotheses of the proposition are still satisfied ($§ 2$, No. 1, example 5); one may therefore suppose that $B$ is a finitely generated $A$-module and that $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$.

Let $m$ be a maximal ideal of $\mathrm{Supp}_A(N)$; put $n = \dim(A_m)$. By Cor. 2 of Prop. 3 of No. 1, it is enough to prove that $N_m$ is a Macaulay $A_m$-module of dimension $n$. Every maximal ideal of $B_m$ is of the form $nB_m$, where $n$ is a prime ideal of $B$ lying over $m$ (V, § 2, No. 1, Lemma 1 and Prop. 1). Let $p$ be a minimal prime ideal of $\mathrm{Supp}_B(N)$, contained in $n$. The closed subset $V(pB_n)$ of $\mathrm{Supp}_{B_n}(N_n)$ is then of codimension zero; since the $B_n$-module $N_n$ is Macaulay, the Cor. of Prop. 2, § 2, No. 2 yields the equality $\dim_{B_n}(N_n) = \dim(B_n/pB_n)$. But $p$ lies over a minimal prime ideal of $A$, contained in $m$, so that

#### Corollary {#ac-x-s4-n3-cor-1 .statement}

Let B be an integral noetherian ring and let A be a regular subring of B. Suppose that the A-module B is finitely generated. In order that the ring B be a Macaulay ring, it is necessary and sufficient that the A-module B be projective.

If the ring B is a Macaulay ring, the A-module B is projective by Prop. 5.

Suppose conversely that the A-module B is projective. The A-module A is Macaulay (Cor. 2 of Prop. 4); the A-module B is a direct factor of a free A-module of finite type, hence is Macaulay (§ 2, No. 1, Example 2). One then applies Cor. 1 of Prop. 8 of § 2, No. 6.

#### Example {#ac-x-s4-n3-exa-1 .statement}

Let B be a nonzero integral algebra of finite type over a field K. By VIII, § 2, No. 4, Cor. 1 of Th. 3, there exists a subalgebra A of B isomorphic to a polynomial algebra over K and such that B is a finitely generated A-module. The following properties are equivalent:

(i) the ring B is Macaulay;
(ii) the A-module B is projective;
*(iii) the A-module B is free.*

### 4. Presentable Rings

A ring A is said to be presentable if there exists a regular ring R and a surjective homomorphism of R onto A.

By definition, regular rings are presentable.

#### Proposition 6 {#ac-x-s4-prop-6 .statement}

a) Every ring of fractions of a presentable ring is presentable. Every algebra of finite type over a presentable ring is a presentable ring.

b) Let A be a presentable ring and J an ideal of A. The separated completion $\widehat{A}$ of A for the J-adic topology is presentable.

c) Every complete local noetherian ring is presentable.

d) Let A be a presentable local ring. There exists a regular local ring R and a surjective local homomorphism of R onto A.

Let A be a presentable ring; choose a regular ring R and a surjective homomorphism $\rho : R \to A$.

a) Let S be a multiplicative subset of A; put T = $\rho^{-1}(S)$. The homomorphism $T^{-1}R \to S^{-1}A$ deduced from $\rho$ is surjective and the ring $T^{-1}R$ is regular (No. 3, Example 1), hence $S^{-1}A$ is presentable.

Let B be an A-algebra of finite type; there exist a finite set I and a surjective homomorphism $A[(T_i)_{i \in I}] \to B$, hence a surjective homomorphism $R[(T_i)_{i \in I}] \to B$. Since the ring $R[(T_i)_{i \in I}]$ is regular (No. 2, Cor. 5 of Prop. 4), the ring B is presentable.

b) Put $I = \rho^{-1}(J)$ and denote by $\hat{R}$ the separated completion of R for the I-adic topology; for each integer $n \geq 0$, the canonical mapping $I^n/I^{n+1} \to J^n/J^{n+1}$ is surjective. Consequently, the homomorphism $\hat{R} \to \hat{A}$ deduced from $\rho$ is surjective (III, § 2, No. 8, Cor. 2 of Th. 1); since $\hat{R}$ is regular (No. 2, Cor. 3 of Prop. 4), the ring $\hat{A}$ is presentable.

c) This follows from IX, § 2, No. 5, Th. 3 a) and IX, § 3, No. 3, Th. 2 a).

d) Let $m_A$ be the maximal ideal of A; then $p = \rho^{-1}(m_A)$ is a prime ideal of R, the local ring $R_p$ is regular and the homomorphism $R_p \to A$ deduced from $\rho$ is local and surjective.

Since fields and Dedekind rings are regular, hence presentable, Proposition 6 implies that most rings ordinarily encountered in algebraic geometry are presentable.

#### Proposition 7 {#ac-x-s4-prop-7 .statement}

Let A be a presentable ring.

a) The ring $\Lambda$ is noetherian and catenary.

b) Let M be a finitely generated A-module. The mapping
$$
p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)
$$
of $\operatorname{Spec}(A)$ into $\mathbf{Z}$ is upper semicontinuous.

c) Let M be a finitely generated $\Lambda$-module. The set of $p \in \operatorname{Spec}(A)$ such that the $A_p$-module $M_p$ is Macaulay is a dense open set. Its intersection with $\operatorname{Supp}(M)$ is dense in $\operatorname{Supp}(M)$.

Choose a regular ring R and a surjective homomorphism $R \to A$.

a) The ring R is a Macaulay ring (No. 2, Cor. 2 of Prop. 4), hence A is catenary ($§ 2$, No. 2, Prop. 2 and VIII, § 1, No. 3, Rem. 2).

b) The R-module M is finitely generated and of projective dimension $< +\infty$ (No. 1, Prop. 1). Let us identify $\operatorname{Spec}(A)$ with a closed subset of $\operatorname{Spec}(R)$. Then the function $p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)$ on $\operatorname{Spec}(A)$ is the restriction of the function $q \mapsto \dim_{R_q}(M_q) - \operatorname{prof}_{R_q}(M_q)$ on $\operatorname{Spec}(R)$; it is then enough to apply Cor. 4 of Th. 1 of § 3, No. 5.

c) This is proved as in part c) of loc. cit.

### 5. Regular rings and flat extensions

#### Proposition 8 {#ac-x-s4-prop-8 .statement}

Let $\rho : A \to B$ be a homomorphism of noetherian rings making B a faithfully flat A-module.

a) For every finitely generated A-module M, one has $dp_A(M) = dp_B(B \otimes_A M)$.

b) If the ring B is regular, the ring A is regular.

$$
0 \to N \to L \to M \to 0
$$

where the $A$-module $L$ is free of finite type. One has $dp_A(N) = dp_A(M) - 1$ (A, X, p. 135, Cor. 2 of Prop. 1). Since $B$ is flat over $A$, the sequence

$$
0 \to B \otimes_A N \to B \otimes_A L \to B \otimes_A M \to 0
$$

is exact and one has $dp_B(B \otimes_A N) = dp_B(B \otimes_A M) - 1$. The induction hypothesis applied to $N$ enables one to conclude. This proves a); assertion b) follows from a) and Prop. 4 of No. 2.

#### Corollary {#ac-x-s4-n5-cor-1 .statement}

*Let $B$ be a regular integral ring and let $A$ be a noetherian subring of $B$ such that $B$ is a finitely generated $A$-module. The following conditions are equivalent:*

(i) $A$ is regular ;
(ii) $B$ is a projective $A$-module ;
(iii) $B$ is a flat $A$-module ;
(iv) $B$ is a faithfully flat $A$-module.

(i) $\Rightarrow$ (ii) : this follows from the Cor. of Prop. 5 of No. 3.
(ii) $\Rightarrow$ (iii) : this follows from I, § 3, No. 1, Prop. 1.
(iii) $\Rightarrow$ (iv) : for every prime ideal $\mathfrak{p}$ of $A$, one has $\mathfrak{p}B \neq B$ (V, § 2, No. 1, Cor. 1 of Theorem 1). It is then enough to apply I, § 3, No. 1, Prop. 1.
(iv) $\Rightarrow$ (i) : this follows from Prop. 8, b).

For every noetherian local ring $A$, let us denote by $\delta(A)$ the integer

$$
\delta(A) = [\mathfrak{m}_A / \mathfrak{m}_A^2 : \kappa_A] - \dim(A)
$$

Recall (VIII, § 5, No. 1) that $\delta(A)$ is always positive and that its vanishing characterises regular local rings.

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings; from $\rho$ one deduces a $\kappa_A$-linear homomorphism $\mathfrak{m}_A / \mathfrak{m}_A^2 \to \mathfrak{m}_B / \mathfrak{m}_B^2$, whence a $\kappa_B$-linear homomorphism

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A / \mathfrak{m}_A^2) \to \mathfrak{m}_B / \mathfrak{m}_B^2 .
$$

*Lemma 1.— One has*

$$
\delta(B) + [\mathrm{Ker}(d\rho) : \kappa_B] = \delta(A) + \delta(\kappa_A \otimes_A B) + (\dim(A) - \dim(B) + \dim(\kappa_A \otimes_A B)) .
$$

Let $C$ denote the local ring $\kappa_A \otimes_A B$. Consider the exact sequence of $B$-modules

$$
B \otimes_A \mathfrak{m}_A \to \mathfrak{m}_B \to \mathfrak{m}_C \to 0 ;
$$

by tensor product with $\kappa_B$, one obtains an exact sequence of $\kappa_{13}$-vector spaces

$$
\kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \xrightarrow{d\rho} \mathfrak{m}_B/\mathfrak{m}_B^2 \longrightarrow \mathfrak{m}_C/\mathfrak{m}_C^2 \to 0,
$$

whence one deduces the equality

$$
[\mathfrak{m}_B/\mathfrak{m}_B^2 : \kappa_B] + [\mathrm{Ker}(d\rho) : \kappa_B] = [\mathfrak{m}_A/\mathfrak{m}_A^2 : \kappa_A] + [\mathfrak{m}_C/\mathfrak{m}_C^2 : \kappa_C],
$$

which implies the lemma.

#### Proposition 9 {#ac-x-s4-prop-9 .statement}

*Let $\rho : A \to B$ be a local homomorphism of noetherian local rings. The following conditions are equivalent:

(i) the ring $B$ is regular and the $\kappa_B$-linear mapping

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \longrightarrow \mathfrak{m}_B/\mathfrak{m}_B^2
$$

is injective;
(ii) the rings $B$ and $\kappa_A \otimes_A B$ are regular and the $A$-module $B$ is flat;
(iii) the rings $A$ and $\kappa_A \otimes_A B$ are regular and the $A$-module $B$ is flat;
(iv) the rings $A$ and $\kappa_A \otimes_A B$ are regular, and one has

$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

One has $\dim(B) \leq \dim(A) + \dim(\kappa_A \otimes_A B)$ (VIII, § 3, No. 4, Corollary 1 of Proposition 7); the equivalence of (i) and (iv) therefore follows from Lemma 1. Under hypothesis (ii), the $A$-module $B$ is faithfully flat since one has $\mathfrak{m}_A B \subset \mathfrak{m}_B \neq B$ (I, § 3, No. 1, Proposition 1), which implies (iii) by Proposition 8. The implication (iii) $\Rightarrow$ (iv) follows from VIII, *loc. cit*.

It now remains for us to prove that when the equivalent conditions (i) and (iv) are satisfied, the $A$-module $B$ is flat. Let $x$ be a system of coordinates of $A$. Since $d\rho$ is injective, the image of this sequence under $\rho$ forms part of a system of coordinates of $B$. Thus the sequence $x$ is completely secant for $A$ and for $B$ (VIII, § 5, No. 3, Proposition 2), and generates the ideal $\mathfrak{m}_A$ of $A$. By Remark 3 of A, X, p. 159, the $A$-module $\mathrm{Tor}_1^A(\kappa_A, B)$ is isomorphic to $H_1(x, B)$, and therefore is zero; it follows that $B$ is flat over $A$ (III, § 5, No. 2, Theorem 1 and No. 4, Proposition 2).

#### Example {#ac-x-s4-n5-exa-1 .statement}

*Let $X$, $Y$ be two complex analytic varieties, locally of finite dimension, $f$ a morphism of $X$ into $Y$, and $x$ a point of $X$. Consider the local homomorphism $\rho : \mathcal{O}_{Y, f(x)} \to \mathcal{O}_{X, x}$ associated with $f$. The mapping $d\rho$ is the transpose of the tangent mapping $T_x(f) : T_x(X) \to T_{f(x)}(Y)$. The conditions (i) to (iv) of Proposition 9 are therefore equivalent in this case to the fact that $f$ is a submersion at $x$ (VAR, R, 5.9.1).*

#### Corollary {#ac-x-s4-n5-cor-2 .statement}

*Let $\rho : \Lambda \to B$ be a homomorphism of noetherian rings making $B$ a flat $A$-module. If $A$ is regular and if $\kappa(\rho^{-1}(\mathfrak{n})) \otimes_{\Lambda} B$ is regular for every maximal ideal $\mathfrak{n}$ of $B$, the ring $B$ is regular.

For in fact, for every maximal ideal $\mathfrak{n}$ of $B$, the $A_{\rho^{-1}(\mathfrak{n})}$-module $B_n$ is flat (II, § 3, No. 4, Proposition 15), so that the ring $B_n$ is regular by Proposition 9.

## EXERCISES {#ac-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
