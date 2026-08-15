---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 4
section_title: Union and intersection of a family of sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
pdf_pages: 0097-0108, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE UNION AND THE INTERSECTION OF A FAMILY OF SETS
      page: 0
      pdf_page: 97
    - "no": 2
      title: PROPERTIES OF UNION AND INTERSECTION
      page: 0
      pdf_page: 100
    - "no": 3
      title: IMAGES OF A UNION AND AN INTERSECTION
      page: 0
      pdf_page: 101
    - "no": 4
      title: COMPLEMENTS OF UNIONS AND INTERSECTIONS
      page: 0
      pdf_page: 103
    - "no": 5
      title: UNION AND INTERSECTION OF TWO SETS
      page: 0
      pdf_page: 103
    - "no": 6
      title: COVERINGS
      page: 0
      pdf_page: 105
    - "no": 7
      title: PARTITIONS
      page: 0
      pdf_page: 106
    - "no": 8
      title: SUM OF A FAMILY OF SETS
      page: 0
      pdf_page: 107
statements: 10
exercises: 8
content_sha256: 8e41d9364c862c0e6c822d7802196a688cbc939f7a4e22a5b18510eaa38a0b9a
---

## 4. UNION AND INTERSECTION OF A FAMILY OF SETS

### 1. DEFINITION OF THE UNION AND THE INTERSECTION OF A FAMILY OF SETS

Let X be a family (§3, no. 4) and I its index set. To help the intuitive interpretation of what follows, we shall refer to X as a *family of sets*. If $(\mathrm{X}, \mathrm{I}, \mathfrak{G})$ is a *family of subsets of a set* E (that is, a family whose target $\mathfrak{G}$ is such that the relation $\mathrm{Y} \in \mathfrak{G}$ implies $\mathrm{Y} \subset \mathrm{E}$), we shall denote the family by $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}(\mathrm{X}_\iota \in \mathfrak{G})$ or simply by $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ (§3, no. 6); by abuse of notation we shall denote any family of sets, which has I as its index set, by $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$.

¶ Since the relation $(\forall x)((\iota \in \mathrm{I}$ and $x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{X}_\iota))$ is true, it follows from S5 (Chapter I, §4, no 2.) that the relation

$$(\forall \iota)(\exists \mathrm{Z})(\forall x)((\iota \in \mathrm{I} \text{ and } x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{Z}))$$

is true. By virtue of the scheme S8 (§1, no. 6) the relation $(\exists \iota)(\iota \in \mathrm{I}$ and $x \in \mathrm{X}_\iota)$ is *collectivizing in $x$*.

#### Definition 1 {#ens-ii-s4-def-1 .statement tag=03I1}

*Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets* (resp. *a family of subsets of a set* E). *The set $\mathcal{E}_x((\exists \iota)(\iota \in \mathrm{I}$ and $x \in \mathrm{X}_\iota))$, that is to say, the set of all $x$*

*which belong to at least one set of the family $(X_l)_{l\in I}$, is called the union of the family, and is denoted by*
$$\bigcup_{l\in I}X_l,$$ [^1]

If $(X_l)_{l\in I}$ is a family of subsets of a set $E$, then its union is a subset of $E$; notice that it does not depend on $E$, nor on the target $\mathcal{G}$ of the mapping $l\to X_l$.

It is clear that if $I=\varnothing$, we have $\displaystyle\bigcup_{l\in I}X_l=\varnothing$, because the relation $(\exists l)(l\in I\text{ and }x\in X_l)$ is then false.

¶ Suppose now that $I\neq\varnothing$. If $\alpha$ is an element of $I$, the relation
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)) $$
implies $x\in X_\alpha$ and therefore, by virtue of C52 (§1, no. 6), this relation is *collectivizing in $x$.*

**Definition 2.** *Let $(X_l)_{l\in I}$ be a family of sets whose index set $I$ is not empty. The set $\mathcal{E}_x((\forall l)((l\in I)\Longrightarrow(x\in X_l)))$, that is to say, the set of all $x$ which belong to every set of the family $(X_l)_{l\in I}$, is called the intersection of the family and is denoted by*
$$\bigcap_{l\in I}X_l.$$

If $I=\varnothing$, the relation $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$ is not collectivizing in $x$; for it is a true relation and there exists no set $Y$ such that $x\in Y$ is a true relation, because $Y$ would then be the set of all objects (cf. §1, no. 7, Remark).

