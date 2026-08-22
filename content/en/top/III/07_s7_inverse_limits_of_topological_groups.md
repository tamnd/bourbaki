---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 7
section_title: Inverse limits of topological groups and rings
lang: en
source: top-i-iv
pdf_pages: 0290-0301, 0330-0332
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF ALGEBRAIC STRUCTURES
      page: 0
      pdf_page: 290
    - "no": 2
      title: INVERSE LIMITS OF TOPOLOGICAL GROUPS AND SPACES WITH OPERATORS
      page: 0
      pdf_page: 292
    - "no": 3
      title: APPROXIMATION OF TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 295
    - "no": 4
      title: APPLICATION TO INVERSE LIMITS
      page: 0
      pdf_page: 299
statements: 15
exercises: 2
content_sha256: d8ae46ff31970d55849edbf8f1456dea36de8f73d914c85e3eae63c8b2a041e6
---

## 7. INVERSE LIMITS OF TOPOLOGICAL GROUPS AND RINGS

Throughout this section, I denotes a non-empty directed set (*) and $ \alpha \leq \beta $ denotes the partial order relation in I. Unless the contrary is expressly stated, all the inverse systems considered are indexed by I.

### 1. INVERSE LIMITS OF ALGEBRAIC STRUCTURES

Let $ (X_\alpha, f_{\alpha \beta}) $ be an inverse system of sets, and suppose that each $ X_\alpha $ is endowed with an internal law of composition, everywhere defined, and written multiplicatively. Suppose also that the $ f_{\alpha \beta} $ are homomorphisms with respect to these internal laws. Since

$$
f_{\alpha \beta}(x_\beta \cdot y_\beta) = f_{\alpha \beta}(x_\beta) \cdot f_{\alpha \beta}(y_\beta)
$$

whenever $ \alpha \leq \beta $ and $ x_\beta $ and $ y_\beta $ belong to $ X_\beta $, it is clear that $ X = \varprojlim X_\alpha $ is a stable subset of the product $ \prod_\alpha X_\alpha $, with respect to the internal law

$$
(x_\alpha) \cdot (y_\alpha) = (x_\alpha \cdot y_\alpha).
$$

Let $ (\Lambda_\alpha, \varphi_{\alpha \beta}) $ be another inverse system of sets, indexed by I, and suppose that each $ X_\alpha $ carries an external law of composition, everywhere defined, written multiplicatively and having $ \Lambda_\alpha $ as a set of operators, such that whenever $ \alpha \leq \beta $ we have

$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$

for $ \lambda_\beta \in \Lambda_\beta $ and $ x_\beta \in X_\beta $. Then we can define an external law on $ \prod_\alpha X_\alpha $, having $ \prod_\alpha \Lambda_\alpha $ as a set of operators, by defining $ (\lambda_\alpha) \cdot (x_\alpha) = (\lambda_\alpha \cdot x_\alpha) $; restricting the set of operators to $ \Lambda = \varprojlim \Lambda_\alpha $, we have an external law on $ \prod_\alpha X_\alpha $ with respect to which $ X $ is again a stable subset. The internal (resp. external) law thus defined on $ X $ is said to be the inverse limit of the internal (resp. external) laws of the $ X_\alpha $. In the case of external laws, it may happen that all the $ \Lambda_\alpha $ are identical with the same set $ \Lambda_0 $ and

(*) The reader may easily verify that most of the definitions and results which precede Proposition 1 in this section remain valid if I is merely partially ordered.

that all the $ \varphi_{\alpha \beta} $ are identity mappings; then, since $ I $ is a directed set, $ \Lambda $ can be identified with $ \Lambda_0 $.

It is immediately verified that the usual properties of associativity, commutativity, existence of an identity element for an internal law (provided that the $ f_{\alpha \beta} $ map identity element to identity element), distributivity of an external law with respect to an internal law, etc., are preserved under passage to the inverse limit.

Let $ \Sigma $ be a species of algebraic structure and let $ \Sigma_0 $ be the *impoverished* structure corresponding to $ \Sigma $. Whenever we speak of an inverse system of sets $ (X_\alpha, f_{\alpha \beta}) $ endowed with structures of species $ \Sigma $, we shall always suppose that the $ f_{\alpha \beta} $ are *homomorphisms* for these structures. If we endow $ X = \varprojlim X_\alpha $ with the internal and external laws which are the respective inverse limits of the internal and external laws of the $ X_\alpha $, then $ X $ carries an algebraic structure of *species* $ \Sigma_0 $. Naturally it remains to be seen in each particular case whether or not this structure is of species $ \Sigma $.

For example, if $ (G_\alpha, f_{\alpha \beta}) $ is an inverse system of groups (resp. rings), then $ \varprojlim G_\alpha $ is a subgroup (resp. subring) of $ \prod_\alpha G_\alpha $, and is called the *inverse* limit of the system $ (G_\alpha, f_{\alpha \beta}) $ of groups (resp. rings).

Let $ (X_\alpha, g_{\alpha \beta}) $ be an inverse system of sets and let $ (G_\alpha, f_{\alpha \beta}) $ be an inverse system of groups; suppose that each $ X_\alpha $ has $ G_\alpha $ as a group of operators and that whenever $ \alpha \leq \beta $ we have

