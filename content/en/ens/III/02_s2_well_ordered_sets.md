---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 2
section_title: Well-ordered sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 148-157, 221-229
pdf_pages: 0154-0163, 0227-0235
extraction: ocr
subsections:
    - "no": 1
      title: SEGMENTS OF A WELL-ORDERED SET
      page: 148
      pdf_page: 154
    - "no": 2
      title: THE PRINCIPLE OF TRANSFINITE INDUCTION
      page: 151
      pdf_page: 157
    - "no": 3
      title: ZERMELO'S THEOREM
      page: 152
      pdf_page: 158
    - "no": 4
      title: INDUCTIVE SETS
      page: 154
      pdf_page: 160
    - "no": 5
      title: ISOMORPHISMS OF WELL-ORDERED SETS
      page: 155
      pdf_page: 161
    - "no": 6
      title: LEXICOGRAPHIC PRODUCTS
      page: 157
      pdf_page: 163
statements: 28
exercises: 20
content_sha256: 4ac2fa7577e3b279c1918b0f52c4d00e31f38944f59ee1c696ac83de2fb7f10b
---

## 2. WELL-ORDERED SETS

### 1. SEGMENTS OF A WELL-ORDERED SET

A relation $\mathrm{R}\{x, y\}$ is said to be a *well-ordering relation between $x$ and $y$* if R is an order relation between $x$ and $y$ and if, for each non-empty set E on which $\mathrm{R}\{x, y\}$ induces an order relation (i.e., such that $x \in \mathrm{E}$ implies $\mathrm{R}\{x, x\}$; cf. § 1, no. 1), E, ordered by this relation, has a *least element*.

¶ A set E ordered by an ordering $\Gamma$ is said to be *well-ordered* if the relation $y \in \Gamma\langle x\rangle$ is a well-ordering relation between $x$ and $y$; $\Gamma$ is then said to be a *well-ordering* on E. The following definition is equivalent to this:

#### Definition 1 {#ens-iii-s2-def-1 .statement tag=03JY}

*A set* E *is said to be well-ordered if it is ordered and if each non-empty subset of* E *has a least element.*

A well-ordered set E is totally ordered because every subset $\{x, y\}$ of E has a least element. Every subset A of E which is bounded above in E has a least upper bound in E.

*Examples*

#### Example 1 {#ens-iii-s2-n1-exa-1 .statement tag=03SX}

Let $\mathrm{E} = \{\alpha, \beta\}$ be a set whose elements are distinct. It is easily verified that the subset $\{(\alpha, \alpha), (\beta, \beta), (\alpha, \beta)\}$ of $\mathrm{E} \times \mathrm{E}$ is the graph of a well-ordering on E.

#### Example 2 {#ens-iii-s2-n1-exa-2 .statement tag=03SY}

Every subset (in particular, the empty subset) of a well-ordered set is well-ordered by the induced ordering.

#### Example 3 {#ens-iii-s2-n1-exa-3 .statement tag=03SZ}

The existence of totally ordered sets which are not well-ordered is equivalent to the axiom of infinity (§ 4, no. 4, Corollary 1 to Proposition 3, and Exercise 3).

#### Example 4 {#ens-iii-s2-n1-exa-4 .statement tag=03T0}

If $\Gamma$ is a well-ordering on E, the ordering opposite to $\Gamma$ is a well-ordering on E only if E is finite (§ 4, Exercise 3). \*

#### Example 5 {#ens-iii-s2-n1-exa-5 .statement tag=03T1}

Let E be a well-ordered set. The set $\mathrm{E}_1$ obtained by adjoining to E a greatest element $b$ (§ 1, no. 7) is well-ordered, for if H is any non-empty subset of $\mathrm{E}_1$ other than $\{b\}$, the least element of $\mathrm{H} \cap \mathrm{E}$ is also the least element of H.

#### Remark {#ens-iii-s2-n1-rem-1 .statement tag=03JZ}

\* As a consequence of the axiom of infinity (§ 6, no. 1), there exist well-ordered sets which have no greatest element, for example the set $\mathbf{N}$ of natural integers. \*

#### Definition 2 {#ens-iii-s2-def-2 .statement tag=03QN}

*In an ordered set* E, *a subset of* E *such that the relations* $x \in \mathrm{S}$, $y \in \mathrm{E}$, *and* $y \leqslant x$ *imply* $y \in \mathrm{S}$ *is called a segment of* E.

