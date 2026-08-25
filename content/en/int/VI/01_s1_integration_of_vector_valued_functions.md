---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 1
section_title: Integration of vector-valued functions
lang: en
source: int-i-vi
pdf_pages: 0392-0409, 0447-0453
extraction: ocr
subsections:
    - "no": 1
      title: Scalarly essentially integrable functions
      page: 2
      pdf_page: 393
    - "no": 2
      title: Properties of the integral of a scalarly essentially integrable function
      page: 5
      pdf_page: 396
    - "no": 3
      title: Integrals of operators
      page: 7
      pdf_page: 398
    - "no": 4
      title: The property (GDF)
      page: 9
      pdf_page: 400
    - "no": 5
      title: Measurable mappings and scalarly measurable mappings
      page: 12
      pdf_page: 403
    - "no": 6
      title: 'Applications: I. Extension of a continuous function to a space of measures'
      page: 13
      pdf_page: 404
    - "no": 7
      title: 'Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators'
      page: 15
      pdf_page: 406
statements: 34
exercises: 27
content_sha256: 700f5238b6835a0128f0c9da6a8c0df48ca0c3db61ed62e430c13385c23f98e2
---

## § 1. INTEGRATION OF VECTOR-VALUED FUNCTIONS

Throughout this section, $\mu$ denotes a positive measure on T, and F a Hausdorff locally convex vector space over $\mathbf{R}$. For every mapping f of T into F, and every element $z'$ of the dual $F'$ of F, we denote by $\langle f, z' \rangle$ or $\langle z', f \rangle$ the numerical function $z' \circ f$ on T. We shall say that f has a property $P$ *scalarly* if, for every $z' \in F'$, $\langle z', f \rangle$ has the property $P$. For example, we shall say that $f$ is *scalarly essentially $\mu$-integrable* if, for every $z' \in F'$, $\langle z', f \rangle$ is essentially $\mu$-integrable.\footnote{The special case $F = \mathcal{M}(X)$ ($X$ a locally compact space), equipped with the vague topology $\sigma(\mathcal{M}(X), \mathcal{K}(X))$, yields the concept of 'scalarly essentially $\mu$-integrable', for a mapping $f : T \to \mathcal{M}_+(X)$, defined in Ch. V, §3, No. 1.}

Note that in this definition, the topology of $F$ intervenes only through the intermediary of the dual $F'$ of $F$. If a function $f$ has the property $P$ scalarly, then it again has the property $P$ scalarly when the topology of $F$ is replaced by any Hausdorff locally convex topology compatible with the duality between $F$ and $F'$.

### 1. Scalarly essentially integrable functions

If $f$ is a scalarly essentially $\mu$-integrable mapping of $T$ into $F$, the mapping $z' \mapsto \int \langle f(t), z' \rangle d\mu(t)$ is a linear form on $F'$, that is, an element of the algebraic dual ${F'}^*$.

#### Definition 1 {#int-vi-s1-def-1 .statement}

*One calls* integral of $f$ with respect to $\mu$, *and denotes by* $\int f d\mu$ *or* $\int f(t) d\mu(t)$, *the element of* ${F'}^*$ *defined by*
$$
\left\langle z', \int f d\mu \right\rangle = \int \langle z', f \rangle d\mu
$$
*for all* $z' \in F'$.

If $f$ is continuous with compact support, it is scalarly integrable and Def. 1 coincides with the definition of the integral of $f$ given in Ch. III, §3, No. 1. On the other hand, if $F$ is a Banach space and $f$ is essentially integrable (Ch. V, §1, No. 3, Def. 3), then $f$ is scalarly essentially integrable and Def. 1 coincides with the definition of the integral of $f$ given in Chapter V (Ch. V, §1, No. 3 and Ch. IV, §4, No. 2, Cor. 1 of Th. 1).

#### Example {#int-vi-s1-n1-exa-1 .statement}

— Let $X$ be a locally compact space, $t \mapsto \lambda_t$ a mapping of $T$ into the space $\mathcal{M}(X)$ of measures on $X$. To say that the family $t \mapsto \lambda_t$ is $\mu$-adequate means that it consists of positive measures and that the mapping $t \mapsto \lambda_t$ is scalarly essentially $\mu$-integrable and $\mu$-measurable for the topology $\sigma(\mathcal{M}(X), \mathcal{K}(X))$.\footnote{This is the definition of 'µ-adequate' in the first edition of Chapter 5 (Ch. V, 1st edn., §3, No. 1, Def. 1). In the second edition, of which the preceding chapter is a translation, the term 'µ-adequate' defines a weaker (more general) concept (Ch. V, §3, No. 1, Def. 1); more precisely, a scalarly essentially $\mu$-integrable family $t \mapsto \lambda_t$ of positive measures is $\mu$-adequate in the sense of the first edition of Chapter V if and only if it is $\mu$-adequate in the sense of the second edition and is vaguely $\mu$-measurable, that is, $\mu$-measurable for $\sigma(\mathcal{M}(X), \mathcal{K}(X))$ (Ch. V, §3, No. 1, Prop 2 b)). The two definitions are equivalent whenever the topology of $X$ has a countable base (*ibid*. Prop. 2 c)), which is the case for the applications in Chapter VI (§3); consequently for the rest of the chapter, no distinction is made between the two interpretations of 'µ-adequate', and the references to the first edition of Ch. V have been replaced by their nearest equivalent in the second edition.}

integral with respect to $\mu$ is the measure that was denoted $\int \lambda_t\, d\mu(t)$ in Ch. V, §3, No. 1.

#### Remark 1 {#int-vi-s1-n1-rem-1 .statement}

If F is finite-dimensional, then every scalarly essentially integrable mapping of T into F is essentially integrable (Ch. V, §1, No. 3). However, in the general case, a scalarly negligible function on a compact space T may even fail to be $\mu$-measurable (Exer. 12).

#### Remark 2 {#int-vi-s1-n1-rem-2 .statement}

