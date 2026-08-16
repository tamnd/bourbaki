---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 3
section_title: Equipotent sets. Cardinals
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 157-165, 229-230
pdf_pages: 0163-0171, 0235-0236
extraction: ocr
subsections:
    - "no": 1
      title: THE CARDINAL OF A SET
      page: 157
      pdf_page: 163
    - "no": 2
      title: ORDER RELATION BETWEEN CARDINALS
      page: 158
      pdf_page: 164
    - "no": 3
      title: OPERATIONS ON CARDINALS
      page: 160
      pdf_page: 166
    - "no": 4
      title: PROPERTIES OF THE CARDINALS 0 AND 1
      page: 162
      pdf_page: 168
    - "no": 5
      title: EXPONENTIATION OF CARDINALS
      page: 163
      pdf_page: 169
    - "no": 6
      title: ORDER RELATION AND OPERATIONS ON CARDINALS
      page: 164
      pdf_page: 170
statements: 37
exercises: 6
errata:
    - says: § 5, no. 4, Proposition 5, Corollary 2
      read: § 5, no. 4, Proposition 6, Corollary 2
      why: The sentence on page 157 is a translation of the condition that a product set should be non-empty, which is Corollary 2 of no. 4 of § 5 of chapter II. The five corollaries of that no. are printed under Proposition 6 and the volume names them under Proposition 5 here as it does three times in chapter II itself.
    - says: § 6, no. 3, Theorem 3
      read: § 6, no. 3, Theorem 2
      why: Section 6 has no Theorem 3. No. 3 prints Theorem 2 on page 186, then Lemma 1 and Lemma 2, then the proof of Theorem 2 on page 187, then four corollaries on page 188. The Corollary 4 this sentence cites with it is the one that puts the product of two cardinals, one of them infinite, at their supremum, which is Corollary 4 of Theorem 2 and is what the sentence is about.
content_sha256: 155ceb1fa79c2e2f92adc39b2358178220f94a8b40cabc2c2895bcd17ab7ece2
---

## 3. EQUIPOTENT SETS. CARDINALS

### 1. THE CARDINAL OF A SET

#### Definition 1 {#ens-iii-s3-def-1 .statement tag=03QU}

A set $X$ is *said to be equipotent to a set $Y$ if there exists a bijection of $X$ onto $Y$. The relation “$X$ is equipotent to $Y$” is denoted by $\operatorname{Eq}(X,Y)$.

The relations $\operatorname{Eq}(X,Y)$ and $\operatorname{Eq}(Y,X)$ are clearly equivalent, so that the relation $\operatorname{Eq}(X,Y)$ is *symmetric*; when it is true, we say that $X$ and $Y$ are *equipotent*. Next, $\operatorname{Eq}(X,X)$ is true. Finally, the relation $\operatorname{Eq}(X,Y)$ is *transitive* since the composition of two bijections is a bijection (Chapter II, § 3, no. 8, Theorem 1); it is therefore an *equivalence relation*, reflexive on every set.

¶ From what has been said it follows that if $X$ and $Y$ are equipotent, the relation

$$
(\forall Z)(\operatorname{Eq}(X,Z)\Longleftrightarrow\operatorname{Eq}(Y,Z))
$$

is true. Now the axiom scheme S7 (Chapter I, § 5, no. 1) gives us the following axiom :

