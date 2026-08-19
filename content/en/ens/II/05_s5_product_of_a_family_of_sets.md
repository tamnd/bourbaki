---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 5
section_title: Product of a family of sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 101-112, 127
pdf_pages: 0108-0119, 0134-0134
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE SET OF SUBSETS
      page: 101
      pdf_page: 108
    - "no": 2
      title: SET OF MAPPINGS OF ONE SET INTO ANOTHER
      page: 102
      pdf_page: 109
    - "no": 3
      title: DEFINITIONS OF THE PRODUCT OF A FAMILY OF SETS
      page: 103
      pdf_page: 110
    - "no": 4
      title: PARTIAL PRODUCTS
      page: 105
      pdf_page: 112
    - "no": 5
      title: ASSOCIATIVITY OF PRODUCTS OF SETS
      page: 106
      pdf_page: 113
    - "no": 6
      title: DISTRIBUTIVITY FORMULAE
      page: 107
      pdf_page: 114
    - "no": 7
      title: EXTENSION OF MAPPINGS TO PRODUCTS
      page: 111
      pdf_page: 118
statements: 24
exercises: 3
errata:
    - says: Proposition 1, Corollary 5
      read: Proposition 6, Corollary 1
      why: Section 5 prints five corollaries in no. 4 and all five stand under Proposition 6, which is on page 105 and is the auxiliary the no. announces with "it is enough to prove the following proposition". Proposition 1 has no corollary at all, so there is no Corollary 5 of it. The sentence citing this, on page 106, needs the projection of a product onto a factor to be surjective, and that is Corollary 1 of Proposition 6, whose proof reads "Apply Proposition 5 to the subset J = {alpha} of I".
    - says: Proposition 5, Corollary 2
      read: Proposition 6, Corollary 2
      why: The volume hangs these five corollaries on Proposition 5 four times over and on Proposition 6 once, and the page prints them under Proposition 6. The fact wanted in both sentences here, on pages 108 and 109, is that a product is empty exactly when one of its factors is, which is Corollary 2. Proposition 5 is the statement about a partial product that the proof of Corollary 1 applies, and it carries no corollary of its own.
    - says: Corollary 2 to Proposition 5
      read: Corollary 2 to Proposition 6
      why: The same reference as the two above, written the other way round on page 109, and wrong the same way.
content_sha256: 6393d275988966957f40f77915a91adb15df38100389f3da1b06130ef11ecd50
---

## 5. PRODUCT OF A FAMILY OF SETS

### 1. THE AXIOM OF THE SET OF SUBSETS

A4. $(\forall \mathrm{X}) \ \mathrm{Coll}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X}).$

This axiom means that for every set X there exists a set whose elements are all the subsets of X, namely the set $\mathscr{E}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X})$ (§1, no. 4); this set is denoted by $\mathfrak{P}(\mathrm{X})$ and is called the *set of subsets of* X. Clearly, if $\mathrm{X} \subset \mathrm{X}'$, we have $\mathfrak{P}(\mathrm{X}) \subset \mathfrak{P}(\mathrm{X}')$.

¶ Let A, B be two sets and let $\Gamma$ be a correspondence between A and B. The *function* $\mathrm{X} \to \Gamma \langle \mathrm{X} \rangle$ $(\mathrm{X} \subset \mathfrak{P}(\mathrm{A}), \ \Gamma \langle \mathrm{X} \rangle \in \mathfrak{P}(\mathrm{B}))$ is called the *canonical extension* (or simply the *extension*) *of* $\Gamma$ *to sets of subsets* and is denoted by $\hat{\Gamma}$; it is a mapping of $\mathfrak{P}(\mathrm{A})$ into $\mathfrak{P}(\mathrm{B})$. If $\Gamma'$ is a correspondence between B and a set C, the formula $(\Gamma' \circ \Gamma) \langle \mathrm{X} \rangle = \Gamma' \langle \Gamma \langle \mathrm{X} \rangle \rangle$ shows that the extension of $\Gamma' \circ \Gamma$ to sets of subsets is the mapping $\hat{\Gamma}' \circ \hat{\Gamma}$.

#### Proposition 1 {#ens-ii-s5-prop-1 .statement tag=03IJ}

(1) *If* $f$ *is a surjection of a set* E *onto a set* F, *the canonical extension* $\hat{f}$ *of* $f$ *is a surjection of* $\mathfrak{P}(\mathrm{E})$ *onto* $\mathfrak{P}(\mathrm{F})$.

(2) *If* $f$ *is an injection of* E *into* F, *the canonical extension* $\hat{f}$ *of* $f$ *is an injection of* $\mathfrak{P}(\mathrm{E})$ *into* $\mathfrak{P}(\mathrm{F})$.

