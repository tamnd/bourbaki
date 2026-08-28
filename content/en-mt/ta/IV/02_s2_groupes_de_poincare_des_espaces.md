---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 2
section_title: Groupes de Poincaré des espaces délaçables
lang: en
source: ta-i-iv-fr
book_pages: TA IV.351-TA IV.368, TA IV.457-TA IV.458
pdf_pages: 0367-0384, 0473-0474
extraction: native
subsections:
    - "no": 1
      title: Propriétés des homomorphismes $\pi_1(f, a)$
      page: 351
      pdf_page: 367
    - "no": 2
      title: Applications relativement connexes
      page: 353
      pdf_page: 369
    - "no": 3
      title: Présentation des groupes de Poincaré
      page: 359
      pdf_page: 375
    - "no": 4
      title: Compléments sur les espaces polonais
      page: 360
      pdf_page: 376
    - "no": 5
      title: Relations d’équivalence maigres dans les espaces polonais
      page: 363
      pdf_page: 379
    - "no": 6
      title: Cardinal des groupes de Poincaré
      page: 365
      pdf_page: 381
statements: 30
exercises: 5
content_sha256: 4c430974a7d8e06ebe947357f0d54c7fd0baf1beadadb269fea12855e8e9e4df
translated_from: content/fr/ta/IV/02_s2_groupes_de_poincare_des_espaces.md
source_lang: fr
translation_method: machine
source_content_sha256: a5eeffc52f66c26498857170cbe24722714d48e553f2f8cd94068e19621fadad
translation_model: gpt-5.4
translation_run: translate-en-mt-c731899c
glossary_version: 34
glossary_terms_sha256: 593801fc53e17815f2b7c4c295c651f3a6c803f34d532165756e0e91e0bf7756
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. POINCARÉ GROUPS OF UNRAVELABLE SPACES

### 1. Properties of the homomorphisms $\pi_1(f, a)$

Let A and B be topological spaces, let $(E, p)$ be a covering of A, let $(E', p')$ be a covering of B, let $f: A\rightarrow B$ and $g: E\rightarrow E'$ be continuous mappings such that $p'\circ g=f\circ p$. Let $a$ be a point of A and let $b=f(a)$. For every $\gamma \in \pi_1(A, a)$ and every $x\in E_a$, one has $g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma )$, by relation (3), III, p. 304. If the diagram

E $^gE'$

$pp'$

A $^f$ B

is a cartesian square, the mapping $g$ induces a bijection of $E_a$ onto $E'_b$. The operation of $\pi_1(A, a)$ in the fibre $E_a$ is then the composite of the operation of the group $\pi_1(B, b)$ in $E'_b$ and of the homomorphism $\pi_1(f, a)$ of $\pi_1(A, a)$ into $\pi_1(B, b)$.

#### Proposition 1 {#ta-iv-s2-prop-1 .statement tag=020S}

Let A be an unravelable topological space, let B be a topological space locally connected by arcs, and let $f: A\rightarrow B$ be a continuous mapping. Let $a$ be a point of A and $b=f(a)$. Suppose that every covering of A is isomorphic to the inverse image by $f$ of a covering of B. Then the homomorphism $\pi_1(f, a):\pi_1(A, a)\rightarrow$ $\pi_1(B, b)$ is injective.

Since the space A is unravelable, there exists a covering E of A whose fibre $E_a$ is a principal homogeneous $\pi_1(A, a)$-set (IV, p. 342, Theorem 1). By assumption, this operation is obtained by means of the homomorphism $\pi_1(f, a)$ from an operation of $\pi_1(B, b)$ on $\pi_1(A, a)$. This implies the injectivity of the homomorphism $\pi_1(f, a)$.

#### Proposition 2 {#ta-iv-s2-prop-2 .statement tag=020T}

Let A be a connected topological space locally connected by arcs, let B be an unravelable topological space, and let $f: A\rightarrow B$ be a continuous mapping. Let $a$ be a point of A and $b=$ $f(a)$. The following assertions are equivalent:

(i) The homomorphism $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ is surjective.

(ii) For every pair $(E,E')$ of coverings of B, the mapping

$$
f^*:\mathscr{C}_B(E; E')\rightarrow \mathscr{C}_A(A\times_BE; A\times_BE')
$$

which associates to a B-morphism $g: E\rightarrow E'$ the A-morphism

$$
f^*(g): A\times_BE\rightarrow A\times_BE',(x, y)\mapsto (x, g(y))
$$

is bijective.

By means of the homomorphism $\pi_1(f, a)$, every $\pi_1(B, b)$-set is endowed with a structure of $\pi_1(A, a)$-set. Condition (i) is then equivalent to the following condition (i$'$):

(i$'$) For every pair $(F,F')$ of $\pi_1(B, b)$-sets, every $\pi_1(A, a)$-morphism of F into $F'$ is a $\pi_1(B, b)$-morphism.

In fact, if the homomorphism $\pi_1(f, a)$ is surjective, every $\pi_1(A, a)$-morphism of $\pi_1(B, b)$-sets is a $\pi_1(B, b)$-morphism. Conversely, let us take a $\pi_1(B, b)$-set F reduced to a point and let $F'=\pi_1(B, b)/f_*(\pi_1(A, a))$. The mapping of F into $F'$ whose image is $f_*(\pi_1(A, a))$ is a $\pi_1(A, a)$-morphism but is not a $\pi_1(B, b)$-morphism if $F'$ is not reduced to a point, that is to say if $\pi_1(f, a)$ is not surjective.

Since the space B is unrollable, every $\pi_1(B, b)$-set is isomorphic to the $\pi_1(B, b)$-set $E_b$, where E is a covering of B (IV, p. 344, remark 1). The equivalence of (i$'$) and (ii) therefore follows from prop. 2 of III, p. 310.

#### Proposition 3 {#ta-iv-s2-prop-3 .statement tag=020U}

Let B be an unrollable topological space and let A be a connected and locally arcwise connected subspace of B (for example an open and connected subset). Let $a$ be a point of A. The following properties are equivalent:

(i) Every covering of B is trivializable over A.

(ii) The image of the homomorphism from $\pi_1(A, a)$ into $\pi_1(B, a)$ induced by the canonical injection is reduced to the identity element.

The implication (ii)$\Rightarrow$(i) follows from corollary 3 (III, p. 309).

Conversely, suppose that every covering of B is trivializable over A. This is in particular the case for the simply arcwise connected covering $(\lambda_a(B), \varepsilon_B)$ (IV, p. 342, th. 1), so that the homomorphism $\pi_1(A, a)\rightarrow \pi_1(B, a)$ is trivial (III, p. 309, cor. 3 of prop. 1).

### 2. Relatively connected mappings

#### Definition 1 {#ta-iv-s2-def-1 .statement tag=020V}

Let X and Y be topological spaces and let $f$ be a continuous mapping of X into Y. One says that the mapping $f$ is relatively connected if every point of Y possesses a fundamental system

of neighbourhoods consisting of sets V such that $\overset{-1}{f}(V)$ is connected and nonempty.

Let $f: X\rightarrow Y$ be a continuous mapping; in order that $f$ be relatively connected, it is necessary and sufficient that every point of Y possess a neighbourhood V such that the mapping $f_V:\overset{-1}{f}(V)\rightarrow V$ induced by $f$ be relatively connected.

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a relatively connected continuous mapping. The image of $f$ is dense in Y. For every open subset of Y, the mapping $f_V:\overset{-1}{f}(V)\rightarrow V$ is relatively connected.

#### Proposition 4 {#ta-iv-s2-prop-4 .statement tag=020W}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a relatively connected continuous mapping.

a) For every connected component U of X$,\overline{f(U)}$ is a

connected, open and closed subset of Y, and one has $\overset{-1}{f}(f(U)) = U$.

b) For every connected component V of Y, there exists a connected component U of X such that $V =f(U)$. The mapping of U into V induced by $f$ by passing to the subsets is relatively connected.

c) The connected components of X ( resp. of Y) are open and closed.

