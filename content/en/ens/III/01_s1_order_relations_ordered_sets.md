---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 1
section_title: Order relations. Ordered sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
pdf_pages: 0137-0154, 0218-0227
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ORDER RELATION
      page: 0
      pdf_page: 137
    - "no": 2
      title: PREORDER RELATIONS
      page: 0
      pdf_page: 139
    - "no": 3
      title: NOTATION AND TERMINOLOGY
      page: 0
      pdf_page: 141
    - "no": 4
      title: ORDERED SUBSETS. PRODUCT OF ORDERED SETS
      page: 0
      pdf_page: 142
    - "no": 5
      title: INCREASING MAPPINGS
      page: 0
      pdf_page: 144
    - "no": 6
      title: MAXIMAL AND MINIMAL ELEMENTS
      page: 0
      pdf_page: 145
    - "no": 7
      title: GREATEST ELEMENT AND LEAST ELEMENT
      page: 0
      pdf_page: 146
    - "no": 8
      title: UPPER AND LOWER BOUNDS
      page: 0
      pdf_page: 147
    - "no": 9
      title: LEAST UPPER BOUND AND GREATEST LOWER BOUND
      page: 0
      pdf_page: 147
    - "no": 10
      title: DIRECTED SETS
      page: 0
      pdf_page: 151
    - "no": 11
      title: LATTICES
      page: 0
      pdf_page: 151
    - "no": 12
      title: TOTALLY ORDERED SETS
      page: 0
      pdf_page: 152
    - "no": 13
      title: INTERVALS
      page: 0
      pdf_page: 153
statements: 21
exercises: 3
content_sha256: 70a2a572a2fde9b17fe7e7f56f801d935c7df809acb11d95eed3b2f9a5a1149e
---

## 1. ORDER RELATIONS. ORDERED SETS

### 1. DEFINITION OF AN ORDER RELATION

Let $R\{x, y\}$ be a relation, $x$ and $y$ being distinct letters. R is said to be an *order relation with respect to the letters x and y* (or *between x and y*) if

$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, z\}) \Rightarrow R\{x,\, z\},$$
$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, x\}) \Rightarrow (x = y),$$
$$R\{x, y\} \Rightarrow (R\{x,\, x\} \ \text{ and } \ R\{\, y,\, y\}).$$

The first of the above relations says that R is *transitive* with respect to the letters $x$ and $y$ (Chapter II, § 6, no. 1).

*Examples*

(1) The *relation of equality*, $x = y$, is an order relation.

(2) The relation $X \subset Y$ is an order relation between X and Y (Chapter II, § 1, no. 2, Propositions 1 and 2 and axiom A1) which is often called the *inclusion relation*.

(3) Let $R\{x, y\}$ be an order relation between $x$ and $y$. The relation $R\{\, y,\, x\}$ is then an order relation *between x and y*, called the *opposite* of the order relation $R\{x,\, y\}$.

An *order relation on a set* E is an order relation $R\{x,\, y\}$ with respect to two distinct letters $x$, $y$ such that the relation $R\{x,\, x\}$ is *equivalent to* $x \in E$ (in other words, is such that $R\{x,\, y\}$ is *reflexive* on E (Chapter II, § 6, no. 1)). Then the relation $R\{x,\, y\}$ implies "$x \in E$ and $y \in E$" and the relation $(R\{x,\, y\}$ and $R\{\, y,\, x\})$ is equivalent to "$x \in E$ and $y \in E$ and $x = y$".

*Examples*

(1) The relations of equality and inclusion are not order relations on a set, for the relations $x = x$ and $\mathrm{X} \subset \mathrm{X}$ are not collectivizing (Chapter II, § 1, no. 7).

