---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 1
section_title: Collectivizing relations
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 65-72, 123
pdf_pages: 0072-0079, 0130-0130
extraction: ocr
subsections:
    - "no": 1
      title: THE THEORY OF SETS
      page: 65
      pdf_page: 72
    - "no": 2
      title: INCLUSION
      page: 66
      pdf_page: 73
    - "no": 3
      title: THE AXIOM OF EXTENT
      page: 67
      pdf_page: 74
    - "no": 4
      title: COLLECTIVIZING RELATIONS
      page: 67
      pdf_page: 74
    - "no": 5
      title: THE AXIOM OF THE SET OF TWO ELEMENTS
      page: 69
      pdf_page: 76
    - "no": 6
      title: THE SCHEME OF SELECTION AND UNION
      page: 69
      pdf_page: 76
    - "no": 7
      title: COMPLEMENT OF A SET. THE EMPTY SET
      page: 71
      pdf_page: 78
statements: 10
exercises: 6
content_sha256: d56a752b9382bcb5c79d67d5985b55c2f3bd6fb3df74a70fba0b4987d204ff5e
---

## 1. COLLECTIVIZING RELATIONS

### 1. THE THEORY OF SETS

The *theory of sets* is a theory which contains the relational signs $=$, $\in$ and the substantific sign $\supset$ (all these signs being of weight 2); in addition to the schemes S1 to S7 given in Chapter I, it contains the scheme S8, which will be introduced in no. 6, and the explicit axioms A1 (no. 3.) A2 (no. 5), A3 (§ 2, no. 1), A4 (§ 5, no. 1), and A5 (Chapter III, § 6, no. 1), These explicit axioms contain no letters; in other words, the theory of sets is a theory *without constants*.

Since the theory of sets is an equalitarian theory, the results of Chapter I are applicable.

¶ From now on, unless the contrary is expressly stated, we shall always argue in a theory which is stronger (Chapter I, § 2, no. 4) than the theory of sets; if the theory is not mentioned, it is to be assumed that the theory of sets is implied. It will be evident in many cases that this hypothesis is superfluous, and the reader should have no difficulty in determining in what theory weaker than the theory of sets the results stated are valid.

If $T$ and $U$ are terms, the assembly $\in TU$ is a relation (called the *relation of membership*) which in practice we write in one of the following ways : $T \in U$, $(T) \in (U)$, "$T$ belongs to $U$", "$T$ is an element of $U$". The relation "not $(T \in U)$" is written $T \notin U$.

From a "naive" point of view, many mathematical entities can be considered as collections or "sets" of objects. We do not seek to formalize this notion, and in the formalistic interpretation of what follows, the word "set" is to be considered as strictly synonymous with "term". In particular, phrases such as "let X be a set" are, in principle, quite superfluous, since every letter is a term. Such phrases are introduced only to assist the intuitive interpretation of the text.

### 2. INCLUSION

#### Definition 1 {#ens-ii-s1-def-1 .statement tag=03H5}

*The relation denoted by* $(\forall z)((z \in x) \Rightarrow (z \in y))$, *in which only the letters $x$ and $y$ appear, is written in one of the following ways :* $x \subset y$, $y \supset x$, *"$x$ is contained in $y$", "$y$ contains $x$", "$x$ is a subset of $y$". The relation* "not $(x \subset y)$" *is written* $x \not\subset y$ *or* $y \not\supset x$.

In accordance with the conventions mentioned in Chapter I, § 1, no. 1, this definition entails the following metamathematical convention. Let $T$ and $U$ be assemblies; if we substitute $T$ for $x$ and $U$ for $y$ in the assembly $x \subset y$, we obtain an assembly which is denoted by $T \subset U$; if we denote by $\mathbf{x}$, $\mathbf{y}$ letters which are distinct from $x$, $y$ and distinct from each other, and which appear neither in $T$ nor in $U$, the assembly $T \subset U$ is then identical with $(T|\mathbf{x})(U|\mathbf{y})(\mathbf{x}|x)(\mathbf{y}|y)(x \subset y,)$ and hence by CS8, CS9 (Chapter I, § 4, no. 1), and CS5 (Chapter I, § 1, no. 2) with $(\forall z)((z \in T) \Rightarrow (z \in U))$, provided that $z$ is a letter which appears neither in $T$ nor in $U$.

