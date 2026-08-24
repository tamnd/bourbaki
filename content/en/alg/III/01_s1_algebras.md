---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 1
section_title: Algebras
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0452-0462, 0642-0642
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ALGEBRA
      page: 0
      pdf_page: 452
    - "no": 2
      title: SUBALGEBRAS. IDEALS. QUOTIENT ALGEBRAS
      page: 0
      pdf_page: 453
    - "no": 3
      title: DIAGRAMS EXPRESSING ASSOCIATIVITY AND COMMUTATIVITY
      page: 0
      pdf_page: 455
    - "no": 4
      title: PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 456
    - "no": 5
      title: RESTRICTION AND EXTENSION OF SCALARS
      page: 0
      pdf_page: 457
    - "no": 6
      title: INVERSE AND DIRECT LIMITS OF ALGEBRAS
      page: 0
      pdf_page: 458
    - "no": 7
      title: BASES OF AN ALGEBRA. MULTIPLICATION TABLE
      page: 0
      pdf_page: 460
statements: 5
exercises: 1
content_sha256: df1bf9d1994bf065f92a5e355edfddb031eece07963c82645afd130ae8c05a13
---

## § 1. ALGEBRAS

### 1. DEFINITION OF AN ALGEBRA

#### Definition 1 {#alg-iii-s1-def-1 .statement}

Let $ A $ be a commutative ring. An algebra over $ A $ (or an $ A $-algebra, or simply an algebra, when no confusion is to be feared) is a set $ E $ with a structure defined by giving the following:
(1) an $ A $-module structure on $ E $;
(2) an $ A $-bilinear mapping (II, § 3, no. 5) of $ E \times E $ into $ E $.

The $ A $-bilinear mapping of $ E \times E $ into $ E $ occurring in this definition is called the multiplication of the algebra $ E $; it is usually denoted by $ (x, y) \mapsto x.y $, or simply $ (x, y) \mapsto xy $.

Let $ (\alpha_i)_{i \in I} $ and $ (\beta_j)_{j \in J} $ be two families of elements of $ A $, of finite support (I, § 2, no. 1). Then, for all families $ (x_i)_{i \in I} $ and $ (y_j)_{j \in J} $ of elements of $ E $, the general distributivity formula (I, § 3, no. 4)

$$
\left( \sum_{i \in I} \alpha_i x_i \right) \left( \sum_{j \in J} \beta_j y_j \right) = \sum_{(i, j) \in I \times J} (\alpha_i \beta_j)(x_i y_j)
$$

holds; in particular

$$
(\alpha x)y = x(\alpha y) = \alpha(xy) \quad \text{for } \alpha \in A, x \in E \text{ and } y \in E.
$$

The bilinear mapping $ (x, y) \mapsto yx $ of $ E \times E $ into $ E $ and the $ A $-module structure on $ E $ define an $ A $-algebra structure on $ E $, called opposite to the given algebra structure. The set $ E $ with this new structure is called the opposite algebra to the algebra $ E $; it is often denoted by $ E^0 $. The $ A $-algebra $ E $ is called commutative if it is identical with its opposite, in other words if multiplication in $ E $ is commutative. An isomorphism of $ E $ onto $ E^0 $ is also called an anti-automorphism of the algebra $ E $.

When multiplication in the algebra $ E $ is associative, $ E $ is called an associative $ A $-algebra. When multiplication in $ E $ admits an identity element (necessarily unique (I, § 2, no. 1)), this element is called the unit element of $ E $ and $ E $ is called a unital algebra.

#### Example {#alg-iii-s1-n1-exa-1 .statement}

(1) Every commutative ring $ A $ can be considered as an (associative and commutative) $ A $-algebra.
(2) Let $ E $ be a pseudo-ring (I, § 8, no. 1). Multiplication on $ E $ and the unique $ \mathbf{Z} $-module structure on $ E $ define on $ E $ an associative $ \mathbf{Z} $-algebra structure.
(3) Let $ F $ be a set and $ A $ a commutative ring. The set $ A^F $ of all mappings of $ F $ into $ A $, with the product ring structure (I, § 8, no. 10) and the product