(2) Let $\mathrm{R}\}x,\ y\{$ be an order relation between $x$ and $y$, and let E be a set such that $x \in \mathrm{E}$ implies $\mathrm{R}\}x,\ x\{$ (notice that the empty set satisfies this condition). The relation "$\mathrm{R}\}x,\ y\{$ and $x \in \mathrm{E}$ and $y \in \mathrm{E}$" is then an order relation on E, as is immediately verified; it is called the order relation *induced* by $\mathrm{R}\}x,y\{$ on E (cf. no. 4). By abuse of language, the phrase "the relation $\mathrm{S}\}x,\ y\{$ is an order relation between elements of E" is often used in place of "the relation ($\mathrm{S}\}x,\ y\{$ and $x \in \mathrm{E}$ and $y \in \mathrm{E}$) is an order relation on E". For example, if A is a set, the relation "$\mathrm{X} \subset \mathrm{Y}$ and $\mathrm{X} \subset \mathrm{A}$ and $\mathrm{Y} \subset \mathrm{A}$" is an order relation between subsets of A.

(3) Let E, F be sets. The relation "*g extends f*" is an order relation (between $f$ and $g$) on the set of mappings of subsets of E into F.

(4) In the set $\mathfrak{P}(\mathfrak{P}(\mathrm{E}))$ of sets of subsets of a set E, let $\mathscr{P}$ be the set of *partitions* of E (Chapter II, § 4, no. 7). We recall that a partition $\varpi$ is said to be *coarser* than a partition $\varpi'$ if given any $\mathrm{Y} \in \varpi'$ there exists $\mathrm{X} \in \varpi$ such that $\mathrm{Y} \subset \mathrm{X}$ (Chapter II, § 4, no. 6). For each partition $\varpi$ of E let $\tilde{\varpi}$ be the graph of the equivalence relation defined by $\varpi$ on E (Chapter II, § 6, no. 2), that is to say, the union of the (mutually disjoint) sets $\mathrm{A} \times \mathrm{A}$, where A runs through $\varpi$. The relation "$\varpi$ is coarser than $\varpi'$" is immediately seen to be equivalent to $\tilde{\varpi} \supset \tilde{\varpi}'$, and is therefore an order relation on the set $\mathscr{P}$ between $\varpi$ and $\varpi'$.

An *ordering* on a set E is a correspondence $\Gamma = (\mathrm{G},\ \mathrm{E},\ \mathrm{E})$ with E as source and as target, and such that the relation $(x,\ y) \in \mathrm{G}$ is an order relation on E. By abuse of language we shall sometimes refer to the graph G of $\Gamma$ as an ordering on E. If $\mathrm{R}\}x,\ y\{$ is an order relation on E, it has a graph which is an ordering on E.

#### Proposition 1 {#ens-iii-s1-prop-1 .statement tag=03JA}

*A correspondence* $\Gamma$ *between* E *and* E *is an ordering on* E *if and only if its graph* G *satisfies the following conditions :*

(a) $\mathrm{G} \circ \mathrm{G} = \mathrm{G}$.

(b) *The set* $\mathrm{G} \cap \overset{-1}{\mathrm{G}}$ *is the diagonal* $\Delta$ *of* $\mathrm{E} \times \mathrm{E}$.

For the relation $((x,\ y) \in \mathrm{G}$ and $(y,\ z) \in \mathrm{G}) \Rightarrow ((x,\ z) \in \mathrm{G})$ can be written as $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$, and the relation

$$((x,\ y) \in \mathrm{G} \text{ and } (y,\ x) \in \mathrm{G}) \Leftrightarrow (x = y \text{ and } x \in \mathrm{E} \text{ and } y \in \mathrm{E})$$

can be written as $\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$. From $\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$ we then deduce $\Delta \subset \mathrm{G}$, whence $\mathrm{G} = \Delta \circ \mathrm{G} \subset \mathrm{G} \circ \mathrm{G}$; since also $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$, we have

$$\mathrm{G} \circ \mathrm{G} = \mathrm{G}.$$

### 2. PREORDER RELATIONS

Let $R\{x, y\}$ be a relation, $x$ and $y$ being distinct letters. If $R$ is transitive and if we have $R\{x, y\} \Rightarrow (R\{x, x\}$ and $R\{y, y\})$, it does not necessarily follow that $R$ is an order relation because the relation

$$(R\{x, y\} \text{ and } R\{y, x\})$$

does not necessarily imply $x = y$. $R\{x, y\}$ is said to be a *preorder relation* between $x$ and $y$; $R\{y, x\}$ is then also a preorder relation between $x$ and $y$, called the *opposite* of the relation $R\{x, y\}$.

For example, let $\mathfrak{R}$ be the set of subsets of $\mathfrak{P}(E)$ which are coverings of E (Chapter II, § 4, no. 6). The relation "$\mathfrak{R}$ is coarser than $\mathfrak{R}'$" between elements $\mathfrak{R}$, $\mathfrak{R}'$ of $\mathfrak{R}$ (Chapter II, § 4, no. 6) is transitive and reflexive. But two distinct coverings can be such that each is coarser than the other; for example, this is the case when $\mathfrak{R}'$ is the union (in $\mathfrak{P}(E)$) of $\mathfrak{R}$ and a subset of E contained in a set of $\mathfrak{R}$ but not belonging to $\mathfrak{R}$.

But in any case the relation $(R\{x, y\}$ and $R\{y, x\})$ is an *equivalence relation* $S\{x, y\}$ with respect to $x$ and $y$. Let $x'$, $y'$ be letters distinct from $x$, $y$ which do not appear in R. Then $R\{x, y\}$ is *compatible* (with respect to $x$ and $y$) with the equivalence relations $S\{x, x'\}$ and $S\{y, y'\}$; in other words (Chapter II, § 6, no. 8), the relation

$$(R\{x, y\} \text{ and } S\{x, x'\} \text{ and } S\{y, y'\})$$

implies $R\{x', y'\}$.

¶ A *preorder relation on a set* E is a preorder relation $R\{x, y\}$ such that the relation $R\{x, x\}$ is equivalent to $x \in E$. The relation $R\{x, y\}$ then implies "$x \in E$ and $y \in E$".

¶ If $R\{x, y\}$ is a preorder relation on a set E, then the relation $S\{x, y\}$ defined above is an equivalence relation on E. Let $R'\{X, Y\}$ denote the relation

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\exists x)(\exists y)(x \in X \text{ and } y \in Y \text{ and } R\{x, y\}),$$

that is to say, the relation induced by R on passing to the quotient (with respect to $x$ and $y$); we saw in Chapter II, § 6, no. 3, that it is equivalent to the relation

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow R\{x, y\}).$$

¶ Let us show that $R'\{X, Y\}$ is an *order relation* between elements of E/S. The relation $(R'\{X, Y\}$ and $R'\{Y, Z\})$ is equivalent to

$$X \in E/S \text{ and } Y \in E/S \text{ and } Z \in E/S \text{ and }$$
$$(\forall x)(\forall y)(\forall z)((x \in X \text{ and } y \in Y \text{ and } z \in Z) \Rightarrow (R\{x, y\} \text{ and } R\{y, z\}))$$

(Chapter I, § 4, criteria C40, C41). Since $R\{x, y\}$ is transitive and $Y \in E/S \Rightarrow Y \neq \emptyset$ (Chapter II, § 6, no. 2), it follows immediately that $R'\{X, Y\}$ is transitive. Next, $(R'\{X, Y\}$ and $R'\{Y, X\})$ is equivalent to

$$X \in E/S \text{ and } Y \in E/S \text{ and }$$
$$(\forall x)(\forall y) \ ((x \in X \text{ and } y \in Y) \Rightarrow (R\{x, y\} \text{ and } R\{y, x\})),$$

and hence equivalent to

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow S\{x, y\}),$$

and therefore implies

$$X \in E/S \quad \text{and} \quad Y \in E/S \quad \text{and} \quad X = Y.$$

Moreover, $R\{x, y\}$ implies $R\{x, x\}$ and $R\{y, y\}$, and hence $R'\{X, Y\}$ implies each of the relations

$$X \in E/S \text{ and } (\forall x)((x \in X) \Rightarrow R\{x, x\}),$$
$$Y \in E/S \text{ and } (\forall y)((y \in Y) \Rightarrow R\{y, y\}),$$

whence $R'\{X, Y\}$ implies $(R'\{X, X\}$ and $R'\{Y, Y\})$. Finally, since $x \in E$ implies $R\{x, x\}$, $X \in E/S$ implies $R'\{X, X\}$, and the proof of our assertion is complete. $R'\{X, Y\}$ is said to be the order relation *associated* with $R\{x, y\}$.

¶ A *preordering* on a set E is a correspondence $\Gamma = (G, E, E)$ with E as source and as target, and such that $(x, y) \in G$ is a preorder relation on E. By abuse of language we refer sometimes to the graph G of $\Gamma$ as a preordering on E. For this to be so it is necessary and sufficient that $\Delta \subset G$ and $G \circ G \subset G$ (which implies $G \circ G = G$). The equivalence relation S corresponding to the preorder relation $(x, y) \in G$ then has $G \cap \overset{-1}{G}$ as its graph; the order relation associated with $(x, y) \in G$ has as graph the subset G' of $(E/S) \times (E/S)$ which corresponds (Chapter II, § 6, no. 8) to the image of G under the canonical mapping of $E \times E$ onto

$$(E \times E)/(S \times S).$$

#### Example {#ens-iii-s1-n2-exa-1 .statement tag=03JB}

