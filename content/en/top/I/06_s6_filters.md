---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 6
section_title: Filters
lang: en
source: top-i-iv
book_pages: 57-68
pdf_pages: 0063-0074, 0135-0138
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A FILTER
      page: 57
      pdf_page: 63
    - "no": 2
      title: COMPARISON OF FILTERS
      page: 58
      pdf_page: 64
    - "no": 3
      title: BASES OF A FILTER
      page: 59
      pdf_page: 65
    - "no": 4
      title: ULTRAFILTERS
      page: 60
      pdf_page: 66
    - "no": 5
      title: INDUCED FILTER
      page: 61
      pdf_page: 67
    - "no": 6
      title: DIRECT IMAGE AND INVERSE IMAGE OF A FILTER BASE
      page: 62
      pdf_page: 68
    - "no": 7
      title: PRODUCT OF FILTERS
      page: 63
      pdf_page: 69
    - "no": 8
      title: ELEMENTARY FILTERS
      page: 64
      pdf_page: 70
    - "no": 9
      title: GERMS WITH RESPECT TO A FILTER
      page: 65
      pdf_page: 71
    - "no": 10
      title: GERMS AT A POINT
      page: 68
      pdf_page: 74
statements: 30
exercises: 20
content_sha256: 6819de812cc0a066f3d9d41f17299c6a6b5cfd00b8e0cf993c3f1e890810bef8
---

## 6. FILTERS

### 1. DEFINITION OF A FILTER

#### Definition 1 {#top-i-s6-def-1 .statement}

*A filter on a set $X$ is a set $\mathfrak{F}$ of subsets of $X$ which has the following properties:*

$(\mathrm{F}_1)$ *Every subset of $X$ which contains a set of $\mathfrak{F}$ belongs to $\mathfrak{F}$.*
$(\mathrm{F}_\mathrm{II})$ *Every finite intersection of sets of $\mathfrak{F}$ belongs to $\mathfrak{F}$.*
$(\mathrm{F}_\mathrm{III})$ *The empty set is not in $\mathfrak{F}$.*

It follows from $(\mathrm{F}_\mathrm{II})$ and $(\mathrm{F}_\mathrm{III})$ that every finite intersection of sets of $\mathfrak{F}$ is *non-empty*.

A filter $\mathfrak{F}$ on $X$ defines a structure on $X$, the axioms of which are $(\mathrm{F}_1)$, $(\mathrm{F}_\mathrm{II})$ and $(\mathrm{F}_\mathrm{III})$; this structure is called a *structure of a filtered set*, and the set $X$ endowed with this structure is called a *set filtered by* $\mathfrak{F}$.

Axiom $(\mathrm{F}_\mathrm{II})$ is equivalent to the conjunction of the following two axioms:
$(\mathrm{F}_{\mathrm{II}\,\mathrm{a}})$ *The intersection of two sets of $\mathfrak{F}$ belongs to $\mathfrak{F}$.*
$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ *$X$ belongs to $\mathfrak{F}$.*

Axioms $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ and $(\mathrm{F}_\mathrm{III})$ show that *there is no filter on the empty set*.

In order for a set of subsets which satisfies $(\mathrm{F}_1)$ also to satisfy $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ it is necessary and sufficient that it is *not empty*. A set of subsets which satisfies $(\mathrm{F}_1)$ also satisfies $(\mathrm{F}_\mathrm{III})$ if and only if it is different from $\mathscr{P}(X)$.

*Examples of filters.* 1) If $X \neq \varnothing$, the set of subsets consisting of $X$ alone is a filter on $X$. More generally, the set of all subsets of $X$ which contain a given non-empty subset $A$ of $X$ is a filter on $X$.

2) In a topological space $X$, the *set of all neighbourhoods* of an arbitrary non-empty subset $A$ of $X$ (and in particular the set of all neighbourhoods of a point of $X$) is a filter, called the *neighbourhood filter* of $A$.

3) If $X$ is an *infinite* set, the *complements of the finite subsets* of $X$ are the elements of a filter. The filter of complements of finite subsets of the set $\mathbf{N}$ of integers $\geqslant 0$ is called the *Fréchet filter*.

### 2. COMPARISON OF FILTERS

#### Definition 2 {#top-i-s6-def-2 .statement}

Given two filters $\mathfrak{F}, \mathfrak{F}'$ on the same set $X$, $\mathfrak{F}'$ is said to be finer than $\mathfrak{F}$, or $\mathfrak{F}$ is coarser than $\mathfrak{F}'$, if $\mathfrak{F} \subset \mathfrak{F}'$. If also $\mathfrak{F} \neq \mathfrak{F}'$, then $\mathfrak{F}'$ is said to be strictly finer than $\mathfrak{F}$, or $\mathfrak{F}$ strictly coarser than $\mathfrak{F}'$.

Two filters are said to be comparable if one is finer than the other. The set of all filters on $X$ is ordered by the relation " $\mathfrak{F}$ is coarser than $\mathfrak{F}'$"; this relation is induced by the inclusion relation in $\mathscr{P}(\mathscr{P}(X))$.

Let $(\mathfrak{F}_i)_{i \in I}$ be any non-empty family of filters on a set $X$ (which must therefore be non-empty); then the set

$$
\mathfrak{F} = \bigcap_{i \in I} \mathfrak{F}_i
$$

