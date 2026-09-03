---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 1
section_title: Structures and isomorphisms
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 259-271, 289
pdf_pages: 0264-0276, 0294-0294
extraction: ocr
subsections:
    - "no": 1
      title: ECHELONS
      page: 259
      pdf_page: 264
    - "no": 2
      title: CANONICAL EXTENSIONS OF MAPPINGS
      page: 260
      pdf_page: 265
    - "no": 3
      title: TRANSPORTABLE RELATIONS
      page: 261
      pdf_page: 266
    - "no": 4
      title: SPECIES OF STRUCTURES
      page: 262
      pdf_page: 267
    - "no": 5
      title: ISOMORPHISMS AND TRANSPORT OF STRUCTURES
      page: 264
      pdf_page: 269
    - "no": 6
      title: DEDUCTION OF STRUCTURES
      page: 266
      pdf_page: 271
    - "no": 7
      title: EQUIVALENT SPECIES OF STRUCTURES
      page: 268
      pdf_page: 273
statements: 17
exercises: 1
content_sha256: dc6eca4ee1f30deffd779304c1cc6b07cc7d4bc2628cb62a2e8cac1082e1af75
---

## 1. STRUCTURES AND ISOMORPHISMS

The purpose of this chapter is to describe once and for all a certain number of formative constructions and proofs (cf. Chapter I, § 1, no. 3 and § 2, no. 2) which arise very frequently in mathematics.

### 1. ECHELONS

An *echelon construction scheme* is a sequence $c_1$, $c_2$, ..., $c_m$ of ordered pairs of natural integers [^1] $c_i = (a_i,\ b_i)$, satisfying the following conditions :

(a)　If $b_i = 0$, then $1 \leqslant a_i \leqslant i - 1$.
(b)　If $a_i \neq 0$ and $b_i \neq 0$, then $1 \leqslant a_i \leqslant i - 1$ and $1 \leqslant b_i \leqslant i - 1$.

These conditions imply that $c_1 = (0,\ b_1)$, with $b_1 > 0$. If $n$ is the largest of the integers $b_i$ which appear in the pairs $(0,\ b_i)$, then $c_1, c_2, ..., c_m$ is said to be an echelon construction scheme *on $n$ terms*.

Given an echelon construction scheme $\mathrm{S} = (c_1,\ c_2,\ \ldots,\ c_m)$ on $n$ terms, and given $n$ terms $\mathrm{E}_1$, $\mathrm{E}_2$, ..., $\mathrm{E}_n$ in a theory $\mathscr{T}$ which is stronger than the theory of sets, an *echelon construction of scheme* $\mathrm{S}$ *on* $\mathrm{E}_1$, ..., $\mathrm{E}_n$ is defined to be a sequence $\mathrm{A}_1$, $\mathrm{A}_2$, ..., $\mathrm{A}_m$ of $m$ terms in the theory $\mathscr{T}$, defined step by step by the following conditions :

(a)　If $c_i = (0,\ b_i)$, then $\mathrm{A}_i$ is the term $\mathrm{E}_{b_i}$.
(b)　If $c_i = (a_i,\ 0)$, then $\mathrm{A}_i$ is the term $\mathfrak{P}(\mathrm{A}_{a_i})$.
(c)　If $c_i = (a_i,\ b_i)$, where $a_i \neq 0$ and $b_i \neq 0$, then $\mathrm{A}_i$ is the term $\mathrm{A}_{a_i} \times \mathrm{A}_{b_i}$.

The last term $\mathrm{A}_m$ of the echelon construction of scheme S on $\mathrm{E}_1$, ..., $\mathrm{E}_n$ is called the *echelon of scheme* S *on the base sets* $\mathrm{E}_1$, ..., $\mathrm{E}_n$; in the general arguments which follow, it will be denoted by the notation $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n)$.

#### Example {#ens-iv-s1-n1-exa-1 .statement tag=03V4}

Given two sets E, F, the set $\mathfrak{P}(\mathfrak{P}(\mathrm{E})) \times \mathfrak{P}(\mathrm{F})$ is an echelon on E, F, with scheme

$$(0, 1), \quad (0, 2), \quad (1, 0), \quad (3, 0), \quad (2, 0), \quad (4, 5).$$

It is also the echelon on E, F with scheme

$$(0, 2), \quad (0, 1), \quad (1, 0), \quad (2, 0), \quad (4, 0), \quad (5, 3).$$

Distinct schemes may therefore give rise to the same echelon on the same terms.

### 2. CANONICAL EXTENSIONS OF MAPPINGS

Let $\mathrm{S} = (c_1, c_2, \ldots, c_m)$ be an echelon construction scheme on $n$ terms. Let $\mathrm{E}_1$, ..., $\mathrm{E}_n$, $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$ be sets (terms in $\mathscr{C}$) and let $f_1$, ..., $f_n$ be terms in $\mathscr{C}$ such that the relations "$f_i$ is a mapping of $\mathrm{E}_i$ into $\mathrm{E}'_i$" are theorems in $\mathscr{C}$ for $1 \leqslant i \leqslant n$. Let $\mathrm{A}_1$, ..., $\mathrm{A}_m$ (resp. $\mathrm{A}'_1$, ..., $\mathrm{A}'_m$) be the echelon construction of scheme S on $\mathrm{E}_1$, ..., $\mathrm{E}_n$ (resp. $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$). We define step by step a sequence of $m$ terms $g_1$, ..., $g_m$ such that $g_i$ is a *mapping of* $\mathrm{A}_i$ *into* $\mathrm{A}'_i$ (for $1 \leqslant i \leqslant m$) by the following conditions :

