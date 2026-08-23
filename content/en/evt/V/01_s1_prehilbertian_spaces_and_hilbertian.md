---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 1
section_title: Prehilbertian spaces and hilbertian spaces
lang: en
source: evt-i-v
pdf_pages: 0259-0275, 0318-0328
extraction: ocr
subsections:
    - "no": 1
      title: Hermitian forms
      page: 0
      pdf_page: 259
    - "no": 2
      title: Positive hermitian forms
      page: 2
      pdf_page: 260
    - "no": 3
      title: Prehilbertian spaces
      page: 4
      pdf_page: 262
    - "no": 4
      title: Hilbertian spaces
      page: 6
      pdf_page: 264
    - "no": 5
      title: Convex subsets of a prehilbertian space
      page: 9
      pdf_page: 267
    - "no": 6
      title: Vector subspaces and orthoprojectors
      page: 12
      pdf_page: 270
    - "no": 7
      title: Dual of a hilbertian space
      page: 15
      pdf_page: 273
statements: 31
exercises: 6
content_sha256: 52ef3981439a9aee715cc1e40006201a012b7b2e455fca13073ea20cf4caa176
---

## § 1. PREHILBERTIAN SPACES AND HILBERTIAN SPACES

### 1. Hermitian forms

We recall the following definition given in Algebra (A, IX, § 3, No. 1):

Definition 1. — Let E be a vector space over the field K. A hermitian form (on the left) on E is a map f from E × E into K satisfying the following conditions (for $ x_1, x_2, x, y_1, y_2, y $ in E and $ \lambda, \mu $ in K):

(1)
$$
\begin{cases}
f(x_1 + x_2, y) = f(x_1, y) + f(x_2, y) \\
f(x, y_1 + y_2) = f(x, y_1) + f(x, y_2)
\end{cases}
$$

(2)
$$
\begin{cases}
f(\lambda x, y) = \overline{\lambda} f(x, y) \\
f(x, \mu y) = \mu f(x, y)
\end{cases}
$$

(3)
$$
f(x, y) = \overline{f(y, x)} .
$$

When the field K is R, the notion of hermitian form on E reduces to that of symmetric bilinear form on E × E (A, III, § 6, No. 3).

We note that the second condition (1) and the second condition (2) follow from the other three.

¹ For the reader specially interested in hilbertian spaces, we point out that only No. 7 of § 1 and No. 8 of § 4 depend on results of chapters III and IV. For this the reader can consult « Summary of some important properties of Banach spaces » which appears at the end of this volume. The only references to chapters I and II concern the definition of a convex set and of a semi-norm (II, p. 1 and p. 7), that of a topological direct sum (I, p. 4), of a total family and a topologically independent family (I, p. 12).

From (1) and (2) we deduce immediately that

$$
f(\sum_j \lambda_j x_j, \sum_k \mu_k y_k) = \sum_{j,k} \overline{\lambda}_j \mu_k f(x_j, y_k).
$$

In particular, if E is finite dimensional, and if $(e_j)_{1 \leq j \leq n}$ is a basis of E, then for $x = \sum_{j=1}^n \xi_j e_j$ and $y = \sum_{j=1}^n \eta_j e_j$, we have,

$$
f(x, y) = \sum_{j,k} \alpha_{jk} \overline{\xi}_j \eta_k
$$

with the notation $\alpha_{jk} = f(e_j, e_k)$; moreover, relation (3) amounts to $\alpha_{jk} = \overline{\alpha}_{kj}$ for every pair of indices $j, k$; this implies in particular that the numbers $\alpha_{jj}$ are real.

From (3), the number $Q(x) = f(x, x)$ is real for all $x \in E$. Moreover, we immediately establish the following formulas, known as *polarization* formulas

(5)
$$
4f(x, y) = \sum_{\varepsilon^2 = 1} \varepsilon Q(x + \varepsilon y) \quad \text{if } K \text{ is } \mathbf{R},
$$
(6)
$$
4f(x, y) = \sum_{\varepsilon^4 = 1, \varepsilon \in \mathbf{C}} \varepsilon Q(x + \overline{\varepsilon} y) \quad \text{if } K \text{ is } \mathbf{C}.
$$

#### Remark {#evt-v-s1-n1-rem-1 .statement}

— We observe that formula (6) is valid for every *sesquilinear* form on $E \times E$ (that is to say, for every function $f$ satisfying (1) and (2), but not necessarily (3)). This remark shows that, when $K = \mathbf{C}$, a sesquilinear form $f$ such that $f(x, x)$ is real for all $x \in E$ is necessarily *hermitian*: relation (6) then gives $\overline{f(y, x)} = f(x, y)$ since we have $y + \varepsilon x = \varepsilon(x + \overline{\varepsilon} y)$ and $Q(\varepsilon z) = Q(z)$ whenever $\varepsilon^4 = 1$.

From the polarisation formulas, we have in particular,

#### Proposition 1 {#evt-v-s1-prop-1 .statement}

*If $f$ is a hermitian form on $E$, and $M$ a vector subspace of $E$ such that $f(x, x) = 0$ for all $x \in M$, then we also have $f(x, y) = 0$ for every pair of points $x, y$ in $M$.*

Let $f$ be a hermitian form on $E$; the set $N$ of all $x \in E$ such that $f(x, y) = 0$ for all $y \in E$ is a vector subspace of $E$. It follows from (3) that, if $x_1 \equiv x_2$ (mod. $N$) and $y_1 \equiv y_2$ (mod. $N$), we have $f(x_1, y_1) = f(x_2, y_2)$; hence, on the quotient space $E/N$ we define a sesquilinear form $f$ by putting $f(\dot{x}, \dot{y}) = f(x, y)$ for all $x \in \dot{x}$ and all $y \in \dot{y}$; it is clear that $f$ is hermitian and that the relation «$f(\dot{x}, \dot{y}) = 0$ for all $\dot{y} \in E/N$» implies $\dot{x} = 0$ in $E/N$, in other words (A, IX) $f$ is separating. We say that $f$ is the *separating* hermitian form *associated* with $f$.

### 2. Positive hermitian forms

#### Definition 2 {#evt-v-s1-def-2 .statement}

*Let $E$ be a vector space over the field $K$. A hermitian form $f$ on $E$ is said to be positive if $f(x, x) \geq 0$ for all $x \in E$.*

It is clear that hermitian forms on a vector space $E$ form a vector space *over the field* $\mathbf{R}$ (but not over the field $\mathbf{C}$, when $K$ is $\mathbf{C}$) : in this space the positive hermitian forms constitute *a pointed convex proper cone* (II, p. 10) as a result of def. 2 and prop. 1.

#### Proposition 2 {#evt-v-s1-prop-2 .statement}

— *If f is a positive hermitian form, we have*

$$
|f(x, y)|^2 \leq f(x, x) \ f(y, y)
$$

*for every x and y in E* (Cauchy-Schwarz inequality).

First assume that we have $ f(y, y) \neq 0 $. For every $ \xi \in \mathbf{K} $, we have

$$
f(y, y) \ f(x + \xi y, x + \xi y) \geq 0
$$

which can be written as

$$
f(x, x) \ f(y, y) - |f(x, y)|^2 + (\xi f(y, y) + \overline{f(x, y)}) (\overline{\xi} f(y, y) + f(x, y)) \geq 0 .
$$

Replacing $ \xi $ by $ -\overline{f(x, y)}/f(y, y) $ in this inequality, we get (7). If $ f(x, x) \neq 0 $, we argue similarly.

Finally, if $ f(x, x) = f(y, y) = 0 $, we have $ f(x + \xi y, x + \xi y) \geq 0 $ for all $ \xi \in \mathbf{K} $, which can be written as

