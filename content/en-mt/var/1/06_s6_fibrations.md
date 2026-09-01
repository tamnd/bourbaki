---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 6
section_title: Fibrations
lang: en
source: var-fr
pdf_pages: 0059-0067
extraction: ocr
subsections:
    - "no": 1
      title: Fibrations
      page: 0
      pdf_page: 59
    - "no": 2
      title: Fibrations principales
      page: 0
      pdf_page: 60
    - "no": 3
      title: Morphismes de fibrations principales
      page: 0
      pdf_page: 61
    - "no": 4
      title: Construction de fibrations principales au moyen de cocycles
      page: 0
      pdf_page: 63
    - "no": 5
      title: Espaces fibrés associés à une fibration principale
      page: 0
      pdf_page: 64
    - "no": 6
      title: Extension et restriction du groupe structural
      page: 0
      pdf_page: 66
    - "no": 7
      title: Changements de structure
      page: 0
      pdf_page: 67
statements: 0
exercises: 0
content_sha256: a242e363f8011bc48188d01d98463e2608dfef2f362a989490fe9ffa9cfa9701
translated_from: content/fr/var/1/06_s6_fibrations.md
source_lang: fr
translation_method: machine
source_content_sha256: 041a801bb9638dc98ed267f9a74ade144cc09841cb4d2f742e4682ab57d1cafb
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-83e29116
glossary_version: 34
glossary_terms_sha256: 1b4c7bfbe90668f1b0378db43832f5d2cf72b3cf2f9faad2f0ef58ffad7104ad
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. Fibrations¹

### 6.1. Fibrations

6.1.1. A fibration of class $C'$, or simply a fibration, is called a triplet $(X, B, \pi)$ where $B$ and $X$ are manifolds of class $C'$ and $\pi$ a morphism of $X$ into $B$, having the following property:

(F) For every $x \in B$, there exists an open neighbourhood $U$ of $x$, a manifold $F$, and an isomorphism $\varphi$ of $\pi^{-1}(U)$ onto $U \times F$ such that $\pi(\varphi^{-1}(x, y)) = x$ for every $x \in U$ and every $y \in F$.

If $\lambda = (X, B, \pi)$ is a fibration, $X$ is called the space of $\lambda$, $B$ the base of $\lambda$, and $\pi$ the projection of $\lambda$. The mapping $\pi$ is a submersion; in particular $\pi(X)$ is open in $B$, and if $R$ denotes the equivalence relation defined by $\pi$ in $X$, the canonical mapping of $X/R$ into $\pi(X)$ is an isomorphism. For every $x \in B$, the inverse image $\pi^{-1}(x)$ is a closed submanifold of $X$, called the fibre of $x$, and denoted $X_x$.

6.1.2. Examples:
(a) If $B$ and $F$ are two manifolds, the triplet $(B \times F, B, pr_1)$ is a fibration whose fibres are canonically isomorphic to $F$.
(b) If $\lambda = (X, B, \pi)$ and $\lambda' = (X', B', \pi')$ are fibrations,
$$
\lambda \times \lambda' = (X \times X', B \times B', \pi \times \pi')
$$
is a fibration; it is called the product of $\lambda$ and of $\lambda'$.
(c) If $\lambda = (X, B, \pi)$ and $\lambda' = (X', B, \pi')$ are fibrations with the same base, $\lambda \times_B \lambda' = (X \times_B X', B, \pi \times_B \pi')$ is a fibration; it is called the product of $\lambda$ and of $\lambda'$ over $B$, or again the fibred product of $\lambda$ and of $\lambda'$.