(a) If $c_i = (0, b_i)$, so that $\mathrm{A}_i = \mathrm{E}_{b_i}$ and $\mathrm{A}'_i = \mathrm{E}'_{b_i}$, then $g_i$ is the mapping $f_{b_i}$.

(b) If $c_i = (a_i, 0)$, so that $\mathrm{A}_i = \mathfrak{P}(\mathrm{A}_{a_i})$ and $\mathrm{A}'_i = \mathfrak{P}(\mathrm{A}'_{a_i})$, then $g_i$ is the *canonical extension* $\hat{g}_{a_i}$ of $g_{a_i}$ to sets of subsets (Chapter II, § 5, no. 1).

(c) If $c_i = (a_i, b_i)$, where $a_i \neq 0$ and $b_i \neq 0$, so that

$$\mathrm{A}_i = \mathrm{A}_{a_i} \times \mathrm{A}_{b_i} \qquad \text{and} \qquad \mathrm{A}'_i = \mathrm{A}'_{a_i} \times \mathrm{A}'_{b_i},$$

then $g_i$ is the *canonical extension* $g_{a_i} \times g_{b_i}$ of $g_{a_i}$ and $g_{b_i}$ to $\mathrm{A}_{a_i} \times \mathrm{A}_b$ (Chapter II, § 3, no. 9).

The last term $g_m$ of this sequence is called the *canonical extension, with scheme* S, *of the mappings* $f_1$, ..., $f_n$, and will be denoted by $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$.

¶ The following criteria can be verified step by step :

CST1. *If* $f_i$ *is a mapping of* $\mathrm{E}_i$ *into* $\mathrm{E}'_i$, *and if* $f'_i$ *is a mapping of* $\mathrm{E}'_i$ *into* $\mathrm{E}''_i$ *(*$1 \leqslant i \leqslant n$*), then for every echelon construction scheme* S *on* $n$ *terms we have*

$$\langle f'_1 \circ f_1, f'_2 \circ f_2, \ldots, f'_n \circ f_n \rangle^{\mathrm{S}} = \langle f'_1, f'_2, \ldots, f'_n \rangle^{\mathrm{S}} \circ \langle f_1, f_2, \ldots, f_n \rangle^{\mathrm{S}}.$$

CST2. *If $f_i$ is injective* (resp. *surjective*) *for* $1 \leqslant i \leqslant n$, *then* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ *is injective* (resp. *surjective*).

This criterion follows from the corresponding properties of the extension $\hat{g}$ (Chapter II, § 5, no. 1, Proposition 1) and the extension $g \times h$ (Chapter II, § 3, no. 9).

CST3. *If $f_i$ is a bijection of* $\mathrm{E}_i$ *onto* $\mathrm{E}'_i$, *and if $f_i^{-1}$ is the inverse bijection* [^2], *then* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ *is a bijection and* $\langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}$ *is its inverse; in other words*,

$$(\langle f_1, \ldots, f_n \rangle^{\mathrm{S}})^{-1} = \langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}.$$

This follows immediately from CST1 and CST2.

### 3. TRANSPORTABLE RELATIONS

Let $\mathscr{T}$ be a theory which is stronger than the theory of sets, let $x_1, \ldots, x_n$, $s_1, \ldots, s_p$ be distinct letters which are distinct from the constants of $\mathscr{T}$, and let $\mathrm{A}_1, \ldots, \mathrm{A}_m$ be terms in $\mathscr{T}$ in which none of the letters $x_i$ $(1 \leqslant i \leqslant n)$ and $s_j$ $(1 \leqslant j \leqslant p)$ appears. Let $\mathrm{S}_1, \ldots, \mathrm{S}_p$ be echelon construction schemes on $n + m$ terms. Then the relation $\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ :

"$s_1 \in \mathrm{S}_1(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ and $s_2 \in \mathrm{S}_2(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ and $\ldots$ and $s_p \in \mathrm{S}_p(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$"

is called a *typification* of the letters $s_1, \ldots, s_p$.

¶ Let $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ be a relation in $\mathscr{T}$ which contains certain of the letters $x_i$, $s_j$ (and possibly other letters as well). Then R is said to be *transportable* (*in* $\mathscr{T}$) *with respect to the typification* T, *the $x_i$ $(1 \leqslant i \leqslant n)$ being considered as principal base sets and the* $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$ *as auxiliary base sets*, if the following condition is satisfied : let $y_1, \ldots, y_n, f_1, \ldots, f_n$ be distinct letters which are distinct from the $x_i$ $(1 \leqslant i \leqslant n)$, the $s_j$ $(1 \leqslant j \leqslant p)$, the constants of $\mathscr{T}$, and all the letters which appear in R or in the terms $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$, and let $\mathrm{Id}_h$ $(1 \leqslant h \leqslant m)$ denote the identity mapping of $\mathrm{A}_h$ on to itself. Then the relation

(1)     "$\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ and ($f_1$ is a bijection of $x_1$ onto $y_1$) and $\ldots$ and ($f_n$ is a bijection of $x_n$ onto $y_n$)"

*implies, in* $\mathscr{T}$, *the relation*

