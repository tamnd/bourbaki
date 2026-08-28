---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 4
section_title: Revêtements
lang: en
source: ta-i-iv-fr
book_pages: TA I.68-TA I.90, TA I.145-TA I.147
pdf_pages: 0084-0106, 0161-0163
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés localement triviaux
      page: 68
      pdf_page: 84
    - "no": 2
      title: Revêtements
      page: 69
      pdf_page: 85
    - "no": 3
      title: Produits et produits fibrés
      page: 71
      pdf_page: 87
    - "no": 4
      title: Degré d’un revêtement
      page: 73
      pdf_page: 89
    - "no": 5
      title: Revêtements finis
      page: 75
      pdf_page: 91
    - "no": 6
      title: Revêtements des espaces localement connexes
      page: 79
      pdf_page: 95
    - "no": 7
      title: Revêtements d’un espace paracompact
      page: 84
      pdf_page: 100
    - "no": 8
      title: Faisceaux localement constants
      page: 86
      pdf_page: 102
    - "no": 9
      title: Produits de faisceaux localement constants
      page: 87
      pdf_page: 103
    - "no": 10
      title: Morphismes de faisceaux localement constants sur un espace localement connexe
      page: 89
      pdf_page: 105
statements: 50
exercises: 9
content_sha256: 28a8ab4dfdce641c77cb1c35e6e3d45d59595535573c27956687c039fb452550
translated_from: content/fr/ta/I/04_s4_revetements.md
source_lang: fr
translation_method: machine
source_content_sha256: fec85f8311822c8b3f0a7be940cb84e71931964b3bf2f7e600f3761918a89a4e
translation_model: gpt-5.4
translation_run: translate-en-mt-08f23ce1
glossary_version: 34
glossary_terms_sha256: 505f9e0f4f180029cc86790a5e1c146a94676c5dd6648d161ac793aa34d17fee
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. COVERINGS

### 1. Locally trivial fibre spaces

Let B be a topological space. If F is a topological space, the B-space $(B\times F$, pr$_1)$ is called a trivial fibred B-space of fibre type F.

Let E be a B-space. If there exist a topological space F and a B-isomorphism $u: E\rightarrow B\times F$, we say that the B-space E is a trivializable fibred B-space and that $u$ is a trivialization of it of fibre type F.

#### Definition 1 {#ta-i-s4-def-1 .statement tag=01OR}

Let B be a topological space. Let E be a B-space and let $p$ be its projection. We say that E is a locally trivial fibred B-space if every point of B possesses a neighbourhood V such that $(\overset{-1}{p}(V), p_V)$ is a trivializable fibred V-space.

Instead of saying "locally trivial fibred B-space", we also say "locally trivial fibre space with base B". If E is a locally trivial fibred B-space, we sometimes say that $(E,B, p)$ is a locally trivial fibration, or, by abuse, that $p$ is a locally trivial fibration. We also say that a B-space $(E, p)$ is trivializable over a subset A of B if the A-space $E_A$ induced by $(E, p)$ over A is a trivializable fibre space.

Let E be a locally trivial fibred B-space; let us denote by $p$ its projection.

The set of points $a$ of B such that the fibre $\overset{-1}{p}(a)$ is empty (resp. nonempty) is open. The image of $p$ is therefore an open and closed subset of B.

Let F be a topological space. If all the fibres of E are homeomorphic to F, we say that E is a locally trivial fibred B-space of fibre type F.

#### Remark 1 {#ta-i-s4-n1-rem-1 .statement tag=01OS}

Let $(E, p)$ be a locally trivial fibred B-space and let A be a subset of B. The A-space $E_A= (\overset{-1}{p}(A), p_A)$ deduced from E by passing to the subspaces is a locally trivial fibre space. If E is trivializable, the same is true of $E_A$.

In fact, for every point $a$ of A, there exist an open neighbourhood U of $a$ in B, a topological space F and a U-isomorphism $g:\overset{-1}{p}(U)\rightarrow$ $U\times F$. The mapping $f$ induces an $(A\cap U)$-isomorphism of $p^{-1}_A(A\cap U)$ onto $(A\cap U)\times F$, which proves that $E_A$ is a locally trivial fibred A-space.

#### Remark 2 {#ta-i-s4-n1-rem-2 .statement tag=01OT}

Let $(E, p)$ be a B-space and let $(E_i)_{i\in I}$ be a partition of E consisting of open sets.

If each of the B-spaces $(E_i, p|E_i)$ is a trivializable fibre space, E is a trivializable fibred B-space. In fact, for each $i\in I$, let $F_i$ be a topological space such that the B-spaces $(E_i, p|E_i)$ and $(B\times F_i$, pr$_1)$ are isomorphic. Then the B-space $(E, p)$ is isomorphic to $(B\times F$, pr$_1)$, where F is the topological space sum of the family $(F_i)_{i\in I}$.

Suppose the set I finite. If each of the B-spaces $(E_i, p|E_i)$ is a locally trivial fibred B-space, the same is true of the B-space E. In fact, since the set I is finite, every point of B possesses a neighbourhood U above which the fibred B-spaces $E_i$ are all trivializable. By what precedes, the U-space $(\overset{-1}{p}(U), p_U)$ is then a trivializable fibre space.

### 2. Coverings

#### Definition 2 {#ta-i-s4-def-2 .statement tag=01OU}

A covering is a locally trivial fibre space all of whose fibres are discrete.

Instead of saying that a B-space E is a covering, we also say that E is a covering of B.

Let E be a B-space, and let us denote by $p$ its projection; let A be a subset of B. If E is a covering of B, the fibres of $p$ are discrete, hence so are those of $p_A:\overset{-1}{p}(A)\rightarrow A$, and the locally trivial fibred A-space $(\overset{-1}{p}(A), p_A)$ is a covering.

#### Proposition 1 {#ta-i-s4-prop-1 .statement tag=01OV}

Let B and E be topological spaces and let $p: E\rightarrow B$ be a mapping. The following conditions are equivalent:

(i) The mapping $p$ is continuous and the B-space $(E, p)$ is a trivializable covering;

(ii) There exists a partition $(V_i)_{i\in I}$ of E consisting of open sets such that, for every $i\in I$, the mapping $p|V_i: V_i\rightarrow B$ is a homeomorphism.

Suppose that condition (i) is satisfied, and let $g: E\rightarrow B\times F$ be a trivialization of the B-space $(E, p)$, of fibre type F. Then F is a discrete topological space and the sets $V_i=\overset{-1}{g}(B\times  \{i\})$, for $i\in F$, form a partition of E consisting of open sets. For every $i$, the mapping $p|V_i: V_i\rightarrow B$ is a homeomorphism, with reciprocal homeomorphism the mapping $x\mapsto g^{-1}(x, i)$, whence condition (ii).

Conversely, suppose that condition (ii) is satisfied. The mapping $p$ is then continuous. Consider the mapping from E into $B\times I$ which associates to $x\in E$ the pair $(p(x), i)$, where $i$ is the unique element of I such that $x\in V_i$. If I is endowed with the discrete topology, condition (ii) means that this mapping is a B-isomorphism and the B-space $(E, p)$ is a trivializable covering.

#### Corollary 1 {#ta-i-s4-prop-1-cor-1 .statement tag=01OW}

Let B and E be topological spaces and let $p: E\rightarrow B$ be a mapping. In order that E, endowed with the mapping $p$, be a covering of B, it is necessary and sufficient that, for every point $a$ of B, there exist an open neighbourhood U of $a$ and a partition $(V_i)_{i\in I}$ of $\overset{-1}{p}(U)$ consisting of open sets of E such that, for every $i\in I$, the mapping $p$ induces a homeomorphism of $V_i$ onto U.

#### Remark {#ta-i-s4-n2-rem-1 .statement tag=01OX}

