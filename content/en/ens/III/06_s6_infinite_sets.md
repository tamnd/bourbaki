---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 6
section_title: Infinite sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 183-190, 241-251
pdf_pages: 0189-0196, 0247-0257
extraction: ocr
subsections:
    - "no": 1
      title: THE SET OF NATURAL INTEGERS
      page: 183
      pdf_page: 189
    - "no": 2
      title: DEFINITION OF MAPPINGS BY INDUCTION
      page: 184
      pdf_page: 190
    - "no": 3
      title: PROPERTIES OF INFINITE CARDINALS
      page: 186
      pdf_page: 192
    - "no": 4
      title: COUNTABLE SETS
      page: 188
      pdf_page: 194
    - "no": 5
      title: STATIONARY SEQUENCES
      page: 189
      pdf_page: 195
statements: 26
exercises: 32
content_sha256: 77f70aee6764a579bfe1b9d46b02201949dbe28ed9954f8d2836dfccee740326
---

## 6. INFINITE SETS

### 1. THE SET OF NATURAL INTEGERS

#### Definition 1 {#ens-iii-s6-def-1 .statement tag=03MV}

*A set is said to be infinite if it is not finite.*

In particular, a cardinal is infinite if it is not an integer.

The relation "there exists an infinite set" implies that the relation "$x$ is an integer" is *collectivizing* (Chapter II, § 1, no. 4); for if $\mathfrak{a}$ is an infinite cardinal and $n$ an arbitrary integer, we cannot have $\mathfrak{a} \leqslant n$ (§ 4, no. 2, Proposition 2). We have therefore $n < \mathfrak{a}$ for all integers $n$, which shows that the set of integers $< \mathfrak{a}$ (§ 3, no. 2, Remark following Theorem 1) contains all integers. Conversely, if the relation "$x$ is an integer" is collectivizing, then the set E of integers is an *infinite* set. For each integer $n$, the interval $[0, n]$ is a subset of $n + 1$ elements of E (§ 5, no. 3, Proposition 5). Therefore Card (E) $\geqslant n + 1 > n$. But to say that Card(E) $\neq n$ for every integer $n$ means that E is infinite.

¶ We now introduce the following axiom :

A5 ("Axiom of infinity".) *There exists an infinite set.*

It is not known whether or not this axiom can be deduced from the axioms and axiom schemes introduced previously; although the question has not been definitively settled, it is to be presumed that this axiom is independent of the others.

The preceding remarks then prove the following theorem :

#### Theorem 1 {#ens-iii-s6-thm-1 .statement tag=03MW}

*The relation "$x$ is an integer" is collectivizing.*

We shall denote by $\mathbf{N}$ the set of integers (also called "the set of natural integers" when necessary to avoid ambiguity). The cardinal of $\mathbf{N}$ is

denoted by $\aleph_0$. Whenever $\mathbf{N}$ is considered as an ordered set, it is always the ordering (called the *usual* ordering) defined in § 3, no. 2 that is under consideration, unless the contrary is expressly stated.

#### Definition 2 {#ens-iii-s6-def-2 .statement tag=03MX}

*A sequence* (resp. *a sequence of elements of a set* E) *is a family* (resp. *a family of elements of* E) *whose index set is a subset of* $\mathbf{N}$. *The sequence is said to be infinite if its index set is an infinite subset of* $\mathbf{N}$.

Let $\mathrm{P}\{n\}$ be a relation and let I denote the set of integers $n$ such that $\mathrm{P}\{n\}$ is true. I is then a subset of $\mathbf{N}$. A sequence $(x_n)_{n\in\mathrm{I}}$ is then sometimes written $(x_n)_{\mathrm{P}\{n\}}$, and $x_n$ is called the *nth term* in the sequence. A sequence whose index set is the set of integers $n \geqslant k$ is often written $(x_n)_{k \leqslant n}$ or $(x_n)_{n \geqslant k}$, or even just $(x_n)$ if $k = 0$ or $k = 1$. Under the same conditions, for example, the notations $\prod_{\mathrm{P}\{n\}} \mathrm{X}_n$ and $\prod_{n=k}^{\infty} \mathrm{X}_n$ are used to denote the product of a sequence of sets $(\mathrm{X}_n)_{n\in\mathrm{I}}$, and there are analogous notations for unions, intersections, cardinal products, and cardinal sums.