a) Let V be the set of $y\in Y$ which possess a neighbourhood W such that

$\overset{-1}{f}(W)$ is connected and meets U; this is an open set of Y. It contains $\overline{f(U)}$ since $f$ is relatively connected. Conversely, let $y\in V$; let

W be a neighbourhood of $y$ such that $\overset{-1}{f}(W)$ is connected and meets U. For

every neighbourhood $W'$ of $y$ such that $\overset{-1}{f}(W')$ is connected, $\overset{-1}{f}(W\cap W')$ is

not empty, hence $\overset{-1}{f}(W\cup W')$ is connected (TG, I, p. 81, prop. 2). By

hypothesis, $\overset{-1}{f}(W\cup W')$ meets U; hence one has $\overset{-1}{f}(W\cup W')\subset U$ and, a fortiori, $W'\cap f(U)=\not\emptyset$. This proves that $y\in \overline{f(U)}$; therefore, $V =\overline{f(U)}$. In particular, the set $\overline{f(U)}$ is open and closed in Y; prop. 1 (TG, I, p. 81) further implies that it is connected.

The preceding arguments show moreover that $\overset{-1}{f}(f(U))\subset U$,

whence the equality $\overset{-1}{f}(f(U)) = U$, the other inclusion being obvious. In particular, U is open and closed in X.

b) Let V be the connected component of a point $y$ of Y, let W be a

neighbourhood of $y$ such that $\overset{-1}{f}(W)$ is connected and nonempty and let U be the

connected component of X containing $\overset{-1}{f}(W)$. Since $y\in \overline{f(U)}$, it follows from a) and from the definition of the connected component of $y$ that $V =\overline{f(U)}$. Hence V is open and closed in Y.

#### Corollary 1 {#ta-iv-s2-prop-4-cor-1 .statement tag=020X}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous and relatively connected mapping. By passing to connected components, the mapping $f$ induces a bijection from the set of connected components of X onto the set of connected components of Y.

#### Corollary 2 {#ta-iv-s2-prop-4-cor-2 .statement tag=020Y}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a continuous mapping. In order that $f$ be relatively connected, it is necessary and sufficient that the following three properties be satisfied:

a) The image $f(X)$ is dense in Y;

b) The space Y is locally connected; $-_1$

c) For every open and connected set V of Y, the set $f(V)$ is connected.

Suppose that the mapping $f$ is relatively connected. The density of $f(X)$ in Y follows from the definition of a relatively

connected mapping. Let V be an open subset of Y; the mapping $f_V:\overset{-1}{f}(V)\rightarrow$ V is relatively connected. By Prop. 4, the connected components of V are open and closed in V. It follows that Y is locally connected (TG, I, p. 85, prop. 11). To prove assertion c), it is enough to prove that X is connected if Y is. By the lemma, there exists

a connected component U of X such that $Y =\overline{f(U)}$ and $\overset{-1}{f}(f(U)) = U$, whence U = X and X is connected.

Conversely, suppose that conditions a), b), c) are satisfied, and let us show that $f$ is relatively connected. Let $y$ be a point of Y; since Y is locally connected, $y$ has a fundamental system of connected open neighbourhoods. If W is such a neighbourhood, conditions

c) and a) imply that $\overset{-1}{f}(W)$ is connected and nonempty. Hence the mapping $f$ is relatively connected.

#### Corollary 3 {#ta-iv-s2-prop-4-cor-3 .statement tag=020Z}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous and relatively connected mapping. Let F be a set and let $g: X\rightarrow F$ be a locally constant mapping. There exists a unique locally constant mapping $h: Y\rightarrow F$ such that $g=h\circ f$.

The restriction of $g$ to every connected component of X is constant. By Corollary 1, there exists a mapping $h: Y\rightarrow F$, constant on each connected component of Y, such that $g=h\circ f$. The mapping $h$ is locally constant, since the connected components of Y are open. The uniqueness of such a mapping follows from the fact that $f(X)$ is dense in Y.

#### Example 1 {#ta-iv-s2-n2-exa-1 .statement tag=0210}

Let X be a topological space and let R be an equivalence relation in X. Let Y denote the quotient topological space $X/R$ and $f: X\rightarrow Y$ the canonical mapping. Suppose that the equivalence classes of R are connected. Then, for every open and

connected subset V of Y, the set $\overset{-1}{f}(V)$ is connected (TG, I, p. 23, corollary 1 and p. 82, proposition 7). If the space Y is locally connected, the mapping $f$ is thus relatively connected.

#### Example 2 {#ta-iv-s2-n2-exa-2 .statement tag=0211}

Let Y be a topological space locally connected by arcs, and let X be an open subset of Y. The space $\mathscr{C}_c(\mathbf{I}; X)$ of paths in X is identified with a subspace of the space $\mathscr{C}_c(\mathbf{I}; Y)$ of paths in Y; suppose that it is dense. The canonical injection of X into Y is then a relatively connected mapping.

