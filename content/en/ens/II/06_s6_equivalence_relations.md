---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 6
section_title: Equivalence relations
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 112-122, 127-129
pdf_pages: 0119-0129, 0134-0136
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN EQUIVALENCE RELATION
      page: 113
      pdf_page: 120
    - "no": 2
      title: EQUIVALENCE CLASSES ; QUOTIENT SET
      page: 114
      pdf_page: 121
    - "no": 3
      title: RELATIONS COMPATIBLE WITH AN EQUIVALENCE RELATION
      page: 116
      pdf_page: 123
    - "no": 4
      title: SATURATED SUBSETS
      page: 117
      pdf_page: 124
    - "no": 5
      title: MAPPINGS COMPATIBLE WITH EQUIVALENCE RELATIONS
      page: 118
      pdf_page: 125
    - "no": 6
      title: INVERSE IMAGE OF AN EQUIVALENCE RELATION; INDUCED EQUIVALENCE RELATION
      page: 119
      pdf_page: 126
    - "no": 7
      title: QUOTIENTS OF EQUIVALENCE RELATIONS
      page: 119
      pdf_page: 126
    - "no": 8
      title: PRODUCT OF TWO EQUIVALENCE RELATIONS
      page: 120
      pdf_page: 127
    - "no": 9
      title: CLASSES OF EQUIVALENT OBJECTS
      page: 121
      pdf_page: 128
statements: 13
exercises: 11
content_sha256: e6575e4e849279138a1a581ab84cb1b482758b417a93c62ef93c5b5e7766db0c
---

## 6. EQUIVALENCE RELATIONS

In principle, from now on we shall stop using bold-face italic letters to denote undetermined assemblies; the reader will be able to discern easily from the context the assertions which apply to undetermined letters or relations.

### 1. DEFINITION OF AN EQUIVALENCE RELATION

Let $R\{x, y\}$ be a relation, $x$ and $y$ being distinct letters. The relation $R$ is said to be *symmetric* (with respect to the letters $x$ and $y$) if

$$R\{x, y\} \Rightarrow R\{y, x\}.$$

If so, by substituting for $x$ and $y$ two letters $x'$ and $y'$, distinct from each other and from all the letters which appear in $R$, and then by substituting $y$ and $x$ for $x'$ and $y'$, respectively, we see that

$$R\{y, x\} \Rightarrow R\{x, y\}.$$

Hence $R\{x, y\}$ and $R\{y, x\}$ are equivalent.

¶ Let $z$ be a letter which does not appear in $R$. The relation $R$ is said to be *transitive* (with respect to the letters $x, y$) if we have

$$(R\{x, y\} \text{ and } R\{y, z\}) \Rightarrow R\{x, z\}.$$

#### Example {#ens-ii-s6-n1-exa-7 .statement}

The relation $x = y$ is symmetric and transitive. The relation $X \subset Y$ is transitive but not symmetric. The relation $X \cap Y = \emptyset$ is symmetric but not transitive.

If $R\{x, y\}$ is both symmetric and transitive it is said to be an *equivalence relation* (with respect to the letters $x$ and $y$). In this case the notation $x \equiv y \pmod{R}$ is sometimes used as a synonym of $R\{x, y\}$; it is read "*x is equivalent to y modulo* $R$". If $R$ is an equivalence relation, we have $R\{x, y\} \Rightarrow (R\{x, x\}$ and $R\{y, y\})$, because $R\{x, y\}$ implies $R\{y, x\}$, and $(R\{x, y\}$ and $R\{y, x\})$ implies $(R\{x, x\}$ and $R\{y, y\})$ by virtue of the definitions.

¶ Let $R\{x, y\}$ be a relation; it is said to be *reflexive on* $E$ (with respect to the letters $x, y$) if the relation $R\{x, x\}$ is equivalent to $x \in E$. If there is no possible ambiguity about $E$, one says simply, by abuse of language, that $R$ is reflexive.

¶ An *equivalence relation on* $E$ is defined to be an equivalence relation which is reflexive on $E$. If $R\{x, y\}$ is an equivalence relation on $E$, we have $R\{x, y\} \Rightarrow ((x, y) \in E \times E)$, hence $R$ has a graph (with respect to the letters $x, y$). Conversely, suppose that the equivalence relation $R\{x, y\}$ has a graph $G$. Observe that the relation $R\{x, x\}$ is equivalent to the relation $(\exists y)R\{x, y\}$; for the former implies the latter (Chapter I, § 4, no. 2, scheme S5), and conversely, since $R\{x, y\}$ implies $R\{x, x\}$, $(\exists y) R\{x, y\}$ implies $(\exists y) R\{x, x\}$ and therefore also $R\{x, x\}$. Thus $R\{x, x\}$ is equivalent to $x \in \mathrm{pr}_1 G$, and hence $R$ is an equivalence relation on $\mathrm{pr}_1 G$.