(I)
$$
g_{\alpha \beta}(s_\beta \cdot x_\beta) = f_{\alpha \beta}(s_\beta) \cdot g_{\alpha \beta}(x_\beta)
$$
for $ x_\beta \in X_\beta $ and $ s_\beta \in G_\beta $. Then $ X = \varprojlim X_\alpha $ has $ G = \varprojlim G_\alpha $ as group of operators. It follows from (I) that, if $ \alpha \leq \beta $, the mappings $ f_{\alpha \beta} $ and $ g_{\alpha \beta} $ are compatible (\S 2, no. 4) and hence define a mapping $ \varphi_{\alpha \beta} : X_\beta / G_\beta \to X_\alpha / G_\alpha $ of the quotient sets, such that $ (X_\alpha / G_\alpha, \varphi_{\alpha \beta}) $ is an inverse system. Moreover, if $ f_\alpha : G \to G_\alpha $ and $ g_\alpha : X \to X_\alpha $ are the canonical mappings, then $ f_\alpha $ and $ g_\alpha $ are compatible and consequently define a mapping $ h_\alpha : X / G \to X_\alpha / G_\alpha $ of the quotient sets; it is clear that the $ h_\alpha $ form an inverse system of mappings, whose inverse limit is therefore a mapping $ h : X / G \to \varprojlim X_\alpha / G_\alpha $, *which is not necessarily either injective or surjective* (Exercise 1).

Again, let $ (A_\alpha, \varphi_{\alpha \beta}) $ be an inverse system of rings and let $ (M_\alpha, f_{\alpha \beta}) $ be an inverse system of commutative groups; and suppose that each $ M_\alpha $ carries a left $ A_\alpha $-module structure in such a way that whenever $ \alpha \leq \beta $ we have

(2)
$$
f_{\alpha \beta}(\lambda_\beta \cdot x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
for $ x_\beta \in M_\beta $ and $ \lambda_\beta \in A_\beta $; then $ \varprojlim M_\alpha $ has a structure of a left module over $ \varprojlim A_\alpha $. If we suppose in addition that, for each $ \alpha $, $ A_\alpha $ is commutative and that each $ M_\alpha $ has an $ A_\alpha $-algebra structure, and finally that $ (M_\alpha, f_{\alpha\beta}) $ is an inverse system of *rings*, then $ \varprojlim M_\alpha $ has a structure of an *algebra* over $ \varprojlim A_\alpha $.

Let $ (G_\alpha, f_{\alpha\beta}) $ be an inverse system of groups, and for each $ \alpha $ let $ H_\alpha $ be a subgroup of $ G_\alpha $. If $ f_{\alpha\beta}(H_\beta) \subset H_\alpha $ whenever $ \alpha \leq \beta $, then the inverse system of subsets $ H_\alpha $ of $ G_\alpha $ is an inverse system of groups with respect to the restrictions of the $ f_{\alpha\beta} $, and $ H = \varprojlim H_\alpha $ is a *subgroup* of $ G = \varprojlim G_\alpha $. If each $ H_\alpha $ is a normal subgroup of $ G_\alpha $, then $ H $ is a normal subgroup of $ G $. If $ (G'_\alpha, f'_{\alpha\beta}) $ is another inverse system of groups and, for each $ \alpha $, $ u_\alpha : G_\alpha \to G'_\alpha $ is a homomorphism such that the $ u_\alpha $ form an inverse system of mappings, then, if $ H_\alpha $ is the kernel of $ u_\alpha $, we have $ f_{\alpha\beta}(H_\beta) \subset H_\alpha $ whenever $ \alpha \leq \beta $; $ u = \varprojlim u_\alpha $ is a homomorphism of $ G $ into $ G' = \varprojlim G'_\alpha $, and $ H = \varprojlim H_\alpha $ is the kernel of $ u $. If we put $ K_\alpha = u_\alpha(G_\alpha) $, then we have $ f'_\alpha(K_\alpha) \subset K_\alpha $ whenever $ \alpha \leq \beta $, so that the $ K_\alpha $ form an inverse system of subgroups of the $ G'_\alpha $; but $ K = \varprojlim K_\alpha $ *is not necessarily the image of* $ G $ *under* $ u $ [Exercise 1 c)].

We obtain analogous results by replacing "group" by "ring", "subgroup" by "ideal" (left or right); we leave to the reader the task of stating the analogous results for modules and algebras.

### 2. INVERSE LIMITS OF TOPOLOGICAL GROUPS AND SPACES WITH OPERATORS

We shall say that an inverse system $ (G_\alpha, f_{\alpha\beta}) $ is an *inverse system of topological groups* if the $ G_\alpha $ are topological groups and the $ f_{\alpha\beta} $ are *continuous* homomorphisms. Then $ G = \varprojlim G_\alpha $ is a subgroup of the product group $ \prod_\alpha G_\alpha $; if we endow $ G $ with the topological group structure induced by that of $ \prod_\alpha G_\alpha $, then the topological group so obtained is called the *inverse limit* of the inverse system of topological groups $ (G_\alpha, f_{\alpha\beta}) $. If the $ G_\alpha $ are Hausdorff (resp. Hausdorff and complete) then $ G $ is Hausdorff and closed in $ \prod_\alpha G_\alpha $ (resp. Hausdorff and complete) (Chapter I, § 8, no. 2, Proposition 7, Corollary 2 and Chapter II, § 3, no. 5, Corollary to Proposition 10).

If $ (G'_\alpha, f'_{\alpha\beta}) $ is another inverse system of topological groups and if, for each $ \alpha $, $ u_\alpha : G_\alpha \to G'_\alpha $ is a continuous homomorphism such that the $ u_\alpha $ form an inverse system of mappings, then $ u = \varprojlim u_\alpha $ is a continuous homomorphism of $ G $ into $ G' = \varprojlim G'_\alpha $ (Chapter I, § 4, no. 4). The same results are valid when "topological group" is replaced by "topological ring"; we leave to the reader the task of stating the analogous results for topological modules (§ 6, no. 6).

Let $(X_\alpha, g_{\alpha\beta})$ be an inverse system of topological spaces, and let $(G_\alpha, f_{\alpha\beta})$ be an inverse system of topological groups. Suppose that each $G_\alpha$ operates continuously on $X_\alpha$ (\S 2, no. 4) and that the relations (i) hold for all $x_\beta \in X_\beta, s_\beta \in G_\beta$ and $\alpha \leq \beta$. We have seen (no. 1) that $X = \varprojlim X_\alpha$ has $G = \varprojlim G_\alpha$ as group of operators; furthermore, $G$ operates continuously on $X$. For if $g_\alpha$ (resp. $f_\alpha$) is the canonical mapping $X \to X_\alpha$ (resp. $G \to G_\alpha$), then by definition
$$
g_\alpha(s.x) = f_\alpha(s) \cdot g_\alpha(x)
$$
and therefore the mappings $(s.x) \to g_\alpha(s.x)$ are continuous on $X \times G$, which shows the continuity of $(s, x) \to (s.x)$ (Chapter I, \S 4, no. 4).

The mapping $h_\alpha : X/G \to X_\alpha/G_\alpha$ induced by $f_\alpha$ and $g_\alpha$ is therefore continuous (\S 2, no. 4), and so is the mapping $h : X/G \to \varprojlim X_\alpha/G_\alpha$ defined by the $h_\alpha$ (Chapter I, \S 2, no. 3, Proposition 4).

#### Proposition 1 {#top-iii-s7-prop-1 .statement}

*Suppose that the $X_\alpha$ and the $G_\alpha$ satisfy the above hypotheses.*

a) *If the stabilizer of each point of $X_\alpha$ is a compact subgroup of $G_\alpha$ for each $\alpha \in I$, then the stabilizer of each point $x = (x_\alpha)$ of $X$ is a compact subgroup of $G$; the orbit of $x$ (with respect to $G$) is canonically homeomorphic to the inverse limit of the orbits of the $x_\alpha$ (with respect to $G_\alpha$); and the canonical mapping $h : X/G \to \varprojlim X_\alpha/G_\alpha$ is injective.*

