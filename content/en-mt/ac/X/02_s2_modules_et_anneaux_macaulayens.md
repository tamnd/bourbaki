---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 2
section_title: Modules et anneaux macaulayens
lang: en
source: ac-x-fr
book_pages: AC X.154-AC X.157
pdf_pages: 0022-0035, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: Modules macaulayens
      page: 0
      pdf_page: 22
    - "no": 2
      title: Support d’un module macaulayen
      page: 24
      pdf_page: 23
    - "no": 3
      title: Modules macaulayens sur un anneau local
      page: 26
      pdf_page: 25
    - "no": 4
      title: Parties fortement sécantes et quotients d’un module macaulayen
      page: 28
      pdf_page: 27
    - "no": 5
      title: Anneaux de Macaulay
      page: 30
      pdf_page: 29
    - "no": 6
      title: Modules macaulayens et algèbres finies
      page: 32
      pdf_page: 31
    - "no": 7
      title: Modules macaulayens et algèbres plates
      page: 0
      pdf_page: 33
statements: 46
exercises: 11
content_sha256: a8db826b7ca09881d463dde0cdd85fdb21ded4664105d9fcd21f4d357498696b
translated_from: content/fr/ac/X/02_s2_modules_et_anneaux_macaulayens.md
source_lang: fr
translation_method: machine
source_content_sha256: 650bbfdcc8ed4e299912939fbb5d1419edd5bfe730a6cdaaf497218c5852c4b7
translation_model: gpt-5.4
translation_run: translate-en-mt-be1034d2
glossary_version: 34
glossary_terms_sha256: 53d92b366659f9348e2438fca012927b54c6ef8ec217b048155cf6452ff0b431
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. MACAULAY MODULES AND RINGS

### 1. Macaulay modules

Let $A$ be a noetherian ring, $M$ a finitely generated $A$-module and $p$ a prime ideal of $A$. If $p \not\in \mathrm{Supp}(M)$, one has $M_p = 0$, hence $\mathrm{prof}_{A_p}(M_p) = +\infty$ and $\dim_{A_p}(M_p) = -\infty$. If $p \in \mathrm{Supp}(M)$, one has $0 \leq \mathrm{prof}_{A_p}(M_p) \leq \dim_{A_p}(M_p) < +\infty$ ($§ 1$, No. 4, Cor. 2 of Theorem 2).

#### Definition 1 {#ac-x-s2-def-1 .statement}

*Let $A$ be a noetherian ring and $M$ a finitely generated $A$-module. One says that $M$ is Macaulay or is a Macaulay module if, for every maximal ideal $m \in \mathrm{Supp}(M)$, one has $\mathrm{prof}_{A_m}(M_m) = \dim_{A_m}(M_m)$.*

From the above, it amounts to the same thing to say that one has $\mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m)$ for every maximal ideal $m$ of $A$. Let $A$ be a noetherian local ring; in order that a nonzero finitely generated $A$-module be Macaulay, it is necessary and sufficient that its depth be equal to its dimension.

#### Example 1 {#ac-x-s2-n1-exa-1 .statement}

Every $A$-module of finite length is Macaulay.

#### Example 2 {#ac-x-s2-n1-exa-2 .statement}

Let $M'$ be a direct factor submodule of a finitely generated Macaulay $A$-module $M$. Then $M'$ is Macaulay; in fact, for every maximal ideal $m$ of $A$, the $A_m$-module $M'_m$ is a direct factor of $M_m$ and one consequently has
$$
\mathrm{prof}_{A_m}(M'_m) \geq \mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m) \geq \dim_{A_m}(M'_m),
$$
by Remark 4 of $§ 1$, No. 1 and VIII, $§ 1$, No. 4, Proposition 9 c).

#### Example 3 {#ac-x-s2-n1-exa-3 .statement}

Let $M$ be a finitely generated Macaulay $A$-module and $(x_1, \ldots, x_n)$ an $M$-regular sequence of elements of $A$. Then the $A$-module $\overline{M} = M/(x_1M + \cdots + x_nM)$ is Macaulay. Let indeed $m$ be a maximal ideal of $A$ belonging to the support of $\overline{M}$; one has $x_i \in m$ for every $i$ since $x_i$ annihilates $\overline{M}$, and the canonical images of the $x_i$ in $A_m$ form an $M_m$-regular sequence of elements of $mA_m$. One consequently has ($§ 1$, No. 4, Proposition 7 and VIII, $§ 3$, No. 2, Cor. of Proposition 3) the equalities
$$
\mathrm{prof}_{A_m}(\overline{M}_m) = \mathrm{prof}_{A_m}(M_m) - n,
$$
$$
\dim_{A_m}(\overline{M}_m) = \dim_{A_m}(M_m) - n,
$$
whence our assertion.

#### Example 4 {#ac-x-s2-n1-exa-4 .statement}

Let $M$ be a finitely generated $A$-module, and let $a$ be an ideal of $A$ such that $aM = 0$. In order that the $A$-module $M$ be Macaulay, it is necessary and sufficient that it be Macaulay as an $(A/a)$-module. In fact, put $B = A/a$; let $n$ be a maximal ideal of $B$ and $m$ its inverse image in $A$; then $\dim_{A_m}(M_m) = \dim_{B_n}(M_n)$ and $\mathrm{prof}_{A_m}(M_m) = \mathrm{prof}_{B_n}(M_n)$ ($§ 1$, No. 3, cor. of prop. 4).

#### Proposition 1 {#ac-x-s2-prop-1 .statement}

Let $\Lambda$ be a noetherian ring, $M$ a finitely generated $\Lambda$-module, and $p$ and $q$ prime ideals of $\mathrm{Supp}(M)$ such that $p \subset q$. Suppose that $\dim_{\Lambda_q}(M_q) = \mathrm{prof}_{\Lambda_q}(M_q)$. Then one has $\dim_{\Lambda_p}(M_p) = \mathrm{prof}_{\Lambda_p}(M_p)$ and
$$
\dim_{\Lambda_q}(M_q) = \dim_{\Lambda_p}(M_p) + \dim(\Lambda_q/\mathfrak{p}\Lambda_q) .
$$
This follows directly from cor. 1 of prop. 13 of § 1, No. 7.

#### Corollary {#ac-x-s2-n1-cor-1 .statement}

