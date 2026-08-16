---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 3
section_title: Correspondences
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 75-90, 124-125
pdf_pages: 0082-0097, 0131-0132
extraction: ocr
subsections:
    - "no": 1
      title: GRAPHS AND CORRESPONDENCES
      page: 75
      pdf_page: 82
    - "no": 2
      title: INVERSE OF A CORRESPONDENCE
      page: 78
      pdf_page: 85
    - "no": 3
      title: COMPOSITION OF TWO CORRESPONDENCES
      page: 78
      pdf_page: 85
    - "no": 4
      title: FUNCTIONS
      page: 81
      pdf_page: 88
    - "no": 5
      title: RESTRICTIONS AND EXTENSIONS OF FUNCTIONS
      page: 82
      pdf_page: 89
    - "no": 6
      title: DEFINITION OF A FUNCTION BY MEANS OF A TERM
      page: 83
      pdf_page: 90
    - "no": 7
      title: COMPOSITION OF TWO FUNCTIONS. INVERSE FUNCTION
      page: 84
      pdf_page: 91
    - "no": 8
      title: RETRACTIONS AND SECTIONS
      page: 86
      pdf_page: 93
    - "no": 9
      title: FUNCTIONS OF TWO ARGUMENTS
      page: 89
      pdf_page: 96
statements: 37
exercises: 11
content_sha256: 8a4115cf22d57ea009a5fd57d02c81b51fc1ae5d0adb1e6d32b5c21f6d93004f
---

## 3. CORRESPONDENCES

### 1. GRAPHS AND CORRESPONDENCES

#### Definition 1 {#ens-ii-s3-def-1 .statement tag=03PG}

G *is said to be a graph if every element of* G *is an ordered pair, i.e., if the relation*

$$(\forall z)(z \in G \Rightarrow (z \text{ is an ordered pair}))$$

*is true.*

If G is a graph, the relation $(x, y) \in G$ is expressed by saying that "$y$ corresponds to $x$ under G".

Let $\boldsymbol{R}\{x, y\}$ be a relation, where $x$ and $y$ are distinct letters. Let $\boldsymbol{G}$ be a letter, distinct from $x$ and $y$, which does not appear in $\boldsymbol{R}$. If the relation

$$(\exists \boldsymbol{G})(\boldsymbol{G} \text{ is a graph and } (\forall x)(\forall y)(\boldsymbol{R} \Leftrightarrow ((x, y) \in \boldsymbol{G})))$$

is true, the relation $\boldsymbol{R}$ is said to *have a graph* (with respect to the letters $x$ and $y$). The graph $\boldsymbol{G}$ is then unique by virtue of the axiom of extent, and is called the *graph* of $\boldsymbol{R}$ with respect to $x$ and $y$.

¶ Let $Z$ be a letter, distinct from $x$ and $y$, which does not appear in $R$. If the relation

$$(\exists Z)(\forall x)(\forall y)(R \Rightarrow ((x, y) \in Z))$$

is true, then $R$ has a graph; we may take this graph to be the set of ordered pairs $z$ such that $z \in Z$ and $R \{ \mathrm{pr}_1 z,\ \mathrm{pr}_2 z \}$ ($z$ being a letter distinct from $x$, $y$, $Z$ which does not appear in $R$). This condition is satisfied if we know a term $T$, which does not contain either $x$ or $y$, such that $R \Rightarrow ((x,\ y) \in T)$ is true.

#### Proposition 1 {#ens-ii-s3-prop-1 .statement tag=03HI}

*Let* G *be a graph. There exists exactly one set* A *and exactly one set* B *with the following properties* :

(1) *the relation* $(\exists y)((x,\ y) \in \mathrm{G})$ *is equivalent to* $x \in \mathrm{A}$;

(2) *the relation* $(\exists x)((x,\ y) \in \mathrm{G})$ *is equivalent to* $y \in \mathrm{B}$.

For it is sufficient to take A (resp. B) to be the set of all objects of the form $\mathrm{pr}_1 z$ (resp. $\mathrm{pr}_2 z$), where $z \in \mathrm{G}$ (§ 1, no. 6). Precisely,

$$\mathrm{A} = \mathscr{E}_x((\exists y)((x, y) \in \mathrm{G}))) \qquad \text{and} \qquad \mathrm{B} = \mathscr{E}_y((\exists x)((x,\ y) \in \mathrm{G}));$$

these sets are called respectively *the first and second projections* of the graph G, or the *domain* and *range* of G; they are denoted by $\mathrm{pr}_1 \langle \mathrm{G} \rangle$ and $\mathrm{pr}_2 \langle \mathrm{G} \rangle$ (or by $\mathrm{pr}_1 \mathrm{G}$ and $\mathrm{pr}_2 \mathrm{G}$ if there is no risk of confusion). It is immediately verified that $\mathrm{G} \subset (\mathrm{pr}_1 \mathrm{G}) \times (\mathrm{pr}_2 \mathrm{G})$; every set of ordered pairs is therefore a subset of a product, and conversely. If one of the two sets $\mathrm{pr}_1 \mathrm{G}$, $\mathrm{pr}_2 \mathrm{G}$ is empty, we have $\mathrm{G} = \emptyset$ (§ 2, Proposition 2).

#### Remark {#ens-ii-s3-n1-rem-3 .statement tag=03S1}

The relation $x = y$ has no graph, for the first projection of the graph, if it existed, would be the set of all objects (cf. § 1, no. 7, Remark).

#### Definition 2 {#ens-ii-s3-def-2 .statement tag=03HJ}

*A correspondence between a set* A *and a set* B *is a triple*

$$\Gamma = (\mathrm{G},\ \mathrm{A},\ \mathrm{B}),$$

*where* G *is a graph such that* $\mathrm{pr}_1 \mathrm{G} \subset \mathrm{A}$ *and* $\mathrm{pr}_2 \mathrm{G} \subset \mathrm{B}$. G *is said to be the graph of* $\Gamma$, A *is the source, and* B *the target of* $\Gamma$.

If $(x,\ y) \in \mathrm{G}$, we say that "$y$ corresponds to $x$ in the correspondence $\Gamma$". For each $x \in \mathrm{pr}_1 \mathrm{G}$ the correspondence $\Gamma$ is said to be *defined at* $x$, and $\mathrm{pr}_1 \mathrm{G}$ is called the *domain of* $\Gamma$; each $y \in \mathrm{pr}_2 \mathrm{G}$ is said to be a *value taken by* $\Gamma$, and $\mathrm{pr}_2 \mathrm{G}$ is called the *range of* $\Gamma$.