Let B be a topological space. Let E be a B-space and let $p$ be its projection. If E is a covering of B, it follows from corollary 1 above that the mapping $p$ is étale (I, p. 28, Def. 2) and separated (I, p. 25, Prop. 1, (iii)). These conditions do not suffice, however, to ensure that E is a covering. Consider, for example, an open set U of B. The canonical injection $i: U\rightarrow B$ is étale and separated. In order that the B-space $(U, i)$ be a covering, it is necessary and sufficient that the open set U be also closed.

#### Corollary 2 {#ta-i-s4-prop-1-cor-2 .statement tag=01OY}

Let B be a topological space, let E be a B-space and let $p$ be its projection. Suppose that $p$ is étale and separated and that the space B is connected. In order that E be a trivializable covering of B, it is necessary and sufficient that, for every point $x$ of E, there exist a continuous section $s: B\rightarrow E$ of $p$ such that $s\circ p(x) =x$.

This is obviously necessary. Conversely, for every continuous section $s$ of $p$, the set $s(B)$ is open and the mapping $p$ induces a homeomorphism of $s(B)$ onto B (I, p. 30, Cor. 3 of Prop. 6). Moreover, when $s$ ranges over the set $\mathscr{S}(B; E)$ of sections of $p$, the sets $s(B)$ are pairwise disjoint, since B is connected (I, p. 34, Cor. 1 of Prop. 11). It then follows from proposition 1 that if the sets $s(B)$ cover E, the space E is a trivializable covering of B.

### 3. Products and Fibred Products

#### Proposition 2 {#ta-i-s4-prop-2 .statement tag=01OZ}

Let B and $B'$ be topological spaces, let $(E, p)$ be a B-space and let $(E', p')$ be a $B'$-space. Suppose that E and $E'$ are locally trivial fibre spaces ( resp. coverings). The space $E\times E'$, endowed with the mapping $p\times p': E\times E'\rightarrow B\times B'$, is then a locally trivial fibre space ( resp. a covering) with base $B\times B'$. If E and $E'$ are trivializable, so is $E\times E'$.

Suppose first that the B-space E and the $B'$-space $E'$ admit trivializations $g: E\rightarrow B\times F,g': E'\rightarrow B'\times F'$; the composite of the homeomorphism $g\times g'$ of $E\times E'$ onto $(B\times F)\times (B'\times F')$ and of the canonical homeomorphism of $(B\times F)\times (B'\times F')$ onto $(B\times B')\times (F\times F')$ is a trivialization of the $B\times B'$-space $E\times E'$, of fibre-type $F\times F'$. If F and $F'$ are discrete spaces, the space $F\times F'$ is also discrete.

In the general case, for every point $(a, a')$ of $B\times B'$, there exists a neighbourhood U of $a$ in B and a neighbourhood $U'$ of $a'$ in $B'$ such that the U-space $E_U$ and the $U'$-space $E'_{U'}$ are trivializable. It follows from the foregoing that the $B\times B'$-space $E\times E'$ is trivializable over $U\times U'$. Hence it is a locally trivial fibre space with base $B\times B'$. Its fibres are discrete if E and $E'$ are coverings, whence the proposition.

It should be observed that, if $(p_i: E_i\rightarrow B_i)_{i\in I}$ is a family of locally trivial fibre spaces, or even of coverings, the product space $\prod_{i\in I}E_i$ endowed with the mapping $(p_i)_{i\in I}$ is not necessarily a locally trivial fibre space with base $\prod_{i\in I}B_i($I, p. 145, Exercise 3).

#### Corollary 1 {#ta-i-s4-prop-2-cor-1 .statement tag=01P0}

Let A be a topological space, B, $B'$ A-spaces. Let E and $E'$ be locally trivial fibre spaces ( resp. coverings) with bases B and $B'$; let $p$ and $p'$ denote their projections. The $B\times_AB'$-space $E\times_AE'$ obtained from $p\times p'$ by passing to the subspaces is then a locally trivial fibre space ( resp. a covering). It is trivializable if E and $E'$ are.

Since the set $E\times_AE'$ is the inverse image of $B\times_AB'$ by the mapping $p\times p': E\times E'\rightarrow B\times B'$, the corollary follows from proposition 2 and remark 1 (I, p. 68).

#### Corollary 2 {#ta-i-s4-prop-2-cor-2 .statement tag=01P1}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. If $(E, p)$ is a locally trivial fibre B-space ( resp. a covering), then $(E', p')$ is a locally trivial fibre space ( resp. a covering) with base $B'$, trivializable if $(E, p)$ is.

This follows from corollary 1, applied with B = A and $E'= B'$.

#### Corollary 3 {#ta-i-s4-prop-2-cor-3 .statement tag=01P2}

Let B be a topological space. Let E and $E'$ be locally trivial fibre B-spaces ( resp. coverings). Then $E\times_BE'$ is a locally trivial fibre B-space ( resp. a covering of B). It is trivializable if E and $E'$ are.

This follows from corollary 1, applied to the case where A, B and $B'$ are equal.

#### Proposition 3 {#ta-i-s4-prop-3 .statement tag=01P3}

Let

${E'}^{f'}$ E

$$
p'p \tag{1}
$$

