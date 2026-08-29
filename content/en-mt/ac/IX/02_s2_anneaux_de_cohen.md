---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 2
section_title: Anneaux de Cohen
lang: en
source: ac-viii-ix-fr
book_pages: AC IX.17-AC IX.27, AC IX.68-AC IX.75
pdf_pages: 0129-0139, 0180-0187
extraction: ocr
subsections:
    - "no": 1
      title: $p$-anneaux
      page: 17
      pdf_page: 129
    - "no": 2
      title: Anneaux de Cohen
      page: 20
      pdf_page: 132
    - "no": 3
      title: Existence et unicité des $p$-anneaux
      page: 22
      pdf_page: 134
    - "no": 4
      title: Représentants multiplicatifs
      page: 24
      pdf_page: 136
    - "no": 5
      title: Structure des anneaux locaux noethériens complets
      page: 0
      pdf_page: 138
statements: 30
exercises: 17
content_sha256: d23599edc2c0840270fb99102a3340399d8d1e5d81cbfe51a36bfda141c52698
translated_from: content/fr/ac/IX/02_s2_anneaux_de_cohen.md
source_lang: fr
translation_method: machine
source_content_sha256: 55a245e21b3153aae0c2254426dfc0000c89fee4a5e3f77c1215285ee543c76f
translation_model: gpt-5.4
translation_run: translate-en-mt-eb8fbb4e
glossary_version: 34
glossary_terms_sha256: 6f89be7d280f7cee296a3030ccb8aca6f38dc60c6bbb6646432e83cfca7cfcd4
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. COHEN RINGS

Throughout this paragraph, $p$ denotes a prime number.

### 1. $p$-rings

#### Definition 1 {#ac-ix-s2-def-1 .statement}

A ring $C$ is said to be a $p$-ring if the ideal $pC$ of $C$ is maximal, and if $C$ is separated and complete for the $pC$-adic topology.

Let $C$ be a ring; if $p1_C$ is nilpotent and if the ideal $pC$ of $C$ is maximal, $C$ is a $p$-ring, for the $pC$-adic topology of $C$ is discrete. In particular, every field of characteristic $p$ is a $p$-ring.

#### Proposition 1 {#ac-ix-s2-prop-1 .statement}

Let $C$ be a $p$-ring.

a) The ring $C$ is local, with maximal ideal $pC$.

b) Suppose $p1_C$ nilpotent. Let $d$ be the smallest positive integer such that $p^d1_C = 0$. The ideals of $C$ are of the form $p^kC$ with $0 \leq k \leq d$, and one has $p^kC \neq p^lC$ when $k$ and $l$ are two distinct integers satisfying $0 \leq k \leq d, 0 \leq l \leq d$. The $C$-module $C$ is of length $d$.

c) Suppose that $p1_C$ is not nilpotent. Then $C$ is a discrete valuation ring whose residue field is of characteristic $p$, and whose field of fractions is of characteristic $0$. The ideals of the form $p^nC$, with $n \in \mathbf{N}$, are pairwise distinct; they form all the non-zero ideals of $C$. The $C$-module $C$ is not of finite length.

Assertion a) follows from prop. 19 of III, $§ 2$, no. 13.

By hypothesis, one has $\bigcap_{n \geqslant 0} p^n C = \{0\}$. Let $x \neq 0$ in $C$; there exists an integer $n \geqslant 0$ such that $x \in p^n C$, $x \notin p^{n+1} C$; therefore there exists an element $y$ of $C$ such that $x = p^n y$; since $y$ does not belong to $pC$, $y$ is invertible.

Suppose that $p 1_C$ is not nilpotent. If $x$ and $x'$ are two non-zero elements of $C$, there exist two integers $n \geqslant 0$, $n' \geqslant 0$ and two invertible elements $y$, $y'$ of $C$ such that $x = p^n y$, $x' = p^{n'} y'$. We then have $xx' = p^{n+n'} yy' \neq 0$, hence $C$ is an integral domain. Since $C$ is a local ring, but is not a field, and since the maximal ideal $m_C = pC$ of $C$ is principal, $C$ is a discrete valuation ring (VI, $§ 3$, no 6, prop. 9). The non-zero ideals of $C$ are then of the form $p^n C$ by *loc. cit.*, prop. 8, and are pairwise distinct. In particular, the ring $C$ is not artinian, hence the $C$-module $C$ is not of finite length. The residue field $C/pC$ of $C$ is of characteristic $p$. Let $q$ be the characteristic of the field of fractions of $C$. We have $p 1_C \neq 0$, whence $p \neq q$. Moreover, if $q$ were non-zero, we should have $q 1_C = 0$ hence $C/pC$ would be of characteristic $q \neq p$, which is absurd. This proves c).

Suppose that $p 1_C$ is nilpotent. Let $d$ be the smallest positive integer such that $p^d 1_C = 0$. We have a sequence of ideals

(E)
$$
C \supset pC \supset p^2 C \supset ... \supset p^{d-1} C \supset p^d C = \{0\} .
$$

If $k$ is an integer such that $0 \leqslant k < d$ and $p^k C = p^{k+1} C$, we deduce

$$
p^{d-k-1} p^k C = p^{d-k-1} p^{k+1} C = \{0\}
$$

contrary to the hypothesis $p^{d-1} 1_C \neq 0$. Therefore the elements of the sequence (E) are pairwise distinct. Let $a$ be an ideal of $C$ and let $k$ be the smallest positive integer such that $a \supset p^k C$. Let $x$ be a nonzero element of $a$; we have seen that $x$ is of the form $p^m u$ with $m \geqslant 0$ and $u$ invertible in $C$. Hence $p^m C \subset a$, whence $m \geqslant k$, and finally $x \in p^k C$. In conclusion, one has $a = p^k C$. The sequence (E) is then a Jordan-Hölder sequence of the $C$-module $C$, which is of length $d$.