satisfies axioms $(F_I), (F_{II})$ and $(F_{III})$ and is therefore a filter; $\mathfrak{F}$ is called the intersection of the family of filters $(\mathfrak{F}_i)_{i \in I}$ and is obviously the greatest lower bound of the set of the $\mathfrak{F}_i$ in the ordered set of all filters on $X$.

The filter formed by the single set $X$ is the smallest element of the ordered set of all filters on $X$. We shall see in no. 4 that, if $X$ has more than one element, the set of all filters on $X$ has no greatest element.

Given a set $\mathscr{G}$ of subsets of a set $X$, let us consider whether there are any filters on $X$ which contain $\mathscr{G}$. If such a filter exists then by $(F_{II})$ it contains also the set $\mathscr{G}'$ of finite intersections of sets of $\mathscr{G}$ (including $X$, which is the intersection of the empty subset of $\mathscr{G}$); hence a necessary condition for such a filter to exist is that the empty subset of $X$ is not in $\mathscr{G}'$. This condition is also sufficient, for by $(F_I)$ any filter which contains $\mathscr{G}'$ also contains the set $\mathscr{G}''$ of subsets of $X$ which contain a set of $\mathscr{G}'$. Now $\mathscr{G}''$ clearly satisfies $(F_I)$; it satisfies $(F_{II})$ by reason of the definition of $\mathscr{G}'$; and finally it satisfies $(F_{III})$ because the empty subset of $X$ does not belong to $\mathscr{G}'$. Hence $\mathscr{G}''$ is the coarsest filter which contains $\mathscr{G}$, and we have proved:

#### Proposition 1 {#top-i-s6-prop-1 .statement}

A necessary and sufficient condition that there should exist a filter on $X$ containing a set $\mathscr{G}$ of subsets of $X$ is that no finite subset of $\mathscr{G}$ has an empty intersection.

The filter $\mathscr{G}''$ defined above is said to be generated by $\mathscr{G}$, and $\mathscr{G}$ is said to be a subbase of $\mathscr{G}''$.

#### Example {#top-i-s6-n2-exa-1 .statement}

Let $\mathscr{S}$ be any set of subsets of a set $X$, and let $\mathscr{T}$ be the topology on $X$ generated by $\mathscr{S}$ ($\S$ 2, no. 3, Example II). Since the set of finite intersections of sets of $\mathscr{S}$ is a base of $\mathscr{T}$, it follows from the proof of Proposition 1 above and from Proposition 3 of $\S$ 1, no. 3 that for each $x \in X$ the neighbourhood filter of $x$ for $\mathscr{T}$ is generated by the set $\mathscr{G}(x)$ of sets of $\mathscr{S}$ which contain $x$.

#### Corollary 1 {#top-i-s6-prop-1-cor-1 .statement}

Let $\mathfrak{F}$ be a filter on a set $X$, and $A$ a subset of $X$. Then there is a filter $\mathfrak{F}'$ which is finer than $\mathfrak{F}$ and such that $A \in \mathfrak{F}'$, if and only if $A$ meets all the sets of $\mathfrak{F}$.

#### Corollary 2 {#top-i-s6-prop-1-cor-2 .statement}

A set $\Phi$ of filters on a non-empty set $X$ has a least upper bound in the set of all filters on $X$ if and only if, for all finite sequences $(\mathfrak{F}_i)_{1 \leq i \leq n}$ of elements of $\Phi$ and all $A_i \in \mathfrak{F}_i$ ($1 \leq i \leq n$), the intersection $A_1 \cap \cdots \cap A_n$ is not empty.

For this condition expresses that the union $\mathscr{G}$ of the filters $\mathfrak{F} \in \Phi$ satisfies the condition of Proposition 1.

#### Corollary 3 {#top-i-s6-prop-1-cor-3 .statement}

The ordered set of all filters on a non-empty set $X$ is inductive.

For every linearly ordered set $\Phi$ of filters on $X$ satisfies the condition of Corollary 2 of Proposition 1, since the sets $A_i$ all belong to the same $\mathfrak{F}_j$ by hypothesis, and we can apply $(\mathrm{F}_{\mathrm{II}})$.

### 3. BASES OF A FILTER

If $\mathscr{G}$ is a subbase of a filter $\mathfrak{F}$ on $X$ (no. 2), then $\mathfrak{F}$ is not in general the set of subsets of $X$ which contain a set of $\mathscr{G}$; for $\mathscr{G}$ to have this property it is necessary and sufficient that every finite intersection of sets of $\mathscr{G}$ should contain a set of $\mathscr{G}$. Hence the following proposition:

#### Proposition 2 {#top-i-s6-prop-2 .statement}

Let $\mathscr{B}$ be a set of subsets of a set $X$. Then the set of subsets of $X$ which contain a set of $\mathscr{B}$ is a filter if and only if $\mathscr{B}$ has the following two properties:
(B_I) The intersection of two sets of $\mathscr{B}$ contains a set of $\mathscr{B}$.
(B_{II}) $\mathscr{B}$ is not empty, and the empty subset of $X$ is not in $\mathscr{B}$.

#### Definition 3 {#top-i-s6-def-3 .statement}

A set $\mathscr{B}$ of subsets of a set $X$ which satisfies axioms (B_I) and (B_{II}) is said to be a base of the filter it generates. Two filter bases are said to be equivalent if they generate the same filter.

If $\mathscr{G}$ is a subbase of a filter $\mathfrak{F}$, then the set $\mathscr{G}'$ of finite intersections of sets of $\mathscr{G}$ is a base of $\mathfrak{F}$ (no. 2).

