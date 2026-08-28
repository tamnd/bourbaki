---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 6
section_title: Espaces simplement connexes
lang: en
source: ta-i-iv-fr
book_pages: TA I.120-TA I.137, TA I.149-TA I.150
pdf_pages: 0136-0153, 0165-0166
extraction: native
subsections:
    - "no": 1
      title: Revêtement universel
      page: 120
      pdf_page: 136
    - "no": 2
      title: Parties convexes d’un espace numérique
      page: 122
      pdf_page: 138
    - "no": 3
      title: Espaces simplement connexes
      page: 124
      pdf_page: 140
    - "no": 4
      title: Produit d’un espace par un espace simplement connexe
      page: 129
      pdf_page: 145
    - "no": 5
      title: Groupes d’homéomorphismes des espaces simplement connexes
      page: 133
      pdf_page: 149
statements: 37
exercises: 6
content_sha256: ea73a4b6ca508a16865cbf192ca6bdf346b0d854357139b45cb4fefd332cffaf
translated_from: content/fr/ta/I/06_s6_espaces_simplement_connexes.md
source_lang: fr
translation_method: machine
source_content_sha256: 55a3d9d969cfe0bffca545e5628334848137b5a6db2aaf667e32616875d4bf8b
translation_model: gpt-5.4
translation_run: translate-en-mt-0b3dc971
glossary_version: 34
glossary_terms_sha256: e470bf1719c62b6fa07143346b82aed1d50b76f9f860c1d5644c810ac6efa0fa
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. SIMPLY CONNECTED SPACES

### 1. Universal covering

#### Definition 1 {#ta-i-s6-def-1 .statement tag=01RR}

A pointed set is a set X endowed with one of its elements, called the base point. The set X endowed with the point $x$ is sometimes denoted by $(X, x)$. Let $(X, x)$ and $(Y, y)$ be pointed sets; a pointed mapping of $(X, x)$ into $(Y, y)$ is a mapping $f$ of X into Y such that $f(x) =y$.

The notions of pointed topological space, continuous pointed mapping, pointed covering of a pointed topological space, etc., are defined analogously.

If $(X, x)$ and $(Y, y)$ are pointed topological spaces, the set of continuous pointed mappings of $(X, x)$ into $(Y, y)$ is denoted by $\mathscr{C}((X, x); (Y, y))$.

Instead of saying “let $f$ be a pointed mapping of $(X, x)$ into $(Y, y)$”, one often uses the following phrase: “let $f: (X, x)\rightarrow (Y, y)$ be a pointed mapping”.

Let B be a topological space and let $b$ be a point of B.

#### Definition 2 {#ta-i-s6-def-2 .statement tag=01RS}

A pointed covering $(E, x)$ of $(B, b)$ is said to be a universal covering if, for every pointed covering $(E', x')$ of $(B, b)$, there exists a unique morphism of coverings of B, $f: E\rightarrow E'$, such that $f(x) =x'$.

If $(E, x)$ and $(E', x')$ are universal coverings of $(B, b)$, the unique B-morphism of $(E, x)$ into $(E', x')$ is an isomorphism of B-spaces.

Let E be a connected covering of B and let $x$ be a point of the fibre $E_b$. Suppose that, for every pointed covering $(E', x')$ of $(B, b)$, there exists a morphism $f: E\rightarrow E'$ of coverings of B such that $f(x) =x'$. Such a morphism $f$ is then unique (I, p. 34, Cor. 1 of Prop. 11), hence $(E, x)$ is a universal covering of $(B, b)$. *We shall see later (I, p. 126, Cor. of Prop. 3) that this is in particular the case if every covering of E is trivialisable.*

#### Proposition 1 {#ta-i-s6-prop-1 .statement tag=01RT}

Let B be a connected and locally connected topological space and let $b$ be a point of B. Let $(E, x)$ be a universal covering of $(B, b)$. Then E is a Galois covering of B and every covering of B can be associated with E.

The space E is locally connected, since B is. Let $E_0$ be the connected component of $x$ in E, so that the space $(E_0, x)$ is a pointed covering of $(B, b)$ (I, p. 80, Cor. 1 of Prop. 6). There then exists a unique morphism of coverings $f: E\rightarrow E_0$ such that $f(x) =x$. If $i$ denotes the canonical injection of $E_0$ into E, the mapping $i\circ f: E\rightarrow E$ is a morphism of coverings which maps $x$ to $x$, just as does the mapping Id$_E$; since $(E, x)$ is a universal covering of $(B, b)$, we therefore have $i\circ f=$ Id$_E$. It follows that $i$ is surjective, hence $E_0= E$. Consequently, E is connected.

Let $y$ be a point of $E_b$ and let us consider the pointed covering $(E, y)$ of $(B, b)$; by hypothesis there exists a unique morphism of coverings $f: E\rightarrow E$ such that $f(x) =y$. The mapping $s: E\rightarrow E\times_BE$ defined by $t\mapsto (t, f(t))$ is a continuous section of the mapping pr$_1: E\times_BE\rightarrow E$. By Corollary 4 of I, p. 81, this proves that the covering $E\times_BE$ of E given by the mapping pr$_1$ is trivializable. The covering E is therefore Galois (Theorem 2 of I, p. 102). It then follows from I, p. 112, corollary to Proposition 10, that every covering of B can be associated with E.

#### Corollary {#ta-i-s6-n1-cor-1 .statement tag=01RU}

Let B be a locally connected topological space. Let $b$ be a point of B and let $(E, x)$ be a universal covering of $(B, b)$. For a subspace A of B, the following two properties are equivalent:

(i) The covering E is trivializable over A;

(ii) Every covering of B is trivializable over A.

Property (ii) obviously implies property (i). The converse follows from the fact that every covering of B can be associated with the covering E (I, p. 105, Proposition 7).

### 2. Convex subsets of a numerical space

Let E be the $n$-dimensional numerical space *(or, more generally, a topological vector space over $\mathbf{R}$)$*$. For every pair $(x, y)$ of points of E, the segment (resp. the open segment) with endpoints $x$ and $y($cf. EVT, II, p. 7) is by definition the set of points of E of the form $tx+$ $(1-t)y$, for $t\in [0,1]$ (resp. for $t\in ]0,1[$). Let A be a subset of E. One says that the set A is convex if for every pair $(x, y)$ of points of A and every $t\in \mathbf{I}$, the point $tx+ (1-t)y$ belong to A.

*A convex subset is connected by arcs.*

#### Lemma 1 {#ta-i-s6-lem-1 .statement tag=01RV}

Let E be the $n$-dimensional numerical space and let A be a convex compact subset of E of which 0 is an interior point. For every $x\in E$, let us denote by $p_A(x)$ the greatest lower bound in $\overline{\mathbf{R}}$ of the set of real numbers $t >0$ such that $x\in tA$.

The mapping $p_A$ is finite, continuous, and has the following properties:

(i) For every $x\in E$ such that $x= 0\not$ , one has $p_A(x)>0$ ;

(ii) For every $s\in \mathbf{R}_+$ and every $x\in E$, one has $p_A(sx) =sp_A(x)$.

