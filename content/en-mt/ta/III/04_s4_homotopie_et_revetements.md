---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 4
section_title: Homotopie et revêtements
lang: en
source: ta-i-iv-fr
book_pages: TA III.300-TA III.307, TA III.334
pdf_pages: 0316-0323, 0350-0350
extraction: native
subsections:
    - "no": 1
      title: Homotopie et revêtements
      page: 300
      pdf_page: 316
    - "no": 2
      title: Relèvement des chemins
      page: 301
      pdf_page: 317
    - "no": 3
      title: Opérations du groupoïde de Poincaré dans les revêtements
      page: 303
      pdf_page: 319
    - "no": 4
      title: Cas des revêtements associés à un revêtement principal
      page: 305
      pdf_page: 321
statements: 16
exercises: 1
content_sha256: f960904cd7e582f971e9ae716460b2848676516ab8cab1144e1942067c2951c5
translated_from: content/fr/ta/III/04_s4_homotopie_et_revetements.md
source_lang: fr
translation_method: machine
source_content_sha256: a750048c9fd54f1eedac19d785b692367add6fdf7ee793afa41d547643b4161e
translation_model: gpt-5.4
translation_run: translate-en-mt-99ca7ce2
glossary_version: 34
glossary_terms_sha256: fd51d2f2f8ca7e427e8ce997d3fd2cd87a53188f16b335048039917c37a81e82
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. HOMOTOPY AND COVERINGS

### 1. Homotopy and coverings

#### Proposition 1 {#ta-iii-s4-prop-1 .statement tag=01Z5}

Let B be a topological space and let E be a covering of B. Let $B'$ be a topological space and let $f_0$ and $f_1$ be continuous mappings of $B'$ into B. If the mappings $f_0$ and $f_1$ are homotopic, the coverings $f_0^*(E)$ and $f_1^*(E)$ of $B'$ are isomorphic.

Let $\sigma : B'\times \mathbf{I}\rightarrow B$ be a homotopy joining $f_0$ to $f_1$. Let us denote by $i_0$ and $i_1$ the mappings $x\mapsto (x,0)$ and $x\mapsto (x,1)$ of $B'$ into $B'\times \mathbf{I}$. If $t\in  \{0,1\}$, we have $f_t=\sigma \circ i_t$ and the coverings $f_t^*(E)$ and $i^*_t(\sigma^*(E))$ of $B'$ are therefore isomorphic (I, p. 15). Since the topological space $\mathbf{I}$ is locally connected and simply connected (I, p. 127, corollary), the coverings $i^*_0(\sigma^*(E))$ and $i^*_1(\sigma^*(E))$ of $B'$ are isomorphic (I, p. 130, cor. 1 of prop. 8).

#### Corollary {#ta-iii-s4-n1-cor-1 .statement tag=01Z6}

A topological space homotopic to a simply connected topological space is simply connected.

Let B and $B'$ be topological spaces, let $f: B\rightarrow B'$ be a homotopy equivalence and let $g: B'\rightarrow B$ be a continuous mapping, inverse to $f$ up to homotopy. Let E be a covering of B. Since $g\circ f$ is homotopic to the identity mapping of B, the covering E is isomorphic to the covering $f^*(g^*(E))$ (prop. 1). If the space $B'$ is simply connected, the covering $g^*(E)$ is trivializable. Consequently, the covering E is trivializable. This proves that the space B is simply connected.

#### Remark {#ta-iii-s4-n1-rem-1 .statement tag=01Z7}

Let G be a discrete topological group. With the notation of the proposition, suppose that E is a principal covering with group G. Then the coverings $f_0^*(E)$ and $f_1^*(E)$ are isomorphic principal coverings (I, p. 131, remark).

#### Proposition 2 (Lifting of homotopies) {#ta-iii-s4-prop-2 .statement tag=01Z8}

Let B be a topological space and let E be a covering of B. Let $B'$ be a topological space and let $f_0$ and $f_1$ be continuous mappings of $B'$ into B. Let $\sigma : B'\times$ $\mathbf{I}\rightarrow B$ be a homotopy joining $f_0$ to $f_1$. Let $g_0: B'\rightarrow E$ be a continuous lifting of $f_0$ to E. There exists a unique continuous mapping $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow$ E lifting $\sigma$ which is a homotopy with initial term $g_0$. Its term $g_1: B'\rightarrow E$ is a continuous lifting of $f_1$ to E.

This follows from corollary 3 of prop. 8 of I, p. 130, applied to the simply connected and locally connected topological space $\mathbf{I}$.