#### Proposition 3 {#top-i-s6-prop-3 .statement}

A subset $\mathscr{B}$ of a filter $\mathfrak{F}$ on $X$ is a base of $\mathfrak{F}$ if and only if every set of $\mathfrak{F}$ contains a set of $\mathscr{B}$.

If $\mathscr{B}$ is a base of $\mathfrak{F}$, then clearly every set of $\mathfrak{F}$ contains a set of $\mathscr{B}$; conversely, if every set of $\mathfrak{F}$ contains a set of $\mathscr{B}$, then the set of subsets of $X$ containing a set of $\mathscr{B}$ coincides with $\mathfrak{F}$ by reason of $(\mathrm{F}_1)$.

#### Proposition 4 {#top-i-s6-prop-4 .statement}

On a set $X$, a filter $\mathscr{F}'$ with base $\mathscr{B}'$ is finer than a filter $\mathscr{F}$ with base $\mathscr{B}$ if and only if every set of $\mathscr{B}$ contains a set of $\mathscr{B}'$.

This is an immediate consequence of Definitions 2 and 3.

#### Corollary {#top-i-s6-n3-cor-1 .statement}

Two filter bases $\mathscr{B}, \mathscr{B}'$ on a set $X$ are equivalent if and only if every set of $\mathscr{B}$ contains a set of $\mathscr{B}'$ and every set of $\mathscr{B}'$ contains a set of $\mathscr{B}$.

Examples of filter bases. 1) Let $X$ be a topological space. Proposition 3 shows that the bases of the neighbourhood filter of a point $x \in X$ are precisely the fundamental systems of neighbourhoods of $x$ (§ 1, no. 3, Definition 5).

2) Let $X$ be a non-empty directed set with respect to a relation $(\sigma)$ (Set Theory, Chapter III, § 1, no. 10). For each $a \in X$, the set $S(a)$ of all $x \in X$ such that $a(\sigma)x$ will be called the section of $X$ relative to the element $a$. Then the set $\mathscr{S}$ of sections of $X$ is a filter base, for it clearly satisfies $(\mathrm{B}_{\mathrm{II}})$, and if $a, b$ are any two elements of $X$, then there is by hypothesis an element $c \in X$ such that $a(\sigma)c$ and $b(\sigma)c$, and therefore
$$
S(c) \subset S(a) \cap S(b),
$$
so that $(\mathrm{B}_1)$ is satisfied. The filter generated by $\mathscr{S}$ is called the section filter of the directed set $X$.

For example, the Fréchet filter (no. 1) is the section filter of the ordered set $\mathbf{N}$, considered as directed by the relation $\leqslant$.
Let $\mathscr{F}$ be a filter on a set $Z$. Since $\mathscr{F}$ is directed with respect to the relation $\supset$ [by reason of axiom $(\mathrm{F}_{\mathrm{II}})$] we can define a section filter on $\mathscr{F}$; here a section of $\mathscr{F}$ relative to a set $A \in \mathscr{F}$ is the set $S(A)$ of all $M \in \mathscr{F}$ such that $M \subset A$. This filter is called the section filter of the filter $\mathscr{F}$.

### 4. ULTRAFILTERS

#### Definition 4 {#top-i-s6-def-4 .statement}

An ultrafilter on a set $X$ is a filter $\mathscr{F}$ such that there is no filter on $X$ which is strictly finer than $\mathscr{F}$ (in other words, a maximal element in the ordered set of all filters on $X$).

Since the ordered set of all filters on $X$ is inductive (no. 2, Proposition 1, Corollary 3), Zorn's lemma (Set Theory, R, § 6, no. 10) shows that:

#### Theorem 1 {#top-i-s6-thm-1 .statement}

If $\mathscr{F}$ is any filter on a set $X$, there is an ultrafilter finer than $\mathscr{F}$.

#### Proposition 5 {#top-i-s6-prop-5 .statement}

Let $\mathscr{F}$ be an ultrafilter on a set $X$. If $A$ and $B$ are two subsets of $X$ such that $A \cup B \in \mathscr{F}$, then either $A \in \mathscr{F}$ or $B \in \mathscr{F}$.

If the proposition is false, there exist subsets $A$ and $B$ of $X$ such that $A \notin \mathscr{F}$ and $B \notin \mathscr{F}$ and $A \cup B \in \mathscr{F}$. Let $\mathscr{G}$ be the set of subsets $M$ of $X$ such that $A \cup M \in \mathscr{F}$. It is straightforward to check that $\mathscr{G}$ is a filter on $X$, and $\mathscr{G}$ is strictly finer than $\mathscr{F}$, since $B \in \mathscr{G}$; but this contradicts the hypothesis that $\mathscr{F}$ is an ultrafilter.

#### Corollary {#top-i-s6-n4-cor-1 .statement}

*If the union of a finite sequence* $(A_i)_{1 \leq i \leq n}$ *of subsets of* $X$ *belongs to an ultrafilter* $\mathscr{F}$, *then at least one of the* $A_i$ *belongs to* $\mathscr{F}$.

Proof is by induction on $n$.
In particular, if $(A_i)_{1 \leq i \leq n}$ is a *covering* of $X$, then at least one of the $A_i$ belongs to $\mathscr{F}$.
Proposition 5 *characterizes* the ultrafilters; more generally, we have:

#### Proposition 6 {#top-i-s6-prop-6 .statement}

