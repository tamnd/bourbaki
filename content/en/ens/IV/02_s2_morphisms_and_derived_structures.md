---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 2
section_title: Morphisms and derived structures
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 271-283, 290-294
pdf_pages: 0276-0288, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: MORPHISMS
      page: 271
      pdf_page: 276
    - "no": 2
      title: FINER STRUCTURES
      page: 273
      pdf_page: 278
    - "no": 3
      title: INITIAL STRUCTURES
      page: 274
      pdf_page: 279
    - "no": 4
      title: EXAMPLES OF INITIAL STRUCTURES
      page: 276
      pdf_page: 281
    - "no": 5
      title: FINAL STRUCTURES
      page: 280
      pdf_page: 285
    - "no": 6
      title: EXAMPLES OF FINAL STRUCTURES
      page: 281
      pdf_page: 286
statements: 12
exercises: 11
content_sha256: 33716172cbb3b2bb56712f0439f68cc2acc589398de3fe56f5601e43675e217a
---

## 2. MORPHISMS AND DERIVED STRUCTURES

### 1. MORPHISMS

In this section and the next we shall assume for the sake of simplicity that the species of structures under consideration has only one base set (which is therefore a principal base set). The reader will have no difficulty in extending the definitions and results to the general case.

Let $\Sigma$ be a species of structures in a theory $\mathscr{T}$ which is stronger than the theory of sets, and let $x$, $y$, $s$, $t$ be four distinct letters which are different from the constants of $\mathscr{T}$. We recall that the notation $\mathfrak{F}(x,y)$ denotes the set of mappings of $x$ into $y$ (Chapter II, § 5, no. 2). Suppose that we are given a term $\sigma\{x,y,s,t\}$ in $\mathscr{T}$ which satisfies the following conditions :

$(\mathrm{MO}_{\mathrm{I}})$ *The relation “$s$ is a structure of species $\Sigma$ on $x$, and $t$ is a structure of species $\Sigma$ on $y$” implies, in E, the relation $\sigma\{x,y,s,t\}\subset\mathfrak{F}(x,y)$.*

$(\mathrm{MO}_{\mathrm{II}})$ *If, in a theory $\mathscr{T}'$ stronger than $\mathscr{T}$, we have three sets E, E′, E″ endowed respectively with structures $\mathscr{S}$, $\mathscr{S}'$, $\mathscr{S}''$ of species $\Sigma$, then the relations $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ and $g\in\sigma\{E',E'',\mathscr{S}',\mathscr{S}''\}$ imply the relation*

$$
g\circ f\in\sigma\{E,E'',\mathscr{S},\mathscr{S}''\}.
$$

$(\mathrm{MO}_{\mathrm{III}})$ *If, in a theory $\mathscr{T}'$ stronger than $\mathscr{T}$, we have two sets E, E′ endowed respectively with structures $\mathscr{S}$, $\mathscr{S}'$ of species $\Sigma$, then a bijection $f$ of E onto E′ is an isomorphism if and only if $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ and $f^{-1}\in\sigma\{E',E,\mathscr{S}',\mathscr{S}\}$.*