$$
\xi f(x, y) + \overline{\xi} f(x, y) \geq 0 .
$$

Replacing $ \xi $ by $ -\overline{f(x, y)} $ in this inequality, we get $ -2 \ |f(x, y)|^2 \geq 0 $, and therefore $ f(x, y) = 0 $; we again get (7) in this case.

#### Corollary 1 {#evt-v-s1-prop-2-cor-1 .statement}

— *If f is a positive hermitian form, the set N of all x \in E such that f(x, x) = 0 coincides with the vector subspace of all x \in E such that f(x, y) = 0 for all y \in E.*

#### Corollary 2 {#evt-v-s1-prop-2-cor-2 .statement}

— *For a positive hermitian form to be separating, it is necessary and sufficient that the relation x \neq 0 implies f(x, x) > 0.*

This follows immediately from cor. 1.

For every positive hermitian form f on E, the separating hermitian form associated with f (V, p. 2) is evidently a positive hermitian form on E/N.

#### Proposition 3 {#evt-v-s1-prop-3 .statement}

— *Let f be a positive hermitian form on E. Put*

$$
p(x) = f(x, x)^{1/2}
$$

*for all x \in E. Then p is a semi-norm on E, and is a norm if and only if f is separating.*

It is enough to prove the inequality $ p(x + y) \leq p(x) + p(y) $. But we have

$$
f(x + y, x + y) = f(x, x) + f(y, y) + f(x, y) + \overline{f(x, y)}
$$

and, by Cauchy-Schwarz inequality

$$
f(x + y, x + y) \leq f(x, x) + f(y, y) + 2(f(x, x) f(y, y))^{1/2}
$$
$$
= (f(x, x)^{1/2} + f(y, y)^{1/2})^2 .
$$

#### Remark {#evt-v-s1-n2-rem-1 .statement}

— 1) Suppose f is positive and separating, and let x, y be two vectors $ \neq 0 $. The proof of Cauchy-Schwarz inequality shows that, if the two members of (7) are equal, then there exists a scalar $ \xi $ such that $ f(x + \xi y, x + \xi y) = 0 $, hence $ x + \xi y = 0 $, in other words, $ x $ and $ y $ are *linearly dependent*; the converse is immediate. The proof of inequality (8) shows that the equality $ p(x + y) = p(x) + p(y) $ is possible only if $ x $ and $ y $ are linearly dependent; if $ y = \lambda x $, the preceding equality can be written as $ |1 + \lambda| = 1 + |\lambda| $, and implies that $ \lambda $ is *real and positive*.

2) Let $ f $ be a positive hermitian form on $ E $, and let $ E $ be assigned the semi-norm $ x \mapsto f(x, x)^{1/2} $; if $ f $ is the positive, separating hermitian form defined on $ E/N $ associated with $ f $, then the normed space obtained by assigning the norm $ x \mapsto f(\dot{x}, \dot{x})^{1/2} $ to $ E/N $ is the normed space associated with $ E $ (II, p. 5).

#### Definition 3 {#evt-v-s1-def-3 .statement}

*Let $ E $ be a vector space over the field $ K $. A semi-norm $ p $ on $ E $ is said to be prehilbertian if there exists a positive hermitian form $ f $ on $ E $ such that $ p(x) = f(x, x)^{1/2} $ for all $ x \in E $*.

Observe that for a semi-norm $ p $ on $ E $, there exists at most one positive hermitian form $ f $ such that $ p(x) = f(x, x)^{1/2} $ for all $ x \in E $; this follows from the polarization formulas (V, p. 2).

### 3. Prehilbertian spaces

#### Definition 4 {#evt-v-s1-def-4 .statement}

*A prehilbertian space is a set $ E $ with the structure of a vector space over $ K $ and with a positive hermitian form. We say that $ E $ is a real (resp. complex) prehilbertian space when $ K $ is $ \mathbf{R} $ (resp. $ K $ is $ \mathbf{C} $).

#### Example {#evt-v-s1-n3-exa-1 .statement}

— 1) The form $ (\lambda, \mu) \mapsto \overline{\lambda} \mu $ defines a prehilbertian structure on $ K $, said to be *canonical*. When $ K $ is considered as a prehilbertian space, we shall always mean, unless otherwise mentioned that it has this structure.

2) Let $ I $ be an interval (bounded or not) in $ \mathbf{R} $, and let $ E $ be the set of regulated functions (FVR, II, p. 4) defined on $ I $ with values in $ \mathbf{C} $, having compact support. It is clear that $ E $ is a vector space over $ \mathbf{C} $; let $ f $ be the sesquilinear form $ (x, y) \mapsto \int_1^1 \overline{x(t)}\ y(t)\ dt $; it is immediate that $ f $ is a positive hermitian form on $ E $, and hence defines a prehilbertian structure on this space.

3) Let $ n \geqslant 0 $ be an integer. We define a prehilbertian space structure on the space $ K^n $, by means of the hermitian form

$$
(x, y) \mapsto \sum_{j=1}^n \overline{x_j} y_j
$$

(for $ x = (x_1, ..., x_n) $ and $ y = (y_1, ..., y_n) $). When $ K $ is $ \mathbf{R} $, we see that this is just the scalar product of two vectors of $ \mathbf{R}^n $ (GT, VI, § 2, No. 2).

*4) Let $ \ell^2 $ (or $ \ell^2(\mathbf{N}) $) be the set of sequences $ x = (x_n)_{n \in \mathbf{N}} $ of elements of $ K $ such that $ \sum_{n=0}^\infty |x_n|^2 $ is finite. One can show that $ \ell^2 $ is a vector subspace of $ K^\mathbf{N} $ and define a prehilbertian space structure on $ \ell^2 $ by means of the hermitian form $ (x, y) \mapsto \sum_{n=0}^\infty \overline{x_n} y_n $ (cf. V, p. 18).

5) Let $ E $ be a real prehilbertian space, $ f $ the corresponding symmetric bilinear form on $ E $. Let $ E_{(c)} $ be the vector space complexification of $ E $; we identify $ E $ with a subset of $ E_{(c)} $ by the map $ x \mapsto 1 \otimes x $, in such a way that every element of $ E_{(c)} $ can be written uniquely as $ x_1 + ix_2 $ with $ x_1, x_2 $ in $ E $. The map $ f $ extends uniquely to a hermitian form $ f_{(c)} $ on $ E_{(c)} $; we have,

$$
f_{(c)}(x_1 + ix_2, y_1 + iy_2) = f(x_1, y_1) + f(x_2, y_2) + i(f(x_1, y_2) - f(x_2, y_1)) .
$$

In particular, we have
$$
f_{(\mathbf{C})}(x_1 + ix_2, x_1 + ix_2) = f(x_1, x_1) + f(x_2, x_2) \geqslant 0,
$$
hence $ f_{(\mathbf{C})} $ is positive. We say that $ E_{(\mathbf{C})} $, with $ f_{(\mathbf{C})} $ is the *prehilbertian space complexification* of $ E $.

Whenever only one prehilbertian space structure on a vector space $ E $ is under consideration, the value, for a pair $ (x, y) $ of points of $ E $, of the hermitian form which defines the said structure is denoted by $ \langle x|y \rangle_E $ or simply $ \langle x|y \rangle $, if no confusion is likely to arise. This number is called the *scalar product* $ ^1 $ of $ x $ and $ y $ (*scalar square* of $ x $ if $ y = x $). Two vectors $ x, y $ are said to be *orthogonal* if $ \langle x|y \rangle = 0 $. The function $ x \mapsto \|x\| = \langle x|x \rangle^{1/2} $ is a *semi-norm* on the vector space $ E $ (V, p. 3); a prehilbertian space is always considered with this semi-norm assigned to it (and consequently also with the corresponding topology and uniform structure).

