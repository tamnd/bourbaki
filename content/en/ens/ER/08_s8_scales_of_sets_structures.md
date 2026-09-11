---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 8
section_title: Scales of sets. Structures
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 383-385
pdf_pages: 0388-0390
extraction: ocr
statements: 0
exercises: 0
content_sha256: 1729e7f56fb13a5cfb4b19ed30304bcfc4d735d7f99cdf7c9579aa41117e6f82
---

## 8. SCALES OF SETS. STRUCTURES

1. Given, for example, three *distinct* sets E, F, G, we may form other sets from them by taking their sets of subsets, or by forming the product of one of them by itself, or again by forming the product of two of them taken in a certain order. In this way we obtain *twelve* new sets. If we add these to the three original sets E, F, G, we may repeat the same operations on these fifteen sets, omitting those which give us sets already obtained; and so on. In general, any one of the sets obtained by this procedure (according to an explicit scheme) is said to belong to the *scale of sets* on E, F, G *as base*.

For example, let M, N, P be three sets of this scale, and let $R\{x,y,z\}$ be a *relation* between generic elements $x$, $y$, $z$ of M, N, P, respectively. Then R defines a subset of $M \times N \times P$, hence (via a canonical correspondence) a subset of $(M \times N) \times P$, i.e., an element of $\mathfrak{P}((M \times N) \times P)$. Thus to give a *relation* between elements of several sets in the same scale is the same as to give an *element* of another set in the scale. Likewise, to give a mapping of M into N, for example, amounts (by considering the graph of this mapping) to giving a subset of $M \times N$, i.e., an element of $\mathfrak{P}(M \times N)$, which is again a set in the scale. Finally, to give two elements (for example) of M amounts to giving a single element in the product set $M \times M$.

Thus being given a certain number of elements of sets in a scale, relations between generic elements of these sets, and mappings of subsets of certain of these sets into others, all comes down in the final analysis to being given a *single element* of one of the sets in the scale.

2. We said earlier (§6) that an element C of the set $\mathfrak{P}(E \times E)$ defines an order structure on E if it has the properties (a) $C \circ C \subset C$ and (b)

$$C \cap C^{-1} = \Delta.$$

In general, consider a set M in a scale of sets whose base consists, for the sake of example, of three sets E, F, G. Let us give ourselves a certain number of explicitly stated properties of a generic element of M, and let T be the intersection of the subsets of M defined by these properties. An element $\sigma$ of T is said to define a *structure* of the *species* T on E, F, G. The structures of species T are therefore characterized by the scheme of formation of M from E, F, G, and by the properties defining T, which are called the *axioms* of these structures. We give a specific name to all the structures of the same species. Every proposition which is a consequence of the proposition “$\sigma \in T$” (i.e., of the axioms defining T) is said to belong to the *theory* of the structures of species T; for example, the propositions stated in § 6 belong to the theory of structures of ordered sets.

In the last example, the axioms may be stated for a completely arbitrary base set E. Hence we give the same name to the structures which satisfy these axioms, independently of the set on which they are defined; and the propositions deduced from these axioms are valid in any set, because their formulation does not involve any special properties of the set E. Such remarks apply whenever the axioms are of this nature [^1].

Most often when a scale is used with a base consisting of several sets E, F, G, one of these sets, say E, plays a preponderant role in the structures under consideration. Therefore, by abuse of language, these structures are said to be defined in the set E, with F and G considered as auxiliary sets.

Finally, to simplify the language, a particular name is often given to a set which has been endowed with a structure of a definite species. Thus we speak of an *ordered set*, and in later parts of this series we shall define the notions of *group, ring, field, topological space, uniform space*, etc., all of which are words denoting sets endowed with certain structures.

3. Consider the structures of the same species T, where T is a subset of a set M in a scale of sets. If we adjoin new “axioms” to those which define T, the system of axioms thus obtained defines a subset U of M, contained in T. The structures of the species U are said to be *richer* than the structures of the species T. For example, the structures of *totally ordered* sets are richer than the structures of ordered sets, because the element C of $\mathfrak{P}(E \times E)$ which defines such a structure has to satisfy the additional axiom