#### Corollary 1 {#ac-ix-s2-prop-1-cor-1 .statement}

If the $p$-ring $C$ is an integral domain, it is a discrete valuation ring, or a field of characteristic $p$.

Suppose $C$ is an integral domain. If $p 1_C$ is nilpotent, one has $p 1_C = 0$, and $\{0\}$ is a maximal ideal of $C$, hence $C$ is a field of characteristic $p$. If $p 1_C$ is not nilpotent, then $C$ is a discrete valuation ring by Prop. 1, c).

#### Corollary 2 {#ac-ix-s2-prop-1-cor-2 .statement}

Let $C$ be a $p$-ring and $a$ an ideal of $C$ distinct from $C$. The ring $C/a$ is a $p$-ring.

One may suppose $a \neq \{0\}$. There then exists an integer $i \geqslant 1$ such that $a = p^i C$; the ideal $pC/a$ of $C/a$ is maximal and one has $p^i 1_{C/a} = 0$, therefore $C/a$ is a $p$-ring.

Let $C$ be a $p$-ring. The *length of* $C$, denoted by $l(C)$, is the least upper bound in $\overline{\mathbf{R}}$ of the set of integers $n \geqslant 1$ such that $p^{n-1} 1_C \neq 0$. When $l(C)$ is finite, it is the length of the $C$-module $C$, and when $l(C)$ is equal to $+ \infty$, the $C$-module $C$ is not of finite length (prop. 1).

#### Example 1 {#ac-ix-s2-n1-exa-1 .statement}

For every integer $n \geqslant 1$, the ring $\mathbf{Z}/p^n\mathbf{Z}$ is a $p$-ring of length $n$. The ring $\mathbf{Z}_p$ of $p$-adic integers is a $p$-ring of infinite length.

#### Example 2 {#ac-ix-s2-n1-exa-2 .statement}

Let $K$ be a perfect field of characteristic $p$. By prop. 8 of § 1, No. 8, the ring $W(K)$ of Witt vectors is a $p$-ring of infinite length. The mapping $(a_n)_{n \in \mathbf{N}} \mapsto a_0$ induces, by passing to quotients, an isomorphism of $W(K)/pW(K)$ onto the field $K$ (loc. cit., prop. 7). For every integer $n \geqslant 1$, the ring
$$
W_n(K) = W(K)/p^nW(K)
$$
is a $p$-ring of length $n$.

#### Proposition 2 {#ac-ix-s2-prop-2 .statement}

Let $C$ and $C'$ be two $p$-rings and $u$ a homomorphism of $C$ into $C'$. Let $v$ be the homomorphism of $\kappa_C = C/pC$ into $\kappa_{C'} = C'/pC'$ deduced from $u$ by passing to quotients.

a) One has $l(C) \geqslant l(C')$, and $u$ is injective if and only if one has $l(C) = l(C')$.

b) In order that $u$ be surjective, it is necessary and sufficient that $v$ be an isomorphism.

c) In order that $u$ be an isomorphism, it is necessary and sufficient that $v$ be an isomorphism and that one have $l(C) = l(C')$.

Let $n \geqslant 1$ be an integer. We have $u(p^{n-1}1_C) = p^{n-1}1_{C'}$, hence the relation $p^{n-1}1_{C'} \neq 0$ implies $p^{n-1}1_C \neq 0$ and is equivalent to it if $u$ is injective. Therefore $l(C') \leqslant l(C)$, with equality if $u$ is injective. If $u$ is not injective, there exists an integer $i < l(C)$ such that the kernel of $u$ is the ideal $p^iC$ of $C$; then $p^i1_{C'} = 0$, whence $l(C') \leqslant i$. This proves a).

Since $\kappa_C$ and $\kappa_{C'}$ are fields, the homomorphism $v$ is injective. If $u$ is surjective, the same is true of $v$, which is therefore an isomorphism. Conversely, suppose $v$ surjective. Then for every integer $n \geqslant 0$, the mapping $v_n : p^nC/p^{n+1}C \to p^nC'/p^{n+1}C'$ induced by $u$ is surjective. Since $C$ is complete for the $pC$-adic filtration and $C'$ separated for the $pC'$-adic filtration, $u$ is surjective by Cor. 2 of Th. 1 of III, § 2, No. 8. This proves b).

Finally, c) follows from a) and b).

#### Proposition 3 {#ac-ix-s2-prop-3 .statement}

Let $(C_n, \pi_{n,m})$ be a projective system of rings relative to the set of indices $\mathbf{N}$. Suppose that $C_n$ is a $p$-ring for every $n \in \mathbf{N}$ and that the homomorphisms $\pi_{n,m}$ are surjective. Then $C = \varprojlim C_n$ is a $p$-ring, and for every $n \in \mathbf{N}$, the canonical homomorphism $\pi_n : C \to C_n$ is surjective and induces an isomorphism of $\kappa_C$ onto $\kappa_{C_n}$.

Since the mappings $\pi_{n,m}$ are surjective, the same is true of the mappings $\pi_n$ (E, III, p. 58, prop. 5). Let us show that $C$ is a $p$-ring. Let $d_n$ be the length of $C_n$. By prop. 2, a), the sequence of the elements $d_n$ of $\mathbf{N} \cup \{ + \infty \}$ is increasing; if it is stationary, there exists an integer $n_0$ such that $\pi_{n,m}$ is an isomorphism of $C_m$ onto $C_n$ whenever $n_0 \leqslant n \leqslant m$, so that $C$, isomorphic to $C_{n_0}$, is a $p$-ring.

