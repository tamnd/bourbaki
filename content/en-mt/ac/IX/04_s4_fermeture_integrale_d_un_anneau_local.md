---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 4
section_title: Fermeture intégrale d'un anneau local complet
lang: en
source: ac-viii-ix-fr
book_pages: AC IX.78-AC IX.84
pdf_pages: 0142-0148, 0190-0196
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux japonais
      page: 30
      pdf_page: 142
    - "no": 2
      title: Théorème de Nagata
      page: 0
      pdf_page: 143
    - "no": 3
      title: Quelques lemmes
      page: 33
      pdf_page: 145
    - "no": 4
      title: Anneaux de Nagata
      page: 0
      pdf_page: 146
statements: 25
exercises: 32
content_sha256: c99f00ea92b0543993afc373c2da1ed8fe1a64884eee789c95c982869175bfae
translated_from: content/fr/ac/IX/04_s4_fermeture_integrale_d_un_anneau_local.md
source_lang: fr
translation_method: machine
source_content_sha256: cb927004891b75f7bec7495a3fa16bafa8f97a5ce54d872780a5fd5e2ad7a98d
translation_model: gpt-5.4
translation_run: translate-en-mt-8824c852
glossary_version: 34
glossary_terms_sha256: a09747d7c6c2bcf9074744cf7b96a01873343e77ad16b1185c239b4ccf757045
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. INTEGRAL CLOSURE OF A COMPLETE LOCAL RING

### 1. Japanese rings

#### Definition 1 {#ac-ix-s4-def-1 .statement}

Let $A$ be a noetherian integral ring. One says that $A$ is Japanese if the integral closure of $A$ in every finite extension of its field of fractions is a finite $A$-algebra.

#### Remark 1 {#ac-ix-s4-n1-rem-1 .statement}

It amounts to saying that $A$ satisfies the following condition: every integral $A$-algebra $B$ integral over $A$, contained in a finitely generated extension of the field of fractions $K$ of $A$, is a finite $A$-algebra. In fact, the field of fractions $L$ of $B$ is an algebraic extension of $K$, and therefore is of finite degree over $K$ (A, V, p. 112, cor. 1 of prop. 17). The $A$-algebra $B$ is contained in the integral closure of $A$ in $L$, and is therefore finite if the latter is finite.

#### Example {#ac-ix-s4-n1-exa-1 .statement}

Every finitely generated integral algebra over a field is a Japanese ring (V, § 3, No. 2, th. 2).

#### Proposition 1 {#ac-ix-s4-prop-1 .statement}

Let A be a noetherian integral ring, K its field of fractions. Suppose that for every finite radicial extension L of K, the integral closure of A in L is a finite A-algebra. Then the ring A is Japanese.

Let E be a finite extension of K. Let N be a finite quasi-Galois extension of K containing E (A, V, p. 54, cor. 1), and L the field of invariants of the group of K-automorphisms of N. Then (A, V, p. 73, prop. 13), L is a radicial extension of K and N is a separable extension of L. The integral closure B of A in L is therefore by hypothesis a finite A-algebra; the integral closure C of B in N is a finite B-algebra (V, § 1, No. 6, cor. 1 to prop. 18), hence a finite A-algebra. The integral closure of A in E is contained in C, and is therefore a finite A-algebra since A is noetherian.

#### Corollary {#ac-ix-s4-n1-cor-1 .statement}

Suppose the field K perfect (for example of characteristic 0). Then A is Japanese if and only if its integral closure is a finite A-algebra.

#### Proposition 2 {#ac-ix-s4-prop-2 .statement}

Let B be a noetherian integral ring and A a noetherian subring of B, such that B is a finite A-algebra. In order that A be Japanese, it is necessary and sufficient that B be Japanese.

Let K (resp. L) denote the field of fractions of A (resp. B). Suppose first that A is Japanese, and let M be a finite extension of L. Let C denote the integral closure of B in M. By V, § 1, No. 1, prop. 6, C is the integral closure of A in M, and therefore is a finite A-algebra since M is a finite extension of K and A is Japanese. A fortiori, C is a finite B-algebra. This proves that B is Japanese.

Conversely, suppose B Japanese and let N be a finite extension of K. Let D denote the integral closure of A in N. Let E be an extension of K compounded of L and N; since B is Japanese, the integral closure D’ of B in E is a finite B-algebra, therefore a finite A-algebra; the A-module D, which is a submodule of D’, is therefore finitely generated, whence it follows that A is Japanese.