If $(X_l)_{l\in I}$ is a family of subsets of a set $E$ and if $I\neq\varnothing$, the relation “$x\in E$ and $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$” is equivalent to
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)); $$
consequently it is collectivizing in $x$, and the set of all $x$ which satisfy this relation is equal to $\displaystyle\bigcap_{l\in I}X_l$. If $I=\varnothing$, the relation “$x\in E$ and $(\forall l)((l\in I)\Longrightarrow(x\in X_l))$” is equivalent to $x\in E$; it is therefore collectivizing in $x$, and the set of all $x$ which satisfy this relation is $E$. Hence we may state the following definition :

**Definition 3.** *Let $(X_l)_{l\in I}$ be a family of subsets of a set $E$. The set*
$$\mathcal{E}_x\left(x\in E\text{ and }(\forall l)((l\in I)\Longrightarrow(x\in X_l))\right),$$

*in other words, the set of all $x$ which belong to* E *and to each of the sets* $X_\iota$, *is called the intersection of the family and is denoted by* $\bigcap\limits_{\iota \in I} X_\iota$.

Hence for a family $(X_\iota)_{\iota \in \emptyset}$ of subsets of E we have

$$\bigcap_{\iota \in \emptyset} X_\iota = E.$$

But for a family $(X_\iota)_{\iota \in I}$ of subsets of E whose index set is not empty, the intersection $\bigcap\limits_{\iota \in I} X_\iota$ depends neither on E nor on the target of $\iota \rightarrow X_\iota$; and this justifies the use of the same notation in Definitions 2 and 3.

**Proposition 1.** *Let* $(X_\iota)_{\iota \in I}$ *be a family of sets, and let $f$ be a mapping of a set* K *onto* I. *Then*

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota,$$

*and, if* $I \neq \emptyset$,

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

Let $x$ be an element of $\bigcap\limits_{\iota \in I} X_\iota$. There exists an index $\iota \in I$ such that $x \in X_\iota$. Since $f\langle K \rangle = I$, there exists an index $\varkappa \in K$ such that $\iota = f(\varkappa)$, whence $x \in X_{f(\varkappa)}$ and consequently

$$x \in \bigcup_{\varkappa \in K} X_{f(\varkappa)}.$$

Conversely, if $x \in \bigcup\limits_{\varkappa \in K} X_{f(\varkappa)}$, there exists $\varkappa \in K$ such that $x \in X_{f(\varkappa)}$, and therefore, since $f(\varkappa) \in I$, $x \in \bigcup\limits_{\iota \in I} X_\iota$. Hence

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota.$$

¶ Now suppose that $I \neq \emptyset$, and let $x$ be an element of $\bigcap\limits_{\iota \in I} X_\iota$. For each element $\varkappa$ of K we have $f(\varkappa) \in I$, hence $x \in X_{f(\varkappa)}$, and therefore

$$x \in \bigcap_{\varkappa \in K} X_{f(\varkappa)}.$$

Conversely, let $x$ be an element of $\bigcap\limits_{\varkappa \in K} X_{f(\varkappa)}$. If $\iota$ is any element of I, there exists an element $\varkappa$ of K such that $\iota = f(\varkappa)$, whence $x \in X_\iota$ and

consequently $x \in \bigcap_{\iota \in I} X_\iota$. Hence

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

For families of subsets of a given set, it is clear that the second part of Proposition 1 remains valid without the restriction $I \neq \emptyset$.

#### Corollary {#ens-ii-s4-n1-cor-1 .statement tag=03I2}

*Let* $(X_\iota)_{\iota \in I}$ *be a family of sets such that* $X_\iota = X_\varkappa$ *for each pair of indices* $(\iota, \varkappa)$. *Then for each* $\alpha \in I$ *we have*

$$\bigcup_{\iota \in I} X_\iota = X_\alpha, \qquad \textit{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} X_\iota = X_\alpha.$$

Apply Proposition 1 to the constant mapping $\iota \to \alpha$ of I onto $\{\alpha\}$.

#### Definition 4 {#ens-ii-s4-def-4 .statement tag=03I3}