With these notations, in a prehilbertian space $ E $, the Cauchy-Schwarz inequality can be written as
$$
|\langle x|y \rangle| \leqslant \|x\| \cdot \|y\|.
$$

Consequently, the scalar product is a *continuous sesquilinear form* on $ E \times E $ (II, p. 5, prop. 4).

In order that $ E $ be Hausdorff, it is necessary and sufficient that $ x \mapsto \|x\| $ is a *norm* on $ E $; in other words, that the hermitian form $ (x, y) \mapsto \langle x|y \rangle $ *is positive and separating*; this is equivalent to saying that *$ 0 $ is the only vector of $ E $, which is orthogonal to itself*.

According to general definitions (S, IV, § 1, No. 5), an isomorphism from a prehilbertian space $ E $ onto a prehilbertian space $ F $ is a bijective linear mapping $ u $ from $ E $ onto $ F $ such that
$$
\langle u(x)|u(y) \rangle = \langle x|y \rangle
$$
for every $ x $ and $ y $ in $ E $. We deduce from this that $ \|u(x)\| = \|x\| $ for all $ x \in E $, and $ u $ is evidently an isomorphism for the topological vector space structures of $ E $ and of $ F $; if $ E $ and $ F $ are Hausdorff, $ u $ is an *isometry* from $ E $ onto $ F $. Conversely, if $ u $ is a bijective linear mapping from $ E $ onto $ F $, such that $ \|u(x)\| = \|x\| $ for all $ x \in E $, the polarization formulas (V, p. 2) show that $ u $ is a prehilbertian space isomorphism from $ E $ onto $ F $.

Let $ E $ be a *complex* prehilbertian space, and $ \langle x|y \rangle $ the scalar product in $ E $. On the set $ E $, we can define a second vector space structure with respect to $ \mathbf{C} $, taking the same law of the additive group and for the law of external composition $ (\lambda, x) \mapsto \overline{\lambda} x $ (A, II, § 1, No. 13) for this vector space structure, $ (x, y) \mapsto \langle y|x \rangle $ is a *positive hermitian*

1 It may happen sometimes that we write $ (x|y) $ for $ \langle y|x \rangle $. Observe that the formula (4) of V, p. 2, takes the following equivalent forms:
$$
\begin{align*}
\langle \sum_i \lambda_i x_i | \sum_j \mu_j y_j \rangle &= \sum_{i,j} \overline{\lambda}_i \mu_j \langle x_i|y_j \rangle. \\
(\sum_i \lambda_i x_i | \sum_j \mu_j y_j) &= \sum_{i,j} \lambda_i \overline{\mu}_j (x_i|y_j).
\end{align*}
$$

form. The prehilbertian space $ \overline{E} $ obtained by assigning this new vector space structure and the new hermitian form to E, is said to be conjugate to E. An isomorphism $ u $ from E onto $ \overline{E} $ is a semi-linear mapping from E onto itself (with respect to the automorphism $ \xi \mapsto \overline{\xi} $ of $ \mathbf{C} $) such that $ \langle u(y)|u(x) \rangle = \langle x|y \rangle $ or $ \langle u(x)|u(y) \rangle = \overline{\langle x|y \rangle} $ (for $ x, y $ in E); such a mapping is said to be a semi-automorphism of the prehilbertian space E.

If E is a prehilbertian space, M a vector subspace of E, the restriction of the scalar product $ \langle x|y \rangle $ to $ M \times M $ is a positive hermitian form on M, which then defines a prehilbertian space structure on M; we say that this structure is induced by the structure of E, or that M is a prehilbertian subspace of E.

### 4. Hilbertian spaces

Definition 5. — *A hilbertian space* (or *Hilbert space*) *is a prehilbertian space which is Hausdorff and complete*. *We say that a norm on a vector space E (over K) is hilbertian if it is prehilbertian, and if the normed space E is complete*.

If E is a hilbertian space and M a closed vector subspace of E, the prehilbertian space structure induced on M is in fact a hilbertian space structure. In this case we say that M, with the induced structure is a *hilbertian subspace* of E.

#### Example {#evt-v-s1-n4-exa-1 .statement}

— 1) The prehilbertian spaces defined in examples 1, 3, 4 of V, p. 4, are hilbertian spaces. On the other hand, the prehilbertian space defined in example 2 is neither Hausdorff, nor complete. The *complexification* of a hilbertian space is a hilbertian space.

\* 2) Let X be a Hausdorff topological space and let $ \mu $ be a positive measure on X. Let $ L^2(X, \mu) $ be the space consisting of equivalence classes, for $ \mu $, of all square $ \mu $-integrable functions on X with values in $ \mathbf{C} $. This is a complex hilbertian space, whose scalar product is given by

$$
\langle f|g \rangle = \int_X \overline{f(x)}\ g(x)\ d\mu(x) .
$$

\* 3) Let $ n \geqslant 1 $ be an integer and let U be an open set in $ \mathbf{R}^n $. Let $ \mu $ be the measure on U induced by the Lebesgue measure on $ \mathbf{R}^n $, and put $ \mathcal{H}^0 = L^2(U, \mu) $. Let $ \mathcal{H}^1 $ denote the space of all functions $ f \in \mathcal{H}^0 $ with the following property; for $ 1 \leqslant i \leqslant n $, there exists a function $ g_i \in \mathcal{H}^\circ $ such that

$$
\int_U g_i(x)\ h(x)\ d\mu(x) = - \int_U f(x)\ D_i h(x)\ d\mu(x)
$$

for every function $ h $ of class $ C^1 $ with compact support in U. The function $ g_i $ is defined uniquely up to equivalence with respect to $ \mu $, and is denoted by $ D_i f $ or $ \partial f / \partial x_i $ (ith partial derivative). By induction on the integer $ s \geqslant 1 $, we define $ \mathcal{H}^s $ as the set of all functions $ f \in \mathcal{H}^1 $ such that $ D_i f \in \mathcal{H}^{s-1} $ for $ 1 \leqslant i \leqslant n $. We define a scalar product on $ \mathcal{H}^s $ by the formula

$$
\langle f|g \rangle = \sum_{k=0}^s \sum_{1 \leqslant i_1 \leqslant \ldots \leqslant i_k \leqslant n} \int \overline{D_{i_1} \ldots D_{i_k} f} \cdot D_{i_1} \ldots D_{i_k} g\ d\mu .
$$

Then $ \mathcal{H}^s $ is a complex hilbertian space, called *Sobolev space* of index s.

\* 4) Let X be a differential variety of class $ C^r $ (with $ r \geqslant 1 $) pure of finite dimension $ n $.

In the vector fibre space $ \Lambda^n T(X) $, let L be the complement of the zero section. For every real number $ \lambda \neq 0 $, the mapping $ u \mapsto \lambda u $ from $ \Lambda^n T(X) $ into itself leaves L stable.

Let $ \alpha $ be a complex number. A complex valued function $ \omega $ on L such that $ \omega(\lambda u) = |\lambda|^{\alpha} \omega(u) $ for $ u \in L $ and any non-zero real number $ \lambda $ is called a density of order $ \alpha $ on X. We say that a density $ \omega $ of order 1 is locally integrable if there exists an open cover $ (U_i)_{i \in I} $ of X, and for every $ i \in I $ a system of coordinates $ \xi_i = (\xi_i^1, ..., \xi_i^n) $ on $ U_i $ and a complex valued function $ f_i $ on $ \xi_i(U_i) $ satisfying the following conditions:

a) The function $ f_i $ is locally integrable on the open set $ \xi_i(U_i) $ of $ \mathbf{R}^n $ with respect to the Lebesgue measure $ \mu $;