(2)     $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\} \Leftrightarrow \mathrm{R}\{y_1, \ldots, y_n, s'_1, \ldots, s'_p\}$, where

$$(3) \qquad s'_j = \langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^s{}_j(s_j) \qquad (1 \leqslant j \leqslant p).$$

There is an analogous but simpler definition in the case where there is no auxiliary set.

For example, if $n = p = 2$ and if the typification T is "$s_1 \in x_1$ and $s_2 \in x_1$", the relation $s_1 = s_2$ is transportable. On the other hand, the relation $x_1 = x_2$ is not transportable.

### 4. SPECIES OF STRUCTURES

Let $\mathscr{T}$ be a theory which is stronger than the theory of sets. *A species of structures* in $\mathscr{T}$ is a text $\Sigma$ formed of the following assemblies :

(1)  a certain number of letters $x_1, \ldots, x_n, s$, distinct from each other and from the constants of $\mathscr{T}$; $x_1, \ldots, x_n$ are called the *principal base sets* of the species of structures $\Sigma$;

(2)  a certain number of terms $\mathrm{A}_1, \ldots, \mathrm{A}_m$ in $\mathscr{T}$ in which none of the letters $x_1, \ldots, x_n, s$ appears, and which are called the *auxiliary base sets* of $\Sigma$; $\Sigma$ possibly contains no auxiliary base sets (but it must contain at least one principal base set);

(3)  a typification $\mathrm{T}\{x_1, \ldots, x_n, s\}$ :

$$s \in \mathrm{S}(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m),$$

where S is an echelon construction scheme on $n + m$ terms (no. 1); $\mathrm{T}\{x_1, \ldots, x_n, s\}$ is called the *typical characterization* of the species of structures $\Sigma$;

(4)  a relation $\mathrm{R}\{x_1, \ldots, x_n, s\}$ which is *transportable* (in $\mathscr{T}$) with respect to the typification T, the $x_i$ being the principal base sets and the $\mathrm{A}_h$ the auxiliary base sets (no. 3); R is called the *axiom* of the species of structures $\Sigma$.

The theory $\mathscr{T}_\Sigma$ which has the same axiom schemes as $\mathscr{T}$ and whose explicit axioms are those of $\mathscr{T}$, together with the axiom "T and R", is called the *theory of the species of structures* $\Sigma$. The constants of $\mathscr{T}_\Sigma$ are therefore the constants of $\mathscr{T}$ and the letters which appear in T or in R.

¶ Let $\mathscr{T}'$ be a theory which is stronger than $\mathscr{T}$, and let $\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}$ be terms in $\mathscr{T}'$. In the theory $\mathscr{T}'$, U is said to be a *structure of species* $\Sigma$ *on the principal base sets* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, *with* $\mathrm{A}_1, \ldots, \mathrm{A}_m$ *as auxiliary base sets*, if the relation

$$\text{"}\mathrm{T}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\} \text{ and } \mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}\text{"}$$

is a *theorem in* $\mathscr{T}'$. When this is so, then for each theorem $\mathrm{B}\{x_1, \ldots, x_n, s\}$ in the theory $\mathscr{T}_\Sigma$ the relation $\mathrm{B}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}$ is a *theorem in* $\mathscr{T}'$ (Chapter I, § 2, no. 3). In $\mathscr{T}_\Sigma$, the constant $s$ is called the *generic structure of the species* $\Sigma$.

¶ In the theory $\mathscr{T}'$, the principal base sets $\mathrm{E}_1, \ldots, \mathrm{E}_n$ are said to be *endowed with the structure* $\mathrm{U}$. Clearly, $\mathrm{U}$ is an element of the set

$$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m).$$

The set of elements $\mathrm{V}$ of $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ which satisfy the relation $\mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{V}\}$ is therefore the *set of structures of the species* $\Sigma$ *on* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ (and it may be empty).

*Examples*

#### Example 1 {#ens-iv-s1-n4-exa-1 .statement tag=03V5}

Take $\mathscr{T}$ to be the theory of sets, and consider the species of structures which has no auxiliary base set, one principal base set $\mathrm{A}$, the typical characterization $s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$, and the axiom

$$s \circ s = s \quad \text{and} \quad s \cap \overset{-1}{s} = \Delta_{\mathbf{A}}$$

($\Delta_{\mathbf{A}}$ being the diagonal of $\mathrm{A} \times \mathrm{A}$), which is a transportable relation with respect to the typification $s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$, as is easily verified. It is clear that the theory of this species of structures is just the theory of *ordered sets* (Chapter III, §1, no. 3); and therefore the species of structure so defined is also called the *species of order structures* on $\mathrm{A}$. In Chapter III we saw many examples of sets endowed with structures of this species.

#### Example 2 {#ens-iv-s1-n4-exa-2 .statement tag=03V6}

Take $\mathscr{T}$ to be the theory of sets, and consider the species of structures which has no auxiliary base set, one principal base set $\mathrm{A}$, the typical characterization $\mathrm{F} \in \mathfrak{P}((\mathrm{A} \times \mathrm{A}) \times \mathrm{A})$, and as axiom the transportable relation "F is a functional graph whose domain is $\mathrm{A} \times \mathrm{A}$". The structures of this species are particular cases of what are called *algebraic structures*, and the function whose graph is $\mathrm{F}$ (a mapping of $\mathrm{A} \times \mathrm{A}$ into $\mathrm{A}$) is called *the* (*everywhere defined*) *internal law of composition* of such a structure.

