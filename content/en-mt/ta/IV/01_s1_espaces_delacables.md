---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 1
section_title: Espaces délaçables
lang: en
source: ta-i-iv-fr
book_pages: TA IV.340-TA IV.351, TA IV.455-TA IV.457
pdf_pages: 0356-0367, 0471-0473
extraction: native
subsections:
    - "no": 1
      title: Espaces simplement connexes par arcs
      page: 340
      pdf_page: 356
    - "no": 2
      title: Espaces délaçables
      page: 340
      pdf_page: 356
    - "no": 3
      title: Revêtement universel d’un espace délaçable
      page: 342
      pdf_page: 358
    - "no": 4
      title: Exemples
      page: 346
      pdf_page: 362
statements: 20
exercises: 6
content_sha256: 6fc423d8711798f8f570057261de9eb8f2b9492c8563a065ae96d37c64302106
translated_from: content/fr/ta/IV/01_s1_espaces_delacables.md
source_lang: fr
translation_method: machine
source_content_sha256: 90407d2b56ffe54b38305250d19bf65950e3750b5e543cf8c3a179d928c67e98
translation_model: gpt-5.4
translation_run: translate-en-mt-09d366ee
glossary_version: 34
glossary_terms_sha256: 65dd4ee21de577aca3fcaba1db839b1f73b06fc96d53787ac6a0f62c73ff6a50
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. SIMPLY CONNECTED SPACES

### 1. Arcwise simply connected spaces

#### Definition 1 {#ta-iv-s1-def-1 .statement tag=0208}

A topological space X is said to be arcwise simply connected if it is arcwise connected and if every loop in X is strictly homotopic to a constant loop.

The empty space is arcwise simply connected. In order that an arcwise connected space X be arcwise simply connected, it is necessary and sufficient that the group $\pi_1(X, x)$ be reduced to the identity element for every point $x$ of X (III, p. 292, prop. 2). It is sufficient that this be so for one point $x$ of X (loc. cit.).

Every topological space homotopic to an arcwise simply connected space is arcwise simply connected. In fact, it is arcwise connected (III, p. 260) and, at every point, its Poincaré group is reduced to the identity element (III, p. 296, cor. 2 of prop. 6). In particular, a topological space homotopic to a point is arcwise simply connected.

A topological space which is arcwise simply connected and locally arcwise connected is simply connected (III, p. 309, cor. 2 of prop. 1).

### 2. Unloopable spaces

#### Definition 2 {#ta-iv-s1-def-2 .statement tag=0209}

A topological space B is said to be unloopable if it is locally arcwise connected and if every point $b$ of B possesses a neighbourhood V such that the homomorphism of $\pi_1(V, b)$ into $\pi_1(B, b)$ deduced from the canonical injection has as image the identity element.

A locally arcwise connected topological space is unloopable if and only if each of its connected components is so.

Let B be a locally arcwise connected topological space. Suppose that every point of B possesses a neighbourhood V which is unloopable. Then B is unloopable.

Every topological space which is locally arcwise connected and arcwise simply connected is unloopable. This is in particular the case for a locally arcwise connected space homotopic to a point.

#### Remark 1 {#ta-iv-s1-n2-rem-1 .statement tag=020A}

There exist topological spaces B, connected and locally arcwise connected, such that certain points $a$ of B, but not all, possess a neighbourhood V such that the homomorphism of $\pi_1(V, a)$ into $\pi_1(B, a)$ is trivial (III, p. 336, exerc. 6).

#### Remark 2 {#ta-iv-s1-n2-rem-2 .statement tag=020B}

Let B be an unloopable space; every operation of the groupoid $\varpi (B)$ on a B-space is without local monodromy (cf. III, p. 313, remark). In particular, in order that a mapping $p: E\rightarrow B$ make E into a covering of B, it is necessary and sufficient that it be étale, separated and that it satisfy the path lifting property (III, p. 315, corollary 3).

#### Proposition 1 {#ta-iv-s1-prop-1 .statement tag=020C}

The product space of a finite family of unloopable spaces is unloopable.