Clearly, every intersection and union of segments of E is a segment of E. If S is a segment of E, every segment of S is also a segment of E. The set E itself and the empty set are segments of E.

#### Proposition 1 {#ens-iii-s2-prop-1 .statement tag=03QO}

*In a well-ordered set* E, *every segment of* E *other than* E *itself is an interval* $]\leftarrow, a[$, *where* $a \in \mathrm{E}$.

Let S be a segment of E such that $\mathrm{S} \neq \mathrm{E}$. Since $\mathrm{E} - \mathrm{S}$ is not empty, it has a least element $a$. By virtue of Definition 2, the relation $x \geqslant a$ implies $x \notin \mathrm{S}$; otherwise we would have $a \in \mathrm{S}$, which is absurd. Hence $\mathrm{E} - \mathrm{S}$ is the interval $[a, \rightarrow[$, and S is the interval $]\leftarrow, a[$.

¶ For every element $x$ in a totally ordered set E the segment $]\leftarrow, x[$ is called the *segment with endpoint x*, and is denoted by $\mathrm{S}_x$.

Note that if E is well-ordered and not empty, $\mathrm{S}_x$ has a least element $\alpha$ and consequently is also the interval $[\alpha, x[$.

Let E be a totally ordered set. The union A of the $\mathrm{S}_x$, as $x$ runs through E, is E if E has no greatest element; and if E has a greatest element $b$, we have $\mathrm{A} = \mathrm{E} - \{b\}$.

#### Proposition 2 {#ens-iii-s2-prop-2 .statement tag=03QP}

*The set* E\* *of segments of a well-ordered set* E *is well-ordered by inclusion. The mapping* $x \rightarrow \mathrm{S}_x$ *is an isomorphism of the well-ordered set* E *onto the set of segments of* E *other than* E *itself.*

It is clear that if $x \in \mathrm{E}$ and $y \in \mathrm{E}$, the relation $x \leqslant y$ implies $\mathrm{S}_x \subset \mathrm{S}_y$, and that $x < y$ implies $\mathrm{S}_x \neq \mathrm{S}_y$; the mapping $x \rightarrow \mathrm{S}_x$ is therefore an isomorphism of E onto the set S(E) of segments of E distinct from E itself (§ 1, no. 12, Proposition 11), and consequently S(E) is well-ordered. Moreover, E\* is isomorphic to the well-ordered set obtained from S(E) by adjoining a greatest element.

#### Proposition 3 {#ens-iii-s2-prop-3 .statement tag=03QQ}

*Let* $(\mathrm{X}_\iota)_{\iota \in \mathbf{I}}$ *be a family of well-ordered sets such that for each pair of indices* $(\iota, \varkappa)$ *one of the sets* $\mathrm{X}_\iota$, $\mathrm{X}_\varkappa$ *is a segment of the other. Then there exists a unique ordering on the set* $\mathrm{E} = \bigcup_{\iota \in \mathbf{I}} \mathrm{X}_\iota$ *which induces the given ordering on each of the* $\mathrm{X}_\iota$. *Endowed with this ordering,* E *is a well-ordered set. Every* *segment of* $\mathrm{X}_\iota$ *is a segment of* E; *for each* $x \in \mathrm{X}_\iota$, *the segment with endpoint* $x$ *in* $\mathrm{X}_\iota$ *is equal to the segment with endpoint* $x$ *in* E; *and each segment of* E *is either* E *itself or a segment of one of the* $\mathrm{X}_\iota$.

The first assertion is a consequence of the following general lemma :

#### Lemma 1 {#ens-iii-s2-lem-1 .statement tag=03QR}

*Let* $(\mathrm{X}_\alpha)_{\alpha \in \mathrm{A}}$ *be a family of ordered sets, directed with respect to the relation* $\subset$ (in other words, such that for each pair of indices $\alpha$, $\beta$ there exists an index $\gamma$ such that $\mathrm{X}_\alpha \subset \mathrm{X}_\gamma$ and $\mathrm{X}_\beta \subset \mathrm{X}_\gamma$). *Suppose that, for each pair of indices* $(\alpha, \beta)$ *such that* $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$, *the ordering induced on* $\mathrm{X}_\alpha$ *by that of* $\mathrm{X}_\beta$ *is identical with the given ordering on* $\mathrm{X}_\alpha$. *Under these conditions there exists a unique ordering on the set* $\mathrm{E} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{X}_\alpha$ *which induces the given ordering on each* $\mathrm{X}_\alpha$.

Let $\mathrm{G}_\alpha$ be the graph of the given ordering on $\mathrm{X}_\alpha$. If G is the graph of an ordering on E which induces on each $\mathrm{X}_\alpha$ the ordering whose graph is $\mathrm{G}_\alpha$, then we must have $\mathrm{G}_\alpha \subset \mathrm{G}$ for each $\alpha \in \mathrm{A}$; hence G contains $\bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. On the other hand, for each pair $(x, y)$ of elements of E there exists by hypothesis an index $\alpha \in \mathrm{A}$ such that $x \in \mathrm{X}_\alpha$ and $y \in \mathrm{X}_\alpha$; if $(x, y) \in \mathrm{G}$, we have $(x, y) \in \mathrm{G}_\alpha$, so that $\mathrm{G} \subset \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. Hence if the required ordering on E exists, its graph is necessarily $\mathrm{G} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. It remains to be shown that this set satisfies the conditions of the lemma. Since $\mathrm{G}_\beta \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ if $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$, we have $\mathrm{G} \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ for all $\alpha \in \mathrm{A}$; on the other hand, it follows from the hypothesis that any three elements $x$, $y$, $z$ of E belong to the same $\mathrm{X}_\alpha$. Hence $(x, y) \in \mathrm{G}$ is an order relation on E, and the lemma is proved.

¶ We now take up the proof of Proposition 3. Let us begin by showing that each $\mathrm{X}_\iota$ is a segment of E. Indeed, if $x \in \mathrm{X}_\iota$, $y \in \mathrm{E}$, and $y \leqslant x$, there exists an index $\varkappa$ such that $\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ and $y \in \mathrm{X}_\varkappa$; since by hypothesis $\mathrm{X}_\iota$ is a segment of $\mathrm{X}_\varkappa$, we have $y \in \mathrm{X}_\iota$, which proves the assertion. The same reasoning proves that for each $x \in \mathrm{X}_\iota$ the segment with endpoint $x$ in $\mathrm{X}_\iota$ is identical with the interval $]\leftarrow, x[$ in E. Next let us show that E is well-ordered. If H is a non-empty subset of E, there is an index $\iota \in \mathrm{I}$ such that $\mathrm{H} \cap \mathrm{X}_\iota \neq \emptyset$; if $a$ is the least element of $\mathrm{H} \cap \mathrm{X}_\iota$ in $\mathrm{X}_\iota$, then $a$ is also the least element of H in E. That is, if $x \in \mathrm{H}$, there exists an index $\varkappa \in \mathrm{I}$ such that $\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ and $x \in \mathrm{X}_\varkappa$; we cannot have $x < a$, because the interval $]\leftarrow, a[$ is contained in $\mathrm{X}_\iota$, and therefore we have $x \geqslant a$ since $\mathrm{X}_\varkappa$ is totally ordered.

¶ Finally, we must show that a segment of E, other than E itself, is a segment of one of the $\mathrm{X}_\iota$; this is an immediate consequence of the preceding arguments, since such a segment is of the form $]\leftarrow, x[$ (Proposition 1) and since $x$ belongs to some $\mathrm{X}_\iota$.

### 2. THE PRINCIPLE OF TRANSFINITE INDUCTION

#### Lemma 2 {#ens-iii-s2-lem-2 .statement tag=03K0}

Let $E$ be a well-ordered set and let $\mathscr{C}$ be a set of segments of $E$ with the following properties : (1) every union of segments belonging to $\mathscr{C}$ belongs to $\mathscr{C}$; (2) if $S_x\in\mathscr{C}$, then $S_x\cup\{x\}\in\mathscr{C}$. Then every segment of $E$ belongs to $\mathscr{C}$.

Suppose that there are segments of $E$ which do not belong to $\mathscr{C}$, and let $S$ be the smallest of them (no. 1, Proposition 2). If $S$ has no greatest element, then $S$ is the union of the segments of $S$ distinct from $S$ itself, and these segments belong to $\mathscr{C}$ by virtue of the definition of $S$; hence $S\in\mathscr{C}$, which is absurd. If, on the other hand, $S$ has a greatest element $a$, then $S=S_a\cup\{a\}$, and since $S_a$ is a segment of $S$ distinct from $S$, we have $S_a\in\mathscr{C}$; but then also $S\in\mathscr{C}$, which again is absurd.

¶ For greater convenience we shall place ourselves in a theory $\mathscr{T}$ in which $E$ is a set *well-ordered* by a relation written $x\leq y$. We have then the following criteria :

C59. (Principle of transfinite induction). *Let $R\{x\}$ be a relation in $\mathscr{T}$ ($x$ not being a constant of $\mathscr{T}$) such that the relation

$$
(x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\}))\Rightarrow R\{x\}
$$

is a theorem in $\mathscr{T}$. Under these conditions the relation $(x\in E)\Rightarrow R\{x\}$ is a theorem in $\mathscr{T}$.*

Let $\mathscr{C}$ be the set of segments $S$ of $E$ such that $(y\in S)\Rightarrow R\{y\}$. It is clear that every union of segments belonging to $\mathscr{C}$ also belongs to $\mathscr{C}$. On the other hand, if $S_x\in\mathscr{C}$, we have $R\{x\}$ by hypothesis; hence $(y\in S_x\cup\{y\})\Rightarrow R\{y\}$ by the method of disjunction of cases. Hence (Lemma 2) $E\in\mathscr{C}$, which proves the criterion.

¶ In the applications of C59, the relation

$$
x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\})
$$

is usually called the “inductive hypothesis”.

¶ In what follows, for every mapping $g$ of a segment $S$ of $E$ into a set $F$, and for each $x\in S$ we shall denote by $g^{(x)}$ the mapping of the segment $S_x=]\leftarrow,x[$ of $E$ onto $g(S_x)$ which coincides with $g$ on $S_x$. With this notation we have

C60. (Definition of a mapping by transfinite induction.) *Let $u$ be a letter, $\mathrm{T}\{u\}$ a term in the theory $\mathscr{T}$. There exists a set $U$ and a mapping $f$ of $E$ onto $U$ such that for all $x\in E$ we have $f(x)=\mathrm{T}\{f^{(x)}\}$. Furthermore, the set $U$ and the mapping $f$ are uniquely determined by these conditions.*

Let us first prove the uniqueness. Suppose that $f'$ and $\mathrm{U}'$ also satisfy the conditions of the criterion. Let $\mathfrak{S}$ be the set of segments S of E such that $f$ and $f'$ coincide on S. It is clear that every union of segments belonging to $\mathfrak{S}$ also belongs to $\mathfrak{S}$. On the other hand, if $\mathrm{S}_x \in \mathfrak{S}$, then $f$ and $f'$ agree on $\mathrm{S}_x$ and therefore $f^{(x)} = {f'}^{(x)}$; consequently

$$f(x) = \mathrm{T}\{f^{(x)}\} = \mathrm{T}\{{f'}^{(x)}\} = f'(x),$$

which shows that $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}$. It follows that $\mathrm{E} \in \mathfrak{S}$ (Lemma 2), hence $f' = f$ and $\mathrm{U}' = f'(\mathrm{E}) = f(\mathrm{E}) = \mathrm{U}$.

¶ Now let $\mathfrak{S}_1$ denote the set of segments S of E for which there exists a set $\mathrm{U_S}$ and a mapping $f_\mathrm{S}$ of S *onto* $\mathrm{U_S}$ such that for all $x \in \mathrm{S}$ we have $f_\mathrm{S}(x) = \mathrm{T}\{f^{(x)}\}$. For each $\mathrm{S} \in \mathrm{S}_1$, $f_\mathrm{S}$ and $\mathrm{U_S}$ are uniquely determined, by the first part of the proof; in particular, if $\mathrm{S}'$ and $\mathrm{S}''$ are two segments belonging to $\mathfrak{S}_1$ such that $\mathrm{S}' \subset \mathrm{S}''$, then $f_{\mathrm{S}'}$ is the mapping of $\mathrm{S}'$ onto $f_{\mathrm{S}''}(\mathrm{S}')$ which agrees with $f_{\mathrm{S}''}$ on $\mathrm{S}'$. From this remark it follows that every union of segments belonging to $\mathfrak{S}_1$ also belongs to $\mathfrak{S}_1$ (Chapter II, § 4, no. 6, Proposition 7). On the other hand, if $\mathrm{S}_x \in \mathfrak{S}_1$, we define on $\mathrm{S} = \mathrm{S}_x \cup \{x\}$ a function $f_\mathrm{S}$ extending $f_{\mathrm{S}_x}$ by putting

$$f_\mathrm{S}(x) = \mathrm{T}\{f_{\mathrm{S}_x}\}$$

(Chapter II, § 4, no. 7, Proposition 8); since $f_\mathrm{S}^{(x)} = f_{\mathrm{S}_x}$, it is obvious that $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_1$. Hence (Lemma 2) $\mathrm{E} \in \mathfrak{S}_1$, and the proof is complete.

¶ Usually this criterion is applied in situations where there exists a set F such that *for every mapping h of a segment of* E *onto a subset of* F *we have* $\mathrm{T}\{h\} \in \mathrm{F}$. Then the set U obtained by applying C60 is a *subset of* F. For, with the notation used above, let $\mathfrak{S}_2$ be the subset of $\mathfrak{S}_1$ consisting of segments S of E such that $\mathrm{U_S} \subset \mathrm{F}$. It is evident that every union of segments belonging to $\mathfrak{S}_2$ also belongs to $\mathfrak{S}_2$; on the other hand, the hypothesis on F implies that if $\mathrm{S}_x \in \mathfrak{S}_2$, we have $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_2$. The assertion now follows from Lemma 2.

### 3. ZERMELO'S THEOREM

#### Lemma 3 {#ens-iii-s2-lem-3 .statement tag=03K1}

*Let* E *be a set, let* $\mathfrak{S}$ *be a subset of* $\mathfrak{P}(\mathrm{E})$, *and let* $p$ *be a mapping of* $\mathfrak{S}$ *into* E *such that* $p(\mathrm{X}) \notin \mathrm{X}$ *for all* $\mathrm{X} \in \mathfrak{S}$. *Then there exists a subset* M *of* E *and a well-ordering* $\Gamma$ *on* M *such that, if* $x \leqslant y$ *denotes the relation* $y \in \Gamma\langle x \rangle$ *and* $\mathrm{S}_x$ *denotes the segment* $]\leftarrow, x]$,

(1) *for all* $x \in \mathrm{M}$ *we have* $\mathrm{S}_x \in \mathfrak{S}$ *and* $p(\mathrm{S}_x) = x$;

(2) $\mathrm{M} \notin \mathfrak{S}$.

Let $\mathfrak{M}$ be the set of subsets G of $\mathrm{E} \times \mathrm{E}$ satisfying the following conditions :

(a) G is the graph of a well-ordering on $\mathrm{pr}_1 \mathrm{G} = \mathrm{U}$;

(b) if $x \leqslant y$ denotes the relation $(x, y) \in \mathrm{G}$ on U, then for each $x \in \mathrm{U}$ the segment $\mathrm{S}_x$ is such that $\mathrm{S}_x \in \mathfrak{S}$ and $p(\mathrm{S}_x) = x$.

¶ We shall show that if G and G' are two elements of M and if U, U' denote their first projections, then one of the two sets U, U' is contained in the other and that if, for example, $\mathrm{U} \subset \mathrm{U}'$, then $\mathrm{G} = \mathrm{G}' \cap (\mathrm{U} \times \mathrm{U})$ (in other words, that the order relation on U is induced by the order relation on U') and U is a *segment* of U'.

¶ Consider the set V of elements $x \in \mathrm{U} \cap \mathrm{U}'$ such that the segments with endpoint $x$ are the same in U and U', and such that the orderings induced on this segment by the orderings on U and U' are identical. It is clear that V is a *segment* in both U and U' and that the orderings induced on V are the same; our assertion will therefore be proved if we show that either $\mathrm{V} = \mathrm{U}$ or $\mathrm{V} = \mathrm{U}'$. Let us argue by contradiction and suppose that $\mathrm{V} \neq \mathrm{U}$ and $\mathrm{V} \neq \mathrm{U}'$. Let $x$ be the least element of $\mathrm{U} - \mathrm{V}$ in U and let $x'$ be the least element of $\mathrm{U}' - \mathrm{V}$ in U'; we have $\mathrm{V} = \mathrm{S}_x$ in U, and $\mathrm{V} = \mathrm{S}_{x'}$ in U'. But by hypothesis, $\mathrm{V} \in \mathfrak{S}$ and

$$x = p(\mathrm{S}_x), \qquad x' = p(\mathrm{S}_{x'}),$$