#### Example 3 {#ens-iv-s1-n4-exa-3 .statement tag=03V7}

As before, let $\mathscr{T}$ be the theory of sets, and consider the species of structures which has no auxiliary base set, one principal base set $\mathrm{A}$, the typical characterization $\mathrm{V} \in \mathfrak{P}(\mathfrak{P}(\mathrm{A}))$, and as axiom the transportable relation

$$(\forall \mathrm{V}) \, ((\mathrm{V}' \subset \mathrm{V}) \Rightarrow ((\bigcup_{\mathrm{X} \in \mathrm{V}'} \mathrm{X}) \in \mathrm{V}))$$
$$\text{and} \quad (\forall \mathrm{X})(\forall \mathrm{Y})((\mathrm{X} \in \mathrm{V} \text{ and } \mathrm{Y} \in \mathrm{V}) \Rightarrow ((\mathrm{X} \cap \mathrm{Y}) \in \mathrm{V})).$$

This species of structures is called the *species of topological structures*. A structure of this species is also called a *topology*, and the relation $\mathrm{X} \in \mathrm{V}$ is expressed by saying that $\mathrm{X}$ is an *open set* in the topology $\mathrm{V}$ (*General Topology*, Chapter I, § 1).

#### Example 4 {#ens-iv-s1-n4-exa-4 .statement tag=03V8}

\* Take $\mathscr{T}$ to be the theory of the species of division ring structures, which has (among other things) a constant K as unique (principal) base set. The species of structure of a *left vector space over* K has K as auxiliary base set, a principal base set E, and as typical characterization the relation

$$V \in \mathfrak{P}((E \times E) \times E) \times \mathfrak{P}((K \times E) \times E)$$

(pr$_1$V being the graph of addition in E, and pr$_2$V the graph of scalar multiplication); we shall not state here the axiom for this species of structures.

#### Example 5 {#ens-iv-s1-n4-exa-5 .statement tag=03V9}

Again let $\mathscr{T}$ be the theory of sets; in this theory, the field $\mathbf{C}$ of complex numbers is a term which contains no letters. The species of structure of a *complex analytic manifold of dimension n* has $\mathbf{C}$ as auxiliary base set, and one principal base set V. We shall not indicate here the typical characterization or the axiom of this species of structure. \*

*Remarks*

#### Remark 1 {#ens-iv-s1-n4-rem-1 .statement tag=03VA}

In applications it is often the case (as in Example 4 above) that the echelon $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$ is a product of echelons

$$S_1(E_1, \ldots, A_m) \times \cdots \times S_p(E_1, \ldots, A_m).$$

If so, the letter $s$ in the definition of $\Sigma$ is often replaced by a "$p$-tuple" $(s_1, \ldots, s_p)$ (cf. Chapter II, § 2, no. 1).

Moreover, the axiom of a species of structures $\Sigma$ is most frequently written as a conjunction of several transportable relations (as in Example 3 above). These relations are called *the axioms* of the species $\Sigma$.

#### Remark 2 {#ens-iv-s1-n4-rem-2 .statement tag=03VB}

Names are given to the species of structures most frequently used in mathematics, and to sets endowed with structures of these species. Thus an *ordered set* (Chapter III, § 1) is a set endowed with an order structure (Example 1); \* in the later Books of this series, we shall define the notions of *group, field, topological space, differentiable manifold*, etc., all of which denote sets endowed with certain structures. \*

#### Remark 3 {#ens-iv-s1-n4-rem-3 .statement tag=03VC}

By abuse of language, in the theory of sets $\mathscr{T}$, the giving of $n$ distinct letters $x_1, \ldots, x_n$ (with no typical characterization and no axiom) is considered as a species of structure $\Sigma_0$, called the *structure of a set* on the $n$ principal base sets $x_1, \ldots, x_n$.

### 5. ISOMORPHISMS AND TRANSPORT OF STRUCTURES

Let $\Sigma$ be a species of structures in a theory $\mathscr{T}$, on $n$ principal base sets $x_1, \ldots, x_n$, with $m$ auxiliary base sets $A_1, \ldots, A_m$. Let S be the echelon construction scheme on $n + m$ letters which features in the typical characterization of $\Sigma$, and let R be the axiom of $\Sigma$. In a theory $\mathscr{T}'$ which is stronger than $\mathscr{T}$, let U be a structure of species $\Sigma$ on sets $E_1, \ldots, E_n$ (as principal base sets) and let U$'$ be a structure *of the same species* on sets $E'_1, \ldots, E'_n$. Finally, let $f_i$ (in $\mathscr{T}'$) be a *bijection* of $E_i$ onto $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$. Then $(f_1, \ldots, f_n)$ is said to be an *isomorphism* of the sets $\mathrm{E}_1, \ldots, \mathrm{E}_n$, endowed with the structure U, onto the sets $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, endowed with the structure $\mathrm{U}'$, if we have (in $\mathscr{C}'$)

(4) $$\langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}) = \mathrm{U}'$$

where $\mathrm{Id}_h$ denotes the identity mapping of $\mathrm{A}_h$ onto itself $(1 \leqslant h \leqslant m)$.

¶ Let $f'_i$ be the inverse of the bijection $f_i$ $(1 \leqslant i \leqslant n)$. It follows immediately from (4) and the criterion CST3 (no. 2) that we have

$$\langle f'_1, \ldots, f'_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}') = \mathrm{U}$$

