---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 10
section_title: Inverse and direct limits
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0142-0147, 0203-0203
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE SYSTEMS OF MAGMAS
      page: 0
      pdf_page: 142
    - "no": 2
      title: INVERSE LIMITS OF ACTIONS
      page: 0
      pdf_page: 143
    - "no": 3
      title: DIRECT SYSTEMS OF MAGMAS
      page: 0
      pdf_page: 144
    - "no": 4
      title: DIRECT LIMIT OF ACTIONS
      page: 0
      pdf_page: 147
statements: 5
exercises: 2
content_sha256: b08bffa16dc436eeac0e17dcfce948125f5417d3d262e5a26fd8ffccc2df44ff
---

## § 10. INVERSE AND DIRECT LIMITS

Throughout this paragraph, I will denote a non-empty preordered set, $ \alpha \leq \beta $ the preordering on I. The notion of inverse (resp. direct) system of sets relative to the indexing set I is defined in *Set Theory*, III, § 7, no. 1 (resp. *Set Theory*, III, § 7, no. 5, under the hypothesis that I is right directed).

### 1. INVERSE SYSTEMS OF MAGMAS

#### Definition 1 {#alg-i-s10-def-1 .statement}

*An inverse system of magmas relative to the indexing set I is an inverse system of sets* $ (\mathbf{E}_\alpha, f_{\alpha\beta}) $ *relative to I, each* $ \mathbf{E}_\alpha $ *having a magma structure and each* $ f_{\alpha\beta} $ *being a magma homomorphism.*

Let $ (\mathbf{E}_\alpha, f_{\alpha\beta}) $ be an inverse system of magmas whose laws are written multiplicatively. The inverse limit set $ E = \lim_{\leftarrow} \mathbf{E}_\alpha $ is a subset of the product magma $ \prod_{\alpha \in I} \mathbf{E}_\alpha $ consisting of the families $ (x_\alpha)_{\alpha \in I} $ such that $ x_\alpha = f_{\alpha\beta}(x_\beta) $ for $ \alpha \leq \beta $. If $ (x_\alpha) $ and $ (y_\alpha) $ belong to E, then for $ \alpha \leq \beta $, $ x_\alpha = f_{\alpha\beta}(x_\beta) $ and $ y_\alpha = f_{\alpha\beta}(y_\beta) $, hence $ x_\alpha y_\alpha = f_{\alpha\beta}(x_\beta) f_{\alpha\beta}(y_\beta) = f_{\alpha\beta}(x_\beta y_\beta) $; hence E is a submagma of $ \prod_{\alpha \in I} \mathbf{E}_\alpha $. E will be given the law induced by that on $ \prod_{\alpha \in I} \mathbf{E}_\alpha $; the magma obtained is called the

† We avoid the current terminology where positive means $ > 0 $.

inverse limit magma of the magmas $ E_\alpha $. It enjoys the following universal property:

(a) For all $ \alpha \in I $, the canonical mapping $ f_\alpha $ of $ E $ into $ E_\alpha $ is a magma homomorphism of $ E $ into $ E_\alpha $. $ f_\alpha = f_{\alpha \beta} \circ f_\beta $ for $ \alpha \leq \beta $.

(b) Suppose a magma $ F $ is given and homomorphisms $ u_\alpha : F \to E_\alpha $ such that $ u_\alpha = f_{\alpha \beta} \circ u_\beta $ for $ \alpha \leq \beta $. There exists one and only one homomorphism $ u : F \to E $ such that $ u_\alpha = f_\alpha \circ u $ for all $ \alpha \in I $ (namely $ x \mapsto u(x) = (u_\alpha(x))_{\alpha \in I} $).

