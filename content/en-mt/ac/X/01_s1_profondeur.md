---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 1
section_title: Profondeur
lang: en
source: ac-x-fr
book_pages: AC X.3-AC X.22
pdf_pages: 0002-0021, 0150-0153
extraction: ocr
subsections:
    - "no": 2
      title: Profondeur et acyclicité
      page: 4
      pdf_page: 3
    - "no": 3
      title: Profondeur et complexe de Koszul
      page: 5
      pdf_page: 4
    - "no": 4
      title: Profondeur et suites régulières
      page: 8
      pdf_page: 7
    - "no": 5
      title: Profondeur le long d’une partie fermée
      page: 0
      pdf_page: 9
    - "no": 6
      title: Profondeur des algèbres
      page: 11
      pdf_page: 10
    - "no": 7
      title: Majorations de la profondeur
      page: 13
      pdf_page: 12
    - "no": 8
      title: Anneaux noethériens localement intègres ; anneaux noethériens normaux
      page: 15
      pdf_page: 14
    - "no": 9
      title: Profondeur et connexité
      page: 0
      pdf_page: 15
    - "no": 10
      title: Profondeur et normalité
      page: 19
      pdf_page: 18
statements: 60
exercises: 18
content_sha256: 45ce4aed8b702b2a4fc75c122b0bedf601f22162b148fd2e307422069f1eee3b
translated_from: content/fr/ac/X/01_s1_profondeur.md
source_lang: fr
translation_method: machine
source_content_sha256: 225c9460593c8de13dabe30c37d11a994b8dc41f2db1aa24ece65402eb5a3910
translation_model: gpt-5.4
translation_run: translate-en-mt-e62336b8
glossary_version: 34
glossary_terms_sha256: 07c5a90451887259a465f1827398c82fb0bca0868ef90f172c1015a08935bd39
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. DEPTH

#### Proposition 1 {#ac-x-s1-prop-1 .statement}

Let $A$ be a ring, $J$ an ideal of $A$ and $0 \to M' \to M \to M'' \to 0$ an exact sequence of $A$-modules. Put

$$
p' = \operatorname{prof}(J; M') \quad , \quad p = \operatorname{prof}(J; M) \quad , \quad p'' = \operatorname{prof}(J; M'') .
$$

Then one is in one of the following three cases, which are mutually exclusive:

$$
p' = p \leqslant p'' \quad , \quad p = p'' < p' \quad , \quad p'' = p' - 1 < p .
$$

Consider the exact sequence of extension modules associated with $A/J$ and with the exact sequence above (A, X, p. 92, th. 2). Exclude the case $p = p' = p'' = +\infty$; there then exists in this sequence a first nonzero module, and the following module is also nonzero. This gives the following three possibilities:

a) The first nonzero module is $\operatorname{Ext}_A^{p'}(A/J, M')$. Then $p' = p \leqslant p''$.

b) The first nonzero module is $\operatorname{Ext}_A^p(A/J, M)$. Then $p = p'' < p'$.

c) The first nonzero module is $\operatorname{Ext}_A^{p''}(A/J, M'')$. Then $p'' + 1 = p' \leqslant p$.

#### Remark 5 {#ac-x-s1-rem-5 .statement}

Suppose that one has $p = p'$ and that the injection $u : M' \to M$ which occurs in the exact sequence of prop. 1 belongs to $J \operatorname{Hom}_A(M', M)$. *One then has* $p'' = p - 1$. In fact, the assumption implies that the mapping $\operatorname{Ext}_A^i(1_{A/J}, u)$ is zero for every integer $i$; this excludes case a) considered above.

#### Proposition 2 {#ac-x-s1-prop-2 .statement}

Let $A$ be a ring, $J$ an ideal of $A$, $M$ an $A$-module and $N$ an $A$-module annihilated by a power of $J$. *One has* $\operatorname{Ext}_A^i(N, M) = 0$ *for every integer* $i < \operatorname{prof}_A(J; M)$.

Suppose first that $JN = 0$ and reason by induction on the integer $i < \operatorname{prof}_A(J; M)$. The assertion is obvious for $i < 0$. Consider $N$ as an $(A/J)$-module and choose an exact sequence of $(A/J)$-modules

$$
0 \to K \longrightarrow (A/J)^{(I)} \longrightarrow N \to 0 .
$$

One deduces from this an exact sequence of extension modules

$$
\operatorname{Ext}_A^{i-1}(K, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i((A/J)^{(I)}, M) .
$$

The $A$-module $\operatorname{Ext}_A^{i-1}(K, M)$ is zero by the induction hypothesis, and the $A$-module $\operatorname{Ext}_A^i((A/J)^{(I)}, M)$ is isomorphic to $\operatorname{Ext}_A^i(A/J, M)^I$ (A, X, p. 89, prop. 7), which is zero by definition of depth. Hence one has $\operatorname{Ext}_A^i(N, M) = 0$.

Pass to the general case, and reason by induction on the smallest integer $m > 0$ such that $J^m N = 0$. We have just treated the case $m = 1$. Suppose $m > 1$ and let $i < \operatorname{prof}_A(J; M)$ be an integer. Consider the exact sequence

$$
\operatorname{Ext}_A^i(N/JN, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i(JN, M)
$$

deduced from the exact sequence $0 \to JN \to N \to N/JN \to 0$. The two extreme modules are zero by the induction hypothesis, since $N/JN$ and $JN$ are annihilated by $J^{m-1}$. Therefore one has $\operatorname{Ext}_A^i(N, M) = 0$, which was to be proved.

#### Corollary 1 {#ac-x-s1-prop-2-cor-1 .statement}

Let m be an integer > 0 and let J' be an ideal of A which contains J^m. One has prof_A(J ; M) \leq prof_A(J' ; M).

In fact J^m annihilates the A-module A/J', hence Ext^i_A(A/J', M) is zero for every integer i < prof_A(J ; M) (prop. 2).

#### Corollary 2 {#ac-x-s1-prop-2-cor-2 .statement}

Suppose the ideal J to be of finite type, and let J' be an ideal of A such that V(J) \supset V(J').