$$
((\forall Z)(\operatorname{Eq}(X,Z)\Longleftrightarrow\operatorname{Eq}(Y,Z))\Longrightarrow(\tau_Z(\operatorname{Eq}(X,Z))=\tau_Z(\operatorname{Eq}(Y,Z))).
$$

Hence, if X and Y are equipotent, we have

$$\tau_Z(\mathrm{Eq}(X, Z)) = \tau_Z(\mathrm{Eq}(Y, Z)),$$

which justifies the following definition :

#### Definition 2 {#ens-iii-s3-def-2 .statement tag=03QV}

*The set* $\tau_Z(\mathrm{Eq}(X, Z))$ *is called the cardinal of* X (or the *power* of X) *and is written* $\mathrm{Card}(X)$.

Since $\mathrm{Eq}(X, X)$ is true, $\mathrm{Card}(X)$ is *equipotent* to X (Chapter I, § 4, Scheme S5). We have therefore proved the following result :

#### Proposition 1 {#ens-iii-s3-prop-1 .statement tag=03QW}

*Two sets* X *and* Y *are equipotent if and only if their cardinals are equal.*

*Examples*

#### Example 1 {#ens-iii-s3-n1-exa-1 .statement tag=03T5}

$\mathrm{Card}(\emptyset)$ is denoted by 0. Since the only set equipotent to $\emptyset$ is $\emptyset$ (Chapter II, § 3, nos. 1 and 4), we have $0 = \mathrm{Card}(\emptyset) = \emptyset$.

#### Example 2 {#ens-iii-s3-n1-exa-2 .statement tag=03T6}

All sets consisting of a single element are equipotent, since $\{(a, b)\}$ is the graph of a bijection of $\{a\}$ onto $\{b\}$; in particular, they are all equipotent to $\{\emptyset\}$. The cardinal $\mathrm{Card}(\{\emptyset\}) = \tau_Z(\mathrm{Eq}(\{\emptyset\}, Z))$ is denoted by 1. [^1]

#### Example 3 {#ens-iii-s3-n1-exa-3 .statement tag=03T7}

$\mathrm{Card}(\{\emptyset, \{\emptyset\}\})$ is denoted by 2; this is the cardinal of every set consisting of two distinct elements.

#### Example 4 {#ens-iii-s3-n1-exa-4 .statement tag=03T8}

A Hilbert space of countable type is equipotent to the set of real numbers. *

### 2. ORDER RELATION BETWEEN CARDINALS

The relation "X is equipotent to a subset of Y" is equivalent to "there exists an injection of X into Y"; it is also equivalent to the relation "Card (X) is equipotent to a subset of Card (Y)" (Chapter II, § 3, no. 8, Theorem 1).

#### Theorem 1 {#ens-iii-s3-thm-1 .statement tag=03QX}

*The relation $R\{\xi,\eta\}$: “$\xi$ and $\eta$ are cardinals and $\xi$ is equipotent to a subset of $\eta$” is a well-ordering relation (§ 2, no. 1).*

Since $R\{\xi,\xi\}$ is true for every cardinal $\xi$, what must be proved is that, for every set E of cardinals the relation “$\xi\in E$ and $\eta\in E$ and $R\{\xi,\eta\}$” is a well-ordering relation on E. Consider the set $A=\bigcup_{\xi\in E}\xi$.

Every cardinal $\xi\in E$ is then a subset of A. By § 2, Theorem 1 there exists a well-ordering relation on A, which we shall denote by $\xi\leq\eta$, and every subset of A is equipotent to a segment of A (§ 2, no. 5, Theorem 3, Corollary x). For every cardinal $\xi\in E$ consider the set of segments of A which are equipotent to $\xi$; this set of segments is not empty and therefore has a least element (§ 2, no. 1, Proposition 2); let $\varphi(\xi)$ denote this least element. The relation

“$\xi\in E$ and $\eta\in E$ and $\xi$ is equipotent to a subset of $\eta$”

is then *equivalent* to

“$\xi\in E$ and $\eta\in E$ and $\varphi(\xi)\subset\varphi(\eta)$”.

For clearly the second relation implies the first. Conversely, if $\xi$ is equipotent to a subset of $\varphi(\eta)$, we cannot have $\varphi(\eta)\subset\varphi(\xi)$ and $\varphi(\eta)\neq\varphi(\xi)$; otherwise there would exist a segment of $\varphi(\eta)$ equipotent to $\xi$ (§ 2, no. 5, Theorem 3, Corollary 3), contrary to the definition of $\varphi(\xi)$. Since the set of segments of A is well-ordered by inclusion (§ 2, no. 1, Proposition 2), the theorem follows.

¶ We shall denote the relation $R\{\xi,\eta\}$ by $\xi\leq\eta$. A set X is equipotent to a subset of a set Y if and only if $\operatorname{Card}(X)\leq\operatorname{Card}(Y)$.

Clearly we have $0\leq\xi$ for every cardinal $\xi$, and $1\leq\xi$ for every cardinal $\xi\neq0$.

#### Corollary 1 {#ens-iii-s3-thm-1-cor-1 .statement tag=03QY}

*Given any two sets, one of them is equipotent to a subset of the other.*

#### Corollary 2 {#ens-iii-s3-thm-1-cor-2 .statement tag=03QZ}

*Two sets each of which is equipotent to a subset of the other are equipotent.*

#### Remark {#ens-iii-s3-n2-rem-1 .statement tag=03R0}

Given any set A, there exists a set whose elements are the cardinals $\operatorname{Card}(X)$ for all the subsets X of A, namely, the set of objects of the form $\operatorname{Card}(X)$ for $X\in\mathfrak{P}(A)$ (Chapter II, § 1, no. 6). For every cardinal $\alpha$ the relation “$\xi$ is a cardinal and $\xi\leq\alpha$” is therefore collectivizing in $\xi$ (Chapter II, § 1, no. 4), because it is equivalent to the

relation "$\mathfrak{x}$ is of the form Card (X) for $X \subset \mathfrak{a}$"; the set of all $\mathfrak{x}$ satisfying this relation is called the *set of cardinals* $\leqslant \mathfrak{a}$.

#### Proposition 2 {#ens-iii-s3-prop-2 .statement tag=03KL}

*For every family* $(\mathfrak{a}_\iota)_{\iota \in I}$ *of cardinals, there exists a unique cardinal* $\mathfrak{b}$ *such that* $\mathfrak{a}_\iota \leqslant \mathfrak{b}$ *for all* $\iota \in I$ *and such that every cardinal* $\mathfrak{c}$ *for which* $\mathfrak{a}_\iota \leqslant \mathfrak{c}$ *for all* $\iota \in I$ *is* $\geqslant \mathfrak{b}$.

There exists a set E containing all the sets $\mathfrak{a}_\iota$ (e.g., the sum of these sets (Chapter II, § 4, no. 8)), whence $\mathfrak{a}_\iota \leqslant \mathfrak{a} = $ Card (E) for all $\iota \in I$. The set F of cardinals $\leqslant \mathfrak{a}$ is well-ordered and contains all the $\mathfrak{a}_\iota$, and therefore the family $(\mathfrak{a}_\iota)_{\iota \in I}$ has a least upper bound $\mathfrak{b}$ in F. Let $\mathfrak{c}$ be a cardinal $\geqslant \mathfrak{a}_\iota$ for all $\iota \in I$; if $\mathfrak{c} < \mathfrak{b} \leqslant \mathfrak{a}$, then $\mathfrak{c} \in F$, and the inequality $\mathfrak{a}_\iota \leqslant \mathfrak{c}$ contradicts the definition of the least upper bound of the family $(\mathfrak{a}_\iota)$ in the ordered set F; hence the result.

¶ By abuse of language, the cardinal $\mathfrak{b}$ is called the *least upper bound* of the family $(\mathfrak{a}_\iota)_{\iota \in I}$ and is denoted by $\sup_{\iota \in I} \mathfrak{a}_\iota$.

#### Proposition 3 {#ens-iii-s3-prop-3 .statement tag=03KM}

*Let* X *and* Y *be sets. If there exists a surjection $f$ of* X *onto* Y, *then* Card (Y) $\leqslant$ Card (X).

For there exists a section $s$ associated with $f$ (Chapter II, § 3, no. 8, Proposition 8) and $s$ is an injection of Y into X.

### 3. OPERATIONS ON CARDINALS

#### Definition 3 {#ens-iii-s3-def-3 .statement tag=03KN}

*Let* $(\mathfrak{a}_\iota)_{\iota \in I}$ *be a family of cardinals. The cardinal of the product* (resp. *sum*) *of the sets* $\mathfrak{a}_\iota$ *is called the cardinal product* (resp. *cardinal sum*) *of the cardinals* $\mathfrak{a}_\iota$ *and is denoted by* $\mathop{\mathbf{P}}_{\iota \in I} \mathfrak{a}_\iota$ $\left(\text{resp. } \sum_{\iota \in I} \mathfrak{a}_\iota\right)$.

Whenever there is no risk of confusion we shall say simply "product" and "sum" in place of "cardinal product" and "cardinal sum", and we shall write $\prod_{\iota \in I} \mathfrak{a}_\iota$ in place of $\mathop{\mathbf{P}}_{\iota \in I} \mathfrak{a}_\iota$ (cf. Exercise 2).

#### Proposition 4 {#ens-iii-s3-prop-4 .statement tag=03KO}

*Let* $(E_\iota)_{\iota \in I}$ *be a family of sets,* P *their product, and* S *their sum, and let* $\mathfrak{a}_\iota$ *be the cardinal of* $E_\iota$. *Then the cardinal of* P (resp. S) *is the cardinal product* (resp. *cardinal sum*) *of the family* $(\mathfrak{a}_\iota)_{\iota \in I}$.

For there exists a bijection of P (resp. S) onto the product (resp. sum) of the sets $(\mathfrak{a}_\iota)$ (Chapter II, § 4, no. 8, Proposition 10, and § 5, no. 7, Corollary to Proposition 11).

#### Corollary {#ens-iii-s3-n3-cor-1 .statement tag=03KP}

*If* $(E_\iota)_{\iota \in I}$ *is any family of sets, the cardinal of the union* $\bigcup_{\iota \in I} E_\iota$ *is at most equal to the sum* $\sum_{\iota \in I}$ Card $(E_\iota)$.

For there exists a mapping of the sum S of the $\mathrm{E}_\iota$ onto the union of the $\mathrm{E}_\iota$ (Chapter II, § 4, no. 8); the Corollary therefore follows from Propositions 3 and 4.

#### Proposition 5 {#ens-iii-s3-prop-5 .statement tag=03R1}

(a) *Let* $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ *be a family of cardinals, and let f be a bijection of a set* K *onto the index set* I. *Then*

$$\sum_{x \in \mathrm{K}} \mathfrak{a}_{f(x)} = \sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota, \qquad \mathop{\mathrm{P}}_{x \in \mathrm{K}} \mathfrak{a}_{f(x)} = \mathop{\mathrm{P}}_{\iota \in \mathrm{I}} \mathfrak{a}_\iota.$$

(b) *Let* $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ *be a family of cardinals and let* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *be a partition of* I. *Then*

$$\sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \sum_{\lambda \in \mathrm{L}} \left( \sum_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_\iota \right), \qquad \mathop{\mathrm{P}}_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \left( \mathop{\mathrm{P}}_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_\iota \right)$$

("associativity of the sum and product").

(c) *Let* $((\mathfrak{a}_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda})_{\lambda \in \mathrm{L}}$ *be a family (indexed by* L) *of families of cardinals, and let* $\mathrm{I} = \coprod_{\lambda \in \mathrm{L}} \mathrm{J}_\lambda$. *Then*

$$\mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \left( \sum_{\iota \in \mathrm{J}_\lambda} \mathfrak{a}_{\lambda\iota} \right) \sum_{f \in \mathrm{I}} = \left( \mathop{\mathrm{P}}_{\lambda \in \mathrm{L}} \mathfrak{a}_{\lambda, f(\lambda)} \right)$$

("distributivity of product over sum").

The relations in (a) follow from the analogous formulae for the union and product of sets, for the fact that $f$ is a bijection implies that if $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is a family of mutually disjoint sets, the elements of the family $(\mathrm{X}_{f(x)})_{x \in \mathrm{K}}$ are also mutually disjoint (cf. Chapter II, § 4, no. 1, Proposition 1 and § 5, no. 3, Proposition 4).

¶ The relations in (b) are immediate consequences of the associativity formulae for unions and products (Chapter II, § 4, no. 2, Proposition 2 and § 5, no. 5, Proposition 7) and the distributivity of intersection over union (Chapter II, § 5, no. 6, Proposition 8), which shows that if $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is a family of mutually disjoint sets, then the elements of the family

$$\left( \bigcup_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota \right)_{\lambda \in \mathrm{L}}$$

are also mutually disjoint.

¶ Finally, (c) follows from the distributivity of the product over union and intersection (Chapter II, § 5, no. 6, Proposition 9 and Corollary 1).

¶ Let $\mathfrak{a}$ and $\mathfrak{b}$ be two cardinals. If I is a set consisting of two distinct elements (e.g., the cardinal 2), there exists a mapping $f$ of I onto $\{\mathfrak{a}, \mathfrak{b}\}$ which defines a family of cardinals. The sum and product of this family

depend only on $\mathfrak{a}$ and $\mathfrak{b}$ (by reason of Proposition 5(a)); these cardinals are called respectively the *sum* and the *product* of $\mathfrak{a}$ and $\mathfrak{b}$, and are denoted by $\mathfrak{a} + \mathfrak{b}$ and $\mathfrak{a}\mathfrak{b}$. Similarly for the sum and product of three or more cardinals. Proposition 5 then implies the following corollary :

#### Corollary {#ens-iii-s3-n3-cor-2 .statement tag=03R2}

*Let $\mathfrak{a}$, $\mathfrak{b}$, $\mathfrak{c}$ be cardinals. Then*

(1) $$\mathfrak{a} + \mathfrak{b} = \mathfrak{b} + \mathfrak{a}, \qquad \mathfrak{a}\mathfrak{b} = \mathfrak{b}\mathfrak{a};$$
(2) $$\mathfrak{a} + (\mathfrak{b} + \mathfrak{c}) = (\mathfrak{a} + \mathfrak{b}) + \mathfrak{c}, \qquad \mathfrak{a}(\mathfrak{b}\mathfrak{c}) = (\mathfrak{a}\mathfrak{b})\mathfrak{c};$$
(3) $$\mathfrak{a}(\mathfrak{b} + \mathfrak{c}) = \mathfrak{a}\mathfrak{b} + \mathfrak{a}\mathfrak{c}.$$

### 4. PROPERTIES OF THE CARDINALS 0 AND 1

#### Proposition 6 {#ens-iii-s3-prop-6 .statement tag=03R3}

*Let $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ be a family of cardinals, and let $\mathrm{J}$ (resp. $\mathrm{K}$) be a subset of $\mathrm{I}$ such that $\mathfrak{a}_\iota = 0$ for all $\iota \notin \mathrm{J}$ (resp. $\mathfrak{a}_\iota = 1$ for all $\iota \notin \mathrm{K}$). Then*

$$\sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \sum_{\iota \in \mathrm{J}} \mathfrak{a}_\iota \qquad \left(\text{resp. } \mathbf{P}_{\iota \in \mathrm{I}}\, \mathfrak{a}_\iota = \mathbf{P}_{\iota \in \mathrm{K}}\, \mathfrak{a}_\iota\right).$$

The proposition is obvious as regards the sum, for the sum $\mathrm{S}_\mathrm{I}$ of the family of sets $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ is equipotent to the union of the sum $\mathrm{S}_\mathrm{J}$ of the family $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ and the empty set, and hence equipotent to $\mathrm{S}_\mathrm{J}$. The assertion concerning products follows from the fact that the projection $\mathrm{pr}_\mathrm{K}$ of the product set $\prod_{\iota \in \mathrm{I}} \mathfrak{a}_\iota$ onto the partial product $\prod_{\iota \in \mathrm{K}} \mathfrak{a}_\iota$ is a bijection (Chapter II, § 5, no. 5, Remark 1).

#### Corollary 1 {#ens-iii-s3-prop-6-cor-1 .statement tag=03R4}

*For every cardinal $\mathfrak{a}$ we have $\mathfrak{a} + 0 = \mathfrak{a} . 1 = \mathfrak{a}$.*

#### Corollary 2 {#ens-iii-s3-prop-6-cor-2 .statement tag=03R5}

*Let $\mathfrak{a}$ and $\mathfrak{b}$ be cardinals and let $\mathrm{I}$ be a set equipotent to $\mathfrak{b}$. For each $\iota \in \mathrm{I}$ let $\mathfrak{a}_\iota = \mathfrak{a}$, $\mathfrak{c}_\iota = 1$. Then*

$$\mathfrak{a}\mathfrak{b} = \sum_{\iota \in \mathrm{I}} \mathfrak{a}_\iota, \qquad \mathfrak{b} = \sum_{\iota \in \mathrm{I}} \mathfrak{c}_\iota.$$

The second formula is a consequence of the fact that any set is the union of its one-element subsets. The first formula follows from the second by multiplying by $\mathfrak{a}$ and using Corollary 1.

#### Proposition 7 {#ens-iii-s3-prop-7 .statement tag=03R6}

*Let $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ be a family of cardinals. Then $\mathbf{P}_{\iota \in \mathrm{I}}\, \mathfrak{a}_\iota \neq 0$ if and only if $\mathfrak{a}_\iota \neq 0$ for all $\iota \in \mathrm{I}$.*

This is merely a translation of the condition that a product set should be non-empty (Chapter II, § 5, no. 4, Proposition 5, Corollary 2).

#### Proposition 8 {#ens-iii-s3-prop-8 .statement tag=03R7}

*If $\mathfrak{a}$ and $\mathfrak{b}$ are cardinals such that $\mathfrak{a} + 1 = \mathfrak{b} + 1$, then $\mathfrak{a} = \mathfrak{b}$.*

Let $X = \mathfrak{a} + 1 = \mathfrak{b} + 1$. Then there exist subsets A, B of X with cardinals $\mathfrak{a}$, $\mathfrak{b}$, respectively, such that the complements $X - A, X - B$ each consist of a single element. Let $u$, $v$ be these elements. The intersection $C = A \cap B$ has as complement in X the set $\{u, v\}$. If $u = v$, then $A = B = C$, so that $\mathfrak{a} = \mathfrak{b}$. If $u \neq v$, then $A = C \cup \{v\}$, $B = C \cup \{u\}$, and therefore $\mathfrak{a} = 1 + \mathrm{Card}\ (C) = \mathfrak{b}$.

☡

The reader should beware of assuming that $\mathfrak{a} + \mathfrak{m} = \mathfrak{b} + \mathfrak{m}$ implies $\mathfrak{a} = \mathfrak{b}$ for all cardinals $\mathfrak{m}$ (cf. § 6); \* we shall see later, however, that this implication is true if $\mathfrak{m}$ is *finite* (§ 5, no. 2, Proposition 3, Corollary 4 and § 6, no. 3, Theorem 3, Corollary 4). \*

### 5. EXPONENTIATION OF CARDINALS

#### Definition 4 {#ens-iii-s3-def-4 .statement tag=03KQ}

*Let $\mathfrak{a}$ and $\mathfrak{b}$ be cardinals. The cardinal of the set of mappings of $\mathfrak{b}$ into $\mathfrak{a}$ is denoted by $\mathfrak{a}^{\mathfrak{b}}$, by abuse of notation.*

The abuse of notation here lies in the the fact that $\mathfrak{a}^{\mathfrak{b}}$ already denotes the set of graphs of mappings of $\mathfrak{b}$ into $\mathfrak{a}$ (Chapter II, § 5, no. 3), and this set is not necessarily a cardinal (Exercise 2). It will always be clear from the context which meaning is to be attached to the symbol $\mathfrak{a}^{\mathfrak{b}}$.

#### Proposition 9 {#ens-iii-s3-prop-9 .statement tag=03KR}

*Let X and Y be two sets, $\mathfrak{a}$ and $\mathfrak{b}$ their respective cardinals. Then the set $X^{Y}$ has cardinal $\mathfrak{a}^{\mathfrak{b}}$.*

For there exists a bijection of $X^{Y}$ onto the set of mappings of $\mathfrak{b}$ into $\mathfrak{a}$ (Chapter II, § 5, no. 2, Proposition 2, Corollary).

#### Proposition 10 {#ens-iii-s3-prop-10 .statement tag=03KS}

*Let $\mathfrak{a}$ and $\mathfrak{b}$ be cardinals and let I be a set such that $\mathrm{Card}\ (I) = \mathfrak{b}$. If $\mathfrak{a}_{\iota} = \mathfrak{a}$ for all $\iota \in I$, we have $\mathfrak{a}^{\mathfrak{b}} = \mathbf{P}_{\iota \in I} \mathfrak{a}_{\iota}$.*

This follows from the definition of the product of a family of sets as a set of functional graphs (Chapter II, § 5, no. 3).

#### Corollary 1 {#ens-iii-s3-prop-10-cor-1 .statement tag=03KT}

*Let $\mathfrak{a}$ be a cardinal and let $(\mathfrak{b}_{\iota})_{\iota \in I}$ be a family of cardinals. Then*

$$\mathfrak{a}^{\sum_{\iota \in I} \mathfrak{b}_{\iota}} = \mathbf{P}_{\iota \in I} \mathfrak{a}^{\mathfrak{b}_{\iota}}.$$

Let S be the sum of the sets $\mathfrak{b}_{\iota}$, and put $\mathfrak{a}_{s} = \mathfrak{a}$ for all $s \in S$. Both sides of the equality to be proved are then equal to $\mathbf{P}_{s \in S} \mathfrak{a}_{s}$, by virtue of Proposition 10 and the associativity formula for products (no. 3, Proposition 5(b)).

#### Corollary 2 {#ens-iii-s3-prop-10-cor-2 .statement tag=03KU}

*Let $(\mathfrak{a}_\iota)_{\iota \in \mathbf{I}}$ be a family of cardinals and let $\mathfrak{b}$ be a cardinal. Then*
$$\left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota \right)^{\mathfrak{b}} = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota^{\mathfrak{b}}.$$