Let $\Lambda$ be a noetherian ring and $M$ a finitely generated $\Lambda$-module. The following conditions are equivalent:
(i) the $\Lambda$-module $M$ is Macaulay;
(ii) one has $\mathrm{prof}_{\Lambda_p}(M_p) = \dim_{\Lambda_p}(M_p)$ for every $p \in \mathrm{Supp}(M)$;
(iii) one has $\mathrm{prof}_F(M) = \mathrm{codim}(\mathrm{Supp}(M) \cap F', \mathrm{Supp}(M))$ for every closed subset $F$ of $\mathrm{Spec}(\Lambda)$;
(iv) one has $\mathrm{prof}_A(p; M) = \dim_{\Lambda_p}(M_p)$ for every $p \in \mathrm{Supp}(M)$.

(i) $\Rightarrow$ (ii): this follows from Proposition 1.
(ii) $\Rightarrow$ (iii): by prop. 8 of § 1, No. 5, $\mathrm{prof}_F(M)$ is the greatest lower bound of the integers $\mathrm{prof}(M_p)$ for $p$ ranging over $\mathrm{Supp}(M) \cap F$. If $M$ is Macaulay, then for such an ideal $p$ one has the equalities $\mathrm{prof}(M_p) = \dim(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M))$ (VIII, § 1, No. 4, prop. 9), whence (iii).
(iii) $\Rightarrow$ (iv): it is enough to take $F = V(p)$.
(iv) $\Rightarrow$ (i): this follows from the inequalities $\mathrm{prof}_A(p; M) \leq \mathrm{prof}(M_p) \leq \dim(M_p)$, valid for every $p \in \mathrm{Supp}(M)$ ($§ 1$, No. 5, remark 3 and No. 4, cor. 2 of th. 2).

#### Remark {#ac-x-s2-n1-rem-1 .statement}

Let $S$ be a multiplicative subset of $\Lambda$ and $M$ a finitely generated Macaulay $\Lambda$-module. Then $S^{-1}M$ is a Macaulay $S^{-1}\Lambda$-module. In fact, let $q \in \mathrm{Spec}(S^{-1}\Lambda)$; let $i_A^S : \Lambda \to S^{-1}\Lambda$ denote the canonical homomorphism and put $p = (i_A^S)^{-1}(q)$. The ring $(S^{-1}\Lambda)_q$ is identified with $A_p$ (II, § 2, No. 5, prop. 11), and the $A_p$-module $(S^{-1}M)_q$ with the $A_p$-module $M_p$ (II, § 2, No. 7, prop. 20), which is Macaulay by the corollary.

### 2. Support of a Macaulay module

#### Proposition 2 {#ac-x-s2-prop-2 .statement}

Let $\Lambda$ be a noetherian ring and $M$ a finitely generated Macaulay $\Lambda$-module.
a) The $\Lambda$-module $M$ has no embedded associated prime ideals.\footnote{Recall (cf. IV, § 2, No. 3, remark) that an associated prime ideal of $M$ is said to be embedded if it is not a minimal element of $\mathrm{Supp}(M)$. Thus to say that $M$ has no embedded associated prime ideals means that the associated prime ideals of $M$ are the minimal elements of $\mathrm{Supp}(M)$.}
b) Let $X$ be an irreducible closed subset of $\mathrm{Supp}(M)$ and $Y$ a closed subset of $X$. Then
$$
\mathrm{codim}(Y, X) + \mathrm{codim}(X, \mathrm{Supp}(M)) = \mathrm{codim}(Y, \mathrm{Supp}(M)) .
$$
c) The topological space $\mathrm{Supp}(M)$ is catenary (VIII, § 1, No. 2, def. 4).

d) Let $X_1$ and $X_2$ be irreducible components of $\mathrm{Supp}(M)$ and $Y$ a closed subset of $X_1 \cap X_2$. Then $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, X_2)$.

a) Let $\mathfrak{p} \in \mathrm{Ass}(M)$. Then $\mathrm{prof}_A(\mathfrak{p}; M) = 0$ (§ 1, No. 1, remark 2), hence $\dim(M_{\mathfrak{p}}) = 0$ (No. 1, cor. of prop. 1), which implies that $\mathfrak{p}$ is a minimal element of $\mathrm{Supp}(M)$.

b) Suppose first that $Y$ is irreducible. Let $\mathfrak{p}$ and $\mathfrak{q}$ be the prime ideals of $\mathrm{Supp}(M)$ such that one has $Y = V(\mathfrak{q})$ and $X = V(\mathfrak{p})$. It follows from prop. 1 that one has

$$
\begin{align*}
\mathrm{codim}(Y, X) &= \dim(A_{\mathfrak{q}}/\mathfrak{p}A_{\mathfrak{q}}) = \dim(M_{\mathfrak{q}}) - \dim(M_{\mathfrak{p}}) \\
&= \mathrm{codim}(Y, \mathrm{Supp}(M)) - \mathrm{codim}(X, \mathrm{Supp}(M)) .
\end{align*}
$$

The general case follows from VIII, $\S$ 1, No. 2, remark 3.

c) Let $X$, $Y$, $Z$ be irreducible closed subsets of $\mathrm{Supp}(M)$ such that $Z \subset Y \subset X$. The codimension of each of these subsets in $\mathrm{Supp}(M)$ is finite (VIII, $\S$ 1, No. 4, prop. 9 and $\S$ 3, No. 1, cor. 1 of prop. 2). One then deduces from b) the equality

$$
\mathrm{codim}(Z, Y) + \mathrm{codim}(Y, X) = \mathrm{codim}(Z, X)
$$

which implies c) (VIII, $\S$ 1, No. 2, prop. 4).

d) By b), we have $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, \mathrm{Supp}(M)) = \mathrm{codim}(Y, X_2)$.

In particular, if there exists a finitely generated Macaulay $A$-module $M$, with support equal to $\mathrm{Spec}(A)$, the ring $A$ is catenary and consequently every ring of fractions or every quotient ring of $A$ is catenary (VIII, $\S$ 1, No. 3, remark 2).

#### Remark 1 {#ac-x-s2-n2-rem-1 .statement}

Under the hypotheses of Prop. 2, it may happen that two irreducible components $X_1$ and $X_2$ of $\mathrm{Supp}(M)$ have an intersection $Y$ reduced to a point and that one has $\dim X_1 \neq \dim X_2$ and $\dim X_2 \neq \mathrm{codim}(Y, X_2)$ (cf. exercise 4). However, this cannot happen when the ring $A$ is local, as is shown by the following corollary.

#### Corollary {#ac-x-s2-n2-cor-1 .statement}

Let $A$ be a noetherian local ring and $M$ a nonzero finitely generated Macaulay $A$-module.

a) All maximal chains of irreducible closed subsets of $\mathrm{Supp}(M)$ have length equal to $\dim(M)$.

b) For every closed subset $X$ of $\mathrm{Supp}(M)$, one has

$$
\mathrm{codim}(X, \mathrm{Supp}(M)) = \dim(\mathrm{Supp}(M)) - \dim(X) .
$$