It is enough, in fact, to prove that, for every connected and nonempty open subset V of Y, the set $V\cap X$ is connected and nonempty. The space $\mathscr{C}_c(\mathbf{I}; V)$ is a nonempty open subset of $\mathscr{C}_c(\mathbf{I}; Y)$; it meets $\mathscr{C}_c(\mathbf{I}; X)$, which proves that $V\cap X=\not\emptyset$. Let $x$ and $x'$ be points of $V\cap X$. Since $V\cap X$ is locally connected by arcs, the points $x$ and $x'$ have open neighbourhoods U and $U'$, connected by arcs and contained in $V\cap X$. Since V is connected by arcs (III, p. 260, prop. 7), there exists a path in V joining $x$ to $x'$. By the density assumption and the definition of the topology of compact convergence, there exists a path in $V\cap X$ joining a point of U to a point of $U'$. There then exists a path joining $x$ to $x'$ in $V\cap X$, which proves that the set $V\cap X$ is connected.

#### Proposition 5 {#ta-iv-s2-prop-5 .statement tag=0212}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a continuous and relatively connected mapping. For every pair $(T,T')$ of coverings of Y, the mapping $f^*:\mathscr{C}_Y(T; T')\rightarrow$ $\mathscr{C}_X(X\times_YT; X\times_YT')$ is bijective.

Let $\mathscr{F}$ be the sheaf on X of X-morphisms from $X\times_YT$ into $X\times_YT'$ and let $\mathscr{G}$ be the sheaf on Y of Y-morphisms from T into $T'($I, p. 45, example 4). For every open set U of Y, let us put $\varphi_U= (f_U)^*:\mathscr{G}(U)\rightarrow$

$\mathscr{F}(\overset{-1}{f}(U))$. The mappings $\varphi_U$ define a sheaf morphism $\varphi :\mathscr{G}\rightarrow \varphi_*(\mathscr{F})$ and it is enough to prove that $\varphi$ is an isomorphism of sheaves.

Since Y is locally connected (IV, p. 354, cor. 2), the connected open sets over which T and $T'$ are trivializable form a basis of the topology of Y. By corollary 2 of I, p. 55, it is enough to prove that for such an open set U, the mapping $\varphi_U$ is bijective, which allows us to suppose that Y is connected and that the coverings T and $T'$ are the trivial coverings $Y\times F$ and $Y\times F'$ where F and $F'$ are sets endowed with the discrete topology. The mapping $(x,(y, t))\mapsto (x, t)$ identifies the X-space $X\times_Y(Y\times F)$ with $X\times F$ (resp. the X-space $X\times_Y(Y\times F')$ with $X\times F'$). Since the space X is connected (IV, p. 354, cor. 2), the sets $\mathscr{C}_Y(Y\times F; Y\times F')$ and $\mathscr{C}_X(X\times F; X\times F')$ are both identified with the set $\mathscr{F}(F; F')$ of mappings from F into $F'$, and the mapping $f^*$ is identified with the identity mapping of $\mathscr{F}(F; F')$. This concludes the proof.

#### Corollary 1 {#ta-iv-s2-prop-5-cor-1 .statement tag=0213}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous relatively connected mapping. Let T and $T'$ be coverings of Y. If the coverings $X\times_YT$ and $X\times_YT'$ of X are isomorphic, the coverings T and $T'$ are isomorphic.

Let in fact $h: X\times_YT\rightarrow X\times_YT'$ and $h': X\times_YT'\rightarrow X\times_YT$ be X-isomorphisms inverse to one another. By proposition 5, there exist Y-morphisms $g: T\rightarrow T'$ and $g': T'\rightarrow T$ such that $f^*(g) =h$ and $f^*(g') =h'$. We then have $f^*(g'\circ g) =f^*(g')\circ f^*(g) =$ Id$_{X\times_YT}$, therefore $g'\circ g=$ Id$_T$, because the mapping $f^*$ is injective. Analogously, $g\circ g'=$ Id$_{T'}$. The coverings T and $T'$ are therefore isomorphic.

#### Corollary 2 {#ta-iv-s2-prop-5-cor-2 .statement tag=0214}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous and relatively connected mapping. If the space X is simply connected, the same is true of the space Y.

By corollary 1, every covering of Y is in fact trivializable.

#### Corollary 3 {#ta-iv-s2-prop-5-cor-3 .statement tag=0215}

Let X be a topological space locally connected by arcs, Y an unravelable topological space, and let $f: X\rightarrow$ Y be a continuous relatively connected mapping. For every point $x$ of X, the homomorphism $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ is surjective.

By IV, p. 353, prop. 4, one may suppose that the spaces X and Y are connected. The corollary then follows from proposition 5 and proposition 2 of IV, p. 352.

#### Proposition 6 {#ta-iv-s2-prop-6 .statement tag=0216}

Let X and Y be topological spaces and let $f: X\rightarrow Y$ be a continuous and relatively connected mapping. Suppose that every point of Y possesses an open neighbourhood V whose inverse image $\overset{-1}{f}(V)$ is simply connected. Then, for every covering Z of X, there exists a covering T of Y such that $X\times_YT$ is X-isomorphic to Z.

Let $\mathscr{U}$ be the set of open sets of Y whose inverse image in X

is simply connected. For every $V\in \mathscr{U}$, the covering $\overset{-1}{f}(V)\times_XZ$

of $\overset{-1}{f}(V)$ is trivializable; there thus exists a discrete space $F_V$ and an

isomorphism of coverings $g_V:\overset{-1}{f}(V)\times_XZ\rightarrow \overset{-1}{f}(V)\times F_V$. For every

pair $(V,V')$ of open sets belonging to $\mathscr{U}$, the mapping $f_{V\cap V'}:\overset{-1}{f}(V\cap$ $V')\rightarrow V\cap V'$ is relatively connected. By proposition 5 of IV, p. 356, there exists a unique isomorphism of coverings of $V\cap V'$, $h_{V',V}: (V\cap V')\times F_V\rightarrow (V\cap V')\times F_{V'}$, such that one has $f^*(h_{V',V})(x, t) =$ $g_{V'}(g_V^{-1}(x, t))$ for every $x\in V\cap V'$ and every $t\in F_V$. If V, $V',V''$ are elements of $\mathscr{U}$, one has $h_{V'',V}(x, t) =h_{V'',V'}(h_{V',V}(x, t))$ for every $x\in V\cap V'\cap V''$ and every $t\in F_V$. There then exists a unique Y-space T and, for every $V\in \mathscr{U}$, an isomorphism $h_V: T_V\rightarrow V\times F_V$, such that one has $h_{V',V}(x, t) =h_{V'}\circ h^{-1}_V(x, t)$ for every pair $(V,V')$ of open sets belonging to $\mathscr{U}$, every $x\in V\cap V'$ and every $t\in F_V($cf. TG, I, p. 16). The space T is in particular a covering of Y. There moreover exists a

unique mapping of $X\times_YT$ onto Z whose restriction to $\overset{-1}{f}(V)\times_YT$ is given by $g^{-1}_V\circ f^*(h_V)$ and this is an isomorphism of X-spaces, whence the proposition.

#### Corollary {#ta-iv-s2-n2-cor-1 .statement tag=0217}

Let X and Y be contractible topological spaces and let $f: X\rightarrow Y$ be a continuous and relatively connected mapping. Suppose that every point of Y possesses a neighbourhood V whose inverse

image $\overset{-1}{f}(V)$ is simply connected. Then, for every point $x$ of X, the homomorphism $\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))$ is bijective.

One may suppose the spaces X and Y connected (IV, p. 353, prop. 4). By corollary 3 (IV, p. 357), the homomorphism $\pi_1(f, x)$ is surjective. Proposition 6 and proposition 1 of IV, p. 351 imply that it is injective.

#### Remark {#ta-iv-s2-n2-rem-1 .statement tag=0218}

Let Y be a topological space, and let X, $X'$ and $Y'$ be subspaces of Y such that $X\subset X'\subset Y'\subset Y$. Suppose that the canonical injection of X into Y is relatively connected. For every connected open subset V of Y, the set $V\cap X$ is connected and dense in V (IV, p. 354, cor. 2); consequently, the set $V\cap X'$ is connected (TG, I, p. 81, prop. 1). This proves that the canonical injection of $X'$ into $Y'$ is relatively connected.

Let V be an open subset of Y; by what precedes, the canonical injection of $V\cap X$ into $V\cap X'$ is relatively connected. If the set $V\cap X$ is simply connected, $V\cap X'$ is so also, by virtue of corollary 2 of IV, p. 357. Consequently, if the canonical injection of X into Y satisfies the hypotheses of proposition 6, the same is true of the canonical injection of $X'$ into $Y'$.

#### Example {#ta-iv-s2-n2-exa-3 .statement tag=0219}

Let Y be a locally finite-dimensional differentiable manifold and let Z be a closed submanifold of Y (VAR, R, 5.8.3). Put X = Y-Z.

a) If the codimension of Z is at least 2 at every point, the canonical injection of X into Y is relatively connected. Let indeed $z$ be a point of Z; there exists an open neighbourhood V of $z$ in Y and a homeomorphism $\varphi$ of V onto a finite-dimensional vector space E over $\mathbf{R}$ such that $\varphi (V\cap Z)$ is a vector subspace F of E whose codimension is $\geqslant 2$. The set E-F is connected (TG, VI, p. 5, proposition 4), whence the assertion.

b) Suppose moreover that the codimension of Z is at least equal to 3 at every point; the hypotheses of proposition 6 and of its corollary are then satisfied because, with the notations of the preceding paragraph, E-F is simply connected (I, p. 128, example 4).

Differentiable manifolds being contractible spaces (IV, p. 347), the results of this No. admit the following particular case.

Let Y be a locally finite-dimensional differentiable manifold, Z a closed submanifold of Y and $i$ the canonical injection of Y-Z into Y.

a) If the codimension of Z in Y is $\geqslant 1$ at every point, the manifold Y-Z is dense in Y and the mapping $\pi_0(i)$ is surjective.

b) If the codimension of Z in Y is $\geqslant 2$ at every point, the mapping $\pi_0(i)$ is bijective and, for every point $x$ of Y-Z, the mapping $\pi_1(i, x)$ is surjective.

c) If the codimension of Z in Y is $\geqslant 3$ at every point, the mappings $\pi_0(i)$ and $\pi_1(i, x)$ are bijective, for every point $x$ of Y-Z.