(iii) For all $x$ and $y\in E$, one has $p_A(x+y)\leqslant p_A(x) +p_A(y)$.

(iv) In order that a point $x$ of E belong to A, it is necessary and sufficient that $p_A(x)\leqslant 1$.

For $x\in E$, let us denote by $\|x\|$ the euclidean norm of $x$ (TG, VI, p. 7). Since A is compact, there exists a real number $M>0$ such that every point $x$ of A satisfies $\|x\|\leqslant M$. Since 0 is an interior point of A, there exists a real number $m >0$ such that every point $x$ of E such that $\|x\|\leqslant m$ belong to A. Consequently, one has the relation $\|x\|/M\leqslant p_A(x)\leqslant \|x\|/m$, for every $x\in E$. In particular, $p_A(0) = 0$ and $p_A(x)= 0\not$ if $x= 0\not$ .

Assertions (ii) and (iv) follow immediately from the definition of the mapping $p_A$.

Let $x$ and $y$ be points of E. Let $x'$ and $y'$ be points of A such that $x=p_A(x)x'$ and $y=p_A(y)y'$. If $x$ and $y$ are not both zero, $p_A(x) +p_A(y)>0$ and one has

$$
x+y=p_A(x)x'+p_A(y)y'
$$

$$
= (p_A(x) +p_A(y))(\frac{p_A(x)}{p_A(x) + p_A(y)}x'+\frac{p_A(y)}{p_A(x) + p_A(y)}y')
$$

Since A is convex, this proves that $x+y$ belongs to $(p_A(x) +$ $p_A(y))A$, whence $p_A(x+y)\leqslant p_A(x) +p_A(y)$. If $x=y= 0$, this inequality still holds, for $p_A(0) = 0$. This proves assertion (iii).

Applying this inequality to $x+y$ and $-y$, one deduces that, for every pair $(x, y)$ of points of E, one has

$|p_A(x+y)-p_A(x)|\leqslant$ max($p_A(y), p_A(-y)$)$\leqslant m^{-1}\|y\|$.

This proves that the mapping $p_A$ is continuous, whence the lemma.

The mapping $p_A$ is called the gauge of the convex subset A.

#### Proposition 2 {#ta-i-s6-prop-2 .statement tag=01RW}

Let E be the numerical space of dimension $n$ and let A be a convex and compact subset of E of which 0 is an interior point. There exists a unique bijection $u$ of E onto itself satisfying the following three properties:

(i) For every $x\in E$ and every $t\in \mathbf{R}_+,u(tx) =tu(x)$;

(ii) For every $x\in E$, there exists $\lambda \in \mathbf{R}_+$ such that $u(x) =\lambda x$;

(iii) One has $u(A) =\mathbf{B}_n$.

The mapping $u$ is a homeomorphism and induces, by passing to subspaces, a homeomorphism of A onto $\mathbf{B}_n$, a homeomorphism of the interior of A onto the interior of $\mathbf{B}_n$ and a homeomorphism of the boundary of A in E onto the sphere $\mathbf{S}_{n-1}$.

Let $p_A$ be the gauge of the convex subset A. Let $x\in E$ and let $t\in \mathbf{R}_+$; in order that $x\in tA$, it is necessary and sufficient that $p_A(x)\leqslant t$. Since A is compact, there exists a real number M such that $\|x\|\leqslant M$ for every $x\in A$.

Let $u$ be a mapping satisfying the conditions of the proposition. We have $u(0) = 0$. Let $x\in E-\{0\}$ and let $\lambda \in \mathbf{R}_+$ be such that $u(x) =\lambda x$. For every $t\in \mathbf{R}_+$ such that $tx\in A$, we have $u(tx) =t\lambda x$. Since $u$ is injective, $\lambda = 0\not$ . Since $u(A)$ is contained in $\mathbf{B}_n$, we also have $\lambda \leqslant p_A(x)/\|x\|$. Put $z=x/\|x\|$; this is a point of $\mathbf{S}_{n-1}$. In order that $z$ should have a preimage in A under $u$, it is necessary and sufficient that the point $(\lambda \|x\|)^{-1}x$ should belong to A, that is, that $\lambda \|x\|\geqslant p_A(x)$, i.e. $\lambda \geqslant p_A(x)/\|x\|$. This implies the uniqueness of such a mapping $u$.

Let us now denote by $u$ the mapping of E into itself which maps 0 to 0 and $x$ to $(p_A(x)/\|x\|)x$, for every $x\in E-\{0\}$.

By Lemma $1,u$ is continuous at every point of E $-\{0\}$. We have $\|u(x)\|=p_A(x)$ for every $x\in E$ and $p_A(x)\rightarrow 0$ when $x\rightarrow 0$ (loc. cit.); consequently, $u$ is continuous at 0. Therefore $u$ is continuous.

The only preimage of 0 under $u$ is 0. Let $y\in E-\{0\}$. In order that an element $x$ of E should satisfy $u(x) =y$, it is necessary and sufficient that $x= (\|y\|/p_A(y))y$. It follows that $u$ is a continuous bijection of E onto itself. Its inverse is the mapping $v:y\mapsto (\|y\|/p_A(y))y$. Since $p_A$ is continuous and vanishes only at 0, the mapping $v$ is continuous at every point of E $-\{0\}$; the inequality $p_A(y)\geqslant \|y\|/M$ implies that $\|v(y)\|\leqslant M\|y\|$ for every $y\in E$. It follows that $v$ is continuous. Therefore the mapping $u$ is a homeomorphism of E onto itself. Since the relations $p_A(x)\leqslant 1$ and $x\in A$ are equivalent, we also have $u(X) =\mathbf{B}_n$. The proposition follows.

#### Example {#ta-i-s6-n2-exa-1 .statement tag=01RX}