6.1.3. Let $\lambda = (X, B, \pi)$ and $\lambda' = (X', B', \pi')$ be two fibrations. A morphism of $\lambda$ into $\lambda'$ is called any pair $(f, g)$, where $f$ is a morphism of $B$ into $B'$, and $g$ a morphism of $X$ into $X'$, such that $\pi' \circ g = f \circ \pi$. When $B = B'$ and $f = \mathrm{Id}_B$, one says that $g$ is a $B$-morphism of $\lambda$ into $\lambda'$; if $g$ is an isomorphism of $X$ onto $X'$, $g^{-1}$ is a $B$-morphism of $\lambda'$ into $\lambda$, and one says that $g$ is a $B$-isomorphism of $\lambda$ onto $\lambda'$; for this to be so, it is necessary and sufficient that, for every $x \in B$, the mapping $g_x : X_x \to X'_x$ induced by $g$ be an isomorphism.

¹ The definitions and the greater part of the results of §§ 6 and 7 also apply to the category of topological spaces; one must then replace the words « varieties », « subvarieties », « morphisms » and « group varieties » by « topological spaces », « topological subspaces », « continuous mappings » and « topological groups ». Exceptions are the results concerning immersions, submersions, and regular equivalence relations, as well as those of Nos. 6.2.3 and 6.2.4 (a).

6.1.4. The fibration $(B \times F, B, pr_1)$ is called the *trivial* fibration of base $B$ and fibre $F$. An isomorphism of a fibration $\lambda$ onto a trivial fibration is called a *trivialization* of $\lambda$.

6.1.5. Let $\lambda = (X, B, \pi)$ be a fibration, and let $f : B' \to B$ be a morphism. Let $\pi'$ be the canonical morphism from $B' \times_B X$ into $B'$. The triple $(B' \times_B X, B', \pi')$ is a fibration, called the *inverse image of $\lambda$ by $f'$* or the fibration deduced from $\lambda$ by change of basis from $B$ to $B'$ following $f$, and denoted by $B' \times_B \lambda$, or also by $f^*\lambda$. If $f'$ denotes the canonical mapping from $B' \times_B X$ into $X$, the pair $(f, f')$ is a *morphism* from $B' \times_B \lambda$ into $\lambda$; it has the following universal property: if $(f, g)$ is a morphism from a fibration $\lambda'$ with basis $B'$ into the fibration $\lambda$, there exists a unique $B'$-morphism $\varphi : \lambda' \to B' \times_B \lambda$ such that $(f, g) = (f, f') \circ \varphi$.

When $B'$ is a subvariety of $B$, and $f$ the canonical injection of $B'$ into $B$, $B' \times_B X$ is identified with the subvariety $\pi^{-1}(B')$ of $X$, and $\pi'$ is identified with the restriction of $\pi$ to $\pi^{-1}(B')$; the inverse image of $\lambda$ by $f$ is then called the *fibration induced by $\lambda$ on $B'$*.

6.1.6. If $\lambda = (X, B, \pi)$ is a fibration, one calls *morphic section* (or simply *section*) of $\lambda$ any morphism $s : B \to X$ such that $\pi \circ s = \mathrm{Id}_B$.

### 6.2. Principal fibrations

6.2.1. Let $B$ be a variety and $G$ a group variety. One calls a *principal fibration with basis $B$ and structural group $G$* a quadruple $\lambda = (P, G, B, \pi)$ where $P$ is a variety on which $G$ operates on the right by $(x, g) \mapsto x . g$ (cf. n° 5.12.5), and where $\pi$ is a morphism from $P$ into $B$, these data being subject to verifying the following axiom:

(P) For every $b \in B$ there exists an open neighbourhood $U$ of $b$ and an isomorphism $f : U \times G \to \pi^{-1}(U)$ such that one has