c) All irreducible components of $\mathrm{Supp}(M)$ have the same dimension.

d) For every ideal $J$ of $A$, one has

$$
\mathrm{prof}_A(J; M) = \dim(M) - \dim(M/JM) .
$$

a) A maximal chain of irreducible closed subsets of $\mathrm{Supp}(M)$ has as smallest element $\{m_A\}$ and as greatest element an irreducible component $X$ of

Supp(M). Its length is equal to the codimension of $\{ m_A \}$ in X (Prop. 2, c)); by Prop. 2, b) applied to the closed subsets $\{ m_A \} \subset X$, this is equal to $\operatorname{codim}(\{ m_A \}, \operatorname{Supp}(M))$, that is, to $\dim(M)$.

b) This is a consequence of a) when the subset X is irreducible (VIII, § 1, No. 2, prop. 5); the general case follows from VIII, § 1, No. 1, prop. 1 and § 1, No. 2, remark 4.

c) This is a consequence of b).

d) One has $\operatorname{prof}_A(J; M) = \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M))$ by the cor. to Prop. 1 of No. 1. It then suffices to apply b) with $X = \operatorname{Supp}(M) \cap V(J) = \operatorname{Supp}(M/JM)$ (II, § 4, No. 4, cor. to Prop. 18).

#### Remark 2 {#ac-x-s2-n2-rem-2 .statement}

Let M be a finitely generated Macaulay A-module, and $p$ an element of $\operatorname{Supp}(M)$. In view of Theorem 2 of § 1, No. 4, one has $\operatorname{prof}_A(p; M) < +\infty$, and there exists an M-regular sequence of length $\operatorname{prof}_A(p; M)$ consisting of elements of $p$. Let J denote the ideal of A generated by such a sequence; then the A-module $M/JM$ is Macaulay (No. 1, example 3) and $p$ is a minimal element of its support. In fact, $p$ contains J and therefore belong to the support of $M/JM$ (II, § 4, No. 4, cor. to Prop. 18); by Corollary 1 to Theorem 2 of § 1, No. 4, the ideal $p$ is contained in an element of $\operatorname{Ass}(M/JM)$, but every prime ideal associated with a finitely generated Macaulay module is a minimal element of its support (Prop. 2).

### 3. Macaulay modules over a local ring

#### Proposition 3 {#ac-x-s2-prop-3 .statement}

Let A be a noetherian local ring, M a nonzero finitely generated A-module, and d the dimension of M. The following conditions are equivalent:

(i) the A-module M is Macaulay;
(ii) one has $\operatorname{prof}(M) = d$;
(iii) one has $\operatorname{Ext}_A^i(\kappa_A, M) = 0$ for every integer $i < d$;
(iv) one has $\operatorname{Ext}_A^i(N, M) = 0$ for every A-module N of finite length and every integer $i < d$;
(v) one has $\operatorname{Ext}_A^i(N, M) = 0$ for every finitely generated A-module N and every integer $i < d - \dim(M \otimes_A N)$;
(vi) there exists an M-regular sequence of elements of $m_A$ of length d.

Condition (i) is equivalent to the equality $\operatorname{prof}(M) = d$, that is, to condition (ii), or again to the inequality $\operatorname{prof}(M) \geq d$, that is, to (iii) and to (vi) (§ 1, No. 4, Th. 2). The implications (v) $\Rightarrow$ (iv) and (iv) $\Rightarrow$ (iii) are obvious.

Lastly, let us suppose $M$ Macaulay and let $N$ be a finitely generated A-module. Put $F = \operatorname{Supp}(N)$; by II, § 4, No. 4, Prop. 18, one has $\operatorname{Supp}(M) \cap F = \operatorname{Supp}(M \otimes_A N)$, so that

$$
\operatorname{prof}_F(M) = \operatorname{codim}(\operatorname{Supp}(M) \cap F, \operatorname{Supp}(M)) = \dim M - \dim(M \otimes_A N)
$$

(No. 1, cor. to Prop. 1 and No. 2, cor. to Prop. 2). The implication (i) $\Rightarrow$ (v) then follows from Remark 1 of § 1, No. 5.

In the rest of this number we shall say that a finitely generated module M over a noetherian local ring A is pure if, for every prime ideal p associated with M, one has dim(A/p) = dim(M). This also means that M has no embedded associated prime ideals and that the irreducible components of the support of M all have the same dimension. Every Macaulay module over a noetherian local ring is pure (No. 2, Prop. 2 and its corollary).

Lemma 1:— Let A be a noetherian local ring, M a finitely generated and pure A-module, and x an element of mA. The following conditions are equivalent:

(i) one has dim(M/xM) = dim(M) − 1 ;
(ii) the homothety xM is injective.

One may suppose M nonzero. Assertion (i) is equivalent to the fact that x belongs to none of the minimal elements p of Supp(M) such that dim(A/p) = dim(M) (VIII, § 3, No. 2, Prop. 3), and assertion (ii) is equivalent to the fact that x belongs to none of the prime ideals associated with M (IV, § 1, No. 1, Cor. 2 to Prop. 2). Since M is pure, its associated prime ideals are the minimal elements of Supp(M); therefore (i) and (ii) are equivalent.

Let A be a noetherian local ring and M a nonzero finitely generated A-module. Recall (VIII, § 3, No. 2) that a sequence (x₁, ..., x_r) of elements of mA is said to be secant for M if one has dim(M/(x₁M + ... + x_rM)) = dim(M) − r.

#### Proposition 4 {#ac-x-s2-prop-4 .statement}

Let A be a noetherian local ring, M a nonzero finitely generated A-module, and (x₁, ..., x_r) a sequence of elements of mA secant for M. The following conditions are equivalent:

(i) the A-module M is Macaulay ;
(ii) the sequence (x₁, ..., x_r) is M-regular and the A-module M/(x₁M + ... + x_rM) is Macaulay.

Suppose that the sequence (x₁, ..., x_r) is M-regular. One then has

$$
\dim(M) = r + \dim(M/(x_1M + ... + x_rM))
$$
$$
\operatorname{prof}(M) = r + \operatorname{prof}(M/(x_1M + ... + x_rM))
$$

(§ 1, No. 4, Prop. 7), whence the implication (ii) ⇒ (i).

Suppose the A-module M Macaulay, and prove (ii) by induction on r. The assertion is obvious if r = 0. If r ≥ 1, the A-module N = M/(x₁M + ... + x_{r−1}M) is Macaulay by the induction hypothesis, and one has dim(N/x_rN) = dim(N) − 1 since the sequence (x₁, ..., x_r) is secant; the homothety (x_r)_N is therefore injective (Lemma 1), and N/x_rN is Macaulay (No. 1, Example 3), whence (ii).