(1) If $s$ is a section of $f$, then $f \circ s$ is the identity mapping of F, hence $\hat{f} \circ \hat{s}$ is the identity mapping of $\mathfrak{P}(\mathrm{F})$; therefore $\hat{f}$ is surjective and $\hat{s}$ is a section of $\hat{f}$ (§3, no. 8).

(2) The proposition is obvious if $E = \varnothing$, because then $\mathscr{P}(E) = \{\varnothing\}$. If $E \ne \varnothing$ and if $r$ is a retraction of $f$, then $r \circ f$ is the identity mapping of $E$, so that $\hat{r} \circ \hat{f}$ is the identity mapping of $\mathscr{P}(E)$; therefore $\hat{f}$ is injective, and $\hat{r}$ is a retraction of $\hat{f}$ (§3, no. 8).

### 2. SET OF MAPPINGS OF ONE SET INTO ANOTHER

Let $E$, $F$ be sets. The graph of a mapping of $E$ into $F$ is a subset of $E \times F$. The set of elements of $\mathscr{P}(E \times F)$ which have the property of being graphs of mappings of $E$ into $F$ is therefore a subset of $\mathscr{P}(E \times F)$, which is denoted by $F^E$. The set of triples $f = (G, E, F)$, where $G \in F^E$, is therefore the set of mappings of $E$ into $F$; it is denoted by $\mathscr{F}(E, F)$. Clearly $G \mapsto (G, E, F)$ is a bijection (called the canonical bijection) of $F^E$ onto $\mathscr{F}(E, F)$. The existence of this bijection allows us to translate immediately every proposition relating to the set $F^E$ into one relating to $\mathscr{F}(E, F)$, and vice versa.

¶ Let $E$, $E'$, $F$, $F'$ be sets. Let $u$ be a mapping of $E'$ into $E$, and let $v$ be a mapping of $F$ into $F'$. Then the function $f \mapsto v \circ f \circ u$ is a mapping of $\mathscr{F}(E, F)$ into $\mathscr{F}(E', F')$.

#### Proposition 2 {#ens-ii-s5-prop-2 .statement tag=03Q5}

(1) *If $u$ is a surjection of $E'$ onto $E$ and $v$ an injection of $F$ into $F'$, then the mapping $f \mapsto v \circ f \circ u$ is injective.*

(2) *If $u$ is an injection of $E'$ into $E$ and $v$ a surjection of $F$ onto $F'$, then the mapping $f \mapsto v \circ f \circ u$ is surjective.*

We shall assume that the sets $E$, $E'$, $F$, $F'$ are all non-empty, since otherwise the proposition is trivially verified.

(1) Let $s$ be a section of $u$ and let $r$ be a retraction of $v$ (§3, Definition 11). Then $r \circ (v \circ f \circ u) \circ s = I_F \circ f \circ I_E = f$, so that

$$
f \mapsto v \circ f \circ u
$$

is injective.

(2) Let $r'$ be a retraction of $u$ and let $s'$ be a section of $v$. For every mapping $f' : E' \to F'$ we have $v \circ (s' \circ f' \circ r') \circ u = f'$, which shows that the mapping $f \mapsto v \circ f \circ u$ is surjective.

#### Corollary {#ens-ii-s5-n2-cor-1 .statement tag=03Q6}

*If $u$ is a bijection of $E'$ onto $E$ and $v$ is a bijection of $F$ onto $F'$, then $f \mapsto v \circ f \circ u$ is bijective.*

Let $A$, $B$, $C$ be three sets and let $f$ be a mapping of $B \times C$ into $A$. For every $y \in C$ let $f(\mathord{\cdot}, y)$ be the partial mapping $x \mapsto f(x,y)$ of $B$ into $A$ (§ 3, no. 9); the function $y \mapsto f(\mathord{\cdot}, y)$ is a mapping of $C$ into $\mathscr{F}(B, A)$ exists a unique mapping $f$ of $\mathrm{B} \times \mathrm{C}$ into A such that $g(y) = f(\bullet, y)$ for each $y \in \mathrm{C}$, namely the mapping $(x, y) \to (g(y))(x)$. Hence :

#### Proposition 3 {#ens-ii-s5-prop-3 .statement tag=03Q7}