$$
\pi(f(u, g)) = u \text{ and } f(u, gg') = f(u, g) \cdot g' \text{ if } u \in U \text{ and } g, g' \in G.
$$

6.2.2. Let $\lambda = (P, G, B, \pi)$ be a principal fibration. The triplet $(P, B, \pi)$ is a fibration; one has $\pi(P) = B$. The equivalence relation $R$ defined by $\pi$ in $P$ coincides with that defined by $G$; its graph is none other than the product $P \times_B P$ (cf. No. 5.11.2); it is a subvariety of $P \times P$. The mapping $(x, g) \mapsto (x, x . g)$ is an isomorphism of $P \times G$ onto $P \times_B P$; the mapping which corresponds to every $(x, y) \in P \times_B P$ the unique element $g \in G$ such that $y = x . g$ is a morphism of $P \times_B P$ into $G$.

The group $G$ operates *properly and freely* on $P$ (cf. Top. Gén., chap. III, 3e éd., § 4). If $x \in P$ and if $b = \pi(x)$, the mapping $g \mapsto x . g$ is an *isomorphism of the variety $G$ onto the fibre of $b$*.

6.2.3. Conversely, let $G$ be a group variety, and let $P$ be a variety on which $G$ operates on the right in such a way as to satisfy the following two conditions:
(a) $G$ operates properly and freely on $P$.
(b) For every $x \in P$, the mapping $g \mapsto x . g$ is an immersion of $G$ in $P$.

Then the equivalence relation defined by $G$ in $P$ is regular; if one denotes by $P/G$ the quotient variety, and by $\pi$ the canonical projection of $P$ onto $P/G$, the quadruplet $(P, G, P/G, \pi)$ is a principal fibration.
When $K$ is of characteristic 0 and $P$ is finite-dimensional, the condition (b) above is a consequence of condition (a).

6.2.4. The conditions of the preceding No. are verified in the following two cases:
(a) $P$ is a group variety and $G$ a group subvariety operating on $P$ by right translations; the basis of the principal fibration thus obtained is the homogeneous space $P/G$.
(b) $G$ is a discrete group operating properly and freely on $P$. The projection $\pi : P \to P/G$ is then an étale morphism (No. 5.7.6).

6.2.5. Examples:
(a) Let $B$ be a variety and let $G$ be a group variety. Let $G$ operate on $B \times G$ by $(b, g) . g' = (b, gg')$. The quadruple $(B \times G, G, B, \mathrm{pr}_1)$ is a principal fibration.
(b) Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G', B', \pi')$ be two principal fibrations. Let $G \times G'$ operate on $P \times P'$ by the formula:
$$
(x, x') . (g, g') = (x.g, x'.g'), \quad x \in P, x' \in P', g \in G, g' \in G'.
$$
The quadruple $\lambda \times \lambda' = (P \times P', G \times G', B \times B', \pi \times \pi')$ is a principal fibration; it is called the product of $\lambda$ and $\lambda'$.
(c) Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G', B, \pi')$ be two principal fibrations with the same base. The subvariety $P \times_B P'$ of $P \times P'$ is stable under the operations of $G \times G'$, and the quadruple
$$
\lambda \times_B \lambda' = (P \times_B P', G \times G', B, \pi \times_B \pi')
$$
is a principal fibration; it is called the product of $\lambda$ and $\lambda'$ over $B$, or also the fibred product of $\lambda$ and $\lambda'$.

### 6.3. Morphisms of principal fibrations

6.3.1. Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G', B', \pi')$ be two principal fibrations. A morphism of $\lambda$ into $\lambda'$ is called any triplet $(f, \varphi, h)$, where $f : P \to P'$ and $h : B \to B'$ are morphisms, $\varphi : G \to G'$ is a homomorphism of group varieties, and where $\pi' \circ f = h \circ \pi$ and $f(x . g) = f(x) . \varphi(g)$ for $x \in P, g \in G$. We note that $f$ determines $h$; one will often say that $(f, \varphi)$, or even simply $f$, is a morphism.

When $B = B'$ and $h = \mathrm{Id}_B$ (resp. when $G = G'$ and $\varphi = \mathrm{Id}_G$), a morphism is called a $B$-morphism compatible with $\varphi$ (resp. a $G$-morphism compatible with $h$). A morphism which is at the same time a $B$-morphism and a $G$-morphism is called a $G$-$B$-morphism (here again, one often says simply “morphism” when there cannot be any confusion). Every $G$-$B$-morphism $f : P \to P'$ is an isomorphism of the variety $P$ onto the variety $P'$; the inverse isomorphism $f^{-1}$ is a $G$-$B$-morphism: $f$ is a $G$-$B$-isomorphism of $P$ onto $P'$.