It is sufficient to prove that, if A and B are two unloopable spaces, the same is true of their product $A\times B$. Under these conditions, the space $A\times B$ is in fact locally arcwise connected (III, p. 261, prop. 9). Let $(a, b)$ be a point of $A\times B$. By hypothesis there exists a neighbourhood U of $a$ (resp. a neighbourhood V of $b$) such that the image of the homomorphism $i_*:\pi_1(U, a)\rightarrow \pi_1(A, a)$ deduced from the canonical injection $i: U\rightarrow A$ (resp. of the homomorphism $j_*:\pi_1(V, b)\rightarrow \pi_1(B, b)$ deduced from the canonical injection $j: V\rightarrow B$) is reduced to the identity element. Then $U\times V$ is a neighbourhood of $(a, b)$ in $A\times B$. The homomorphism $\pi_1(U\times V,(a, b))\rightarrow \pi_1(A\times B,(a, b))$ identifies with the homomorphism $(i_*, j_*)$ (III, p. 297, corollary of prop. 4). Its image is therefore reduced to the identity element. This proves that $A\times B$ is unloopable.

#### Proposition 2 {#ta-iv-s1-prop-2 .statement tag=020D}

a) Every covering of an unloopable space is unloopable.

b) Conversely, let $p: E\rightarrow B$ be an étale and surjective mapping and suppose that E is an unloopable space. Then B is unloopable.

a) Let B be an unloopable topological space and let $(E, p)$ be a covering of B. Then the space E is locally arcwise connected. Let $x$ be a point of E, put $b=p(x)$, and let V be a neighbourhood of $b$ in B such that the canonical homomorphism $\pi_1(V, b)\rightarrow \pi_1(B, b)$ is trivial. Let $i: V\rightarrow B$ and $j:\overset{-1}{p}(V)\rightarrow E$ denote the canonical injections. By hypothesis, the image of the homomorphism $\pi_1(i, b)$ is reduced to the identity element. Since $p\circ i=j\circ p$ and $\pi_1(p, x)$ is injective, the image of the homomorphism $\pi_1(j, x)$ is reduced to the identity element. This proves that E is unloopable.

b) The space B is locally arcwise connected. Let $b$ be a point of B and let $x$ be a point of $E_b$. Since $p$ is étale, there exists a neighbourhood U of $x$ in E such that $p$ induces a homeomorphism of U onto $p(U)$. Let V be a neighbourhood of $x$ in E contained in U such that the homomorphism $\pi_1(j, x)$ is trivial, where $j: V\rightarrow E$ denotes the canonical injection. Let $q: V\rightarrow p(V)$ be the mapping deduced from $p$ by passing to subspaces; it is a homeomorphism. Let also $i$ denote the canonical injection of $p(V)$ into B. We have $p\circ j=i\circ q$, hence $\pi_1(i, b)\circ \pi_1(q, x) =\pi_1(p, x)\circ \pi_1(j, x)$ is the trivial homomorphism. Since the homomorphism $\pi_1(q, x)$ is an isomorphism, the homomorphism $\pi_1(i, b)$ is trivial. It follows that the space B is unloopable.

#### Proposition 3 {#ta-iv-s1-prop-3 .statement tag=020E}

Let B be an unloopable topological space. Let $(Y, q)$ be a covering of B and let $(Z, p)$ be a covering of Y. The topological space Z, endowed with the mapping $q\circ p$, is then a covering of B.

In fact, the mapping $q\circ p$ is étale (I, p. 29, prop. 6) and separated (I, p. 25, prop. 2). By Remark 2 above, it is therefore enough to prove that it satisfies the path-lifting property. Let $z$ be a point of Z and let $c:\mathbf{I}\rightarrow B$ be a path in B with origin $q(p(z))$. There exists a path $c'$ with origin $p(z)$ in Y which lifts $c$, because Y is a covering of B (III, p. 302, Cor. 2). Since Z is a covering of Y, there exists a path $c''$ with origin $z$ in Z which lifts $c'$; the path $c''$ lifts $c$. This proves the proposition.

### 3. Universal covering of an unlaceable space

Let B be a topological space and let $b$ be a point of B. Recall that $\Lambda_b(B)$ denotes the subspace of $\mathscr{C}_c(\mathbf{I}; B)$ formed by the paths with origin $b$, endowed with the quotient topology of the compact-convergence topology. We denote by $e_B: \Lambda_b(B)\rightarrow$ B the mapping which associates to a path its endpoint; it is continuous. Let us denote by $\lambda_b(B)$ the quotient space of $\Lambda_b(B)$ for the relation of strict homotopy and endow it with the quotient topology. Since two strictly homotopic paths have the same endpoint, the mapping $e_B$ defines, by passing to the quotient, a continuous mapping $\varepsilon_B:\lambda_b(B)\rightarrow B$, called the endpoint mapping.

