---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 7
section_title: Powers. Countable sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 380-382
pdf_pages: 0385-0387
extraction: ocr
statements: 0
exercises: 0
content_sha256: 86ddec08acce4507f77a4f26c22ecf7fe435bb7014433e7736350957d8534e86
---

## 7. POWERS. COUNTABLE SETS

1. Two sets E, F are said to be *equipotent* if they can be put in one-to-one correspondence.
Two sets, each equipotent to a third, are themselves equipotent.
If E and F are equipotent, then $\mathfrak{P}(E)$ and $\mathfrak{P}(F)$ are equipotent.
If E and F, E′ and F′, E″ and F″ are respectively equipotent, then $E\times E'\times E''$ and $F\times F'\times F''$ are equipotent. This proposition extends to the product of any number of sets.

2. Let X and Y be two generic subsets of a set E. The relation “X and Y are equipotent” is an *equivalence relation* on $\mathfrak{P}(E)$. The equivalence class (with respect to this relation) to which X belongs is called the *power* [^1] of X, and the set of these classes (i.e., the quotient of $\mathfrak{P}(E)$ by the above relation) is called the *set of powers* of subsets of E.
If E and F are two distinct sets, the relation “X and Y are equipotent” between a subset X of E and a subset Y of F is expressed by saying that the power of X and the power of Y are *equivalent*. In this way we have a one-to-one correspondence between a subset of the set of powers of subsets of E and a subset of the set of powers of subsets of F.

3. Let E, F be any two sets, which may or may not be distinct, and let $\mathfrak{a}$ (resp. $\mathfrak{b}$) be an element of the set of powers of subsets of E (resp. F). Then $\mathfrak{a}$ is said to be *less than* $\mathfrak{b}$, or $\mathfrak{b}$ *greater than* $\mathfrak{a}$, if there exists a one-to-one mapping of a subset $X\subset E$ with power $\mathfrak{a}$ into a subset $Y\subset F$ with power $\mathfrak{b}$. If also $\mathfrak{a}$ and $\mathfrak{b}$ are not equivalent powers, than $\mathfrak{a}$ is said to be *strictly less than* $\mathfrak{b}$, or $\mathfrak{b}$ *strictly greater than* $\mathfrak{a}$.

If $\mathfrak{a}$ and $\mathfrak{b}$ are equivalent, then $\mathfrak{a}$ is both greater and less than $\mathfrak{b}$.

Conversely, it is a theorem that *if $\mathfrak{a}$ is both greater and less than $\mathfrak{b}$, then $\mathfrak{a}$ and $\mathfrak{b}$ are equivalent.* It follows in particular that the set of powers of subsets of a set E is *ordered* by the relation “$\mathfrak{a}$ is less than $\mathfrak{b}$”; whenever we speak of this set as an ordered set, it is always the ordering defined by this relation that we mean.

Furthermore, using Zorn’s lemma (and hence the axiom of choice), it is shown that *the set of powers of subsets of a set E is well-ordered.*

4. The power of a set E is *strictly less than* that of the set $\mathfrak{P}(E)$.

If $f$ is a mapping of a set E into a set F, then the power of the image $f(X)$ of any subset X of E is *less than* the power of X.

5. Let $(X_i)_{i\in I}$ be a family of subsets of a set E such that $X_i\cap X_k=\varnothing$ whenever $i\ne k$. Let $(Y_i)_{i\in I}$ be a family of subsets of a set F, indexed by the same set I and such that the power of $Y_i$ is *less than* that of $X_i$, for all $i\in I$. Then the power of the union $\bigcup_{i\in J}Y_i$ is *less than* that of $\bigcup_{i\in J}X_i$ for all subsets J of I.

If also $Y_i\cap Y_k=\varnothing$ whenever $i\ne k$, and if $X_i$ and $Y_i$ are *equipotent* for all $i\in I$, then $\bigcup_{i\in J}X_i$ is *equipotent* to $\bigcup_{i\in J}Y_i$.

In particular, if F and E are the same set, we see that the power of the union of a set of *pairwise disjoint* subsets of E depends only on the powers of these subsets; it is called the *sum* of these powers (thus this function is defined for a family $(\mathfrak{a}_i)$ of elements of the set of powers only if there exists a family $(X_i)$ of pairwise disjoint subsets of E such that $X_i$ has power $\mathfrak{a}_i$ for each index $i$).

If $(X_i)_{i\in I}$ and $(Y_i)_{i\in I}$ are families of subsets of E and F, respectively, indexed by the same set I such that $X_i$ and $Y_i$ are *equipotent* for all $i$, then the products $\prod_i X_i$ and $\prod_i Y_i$ are *equipotent*.