Let $\mathfrak{a}_{\iota\beta} = \mathfrak{a}_\iota$ for each pair $(\iota, \beta) \in \mathbf{I} \times \mathfrak{b}$. Then, by associativity of the product, we have
$$\left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota \right)^{\mathfrak{b}} = \mathop{\mathbf{P}}_{\beta \in \mathfrak{b}} \left( \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_{\iota\beta} \right) = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \left( \mathop{\mathbf{P}}_{\beta \in \mathfrak{b}} \mathfrak{a}_{\iota\beta} \right) = \mathop{\mathbf{P}}_{\iota \in \mathbf{I}} \mathfrak{a}_\iota^{\mathfrak{b}}.$$

#### Corollary 3 {#ens-iii-s3-prop-10-cor-3 .statement tag=03KV}

*Let $\mathfrak{a}$, $\mathfrak{b}$, $\mathfrak{c}$ be cardinals. Then $\mathfrak{a}^{\mathfrak{b}\mathfrak{c}} = (\mathfrak{a}^{\mathfrak{b}})^{\mathfrak{c}}$.*

Let $\mathfrak{b}_\gamma = \mathfrak{b}$ for all $\gamma \in \mathfrak{c}$. Then
$$\mathfrak{a}^{\mathfrak{b}\mathfrak{c}} = \mathfrak{a}^{\sum\limits_{\gamma \in \mathfrak{c}} \mathfrak{b}_\gamma} = \mathop{\mathbf{P}}_{\gamma \in \mathfrak{c}} \mathfrak{a}^{\mathfrak{b}_\gamma} = (\mathfrak{a}^{\mathfrak{b}})^{\mathfrak{c}}$$
by virtue of Corollary 1.

