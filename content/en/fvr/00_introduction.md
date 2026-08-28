---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: en
source: fvr-i-vii
pdf_pages: 0016-0017
extraction: ocr
statements: 0
exercises: 0
content_sha256: 85e0ba02d9e87d1ef4af523569a61f14e491623624b2c9c740da85ac45ab1be5
---

## INTRODUCTION

The purpose of this Book is the elementary study of the infinitesimal properties of one real variable; the extension of these properties to functions of several real variables, or, all the more, to functions defined on more general spaces, will be treated only in later Books.

The results which we shall demonstrate will be useful above all in relation to (finite) real-valued functions of a real variable; but most of them extend without further argument to functions of a real variable taking values in a topological vector space over $\mathbf{R}$ (see below); as these functions occur frequently in Analysis we shall state for them all results which are not specific to real-valued functions.

The notion of a topological vector space, of which we have just spoken, is defined and studied in detail in Book V of this Series; but we do not need any of the results of Book V in this Book; some definitions, however, are needed, and we shall reproduce them below for the convenience of the reader.

We shall not repeat the definition of a vector space over a (commutative) field K (Alg., II, p. 193). $^1$ A topological vector space E over a topological field K is a vector space over K endowed with a topology such that the functions $x + y$ and $xt$ are continuous on $E \times E$ and $E \times K$ respectively; in particular, such a topology is compatible with the structure of the additive group of E. All topological vector spaces considered in this Book are implicitly assumed to be Hausdorff. When the topological group E is complete one says that the topological vector space E is complete. Every normed vector space over a valued field K (Gen. Top., IX, p. 169) $^2$ is a topological vector space over K.

Let E be a vector space (with or without a topology) over the real field $\mathbf{R}$; if x, y are arbitrary points in E the set of points $xt + y(1-t)$ where t runs through the closed

$^1$ The elements (or vectors) of a vector space E over a commutative field K will usually be denoted in this chapter by thick minuscules, and scalars by roman minuscules; most often we shall place the scalar t to the right in the product of a vector x by t, writing the product as $xt$; on occasion we will allow ourselves to use the left notation $tx$ in certain cases where it is more convenient; also, sometimes we shall write the product of the scalar $1/t$ ($t \neq 0$) and the vector x in the form $x/t$.

$^2$ We recall that a norm on E is a real function $\|x\|$ defined on E, taking finite non-negative values, such that the relation $\|x\| = 0$ is equivalent to $x = 0$ and such that

$$
\|x + y\| \leq \|x\| + \|y\| \quad \text{and} \quad \|xt\| = \|x\| \cdot |t|
$$

for all $t \in K$ ($|t|$ being the absolute value of $t$ in K).

segment [0, 1] of $\mathbf{R}$ is called the *closed segment* with endpoints $x, y$. One says that a subset $A$ of $E$ is *convex* if for any $x, y$ in $A$ the closed segment with endpoints $x$ and $y$ is contained in $A$. For example, an affine linear variety is convex; so is any closed segment; in $\mathbf{R}^n$ any parallelootope (*Gen. Top.*, VI, p. 34) is convex. Every intersection of convex sets is convex.

We say that a topological vector space $E$ over the field $\mathbf{R}$ is *locally convex* if the origin (and thus any point of $E$) has a fundamental system of *convex* neighbourhoods. Every *normed* space is locally convex; indeed, the balls $\|x\| \leq r \ (r > 0)$ form a fundamental system of neighbourhoods of 0 in $E$, and each of these is convex, for the relations $\|x\| \leq r,\ \|y\| \leq r$ imply that

$$
\|xt + y(1-t)\| \leq \|x\| t + \|y\| (1-t) \leq r
$$

for $0 \leq t \leq 1$.

Finally, a *topological algebra* $A$ over a (commutative) *topological field* $K$ is an algebra over $K$ endowed with a topology for which the functions $x + y,\ xy$ and $xt$ are continuous on $A \times A,\ A \times A$ and $A \times K$ respectively; when one endows $A$ only with its topology and vector space structure over $K$ then $A$ is a topological vector space. Every *normed algebra* over a *valued field* $K$ (*Gen. Top.*, IX, p. 175) is a topological algebra over $K$.