*Let* $\mathscr{G}$ *be a subbase of a filter on a set* $X$. *If for each subset* $Y$ *of* $X$ *we have either* $Y \in \mathscr{G}$ *or* $\complement Y \in \mathscr{G}$, *then* $\mathscr{G}$ *is an ultrafilter on* $X$.

Let $\mathscr{F}$ be a filter containing $\mathscr{G}$ (there is one, by hypothesis); then $\mathscr{F}$ coincides with $\mathscr{G}$; for if $Y \in \mathscr{F}$ then $\complement Y \notin \mathscr{F}$; hence $\complement Y \notin \mathscr{G}$ and therefore $Y \in \mathscr{G}$.

*Example of an ultrafilter.* The set of all subsets of a non-empty set $X$ which contain a given element $a \in X$ is an ultrafilter; for it is a filter, and if $Y$ is any subset of $X$ then either $a \in Y$ or $a \in \complement Y$. Such ultrafilters are called *trivial*.

Apart from this example, we shall never prove the existence of an ultrafilter (even on a countably infinite set) except by using Theorem 1 (and therefore the axiom of choice).

#### Remark {#top-i-s6-n4-rem-1 .statement}

If $X$ contains at least two elements, there are at least two distinct ultrafilters on $X$, and therefore the ordered set of filters on $X$ has no greatest element.

#### Proposition 7 {#top-i-s6-prop-7 .statement}

*Every filter* $\mathscr{F}$ *on a set* $X$ *is the intersection of the ultrafilters finer than* $\mathscr{F}$.

Clearly this intersection contains $\mathscr{F}$. Conversely, let $A$ be a subset of $X$ which does not belong to $\mathscr{F}$, and let $A'$ denote $\complement A$; $A$ contains no set of $\mathscr{F}$; hence every $M \in \mathscr{F}$ meets $A'$ and therefore (no. 2, Proposition 1, Corollary 1) there is a filter $\mathscr{F}'$ which is finer than $\mathscr{F}$ and contains $A'$. If $\mathscr{U}$ is an ultrafilter finer than $\mathscr{F}'$ (Theorem 1) it follows that $A \notin \mathscr{U}$. This completes the proof.

### 5. INDUCED FILTER

#### Proposition 8 {#top-i-s6-prop-8 .statement}

*Let* $\mathscr{F}$ *be a filter on a set* $X$ *and* $A$ *a subset of* $X$. *Then the trace* $\mathscr{F}_A$ *of* $\mathscr{F}$ *on* $A$ *is a filter if and only if each set of* $\mathscr{F}$ *meets* $A$.

Since $(M \cap N) \cap A = (M \cap A) \cap (N \cap A)$ we see that $\mathfrak{F}_A$ satisfies $(\mathrm{F}_{\mathrm{II}})$; again, if $M \cap A \subset P \subset A$ then $P = (M \cup P) \cap A$, whence $\mathfrak{F}_A$ satisfies $(\mathrm{F}_1)$. Hence $\mathfrak{F}_A$ is a filter if and only if it satisfies $(\mathrm{F}_{\mathrm{III}})$, i.e. if and only if each set of $\mathfrak{F}$ meets $A$.

In particular, if $A \in \mathfrak{F}$ then $\mathfrak{F}_A$ is a filter on $A$, by $(\mathrm{F}_{\mathrm{II}})$ and $(\mathrm{F}_{\mathrm{III}})$.

#### Definition 5 {#top-i-s6-def-5 .statement}

*Let $A$ be a subset of a set $X$ and $\mathfrak{F}$ a filter on $X$. If the trace of $\mathfrak{F}$ on $A$ is a filter on $A$, this filter is said to be induced by $\mathfrak{F}$ on $A$.*

If a filter $\mathfrak{F}$ on $X$ induces a filter on $A \subset X$, then the trace on $A$ of a base of $\mathfrak{F}$ is a base of $\mathfrak{F}_A$, by reason of Proposition 3 of no. 3.

#### Example {#top-i-s6-n5-exa-1 .statement}

Let $X$ be a topological space, $A$ a subset of $X$, $x$ a point of $X$. In order that the trace on $A$ of the *neighbourhood filter* $\mathscr{B}$ of $x$ should be a filter on $A$, it is necessary and sufficient that every neighbourhood of $x$ meets $A$, i.e. that $x$ lies in the *closure* of $A$ (§ 1, no. 6, Definition 10).

This example of an induced filter is of interest for two reasons: first because it plays an important role in the theory of limits (§ 7, no. 5) and secondly because *every filter can be defined in this way*. Indeed, let $\mathfrak{F}$ be a filter on a set $X$ and let $X'$ be the set obtained by *adjoining* a new element $\omega$ to $X$, $X$ being identified with the complement of $\{ \omega \}$ in $X'$ (*Set Theory*, R, § 4, no. 5); let $\mathfrak{F}'$ be the filter on $X'$ consisting of the sets $M \cup \{ \omega \}$ where $M$ runs through $\mathfrak{F}$. For each point $x \neq \omega$ of $X'$, let $\mathscr{B}(x)$ be the set of all subsets of $X'$ which contain $x$, and let $\mathscr{B}(\omega)$ be $\mathfrak{F}'$; then the $\mathscr{B}(x)$ for $x \in X'$ obviously satisfy axioms $(\mathrm{V}_1), (\mathrm{V}_{\mathrm{II}}), (\mathrm{V}_{\mathrm{III}})$ and $(\mathrm{V}_{\mathrm{IV}})$ and therefore define a topology on $X'$ for which they are the neighbourhood filters of points. Finally $\omega$ lies in the *closure* of $X$ in this topology, and $\mathfrak{F}$ is induced by $\mathfrak{F}' = \mathscr{B}(\omega)$ on $X$. The topology thus defined on $X'$ (resp. the set $X'$ with this topology) is called the *topology* (resp. the *topological space*) *associated with* $\mathfrak{F}$.