$$C \cup \overline{C}^{-1} = E \times E.$$

4. Let M, M′ be two sets in the same scale, say with E, F, G as base. Let T be a subset of M and T′ a subset of M′, each defined by certain explicitly stated axioms. Whenever we can define explicitly a *one-to-one mapping* of T onto T′, we consider two elements $\sigma \in T$, $\sigma' \in T'$, which correspond to each other under this mapping, as defining the *same structure* on E, F, G; and the systems of axioms which define T and T′ are said to be *equivalent*.

The *topological structures* provide an example of this situation; they can be defined by means of several equivalent systems of axioms, two of which systems are particularly useful (see *General Topology*, Chapter I, § 1).

5. Let E, F, G be three sets, and suppose we are given *bijective* mappings of E, F, G onto three other sets E′, F′, G′, respectively. Since we know how to define the *canonical extensions* of bijective mappings to sets of subsets (§ 2, no. 9) and to product sets (§ 3, no. 14), we can define, step by step, the *extension* of the given bijections to two sets M, M′ constructed respectively according to the *same scheme* in the scale of sets based on E, F, G, and that based on E′, F′, G′. Let $f$ be the bijection of M onto M′ so obtained. If $\sigma$ is a structure on E, F, G which is an element of a subset T of M, we say that $f(\sigma)$ is the structure obtained by *transporting* the structure $\sigma$ onto E′, F′, G′ by means of the given bijections of E onto E′, F onto F′, G onto G′. Every proposition relating to the structure $\sigma$ on E, F, G gives rise (by use of appropriate extensions) to a proposition relating to the structure $f(\sigma)$ on E′, F′, G′.

Conversely, a structure $\sigma$ on E, F, G and a structure $\sigma'$ on E′, F′, G′ are said to be *isomorphic* if $\sigma'$ can be obtained by *transporting* $\sigma$ by means of bijections of E, F, G onto E′, F′, G′, respectively; these mappings are then said to constitute an *isomorphism* of $\sigma$ onto $\sigma'$.

When we are concerned with structures on a single set E, the bijection of E onto E′ which transports $\sigma$ into $\sigma'$ is also called an *isomorphism of the set E, endowed with the structure $\sigma$, onto the set E′, endowed with the structure $\sigma'$.*

This mapping is also called an *isomorphism* when F and G are two auxiliary sets, and the bijections for these two sets are the *identity* mappings of F and G onto themselves.

An *isomorphism* of a set E, endowed with a structure $\sigma$, onto itself is called an *automorphism*.

When there exists an *isomorphism* of a set E, endowed with a structure $\sigma$, onto a set E′, endowed with a structure $\sigma'$, it is often convenient to *identify* E with E′, i.e., to give *the same name* to an element of a set M in the scale based on E and to the element which is its image under the appropriate extension of $f$ to the set M.

6. Given a system of axioms defining a subset T of a set M in a scale of sets, we should make sure, before speaking of the structures which satisfy these axioms, that the set T is *not necessarily empty*; otherwise the axioms would be said to be *contradictory* or *inconsistent*.

7. It may happen that a system of axioms defining a structure on a set can be stated for an arbitrary set, but that when we consider two structures satisfying these axioms and defined on two distinct sets E, F, we find from the axioms that these structures (if they exist) are necessarily *isomorphic* (which implies in particular that E and F are *equipotent*). Then the theory of the structures satisfying these axioms is said to be *univalent*; otherwise they are said to be *multivalent*.

The theory of integers, the theory of real numbers, and classical Euclidean geometry are univalent theories; the theory of ordered sets, group theory, and topology are multivalent theories. The study of multivalent theories is the most striking feature which distinguishes modern mathematics from classical mathematics.

[^1]: The reader may have observed that the indications given here are left rather vague; they are not intended to be other than heuristic, and indeed it seems scarcely possible to state general and precise definitions for structures outside of the framework of formal mathematics (see Chapter IV).
