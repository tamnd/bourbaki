---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 11
section_title: Graded modules and rings
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0387-0401, 0448-0449
extraction: ocr
subsections:
    - "no": 1
      title: GRADED COMMUTATIVE GROUPS
      page: 0
      pdf_page: 387
    - "no": 2
      title: GRADED RINGS AND MODULES
      page: 0
      pdf_page: 388
    - "no": 3
      title: GRADED SUBMODULES
      page: 0
      pdf_page: 391
    - "no": 4
      title: CASE OF AN ORDERED GROUP OF DEGREES
      page: 0
      pdf_page: 395
    - "no": 5
      title: GRADED TENSOR PRODUCT OF GRADED MODULES
      page: 0
      pdf_page: 398
    - "no": 6
      title: GRADED MODULES OF GRADED HOMOMORPHISMS
      page: 0
      pdf_page: 399
statements: 28
exercises: 1
content_sha256: d4e3ce7cd2b861bb7c9f076b7cfbacdd960d48f097f2e3c7ac86a9264dde8772
---

## § 11. GRADED MODULES AND RINGS

*From no. 2 of this paragraph onwards, $ \Delta $ will denote a commutative monoid (I, § 2, no. 1), written additively, with an identity element denoted by 0.*

### 1. GRADED COMMUTATIVE GROUPS

We are going to translate into another language the definitions concerning direct sums (§ 1, no. 8).

#### Definition 1 {#alg-ii-s11-def-1 .statement}

*Given a commutative group $ G $ written additively and a set $ \Delta $, a graduation of type $ \Delta $ on $ G $ is a family $ (G_\lambda)_{\lambda \in \Delta} $ of subgroups of $ G $, of which $ G $ is the direct sum. The set $ G $, with the structure defined by its group law and its graduation, is called a graded (commutative) group of type $ \Delta $.*

$ \Delta $ is called the *set of degrees* of $ G $. An element $ x \in G $ is called *homogeneous* if it belongs to one of the $ G_\lambda $, *homogeneous of degree* $ \lambda $ if $ x \in G_\lambda $. The element 0 is therefore homogeneous of all degrees; but if $ x \neq 0 $ is homogeneous, it belongs to only one of the $ G_\lambda $; the index $ \lambda $ such that $ x \in G_\lambda $ is then called *the degree of* $ x $ (or sometimes the *weight* of $ x $) and is sometimes denoted by $ \deg(x) $. Every $ y \in G $ may be written uniquely as a sum $ \sum_\lambda y_\lambda $ of homogeneous elements with $ y_\lambda \in G_\lambda $; $ y_\lambda $ is called the *homogeneous component of degree* $ \lambda $ (or simply the *component of degree* $ \lambda $) of $ y $. When the word "weight" is used instead of "degree", the adjective "homogeneous" is replaced by "isobaric".

#### Example {#alg-ii-s11-n1-exa-1 .statement}

(1) Given any commutative monoid $ \Delta $ (with identity element 0) and a commutative group $ G $, a graduation $ (G_\lambda)_{\lambda \in \Delta} $ is defined on $ G $ by taking $ G_0 = G $ and $ G_\lambda = \{0\} $ for $ \lambda \neq 0 $; this graduation is called *trivial*.

(2) Let $ \Delta, \Delta' $ be two sets and $ \rho $ a mapping of $ \Delta $ into $ \Delta' $. Let $ (G_\lambda)_{\lambda \in \Delta} $ be a graduation of type $ \Delta $ on a commutative group $ G $; for $ \mu \in \Delta' $, let $ G'_\mu $ be the sum of the $ G_\lambda $ such that $ \rho(\lambda) = \mu $; clearly $ (G'_\mu)_{\mu \in \Delta'} $ is a graduation of type $ \Delta' $ on $ G $, said to be *derived* from $ (G_\lambda) $ by means of the mapping $ \rho $.

When $ \Delta $ is a commutative group written additively and $ \rho $ the mapping $ \lambda \mapsto -\lambda $ of $ \Delta $ onto itself, $ (G'_\mu) $ is called the *opposite* graduation of $ (G_\lambda) $.

(3) If $ \Delta = \Delta_1 \times \Delta_2 $ is a product of two sets, a graduation of type $ \Delta $ is called a *bigraduation* of types $ \Delta_1, \Delta_2 $. For all $ \lambda \in \Delta_1 $, let $ G'_\lambda = \bigoplus_{\mu \in \Delta_2} G_{\lambda \mu} $ and, for all $ \mu \in \Delta_2 $, let $ G''_\mu = \bigoplus_{\lambda \in \Delta_1} G_{\lambda \mu} $; clearly $ (G'_\lambda)_{\lambda \in \Delta_1} $ is a graduation of type $ \Delta_1 $ and $ (G''_\mu)_{\mu \in \Delta_2} $ a graduation of type $ \Delta_2 $ on $ G $; these graduations are called the *partial graduations* derived from the bigraduation $ (G_{\lambda \mu}) $. Note that $ G_{\lambda \mu} = G'_\lambda \cap G''_\mu $; conversely, if $ (G'_\lambda)_{\lambda \in \Delta_1} $ and $ (G''_\mu)_{\mu \in \Delta_2} $ are two graduations on $ G $ such that $ G $ is the direct sum of the $ G_{\lambda \mu} = G'_\lambda \cap G''_\mu $, these subgroups form a bigraduation of types $ \Delta_1, \Delta_2 $ on $ G $, of which $ (G'_\lambda) $ and $ (G''_\mu) $ are the partial graduations. We leave to the reader the task of generalizing this to the case where $ \Delta $ is a finite product of sets.

(4) Let $ \Delta_0 $ be a commutative monoid written additively, with identity element denoted by 0; let $ I $ be any set and $ \Delta_0^{(I)} = \Delta $ denote the submonoid of the product $ \Delta_0^I $ consisting of the families $ (\lambda_i)_{i \in I} $ of finite support. Let $ \rho : \Delta \to \Delta_0 $ be the surjective (codiagonal) homomorphism of $ \Delta $ into $ \Delta_0 $ defined by $ \rho((\lambda_i)) = \sum_{i \in I} \lambda_i $. From every graduation of type $ \Delta $ a graduation of type $ \Delta_0 $ is derived by means of $ \rho $ (*Example 2*); it is called the *total graduation* associated with the given "multigraduation" of type $ \Delta $.

The definitions and examples of this no. extend immediately to the case where $ G $ is a group which is *not necessarily commutative*; it is simply necessary to replace everywhere the notion of direct sum by that of "restricted sum" (\S 1, no. 6, *Remark*). Note that in this case the $ G_\lambda $ are normal subgroups of $ G $ and that for $ \lambda \neq \mu $ every element of $ G_\lambda $ is permutable with every element of $ G_\mu $.

### 2. GRADED RINGS AND MODULES

#### Definition 2 {#alg-ii-s11-def-2 .statement}

*Given a ring $ A $ and a graduation $ (A_\lambda) $ of type $ \Delta $ on the additive group $ A $, this graduation is said to be compatible with the ring structure on $ A $ if*

$$
A_\lambda A_\mu \subset A_{\lambda + \mu} \quad \text{for all } \lambda, \mu \text{ in } \Delta.
$$

*The ring $ A $ with this graduation is then called a graded ring of type $ \Delta $.*