Two principal fiber spaces $P$ and $P'$ having the same base $B$ and the same structural group $G$ are said to be $G$-$B$-isomorphic (or simply isomorphic) if there exists a $G$-$B$-isomorphism of $P$ onto $P'$.

6.3.2. The principal fibration $(B \times G, G, B, \mathrm{pr}_1)$ is called the *trivial* principal fibration with base $B$ and structural group $G$. An isomorphism of a principal fibration $\lambda = (P, G, B, \pi)$ onto the trivial principal fibration with base $B$ and structural group $G$ is called a *trivialization* of $\lambda$. Every section $s$ of $\lambda$ defines a trivialization $f_s$ of $\lambda$ by the formula:

$$
f_s^{-1}(b, g) = s(b) \cdot g \quad \text{for } b \in B \text{ and } g \in G.
$$

One thus obtains a *bijection from the set of sections of $\lambda$ onto the set of trivializations of $\lambda$*. Moreover, if $s_0$ is a section of $\lambda$, every section $s$ of $\lambda$ can be written uniquely in the form $s(b) = s_0(b) \cdot r(b)$, where $r : B \to G$ is a morphism.

6.3.3. Let $\lambda = (P, G, B, \pi)$ be a principal fibration, and let $h : B' \to B$ be a morphism. Let $\pi'$ (resp. $h'$) be the canonical morphism from $B' \times_B P$ into $B'$ (resp. into $P$). Let $G$ operate on $B' \times_B P$ by the formula

$$
(b', x) \cdot g = (b', x \cdot g), \quad (b', x) \in B' \times_B P, \quad g \in G.
$$

The quadruple $(B' \times_B P, G, B', \pi')$ is a principal fibration, called the *inverse image* of $\lambda$ by $h$, and denoted by $B' \times_B \lambda$ or also $h^* \lambda$. The mapping $h' : B' \times_B P \to P$ is a $G$-morphism compatible with $h$; it has the following universal property: if $f$ is a $G$-morphism compatible with $h$ from a principal fibration $\lambda'$ with basis $B'$ into the fibration $\lambda$, there exists a unique $G$-$B'$-isomorphism $k : \lambda' \to B' \times_B \lambda$ such that $f = h' \circ k$.

When $B'$ is a subvariety of $B$, and $h$ the canonical injection of $B'$ into $B$, $B' \times_B P$ is identified with the subvariety $\pi^{-1}(B')$ of $P$; it is called the *principal fibered space induced by $P$ over $B'$*, and is denoted by $\pi^{-1}(B')$, or also $P|B'$. Every $x \in V$ has an open neighbourhood $U$ such that $P|U$ is trivial.

### 6.4. Construction of principal fibrations by means of cocycles

Let B be a variety, G a group variety and let $\mathcal{U} = (U_i)_{i \in I}$ be an open covering of B.

6.4.1. A cocycle of class $C^r$ on B with values in G, subordinate to $\mathcal{U}$, is called a family $(g_{i,j})_{(i,j) \in I \times I}$ possessing the following two properties:
(1) for every pair $(i,j) \in I \times I$, $g_{i,j}$ is a mapping of class $C^r$ from the open set $U_i \cap U_j$ of B into G;
(2) for every triplet $(i,j,k) \in I^3$, one has
$$
g_{i,k}(x) = g_{i,j}(x) \cdot g_{j,k}(x) \quad \text{for all } x \in U_i \cap U_j \cap U_k.
$$
Two such cocycles $(g_{i,j})$ and $(g'_{i,j})$ are said to be cohomologous if there exists a family $(h_i)_{i \in I}$ where, for every $i \in I$, $h_i$ is a mapping of class $C^r$ from $U_i$ into G, such that:
(3)
$$
g'_{i,j}(x) = h_i(x)^{-1} \cdot g_{i,j}(x) \cdot h_j(x) \quad \text{for all } x \in U_i \cap U_j.
$$

6.4.2. Let $\lambda = (P, G, B, \pi)$ be a principal fibration. Let us give ourselves for every $i \in I$ a section $s_i$ of $\lambda$ above $U_i$ (6.3.3). For every pair $(i,j) \in I^2$, there exists then one and only one morphism $g_{i,j}$ from $U_i \cap U_j$ into G such that:
(4)
$$
s_j(b) = s_i(b) \cdot g_{i,j}(b) \quad \text{for all } b \in U_i \cap U_j.
$$
The family of the $g_{i,j}$ is a cocycle on B with values in G, subordinate to the open covering $\mathcal{U}$. This cocycle is said to be associated with the object $(\lambda, \mathcal{U}, (s_i)_{i \in I})$ and the mappings $g_{i,j}$ are called the transition functions of this object.
For $i \in I$, let $x \mapsto (\pi(x), f_i(x))$ be the trivialization defined by the section $s_i$ of $\lambda|U_i$ (6.3.2). For $x \in \pi^{-1}(U_i \cap U_j)$, one has:
(5)
$$
f_i(x) = g_{i,j}(\pi(x)) \cdot f_j(x).
$$

6.4.3. Conversely, let $g = (g_{i,j})$ be a cocycle on B with values in G, subordinate to the covering $\mathcal{U}$. There exists then a principal fibration $\lambda = (P, G, B, \pi)$ and a family of sections $(s_i)_{i \in I}$ of $\lambda$ over the $U_i$, such that relation (4) is satisfied. The same is then true of (5). If moreover $(\lambda', (s'_i))$ satisfies the same conditions, there exists a unique G-B-isomorphism $f$ of $\lambda$ onto $\lambda'$ such that $s'_i = f \circ s_i$ for every $i \in I$. This result is expressed by saying that $(\lambda, (s_i))$ is determined up to a unique isomorphism by the cocycle $g$.

6.4.4. Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G, B, \pi')$ be two principal fibrations. Let $(s_i)$ (resp. $(s'_i)$) be a family of sections of $\lambda$ (resp. $\lambda'$) over the $U_i$ and let $g$ (resp. $g'$) be the cocycle associated with $(\lambda, \mathcal{U}, (s_i))$ (resp. $(\lambda', \mathcal{U}, (s'_i))$). For $\lambda$ and $\lambda'$ to be G-B-isomorphic, it is necessary and sufficient that the cocycles $g$ and $g'$ be cohomologous. More precisely, for every G-B-isomorphism $f$ of $\lambda$ onto $\lambda'$, there exists one and only one family $(h_i)_{i \in I}$ of morphisms of the $U_i$ into $G$ such that relation (3) is satisfied and such that one has $f \circ (s'_i(x)) = s_i(x) \cdot h_i(x)$ for every $i \in I$ and every $x \in U_i$, and one thus obtains a bijection of the set of G-B-isomorphisms of $\lambda$ onto $\lambda'$ onto the set of families $(h_i)_{i \in I}$ satisfying (3).