#### Theorem 1 {#ta-iv-s1-thm-1 .statement tag=020F}

Let B be a connected topological space, locally connected by arcs, and let $b$ be a point of B. The following properties are equivalent:

(i) The space B is unlaceable.

(ii) There exists a nonempty covering of B which is simply connected by arcs.

(iii) The space $\lambda_b(B)$, endowed with the endpoint mapping $\varepsilon_B:\lambda_b(B)\rightarrow B$, is a covering of B.

(iv) The group $\pi_1(B, b)$ is discrete for the admissible topology.

(v) The group $\pi_1(B, b)$ is discrete for the quotient topology of the compact-convergence topology.

Moreover, when these conditions are satisfied, the space $\lambda_b(B)$ is simply connected by arcs, simply connected, Galois with group $\pi_1(B, b)^{\circ}$, and the pointed covering $(\lambda_b(B), \varepsilon_b)$ is a universal covering of the pointed space $(B, b)$.

It follows from the definition of an unlaceable space that the subgroup of $\pi_1(B, b)$ reduced to the identity element is admissible if and only if B is unlaceable. This proves the equivalence (i)$\Leftrightarrow ($iv). Moreover, the equivalence of properties (iv) and (v) follows from Remarks 4 and 5 of III, p. 320.

(iv)$\Rightarrow ($ii). By III, p. 316, Prop. 5, there exists a covering $(E, p)$ of B and a point $x\in E_b$ such that $p_*(\pi_1(E, x)) =\{e\}$; in particular, $\pi_1(E, x)$ is reduced to the identity element. The connected component by arcs of $x$ in E is then a nonempty covering of B (I, p. 80, Cor. 1 to Prop. 6), simply connected by arcs.

(ii)$\Rightarrow ($iii). Let E be a nonempty covering of B which is simply connected by arcs. Let $x$ be a point of $E_b$ (there exists one because B is connected, I, p. 74, Prop. 4). The projection $q: E\rightarrow$ B induces a homeomorphism $\Lambda_x(E)\rightarrow \Lambda_b(B)$ (III, p. 302, Cor. 2 to Prop. 3), whence, by passing to connected components by arcs, a homeomorphism $q_*:\lambda_x(E)\simeq \lambda_b(B)$. The endpoint mapping $\Lambda_x(E)\rightarrow E$ is continuous and open, because E is locally connected by arcs (III, p. 264, Corollary). The mapping $\varepsilon_E:\lambda_x(E)\rightarrow E$ which it defines by passing to connected components by arcs is therefore continuous and open. The mapping $\varepsilon_E\circ (q_*)^{-1}:\lambda_b(B)\rightarrow E$ is bijective, continuous and open. This proves that the topological space $\lambda_b(B)$, endowed with the compact-convergence topology and the endpoint mapping, is a covering of B.

(iii)$\Rightarrow ($v). In fact, the set $\pi_1(B, b)$, endowed with the quotient topology of the compact-convergence topology, is identified with the fibre of the B-space $\lambda_b(B)$ over the class of the constant loop at $b$. If $\lambda_b(B)$ is a covering of B, then $\pi_1(B, b)$ is discrete for the compact-convergence topology.

Suppose that these assertions are verified. From the foregoing, the space $\lambda_b(B)$ is then a covering of B which is simply connected by arcs, hence simply connected. The pointed space $(\lambda_b(B), \varepsilon_b)$ is consequently a universal covering of $(B, b)$ (I, p. 126, corollary to Prop. 3) and the covering $\lambda_b(B)$ is a Galois covering of B (I, p. 120, Prop. 1). The canonical homomorphism $h_{(\lambda_b(B),\varepsilon_b)}:\pi_1(B, b)\rightarrow$ Aut$_B(\lambda_b(B))$ is then an isomorphism (III, p. 306, Prop. 5).

#### Remark 1 {#ta-iv-s1-n3-rem-1 .statement tag=020G}

