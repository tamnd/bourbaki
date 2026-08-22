---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 8
section_title: Complex locally convex spaces
lang: en
source: evt-i-v
book_pages: TVS II.95
pdf_pages: 0097-0102, 0132-0132
extraction: ocr
subsections:
    - "no": 1
      title: Topological vector spaces over $ \mathbf{C} $
      page: 60
      pdf_page: 97
    - "no": 2
      title: Complex locally convex spaces
      page: 62
      pdf_page: 99
    - "no": 3
      title: The Hahn-Banach theorem and its applications
      page: 63
      pdf_page: 100
    - "no": 4
      title: Weak topologies on complex vector spaces
      page: 64
      pdf_page: 101
statements: 10
exercises: 3
content_sha256: f1b6f9a0f20e8a5d426e0afb015b4b18f923029970ed2f6ea81b92b6461e39ff
---

## § 8. COMPLEX LOCALLY CONVEX SPACES

### 1. Topological vector spaces over $ \mathbf{C} $

Let $ E $ be a topological vector space over $ \mathbf{C} $ the field of complex numbers; the topology of $ E $ is also compatible with the structure of the vector space over $ \mathbf{R} $, obtained by restricting the field of scalars to $ \mathbf{R} $. We denote by $ E_0 $ the topological vector space on $ \mathbf{R} $ which *underlies* E (I, p. 2). Note that, in $ E_0 $, the mapping $ x \mapsto ix $ (which is not a homothety) is an *automorphism* $ u $ of the topological vector space structure of $ E_0 $ such that $ u^2(x) = -x $.

Conversely, let F be a topological vector space over $ \mathbf{R} $, and suppose that there exists an automorphism $ u $ of F such that $ u^2 = -1_F $ ($ 1_F $ is the identity automorphism of F). We know (A, IX, § 3, No. 2) that it is then possible to define a vector space structure on F relative to $ \mathbf{C} $ writing $ \lambda x = \alpha x + \beta u(x) $ for all $ \lambda = \alpha + i\beta \in \mathbf{C} $ and all $ x \in F $. Further since the mapping $ (\alpha, \beta, x) \mapsto \alpha x + \beta u(x) $ of $ \mathbf{R}^2 \times F $ in F is continuous the topology of F is compatible with the vector space structure relative to $ \mathbf{C} $ defined above; if E denotes the topological vector space on $ \mathbf{C} $ defined in this manner, then F is the topological vector space on $ \mathbf{R} $ which underlies E.

#### Remark {#evt-ii-s8-n1-rem-1 .statement}

— Given a topological vector space F over $ \mathbf{R} $, it is not always the case that there exists an automorphism $ u $ of F whose square is $ -1_F $; for example, it is not possible to define vector space structure relative to $ \mathbf{C} $ on a vector space over $ \mathbf{R} $ of finite *odd* dimension.

Let E be a topological vector space on $ \mathbf{C} $, and $ E_0 $ the topological vector space on $ \mathbf{R} $ which underlies E. Every linear variety M in E is also a linear variety in $ E_0 $, but the converse is false. To avoid confusion we say that a linear variety for a vector space structure relative to $ \mathbf{C} $ (resp. relative to $ \mathbf{R} $) is a *complex* (resp. *real*) linear variety. A complex linear variety of finite dimension $ n $ (resp. of finite codimension $ n $) is a real linear variety of dimension $ 2n $ (resp. of codimension $ 2n $). In order that a real vector subspace M of E should also be a complex vector subspace, it is necessary and sufficient that $ iM \subset M $.

Recall that, if E and F are two topological vector spaces on $ \mathbf{C} $, then a mapping of E in F is called $ \mathbf{C} $-linear (resp. $ \mathbf{R} $-linear) if it is a linear mapping for the vector space structures of E and of F relative to $ \mathbf{C} $ (resp. $ \mathbf{R} $); every $ \mathbf{C} $-linear mapping is evidently $ \mathbf{R} $-linear but the converse is false. We say that a $ \mathbf{C} $-linear form on E is a *complex* linear form and that an $ \mathbf{R} $-linear form on E (*i.e.* a linear form on $ E_0 $) is a *real* linear form. If $ f $ is a complex linear form on E, it is clear that the real part $ g = \Re f $ and the imaginary part $ h = \Im f $ of $ f $ are real linear forms; further, the relation $ f(ix) = if(x) $ implies the identity $ h(x) = -g(ix) $; in other words we have

