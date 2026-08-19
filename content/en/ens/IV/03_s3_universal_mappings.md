---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 3
section_title: Universal mappings
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 283-288, 294-295
pdf_pages: 0288-0293, 0299-0300
extraction: ocr
subsections:
    - "no": 1
      title: UNIVERSAL SETS AND MAPPINGS
      page: 283
      pdf_page: 288
    - "no": 2
      title: EXISTENCE OF UNIVERSAL MAPPINGS
      page: 284
      pdf_page: 289
    - "no": 3
      title: EXAMPLES OF UNIVERSAL MAPPINGS
      page: 286
      pdf_page: 291
statements: 0
exercises: 3
content_sha256: 98de15070c6122f15d37cc5ed3db1f93782ce63e3a7bbc618529bef0a4082473
---

## 3. UNIVERSAL MAPPINGS

### 1. UNIVERSAL SETS AND MAPPINGS

Let $\mathscr{T}$ be a theory which is stronger than the theory of sets, and let E be a term in $\mathscr{T}$. Let $\Sigma$ be a species of structures in $\mathscr{T}$. For simplicity we shall suppose throughout that $\Sigma$ is defined on a single (principal) base set, and for brevity we shall say “$\Sigma$-set” for “set endowed with a structure of species $\Sigma$”. Furthermore, we shall suppose that the $\sigma$-morphisms have been defined for the species $\Sigma$ (§ 2, no. 1; as in § 2, we shall say “morphism” in place of “$\sigma$-morphism”). Finally, the species $\Sigma$ being defined on the base set $x$ and having $s$ as generic structure (§ 1, no. 4), let us suppose that a term $\alpha\{x,s\}$ is defined in $\mathscr{T}_{\Sigma}$, satisfying the following conditions :

(QM$_{\mathrm{I}}$) *The relation $\alpha\{x,s\}\subset\mathscr{T}(E;x)$ is true in $\mathscr{T}_{\Sigma}$.*