A-module structure (II, § 1, no. 5) is an associative and commutative A-algebra.

(4) Let E be an A-algebra; the internal laws $(x, y) \mapsto xy + yx$ and $(x, y) \mapsto xy - yx$ define (with the A-module structure on E) two A-algebra structures on E, which are not in general associative; the first law

$$(x, y) \mapsto xy + yx$$

is always commutative.

#### Definition 2 {#alg-iii-s1-def-2 .statement}

*Given two algebras* E, E' *over a commutative ring* A, *a homomorphism of* E *into* E' *is a mapping* $f : E \to E'$ *such that*
(1) *f is an* A*-module homomorphism*;
(2) $f(xy) = f(x)f(y)$ *for all* $x \in E$ *and* $y \in E$.

Clearly the composition of two A-algebra homomorphisms is an A-algebra homomorphism. Every bijective algebra homomorphism is an isomorphism. Therefore A-algebra homomorphisms may be taken as *morphisms* of the species of A-algebra structure (*Set Theory*, IV, 2, no. 1). We shall always suppose in what follows that this choice of morphisms has been made. If E, E' are two A-algebras, let $\operatorname{Hom}_{A\text{-alg}}(E, E')$ denote the set of A-algebra homomorphisms of E into E'.

Let E, E' be two algebras each with a unit element. A homomorphism of E into E' mapping the unit element of E to the unit element of E' is called a *unital homomorphism* (or *unital algebra morphism*).

### 2. SUBALGEBRAS. IDEALS. QUOTIENT ALGEBRAS

Let A be a commutative ring and E an A-algebra. If F is a sub-A-module of W which is stable under the multiplication on E, the restriction to F × F of the multiplication of E defines (with the A-module structure on F) an A-algebra structure on F. F, with this structure, is called a *subalgebra* of the A-algebra E. Every intersection of subalgebras of E is a subalgebra of E. For every family $(x_i)_{i \in I}$ of elements of E, the intersection of the subalgebras of E containing all the $x_i$ is called the subalgebra of E *generated* by the family $(x_i)_{i \in I}$ and $(x_i)_{i \in I}$ is called a *generating system* (or *generating family*) of this subalgebra. If $u : E \to E'$ is an A-algebra homomorphism, the image $u(F)$ of every subalgebra F of E is a subalgebra of E'.

Let E be an *associative* algebra. For every subset M of E, the set $M'$ of elements of E which are permutable with all the elements of M is a subalgebra of E called the *centralizer* subalgebra of M in E (I, § 1, no. 5). The centralizer $M''$ of $M'$ in E is also called the *bicentralizer* of M; clearly $M \subset M''$. It follows that $M'$ is contained in its bicentralizer $M''$, which is just the centralizer of $M''$; but the relation $M \subset M''$ implies $M'' \subset M'$, so that $M' = M''$ (cf. *Set Theory*, III, § 1, no. 7, Proposition 2). If F is a subalgebra of E, the *centre* of F is the intersection $F \cap F'$ of F and its centralizer $F'$ in E. Note that if

F is *commutative*, then $ F \subset F' $ and hence $ F' \supset F'' $; the bicentralizer $ F'' $ of F is in this case the *centre* of F.

For certain non-associative algebras (for example Lie algebras) the notions of centralizer of a subalgebra and centre are defined differently (*Lie Groups and Lie algebras*, I, § 1, no. 6).

A subset $ a $ of an A-algebra E is called a *left ideal* (resp. *right ideal*) of E when $ a $ is a sub-A-module of E and the relations $ x \in a,\ y \in E $ imply $ yx \in a $ (resp. $ xy \in a $). It amounts to the same to say that $ a $ is a left ideal of E or a right ideal of the opposite algebra $ E^0 $. A *two-sided ideal* of E is a subset $ a $ of E which is both a left ideal and a right ideal. When E is associative and admits a unit element $ e $, then, for $ \alpha \in A $ and $ x \in E $, $ \alpha x = (\alpha e)x = x(\alpha e) $ by virtue of (2) (no. 1) and hence the (right, left, two-sided) ideals of the *ring* E (I, § 8, no. 6) are identical with the (right, left, two-sided) ideals of the *algebra* E. Every sum and every intersection of left (resp. right, two-sided) ideals of the algebra E is a left (resp. right, two-sided) ideal. The intersection of the left (resp. right, resp. two-sided) ideals containing a subset X of E is called the left (resp. right, resp. two-sided) ideal of E *generated* by X.

