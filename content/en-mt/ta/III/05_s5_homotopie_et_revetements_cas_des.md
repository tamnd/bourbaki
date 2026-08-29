---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 5
section_title: Homotopie et revêtements (cas des espaces localement connexes par arcs)
lang: en
source: ta-i-iv-fr
book_pages: TA III.308-TA III.320, TA III.334-TA III.338
pdf_pages: 0324-0336, 0350-0354
extraction: native
subsections:
    - "no": 1
      title: Condition homotopique de relèvement des applications continues
      page: 308
      pdf_page: 324
    - "no": 2
      title: Opérations du groupe de Poincaré et morphismes de revêtements
      page: 310
      pdf_page: 326
    - "no": 3
      title: Opérations sans monodromie locale du groupoïde de Poincaré
      page: 312
      pdf_page: 328
    - "no": 4
      title: Topologie admissible des groupes de Poincaré
      page: 315
      pdf_page: 331
statements: 23
exercises: 10
content_sha256: 3e9437934d252802ed8ffe4dc4e1276f2b4d6a063e837e3327e57c7807a6245d
translated_from: content/fr/ta/III/05_s5_homotopie_et_revetements_cas_des.md
source_lang: fr
translation_method: machine
source_content_sha256: c910e3f65fe77bd1794c50ec83433f962e78c09ae594efb024d605ff42619bb7
translation_model: gpt-5.4
translation_run: translate-en-mt-f8d2de3e
glossary_version: 34
glossary_terms_sha256: b839a0ad7bbe7424b31dacee3eb6ef15d489c8fd8576071fc4c2dac012202844
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. HOMOTOPY AND COVERINGS (CASE OF LOCALLY ARCWISE CONNECTED SPACES)

### 1. Homotopic condition for lifting continuous mappings

#### Proposition 1 {#ta-iii-s5-prop-1 .statement tag=01ZL}

Let B be a topological space and let $(E, p)$ be a covering of B. Let Y be a topological space and let $f: Y\rightarrow B$ be a continuous mapping. Let $y\in$ Y$,x\in$ E$,b\in$ B be points such that $f(y) =p(x) =b$. Suppose the space Y connected and locally arcwise connected. In order that there exist a continuous lifting $g: Y\rightarrow E$ of $f$ such that $g(y) =x$, it is necessary and sufficient that the image of the homomorphism $\pi_1(f, y):\pi_1(Y, y)\rightarrow \pi_1(B, b)$ be contained in the image of the homomorphism $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, b)$.

The condition is necessary without any assumption on the space Y. In fact, if such a lifting $g$ exists, we have $\pi_1(f, y) =\pi_1(p, x)\circ \pi_1(g, y)$.

Let us prove that it is sufficient. Let $s: \Lambda_b(B)\rightarrow \Lambda_x(E)$ denote the homeomorphism inverse to the homeomorphism $c\mapsto p\circ c($III, p. 302, cor. 2 of prop. 3) and let $\varphi : \Lambda_y(Y)\rightarrow \Lambda_x(E)$ be the mapping $d\mapsto$ $s(f\circ d)$. The mapping $\varphi$ is continuous (I, p. 132, lemma).