If the magmas $ E_\alpha $ are associative (resp. commutative), so is $ E $. Suppose that each magma $ E_\alpha $ admits an identity element $ e_\alpha $ and that the homomorphisms $ f_{\alpha \beta} $ are unital. Then $ e = (e_\alpha)_{\alpha \in I} $ belongs to $ E $ for $ e_\alpha = f_{\alpha \beta}(e_\beta) $ for $ \alpha \leq \beta $ and it is an identity element of the magma $ E $; with the above notation, the homomorphisms $ f_\alpha $ are unital and if the $ u_\alpha $ are unital then $ u $ is unital. Further, an element $ x = (x_\alpha)_{\alpha \in I} $ of $ E $ is invertible if and only if each of the $ x_\alpha $ is invertible in the corresponding magma $ E_\alpha $ and $ x^{-1} = (x_\alpha^{-1})_{\alpha \in I} $; this follows from the formula $ f_{\alpha \beta}(x_\beta^{-1}) = f_{\alpha \beta}(x_\beta)^{-1} = x_\alpha^{-1} $ for $ \alpha \leq \beta $.

From these remarks it can be deduced that if the magmas $ E_\alpha $ are monoids (resp. groups) and the $ f_{\alpha \beta} $ are monoid homomorphisms, then the magma $ E $ is a monoid (resp. a group). In this case we speak of an inverse system of monoids (resp. groups). The universal property goes over immediately to this case.

It is left to the reader to define an inverse system of rings $ (E_\alpha, f_{\alpha \beta}) $ and to verify that $ E = \lim \leftarrow E_\alpha $ is a subring of the product ring $ \prod_{\alpha \in I} E_\alpha $, called the inverse limit ring of the rings $ E_\alpha $; it can be verified that the universal property extends to this case.

Let $ \mathfrak{C} = (E_\alpha, f_{\alpha \beta}) $ and $ \mathfrak{C}' = (E'_\alpha, f'_{\alpha \beta}) $ be two inverse systems of magmas (resp. monoids, groups, rings) relative to the same indexing set. A homomorphism of $ \mathfrak{C} $ into $ \mathfrak{C}' $ is an inverse system $ (u_\alpha)_{\alpha \in I} $ of mappings $ u_\alpha : E_\alpha \to E'_\alpha $ such that each $ u_\alpha $ is a homomorphism. Under these conditions, the mapping $ u = \lim \leftarrow u_\alpha $ of $ \lim \leftarrow E_\alpha $ into $ \lim \leftarrow E'_\alpha $ is a homomorphism (cf. Set Theory , III, § 7, no. 2).

### 2. INVERSE LIMITS OF ACTIONS

Suppose there are given two inverse systems of sets $ (\Omega_\alpha, \phi_{\alpha \beta}) $ and $ (E_\alpha, f_{\alpha \beta}) $ relative to the same indexing set $ I $. Suppose there is given for all $ \alpha \in I $ an action of $ \Omega_\alpha $ on $ E_\alpha $ such that