*Let* $\mathfrak{F}$ *be a set of sets and let* $\Phi$ *be the family of sets defined by the identity mapping of* $\mathfrak{F}$. *The union of the sets of* $\Phi$ *and (if* $\mathfrak{F}$ *is not empty) the intersection of the sets of* $\Phi$ *are called, respectively, the* union *and the* intersection *of the sets of* $\mathfrak{F}$, *and are denoted by* $\bigcup_{X \in \mathfrak{F}} X$ *and* $\bigcap_{X \in \mathfrak{F}} X$.

If follows immediately from Proposition 1 that if $(X_\iota)_{\iota \in I}$ is a family of sets, then the union and (if $I \neq \emptyset$) the intersection of the family are respectively equal to the union and the intersection of the sets of the set of elements of this family.

### 2. PROPERTIES OF UNION AND INTERSECTION

If $(X_\iota)_{\iota \in I}$ and $(Y_\iota)_{\iota \in I}$ are families of sets having the same index set I, and if $Y_\iota \subset X_\iota$ for each $\iota \in I$, then it is clear that

$$\bigcup_{\iota \in I} Y_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} Y_\iota \subset \bigcap_{\iota \in I} X_\iota.$$

¶ Let $(X_\iota)_{\iota \in I}$ be a family of sets. If $J \subset I$, we have

$$\bigcup_{\iota \in J} X_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } J \neq \emptyset) \qquad \bigcap_{\iota \in J} X_\iota \supset \bigcap_{\iota \in I} X_\iota.$$

#### Proposition 2 {#ens-ii-s4-prop-2 .statement tag=03I4}

*Let* $(X_\iota)_{\iota \in I}$ *be a family of sets whose index set* I *is the union of a family* $(J_\lambda)_{\lambda \in L}$ *of sets. Then*

$$\bigcup_{\iota \in I} X_\iota = \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right),$$

*and* (*if* $L \neq \emptyset$ and $J_\lambda \neq \emptyset$ *for each* $\lambda \in L$)

$$\bigcap_{\iota \in I} X_\iota = \bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$$

("associativity" of union and intersection).

Let $x$ be an element of $\bigcup_{\iota \in I} X_\iota$. There exists an index $\iota \in I$ such that $x \in X_\iota$. Since I is the union of the family $(J_\lambda)_{\lambda \in L}$, there exists an index $\lambda \in L$ such that $\iota \in J_\lambda$, whence $x \in \bigcup_{\iota \in J_\lambda} X_\iota$, and consequently

$$x \in \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right).$$

Conversely, let $x$ be an element of this set. There exists an index $\lambda \in L$ such that $x \in \bigcup_{\iota \in J_\lambda} X_\iota$, hence there exists an index $\iota \in J_\lambda$ (and therefore $\iota \in I$) such that $x \in X_\iota$; it follows that

$$x \in \bigcup_{\iota \in I} X_\iota.$$

Now suppose that $L \neq \emptyset$ and $J_\lambda \neq \emptyset$ for each $\lambda \in L$. Then $I \neq \emptyset$. Let $x$ be an element of $\bigcap_{\iota \in I} X_\iota$. If $\lambda \in L$, we have $x \in X_\iota$ for each $\iota \in J_\lambda$ (since $J_\lambda \subset I$), whence $x \in \bigcap_{\iota \in J_\lambda} X_\iota$. Since the last inclusion is true for all $\lambda \in L$, $x$ belongs to $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$. Conversely, let $x$ be an element of this latter set, and let $\iota$ be any element of I. There exists $\lambda \in L$ such that $\iota \in J_\lambda$; since $x \in \bigcap_{\iota \in J_\lambda} X_\iota$, we have $x \in X_\iota$, which is true for all $\iota \in I$. Hence $x \in \bigcap_{\iota \in I} X_\iota$. This completes the proof.

For families of subsets of a given set the second part of Proposition 2 remains valid without restriction on L and $J_\lambda$.

### 3. IMAGES OF A UNION AND AN INTERSECTION

#### Proposition 3 {#ens-ii-s4-prop-3 .statement tag=03I5}

*Let* $(X_\iota)_{\iota \in I}$ *be a family of subsets of a set* A, *and let* $\Gamma$ *be a correspondence between* A *and* B. *Then*

$$\Gamma \left\langle \bigcup_{\iota \in I} X_\iota \right\rangle = \bigcup_{\iota \in I} \Gamma \langle X_\iota \rangle, \qquad \Gamma \left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma \langle X_\iota \rangle.$$