Let $d$ and $d'\in \Lambda_y(Y)$ be paths with origin $y$ having the same term; let us prove that the paths $\varphi (d)$ and $\varphi (d')$ have the same term. Put $c=f\circ d,c'=f\circ d'$. Since the path $d*\overline{d'}$ is a loop in Y at $y$, the path $c*\overline{c'}$ is a loop in B at $b$ and its class belongs to the image of the homomorphism $\pi_1(f, y)$, hence to the image of the homomorphism $\pi_1(p, x)$ by assumption. By cor. 2 of prop. 4 (III, p. 303), the path $s(c*\overline{c'})$ is a loop in E at $x$. The same is true of the path $s(c'*\overline{c})$ which, by uniqueness of the lifting of paths, is equal to $s(c*\overline{c'})$. Therefore $s(c'*\overline{c})(\frac{1}{2}) =s(c')(1) =s(c)(1)$, as was to be proved.

Let us denote by $e_E: \Lambda_x(E)\rightarrow E$ and $e_Y: \Lambda_y(Y)\rightarrow Y$ respectively the term mappings. Since the space Y is supposed connected and locally arcwise connected, the mapping $e_Y$ is surjective and open (III, p. 262, prop. 10). By the preceding paragraph, there exists a unique mapping $g: Y\rightarrow E$ such that $e_E\circ \varphi =g\circ e_Y$. It is continuous, for the mapping $e_Y$ is strict ( I, p. 18, example 2).

Let us verify finally that the mapping $g$ lifts the mapping $f$ and that $g(y) =x$. Every point $z$ of Y is the term of a path $c$ with origin $y$. The path $\varphi (c)$ is a lifting of $f\circ c$ with origin $x$ and with term the point $g(z)$. Therefore $p(g(z)) =f(z)$. For $z=y$ and $c=e_y$, we have $\varphi (e_y) =e_x$, whence $g(y) =x$.

#### Corollary 1 {#ta-iii-s5-prop-1-cor-1 .statement tag=01ZM}

Let B be a connected topological space locally connected by paths, and let $b$ be a point of B. In order that a covering $(E, p)$ of B be trivializable, it is necessary and sufficient that, for every point $x$ of the fibre $E_b$, the homomorphism $\pi_1(p, x)$ be bijective.

Recall that the homomorphism $\pi_1(p, x)$ is injective (III, p. 303, cor. 1 of prop. 4). The statement therefore follows from prop. 1 and I, p. 81, cor. 4 of prop. 6.

#### Remark {#ta-iii-s5-n1-rem-1 .statement tag=01ZN}

Let B be a topological space locally connected by paths, let $b$ be a point of B, and let V be an open connected neighbourhood of $b$ such that the image of the homomorphism from $\pi_1(V, b)$ into $\pi_1(B, b)$ is the subgroup reduced to the identity element. By cor. 1, every covering of B is trivializable over V, and fortiori over every subset of B contained in V.

#### Corollary 2 {#ta-iii-s5-prop-1-cor-2 .statement tag=01ZO}

Let B be a connected topological space locally connected by paths. If, for a point $b$ of B, the group $\pi_1(B, b)$ is reduced to the identity element, the space B is simply connected.

In fact, it follows from corollary 1 that, under these hypotheses, every covering of B is trivializable.

#### Corollary 3 {#ta-iii-s5-prop-1-cor-3 .statement tag=01ZP}

Let

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

be a cartesian square. Suppose that E is a covering of B and that the space $B'$ is connected and locally connected by paths. Let $b'$ be a point of $B'$ and $b=f(b')$. In order that $(E', p')$ be a trivializable covering of $B'$, it is necessary and sufficient that, for every point $x$ of the fibre $E_b$, the image of $\pi_1(p, x)$ contain the image of $\pi_1(f, b)$.

This follows from prop. 1 and I, p. 81, cor. 5 of prop. 6.

### 2. Operations of the Poincaré group and morphisms of coverings

Let B be a connected topological space locally connected by paths and let $b$ be a point of B.

Let E be a covering of B. Since the space B is assumed connected, the fibre $E_b$ is not empty if E is not empty (I, p. 74, prop. 4). By assertion a) of theorem 1 of III, p. 305, the covering E is connected and nonempty if and only if the group $\pi_1(B, b)$ operates transitively on $E_b$.

#### Proposition 2 {#ta-iii-s5-prop-2 .statement tag=01ZQ}

Let E and $E'$ be coverings of B.

a) Let $f: E\rightarrow E'$ be a B-morphism. The mapping $f_b: E_b\rightarrow E'_b$ derived from $f$ is compatible with the operations of $\pi_1(B, b)$ on $E_b$ and $E'_b$ respectively. It is bijective if and only if $f$ is an isomorphism.