The set $[0,1]^n$ is a convex, compact subset with nonempty interior of $\mathbf{R}^n$. It follows from proposition 2 of I, p. 123 that it is homeomorphic to the closed euclidean ball. More precisely, for every point $x$ of the interior $]0,1[^n$ and every point $b$ of the open euclidean ball, there exists a homeomorphism of $[0,1]^n$ onto $\mathbf{B}_n$ which maps $x$ to $b$ and induces, by passing to subspaces, a homeomorphism of $]0,1[^n$ onto the open euclidean ball, and also a homeomorphism of the boundary of $[0,1]^n$ onto the sphere $\mathbf{S}_{n-1}$.

It follows that every convex, compact subset with nonempty interior of $\mathbf{R}^n$ is homeomorphic to a cube (loc. cit.).

### 3. Simply Connected Spaces

#### Definition 3 {#ta-i-s6-def-3 .statement tag=01RY}

A topological space is said to be simply connected if all its coverings are trivializable.

A simply connected space is connected. In fact, if a space X is the disjoint union of two nonempty open sets U and V, the canonical injection of U into X is a covering which is not trivializable.

The empty space is simply connected. Every topological space reduced to a point is simply connected.

#### Remark 1 {#ta-i-s6-n3-rem-1 .statement tag=01RZ}

Let B be a simply connected topological space and let $(E, p)$ be a covering of B. If the space E is connected and nonempty, the mapping $p$ is a homeomorphism. Let, for example, G be a connected topological group and H a discrete subgroup of G, so that the canonical mapping $p: G\rightarrow G/H$ makes G a covering of $G/H$ (I, p. 100, cor. 2 of th. 1). If the space $G/H$ is simply connected, the mapping $p$ is a homeomorphism and H is the one-element subgroup.

#### Remark 2 {#ta-i-s6-n3-rem-2 .statement tag=01S0}

Let B be a topological space such that every point has a simply connected neighbourhood; then every covering of a covering of B is a covering of B. Consider in fact a covering $(E, p)$ of B together with a covering $(F, q)$ of E. We shall prove that $(F, p\circ q)$ is a covering of B. Since the question is local on B, we may suppose that the space B is simply connected and therefore that E is a trivializable covering of B. Let V be a connected component of E. It is open and closed and $p|V: V\rightarrow B$ is a homeomorphism (I, p. 69, proposition 1); it follows that the space V is simply connected. Every connected component W of $\overset{-1}{q}(V)$ is open and closed in $\overset{-1}{q}(V)$, hence in F, and the mapping $q$ induces a homeomorphism of W onto V. The mapping $p\circ q$ therefore makes F a covering of B, trivializable (loc. cit.).

#### Proposition 3 {#ta-i-s6-prop-3 .statement tag=01S1}

Let B be a topological space. Let $(E, p)$ be a covering of B and let $y$ be a point of E. Let X be a simply connected topological space, let $f: X\rightarrow B$ be a continuous mapping and let $x$ be a point of X such that $f(x) =p(y)$. Then there exists a unique continuous lifting $g: X\rightarrow E$ of the mapping $f$ such that $g(x) =y$.

The mappings $g$ sought correspond bijectively (I, p. 9, prop. 3) to the continuous sections $s$ of the covering pr$_1: X\times_BE\rightarrow X$ such that $s(x) = (x, y)$. Such a section exists because the space X is simply connected; it is unique because the space X is connected (I, p. 34, cor. 1 of prop. 11).

#### Example 1 {#ta-i-s6-n3-exa-1 .statement tag=01S2}

Let X be a simply connected topological space and let $f$ be a continuous function from X into $\mathbf{C}^*$. Recall (I, p. 101, example 6) that the mapping $z\mapsto e^z$ makes $\mathbf{C}$ a covering of $\mathbf{C}^*$. By prop. 3, there exists a continuous function $h: X\rightarrow \mathbf{C}$ such that $f(x) =e^{h(x)}$ for every $x\in X$. If $h': X\rightarrow \mathbf{C}$ is another continuous function such that $f(x) =e^{h'(x)}$ for every $x\in X$, there exists an integer $q\in \mathbf{Z}$ such that $h'=h+ 2\pi iq$.

Analogously, let $n$ be an integer $>0$; the mapping $z\mapsto z^n$ makes $\mathbf{C}^*$ into a covering of itself (I, p. 101, example 5). There therefore exists a continuous function $k$ from X into $\mathbf{C}^*$ such that $k(x)^n=f(x)$ for every $x\in X$, for example the function $k(x) =e^{h(x)/n}$. If $k': X\rightarrow \mathbf{C}^*$ is another continuous function such that $k'(x)^n=f(x)$ for every $x\in X$, there exists an $n^e$ root of unity $\mu\in \mathbf{C}$ such that $k'=\mu k$.

#### Corollary {#ta-i-s6-n3-cor-1 .statement tag=01S3}

Let B be a topological space and let $b$ be a point of B. Let E be a simply connected covering of B. For every point $x$ of $E_b$, the pointed space $(E, x)$ is a universal covering of $(B, b)$.

#### Proposition 4 {#ta-i-s6-prop-4 .statement tag=01S4}

The product of two simply connected spaces, one of which is locally connected, is a simply connected space.

Let X and Y be simply connected spaces, and suppose that Y is locally connected. The space $X\times Y$ is connected, since X and Y are so (I, p. 124). Let $(Z, f)$ be a nonempty covering of $X\times Y$; let us prove that it is trivializable. By corollary 2 of I, p. 70, it is enough to prove that for every point $z_0$ of Z, there exists a continuous section $s$ of $f$ such that $s(f(z_0)) =z_0$. Let therefore $z_0$ be a point of Z. Put $(x_0, y_0) =f(z_0)$. The subspace $X\times  \{y_0\}$ of $X\times Y$ is homeomorphic to X. Hence the covering deduced from Z over $X\times  \{y_0\}$ is trivializable and has a continuous section $\sigma$ such that $\sigma (x_0, y_0) =z_0$. Analogously, for every point $x$ of X, there exists a continuous section $\tau_x$ of $f$ over $\{x\}\times Y$ such that $\tau_x(x, y_0) =\sigma (x, y_0)$. For $(x, y)\in X\times Y$, put $s(x, y) =\tau_x(x, y)$. The mapping $s$ is a section of $f$, and one has $s(x_0, y_0) =z_0$. Since the space Y is connected and locally connected, it follows from theorem 1 of I, p. 35 that the mapping $s$ is continuous.

#### Proposition 5 {#ta-i-s6-prop-5 .statement tag=01S5}

A connected and locally connected topological space such that the intersection of any two connected open subsets is connected is a simply connected space.

Let B be such a topological space. Let $(E, p)$ be a covering of B, let $x$ be a point of E and write $b=p(x)$. We have to prove that there exists a continuous section $s$ of $p$ such that $s(b) =x$ (cor. 2, I, p. 70). Let $\mathscr{S}$ be the set of pairs $(U, s_U)$ where U is a connected open subset of B containing $b$ and $s_U$ a continuous section of $p_U:\overset{-1}{p}(U)\rightarrow U$ such that $s_U(b) =x$. The set $\mathscr{S}$ is not empty ( I, p. 34, prop. 10). Let $(U, s_U)$ and $(V, s_V)$ be elements of $\mathscr{S}$. Then $s_U|U\cap V$ and $s_V|U\cap V$ are continuous sections of $p_{U\cap V}$ taking the value $x$ at $b$. By hypothesis, $U\cap V$ is connected; hence $s_U|U\cap V =s_V|U\cap V$ (I, p. 34, cor. 1 of prop. 11). Let A be the union of the open sets U when $(U, s_U)$ ranges over $\mathscr{S}$ and let $s: A\rightarrow E$ be the unique mapping such that $s|U =s_U$ for every pair $(U, s_U)\in \mathscr{S}$. The set A is open and connected (TG, I, p. 81, prop. 2), it contains $b$, and $s$ is a continuous section of $p_A$ such that $s(b) =x$. It now suffices to prove that the set A is closed, which will imply that it is equal to B.

