---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 4
section_title: Natural integers. Finite sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 166-171, 230-234
pdf_pages: 0172-0177, 0236-0240
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF INTEGERS
      page: 166
      pdf_page: 172
    - "no": 2
      title: INEQUALITIES BETWEEN INTEGERS
      page: 166
      pdf_page: 172
    - "no": 3
      title: THE PRINCIPLE OF INDUCTION
      page: 168
      pdf_page: 174
    - "no": 4
      title: FINITE SUBSETS OF ORDERED SETS
      page: 170
      pdf_page: 176
    - "no": 5
      title: PROPERTIES OF FINITE CHARACTER
      page: 170
      pdf_page: 176
statements: 15
exercises: 11
content_sha256: 4a072096ffffd9564c385dad351b447db76172ec442dedd3e07d9c5178c5b614
---

## 4. NATURAL INTEGERS. FINITE SETS

### 1. DEFINITION OF INTEGERS

#### Definition 1 {#ens-iii-s4-def-1 .statement tag=03R9}

*A cardinal $\alpha$ is said to be finite if $\alpha \ne \alpha + 1$. A finite cardinal is also called a natural integer (or simply an integer if there is no risk of confusion [^1]). A set $E$ is said to be finite if $\operatorname{Card}(E)$ is a finite cardinal; and $\operatorname{Card}(E)$ is then called the number of elements of $E$.*

A family (Chapter II, § 3, no. 4) is said to be *finite* if its index set is finite.

*When we say that the number of objects of a certain type is an integer $m$, we mean that these objects are elements of a finite set whose number of elements is $m$. A set whose number of elements is $m$ is also called a set of $m$ elements.*

#### Proposition 1 {#ens-iii-s4-prop-1 .statement tag=03RA}

*A cardinal $\alpha$ is finite if and only if $\alpha + 1$ is finite.*

For the relations $\alpha = \mathfrak{b}$ and $\alpha + 1 = \mathfrak{b} + 1$ between cardinals $\alpha$ and $\mathfrak{b}$ are equivalent (§ 3, no. 4, Proposition 8); the relations $\alpha \ne \alpha + 1$ and $\alpha + 1 \ne (\alpha + 1) + 1$ are therefore equivalent.

¶ It is clear that $0 \ne 1$; hence $0$ is an integer. It follows that $1$ and $2$ are integers. The cardinals $2 + 1$ and $(2 + 1) + 1$ are integers, denoted by $3$ and $4$, respectively.

### 2. INEQUALITIES BETWEEN INTEGERS

#### Proposition 2 {#ens-iii-s4-prop-2 .statement tag=03RB}

*Let $n$ be an integer. Then every cardinal $\alpha$ such that $\alpha \le n$ is an integer. If $n \ne 0$, there exists a unique integer $m$ such that $n = m + 1$, and the relation $\alpha < n$ is equivalent to $\alpha \le m$.*

If $\alpha \le n$, there exists a cardinal $\mathfrak{b}$ such that $n = \alpha + \mathfrak{b}$ (§ 3, no. 6, Proposition 13). Then $(\alpha + 1) + \mathfrak{b} = (\alpha + \mathfrak{b}) + 1 = n + 1$ (§ 3, no. 3, Proposition 5, Corollary); and since $n \ne n + 1$, we have

$$
(\alpha + 1) + \mathfrak{b} \ne \alpha + \mathfrak{b}.
$$

Hence $\alpha + 1 \ne \alpha$, which means that $\alpha$ is an integer. If $n \ne 0$, we have $n \ge 1$ (§ 3, no. 2), and therefore there exists a unique cardinal $m$ such that $n = m + 1$ (§ 3, no. 6, Proposition 13 and no. 4, Proposition 8). Since $m \leqslant n$, $m$ is an integer, from what has already been proved. Finally, if an integer $a$ is such that $a < n$, we have $n = a + b$, with $b \neq 0$ (§ 3, no. 6, Proposition 13); since $b$ is an integer, we have $b = c + 1$ and $n = m + 1 = (a + c) + 1$. It follows that $m = a + c$ (§ 3, no. 4, Proposition 8), hence $a \leqslant m$. Conversely, if $a \leqslant m$, we have