It is clear that the integral of f depends only on the class of f modulo the space of mappings of T into F that are scalarly locally $\mu$-negligible. Note that a scalarly locally negligible function g is not necessarily zero almost everywhere (Exer. 12). However, this is indeed the case when there exists in F' a sequence $(\mathbf{z}'_n)$ that is dense for the topology $\sigma(F', F)$: for, if $H_n$ is the locally negligible set of points $t \in T$ such that $\langle g(t), \mathbf{z}'_n \rangle \neq 0$, the union H of the $H_n$ is locally negligible and, for every $t \notin H$, one has $\langle g(t), \mathbf{z}'_n \rangle = 0$ for all n, whence $g(t) = 0$.

Let u be a continuous linear mapping of F into a Hausdorff locally convex space G; its transpose $^t u$ is a linear mapping of $G'$ into $F'$, and the (algebraic) transpose $^t(^t u)$ is a linear mapping of ${F'}^*$ into ${G'}^*$ that extends u, which we shall again denote by u. With this convention:

#### Proposition 1 {#int-vi-s1-prop-1 .statement}

— *If f is a mapping of T into F that is scalarly essentially $\mu$-integrable, then the mapping $u \circ f$ is scalarly essentially $\mu$-integrable and*
$$
\int (u \circ f)\, d\mu = u \left( \int f\, d\mu \right).
$$
For every $\mathbf{z}' \in G'$, $\langle \mathbf{z}', u \circ f \rangle = \langle ^t u(\mathbf{z}'), f \rangle$, whence the first assertion; the second follows from the formula
$$
\left\langle \mathbf{z}', \int (u \circ f)\, d\mu \right\rangle = \int \langle \mathbf{z}', u \circ f \rangle\, d\mu = \left\langle ^t u(\mathbf{z}'), \int f\, d\mu \right\rangle = \left\langle \mathbf{z}', u \left( \int f\, d\mu \right) \right\rangle.
$$

In particular, if f is scalarly essentially $\mu$-integrable, then it remains scalarly essentially $\mu$-integrable when the topology of F is replaced by a coarser topology.

#### Proposition 2 {#int-vi-s1-prop-2 .statement}

— *Let f be a scalarly essentially $\mu$-integrable mapping of T into F. For every numerical function $g \geqslant 0$ that is $\mu$-measurable and bounded, the mapping $t \mapsto g(t)f(t)$ (denoted gf or fg) of T into F is scalarly essentially $\mu$-integrable, f is scalarly essentially $(g \cdot \mu)$-integrable, and*
$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

This is an immediate consequence of the formula $\langle \mathbf{z}', gf \rangle = g \langle \mathbf{z}', f \rangle$, for all $\mathbf{z}' \in F'$, and the formula $\int h d(g \cdot \mu) = \int hg d\mu$ for every essentially $\mu$-integrable scalar function $h$ (Ch. V, §5, No. 3, Th. 1).

A great many propositions about essentially integrable numerical functions may be transposed word for word into propositions about scalarly essentially integrable vector-valued functions. Among the more important, we call attention to the conditions for a function to be essentially integrable with respect to a measure defined by a density (Ch. V, §5, No. 3, Th. 1), or with respect to the image of a measure (Ch. V, §6, No. 2, Th. 1), or with respect to an induced measure (Ch. V, §7, No. 1, Th. 1), or with respect to the sum of a summable family of positive measures (Ch. V, §2, No. 2, Props. 1 and 3 and Cor. 3 of Prop. 1). These transpositions are left to the reader.

However, to obtain statements corresponding to the theorems on 'double integrals' (Ch. V, §3, No. 3, Th. 1 and §8, No. 4, Th. 1 (Lebesgue–Fubini theorem)), it is necessary to strengthen the hypotheses (cf. Exer. 1); on applying the previously cited theorems to each of the functions $\langle \mathbf{z}', f \rangle$, where $\mathbf{z}' \in F'$, one thus obtains the following propositions:

#### Proposition 3 {#int-vi-s1-prop-3 .statement}

— Let $X$ be a locally compact space, $t \mapsto \lambda_t$ a $\mu$-adequate$^3$ family (Ch. V, §3, No. 1, Def. 1) of positive measures on $X$, and let $\nu = \int \lambda_t d\mu(t)$. Let $f$ be a mapping of $X$ into $F$; assume that $1^\circ$ $f$ is scalarly $\nu$-integrable; $2^\circ$ there exists a locally $\mu$-negligible set $N \subset T$ such that, for every $t \notin N$, $f$ is scalarly $\lambda_t$-integrable and $\int f d\lambda_t \in F$. Then, the function $t \mapsto \int f d\lambda_t$, defined for $t \notin N$, is scalarly essentially $\mu$-integrable, and$^4$

$$
\int f(x) d\nu(x) = \int d\mu(t) \int f(x) d\lambda_t(x) .
$$

#### Proposition 4 {#int-vi-s1-prop-4 .statement}

— Let $T$ and $T'$ be two locally compact spaces, $\mu$ (resp. $\mu'$) a positive measure on $T$ (resp. $T'$), $\nu = \mu \otimes \mu'$ the product measure on $X = T \times T'$. Let $f$ be a mapping of $X$ into $F$. Assume that: $1^\circ$ $f$ is scalarly $\nu$-integrable; $2^\circ$ there exists a locally $\mu$-negligible set $N \subset T$ such that, for every $t \notin N$, the mapping $t' \mapsto f(t, t')$ is scalarly $\mu'$-integrable, and $\int f(t, t') d\mu'(t') \in F$. Then, the function $t \mapsto \int f(t, t') d\mu'(t')$, defined for $t \notin N$, is scalarly essentially $\mu$-integrable and$^4$

$$
\iint f(t, t') d\mu(t) d\mu'(t') = \int d\mu(t) \int f(t, t') d\mu'(t') .
$$

$^3$It suffices to assume that the family is scalarly essentially $\mu$-integrable, thus the proposition holds for either of the two interpretations of ' $\mu$-adequate'.
$^4$Equality as elements of ${F'}^*$.

### 2. Properties of the integral of a scalarly essentially integrable function

#### Proposition 5 {#int-vi-s1-prop-5 .statement}

— Let $\mu$ be a bounded positive measure on $T$, $S$ a $\mu$-measurable set carrying $\mu$ (Ch. V, §5, No. 7, Def. 4), $f$ a scalarly $\mu$-integrable (*) function with values in $F$. Let $D$ be the closed convex envelope of $f(S)$ in the space $F'$* equipped with the topology $\sigma(F', F')$. Then $\int f\, d\mu \in \mu(T)D$.

Since $D$ is the intersection of the closed half-spaces containing $f(S)$ (TVS, II, §5, No. 3, Cor. 1 of Prop. 4), it suffices to prove that the relation $\langle f(t), z' \rangle \leq a$ for all $t \in S$ (where $z' \in F', a \in \mathbf{R}$) implies $\langle z', \int f\, d\mu \rangle \leq a \cdot \mu(T)$; but since $\int f\, d\mu = \int_S f\, d\mu$, this follows from Ch. IV, §4, No. 2, Cor. 1 of Th. 1.

#### Corollary {#int-vi-s1-n2-cor-1 .statement}

— Let $\mu$ be a bounded positive measure on $T$, $S$ a $\mu$-measurable set carrying $\mu$, and $f$ a mapping of $T$ into $F$, scalarly $\mu$-measurable and such that $f(S)$ is contained in a weakly compact convex subset $A$ of $F$. Then $f$ is scalarly $\mu$-integrable, and $\int f\, d\mu \in \mu(T)A \subset F$.

For every $z' \in F'$, $\langle z', f \rangle$ is $\mu$-measurable and bounded in $S$, hence integrable, which proves that $f$ is scalarly integrable. Moreover, since $A$ is compact in $F_\sigma$, it is closed in $F'$*, and the closed convex envelope of $f(S)$ in $F'$* is contained in $A$, whence the corollary.

#### Proposition 6 {#int-vi-s1-prop-6 .statement}

— Let $f$ be a scalarly essentially $\mu$-integrable function with values in $F$, such that $\int f\, d\mu \in F$. For every lower semi-continuous semi-norm $q$ on $F$,

$$
q\left( \int f\, d\mu \right) \leq \int^\bullet (q \circ f)\, d\mu .
$$

Let $D$ be the set of $z \in F$ such that $q(z) \leq 1$; $D$ is closed, convex, and contains $0$, therefore $D = D^{oo}$ (TVS, II, §6, No. 3, Cor. 3 of Th. 1). It therefore suffices to prove that for every $z' \in D^\circ$, one has $|\langle z', \int f\, d\mu \rangle| \leq \int^\bullet (q \circ f)\, d\mu$; but this follows at once from the fact that $|\langle z', f(t) \rangle| \leq q(f(t))$ for every $t \in T$.

Note that the numerical function $q \circ f$ need not be $\mu$-measurable (Exer. 12).

#### Proposition 7 {#int-vi-s1-prop-7 .statement}

— Let $f$ be a mapping of $T$ into $F$, scalarly essentially $\mu$-integrable, such that for every compact subset $K$ of $T$, $f(K)$ is contained

(*) Recall that for a *bounded* positive measure $\mu$, the concepts of $\mu$-integrable function and essentially $\mu$-integrable function are the same (Ch. V, §1, No. 3, Cor. of Prop. 9).

5 The original notation for upper essential integral is $\overline{\int^*}$, changed to $\int^\bullet$ in the second edition of Ch. V.

in a weakly compact, balanced, convex subset of F. Then $\int f d\mu$ belongs to the bidual $F''$ of F.

For every compact subset K of T,

$$
\int f \varphi_K d\mu = \int (f \varphi_K) d(\varphi_K \cdot \mu);
$$

the Cor. of Prop. 5 can be applied to the bounded measure $\varphi_K \cdot \mu$ and the function $f \varphi_K$, consequently $\int f \varphi_K d\mu \in F$. For every $z' \in F'$, $\langle z', f \rangle$ is essentially $\mu$-integrable, consequently (Ch. V, §1, No. 3, Prop. 10)

$$
\int \langle z', f \rangle d\mu = \lim_K \int \langle z', f \rangle \varphi_K d\mu,
$$

the limit being taken with respect to the increasing directed set of compact subsets of T. One concludes that, with respect to this set, $\int f \varphi_K d\mu$ converges to $\int f d\mu$ for the topology $\sigma({F'}^*, F')$. Now,

$$
\left| \left\langle z', \int f \varphi_K d\mu \right\rangle \right| = \left| \int \langle z', f \rangle \varphi_K d\mu \right| \leq \int |\langle z', f \rangle| d\mu,
$$

which proves that the set of elements $\int f \varphi_K d\mu$ is a *bounded* subset of $F_\sigma$, hence also of F (TVS, IV, §1, No. 1, Prop. 1). Proposition 7 is therefore a consequence of the following lemma:

#### Lemma 1 {#int-vi-s1-lem-1 .statement}

*The closure in ${F'}^*$ (for the topology $\sigma({F'}^*, F')$) of every bounded subset of F is contained in the bidual $F''$.*

For, a bounded subset of F is contained in the polar (in $F''$) of a neighborhood of 0 in the strong dual $F'$ of F, hence is relatively compact in $F''$ for $\sigma(F'', F')$ (TVS, III, §3, No. 5, Prop. 7 and No. 4, Cor. 2 of Prop. 4); since $\sigma(F'', F')$ is induced by $\sigma({F'}^*, F')$, the lemma is proved.

#### Corollary {#int-vi-s1-n2-cor-2 .statement}

*Suppose F is semi-reflexive, and let f be a scalarly essentially $\mu$-integrable mapping of T into F such that, for every compact subset K of T, $f(K)$ is bounded. Then $\int f d\mu$ belongs to F.*

For, every bounded subset of F is relatively weakly compact (TVS, IV, §2, No. 2, Th. 1), and $F = F''$.

#### Proposition 8 {#int-vi-s1-prop-8 .statement}

*Let $\mu$ be a bounded positive measure on T, S a $\mu$-measurable set carrying $\mu$, f a $\mu$-measurable mapping of T into F, such that $f(S)$ is contained in a complete, bounded, balanced convex subset B of F. Then, f is scalarly $\mu$-integrable and $\int f d\mu \in \mu(T)B \subset F$.*

Since S is $\mu$-integrable, there exists a partition of S formed by a $\mu$-negligible set N and a sequence $(K_n)$ of compact subsets such that the restriction of f to each $K_n$ is continuous (Ch. IV, §4, No. 6, Cor. 3 of Th. 4 and §5, No. 1, Def. 1); $f(K_n)$ is therefore a compact subset of $F$. The closed, balanced convex envelope $B_n$ of $f(K_n)$ is then pre-compact (TVS, II, §4, No. 1, Prop. 3) and is contained in the complete subset $B$ of $F$, therefore it is compact, and *a fortiori* weakly compact. Consequently (Cor. of Prop. 5) $f \varphi_{K_n}$ is scalarly $\mu$-integrable, and

$$
z_n = \int f \varphi_{K_n} d\mu \in \mu(K_n)B_n \subset \mu(K_n)B .
$$

For every continuous semi-norm $p$ on $F$, it follows that

$$
p(z_n) \leq \mu(K_n) \cdot \sup_{x \in B} p(x) ;
$$

since $B$ is bounded and since the series with general term $\mu(K_n)$ is convergent and has sum $\mu(T)$, one sees that the sequence with general term $s_n = z_1 + z_2 + \cdots + z_n$ is a Cauchy sequence in the complete subset $\mu(T)B$ of $F$. This sequence therefore converges to an element $s$ of $\mu(T)B$; since one can suppose that $f(t) = 0$ on $T - S$, Lebesgue’s theorem applied to each of the functions $\langle z', f \rangle$ ($z' \in F'$) proves that $s = \int f d\mu$.

### 3. Integrals of operators

Let $G$ and $H$ be two Hausdorff locally convex spaces over $\mathbf{R}$, and suppose now that $F$ is the space $\mathcal{L}(G; H)$ of continuous linear mappings of $G$ into $H$, equipped with the topology of *pointwise* convergence. Every continuous linear form on $F$ may be extended to a continuous linear form on the product space $H^G$ (TVS, II, §4, No. 1, Prop. 2), hence may be written $u \mapsto \sum_{i=1}^n \langle u(a_i), b'_i \rangle$, where the $a_i$ (resp. the $b'_i$) are elements of $G$ (resp. of the dual $H'$ of $H$). To say that a mapping $U$ of $T$ into $F$ is scalarly essentially $\mu$-integrable means that, for every $a \in G$ and every $b \in H'$, the numerical function $t \mapsto \langle U(t) \cdot a, b' \rangle$ is essentially $\mu$-integrable.

#### Proposition 9 {#int-vi-s1-prop-9 .statement}

*Let $U$ be a scalarly essentially $\mu$-integrable mapping of $T$ into $F = \mathcal{L}_s(G; H)$. In order that $\int U d\mu \in F$, it is necessary and sufficient that the following two conditions be satisfied:*

a) *For every $x \in G$, $\int (U(t) \cdot x) d\mu(t) \in H$.*

b) *For every equicontinuous subset $B'$ of $H'$, the set of linear forms $u_{y'} : x \mapsto \int \langle U(t) \cdot x, y' \rangle d\mu(t)$, where $y'$ runs over $B'$, is equicontinuous.*

The conditions a) and b) are necessary. For, since for every $x \in G$, the mapping $\tilde{x} : V \mapsto V \cdot x$ of $\mathcal{L}_s(G; H)$ into $H$ is linear, one sees (No. 1,

Prop. 1) that $\widetilde{\mathbf{x}} \circ U : t \mapsto U(t) \cdot \mathbf{x}$ is scalarly essentially $\mu$-integrable and that