#### Proposition 1 {#alg-ii-s11-prop-1 .statement}

*If every element of $ \Delta $ is cancellable and $ (A_\lambda) $ is a graduation of type $ \Delta $ compatible with the structure of a ring $ A $, $ A_0 $ is a subring of $ A $ (and in particular $ 1 \in A_0 $).*

As $ A_0 A_0 \subset A_0 $ by definition, it suffices to prove that $ 1 \in A_0 $. Let $ 1 = \sum_{\lambda \in \Delta} e_\lambda $ be the decomposition of 1 into its homogeneous components. If $ x \in A_\mu $, then $ x = x . 1 = \sum_{\lambda \in \Delta} x e_\lambda $; comparing the components of degree $ \mu $, (since $ \mu + \lambda = \mu $ implies $ \lambda = 0 $) $ x = x e_0 $. Since this relation is true for every homogeneous element of $ A $, it is true for all $ x \in A $; in particular $ 1 = 1 . e_0 = e_0 \in A_0 $.

#### Definition 3 {#alg-ii-s11-def-3 .statement}

*Let $ A $ be a graded ring of type $ \Delta $, $ (A_\lambda) $ its graduation and $ M $ a left (resp. right) $ A $-module; a graduation $ (M_\lambda) $ of type $ \lambda $ on the additive group $ M $ is compatible with the $ A $-module structure on $ M $ if*

(2)
$$
A_\lambda M_\mu \subset M_{\lambda + \mu} \quad (\text{resp. } M_\mu A_\lambda \subset M_{\lambda + \mu})
$$
*for all $ \lambda, \mu $ in $ \Delta $. The module $ M $ with this graduation is then called a left (resp. right) graded module of type $ \Delta $ over the graded ring $ A $.*

When the elements of $ \Delta $ are cancellable, it follows from (2) and Proposition 1 that the $ M_\lambda $ are $ A_0 $-modules.

Clearly if $ A $ is a graded ring of type $ \Delta $, the left $ A $-module $ A_s $ (resp. the right $ A $-module $ A_d $) is graded of type $ \Delta $.

#### Example {#alg-ii-s11-n2-exa-1 .statement}

(1) On any ring $ A $ the trivial graduation of type $ \Delta $ is compatible with the ring structure. If $ A $ is graded by the trivial graduation, for a graduation $ (M_\lambda) $ of type $ \Delta $ on an $ A $-module $ M $ to be compatible with the $ A $-module structure, it is necessary and sufficient that the $ M_\lambda $ be *submodules* of $ M $.

(2) Let $ A $ be a graded ring of type $ \Delta $, $ M $ a graded $ A $-module of type $ \Delta $ and $ \rho $ a homomorphism of $ \Delta $ into a commutative monoid $ \Delta' $ whose identity element is denoted by 0. Then $ A $ is a graded ring of type $ \Delta' $ and $ M $ a graded module of type $ \Delta' $ for the graduations of type $ \Delta' $ derived from $ \rho $ and the graduations of type $ \Delta $ on $ A $ and $ M $ by the procedure of no. 1, *Example* 1: this follows immediately from the relation $ \rho(\lambda + \mu) = \rho(\lambda) + \rho(\mu) $.

In particular, if $ \Delta = \Delta_1 \times \Delta_2 $ is a product of two commutative monoids, the projections $ \mathrm{pr}_1 $ and $ \mathrm{pr}_2 $ are homomorphisms and the corresponding graduations are just the *partial graduations* derived from the graduations of type $ \Delta $ (no. 1, *Example* 3); these partial graduations are thus compatible with the ring structure of $ A $ and the module structure of $ M $.

Similarly, if $ \Delta = \Delta_0^{(r)} $ (where $ \Delta_0 $ is a commutative monoid with identity element denoted by 0), the *total graduation* (no. 1, Example 4) of type $ \Delta_0 $ derived from the graduation of type $ \Delta $ on $ A $ (resp. $ M $) by means of the codiagonal homomorphism is compatible with the ring structure on $ A $ (resp. with the module structure on $ M $).

(3) Let $ A $ be a graded ring of type $ \Delta $, $ M $ a graded $ A $-module of type $ \Delta $ and $ \lambda_0 $ an element of $ \Delta $; for all $ \lambda \in \Delta $, let $ M'_\lambda = M_{\lambda + \lambda_0} $ and let $ M' $ be the $ \mathbf{Z} $-module $ \bigoplus_{\lambda \in \Delta} M'_\lambda $. As $ A_\lambda M'_\mu \subset M_{\lambda + \mu + \lambda_0} = M'_{\lambda + \mu} $, $ M' $ is an $ A $-module and the $ M'_\lambda $ form on $ M' $ a graduation of type $ \Delta $ compatible with the $ A $-module structure of $ M' $; the graded $ A $-module $ M' $ of type $ \Delta $ thus defined is said to be obtained by shifting by $ \lambda_0 $ the graduation of $ M $ and it is denoted by $ M(\lambda_0) $. When $ \Delta $ is a group, the underlying $ A $-module of the graded $ A $-module $ M' $ is identified with $ M $.

*(4) Let $ B $ be a commutative ring. The polynomial ring $ B[X] $ in one indeterminate is graded of type $ \mathbf{N} $ by the subgroups $ BX^n $ ($ n \geqslant 0 $) (cf. III, § 2, no. 9 and IV).*

*(5) Let $ B $ be a commutative ring, $ E $ a $ B $-module, $ Q $ a quadratic form on $ E $ and $ C(Q) $ the Clifford algebra of $ Q $ (cf. IX, § 9). The sub-$ B $-modules $ C^+(Q) $ and $ C^-(Q) $ form on $ C(Q) $ a graduation of type $ \mathbf{Z}/2\mathbf{Z} $ compatible with the ring structure on $ C(Q) $.*

#### Remark {#alg-ii-s11-n2-rem-1 .statement}

(1) The graduations most often used are of type $ \mathbf{Z} $ or of type $ \mathbf{Z}^n $; when we speak of graded (resp. bigraded, trigraded, etc.) modules and rings without mentioning the type, it is understood that we mean graduations of type $ \mathbf{Z} $ (resp. $ \mathbf{Z}^2, \mathbf{Z}^3 $, etc.); a graded ring (resp. module) of type $ \mathbf{N} $ is also called a graded ring (resp. module) with positive degrees.

(2) The graded $ \mathbf{Z} $-modules of type $ \Delta $, when $ \mathbf{Z} $ has the trivial graduation, are just the graded commutative groups (whose set of degrees is a commutative monoid) of Definition 1 (no. 1).

#### Definition 4 {#alg-ii-s11-def-4 .statement}

*Let $ A, A' $ be two graded rings of the same type $ \Delta $ and $ (A_\lambda), (A'_\lambda) $ their respective graduations. A ring homomorphism $ h : A \to A' $ is called graded if $ h(A_\lambda) \subset A'_\lambda $ for all $ \lambda \in \Delta $.

Let $ M, M' $ be two graded modules of type $ \Delta $ over a graded ring of type $ \Delta $. Let $ u : M \to M' $ be an $ A $-homomorphism and $ \delta $ an element of $ \Delta $; $ u $ is called graded of degree $ \delta $ if $ u(M_\lambda) \subset M_{\lambda + \delta} $ for all $ \lambda \in \Delta $.