#### Theorem 1 {#ac-x-s2-thm-1 .statement}

Let A be a noetherian local ring, M a nonzero finitely generated A-module, d the dimension of M, x = (x₁, ..., x_d) a sequence of elements of mA secant for M, and J the ideal generated by it. The following conditions are equivalent:

(i) the A-module M is Macaulay ;

(ii) the sequence $x$ is M-regular ;
(iii) the sequence $x$ is completely secant for $M$ (A, X, p. 157, Def. 2) ;
(iv) the multiplicity (VIII, § 7, No. 1, Def. 1) $e_J(M)$ of $M$ relative to the ideal $J$ is equal to the length of the A-module $M/JM$ ;
(v) for each integer $i$ such that $1 \leq i \leq d$, the A-module $M/(x_1M + \ldots + x_{i-1}M)$ is pure.

The equivalence of (ii) and (iii) follows from A, X, p. 160, Cor. 1 to Th. 1. Since the A-module $M/JM$ is of finite length (VIII, § 3, No. 2, Th. 1), the equivalence of (iii) and (iv) follows from VIII, § 4, No. 3, Prop. 4 and No. 4, Th. 3. It remains to prove the equivalence of (i), (ii), and (v).

(i) $\Rightarrow$ (v) : if $M$ is Macaulay, each of the modules $M/(x_1M + \ldots + x_{i-1}M)$ is Macaulay (Prop. 4), hence pure.

(v) $\Rightarrow$ (ii) : this follows from Lemma 1 applied to each of the modules $M/(x_1M + \ldots + x_{i-1}M)$.

(ii) $\Rightarrow$ (i) : this follows from Prop. 4, since $M/JM$ is of finite length, hence Macaulay.

### 4. Strongly secant subsets and quotients of a Macaulay module

Let $A$ be a noetherian ring, $M$ a finitely generated A-module, and $S$ a subset of $A$. In accordance with the conventions of Chapter VIII, we shall denote by $SM$ the submodule $\sum_{s \in S} sM$ of $M$, and by $\mathcal{G}$ the ideal of $A$ generated by $S$.

#### Lemma 2 {#ac-x-s2-lem-2 .statement}

Let $\overline{\mathcal{G}}$ be the image of $\mathcal{G}$ in $A/\mathrm{Ann}(M)$. One has
$$
\mathrm{ht}(\overline{\mathcal{G}}) = \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$
When moreover $SM \neq M$, one has
$$
\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S) .
$$

Let us denote by $\alpha$ the annihilator of $M$. By the cor. to Prop. 18 of II, § 4, No. 4, the support of the A-module $M/SM$ is $V(\mathcal{G} + \alpha)$. Its codimension in $\mathrm{Supp}(M)$ is therefore equal to the codimension of $V(\mathcal{G} + \alpha)$ in $V(\alpha)$, or again to the codimension of $V((\mathcal{G} + \alpha)/\alpha)$ in $\mathrm{Spec}(A/\alpha)$, which is none other than the height of $\overline{\mathcal{G}}$.

Suppose $SM \neq M$; the inequality $\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S)$ is obvious when $S$ is infinite, and follows from Prop. 4 b) of VIII, § 3, No. 3 when $S$ is finite.

#### Definition 2 {#ac-x-s2-def-2 .statement}

Let $A$ be a noetherian ring, $M$ a finitely generated A-module, and $S$ a finite subset of $A$. One says that $S$ is strongly secant for $M$ if one has
$$
\mathrm{Card}(S) \leq \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$

#### Remark 1 {#ac-x-s2-n4-rem-1 .statement}

Every finite subset S of A such that SM = M is strongly secant for M. When SM ≠ M, it follows from lemma 2 that, for S to be strongly secant for M, it is necessary and sufficient that one have Card(S) = codim(Supp(M/SM), Supp(M)), or again ht($\overline{\mathcal{G}}$) = Card(S).

#### Remark 2 {#ac-x-s2-n4-rem-2 .statement}

If the ring A is local and the nonzero module M, every subset S of $m_A$ strongly secant for M is secant for M. In fact, since the $\Lambda$-module M/SM is nonzero, one has

$$
\text{Card}(S) \leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/SM)
$$

(VIII, § 1, No. 2, Prop. 3 a)), whence our assertion.

#### Proposition 5 {#ac-x-s2-prop-5 .statement}

Let A be a noetherian ring, M a finitely generated A-module, and S a finite subset of A. The following conditions are equivalent:

(i) the subset S of A is strongly secant for M;
(ii) for every element $p$ of Supp(M/SM), the canonical mapping $\Lambda \to A_p$ induces a bijection of S onto a subset of $pA_p$ secant for $M_p$.

(i) $\Rightarrow$ (ii) : Let $p \in \operatorname{Supp}(M/SM)$ and let $S'$ be the image of S in $A_p$. The set $S'$ is contained in the maximal ideal $pA_p$, and one has

$$
\dim(M_p/S'M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M/SM))
$$

(VIII, § 1, No. 4, Prop. 9). The inequality Card(S) $\leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M))$ and Prop. 3 b) of VIII, § 1, No. 2 imply the relations