so that $x = x'$. Hence by definition $x \in \mathrm{V}$, which is absurd.

¶ We may therefore apply Proposition 3 of no. 1 to the set of first projections $\mathrm{U} = \mathrm{pr}_1 \mathrm{G}$ (where $\mathrm{G} \in \mathfrak{M}$) and thus obtain a well-ordered set

$$\mathrm{M} = \bigcup_{\mathrm{G} \in \mathfrak{M}} \mathrm{pr}_1 \mathrm{G}.$$

It is easily seen that the graph of the ordering on M belongs to $\mathfrak{M}$. If we had $\mathrm{M} \in \mathrm{S}$, then, putting $a = p(\mathrm{M})$, we should have $a \notin \mathrm{M}$. We could therefore adjoin to M the element $a$ as greatest element, and the set $\mathrm{M}' = \mathrm{M} \cup \{a\}$ would be well-ordered. Since $\mathrm{M} = \mathrm{S}_a$ in M', we should have $\mathrm{S}_a \in \mathfrak{S}$ and $p(\mathrm{S}_a) = a$; the graph of the ordering on M' would therefore belong to $\mathfrak{M}$, which is absurd.

Note that if $\emptyset \notin \mathfrak{S}$ (and in particular if $\mathfrak{S}$ is empty), the set M whose existence is asserted by Lemma 3 is the empty set; this follows from condition 1 of Lemma 3.