b) The mapping $f\mapsto f_b$ is a bijection of the set $\mathscr{C}_B(E; E')$ of B-morphisms from E into $E'$ onto the set $\mathscr{F}_{\pi_1(B,b)}(E_b; E'_b)$ of $\pi_1(B, b)$-morphisms from $E_b$ into $E'_b$.

If $f$ is a B-morphism from E into $E'$, the mapping $f_b: E_b\rightarrow E'_b$ is a $\pi_1(B, b)$-morphism (cf. III, p. 305). Moreover, two B-morphisms from E into $E'$ which coincide on the fibre $E_b$ are equal (I, p. 80, cor. 3 of prop. 6).

Let $\varphi : E_b\rightarrow E'_b$ be a morphism of $\pi_1(B, b)$-sets; let us prove that there exists a B-morphism $f$ of E into $E'$ such that $f_b=\varphi$. We may suppose that the spaces E and $E'$ are connected and non-empty, so that $E_b$ and $E'_b$ are homogeneous $\pi_1(B, b)$-sets. Let $x$ be a point of $E_b$; its stabilizer G is the image of the mapping $\pi_1(p, x)$ (III, p. 305, Theorem 1). Since the mapping $\varphi$ is a $\pi_1(B, b)$-morphism, the group G fixes the point $x'=\varphi (x)$ of $E'_b$, and is therefore contained in the image of the mapping $\pi_1(p', x')$. By Prop. 1 of III, p. 308, there exists a B-morphism $f$ of E into $E'$ such that $f(x) =x'$. The mappings $f_b$ and $\varphi$ are $\pi_1(B, b)$-morphisms of the homogeneous $\pi_1(B, b)$-set $E_b$ into $E'_b$ which agree at the point $x$; they are therefore equal.

If $f: E\rightarrow E'$ is a B-isomorphism, the mapping $f_b: E_b\rightarrow E'_b$ is bijective. Conversely, suppose that the mapping $f_b$ is bijective, and let $g: E'\rightarrow$ E be a B-morphism such that $g_b= (f_b)^{-1}$. The B-morphism $g\circ f: E\rightarrow E$ induces on $E_b$ the identical mapping; it therefore follows from the proposition that $g\circ f=$ Id$_E$. Analogously, $f\circ g=$ Id$_{E'}$, which proves that $f$ is a B-isomorphism.

#### Corollary 1 {#ta-iii-s5-prop-2-cor-1 .statement tag=01ZR}

The coverings E and $E'$ are isomorphic if and only if the $\pi_1(B, b)$-sets $E_b$ and $E'_b$ are isomorphic.

#### Corollary 2 {#ta-iii-s5-prop-2-cor-2 .statement tag=01ZS}

Let $(E, p)$ and $(E', p')$ be connected coverings of B. Let $x$ be a point of $E_b$ and $x'$ a point of $E'_b$. In order that there exist a B-morphism $g: E\rightarrow E'$ such that $g(x) =x'$, it is necessary and sufficient that one have $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. Such a morphism is then unique, and is an isomorphism if and only if the subgroups $p_*(\pi_1(E, x))$ and $p'_*(\pi_1(E', x'))$ of $\pi_1(B, b)$ are equal.

According to III, p. 305, Theorem 1, the mapping of $\pi_1(B, b)$ onto $E_b$ defined by $\gamma \mapsto x\cdot \gamma$ induces by passing to the quotient an isomorphism of the $\pi_1(B, b)$-set $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ onto $E_b$. Analogously, there exists a unique isomorphism of $\pi_1(B, b)$-sets of $p_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ onto $E'_b$. According to Proposition 2, there exists a B-morphism $g: E\rightarrow E'$ such that $g(x) =x'$ if and only if there exists a morphism of $\pi_1(B, b)$-sets of $p_*(\pi_1(E, x))\backslash \pi_1(B, b)$ onto $p'_*(\pi_1(E', x'))\backslash \pi_1(B, b)$ which sends the class $p_*(\pi_1(E, x))$ onto the class $p'_*(\pi_1(E', x'))$. Such a morphism exists if and only if one has $p_*(\pi_1(E, x))\subset p'_*(\pi_1(E', x'))$. It is then unique, since the space E is assumed connected (I, p. 34, cor. 2 of prop. 11). It is an isomorphism if and only if the subgroups $p_*(\pi_1(E, x))$ and $p'_*(\pi_1(E', x'))$ of $\pi_1(B, b)$ are equal.

#### Corollary 3 {#ta-iii-s5-prop-2-cor-3 .statement tag=01ZT}

Let $(E, p)$ be a connected covering of B and let $x$ be a point of the fibre $E_b$. Let N denote the normalizer of $p_*(\pi_1(E, x))$ in $\pi_1(B, b)$. For every element $\gamma$ of N, there exists a unique B-automorphism $g$ of E such that $g(x) =x\cdot \gamma$, and the mapping $\gamma \mapsto g$ defines by passing to the quotient a group isomorphism of $N/p_*(\pi_1(E, x))$ onto Aut$_B(E)$.

Let $\gamma \in \pi_1(B, b)$; one has $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot \gamma )))$ (III, p. 305, Theorem 1, c)). According to Corollary 2, in order that there should exist a B-automorphism $g$ of E such that $g(x) =x\cdot \gamma$, it is necessary and sufficient that $\gamma$ belong to N. Such an isomorphism is then unique. Let $\alpha : N\rightarrow$ Aut$_B(E)$ denote the mapping $\gamma \mapsto g$ thus defined.

Let $\gamma$ and $\gamma '$ be two elements of N. Put $g=\alpha (\gamma ),g'=\alpha (\gamma ')$; one has $g(g'(x)) =g(x\cdot \gamma ') =g(x)\cdot \gamma '= (x\cdot \gamma )\cdot \gamma '=x\cdot (\gamma \gamma ')$ according to relations (4), III, p. 305 and (1), p. 304. Consequently, $\alpha$ is a group homomorphism. In order that $\alpha (\gamma ) =$ Id$_E$, it is necessary and sufficient that one have $x\cdot \gamma =x$, by virtue of the uniqueness of $\alpha (\gamma )$, that is to say $\gamma \in p_*(\pi_1(E, x))$ (III, p. 305, Theorem 1, b)). Finally, if $g$ is a B-automorphism of E, there exists a path $c$ joining $x$ to $g(x)$ in E (which is arcwise connected), and one then has $g(x) =x\cdot \gamma$, where $\gamma$ is the class of the path $p\circ c$. This proves that the homomorphism $\alpha$ is surjective.

The group Aut$_B(E)$ operates on the fibre $E_b$ and is identified with the automorphism group of the homogeneous (right) $\pi_1(B, b)$-set $E_b($cf. A, I, p. 56, prop. 5 and 6).

#### Corollary 4 {#ta-iii-s5-prop-2-cor-4 .statement tag=01ZU}