Let B be a connected unwindable space and let $b$ be a point of B. It follows from Theorem 1, (iv), that every operation of the group $\pi_1(B, b)$ is admissible. Consequently, every $\pi_1(B, b)$-set is isomorphic to a $\pi_1(B, b)$-set $E_b$, where E is a covering of B (III, p. 318, prop. 7). Recall also (III, p. 310, prop. 2) that if E and $E'$ are coverings of B, the mapping $f\mapsto f_b$ induces a bijection of the set of morphisms of B-spaces from E into $E'$ onto the set of morphisms of $\pi_1(B, b)$-sets from $E_b$ into $E'_b$.

*In the language of categories, one says that the functor which associates with a covering E of B the fibre $E_b$ is an equivalence of categories from the category of coverings of B into the category of $\pi_1(B, b)$-sets.*

#### Corollary 1 {#ta-iv-s1-thm-1-cor-1 .statement tag=020H}

Let B be an unwindable topological space and let $b$ be a point of B. Let E be a connected covering of B and let $x$ be a point of the fibre $E_b$. The following properties are equivalent:

(i) The group $\pi_1(E, x)$ is trivial.

(ii) The space E is simply connected.

(iii) The pointed space $(E, x)$ is a universal covering of $(B, b)$.

The implication (i)$\Rightarrow$(ii) has already been proved under the sole assumption that the space B is connected and locally arcwise connected (III, p. 309, cor. 2 of prop. 1), and the implication (ii)$\Rightarrow$(iii) without any assumption (I, p. 126, corollary).

Let us prove (iii)$\Rightarrow$(i). By Theorem 1 of IV, p. 342, there exists a covering $E'$ of B and a point $x'$ of the fibre $E'_b$ such that the group $\pi_1(E', x')$ is reduced to the identity element. Under assumption (iii), there exists a pointed B-morphism $f: (E, x)\rightarrow (E', x')$. Let $p: E\rightarrow$ B and $p': E'\rightarrow B$ denote the projections of the coverings E and $E'$; we have $p=p'\circ f$, hence $\pi_1(p, x) =\pi_1(p', x')\circ \pi_1(f, x)$. Since the group $\pi_1(E', x')$ is trivial, the injective homomorphism $\pi_1(p, x)$ has the identity element for image. This proves that the group $\pi_1(E, x)$ is reduced to the identity element.

#### Corollary 2 {#ta-iv-s1-thm-1-cor-2 .statement tag=020I}

Let B be an unwindable topological space and let $b$ be a point of B. Let $(E, x)$ be a universal covering of the pointed space $(B, b)$. For every covering $E'$ of B and every point $x'$ of $E'_b$, the unique B-morphism $f: E\rightarrow E'$ such that $f(x) =x'$ makes E a covering of $E'$. The pointed space $(E, x)$ is then a universal covering of $(E', x')$.

By prop. 7 of I, p. 81, the space E, endowed with the mapping $f$, is a covering of $E'$. The last assertion then follows from Corollary 1.

Let B be an unwindable topological space and let $a,b$ be two points of B. The quotient topological space $\varpi_{a,b}(B)$ is homeomorphic to the space $\pi_1(B, a)$, endowed with the quotient topology of the compact-open topology (III, p. 293, remark 3), and therefore is discrete by Theorem 1 of IV, p. 342. Consequently, the strict homotopy class of every path in B joining $a$ to $b$ is an open subset of $\Lambda_{a,b}(B)$. More generally:

#### Proposition 4 {#ta-iv-s1-prop-4 .statement tag=020J}

Let B be an unwindable topological space. The relation of strict homotopy is an open equivalence relation in the topological space $\mathscr{C}_c(\mathbf{I}; B)$.

Suppose first that the space B is simply arcwise connected. Let $\varphi : \Lambda (B)\rightarrow B\times B$ denote the mapping which associates with a path $c$ in B the pair $(c(0), c(1))$ formed by its origin and its end. In order that two paths in B be strictly homotopic, it is necessary and sufficient that they have the same origin and the same end (III, p. 292, prop. 2). Since the space B is connected and locally arcwise connected, the mapping $\varphi$ is surjective, continuous and open (III, p. 262, prop. 10). The relation of strict homotopy is therefore open (TG, I, p. 32, prop. 3).