b) *If, for each $\alpha \in I$, every orbit of a point of $X_\alpha$ (with respect to $G_\alpha$) is compact, then every orbit of a point of $X$ (with respect to $G$) is relatively compact, and $h$ is surjective. If also $h$ is bijective, then every orbit of a point of $X$ is compact.*

Let $x = (x_\alpha) \in X$, and for each $\alpha \in I$ let $X'_\alpha = G_\alpha \cdot x_\alpha$ be the orbit of $x_\alpha$. If $\alpha \leq \beta$, it follows from (i) and the relation $g_{\alpha\beta}(x_\beta) = x_\alpha$ that $g_{\alpha\beta}(X'_\beta) \subset X'_\alpha$, and hence that $(X'_\alpha)$ is an inverse system of subsets of the $X_\alpha$. For each $\alpha \in I$ let $u_\alpha : G_\alpha \to X'_\alpha$ be the continuous mapping $s_\alpha \to s_\alpha \cdot x_\alpha$; the $u_\alpha$ form an inverse system of mappings, and $u = \varprojlim u_\alpha$ is the continuous mapping $s \to s.x$ of $G$ into the subspace $X' = \varprojlim X'_\alpha$ of $X$. The hypothesis of a) implies that $\overline{u}_\alpha(y_\alpha)$ is compact for each $y_\alpha \in X'_\alpha$. Since also $u_\alpha$ is surjective, the conditions of Chapter I, \S 9, no. 6, Proposition 8, Corollary 2 are satisfied, and the first two assertions of a) are therefore established. Hence, if $x = (x_\alpha)$ and $y = (y_\alpha)$ are such that $x_\alpha$ and $y_\alpha$ belong to the same orbit with respect to $G_\alpha$ for each $\alpha \in I$, then $x$ and $y$ belong to the same orbit with respect to $G$, and therefore $h$ is injective.

Likewise, the hypothesis of b) implies that the inverse system of canonical mappings $v_\alpha : X_\alpha \to X_\alpha/G_\alpha$ satisfies the conditions of Chapter I, \S 9, no. 6, Proposition 8, Corollary 2, and therefore its inverse limit $v = \varprojlim v_\alpha : X \to \varprojlim X_\alpha/G_\alpha$ is surjective, and the inverse image under v of every point of $ \varprojlim X_\alpha / G_\alpha $ is compact. Since v factorizes into
$$
X \xrightarrow{\psi} X/G \xrightarrow{h} \varprojlim X_\alpha / G_\alpha,
$$
where $ \psi $ is the canonical mapping, the assertions of b) follow.

#### Corollary 1 {#top-iii-s7-prop-1-cor-1 .statement}

*If the $ G_\alpha $ are compact and the $ X_\alpha $ Hausdorff, then the conclusions of a) and b) are valid.*

For the hypotheses of a) and b) are satisfied, since every closed subgroup of $ G_\alpha $ is compact and $ u_\alpha : s_\alpha \to s_\alpha \cdot x_\alpha $ is a continuous mapping of a compact space into a Hausdorff space.

#### Corollary 2 {#top-iii-s7-prop-1-cor-2 .statement}

*If, for each $ \alpha \in I $, the group $ G_\alpha $ operates transitively on the space $ X_\alpha $, and if the stabilizer of each point of $ X_\alpha $ is a compact subgroup of $ G_\alpha $, then $ G $ operates transitively on $ X $ and the stabilizer of each point of $ X $ is a compact subgroup of $ G $.*

For hypothesis a) is satisfied, and $ X'_\alpha = X_\alpha $ for each $ \alpha $.

#### Corollary 3 {#top-iii-s7-prop-1-cor-3 .statement}