Every subfamily of a sequence is a sequence, called a *subsequence* of the given sequence.

Two sequences $(x_n)_{n\in\mathrm{I}}$, $(y_n)_{n\in\mathrm{I}}$ with the same index set are said to *differ only in the order of their terms* if there exists a permutation $f$ of the index set I such that $x_{f(n)} = y_n$ for all $n \in \mathrm{I}$.

A *multiple sequence* is a family whose index set is a subset of a product $\mathbf{N}^p$ ($p$ an integer) ("double sequence" for $p = 2$, "triple sequence" for $p = 3$, and so on).

Let I be a set equipotent to $\mathbf{N}$ and let $f$ be a bijection of $\mathbf{N}$ onto I. For each family $(x_\iota)_{\iota\in\mathrm{I}}$ indexed by the set I, the sequence $n \to x_{f(n)}$ is said to be obtained by *arranging the family* $(x_\iota)_{\iota\in\mathrm{I}}$ *in the order defined by* $f$. The sequences which correspond in this way to two distinct bijections of $\mathbf{N}$ onto I differ only in the order of their terms. For a finite family indexed by a set I of $n$ elements we may similarly define a finite sequence with $[1, n]$ or $[0, n-1]$ as index set, by arranging the family in the order defined by a bijection of one or the other of these intervals onto I.

### 2. DEFINITION OF MAPPINGS BY INDUCTION

Since the set $\mathbf{N}$ is well-ordered, we may apply criterion C60 (§ 2, no. 2), which now takes the following form (with the same notation) :