Let $a$ be a point of B adherent to A and let V be a connected open neighbourhood of $a$ such that the covering E is trivializable over V. There exists a point $c$ in $A\cap V$ and a continuous section $s_V$ of $p_V$ such that $s_V(c) =s(c)$. Let $A'$ be the open set $A\cup V$. Since $A\cap V$ is connected, there exists a continuous section $s'$ of $p_{A'}$ extending $s$ and $s_V($I, p. 35, cor. 3 of prop. 11); the pair $(A', s')$ belongs to $\mathscr{S}$ and therefore $A'$ is contained in A. Hence $a$ belongs to A and A is closed.

#### Corollary {#ta-i-s6-n3-cor-2 .statement tag=01S6}

Every interval of the real line $\mathbf{R}$ is simply connected.

In fact, the connected subspaces of $\mathbf{R}$ are the intervals (TG, IV, p. 8, th. 4) and the intersection of two intervals is an interval.

#### Example 2 {#ta-i-s6-n3-exa-2 .statement tag=01S7}

The numerical space of $n$ dimensions $\mathbf{R}^n$ (TG, VI, p. 1) is simply connected. It is in fact a product of simply connected and locally connected spaces (I, p. 126, prop. 4 and cor. of prop. 5 above). The same is true of every open or closed cell in $\mathbf{R}^n$. A parallelotope, an euclidean ball, open or closed, in $\mathbf{R}^n$ are simply connected because they are homeomorphic to a cell (TG, VI, p. 10, prop. 2 and I, p. 124, example).

#### Proposition 6 {#ta-i-s6-prop-6 .statement tag=01S8}

Let X be a topological space. Let $U_1$ and $U_2$ be open ( resp. closed) subspaces of X such that $X = U_1\cup U_2$. Suppose that $U_1$ and $U_2$ are simply connected and that their intersection $U_1\cap U_2$ is connected and nonempty. Then the space X is simply connected.

Let $(E, p)$ be a covering of X and let $y$ be a point of E. It is enough to prove that there exists a continuous section $s$ of $p$ such that $s(p(y)) =y$ (I, p. 70, cor. 2 of prop. 1). Suppose for example that $p(y)$ belongs to $U_1$. There then exists a continuous section $s_1: U_1\rightarrow E$ of $p_{U_1}$ such that $s_1(p(y)) =y$. Let $x$ be a point of $U_1\cap U_2$; there exists a continuous section $s_2$ of $p_{U_2}$ such that $s_2(x) =s_1(x)$. By corollary 3 of proposition 11 of I, p. 34, there exists a continuous section $s$ of $p$ extending both $s_1$ and $s_2$.

#### Example 3 {#ta-i-s6-n3-exa-3 .statement tag=01S9}

For $n\geqslant 2$, the sphere $\mathbf{S}_n$ (TG, VI, p. 10) is simply connected. Indeed, the sphere $\mathbf{S}_n$ is the union of two closed hemispheres homeomorphic to $\mathbf{B}_n$ whose intersection is homeomorphic to $\mathbf{S}_{n-1}($cf. TG, VI, p. 12). For $n\geqslant 2$, the sphere $\mathbf{S}_{n-1}$ is connected, whence the assertion.

On the other hand, the circle $\mathbf{S}_1$ is not simply connected. Indeed, the continuous mapping $p:\mathbf{R}\rightarrow \mathbf{S}_1$ defined by $p(\theta ) =$ (cos $\theta$, sin $\theta$ ) makes $\mathbf{R}$ a connected covering of $\mathbf{S}_1$ of infinite degree, hence one which is not trivializable.

#### Example 4 {#ta-i-s6-n3-exa-4 .statement tag=01SA}

Let E be a finite-dimensional vector space of dimension $n$ over $\mathbf{R}$ and let F be an affine subspace of E of codimension $p\geqslant 3$. The set $\mathbf{R}^p-\{0\}$ is homeomorphic to $\mathbf{R}\times \mathbf{S}_{p-1}$ (TG, VI, p. 10, cor. 2), and therefore is simply connected, since $\mathbf{R}$ and $\mathbf{S}_{p-1}$ are locally connected and simply connected (I, p. 126, prop. 4). The set E-F, homeomorphic to $\mathbf{R}^{n-p}\times$ $(\mathbf{R}^p-\{0\})$, is therefore simply connected (loc. cit.).

#### Proposition 7 {#ta-i-s6-prop-7 .statement tag=01SB}

Let X be a topological space. Let $U_1$ and $U_2$ be connected open ( resp. closed) subspaces of X such that $X = U_1\cup$ $U_2$. If the space X is simply connected, then $U_1\cap U_2$ is connected.

Put $U = U_1\cap U_2$ and suppose, arguing by contradiction, that the space U is not connected. We shall construct a connected covering of X of infinite degree; such a covering is not trivializable.

By assumption, the set U is the union of two disjoint, non-empty sets A and B, open (resp. closed) in X. For $i\in  \{1,2\}$, let $Y_i$ be the $U_i$-space $(U_i\times \mathbf{Z}$, pr$_1)$ and let $Z_i$ be the subspace $U\times \mathbf{Z}$ of $Y_i$. The mapping $h: Z_1\rightarrow Z_2$ defined by

$(x, n)$ if $x\in A$ and $n\in \mathbf{Z}$

$$
h(x, n) =
$$

$(x, n+ 1)$ if $x\in B$ and $n\in \mathbf{Z}$

is a homeomorphism. Let Y be the space obtained by gluing $Y_1$ and $Y_2$ along $Z_1$ and $Z_2$ by means of the homeomorphism $h$ (TG, I, p. 17).

For $i\in  \{1,2\}$, the canonical mapping $g_i$ of $Y_i$ into Y is a homeomorphism of $Y_i$ onto an open (resp. closed) subset of Y (loc. cit., prop. 9). For every integer $n\in \mathbf{Z}$, the sets $g_i(U_i\times  \{n\})$, $i\in  \{1,2\}$, are connected; since A and B are non-empty, $g_1(U_1\times \{n\})$ meets $g_2(U_2\times  \{n\})$ and $g_2(U_2\times  \{n+1\})$. It follows that the space Y is connected (TG, I, p. 81, corollary).

For $x\in U$ and $n\in \mathbf{Z}$, one has (pr$_1\circ h$)$(x, n) =x=$ pr$_1(x, n)$. There exists therefore a unique continuous mapping $p: Y\rightarrow X$ such that $p\circ g_i=$ pr$_1$ for $i\in  \{1,2\}$. Let us prove that the X-space $(Y, p)$ is a covering. By construction, the fibres of the mapping $p$ are homeomorphic to the discrete space $\mathbf{Z}$.

For $i\in  \{1,2\}$, the mapping $g_i$ defines by passing to subspaces an isomorphism of $U_i$-spaces of $U_i\times \mathbf{Z}$ onto $\overset{-1}{p}(U_i)$.

By definition of the space Y, there exists a unique mapping $k$ of $(X-A)\times \mathbf{Z}$ into Y such that $k(x, n) =g_1(x, n)$ for $x\in (U_1-A)\times \mathbf{Z}$ and $k(x, n) =g_2(x, n-1)$ for $x\in (U_2-A)\times \mathbf{Z}$; it is an isomorphism of (X-A)-spaces of $(X-A)\times \mathbf{Z}$ onto $\overset{-1}{p}(X-A)$. Analogously, there exists a unique mapping $k'$ of $(X-B)\times \mathbf{Z}$ into Y which coincides with $g_1$ on $(U_1-B)\times \mathbf{Z}$ and with $g_2$ on $(U_2-B)\times \mathbf{Z}$ and it is an isomorphism of (X-B)-spaces of $(X-B)\times \mathbf{Z}$ onto $\overset{-1}{p}(X-B)$.

This proves that the X-space $(Y, p)$ is trivializable over the subsets $U_1,U_2$, X-A and X-B. One has $U_1\cup U_2= X$; if $U_1$ and $U_2$ are open in X, this proves that $(Y, p)$ is a covering of X. The same holds when $U_1$ and $U_2$ are closed in X, for then X-A and X-B are open subsets of X whose union is X. The proposition is thus proved.

#### Corollary {#ta-i-s6-n3-cor-3 .statement tag=01SC}

Let X be a simply connected topological space and let A be a connected subset of X. If the complement of A is connected, its boundary is also connected.

Let $X_1$ and $X_2$ be the closures of A and of X-A respectively. The sets $X_1$ and $X_2$ are closed and connected (TG, I, p. 81, prop. 1); one has $X_1\cup X_2= X$ and their intersection $X_1\cap X_2$ is equal to the boundary of A. It is then enough to apply proposition 7.

### 4. Product of a Space by a Simply Connected Space

#### Proposition 8 {#ta-i-s6-prop-8 .statement tag=01SD}

Let B be a topological space. Let T be a simply connected and locally connected space. Let E be a covering of $B\times T$, with projection $p$, and let $t$ be a point of T. Let $E_t$ denote the space $\overset{-1}{p}(B\times  \{t\})$; endowed with the mapping $p_t=$ pr$_1\circ p|E_t: E_t\rightarrow B$, it is a covering of B. There then exists a unique $(B\times T)$-isomorphism of the covering $(E_t\times T, p_t\times$ Id$_T)$ onto the covering E which maps $(x, t)$ to $x$ for every $x\in E_t$.

One may suppose that B is not empty. Let $x$ be a point of $E_t$. By proposition 3 of I, p. 125 applied to the covering E and to the continuous mapping $T\rightarrow B\times T,u\mapsto (p_t(x), u)$, there exists a unique continuous mapping $f_x: T\rightarrow E$ such that $f_x(t) =x$ and $p(f_x(u)) =$ $(p_t(x), u)$ for every $u\in T$. Let $h: E_t\times T\rightarrow E$ be the mapping defined by $h(x, u) =f_x(u)$. We have $h(x, t) =x$ and $p\circ h=p_t\times$ Id$_T$. The mapping $h$ is a lifting to E of the mapping $p_t\times$ Id$_T$. The restriction of $h$ to $E_t\times  \{t\}$ is continuous, as is also the restriction of $h$ to $\{x\} \times T$ for every point $x$ of $E_t$. Since the space T is locally connected, the mapping $h$ is continuous ( I, p. 37, cor. 1 of th. 1).

Let $b$ be a point of B. By construction, the mapping $h$ induces a bijection of the fibre $\overset{-1}{p_{t}}(b)\times  \{t\}$ of $E_t\times T$ onto the fibre $\overset{-1}{p}(b, t)$ of E at $(b, t)$. Since the space T is connected and locally connected, the mapping $h$ is bijective (I, p. 84, cor. of prop. 7). It is therefore a $B\times T$-isomorphism (I, p. 30, cor. 2 of prop. 6).

Let $h'$ be a $(B\times T)$-isomorphism of the covering $(E_t\times T, p_t\times$ Id$_T)$ onto the covering E which maps $(x, t)$ to $x$ for every point $x\in E_t$. For every $x\in E_t$, the mappings $u\mapsto h(x, u)$ and $u\mapsto h'(x, u)$ are equal (I, p. 34, cor. 1 of prop. 11). Hence $h=h'$.

#### Corollary 1 {#ta-i-s6-prop-8-cor-1 .statement tag=01SE}

Under the hypotheses of prop. 8, if $t$ and $t'$ are two points of T, the coverings $E_t$ and $E_{t'}$ are B-isomorphic.