\* Let A be a ring with an identity element. The relation $(\exists z)(z \in \mathrm{A}$ and $y = zx)$ between two elements $x$, $y$ of A is a preorder relation on A; it is read "$x$ is a right divisor of $y$" or "$y$ is a left multiple of $x$". \*

### 3. NOTATION AND TERMINOLOGY

The definitions to be given in the remainder of this section apply to an arbitrary order (or preorder) relation $\mathrm{R}\{x, y\}$ between $x$ and $y$, but will be used mainly in the case where $\mathrm{R}\{x, y\}$ is written $x \leqslant y$ \*(by analogy with the usual order relation between integers or real numbers)\* (or $x \subset y$, or by means of some analogous sign); we shall therefore state them only for the notation $x \leqslant y$, and leave to the reader the task of transcribing them into other notations. When $\mathrm{R}\{x, y\}$ is written $x \leqslant y$, then $y \geqslant x$ is synonymous with $x \leqslant y$, and these relations are read "$x$ is *smaller* than $y$", or "$x$ is *less than* $y$", or "$y$ is *larger* than $x$" or "$y$ is *greater than* $x$". The relation $x \geqslant y$ is then the preorder relation (*between* $x$ *and* $y$) *opposite to* $x \leqslant y$.

By abuse of language, we shall often speak of "the relation $\leqslant$" instead of "the relation $x \leqslant y$"; in this case "the relation $\geqslant$" is the opposite of "the relation $\leqslant$". We remark also that, in the same proof, we may often use the same sign $\leqslant$ to denote several different order relations when there is no risk of confusion.

The conditions for a relation written $x \leqslant y$ to be an order relation on a set E are as follows :

(RO$_{\mathrm{I}}$)    *The relation "$x \leqslant y$ and $y \leqslant z$" implies $x \leqslant z$.*
(RO$_{\mathrm{II}}$)   *The relation "$x \leqslant y$ and $y \leqslant x$" implies $x = y$.*
(RO$_{\mathrm{III}}$)  *The relation $x \leqslant y$ implies "$x \leqslant x$ and $y \leqslant y$".*
(RO$_{\mathrm{IV}}$)   *The relation $x \leqslant x$ is equivalent to $x \in \mathrm{E}$.*

If we leave out condition (RO$_{\mathrm{II}}$), we have the conditions for $x \leqslant y$ to be a preorder relation on E.
¶ When an order relation is written $x \leqslant y$ we shall write $x < y$ (or $y > x$) for the relation "$x \leqslant y$ and $x \neq y$"; these relations are read "$x$ is *strictly smaller* than $y$", or "$x$ is *strictly less* than $y$", or "$y$ is *strictly larger* than $x$", or "$y$ is *strictly greater* than $x$".

The example of the inclusion relation shows that the negation of $x \leqslant y$ (sometimes denoted by $x \nleqslant y$) is *not necessarily equivalent to* $y < x$ (cf. no. 12).

C58. *Let $\leqslant$ be an order relation, and let $x$, $y$ be two distinct letters. The relation $x \leqslant y$ is equivalent to "$x < y$ or $x = y$". Each of the relations "$x \leqslant y$ and $y < z$", "$x < y$ and $y \leqslant z$" implies $x < z$.*

The first assertion follows from the criterion $A \Rightarrow ((A$ and (not $B$)) or $B$) (Chapter I, § 3, criterion C24). To prove the second assertion, we remark that each of the hypotheses implies $x \leqslant z$, by transitivity; and the relation ($x = z$ and $x \leqslant y$ and $y \leqslant z$) would imply $x = y = z$, contrary to the hypothesis.

¶ In order to make matters easier and to replace metamathematical criteria by mathematical theorems we shall usually consider a theory $\mathscr{T}$ which contains the axioms and axiom schemes of the theory of sets, and in addition, two constants E and $\Gamma$ satisfying the axiom

"$\Gamma$ is an ordering on the set E" (no. 1).

We shall denote by $x \leqslant y$ the relation $y \in \Gamma\langle x \rangle$, and we shall say that the set E is *ordered by the ordering* $\Gamma$ (or by the order relation $y \in \Gamma\langle x \rangle$) (cf. Chapter IV, § 1).

¶ Whenever, in $\mathscr{T}$, $\Gamma$ is a preordering on E, we say likewise that E is *preordered by the preordering* $\Gamma$.

In some situations (for example in the following definition) the theories which we shall consider are a little more complicated. We shall leave it to the reader to make explicit the constants and axioms of such theories.

Let E, E$'$ be two sets ordered by orderings $\Gamma$, $\Gamma'$. An *isomorphism of* E *onto* E$'$ (for the orderings $\Gamma$ and $\Gamma'$) is a bijection $f$ of E onto E$'$ such that the relations $x \leqslant y$ and $f(x) \leqslant f(y)$ are equivalent (cf. Chapter IV, § 1).

### 4. ORDERED SUBSETS. PRODUCT OF ORDERED SETS

Let E be a set ordered by an ordering $\Gamma$, with graph G. For each subset A of E, $G \cap (A \times A)$ is an ordering on A; the corresponding order relation is equivalent to "$x \leqslant y$ and $x \in A$ and $y \in A$", and we shall denote it simply by $x \leqslant y$ (by abuse of language). The ordering and the order relation thus defined on A are said to be *induced* by the ordering and order relation given on E; and the ordering and order relation on E are said to be *extensions* of the ordering and order relation which they induce on A. Whenever we consider A as an ordered set we have in mind the ordering induced on A by that on E, unless the contrary is expressly stated.

*Examples*. The relations induced by the inclusion relation $X \subset Y$ on various sets of subsets are of considerable importance. Here are some examples :

(1) Let E, F be two sets, and let $\Phi(E, F)$ be the set of all mappings of subsets of E into F. For each $f \in \Phi(E, F)$ let $G_f$ be the graph of $f$, which is a subset of $E \times F$. If we endow $\Phi(E, F)$ with the order relation "*g extends f*" between $f$ and $g$ (no. 1, Example 3), then $f \to G_f$ is an isomorphism of the ordered set $\Phi(E, F)$ onto a subset of $\mathfrak{P}(E \times F)$, ordered by inclusion.

(2) For each partition $\varpi$ of a set E, let $\tilde{\varpi}$ be the graph of the equivalence relation defined by $\varpi$ on E. The mapping $\varpi \to \tilde{\varpi}$ is an isomorphism of the set $\mathfrak{L}$ of partitions of E, ordered by the relation "$\varpi$ is finer than $\varpi'$" between $\varpi$ and $\varpi'$ (no. 1, Example 4) onto a subset of $\mathfrak{P}(E \times E)$, ordered by inclusion.