From now on, whenever we state a mathematical definition, we shall not mention the metamathematical convention which it entails.

CS12. *Let $T$, $U$, $V$ be assemblies and let $x$ be a letter. Then the assembly $(V|x)(T \subset U)$ is identical with $(V|x)T \subset (V|x)U$.*

This follows immediately from CS9 (Chapter I, § 4, no. 1) and CS5 (Chapter I, § 1, no. 2).

CF13. *If $T$ and $U$ are terms, $T \subset U$ is a relation.*

This follows immediately from CF8 (Chapter I, § 1, no. 4).

¶ Every relation of the form $T \subset U$ (where $T$ and $U$ are terms) is called an *inclusion relation*.

From now on we shall no longer write down explicitly the criteria of substitution and the formative criteria which should follow the definitions. It should be noted, however, that these criteria will often be used implicitly in proofs.

To prove the relation $x \subset y$ in a theory $\mathscr{T}$, it is enough, by C27 (Chapter I, § 4, no. 1), to prove that $z \in y$ in the theory obtained by adjoining $z \in x$ to the axioms of $\mathscr{T}$, where $z$ is a letter distinct from $x$, $y$ and the constants of the theory. In pratice we say "let $z$ be an element of $x$", and we attempt to prove $z \in y$.

#### Proposition 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x \subset x$.

Obvious.

#### Proposition 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x \subset y$ and $y \subset z) \Rightarrow (x \subset z)$.

Adjoin the hypotheses $x \subset y$, $y \subset z$, and $u \in x$. Then the relations

$$(u \in x) \Rightarrow (u \in y), \qquad (u \in y) \Rightarrow (u \in z),$$

are true, and therefore the relation $u \in z$ is true.

### 3. THE AXIOM OF EXTENT

The *axiom of extent* is the following axiom :

A1. $\qquad (\forall x)(\forall y)((x \subset y \text{ and } y \subset x) \Rightarrow (x = y))$.

Intuitively, this axiom expresses the fact that two sets which have the same elements are equal.

To prove that $x = y$ it is therefore enough to prove $z \in y$ in the theory obtained by adjoining the hypothesis $z \in x$, and $z \in x$ in the theory obtained by adjoining the hypothesis $z \in y$, where $z$ is a letter distinct from $x$, $y$, and the constants.

C48. *Let $\mathbf{R}$ be a relation, $x$ a letter, and $y$ a letter distinct from $x$ which does not appear in $\mathbf{R}$. Then the relation $(\forall x)((x \in y) \Leftrightarrow \mathbf{R})$ is single-valued in $y$.*

Let $z$ be a letter distinct from $x$ which does not appear in $\mathbf{R}$. Adjoin the hypotheses

$$(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\forall x)((x \in z) \Leftrightarrow \mathbf{R}).$$

Then we have successively the theorems

$$(\forall x)(((x \in y) \Leftrightarrow \mathbf{R}) \text{ and } ((x \in z) \Leftrightarrow \mathbf{R})),$$
$$(\forall x)((x \in y) \Leftrightarrow (x \in z)),$$
$$y \subset z, \qquad z \subset y.$$

By A1 we have then $y = z$. This proves C48.

### 4. COLLECTIVIZING RELATIONS

Let $\mathbf{R}$ be a relation and let $x$ be a letter. If $y$ and $y'$ denote letters distinct from $x$ *which do not appear in $\mathbf{R}$*, then the relations

$$(\exists y)(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\exists y')(\forall x)((x \in y') \Leftrightarrow \mathbf{R})$$

are identical by CS8 (Chapter I, §4, no. 1). The relation thus defined (which does not contain $x$) is denoted by $\operatorname{Coll}_xR$.

¶ If $\operatorname{Coll}_xR$ is a theorem in a theory $\mathscr{T}$, $R$ is said to be *collectivizing in $x$* in $\mathscr{T}$. When this is so, we may introduce an auxiliary constant $a$, distinct from $x$ and the constants of $\mathscr{T}$, and which does not appear in $R$, with the introductory axiom $(\forall x)((x \in a) \Longleftrightarrow R)$, or equivalently (if $x$ is not a constant of $\mathscr{T}$) $(x \in a) \Longleftrightarrow R$.