C62. *Let $u$ be a letter and let* $\mathrm{T}\{u\}$ *be a term. Then there exists a set* U *and a mapping $f$ of* $\mathbf{N}$ *onto* U *such that for each integer $n$ we have* $f(n) = \mathrm{T}\{f^{(n)}\}$, *where $f^{(n)}$ denotes the mapping of* $[0, n[$ *onto* $f([0, n[)$ *which agrees with $f$ on* $[0, n[$. *Moreover, the set* U *and the mapping $f$ are uniquely determined by this condition.*

We shall deduce from this the following criterion :

C63. *Let* $S\{v\}$ *and* $a$ *be two terms. Then there exists a set* $V$ *and a mapping* $f$ *of* $\mathbf{N}$ *onto* $V$ *such that* $f(0) = a$ *and* $f(n) = S\{f(n-1)\}$ *for each integer* $n \geqslant 1$. *Moreover, the set* $V$ *and the mapping* $f$ *are uniquely determined by these conditions.*

To deduce C63 from C62 [^1], let

$$D(u) = \mathcal{E}_x(x \in \mathbf{N} \ \text{and} \ (\exists y)((x, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))))$$

for each letter $u$. If $u$ is a mapping of a subset of $\mathbf{N}$ into a set, then $D(u)$ is just the domain of $u$ (Chapter II, § 3, no. 1). Let $M(u)$ be the least upper bound of $D(u)$ in $\mathbf{N}$ [^2]. Let $\varphi$ be the empty mapping, with $\emptyset$ as source and target, i.e. (Chapter II, § 3, nos. 1 and 4), the triple $(\emptyset, \emptyset, \emptyset))$ and consider the relation

$$(u = \varphi \ \text{and} \ y = a) \ \text{or} \ (u \neq \varphi \ \text{and} \ y = S\{u(M(u))\})$$

which we denote by $R\{y, u\}$ ; finally, let $T\{u\}$ be the term $\tau_y(R\{y, u\})$. Apply C62 to the term $T\{u\}$. Since $f^{(0)}$ is equal to $\varphi$, we have $T\{f^{(0)}\} = a$; hence $f(0) = a$. If on the other hand $n > 0$, we have $D(f^{(n)}) = [0, n-1]$ and $M(f^{(n)}) = n-1$, whence

$$T\{f^{(n)}\} = S\{f^{(n)}(n-1)\} = S\{f(n-1)\}.$$

*Examples*

#### Example 1 {#ens-iii-s6-n2-exa-1 .statement tag=03TC}

Suppose that $a$ is an element of a set $E$ and that $S\{u\}$ is the term $g(u)$, where $g$ is a mapping of $E$ into itself [^3]. Then it is immediately seen by induction on $n$ that for all $n \in \mathbf{N}$ we have $f(n) \in E$; consequently $f$ is a mapping of $\mathbf{N}$ into $E$ such that $f(0) = a$ and $f(n+1) = g(f(n))$ for all integers $n$.

Likewise, let $h$ be a mapping of $\mathbf{N} \times E$ into $E$, and let $\psi$ be the mapping of $\mathbf{N} \times E$ into itself defined by $\psi(n, x) = (n+1, h(n, x))$. By the preceding discussion there exists a unique mapping $g = (\theta, f)$ of $\mathbf{N}$ into $\mathbf{N} \times E$ such that $g(0) = (0, a)$ and $g(n+1) = \psi(g(n))$ for all $n$, from which follows the existence and uniqueness of a mapping $f$

of $\mathbf{N}$ into E such that $f(0) = a$ and $f(n + 1) = h(n, f(n))$ for each integer $n$.

#### Example 2 {#ens-iii-s6-n2-exa-2 .statement tag=03TD}

Let X be a set and let E be the set of mappings of X into itself. Let $e$ denote the identity mapping of X into itself, and let $f$ be any element of E. Take $S\{u\}$ to be the term $f \circ u$ (*)[^4]. By applying C63 we see that there exists a unique mapping of $\mathbf{N}$ into E, denoted by $n \to f^n$, such that $f^0 = e$ and $f^{n+1} = f \circ f^n$. The mapping $f^n$ is called the *nth iterate* of the mapping $f$.

#### Example 3 {#ens-iii-s6-n2-exa-3 .statement tag=03TE}

If we take $S\{u\}$ to be the term $\mathfrak{P}(u)$, and $a$ to be a set E, it follows likewise that there exists a mapping, denoted by $n \to \mathfrak{P}^n(\mathrm{E})$, of $\mathbf{N}$ into a set V(E) such that $\mathfrak{P}^0(\mathrm{E}) = \mathrm{E}$, $\mathfrak{P}^1(\mathrm{E}) = \mathfrak{P}(\mathrm{E})$, and $\mathfrak{P}^{n+1}(\mathrm{E}) = \mathfrak{P}(\mathfrak{P}^n(\mathrm{E}))$ for every integer $n$.

#### Remark {#ens-iii-s6-n2-rem-1 .statement tag=03MY}

Let E be a set, let A be a subset of E, let $g$ be a mapping of A into E, and let $a$ be an element of A. Take $S\{u\}$ to be the term $g(u)$. Criterion C63 is applicable and proves the existence of a mapping $f$ of $\mathbf{N}$ onto a set V such that $f(0) = a$ and $f(n + 1) = g(f(n))$ for every integer $n$. It may happen that $\mathrm{V} \subset \mathrm{A}$; if not, let $p$ be the largest integer such that $f([0, p]) \subset \mathrm{A}$. Then $f(p + 1) = g(p) \notin \mathrm{A}$, and $g(g(p))$ is a term about which nothing can be said. Hence in this case $f$ is considered to be defined only on the interval $[0, p + 1]$ ("restricted induction").

### 3. PROPERTIES OF INFINITE CARDINALS

#### Theorem 2 {#ens-iii-s6-thm-2 .statement tag=03MZ}

*For every infinite cardinal $\mathfrak{a}$ we have $\mathfrak{a}^2 = \mathfrak{a}$.*

We shall use the following two lemmas :

#### Lemma 1 {#ens-iii-s6-lem-1 .statement tag=03N0}

*Every infinite set E contains a set equipotent to $\mathbf{N}$.*

There exists a well-ordering relation on E (§ 2, no. 3, Theorem 1), which we shall denote by $x \leqslant y$. The hypothesis implies that the well-ordered set E cannot be isomorphic to a segment of $\mathbf{N}$ distinct from $\mathbf{N}$, for such a segment is of the form $[0, n]$ (§ 2, no. 1, Proposition 1) and is therefore finite. It follows that $\mathbf{N}$ is isomorphic to a segment of E (§ 2, no. 3, Theorem 3), whence the result.

#### Lemma 2 {#ens-iii-s6-lem-2 .statement tag=03N1}

*The set $\mathbf{N} \times \mathbf{N}$ is equipotent to $\mathbf{N}$.*

Since $\mathbf{N} \times \mathbf{N}$ contains the set $\{0\} \times \mathbf{N}$, which is equipotent to $\mathbf{N}$, we have $\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathbf{N} \times \mathbf{N})$. To complete the proof it is enough to define an injection $f$ of $\mathbf{N} \times \mathbf{N}$ into $\mathbf{N}$. For this purpose we note that

there exists an injection $\varphi$ of $\mathbf{N}$ into the set of mappings of $\mathbf{N}$ into $\mathrm{I} = \{0, 1\}$, obtained as follows : if $r$ is the least integer such that $n > 2^r$, and if $\sum_{k=0}^{r-1} \varepsilon_k 2^{r-k-1}$ is the dyadic expansion of $n$ (§ 5, no. 7), $\varphi(n)$ is defined to be the sequence $(u_m)_{m \in \mathbf{N}}$ such that $u_m = \varepsilon_{r-m-1}$ for $m < r$ and $u_m = 0$ for $m \geqslant r$. Proposition 8 of § 5, no. 7 shows that $\varphi$ is injective. For each pair $(n, n') \in \mathbf{N} \times \mathbf{N}$ we define $f(n, n')$ as follows : if $\varphi(n) = (u_m)$ and $\varphi(n') = (v_m)$, let $f(n, \; n')$ be the integer $s$ such that $\varphi(s) = w_m$, where $w_{2m} = u_m$ and $w_{2m+1} = v_m$ for all $m \in \mathbf{N}$. It is clear that the relation $f(n, \; n') = f(n_1, \; n_1')$ implies $\varphi(n) = \varphi(n_1)$ and $\varphi(n') = \varphi(n_1')$; hence $(n, n') = (n_1, n_1')$, and therefore $f$ is injective.

¶ We come now to the proof of Theorem 2. Let E be a set such that $\mathrm{Card}(\mathrm{E}) = \mathfrak{a}$. Let D be a subset of E equipotent to $\mathbf{N}$ (Lemma 1). Then there exists a bijection $\psi_0$ of D onto $\mathrm{D} \times \mathrm{D}$ (Lemma 2). Let $\mathfrak{M}$ be the set of pairs $(\mathrm{X}, \psi)$, where X is a subset of E containing D and $\psi$ is a bijection of X onto $\mathrm{X} \times \mathrm{X}$ which extends $\psi_0$. Order the set $\mathfrak{M}$ by means of the relation

$$\text{``} \mathrm{X} \subset \mathrm{X}' \text{ and } \psi' \text{ is an extension of } \psi \text{''}$$

between $(\mathrm{X}, \psi)$ and $(\mathrm{X}', \psi')$. Then it is immediately seen that $\mathfrak{M}$ is *inductive* (cf. § 2, no. 4, Example 2). Hence, by Zorn's Lemma (§ 2, no. 4, Theorem 2), $\mathfrak{M}$ has a maximal element $(\mathrm{F}, f)$. We shall show that $\mathrm{Card}\,(\mathrm{F}) = \mathfrak{a}$, which will suffice to prove the theorem. If $\mathrm{Card}\,(\mathrm{F})$ is not equal to $\mathfrak{a}$, let $\mathrm{Card}\,(\mathrm{F}) = \mathfrak{b} < \mathfrak{a}$. Then $\mathfrak{b} = \mathfrak{b}^2$ and $\mathfrak{b}$ is infinite, and $\mathfrak{b} \leqslant 2\mathfrak{b} \leqslant 3\mathfrak{b} \leqslant \mathfrak{b}^2 = \mathfrak{b}$ (§ 3, no. 6, Proposition 14); hence $2\mathfrak{b} = \mathfrak{b}$ and $3\mathfrak{b} = \mathfrak{b}$. From the hypothesis $\mathfrak{b} < \mathfrak{a}$ it follows that $\mathrm{Card}\,(\mathrm{E} - \mathrm{F}) > \mathfrak{b}$, for otherwise we should have $\mathrm{Card}\,(\mathrm{E}) \leqslant 2\mathfrak{b} = \mathfrak{b}$, and we have assumed that $\mathfrak{b} < \mathrm{Card}\,(\mathrm{E})$. Hence there is a subset $\mathrm{Y} \subset \mathrm{E} - \mathrm{F}$ equipotent to F. Let $\mathrm{Z} = \mathrm{F} \cup \mathrm{Y}$; we shall show that there exists a bijection $g$ of Z onto $\mathrm{Z} \times \mathrm{Z}$ which extends $f$. We have

$$\mathrm{Z} \times \mathrm{Z} = (\mathrm{F} \times \mathrm{F}) \cup (\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y}),$$

and the four products on the right-hand side are mutually disjoint. Since F and Y are equipotent, we have

$$\mathrm{Card}(\mathrm{F} \times \mathrm{Y}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{F}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{Y}) = \mathfrak{b}^2 = \mathfrak{b},$$

whence

$$\mathrm{Card}((\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y})) = 3\mathfrak{b} = \mathfrak{b}.$$

There is therefore a bijection $f_1$ of Y onto the set

$$(\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y});$$