$$a \leqslant m + 1 = n;$$

and if $a = n = m + 1$, we would have $a > m$, contrary to hypothesis.

#### Corollary 1 {#ens-iii-s4-prop-2-cor-1 .statement tag=03RC}

*Every subset of a finite set is finite.*

#### Corollary 2 {#ens-iii-s4-prop-2-cor-2 .statement tag=03RD}

*If* X *is a subset of a finite set* E *and* X $\neq$ E, *then*

$$\mathrm{Card}\ (\mathrm{X})\ <\ \mathrm{Card}\ (\mathrm{E}).$$

For X is contained in the complement X$'$ of a subset of E consisting of a single element; we have $\mathrm{Card}\,(\mathrm{X}) \leqslant \mathrm{Card}\,(\mathrm{X}')$ and $\mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{X}') + 1$, hence (Proposition 2) $\mathrm{Card}\,(\mathrm{X}') < \mathrm{Card}\,(\mathrm{E})$ and *a fortiori* $\mathrm{Card}\,(\mathrm{X}) < \mathrm{Card}\,(\mathrm{E})$.

Definition 1 shows that, conversely, if E is a set such that

$$\mathrm{Card}\ (\mathrm{X}) < \mathrm{Card}\ (\mathrm{E})$$

for every subset X of E such that X $\neq$ E, then E is finite.

#### Corollary 3 {#ens-iii-s4-prop-2-cor-3 .statement tag=03RE}

*If* $f$ *is a mapping of a finite set* E *into a set* F, *then* $f(\mathrm{E})$ *is a finite subset of* F.

For $\mathrm{Card}\ (f(\mathrm{E})) \leqslant \mathrm{Card}\ (\mathrm{E})$ (§ 3, no. 2, Proposition 3).

#### Corollary 4 {#ens-iii-s4-prop-2-cor-4 .statement tag=03RF}

*Let* E *and* F *be two finite sets with the same number of elements, and let* $f$ *be a mapping of* E *into* F. *Then the following statements are equivalent :*

(a) $f$ *is an injection*;
(b) $f$ *is a surjection*;
(c) $f$ *is a bijection.*

It is enough to prove that (a) and (b) are equivalent. If $f$ is injective, then $\mathrm{Card}(f(\mathrm{E})) = \mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{F})$, whence $f(\mathrm{E}) = \mathrm{F}$ (Corollary 2). If $f$ is not injective, let $x$ and $x'$ be two elements of E such that $x \neq x'$ and $f(x) = f(x')$. Then, putting $\mathrm{E}' = \mathrm{E} - \{x\}$, we have $f(\mathrm{E}') = f(\mathrm{E})$, whence $\mathrm{Card}(f(\mathrm{E})) \leqslant \mathrm{Card}\,(\mathrm{E}') < \mathrm{Card}\,(\mathrm{E})$ by virtue of Corollary 2; but since $\mathrm{Card}\,(\mathrm{F}) = \mathrm{Card}\,(\mathrm{E})$, it follows that $f(\mathrm{E}) \neq \mathrm{F}$.

### 3. THE PRINCIPLE OF INDUCTION

C61 (Principle of Induction). *Let* $R\{n\}$ *be a relation in a theory* $\mathscr{T}$ *(where n is not a constant of* $\mathscr{T}$*).* *Suppose that the relation*

$$R\{0\} \quad \text{and} \quad (\forall n)((n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\})$$

*is a theorem in* $\mathscr{T}$. *Under these conditions the relation*

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

*is a theorem in* $\mathscr{T}$.

We shall argue by contradiction. Suppose that the relation

$$(\exists n)(n \text{ is an integer and } (\text{not } R\{n\}))$$

is true. Let $q$ be an integer such that "not $R\{q\}$" (method of the auxiliary constant; cf. Chapter I, § 3, no. 3 and § 4, no. 1). The integers $n$ for which "$n \leqslant q$ and (not $R\{n\}$)" form a well-ordered non-empty set (§ 3, no. 2, Remark), which therefore has a least element $s$. If $s = 0$, then "not $R\{0\}$", contrary to hypothesis. If $s > 0$, then $s = s' + 1$, where $s'$ is an integer such that $s' < s$ (no. 2, Proposition 2). By definition of $s$, we have $R\{s'\}$, but then the hypothesis implies that $R\{s\}$ is true, contrary to the definition of $s$.