Let $(E, p)$ be a connected covering of B and let $x$ be a point of the fibre $E_b$. In order that E be a Galois covering of B, it is necessary and sufficient that $p_*(\pi_1(E, x))$ be a distinguished subgroup of $\pi_1(B, b)$. The group Aut$_B(E)$ is then isomorphic to the quotient group $\pi_1(B, b)/p_*(\pi_1(E, x))$.

If $p_*(\pi_1(E, x))$ is a distinguished subgroup of $\pi_1(B, b)$, the group Aut$_B(E)$ operates transitively on the fibre $E_b$ by Corollary 3, so that E is a Galois covering of B (I, p. 102, th. 2). The converse is assertion d) of Theorem 1 (III, p. 305). The last assertion follows from Corollary 3.

### 3. Operations without local monodromy of the Poincaré groupoid

#### Lemma 1 {#ta-iii-s5-lem-1 .statement tag=01ZV}

Let B be a topological space locally connected by paths, let $p: E\rightarrow B$ and $p': E'\rightarrow B$ be étale and separated mappings satisfying the path-lifting property (III, p. 302). Let $g: E\rightarrow E'$ be a mapping such that $p'\circ g=p$. Suppose that $g$ is compatible with the canonical operations of the groupoid $\varpi (B)$ on E and $E'$. Then $g$ is continuous.

Let $c$ be a path in E; put $c'=g\circ c$ and prove that the mapping $c'$ is continuous. Let $d$ denote the path $p\circ c$ in B and, for every $t\in \mathbf{I}$, let $d_t$ denote the path $s\mapsto d(st)$. For every $t\in \mathbf{I}$, we have $c(t) =c(0)\cdot d_t($III, p. 304, remark 3), whence $c'(t) =c'(0)\cdot d_t$ by the hypothesis made on $g$, which proves that $c'$ is a path lifting the path $d$, by the same remark. This proves that the mapping $g$ is pathwise continuous. Since the space E is locally connected by paths (III, p. 261, cor. 2), the mapping $g$ is continuous (III, p. 269, corollary to prop. 13).

Let B be a topological space. Consider an operation $\varphi$ = $(\varphi_{a,b})_{(a,b)\in B\times B}$ of the groupoid $\varpi (B)$ on a set E, relative to a mapping $p: E\rightarrow B$. One says that $\varpi (B)$ operates without monodromy on E (cf. II, p. 168) if for every $b\in$ B and every class of loops $\gamma \in \pi_1(B, b)$, the action of $\gamma$ on the fibre $E_b$ is trivial. If B is connected by paths, it is enough that this be so for one point of B (loc. cit.). We shall say that the operation $\varphi$ of the groupoid $\varpi (B)$ is without local monodromy if every point of B possesses a neighbourhood V such that $\varpi (V)$ operates without monodromy on the set $E_V$ = $\overset{-1}{p}(V)$ relative to the mapping $p_V=p|\overset{-1}{p}(V)$.

#### Remark {#ta-iii-s5-n3-rem-1 .statement tag=01ZW}

Let B be a topological space locally connected by paths and suppose that every point $b$ of B possesses a neighbourhood V such that the image of $\pi_1(V, b)$ in $\pi_1(B, b)$ reduces to the identity element (cf. IV, p. 340, def. 2). Then every operation of the groupoid $\varpi (B)$ is without local monodromy.

In fact, let us consider a set E, a mapping $p: E\rightarrow B$ and an operation $\varphi$ of the groupoid $\varpi (B)$ on E relative to $p$. Let $a$ be a point of B and let V be a neighbourhood of $a$ such that the image of $\pi_1(V, a)$ in $\pi_1(B, a)$ is reduced to the identity element. Let U be a path-connected neighbourhood of $a$ contained in V. Let $b$ be a point of U and let $\gamma \in \pi_1(U, b)$. Let $\delta$ be the class of a path joining $a$ to $b$ in U. Then $\delta \gamma \delta^{-1}$ is the class of a loop at $a$ in U; its image in $\pi_1(B, a)$ is therefore trivial. Thus $\varphi_{a,a}(\delta \gamma \delta^{-1}) =$ Id$_{E_a}$, whence $\varphi_{b,b}(\gamma ) =$ Id$_{E_b}$. This proves that the operation of $\varpi (U)$ on the U-space $E_U$ is without monodromy. Consequently, the operation $\varphi$ is without local monodromy.

#### Proposition 3 {#ta-iii-s5-prop-3 .statement tag=01ZX}

Let B be a topological space locally path-connected and let E be a set endowed with an operation without local monodromy $\varphi$ of the groupoid $\varpi (B)$, relative to a mapping $p: E\rightarrow B$. Then there exists on E a unique topology for which the following conditions are satisfied:

(i) The set E endowed with this topology and the mapping $p$ is a covering of B;

(ii) The canonical operation of $\varpi (B)$ on this covering is identical with the operation $\varphi$.