#### Theorem 1 (Zermelo) {#ens-iii-s2-thm-1 .statement tag=03QS}

*Every set* E *can be well-ordered.*

Let $\mathfrak{S} = \mathfrak{P}(\mathrm{E}) - \{\mathrm{E}\}$ be the set of all subsets of E other than E itself. For each $\mathrm{X} \in \mathfrak{S}$ let $p(\mathrm{X}) = \tau_x \ (x \in \mathrm{E} - \mathrm{X})$; since the relation $\mathrm{X} \in \mathfrak{S}$ implies $(\exists x)(x \in \mathrm{E} - \mathrm{X})$, we have $p(\mathrm{X}) \in \mathrm{E} - \mathrm{X}$ (Chapter I, § 4, no. 1) and therefore $p(\mathrm{X}) \notin \mathrm{X}$. We may therefore apply Lemma 3, and consequently there exists a well-ordering on a subset M of E such that $\mathrm{M} \notin \mathfrak{S}$; but the only subset of E which does not belong to $\mathfrak{S}$ is E itself, and the theorem is proved.

### 4. INDUCTIVE SETS

#### Definition 3 {#ens-iii-s2-def-3 .statement tag=03K2}

*An ordered set* E *is said to be inductive if every totally ordered subset of* E *has an upper bound in* E.