It is therefore enough to consider the case where each $d_n$ is finite, and where the sequence $(d_n)$ tends to $+ \infty$. Endow the ring $C$ with the trivial filtration (III, § 2, No. 1, example 5). For $n \in \mathbf{N}$, let $I_n$ be the kernel of $\pi_n$; put $I_n = C$ if $n < 0$. Let $E$ denote the $C$-module $C$ endowed with the filtration $(I_n)_{n \in \mathbf{Z}}$. It is separated and complete, for the topology $\mathcal{T}$ defined by the filtration $(I_n)_{n \in \mathbf{Z}}$ is the projective limit topology of the discrete topologies on the $C_n$.

Let k be an integer $\geqslant 1$. We have $p^k C \subset \varprojlim (p^k C_n)$ (E, III, p. 55, formula (9)). Conversely, if $x = (x_n)_{n \in \mathbf{N}} \in \varprojlim (p^k C_n)$ and if one puts $X_n = \{ y \in C | \pi_n(p^k y) = x_n \}$, the sequence $(X_n)_{n \in \mathbf{N}}$ is a decreasing sequence of nonempty closed affine parts of E. Since $E/I_n$ is an artinian C-module, the intersection of the $X_n$ is nonempty (III, § 2, No. 7, prop. 7); for every $z \in \bigcap_{n \in \mathbf{N}} X_n$, one has $p^k z = x$. We have therefore proved that one has $p^k C = \varprojlim p^k C_n$ for every integer $k \geqslant 1$. In particular the ideal $p^k C$ of C is closed for the topology $\mathcal{T}$. On C, the $p$-adic topology is finer than the topology $\mathcal{T}$ since one has $p^{d_n} C \subset I_n$. It then follows from TG, III, p. 26, cor. 1 to prop. 10, that C is separated and complete for the $pC$-adic topology. Moreover one has $pC = \varprojlim pC_n = \pi_0^{-1}(pC_0)$ and therefore the surjective homomorphism from $C/pC$ into $C_0/pC_0$ deduced from $\pi_0$ is an isomorphism. This shows that the ideal $pC$ of C is maximal and consequently that C is a $p$-ring. The last assertion of prop. 3 follows from prop. 2, b).

### 2. Cohen Rings

#### Definition 2 {#ac-ix-s2-def-2 .statement}

Let A be a separated and complete local ring, whose residue field is of characteristic p. A Cohen subring of A means a subring C of A which is a $p$-ring such that $A = m_A + C$ (i.e. $A/m_A = C/(m_A \cap C)$).

If C is a Cohen subring of A, the ideal $m_A \cap C$ of C is maximal, hence equal to $pC$. The canonical mapping of $\kappa_C = C/pC$ onto $\kappa_A = A/m_A$ is therefore a field isomorphism.

#### Example {#ac-ix-s2-n2-exa-1 .statement}

Let C be a $p$-ring. The ring of formal series $A = C[[T_1, ..., T_n]]$ is a noetherian, local, separated and complete ring, whose maximal ideal is generated by the sequence $(p, T_1, ..., T_n)$. It is immediate that C is a Cohen subring of A. This applies in particular when C is equal to $\mathbf{Z}_p$, to $\mathbf{Z}/p^n \mathbf{Z}$ or to a field of characteristic $p$.

#### Theorem 1 {#ac-ix-s2-thm-1 .statement}

Let A be a local, separated and complete ring, whose residue field k is of characteristic p. Let $\pi$ be the canonical mapping of A onto k, and let S be a subset of A, such that $\pi$ induces a bijection of S onto a $p$-basis of k (A, V, p. 95).
a) There exists one and only one Cohen subring C of A containing S.
b) The subring C of A is closed, and the $pC$-adic topology of C is induced by the $m_A$-adic topology of A.
c) Every closed subring $A'$ of A, containing S, and such that $A = A' + m_A$, contains C.

A) Particular case: $m_A$ nilpotent

Let n be a positive integer such that $m_A^{n+1} = \{0\}$. If $\Phi_n$ is the nth Witt polynomial ($§ 1$, No. 1), the mapping $u : [a_0, ..., a_n] \mapsto \Phi_n(a_0, ..., a_n)$ is a ring homomorphism of $W_{n+1}(A)$ into A ($§ 1$, No. 7). Let $B_n$ be the image of $u$ and let $C_n$ be the subring of A generated by $B_n \cup S$.

#### Lemma 1 {#ac-ix-s2-lem-1 .statement}

Let $A'$ be a subring of $A$ containing $S$. In order that $A'$ contain $C_n$, it is necessary and sufficient that one have $A' + m_A = A$.

One has $pA \subset m_A$ and $B_n$ consists of the elements of the form $a_0^{p^n} + pa_1^{p^{n-1}} + \cdots + p^n a_n$ with $a_0, ..., a_n$ in $A$. Hence one has $\pi(B_n) = k^{p^n}$, whence $\pi(C_n) = k^{p^n}[\pi(S)]$. But since $\pi(S)$ is a $p$-basis of $k$, one has $k = k^{p^n}[\pi(S)]$ (A, V, p. 96), whence $\pi(C_n) = k$, that is to say $C_n + m_A = A$.