a) One has prof_A(J ; M) \leq prof_A(J' ; M).

b) If the ideal J' is of finite type and if V(J) = V(J'), one has prof_A(J ; M) = prof_A(J' ; M).

By II, § 4, No. 3, cor. 2 of prop. 11 and § 2, No. 6, prop. 15, there exists an integer m > 0 such that J^m \subset J'. The assertion a) therefore follows from cor. 1 and assertion b) is deduced from it.

Cor. 2 may fail when the ideal J is not of finite type (exercise 2).

### 2. Depth and Acyclicity

#### Proposition 3 {#ac-x-s1-prop-3 .statement}

Let A be a ring, C a complex of A-modules bounded on the left and p an integer. Suppose that for every pair of integers (m, n) with m \geq n \geq p, the depth of the A-module C_m relative to the annihilator of H_n(C) is > m - n. Then one has H_n(C) = 0 for n \geq p.

Since C is bounded on the left, H_n(C) is zero for n sufficiently large. If the conclusion were false, there would exist an integer q \geq p such that H_n(C) = 0 for n > q and H_q(C) \neq 0. Denote by J the annihilator of H_q(C); one then has prof_A(J ; H_q(C)) = 0. Moreover, since Z_q(C) is a submodule of C_q, and since by hypothesis one has prof_A(J ; C_q) > q - q = 0, one has prof_A(J ; Z_q(C)) > 0. One then deduces from the exact sequence

$$
0 \to B_q(C) \to Z_q(C) \to H_q(C) \to 0
$$

the equality prof_A(J ; B_q(C)) = 1 (No. 1, prop. 1). By the definition of q, B_n(C) is equal to Z_n(C) for every integer n > q. From the canonical exact sequences

$$
0 \to B_n(C) \to C_n \to B_{n-1}(C) \to 0 \quad (n > q)
$$

and from the hypothesis prof_A(J ; C_n) > n - q, one obtains by induction the equality prof_A(J ; B_n(C)) = n - q + 1 for every n \geq q (loc. cit.). But this is absurd since B_n(C) is zero for n sufficiently large.

#### Corollary 1 {#ac-x-s1-prop-3-cor-1 .statement}

Let A be a ring, J an ideal of A, C a complex of A-modules bounded on the left and p an integer. Suppose that one has JH_m(C) = 0 and prof_A(J ; C_m) > m - p for m \geq p. Then one has H_n(C) = 0 for n \geq p.

In fact for n \geq p the annihilator J_n of H_n(C) contains J, hence one has prof_A(J_n ; C_m) \geq prof_A(J ; C_m) (No. 1, cor. 1 of prop. 2), so that the hypothesis of the proposition is satisfied.

#### Corollary 2 {#ac-x-s1-prop-3-cor-2 .statement}

Let $A$ be a local ring, $C$ a complex of $A$-modules bounded to the left, $p$ an integer. Suppose that for $m \geq p$, $H_m(C)$ is of finite length and $C_m$ of depth $> m - p$. Then $H_n(C) = 0$ for $n \geq p$.

The $A$-module $\bigoplus_{m \geq p} H_m(C)$ is of finite length. Let $J$ denote its annihilator; by A, VIII, § 1, No. 3, corollary, the ring $A/J$ is artinian, hence $J$ contains a power of the maximal ideal of $A$ (A, VIII, § 10, No. 1, th. 1). It follows that $\operatorname{prof}_A(J; C_m) \geq \operatorname{prof}(C_m) > m - p$ for $m \geq p$ (No. 1, cor. 1 of prop. 2), so that one may apply cor. 1.

### 3. Depth and Koszul complex

Let $A$ be a ring, $M$ an $A$-module, $x = (x_i)_{i \in I}$ a family of elements of $A$. Let $u : A^{(I)} \to A$ denote the linear form such that $u(e_i) = x_i$ for every $i \in I$, and $K^\bullet(x, M)$ the complex $K_A^\bullet(u, M)$ associated with $u$ (A, X, p. 147). We have $K^p(x, M) = 0$ for $p < 0$; for $p \geq 0$ the $A$-module $K^p(x, M) = \operatorname{Hom}_A(\Lambda^p(A^{(I)}), M)$ is canonically identified with the $A$-module $C_I^p(M)$ formed by the alternating mappings of $I^p$ into $M$ (A, X, p. 153), the differential $\partial^p : K^p(x, M) \to K^{p+1}(x, M)$ being given by the formula

$$
(\partial^p m)(\alpha_1, \ldots, \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, \ldots, \alpha_{j-1}, \alpha_{j+1}, \ldots, \alpha_{p+1})
$$

for $m \in K^p(x, M)$ and $(\alpha_1, \ldots, \alpha_{p+1}) \in I^{p+1}$ (A, X, p. 154, formula (12)). It follows in particular that the complex $K^\bullet(x, M)$ depends only on the structure of $M$ as a $\mathbf{Z}$-module and on the endomorphisms $(x_i)_M$.

We denote by $H^\bullet(x, M)$ the homology of the complex $K^\bullet(x, M)$. The $A$-module $H^0(x, M)$ is identified with $\operatorname{Hom}_A(A/J, M)$, where $J$ is the ideal of $A$ generated by the $x_i$ (A, X, p. 147, lemma 1).

Let $(M_\alpha)_{\alpha \in K}$ be a family of $A$-modules, and $M$ its product; the complex $K^\bullet(x, M)$ is canonically isomorphic to the product complex of the $K^\bullet(x, M_\alpha)$, so that for each integer $s$ the $A$-module $H^s(x, M)$ is identified with the product of the $H^s(x, M_\alpha)$ (A, X, p. 28, Proposition 1).

#### Theorem 1 {#ac-x-s1-thm-1 .statement}

Let $A$ be a ring, $J$ an ideal of $A$, $x = (x_i)_{i \in I}$ a generating family of $J$, $M$ an $A$-module. The depth of $M$ relative to $J$ is the greatest lower bound (in $\mathbf{N} \cup \{+\infty\}$) of the integers $n$ such that $H^n(x, M) \neq 0$.

Put $p = \operatorname{prof}_A(J; M)$. Consider the complex $K^\bullet(x, M)$. Its homology is annihilated by $J$ (A, X, p. 148, Corollary 2), and the depth relative to $J$ of each of the modules $K^i(x, M)$ is equal to $p$ or to $+\infty$ (No. 1, Remark 4). It then follows from Corollary 1 of No. 2 that we have $H^i(x, M) = 0$ for $i < p$. It remains to prove that $H^p(x, M)$ is non-zero when $p < +\infty$.

The case $p = 0$ being evident, suppose $0 < p < +\infty$ and $H^p(x, M) = 0$. Let $L$ be a free resolution of the $A$-module $A/J$; let $C$ denote the complex $\operatorname{Homgr}_A(L, M)$. The $A$-module $H^i(C)$ is isomorphic to $\operatorname{Ext}_A^i(A/J, M)$ (A, X, p. 100, Theorem 1); it is therefore zero for $i < p$. We then have for $i < p$ canonical exact sequences

$$
0 \to B^i(C) \to C^i \to B^{i+1}(C) \to 0 .
$$

The $A$-module $C^i$ is a product of $A$-modules isomorphic to $M$; therefore $H^s(x, C^i) = 0$ for $s \leq p$. From the preceding exact sequences and from A, X, p. 150, we deduce that the connecting homomorphism $\partial^s : H^s(x, B^{i+1}(C)) \longrightarrow H^{s+1}(x, B^i(C))$ is injective for $s \leq p$ and $i < p$; since $B^0(C) = 0$, it follows that $H^{p-i}(x, B^{i+1}(C))$ is zero for $i < p$. In particular, we have $H^1(x, B^p(C)) = 0$, so that the exact sequence

$$
0 \to B^p(C) \to Z^p(C) \to H^p(C) \to 0
$$

yields a surjection $H^0(x, Z^p(C)) \longrightarrow H^0(x, H^p(C))$. Since $H^p(C)$ is isomorphic to $\operatorname{Ext}_A^p(A/J, M)$, which is nonzero and annihilated by J, one has $H^0(x, H^p(C)) \neq 0$, whence $H^0(x, Z^p(C)) \neq 0$ and consequently $H^0(x, C^p) \neq 0$. But this implies $H^0(x, M) \neq 0$, contrary to the hypothesis. Hence $H^p(x, M) \neq 0$, which completes the proof.

#### Corollary 1 {#ac-x-s1-thm-1-cor-1 .statement}

*Suppose the ideal J to be of finite type and JM $\neq$ M. Then* $\operatorname{prof}_A(J; M)$ *is finite and $\leq$ Card(I)* ; *in order that it be equal to Card(I), it is necessary and sufficient that the family x be completely secant for M* (A, X, p. 157, Def. 2).

Suppose first that I is finite, and let r denote its cardinal. The A-module $H^r(x, M)$ is canonically isomorphic to $H_0(x, M)$, itself isomorphic to $M/JM$ (A, X, p. 155); the inequality $\operatorname{prof}_A(J; M) \leq r$ therefore follows from Theorem 1. For equality to hold, it is necessary and sufficient that the A-module $H^i(x, M)$ be zero for $i < r$, which signifies that the family x is completely secant for M (A, X, p. 157).

From the foregoing, $\operatorname{prof}_A(J; M)$ is finite; it remains to prove that if the family x is completely secant for M, the set I is finite. Now the condition $H_1(x, M) = 0$ (A, X, p. 157, Def. 2) implies that one has an exact sequence

$$
\Lambda^2(A^{(I)}) \otimes_A M \xrightarrow{\partial_2} M^{(I)} \xrightarrow{\partial_1} JM \to 0 ,
$$

where the image of $\partial_2$ is contained in $JM^{(I)}$. By tensor product with $A/J$, one deduces from this an A-linear isomorphism of $(M/JM)^{(I)}$ onto $JM/J^2M$. Now the latter module is of finite type, since J and M are so; as $M/JM$ is not zero, it follows that the set I is finite.

#### Corollary 2 {#ac-x-s1-thm-1-cor-2 .statement}

*Let A be a local ring, J an ideal of finite type of A distinct from A, M a nonzero A-module of finite type. Put* $r = [J/m_AJ : \kappa_A]$. *One has* $\operatorname{prof}_A(J; M) \leq r$ ; *there is equality if and only if J is generated by a family completely secant for M. In this case, in order that a generating family of J be completely secant, it is necessary and sufficient that it have r elements*.

By Nakayama's lemma, one has $JM \neq M$, and r is the minimal number of generators of J; Corollary 2 therefore follows from Corollary 1.

#### Proposition 4 {#ac-x-s1-prop-4 .statement}

Let $\rho : A \to B$ be a ring homomorphism, $J$ an ideal of $A$ and $N$ a $B$-module. One has the equality $\operatorname{prof}_A(J; N) = \operatorname{prof}_B(JB; N)$.

Let $x = (x_i)_{i \in I}$ be a generating family of $J$; the family $\rho(x) = (\rho(x_i))_{i \in I}$ generates $JB$. By construction the complex $K^\bullet(\rho(x), N)$ is equal to $K^\bullet(x, N)$. The proposition therefore follows from Theorem 1.

#### Corollary {#ac-x-s1-n3-cor-1 .statement}

Let $A$ be a local ring, $a$ an ideal of $A$ distinct from $A$ and $M$ an $A$-module annihilated by $a$. One has $\operatorname{prof}_A(M) = \operatorname{prof}_{A/a}(M)$.

Let $\rho : A \to B$ be a ring homomorphism, $x = (x_i)_{i \in I}$ a finite family of elements of $A$ and $M$ an $A$-module. For every integer $p$, let us denote by $u^p : B \otimes_A C_I^p(M) \to C_I^p(B \otimes_A M)$ the $B$-linear homomorphism which associates to $b \otimes m$ the alternating mapping $(\alpha_1, \ldots, \alpha_p) \mapsto b \otimes m(\alpha_1, \ldots, \alpha_p)$. The family $(u^p)$ defines an isomorphism of complexes

$$
u : B \otimes_A K^\bullet(x, M) \to K^\bullet(x, B \otimes_A M)
$$

Let us consider the canonical homomorphism

$$
\gamma^p(B, K^\bullet(x, M)) : B \otimes_A H^p(x, M) \to H^p(B \otimes_A K^\bullet(x, M))
$$

(A, X, p. 62); by composition with $H^p(u)$, we deduce from it a homomorphism

$$
v^p : B \otimes_A H^p(x, M) \to H^p(x, B \otimes_A M)
$$

#### Lemma 1 {#ac-x-s1-lem-1 .statement}

If the $A$-module $B$ is flat, the homomorphism $v^p$ is bijective for every integer $p$.

This results from A, X, p. 66, Cor. 2.

#### Proposition 5 {#ac-x-s1-prop-5 .statement}

Let $A$ be a ring, $J$ an ideal of finite type of $A$ and $M$ an $A$-module. Let $\Omega$ denote the set of maximal ideals of $A$ belonging to $\operatorname{Supp}(M)$ and containing $J$. Then

$$
\operatorname{prof}_A(J; M) = \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) = \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)
$$

Let $x = (x_i)_{i \in I}$ be a finite generating family of $J$. Let $p$ be a prime ideal of $A$; the ideal $J_p$ is generated by the image $x_p$ of the family $(x_i)$ in $A_p$. For every $p \geq 0$, the $A_p$-module $(H^p(x, M))_p$ is isomorphic to $H^p(x_p, M_p)$ (Lemma 1); in view of Theorem 1, we therefore have $\operatorname{prof}_A(J; M) \leq \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) \leq \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)$.