b) Let $ x \in U_i $; if $ (\partial_{1,i,x}, ..., \partial_{n,i,x}) $ is the basis of $ T_x X $ associated to the system of coordinates $ (\xi_i', ..., \xi_i^n) $ in $ U_i $ we have
$$
\omega(\partial_{1,i,x} \wedge ... \wedge \partial_{n,i,x}) = f_i(\xi_i^1(x), ..., \xi_i^n(x)) .
$$

Then, there exists one and only one measure $ \tilde{\omega} $ on X such that for every $ i \in I $, the image under $ \xi_i $ of the restriction of $ \tilde{\omega} $ to $ U_i $ is equal to the measure $ f_i \cdot \mu $ (cf. VAR, R, 10.4.3).

Let $ \mathcal{V} $ (resp. $ \mathcal{N} $) be the vector space of measurable densities $ \omega $ of order 1/2 such that the measure associated with the density $ |\omega|^2 $ of order 1 is bounded (resp. null). Let $ \omega_1 $ and $ \omega_2 $ be in $ \mathcal{V} $; then $ \omega = \overline{\omega_1} \omega_2 $ is a density of order 1, and the measure $ \tilde{\omega} $ associated with $ \omega $ is bounded; the number $ \int_X \tilde{\omega} $ depends only on the classes $ \dot{\omega}_1 $ and $ \dot{\omega}_2 $ of $ \omega_1 $ and $ \omega_2 $ modulo $ \mathcal{N} $ and is denoted by $ \langle \omega_1 | \omega_2 \rangle $ or $ \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle $. Then the mapping $ (\dot{\omega}_1, \dot{\omega}_2) \mapsto \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle $ assigns a complex hilbertian space structure to the vector space $ \Omega_{1/2}(X) = \mathcal{V}/\mathcal{N} $.

\* 5) Let D be the open disc with centre 0 and radius 1 in $ \mathbf{C} $. *The Hardy space* $ H^2(D) $ consists of all holomorphic functions $ f : D \to \mathbf{C} $ for which
$$
\sup_{0 < R < 1} \int_0^1 |f(R \cdot e(\theta))|^2 d\theta < + \infty .
$$
If $ f_1 $ and $ f_2 $ belong to $ H^2(D) $, the limit
$$
\langle f_1 | f_2 \rangle = \lim_{R \to 1} \int_0^1 \overline{f_1(R \cdot e(\theta))} \cdot f_2(R \cdot e(\theta)) \, d\theta
$$
exists; the mapping $ (f_1, f_2) \mapsto \langle f_1 | f_2 \rangle $ assigns a complex hilbertian space structure to the vector space $ H^2(D) $.

For a function $ f : D \to \mathbf{C} $ to belong to $ H^2(D) $, it is necessary and sufficient that there exists a sequence $ (a_n)_{n \in \mathbf{N}} $ of complex numbers such that $ \sum_{n=0}^\infty |a_n|^2 < + \infty $ and that
$$
f(z) = \sum_{n=0}^\infty a_n z^n
$$
for all $ z \in D $. Then we have $ \|f\|^2 = \sum_{n=0}^\infty |a_n|^2 $ which gives an isomorphism from $ H^2(D) $ onto the hilbertian space $ \ell^2 $ (V, p. 4).

Every Hausdorff prehilbertian space is isomorphic to an everywhere dense subspace of a hilbertian space determined up to an isomorphism. Precisely :

#### Proposition 4 {#evt-v-s1-prop-4 .statement}

— *Let E be a Hausdorff prehilbertian space, $ \hat{E} $ the normed space completion of E*(GT, IX, § 3, No. 3). The scalar product* $ (x, y) \mapsto \langle x|y \rangle $ *extends by conti*nuity to a positive and separating hermitian form on* $ \hat{E} $, *and defines a hilbertian space structure on* $ \hat{E} $.

The existence of the extension of $ (x, y) \mapsto \langle x|y \rangle $ to $ \hat{E} \times \hat{E} $ follows from the continuity of this sesquilinear form an $ E \times E $ (GT, III, § 6, No. 5, th. 1). Moreover, this extension, which will also be denoted by $ (x, y) \mapsto \langle x|y \rangle $ is a hermitian form and satisfies the relation $ \langle x|x \rangle = \|x\|^2 $, by virtue of the principle of extension of identities ($ \|x\| $ being the norm on $ \hat{E} $ obtained by extending the norm on E by continuity) ; this proves that the relation $ \langle x|x \rangle = 0 $ implies $ x = 0 $ in $ \hat{E} $, hence that the form $ (x, y) \mapsto \langle x|y \rangle $ is positive and separating, and consequently defines a hilbertian space structure on $ \hat{E} $. Q.E.D.

This hilbertian space is said to be the *completion* of the Hausdorff prehilbertian space E.

\* *Example 6*. — Let U be an open subset of $ \mathbf{R}^n $ ($ n \geqslant 1 $). Let $ \mathscr{C}_0^1(\mathrm{U}) $ be the vector space of all functions of class $ \mathrm{C}^1 $ with compact support in U. We define a Hausdorff prehilbertian space structure on $ \mathscr{C}_0^1(\mathrm{U}) $ whose scalar product is given by

$$
\langle f|g \rangle = \sum_{i=1}^{n} \int_{\mathrm{U}} \overline{\mathrm{D}_i f(x)} . \mathrm{D}_i g(x) \, dx .
$$

This prehilbertian space is not complete. Its completion is called the *Dirichlet space* associated with U. \*

#### Corollary {#evt-v-s1-n4-cor-1 .statement}

— *Let V be a vector space over K and f a positive hermitian form on V.*
a) *There exists a Hilbert space E and a linear mapping* $ u : V \to E $ *such that* $ f(x, y) = \langle u(x)|u(y) \rangle $ *for x, y in V, and such that u(V) is dense in E.*
b) *If two pairs* $ (E_i, u_i) $ *satisfy the conditions analogous to a), then there exists a unique isomorphism* $ \phi $ *from the Hilbert space* $ E_1 $ *onto the Hilbert space* $ E_2 $ *such that* $ u_2 = \phi \circ u_1 $.

Let N be the set of all $ x \in V $ such that $ f(x, x) = 0 $. We define a positive and separating hermitian form on the space V/N by $ \langle \dot{x}|\dot{y} \rangle = f(x, y) $ for $ x \in \dot{x} $ and $ y \in \dot{y} $. Let E be the hilbertian space completion of V/N and $ u $ the mapping $ x \mapsto x + N $ from V into E. Then the conditions of *a*) are satisfied.

Under the hypotheses of *b*), N is equal to the kernel of $ u_1 $ and to that of $ u_2 $. Hence there exists a bijective linear mapping $ \phi_0 $ from $ u_1(V) $ onto $ u_2(V) $ such that $ u_2(x) = \phi_0(u_1(x)) $ for all $ x \in V $. We verify immediately that $ \phi_0 $ is an isomorphism of prehilbertian spaces, hence an isometry. Since $ u_i(V) $ is dense in $ E_i $ for $ i = 1, 2 $, $ \phi_0 $ extends uniquely to an isometry $ \phi $ from $ E_1 $ onto $ E_2 $, and *b*) follows.

We say that the hilbertian space E is the *separated completion* of V (for the form *f*).

*Example 7*. — Let G be a group (with unit element 1) and $ \pi $ a homomorphism from G into the group of automorphisms of a complex hilbertian space E ; we say that $ \pi $ is a *unitary representation* of G in E. Let $ a \in E $ ; we put

$$
\phi(x) = \langle a|\pi(x).a \rangle
$$

for all $ x \in G $. Then $ \phi : G \to \mathbf{C} $ is *positive definite*, in other words satisfies the relation :