The relation $(\exists x)\left(x \in \bigcup_{\iota \in I} X_\iota \text{ and } y \in \Gamma(x)\right)$ is equivalent to

$$(\exists x)(\exists \iota)(\iota \in I \text{ and } x \in X_\iota \text{ and } y \in \Gamma(x)),$$

hence to $(\exists \iota)(\iota \in I$ and $y \in \Gamma\langle X_\iota \rangle)$, hence is equivalent to $y \in \bigcup_{\iota \in I} \Gamma\langle X_\iota \rangle$; this proves the first formula. As to the second formula, we have $\bigcap_{\iota \in I} X_\iota \subset X_\iota$ for all $\iota \in I$, whence (§3, Proposition 2)

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \Gamma\langle X_\iota \rangle,$$

and consequently

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle.$$

¶ If $\Gamma$ is an arbitrary correspondence (and in particular an arbitrary function), the formula

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle$$

is usually *false*.

* For example, in the plane $\mathbf{R}^2$ the first projections of the lines $y = x$ and $y = x + 1$ are equal to $\mathbf{R}$, but the intersection of these lines is empty, and therefore so is the first projection of this intersection [^2]. *

However, we have the following important result :

#### Proposition 4 {#ens-ii-s4-prop-4 .statement tag=03I6}

*Let $f$ be a mapping of* A *into* B *and let* $(Y_\iota)_{\iota \in I}$ *be a family of subsets of* B. *Then* $\overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle = \bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle.$

To prove this, let $x$ be an element of $\bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle$. We have $f(x) \in Y_\iota$ for all $\iota \in I$, whence $f(x) \in \bigcap_{\iota \in I} Y_\iota$, and consequently

$$x \in \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle.$$

Therefore $\bigcap_{\iota \in I} \overset{-1}{f}(Y_\iota) \subset \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle$; this relation, together with Proposition 3, gives the result.

#### Corollary {#ens-ii-s4-n3-cor-1 .statement tag=03I7}

*If $f$ is an injection of* A *into* B *and if* $(X_\iota)_{\iota \in I}$ *is a family of subsets of* A *whose index set* I *is not empty, then* $f\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} f\langle X_\iota \rangle$.

For we may write $f = i \circ g$, where $i$ is the canonical injection of $f\langle A \rangle$ into B and $g$ is a bijection of A onto $f\langle A \rangle$. If $h$ denotes the inverse mapping of $g$, we have $f\langle X \rangle = \overset{-1}{h}\langle X \rangle$ for every subset X of A, and we are therefore brought back to Proposition 4.

### 4. COMPLEMENTS OF UNIONS AND INTERSECTIONS

#### Proposition 5 {#ens-ii-s4-prop-5 .statement tag=03I8}

*For every family* $(X_\iota)_{\iota \in I}$ *of subsets of a set* E, *we have*

$$\complement_E\left(\bigcup_{\iota \in I} X_\iota\right) = \bigcap_{\iota \in I} (\complement_E X_\iota), \qquad \complement_E\left(\bigcap_{\iota \in I} X_\iota\right) = \bigcup_{\iota \in I} (\complement_E X_\iota).$$

Let $x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right)$. Then $x \in E$ and, for every $\iota \in I$, $x \notin X_\iota$, so that $x \in \complement_E X_\iota$; consequently

$$x \in \bigcap_{\iota \in I} (\complement_E X_\iota).$$

Conversely, let $x$ be an element of $\bigcap_{\iota \in I} (\complement_E X_\iota)$; by the definition of intersection we have $x \in E$. Furthermore, if we had $x \in \bigcup_{\iota \in I} X_\iota$, there would exist an index $\varkappa \in I$ such that $x \in X_\varkappa$, which contradicts the hypothesi $x \in \bigcap_{\iota \in I} (\complement_E X_\iota)$; hence

$$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right).$$

This proves the first formula; the second one is an immediate consequence, in view of the relation $\complement_E(\complement_E X) = X$ for every subset X of E.

### 5. UNION AND INTERSECTION OF TWO SETS

If A, B are sets, we write

$$A \cup B = \bigcup_{X \in \{A, B\}} X, \qquad A \cap B = \bigcap_{X \in \{A, B\}} X.$$

It is clear that $A \cup B$ is the set of all objects which belong either to $A$ or to $B$ (or possibly to both), while $A \cap B$ is the set of all objects which belong to both $A$ and $B$. In particular, $\{x, y\} = \{x\} \cup \{y\}$.