$$
f(x) = (\Re f)(x) - i(\Re f)(ix).
$$

Conversely, if $ g $ is a real linear form on E, then $ f(x) = g(x) - ig(ix) $ is the unique complex linear form on E such that $ \Re f = g $; and $ f $ is continuous if, and only if, $ g $ is continuous.

Now let H be a *complex hyperplane* in E, with the equation $ f(x) = \alpha + i\beta $, where $ f $ is a complex linear form on E; putting $ g = \Re f $, we see that H is the intersection of two *real hyperplanes* $ H_1, H_2 $ with equations respectively $ g(x) = \alpha $ and $ g(ix) = -\beta $; if H is *closed*, so also are $ H_1 $ and $ H_2 $ (I, p. 13, th. 1). Conversely let $ H_0 $ be a homogeneous *real* hyperplane, with equation $ g(x) = 0 $ (where $ g $ is a real linear form on E); then H, the intersection of $ H_0 $ and $ iH_0 $, is a homogeneous *complex* hyperplane, and if $ f $ is the complex linear form such that $ \Re f = g $, then $ f(x) = 0 $ is the equation of H; if $ H_0 $ is closed then H also is closed.

Let G be a topological vector space over $ \mathbf{R} $ and let $ G_{(c)} $ be the vector space on $ \mathbf{C} $ obtained from G by extending the field of scalars to $ \mathbf{C} $ (A, II, § 5.1). Identify G as a subset of $ G_{(c)} $ by the mapping $ x \mapsto 1 \otimes x $. The $ \mathbf{R} $-linear mapping $ (x, y) \mapsto x + i.y $ is then a bijection of $ G \times G $ on $ G_{(c)} $, by means of which we transfer the product topology of $ G \times G $ to $ G_{(c)} $. Then $ G_{(c)} $ with this topology is a topological vector space on $ \mathbf{C} $. We say that $ G_{(c)} $ is the *complexified topological vector space of* G.

### 2. Complex locally convex spaces

To say that a subset A of a complex vector space E is *balanced* means that, for all $ x \in A $, we have $ \rho x \in A $ for $ 0 \leq \rho \leq 1 $ and $ e^{i\vartheta}x \in A $ for all real $ \vartheta $.

We say that a set A of E is *convex* if it is convex in the real space $ E_0 $ which underlies E. In order that a convex set $ A \neq \varnothing $ of E be balanced, it is sufficient that $ e^{i\vartheta}A \subset A $ for all real $ \vartheta $; for this implies firstly that $ -A = A $; as A is convex, we see that 0 belongs to A and thus $ \rho A \subset A $ for $ 0 \leq \rho \leq 1 $.

Let E be a complex topological vector space. The smallest balanced convex (resp. closed balanced convex) set containing a set A of E is called the *balanced convex envelope* (resp. *balanced closed convex envelope*) of A; the balanced closed convex envelope of A is the closure of the balanced convex envelope of A. This last is the convex envelope of the union of the sets $ e^{i\vartheta}A $; we can therefore define it as the set of linear sums $ \sum_i \lambda_i x_i $, when $ (x_i) $ is any finite family of points of A, and $ (\lambda_i) $ a family of complex numbers such that $ \sum_i |\lambda_i| \leq 1 $. If A is precompact so also is its balanced envelope (I, p. 6, prop. 3).

We say that a complex topological vector space E is *locally convex* if the real underlying topological vector space $ E_0 $ is locally convex, that is to say if every neighbourhood of 0 in E contains a convex neighbourhood of 0; a topology $ \mathcal{T} $ on E is *locally convex* if it is compatible with the vector space structure of E (relative to $ \mathbf{C} $) and if E, with topology $ \mathcal{T} $, is locally convex. As in this case every closed convex neighbourhood V of 0 contains a balanced neighbourhood W of (I, p. 7, prop. 4), we see that V also contains U, the balanced closed convex envelope of W; in other words the *balanced, closed, convex* neighbourhoods of 0 form a fundamental system of neighbourhoods of 0 in E, invariant under every homothety of ratio $ \neq 0 $.