${B'}^f$ B

be a cartesian square. Suppose that in a neighbourhood of every point of B, the mapping $f$ has a continuous section. Then, if $(E', p')$ is a locally trivial fibre $B'$-space ( resp. a covering), the B-space $(E, p)$ is a locally trivial fibre space ( resp. a covering).

It is a question of proving that every point $a$ of B possesses a neighbourhood U such that the U-space induced by $(E, p)$ over U is a locally trivial fibre space (resp. a covering). Take for U a neighbourhood of $a$ over which there exists a continuous section $s$ of $f$. Let $i: U\rightarrow B$ and $j:\overset{-1}{p}(U)\rightarrow E$ denote the canonical injections. Since square (1) is cartesian, there exists a unique continuous mapping $s':\overset{-1}{p}(U)\rightarrow E'$ such that $f'\circ s'=j$ and $p'\circ s'=s\circ p_U$. The square

$$
\overset{-1}{p}(U)^{s'}E'
$$

$$
p_{_U}p' \tag{2}
$$

U $^sB'$

is thus commutative and its composite with square (1) is the cartesian square

$\overset{-1}{p}(U)^j$ E

$p_Up$

U $^iB$.

By proposition 7 of I, p. 15, square (2) is cartesian. Corollary 2 permits one to conclude.

#### Remark {#ta-i-s4-n3-rem-1 .statement tag=01P4}

If, in proposition 3, one weakens the hypothesis on the mapping $f$ by supposing it only universally strict and surjective, and if $p'$ is a covering, the mapping $p$ is etale (I, p. 31, prop. 8) and separated (I, p. 27, prop. 4), but E is not necessarily a covering of B. One can find, for example, a topological space B and a locally finite closed covering $(A_i)_{i\in I}$ of B, a B-space $(E, p)$ which is not a covering but such that, for every $i\in I$, the induced $A_i$-space $E_{A_i}$ is a covering of $A_i($I, p. 146, exerc. 5). For a sufficient condition, see however corollary 4 of I, p. 77.

### 4. Degree of a covering

Let B be a topological space, let E be a covering of B, and let us denote by $p$ its projection. Let us denote by C the set of cardinals Card($\overset{-1}{p}(b)$), where $b$ ranges over B. The mapping $b\mapsto$ Card($\overset{-1}{p}(b)$) is a locally constant mapping of B into C. One says that the covering E has a degree if B is nonempty and if the mapping $b\mapsto$ Card($\overset{-1}{p}(b)$) is constant. The common value of the cardinals Card($\overset{-1}{p}(b)$), for $b\in B$, is then called the degree of the covering E and is denoted deg(E$, p$), or even [E: B] if there cannot be any ambiguity about the mapping $p$.

If B is nonempty, the trivial covering with base B and fibre-type F has a degree equal to Card(F).

If B is connected, the function $b\mapsto$ Card($\overset{-1}{p}(b)$) is constant. Hence:

#### Proposition 4 {#ta-i-s4-prop-4 .statement tag=01P5}

Every covering of a nonempty connected space has a degree.

Let G be a topological space, let $(F, g)$ be a covering of G and let $(E, f)$ be a covering of F; suppose that these coverings have a degree. If the G-space $(E, g\circ f)$ is a covering, then it has a degree and one has deg(E$, g\circ f$) $=$ deg(F$, g$) deg(E$, f$), which can also be written

$$
[E : G] = [E : F] [F : G]
$$

In fact, if $z$ is a point of G, all the fibres of the mapping

$$
f_{\overset{-1}{g}(z)}:\overset{-1}{f}(\overset{-1}{g}(z))\rightarrow \overset{-1}{g}(z)
$$

have for cardinal deg(E$, f$), and $\overset{-1}{g}(z)$ has for cardinal deg(F$, g$). The assertion therefore follows from the shepherds' principle (E, III, p. 41, prop. 9).

Let B and $B'$ be topological spaces, let $(E, p)$ be a covering of B and let $(E', p')$ be a covering of $B'$. Suppose that these coverings have a degree; then the covering $(E\times E', p\times p')$ of $B\times B'$ (I, p. 71, prop. 2) has a degree and one has:

deg(E $\times E', p\times p'$) $=$ deg(E$, p$) deg(E$', p'$).

In fact, for every pair $(b, b')\in B\times B'$, the fibre $(E\times E')_{(b,b')}$ is the product $E_b\times E'_{b'}$.

Let B and $B'$ be topological spaces, $(E, p)$ a covering of B, $(E', p')$ a covering of $B'$ and let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

a Cartesian square. If $B'$ is non-empty and if the covering $(E, p)$ has a degree, then the covering $(E', p')$ has a degree, equal to that of E, after I, p. 10, cor. of prop. 4.

### 5. Finite coverings

A covering is said to be locally finite if the cardinals of all its fibres are finite. A covering is said to be finite if the set of the cardinals of its fibres is bounded above by a finite cardinal.

#### Theorem 1 {#ta-i-s4-thm-1 .statement tag=01P6}

Let E, B be topological spaces and $p: E\rightarrow B$ a mapping. The following conditions are equivalent:

(i) The space E, endowed with the mapping $p$, is a locally finite covering of B;

(ii) The mapping $p$ is étale, proper and separated;

(iii) The mapping $p$ is continuous, open and separated, its fibres are finite, and the numerical function $b\mapsto$ Card($\overset{-1}{p}(b)$) is upper semicontinuous on B (TG, IV, p. 28).

We shall use the following lemma in the proof:

#### Lemma {#ta-i-s4-n5-lem-1 .statement tag=01P7}

Let X and Y be topological spaces. In order that a mapping $f: X\rightarrow Y$ be closed, it is necessary and sufficient that for every point $y$ of Y and every neighbourhood W of the fibre $\overset{-1}{f}(y)$, there exist a neighbourhood V

of $y$ such that W contain $\overset{-1}{f}(V)$.

In this statement, one may consider only the neighbourhoods W of $\overset{-1}{f}(y)$ which are open. Denoting by F the complement of W in Y, one may then reformulate the statement in the following way: in order that a mapping $f: X\rightarrow Y$ be closed, it is necessary and sufficient that, for every closed subset F of X, every point $y$ of Y which does not belong to $f(F)$ possess a neighbourhood V disjoint from $f(F)$. Now this assertion results immediately from the definition of a closed mapping (TG, I, p. 30, def. 1).

Let us now prove theorem 1. Each of the three conditions implies that the mapping $p$ is continuous, open and separated, and also that the fibres of $p$ are finite. This is clear under assumptions (i) and (iii); under assumption (ii), the fibres of $p$ are discrete (I, p. 29, remark 2) and quasi-compact (TG, I, p. 75, th. 1), hence finite (TG, I, p. 60, example 1).

(i)$\Rightarrow$(ii) : it is enough to prove that $p$ is proper and, for this, that for every open set U over which the covering $(E, p)$ is trivializable, the mapping $p_U:\overset{-1}{p}(U)\rightarrow U$ is proper (TG, I, p. 72, prop. 3). Since the fibres of $p_U$ are finite, the latter assertion results from Corollary 5 of TG, I, p. 77.

(ii)$\Rightarrow$(iii) : let $b$ be a point of B and, for every $x\in \overset{-1}{p}(b)$, let $W_x$ be an open neighbourhood of $x$ in E such that $p|W_x$ be injective. The set $W =\bigcup_{x\in\overset{-1}{p}(b)}W_x$ is an open neighbourhood of $\overset{-1}{p}(b)$. Since the mapping $p$ is closed, there exists by the above lemma an open neighbourhood U of $b$ such that $\overset{-1}{p}(U)\subset W$. For every $a\in U$, one has $\overset{-1}{p}(a)\subset W$; since the restriction of $p$ to each $W_x$ is injective, it follows that Card($\overset{-1}{p}(a)$)$\leqslant$ Card($\overset{-1}{p}(b)$), which proves the upper semicontinuity of the mapping $a\mapsto$ Card($\overset{-1}{p}(a)$).

(iii)$\Rightarrow$(i): let $b$ be a point of B. Since the fibre $E_b=\overset{-1}{p}(b)$ is finite and the mapping $p$ is separated, one can choose, for each $x\in E_b$, an open neighbourhood $V'_x$ of $x$ such that the $V'_x$ are pairwise disjoint (I, p. 26, remark 4). Since the mapping $p$ is open and the set $E_b$ finite, the set $U'=\bigcap_{x\in E_b}p(V'_x)$ is an open neighbourhood of $b$ in B. Let U be an open neighbourhood of $b$ in B, contained in $U'$ and such that for every $a\in U$, Card(E$_a$)$\leqslant$ Card(E$_b$). For each $x\in E_b$, put $V_x= V'_x\cap \overset{-1}{p}(U)$. Let $a$ be a point of U; the sets $E_a\cap V_x$, for $x\in E_b$, are non-empty and pairwise disjoint. Hence each of these sets contains a unique element and they form a partition of $E_a$. This shows that, for each $x\in E_b$, the mapping $p|V_x$ is injective and that one has $\overset{-1}{p}(U) =\bigcup_{x\in E_b}V_x$. Since the mapping $p$ is open, it induces a homeomorphism of $V_x$ onto U and consequently, $(E, p)$ is a covering of B (I, p. 70, cor. 1 of prop. 1).

#### Remark {#ta-i-s4-n5-rem-1 .statement tag=01P8}