Let $ b $ be a *two-sided* ideal of an A-algebra E. If $ x \equiv x' \pmod{b} $ and $ y \equiv y' \pmod{b} $, then
$$
x(y - y') \in b \quad \text{and} \quad (x - x')y' \in b
$$
and hence $ xy \equiv x'y' \pmod{b} $. Hence an internal law can be defined on the quotient A-module $ E/b $, which is the quotient of the multiplication law $ (x, y) \mapsto xy $ of E by the equivalence relation $ x \equiv x' \pmod{b} $ (I, § 1, no. 6). It is immediately verified that this quotient law is an A-bilinear mapping of $ (E/b) \times (E/b) $ into $ E/b $; it therefore defines with the A-module structure on $ E/b $ an A-algebra structure on $ E/b $. $ E/b $, with this algebra structure, is called the *quotient algebra* of the algebra E by the two-sided ideal $ b $. The canonical mapping $ p : E \to E/b $ is an algebra homomorphism.

Let E, $ E' $ be two A-algebras and $ u : E \to E' $ an algebra homomorphism. The image $ u(E) $ is a subalgebra of $ E' $ and the kernel $ b = u^{-1}(0) $ is a two-sided ideal of E; further, in the canonical decomposition of $ u $:
$$
E \xrightarrow{p} E/b \xrightarrow{v} u(E) \xrightarrow{j} E'
$$
$ v $ is an *algebra isomorphism*. More generally, all the results of Chapter I, § 8, no. 9 are still valid (and also their proofs) when the word "ring" is replaced by "algebra".

Let A be a commutative ring and E an A-algebra. On the set $ \tilde{E} = A \times E $, we define the following laws of composition:
$$
\begin{align*}
(\lambda, x) + (\mu, y) &= (\lambda + \mu, x + y) \\
(\lambda, x)(\mu, y) &= (\lambda \mu, xy + \mu x + \lambda y) \\
\lambda(\mu, x) &= (\lambda \mu, \lambda x).
\end{align*}
$$

It is immediately verified that $ \tilde{E} $, with these laws of composition, is an algebra over $ A $ and $ (1,0) $ is a unit element of this algebra. The set $ \{0\} \times E $ is a two-sided ideal of $ \tilde{E} $ and $ x \mapsto (0,x) $ is an isomorphism of the algebra $ E $ onto the subalgebra $ \{0\} \times E $, by means of which $ E $ and $ \{0\} \times E $ are identified. $ \tilde{E} $ is called the algebra derived from $ E $ by adjoining a unit element; it is associative (resp. commutative) if and only if $ E $ is.

### 3. DIAGRAMS EXPRESSING ASSOCIATIVITY AND COMMUTATIVITY

Let $ A $ be a commutative ring and $ E $ an $ A $-module; being given a bilinear mapping of $ E \times E $ into $ E $ is equivalent to being given an $ A $-linear mapping:

$$
m : E \otimes_A E \to E
$$

(II, § 3, no. 5). An $ A $-algebra structure on $ E $ is therefore defined by giving an $ A $-module structure on $ E $ and an $ A $-linear mapping of $ E \otimes_A E $ into $ E $.

Let $ E' $ be another $ A $-algebra and $ m' : E' \otimes_A E' \to E' $ the $ A $-linear mapping defining the multiplication of $ E' $. A mapping $ f : E \to E' $ is an $ A $-algebra homomorphism if and only if $ f $ is a mapping rendering commutative the diagram

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{f \otimes f} & E' \otimes_A E' \\
\downarrow m & & \downarrow m' \\
E & \xrightarrow{f} & E'
\end{array}
$$