$$
\text{Card}(S) + \dim(M_p/S'M_p) \leq \operatorname{codim}(V(p), \operatorname{Supp}(M)) = \dim(M_p) .
$$

Since $M_p$ is nonzero, one has on the other hand $\dim(M_p) \leq \text{Card}(S') + \dim(M_p/S'M_p)$ (VIII, § 3, No. 2, formula (8)). Condition (ii) then follows from the inequality $\text{Card}(S') \leq \text{Card}(S)$.

(ii) $\Rightarrow$ (i) : One may suppose SM $\neq$ M. If condition (ii) is satisfied, one has for every prime ideal $p$ of Supp(M/SM)

$$
\text{Card}(S) = \text{Card}(S') \leq \dim(M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M)) ,
$$

which implies (i) by passing to the greatest lower bound.

#### Corollary {#ac-x-s2-n4-cor-1 .statement}

Let A be a noetherian ring and M a finitely generated A-module. Every M-regular sequence is strongly secant for M.

Let x be an M-regular sequence, and J the ideal of A generated by it. For every prime ideal $p \in \operatorname{Supp}(M/JM)$, the image of x in $A_p$ is an $M_p$-regular sequence of elements of $pA_p$, hence a secant sequence for $M_p$ (VIII, § 3, No. 2, cor. to Prop. 3).

#### Proposition 6 {#ac-x-s2-prop-6 .statement}

Let A be a noetherian ring, M a finitely generated Macaulay A-module, and S a finite subset of A strongly secant for M. Then the A-module M/SM is Macaulay.

For every maximal ideal $m \in \mathrm{Supp}(M/SM)$, the image of S in $A_m$ is secant for $M_m$ (Prop. 5). Since $M_m$ is a Macaulay $A_m$-module, the same is true of $(M/SM)_m$ (Prop. 4), whence the proposition.

**Theorem 2 (Macaulay-Cohen).**— *Let A be a noetherian ring and M a finitely generated A-module. The following conditions are equivalent:*

(i) *the A-module M is Macaulay;*

(ii) *for every ideal J of A generated by an M-regular sequence of elements of A, the A-module M/JM has no embedded associated prime ideals;*

(iii) *for every finite subset S of A strongly secant for M, the A-module M/SM has no embedded associated prime ideals.*

(i) $\Rightarrow$ (iii) : Let S be a finite subset of A strongly secant for M. The A-module M/SM is Macaulay (Prop. 6) and in particular has no embedded associated prime ideals (No. 2, Prop. 2, a)).

(iii) $\Rightarrow$ (ii) : This follows from the cor. to Prop. 5.

(ii) $\Rightarrow$ (i): Let $p \in \mathrm{Supp}(M)$; let us prove that the $A_p$-module $M_p$ is Macaulay. We argue by induction on the integer $\dim(M_p)$. If $\dim(M_p)$ is zero, $M_p$ is an $A_p$-module of finite length, hence Macaulay (Example 1, No. 1). Suppose that $\dim(M_p)$ is nonzero, that is to say that $p$ is not a minimal element of $\mathrm{Supp}(M)$ (VIII, § 1, No. 4, Prop. 9 a)). Since M has no embedded associated prime ideals, $p$ is contained in no associated prime ideal of M, and there exists an element $x$ of $p$ such that the homothety $x_M$ is injective (§ 1, Remark 2). The homothety $x_{M_p}$ is then injective, and one has $\dim(M_p/xM_p) < \dim(M_p)$ (VIII, § 3, No. 2, Prop. 3). By the induction hypothesis applied to the A-module $M/xM$ and to the prime ideal $p$ of $\mathrm{Supp}(M/xM)$, the $A_p$-module $M_p/xM_p$ is Macaulay, which implies that the $A_p$-module $M_p$ is Macaulay (No. 3, Prop. 4).

### 5. Macaulay Rings

#### Definition 3 {#ac-x-s2-def-3 .statement}

*One says that a ring $\Lambda$ is Macaulay, or is a Macaulay ring, if it is noetherian and the A-module $\Lambda$ is Macaulay.*

#### Example 1 {#ac-x-s2-n5-exa-1 .statement}

Every artinian ring is a Macaulay ring (No. 1, Example 1).

#### Example 2 {#ac-x-s2-n5-exa-2 .statement}

A Macaulay ring has no embedded associated prime ideals (No. 2, Prop. 2). Conversely, let $A$ be a noetherian ring of dimension $\leqslant 1$ which has no embedded associated prime ideals; for every nonempty finite subset strongly secant S of A, the A-module $A/SA$ is of dimension $\leqslant 0$, hence Macaulay (No. 1, Example 1); hence A is a Macaulay ring (No. 4, Theorem 2). In particular a reduced noetherian ring of dimension $\leqslant 1$ is a Macaulay ring.

#### Example 3 {#ac-x-s2-n5-exa-3 .statement}

A normal noetherian ring of dimension $\leqslant 2$ is a Macaulay ring (§ 1, No. 10, text preceding Theorem 4). Conversely, let $A$ be a Macaulay ring whose local ring $A_p$ at every prime ideal $p$ of height $\leqslant 1$ is integrally closed; then A is normal (§ 1, No. 10, Theorem 4).

#### Example 4 {#ac-x-s2-n5-exa-4 .statement}

If $A$ is a Macaulay ring, the same is true of $S^{-1}A$ for every multiplicative subset $S$ of $A$ (No. 1, Remark). Conversely, if the ring $A_m$ is a Macaulay ring for every maximal ideal $m$ of $A$, then the ring $A$ is Macaulay (No. 1, Def. 1).

#### Example 5 {#ac-x-s2-n5-exa-5 .statement}

Let $A$ be a noetherian ring and $J$ an ideal of $A$. In order that $A/J$ be a Macaulay ring, it is necessary and sufficient that it be a Macaulay $\Lambda$-module (No. 1, Example 4).

#### Example 6 {#ac-x-s2-n5-exa-6 .statement}

Let $A$ be a noetherian local ring and $J$ an ideal of $A$ generated by an $A$-regular sequence. In order that $A/J$ be a Macaulay ring, it is necessary and sufficient that $A$ be one (Example 5 and Prop. 4 of No. 3).

#### Example 7 {#ac-x-s2-n5-exa-7 .statement}

For a noetherian local ring $A$ to be a Macaulay ring, it is necessary and sufficient that it possess an ideal of definition generated by an $A$-regular sequence: this follows from Prop. 3 of No. 3, and from the fact that an $A$-regular sequence of elements of $m_A$ generates an ideal of definition if and only if it is of length $\dim(A)$ (VIII, § 3, No. 2, Th. 1 and cor. to Prop. 3). In particular, every regular noetherian local ring is a Macaulay ring (VIII, § 5, No. 2, Th. 1). More generally, the quotient of a regular noetherian local ring $A$ by an ideal generated by an $A$-regular sequence is a Macaulay ring (Example 6).

#### Proposition 7 {#ac-x-s2-prop-7 .statement}

Let $A$ be a noetherian ring. The following conditions are equivalent:

(i) $A$ is a Macaulay ring;
(ii) for every closed subset $F$ of $\mathrm{Spec}(A)$, one has $\mathrm{prof}_F(A) = \mathrm{codim}(F)$;
(iii) every ideal $J$ of $A$ contains an $A$-regular sequence of length $\mathrm{ht}(J)$;
(iii') every maximal ideal $m$ of $A$ contains an $A$-regular sequence of length $\mathrm{ht}(m)$;
(iv) for every ideal $J$ of $A$, one has $\mathrm{Ext}_A^i(A/J, A) = 0$ for $i < \mathrm{ht}(J)$;
(iv') for every maximal ideal $m$ of $A$, one has $\mathrm{Ext}_A^i(A/m, A) = 0$ for $i < \mathrm{ht}(m)$;
(v) for every prime ideal $p$ of $A$ and every ideal $J$ of $A_p$ generated by a maximal secant sequence for $A_p$, one has $e_J(A_p) = \mathrm{long}(A_p/ JA_p)$;
(v') for every maximal ideal $m$ of $A$, there exists an ideal $J$ of $A_m$, generated by a maximal secant sequence for $A_m$, satisfying $e_J(A_m) = \mathrm{long}(A_m/ JA_m)$;
(vi) (Macaulay-Cohen criterion) for every finite subset $S$ of $A$ such that the ideal $\mathfrak{S}$ generated by $S$ is of height $\mathrm{Card}(S)$, the $A$-module $A/\mathfrak{S}$ has no embedded associated prime ideals.

The equivalence of (i) and (ii) follows from No. 1, cor. to Prop. 1. By Th. 2 of § 1, No. 4, and the definition of depth, conditions (iii) and (iv) (resp. (iii') and (iv')) mean that one has $\mathrm{prof}_A(J; A) \geq \mathrm{ht}(J)$ for every ideal (resp. every maximal ideal) $J$ of $A$. Hence one has

$$
(i) \Leftrightarrow (ii) \Rightarrow (iii) \Leftrightarrow (iv) \Rightarrow (iii') \Leftrightarrow (iv').
$$

But (iv') implies, for every maximal ideal $m$ of $A$, $\mathrm{Ext}_{A_m}^i(\kappa(m), A_m) = 0$ for $i < \dim(A_m)$, whence $\mathrm{prof}(A_m) \geq \dim(A_m)$, so that $A$ is a Macaulay ring.

The equivalence of (i), (v) and (v’) follows from Th. 1 of No. 3, and that of (i) and (vi) from Th. 2 of No. 4.

### 6. Macaulay modules and finite algebras

#### Remark {#ac-x-s2-n6-rem-1 .statement}

Let $\rho : A \to B$ be a homomorphism of rings, and let $p \in \mathrm{Spec}(A)$. Let us denote by $\overline{B}$ the ring $\kappa(p) \otimes_A B$. It may be identified with $S^{-1}B/p(S^{-1}B)$, where $S$ is the multiplicative subset $\rho(A - p)$ of $B$; the prime ideals of $\overline{B}$ are therefore the ideals $q\overline{B}$, where $q$ is a prime ideal of $B$ containing $pB$ and not meeting $S$, in other words a prime ideal of $B$ lying over $p$. For such an ideal $q$, one has $S \subset B - q$, hence the local ring of $\overline{B}$ at $q\overline{B}$ may be identified with $B_q/pB_q$, that is to say again with $\kappa(p) \otimes_A B_q$.

Analogously, if $N$ is a $B$-module, the $\overline{B}_{q\overline{B}}$-module $(\kappa(p) \otimes_A N)_{q\overline{B}}$ may be identified with $\kappa(p) \otimes_A N_q$. Suppose moreover that the $B$-module $N$ is finitely generated; by Nakayama's lemma, the condition $\kappa(p) \otimes_A N_q = 0$ is equivalent to $N_q = 0$. Thus the support of the $\overline{B}$-module $\kappa(p) \otimes_A N$ consists of the ideals $q\overline{B}$, where $q$ runs through the prime ideals of $\mathrm{Supp}_B(N)$ lying over $p$. In particular, in order that the module $\kappa(p) \otimes_A N$ be nonzero, it is necessary and sufficient that there exist a prime ideal of $\mathrm{Supp}_B(N)$ lying over $p$.

#### Proposition 8 {#ac-x-s2-prop-8 .statement}

Let $\rho : A \to B$ be a homomorphism of Noetherian rings and let $N$ be a $B$-module which is a finitely generated $A$-module. In order that the $A$-module $N$ be Macaulay, it is necessary and sufficient that the $B$-module $N$ be Macaulay and that, for every pair $(n, n')$ of maximal ideals of $\mathrm{Supp}_B(N)$ such that $\rho^{-1}(n) = \rho^{-1}(n')$, one has $\dim_{B_n}(N_n) = \dim_{B'_n}(N'_n)$.

The $A$-module $B/\mathrm{Ann}_B(N)$ is isomorphic to a submodule of the finitely generated $A$-module $\mathrm{End}_A(N)$, and is therefore of finite type. Replacing $A$ by $A/\mathrm{Ann}_A(N)$ and $B$ by $B/\mathrm{Ann}_B(N)$, we are reduced to the case where $\rho$ is injective and makes $B$ into a finite $A$-algebra, and where one has $\mathrm{Supp}_A(N) = \mathrm{Spec}(A)$ and $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$. The mapping $f : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$ deduced from $\rho$ is then surjective, and a prime ideal $q$ of $B$ is maximal if and only if $f(q)$ is a maximal ideal of $A$ (V, § 2, No. 1, th. 1 and prop. 1).

Let $m$ be a maximal ideal of $A$. By the above remark, the prime ideals of the ring $B_m$ containing $mB_m$ are the ideals of the form $qB_m$, where $q \in \mathrm{Spec}(B)$ is an ideal of $B$ (necessarily maximal) such that $f(q) = m$. One has

$$
\mathrm{prof}_{A_m}(N_m) = \mathrm{prof}_{B_m}(mB_m; N_m) = \inf_{q \in f^{-1}(m)} (\mathrm{prof}_{B_q}(N_q))
$$

(§ 1, No. 3, prop. 4 and No. 5, prop. 8), and

$$
\dim_{A_m}(N_m) = \dim_{B_m}(N_m) = \sup_{q \in f^{-1}(m)} (\dim_{B_q}(N_q))
$$

(VIII, § 2, No. 3, th. 1 and § 1, No. 4, prop. 9). Since one has $\mathrm{prof}_{B_q}(N_q) \leq \dim_{B_q}(N_q)$ for every $q \in f^{-1}(m)$, the proposition follows from these equalities.

#### Corollary 1 {#ac-x-s2-prop-8-cor-1 .statement}

Let $\rho : A \to B$ be a homomorphism of Noetherian rings. If $B$ is a finite $A$-algebra and a Macaulay $A$-module, it is a Macaulay ring. If moreover $\rho$ is injective, one has $\mathrm{ht}(aB) = \mathrm{ht}(a)$ for every ideal $a$ of $A$, and $\mathrm{ht}(b) = \mathrm{ht}(\rho^{-1}(b))$ for every ideal $b$ of $B$.

The first assertion results from Prop. 8. Suppose $\rho$ injective. Let $a$ be an ideal of $A$. We have $\mathrm{ht}(a) = \mathrm{prof}_A(a; B)$ since the $A$-module $B$ is Macaulay, with support equal to $\mathrm{Spec}(A)$ (No. 1, corollary to Prop. 1), $\mathrm{ht}(aB) = \mathrm{prof}_B(aB; B)$ (*loc. cit.*) and $\mathrm{prof}_A(a; B) = \mathrm{prof}_B(aB; B)$ ($§ 1$, No. 3, Prop. 4), whence $\mathrm{ht}(aB) = \mathrm{ht}(a)$. Let $b$ be an ideal of $B$. From the preceding, we have $\mathrm{ht}(\rho^{-1}(b)) = \mathrm{ht}(\rho^{-1}(b)B)$. But $\rho^{-1}(b)B$ is contained in $b$, hence of height less than $\mathrm{ht}(b)$, and we have $\mathrm{ht}(b) \leq \mathrm{ht}(\rho^{-1}(b))$ by VIII, $§ 2$, No. 3, Theorem 1, b).

#### Corollary 2 {#ac-x-s2-prop-8-cor-2 .statement}

Let $A$ be an integrally closed noetherian ring and $B$ a ring containing $A$. Suppose that $B$ is a torsion-free $A$-module, of finite type. If $B$ is a Macaulay ring, the $A$-module $B$ is Macaulay.

In fact, two prime ideals of $B$ lying over the same ideal of $A$ have the same height (VIII, $§ 2$, No. 3, Theorem 2). One can therefore apply Prop. 8 with $N = B$.

#### Corollary 3 {#ac-x-s2-prop-8-cor-3 .statement}

Let $A$ be an integrally closed ring, $K$ its field of fractions, $L$ a finite $K$-algebra such that $[L : K] 1_A$ is invertible in $A$, and $B$ a sub-$A$-algebra of $L$, finite over $A$.

a) *The sub*-$A$-*module* $Al_B$ of $B$ is a direct factor.

b) *For every ideal* $J$ *of* $A$, *one has the inequality* $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_B(JB; B)$.

c) *If* $B$ *is a Macaulay ring*, *the same is true of* $A$.

The $K$-linear mapping $\mathrm{Tr}_{L/K} : L \to K$ maps $B$ into $A$ (V, $§ 1$, No. 6, corollary 2 to Prop. 17), and therefore defines by restriction an $A$-linear mapping $t : B \to A$. For every $x \in A$, we have $t(xl_B) = [L : K] x$, whence a).