A continuous, separated, open, proper mapping with finite fibres is not necessarily a covering. This is the case for the mapping $x\mapsto x^2$ of $\mathbf{R}$ into $[0; +\infty [$.

#### Corollary 1 {#ta-i-s4-thm-1-cor-1 .statement tag=01P9}

Let E and B be topological spaces and let $p: E\rightarrow B$ be a proper and separated mapping. The set U of points $b$ of B such that $p$ is étale at every point of the fibre $E_b$ is open in B. The U-space induced by $(E, p)$ over U is a locally finite covering.

The set F of points of E at which the mapping $p$ is not étale is closed in E (I, p. 29, remark 1). Its image $p(F)$ is closed since the mapping $p$ is proper; the complement U of $p(F)$ is therefore open. The mapping $p_U$ is separated (I, p. 27, prop. 4) and proper (TG, I, p. 72, prop. 3). By construction, the mapping $p_U$ is étale; it therefore satisfies condition (ii) of theorem 1.

#### Corollary 2 {#ta-i-s4-thm-1-cor-2 .statement tag=01PA}

Let B be a separated topological space and let E be a B-space. Suppose that E is compact and that its projection $p: E\rightarrow B$ is étale. Then, E is a finite covering of B.

The mapping $p$ is separated (I, p. 26, remark 2) and proper (TG, I, p. 76, cor. 2). By corollary 1, E is therefore a locally finite covering of B. Since E is compact, $p(E)$ is a quasi-compact subset of B; the mapping of $p(E)$ into $\mathbf{N}$ given by $b\mapsto$ Card $\overset{-1}{p}(b)$ being locally constant, it is bounded above (TG, IV, p. 30, corollary).

#### Corollary 3 {#ta-i-s4-thm-1-cor-3 .statement tag=01PB}

Let B be a topological space, let $(E, p)$ and $(E', p')$ be B-spaces and let $f: E'\rightarrow E$ be a B-morphism. Suppose that $E'$ is a locally finite covering of B.

a) If the mapping $p$ is étale and separated, the E-space $(E', f)$ is a covering.

b) If the mapping $f$ is surjective and makes the space $E'$ a covering of E, then E is a covering of B.

Under assumption a), the mappings $p$ and $p'$ are etale and separated, and the mapping $p'$ is proper (theorem 1). The mapping $f$ is therefore etale (I, p. 30, cor. 1 of prop. 6), separated (I, p. 25, prop. 2 b)) and proper (I, p. 28, prop. 5). By theorem 1, $(E', f)$ is a covering of E.

Now suppose that $f$ is surjective and that $(E', f)$ is a covering of E. Then it is locally finite, hence the mapping $f$ is proper and surjective (th. 1). By I, p. 25, prop. 2, c), the mapping $p$ is separated, since $p'=p\circ f$ and $p'$ is separated. The mapping $p$ is etale (I, p. 29, prop. 6, d)), proper (TG, I, p. 73, prop. 5, b)) and its fibres are finite. By th. 1, the B-space $(E, p)$ is then a covering of B.

#### Corollary 4 {#ta-i-s4-thm-1-cor-4 .statement tag=01PC}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B be a cartesian square. Suppose that $(E', p')$ is a locally finite covering of $B'$ and that the mapping $f$ is universally strict and surjective. Then $(E, p)$ is a locally finite covering of B.

In fact, the mapping $p$ is etale (I, p. 31, prop. 8), proper (I, p. 21, prop. 11) and separated (I, p. 27, prop. 4).

#### Corollary 5 {#ta-i-s4-thm-1-cor-5 .statement tag=01PD}

Let B be a connected topological space and let $(E, p)$ be a finite covering of B. The space E has only a finite number of connected components, and each of them is a covering of B.

The result is true if B is empty; henceforth we assume it nonempty.

If X is an open and closed subset of E, the restriction of $p$ to X is a separated mapping (I, p. 25, prop. 2, a) and I, p. 26, remark 1), etale and proper (TG, I, p. 74, corollary 1); by theorem 1, $(X, p)$ is a locally finite covering of B. Since B is connected, this covering has finite degree. If X is distinct from E, there exists a point $b\in B$ such that $X_b(E_b$, whence $[X : B]<[E : B]$ because B is connected. It follows that every decreasing sequence of open and closed sets in E is stationary.

Let $x\in E$; then there exists a smallest open and closed subset X of E containing $x$ (E, III, p. 51, prop. 6). Such a set X is connected; it is therefore the connected component of $x$ in E. This shows that the connected components of E are open and closed and that each of them is a covering of B. Since B is connected, each connected component of E meets each fibre of $p$; the connected components of E are therefore finite in number.

#### Proposition 5 {#ta-i-s4-prop-5 .statement tag=01PE}

Let B be a topological space, let E and $E'$ be B-spaces, and let $f: E'\rightarrow E$ be a B-morphism. We assume that E is a locally finite covering and that the space $E'$, endowed with the mapping $f$, is a locally trivial fibred E-space ( resp. a covering). Then, $E'$ is a locally trivial fibred B-space ( resp. a covering).

Let us denote by $p$ and $p'$ the respective projections of the B-spaces E and $E'$. Let $b$ be a point of B. There exists an open neighbourhood U of $b$ in B and a finite partition $(V_i)_{i\in I}$ of $\overset{-1}{p}(U)$ formed of open sets of E such that, for every $i\in I$, the mapping $p$ induces a homeomorphism of

$V_i$ onto U. Put $V'_i=\overset{-1}{f}(V_i)$. The sets $V'_i$ are open in $E'$,

form a partition of $(^-{p'}^1)(U)$ and the mapping from $V'_i$ to U deduced from $p'$ by passing to the subspaces makes $V'_i$ into a locally trivial fibred U-space. It follows that the space $(^-{p'}^1)(U)$, endowed with the mapping

$p'_U:(^-{p'}^1)(U)\rightarrow U$, is a locally trivial fibred U-space (I, p. 69, remark 2). If $(E', f)$ is a covering of E, the fibres of $p'_U$ are discrete because their intersections with each of the open sets $V'_i$ are so. This completes the proof.

#### Remark {#ta-i-s4-n5-rem-2 .statement tag=01PF}

If $(E, p)$ is a covering of B and if $(E', f)$ is a covering of E, the mapping $p\circ f$ is étale (I, p. 29, prop. 6, a)) and separated (I, p. 25, prop. 2, a)). But it can happen, see exercise 5, b) of I, p. 146, that the space $E'$, endowed with the mapping $p\circ f$, is not a covering of B. See however IV, p. 342, prop. 3.

### 6. Coverings of Locally Connected Spaces

Let B be a topological space and let E be a B-space. Suppose that its projection $p$ is an étale and separated mapping.

If the space B is locally connected, the space E is locally connected. If the space E is locally connected, the open subset $p(E)$ of B (cf. I, p. 29, remark 2) is locally connected.

The image $s(B)$ of every section $s$ of $p$ is open (I, p. 30, cor. 3) and closed in B (I, p. 27, prop. 3). If B is connected and nonempty, it is therefore a connected component of E; in general, it is a union of connected components of E.

If B is locally connected, the union of the images of the sections of $p$ is therefore an open and closed subset of E (cf. TG, I, p. 85).

Suppose that E is a trivializable covering of B and let $g: E\rightarrow B\times F$ be a trivialization. If the space B is connected, the sets $V_x=\overset{-1}{g}(B\times  \{x\})$, for $x$ ranging over F, are the connected components of E (cf. prop. 1 of I, p. 69).

#### Proposition 6 {#ta-i-s4-prop-6 .statement tag=01PG}

Let B be a topological space and let E be a B-space; let us denote by $p$ its projection. Suppose that the space E is locally connected. In order that E be a covering of B, it is necessary and sufficient that every point of B possess an open neighbourhood U such that the mapping $p$ induce a homeomorphism of every connected component of $\overset{-1}{p}(U)$ onto U.

Let $b$ be a point of B. If E is a covering of B, every open neighbourhood U of $b$ which is connected and over which the covering E is trivializable satisfies the conditions stated in the proposition. Conversely, let U be an open neighbourhood of $b$ satisfying these conditions. The set $\overset{-1}{p}(U)$ is open; its connected components are open subsets of E (TG, I, p. 85, prop. 11) and constitute a partition of $\overset{-1}{p}(U)$. The proposition therefore follows from corollary 1 (I, p. 70) to proposition 1.

#### Corollary 1 {#ta-i-s4-prop-6-cor-1 .statement tag=01PH}

Let B be a locally connected topological space, let $(E, p)$ be a covering of B and let $E'$ be an open and closed subset of E. The B-space $(E', p|E')$ is a covering and $p(E')$ is open and closed in B.

The spaces E and $E'$ are locally connected. For every open subset U of B, the set $E'\cap \overset{-1}{p}(U)$ is open and closed in $\overset{-1}{p}(U)$, hence is a union of connected components of $\overset{-1}{p}(U)$. The open subsets U of B such that $p$ induce a homeomorphism of each connected component of $\overset{-1}{p}(U)$ onto U cover B. By the proposition, $p|E'$ makes $E'$ into a covering of B. The second assertion follows from this (cf. I, p. 68).

#### Corollary 2 {#ta-i-s4-prop-6-cor-2 .statement tag=01PI}

Let B be a locally connected topological space, let $(E, p)$, $(E', p')$ be coverings of B and let $f, g: E'\rightarrow E$ be B-morphisms. For every point $b$ of B, let us denote by $f_b, g_b: E_b\rightarrow E'_b$ the mappings deduced from $f$ and $g$ respectively. The set of points $b$ of B such that $f_b=g_b$ is open and closed in B.

Let X be the set of points $x$ of $E'$ such that $f(x) =g(x)$. It is the set of points where the liftings $f$ and $g$ of $p'$ to E coincide; therefore X is open and closed in $E'$ (prop. 11 of I, p. 34). The complement Y of X is also open and closed; consequently $p(Y)$ is open and closed in B (corollary 1). Its complement, which is the set of points $b$ of B such that $f_b=g_b$, is therefore so as well.

#### Corollary 3 {#ta-i-s4-prop-6-cor-3 .statement tag=01PJ}

Let B be a connected and locally connected topological space, let $(E, p)$ and $(E', p')$ be coverings of B. For every point $b$ of B, the mapping $f\mapsto f_b$ of $\mathscr{C}_B(E'; E)$ into $\mathscr{C}(E'_b; E_b)$ is injective.

Let $b$ be a point of B. Let $f$ and $g$ be B-morphisms from $E'$ into E such that $f_b=g_b$. The set of points $a$ of B such that $f_a=g_a$ is open and closed in B (Corollary 2) and contains $b$. It is therefore equal to B, and $f$ is equal to $g$.

#### Corollary 4 {#ta-i-s4-prop-6-cor-4 .statement tag=01PK}

Let B be a connected and locally connected topological space, let $(E, p)$ be a covering of B, and let $b$ be a point of B. In order that E be a trivializable covering, it is necessary and sufficient that every point of the fibre $E_b$ belong to the image of a continuous section of $p$.

The condition is necessary. Let $E'$ be the union of the images of the continuous sections of $p$, and let $E''$ be its complement in E. The set $E'$ is open and closed in E (cf. I, p. 79). Hence $(E', p|E')$ is a covering of B (Corollary 1), and this covering is trivializable by virtue of Corollary 2 (I, p. 70). Suppose that $E'$ contains $E_b$ and let us prove that $E''$ is empty. Since $E''$ is open and closed in E, $p(E'')$ is open and closed in B (Corollary 1). Since B is connected and $b$ does not belong to $p(E''),p(E'') =\emptyset$, hence $E''=\emptyset$.

#### Corollary 5 {#ta-i-s4-prop-6-cor-5 .statement tag=01PL}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. Suppose that the B-space $(E, p)$ is a covering and that the space $B'$ is connected and locally connected. Let $b'$ be a point of $B'$. In order that the $B'$-space $(E', p')$ be a trivializable covering, it is necessary and sufficient that for every point $x$ of E such that $p(x) =f(b')$, there exist a continuous lifting $g: B'\rightarrow E$ of $f$ such that $g(b') =x$.

Let us recall that $(E', p')$ is a covering of $B'($I, p. 71, Cor. 2) and that the mapping $f'$ induces a bijection $E'_{b'}\rightarrow E_{f(b')}($I, p. 10, Cor.). By Prop. 3 of I, p. 9, the mapping $s\mapsto f'\circ s$ defines a bijection between the set of continuous sections of $p'$ and the set of continuous liftings of $f$ to E. The corollary therefore follows from Corollary 4.

#### Proposition 7 {#ta-i-s4-prop-7 .statement tag=01PM}

Let B be a topological space, let E and $E'$ be B-spaces, and let $f: E'\rightarrow E$ be a B-morphism. It is assumed that $E'$ is a covering of B and that the space B is locally connected.

a) If the projection of the B-space E is an étale and separated mapping, $(E', f)$ is a covering of E.

b) If $f$ is surjective, then E is a covering of B.

Let $p$ and $p'$ denote the projections of the B-spaces E and $E'$ respectively. Under assumption a$),f$ is étale (I, p. 29, Prop. 6, c)). Under assumption b$),p$ is étale (loc. cit., d)). Hence, under either one of these two assumptions, E is locally connected; in particular, its connected components are open and closed in E (TG, I, p. 85, Prop. 11).

We shall first prove Proposition 7 under the additional assumption that B is connected, locally connected, and that $E'$ is the trivial covering $(B\times F'$, pr$_1)$.