*Examples*

#### Example 1 {#ens-iii-s2-n4-exa-1 .statement tag=03T2}

Let $\mathfrak{F}$ be a set of subsets of a set A, ordered by inclusion, and such that for every totally ordered subset $\mathfrak{G}$ of $\mathfrak{F}$ the union of the sets of $\mathfrak{G}$ belongs to $\mathfrak{F}$. Then $\mathfrak{F}$ is inductive with respect to the relation $\subset$ because the union of the sets of $\mathfrak{G}$ is the least upper bound of $\mathfrak{G}$ in $\mathfrak{P}(\mathrm{A})$.

#### Example 2 {#ens-iii-s2-n4-exa-2 .statement tag=03T3}

An important example of a set of subsets which is inductive with respect to the relation $\subset$ is the set $\mathfrak{F}$ of graphs of mappings of subsets of a set A into a set B. For $\mathfrak{F}$ is a subset of $\mathfrak{P}(\mathrm{A} \times \mathrm{B})$, and to say that a subset $\mathfrak{G}$ of $\mathfrak{F}$ is totally ordered by inclusion means that the elements of $\mathfrak{G}$ are graphs of mappings such that, given any two of these mappings, one is an extension of the other. It follows immediately that the union of the sets of $\mathfrak{G}$ is an element of $\mathfrak{F}$ (Chapter II, § 4, no. 6, Proposition 7). Hence the set $\Phi(\mathrm{A}, \mathrm{B})$ of mappings of subsets of A into B is inductive with respect to the order relation "$v$ extends $u$" between $u$ and $v$.