#### Proposition 11 {#ens-iii-s3-prop-11 .statement tag=03KW}

*Let $\mathfrak{a}$ be a cardinal. Then $\mathfrak{a}^0 = 1$, $\mathfrak{a}^1 = \mathfrak{a}$, $1^{\mathfrak{a}} = 1$; and $0^{\mathfrak{a}} = 0$ if $\mathfrak{a} \neq 0$.*

For there exists a unique mapping of $\varnothing$ into any given set (namely, the mapping whose graph is the empty set); the set of mappings of a set consisting of a single element into an arbitrary set X is equipotent to X (Chapter II, § 5, no. 3); there exists a unique mapping of an arbitrary set into a set consisting of a single element; and, finally, there is no mapping of a non-empty set into $\varnothing$.

¶ Note in particular that $0^0 = 1$.

#### Proposition 12 {#ens-iii-s3-prop-12 .statement tag=03KX}

*Let X be a set and let $\mathfrak{a}$ be its cardinal. Then the cardinal of the set $\mathfrak{P}(\mathrm{X})$ of all subsets of X is $2^{\mathfrak{a}}$.*

Let $\alpha$ and $\beta$ be the elements of the cardinal 2. For each subset Y of X let $f_{\mathrm{Y}}$ be the mapping of X into 2 defined by $f_{\mathrm{Y}}(x) = \alpha$ if $x \in \mathrm{Y}$ and $f_{\mathrm{Y}}(x) = \beta$ if $x \in \mathrm{X} - \mathrm{Y}$. Let $u$ be the mapping $\mathrm{Y} \to f_{\mathrm{Y}}$ of $\mathfrak{P}(\mathrm{X})$ into $2^{\mathrm{X}}$. Conversely, with each mapping $g$ of X into 2 let us associate the subset $\overset{-1}{g}(\alpha)$ of X, and let $v$ be the mapping $g \to \overset{-1}{g}(\alpha)$ of $2^{\mathrm{X}}$ into $\mathfrak{P}(\mathrm{X})$. It is clear that $u \circ v$ and $v \circ u$ are the identity mappings of $2^{\mathrm{X}}$ and $\mathfrak{P}(\mathrm{X})$; hence $u$ and $v$ are bijections (Chapter II, § 3, no. 8, Proposition 8, Corollary) and therefore Card $(\mathfrak{P}(\mathrm{X})) = 2^{\mathfrak{a}}$.