Let $p$ be an integer strictly less than $\operatorname{prof}_{A_m}(JA_m; M_m)$ for every $m \in \Omega$. Then $H^p(x_m, M_m) = 0$ for every maximal ideal $m$ of $A$: this results from Theorem 1 if $m \in \Omega$, from the fact that $M_m = 0$ if $m \not\in \operatorname{Supp}(M)$, and from the fact that the ideal $JA_m$, which annihilates $H^p(x_m, M_m)$ (A, X, p. 148, Cor. 2), is equal to $A_m$ if $m \not\in V(J)$. Hence $(H^p(x, M))_m = 0$ for every maximal ideal $m$ of $A$, which implies $H^p(x, M) = 0$ (II, § 3, No. 3, Cor. 2 of Theorem 1). The proposition then results from Theorem 1.

#### Proposition 6 {#ac-x-s1-prop-6 .statement}

Let $A$ be a ring, $J$ an ideal of finite type of $A$ and $M$ an $A$-module. Let $B$ be a ring and $\rho : A \to B$ a ring homomorphism making $B$ into a flat $A$-module.

a) One has $\operatorname{prof}_A(J; M) \leq \operatorname{prof}_B(JB; B \otimes_A M)$.

b) Suppose moreover that every maximal ideal of $\operatorname{Supp}(M)$ containing $J$ belongs to the image of the canonical mapping $\operatorname{Spec}(B) \to \operatorname{Spec}(A)$. Then one has $\operatorname{prof}_A(J; M) = \operatorname{prof}_B(JB; B \otimes_A M)$. This is the case for example if the $A$-module $B$ is faithfully flat.

Assertion a) follows from Theorem 1 and Lemma 1.

Let $p$ be an integer strictly less than $\operatorname{prof}_B(JB; B \otimes_A M)$, and let $m$ be a maximal ideal of $A$ belonging to $\operatorname{Supp}(M) \cap V(J)$. Let $x$ be a finite generating family of the ideal $J$. Under the hypothesis of b), there exists a prime ideal $n$ of $B$ lying over $m$, and one has a canonical isomorphism

$$
B_n \otimes_{A_m} (A_m \otimes_A H^p(x, M)) \longrightarrow B_n \otimes_B (B \otimes_A H^p(x, M))
$$

Now $B \otimes_A H^p(x, M)$ is isomorphic to $H^p(\rho(x), B \otimes_A M)$ (Lemma 1), hence is zero; moreover $B_n$ is faithfully flat over $A_m$ (I, § 3, No. 5, Proposition 9 and II, § 3, No. 4, Proposition 14 and Remark). Hence one has $A_m \otimes_A H^p(x, M) = 0$ and therefore $p < \operatorname{prof}_{A_m}(J_m; M_m)$ (Lemma 1 and Theorem 1). The first assertion of b) then follows from Proposition 5; the second follows from I, § 3, No. 5, Proposition 9).

#### Corollary {#ac-x-s1-n3-cor-2 .statement}

Let $A$ be a noetherian ring, $J$ an ideal of $A$, $M$ a finitely generated $A$-module, $\widehat{A}$ and $\widehat{M}$ the separated completions of $A$ and $M$ for the $J$-adic topology. Then one has $\operatorname{prof}_A(J; M) = \operatorname{prof}_{\widehat{A}}(J\widehat{A}; \widehat{M})$.

In fact, the $A$-module $\widehat{A}$ is flat and the $\widehat{A}$-module $\widehat{M}$ is isomorphic to $\widehat{A} \otimes_A M$ (III, § 3, No. 4, Theorem 3); moreover, every maximal ideal of $A$ containing $J$ belongs to the image of the mapping $\operatorname{Spec}(\widehat{A}) \to \operatorname{Spec}(A)$ (*loc. cit.*, Proposition 8).

### 4. Depth and regular sequences

Let $A$ be a ring, $M$ an $A$-module. Recall (A, X, p. 158) that a finite sequence $(x_1, \ldots, x_r)$ of elements of $A$ is said to be *regular for $M$* or *$M$-regular* if, for $i = 1, \ldots, r$, the homothety with ratio $x_i$ in the $A$-module $M/(x_1 M + \ldots + x_{i-1} M)$ is injective. Let $(x_1, \ldots, x_r)$ be an $M$-regular sequence; for every flat $A$-module $N$, the sequence $(x_1, \ldots, x_r)$ is regular for $M \otimes_A N$. If $\rho : A \to B$ is a ring homomorphism making $B$ into a flat $A$-module, the sequence $(\rho(x_1), \ldots, \rho(x_r))$ is regular for the $B$-module $B \otimes_A M$. In particular, for every prime ideal $p$ of $A$, the image in $A_p$ of the sequence $(x_1, \ldots, x_r)$ is $M_p$-regular.

In the sequel we shall consider chiefly the notion of an $M$-regular sequence in the case where the ring $A$ is local noetherian, the module $M$ is finitely generated and the elements of the sequence belong to $m_A$; the notion of an $M$-regular sequence then coincides with that of a completely secant sequence for $M$ (A, X, p. 160, cor. 1).

#### Proposition 7 {#ac-x-s1-prop-7 .statement}

Let $A$ be a ring, $J$ an ideal of $A$, $M$ an $A$-module, and $(x_1, \ldots, x_r)$ an $M$-regular sequence of elements of $J$. Then
$$
\operatorname{prof}_A(J; M) = r + \operatorname{prof}_A(J; M/(x_1M + \ldots + x_rM))
$$
and in particular $\operatorname{prof}_A(J; M) \geqslant r$.

The case $r = 1$ follows from Remark 5 of No. 1, applied to the exact sequence
$$
0 \to M \xrightarrow{(x_1)_M} M \longrightarrow M/x_1M \to 0 .
$$
The general case follows by induction on $r$.

#### Theorem 2 {#ac-x-s1-thm-2 .statement}

Let $A$ be a noetherian ring, $J$ an ideal of $A$ and $M$ a finitely generated $A$-module.

a) Suppose that $\operatorname{prof}_A(J; M)$ is finite. Then every $M$-regular sequence of elements of $J$ can be completed to an $M$-regular sequence of length $\operatorname{prof}_A(J; M)$ of elements of $J$.

b) The depth of $M$ relative to $J$ is the least upper bound of the lengths of $M$-regular sequences formed of elements of $J$.

c) For $\operatorname{prof}_A(J; M)$ to be finite, it is necessary and sufficient that the support of $M$ meet $V(J)$, or again that one have $JM \neq M$.

Let $(x_1, \ldots, x_r)$ be an $M$-regular sequence of elements of $J$. One has $r \leqslant \operatorname{prof}_A(J; M)$ (Prop. 7); suppose that the inequality is strict. Let $N$ denote the $A$-module $M/(x_1M + \ldots + x_rM)$. One has $\operatorname{prof}_A(J; N) > 0$ (*loc. cit.*), so that there exists an element $x$ of $J$ such that the homothety $x_N$ is injective (No. 1, Remark 2), that is to say, such that the sequence $(x_1, \ldots, x_r, x)$ is $M$-regular. It follows by induction that for every integer $s$ such that $r \leqslant s \leqslant \operatorname{prof}_A(J; M)$ the sequence $(x_1, \ldots, x_r)$ can be completed to an $M$-regular sequence of length $s$, which entails assertions a) and b). Assertion c) follows from Remark 1 of No. 1 and Corollary 1 of Theorem 1 of No. 3.

#### Corollary 1 {#ac-x-s1-thm-2-cor-1 .statement}

For every $M$-regular sequence $(x_1, \ldots, x_r)$ of elements of $J$, the following properties are equivalent:

(i) one has $r = \operatorname{prof}_A(J; M)$ ;
(ii) the sequence $(x_1, \ldots, x_r)$ is maximal among the $M$-regular sequences formed of elements of $J$ ;
(iii) the $A$-module $M/(x_1M + \ldots + x_rM)$ has a nonzero element annihilated by $J$ ;
(iv) one has $\operatorname{Ass}(M/(x_1M + \ldots + x_rM)) \cap V(J) \neq \varnothing$.

The equivalence of (i) and (ii) follows from Theorem 2; the equivalence of (ii), (iii) and (iv) follows from Remark 2 of No. 1 applied to the $A$-module $M/(x_1M + \ldots + x_rM)$.

#### Corollary 2 {#ac-x-s1-thm-2-cor-2 .statement}

Let $A$ be a noetherian local ring, $M$ a nonzero finitely generated $A$-module. One has
$$
\operatorname{prof}_A(M) \leqslant \dim_A(M) < +\infty .
$$

### 5. Depth along a closed subset

Let A be a noetherian ring, F a closed subset of $\mathrm{Spec}(A)$ and M an A-module. By Corollary 2 of Proposition 2 of No. 1, the element $\mathrm{prof}_A(J;M)$ of $\mathbf{N} \cup \{+\infty\}$ does not depend on the ideal J of A such that $F = V(J)$; it is called the *depth of M along F* and is denoted by $\mathrm{prof}_F(M)$.

#### Remark 1 {#ac-x-s1-n5-rem-1 .statement}

Let r be an integer. By Proposition 2 of No. 1 and II, § 4, No. 4, Corollary 2 of Proposition 17, the inequality $\mathrm{prof}_F(M) \geqslant r$ is equivalent to the following property: for every finitely generated A-module N whose support is contained in F, one has $\mathrm{Ext}_A^i(N,M) = 0$ for $i < r$.

#### Remark 2 {#ac-x-s1-n5-rem-2 .statement}