$$
(1) \quad S \cdot \mathbf{x} = \int (U(t) \cdot \mathbf{x})\, d\mu(t),
$$

where $S = \int U\, d\mu \in \mathcal{L}_s(G; H)$. This proves a). Moreover, (1) may also be written

$$
(2) \quad \langle S \cdot \mathbf{x}, \mathbf{y}' \rangle = \int \langle U(t) \cdot \mathbf{x}, \mathbf{y}' \rangle\, d\mu(t) = \langle \mathbf{x}, u_{\mathbf{y}'} \rangle,
$$

in other words ${}^t S \cdot \mathbf{y}' = u_{\mathbf{y}'}$. Since $S$ is continuous, ${}^t S$ transforms every equicontinuous subset of $H'$ into an equicontinuous subset of $G'$, whence b).

Conversely, suppose a) and b) verified. By virtue of a), the formula (1) defines a linear mapping $S$ of $G$ into $H$, and, for every $\mathbf{y}' \in H'$, this mapping satisfies (2) (No. 1, Prop. 1); but then, condition (b) says that $S$ is continuous (TVS, II, §6, No. 4, Props. 5 and 6, and III, §3, No. 5, Prop. 7), therefore $S \in \mathcal{L}_s(G; H)$. Finally, formula (2) proves that $S = \int U\, d\mu$.