### 6. ORDER RELATION AND OPERATIONS ON CARDINALS

#### Proposition 13 {#ens-iii-s3-prop-13 .statement tag=03KY}

*Let $\mathfrak{a}$ and $\mathfrak{b}$ be cardinals. Then $\mathfrak{a} \geqslant \mathfrak{b}$ if and only if there exists a cardinal $\mathfrak{c}$ such that $\mathfrak{a} = \mathfrak{b} + \mathfrak{c}$.*

For the relation $\mathfrak{a} \geqslant \mathfrak{b}$ means that there exists a subset B of $\mathfrak{a}$ which is equipotent to $\mathfrak{b}$ (no. 2), i.e., $\mathfrak{a}$ is equipotent to the set which is the sum of $\mathfrak{b}$ and a set $c$.

☡

If $\mathfrak{a} \geqslant \mathfrak{b}$, there usually exist many cardinals $\mathfrak{c}$ such that $\mathfrak{a} = \mathfrak{b} + \mathfrak{c}$ (cf. § 6); in general, therefore, it is not possible to define the "difference" $\mathfrak{a} - \mathfrak{b}$ of two such cardinals (cf. § 5, no. 2).

#### Proposition 14 {#ens-iii-s3-prop-14 .statement tag=03KZ}

*Let* $(\mathfrak{a}_\iota)_{\iota \in I}$ *and* $(\mathfrak{b}_\iota)_{\iota \in I}$ *be two families of cardinals, both indexed by the same set* I, *and such that* $\mathfrak{a}_\iota \geqslant \mathfrak{b}_\iota$ *for all* $\iota \in I$. *Then*