¶ An *equivalence* on a set E is a correspondence whose source and target are both equal to E, and whose graph F is such that the relation $(x, y) \in F$ is an equivalence relation on E.

*Examples*

#### Example 1 {#ens-ii-s6-n1-exa-1 .statement tag=03IX}

The relation $x = y$ is an equivalence relation which has no graph, for if it did, the first projection of this graph would be the set of all objects.

#### Example 2 {#ens-ii-s6-n1-exa-2 .statement tag=03SC}

The relation "$x = y$ and $x \in E$" is an equivalence relation on E whose graph is the diagonal of $E \times E$.

#### Example 3 {#ens-ii-s6-n1-exa-3 .statement tag=03TQ}

The relation "there exists a bijection of X onto Y" is an equivalence relation which has no graph (cf. Chapter III, § 3).

#### Example 4 {#ens-ii-s6-n1-exa-4 .statement tag=03TR}

The relation "$x \in E$ and $y \in E$" is an equivalence relation on E, whose graph is $E \times E$.

#### Example 5 {#ens-ii-s6-n1-exa-5 .statement tag=03TS}

Suppose $A \subset E$; then the relation

$$(x \in E - A \text{ and } y = x) \text{ or } (x \in A \text{ and } y \in A)$$

is an equivalence relation on E.

#### Example 6 {#ens-ii-s6-n1-exa-6 .statement tag=03TP}

\* The relation "$x \in \mathbf{Z}$ and $y \in \mathbf{Z}$ and $x - y$ is divisible by 4" is an equivalence relation on $\mathbf{Z}$.\*

#### Proposition 1 {#ens-ii-s6-prop-1 .statement tag=03QH}

*A correspondence* $\Gamma$ *between* X *and* X *is an equivalence on* X *if and only if it satisfies the following conditions :* (a) X *is the domain of* $\Gamma$; (b) $\Gamma = \overset{-1}{\Gamma}$; (c) $\Gamma \circ \Gamma = \Gamma$.
Let $\Gamma$ be a correspondence between X and X, and let G be its graph. If $\Gamma$ is an equivalence on X, then $(x, x) \in G$ for all $x \in X$; hence X is the domain of $\Gamma$. The relation $(x, y) \in G$ is equivalent to $(y, x) \in G$, hence to $(x, y) \in \overset{-1}{G}$, so that $G = \overset{-1}{G}$ and therefore $\Gamma = \overset{-1}{\Gamma}$. The relations $(x, y) \in G$ and $(y, z) \in G$ imply $(x, z) \in G$, so that $G \circ G \subset G$; conversely, $(x, y) \in G$ implies $(x, x) \in G$ and therefore $(x, y) \in G \circ G$, so that $G \subset G \circ G$; hence $G = G \circ G$ and consequently $\Gamma = \Gamma \circ \Gamma$.
¶ Conversely, suppose that conditions (a), (b), and (c) are satisfied. The relation $(x, y) \in G$ is symmetric (by (b)) and transitive (by (c)); hence it is an equivalence relation, and by (a) it is an equivalence relation on X.

### 2. EQUIVALENCE CLASSES ; QUOTIENT SET

Let $f$ be a function, E its domain, F its graph. The relation "$x \in E$ and $y \in E$ and $f(x) = f(y)$" is an equivalence relation on E, called the equivalence relation *associated with f*. It is equivalent to the relation $(\exists z)((x, z) \in F$ and $(y, z) \in F)$, i.e., to $(\exists z)((x, z) \in F$ and $(z, y) \in \overset{-1}{F})$, and therefore its graph is $\overset{-1}{F} \circ F$.