*Suppose that the $ G_\alpha $ are Hausdorff. For each $ \alpha \in I $, let $ K_\alpha $ be a compact subgroup of $ G_\alpha $, such that $ f_{\alpha \beta} (K_\beta) \subset K_\alpha $ whenever $ \alpha \leq \beta $. Then, if $ K = \varprojlim K_\alpha $, the canonical mapping $ h $ of the homogeneous space $ G/K $ into $ \varprojlim G_\alpha / K_\alpha $ is a homeomorphism.*

The fact that $ h $ is bijective follows from Corollary 1, applied by replacing $ X_\alpha $ by $ G_\alpha $, and $ G_\alpha $ by $ K_\alpha $ operating by *right* translations (\S 2, no. 5). Let $ \varphi $ be the canonical mapping $ G \to G/K $, and for each $ \alpha $ let $ f_\alpha $ be the canonical mapping $ G \to G_\alpha $. If, for each $ \alpha $, $ V_\alpha $ runs through a fundamental system of open neighbourhoods of the identity element $ e_\alpha $ of $ G_\alpha $, then the sets $ V = \overline{f}_\alpha^{-1}(V_\alpha) $ ($ \alpha $ and $ V_\alpha $ variable) form a fundamental system of neighbourhoods of the identity element $ e $ in $ G $ (Chapter I, \S 4, no. 4, Proposition 9), and the sets $ \varphi(V.K) $ form a fundamental system of neighbourhoods of $ \varphi(e) $ in $ G/K $. We have to show that the image of $ \varphi(V.K) $ under $ h $ contains a neighbourhood of $ h(\varphi(e)) $, that is that there exists $ \beta \geq \alpha $ and a neighbourhood $ W_\beta $ of $ e_\beta $ in $ G_\beta $ such that $ \overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset V.K $. Now, the relation $ x \in V.K $ is equivalent to the existence of $ y $ in $ K $ such that $ f_\alpha(xy^{-1}) \in V_\alpha $, i.e. $ f_\alpha(x) \in V_\alpha \cdot f_\alpha(K) $; so that $ V.K = \overline{f}_\alpha^{-1}(V_\alpha \cdot f_\alpha(K)) $. Let $ U_\alpha = V_\alpha \cdot f_\alpha(K) $; we shall see that there exists $ \beta \geq \alpha $ such that if we put $ U_\beta = \overline{f}_{\alpha \beta}^{-1}(U_\alpha) $, we have $ K_\beta \subset U_\beta $; it will then follow that there is a neighbourhood $ W_\beta $ of $ e_\beta $ in $ G_\beta $ such that $ W_\beta . K_\beta \subset U_\beta $ (Chapter II, \S 4, no. 3, Corollary to Proposition 4), and this will establish the desired relation
$$
\overline{f}_\beta^{-1}(W_\beta . K_\beta) \subset \overline{f}_\beta^{-1}(U_\beta) = V.K.
$$

We proceed by *reductio ad absurdum*: for each $ \beta \geq \alpha $, let $ M_\beta $ denote $ K_\beta \cap G U_\beta $; since $ f_{\beta \gamma}^{-1}(U_\beta) = U_\gamma $ if $ \alpha \leq \beta \leq \gamma $, the $ M_\beta $ form an inverse system of compact subsets of the $ G_\beta $ (for $ \beta \geq \alpha $). If they were all non-empty, then their inverse limit $ M $ would also be non-empty (Chapter I, § 9, no. 6, Proposition 8). It is clear that $ M \subset K $ and $ f_\alpha(M) \subset M_\alpha $; but this is absurd since $ f_\alpha(K) \subset U_\alpha $, and the proof is therefore complete.

### 3. APPROXIMATION OF TOPOLOGICAL GROUPS

Let $ G $ be a group and let $ (H_\alpha)_{\alpha \in I} $ be a family of normal subgroups of $ G $ such that $ H_\alpha \supset H_\beta $ whenever $ \alpha \leq \beta $. For each $ \alpha \in I $ let $ G_\alpha = G / H_\alpha $, and for $ \alpha \leq \beta $ let $ f_{\alpha \beta} $ be the canonical homomorphism $ G / H_\beta \to G / H_\alpha $, which therefore maps a coset $ T $ of $ H_\beta $ in $ G $ to the coset $ TH_\alpha $ of $ H_\alpha $ in $ G $. Clearly $ (G_\alpha, f_{\alpha \beta}) $ is an inverse system of groups; the elements of $ \tilde{G} = \varprojlim G_\alpha $ are families $ (T_\alpha)_{\alpha \in I} $, where $ T_\alpha $ is a coset of $ H_\alpha $ in $ G $ for each $ \alpha $, and $ T_\alpha \supset T_\beta $ whenever $ \alpha \leq \beta $. The mapping $ i : s \mapsto (s H_\alpha) $ of $ G $ into $ \tilde{G} $ is the inverse limit of the canonical homomorphisms $ G \to G / H_\alpha $ and is therefore a homomorphism of $ G $ into $ \tilde{G} $, and the inverse image under $ i $ of an element $ (T_\alpha) \in \tilde{G} $ is equal to $ \bigcap_{\alpha \in I} T_\alpha $. The kernel of $ i $ is therefore $ \bigcap_{\alpha \in I} H_\alpha $, and the image of $ i $ consists of all families $ (T_\alpha) \in \tilde{G} $ whose intersection is *non-empty*.

Now suppose that $ G $ is a *topological group*; if we give each $ G_\alpha = G / H_\alpha $ the quotient topology, it is clear that $ (G_\alpha, f_{\alpha \beta}) $ is an inverse system of topological groups, and that $ i : G \to \tilde{G} $ is a continuous homomorphism.

#### Proposition 2 {#top-iii-s7-prop-2 .statement}