Suppose that the A-module M is finitely generated. By Remark 2 of No. 1 and Theorem 2 of No. 4, one has the following equivalences

$$
\mathrm{prof}_F(M) = 0 \iff \mathrm{Ass}(M) \cap F \neq \varnothing \\
\mathrm{prof}_F(M) < +\infty \iff \mathrm{Supp}(M) \cap F \neq \varnothing .
$$

#### Proposition 8 {#ac-x-s1-prop-8 .statement}

*Let A be a noetherian ring, F a closed subset of $\mathrm{Spec}(A)$, and M a finitely generated A-module. One has*

$$
\mathrm{prof}_F(M) = \inf_{p \in F} \mathrm{prof}_{A_p}(M_p) = \inf_{p \in \mathrm{Supp}(M) \cap F} \mathrm{prof}_{A_p}(M_p) .
$$

This is clear if $\mathrm{prof}_F(M) = +\infty$ (Remark 2). If $\mathrm{prof}_F(M) = 0$, there exists a prime ideal $p \in \mathrm{Ass}(M) \cap F$ (Remark 2); one has $pA_p \in \mathrm{Ass}(M_p)$ (IV, § 1, No. 2, Prop. 5), hence $\mathrm{prof}_{A_p}(M_p) = 0$ (Remark 2 of No. 1), whence the proposition in this case.

Suppose $0 < \mathrm{prof}_F(M) < +\infty$; let J be an ideal of A such that $V(J) = F$, and let x be an element of J such that the homothety $x_M$ is injective (*loc. cit.*). For each prime ideal p, the homothety $x_{M_p}$ is injective. By Prop. 7 of No. 4, we therefore have

$$
\mathrm{prof}_F(M/xM) = \mathrm{prof}_F(M) - 1 \\
\mathrm{prof}_{A_p}((M/xM)_p) = \mathrm{prof}_{A_p}(M_p) - 1 .
$$

One then concludes by induction on the integer $\mathrm{prof}_F(M)$.

#### Remark 3 {#ac-x-s1-n5-rem-3 .statement}

If q is a point of $\mathrm{Supp}(M)$, we therefore have $\mathrm{prof}_A(q;M) = \inf_{p \supseteq q} \mathrm{prof}_{A_p}(M_p)$. In particular, one has the inequality $\mathrm{prof}_A(q;M) \leqslant \mathrm{prof}_{A_q}(M_q)$; there is equality when q is maximal. In the general case, one may have $\mathrm{prof}_A(q;M) < \mathrm{prof}_{A_q}(M_q)$; one may also have $\mathrm{prof}_A(q;M) < \inf \mathrm{prof}_{A_m}(M_m)$ where m runs through the set of maximal ideals of A containing q. Let p, for example, be a nonmaximal prime ideal of A, containing q and distinct from q; put $M = A/p$. One has $\mathrm{prof}_A(q;M) = 0$, $\mathrm{prof}_{A_q}(M_q) = +\infty$ and $\mathrm{prof}_{A_m}(M_m) > 0$ for every maximal ideal m of A.

#### Proposition 9 {#ac-x-s1-prop-9 .statement}

Let $A$ be a noetherian ring, $M$ and $N$ two A-modules of finite type, and $F$ the support of $N$. Then $\mathrm{prof}_F(M)$ is the greatest lower bound (in $N \cup \{+\infty\}$) of the set of integers $n$ such that $\mathrm{Ext}_A^n(N, M) \neq 0$.

By Remark 1, one has $\mathrm{Ext}_A^i(N, M) = 0$ for every $i < \mathrm{prof}_F(M)$. It remains to prove that if $\mathrm{prof}_F(M) = n < +\infty$, one has $\mathrm{Ext}_A^n(N, M) \neq 0$. Let $J$ be the annihilator of $N$; one has $F = V(J)$, hence $\mathrm{prof}_F(M) = \mathrm{prof}_A(J; M)$. By Cor. 1 of Th. 2 (No. 4), there exists an $M$-regular sequence $(x_1, \ldots, x_n)$ of length $n$ consisting of elements of $J$, and the depth relative to $J$ of the A-module $\overline{M} = M/(x_1 M + \ldots + x_n M)$ is zero. By A, X, p. 166, Prop. 9, it is enough to prove that $\mathrm{Hom}_A(N, \overline{M})$ is nonzero. Now, by Prop. 8, there exists $p \in \mathrm{Supp}(M) \cap \mathrm{Supp}(N)$ such that $\mathrm{prof}_{A_p}(\overline{M}_p) = 0$, that is to say $\mathrm{Hom}_{A_p}(\kappa(p), \overline{M}_p) \neq 0$. Since $N_p$ is nonzero, the $\kappa(p)$-vector space $N_p \otimes_{A_p} \kappa(p)$ is nonzero (Nakayama's lemma), and so is its dual; there therefore exists a surjective $A_p$-linear mapping of $N_p$ onto $\kappa(p)$. It follows that one has $\mathrm{Hom}_{A_p}(N_p, \overline{M}_p) \neq 0$, hence $\mathrm{Hom}_A(N, \overline{M}) \neq 0$ (II, § 2, No. 7, Prop. 19), which was to be proved.

#### Remark 4 {#ac-x-s1-n5-rem-4 .statement}

Let $A$ be a noetherian ring, $N$ a finitely generated $A$-module. The greatest lower bound in $N \cup \{+\infty\}$ of the set of integers $n$ such that $\mathrm{Ext}_A^n(N, A)$ is nonzero is sometimes called the grade of $N$, and is denoted by grade$(N)$. By Prop. 9, this is also the depth of $A$ along the support of $N$, or again (No. 4, Theorem 2) the least upper bound of the set of lengths of $A$-regular sequences of elements of the annihilator of $N$. Since for every prime ideal $p$ of $A$ the annihilator of $N_p$ is equal to $\mathrm{Ann}(N)_p$ (II, § 2, No. 4, formula (9)), we deduce from Prop. 5 of No. 3 the equality

$$
\mathrm{grade}(N) = \inf_{p \in \mathrm{Spec}(A)} \mathrm{grade}(N_p) = \inf_{m \in \Omega} \mathrm{grade}(N_m),
$$

where $\Omega$ denotes the set of maximal ideals of $A$.

### 6. Depth of Algebras

#### Lemma 2 {#ac-x-s1-lem-2 .statement}

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings, $N$ a finitely generated $B$-module and $y$ an element of $m_B$. The following two conditions are equivalent:

(i) the $A$-module $N/yN$ is flat and the homothety $y_N$ is injective;
(ii) the $A$-module $N$ is flat and the homothety $y_{\kappa_A \otimes N}$ is injective.

When they are satisfied, the homothety $y_{M \otimes_A N}$ is injective for every $A$-module $M$.

Assume that the hypotheses of (i) are satisfied, and let us prove (ii) as well as the last assertion. Let $M$ be an $A$-module. Since the $A$-module $N/yN$ is flat, we deduce from the exact sequence $0 \to N \xrightarrow{y_N} N \to N/yN \to 0$ the exact sequences

$$
0 \to M \otimes_A N \xrightarrow{u} M \otimes_A N \to M \otimes_A (N/yN) \to 0
$$
$$
0 \to \mathrm{Tor}_1^A(M, N) \xrightarrow{v} \mathrm{Tor}_1^A(M, N) \to 0
$$

where $u = 1_M \otimes y_N$ and $v = \mathrm{Tor}_1^A(1_M, y_N)$; it follows that the homothety of ratio $y$ is injective in $M \otimes_A N$, and bijective in $\mathrm{Tor}_1^A(M, N)$. Assume moreover that the A-module $M$ is finitely generated; then the B-module $\mathrm{Tor}_1^A(M, N)$ is finitely generated (A, X, p. 107, Prop. 6), hence is zero since $y$ belongs to $m_B$ (Nakayama's lemma), which implies that the A-module $N$ is flat (A, X, p. 74, Theorem 2).

(ii) $\Rightarrow$ (i): assume that the hypotheses of (ii) are satisfied. Consider the two exact sequences of B-modules

(1)
$$
0 \to \mathrm{Ker}(y_N) \longrightarrow N \xrightarrow{p} \mathrm{Im}(y_N) \to 0
$$

(2)
$$
0 \to \mathrm{Im}(y_N) \xrightarrow{i} N \longrightarrow N/yN \to 0,
$$

where $p$ and $i$ are the canonical homomorphisms. It follows that the homomorphism $1 \otimes p : \kappa_A \otimes_A N \longrightarrow \kappa_A \otimes_A \mathrm{Im}(y_N)$ is surjective, and (since $N$ is flat) that the kernel of the homomorphism $1 \otimes i : \kappa_A \otimes_A \mathrm{Im}(y_N) \longrightarrow \kappa_A \otimes_A N$ is isomorphic to $\mathrm{Tor}_1^A(\kappa_A, N/yN)$. But the mapping $(1 \otimes i) \circ (1 \otimes p)$, equal to $y_{\kappa_A \otimes_A N}$, is injective by hypothesis; it follows that $1 \otimes p$ is bijective and $1 \otimes i$ injective, and consequently that one has $\mathrm{Tor}_1^A(\kappa_A, N/yN) = 0$. It follows that the A-module $N/yN$ is flat (III, § 5, No. 2, Theorem 1 and No. 4, Proposition 2).

Since $N$ and $N/yN$ are flat over $A$, the same is true of $\mathrm{Im}(y_N)$ (exact sequence (2)). One then deduces from exact sequence (1) that $\kappa_A \otimes_A \mathrm{Ker}(y_N)$ is isomorphic to the kernel of $1 \otimes p$, hence is zero; thus the homothety $y_N$ is injective by Nakayama's lemma.

#### Proposition 10 {#ac-x-s1-prop-10 .statement}

*Let $\rho : \Lambda \to B$ be a local homomorphism of noetherian local rings, $N$ a finitely generated B-module and $y = (y_1, \ldots, y_s)$ a sequence of elements of $m_B$. Let $\mathfrak{y}$ denote the ideal of $B$ generated by this sequence. The following conditions are equivalent:

(i) the A-module $N/\mathfrak{y}N$ is flat and the sequence $y$ is N-regular;
(ii) the A-module $N$ is flat and the sequence $y$ is $(\kappa_A \otimes_A N)$-regular.*

When these conditions are satisfied, for every A-module $M$, the sequence $y$ is $M \otimes_A N$-regular.

Let us prove the equivalence of (i) and (ii) by induction on $s$. The case $s = 0$ being evident, suppose $s \geqslant 1$; let $y'$ denote the sequence $(y_1, \ldots, y_{s-1})$ and $\mathfrak{y}'$ the ideal of $B$ generated by it. By lemma 2 applied to the B-module $N/\mathfrak{y}'N$ and to the element $y_s$ of $B$, condition (i) is equivalent to

(i') the A-module $N/\mathfrak{y}'N$ is flat, the sequence $y'$ is N-regular, and the homothety of ratio $y_s$ in $\kappa_A \otimes_A (N/\mathfrak{y}'N) = (\kappa_A \otimes_A N)/\mathfrak{y}'(\kappa_A \otimes_A N)$ is injective.

This condition is equivalent to (ii) by the induction hypothesis.

The last assertion follows likewise by induction on $s$ from the last assertion of lemma 2.

#### Proposition 11 {#ac-x-s1-prop-11 .statement}

*Let $\rho : \Lambda \to B$ be a local homomorphism of noetherian local rings, $M$ a finitely generated A-module and $N$ a finitely generated B-module; suppose that the A-module $N$ is flat.*

a) Let $(x_1, \ldots, x_r)$ be a sequence of elements of $m_A$ which is regular for the A-module $M$, and $(y_1, \ldots, y_s)$ a sequence of elements of $m_B$ which is regular for the B-module $\kappa_A \otimes_A N$; then the sequence $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ of elements of $m_B$ is regular for the B-module $M \otimes_A N$.

b) One has the equality