Let $A'$ be a subring of $A$ containing $S$. If $A'$ contains $C_n$, we have
$$
A' + m_A \supset C_n + m_A = A, \quad \text{whence} \quad A' + m_A = A.
$$
Conversely, suppose that one has $A' + m_A = A$. Let $a_0, ..., a_n$ be elements of $A$; by assumption there exist elements $a'_0, ..., a'_n$ of $A'$ such that $a_i \equiv a'_i \mod m_A$ for $0 \leq i \leq n$. By prop. 1 of § 1, No. 1 and the assumption $m_A^{n+1} = \{0\}$, we therefore have $\Phi_n(a_0, ..., a_n) = \Phi_n(a'_0, ..., a'_n) \in A'$, whence $B_n \subset A'$. Since $C_n$ is the ring generated by $B_n \cup S$, one has $C_n \subset A'$.

In the set $S$ of subrings $A'$ of $A$ containing $S$ and such that $A' + m_A = A$, there exists by lemma 1 a smallest element $C$, and one has $C_n = C$ for every integer $n \geq 0$ such that $m_A^{n+1} = \{0\}$.

One has $C + m_A = A$ by construction and $p1_C$ is nilpotent. One obviously has $pC \subset C \cap m_A$ and lemma 2 below therefore shows that $pC$ is a maximal ideal of $C$ and consequently that $C$ is a Cohen subring of $A$.

#### Lemma 2 {#ac-ix-s2-lem-2 .statement}

One has $C \cap m_A \subset pC$.

Choose an integer $m \geq 1$ such that $m_A^m = \{0\}$, whence $C = C_m = C_{m-1}$. Let $\Lambda$ be the subset of $\mathbf{N}^{(S)}$ formed by the families of integers $(\alpha_s)_{s \in S}$ with finite support satisfying $0 \leq \alpha_s < p^m$ for every $s \in S$. Since $B_m$ contains $s^{p^m} = \Phi_m(s, 0, ..., 0)$ for every $s \in S$, the monomials $Z_\alpha = \prod_{s \in S} s^{\alpha_s}$, where $\alpha$ runs through $\Lambda$, generate $C_m$ as a $B_m$-module.

Moreover, from the formula
$$
\Phi_m(a_0, ..., a_m) = a_0^{p^m} + p \Phi_{m-1}(a_1, ..., a_m),
$$
every element of $B_m$ is of the form $a^{p^m} + pb$ with $a \in A$ and $b \in B_{m-1}$. Consequently every element of $C = C_m$ is of the form
$$
x = \sum_{\alpha \in \Lambda} c_\alpha^{p^m} Z_\alpha + py
$$
with $c_\alpha \in A$ for every $\alpha \in \Lambda$, and $y \in C_{m-1} = C$. If $x$ belongs to $C \cap m_A$, one has $\pi(x) = 0$, whence $\sum_{\alpha \in \Lambda} \pi(c_\alpha)^{p^m} \pi(Z_\alpha) = 0$. Since $\pi(S)$ is a $p$-base of $k$, one has $\pi(c_\alpha) = 0$ for every $\alpha \in \Lambda$ from A, V, p. 96. One then has $c_\alpha \in m_A$, whence $c_\alpha^m = 0$ and a fortiori $c_\alpha^{p^m} = 0$. From (1), one has $x = py$, whence lemma 2.

One has $p^m C = m_A^m = \{0\}$ for $m$ sufficiently large, and assertion b) is therefore trivial. Assertion c) results from lemma 1. If $C'$ is a Cohen subring of $A$ containing $S$, one has $C' \supset C$ from lemma 1. But since the inclusion of $C$ in $C'$ induces an isomorphism of $\kappa_C$ onto $\kappa_{C'}$, one has $C = C'$ (No. 1, prop. 2, b)), and this completes the proving of a).

B) *General case*

For every integer $n \geqslant 0$, let $A_n$ denote the local ring $A/m_A^{n+1}$, let $m_n = m_A/m_A^{n+1}$ denote its maximal ideal, and let $\pi_n$ denote the canonical homomorphism of $A$ onto $A_n$. By A), there exists a unique Cohen subring $C_n$ of $A_n$ containing $\pi_n(S)$. When $0 \leqslant n \leqslant m$, we denote by $\pi_{n,m}$ the canonical homomorphism of $A_m$ onto $A_n$. By Corollary 2 of Proposition 1 of No. 1, $\pi_{n,m}(C_m)$ is a $p$-ring; one has $\pi_{n,m}(C_m) + m_n = A_n$, hence $\pi_{n,m}(C_m)$ is equal to the Cohen subring $C_n$ of $A_n$. By Proposition 3 of No. 1, the subring $\lim C_n$ of $\lim A_n$ is a $p$-ring. Put $C = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(C_n)$. Since $C$ is the inverse image of $\lim C_n$ under the isomorphism $a \mapsto (\pi_n(a))_{n \in \mathbf{N}}$ of $A$ onto $\lim A_n$, it is a closed subring of $A$, and a $p$-ring. One has $\pi_n(C) = C_n$ for every $n \in \mathbf{N}$ (No. 1, Proposition 3), and in particular $\pi_0(C) = A_0$, that is to say $\pi(C) = k$. Therefore $C$ is a Cohen subring of $A$.

For every integer $n \geqslant 0$, put $J_n = C \cap m_A^n$. Since the local ring $A$ is separated, one has $\bigcap_{n \in \mathbf{N}} J_n = \{0\}$, and in view of the structure of the ideals of a $p$-ring (No. 1, Proposition 1), every ideal of $C$ of the form $p^kC$ contains one of the $J_n$. Conversely, $J_n$ contains $p^nC$. Consequently, the $pC$-adic topology of $C$ is induced by the $m_A$-adic topology of $A$. This proves b).