*Let $ G $ be a topological group and let $ (H_\alpha)_{\alpha \in I} $ be a family of normal subgroups of $ G $ such that $ H_\alpha \supset H_\beta $ whenever $ \alpha \leq \beta $, and which satisfy the following condition:*

(AP) *For each $ \alpha \in I $, $ H_\alpha $ is closed in $ G $ and every neighbourhood of the identity element $ e $ in $ G $ contains one of the $ H_\alpha $ (in other words, the filter base formed by the $ H_\alpha $ converges to $ e $).*

*Then the mapping $ i : G \to \tilde{G} = \varprojlim G / H_\alpha $ is a strict morphism of $ G $ onto $ i(G) $; $ \tilde{G} $ is Hausdorff and $ i(G) $ is dense in $ \tilde{G} $; and finally the kernel of $ i $ is the closure of $ \{e\} $ in $ G $. If in addition one of the $ H_\alpha $ is complete, then $ i $ is surjective.*

Clearly the $ G_\alpha = G / H_\alpha $ are Hausdorff (\S 2, no. 5, Proposition 13), hence so is $ \tilde{G} $ (since it is a subspace of $ \prod_{\alpha \in I} G_\alpha $). The kernel $ H $ of $ i $ is the intersection of the $ H_\alpha $ and is therefore a closed subgroup of $ G $. Since each neighbourhood of $ e $ contains some $ H_\alpha $, it contains $ H $ and therefore [§ 3, no. 1, formula (1)] $ H $ is the closure of $ \{e\} $. Let us next show that $ i(G) $ is dense in $ \tilde{G} $. Let $ f_\alpha $ be the canonical mapping $ \tilde{G} \to G_\alpha $, which is the restriction to $ \tilde{G} $ of the projection $ pr_\alpha $; $ \varphi_\alpha = f_\alpha \circ i $ is the canonical mapping $ G \to G/H_\alpha $. If $ U $ is any non-empty open set of $ \tilde{G} $, then there is an index $ \alpha \in I $ and a non-empty open set $ U_\alpha $ in $ G_\alpha $ such that $ \overline{f}_\alpha^{-1}(U_\alpha) \subset U $ (Chapter I, § 4, no. 4, Proposition 9); therefore
$$
\overline{i}^{-1}(U) \supset \overline{\varphi}_\alpha^{-1}(U_\alpha);
$$
but since $ \varphi_\alpha $ is surjective, $ \overline{i}^{-1}(U) $ is not empty, and therefore $ i(G) \cap U \neq \emptyset $.

To see that $ i $ is a strict morphism of $ G $ onto $ i(G) $, consider a neighbourhood $ V $ of $ e $ in $ G $. There is a neighbourhood $ W $ of $ e $ in $ G $ such that $ W^2 \subset V $, and an index $ \alpha \in I $ such that $ H_\alpha \subset W $; it follows that $ V $ contains $ WH_\alpha = \overline{\varphi}_\alpha(\varphi_\alpha(W)) = \overline{i}^{-1}(\overline{f}_\alpha^{-1}(\varphi_\alpha(W))) $. Since $ \overline{f}_\alpha(\varphi_\alpha(W)) $ is a neighbourhood of the identity element in $ \tilde{G} $, the result follows.

Finally, suppose that there is an index $ \gamma \in I $ such that $ H_\gamma $ is complete. To show that $ i $ is surjective it is enough to prove that every family $ (T_\alpha)_{\alpha \in I} \in \tilde{G} $ has a non-empty intersection. Since $ T_\gamma $ is obtained by translation from $ H_\gamma $, it is a complete subspace of $ G $ (with respect to both the right and the left uniformities). Moreover, since every neighbourhood $ U $ of $ e $ in $ G $ contains one of the $ H_\alpha $, the corresponding set $ T_\alpha $ is $ U_{d-} $ (or $ U_{s-} $) small, and hence the set of $ T_\alpha $ contained in $ T_\gamma $ is a Cauchy filter base; therefore it converges in $ T_\gamma $, and since the $ T_\alpha $ are closed in $ G $ (since they are translations of the $ H_\alpha $), their intersection is not empty.

Q.E.D.

#### Corollary 1 {#top-iii-s7-prop-2-cor-1 .statement}

*If the condition (AP) is satisfied and if in addition the (Hausdorff) groups $ G/H_\alpha $ are complete, then the group $ G $ has a Hausdorff completion which can be identified with $ \tilde{G} $; and the mapping $ i : G \to \tilde{G} $ is then identified with the canonical mapping ($ \S 3 $, no. 3, Proposition 5).*

For $ \tilde{G} $ is then complete (no. 2), and Proposition 2 shows that $ i(G) $ is isomorphic with the Hausdorff group associated with $ G $; since it is dense in $ \tilde{G} $, the corollary follows ($ \S 3 $, no. 3, Proposition 5). In particular:

#### Corollary 2 {#top-iii-s7-prop-2-cor-2 .statement}

*Let $ G $ be a group and let $ (H_\alpha) $ be a family of normal subgroups of $ G $, directed with respect to the relation $ H_\alpha \supset H_\beta $. If we endow $ G $ with the group topology for which the $ H_\alpha $ form a fundamental system of neighbourhoods of the identity element $ e $, then the Hausdorff group associated with $ G $ is isomorphic to $ G_1 = G / \left( \bigcap_\alpha H_\alpha \right) $; $ G_1 $ has a completion $ \hat{G}_1 = \tilde{G} $; and the canonical mapping $ G_1 \to \tilde{G} = \varprojlim G/H_\alpha $ extends to an isomorphism of $ \hat{G} = \hat{G}_1 $ onto $ \tilde{G} $.*

The subgroup $ H_\alpha $ of $ G $ is open and therefore also closed ($ \S $ 2, no. 1, Corollary to Proposition 4), and $ G/H_\alpha $ is discrete ($ \S $ 2, no. 6, Proposition 18); hence the conditions of Corollary 1 are satisfied.