6.4.5. Let us take up again the notations of 6.4.2. and let $\mathcal{V} = (V_\alpha)_{\alpha \in A}$ be an open covering finer than the open covering $\mathcal{U}$. Let $\tau : A \to I$ be a mapping such that $V_\alpha \subset U_{\tau(\alpha)}$ for every $\alpha \in A$. Let $s'_\alpha$ be the restriction to $V_\alpha$ of the section $s_{\tau(\alpha)}$ and let $g' = (g'_{\alpha,\beta})$ be the cocycle subordinate to the open covering $\mathcal{V}$ associated with $(\lambda, \mathcal{V}, (s'_\alpha))$. The transition function $g'_{\alpha,\beta}$ is then the restriction to $V_\alpha \cap V_\beta$ of the transition function $g_{\tau(\alpha), \tau(\beta)}$.

### 6.5. Fibre spaces associated with a principal fibration

6.5.1. Let $\lambda = (P, G, B, \pi)$ be a principal fibration. Let F be a variety on which the group G operates on the left; we denote by $(g, y) \mapsto g \cdot y$ the law of operation of G on F. The group G operates on the right on $P \times F$ by the formula $(x, f) \cdot g = (x \cdot g, g^{-1} \cdot f)$; the equivalence relation defined by G in $P \times F$ is regular; the quotient $P \times^G F = (P \times F)/G$ is endowed with a structure of variety.