*If for every mapping $f$ of* $\mathrm{B} \times \mathrm{C}$ *into* A *we denote by $\tilde{f}$ the mapping $y \to f(\bullet, y)$ of* C *into* $\mathscr{F}(\mathrm{B}, \mathrm{A})$, *then the function $f \to \tilde{f}$ is a bijection* (called the *canonical bijection*) *of* $\mathscr{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ *onto* $\mathscr{F}(\mathrm{C}, \mathscr{F}(\mathrm{B}, \mathrm{A}))$.

Similarly we define a *canonical bijection* of $\mathscr{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ onto $\mathscr{F}(\mathrm{B}, \mathscr{F}(\mathrm{C}, \mathrm{A}))$. By reason of the one-to-one correspondence between mappings and functional graphs, these bijections give rise to *canonical bijections* of $\mathrm{A}^{\mathrm{B} \times \mathrm{C}}$ onto $(\mathrm{A}^{\mathrm{B}})^{\mathrm{C}}$ (resp. $(\mathrm{A}^{\mathrm{C}})^{\mathrm{B}}$).

### 3. DEFINITIONS OF THE PRODUCT OF A FAMILY OF SETS

Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets and let F be a functional graph with domain I such that $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ for each $\iota \in \mathrm{I}$. Then for each $\iota \in \mathrm{I}$ we have $\mathrm{F}(\iota) \in \mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$, and therefore F is an element of $\mathfrak{P}(\mathrm{I} \times \mathrm{A})$. The functional graphs with the above property therefore form a subset of $\mathfrak{P}(\mathrm{I} \times \mathrm{A})$.

#### Definition 1 {#ens-ii-s5-def-1 .statement tag=03Q8}

*Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets. The set of functional graphs* F *with domain* I *such that* $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ *for each* $\iota \in \mathrm{I}$ *is called the product of the family of sets $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ and is denoted by* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. *For each* $\iota \in \mathrm{I}$, $\mathrm{X}_\iota$ *is called the factor of index $\iota$ in the product* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. *The mapping* $\mathrm{F} \to \mathrm{F}(\iota)$ $\left( \mathrm{F} \in \prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota,\ \mathrm{F}(\iota) \in \mathrm{X}_\iota \right)$ *is called the coordinate function* (or *projection*) *of index $\iota$, and is denoted by* $\mathrm{pr}_\iota$.

$\mathrm{F}(\iota)$ is called the *coordinate of index* $\iota$ (or *projection of index* $\iota$) of F; the image $\mathrm{pr}_\iota\langle \mathrm{A} \rangle$ of a subset A of $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ under the coordinate function of index $\iota$ is called the *projection of index* $\iota$ of A. It is easily verified that $\mathrm{A} \subset \prod_{\iota \in \mathrm{I}} \mathrm{pr}_\iota \langle \mathrm{A} \rangle$.

We shall often use the notation $(x_\iota)_{\iota \in \mathrm{I}}$ to denote an element of $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ (§3, no. 6).

If $\mathrm{I} = \emptyset$, the set $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ has only one element, namely the empty set (§3, no. 4, Example 1).

¶ If all the factors $\mathrm{X}_\iota$ of the product $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ are equal to the same set E, we have $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \mathrm{E}^{\mathrm{I}}$; this follows immediately from the definitions.

¶ If $(X_\iota)_{\iota \in I}$ is an arbitrary family of sets and if E is a set such that

$$\bigcup_{\iota \in I} X_\iota \subset E,$$

then Definition 1 shows that $\prod_{\iota \in I} X_\iota \subset E^I$; there is therefore a one-to-one correspondence between $\prod_{\iota \in I} X_\iota$ and a set of mappings of I into E (i.e., a subset of $\mathscr{F}(I, E)$).

¶ If $I = \{\alpha\}$ is a set consisting of a single element, we have

$$\prod_{\iota \in I} X_\iota = X_\alpha^{\{\alpha\}};$$

the mapping $F \to F(\alpha)$ is then a bijection (called *canonical*) of $\prod_{\iota \in \{\alpha\}} X_\iota$ onto $X_\alpha$.

¶ Let A, B be sets and let $\alpha$, $\beta$ be distinct objects (there exist two distinct objects, for example $\emptyset$ and $\{\emptyset\}$). Consider the graph $\{(\alpha, A), (\beta, B)\}$, which is clearly functional and is precisely the family $(X_\iota)_{\iota \in \{\alpha, \beta\}}$ such such that $X_\alpha = A$ and $X_\beta = B$. For each pair $(x, y) \in A \times B$, let $f_{x,y}$ be the functional graph $\{(\alpha, x), (\beta, y)\}$. It is evident that the function $(x, y) \to f_{x,y}$ is a bijective mapping of $A \times B$ onto $\prod_{\iota \in \{\alpha, \beta\}} X_\iota$; the inverse of this bijection is $g \to (g(\alpha), g(\beta))$. These two bijections are called *canonical*. In what follows we shall use this one-to-one correspondence to deduce properties of the product of two sets from properties of the product of a family of sets.

¶ Let $(X_\iota)_{\iota \in I}$ be a family of sets each of which consists of a single element, say $X_\iota = \{a_\iota\}$; then the product $\prod_{\iota \in I} X_\iota$ is a set consisting of the single element $(a_\iota)_{\iota \in I}$.

¶ Let E be a set. The graphs of the *constant* mappings $\iota \to x$ of I into E form a subset $\Delta$ of the product $E^I$, called the *diagonal*. If $\bar{x}$ denotes the graph of the mapping $\iota \to x$ (where $x \in E$), the mapping $x \to \bar{x}$ is a bijection of E onto $\Delta$, called the *diagonal mapping*.

#### Proposition 4 {#ens-ii-s5-prop-4 .statement tag=03IK}

*Let* $(X_\iota)_{\iota \in I}$ *be a family of sets, and let u be a bijection of a set* K *onto the index set* I. *If* U *is the graph of u, the mapping* $F \to F \circ U$ *of* $\prod_{\iota \in I} X_\iota$ *into* $\prod_{x \in K} X_{u(x)}$ *is bijective.*

Let

$$A = \bigcup_{\iota \in I} X_\iota = \bigcup_{x \in K} X_{u(x)}$$

(§4, Proposition 1). The mapping $F\to F\circ U$ ($F\in A^I$) is a bijection of $A^I$ onto $A^K$ (Proposition 2). It is evident that the condition “for each $\iota\in I$, $F(\iota)\in X_\iota$” is equivalent to “for each $x\in K$, $(F\circ U)(x)\in X_{u(x)}$”, and the result follows.

### 4. PARTIAL PRODUCTS

Let $(X_\iota)_{\iota\in I}$ be a family of sets, and let $J$ be a subset of $I$. The product $\displaystyle\prod_{\iota\in J}X_\iota$ is called a *partial product* of $\displaystyle\prod_{\iota\in I}X_\iota$. If $f$ is a function whose graph $F$ is a member of $\displaystyle\prod_{\iota\in I}X_\iota$, then $F\circ\Delta_J$ (where $\Delta_J$ is the diagonal of $J\times J$) is the graph of the *restriction* of $f$ to $J$. Clearly $F\circ\Delta_J\in\displaystyle\prod_{\iota\in J}X_\iota$; the mapping $F\to F\circ\Delta_J$ of $\displaystyle\prod_{\iota\in I}X_\iota$ into $\displaystyle\prod_{\iota\in J}X_\iota$ is called the *projection of index* $J$ and is denoted by $\operatorname{pr}_J$.

#### Proposition 5 {#ens-ii-s5-prop-5 .statement tag=03Q9}

*Let $(X_\iota)_{\iota\in I}$ be a family of sets and let $J$ be a subset of $I$. If for each $\iota\in I$ we have $X_\iota\ne\varnothing$, the projection $\operatorname{pr}_J$ is a mapping of $\displaystyle\prod_{\iota\in I}X_\iota$ onto $\displaystyle\prod_{\iota\in J}X_\iota$.*

In view of the remarks made above, it is enough to prove the following proposition :

#### Proposition 6 {#ens-ii-s5-prop-6 .statement tag=03QA}

*Let $(X_\iota)_{\iota\in I}$ be a family of sets such that $X_\iota\ne\varnothing$ for all $\iota\in I$. If $g$ is a mapping of $J\subset I$ into $A=\displaystyle\bigcup_{\iota\in I}X_\iota$, such that $g(\iota)\in X_\iota$ for all $\iota\in J$, then there exists an extension $f$ of $g$ to $I$ such that $f(\iota)\in X_\iota$ for all $\iota\in I$.*

For each $\iota\in I-J$ let $T_\iota$ denote the term $\tau_\iota(y\in X_\iota)$. Since $X_\iota\ne\varnothing$ by hypothesis, we have $T_\iota\in X_\iota$ for all $\iota\in I-J$ (Chapter I, §4, no. 1). If $G$ is the graph of $g$, the graph $G\cup\left(\displaystyle\bigcup_{\iota\in I-J}\{(\iota,T_\iota)\}\right)$ is the graph of a function which has the required properties, as is immediately verified.

#### Corollary 1 {#ens-ii-s5-prop-6-cor-1 .statement tag=03QB}

*Let $(X_\iota)_{\iota\in I}$ be a family of sets such that for each $\iota\in I$ we have $X_\iota\ne\varnothing$. Then for each $\alpha\in I$ the projection $\operatorname{pr}_\alpha$ is a mapping of $\displaystyle\prod_{\iota\in I}X_\iota$ onto $X_\alpha$.*

Apply Proposition 5 to the subset $J=\{\alpha\}$ of $I$ and note that $\operatorname{pr}_\alpha$ is the composition of the canonical mapping of $X_\alpha^{\{\alpha\}}$ onto $X_\alpha$ and the mapping $\operatorname{pr}_{\{\alpha\}}$.

#### Corollary 2 {#ens-ii-s5-prop-6-cor-2 .statement tag=03QC}

*Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets. Then $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \emptyset$ if and only if there exists $\iota \in \mathrm{I}$ such that $\mathrm{X}_\iota = \emptyset$.*

If we have $\mathrm{X}_\iota \neq \emptyset$ for each $\iota \in \mathrm{I}$, then it follows from Corollary 1 that $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$; conversely, if $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$, the relation $\mathrm{pr}_\alpha\Big(\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{X}_\alpha$ shows that $\mathrm{X}_\alpha \neq \emptyset$ for each $\alpha \in \mathrm{I}$.

Hence, if we have a family $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ of non-empty sets, we may introduce (as an auxiliary constant) a function $f$ with domain I such that $f(\iota) \in \mathrm{X}_\iota$ for all $\iota \in \mathrm{I}$. In practice one says : "take an element $x_\iota$ in each $\mathrm{X}_\iota$". Intuitively, we have thus "chosen" an element $x_\iota$ in each set $\mathrm{X}_\iota$; the introduction of the logical sign $\tau$ and the criteria governing its use absolve us from the necessity of formulating an "axiom of choice" to legalize this operation (cf. Summary of Results, §4, no. 10).

#### Corollary 3 {#ens-ii-s5-prop-6-cor-3 .statement tag=03QD}

*Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ and $(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ be two families of sets having the same index set I. If $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ for each $\iota \in \mathrm{I}$, then*

$$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota.$$

*Conversely, if $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod\limits_{\iota \in \mathrm{I}} \mathrm{Y}_\iota$, and if $\mathrm{X}_\iota \neq \emptyset$ for each $\iota \in \mathrm{I}$, then $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ for each $\iota \in \mathrm{I}$.*

The first assertion is obvious, and the second follows from Proposition 1, Corollary 5, because we have then, for each $\alpha \in \mathrm{I}$,

$$\mathrm{X}_\alpha = \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota\Big) = \mathrm{Y}_\alpha.$$

### 5. ASSOCIATIVITY OF PRODUCTS OF SETS

#### Proposition 7 {#ens-ii-s5-prop-7 .statement tag=03IN}

*Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets whose index set I is not the empty set. Let $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ be a partition of I. Then the mapping*

$$f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$$

*of $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ into the product set $\prod\limits_{\lambda \in \mathrm{L}} \Big(\prod\limits_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota\Big)$ is bijective ("associativity" of products of sets).*

From the interpretation of $\mathrm{pr}_{\mathrm{J}_\lambda} f$ as the graph of the restriction of the function whose graph is $f$ (no. 4), it follows that the statement that the mapping $f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$ is bijective means that, for each family $(v_\lambda)_{\lambda \in \mathrm{L}}$, where $v_\lambda$ is a mapping of $\mathrm{J}_\lambda$ into $\bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$, there exists a unique mapping $u$ of I into $\bigcup_{\iota \in I} X_\iota$ such that $v_\lambda$ is the restriction of $u$ to $J_\lambda$ for each $\lambda \in L$. But this is a consequence of the hypothesis that $(J_\lambda)_{\lambda \in L}$ is a partition of I (§4, Proposition 8).

¶ The bijection defined in Proposition 7, and its inverse bijection are said to be *canonical*.

*Remarks*

#### Remark 1 {#ens-ii-s5-n5-rem-1 .statement tag=03SA}

Let $\alpha$, $\beta$ be two distinct objects and let $(J_\lambda)_{\lambda \in \{\alpha, \beta\}}$ be a partition of I into two sets $J_\alpha$, $J_\beta$. We thus obtain a one-to-one mapping (again called *canonical*) of the product $\prod_{\iota \in I} X_\iota$ onto $\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$ by forming the composition of the canonical mapping of $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$ onto $\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$ and the canonical mapping of $\prod_{\iota \in I} X_\iota$ onto $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$. If $X_\iota$ is a set consisting of a *single element* for each $\iota \in J_\beta$, then $\mathrm{pr}_{J_\alpha}$ is a bijective mapping of $\prod_{\iota \in I} X_\iota$ onto $\prod_{\iota \in J_\alpha} X_\iota$.

#### Remark 2 {#ens-ii-s5-n5-rem-2 .statement tag=03SB}

Let $\alpha$, $\beta$, $\gamma$ be three objects, no two of which are equal (three such objects exist; for example, $\emptyset$, $\{\emptyset\}$, $\{\{\emptyset\}\}$), and let A, B, C be sets. Consider the functional graph $\{(\alpha, A), (\beta, B), (\gamma, C)\}$, i.e., the family of sets $(X_\iota)_{\iota \in \{\alpha, \beta, \gamma\}}$ such that $X_\alpha = A$, $X_\beta = B$, $X_\gamma = C$. To the partition of $\{\alpha, \beta, \gamma\}$ formed by the two sets $\{\alpha, \beta\}$ and $\{\gamma\}$ there corresponds a canonical bijection of $\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ onto the product

$$\left( \prod_{\iota \in \{\alpha, \beta\}} X_\iota \right) \times X_\gamma^{\{\gamma\}},$$

and hence a bijection (again called *canonical*) of $\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ onto $A \times B \times C$ (§ 2, no. 2) which transforms each graph $f \in \prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ into the element $(f(\alpha), f(\beta), f(\gamma))$ of $A \times B \times C$. By Proposition 4 we may therefore put any two of the six sets $A \times B \times C$, $B \times C \times A$, $C \times A \times B$, $B \times A \times C$, $A \times C \times B$, $C \times B \times A$ in one-to-one correspondence.

### 6. DISTRIBUTIVITY FORMULAE

#### Proposition 8 {#ens-ii-s5-prop-8 .statement tag=03IO}

*Let* $((X_{\lambda,\iota})_{\iota \in J_\lambda})_{\lambda \in L}$ *be a family (with index set* L*) of families of sets. Suppose that* $L \neq \emptyset$ *and that* $J_\lambda \neq \emptyset$ *for each* $\lambda \in L$. *Let*

$$I = \prod_{\lambda \in L} J_\lambda \neq \emptyset.$$

*Then we have*

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right),$$
$$\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcup_{f \in I} \left( \bigcap_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$$

("distributivity" of union over intersection, and of intersection over union).

Let $x$ be an element of $\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right)$ and let $f$ be any element of I. There exists an index $\lambda$ such that $x \in \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$; consequently $x \in X_{\lambda, f(\lambda)}$ and hence

$$x \in \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}.$$

Since this is true for each $f \in I$, we have

$$x \in \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

Conversely, let $x$ be an object which does not belong to the set

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right).$$