(3) Let E be a set and let $\Omega \subset \mathfrak{P}(E \times E)$ be the set of graphs of *preorderings* on E (no. 2) (or, by abuse of language, the set of all preorderings on E). The order relation $s \subset t$ between $s$ and $t$, induced on $\Omega$ by the inclusion relation on $\mathfrak{P}(E \times E)$, is expressed by saying that "the preordering $s$ is *finer* than $t$" (or that "$t$ is *coarser* than $s$"). Let $x(s)y$ and $x(t)y$ respectively denote the preorder relations $(x, y) \in s$ and $(x, y) \in t$ on E; then to say that $s$ is finer than $t$ is equivalent to saying that the relation $x(s)y$ *implies* $x(t)y$.

Let $(E_\iota)_{\iota \in I}$ be a family of sets, and for each index $\iota \in I$ let $\Gamma_\iota$ be an ordering on $E_\iota$; let $G_\iota \subset E_\iota \times E_\iota$ be its graph, and let $x_\iota \leqslant y_\iota$ denote the order relation $(x_\iota, y_\iota) \in G_\iota$ on $E_\iota$. On the product set $F = \prod_{\iota \in I} E_\iota$, the relation

$$(\forall \iota) \, ((\iota \in I) \Rightarrow (x_\iota \leqslant y_\iota))$$

is an order relation between $x = (x_\iota)$ and $y = (y_\iota)$, as is immediately verified. The ordering and the order relation so defined on F are called the *product of the orderings* $\Gamma_\iota$ and the *product of the order relations* $x_\iota \leqslant y_\iota$; this relation is written $x \leqslant y$, and the set F, ordered by the product of the orderings $\Gamma_\iota$, is called the *product of the ordered sets* $E_\iota$.

It is immediately verified that the graph of the product ordering on F is the image of the product set $\prod_{\iota \in I} G_\iota$ under the canonical mapping of $\prod_{\iota \in I} (E_\iota \times E_\iota)$ onto $F \times F$ (Chapter II, § 5, no. 5).

An important example of a product of ordered sets is the set $F^E$ of graphs of mappings of a set E into an ordered set F. There is a canonical bijection of $F^E$ onto the set $\mathfrak{F}(E, F)$ of mappings of E into F, and this mapping is an isomorphism of the ordered set $F^E$ onto $\mathfrak{F}(E, F)$ endowed

with the ordering defined by the relation "for all $x \in E$, $f(x) \leqslant g(x)$" between two mappings $f$, $g$ of E into F.  This relation is written $f \leqslant g$.

☡

It should be observed that in the ordered set $\mathscr{F}(E, F)$, the relation $f < g$ means
$$\text{"for all } x \in E, f(x) \leqslant g(x), \text{ and there exists } y \in E \text{ such that } f(y) < g(y)\text{"}$$
*and not*
$$\text{"for all } x \in E, f(x) < g(x)\text{"}.$$

In order to avoid confusion it is better not to use the notation $f < g$ in this situation.

The definitions of this subsection apply without change to preordered sets when "ordering" is replaced by "preordering" throughout.

### 5. INCREASING MAPPINGS

#### Definition 1 {#ens-iii-s1-def-1 .statement tag=03JC}

*Let* E *and* F *be preordered sets* (*the preorder relation in each being denoted by* $\leqslant$). *A mapping f of* E *into* F *is said to be increasing* (or *order-preserving*) *if the relation* $x \leqslant y$ *implies* $f(x) \leqslant f(y)$; *it is decreasing* (or *order-reversing*) *if the relation* $x \leqslant y$ *implies* $f(x) \geqslant f(y)$. *A mapping of* E *into* F *is said to be monotone if it is either increasing or decreasing.*

An increasing mapping of E into F becomes decreasing (and vice versa) when we replace *one* of the preorderings on E or on F by the opposite preordering.  Every *constant* function is both increasing and decreasing; the converse of this statement is usually not true.

For example, if a set E is ordered by the equality relation, the identity mapping of E onto itself is both increasing and decreasing, but not constant if E has more than one element (cf. Exercise 7).

#### Definition 2 {#ens-iii-s1-def-2 .statement tag=03JD}

*Let* E *and* F *be two ordered sets. A mapping f of* E *into* F *is said to be strictly increasing* (or *strictly order-preserving*) *if the relation* $x < y$ *implies* $f(x) < f(y)$; *f is said to be strictly decreasing* (or *strictly order-reversing*) *if the relation* $x < y$ *implies* $f(x) > f(y)$. *A mapping of* E *into* F *is said to be strictly monotone if it is either strictly increasing or strictly decreasing.*

*Examples*

(1) Let E be a set.  The mapping $X \rightarrow E - X$ of $\mathfrak{P}(E)$ (ordered by inclusion) onto itself is strictly decreasing.

(2) Let E be an ordered set. For each $x \in E$ let $U_x$ be the set of all $y \in E$ such that $y \geqslant x$. The mapping $x \to U_x$ is a strictly decreasing mapping of E into $\mathfrak{P}(E)$ (ordered by inclusion); indeed, the relation $x \leqslant y$ is equivalent to $U_x \supset U_y$.

An injective monotone mapping of an ordered set E into an ordered set F is *strictly monotone*; the converse is usually not true, because it may happen that $f(x) = f(y)$ when neither of the relations $x \leqslant y$, $x \geqslant y$ is true (cf. no. 12, Proposition 11).

¶ A bijective mapping $f$ of an ordered set E onto an ordered set E' is an isomorphism of E onto E' (no. 3) if and only if both $f$ and its inverse mapping are increasing.

¶ If I is an *ordered* index set, a *family of subsets* $(X_\iota)_{\iota \in I}$ of a set E is said to be *increasing* if $\iota \to X_\iota$ is an increasing mapping of I into $\mathfrak{P}(E)$, ordered by inclusion (in other words, if $\iota \leqslant \varkappa$ implies $X_\iota \subset X_\varkappa$). Similarly we define a *decreasing, strictly increasing,* or *strictly decreasing* family of subsets $(X_\iota)_{\iota \in I}$.

#### Proposition 2 {#ens-iii-s1-prop-2 .statement tag=03JE}

*Let* E, E' *be two ordered sets, and let* $u : E \to E'$ *and* $v : E' \to E$ *be two decreasing mappings such that for all* $x \in E$ *and all* $x' \in E'$ *we have* $v(u(x)) \geqslant x$ *and* $u(v(x')) \geqslant x'$. *Then*

$$u \circ v \circ u = u \quad \textit{and} \quad v \circ u \circ v = v.$$