If $\Sigma$ and $\sigma$ are given, the relation $f\in\sigma\{x,y,s,t\}$ is expressed by saying that $f$ is a *morphism* (or a $\sigma$-*morphism*) of $x$, endowed with $s$, into $y$, endowed with $t$. If (in a theory $\mathscr{T}'$ stronger than $\mathscr{T}$) E and E′ are two sets endowed with structures $\mathscr{S},\mathscr{S}'$ of species $\Sigma$, then the term $\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ is the *set of $\sigma$-morphisms of E into E′.*

*Examples*

#### Example 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

Take $\Sigma$ to be the species of order structures and let $\sigma\{x,y,s,t\}$ denote the set of all mappings $f$ of $x$ into $y$ such that the relation $(u,v)\in s$ implies $(f(u),f(v))\in t$. With the notation of Chapter III, § 1,

271 this means that $u \leqslant v$ implies $f(u) \leqslant f(v)$, i.e., that $f$ is *increasing*. The verification of axioms $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, and $(\mathrm{MO_{III}})$ is obvious.

#### Example 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

Take $\Sigma$ to be a species of algebraic structures which has a single (internal) law of composition, everywhere defined (§1, no. 4, Example 2). Let A, A$'$ be two sets endowed with structures of species $\Sigma$, and let $p$, $p'$ be the composition laws of these two structures. Consider the mappings $f$ of A into A$'$ such that $p'(f(x), f(y)) = f(p(x,\ y))$ for all $x \in \mathrm{A}$ and all $y \in \mathrm{A}$. These mappings satisfy $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, and $(\mathrm{MO_{III}})$, and are called *homomorphisms* of A into A$'$.

#### Example 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

Take $\Sigma$ to be the species of topological strcutures (§1, no. 4, Example 3). Let A, A$'$ be two sets endowed with topologies V, V$'$, respectively. Consider the mappings $f$ of A into A$'$ such that the relation $\mathrm{X}' \in \mathrm{V}'$ implies $\overset{-1}{f}(\mathrm{X}') \in \mathrm{V}$ (in other words, such that the inverse image of every open set in the topology V$'$ is an open set in the topology V). These mappings, which satisfy $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, and $(\mathrm{MO_{III}})$, are the *continuous* mappings of A into A$'$ (with respect to the topologies V and V$'$) (cf. *General Topology*, Chapter I, § 2).

#### Remark {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

For given species of structures $\Sigma$ we may have occasion to define various terms $\sigma \} x,\ y,\ s,\ t \{$ which satisfy the conditions $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, and $(\mathrm{MO_{III}})$. For example, if $\Sigma$ is the species of topological structures, with the notation of Example 3 above, a mapping $f$ of A into A$'$ is said to be *open* if the relation $\mathrm{X} \in \mathrm{V}$ implies $f(\mathrm{X}) \in \mathrm{V}'$ (in other words, if the image under $f$ of every open set is an open set). It is easily checked that the open mappings also satisfy conditions $(\mathrm{MO_I})$, $(\mathrm{MO_{II}})$, and $(\mathrm{MO_{III}})$ for the species $\Sigma$. \* Moreover, it can be shown that a continuous mapping is not necessarily open, and that an open mapping is not necessarily continuous. \* A given species of structures therefore *does not imply* a well-defined notion of morphisms.

☡

Where order structures, algebraic structures, and topological structures are concerned, it is always to be understood that the morphisms are those which have been defined in the Examples above, unless the contrary is expressly stated.

The condition $(\mathrm{MO_{III}})$ and the characterization of bijections (Chapter II, § 3, no. 8, Corollary to Proposition 8) imply the following criterion :

CST8. *Let* E, E$'$ *be two sets, each endowed with a structure of species $\Sigma$. Let $f$ be a $\sigma$-morphism of* E *into* E$'$ *and let $g$ be a $\sigma$-morhpism of* E$'$ *into* E. *If $g \circ f$ is the identity mapping of* E *onto itself, and if $f \circ g$ is the identity mapping of* E$'$ *onto itself, then $f$ is an isomorphism of* E *onto* E$'$, *and $g$ is the inverse isomorphism.*

It should be noted that a bijection of E onto E$'$ may be a $\sigma$-morphism without the inverse bijection necessarily being a $\sigma$-morphism. \* For example, a bijective mapping of a topological space A onto a topological space A$'$ can be continuous without the inverse bijection being continuous (*General Topology*, Chapter I, § 2, no. 1, Remark 1). \*

☡

#### Remark {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

When a species of structures $\Sigma$ has several principal base sets $x_1, \ldots, x_n$, and auxiliary base sets $\mathrm{A}_1, \ldots, \mathrm{A}_m$, a $\sigma$-morphism is a system $(f_1, \ldots, f_n)$, where $f_i$ is a mapping of $x_i$ into $y_i$ $(1 \leqslant i \leqslant n)$, and these systems of mappings satisfy conditions analogous to $(\mathrm{MO_{II}})$ and $(\mathrm{MO_{III}})$, which the reader may easily state for himself.

### 2. FINER STRUCTURES

For the rest of this section we shall suppose that we are given a species of structures $\Sigma$ and a notion of $\sigma$-morphism relative to this species of structures; *all the notions which will be introduced will depend not only on $\Sigma$ but also on the notion of $\sigma$-morphism envisaged.* Usually we shall say "morphism" in place of "$\sigma$-morphism".

¶ Let E be a set and let $\mathscr{S}_1$, $\mathscr{S}_2$ be two structures of species $\Sigma$ on E. The structure $\mathscr{S}_1$ is said to be *finer* than $\mathscr{S}_2$ (and $\mathscr{S}_2$ *coarser* than $\mathscr{S}_1$) if the identity mapping of E, endowed with $\mathscr{S}_1$, onto E, endowed with $\mathscr{S}_2$, is a morphism.

When necessary to avoid ambiguity, we shall say that $\mathscr{S}_1$ is finer than $\mathscr{S}_2$ *relative to the notion of $\sigma$-morphism under consideration*; and similarly for all the other notions to be defined in this section.

Suppose that $\mathscr{S}_1$ is finer than $\mathscr{S}_2$. If E$'$ is a set endowed with a structure $\mathscr{S}'$ of species $\Sigma$, and if $f$ is a morphism of E, endowed with $\mathscr{S}_2$, into E$'$, endowed with $\mathscr{S}'$, then $f$ is also a morphism of E, endowed with $\mathscr{S}_1$, into E$'$, endowed with $\mathscr{S}'$; this follows from the preceding definition and from $(\mathrm{MO_{II}})$. Likewise, if $g$ is a morphism of E$'$, endowed with $\mathscr{S}'$, into E, endowed with $\mathscr{S}_1$, then $g$ is also a morphism of E$'$, endowed with $\mathscr{S}'$, into E, endowed with $\mathscr{S}_2$.

Thus the *finer* the structure (of species $\Sigma$) on E, the *more* morphisms there are with E as source, and the *fewer* morphisms with E as target.

The relation "$\mathscr{S}_1$ is coarser than $\mathscr{S}_2$" is an *order relation* between $\mathscr{S}_1$ and $\mathscr{S}_2$ on the set of all structures of the species $\Sigma$ on E; for it is reflexive by $(\mathrm{MO_{III}})$, transitive by $(\mathrm{MO_{II}})$, and if a structure of species $\Sigma$ is both finer and coarser than another, then the two structures are identical by virtue of $(\mathrm{MO_{III}})$. In conformity with the general definitions (Chapter III, § 1, no. 14), two structures of species $\Sigma$ on E are said to be *comparable* if one is finer than the other; a structure is said to be *strictly finer* (resp. *strictly coarser*) than another if it is *finer* (resp. *coarser*) than the other and is distinct from it.

*Examples*

#### Example 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

An order structure with graph $s$ on a set A is finer than an order structure with graph $s'$ if and only if $s \subset s'$. In other words, the relation $x \leqslant y$ with respect to $s$ implies $x \leqslant y$ with respect to $s'$; this is in accordance with the definition given in Chapter III, § 1, no. 4, Example 3.

#### Example 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

Consider two algebraic structures F, F' of the same species $\Sigma$ on a set A, where F and F' are the graphs of the (everywhere defined) laws of composition of these two structures. From the definition of morphisms in this case (no. 1, Example 2), F is finer than F' if and only if $F \subset F'$. But since F and F' are both functional graphs with the same domain $A \times A$, we must have $F = F'$. In other words, two *comparable* structures of species $\Sigma$ are necessarily *identical*.

#### Example 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

Let V, V' be two topologies on the same set A. To say that V is finer than V' means, by virtue of the definition of morphisms in this case (no. 1, Example 3), that $V' \subset V$; in other words, every subset of A which is an open set in the topology V' is also an open set in the topology V (and thus, the finer the topology, the more open sets there are).

#### Remark {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

We have just met an example (Example 2) in which two comparable structures of the same species $\Sigma$ are necessarily identical. There are many other such examples : linear order structures, \* compact topologies, Fréchet space structures (the morphisms being continuous linear mappings), topologies defined by an absolute value (or a valuation) on a division ring, etc. \*

For such a species of structures $\Sigma$, a morphism $f$ of E into E' which is *bijective* is an *isomorphism*; for if we transport to E' the structure $\mathscr{S}$ on E by means of $f$, we obtain a structure of species $\Sigma$ which is finer than the structure $\mathscr{S}'$ on E' and therefore coincides with $\mathscr{S}'$.

### 3. INITIAL STRUCTURES

Consider a family $(A_\iota)_{\iota \in I}$ of sets, each of which is endowed with a structure $\mathscr{S}_\iota$ of species $\Sigma$. Let E be a set, and for each $\iota \in I$ let $f_\iota$ be a mapping *of* E *into* $A_\iota$. A structure $\mathscr{S}$ of species $\Sigma$ on E is said to be an *initial structure with respect to the family* $(A_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in I}$ if it has the following property :

(IN) Given any set E', any structure of species $\mathscr{S}'$ on E', and any mapping $g$ *of* E' *into* E, the relation

"$g$ is a morphism of E' into E"

is *equivalent* to the relation

"for each $\iota \in I, f_\iota \circ g$ is a morphism of E' into $A_\iota$".

CST9. *If there exists an initial structure on* E *with respect to the family* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ f_\iota)_{\iota \in \mathrm{I}}$, *it is the coarsest of all structures of species* $\Sigma$ *on* E *for which each of the mappings* $f_\iota$ *is a morphism, and consequently is unique.*

Let $\mathscr{I}$ be an initial structure on E, and let $\mathscr{S}$ be a structure of species $\Sigma$ on E for which each of the $f_\iota$ is a morphism. If $i$ denotes the identity mapping of E, endowed with $\mathscr{S}$, into E, endowed with $\mathscr{I}$, then $f_\iota \circ i$ is a morphism for all $\iota \in \mathrm{I}$, and the condition (IN) shows that $i$ is a morphism, which means (no. 2) that $\mathscr{S}$ is *finer* than $\mathscr{I}$. On the other hand, applying (IN) to the case in which $g$ is the identity mapping of E (endowed with $\mathscr{I}$) onto itself, we see (by $(\mathrm{MO_{III}})$) that each $f_\iota$ is a morphism of E into $\mathrm{A}_\iota$, which completes the proof.

It may happen that there exists a structure of species $\Sigma$ on E which is the coarsest of all the structures of species $\Sigma$ for which the $f_\iota$ are morphisms, but that this structure is not the initial structure with respect to $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)$ (Exercise 6).