Intuitively, to say that $R$ is collectivizing in $x$ is to say that there exists a set $a$ such that the objects $x$ which possess the property $R$ are precisely the elements of $a$.

*Examples*

#### Example 1 {#ens-ii-s1-n4-exa-1 .statement tag=03RZ}

The relation $x \in y$ is clearly collectivizing in $x$.

#### Example 2 {#ens-ii-s1-n4-exa-2 .statement tag=03S0}

The relation $x \neq x$ *is not collectivizing in $x$*; in other words, (not $\operatorname{Coll}_x(x \neq x)$) is a theorem. Let us argue by contradiction and suppose that $x \neq x$ is collectivizing. Let $a$ be an auxiliary constant, distinct from $x$ and the constants of the theory, with the introductory axiom

$$
(\forall x)((x \neq x) \Longleftrightarrow (x \in a)).
$$

Then the relation

$$
(a \neq a) \Longleftrightarrow (a \in a)
$$

is true by C30 (Chapter I, §4, no. 3). The method of disjunction of cases (Chapter I, §3, no. 3) shows first that the relation $a \neq a$ is true, and then that the relation $a \in a$ is true, which is absurd.

**C49.** *Let $R$ be a relation and $x$ a letter. If $R$ is collectivizing in $x$, the relation $(\forall x)((x \in y) \Longleftrightarrow R)$, where $y$ is a letter distinct from $x$ which does not appear in $R$, is functional in $y$.*

This follows immediately from C48.

Very often in what follows we shall have at our disposal a theorem of the form $\operatorname{Coll}_xR$. To represent the term

$$
\tau_y(\forall x)((x \in y) \Longleftrightarrow R),
$$

which does not depend on the choice of the letter $y$ (distinct from $x$ and not appearing in $R$), we shall introduce a functional symbol $\mathcal{E}_x(R)$; the corresponding term does not contain $x$. This term is denoted by “the set of all $x$ such that $R$”. By definition (Chapter I, §4, no. 1) the relation

$$
(\forall x)((x \in \mathcal{E}_x(R)) \Longleftrightarrow R)
$$

is *identical* with $\mathrm{Coll}_x R$; consequently the relation $R$ is *equivalent* to

$$x \in \mathscr{E}_x(R).$$

C50. *Let $R$, $S$ be two relations and let $x$ be a letter. If $R$ and $S$ are collectivizing in $x$, the relation $(\forall x)(R \Rightarrow S)$ is equivalent to*

$$\mathscr{E}_x(R) \subset \mathscr{E}_x(S),$$

*and the relation $(\forall x)(R \Leftrightarrow S)$ is equivalent to $\mathscr{E}_x(R) = \mathscr{E}_x(S)$.*

This follows immediately from the preceding remark and from Definition 1 and axiom A1.

### 5. THE AXIOM OF THE SET OF TWO ELEMENTS

A2. $\qquad\qquad (\forall x)(\forall y)\ \mathrm{Coll}_z(z = x \text{ or } z = y).$

This axiom says that if $x$ and $y$ are objects, then there is a set whose only elements are $x$ and $y$.

#### Definition 2 {#ens-ii-s1-def-2 .statement tag=03H6}

*The set $\mathscr{E}_z (z = x \text{ or } z = y)$, whose only elements are $x$ and $y$, is denoted by $\{x, y\}$.*

The relation $z \in \{x, y\}$ is therefore equivalent to "$z = x$ or $z = y$"; it follows from C50 that $\{y, x\} = \{x, y\}$.

Let $R\{z\}$ be a relation and let $x, y$ be letters distinct from $z$. From the criteria C32, C33 (Chapter I, §4, no. 3), and C43 (Chapter I, §5, no. 1) it follows easily that the relation $(\exists z)((z \in \{x, y\})$ and $R\{z\})$ is equivalent to "$R\{x\}$ or $R\{y\}$"; consequently the relation $(\forall z)((z \in \{x, y\}) \Rightarrow R\{z\})$ is equivalent to "$R\{x\}$ and $R\{y\}$".