#### Lemma {#ta-i-s4-n6-lem-1 .statement tag=01PN}

If U is a connected component of $E'$, the restriction of $f$ to U induces a homeomorphism of U onto a connected component of E.

Let $x\in F'$ be such that $U = B\times  \{x\}($cf. I, p. 79). The mapping from B into E which to $b\in B$ assigns $f(b, x)$ is a continuous section of $p$. Its image X is therefore connected and open in E, since $p$ is etale (I, p. 30, Corollary 3). It is moreover closed under assumption a), since $p$ is separated (I, p. 27, Proposition 3). It is also closed under assumption b) by Corollary 1 of I, p. 80, since U is open and closed in $E'$. Consequently, X is a connected component of E.

Since $f|U: U\rightarrow X$ is bijective and open, it is a homeomorphism onto its image, which proves the lemma.

Let us retain the assumptions preceding the lemma and now prove assertion a). Let V be a connected component of E. It is a

set open and closed in E and $\overset{-1}{f}(V)$ is a union of connected components of $E'$ which $f$ maps homeomorphically onto V by the lemma. It follows from Proposition 6 of I, p. 79 that $(E', f)$ is a covering.

Let us prove b). Since $f$ is surjective, it follows from the lemma that every connected component V of E is the homeomorphic image of a connected component $U = B\times \{x\}$ of $E'$. The mapping $p$ then induces a homeomorphism of V onto B. By Proposition 6, E is a covering of B.

This therefore proves the proposition, under the additional assumption that B is connected and $E'$ a trivializable covering of B. Let us prove it in the general case.

There exists a covering $(U_i)_{i\in I}$ of B, consisting of connected open sets over which the covering $E'$ is trivializable. Let $i\in I$.

Let us prove a). If the mapping $p$ is etale and separated, the same is true of the mapping $p_{U_i}: U_i\times_BE\rightarrow U_i$, for $i\in I$, by Propositions 8 of I, p. 31 and 4 of I, p. 27. It therefore follows from the particular case treated that,

for every $i\in I$, the $U_i$-space ($(^-{p'}^1)(U_i), f_{U_i}$) is a covering. Let A denote the sum space of the $U_i$ and $q: A\rightarrow B$ the canonical mapping. Then the space $A\times_BE'$, endowed with the mapping $f_A: A\times_BE'\rightarrow A\times_BE$ is a covering of $A\times_BE$. The mapping $q$ admits a continuous section in a neighbourhood of every point of B and Proposition 3 of I, p. 72, applied to the cartesian square

$$
A\times_BE'E'
$$

$$
_{f_A}f
$$

$A\times_BE$ E

implies that $E'$ is a covering of E.

Let us prove b). Suppose that $f$ is surjective. Then, for every element $i$ of I, the mapping $f_{U_i}: U_i\times_BE'\rightarrow U_i\times_BE$ is surjective and the space $U_i\times_BE'$, endowed with the mapping $f_{U_i}$, is a covering of $U_i\times_BE$ (I, p. 71, Corollary 2 of Proposition 2). It follows from the particular case treated above that the $U_i$-space $(\overset{-1}{p}(U_i), p_{U_i})$ is a covering. Consequently, E is a covering of B.

Let B be a topological space, let E and $E'$ be coverings of B, and let $f: E\rightarrow E'$ be a B-morphism We have seen that $(E, f)$ is a covering under each of the two following assumptions: 1) the covering E is locally of finite degree (I, p. 76, Corollary 1) ; 2) the space B is locally connected (I, p. 81, Proposition 7). This phenomenon may be explained as follows.