We have the following *transitivity criterion* :

CST10. *Let* E *be a set, let* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *be a family of sets, and for each* $\iota \in \mathrm{I}$ *let* $\mathscr{S}_\iota$ *be a structure of species* $\Sigma$ *on* $\mathrm{A}_\iota$. *Let* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *be a partition of* I, *and let* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *be a family of sets indexed by* L. *For each* $\lambda \in \mathrm{L}$ *let* $h_\lambda$ *be a mapping of* E *into* $\mathrm{B}_\lambda$, *and for each* $\lambda \in \mathrm{L}$ *and each* $\iota \in \mathrm{J}_\lambda$ *let* $g_{\lambda\iota}$ *be a mapping of* $\mathrm{B}_\lambda$ *into* $\mathrm{A}_\iota$, *and let* $f_\iota = g_{\lambda\iota} \circ h_\lambda$. *Suppose that, for each* $\lambda \in \mathrm{L}$, *there exists an initial structure* $\mathscr{S}'_\lambda$ *on* $\mathrm{B}_\lambda$ *with respect to the family* $(\mathrm{A}_\iota, \mathscr{S}_\iota, g_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda}$. *Then the following statements are equivalent* :

(a) *there exists an initial structure* $\mathscr{I}$ *on* E *with respect to the family* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$;

(b) *there exists an initial structure* $\mathscr{I}'$ *on* E *with respect to the family* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Furthermore, these statements imply that* $\mathscr{I} = \mathscr{I}'$.

Let F be a set endowed with a structure of species $\Sigma$, and let $u$ be a mapping of F into E. Observe that by definition the relation "$h_\lambda \circ u$ is a morphism of F into $\mathrm{B}_\lambda$" is equivalent to the relation "for all $\iota \in \mathrm{J}_\lambda$, $g_{\lambda\iota} \circ h_\lambda \circ u = f_\iota \circ u$ is a morphism of F into $\mathrm{A}_\iota$". The relation

