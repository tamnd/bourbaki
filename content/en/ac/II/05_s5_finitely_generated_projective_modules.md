---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 5
section_title: Finitely generated projective modules. Invertible fractional ideals
lang: en
source: ac-i-vii
book_pages: 108-120, 146-153
pdf_pages: 0128-0140, 0166-0173
extraction: ocr
subsections:
    - "no": 1
      title: LOCALIZATION WITH RESPECT TO AN ELEMENT
      page: 108
      pdf_page: 128
    - "no": 2
      title: LOCAL CHARACTERIZATION OF FINITELY GENERATED PROJECTIVE MODULES
      page: 109
      pdf_page: 129
    - "no": 3
      title: RANKS OF PROJECTIVE MODULES
      page: 111
      pdf_page: 131
    - "no": 4
      title: PROJECTIVE MODULES OF RANK 1
      page: 114
      pdf_page: 134
    - "no": 5
      title: NON-DEGENERATE SUBMODULES
      page: 116
      pdf_page: 136
    - "no": 6
      title: INVERTIBLE SUBMODULES
      page: 117
      pdf_page: 137
    - "no": 7
      title: THE GROUP OF CLASSES OF INVERTIBLE MODULES
      page: 119
      pdf_page: 139
statements: 34
exercises: 8
content_sha256: b0d54943b748610ad0e7af93405f294a99c6edab5712a336877d7ebc3241e9b3
---

## 5. FINITELY GENERATED PROJECTIVE MODULES. INVERTIBLE FRACTIONAL IDEALS

### 1. LOCALIZATION WITH RESPECT TO AN ELEMENT

Let $A$ be a ring and $M$ an $A$-module. For every element $f \in A$, we shall write $A_f = A[f^{-1}], M_f = M[f^{-1}] = M \otimes_A A[f^{-1}]$ (\S 2, nos. 1 and 2); if $S_f$ is the set off" for $n \geq 0$, then $A_{S_f} = S_f^{-1}A, M_{S_f} = S_f^{-1}M$. Iff is invertible in $A$, $A_f$ (resp. $M_f$) is canonically identified with $A$ (resp. $M$); iff is nilpotent, then $A_f = 0$ and $M_f = 0$. For every $A$-module homomorphism $u : M \to N$, we write $u_f = u \otimes 1 : M_f \to N_f$.

Let $g$ be another element of $A$; $A_g$ (resp. $M_g$) is canonically identified with $(A,)_{g/1}$ (resp. $(M_f)_{g/1}$), where $g/1$ is the image of $g$ in $A_g$, and $u_{f,g}$ with $(u_f)_{g/1}$ (\S 2, no. 3, Proposition 7).

#### Proposition 1 {#ac-ii-s5-prop-1 .statement}

*Let $f$ be an element of a ring $A$ and $\phi : A \to A_f$, the canonical mapping. The mapping $^a\phi : \operatorname{Spec}(A_f) \to \operatorname{Spec}(A)$ is a homeomorphism of $\operatorname{Spec}(A_f)$ onto the open subspace $X_f$ of $X = \operatorname{Spec}(A)$ (\S 4, no. 3).*

This a particular case of \S 4, no. 3, Corollary to Proposition 13.

#### Proposition 2 {#ac-ii-s5-prop-2 .statement}

*Let $A$ be a ring, $u : M \to N$ an $A$-module homomorphism and $p$ a prime ideal of $A$.

(i) Suppose that $u_p : M_p \to N_p$ is surjective and that $N$ is finitely generated. Then there exists $f \in A - p$ such that $u_f : M \to N$, is surjective.

(ii) Suppose that $u_p$ is bijective, that $M$ is finitely generated and that $N$ is finitely presented. Then there exists $f \in A - p$ such that $u_f$ is bijective.*

Let $R$ and $Q$ be the kernel and cokernel of $u$; if $g \in A$, the kernel and cokernel of $u_g$ (resp. $u_p$) are $R_g$ and $Q_g$, (resp. $R_p$ and $Q_p$) (\S 2, no. 4, Theorem 1). Then $Q_p = 0$; as $N$ is finitely generated, so is $Q$ and there exists $g' \in A - p$ such that $g'Q = 0$ (\S 2, no. 2, Corollary 2 to Proposition 4), whence $Q_{g'} = 0$. Under the hypotheses of (ii), the sequence $0 \to R_{g'} \to M \to N \to 0$ is exact, hence $R_{g'}$ is finitely generated (Chapter I, \S 2, no. 8, Lemma 9). Now,

$$
(R_{g'})_{pR_{g'}} = R_p = 0;
$$

hence there exists $g_1 \in A, - pA_{g'}$ such that $g_1 R_{g'} = 0$ (\S 2, no. 2, Corollary 2 to Proposition 4). Then $g_1 = g''/g'^h$, where $g'' \in A - p$; as $g'/1$ is invertible in $R_{g'}$, $(g''/1)R_{g'} = 0$, whence $R_{g'g''} = (R_{g'})_{g''/1} = 0$. If $f = g'g''$, $f \in A - p$, $Q_f = 0$ and $R_f = 0$, so that $u_f$ is bijective.

#### Corollary {#ac-ii-s5-n1-cor-1 .statement}

*If $N$ is finitely presented and $N_p$ is a free $A_p$-module of rank $p$, there exists $f \in A - p$ such that $N$, is a free $A_f$-module of rank $p$.*