Then for each $\lambda \in L$ we have $x \notin \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$, which means that the set $J'_\lambda$ of indices $\iota \in J_\lambda$ such that $x \notin X_{\lambda, \iota}$ is not empty for each $\lambda \in L$. By Proposition 5, Corollary 2, there exists a functional graph $f$ with domain L such that for each $\lambda \in L$ we have $f(\lambda) \in J'_\lambda$. Consequently $f \in I$ and $x \notin X_{\lambda, f(\lambda)}$ for each $\lambda \in L$; hence

$$x \notin \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$$

and thus

$$x \notin \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

This completes the proof of the first formula. The second formula follows by applying the first to the family $((\complement_A X_{\lambda, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$, where A denotes the union $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\lambda \right)$.

#### Corollary {#ens-ii-s5-n6-cor-1 .statement tag=03IP}

*Let* $(X_\iota)_{\iota \in I}$ *and* $(Y_\varkappa)_{\varkappa \in K}$ *be two families of sets with non-empty index sets* I, K. *Then*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \cup \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cup Y_\varkappa),$$
$$\left( \bigcup_{\iota \in I} X_\iota \right) \cap \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cap Y_\varkappa).$$

Let $\alpha$, $\beta$ be two distinct objects; apply the formulae of Proposition 8 (with $L = \{\alpha,\ \beta\}$, $J_\alpha = I$, $J_\beta = K$) to the family $((Z_{\lambda,\, \mu})_{\mu \in J_\lambda})_{\lambda \in L}$, where $Z_{\alpha,\, \iota} = X_\iota$ for all $\iota \in I$ and $Z_{\beta,\, \varkappa} = Y_\varkappa$ for each $\varkappa \in K$. By the existence of the canonical bijection of $\coprod_{\lambda \in L} J_\lambda$ onto $I \times K$ (no. 3) and by Proposition 1 of § 4 we obtain the formulae stated.