### 3. Presentation of Poincaré groups

#### Theorem 1 {#ta-iv-s2-thm-1 .statement tag=021A}

Let X be a compact contractible topological space and let $x$ be a point of X. The Poincaré group $\pi_1(X, x)$ has a finite presentation.

The arcwise connected component of $x$ in X is open, closed and contractible; this makes it possible to suppose that the space X is connected. Since the space X is contractible, the X-space $E =\lambda_x(X)$, endowed with the terminal mapping, is a nonempty arcwise simply connected covering (IV, p. 342, th. 1). The group G = Aut$_X(E)$ is isomorphic to $\pi_1(X, x)$; it therefore suffices to prove that the group G has a finite presentation.

Since X is compact, every point $x$ of X possesses a compact neighbourhood $K_x$ over which the covering E is trivializable (TG, I, p. 65, corollary). Since X is locally connected, every $x\in X$ possesses an open connected neighbourhood $W_x$, contained in $K_x$. Let F be a finite subset of X such that the $W_x$, for $x\in F$, cover X. Let $n$ be the cardinal of F.

We shall prove by induction that, for every integer $k$ such that 1 $\leqslant k\leqslant n$, there exist a subset A of cardinal $k$ contained in F and, for $x\in A$, a section $s_x$ of $p$ over $K_x$, such that the union of the $s_x(W_x)$, for $x\in A$, is a connected subset of E. The assertion is true for $k= 1$. Suppose it true for an integer $k$ such that $1\leqslant k < n$ and let us prove that it is true for $k+ 1$. Let A be a subset of F of cardinal $k$ and, for every $x\in A$, let $s_x$ be a section of E over $K_x$, such that $\bigcup_{x\in A}s_x(W_x)$ is connected. The open sets $\bigcup_{x\in A}W_x$ and $\bigcup_{x\in F-A}W_x$ are nonempty and cover X; their intersection is therefore nonempty, since X is connected. There thus exist $x\in A,y\in F-A$ and $z\in W_x\cap W_y$. Put $A'= A\cup  \{y\}$ and choose a section $s_y$ of E over $K_y$ such that $s_y(z) =s_x(z)$. The connected open sets $\bigcup_{p\in A}s_p(W_p)$ and $s_y(W_y)$ are nonempty and have a common point; their union is therefore connected. This proves the assertion for $k+ 1$. By induction, it is therefore true for every integer $k\in  \{1, . . . , n\}$.

Applying the preceding to $k=n$, there then exists, for every $x\in F$, a section $s_x$ of E over $K_x$, in such a way that $U =\bigcup_{x\in F}s_x(W_x)$ is a connected open subset of E. We have $p(U) = X$. Since the group G operates transitively in each fibre of the covering E, we have GU = E.