#### Proposition 9 {#top-i-s6-prop-9 .statement}

*An ultrafilter $U$ on a set $X$ induces a filter on a subset $A$ of $X$ if and only if $A \in U$; and if this condition is satisfied then $U_A$ is an ultra-filter on $A$.*

This is an immediate consequence of Propositions 5 and 6 of no. 4.

### 6. DIRECT IMAGE AND INVERSE IMAGE OF A FILTER BASE

Let $\mathscr{B}$ be a filter base on a set $X$, and let $f$ be a mapping of $X$ into a set $X'$; then $f(\mathscr{B})$ is a *filter base* on $X'$, for the relation $M \neq \emptyset$ implies $f(M) \neq \emptyset$, and we have $f(M \cap N) \subset f(M) \cap f(N)$. If $\mathscr{B}_1$ is a base of a filter which is *finer* than the filter of base $\mathscr{B}$, then $f(\mathscr{B}_1)$ is a base of a filter *finer* than the filter of base $f(\mathscr{B})$ (no. 3, Proposition 4).

#### Proposition 10 {#top-i-s6-prop-10 .statement}

*If $\mathscr{B}$ is an ultrafilter base on a set $X$ and if $f$ is a mapping of $X$ into a set $X'$, than $f(\mathscr{B})$ is an ultrafilter base on $X'$.*

Let $M'$ be a subset of $X'$. If $\overline{f}^{-1}(M')$ contains a set $M$ of $\mathscr{B}$, then $M'$ contains $f(M)$; if not, then $\mathscr{C}_{\overline{f}}^{-1}(M') = \overline{f}^{-1}\mathscr{C}(M')$ contains a set $N$ of $\mathscr{B}$ (no. 4, Proposition 5) and therefore $\mathscr{C}M'$ contains $f(N)$. Hence the result follows from Proposition 6 of no. 4.

Consider in particular the case where $f$ is the canonical injection $A \to X$ of a subset $A$ of a set $X$. If $\mathscr{B}$ is a filter base on $A$ then $f(\mathscr{B})$ is a filter base on $X$. The filter $\mathfrak{F}$ on $X$ generated by $f(\mathscr{B})$ is called the *filter generated by $\mathscr{B}$ when $\mathscr{B}$ is considered as a filter base on $X$*. If $\mathscr{B}$ is an *ultrafilter base* on $A$ it is also an *ultrafilter base* on $X$ by reason of Proposition 10.

Let us next examine whether the *inverse image* of a filter base is a filter base. Let $\mathscr{B}'$ be a filter base on a set $X'$, and let $f$ be a mapping of a set $X$ into $X'$; then $\overline{f}^{-1}(\mathscr{B}')$ is a filter base on $X$ *if and only if* $\overline{f}^{-1}(M') \neq \varnothing$ *for each* $M' \in \mathscr{B}'$. This is an immediate consequence of the relation $\overline{f}^{-1}(M' \cap N') = \overline{f}^{-1}(M') \cap \overline{f}^{-1}(N')$ and of Definition 3 of no. 3. This condition can also be expressed by saying that *every set of $\mathscr{B}'$ meets $f(X)$* [or that the trace of $\mathscr{B}'$ on $f(X)$ is a filter base]. If this condition is satisfied, then $f(\overline{f}^{-1}(\mathscr{B}'))$ is a base of a filter *finer* than the filter of base $\mathscr{B}$.

If $\mathscr{B}$ is a filter base on $X$ it is clear that the above condition is satisfied by $\mathscr{B}' = f(\mathscr{B}); \; \overline{f}^{-1}(f(\mathscr{B}))$ is then a base of a filter *coarser* than the filter of base $\mathscr{B}$.

Let $A$ be a subset of a set $X$, $\varphi$ the canonical injection $A \to X$; if $\mathscr{B}$ is a filter base on $X$ then $\overline{\varphi}^{-1}(\mathscr{B})$ is the same as $\mathscr{B}_A$. If we express this as a filter base of $A$ by means of the above condition, we recover part of Proposition 8 of no. 5.

### 7. PRODUCT OF FILTERS

Let $(X_i)_{i \in I}$ be a family of sets, and for each $i \in I$ let $\mathscr{B}_i$ be a *filter base* on $X_i$. Let $\mathscr{B}$ be the set of subsets of the product set $X = \prod_{i \in I} X_i$ which are of the form $\prod_{i \in I} M_i$, where $M_i = X_i$ except for a *finite* number of indices and where $M_i \in \mathscr{B}_i$ for each $i$ such that $M_i \neq X_i$. The formula $\left( \prod_{i \in I} M_i \right) \cap \left( \prod_{i \in I} N_i \right) = \prod_{i \in I} (M_i \cap N_i)$ shows that $\mathscr{B}$ is a *filter base* on $X$. Note that the filter of base $\mathscr{B}$ is also generated by the

sets $\overline{\mathrm{pr}}_x^{-1}(M_x)$, where $M_x \in \mathscr{B}_x$ and $x$ runs through $I$, since
$$
\overline{\mathrm{pr}}_x^{-1}(M_x) = M_x \times \prod_{i \neq x} X_i.
$$

