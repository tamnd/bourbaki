---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 1
section_title: Homotopies, homéotopies
lang: en
source: ta-i-iv-fr
book_pages: TA III.229-TA III.256, TA III.321-TA III.330
pdf_pages: 0245-0272, 0337-0346
extraction: native
subsections:
    - "no": 1
      title: Applications continues homotopes
      page: 229
      pdf_page: 245
    - "no": 2
      title: Homotopies pointées
      page: 231
      pdf_page: 247
    - "no": 3
      title: Espaces homéotopes
      page: 232
      pdf_page: 248
    - "no": 4
      title: Homéotopies relatives
      page: 234
      pdf_page: 250
    - "no": 5
      title: Rétractions et contractions
      page: 235
      pdf_page: 251
    - "no": 6
      title: Cylindre d’une application
      page: 237
      pdf_page: 253
    - "no": 7
      title: La propriété d’extension des homotopies
      page: 240
      pdf_page: 256
    - "no": 8
      title: Attachement d’un espace topologique
      page: 247
      pdf_page: 263
    - "no": 9
      title: Espace obtenu par contraction d’un sous-espace
      page: 251
      pdf_page: 267
    - "no": 10
      title: Cône d’une application
      page: 253
      pdf_page: 269
statements: 55
exercises: 32
content_sha256: de0ef62b9f9d66991b9ad4548ceb259cb8f282c2877ebedb8e720ef4cfcd07b6
translated_from: content/fr/ta/III/01_s1_homotopies_homeotopies.md
source_lang: fr
translation_method: machine
source_content_sha256: 7d307de563268aa5114dcb65b0ac06ee2554374e654735a774bec52a11dcbd05
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-mini
translation_run: translate-en-mt-8c14793a
glossary_version: 34
glossary_terms_sha256: 66447a73efd5987a4d6be645abb09f11e61359bfbe2bdbb1f074c87d2ceed1f9
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. HOMOTOPIES, HOMEOTOPIES

In this paragraph and those that follow, $\mathbf{I}$ denotes the interval $[0,1]$ of $\mathbf{R}$.

### 1. Homotopic continuous mappings

#### Definition 1 {#ta-iii-s1-def-1 .statement tag=01V4}

Let X and Y be topological spaces and let $f$ and $g$ be continuous mappings of X into Y. A homotopy relating $f$ to $g$ is by definition a continuous mapping $\sigma : X\times \mathbf{I}\rightarrow Y$ such that, for every $x\in X$, one has $\sigma (x,0) =f(x)$ and $\sigma (x,1) =g(x)$. One says that $f$ is homotopic to $g$ if there exists a homotopy relating $f$ to $g$.

One says that $f$ is the origin and $g$ the term of the homotopy $\sigma ($cf. below, III, p. 257, remark 2).

Let A be a subset of X. One says that the homotopy $\sigma$ is fixed on A if, for every $a\in A$, the mapping $t\mapsto \sigma (a, t)$ of $\mathbf{I}$ into Y is constant. In this case, the origin and the term of $\sigma$ coincide at every point of A.

Let X and Y be topological spaces. One says that homotopies $\sigma : X\times \mathbf{I}\rightarrow Y$ and $\tau : X\times \mathbf{I}\rightarrow Y$ are juxtaposed if the term of $\sigma$ is

N. Bourbaki and Springer-Verlag Berlin Heidelberg 2   016

N.©  Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_3  229 the origin of $\tau$, in other words if one has $\sigma (x,1) =\tau (x,0)$ for every $x\in X$. In this case, the mapping $\sigma *\tau$ of $X\times \mathbf{I}$ into Y defined by

$\sigma (x,2t)$ for $0\leqslant t\leqslant 1/2$

$$
(\sigma *\tau )(x, t) = \tag{1}
$$

$\tau (x,2t-1)$ for $1/2\leqslant t\leqslant 1$

is continuous (TG, I, p. 19, prop. 4) and is a homotopy relating the origin of $\sigma$ to the term of $\tau$. It is called the juxtaposed homotopy of the homotopies $\sigma$ and $\tau$.

If $\sigma : X\times \mathbf{I}\rightarrow Y$ is a homotopy, the mapping $\overline{\sigma}: X\times \mathbf{I}\rightarrow Y$ defined bythe origin of$(\sigma x, t$. One has$)\mapsto \frac{\sigma}{\sigma}(=x,1\sigma -$. If$t)\sigma$is a homotopy relating the term ofand $\tau$ are juxtaposed homotopies$\sigma$ to

of $X\times \mathbf{I}$ into Y, the homotopies $\overline{\tau}$ and $\overline{\sigma}$ are juxtaposed and one has $\overline{\sigma*\tau}=\overline{\tau}*\overline{\sigma}$.

#### Proposition 1 {#ta-iii-s1-prop-1 .statement tag=01V5}

Let X and Y be topological spaces. The relation “ $f$ is homotopic to $g$ ” is an equivalence relation in the set $\mathscr{C}(X; Y)$ of continuous mappings of X into Y.

Let $f$ be an element of $\mathscr{C}(X; Y)$. The mapping $f\circ$ pr$_1: X\times \mathbf{I}\rightarrow Y$ is a homotopy relating $f$ to $f$; this relation is therefore reflexive.

Let $f$ and $g$ be elements of $\mathscr{C}(X; Y)$ and $\sigma : X\times \mathbf{I}\rightarrow Y$ a homotopy joining $f$ to $g$. The mapping $\overline{\sigma}: X\times \mathbf{I}\rightarrow Y$ is then a homotopy joining $g$ to $f$; the relation considered is therefore symmetric.

Finally, let us prove that it is transitive. If $f,g$ and $h$ are elements of $\mathscr{C}(X; Y),\sigma$ a homotopy joining $f$ to $g$ and $\tau$ a homotopy joining $g$ to $h$, then $\sigma$ and $\tau$ are juxtaposed and $\sigma *\tau$ is a homotopy joining $f$ to $h$.

Let X and Y be topological spaces. The equivalence relation “$f$ is homotopic to $g$” in $\mathscr{C}(X; Y)$ (Prop. 1) is called the homotopy relation. The quotient set of $\mathscr{C}(X; Y)$ by this relation is denoted by [X; Y]. Its elements are called homotopy classes of continuous mappings of X into Y. The homotopy class of a continuous mapping $f: X\rightarrow Y$ will often be denoted by $[f]$.

#### Proposition 2 {#ta-iii-s1-prop-2 .statement tag=01V6}

Let X, Y and Z be topological spaces, $f$ and $f'$ continuous mappings of X into Y$,g$ and $g'$ continuous mappings of Y into Z. If $f$ is homotopic to $f'$ and if $g$ is homotopic to $g'$, then $g\circ f$ is homotopic to $g'\circ f'$.

Let $\sigma$ be a homotopy joining $f$ to $f'$ and $\tau$ a homotopy joining $g$ to $g'$. Then the mapping $\theta : X\times \mathbf{I}\rightarrow Z$ defined by $\theta (x, t) =\tau (\sigma (x, t), t)$ is a homotopy joining $g\circ f$ to $g'\circ f'$.

Let X, Y and Z be topological spaces. Given homotopy classes $\varphi \in [X; Y]$ and $\psi \in [Y; Z]$, the mappings $g\circ f: X\rightarrow Z$, where $f\in \varphi ,g\in \psi$, all belong to one and the same homotopy class (Prop. 2), which is denoted by $\psi \circ \varphi$ and is called the composite homotopy class of the classes $\psi$ and $\varphi$. The mapping $[X; Y]\times [Y; Z]\rightarrow [X; Z]$ which associates $\psi \circ \varphi$ to $(\varphi , \psi )$ is called the composition mapping.

Let $\varphi \in [X; Y]$ ; we have $\varphi =\varphi \circ$ [Id$_X] =$ [Id$_Y]\circ \varphi$.

Let X, Y, Z and T be topological spaces, let $\varphi \in [X; Y]$, $\psi \in [Y; Z]$ and $\chi \in [Z; T]$. The homotopy class $\chi \circ (\psi \circ \varphi )$ is equal to $(\chi \circ \psi )\circ \varphi$; it is denoted by $\chi \circ \psi \circ \varphi$.

#### Proposition 3 {#ta-iii-s1-prop-3 .statement tag=01V7}

Let X be a topological space and let $(Y_j)_{j\in J}$ be a family of topological spaces. The mapping of $[X;\prod_{j\in J}Y_j]$ into the product set $\prod_{j\in J}[X; Y_j]$ defined by $\varphi \mapsto$ ([pr$_j]\circ \varphi$ )$_{j\in J}$ is bijective.

Surjectivity results immediately from I, p. 25, prop. 1. Let us prove injectivity. Let $f$ and $g$ be continuous mappings of X into $\prod_{j\in J}Y_j$. For each $j\in J$, put $f_j=$ pr$_j\circ f$ and $g_j=$ pr$_j\circ g$; suppose $f_j$ homotopic to $g_j$ and let $\sigma_j$ be a homotopy joining $f_j$ to $g_j$. The mapping $\sigma = (\sigma_j)$ of $X\times \mathbf{I}$ into $\prod_{j\in J}Y_j$ is continuous (loc. cit.) ; it is a homotopy joining $f$ to $g$, whence the proposition.

#### Corollary {#ta-iii-s1-n1-cor-1 .statement tag=01V8}

Let $(X_j)_{j\in J}$ and $(Y_j)_{j\in J}$ be families of topological spaces having the same index set. For each $j\in J$, let $f_j$ and $g_j$ be continuous mappings of $X_j$ into $Y_j$. If, for each $j\in J$, the mappings $f_j$ and $g_j$ are homotopic, the same is true of the product mappings $f: (x_j)\mapsto (f_j(x_j))$ and $g: (x_j)\mapsto (g_j(x_j))$ of $\prod_{j\in J}X_j$ into $\prod_{j\in J}Y_j$.

Suppose that we have $[f_j] = [g_j]$ for each $j\in J$. We have [pr$_j]\circ [f] =$ $[f_j\circ$ pr$_j]$ and [pr$_j]\circ [g] = [g_j\circ$ pr$_j]$, hence [pr$_j]\circ [f] =$ [pr$_j]\circ [g]$ by prop. 2, whence $[f] = [g]$ by prop. 3.

### 2. Pointed homotopies

Let X and Y be topological spaces and let $x$ be a point of X. A homotopy $\sigma : X\times \mathbf{I}\rightarrow Y$ is said to be pointed at $x$ if it is fixed on $\{x\}$, that is to say if the mapping $t\mapsto \sigma (x, t)$ from $\mathbf{I}$ into Y is constant. The juxtaposition of two homotopies pointed at $x$ is pointed at $x$. The origin and the end of a homotopy pointed at $x$ take the same value $y$ at $x$; they are therefore pointed continuous mappings from $(X, x)$ into $(Y, y)$.