For the relation $v(u(x)) \geqslant x$ implies $(u(v(u(x))) \leqslant u(x)$ because $u$ is decreasing; on the other hand, we have $u(v(u(x))) \geqslant u(x)$ by replacing $x'$ by $u(x)$ in the inequality $u(v(x')) \geqslant x'$. Hence the first equality; the proof of the second is similar.

### 6. MAXIMAL AND MINIMAL ELEMENTS

#### Definition 3 {#ens-iii-s1-def-3 .statement tag=03JF}

*Let* E *be an ordered set. An element* $a \in E$ *is said to be a minimal* (resp. *maximal*) *element of* E *if the relation* $x \leqslant a$ (resp. $x \geqslant a$) *implies* $x = a$.

Every minimal element of E is a maximal element with respect to the opposite ordering, and vice versa.

*Examples*

(1) Let A be a set. In the subset of $\mathfrak{P}(A)$ (ordered by inclusion) consisting of the non-empty subsets of A, the minimal elements are the subsets consisting of a single element.

(2) In the set $\Phi(E, F)$ of mappings of subsets of E into F (F being non-empty), ordered by the relation "$v$ extends $u$" between $u$ and $v$, the maximal elements are the mappings of the whole of E into F.

\* (3) In the set of natural integers $> 1$, ordered by the relation "$m$ divides $n$" between $m$ and $n$, the minimal elements are the prime numbers. $_*$

\* (4) The set of real numbers has no maximal element and no minimal element. $_*$

### 7. GREATEST ELEMENT AND LEAST ELEMENT

If there exists an element $a$ in an ordered set E such that $a \leqslant x$ for all $x \in E$, then $a$ is the *only* element of E with this property; for if also $b \leqslant x$ for all $x \in E$, then we should have $a \leqslant b$ and $b \leqslant a$, and consequently $a = b$.

#### Definition 4 {#ens-iii-s1-def-4 .statement tag=03JG}

*Let* E *be an ordered set. An element* $a \in E$ *is said to be the* least (resp. *greatest*) *element of* E *if for all* $x \in E$ *we have* $a \leqslant x$ (resp. $x \leqslant a$).

An ordered set need not have a greatest element nor a least element. If E has a least element $a$, then $a$ is the greatest element with respect to the opposite ordering.

¶ If E has a least element $a$, then $a$ is the *unique minimal element* of E; for if $x \in E$ is distinct from $a$, we have $a < x$.

*Examples*

(1) Let $\mathfrak{S}$ be a non-empty subset of the set $\mathfrak{P}(E)$ of subsets of a set E. If $\mathfrak{S}$ has a least (resp. greatest) element A with respect to the inclusion relation, then A is the intersection (resp. union) of the sets of $\mathfrak{S}$. Conversely, if the intersection (resp. union) of the sets of $\mathfrak{S}$ belongs to $\mathfrak{S}$, then it is the least (resp. greatest) element of $\mathfrak{S}$.

(2) In particular, $\emptyset$ is the least element and E the greatest element of $\mathfrak{P}(E)$. In the set $\Phi(E, F)$ of mappings of subsets of E into F, ordered by extension of mappings (no. 1, Example 3), the empty mapping is the least element, and there is no greatest element unless F consists of a single element. The diagonal $\Delta$ of $E \times E$ is the least element of the set of graphs of equivalence relations on E (or of the set of preorderings on E).

#### Proposition 3 {#ens-iii-s1-prop-3 .statement tag=03JH}

*Let* E *be an ordered set and let* E$'$ *be the disjoint union of* E *and a set* $\{a\}$ *consisting of a single element. Then there exists a unique ordering on* E$'$ *which induces the given ordering on* E *and for which* $a$ *is the greatest element of* E$'$.

For if G is the graph of the ordering on E, the graph of an ordering on E$'$ which satisfies the conditions of the Proposition must be the union G$'$ of G and the set of all pairs $(x, a)$ where $x \in E'$; conversely, it is clear that G$'$ is the graph of an ordering on E$'$ which satisfies the given conditions.

¶ The ordered set E$'$ is said to be obtained by *adjoining a greatest element* $a$ *to* E (cf. Exercise 3).

¶ A subset A of a preordered set E is said to be *cofinal* (resp. *coinitial*) in E if for every $x\in E$ there exists $y\in A$ such that $x\leq y$ (resp. $y\leq x$). To say that an ordered set E has a greatest (resp. least) element therefore means that E has a cofinal (resp. coinitial) subset consisting of a single element.

### 8. UPPER AND LOWER BOUNDS

#### Definition 5 {#ens-iii-s1-def-5 .statement tag=03JI}

*Let E be a preordered set and let X be a subset of E. Any element $x\in E$ such that $x\leq y$ (resp. $x\geq y$) for all $y\in X$ is called a lower (resp. upper) bound of X in E.*

Every upper bound of X is a lower bound of X with respect to the opposite ordering, and vice versa.

¶ If $x$ is a lower bound of X, every element $z\leq x$ is also a lower bound of X. A lower bound of X is also a lower bound of every subset of X. An ordered set X has a least element if and only if there exists a lower bound of X which belongs to X.

¶ The set of lower bounds of a subset X of a preordered set E may be empty : this is the case when $X=E$ and E is an ordered set which has no least element.

¶ A subset X of E whose set of lower (resp. upper) bounds is not empty is said to be *bounded below* (resp. *bounded above*). A subset which is bounded both below and above is said to be *bounded*. If X is bounded below (resp. bounded above, bounded), the same is true of every subset of X.

Every subset consisting of a single element is bounded. But a subset consisting of two elements need not be bounded either above or below (no. 10).

Let E be a preordered set and let $f$ be a mapping of an arbitrary set A into E. The mapping $f$ is said (by abuse of language) to be *bounded below* (resp. *bounded above, bounded*) if the set $f(A)$ is bounded below (resp. bounded above, bounded) in E.

### 9. LEAST UPPER BOUND AND GREATEST LOWER BOUND

#### Definition 6 {#ens-iii-s1-def-6 .statement tag=03JJ}

*Let E be an ordered set and let X be a subset of E. An element of E is said to be the greatest lower bound or infimum (resp. least upper bound or supremum) of X in E if it is the greatest (resp. least) element of the set of lower (resp. upper) bounds of X in E.*

Given a subset X of an ordered set E, the least upper bound (resp. greatest lower bound) of X in E, when it exists, is denoted by

$$
\operatorname{sup}_{E}X\quad(\text{resp. }\operatorname{inf}_{E}X)
$$

or by sup X (resp. inf X) if there is no risk of ambiguity. The least upper bound (resp. greatest lower bound) of a set $\{x, y\}$ of two elements, when it exists, is denoted by sup $(x, y)$ (resp. inf $(x, y)$). Similarly for the least upper bound and greatest lower bound of a set of three elements, etc.