### 2. Lifting of paths

#### Proposition 3 {#ta-iii-s4-prop-3 .statement tag=01Z9}

Let B be a topological space and let $p: E\rightarrow B$ be a covering. Let us denote by $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ the mapping $c\mapsto p\circ c$. Let us denote by $o_E:\mathscr{C}_c(\mathbf{I}; E)\rightarrow E$ ( resp. $o_B:\mathscr{C}_c(\mathbf{I}; B)\rightarrow B$) the mapping defined by $c\mapsto c(0)$. Then, the diagram

$\mathscr{C}_c(\mathbf{I}; E)^{o_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(\mathbf{I}; B)^{o_B}$ B is a cartesian square.

The topological space $\mathbf{I}$ is locally connected, locally compact and simply connected. The proposition thus follows from prop. 9 of I, p. 131, applied with $T =\mathbf{I}$ and $t= 0$.

#### Corollary 1 {#ta-iii-s4-prop-3-cor-1 .statement tag=01ZA}

The mapping $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ is a covering.

This follows from I, p. 71, cor. 2 of prop. 1.

#### Corollary 2 (Lifting of paths) {#ta-iii-s4-prop-3-cor-2 .statement tag=01ZB}

Let $p: E\rightarrow B$ be a covering, let $x$ be a point of E and $a=p(x)$. The mapping $c\mapsto p\circ c$ is a homeomorphism of the space $\Lambda_x(E)$ of paths in E with origin $x$ onto the space $\Lambda_a(B)$ of paths in B with origin $a$.

With the notation of proposition 3, we have $\Lambda_a(B) =o^{-1}_B(a)$ and $\Lambda_x(E) =\overset{-1}{o_{E}}(x)$. The corollary then follows from I, p. 10, cor. of prop. 4.

We shall say that a continuous mapping $p: E\rightarrow B$ satisfies the path-lifting property if, for every path $c:\mathbf{I}\rightarrow$ B and every point $x$ of E lying over $c(0)$, there exists a path $c'$ in E with origin $x$ which lifts $c$. Such a path is then unique if $p$ is étale and separated (I, p. 34, cor. 1 of prop. 11). Let E be a covering and $p$ its projection; the mapping $p$ is étale, separated and has the path-lifting property (corollary 2). For a partial converse, cf. III, p. 315, corollary.

#### Proposition 4 {#ta-iii-s4-prop-4 .statement tag=01ZC}

Let $p: E\rightarrow B$ be an étale and separated mapping which satisfies the path-lifting property. Let $a$ and $b$ be points of B and let $x$ be a point of E such that $p(x) =a$. Let $c_0$ and $c_1$ be two strictly homotopic paths joining $a$ to $b$ in B. The paths with origin $x$ in E which lift respectively $c_0$ and $c_1$ have the same term and are strictly homotopic.

Let $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow$ B be a strict homotopy joining $c_0$ to $c_1$. For $s\in \mathbf{I}$, let $c'_s$ be the unique path with origin $x$ in E which lifts the path $t\mapsto \sigma (t, s)$. For $(t, s)\in \mathbf{I}\times \mathbf{I}$, put $\sigma '(t, s) =c'_s(t)$; we have $p\circ \sigma '=\sigma$. The mapping $\sigma '$ is constant on $\{0\} \times \mathbf{I}$; by construction, it is continuous on $\mathbf{I}\times  \{s\}$ for every $s\in \mathbf{I}$. It is therefore continuous, by I, p. 37, cor. 1 of th. 1. In particular, the mapping from $\mathbf{I}$ into $E_b$ defined by $s\mapsto \sigma '(1, s)$ is a continuous lifting of the constant path with image $b$; it is therefore constant. This proves that the mapping $\sigma '$ is a strict homotopy joining $c'_0$ to $c'_1$.

#### Corollary 1 {#ta-iii-s4-prop-4-cor-1 .statement tag=01ZD}

Let B be a topological space and let E be a covering of B; let us denote by $p$ its projection. For every pair $(x, y)$ of points of E, the mapping $\varpi_{x,y}(p):\varpi_{x,y}(E)\rightarrow \varpi_{p(x),p(y)}(B)$ is injective. In particular, for every point $x$ of E, the homomorphism $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, p(x))$ is injective.

#### Corollary 2 {#ta-iii-s4-prop-4-cor-2 .statement tag=01ZE}