(1)     "for all $\lambda \in \mathrm{L}$, $h_\lambda \circ u$ is a morphism of F into $\mathrm{B}_\lambda$"

is therefore equivalent to the relation

(2)     "for all $\iota \in \mathrm{I}$, $f_\iota \circ u$ is a morphism of F into $\mathrm{A}_\iota$".

Now, to say that $\mathscr{I}'$ is the initial structure with respect to the family $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ means that relation (1) is equivalent to the relation "$u$ is a morphism of F into E endowed with $\mathscr{I}'$"; and to say that $\mathscr{I}$ is the initial structure with respect to the family $(A_i,\,\mathscr{G}_i,\,f_i)_{i\in I}$ means that relation (2) is equivalent to the relation “$u$ is a morphism of F into E endowed with $\Gamma$”. Hence the result, in view of the property of uniqueness of initial structure.

### 4. EXAMPLES OF INITIAL STRUCTURES

I. *Inverse image of a structure.* When I is a set consisting of a single element, the initial structure with respect to $(A,\,\mathscr{G},\,f)$ is called the *inverse image under $f$ of the structure $\mathscr{G}$* (when it exists).

\* A topology always has an inverse image under any mapping $f$; but this is not the case for an order structure or an algebraic structure. \*

II. *Induced structure.* Let A be a set endowed with a structure $\mathscr{G}$ of species $\Sigma$, let B be a subset of A, and let $j$ be the canonical injection of B into A. Then the inverse image under $j$ of the structure B (if it exists) is called the *structure induced by $\mathscr{G}$ on B.*

An order structure induces a structure of the same species on every subset of the set on which it is defined; but this is not the case for the structure of a directed set. \* A topology induces a topology on every subset of the set on which it is defined, but a compact topology does not in general induce a compact topology. An algebraic structure on a set A does not in general induce a structure of the same species on an arbitrary subset B; if the given structure on A consists of laws of composition which are everywhere defined, then it is necessary that B should be stable with respect to each of these laws, but this necessary condition is not always sufficient. \*

The general criterion CST10 gives us the following *transitivity criterion* for induced structures :

CST11. *Let B be a subset of A, let C be a subset of B, and let $\mathscr{G}$ be a structure of species $\Sigma$ on A which induces a structure $\mathscr{G}'$ of the same species on B. Then $\mathscr{G}$ induces a structure of species $\Sigma$ on C if and only if $\mathscr{G}'$ induces a structure of species $\Sigma$ on C, and the structures induced on C by $\mathscr{G}$ and $\mathscr{G}'$ are then identical.*

CST12. *Let A, A' be two sets endowed with structures $\mathscr{G}$, $\mathscr{G}'$ of species $\Sigma$. Let B be a subset of A, and B' a subset of A'. Suppose that $\mathscr{G}$ (resp. $\mathscr{G}'$) induces a structure of species $\Sigma$ on B (resp. B'). If $f$ is a morphism of A into A' such that $f(B)\subset B'$, then the mapping of B into B' which coincides with $f$ on B is a morphism (with respect to the structures induced by $\mathscr{G}$ and $\mathscr{G}'$).*

Let $j$ (resp. $j'$) be the canonical injection of B (resp. B') into A (resp. A'). By definition we have $f\circ j=j'\circ g$. Since $f$ and $j$ are morphisms,

276 so is $f\circ j$ by (MO$_{\mathrm{II}}$); but then, $j'\circ g$ being a morphism, the mapping $g$ is a morphism by the definition of initial structure.

III. *Product structure.* Let $(A_i)_{i\in I}$ be a family of sets, and on each set $A_i$ let $\mathscr{S}_i$ be a structure of species $\Sigma$. Let $E=\prod_{i\in I}A_i$ be the *product* of the family $(A_i)_{i\in I}$ (Chapter II, § 5), and let $\operatorname{pr}_i$ denote the projection of $E$ onto $A_i$. The initial structure (if it exists) with respect to the family $(A_i,\mathscr{S}_i,\operatorname{pr}_i)_{i\in I}$ is called the *product* of the structures $\mathscr{S}_i$.

\* A family of order structures always admits a product structure, but the same is not always true of a family of total order structures. A family of group structures always admits a product structure, but the same need not be true of a family of division ring structures. A family of topologies always admits a product structure, but this is not always true of a family of structures of locally compact spaces; in this case, there is a product structure of the same species if the family is *finite*, but there need not be one if the family is *infinite* (cf. *General Topology*, Chapter I, § 9, no. 7, Prop. 14). \*

Criterion CST10 gives rise to the following *associativity criterion* for product structures :

CST13. *Let $(A_i)_{i\in I}$ be a family of sets, and for each index $i\in I$ let $\mathscr{S}_i$ be a structure of species $\Sigma$ on $A_i$. Let $(J_\lambda)_{\lambda\in L}$ be a partition of $I$. Suppose that on each partial product $B_\lambda=\prod_{i\in J_\lambda}A_i$, the family $(\mathscr{S}_i)_{i\in J_\lambda}$ admits a product structure $\mathscr{S}'_\lambda$. Then the family $(\mathscr{S}_i)_{i\in I}$ admits a product structure $\mathscr{S}$ if and only if the family $(\mathscr{S}'_\lambda)_{\lambda\in L}$ admits a product structure $\mathscr{S}'$, and the canonical mapping of $E=\prod_{i\in I}A_i$, endowed with $\mathscr{S}$, onto $F=\prod_{\lambda\in L}B_\lambda$, endowed with $\mathscr{S}'$ (Chapter II, § 5, no. 5), is then an isomorphism.*