Let $ A $ be a graded ring of type $ \Delta $, $ A' $ a graded ring of type $ \Delta' $ and $ \rho : \Delta \to \Delta' $ a homomorphism. A ring homomorphism $ h : A \to A' $ is called graded if $ h $ is a graded homomorphism of graded rings of type $ \Delta' $ when $ A $ is given the graduation of type $ \Delta' $ derived from its graduation of type $ \Delta $ by means of $ \rho $ (no. 1, Example 2); this therefore means that $ h(A_\lambda) \subset A'_{\rho(\lambda)} $ for all $ \lambda \in \Delta $.

An $ A $-homomorphism $ u : M \to M' $ is called graded if there exists $ \delta \in \Delta $ such that $ u $ is graded of degree $ \delta $. If $ u \neq 0 $ and every element of $ \Delta $ is cancellable, the degree $ \delta $ of $ u $ is then determined uniquely.

If $ h : A \to A', h' : A' \to A'' $ are two graded homomorphisms of graded rings of type $ \Delta $, so is $ h' \circ h : A \to A'' $; for a mapping $ h : A \to A' $ to be a graded ring isomorphism, it is necessary and sufficient that $ h $ be bijective and that $ h $ and the inverse mapping $ h' $ be graded homomorphisms; it also suffices for this that $ h $ be a bijective graded homomorphism. Thus it is seen that graded homomorphisms can be taken as the morphisms of the species of graded ring structure of type $ \Delta $ (*Set Theory*, IV, § 2, no. 1).

Similarly, if $ u : M \to M' $ and $ u' : M' \to M'' $ are two graded homomorphisms of graded A-modules of type $ \Delta $, of respective degrees $ \delta $ and $ \delta' $, $ u' \circ u : M \to M'' $ is a graded homomorphism of degree $ \delta + \delta' $. If $ \delta $ admits an inverse $ -\delta $ in $ \Delta $ and $ u : M \to M' $ is a bijective graded homomorphism of degree $ \delta $, the inverse mapping $ u' : M' \to M $ is a bijective graded homomorphism of degree $ -\delta $. It follows as above that the *graded homomorphisms of degree* 0 can be taken as the morphisms of the species of graded A-module of type $ \Delta $. But a bijective graded homomorphism $ u : M \to N $ of degree $ \neq 0 $ is not a graded A-module isomorphism if $ M $ and $ N $ are non-zero and the elements of $ \Delta $ are cancellable.

#### Example {#alg-ii-s11-n2-exa-2 .statement}

(6) If $ M $ is a graded A-module and $ M(\lambda_0) $ is a graded A-module obtained by shifting (no. 2, *Example 3*), the $ \mathbf{Z} $-linear mapping of $ M(\lambda_0) $ into $ M $ which coincides with the canonical injection on each $ M_{\lambda + \lambda_0} $ is a graded homomorphism of degree $ \lambda_0 $ (which is bijective when $ \Delta $ is a *group*).

(7) If $ a $ is a homogeneous element of degree $ \delta $ belonging to the centre of $ A $, the homothety $ x \mapsto ax $ of any graded A-module $ M $ is a graded homomorphism of degree $ \delta $.

*Remark* (3) A graded A-module $ M $ is called a *graded free A-module* if there exists a basis $ (m_i)_{i \in I} $ of $ M $ consisting of *homogeneous* elements. Suppose it is and $ \Delta $ is a commutative *group*; let $ \lambda_i $ be the degree of $ m_i $ and consider for each $ i $ the shifted A-module $ A(-\lambda_i) $ (no. 2, *Example 3*); if $ e_i $ denotes the element 1 of $ A $ considered as an element *of degree* $ \lambda_i $ in $ A(-\lambda_i) $, the A-linear mapping $ u : \bigoplus_{i \in I} A(-\lambda_i) \to M $ such that $ u(e_i) = m_i $ for all $ i $, is a *graded A-module isomorphism*.

Assuming always that $ \Delta $ is a commutative group, now let $ N $ be a graded A-module, $ (n_i)_{i \in I} $ a system of *homogeneous* generators of $ N $ and suppose that $ n_i $ is of degree $ \mu_i $. Then the A-linear mapping $ v : \bigoplus_{i \in I} A(-\mu_i) \to N $ such that $ u(e_i) = n_i $ for all $ i $ is a *surjective graded A-module homomorphism of degree* 0. If $ N $ is a *finitely generated* graded A-module, there is always a finite system of homogeneous generators of $ N $ and hence there is a surjective homomorphism of the above type with $ I $ *finite*.

### 3. GRADED SUBMODULES

#### Proposition 2 {#alg-ii-s11-prop-2 .statement}

*Let A be a graded ring of type $ \Delta $, M a graded A-module of type $ \Delta $, $ (M_\lambda) $ its graduation and N a sub-A-module of M. The following properties are equivalent:*

(a) $ N $ *is the sum of the family* $ (N \cap M_\lambda)_{\lambda \in \Delta} $.
(b) *The homogeneous components of every element of N belong to N*.
(c) $ N $ *is generated by homogeneous elements*.

Every element of N can be written uniquely as a sum of elements of the $ M_\lambda $ and hence it is immediate that (a) and (b) are equivalent and that (a) implies (c). We show that (c) implies (b). Then let $ (x_i)_{i \in I} $ be a family of homogeneous generators $ \neq 0 $ of N and let $ \delta(i) $ be the degree of $ x_i $. Every element of N can be written as $ \sum_i a_i x_i $ with $ a_i \in A $; if $ a_{i,\lambda} $ is the component of $ a_i $ of degree $ \lambda $, the conclusion follows from the relation

$$
\sum_{i \in I} \left( \sum_{\mu \in \Delta} a_{i,\mu} x_i \right) = \sum_{\lambda \in \Delta} \left( \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i \right).
$$

**Remark (1)** In the above notation, the relation $ \sum_{i \in I} a_i x_i = 0 $ is therefore equivalent to the system of relations $ \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i = 0 $. When $ \Delta $ is a group, these relations can be written $ \sum_{i \in I} a_{i,\lambda - \delta(i)} x_i = 0 $.

When a submodule N of M has the equivalent properties stated in Proposition 2, clearly the $ N \cap M_\lambda $ form a graduation compatible with the A-module structure of N, called the *graduation induced* by that on M; N with this graduation is called a *graded submodule* of M.

#### Corollary 1 {#alg-ii-s11-prop-2-cor-1 .statement}

*If N is a graded submodule of M and $ (x_i) $ is a generating system of N, the homogeneous components of the $ x_i $ form a generating system of N.*

#### Corollary 2 {#alg-ii-s11-prop-2-cor-2 .statement}

*If N is a finitely generated submodule of M, N admits a finite generating system consisting of homogeneous elements.*

It suffices to apply Corollary 1 noting that an element of M has only a finite number of homogeneous components $ \neq 0 $.

A graded submodule of $ A_s $ (resp. $ A_d $) is called a *graded left* (resp. *right*) *ideal* of the graded ring A. For every subring B of $ A(B \cap A_\lambda)(B \cap A_\mu) \subset B \cap A_{\lambda+\mu} $; if B is a *graded sub-$\mathbf{Z}$-module* of A, the graduation induced on B by that on A is therefore compatible with the ring structure on B; B is then called a *graded subring* of A.