Let B be a topological space and let E be a covering of B; let us denote by $p$ its projection. Let $x$ be a point of E, and put $b=p(x)$. In order that the class in $\pi_1(B, b)$ of a loop $c$ in B at $a$ should belong to the image subgroup of the homomorphism $\pi_1(p, x)$, it is necessary and sufficient that the path $c'$ with origin $x$ lifting $c$ should be a loop of E at $x$.

The condition is obviously sufficient. Conversely, let $c'_1$ be a loop of E at $x$. Put $c_1=p\circ c'_1$ and suppose that the loops $c$ and $c_1$ are strictly homotopic. By Prop. 4, the path $c'$ has the same end point as the path $c'_1$. It is therefore a loop at $x$.

#### Corollary 3 {#ta-iii-s4-prop-4-cor-3 .statement tag=01ZF}

Let B be a topological space and let $(E_1, p_1)$ and $(E_2, p_2)$ be coverings of B. Let us denote by $(E, p)$ their fibre product over B, and let $x= (x_1, x_2)$ be a point of E. The image of the homomorphism $\pi_1(p, x)$ is the intersection of the images of the homomorphisms $\pi_1(p_1, x_1)$ and $\pi_1(p_2, x_2)$.

Let $c$ be a loop in B at $p_1(x_1) =p_2(x_2)$ and, for $i\in  \{1,2\}$, let $c'_i$ be the path with origin $x_i$ in $E_i$ lifting $c$. The fibre product over B $E = E_1\times_BE_2$ is a covering of B (I, p. 72, cor. 3 of Prop. 2), and the path $c':t\mapsto$ $(c'_1(t), c'_2(t))$ is the unique path with origin $x$ in E which lifts $c$. In order that $c'$ should be a loop, it is necessary and sufficient that $c'_1$ and $c'_2$ should be so. Corollary 3 thus follows from Corollary 2.

### 3. Operations of the Poincaré groupoid in coverings

Let B be a topological space and let $p: E\rightarrow$ B be an etale and separated mapping satisfying the path-lifting property (III, p. 302); this is the case if the mapping $p$ makes E a covering of B (loc. cit.). Let $b$ and $b'$ be points of B and let $c\in \Lambda_{b,b'}(B)$ be a path in B joining $b$ to $b'$. For every point $x$ of the fibre $E_b$, let us denote by $x\cdot c$ the term of the path with origin $x$ in E which lifts $c$. The point $x\cdot c$ belongs to the fibre $E_{b'}$ and depends only on the class $\gamma \in \varpi_{b,b'}(B)$ of the path $c($III, p. 302, prop. 4); we shall thus write $x\cdot \gamma$ instead of $x\cdot c$.

If $c$ is the constant path at $b$, one has $x\cdot \gamma =x$ because the constant path with origin $x$ lifts $c$.

Let $b''$ be another point of B and let $c'\in \Lambda_{b',b''}(B)$. For every point $x$ of $E_b$, one has:

$$
(x\cdot c)\cdot c'=x\cdot (c*c') \tag{1}
$$

In fact, let $\widetilde{c}$ denote the lift of $c$ with origin $x$ and $\widetilde{c}'$ the lift of $c'$ with origin $x\cdot c=\widetilde{c}(1)$. The paths $\widetilde{c}$ and $\widetilde{c}'$ can be juxtaposed and $\widetilde{c}*\widetilde{c}'$ is the path with origin $x$ lifting $c*c'$.