Conversely, let E be a complex vector space and let $ \mathfrak{S} $ be a filter base on E formed by *absorbent*, *balanced convex* sets. We know then (II, p. 23, prop. 1) that the set $ \mathfrak{B} $, of the transforms of the sets of $ \mathfrak{S} $ by homotheties of ratio $ > 0 $, is a fundamental system of neighbourhoods of 0 for a locally convex topology $ \mathcal{T} $ on the real vector space $ E_0 $ underlying E. Further, as the sets of $ \mathfrak{B} $ are balanced, they are invariant under every homothety $ x \mapsto e^{i\vartheta}x $, which shows that $ \mathcal{T} $ is compatible with the vector space structure of E (over $ \mathbf{C} $) (I, p. 7, prop. 4).

Every locally convex topology on a complex vector space E can be defined by a set of semi-norms, for the gauge of an open balanced convex neighbourhood of 0 is a semi-norm on E.

The ideas and results for real locally convex spaces detailed in II, p. 25 to 36, extend to complex locally convex spaces with no modification other than the replacement of symmetric convex sets by balanced convex sets.

A complex locally convex space is a Fréchet space if it is metrisable and complete.

### 3. The Hahn-Banach theorem and its applications

#### Theorem 1 (Hahn-Banach) {#evt-ii-s8-thm-1 .statement}

— Let V be a vector subspace of E, a complex vector space, and let f be a (complex) linear form on V and p a semi-norm on E such that $ |f(y)| \leq p(y) $ for all $ y \in V $. Then there exists a linear form $ f_1 $ on E extending f and such that $ |f_1(x)| \leq p(x) $ for all $ x \in E $.

For $ g = \Re f $ is a real linear form defined in V and satisfying $ |\cdot(y)| \leq p(y) $ at every point of V; therefore there exists a real linear form $ g_1 $ in E extending g and such that $ |g_1(x)| \leq p(x) $ for all $ x \in E $ (II, p. 23, cor. 1). Let $ f_1(x) = g_1(x) - ig_1(ix) $ be the complex linear form on E of which $ g_1 $ is the real part (II, p. 61). For all real $ \vartheta $

$$
|\Re(e^{i\vartheta}f_1(x))| = |\Re(f_1(e^{i\vartheta}x))| = |g_1(e^{i\vartheta}x)| \leq p(e^{i\vartheta}x) = p(x)
$$

since $ p $ is a semi-norm on the complex space E; this implies the relation $ |f_1(x)| \leq p(x) $, and the theorem is proved.

#### Corollary 1 {#evt-ii-s8-thm-1-cor-1 .statement}

— Let $ x_0 $ be a point of a complex topological vector space E and p be a continuous semi-norm in E; then there exists a continuous (complex) linear form f defined in E, such that $ f(x_0) = p(x_0) $ and $ |f(x)| \leq p(x) $ for all $ x \in E $.

#### Corollary 2 {#evt-ii-s8-thm-1-cor-2 .statement}

— Let V be a vector subspace of a complex locally convex space E and f be a (complex) linear form defined and continuous in V; then there exists a continuous linear form $ f_1 $ defined in E and extending f. If E is normed there exists such a form $ f_1 $ that also satisfies $ \|f_1\| = \|f\| $.

#### Corollary 3 {#evt-ii-s8-thm-1-cor-3 .statement}

— Let M be a finite dimensional vector subspace of a Hausdorff complex locally convex space E. Then there exists a closed vector subspace N of E that is a topological complement of M in E.

The proofs using theorem 1, p. 24 are the same as those of II, p. 23, cor. 2 and cor. 3, p. 24, prop. 2 and p. 25, cor. 2.

#### Proposition 1 {#evt-ii-s8-prop-1 .statement}

— Let A be an open non-empty convex set in a complex topological vector space E and M be a non-empty (complex) linear variety that does not meet A. Then there exists a closed complex hyperplane H that contains M and does not meet A.

We can suppose that $ 0 \in M $. Then there exists a closed real hyperplane $ H_0 $ containing M and not meeting A (II, p. 36; th. 1). As $ M = iM $, the closed complex hyperplane $ H = H_0 \cap (iH_0) $ has the properties required.

#### Corollary {#evt-ii-s8-n3-cor-1 .statement}

— In a complex locally convex space E, every closed complex linear variety M is the intersection of the closed complex hyperplanes which contain it.