For an $ A $-algebra $ E $ to be associative, it is necessary and sufficient (taking account of the associativity of tensor products, cf. II, § 3, no. 8) that the diagram of $ A $-linear mappings

$$
\begin{array}{ccc}
E \otimes_A E \otimes_A E & \xrightarrow{m \otimes 1_E} & E \otimes_A E \\
\downarrow 1_E \otimes m & & \downarrow m \\
E \otimes_A E & \xrightarrow{m} & E
\end{array}
$$

be commutative. Similarly, for the $ A $-algebra $ E $ to be commutative, it is necessary and sufficient that the diagram of $ A $-linear mappings

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E \\
\downarrow m & & \downarrow m \\
E & & E
\end{array}
$$

be commutative, where $ \sigma $ denotes the canonical $ A $-linear mapping defined by σ(x \otimes y) = y \otimes x \text{ for } x \in E, y \in E \text{ (II, § 3, no. 1, Corollary 2 to Proposition 1).}

For all $ c \in E $, let $ \eta_c $ denote the A-linear mapping of A into E defined by the condition $ \eta_c(1) = c $. For $ c $ to be a unit element of E, it is necessary and sufficient that the two diagrams

$$
\begin{array}{ccc}
A \otimes_A E & \xrightarrow{\eta_c \otimes 1_E} & E \otimes_A E \\
\downarrow i & & \downarrow m \\
E & & E \\
& \uparrow & \\
E \otimes_A A & \xrightarrow{1_E \otimes \eta_c} & E \otimes_A E \\
& \downarrow i' & \downarrow m \\
E & & E
\end{array}
$$