#### Proposition 9 {#ens-ii-s5-prop-9 .statement tag=03IQ}

*Let* $((X_{\lambda,\, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$ *be a family (with index set* L) *of families of sets. Let* $I = \prod_{\lambda \in L} J_\lambda$. *Then*

$$\prod_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

*and (if* $L \neq \emptyset$ *and* $J_\lambda \neq \emptyset$ *for each* $\lambda \in L$)

$$\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcap_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

("distributivity" of product over union and over intersection).
The first formula is trivially true if $L = \emptyset$ or if $J_\lambda = \emptyset$ for some $\lambda \in L$. If not, let $g$ be an element of $\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right)$. For each $\lambda \in L$ there exists an index $\iota \in J_\lambda$ such that $g(\lambda) \in X_{\lambda,\, \iota}$; in other words, the set $H_\lambda$ of indices $\iota \in J_\lambda$ such that $g(\lambda) \in X_{\lambda,\, \iota}$ is not empty. By Corollary 2 to Proposition 5 there is therefore a functional graph $f$ with domain L such that

$$f(\lambda) \in H_\lambda$$

for each $\lambda \in L$, i.e., $g(\lambda) \in X_{\lambda,\, f(\lambda)}$. Hence we have $g \in \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)}$ and consequently $g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$. Conversely, if