The uniqueness of such a topology follows from lemma 1 of III, p. 312, where one takes for $g$ the identical mapping of E. To prove its existence, one may moreover suppose that B is connected and nonempty.

Let us suppose first of all that the operation $\varphi = (\varphi_{a,b})_{(a,b)\in B\times B}$ of the groupoid $\varpi (B)$ on the set E, relative to $p$, is without monodromy.

Let $a$ be a point of B. For every point $b\in B$, there exists a path $c$ in B joining $a$ to $b$. If $\gamma \in \varpi_{a,b}(B)$ denotes the class of the path $c$, the bijection $\varphi_{a,b}(\gamma ): E_a\rightarrow E_b$ is independent of the path $c$, since the operation is without monodromy; let $f_{a,b}$ denote this bijection. The mapping $\Phi_a: B\times E_a\rightarrow$ E defined by $(b, x)\mapsto f_{a,b}(x)$ is a bijection; the inverse bijection associates with $x\in E$ the pair $(p(x), f_{p(x),a}(x))$. Endow the set $E_a$ with the discrete topology, so that the B-space $B\times E_a$ is a trivial covering of B. By transport of structure, the bijection $\Phi_a$ endows E with a topology which makes it into a covering of B.

Let us prove that the canonical operation of $\varpi (B)$ on E is identical with the operation $\varphi$. Let $x$ be a point of $E_a$ and $b$ a point of B. Let $c$ be a path in B joining the point $a$ to the point $b$; the mapping $t\mapsto \Phi_a(c(t), x)$ is then a path in E joining the point $x$ to the point $\Phi_a(b, x) =f_{a,b}(x)$. If $\gamma \in \varpi_{a,b}(B)$ denotes the class of the path $c$, we thus have $x\cdot \gamma =f_{a,b}(x)$. This proves that the canonical operation of $\varpi (B)$ on the covering E and the operation $\varphi$ coincide on the classes of paths with origin $a$. Since these classes generate the groupoid $\varpi (B)$, the two operations are equal.

Let us now treat the general case. Let $\mathscr{B}$ be the set of open subsets V of E such that $\varpi (V)$ operates without monodromy on $\overset{-1}{p}(V)$. By hypothesis, the elements of $\mathscr{B}$ cover B. From the preceding, there exists for every $V\in \mathscr{B}$ a unique topology on the set $\overset{-1}{p}(V)$ such that $(\overset{-1}{p}(V), p_V)$ is a covering of V and that the canonical operation of $\varpi (V)$ on this covering coincides with the operation induced by $\varphi$.

Let V and $V'\in \mathscr{B}$. The topology on $\overset{-1}{p}(V\cap V')$ induced by the topology of $\overset{-1}{p}(V)$ (resp. of $\overset{-1}{p}(V')$) defined above makes it into a covering of $V\cap V'$ on which the canonical operation of $\varpi (V\cap V')$ is induced by the operation $\varphi$. These topologies therefore coincide with that of $\overset{-1}{p}(V\cap V')$. There then exists a unique topology on E inducing on each $\overset{-1}{p}(V)$ the topology previously defined (cf. I, § 2, p. 16).

When E is endowed with this topology, the mapping $p$ is continuous and the B-space E is a covering. The canonical operation of $\varpi (B)$ on this covering coincides with the operation $\varphi$ on the classes of paths whose image is contained in one of the open sets of $\mathscr{B}$. By lemma 4 of III, p. 272, these classes generate the groupoid $\varpi (B)$. It follows that these two operations are equal (II, p. 167).

#### Corollary {#ta-iii-s5-n3-cor-1 .statement tag=01ZY}

Let B be a connected topological space, locally connected by arcs, let $(E, p)$ be a B-space whose projection $p$ is etale, separated, and has the path-lifting property. If the canonical operation of $\varpi (B)$ on the set E, relative to $p$, is without local monodromy, then E is a covering of B.

Let us endow E with the canonical operation of $\varpi (B)$ defined by path lifting (III, p. 303, n$^o3$). There exists a topology on E for which conditions (i) and (ii) of prop. 3 are satisfied. This topology coincides with the given topology on E by lemma 1 of III, p. 312.

### 4. Admissible topology of Poincaré groups

Let B be a topological space and let $a$ be a point of B. A subgroup H of $\pi_1(B, a)$ is said to be admissible if every point $b$ of B has a neighbourhood V such that one has $\gamma i_*(\delta )\gamma^{-1}\in H$ for every $\gamma \in \varpi_{a,b}(B)$ and every $\delta \in \pi_1(V, b)$, where $i: V\rightarrow$ B is the canonical injection. If H is a normal subgroup of $\pi_1(B, a)$, it is enough, in order that H be admissible, that this condition be satisfied for one class of paths $\gamma \in \varpi_{a,b}(B)$.

#### Proposition 4 {#ta-iii-s5-prop-4 .statement tag=01ZZ}

There exists a unique topology on $\pi_1(B, a)$, compatible with its group structure, for which the admissible normal subgroups of $\pi_1(B, a)$ form a fundamental system of neighbourhoods of the identity element. For this topology, the open subgroups are exactly the admissible subgroups.

The following facts result from the definition of an admissible subgroup:

a) The group $\pi_1(B, a)$ is admissible;

b) A subgroup containing an admissible subgroup is admissible;