In the general case, let E be a simply connected by paths covering of B, nonempty if B $=\not\emptyset$. This covering is surjective because B is connected (I, p. 74, prop. 4). Let us denote by $p$ the projection of the B-space E and let $\widetilde{p}: \Lambda (E)\rightarrow \Lambda (B)$ be the mapping which associates to a path $c$ in E the path $p\circ c$. Endowed with the mapping $\widetilde{p}$, Λ(E) is a covering of Λ(B) (III, p. 302, cor. 1 of prop. 3). In order that two paths in B should be strictly homotopic, it is necessary and sufficient that they should be the images under the mapping $\widetilde{p}$ of two strictly homotopic paths in E (III, p. 302, prop. 4). Let U be an open subset of the space Λ(B). The set $(\overset{-1}{\widetilde{p}})(U)$ is open in Λ(E) ; by the first part of the

proof, the set $U'$ saturated of $(\overset{-1}{\widetilde{p}})(U)$ for the relation of strict homotopy is open in Λ(E). Since Λ(E) is a covering of Λ(B), the set $\widetilde{p}(U')$ is open in Λ(B). This proves the proposition, for $\widetilde{p}(U')$ is the saturated set of U for the relation of strict homotopy.

### 4. Examples

1) Locally contractible spaces

#### Definition 3 {#ta-iv-s1-def-3 .statement tag=020K}

A topological space B is said to be locally contractible if every point $b$ of B possesses a neighbourhood V such that the pointed space $(V, b)$ is contractible (III, p. 234, example 3).

#### Proposition 5 {#ta-iv-s1-prop-5 .statement tag=020L}

A locally contractible topological space is unlaceable.

Let B be a locally contractible space. Let $b$ be a point of B and let V be a neighbourhood of $b$ such that $(V, b)$ is a contractible pointed space. The space V is homotopic to a point, hence $\pi_1(V, b) =\{\varepsilon_b\}($III, p. 296, corollary 3).

To prove the proposition, it remains to prove that the space B is locally connected by paths. Let $\sigma : V\times \mathbf{I}\rightarrow$ V be a pointed homotopy at $b$ joining the constant mapping of image $b$ to the mapping Id$_V$. For every neighbourhood W of $b$ contained in V, the set $\sigma (W\times \mathbf{I})$ is a neighbourhood of $b$ because it contains $W =\sigma (W\times  \{1\})$, and it is connected by paths because for every $(a, s)\in W\times \mathbf{I}$, the mapping $t\mapsto \sigma (a, ts)$ is a path joining $b=\sigma (a,0)$ to $\sigma (a, s)$ in $\sigma (W\times \mathbf{I})$. Let us prove that the sets of the form $\sigma (W\times \mathbf{I})$ form a fundamental system of neighbourhoods of $b$. Let $V'$ be an open neighbourhood of $b$ in B; then, $\overset{-1}{\sigma}(V')$ is an open neighbourhood of $\{b\} \times \mathbf{I}$ in $V\times \mathbf{I}$. Since the space $\mathbf{I}$ is compact, the projection pr$_1: V\times \mathbf{I}\rightarrow V$ is proper (TG, I, p. 77, cor. 5) and pr$_1(\complement \overset{-1}{\sigma}(V'))$ is a closed subset of V not containing $b$. Its complement W is thus an open neighbourhood of $b$ in V such that $W\times \mathbf{I}\subset \overset{-1}{\sigma}(V')$, whence $\sigma (W\times \mathbf{I})\subset V'$.

Every open subset of a numerical space or of a projective space, real or complex, of dimension $n$ (cf. Chapters VI and VIII) is unlaceable, as are the Euclidean spheres $\mathbf{S}_n$ (TG, VI, p. 11, prop. 4). More generally, every topological manifold (VAR R, second part, p. 7, Notations et Conventions) is unlaceable. In fact, these spaces are locally contractible.

2) Poincaré group of the circle. — The topological space $\mathbf{R}$ is homotopic to a point (III, p. 234, example 4), hence simply connected by paths (IV, p. 340). The canonical surjection $p$ of $\mathbf{R}$ onto $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ makes it a principal covering of group $\mathbf{Z}($I, p. 100, example 4). The topological space $\mathbf{T}$ is unlaceable and $(\mathbf{R},0)$ is a universal covering of $(\mathbf{T},0)$. One deduces from this a canonical isomorphism of groups $\pi_1(\mathbf{T},0)\rightarrow \mathbf{Z}:$ it maps the class of the loop $t\mapsto p(nt)$ at 0 to the element $n$ of $\mathbf{Z}$. Taking into account example 6 (I, p. 101), one deduces the following proposition.