$$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right),$$

there is a functional graph $f \in I$ such that for every $\lambda \in L$ we have

$$g(\lambda) \in X_{\lambda,\, f(\lambda)}$$

and, *a fortiori*, $g(\lambda) \in \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$. This completes the proof of the first formula. The proof of the second formula is analogous but simpler, and we leave it to the reader.

#### Corollary 1 {#ens-ii-s5-prop-9-cor-1 .statement tag=03QE}

*Suppose that* $L \neq \emptyset$ *and that* $J_\lambda \neq \emptyset$ *for each* $\lambda \in L$. *If for e achindex* $\lambda \in L$ *the family* $(X_{\lambda, \iota})_{\iota \in J_\lambda}$ *is a partition of* $X_\lambda = \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$, *then the family* $\left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)_{f \in I}$ *is a partition of* $\prod_{\lambda \in L} X_\lambda$.

If we set

$$\mathrm{P}_f = \prod_{\lambda \in L} X_{\lambda, f(\lambda)},$$

then, by virtue of the first formula of Proposition 9, it is sufficient to show that $\mathrm{P}_f \neq \emptyset$ for all $f \in I$ and that $\mathrm{P}_f \cap \mathrm{P}_g = \emptyset$ whenever $f$ and $g$ are distinct elements of I. The first point follows from Proposition 5, Corollary 2. As to the second, if $f \neq g$, there exists $\lambda \in L$ such that