For the remainder of this sub-section we shall assume that $ G $ is *Hausdorff* and that $ (H_\alpha) $ is a family of *compact* normal subgroups of $ G $, which is directed with respect to the relation $ H_\alpha \supset H_\beta $ and which satisfies the condition (AP); by virtue of Proposition 2, the mapping

$$
i : G \to \tilde{G} = \varprojlim G/H_\alpha
$$

is then an *isomorphism of topological groups* which permits us to identify $ G $ and $ \tilde{G} $. We denote by $ f_\alpha $ the canonical mapping $ G \to G/H_\alpha $.

#### Lemma 1 {#top-iii-s7-lem-1 .statement}

*Under the hypotheses of Proposition 2, if $ E $ is any closed subset of $ G $ we have* $ E = \bigcap_\alpha E H_\alpha $.

For $ E $ is the intersection of the sets $ EV $ where $ V $ runs through the neighbourhood filter of $ e $ [$ \S $ 3, no. 1, formula (1)], and every neighbourhood of $ e $ contains an $ H_\alpha $; whence the result, since $ E \subset EH_\alpha $.

#### Proposition 3 {#top-iii-s7-prop-3 .statement}

*Suppose that $ G $ is Hausdorff and that the $ H_\alpha $ are compact and satisfy* (AP).

a) *Let $ L $ be a closed subgroup of $ G $; then, for each $ \alpha \in I $, the subgroup $ L_\alpha = f_\alpha(L) $ of $ G_\alpha = G/H_\alpha $ is closed, and the isomorphism $ i $ of $ G $ onto $ \varprojlim G_\alpha $ gives by restriction an isomorphism of $ L $ onto $ \varprojlim L_\alpha $. If also $ L $ is normal in $ G $, then $ L_\alpha $ is normal in $ G_\alpha $ for each $ \alpha \in I $, and by passing to the quotients, $ i $ induces an isomorphism of $ G/L $ onto $ \varprojlim G_\alpha/L_\alpha $.

b) *Conversely, for each $ \alpha \in I $ let $ L_\alpha $ be a closed subgroup of $ G_\alpha $, such that $ L_\alpha = f_{\alpha\beta}(L_\alpha) $ whenever $ \alpha \leq \beta $. Then there is a unique closed subgroup $ L $ of $ G $ such that $ L_\alpha = f_\alpha(L) $ for each $ \alpha \in I $; and if in addition $ L_\alpha $ is normal in $ G_\alpha $ for each $ \alpha \in I $, then $ L $ is normal in $ G $.*

a) Since $ H_\alpha $ is compact, $ LH_\alpha $ is closed in $ G $ ($ \S $ 4, no. 1, Proposition 1, Corollary 1) and therefore $ L_\alpha $ is closed in $ G_\alpha $. Since $ i $ identifies the topological groups $ G $ and $ \varprojlim G_\alpha $, and since $ \varprojlim L_\alpha $ may be identified with a (topological) subgroup of $ \varprojlim G_\alpha $, $ i $ identifies the subgroup $ \bigcap_\alpha LH_\alpha $ of $ G $ with $ \varprojlim L_\alpha $, and to prove the first assertion it is enough to remark that $ L = \bigcap_\alpha LH_\alpha $ by Lemma 1. On the other hand, if $ L $ is normal, then for each $ \alpha \in I $ the mapping $ f'_\alpha : G/L \to G_\alpha/L_\alpha $ induced by $ f_\alpha $ is a surjective strict morphism ($ \S $ 2, no. 8, Remark 3), whose kernel is the *compact* normal subgroup $ H_\alpha L/L $ of $ G/L $, the canonical image of the compact subgroup $ H_\alpha $ of $ G $. Since the subgroups $ H_\alpha L/L $ of $ G/L $ satisfy condition (AP) (\S 2, no. 8, Proposition 24), and since $ G/L $ is Hausdorff, the last assertion of a) is a consequence of Proposition 2.