Clearly if N (resp. B) is a graded sub-A-module of M (resp. a graded subring of A), the canonical injection $ N \to M $ (resp. $ B \to A $) is a graded module homomorphism of degree 0 (resp. a graded ring homomorphism).

If N is a graded submodule of a graded A-module M and $ (M_\lambda)_{\lambda \in \Delta} $ the graduation of M, the submodules $ (M_\lambda + N)/N $ of $ M/N $ form a *graduation* compatible with the structure of this quotient module. For, if $ N_\lambda = M_\lambda \cap N $, $ (M_\lambda + N)/N $ is identified with $ M_\lambda/N_\lambda $ and it follows from Proposition 2 and § 1, no. 6, formula (26) that $ M/N $ is their direct sum. Moreover,

$$
A_\lambda(M_\mu + N) \subset A_\lambda M_\mu + N \subset M_{\lambda+\mu} + N
$$
and hence $ A_\lambda((M_\mu + N)/N) \subset (M_{\lambda+\mu} + N)/N $, which establishes our assertion.

tion. The graduation ((M_\lambda + N)/N)_{\lambda \in \Delta} is called the quotient graduation of that on M by N and the quotient module M/N with this graduation is called the graded quotient module of M by the graded submodule N; the canonical homomorphism M \to M/N is a graded homomorphism of degree 0 for this graduation.

If b is a graded two-sided ideal of A, the quotient graduation on A/b is compatible with the ring structure on A/b; the ring A/b with this graduation is called the quotient graded ring of A by b; the canonical homomorphism A \to A/b is a homomorphism of graded rings for this graduation.

#### Proposition 3 {#alg-ii-s11-prop-3 .statement}

*Let A be a graded ring of type \Delta, M, N two graded A-modules of type \Delta and u: M \to N a graded A-homomorphism of degree \delta. Then:*
(i) Im(u) is a graded submodule of N.
(ii) *If \delta is a regular element of \Delta, Ker(u) is a graded submodule of M.*
(iii) *If \delta = 0, the bijection M/Ker(u) \to Im(u) canonically associated with u is an isomorphism of graded modules.*

Assertion (i) follows immediately from the definitions and Proposition 2(c). If x is an element of M such that u(x) = 0 and x = \sum_\lambda x_\lambda is its decomposition into homogeneous components (where x_\lambda is of degree \lambda), then
$$
\sum_\lambda u(x_\lambda) = u(x) = 0
$$
and u(x_\lambda) is of degree \lambda + \delta; if \delta is regular the relation \lambda + \delta = \mu + \delta implies \lambda = \mu, hence the u(x_\lambda) are the homogeneous components of u(x) and necessarily u(x_\lambda) = 0 for all \lambda \in \Delta, which proves (ii). The bijection v: M/Ker(u) \to Im(u) canonically associated with u is then a graded homomorphism of degree \delta, as follows from the definition of the quotient graduation; whence (iii) when \delta = 0.

#### Corollary {#alg-ii-s11-n3-cor-1 .statement}

*Let A, B be two graded rings of type \Delta and u: A \to B a graded homomorphism of graded rings. Then Im(u) is a graded submodule of B, Ker(u) a graded two-sided ideal of A and the bijection A/Ker(u) \to Im(u) canonically associated with u is an isomorphism of graded rings.*

It suffices to apply Proposition 3 to u considered as a homomorphism of degree 0 of graded \mathbf{Z}-modules.

#### Proposition 4 {#alg-ii-s11-prop-4 .statement}

*Let A be a graded ring of type \Delta and M a graded A-module of type \Delta.*
(i) *Every sum and every intersection of graded submodules of M is a graded submodule.*
(ii) *If x is a homogeneous element of M of degree \mu which is cancellable in \Delta, the annihilator of x is a graded left ideal of A.*
(iii) *If all the elements of \Delta are cancellable, the annihilator of a graded submodule of M is a graded two-sided ideal of A.*

If $(\mathbf{N}_i)$ is a family of graded submodules of $M$, property (c) of Proposition 2 shows that the sum of the $\mathbf{N}_i$ is generated by homogeneous elements and property (b) of Proposition 2 proves that the homogeneous components of every element of $\bigcap_i \mathbf{N}_i$ belongs to $\bigcap_i \mathbf{N}_i$; whence (i).

To prove (ii), it suffices to note that $\operatorname{Ann}(x)$ is the kernel of the homomorphism $a \mapsto ax$ of the $A$-module $A_s$ into $M$ and that this homomorphism is graded of degree $\mu$; the conclusion follows from Proposition 3(ii). Finally (iii) is a consequence of (i) and (ii) for the annihilator of a graded submodule $N$ of $M$ is the intersection of the annihilators of the homogeneous elements of $N$, by virtue of Proposition 2.

#### Remark 2 {#alg-ii-s11-n3-rem-2 .statement}

Let $M$ be a graded $A$-module and $E$ a submodule of $M$; it follows from Proposition 4(i) that there exists a *largest* graded submodule $N'$ of $M$ contained in $E$ and a *smallest* graded submodule $N''$ of $M$ containing $E$; $N'$ is the set of $x \in E$ all of whose homogeneous components belong to $E$ and $N''$ is the submodule of $M$ generated by the homogeneous components of a generating system of $E$.

#### Proposition 5 {#alg-ii-s11-prop-5 .statement}

*Let $A$ be a graded ring of type $\Delta$. If every element of $\Delta$ is cancellable, then, for every homogeneous element $a \in A$, the centralizer of $a$ in $A$ (I, § 1, no. 5) is a graded subring of $A$.*

Suppose that $a$ is of degree $\delta$; let $b = \sum_\lambda b_\lambda$ be an element permutable with $a$, $b_\lambda$ being the homogeneous component of $b$ of degree $\lambda$ for all $\lambda \in \Delta$. Then by hypothesis $\sum_\lambda (ab_\lambda - b_\lambda a) = 0$ and $ab_\lambda - b_\lambda a$ is homogeneous of degree $\lambda + \delta$; as $\delta$ is cancellable, it follows that $ab_\lambda = b_\lambda a$ for all $\lambda$, which proves our assertion.

#### Corollary {#alg-ii-s11-n3-cor-2 .statement}

*If every element of $\Delta$ is cancellable, the centralizer of the graded subring $B$ of $A$ (and in particular the centre of $A$) is a graded subring of $A$.*

It is the intersection of the centralizers of the homogeneous elements of $B$.

Remark (3) *A direct system $(A_\alpha, \phi_{\beta\alpha})$ of graded rings of type $\Delta$ (resp. a direct system $(M_\alpha, f_{\beta\alpha})$ of graded $A_\alpha$-modules of type $\Delta$) is a direct system of rings (resp. $A_\alpha$-modules) such that each $A_\alpha$ (resp. $M_\alpha$) is graded of type $\Delta$ and each $\phi_{\beta\alpha}$ (resp. $f_{\beta\alpha}$) is a *homomorphism of graded rings* (resp. an *$A_\alpha$*-homomorphism of degree 0 of *graded modules*). If $(A^\lambda_\alpha)_{\lambda \in \Delta}$ (resp. $(M^\lambda_\alpha)_{\lambda \in \Delta}$) be the graduation of $A_\alpha$ (resp. $M_\alpha$) and we write