be commutative ($ i $ and $ i' $ denoting the canonical isomorphisms (II, § 3, no. 4, Proposition 4)).

Let E be an A-algebra with unit element e and let $ \eta = \eta_e $ (also denoted by $ \eta_E $); then $ \eta(\alpha \beta) = \eta(\alpha) \eta(\beta) = \alpha \eta(\beta) $, for by (2) (no. 1),

$$(\alpha e)(\beta e) = (\alpha \beta)e = \alpha(\beta e);$$

hence $ \eta $ is an A-algebra homomorphism. Observe that the A-module structure on E can be defined using $ \eta $, for

$$(3)$$
$$\alpha x = \eta(\alpha) \cdot x \quad \text{for } \alpha \in A, x \in E$$

(where, on the right hand side, multiplication is in E). The image of the homomorphism $ \eta $ is a subalgebra of E whose elements commute with all those of E. The kernel of the homomorphism $ \eta $ is the annihilator of the element e of the A-module E; by (3), it is also the annihilator of the A-module E (II, § 1, no. 12).

When the algebra E is unital and associative, $ \eta $ is a ring homomorphism. Conversely, let $ \rho : A \to B $ be a ring homomorphism such that the image $ \rho(A) $ is contained in the centre of B, assuming also that the ring A is commutative; then an A-algebra structure is defined on B which is associative and unital, by writing (cf. (3))

$$\lambda x = \rho(\lambda) \cdot x \quad \text{for } \lambda \in A, x \in E.$$

### 4. PRODUCTS OF ALGEBRAS

Let $ (E_i)_{i \in I} $ be a family of algebras over the same commutative ring A. It is immediately verified that on the product set $ E = \prod_{i \in I} E_i $, the product A-module structure (II, § 1, no. 5) and the multiplication

$$(4)$$
$$((x_i), (y_i)) \mapsto (x_i y_i)$$

define an A-algebra structure; with this structure, the set E is called the product algebra of the family of algebras $ (E_i)_{i \in I} $.

When all the algebras $ E_i $ are associative (resp. commutative, resp. unital), so is their product. Moreover, all the properties stated in I, § 8, no. 10, extend without modification to arbitrary products of algebras.

### 5. RESTRICTION AND EXTENSION OF SCALARS

Let $ A_0 $ and A be two commutative rings and $ \rho : A_0 \to A $ a ring homomorphism. If E is an A-algebra, we denote (conforming with II, § 1, no. 13) by $ \rho_* (E) $ the $ A_0 $-module defined by addition on E and the external law

$$
\lambda . x = \rho(\lambda)x \quad \text{for all } \lambda \in A_0 \text{ and all } x \in E.
$$

Multiplication in E and the $ A_0 $-module structure on $ \rho_* (E) $ define an $ A_0 $-algebra structure on $ \rho_* (E) $. When $ A_0 $ is a subring of A and $ \rho $ the canonical injection, the algebra $ \rho_* (E) $ is said to be obtained from E by restricting the ring A of scalars to $ A_0 $. By an abuse of language, this is also sometimes said when $ \rho $ is arbitrary.

Let F be an $ A_0 $-algebra. An $ A_0 $-algebra homomorphism $ F \to \rho_* (E) $ is called a semi-homomorphism (relative to $ \rho $) or a $ \rho $-homomorphism of F into the A-algebra E; it is also called an $ A_0 $-homomorphism if no confusion arises. If E, $ E' $ are two A-algebras, every A-algebra homomorphism $ E \to E' $ is also an $ A_0 $-algebra homomorphism $ \rho_* (E) \to \rho_* (E') $.

Consider now two commutative rings A and B and a ring homomorphism $ \rho : A \to B $. For every A-module E, the B-module $ \rho^*(E) = E \otimes_A B $, obtained from E by extending the ring A of scalars to B, has been defined (II, § 5, no. 1). If E is also an A-algebra, we shall define on $ \rho^*(E) $ a B-algebra structure. For this, observe that $ (E \otimes_A B) \otimes_B (E \otimes_A B) $ is canonically isomorphic to $ (E \otimes_A E) \otimes_A B $ (II, § 5, no. 1, Proposition 3). If $ m : E \otimes_A E \to E $ defines the multiplication on E, the mapping $ m \otimes 1_B : (E \otimes_A E) \otimes_A B \to E \otimes_A B $ is therefore canonically identified with a B-linear mapping

$$
m' : \rho^*(E) \otimes_B \rho^*(E) \to \rho^*(E)
$$

which defines the desired B-algebra structure on $ \rho^*(E) $. Hence

(5)

$$
(x \otimes \beta)(x' \otimes \beta') = (xx') \otimes (\beta \beta')
$$

for $ x, x' $ in E, $ \beta $ and $ \beta' $ in B. The B-algebra $ \rho^*(E) $ is said to be derived from the A-algebra E by extending the ring A of scalars to B (by means of $ \rho $). It is also denoted by $ E_{(B)} $ or $ E \otimes_A B $. When E is associative (resp. commutative, resp. unital), so is $ \rho^*(E) $.

#### Proposition 1 {#alg-iii-s1-prop-1 .statement}

For every A-algebra E, the canonical mapping $ \phi_E : x \mapsto x \otimes 1 $ of E into $ E_{(B)} $ is an A-homomorphism of algebras. Moreover, for every B-algebra F and every $ A $-homomorphism $ f : E \to F $, there exists one and only one $ B $-homomorphism $ \bar{f} : E_{(B)} \to F $ such that $ \bar{f}(x \otimes 1) = f(x) $ for all $ x \in E $.

The first assertion follows immediately from the definition of multiplication in $ E_{(B)} $, which gives $ (x \otimes 1)(x' \otimes 1) = (xx') \otimes 1 $ for $ x \in E $ and $ x' \in E $. The existence and uniqueness of the $ B $-linear mapping $ \bar{f} $ of $ E_{(B)} $ into $ F $ satisfying the relation $ \bar{f}(x \otimes 1) = f(x) $ for all $ x \in E $ follow from II, § 5, no. 1, Proposition 1; here it all amounts to verifying that $ \bar{f}(yy') = \bar{f}(y)\bar{f}(y') $ for $ y $ and $ y' $ in $ E_{(B)} $; as the elements of the form $ x \otimes 1 $ (with $ x \in E $) generate the $ B $-module $ E_{(B)} $, attention may be confined to the case where $ y = x \otimes 1, y' = x' \otimes 1 $ with $ x \in E, x' \in E $; as $ yy' = (xx') \otimes 1 $, the relation $ \bar{f}(yy') = \bar{f}(y)\bar{f}(y') $ then follows from $ f(xx') = f(x)f(x') $.

It can also be said that $ f \mapsto \bar{f} $ is a canonical bijection

$$
\text{Hom}_{A\text{-alg.}}(E, \rho_*(F)) \to \text{Hom}_{B\text{-alg.}}(\rho^*(E), F).
$$

The ordered pair consisting of $ E_{(B)} $ and $ \phi_E $ is therefore a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1) where $ \Sigma $ is the species of $ B $-algebra structure and the $ \alpha $-mappings the $ A $-homomorphisms from $ E $ to a $ B $-algebra.

#### Corollary {#alg-iii-s1-n5-cor-1 .statement}

*Let $ E, E' $ be two $ A $-algebras; for every $ A $-homomorphism of algebras $ u : E \to E', u \otimes 1_B $ is the unique $ B $-homomorphism of algebras $ v : E \otimes_A B \to E' \otimes_A B $ rendering commutative the diagram*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E \otimes_A B \\
u \downarrow & & \downarrow v \\
E' & \xrightarrow{\phi_{E'}} & E' \otimes_A B
\end{array}
$$