### 2. Nagata's Theorem

#### Theorem 1 (Tate) {#ac-ix-s4-thm-1 .statement}

Let A be an integrally closed noetherian ring, a an element of A. It is assumed that the ideal $aA$ is prime, that the ring $A/aA$ is Japanese, and that A is complete for the $aA$-adic topology. Then the ring A is Japanese.

a) The field of fractions of A being denoted by K, the assertion being trivial when K is of characteristic 0 (No. 1, corollary of prop. 1), one may suppose K of characteristic $p > 0$. One may also suppose $a \neq 0$.

Let L be a finite radicial extension of K and q a power of p such that $L \subset K^{1/q}$. Put $x = a^{1/q}$ and $M = L(x)$. By prop. 1 of No. 1, it is enough to prove that the integral closure B of A in M is a finite A-algebra.

b) Let us first prove that the ideal $xB$ is the unique prime ideal of B over $aA$. In fact there exists at least one prime ideal of B over $aA$ (V, § 2, No. 1, th. 1). Let q be one of these ideals. We have $x^q = a \in q$, whence $xB \subset q$ since q is prime. Conversely, let y be an element of q; the element $y^q$ of K is integral over A, and therefore belongs to A since A is integrally closed. Since $q \cap A = aA$, there exists an element $\alpha$ of A such that $y^q = a\alpha = x^q\alpha$. Consequently the element $y/x$ of M is integral over A, and therefore belongs to B; thus one has $y \in xB$, whence $q = xB$, which proves our assertion.

c) It follows that the ring $B_{xB}$ is the integral closure in M of the ring $A_{aA}$ (V, § 1, No. 5, prop. 16 and § 2, No. 1, prop. 2). By VI, § 3, No. 6, prop. 9, $A_{aA}$ is a discrete valuation ring; one then deduces from the Krull-Akizuki theorem (VII, § 2, No. 5, prop. 5) that the field $\kappa(xB)$ is a finite extension of $\kappa(aA)$ and that $B_{xB}$ is noetherian.

d) The ring $B/xB$ is integral over the Japanese ring $A/aA$ and its field of fractions is a finite extension of the field of fractions of the latter. Consequently, $B/xB$ is a finitely generated $(A/aA)$-module. For every integer $i \geq 0$, the same is true of the module $x^iB/x^{i+1}B$; it follows that the $(A/aA)$-module $B/aB$ possesses a composition series of length q whose quotients are finitely generated $(A/aA)$-modules, and is therefore itself a finitely generated $(A/aA)$-module.

e) Let us endow the ring A with the $(aA)$-adic filtration and the ring B with the $(aB)$-adic filtration. Then A is complete by hypothesis; since $B_{xB}$ is an integral domain and noetherian, the $aB_{xB}$-adic filtration of $B_{xB}$ is separated (III, § 3, No. 2, corollary to prop. 5); consequently one has $\bigcap a^nB \subset \bigcap a^nB_{xB} = \{0\}$, and the $aB$-adic filtration of B is separated; the gr(A)-module gr(B) is generated by gr_0(B), hence is finitely generated by d). It then follows from III, § 2, No. 9, cor. 1 to prop. 12, that B is a finitely generated A-module, which completes the proof.

#### Corollary {#ac-ix-s4-n2-cor-1 .statement}

Let R be a noetherian integral domain and n an integer. If R is Japanese, the ring $R[[T_1, ..., T_n]]$ is Japanese.

Reasoning by induction, we may suppose that $n = 1$. Let S denote the integral closure of R; if R is Japanese, S is a finite algebra over R, hence a Japanese ring (No. 1, prop. 2). The ring S[[T]] is noetherian and integrally closed (V, § 1, No. 4, prop. 14); applying Theorem 1 to $A = S[[T]]$ and $a = T$, we deduce that S[[T]] is Japanese. Consequently R[[T]] is Japanese (No. 1, prop. 2).

#### Theorem 2 (Nagata) {#ac-ix-s4-thm-2 .statement}

Every complete local noetherian integral domain A is Japanese.