the mapping $g$ of Z into Z $\times$ Z, which is equal to $f$ on F and to $f_1$ on Y, is therefore a bijection which extends $f$, contrary to the definition of $f$. Hence $\mathrm{Card}(\mathrm{F}) = \mathfrak{a}$, and the proof is complete.

#### Corollary 1 {#ens-iii-s6-lem-2-cor-1 .statement tag=03N2}

*If $\mathfrak{a}$ is an infinite cardinal, then $\mathfrak{a}^n = \mathfrak{a}$ for every integer $n \geqslant 1$.*

By induction on $n$.

#### Corollary 2 {#ens-iii-s6-lem-2-cor-2 .statement tag=03N3}

*The product of a finite family $(\mathfrak{a}_i)_{i \in \mathrm{I}}$ of non-zero cardinals, of which the greatest is an infinite cardinal $\mathfrak{a}$, is equal to $\mathfrak{a}$.*

Let $\mathfrak{b}$ denote the product and let $n$ be the number of elements in I. Then $\mathfrak{b} \leqslant \mathfrak{a}^n = \mathfrak{a}$ (§ 3, no. 6, Proposition 14). On the other hand, since $\mathfrak{a}_i \geqslant 1$ for all $i \in \mathrm{I}$, we have $\mathfrak{b} \geqslant \mathfrak{a}$ (§ 3, no. 6, Proposition 14).