$$f(\lambda) \neq g(\lambda)$$

and therefore, by virtue of the hypothesis, $X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$. It follows that there is no graph belonging to $\mathrm{P}_f \cap \mathrm{P}_g$; for if G were such a graph, we would have $\mathrm{G}(\lambda) \in X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$, which is absurd.

#### Corollary 2 {#ens-ii-s5-prop-9-cor-2 .statement tag=03QF}

*Let* $(X_\iota)_{\iota \in I}$ *and* $(Y_\varkappa)_{\varkappa \in K}$ *be two families of sets. Then*

$$\left( \bigcup_{\iota \in I} X_\iota \right) \times \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa)$$

*and, if* I *and* K *are non-empty,*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \times \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa).$$

The proof follows the pattern of the proof of the Corollary to Proposition 8.

#### Proposition 10 {#ens-ii-s5-prop-10 .statement tag=03QG}

*Let* $(X_{\iota, \varkappa})_{(\iota, \varkappa) \in I \times K}$ *be a family of sets whose index set is the product of two sets* I *and* K. *If* $K \neq \emptyset$, *we have*

$$\bigcap_{\varkappa \in K} \left( \prod_{\iota \in I} X_{\iota, \varkappa} \right) = \prod_{\iota \in I} \left( \bigcap_{K \in \varkappa} X_{\iota, \varkappa} \right).$$

Both sides of the equality to be proved are functional graphs. A graph $f$ belongs to the left-hand side if and only if, for each $\varkappa \in K$, $f \in \prod_{\iota \in I} X_{\iota, \varkappa}$; that is, if and only if $f(\iota) \in X_{\iota, \varkappa}$ for all $(\iota, \varkappa) \in I \times K$. For $f$ to belong to the right-hand side it is necessary and sufficient that $f(\iota) \in \bigcap_{\varkappa \in K} X_{\iota, \varkappa}$ for each $\iota \in I$, i.e., that $f(\iota) \in X_{\iota, \varkappa}$ for each pair $(\iota, \varkappa) \in I \times K$. This completes the proof.

#### Corollary {#ens-ii-s5-n6-cor-2 .statement tag=03IR}

*Let* $(X_\iota)_{\iota \in I}$ *and* $(Y_\iota)_{\iota \in I}$ *be two families of sets with the same index set* $I \neq \emptyset$. *Then*

$$\Big(\prod_{\iota \in I} X_\iota\Big) \cap \Big(\prod_{\iota \in I} Y_\iota\Big) = \prod_{\iota \in I} (X_\iota \cap Y_\iota),$$
$$\Big(\bigcap_{\iota \in I} X_\iota\Big) \times \Big(\bigcap_{\iota \in I} Y_\iota\Big) = \bigcap_{\iota \in I} (X_\iota \times Y_\iota).$$

Apply Proposition 10 to the case where K (resp. I) is a set consisting of two distinct elements.

### 7. EXTENSION OF MAPPINGS TO PRODUCTS

#### Definition 2 {#ens-ii-s5-def-2 .statement tag=03IS}

*Let* $(X_\iota)_{\iota \in I}$, $(Y_\iota)_{\iota \in I}$ *be two families of sets, and let* $(g_\iota)_{\iota \in I}$ *be a family of functions with the same index set* I *such that* $g_\iota$ *is a mapping of* $X_\iota$ *into* $Y_\iota$ *for each* $\iota \in I$. *For each* $f \in \prod_{\iota \in I} X_\iota$ *let* $u_f$ *be the graph of the function* $\iota = g_\iota(f(\iota))$ $(\iota \in I)$, *which is an element of* $\prod_{\iota \in I} Y_\iota$. *The mapping* $f \to u_f$ *of* $\prod_{\iota \in I} X_\iota$ *into* $\prod_{\iota \in I} Y_\iota$ *is called the canonical extension* (or simply the *extension*) *to products of the family of mappings* $(g_\iota)_{\iota \in I}$; *it is also sometimes called the product of the family of mappings* $(g_\iota)_{\iota \in I}$.

