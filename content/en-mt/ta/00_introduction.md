---
book: ta
book_title: Topologie algébrique
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: en
source: ta-i-iv-fr
pdf_pages: 0012-0015
extraction: native
statements: 0
exercises: 0
content_sha256: 31e78ed45d903524fc86eeb328fdbc7d9c35f20770c3034329ffe419c950e653
translated_from: content/fr/ta/00_introduction.md
source_lang: fr
translation_method: machine
source_content_sha256: bac57c1565b556784f0c497ef2fe5450c8af0eb67cb4ae628bbae4dc7752d614
translation_model: gpt-5.4
translation_run: translate-en-mt-edca99c5
glossary_version: 34
glossary_terms_sha256: 4146d4b8ed689218f8ac134cf963f30c0ea6805c27f02a0a608680a97616541a
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## INTRODUCTION

Algebraic Topology aims at studying topological spaces by associating with them functorially various algebraic structures (modules, groupoids, etc.) whose properties reflect those of the spaces considered.

Chapters I to IV of this Book concern the theory of coverings and the Poincaré group; they lead to a general formulation of van Kampen's theorem. The following chapters will deal with homology and cohomology, the higher homotopy groups and cellular spaces.

The notion of covering is the subject of Chapter I. Though this notion bears on certain continuous mappings $p: E\rightarrow B$, where E and B are topological spaces, the terminology adopted considers that the space E is the covering, the space B being its base, and the mapping $p$ is most often left implicit. We are thus led to study in general the structure of B-space (§1). Étalé B-spaces are defined in §2, but it is often useful to study them from the equivalent point of view of sheaves on B (§3). The notion of locally trivial fibre space is introduced in §4; these are the B-spaces locally isomorphic to a product $B\times F$, where the fibre F is a topological space. Coverings are those for which the fibre is a discrete topological space. In §5, we define the notion of Galois covering and prove that if the base B is nonempty, connected and locally connected, every covering can be associated with a Galois covering. Simply connected spaces are defined in §6: these are those for which every covering is trivializable; an interval of $\mathbf{R}$, a convex subset of

xi the numerical space $\mathbf{R}^n$, the sphere $\mathbf{S}_n$ of dimension $n\geqslant 2$ are simply connected spaces, but not the circle $\mathbf{S}_1$.

The algebraic notion of groupoid is defined in Chapter II; it generalizes that of group and had been introduced by H. Brandt in his study of invertible fractional ideals of quaternion algebras. The notions of quivers, graphs and categories are defined in §§1, 2 and 3 of Chapter II; a groupoid is a category all of whose arrows are invertible. The results of §§4 and 5 will make it possible to deduce from van Kampen's theorem, formulated in terms of groupoids, explicit presentations of Poincaré groups in various situations.

The classification of coverings of a given topological space B is effected by the introduction, in Chapter III, §3, of its Poincaré groupoid $\varpi (B)$, which is defined in terms of equivalence classes of paths in B modulo the relation of strict homotopy. When $b$ is a point of B, the Poincaré group $\pi_1(B, b)$ appears as the isotropy group at $b$ of the groupoid $\varpi (B)$. The notion of homotopy is introduced in §1; there one studies in particular the important homotopy extension property. §2 is devoted to the notion of path in a topological space and to the notions of arcwise connected space and locally arcwise connected space. There also a path lifting theorem is established.

The link between homotopy and coverings is studied in §§4 and 5. If E is a covering of a topological space B and if $b\in B$, the fibre $E_b$ is endowed with a natural operation of the group $\pi_1(B, b)$; this construction gives rise to a functor from the category of coverings of B into that of sets endowed with an action of $\pi_1(B, b)$. When B is a connected and locally arcwise connected topological space, this functor is fully faithful; its image consists of the operations of the group $\pi_1(B, b)$ on a discrete set which are continuous for a certain topology, called "admissible", on the group $\pi_1(B, b)$.

Chapter IV is devoted to unravelable spaces; these are the locally arcwise connected topological spaces for which the admissible topology of the Poincaré groups is the discrete topology. For these spaces, the correspondence between coverings and operations of the Poincaré group is thus perfect: the functor described above furnishes an equivalence of categories between the category of coverings of B and that of sets endowed with an operation of the group $\pi_1(B, b)$.

xii