Another application of CST10 gives the following criterion concerning structures induced by a product structure :

CST14. *Let $(A_i)_{i\in I}$ be a family of sets, and for each $i\in I$ let $\mathscr{S}_i$ be a structure of species $\Sigma$ on $A_i$. For each $i\in I$, let $B_i$ be a subset of $A_i$. Suppose that each $\mathscr{S}_i$ induces a structure $\mathscr{S}'_i$ on $B_i$, and that on the product $E=\prod_{i\in I}A_i$ there exists a structure $\mathscr{S}_0$ which is the product of the family $(\mathscr{S}_i)$. Then the following statements are equivalent :*

(a) on the set $B=\prod_{i\in I}B_i\subset E$ there exists a structure $\mathscr{S}$ induced by $\mathscr{S}_0$;

(b) on the set $B$ there exists a structure $\mathscr{S}'$ which is the product of the family of structures $(\mathscr{S}'_i)$.

*Furthermore, these statements imply that $\mathscr{S}=\mathscr{S}'$.*

Let $j_\iota$ be the canonical injection of $\mathrm{B}_\iota$ into $\mathrm{A}_\iota$, let $j$ be the canonical injection of B into E, let $p_\iota$ be the projection of E onto $\mathrm{A}_\iota$, and let $p'_\iota$ be the projection of B onto $\mathrm{B}_\iota$. Then we have $p_\iota \circ j = j_\iota \circ p'_\iota$ for all $\iota \in \mathrm{I}$. By CST10, $\mathscr{S}$ is the initial structure with respect to the family $(\mathrm{A}_\iota, \mathscr{S}_\iota, p_\iota \circ j)_{\iota \in \mathrm{I}}$, and $\mathscr{S}'$ is the initial structure with respect to the family $(\mathrm{A}_\iota, \mathscr{S}_\iota, j_\iota \circ p'_\iota)_{\iota \in \mathrm{I}}$. Hence the result.

¶ The notions of inverse image and product are related by the following criterion :