#### Proposition 6 {#ta-iv-s1-prop-6 .statement tag=020M}

The mapping $p:x\mapsto e^{2\pi ix}$ of $\mathbf{R}$ into $\mathbf{S}_1$ makes $(\mathbf{R},0)$ a universal covering of $(\mathbf{S}_1,1)$. The group $\pi_1(\mathbf{S}_1,1)$ is isomorphic to $\mathbf{Z}$; the class of the loop $t\mapsto e^{2\pi it}$ is a generator of it. For every integer $n >0$, the mapping $z\mapsto z^n$ makes $\mathbf{S}_1$ a Galois covering of group $\mathbf{Z}/n\mathbf{Z}$ of $\mathbf{S}_1$. Every connected nonempty covering of $\mathbf{S}_1$ is isomorphic to one of these coverings.

Only the last assertion remains to be proved. The fibre $E_1$ over 1 of a connected nonempty covering E of $\mathbf{S}_1$ is endowed with a transitive operation of the group $\pi_1(§_1,1)$. Since the subgroups of $\mathbf{Z}$ are the sets $n\mathbf{Z}$, for $n\geqslant 0$, we see that $E_1$ is isomorphic to one of the homogeneous sets associated with the coverings described above. Since $\mathbf{S}_1$ is connected and locally arcwise connected, E is isomorphic to one of these coverings.

#### Corollary {#ta-iv-s1-n4-cor-1 .statement tag=020N}

The mapping $z\mapsto e^z$ of $\mathbf{C}$ into $\mathbf{C}^*$ makes $(\mathbf{C},0)$ a universal covering of $(\mathbf{C}^*,1)$. The group $\pi_1(\mathbf{C}^*,1)$ is isomorphic to $\mathbf{Z}$; the class of the loop $t\mapsto e^{2\pi it}$ is a generator of it. For every integer $n >0$, the mapping $z\mapsto z^n$ makes $\mathbf{C}^*$ a Galois covering of group $\mathbf{Z}/n\mathbf{Z}$ of $\mathbf{C}^*$. Every connected nonempty covering of $\mathbf{C}^*$ is isomorphic to one of these coverings.

The mapping $z\mapsto (|z|, z/|z|)$ is a homeomorphism of the space $\mathbf{C}^*$ onto the space $\mathbf{R}^*_+\times \mathbf{S}^1$ (TG, VI, p. 10, prop. 3); in particular, $\mathbf{C}^*$ is arcwise connected. Since the mapping $x\mapsto e^x$ of $\mathbf{R}$ into $\mathbf{R}_+^*$ is a homeomorphism, it follows from proposition 6 that the mapping $(x, y)\mapsto e^xe^{2\pi iy}$ makes $\mathbf{R}^2$ a covering of $\mathbf{C}^*$. On identifying $\mathbf{R}^2$ with $\mathbf{C}$ by means of the mapping $(x, y)\mapsto x+iy$, we conclude that the space $\mathbf{C}$, endowed with the mapping $z\mapsto e^z$, is a covering of $\mathbf{C}^*$. Since the space $\mathbf{C}$ is connected and simply arcwise connected, the pointed covering $(\mathbf{C},0)$ is a universal covering of the pointed space $(\mathbf{C}^*,1)$.

It also follows from the corollary, III, p. 297, that the Poincaré group of $\mathbf{C}^*$ at 1 is isomorphic to $\mathbf{Z}$ and that the class $\gamma$ of the loop $t\mapsto e^{2\pi it}$ is a generator of it.

Let $n$ be an integer $>0$. The mapping $x\mapsto x^n$ of $\mathbf{R}^*_+$ onto itself is a homeomorphism; it follows as above that the mapping $z\mapsto z^n$ makes $\mathbf{C}^*$ a covering of degree $n$ of $\mathbf{C}^*$. It is Galoisian with group $\mathbf{Z}/n\mathbf{Z}$. The last assertion is proved as in the proof of prop. 6.

For every integer $n\geqslant 0$, the torus $(\mathbf{S}_1)^n$ is an unwindable space (IV, p. 341, prop. 1) and its Poincaré group at every point is isomorphic to $\mathbf{Z}^n($III, p. 297, prop. 4).

We shall generalize these results in paragraph 3 devoted to coverings of topological groups.