In order to apply the principle of induction it is necessary in particular to prove the relation

$$(n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\}.$$

For this purpose the method of the auxiliary hypothesis (Chapter I, § 3, no. 3) is commonly used, and it is for this reason that the relation "$n$ is an integer and $R\{n\}$" (or even $R\{n\}$) is called the *inductive hypothesis*.

*Remark*. There are various criteria which are frequently used under the name of "principle of induction". They can all be easily deduced from C61, and we indicate here the most important of them :

(1) Let $S\{n\}$ be the relation

$$(\forall p)((n \text{ is an integer and } p \text{ is an integer and } p < n) \Rightarrow R\{p\})$$

and suppose that $S\{n\}$ *implies* $R\{n\}$. Then the relation

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

is true. For the relation $S\{0\}$ is true, and by hypothesis $S\{n\}$ implies $R\{n\}$; since the relation $m < n + 1$ is equivalent to $m \leqslant n$ (no. 2, Proposition 2), the relation $S\{n + 1\}$ is equivalent to "$S\{n\}$ and $R\{n\}$", consequently, $S\{n\}$ implies $S\{n + 1\}$. The criterion C61 therefore proves that the relation

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow S\{n\})$$

is true, and since $S\{n\}$ implies $R\{n\}$, the relation

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow R\{n\})$$

is true.

(2) Let $k$ be an integer and let $R\{n\}$ be a relation such that the relation

$$R\{k\} \text{ and } (\forall n)\ ((n \text{ is an integer} \geqslant k \text{ and } R\{n\}) \Rightarrow R\{n + 1\})$$

is true. Then the relation

$$(\forall n)\ ((n \text{ is an integer} \geqslant k) \Rightarrow R\{n\})$$

is true ("*induction starting at k*"). For let $S\{n\}$ be the relation

$$(n \geqslant k) \Rightarrow R\{n\}.$$

Then by the method of disjunction of cases we see that $S\{0\}$ is true. On the other hand, it is easily verified that the relation

$$(n \text{ is an integer and } S\{n\}) \Rightarrow S\{n + 1\}$$

is true. It follows from C61 that the relation

$$(n \text{ is an integer}) \Rightarrow S\{n\}$$

is true, which proves our assertion.

(3) Let $a$ and $b$ be two integers such that $a \leqslant b$, and let $R\{n\}$ be a relation such that

$$R\{a\} \text{ and } (\forall n)((n \text{ is an integer and } a \leqslant n < b \text{ and } R\{n\}) \Rightarrow R\{n + 1\}).$$

Then the relation

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow R\{n\})$$

is true. The proof is similar to that of the preceding case; we take $S\{n\}$ to be the relation "$(a \leqslant n < b) \Rightarrow R\{n\}$" ("*induction restricted to an interval*").

(4) Let $a$, $b$ be two integers such that $a \leqslant b$, and let $\mathrm{R}\{n\}$ be a relation such that

$\mathrm{R}\{b\}$ and $(\forall n)((n$ is an integer and $a \leqslant n < b$ and $\mathrm{R}\{n+1\}) \Rightarrow \mathrm{R}\{n\})$.

Then the relation

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow \mathrm{R}\{n\})$$

is true. For we have the relation

$(n$ is an integer and $a \leqslant n < b$ and (not $\mathrm{R}\{n\}$)) $\Rightarrow$ not $\mathrm{R}\{n+1\}$.

If for some $n$ such that $a \leqslant n \leqslant b$ we had (not $\mathrm{R}\{n\}$), it would follow from (3) that (not $\mathrm{R}\{b\}$), contrary to the hypothesis, whence the result (*"descending induction"*).

### 4. FINITE SUBSETS OF ORDERED SETS

#### Proposition 3 {#ens-iii-s4-prop-3 .statement tag=03L9}