and consequently that $(f'_1, \ldots, f'_n)$ is an *isomorphism* of $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, endowed with $\mathrm{U}'$, onto $\mathrm{E}_1, \ldots, \mathrm{E}_n$, endowed with U. The isomorphisms $(f_1, \ldots, f_n)$ and $(f'_1, \ldots, f'_n)$ are said to be *inverses* of each other.

$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, endowed with $\mathrm{U}'$, are said to be *isomorphic* to $\mathrm{E}_1, \ldots, \mathrm{E}_n$, endowed with U, if there exists an isomorphism of $\mathrm{E}_1, \ldots, \mathrm{E}_n$ onto $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$; in this case the structures U and $\mathrm{U}'$ are said to be *isomorphic*.

¶ The above definitions, together with CST1, imply the following criterion:

CST4. *Let* U, $\mathrm{U}'$, $\mathrm{U}''$ *be three structures of the same species* $\Sigma$ *on the principal base sets* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, $\mathrm{E}''_1, \ldots, \mathrm{E}''_n$, *respectively. Let* $f_i$ *be a bijection of* $\mathrm{E}_i$ *onto* $\mathrm{E}'_i$, *and let* $g_i$ *be a bijection of* $\mathrm{E}'_i$ *onto* $\mathrm{E}''_i$ $(1 \leqslant i \leqslant n)$. *If* $(f_1, \ldots, f_n)$ *and* $(g_1, \ldots, g_n)$ *are isomorphisms, then so is* $(g_1 \circ f_1, \ldots, g_n \circ f_n)$.

An isomorphism of $\mathrm{E}_1, \ldots, \mathrm{E}_n$ onto $\mathrm{E}_1, \ldots, \mathrm{E}_n$ (with respect to the *same* structure) is called an *automorphism* of $\mathrm{E}_1, \ldots, \mathrm{E}_n$. The composition of two automorphisms of $\mathrm{E}_1, \ldots, \mathrm{E}_n$ is an automorphism, and so is the inverse of an automorphism, \* so that the automorphisms of $\mathrm{E}_1, \ldots, \mathrm{E}_n$ form a *group*. \*

#### Remark {#ens-iv-s1-n5-rem-1 .statement tag=03VD}

By abuse of language, if $f_i$ is any bijection of $\mathrm{E}_i$ onto $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$, $(f_1, \ldots, f_n)$ is said to be an isomorphism of $\mathrm{E}_1, \ldots, \mathrm{E}_n$ onto $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ with respect to the species of structure of a set (no. 4, Remark 3).

CST5. *In a theory* $\mathscr{C}'$ *which is stronger than* $\mathscr{C}$, *let* U *be a structure of species* $\Sigma$ *on* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, *and let* $f_i$ *be a bijection of* $\mathrm{E}_i$ *onto a set* $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$. *Then there exists a unique structure of species* $\Sigma$ *on* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ *such that* $(f_1, \ldots, f_n)$ *is an isomorphism of* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ *onto* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$.

For this structure, if it exists, can only be the term $\mathrm{U}'$ defined by the relation (4); it remains to be verified that this term is indeed a structure of species $\Sigma$, i.e., that the relation $\mathrm{R}\{\mathrm{E}'_1, \ldots, \mathrm{E}'_n, \mathrm{U}'\}$ is true in $\mathscr{C}'$. But this follows from the fact that $\mathrm{R}\{x_1, \ldots, x_n, s\}$ is *transportable*, for