In fact, for all $ x \notin M $, there exists a convex open neighbourhood $ V $ of $ x $ that does not meet $ M $, and thus there exists a closed complex hyperplane $ H $ containing $ M $ and not meeting $ V $; *a fortiori* $ H $ does not contain $ x $.

#### Proposition 2 {#evt-ii-s8-prop-2 .statement}

*Let $ A $ be a non-empty balanced open convex set of a complex topological vector space $ E $, and $ B $ be a non-empty convex set that does not meet $ A $. Then there exists a continuous complex linear form $ f $ on $ E $ and a number $ \alpha > 0 $ such that $ |f(x)| < \alpha $ in $ A $ and $ |f(y)| \geq \alpha $ in $ B $.*

For, there exists a continuous *real* linear form $ g $ on $ E $ and a real number $ \alpha $ such that $ g(x) < \alpha $ in $ A $ and $ g(y) \geq \alpha $ in $ B $ (II, p. 37, prop. 1). As $ 0 \in A $, we have $ \alpha > 0 $. We show that the continuous complex linear form $ f(x) = g(x) - ig(ix) $ and the number $ \alpha $ have the properties required. For, since $ \Re f = g $, we have $ |f(y)| \geq \alpha $ in $ B $. On the other hand, for all $ x \in A $ and all real $ \vartheta $, the point $ e^{i\vartheta}x $ belongs to $ A $, since $ A $ is balanced, and we have $ f(x) = e^{-i\vartheta}f(e^{i\vartheta}x) $; then there exists a number $ \vartheta $ such that $ |f(x)| = \Re(e^{i\vartheta}f(x)) = g(e^{i\vartheta}x) < \alpha $, and the proposition follows.

#### Proposition 3 {#evt-ii-s8-prop-3 .statement}

*Let $ A $ be a balanced, closed, convex set in a complex locally convex space $ E $ and let $ K $ be a non-empty compact convex set in $ E $ that does not meet $ A $. Then there exists a continuous complex linear form $ f $ on $ E $ and a number $ \alpha > 0 $ such that $ |f(x)| < \alpha $ in $ A $ and $ |f(y)| > \alpha $ in $ K $.*

The proposition follows from II, p. 38, prop. 4 as prop. 2 follows from II, p. 37, prop. 1.

### 4. Weak topologies on complex vector spaces

The definition and results of II, § 6, Nos. 1 and 2 apply without change to *complex* vector spaces. If $ F $ and $ G $ are two complex vector spaces in duality by a bilinear form $ B $, then the underlying spaces $ F_0 $ and $ G_0 $ are in duality by $ \Re B $, and it follows from II, p. 61, formula (1) that the weak topologies $ \sigma(F, G) $ and $ \sigma(F_0, G_0) $ are identical.

#### Definition 1 {#evt-ii-s8-def-1 .statement}

*Let $ F $ and $ G $ be two complex vector spaces in duality. For any subset $ M $ of $ F $, the polar of $ M $ in $ G $, denoted by $ M^\circ $, is the set of $ y \in G $ such that $ \Re(\langle x, y \rangle) \geq -1 $ for all $ x \in M $.*

If $ M^\circ $ is the polar of $ M \subset F $ in $ G $ then $ (\lambda M)^\circ = \lambda^{-1}M^\circ $ for all $ \lambda \in \mathbf{C}^* $.

If $ M $ is a (complex) vector subspace of $ E $, then $ M^\circ $ is a closed vector subspace (for $ \sigma(G, F) $), since the relation $ \Re(\lambda \langle x, y \rangle) \geq -1 $ for *every* scalar $ \lambda \in \mathbf{C} $ implies $ \langle x, y \rangle = 0 $; again we say that $ M^\circ $ is the subspace of $ G $ *orthogonal* to $ M $.

If $ M $ is a balanced set in $ F $, then $ M^\circ $ is a balanced set in $ G $; in this case $ M^\circ $ is the set of $ y \in G $ such that $ |\langle x, y \rangle| \leq 1 $ for all $ x \in M $; for this relation is equivalent to $ \Re(\langle \zeta x, y \rangle) \leq 1 $ for all $ x \in M $ and all $ \zeta \in \mathbf{C} $ such that $ |\zeta| = 1 $.

The results of II, p. 41 to 51 are also valid without restriction for complex vector spaces.

Exercises

### Exercises {#evt-ii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