$$
\operatorname{prof}_B(M \otimes_A N) = \operatorname{prof}_A(M) + \operatorname{prof}_B(\kappa_A \otimes_A N)
$$

Let $x$ denote the ideal of A generated by the sequence $x$ and $y$ the ideal of B generated by $y$. By Prop. 10, the sequence $y$ is $M \otimes_A N$-regular and $N/yN$ is flat over A, so that the sequence $\rho(x) = (\rho(x_1), \ldots, \rho(x_r))$ is regular for $M \otimes_A (N/yN) = (M \otimes_A N)/y(M \otimes_A N)$. This proves a).

To prove b), we may suppose that M and N are nonzero. By Nakayama's lemma, $\kappa_A \otimes_A N$ is likewise nonzero, so that $\operatorname{prof}_A(M)$ and $\operatorname{prof}_B(\kappa_A \otimes_A N)$ are finite (No. 4, Cor. 2 of Th. 2). Take maximal regular sequences $x$ and $y$; then one has $r = \operatorname{prof}_A(M)$, $s = \operatorname{prof}_B(\kappa_A \otimes_A N)$, and there exists an injective a-linear mapping $u : \kappa_A \to M/xM$ and an injective b-linear mapping $v : \kappa_B \to \kappa_A \otimes_A (N/yN)$ (No. 4, Cor. 1 of Th. 2). Since $N/yN$ is flat over A, the b-linear mapping $(u \otimes 1_{N/yN}) \circ v$ of $\kappa_B$ into $(M/xM) \otimes_A (N/yN) = (M \otimes_A N)/(\rho(x) + y)(M \otimes_A N)$ is injective. This implies the equality $\operatorname{prof}_B(M \otimes_A N) = r + s$ (*loc. cit.*).

#### Remark {#ac-x-s1-n6-rem-1 .statement}

Recall that, under the preceding assumptions,

$$
\dim_B(M \otimes_A N) = \dim_A(M) + \dim_B(\kappa_A \otimes_A N)
$$
(VIII, § 3, No. 4, Prop. 7).

#### Corollary {#ac-x-s1-n6-cor-1 .statement}

Let $\rho : A \to B$ be a local homomorphism of noetherian local rings making B a flat A-module. One has

$$
\operatorname{prof}(B) = \operatorname{prof}(A) + \operatorname{prof}(\kappa_A \otimes_A B),
$$
$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

In fact the depth (resp. the dimension) of the B-module $\kappa_A \otimes_A B$ is equal to the depth (resp. the dimension) of the ring $\kappa_A \otimes_A B$ by the cor. of Prop. 4 (resp. by VIII, § 1, No. 4).

### 7. Upper Bounds for Depth

#### Proposition 12 {#ac-x-s1-prop-12 .statement}

Let A be a noetherian local ring, M a nonzero finitely generated A-module and J an ideal of A distinct from A. One has the sequence of inequalities

$$
\operatorname{prof}_A(J; M) \leq \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/JM)
$$
$$
\leq [J/m_A J : \kappa_A].
$$

For every element $p$ of $\operatorname{Supp}(M) \cap V(J)$, $\operatorname{prof}_A(J; M)$ is less than or equal to $\dim_{A_p}(M_p)$ (No. 5, Prop. 8 and No. 4, Cor. 2 of Th. 2), that is to say (VIII, § 1, No. 4, Prop. 9)

#### Remark 1 {#ac-x-s1-n7-rem-1 .statement}

Consider the chain of inequalities of Prop. 12.

a) In order that one have prof_A(J ; M) = [J/m_AJ : κ_A], it is necessary and sufficient that J can be generated by an M-regular sequence (No. 3, Cor. 2 of Th. 1 and A, X, p. 160, Cor. 1).

b) The equality dim(M) − dim(M/JM) = [J/m_AJ : κ_A] means that J can be generated by a secant sequence for M (VIII, § 3, No. 2).

c) *If M is Macaulay, one has prof_A(J ; M) = dim(M) − dim(M/JM) (§ 2, No. 2, cor. of Prop. 2).*

#### Lemma 3 {#ac-x-s1-lem-3 .statement}

Let A be a noetherian ring, p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q a saturated chain of length r of prime ideals of A, M a finitely generated Λ-module and n an integer. If the A-module Ext^n_{A_p}(κ(p), M_p) is nonzero, the same is true of Ext^{n+r}_{A_q}(κ(q), M_q).

It is obviously enough to treat the case r = 1; then, replacing A, M, p and q by A_q, M_q, pA_q and qA_q respectively, one is reduced to treating the case where A is local and q = m_A. Let x be an element of m_A − p. The A_p-module Ext^n_A(A/p, M) ⊗_A A_p is isomorphic to Ext^n_{A_p}(κ(p), M_p) (A, X, p. 111, Prop. 10 b)), and is therefore nonzero by assumption; a fortiori Ext^n_A(A/p, M) is nonzero. The exact sequence

$$
0 \to A/p \xrightarrow{x_{A/p}} A/p \to A/(p + xA) \to 0
$$

yields an exact sequence of extension modules

$$
\text{Ext}^n_A(A/p, M) \xrightarrow{u} \text{Ext}^n_A(A/p, M) \to \text{Ext}^{n+1}_A(A/(p + xA), M),
$$

where u is the homothety with ratio x. By Nakayama's lemma, this is not surjective, hence the A-module Ext^{n+1}_A(A/(p + xA), M) is nonzero. But the only prime ideal of A containing p + xA is m_A, so the A-module A/(p + xA) is of finite length (VIII, § 3, No. 2, Lemma 2). If Ext^{n+1}_A(κ_A, M) were zero, one would deduce from this, by induction on the length of N, that Ext^{n+1}_A(N, M) = 0 for every A-module N of finite length. This contradiction completes the proof.

#### Proposition 13 {#ac-x-s1-prop-13 .statement}

Let A be a noetherian ring, M a finitely generated A-module, p and q two prime ideals of Supp(M) with p ⊂ q. One has

$$
\text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + \dim(A_q/pA_q).
$$

More precisely, for every saturated chain of prime ideals p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q, one has \text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + r.

Put p = \text{prof}_{A_p}(M_p), and let us prove the second inequality. It is obvious if p = +∞; in the contrary case one has \text{Ext}^p_{A_p}(κ(p), M_p) ≠ 0, whence

$Ext_{A_q}^{p+r}(\kappa(q), M_q) \neq 0$ by lemma 3, which implies $prof_{A_q}(M_q) \leq p + r$. Since $\dim(A_q/pA_q)$ is the least upper bound of the lengths of saturated chains of prime ideals with endpoints $p$ and $q$, the first assertion is a consequence of the second.

#### Corollary 1 {#ac-x-s1-prop-13-cor-1 .statement}

*One has the inequality*

$$
\dim(M_q) - prof_{A_q}(M_q) \geq \dim(M_p) - prof_{A_p}(M_p) \geq 0 .
$$

This follows from prop. 13 and the inequality $\dim(M_q) \geq \dim(M_p) + \dim(A_q/pA_q)$ (VIII, § 1, No. 4, prop. 9, a) and No. 3, prop. 7, b)).

#### Corollary 2 {#ac-x-s1-prop-13-cor-2 .statement}

*Let A be a local noetherian ring and M a finitely generated A-module. One has the inequality*

$$
prof_A(M) \leq \inf_{p \in \operatorname{Ass}(M)} \dim(A/p) .
$$

Let $p$ be a prime ideal associated with $M$; one has $prof_{A_p}(M_p) = 0$ (No. 1, remark 2). Prop. 13 applied to the ideals $p \subset m_A$ yields the inequality $prof_A(M) \leq \dim(A/p)$, whence the corollary.