#### Corollary {#int-vi-s1-n3-cor-1 .statement}

— *The condition b) of Prop. 9 is satisfied in each of the following two cases*:

$1^\circ$ *The measure $\mu$ is bounded, and if $S$ is its support, then $U(S)$ is an equicontinuous subset of $\mathcal{L}(G; H)$*.

$2^\circ$ *The condition a) of Prop. 9 is satisfied, the space $G$ is barreled, and, for every compact subset $K$ of $T$, $U(K)$ is a bounded subset of $\mathcal{L}_s(G; H)$*.

Let us first place ourselves in case $1^\circ$. We can restrict ourselves to the case that $S = T$ (Ch. V, §7, No. 1, Th. 1). Then, for every equicontinuous subset $B'$ of $H'$, there exists an equicontinuous, convex, balanced and weakly closed subset $A' \subset G'$ such that ${}^t U(t) \cdot \mathbf{y}' \in A'$ for all $\mathbf{y}' \in B'$ and all $t \in T$ (TVS, II, §6, No. 4, Prop. 6). Since $U$ is scalarly $\mu$-integrable, the mapping $t \mapsto {}^t U(t) \cdot \mathbf{y}'$ of $T$ into the dual $G'$ of $G$ equipped with $\sigma(G', G)$, is scalarly $\mu$-integrable, and one may write

$$
u_{\mathbf{y}'} = \int ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t).
$$

Since $A'$ is convex and compact for $\sigma(G', G)$, the Cor. of Prop. 5 of No. 2 shows that $u_{\mathbf{y}'} \in \mu(T)A'$ for every $\mathbf{y}' \in B'$, which proves our assertion.

Let us now place ourselves in case $2^\circ$. For every $\mathbf{y}' \in H'$ and every compact subset $K$ of $T$, set

$$
u_{K, \mathbf{y}'} = \int \varphi_K(t) ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t),
$$

an element of the algebraic dual $G^*$ of $G$. Since $G$ is barreled, every bounded subset of $\mathcal{L}_s(G; H)$ is equicontinuous (TVS, III, §4, No. 2, Th. 1); the first part of the argument, applied to the function $\varphi_K U$ and the bounded measure $\varphi_K \cdot \mu$, shows that $u_{K, y'} \in G'$. Moreover, for the topology $\sigma(G^*, G)$, one has $u_{y'} = \lim_{K} = u_{K, y'}$, the limit being taken with respect to the increasing directed set of compact subsets of $T$ (Ch. V, §1, No. 3, Prop. 10). To verify condition b) of Prop. 9, it suffices, by Prop. 9, to prove that the linear mapping $S$ of $G$ into $H$ defined by (1) is continuous; moreover, $G$ is barreled, therefore it will suffice to prove that $S$ is continuous when $G$ and $H$ are equipped with their weakened topologies (TVS, IV, §1, No. 3, Prop. 7); finally, by virtue of (2), one is reduced to showing that $u_{y'} \in G'$ for every $y' \in H'$. Since $u_{y'}$ is in the closure, for $\sigma(G^*, G)$, of the set $M'$ of the $u_{K, y'}$, where $K$ runs over the set of compact subsets of $T$, it suffices to prove that $M'$ is equicontinuous (TVS, III, §3, No. 4, Prop. 4); and since $G$ is barreled, it comes to the same to say that for every $x \in G$, the set of $\langle x, u_{K, y'} \rangle$ is bounded (TVS, III, §4, No. 2, Th. 1). But this follows at once from the relations

$$
|\langle x, u_{K, y'} \rangle| = \left| \int \varphi_K(t) \langle U(t) \cdot x, y' \rangle d\mu(t) \right| \leq \int |\langle U(t) \cdot x, y' \rangle| d\mu(t).
$$

#### Proposition 10 {#int-vi-s1-prop-10 .statement}

— *Let $U$ be a mapping of $T$ into $F = \mathcal{L}_s(G; H)$. In each of the following three cases, $U$ is scalarly essentially $\mu$-integrable and $\int U d\mu \in \mathcal{L}_s(G; H)$:*

a) $H$ is quasi-complete, $\mu$ is bounded and, if $S$ is its support, $U$ is $\mu$-measurable and $U(S)$ is equicontinuous.

b) $H$ is semi-reflexive, $\mu$ is bounded and, if $S$ is its support, $U$ is scalarly $\mu$-measurable and $U(S)$ is equicontinuous.

c) $H$ is semi-reflexive, $G$ is barreled, $U$ is scalarly essentially $\mu$-integrable, and, for every compact subset $K$ of $T$, $U(K)$ is bounded.

The fact that $U$ is scalarly essentially integrable is obvious in all three cases; by virtue of Prop. 9 and its corollary, it suffices in each case to verify condition a) of Prop. 9. Now, this condition follows from Prop. 8 of No. 2 in the first case, and from the Cor. of Prop. 7 of No. 2 in the other two cases.

### 4. The property (GDF)

In this No. we are going to consider locally convex spaces $F$ having the following property (called the 'countably closed graph' property):⁶

⁶ *Graphe dénombrablement fermé*, whence the initials (GDF).

(GDF) *If u is a linear mapping of F into a Banach space B such that, in the product space F × B, every limit of every convergent sequence of points of the graph Γ of u again belongs to Γ, then u is continuous.*

Every Fréchet space has the property (GDF) (TVS, I, §3, No. 3, Cor. 5 of Th. 1). In the Appendix, we shall see other examples of spaces having the property (GDF).

#### Proposition 11 {#int-vi-s1-prop-11 .statement}

*Every Hausdorff locally convex space F with the property (GDF) is barreled.*

Let V be a barrel in F, q is gauge, which is a semi-norm on F; let H be the Hausdorff space associated with the space F equipped with the topology defined by this single semi-norm. The completion $\widehat{H}$ of H is a Banach space; let $\pi$ be the canonical mapping of F into $\widehat{H}$; we are going to show that $\pi$ is *continuous* (for the original topology on F); this will establish the proposition, because V, the inverse image under $\pi$ of the unit ball of $\widehat{H}$, will then be a neighborhood of 0 in F. To establish the continuity of $\pi$ it will suffice, by virtue of (GDF), to show that the graph of $\pi$ is *closed* in $F \times \widehat{H}$; in other words, we must see that if $\mathcal{F}$ is a filter on F, convergent to $x \in F$, and its image $\pi(\mathcal{F})$ converges to $y \in \widehat{H}$, then $y = \pi(x)$. Now, every element $x'$ of the polar $V^\circ$ of V in $F'$ may be extended in only one way to a continuous linear form on $\widehat{H}$ (again denoted $x'$), and the set of these forms is the unit ball of the dual of $\widehat{H}$; it therefore suffices to show that $\langle y, x' \rangle = \langle \pi(x), x' \rangle$ for every $x' \in V^\circ$. But this follows from the relations

$$
\langle y, x' \rangle = \lim_{\mathcal{F}} \langle \pi(z), x' \rangle = \lim_{\mathcal{F}} \langle z, x' \rangle = \langle x, x' \rangle = \langle \pi(x), x' \rangle .
$$

#### Theorem 1 {#int-vi-s1-thm-1 .statement}

(Gelfand–Dunford)—*Let F be a Hausdorff locally convex space having the property (GDF), $F'_s$ its weak dual. For every mapping f of T into $F'_s$ that is scalarly essentially $\mu$-integrable, the integral $\int f d\mu$ belongs to $F'$.*

Recall that the dual of $F'_s$ is F (TVS, II, §6, No. 2, Prop. 3). For every $z \in F$, the numerical function $\langle z, f \rangle$ is therefore essentially $\mu$-integrable; let $\theta(z)$ be its class in $L^1(\mu)$. To show that $\int f d\mu \in F'$, one must establish that the linear form $z \mapsto \langle z, \int f d\mu \rangle$ is continuous on F; in fact, we are going to prove the following stronger result:

#### Lemma 2 {#int-vi-s1-lem-2 .statement}

*Let f be a mapping of T into $F'_s$, such that for every $z \in F$, the numerical function $\langle z, f \rangle$ belongs to $\overline{\mathcal{L}}^p(\mu)$ ($1 \leq p \leq +\infty$); let $\theta(z)$ be the class of this function in $L^p(\mu)$. Then $z \mapsto \theta(z)$ is a continuous linear mapping of F into $L^p(\mu)$.*

By virtue of the (GDF) property, it suffices to show that for every sequence $(z_n)$ of elements of F converging to $z$, such that $(\theta(z_n))$ converges to $u \in L^p(\mu)$, one has $u = \theta(z)$. Now, replacing if necessary the sequence $(z_n)$ by a subsequence, one can suppose that the sequence of functions $\langle z_n, f \rangle$ converges locally almost everywhere to a function $h \in \overline{\mathcal{L}}^p(\mu)$, with class $u$ in $L^p(\mu)$ (Ch. IV, §3, No. 4, Th. 3 and Ch. V, §1, No. 3). Since, by hypothesis, for every $t \in T$ the sequence $(\langle z_n, f(t) \rangle)$ converges to $\langle z, f(t) \rangle$, we have $h(t) = \langle z, f(t) \rangle$ locally almost everywhere, consequently $u = \theta(z)$.

#### Corollary 1 {#int-vi-s1-lem-2-cor-1 .statement}

*Let $G_i$ ($1 \leq i \leq n$) be $n$ Hausdorff locally convex spaces having the property (GDF), and let $F$ be the space of separately continuous multilinear forms on $\prod_{i=1}^n G_i$, equipped with the topology of pointwise convergence. For every mapping $f$ of $T$ into $F$ that is scalarly essentially $\mu$-integrable, one has $\int f d\mu \in F$.*

The space $F$ is in duality with the tensor product $\bigotimes_{i=1}^n G_i$, and the topology of pointwise convergence on $F$ is none other than the topology $\sigma(F, \bigotimes_{i=1}^n G_i)$. The algebraic dual ${F'}^*$ is therefore the space of all multilinear forms on $\prod_{i=1}^n G_i$. Let $z = (z_1, \ldots, z_n)$ be an element of $\prod_{i=1}^n G_i$; for every multilinear form $u \in {F'}^*$, the mapping $x \mapsto u(z_1, \ldots, z_{i-1}, x, z_{i+1}, \ldots, z_n)$ is a linear form on $G_i$, which we shall denote by $\lambda_i(z)(u)$; we thus obtain a linear mapping $\lambda_i(z)$ of ${F'}^*$ into the algebraic dual $G_i^*$ of $G_i$, continuous for the topologies $\sigma({F'}^*, \bigotimes_{i=1}^n G_i)$ and $\sigma(G_i^*, G_i)$. To say that $u \in F$ means that for every index $i$ and every $z \in \prod_{i=1}^n G_i$, one has $\lambda_i(z)(u) \in G_i'$. Now, by Prop. 1 of No. 1, the mapping $\lambda_i(z)$ of $F$ is a scalarly essentially $\mu$-integrable mapping of $T$ into $G_i'$ equipped with the topology $\sigma(G_i', G_i)$, and
$$
\int (\lambda_i(z) \circ f) d\mu = \lambda_i(z) \left( \int f d\mu \right).
$$
By Th. 1, $\int (\lambda_i(z) \circ f) d\mu \in G_i'$ for $1 \leq i \leq n$, therefore $\int f d\mu \in F$.

#### Corollary 2 {#int-vi-s1-lem-2-cor-2 .statement}

*Let $G$ be a Hausdorff locally convex space having the property (GDF), and $H$ a semi-reflexive space whose strong dual $H_b'$ has the property (GDF) (cf. App., No. 2, Prop. 3). Let $F$ be the space $\mathcal{L}_s(G; H)$; for every mapping $U$ of $T$ into $F$ that is scalarly essentially $\mu$-integrable, the integral $\int U d\mu$ belongs to $F$.

Since $G$ is barreled (Prop. 11), $\mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$ (TVS, IV, §1, No. 3, Prop. 7); moreover, one can replace $F = \mathcal{L}_s(G; H)$ by the space $\mathcal{L}_s(G_\sigma; H_\sigma)$, since the two spaces have the same dual $G \otimes H'$ (TVS, II, §6, No. 2, Prop. 3, and the first paragraph of No. 3 above). If, for every $u \in \mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$, one sets $\tilde{u}(x, y') = \langle u(x, y') \rangle$ (for $x \in G$, y' \in H' ), the linear mapping $u \mapsto \tilde{u}$ is a bijection of F onto the space $F_1$ of separately continuous bilinear forms on $G_\sigma \times H'_s$, where $H'_s$ denotes the dual $H'$ equipped with the weak topology $\sigma(H', H)$ (App., No. 1); moreover, this mapping is an isomorphism of $\mathcal{L}_s(G_\sigma; H_\sigma)$ onto $F_1$ equipped with the topology of pointwise convergence (*loc. cit.*). But since by hypothesis H is the dual of $H'_b$, $F_1$ is also the space of separately continuous bilinear forms on $G \times H'_b$. Cor. 2 therefore follows from Cor. 1.

Note that Cor. 2 is applicable in particular when G is *Banach space* and H is a *reflexive Banach space*.

### 5. Measurable mappings and scalarly measurable mappings

If a mapping f of T into a Hausdorff locally convex space F is scalarly $\mu$-measurable, it does not in general follow that f is $\mu$-measurable (Exer. 12). Nevertheless:

#### Proposition 12 {#int-vi-s1-prop-12 .statement}

*If F is a separable, metrizable locally convex space, then every scalarly $\mu$-measurable mapping f of T into F is $\mu$-measurable.*

For, F may be regarded as a subspace of a countable product $\prod_n E_n$ of Banach spaces (TVS, II, §1, No. 3, Prop. 3), and one can suppose that $\mathrm{pr}_n(F)$ is dense in $E_n$, which is therefore separable. For every n, the mapping $\mathrm{pr}_n \circ f$ is scalarly $\mu$-measurable, hence $\mu$-measurable (Ch. IV, §5, No. 5, Cor. 2 of Prop. 10), consequently f is $\mu$-measurable (Ch. IV, §5, No. 3, Th. 1).

#### Proposition 13 {#int-vi-s1-prop-13 .statement}

*Let F be a locally convex space that is the direct limit of a sequence of separable, metrizable locally convex spaces $F_n$, F being the union of the $F_n$. Let $F'$ be the dual of F, equipped with the topology $\sigma(F', F)$. Then, every scalarly $\mu$-measurable mapping f of T into $F'$ is $\mu$-measurable.*

Suppose first that F is metrizable and separable, and let D be a countable dense set in F. Let $(V_n)$ be a decreasing fundamental sequence of balanced, convex, open neighborhoods of 0 in F; the polar sets $V_n^\circ$ are equicontinuous and their union is all of $F'$. Let $T_n = f(V_n^\circ)$; the sequence $(T_n)$ is increasing and $T = \bigcup T_n$; let us show that each of the $T_n$ is $\mu$-*measurable*. Indeed, $D \cap V_n^n$ is dense in $V_n$; for every $y \in D \cap V_n$, let $S_y$ be the set of $t \in T$ such that $|\langle y, f(t) \rangle| \leq 1$; the hypothesis implies that each of the $S_y$ is measurable, and $T_n$ is the intersection of the countable family of the $S_y$ ($y \in D \cap V_n$). This being so, for every compact subset K of T and every $\varepsilon > 0$, there exists an integer n such that $\mu(K - (K \cap T_n)) \leq \frac{\varepsilon}{4}$, then a compact subset $K_1$ of $K \cap T_n$ such that $\mu((K \cap T_n) - K_1) \leq \frac{\varepsilon}{4}$; finally, there exists a compact subset $K_2$ of $K_1$ such that $\mu(K_1 - K_2) \leq \frac{\varepsilon}{2}$ and such that the restrictions to $K_2$ of all of the functions $\langle y, f \rangle$, where $y \in D$, are continuous (Ch. IV, §5, No. 1, Prop. 2). Since the set $f(K_2) \subset f(T_n) \subset V_n^\circ$ is equicontinuous, the topology induced by $\sigma(F', F)$ on $f(K_2)$ is identical to the topology of pointwise convergence in $D$ (GT, X, §2, No. 4, Th. 1); consequently, the restriction of $f$ to $K_2$ is continuous, whence our assertion in the first case.

Let us pass to the general case. If $z'$ is a continuous linear form on $F$, its restriction $z'_n$ to $F_n$ is continuous; since $F = \bigcup_n F_n$, the dual $F'$ of $F$ may be identified (algebraically) with a linear subspace of the product $\prod_n F'_n$, and $\operatorname{pr}_n z' = z'_n$. Moreover, since each finite subset of $F$ is contained in one of the $F_n$, the topology $\sigma(F', F)$ is none other than the topology induced by the product topology of the topologies $\sigma(F'_n, F_n)$. This being so, if $f$ is scalarly $\mu$-measurable then $\operatorname{pr}_n \circ f$ is scalarly $\mu$-measurable, since for every $t \in T$, $\operatorname{pr}_n(f(t))$ is the restriction of $f(t)$ to $F_n$. The first part of the proof shows that $\operatorname{pr}_n \circ f$ is $\mu$-measurable for every $n$, therefore so is $f$ (Ch. IV, §5, No. 3, Th. 1).

### 6. Applications: I. Extension of a continuous function to a space of measures

Let $T$ be a locally compact space, $F$ a quasi-complete, Hausdorff locally convex space, and $f$ a continuous mapping of $T$ into $F$; if $\mu$ is a positive measure on $T$, with compact support $S$, then $f(S)$ is compact; the closed convex envelope of $f(S)$ is then compact (TVS, III, §1, No. 6), therefore $f$ is scalarly $\mu$-integrable and $\int f \, d\mu \in F$ (No. 2, Cor. of Prop. 5). If now $\lambda$ is any real measure with compact support, $\lambda^+$ and $\lambda^-$ are positive measures with compact support; setting $\int f \, d\lambda = \int f \, d\lambda^+ - \int f \, d\lambda^-$, one verifies immediately (using the relation $(\lambda + \mu)^+ + \lambda^- + \mu^- = \lambda^+ + \mu^+ + (\lambda + \mu)^-$) that $\lambda \mapsto \int f \, d\lambda$ is a linear mapping of the space $\mathcal{C}'(T)$ of measures on $T$ with compact support, into the locally convex space $F$.

Let us now observe that the space $\mathcal{C}'(T)$ may be identified with the dual of the space $\mathcal{C}(T)$ of continuous numerical functions on $T$ (whence its notation), when $\mathcal{C}(T)$ is equipped with the topology of compact convergence (which we shall always assume in this No. and in the following one): for, it is known on the one hand (Ch. IV, §4, No. 8, Prop. 14) that the measures on $T$ that can be extended to continuous linear forms on $\mathcal{C}(T)$ are the measures with compact support, and conversely, the restriction to $\mathcal{K}(T)$ of a continuous linear form on $\mathcal{C}(T)$ is a measure (since the topology of $\mathcal{K}(T)$ is finer than the one induced by the topology of $\mathcal{C}(T)$).

#### Proposition 14 {#int-vi-s1-prop-14 .statement}

*Let T be a locally compact space, F a quasi-complete, Hausdorff locally convex space, and f a continuous mapping of T into F. If the space $\mathcal{C}'(T)$ of measures on T with compact support is equipped with the topology of uniform convergence in the compact subsets of $\mathcal{C}(T)$, then the mapping $\lambda \mapsto \int f d\lambda$ is the unique continuous linear mapping $\tilde{f}$ of $\mathcal{C}'(T)$ into F such that $\tilde{f}(\varepsilon_t) = f(t)$ for every $t \in T$.*

To establish the uniqueness of the extension, it suffices to see that the point measures $\varepsilon_t$ form a total set in $\mathcal{C}'(T)$; since the dual of $\mathcal{C}'(T)$ is $\mathcal{C}(T)$ (TVS, IV, §1, No. 1, Th. 1), it suffices to observe that every function $g \in \mathcal{C}(T)$ that is orthogonal to all of the measures $\varepsilon_t$ is equal to 0 by definition (TVS, IV, §1, No. 2, Prop. 2).

Let us now show that $\lambda \mapsto \int f d\lambda$ is continuous. Let V be a closed, balanced convex neighborhood of 0 in F; it suffices to prove that there exists a relatively compact subset L of $\mathcal{C}(T)$ such that the relations $\lambda \in L^\circ$ and $z' \in V^\circ$ imply $|\langle \int f d\lambda, z' \rangle| \leq 1$, or again that $|\int \langle f, z' \rangle d\lambda| \leq 1$. To this end, we are going to show that as $z'$ runs over $V^\circ$, the set L of numerical functions $\langle f, z' \rangle$ is relatively compact in $\mathcal{C}(T)$. Since $V^\circ$ is bounded for $\sigma(F', F)$, the supremum of the numbers $|\langle f(t), z' \rangle|$, for $t \in T$ fixed and $z'$ running over $V^\circ$, is finite; by virtue of Ascoli’s theorem (GT, X, §2, No. 5, Cor. 2 of Th. 2), it therefore suffices to show that the set of $\langle f, z' \rangle$ ($z' \in V^\circ$) is *equicontinuous*. But, for every $t_0 \in T$ and every $\delta > 0$, there exists by hypothesis a neighborhood W of $t_0$ in T such that $f(t) - f(t_0) \in \delta V$ for all $t \in W$; it follows that $|\langle f(t), z' \rangle - \langle f(t_0), z' \rangle| \leq \delta$ for all $t \in W$ and all $z' \in V^\circ$, which completes the proof.

#### Remark {#int-vi-s1-n6-rem-1 .statement}

— 1) The mapping $t \mapsto \varepsilon_t$ is a *homeomorphism* of T into the space $\mathcal{C}'(T)$; for, if L is a compact subset of $\mathcal{C}(T)$, and $t_0 \in T$, there exists (GT, X, §2, No. 5, Cor. 3 of Th. 2) a neighborhood W of $t_0$ such that $|g(t) - g(t_0)| \leq 1$ for every $t \in W$ and every function $g \in L$, therefore $\varepsilon_t - \varepsilon_{t_0} \in L^\circ$ for $t \in W$, which proves the continuity of $t \mapsto \varepsilon_t$ (cf. Ch. IV, §4, No. 8, Prop. 15); one knows in addition that the inverse mapping is already continuous for the vague topology (Ch. III, §1, No. 9, Prop. 13), hence *a fortiori* for the topology of uniform convergence in the compact subset of $\mathcal{C}(T)$. If one then identifies T with its image in $\mathcal{C}'(T)$ via $t \mapsto \varepsilon_t$, one can say that $\lambda \mapsto \int f d\lambda$ is the unique *continuous extension* of f to a *linear* mapping.

2) Note that in the proof of the continuity of $\lambda \mapsto \int f d\lambda$, we have not used the fact that F is quasi-complete. The conclusion of Prop. 14 is therefore still valid without this hypothesis, provided one knows in addition that $\int f d\mu \in F$ for every positive measure $\mu$ with compact support.