Let F and $F'$ be discrete topological spaces and let $f: B\times F\rightarrow$ $B\times F'$ be a B-morphism. The mapping $\widetilde{f}:a\mapsto$ pr$_2\circ f(b,\cdot )$ of B into the space $\mathscr{C}_c(F; F')$ is continuous (TG, X, p. 28, th. 3). If U is an open set of B such that the mapping $\widetilde{f}$ is constant on U, the mapping $f_U: U\times$ $F\rightarrow U\times F'$ deduced from $f$ is a trivializable covering (I, p. 69, prop. 1).

The space $\mathscr{C}_c(F; F')$ is none other than the set $\mathscr{F}(F; F')$ of mappings of F into $F'$ endowed with the topology deduced from the topology of the product space $(F')^F$ by the canonical identification. For this topology, the space $\mathscr{F}(F; F')$ is totally disconnected (I, p. 84, prop. 10). Consequently, if the space B is connected, the mapping $\widetilde{f}$ is constant (I, p. 82, prop. 4); if the space B is locally connected, the mapping $\widetilde{f}$ is locally constant. When the set F is finite, the space $\mathscr{F}(F; F')$ is discrete and the mapping $\widetilde{f}$ is locally constant.

#### Remark {#ta-i-s4-n6-rem-1 .statement tag=01PO}

Let B be a topological space, let $(E, p)$ and $(E', p')$ be B-spaces and let $f: E'\rightarrow E$ be a B-morphism.

a) If E and $E'$ are coverings of B, the mapping $f$ is etale (I, p. 29, prop. 6) and separated (I, p. 25, prop. 2). But it is not true, in general, that $(E', f)$ is a covering of E if the space B is not locally connected (I, p. 145, exerc. 4).

b) If $(E', p')$ is a covering of B, $f$ is surjective and makes $E'$ a covering of E, then the mapping $p$ is etale (I, p. 29, prop. 6). But it is not true, in general, that it is separated if the space B is not locally connected (I, p. 145, exerc. 4). In particular, E is not necessarily a covering of B.

#### Corollary {#ta-i-s4-n6-cor-1 .statement tag=01PP}

Let B be a connected and locally connected topological space. Let E and $E'$ be coverings of B. Let $b$ be a point of B. Let $f: E'\rightarrow E$ be a B-morphism and let $f_b: E'_b\rightarrow E_b$ be the mapping deduced from $f$ by restriction to the fibres. If the mapping $f_b$ is injective ( resp. surjective, resp. bijective), the same is true of the mapping $f$.