#### Remark 2 {#ac-x-s1-n7-rem-2 .statement}

One has $\sup_{p \in \operatorname{Ass}(M)} \dim(A/p) = \dim(M)$ (VIII, § 1, No. 4, remark 2), and one recovers the inequality $prof(M) \leq \dim(M)$ for $M \neq 0$ (No. 4, cor. 2 of th. 2).

### 8. Locally Integral Noetherian Rings; Normal Noetherian Rings

Let $A$ be a noetherian ring. Denote by $(Y_i)_{i \in I}$ the finite family (II, § 4, No. 2, prop. 10 and No. 3, cor. 7 of prop. 11) of connected components of $\operatorname{Spec}(A)$. By II, § 4, No. 3, prop. 15, for each $i$ there exists a unique idempotent element $e_i$ of $A$ such that $Y_i = V(e_i)$, and the canonical mapping of $A$ into the product of the rings $A/Ae_i$ is bijective. The quotient rings $A/Ae_i$ of $A$ are called the *canonical components* of $A$. Put $f_i = 1 - e_i$. One has $\sum_{i \in I} f_i = 1$, and $(f_i)_{i \in I}$ is an orthogonal family of non-zero idempotents of $A$ (*loc. cit.*). It follows that the image of $f_i$ in $A/Ae_j$ is equal to 1 if $j = i$ and to 0 if $j \neq i$; one therefore deduces from the ring homomorphism $A \to \prod_j A/Ae_j$ a canonical isomorphism $A_{f_i} \to A/Ae_i$.

By *loc. cit.*, cor. 2 of prop. 14, the following conditions are equivalent:
(i) the connected components of $\operatorname{Spec}(A)$ are irreducible;
(ii) every prime (resp. maximal) ideal of $A$ belong to only one irreducible component of $\operatorname{Spec}(A)$;
(iii) every prime (resp. maximal) ideal of $A$ contains only one minimal prime ideal;
(iv) for every prime (resp. maximal) ideal $p$ of $A$, the topological space $\operatorname{Spec}(A_p)$ is irreducible;
(v) for every canonical component $C$ of $A$, the topological space $\operatorname{Spec}(C)$ is irreducible.

(i) $A$ is reduced and the connected components of $\mathrm{Spec}(A)$ are irreducible;
(ii) for every prime (resp. maximal) ideal $p$ of $A$, the ring $A_p$ is an integral domain;
(iii) the canonical components of $A$ are integral domains.

A noetherian ring is said to be *locally integral* if it satisfies the equivalent conditions (i) to (iii) above.

Suppose the ring $A$ locally integral; let $u$ be an isomorphism of $A$ onto a (finite) product $\prod_{j \in J} A_j$ of integral domains. There exists a bijection $\sigma : J \to I$ such that the mapping of $\mathrm{Spec}(\prod_{j \in J} A_j)$ into $\mathrm{Spec}(A)$ associated with $u$ defines a homeomorphism of $\mathrm{Spec}(A_j)$ onto the connected component $Y_{\sigma(j)}$ of $\mathrm{Spec}(A)$; one then deduces from $u$ an isomorphism of the canonical component $A/Ae_{\sigma(j)}$ onto $A_j$.

#### Proposition 14 {#ac-x-s1-prop-14 .statement}

*Let $A$ be a noetherian ring. The following conditions are equivalent:*

(i) $A$ is reduced and integrally closed in its total ring of fractions ;
(ii) $A$ is isomorphic to the product of a finite family of integrally closed rings ;
(iii) *the canonical components of $A$ are integrally closed* ;
(iv) *for every prime ideal (resp. maximal ideal) $p$ of $A$, the ring $A_p$ is integrally closed*.

The equivalence of (i) and (ii) follows from V, § 1, No. 2, Cor. 2 of Prop. 9, and that of (ii) and (iii) from the remarks preceding the proposition. Let $p$ be a prime ideal of $A$; there exists a unique canonical component $A'$ of $A$ such that $p$ belongs to the closed subset $\mathrm{Spec}(A')$ of $\mathrm{Spec}(A)$, and one has a canonical isomorphism $A_p \to A'_pA'$. The equivalence of (iii) and (iv) therefore follows from *loc. cit.*, No. 5, Cor. 1 and Cor. 3 of Prop. 16.

A ring $A$ is said to be *normal* if it is noetherian and satisfies the equivalent conditions (i) to (iv) of Proposition 14. A noetherian ring is integrally closed if and only if it is integral and normal. A normal local ring is integrally closed.

### 9. Depth and Connectedness

#### Lemma 4 {#ac-x-s1-lem-4 .statement}

*Let $A$ be a noetherian ring, $F$ a closed subset of $\mathrm{Spec}(A)$, $U$ the complementary open set, and $u : M \to N$ a homomorphism of finitely generated $A$-modules.*

a) *Suppose that $u_p : M_p \to N_p$ is injective for every $p \in U$ and that one has $\mathrm{prof}_F(M) \geqslant 1$. Then $u$ is injective.*

b) Suppose that $u_p : M_p \to N_p$ is bijective for every $p \in U$ and that one has $\mathrm{prof}_F(M) \geqslant 2$ and $\mathrm{prof}_F(N) \geqslant 1$. Then $u$ is bijective.

a) The hypotheses imply $\mathrm{Supp}(\mathrm{Ker}\,u) \subset F$, hence $\mathrm{Hom}_\Lambda(\mathrm{Ker}\,u, M) = 0$ (No. 5, Remark 1); therefore one has $\mathrm{Ker}\,u = 0$.

b) One already knows that $u$ is injective, and one has $\mathrm{Supp}(\mathrm{Coker}\,u) \subset F$. By loc. cit., one has $\mathrm{Hom}_A(\mathrm{Coker}\,u, N) = 0$ and $\mathrm{Ext}_A^1(\mathrm{Coker}\,u, M) = 0$. From the exact sequence of extension modules

$$
\mathrm{Hom}_A(\mathrm{Coker}\,u, N) \to \mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) \to \mathrm{Ext}_A^1(\mathrm{Coker}\,u, M)
$$

one deduces $\mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) = 0$, which implies $\mathrm{Coker}\,u = 0$.

#### Remark 1 {#ac-x-s1-n9-rem-1 .statement}

Let $A$ be a noetherian ring, $F$ a closed subset of $\mathrm{Spec}(A)$, $U$ the complementary open set. In order that $\mathrm{prof}_F(A) \geqslant 1$, it is necessary and sufficient that $\mathrm{Ass}(A) \subset U$ (remark 2, No. 5). When this condition is satisfied, each irreducible component of $\mathrm{Spec}(A)$ meets $U$, so that $U$ is dense in $\mathrm{Spec}(A)$.

#### Theorem 3 (Hartshorne) {#ac-x-s1-thm-3 .statement}

Let $A$ be a noetherian ring, $F$ a closed subset of $\mathrm{Spec}(A)$ and $U$ the complementary open set. Suppose that $\mathrm{prof}_F(A) \geqslant 2$. Then, for every connected component $Y$ of $\mathrm{Spec}(A)$, the set $Y \cap \overline{U}$ is connected and dense in $Y$.

Suppose first that $\mathrm{Spec}(A)$ is connected. By remark 1, $U$ is dense in $\mathrm{Spec}(A)$, and it remains to prove that it is connected. Reasoning by contradiction, suppose that there are given two disjoint open sets $U_0$ and $U_1$ of $\mathrm{Spec}(A)$, non-empty and with union $U$. Since the set $\mathrm{Ass}(\Lambda)$ is contained in $U$ by remark 1, it is the disjoint union of $\mathrm{Ass}(A) \cap U_0$ and $\mathrm{Ass}(A) \cap U_1$. By IV, § 1, No. 1, Prop. 4, there exist ideals $J_0$ and $J_1$ of $A$ such that $\mathrm{Ass}(J_i) = \mathrm{Ass}(A) \cap U_i$, $\mathrm{Ass}(A/J_i) = \mathrm{Ass}(A) \cap U_{1-i} \quad (i = 0, 1)$. The complement of $U_i$ in $\mathrm{Spec}(A)$ contains $\mathrm{Ass}(A/J_i)$ and $\mathrm{Ass}(J_{1-i})$; since it is closed, it contains $\mathrm{Supp}(A/J_i)$ and $\mathrm{Supp}(J_{1-i})$. For $p \in U_i$, one has thus $(J_i)_p = A_p$ and $(J_{1-i})_p = 0$; this implies in particular that $J_0$ and $J_1$ are distinct from $A$. Let $B$ be the $A$-module $A/J_0 \times A/J_1$ and let $u : A \to B$ be the canonical homomorphism. By what precedes, the homomorphism $u_p$ is bijective for every $p \in U$; moreover, one has $\mathrm{Ass}(B) \subset U_0 \cup U_1 = U$, hence $\mathrm{prof}_F(B) \geqslant 1$ by remark 1. Lemma 4 then implies that $u$ is bijective, which contradicts the connectedness of $\mathrm{Spec}(A)$.

Let us treat the general case. Let $J$ be an ideal of $A$ such that $F = V(J)$ and let $Y$ be a connected component of $\mathrm{Spec}(A)$. By II, § 4, No. 3, Prop. 15, there exists an idempotent element $f$ of $\Lambda$ such that $Y$ is identified with the subset $\mathrm{Spec}(A_f)$ of $\mathrm{Spec}(A)$. Then $Y \cap F$ is identified with $V(J_f)$; one has $\mathrm{prof}_{\Lambda_f}(J_f, A_f) \geqslant \mathrm{prof}_A(J; A) \geqslant 2$ by Prop. 6, a) of No. 3. It follows from the first part of the proof that $Y \cap U = Y - (Y \cap F)$ is connected and dense in $Y$.