#### Corollary 3 {#ens-iii-s6-lem-2-cor-3 .statement tag=03N4}

*Let $\mathfrak{a}$ be an infinite cardinal and let $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ be a family of cardinals $\leqslant \mathfrak{a}$ whose index set I has a cardinal $\leqslant \mathfrak{a}$. Then $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}$; and if $\mathfrak{a}_\iota = \mathfrak{a}$ for at least one index $\iota \in \mathrm{I}$, then $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathfrak{a}$.*

Let $\mathfrak{b}$ be the cardinal of I; then we have $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}\mathfrak{b} \leqslant \mathfrak{a}^2 = \mathfrak{a}$ (§ 3, no. 6, Proposition 14), and $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \geqslant \mathfrak{a}_\varkappa$ for all $\varkappa \in \mathrm{I}$.

#### Corollary 4 {#ens-iii-s6-lem-2-cor-4 .statement tag=03N5}

*If $\mathfrak{a}$ and $\mathfrak{b}$ are two non-zero cardinals, one of which is infinite, we have $\mathfrak{a}\mathfrak{b} = \mathfrak{a} + \mathfrak{b} = \sup\,(\mathfrak{a},\,\mathfrak{b})$.*

This follows directly from Corollaries 2 and 3.

### 4. COUNTABLE SETS