(1)
$$
f_{\alpha \beta}(\omega_\beta x_\beta) = \phi_{\alpha \beta}(\omega_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
for $ \alpha \leq \beta, x_\beta \in E_\beta, \omega_\beta \in \Omega_\beta $. Then the family of actions considered is said to be an inverse system of actions. Let $ \Omega = \lim \leftarrow \Omega_\alpha $ and $ E = \lim \leftarrow E_\alpha $; if $ x = (x_\alpha)_{\alpha \in I} $ belongs to $ E $ and $ \omega = (\omega_\alpha)_{\alpha \in I} $ belongs to $ \Omega $, then $ \omega . x = (\omega_\alpha . x_\alpha)_{\alpha \in I} $ belongs to E by (1). Thus an action of $ \Omega $ on E is defined called the *inverse limit of the actions of the $ \Omega_\alpha $ on the $ E_\alpha $*.

The above applies especially in the case where the $ \Omega_\alpha $ are monoids and each action of $ \Omega_\alpha $ on $ E_\alpha $ is an operation. Then the inverse limit of these operations is an operation of the monoid on E.

It is left to the reader to define the inverse limit of an inverse system of groups with operators and to verify that this limit is a group with operators.

### 3. DIRECT SYSTEMS OF MAGMAS

In this no. and the following we shall assume that I is *right directed*.

#### Definition 2 {#alg-i-s10-def-2 .statement}

*A direct system of magmas relative to the indexing set I is a direct system of sets* $ (E_\alpha, f_{\beta\alpha}) $ *relative to I, each* $ E_\alpha $ *having a magma structure and each* $ f_{\beta\alpha} $ *being a magma homomorphism.*

Let $ (E_\alpha, f_{\beta\alpha}) $ be a direct system of magmas. E will denote the direct limit set $ \lim_{\longrightarrow} E_\alpha $ and $ f_\alpha $ the canonical mapping of $ E_\alpha $ into E. Recall that

(2)
$$
f_\beta \circ f_{\beta\alpha} = f_\alpha \quad \text{for } \alpha \leq \beta,
$$

(3)
$$
E = \bigcup_{\alpha \in I} f_\alpha(E_\alpha).
$$

By (2), also

(4)
$$
f_\alpha(E_\alpha) \subset f_\beta(E_\beta) \quad \text{for } \alpha \leq \beta.
$$

If $ x_\alpha, y_\alpha \in E_\alpha $ are such that $ f_\alpha(x_\alpha) = f_\alpha(y_\alpha) $, there exists a $ \beta \geq \alpha $ such that $ f_{\beta\alpha}(x_\alpha) = f_{\beta\alpha}(y_\alpha) $.

#### Proposition 1 {#alg-i-s10-prop-1 .statement}

*There exists on E one and only one magma structure for which the mappings* $ f_\alpha : E_\alpha \to E $ *are homomorphisms. If the magmas* $ E_\alpha $ *are associative (resp. commutative), so is E. If the magmas* $ E_\alpha $ *and the homomorphism* $ f_{\beta\alpha} $ *are unital, so are the magma* E *and the homomorphisms* $ f_\alpha $.

The magmas $ E_\alpha $ will be written multiplicatively.

Let $ x, y $ be in E. There exist $ \alpha $ in I and $ x_\alpha, y_\alpha $ in $ E_\alpha $ such that $ x = f_\alpha(x_\alpha) $ and $ y = f_\alpha(y_\alpha) $. If there exists a magma structure on E for which $ f_\alpha $ is a homomorphism, then $ x.y = f_\alpha(x_\alpha y_\alpha) $, whence the *uniqueness* of this magma structure.

To prove the existence, we must prove that for $ \alpha, \beta $ in I, $ x_\alpha, y_\alpha $ in $ E_\alpha $ and $ x'_\beta, y'_\beta $ in $ E_\beta $, the relations

(5)
$$
f_\alpha(x_\alpha) = f_\beta(x'_\beta), \qquad f_\alpha(y_\alpha) = f_\beta(y'_\beta)
$$
imply $ f_\alpha(x_\alpha y_\alpha) = f_\beta(x'_\beta y'_\beta) $. For $ \gamma \geq \alpha $ and $ \gamma \geq \beta $, we set $ x_\gamma = f_{\gamma\alpha}(x_\alpha) $, $ y_\gamma = f_{\gamma \alpha}(y_\alpha), x'_\gamma = f_{\gamma \beta}(x'_\beta), y'_\gamma = f_{\gamma \beta}(y'_\beta) $. By the definition of direct limit, there exists $ \gamma $ in $ I $ with $ \gamma \geq \alpha, \gamma \geq \beta, x_\gamma = x'_\gamma, y_\gamma = y'_\gamma $. Then
$$
f_\alpha(x_\alpha y_\alpha) = f_\gamma(f_{\gamma \alpha}(x_\alpha y_\alpha)) = f_\gamma(x_\gamma y_\gamma) = f_\gamma(x'_\gamma y'_\gamma) = f_\gamma(f_{\gamma \beta}(x'_\beta y'_\beta)) \\
= f_\beta(x'_\beta y'_\beta).
$$
Suppose the magmas $ E_\alpha $ are associative. Let $ x, y, z $ be in $ E $. There exist $ \alpha \in I $ and elements $ x_\alpha, y_\alpha, z_\alpha $ in $ E_\alpha $ such that
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad z = f_\alpha(z_\alpha).
$$
Then $ xy = f_\alpha(x_\alpha y_\alpha) $, whence $ (xy)z = f_\alpha((x_\alpha y_\alpha)z_\alpha) $; similarly
$$
x(yz) = f_\alpha(x_\alpha(y_\alpha z_\alpha)),
$$
whence $ (xy)z = x(yz) $ for $ (x_\alpha y_\alpha)z_\alpha = x_\alpha(y_\alpha z_\alpha) $. The case of commutative magmas is treated analogously.