3) Real projective spaces. --- Let $n$ be an integer $>0$. The spaces $\mathbf{S}_n$ and $\mathbf{P}_n(\mathbf{R})$ are connected, non-empty, and the canonical mapping (TG, VI, p. $13$)$\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ makes $\mathbf{S}_n$ a principal covering of $\mathbf{P}_n(\mathbf{R})$ with group $\{+1,-1\}($I, p. 99, example 1). For $n\geqslant 2$, the sphere $\mathbf{S}_n$ is simply connected (I, p. 127, example 3) and unwindable, hence simply connected by arcs (IV, p. 344, corollary 1). For $n= 1$, the mapping $z\mapsto z^2$ of $\mathbf{S}_1$ into $\mathbf{S}_1$ defines an equivalence relation in $\mathbf{S}_1$ whose classes are the pairs of opposite points of $\mathbf{S}_1$. The mapping $\varphi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ defines by passing to the quotient a continuous bijection $\psi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ such that $\psi (z^2) =\varphi (z)$. Since $\mathbf{S}_1$ is a compact space, the mapping $\psi$ is a homeomorphism (TG, I, p. 63, cor. 2).

#### Proposition 7 {#ta-iv-s1-prop-7 .statement tag=020O}

The mapping $x\mapsto \varphi (e^{2\pi ix})$ of $\mathbf{R}$ onto $\mathbf{P}_1(\mathbf{R})$ makes $(\mathbf{R},0)$ a universal covering of $(\mathbf{P}_1(\mathbf{R}), \varphi (1))$. Let $c:\mathbf{I}\rightarrow \mathbf{S}_1$ be the path $t\mapsto e^{\pi it}$; the class of $\varphi (c)$ is a generator of the group $\pi_1(\mathbf{P}_1(\mathbf{R}), \varphi (1))$, which is isomorphic to $\mathbf{Z}$.

For every integer $n\geqslant$ 2 and every point $x$ of $\mathbf{S}_n$, the canonical mapping $\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ makes $(\mathbf{S}_n, x)$ a universal covering of $(\mathbf{P}_n(\mathbf{R}), \varphi (x))$. For every path $c$ in $\mathbf{S}_n$ joining $x$ to $-x$, the class of $\varphi \circ c$ generates the group $\pi_1(\mathbf{P}_n(\mathbf{R}), \varphi (x))$, which is isomorphic to $\mathbf{Z}/2\mathbf{Z}$.

4) Quotient of a space by the proper action of a discrete group

#### Lemma 1 {#ta-iv-s1-lem-1 .statement tag=020P}

Let X be a topological space, let G be a discrete group operating properly in X, and let $p$ be the canonical projection of X onto $X/G$.

Let $x$ be a point of X, let $K_x$ be its stabilizer in G. Let $U_1$ be a neighbourhood of $x$ in X; there exists a neighbourhood U of $x$ in X, stable under $K_x$ and contained in $U_1$ such that $g\cdot U\cap U =\emptyset$ if $g\notin K_x$ and such that the canonical mapping $p$ induces a homeomorphism of $U/K_x$ onto a neighbourhood V of $p(x)$ in $X/G$.

By prop. 8 of TG, III, p. 32, there exists a neighbourhood $U_2$ of $x$ in X, stable under $K_x$, such that $g\cdot U_2\cap U_2=\emptyset$ if $g\notin K_x$ and such that the canonical mapping $p$ induces a homeomorphism of $U_2/K_x$ onto a neighbourhood of $p(x)$ in $X/G$.

Since the canonical mapping $U_2\rightarrow U_2/K_x$ is closed (TG, III, p. 28, prop. 2), there exists an open neighbourhood U of $x$ contained in $U_1\cap U_2$ which is stable under $K_x($I, p. 75, lemma). The equivalence relation in $U_2$ defined by $K_x$ is also open (TG, III, p. 10, lemma 2). It then follows from TG, I, p. 32, prop. 4, that the canonical mapping induces a homeomorphism of $U/K_x$ onto an open neighbourhood of $p(x)$ in $X/G$, whence the lemma.

#### Proposition 8 {#ta-iv-s1-prop-8 .statement tag=020Q}

Let X be a topological space and let G be a discrete group operating properly in X. Let us denote by $p$ the canonical projection of X onto $X/G$.