¶ If a subset X of E has a greatest element $a$, then $a$ is the least upper bound of X in E.

¶ If X has a greatest lower bound $a$ in E, then $a$ is the least upper bound of X with respect to the opposite ordering on E. For this reason we may restrict ourselves for the most part, in what follows, to consideration of the properties of least upper bounds.

*Examples*

(1) The set of upper bounds of the empty set $\emptyset$ in an ordered set E is evidently E itself; hence $\emptyset$ has a supremum in E if and only if E has a *least* element, which is then the *least upper bound* of $\emptyset$.

(2) In the set $\mathfrak{P}(E)$ of subsets of a set E, ordered by inclusion, every subset $\mathfrak{S}$ of $\mathfrak{P}(E)$ has a least upper bound, namely the *union* of the sets of $\mathfrak{S}$, and a greatest lower bound, namely the *intersection* of the sets of $\mathfrak{S}$.

(3) Let E, F be two sets and let $\Theta$ be a subset of the $\Phi(E, F)$ of mappings of subsets of E into F, ordered by extension of mappings (no. 1, Example 3). For each $u \in \Phi(E, F)$ let $D(u)$ be the domain of $u$. The condition for the existence of a common extension of a family of mappings belonging to $\Phi(E, F)$ (Chapter II, § 4, no. 6, Proposition 7) shows that $\Theta$ has a least upper bound in $\Phi(E, F)$ if and only if for each pair $(u, v)$ of elements of $\Theta$ we have $u(x) = v(x)$ whenever $x \in D(u) \cap D(v)$.

A mapping $f$ of a set A into an ordered set E is said to have a least upper bound if the image $f(A)$ has a least upper bound in E; this bound is then called the *least upper bound of f* and is written $\sup_{x \in A} f(x)$. Similarly for the greatest lower bound.

In particular, if a subset A of E has a least upper bound in E, this bound is the least upper bound of the canonical injection of A into E, and may therefore be written as $\sup_{x \in A} x$.

#### Proposition 4 {#ens-iii-s1-prop-4 .statement tag=03JK}

*Let* E *be an ordered set and let* A *be a subset of* E *which has both a greatest lower bound and a least upper bound in* E. *Then* $\inf A \leqslant \sup A$ *if* $A \neq \emptyset$; *if* $A = \emptyset$, $\sup A$ *is the least and* $\inf A$ *the greatest element of* E.

This follows immediately from the definitions.

#### Proposition 5 {#ens-iii-s1-prop-5 .statement tag=03JL}

*Let* E *be an ordered set and let* A, B *be two subsets of* E, *each of which has a least upper bound* (resp. *greatest lower bound*) *in* E. *If* $A \subset B$, *then* $\sup A \leqslant \sup B$ (resp. $\inf A \geqslant \inf B$).

#### Corollary {#ens-iii-s1-n9-cor-1 .statement tag=03JM}

*Let $(x_\iota)_{\iota \in I}$ be a family of elements of an ordered set* $\mathrm{E}$ *which has a least upper bound in* $\mathrm{E}$. *If* $\mathrm{J}$ *is a subset of* $\mathrm{I}$ *such that the family* $(x_\iota)_{\iota \in J}$ *has a least upper bound in* $\mathrm{E}$, *we have* $\sup\limits_{\iota \in J} x_\iota \leqslant \sup\limits_{\iota \in I} x_\iota$.

#### Proposition 6 {#ens-iii-s1-prop-6 .statement tag=03JN}

*Let* $(x_\iota)_{\iota \in I}$, $(y_\iota)_{\iota \in I}$ *be two families of elements of an ordered set* $\mathrm{E}$, *indexed by the same set* $\mathrm{I}$, *and such that* $x_\iota \leqslant y_\iota$ *for all* $\iota \in \mathrm{I}$. *If both families have a least upper bound in* $\mathrm{E}$, *then* $\sup\limits_{\iota \in I} x_\iota \leqslant \sup\limits_{\iota \in I} y_\iota$.

For $a = \sup\limits_{\iota \in I} y_\iota$ is an upper bound of the set of the $y_\iota$, so that $x_\iota \leqslant y_\iota \leqslant a$ for all $\iota \in \mathrm{I}$, and hence $\sup\limits_{\iota \in I} x_\iota \leqslant a$.

#### Proposition 7 {#ens-iii-s1-prop-7 .statement tag=03JO}

*Let* $(x_\iota)_{\iota \in I}$ *be a family of elements of an ordered set* $\mathrm{E}$, *and let* $(\mathrm{J}_\lambda)_{\lambda \in L}$ *be a covering of the index set* $\mathrm{I}$. *Suppose that each of the subfamilies* $(x_\iota)_{\iota \in J_\lambda}$ *has a least upper bound in* $\mathrm{E}$. *For the family* $(x_\iota)_{\iota \in I}$ *to have a least upper bound in* $\mathrm{E}$, *it is necessary and sufficient that the family* $\left( \sup\limits_{\iota \in J_\lambda} x_\iota \right)_{\lambda \in L}$ *should have a least upper bound in* $\mathrm{E}$, *and then we have*

$$(1) \qquad \sup_{\iota \in I} x_\iota = \sup_{\lambda \in L} \left( \sup_{\iota \in J_\lambda} x_\iota \right).$$

Let $b_\lambda = \sup\limits_{\iota \in J_\lambda} x_\iota$. Suppose that $(x_\iota)_{\iota \in I}$ has a least upper bound $a$. Then $a \geqslant b_\lambda$ for each $\lambda \in \mathrm{L}$ (Corollary to Proposition 5). On the other hand, if $c \geqslant b_\lambda$ for each $\lambda \in \mathrm{L}$, then we have $c \geqslant x_\iota$ for each $\iota \in \mathrm{I}$, because $(\mathrm{J}_\lambda)_{\lambda \in L}$ is a covering of $\mathrm{I}$; hence $c \geqslant a$, which proves that

$$a = \sup_{\lambda \in L} b_\lambda.$$

Conversely, suppose that the family $(b_\lambda)_{\lambda \in L}$ has a least upper bound $a'$. Then $a' \geqslant x_\iota$ for all $\iota \in \mathrm{I}$. On the other hand, if $c' \geqslant x_\iota$ for all $\iota \in \mathrm{I}$, then we have in particular

$$c' \geqslant \sup_{\iota \in J_\lambda} x_\iota = b_\lambda$$

for each $\lambda \in \mathrm{L}$, so that $c' \geqslant a'$ and therefore

$$a' = \sup_{\iota \in I} x_\iota.$$