#### Example 3 {#ens-iii-s2-n4-exa-3 .statement tag=03T4}

It follows from the axiom of infinity (§ 6, no. 1) that the well-ordered set of natural integers is not inductive with respect to the relation $\leqslant$. \*

#### Theorem 2 ("Zorn's lemma") {#ens-iii-s2-thm-2 .statement tag=03QT}

— *Every inductive ordered set has a maximal element.*

This theorem is a particular case of the following result :

#### Proposition 4 {#ens-iii-s2-prop-4 .statement tag=03K3}

*Let* E *be an ordered set in which every well-ordered subset is bounded above; then* E *has a maximal element.*

We shall say that an element $v \in \mathrm{E}$ is a *strict upper bound* of a subset X of E if $v$ is an upper bound of X and $v \notin \mathrm{X}$. Let $\mathfrak{S}$ be the set of subsets of E which have a strict upper bound in E, and for each $\mathrm{S} \in \mathfrak{S}$ put $p(\mathrm{S}) = \tau_v(v$ is a strict upper bound of S$)$; then $p(\mathrm{S})$ is a strict upper bound of S. Applying Lemma 3 of no. 3 to $\mathfrak{S}$ and $p$, we see that there exists a subset M of E and a well-ordering $\Gamma$ on M which satisfies the conditions of Lemma 3; in particular, M has no strict upper bound in E. Furthermore, the ordering $\Gamma$ is identical with that induced on M by the ordering on E. For in M the relation “$y\in\Gamma\langle x\rangle$ and $x\ne y$” is equivalent to $x\in S_y$; and since $p(S_y)=y$ is an upper bound of $S_y$ (with respect to the ordering on E), it implies $x<y$ in E. But this means that the injection of M into E is a strictly increasing mapping (M being endowed with the ordering $\Gamma$); and since M is totally ordered, it follows that the relations $y\in\Gamma\langle x\rangle$ and $x\leq y$ are equivalent in M (§ 1, no. 12, Proposition 11). This being so, there exists by hypothesis an upper bound $m$ of M in E; but since M has no strict upper bound, it follows that $m$ is a maximal element of E.