b) Let $ f'_{\alpha \beta} $ be the restriction of $ f_{\alpha \beta} $ to $ L_\beta $ ($ \alpha \leq \beta $). Then $ (L_\alpha, f'_{\alpha \beta}) $ is an inverse system of topological groups, whose inverse limit $ L $ can be identified with the subgroup $ G \cap \prod_\alpha L_\alpha $ of $ G $. By hypothesis, $ f'_{\alpha \beta} $ is surjective and its kernel is the compact subgroup $ f_\beta(H_\alpha) \cap L_\beta $ of $ L_\beta $; consequently (Chapter I, \S 9, no. 6, Corollary 1 to Proposition 8) we have $ L_\alpha = f_\alpha(L) $ for all $ \alpha \in I $. If $ L' $ is another closed subgroup of $ G $ such that $ f_\alpha(L') = L_\alpha $ for all $ \alpha \in I $, then $ L'H_\alpha = \overline{f'}_\alpha(L_\alpha) $, whence (Lemma 1) $ L' = \bigcap_\alpha L'H_\alpha = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha) = L $. Finally, the last assertion of b) follows from the formula $ L = \bigcap_\alpha \overline{f'}_\alpha(L_\alpha) $, since the $ \overline{f'}_\alpha(L_\alpha) $ are now normal subgroups of $ G $.

#### Proposition 4 {#top-iii-s7-prop-4 .statement}

*Suppose that $ G $ is Hausdorff, the $ H_\alpha $ are compact and that (AP) is satisfied. If $ C_\alpha $ is the identity component of $ G_\alpha = G/H_\alpha $, then the identity component $ C $ of $ G $ can be identified with $ \varprojlim C_\alpha $, and we have $ f_\alpha(C) = C_\alpha $.*

The proposition is a consequence of the following lemma:

#### Lemma 2 {#top-iii-s7-lem-2 .statement}

*Let $ G $ be a Hausdorff topological group and let $ H $ be a compact normal subgroup of $ G $, and $ \varphi $ the canonical mapping $ G \to G/H $. If $ C $ is the identity component of $ G $, then $ \varphi(C) $ is the identity component of $ G' = G/H $.*

Once this lemma is established, we shall have $ f_\alpha(C) = C_\alpha $ for each $ \alpha \in I $, and since $ C $ is a closed subgroup of $ G $ (\S 2, no. 2, Proposition 7) it suffices to apply Proposition 3 a).

To prove the lemma, notice first that if $ C' $ is the component of the identity element $ e' $ in $ G' $, then $ \varphi(C) \subset C' $ since $ \varphi(C) $ is connected. Suppose that $ \varphi(C) \neq C' $. Since $ C $ is a closed normal subgroup of $ G $ (\S 2, no. 2, Proposition 7), $ \varphi(C) $ is a normal subgroup of $ G' $; if $ \psi $ is the canonical mapping $ G' \to G'/\varphi(C) $, then $ \psi(C') $ is connected and does not consist of the identity element alone; hence the identity component of $ G'/\varphi(C) $ does not consist of the identity element alone. But $ G'/\varphi(C) $ is isomorphic to $ (G/H)/(HC/H) $, hence to $ G/HC $, and consequently also to $ (G/C)/(HC/C) $ (\S 2, no. 7, Corollary to Proposition 22, and Proposition 20). Now, $ G/C $ is Hausdorff and totally disconnected (Chapter I, \S 11, no. 5, Proposition 9), and $ HC/C $, being the canonical image of the compact normal subgroup $ H $ of $ G $, is a compact subgroup of $ G/C $. It is therefore sufficient to prove Lemma 2 under the additional hypothesis that $ G $ is *totally disconnected*, i.e. $ C = \{e\} $.

Suppose then that $ C' \neq \{e'\} $; replacing $ G $ by its subgroup $ \overline{f'}(C') $, which is totally disconnected and contains $ H $, we may suppose that $ G' $ is *connected* and does not consist of a single point.

Let $ \mathfrak{M} $ be the set of closed subgroups $ L $ of $ G $ such that $ LH = G $. We shall show that the set $ \mathfrak{M} $, ordered by the relation $ \supset $, is *inductive*. Indeed, if $ \mathfrak{T} $ is a linearly ordered subset of $ \mathfrak{M} $, then for each $ x \in G $ the set of sets $ xH \cap L $ with $ L \in \mathfrak{T} $ is a filter base formed of closed sets in the compact space $ xH $; hence the intersection of these sets is not empty, which shows that the intersection of the subgroups $ L \in \mathfrak{T} $ belongs to $ \mathfrak{M} $. Applying Zorn's lemma, we see therefore that $ \mathfrak{M} $ has a *minimal* element $ L_0 $. Since $ H $ is compact, $ G/H = L_0H/H $ is isomorphic to $ L_0/(L_0 \cap H) $ (\S 4, no. 1, Proposition 1, Corollary 3); since $ L_0 $ is totally disconnected and $ L_0 \cap H $ is compact, we see that we may replace $ G $ by $ L_0 $; in other words, we may suppose in addition that there is *no* closed subgroup $ L \neq G $ such that $ LH = G $.

Now let $ F $ be the intersection of the neighbourhoods of the identity element which are both open and closed in $ G $, and let us show that $ F $ is a closed subgroup of $ G $. Clearly $ F $ is closed in $ G $; hence it is enough to show that $ F^{-1}F \subset F $. But if $ x \in F $ and if $ V $ is an open and closed neighbourhood of $ e $ in $ G $, then so is $ xV $; for otherwise $ e $ would belong to the complement $ W $ of $ xV $ in $ G $, which is again open and closed, and we should have $ x \notin W $; hence $ x \notin F $, contrary to hypothesis. It follows that $ xF $, the intersection of the sets $ xV $ as $ V $ runs through the open and closed neighbourhoods of $ e $ in $ G $, contains $ F $; in other words, $ x^{-1}F \subset F $, which proves our assertion. Since $ G $ is totally disconnected and $ G \neq \{e\} $, we have $ F \neq G $. But if $ V $ is an open and closed neighbourhood of $ e $ in $ G $, then $ VH $ is also open and closed in $ G $ (\S 4, no. 1, Corollary 1 to Proposition 1), hence $ \varphi(V) $ is both open and closed in $ G/H $, and this implies that $ \varphi(V) = G/H $ by virtue of the hypothesis. We shall conclude from this that $ FH = G $, which will give us the desired contradiction and complete the proof of the lemma. Indeed, for each $ x \in G $, $ xH $ meets every neighbourhood $ V $ of $ e $ which is both open and closed, hence also meets the intersection $ F $ of these neighbourhoods, since the sets $ Vx \cap H $ form a filter base consisting of closed sets in the compact space $ xH $.

Q.E.D.

#### Remark {#top-iii-s7-n3-rem-1 .statement}

If the subgroup $ H_\alpha $ is compact for *some* $ \alpha \in I $, then $ H_\beta $ is compact for all $ \beta \geq \alpha $, because it is a closed subgroup of $ H_\alpha $. Since the set of all $ \beta \in I $ such that $ \beta \geq \alpha $ is cofinal in $ I $, it makes essentially no difference, in the study of the group $ G $, whether we suppose that one of the $ H_\alpha $ is compact or that *all* the $ H_\alpha $ are compact.

### 4. APPLICATION TO INVERSE LIMITS

#### Proposition 5 {#top-iii-s7-prop-5 .statement}

*Let* $ (G_\alpha, f_{\alpha\beta}) $ *be an inverse system of Hausdorff topological groups such that the* $ f_{\alpha\beta} $ *are surjective strict morphisms with compact kernels.* Then for each $ \alpha \in I $ the canonical mapping $ f_\alpha $ of $ G = \varprojlim G_\alpha $ into $ G_\alpha $ is a surjective strict morphism whose kernel is compact.

The facts that $ f_\alpha $ is surjective and that its kernel is compact are consequences of Chapter I, § 9, no. 6, Corollary 1 to Proposition 8. It remains to show that $ f_\alpha $ is a strict morphism. Let $ e $ (resp. $ e_\alpha $) denote the identity element of $ G $ (resp. $ G_\alpha $). Each neighbourhood $ V $ of $ e $ in $ G $ contains a set of the form $ f_\beta^{-1}(V_\beta) $, where $ V_\beta $ is a neighbourhood of $ e_\beta $ in $ G_\beta $, and we may suppose that $ \beta \geq \alpha $; since $ f_{\alpha \beta} $ is a surjective strict morphism, $ f_{\alpha \beta}(V_\beta) $ is a neighbourhood of $ e_\alpha $ in $ G_\alpha $, and since $ f_\beta $ is surjective, we have $ V_\beta \subset f_\beta(V) $, whence

$$
f_\alpha(V) = f_{\alpha \beta}(f_\beta(V)) \supset f_{\alpha \beta}(V_\beta);
$$

this shows that $ f_\alpha(V) $ is a neighbourhood of $ e_\alpha $ in $ G_\alpha $.

If $ H_\alpha = f_\alpha^{-1}(e_\alpha) $, then each $ H_\alpha $ is a compact normal subgroup of $ G $; the $ H_\alpha $ clearly satisfy the condition (AP) of no. 3; and $ G_\alpha $ can be identified with $ G/H_\alpha $. In particular Propositions 3 and 4 of no. 3 apply to $ G $ and the $ H_\alpha $.

#### Corollary 1 {#top-iii-s7-prop-5-cor-1 .statement}

*Let* $ (G_\alpha, f_{\alpha \beta}) $ *be an inverse system of topological groups which satisfies the hypotheses of Proposition 5; let* $ (G'_\alpha, f'_{\alpha \beta}) $ *be an inverse system of topological groups, and for each* $ \alpha $ *let* $ u_\alpha : G_\alpha \to G'_\alpha $ *be a surjective strict morphism with compact kernel, such that the* $ u_\alpha $ *from an inverse system of mappings. Then* $ u = \varprojlim u_\alpha $ *is a strict morphism of* $ G = \varprojlim G_\alpha $ *onto* $ G' = \varprojlim G'_\alpha $, *and its kernel is compact*.

Let $ N_\alpha $ be the kernel of $ u_\alpha $. $ L_\alpha = f_\alpha^{-1}(N_\alpha) $ is then the kernel of the surjective strict morphism $ v_\alpha = u_\alpha \circ f_\alpha : G \to G'_\alpha $; since $ L_\alpha / H_\alpha $ is isomorphic to $ N_\alpha $ (\S 2, no. 7, Proposition 20), $ L_\alpha $ is a *compact* normal subgroup of $ G $ (\S 4, no. 1, Corollary 2 to Proposition 2). The kernel $ L $ of $ u $ is the intersection of the $ L_\alpha $. Let $ \varphi $ denote the canonical mapping $ G \to G/L $; then we can write $ v_\alpha = w_\alpha \circ \varphi $, where $ w_\alpha $ is a strict morphism of $ G/L $ onto $ G'_\alpha $, whose kernel is $ L_\alpha / L $. Since the intersection of the $ L_\alpha / L $ is the identity element of $ G/L $, and since the $ L_\alpha / L $ form a filter base and are compact, this filter base converges to the identity element of $ G/L $ (Chapter I, § 9, no. 1, Corollary to Theorem 1). Proposition 2 of no. 3 then shows that $ w = \varprojlim w_\alpha $ is an *isomorphism* of $ G/L $ onto $ G' $; it follows that $ w \circ \varphi $ is a strict morphism of $ G $ onto $ G' $, with kernel $ L $. But it is clear that $ u = w \circ \varphi $, and thus the corollary is proved.

#### Corollary 2 {#top-iii-s7-prop-5-cor-2 .statement}

*Let* $ (G_\alpha, f_{\alpha \beta}) $ *be an inverse system of topological groups which satisfies the conditions of Proposition 5, and let* $ G' $ *be a topological group in which there is a neighbourhood* $ V' $ *of the identity element* $ e' $ *which contains no subgroup* of $ G' $ other than $ \{ e' \} $. Then if $ v : G \to G' $ is any continuous homomorphism, there is an index $ \alpha \in I $ and a continuous homomorphism $ v_\alpha : G_\alpha \to G' $ such that $ v = v_\alpha \circ f_\alpha $.

For since $ \overline{v}^{-1}(V') $ is a neighbourhood of $ e $ in $ G $, there is an index $ \alpha $ and a neighbourhood $ V_\alpha $ of $ e_\alpha $ in $ G_\alpha $ such that $ f_\alpha^{-1}(V_\alpha) \subset \overline{v}^{-1}(V') $. Hence $ v(H_\alpha) \subset V' $, and since $ v(H_\alpha) $ is a subgroup of $ G' $, it follows that $ v(H_\alpha) = \{ e' \} $. Since $ f_\alpha $ may be identified with the canonical mapping $ G \to G/H_\alpha $, the corollary is a consequence of the canonical factorization of a continuous homomorphism (\$ 2, no. 8).

### Exercises {#top-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