c) The intersection of a finite family of admissible subgroups is admissible;

d) For every admissible subgroup H of $\pi_1(B, a)$ the intersection of the subgroups $\gamma H\gamma^{-1}$, when $\gamma$ runs through $\pi_1(B, a)$, is admissible. In particular, the set of admissible normal subgroups is a filter basis formed of subgroups of $\pi_1(B, a)$ satisfying axiom (GV$'_{III}$) of III, p. 4, whence the first part of the proposition after TG, III, p. 5, example. The second part is then immediate (cf. TG, III, p. 7, corollary of prop. 4).

The topology on the group $\pi_1(B, a)$ characterized in proposition 4 is called the admissible topology.

#### Remark 1 {#ta-iii-s5-n4-rem-1 .statement tag=0200}

If $B_0$ denotes the path-connected component of $a$ in B, the canonical isomorphism $\pi_1(B_0, a)\rightarrow \pi_1(B, a)$ is an isomorphism of topological groups when these groups are endowed with the admissible topology.

#### Remark 2 {#ta-iii-s5-n4-rem-2 .statement tag=0201}

Let B be a topological space. Let $b$ and $b'$ be points of B which belong to the same path-connected component and let $\gamma$ be an element of $\varpi_{b,b'}(B)$. It follows from the definition of an admissible subgroup that, for every admissible subgroup H of $\pi_1(B, b')$, the subgroup $\gamma H\gamma^{-1}$ of $\pi_1(B, b)$ is admissible. Consequently, the isomorphism $u_{\gamma}:\delta \mapsto \gamma \delta \gamma^{-1}$ of $\pi_1(B, b')$ onto $\pi_1(B, b)$ (cf. III, p. 292) is a homeomorphism when these groups are endowed with the admissible topologies.

#### Remark 3 {#ta-iii-s5-n4-rem-3 .statement tag=0202}

Let A and B be topological spaces, let $a$ be a point of A, and let $f: A\rightarrow B$ be a continuous mapping. Put $b=f(a)$. If H is an admissible subgroup of $\pi_1(B, b)$, its inverse image under the homomorphism $\pi_1(f, a)$ is an admissible subgroup of $\pi_1(A, a)$. Consequently, the group homomorphism $\pi_1(f, a):\pi_1(A, a)\rightarrow \pi_1(B, b)$ is continuous, when these groups are endowed with the admissible topology.

#### Proposition 5 {#ta-iii-s5-prop-5 .statement tag=0203}

Let B be a topological space locally arcwise connected, and let $a$ be a point of B. In order that a subgroup H of $\pi_1(B, a)$ be admissible, it is necessary and sufficient that there exist a covering $(E, p)$ of B and a point $x\in E_a$ such that $H =p_*(\pi_1(E, x))$.

Let $(E, p)$ be a covering of B and let $x$ be a point of $E_a$; put $H =p_*(\pi_1(E, x))$ and let us prove that this is an admissible subgroup of $\pi_1(B, a)$. Let $b$ be a point of B and let V be a neighbourhood of $b$ such that $E_V=$ $(\overset{-1}{p}(V), p_V)$ is a trivializable covering of V. Let $\gamma \in \varpi_{a,b}(B)$ ; we shall prove that for every element $\delta \in \pi_1(V, b)$, the class of paths $\gamma \delta \gamma^{-1}$ belongs to H.