(PD) For every $ \lambda_1, ..., \lambda_n $ in $ \mathbf{C} $ and $ x_1, ..., x_n $ in $ G $, we have

$$
\sum_{i,j=1}^n \overline{\lambda_i} \lambda_j \phi(x_i^{-1} x_j) \geqslant 0 .
$$

In fact, the first member of (11) is precisely $ \| \sum_{i=1}^n \lambda_i \pi(x_i) . a \| ^2 $.

Conversely, let $ \phi $ be a positive definite function on $ G $. Let $ C^{(G)} $ be the vector space of all functions with finite support on $ G $. We define a hermitian form $ \Phi $ on $ G $ by

$$
\Phi(u, v) = \sum_{x,y \in G} \overline{u(x)} \ v(y) \ \phi(x^{-1} y)
$$

and the relation (PD) expresses the fact that $ \Phi $ is positive. By the corollary of prop. 4, there exists a hilbertian space $ E $ and a linear mapping $ \rho : C^{(G)} \to E $, with a dense image, such that

$$
\Phi(u, v) = \langle \rho(u)|\rho(v) \rangle \quad \text{for} \quad u, v \quad \text{in} \quad C^{(G)} .
$$

For every $ x \in G $, let $ \gamma_x $ be the left translation by $ x $ in $ C^{(G)} $ defined by $ \gamma_x u(y) = u(x^{-1} y) $ for $ u \in C^{(G)} $ and $ y \in G $. We have $ \Phi(\gamma_x u, \gamma_x v) = \Phi(u, v) $. Now apply assertion b) of the corollary of prop. 4 to $ \rho $ and $ \rho \circ \gamma_x $: there exists a unique automorphism $ \pi(x) $ of the hilbertian space $ E $ such that $ \rho \circ \gamma_x = \pi(x) \circ \rho $. We see immediately that $ \pi $ is a homomorphism from $ G $ into the group of automorphisms of $ E $.

Let $ \delta $ be the element of $ C^{(G)} $ defined by $ \delta(1) = 1, \delta(x) = 0 $ for $ x \neq 1 $ in $ G $. We have $ u = \sum_{x \in G} u(x) . \gamma_x \delta $ for all $ u \in C^{(G)} $, and so $ \rho(u) = \sum_{x \in G} u(x) \ \pi(x) . a $ by putting $ a = \rho(\delta) $.

Formulas (12) and (13) imply that $ \phi(x) = \langle a|\pi(x).a \rangle $ for all $ x \in G $. We remark that the set of vectors $ \pi(x).a $ for all $ x \in G $, is total in $ E $.

### 5. Convex subsets of a prehilbertian space

If we calculate $ \| x - y \| ^2 = \langle x - y|x - y \rangle $ and $ \| x + y \| ^2 = \langle x + y|x + y \rangle $ for any two points $ x, y $ of a prehilbertian space $ E $, we immediately get the « identity of the median »

$$
\| \frac{1}{2}(x + y) \| ^2 + \| \frac{1}{2}(x - y) \| ^2 = \frac{1}{2} (\| x \| ^2 + \| y \| ^2 ) .
$$

From this identity we deduce the following proposition :