The closure of U is contained in $\bigcup_{x\in F}s_x(K_x)$ and therefore is compact. The operation of G in E is proper (I, p. 96, cor. 1), hence the set of pairs $(g, x)\in G\times E$ such that $x\in \overline{U}$ and $gx\in \overline{U}$ is a compact subset of $G\times E$ (TG, I, p. 77, prop. 6). It follows that the set of $g\in G$ such that $\overline{U}\cap g\overline{U}=\not\emptyset$ is compact. Since it is discrete, it is finite. A fortiori, the set of $g\in G$ such that $U\cap gU=\not\emptyset$ is finite. The theorem thus follows from prop. 10 of I, p. 136.

### 4. Complements on Polish spaces

#### Lemma 1 {#ta-iv-s2-lem-1 .statement tag=021B}

Let X be a topological space and let A be a subset of X. In order that A be meagre, it is necessary and sufficient that there exist an open covering $(U_i)_{i\in I}$ of X such that $A\cap U_i$ be meagre in $U_i$ for every $i\in I$.

Let $\mathscr{O}$ be the set of open subsets U of X such that $A\cap U$ be meagre. The set of subsets of $\mathscr{O}$ consisting of pairwise disjoint open subsets, ordered by inclusion, is inductive. Let $\mathfrak{U}$ be a maximal element; there exists one by E, III, p. 20, th. 2.

Let O be the union of the open subsets of X belonging to $\mathfrak{U}$. For every open subset $U\in \mathfrak{U}$, let $(B_{U,n})$ be a sequence of rare subsets of U whose union is $A\cap U$. For every integer $n$, the union $B_n$ of the subsets $B_{U,n}$, with U ranging over $\mathfrak{U}$, is rare relative to O (TG, IX, p. 52, prop. 1). By TG, IX, p. 53, prop. 2, $B_n$ is a rare subset of X, since O is open in X. Consequently, the set $A\cap O$, equal to the union of the $B_n$, is a meagre subset of X.

Let F be the complement of O. It is a closed subset of X; let us prove that it has empty interior. In the contrary case, let $x$ be an interior point of F. By assumption, there exists an open neighbourhood V of $x$, which may be supposed contained in F, such that $A\cap V$ be meagre. Then V is disjoint from the open subsets of X belonging to $\mathfrak{U}$ and $\mathfrak{U}\cup  \{V\}$ is a set of pairwise disjoint open subsets belonging to $\mathscr{O}$, which contradicts the maximality of $\mathfrak{U}$. The relation

$$
A = (A\cap F)\cup (A\cap O)
$$

then implies that A is meagre, which was to be proved.

Let X be a topological space.

Recall (TG, IX, p. 69) that a subset A of X is said to be approachable if there exists an open subset U of X such that $U\cap \complement A$ and $A\cap \complement U$ be meagre in X. The set of approachable subsets of X is a tribe which contains the Borel tribe (TG, IX, p. 69, lemma 8 and its proof). A meagre subset is approachable.

For every subset A of X, let D(A) be the set of points $x\in X$ such that for every neighbourhood V of $x,A\cap V$ is not meagre. One also sets $D^*(A) = A\cup D(A)$.

#### Lemma 2 {#ta-iv-s2-lem-2 .statement tag=021C}

Let X be a topological space and let A be a subset of X.

a) The set D(A) is closed in X; its complement is the largest open subset U of X such that $A\cap U$ be a meagre set.

b) In order that A be meagre, it is necessary and sufficient that D(A) be empty.

c) The set $D^*(A)$ is approachable.

d) For every approachable set B of X containing A, $D^*(A)\cap$ $\complement B$ is meagre.

Let U be the union of the open subsets V of X such that $A\cap V$ be meagre. In order that a point $x$ belong to U, it is necessary and sufficient that it possess a neighbourhood V such that $A\cap V$ be meagre. Thus one has $U =\complement D(A)$ and therefore D(A) is a closed subset of X. By construction, the subspace U has a covering by open subsets whose intersection with A is meagre. By lemma 1, applied to the topological space U and to the subset $A\cap U$, $A\cap U$ is meagre in U, hence also in X. This proves assertion a), since, by construction, every open subset V of X such that $A\cap V$ be meagre is contained in U.

Assertion b) follows immediately from this.

c) One has $D^*(A) = A\cup D(A) = (A\cap U)\cup D(A)$. The set D(A) is closed, hence approachable (IV, p. 361); the meagre subset $A\cap U$ is so as well. Hence $D^*(A)$ is approachable (loc. cit.).

d) Let B be an approachable subset of X containing A. Its complement $\complement B$ is then an approachable subset of X (loc. cit.) and there therefore exists an open subset V of X such that $V\cap B$ and $\complement V\cap \complement B$ are meagre. Since $A\subset B$, $V\cap A$ is still meagre, whence $V\subset U$. Since $\complement U\cap \complement B$ is contained in $\complement V\cap \complement B$, it is also a meagre subset of X. Finally, the inclusions

$$
D^*(A)\cap \complement B =((A\cap U)\cap \complement B)\cup (\complement U\cap \complement B)\subset (A\cap U)\cup (\complement U\cap \complement B)
$$

show that $D^*(A)\cap \complement B$ is a meagre subset of X.

#### Remark 1 {#ta-iv-s2-n4-rem-1 .statement tag=021D}

Let G be a topological group and let A be a meagre subset of G. Suppose that A contains a nonempty open subset U of G and let $y$ be a point of U. Then U is meagre and for every $x\in G,xy^{-1}U$ is a neighbourhood of $x$ in G. Hence every point of G possesses a meagre neighbourhood, therefore G is meagre (IV, p. 360, lemma 1).

Conversely, if G is not meagre, every meagre subset has empty interior and G is a Baire space. Since a Baire space is not meagre, this proves the following assertion: In order that a topological group be a Baire space, it is necessary and sufficient that it be not meagre.

#### Proposition 7 {#ta-iv-s2-prop-7 .statement tag=021E}

Let X be a separated space. Every Souslinian subspace (TG, IX, p. 59, def. 2) of X is approachable.

Let S be a Souslinian subspace of X. By definition, there exists a complete metric space P of countable type and a continuous surjective mapping $g$ of P onto S. By TG, IX, p. 64, lemma 3, there exists a sieve $C = (C_n, p_n, \varphi_n)_{n\in\mathbf{N}}$ of the metric space P.

For every integer $n$ and every $c\in C_n$, let us denote by $F_n(c)$ the image of the set $\varphi_n(c)$ under $g$; let us also put $F^*_n(c) = D^*(F_n(c))$ and