#### Definition 6 {#top-i-s6-def-6 .statement}

*Given a filter $\mathfrak{F}_i$ on each set $X_i$ of a family of sets $(X_i)_{i \in I}$, the product of the filters $\mathfrak{F}_i$ is the filter on $X = \prod_{i \in I} X_i$ which has as a base the set of subsets of $X$ of the form $\prod_{i \in I} M_i$, where $M_i \in \mathfrak{F}_i$ for each $i \in I$ and $M_i = X_i$ for all but a finite number of indices. The product filter is denoted by $\prod_{i \in I} \mathfrak{F}_i$.*

The reader may easily verify that the product of the filters $\mathfrak{F}_i$ can also be defined as the *coarsest* filter $\mathfrak{G}$ on $X$ such that $\mathrm{pr}_i(\mathfrak{G}) = \mathfrak{F}_i$ for each $i \in I$.

The preceding remarks show that if $\mathscr{B}_i$ is a base of $\mathfrak{F}_i$ for each $i \in I$, then $\mathscr{B}$ is a *base* of the product filter $\prod_{i \in I} \mathfrak{F}_i$ (no. 3, Proposition 3).

On a product $X = \prod_{i \in I} X_i$ of topological spaces, the neighbourhood filter of any point $x = (x_i)$ is the *product* of the neighbourhood filters of the $x_i$ (§ 4, no. 1).

The construction of a product filter $\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i$ is simpler when the index set $I$ is *finite*: a base of $\mathfrak{F}$ is then formed by *all* products $\prod_{i \in I} M_i$, where $M_i \in \mathfrak{F}_i$ for each $i \in I$. If $I = \{ 1, 2, \ldots, n \}$ we write
$$
\mathfrak{F}_1 \times \mathfrak{F}_2 \times \cdots \times \mathfrak{F}_n
$$
instead of $\prod_{i \in I} \mathfrak{F}_i$.

### 8. ELEMENTARY FILTERS

#### Definition 7 {#top-i-s6-def-7 .statement}

*Let $(x_n)_{n \in \mathbf{N}}$ be an infinite sequence of elements of a set $X$. The elementary filter associated with the sequence $(x_n)$ is the filter generated by the image of the Fréchet filter (no. 1) by the mapping $n \to x_n$ of $\mathbf{N}$ into $X$.*

It comes to the same thing to say that the elementary filter associated with $(x_n)$ is the set of subsets $M$ of $X$ such that $x_n \in M$ except for a *finite* number of values of $n$. If $S_n$ denotes the set of all $x_p$ such that $p \geq n$, then the sets $S_n$ form a *base* of the elementary filter associated with the sequence $(x_n)$.

The elementary filter associated with an infinite *subsequence* of a sequence $(x_n)$ is *finer* than the elementary filter associated with $(x_n)$ (cf. Exercise 15).

By definition, every elementary filter has a countable base. Conversely:

#### Proposition 11 {#top-i-s6-prop-11 .statement}

*If a filter $\mathfrak{F}$ has a countable base, it is the intersection of the elementary filters which are finer than $\mathfrak{F}$.*

Let us arrange the countable base of $\mathfrak{F}$ as a sequence $(A_n)_{n \in \mathbf{N}}$; if we put

$$
B_n = \bigcap_{p=0}^n A_p,
$$

then the $B_n$ again form a base of $\mathfrak{F}$ (no. 3, Proposition 3) and we have $B_{n+1} \subset B_n$ for each $n$. Let $a_n$ be any element of $B_n$ for each $n \in \mathbf{N}$; then it is clear that $\mathfrak{F}$ is coarser than the elementary filter associated with $(a_n)$. Hence the intersection $\mathfrak{J}$ of the elementary filters which are finer than $\mathfrak{F}$ exists and is finer than $\mathfrak{F}$; if $\mathfrak{J}$ is *strictly finer* than $\mathfrak{F}$ there exists a set $M \in \mathfrak{J}$ such that $B_n \cap \complement M \neq \varnothing$ for each $n$; if $b_n \in B_n \cap \complement M$, the elementary filter associated with the sequence $(b_n)$ is finer than $\mathfrak{F}$ and does not contain $M$. This contradicts the definition of $\mathfrak{J}$.

#### Remark {#top-i-s6-n8-rem-1 .statement}

A filter which is *coarser* than a filter with a countable base need not possess a countable base; for example, if $X$ is an uncountable infinite set, then the filter consisting of the complements of finite subsets of $X$ has no countable base (otherwise the set of finite subsets of $X$ would be countable, contrary to assumption); nevertheless this filter is coarser than every elementary filter associated with an infinite sequence of distinct elements of $X$.

### 9. GERMS WITH RESPECT TO A FILTER

Let $\mathfrak{F}$ be a filter on a set $X$. On the set $\mathfrak{P}(X)$ of all subsets of $X$, the relation

"there exists $V \in \mathfrak{F}$ such that $M \cap V = N \cap V$"

between $M$ and $N$ is an *equivalence relation* $R$, for $R$ is obviously reflexive and symmetric, and if $M, N, P$ are three subsets of $X$ such that $M \cap V = N \cap V$ and $N \cap W = P \cap W$, where $V$ and $W$ belong to $\mathfrak{F}$, it follows that $M \cap (V \cap W) = N \cap (V \cap W) = P \cap (V \cap W)$ and $V \cap W \in \mathfrak{F}$, so that $R$ is transitive. The equivalence class mod $R$ of a subset $M$ of $X$ is called the *germ of $M$ with respect to $\mathfrak{F}$*; the quotient set $\mathfrak{P}(X)/R$ is called the *set of germs of subsets of $X$ (with respect to $\mathfrak{F}$)*. The mappings $(M, N) \to M \cap N$ and $(M, N) \to M \cup N$ of

