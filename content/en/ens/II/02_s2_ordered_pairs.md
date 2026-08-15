---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 2
section_title: Ordered pairs
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 72-75, 123-124
pdf_pages: 0079-0082, 0130-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE ORDERED PAIR
      page: 72
      pdf_page: 79
    - "no": 2
      title: PRODUCT OF TWO SETS
      page: 74
      pdf_page: 81
statements: 4
exercises: 2
content_sha256: 39df2ab84c1a4cd7487506eb10473433071a3570142a04a0b8feb982b45bc203
---

## 2. ORDERED PAIRS

### 1. THE AXIOM OF THE ORDERED PAIR

As we have said in §1, no. 1, the sign $\supset$ is a substantific sign of weight 2 in the theory of sets. If T, U are terms, then $\supset$TU is a term, which in practice is denoted by (T, U). In this notation, the *axiom of the ordered pair* is the following :

A3. $(\forall x)(\forall x')(\forall y)(\forall y')(((x, y) = (x', y')) \Rightarrow (x = x' \quad \text{and} \quad y = y'))$.

Since the relation "$x = x'$ and $y = y'$" implies $(x, y) = (x', y')$ by C44 (Chapter I, § 5, no. 2), the relation $(x, y) = (x', y')$ is *equivalent* to "$x = x'$ and $y = y'$".

¶ The relation $(\exists x)(\exists y)(z=(x,y))$ is written “$z$ is an *ordered pair*”. If $z$ is an ordered pair, the relations

$$
(\exists y)(z=(x,y)),\qquad(\exists x)(z=(x,y))
$$

are functional with respect to $x$ and $y$ respectively; this is an immediate consequence of A3. The terms

$$
\tau_x((\exists y)(z=(x,y)))\qquad\text{and}\qquad\tau_y((\exists x)(z=(x,y)))
$$

are denoted by $\operatorname{pr}_1z$ and $\operatorname{pr}_2z$, respectively, and are called the *first coordinate* (or *first projection*) and the *second coordinate* (or *second projection*) of $z$. If $z$ is an ordered pair, the relation $(\exists y)(z=(x,y))$ is equivalent to $x=\operatorname{pr}_1z$, and the relation $(\exists x)(z=(x,y))$ to $y=\operatorname{pr}_2z$ (Chapter I, §5, no. 3).

¶ The relation $z=(x,y)$ is equivalent to “$z$ is an ordered pair, and $x=\operatorname{pr}_1z$ and $y=\operatorname{pr}_2z$”; for the latter relation is equivalent to

$$
(\exists x')(\exists y')(\exists x'')(\exists y'')(z=(x',y')\text{ and }z=(x,y'')\text{ and }z=(x'',y));
$$

by A3, “$z=(x',y')$ and $z=(x,y'')$ and $z=(x'',y)$” is equivalent to “$z=(x,y)$ and $x=x'$ and $x=x''$ and $y=y'$ and $y=y''$”; hence by C33 (Chapter I, §4, no. 3), “$z$ is an ordered pair, and $x=\operatorname{pr}_1z$ and $y=\operatorname{pr}_2z$” is equivalent to

$$
z=(x,y)\text{ and }(\exists x')(\exists y')(\exists x'')(\exists y'')(x=x'\text{ and }x=x''\text{ and }y=y'\text{ and }y=y''),
$$

which proves our assertion. Evidently we have

$$
\operatorname{pr}_1(x,y)=x,\qquad \operatorname{pr}_2(x,y)=y,
$$

and the relation $z=(\operatorname{pr}_1(z),\operatorname{pr}_2(z))$ is equivalent to “$z$ is an ordered pair”.

¶ Let $R\{x,y\}$ be a relation, where the letters $x$ and $y$ are distinct and appear in $R$. Let $z$ be a letter, distinct from $x$ and $y$, which does not appear in $R$. Let $S\{z\}$ denote the relation

$$
(\exists x)(\exists y)(z=(x,y)\text{ and }R\{x,y\});
$$

this is a relation which contains one letter fewer than $R$, and which is *equivalent* to “$z$ is an ordered pair and $R\{\operatorname{pr}_1z,\operatorname{pr}_2z\}$”, this follows from the fact that $z=(x,y)$ is equivalent to “$z$ is an ordered pair and $x=\operatorname{pr}_1z$ and $y=\operatorname{pr}_2z$”, and from criteria C33 (Chapter I, §4, no. 3)