Let $A'$ be a closed subring of $A$, containing $S$ and such that $A' + m_A = A$. Since $A'$ is closed, one has $A' = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(\pi_n(A'))$. One has $\pi_n(A') \supset \pi_n(S)$ and $\pi_n(A') + m_n = A_n$, whence $\pi_n(A') \supset C_n$ by what was seen in A). Finally, one has $\pi_n^{-1}(\pi_n(A')) \supset \pi_n^{-1}(C_n)$, whence $A' \supset C$. This proves c). One deduces the uniqueness of a Cohen subring as in A).

#### Remark {#ac-ix-s2-n2-rem-1 .statement}

Suppose that $p1_A$ is not nilpotent (this takes place in particular when $A$ is an integral ring whose field of fractions is of characteristic 0). Then $C$ is a discrete valuation ring whose field of fractions is of characteristic 0.

### 3. Existence and uniqueness of $p$-rings

#### Proposition 4 {#ac-ix-s2-prop-4 .statement}

*Let $C$ and $C'$ be two $p$-rings such that $l(C) \geqslant l(C')$, and let $\pi$ (resp. $\pi'$) be the canonical homomorphism of $C$ (resp. $C'$) onto $\kappa_C$ (resp. $\kappa_{C'}$). Let $(x_\lambda)_{\lambda \in \Lambda}$ (resp. $(x'_\lambda)_{\lambda \in \Lambda}$) be a family of elements of $C$ (resp. $C'$) whose image under $\pi$ (resp. $\pi'$) is a $p$-basis of $\kappa_C$ (resp. $\kappa_{C'}$). Let $v$ be an isomorphism of $\kappa_C$ onto $\kappa_{C'}$ such that $v(\pi(x_\lambda)) = \pi'(x'_\lambda)$ for every $\lambda \in \Lambda$. Then there exists a unique homomorphism $u$ of $C$ into $C'$, such that $v \circ \pi = \pi' \circ u$ and $u(x_\lambda) = x'_\lambda$ for every $\lambda \in \Lambda$. It is surjective. If $l(C) = l(C')$, it is an isomorphism.*

Let us prove the existence of $u$. Let $A$ be the subring of $C \times C'$ formed by the pairs $(x, x')$ such that $v(\pi(x)) = \pi'(x')$. The mapping $(x, x') \mapsto \pi(x)$ is a surjective homomorphism of rings from A onto $\kappa_C$. Its kernel $m$, equal to $pC \times pC'$, is therefore a maximal ideal of A. The topological subspace A of $C \times C'$ is closed in $C \times C'$, hence complete, and the topology induced on A by that of $C \times C'$ is the $m$-adic topology. Hence A is a separated complete local ring with maximal ideal $m$ (III, § 2, No. 13, Prop. 19). For every $\lambda \in \Lambda$, we have $(x_\lambda, x'_\lambda) \in A$ by hypothesis; if $\xi_\lambda$ is the class of $(x_\lambda, x'_\lambda)$ modulo $m$, the family $(\xi_\lambda)_{\lambda \in \Lambda}$ is a $p$-basis of the field $A/m$. By theorem 1 of No. 2, there exists a Cohen subring $C''$ of A, and only one, containing $(x_\lambda, x'_\lambda)$ for every $\lambda \in \Lambda$. We have $l(C'') = l(C) \geq l(C')$. The restriction to $C''$ of the projection of $C \times C'$ onto C is a homomorphism $h : C'' \to C$ which induces an isomorphism of $\kappa_{C''}$ onto $\kappa_C$. By Prop. 2, c) of No. 2, $h$ is an isomorphism of $C''$ onto C. One sees analogously that the restriction $h'$ to $C''$ of the projection of $C \times C'$ onto $C'$ is a surjective homomorphism of $C''$ onto $C'$. Hence, $C''$ is the graph of a surjective homomorphism $u = h' \circ h^{-1}$ of C onto $C'$, and one obviously has $v \circ \pi = \pi' \circ u$, $u(x_\lambda) = x'_\lambda$ for every $\lambda \in \Lambda$. Moreover, if $l(C) = l(C')$, $u$ is an isomorphism.

Let us prove the uniqueness of $u$. Let $u_1$ be a homomorphism of C into $C'$ such that $v \circ \pi = \pi' \circ u_1$ and $u_1(x_\lambda) = x'_\lambda$ for every $\lambda \in \Lambda$, and let $C_1$ be the graph of $u_1$. It is immediate that $C_1$ is a Cohen subring of A, containing $(x_\lambda, x'_\lambda)$ for every $\lambda \in \Lambda$, whence $C_1 = C''$ (theorem 1 of No. 2) and finally $u_1 = u$.

#### Proposition 5 {#ac-ix-s2-prop-5 .statement}

Let k be a field of characteristic p, and let n be an integer $\geq 1$, or $+ \infty$. There exists a p-ring of length n whose residue field is isomorphic to k.

The ring $W(k)$ of Witt vectors with coefficients in k is an integral separated complete local ring whose residue field is isomorphic to k ($§ 1$, no. 8, prop. 8), and one has $p \cdot 1_{W(k)} \neq 0$ (loc. cit., formula (52)). Let C be a Cohen subring of $W(k)$ (no. 2, th. 1). Then C is a p-ring of length $+ \infty$ whose residue field is isomorphic to k, and, if n is an integer $\geq 1$, the quotient $C/p^nC$ is a p-ring of length n whose residue field is isomorphic to k.