Suppose now that $f(T)$ is a *bounded* subset of F. Then, for every *bounded* positive measure $\mu$ on T, f is scalarly $\mu$-integrable and $\int f d\mu \in F$

(No. 2, Prop. 8). If $\lambda$ is any bounded real measure on $T$, then $\lambda^+$ and $\lambda^-$ are bounded, and one sees immediately that $\lambda \mapsto \int f\, d\lambda$, defined as above, is a *linear* mapping of the space $\mathcal{M}^1(T)$ of *bounded* measures on $T$, into the locally convex space $F$, that obviously extends the mapping $\lambda \mapsto \int f\, d\lambda$ of $\mathcal{C}'(T)$ into $F$.

#### Proposition 15 {#int-vi-s1-prop-15 .statement}

*Let $T$ be a locally compact space, $F$ a Hausdorff locally convex space that is quasi-complete, and $f$ a continuous mapping of $T$ into $F$ such that $f(T)$ is bounded. If $\mathcal{M}^1(T)$ is equipped with its Banach space topology, then the linear mapping $\lambda \mapsto \int f\, d\lambda$ of $\mathcal{M}^1(T)$ into $F$ is continuous.*

For every closed, balanced, convex neighborhood $V$ of 0 in $F$, there exists a $\rho > 0$ such that $f(T) \subset \rho V$; the closed, balanced, convex envelope $B$ of $f(T)$ is therefore contained in $\rho V$, and it is complete by hypothesis. If then $\| \lambda \| \leq 1/\rho$, it follows from No. 2, Prop. 8, and the relation $\| \lambda \| = \lambda^+(T) + \lambda^-(T)$, that $\int f\, d\lambda \in B/\rho \subset V$.