When the index notation is used, the product of the family $(g_\iota)_{\iota \in I}$ is the function $(x_\iota)_{\iota \in I} \to (g_\iota(x_\iota))_{\iota \in I}$; it is sometimes denoted by $(g_\iota)_{\iota \in I}$.

If $I = \{\alpha, \beta\}$, where $\alpha$ and $\beta$ are distinct, the extension to products of the family of mappings $(g_\iota)_{\iota \in I}$ is just $\psi \circ (g_\alpha \times g_\beta) \circ \varphi$, where $\varphi$ denotes the canonical mapping of $\prod_{\iota \in I} X_\iota$ onto $X_\alpha \times X_\beta$ (no. 3) and $\psi$ the canonical mapping of $Y_\alpha \times Y_\beta$ onto $\prod_{\iota \in I} Y_\iota$.

#### Proposition 11 {#ens-ii-s5-prop-11 .statement tag=03IT}

*Let* $(X_\iota)_{\iota \in I}$, $(Y_\iota)_{\iota \in I}$, $(Z_\iota)_{\iota \in I}$ *be three families of sets and let* $(g_\iota)_{\iota \in I}$, $(g'_\iota)_{\iota \in I}$ *be two families of functions, all having the same index set, such that* $g_\iota$ *is a mapping of* $X_\iota$ *into* $Y_\iota$ *and* $g'_\iota$ *a mapping of* $Y_\iota$ *into* $Z_\iota$, *for each* $\iota \in I$. *Let* $g$ *and* $g'$ *be the extensions of the families* $(g_\iota)_{\iota \in I}$ *and* $(g'_\iota)_{\iota \in I}$ *to products. Then the extension of the family* $(g'_\iota \circ g_\iota)_{\iota \in I}$ *to products is equal to* $g' \circ g$.

This follows immediately from Definition 2.

#### Corollary {#ens-ii-s5-n7-cor-1 .statement tag=03IU}

Let $(X_i)_{i\in I}$, $(Y_i)_{i\in I}$ be two families of sets and let $(g_i)_{i\in I}$ be a family of functions. If $g_i$ is an injection (resp. surjection) of $X_i$ into $Y_i$, for each $i\in I$, then the extension $g$ of $(g_i)_{i\in I}$ to products is an injection (resp. surjection) of $\displaystyle\prod_{i\in I}X_i$ into $\displaystyle\prod_{i\in I}Y_i$.

(1) Let us assume that $X_i\ne\varnothing$ for each $i\in I$; otherwise the result is trivial. Suppose that $g_i$ is injective for each $i\in I$, and let $r_i$ be a retraction of $g_i$ (§ 3, no. 8, Definition 11), so that $r_i\circ g_i$ is the identity mapping of $X_i$. Let $r$ be the extension to products of the family $(r_i)_{i\in I}$; since $r\circ g$ is the extension to products of the family of identity mappings $I_{X_i}$, $r\circ g$ is the identity mapping of $\displaystyle\prod_{i\in I}X_i$, and hence $g$ is injective (§ 3, Proposition 8).

(2) Suppose that $g_i$ is a surjection of $X_i$ onto $Y_i$ for each $i\in I$, and let $s_i$ be a section of $g_i$ (§ 3, no. 8, definition 11), so that $g_i\circ s_i$ is the identity mapping of $Y_i$. If $s$ is the extension to products of the family $(s_i)_{i\in I}$, then $g\circ s$ is the extension to products of the family of identity mappings $I_{Y_i}$, and is therefore the identity mapping of $\displaystyle\prod_{i\in I}Y_i$; hence $g$ is surjective (§ 3, Proposition 8).

Let $(X_i)_{i\in I}$ be a family of sets, and let $E$ be a set. For every mapping $f$ of $E$ into $\displaystyle\prod_{i\in I}X_i$, $\operatorname{pr}_i\circ f$ is a mapping of $E$ into $X_i$. If $\bar f$ is the extension to products of this family of mappings, and if $d$ is the diagonal mapping of $E$ into $E^I$, then it is immediate that $f=\bar f\circ d$. Conversely, let $(f_i)_{i\in I}$ be a family of functions such that $f_i$ is a mapping of $E$ into $X_i$ for each $i\in I$, and let $\bar f$ be the extension to products of this family; then we have $\operatorname{pr}_i\circ(\bar f\circ d)=f_i$ for each $i\in I$. By abuse of language, the mapping $\bar f\circ d$ is also written as $(f_i)_{i\in I}$. In this way we define a one-to-one mapping of the set $\displaystyle\prod_{i\in I}X_i^E$ onto the set $\displaystyle\left(\prod_{i\in I}X_i\right)^E$; this mapping and its inverse are said to be canonical.

### Exercises {#ens-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