#### Corollary 2 {#ta-i-s6-prop-8-cor-2 .statement tag=01SF}

Under the hypotheses of prop. 8, let $(E, p)$ and $(E', p')$ be coverings of $B\times T$ and let $k: E_t\rightarrow E'_t$ be a B-morphism. There exists a unique $(B\times T)$-morphism $\widetilde{k}: E\rightarrow E'$ which extends $k$. If $k$ is a B-isomorphism, $\widetilde{k}$ is a $(B\times T)$-isomorphism.

By proposition 8, one may suppose that there exist coverings F and $F'$ of B such that E and $E'$ are respectively the $(B\times T)$-spaces $F\times T$ and $F'\times T$. One then has $E_t= F\times  \{t\},E'_t= F'\times  \{t\}$ and the mapping $k$ is written $(x, t)\mapsto (k'(x), t)$, where $k'$ is a B-morphism of F into $F'$. The mapping $k'\times$Id$_T$ is a $B\times T$-morphism extending $k$; it is an isomorphism if $k$ is one.

Let $\widetilde{k}: E\rightarrow E'$ be a $(B\times T)$-morphism extending $k$. Let $x$ be a point of F. Denote by $q$ the projection of F and put $b=q(x)$. The mappings $u\mapsto \widetilde{k}(x, u)$ and $u\mapsto (k'(x), u)$ are liftings in $E'$ of the mapping $u\mapsto (b, u)$ of T into $B\times T$. They coincide at $t$. Since the space T is connected, they are equal. Thus, $\widetilde{k}$ is the $(B\times T)$-morphism $k'\times$ Id$_T: F\times T\rightarrow F'\times T$.

#### Corollary 3 {#ta-i-s6-prop-8-cor-3 .statement tag=01SG}

Let B and $B'$ be topological spaces, let T be a simply connected and locally connected topological space. Let $f: B'\times T\rightarrow B$ be a continuous mapping and let E be a covering of B. Given a point $t$ of T and a continuous lifting $g_t: B'\times \{t\} \rightarrow E$ of $f|B'\times  \{t\}$ to E, there exists a unique continuous lifting $g$ of $f$ to E extending $g_t$.