$$\sum_{\iota \in I} \mathfrak{a}_\iota \geqslant \sum_{\iota \in I} \mathfrak{b}_\iota, \qquad \mathbf{P}_{\iota \in I} \, \mathfrak{a}_\iota \geqslant \mathbf{P}_{\iota \in I} \, \mathfrak{b}_\iota.$$

The second inequality follows from the inclusion relations between products of sets (Chapter II, § 5, no. 4, Proposition 6, Corollary 3). As to the first inequality, if a set E is the union of a family $(A_\iota)_{\iota \in I}$ of mutually disjoint subsets and if $B_\iota \subset A_\iota$ for all $\iota \in I$, then the $B_\iota$ are also mutually disjoint and $\bigcup_\iota B_\iota \subset \bigcup_\iota A_\iota$ (Chapter II, § 4, no. 2).

#### Corollary 1 {#ens-iii-s3-prop-14-cor-1 .statement tag=03L0}

*Let* $(\mathfrak{a}_\iota)_{\iota \in I}$ *be a family of cardinals. For each subset* J *of* I *we have* $\sum_{\iota \in J} \mathfrak{a}_\iota \leqslant \sum_{\iota \in I} \mathfrak{a}_\iota$. *If also* $\mathfrak{a}_\iota \neq 0$ *for all* $\iota \in I - J$, *then* $\mathbf{P}_{\iota \in J} \, \mathfrak{a}_\iota \leqslant \mathbf{P}_{\iota \in I} \, \mathfrak{a}_\iota$.