There exist by hypothesis $p$ elements $x_i \in \mathbf{N}$ ($1 \leq i \leq p$) such that the $x_i/1$ form a basis of the free $A_,-$-module $N_p$. Consider the homomorphism $u : A^p \to \mathbf{N}$ such that $u(e_i) = x_i$ for $1 \leq i \leq p$, $(e_i)_{1 \leq i \leq p}$ being the canonical basis of $A^p$. As $u_p$ is bijective by hypothesis, there exists $f \in A - p$ such that $u_f$ is bijective, by virtue of Proposition 2.

#### Proposition 3 {#ac-ii-s5-prop-3 .statement}

*Let* $(f_i)_{i \in I}$ *be a finite family of elements of a ring* $A$, *generating the ideal* $A$ *of* $A$. *The ring* $B = \prod_{i \in I} A_i$, *is then a faithfully flat* $A$*-module*.

By § 2, no. **4**, Theorem 1, each of the $A_i$ is a flat $A$-module, hence so is $B$ (Chapter I, § 2, no. 3, Proposition 2). On the other hand, if $p$ is a prime ideal of $A$, there exists an index $i$ such that $f_i \notin p$ and $p_{f_i} = pA_{f_i}$ is therefore a prime ideal of $A_{f_i}$. Then $pB \subset pA_{f_i} \times \prod_{j \neq i} A_j \neq B$ since $pA_{f_i} \neq A_{f_i}$; this suffices to imply that $B$ is a faithfully flat $A$-module (Chapter I, § 3, no. 1, Proposition 1).

#### Corollary {#ac-ii-s5-n1-cor-2 .statement}

*Under the hypotheses of Proposition 3, for an* $A$*-module* $M$ *to be finitely generated (resp. finitely presented), it is necessary and sufficient that, for every index* $i$, *the* $A_{f_i}$*-module* $M_{f_i}$ *be finitely generated (resp. finitely presented)*.

The condition is obviously necessary (§ 2, no. **4**). Conversely, if all the $M_{f_i}$ are finitely generated (resp. finitely presented), $M' = \prod_{i \in I} M_{f_i}$ is a finitely generated (resp. finitely presented) $B$-module, for we can obviously suppose that for each $i$ there is an exact sequence $AT_i \to A^n_{f_i} \to M_{f_i} \to 0$, where $m$ and $n$ are *independent of* $i$. Now, $M' = M \otimes_A B$. The corollary then follows from Proposition 3 and Chapter I, § 3, no. **6**, Proposition 11.

Note that the condition on the $f_i$ means that the open sets $X_{f_i}$ form a *covering* of $\mathrm{Spec}(A)$ (§ 4, no. 3, Corollary 3 to Proposition 11).

### 2. LOCAL CHARACTERIZATION OF FINITELY GENERATED PROJECTIVE MODULES

#### Theorem 1 {#ac-ii-s5-thm-1 .statement}

*Let* $A$ *be a ring and* $P$ *an* $A$*-module*. *The following properties are equivalent*:

(a) $P$ *is a finitely generated projective module*.
(b) $P$ *is a finitely presented module and, for every maximal ideal* $m$ *of* $A$, $P_m$ *is a free* $A_m$*-module*.
(c) $P$ *is a finitely generated module, for all* $p \in \mathrm{Spec}(A)$, *the* $A_p$*-module* $P_p$ *is free and, if we denote its rank by* $r_p$, *the function* $p \mapsto r_p$ *is locally constant in the topological space* $\mathrm{Spec}(A)$ *(that is, every point of* $\mathrm{Spec}(A)$ *admits a neighbourhood in which this function is constant)*.

(d) There exists a finite family $(f_i)_{i \in I}$ of elements of $A$, generating the ideal $A$, such that, for all $i \in I$, the $A,$-module $P_{f_i}$ is free with finite rank.

(e) For every maximal ideal $m$ of $A$, there exists $f \in A - m$ such that $P_f$ is a free $A,$-module of finite rank.

We show the theorem by proving the following scheme of implications

(a) ⇔ (d)

(b) ⇌ (e)

(c)

(a) ⇒ (b): We know that a finitely generated projective module is finitely presented (Chapter I, § 2, no. 8, Lemma 8 (iii)); if $P$ is a projective $A$-module, $P_m = P \otimes_A A_m$ is a projective $A_m$-module (\emph{Algebra}, Chapter II, § 5, no. 1, Corollary to Proposition 4); finally, as $A,$ is a local ring, every finitely presented projective $A,,$-module is free (\S 3, no. 2, Corollary to Proposition 5).

(b) ⇒ (e): This follows from the Corollary to Proposition 2 of no. 1.

(c) ⇒ (e): Let $m$ be a maximal ideal of $A$; write $r_m = n$ and let $(x_i)_{1 \leq i \leq n}$ be a basis of $P$. We can assume that the $x_i$ are canonical images of elements $p_i \in P$ $(1 \leq i \leq n)$ to within multiplication by an invertible element of $A,$. Let $(e_i)_{1 \leq i \leq n}$ be the canonical basis of $A^n$ and $u : A^n \to P$ the homomorphism such that $u(e_i) = p_i$ for $1 \leq i \leq n$. As $P$ is finitely generated, it follows from Proposition 2 of no. 1 that there exists $f \in A - m$ such that $u_f$ is surjective. We conclude that $u_{f,g}$ is also surjective for all $g \in A - m$ and by hypothesis there exists $g \in A - m$ such that $r_p = n$ for $p \in X,$. Then, replacing $f$ by $f g$, we may assume that $r_p = n$ for all $p \in X,$. Then $u_p : A_p^n \to P_p$ is a surjective homomorphism and $P_p$ and $A_p$ are both free $A,$-modules of the same rank; hence (\S 3, no. 2, Corollary to Proposition 6) $u_p$ is bijective for all $p \in X_f$. Let $p'$ be a prime ideal of $A,$ and let $p$ be its inverse image in $A$ under the canonical mapping; if $(A_f^{n})_{p'}$ and $(P_f)_{p'}$ are identified with $A_p^n$ and $P_p$ under the canonical isomorphisms, $(u_f)_{p'}$ is identified with $u_p$ and is consequently bijective. We conclude that $u_f$ is bijective (\$3, no. 3, Theorem 1), which establishes (e).