If $R \{ x, y \}$ is a relation which has a graph $G$ (with respect to the letters $x$, $y$), and if $A$, $B$ are two sets such that $\mathrm{pr}_1 G \subset A$ and $\mathrm{pr}_2 G \subset B$, we

say that $R$ is a *relation between an element of $A$ and an element of $B$* (with respect to the letters $x$, $y$). The correspondence $\Gamma = (G, A, B)$ is said to be the correspondence between $A$ and $B$ *defined by the* relation $R$ (with respect to $x$ and $y$).

Let G be a graph and let X be a set. The relation

$$x \in X \text{ and } (x, y) \in G$$

implies $(x, y) \in G$ and therefore has a graph $G'$. The second projection of $G'$ consists of all the objects which correspond under G to objects of X.

#### Definition 3 {#ens-ii-s3-def-3 .statement tag=03PI}

*Let* G *be a graph and* X *a set. The set of all objects which correspond under* G *to elements of* X *is called the image of* X *under* G *and is denoted by* $G\langle X \rangle$ *or* $G(X)$.

¶ *Let* $\Gamma = (G, A, B)$ *be a correspondence and let* X *be a subset of* A. *The set* $G\langle X \rangle$ *is also denoted by* $\Gamma\langle X \rangle$ *or* $\Gamma(X)$ *and is called the image of* X *under* $\Gamma$.

*Remarks*

#### Remark 1 {#ens-ii-s3-n1-rem-1 .statement tag=03PH}

Precisely, $G\langle X \rangle$ denotes the set $\mathscr{E}_y((\exists x)(x \in X \text{ and } (x,y) \in G))$. From now on we shall not usually translate our definitions into formal language.

#### Remark 2 {#ens-ii-s3-n1-rem-2 .statement tag=03S2}

The notations $G(X)$ and $\Gamma(X)$ can occasionally lead to confusion with the notation introduced later (cf. no. 4, Remark following Definition 9).

Let G be a graph. Since the relation $(x, y) \in G$ implies $y \in \mathrm{pr}_2 G$, we have $G\langle X \rangle \subset \mathrm{pr}_2 G$ for every set X. Since $(x, y) \in G$ implies $x \in \mathrm{pr}_1 G$, we have $G\langle \mathrm{pr}_1 G \rangle = \mathrm{pr}_2 G$. We have $G\langle \emptyset \rangle = \emptyset$, since $x \notin \emptyset$ is a theorem. If $X \subset \mathrm{pr}_1 G$ and $X \neq \emptyset$, we have $G\langle X \rangle \neq \emptyset$.

#### Proposition 2 {#ens-ii-s3-prop-2 .statement tag=03PJ}

*Let* G *be a graph and let* X, Y *be two sets; then the relation* $X \subset Y$ *implies* $G\langle X \rangle \subset G\langle Y \rangle$.

This is an immediate consequence of the definitions and of C50 (§ 1, no. 4).

#### Corollary {#ens-ii-s3-n1-cor-1 .statement tag=03PK}

*If* $A \supset \mathrm{pr}_1 G$, *we have* $G\langle A \rangle = \mathrm{pr}_2 G$.

#### Definition 4 {#ens-ii-s3-def-4 .statement tag=03PL}

*Let* G *be a graph and* $x$ *an object. The set* $G\langle \{x\} \rangle$ (which is sometimes denoted by $G(x)$, by abuse of language) *is called the section of* G *at* $x$.

It follows immediately from C43 (Chapter I, § 5, no. 1) that the relation $y \in G\langle \{x\} \rangle$ is equivalent to $(x, y) \in G$. If G and $G'$ are two graphs, the relation $G \subset G'$ is thus equivalent to