CST15. *Let $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ be a family of sets, and for each $\iota \in \mathrm{I}$ let $\mathscr{S}_\iota$ be a structure of species $\Sigma$ on $\mathrm{A}_\iota$, and let $f_\iota$ be a mapping of a set E into $\mathrm{A}_\iota$. Suppose that on the product set $\mathrm{A} = \prod_{\iota \in \mathrm{J}} \mathrm{A}_\iota$ there exists a product structure $\mathscr{S}$ of the family $(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$. Then there exists an initial structure with respect to the family $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ if and only if the structure $\mathscr{S}$ has an inverse image under the mapping $x \to f(x) = (f_\iota(x))$ of E into A, and these two structures are then identical.*

Since $f_\iota = \mathrm{pr}_\iota \circ f$, this criterion is a particular case of CST10.

#### Remark {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

Let $(\mathscr{S}_\lambda)_{\lambda \in \mathrm{L}}$ be a family of structures of species $\Sigma$ on the *same* set A; let $\mathrm{A}_\lambda$ denote the set A endowed with the structure $\mathscr{S}_\lambda$, and let $\mathrm{I}_\lambda$ denote the identity mapping of A into $\mathrm{A}_\lambda$. Let B be the product set $\mathrm{A}^{\mathrm{L}} = \prod_{\lambda \in \mathrm{L}} \mathrm{A}_\lambda$, and let $\Delta$ be the diagonal of this product (Chapter II, § 5, no. 3). Let $h$ be the diagonal mapping of A onto $\Delta$, so that $h(x)$ is the element $(x_\lambda)_{\lambda \in \mathrm{L}}$ such that $x_\lambda = x$ for all $\lambda \in \mathrm{L}$. Suppose that there exists on B a product structure $\mathscr{S}'$ of the family $(\mathscr{S}_\lambda)$. Since $h$ is injective, criterion CST 15 shows that there exists an initial structure $\mathscr{S}$ with respect to the family $(\mathrm{A}_\lambda, \mathscr{S}_\lambda, \mathrm{I}_\lambda)_{\lambda \in \mathrm{L}}$ if and only if there exists a structure $\mathscr{S}''$ on $\Delta$ induced by $\mathscr{S}'$; $\mathscr{S}''$ is then identical with the structure obtained by transporting $\mathscr{S}$ to $\Delta$ by means of $h$. In particular, when all the structures $\mathscr{S}_\lambda$ are identical, $h$ is an *isomorphism* of A (endowed with this structure) onto $\Delta$.

We have also the following criterion :

CST16. *Let $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$, $(\mathrm{B}_\iota)_{\iota \in \mathrm{I}}$ be two families of sets indexed by the same set. For each $\iota \in \mathrm{I}$, let $\mathscr{S}_\iota$ be a structure of species $\Sigma$ on $\mathrm{A}_\iota$ and let $\mathscr{S}'_\iota$ be a structure of species $\Sigma$ on $\mathrm{B}_\iota$. Suppose that there exists on $\mathrm{A} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota \left( \text{resp. on } \mathrm{B} = \prod_{\iota \in \mathrm{I}} \mathrm{B}_\iota \right)$ a product structure $\mathscr{S}$ (resp. $\mathscr{S}'$) of the family $(\mathscr{S}_\iota)$ (resp. $(\mathscr{S}'_\iota)$). For each $\iota \in \mathrm{I}$, let $f_\iota$ be a morphism of $\mathrm{A}_\iota$ into $\mathrm{B}_\iota$. Then the mapping $f = (f_\iota)_{\iota \in \mathrm{I}}$ is a morphism of A into B.*

Let $p_\iota$ (resp. $q_\iota$) be the projection of A onto $\mathrm{A}_\iota$ (resp. of B onto $\mathrm{B}_\iota$). Then we have $q_\iota \circ f = f_\iota \circ p_\iota$. Since $f_\iota$ and $p_\iota$ are morphisms (criterion

CST9), $f_i \circ p_i$ is a morphism by (MO$_\Pi$); hence $f$ is a morphism by (IN).

#### Remark {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

For most of the usual structures, the condition given in CST16 is not only sufficient but also necessary for $f$ to be a morphism (cf. Exercise 7). In particular, this is so in the following circumstances (which occur, for example, if $\Sigma$ is the species of order structures, \* or the species of group structures, or the species of topological structures *, etc.; cf. Exercise 8) :

☡

¶ There exists a family $(a_i)_{i\in I}$ such that $a_i\in A_i$ for all $i\in I$ and such that, if we put $r_i(x)=(y_\lambda)$, where $y_i=x_i$ and $y_\lambda=a_\lambda$ whenever $\lambda\ne i$, each of the mappings $r_i$ is a morphism of $A_i$ into $A$. For if $f=(f_i)$ is a morphism of $A$ into $B$, we may write $f_i=q_i\circ f\circ r_i$ for all $i\in I$, and it is enough to apply (MO$_\Pi$).

¶ Note that $r_i$ is a morphism if the following condition is satisfied :

(a) For every set $E$ endowed with a structure of species $\Sigma$, the constant mapping $z\mapsto a_i$ is a morphism of $E$ into $A_i$; namely, for each $x\in I$, $p_x\circ r_i$ is a morphism of $A_i$ into $A_x$, since it is the identity mapping when $x=i$, and a constant mapping $z\mapsto a_x$ when $x\ne i$; by the definition of product structure, $r_i$ is therefore a morphism of $A_i$ into $A$.

¶ The examples listed above satisfy not only (a), but also the following condition :

(b) On every set $A'_i=A_i\times\prod_{x\ne i}\{a_x\}$, the structure $\mathscr{I}$ induces a structure of species $\Sigma$.

¶ Let $p'_i$ denote the restriction of $p_i$ to $A'_i$. If both conditions (a) and (b) are satisfied, then $p'_i$ is an isomorphism of $A'_i$ onto $A_i$. For since $p'_i=p_i\circ j_i$, where $j_i$ is the canonical injection of $A'_i$ into $A$, $p'_i$ is a morphism by (MO$_\Pi$). Also we have $r_i=j_i\circ {p'_i}^{-1}$; hence ${p'_i}^{-1}$ is a morphism of $A_i$ into $A'_i$ by virtue of the definition of induced structure.

Finally, we have the following criterion, which characterizes the morphisms in many cases :

**CST17.** — Let $A$ and $B$ be two sets, endowed with structures $\mathscr{S}_A$, $\mathscr{S}_B$ of the same species $\Sigma$. Suppose that there exists on $A\times B$ the structure $\mathscr{S}_{A\times B}$, the product of $\mathscr{S}_A$ and $\mathscr{S}_B$. Let $f$ be a mapping of $A$ into $B$, let $F$ be its graph, and let $\pi$ be the bijection $x\mapsto (x,f(x))$ of $A$ onto $F$. Then, for $f$ to be a morphism of $A$ into $B$, it is necessary and sufficient that there should exist on $F$ a structure of species $\Sigma$ induced by $\mathscr{S}_{A\times B}$ and that, when $F$ is endowed with this structure, $\pi$ should be an isomorphism of $A$ onto $F$.

To prove sufficiency, let $j$ be the canonical injection of $F$ into $A\times B$. We may write $f=\operatorname{pr}_2\circ j\circ\pi$, and $f$ is then by hypothesis the composition of three morphisms.

¶ To prove necessity, let $\mathscr{S}_{\mathbf{F}}$ be the structure of species $\Sigma$ obtained by transporting the structure $\mathscr{S}_{\mathbf{A}}$ to F by means of the bijection $\pi$ (§ 1, no. 5). Then we must show that $\mathscr{S}_{\mathbf{F}}$ is induced by $\mathscr{S}_{\mathbf{A} \times \mathbf{B}}$ on F. We remark first that $j$ is a morphism of F into $\mathbf{A} \times \mathbf{B}$; for $j \circ \pi$ is the mapping $x \to (x, f(x))$ of A into $\mathbf{A} \times \mathbf{B}$ and is therefore a morphism by virtue of the hypothesis on $f$ and the definition of the product structure; hence, by the definition of the structure $\mathscr{S}_{\mathbf{F}}$, $j$ is a morphism. It remains to be shown that if E is a set endowed with a structure of species $\Sigma$, and if $g$ is a mapping of E into F such that $j \circ g$ is a morphism of E into $\mathbf{A} \times \mathbf{B}$, then $g$ is a morphism; or, equivalently, that $g_1 = \overset{-1}{\pi} \circ g$ is a morphism of E into A. But since $g_1 = \mathrm{pr}_1 \circ (j \circ g)$, this follows from the hypothesis and the definition of the product structure.

### 5. FINAL STRUCTURES

Consider a family of sets $(\mathbf{A}_\iota)_{\iota \in \mathbf{I}}$, each endowed with a structure $\mathscr{S}_\iota$ of species $\Sigma$. Let E be a set, and for each $\iota \in \mathbf{I}$ let $g_\iota$ be a mapping *of* $\mathbf{A}_\iota$ *into* E. A structure $\mathscr{T}$ of species $\Sigma$ on E is said to be a *final structure with respect to the family* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$ if it has the following property :

(FI) Given any set E′, any structure $\mathscr{S}'$ of species $\Sigma$ on E, and any mapping $f$ *of* E *into* E′, the relation

$$\text{``}f \text{ is a morphism of E into E'''}$$

is *equivalent* to the relation

$$\text{``for all } \iota \in \mathbf{I}, f \circ g_\iota \text{ is a morphism of } \mathbf{A}_\iota \text{ into E'''}.$$

CST18. *If there exists a final structure on* E *with respect to the family* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$, *then it is the finest structure of species* $\Sigma$ *on* E *for which each of the mappings* $g_\iota$ *is a morphism, and is therefore unique.*

Let $\mathscr{T}$ be a final structure on E, and let $\mathscr{S}$ be a structure of species $\Sigma$ on E for which each $g_\iota$ is a morphism. If $i$ denotes the identity mapping of E, endowed with $\mathscr{T}$, onto E, endowed with $\mathscr{S}$, then $i \circ g_\iota$ is a morphism for each $\iota \in \mathbf{I}$. The condition (FI) then shows that $i$ is a morphism, which means (no. 2) that $\mathscr{S}$ is *coarser* than $\mathscr{T}$. Applying (FI) again to the case in which $f$ is the identity mapping of E (endowed with $\mathscr{T}$) onto itself, we see (using $(\mathrm{MO_{III}})$) that each $g_\iota$ is a morphism of $\mathbf{A}_\iota$ into E. This completes the proof.

It may happen that there exists a structure of species $\Sigma$ on E which is the finest of all structures of species $\Sigma$ on E for which the $g_\iota$ are morphisms, but that this structure is not the final structure with respect to the family $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)$ (Exercise 6).

We have the following *transitivity criterion* :

CST19. *Let* E *be a set, let* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *be a family of sets, and for each* $\iota \in \mathrm{I}$ *let* $\mathscr{S}_\iota$ *be a structure of species* $\Sigma$ *on* $\mathrm{A}_\iota$. *Let* $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *be a partition of* I, *and let* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$ *be a family of sets indexed by* L. *For each* $\lambda \in \mathrm{L}$, *let* $h_\lambda$ *be a mapping of* $\mathrm{B}_\lambda$ *into* E; *for each* $\lambda \in \mathrm{L}$ *and each* $\iota \in \mathrm{J}_\lambda$, *let* $g_{\iota\lambda}$ *be a mapping of* $\mathrm{A}_\iota$ *into* $\mathrm{B}_\lambda$, *and put* $f_\iota = h_\lambda \circ g_{\iota\lambda}$. *Suppose that, for each* $\lambda \in \mathrm{L}$, *there exists a final structure* $\mathscr{S}'_\lambda$ *on* $\mathrm{B}_\lambda$ *with respect to the family* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ g_{\iota\lambda})_{\iota \in \mathrm{J}_\lambda}$. *Then the following statements are equivalent* :

(a) *There exists a final structure* $\mathscr{S}$ *on* E *with respect to the family* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$.

(b) *There exists a final structure* $\mathscr{S}'$ *on* E *with respect to the family* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$.

*Furthermore these statements imply that* $\mathscr{S} = \mathscr{S}'$.

Let F be a set endowed with a structure of species $\Sigma$, and let $u$ be a mapping of E into F. By definition, the relation "$u \circ h_\lambda$ is a morphism of $\mathrm{B}_\lambda$ into F" is equivalent to the relation

"for all $\iota \in \mathrm{J}_\lambda$, $u \circ h_\lambda \circ g_{\iota\lambda} = u \circ f_\iota$ is a morphism of $\mathrm{A}_\iota$ into F".

The relation

(3)             "for all $\lambda \in \mathrm{L}$,   $u \circ h_\lambda$ is a morphism of $\mathrm{B}_\lambda$ into F"

is therefore equivalent to the relation

(4)             "for all $\iota \in \mathrm{I}$,   $u \circ f_i$ is a morphism of $\mathrm{A}_\iota$ into F".

To say that $\mathscr{S}'$ is the final structure with respect to the family $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ means that the relation (3) is equivalent to the relation "$u$ is a morphism of E (endowed with $\mathscr{S}'$) into F"; and to say that E is the final structure with respect to the family $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ means that the relation (4) is equivalent to the relation "$u$ is a morphism of E (endowed with $\mathscr{S}$) into F"; hence the result, in view of the property of uniqueness of final structure.

