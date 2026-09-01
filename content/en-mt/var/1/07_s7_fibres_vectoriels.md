---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 7
section_title: Fibrés vectoriels
lang: en
source: var-fr
pdf_pages: 0068-0085
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fibrés vectoriels
      page: 0
      pdf_page: 68
    - "no": 2
      title: Morphismes de fibrés vectoriels
      page: 0
      pdf_page: 69
    - "no": 3
      title: Morphismes multilinéaires
      page: 0
      pdf_page: 71
    - "no": 4
      title: Sections
      page: 0
      pdf_page: 72
    - "no": 5
      title: Sous-fibrés vectoriels, fibrés vectoriels quotients, suites exactes
      page: 0
      pdf_page: 74
    - "no": 6
      title: Foncteurs vectoriels
      page: 0
      pdf_page: 76
    - "no": 7
      title: Sommes directes, fibrés d’applications multilinéaires, dual
      page: 0
      pdf_page: 78
    - "no": 8
      title: Fibrés d’applications multilinéaires alternées
      page: 0
      pdf_page: 79
    - "no": 9
      title: Produits tensoriels, espaces tensoriels, algèbre extérieure
      page: 0
      pdf_page: 81
    - "no": 10
      title: Fibrés vectoriels et fibrés principaux
      page: 0
      pdf_page: 83
    - "no": 11
      title: Changement de structure
      page: 0
      pdf_page: 85
statements: 0
exercises: 0
content_sha256: 3ea89201f780c796ce69c1f3f443fb7823d3576700c6b7dc188afb4fa20c7b4c
translated_from: content/fr/var/1/07_s7_fibres_vectoriels.md
source_lang: fr
translation_method: machine
source_content_sha256: fe137a4e6ae9d21a89fb2166378f27a2362444957d7ddf2dad763fead7f89cf4
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-13b5f93c
glossary_version: 34
glossary_terms_sha256: 49ff4558a10e2221e5afd2d1ce3e8d8298435e8916b2eaaa7f5ffbf0cec2c50a
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 7. Vector bundles

Throughout this paragraph, the letter B denotes a manifold of class $C^r$ ($r \geqslant 1$) and the letter M denotes a set endowed with a mapping $\pi$ from M into B. We say that B is the base of M and for every $b \in B$, we denote by $M_b$ and call the fiber of M at $b$ the subset $\pi^{-1}(b)$ of M.

### 7.1. Definition of vector bundles

7.1.1. A vector chart of M is a triple $t = (U, \varphi, F)$, where U is an open set of B, where F is a Banach space and $\varphi$ a bijection of $\pi^{-1}(U)$ onto $U \times F$ such that $\pi(\varphi^{-1}(b, h)) = b$ for all $b \in B$ and all $h \in F$. We say that U is the domain of the vector chart t and that t is a vector chart of M at $b \in B$ if $b \in U$. For every $b \in U$, we denote by $t_b$ the bijection of F onto $M_b$ defined by $t_b(h) = \varphi^{-1}(b, h)$ for $h \in F$.

7.1.2. We say that two vector charts $t = (U, \varphi, F)$ and $t' = (U', \varphi', F')$ of M are $C^r$-compatible (or simply compatible) if there exists a mapping $\lambda$ of class $C^r$ of the manifold $U \cap U'$ into the Banach space $\mathcal{L}(F; F')$ such that:

$$
t_b = t'_b \circ \lambda(b) \quad \text{for all } b \in U \cap U'.
$$

7.1.3. We say that a set of vector charts of M is a $C^r$-vector atlas (or simply vector atlas) of M if it consists of vector charts which are pairwise $C^r$-compatible and whose domains have B as their union. We say that two vector atlases $\mathcal{A}$ and $\mathcal{B}$ of M are $C^r$-equivalent (or equivalent) if $\mathcal{A} \cup \mathcal{B}$ is again a vector atlas of M. This relation is an equivalence relation.

7.1.4. A structure of vector bundle of class $C^r$ (with base B) on M is the data of an equivalence class of vector atlases (Ens., Chap. II, § 6, No. 9). A vector chart belonging to a vector atlas of this class is called a vector chart of the vector bundle M.

Let M be a vector bundle with base B. For every $b \in B$, there exists on the fiber $M_b$ one and only one Banach space structure such that, for every vector chart $t = (U, \varphi, F)$ of the vector bundle M at $b$, the mapping $t_b$ is an isomorphism of F onto $M_b$.

Let $c = (U, \psi, E)$ be a chart of the manifold B and let $t = (U, \varphi, F)$ be a vector chart of the vector bundle M, with the same domain U. For $x \in \pi^{-1}(U)$, put:

$$
\alpha(x) = (\psi(\pi(x)), t_{\pi(x)}^{-1}(x)).
$$

Then the triple $(\pi^{-1}(U), \alpha, E \times F)$ is a chart of the set $M$. There exists on $M$ one and only one manifold structure of class $C'$ (said to be underlying $M$) for which all the charts thus obtained are charts of the manifold $M$. The triple $(M, B, \pi)$ is then a fibration (6.1.1).

7.1.5. Let $F$ be a Banach space. Put $M = B \times F$, the mapping being the first projection. There exists on $M$ a vector bundle structure (with basis $B$) and only one for which $(B, \mathrm{Id}_M, F)$ is a vector chart. One says that $B \times F$ endowed with this structure is the trivial vector bundle with basis $B$ and fibre $F$ and one sometimes denotes it by $F_B$. The manifold structure of $F_B$ is the product manifold structure and for every $b \in B$, the mapping $h \mapsto (b, h)$ is an isomorphism of Banach spaces of $F$ onto the fibre of $F_B$ at the point $b \in B$. One often denotes by $0$ a trivial vector bundle whose fibre is reduced to $0$.

7.1.6. Let $M$ be a vector bundle with basis $B$. For $b \in B$, one calls rank of $M$ at $b$ and denotes by $\mathrm{rg}_b(M)$, the dimension (finite or $+\infty$) of the Banach space $M_b$. One has $\dim_x M = \dim_b B + \mathrm{rg}_b M$ for $b = \pi(x)$. The function $b \mapsto \mathrm{rg}_b M$ is locally constant. One says that $M$ is of finite rank if $\mathrm{rg}_b M < +\infty$ for every $b \in B$.

### 7.2. Morphisms of vector bundles

7.2.1. Let $B$ and $B'$ be two manifolds and let $f$ be a morphism from $B$ into $B'$. Let $M$ be a vector bundle with basis $B$ and $M'$ a vector bundle with basis $B'$. One says that a mapping $g$ from $M$ into $M'$ is an $f$-morphism of vector bundles if the following condition is satisfied:

For every point $b_0 \in B$, there exists a vector chart $t = (U, \varphi, F)$ of $M$ at $b_0$, a vector chart $t' = (U', \varphi', F')$ of $M'$ at $f(b_0)$ and a mapping $\lambda$ of class $C'$ from $U$ into $\mathcal{L}(F; F')$ such that $f(U) \subset U'$ and that $g_b \circ t_b = t'_{f(b)} \circ \lambda(b)$ for every $b \in U$, where $g_b$ is the restriction of $g$ to $M_b$.

Under these hypotheses, $g$ is a morphism of varieties and, for every $b \in B$, $g$ induces a continuous linear mapping of $M_b$ into $M'_{f(b)}$. The vector rank of $g$ at $b \in B$ is called and is denoted by $\mathrm{rg}_b(g)$ the rank (finite or $+\infty$) of the linear mapping $g_b$.

Conversely, if $r \geqslant \infty$ or if $M$ is of finite rank, an $f$-morphism of fibrations of $(M, B, \pi)$ into $(M', B', \pi')$ which induces on each fibre $M_b$ a linear mapping of $M_b$ into $M'_{f(b)}$ (for every $b \in B$), is an $f$-morphism of vector bundles.

7.2.2. Let in addition $f'$ be a morphism of $B'$ into a variety $B''$. If $g$ is an $f$-morphism of $M$ into $M'$, and if $g'$ is an $f'$-morphism of $M'$ into a vector bundle $M''$ with base $B''$, the mapping $g' \circ g$ is an $(f' \circ f)$-morphism of $M$ into $M''$. We have $(g' \circ g)_b = g'_{f(b)} \circ g_b$ for every $b$ in $B$.

7.2.3. Let M and M' be two vector bundles with the same base B. A B-morphism, or simply a morphism of M into M', is called every Id_B-morphism. The composite of two morphisms is a morphism.

Let g be a morphism of vector bundles of M into M'; if g is bijective, it is an isomorphism of the variety M onto the variety M', the reciprocal mapping $g^{-1}$ is a morphism of vector bundles of M' into M and we have $(g^{-1})_b = g_b^{-1}$ for every b in B. The mapping g is then an isomorphism of vector bundles.

7.2.4. Let f be a morphism of a variety B' into B and let M be a vector bundle with base B. Put $M' = B' \times_B M$ and denote by $\pi'$ (resp. g) the restriction to M' of the projection of $B' \times M$ onto B' (resp. M). There exists on M' one and only one structure of vector bundle with base B' (relative to $\pi'$) for which g is a f-morphism. We say that M' is the vector bundle with base B' inverse image of M by f and denote it by $f^*M$; the f-morphism g is called the canonical f-morphism of $f^*M$ into M.

The structure of variety of $f^*M$ is that of the fiber product of the varieties B' and M over B (5.11.2); for every $b \in B'$, the mapping $x \mapsto (b, x)$ is an isomorphism of Banach spaces of $M_{f(b)}$ onto $(f^*M)_b$.

The formation of inverse images of vector bundles is transitive.

Let N' be a vector bundle with base B' and let h be a f-morphism of N' into M. There exists one and only one B'-morphism $\tilde{h}$ of N' into $f^*M$ such that $h = g \circ \tilde{h}$.

Let N be a vector bundle with base B and v a B-morphism of N into M. There exists one and only one B'-morphism, denoted by $f^*v$, of $f^*N$ into $f^*M$ such that the diagram

$$
\begin{array}{ccc}
f^*N & \xrightarrow{f^*v} & f^*M \\
\downarrow & & \downarrow \\
N & \xrightarrow{v} & M
\end{array}
$$

is commutative.

7.2.5. Let B' be a subvariety of B and let i be the canonical injection of B' into B. If M is a vector bundle with base B, the inverse image $i^*M$ is called the vector bundle induced on B' by M and is denoted by $M|B'$. If $t = (U, \varphi, F)$ is a vector chart of M, then $(U \cap B', \varphi|\pi^{-1}(U \cap B'), F)$ is a vector chart of $M|B'$. The canonical f-morphism of $M|B'$ into M is an isomorphism of varieties of $M|B'$ onto the subvariety $\pi^{-1}(B')$ of M.