#### Remark 1 {#ac-ix-s2-n3-rem-1 .statement}

Let n be an integer $\geq 1$ and S a p-basis of k. One can prove that the subring of $W_n(k)$ generated by $W_n(k^{p^n})$ and by the elements $[\xi, 0, ..., 0]$ ($\xi \in S$), is a p-ring of length n whose residue field is isomorphic to k (cf. p. 72, exerc. 10).

#### Remark 2 {#ac-ix-s2-n3-rem-2 .statement}

The reader will find in the Appendix a proof of prop. 5 which uses neither the results of $§ 1$, nor the existence theorem for Cohen subrings (no. 2, th. 1).

#### Corollary {#ac-ix-s2-n3-cor-1 .statement}

Let C be a p-ring of finite length n. There exists a p-ring $C'$ of infinite length such that C is isomorphic to $C'/p^nC'$.

By prop. 5, there exists a p-ring $C'$ of infinite length such that $\kappa_{C'}$ is isomorphic to $\kappa_C$. Then $C'/p^nC' = C'_n$ is a p-ring of length n, and the field $\kappa_{C'_n}$ is isomorphic to $\kappa_{C'}$, hence to $\kappa_C$. By prop. 4, the rings C and $C'_n$ are therefore isomorphic.

### 4. Multiplicative Representatives

#### Proposition 6 {#ac-ix-s2-prop-6 .statement}

Let C be a p-ring, whose residue field k be perfect. Suppose that C is of finite length n (resp. infinite). There exists a unique isomorphism $u : W_n(k) \to C$ (resp. $u : W(k) \to C$) which induces, by passing to quotients, the identical mapping of k.

Since $W_n(k)$ (resp. $W(k)$) is a p-ring with residue field k, and of length n (resp. of infinite length) (No. 1, Example 2), and since $\varnothing$ is a p-basis of the perfect field k, prop. 6 is a particular case of prop. 4 of No. 3.

#### Theorem 2 {#ac-ix-s2-thm-2 .statement}

Let A be a separated complete local ring, k its residue field and $\pi$ the canonical homomorphism of A onto k. It is assumed that k is a perfect field of characteristic p.

a) There exists a unique ring homomorphism $u : W(k) \to A$ such that $\pi(u(a)) = a_0$ for $a = (a_n)_{n \in \mathbf{N}}$ in W(k).

b) The homomorphism u is continuous when W(k) is endowed with the $pW(k)$-adic topology, and the image of u is the unique Cohen subring of A.

By th. 1 of No. 2, there exists a unique Cohen subring of A; let us denote it by C. Let u be a homomorphism of W(k) into A such that $\pi(u(a)) = a_0$ for every $a = (a_n)_{n \in \mathbf{N}}$ in W(k); it is immediate that the image of u is a Cohen subring of A, hence equal to C. The existence and uniqueness of u then result from prop. 6. The $pC$-adic topology of C is induced by the $m_A$-adic topology of A (No. 2, th. 1, b)), whence the continuity of u.

For a direct construction of u, see p. 70, exerc. 6.

#### Proposition 7 {#ac-ix-s2-prop-7 .statement}

Let us retain the hypotheses and notations of th. 2. There exists a unique multiplicative subset S of A such that $\pi$ induces a bijection of S onto k. In order that an element a of A belong to S, it is necessary and sufficient that for every $n \in \mathbf{N}$, there exist an element $a_n$ of A such that $a = a_n^{p^n}$. The set S is the set of elements of the form $u(x, 0, 0, ...)$.

Let us first prove the uniqueness of S. Let S be a multiplicative subset of A, such that $\pi$ induces a bijection of S onto k. Let T be the set of elements of A which are $p^n$-th powers for every $n \in \mathbf{N}$.

a) One has $S \subset T$ : Let $a \in S$ and $n \in \mathbf{N}$; since the field k is perfect, there exists an element $x_n$ of k such that $x_n^{p^n} = \pi(a)$; since one has $\pi(S) = k$, there exists an element $a_n$ of S such that $x_n = \pi(a_n)$. One then has $\pi(a_n^{p^n}) = \pi(a)$ whence $a_n^{p^n} = a$ since the restriction of $\pi$ to S is injective.

b) The restriction of $\pi$ to T is injective: let a and b be two elements of T such that $\pi(a) = \pi(b)$. Let $n \in \mathbf{N}$; there exist two elements $a_n$ and $b_n$ of A such that $a = a_n^{p^n}, b = b_n^{p^n}$. We then have $\pi(a_n)^{p^n} = \pi(b_n)^{p^n}$, whence $\pi(a_n) = \pi(b_n)$, that is to say $a_n \equiv b_n$ mod. $m_A$. By Lemma 1 of § 1, No. 1, we have $a_n^{p^n} \equiv b_n^{p^n}$ mod. $m_A^{n+1}$ that is to say $a \equiv b$ mod. $m_A^{n+1}$. Since n is arbitrary, we have $a = b$.

Properties a) and b) above, together with the formula $\pi(S) = k$, imply the relation $S = T$, whence uniqueness.

Let us now prove the existence of S. With the notation of Theorem 2, put $\varphi = u \circ \tau_k$, that is to say (§ 1, No. 6)

(2)
$$
\varphi(x) = u(x, 0, 0, ...)
$$
for every $x \in k$. By Proposition 4 of loc. cit., we have

(3)
$$
\varphi(1) = 1,\quad \varphi(xy) = \varphi(x) \varphi(y) \text{ for } x, y \text{ in } k.
$$