Suppose finally that each magma $ E_\alpha $ has an identity element $ e_\alpha $ and that $ f_{\beta \alpha}(e_\alpha) = e_\beta $ for $ \alpha \leq \beta $. For $ \alpha, \beta $ in $ I $, there exists $ \gamma $ in $ I $ with $ \gamma \geq \alpha $ and $ \gamma \geq \beta $, whence
$$
f_\alpha(e_\alpha) = f_\gamma(f_{\gamma \alpha}(e_\alpha)) = f_\gamma(e_\gamma) = f_\gamma(f_{\gamma \beta}(e_\beta)) = f_\beta(e_\beta)
$$
and there thus exists an element $ e $ in $ E $ such that $ f_\alpha(e_\alpha) = e $ for all $ \alpha \in I $. Let $ x $ be in $ E $; choose $ \alpha \in I $ and $ x_\alpha \in E_\alpha $ such that $ x = f_\alpha(x_\alpha) $. Then
$$
ex = f_\alpha(e_\alpha) \cdot f_\alpha(x_\alpha) = f_\alpha(e_\alpha \cdot x_\alpha) = f_\alpha(x_\alpha) = x
$$
and similarly $ x \cdot e = x $, hence $ e $ is the identity element of $ E $.

The magma $ E $ is called the *direct limit of the magmas* $ E_\alpha $.

#### Proposition 2 {#alg-i-s10-prop-2 .statement}

*Let* $ (E_\alpha, f_{\beta \alpha}) $ *be a direct system of magmas and let* $ E $ *be its direct limits* $ f_\alpha : E_\alpha \to E $ *the canonical homomorphisms. Suppose a magma* $ F $ *and homomorphisms* $ u_\alpha : E_\alpha \to F $ *are given such that* $ u_\alpha = u_\beta \circ f_{\beta \alpha} $ *for* $ \alpha \leq \beta $. *There exists one and only one homomorphism* $ u : E \to F $ *such that* $ u_\alpha = u \circ f_\alpha $ *for all* $ \alpha \in I $. *If the magmas* $ E_\alpha $ *and* $ F $ *and the homomorphisms* $ f_{\beta \alpha} $ *and* $ u_\alpha $ *are unital, the homomorphism* $ u $ *is unital.*