Let $(X, x)$ and $(Y, y)$ be pointed topological spaces (I, p. 120, definition 1). The relation « $f$ is related to $g$ by a homotopy pointed at $x$ » is an equivalence relation in the set $\mathscr{C}((X, x); (Y, y))$, called the pointed homotopy relation. The quotient set of $\mathscr{C}((X, x); (Y, y))$ by this equivalence relation is denoted by $[(X, x); (Y, y)]$. Its elements are called pointed homotopy classes of pointed continuous mappings from $(X, x)$ into $(Y, y)$.

The set $\mathscr{C}((X, x); (Y, y))$ is a subset of $\mathscr{C}(X; Y)$. It should be noted that pointed homotopy is a finer equivalence relation than the relation induced by homotopy in $\mathscr{C}(X; Y)$. It is in general a strictly finer relation (see III, p. 321, exerc. 1 and III, p. 234, example 3).

Let also $(Z, z)$ be a pointed topological space. Let $f$ and $f'$ be pointed continuous mappings from $(X, x)$ into $(Y, y),g$ and $g'$ pointed continuous mappings from $(Y, y)$ into $(Z, z)$. If $f$ and $f'$ are related by a homotopy $\sigma$ pointed at $x$, and if $g$ and $g'$ are related by a homotopy $\tau$ pointed at $y$, then $g\circ f$ and $g'\circ f'$ are related by the homotopy $\theta : X\times \mathbf{I}\rightarrow Z$, $(u, t)\mapsto \tau (\sigma (u, t), t)$, which is pointed at $x$. As above, this makes it possible to define the composition mapping of $[(X, x); (Y, y)]\times [(Y, y); (Z, z)]$ into $[(X, x); (Z, z)]$. We leave to the reader the task of formulating and proving for pointed mappings and homotopies the statements analogous to prop. 3 and its corollary.

### 3. Homotopic spaces

#### Definition 2 {#ta-iii-s1-def-2 .statement tag=01V9}

Let X and Y be topological spaces. A homotopy class $\varphi \in$ [X; Y] is said to be invertible if there exists a homotopy class $\psi \in [Y; X]$ such that $\psi \circ \varphi =$ [Id$_X]$ and $\varphi \circ \psi =$ [Id$_Y]$. A continuous mapping is said to be a homotopy equivalence if its homotopy class is invertible.

Let $\varphi \in$ [X; Y] be an invertible homotopy class. There exists a unique homotopy class $\psi \in [Y; X]$ having the properties of definition 2. Let indeed $\psi ,\psi '$ be classes having these properties; one has

$\psi =\psi \circ$ [Id$_Y] =\psi \circ \varphi \circ \psi '=$ [Id$_X]\circ \psi '=\psi '$.

This unique class is called the inverse of the homotopy class $\varphi$ and is denoted $\varphi^{-1}$.

Let Z be a topological space. We have $\chi \circ \varphi \circ \varphi^{-1}=\chi$ for all $\chi \in$ [Y; Z] and $\theta \circ \varphi^{-1}\circ \varphi =\theta$ for all $\theta \in [X; Z]$. It follows that the mappings $\chi \mapsto \chi \circ \varphi$ of [Y; Z] into [X; Z] and $\theta \mapsto \theta \circ \varphi^{-1}$ of [X; Z] into [Y; Z] are bijections inverse to one another. Analogously, the mapping $\chi \mapsto \varphi \circ \chi$ of [Z; X] into [Z; Y] is bijective and its inverse bijection is the mapping $\theta \mapsto \varphi^{-1}\circ \theta$ of [Z; Y] into [Z; X].

Let X, Y, Z be topological spaces, $\varphi \in [X; Y]$ and $\psi \in [Y; Z]$ invertible homotopy classes. Then the class $\psi \circ \varphi$ is invertible, with inverse $\varphi^{-1}\circ \psi^{-1}$. Indeed, we have

$$
(\psi \circ \varphi )\circ (\varphi^{-1}\circ \psi^{-1}) =\psi \circ (\varphi \circ \varphi^{-1})\circ \psi^{-1}
$$

$=\psi \circ$ [Id$_Y]\circ \psi^{-1}$

$=\psi \circ \psi^{-1}=$ [Id$_Z]$

and, analogously, $(\varphi^{-1}\circ \psi^{-1})\circ (\psi \circ \varphi ) =$ [Id$_X]$.

Let X, Y be topological spaces and let $f: X\rightarrow Y$ be a homotopy equivalence. Any continuous mapping $g: Y\rightarrow X$ whose class is the inverse of that of $f$ is called a reciprocal (or inverse) of $f$ up to homotopy. Such a mapping $g$ is a homotopy equivalence.

A homeomorphism $f$ is a homotopy equivalence, and $[f]^{-1}= [f^{-1}]$. The composite mapping of two homotopy equivalences is a homotopy equivalence. The relation "X and Y are topological spaces and there exists a homotopy equivalence of X into Y" is an equivalence relation.

#### Definition 3 {#ta-iii-s1-def-3 .statement tag=01VA}

One says that topological spaces X and Y are homotopy equivalent if there exists a homotopy equivalence of X into Y.

#### Example 1 {#ta-iii-s1-n3-exa-1 .statement tag=01VB}

The empty topological space is homotopy equivalent only to itself.

#### Example 2 {#ta-iii-s1-n3-exa-2 .statement tag=01VC}

Let X be a nonempty topological space. In order that X be homotopy equivalent to a space reduced to one point, it is necessary and sufficient that there exist a constant mapping $p: X\rightarrow$ X which is homotopic to the identity mapping of X. (This is then so for every constant mapping $q: X\rightarrow X$, since $[p] = [p]\circ [q] =$ [Id$_X]\circ [q] = [q]$.) Indeed, let P be a space reduced to one point, $f: P\rightarrow X$ a mapping and $g: X\rightarrow P$ the unique mapping of X into P. We have $g\circ f=$ Id$_P$; in order that $f$ be a homotopy equivalence, it is necessary and sufficient that $f\circ g$ be homotopic to Id$_X$. Now, $f\circ g$ is constant, of image $f(P)$.

#### Example 3 {#ta-iii-s1-n3-exa-3 .statement tag=01VD}

One says that a pointed topological space $(X, x)$ is contractible, or that the topological space X is contractible at $x$, if there exists a homotopy pointed at $x$ connecting Id$_X$ to the constant mapping of X into X of image $\{x\}$. Such a space is homotopy equivalent to a point. There nevertheless exist spaces homotopy equivalent to a point which are not contractible at any of their points, and spaces contractible at one point, but not at every point (III, p. 321, exerc. 1).

#### Example 4 {#ta-iii-s1-n3-exa-4 .statement tag=01VE}

Let E be the numerical space of $n$ dimensions (or, more generally, a topological vector space over $\mathbf{R}$) and let X be a subset of E. One says that the set X is star-shaped at a point $x$ of X if, for all $y\in X$ and all $t\in \mathbf{I}$, the point $tx+ (1-t)y$ belongs to X. A convex subset (I, p. 122) of E is star-shaped at each of its points.

A topological subspace X of E which is star-shaped at one of its points $x$ is contractible at this point. Indeed, the mapping $\sigma : X\times \mathbf{I}\rightarrow X$ defined by $\sigma (y, t) =tx+ (1-t)y$ is a pointed homotopy at $x$ joining Id$_X$ to the constant mapping with image $\{x\}$.

In particular, every interval of $\mathbf{R}$, every convex subset of a numerical space or, more generally, of a topological vector space over $\mathbf{R}$ is contractible at each of its points.

#### Example 5 {#ta-iii-s1-n3-exa-5 .statement tag=01VF}

We shall prove later (TA, V) that the Euclidean spheres $\mathbf{S}_n,n\geqslant 1$, are not spaces homotopic to a point. The unit sphere of a Hilbert space of countable type and infinite dimension is contractible at each of its points (EVT, V, p. 71, exerc. 13).

### 4. Relative homotopies

Let X, Y be topological spaces, let A be a subspace of X and let B be a subspace of Y.

Let $f: X\rightarrow Y$ be a continuous mapping such that $f(A)\subset B$. We say that $f$ is a homotopy of the pair $(X,A)$ onto the pair $(Y,B)$ if there exists a continuous mapping $g: Y\rightarrow X$ such that $g(B)\subset A$, a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$, fixed on A, joining Id$_X$ to $g\circ f$, and a homotopy $\tau : Y\times \mathbf{I}\rightarrow Y$, fixed on B, joining Id$_Y$ to $f\circ g$.

Suppose these conditions are satisfied. Then:

a) The mapping $f$ is a homotopy of X into Y, the mapping $g$ is a homotopy of Y into X, and these homotopies are inverses of one another up to homotopy.

b) The mapping $g$ is then a homotopy of the pair $(Y,B)$ onto the pair $(X,A)$, called the inverse of $f$ up to homotopy.

c) The mappings $f$ and $g$ define, by passing to the subspaces, homeomorphisms of A onto B which are inverse to one another.

We say that the pairs $(X,A)$ and $(Y,B)$ are homotopic if there exists a homotopy of the pair $(X,A)$ onto the pair $(Y,B)$. The relation “X, Y are topological spaces, A is a subspace of X, B is a subspace of Y and the pairs $(X,A)$ and $(Y,B)$ are homotopic” is an equivalence relation.

### 5. Retractions and contractions

#### Definition 4 {#ta-iii-s1-def-4 .statement tag=01VG}

Let X be a topological space and let A be a subset of X.

A retraction of X onto A is called a continuous mapping from X into A which is a retraction of the canonical injection of A into X. If there exists a retraction of X onto A, we say that X can be retracted onto A, or also that A is a retract of X.

Let X be a topological space and let A be a subspace of X.

Suppose that there exists a retraction $r$ of X onto A. The subspace A is identified with the set of points $x\in X$ such that $x=r(x)$. If X is a separated space, A is then closed in X.

According to the following lemma, for a subspace A to be a retract of X, it is necessary and sufficient that every continuous mapping from A into a topological space Y extend to a continuous mapping from X into Y.

#### Lemma 1 {#ta-iii-s1-lem-1 .statement tag=01VH}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. The following conditions are equivalent:

(i) For every topological space Z and every continuous mapping $g: X\rightarrow Z$, there exists a continuous mapping $g': Y\rightarrow Z$ such that $g=$ $g'\circ f$;

(ii) The mapping $f$ is injective and possesses a continuous retraction ;

(iii) The mapping $f$ defines a homeomorphism of X onto its image $f(X)$, which is a retract of Y.

Suppose that $f$ is injective and that $r: Y\rightarrow$ X is a continuous retraction of the mapping $f$. For every continuous mapping $g: X\rightarrow Z$, the mapping $g'=g\circ r: Y\rightarrow Z$ satisfies $g'\circ f=g\circ r\circ f=g$. This proves that (ii)$\Rightarrow$(i).

Suppose that condition (i) is satisfied. Let $g: X\rightarrow X$ be the identity mapping. By hypothesis, there exists a continuous mapping $g': Y\rightarrow X$ such that $g'\circ f=g$. This implies that the mapping $f$ is injective and that $g'$ is a continuous retraction of $f$.

The equivalence of the properties (ii) and (iii) is immediate.

#### Definition 5 {#ta-iii-s1-def-5 .statement tag=01VI}