$$
\mathfrak{P}(X) \times \mathfrak{P}(X)
$$

into $\mathfrak{P}(X)$ are compatible with the equivalence relations $R \times R$ and $R$

(Set Theory, R, , no. 8). For if $M \equiv M' \pmod{R}$ and $N \equiv N' \pmod{R}$ then there exist $V$ and $W$ in $\mathfrak{F}$ such that

$$
M \cap V = M' \cap V \quad \text{and} \quad N \cap W = N' \cap W,
$$
so that
$$
(M \cap N) \cap (V \cap W) = (M' \cap N') \cap (V \cap W)
$$
and
$$
\begin{align*}
(M \cup N) \cap (V \cap W) &= (M \cap (V \cap W)) \cup (N \cap (V \cap W)) \\
&= (M' \cap (V \cap W)) \cup (N' \cap (V \cap W)) \\
&= (M' \cup N') \cap (V \cap W).
\end{align*}
$$

Passing to the quotients, these mappings induce two mappings of $(\mathfrak{P}(X)/R) \times (\mathfrak{P}(X)/R)$ into $\mathfrak{P}(X)/R$, which we denote (by abuse of language) by $(\xi, \eta) \to \xi \cap \eta$ and $(\xi, \eta) \to \xi \cup \eta$ respectively. It is a straightforward exercise to verify that with respect to these laws of composition [defined throughout $\mathfrak{P}(X)/R$] every element is idempotent, and that each law is commutative and associative and distributive with respect to the other. Further, the relations $\xi = \xi \cap \eta$ and $\eta = \xi \cup \eta$ are equivalent; if we denote them (by abuse of language) by $\xi \subset \eta$, it is easily verified that this relation is an ordering on $\mathfrak{P}(X)/R$, with respect to which $\mathfrak{P}(X)/R$ is a lattice which has the germ of $\varnothing$ as least element and the germ of $X$ as greatest element. Note that the relation $\xi \subset \eta$ means that there exist $M \in \xi$, $N \in \eta$ and $V \in \mathfrak{F}$ such that $M \cap V \subset N \cap V$.

Now let $X'$ be another set, and let $\Phi$ be the set of all mappings of a set of $\mathfrak{F}$ into $X'$. The relation on $\Phi$

"there exists $V \in \mathfrak{F}$ such that $f$ and $g$ are defined and agree on $V$"

between $f$ and $g$ is an equivalence relation $S$; it is clear that $S$ is reflexive and symmetric, and if $f, g, h$ are three elements of $\Phi$ such that $f$ and $g$ are defined on $V \in \mathfrak{F}$, and $g$ and $h$ are defined and agree on $W \in \mathfrak{F}$, then $f$ and $h$ are defined and agree on $V \cap W \in \mathfrak{F}$, so that $S$ is transitive. The equivalence class mod $S$ of a mapping $f$ of a set $V \in \mathfrak{F}$ into $X'$ is called the germ of $f$ (with respect to $\mathfrak{F}$), and the quotient set $\tilde{\Phi} = \Phi/S$ is called the set of germs of mappings of $X$ into $X'$ (with respect to $\mathfrak{F}$).

#### Remark 1 {#top-i-s6-n9-rem-1 .statement}

Every mapping $f$ of a subset $M$ of $X$ into $X'$, where $M$ belongs to $\mathfrak{F}$, is equivalent mod $S$ to a mapping $f_1$ of $X$ into $X'$ (which justifies the above terminology): it is sufficient to extend $f$ to $X$, e.g. by giving it a constant value on $X - M$.

#### Remark 2 {#top-i-s6-n9-rem-2 .statement}

The characteristic functions $\varphi_M$ and $\varphi_N$ of two subsets $M$ and $N$ of $X$ have the same germ with respect to $\mathfrak{F}$ if and only if $M$ and $N$ have the same germ with respect to $\mathfrak{F}$.

Let $X''$ be a third set, $\varphi$ a mapping of $X'$ into $X''$, $\Phi'$ the set of all mappings of a set of $\mathfrak{F}$ into $X''$. For each $f \in \Phi$, $\varphi \circ f$ belongs to $\Phi'$; further, it is immediately seen that if $g \in \Phi$ has the same germ as $f$ with respect to $\mathfrak{F}$, then $\varphi \circ f$ and $\varphi \circ g$ have the same germ with respect to $\mathfrak{F}$.

This germ therefore depends only on the germ $\tilde{f}$ of $f$ with respect to $\mathfrak{F}$ and is denoted by $\varphi(\tilde{f})$. We thus define a mapping (denoted by $\varphi$, by abuse of language) of the set $\tilde{\Phi}$ of germs of mappings of $X$ into $X'$, into the set $\tilde{\Phi}'$ of germs of mappings of $X$ into $X''$.