a) Suppose that X is connected by arcs and that the group G is generated by the stabilizers of the points of X. Then the canonical homomorphism $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ is surjective for every point $x$ of X. In particular, $X/G$ is simply connected by arcs if X is.

b) If the space X is unloopable, the space $X/G$ is unloopable.

a) The set N of the elements $g\in G$ for which there exists a path $c_g:\mathbf{I}\rightarrow X$ such that $c_g(0) =x,c_g(1) =g\cdot x$ and such that the loop $p\circ c_g$ in $X/G$ is strictly homotopic to a constant loop is a subgroup of G. If $g\in G$ and if there exists a point $y$ of X such that $g\cdot y=y$, let us choose a path $c:\mathbf{I}\rightarrow X$ joining $x$ to $y$; then the path $c'=c*$ $\overline{(g\cdot c)}$ satisfies $c'(0) =x,c'(1) =g\cdot x$ and $[p\circ c'] = [p\circ c][p\circ (g\cdot c)]^{-1}=e_{p(x)}$, whence $p\circ c'$ is strictly homotopic to a constant loop. Since G is generated by the stabilizers of the points of X, it follows that N = G.

Let $c$ be a loop in $X/G$ at $p(x)$. By Theorem 4 of III, p. 287, there exists a path $\widetilde{c}:\mathbf{I}\rightarrow X$ lifting $c$ such that $\widetilde{c}(0) =x$. Since $p(\widetilde{c}(1)) =c(1) =p(x)$, there exists $g\in G$ such that $\widetilde{c}(1) =g\cdot x$. Choose a path $c_g:\mathbf{I}\rightarrow X$ joining $x$ to $g\cdot x$ and such that $p\circ c_g$ is strictly homotopic to a constant loop. Then the path $c'=\widetilde{c}*\overline{c_g}$ is a loop at $x$ in X such that $[p\circ c'] = [c]$. This shows that the homomorphism $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ is surjective. The other assertion follows immediately.

Let us now prove assertion b). The space $X/G$ is locally arcwise connected (III, p. 261, Prop. 8).

Let $x$ be a point of X and let $K_x$ be its stabilizer in G. Let $U_1$ be an open neighbourhood of $x$, contained in U, such that the image of the canonical homomorphism $\pi_1(U_1, x)\rightarrow \pi_1(X, x)$ is reduced to the identity element. By Lemma 1 (IV, p. 349), there exists a neighbourhood U of $x$ in X, contained in $U_1$, stable under $K_x$, such that $g\cdot U\cap U =\emptyset$ if $g\notin K_x$ and such that the canonical mapping $p$ induces a homeomorphism of $U/K_x$ onto a neighbourhood V of $p(x)$ in $X/G$.

Let $c$ be a loop at $x$ in V; by Theorem 4 (III, p. 287), applied to the topological space U and the group $K_x$, there exists a path $\widetilde{c}:\mathbf{I}\rightarrow U$ such that $\widetilde{c}(0) =x$ and which lifts $c$. Necessarily $\widetilde{c}(1) =x$, so that $\widetilde{c}$ is a loop at $x$ in U. By assumption, $\widetilde{c}$ is strictly homotopic to a constant loop in X; consequently, the same is true of $c$, and the canonical homomorphism $\pi_1(V, p(x))\rightarrow \pi_1(X/G, p(x))$ is trivial. This proves that $X/G$ is unloopable if X is.

5) In the Euclidean plane $\mathbf{R}^2$, let P be the topological space equal to the union of the circles with center $(1/n,0)$ passing through the origin (for $n\in \mathbf{N}^*$). The space P is compact, connected and locally arcwise connected, but is not unloopable. The group $\pi_1(P,0)$, endowed with the admissible topology, is separated and non-discrete (III, p. 337, Exerc. 7).

#### Remark 1 {#ta-iv-s1-n4-rem-1 .statement tag=020R}

Theorem 4 of III, p. 287 and Prop. 8 (IV, p. 349) remain valid under the more general assumption that G is a finite-dimensional Lie group over $\mathbf{R}$ operating properly in X. For more details, cf. D. Montgomery and C. T. Yang, « The existence of a slice », Annals of mathematics 65 (1957), p. 108–116 ; R. Palais, « On the existence of slices for actions of non-compact Lie groups », Annals of mathematics 73 (1961), p. 295–323 ; and G. Bredon, Introduction to compact transformation groups, Academic Press, 1972.

## EXERCISES {#ta-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