$$(\forall x)(G\langle \{x\} \rangle \subset G'\langle \{x\} \rangle).$$

If $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ is a correspondence between A and B, then for every $x \in \mathrm{A}$ the section of G at $x$ is also called the *section of* $\Gamma$ *at* $x$ and is denoted by $\Gamma\langle\{x\}\rangle$ (or $\Gamma(x)$).

### 2. INVERSE OF A CORRESPONDENCE

Let G be a graph and $\mathrm{A} = \mathrm{pr}_1\mathrm{G}$, $\mathrm{B} = \mathrm{pr}_2\mathrm{G}$ its projections. The relation $(y, x) \in \mathrm{G}$ implies $(x, y) \in \mathrm{B} \times \mathrm{A}$; this relation therefore has a graph which consists of all ordered pairs $(x, y)$ such that $(y, x) \in \mathrm{G}$.

#### Definition 5 {#ens-ii-s3-def-5 .statement tag=03PM}

*Let G be a graph. The graph whose elements are the ordered pairs $(x, y)$ such that $(y, x) \in \mathrm{G}$ is called the inverse of G and is denoted by* $\overset{-1}{\mathrm{G}}$.

For every set X, $\overset{-1}{\mathrm{G}}\langle\mathrm{X}\rangle$ is called the *inverse image of* X *under* G.

¶ It is clear that the inverse of $\overset{-1}{\mathrm{G}}$ is G, and that

$$\mathrm{pr}_1\overset{-1}{\mathrm{G}} = \mathrm{pr}_2\mathrm{G}, \qquad \mathrm{pr}_2\overset{-1}{\mathrm{G}} = \mathrm{pr}_1\mathrm{G}.$$

In particular, if X, Y are two sets, we have

$$\overset{-1}{\overbrace{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

A graph G is said to be *symmetric* if $\overset{-1}{\mathrm{G}} = \mathrm{G}$.

¶ Let $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ be a correspondence between A and B. Since $\mathrm{pr}_1\overset{-1}{\mathrm{G}} \subset \mathrm{B}$ and $\mathrm{pr}_2\overset{-1}{\mathrm{G}} \subset \mathrm{A}$, the triple $(\overset{-1}{\mathrm{G}}, \mathrm{B}, \mathrm{A})$ is a *correspondence between* B and A, called the *inverse* of the correspondence $\Gamma$, and denoted by $\overset{-1}{\Gamma}$. For every subset Y of B, the image $\overset{-1}{\Gamma}\langle\mathrm{Y}\rangle$ of Y under $\overset{-1}{\Gamma}$ is also called the *inverse image* of Y under $\Gamma$. Clearly the inverse of $\overset{-1}{\Gamma}$ is $\Gamma$.

### 3. COMPOSITION OF TWO CORRESPONDENCES

Let G, G′ be two graphs. Let A denote the set $\mathrm{pr}_1\mathrm{G}$ and let C denote the set $\mathrm{pr}_2\mathrm{G}'$. The relation $(\exists y)((x, y) \in \mathrm{G}$ and $(y, z) \in \mathrm{G}')$ implies that $(x, z) \in \mathrm{A} \times \mathrm{C}$, and therefore has a graph with respect to $x$ and $z$.

#### Definition 6 {#ens-ii-s3-def-6 .statement tag=03PN}

*Let G, G′ be two graphs. The graph (with respect to $x$ and $z$) of the relation $(\exists y)((x, y) \in \mathrm{G}$ and $(y, z) \in \mathrm{G}')$ is called the composition of G′ and G, and is denoted by* $\mathrm{G}' \circ \mathrm{G}$ (or sometimes by $\mathrm{G}'\mathrm{G}$).

#### Proposition 3 {#ens-ii-s3-prop-3 .statement tag=03HK}

*Let* G, G′ *be two graphs. The inverse of* G′ ∘ G *is then* $\overset{-1}{G} \circ \overset{-1}{G'}$.

For the relation "$(x, y) \in G$ and $(y, z) \in G'$" is equivalent to

$$(z, y) \in \overset{-1}{G'} \text{ and } (y, x) \in \overset{-1}{G}.$$

#### Proposition 4 {#ens-ii-s3-prop-4 .statement tag=03HL}

*Let* $G_1$, $G_2$, $G_3$ *be graphs. Then*

$$(G_3 \circ G_2) \circ G_1 = G_3 \circ (G_2 \circ G_1).$$

The relation $(x, t) \in (G_3 \circ G_2) \circ G_1$ is equivalent to the relation

$$(\exists y)((x, y) \in G_1 \text{ and } \exists z((y, z) \in G_2 \text{ and } (z, t) \in G_3))$$

and therefore (by C33 (Chapter I, § 4, no. 3)) to the relation

(1) $$(\exists y)(\exists z)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

Similarly, the relation $(x, t) \in G_3 \circ (G_2 \circ G_1)$ is equivalent to

(2) $$(\exists z)(\exists y)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

But the relations (1) and (2) are equivalent; hence the result.

¶ The graph $G_3 \circ (G_2 \circ G_1)$ is denoted by $G_3 \circ G_2 \circ G_1$. Similarly, if $G_1$, $G_2$, $G_3$, $G_4$ are graphs, we put

$$G_4 \circ (G_3 \circ G_2 \circ G_1) = G_4 \circ G_3 \circ G_2 \circ G_1;$$

and so on.

#### Proposition 5 {#ens-ii-s3-prop-5 .statement tag=03HM}

*Let* G, G′ *be graphs and let* A *be a set. Then*

$$(G' \circ G)\langle A \rangle = G'\langle G\langle A \rangle\rangle.$$

For by virtue of C33 (Chapter I, § 4, no. 3) the relation $z \in (G' \circ G)\langle A \rangle$ is equivalent to

$$(\exists y)((\exists x)(x \in A \text{ and } (x, y) \in G) \text{ and } (y, z) \in G')$$

and is therefore equivalent to $(\exists y)(y \in G\langle A \rangle$ and $(y, z) \in G')$; hence the result.

¶ If G and G′ are two graphs, we have $\mathrm{pr}_1(G' \circ G) = \overset{-1}{G}\langle \mathrm{pr}_1 G'\rangle$, and $\mathrm{pr}_2(G' \circ G) = G'\langle \mathrm{pr}_2 G\rangle$. For example, to prove the second of these

relations it is enough to note that the relation $z \in \mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G})$ is equivalent to $(\exists x)((x, z) \in \mathrm{G}' \circ \mathrm{G})$ and therefore to

$$(\exists y)((\exists x)((x, y) \in \mathrm{G}) \quad \text{and} \quad (y, z) \in \mathrm{G}');$$

but this is equivalent to $z \in \mathrm{G}'\langle \mathrm{pr}_2\mathrm{G}\rangle$.

¶ If G is a graph and X a set such that $\mathrm{X} \subset \mathrm{pr}_1\mathrm{G}$, we have

$$\mathrm{X} \subset \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle.$$

For the relation $x \in \mathrm{X}$ implies by hypothesis that $(\exists y)((x, y) \in \mathrm{G})$; but $(x, y) \in \mathrm{G}$ is equivalent to $(y, x) \in \overset{-1}{\mathrm{G}}$, and on the other hand $(x, y) \in \mathrm{G}$ implies $(\exists z)(z \in \mathrm{X}$ and $(z, y) \in \mathrm{G})$; hence $x \in \mathrm{X}$ implies

$$(\exists y)((\exists z)(z \in \mathrm{X} \quad \text{and} \quad (z, y) \in \mathrm{G}) \quad \text{and} \quad (y, x) \in \overset{-1}{\mathrm{G}}),$$

that is to say, $x \in \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle$.

¶ It is clear that if $\mathrm{G}_1$, $\mathrm{G}_2$, $\mathrm{G}'_1$, $\mathrm{G}'_2$ are graphs, the relations $\mathrm{G}_1 \subset \mathrm{G}_2$ and $\mathrm{G}'_1 \subset \mathrm{G}'_2$ imply $\mathrm{G}'_1 \circ \mathrm{G}_1 \subset \mathrm{G}'_2 \circ \mathrm{G}_2$.

¶ Let $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ and $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ be two correspondences such that the target of $\Gamma$ is the same as the source of $\Gamma'$. From the above discussion we have $\mathrm{pr}_1(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_1\mathrm{G} \subset \mathrm{A}$ and $\mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_2\mathrm{G}' \subset \mathrm{C}$; hence we may state the following definition :

#### Definition 7 {#ens-ii-s3-def-7 .statement tag=03PO}

*Let* $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ *and* $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ *be two correspondences such that the target of* $\Gamma$ *is the source of* $\Gamma'$. *Then the correspondence* $(\mathrm{G}' \circ \mathrm{G}, \mathrm{A}, \mathrm{C})$ *is called the composition of* $\Gamma'$ *and* $\Gamma$, *and is denoted by* $\Gamma' \circ \Gamma$ (or sometimes $\Gamma'\Gamma$).

It follows immediately from Proposition 5 that if X is a subset of A we have $(\Gamma' \circ \Gamma)\langle \mathrm{X}\rangle = \Gamma'\langle \Gamma\langle \mathrm{X}\rangle\rangle$. Furthermore, since the target of $\overset{-1}{\Gamma'}$ is the same as the source of $\overset{-1}{\Gamma}$, the inverse of $\Gamma' \circ \Gamma$ is $\overset{-1}{\Gamma} \circ \overset{-1}{\Gamma'}$, by Proposition 3.

#### Definition 8 {#ens-ii-s3-def-8 .statement tag=03PP}

*If* A *is a set, the set* $\Delta_\mathrm{A}$ *of all objects of the form* $(x, x)$, *where* $x \in \mathrm{A}$, *is called the diagonal of* $\mathrm{A} \times \mathrm{A}$.

Clearly we have $\mathrm{pr}_1\Delta_\mathrm{A} = \mathrm{pr}_2\Delta_\mathrm{A} = \mathrm{A}$. The correspondence

$$\mathrm{I}_\mathrm{A} = (\Delta_\mathrm{A}, \mathrm{A}, \mathrm{A})$$

is called the *identity correspondence* on A; it is its own inverse.

¶ If $\Gamma$ is a correspondence between A and B and if $\mathrm{I}_\mathrm{A}$, $\mathrm{I}_\mathrm{B}$ are the identity correspondences on A, B, respectively, then $\Gamma \circ \mathrm{I}_\mathrm{A} = \mathrm{I}_\mathrm{B} \circ \Gamma = \Gamma$.

### 4. FUNCTIONS

#### Definition 9 {#ens-ii-s3-def-9 .statement tag=03HN}

*A graph* F *is said to be a functional graph if for each x there is at most one object which corresponds to x under* F (Chapter I, § 5, no. 3). *A correspondence* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *is said to be a function if its graph* F *is a functional graph and if its source* A *is equal to its domain* $\mathrm{pr}_1\mathrm{F}$. *In other words, a correspondence* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *is a function if for every x belonging to the source* A *of f the relation* $(x, y) \in \mathrm{F}$ *is functional in y* (Chapter I, § 5, no. 3); *the unique object which corresponds to x under f is called the value of f at the element x of* A, *and is denoted by* $f(x)$ (*or* $f_x$, *or* $\mathrm{F}(x)$, *or* $\mathrm{F}_x$).

If $f$ is a function, F its graph, and $x$ an element of the domain of $f$, the relation $y = f(x)$ is then equivalent to $(x, y) \in \mathrm{F}$ (Chapter I, § 5, no. 3, criterion C46).

#### Remark {#ens-ii-s3-n4-rem-1 .statement tag=03HO}

The reader should beware of the confusion which may arise from the simultaneous use of the notations $f(x)$ and $f(\mathrm{X})$ (synonymous with $f\langle \mathrm{X} \rangle$) introduced in Definition 3 (cf. Exercise 11).

Let A and B be two sets; a *mapping of* A *into* B is a function $f$ whose source (which is equal to its domain) is equal to A and whose target is equal to B; such a function is also said to be *defined on* A and to *take its values in* B.

Instead of the phrase "let $f$ be a mapping of A into B", the following phrases are often used : "let $f : \mathrm{A} \to \mathrm{B}$ be a mapping" or even "let $f : \mathrm{A} \to \mathrm{B}$". To simplify the presentation of an argument involving several mappings, we use *diagrams* such as

$$\begin{array}{ccccccc} & f & & & g & \mathrm{C} & & i & \\ \mathrm{A} & \to & \mathrm{B} & \nearrow & & & \searrow & & \mathrm{E} \\ & & & \searrow & & \mathrm{D} & \nearrow & & \\ & & & h & & & j & & \end{array}$$

in which a group of signs such as $\mathrm{A} \overset{f}{\to} \mathrm{B}$ is to be interpreted as meaning that $f$ is a mapping of A into B.

A function $f$ defined on A is said to *transform x into* $f(x)$ (for all $x \in \mathrm{A}$); $f(x)$ is called the *transform of x by f* or (by abuse of language) the *image* of $x$ under $f$.

¶ Under certain circumstances, a functional graph is called a *family*; the domain is then called the *index set*, and the range is called (by abuse of language) the *set of elements* of the family. It is mainly in this connection that the indicial notation $f_x$ is used to denote the value of $f$ at the element $x$. When the index set is the product of two sets, we often speak of a *double family*.

¶ Likewise a function whose target is E is sometimes called a *family of elements* of E. If every element of E is a subset of a set F, we speak of a *family of subsets* of F.

Throughout this series we shall often use the word “function” in place of “functional graph”.

*Examples of functions*

#### Example 1 {#ens-ii-s3-n4-exa-1 .statement tag=03V1}

The empty set is a functional graph. Every function whose graph is empty has domain and range equal to the empty set. Among such functions, the one whose target is empty (i.e., the function $(\varnothing,\varnothing,\varnothing)$) is called the *empty function*.

#### Example 2 {#ens-ii-s3-n4-exa-2 .statement tag=03V2}

Let A be a set. The identity correspondence of A (no. 3) is a function, called the *identity mapping* of A.

Thus with every set A there is associated a family, defined by the identity mapping of A, whose index set is A and whose set of elements is A. By abuse of language, a set is sometimes referred to as a “family”, in which case it is the family thus associated with the set in question.

A function $f$ is said to be *constant* if for all $x$ and $x'$ in the domain of $f$ we have $f(x)=f(x')$.

¶ Let $f$ be a mapping of a set E into E. An element $x$ of E is said to be *fixed under* $f$ if $f(x)=x$.

### 5. RESTRICTIONS AND EXTENSIONS OF FUNCTIONS

Two functions $f$ and $g$ are said to *agree* (or *coincide*) on a set E if E is contained in the domains of $f$ and $g$ and if $f(x)=g(x)$ for all $x\in E$. Two functions which have the same graph agree on their domain. To say that $f=g$ is to say that $f$ and $g$ have the same domain A and the same target B, and that they agree on A.

¶ Let $f=(F,A,B)$ and $g=(G,C,D)$ be two functions. To say that $F\subset G$ is to say that the domain A of $f$ is contained in the domain C of $g$ and that $g$ agrees with $f$ on A. If also $B\subset D$, then $g$ is said to be an *extension* of $f$ (more precisely, an extension of $f$ to C), and $g$ is said to *extend* $f$ (to C). When $g$ is called a *family of elements* of D, $f$ is said to be a *subfamily* of $g$.

¶ Let $f$ be a function and let A be a subset of the domain of $f$. It is immediate that the relation “$x\in A$ and $y=f(x)$” has a graph G with respect to $x$ and $y$, that this graph is functional, and that A is its domain; the function whose graph is G, which has the same target as $f$,

is called the *restriction* of $f$ to $A$, and is sometimes denoted by $f|A$. A function is an extension of any of its restrictions. If two functions $f$, $g$ have the same target and agree on a set $E$, then their restrictions to $E$ are equal.

### 6. DEFINITION OF A FUNCTION BY MEANS OF A TERM

C54. *Let $T$, $A$ be two terms and let $x$, $y$ be distinct letters. Suppose that $x$ does not appear in $A$ and that $y$ does not appear in either $T$ or $A$. Let $R$ be the relation “$x \in A$ and $y = T$”. The relation $R$ has a graph $F$ with respect to the letters $x$ and $y$. This graph is functional; its first projection is $A$, and its second projection is the set of objects of the form $T$ for $x \in A$ (§ 1, no. 6). For every $x \in A$ we have $F(x) = T$.*

Let $B$ be the set of objects of the form $T$ for $x \in A$. Then

$$
R \Longrightarrow ((x,y) \in A \times B);
$$

since the assembly denoted by $A \times B$ contains neither $x$ nor $y$, $R$ has a graph $F$ with respect to the letters $x$ and $y$ (no. 1). It is clear that the relation

$$
(x,y) \in F \quad\text{and}\quad (x,y') \in F
$$

implies $y = y'$, and hence $F$ is a functional graph. The remaining statements are evident.

¶ If $C$ is a set which contains the set $B$ of objects of the form $T$ for $x \in A$ (where $y$ does not appear in $C$), then the function $(F,A,C)$ is also denoted by the notation $x \to T$ ($x \in A$, $T \in C$); the corresponding assembly in formal mathematics contains neither $x$ nor $y$ and does not depend on the choice of the letter $y$ satisfying the above conditions. When the context is sufficiently explicit we shall permit ourselves the notations $x \to T(x \in A)$, $(T)_{x \in A}$, or $x \to T$, and sometimes simply $T$ or $(T)$. *Thus we may speak of “the function $x^3$”, if the context indicates clearly that we mean the mapping $x \to x^3$ of the set of complex numbers into itself. *

*Examples*

#### Example 1 {#ens-ii-s3-n6-exa-1 .statement tag=03S3}

If $f$ is a mapping of $A$ into $B$, the function $f$ is equal to the function $x \to f(x)$ ($x \in A$, $f(x) \in B$), which is written simply as $x \to f(x)$ or also $(f_x)_{x \in A}$ (the latter notation is especially associated with the phrase “family of elements” instead of “function”).

#### Example 2 {#ens-ii-s3-n6-exa-2 .statement tag=03S4}

Let G be a set of ordered pairs. The functions

$$z \to \mathrm{pr}_1 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_1 z \in \mathrm{pr}_1 \mathrm{G})$$

and

$$z \to \mathrm{pr}_2 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_2 z \in \mathrm{pr}_2 \mathrm{G})$$

are called respectively the *first and second coordinate functions on* G; they are denoted by $\mathrm{pr}_1$ and $\mathrm{pr}_2$ when there is no risk of confusion.

### 7. COMPOSITION OF TWO FUNCTIONS. INVERSE FUNCTION

#### Proposition 6 {#ens-ii-s3-prop-6 .statement tag=03HP}

*If f is a mapping of* A *into* B, *and g is a mapping of* B *into* C, *then* $g \circ f$ *is a mapping of* A *into* C.

Let F, G be the graphs of $f$, $g$, respectively, and let us show that $\mathrm{G} \circ \mathrm{F}$ is a functional graph. Let $x$, $z$, $z'$ be objects such that $(x, z) \in \mathrm{G} \circ \mathrm{F}$, $(x, z') \in \mathrm{G} \circ \mathrm{F}$. There exist objects $y$, $y'$ such that

$$(x, y) \in \mathrm{F}, \qquad (x, y') \in \mathrm{F}, \qquad (y, z) \in \mathrm{G}, \qquad (y', z') \in \mathrm{G}.$$

Since F is a functional graph, we have $y = y'$ and hence $(y, z') \in \mathrm{G}$. Since G is a functional graph, it follows that $z = z'$, which proves our assertion. Furthermore, the domain of $g \circ f$ is evidently A, and the proof is complete.

¶ The function $g \circ f$ may also be written as $x \to g(f(x))$, or as $gf$ when there is no risk of confusion.

#### Definition 10 {#ens-ii-s3-def-10 .statement tag=03HQ}

*Let f be a mapping of* A *into* B. *The mapping f is said to be injective, or an injection, if any two distinct elements of* A *have distinct images under f. The mapping f is said to be surjective, or a surjection, if* $f(\mathrm{A}) = \mathrm{B}$. *If f is both injective and surjective, it is said to be bijective, or a bijection.*

Instead of saying that $f$ is surjective, we sometimes say that $f$ is a mapping of A *onto* B, or that it is a *parametric representation* of B by means of A (in which case A is called the *set of parameters* of the representation, and the elements of A are called *parameters*). If $f$ is bijective, we sometimes say that *f puts* A *and* B *in one-to-one correspondence*. A bijection of A onto A is called a *permutation* of A.

*Examples*

#### Example 1 {#ens-ii-s3-n7-exa-1 .statement tag=03S5}

If $\mathrm{A} \subset \mathrm{B}$, the mapping of A into B whose graph is the diagonal of A is injective and is called the *canonical mapping* or the *canonical injection* (or simply the *injection*) of A into B.

#### Example 2 {#ens-ii-s3-n7-exa-2 .statement tag=03S6}

Let A be a set. The mapping $x \to (x, x)$ of A into the diagonal $\Delta_\mathbf{A}$ of $\mathrm{A} \times \mathrm{A}$ is a bijective mapping, called the *diagonal mapping* of A.

#### Example 3 {#ens-ii-s3-n7-exa-3 .statement tag=03S7}

Let G be a set of ordered pairs. The mapping $\mathrm{pr}_1$ (resp. $\mathrm{pr}_2$) of G into $\mathrm{pr}_1\mathrm{G}$ (resp. $\mathrm{pr}_2\mathrm{G}$) is surjective; $\mathrm{pr}_1$ is injective if and only if G is a functional graph.

#### Example 4 {#ens-ii-s3-n7-exa-4 .statement tag=03S8}

Let G be a set of ordered pairs. The mapping

$$z \to (\mathrm{pr}_2 z,\ \mathrm{pr}_1 z)$$

of G into $\overset{-1}{\mathrm{G}}$ is a bijection (called the *canonical* bijection).

#### Example 5 {#ens-ii-s3-n7-exa-5 .statement tag=03S9}

Let A be a set and $b$ an object. The mapping $x \to (x,\ b)$ of A into $\mathrm{A} \times \{b\}$ is a bijection.

#### Proposition 7 {#ens-ii-s3-prop-7 .statement tag=03PQ}

*Let $f$ be a mapping of* A *into* B. *Then* $\overset{-1}{f}$ *is a function if and only if $f$ is bijective.*

If $\overset{-1}{f}$ is a function, its source B is equal to its domain, i.e., to $f(\mathrm{A})$; hence $f$ is surjective. To show that $f$ is injective, let $x$ and $y$ be two elements of A such that $f(x) = f(y)$. If F denotes the graph of $f$, we have

$$(f(x),\ x) \in \overset{-1}{\mathrm{F}} \qquad \text{and} \qquad (f(y),\ y) \in \overset{-1}{\mathrm{F}},$$

hence

$$(f(x),\ y) \in \overset{-1}{\mathrm{F}},$$

so that $x = y$, which proves the assertion.

¶ Conversely, if $f$ is bijective, it is immediate that $\overset{-1}{\mathrm{F}}$ is functional and that the domain of $\overset{-1}{f}$ is equal to B.

When $f$ is bijective, $\overset{-1}{f}$ is called the *inverse mapping* of $f$; $\overset{-1}{f}$ is bijective, $\overset{-1}{f} \circ f$ is the identity mapping of A, and $f \circ \overset{-1}{f}$ is the identity mapping of B.

¶ If a permutation is the same as its inverse, it is said to be *involutory*.

#### Remark {#ens-ii-s3-n7-rem-1 .statement tag=03HR}

Let $f$ be a mapping of A into B. For each subset X of A we have (no. 3) $\mathrm{X} \subset \overset{-1}{f}\langle f\langle \mathrm{X}\rangle\rangle$. Furthermore, for each subset Y of B we have $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle \subset \mathrm{Y}$, for the relation $y \in f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle$ is equivalent to

$$(\exists x)((\exists z)(z \in \mathrm{Y} \text{ and } z = f(x)) \text{ and } y = f(x))$$

and therefore implies the relation $(\exists z)(z \in \mathrm{Y} \text{ and } y = z)$ and consequently also the relation $y \in \mathrm{Y}$.

If $f$ is *surjective*, we have $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle = \mathrm{Y}$ for every subset Y of B, for the relation $y \in \mathrm{Y} \subset \mathrm{B}$ implies by hypothesis the relation $(\exists x)(y = f(x))$ and therefore also $(\exists x)(y \in \mathrm{Y} \text{ and } y = f(x))$; but "$y \in \mathrm{Y}$ and $y = f(x)$" implies $(\exists z)(z \in \mathrm{Y} \text{ and } z = f(x))$, and our assertion follows.

If $f$ is *injective*, we have $\overset{-1}{f}\langle f\langle X\rangle\rangle = X$ for every subset X of A. For the relation $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ is equivalent to $f(x) \in f\langle X\rangle$, hence to

$$(\exists z)(z \in X \text{ and } f(z) = f(x));$$

but the hypothesis means that $f(z) = f(x)$ implies $z = x$, hence $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ implies $x \in X$.

### 8. RETRACTIONS AND SECTIONS

#### Proposition 8 {#ens-ii-s3-prop-8 .statement tag=03HS}

*Let $f$ be a mapping of* A *into* B. *If there exists a mapping $r$* (resp. $s$) *of* B *into* A *such that $r \circ f$* (resp. $f \circ s$) *is the identity mapping of* A (resp. B), *then $f$ is injective* (resp. *surjective*). *Conversely, if $f$ is surjective, there exists a mapping $s$ of* B *into* A *such that $f \circ s$ is the identity mapping of* B. *If $f$ is injective and if* A $\neq \emptyset$, *there exists a mapping $r$ of* B *into* A *such that $r \circ f$ is the identity mapping of* A.

If there exists a mapping $r$ of B into A such that $r \circ f$ is the identity mapping of A, then the equality $f(x) = f(y)$, where $x \in A$ and $y \in A$, implies $x = r(f(x)) = r(f(y)) = y$, and so $f$ is injective. If there exists a mapping $s$ of B into A such that $f \circ s$ is the identity mapping of B, we have $B = f(s(B)) \subset f(A) \subset B$, so that $f$ is surjective. If $f$ is surjective, let T denote the term $\tau_y(y \in A \text{ and } f(y) = x)$. We have $f(T) = x$ for $x \in B$; if $s$ denotes the mapping $x \to T$ $(x \in B, T \in A)$, then $f \circ s$ is the identity mapping of B. Finally, suppose that $f$ is injective and that A $\neq \emptyset$, and let $a$ be an element of A. The relation

$$\text{“}(y \in A \text{ and } x = f(y)) \text{ or } (y = a \text{ and } x \in B - f(A))\text{''}$$

implies $(x, y) \in B \times A$ and therefore has a graph R with respect to the letters $x$, $y$. This graph is functional by reason of the hypothesis on $f$, and has B as its domain; and we have $R(x) = a$ if $x \in B - f(A)$, and $f(R(x)) = x$ if $x \in f(A)$. Hence the function $r = (R, B, A)$ is such that $r \circ f$ is the identity mapping of A.

#### Corollary {#ens-ii-s3-n8-cor-1 .statement tag=03HT}

*Let* A, B *be sets, let $f$ be a mapping of* A *into* B, *and let $g$ be a mapping of* B *into* A. *If $g \circ f$ is the identity mapping of* A *and if $f \circ g$ is the identity mapping of* B, *then $f$ and $g$ are bijective, and $g = \overset{-1}{f}$.*

#### Definition 11 {#ens-ii-s3-def-11 .statement tag=03HU}

*Let $f$ be an injective* (resp. *surjective*) *mapping of* A *into* B. *Any mapping $r$* (resp. $s$) *of* B *into* A *such that $r \circ f$* (resp. $f \circ s$) *is the identity mapping of* A (resp. B) *is called a retraction* (resp. *section*) *of $f$.*

Instead of retraction (resp. section) the phrase *left-inverse* (resp. *right-inverse*) is sometimes used.

¶ If $f$ is injective (resp. surjective) and if $r$ (resp. $s$) is a retraction (resp. section) of $f$, then $f$ is a section (resp. retraction) of $r$ (resp. $s$). Hence a retraction is surjective and a section is injective.

¶ If $f$ is surjective and if $s$, $s'$ are two sections of $f$ such that $s(\mathrm{B}) = s'(\mathrm{B})$, then $s = s'$; for if $x \in \mathrm{B}$, there exists $y \in \mathrm{B}$ such that $s(x) = s'(y)$, and we have $x = f(s(x)) = f(s'(y)) = y$, so that $s(x) = s'(x)$ and consequently $s = s'$. Thus a section $s$ is uniquely determined by the set $s(\mathrm{B})$. By abuse of language, the set $s(\mathrm{B})$ is sometimes called a *section of $f$*.

#### Theorem 1 {#ens-ii-s3-thm-1 .statement tag=03PR}

*Let $f$ be a mapping of* A *into* B, *let $f'$ be a mapping of* B *into* C, *and let $f'' = f' \circ f$. Then :*

(a) *If $f$ and $f'$ are injections, then $f''$ is an injection. If $r$, $r'$ are retractions of $f$, $f'$, respectively, then $r \circ r'$ is a retraction of $f''$.*

(b) *If $f$ and $f'$ are surjections, then $f''$ is a surjection. If $s$, $s'$ are sections of $f$, $f'$, respectively, then $s \circ s'$ is a section of $f''$.*

(c) *If $f''$ is an injection, then $f$ is an injection. If $r''$ is a retraction of $f''$, then $r'' \circ f'$ is a retraction of $f$.*

(d) *If $f''$ is a surjection, then $f'$ is a surjection. If $s''$ is a section of $f''$, then $f \circ s''$ is a section of $f'$.*

(e) *If $f''$ is a surjection and $f'$ an injection, then $f$ is a surjection. If $s''$ is a section of $f''$, then $s'' \circ f'$ is a section of $f$.*

(f) *If $f''$ is an injection and $f$ a surjection, then $f'$ is an injection. If $r''$ is a retraction of $f''$, then $f \circ r''$ is a retraction of $f'$.*

For every set E let $\mathrm{I_E}$ denote the identity mapping of E.

(a) We have $r \circ f = \mathrm{I_A}$ and $r' \circ f' = \mathrm{I_B}$, hence

$$(r \circ r') \circ (f' \circ f) = r \circ \mathrm{I_B} \circ f = r \circ f = \mathrm{I_A}.$$

If $f$ and $f'$ are injections, then $f''$ is an injection, by Proposition 8 if $\mathrm{A} \neq \emptyset$, and trivially if $\mathrm{A} = \emptyset$.

(b) We have $f \circ s = \mathrm{I_B}$ and $f' \circ s' = \mathrm{I_C}$, hence

$$(f' \circ f)(s \circ s') = f' \circ \mathrm{I_B} \circ s' = f' \circ s' = \mathrm{I_C}.$$

If $f$ and $f'$ are surjections, $f''$ is then a surjection by Proposition 8.

(c) We have $r'' \circ f'' = \mathrm{I_A}$, hence $(r'' \circ f') \circ f = r'' \circ f'' = \mathrm{I_A}$. If $f''$ is an injection, then $f$ is an injection, by Proposition 8 if $\mathrm{A} \neq \emptyset$, and trivially if $\mathrm{A} = \emptyset$.

(d) We have $f'' \circ s'' = \mathrm{I_C}$, hence $f' \circ (f \circ s'') = f'' \circ s'' = \mathrm{I_C}$. If $f''$ is a surjection, then $f'$ is a surjection by Proposition 8.

(e) We have $f'' \circ s'' = \mathrm{I_C}$, and $f'$ is a bijection by (d). Hence

$$f \circ (s'' \circ f') \;=\; (\overset{-1}{f}{}' \circ f') \circ f \circ (s'' \circ f') \;=\; \overset{-1}{f}{}' \circ (f'' \circ s'') \circ f'$$
$$= \overset{-1}{f}{}' \circ \mathrm{I_C} \circ f' = \overset{-1}{f}{}' \circ f' = \mathrm{I_B}.$$

If $f''$ is a surjection and $f'$ an injection, $f$ is then a surjection by Proposition 8.

(f) We have $r'' \circ f'' = \mathrm{I_A}$, and $f$ is a bijection by (c). Hence

$$(f \circ r'') \circ f' = (f \circ r'') \circ f' \circ (f \circ \overset{-1}{f}) = f \circ (r'' \circ f'') \circ \overset{-1}{f} = f \circ \mathrm{I_A} \circ \overset{-1}{f}$$
$$= f \circ \overset{-1}{f} = \mathrm{I_B}.$$

If $f''$ is an injection and $f$ a surjection, then $f'$ is an injection, by Proposition 8 if $\mathrm{A} \neq \emptyset$, and trivially if $\mathrm{A} = \emptyset$ (for then we have $\mathrm{B} = f\langle \mathrm{A}\rangle = \emptyset$).

#### Proposition 9 {#ens-ii-s3-prop-9 .statement tag=03PS}

(a) *Let* E, F, G *be sets, let* $g$ *be a mapping of* E *onto* F *and* $f$ *a mapping of* E *into* G. *Then there exists a mapping* $h$ *of* F *into* G *such that* $f = h \circ g$ *if and only if the relation* $g(x) = g(y)$ *(where* $x \in \mathrm{E}$, $y \in \mathrm{E}$*) implies the relation* $f(x) = f(y)$. *The mapping* $h$ *is then uniquely determined by* $f$; *if* $s$ *is a section of* $g$, *we have* $h = f \circ s$.

$$\begin{array}{ccc}
\mathrm{E} & \overset{f}{\searrow} & \\
{\scriptstyle g}\big\downarrow\big\uparrow{\scriptstyle s} & & \\
\mathrm{F} & \underset{h}{\longrightarrow} & \mathrm{G}
\end{array}
\qquad\qquad
\begin{array}{ccc}
 & \overset{f}{\nearrow} & \mathrm{E} \\
 & & {\scriptstyle r}\big\downarrow\big\uparrow{\scriptstyle g} \\
\mathrm{G} & \underset{h}{\longrightarrow} & \mathrm{F}
\end{array}$$
$$\text{(a)} \qquad\qquad\qquad \text{(b)}$$

(b) *Let* E, F, G *be sets, let* $g$ *be an injection of* F *into* E, *and let* $f$ *be a mapping of* G *into* E. *Then there exists a mapping* $h$ *of* G *into* F *such that* $f = g \circ h$ *if and only if* $f(\mathrm{G}) \subset f(\mathrm{F})$. *The mapping* $h$ *is uniquely determined by* $f$; *if* $r$ *is a retraction of* $g$, *we have* $h = r \circ f$.

(a) If $f = h \circ g$, the relation $g(x) = g(y)$ (where $x \in \mathrm{E}$, $y \in \mathrm{E}$) clearly implies $f(x) = f(y)$. And for every section $s$ of $g$ we have

$$h = h \circ (g \circ s) = f \circ s,$$

which shows that $h$ is uniquely determined by $f$. Conversely, suppose that the relation $g(x) = g(y)$ implies $f(x) = f(y)$; let $s$ be a section

of $g$, and let $h = f \circ s$; then for every $x \in E$ we have $g(s(g(x))) = g(x)$, hence $f(s(g(x))) = f(x)$, that is, $h(g(x)) = f(x)$ and therefore $f = h \circ g$.

(b) If $f = g \circ h$, then clearly $f(G) \subset f(F)$, and for every retraction $r$ of $g$ we have $h = (r \circ g) \circ h = r \circ f$, which shows that $h$ is uniquely determined by $f$. Conversely, suppose that $f(G) \subset f(F)$; let $r$ be a retraction of $g$, and put $h = r \circ f$; for every $x \in G$, there exists $y \in F$ such that $f(x) = g(y)$, so that

$$g(h(x)) = g(r(f(x))) = g(r(g(y))) = g(y) = f(x)$$

and therefore $f = g \circ h$.

### 9. FUNCTIONS OF TWO ARGUMENTS

A *function of two arguments* is a function whose domain is a set of ordered pairs (or, equivalently, a subset of a product). Let $f$ be such a function; if $(x, y)$ is an element of the domain of $f$, the value $f((x, y))$ of $f$ at the element $(x, y)$ is generally denoted by $f(x, y)$.

¶ Let $f$ be a function of two arguments, D its domain, and C its target. For each $y$ let $A_y$ be the set of all $x$ such that $(x, y) \in D$ (that is, the section of $\overset{-1}{D}$ at $y$ (no. 1)). The mapping

$$x \to f(x, y) \quad (x \in A_y, f(x, y) \in C)$$

is called *the partial mapping defined by $f$, with respect to the value $y$ of the second argument*, and is denoted by $f(\bullet, y)$, or $f(\ , y)$ (or sometimes $f_y$); we have $f(\bullet, y)(x) = f(x, y)$ for all $(x, y) \in D$. Similarly, for each $x$ let $B_x$ be the set of all $y$ such that $(x, y) \in D$. The mapping

$$y \to f(x, y) \quad (y \in B_x, f(x, y) \in C)$$

is called *the partial mapping defined by $f$, with respect to the value $x$ of the first argument*, and is denoted by $f(x, \bullet)$, or $f(x, \ )$ (or sometimes $f_x$); we have $f(x, \bullet)(y) = f(x, y)$ for all $(x, y) \in D$.

¶ If for every $y$ (resp. $x$) the partial mapping $f(\bullet, y)$ (resp. $f(x, \bullet)$) is a constant mapping, we say that $f$ *does not depend on* its first (resp. second) argument; this means therefore that $f(x, y) = f(x', y)$ whenever $(x, y)$ and $(x', y)$ belong to D (resp. $f(x, y) = f(x, y')$ whenever $(x, y)$ and $(x, y')$ belong to D). For each $y$ belonging to the second projection of D let $g(y)$ denote the common value of the $f(x, y)$ for $x \in A_y$; the mapping $y \to g(y)$ is then a mapping of $\mathrm{pr}_2 D$ into C such that

$$g(y) = f(x, y) \qquad \text{for all } (x, y) \in D.$$

¶ Conversely, let $g$ be a mapping of a set B into a set C, and let A be any set. Then the mapping $(x, y) \to g(y)$ of $A \times B$ into C does not depend on its first argument.

¶ Let $u$ be a mapping of A into C and $v$ a mapping of B into D. The mapping $z \to (u(\mathrm{pr}_1 z), v(\mathrm{pr}_2 z))$ of $A \times B$ into $C \times D$ is called the (*canonical*) *extension of $u$ and $v$ to the product sets*, or simply *the product of $u$ and $v$* (if there is no risk of confusion); its range is $u\langle A\rangle \times v\langle B\rangle$. It is denoted by $u \times v$. If $u$ and $v$ are injective (resp. surjective) then $u \times v$ is injective (resp. surjective). If $u$ and $v$ are bijective, then $u \times v$ is bijective, and its inverse mapping is $\overset{-1}{u} \times \overset{-1}{v}$. If $u'$ is a mapping of C into a set E and if $v'$ is a mapping of D into a set F, we have

$$(u' \times v') \circ (u \times v) = (u' \circ u) \times (v' \circ v).$$

If U, V are the graphs of $u$, $v$ respectively, the graph W of $u \times v$ is the set of ordered pairs $((x,y), (z, t))$ of $(A \times B) \times (C \times D)$ such that $(x, z) \in U$ and $(y, t) \in V$; the mapping $((x, y), (z, t)) \to ((x, z), (y, t))$ puts W in one-to-one correspondence with the product $U \times V$ (a subset of $(A \times C) \times (B \times D)$) (cf. §5, no. 5).

### Exercises {#ens-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