Let us denote by $\varphi_{b,b'}:\varpi_{b,b'}(B)\rightarrow \mathscr{F}(E_b; E_{b'})$ the mapping such that, for $\gamma \in \varpi_{b,b'}(B)$ and $x\in E_b$, one has

$$
\varphi_{b,b'}(\gamma )(x) =x\cdot \gamma
$$

For every $\gamma \in \varpi_{b,b'}(B)$ and every $\gamma '\in \varpi_{b',b''}(B)$, it follows from relation (1) that one has

$$
\varphi_{b,b''}(\gamma \gamma ') =\varphi_{b',b''}(\gamma ')\circ \varphi_{b,b'}(\gamma ) \tag{2}
$$

The family $\varphi = (\varphi_{b,b'})_{(b,b')\in B\times B}$ therefore defines a law of right operation of the groupoid $\varpi (B)$ on the set E relative to the mapping $p: E\rightarrow$ B (II, p. 167). It is called the canonical operation of the groupoid $\varpi (B)$ associated with the mapping $p: E\rightarrow B$. The mapping $\varphi_{b,b}:\pi_1(B, b)\rightarrow \mathscr{F}(E_b; E_b)$ defines a law of right operation of the group $\pi_1(B, b)$ on the fibre $E_b$ of E. This operation is called the canonical operation of $\pi_1(B, b)$ on the fibre $E_b$.

#### Remark {#ta-iii-s4-n3-rem-1 .statement tag=01ZG}

Let $b$ and $b'$ be two points of B$,x$ a point of $E_b,c\in$ $\Lambda_{b,b'}(B)$ a path in B and $\widetilde{c}$ the path in E originating at $x$ which lifts $c$. For every $s\in \mathbf{I}$, let us denote by $c_s$ the path $t\mapsto c(st)$; the path in E originating at $x$ which lifts $c_s$ is the path $t\mapsto \widetilde{c}(st)$ whose term is the point $\widetilde{c}(s)$. We have therefore $\widetilde{c}(s) =x\cdot c_s$ for every $s\in \mathbf{I}$.

Let $B'$ be a topological space and let $p': E'\rightarrow B'$ be an étale and separated mapping satisfying the path lifting property. Let $f: B\rightarrow B'$ and $g: E\rightarrow E'$ be continuous mappings such that $p'\circ g=f\circ p$. For $b,b'\in B,\gamma \in \varpi_{b,b'}(B)$ and $x\in E_b$, we have:

$$
g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma ) \tag{3}
$$

In fact, let $c$ be a path in B whose strict homotopy class is $\gamma$, and let us denote by $\widetilde{c}$ the path in E originating at $x$ which lifts $c$; the path $g\circ \widetilde{c}$ is then the lift originating at $g(x)$ of $f\circ c$ in $E'$.

In particular, for $B = B'$ and $f=$ Id$_B$, we have

$$
g(x\cdot \gamma ) =g(x)\cdot \gamma \tag{4}
$$

Let $p: E\rightarrow B$ and $p': E'\rightarrow B$ be étale and separated mappings satisfying the path lifting property. Let $b$ be a point of B. If $f: E\rightarrow E'$ is a B-morphism, the mapping $f_b: E_b\rightarrow E'_b$ is a $\pi_1(B, b)$-morphism.

#### Theorem 1 {#ta-iii-s4-thm-1 .statement tag=01ZH}

Let B be a topological space, let $(E, p)$ be a covering of B, let $b$ be a point of B and let $x$ be a point of the fibre $E_b$.

a) The orbit of $x$ for the canonical operation of the group $\pi_1(B, b)$ is the intersection of $E_b$ and the arcwise connected component of $x$ in E. In particular, if the space E is arcwise connected, this operation is transitive.

b) The stabilizer (A, I, p. 51) of $x$ is the subgroup $p_*(\pi_1(E, x))$ of $\pi_1(B, b)$.

c) For every $\gamma \in \pi_1(B, b)$, we have $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot$ $\gamma )))$.

d) If the space B is connected and the covering E is Galois, the subgroup $p_*(\pi_1(E, x))$ is normal in $\pi_1(B, b)$.

Assertion a) is immediate. Assertion b) follows from Cor. 2 of Prop. 4 (III, p. 303). Assertion c) follows from b) and from Proposition 2 of A, I, p. 52. Finally, suppose that B is connected and that E is a Galois covering of B. For every $\gamma \in \pi_1(B, b)$, there exists a B-automorphism $g$ of E such that $g(x) =x\cdot \gamma ($I, p. 102, th. 2, c)). We have $p=p\circ g$, whence $p_*(\pi_1(E, x)) =p_*(\pi_1(E, x\cdot \gamma ))$. Assertion d) therefore follows from c).

### 4. Case of coverings associated with a principal covering

Let B be a topological space, let G be a discrete topological group, and let E be a principal covering of B with group G. Let us denote by $p$ the projection of the B-space E. Let $b$ be a point of B and let $x$ be a point of $E_b$.

#### Proposition 5 {#ta-iii-s4-prop-5 .statement tag=01ZI}

The mapping $h_{(E,x)}$ of $\pi_1(B, b)$ into G which, to $\gamma \in$ $\pi_1(B, b)$, associates the unique element $g$ of G such that $x\cdot g=x\cdot \gamma^{-1}$, is a group homomorphism, whose kernel is the subgroup $p_*(\pi_1(E, x))$ of $\pi_1(B, b)$. If E is connected, this homomorphism is surjective.

For every $g\in G$, one has $h_{(E,x\cdot g)}=$ Int($g^{-1}$)$\circ h_{(E,x)}$.