Let E be a variety. We say that E is endowed with a structure of associated fibre space to $\lambda$ of fibre type F when we have been given a morphism $\rho : P \times F \to E$ having the following property:

(As) One has $\rho(x \cdot g, g^{-1}f) = \rho(x, f)$ for $x \in P, f \in F, g \in G$, and the mapping $\bar{\rho} : P \times^G F \to E$ deduced from $\rho$ by passing to the quotient is an isomorphism of varieties.

It amounts to the same thing to say that $(P \times F, G, E, \rho)$ is a principal fibration. The mapping $\rho$ (or sometimes the mapping $\bar{\rho}$) is called the frame mapping of E, and denoted $(x, f) \mapsto x \cdot f$; one has

$$
(x \cdot g) \cdot f = x \cdot (g \cdot f), \quad \text{for } x \in P, g \in G \text{ and } f \in F.
$$

The datum of $\lambda$ and F determines E up to a unique isomorphism; in particular, one may take for E the variety $P \times^G F$ itself; this is called the associated fibre space to $\lambda$ of fibre type F, and is denoted by $\lambda(F)$.

6.5.2. Let E be an associated fibre space to $\lambda$ and of fibre type F. There exists a unique morphism $\pi_E$ from E into B such that $\pi_E(x \cdot f) = \pi(x)$ if $x \in P, f \in F$; the triplet $(E, B, \pi_E)$ is a fibration; if B and F are separated, E is separated.

Let $b \in B$, and let $F_b = \pi_E^{-1}(b)$; this is a closed subvariety of E. If $x \in P$ is such that $\pi(x) = b$, let $\theta_x : F \to F_b$ be the mapping defined by $\theta_x(f) = x \cdot f$; this is an isomorphism of varieties. Moreover, for every $g \in G$, one has $\theta_{x \cdot g} = \theta_x \circ \rho_g$, where $\rho_g$ denotes the automorphism $f \mapsto g \cdot f$ of F. Suppose

F endowed with a structure s of any species Σ (cf. Ens., chap. IV, § 1, n° 4) and suppose that s is invariant under G; there then exists on F_b a structure s_b of species Σ and only one such that the $\theta_x : F \to F_b$ are isomorphisms; it is obtained by transporting s by means of one of the $\theta_x$ (loc. cit., n° 5).

If s is a section of P above an open set U of B, the mapping $(b, f) \mapsto s(b) . f$ is an isomorphism of $U \times F$ onto $\pi_E^{-1}(U)$.

6.5.3. Examples:
(a) Let $\lambda = (B \times G, B, pr_1)$, let $E = B \times F$, and let
$$
\rho : (B \times G) \times F \to E
$$
the mapping $(b, g, f) \mapsto (b, g . f)$. One thus obtains on $B \times F$ a structure of associated fibre space to $\lambda$ of fibre type F, which is said to be trivial.

(b) Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G', B', \pi')$ be two principal fibrations. Let F (resp. F') be a variety on which G (resp. G') operates on the left; and let E (resp. E') be an associated fibre space to $\lambda$ (resp. to $\lambda'$) of fibre type F (resp. F'). The group $G \times G'$ operates on $F \times F'$ by $(g . g') . (f, f') = (g . f, g' . f')$. The mapping $(P \times P') \times (F \times F') \to E \times E'$ which produces the mappings $P \times F \to E$ and $P' \times F' \to E'$ endows $E \times E'$ with a structure of associated fibre space to $\lambda \times \lambda'$ of fibre type $F \times F'$.