Put $\mathfrak{b}_\iota = \mathfrak{a}_\iota$ if $\iota \in J$, and $\mathfrak{b}_\iota = 0$ (resp. $\mathfrak{b}_\iota = 1$) if $\iota \in I - J$. Then apply Proposition 14, observing that the relation $\mathfrak{a} \neq 0$ implies $\mathfrak{a} \geqslant 1$.

#### Corollary 2 {#ens-iii-s3-prop-14-cor-2 .statement tag=03L1}

*If* $\mathfrak{a}$, $\mathfrak{a}'$, $\mathfrak{b}$, $\mathfrak{b}'$ *are cardinals such that* $\mathfrak{a} \leqslant \mathfrak{a}'$, $\mathfrak{b} \leqslant \mathfrak{b}'$, *and* $\mathfrak{a}' > 0$, *then* $\mathfrak{a}^\mathfrak{b} \leqslant \mathfrak{a}'^{\mathfrak{b}'}$.

For $\mathfrak{a}^\mathfrak{b} \leqslant \mathfrak{a}'^\mathfrak{b}$ by Propositions 10 and 14, and $\mathfrak{a}'^\mathfrak{b} \leqslant \mathfrak{a}'^{\mathfrak{b}'}$ by Proposition 10 and Corollary 1 to Proposition 14.