¶ We shall now show that every equivalence relation $\mathrm{R}$ on a set $\mathrm{E}$ is of this type. Let $\mathrm{G}$ be the graph of $\mathrm{R}$. For each $x \in \mathrm{E}$ the (non-empty) set $\mathrm{G}(x) \subset \mathrm{E}$ is called the *equivalence class of $x$ with respect to* $\mathrm{R}$; it is thus the set of all $y \in \mathrm{E}$ such that $\mathrm{R}\{x, y\}$. Every set which can be written as $\mathrm{G}(x)$ for some $x \in \mathrm{E}$ is called an equivalence class (with respect to $\mathrm{R}$). An element of an equivalence class is called a *representative* of this class. The set of equivalence classes with respect to $\mathrm{R}$ (that is, the set of all objects of the form $\mathrm{G}(x)$ for some $x \in \mathrm{E}$) is called the *quotient set* of $\mathrm{E}$ by $\mathrm{R}$ and is denoted by $\mathrm{E}/\mathrm{R}$. The mapping $x \to \mathrm{G}(x)$ $(x \in \mathrm{E})$ whose domain is $\mathrm{E}$ and whose target is $\mathrm{E}/\mathrm{R}$ is called the *canonical mapping* of $\mathrm{E}$ onto $\mathrm{E}/\mathrm{R}$.

C55. *Let* $\mathrm{R}$ *be an equivalence relation on a set* $\mathrm{E}$, *and let $p$ be the canonical mapping of* $\mathrm{E}$ *onto* $\mathrm{E}/\mathrm{R}$. *Then*

$$\mathrm{R}\{x, y\} \Leftrightarrow (p(x) = p(y)).$$

With the notation above, let $x$ and $y$ be elements of $\mathrm{E}$ such that

$$(x, y) \in \mathrm{G}.$$

Then $x \in \mathrm{E}$ and $y \in \mathrm{E}$; let us show that $\mathrm{G}(x) = \mathrm{G}(y)$. Since $y \in \mathrm{G}(x)$, we have (Proposition 1) $\mathrm{G}(y) \subset (\mathrm{G} \circ \mathrm{G})(x) = \mathrm{G}(x)$. On the other hand, we also have $(y, x) \in \mathrm{G}$, whence $\mathrm{G}(x) \subset \mathrm{G}(y)$ and therefore

$$\mathrm{G}(x) = \mathrm{G}(y),$$

i.e., $p(x) = p(y)$. Conversely, if $\mathrm{G}(x) = \mathrm{G}(y)$, we have $y \in \mathrm{G}(y) = \mathrm{G}(x)$, so that $(x, y) \in \mathrm{G}$. This completes the proof.

¶ A section of the canonical mapping $p$ of $\mathrm{E}$ onto $\mathrm{E}/\mathrm{R}$ (§ 3, no. 8, Definition 11) is called more briefly a *section* of $\mathrm{E}$ (with respect to the relation $\mathrm{R}$).

*Examples*

#### Example 1 {#ens-ii-s6-n2-exa-1 .statement tag=03SD}

Let $\mathrm{R}$ be the equivalence relation "$x \in \mathrm{E}$ and $y \in \mathrm{E}$ and $x = y$" on a set $\mathrm{E}$. The equivalence class of $x \in \mathrm{E}$ is then the set $\{x\}$, and the canonical mapping $x \to \{x\}$ of $\mathrm{E}$ onto $\mathrm{E}/\mathrm{R}$ is bijective.

#### Example 2 {#ens-ii-s6-n2-exa-2 .statement tag=03SE}

Let $\mathrm{E}$, $\mathrm{F}$ be two sets and let $\mathrm{R}$ be the equivalence relation on $\mathrm{E} \times \mathrm{F}$ associated with the mapping $\mathrm{pr}_1$ of $\mathrm{E} \times \mathrm{F}$ onto $\mathrm{E}$. The equivalence classes with respect to $\mathrm{R}$ are the sets of the form $\{x\} \times \mathrm{F}$, where $x \in \mathrm{E}$; the mapping $x \to \{x\} \times \mathrm{F}$ is a bijection of $\mathrm{E}$ onto $(\mathrm{E} \times \mathrm{F})/\mathrm{R}$.

Let $\mathrm{R}$ be an equivalence relation on a set $\mathrm{E}$. The quotient set $\mathrm{E}/\mathrm{R}$ is a subset of $\mathfrak{P}(\mathrm{E})$, and the identity mapping of $\mathrm{E}/\mathrm{R}$ is a *partition* of $\mathrm{E}$ (§ 4, no. 7); for if $\mathrm{G}$ is the graph of $\mathrm{R}$, we have $x \in \mathrm{G}(x)$ for all $x \in \mathrm{E}$, and if two equivalence classes $\mathrm{G}(x)$ and $\mathrm{G}(y)$ have a common element $z$, then $\mathrm{R}\{x,\ z\}$ and $\mathrm{R}\{y,\ z\}$, so that $\mathrm{G}(x) = \mathrm{G}(y)$. Furthermore, the relation