By III, p. 301, prop. 3, there exists a unique strict homotopy class $\gamma '$ of path with origin $x$ in E such that $p_*(\gamma ') =\gamma$ Let $y$ be the end of $\gamma '$; we have $p(y) =b($III, p. 302, prop. 4). Let then $\delta '$ be the unique class of path with origin $y$ in E such that $p_*(\delta ') =\delta$. Since $E_V$ is trivializable, $\delta '$ is the class of a loop at $y$. Then $\gamma '\delta '(\gamma ')^{-1}$ is the class of a loop at $a$ in E whose image under $p_*$ is the class $\gamma \delta \gamma^{-1}$, which was to be proved.

Conversely, let H be an admissible subgroup of $\pi_1(B, a)$. Let $\lambda_a(B)$ be the quotient of the space $\Lambda_a(B)$ of paths with origin $a$ by the relation of strict homotopy; since two strictly homotopic paths have the same end-point, the end-point mapping $e: \Lambda_a(B)\rightarrow B$ defines, by passing to the quotient, a mapping $\varepsilon :\lambda_a(B)\rightarrow B$. The composition of classes of paths endows the set $\lambda_a(B)$ with a left action of the group $\pi_1(B, a)$. Endow it with the action of the group H deduced by restriction, and denote by $H\backslash \lambda_a(B)$ the set of its orbits.

The mapping $\varepsilon :\lambda_a(B)\rightarrow B$ induces, by passing to the quotient, a mapping $q: H\backslash \lambda_a(B)\rightarrow B$. The composition of classes of paths endows the set $H\backslash \lambda_a(B)$ with a right operation of the groupoid $\varpi (B)$ relative to the mapping $q$.

This operation is without local monodromy. In fact, let $b$ be a point of B and let V be a neighbourhood of $b$ such that $\gamma i_*(\pi_1(V, b))\gamma^{-1}\subset H$ for every class of paths $\gamma$ joining $a$ to $b$ in B, where $i$ denotes the inclusion of V in B. Since B is locally arcwise connected, one may moreover suppose that V is arcwise connected. Let $c\in V$, let $\delta$ be the class in $\pi_1(B, c)$ of a loop at $c$ contained in V, and let $\delta '$ be an element of $\lambda_a(B)$ such that $\varepsilon (\delta ') =c$. Let $\delta ''$ be an element of $\varpi_{c,b}(V)$ and put $\gamma =\delta '\delta ''$. By definition of V, the element $\delta '\delta (\delta ')^{-1}=\gamma ((\delta '')^{-1}\delta \delta '')\gamma^{-1}$ of $\pi_1(B, a)$ belongs to H. Then $H\delta '\cdot \delta = H\delta '$; this proves that $\pi_1(V, c)$ acts trivially on the set $\overset{-1}{q}(c)$.

By III, p. 313, Proposition 3, there exists a unique topology on $H\backslash \lambda_a(B)$ for which $q$ is continuous and the B-space $(H\backslash \lambda_a(B), q)$ is a covering such that the canonical operation of $\varpi (B)$ on this covering is the operation defined above. By assertion b) of Theorem 1 of III, p. 305, the group $q_*(\pi_1(H\backslash \lambda_a(B),H))$ is equal to H.

We shall say that an operation of the group $\pi_1(B, b)$ on a set X is admissible if the kernel of the canonical mapping $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ is an open subgroup of $\pi_1(B, b)$. This amounts to saying that the homomorphism $\pi_1(B, b)\rightarrow \mathfrak{S}_X$ is continuous if the group $\mathfrak{S}_X$ is endowed with the discrete topology. The mapping $\pi_1(B, b)\times X\rightarrow X$ is then continuous, when X is endowed with the discrete topology. Conversely, consider a continuous operation of $\pi_1(B, b)$ on a discrete space X. Let $x$ be a point of X; its stabiliser is an open subgroup H of $\pi_1(B, b)$ by hypothesis. For $\gamma \in \pi_1(B, b)$, the stabiliser of $\gamma \cdot x$ is the subgroup $\gamma H\gamma^{-1}$, so that the subgroup of $\pi_1(B, b)$ fixing each element of the orbit of $x$ is the intersection of the subgroups $\gamma H\gamma^{-1}$, for $\gamma$ ranging over $\pi_1(B, b)$. It is an open subgroup because the open normal subgroups of $\pi_1(B, b)$ form a basis of its topology (III, p. 315, Proposition 4). It follows that a continuous operation of $\pi_1(B, b)$ on a discrete space X is admissible if it is transitive or, more generally, if the set of orbits of the elements of X is finite.

For every discrete group G, every principal covering E of B with group G, and every point $x\in E_b$, let us recall that the mapping $h_{(E,x)}$ from $\pi_1(B, b)$ into G which, to $\gamma \in \pi_1(B, b)$, associates the unique element $g\in G$ such that $x\cdot g=x\cdot \gamma^{-1}$ is a group homomorphism (III, p. 306, prop. 5).

#### Proposition 6 {#ta-iii-s5-prop-6 .statement tag=0204}

Let B be a topological space and let $b$ be a point of B. Endow the group $\pi_1(B, b)$ with the admissible topology.

a) For every discrete group G, every principal covering E of B with group G, and every $x\in E_b$, the homomorphism $h_{(E,x)}$ is a continuous homomorphism of topological groups.

b) For every covering E of B, the canonical action of $\pi_1(B, b)$ on the fibre $E_b$ is admissible.

It is enough to prove the second assertion. Let K be the set of elements $k\in \pi_1(B, b)$ such that $x\cdot k=x$ for every $x\in E_b$; let us prove that K is an admissible subgroup of $\pi_1(B, b)$.