Now let $X'_i$ ($1 \leq i \leq n$) be sets and
$$
Y = \prod_{i=1}^n X'_i
$$
their product; let $\Phi_i$ (resp. $\Phi$) denote the set of all mappings of a set of $\mathfrak{F}$ into $X'_i$ (resp. $Y$). If $f_i \in \Phi_i$ for $1 \leq i \leq n$ and if $M_i \in \mathfrak{F}$ is the domain and $f_i$, then the mapping $t \to (f_1(t), \ldots, f_n(t))$ is defined on
$$
\bigcap_{i=1}^n M_i
$$
and hence belongs to $\Phi$; we denote this mapping (by abuse of language) by $(f_1, \ldots, f_n)$. Furthermore, if $f_i$ and $g_i$ belong to $\Phi_i$ and have the same germ with respect to $\mathfrak{F}$ (for $1 \leq i \leq n$), it is immediately seen that $(f_1, \ldots, f_n)$ and $(g_1, \ldots, g_n)$ have the same germ with respect to $\mathfrak{F}$; this germ therefore depends only on the germs $\tilde{f}_i$ of the $f_i$. If we denote it by $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ then $\Gamma$ is clearly a bijection of the product set
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
onto the set $\tilde{\Phi}$, where $\tilde{\Phi}_i$ (resp. $\tilde{\Phi}$) denotes the set of germs of mappings of $X$ into $X'_i$ (resp. $Y$) with respect to $\mathfrak{F}$; hence, by abuse of language, we shall generally write $(\tilde{f}_1, \ldots, \tilde{f}_n)$ instead of $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ whenever there is no risk of confusion.

From what has been said, every mapping $\psi$ of $Y$ into a set $X''$ defines a mapping $(\tilde{f}_1, \ldots, \tilde{f}_n) \to \psi(\tilde{f}_1, \ldots, \tilde{f}_n)$ of
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
into the set $\tilde{\Phi}'$ of germs of mappings of $X$ into $X''$.

In particular, if $n = 2$ and if $X'_1, X'_2$ and $X''$ are all equal to the same set $X'$ (so that $\psi$ is a law of composition defined throughout $X'$), then $\psi$ induces a law of composition defined throughout the set $\tilde{\Phi}$ of germs of mappings of $X$ into $X'$. It is easily verified that if the law given on $X'$ is associative (resp. commutative) then so is the corresponding law on $\tilde{\Phi}$; if the law $\psi$ on $X'$ has an identity element $e'$, then the germ with respect to $\mathfrak{F}$ of the constant mapping $x \to e'$ is an identity element for the corresponding law on $\tilde{\Phi}$. Finally, if the law on $X'$ has an identity element $e'$, then the germ $\tilde{f}$ of $f \in \Phi$ has an inverse in $\tilde{\Phi}$ if and only if there exists $V \in \mathfrak{F}$, contained in the domain of $f$, such that $f(t)$ is invertible in $X'$ for each $t \in V$; if, for each $t \in V$, $g(t)$ denotes the inverse of $f(t)$ then the germ $\tilde{g}$ of $g$ is the inverse of $\tilde{f}$ in $\tilde{\Phi}$. In particular if $X'$ is a group with respect to the law $\psi$, then $\tilde{\Phi}$ is a group with respect to the corresponding law; likewise, if $X'$ is a ring (resp. an algebra over a ring $A$) then $\tilde{\Phi}$ is a ring (resp. an algebra over $A$) with respect to the corresponding laws of composition.

### 10. GERMS AT A POINT

One of the commonest situations to which the definitions and results of no. 9 apply is that in which $\mathfrak{F}$ is the neighbourhood filter of a point $a$ of a topological space $X$; instead of "germs with respect to $\mathfrak{F}$" we then speak of "germs at the point $a$". Notice that there is only one germ of neighbourhoods of $a$, namely the germ of the whole space $X$. The germs of closed sets are identical with the germs of sets which are locally closed at the point $a$, for if $L$ is locally closed at $a$, then the germs of $L$ and $\overline{\Gamma}$ at $a$ are equal (§ 3, no. 1, Proposition 1). It follows that if $\xi, \eta$ are two germs of locally closed sets at $a$, then so are $\xi \cup \eta$ and $\xi \cap \eta$.

Since $a$ is in each $V \in \mathfrak{F}$, $f(a)$ is defined for each mapping $f$ whose domain belongs to $\mathfrak{F}$; furthermore, if $f$ and $g$ have the same germ at $a$ we must have $f(a) = g(a)$, so that $f(a)$ depends only on the germ $\tilde{f}$ of $f$ at $a$, and is called the value of $\tilde{f}$ at $a$ and is denoted by $\tilde{f}(a)$. It should be emphasized that the relation $\tilde{f}(a) = \tilde{g}(a)$ does not in general imply that $\tilde{f} = \tilde{g}$.

Let $X', X''$ be two topological spaces; $b$ a point of $X''$; $g, g'$ two mappings of $X'$ into $X''$ having the same germ at $b$. If $f, f'$ are two mappings of $X$ into $X'$ which are continuous at $a$ and have the same germ at $a$ and are such that $f(a) = b$, then $g \circ f$ and $g' \circ f'$ have the same germ at the point $a$; for if $V'$ is a neighbourhood of $b$ in $X'$ such that $g(x') = g'(x')$ for all $x' \in V'$, then there is a neighbourhood $V$ of $a$ such that $f(V) \subset V'$, $f'(V) \subset V'$ and $f(x) = f'(x')$ for all $x \in V$, and the assertion follows. The germ of $g \circ f$ at $a$ is then called the composition of the germs $\tilde{g}$ and $\tilde{f}$ of $g$ and $f$ respectively and is denoted by $\tilde{g} \circ \tilde{f}$.

### Exercises {#top-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