(QM$_{\mathrm{II}}$) *If (in a theory $\mathscr{T}'$ which is stronger than $\mathscr{T}$) F and F′ are two sets endowed with structures $\mathscr{G},\mathscr{G}'$ of species $\Sigma$, and if $f$ is a morphism of F into F′, then the relation $\varphi\in\alpha\{F,\mathscr{G}\}$ implies $f\circ\varphi\in\alpha\{F',\mathscr{G}'\}$.*

We shall express the relation $\varphi\in\alpha\{x,s\}$ by saying that $\varphi$ is an $\alpha$-mapping of E into $x$ (endowed with $s$).

A $\Sigma$-set $F_E$ and an $\alpha$-mapping $\varphi_E$ of E into $F_E$ are said to be *universal* if the following condition is satisfied :

$(AU)$ *For each $\alpha$-mapping $\varphi$ of E into a $\Sigma$-set F there exists a unique morphism $f$ of $F_E$ into F such that $\varphi=f\circ\varphi_E$.*

The pair $(F_E,\varphi_E)$ is then also said to be a *solution of the universal mapping problem* for E (relative to $\Sigma$, $\sigma$, and $\alpha$).

¶ Let $(F'_E,\varphi'_E)$ and $(F''_E,\varphi''_E)$ be two solutions of the universal mapping problem for E. The condition $(AU)$ shows then that there exists a unique morphism $f_1$ of $F'_E$ into $F''_E$ and a unique morphism $f_2$ of $F''_E$ into $F'_E$ such that $\varphi''_E=f_1\circ\varphi'_E$ and $\varphi'_E=f_2\circ\varphi''_E$. We have therefore $\varphi''_E=f_2\circ f_1\circ\varphi'_E$ and $\varphi'_E=f_1\circ f_2\circ\varphi''_E$. Applying $(AU)$ to the case where $F=F'_E$ and $\varphi=\varphi'_E$, we find that $f_2\circ f_1$ is the identity mapping of $F'_E$ onto itself. Similarly, $f_1\circ f_2$ is the identity mapping of $F''_E$ onto itself. Consequently (§ 2, no. 1, criterion CST8) $f_1$ is an *isomorphism* of $F'_E$ onto $F''_E$, and $f_2$ is its inverse isomorphism. This result is expressed by saying that the solution of the universal mapping problem for E is *unique up to isomorphism*.

To verify that a pair $(F_E,\varphi_E)$ is a solution of the universal mapping problem for E, it is often convenient to verify the following two conditions :

$(AU'_{\mathrm I})$ *For every $\Sigma$-set F and every $\alpha$-mapping $\varphi$ of E into F, there exists a morphism $f$ of $F_E$ into F such that $\varphi=f\circ\varphi_E$.*

$(AU'_{\mathrm{II}})$ *For every $\Sigma$-set F, two morphisms of $F_E$ into F which agree on $\varphi_E(E)$ are equal.*

For if these two conditions are satisfied, the morphism $f$ whose existence is ensured by $(AU'_{\mathrm I})$ is unique by $(AU'_{\mathrm{II}})$. Conversely, it is clear that $(AU)$ implies $(AU'_{\mathrm I})$; furthermore, if $f$ and $f'$ are two morphisms of $F_E$ into F which agree on $\varphi_E(E)$, we have $f\circ\varphi_E=f'\circ\varphi_E$, whence $f=f'$ by applying $(AU)$ to the $\alpha$-mapping $f\circ\varphi_E$. Hence $(AU)$ implies $(AU'_{\mathrm{II}})$.

### 2. EXISTENCE OF UNIVERSAL MAPPINGS

A universal mapping problem does not necessarily have a solution (Exercise 1). However, we shall show that the following conditions imply the existence of a solution :

$(CU_{\mathrm I})$ *On every product of a family of $\Sigma$-sets there exists a product structure of species $\Sigma$ (§ 2, no. 4).*

$(CU_{\mathrm{II})}$ *Let $(F_i)_{i\in I}$ be a family of $\Sigma$-sets, and for each $i\in I$ let $\varphi_i$ be an $\alpha$-mapping of E into $F_i$. Then the mapping $(\varphi_i)_{i\in I}$ of E into $\prod_{i\in I}F_i$ (endowed with the product structure) is an $\alpha$-mapping.*

A subset G of a $\Sigma$-set F will be said to be $\Sigma$-*admissible* if the structure on F induces a structure of species $\Sigma$ on G ($\S\,2$, no. 4).

$(\mathrm{CU_{III}})$ *There exists a cardinal* $\mathfrak{a}$ *with the following properties : for every* $\Sigma$-*set* F *and every* $\alpha$-*mapping* $\varphi$ *of* E *into* F *there exists a* $\Sigma$-*admissible subset* G *of* F *which contains* $\varphi(\mathrm{E})$, *has cardinal* $\leqslant \mathfrak{a}$, *is such that the mapping of* E *into* G *having the same graph as* $\varphi$ *is an* $\alpha$-*mapping, and such that any two morphisms of* G *into a* $\Sigma$-*set, which agree on* $\varphi(\mathrm{E})$, *are equal.*

CST22. *If the conditions* $(\mathrm{CU_I})$ *to* $(\mathrm{CU_{III}})$ *are satisfied, then the universal mapping problem for* E *has a solution.*

We shall first show that if there exists a pair $(\mathrm{F_E},\ \varphi_\mathrm{E})$ which satisfies $(\mathrm{AU'_I})$, then there also exists a solution of the universal mapping problem for E. For by $(\mathrm{CU_{III}})$ there exists a $\Sigma$-admissible subset $\mathrm{F'_E}$ of $\mathrm{F_E}$ containing $\varphi_\mathrm{E}(\mathrm{E})$, such that the mapping $\varphi'_\mathrm{E}$ of E into $\mathrm{F'_E}$ which has the same graph as $\varphi_\mathrm{E}$ is an $\alpha$-mapping, and such that any two morphisms of $\mathrm{F'_E}$ into a $\Sigma$-set which agree on $\varphi_\mathrm{E}(\mathrm{E})$ are equal. Let $j$ be the canonical injection of $\mathrm{F'_E}$ into $\mathrm{F_E}$, so that $\varphi_\mathrm{E} = j \circ \varphi'_\mathrm{E}$. For every morphism $f$ of $\mathrm{F_E}$ into a $\Sigma$-set F, $f \circ j$ is a morphism of $\mathrm{F'_E}$ into F, and we have $f \circ \varphi_\mathrm{E} = (f \circ j) \circ \varphi'_\mathrm{E}$. It is therefore clear that $(\mathrm{F'_E},\ \varphi'_\mathrm{E})$ satisfies $(\mathrm{AU'_I})$ and $(\mathrm{AU'_{II}})$.

It remains for us to establish the existence of a pair $(\mathrm{F_E},\ \varphi_\mathrm{E})$ satisfying $(\mathrm{AU'_I})$. Let $s \in \mathrm{S}(x)$ be the typical characterization of the species of structures $\Sigma$, and consider the subset L of $\mathfrak{P}(\mathfrak{a}) \times \mathrm{S}(\mathfrak{a}) \times \mathfrak{P}(\mathrm{E} \times \mathfrak{a})$ consisting of all triples $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P})$ having the following property : "V is a structure of species $\Sigma$ on $\mathrm{X} \subset \mathfrak{a}$, and P is the graph of an $\alpha$-mapping of E into X (with respect to the structure V)" (observe that we have $\mathrm{S}(\mathrm{X}) \subset \mathrm{S}(\mathfrak{a})$, as is easily seen by arguing step by step on the length of the echelon construction scheme S). For every $\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P}) \in \mathrm{L}$, we denote by $\mathrm{X}_\lambda$ the set X endowed with the structure V, and by $\varphi_\lambda$ the mapping of E into $\mathrm{X}_\lambda$ whose graph is P.

Let $\mathrm{F_E}$ be the $\Sigma$-set which is the product of the $\mathrm{X}_\lambda$ (it exists by $(\mathrm{CU_I})$), and let $\varphi_\mathrm{E}$ be the mapping $x \to (\varphi_\lambda(x))$ of E into $\mathrm{F_E}$, which is an $\alpha$-mapping by virtue of $(\mathrm{CU_{II}})$. Let us show that the pair $(\mathrm{F_E},\ \varphi_\mathrm{E})$ satisfies $(\mathrm{AU'_I})$. Given an $\alpha$-mapping $\varphi$ of E into a $\Sigma$-set F, let G be a subset of F which satisfies the conditions stated in $(\mathrm{CU_{III}})$. Let $j$ be the canonical injection of G into F, and let $\psi$ be the mapping of E into G which has the same graph as $\varphi$, so that $\varphi = j \circ \psi$. It follows from $(\mathrm{CU_{III}})$ that $\psi$ is an $\alpha$-mapping of E into G. Since Card (G) $\leqslant \mathfrak{a}$, there is a subset G$'$ of $\mathfrak{a}$ equipotent to G. Let $g$ be a bijection of G onto G$'$. If we transport by means of $g$ the structure of species $\Sigma$ on G, there exists by definition an element $\lambda$ of L such that G$'$ (endowed with the transported structure) is equal to $\mathrm{X}_\lambda$ and such that $g \circ \psi = \varphi_\lambda$. Then

$f = j \circ \overset{-1}{g} \circ \mathrm{pr}_\lambda$ is a morphism of $\mathrm{F_E}$ into F such that $\varphi = f \circ \varphi_\mathrm{E}$, and the proof is complete.

CST23. *Let* $(\mathrm{F_E},\ \varphi_\mathrm{E})$ *be a solution of the universal mapping problem for* E. *Then* $\varphi_\mathrm{E}$ *is an injection of* E *into* $\mathrm{F_E}$ *if and only if, for each pair of distinct elements* $x$, $y$ *of* E, *there exists an* $\alpha$-*mapping* $\varphi$ *of* E *into a* $\Sigma$-*set* F *such that* $\varphi(x) \neq \varphi(y)$.

Since $\varphi_\mathrm{E}$ is an $\alpha$-mapping, the criterion is an immediate consequence of the definitions.

¶ In this case the $\alpha$-mappings are said to *separate* the elements of E, and we do not ordinarily make any distinction, in the terminology, between the elements of E and their images under $\varphi_\mathrm{E}$. With this convention, if $(\mathrm{F_E},\ \varphi_\mathrm{E})$ is a solution of a universal mapping problem, and if condition $(\mathrm{CU_{III}})$ is satisfied, then every $\alpha$-mapping of E into a $\Sigma$-set F *extends uniquely to a morphism of* $\mathrm{F_E}$ *into* F.

### 3. EXAMPLES OF UNIVERSAL MAPPINGS

\* The examples which follow will, for the most part, be treated in detail elsewhere in this series.

I. *Free algebraic structures.* Let E be a set and let $\Sigma$ be a species of algebraic structures, defined by one or more laws of composition. We take as morphisms the *homomorphisms* for the species $\Sigma$ under consideration, and as $\alpha$-mappings *arbitrary* mappings of E into a $\Sigma$-set (in other words, $\alpha \{ x,\ s \} = \mathscr{F}(\mathrm{E},\ x)$). All the usual species of algebraic structures satisfy $(\mathrm{CU_{III}})$; with the exception of division ring structures, they also satisfy $(\mathrm{CU_I})$, and $(\mathrm{CU_{II}})$ is here a trivial consequence of $(\mathrm{CU_I})$.

Since in general there exist structures of species $\Sigma$ defined on sets with at least two elements, the $\alpha$-mappings separate the elements of E, and E may therefore be considered as embedded in $\mathrm{F_E}$. $\mathrm{F_E}$ is said to be the *free* $\Sigma$-*set generated by* E. Thus in algebra we speak of *free semigroups*, *free groups*, *free modules*, and *free algebras*.

II. *Rings and fields of fractions.* Let E be a commutative ring with an identity element and let S be a multiplicatively closed subset of E which does not contain 0. We take $\Sigma$ to be the species of structures of commutative rings with identity element, and the morphisms to be ring homomorphisms which transform identity element into identity element. The $\alpha$-mappings will be the homomorphisms $\varphi$ of E into a commutative ring A with an identity element, such that $\varphi(1) = 1$ and $\varphi(\mathrm{S})$ contains only *units* of A. The conditions $(\mathrm{QM_{II}})$, $(\mathrm{CU_I})$ throngh $(\mathrm{CU_{III}})$ (with $\mathfrak{a} = \mathrm{Card}\ (\mathrm{E})\ \mathrm{Card}\ (\mathbf{N})$) are immediately verified. The universal mapping problem therefore always has a solution $(\mathrm{F_E},\ \varphi_\mathrm{E})$, but in general $\varphi_\mathrm{E}$

is not injective. The most frequently arising case is that in which $E$ is an integral domain; in this case, $\varphi_E$ is injective. If, moreover, we take $S = E - \{0\}$, then $F_E$ is a field, called the *field of fractions* of $E$.

III. *Tensor product of two modules.* Let $E$ be the product $A \times B$ of two modules over a commutative ring $C$ which has an identity element. Take $\Sigma$ to be the species of $C$-module structures, the morphisms to be linear mappings, and the $\alpha$-mappings to be *bilinear* mappings of $A \times B$ into a $C$-module. The condition $(QM_{II})$ is evidently satisfied, and so are $(CU_I)$ through $(CU_{III})$ (with $\mathfrak{a} = \mathrm{Card}\ (E)\ \mathrm{Card}\ (C)\ \mathrm{Card}\ (\mathbf{N})$). The universal $C$-module $F_E$ corresponding to the pair $(A, B)$ is called the *tensor product* of $A$ and $B$ and is written $A \otimes B$. The universal mapping $\varphi_E$ is written $(x,\ y) \to x \otimes y$; it is bilinear but not, in general, injective.

IV. *Extension of the ring of operators of a module.* Let $A$ be a commutative ring with an identity element, let $B$ be a subring of $A$ containing the identity element of $A$, and let $E$ be a $B$-module. The species $\Sigma$ is the species of $A$-module structures, the morphisms are $A$-*linear* mappings, and the $\alpha$-mappings are the $B$-*linear* mappings of $E$ into an $A$-module. The universal $A$-module $F_E$ corresponding to the $B$-module $E$ is said to be obtained by *extending to* $A$ the ring of operators $B$ of $E$.

V. *Completion of a uniform space.* Let $E$ be a uniform space. Take $\Sigma$ to be the species of structures of complete Hausdorff uniform spaces, the morphisms to be uniformly continuous mappings, and the $\alpha$-mappings to be uniformly continuous mappings of $E$ into a complete Hausdorff uniform space. The $\Sigma$-admissible subsets of a complete Hausdorff uniform space are here the *closed* subsets (with respect to the topology of the space), and conditions $(QM_{II})$ and $(CU_I)$ through $(CU_{III})$ are satisfied (with $\mathfrak{a} = 2^{2^{\mathrm{Card}(E)}}$). The complete Hausdorff uniform space is (up to isomorphism) the *completion* of the Hausdorff uniform space associated with $E$ (*General Topology*, Chapter II, § 3, no. 7).

VI. *Stone-Čech compactification.* Let $E$ be a completely regular space. $\Sigma$ is the species of structures of compact spaces, the morphisms being continuous mappings (of a compact space into a compact space), and the $\alpha$-mappings are continuous mappings of $E$ into a compact space. The $\Sigma$-admissible subsets are again the *closed* subsets, and conditions $(QM_{II})$, $(CU_I)$ through $(CU_{III})$ are easily verified (with the same cardinal as in Example V). The compact space $F_E$ is (up to isomorphism) the "Stone-Čech compactification" obtained by completing $E$ with respect to the coarsest uniformity for which all the continuous mappings of $E$ into the interval $[0,\ 1]$ of $\mathbf{R}$ are uniformly continuous (*General Topology*, Chapter IX, § 1, Exercise 7); the mapping $\varphi_E$ is injective, because any

two distinct points of E can be separated by a continuous mapping of E into $[0, 1]$.

VII. *Free topological groups*. Let E be a completely regular space, let $\Sigma$ be the species of Hausdorff topological group structures, the morphisms being continuous homomorphisms; and take the $\alpha$-mappings to be the continuous mappings of E into a Hausdorff topological group. Conditions $(\mathrm{QM_{II}})$ and $(\mathrm{CU_I})$ to $(\mathrm{CU_{III}})$ are easily verified, with

$$\mathfrak{a} = \mathrm{Card\ (E)\ Card\ (\mathbf{N})}.$$

The Hausdorff topological group $\mathrm{F_E}$ which is the solution of this universal mapping problem for E is called the *free topological group generated by the space* E. Since any two distinct points of E can be separated by a continuous mapping of E into the Hausdorff topological group **R**, the mapping $\varphi_\mathrm{E}$ is injective; it can be shown that $\varphi_\mathrm{E}$ is a homeomorphism of E onto the subspace $\varphi_\mathrm{E}(\mathrm{E})$ of $\mathrm{F_E}$ [^1]. Instead of taking $\Sigma$ to be the species of structures of Hausdorff topological groups, we could also take other species of structures, such as those of Hausdorff topological abelian groups, compact groups, Hausdorff topological rings, Hausdorff topological vector spaces (over a topological division ring, considered as an auxiliary base set), etc.

VIII. *Almost periodic functions on a topological group*. Let E be a topological group. Take $\Sigma$ to be the species of compact group structures, the morphisms being continuous homomorphisms, and the $\alpha$-mappings being continuous homomorphisms of E into a compact group. Conditions $(\mathrm{QM_{II}})$, $(\mathrm{CU_I})$ through $(\mathrm{CU_{III}})$ are satisfied, with $\mathfrak{a} = 2^{2^{\mathrm{Card\,(E)}}}$. The compact group $\mathrm{F_E}$ which is the solution of this universal mapping problem for E is called the *compact group associated* with E; the mapping $\varphi_\mathrm{E}$ is not necessarily injective. Every continuous real-valued function on E, of the form $g \circ \varphi_\mathrm{E}$, where $g$ is a continuous real-valued function on E, is called an *almost periodic function* on E.

IX. *Albanese variety*. Let E be an algebraic variety, let $\Sigma$ be the species of structures of abelian varieties over the same base field as E (an abelian variety is a complete algebraic variety endowed with an algebraic group structure; it is necessarily commutative). The morphisms are rational mappings of one abelian variety into another (each morphism is necessarily the composition of a homomorphism and a translation). The $\alpha$-mappings are rational mappings of E into an abelian variety. Condition $(\mathrm{CU_I})$ is not satisfied, yet this universal mapping problem for E admits a solution $\mathrm{F_E}$, called the *Albanese variety* of E. In general, the rational mapping $\varphi_\mathrm{E}$ is not injective. ✳

### Exercises {#ens-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: See P. SAMUEL, "On universal mappings and free topological groups", *Bull. Amer. Math. Soc.*, **54** (1948), pp. 591-598.