#### Corollary {#ens-iii-s1-n9-cor-2 .statement tag=03JP}

*Let* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *be a "double" family of elements of an ordered set* $\mathrm{E}$ *such that for each* $\mu \in \mathrm{M}$ *the family* $(x_{\lambda\mu})_{\lambda \in L}$ *has a least upper bound in* $\mathrm{E}$. *For the family* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *to have a least upper bound in* $\mathrm{E}$, *it is necessary and sufficient that the family* $\left( \sup\limits_{\lambda \in L} x_{\lambda\mu} \right)_{\mu \in M}$ *should have a least*

*upper bound in* E, *and then we have*

$$(2) \qquad \sup_{(\lambda,\,\mu)\in L\times M} x_{\lambda\mu} = \sup_{\mu\in M}\left(\sup_{\lambda\in L} x_{\lambda\mu}\right).$$

**Proposition 8.** *Let* $(E_\iota)_{\iota\in I}$ *be a family of ordered sets. Let* A *be a subset of the product ordered set* $E = \prod_{\iota\in I} E_\iota$, *and let* $A_\iota = \mathrm{pr}_\iota A$ *for each* $\iota \in I$. *For* A *to have a least upper bound in* E *it is necessary and sufficient that, for each* $\iota \in I$, $A_\iota$ *should have a least upper bound in* $E_\iota$, *and then we have*

$$\sup A = (\sup A_\iota)_{\iota\in I} = \left(\sup_{x\in A} \mathrm{pr}_\iota x\right)_{\iota\in I}.$$