$$
A = \lim_{\longrightarrow} A_\alpha,\quad A^\lambda = \lim_{\longrightarrow} A^\lambda_\alpha \quad (\text{resp. } M = \lim_{\longrightarrow} M_\alpha,\ M^\lambda = \lim_{\longrightarrow} M^\lambda_\alpha),
$$

it follows from § 6, no. 2, Proposition 5 that $(A^\lambda)$ (resp. $(M^\lambda)$) is a graduation of A (resp. M) and it follows from I, § 10, nos. 3 and 4 that this graduation is compatible with the ring structure on A (resp. the A-module structure on M). The graded ring A (resp. graded A-module M) is called the direct limit of the direct system of graded rings $(A_\alpha, \phi_{\beta\alpha})$ (resp. graded modules $(M_\alpha, f_{\beta\alpha})$). If $\phi_\alpha : A_\alpha \to A$ (resp. $f_\alpha : M_\alpha \to M$) is the canonical mapping, $\phi_\alpha$ (resp. $f_\alpha$) is a homomorphism of graded rings (resp. a homomorphism of degree 0 of graded $A_\alpha$-modules).

### 4. CASE OF AN ORDERED GROUP OF DEGREES

An order structure (denoted by $\leq$) on a commutative group $\Delta$ written additively is said to be *compatible* with the group structure if, for all $\rho \in \Delta$, the relation $\lambda \leq \mu$ implies $\lambda + \rho \leq \mu + \rho$. The group $\Delta$ with this order structure is then called an *ordered group*. We shall study these groups in detail in VI, § 1; here we restrict ourselves to the remark that in such a group the relation $\lambda > 0$ implies $\lambda + \mu > \mu$ for all $\mu$, for it implies $\lambda + \mu \geq \mu$ by definition and the relation $\xi + \mu = \mu$ is equivalent to $\xi = 0$.

Let $\Delta$ be an ordered commutative group, A a graded ring of type $\Delta$ and $(A_\lambda)$ its graduation and suppose that the relation $A_\lambda \neq \{0\}$ implies $\lambda \geq 0$; then it follows from the definitions that $\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$ is a *graded two-sided ideal* of A, by virtue of the remark made above.

#### Proposition 6 {#alg-ii-s11-prop-6 .statement}

*Let $\Delta$ be an ordered commutative group, A a graded ring of type $\Delta$, $(A_\lambda)$ its graduation, M a graded A-module of type $\Delta$ and $(M_\lambda)$ its graduation. Suppose that the relation $A_\lambda \neq \{0\}$ implies $\lambda \geq 0$ and that there exists $\lambda_0$ such that $M_{\lambda_0} \neq \{0\}$ and $M_\lambda = \{0\}$ for $\lambda < \lambda_0$. Then, if $\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$, $\mathfrak{I}_0 M \neq M$.*

Let $x$ be a non-zero element of $M_{\lambda_0}$; suppose that $x \in \mathfrak{I}_0 M$. Then $x = \sum_i a_i x_i$, where the $a_i$ are homogeneous elements $\neq 0$ of $\mathfrak{I}_0$ and the $x_i$ homogeneous elements $\neq 0$ of M with $\deg(x) = \deg(a_i) + \deg(x_i)$ for all $i$ (no. 2). But, as $\deg(a_i) > 0$, $\lambda_0 = \deg(a_i) + \deg(x_i) > \deg(x_i)$, which contradicts the hypothesis.

#### Corollary 1 {#alg-ii-s11-prop-6-cor-1 .statement}

*With the hypotheses on $\Delta$ and A of Proposition 6, if M is a finitely generated graded A-module such that $\mathfrak{I}_0 M = M$, then $M = \{0\}$.*

Suppose $M \neq \{0\}$. Let $\lambda_0$ be a minimal element of the set of degrees of a finite generating system of M consisting of homogeneous elements $\neq 0$; then the hypotheses of Proposition 6 would be fulfilled, which implies a contradiction.

#### Corollary 2 {#alg-ii-s11-prop-6-cor-2 .statement}

*With the hypotheses on $\Delta$ and A of Proposition 6, let M be a finitely* generated graded $ \mathbf{A} $-module and $ \mathbf{N} $ a graded submodule of $ \mathbf{M} $ such that $ \mathbf{N} + \mathfrak{J}_0 \mathbf{M} = \mathbf{M} $; then $ \mathbf{N} = \mathbf{M} $.

$ \mathbf{M}/\mathbf{N} $ is a finitely generated graded $ \mathbf{A} $-module and the hypothesis implies that $ \mathfrak{J}_0 . (\mathbf{M}/\mathbf{N}) = \mathbf{M}/\mathbf{N} $; hence $ \mathbf{M}/\mathbf{N} = 0 $.

#### Corollary 3 {#alg-ii-s11-prop-6-cor-3 .statement}

*With the hypotheses on $ \Delta $ and $ \mathbf{A} $ of Proposition 6, let $ u : \mathbf{M} \to \mathbf{N} $ be a graded homomorphism of graded right $ \mathbf{A} $-modules, where $ \mathbf{N} $ is assumed to be finitely generated. If the homomorphism*

$$
u \otimes 1 : \mathbf{M} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) \to \mathbf{N} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

*is surjective, then $ u $ is surjective.*

$ u(\mathbf{M}) $ is a graded submodule of $ \mathbf{N} $ and the $ (\mathbf{A}/\mathfrak{J}_0) $-module

$$
(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

is isomorphic to $ (N \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0))/\mathrm{Im}(u \otimes 1) $ (\S 3, no. 6, Proposition 6). The hypothesis therefore implies $ (N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) = 0 $ and hence $ \mathbf{N} = u(\mathbf{M}) $ by Corollary 1.

#### Remark {#alg-ii-s11-n4-rem-1 .statement}

It follows from the proof of Corollary 1 that Corollaries 1 and 2 (resp. Corollary 3) are still valid when, instead of assuming that $ \mathbf{M} $ (resp. $ \mathbf{N} $) is finitely generated, the following hypothesis is made: there exists a subset $ \Delta^+ $ of $ \Delta $ satisfying the following conditions:

(1) for $ \lambda \notin \Delta^+ $, $ M_\lambda = \{0\} $ (resp. $ N_\lambda = \{0\} $);
(2) every non-empty subset of $ \Delta^+ $ has a least element.

This will be the case if $ \Delta = \mathbf{Z} $ and $ \mathbf{M} $ (resp. $ \mathbf{N} $) is a graded module with *positive* degrees.

#### Proposition 7 {#alg-ii-s11-prop-7 .statement}

*Suppose that $ \Delta = \mathbf{Z} $. With the hypotheses on $ \mathbf{A} $ and $ \mathbf{M} $ of Proposition 6, consider the graded $ \mathbf{A}_0 $-module $ \mathbf{N} = \mathbf{M}/\mathfrak{J}_0 \mathbf{M} $ and suppose the following conditions hold:
(i) each of the $ N_\lambda $ considered as an $ \mathbf{A}_0 $-module admits a basis $ (y_{i\lambda})_{i \in I_\lambda} $;
(ii) the canonical homomorphism $ \mathfrak{J}_0 \otimes_{\mathbf{A}} \mathbf{M} \to \mathbf{M} $ is injective.