7.2.6. Let f be a morphism of a variety B' into B and let M (resp. M') be a vector bundle with base B (resp. B'). A f-comorphism of M into M' is called a B'-morphism of $f^*M$ into M'. When B = B' and $f = \mathrm{Id}_B$, the data of a $f$-comorphism of $M$ into $M'$ is equivalent to the data of a $B$-morphism of $M$ into $M'$.

Let $g$ be a $f$-comorphism of $M$ into $M'$. For every $b \in B'$, the mapping $g_b : x \mapsto g(b, x)$ of $M_{f(b)}$ into $M'_b$ is a continuous linear mapping.

Suppose moreover that $f'$ is a morphism of a variety $B''$ into $B'$ and that $h$ is a $f'$-comorphism of $M'$ into a vector bundle $M''$ with base $B''$. The mapping $h \circ f^*g$ of ${f'}^*(f^*M) = (f \circ f')^*M$ into $M''$ is then a $(f \circ f')$-comorphism of $M$ into $M''$, denoted by $h \circ g$. For $b \in B''$, one has

$$
(h \circ g)_b = h_b \circ g_{f'(b)}.
$$

### 7.3. Multilinear morphisms

7.3.1. Let $M_1, \ldots, M_d$ and $N$ be vector bundles with base $B$, and let $u$ be a mapping of the set $M_1 \times_B \cdots \times_B M_d$ into $N$. We say that $u$ is a *multilinear morphism* (or $d$-linear) if the following condition is satisfied:

*For every $b_0 \in B$, there exist an open neighbourhood $U$ of $b_0$ in $B$, vector bundle charts $t^j = (U, \varphi^j, F^j)$ of $M_j$ (for $1 \leq j \leq d$) and $t = (U, \varphi, F)$ of $N$, and a mapping $\lambda$ of class $C^r$ from $U$ into the Banach space $\mathcal{L}(F^1, \ldots, F^d; F)$ of continuous $d$-linear mappings from $F^1 \times \cdots \times F^d$ into $F$, such that*:

$$
(t_b \circ \lambda(b))(x_1, \ldots, x_d) = u(t_b^1(x_1), \ldots, t_b^d(x_d))
$$

*for every $b \in U$ and all $x_j \in F^j$*.

Every multilinear morphism $u$ is a morphism of manifolds from the fibre product $M_1 \times_B \cdots \times_B M_d$ into $N$ and induces for every $b \in B$ a continuous $d$-linear mapping $u_b$ from $(M_1)_b \times \cdots \times (M_d)_b$ into $N_b$.

If $f$ is a morphism from $B$ into a manifold $B'$, a multilinear morphism from $M_1 \times_B \cdots \times_B M_d$ into a vector bundle $M'$ with base $B'$ is by definition the composite of a multilinear morphism from $M_1 \times_B \cdots \times_B M_d$ into $f^*M'$ with the canonical $f$-morphism of $f^*M'$ into $M'$.

A bilinear morphism is also called a *pairing*. For $d = 1$, a linear morphism is a morphism in the sense of 7.2.1. For $d = 0$, a 0-linear morphism is identified with a *section* of $N$ (7.4).

7.3.2. A *bundle of algebras* of base $B$ is called a vector bundle $A$ of base $B$, endowed with a pairing of $A \times_B A$ into $A$. Each fibre $A_b$ is then endowed with a structure of $K$-algebra. If, for every $b \in B$, the algebra $A_b$ has a unit element, denoted by $e_b$, the mapping $b \mapsto e_b$ is a section of $A$ (cf. 7.4). A bundle of algebras $A$ is said to be *locally trivial* if, for every point $b_0$ of $B$, there exists a vector chart $t = (U, \varphi, E)$ of $A$ at the point $b_0$ and a structure of $K$-algebra on $E$ such that $t_b$ is an isomorphism of algebras of $E$ onto $A_b$ for every $b \in U$.

7.3.3. Let $A$ be a bundle of associative algebras with unit element of base $B$. A *bundle of A-modules* of base $B$ is called a vector bundle $M$ of base $B$ endowed with a pairing $m : A \times_B M \to M$ such that the mapping $m_b : A_b \times M_b \to M_b$ defines, for every $b \in B$, a structure of $A_b$-module on the fibre $M_b$.

Let $M$ and $M'$ be two bundles of $A$-modules. An *A-homomorphism* of $M$ into $M'$ is called any morphism $g : M \to M'$ of vector bundles of base $B$ which induces for every $b$ in $B$ an $A_b$-linear mapping of $M_b$ into $M'_b$.

Suppose $A$ is locally trivial. A fibré $M$ in $A$-modules is said to be *locally trivial* if, for every point $b_0$ of $B$, there exists a vector chart $t = (U, \varphi, E)$ of $A$ at $b_0$ as in 7.3.2, a vector chart $t' = (U, \varphi', L)$ of $M$ at $b_0$, and a module structure of $E$ on $L$ such that, for every $b \in U$, $t'_b$ is a $t_b$-isomorphism of the $A_b$-module $M_b$ onto the $E$-module $L$.

7.3.4. Let $A$ be a Banach algebra over $K$ (for example a field endowed with a finite-dimensional $K$-algebra structure). The trivial fibré $A_B$ is then a fibré in algebras, locally trivial. A locally trivial fibré in $A_B$-modules $M$ is also called a vector fibré over $A$ (with base $B$). The fibres $M_b$ are then topological $A$-modules. An $f$-morphism $u$ of $M$ into another vector fibré over $A$ is said to be $A$-linear if the mappings $u_b$ are $A$-linear for every $b \in B$.

### 7.4. Sections

7.4.1. Let $M$ be a vector fibré with base $B$. For every open $U$ of $B$, we denote by $\mathscr{S}_M^r(U)$ the set of sections of class $C^r$ of $M$ over $U$, that is to say, morphisms $s$ of class $C^r$ from $U$ into $M$ such that $s(b) \in M_b$ for every $b \in U$. This set is endowed with a module structure over the ring $\mathscr{C}^r(U)$ of morphic functions by the rules:

(1)
$$
(s + s')(b) = s(b) + s'(b)
$$
(2)
$$
(\varphi \cdot s)(b) = \varphi(b) \cdot s(b)
$$
for $s, s'$ in $\mathscr{S}_M^r(U)$ and $\varphi$ in $\mathscr{C}^r(U)$. When the open set $U$ varies, one obtains a sheaf $\mathscr{S}_M^r$ of mappings from $B$ into $M$ (cf. No. 5.4.1), called the *sheaf of sections* of $M$.

7.4.2. Let $M_1, \ldots, M_d$ and $N$ be vector bundles with base $M$ and let $u$ be a multilinear morphism from $M_1 \times_B \ldots \times_B M_d$ into $N$. For $1 \leq j \leq d$, let us give ourselves a section $s_j$ of $M_j$ over an open set $U$ of $B$; one defines a section $u(s_1, \ldots, s_d)$ of $N$ over $U$ by the formula:
$$
u(s_1, \ldots, s_d)(b) = u_b(s_1(b), \ldots, s_d(b)) \quad \text{for } b \in U.
$$

The mapping $(s_1, \ldots, s_d) \mapsto u(s_1, \ldots, s_d)$ is $\mathcal{C}^r(U)$-multilinear. It is sometimes denoted $\mathscr{S}(u)$.

7.4.3. Let $f$ be a morphism of a manifold $B'$ into $B$ and let $M$ be a vector bundle with base $B$. For every open set $U$ of $B$ and every $s \in \mathscr{S}_M^r(U)$, the mapping $x \mapsto (x, s(f(x)))$ is a section of class $C^r$ of $f^*M$ over the open set $f^{-1}(U)$, denoted $f^*s$ and called the inverse image of $s$ by $f$. The mapping $s \mapsto f^*s$ from $\mathscr{S}_M^r(U)$ into $\mathscr{S}_{f^*M}(f^{-1}(U))$ is semilinear with respect to the homomorphism $g \mapsto g \circ (f|f^{-1}(U))$ of $\mathcal{C}^r(U)$ into $\mathcal{C}^r(f^{-1}(U))$.

If moreover $N$ is a vector bundle with base $B'$ and $g$ an $f$-comorphism of $M$ into $N$, one sometimes denotes by $\mathscr{S}(g)$ the mapping $s \mapsto g \circ f^*s$ from $\mathscr{S}_M^r(U)$ into $\mathscr{S}_N^r(f^{-1}(U))$.

7.4.4. Let $M$ be a vector bundle with base $B$, *of finite rank*. A *frame* of $M$ over an open subset $U$ of $B$ is called a finite sequence $(s_1, \ldots, s_n)$ of sections of $M$ over $U$ such that $(s_1(b), \ldots, s_n(b))$ is a *basis* of the vector space $M_b$ for every $b \in B$. The sequence $(s_1, \ldots, s_n)$ is then a basis of the $\mathcal{C}^r(U)$-module $\mathscr{S}_M^r(U)$. If $f$ is a morphism of a manifold $B'$ into $B$, the sections $f^*s_j$ form a frame of $f^*M$ over $f^{-1}(U)$.

7.4.5. Let $L$ be a field, endowed with a structure of $K$-algebra of finite dimension and let $(M, B, \pi)$ be a fibration. Suppose that on each fibre $M_b$ a structure of vector space over $L$, *of finite dimension*, is given. There exists then at most one structure of vector bundle over $L$ with base $B$ on $M$, compatible with the mapping $\pi$, the manifold structure of $M$ and the $L$-vector space structures on the fibres (7.3.4). For such a structure to exist, it is necessary and sufficient that the following condition be satisfied:

(FV) *For every $b_0 \in B$, there exists an open neighbourhood $U$ of $b_0$ in $B$ and an isomorphism of manifolds $\varphi$ from $\pi^{-1}(U)$ onto the product $U \times F$ of $U$ by a vector space $F$ over $L$ of finite dimension, such that for every $b \in U$, the bijection $\varphi_b$ of $M_b$ onto $F$ induced by $\varphi$ is an isomorphism of vector spaces over the field $L$.*

The triples $(U, \varphi, F)$ satisfying (FV) are then vector bundle charts of the vector bundle $M$.

The condition (FV) is equivalent to:
(FV') *For every $b_0 \in B$, there exists an integer $n$ and $n$ sections $s_1, \ldots, s_n$ of $M$ over an open neighbourhood $U$ of $b_0$ such that the mapping*
$$
(b, a_1, \ldots, a_n) \mapsto a_1 s_1(b) + \cdots + a_n s_n(b)
$$
*is an isomorphism of the manifold $U \times L^n$ onto the manifold $\pi^{-1}(U)$.*

7.4.6. Let $M_1, \ldots, M_d$ and $N$ be vector bundles with base $B$, the $M_j$ being of *finite rank*. Suppose that for every open set $U$ of $B$ a mapping $\varphi_U$ from $\mathscr{S}_{M_1}^r(U) \times \cdots \times \mathscr{S}_{M_d}^r(U)$ into $\mathscr{S}_N^r(U)$ is given, $\mathcal{C}^r(U)$-multilinear, such that for $V \subset U$ one has:

$$
\varphi_U(s_1, \ldots, s_d)|V = \varphi_V(s_1|V, \ldots, s_d|V).
$$

There then exists one and only one multilinear morphism $u$ from $M_1 \times_B \ldots \times_B M_d$ into $N$ such that $\varphi_U(s_1, \ldots, s_d) = u(s_1, \ldots, s_d)$ whatever the sections $s_j$ of $M$ on the open set $U$ of $B$.

7.4.7. Let $f$ be a morphism of a variety $B'$ into $B$ and let $M$ (resp. $M'$) be a vector bundle with base $B$ (resp. $B'$) and of finite rank. Suppose that for every open set $U$ of $B$ a mapping $\varphi_U$ from $\mathcal{S}_M^r(U)$ into $\mathcal{S}_{M'}^{r'}(f^{-1}(U)), \mathcal{C}^r(U)$-semilinear, is given, such that

$$
\varphi_U(s)|f^{-1}(V) = \varphi_V(s|V)
$$

for every open set $V \subset U$. There then exists one and only one $f$-comorphism $g$ from $M$ into $M'$ such that $\varphi_U(s) = \mathcal{S}(g)(s)$ for every $s \in \mathcal{S}_M^r(U)$.

*7.4.8. Let $\mathcal{F}$ be a sheaf of modules over the sheaf of rings $\mathcal{C}_B^r$. One says that $\mathcal{F}$ is locally free if for every $b \in B$, there exists an open neighbourhood $U$ of $b$ and an integer $n$ such that $\mathcal{F}|U$ is isomorphic (as a sheaf of $\mathcal{C}_U^r$-modules) to the sheaf $(\mathcal{C}_U^r)^n$.

If $M$ is a vector bundle of base $B$ of finite rank, the sheaf $\mathcal{S}_M^r$ is locally free. Conversely, for every locally free sheaf $\mathcal{F}$ on $B$, there exists a vector bundle $M$ and an isomorphism of sheaves from $\mathcal{S}_M^r$ onto $\mathcal{F}$. If $M'$ is another vector bundle of base $B$ of finite rank, the mapping $g \mapsto \mathcal{S}(g)$ is a bijection from the set of $B$-morphisms of $M$ into $M'$ onto the set of morphisms of sheaves of $\mathcal{C}^r$-modules from $\mathcal{S}_M^r$ into $\mathcal{S}_{M'}^{r'}$*

### 7.5. Vector subbundles, quotient vector bundles, exact sequences

In this number, a vector bundle means a vector bundle of base $B$ and a morphism of vector bundles means an $\mathrm{Id}_B$-morphism.

7.5.1. Let $M$ be a vector bundle. A subset $M'$ of $M$ is called a vector subbundle of $M$ if, for every point $b \in B$, there exists a vector chart $t = (U, \varphi, E)$ of $M$ at $b$ and a closed vector subspace $F$ of $E$ admitting a topological supplement, such that

$$
\varphi(\pi^{-1}(U) \cap M') = U \times F.
$$

Under these conditions, there exists on $M'$ one and only one structure of vector bundle for which the canonical injection of $M'$ into $M$ is a morphism. For each $b \in B$, the fibre $M'_b$ of $M'$ is the closed vector subspace $M' \cap M_b$ of $M_b$; $M'$ is a closed submanifold of $M$ and the structure of underlying manifold of the structure of vector bundle of $M'$ coincides with that induced by the manifold structure of $M$.

7.5.2. Let $M'$ be a vector subbundle of $M$. Let $R\{x, y\}$ denote the following relation between points $x, y$ of $M$:
« there exists an element $b$ of $B$ such that $x \in M_b, y \in M_b$ and $x - y \in M'_b$ ». Then $R$ is a regular equivalence relation on $M$ (cf. n° 5.9.7). On the set $M/R$, there exists one and only one structure of vector bundle such that the canonical mapping of $M$ onto $M/R$ is a morphism. We denote it by $M/M'$ and call the vector bundle thus defined the quotient of $M$ by $M'$; for each point $b$ of $B$, the bundle $(M/M')_b$ is the quotient topological vector space $M_b/M'_b$ and the manifold structure on $M/M'$ is the quotient of that of $M$.

7.5.3. Retain the hypotheses of 7.5.2. For every point $b_0$ of $B$, one can find an open neighbourhood $U$ of $b_0$, a Banach space $F$, direct sum of two closed subspaces $F'$ and $F''$, and an isomorphism of vector bundles $\iota$ from $F_U$ onto $M|U$ with the following properties:
(i) The restriction $\iota'$ of $\iota$ to $U \times F'$ is an isomorphism from $F'_U$ onto $M'|U$.
(ii) If $\rho$ is the canonical mapping of $M$ onto $M'' = M/M'$, and if $\iota''$ is the restriction of $\iota$ to $U \times F''$, the map $\rho \circ \iota''$ is an isomorphism from $F''_U$ onto $M''|U$.

7.5.4. If a morphism of vector bundles $g : L \to M$ has its image contained in $M'$, it is a morphism of vector bundles from $L$ into $M'$.
Consider now a morphism of vector bundles $h : M \to N$ and suppose that, for every $b$ in $B$, the restriction of $h_b$ to $M'_b$ is zero. If $\rho$ is the canonical morphism from $M$ onto $M/M'$, there exists one and only one morphism $\bar{h}$ from $M/M'$ into $N$ such that $h = \bar{h} \circ \rho$.

7.5.5. Let $P$ and $Q$ be two vector bundles, and let $g$ be a morphism from $P$ into $Q$; for every point $b$ of $B$, denote by $N_b$ and $I_b$ respectively the kernel and the image of the linear mapping $g_b : P_b \to Q_b$. Put $N = \bigcup_{b \in B} N_b$ and $I = \bigcup_{b \in B} I_b$. The morphism $g$ is said to be locally direct if $N$ is a vector subbundle of $P$ and $I$ a vector subbundle of $Q$. The morphism $g$ then defines by passing to the quotient an isomorphism of $P/N$ onto $I$. It is said that $N$ is the kernel of $g$ and it is denoted by $\mathrm{Ker}\,g$. Analogously, the subbundle $I$ is called the image of $g$ and is denoted by $\mathrm{Im}\,g$.
If $r \geqslant \infty$, the morphism $g$ is locally direct if and only if $g$ is a subimmersion. If $P$ is of finite rank, the morphism $g$ is locally direct if and only if the vector rank of $g$ is locally constant or equivalently if and only if $g$ is a subimmersion.

7.5.6. Let $M \xrightarrow{f} M' \xrightarrow{g} M''$ be two morphisms of vector bundles. We say that the sequence $(f, g)$ is locally direct exact if the two morphisms $f$ and $g$ are locally direct and if $\operatorname{Im} f = \operatorname{Ker} g$. If $g \circ f = 0$, the set $D$ of points $b \in B$ such that the sequence $M_b \xrightarrow{f_b} M'_b \xrightarrow{g_b} M''_b$ is direct exact (that is to say, such that $\operatorname{Ker} f_b$ and $\operatorname{Im} g_b$ admit topological complements and that $\operatorname{Im} f_b = \operatorname{Ker} g_b$) is open and the sequence $M|D \xrightarrow{f} M'|D \xrightarrow{g} M''|D$ is locally direct exact.

One defines analogously the locally direct exact sequences of arbitrary length. By abuse of language, one sometimes says direct exact sequence instead of locally direct exact sequence.

7.5.7. Let $0 \to M \xrightarrow{f} M' \xrightarrow{g} M'' \to 0$ be a sequence of morphisms of vector bundles. For this sequence to be locally direct exact, it is necessary and sufficient that $f$ be an isomorphism of $M$ onto a vector subbundle $f(M)$ of $M'$ and that $g$ define by passing to the quotient an isomorphism of the quotient vector bundle $M'/f(M)$ onto $M''$.

### 7.6. Vector functors

In this no. and in the following three no.s 7.7 to 7.9, the letter I denotes a finite set, union of two disjoint subsets $I_+$ and $I_-$. We denote by $\mathcal{V} = (V_i)_{i \in I}$ (and analogously by $\mathcal{V}', \mathcal{V}'', \ldots$) a family of Banach spaces indexed by $I$. We denote by $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ the Banach space $\prod_{i \in I_+} \mathcal{L}(V_i; V'_i) \times \prod_{i \in I_-} \mathcal{L}(V'_i; V_i)$ and by $f = (f_i)$ an element of $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$. We denote by $\operatorname{Id}_{\mathcal{V}}$ the element $(\operatorname{Id}_{V_i})_{i \in I}$ of $\operatorname{Hom}(\mathcal{V}, \mathcal{V})$. For $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ and $f' \in \operatorname{Hom}(\mathcal{V}', \mathcal{V}'')$, we denote by $f' \circ f$ the element of $\operatorname{Hom}(\mathcal{V}, \mathcal{V}'')$ whose components are given by:

$$
(f' \circ f)_i = f'_i \circ f_i \quad \text{if } i \in I_+
$$
$$
(f' \circ f)_i = f_i \circ f'_i \quad \text{if } i \in I_-
$$

7.6.1. A vector functor (resp. vector functor of finite dimension) of type I and of class $C^r$ is called the data, for every family $\mathcal{V} = (V_i)_{i \in I}$ of Banach spaces (resp. of finite-dimensional vector spaces over $K$), of a Banach space $\tau(\mathcal{V})$ and, for every $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$, of an element $\tau(f) \in \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$, these data being subject to the following two conditions:
(a) One has $\tau(\operatorname{Id}_\mathcal{V}) = \operatorname{Id}_{\tau(\mathcal{V})}$ and $\tau(f' \circ f) = \tau(f') \circ \tau(f)$.
(b) The mapping $\tau : \operatorname{Hom}(\mathcal{V}, \mathcal{V}') \to \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$ is of class $C^r$.

7.6.2. Let $\mathcal{M} = (M^i)_{i \in I}$ be a family of vector bundles with base $B$. For $b \in B$, put $\mathcal{M}_b = (M^i_b)_{i \in I}$. Let $\tau$ be a vector functor and let $\tau(\mathcal{M})$ be the sum set of the $\tau(\mathcal{M}_b)$ for $b \in B$; *there exists on $\tau(\mathcal{M})$ one and only one structure of vector bundle* (with base $B$ relative to the mapping $\pi$ of $\tau(\mathcal{M})$ into $B$ such that, for every $b \in B$, one has $\tau(\mathcal{M}_b) = \{ b \}$) possessing the following property:

Let $U$ be an open set of $B$ and, for every $i$, let $t^i = (U, \varphi_i, F_i)$ be a vector chart of $M^i$, with domain $U$; put $\mathcal{F} = (F_i)_{i \in I}$ and let $\psi_b$ be the element of $\mathrm{Hom}(\mathcal{M}_b, \mathcal{F})$ defined by $(\psi_b)_i = (t^i_b)^{-1}$ for $i \in I_+$ and $(\psi_b)_i = t^i_b$ for $i \in I_-$; for $x \in \pi^{-1}(U)$, put $\psi(x) = (\pi(x), \tau(\psi_{\pi(x)})(x))$. Then the triplet $(U, \psi, \tau(\mathcal{F}))$ is a vector chart of the vector bundle $\tau(\mathcal{M})$.

Endowed with this structure, $\tau(\mathcal{M})$ is called the *vector bundle deduced from the family $\mathcal{M}$ by the vector functor $\tau$*.

7.6.3. Let $f$ be a morphism from $B$ into a manifold $B'$. Let $\mathcal{M} = (M^i)$ (resp. $\mathcal{M}' = ({M'}^i)$) be a family indexed by $I$ of vector bundles with base $B$ (resp. $B'$). For every $i \in I_+$, let $g_i$ be an $f$-morphism from $M^i$ into ${M'}^i$ and for every $i \in I_-$, let $g_i$ be an $f$-comorphism from ${M'}^i$ into $M^i$. Put $g = (g_i)_{i \in I}$ and for $b \in B$, put $g_b = ((g_i)_b)_{i \in I}$ (cf. 7.2.1 and 7.2.6). *There exists one and only one $f$-morphism, denoted $\tau(g)$, from $\tau(\mathcal{M})$ into $\tau(\mathcal{M}')$ such that $\tau(g)_b = \tau(g_b)$ for every $b \in B$*.

If in particular $M^i = f^*{M'}^i$, the $g_i$ being the canonical morphisms or comorphisms, then the $B$-morphism from $\tau(\mathcal{M})$ into $f^*\tau(\mathcal{M}')$ defined by $\tau(g)$ (7.2.4) is an isomorphism: this fact is expressed by saying that $\tau$ *commutes with inverse images*.

In particular let $B'$ be a submanifold of $B$ and put $\mathcal{M}|B' = (M^i|B')_{i \in I}$. The vector bundles $\tau(\mathcal{M})|B'$ and $\tau(\mathcal{M}|B')$ are then canonically $B'$-isomorphic.

7.6.4. Let $\tau, \tau_1, \ldots, \tau_d$ be vector functors (of type $I$ and of class $C'$). A *d-linear morphism* $\theta$ from $(\tau_1, \ldots, \tau_d)$ into $\tau$ is the data, for every family $\mathcal{V}$ of Banach spaces indexed by $I$, of a continuous $d$-linear mapping $\theta_{\mathcal{V}}$ from $\tau_1(\mathcal{V}) \times \cdots \times \tau_d(\mathcal{V})$ into $\tau(\mathcal{V})$, this data satisfying the following condition: for every $f \in \mathrm{Hom}(\mathcal{V}', \mathcal{V}'')$ one has
$$
\tau(f) \circ \theta_{\mathcal{V}} = \theta_{\mathcal{V}''} \circ (\tau_1(f) \times \cdots \times \tau_d(f)).
$$
For $d = 1$, one simply says a *morphism* from $\tau_1$ into $\tau$.

Let $\mathcal{M}$ be then a family indexed by $I$ of vector bundles over $B$.
*There exists one and only one B-d-linear morphism $\theta_{\mathcal{M}}$ from $\tau_1(\mathcal{M}) \times_B \cdots \times_B \tau_d(\mathcal{M})$ into $\tau(\mathcal{M})$ such that $(\theta_{\mathcal{M}})_b = \theta_{\mathcal{M}_b}$ for every $b \in B$*.

With the notations of 7.6.3., one has
$$
\tau(g) \circ \theta_{\mathcal{M}} = \theta_{\mathcal{M}'} \circ (\tau_1(g) \times \cdots \times \tau_d(g)).
$$
If $d = 1$, and if $\theta$ is an isomorphism (which means that $\theta_{\mathcal{V}}$ is an isomorphism for every family $\mathcal{V}$), then $\theta_{\mathcal{M}}$ is an isomorphism.

7.6.5. The definitions and results of Nos. 7.6.2 to 7.6.4 extend to the case of finite-dimensional vector functors, provided that the vector bundles given are assumed everywhere to have finite rank.

They also extend to the following case: let L be a field endowed with a structure of finite-dimensional K-algebra; one takes for τ a vector functor over L (i.e. satisfying the hypotheses of 7.6.1 in which K has been replaced by L), and one considers only vector bundles over L in the sense of 7.3.4.

7.6.6. One calls a vector functor (resp. finite-dimensional vector functor) for isomorphisms the data, for every Banach space V (resp. every finite-dimensional vector space over K), of a Banach space τ(V) and, for every isomorphism f of V onto a Banach space V’, of an isomorphism τ(f) of τ(V) onto τ(V’), these data being subject to condition (a) of 7.6.1 and to the following condition:

(b’) The mapping $f \mapsto \tau(f)$ from the open subset of $\mathcal{L}(V; V')$ constituted by the isomorphisms of V onto V’, into $\mathcal{L}(\tau(V); \tau(V'))$, is of class $C^r$.

The definitions and results of the preceding Nos. extend to the case of vector functors for isomorphisms (by taking $I_+ = \{1\}$ and $I_- = \varnothing$), with the exception of those of the first paragraph of No. 7.6.3.

### 7.7. Direct sums, bundles of multilinear mappings, dual

7.7.1. Assume that $I_- = \varnothing$. One defines a vector functor σ called the direct sum functor by putting $\sigma(\mathcal{V}) = \bigoplus_{i \in I} V_i$ and $\sigma(\mathfrak{f}) = \bigoplus_{i \in I} f_i$. If $\mathcal{M} = (M^i)_{i \in I}$ is a family of vector bundles over B, the vector bundle $\sigma(\mathcal{M})$ is called the direct sum of the $M^i$ and is denoted by $\bigoplus_{i \in I} M^i$. For every $b \in B$, the fibre at $b$ of $\bigoplus_{i \in I} M^i$ is the direct sum of the fibres of the $M^i$ at $b$.

Let U be an open subset of B and let $s_i \in \mathscr{F}_{M_i}(U)$ (for $i \in I$). The mapping $b \mapsto \sum_{i \in I} s_i(b)$ is then a section, denoted $\sum_i s_i$, of class $C^r$ of $M = \bigoplus_{i \in I} M^i$ and the mapping $(s_i)_{i \in I} \mapsto \sum_i s_i$ is an isomorphism of $\mathscr{C}^r(U)$-modules from $\bigoplus_{i \in I} \mathscr{F}_{M_i}(U)$ onto $\mathscr{F}_M(U)$.

The underlying manifold of $\bigoplus_{i \in I} M^i$ is identified with the fibre product $\prod_B M^i$.

We denote by $\mathrm{pr}_i$ the morphism of vector bundles from $\bigoplus_{i \in I} M^i$ into $M^i$ which on each fibre $\bigoplus_{i \in I} M^i_b$ is the i-th projection. We define analogously the canonical injection $j_i$ of $M^i$ into $\bigoplus_{i \in I} M^i$.

Let $f$ be a morphism from B into a manifold $B'$; let H be a second finite set and let $\mathcal{N} = (N^h)_{h \in H}$ be a family of vector bundles with basis $B'$. The mapping $u \to \bigoplus_{i \in I} (\mathrm{pr}_h \circ u \circ j_i)_{(h,i) \in H \times I}$ is a bijection from the set of $f$-morphisms of $\bigoplus_{i \in I} M^i$ into $\bigoplus_{h \in H} N^h$ onto the set of matrices $(u_{h,i})_{(h,i) \in H \times I}$, where $u_{h,i}$ is an $f$-morphism from $M^i$ into $N^h$.

If $I = \{1,2\}$, the sequence
$$
0 \to M^{1} \xrightarrow{j_1} M^1 \oplus M^2 \xrightarrow{\mathrm{pr}_2} M^2 \to 0
$$
is exact direct.

Conversely, let $M$ be a vector bundle with basis $B$ and let $M'$ be a vector subbundle of $M$. Suppose that the manifold $B$ is paracompact and that one of the following two conditions is satisfied :
(i) $K$ is different from $\mathbf{R}$ or $\mathbf{C}$;
(ii) $K = \mathbf{R}, r \neq \omega$ and the manifold $B$ admits partitions of unity of class $C^r$ (5.3.6).

There then exists a vector subbundle $M''$ of $M$ such that $M$ is identified with the direct sum $M' \oplus M''$.

7.7.2. Suppose that $I_+ = \{0\}$ and that $I_- = \{1,2,\ldots,d\}$. We define a vector functor $\eta_d$ of type $I$ and of class $C^r$ by setting $\eta_d(\mathcal{V}) = \mathcal{L}(V_1,\ldots,V_d; V_0)$ and $\eta_d(f)(u) = f_0 \circ u \circ (f_1 \times \cdots \times f_d)$ for $u \in \eta_d(\mathcal{V})$. If $\mathcal{M} = (M_i)_{i \in I}$ is a family of vector bundles with basis $B$, the vector bundle $\eta_d(\mathcal{M})$ is denoted by $\mathcal{L}(M_1,\ldots,M_d; M_0)$.

Let $u$ be a multilinear morphism from $M_1 \times_B \cdots \times_B M_d$ into $M_0$. The mapping $\hat{u} : b \mapsto u_b$ is then a section of $\mathcal{L}(M_1,\ldots,M_d; M_0)$ and the mapping $u \mapsto \hat{u}$ is bijective.

7.7.3. Retain the notations of 7.7.2 and suppose moreover that $d = 1$. The vector bundle $\mathcal{L}(M_1; M_0)$ is then called the bundle of homomorphisms from $M_1$ into $M_0$. Its sections correspond to the $B$-morphisms from $M_1$ into $M_0$.

If moreover $M_0$ is the trivial bundle $K_B$, the vector bundle $\mathcal{L}(M_1; K_B)$ is called the dual of $M = M_1$ and is denoted by $M'$: the fibre $(M')_b$ is the space of continuous linear forms on the fibre $M_b$ of $M$ at the point $b \in B$.

If $s$ (resp. $t$) is a section of $M$ (resp. $M'$) over an open set $U$ of $B$, the mapping $b \mapsto (b, \langle s(b), t(b) \rangle)$ is a section, denoted $\langle s, t \rangle$ of the trivial bundle $K_B$.$^1$

### 7.8. Bundles of alternating multilinear mappings

In nos. 7.8.1 to 7.8.5, it is assumed that $K$ is of characteristic 0 or that the vector bundles considered are of finite rank. It is not known whether the definition of the vector functor $\alpha_d$ given in 7.8.1 can be made without any restriction.

7.8.1. Let $I_+ = \{0\}, I_- = \{1\}$ and let $d$ be an integer $\geqslant 1$. We define a

$^1$ When $M$ is of finite rank, $M^*$ is written instead of $M'$.

vector functor $\alpha_d$ by denoting by $\alpha_d(\mathcal{V})$ the Banach space of continuous alternating $d$-linear mappings from $V_1^d$ into $V_0$ and by setting $\alpha_d(f)(u) = f_0 \circ u \circ f_1^d$ for $u \in \alpha_d(\mathcal{V})$. The vector bundle $\alpha_d((M_1, M_0))$ is denoted $\mathrm{Alt}^d(M_1; M_0)$ and is called the vector bundle of alternating $d$-linear mappings from $M_1$ into $M_0$.

The canonical injection of $\mathrm{Alt}^d(M_1; M_0)$ into $\mathcal{L}(M_1, \ldots, M_1; M_0)$ is a morphism of vector bundles; $\mathrm{Alt}^d(M_1; M_0)$ is a vector subbundle of $\mathcal{L}(M_1, \ldots, M_1; M_0)$.

One has $\mathrm{Alt}^1(M_1; M_0) = \mathcal{L}(M_1; M_0)$. We put $\mathrm{Alt}^0(M_1; M_0) = M_0$.

If $\omega$ is a section $^1$ of $\mathrm{Alt}^d(M_1; M_0)$ and if $s_1, \ldots, s_d$ are sections of $M_1$, there exists one and only one section of $M_0$, denoted $\omega(s_1, \ldots, s_d)$, such that
$$
\omega(s_1, \ldots, s_d)(b) = \omega(b)(s_1(b), \ldots, s_d(b)) \quad \text{for all } b \in B.
$$

7.8.2 Let $\varphi$ be a pairing of $N \times_B N'$ into $N''$ (cf. No. 7.3.1); for each $b$, we have a bilinear mapping $\varphi_b$ of $N_b \times N'_b$ into $N''_b$ which defines (cf. A, III, p. 142) a bilinear mapping of
$$
\mathrm{Alt}^d(M; N)_b \times \mathrm{Alt}^e(M; N')_b
$$
into $\mathrm{Alt}^{d+e}(M; N'')_b$. The collection of these bilinear mappings defines a pairing $u$ of
$$
\mathrm{Alt}^d(M; N) \times_B \mathrm{Alt}^e(M; N')
$$
into $\mathrm{Alt}^{d+e}(M; N'')$; if $\omega$ and $\omega'$ are respectively sections of $\mathrm{Alt}^d(M; N)$ and $\mathrm{Alt}^e(M; N')$ on an open set $U$, the section $u(\omega, \omega')$ of $\mathrm{Alt}^{d+e}(M; N'')$ on $U$ will be denoted by $\omega \wedge_\varphi \omega'$, and called the exterior product of $\omega$ and $\omega'$.
We have the formula:
(1) $$
(\omega \wedge_\varphi \omega')(s_1, \ldots, s_{d+e}) = \sum_\sigma \varepsilon_\sigma \varphi(\omega(s_{\sigma(1)}, \ldots, s_{\sigma(d)}), \omega'(s_{\sigma(d+1)}, \ldots, s_{\sigma(d+e)}))
$$
where the $s_i$ are sections of $M$ on $U$, and where the summation is extended to the permutations $\sigma$ of $\{1, 2, \ldots, d+e\}$ such that
$$
\sigma(1) < \cdots < \sigma(d) \quad \text{and} \quad \sigma(d+1) < \cdots < \sigma(d+e).
$$

7.8.3. Let $M$ be a vector bundle and $A$ an algebra bundle, with base $B$. Suppose that the fibres $A_b$ of $A$ are associative and commutative algebras, possessing a unit element, denoted by $e_b$. For every open set $U$ of $B$, we shall denote by $\Omega^d(U)$ the $\mathcal{C}^r(U)$-module formed by the sections of the bundle $\mathrm{Alt}^d(M; A)$ and by $\Omega^*(U)$ the direct sum of the $\Omega^d(U)$ for $d \geq 0$. The multiplications on each fibre define a pairing of $A \times_B A$ into $A$, whence (7.8.2) a graded algebra structure on $\Omega^*(U)$, which is associative and anticommutative. The subalgebra $\Omega^0(U)$ is the algebra of

¹ The reader should take care not to confuse this use of the letter $\omega$ with that defined p. 10.

sections of A. An element $\omega$ of $\Omega^1(U)$ identifies with a $U$-morphism of $M|U$ into $A|U$ (7.7.3): if $s \in \mathcal{S}'_M(U)$, we shall denote by $\langle \omega, s \rangle$ the section $\omega(s)$ of A (7.4.2). Let $s_j \in \mathcal{S}'_M(U)$ and $\omega_j \in \Omega^1(U)$ (for $1 \leq j \leq d$); we have:

(2) $$
\omega(s_1, \ldots, s_d) = \det(\langle \omega_i, s_j \rangle) \quad \text{for } \omega = \omega_1 \wedge \ldots \wedge \omega_d.
$$

7.8.4. Let $d \geq 1$. There exists a pairing $i$ of $M \times_B \mathrm{Alt}^d(M; A)$ into $\mathrm{Alt}^{d-1}(M; A)$ whose restriction to each fibre is given by the right interior product (cf. A, III, p. 156). If $s$ is a section of $M$ on the open set $U$ and if $\omega \in \Omega^d(U)$, we denote by $i(s)\omega$ the section $i(s, \omega)$ of $\mathrm{Alt}^{d-1}(M; A)$ on $U$; we set $i(s)\omega = 0$ for $\omega$ in $\Omega^0(U)$.

One thus associates with every section $s$ of $M$ on $U$ an endomorphism of the $\mathcal{C}'(U)$-module $\Omega^*(U)$. We have the following formulas:

(3) $$(i(s)\omega)(s_1, \ldots, s_{d-1}) = \omega(s, s_1, \ldots, s_{d-1}) \quad \text{for } \omega \in \Omega^d(U), d \geq 1$$
(4) $$i(s) \circ i(s) = 0$$
(5) $$i(s)\omega = \langle \omega, s \rangle \quad \text{for } \omega \in \Omega^1(U)$$
(6) $$i(s) . (\omega \wedge \omega') = i(s)\omega \wedge \omega' + (-1)^d \omega \wedge i(s)\omega' \quad \text{for } \omega \in \Omega^d(U)$$
(7) $$i(s)(\omega_1 \wedge \ldots \wedge \omega_p) = \sum_{i=1}^p (-1)^{i+1} \langle \omega_i, s \rangle \omega_1 \wedge \ldots \wedge \hat{\omega}_i \wedge \ldots \wedge \omega_d.$$

In the last formula, the $\omega_i$ are in $\Omega^1(U)$ and the sign $\hat{}$ indicates that the symbol which it surmounts is to be omitted.

All the operations described above on the sections are multilinear over the ring $\mathcal{C}'(U; K)$.

7.8.5. Let L be a Banach algebra over K. The definitions and results of Nos. 7.7 and 7.8 extend to the case of vector bundles over L: one defines in an analogous manner the bundles of L-multilinear or L-multilinear alternating mappings.

### 7.9. Tensor products, tensor spaces, exterior algebra

We retain the notations of 7.6. Moreover, we denote by L a commutative field endowed with a structure of finite-dimensional K-algebra and we call vector bundle a vector bundle over L, with base B and locally finite rank.

7.9.1. Suppose that $I_- = \varnothing$. If $\mathcal{V}$ and $\mathcal{V}'$ are two families indexed by I of finite-dimensional vector spaces over L, we denote by $\tau(\mathcal{V})$ the tensor product of the $V_i$ for $i \in I$ (A, II, p. 71) and if $f \in \mathrm{Hom}(\mathcal{V}, \mathcal{V}')$, we set $\tau(f) = \otimes f_i$. We thus define a vector functor over L in finite dimension and if $\mathcal{M} = (M_i)_{i \in I}$ is a family of vector bundles, we denote by $\bigotimes_{i \in I} M_i$ and call the tensor product (over L) of the $M_i$ the vector bundle $\tau(\mathcal{M})$.

If $s_i$ is a section of $M_i$ on the open set U of B (for $i \in I$), the mapping $b \mapsto \bigotimes_{i \in I} s_i(b)$ is a section of $\bigotimes_{i \in I} M_i$, denoted by $\bigotimes_{i \in I} s_i$. The mapping $(s_i)_{i \in I} \mapsto \bigotimes_{i \in I} s_i$ is multilinear over the ring $\mathcal{C}^r(U;L)$.

7.9.2. The canonical isomorphisms defined in Alg., Chap. II provide isomorphisms of vector functors. It follows from 7.6.4 that there are isomorphisms of vector bundles. For example, there are canonical isomorphisms:

$$
(M_1 \oplus M_2) \otimes M_3 \longrightarrow (M_1 \otimes M_3) \oplus (M_2 \otimes M_3)
$$
$$
M_1^* \otimes M_2 \longrightarrow \mathcal{L}(M_1; M_2)
$$

etc.

7.9.3. Let $M$ be a vector bundle and let $I$ and $J$ be two finite disjoint sets. The tensor bundle $T^I_J(M)$ is defined as the tensor product $\bigotimes_{\alpha \in I \cup J} M_\alpha$, where $M_\alpha = M$ if $\alpha \in I$, and $M_\alpha = M^*$ if $\alpha \in J$, $M^*$ denoting the dual of $M$ (A, III, p. 63). The fibre $T^I_J(M)_b$ of this bundle at a point $b$ is equal to the tensor space $T^I_J(M_b)$ defined in Alg., loc. cit. When $I = \{1, \ldots, p\}$ and $J = \{p+1, \ldots, p+q\}$, one writes $T^p_q(M)$ in place of $T^I_J(M)$; one has
$$
T^p_q(M) = (\bigotimes^p M) \otimes (\bigotimes^q M^*).
$$
The giving of a total order on $I$ and on $J$ defines a canonical isomorphism of $T^I_J(M)$ onto $T^p_q(M)$.

7.9.4. If $I$ (resp. $J$) is the union of two disjoint subsets $I'$ and $I''$ (resp. $J'$ and $J''$), $T^I_J(M)$ is canonically identified with the tensor product $T^{I'}_{J'}(M) \otimes T^{I''}_{J''}(M)$. In particular, if $s'$ (resp. $s''$) is a section of $T^{I'}_{J'}(M)$ (resp. of $T^{I''}_{J''}(M)$), the tensor product $s' \otimes s''$ is identified with a section of $T^I_J(M)$.

7.9.5. The dual of $T^I_J(M)$ is identified with $T^J_I(M)$.

7.9.6. Let $i \in I$ and $j \in J$. For every $b \in B$, the homomorphism of contraction of the indices $i$ and $j$ is defined (cf. Alg., loc. cit.); it is a homomorphism $(c^i_j)_b : T^I_J(M_b) \to T^{I-\{i\}}_{J-\{j\}}(M_b)$. The collection of the $(c^i_j)_b$ defines a morphism of vector bundle spaces
$$
c^i_j : T^I_J(M) \to T^{I-\{i\}}_{J-\{j\}}(M),
$$

also called contraction of the indices $i$ and $j$. One defines analogously the contraction of the indices $i_1, \ldots, i_k$ of $I$ with the indices $j_1, \ldots, j_k$ of $J$.

7.9.7. Let $d$ be an integer $\geqslant 0$; let $V$ and $V'$ be two vector spaces of finite dimension over $L$ and $f \in \mathrm{Hom}_L(V, V')$; put $\lambda_d(V) = \bigwedge^d(V)$ and $\lambda_d(f) = \bigwedge^d(f)$. One thus defines a vector functor over $L$ in finite dimension and, if $M$ is a vector bundle, one denotes by $\bigwedge^d(M)$ and calls $d$-th exterior power of $M$ (over $L$) the vector bundle $\lambda_d(M)$.

The canonical mapping of $\bigotimes^d V$ onto $\bigwedge^d(V)$ defines a morphism of vector functors, whence a canonical morphism of $\bigotimes^d M$ into $\bigwedge^d(M)$. This morphism is surjective.

The canonical isomorphisms of the space of alternating $d$-multilinear mappings on the space $\bigwedge^d(V^*)$ or on $(\bigwedge^d(V))^*$ provide isomorphisms, called canonical, of the vector bundle $\mathrm{Alt}^d(M; L)$ of alternating $d$-multilinear mappings on $L$, onto the vector bundle $\bigwedge^d(M^*)$ or onto $(\bigwedge^d(M))^*$.

7.9.8. Put now $\lambda(V) = \bigwedge(V)$ and $\lambda(f) = \bigwedge(f)$; one thus again defines a vector functor on $L$ in finite dimension. The vector bundle $\lambda(M)$ is denoted by $\bigwedge(M)$. Its fibre $\bigwedge(M)_b$ at $b \in B$ is the exterior algebra (over $L$) of the fibre $M_b$. The vector bundle $\bigwedge(M)$ is a locally trivial vector bundle in algebras.

The definitions and properties of the interior products given in Alg., Chap. III, 3rd ed., § 10 extend immediately to the sections of the vector bundles $\bigwedge(M)$ and $\bigwedge(M^*)$ (cf. also the formulas (1) to (7) of Nos. 7.8.2 to 7.8.4).

7.9.9. Let $M$ be a vector bundle. For every integer $n$, let $B_n$ be the set (open) of the points $b \in B$ such that the dimension (over $L$) of $M_b$ is equal to $n$. For $b \in B_n$, put $N_b = \bigwedge^n(M_b)$ and let $N$ be the sum set of the $N_b$ for $b \in B$. There exists on $N$ one and only one structure of vector bundle such that the obvious mapping of $N|B_n$ into $\bigwedge^n(M)|B_n$ is an isomorphism for every $n$. Endowed with this structure, the vector bundle $N$ of rank one at each point is denoted by $\det(M)$.

### 7.10. Vector bundles and principal bundles

7.10.1. Let $F$ be a Banach space. A vector bundle $M$ with base $B$ is said to be pure of type $F$ if all the fibres $M_b$ of $M$ (for $b \in B$) are isomorphic (as Banach spaces) to $F$.

Let $M$ be a vector bundle of base $B$ pure of type $F$ and let $P$ be the open subvariety of the vector bundle $\mathcal{L}(F_B; M)$ composed of the pairs $(b, u)$ where $b \in B$ and where $u$ is an isomorphism of $F_b = F$ onto $M_b$. The group $\mathrm{GL}(F)$ of automorphisms of $F$ operates on the right on $P$ by setting $(b, u) \cdot g = (b, u \circ g)$ for $(b, u) \in P$ and $g \in \mathrm{GL}(F)$. Let $\pi_P$ denote the mapping $(b, u) \mapsto b$ from P into B. The quadruplet $\lambda = (P, GL(F), B, \pi_P)$ (where $GL(F)$ is endowed with its canonical structure of group variety (5.12.2)) is a principal fibration (6.2.1): it is called the fibration of frames of M. The mapping $((b, u), h) \mapsto u(h)$ from $P \times F$ into M endows M with a structure of associated bundle to $\lambda$, of fibre type F (6.5.1).

When $F = K^n$, one can identify an isomorphism $u$ of F onto $M_b$ with the basis of $M_b$ image by $u$ of the canonical basis of $K^n$. The fibred space of frames of M is then identified with the open subvariety of $M \times_B \ldots \times_B M$ formed by the bases $(e_1, \ldots, e_n)$ of the different fibres $M_b$.

Let U be an open subset of B and let $t = (U, \varphi, E)$ be a vector chart of M of domain U, with $E = F$. The mapping $b \mapsto (b, t_b)$ is then a section of P, denoted $\tilde{t}$, and the mapping $t \mapsto \tilde{t}$ is a bijection from the set of vector charts of M of the form $(U, \varphi, F)$ onto the set of sections of P over U.

7.10.2. Conversely, let $\lambda = (Q, G, B, \pi_Q)$ be a principal fibration and let $\varphi$ be a homomorphism of group varieties of G into the group $GL(F)$ of automorphisms of a Banach space F. Let G operate on the left on F by setting $g . h = \varphi(g)(h)$ ($h \in F, g \in G$). Let M be a fibred space associated with $\lambda$, of fibre type F, and let $\rho : Q \times F \to M$ be its frame mapping (6.5.1). Let $\pi$ be the mapping from M into B defined by
$$
\pi(\rho(q, h)) = \pi_Q(q) \quad (q \in Q \text{ and } h \in F).
$$
Let s be a section of Q over an open subset U of B; the mapping
$$
\tilde{s} : (b, h) \mapsto (s(b), h)
$$
is then a bijection from $U \times F$ onto $\pi^{-1}(U)$. There exists on the pair $(M, \pi)$ one and only one structure of vector bundle of base B for which the triples $t_s = (U, \tilde{s}^{-1}, F)$ are vector charts (for every section s of Q). The structure of underlying variety of this structure is that of the fibred space associated with $\lambda$.

Let $q \in Q$; put $b = \pi_Q(q)$ and let $u$ be the isomorphism of F onto $M_b$ defined by $u(h) = \rho(q, h)$ (for $h \in F$). The mapping $f : q \mapsto (b, u)$ is a B-morphism of principal fibrations, compatible with $\varphi$, from $(Q, G, B, \pi_Q)$ into the frame bundle $(P, GL(F), B, \pi_P)$ of the vector bundle M.

7.10.3. Let us take up again the notations of No. 7.6. For every $i \in I$, let
$$
\lambda_i = (P_i, G_i, B, \pi_i)
$$
be a principal fibration with base B and suppose that $G_i$ operates on the left on a Banach space $V_i$ by means of a homomorphism
$$
\varphi_i : G_i \to GL(V_i).
$$
Let $M_i$ be a fibre space associated with $\lambda_i$ of fibre type $V_i$. Put $\mathcal{M} = (M_i)_{i \in I}$ and $\mathcal{V} = (V_i)_{i \in I}$ and let $\lambda$ be the product principal fibration of the $\lambda_i$ over B (6.2.5). Put $\hat{\lambda} = (\mathbf{P}, G, B, \pi_p)$, with $G = \prod_{i \in I} G_i$.

Let now $\tau$ be a vector functor. For $g = (g_i) \in G$, let $\varphi(g)$ be the element of $\mathrm{Hom}(\mathcal{V}, \mathcal{V})$ defined by:

$$
\varphi(g)_i = \varphi_i(g_i) \quad \text{si } i \in I_+
$$
$$
\varphi(g)_i = \varphi_i(g_i)^{-1} \quad \text{si } i \in I_-
$$

The group $G$ then operates on $\tau(\mathcal{V})$ by means of the morphism $g \mapsto \tau(\varphi(g))$ from $G$ into $\mathbf{GL}(\tau(\mathcal{V}))$.

Let on the other hand $x = (x_i)$ be a point of $\mathbf{P}$ and let $b = \pi_p(x)$. For each $i$, the mapping $\theta_{x_i}$ defined in No. 6.5.2 is an isomorphism of $V_i$ onto $(M_i)_b$. Let $\theta_x$ be the element of $\mathrm{Hom}(\mathcal{V}, ((M_i)_b)_{i \in I})$ defined by:

$$
(\theta_x)_i = \theta_{x_i} \quad \text{si } i \in I_+
$$
$$
(\theta_x)_i = \theta_{x_i}^{-1} \quad \text{si } i \in I_-
$$

Let $\rho$ be the mapping $(x, h) \mapsto (b, \tau(\theta_x)(h))$ from $\mathbf{P} \times \tau(\mathcal{V})$ into the vector bundle $\tau(\mathcal{M})$; the mapping $\rho$ endows $\tau(\mathcal{M})$ with a structure of fibre space associated with $\lambda$ of fibre type $\tau(\mathcal{V})$.

These considerations generalize to the case of finite-dimensional vector functors, or of vector functors over a field $L$ endowed with a structure of finite-dimensional K-algebra.

### 7.11. Change of structure

The structures and operations described in this paragraph are compatible with the changes of structure described in Nos. 5.13 and 5.14.