Let E be a principal covering of B with group G, let $x$ be a point of $E_b$, and let us denote by $p$ the projection of E. For every $g\in G$, the mapping $y\mapsto y\cdot g$ is a B-automorphism of E. Hence, for every $g\in G$, every $y\in E_b$, and every $\gamma \in \pi_1(B, b)$, one has the relation $(y\cdot g)\cdot \gamma = (y\cdot \gamma )\cdot g($cf. III, p. 305, relation (4)). Consequently, for $\gamma , \delta \in \pi_1(B, b)$, one has

$$
x\cdot h_{(E,x)}(\gamma \delta ) =x\cdot \delta^{-1}\gamma^{-1}
$$

$$
= (x\cdot h_{(E,x)}(\delta ))\cdot \gamma^{-1}
$$

$$
= (x\cdot \gamma^{-1})\cdot h_{(E,x)}(\delta )
$$

$$
=x\cdot h_{(E,x)}(\gamma )h_{(E,x)}(\delta )
$$

which proves that $h_{(E,x)}$ is a group homomorphism.

Its kernel is the stabilizer of $x$ for the canonical operation of $\pi_1(B, b)$, hence is equal to $p_*(\pi_1(E, x))$ by Theorem 1 of III, p. 305. The mapping $g\mapsto x\cdot g$ is a bijection of G onto $E_b$. The image of the homomorphism $h_{(E,x)}$ is therefore the set of $g\in G$ such that $x\cdot g$ belongs to the orbit of $x$ for this operation. If E is connected, $\pi_1(B, b)$ operates transitively on $E_b($loc. cit.) and the homomorphism $h_{(E,x)}$ is surjective.

Let $g\in G$; for every $\gamma \in \pi_1(B, b)$, one has

$$
x\cdot gh_{(E,x\cdot g)}(\gamma ) = (x\cdot g)\cdot \gamma^{-1}= (x\cdot \gamma^{-1})\cdot g=x\cdot h_{(E,x)}(\gamma )g
$$

whence $h_{(E,x\cdot g)}(\gamma ) =g^{-1}h_{(E,x)}(\gamma )g$. This completes the proof of the proposition.

#### Example 1 {#ta-iii-s4-n4-exa-1 .statement tag=01ZJ}

Let F be a discrete set endowed with an operation of G, and let $X = E\times^GF$ be the associated covering of B. Let us denote by $\varphi : E\times F\rightarrow X$ the canonical B-morphism. It is a morphism of coverings. For every $\gamma \in \pi_1(B, b)$ and every $f\in F$, one then has

(5)

$$
\varphi (x, f)\cdot \gamma =\varphi (x\cdot \gamma , f) =\varphi (x\cdot h_{(E,x)}(\gamma )^{-1}, f) =\varphi (x, h_{(E,x)}(\gamma^{-1})\cdot f)
$$

If one identifies F with $X_b$ by the bijective mapping $f\mapsto \varphi (x, f)$, it follows that the right operation $\pi_1(B, b)\rightarrow$ Aut(X$_b$)$^{\circ}$ is the composite of the homomorphism $h_{(E,x)}$, the antihomomorphism $g\mapsto g^{-1}$ of G into itself and the homomorphism $G\rightarrow$ Aut(F) deduced from the operation of G on F.

#### Example 2 {#ta-iii-s4-n4-exa-2 .statement tag=01ZK}

Let H be a discrete topological group, let $f: G\rightarrow H$ be a group morphism. Endow H with the left operation of G given by $g\cdot h=f(g)h$, for $g\in G$ and $h\in H$. Let $E'= E\times^GH$ be the associated covering; it is a principal covering of group H (I, p. 107, Example 6). Let us denote by $q: E\times H\rightarrow E\times^GH$ the canonical mapping and put $x'=q(x, e)$. We have $h_{(E',x')}=f\circ h_{(E,x)}$.

In fact, let $c$ be a loop at $b$ in B, let $\gamma$ be its class in $\pi_1(B, b)$ and let $g=h_{(E,x)}$; one has therefore $x\cdot \gamma =x\cdot g^{-1}$. Let $\widetilde{c}$ be a path with origin $x$ in E; then $t\mapsto q(\widetilde{c}(t), e)$ is a path with origin $x'$ in $E'$ which lifts the path $p\circ \widetilde{c}$ in B, so that

$$
x'\cdot \gamma =q(x\cdot \gamma , e) =q(x\cdot g^{-1}, e) =q(x, f(g)^{-1}) =q(x, e)\cdot f(g)^{-1}
$$

which proves that $h_{(E',x')}(\gamma ) =f(g)$.

## EXERCISES {#ta-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