Suppose that, for each $\iota \in I$, $A_\iota$ has a least upper bound $b_\iota$ in $E_\iota$. To say that $c = (c_\iota)$ is an upper bound of A then means that $c_\iota \geqslant b_\iota$ for each $\iota \in I$, hence $(b_\iota)_{\iota\in I}$ is an upper bound of A. Conversely, suppose that A has a least upper bound $a = (a_\iota)_{\iota\in I}$; for each $\varkappa \in I$, $a_\varkappa$ is an upper bound of $A_\varkappa$, because if $x_\varkappa \in A_\varkappa$, there exists $x \in A$ such that $\mathrm{pr}_\varkappa x = x_\varkappa$, by the definition of $A_\varkappa$; on the other hand, if $a'_\varkappa$ is an upper bound of $A_\varkappa$ in $E_\varkappa$, the element $c' = (c'_\iota)_{\iota\in I}$ for which

$$c'_\iota = a_\iota \quad \text{for} \quad \iota \neq \varkappa \qquad \text{and} \qquad c'_\varkappa = a'_\varkappa$$

is an upper bound of A; consequently $c' \geqslant a$ and therefore $a'_\varkappa \geqslant a_\varkappa$; hence $a_\varkappa$ is the least upper bound of $A_\varkappa$ in $E_\varkappa$.

☡

¶ Let F be a subset of an ordered set E, and let A be a subset of F. It can happen that one of the two elements $\sup_E A$, $\sup_F A$ exists but the other does not, or that both exist but are unequal.

*Examples*

\* (1) In the ordered set $E = \mathbf{R}$ of real numbers, consider the subset $F = \mathbf{Q}$ of rational numbers and the set $A \subset F$ of rational numbers $< \sqrt{2}$; $\sup_E A$ exists but $\sup_F A$ does not.

(2) In the notation of Example 1, let G be the union of A and the set $\{2\}$; then $G \subset F$ and $\sup_G A$ exists, but $\sup_F A$ does not.

(3) With the same notation, $\sup_E A = \sqrt{2}$, $\sup_G A = 2$. \*

However, we have the following result :

**Proposition 9.** *Let* E *be an ordered set,* F *a subset of* E, A *a subset of* F. *If both* $\sup_E A$ *and* $\sup_F A$ *exist, we have* $\sup_E A \leqslant \sup_F A$. *If* $\sup_E A$ *exists and belongs to* F, *then* $\sup_F A$ *exists and is equal to* $\sup_E A$.

The first assertion follows from the fact that the set $\mathrm{M}$ of upper bounds of A in F is contained in the set N of upper bounds of A in E, and from Proposition 5. On the other hand, if the least element of N lies in F, then it belongs to M and is clearly the least element of M; this proves the second assertion.

### 10. DIRECTED SETS

**Definition 7.** *A preordered set* E *is said to be right directed* (resp. *left directed*) *if every subset of two elements of* E *is bounded above* (resp. *bounded below*).

In place of "right directed" we shall often use the expression "directed with respect to the relation $\leqslant$", and analogous expressions when the preorder relation is denoted by some other sign. For example, if $\mathfrak{S}$ is a set of subsets of a set A, we say that $\mathfrak{S}$ is *directed with respect to the relation* $\subset$ (resp. $\supset$) if, for each subset $\{\mathrm{X}, \mathrm{Y}\}$ consisting of two elements of $\mathfrak{S}$, there exists $\mathrm{Z} \in \mathfrak{S}$ such that $\mathrm{X} \subset \mathrm{Z}$ and $\mathrm{Y} \subset \mathrm{Z}$ (resp. $\mathrm{X} \supset \mathrm{Z}$ and $\mathrm{Y} \supset \mathrm{Z}$).

*Examples*
(1) An ordered set which has a greatest element is right directed.
\* (2) In a topological space, a fundamental system of neighbourhoods of a point is directed with respect to the relation $\supset$.
(3) The set of submodules of finite type of an arbitrary module is directed with respect to the relation $\subset$. \*

**Proposition 10.** *In a right directed ordered set* E, *a maximal element a is the greatest element of* E.

For every $x \in \mathrm{E}$ there exists by hypothesis $y \in \mathrm{E}$ such that $x \leqslant y$ and $a \leqslant y$; since $a$ is maximal, $y = a$.

¶ A right directed preordered set is left directed with respect to the opposite ordering. Any product of right directed sets is right directed. On the other hand, a subset of a right directed set is not necessarily right directed. However, a *cofinal* subset F of a right directed set E is always right directed; for given $x$, $y \in \mathrm{F}$ there exists $z \in \mathrm{E}$ such that $x \leqslant z$ and $y \leqslant z$, and then $t \in \mathrm{F}$ such that $z \leqslant t$.

### 11. LATTICES

**Definition 8.** *An ordered set* E *is said to be a lattice if every subset consisting of two elements of* E *has a least upper bound and a greatest lower bound in* E.

Every product of lattices is a lattice; this follows from the condition for the existence of a least upper bound in a product of ordered sets (no. 9, Proposition 8). The set of subsets of a set A, ordered by inclusion, is a lattice

because the union and intersection of two subsets of A are again subsets of A.

*Examples*

* (1) The set of integers $\geq 1$, ordered by the relation “$m$ divides $n$” between $m$ and $n$, is a lattice; the least upper bound of $\{m,n\}$ is the l.c.m. of $m$ and $n$, and the greatest lower bound is their h.c.f.
(2) The set of subgroups of a group G, ordered by inclusion, is a lattice.
(3) The set of topologies on a set A, ordered by the relation “$\mathcal{T}$ is coarser than $\mathcal{T}'$” between $\mathcal{T}$ and $\mathcal{T}'$, is a lattice. (General Topology, Chapter I, § 2).
(4) The set $\mathscr{F}(I,\mathbf{R})$ of all real-valued functions defined on an interval I of $\mathbf{R}$ is a lattice with respect to the order relation $f\leq g$ (no. 4), and as such is isomorphic to the product $\mathbf{R}^{I}$. *

#### Remark {#ens-iii-s1-n11-rem-1 .statement tag=03JQ}

A lattice is obviously both left and right directed. But an ordered set which is both left and right directed is not necessarily a lattice. * An example of the latter is the set of mappings $x\mapsto p(x)$ of $\mathbf{R}$ into itself, where $p$ is a polynomial in $\mathbf{R}[X]$, this set being ordered by the relation $p\leq q$ (no. 4). *

### 12. TOTALLY ORDERED SETS

#### Definition 9 {#ens-iii-s1-def-9 .statement tag=03JR}

*Two elements $x$, $y$ of a preordered set E are said to be comparable if the relation “$x\leq y$ or $y\leq x$” is true. A set E is said to be totally ordered if it is ordered and if any two elements of E are comparable. The ordering on E is then said to be a total ordering, and the corresponding order relation a total order relation.*

If $x$ and $y$ are elements of a totally ordered set, then $x=y$ or $x<y$ or $x>y$; the negation of $x\leq y$ is thus $x>y$.

An ordering on E is a total ordering if and only if its graph G satisfies the relation $G\cup G^{-1}=E\times E$, as well as the relations $G\circ G=G$ and $G\cap G^{-1}=\Delta$.

*Examples*

(1) Every subset of a totally ordered set is totally ordered by the induced ordering.
(2) Let E be an arbitrary ordered set. The empty subset of E is totally ordered, and so is every subset of E consisting of a single element.
* (3) The set $\mathbf{R}$ of real numbers is totally ordered. *
(4) If A is a set which has at least two distinct elements, the set $\mathscr{P}(A)$ (ordered by inclusion) is not totally ordered, for if $x\neq y$, the subsets $\{x\}$ and $\{y\}$ are not comparable.

A totally ordered set is also totally ordered with respect to the opposite ordering; it is a lattice and *a fortiori* both left and right directed.

#### Proposition 11 {#ens-iii-s1-prop-11 .statement tag=03JS}

*Every strictly monotone mapping $f$ of a totally ordered set* E *into an ordered set* F *is injective. If $f$ is strictly increasing, $f$ is an isomorphism of* E *onto $f(\mathrm{E})$.*

For $x \neq y$ implies that either $x < y$ or $x > y$; hence

$$f(x) < f(y) \qquad \text{or} \qquad f(x) > f(y),$$

so that $f(x) \neq f(y)$ in either case. It remains to be shown that if $f$ is strictly increasing, $f(x) \leqslant f(y)$ implies $x \leqslant y$; if not, we should have $x > y$, and therefore $f(x) > f(y)$.

#### Proposition 12 {#ens-iii-s1-prop-12 .statement tag=03JT}

*Let* E *be a totally ordered set and let* X *be a subset of* E. *For an element $b$ of* E *to be the least upper bound of* X *in* E, *it is necessary and sufficient that* (1) *$b$ is an upper bound of* X, (2) *for every $c \in \mathrm{E}$ such that $c < b$, there exists $x \in \mathrm{X}$ such that $c < x \leqslant b$.*

The second condition says that no element $c < b$ is an upper bound of X, i.e., $b$ is a minimal element of the set M of upper bounds of X; but this is the same as saying that $b$ is the least element of M, since M is totally ordered (no. 10, Proposition 10).

### 13. INTERVALS

Let E be an ordered set and let $a$, $b$ be two elements of E such that $a \leqslant b$. The subset of E consisting of elements $x$ such that $a \leqslant x \leqslant b$ is called the *closed interval with left-hand endpoint a and right-hand endpoint b*, and is denoted by $[a, b]$. The set of all $x \in \mathrm{E}$ such that $a \leqslant x < b$ (resp. $a < x \leqslant b$) is called the *interval half-open on the right* (resp. *on the left*) with endpoints $a$ and $b$, and is denoted by $[a, b[$ (resp. $]a, b])$. The set of all $x \in \mathrm{E}$ such that $a < x < b$ is called the *open interval* with endpoints $a$ and $b$, and is denoted by $]a, b[$.

Note that a closed interval is never empty; the interval $[a, a]$ is the set $\{a\}$. On the other hand, the intervals $[a, a[$, $]a, a]$, $]a, a[$ are all empty; and an open interval $]a, b[$ may be empty even when $a < b$.

Let $a$ be an element of E. The set of all $x \in \mathrm{E}$ such that $x \leqslant a$ (resp. $x < a$) is called the *closed* (resp. *open*) *interval unbounded on the left, with right-hand endpoint a*, and is denoted by $]{\leftarrow}, a]$ (resp. $]{\leftarrow}, a[$); likewise, the set of all $x \in \mathrm{E}$ such that $x \geqslant a$ (resp. $x > a$) is called the *closed* (resp. *open*) *interval with left-hand endpoint a, unbounded on the right*, and is denoted by $[a, {\rightarrow}[$ (resp. $]a, {\rightarrow}[$). Finally, E itself may be

regarded as the *open interval unbounded on the left and on the right*, denoted by $]\leftarrow, \rightarrow[$.

#### Proposition 13 {#ens-iii-s1-prop-13 .statement tag=03JU}

*In a lattice, the intersection of two intervals is an interval.* Consider for example the intersection of two closed intervals $[a, b]$ and $[c, d]$, and let $\alpha = \sup (a, c)$, $\beta = \inf (b, d)$. If both $a \leqslant x \leqslant b$ and $c \leqslant x \leqslant d$, then we have $\alpha \leqslant x \leqslant \beta$, and conversely; if $\alpha \not\leqslant \beta$, the intersection of $[a, b]$ and $[c, d]$ is empty; if $\alpha \leqslant \beta$, this intersection is $[\alpha, \beta]$. We leave it to the reader to carry through the proof for the other cases.

### Exercises {#ens-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