Let us denote by $p$ the projection of the B-space E. By the proposition, $(E', f)$ is a covering of E; its image $f(E')$ is open and closed in E. Let U denote the complement of $f(E')$ in E, so that the B-space $(U, p|U)$ is a covering of B (I, p. 80, corollary 1). If the mapping $f_b$ is surjective, the fibre at $b$ of this covering is empty. Since B is a connected space, U is then empty, hence $f$ is surjective.

The set V of points of E at which the fibre of $f$ has exactly one element is open and closed. The B-spaces $(V, p|V)$ and $(f(E'), p|f(E'))$ are coverings of B (loc. cit.) and the canonical mapping $i: V\rightarrow$ $f(E')$ is a B-morphism. If the mapping $f_b$ is injective, the mapping $i_b$ is surjective, hence $i$ is surjective by what precedes, and one has $V =f(E')$. Consequently, the mapping $f$ is injective.

### 7. Coverings of a Paracompact Space

#### Proposition 8 {#ta-i-s4-prop-8 .statement tag=01PQ}

A covering of a paracompact space ( I, p. 69) is a paracompact space.

Let us first prove a lemma.

#### Lemma {#ta-i-s4-n7-lem-1 .statement tag=01PR}

Let E be a separated topological space. Suppose that E has a locally finite open covering $(V_i)_{i\in I}$ such that, for every $i\in I,\overline{V_i}$ is a paracompact space. Then the space E is paracompact.

Let $(W_j)_{j\in J}$ be an open covering of E; we shall prove that there exists an open locally finite covering $(A_k)_{k\in K}$ of E which is finer than the covering $(W_j)_{j\in J}$. For each $i\in I$, let $(A'_{\ell})_{\ell\in K_i}$ be a locally finite covering of $\overline{V_i}$ by open sets of $\overline{V_i}$, finer than the covering $(W_j\cap \overline{V_i})_{j\in J}$. Let K be the sum of the family $(K_i)_{i\in I}$ (E, II, p. 30, Def. 8). For each element $k= (\ell , i)$ of K, put $A_k= A'_{\ell}\cap V_i$. Then $A_k$ is open in E and one has $\bigcup_{k\in K}A_k=\bigcup_{i\in I}V_i= E$; moreover, for each $k\in K$, there exists an index $j\in J$ such that $A_k\subset W_j$. Thus, the family $(A_k)_{k\in K}$ is an open covering of E finer than $(W_j)_{j\in J}$. It remains to prove that the family $(A_k)_{k\in K}$ is locally finite. Let $x\in E$; there exists an open neighbourhood U of $x$ which meets $V_i$ only for $i$ belonging to a finite subset $I'$ of I. For each $i\in I',x$ has an open neighbourhood $U_i\subset U$ which meets only a finite number of the open sets $A_k$, for $k\in K_i\times \{i\}:$ this is obvious if $x$ does not belong to $\overline{V_i}$, and if $x$ belongs to $\overline{V_i}$, this follows from the property of local finiteness of the covering $(A'_{\ell})_{\ell\in K_i}$ of $\overline{V_i}$. It follows that $V'=\bigcap_{i\in I'}U_i$ is an open neighbourhood of $x$ which meets only a finite number of the $A_k,k\in K$, and the covering $(A_k)_{k\in K}$ is locally finite.

Let us prove the proposition. Let E be a covering of B, let $p$ denote its projection, and suppose that the space B is paracompact. Let $(A_i)_{i\in I}$ be an open locally finite covering of B such that, for each $i\in I$, the covering E is trivializable over $A_i$. For each $i\in I$, let $F_i$ be a discrete topological space and let $g_i:\overset{-1}{p}(A_i)\rightarrow A_i\times F_i$ be a trivialization of E over $A_i$. Let $(B_i)_{i\in I}$ be an open covering of B such that, for each $i\in I$, one has $\overline{B_i}\subset A_i$ (TG, IX, p. 49, Prop. 4 and p. 48, Cor. 1). For each $i\in I$, put $V_i=\overset{-1}{p}(B_i)$; one has $\overline{V_i}\subset \overset{-1}{p}(B_i)\subset \overset{-1}{p}(A_i)$ and $V_i=\overset{-1}{g_{i}}(B_i\times F_i)$, whence $\overline{V_i}\subset \overset{-1}{g_{i}}(B_i\times F_i)$. Since B is paracompact, $\overline{B_i}$ is paracompact (TG, I, p. 69, Prop. 16) and $\overline{B_i}\times F_i$ is paracompact (TG, I, p. 70, Prop. 18). It follows that $\overset{-1}{g_{i}}(B_i\times F_i)$ is paracompact, hence so is $\overline{V_i}$ (TG, I, p. 69, Prop. 16). The family $(V_i)_{i\in I}$ is, by construction, an open locally finite covering of E. Finally, the space E is separated (I, p. 26, Remark 3). It therefore satisfies the hypotheses of the lemma, whence the proposition.

#### Remark {#ta-i-s4-n7-rem-1 .statement tag=01PS}

One can prove that a covering of a metrisable space is metrisable (I, p. 145, Exer. 1) and that a connected covering of a locally compact countable at infinity space is itself locally compact countable at infinity (I, p. 145, Exer. 2).

### 8. Locally Constant Sheaves

Let B be a topological space and F a set; endow F with the discrete topology. The sheaf on B of locally constant mappings with values in F is called the constant sheaf on B with stalk-type F (I, p. 45, Example 2). This sheaf is sometimes denoted by F, when no confusion as to the space B is to be feared. It is identified with the sheaf on B of the continuous sections of the étalé B-space $(B\times F$, pr$_1)$: the formula $i([U, s, a]) = (a, s(a))$ indeed defines a canonical isomorphism $i$ of the étalé space associated with F onto $(B\times F$, pr$_1)$. For every $a\in B$, the mapping $[U, s, a]\mapsto s(a)$ is a canonical bijection of the stalk $F_a$ of F at $a$ onto the set F.

Let $\mathscr{P}= (\mathscr{P}(U), r_{UV})$ be the presheaf on B such that $\mathscr{P}(U) = F$ for every open set U of B and $r_{UV}=$ Id$_F$ for every pair $(U,V)$ of open sets of B such that $U\subset V$. Then the sheaf $\widetilde{\mathscr{P}}$ associated with $\mathscr{P}$ is canonically isomorphic to the constant sheaf F (I, p. 52, Example 1).

#### Definition 3 {#ta-i-s4-def-3 .statement tag=01PT}

A sheaf $\mathscr{F}$ on a topological space B is said to be locally constant if every point of B possesses an open neighbourhood U such that the induced sheaf $\mathscr{F}|U$ is isomorphic to a constant sheaf on U.

#### Proposition 9 {#ta-i-s4-prop-9 .statement tag=01PU}

In order that a sheaf be locally constant, it is necessary and sufficient that the associated étalé space be a covering.

Let B be a topological space and let $\mathscr{F}$ be a sheaf on B. The sheaf $\mathscr{F}$ is constant if and only if the étalé space $E_{\mathscr{F}}$ is B-isomorphic to a trivial covering $(B\times F$, pr$_1)$, where F is a discrete topological space. If U is an open set of B, the étalé space associated with the induced sheaf $\mathscr{F}|U$ is identified with the induced étalé U-space obtained from $E_{\mathscr{F}}$ over U (cf. I, p. 51). The proposition follows.

#### Corollary {#ta-i-s4-n8-cor-1 .statement tag=01PV}

In order that an étalé B-space be a covering, it is necessary and sufficient that the sheaf of its sections be locally constant.

This follows from the proposition and from Example 2 of I, p. 52.

### 9. Products of Locally Constant Sheaves

Let B be a topological space and let $(\mathscr{F}_i)_{i\in I}$ be a family of sheaves on B. Let $\mathscr{F}$ denote the product sheaf $\prod_{i\in I}\mathscr{F}_i$ and, for $i\in I$, let pr$_i:\mathscr{F}\rightarrow \mathscr{F}_i$ be the projection morphism of index $i($I, p. 46, Example 7). Let $(E, p)$ and $(E_i, p_i)$ be the étalé B-spaces associated with the sheaves $\mathscr{F}$ and $\mathscr{F}_i$ respectively, and $\varphi_i: E\rightarrow E_i$ the B-morphism associated with pr$_i($I, p. 50). Finally, let $(E', p')$ denote the B-product $\prod_BE_i$. By the universal property of the product B-space (I, p. 5), there exists a unique B-morphism $\Phi : E\rightarrow E'$ such that, for every $i\in I$, pr$_i\circ \Phi  =\varphi_i$.

#### Proposition 10 {#ta-i-s4-prop-10 .statement tag=01PW}

If the set I is finite, the B-morphism Φ is an isomorphism.

By the corollary of I, p. 32, the B-space $E'$ is étalé, and it is enough to prove that the B-morphism Φ is bijective ( I, p. 30, Cor. 2). For every point $b$ of B, the restriction $\Phi_b: E_b\rightarrow E'_b$ of Φ to the fibres at $b$ is identified with the canonical mapping from lim$\longrightarrow \prod^{i\in I}\mathscr{F}_i(U)$ into $\prod_{i\in I}$ lim$\longrightarrow \mathscr{F}_i(U)$, where U runs through the set of open sets of B which contain $b($cf. I, p. 50). By Prop. 10 of E, III, p. 67, this mapping is a bijection.

Now consider the case of locally constant sheaves on a topological space B. Let $(F_i)_{i\in I}$ be a family of sets and put $F =\prod_{i\in I}F_i$. A canonical morphism $\psi = (\psi_U)$ of the constant sheaf F into the product $\prod_{i\in I}F_i$ of the constant sheaves $F_i$ is defined by putting, for every open set U of B and every locally constant function $f: U\rightarrow F,\psi_U(f) =$ (pr$_i\circ f$)$_{i\in I}$.

#### Proposition 11 {#ta-i-s4-prop-11 .statement tag=01PX}

If the set I is finite, or if the space B is locally connected, the canonical morphism $\psi : F\rightarrow \prod F_i$ is an isomorphism.

Let U be an open set of B. It is clear that the mapping $\psi_U$ is injective. Let us show that it is surjective. It is a matter of proving that for every family $(f_i)_{i\in I}$ where $f_i$ is a locally constant mapping of U into $F_i$, and every point $a$ of U, there exists a neighbourhood V of $a$ in U such that for every $i\in I$, the mapping $f_i|V$ is constant. When the set I is finite, the existence of such a neighbourhood is clear. When the space B is locally connected, it is enough to take for V a connected neighbourhood of $a$ in U. This proves the proposition.

#### Corollary 1 {#ta-i-s4-prop-11-cor-1 .statement tag=01PY}

A finite product of locally constant sheaves is locally constant.

Let $(\mathscr{F}_i)_{i\in I}$ be a finite family of locally constant sheaves on B. Every point $a$ of B possesses an open neighbourhood U in B such that, for every $i\in I$, the sheaf $\mathscr{F}_i|U$ is isomorphic to a constant sheaf. The same is then true of the sheaf $((\prod\mathscr{F}_i)|U$, which is equal to $\prod ((\mathscr{F}_i|U)$.

#### Corollary 2 {#ta-i-s4-prop-11-cor-2 .statement tag=01PZ}

Let $(\mathscr{F}_i)_{i\in I}$ be a family of sheaves on B. Suppose that the space B is locally connected and that every point of B possesses an open neighbourhood U such that, for every $i\in I$, the sheaf $\mathscr{F}_i|U$ is isomorphic to a constant sheaf. Then the product sheaf $\prod\mathscr{F}_i$ is locally constant.

#### Remark 1 {#ta-i-s4-n9-rem-1 .statement tag=01Q0}

Let $(E_i, p_i)_{i\in I}$ be a family of coverings of the topological space B. Suppose that the space B is locally connected and that there exists an open covering $(U_j)_{j\in J}$ of B such that, for every $j\in J$ and every $i\in I$, the covering $E_i$ is trivializable over $U_j$. For $i\in I$, let $\mathscr{F}_i$ be the locally constant sheaf of sections of $E_i$ and let $\mathscr{F}$ be the product sheaf $\prod_i\mathscr{F}_i$. By the preceding corollary, $\mathscr{F}$ is a locally constant sheaf and the étalé B-space E associated with it is therefore a covering (I, p. 86, prop. 8). For $i\in I$, let pr$_i: E\rightarrow E_i$ be the B-morphism induced by the projection morphism of index $i,\mathscr{F}\rightarrow \mathscr{F}_i$.

Now consider a covering $(Y, q)$ of B and, for every $i\in$ I, let $f_i: Y\rightarrow E_i$ be a B-morphism. If $\mathscr{G}$ denotes the locally constant sheaf of sections of $q$, the B-morphisms $f_i$ induce sheaf morphisms $\widetilde{f}_i:\mathscr{G}\rightarrow \mathscr{F}_i$. Let $\widetilde{f}:\mathscr{G}\rightarrow \mathscr{F}$ be the unique sheaf morphism such that $\widetilde{f}_i=$ pr$_i\circ \widetilde{f}$ for every $i\in I$. There then exists a unique B-morphism $f: Y\rightarrow E$ such that $f_i$ = pr$_i\circ f$ for every $i:$ this is the B-morphism which induces $\widetilde{f}$.

One sometimes says that E is the product covering of the family $(E_i)_{i\in I}$.

#### Remark 2 {#ta-i-s4-n9-rem-2 .statement tag=01Q1}

With the preceding notations, the canonical B-morphism $\Phi : E\rightarrow \prod_BE_i$ is bijective. The question is in fact of a local nature on B, and one may suppose that, for every $i\in I$, the B-space $E_i$ is isomorphic to the B-space $(B\times F_i$, pr$_1)$, where $F_i$ is a discrete topological space, so that the sheaf $\mathscr{F}_i$ is isomorphic to the sheaf $F_i$. By Prop. 11, the sheaf $\mathscr{F}$ is identified with the sheaf F, where F is the set $\prod F_i$, endowed with the discrete topology, and the mapping Φ is identified with the canonical mapping $B\times F\rightarrow B\times (\prod_iF_i)$, which is bijective.

### 10. Morphisms of locally constant sheaves on a locally connected space

Let B be a topological space, and let $(E, p)$ and $(E', p')$ be B-spaces. Let us denote by $\mathscr{M}$ = $\mathscr{M}$or$_B(E; E')$ the sheaf on B of B-morphisms of $(E, p)$ into $(E', p')$ (I, p. 45, Example 4). If U is an open set of B and $b$ a point of U, we shall denote by $\theta_{b,U}:\mathscr{M}(U)\rightarrow \mathscr{C}(E_b; E'_b)$ the canonical mapping obtained by passing to the fibres at $b$. One denotes by $\theta_b:\mathscr{M}_b\rightarrow$ $\mathscr{C}(E_b; E'_b)$ the unique mapping such that $\theta_{b,U}$ is the composite of $\theta_b$ and the canonical mapping $\mathscr{M}(U)\rightarrow \mathscr{M}_b$ for every open set U of B containing $b$ (E, III, p. 62).

Let also $\mathscr{I}=\mathscr{I}$som$_B(E; E')$ be the sheaf on B of B-isomorphisms of $(E, p)$ into $(E', p')$. Let us denote by $i:\mathscr{I}\rightarrow \mathscr{M}$ the canonical morphism. For every $b\in B$, the mapping $\theta_b\circ i_b$ induces a mapping $\theta '_b$ of $\mathscr{I}_b$ into the set of continuous bijections of $E_b$ onto $E'_b$.

#### Proposition 12 {#ta-i-s4-prop-12 .statement tag=01Q2}

Suppose that the space B is locally connected and that the B-spaces E and $E'$ are coverings. Then the sheaf $\mathscr{M}$or$_B(E; E')$ is locally constant and, for every $b\in B$, the mapping $\theta_b$ is a bijection of its stalk at $b$ onto the set of mappings of $E_b$ into $E'_b$.

Analogously, the sheaf $\mathscr{I}$som$_B(E; E')$ is locally constant and, for every point $b$ of B, the mapping $\theta '_b$ is a bijection of its stalk at $b$ onto the set of bijections of $E_b$ onto $E'_b$.

We shall denote by $\mathscr{M}=\mathscr{M}$or$_B(E; E')$ and $\mathscr{I}=\mathscr{I}$som$_B(E; E')$. The assertions to be proved are of a local nature on B; we may therefore suppose that $E = B\times F$ and $E'= B\times F'$ are trivial coverings, where F and $F'$ are discrete topological spaces.

Let us first prove that, for every connected open set U of B and every point $b$ of U, the mapping $\theta_{b,U}$ is a bijection. Let $f: U\times F\rightarrow$ $U\times F'$ be a morphism of U-spaces; then $\theta_{b,U}(f)$ is the mapping $y\mapsto$ pr$_2(f(b, y))$ of F into $F'$. For every $y\in F$, the mapping $x\mapsto$ pr$_2(f(x, y))$ is a continuous mapping of the connected space U into the discrete space $F'$, and is therefore constant, equal to pr$_2(f(b, y))$. Thus $f(x, y) = (x, \theta_{b,U}(f)(y))$. It follows that $\theta_{b,U}$ is a bijection; its inverse bijection associates with every mapping $\varphi : F\rightarrow F'$ the U-morphism of $U\times F$ into $U\times F'$ given by $(x, y)\mapsto (x, \varphi (y))$.

By hypothesis, every point $b\in B$ admits a basis of connected open neighbourhoods; the mapping $\theta_b$ is therefore a bijection. The mappings $\theta^{-1}_{b,U}$, for U a nonempty connected open set of B and $b$ any point of $b$, define a morphism of presheaves (relative to the basis of connected open sets of B) of the constant sheaf of stalk-type ${F'}^F$ into the sheaf $\mathscr{M}$. From what precedes, this morphism induces a bijection on the stalks; it is therefore an isomorphism.

The assertions relative to the sheaf $\mathscr{I}$ are proved analogously.

#### Corollary 1 {#ta-i-s4-prop-12-cor-1 .statement tag=01Q3}

Let B be a topological space and A a subspace of B. Suppose that the spaces A and B are locally connected. Let E and $E'$ be coverings of B. Then the canonical morphisms $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ and $\psi ':\mathscr{I}$som$_B(E; E')_A\rightarrow$ $\mathscr{I}$som$_A(E_A; E'_A)$ (I, p. 45, example 4) are isomorphisms.

For every point $a\in A$, it follows from the preceding proposition and from example 2 of I, p. 63, applied to the spaces $\{a\}$, A, B and to the canonical injections, that the canonical morphism $\psi$ induces on passing to the stalks the identity of $E^{E'_a}_a$. It is therefore an isomorphism. The fact that $\psi '$ is an isomorphism is proved analogously.

#### Corollary 2 {#ta-i-s4-prop-12-cor-2 .statement tag=01Q4}

Let B be a topological space and A a subspace of B. Suppose that the spaces A and B are locally connected and that the pair $(B,A)$ has property (PCV) of I, p. 37. Let E and $E'$ be coverings of B, and let us denote by $p$ and $p'$ their projections. Let

$g:\overset{-1}{p}(A)\rightarrow (^-{p'}^1)(A)$ be an A-morphism ( resp. an A-isomorphism). Then there exists a neighbourhood U of A in B and a U-morphism ( resp. a

U-isomorphism) $f:\overset{-1}{p}(U)\rightarrow (\overset{-1}{p}')(U)$ such that $f_A=g$.

Let us retain the notation of corollary 1. By that same corollary, an A-morphism $g: E_A\rightarrow E'_A$ is identified with a section $s_0$ above A of the étale space $E_{\mathscr{M}}$ associated with $\mathscr{M}$. By the hypothesis made on the pair $(B,A)$ and lemma 3 of I, p. 39, there exists an open neighbourhood U of A in B and a continuous section $s$ of $E_{\mathscr{M}}$ above U extending $s_0$. This section $s$ is identified with a U-morphism $f: E_U\rightarrow E'_U$ extending $f$.

The case where $g$ is an A-isomorphism is treated analogously by considering, in place of the sheaf $\mathscr{M}$, the sheaf $\mathscr{I}$.

## EXERCISES {#ta-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