$R\{E'_1, \ldots, E'_n, U'\}$ is equivalent in $\mathscr{T}'$ to the relation $R\{E_1, \ldots, E_n, U\}$ (no. 3), which is true in $\mathscr{T}'$ by hypothesis.

¶ The structure $U'$ is said to be obtained by *transporting the structure* $U$ *to the sets* $E'_1, \ldots, E'_n$ *by means of the bijective mappings* $f_1, \ldots, f_n$. Thus two structures of the same species are isomorphic if and only if each is obtained from the other by transport of structure.

It may happen that *any* two structures of species $\Sigma$ are *necessarily isomorphic*; the species of structure $\Sigma$ is then said be *univalent*. \* This is the case for the structure of an infinite cyclic group (isomorphic to $\mathbf{Z}$), the structure of a prime field of characteristic zero (isomorphic to $\mathbf{Q}$), the structure of a complete Archimedean ordered field (isomorphic to $\mathbf{R}$), the structure of an algebraically closed, connected, locally compact topological field (isomorphic to $\mathbf{C}$), and of the structure of a non-commutative, connected, locally compact topological division ring (isomorphic to $\mathbf{H}$, the division ring of quaternions). For some of these species of structure, for example that of a prime field of characteristic zero, or that of a complete Archimedean ordered field, there is not even any automorphism other than the identity mapping; but there do exist such automorphisms for the other examples given above (for example, the symmetry $x \rightarrow -x$ in $\mathbf{Z}$). \*

It will be observed that the above species of structure are essentially those which are the basis of classical mathematics. On the other hand, \* the species of group structures, the species of structures of an ordered set, and the species of topological structures, are not univalent. \*

### 6. DEDUCTION OF STRUCTURES

Let $\Sigma$ be a species of structures in a theory $\mathscr{T}$, on $n$ principal base sets $x_1, \ldots, x_n$, with $m$ auxiliary base sets $A_1, \ldots, A_m$. Let $s$ be the generic structure of $\Sigma$, and let $T$ be an echelon construction scheme on $n + m$ terms. A term $V\{x_1, \ldots, x_n, s\}$ which contains no letter other than the constants of $\mathscr{T}_\Sigma$ is said to be *intrinsic* for $s$, of type $T(x_1, \ldots, x_n, A_1, \ldots, A_m)$, if it satisfies the following conditions :

(1) the relation $V\{x_1, \ldots, x_n, s\} \in T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ is a theorem in $\mathscr{T}_\Sigma$;

(2) let $\mathscr{T}'_\Sigma$ be the theory obtained by adjoining to the axioms of $\mathscr{T}_\Sigma$ the axioms "$f_i$ is a bijection of $x_i$ onto $y_i$" $(1 \leqslant i \leqslant n)$ (where the letters $y_i$ and $f_i$ are distinct from each other and from the constants of $\mathscr{T}_\Sigma$, for $1 \leqslant i \leqslant n$); if $s'$ is the structure obtained by transporting $s$ by means of $(f_1, \ldots, f_n)$ (no. 5), then

$$V\{y_1, \ldots, y_n, s'\} = \langle f_1, \ldots, f_n. \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{T}}(V\{x_1, \ldots, x_n, s\})$$

is a theorem in $\mathscr{T}'_\Sigma$.

Most of the terms which one is led to define in the theory of a species of structures are intrinsic terms.

¶ Let $\Theta$ be another species of structures in the theory $\mathscr{T}$, on $r$ principal base sets $u_1,\ldots,u_r$, with $p$ auxiliary base sets $B_1,\ldots,B_p$, and let $t\in T(u_1,\ldots,u_r,B_1,\ldots,B_p)$ be the typical characterization of $\Theta$ (no. 4). Then a system of $r+1$ terms $P,U_1,\ldots,U_r$, intrinsic for $s$, and such that $P$ is a structure of species $\Theta$ on $U_1,\ldots,U_r$, in the theory $\mathscr{T}_\Sigma$, is called a procedure of deduction of a structure of species $\Theta$ from a structure of species $\Sigma$. By abuse of language, the term $P$ alone is often called a procedure of deduction.

¶ Let $\mathscr{T}'$ be a theory stronger than $\mathscr{T}$. If $\mathscr{G}$ is a structure in $\mathscr{T}'$ of species $\Sigma$ on $E_1,\ldots,E_n$, then $P\{E_1,\ldots,E_n,\mathscr{G}\}$ is a structure of species $\Theta$ on the $r$ sets $F_j=U_j\{E_1,\ldots,E_n,\mathscr{G}\}$ $(1\leq j\leq r)$, said to be deduced from $\mathscr{G}$ by the procedure $P$, or subordinate to $\mathscr{G}$. The hypothesis that the terms $P,U_1,\ldots,U_r$ are intrinsic for $s$ moreover implies the following criterion:

**CST6.** Let $(g_1,\ldots,g_n)$ be an isomorphism of $E_1,\ldots,E_n$, endowed with a structure $\mathscr{G}$ of species $\Sigma$, onto $E'_1,\ldots,E'_n$, endowed with a structure $\mathscr{G}'$ of the same species. If $U_j$ is of type $\mathfrak{P}(T_j)$, put

$$
h_j=\langle g_1,\ldots,g_n,\mathrm{Id}_1,\ldots,\mathrm{Id}_{m}\rangle^{T_j}\quad(1\leq j\leq r),
$$

and let $F'_j=U_j\{E'_1,\ldots,E'_n,\mathscr{G}'\}$ $(1\leq j\leq r)$. Then $(h_1,\ldots,h_r)$ is an isomorphism of $F_1,\ldots,F_r$ onto $F'_1,\ldots,F'_r$ when these systems of sets are endowed with the structures of species $\Theta$ deduced from $\mathscr{G}$ and $\mathscr{G}'$ respectively by the procedure $P$.

It is clear that the terms $x_1,\ldots,x_n$ are intrinsic for $s$. In many cases, the terms $U_1,\ldots,U_r$ are certain of the letters $x_1,\ldots,x_n$; the structure of species $\Theta$ deduced from $s$ by the procedure $P$ is then said to be a structure underlying $s$.

*Examples*

#### Example 1 {#ens-iv-s1-n6-exa-1 .statement tag=03VE}

\* The species of topological group structures has a single principal base set $A$, no auxiliary base set, and the corresponding generic structure is a pair $(s_1,s_2)$ ($s_1$ being the graph of the law of composition on $A$, and $s_2$ the set of open sets in the topology of $A$; cf. General Topology, Chapter III, § 1). Each of the terms $s_1,s_2$ is a procedure of deduction and provides respectively the group structure and the topology underlying the topological group structure $(s_1,s_2)$.

Likewise, from a vector space structure can be deduced an underlying commutative group structure. From a ring structure can be deduced an underlying commutative group structure and a (multiplicative) semigroup

IV
STRUCTURES

structure. From the structure of a differentiable manifold can be deduced an underlying topology, etc.

#### Example 2 {#ens-iv-s1-n6-exa-2 .statement tag=03VF}

The species of vector space structures over $\mathbf{C}$ (resp. $\mathbf{R}$) has a principal base set $E$, an auxiliary base set equal to $\mathbf{C}$ (resp. $\mathbf{R}$), and typical characterization

$$
s_1\in\mathfrak{P}((E\times E)\times E)\qquad\text{and}\qquad s_2\in\mathfrak{P}((\mathbf{C}\times E)\times E)
$$

(resp. $s_1\in\mathfrak{P}((E\times E)\times E)$ and $s_2\in\mathfrak{P}((\mathbf{R}\times E)\times E)$).

The pair $(s_1,s_2\cap((\mathbf{R}\times E)\times E))$ is a procedure of deduction of a vector space structure over $\mathbf{R}$ from a vector space structure over $\mathbf{C}$ (“restriction of the field of scalars to $\mathbf{R}$”). \*

#### Example 3 {#ens-iv-s1-n6-exa-3 .statement tag=03VG}

Suppose that $\Theta$ has the same (principal and auxiliary) base sets as $\Sigma$, and the same typical characterization. If, moreover, the axiom of $\Sigma$ implies (in $\mathscr{T}$) the axiom of $\Theta$, it is clear that the term $s$ is a procedure of deduction of a structure of species $\Theta$ from a structure of species $\Sigma$. $\Theta$ is then said to be poorer than $\Sigma$, and $\Sigma$ is richer than $\Theta$. Every structure of species $\Sigma$, in a theory $\mathscr{T}'$ which is stronger than $\mathscr{T}$, is then also a structure of species $\Theta$. For example, the species of structures of totally ordered sets (obtained by taking as axiom the conjunction of the axiom of order structures (no. 4, Example 1) and the relation $s\cup s^{-1}=A\times A$) is richer than the species of order structures. \*The species of commutative group structures is richer than the species of group structures. The species of compact topological space structures is richer than the species of topological structures, etc. \*

#### Example 4 {#ens-iv-s1-n6-exa-4 .statement}

\* When each of $\Sigma$ and $\Theta$ is the species of group structures (resp. ring structures), there is defined in algebra a procedure of deduction which associates with each group structure (resp. ring structure) the group structure (resp. ring structure) on its centre. When $\Sigma$ is the species of vector space structures over a field $K$, and when $\Theta$ is the species of algebraic structures over $K$, there are defined procedures of deduction which associate with every vector space over $K$ its tensor algebra or its exterior algebra. We shall meet many other examples later in this series. \*

#### Remark {#ens-iv-s1-n6-rem-1 .statement tag=03VH}

When $P$ is a “q-tuple” $(P_1,\ldots,P_q)$, it is also said that the terms $P_1,\ldots,P_q$ constitute a procedure of deduction of a structure of species $\Theta$ from a structure of species $\Sigma$.

### 7. EQUIVALENT SPECIES OF STRUCTURES

Let $\Sigma$ and $\Theta$ be two species of structures, in the same theory $\mathscr{T}$, having the same principal base sets $x_1,\ldots,x_n$. Let $s,t$ be the generic structures of the species $\Sigma,\Theta$ respectively. Suppose that the following conditions are satisfied:

(1) We have a procedure of deduction $P\{x_1,\ldots,x_n,s\}$ of a structure of species $\Theta$ on $x_1,\ldots,x_n$ from a structure of species $\Sigma$ on $x_1,\ldots,x_n$.

(2) We have a procedure of deduction $Q\{x_1,\ldots,x_n,t\}$ of a structure of species $\Sigma$ on $x_1,\ldots,x_n$ from a structure of species $\Theta$ on $x_1,\ldots,x_n$.

(3) The relation $Q\{x_1,\ldots,x_n,P\{x_1,\ldots,x_n,s\}\}=s$ is a theorem in $\mathscr{T}_{\Sigma}$, and the relation $P\{x_1,\ldots,x_n,Q\{x_1,\ldots,x_n,t\}\}=t$ is a theorem in $\mathscr{T}_{\Theta}$.

The species of structures $\Sigma$ and $\Theta$ are then said to be equivalent by means of the procedures of deduction $P$ and $Q$. In this case, for every theorem $B\{x_1,\ldots,x_n,s\}$ in the theory $\mathscr{T}_{\Sigma}$, the relation $B\{x_1,\ldots,x_n,Q\}$ is a theorem in $\mathscr{T}_{\Theta}$; and conversely, for every theorem $C\{x_1,\ldots,x_n,t\}$ in the theory $\mathscr{T}_{\Theta}$, the relation $C\{x_1,\ldots,x_n,P\}$ is a theorem in $\mathscr{T}_{\Sigma}$.

☡

If $U$ is a structure of species $\Sigma$, the structure deduced from $U$ by the procedure $P$ is said to be equivalent to $U$. Criterion CST6 implies the following :

CST7. *Let $\mathscr{Y},\mathscr{Y}'$ be two structures of species $\Sigma$ on the principal base sets $(E_1,\ldots,E_n),(E'_1,\ldots,E'_n)$, respectively. Let $\mathscr{Y}_0,\mathscr{Y}'_0$ be structures of species $\Theta$ which are equivalent respectively to $\mathscr{Y}$ and $\mathscr{Y}'$. In order that $(g_1,\ldots,g_n)$ should be an isomorphism with respect to the structures $\mathscr{Y}_0$ and $\mathscr{Y}'_0$, it is necessary and sufficient that $(g_1,\ldots,g_n)$ should be an isomorphism with respect to the structures $\mathscr{Y}$ and $\mathscr{Y}'$.*

In practice, we make no distinction between the theories $\mathscr{T}_{\Sigma}$ and $\mathscr{T}_{\Theta}$ of two equivalent species of structures.

*Examples*

#### Example 1 {#ens-iv-s1-n7-exa-1 .statement tag=03VI}

\* Let $\Sigma$ be the species of commutative group structures; $\Sigma$ has a single (principal) base set $A$, and its generic structure consists of a single letter $F$; the typical characterization of $\Sigma$ is $F\in\mathscr{P}((A\times A)\times A)$, and we denote the axiom of $\Sigma$ by $R\{A,F\}$. This axiom implies in particular that $F$ is the graph of a function (the “law of composition” of the group; cf. no. 4, Example 2). In the theory $\mathscr{T}_{\Sigma}$ (where $\mathscr{T}$ denotes the theory of sets) we define a term $M\{A,F\}$ which is a functional graph in $\mathscr{P}((\mathbf{Z}\times A)\times A)$ and satisfies the following relation $B\{M,A,F\}$:

$$
(\forall x)(\forall y)(\forall n)((x\in A\ \text{and}\ y\in A\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(n,F(x,y))=F(M(n,x),M(n,y))))
$$

and

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m+n,x)=F(M(m,x),M(n,x))))
$$