Let $ C $ be a third commutative ring and $ \sigma : B \to C $ a ring homomorphism; it is immediate that the canonical $ C $-homomorphism

$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$

mapping $ (x \otimes 1) \otimes 1 $ to $ x \otimes 1 $ for all $ x \in E $ (II, § 5, no. 1, Proposition 2) is an algebra isomorphism.

### 6. INVERSE AND DIRECT LIMITS OF ALGEBRAS

Let $ I $ be a preordered set and $ (A_i, \phi_{ij}) $ an inverse system of *commutative rings* with $ I $ as indexing set. Let $ (E_i, f_{ij}) $ be an inverse system of $ A_i $-modules with $ I $ as indexing set (II, § 6, no. 1) and suppose further that each $ E_i $ has an $ A_i $-algebra structure and that, for $ i \leq j $, $ f_{ij} $ is an $ A_j $-homomorphism of algebras (relative to $ \phi_{ij} $) (no. 5). Let $ A = \lim \leftarrow A_i $ and $ E = \lim \leftarrow E_i $, which has an $ A $-module structure, the inverse limit of the structure of the $A_i$-modules $E_i$ (II, § 6, no. 1); it is immediately verified that the law of composition on $E$, considered as the inverse limit of the $E_i$ considered as magmas under multiplication (I, § 10, no. 1), with the $A$-module structure on $E$, defines on $E$ an $A$-algebra structure; $(E_i, f_{ij})$ is called an *inverse system* of $A_i$-algebras and the $A$-algebra $E$ is called its *inverse limit*. If $f_i : E \to E_i$, $\phi_i : A \to A_i$ are the canonical mappings, $f_i$ is an *$A$*-homomorphism of algebras (relative to $\phi_i$). If the $E_i$ are associative (resp. commutative), so is $E$; if each $E_i$ admits a unit element $e_i$ and $f_{ij}(e_j) = e_i$ for $i \leq j$, $e = (e_i)$ is a unit element of the algebra $E$.

Let $(E'_i, f'_{ij})$ be another inverse system of $A_i$-algebras and for all $i$ let $u_i : E_i \to E'_i$ be an $A_i$-algebra homomorphism, these mappings forming an *inverse system*; then $u = \lim u_i$ is an *$A$*-algebra homomorphism.

Suppose now that all the $A_i$ are equal to the *same* commutative *ring* $A$ and the $\phi_{ij}$ to $\mathrm{Id}_A$, so that $E = \lim \leftarrow E_i$ is an $A$-algebra. Let $F$ be an $A$-algebra and, for all $i \in I$, let $u_i : F \to E_i$ be an $A$-algebra homomorphism such that $(u_i)$ is an inverse system of mappings; then $u = \lim \leftarrow u_i$ is a homomorphism of the algebra $F$ into the algebra $E$. *Conversely*, for every $A$-algebra homomorphism $v : F \to E$, the family of $v_i = f_i \circ v$ is an inverse system of $A$-algebra homomorphisms such that $v = \lim \leftarrow v_i$. As moreover, writing $\bar{f}_{ij} = \mathrm{Hom}(1_F, f_{ij})$, $(\mathrm{Hom}_{A\text{-alg.}}(F, E_i), \bar{f}_{ij})$ is clearly an inverse system of sets, it is seen that the above remarks can also be expressed by saying that the canonical mapping $v \mapsto (f_i \circ v)$ is a *bijection*