We know (*Set Theory*, III, § 7, no. 6, Proposition 6) that there exists one and only one mapping $ u : E \to F $ such that $ u_\alpha = u \circ f_\alpha $ for all $ \alpha \in I $. We verify that $ u $ is a homomorphism: let $ x, y $ be in $ E $, $ \alpha $ in $ I $ and $ x_\alpha, y_\alpha $ in $ E_\alpha $ such that $ x = f_\alpha(x_\alpha) $ and $ y = f_\alpha(y_\alpha) $. Then $ xy = f_\alpha(x_\alpha y_\alpha) $, whence
$$
u(xy) = u(f_\alpha(x_\alpha y_\alpha)) = u_\alpha(x_\alpha y_\alpha) = u_\alpha(x_\alpha)u_\alpha(y_\alpha) \\
= u(f_\alpha(u_\alpha))u(f_\alpha(y_\alpha)) = u(x)u(y).
$$
We consider now the unital case and let $ e_\alpha $ denote the identity element of $ E_\alpha $, $ e $ that of $ E $ and $ e' $ that of $ F $. Choose $ \alpha \in I $, then $ e = f_\alpha(e_\alpha) $, whence
$$
u(e) = u(f_\alpha(e_\alpha)) = u_\alpha(e_\alpha) = e'
$$
for $ u_\alpha $ is unital. Hence $ u $ is unital.

By analogy with the notion of direct system of magmas, that of a direct system of monoids or groups can be formulated. Proposition 1 shows that the magma E which is the limit of a direct system of monoids $(E_\alpha, f_{\beta\alpha})_{\alpha, \beta \in I}$ is a monoid. We show that E is a group if the $E_\alpha$ are groups: let $x \in E, \alpha \in I$ and $x_\alpha \in E_\alpha$ be such that $x = f_\alpha(x_\alpha)$; the element $y = f_\alpha(x_\alpha^{-1})$ of E is the inverse of x (\S 2, no. 3). The universal property of Proposition 2 goes over immediately in the case of a direct system of monoids or groups.

The reader is left to define a direct system of rings. Let $(A_\alpha, f_{\beta\alpha})$ be such a direct system; let $A = \lim \overrightarrow{A_\alpha}$ and $f_\alpha : A_\alpha \to A$ the canonical homomorphisms. There exists (Proposition 2) on A one and only one addition and multiplication characterized by $x + y = f_\alpha(x_\alpha + y_\alpha), xy = f_\alpha(x_\alpha y_\alpha)$ for $\alpha \in I, x_\alpha, y_\alpha$ in $A_\alpha$ and $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Under addition A is a commutative group and multiplication is associative and unital. Finally, for $x, y, z$ in A, choose $\alpha$ in I and $x_\alpha, y_\alpha$ and $z_\alpha$ in $A_\alpha$ with
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha) \quad \text{and} \quad z = f_\alpha(z_\alpha).
$$
Then
$$
(x + y) \cdot z = f_\alpha(x_\alpha + y_\alpha)f_\alpha(z_\alpha) = f_\alpha((x_\alpha + y_\alpha)z_\alpha)
= f_\alpha(x_\alpha z_\alpha + y_\alpha z_\alpha) = f_\alpha(x_\alpha z_\alpha) + f_\alpha(y_\alpha z_\alpha) = xz + yz
$$
and the relation $x(y + z) = xy + xz$ is proved analogously. In other words, A has the structure of a ring, characterized by the fact that $f_\alpha$ is a ring homomorphism for all $\alpha \in I$.

The ring A is called the direct limit of the rings $A_\alpha$. Proposition 2 extends immediately to the case of rings.

#### Proposition 3 {#alg-i-s10-prop-3 .statement}

(a) *If the $A_\alpha$ are non-zero, A is non-zero.*
(b) *If the $A_\alpha$ are integral domains, A is an integral domain.*
(c) *If the $A_\alpha$ are fields, A is a field.*

Let $0_\alpha, 1_\alpha$ be the zero and unit of $A_\alpha$ and 0, 1 the zero and unit of A. There exists $\alpha \in I$ such that $f_\alpha(0_\alpha) = 0, f_\alpha(1_\alpha) = 1$. If $0 = 1$, there exists $\beta \geq \alpha$ such that $f_{\beta\alpha}(0_\alpha) = f_{\beta\alpha}(1_\alpha)$, that is $0_\beta = 1_\beta$. This proves (a).