#### Corollary 1 {#ac-x-s1-thm-3-cor-1 .statement}

The mapping which associates to each connected component of $U$ its closure in $\mathrm{Spec}(A)$ is a bijection of the set of connected components of $U$ onto the set of connected components of $\mathrm{Spec}(A)$.

#### Corollary 2 {#ac-x-s1-thm-3-cor-2 .statement}

For every noetherian local ring B of depth $\geq 2$, the topological space $\operatorname{Spec}(B) - \{ m_B \}$ is connected.

#### Corollary 3 {#ac-x-s1-thm-3-cor-3 .statement}

Under the hypotheses of Theorem 3, suppose that $\operatorname{Spec}(A_p)$ is irreducible (resp. that $A_p$ is an integral domain) for every $p \in U$; then $\operatorname{Spec}(A_p)$ is irreducible (resp. $A_p$ is an integral domain) for every $p \in \operatorname{Spec}(A)$.

Let $(Y_i)_{i \in I}$ be the (finite) family of irreducible components of $\operatorname{Spec}(A)$. Let $p \in U$; since $\operatorname{Spec}(\Lambda_p)$ is irreducible, $p$ contains only one minimal prime ideal of $\Lambda$, and therefore belongs to only one of the $Y_i$ (II, § 4, No. 3, Cor. 2 of Prop. 14). The subsets $Y_i \cap U$ are closed subsets of $U$, pairwise disjoint, non-empty since $U$ is dense in $\operatorname{Spec}(A)$, and irreducible by II, § 4, No. 1, Prop. 7; they are therefore the connected components of $U$. Their closures $Y_i$ are the connected components of $\operatorname{Spec}(\Lambda)$ (Cor. 1). This proves that the connected components of $\operatorname{Spec}(A)$ are irreducible, and therefore that $\operatorname{Spec}(A_p)$ is irreducible for every $p$ (No. 8).

Suppose that $A_q$ is an integral domain for every $q \in U$. Let $p \in \operatorname{Spec}(A)$. Since $\operatorname{Spec}(A_p)$ is irreducible, the nilradical of $A_p$ is the unique minimal prime ideal of $A_p$; it therefore belongs to $\operatorname{Ass}(A_p)$ (IV, § 1, No. 3, Cor. 1 of Prop. 7), and consequently is equal to $qA_p$, where $q$ is a prime ideal associated with $A$ (IV, § 1, No. 2, Cor. of Prop. 5). One has $q \in U$ (Remark 1) and $qA_q \in \operatorname{Ass}(A_q)$ (loc. cit.); since $A_q$ is an integral domain, $q$ is zero, and therefore $A_p$ is an integral domain.

#### Corollary 4 {#ac-x-s1-thm-3-cor-4 .statement}

Let $\Lambda$ be a noetherian ring whose spectrum is connected. Suppose there exists an integer $d \geq 1$ such that one has $\operatorname{prof}(\Lambda_p) \geq 2$ for every prime ideal $p$ of $A$ of height $> d$.

a) For every closed subset $Z$ of $\operatorname{Spec}(A)$ of codimension $> d$, the space $\operatorname{Spec}(A) - Z$ is connected.

b) Let $Y$ and $Y'$ be irreducible components of $\operatorname{Spec}(A)$. There exists a sequence $X_1, X_2, \ldots, X_n$ of irreducible components of $\operatorname{Spec}(A)$ such that one has $X_1 = Y$, $X_n = Y'$ and, for $i = 1, \ldots, n-1$

$$
\operatorname{codim}(X_i \cap X_{i+1}, \operatorname{Spec}(A)) \leq d .
$$

Let $Z \subset \operatorname{Spec}(A)$ be a closed subset of codimension $> d$. For every $p \in Z$, one has $\dim(A_p) > d$, hence $\operatorname{prof}(A_p) \geq 2$, which implies that $\operatorname{prof}_Z(A)$ is $\geq 2$ (No. 5, Prop. 8) and therefore that $\operatorname{Spec}(A) - Z$ is connected (Theorem 3).

Let us prove b). Denote by $Z$ the union of the sets $X' \cap X''$ where $(X', X'')$ runs through the (finite) set of pairs of irreducible components of $\operatorname{Spec}(A)$ such that $\operatorname{codim}(X' \cap X'', \operatorname{Spec}(A)) > d$. By a), the set $\operatorname{Spec}(A) - Z$ is connected. All the irreducible components of $\operatorname{Spec}(A)$ meet $\operatorname{Spec}(A) - Z$; their traces on $\operatorname{Spec}(A) - Z$ are the irreducible components of $\operatorname{Spec}(A) - Z$ (II, § 4, No. 1, Prop. 7). Since $\operatorname{Spec}(A) - Z$ is connected, there exists a sequence $X_1, \ldots, X_n$ of irreducible components of $\operatorname{Spec}(A)$ such that one has $X_1 - Z = Y - Z$, $X_n - Z = Y' - Z$ and $(X_i - Z) \cap (X_{i+1} - Z) \neq \varnothing$ for $1 \leq i \leq n-1$; in other words one has $X_1 = Y$, $X_n = Z$ and $\operatorname{codim}(X_i \cap X_{i+1}) \leq d$.

#### Remark 2 {#ac-x-s1-n9-rem-2 .statement}

*When A is a Macaulay ring, one can apply corollary with $d = 1$ (§ 2, No. 5).*

#### Example (Complete intersection formed by four coordinate planes of an affine space of dimension 4) {#ac-x-s1-n9-exa-1 .statement}

Let $k$ be a field. Let S denote the polynomial ring $k[T_1, T_2, T_3, T_4]$. Recall (VIII, § 2, No. 4, Theorem 3) that every maximal chain of prime ideals of S is of length 4. Let m denote the ideal of S generated by the $T_i$, a the ideal generated by $T_1T_2$ and $T_3T_4$, and $p_{ij}$, for $1 \leq i < j \leq 4$, the ideal generated by $T_i$ and $T_j$. The ideals $p_{ij}$ are prime of height 2, their sum is the maximal ideal m, and one has $a = p_{13} \cap p_{14} \cap p_{23} \cap p_{24}$.

a) The ring $A = S/a$ is reduced; the irreducible components of Spec(A) are the sets $X_{ij} = V(p_{ij}/a)$ for $i = 1,2,\ j = 3,4$, which are of dimension 2 and all contain the point $m/a$. In particular, Spec(A) is connected and of dimension 2. The intersection of two distinct components $X_{ij}$ and $X_{kl}$ is reduced to $\{m/a\}$ if $\{i,j\} \cap \{k,l\} = \varnothing$, of dimension 1 otherwise. It follows that the conclusion of cor. 4 is satisfied with $d = 1$ (we shall see later that A is a Macaulay ring, so that the assumption of corollary 4 is itself satisfied for $d = 1$).

b) Let b denote the ideal of S generated by $T_1T_2$, $T_1T_3$, $T_2T_4$, $T_3T_4$, and B the ring $S/b$. One has $b = p_{14}p_{23} = p_{14} \cap p_{23}$. The ring B is reduced. Its spectrum is identified with the closed subset $X_{14} \cup X_{23}$ of Spec(A); it has two irreducible components (of dimension 2) whose intersection is reduced to a point. The depth of B along this point is strictly positive because B is reduced, and less than 1 by Theorem 3, hence equal to 1.* Thus B is not a Macaulay ring. \*

### 10. Depth and normality

Let A be a noetherian ring and $p$ a prime ideal of A. One has $\mathrm{prof}(A_p) \leq \mathrm{ht}(p)$ (No. 4, cor. 2 of Theorem 2). If moreover A is reduced, the local ring $A_p$ is reduced (II, § 2, No. 6, prop. 17), whence:

a) if $\mathrm{ht}(p) = 0$, $A_p$ is a field;
b) if $\mathrm{ht}(p) \geq 1$, one has $\mathrm{prof}(A_p) \geq 1$ (No. 1, remark 3).

Conversely:

#### Proposition 15 {#ac-x-s1-prop-15 .statement}

Let A be a noetherian ring satisfying the following two conditions:
(i) for every minimal prime ideal $p$ of $\Lambda$, the ring $\Lambda_p$ is reduced;
(ii) for every prime ideal $p$ of A of height $\geq 1$, one has $\mathrm{prof}(A_p) \geq 1$.
Then A is reduced.

Let $n$ denote the nilradical of A. For every minimal prime ideal $p$ of A, one has by (i) $n_p = 0$, that is, $p \not\in \mathrm{Supp}(n)$ and $a fortiori$ $p \not\in \mathrm{Ass}_A(n)$. For every $p \in \mathrm{Spec}(A)$ of height $\geq 1$, one has by (ii) $pA_p \not\in \mathrm{Ass}_{A_p}(A_p)$ and $a fortiori$ $pA_p \not\in \mathrm{Ass}_{A_p}(n_p)$, whence $p \not\in \mathrm{Ass}_A(n)$ (IV, § 1, No. 2, prop. 5). Thus the set $\mathrm{Ass}_A(n)$ is empty, which implies that $n$ is zero.

#### Proposition 16 {#ac-x-s1-prop-16 .statement}

Let $A$ be an integrally closed noetherian ring, $J$ an ideal of $A$ of height $\geqslant 2$, and $M$ a reflexive $A$-module of finite type. One has $\operatorname{prof}_A(J; M) \geqslant 2$.