By Theorem 3 of § 2, No. 5 and Theorem 2 of § 3, No. 3, there exist an integer $n \geq 0$, a ring R which is a field or a discrete valuation ring with field of fractions of characteristic 0, and a subring B of A, isomorphic to R[[T₁, ..., Tₙ]] and such that A is a finite B-algebra. Then R is Japanese (No. 1, example and corollary to prop. 1), hence B is Japanese (corollary to Theorem 1), and A is Japanese (No. 1, prop. 2).

#### Corollary {#ac-ix-s4-n2-cor-2 .statement}

Let A be a semi-local noetherian ring whose completion is reduced. Then the integral closure A' of A in its total ring of fractions R is a finite A-algebra.

Suppose first that A is local and complete, and let p₁, ..., pₙ be the minimal (distinct) prime ideals of A; for i = 1, ..., n, let Kᵢ denote the field of fractions of A/pᵢ and Aᵢ' the integral closure of A/pᵢ. Since A is reduced, R is the product of the rings Kᵢ and A' the product of the rings Aᵢ' (V, § 1, No. 2, cor. 1 to prop. 9). Since the local rings A/pᵢ are integral domains and complete, they are Japanese (Theorem 2), so that each Aᵢ' is a finite A-algebra, and A' is a finite A-algebra.

If A is semi-local and complete, it is isomorphic to a finite product of complete local rings (III, § 2, No. 13, corollary to prop. 19), and we conclude at once from the preceding.

Let us pass to the general case, and note that the completion Â of A is a semi-local, complete, noetherian ring faithfully flat over A (III, loc. cit., § 3, No. 4, corollary to prop. 8 and § 3, No. 5, prop. 9). Let S be the set of non-zero-divisors of A; one has R = S⁻¹A. Since Â is flat over A, the elements of S are non-zero-divisors in Â, and S⁻¹Â is identified with a subring of the total ring of fractions T of Â. Again because Â is flat over A, the ring A' ⊗_A Â is identified with a subring of R ⊗_A Â = S⁻¹Â, hence also with a subring of T integral over Â. By the first part of the proof, A' ⊗_A Â is therefore a finitely generated Â-module; hence A' is a finitely generated A-module (I, § 3, No. 6, prop. 11).

Recall (A, V, p. 114, def. 1) that an algebra E over a field K is said to be separable if the ring L ⊗_K E is reduced for every extension L of K; it is enough that this be so for every finite extension of K. The following proposition generalizes Theorem 2:

#### Proposition 3 {#ac-ix-s4-prop-3 .statement}

Let A be a semi-local noetherian integral domain, K its field of fractions. If the K-algebra K ⊗_A Â is separable, the ring A is Japanese.

Let L be a finite extension of K and B the integral closure of A in L. Let F be a finite subset of B such that L = K[F] (V, § 1, No. 5, cor. 2 to prop. 16); let C denote the (finite) A-algebra generated by F. Since L is the field of fractions of C, the ring B is the integral closure of C (V, § 1, No. 1, prop. 6) and it is enough to prove that B is a finite C-algebra. Now, C is a semi-local noetherian ring (IV, § 2, No. 5, cor. 3 to prop. 9 ); its completion is identified with C ⊗_A Â (III, § 3, No. 4, th. 3 (ii)), hence also with a subring of the reduced ring L ⊗_A Â = L ⊗_K (K ⊗_A Â) and therefore is reduced. Proposition 3 therefore follows from the corollary to Theorem 2.

### 3. Some lemmas

#### Lemma 1 {#ac-ix-s4-lem-1 .statement}

Let A be a semi-local noetherian ring and B a finite A-algebra. Then the ring B is semi-local and noetherian; let m₁, ..., mₙ be its maximal ideals.

The canonical homomorphism of B into $\prod_{i=1}^n \hat{B}_{m_i}$ extends to an isomorphism of $\hat{A} \otimes_A B$ onto $\prod_{i=1}^n \hat{B}_{m_i}$.

By IV, § 2, No. 5, cor. 3 to prop. 9, the ring B is semi-local and $m_A B$ is an ideal of definition of it. By III, § 3, No. 4, th. 3, (ii), the ring $\hat{A} \otimes_A B$ is the completion of B for the topology defined by its radical; one then applies III, § 2, No. 13, corollary to prop. 19.

#### Lemma 2 {#ac-ix-s4-lem-2 .statement}

Let A be a noetherian ring and M an A-module. The canonical mapping of M into the product $\prod_{p \in \mathrm{Ass}(M)} M_p$ is injective.