Then $ \mathbf{M} $ is a graded free $ \mathbf{A} $-module (no. 2, Remark 3) and, to be precise, if $ x_{i\lambda} $ is an element of $ M_\lambda $ whose image in $ N_\lambda $ is $ y_{i\lambda} $, the family $ (x_{i\lambda})_{(i, \lambda) \in I} $ (where $ I $ is the set the sum of the $ I_\lambda $) is a basis of $ \mathbf{M} $.*

We know (no. 2, *Remark 3*) that there is a graded free $ \mathbf{A} $-module $ \mathbf{L} $ (of graduation $ (L_\lambda) $) and a surjective homomorphism $ p : \mathbf{L} \to \mathbf{M} $ of degree 0 such that $ p(e_{i\lambda}) = x_{i\lambda} $ for all $ (i, \lambda) \in I $ ($ (e_{i\lambda})_{(i, \lambda) \in I} $ being a basis of $ \mathbf{L} $ consisting of homogeneous elements $ e_{i\lambda} \in L_\lambda $). It follows from the above *Remark* that $ p $ is *surjective*. Consider the graded $ \mathbf{A} $-module $ \mathbf{R} = \mathrm{Ker}(p) $ and note that $ R_\lambda = \{0\} $ for $ \lambda < \lambda_0 $ by definition; we need to prove that $ \mathbf{R} = \{0\} $ and by Proposition 6 it will suffice to show that $ \mathfrak{J}_0 R = R $. Consider the commutative diagram (\S 3, no. 6, Proposition 5)

$$
\begin{array}{ccccccccc}
\mathfrak{J}_0 \otimes R & \xrightarrow{1 \otimes j} & \mathfrak{J}_0 \otimes L & \xrightarrow{1 \otimes p} & \mathfrak{J}_0 \otimes M & \longrightarrow & 0 \\
\downarrow a & & \downarrow b & & \downarrow c & & \\
0 & \longrightarrow & R & \xrightarrow{f} & L & \xrightarrow{p} & M & \longrightarrow & 0
\end{array}
$$

where $ j $ is the canonical injection, $ a, b, c $ deriving from the canonical injection $ \mathfrak{J}_0 \to A $ (\S 3, no. 4, Proposition 4); it must be shown that $ a $ is surjective. Note that, as $ L $ is free, $ b $ is injective (\S 3, no. 7, Corollary 6 to Proposition 7) and $ c $ is injective by hypothesis. Then let $ t $ be an element of $ R $ and $ t $ its class in $ R / \mathfrak{J}_0 R $; then there is an exact sequence (\S 3, no. 6, Proposition 5 and Corollary 2 to Proposition 6)

$$
R / \mathfrak{J}_0 R \xrightarrow{j} L / \mathfrak{J}_0 L \xrightarrow{\bar{p}} M / \mathfrak{J}_0 M \longrightarrow 0
$$

where $ j $ and $ \bar{p} $ derive from $ j $ and $ p $ when passing to the quotients and $ \bar{p} $ is by hypothesis a bijection; then $ j(\bar{t}) = 0 $, in other words $ j(t) \in \mathfrak{J}_0 L $. Then there is an element $ z \in \mathfrak{J}_0 \otimes L $ such that $ j(t) = b(z) $; as $ p(b(z)) = 0 $, $ c((1 \otimes p)(z)) = 0 $ and, as $ c $ is injective, $ (1 \otimes p)(z) = 0 $. In other words, $ z $ is the image of an element $ t' \in \mathfrak{J}_0 \otimes R $ under $ 1 \otimes j $ and then $ j(a(t')) = b(z) = j(t) $; as $ j $ is injective, this implies $ t = a(t') $.

We shall show later (Commutative Algebra, II, \S 3, no. 2, Proposition 5) how this proposition can be extended to non-graded modules.

#### Lemma 1 {#alg-ii-s11-lem-1 .statement}

*For a commutative group $ \Delta $ to be such that there exists on $ \Delta $ a total ordering compatible with the group structure of $ \Delta $, it is necessary and sufficient that $ \Delta $ be torsion-free.*

If there exists such an order structure on $ \Delta $ and if $ \lambda > 0 $, then $ \lambda + \mu > 0 $ for all $ \mu \geq 0 $ and in particular, by induction on the integer $ n > 0 $, $ n.\lambda > 0 $, which proves that $ \Delta $ is torsion-free (since every element $ \neq 0 $ of $ \Delta $ is either $ > 0 $ or $ < 0 $). Conversely, if $ \Delta $ is torsion-free, $ \Delta $ is a sub-$ \mathbf{Z} $-module of a vector $ \mathbf{Q} $-space (\S 7, no. 10, Corollary 1 to Proposition 26) which may be assumed of the form $ \mathbf{Q}^{(I)} $; if $ I $ is given a well-ordering (*Set Theory*, III, \S 2, no. 3, Theorem 1) and $ \mathbf{Q} $ its usual ordering, the set $ \mathbf{Q}^{(I)} $ with the *lexicographical ordering* is totally ordered (*Set Theory*, III, \S 2, no. 6); it is immediate that this ordering is compatible with the additive group structure of $ \mathbf{Q}^{(I)} $.

#### Proposition 8 {#alg-ii-s11-prop-8 .statement}

*Let $ \Delta $ be a torsion-free commutative group and $ A $ a graded ring of type $ \Delta $. If the product in $ A $ of two homogeneous elements $ \neq 0 $ is $ \neq 0 $, the ring $ A $ has no divisor of 0.*

Let $ \Delta $ be given a total ordering compatible with its group structure (Lemma

1) and let $ x = \sum_{\lambda \in \Delta} x_\lambda, y = \sum_{\lambda \in \Delta} y_\lambda $ be two non-zero elements of $ A $ ($ x_\lambda $ and $ y_\lambda $ being homogeneous of degree $ \lambda $ for all $ \lambda \in \Delta $); let $ \alpha $ (resp. $ \beta $) be the greatest of the elements $ \lambda \in \Delta $ such that $ x_\lambda \neq 0 $ (resp. $ y_\lambda \neq 0 $); it is immediate that if $ \lambda \neq \alpha $ or $ \mu \neq \beta $, either $ x_\lambda y_\mu = 0 $ or $ \deg(x_\lambda y_\mu) < \alpha + \beta $; the homogeneous component of $ xy $ of degree $ \alpha + \beta $ is therefore $ x_\alpha y_\beta $, which is non-zero by hypothesis; whence $ xy \neq 0 $.

### 5. GRADED TENSOR PRODUCT OF GRADED MODULES

Let $ \Delta $ be a commutative monoid with its identity element denoted by 0, $ A $ a graded ring of type $ \Delta $ and $ M $ (resp. $ N $) a graded right (resp. left) $ A $-module of type $ \Delta $. Let $ (A_\lambda) $ (resp. $ (M_\lambda), (N_\lambda) $) be the graduation of $ A $ (resp. $ M, N $); the tensor product $ M \otimes_{\mathbf{Z}} N $ of the $ \mathbf{Z} $-modules $ M $ and $ N $ is the direct sum of the $ M_\lambda \otimes_{\mathbf{Z}} N_\mu $ (\S 3, no. 7, Proposition 7) and hence the latter form a *bigraduation* of types $ \Delta, \Delta $ on this $ \mathbf{Z} $-module. Consider on $ M \otimes_{\mathbf{Z}} N $ the *total graduation* of type $ \Delta $ associated with this bigraduation (no. 1, *Example 4*); it consists of the sub-$ \mathbf{Z} $-modules $ P_\lambda = \sum_{\mu + \nu = \lambda} (M_\mu \otimes_{\mathbf{Z}} N_\nu) $. It is known that the $ \mathbf{Z} $-module $ M \otimes_A N $ is the quotient of $ M \otimes_{\mathbf{Z}} N $ by the sub-$ \mathbf{Z} $-module $ Q $ generated by the elements $ (xa) \otimes y - x \otimes (ay) $, where $ x \in M, y \in N $ and $ a \in A $ (\S 3, no. 1); if, for all $ \lambda \in \Delta $, $ x_\lambda, y_\lambda, a_\lambda $ are the homogeneous components of degree $ \lambda $ of $ x, y, a $ respectively, clearly $ (xa) \otimes y - x \otimes (zy) $ is the sum of the homogeneous elements $ (x_\lambda a_\nu) \otimes y_\mu - x_\lambda \otimes (a_\nu y_\mu) $, in other words $ Q $ is a *graded* sub-$ \mathbf{Z} $-module of $ M \otimes_{\mathbf{Z}} N $ (no. 3, Proposition 2) and the quotient

$$
M \otimes_A N = (M \otimes_{\mathbf{Z}} N)/Q
$$

therefore has canonically a graded $ \mathbf{Z} $-module structure of type $ \Delta $ (no. 3). Moreover (no. 3, Proposition 5), the *centre* $ C $ of $ A $ is a graded subring of $ A $; the graduation which we have just defined on $ M \otimes_A N $ is *compatible with its module structure over the graded ring* $ C $. For $ M \otimes_{\mathbf{Z}} N $ has canonically *two* $ C $-module structures, for which respectively $ c(x \otimes y) = (xc) \otimes y $ and $ (x \otimes y)c = x \otimes (cy) $ for $ x \in M, y \in N, c \in C $ (\S 3, no. 3); if $ x \in M_\lambda, y \in N_\mu, c \in C \cap A_v $, the two elements $ c(x \otimes y) $ and $ (x \otimes y)c $ belong to $ (M \otimes_{\mathbf{Z}} N)_{\lambda + \mu + v} $ and their difference belongs to $ Q $ and hence their common image in $ M \otimes_A N $ belongs to $ (M \otimes_A N)_{\lambda + \mu + v} $, which establishes our assertion. When we speak of $ M \otimes_A N $ as a *graded* $ C $-*module*, we always mean with the structure thus defined, unless otherwise mentioned. Note that $ (M \otimes_A N)_\lambda $ can be defined as the additive group of $ M \otimes_A N $ generated by the $ x_\mu \otimes y_\nu $, where $ x_\mu \in M_\mu, y_\nu \in N_\nu $ and $ \mu + \nu = \lambda $.

Let $ M' $ (resp. $ N' $) be another graded right (resp. left) $ A $-module and $ u : M \to M', v : N \to N' $ graded homomorphisms of respective degrees $ \alpha $ and $ \beta $. Then it follows immediately from the above remark that $ u \otimes v $ is a *graded* (C-module) homomorphism of degree $ \alpha + \beta $.