¶ Let $\{x, y, z\} = \{x, y\} \cup \{z\}$. The set $\{x, y, z\}$ is the set whose only elements are $x$, $y$, and $z$. Similarly we write

$$\{x, y, z, t\} = \{x, y, z\} \cup \{t\},$$

and so on.

¶ If now $A$, $B$, $C$, $D$ are sets, we write

$$A \cup B \cup C = \bigcup_{X \in \{A,\, B,\, C\}} X, \qquad A \cap B \cap C = \bigcap_{X \in \{A,\, B,\, C\}} X;$$

$$A \cup B \cup C \cup D = \bigcup_{X \in \{A,\, B,\, C,\, D\}} X, \qquad A \cap B \cap C \cap D = \bigcap_{X \in \{A,\, B,\, C,\, D\}} X;$$

and so on.

¶ Let $A, B, C$ be sets. From Propositions 1 and 2 we deduce the formulae

$$A \cup B = B \cup A, \qquad A \cap B = B \cap A,$$
$$A \cup (B \cup C) = (A \cup B) \cup C = A \cup B \cup C,$$
$$A \cap (B \cap C) = (A \cap B) \cap C = A \cap B \cap C.$$

These formulae are also immediate consequences of the theorems enunciated in the criterion C24 (Chapter I, §3, no. 5). Similarly one proves the formulae

$$A \cup (B \cap C) = (A \cup B) \cap (A \cup C), \qquad A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$$

("distributivity" of union over intersection and of intersection over union; cf. §5, no. 6).

¶ The relation $A \subset B$ is equivalent to $A \cup B = B$ and to $A \cap B = A$. If $A$ and $B$ are subsets of a set $E$, we deduce from Proposition 5 (or from criterion C24) the formulae

$$\complement_E(A \cup B) = (\complement_E A) \cap (\complement_E B), \qquad \complement_E(A \cap B) = (\complement_E A) \cup (\complement_E B);$$

furthermore, we have

$$A \cup (\complement_E A) = E, \qquad A \cap (\complement_E A) = \emptyset.$$

¶ If $\Gamma$ is a correspondence between $E$ and $F$, and if $A$, $B$ are subsets of $E$, it follows from Proposition 3 that

$$\Gamma\langle A \cup B \rangle = \Gamma\langle A \rangle \cup \Gamma\langle B \rangle, \qquad \Gamma\langle A \cap B \rangle \subset \Gamma\langle A \rangle \cap \Gamma\langle B \rangle,$$

and that, if $f$ is a mapping of F into E,

$$\overset{-1}{f}\langle \mathrm{A} \cap \mathrm{B} \rangle = \overset{-1}{f}\langle \mathrm{A} \rangle \cap \overset{-1}{f}\langle \mathrm{B} \rangle$$

from Proposition 4.

¶ We record also the following Proposition on complements :

**Proposition 6.** *Let $f$ be a mapping of* A *into* B. *For every subset* Y *of* B, *we have*

$$\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle = \overset{-1}{f}\langle \mathrm{B} \rangle - \overset{-1}{f}\langle \mathrm{Y} \rangle.$$

For $x$ belongs to $\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle$ if and only if $f(x)$ belongs to B but not to Y, i.e., if and only if $x$ belongs to $\overset{-1}{f}\ \langle \mathrm{B} \rangle$ but not to $\overset{-1}{f}\ \langle \mathrm{Y} \rangle$.

**Corollary.** *Let $f$ be an injection of* A *into* B. *For every subset* X *of* A, *we have $f\langle \mathrm{A} - \mathrm{X} \rangle = f\langle \mathrm{A} \rangle - f\langle \mathrm{X} \rangle$.*

Writing $f = i \circ g$, where $i$ is the canonical injection of $f\langle \mathrm{A} \rangle$ into B, we reduce the Corollary to Proposition 6 applied to $\overset{-1}{g}$.

¶ The intersection $\mathrm{X} \cap \mathrm{A}$ is sometimes called the *trace* of X on A. If $\mathfrak{F}$ is a family of sets, the set of traces on A of the sets belonging to $\mathfrak{F}$ is called the *trace* of $\mathfrak{F}$ on A.

### 6. COVERINGS