(e) ⇒ (d): Let $E$ be the set off $\in A$ such that $P_f$ is a finitely generated free $A_f$-module. The hypothesis implies that $E$ is contained in no maximal ideal of $A,$ hence $E$ generates the ideal $A$ and there therefore exist a finite family $(f_i)_{1 \leq i \leq n}$ of elements of $E$ and $a_i \in A$ $(1 \leq i \leq n)$ such that $1 = \sum_{i=1}^n a_i f_i$; whence (d).

(d) ⇒ (c): It follows from no. 1, Corollary to Proposition 3 that $P$ is finitely generated. On the other hand, for every prime ideal $p$ of $A$, there exists an index $i$ such that $p \in X_{f_i}$; if $p' = p_{f_i}$, then $P_p = (P_{f_i})_{p'}$ (\S 2, no. 5, Proposition

10) and hence by hypothesis $P_p$ is free and of the same rank as $P_{f_i}$, which proves (c).

(d) ⇒ (a): Consider the ring $B = \prod_{i \in I} A_i$ and the B-module
$$
M = \prod_{i \in I} P_i = P \otimes_A B.
$$
For every index $i$, there exists a free $A_i$-module $L$, such that $P_i$ is a direct factor of $L$, and it may be assumed that all the $L$, have the same rank; then $L = \prod_{i \in I} L_i$ is a free B-module of which M is a direct factor, in other words M is a finitely generated projective B-module. As B is a faithfully flat A-module (no. 1, Proposition 3), we conclude that P is a finitely generated projective A-module (Chapter I, §3, no. 6, Proposition 12).

#### Corollary 1 {#ac-ii-s5-thm-1-cor-1 .statement}

Suppose that the equivalent properties of the statement of Theorem 1 hold. Let m be an integer > 0 such that, for every family $(x_i)_{1 \leq i \leq m}$ of elements of P, there exists a family $(a_i)_{1 \leq i \leq m}$ of elements of A, which are not all divisors of zero and for which $\sum_{i=1}^m a_i x_i = 0$. Then, for all $p \in \operatorname{Spec}(A)$, $r_p \leq m$.

Let p be a prime ideal of A; set $r = r_p$ and let $(y_j)_{1 \leq j \leq r}$ be a basis of the free $A_p$-module $P_p$. There exist elements $x_j$ ($1 \leq j \leq r$) of P and $s \in A - p$ such that $y_j = x_j / s$ for all $j$. Then for every family $(a_j)_{1 \leq j \leq r}$ of elements of A such that $\sum_{j=1}^r a_j x_j = 0$, $\sum_{j=1}^r (a_j/1) y_j = 0$ in $P_p$, whence $a_j/1 = 0$ for $1 \leq j \leq r$. As $A - p$ does not contain 0, this shows that the $a_j$ are all divisors of zero in A (\S 2, no. 1, Remark 3), hence of necessity $r \leq m$.

#### Corollary 2 {#ac-ii-s5-thm-1-cor-2 .statement}

Every finitely presented flat module is projective.

If P is a finitely presented flat A-module and m a maximal ideal of A, the $A_m$-module P, is flat (\S 3, no. 4, Proposition 13) and finitely presented (\S 2, no. 4) and hence free (\$3, no. 2, Corollary 2 to Proposition 5), Condition (b) of Theorem 1 therefore holds.

Remarks
(1) There exist finitely generated flat modules which are not projective (Exercise 7).
(2) Corollary 2 to Theorem 1 extends to modules over non-commutative rings (Chapter I, §2, Exercise 15).

### 3. RANKS OF PROJECTIVE MODULES

#### Definition 1 {#ac-ii-s5-def-1 .statement}

Let P be a finitely generated projective A-module. For every prime ideal $p$ of A, the rank of the free $A_p$-module $P_p$ is called the rank of P at $p$ and is denoted by $\operatorname{rg}_p(P)$.

By Theorem 1 the integer-valued function $p \mapsto \mathrm{rg}_p(P)$ is *locally constant* on $X = \mathrm{Spec}(A)$; it is therefore constant if $X$ is *connected* and in particular if the ring $A$ is an *integral domain* (\S 4, no. 3, Corollary 2 to Proposition 15).

#### Definition 2 {#ac-ii-s5-def-2 .statement}

*Let $n$ be an integer $\geqslant 0$. A projective $A$-module $P$ is said to be *of rank* $n$ if it is finitely generated and $\mathrm{rg}_p(P) = n$ for every prime ideal $p$ of $A$.*

Clearly every finitely generated *free* $A$-module $L$ is of rank $n$ in the sense of Definition 2, $n$ being equal to the *dimension* (or *rank*) of $L$ defined in *Algebra*, Chapter II, \S 7, no. 2.

A projective module of rank 0 is zero (\S 3, no. 3, Corollary 2 to Theorem 1). If $A$ is not reduced to 0 and a projective $A$-module $P$ is of rank $n$, the integer $n$ is determined uniquely; it is then denoted by $\mathrm{rg}(P)$.