#### Definition 3 {#ens-iii-s6-def-3 .statement tag=03N6}

*A set is said to be countable if it is equipotent to a subset of the set $\mathbf{N}$ of integers.*

#### Proposition 1 {#ens-iii-s6-prop-1 .statement tag=03N7}

*Every subset of a countable set is countable. The product of a finite family of countable sets is countable. The union of a sequence of countable sets is countable.*

The first assertion is obvious. The others follow from the Corollaries to Theorem 2, no. 3.

¶ We have proved (no. 3, Lemma 1) that if $\mathfrak{a}$ is any infinite cardinal, then $\mathrm{Card}(\mathbf{N}) \leqslant \mathfrak{a}$. This has the following consequences :

#### Proposition 2 {#ens-iii-s6-prop-2 .statement tag=03N8}

*Every countable infinite set E is equipotent to $\mathbf{N}$.*

For $\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathbf{N})$ by definition; and $\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathrm{E})$ since E is infinite.

#### Proposition 3 {#ens-iii-s6-prop-3 .statement tag=03N9}

*Every infinite set has a partition* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *formed of countable infinite sets* $\mathrm{X}_\iota$, *the index set* I *being equipotent to* E.

For $\mathrm{Card}(\mathrm{E}) = \mathrm{Card}(\mathrm{E})\ \mathrm{Card}(\mathbf{N})$ (no. 3, Theorem 2, Corollary 4).

#### Proposition 4 {#ens-iii-s6-prop-4 .statement tag=03NA}

*Let* $f$ *be a mapping of a set* E *onto an infinite set* F *such that, for each* $y \in \mathrm{F}$, $\overset{-1}{f}(y)$ *is countable. Then* F *is equipotent to* E.

For the sets $\overset{-1}{f}(y)$ $(y \in \mathrm{F})$ form a partition of E; hence

$$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathrm{F})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{F}),$$

and $\mathrm{Card}(\mathrm{F}) \leqslant \mathrm{Card}(\mathrm{E})$ by Proposition 3 of § 3, no. 2.

#### Proposition 5 {#ens-iii-s6-prop-5 .statement tag=03NB}

*The set* $\mathfrak{F}(\mathrm{E})$ *of finite subsets of an infinite set* E *is equipotent to* E.

For each integer $n$, let $\mathfrak{F}_n$ denote the set of subsets of E which have $n$ elements. For each $\mathrm{X} \in \mathfrak{F}_n$ there exists a bijection of $[1, n]$ onto X. Hence the cardinal of $\mathfrak{F}_n$ is at most equal to that of the set of mappings of $[1, n]$ into E, i.e., to $\mathrm{Card}(\mathrm{E}^n) = \mathrm{Card}(\mathrm{E})$ (no. 3, Theorem 2, Corollary 1). Therefore

$$\mathrm{Card}(\mathfrak{F}(\mathrm{E})) = \sum_{n \in \mathbf{N}} \mathrm{Card}(\mathfrak{F}_n) \leqslant \mathrm{Card}(\mathrm{E})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{E}).$$

On the other hand, since $x \to \{x\}$ is an injective mapping of E into $\mathfrak{F}(\mathrm{E})$, we have $\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathfrak{F}(\mathrm{E}))$.

#### Definition 4 {#ens-iii-s6-def-4 .statement tag=03NC}

*A set is said to have the power of the continuum if it is equipotent to the set of all subsets of* $\mathbf{N}$.

A set which has the power of the continuum is not countable (§ 3, no. 6, Theorem 2).