It is clear that the mapping $\pi \circ \varphi$ is the identity mapping of $k$. Therefore the image S of $\varphi$ satisfies the conditions of Proposition 7.

The elements of S are often called the multiplicative (or Teichmüller) representatives of A.

#### Remark 1 {#ac-ix-s2-n4-rem-1 .statement}

Let us retain the preceding hypotheses and notation. We have
$$
a = \sum_{n=0}^{\infty} p^n \tau_k(a_n^{p^{-n}}) \quad (a = (a_n)_{n \in \mathbf{N}} \in \mathbf{W}(k))
$$
by Proposition 7 of § 1, No. 8. Hence
(4)
$$
u(a) = \sum_{n=0}^{\infty} p^n \varphi(a_n^{p^{-n}})
$$
for every $a = (a_n)_{n \in \mathbf{N}}$ in $\mathbf{W}(k)$, since $u$ is continuous (Theorem 2, b)). By formula (4), the unique Cohen subring of A consists of the elements of the form $\sum_{n=0}^{\infty} p^n s_n$ with $s_n \in S$ for every integer $n \geq 0$.

#### Remark 2 {#ac-ix-s2-n4-rem-2 .statement}

Let A be a separated and complete local ring, $k$ its residue field and $\pi$ the canonical homomorphism of A onto $k$. It may be shown that there exists a multiplicative subset S of A (not unique in general) such that $\pi$ induces a bijection of S onto $k$ (cf. p. 72, Exercise 11).

#### Example 1 {#ac-ix-s2-n4-exa-1 .statement}

Let $k$ be a perfect field of characteristic $p$. The multiplicative representatives of the ring $\mathbf{W}(k)$ are the Witt vectors $\tau(x) = (x, 0, 0, ...)$ for $x \in k$.

#### Example 2 {#ac-ix-s2-n4-exa-2 .statement}

Let A be an integral, separated and complete local ring. Suppose that the residue field $k$ of A is finite, with $q = p^f$ elements, hence perfect of characteristic $p$. We have $x^q = x$ for every $x \in k$, whence $s^q = s$ for every multiplicative representative s. It follows that the set of multiplicative representatives consists of 0 and the $q - 1$ $(q - 1)$-th roots of unity in the field of fractions of A. If the field of fractions of A is locally compact, the existence of multiplicative representatives also follows from VI, § 9, No. 2, Proposition 3 (cf. also VI, § 9, Exercise 5).

#### Example 3 {#ac-ix-s2-n4-exa-3 .statement}

More particularly, consider the case $A = \mathbf{Z}_p$. Then the multiplicative representatives are 0 and the $(p - 1)$-th roots of unity in the field of fractions $\mathbf{Q}_p$ of $\mathbf{Z}_p$.

### 5. Structure of complete noetherian local rings

Let $A$ and $C$ be complete noetherian local rings, and let $u$ be a local homomorphism of $C$ into $A$, inducing by passing to quotients an isomorphism of $\kappa_C$ onto $\kappa_A$. Let $(p_1, ..., p_m)$ be a sequence generating the ideal $m_C$ of $C$, and let $t_1, ..., t_n$ be elements of $m_A$. Put $B = C[[T_1, ..., T_n]]$.

#### Lemma 3 {#ac-ix-s2-lem-3 .statement}

a) There exists a unique homomorphism $v : B \to A$ extending $u$ and mapping $T_i$ to $t_i$ for $1 \leq i \leq n$.

b) In order that $v$ be surjective, it is necessary and sufficient that the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ generate the ideal $m_A$ of $A$, or again that the classes of these elements modulo $m_A^2$ generate $m_A/m_A^2$ as a vector space over the field $\kappa_A$.

c) In order that $v$ make $A$ into a finite $B$-algebra, it is necessary and sufficient that the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ generate an ideal of definition of (the $m_A$-adic topology of) $A$.

Let $n$ denote the ideal of the ring $B$ generated by $T_1, ..., T_n$. Every homomorphism $v$ of $B$ into $A$ extending $u$ and such that $v(T_i) = t_i$ maps $n$ into $m_A$, and is therefore continuous when $B$ is endowed with the $n$-adic topology. The existence and uniqueness of $v$ then result from A, IV, p. 26, Prop. 4.

The ring $B = C[[T_1, ..., T_n]]$ is a complete noetherian local ring (III, § 2, No. 10, Corollary 6 to Theorem 2 and No. 6, Proposition 6), whose maximal ideal $m_B$ is generated by $p_1, ..., p_m, T_1, ..., T_n$. Hence $v(m_B) \subset m_A$ and $v$ defines a homomorphism gr$(v)$ of $\operatorname{gr}(B) = \bigoplus_{n=0}^\infty m_B^n/m_B^{n+1}$ into $\operatorname{gr}(A) = \bigoplus_{n=0}^\infty m_A^n/m_A^{n+1}$. Now the ring $\operatorname{gr}(A)$ is generated by $A/m_A = \kappa_A$ and $m_A/m_A^2$, gr$(v)$ induces an isomorphism of $\kappa_B = \kappa_C$ onto $\kappa_A$, and the classes modulo $m_B^2$ of the elements $p_1, ..., p_m, T_1, ..., T_n$ generate $m_B/m_B^2$ as a vector space over $\kappa_B$; moreover $v$ is surjective if and only if gr$(v)$ is surjective (III, § 2, No. 8, Corollary 2 to Theorem 1). This proves $b$.