**Definition 5.** *A family of sets $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is said to be a covering of a set* E *(or to cover* E) *if $\mathrm{E} \subset \bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. If $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ and $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ are coverings of* E, *the second of these coverings is said to be finer than the first (or to be a refinement of the first, or to refine the first) if, for each $\varkappa \in \mathrm{K}$, there exists $\iota \in \mathrm{I}$ such that*

$$\mathrm{Y}_\varkappa \subset \mathrm{X}_\iota.$$

A set of sets $\mathfrak{R}$ is a covering of E if the family of sets defined by the identity mapping of $\mathfrak{R}$ is a covering of E, in other words, if $\mathrm{E} \subset \bigcup\limits_{\mathrm{X} \in \mathfrak{R}} \mathrm{X}$.

If $\mathfrak{R}$, $\mathfrak{R}'$, $\mathfrak{R}''$ are three coverings of E such that $\mathfrak{R}'$ refines $\mathfrak{R}$ and $\mathfrak{R}''$ refines $\mathfrak{R}'$, it is clear that $\mathfrak{R}''$ refines $\mathfrak{R}$.

Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ be a covering of E. If J is a subset of I such that $(\mathrm{X}_\iota)_{\iota \in \mathrm{J}}$ is still a covering of E, then this covering clearly refines $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$.