Let indeed m be a nonzero element of M; then Ann(m) is contained in a prime ideal p of A associated with M (IV, § 1, No. 1, prop. 2), and the image of m in $M_p$ is nonzero (II, § 2, No. 2, prop. 4).

#### Lemma 3 {#ac-ix-s4-lem-3 .statement}

Let $A$ be a noetherian ring, $x$ an element of $A$, $M$ a finitely generated $A$-module, and $p$ a prime ideal of $A$ associated with $M$. Suppose that the homothety $x_M$ is injective. Let $q$ be a prime ideal of $A$, minimal among those containing $p + xA$. Then $q$ is associated with the $A$-module $M/xM$.

Let $N$ denote the submodule of $M$ formed by the elements $m$ such that $pm = 0$. We have $N \cap xM = xN$; in fact, if an element $m$ of $M$ is such that $pxm = 0$, then $pm = 0$ since $x_M$ is injective, hence $m \in N$. Consequently, the $A$-module $N/xN$ is isomorphic to the submodule $(N + xM)/xM$ of $M/xM$, and it is enough to prove that $q$ is associated with $N/xN$. Since $p$ is associated with $M$, there exists an element $m$ of $M$ such that $p = \mathrm{Ann}(m)$; we have $m \in N$, whence $p = \mathrm{Ann}(N)$ and therefore $\mathrm{Supp}(N/xN) = V(p + xA)$ by II, § 4, No. 4, corollary to prop. 18; consequently, $q$ is associated with $N/xN$ (IV, § 1, No. 4, th. 2).

#### Lemma 4 {#ac-ix-s4-lem-4 .statement}

Let $A$ be a discrete valuation ring, $B$ a noetherian local ring, and $\rho : A \to B$ a local and flat homomorphism. If the ring $\kappa_A \otimes_A B$ is reduced, then $B$ is reduced.

Suppose there exists a nonzero nilpotent element $x$ of $B$, and let $\pi$ be a uniformizer of $A$. Since one has $\pi B \subset m_B$, the ring $B$ is separated for the $\pi B$-adic topology. There therefore exist $n \in \mathbf{N}$ and $y \in B$ with $x = \pi^n y$ and $y \notin \pi B$. Since $B$ is flat over $A$, multiplication by $\pi$ is injective in $B$. The class of $y$ in $B/\pi B$ is therefore a nonzero nilpotent element, which contradicts the assumption.

### 4. Nagata Rings

#### Definition 2 {#ac-ix-s4-def-2 .statement}

A ring $A$ is said to be a Nagata ring if it is noetherian and if, for every prime ideal $p$ of $A$, the noetherian integral ring $A/p$ is Japanese (No. 1, def. 1).

#### Example 1 {#ac-ix-s4-n4-exa-1 .statement}

Every finitely generated algebra over a field is a Nagata ring (No. 1, example).

#### Example 2 {#ac-ix-s4-n4-exa-2 .statement}

Every complete noetherian local ring is a Nagata ring (No. 2, th. 2).

#### Example 3 {#ac-ix-s4-n4-exa-3 .statement}

The ring $\mathbf{Z}$ is a Nagata ring (No. 1, example and corollary to prop. 1).

#### Example 4 {#ac-ix-s4-n4-exa-4 .statement}

One can prove (exercise 30) that every finitely generated algebra over a Nagata ring is a Nagata ring.

#### Proposition 4 {#ac-ix-s4-prop-4 .statement}

Let $A$ be a Nagata ring.
a) Every finite $A$-algebra is a Nagata ring.
b) For every multiplicative subset $S$ of $A$, the ring $S^{-1}A$ is a Nagata ring.
a) Let $B$ be a finite $A$-algebra, $\rho : A \to B$ the canonical homomorphism. For every prime ideal $p$ of $B$, the ring $B/p$, which is a finite algebra over the Japanese ring $A/\rho^{-1}(p)$, is Japanese (No. 1, prop. 2).
b) Let $q$ be a prime ideal of $S^{-1}A$; then there exists a prime ideal $p$ of $A$ such that $q = S^{-1}p$. The ring $(S^{-1}A)/q$ is a ring of fractions of the Japanese ring $A/p$, and is therefore Japanese (No. 1, remark 2).

#### Theorem 3 (Zariski-Nagata) {#ac-ix-s4-thm-3 .statement}