Let $b'$ be a point of B and let $V'$ be a neighbourhood of $b'$ in B over which the covering E is trivializable. Let $\gamma$ be the class of a path $c$ joining $b$ to $b'$ in B and let $c'$ be the unique path in E with origin $x$ which lifts $c$. For every $\delta \in \pi_1(V', b')$ and every $x'\in E_{b'}$, one has $x'\cdot \delta =x'$. Consequently, for $x\in E_b$ and $\delta \in \pi_1(V', b')$, one has

$$
x\cdot \gamma \delta \gamma^{-1}= ((x\cdot \gamma )\cdot \delta )\cdot \gamma^{-1}= (x\cdot \gamma )\cdot \gamma^{-1}=x
$$

so that $\gamma \delta \gamma^{-1}$ belongs to K. In other words, K is an admissible subgroup, whence the proposition.

#### Proposition 7 {#ta-iii-s5-prop-7 .statement tag=0205}

Let B be a connected topological space, locally connected by arcs, and let $b$ be a point of B. Endow the group $\pi_1(B, b)$ with the admissible topology.

a) Let G be a discrete topological group. For every continuous homomorphism $f:\pi_1(B, b)\rightarrow$ G, there exist a principal covering E of B with group G and a point $x$ of $E_b$ such that $h_{(E,x)}=f$.

b) For every discrete topological space F endowed with an admissible right action of the group $\pi_1(B, b)$, there exists a covering E of B such that the $\pi_1(B, b)$-sets F and $E_b$ are isomorphic.

Let us prove a). Let $f$ be a continuous homomorphism from $\pi_1(B, b)$ into a discrete group G. Its kernel is an open invariant subgroup K of $\pi_1(B, b)$; let H denote the group $\pi_1(B, b)/K$ and $\overline{f}: H\rightarrow G$ the group homomorphism deduced from $f$ by passing to the quotient. By III, p. 316, prop. 5, there exists a connected covering $E'$ of B such that the subgroup K is the stabilizer of every point of the fibre $E'_b$; the covering $E'$ is principal with group $H =\pi_1(B, b)/K$. Let $x'$ be a point of $E'_b$; the homomorphism $h_{(E',x')}:\pi_1(B, b)\rightarrow H$ is surjective with kernel K (III, p. 306, prop. 5). There is therefore a unique group homomorphism $\varphi : H\rightarrow G$ such that $\varphi \circ h_{(E',x')}=f$. The associated covering $E = E'\times^HG$ of B is principal with group G and one has $h_{(E,x)}=\varphi \circ h_{(E',x')}=f$ (III, p. 307, example 2). This proves assertion a).

Let us prove b). Let F be a set endowed with an admissible right action of the group $\pi_1(B, b)$. Let $f:\pi_1(B, b)\rightarrow \mathfrak{S}_F$ denote this action and endow the group $\mathfrak{S}_F$ with the discrete topology. By a), there exist a covering E of B, principal with group $\mathfrak{S}_F$, and a point $x\in E$ such that the homomorphism $h_{(E,x)}$ is equal to $f$. The canonical action of the group $\pi_1(B, b)$ on the fiber over $b$ of the associated covering $E\times^{\mathfrak{S}_F}F$ of B is identified with the action of $\pi_1(B, b)$ on F (III, p. 306, Example 1).

#### Remark 4 {#ta-iii-s5-n4-rem-4 .statement tag=0206}

The admissible topology on $\pi_1(B, b)$ is the least fine topology for which the action of $\pi_1(B, b)$ on $E_b$ is continuous for every connected covering E of B (Prop. 6 of III, p. 318 and Prop. 7 of III, p. 318). If E is a connected covering of B and $x$ a point of the fiber $E_b$, the mapping $c'\mapsto c'(1)$ of $\Lambda_x(E)$ into E is continuous. Consequently, the mapping $c\mapsto x\cdot c$ of $\Lambda_b(B)$ into E is continuous (III, p. 302, Cor. 2 of Prop. 3). By restriction to $\Omega_b(B)$ and passing to the quotient, it follows that the mapping $\gamma \mapsto x\cdot \gamma$ is continuous when the group $\pi_1(B, b)$ is endowed with the quotient-space topology of $\Omega_b(B)$. The admissible topology on $\pi_1(B, b)$ is therefore less fine than the quotient topology of the topology of compact convergence. It may be strictly less fine (III, p. 337, Exercise 7).

#### Remark 5 {#ta-iii-s5-n4-rem-5 .statement tag=0207}

Let B be a connected and locally arcwise connected topological space, let $a$ be a point of B, and let H be a subgroup of $\pi_1(B, a)$. By the preceding remark, if H is admissible, it is also open for the quotient topology of the topology of compact convergence. Conversely, suppose that H is a normal subgroup of $\pi_1(B, a)$ which is open for the quotient topology of the topology of compact convergence. Let $x$ be a point of B and let $\gamma \in \varpi_{a,x}(B)$. The subgroup $\gamma^{-1}H\gamma$ of $\pi_1(B, x)$ is again open for the quotient topology of the topology of compact convergence (III, p. 293, Remark 3). There therefore exists a neighbourhood V of $x$ in B such that $\gamma^{-1}H\gamma$ contains the class of every loop at $x$ whose image is contained in V. Thus $\gamma \pi_1(V, x)\gamma^{-1}\subset H$; since H is normal, this implies that H is an admissible subgroup of $\pi_1(B, a)$.

## EXERCISES {#ta-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