![Diagram showing sets B', B, and A, with x and y marked within A](https://i.imgur.com/3Q5z5QG.png)

Fig. 1.

#### Proposition 5 {#evt-v-s1-prop-5 .statement}

— Let $ E $ be a prehilbertian space. Let $ d $ be a real number $ > 0 $, $ \delta $ a real number such that $ 0 \leqslant \delta \leqslant d $. Let $ B $ and $ B' $ be subsets of $ E $ defined by $ \| x \| < d $,

$$
\|x\| \leq d + \delta \text{ respectively, and let } A \text{ be a convex set contained in } B' - B. \text{ Then for every pair of points } x, y \text{ of } A, \text{ we have } \|x - y\| \leq \sqrt{12d\delta} \text{ (fig. 1).}
$$
In fact, we have $ \frac{1}{2}(x + y) \in A $, hence $ \left\| \frac{1}{2}(x + y) \right\| \geq d $; hence from (14) we get the inequality
$$
\left\| \frac{1}{2}(x - y) \right\|^2 = \frac{1}{2}(\|x\|^2 + \|y\|^2) - \left\| \frac{1}{2}(x + y) \right\|^2 \leq (d + \delta)^2 - d^2 \leq 3d\delta
$$
from which the proposition follows.

#### Theorem 1 {#evt-v-s1-thm-1 .statement}

*Let E be a prehilbertian space, and H a non-empty convex subset of E such that H is a Hausdorff and complete uniform subspace of E. For every $ x \in E $, there exists a unique point $ p_H(x) $ in H such that $ \|x - p_H(x)\| = \inf_{y \in H} \|x - y\| $. The element $ p_H(x) $ of H is also the unique element a of H satisfying the relation*
$$
\Re \langle x - a | y - a \rangle \leq 0
$$
*for all* $ y \in H $.

![Diagram showing a point x, a point y, and a line segment labeled a + λ(y − a)](https://i.imgur.com/3Q5z5QG.png)

Fig. 2.

Put $ d = \inf_{y \in H} \|x - y\| $, and for every integer $ n > 0 $, let $ H_n $ be the set of points $ y $ of H such that $ \|x - y\| \leq d + n^{-1} $. The set $ H_n $ is closed in H, is convex and non-empty, and its diameter is bounded by $ \sqrt{12 \frac{d}{n}} $ for all large enough $ n $, by prop. 5. The sequence $ (H_n)_{n \geq 1} $ being decreasing, and the set H being Hausdorff and complete it follows that the base of the Cauchy filter $ (H_n)_{n \geq 1} $ converges to a point $ p_H(x) $ of H; we have $ \{ p_H(x) \} = \bigcap_{n \geq 1} H_n $, hence $ p_H(x) $ is the unique point $ a $ of H such that $ \|x - a\| = d $.

1 We recall (GT, VIII, § 1, No. 1) that $ \Re(z) $ denotes the real part of the complex number z; we have $ \Re(z) = z $ if z is real.

Let $ y \in \mathbf{H} $; since $ \mathbf{H} $ is convex, the point $ z(\lambda) = p_{\mathbf{H}}(x) + \lambda(y - p_{\mathbf{H}}(x)) $ of E belongs to $ \mathbf{H} $ for every real number $ \lambda $ such that $ 0 < \lambda < 1 $. Hence we have
$$
\| x - z(\lambda) \|^{2} \geq \| x - p_{\mathbf{H}}(x) \|^{2} \quad \text{for} \quad 0 < \lambda < 1 ,
$$
which gives
$$
\mathcal{R} \langle x - p_{\mathbf{H}}(x)|y - p_{\mathbf{H}}(x) \rangle = \lim_{\lambda \to 0} \frac{1}{2\lambda} \left\{ \| x - p_{\mathbf{H}}(x) \|^{2} - \| x - z(\lambda) \|^{2} \right\} \leq 0 .
$$
Conversely, let $ a $ be a point of $ \mathbf{H} $ such that $ \mathcal{R} \langle x - a|y - a \rangle \leq 0 $ for all $ y \in \mathbf{H} $. For every $ y \in \mathbf{H} $, we have
$$
\| x - y \|^{2} = \| x - a \|^{2} + \| y - a \|^{2} - 2 \mathcal{R} \langle x - a|y - a \rangle \geq \| x - a \|^{2} ,
$$
and so $ \| x - a \| = d $ and finally that $ a = p_{\mathbf{H}}(x) $ follows from the first part of the proof. Q.E.D.

In what follows the mapping $ p_{\mathbf{H}} $ of E in $ \mathbf{H} $ will be called the *projection* from E onto $ \mathbf{H} $. We remark that $ p_{\mathbf{H}}(x) = x $ for all $ x \in \mathbf{H} $.

The first part of th. 1 is valid under more general hypotheses on the space E (V, p. 67, exerc. 31).

The proof of th. 1 establishes, among others, the following property :

#### Corollary 1 {#evt-v-s1-thm-1-cor-1 .statement}

*Let I be a set directed by a filter $ \mathfrak{F} $ and let $ (y_{i})_{i \in I} $ be a family of points of $ \mathbf{H} $. Let $ x \in \mathbf{E} $. Suppose that we have*
$$
\lim_{i, \mathfrak{F}} \| x - y_{i} \| = \inf_{z \in \mathbf{H}} \| x - z \| .
$$
*Then $ y_{i} $ tends to $ p_{\mathbf{H}}(x) $ with respect to the filter $ \mathfrak{F} $.*

#### Corollary 2 {#evt-v-s1-thm-1-cor-2 .statement}

*For every $ x, y $ in $ \mathbf{E} $, we have*
$$
\| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \| \leq \| x - y \| .
$$
*In particular, the mapping $ p_{\mathbf{H}} $ from $ \mathbf{E} $ into $ \mathbf{H} $ is continuous.*

Let $ x, y $ be two points of $ \mathbf{E} $. Put $ a = p_{\mathbf{H}}(x) - x, b = p_{\mathbf{H}}(y) - p_{\mathbf{H}}(x), c = y - p_{\mathbf{H}}(y) $. By formula (15) (V, p. 10) we have $ \mathcal{R} \langle a|b \rangle \geq 0 $ and $ \mathcal{R} \langle c|b \rangle \geq 0 $. We also have $ a + b + c = y - x $, which gives,
$$
\| x - y \|^{2} = \| a + b + c \|^{2} = \| b \|^{2} + \| a + c \|^{2} + 2 \mathcal{R} \langle a|b \rangle + 2 \mathcal{R} \langle c|b \rangle
$$
$$
\geq \| b \|^{2} = \| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \|^{2} .
$$
This proves corollary 2.

#### Proposition 6 {#evt-v-s1-prop-6 .statement}

*Let $ \mathbf{E} $ be a prehilbertian space and let $ \Phi $ be a non-empty, directed decreasing set of non-empty Hausdorff and complete convex subsets of $ \mathbf{E} $. For every $ x \in \mathbf{E} $ and every subset $ \mathbf{H} $ of $ \mathbf{E} $, put $ d(x, \mathbf{H}) = \inf_{z \in \mathbf{H}} \| x - z \| $. In order that the intersection M of the sets H belonging to $ \Phi $ be non-empty, it is necessary and sufficient that there exists $ x_0 $ in E such that $ \sup_{H \in \Phi} d(x_0, H) $ is finite. For every $ x \in E $ we then have
$$
p_M(x) = \lim_{H \in \Phi} p_H(x)
$$
(limit with respect to the directed set $ \Phi $).

If M is non-empty, $ d(x, H) \leq d(x, M) $ for all $ H \in \Phi $ and all $ x \in E $.

Conversely, suppose that there exists a point $ x_0 $ in E and a real number $ C \geq 0 $ such that $ d(x_0, H) \leq C $ for all $ H \in \Phi $. Let $ x \in E $; then
$$
d(x, H) \leq \|x - x_0\| + C \quad \text{for all } H \in \Phi,
$$
hence the number $ d = \sup_{H \in \Phi} d(x, H) $ is finite. Let B be the set of all $ z \in E $ such that $ \|x - z\| \leq d $. Since B is convex and closed in E, the sets $ H \cap B $, for H ranging over $ \Phi $, are convex, Hausdorff and complete. Let $ \varepsilon > 0 $; there exists a set $ H \in \Phi $ such that $ d(x, H) \geq d - \varepsilon $, and if $ \varepsilon < d/2 $, the diameter of $ H \cap B $ is bounded by $ \sqrt{12 \varepsilon (d - \varepsilon)} $ by prop. 5 (V, p. 9). In other words, for all $ H_0 \in \Phi $, the closed sets $ H \cap B $, for $ H \in \Phi $ and $ H \subset H_0 $, form a base of the Cauchy filter on the Hausdorff and complete space $ H_0 $. Hence the intersection of the sets $ H \cap B $ (for $ H \in \Phi $) reduces to a point y. We get $ y \in M $ and $ \|x - y\| = d = d(x, M) $. Since M is closed in $ H_0 $, it is a Hausdorff, convex and complete set in E, and so $ y = p_M(x) $. For every $ H \in \Phi $, we have $ p_H(x) \in H \cap B $, from which we get that $ p_M(x) = \lim_{H \in \Phi} p_H(x) $.

#### Proposition 7 {#evt-v-s1-prop-7 .statement}

*Let E be a Hausdorff prehilbertian space and let $ \Psi $ be a non-empty directed increasing set of non-empty, convex, complete subsets of E. Put $ A = \bigcup_{H \in \Psi} H $ and suppose that the closure N of A is complete. Then N is convex and we have*
$$
p_N(x) = \lim_{H \in \Psi} p_H(x) \text{ for all } x \in E.
$$

It is clear that A is convex, hence its closure N is convex (II, p. 13). With the notations of prop. 6, $ d(x, N) = \inf_{H \in \Psi} d(x, H) $, and consequently $ d(x, N) $ is the limit of $ d(x, H) $ with respect to the section filter of $ \Psi $. Since $ p_H(x) \in H $ and
$$
\lim_{H \in \Psi} \|x - p_H(x)\| = \lim_{H \in \Psi} d(x, H) = d(x, N),
$$
it follows from cor. 1 of V, p. 11 that $ p_H(x) $ tends to the projection $ p_N(x) $ of $ x $ onto N with respect to the section filter of $ \Psi $.

### 6. Vector subspaces and orthoprojectors

Let E be a prehilbertian space. Recall that two vectors $ x $ and $ y $ of E are said to be *orthogonal* if $ \langle x | y \rangle = 0 $; then
$$
\|x + y\|^2 = \|x\|^2 + \|y\|^2
$$
(« Pythagoras’ theorem »).

Let A be a subset of E. We say that a vector x in E is orthogonal to A if it is orthogonal to every vector of A. The set of all vectors orthogonal to A is a closed vector subspace of A, denoted by $ A^\circ $ and called (by abuse of language) the orthogonal of A.

Let A and B be two subsets of E. We say that A and B are orthogonal if every vector of A is orthogonal to every vector of B. This is equivalent to saying that $ A \subset B^\circ $, or that $ B \subset A^\circ $. If E is Hausdorff and if A and B are orthogonal then $ A \cap B $ is empty or reduces to 0 since 0 is the only vector of E orthogonal to itself.

#### Theorem 2 {#evt-v-s1-thm-2 .statement}

*Let E be a prehilbertian space and M a vector subspace of E, which is Hausdorff and complete. Then E is the topological direct sum of M and of $ M^\circ $ the subspace orthogonal to M. The projector from E onto M associated with the decomposition $ E = M \oplus M^\circ $ is the projection $ p_M $ from E onto M defined in th. 1 (V, p. 10).

We first show that $ x - p_M(x) $ belongs to $ M^\circ $ for all $ x \in E $. Let $ y \in M $. For every scalar $ \lambda \in K $, the vector $ p_M(x) + \lambda y $ belongs to M; hence by formula 15 (V, p. 10) we have,

$$
\mathcal{R}(\lambda \langle x - p_M(x)|y \rangle) \leq 0
$$

for all $ \lambda \in K $. If, in particular we take $ \lambda = \overline{\langle x - p_M(x)|y \rangle} $ we conclude that $ \langle x - p_M(x)|y \rangle = 0 $, hence our assertion.

Since M is Hausdorff, 0 is the only vector of M, orthogonal to itself, hence $ M \cap M^\circ = \{0\} $. For every $ x \in E $, we have $ p_M(x) \in M $ and $ x - p_M(x) \in M^\circ $. Consequently, E is the direct sum of M and $ M^\circ $, and $ p_M $ is the projector from E onto M with kernel $ M^\circ $. Since $ p_M $ is a continuous mapping from E into M (V, p. 11, cor. 2), if follows from GT, III, § 6, No. 2 that E is the topological direct sum of M and $ M^\circ $.

#### Corollary {#evt-v-s1-n6-cor-1 .statement}

*Let E be a Hausdorff prehilbertian space and M a finite dimensional vector subspace of E. Then E is the direct sum of M and $ M^\circ $.

Since E is Hausdorff, so is M; since M is finite dimensional, it is complete (I, p. 13). It is therefore enough to apply th. 2.

With the notations of th. 2, we say that $ M^\circ $ is the orthogonal complement of M and that $ p_M $ is the orthoprojector (or the orthogonal projector, or by abuse of language, the projector) from E onto M; if x is a vector of E, the vector $ p_M(x) $ of M is also called the orthogonal projection of x on M. Note that $ p_M $ is a continuous linear mapping from E onto M and that we have $ \|p_M\| = 1 $ by cor. 2 of V, p. 11, except in the case when $ M = \{0\} $ in which case $ p_M = 0 $.

It follows immediately from Pythagoras theorem that the canonical mapping $ \psi $ from $ E/M $ onto $ M^\circ $ deduced from the direct sum decomposition $ E = M \oplus M^\circ $ is isometric if $ E/M $ is assigned the quotient semi-norm from that of E (II, p. 4). We shall always assign that prehilbertian structure to $ E/M $ for which $ \psi $ is an isomorphism of prehilbertian spaces; the quotient semi-norm on $ E/M $ is then deduced from this prehilbertian structure.

We shall often use the preceding results when E is a hilbertian space and M a closed vector subspace of E. In this case, $ M^\circ $ is a closed vector subspace of E, and $ p_{M^\circ} = 1 - p_M $, and $ (M^\circ)^\circ = M $.

#### Proposition 8 {#evt-v-s1-prop-8 .statement}

— Let E be a hilbertian space, M a closed vector subspace of E, I a non-empty ordered directed set and $(M_i)_{i \in I}$ a family of closed vector subspaces of E. We assume that either the mapping $i \mapsto M_i$ is increasing and that M is the closure of $\bigcup_{i \in I} M_i$ or that the mapping $i \mapsto M_i$ is decreasing and that $M = \bigcap_{i \in I} M_i$. Then $p_M(x) = \lim_{i \in I} p_{M_i}(x)$ for all $x \in E$.

Prop. 8 follows immediately from props. 6 (V, p. 11) and 7 (V, p. 12).

#### Proposition 9 {#evt-v-s1-prop-9 .statement}

— Let E be a hilbertian space and M, N two closed vector subspaces of E.

a) The following conditions are equivalent :
(i) $p_M p_N = p_N p_M$;
(ii) if $x \in M$ is orthogonal to $M \cap N$ and if $y \in N$ is orthogonal to $M \cap N$, then x and y are orthogonal;
(iii) every vector of M orthogonal to $M \cap N$ is orthogonal to N;
(iv) $M = (M \cap N) + (M \cap N^\circ)$.

b) If the equivalent conditions of a) are satisfied, we have $p_{M \cap N} = p_M p_N$, the vector subspace $M + N$ of E is closed and we have $p_{M+N} = p_M + p_N - p_M p_N$.