$$
G_n(c) = F^*_n(c)\cap \complement \bigcup_{c'\in\overset{-1}{p_{n}}(c)}F^*_{n+1}(c') \tag{1}
$$

For every $c\in C_n,F^*_n(c)$ is approachable (IV, p. 361, lemma 2, c)). Since $C_{n+1}$ is countable, the union of the approachable subsets $F^*_{n+1}(c')$, where $c'$ runs through $\overset{-1}{p_{n}}(c)$, is again an approachable subset of X. It contains the union of the $F_{n+1}(c')$, which is equal to $F_n(c)$. Hence (loc. cit., d)), $G_n(c)$ is a meagre subset of X. The union G of the subsets $G_n(c)$, for $n\in \mathbf{N}$ and $c\in C_n$, is therefore a meagre subset of X.

Let $c_0\in C_0$ and let $x$ be an element of $F^*_0(c_0)\cap \complement G$; let us prove that $x\in F_0(c_0)$. Since $x\notin G_0(c_0)$ and $x\in F^*_0(c_0)$, there exists $c_1\in \overset{-1}{p_{0}}(c_0)$ such that $x\in F^*_1(c_1)$, by relation (1). By recurrence, there exists an element $c= (c_n)_n$ of $\prod_nC_n$ such that, for every integer $n\in \mathbf{N}$, one has $x\in F^*_n(c_n)$ and $p_n(c_{n+1}) =c_n$.

The subsets $\varphi_n(c_n)$ form a basis of a Cauchy filter in P; this filter converges to a point $p$ of P, since P is complete. The image of this filter under $g$ is a filter F on X, having as basis the set of the $F_n(c_n)$ for $n\in \mathbf{N}$, which converges to $g(p)$. Since $F^*_n(c_n)$ is contained in $\overline{F_n(c_n)}$ and $x$ belongs to each of the $F_n(c_n)$, $x$ is an adherent point of F, hence $x=g(p)$ because the space X is separated (TG, I, p. 52, prop. 1). The point $p$ belongs to $\overline{\varphi_1(c_1)}$, hence to $\varphi_0(c_0)$. Consequently, $x\in F_0(c_0)$.

Consequently, the set $F^*_0(c_0)$ - $F_0(c_0)$ is contained in G. It is therefore a meagre subset of X, hence also an approachable subset. Since $F_0(c_0) = F^*_0(c_0)$ - $(F^*_0(c_0)$ - $F_0(c_0))$ and $F^*_0(c_0)$ is approachable, $F_0(c_0)$ is approachable, because the approachable subsets of X form a tribe. Since $C_0$ is countable, the set S which is the union of the $F_0(c_0)$, for $c_0\in C_0$, is again approachable.

### 5. Meagre equivalence relations in Polish spaces

#### Lemma 3 {#ta-iv-s2-lem-3 .statement tag=021F}

Let $(U_i)_{i\in I}$ be a finite family of nonempty open subsets of a topological space X and let O be an open dense subset of $X\times X$. There exists a family $(V_i)_{i\in I}$ of nonempty open subsets of X such that $V_i\subset U_i$ for all $i\in I$ and such that $V_i\times V_{i'}\subset O$ for every pair $(i, i')$ of distinct elements of I.

For every pair $(j_1, j_2)$ of distinct elements of I, the set of families $(x_i)\in X^I$ such that $(x_{j_1}, x_{j_2})\in O$ is an open dense subset of $X^I$. The intersection Ω of these open sets, when $(j_1, j_2)$ runs through the finite set of pairs of distinct elements of I, is therefore an open dense subset of $X^I$. Consequently, $\Omega \cap \prod_{i\in I}U_i$ is a nonempty open subset of $X^I$, hence contains an open subset of $X^I$ of the form $\prod_{i\in I}V_i$, where for every $i\in I$, $V_i$ is an open, nonempty, subset of $U_i$. This proves the lemma.

#### Proposition 8 {#ta-iv-s2-prop-8 .statement tag=021G}

Let P be a nonempty Polish topological space and let R be an equivalence relation in P whose graph is a meagre subset of $P\times P$. There exists a continuous injective mapping of the set $\{0,1\}^{\mathbf{N}}$, endowed with the product topology of the discrete topologies, into P whose image meets each equivalence class with respect to R in at most one point.

Let the space P be endowed with a metric $d$ compatible with its topology for which it is complete. Let $(A_n)_{n\in\mathbf{N}}$ be an increasing sequence of closed subsets of $P\times P$, with empty interiors, such that the graph $\Gamma_R$ of the relation R is contained in the union of the $A_n$.

Let $\mathscr{O}$ be the set of nonempty open subsets of P. We shall construct by induction a sequence $(f_n)_{n\in\mathbf{N}}$, where for every $n$, $f_n$ is a mapping of $\{0,1\}^n$ into $\mathscr{O}$, satisfying the following properties :

(i) For every $n\geqslant 1$, every $x\in  \{0,1\}^{n-1}$ and every $t\in  \{0,1\}$, the closure of the open set $f_n(x, t)$ is contained in $f_{n-1}(x)$;

(ii) For every $x\in  \{0,1\}^n$, one has diam($f_n(x)$)$\leqslant 2^{-n}$;

(iii) For every $n\geqslant 1$ and every pair $(x, x')$ of distinct elements of $\{0,1\}^n,f_n(x)\times f_n(x')$ does not meet $A_{n-1}$.

Choose a nonempty open set U of X of diameter $\leqslant 1$ and define $f_0$ as the constant mapping with image $\{U\}$. Suppose that the mappings $f_0, . . . , f_n$ have been constructed.

Let $p:\{0,1\}^{n+1}\rightarrow  \{0,1\}^n$ be the mapping defined by $p(x_0, . . . , x_n) =$ $(x_0, . . . , x_{n-1})$. By lemma 3 above, applied to the family of open sets $(f_n(p(x)))$ for $x\in  \{0,1\}^{n+1}$ and to the dense open set $\complement A_n$ of $P\times P$, there exists a family $(g(x))_{x\in \{0,1\}^{n+1}}$ of nonempty open sets of P such that $g(x)\subset f_n(p(x))$ for every $x$ and such that $(g(x)\times g(x'))\cap A_n$ be empty for every pair $(x, x')$ of distinct elements of $\{0,1\}^{n+1}$. One then defines the mapping $f_{n+1}$ by choosing, for each element $x\in  \{0,1\}^{n+1}$, a nonempty open subset of $g(x)$ whose diameter is $\leqslant 2^{-n-1}$ and whose closure is contained in $g(x)$.

For every element $x= (x_n)_{n\in\mathbf{N}}$ of $\{0,1\}^{\mathbf{N}}$, the sequence of sets $(f_n(x_0, . . . , x_{n-1}))_{n\in\mathbf{N}}$ is a decreasing sequence of open subsets of X each of which contains the closure of the next and whose diameter tends to 0; the intersection of this sequence of sets is therefore reduced to a point (TG, II, p. 15), which we denote by $f(x)$. If two points $x,x'$ of $\{0,1\}^{\mathbf{N}}$ satisfy $x_i=x'_i$ for $i\leqslant n$, one has $d(f(x), f(x'))\leqslant 2^{-n}$. Consequently, the mapping $f:\{0,1\}^{\mathbf{N}}\rightarrow P$ is continuous. Let $x$ and $x'$ be distinct elements of $\{0,1\}^{\mathbf{N}}$. For $n\in \mathbf{N}$ such that $(x_0, . . . , x_n)=\not$ $(x'_0, . . . , x'_n)$, the open set $f_{n+1}(x_0, . . . , x_n)\times f_{n+1}(x'_0, . . . , x'_n)$ is disjoint from $A_n$, by definition of $f_{n+1}$, hence the pair $(f(x), f(x'))$ does not belong to $A_n$. It follows that $f(x)$ and $f(x')$ are not equivalent for the relation R. Consequently, $f$ is injective and its image meets each equivalence class for R in at most one point. The proposition is thus proved.

### 6. Cardinal of Poincaré groups

#### Proposition 9 {#ta-iv-s2-prop-9 .statement tag=021H}

Let X be an unravelable topological space and let $\mathscr{W}$ be a basis for the topology of X. For every point $x$ of X, the cardinal of the group $\pi_1(X, x)$ is bounded above by sup(Card($\mathscr{W}$), Card($\mathbf{N}$)). In particular, the Poincaré group of a metric space of countable type and unravelable is countable.

In fact, the space $\lambda_x(X)$ endowed with the endpoint mapping is a connected covering of X whose fibre at $x$ is $\pi_1(X, x)$. The assertion then results from I, p. 40, th. 3.

#### Lemma 4 {#ta-iv-s2-lem-4 .statement tag=021I}

Let X be a Baire space, let G be a topological group acting continuously on X and let B be an approachable subset of X which is not meagre. The set of points $g\in G$ such that $B\cap gB=\not\emptyset$ is a neighbourhood of the identity element of G.

Since B is approachable, $\complement B$ is also approachable, for the set of approachable subsets of X is a tribe. Hence there exists an open subset U of X such that $U\cap \complement B$ and $B\cap \complement U$ are meagre in X.

Let V be a neighbourhood of the identity element of G and W a nonempty open subset of X contained in U such that $V\cdot W\subset U$. For every $g\in V$, $U\cap gU$ is nonempty.

Let $g\in G$ be such that $B\cap gB$ is empty. The relations

$$
U\cap gU = (U\cap gU)\cap \complement (B\cap gB)
$$

$$
= (U\cap gU)\cap (\complement B\cup g\complement B)
$$

$$
= (U\cap gU\cap \complement B)\cup (U\cap gU\cap g\complement B)
$$

$$
\subset (U\cap \complement B)\cup g(U\cap \complement B)
$$

imply that $U\cap gU$ is meagre in X. Since this is an open subset and X is a Baire space, it is empty. Hence $g\notin V$, which proves the lemma.

#### Theorem 2 (Shelah[^1]) {#ta-iv-s2-thm-2 .statement tag=021J}

Let X be a connected Polish space which is locally connected by arcs, and let $x$ be a point of X. If X is not unravelable, the group $\pi_1(X, x)$ has the power of the continuum.

Let $d$ be a metric defining the topology of X for which it is complete. Suppose that X is not unravelable. Then there exists a point $a\in X$ and, for every integer $n\geqslant 0$, a loop $c_n$ at $a$ in X whose image has diameter $\leqslant 2^{-n}$ and whose class in $\pi_1(X, a)$ is nontrivial.

Let us denote by K the set $\{0,1\}^{\mathbf{N}}$ and endow it with the product topology, the space $\{0,1\}$ being endowed with the discrete topology. For every element $\varepsilon = (\varepsilon_n)$ of K, let $c_{\varepsilon}$ be the mapping of $\mathbf{I}$ into X defined by $c_{\varepsilon}(0) =a$ and, for $2^{-n-1}\leqslant t\leqslant 2^{-n},c_{\varepsilon}(t) =c_n(2^{n+1}t-1)$ if $\varepsilon_n= 1$ and $c_{\varepsilon}(t) =a$ otherwise. One has $c_{\varepsilon}(0) =c_{\varepsilon}(1) =a$. The mapping $c_{\varepsilon}$ is continuous at every point $t\in ]0,1]$. It is also so at 0, since $d(a, c_{\varepsilon}(t))\leqslant 2^{-n}$ if $t\in [0,2^{-n}]$. The mapping $c_{\varepsilon}$ is therefore a loop in X at $a$.

If $\varepsilon$ and $\varepsilon '$ are elements of K such that $(\varepsilon_0, . . . , \varepsilon_n) = (\varepsilon '_0, . . . , \varepsilon '_n)$, then $c_{\varepsilon}(t) =c_{\varepsilon'}(t)$ for every $t\in [2^{-n-1},1]$ and $d(c_{\varepsilon}(t), c_{\varepsilon'}(t))\leqslant$ $d(a, c_{\varepsilon}(t)) +d(a, c_{\varepsilon'}(t))\leqslant 2^{-n}$ if $t\in [0,2^{-n-1}]$. It follows that the mapping $\varepsilon \mapsto c_{\varepsilon}$ of K into the space $\Omega_a(X)$ is continuous, when the space $\Omega_a(X)$ is endowed with the topology of compact convergence.

Let $\Gamma \subset K\times K$ denote the set of pairs $(\varepsilon , \varepsilon ')$ such that $c_{\varepsilon}$ is strictly homotopic to $c_{\varepsilon'}$. It is the graph of an equivalence relation R in K.

#### Lemma 5 {#ta-iv-s2-lem-5 .statement tag=021K}

The set Γ is a meagre subset of $K\times K$.

Let Z denote the space $K\times K\times \mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$. The topology of the space $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ is defined by the distance $\delta$ given by $\delta (h, h') =$ sup$_{u\in\mathbf{I}\times\mathbf{I}}d(h(u), h'(u))$ and it is complete for this distance (TG, X, p. 20, corollaire and TG, X, p. 9, cor. 1); after TG, X, p. 24, th. 1, this topology is of countable type. The space $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ is therefore a Polish space. The same is true of the space Z, for K is a Polish space (TG, IX, p. 57, prop. 1).

Let H be the subset of Z consisting of the triples $(\varepsilon , \varepsilon ', h)$ such that $h$ is a strict homotopy joining $c_{\varepsilon}$ to $c_{\varepsilon'}$. The mappings from Z into $X^2$ given by $a_t: (\varepsilon , \varepsilon ', h)\mapsto (c_{\varepsilon}(t), h(t,0)),b_t: (\varepsilon , \varepsilon ', h)\mapsto$ $(c_{\varepsilon'}(t), h(t,1))$ and $c_t: (\varepsilon , \varepsilon ', h)\mapsto (h(0, t), h(1, t))$ are continuous, for every $t\in \mathbf{I}$, because the mapping $\varepsilon \mapsto c_{\varepsilon}$ from K into $\Omega_a(X)$ is continuous, and analogously the mappings $h\mapsto h(s, t)$ from $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ into X.

By definition, H is the intersection of the sets $\overset{-1}{a_{t}}(\Delta_X),\overset{-1}{b_{t}}(\Delta_X)$ and $\overset{-1}{c_{t}}((a, a))$, for $t\in \mathbf{I}$, where $\Delta_X$ denotes the diagonal of X. This proves that H is a closed subset of Z.

It follows that H is a Polish space. Let $p: Z\rightarrow K\times K$ be the canonical projection; we have $\Gamma  =p(H)$ by definition. Since $K\times K$ is separated, Γ is a Souslin subset of $K\times K$ (TG, IX, p. 59, déf. 2). After IV, p. 362, prop. 7, it is an approachable subset of $K\times K$.

Suppose that Γ is not meagre. The space $K\times K$ is a compact topological space and therefore a Baire space (TG, IX, p. 55, th. 1). Endow the group $G_0$ of permutations of the set $\{0,1\}$ with the discrete topology; let the product topological group $G = G^{\mathbf{N}}_0$ operate diagonally in $K =\{0,1\}^{\mathbf{N}}$. The group G then operates continuously in $K\times K$ by the mapping $(g,(x, y))\mapsto (x, g\cdot y)$. After Lemma 4, the set V of elements $g\in G$ such that $\Gamma \cap g\cdot \Gamma =\not\emptyset$ is a neighbourhood of the identity element of G.

Let $g\in V$; let $(\varepsilon , \varepsilon ')\in \Gamma \cap g\Gamma$. Since $(\varepsilon , \varepsilon ')\in \Gamma$, we have $R\{\varepsilon , \varepsilon '\}$; since $(\varepsilon , \varepsilon ')\in g\Gamma ,g^{-1}\cdot (\varepsilon , \varepsilon ') = (\varepsilon , g^{-1}\varepsilon ')\in \Gamma$, so that $R\{\varepsilon , g^{-1}\varepsilon '\}$. We have thus proved that, for every $g\in V$, there exists $\varepsilon \in K$ such that $\varepsilon$ and $g\varepsilon$ are equivalent for R.

For $m\in \mathbf{N}$, let $\tau_m$ denote the element of G all of whose terms are equal to $e$ except that with index $m$, which is equal to the nontrivial element $\tau$ of $G_0$. There exists an integer $m$ such that $\tau_m$ belongs to V; let then $\varepsilon \in K$ be such that $\varepsilon$ and $\varepsilon '=\tau_m\cdot \varepsilon$ are equivalent for R. This implies that the loops $c_{\varepsilon}$ and $c_{\varepsilon'}$ are strictly homotopic. By construction, these loops coincide on the intervals $[0,2^{-m-1}]$ and $[2^{-m},1]$; on the interval $[2^{-m-1},2^{-m}]$, one is the constant mapping with image $a$ and the other is the mapping $t\mapsto c_m(2^{m+1}t-1)$. It follows that $c_m$ is strictly homotopic to the constant loop with image $\{a\}$, hence a contradiction. Lemma 5 is thus proved.

Let us now complete the proof of theorem 2. By Prop. 8, there exists a continuous injective mapping $\gamma$ of $\{0,1\}^{\mathbf{N}}$ into K whose image meets each equivalence class for R in at most one point. If $k$ and $k'$ are distinct elements of $\{0,1\}^{\mathbf{N}}$, the loops $c_{\gamma(k)}$ and $c_{\gamma(k')}$ are not strictly homotopic in X, and the mapping $\{0,1\}^{\mathbf{N}}\rightarrow \pi_1(X, a)$ given by $k\mapsto [c_{\gamma(k)}]$ is injective. In particular, Card($\pi_1(X, a)$)$\geqslant$ Card($\{0,1\}^{\mathbf{N}}$) $=$ Card($\mathfrak{P}(\mathbf{N})$). Since X is a metrizable topological space of countable type, the same is true of $\Omega_a(X)$ (TG, X, p. 24, th. 1). Hence $\Omega_a(X)$ is homeomorphic to a subspace of $[0,1]^{\mathbf{N}}$ (TG, IX, p. 18, prop. 12) and

Card(Ω$_a(X)$)$\leqslant$ Card([0$,1]^{\mathbf{N}}$) $=$ Card($\mathfrak{P}(\mathbf{N})^{\mathbf{N}}$)

= Card($\mathfrak{P}(\mathbf{N}\times \mathbf{N})$) $=$ Card($\mathfrak{P}(\mathbf{N})$).

A fortiori, Card($\pi_1(X, a)$)$\leqslant$ Card($\mathfrak{P}(\mathbf{N})$). It then follows from Cor. 2 of E, III, p. 25, that $\pi_1(X, a)$ has the power of the continuum, which was to be proved.

#### Example {#ta-iv-s2-n6-exa-1 .statement tag=021L}

Let P be the topological space which is the union of the circles with center $(2/n,0)$ passing through the origin of the plane $\mathbf{R}^2$, for $n\geqslant$ 1 (III, p. 336, Exercise 6). The Poincaré group of P has the power of the continuum (III, p. 338, Exercise 9).

## EXERCISES {#ta-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: See "Can the fundamental (homotopy) group of a space be the rationals ?", Proc. Amer. Math. Soc. 103 (1988), No. 2, p. 627–632. The proof which follows is based on the article by J. Pawlikowski, "The fundamental group of a compact metric space", Proc. Amer. Math. Soc. 126 (1998), No. 10, p. 3083–3087.