#### Corollary 1 {#ens-iii-s2-prop-4-cor-1 .statement tag=03K4}

*Let E be an inductive ordered set and let a be an element of E. Then there exists a maximal element m of E such that $m\geq a$.*

For it follows from Definition 3 that the set F of elements $x\geq a$ in E is inductive, and a maximal element of F is also maximal in E.

#### Corollary 2 {#ens-iii-s2-prop-4-cor-2 .statement tag=03K5}

*Let $\mathfrak{F}$ be a set of subsets of a set E such that, for every subset $\mathfrak{G}$ of $\mathfrak{F}$ which is totally ordered by inclusion, the union (resp. intersection) of the sets of $\mathfrak{G}$ belongs to $\mathfrak{F}$; then $\mathfrak{F}$ has a maximal (resp. minimal) element.*

### 5. ISOMORPHISMS OF WELL-ORDERED SETS

#### Theorem 3 {#ens-iii-s2-thm-3 .statement tag=03K6}

*Let E and F be two well-ordered sets. Then at least one of the following two statements is true :*

(1) *there exists a unique isomorphism of E onto a segment of F;*

(2) *there exists a unique isomorphism of F onto a segment of E.*

Let $\mathfrak{F}$ be the set of mappings of subsets of E into F such that each mapping is defined on a segment of E and is an isomorphism of this segment onto a segment of F. Then the set $\mathfrak{F}$, ordered by the relation “$v$ extends $u$” between $u$ and $v$, is inductive. For if $\mathfrak{G}$ is a totally ordered subset of $\mathfrak{F}$, the union S of the domains of the mappings $u\in\mathfrak{G}$ is a union of segments of E and is therefore itself a segment of E. If $v$ is the least upper bound of $\mathfrak{G}$ in $\Phi(E,F)$ (no. 4, Example 2), then $v(S)$ is the union of the ranges of the mappings $u\in\mathfrak{G}$ and is therefore a segment of F. Finally, for each pair of elements $x$, $y$ of S such that $x<y$ there exists $u\in\mathfrak{G}$ whose domain contains both $x$ and $y$ (because $\mathfrak{G}$ is totally ordered); and since $v(x)=u(x)<u(y)=v(y)$, $v$ is an isomorphism of S onto $v(S)$, and our assertion is proved.

¶ Now let $u_0$ be a maximal element of $\mathfrak{F}$ (no. 4, Theorem 2) and let $S_0$ be the segment of E which is the domain of $u_0$. If we show that either $S_0=E$ or $u_0(S_0)=F$, the theorem will be proved. Let us argue by contradiction and suppose that $S_0\ne E$ and $u_0(S_0)\ne F$. There will then be an element $a\in E$ and an element $b\in F$ such that $S_0=]-\leftarrow,a[$ and $u_0(S_0)]=]-\leftarrow,b[$ (no. 1, Proposition 1). Extend $u_0$ to a mapping $u_1$ of the segment $]-\leftarrow,a]$ into F by putting $u_1(a)=b$; since $u_1$ is an isomorphism of $]-\leftarrow,a]$ onto the segment $]-\leftarrow,b]$, this contradicts the maximality of $u_0$ in $\mathfrak{F}$.