(c) With the notation of (b), if one supposes that $B' = B$, one defines analogously on $E \times_B E'$ a structure of associated fibre space to $\lambda \times_{B'} \lambda'$ of fibre type $F \times F'$.

6.5.4. With the notation of n° 6.5.1, let $h : B' \to B$ be a morphism, let $\lambda' = B' \times_B \lambda$, and let $E' = E' \times_B E$. If $P' = B' \times_B P$, define a mapping $P' \times F \to E'$ by setting $(b', x) . f = (b', x . f)$; one thus endows $E'$ with a structure of associated fibre space to $\lambda'$ of fibre type F; it is called the inverse image by $h$ of the structure given on $E$.

6.5.5. Let $\lambda = (P, G, B, \pi)$ be a principal fibre bundle, and let E (resp. E') be a fibre space associated with $\lambda$ of fibre type F (resp. F'). Let $u : F \to F'$ be a morphism compatible with the operations of G (that is to say such that $u(g . f) = g . u(f)$ for $f \in F, g \in G$). There then exists one and only one morphism $\bar{u} : E \to E'$ such that one has $\bar{u}(x . f) = x . u(f)$ for $x \in P, f \in F$. If $u$ is an immersion (resp. a submersion, a subimmersion), the same is true of $\bar{u}$.

In particular, suppose that a group variety H operates on the right on F in such a way that $g . (f . h) = (g . f) . h$ for $g \in G, f \in F, h \in H$. Every $h \in H$ then defines an automorphism $u_h$ of F compatible with the operations of G, whence an automorphism $\bar{u}_h$ of E; the group H operates on the right on E by $(y, h) \mapsto \bar{u}_h(y)$.

6.5.6. Let $\lambda = (P, G, B, \pi)$ be a principal fibre bundle, and let E be a fibre space associated with $\lambda$ of fibre type F. Let $s : B \to E$ be a section of E. For every $x \in P$, there exists a unique element $\sigma(x) \in F$ such that $s(\pi(x)) = x . \sigma(x)$. The mapping $\sigma : P \to F$ thus defined is a morphism of varieties, and satisfies the identity:

(*) $$
\sigma(x . g) = g^{-1} . \sigma(x).
$$

The mapping $s \mapsto \sigma$ is a bijection of the set of sections of E onto the set of morphisms of P into F which satisfy the identity (*).

6.5.7. Let $\lambda = (P, G, B, \pi)$ and $\lambda' = (P', G, B, \pi')$ be two principal fibre bundles with the same basis B and the same structural group G. The principal fibre bundle $\lambda \times_B \lambda' = (P \times_B P', G \times G, B, (\pi, \pi')_B)$ has structural group $G \times G$. Let $G \times G$ operate on the left on G by the formula:

$$
(g, g') . g_1 = g . g_1 . {g'}^{-1},
$$

and let E be the fibre space associated with $\lambda \times_B \lambda'$ of fibre type G (endowed with the law of operation defined above). Then the sections of E correspond bijectively to the isomorphisms of P onto P’. More precisely, if s is a section of E corresponding (cf. n° 6.5.6) to the morphism $\sigma : P \times_B P' \to G$, there exists one and only one G-B-isomorphism $f_s : P \to P'$ such that $\sigma(x, f_s(x)) = e$ for every $x \in P$; the mapping $s \mapsto f_s$ is a bijection of the set of sections of E onto the set of G-B-isomorphisms of P onto P’.

### 6.6. Extension and restriction of the structural group

6.6.1. Let $\lambda = (P, G, B, \pi)$ be a principal fibre bundle, and let $\varphi$ be a homomorphism of G into a group variety H. Let G operate on the left on H by $g . h = \varphi(g) . h$ and let $P \times^G H$ be the fibre space associated with $\lambda$ of fibre type H. Since the right translations in H are compatible with the operations of G, the group H operates on the right on $P \times^G H$ (cf. n° 6.5.5); if $\pi_H$ denotes the projection of $P \times^G H$ onto B, the quadruplet $(P \times^G H, H, B, \pi_H)$ is a principal fibre bundle, denoted by $\varphi(\lambda)$; it is said to be deduced from $\lambda$ by the homomorphism $\varphi$.