The ideal of $A$ generated by the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ is none other than $v(m_B)$ $A$. Since $m_A$ contains $v(m_B)$, $A$ is a Zariski ring for the $v(m_B)$ $A$-adic topology. The ring $A/v(m_B)$ $A$ is artinian if and only if its length as an $A$-module is finite. But since every simple module over $A$ is annihilated by $m_A$ and since, by hypothesis, $A/m_A$ and $B/m_B$ are isomorphic, this occurs if and only if the dimension over the field $B/m_B$ of the vector space $A/v(m_B)$ $A$ is finite. By IV, § 2, No. 5, Corollary 2 of Proposition 9, we see therefore that $v(m_B)$ $A$ is an ideal of definition of $A$ if and only if the dimension of $A/v(m_B)$ $A$ over $B/m_B$ is finite. This is indeed the case if $A$ is a finite $B$-algebra.

Suppose that $v(m_B)$ $A$ is an ideal of definition of $A$. The $m_B$-adic topology of the $B$-module $A$ then coincides with the $m_A$-adic topology of the ring $A$, and is therefore separated. Since $A/v(m_B)$ $A$ is a finitely generated module over $B/m_B$, $A$ is a finitely generated $B$-module (III, § 2, No. 3, Example 3 and No. 9, cor. 1 of Prop. 12). This proves $c$.

#### Lemma 4 {#ac-ix-s2-lem-4 .statement}

Suppose that the noetherian local ring C is regular, and that $(p_1, ..., p_m)$ is a system of coordinates of C (VIII, § 5, No. 1, Def. 1).

a) If the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ is secant for A (VIII, § 3, No. 2, Def. 1), the homomorphism $v : B \to A$ is injective.

b) In order that v be injective and make A a finite algebra over B, it is necessary and sufficient that $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ be a maximal secant sequence for A. Then A is of dimension $m + n$.

In order that the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ be a maximal secant sequence for A, it is necessary and sufficient that it generate an ideal of definition of A, and that A be of dimension $m + n$ (VIII, § 3, No. 2, Th. 1). By lemma 3, c), this comes to saying that A is a finite B-algebra, and a ring of dimension $m + n$. Now C is a noetherian integral ring of dimension $m$, hence $B = C[[T_1, ..., T_n]]$ is a noetherian integral ring of dimension $m + n$ (VIII, § 3, No. 4, cor. 3 of Prop. 8). If A is a finite B-algebra, and if $a$ is the kernel of $v$, one has $\dim(A) = \dim(B/a)$ (VIII, § 2, No. 3, th. 1, c)); since B is an integral ring of finite dimension, one has $\dim(B/a) < \dim(B)$ if $a \neq \{0\}$ (VIII, § 1, No. 3, prop. 6, e)). Hence, if A is a finite B-algebra, $v$ is injective if and only if A is of dimension $m + n$. This proves b).

Suppose that the sequence $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ of elements of $m_A$ is secant. One can adjoin to it (VIII, § 3, No. 2, Th. 1) elements $t_{n+1}, ..., t_{n+r}$ of $m_A$ in order to make it into a maximal secant sequence. From what precedes, there then exists an injective homomorphism $w$ of $C[[T_1, ..., T_n, T_{n+1}, ..., T_{n+r}]] = B[[T_{n+1}, ..., T_{n+r}]]$ which extends $v$ and maps $T_{n+j}$ to $t_{n+j}$ for $1 \leq j \leq r$. Hence $v$ is injective. This proves a).

#### Theorem 3 {#ac-ix-s2-thm-3 .statement}

Let A be a local, noetherian and complete ring whose residue field k is of characteristic p. Let C be a p-ring of infinite length, whose residue field is isomorphic to k (No. 3, Prop. 5).

a) Let m be the dimension of the vector space $m_A/(m_A^2 + pA)$ over the field k. There exists an ideal $a$ of the ring $C[[T_1, ..., T_m]]$ such that A is isomorphic to $C[[T_1, ..., T_m]]/a$.

b) Let d be the dimension of A. Suppose that $p1_A$ is not a divisor of 0 in A. Then there exists a subring $A'$ of A isomorphic to $C[[T_1, ..., T_{d-1}]]$ and such that A is a finite algebra over $A'$.

Let $C'$ be a Cohen subring of $A$ (No. 2, Theorem 1). Since $C$ is of infinite length, there exists a homomorphism of $C$ onto $C'$ (No. 3, Proposition 4). Consequently, there exists a local homomorphism $u : C \to A$. Let us choose elements $t_1, ..., t_m$ of $m_A$ whose classes form a basis of the vector space $m_A/(m_A^2 + pA)$ over the field $k$. We have $u(p1_C) = p1_A$, and Lemma 3, b) proves the existence of a surjective homomorphism of $C[[T_1, ..., T_m]]$ onto $A$, extending $u$ and mapping $T_i$ to $t_i$ for $1 \leq i \leq m$. This proves a).

Suppose that $p1_A$ is not a divisor of $0$ in $A$, hence is secant for $A$ (VIII, § 3, No. 2, Proposition 3). Then there exist (VIII, § 3, No. 2, Theorem 1) elements $t_1, ..., t_{d-1}$ of $m_A$ such that the sequence $(p1_A, t_1, ..., t_{d-1})$ is a maximal secant sequence for $A$. The noetherian local ring $C$ is regular, and $(p1_C)$ is a system of coordinates of $C$. The assertion b) of Theorem 3 then follows from Lemma 4, b).

## EXERCISES {#ac-ix-s2-exercises}

In the exercises of § 2, $p$ is a fixed prime number. If $a$ is an ideal of a ring $A$, $a^p$ denotes the ideal generated by the elements $a^p$, where $a$ ranges over $a$.

See the [exercises for § 2](exercises/s2/).