### 7. Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators

Let $G$ be a Hausdorff locally convex space, $H$ a Hausdorff and quasi-complete locally convex space, and denote by $F$ the space $\mathcal{L}(G; H)$ of continuous linear mappings of $G$ into $H$, equipped with the topology of *compact convergence*. The space $F$ is not necessarily quasi-complete, and if $t \mapsto U(t)$ is a continuous mapping of $T$ into $F$, and $\mu$ is a positive measure on $T$ with compact support, one does not necessarily have $\int U\, d\mu \in F$ (Exer. 27). However, if, for every compact subset $K$ of $T$, $U(K)$ is *equicontinuous*, then its balanced convex envelope in $F$ is also equicontinuous (TVS, III, §3, No. 4), and since $H$ is quasi-complete, the closure of this balanced convex envelope will be a complete subset of $F$ (TVS, III, §3, No. 8, Prop. 11); one will then indeed have $\int U\, d\mu \in F$ (No. 2, Prop. 8).

The supplementary condition imposed on $U$ may be expressed otherwise:

#### Lemma 3 {#int-vi-s1-lem-3 .statement}

*Let $G, H$ be two locally convex spaces, $U$ a mapping of a locally compact space $T$ into $\mathcal{L}(G; H)$. The following conditions are equivalent:
a) The mapping $(t, x) \mapsto U(t) \cdot x$ of $T \times G$ into $H$ is continuous.
b) For every compact subset $K$ of $T$, $U(K)$ is equicontinuous, and there exists a total set $D \subset G$ such that for every $x \in D$, the mapping $t \mapsto U(t) \cdot x$ is continuous on $T$.*