and

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m,M(n,x))=M(mn,x)))
$$

and

$$
(\forall x)((x\in A)\Rightarrow (M(1,x)=x)).
$$

(“multiplication of an element of $A$ by an integer”).

Consider the species $\Theta$ of $\mathbf{Z}$-module structures, which has a single principal base set $A$, with $\mathbf{Z}$ as auxiliary set, and whose generic structure contains two letters G, L, with the typical characterization

$G \in \mathfrak{P}((A \times A) \times A)$ and $L \in \mathfrak{P}((\mathbf{Z} \times A) \times A)$

and the axiom

“$R \mid A, G$ and $(L$ is a functional graph) and $B \mid L, A, G$”.

It is immediately verified that the terms F, M constitute a procedure of deduction of a structure of species $\Theta$ from a structure of species $\Sigma$, and that the term G is a procedure of deduction of a structure of species $\Sigma$ from a structure of species $\Theta$. Furthermore, the condition (3) above is trivially satisfied. We may therefore say that the species of commutative group structures and the species of $\mathbf{Z}$-module structures are equivalent.

#### Example 2 {#ens-iv-s1-n7-exa-2 .statement tag=03VJ}

Let $\Sigma$ be the species of topological structures (no. 4, Example 3), let $A$ be the (principal) base set, and let $V$ be the generic structure of $\Sigma$. Consider the relation