By Proposition 4 of $§ 1$, No. 3, we have $\mathrm{prof}_A(J; B) = \mathrm{prof}_B(JB; B)$; but by a) and Remark 4 of $§ 1$, No. 1, we have $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_A(J; B)$, whence b).

If the ring $B$ is noetherian, the same is true of $A$: in fact, by a) we have $aB \cap A = a$ for every ideal $a$ of $A$; thus every increasing sequence $(a_n)_{n \in \mathbf{N}}$ of ideals of $A$ is stationary since the sequence $(a_nB)_{n \in \mathbf{N}}$ is stationary. Under the hypotheses of c), the $A$-module $B$ is Macaulay (Corollary 2), and the same is true of the $A$-module $A$ (No. 1, Example 2).

#### Example {#ac-x-s2-n6-exa-1 .statement}

Corollary 3 applies in particular in the following two situations:

a) Consider a noetherian integrally closed ring $A$, a separable extension $L$ of its field of fractions, of finite degree $n$ such that $n1_A$ is invertible in $A$, and take for $B$ the integral closure of $A$ in $L$ (V, $§ 1$, No. 6, Corollary 1 of Proposition 18).

b) Consider a noetherian integrally closed ring $B$ and a finite group $G$ of automorphisms of $B$, such that $\mathrm{Card}(G) 1_B$ is invertible in $B$. Take for $A$ the ring of elements of $B$ invariant under the action of $G$. Let us verify that we are in a particular case of a). The group $G$ operates on the field of the