*Let* E *be a right directed preordered set* (resp. *a lattice*, resp. *a totally ordered set*). *Then every non-empty finite subset of* E *is bounded above* (resp. *has a least upper bound and a greatest lower bound*, resp. *has a greatest element and a least element*).

The proof is by induction on the number $n$ of elements of the subset under consideration. The result is trivial for $n = 1$. Let X be a subset of $n + 1$ elements of E (with $n \geqslant 1$), and put $\mathrm{X} = \mathrm{Y} \cup \{x\}$, where Y has $n$ elements and is therefore not empty. The inductive hypothesis implies the existence of an upper bound (resp. least upper bound, resp. greatest element) $y$ of Y. Since E is right directed (resp. a lattice, resp. totally ordered), $\{x, y\}$ has an upper bound (resp. least upper bound, resp. greatest element) which is evidently an upper bound (resp. least upper bound, resp. greatest element) of X.

#### Corollary 1 {#ens-iii-s4-prop-3-cor-1 .statement tag=03LA}

*Every totally ordered finite set is well-ordered and has a greatest element.*

#### Corollary 2 {#ens-iii-s4-prop-3-cor-2 .statement tag=03LB}

*Every finite ordered set has a maximal element.*

For such a set is inductive by Corollary 1 (cf. § 2, no. 4, Theorem 2).

### 5. PROPERTIES OF FINITE CHARACTER

#### Definition 2 {#ens-iii-s4-def-2 .statement tag=03LC}

*Let* E *be a set. A set* $\mathfrak{S}$ *of subsets of* E *is said to be of finite character if the relation* $\mathrm{X} \in \mathfrak{S}$ *is equivalent to the relation "every finite subset of* X *belongs to* $\mathfrak{S}$".

A property $P\{X\}$ of a subset $X$ of a set $E$ is said to be *of finite character* if the set of subsets $X$ of $E$ for which $P\{X\}$ is true is of finite character.

*Examples*

#### Example 1 {#ens-iii-s4-n5-exa-1 .statement tag=03T9}

The set of totally ordered subsets of an ordered set $E$ is of finite character. Indeed, a subset $X$ of $E$ is totally ordered if and only if every subset of $X$ consisting of two elements is totally ordered.

#### Example 2 {#ens-iii-s4-n5-exa-2 .statement tag=03TA}

The set of all free subsets of a module is of finite character. The same is true of the set of all algebraically free subsets of an extension of a field.

#### Example 3 {#ens-iii-s4-n5-exa-3 .statement tag=03TB}

The set of submodules of a module $E$ is not of finite character, because a finite subset of a submodule of $E$ is not necessarily a submodule of $E$. $_*$

#### Theorem 1 {#ens-iii-s4-thm-1 .statement tag=03LD}

*Every set $\mathfrak{S}$ of subsets of a set $E$ which is of finite character has a maximal element (when ordered by inclusion).*

By Theorem 2 of § 2, no. 4 it is enough to show that $\mathfrak{S}$ is inductive. To do this we shall show that if $\mathfrak{G}$ is any subset of $\mathfrak{S}$ which is totally ordered by inclusion, the union $X$ of the sets of $\mathfrak{G}$ belongs to $\mathfrak{S}$ (§ 2, no. 4, Theorem 2, Corollary 2). Since $\mathfrak{S}$ is of finite character, it is enough to show that every finite subset $Y$ of $X$ belongs to $\mathfrak{S}$. Now, for each $y \in Y$, there exists a set $Z_y \in \mathfrak{G}$ such that $y \in Z_y$. Since the set of sets $Z_y$ $(y \in Y)$ is finite and totally ordered by inclusion, it has a greatest element $S$ (no. 4, Corollary 1 to Proposition 3); in other words, there exists a set $S \in \mathfrak{G}$ such that $Y \subset S$. But since $S \in \mathfrak{S}$ and since $Y$ is a finite subset of $S$, we have $Y \in \mathfrak{S}$ because $\mathfrak{S}$ is of finite character; this completes the proof.

### Exercises {#ens-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).

[^1]: The notion of “integer” will be generalized later, in Algebra, where we shall define the *rational integers* and the *algebraic integers*.