### 6. EXAMPLES OF FINAL STRUCTURES

I. *Direct image of a structure.*   When I is a set consisting of a single element, the final structure with respect to $(\mathrm{A}, \mathscr{S}, f)$ is called the *direct image under* $f$ *of the structure* $\mathscr{S}$ (when it exists).

II. *Quotient structure.*   Let A be a set endowed with a structure $\mathscr{S}$ of species $\Sigma$, let R be an equivalence relation on A, and let $\varphi$ be the canonical mapping of A onto the quotient set $\mathrm{E} = \mathrm{A}/\mathrm{R}$ (Chapter II, § 6, no. 2). The direct image of the structure $\mathscr{S}$ under the mapping $\varphi$ is called (when it exists) the *quotient* of the structure $\mathscr{S}$ by the relation R.

\* In general, an order structure or an algebraic structure does not admit quotient structures with respect to arbitrary equivalence relations (cf. Chapter III, § 1, Exercise 2). On the other hand, a topology always admits a quotient structure with respect to an arbitrary equivalence relation, but this is not necessarily the case for a Hausdorff topology. \*

Let A, B be two sets endowed respectively with structures $\mathscr{S}$, $\mathscr{S}'$ of species $\Sigma$, and let $f$ be a morphism of A into B. Let R be the equivalence relation $f(x) = f(y)$, let $\varphi$ be the canonical mapping of A onto $\mathrm{A}/\mathrm{R}$, and let $j$ be the canonical injection of $f(\mathrm{A})$ into B. Suppose that $\mathscr{S}$ admits a quotient structure $\mathscr{S}_0$ with respect to R, and that $\mathscr{S}'$ induces a structure $\mathscr{S}'_0$ on $f(\mathrm{A})$. Then, in the *canonical decomposition* $f = j \circ g \circ \varphi$ of $f$ (Chapter II, § 6, no. 5), the bijection $g$ of $\mathrm{A}/\mathrm{R}$ onto $f(\mathrm{A})$ which is associated with $f$ is a *morphism* (but not necessarily an isomorphism) when $\mathrm{A}/\mathrm{R}$ is endowed with $\mathscr{S}_0$ and $f(\mathrm{A})$ with $\mathscr{S}'_0$. For $j \circ g$ is a morphism of $\mathrm{A}/\mathrm{R}$ into B by the definition of quotient structure, and $g$ is therefore a morphism of $\mathrm{A}/\mathrm{R}$ onto $f(\mathrm{A})$ by the definition of induced structure.