In particular, if B is a Macaulay ring, the same is true of A.

### 7. Macaulay Modules and Flat Algebras

#### Proposition 9 {#ac-x-s2-prop-9 .statement}

Let ρ : A → B be a homomorphism of noetherian rings, M a finitely generated A-module and N a finitely generated B-module, flat over A. Denote by $^a\rho : \mathrm{Spec}(B) \longrightarrow \mathrm{Spec}(\Lambda)$ the mapping associated with ρ. The following conditions are equivalent:

(i) the B-module $M \otimes_A N$ is Macaulay;
(ii) the $(\kappa(p) \otimes_A B)$-module $\kappa(p) \otimes_A N$ is Macaulay for every $p \in \mathrm{Supp}_A(M)$, and the $A_p$-module $M_p$ is Macaulay for every $p \in ^a\rho(\mathrm{Supp}_B(N))$;
(iii) for every maximal ideal of $\mathrm{Supp}_B(N)$ whose inverse image $p$ in A belongs to $\mathrm{Supp}_A(M)$, the $A_p$-module $M_p$ and the $(\kappa(p) \otimes_A B)$-module $\kappa(p) \otimes_A N$ are Macaulay.

If moreover the B-module N is faithfully flat, these conditions imply that the A-module M is Macaulay.

Let q be a prime ideal of B belonging to the support of $M \otimes_A N$. Put $p = \rho^{-1}(q)$. Since the module $(M \otimes_A N)_q$ is identified with $M_p \otimes_{A_p} N_q$, the modules $M_p$ and $N_q$ are non-zero, and the same is true of $\kappa(p) \otimes_A N_q$ (No. 6, Remark). The $A_p$-module $N_q$, being isomorphic to a module of fractions of $N_p$, is flat and we have the equalities

$$
\mathrm{prof}_{B_q}((M \otimes_A N)_q) = \mathrm{prof}_{A_p}(M_p) + \mathrm{prof}_{B_q}(\kappa(p) \otimes_A N_q)
$$
$$
\dim_{B_q}((M \otimes_A N)_q) = \dim_{A_p}(M_p) + \dim_{B_q}(\kappa(p) \otimes_A N_q)
$$

(§ 1, No. 6, prop. 11, b) and remark), in which each term is an integer $\geq 0$. Taking into account the fact that the $B_q$-module $\kappa(p) \otimes_A N_q$ is a Macaulay module if and only if it is so as a $(\kappa(p) \otimes_A B_q)$-module (No. 1, example 4), we deduce the equivalence of the following two conditions:

(α) the $B_q$-module $(M \otimes_A N)_q$ is a Macaulay module;
(β) the $A_p$-module $M_p$ and the $(\kappa(p) \otimes_A B_q)$-module $\kappa(p) \otimes_A N_q$ are Macaulay modules.

Let us now prove that (iii) implies (i). Let n be a maximal ideal of B belonging to the support of $M \otimes_A N$, and let $p = \rho^{-1}(n)$. From the foregoing we have $p \in \mathrm{Supp}_A(M) \cap ^a\rho(\mathrm{Supp}_B(N))$; condition (iii) and the remark of No. 6 imply that condition (β) above is satisfied with $q = n$. It follows that the $B_n$-module $(M \otimes_A N)_n$ is a Macaulay module, whence (i).