$$(\exists \mathrm{X})(\mathrm{X} \in \mathrm{E}/\mathrm{R} \text{ and } x \in \mathrm{X} \text{ and } y \in \mathrm{X})$$

is equivalent to $\mathrm{R}\{x,\ y\}$.

¶ Conversely, let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a partition of a set E. It is immediately verified that the relation $(\exists \iota)(\iota \in \mathrm{I}$ and $x \in \mathrm{X}_\iota$ and $y \in \mathrm{Y}_\iota)$ is an equivalence relation R on E; the equivalence classes with respect to R are just the sets $\mathrm{X}_\iota$ of the partition, and the mapping $\iota \to \mathrm{X}_\iota$ is a bijection of I onto E/R. Every subset S of E such that, for each $\iota \in \mathrm{I}$, the set $\mathrm{S} \cap \mathrm{X}_\iota$ consists of a single element is called a *system of representatives* (or a *transversal*) of the equivalence classes with respect to R. This name is also used to denote any injection of a set K into E such that the image of K under this injection is a system of representatives of the equivalence classes with respect to R; for example, any *section* of E with respect to R.

### 3. RELATIONS COMPATIBLE WITH AN EQUIVALENCE RELATION

Let $\mathrm{R}\{x,\ x'\}$ be an equivalence relation and let $\mathrm{P}\{x\}$ be a relation. The relation $\mathrm{P}\{x\}$ is said to be *compatible with the equivalence relation* $\mathrm{R}\{x,\ x'\}$ (with respect to $x$) if we have

$$(\mathrm{P}\{x\} \text{ and } \mathrm{R}\{x,\ y\}) \Rightarrow \mathrm{P}\{y\},$$

where $y$ denotes a letter which appears neither in P nor in R.

For example, it follows from C43 (Chapter I, §5), no. 1) that every relation $\mathrm{P}\{x\}$ is compatible with the equivalence relation $x = x'$.