$$
l_F : \mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i).
$$

Moreover, for every $A$-algebra homomorphism $w : F \to F'$, the

$$
\bar{w}_i = \mathrm{Hom}(w, 1_{E_i}) : \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \to \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
$$

form an inverse system of mappings and the diagram

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(F', \lim \leftarrow E_i) & \xrightarrow{l_{F'}} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \\
\downarrow \mathrm{Hom}(w, 1_E) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) & \xrightarrow{l_F} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
\end{array}
$$

is commutative.

Suppose now that $I$ is right *directed*. Consider a direct system of commutative rings $(A_i, \phi_{ji})$ and a direct system $(E_i, f_{ji})$ of $A_i$-modules, with $I$ as indexing set; suppose that each $E_i$ has an $A_i$-algebra structure and that, for $i \leq j$, $f_{ji}$ is an $A_i$-homomorphism of algebras (relative to $\phi_{ji}$) (no. 5). Let $A = \lim \to A_i$, $E = \lim \to E_i$; $E$ has an $A$-module structure, the direct limit of the structures of the $A_i$-modules $E_i$ (II, § 6, no. 2); moreover, the law of composition on E considered as the direct limit of the E_i, considered as magmas under multiplication (I, § 10, no. 3), with the A-module structure on E, defines an A-algebra structure on E; (E_i, f_{ji}) is called a direct system of A_i-algebras and the A-algebra E is called its direct limit. If f_i : E_i \to E, \phi_i : A_i \to A are the canonical mappings, f_i is an A_i-homomorphism of algebras (relative to \phi_i). If the E_i are associative (resp. commutative), so is E; if each E_i admits a unit element e_i and f_{ji}(e_i) = e_j for i \leq j, E admits a unit element e such that f_i(e_i) = e for all i \in I.

Let (E'_i, f'_{ji}) be another direct system of A_i-algebras and for all i let u_i : E_i \to E'_i be an A_i-algebra homomorphism, these mappings forming a direct system; then u = \lim \to u_i is an A-algebra homomorphism.

Suppose now that all the rings A_i are equal to the same ring A and the \phi_{ji} to Id_A, so that E = \lim \to E_i is an A-algebra. Let F be an A-algebra and for all i let u_i : E_i \to F an A-algebra homomorphism such that (u_i) is a direct system of mappings; then u = \lim \to u_i is a homomorphism of the algebra E into the algebra F. Conversely, for every A-algebra homomorphism v : E \to F, the family of v_i = v \circ f_i is a direct system of A-algebra homomorphisms such that v = \lim \to v_i. As moreover, writing \vec{f}_{ij} = \mathrm{Hom}(f_{ij}, 1_F), (\mathrm{Hom}_{A\text{-alg.}}(E_i, F), \vec{f}_{ij}) is clearly an inverse system of sets, it is seen that the above remarks can also be expressed by saying that the canonical mapping v \mapsto (v \circ f_i) is a bijection

d_F : \mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(E_i, F).

Further, for every A-algebra homomorphism w : F \to F', the

\bar{w}_i = \mathrm{Hom}(1_{E_i}, w) : \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \to \mathrm{Hom}_{A\text{-alg.}}(E_i, F')

form an inverse system of mappings and the diagram

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) & \xrightarrow{d_F} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \\
\downarrow \mathrm{Hom}(1_E, w) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F') & \xrightarrow{d_{F'}} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
\end{array}
$$

is commutative.

### 7. BASES OF AN ALGEBRA. MULTIPLICATION TABLE