A topological space B is said to be simply arcwise connected if it is arcwise connected and if the group $\pi_1(B, b)$ is trivial for every point $b$ of B. We prove that a nonempty unravelable space possesses a universal covering which is simply arcwise connected and Galois. We also prove that the Poincaré group of a compact and unravelable topological space is finitely presented (§2); without the assumption that the space is unravelable, this Poincaré group may have the power of the continuum (Shelah's theorem). We prove in §3 that the Poincaré group at the identity element of a connected topological group is abelian and (in the unravelable case) that its universal covering possesses a natural structure of topological group.

When $f: Y\rightarrow$ X is a continuous mapping and E is a Y-space, we describe in §4, in terms of descent data, the possible X-spaces from which E is obtained by base change. Thus we translate into the setting of General Topology a procedure used systematically by A. Grothendieck in Algebraic Geometry. We also give conditions ensuring that a covering of Y arises from a covering of X. Under certain hypotheses on $f$, this makes it possible to prove the general form of van Kampen's theorem: the Poincaré groupoid of X is isomorphic to a certain groupoid (coequalizer, chapter II, §5) constructed with the aid of the Poincaré groupoid of Y and that of the fibre square $Y\times_XY$.

For applications, however, it is necessary to deduce from this a presentation of the Poincaré group of X at a point. In §5, we thus apply the general calculations of chapter II to obtain such presentations in numerous examples. In particular, we calculate there the Poincaré group of X when a covering of X by a family of open subsets connected by paths has been given. As R. Brown in particular has shown, the groupoid point of view makes it possible to make no assumption on the pairwise connectedness of the intersections of these subsets. Under certain conditions of unloopability, we also treat the case of locally finite coverings of X by closed subsets. We also calculate there the Poincaré group of the quotient of an unloopable space by the proper and free action of a discrete group. Finally, we make explicit the original theorem of van Kampen, under somewhat different hypotheses.

Finally, in §6 we study the notion of classifying space for a topological group G: when one has such a space $B_G$, the study of the classes

xiii of isomorphism of principal fibre spaces with group G and paracompact base B is translated into a problem of studying the homotopy classes of mappings from B into $B_G$. When G is discrete, we construct a classifying space which is a metrisable space.

The results of chapters I to IV depend on the first four Books (E, A, TG, FVR); certain examples and remarks also use results of EVT, VAR, LIE III and LIE IV.

It was originally intended that this Book should form chapter XI of the Book on General Topology. In the preceding Books, the references to TG, XI, must therefore be modified as follows:

LIE, III, §1, No. 9, p. 114, note 1. Read "Cf. TA, IV, p. 379, Prop. 6."

LIE, III, §6, p. 192, note 1. Read "Let us recall (TA, I, p. 124, Def. 3) that a space

is said to be simply connected if each of its coverings is trivializable;

a simply connected space is connected. Let us also recall (TA, I, p. 100,

Cor. 3) that if $G_1,G_2$, are connected topological groups, if $\varphi$ is an

open continuous homomorphism of $G_1$ onto $G_2$ with discrete kernel, and if $G_2$ is

simply connected, then $\varphi$ is a homeomorphism."

LIE, III, §6, No. 7, p. 206, line 11. Instead of "by TG, XI", read "by

TA, IV, p. 379, Prop. 6".

LIE, VII, p. 66, appendix II, exercise 1. Instead of "TG, XI", read "TA, I,

p. 69, Def. 2".

LIE, IX, §2, No. 4, p. 12, line $-9$. Instead of "TG, XI, to appear", read "TA,

VII, to appear".

LIE, IX, §3, No. 6, p. 22. Instead of "TG, XI, to appear", read "TA, I, p. 127,

Example 3".

LIE, IX, §4, No. 2, p. 27, line 11. Instead of "TG, XI, to appear", read "TA,

VII, to appear".

LIE, IX, §4, No. 6, p. 34, line $-6$. Instead of "TG, XI, to appear", read "TA,

VII, to appear".

LIE, IX, §4, No. 9, p. 39, line 13. Instead of "TG, XI, to appear", read "by

TA, IV, p. 379, Prop. 6".

LIE, IX, §5, No. 4, p. 51, line $-13$. Instead of "TG, XI, to appear", read "by

TA, IV, p. 358, Example".

LIE, IX, §5, No. 4, p. 51, line $-4$. Instead of "cf. TG, XI, to appear", read "TA,

I, p. 106, Example 4 and p. 111, Prop. 10".

LIE, IX, §9, No. 1, p. 89, line 9. Instead of "by TG, XI", read "by TA,

I, p. 37, Th. 2".

LIE, IX, p. 112, exercise 8. Instead of "TG, XI", read "TA, VII".

LIE, IX, p. 118, exercise 2. Instead of "TG, XI", read "TA, III, p. 229, Def. 1".

xiv