Let us choose a finite-dimensional vector space $V$ over the field of fractions of $A$ and a lattice $N$ in $V$ isomorphic to $M$ (VII, § 4, No. 2, Remark 1). The prime ideals associated with $V/N$, being of height 1 (*loc. cit.*, Theorem 2), do not contain $J$; after Remark 2 of No. 1, this implies $\operatorname{prof}_A(J; V/N) \geqslant 1$. On the other hand, the $A$-module $V$ is divisible and torsion-free, hence injective (A, X, p. 17, Corollary 2 of Proposition 10), which implies $\operatorname{prof}_A(J; V) = +\infty$. The inequality $\operatorname{prof}_A(J; N) \geqslant 2$ then follows from Proposition 1 of No. 1.

#### Corollary {#ac-x-s1-n10-cor-1 .statement}

*A noetherian local integrally closed ring of dimension $\geqslant 2$ has depth $\geqslant 2$*.

Let $A$ be a normal ring (No. 8) and $\mathfrak{p}$ a prime ideal of $A$. Then:
a) if $\operatorname{ht}(\mathfrak{p}) = 0$, $A_{\mathfrak{p}}$ is a field;
b) if $\operatorname{ht}(\mathfrak{p}) = 1$, $A_{\mathfrak{p}}$ is a discrete valuation ring (VII, § 1, No. 7, Proposition 11);
c) if $\operatorname{ht}(\mathfrak{p}) \geqslant 2$, one has $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$ (corollary to Proposition 16).

Conversely:

#### Theorem 4 (Serre) {#ac-x-s1-thm-4 .statement}

*Let $A$ be a noetherian ring satisfying the following conditions*:
(i) *for every minimal prime ideal $\mathfrak{p}$ of $A$, the ring $A_{\mathfrak{p}}$ is reduced*;
(ii) *for every prime ideal $\mathfrak{p}$ of $A$ of height 1, the ring $A_{\mathfrak{p}}$ is integrally closed*;
(iii) *for every prime ideal $\mathfrak{p}$ of $A$ of height $\geqslant 2$, one has $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$*.

*Then $A$ is normal*.

It is a question of proving that the ring $A_{\mathfrak{p}}$ is integrally closed for every $\mathfrak{p} \in \operatorname{Spec}(A)$, which we shall do by induction on $\operatorname{ht}(\mathfrak{p})$. For $\operatorname{ht}(\mathfrak{p}) \leqslant 1$ this follows from assumptions (i) and (ii). Suppose therefore that one has $\operatorname{ht}(\mathfrak{p}) \geqslant 2$ and that $A_q$ is integrally closed for every prime ideal $q$ of $A$ of height $< \operatorname{ht}(\mathfrak{p})$. By assumption (iii), one has $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$. By the induction hypothesis and cor. 3 of th. 3 of No. 9, applied to the ring $A_{\mathfrak{p}}$ and to the closed subset $\{\mathfrak{p}A_{\mathfrak{p}}\}$ of $\operatorname{Spec}(A_{\mathfrak{p}})$, the ring $A_{\mathfrak{p}}$ is an integral domain. Let $K$ be its field of fractions and let $B$ be a subring of $K$, containing $A_{\mathfrak{p}}$ and finite over $A_{\mathfrak{p}}$. It is a question of proving that $B$ is equal to $A_{\mathfrak{p}}$. Let us denote by $i$ the canonical injection of $A_{\mathfrak{p}}$ into $B$. Since $B$ is contained in $K$, it is a torsion-free $A_{\mathfrak{p}}$-module, hence of depth $\geqslant 1$. Moreover, for every prime ideal $q$ of $A_{\mathfrak{p}}$ distinct from $\mathfrak{p}A_{\mathfrak{p}}$, the homomorphism $i_q : (A_{\mathfrak{p}})_q \to B_q$ is bijective since $A_q$ is integrally closed. By lemma 4 of No. 9, applied to the closed subset $F = \{\mathfrak{p}A_{\mathfrak{p}}\}$ of $\operatorname{Spec}(A_{\mathfrak{p}})$, the homomorphism $i$ is bijective, which completes the proof of the theorem.

#### Remark 1 {#ac-x-s1-n10-rem-1 .statement}

A convenient form of th. 4 is the following: let $A$ be a noetherian ring, such that for every prime ideal $p$ of $A$ the ring $A_p$ is integrally closed or of depth $\geqslant 2$; then $A$ is normal. Let us indeed verify the assumptions of th. 4. Let $p \in \mathrm{Spec}(A)$. If $\mathrm{ht}(p) \leqslant 1$, then one has $\mathrm{prof}(A_p) \leqslant 1$, hence $A_p$ is integrally closed. If $\mathrm{ht}(p) \geqslant 2$, the ring $A_p$ is either of depth $\geqslant 2$, or integrally closed, which again implies $\mathrm{prof}(A_p) \geqslant 2$ (No. 1, cor. 2 of prop. 1), whence the desired conclusion. One verifies analogously the following statement: let $A$ be a noetherian ring such that for every prime ideal $p$ of $A$, the ring $A_p$ is reduced or of depth $\geqslant 1$; then $A$ is reduced.

#### Corollary 1 {#ac-x-s1-thm-4-cor-1 .statement}

*Let $\Lambda$ be a noetherian ring, $F$ a closed subset of $\mathrm{Spec}(A)$, $U$ the complementary open set. Suppose that $\mathrm{prof}_F(A)$ is $\geqslant 2$ (resp. $\geqslant 1$) and that, for every $p \in U$, the ring $A_p$ is integrally closed (resp. reduced). Then $A$ is normal* (resp. reduced).

For every $p \in F$, one has $\mathrm{prof}(A_p) \geqslant \mathrm{prof}_F(A)$ (No. 5, Prop. 8); it is therefore enough to apply the preceding remark.

#### Corollary 2 {#ac-x-s1-thm-4-cor-2 .statement}

*Let $\rho : A \to B$ be a homomorphism of noetherian rings making $B$ into a flat $A$-module.

a) *If $B$ is normal and faithfully flat over $A$, $A$ is normal.*

b) *Suppose that $A$ is normal and that the ring $\kappa(p) \otimes_A B$ is normal when $p$ is a minimal prime ideal of $A$, and reduced when $p$ is a prime ideal of height 1. Then the ring $B$ is normal.*

a) Suppose $B$ normal and faithfully flat over $A$. Then $\rho$ is injective (I, § 3, No. 5, Prop. 9) and $B$ is reduced, hence $A$ is reduced. Let $S$ be the set of non-zero-divisors of $A$. Since $B$ is flat over $A$, $\rho(S)$ consists of non-zero-divisors in $B$, so that $B$ is integrally closed in $\rho(S)^{-1}B$. Let $x$ be an element of $S^{-1}A$ integral over $A$; then the element $x \otimes 1_B$ of the ring $S^{-1}A \otimes_A B$ (which is identified with $\rho(S)^{-1}B$) is integral over $B$, hence belong to $B$. Since $B$ is faithfully flat over $A$, one has $x \in A$ (I, § 3, No. 5, Prop. 10, (ii)), and $A$ is normal.

b) Under the hypotheses of b), it is enough, by Remark 1, to prove that for every prime ideal $q$ of $B$, the local ring $B_q$ is normal or of depth $\geqslant 2$. Let $p$ denote the prime ideal $\rho^{-1}(q)$ of $A$; the local homomorphism $A_p \to B_q$ deduced from $\rho$ makes $B_q$ into a faithfully flat $A_p$-module (I, § 3, No. 5, Prop. 9). Let us distinguish four cases :

1) $\mathrm{ht}(p) = 0$. Then $A_p$ is a field, equal to $\kappa(p)$; the ring $A_p \otimes_A B$ is normal by assumption. The same is true of $B_q$, which is a ring of fractions thereof.

#### Remark 2 {#ac-x-s1-n10-rem-2 .statement}

$\mathrm{ht}(p) = 1$ and $\mathrm{ht}(q) \leqslant 1$. Then $A_p$ is a discrete valuation ring; let $\pi$ be a uniformizing element of $A_p$. Since $B_q$ is faithfully flat over $A_p$, the element $\pi 1_{B_q}$ of $B_q$ is not a zero divisor, so that the local ring $B_q/\pi B_q$ is of dimension 0 (VIII, § 3, No. 1, Cor. 2 of Prop. 1). It is reduced, since it is a ring of fractions of the reduced ring $\kappa(p) \otimes_A B$, and consequently it is a field. Therefore $B_q$ is a discrete valuation ring (VI, § 1, No. 4, Prop. 2), hence integrally closed.

#### Remark 3 {#ac-x-s1-n10-rem-3 .statement}

$\mathrm{ht}(p) = 1$ and $\mathrm{ht}(q) \geq 2$. Then, by the relation
$$
\dim(B_q) = \dim(A_p) + \dim(\kappa(p) \otimes_A B_q)
$$
(VIII, § 3, No. 4, Cor. 1 of Prop. 7), the ring $\kappa(p) \otimes_A B_q$ is of dimension $\geq 1$. It is reduced by assumption, hence of depth $\geq 1$ (No. 1, Remark 3). We then have (No. 6, Cor. of Prop. 11)
$$
\mathrm{prof}(B_q) = \mathrm{prof}(A_p) + \mathrm{prof}(\kappa(p) \otimes_A B_q) \geq 1 + 1 = 2 .
$$

#### Remark 4 {#ac-x-s1-n10-rem-4 .statement}

$\mathrm{ht}(p) \geq 2$. Since $A_p$ is of depth $\geq 2$ (Cor. of Prop. 16), the same is true of $B_q$ by *loc. cit*.

#### Corollary 3 {#ac-x-s1-thm-4-cor-3 .statement}

*Let $\rho : A \to B$ be a homomorphism of noetherian rings. Assume that $B$ is a flat $A$-module, that $A$ is normal, and that $\kappa(p) \otimes_A B$ is normal for every $p \in \mathrm{Spec}(A)$. Then $B$ is normal.*

## EXERCISES {#ac-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