In view of prop. 3 of I, p. 9, it is a matter of proving that every continuous section of $f^*(E)$ over $B'\times  \{t\}$ extends uniquely to a continuous section of $f^*(E)$. Now this follows from cor. 2 applied to the coverings $(B'\times T$, Id$_{B'\times T})$ and $f^*E$ of $B'\times T$.

#### Remark {#ta-i-s6-n4-rem-1 .statement tag=01SH}

Let us retain the hypotheses and notations of proposition 8. Let G be a discrete topological group. Suppose that E is a principal covering of group G. If the coverings $E_t$ of B and $E_t\times T$ of $B\times T$ are endowed with the structures of principal coverings of group G deduced from that of E (I, p. 92, examples 1 and 4), then the coverings E and $E_t\times T$ are isomorphic principal coverings. Let in fact $h: E_t\times T\rightarrow E$ be the unique $(B\times T)$-morphism such that $h(x, t) =x$ for every $x\in E_t$. For every element $g$ of G, the mapping $(x, u)\mapsto h(x\cdot g, u)\cdot g^{-1}$ is a $(B\times T)$-morphism which maps $(x, t)$ to $x$ for every $x\in E_t$, hence is equal to $h$. This proves that $h$ is a $(B\times T)$-morphism of principal coverings.

In particular, under the preceding hypotheses, the principal coverings $E_t$ and $E_{t'}$ are isomorphic, for $t'\in T$. One proves analogously that if, in corollary 2, E and $E'$ are principal coverings of group G and if $k$ is a B-isomorphism of principal coverings of group G$,\widetilde{k}$ is a $(B\times T)$-isomorphism of principal coverings.

#### Proposition 9 {#ta-i-s6-prop-9 .statement tag=01SI}

Let B be a topological space and let $(E, p)$ be a covering of B. Let T be a simply connected, locally connected and locally compact topological space. Let us denote by $\widetilde{p}:\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)$ the mapping $g\mapsto p\circ g$. Let $t$ be a point of T. Let us denote by $e_E:\mathscr{C}_c(T; E)\rightarrow E$ the mapping which to $g\in \mathscr{C}_c(T; E)$ associates $g(t)$, and by $e_B:\mathscr{C}_c(T; B)\rightarrow B$ the mapping which to $f\in \mathscr{C}_c(T; B)$ associates $f(t)$.

The square

$\mathscr{C}_c(T; E)^{e_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(T; B)^{e_B}$ B is cartesian.

Let us first prove a lemma.

#### Lemma {#ta-i-s6-n4-lem-1 .statement tag=01SJ}

Let X, Y, Z be topological spaces and let $g: Y\rightarrow Z$ be a continuous mapping.

a) The mapping $f\mapsto g\circ f$ of $\mathscr{C}_c(X; Y)$ into $\mathscr{C}_c(X; Z)$ is continuous.

b) If the topological space Z is separated, the mapping $h\mapsto h\circ g$ of $\mathscr{C}_c(Z; X)$ into $\mathscr{C}_c(Y; X)$ is continuous.

Given a compact subset K of X, an open subset U of Z and a continuous mapping $f$ of X into Y, in order that one have $(g\circ f)(K)\subset U$, it is necessary and sufficient that one have $f(K)\subset \overset{-1}{g}(U)$. The first assertion therefore follows from the definition of the topology of compact convergence (TG, X, p. 26, def. 1).

Analogously, let K be a compact subset of Y and U an open subset of X. Since Z is supposed separated, the set $g(K)$ is compact (TG, I, p. 63, cor. 1). If $h$ is a mapping of Z into X, the condition $(h\circ g)(K)\subset U$ is nothing other than the condition $h(g(K))\subset U$, whence the second assertion.

Let us now prove proposition 9. By the lemma, the mapping $\widetilde{p}$ is continuous; by remark 1 of TG, X, p. 27, the mappings $e_E$ and $e_B$ are continuous. For every mapping $g\in \mathscr{C}_c(T; E)$, one has

$$
(p\circ e_E)(g) =p(g(t)) = (p\circ g)(t) =\widetilde{p}(g)(t) = (e_B\circ \widetilde{p})(g)
$$

so that the square diagram of the proposition is commutative.

Let $\varphi :\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)\times_BE$ be the continuous mapping defined by $\varphi (g) = (p\circ g, g(t))$ for every $g\in \mathscr{C}_c(T; E)$. By proposition 3 of I, p. 125, it is bijective. In fact, for every pair $(f, x)\in \mathscr{C}_c(T; B)\times_BE,\varphi^{-1}(f, x)$ is the unique continuous lifting $g$ of $f$ to E such that $g(t) =x$. Since the space T is locally compact, the mapping $\psi : (\mathscr{C}_c(T; B)\times_BE)\times T\rightarrow B$ defined by $\psi ((f, x), u) =f(u)$ is continuous (TG, X, p. 28, cor. 1). By corollary 3 above, the mapping $\psi$ has a unique continuous lifting $\theta : (\mathscr{C}_c(T; B)\times_B$ $E)\times T\rightarrow E$ such that $\theta ((f, x), t) =x$ for $(f, x)\in \mathscr{C}_c(T; B)\times_BE$. Thus $\theta ((f, x), u) =\varphi^{-1}(f, x)(u)$ for $(f, x)\in \mathscr{C}_c(T; B)\times_BE$ and $u\in T$. By theorem 3 of TG, X, p. 28, the mapping $(f, x)\mapsto \theta ((f, x),\cdot )$ of $\mathscr{C}_c(T; B)\times_BE$ into $\mathscr{C}_c(T; E)$ is continuous, that is to say $\varphi^{-1}$ is continuous.

Thus, the mapping $\varphi$ is a homeomorphism of $\mathscr{C}_c(T; E)$ onto the fibred product $\mathscr{C}_c(T; B)\times_BE$, whence the proposition (I, p. 8, prop. 2).

### 5. Groups of homeomorphisms of simply connected spaces

Let X be a nonempty connected topological space and let G be a discrete group acting continuously on the left in X; let $e$ denote the identity element of G. Let M be a subset of X such that $G\cdot M = X$. Put

$$
S =\{g\in G|g\cdot M\cap M=\not\emptyset \}
$$

Then $e\in S$ and $S = S^{-1}$.

For every $x\in X$, let $E_x$ denote the set of $g\in G$ such that $x\in g\cdot M$. Let $g, h\in E_x$; then $g\cdot M\cap h\cdot M=\not\emptyset$, so that $g^{-1}h\in S$. In particular, for every $x\in M$, one has $e\in E_x$ whence $E_x\subset S$.

We make one of the following two assumptions:

(i) The set M is open;

(ii) The set M is closed and the covering $(g\cdot M)_{g\in G}$ of X is locally finite.

#### Lemma 2 {#ta-i-s6-lem-2 .statement tag=01SK}

For every point $x\in X$, the mapping $\mu_x: E_x\times M\rightarrow X$ given by $(g, u)\mapsto g\cdot u$ is universally strict, and its image $E_x\cdot M$ is a neighbourhood of $x$ in X. In particular, $S\cdot M$ is a neighbourhood of M.

Under assumption (i), the mapping $\mu_x$ is open, since $E_x\times M$ is open in $G\times M$. Its image is therefore open in X.

Now suppose that assumption (ii) is satisfied. The mapping $\mu_x$ is proper (TG, I, p. 6, prop. 4, and p. 75, th. 1), hence universally strict (I, p. 20, corollary 11). Moreover, $(G-E_x)\cdot M$ is a closed subset of X which does not contain $x$, so that $E_x\cdot M$ is a neighbourhood of $x$.

The last assertion results from the fact that $E_x\subset S$ if $x\in M$.

#### Lemma 3 {#ta-i-s6-lem-3 .statement tag=01SL}

The group G is generated by S.