The mapping $f$ of P into $P \times^G H$ which associates with $x \in P$ the class of $(x, e)$ is a B-morphism of P into $P \times^G H$ compatible with $\varphi$ (cf. No. 6.3.1). Moreover, if $f'$ is a B-morphism of P into a principal fiber space $P'$ with structural group H, and if $f'$ is compatible with $\varphi$, there exists a unique H-B-isomorphism $\theta$ of $P \times^G H$ onto $P'$ such that $f' = \theta \circ f$.

6.6.2. Suppose that $\lambda$ is defined by means of an open covering $\mathcal{V} = (U_i)$ of B and a cocycle $(g_{ij})$ (6.4.2). Then $\varphi(\lambda)$ can be defined by means of the same covering and the cocycle $(h_{ij})$, with $h_{ij} = \varphi \circ g_{ij}$.

6.6.3. Let F be a variety on which the group H operates on the left; we denote by $(h, y) \mapsto h . y$ the law of operation of H on F. The group G operates on F by $(g, y) \mapsto \varphi(g) . y$. Let E be a fiber space associated with $\varphi(\lambda)$ of fiber type F. The mapping $(x, y) \mapsto f(x) . y$ of $P \times F$ into E (the mapping $f$ being the one defined in No. 6.6.1) endows E with a structure of fiber space associated with $\lambda$ of fiber type F. In particular, $(P \times^G H) \times^H F$ is canonically identified with $P \times^G F$.

6.6.4. Suppose that G is a subgroup variety of H, and that $\varphi : G \to H$ is the canonical injection of G into H. One then says that $\varphi(\lambda)$ is obtained from $\lambda$ by extension to H of the structural group. The morphism $f : P \to P \times^G H$ of No. 6.6.1 is an isomorphism of P onto a closed subvariety of $P \times^G H$ (equal to $P \times^G H$ if $G = H$); this isomorphism is compatible with the operations of G (note that G operates on $P \times^G H$ as a subgroup of H).

6.6.5. Suppose again that G is a subgroup variety of H, and let $\mu = (Q, H, B, \pi)$ be a principal fibration with structural group H and basis B, and let E be a fiber space associated with $\mu$ of fiber type $H/G$. If $\gamma$ denotes the canonical projection of H onto $H/G$, put $\delta(y) = y . \gamma(e)$, for $y \in Q$ (where $e$ denotes the identity element of H); one thus obtains a morphism $\delta : Q \to E$ and the quadruplet $(Q, G, E, \delta)$ is a principal fibration. In particular, $Q/G$ is canonically identified with E, itself isomorphic to $Q \times^H H/G$ $^{1}$.

Now let $s : B \to E$ be a section of E, and let $\lambda_s$ be the inverse image by $s$ of the fibration $(Q, G, E, \delta)$ which we have just defined. It is a principal fibration, with basis B and structural group G and its extension to H is isomorphic to $\mu$; every fibration having these properties can be obtained in this way, up to an isomorphism; two sections $s_1$ and $s_2$ of E define isomorphic fibrations if and only if they are transformed into one another by an H-B-automorphism of $\mu$.

### 6.7. Changes of structure

The structures and operations described in this paragraph are compatible with the changes of structure described in Nos. 5.13 and 5.14.

$^1$ In the topological case (cf. note $^1$, page 61), it is necessary to suppose that the right translations by the elements of G make H a principal fiber space with structural group G, with base $H/G$; this amounts to saying that there is a nonempty open subset of $H/G$ above which the projection $H \to H/G$ admits a continuous section. In the category of manifolds, the analogous condition is always satisfied (cf. No. 6.2.4).