c) We have $p_M p_N = 0$ if and only if M is orthogonal to N. If this is so, then the vector subspace $M + N$ of E is closed, and $p_{M+N} = p_M + p_N$.

Put $L = M \cap N$, $M_1 = M \cap L^\circ$ and $N_1 = N \cap L^\circ$. Condition (ii) implies that $M_1$ and $N_1$ are orthogonal, and (iii) implies that $M_1$ and N are orthogonal. Since we have $N = N_1 + L$ and $M_1$ is orthogonal to L, we have proved the equivalence of (ii) and (iii). If condition (iii) is satisfied, we have $M_1 = M \cap N^\circ$ and since $M = L + M_1$, condition (iv) is satisfied. Conversely, from (iv) we conclude that $M_1 = M \cap N^\circ$ since the subspaces $M \cap N$ and $M \cap N^\circ$ of M are orthogonal, and so $M_1 \subset N^\circ$, that is, the relation (iii).

Assume that condition (iv) is satisfied. It is immediate that $p_N(y) = p_L(y)$ for all $y \in M$ and hence $p_N p_M(x) = p_L p_M(x)$ for all $x \in E$. But, for every $x \in E$, the vector $p_L p_M(x)$ belongs to L, and the vector
$$
x - p_L p_M(x) = (x - p_M(x)) + (p_M(x) - p_L(p_M(x)))
$$
belongs to $M^\circ + L^\circ = L^\circ$; hence we have $p_L p_M(x) = p_L(x)$. Finally, $p_N p_M = p_L p_M = p_L$. Since condition (ii) is equivalent to (iv) and is symmetric in M and N, we also have $p_M p_N = p_L$. Finally we get $p_M p_N = p_N p_M = p_{M \cap N}$ which gives (i).

Conversely, suppose condition (i) is satisfied. Let $x \in M$; we have
$$
p_M(p_N(x)) = p_N(p_M(x)) = p_N(x)
$$
and so $p_N(x) \in M$. We conclude that $x - p_N(x) \in M$, hence $x$ is the sum of an element $p_N(x)$ of $M \cap N$ and an element $x - p_N(x)$ of $M \cap N^\circ$, which gives (iv).

We have proved a) and the first part of b). Assume now that $p_M$ and $p_N$ commute and put $q = p_M + p_N - p_M p_N$; since $p_M$ and $p_N$ are idempotents in the algebra $\mathcal{L}(E)$, so is q; hence (GT, III, § 6, No. 2) the image of q is a closed vector subspace of E.

It is clear that the image of $ q $ is contained in $ M + N $; however, we have $ p_N(x) = x $, hence $ q(x) = x $ for all $ x \in N $; since we also have $ q = p_M + p_N - p_N p_M $, we get $ q(x) = x $ for all $ x \in M $. We conclude that the image of $ q $ is equal to $ M + N $. The orthogonal of $ M + N $ is equal to $ M^\circ \cap N^\circ $, and the kernel of $ q $ obviously contains $ M^\circ \cap N^\circ $, hence $ q = p_{M+N} $. This proves $ b) $.

We have $ p_M p_N = 0 $ if and only if the image $ N $ of $ p_N $ is contained in the kernel $ M^\circ $ of $ p_M $, that is, if and only if $ M $ is orthogonal to $ N $. The rest of the assertion $ c) $ is then a particular case of $ b) $.

#### Remark {#evt-v-s1-n6-rem-1 .statement}

— Let $ E $ be a hilbertian space and $ M, N $ two closed vector subspaces of $ E $. The relation $ M \subset N $ is equivalent to the orthogonality of $ M $ and $ N^\circ $, that is to say, to the relation $ p_M p_{N^\circ} = 0 $ by prop. 9, $ c) $. Since we have $ p_{N^\circ} = 1 - p_N $, we conclude that *the relations* $ M \subset N $ *and* $ p_M = p_M p_N $ *are equivalent* (« the three perpendicular theorem », *cf.* fig. 3).