The set $\{x, x\}$, which is denoted simply by $\{x\}$, is called *the set whose only element is $x$*; the relation $z \in \{x\}$ is equivalent to $z = x$, and the relation $x \in \mathrm{X}$ is equivalent to $\{x\} \subset \mathrm{X}$.

### 6. THE SCHEME OF SELECTION AND UNION

The *scheme of selection and union* is the following :

S8. *Let $R$ be a relation, let $x$ and $y$ be distinct letters, and let $X$ and $Y$ be letters distinct from $x$ and $y$ which do not appear in $R$. Then the relation*

(1) $\quad (\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R))$ *is an axiom.*

Let us first show that this rule is indeed a scheme. Let $S$ denote the relation (1), and let us substitute a term $T$ for a letter $z$ in $S$; by CS8 (Chapter I, §4, no. 1) we may suppose that $x$, $y$, $X$, $Y$ are distinct from $z$ and do not appear in $T$. Then $(T|z)S$ is identical with

$$(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R')),$$

where $R'$ is $(T|z)R$.

Intuitively, the relation $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ means that for every object $y$ there exists a set $X$ (which may depend on $y$) such that the objects $x$ which are in the relation $R$ with the given object $y$ are elements of $X$ (but not necessarily the whole of $X$). The scheme of selection and union asserts that if this is the case and if $Y$ is any set, then there exists a set whose elements are precisely the objects $x$ which are in the relation $R$ with at least one object $y$ of the set $Y$.

C51. *Let $P$ be a relation, let $A$ be a set, and let $x$ be a letter which does not appear in $A$. Then the relation "$P$ and $x \in A$" is collectivizing in $x$.*

Let $R$ denote the relation "$P$ and $x = y$", where $y$ is a letter distinct from $x$ which appears neither in $P$ nor in $A$. The relation

$$(\forall x)(R \Rightarrow (x \in \{y\}))$$

is true by C27 (Chapter I, §4, no. 1). Let $X$ be a letter distinct from $x$ and $y$ which does not appear in $P$. The preceding relation is identical with $(\{y\}|X)((\forall x)(R \Rightarrow (x \in X)))$ (because $x$ is distinct from $y$), and therefore the relation $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ is true by virtue of S5 and C27 (Chapter I, §4, nos. 1 and 2). If follows from S8 and C30 (Chapter I, §4, no. 3) that the relation

$$(A|Y)\ \mathrm{Coll}x(\exists y)(y \in Y \text{ and } R)$$

(where $Y$ is a letter which does not appear in $R$) is true, and this relation is identical with $\mathrm{Coll}_x(\exists y)(y \in A \text{ and } R)$ (because neither $x$ nor $y$ appears in $A$). Finally, the relation "$y \in A$ and $R$" is equivalent to "$x = y$ and $x \in A$ and $P$" by C43 (Chapter I, §5, no. 1); since $x$ appears neither in $P$ nor in $A$, the relation

$$(\exists y)(x = y \text{ and } x \in A \text{ and } P)$$

is equivalent to "$((\exists y)(x = y))$ and $x \in A$ and $P$" by C33 (Chapter I, §4, no. 3) and therefore to "$P$ and $x \in A$" because $(\exists y)(x = y)$ is true.

¶ The set $\mathscr{E}_x(P$ and $x \in A)$ is called *the set of all $x \in A$ such that $P$* (\* thus we may speak of the set of all real numbers such that $P_*$).

C52. *Let $R$ be a relation, $A$ a set, and $x$ a letter which does not appear in $A$. If the relation $R \Rightarrow (x \in A)$ is a theorem, then $R$ is collectivizing in $x$.*

For $R$ is then equivalent to "$R$ and $x \in A$".

#### Remark {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

Let $R$ be a relation which is collectivizing in $x$, and let $S$ be a relation such that $(\forall x)(S \Rightarrow R)$ is a theorem. Then $S$ is collectivizing in $x$; for $R$ is equivalent to $x \in \mathscr{E}_x(R)$, so that

$$S \Rightarrow (x \in \mathscr{E}_x(R))$$

is a theorem, and the assertion follows from C52. Notice also that in this case we have $\mathscr{E}_X(S) \subset \mathscr{E}_X(R)$ by C50.

C53. *Let $T$ be a term, $A$ a set, $x$ and $y$ distinct letters. Suppose that $x$ does not appear in $A$ and that $y$ does not appear in $A$ nor in $T$. Then the relation $(\exists x)(y = T$ and $x \in A)$ is collectivizing in $y$.*

Let $R$ be the relation $y = T$. The relation $(\forall y)(R \Rightarrow (y \in \{T\}))$ is true, hence so is $(\forall x)(\exists X)(\forall y)(R \Rightarrow (y \in X))$, where $X$ is a letter, distinct from $y$, which does not appear in $R$. By virtue of S8, the relation $(\exists x)(x \in A$ and $R)$ is collectivizing in $y$, and C53 is proved.

¶ The relation $(\exists x)(y = T$ and $x \in A)$ is often read as follows : "$y$ can be put in the form $T$ for some $x$ belonging to $A$". The set

$$\mathscr{E}_y((\exists x)(y = T \text{ and } x \in A))$$

is generally called *the set of objects of the form $T$ for $x \in A$*. The assembly so denoted contains neither $x$ nor $y$, and does not depend on the choice of the letter $y$ satisfying the conditions of C53.

### 7. COMPLEMENT OF A SET. THE EMPTY SET

The relation $(x \notin \mathrm{A}$ and $x \in \mathrm{X})$ is collectivizing in $x$ by C51.

#### Definition 3 {#ens-ii-s1-def-3 .statement tag=03H8}

*Let* $\mathrm{A}$ *be a subset of a set* $\mathrm{X}$. *The set of elements of* $\mathrm{X}$ *which do not belong to* $\mathrm{A}$, *that is to say the set* $\mathscr{E}x$ $(x \notin \mathrm{A}$ *and* $x \in \mathrm{X})$, *is called the complement of* $\mathrm{A}$ *in* $\mathrm{X}$, *and is denoted by* $\complement_{\mathrm{X}}\mathrm{A}$ *or* $\mathrm{X} - \mathrm{A}$ (or by $\complement\mathrm{A}$ if there is no risk of confusion).

Let A be a subset of a set X; the relations "$x \in \mathrm{X}$ and $x \notin \mathrm{A}$" and $x \in \complement_{\mathrm{X}}\mathrm{A}$ are then equivalent. Consequently the relation "$x \in \mathrm{X}$ and $x \notin \complement_{\mathrm{X}}\mathrm{A}$" is equivalent to "$x \in \mathrm{X}$ and $(x \notin \mathrm{X}$ or $x \in \mathrm{A})$", hence to $x \in A$. In other words, $A = \complement_X(\complement_X A)$ is a true relation. Similarly, one shows that if B is a subset of X, the relations $A \subset B$ and $\complement_X B \subset \complement_X A$ are equivalent.

#### Theorem 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

*The relation* $(\forall x)(x \notin X)$ *is functional in* X.

For the relation $(\forall x)(x \notin X)$ implies $(\forall Y)(X \subset Y)$; by virtue of the axiom of extent, the relation $(\forall x)(x \notin X)$ is therefore single-valued in X. On the other hand, the relation $(\forall x)(x \notin \complement_Y Y)$ is true, which proves that $(\exists X)(\forall x)(x \notin X)$ is true.

¶ The term $\tau_x((\forall x)(x \notin X))$ corresponding to this functional relation is represented by the functional symbol $\emptyset$, and is called *the empty set* [^1]; the relation $(\forall x)(x \notin X)$, which is equivalent to $X = \emptyset$, is read as follows: "*the set* X *is empty*". We have the theorems $x \notin \emptyset$, $\emptyset \subset X$, $\complement_X X = \emptyset$, $\complement_X \emptyset = X$. The relation $X \subset \emptyset$ is equivalent to $X = \emptyset$. If $R\{x\}$ is a relation, the relation $(\forall x)((x \in \emptyset) \Rightarrow R\{x\})$ is true.

#### Remark {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

There exists no set of which every object is an element; in other words, "not $(\exists X)(\forall x)(x \in X)$" is a theorem. For if there were such a set, then by C52 every relation would be collectivizing. But we have seen (no. 4) that the relation $x \notin x$ is not collectivizing.

### Exercises {#ens-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: The term denoted by $\emptyset$ is therefore $\tau \neg \neg \in \tau \neg \neg \in \square\square\square$.