CST20. *Let* A, A′ *be two sets endowed with structures* $\mathscr{S}$, $\mathscr{S}'$ *of species* $\Sigma$, *and let* R (*resp.* R′) *be an equivalence relation on* A (*resp.* A′). *Suppose that there exists a quotient structure* $\mathscr{S}_0$ (*resp.* $\mathscr{S}'_0$) *of* $\mathscr{S}$ *by* R (*resp.* $\mathscr{S}'$ *by* R′). *If* $f$ *is a morphism of* A *into* A′ *which is compatible with the equivalence relations* R *and* R′, *and if* $g$ *is the mapping obtained from* $f$ *by passing to the quotients, then* $g$ *is a morphism of* $\mathrm{A}/\mathrm{R}$ *into* $\mathrm{A}'/\mathrm{R}'$.

Let $\varphi$ (resp. $\varphi'$) be the canonical mapping of A onto $\mathrm{A}/\mathrm{R}$ (resp. of A′ onto $\mathrm{A}'/\mathrm{R}'$); then we have $g \circ \varphi = \varphi' \circ f$. Since $\varphi'$ and $f$ are morphisms, so is $\varphi' \circ f$ by ($\mathrm{MO_{II}}$). But then, $g \circ \varphi$ being a morphism, $g$ is also a morphism by the definition of quotient structure.

¶ The transitivity criterion CST19 gives rise in particular to the following criterion :

CST21. *Let* A *be a set endowed with a structure* $\mathscr{S}$ *of species* $\Sigma$, *and let* R *be an equivalence relation on* A *such that there exists on* $\mathrm{A}/\mathrm{R}$ *a quotient structure* $\mathscr{S}'$ *of* $\mathscr{S}$ *by* R. *Let* S *be an equivalence relation on* A *which is coarser than* R, *and let* $\mathrm{S}/\mathrm{R}$ *denote the equivalence relation on* $\mathrm{A}/\mathrm{R}$ *which is the quotient of* S *by* R (Chapter II, § 6, no. 7). *Then there exists on* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *a quotient structure* $\mathscr{S}''$ *of* $\mathscr{S}'$ *by* $\mathrm{S}/\mathrm{R}$ *if and only if there exists on* $\mathrm{A}/\mathrm{S}$ *a quotient structure* $\mathscr{S}_0$ *of* $\mathscr{S}$ *by* S, *and the canonical mapping of* $\mathrm{A}/\mathrm{S}$ (*endowed with* $\mathscr{S}_0$) *onto* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ (*endowed with* $\mathscr{S}''$) *is an isomorphism.*

Let $\varphi$ be the canonical mapping of A onto $A/R$, and let $\psi$ be that of $A/R$ onto $(A/R)/(S/R)$. By virtue of CST19, $\mathscr{G}''$ is the quotient of $\mathscr{G}'$ by $S/R$ if and only if $\mathscr{G}''$ is the final structure with respect to $(A,\mathscr{G},\psi\circ\varphi)$. The criterion then follows from the fact that the relation $\psi(\varphi(x))=\psi(\varphi(y))$ is equivalent to S.

#### Remark {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

Let A be a set endowed with a structure $\mathscr{G}$ of species $\Sigma$, and let R be an equivalence relation on A such that there exists on $E=A/R$ a quotient structure $\mathscr{G}'$ of $\mathscr{G}$ by R. Let $\varphi$ be the canonical mapping of A onto E. In general, there exists no *section* $s$ of $\varphi$ (Chapter II, § 3, no. 8) which is a *morphism* of E into A. Let us suppose that such a section $s$ exists, and moreover that there exists a structure $\mathscr{G}''$ induced by $\mathscr{G}$ on $s(E)$. Then, if $j$ denotes the canonical injection of $s(E)$ into A and if $s=j\circ f$, the bijection $f$ is an *isomorphism* of E onto $s(E)$. For $f$ is a morphism by the definition of induced structure, and $g=\varphi\circ j$ is a morphism of $s(E)$ onto E by reason of (MO$_{\mathrm{II}}$). Since $g\circ f$ and $f\circ g$ are the identity mappings of E and $s(E)$, respectively, the assertion is a consequence of CST8.

### Exercises {#ens-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