Let H be the subgroup of G generated by S. Let $U = H\cdot M$; observe that U is the union of the subsets of the form $h\cdot (S\cdot M)$, for $h\in H$. Since $S\cdot M$ is a neighbourhood of M (lemma 2), the set U is a neighbourhood of $H\cdot M = U$; it follows that U is open in X. Let $g, g'\in G$ be such that $g\cdot U\cap g'\cdot U=\not\emptyset$; let $h, h'\in H$ and $x, x'\in M$ be such that $gh\cdot x=g'h'\cdot x'$; then $h^{-1}g^{-1}g'h'\cdot x'=x$, so that $h^{-1}g^{-1}g'h'\in S$; in particular, $g^{-1}g'\in H$. When $g$ runs through a system of representatives of the left classes modulo H, the sets $g\cdot U$ are thus pairwise disjoint; since $G\cdot M = X$, they cover X. As X is connected, it follows that (G : H) = 1, whence H = G.

Let T be the set of pairs $(s, t)$ of elements of G such that $M\cap s\cdot$ $M\cap st\cdot M=\not\emptyset$; if $(s, t)\in T$, then $s,t$ and $st$ belong to S. Let F be the group $F(S,\mathbf{r})$ defined by the generating set S and by the set $\mathbf{r}$ of relators $str^{-1}$ for $r, s, t\in S$ such that $(s, t)\in T$ and $r=st$; let us denote by $\varepsilon$ its identity element and by $\varphi : F\rightarrow G$ the canonical homomorphism (A, I, p. 86, prop. 9). If $s\in S$, we shall denote by $x_s$ the element of F, image of $s$ under the canonical mapping of S into F; for every $s\in S$, one has $\varphi (x_s) =s$. The homomorphism $\varphi$ is therefore surjective (lemma 3). For $(s, t)\in T$ and $r=st$, one has $x_r=x_sx_t$; hence $x_e=\varepsilon$, since $(e, e)\in T$; for every $s\in S$, one has also $x_{s^{-1}}=x^{-1}_s$ since $(s, s^{-1})\in T$.

Endow the set F with the discrete topology and let Z denote the topological space $F\times M$, endowed with the operation of F given by $(\gamma ,(g, x))\mapsto$ $(\gamma g, x)$, for $\gamma$ and $g\in$ F and $u\in$ M. Let $(g_1, u_1)$ and $(g_2, u_2)$ be elements of Z; we shall say that $(g_1, u_1)$ is congruent to $(g_2, u_2)$ if there exists $s\in S$ such that $g_2=g_1\cdot x_s$ and $s\cdot u_2=u_1$.

#### Lemma 4 {#ta-i-s6-lem-4 .statement tag=01SM}

The relation “$(g_1, u_1)$ is congruent to $(g_2, u_2)$” is an equivalence relation in Z, compatible with the operation of F.

This relation is reflexive, for one has $x_e=\varepsilon$. Let $(g_1, u_1)$ and $(g_2, u_2)$ be elements of Z such that $(g_1, u_1)$ is congruent to $(g_2, u_2)$. Let $s\in S$ be such that $g_2=g_1x_s$ and $s\cdot u_2=u_1$; since $x_{s^{-1}}=x^{-1}_s$, one has $g_1=g_2x_{s^{-1}}$ and $u_2=s^{-1}\cdot u_1$, hence $(g_2, u_2)$ is congruent to $(g_1, u_1)$; consequently, this relation is symmetric. Let us show finally that it is transitive. Let $(g_1, u_1)$, $(g_2, u_2)$ and $(g_3, u_3)$ be points of Z such that $(g_1, u_1)$ and $(g_2, u_2)$ are congruent, and also $(g_2, u_2)$ and $(g_3, u_3)$. Let $s$ and $t$ in S be such that $g_2=g_1x_s$ and $s\cdot u_2=u_1$ on the one hand, and $g_3=g_2x_t$ and $t\cdot u_3=u_2$ on the other hand. One has $u_1=s\cdot u_2=st\cdot u_3$, hence $u_1\in M\cap s\cdot M\cap st\cdot M$, which shows that $(s, t)$ belongs to T and that $st$ belongs to S. One then has $g_3=g_2x_t=g_1x_sx_t=g_1x_{st}$ and $u_1=st\cdot u_3$; consequently, $(g_1, u_1)$ and $(g_3, u_3)$ are congruent. Thus, the relation "to be congruent" is an equivalence relation in Z. It is compatible with the operation of F in Z.

Let Y be the quotient topological space of Z for the equivalence relation defined above. Let us denote by $\pi : Z\rightarrow Y$ the canonical mapping. Let us also denote by $q: Z\rightarrow X$ the mapping given by $(g, x)\mapsto \varphi (g)\cdot x$; it is surjective (lemma 3). By passing to the quotient, the mapping $q$ induces a continuous and surjective mapping $p: Y\rightarrow X$; by lemma 4, the operation of F in Z induces a continuous operation of F in Y such that $p(g\cdot y) =\varphi (g)\cdot p(y)$ for every $g\in F$ and every $y\in Y$. In particular, the group N = Ker($\varphi$ ) operates continuously on the X-space $(Y, p)$.

#### Lemma 5 {#ta-i-s6-lem-5 .statement tag=01SN}

If M is connected, the space Y is connected.

Let $g\in F$ and $s\in S$ be given. Let $u$ and $v$ be elements of M such that $v=s\cdot u$; we have therefore $\pi (g, v) =\pi (gx_s, u)$, and the sets $\pi (\{g\} \times M)$ and $\pi (\{gx_s\} \times M)$ of Y have a common point. Since they are connected, they are contained in the same connected component of Y. Since S is a symmetric subset of the group G, and since $x_{s^{-1}}=x^{-1}_s$ for every $s\in S$, every element $g$ of F is of the form $x_{s_1}. . . x_{s_n}$, where $n\in \mathbf{N}$ and $s_1, . . . , s_n$ are elements of S. By induction on $n$, the sets $\pi (\{e\} \times M)$ and $\pi (\{g\} \times M)$ are contained in the same connected component of Y, for every $g\in F$. It follows that Y is connected.

#### Lemma 6 {#ta-i-s6-lem-6 .statement tag=01SO}

For every $x\in X$, the group N acts faithfully and transitively on the fibre $\overset{-1}{p}(x)$.

Since $p$ is surjective, the fibre $\overset{-1}{p}(x)$ is not empty. Let $y, y'\in$ $\overset{-1}{p}(x)$; let us prove that there exists a unique element $n\in$ N such that $n\cdot y=y'$. Let $g, h\in$ F and let $u, v\in$ M be such that $y=\pi (g, u)$ and $y'=\pi (h, v)$. Put $s=\varphi (g^{-1}h)$. Since $x=\varphi (g)\cdot u=\varphi (h)\cdot v$, we have $u=s\cdot v$, whence $s\in S$. It follows that $\varphi (h) =\varphi (gx_s)$, so that there exists $n\in N$ such that $h=ngx_s$. Then,

$$
y'=\pi (h, v) =\pi (ngx_s, v) =n\cdot \pi (gx_s, v) =n\cdot \pi (g, s\cdot v) =n\cdot y
$$