#### Theorem 2 {#ac-ii-s5-thm-2 .statement}

*Let $P$ be an $A$-module and $n$ an integer $\geqslant 0$. The following properties are equivalent:*

(a) *$P$ is projective of rank* $n$.

(b) *$P$ is finitely generated and, for every maximal ideal* $m$ *of* $A$, *the* $A$-*module* $P$, *is free of rank* $n$.

(c) *$P$ is finitely generated and, for every prime ideal* $p$ *of* $A$, *the* $A$-*module* $P_p$ *is free of rank* $n$.

(d) *For every maximal ideal* $m$ *of* $A$, *there exists* $f \in A - m$ *such that the* $A$-*module* $P_f$ *is free of rank* $n$.

By Definition 2 and Theorem 1, (a) and (c) are equivalent; (b) implies (c), as, for every prime ideal $p$ of $A$, there exists a maximal ideal $m$ containing $p$ and, writing $p' = p_m$, $P_p$ is isomorphic to $(P_m)_{p'}$ (\S 2, no. 5, Proposition 11); if $P_m$ is free of rank $n$, so then is $P_{p'}$. Property (c) implies (d) by virtue of Theorem 1 and the fact that, iff $\in A - m$ and $m' = m_f$, $P_m$ is isomorphic to $(P_f)_{m'}$ and therefore the ranks of $P_f$ and $P$ are equal. Finally, this last argument and Theorem 1 show that (d) implies (b).

#### Remark {#ac-ii-s5-n3-rem-1 .statement}

*If* $A$ *is an integral domain, a projective* $A$-*module admits a well-defined rank* (in the sense of Definition 2), *as has been observed above; moreover, this rank coincides with the rank defined in Algebra, Chapter II, \S 7, no. 2; it is sufficient to apply Theorem 2 (c) with* $p = (0)$.

Let $E$ and $F$ be two finitely generated projective $A$-modules. We know (*Algebra*, Chapter II, §§ 2 and 3) that $E \times F$, $E \otimes_A F$, $\mathrm{Hom}_A(E, F)$ and the dual $E^*$ of $E$ are projective and finitely generated; so is the exterior power $\bigwedge^k E$ for every integer $k > 0$ (*Algebra*, Chapter 111). Also, it follows immediately from Definition 1 and \S 2, no. 7, Propositions 18 and 19 and no. 8, that, for every prime ideal $p$ of $A$:

(1)
$$
\mathrm{rg}_p(E \times F) = \mathrm{rg}_p(E) + \mathrm{rg}_p(F)
$$

(2) $\mathrm{rg}_p(E \otimes_A F) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(3) $\mathrm{rg}_p(\mathrm{Hom}_A(E, F)) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(4) $\mathrm{rg}_p(E^*) = \mathrm{rg}_p(E)$

(5) $\mathrm{rg}_p(\wedge^k E) = \binom{\mathrm{rg}_p(E)}{k}$.

If the ranks of E and F are defined, so are those of $E \times F, E \otimes_A F,$ $\mathrm{Hom}_A(E, F), E^*$ and $\wedge^k E$ and the above equations also hold with the index $p$ omitted. Moreover:

#### Corollary {#ac-ii-s5-n3-cor-1 .statement}

*For a finitely generated projective A-module P to be of rank n, it is necessary and sufficient that $\mathbf{A}^n P$ be of rank 1.*

#### Proposition 4 {#ac-ii-s5-prop-4 .statement}

*Let B be a commutative A-algebra and P a projective A-module of rank n. The B-module $P_{(B)} = B \otimes_A P$ is then projective of rank n.*

We know that $P_{(B)}$ is projective and finitely generated (*Algebra*, Chapter II, § 5, no. 1, Corollary to Proposition 4). If q is a prime ideal of B and p its inverse image in A, then

$$
(P_{(B)})_q = (P \otimes_A B) \otimes_B B_q = P @_A B_q = (P \otimes_A A_i) \otimes_A B_q
$$

and, as, by hypothesis, $P \otimes_A A_i$ is a free A,-module of rank $n$, $(P_{(B)})_q$ is a free $B_q$-module of rank $n$.

#### Proposition 5 {#ac-ii-s5-prop-5 .statement}

*Let A be a semi-local ring and P a finitely generated projective A-module. If the rank of P is defined, P is a free A-module.*

Suppose first that A is isomorphic to a product of fields $K_i$ ($1 \leq i \leq n$). The $K_i$ are then identified with the minimal ideals (*Algebra*, Chapter VIII, § 3, no. 1) of A and, for all $i$, the sum $p_i$ of the K, of index $j \neq i$ is a maximal ideal of A, the $p_i$ ($1 \leq i \leq n$) being the only prime ideals of A. Every finitely generated A-module P is therefore the direct sum of its isotypical components $P_i$ ($1 \leq i \leq n$), $P_i$ being isomorphic to a direct sum of a finite number $r_i$ of A-modules isomorphic to K, (*Algebra*, Chapter VIII, § 5, no. 1, Proposition 1 and no. 3, Proposition 11); the ring $A_{r_i}$ is identified with K, and annihilates the $P_j$ of index $j \neq i$, hence $r_i = \mathrm{rg}_{p_i}(P)$; if all the $r_i$ are equal to the same number $r$, P is isomorphic to $A^r$, whence the proposition in this case. In the general case, let $\mathfrak{R}$ be the Jacobson radical of A and $B = A / \mathfrak{R}$; as B is a product of fields, the projective B-module $P_{(B)}$ is free by the remarks preceding Proposition 4. *Also P is a flat A-module and the proposition then follows from § 3, no. 2, Proposition 5.*

### 4. PROJECTIVE MODULES OF RANK 1

#### Theorem 3 {#ac-ii-s5-thm-3 .statement}

Let $A$ be a ring and $M$ ajnitely generated $A$-module.

(i) *If there exists an $A$-module $N$ such that $M \otimes_A N$ is isomorphic to $A$, the module $M$ is projective of rank 1.*

(ii) *Conversely, if $M$ is projective of rank 1 and $M^*$ is the dual of $M$, the canonical homomorphism $u : M \otimes_A M^* \to A$ corresponding to the canonical bilinear form $(x, x^*) \to \langle x, x^* \rangle$ on $M \times M^*$ (Algebra, Chapter II, § 2, no. 3) is bijective.*

(i) It is required to prove that, for every maximal ideal $m$ of $A$, the $A_m$-module $M$, is free of rank 1 (Theorem 2 (b)); we are free to replace $A$ by $A_m$ and hence may assume that $A$ is a *local* ring ($\S 2$, no. 7, Proposition 18). Let $k = A/m$. The isomorphism $v : M \otimes_A N \to A$ defines an isomorphism

$$
v \otimes 1_k : (M/mM) \otimes_k (N/mN) \to k
$$

as the rank over $k$ of $(M/mM) \otimes_k (N/mN)$ is the product of the ranks of $M/mM$ and $N/mN$, these latter are necessarily equal to 1, in other words $M/mM$ is monogenous. It follows that $M$ is monogenous ($\S 3$, no. 2, Corollary 2 to Proposition 4); on the other hand, the annihilator of $M$ also annihilates $M \otimes_A N$ and hence is zero, which proves that $M$ is isomorphic to $A$.

(ii) It is sufficient to prove that, for every maximal ideal $m$ of $A$, $u_m$ is an isomorphism ($\S 3$, no. 3, Theorem 1). As $M$ is finitely presented (Chapter I, $\S 2$, no. 8, Lemma 8), $(M^*)_m$ is canonically identified with the dual $(M_m)^*$ ($\S 2$, no. 7, Proposition 19) and, as $M_m$ is free of rank 1 like its dual $(M_m)^*$, clearly the canonical homomorphism $u_m : (M,) \otimes_{A_m} (M_m)^* \to A_m$ is bijective, which completes the proof.

*Remark* (1). If $M$ is projective of rank 1 and $N$ is such that $M \otimes_A N$ is isomorphic to $A$, then $N$ is isomorphic to $M^*$: there are isomorphisms

$$
N \to N \otimes A \to N \otimes M \otimes M^* + A \otimes M^* \to M^*.
$$

#### Proposition 6 {#ac-ii-s5-prop-6 .statement}

*Let $M$ and $N$ be projective $A$-modules of rank 1. Then $M \otimes_A N$, $\operatorname{Hom}_A(M, N)$ and the dual $M^*$ of $M$ are projective of rank 1.*

This follows immediately from formulae (2), (3) and (4).

Let us now note that every finitely generated $A$-module is isomorphic to a quotient module of $L = \mathbf{A}^{(\mathbf{N})}$; we may therefore speak of the *set $F(A)$ of classes of finitely generated $A$-modules* with respect to isomorphism (*Set Theory*, Chapter I, §6, no. 9); we denote by $P(A)$ the subset of $F(A)$ consisting of the classes of projective $A$-modules of rank 1 and by $\operatorname{cl}(M)$ the image in $P(A)$ of a projective $A$-module $M$ of rank 1. It is immediate that, for two projective $A$-modules $M$,

N of rank 1, cl(M \otimes_A N) depends only on cl(M) and cl(N); as definition we set

(6) $$ \mathrm{cl}(M) + \mathrm{cl}(N) = \mathrm{cl}(M \otimes AN) $$

and an internal law of composition is thus defined on $P(A)$.

#### Proposition 7 {#ac-ii-s5-prop-7 .statement}

*The set $P(A)$ of classes of projective A-modules of rank 1, with the law of composition (6), is a commutative group. If M is a projective A-module of rank 1 and $M^*$ is its dual, then*

(7) $$ \mathrm{cl}(M^*) = -\mathrm{cl}(M) \quad \text{and} \quad \mathrm{cl}(A) = 0. $$

The associativity and commutativity of the tensor product show that the law of composition (6) is associative and commutative; the isomorphism between $A \otimes_A M$ and M prove that $\mathrm{cl}(A)$ is the identity element under this law and, by virtue of Theorem 3, $\mathrm{cl}(M) + \mathrm{cl}(M^*) = \mathrm{cl}(A)$, whence the proposition.

Let B be a commutative A-algebra and M a projective A-module of rank 1; then $M_{(B)} = B \otimes_A M$ is a projective B-module of rank 1 (no. 3, Proposition 4). Then there exists a mapping called canonical $\phi : P(A) \to P(B)$ such that

(8) $$ \phi(\mathrm{cl}(M)) = \mathrm{cl}(M_{(B)}). $$

The equation $M_{(B)} \otimes_B N_{(B)} = (M \otimes_A N)_{(B)}$ for two A-modules M, N proves that the mapping $\phi$ is a commutative group *homomorphism*.

*Remark (2).* Condition (e) of Theorem 1 (equivalent to the fact that P is projective and finitely generated) may also be expressed by saying that *the sheaf of modules* $\tilde{P}$ over $X = \mathrm{Spec}(A)$ *associated(*) with P is locally free and of finite type* and may therefore be interpreted as the sheaf of sections of a vector bundle over X. Conversely, every vector bundle over X arises from a finitely generated projective module, which is determined to within a unique isomorphism; the projective modules of rank $n$ thus correspond to the vector bundles all of whose fibres have dimension $n$. In particular, the vector bundles of rank 1 correspond to the projective modules of rank 1. If we denote by $\mathcal{O}_X$ the structure sheaf $\tilde{A}$ and by $\mathcal{O}_X^*$ the *sheaf of units* of $\mathcal{O}_X$ (whose sections over an open set U of X are the invertible elements of the ring of sections of $\mathcal{O}_X$ over U), it follows that the group $P(A)$ is isomorphic to the first cohomology group $H^1(X, \mathcal{O}_X^*)$.*

(* See A. Grothendieck, Éléments de géométrie algébrique, I (\S 1) (Publ. Math. I.H.E.S., no. 4, 1960).

### 5. NON-DEGENERATE SUBMODULES

In this no. and the two following, $A$ denotes a ring, $S$ a multiplicative subset of $A$ consisting of elements which are not divisors of zero in $A$, and $B$ the ring $S^{-1}A$; $A$ is canonically identified with a subring of $B$ ($\S 2$, no. 1, Remark 3). The elements of $S$ are therefore invertible in $B$.

One of the most important special cases for applications is that where $A$ is an integral domain and $S$ is the set of elements $\neq 0$ of $A$; $B$ is then the field of fractions of $A$.

#### Definition 3 {#ac-ii-s5-def-3 .statement}

Let $M$ be a sub-A-module of $B$. $M$ is called non-degenerate if $B.M = B$.

If $B$ is a field, this condition simply means that $M$ is not reduced to 0.

#### Proposition 8 {#ac-ii-s5-prop-8 .statement}

Let $M$ be a sub-A-module of $B$. The following conditions are equivalent:
(a) $M$ is non-degenerate.
(b) $M$ meets $S$.
(c) If $j : M \to B$ is the canonical injection, the homomorphism $u = S^{-1}j : S^{-1}M \to B$ is bijective.

(a) implies (b), for if $B.M = B$, there exists $a \in A, s \in S$ and $x \in M$ such that $(a/s)x = 1$, hence $ax = s$ belongs to $S \cap M$. To see that (b) implies (c), note that $u$ is already injective ($\S 2$, no. 4, Theorem 1); moreover, if $x \in M \cap S$, the image under $u$ of $x/x \in S^{-1}M$ in $B$ is equal to 1 and $u$ is therefore surjective. Finally, (c) clearly implies (a).

#### Corollary {#ac-ii-s5-n5-cor-1 .statement}

If $M$ and $N$ are two non-degenerate sub-A-modules of $B$, the A-modules $M + N, M.N$ and $M \cap N$ are non-degenerate.

The assertion is trivial for $M + N$; on the other hand if $s \in S \cap M$ and $t \in S \cap N$, then $st \in S \cap (M.N)$ and $st \in S \cap (M \cap N)$.

Given two sub-A-modules $M$ and $N$ of $B$, let us denote by $N : M$ the sub-A-module of $B$ consisting of those $b \in B$ such that $bM \subset N$ (Chapter I, $\S 2$, no. 10, Remark). If every $b \in N : M$ is mapped to the homomorphism $h_b : x \mapsto bx$ of $M$ to $N$, a canonical homomorphism $b \mapsto h_b$ is obtained from $N : M$ to $\operatorname{Hom}_A(M, N)$.

#### Proposition 9 {#ac-ii-s5-prop-9 .statement}

Let $M, N$ be two sub-A-modules of $B$. If $M$ is non-degenerate, the canonical homomorphism from $N : M$ to $\operatorname{Hom}_A(M, N)$ is bijective.

Let $s \in S \cap M$. If $b \in N : M$ is such that $bx = 0$ for all $x \in M$, then $bs = 0$, whence $b = 0$ since $s$ is not a divisor of 0 in $B$. On the other hand, let f \in \mathrm{Hom}_A(M, N) \text{ and set } b = f(s)/s; \text{ for all } x \in M, \text{ there exists } t \in S \text{ such that } tx \in A. \text{ Then}
$$
f(x) = s^{-1}t^{-1}f(stx) = s^{-1}t^{-1}txf(s) = bx,
$$
whence $b \in N : M$ and $f = h_b$, which proves the proposition.

#### Remark {#ac-ii-s5-n5-rem-1 .statement}

In particular, $A : M$ is canonically identified with the dual $M^*$ of $M$, the canonical bilinear form on $M \times M^*$ being identified with the restriction to $M \times (A : M)$ of the multiplication $B \times B \to B$.

### 6. INVERTIBLE SUBMODULES

(We preserve the notation & no. 5.)

#### Definition 4 {#ac-ii-s5-def-4 .statement}

*A sub*-A-module $M$ of $B$ is called invertible if there exists a *sub*-A-module $N$ of $B$ such that $M.N = A$.

#### Example {#ac-ii-s5-n6-exa-1 .statement}

If $b$ is invertible element of $B$, the $A$-module $Ab$ is invertible, as is seen by taking $N = Ab^{-1}$.

#### Proposition 10 {#ac-ii-s5-prop-10 .statement}

*Let $M$ be an invertible sub*-A*-module & $B$. Then:
(i) There exists $s \in S$ such that $As \subset M \subset As^{-1}$ (and in particular $M$ is non-degenerate).
(ii) $A : M$ is the only *sub*-A*-module* $N$ of $B$ such that $M.N = A$.

If $M.N = A$, then $B.M = B.(B.M) \supset B.(M.N) = B.A = B$, hence $M$ is non-degenerate. Similarly $N$ is non-degenerate. If $t \in S \cap M$ and $u \in S \cap N$ (no. 5, Proposition 8 ), the element $s = tu$ belongs to $S \cap M \cap N$, whence $Ms \subset M.N = A$ and therefore $As \subset M \subset As^{-1}$.
On the other hand, obviously $N \subset A : M$, whence
$$
A = M.N \subset M.(A : M) \subset A
$$
and $M.(A : M) = A$; multiplying the two sides by $N$, we deduce $A : M = N$, which completes the proof.

#### Theorem 4 {#ac-ii-s5-thm-4 .statement}

*Let $M$ be a non-degenerate sub*-A*-module* of $B$. *The following properties are equivalent*:
(a) $M$ is invertible.
(b) $M$ is projective.
(c) $M$ is projective of rank 1.
(d) $M$ is a finitely generated $A$-module and, for every maximal ideal $m$ of $A$, the $A_m$-module $M_m$ is monogenous.

Let us show first the equivalence of properties (a), (b) and (c). If (a) holds and N is sub-A-module of B such that M . N = A, then there is a relation

$$
\sum_{i=1}^{p} m_i n_i = 1 \quad (m_i \in M, n_i \in N \text{ for all } i).
$$

For all $x \in M$, set $v_i(x) = n_i x$; the $v_i$ are linear forms on M and by (9) $x = \sum_{i=1}^{n} m_i v_i(x)$ for all $x \in M$; this proves (Algebra, Chapter 11, §2, no. 6, Proposition 12) that M is projective and generated by the $m_i$; hence M is a finitely generated projective module.

Let m be a maximal ideal of A; we show that the integer $r = \mathrm{rg}_m(M)$ is equal to 1. Let S' be the image of S in $\mathbf{A}_{m'}$; as the elements of S are not divisors of 0 in A, those of S' are not divisors of 0 in $\mathbf{A}_{m'}$ since $\mathbf{A}_{m'}$ is a flat A-module (\S 2, no. 4, Theorem 1 and Chapter I, §2, no. 4, Proposition 3); then $S'^{-1}A_m \neq 0$ and, as $M_m$ is a free $A_m$-module of rank $r$, $S'^{-1}M_m$ is a free $S'^{-1}A_m$-module of rank $r$. But if T' is the image of A $-m$ in $S^{-1}A$, $S'^{-1}A$, (resp. $S'^{-1}M_m$) is canonically identified with $T'^{-1}(S^{-1}A)$ (resp. $T'^{-1}(S^{-1}M)$) (\S 2, no. 3, Proposition 7). Now $S^{-1}M = B$ (Proposition 8 (c)) and hence $T'^{-1}(S^{-1}M)$ is a free A-module of rank 1 over $T'^{-1}(S^{-1}A)$, which proves that $r = 1$ and shows the implication (a) $\Rightarrow$ (c).

The implication (c) $\Rightarrow$ (b) is trivial. Let us show that (b) $\Rightarrow$ (a). There exists by hypothesis a family (not necessarily finite) $(f_\lambda)_{\lambda \in L}$ of linear forms on M and a family $(m_\lambda)_{\lambda \in L}$ of elements of M such that, for all $x \in M$, the family $(f_\lambda(x))$ has finite support and $x = \sum_{\lambda \in L} m_\lambda f_\lambda(x)$ (Algebra, Chapter II, §2, no. 6, Proposition 12). Since M is non-degenerate, $f_\lambda(x) = n_\lambda x$ for some $n_\lambda \in A$: M by virtue of Proposition 9 of no. 5. Taking x as an element of M $\cap S$ (no. 5, Proposition 8), it is seen that of necessity $n_\lambda = 0$ except for a finite number of indices and $\sum_{\lambda \in L} m_\lambda n_\lambda = 1$. This obviously implies M . (A: M) = A, whence (a).

By virtue of Definition 2 of no. 3, (c) implies (d). Let us show the converse. As M is non-degenerate, its annihilator is zero (Proposition 8 (b)), then so is the annihilator of $M_m$ (\S 2, no. 4, formula (9)). As M, is assumed to be a monogenous &-module, it is therefore free of rank 1 and it then follows from no. 3, Theorem 2 that M is projective of rank 1.

#### Corollary {#ac-ii-s5-n6-cor-1 .statement}

Every invertible sub-A-module of B is flat and finitely presented.
This follows from Theorem 4 (c).

#### Proposition 11 {#ac-ii-s5-prop-11 .statement}

Let M, N be two sub-A-modules of B. Suppose that M is invertible. Then:
(i) The canonical homomorphism $M \otimes_A N \to M . N$ is bijective.
(ii) $N : M = N . (A : M)$ and $N = (N : M) . M$.

Let $j$ be the canonical injection $N \to B$. Since $M$ is a flat $A$-module (Corollary to Theorem 4), $1 \otimes j : M \otimes_A N \to M \otimes_A B$ is injective. But, as $B = S^{-1}A$, the $B$-module $M \otimes_A B$ is equal to $S^{-1}M$ and hence is identified with $B$ since $M$ is non-degenerate (no. 5, Proposition 8). If this identification is made, the image of $1 \otimes j$ is $M . N$, whence (i).

Let us set $M' = A : M$. Then obviously $M'.N \subset N : M$ and $M.(N : M) \subset N$. On the other hand, since $M.M' = A$ (Proposition 10),

$$
N : M = M'.M.(N : M) \subset M'.N
$$

and $N = M.M'.N \subset M.(N : M)$, whence (ii).

#### Remark {#ac-ii-s5-n6-rem-1 .statement}

The proof of (i) in Proposition 11 uses only the fact that $M$ is flat and non-degenerate.

### 7. THE GROUP OF CLASSES OF INVERTIBLE MODULES

(We preserve the notation of nos. 5 and 6.)

Under multiplication, the sub-A-modules of B form a commutative monoid $\mathfrak{m}$, with A as identity element. Then the invertible modules are the invertible elements of $\mathfrak{m}$ and therefore form a commutative group $\mathfrak{z}$. We have seen (no. 6, Proposition 10) that the inverse of $M \in \mathfrak{z}$ is $A : M$.

Let $A^*$ (resp. $B^*$) be the multiplicative group of invertible elements of A (resp. B) and let $u$ denote the canonical injection $A + B$. For all $b \in B^*$, $\theta(b) = bA$ is an invertible sub-A-module. The mapping $\theta : B^* \to \mathfrak{g}$ is a homomorphism whose kernel is $u(A^*)$; its cokernel will be denoted by $\mathfrak{c}$ or $\mathfrak{c}(A)$. The group $\mathfrak{c}$ is called the group of classes of invertible sub-A-modules of B. The following exact sequence has been constructed

$$
\text{(10)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{\rho} \mathfrak{c} \longrightarrow (1)
$$

where (1) denotes the group consisting only of the identity element and $\rho$ is the canonical mapping $\mathfrak{g} \to \mathfrak{c} = \mathfrak{g}/\theta(B^*)$.

As every invertible sub-A-module M of B is projective of rank 1 (no. 6, Theorem 4), the element $cl(M) \in P(A)$ is defined (no. 4).

#### Proposition 12 {#ac-ii-s5-prop-12 .statement}

*The mapping* $cl : \mathfrak{g} \to P(A)$ *defines, by taking quotients, an isomorphism from* $\mathfrak{c} = \mathfrak{g}/\theta(B^*)$ *onto the kernel of the canonical homomorphism*

$$
\phi : P(A) \to P(B)
$$

(no. 4).

In other words, there is an exact sequence

$$
\text{(11)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{cl} P(A) \xrightarrow{\phi} P(B).
$$

It follows from Proposition 11 of no. 6 and the definition of addition in $P(A)$ that $cl(M.N) = cl(M) + cl(N)$ for $M, N$ in $\mathbf{3}$, which shows that $cl$ is a homomorphism. If $M \in \mathfrak{J}$ is isomorphic to $A$, there exists $b \in B$ such that $M = Ab$ and, as $M$ is invertible, there exists $b' \in B$ such that $b'b = 1$, in other words $b$ is invertible in $B$; the converse is immediate. Hence the kernel of $cl$ in $\mathfrak{J}$ is $\theta(B^*)$.

Let us now determine the image of $cl$. If $M \in \mathfrak{J}$, then $M \otimes_A B = S^{-1}M = B$ (no. 5, Proposition 8 (c)), whence $cl(M) \in \mathrm{Ker}(\phi)$. Conversely, let $P$ be a projective $A$-module of rank 1 such that $P_{(B)} = P \otimes_A B$ is $B$-isomorphic to $B$. As $P$ is a flat $A$-module, the injection $u : A \to B$ defines an injection $u \otimes 1 : P \to P_{(B)} = B$ and $P$ is thus identified with a sub-$A$-module of $B$; by virtue of Proposition 8 (c) of no. 5, $P$ is non-degenerate and Theorem 4 of no. 6 shows that $P$ is invertible. The kernel of $\phi$ is therefore equal to the image of $cl : \mathfrak{J} \to P(A)$.

#### Corollary 1 {#ac-ii-s5-prop-12-cor-1 .statement}

*For two invertible sub-A-modules of B to have the same image in $\mathfrak{C}$, it is necessary and sufficient that they be isomorphic.*

#### Corollary 2 {#ac-ii-s5-prop-12-cor-2 .statement}

*If the ring $B$ is semi-local, the group $\mathfrak{C}$ of classes of invertible sub-A-modules of B is canonically identified with the group $P(A)$ of classes of projective A-modules of rank 1.*

In this case $P(B) = 0$ (no. 3, Proposition 5).

#### Remark {#ac-ii-s5-n7-rem-1 .statement}

The hypothesis of Corollary 2 is fulfilled in the two following cases:

(1) $A$ is an integral domain and $S$ is the set of elements $\neq 0$ of $A$, $B$ then being the field of fractions of $A$. The invertible sub-A-modules of $B$ are also called in this case *invertible fractional ideals*; those which are monogenous free $A$-modules $Ab$ ($b \# 0$ in $B$) are just the *fractional principal ideals* defined in *Algebra*, Chapter VI, § 1, no. 5.

*(2)* The ring $A$ is Noetherian and $S$ is the set of elements of $A$ which are not divisors of 0 such that $B$ is the total ring of fractions of $A$. In this case $S = A - \bigcup p_i$, where the $p_i$ are the elements (finite in number) of $\mathrm{Ass}(A)$ (Chapter IV, § 1), hence $B$ is semi-local (§ 3, no. 5, Proposition 17).*

### Exercises {#ac-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