Let $A$ be a semi-local noetherian ring. The following conditions are equivalent:
(i) $A$ is a Nagata ring;
(ii) for every prime ideal $p$ of $A$, the $\kappa(p)$-algebra $\kappa(p) \otimes_A \hat{A}$ is separable;
(iii) for every reduced $A$-algebra $R$, the ring $R \otimes_A \hat{A}$ is reduced.
Let us first prove the equivalence of conditions (ii) and (iii). The implication (iii) $\Rightarrow$ (ii) is trivial; conversely, suppose that $A$ satisfies condition (ii). Then, for every $A$-algebra $K$ which is a field, the ring $K \otimes_A \hat{A}$ is reduced. Let now $C$ be a reduced $A$-algebra of finite type; the ring $C$, being noetherian, is isomorphic to a subring of a finite product $K_1 \times \cdots \times K_n$ of fields (IV, § 2, No. 5, Prop. 10); since $\hat{A}$ is flat over $A$, the ring $C \otimes_A \hat{A}$ is isomorphic to a subring of the reduced ring $\prod_i (K_i \otimes_A \hat{A})$, hence is reduced. Finally, let $R$ be any reduced $A$-algebra; then $R$ is the union of the filtered family $(C_\alpha)$ of its subalgebras of finite type, and $R \otimes_A \hat{A}$ is the direct limit of the filtered family $(C_\alpha \otimes_A \hat{A})$ of reduced rings, hence is reduced.
Let us show that (ii) implies (i). Let $p$ be a prime ideal of $A$; the field of fractions $K$ of the ring $A/p$ is identified with $\kappa(p)$, and the $K$-algebra $K \otimes_{A/p} (\widehat{A/p})$ is identified with $\kappa(p) \otimes_{A/p} \hat{A}/p\hat{A}$, hence with $\kappa(p) \otimes_A \hat{A}$. If $\kappa(p) \otimes_A \hat{A}$ is a separable $\kappa(p)$-algebra, the ring $A/p$ is Japanese (No. 2, Prop. 3).
Let us prove the implication (i) $\Rightarrow$ (ii) by induction on $\dim(A)$. It is obvious if $\dim(A) = 0$ since then $A$ is artinian, hence complete. Let $n$ be an integer $> 0$; consider the following assumption:

(R$_n$) $\left\{ \begin{array}{l}
\text{for every local noetherian Nagata ring } C \text{ of dimension } < n \text{ and every prime ideal } r \text{ of } C, \text{ the ring } \kappa(r) \otimes_C \hat{C} \text{ is reduced.}
\end{array} \right.$

Let $A$ be a semi-local noetherian Nagata ring of dimension $n$, let $p$ be a prime ideal of $A$ and $L$ a finite extension of the field $\kappa(p)$; it is enough to prove,

#### Corollary 1 {#ac-ix-s4-thm-3-cor-1 .statement}

*The completion of a local reduced Nagata ring is reduced.*
It is enough, in fact, to put R = A in Th. 3, (iii).

#### Corollary 2 (Chevalley) {#ac-ix-s4-thm-3-cor-2 .statement}

*Let A be a reduced algebra of finite type over a field, and p a prime ideal of A. The completion of the local ring $A_p$ is reduced.*
Since A is reduced, the local ring $A_p$ is reduced; moreover A is a Nagata ring (example 1), hence $A_p$ is a Nagata ring (Prop. 4), and Cor. 2 follows from Cor. 1, applied to the ring $A_p$.

#### Corollary 3 {#ac-ix-s4-thm-3-cor-3 .statement}

*Let $k$ be a field of characteristic 0, and $A$ a local noetherian $k$-algebra. In order that $A$ be a Nagata ring, it is necessary and sufficient that, for every prime ideal $p$ of $A$, the ring $(\widehat{A/p})$ be reduced.*
In fact, since the fields $\kappa(p)$ are of characteristic 0, it is equivalent to say that the algebras $\kappa(p) \otimes_A \hat{A} = \kappa(p) \otimes_{A/p} (\widehat{A/p})$ are reduced or that they are separable (A, V, p. 117, Theorem 1), which shows that the stated condition is sufficient (Theorem 3, (ii) ⇒ (i)); moreover it is necessary (Theorem 3, (i) ⇒ (iii) with R = A/p).

## EXERCISES {#ac-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