Suppose that $A_\alpha$ are integral domains. Then A is commutative and non-zero by (a). Let $x, y$ be elements of A such that $xy = 0$. There exists $\alpha \in I$ and $x_\alpha, y_\alpha \in A_\alpha$ such that $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Then $f_\alpha(x_\alpha y_\alpha) = xy = 0 = f_\alpha(0_\alpha)$. Hence there exists $\beta \geq \alpha$ such that $f_{\beta\alpha}(x_\alpha y_\alpha) = f_{\beta\alpha}(0_\alpha)$. As $A_\beta$ is an integral domain, it follows that $f_{\beta\alpha}(x_\alpha) = 0_\beta$ or $f_{\beta\alpha}(y_\alpha) = 0_\beta$, hence $x = 0$ or $y = 0$. This proves (b).

Suppose that the $A_\alpha$ are fields. Then $A \neq \{0\}$ by (a). Let $x$ be a non-zero element of A. There exist $\alpha \in I$ and $x_\alpha \in A_\alpha$ such that $x = f_\alpha(x_\alpha)$. Then $x_\alpha \neq 0$ and $f_\alpha(x_\alpha^{-1})$ is the inverse of $x$ in A. This proves (c).

Let $\mathfrak{E} = (E_\alpha, f_{\beta\alpha})$ and $\mathfrak{E}' = (E'_\alpha, f'_{\beta\alpha})$ be two direct systems of magmas (resp. monoids, groups, rings). A homomorphism of $ \mathfrak{E} $ into $ \mathfrak{E}' $ is a direct system $ (u_\alpha)_{\alpha \in I} $ of mappings $ u_\alpha : E_\alpha \to E'_\alpha $ such that each $ u_\alpha $ is a homomorphism. Under these conditions, the mapping $ u = \lim u_\alpha $ from $ E = \lim E_\alpha $ to $ E' = \lim E'_\alpha $ is a homomorphism (cf. *Set Theory*, III, § 7, no. 6).

### 4. DIRECT LIMIT OF ACTIONS

Suppose that there are given two direct systems of sets $ (\Omega_\alpha, \phi_{\beta \alpha}) $ and $ (E_\alpha, f_{\beta \alpha}) $ relative to the same indexing set $ I $ and for each $ \alpha \in I $ an action of $ \Omega_\alpha $ on $ E_\alpha $. Suppose that

$$
f_{\beta \alpha}(\omega_\alpha \cdot x_\alpha) = \phi_{\beta \alpha}(\omega_\alpha) \cdot f_{\beta \alpha}(x_\alpha)
$$

for $ \alpha \leq \beta, \omega_\alpha \in \Omega_\alpha $ and $ x_\alpha \in E_\alpha $. Then the family of actions under consideration is said to be a *direct system of actions*. It is easily verified as in Proposition 2 that there exists an action $ h $ of $ \Omega = \lim \Omega_\alpha $ on $ E = \lim E_\alpha $ which is described as follows: let $ \omega \in \Omega $ and $ x \in E $; choose $ \alpha \in I $ and $ \omega_\alpha \in \Omega_\alpha, x_\alpha \in E_\alpha $ such that $ \omega = \phi_\alpha(\omega_\alpha) $ and $ x = f_\alpha(x_\alpha) $ ($ \phi_\alpha : \Omega_\alpha \to \Omega $ and $ f_\alpha : E_\alpha \to E $ denote the canonical mappings); then $ \omega \cdot x = f_\alpha(\omega_\alpha \cdot x_\alpha) $. The action of $ \Omega $ on $ E $ is called the *direct limit of the actions* of the $ \Omega_\alpha $ on the $ E_\alpha $.

If the $ \Omega_\alpha $ are monoids and each action of $ \Omega_\alpha $ on $ E_\alpha $ is an operation, the direct limit action is an operation.

It is left to the reader to define the direct limit of a direct system of groups with operators and to verify that this limit is a group with operators.

### Exercises {#alg-i-s10-exercises}

See the [exercises for § 10](exercises/s10/).