The implication (ii) ⇒ (iii) is clear; let us prove that (i) implies (ii). Suppose the B-module M ⊗_A N to be a Macaulay module. Let p be an element of Supp_A(M). We may suppose that the (κ(p) ⊗_A B)-module κ(p) ⊗_A N is nonzero, that is to say, that there exists a prime ideal q of Supp_B(N) lying over p (No. 6, remark). The B_q-module (M ⊗_A N)_q is a Macaulay module (No. 1, example 3); it follows from implication (α) ⇒ (β) proved above and from the remark of No. 6 that the A_p-module M_p and the (κ(p) ⊗_A B)-module (κ(p) ⊗_A N) are Macaulay modules, whence (ii).

If moreover N is faithfully flat over A, we have κ(p) ⊗_A N ≠ 0 for every p ∈ Spec(A), whence a_p(Supp_B(N)) = Spec(A) (No. 6, remark), so that (ii) implies that M is a Macaulay module.

#### Corollary 1 {#ac-x-s2-prop-9-cor-1 .statement}

Let ρ : Λ → B be a local homomorphism of noetherian local rings, M a nonzero finitely generated A-module and N a nonzero finitely generated B-module which is a flat A-module. In order that the B-module M ⊗_A N be a Macaulay module, it is necessary and sufficient that the A-module M be a Macaulay module and that the B/m_A B-module N/m_A N be a Macaulay module.

In fact, N is a faithfully flat A-module since N/m_A N is nonzero (I, § 3, No. 1, definition 1).

#### Corollary 2 {#ac-x-s2-prop-9-cor-2 .statement}

Let ρ : A → B be a homomorphism of noetherian rings making B into a faithfully flat A-module and let M be a finitely generated A-module. In order that the B-module M ⊗_A B be a Macaulay module, it is necessary and sufficient that the A-module M be a Macaulay module and that κ(p) ⊗_Λ B be a Macaulay ring for every p ∈ Supp(M).

#### Corollary 3 {#ac-x-s2-prop-9-cor-3 .statement}

Let A be a noetherian ring, B a finite flat Λ-algebra, M a finitely generated Macaulay A-module. Then the B-module M ⊗_A B is a Macaulay module.

In fact, for every p ∈ Spec(A), the ring κ(p) ⊗_Λ B is a finite κ(p)-algebra, hence is a Macaulay ring (No. 5, example 1), and we apply prop. 9.

#### Corollary 4 {#ac-x-s2-prop-9-cor-4 .statement}

Let A be a noetherian ring, J an ideal of A and M a finitely generated A-module. Denote by Ā and Ĝ the separated completions of A and M for the J-adic topology, and by S the multiplicative subset 1 + J of Λ. Consider the following conditions:

(i) the A-module M is a Macaulay module;
(ii) the Ā-module Ĝ is a Macaulay module;
(iii) the S^{-1}A-module S^{-1}M is a Macaulay module;
(iv) for every maximal ideal m ∈ Supp(M) ∩ V(J), the A_m-module M_m is a Macaulay module;
(v) for every prime ideal p ∈ Supp(M) such that p + J ≠ A, the Λ_p-module M_p is a Macaulay module and the ring κ(p) ⊗_A Ā is a Macaulay ring.

Conditions (ii) to (v) are equivalent, and are implied by (i). When the ideal J is contained in the radical of A, conditions (i) to (v) are equivalent.

We know that (i) implies (iii) (No. 1, example 3), and (iii) is identical with (i) when J is contained in the radical of A (since the elements of S are then invertible).

It is clear that (v) implies (iv) and that (iv) implies (i).

(i) $\Rightarrow$ (ii) : Let $m$ be a maximal ideal of $A$; then $m\widehat{A}$ is a maximal ideal of $\widehat{A}$ lying over $m$, and every maximal ideal of $\widehat{A}$ is obtained in this way (III, § 3, No. 4, prop. 8). The ring $\kappa(m) \otimes_A \widehat{A}$ is a field, hence a Macaulay ring; if the $A$-module $M$ is a Macaulay module, the same is true of the $\widehat{A}$-module $\widehat{M}$ by implication (iii) $\Rightarrow$ (i) of prop. 9.

(ii) $\Rightarrow$ (v) : The $\widehat{A}$-module $\widehat{M}$ is isomorphic to $M \otimes_A \widehat{A}$ (III, § 3, No. 4, th. 3); if it is a Macaulay module, it follows from prop. 9, (i) $\Rightarrow$ (ii) that $\kappa(p) \otimes_A \widehat{A}$ is a Macaulay ring for every $p \in \mathrm{Supp}(M)$, and that the $A$-module $M$ is a Macaulay module.

#### Proposition 10 {#ac-x-s2-prop-10 .statement}

*Let $\rho : A \to B$ be a homomorphism of noetherian rings making $B$ into a flat $\Lambda$-module. The following conditions are equivalent:*

(i) $B$ is a Macaulay ring;
(ii) for every prime ideal $q$ of $B$, the rings $A_{\rho^{-1}(q)}$ and $\kappa(\rho^{-1}(q)) \otimes_A B$ are Macaulay rings;
(iii) for every maximal ideal $n$ of $B$, the rings $A_{\rho^{-1}(n)}$ and $\kappa(\rho^{-1}(n)) \otimes_A B$ are Macaulay rings.

*If moreover $B$ is faithfully flat over $A$, these conditions imply that $A$ is a Macaulay ring.*

This is the special case $M = A$, $N = B$ of prop. 9.

#### Corollary 1 {#ac-x-s2-prop-10-cor-1 .statement}

*Every finite flat algebra over a Macaulay ring is a Macaulay ring.*

#### Corollary 2 {#ac-x-s2-prop-10-cor-2 .statement}

*Let $A$ be a Macaulay ring and $n$ a positive integer; then $A[X_1, \ldots, X_n]$ and $A[[X_1, \ldots, X_n]]$ are Macaulay rings.*

It is enough to treat the case $n = 1$. The ring $A[T]$ is noetherian (A, VIII, § 1, No. 4, cor. 1), and, for every field $k$, the ring $k[T]$ is a Macaulay ring (No. 5, example 2); consequently, the ring $A[T]$ is a Macaulay ring (prop. 10) and the ring $A[[T]]$ is a Macaulay ring (cor. 4 of prop. 9).

#### Corollary 3 {#ac-x-s2-prop-10-cor-3 .statement}

*Every algebra of finite type over a noetherian Macaulay ring is catenary.*

For such an algebra is a quotient of a polynomial ring over a Macaulay ring, hence a quotient of a Macaulay ring (cor. 2), and therefore is catenary (No. 2).

## EXERCISES {#ac-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