When $ A $ is commutative, a graduation (compatible with the $ A $-module structure) is similarly defined on the tensor product of any finite number of graded $ A $-modules; it is moreover immediate that the associativity isomorphisms such as $ (M \otimes N) \otimes P \to M \otimes (N \otimes P) $ ($ \S 3 $, no. 8, Proposition 8) are isomorphisms of *graded* modules.

#### Remark {#alg-ii-s11-n5-rem-1 .statement}

When $ A $ has the *trivial* graduation (no. 1, *Example* 1), $ (M \otimes_A N)_\lambda $ is then simply the direct sum of the sub-$ Y $-modules $ M_\mu \otimes_A N_\nu $ of $ M \otimes_A N $ such that $ \mu + \nu = \lambda $.

Let $ M $ (resp. $ N $) be a graded right (resp. left) $ A $-module of type $ \Delta $, $ P $ a graded $ \mathbf{Z} $-module of type $ \Delta $ and let $ f $ be a $ \mathbf{Z} $-bilinear mapping of $ M \times N $ into $ P $ satisfying condition (1) of $ \S 3 $, no. 1, and such moreover that
$$
f(x_\lambda, y_\mu) \in P_{\lambda+\mu} \quad \text{for } x_\lambda \in M_\lambda, y_\mu \in N_\mu, \lambda, \mu \text{ in } \Delta.
$$
Then $ f(x, y) = g(x \otimes y) $, where $ g : M \otimes_A N \to P $ is a $ \mathbf{Z} $-linear mapping ($ \S 3 $, no. 1, Proposition 1) and it follows from the above condition that $ g $ is a *graded* $ \mathbf{Z} $-module homomorphism of degree 0.

Let $ B $ be another graded ring of type $ \Delta $ and $ \rho : A \to B $ a homomorphism of graded rings (no. 2); then $ \rho^*(B_d) $ is a graded right $ A $-module of type $ \Delta $. If $ E $ is a graded left $ A $-module of type $ \Delta $ and $ \rho^*(B_d) \otimes_A E $ is given the graded $ \mathbf{Z} $-module structure of type $ \Delta $ defined above, the canonical left $ B $-module structure ($ \S 5 $, no. 1) is compatible with the graduation of
$$
E_{(B)} = \rho^*(E) = \rho^*(B_d) \otimes_A E.
$$
The graded $ B $-module thus obtained is said to be obtained by extending the ring of scalars to $ B $ by means of $ \rho $ and when we speak of $ E_{(B)} $ or $ \rho^*(E) $ as a graded $ B $-module, we always mean this structure, unless otherwise mentioned.

### 6. GRADED MODULES OF GRADED HOMOMORPHISMS

We suppose in this no. that the monoid $ \Delta $ is a *group*. Let $ A $ be a graded ring of type $ \Delta $ and $ M, N $ two graded left (for example) $ A $-modules of type $ \Delta $. Let $ H_\lambda $ denote the additive group of *graded homomorphisms of degree* $ \lambda $ of $ M $ into $ N $ (no. 2); in the additive group $ \mathrm{Hom}_A(M, N) $ of *all* homomorphisms of $ M $ into $ N $ (with the *non-graded* $ A $-module structures) the sum (for $ \lambda \in \Delta $) of the $ H_\lambda $ is *direct*. For, if there is a relation $ \sum_\lambda u_\lambda = 0 $ with $ u_\lambda \in H_\lambda $ for all $ \lambda $, it follows that $ \sum_\lambda u_\lambda(x_\mu) = 0 $ for all $ \mu $ and all $ x_\mu \in M_\mu $. As the elements of $ \Delta $ are cancellable, $ u_\lambda(x_\mu) $ is the homogeneous component of $ \sum_\lambda u_\lambda(x_\mu) $ of degree $ \lambda + \mu $; hence $ u_\lambda(x_\mu) = 0 $ for every ordered pair $ (\mu, \lambda) $ and every $ x_\mu \in M_\mu $, which implies $ u_\lambda = 0 $ for all $ \lambda \in \Delta $. We shall denote (in this paragraph) by $ \mathrm{Homgr}_A(M, N) $ the additive subgroup of $ \mathrm{Hom}_A(M, N) $ the sum of the $ H_\lambda $ and we shall call it the additive group of *graded* $ A $-*module homomorphisms* of $ M $ into $ N $. Let $ C $ be the centre of $ A $, which is a graded subring (no. 3, Corollary to Proposition 5); for the canonical $ C $-module structure on $ \mathrm{Hom}_A(M, N) $ ($ \S 1 $, no. 14, *Remark* 1), $ \mathrm{Homgr}_A(M, N) $ is a *submodule* and the graduation $ (H_\lambda) $ is *compatible* with the $ C $-module structure: for, if $ c_v \in C \cap A_v $, $ x_\mu \in N_\mu $ and $ u_\lambda \in H_\lambda $, then by definition $ (c_vu_\lambda)(x_\mu) = c_v.u_\lambda(x_\mu) \subset N_{\lambda+\mu+v} $ and hence $ c_vu_\lambda \in H_{\lambda+v} $.