\* The name "power of the continuum" arises from the fact that the set of real numbers is equipotent to $\mathfrak{P}(\mathbf{N})$ (*General Topology*, Chapter IV, § 8). ⁎ The *continuum hypothesis* is the assertion that every uncountable set contains a subset which has the power of the continuum; the *generalized continuum hypothesis* is the assertion that, for every infinite cardinal $\mathfrak{a}$, every cardinal $> \mathfrak{a}$ is $\geqslant 2^{\mathfrak{a}}$.

### 5. STATIONARY SEQUENCES

#### Definition 5 {#ens-iii-s6-def-5 .statement tag=03ND}

*A sequence* $(x_n)_{n \in \mathbf{N}}$ *of elements of a set* E *is said to be stationary if there exists an integer* $m$ *such that* $x_n = x_m$ *for all integers* $n \geqslant m$.

#### Proposition 6 {#ens-iii-s6-prop-6 .statement tag=03NE}

*Let* E *be an ordered set. Then the following statements are equivalent :*

(a) *Every non-empty subset of* E *has a maximal element.*
(b) *Every increasing sequence* $(x_n)$ *of elements of* E *is stationary.*

We show first that (a) implies (b). Let X be the set of elements of the sequence $(x_n)$, and let $x_m$ be a maximal element of X. If $n \geqslant m$, we have by hypothesis $x_n \geqslant x_m$, and therefore $x_n = x_m$ by the maximality of $x_m$. Conversely, suppose that there exists a non-empty subset A of E which has no maximal element. For each $x \in A$, let $T_x$ be the set of all $y \in A$ such that $y > x$. By assumption, $T_x \neq \emptyset$ for all $x \in A$; hence there exists a mapping $f$ of A into A such that $f(x) > x$ for all $x \in A$ (Chapter II, § 5, no. 4, Proposition 6). If $a \in A$, then the sequence $(x_n)_{n \in \mathbf{N}}$ defined inductively by the conditions $x_0 = a$, $x_{n+1} = f(x_n)$ is evidently increasing and not stationary.

#### Corollary 1 {#ens-iii-s6-prop-6-cor-1 .statement tag=03NF}

*A totally ordered set* E *is well-ordered if and only if every decreasing sequence of elements of* E *is stationary.*

For to say that E is well-ordered is equivalent to saying that every non-empty subset of E has a minimal element (§ 1, no. 10, Proposition 10), and the assertion therefore follows from Proposition 6.

#### Corollary 2 {#ens-iii-s6-prop-6-cor-2 .statement tag=03NG}

*Every increasing sequence of elements of a finite ordered set is stationary.*

For every finite ordered set has a maximal element (§ 4, no. 4, Proposition 3, Corollary 2).

¶ An ordered set E which satisfies the equivalent conditions of Proposition 6 is sometimes said to be *Noetherian*.

#### Proposition 7 ("Principle of Noetherian induction") {#ens-iii-s6-prop-7 .statement tag=03RM}

— *Let* E *be a Noetherian set, and let* F *be a subset of* E *with the following property : if* $a \in E$ *is such that the relation* $x > a$ *implies* $x \in F$, *then* $a \in F$. *Under these conditions,* F $=$ E.

Indeed, suppose E $\neq$ F; then E $-$ F has a maximal element $b$. By definition we have $x \in F$ for all $x > b$; but this implies $b \in F$, which is absurd.

### Exercises {#ens-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).

[^1]: (*) It is also possible to give a direct proof of C63, analogous to the proof of C60 (§ 2, no. 2).
[^2]: (†) The definition of the least upper bound (§ 1, nos. 7, 8, and 9) can be formulated in such a way that it has a meaning even for a set which is not bounded above (it denotes a term, in the formalized language, of the form $\tau_x(R\{x\})$, which the reader will have no difficulty in writing down).
[^3]: (**) If $g = (G, E, E)$, the term $g(u)$ is the term denoted by $\tau_y((u, y) \in G)$.
[^4]: (*) Here we mean the term denoted by (T, X, X), where T is the term denoted by $\mathfrak{S}_z(z$ is an ordered pair and $(\exists y)((\mathrm{pr}_1 z, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))$ and $(y, \mathrm{pr}_2 z) \in \mathrm{pr}_1(\mathrm{pr}_1(f)))$.