$$x \in A \text{ and } X \subset A \text{ and } (\forall U)((U \in V \text{ and } x \in U) \Rightarrow (X \cap U \neq \varnothing)).$$

This relation has a graph $P \subset \mathfrak{P}(A) \times A$ with respect to the pair $(X, x)$; $P \mid A, V$ is a term called “the set of all pairs $(X, x)$ such that $x$ lies in the closure of $X$ with respect to the topology $V$”. We can then prove (cf. General Topology, Chapter I, § 1) that the following relations are theorems in $\mathscr{T}_{\Sigma}$:

$$P(\varnothing)=\varnothing,$$

$$(\forall Y)((Y \subset A) \Rightarrow (\forall Y \subset P(Y))),$$

$$(\forall Y)((Y \subset A) \Rightarrow (P(P(Y))=P(Y))),$$

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (P(Y \cup Z)=P(Y)\cup P(Z))).$$

Consider the species of structures $\Theta$, having a single (principal) base set $A$, whose generic structure consists of a single letter $W$, which has as typical characterization $W \in \mathfrak{P}(\mathfrak{P}(A) \times A)$ and as axiom

$$W(\varnothing)=\varnothing \text{ and } (\forall Y)((Y \subset A) \Rightarrow (Y \subset W(Y)))$$

and

$$(\forall Y)((Y \subset A) \Rightarrow (W(W(Y))=W(Y)))$$

and

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (W(Y \cup Z)=W(Y)\cup W(Z))).$$

Consider also the relation

$$U \subset A \text{ and } (\forall x)((x \in U) \Rightarrow x \notin W(A-U)).$$

The set of all $U \in \mathfrak{P}(A)$ which satisfy this relation is a subset $Q \mid A, W$ of $\mathfrak{P}(A)$. We can then prove (General Topology, Chapter I, § 1, Exercise 10) that the following relations are theorems in $\mathscr{T}_{\Theta}$:

$$A \in Q,$$

$$(\forall M)((M \subset Q) \Rightarrow ((\bigcup_{X \in M} X) \in Q)),$$

$$(\forall X)(\forall Y)((X \in Q \text{ and } Y \in Q) \Rightarrow ((X \cap Y) \in Q)).$$

Thus the terms $P\{A,V\}$ and $Q\{A,W\}$ satisfy conditions (1) and (2) above, and it is easily seen that they also satisfy condition (3). The species of structures $\Sigma$ and $\Theta$ are therefore equivalent, and we therefore consider every structure of species $\Theta$ as a topology, namely that which corresponds to it under the procedure of deduction $Q\{A,W\}$. \*

### Exercises {#ens-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: We use the notion of integer in the same manner as in Chapter I, that is to say, in the metamathematical sense of marks arranged in a certain order; this use has nothing to do with the mathematical theory of integers which was developed in Chapter III.
[^2]: For typographical reasons we write here $f^{-1}$ instead of $\overset{-1}{f}$.