¶ The uniqueness asserted in Theorem 3 is a consequence of the following Lemma :

#### Lemma 4 {#ens-iii-s2-lem-4 .statement tag=03K7}

*Let E, F be two well-ordered sets and let f, g be two increasing mappings of E into F such that $f(E)$ is a segment of F and g is strictly increasing; then $f(x)\leq g(x)$ for all $x\in E$.*

Suppose, on the contrary, that the set of elements $y\in E$ such that $f(y)>g(y)$ is not empty; then this set will have a least element $a$. If $x<a$, we have then $f(x)\leq g(x)<g(a)<f(a)$ since $g$ is strictly increasing. Since $f(E)$ is a segment of F, there exists $z\in E$ such that $g(a)=f(z)$; $f$ is increasing, so that $f(z)<f(a)$ implies $z<a$. Hence

$$f(z)\leq g(z)<g(a)=f(z),$$

which is absurd.

#### Corollary 1 {#ens-iii-s2-lem-4-cor-1 .statement tag=03K8}

*The only isomorphism of a well-ordered set E onto a segment of E is the identity mapping of E onto itself.*

Put $F=E$ in Theorem 3.

#### Corollary 2 {#ens-iii-s2-lem-4-cor-2 .statement tag=03K9}

*Let E, F be two well-ordered sets. If there exists an isomorphism $f$ of E onto a segment T of F and an isomorphism $g$ of F onto a segment S of E, then we must have $S=E$, $T=F$, and $g,f$ are inverses of each other.*

For $g\circ f$ is an isomorphism of E onto the segment $g(T)\subset S$ of E; by Corollary 1 we have $g(T)=S=E$, and $g\circ f$ is the identity mapping of E. Similarly, $f\circ g$ is the identity mapping of F, whence the result.

#### Corollary 3 {#ens-iii-s2-lem-4-cor-3 .statement tag=03KA}

*Every subset A of a well-ordered set E is isomorphic to a segment of E.*

By virtue of Theorem 3 it is enough to prove that there exists no isomorphism $g$ of E onto a segment of A of the form $S_a$. If there were, $g$ would then be a strictly increasing mapping of E into E such that $g(a)\in S_a$, in other words such that $g(a)<a$; but this inequality contradicts Lemma 4 (with $f$ as the identity mapping).

### 6. LEXICOGRAPHIC PRODUCTS

Let $(E_\iota)_{\iota\in I}$ be a family of ordered sets, indexed by a *well-ordered* set I. Consider the product set $E=\displaystyle\prod_{\iota\in I}E_\iota$, and the relation

$$
\text{``}x\in E\text{ and }y\in E,\text{ and for the least index }\iota\in I\text{ such that }\operatorname{pr}_{\iota}x\ne\operatorname{pr}_{\iota}y,\text{ we have }\operatorname{pr}_{\iota}x<\operatorname{pr}_{\iota}y\text{''},
$$

which we shall denote by $R\{x,y\}$. It is evident that $R\{x,x\}$ is equivalent to $x\in E$, that $R\{x,y\}$ implies $R\{x,x\}$ and $R\{y,y\}$, and that $(R\{x,y\}\text{ and }R\{y,x\})$ implies $x=y$. Also it is easily verified that $(R\{x,y\}\text{ and }R\{y,z\})$ implies $R\{x,z\}$ (consider the least index $\iota\in I$ for which at least two of the three elements $\operatorname{pr}_{\iota}x$, $\operatorname{pr}_{\iota}y$, $\operatorname{pr}_{\iota}z$ are unequal); hence $R\{x,y\}$ is an *order relation on the product set E*. This relation and the ordering it defines are called the *lexicographic order relation* and the *lexicographic ordering* on $E$ (induced by the given orderings on $I$ and on the $E_\iota$); the set E with this ordering is called the *lexicographic product* of the family of ordered sets $(E_\iota)_{\iota\in I}$. If each $E_\iota$ is *totally ordered* the lexicographic product is also *totally ordered*.

### Exercises {#ens-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