Let $n'$ be an element of N such that $n'\cdot y=y'$. We have $n'\cdot \pi (g, u) =n\cdot \pi (g, u)$, whence $\pi (n'g, u) =\pi (ng, u)$. Consequently, there exists $t\in S$ such that $n'g=$ $ngx_t$; this relation implies that $\varphi (x_t) =e$, whence $t=e$ and $n=n'$.

#### Lemma 7 {#ta-i-s6-lem-7 .statement tag=01SP}

Endowed with the action of N, the X-space $(Y, p)$ is a principal left covering. It is trivializable over M.

Let $x\in X$; fix an element $g\in E_x$ and an element $\overline{g}\in F$ such that $\varphi (\overline{g}) =g$. We denote by $\mu_x: E_x\times M\rightarrow X$ the mapping given by $(h, u)\mapsto h\cdot u$.

Let $n\in N$, let $h, k\in E_x$ and let $u, v\in M$ be such that $h\cdot u=k\cdot v$; put $s=g^{-1}h,t=h^{-1}k$ and $r=st=g^{-1}k$. Since $x$ belongs to $g\cdot M\cap h\cdot M\cap k\cdot M$, the pair $(s, t)$ belongs to T, whence $x_sx_t=x_r$. Hence

$$
\pi (ngx_r, v) =\pi (ngx_sx_t, v) =\pi (ngx_s, t\cdot v) =\pi (ngx_s, u)
$$

There thus exists a unique mapping $\theta : N\times (E_x\cdot M)\rightarrow Y$ such that $\theta (n, h\cdot u) =\pi (ngx_{g^{-1}h}, u)$ for every $n\in N$, every $h\in E_x$ and every $u\in M$. We have

$$
p(\theta (n, h\cdot u)) =p(\pi (ngx_s, u)) =q(ngx_s, u) =\varphi (ngx_s)\cdot u=gs\cdot u=h\cdot u
$$

Moreover, for $n, n'\in N$ and $y\in E_x\cdot M$, one has $\theta (n'n, y) =n'\cdot \theta (n, y)$. The mapping $\theta ': N\times (E_x\times M)\rightarrow Y$ defined by $\theta '(n,(h, u)) =\theta (n, \mu_x(h, u))$ is continuous; since the mapping $\mu_x$ is universally strict (I, p. 133, Lemma 2), the mapping $\theta$ is continuous. It is a bijection of $N\times (E_x\cdot M)$ onto the subspace $Y\times_X(E_x\cdot M)$ of Y (Lemma 6).

Let $z= (k, v)\in Z$ and $(h, u)\in E_x\times M$ be such that $q(k, v) =\mu_x(h, u)$. Put $s$ = $h^{-1}\varphi (\overline{k})$; since $\varphi (\overline{k})\cdot v$ = $h\cdot u$, one has $s\in$ S. Then put $\lambda '(z,(h, u)) =kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}$; one has $\varphi (\lambda '(z,(h, u))) =$ $\varphi (\overline{k})s^{-1}h^{-1}gg^{-1}$ = $e$, hence $\lambda '(z,(h, u))\in$ N. Thus a continuous mapping $\lambda ': Z\times_X(E_x\times M)\rightarrow N$ is defined. Moreover, for every $z$ and $(h, u)$ as above, one has

$$
\theta (\lambda '(z,(h, u)), h\cdot u) =\pi (kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}gx_{g^{-1}h}, u)
$$

$$
=\pi (kx^{-1}_s, u) =\pi (k, s^{-1}\cdot u) =\pi (k, v) =\pi (z)
$$

and $\lambda '(z,(h, u))$ is the unique element $n$ of N such that $\theta (n, h\cdot u) =\pi (z)$. In particular there exists a unique mapping

$$
\lambda : Y\times_X(E_x\cdot M)\rightarrow N
$$

such that $\lambda (\pi (z), h\cdot u) =\lambda '(z,(h, u))$ for every $z\in Z$ and every $(h, u)\in$ $E_x\times M$ such that $q(z) =h\cdot u$. It is continuous, since the mapping $\mu_x$ is universally strict. It follows that the $E_x\cdot M$-space $Y_{E_x\cdot M}$ deduced from Y by base change, endowed with the operation of N, is a principal fibre space with group N, trivializable.

The lemma is thus proved.

#### Proposition 10 {#ta-i-s6-prop-10 .statement tag=01SQ}

Let X be a nonempty connected topological space, let G be a discrete group operating continuously on the left in X, and let M be a subset of X such that $G\cdot M = X$. One of the two following hypotheses is made:

(i) The set M is open;

(ii) The set M is closed and the covering $(g\cdot M)_{g\in G}$ of X is locally finite.

Let S be the set of elements $g\in G$ such that $M\cap g\cdot M=\not\emptyset$, let T be the set of pairs $(s, t)\in S\times S$ such that $M\cap s\cdot M\cap st\cdot M=\not\emptyset$. Let F be the group $F(S,\mathbf{r})$ defined by the generator set S and by the set $\mathbf{r}$ of relators $str^{-1}$ for $r, s, t\in$ S such that $(s, t)\in$ T and $r$ = $st$; for $s\in S$, let $x_s$ denote the image of $s$ under the canonical mapping of S into F. There exists a unique group homomorphism $\varphi : F\rightarrow G$ such that $\varphi (x_s) =s$ for every $s\in S$. It is surjective; it is an isomorphism if the space X is simply connected, or, more generally, if every covering of X which is trivializable over M is trivializable.

The homomorphism $\varphi$ is surjective (I, p. 133, lemma 3). With the notation of this No.$^o$, the covering Y of X is trivializable, since it is trivializable over M. By lemma 5, Y is connected. Consequently, $p: Y\rightarrow X$ is a homeomorphism and the group N is reduced to the identity element. Consequently, the homomorphism $\varphi : F\rightarrow G$ is a group isomorphism.

#### Proposition 11 {#ta-i-s6-prop-11 .statement tag=01SR}

Let X be a simply connected topological space and G a discrete group operating continuously on the right in X. If the subgroup of G generated by the union of the stabilizers of the points of X is equal to G, the space $X/G$ is simply connected.

Let $(E, p)$ be a covering of $X/G$. We have to prove that, for every point $x$ of E, there exists a continuous section $s$ of $p$ such that $s\circ p(x) =x($I, p. 70, cor. 2 of prop. 1). Let $q: X\rightarrow X/G$ denote the canonical mapping and choose a point $y$ of X such that $q(y) =p(x)$. Since the space X is simply connected, there exists a continuous mapping $f: X\rightarrow E$ such that $f(y) =x$ and $p\circ f=q($I, p. 125, prop. 3). Let $z$ be a point of X and $g$ an element of the subgroup of G stabilizing $z$. The mappings $t\mapsto f(t)$ and $t\mapsto f(t\cdot g)$ of X into E are continuous liftings to E of the mapping $q$ which coincide for $t=z$. Since the space X is connected, they are equal (I, p. 34, cor. 1 of prop. 11). Since the union of the stabilizer subgroups of the points of X generates G, one has $f(t\cdot g) =f(t)$ for every $t\in X$ and every $g\in G$. Passing to the quotient, one deduces from $f$ a continuous mapping $s: X/G\rightarrow E$ which is a continuous section of $p$ such that $s(p(x)) =x$.

## EXERCISES {#ta-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