Let X be a topological space and let A be a subset of X. A contraction of X onto A is a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$ fixed on A whose origin is the identity mapping of X and whose term is a retraction of X onto A. If there exists a contraction of X onto A, one says that X can be contracted onto A, or again that A is a retractile subset of X.

#### Remark {#ta-iii-s1-n5-rem-1 .statement tag=01VJ}

In other words, a contraction of X onto A is a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$ having the following properties:

(i) $\sigma (x,0) =x$ for every $x\in X$;

(ii) $\sigma (x,1)\in A$ for every $x\in X$;

(iii) $\sigma (x, t) =x$ for every $x\in A$ and every $t\in \mathbf{I}$.

For there to exist a contraction of X onto A, it is necessary and sufficient that the canonical injection of A into X be a homotopy of the pair $(A,A)$ onto the pair $(X,A)$.

Let $a$ be a point of X. A contraction of X onto the subspace $\{a\}$ is nothing other than a homotopy pointed at $a$ joining the mapping Id$_X$ to the constant mapping with image $\{a\}$. Consequently, X contracts onto $\{a\}$ if and only if X is contractible at $a$ (Example 3 of III, p. 234).

Let X be a topological space and let A be a subset of X. Let $\sigma$ be a contraction of X onto A. The mapping $r$ of X into A defined by $r(x) =\sigma (x,1)$ is a retraction of X onto A and $\sigma$ is a homotopy joining Id$_X$ to $r$. The relations $r\circ i=$ Id$_A$ and $i\circ r=r$ then imply that the mappings $i$ and $r$ are homotopies, inverse to one another up to homotopy.

#### Definition 6 {#ta-iii-s1-def-6 .statement tag=01VK}

With the preceding notations, one says that $\sigma$ is a strong contraction if, moreover, one has $r(\sigma (x, t)) =r(x)$ for every $x\in X$ and every $t\in \mathbf{I}$,

#### Example {#ta-iii-s1-n5-exa-1 .statement tag=01VL}

Let X be the complement of the origin in $\mathbf{B}_n$. The mapping of $X\times \mathbf{I}$ into X given by $(x, t)\mapsto ((1-t) +t\frac{1}{\|x\|})x$ is a strong contraction of X onto $\mathbf{S}_{n-1}$. The retraction of X onto $\mathbf{S}_{n-1}$ associated with it is the mapping given by $x\mapsto x/\|x\|$.

#### Lemma 2 {#ta-iii-s1-lem-2 .statement tag=01VM}

Let X be a topological space, let U be an open subset of X and let $\sigma$ be a strong contraction of X onto X-U. Then $\sigma (U\times \mathbf{I})\subset \overline{U}$. In particular, $\sigma (U\times  \{1\})$ is contained in the boundary of U.

Let $x\in U$. The set of real numbers $t\in \mathbf{I}$ such that $\sigma (x, t)\in U$ is open in $\mathbf{I}$ and contains 0; let $s$ be its least upper bound. We have $\sigma (x, s)\in \overline{U}$. If $s <1,\sigma (x, s)\notin U$, by definition of $s$; the same is true if $s= 1$ since $\sigma (x,1)\in X-U$. Consequently, $\sigma (x, s)\in$ Fr(U). By definition of a strong contraction, we then have $\sigma (x, s) =\sigma (\sigma (x, s),1) =\sigma (x,1)$; in particular, $\sigma (x,1)\in \overline{U}$. Consequently, $\sigma (x,1)$ belongs to the boundary $\overline{U}\cap (X-U)$ of U.

Soit $t\in \mathbf{I}$; si $\sigma (x, t)\notin U$, il vient encore $\sigma (x, t) =\sigma (\sigma (x, t),1) =$ $\sigma (x,1)$, donc $\sigma (x, t)\in \overline{U}$, d’où le lemme.

### 6. Cylinder of a mapping

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Denote by U the topological space sum of the topological space $U_1= X\times \mathbf{I}$ and of the space $U_2$ = Y and identify $U_1$ and $U_2$ with subspaces of U by the canonical injections. Let R be the equivalence relation on U the finest for which the points $(x,1)$ of $U_1$ and $f(x)$ of $U_2$ are equivalent, for every $x\in X$.

#### Definition 7 {#ta-iii-s1-def-7 .statement tag=01VN}

The cylinder of the mapping $f$ is called and is denoted by Cyl($f$), the topological space quotient $U/R$.

Denote by $\alpha_f: X\times \mathbf{I}\rightarrow$ Cyl($f$) and $\beta_f: Y\rightarrow$ Cyl($f$) the restrictions to $U_1$ and $U_2$ of the canonical surjection of U onto $U/R$. The mapping $\alpha_f$ is a homotopy and its term is $\beta_f\circ f$.

Proposition 4 (Universal Property of Cylinders)

Let Z be a topological space, let $\beta : Y\rightarrow Z$ be a continuous mapping and let $\alpha : X\times \mathbf{I}\rightarrow Z$ be a homotopy whose term is $\beta \circ f$. There exists a unique continuous mapping $\varphi$ from Cyl($f$) into Z such that $\alpha =\varphi \circ \alpha_f$ and $\beta =\varphi \circ \beta_f$.

The mapping $\psi$ from U into Z which coincides with $\alpha$ in $X\times \mathbf{I}$ and with $\beta$ in Y is continuous. We have $\alpha (x,1) =\beta (f(x))$ for every $x\in X$, hence $\psi$ defines by passing to the quotient a continuous mapping $\varphi$ from Cyl($f$) into Z such that $\alpha =\varphi \circ \alpha_f$ and $\beta =\varphi \circ \beta_f$. Since the images of $\alpha_f$ and $\beta_f$ cover Cyl($f$)$,\varphi$ is the only mapping from Cyl($f$) into Z satisfying these relations.

#### Example 1 {#ta-iii-s1-n6-exa-1 .statement tag=01VO}