¶ Let $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ and $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ be coverings of a set E. Then the family of sets $(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ is a covering of E. For if $x \in \mathrm{E}$, there exist indices $\iota \in \mathrm{I}$ and $\varkappa \in \mathrm{K}$ such that $x \in \mathrm{X}_\iota$ and $x \in \mathrm{Y}_\varkappa$, so that $x \in \mathrm{X}_\iota \cap \mathrm{Y}_\varkappa$ Moreover, it is clear that the covering $(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$ refines each o

the coverings $(X_\iota)_{\iota \in I}$, $(Y_\varkappa)_{\varkappa \in K}$. Conversely, let $(Z_\lambda)_{\lambda \in L}$ be a covering of E which refines each of the coverings $(X_\iota)_{\iota \in I}$, $(Y_\varkappa)_{\varkappa \in K}$; if $\lambda \in L$, then there exist indices $\iota \in I$ and $\varkappa \in K$ such that $Z_\lambda \subset X_\iota$ and $Z_\lambda \subset Y_\varkappa$, so that $Z_\lambda \subset X_\iota \cap Y_\varkappa$; hence the covering $(Z_\lambda)_{\lambda \in L}$ is a refinement of

$$(X_\iota \cap Y_\varkappa)_{(\iota, \varkappa) \in I \times K}.$$

¶ Let $(X_\iota)_{\iota \in I}$ be a covering of a set A, and let $f$ be a mapping of A *onto* a set B. The family $(f\langle X_\iota \rangle)_{\iota \in I}$ is then a covering of B (Proposition 3), called the *image under* $f$ *of the covering* $(X_\iota)_{\iota \in I}$. If $g$ is a mapping of a set C into the set A, the family $(\overset{-1}{g}\langle X_\iota \rangle)_{\iota \in I}$ is a covering of C, called the *inverse image under* $g$ *of the covering* $(X_\iota)_{\iota \in I}$.
¶ Let E and F be sets, let $(X_\iota)_{\iota \in I}$ be a covering of E, and let $(Y_\varkappa)_{\varkappa \in K}$ be a covering of F. The family $(X_\iota \times Y_\varkappa)_{(\iota, \varkappa) \in I \times K}$ is then a covering of $E \times F$, called the *product* of the coverings $(X_\iota)_{\iota \in I}$ of E and $(Y_\varkappa)_{\varkappa \in K}$ of F.

**Proposition 7.** (1) *Let* E *be a set and* $(X_\iota)_{\iota \in I}$ *a covering of* E. *If* $f$ *and* $g$ *are two functions with domain* E *such that* $f$ *and* $g$ *agree on* $E \cap X_\iota$ *for each* $\iota \in I$, *then* $f$ *and* $g$ *agree on* E.

(2) *Let* $(X_\iota)_{\iota \in I}$ *be a family of sets and let* $(f_\iota)_{\iota \in I}$ *be a family of mappings with the same target* F *such that for each* $\iota \in I$ *the domain of* $f_\iota$ *is* $X_\iota$, *and for each pair* $(\iota, \varkappa) \in I \times I$, $f_\iota$ *and* $f_\varkappa$ *agree on* $X_\iota \cap X_\varkappa$. *Then there is exactly one function* $f$ *with domain* $A = \bigcup_{\iota \in I} X_\iota$ *and target* F *which extends each of the functions* $f_\iota$ $(i \in I)$.

(1) Let $x$ be any element of E. Then there exists $\iota \in I$ such that $x \in X_\iota$, whence $f(x) = g(x)$ by hypothesis.
(2) Let $G_\iota$ be the graph of $f_\iota$ and let $G = \bigcup_{\iota \in I} G_\iota$; let us show that G is a functional graph. If $(x, y) \in G$ and $(x, y') \in G$, there exist two indices $\iota$, $\varkappa$ in I such that $(x, y) \in G_\iota$ and $(x, y') \in G_\varkappa$. This implies $x \in X_\iota$, $x \in X_\varkappa$, $y = f_\iota(x)$, $y' = f_\varkappa(x)$; but since $x \in X_\iota \cap X_\varkappa$, we have

$$f_\iota(x) = f_\varkappa(x),$$

that is to say, $y = y'$. The graph G has domain $\mathrm{pr}_1 G = \bigcup_{\iota \in I} \mathrm{pr}_1 G_\iota = A$; the function $f = (G, A, F)$ therefore satisfies the required conditions. Its uniqueness follows from the first part of the Proposition.

### 7. PARTITIONS

**Definition 6.** *Two sets* A *and* B *are said to be disjoint* (*or not to intersect*) *if* $A \cap B = \emptyset$. *If* $A \cap B \neq \emptyset$, *we say that* A *meets* (*or intersects*) B. *Let*

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *be a family of sets. The sets of this family are said to be mutually disjoint if the conditions* $\iota \in \mathrm{I}$, $\varkappa \in \mathrm{I}$, $\iota \neq \varkappa$ *imply* $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$.

Let $f$ be a mapping of A into B, and let $(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ be a family of mutually disjoint subsets of B. Proposition 4 then shows that the sets of the family $(\overset{-1}{f}\langle \mathrm{Y}_\iota \rangle)_{\iota \in \mathrm{I}}$ of subsets of A are mutually disjoint. On the other hand, if $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is a family of mutually disjoint subsets of A, the sets of the family $(f \langle \mathrm{X}_\iota \rangle)_{\iota \in \mathrm{I}}$ are not in general mutually disjoint.

**Proposition 8.** *Let* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *be a family of mutually disjoint sets, and let* $(f_\iota)_{\iota \in \mathrm{I}}$ *be a family of functions with the same target* F *such that the domain of* $f_\iota$ *is* $\mathrm{X}_\iota$ *for each* $\iota \in \mathrm{I}$. *Then there exists exactly one function f with domain* $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ *and target* F *which extends each of the functions* $f_\iota$ $(\iota \in \mathrm{I})$.

This is a corollary of Proposition 7, since $f_\iota$ and $f_\varkappa$ clearly agree on $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$ whenever $\iota \neq \varkappa$.

**Definition 7.** *A partition of a set* E *is a family of* non-empty *mutually disjoint subsets of* E *which covers* E.

#### Example {#ens-ii-s4-n7-exa-1 .statement tag=03I9}

For every non-empty set A, the family $(\{x\})_{x \in \mathrm{A}}$ is a partition of A.

If $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is a partition of a set E, the mapping $\iota \rightarrow \mathrm{X}_\iota$ of I onto the set $\mathfrak{F}$ of elements $\mathrm{X}_\iota$ of the partition is bijective. Hence, if $\mathfrak{F}$ is given, the partition is determined up to a one-to-one correspondence between index sets. Usually when we speak of a partition, it is the set of elements of the partition with which we are concerned.

### 8. SUM OF A FAMILY OF SETS

**Proposition 9.** *Let* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *be a family of sets. Then there exists a set* X *with the following property* : X *is the union of a family* $(\mathrm{X}'_\iota)_{\iota \in \mathrm{I}}$ *of mutually disjoint sets such that for each* $\iota \in \mathrm{I}$ *there exists a one-to-one mapping of* $\mathrm{X}_\iota$ *onto* $\mathrm{X}'_\iota$.

Let $\mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$. If $\iota \in \mathrm{I}$, the mapping $x \rightarrow (x, \iota)$ $(x \in \mathrm{X}_\iota)$ is a one-to-one mapping of $\mathrm{X}_\iota$ onto a subset $\mathrm{X}'_\iota$ of $\mathrm{A} \times \mathrm{I}$. Moreover, the image of $\mathrm{X}'_\iota$ under the second coordinate function on $\mathrm{A} \times \mathrm{I}$ is contained in the set $\{\iota\}$; it follows that $\mathrm{X}'_\iota \cap \mathrm{X}'_\varkappa = \emptyset$ whenever $\iota \neq \varkappa$. We may then take $\mathrm{X} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}'_\iota$.

**Definition 8.** *Let* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *be a family of sets. The sum of this family is the union of the family of sets* $(\mathrm{X}_\iota \times \{\iota\})_{\iota \in \mathrm{I}}$.

#### Proposition 10 {#ens-ii-s4-prop-10 .statement tag=03IA}

*Let* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *be a family of mutually disjoint sets. Let* A *be its union and* S *its sum. Then there exists a bijective mapping of* A *onto* S.

For each $\iota \in \mathrm{I}$, let $f_\iota$ be a bijection of $\mathrm{X}_\iota$ onto $\mathrm{X}_\iota \times \{\iota\}$. By virtue of Proposition 8, there exists a mapping $f$ of A into S which extends all the mappings $f_\iota$. It is immediately verified that $f$ is a bijective mapping of A onto S.

By abuse of language, a set E is said to be the *sum* of a family of sets $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ if there exists a bijection of E onto the sum of the family, as defined in Definition 8.

Note that if $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ is an arbitrary family of sets, the argument of Proposition 10 shows that there exists a mapping of the sum S *onto* the union A.

### Exercises {#ens-ii-s4-exercises}

if and only if

$$
G \circ G^{-1} \circ G = \varnothing.
$$

7. A graph $G$ is functional if and only if for each set $X$ we have

$$
G^{-1}(G(X)) \subset X.
$$

8. Let $A$, $B$ be two sets, let $\Gamma$ be a correspondence between $A$ and $B$, and let $\Gamma'$ be a correspondence between $B$ and $A$. Show that if $\Gamma'(\Gamma(x))=\{x\}$ for all $x\in A$ and if $\Gamma(\Gamma'(y))=\{y\}$ for all $y\in B$, then $\Gamma'$ is a bijection of $A$ onto $B$, and $\Gamma'$ is the inverse mapping.

9. Let $A$, $B$, $C$, $D$ be sets, $f$ a mapping of $A$ into $B$, $g$ a mapping of $B$ into $C$, $h$ a mapping of $C$ into $D$. If $g\circ f$ and $h\circ g$ are bijections, show that all of $f$, $g$, $h$ are bijections.

10. Let $A$, $B$, $C$ be sets, $f$ a mapping of $A$ into $B$, $g$ a mapping of $B$ into $C$, $h$ a mapping of $C$ into $A$. Show that if two of the three mappings $h\circ g\circ f$, $g\circ f\circ h$, $f\circ h\circ g$ are surjections and the third is an injection, then $f$, $g$, $h$ are all bijections.

*11. Find the error in the following argument : Let $\mathbf{N}$ denote the set of natural numbers and let $A$ denote the set of all integers $n>2$ for which there exist three strictly positive integers $x$, $y$, $z$ such that $x^n+y^n=z^n$. Then the set $A$ is not empty (in other words, “Fermat’s last theorem” is false). For let $B=\{A\}$ and $C=\{\mathbf{N}\}$; $B$ and $C$ are sets consisting of a single element, hence there is a bijection $f$ of $B$ onto $C$. We have $f(A)=\mathbf{N}$; if $A$ were empty we should have $\mathbf{N}=f(\varnothing)=\varnothing$, which is absurd. *

See the [exercises for § 4](exercises/s4/).

[^1]: The scheme S8 therefore allows us to define the union of a family of sets without supposing *a priori* that these sets are subsets of the same set (which is the assumption made in the definition of union given in *Summary of Results*, §4, no. 2).
[^2]: (*) A celebrated error arising from the application of this formula is that committed by H. Lebesgue in his attempt to prove that the projection on an axis of a Borel set in the plane is again a Borel set (this statement was subsequently shown to be incorrect, and the discussion it provoked was the origin of the theory of "Souslin" sets) : Lebesgue asserted that the projection of the intersection of a decreasing sequence of sets is equal to the intersection of their projections (*Journal de Mathématiques*, (6) **1** (1905), pp. 191-192).