Moreover, when $U$ satisfies these conditions, $U$ is a continuous mapping of $T$ into $\mathcal{L}(G; H)$ equipped with the topology of compact convergence.

To see that a) implies b), we observe that for every neighborhood $V$ of 0 in $H$ and every $t \in K$, there exist by hypothesis a neighborhood $L_t$ of $t$ in $T$ and a neighborhood $W_t$ of 0 in $G$ such that the relations $t' \in L_t$ and $x \in W_t$ imply $U(t') \cdot x \in V$. It suffices to cover $K$ with a finite number of neighborhoods $L_{t_i}$ and to take $W = \bigcap_i W_{t_i}$ in order to have $U(t) \cdot x \in V$ whenever $t \in K$ and $x \in W$, which proves the equicontinuity of $U(K)$.

Conversely, suppose b) is verified; it suffices to show that for every compact subset $K$ of $T$, the mapping $(t, x) \mapsto U(t) \cdot x$ is continuous on $K \times G$. Let $M = U(K)$; since $M$ is equicontinuous, it follows that on $M$, the topology of pointwise convergence in $G$ is identical to the topology of pointwise convergence in $D$ (GT, X, §2, No. 4, Th. 1); the hypothesis b) therefore implies that $t \mapsto U(t)$ is a continuous mapping of $K$ into $\mathcal{L}(G; H)$ when $\mathcal{L}(G; H)$ is equipped with the topology of pointwise convergence. On the other hand, $(A, x) \mapsto A \cdot x$ is a continuous mapping of $M \times G$ into $H$ when $M$ is equipped with the topology of pointwise convergence (GT, X, §2, No. 1, Cor. 4 of Prop. 1). Since the mapping $(t, x) \mapsto U(t) \cdot x$ may be factored as $(t, x) \mapsto (U(t), x) \mapsto U(t) \cdot x$, we conclude that it is continuous.

Finally, the last assertion of the lemma follows from the fact that, on $M$, the topology of compact convergence is identical to that of pointwise convergence (GT, X, §2, No. 4, Th. 1).

Thus, suppose that $U$ satisfies the conditions of Lemma 3; then (if $H$ is quasi-complete) one defines, as in No. 6, a linear mapping $\lambda \mapsto \int U d\lambda$ of $\mathcal{C}'(T)$ into $F = \mathcal{L}(G; H)$. We set $U(\lambda) = \int U d\lambda$.