![Diagram showing subspaces M, N, and projections p_M(x), p_N(x)](https://i.imgur.com/3Q5z5QG.png)

Fig. 3.

### 7. Dual of a hilbertian space

#### Theorem 3 {#evt-v-s1-thm-3 .statement}

*Let $ E $ be a hilbertian space. For every $ x \in E $, let $ x^* $ be the continuous linear form $ y \mapsto \langle x | y \rangle $ on $ E $; the mapping $ x \mapsto x^* $ is a bijective, semi-linear (for the automorphism $ \xi \mapsto \bar{\xi} $) mapping from $ E $ onto its dual $ E' $, and an isometry from the normed space $ E $ onto the normed space $ E' $.*

The mapping $ x \mapsto x^* $ is semi-linear by (2) (V, p. 1) and by virtue of the Cauchy-Schwarz inequality, we have $ \|x^*\| = \sup_{\|y\| \leq 1} |\langle x | y \rangle| = \|x\| $, hence $ x \mapsto x^* $ is an isometry from $ E $ into $ E' $, and in particular, is injective. To complete the proof, we need to prove that for all $ x' \neq 0 $ in $ E' $, there exists $ x \in E $ such that $ x' = x^* $. But the hyperplane $ H = \mathrm{Ker}\, x' $ is closed in $ E $; its orthogonal is a line $ D $. Let $ b $ be a non-zero element of $ D $; the kernel of the linear form $ b^* $ is equal to $ H $ and hence there exists a scalar $ \lambda \neq 0 $ such that $ x' = \lambda \cdot b^* = (\overline{\lambda} \cdot b)^* $. Q.E.D.

The mapping $ x \mapsto x^* $ from $ E $ onto its dual $ E' $ is said to be *canonical*. The inverse mapping from $ E' $ onto $ E $ is also called canonical and is denoted by $ x' \mapsto x'^* $. We have

$$
\langle x | y \rangle = \langle y, x^* \rangle, \quad \langle x, x' \rangle = \langle x'^* | x \rangle
$$

for $ x, y $ in $ E $ and $ x' $ in $ E' $. Also $ (x^*)^* = x $ for $ x \in E $.

When K is $ \mathbf{R} $, the mapping $ x \mapsto x^* $ is linear. We shall transfer the scalar product of E to E' by this mapping. When $ K = \mathbf{C} $, we can consider the mapping $ x \mapsto x^* $ as an isomorphism from the vector space $ \overline{E} $, the conjugate of E onto E' (V, p. 6). We shall transfer the scalar product of $ \overline{E} $ to E' by this mapping.

In the two cases considered, E' is a hilbertian space and we have the formulae

$$
\langle x^*|y^* \rangle = \overline{\langle x|y \rangle}, \quad \langle x'|x' \rangle = \|x'\|^2
$$

for $ x, y $ in E and $ x' $ in E'.

To say that the vector $ x \in E $ is orthogonal to a vector $ y \in E $ is equivalent to saying that the linear form $ x^* \in E' $ is orthogonal to $ y $ in the sense defined in II, p. 41 (this justifies the use of the word « orthogonal » in the two cases). If M is a closed vector subspace of E, the subspace $ M^\circ $ orthogonal to M in E' (II, p. 44) is the image under $ x \mapsto x^* $ of the orthogonal of M in E, defined in V, p. 13 (this justifies the use of the notation $ M^\circ $ in the two cases).

#### Corollary 1 {#evt-v-s1-thm-3-cor-1 .statement}

*In order that the family $ (x_i)_{i \in I} $ of points of a hilbertian space E be total, it is necessary and sufficient that the relations $ \langle x_i|y \rangle = 0 $ for $ y \in E $ and for all indices $ i \in I $ imply that $ y = 0 $.*

In fact, this says that 0 is the only vector of E' which is orthogonal to all the $ x_i $ (II, p. 43 and IV, p. 1).

#### Corollary 2 {#evt-v-s1-thm-3-cor-2 .statement}

*Let E and F be two hilbertian spaces. For $ u \in \mathcal{L}(E; F) $, $ x \in E $ and $ y \in F $, put*

$$
\Phi_u(y, x) = \langle y|u(x) \rangle .
$$

*The mapping $ u \mapsto \Phi_u $ is an isomorphism from the Banach space $ \mathcal{L}(E; F) $ onto the space of all continuous sesquilinear $ ^1 $ forms on $ F \times E $, endowed with the norm*

$$
\|f\| = \sup_{\substack{x \in E, y \in F \\ \|x\| \leq 1, \|y\| \leq 1}} |f(y, x)| .
$$

It is clear that $ \Phi_u $ is sesquilinear and continuous for all $ u \in \mathcal{L}(E; F) $. Conversely, let $ f $ be a continuous sesquilinear form on $ F \times E $. For every $ x \in E $, the mapping $ y \mapsto f(y, x) $ is a continuous linear form on the hilbertian space F. By th. 3, for every $ x \in E $, there exists a unique element $ u(x) $ in F such that $ f(y, x) = \langle u(x)|y \rangle $ for all $ y \in F $. The mapping $ u : x \mapsto u(x) $ from E into F is linear and we have

$$
\begin{align*}
\|f\| &= \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |f(y, x)| = \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |\langle y|u(x) \rangle| \\
&= \sup_{\|x\| \leq 1} \|u(x)\| ;
\end{align*}
$$

hence $ u $ belongs to $ \mathcal{L}(E; F) $, $ f = \Phi_u $ and $ \|u\| = \|f\| $. This proves cor. 2.

$ ^1 $ Recall (A, IX, § 1, No. 5) that a sesquilinear form (on the left) $ f $ on $ F \times E $ is a mapping from $ F \times E $ into K which satisfies relations (1) and (2) of V, p. 1.

The canonical mapping from E into its bidual E'' (IV, p. 14) maps E onto E'', in other words (IV, p. 16), E is a reflexive Banach space. In fact, if E is a real (resp. complex) hilbertian space, the canonical mapping φ from E' onto E is an isomorphism from the normed space E' onto E (resp. onto the conjugate space $ \overline{E} $ of E); applying th. 3 to E (resp. E), we see that every continuous linear form on the normed space E' is of the form $ x' \mapsto \langle \phi(x')|x \rangle = \langle x, x' \rangle $ with $ x \in E $, hence our assertion follows.

As a consequence (IV, p. 17, prop. 6):

#### Theorem 4 {#evt-v-s1-thm-4 .statement}

*In a hilbertian space E, the unit ball is weakly compact.*

#### Proposition 10 {#evt-v-s1-prop-10 .statement}

*If, in a hilbertian space E, a filter $ \mathfrak{F} $ converges weakly to $ x_0 $, and if moreover $ \lim_{\mathfrak{F}} \|x\| = \|x_0\| $, then $ \mathfrak{F} $ converges to $ x_0 $ for the initial topology of E.*

In fact, $ \|x - x_0\|^2 = \|x\|^2 - 2\Re \langle x|x_0 \rangle + \|x_0\|^2 $. Since $ \langle x|x_0 \rangle $ tends to $ \|x_0\|^2 $ with respect to $ \mathfrak{F} $ by hypothesis, and $ \|x\| $ tends to $ \|x_0\| $ with respect to $ \mathfrak{F} $, $ \|x - x_0\| $ tends to 0 with respect to $ \mathfrak{F} $, hence the proposition.

#### Remark {#evt-v-s1-n7-rem-1 .statement}

— If E is a Hausdorff prehilbertian space and $ \hat{E} $ the hilbertian space completion of E, we know (III, p. 16) that the dual E' of E can be identified with the dual of $ \hat{E} $; it then follows from th. 3 (V, p. 15) that every continuous linear form on E can be written in a unique way as $ x \mapsto \langle a|x \rangle $, where $ a \in \hat{E} $.

### Exercises {#evt-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