By definition, a basis of an A-algebra E is a basis of E for its A-module structure. Let (a_i)_{i \in I} be a basis of E; there exists a unique family (\gamma^k_{ij})_{(i, j, k) \in I \times I \times I} of elements of the ring A such that for every ordered pair (i, j) \in I \times I, the set of k \in I such that \gamma^j_{ij} \neq 0 is finite and

$$
a_i a_j = \sum_{k \in I} \gamma^k_{ij} a_k.
$$

The $ \gamma_{ij}^k $ are called the *constants of structure* of the algebra E with respect to the basis $(a_i)$ and relations (7) constitute the *multiplication table* of the algebra E (relative to the basis $(a_i)$).

Relations (7) can be imagined written down by setting out the right hand sides of these relations in a square table

$$
\begin{array}{c|c|c}
 & \cdots & a_j & \cdots \\
\hline
 & & & \\
\vdots & & & \\
\hline
a_j & & \sum_k \gamma_{ij}^k a_k & \\
\vdots & & & \\
\end{array}
$$

it being understood that the element appearing in the row of index $i$ and the column of index $j$ is equal to the product $a_i a_j$.

Conversely, given an *A-module* E, a basis $(a_i)_{i \in I}$ of E and a family $(\gamma_{ij}^k)$ of elements of A such that for every ordered pair $(i, j) \in I \times I$ the set of $k \in I$ such that $\gamma_{ij}^k \neq 0$ is finite, then there is on E one and only one A-algebra structure under which relations (7) hold, since the A-module $E \otimes_A E$ is free and admits as basis $(a_i \otimes a_j)_{(i, j) \in I \times I}$ (cf. II, § 3, no. 7, Corollary 2 to Proposition 7).

Let E be an A-algebra and $(a_i)_{i \in I}$ a generating system of the A-module E (for example a basis). For E to be *associative*, it is necessary and sufficient that the $a_i$ satisfy the *associativity relations*

$$(8)$$
$$(a_i a_j) a_k = a_i (a_j a_k) \quad \text{for all } i, j, k$$

The mapping $(x, y, z) \mapsto (xy)z - x(yz)$ is an A-trilinear mapping
$$
E \times E \times E \to E
$$
and hence defines an A-linear mapping $E \otimes_A E \otimes_A E \to E$; if the latter mapping is zero for all the elements $a_i \otimes a_j \otimes a_k$, which form a generating system of the A-module $E \otimes_A E \otimes_A E$, it is identically zero.

Similarly, for E to be *commutative*, it is necessary and sufficient that the $a_i$ satisfy the *commutativity relations*

$$(9)$$
$$a_i a_j = a_j a_i \quad \text{for all } i, j.$$

The proof is analogous, this time considering the A-bilinear mapping $(x, y) \mapsto xy - yx$. Finally, for an element $e \in E$ to be a unit element, it is necessary and sufficient that the $a_i$ satisfy the relations

$$(10)$$
$$a_i = e a_i = a_i e \quad \text{for all } i,$$

as is seen this time by considering the A-linear mappings $ x \mapsto x - xe $ and $ x \mapsto x - ex $.

When $ (a_i)_{i \in I} $ is a basis of E and $ (\gamma_{ij}^k) $ the corresponding family of constants of structure, relations (8) are equivalent to the relations

$$
\sum_r \gamma_{ij}^r \gamma_{rk}^s = \sum_r \gamma_{ir}^s \gamma_{jk}^r
$$

for all $ i, j, k, s $. Similarly relations (9) are equivalent to $ \gamma_{ij}^k = \gamma_{ji}^k $ for all $ i, j, k $.

Let $ (a_i)_{i \in I} $ be a basis of the A-algebra E; if $ \rho : A \to B $ is a ring homomorphism, $ (a_i \otimes 1) $ is a basis of the B-algebra $ \rho^*(E) = E \otimes_A B $ (II, § 5, no. 1, Proposition 4). If $ (\gamma_{ij}^k) $ is the family of constants of structure relative to the basis $ (a_i) $, the family $ (\rho(\gamma_{ij}^k)) $ is the family of constants of structure of $ \rho^*(E) $ relative to the basis $ (a_i \otimes 1) $.

### Exercises {#alg-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