#### Proposition 16 {#int-vi-s1-prop-16 .statement}

— Let $G, H$ be two Hausdorff locally convex spaces, with $H$ assumed to be quasi-complete. Let $U$ be a mapping of $T$ into $\mathcal{L}(G; H)$ such that $(t, x) \mapsto U(t) \cdot x$ is a continuous mapping of $T \times G$ into $H$. Then the bilinear mapping $(\lambda, x) \mapsto U(\lambda) \cdot x$ of $\mathcal{C}'(T) \times G$ into $H$ is hypocontinuous relative to the equicontinuous subsets of $\mathcal{C}'(T)$ and the compact subsets of $G$ (which implies that the linear mapping $\lambda \mapsto U(\lambda)$ of $\mathcal{C}'(T)$ into $F$ is continuous).

The continuity of $\lambda \mapsto U(t)$ as a mapping of $\mathcal{C}'(T)$ into $F$ follows from Lemma 3 and Remark 2 following Prop. 14 of No. 6. Thus, it remains to prove that for every closed, balanced, convex neighborhood $V$ of 0 in $H$ and for every equicontinuous subset $N$ of $\mathcal{C}'(T)$, there exists a neighborhood $W$ of 0 in $G$ such that the relations $x \in W, \lambda \in N$ imply that $U(\lambda) \cdot x \in V$. One can suppose that $N = S^\circ$, where $S$ is a neighborhood of 0 in $\mathcal{C}(T)$, consequently one can suppose that $S$ is the set of functions $g \in \mathcal{C}(T)$ such that $|g(t)| \leq 1$ on a compact subset $K$ of $T$. It suffices to show that

|⟨U(λ) · x, x′⟩| ≤ 1 for x ∈ W, x′ ∈ V° and λ ∈ S°. Now, since U(K) is equicontinuous, there exists a neighborhood W of 0 in G such that the relations t ∈ K, x ∈ W imply U(t) · x ∈ V; the relations x ∈ W, x′ ∈ V° therefore imply that the function t ↦ ⟨U(t) · x, x′⟩ belongs to S, hence that |⟨U(t) · x, x′⟩| = |∫⟨U(t) · x, x′⟩ dλ(t)| ≤ 1 by the definition of S°.

Let us now assume that U is a continuous mapping of T into F and, moreover, that U(T) is equicontinuous. Then, the same reasoning as above shows (since H is quasi-complete) that for every bounded positive measure μ on T, ∫ U dμ ∈ F. One can therefore define, as above, a linear mapping λ ↦ ∫ U dλ = U(λ) of M^1(T) into F that extends the analogous mapping of C'(T) into F. Moreover, for every closed, balanced, convex neighborhood V of 0 in H, there exists by hypothesis a neighborhood W of 0 in G such that for every x ∈ W and every t ∈ T, one has U(t) · x ∈ V, consequently (since V is weakly closed) ∫ (U(t) · x)dλ(t) ∈ ||λ|| · V (No. 2, Prop. 5). In other words:

#### Proposition 17 {#int-vi-s1-prop-17 .statement}

— Let G, H be two Hausdorff locally convex spaces, with H assumed to be quasi-complete. Let U be a mapping of T into L(G; H) such that (t, x) ↦ U(t) · x is continuous on T × G, and U(T) is equicontinuous. Then, if M^1(T) is equipped with its Banach space topology, the bilinear mapping (λ, x) ↦ U(λ) · x of M^1(T) × G into H is continuous (which implies, in particular, that the linear mapping λ ↦ U(λ) of M^1(T) into L(G; H) is continuous when L(G; H) is equipped with the topology of bounded convergence).

#### Proposition 18 {#int-vi-s1-prop-18 .statement}

— Let G_1, G_2, H_1, H_2 be four Hausdorff locally convex spaces, with H_1 and H_2 assumed to be quasi-complete. Let A : G_1 → G_2 and B : H_1 → H_2 be two continuous linear mappings. Let U_1 : T → L(G_1; H_1), U_2 : T → L(G_2; H_2) be two mappings satisfying the conditions of Prop. 16 (resp. Prop. 17), and suppose that for every t ∈ T, B ◦ U_1(t) = U_2(t) ◦ A. Then, for every measure with compact support (resp. every bounded measure) λ on T, B ◦ U_1(λ) = U_2(λ) ◦ A.

Indeed, for every x ∈ G_1, one has (No. 1, Prop. 1)

$$
(B \circ U_1(\lambda)) \cdot x = \int \left( (B \circ U_1(t)) \cdot x \right) d\lambda(t)
$$
$$
= \int \left( (U_2(t) \circ A) \cdot x \right) d\lambda(t) = U_2(\lambda) \cdot (A \cdot x).
$$

#### Remark 1 {#int-vi-s1-n7-rem-1 .statement}

Suppose that G and H are Banach spaces, and let U be a mapping of T into L(G; H) such that (t, x) ↦ U(t) · x is continuous on T × G. Note that this implies that the finite function t ↦ \|U(t)\| is bounded on every compact subset of T and lower semi-continuous on T, being the upper envelope of the continuous functions $t \mapsto |U(t) \cdot x|$ as $x$ runs over the ball $|x| \leq 1$ in G. Set $h(t) = \| U(t) \|$. Then, for every positive measure $\mu$ on T such that $h$ is $\mu$-integrable, we again have $\int U d\mu \in \mathcal{L}(G; H)$. For, the measure $\nu = h \cdot \mu$ is bounded by hypothesis; there therefore exists a partition of T formed by a $\nu$-negligible set N and a sequence $(K_n)$ of compact subsets. The argument made at the beginning of this No., applied to the measure $\varphi_{K_n} \cdot \mu$, shows that

$$
A_n = \int \varphi_{K_n} U \, d\mu \in F = \mathcal{L}(G; H),
$$

and, moreover (No. 2, Prop. 6), $\| A_n \| \leq \int \varphi_{K_n} \| U \| \, d\mu \leq \nu(K_n)$. The series with general term $A_n$ is therefore absolutely convergent in the Banach space $\mathcal{L}(G; H)$, and it is immediate that its sum is $\int U \, d\mu$ and that $\| \int U \, d\mu \| \leq \int \| U \| \, d\mu$.

#### Remark 2 {#int-vi-s1-n7-rem-2 .statement}

Suppose that $G = H$ is quasi-complete and that $U$ satisfies the hypotheses of Prop. 16. Let M be a dense subset of the space $\mathcal{C}'(T)$, for the weak topology $\sigma(\mathcal{C}'(T), \mathcal{C}(T))$, and let X be a closed linear subspace of H such that $U(\lambda)(X) \subset X$ for every measure $\lambda \in M$. Then also $U(t)(X) \subset X$ for every $t \in T$: indeed, for every $x \in X$ and every $x' \in H'$ orthogonal to X, by hypothesis $\langle U(\lambda) \cdot x, x' \rangle = 0$ for all $\lambda \in M$, which may be written $\int \langle U(t) \cdot x, x' \rangle \, d\mu(t) = 0$. The continuous function $t \mapsto \langle U(t) \cdot x, x' \rangle$, being orthogonal to M, is therefore 0, which yields $\langle U(t) \cdot x, x' \rangle = 0$ for every $x' \in X^\circ$, whence $U(t) \cdot x \in X$ for all $t \in T$ and $x \in X$, and this proves our assertion.

### Exercises {#int-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