C56. *Let* $\mathrm{R}\{x,\ x'\}$ *be an equivalence relation on a set* E, *and let* $\mathrm{P}\{x\}$ *be a relation which does not contain the letter* $x'$ *and is compatible (with respect to* $x$*) with the equivalence relation* $\mathrm{R}\{x,\ x'\}$. *Then, if* $t$ *does not appear in* $\mathrm{P}\{x\}$, *the relation "*$t \in \mathrm{E}/\mathrm{R}$ *and* $(\exists x)(x \in t$ *and* $\mathrm{P}\{x\})$*" is equivalent to the relation "*$t \in \mathrm{E}/\mathrm{R}$ *and* $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$*".*

Let $t \in \mathrm{E}/\mathrm{R}$. If there exists $a \in t$ such that $\mathrm{P}\{a\}$, then for each $x \in t$ we have $\mathrm{R}\{a,\ x\}$ and hence $\mathrm{P}\{x\}$. Hence $(\exists x)(x \in t$ and $\mathrm{P}\{x\})$ implies $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$. The converse is obvious since $t \in \mathrm{E}/\mathrm{R}$ implies that $t \neq \emptyset$.

¶ The relation

$$t \in \mathrm{E}/\mathrm{R} \text{ and } (\exists x)(x \in t \text{ and } \mathrm{P}\{x\})$$

is said to be *induced by* $P\{x\}$ *on passing to the quotient* (with respect to $x$) with respect to R. If this relation is denoted by $P'\{t\}$, and if $f$ is the canonical mapping of E onto E/R, then the relation

$$y \in E \text{ and } P'\{f(y)\}$$

(where $y$ does not appear in $P\{x\}$) is *equivalent* to ( $y \in E$ and $P\{y\}$), as is immediately verified.

### 4. SATURATED SUBSETS

Let $R\{x, y\}$ be an equivalence relation on a set E, and let A be a subset of E. A is said to be *saturated with respect to* R if the relation $x \in A$ is compatible (with respect to $x$) with $R\{x, y\}$; or, equivalently, if *for each $x \in A$ the equivalence class of $x$ is contained in* A. In other words, a set is saturated with respect to R if and only if it is the *union of a set of equivalence classes with respect to* R.

¶ Let $f$ be the canonical mapping of E onto E/R. If A is saturated with respect to R, then the equivalence class of each $x \in A$, which is equal to $\overset{-1}{f}\langle\{f(x)\}\rangle$, is contained in A, and hence $\overset{-1}{f}\langle f\langle A\rangle\rangle \subset A$; since in any case we have $A \subset \overset{-1}{f}\langle f\langle A\rangle\rangle$, it follows that $\overset{-1}{f}\langle f\langle A\rangle\rangle = A$. Conversely, if $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$, then for every $x \in A$ the equivalence class $K = f(x)$ of $x$ with respect to R is an element of $f\langle A\rangle$; and since $K = \overset{-1}{f}\langle\{K\}\rangle$, we have $K \subset \overset{-1}{f}\langle f\langle A\rangle\rangle = A$. Thus the subsets of E which are saturated with respect to R are precisely the subsets A of E such that $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$. Equivalently, they are the subsets of E of the form $\overset{-1}{f}\langle B\rangle$, where $B \subset E/R$; for the relation $A = \overset{-1}{f}\langle B\rangle$ implies $B = f\langle A\rangle$, hence $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$.

¶ If $(X_\iota)_{\iota \in I}$ is a family of saturated subsets of E, then the sets $\bigcup_{\iota \in I} X_\iota$ and $\bigcap_{\iota \in I} X_\iota$ are saturated (§4, Propositions 3 and 4). If A is a saturated subset of E, then so is $\complement_E A$ (§4, Proposition 6).

¶ Let A now be an arbitrary subset of E. Then the set $\overset{-1}{f}\langle f\langle A\rangle\rangle$ contains A and is saturated. Conversely, if A′ is a saturated subset of E which contains A, we have $f\langle A'\rangle \supset f\langle A\rangle$, so that

$$A' = \overset{-1}{f}\langle f\langle A'\rangle\rangle \supset \overset{-1}{f}\langle f\langle A\rangle\rangle.$$

Hence we may say that $\overset{-1}{f}\langle f\langle A\rangle\rangle$ is the "smallest" saturated subset of E which contains A (cf. Chapter III); this set is called the *saturation* of A with respect to the relation R. It is immediately seen that the saturation of A is the union of the equivalence classes of the elements of A. If $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is a family of subsets of E and if $\mathrm{A}_\iota$ is the saturation of $\mathrm{X}_\iota$ with respect to R, then the saturation of $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ is $\bigcup_{\iota \in \mathrm{I}} \mathrm{A}_\iota$ (§4, Proposition 3).

### 5. MAPPINGS COMPATIBLE WITH EQUIVALENCE RELATIONS

Let R be an equivalence relation on a set E, and let $f$ be a function with domain E. Then $f$ is said to be *compatible with the relation* R if the relation $y = f(x)$ is compatible (with respect to $x$) with the relation $\mathrm{R}\{x,\ x'\}$.

¶ It comes to the same thing to say that the restriction of $f$ to each equivalence class is a constant mapping, in which case we say that *$f$ is constant on each equivalence class with respect to* R. If $g$ is the canonical mapping of E onto E/R, an equivalent statement is that the relation $g(x) = g(x')$ implies $f(x) = f(x')$; hence (§3, Proposition 9) we have the following criterion :

C57. *Let* R *be an equivalence relation on a set* E, *and let g be the canonical mapping of* E *onto* E/R. *Then a mapping f of* E *into* F *is compatible with* R *if and only if f can be put in the form h $\circ$ g, where h is a mapping of* E/R *into* F. *The mapping h is uniquely determined by f; if s is any section of g, we have h $= f \circ s$.*

The mapping $h$ is said to be *induced by f on passing to the quotient* with respect to R.

¶ Let $f$ be a mapping of a set E into a set F, and let $\mathrm{A} = f\langle \mathrm{E}\rangle \subset \mathrm{F}$. Let R be the equivalence relation associated with $f$ (no. 2); it is clear that $f$ is compatible with R. Moreover, the mapping $h$ induced by $f$ on passing to the quotient is an *injection* of E/R into F : for if $t$, $t'$ are equivalence classes with respect to R such that $h(t) = h(t')$, we have $f(x) = f(x')$ for all $x \in t$ and $x' \in t'$, which implies $t = t'$ by the definition of R. Let $k$ be the mapping of E/R onto A which has the same graph as $h$; then $k$ is *bijective*. If $j$ is the canonical injection of A into F and if $g$ is the canonical mapping of E onto E/R, then we may write

$$f = j \circ k \circ g.$$

This relation is called the *canonical decomposition of f*.

¶ Let $f$ be a mapping of a set E into a set F, let R be an equivalence relation on E, and let S be an equivalence relation on F. Let $u$ be the canonical mapping of E onto E/R, and let $v$ be the canonical mapping of $F$ onto $F/S$. The mapping $f$ is said to be *compatible with the equivalence relations* $R$ and $S$ if $v\mathbin{\circ}f$ is compatible with $R$; this means that the relation $x\equiv x'$ (mod $R$) *implies* $f(x)\equiv f(x')$ (mod $S$). The mapping $h$ of $E/R$ into $F/S$ induced by $v\mathbin{\circ}f$ on passing to the quotient with respect to $R$ is then called the *mapping induced by $f$ on passing to the quotients with respect to $R$ and $S$*; it is characterized by the relation $v\mathbin{\circ}f=h\mathbin{\circ}u$.

### 6. INVERSE IMAGE OF AN EQUIVALENCE RELATION; INDUCED EQUIVALENCE RELATION

Let $\varphi$ be a mapping of a set $E$ into a set $F$, and let $S$ be an equivalence relation on $F$. If $u$ is the canonical mapping of $F$ onto $F/S$, the equivalence relation associated with the mapping $u\mathbin{\circ}\varphi$ of $E$ into $F/S$ is called the *inverse image* of $S$ under $\varphi$; if $R$ is this relation, $R\{x,y\}$ is equivalent to $S\{\varphi(x),\varphi(y)\}$, and the equivalence classes with respect to $R$ are the inverse images under $\varphi$ of the equivalence classes with respect to $S$ which meet $\varphi\langle E\rangle$.

¶ In particular, consider an equivalence relation $R$ on a set $E$, and let $A$ be a subset of $E$; then the inverse image of $R$ under the injection $j$ of $A$ into $E$ is called the equivalence relation *induced* by $R$ on $A$, and is denoted by $R_A$.

¶ The equivalence classes with respect to $R_A$ are the *traces* on $A$ of the equivalence classes with respect to $R$ which meet $A$. The injection $j$ is obviously compatible with the relations $R_A$ and $R$; the mapping $h$ of $A/R_A$ into $E/R$ induced by $j$ on passing to the quotient with respect to $R_A$ and $R$ is an *injective* mapping of $A/R_A$ into $E/R$: for if $f$ (resp. $g$) is the canonical mapping of $E$ onto $E/R$ (resp. $A$ onto $A/R_A$), then the relation $h(g(x))=h(g(x'))$, where $x\in A$ and $x'\in A$, is equivalent to $f(x)=f(x')$ and therefore to $g(x)=g(x')$. The image $h\langle A/R_A\rangle$ is equal to $f\langle A\rangle$. If $k$ is the bijective mapping of $A/R_A$ onto $f\langle A\rangle$ which has the same graph as $h$, then $k$ and its inverse are said to be *canonical*.

### 7. QUOTIENTS OF EQUIVALENCE RELATIONS

Let $R$, $S$ be two equivalence relations with respect to two letters $x$, $y$. We shall say that $S$ is *finer* than $R$ (or that $R$ is *coarser* than $S$) if the relation $S\Rightarrow R$ is true. If $R$ and $S$ are equivalence relations on the same set $E$, the statement that $S$ is finer than $R$ means that the graph of $S$ is contained in that of $R$, or again that every equivalence class with respect to $S$ is contained in an equivalence class with respect to $R$; or, equivalently, that every equivalence class with respect to $R$ is saturated with respect to $S$.

*Examples*

#### Example 1 {#ens-ii-s6-n7-exa-1 .statement tag=03SF}

The relation "$x \in E$ and $y \in E$ and $x = y$" is finer than every equivalence relation on E. The relation "$x \in E$ and $y \in E$" is coarser than every equivalence relation on E.

#### Example 2 {#ens-ii-s6-n7-exa-2 .statement tag=03SG}

\* The equivalence relation "$x \in \mathbf{Z}$ and $y \in \mathbf{Z}$ and $x - y$ is divisible by 4" is finer than the equivalence relation "$x \in \mathbf{Z}$ and $y \in \mathbf{Z}$ and $x - y$ is divisible by 2". \*

Let R and S be two equivalence relations on the same set E, such that S is finer than R. Let $f$ and $g$ be the canonical mappings of E onto E/R and E onto E/S respectively; then the function $f$ is compatible with S. Let $h$ be the function induced by $f$ on passing to the quotient with respect to S; then $h$ is a mapping of E/S onto E/R. The equivalence relation associated with $h$ on E/S is called the *quotient of* R *by* S and is denoted by R/S. The relation $x \equiv y \pmod{R}$ is equivalent to $g(x) \equiv g(y) \pmod{R/S}$, and the equivalence classes with respect to R/S are the images under $g$ of the equivalence classes with respect to R. Let $h = j \circ h_2 \circ h_1$ be the canonical decomposition (no. 5) of the mapping $h$. Then $h_1$ is the canonical mapping of E/S onto (E/S)/(R/S), $j$ is the identity mapping of E/R, and $h_2$ is a one-to-one mapping of (E/S)/(R/S) onto E/R. The mapping $h_2$ and its inverse are said to be *canonical*.

¶ Conversely, consider an arbitrary equivalence relation T on the set E/S, and let R be the equivalence relation on E which is the inverse image under $g$ of the relation T (no. 6). Since the relation $x \equiv y \pmod{R}$ is equivalent to $g(x) \equiv g(y) \pmod{T}$, it follows that T is equivalent to R/S.

### 8. PRODUCT OF TWO EQUIVALENCE RELATIONS

Let $R\{x, y\}$ and $R'\{x', y'\}$ be two equivalence relations. Let $S\{u, v\}$ denote the relation

$$(\exists x)(\exists y)(\exists x')(\exists y')(u = (x, x') \text{ and } v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

it is immediately verified that $S\{u, v\}$ is an equivalence relation, called the *product* of R and R', and denoted by $R \times R'$. Suppose that R is an equivalence relation on a set E and that R' is an equivalence relation on a set E'. Then the relation $S\{u, u\}$ is equivalent to

$$(\exists x)(\exists x')(u = (x, x') \text{ and } R\{x, x\} \text{ and } R'\{x', x'\})$$

i.e., to $(\exists x)(\exists x')(u = (x, x')$ and $x \in E$ and $x' \in E')$, hence to $u \in E \times E'$. It follows that $R \times R'$ is an equivalence relation on $E \times E'$. If

$$u = (x, x')$$

is an element of $E \times E'$, the relation $S\{u, v\}$ is equivalent to

$$(\exists y)(\exists y')(v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

if $G$ and $G'$ are the graphs of $R$ and $R'$, respectively, this relation is in turn equivalent to $v \in G(x) \times G(x')$. Hence *every equivalence class with respect to* $R \times R'$ *is the product of an equivalence class with respect to* $R$ *and an equivalence class with respect to* $R'$, *and conversely.*

¶ Let $f$ and $f'$ be the canonical mappings of $E$ onto $E/R$ and $E'$ onto $E'/R'$, respectively, and let $f \times f'$ be the canonical extension of $f$ and $f'$ to the product sets (§ 3, no. 9). Then $(f \times f')(x, x') = (f(x), f'(x'))$ for all $(x, x') \in E \times E'$. The inverse image under $f \times f'$ of an element $(u, u')$ of $(E/R) \times (E'/R')$ is just the product $u \times u'$ of the equivalence class $u$ with respect to $R$ and the equivalence class $u'$ with respect to $R'$. It follows that the equivalence relation associated with $f \times f'$ is equivalent to $R \times R'$. The mapping $f \times f'$ can therefore be written as $h \circ g$, where $g$ is the canonical mapping of $E \times E'$ onto

$$(E \times E')/(R \times R')$$

and $h$ is a one-to-one mapping of $(E \times E')/(R \times R')$ onto

$$(E/R) \times (E'/R');$$

this mapping $h$ and its inverse are said to be *canonical*.

#### Remark {#ens-ii-s6-n8-rem-1 .statement tag=03IY}

Let $P\{x, x'\}$ be a relation in which the letters $y$, $y'$ do not occur. P is said to be *compatible* with the equivalence relations $R\{x, y\}$ and $R'\{x', y'\}$ (with respect to $x$ and $x'$) if the relation $(P\{x, x'\}$ and $R\{x, y\}$ and $R'\{x', y'\})$ implies $P\{y, y'\}$. Let $Q\{u\}$ be the relation $(\exists x)(\exists x')(u = (x, x')$ and $P\{x, x'\})$; then it comes to the same thing to say that $Q\{u\}$ is compatible (with respect to $u$) with the equivalence relation $S\{u, v\}$, the product of $R$ and $R'$.

### 9. CLASSES OF EQUIVALENT OBJECTS

Let $R\{x, y\}$ be an equivalence relation, which need not have a graph. It is obvious that if $x$, $x'$, $y$ are three distinct letters, the relation $R\{x, x'\}$ implies "$R\{x, y\} \Longleftrightarrow R\{x', y\}$" and therefore also implies the relation $(\forall y)(R\{x, y\} \Longleftrightarrow R\{x', y\})$. By the scheme S7 (Chapter I, § 5, no. 1), if we put $\theta\{x\} = \tau_y(R\{x, y\})$, the relation $R\{x, x'\}$ implies

$$\theta\{x\} = \theta\{x'\}.$$

Note, on the other hand, that by definition $R\{x, \theta\{x\}\}$ is the relation $(\exists y)(R\{x, y\})$ and hence (no. 1) is equivalent to $R\{x, x\}$. It follows that the relation $(R\{x, x\}$ and $R\{x', x'\}$ and $\theta\{x\} = \theta\{x'\})$ is *equivalent* to $R\{x, x'\}$, for it implies, by S6 (Chapter I, §5, no. 1), the relation

$$(R\{x, x\} \text{ and } R\{x', x'\} \text{ and } (R\{x', \theta\{x\}\} \Leftrightarrow R\{x', \theta\{x'\}\})),$$

hence also $(R\{x, \theta\{x\}\}$ and $R\{x', \theta\{x\}\})$, and finally $R\{x, x'\}$ by transitivity and symmetry. And since, conversely, $R\{x, x'\}$ implies $R\{x, x\}$ and $R\{x', x'\}$, the assertion is proved. The term $\theta\{x\}$ is called the *class of objects equivalent to x* (with respect to the relation R).

¶ Suppose now that T is a term such that the relation

(1) $$(\forall y)(R\{y, y\} \Rightarrow (\exists x)(x \in T \text{ and } R\{x, y\}))$$

is true. Then the relation $(\exists x)(R\{x, x\}$ and $z = \theta\{x\})$ is *collectivizing in z*. For we may suppose that $x \in T$ implies $R\{x, x\}$; it is sufficient to replace T by the set of all $x \in T$ such that $R\{x, x\}$ (observing that $R\{x, y\}$ implies $R\{x, x\}$). Let $\Theta$ be the set of all objects of the form $\theta\{x\}$ for $x \in T$ (§1, no. 6). Suppose that $R\{y, y\}$ is true; then there exists $x \in T$ such that $R\{x, y\}$ and therefore $\theta\{y\} = \theta\{x\} \in \Theta$. The set $\Theta$ is called the *set of classes of equivalent objects* with respect to R; and for each $x$ such that $R\{x, x\}$, $\theta\{x\}$ is the *unique* element $z \in \Theta$ such that $R\{x, z\}$.

Under the same hypothesis, let $A\{x\}$ be a term such that $R\{x, y\}$ implies $A\{x\} = A\{y\}$. Then the relation $(\exists x)(R\{x, x\}$ and $z = \{x\})$ is collectivizing in $z$, since $R\{x, x\}$, being equivalent to $R\{x, \theta\{x\}\}$, implies $A\{x\} = A\{\theta\{x\}\}$, and consequently if E is the set of objects of the form $A\{t\}$ for $t \in \Theta$, then $R\{x, x\}$ implies $A\{x\} \in E$. If $f$ is the function $t \to A\{t\}$ $(t \in \Theta, A\{t\} \in E)$, then the relation $R\{x, x\}$ implies $A\{x\} = f(\theta\{x\})$.

In particular, if R is an equivalence relation *on a set* F, we may take $A\{x\}$ to be the *equivalence class of x with respect to* R (no. 2), and the function $f$ is then a *bijection* of $\Theta$ onto the quotient set F/R; this justifies the terminology introduced.

\* *Example*. Let $R\{x, y\}$ be the equivalence relation "$x$ and $y$ are two vector spaces of the same finite dimension over $\mathbf{C}$"; this relation has no graph. It satisfies condition (1) when T is the set of all vector subspaces of $\mathbf{C}^{(\mathbf{N})}$, or when the subset T' of T consists of the spaces $\mathbf{C}^n$ $(n \in \mathbf{N})$ with the conventions that $\mathbf{C}^0$ consists of the point 0 of $\mathbf{C}^{(\mathbf{N})}$ and that $\mathbf{C}^n$ $(n > 0)$ is the sum of the first $n$ components of the direct sum $\mathbf{C}^{(\mathbf{N})}$. With this second choice we have $\Theta = T'$.\*

### Exercises {#ens-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