#### Theorem 2 (Cantor) {#ens-iii-s3-thm-2 .statement tag=03R8}

— *For each cardinal* $\mathfrak{a}$, *we have* $2^\mathfrak{a} > \mathfrak{a}$.

We have $\mathrm{Card}(\mathfrak{P}(\mathfrak{a})) = 2^\mathfrak{a}$ (no. 5, Proposition 12). The mapping $x \to \{x\}$ $(x \in \mathfrak{a})$ is an injection of $\mathfrak{a}$ into $\mathfrak{P}(\mathfrak{a})$, whence $\mathfrak{a} \leqslant 2^\mathfrak{a}$. Hence it is enough to show that $\mathfrak{a} \neq 2^\mathfrak{a}$, i.e., that for every mapping $f$ of $\mathfrak{a}$ into $\mathfrak{P}(\mathfrak{a})$, the image $f(\mathfrak{a})$ is distinct from $\mathfrak{P}(\mathfrak{a})$. Let X be the set of all $x \in \mathfrak{a}$ such that $x \notin f(x)$. If $x \in X$, we have $x \notin f(x)$, whence $f(x) \neq X$; if $x \in \mathfrak{a} - X$, we have $x \in f(x)$ and $x \notin X$, whence $f(x) = X$. This shows that $X \notin f(\mathfrak{a})$ and proves the theorem.

#### Corollary {#ens-iii-s3-n6-cor-1 .statement tag=03L2}

*There does not exists a set that has every cardinal as an element.*

If U were such a set, there would exist a set S, the sum of the family of sets $(X)_{X \in U}$, so that every cardinal is equipotent to a subset of S. In particular, let $\mathfrak{S} = \mathrm{Card}(S)$; since $2^\mathfrak{S}$ is a cardinal, we would have $2^\mathfrak{S} \leqslant \mathfrak{S}$, in contradiction to Theorem 2.

### Exercises {#ens-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: (*) The mathematical *term denoted* (Chapter I, § 1, no. 1) by the symbol "1" is of course not to be confused with the *word* "one" in ordinary language. The term denoted by "1" is equal, by virtue of the definition above, to the term denoted by the symbol $$\tau_Z((\exists u)(\exists U)(u = (U, \{\emptyset\}, Z) \text{ and } U \subset \{\emptyset\} \times Z$$ $$\text{and } (\forall x)((x \in \{\emptyset\}) \Rightarrow (\exists y)((x, y) \in U))$$ $$\text{and } (\forall x)(\forall y)(\forall y')(((x, y) \in U \text{ and } (x, y') \in U) \Rightarrow (y = y'))$$ $$\text{and } (\forall y)((y \in Z) \Rightarrow (\exists x)((x, y) \in U)))).$$ As a rough estimate, the term so *denoted* is an assembly of several tens of thousands of signs (each of which is one of $\tau$, $\square$, $\vee$, $\neg$, $=$, $\in$, $\supset$).