6. The set $\mathbf{N}$ of natural integers may be considered as the set of powers of *finite* subsets of an *infinite* set. The order relation “$x\leq y$” on $\mathbf{N}$ is just the relation ordering this set of powers, and the *sum* of two natural integers is a function identical with the sum of two powers as defined above.

7. A set is said to be *countable* if it is equivalent to a subset of the set $\mathbf{N}$ of natural integers. *Every finite set* is therefore countable; if it has $n$ elements, it is equipotent to the interval $[0,n-1]$ of the set $\mathbf{N}$. Every

## SUMMARY OF RESULTS

*countable infinite* set is equipotent to $\mathbf{N}$; in particular, every infinite subset of $\mathbf{N}$ has the same power as $\mathbf{N}$.

If $E$ is an *infinite* set, there exists a *partition* of $E$ into *countable infinite* sets; in particular, every infinite set has a power *greater than* that of $\mathbf{N}$.

If $E$ is an *infinite* set, the sets $E \times E$ and $E \times \mathbf{N}$ are both *equipotent* to $E$, and the set of *finite subsets* of $E$ is *equipotent* to $E$. In particular, $\mathbf{N} \times \mathbf{N}$ is a *countable infinite* set.

8. A *sequence of elements* of a set $E$ is by definition a family of elements of $E$, indexed by the set $\mathbf{N}$ or a subset of $\mathbf{N}$. A sequence whose index set is $\mathbf{N}$ is therefore written $(x_n)_{n\in\mathbf{N}}$, or more simply $(x_n)$ when there is no likelihood of confusion. If $n$ denotes a generic integer, $x_n$ is said to be the *general term* of the sequence, or the *nth term*. The latter terminology is also used when $n$ is replaced by a particular integer. The set of elements of a sequence is countable.

A sequence is said to be *infinite* or *finite* according as the index set is an infinite or finite subset of $\mathbf{N}$. The set of elements of a finite sequence is finite.

Every subfamily of a sequence is again a sequence, called a *subsequence* of the given sequence. Every subsequence of a finite sequence is a finite sequence.

A family of elements whose index set is $\mathbf{N} \times \mathbf{N}$, or a subset of $\mathbf{N} \times \mathbf{N}$, is called a *double sequence*. A double sequence indexed by $\mathbf{N} \times \mathbf{N}$ is written $(x_{m,n})$, or more simply $(x_{mn})$ if there is no risk of confusion. Similarly for sequences with more than two indices.

Two sequences $(x_n)$, $(y_n)$ are said to *differ only in the order of their terms* if there exists a permutation $f$ of the index set such that $y_n=x_{f(n)}$ for all $n$.

With any family of elements $(x_\iota)_{\iota\in I}$ whose index set $I$ is countably infinite we may associate an infinite sequence, as follows : there exists a bijection $n\to f(n)$ of $\mathbf{N}$ onto $I$; putting $y_n=x_{f(n)}$, the sequence $(y_n)$ is said to be obtained by *ranging the family* $(x_\iota)$ in the *order defined by $f$. Thus the sequences corresponding to two distinct bijections of $\mathbf{N}$ onto $I$ differ only in the order of their terms.

Operating in the same way when $I$ is *finite*, we obtain a *finite sequence* associated with the family $(x_\iota)$.

9. The union, intersection, and product of a family $(X_\iota)_{\iota\in I}$ of subsets of a set $E$ are said to be *countable* if $I$ is a *countable* set, *finite* if $I$ is finite.

If $I$ is *countable*, and if the power of $X_\iota$ is *less than* a given infinite power $\alpha$ for all $\iota\in I$, then the power of the union $\bigcup_\iota X_\iota$ is *less than* $\alpha$. If also at least one of the $X_\iota$ has power $\alpha$, then $\bigcup_\iota X_\iota$ has power $\alpha$. In particular, every countable union of sets of power $\alpha$ also has power $\alpha$; every countable union of countable sets is a countable set.

[^1]: In formalized set theory (cf. Chapter III, § 3) we define the notion of the *cardinal* of a set, which we also call (by abuse of language) the *power* of the set. This abuse of language does not, however, cause any confusion, because two subsets of a set have the same power (in the sense defined above) if and only if they have the same cardinal; likewise, the power of a subset A of a set E is less than the power of a subset B of a set F (no. 3) if and only if the cardinal of A is less than that of B; and finally, if the power of A is the sum (no. 5) of the powers of a family $(A_\iota)$ of subsets of E, then the cardinal of A is the sum of the cardinals of the $A_\iota$.