and C47 (Chapter I, §5, no. 3). It follows immediately that $R\{x, y\}$ is equivalent to $S\{(x, y)\}$, and also to

$$(\exists z)(z = (x, y) \text{ and } S\{z\})$$

by C47.

This means that we may interpret a relation between the objects $x$ and $y$ as a property of the ordered pair formed by these objects.

### 2. PRODUCT OF TWO SETS

#### Theorem 1 {#ens-ii-s2-thm-1 .statement tag=03PC}

*The relation*

$$(\forall X)(\forall Y)(\exists Z)(\forall z)((z \in Z) \Leftrightarrow (\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y)$$

*is true. In other words, for all* X *and all* Y *the relation* "$z$ *is an ordered pair and* $\mathrm{pr}_1 z \in X$ *and* $\mathrm{pr}_2 z \in Y$" *is collectivizing in* $z$.

Let $A_y$ denote the set of all objects of the form $(x, y)$ for $x \in X$ (cf. §1, no. 6, criterion C53). Let R be the relation $z \in A_y$, which is equivalent to $(\exists x)(z = (x, y)$ and $x \in X)$. It is clear that the relation

$$(\forall y)(\exists A)(\forall z)(R \Rightarrow (z \in A))$$

is true, by virtue of S5 (Chapter I, §4, no. 2). It then follows from S8 that the relation $(\exists y)(y \in Y$ and R$)$ is collectivizing in $z$. But this relation is equivalent to $(\exists x)(\exists y)(y \in Y$ and $x \in X$ and $z = (x, y))$; hence the result.

#### Definition 1 {#ens-ii-s2-def-1 .statement tag=03PD}

*Given two sets* X *and* Y, *the set*

$$\mathcal{E}_z((\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y))$$

*is called the product of* X *and* Y *and is denoted by* X $\times$ Y.

The relation $z \in X \times Y$ is thus equivalent to "$z$ is an ordered pair and $\mathrm{pr}_1 z \in X$ and $\mathrm{pr}_2 z \in Y$". The sets X and Y are called the *first* and *second factors* of X $\times$ Y.

#### Proposition 1 {#ens-ii-s2-prop-1 .statement tag=03PE}

*If* A$'$, B$'$ *are non-empty sets, the relation* A$' \times$ B$' \subset$ A $\times$ B *is equivalent to* "A$' \subset$ A *and* B$' \subset$ B".

In the first place, the relation $z \in A' \times B'$ is equivalent to "$z$ is an ordered pair and $\mathrm{pr}_1 z \in A'$ and $\mathrm{pr}_2 z \in B'$"; therefore, without any restriction on A$'$ and B$'$, the relation "A$' \subset$ A and B$' \subset$ B" implies

$$A' \times B' \subset A \times B.$$

Conversely, let us first show that if $B' \neq \emptyset$ (without restriction on $A'$), the relation $A' \times B' \subset A \times B$ implies $A' \subset A$. Let $x$ be an element of $A'$; since $B' \neq \emptyset$, there is an object $y$ which is an element of $B'$; we have $(x, y) \in A' \times B'$, hence $(x, y) \in A \times B$, and consequently $x \in A$; thus $A' \subset A$. Similarly, if $A' \neq \emptyset$, the relation $A' \times B' \subset A \times B$ implies $B' \subset B$. Hence the result.

#### Proposition 2 {#ens-ii-s2-prop-2 .statement tag=03PF}

*Let* A *and* B *be two sets. The relation* $A \times B = \emptyset$ *is equivalent to* "$A = \emptyset$ *or* $B = \emptyset$".

For the relation $z \in A \times B$ implies $\mathrm{pr}_1 z \in A$ and $\mathrm{pr}_2 z \in B$; hence $A \neq \emptyset$ and $B \neq \emptyset$. Conversely, the relation "$x \in A$ and $y \in B$" implies $(x, y) \in A \times B$ and hence $A \times B \neq \emptyset$. In other words, the relation $A \times B \neq \emptyset$ is equivalent to "$A \neq \emptyset$ and $B \neq \emptyset$"; hence the result.

If A, B, C are sets, we write

$$(A \times B) \times C = A \times B \times C;$$

an element $((x, y), z)$ of $A \times B \times C$ is written $(x, y, z)$ and is called a *triple*. Again, if A, B, C, D are sets, we write

$$(A \times B \times C) \times D = A \times B \times C \times D;$$

and so on.

### Exercises {#ens-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