Let $ M' $ and $ N' $ be two graded left $ A $-modules of type $ \Delta $ and $ u': M' \to M $, $ v': N \to N' $ graded homomorphisms of respective degrees $ \alpha $ and $ \beta $. Then it is immediate that $ \mathrm{Hom}(u', v'): w \mapsto v' \circ w \circ u' $ maps $ \mathrm{Homgr}_A(M, N) $ into $ \mathrm{Homgr}_A(M', N') $ and that its restriction to $ \mathrm{Homgr}_A(M, N) $ is a *graded* homomorphism into $ \mathrm{Homgr}_A(M', N') $ *of degree* $ \alpha + \beta $.

In particular $ \mathrm{Homgr}_A(M, M) $ is a *graded subring* of $ \mathrm{End}_A(M) $, which is denoted by $ \mathrm{Endgr}_A(M) $.

#### Remark {#alg-ii-s11-n6-rem-1 .statement}

If $ M $ and $ N $ are graded left $ A $-modules, $ \mathrm{Homgr}_A(M, N) $ is in general distinct from $ \mathrm{Hom}_A(M, N) $. However these two sets are equal when $ M $ is a *finitely generated* $ A $-module. For $ M $ is then generated by a finite number of homogeneous elements $ x_i $ ($ 1 \leq i \leq n $); let $ d(i) $ be the degree of $ x_i $; let $ u \in \mathrm{Hom}_A(M, N) $ and for all $ \lambda \in \Delta $ let $ z_{i,\lambda} $ denote the homogeneous component of $ u(x_i) $ of degree $ \lambda + d(i) $. We show that there exists a homomorphism $ u_\lambda : M \to N $ such that $ u_\lambda(x_i) = z_{i,\lambda} $ for all $ i $. It suffices to prove that if $ \sum_i a_ix_i = 0 $ with $ a_i \in A $ for $ 1 \leq i \leq n $, then $ \sum_i a_iz_{i,\lambda} = 0 $ for all $ \lambda \in \Delta $ ($ \S 1 $, no. 7, *Remark*). It can be assumed that each $ a_i $ is homogeneous of degree $ d'(i) $ such that $ d(i) + d'(i) = \mu $ for all $ i $ (no. 3, *Remark* 1); then $ \sum_i a_iu(x_i) = 0 $; taking the homogeneous component of degree $ \lambda + \mu $ on the left-hand side, we obtain $ \sum_i a_iz_{i,\lambda} = 0 $, whence the existence of the homomorphism $ u_\lambda $; clearly moreover $ u_\lambda $ is *graded* of degree $ \lambda $. Finally, $ u_\lambda = 0 $ except for a finite number of values of $ \lambda $, and $ u = \sum_\lambda u_\lambda $ by definition, which proves our assertion.

In particular, $ \mathrm{Homgr}_A(A_s, M) = \mathrm{Hom}_A(A_s, M) $ for every graded left $ A $-module $ M $; moreover $ \mathrm{Hom}_A(A_s, M) $ has a *graded left A-module* structure (and not just a graded $ C $-module structure), and it is immediate that with this structure the canonical mapping of $ M $ into $ \mathrm{Hom}_A(A_s, M) $ ($ \S 1 $, no. 14, *Remark* 2) is a *graded A-module isomorphism*.

Similarly, $ \mathrm{Homgr}_A(M, A_s) $ has a *graded right A-module* structure (and not only a graded $ C $-module structure); it is called the *graded dual* of the graded $ A $-module $ M $ and is denoted by $ M^{*\mathrm{gr}} $, or simply $ M^* $ when no confusion results. If $ u : M \to N $ is a graded homomorphism of degree $ \delta $, it follows from the above that the restriction to $ N^{*\mathrm{gr}} $ of $ {}^t u = \mathrm{Hom}(u, 1_{A_s}) $ is a graded homomorphism of the graded dual $ N^{*\mathrm{gr}} $ into the graded dual $ M^{*\mathrm{gr}} $, of degree $ \delta $, called the *graded transpose* of $ u $.

We sometimes consider on the graded dual $ M^{*\mathrm{gr}} $ the graduation derived from the above with the aid of the isomorphism $ \lambda \mapsto -\lambda $ of $ \Delta $ (no. 1, Example 2) so that the homogeneous elements of degree $ \lambda $ in $ M^{*\mathrm{gr}} $ are the graded linear forms *of degree* $ -\lambda $ on $ M $ (when $ A $ has the trivial graduation, these are the zero linear forms of the $ M_\mu $ of index $ \mu \neq \lambda $). Then, if $ u : M \to N $ is a graded homomorphism of degree $ \delta $, $ u' $ becomes a graded homomorphism of degree $ -\delta $.

Suppose $ A $ is *commutative* and graded of type $ \Delta $ and let $ M, N, P, Q $ be four *graded* $ A $-modules of type $ \Delta $. Then there are *canonical graded homomorphisms of degree* 0

(3) $$
\operatorname{Homgr}_A(M, \operatorname{Homgr}_A(N, P)) \to \operatorname{Homgr}_A(M \otimes_A N, P)
$$
(4) $$
\operatorname{Homgr}_A(M, N) \otimes_A P \to \operatorname{Homgr}_A(M, N \otimes_A P)
$$
(5) $$
\operatorname{Homgr}_A(M, P) \otimes_A \operatorname{Homgr}_A(N, Q) \to \operatorname{Homgr}_A(M \otimes_A N, P \otimes_A Q)
$$
(the tensor products being given the graduations defined in no. 5) obtained by restricting the canonical homomorphisms defined in § 4, nos. 1, 2 and 4; for, if $ u : M \to \operatorname{Homgr}_A(N, P) $ is graded of degree $ \delta $, then, for all $ x \in M_\lambda $, $ u(x) $ is a graded homomorphism $ N \to P $ of degree $ \delta + \lambda $ and hence, for $ y \in N_\mu $, $ u(x)(y) \in P_{\delta + \lambda + \mu} $; if $ v : M \otimes_A N \to P $ corresponds canonically to $ u $, it is then seen that $ v $ is a graded homomorphisms of degree $ \delta $, whence our assertion concerning (3); moreover it is seen that this homomorphism is *bijective*. The argument is similar for (4) and (5).

If in particular $ P = Q = A $ in (5), then there is a canonical *graded* homomorphism of degree 0

(6) $$
M^{*\mathrm{gr}} \otimes_A N^{*\mathrm{gr}} \to (M \otimes_A N)^{*\mathrm{gr}}.
$$

### Exercises {#alg-ii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