Let $X',Y'$ be topological spaces and let $f': X'\rightarrow Y'$ be a continuous mapping. Let $u: X\rightarrow X'$ and $v: Y\rightarrow Y'$ be continuous mappings such that $f'\circ u=v\circ f$. There exists a unique continuous mapping $w:$ Cyl($f$)$\rightarrow$ Cyl($f'$) such that $w\circ \alpha_f=\alpha_{f'}\circ (u\times$ Id$_{\mathbf{I}})$ and $w\circ \beta_f=\beta_{f'}\circ v$.

According to prop. 4, applied to Z = Y and $\beta =$ Id$_Y$, there exists a unique continuous mapping $\gamma_f:$ Cyl($f$)$\rightarrow Y$ such that $\gamma_f(\alpha_f(x, s)) =f(x)$ and $\gamma_f(\beta_f(y)) =y$ for $x\in X,s\in \mathbf{I}$ and $y\in Y$.

#### Proposition 5 {#ta-iii-s1-prop-5 .statement tag=01VP}

The mapping $\alpha_f$ induces a homeomorphism of $X\times [0,1[$ onto an open subset of Cyl($f$). The mapping $\beta_f$ defines a homeomorphism of Y onto the complement of this open subset. The mapping $\beta_f\circ \gamma_f$ is a continuous retraction of Cyl($f$) onto $\beta_f(Y)$.

The set $X\times [0,1[$ is an open subset of U, saturated for the relation R, and the equivalence relation induced by R in $X\times [0,1[$ is the equality relation. The first assertion follows from this (TG, I, p. 23, cor. 10).

The complement of $\alpha_f(X\times [0,1[)$ is $\beta_f(Y)$. Since one has $\gamma_f\circ \beta_f=$ Id$_Y,\beta_f$ defines a homeomorphism of Y onto $\beta_f(Y)$ and $\beta_f\circ \gamma_f$ is a continuous retraction of the canonical injection of $\beta_f(Y)$ into Cyl($f$).

The closed subspace $\beta_f(Y)$ of Cyl($f$) is called the basis of the cylinder of $f$. The mapping $\beta_f\circ \gamma_f$ is called the canonical retraction of Cyl($f$) onto its basis.

Consider the mappings $\sigma_1: U_1\times \mathbf{I}\rightarrow$ Cyl($f$) and $\sigma_2: U_2\times \mathbf{I}\rightarrow$ Cyl($f$) defined by

$\sigma_1((x, s), t) =\alpha_f(x,(1-t)s+t)$ for $(x, s)\in X\times \mathbf{I}$ and $t\in \mathbf{I}$

$\sigma_2(y, t) =\beta_f(y)$ for $y\in Y$ and $t\in \mathbf{I}$.

They are continuous. For $x\in X$ and $t\in \mathbf{I}$, one has

$$
\sigma_1((x,1), t) =\alpha_f(x,1) =\beta_f(f(x)) =\sigma_2(f(x), t)
$$

There therefore exists a unique mapping $\sigma_f$ of Cyl($f$)$\times \mathbf{I}$ into Cyl($f$) such that $\sigma_f\circ (\alpha_f\times$ Id$_{\mathbf{I}}) =\sigma_1$ and $\sigma_f\circ (\beta_f\times$ Id$_{\mathbf{I}}) =\sigma_2$. The mapping $\sigma_f$ is continuous (I, p. 19, prop. 10).

#### Proposition 6 {#ta-iii-s1-prop-6 .statement tag=01VQ}

The mapping $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) is a strong contraction of Cyl($f$) onto its base. Its term is the canonical retraction of Cyl($f$) onto its base.

The mapping $\sigma_f$ is a homotopy. The relations $\sigma_f(\alpha_f(x, s),0) =$ $\alpha_f(x, s)$ and $\sigma_f(\beta_f(y),0) =\beta_f(y)$ imply that the origin of $\sigma_f$ is the identity mapping of Cyl($f$). Let $r_f$ denote the term of $\sigma_f$. The relations

$$
\sigma_f(\alpha_f(x, s),1) =\alpha_f(x,1) =\beta_f(f(x)) = (\beta_f\circ \gamma_f)(\alpha_f(x, s))
$$

and $\sigma_f(\beta_f(y),1) =\beta_f(y) = (\beta_f\circ \gamma_f)(\beta_f(y))$ imply that $r_f$ is the canonical retraction $\beta_f\circ \gamma_f$ of Cyl($f$) onto its base.

For $(x, s)\in X\times \mathbf{I}$ and $t\in \mathbf{I}$, we have

$$
r_f(\sigma_f(\alpha_f(x, s), t)) =r_f(\alpha_f(x, s(1-t) +t)) =\beta_f(f(x)) =r_f(\alpha_f(x, s))
$$

For $y\in Y$ and $t\in \mathbf{I}$, we have $r_f(\sigma_f(\beta_f(y), t)) =r_f(\beta_f(y))$. Consequently, $\sigma_f$ is a strong contraction of Cyl($f$) onto its base.

The mapping $\sigma_f$ is called the canonical contraction of the cylinder of $f$ onto its base.

#### Remark 1 {#ta-iii-s1-n6-rem-1 .statement tag=01VR}

Let A be a subset of $X\times \mathbf{I}$ and let $A_1$ be the set of points $x\in X$ such that $(x,1)\in A$. We have $\alpha^{-1}_f(\alpha_f(A)) = A\cup \overset{-1}{f}(f(A_1))\times \{1\}$ and $\beta^{-1}_f(\alpha_f(A)) =f(A_1)$. It follows that the mapping $\alpha_f$ is closed (resp. open) if $f$ is.

#### Remark 2 {#ta-iii-s1-n6-rem-2 .statement tag=01VS}

Suppose that the mapping $f$ is proper. Let P be a point of Cyl($f$). If P = $\alpha_f(x, t)$, with 0 $\leqslant t <$ 1 and $x\in$ X, we have $\alpha^{-1}_f(P) = (x, t)$. In the contrary case, there exists $y\in Y$ such that $P =\beta_f(y)$ and $\alpha^{-1}_f(P) =\overset{-1}{f}(y)\times  \{1\}$. This proves that the fibres of the mapping $\alpha_f$ are quasi-compact. The mapping $\alpha_f$ is then proper (TG, I, p. 75, th. 1), since it is closed.

By prop. 5 and TG, I, p. 72, prop. 2, the mapping $\beta_f$ is itself proper. It follows that, if $f$ is proper, the canonical surjection of U onto Cyl($f$) is proper and hence, in particular, universally strict (I, p. 20, corollary).

#### Remark 3 {#ta-iii-s1-n6-rem-3 .statement tag=01VT}

If the spaces X and Y are separated, the same is true of the mapping cylinder of the mapping $f$. Indeed, let $z$ and $z'$ be two distinct points of Cyl($f$) and let us prove that they possess disjoint neighbourhoods. Distinguish three cases.

– There exist $(x, t)$ and $(x', t')\in X\times [0,1[$ such that $z=\alpha_f(x, t)$ and $z'=\alpha_f(x', t')$.

In this case, the assertion follows from the fact that the space $X\times [0,1[$ is separated (TG, I, p. 54, prop. 7) and that the mapping $\alpha_f$ induces a homeomorphism of this space onto an open subspace of Cyl($f$).

– There exists $(x, t)\in X\times [0,1[$ such that $z=\alpha_f(x, t)$ and $y'\in Y$ such that $z'=\beta_f(y')$.

Then, $\alpha_f(X\times [0,\frac{t+1}{2}[)$ and Cyl($f$)$-\alpha_f(X\times [0,\frac{t+1}{2}])$ are disjoint open neighbourhoods of $z$ and $z'$ in Cyl($f$).

– There exist $y$ and $y'\in Y$ such that $z=\beta_f(y),z'=\beta_f(y')$.

In this case, $y=\not y'$; since Y is separated, there exists an open neighbourhood V of $y$ in Y and an open neighbourhood $V'$ of $y'$ in Y such that $V\cap V'=\emptyset$. Then, $(\beta_f\circ \gamma_f)^{-1}(V)$ and $(\beta_f\circ \gamma_f)^{-1}(V')$ are disjoint open subsets of Cyl($f$) containing respectively $y$ and $y'$.

### 7. The homotopy extension property

#### Definition 8 {#ta-iii-s1-def-8 .statement tag=01VU}

Let X be a topological space and let A be a subset of X. We say that the pair $(X,A)$ possesses the homotopy extension property if, for every topological space Y, every continuous mapping $f: X\rightarrow Y$ and every homotopy $\sigma : A\times \mathbf{I}\rightarrow Y$ whose term is the mapping $f|A$, there exists a homotopy $\tau : X\times \mathbf{I}\rightarrow Y$ extending $\sigma$ and whose term is the mapping $f$.

#### Remark 1 {#ta-iii-s1-n7-rem-1 .statement tag=01VV}

Let X be a topological space and let A be a subset of X such that the pair $(X,A)$ possesses the homotopy extension property. Let Y be a topological space, let $f: X\rightarrow Y$ be a continuous mapping and let $\sigma : A\times \mathbf{I}\rightarrow Y$ be a homotopy whose origin is the mapping $f|A$. The mapping $\overline{\sigma}: A\times \mathbf{I}\rightarrow Y$ defined by $(a, t)\mapsto \sigma (a,1-t)$ is a homotopy with term $f|A$; let $\tau : X\times \mathbf{I}\rightarrow Y$ be a homotopy with term $f$ which extends $\overline{\sigma}$. The mapping $\overline{\tau}: X\times \mathbf{I}\rightarrow Y$ given by $(x, t)\mapsto \tau (x,1-t)$ is then a homotopy which extends $\sigma$ and whose origin is the mapping $f$.

Let X be a topological space, let A be a subspace of X and let $i: A\rightarrow X$ be the canonical injection. Let $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) and $\beta_i: X\rightarrow$ Cyl($i$) denote the canonical mappings. Let $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ be the unique continuous mapping such that $j(\alpha_i(a, s)) = (i(a), s)$ and $j(\beta_i(x)) = (x,1)$ for $a\in A,s\in \mathbf{I}$ and $x\in X$. It is injective; its image is the subspace $(A\times \mathbf{I})\cup (X\times  \{1\})$ of $X\times \mathbf{I}$. The mapping $j$ is closed if A is closed in X. It is not always strict (III, p. 325, exerc. 17).

#### Proposition 7 {#ta-iii-s1-prop-7 .statement tag=01VW}

With the above notations, the following assertions are equivalent:

(i) The pair $(X,A)$ has the homotopy extension property;

(ii) For every topological space Y and every continuous mapping $g:$ Cyl($i$)$\rightarrow Y$, there exists a continuous mapping $g': X\times \mathbf{I}\rightarrow Y$ such that $g=g'\circ j$;

(iii) The injection $j$ has a continuous retraction;

(iv) The mapping $j$ is strict and there exists a contraction of $X\times \mathbf{I}$ onto the image of $j$.

Suppose that the pair $(X,A)$ has the homotopy extension property. Let $g:$ Cyl($i$)$\rightarrow Y$ be a continuous mapping; put $\sigma =g\circ \alpha_i$ and $f=g\circ \beta_i$. The mapping $f: X\rightarrow$ Y is continuous and $\sigma : A\times \mathbf{I}\rightarrow Y$ is a homotopy whose end is the mapping $f|A$. There therefore exists a homotopy $g': X\times \mathbf{I}\rightarrow Y$ with end $f$ extending $\sigma$. We have $g'\circ j(\alpha_i(a, s)) =g'(a, s) =\sigma (a, s) =g(\alpha_i(a, s))$ and $g'\circ j(\beta_i(x)) =$ $g'(x,1) =f(x) =g(\beta_i(x))$ for $a\in A,s\in \mathbf{I}$ and $x\in X$. Consequently, $g'\circ j=g$, whence (ii).

Conversely, suppose that assertion (ii) is satisfied, and let us prove that the pair $(X,A)$ has the homotopy extension property. Let Y be a topological space, let $f: X\rightarrow Y$ be a continuous mapping and let $\sigma : A\times \mathbf{I}\rightarrow Y$ be a homotopy whose end is equal to $f|A$. There exists a unique continuous mapping $g:$ Cyl($i$)$\rightarrow Y$ such that $g\circ \alpha_i=\sigma$ and $g\circ \beta_i=f$ (III, p. 238, prop. 4). Any mapping $g': X\times \mathbf{I}\rightarrow Y$ such that $g=g'\circ j$ is then a homotopy with end $f$ extending $\sigma$.

The equivalence of assertions (ii) and (iii) is a particular case of lemma 1 of III, p. 235.

Suppose that the injection $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ admits a continuous retraction $r$. The mapping $j$ therefore defines a homeomorphism of Cyl($i$) onto the subspace $T = (A\times \mathbf{I})\cup (X\times  \{1\})$ of $X\times \mathbf{I}($loc. cit.). It is therefore strict.

Put $\rho =$ pr$_1\circ j\circ r$ and $\theta =$ pr$_2\circ j\circ r$. If $x\in A$ or if $s= 1$, we have $\rho (x, s) =x$ and $\theta (x, s) =s$ For $(x, s)\in X\times \mathbf{I}$ and $t\in \mathbf{I}$, put

$$
\sigma ((x, s), t) = (\rho (x,(1-t) +st),(1-t)s+t\theta (x, s))
$$

The mapping $\sigma : (X\times \mathbf{I})\times \mathbf{I}\rightarrow X\times \mathbf{I}$ is continuous. For $(x, s)\in X\times \mathbf{I}$, we have

$$
\sigma ((x, s),0) = (\rho (x,1), s) = (x, s)
$$

and

$$
\sigma ((x, s),1) = (\rho (x, s), \theta (x, s)) =j\circ r(x, s)
$$

for $x\in X$ and $t\in \mathbf{I}$, we have

$$
\sigma ((x,1), t) = (\rho (x,1),(1-t) +t\theta (x,1)) = (x,1)
$$

whereas, for $(x, s)\in A\times \mathbf{I}$ and $t\in \mathbf{I}$, we have

$$
\sigma ((x, s), t) = (x,(1-t)s+ts) = (x, s)
$$

Hence $\sigma$ is a contraction of $X\times \mathbf{I}$ onto T. This shows that assertion (iii) implies assertion (iv).

The implication (iv)$\Rightarrow$(iii) is obvious.

#### Remark 2 {#ta-iii-s1-n7-rem-2 .statement tag=01VX}

Let X be a separated topological space and let A be a subset of X such that the pair $(X,A)$ has the homotopy extension property. Let us denote by $i: A\rightarrow$ X the canonical injection. Let $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ be the canonical injection and let $r$ be a continuous retraction of the mapping $j$. The subspace $j$(Cyl($i$)) is equal to the set of pairs $(x, t)\in X\times \mathbf{I}$ such that $j(r(x, t)) = (x, t)$. Since the space $X\times \mathbf{I}$ is separated, the subset $j$(Cyl($i$)) is closed in $X\times \mathbf{I}$. The set A, equal to the set of $x\in X$ such that $(x,0)\in j$(Cyl($i$)), is then a closed subset of X.

#### Lemma 3 {#ta-iii-s1-lem-3 .statement tag=01VY}

Let X and Y be topological spaces, let $p: X\rightarrow Y$ be a continuous proper and open mapping, and let $f: X\rightarrow \mathbf{R}$ be a continuous mapping. The mapping $g: Y\rightarrow \overline{\mathbf{R}}$ given by $y\mapsto$ sup$_{x\in\overset{-1}{p}(y)}f(x)$ is continuous.

Let $b\in Y$. Since $p$ is proper, its fibre $\overset{-1}{p}(b)$ is a quasi-compact space; hence we have $g(b)\in \mathbf{R}\cup  \{-\infty \}$.

Let $m\in \mathbf{R}$ such that $g(b)< m$. For every $a\in \overset{-1}{p}(b)$, one has $f(a)\leqslant$ $g(b)< m$; let $V_a$ be a neighbourhood of $a$ in X such that $f(x)< m$ for every $x\in V_a$. The union V of the sets $V_a$ is a neighbourhood of $\overset{-1}{p}(b)$ in X. By Lemma 5 (I, p. 75), there exists a neighbourhood W of $b$ in Y such that $\overset{-1}{p}(W)\subset V$. For every $y\in W$, one has $g(y)\leqslant m$. This proves that $g$ is upper semi-continuous at $b$.

Let us now prove that $g$ is lower semi-continuous at $b$. We may suppose that $g(b)\in \mathbf{R}$. Let $m\in \mathbf{R}$ such that $m < g(b)$. Let $a\in \overset{-1}{p}(b)$ such that $m < f(b)$; let then V be a neighbourhood of $a$ in X such that $f(x)> m$ for every $x\in V$. It follows that $g(y)> m$ for every $y\in p(V)$. Since $p$ is open, $p(V)$ is a neighbourhood of $b$, so that $g$ is lower semi-continuous.

The lemma is thus proved.

#### Theorem 1 {#ta-iii-s1-thm-1 .statement tag=01VZ}

Let X be a topological space and let A be a closed subspace of X; denote by $i: A\rightarrow X$ the canonical injection. The following assertions are equivalent:

(i) The pair $(X,A)$ has the homotopy extension property ;

(ii) There exists a continuous mapping $\varphi : X\rightarrow \mathbf{I}$ such that $A =\overset{-1}{\varphi}(0)$ and a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$ fixed on A whose term is the identity mapping of X and such that $\sigma (x,0)\in A$ for every point $x\in X$ such that $\varphi (x)= 1\not$ .

(iii) There exists a continuous mapping $\varphi : X\rightarrow \mathbf{R}_+$ such that $A =\overset{-1}{\varphi}(0)$ and a homotopy $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}\rightarrow X$, fixed on A, such that $\sigma (x,1) =x$ and $\sigma (x,0)\in A$ for every $x\in \overset{-1}{\varphi}(\mathbf{I})$.

(iv) There exists a continuous mapping $\varphi : X\rightarrow \mathbf{R}_+$ such that $A\subset \overset{-1}{\varphi}(0)$ and a continuous mapping

$$
\sigma :\{(x, t)\in X\times \mathbf{I}|t+\varphi (x)\geqslant 1\} \rightarrow X
$$

such that $\sigma (x,1) =x$ for every $x\in X$ and $\sigma (x,1-\varphi (x))\in A$ for every $x\in X$ such that $\varphi (x)\leqslant 1$.

We shall denote by $i$ the canonical injection of A into X$,\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) and $\beta_i: X\rightarrow$ Cyl($i$) the canonical mappings, and by $j$ the mapping of Cyl($i$) into $X\times \mathbf{I}$ such that $j(\alpha_i(x, s)) = (x, s)$ for $(x, s)\in A\times \mathbf{I}$ and $j(\beta_i(x)) = (x,1)$ for $x\in X$.

Suppose that the pair $(X,A)$ has the homotopy extension property and let $r: X\times \mathbf{I}\rightarrow$ Cyl($i$) be a continuous retraction of the mapping $j($III, p. 241, Proposition 7). Let us denote by $\sigma$ the continuous mapping pr$_1\circ j\circ r$ of $X\times \mathbf{I}$ into X. For every $(x, t)\in X\times \mathbf{I}$, one has $|$pr$_2(j(r(x, t)))-t|\leqslant 1$. Since $\mathbf{I}$ is compact, the first projection pr$_1: X\times \mathbf{I}\rightarrow X$ is a proper mapping; it is also open. By Lemma 3, the mapping $\varphi : X\rightarrow \mathbf{I}$ given by

$x\mapsto$ sup$_{t\in\mathbf{I}}(|$pr$_2(j(r(x, t)))-t|)$

is therefore continuous.

For $x\in X$, one has $\sigma (x,1) =x$. Let $x\in X$ be such that $\sigma (x,0)\notin A$; then pr$_2(j(r(x,0))) = 1$ and $\varphi (x)\geqslant 1$. For $x\in A$ and $t\in \mathbf{I}$, one has $j(r(x, t)) = (x, t)$; consequently, $\sigma (x, t) =x$ and $\varphi (x) = 0$. Conversely, let $x\in X$ be such that $\varphi (x) = 0$. One has therefore pr$_2(j(r(x, t))\leqslant t$ for every $t\in \mathbf{I}$; if $t <1$, this implies $j(r(x, t))\in A\times \mathbf{I}$; since A is closed in X, one has therefore $j(r(x,1))\in A\times \mathbf{I}$, hence $x\in A$.

This proves that (i) implies (ii).

Let $\varphi$ and $\sigma$ be mappings satisfying the properties of assertion (ii). Put $\varphi_1= 2\varphi$ and let $\sigma_1$ be the restriction of $\sigma$ to $\overset{-1}{\varphi}_{1}(\mathbf{I})\times \mathbf{I}$. We have $\overset{-1}{\varphi}_{1}(0) = A$; for $a\in A,\sigma_1(a, t) =a$ for all $a\in A$. Let $x\in X$ be such that $\varphi_1(x)\leqslant 1$; we have $\sigma_1(x,1) =x$; moreover, $\varphi (x) =\varphi_1(x)/2<1$, hence $\sigma_1(x,0)\in A$. Thus, (ii) implies (iii).

Let us prove that (iii) implies (iv). Let $\varphi : X\rightarrow \mathbf{R}$ and $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times$ $\mathbf{I}\rightarrow X$ be as in the statement; put $B =\overset{-1}{\varphi}(\mathbf{I})$ and $C =\overset{-1}{\varphi}([1,+\infty [)$.

Let $u_1$ be the mapping from $B\times \mathbf{I}$ into X such that $u_1(x, t) =\sigma (x,1-$ $(1-t)/2\varphi (x))$ if $t+ 2\varphi (x)\geqslant 1$ and $\varphi (x)>0$ and $u_1(x, t) =\sigma (x,0)$ otherwise. By the following lemma 4, it is continuous.

Let $u_2$ be the mapping from $B\times \mathbf{I}$ into X such that $u_2(x, t) =$ $\sigma (x$, sup(0$,1-2(1-t)(1-\varphi (x))$)). It is continuous. For $x\in B$ such that $\varphi (x) = 1/2$ and $t\in \mathbf{I}$, we have $u_1(x, t) =\sigma (x, t) =u_2(x, t)$. Let $u: B\times \mathbf{I}\rightarrow X$ denote the mapping such that $u(x, t) =u_1(x, t)$ if $\varphi (x)\leqslant 1/2$ and $u(x, t) =u_2(x, t)$ if $1/2< x\leqslant 1$ ; it is continuous since its restrictions to the closed subspaces $\overset{-1}{\varphi}([0,1/2])\times \mathbf{I}$ and $\overset{-1}{\varphi}([1/2,1])\times \mathbf{I}$ of $B\times \mathbf{I}$ are continuous (TG, I, p. 19, prop. 4).

For $x\in X$ such that $\varphi (x) = 1$ and $t\in \mathbf{I}$, we have $u(x, t) =u_2(x, t) =$ $\sigma (x,1) =x$. There therefore exists a unique mapping $\tau : X\times \mathbf{I}\rightarrow X$ which coincides with $u$ in $B\times \mathbf{I}$ and with the mapping pr$_1$ in $C\times \mathbf{I}$; it is continuous (loc. cit.).

Let $x\in X$; it is verified that one has $\tau (x,1) = 1$. If, moreover, $x\in A$, then one has $\varphi (x) = 0$, hence $\tau (x, t) =u_1(x, t) =\sigma (x,0) =x$. Finally, if $2\varphi (x)\leqslant 1$, then $\varphi (x)\leqslant 1/2$, hence $\tau (x,1-2\varphi (x)) =\sigma (x,0)\in A$.

This proves that assertion (iv) is satisfied.

Suppose finally that assertion (iv) is satisfied, and let us prove that the pair $(X,A)$ has the homotopy extension property.

Let $C_1$ (resp. $C_2$) be the set of pairs $(x, t)\in X\times \mathbf{I}$ such that $t+\varphi (x)\leqslant 1$ (resp. $t+\varphi (x)\geqslant$ 1). These are closed sets. For $(x, t)\in C_1$, one has $\sigma (x,1-\varphi (x))\in A$; let then $\rho_1: C_1\rightarrow$ Cyl($i$) be the mapping defined by $(x, t)\mapsto \alpha_i(\sigma (x,1-\varphi (x)), t+\varphi (x))$; it is continuous. Let also $\rho_2: C_2\rightarrow$ Cyl($i$) be the continuous mapping defined by $(x, t)\mapsto \beta_i(\sigma (x, t))$. For $(x, t)\in C_1\cap C_2$, one has $t+\varphi (x) = 1$, hence

$$
\rho_1(x, t) =\alpha_i(\sigma (x,1-\varphi (x)),1) =\beta_i(\sigma (x,1-\varphi (x)) =\rho_2(x, t)
$$

There therefore exists a unique mapping $\rho : X\times \mathbf{I}\rightarrow$ Cyl($i$) which coincides with $\rho_1$ in $C_1$ and with $\rho_2$ in $C_2$; it is continuous (TG, I, p. 19, prop. 4).

For $x\in A$ and $t\in \mathbf{I}$, one has $\varphi (x) = 0$, hence $t+\varphi (x)\leqslant 1$

$$
\rho (j(\alpha_i(x, t))) =\rho (x, t) =\alpha_i(\sigma (x,1), t) =\alpha_i(x, t)
$$

For $x\in X$, one also has

$$
\rho (j(\beta_i(x))) =\rho (x,1) =\beta_i(\sigma (x,1)) =\beta_i(x)
$$

Since the images of the mappings $\alpha_i$ and $\beta_i$ cover Cyl($i$), it follows that the mapping $\rho$ is a continuous retraction of the mapping $j$. Consequently, the pair $(X,A)$ has the homotopy extension property (III, p. 241, prop. 7), which concludes the proof of the theorem.

#### Lemma 4 {#ta-iii-s1-lem-4 .statement tag=01W0}

Let X and Y be topological spaces, let $\varphi : X\rightarrow \mathbf{R}_+$ be a continuous mapping, and put $A =\overset{-1}{\varphi}(0)$. Let $\sigma : X\times \mathbf{I}\rightarrow Y$ be a homotopy which is fixed on A. The mapping $\sigma ': X\times \mathbf{I}\rightarrow Y$ which maps $(x, s)$ to $\sigma (x, s/\varphi (x))$ if $s < \varphi (x)$ and to $\sigma (x,1)$ if $s\geqslant \varphi (x)$ is continuous.

The mapping $\sigma '$ is continuous at every point of the closed subset $\overset{-1}{\varphi}([1,+\infty [)\times \mathbf{I}$; it is therefore enough to prove that its restriction to $\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}$ is continuous. We may therefore suppose that $\varphi (X)\subset \mathbf{I}$. Let C and $C'$ be the subspaces of $X\times \mathbf{I}$ consisting of pairs $(x, s)$ such that $s\leqslant \varphi (x)$ and $s\geqslant \varphi (x)$ respectively. They are closed and cover $X\times \mathbf{I}$. The mapping $\sigma '$ is continuous on $C'$; let us prove that it is continuous on C.

Let $\alpha : X\times \mathbf{I}\rightarrow X\times \mathbf{I}$ be the continuous mapping defined by $\alpha (x, t) =$ $(x, t\varphi (x))$. Its image is equal to C and $\sigma '\circ \alpha$ is the continuous mapping $\sigma$. Let us prove that $\alpha$ is a proper map. Consider in fact an ultrafilter $\mathfrak{U}$ on $X\times \mathbf{I}$ and a point $(x, t)\in X\times \mathbf{I}$ adherent to the ultrafilter basis $\alpha (\mathfrak{U})$. Since pr$_1\circ \alpha =$ pr$_1$, the ultrafilter basis pr$_1(\mathfrak{U})$ on X converges to $x$. Since $\mathbf{I}$ is compact, there exists a point $s\in \mathbf{I}$ such that the ultrafilter basis pr$_2(\mathfrak{U})$ converges to $s$. Then $\mathfrak{U}$ converges to $(x, s)$. Since $\alpha$ is continuous, the ultrafilter basis $\alpha (\mathfrak{U})$ converges to $(x, s\varphi (x))$. Since $\mathbf{I}$ is separated, we have $s\varphi (x) =t$, whence $\alpha (x, s) = (x, t)$, so that $\alpha$ is proper (TG, I, p. 75, Theorem 1). It then follows from I, p. 18, example 2 and Proposition 9 that $\sigma '|C$ is continuous.

#### Corollary 1 {#ta-iii-s1-lem-4-cor-1 .statement tag=01W1}

Let X be a normal topological space and let A be a closed subspace of X. Suppose that there exist a neighbourhood V of A in X and a contraction of V onto A, together with a continuous mapping $f: X\rightarrow \mathbf{R}$ such that $\overset{-1}{f}(0) = A$. Then the pair $(X,A)$ has the homotopy extension property.

Let $\rho : V\times \mathbf{I}\rightarrow V$ be a contraction of V onto A. By definition of a normal space (TG, IX, p. 41, Definition 1), there exists a continuous mapping $g: X\rightarrow \mathbf{I}$ which is 0 on A and 1 at every point of X - V. Let $\varphi : X\rightarrow \mathbf{R}$ be the mapping defined by $\varphi (x) =|f(x)|+g(x)$ for $x\in X$; it is continuous. We have $\overset{-1}{\varphi}(0) = A$ and $\overset{-1}{\varphi}(\mathbf{I})\subset V$. Let $\sigma$ be the mapping from $\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}$ into X defined by $\sigma (x, t) =\rho (x,1-t)$ for $x\in \overset{-1}{\varphi}(\mathbf{I})$ and $t\in \mathbf{I}$. For $x\in \overset{-1}{\varphi}(\mathbf{I})$, we have $\sigma (x,1) =\rho (x,0) =x$ and $\sigma (x,0) =\rho (x,1)\in A$.

The mappings $\varphi$ and $\sigma$ satisfy the conditions of assertion (iii) of theorem 1 of III, p. 243; hence the pair $(X,A)$ possesses the homotopy extension property.

#### Example 1 {#ta-iii-s1-n7-exa-1 .statement tag=01W2}

Take for space X the ball $\mathbf{B}_n$ and for subspace A the sphere $\mathbf{S}_{n-1}$. If V = X$-\{0\}$, there exists a strong contraction of V onto $\mathbf{S}_{n-1}($III, p. 237, example). Hence the pair $(\mathbf{B}_n,\mathbf{S}_{n-1})$ possesses the homotopy extension property.

#### Corollary 2 {#ta-iii-s1-lem-4-cor-2 .statement tag=01W3}

Let X and Y be topological spaces, let A be a closed subspace of X, let B be a closed subspace of Y. If the pairs $(X,A)$ and $(Y,B)$ possess the homotopy extension property, the same is true of the pair $(X\times Y,(X\times B)\cup (A\times Y))$.

Let $\varphi : X\rightarrow \mathbf{R}_+$ and $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}\rightarrow$ X, resp. $\varphi ': Y\rightarrow \mathbf{R}_+$

and $\sigma ':\overset{-1}{\psi}(\mathbf{I})\times \mathbf{I}\rightarrow Y$, satisfy the conditions of assertion (iv) of theorem 1 for the pair $(X,A)$, resp. for the pair $(Y,B)$. Let $\psi : X\times Y\rightarrow \mathbf{R}_+$ be the mapping given by $(x, y)\mapsto$ inf($\varphi (x), \varphi '(x)$) ; it is continuous; one has also $\psi (x, y) = 0$ for every $(x, y)\in X\times Y$ such that $x\in A$ or $y\in B$. For $(x, y, t)\in X\times Y\times \mathbf{I}$ such that $t+\psi (x)\geqslant 1$, one has $t+\varphi (x)\geqslant 1$ and $t+\varphi '(x)\geqslant 1$. Thus one defines a continuous mapping

$$
\tau :\{(x, y, t)\in X\times Y\times \mathbf{I}|t+\psi (x)\geqslant 1\} \rightarrow X\times Y
$$

by putting $\tau (x, y, t) = (\sigma (x, t), \sigma '(y, t))$. For every $(x, y)\in X\times Y$, one has $\tau (x, y,1) = (\sigma (x,1), \sigma '(y,1)) = (x, y)$. If, moreover, $\psi (x, y)\leqslant 1$, then $\varphi (x)\leqslant 1$ or $\varphi '(y)\leqslant 1$, so that $\sigma (x,1)\in A$ or $\sigma '(y,1)\in B$; it follows that $\tau (x, y,1-\psi (x))$ belong to $(A\times Y)\cup (X\times B)$. This verifies assertion (iv) of theorem 1, whence the corollary.

#### Example 2 {#ta-iii-s1-n7-exa-2 .statement tag=01W4}

*Here are other cases in which the pair $(X,A)$ possesses the homotopy extension property.

(i) The space X is a paracompact differentiable manifold of class $C^1$ and A a closed submanifold of X. In view of corollary1, this follows from the fact that X is perfectly normal (IX, p. 103, exerc. 11) and that A possesses a tubular neighbourhood in X;

(ii) The space X is a cellular space and A a full subspace with respect to a given cellular decomposition of X.*

### 8. Attachment of a topological space

Let $X,B$ be topological spaces, let A be a subspace of B, and let $f: A\rightarrow X$ be a continuous mapping. Let Y denote the topological sum of the spaces $Y_1= X$ and $Y_2= B$, and identify $Y_1$ and $Y_2$ with subspaces of Y by the canonical injections. Let R be the finest equivalence relation in Y for which the elements $a$ of $Y_2$ and $f(a)$ of $Y_1$ are equivalent, for every $a\in A$. The relation R is the equality relation in $Y_1$. Let $x\in Y_1$ and let $b\in Y_2$; one has $xRb$ if and only if $b\in A$ and $f(b) =x$. Let $b, b'\in Y_2$; in order that one have $bRb'$, it is necessary and sufficient that $b=b'$, or that $b, b'\in A$ and $f(b) =f(b')$.

#### Definition 9 {#ta-iii-s1-def-9 .statement tag=01W5}

The quotient topological space $Y/R$ is called the space obtained by attaching the space B to the space X along the mapping $f$. It is denoted by $X\cup_fB$.

Let $\alpha_f: X\rightarrow X\cup_fB$ and $\beta_f: B\rightarrow X\cup_fB$ denote the restrictions to $Y_1$ and $Y_2$ of the canonical surjection of Y onto $Y/R$. One has $\alpha_f\circ f=\beta_f|A$.

#### Remark 1 {#ta-iii-s1-n8-rem-1 .statement tag=01W6}

The mapping $\alpha_f$ is injective. For every subset U

of X, one has $\alpha^{-1}_f(\alpha_f(U)) = U$ and $\beta^{-1}_f(\alpha_f(U)) =\overset{-1}{f}(U)$. If A is an open (resp. closed) subset of B, these relations imply that $\alpha_f$ is an open (resp. closed) mapping of X into $X\cup_fB$.

Let U be an open subset of X and let V be an open subset of B such that $\overset{-1}{f}(U) = V\cap A$. The union of the subsets U of $Y_1$ and V of $Y_2$ is a saturated open subset of Y; its image in $X\cup_fB$ is therefore open, and its trace on $\alpha_f(X)$ is $\alpha_f(U)$. It follows that the mapping $\alpha_f$ defines a homeomorphism of X onto its image in $X\cup_fB$.

#### Remark 2 {#ta-iii-s1-n8-rem-2 .statement tag=01W7}

Let V be a subset of B. One has $\alpha^{-1}_f(\beta_f(V)) =f(V\cap A)$ and

$\beta^{-1}_f(\beta_f(V)) = V\cup \overset{-1}{f}(f(V\cap A))$. If A is closed in B and if the mapping $f$ is closed, the mapping $\beta_f$ is therefore closed. Analogously, if A is open in B and if the mapping $f$ is open, the mapping $\beta_f$ is open.

In these two cases, the mapping $\beta_f$ then induces a homeomorphism of B-A onto its image.

#### Remark 3 {#ta-iii-s1-n8-rem-3 .statement tag=01W8}

Suppose that A is closed and that the mapping $f$ is proper. We have just seen that the mapping $\beta_f$ is closed. For every $x\in X$,

$\beta^{-1}_f(\alpha_f(x)) =\overset{-1}{f}(x)$. It is therefore a quasi-compact subset of A (TG,

I, p. 75, Theorem 1), hence also of B. For every $b\in B,\beta^{-1}_f(\beta_f(b))$

equal to $\{b\}$ if $b\in B-A$, and to $\overset{-1}{f}(f(b))$ if $b\in A$; in both cases, it is a quasi-compact subset of B. The fibres of the mapping $\beta_f$ are therefore quasi-compact; consequently (loc. cit.), the mapping $\beta_f$ is proper.

The mapping $\alpha_f$ is likewise proper (TG, I, p. 72, prop. 2). It follows that the canonical mapping of Y onto $X\cup_fB$ is proper.

#### Example 1 {#ta-iii-s1-n8-exa-1 .statement tag=01W9}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. The cylinder Cyl($f$) is none other than the space obtained by attaching the space Y to the space $X\times \mathbf{I}$ along the mapping $f\circ$ pr$_1$ of $X\times  \{1\}$ into Y.

#### Example 2 {#ta-iii-s1-n8-exa-2 .statement tag=01WA}

Let X be a topological space, let B be a topological space and let A be a subspace of B, and let $f: A\rightarrow X$ be a continuous mapping inducing a homeomorphism of A onto its image.

Put $A'=f(A)$; let $f'$ be the mapping of $A'$ into B which associates to each $x\in A'$ the unique inverse image of $x$ by $f$. The mapping $f'\circ f$ is continuous; since $f$ is strict, the mapping $f'$ is continuous. There exists a unique continuous mapping $u$ of the space $X\cup_fB$ into the space $B\cup_{f'}X$ which maps $\alpha_f(x)$ to $\beta_{f'}(x)$ for $x\in X$ and $\beta_f(b)$ to $\alpha_{f'}(b)$ for $b\in B$; it is a homeomorphism mapping the subspace $\alpha_f(X)$ onto the subspace $\beta_{f'}(X)$.

#### Proposition 8 {#ta-iii-s1-prop-8 .statement tag=01WB}

Let Z be a topological space.

a) Let $u: X\rightarrow Z$ and $v: B\rightarrow Z$ be continuous mappings such that $v(a) =u(f(a))$ for every $a\in A$. Then there exists a unique continuous mapping $w: X\cup_fB\rightarrow Z$ such that $w\circ \alpha_f=u$ and $w\circ \beta_f=v$.

b) Let $\sigma : X\times \mathbf{I}\rightarrow Z$ and $\tau : B\times \mathbf{I}\rightarrow Z$ be homotopies. Suppose that $\tau$ is fixed on A and that $\sigma (f(a), t) =\tau (a, t)$ for every $a\in A$ and every $t\in \mathbf{I}$. Then there exists a unique homotopy $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ such that $\eta (\alpha_f(x), t) =\sigma (x, t)$ and $\eta (\beta_f(b), t) =\tau (b, t)$ for $x\in X,b\in B$ and $t\in \mathbf{I}$. This homotopy is fixed on $\beta_f(A)$.

The proposition results immediately from the definition of a quotient space and prop. 10 (I, p. 19).

#### Corollary 1 {#ta-iii-s1-prop-8-cor-1 .statement tag=01WC}

Let $B'$ be a topological space, let $A'$ be a subspace of $B'$, and let $f': A'\rightarrow$ X be a continuous mapping. Let $v: B\rightarrow B'$ be a continuous mapping such that $v(A)\subset A'$ and $f$ = $f'\circ (v|A)$. Let $w: X\cup_fB\rightarrow X\cup_{f'}B'$ be the unique continuous mapping such that $w\circ \alpha_f=\alpha_{f'}$ and $w\circ \beta_f=\beta_{f'}\circ v$. If $v$ defines a homotopy equivalence of the pair $(B,A)$ onto the pair $(B',A')$, then $w$ defines a homotopy equivalence of the pair $(X\cup_fB, \alpha_f(X))$ onto the pair $(X\cup_{f'}B', \alpha_{f'}(X))$.

Let $v': B'\rightarrow B$ be a continuous mapping, let $\tau : B\times \mathbf{I}\rightarrow B$ be a homotopy fixed on A joining Id$_B$ to $v'\circ v$, and let $\tau ': B'\times \mathbf{I}\rightarrow B'$ be a homotopy fixed on $A'$ joining Id$_{B'}$ to $v\circ v'$. For $a'\in A'$ and $a=v'(a')$, we have the relations $a'=v(a)$ and $\beta_f(v'(a')) =\beta_f(a) =\alpha_f(f(a)) =\alpha_f(f'(a'))$. By Prop. 8, a), there exists a unique mapping $w': X\cup_{f'}B'\rightarrow$ $X\cup_fB$ such that $w'\circ \alpha_{f'}=\alpha_{f'}$ and $w'\circ \beta_{f'}=\beta_f\circ v'$. By Prop. 8, b), there exists a unique homotopy $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow X\cup_{f'}B'$ such that $\eta (\alpha_f(x), t) =\alpha_{f'}(x)$ and $\eta (\beta_f(b), t) =\beta_{f'}(\tau (b, t))$ for $x\in X,b\in B$ and $t\in \mathbf{I}$. Analogously there exists a unique homotopy $\eta ': (X\cup_{f'}B')\times \mathbf{I}\rightarrow$ $X\cup_fB$ such that $\eta '(\alpha_{f'}(x), t) =\alpha_f(x)$ and $\eta '(\beta_{f'}(b), t) =\beta_f(\tau '(b, t))$ for $x\in X,b\in B'$ and $t\in \mathbf{I}$. The mapping from $(X\cup_fB)\times \mathbf{I}$ into $X\cup_fB$ given by $(x, t)\mapsto \eta '(\eta (x, t), t)$ is then a homotopy fixed on $\alpha_f(X)$ joining the identity mapping of $X\cup_fB$ to the mapping $w'\circ w$. Analogously, the mapping from $(X\cup_{f'}B')\times \mathbf{I}$ into $X\cup_{f'}B'$ given by $(x, t)\mapsto \eta (\eta '(x, t), t)$ is a homotopy fixed on $\alpha_{f'}(X)$ joining the identity mapping of $X\cup_{f'}B'$ to the mapping $w\circ w'$. The corollary follows.

#### Example 3 {#ta-iii-s1-n8-exa-3 .statement tag=01WD}

Let $i$ be the canonical injection of A into B and let us take for the space $B'$ the cylinder of the mapping $i$; let $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) and $\beta_i: B\rightarrow$ Cyl($i$) be the canonical mappings and $r_i:$ Cyl($i$)$\rightarrow B$ the canonical retraction of the cylinder Cyl($i$) onto its base. Let $A_0$ be the subspace $\alpha_i(A\times  \{0\})$ of Cyl($i$) and let $f_0: A_0\rightarrow X$ be the mapping $f\circ r_i$. For $a\in A$, we have

$$
\beta_f\circ r_i(\alpha_i(a,0)) =\beta_f(a) =\alpha_f(f_0(\alpha_i(a,0))) =\alpha_f(f(a))
$$

Let $\eta : X\cup_{f_0}$ Cyl($i$)$\rightarrow X\cup_fB$ be the unique continuous mapping such that $\eta \circ \alpha_{f_0}=\alpha_f$ and $\eta \circ \beta_{f_0}=\beta_f\circ r_i$. Suppose that the pair $(B,A)$ has the homotopy extension property. Then the mapping $r_i$ defines a homotopy equivalence of the pair (Cyl($i$)$,A_0$) with the pair $(B,A)$ (III, p. 243, th. 1). By Corollary 1, the mapping $\eta$ then defines a homotopy equivalence of the pair $(X\cup_{f'}B', \alpha_{f'}(X))$ with the pair $(X\cup_fB, \alpha_f(X))$. In particular, $\eta$ is a homotopy equivalence.

#### Corollary 2 {#ta-iii-s1-prop-8-cor-2 .statement tag=01WE}

Let $X'$ be a topological space, let $u: X\rightarrow X'$ be a continuous mapping, and put $f'=u\circ f$. Let $w: X\cup_fB\rightarrow X'\cup_{f'}B$ be the unique continuous mapping such that $w\circ \alpha_f=\alpha_{f'}\circ u$ and $w\circ \beta_f=\beta_{f'}$. If $u$ defines a homotopy equivalence of the pair $(X, f(A))$ with the pair $(X', f'(A))$, then $w$ defines a homotopy equivalence of the pair $(X\cup_fB, \beta_f(B))$ with the pair $(X'\cup_{f'}B, \beta_{f'}(B))$.

The proof is analogous to that of Corollary 1.

#### Proposition 9 {#ta-iii-s1-prop-9 .statement tag=01WF}

Let X and B be topological spaces, let A be a subspace of B, and let $f: A\rightarrow X$ be a continuous mapping.

a) If the pair $(B,A)$ has the homotopy extension property, the same is true of the pair $(X\cup_fB, \alpha_f(X))$.

b) Suppose that the mapping $f$ is injective and strict. If the pair $(X, f(A))$ has the homotopy extension property, the same is true of the pair $(X\cup_fB, \beta_f(B))$.

a) Suppose that the pair $(B,A)$ has the homotopy extension property. Let Z be a topological space, let $u: X\cup_fB\rightarrow Z$ be a continuous mapping, and let $\sigma :\alpha_f(X)\times \mathbf{I}\rightarrow Z$ be a homotopy whose final term is the restriction of $u$ to the subspace $\alpha_f(X)$.

Let us put $v_1=u\circ \alpha_f$ and denote by $\tau_1: X\times \mathbf{I}\rightarrow Z$ the mapping given by $(x, t)\mapsto \sigma (\alpha_f(x), t)$. Put $v_2=u\circ \beta_f$. Since $\beta_f|A =\alpha_f\circ f$, the mapping from $A\times \mathbf{I}$ into Z which maps $(a, t)$ to $\sigma (\alpha_f(f(a)), t)$ for $a\in A$ and $t\in \mathbf{I}$ is a homotopy whose final term is equal to the mapping $v_2|A$. Since the pair $(B,A)$ has the homotopy extension property, there exists a homotopy $\tau_2: B\times \mathbf{I}\rightarrow Z$ whose final term is the mapping $v_2$ and such that $\tau_2(a, t) =\sigma (\alpha_f(f(a)), t)$ for $(a, t)\in A\times \mathbf{I}$.

For $a\in A$ and $t\in \mathbf{I}$, we have $\tau_2(a, t) =\tau_1(f(a), t)$. By Proposition 8, there exists a unique continuous mapping $\sigma : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ such that $\sigma (\alpha_f(x), t) =\sigma_1(x, t)$ and $\sigma (\beta_f(b), t) =\sigma_2(b, t)$, for $x\in X$, $b\in B$ and $t\in \mathbf{I}$. It is a homotopy with final term $u$ which extends $\tau$, hence assertion a).

b) In view of Example 2 (III, p. 249), assertion b) follows from assertion a).

### 9. Space obtained by contraction of a subspace

Let X be a topological space and let A be a subset of X. Consider the finest equivalence relation R in X for which all the elements of A are equivalent: two elements of X are equivalent under this relation if they are equal or if they both belong to A.

#### Definition 10 {#ta-iii-s1-def-10 .statement tag=01WG}

The quotient space of X by R is denoted by $X/A$ and is called the space obtained from X by contraction of the subset A.

Let us denote by $\rho : X\rightarrow X/A$ the canonical surjection. Let Y be a topological space and let $f: X\rightarrow Y$ be a continuous mapping. In order that there should exist a continuous mapping $g: X/A\rightarrow Y$ such that $g\circ \rho =f$, it is necessary and sufficient that $f$ should be constant on A.

If the set A is closed (resp. open) in X, the mapping $\rho$ is closed (resp. open) and induces a homeomorphism of X-A onto its image. If A is a closed and quasi-compact subset of X, the mapping $\rho$ is proper (TG, I, p. 75, th. 1).

If the set A is empty, $\rho$ is a homeomorphism. If it is not empty, A is a point of $X/A$ called the base point of $X/A$ and denoted by $s_{X/A}$. The space $X/A$ is then identified with the space obtained by attaching the space X to the space $\{s_{X/A}\}$ by means of the unique mapping from A into $\{s_{X/A}\}$.

#### Proposition 10 {#ta-iii-s1-prop-10 .statement tag=01WH}

Let X be a topological space and let A be a subset of $x$. Suppose that there exists a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$ with origin Id$_X$, constant on $A\times  \{1\}$ and such that $\sigma (A\times \mathbf{I})\subset A$. Then the canonical mapping $\rho$ of X into $X/A$ is a homotopy equivalence.

Let $f$ be the terminal mapping of $\sigma$. It is a continuous mapping of X into X, homotopic to Id$_X$. It is constant on A; there therefore exists a unique continuous mapping $g: X/A\rightarrow X$ such that $g\circ \rho =f$. On the other hand, since $\sigma (A\times \mathbf{I})\subset A$, there exists a mapping $\sigma '$ of $X/A\times \mathbf{I}$ into $X/A$ such that $\sigma '(\rho (x), t) =\rho (\sigma (x, t))$ for every $x\in X$ and every $t\in \mathbf{I}$. By I, p. 19, prop. 10, the mapping $\sigma '$ is continuous. It is a homotopy joining the identity mapping of $X/A$ to the mapping $\rho \circ g$. Consequently, the mappings $g$ and $\rho$ are homotopy inverses of one another.

#### Remark {#ta-iii-s1-n9-rem-1 .statement tag=01WI}

Let X be a topological space and let A be a subset of X.

1) If the canonical mapping of X onto $X/A$ is a homotopy equivalence, there exists a homotopy $\sigma : X\times \mathbf{I}\rightarrow X$ whose initial mapping is Id$_X$ and which is constant on $A\times  \{1\}$. But it may happen that there exists no such homotopy satisfying moreover the condition $\sigma (A\times \mathbf{I})\subset A$ (III, p. 322, exerc. 4).

2) There may exist a homotopy joining the identity mapping of X to a mapping of X into X which is constant on A, without the spaces X and $X/A$ being homotopy equivalent (III, p. 325, exerc. 14).

3) Suppose that A is contractible. If the pair $(X,A)$ has the homotopy extension property, the canonical mapping of X onto $X/A$ is a homotopy equivalence. Let in fact $\sigma : A\times \mathbf{I}\rightarrow A$ be a homotopy whose initial mapping is the identity mapping of A and whose terminal mapping is a constant mapping. There then exists a homotopy $\sigma '$ with initial mapping Id$_X$ which extends $\sigma$. The assertion then follows from proposition 10.

4) Let X and Y be topological spaces, let A be a nonempty subspace of X and let B be a subspace of Y. Let $f: X\rightarrow Y$ be a continuous mapping such that $f(A)\subset B$. Let $\varphi : X/A\rightarrow Y/B$ denote the continuous mapping deduced from $f$ by passing to quotients. If $f$ defines a homotopy equivalence of the pair $(X,A)$ onto the pair $(Y,B)$, the mapping $\varphi$ is a homotopy equivalence of the pair $(X/A, s_{X/A})$ onto the pair $(Y/B, s_{Y/B})$. Let P be a topological space reduced to a point, and let $\alpha$ and $\beta$ be the constant mappings of A and B into P. Observe that the mapping $\varphi$ is identified with the mapping of $P\cup_{\alpha}X$ into $P\cup_{\beta}Y$ deduced from $f$ and the identity mapping of P. The assertion then follows from corollary 1 of III, p. 249.

### 10. Cone of a mapping

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. Let Cyl($f$) be the cylinder of the mapping $f$. Let $\alpha_f$ denote the canonical mapping of $X\times \mathbf{I}$ into Cyl($f$) and $f_0$ the mapping $x\mapsto \alpha_f(x,0)$ of X into Cyl($f$); these mappings induce homeomorphisms of $X\times \mathbf{I}$ and X respectively onto their images in Cyl($f$).

#### Definition 11 {#ta-iii-s1-def-11 .statement tag=01WJ}

The **cone** of the mapping $f$ is the topological space deduced from Cyl($f$) by contracting $f_0(X)$; it is denoted by Côn$(f)$.

Let $\beta '_f: Y\rightarrow$ Côn$(f)$ denote the composition of the canonical mapping $\beta_f: Y\rightarrow$ Cyl($f$) and the canonical surjection of Cyl($f$) onto Côn$(f)$. The mapping $\beta '_f$ is continuous and defines a homeomorphism of Y onto a closed subset of Côn$(f)$, called the base of the cone, and which we shall thus identify with Y.

Let $\alpha '_f: X\times \mathbf{I}\rightarrow$ Côn$(f)$ denote the composition of the mapping $\alpha_f$ and the canonical surjection of Cyl($f$) onto Côn$(f)$. The mapping $\alpha '_f$ is a homotopy whose origin is a constant mapping and whose term is the mapping $\beta '_f\circ f$.

If X is empty, the mapping $\beta '_f$ is a homeomorphism of Y onto Côn$(f)$.

Suppose that X is not empty. Let $s$ then denote the base point of the space Cyl($f$)$/f_0(X)$; it is said to be the vertex of the cone Côn$(f)$. Since $f_0(X)$ is closed in Cyl($f$), the canonical mapping $\pi :$ Cyl($f$)$\rightarrow$ Côn$(f)$ induces a homeomorphism of Cyl($f$)$-f_0(X)$ onto Côn$(f)-\{s\}($III, p. 252). The vertex of the cone Côn$(f)$ does not belong to its base; the canonical injection of Y into Côn$(f)-\{s\}$ is a homotopy equivalence (III, p. 239, prop. 6).

Let $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) be the canonical contraction of the cylinder of $f$ onto its base. For $c\in$ Cyl($f$)$-f_0(X)$ and $t\in \mathbf{I}$, we have $\sigma_f(c, t)\notin f_0(X)$. Hence there exists a unique mapping $\sigma '_f: ($Côn$(f)-\{s\})\times \mathbf{I}\rightarrow$ Côn$(f)-\{s\}$ such that $\sigma '_f(\pi (c), t) =\pi (\sigma_f(c, t))$ for $c\in$ Cyl($f$)$-f_0(X)$ and $t\in \mathbf{I}$. It is continuous and is a strong contraction of Côn$(f)-\{s\}$ onto Y. It is said to be the canonical contraction of Côn$(f)-\{s\}$ onto its base. Its term is a retraction of Côn$(f)-\{s\}$ onto Y, called the canonical retraction of the cone deprived of its vertex onto its base.

Proposition 11 (Universal Property of Cones)

Let Z be a topological space, let $\beta : Y\rightarrow Z$ be a continuous mapping and let $\alpha : X\times \mathbf{I}\rightarrow Z$ be a homotopy whose origin is a constant mapping and whose term is equal to $\beta \circ f$. There exists a unique continuous mapping $\varphi$ of Côn$(f)$ into Z such that $\alpha =\varphi \circ \alpha '_f$ and $\beta =\varphi \circ \beta '_f$.

From the universal property of cylinders (III, p. 238, prop. 4), there exists a unique continuous mapping $h:$ Cyl($f$)$\rightarrow$ Z such that $\alpha =h\circ \alpha_f$ and $\beta =h\circ \beta_f$. Since the source of $\alpha$ is a constant mapping, the restriction of $h$ to the subspace $\alpha_f(X\times \{0\})$ is constant. There therefore exists a unique continuous mapping $\varphi :$ Cone$(f)\rightarrow Z$ such that $h=\varphi \circ \pi$, where $\pi$ denotes the canonical surjection of Cyl($f$) onto Cone$(f)$. The mapping $\varphi$ satisfies $\alpha =\varphi \circ \alpha '_f$ and $\beta =\varphi \circ \beta '_f$ and it is the only one having these properties, since the images of $\alpha '_f$ and $\beta '_f$ cover Cone$(f)$.

#### Example 1 {#ta-iii-s1-n10-exa-1 .statement tag=01WK}

Let X be a topological space. One denotes by C(X), and calls the cone of the space X, the cone of the mapping Id$_X$; it is the space obtained from $X\times \mathbf{I}$ by contracting $X\times  \{0\}$. Let $\pi$ be the canonical mapping of $X\times \mathbf{I}$ into C(X); the image $C'(X)$ of $X\times [0,1[$ under $\pi$ is called the open cone of the space X.

Assume that X is not empty. Then the cone C(X) is not empty and its base point is again called the vertex of the cone.

The mapping $((x, t), u)\mapsto (x, t(1-u))$ of $(X\times \mathbf{I})\times \mathbf{I}$ into $X\times \mathbf{I}$ is a homotopy joining the identity mapping of $X\times \mathbf{I}$ to the mapping $(x, t)\mapsto (x,0)$. One deduces from this, by passing to quotient sets, a mapping $\sigma : C(X)\times \mathbf{I}\rightarrow C(X)$ such that $\sigma (\pi (x, t), u) =\pi (x, t(1-u))$ for $x\in X,t, u\in \mathbf{I}$. The mapping $\sigma$ is continuous by I, p. 19, prop. 10. The mapping $\sigma$ is then a pointed homotopy at $s$ joining the identity mapping of C(X) to the constant mapping with image $\{s\}$. Consequently, the cone C(X) is contractible to its vertex $s$. Since $\sigma (C'(X)\times \mathbf{I})$ is contained in $C'(X)$, the mapping $\sigma$ defines, by passing to subspaces, a pointed homotopy at $s$ joining the identity mapping of $C'(X)$ to the constant mapping with image $\{s\}$; the open cone $C'(X)$ is therefore contractible to $s$.

#### Remark 1 {#ta-iii-s1-n10-rem-1 .statement tag=01WL}

Let X be a topological space and let A be a subspace of X; let $i$ denote the canonical injection of A into X. The canonical retraction $r_i$ of the cylinder Cyl($i$) onto its base maps the subspace $\alpha_i(A\times  \{0\})$ into A. Let $\rho :$ Cone$(i)\rightarrow X/A$ be the continuous mapping deduced from it by passing to the quotient spaces. Suppose that the pair $(X,A)$ has the homotopy extension property. By III, p. 243, Theorem 1, the mapping $r_i$ defines a homotopy equivalence of the pair (Cyl($i$)$, \alpha_i(A\times  \{0\})$) with the pair $(X,A)$. By Remark 4 of III, p. 253, the mapping $\rho$ is then a homotopy equivalence of the pair (Cone$(i), s$) with the pair $(X, s_{X/A})$. In particular it is a homotopy equivalence.

#### Remark 2 {#ta-iii-s1-n10-rem-2 .statement tag=01WM}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous mapping. The canonical mapping $\alpha '_f: X\times \mathbf{I}\rightarrow$ Cone$(f)$ is constant on $X\times  \{0\}$ and therefore defines a continuous mapping $\gamma_f: C(X)\rightarrow$ Cone$(f)$. The restriction of the mapping $\gamma_f$ to $C'(X)$ is injective and strict, and defines by passing to the subspaces a homeomorphism of the open cone $C'(X)$ onto the complement of Y in Cone$(f)$.

Let us identify the base of the cone C(X) with the space X and let $u$ denote the continuous mapping of $Y\cup_fC(X)$ into Cone$(f)$ deduced from the mappings $\beta '_f: Y\rightarrow$ Cone$(f)$ and $\gamma_f: C(X)\rightarrow$ Cone$(f)$. Conversely, let $v:$ Cone$(f)\rightarrow Y\cup_fC(X)$ be the unique continuous mapping such that $v\circ \alpha '_f$ is the canonical mapping of $X\times \mathbf{I}$ onto C(X) and $v\circ \beta '_f$ is the canonical mapping of Y onto $Y\cup_fC(X)$. The mappings $u$ and $v$ are inverse homeomorphisms of one another.

## EXERCISES {#ta-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
