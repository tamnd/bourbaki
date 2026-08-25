---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 5
section_title: Extension of the ring of scalars
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0301-0308, 0422-0423
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSION OF THE RING OF SCALARS OF A MODULE
      page: 0
      pdf_page: 301
    - "no": 2
      title: RELATIONS BETWEEN RESTRICTION AND EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 304
    - "no": 3
      title: EXTENSION OF THE RING OF OPERATORS OF A HOMOMORPHISM MODULE
      page: 0
      pdf_page: 306
    - "no": 4
      title: DUAL OF A MODULE OBTAINED BY EXTENSION OF SCALARS
      page: 0
      pdf_page: 307
    - "no": 5
      title: A CRITERION FOR FINITENESS
      page: 0
      pdf_page: 308
statements: 13
exercises: 7
content_sha256: 9dcec4379b178efb0b444af507c3865e7f1e54d30e287fb7364b2bc5107f0bd3
---

## § 5. EXTENSION OF THE RING OF SCALARS

### 1. EXTENSION OF THE RING OF SCALARS OF A MODULE

Let $A, B$ be two rings and $\rho : A \to B$ a ring homomorphism; we consider the right $A$-module $\rho^*(B_d)$ defined by this homomorphism ($\S 1$, no. 13); this $A$-module also has a left $B$-module structure, namely that of $B_s$ and, as $b'(b\rho(a)) = (b'b)\rho(a)$ for $a \in A, b, b'$ in $B$, these two module structures on $B$ are compatible ($\S 1$, no. 14). This allows us, for every left $A$-module $E$, to define a left $B$-module structure on the tensor product $\rho_*(B_d) \otimes_A E$ such that $\beta'(\beta \otimes x) = (\beta'\beta) \otimes x$ for $\beta, \beta'$ in $B$ and $x \in E$ ($\S 3$, no. 3). This left $B$-module is said to be *derived from $E$ by extending the ring of scalars to $B$ by means of $\rho$* and it is denoted by $\rho^*(E)$ or $E_{(B)}$ if no confusion arises.

#### Proposition 1 {#alg-ii-s5-prop-1 .statement}

*For every left $A$-module $E$, the mapping $\phi : x \mapsto 1 \otimes x$ of $E$ into the $A$-module $\rho_*(\rho^*(E))$ is $A$-linear and the set $\phi(E)$ generates the $B$-module $\rho^*(E)$. Further, for every left $B$-module $F$ and every $A$-linear mapping $f$ of $E$ into the $A$-module $\rho_*(F)$, there exists one and only one $B$-linear mapping $\bar{f}$ of $\rho^*(E)$ into $F$ such that $\bar{f}(1 \otimes x) = f(x)$ for all $x \in E$.*

$B$ can be considered as a $(B, A)$-bimodule by means of $\rho$; then there is a canonical $\mathbf{Z}$-module isomorphism

(1)
$$
\operatorname{Hom}_B(B \otimes_A E, F) \to \operatorname{Hom}_A(E, \operatorname{Hom}_B(B_s, F))
$$
as has been seen in $\S 4$, no. 1, Proposition 1. But the left $A$-module $\operatorname{Hom}_B(B_s, F)$ is canonically identified with $\rho^*(F)$: for, by definition ($\S 1$, no. 14), there corresponds to an element $y \in F$ the homomorphism $\theta(y) : B_s \to F$ such that $(\theta(y))(1) = y$; for all $\lambda \in A$, there thus corresponds to $\rho(\lambda)y \in F$ the homomorphism $\mu \mapsto \mu \rho(\lambda)y$ of $B_s$ into $F$, which is just $\lambda \theta(y)$ for the left $A$-module structure on $\operatorname{Hom}_B(B_s, F)$ ($\S 1$, no. 14). Using this identification, we obtain therefore a *canonical* $\mathbf{Z}$-module *isomorphism*, the inverse of (1)

(2)
$$
\delta : \operatorname{Hom}_A(E, \rho_*(F)) \to \operatorname{Hom}_B(\rho^*(E), F)
$$
and it follows immediately from the definitions that if $\delta(f) = \bar{f}$ then $\bar{f}(1 \otimes x) = f(x)$ for all $x \in E$. In particular, the mapping $\phi_E : x \mapsto 1 \otimes x$ is just
(3)
$$
\phi_E = \delta^{-1}(1_{\rho^*(E)}).
$$

Proposition 1 is therefore proved. The mapping $\phi_E : E \to \rho_*(\rho^*(E))$ is called *canonical*.

#### Remark {#alg-ii-s5-n1-rem-1 .statement}

(1) Proposition 1 shows that the ordered pair consisting of $E_{(B)}$ and $\phi_E$ is a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1), where $\Sigma$ is the species of left B-module structures (the morphisms being B-linear mappings) and the $\alpha$-mappings are the A-linear mappings of E into a B-module.

(2) If E is an $(A, (C'_i); (D'_j))$-multimodule and F a $(B, (C''_h); (D''_k))$-multimodule, then the isomorphism (2) is linear with respect to the $((D'_j, (C''_h); (C'_i), (D''_k))$-multimodule structures of the two sides ($§ 1$, no. 14 and $§ 3$, no. 4).

(3) Let E be a left A-module, $a$ a two-sided ideal of A and $\rho : A \to A/a$ the canonical homomorphism. In the notation of $§ 3$, no. 6, Corollary 2 to Proposition 6, the A-module $E/aE$ is annihilated by $a$ and therefore has canonically a left $(A/a)$-module structure ($§ 1$, no. 12); it is immediate that the canonical mapping $\pi : \rho^*(E) \to E/aE$ defined in $§ 3$, no. 6, Corollary 2 to Proposition 6 is an isomorphism for the $(A/a)$-module structures.

#### Corollary {#alg-ii-s5-n1-cor-1 .statement}

*Let E, E' be two left A-modules; for every A-linear mapping $u : E \to E'$, $v = l_B \otimes u$ is the unique B-linear mapping which renders commutative the diagram*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E_{(B)} \\
| & & | \\
u \downarrow & & v \downarrow \\
E' & \xrightarrow{\phi_{E'}} & E'_{(B)}
\end{array}
$$

*where $\phi_E$ and $\phi_{E'}$ are the canonical mappings.*

It suffices to apply Proposition 1 to the A-homomorphism $\phi_{E'} \circ u : E \to E'_{(B)}$.

The mapping $v$ defined in the above corollary is denoted by $\rho^*(u)$ or $u_{(B)}$.

If $E''$ is a third left A-module and $v : E' \to E''$ an A-linear mapping, it is immediate that

$$
(v \circ u)_{(B)} = v_{(B)} \circ u_{(B)}.
$$

Extending the ring of operators of a module is a *transitive* operation; to be precise:

#### Proposition 2 {#alg-ii-s5-prop-2 .statement}

*Let $\rho : A \to B,\ \sigma : B \to C$ be ring homomorphisms. For every left A-module E, there exists one and only one C-homomorphism*

$$(4)$$
$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$
*mapping $1 \otimes (1 \otimes x)$ to $1 \otimes x$ for all $x \in E$ and this homomorphism is bijective.*

The underlying $\mathbf{Z}$-modules of $\sigma^*(\rho^*(E))$ and $(\sigma \circ \rho)^*(E)$ are respectively $C \otimes_B (B \otimes_A E)$ and $C \otimes_A E$. There exists a canonical $\mathbf{Z}$-isomorphism $C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$ ($§ 3$, no. 8, Proposition 8), which is also a C-isomorphism for the left C-module structures on both sides. Moreover, the

C-module $C \otimes_B B$ is canonically identified with the C-module $C_s$ under the isomorphism which maps $\gamma \otimes \beta$ to $\gamma \sigma(\beta)$ (\S 3, no. 4, Proposition 4) and this isomorphism is also an isomorphism for the right A-module structure on $C \otimes_B B$ defined by $\rho$ and the right A-module structure on C defined by $\sigma \circ \rho$. Thus a canonical isomorphism

$$
(C \otimes_B B) \otimes_A E \to C \otimes_A E
$$

is obtained and, composing it with the isomorphism

$$
C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E
$$

defined earlier, the desired canonical isomorphism is obtained.

If $\phi, \phi'$ and $\phi''$ denote the canonical mappings $E \to \rho^*(E), \rho^*(E \to) \sigma^*(\rho^*(E))$ and $E \to (\sigma \circ \rho)^*(E)$, $\phi' \circ \phi$ is identified with $\phi''$ under the canonical isomorphism of Proposition 2.

#### Proposition 3 {#alg-ii-s5-prop-3 .statement}

*Let A, B be two commutative rings, $\rho : A \to B$ a ring homomorphism and E, E' two A-modules. There exists one and only one B-homomorphism*

$$
E_{(B)} \otimes_B E'_{(B)} \to (E \otimes_A E')_{(B)}
$$

*mapping* $(1 \otimes x) \otimes (1 \otimes x')$ *to* $1 \otimes (x \otimes x')$ *for* $x \in E, x' \in E'$, *and this homomorphism is bijective*.

The left hand side of (5) may be written $(B \otimes_A E) \otimes_B (B \otimes_A E')$ and is identified with $(E \otimes_A B) \otimes_B (B \otimes_A E')$ since A and B are commutative; the latter product is identified successively with $E \otimes_A (B \otimes_B B) \otimes_A E'$, $E \otimes_A (B \otimes_A E')$, $E \otimes_A (E' \otimes_A B)$ and finally $(E \otimes_A E') \otimes_A B$, using the associativity of the tensor product (\S 3, no. 8, Proposition 8), Proposition 4, \S 3, no. 4, and the commutativity of A and B. The desired isomorphism is the composition of the successive canonical isomorphisms.

Clearly if S is a generating system of E, the image of S under the canonical mapping $E \to E_{(B)}$ is a generating system of $E_{(B)}$; in particular, if E is a finitely generated A-module, $E_{(B)}$ is a finitely generated B-module.

#### Proposition 4 {#alg-ii-s5-prop-4 .statement}

*Let E be an A-module admitting a basis* $(a_\lambda)_{\lambda \in L}$; *if* $\phi : x \mapsto 1 \otimes x$ *is the canonical mapping of E into* $\rho^*(E)$, *then* $(\phi(a_\lambda))_{\lambda \in L}$ *is a basis of* $\rho^*(E)$. *If* $\rho$ *is injective, so is* $\phi$.

The first assertion follows immediately from \S 3, no. 7, Corollary 1 to Proposition 7. Also, for every family $(\xi_\lambda)_{\lambda \in L}$ of elements of A of finite support,

$$
\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = \sum_{\lambda \in L} \rho(\xi_\lambda) \phi(a_\lambda)
$$

and the relation $\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = 0$ is therefore equivalent to $\rho(\xi_\lambda) = 0$ for all $\lambda \in L$, whence the second assertion.

#### Corollary {#alg-ii-s5-n1-cor-2 .statement}

*For every projective A-module E, the B-module* $\rho^*(E)$ *is projective. If further* $\rho$ *is injective, the canonical mapping of E into* $\rho^*(E)$ *is injective.*

By hypothesis there exists a free A-module M containing E and in which E admits a supplement F. It follows immediately from § 3, no. 7, Proposition 7 that $M_{(B)}$ is identified with the direct sum of $E_{(B)}$ and $F_{(B)}$ and if $\phi$ and $\psi$ are the canonical mappings $E \to E_{(B)}$ and $F \to F_{(B)}$, the canonical mapping $M \to M_{(B)}$ is just $x + y \mapsto \phi(x) + \psi(y)$. The corollary follows immediately from Proposition 4 applied to the A-module M.

When E is a right A-module, we write similarly $\rho^*(E) = E \otimes_A \rho_*(B_s)$, B being considered this time as an (A, B)-bimodule and the right B-module structure on $\rho^*(E)$ being such that $(x \otimes \beta)\beta' = x \otimes (\beta\beta')$ for $\beta \in B' \ \beta' \in B$ and $x \in E$. We leave to the reader the task of stating for right modules the results corresponding to those of this no. and the following.

Remark (4). Consider the left A-module $\rho_*(B_s)$ defined by $\rho$ and for every left A-module E, consider the $\mathbf{Z}$-module
$$
\tilde{\rho}(E) = \operatorname{Hom}_A(\rho_*(B_s), E).
$$
As $\rho_*(B_s)$ has a right B-module structure, a left B-module structure is derived on $\tilde{\rho}(E)$ (\S 1, no. 14) such that, if $u \in \tilde{\rho}(E)$ and $b' \in B$, $b'u$ is the homomorphism $b \mapsto u(bb')$ of $\rho_*(B_s)$ into E. We further define an A-linear mapping, called canonical
$$
\eta : \rho_*(\tilde{\rho}(E)) \to E
$$
associating with every homomorphism $u \in \tilde{\rho}(E)$ the element $u(1)$ in E. As B can be considered as an (A, B)-bimodule by means of $\rho$, for every left B-module F, there is a canonical $\mathbf{Z}$-module isomorphism
$$
\operatorname{Hom}_A(\rho_*(B_s) \otimes_B F, E) \to \operatorname{Hom}_B(F, \operatorname{Hom}_A(\rho_*(B_s), E))
$$
(\S 1, no. 1, Proposition 1). As the left A-module $\rho^*(B_s) \otimes_B F$ is canonically identified with $\rho_*(F)$ by virtue of § 3, no. 4, Proposition 4, we obtain a canonical $\mathbf{Z}$-module isomorphism, the inverse of the above
$$
\operatorname{Hom}_B(F, \tilde{\rho}(E)) \to \operatorname{Hom}_A(\rho_*(F), E)
$$
which associates with every B-linear mapping g of F into $\tilde{\rho}(E)$ the composite mapping $\eta \circ g$, considered as an A-linear mapping of $\rho_*(F)$ into E. In particular, under the hypotheses of Proposition 2, if F is replaced by $\sigma_*(C_s)$, we obtain a canonical C-isomorphism
$$
\tilde{\sigma}(\tilde{\rho}(E)) \to (\sigma \circ \rho)^*(E).
$$

### 2. RELATIONS BETWEEN RESTRICTION AND EXTENSION OF THE RING OF SCALARS

Let $\rho : A \to B$ be a ring homomorphism. For every left A-module E, a canonical A-linear mapping
$$
\phi_E : E \to \rho_*(\rho^*(E))
$$
was defined in no. 1 such that $\phi_E(x) = 1 \otimes x$. We consider now a left B-module F and apply Proposition 1 (no. 1) to the A homomorphism $l_{\rho_*(F)} : \rho_*(F) \to \rho_*(F)$: we obtain a B-linear mapping

$$
\psi_F : \rho^*(\rho_*(F)) \to F
$$

equal to $\delta(l_{\rho_*(F)})$ and such therefore that, for all $y \in F$ and all $\beta \in B$,
$\psi_F(\beta \otimes y) = \beta y$.

#### Proposition 5 {#alg-ii-s5-prop-5 .statement}

*Let E be a left A-module and F a left B-module; the composite mappings*

$$
\rho^*(E) \xrightarrow{\rho^*(\phi_E)} \rho^*(\rho_*(\rho^*(E))) \xrightarrow{\psi_{\rho^*(E)}} \rho^*(E)
$$
$$
\rho_*(E) \xrightarrow{\phi_{\rho_*(F)}} \rho_*(\rho^*(\rho_*(F))) \xrightarrow{\rho_*(\psi_F)} \rho_*(F)
$$

*are respectively equal to the identity mappings of $\rho^*(E)$ and $\rho_*(F)$.*

We give the proof, for example, for (12); for all $x \in E$, the mapping $\rho^*(\phi_E)$ maps $1 \otimes x$ to the element $1 \otimes (1 \otimes x)$ and the mapping $\psi_{\rho^*(E)}$ maps $1 \otimes (1 \otimes x)$ to the element $1 \otimes x$; the conclusion follows from the fact that the elements of the form $1 \otimes x$ generate the B-module $\rho^*(E)$; the proof is even simpler for (13).

#### Corollary {#alg-ii-s5-n2-cor-1 .statement}

*The mappings $\rho^*(\phi_E)$ and $\phi_{\rho_*(F)}^*$ are injective and respectively identify $\rho^*(E)$ with a direct factor of $\rho^*(\rho_*(\rho^*(E)))$ and $\rho_*(F)$ with a direct factor of $\rho_*(\rho^*(\rho_*(F)))$.*

This is a consequence of Proposition 5 and § 1, no. 9, Corollary 2 to Proposition 15.

#### Proposition 6 {#alg-ii-s5-prop-6 .statement}

*Let E be a left A-module and F a right B-module. There exists one and only one $\mathbf{Z}$-homomorphism*

$$
\rho_*(F) \otimes_A E \to F \otimes_B \rho^*(E)
$$

*mapping $y \otimes x$ to $y \otimes (1 \otimes x)$ for all $x \in E$ and all $y \in F$ and this homomorphism is bijective.*

By definition the right hand side of (14) is $F \otimes_B (B \otimes_A E)$, where B is considered as a (B, A)-bimodule, and there is a canonical $\mathbf{Z}$-isomorphism $(F \otimes_B B) \otimes_A E \to F \otimes_B (B \otimes_A E)$ defined in § 3, no. 8, Proposition 8; on the other hand, the canonical isomorphism $F \to F \otimes_B B$ of § 3, no. 4, Proposition 4 is an isomorphism for the right A-module structures on the two sides, defined by $\rho$. Whence the desired isomorphism.

When A and B are *commutative*, the isomorphism (14) is an *A-module* isomorphism

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E)).
$$

### 3. EXTENSION OF THE RING OF OPERATORS OF A HOMOMORPHISM MODULE

Let $A$ be a *commutative* ring, $B$ a ring, $\rho : A \to B$ a ring homomorphism and $E, F$ two $A$-modules; as $B$ is an $(A, A)$-bimodule (by means of $\rho$) and $F$ can be considered as an $(A, A)$-bimodule, there are on the $\mathbf{Z}$-module $B \otimes_A F$ *two* $A$-module structures, under which respectively $a(b \otimes y) = (\rho(a)b) \otimes y$ and $a(b \otimes y) = b \otimes (ay)$ for $a \in A,\ b \in B,\ y \in F$. We shall denote the two $A$-modules thus defined by $G'$ and $G''$; $G'$ is moreover just the $A$-module $\rho_*(\rho^*(F))$.

This being so, in the definition of the canonical homomorphism of § 4, no. 2, formula (7), we replace $B$ by $A$, the $B$-module $F$ by the ring $B$ considered as an $A$-module by means of $\rho$ and $G$ by $F$ considered as an $(A, A)$-bimodule; as $A$ is commutative, we may write the *canonical* $\mathbf{Z}$*-homomorphism* obtained as

$$
(15) \quad B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, G'').
$$

On the other hand (no. 1, formula (2)), there is a *canonical* $\mathbf{Z}$*-isomorphism*

$$
(16) \quad \operatorname{Hom}_A(E, G') = \operatorname{Hom}_A(E, \rho_*(\rho^*(F))) \to \operatorname{Hom}_B(\rho^*(E), \rho^*(F)).
$$

Suppose now that $\rho(A)$ is contained in the *centre* of $B$, in which case $\rho$ is also called a *central* homomorphism *(or $\rho$ is said to define an $A$*-algebra* structure on $B$, cf. III, § 1, no. 3)*. Then the $A$-module structures of $G'$ and $G''$ are *identical* and composing the homomorphisms (16) and (15) we thus obtain a canonical $\mathbf{Z}$*-homomorphism*

$$
(17) \quad \omega : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

which is characterized by the fact that, for all $u \in \operatorname{Hom}_A(E, F)$ and all $b \in B$

$$
(18) \quad \omega(b \otimes u) = r_b \otimes u,
$$

where $r_b$ denotes right multiplication by $b$ in $B$.

Moreover, the hypothesis that $\omega$ is a *central* homomorphism implies that $(bb')\rho(a) = b\rho(a))b'$ for $b,\ b'$ in $B$ and $a \in A$; in other words the *right* $B$-module structure of $B_d$ is *compatible* with its $A$-module structure; it thus defines on $B \otimes_A \operatorname{Hom}_A(E, F)$ a *right* $B$*-module* structure (\S 3, no. 4) and also on $F_{(B)} = B \otimes_A F$, and finally, as the left and right $B$-module structures on $F_{(B)}$ are *compatible*, a *right* $B$*-module* structure is also obtained on $\operatorname{Hom}_B(E_{(B)}, F_{(B)})$ (\S 1, no. 14). Then it is immediately verified that (17) is a *right* $B$*-module* homomorphism* for these structures.

#### Proposition 7 {#alg-ii-s5-prop-7 .statement}

*Let $A$ be a commutative ring, $B$ a ring, $\rho : A \to B$ a central homomorphism and $E, F$ two $A$-modules.*

(i) *If B is a projective* (resp. *finitely generated projective*) *A*-module, the homomorphism (17) is injective* (resp. *bijective*).

(ii) *If E is a finitely generated projective A*-module, the homomorphism* (17) *is bijective*.

As (16) is bijective, the proposition follows from § 4, no. 2. Proposition 2, applied to the canonical homomorphism (15).

### 4. DUAL OF A MODULE OBTAINED BY EXTENSION OF SCALARS

Let A, B be two rings, $\rho : A \to B$ a ring homomorphism, E a left A-module and E* its dual. We shall define a canonical B-*linear* mapping

$$
v_E : (E^*)_{(B)} \to (E_{(B)})^*.
$$

The left hand side of (19) may be written as $\mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s)$, where, in $\mathrm{Hom}_A(E, A)$, A is considered as an (A, A)-bimodule. Then there is a canonical $\mathbf{Z}$-homomorphism ($\S 4$, no. 2, formula (7))

$$
v : \mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s) \to \mathrm{Hom}_A(E, A \otimes_A \rho_* (B_s)) = \mathrm{Hom}_A(E, \rho_* (B_s))
$$

with the identification given by the canonical isomorphism of $\S 3$, no. 4, Proposition 4. On the other hand, the right hand side of (19) may be written as $\mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s)$; as B is a (B, A)-bimodule, there is a canonical $\mathbf{Z}$-isomorphism ($\S 4$, no. 1, Proposition 1)

$$
\beta : \mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s) \to \mathrm{Hom}_A(E, \mathrm{Hom}_B(B_s, B_s))
$$

and $\mathrm{Hom}_B(B_s, B_s)$ is canonically identified, as an A-module, with $\rho_* (B_s)$ (see the proof of no. 1, Proposition 1). Taking account of these identifications, we obtain the homomorphism $v_E$; it is easily verified that this homomorphism is characterized by the equation

$$
\langle \xi \otimes x, v_E(x^* \otimes \eta) \rangle = \xi_p (\langle x, x^* \rangle) \eta,
$$

for $x \in E, x^* \in E^*, \xi, \eta$ in B, which shows immediately that $v_E$ is B-*linear*. Moreover, for every A-linear mapping $u : E \to F$ the diagram

$$
\begin{array}{ccc}
(F^*)_{(B)} & \xrightarrow{v_F} & (F_{(B)})^* \\
(tu)_{(B)} \downarrow & & \downarrow t(u_{(B)}) \\
(E^*)_{(B)} & \xrightarrow{v_E} & (E_{(B)})^*
\end{array}
$$

is commutative.

#### Proposition 8 {#alg-ii-s5-prop-8 .statement}

*If one of the A-modules* E, $\rho_* (B_s)$ *is projective and finitely generated, the homomorphism* $v_E$ *is bijective*.

This follows from the above and § 4, no. 2, Proposition 2.

Suppose in particular that E is a finitely generated free A-module and let $(e_i)_{1 \leq i \leq n}$ be a basis of E and $(e_i^*)$ the dual basis; then the canonical isomorphism (19) maps the basis $(e_i^* \otimes 1)$ of $(E^*)_{(B)}$ to the dual basis of the basis $(1 \otimes e_i)$ of $E_{(B)}$.

### 5. A CRITERION FOR FINITENESS

#### Proposition 9 {#alg-ii-s5-prop-9 .statement}

Let B be a ring, A a subring of B and P a projective left A-module. Then, if $P_{(B)}$ is a finitely generated B-module, P is itself a finitely generated A-module.

We know (\S 2, no. 6, Proposition 12) that there exists a family $(a_\lambda)_{\lambda \in L}$ of elements of P and a family $(a_\lambda^*)_{\lambda \in L}$ of elements of the dual P* such that, for all $x \in P$, the family $\langle x, a_\lambda^* \rangle$ is of finite support and $x = \sum_\lambda \langle x, a_\lambda^* \rangle a_\lambda$. Since $P_{(B)}$ is finitely generated, there exists a finite family $(y_i)_{i \in I}$ of elements of P such that $P_{(B)}$ is generated by the elements $1 \otimes y_i$. For each index i, the family $\langle y_i, a_\lambda^* \rangle$ has finite support. Hence there exists a finite subset H of L such that $\langle y_i, a_\lambda^* \rangle = 0$ for $i \in I$ and $\lambda \notin H$. Since
$$
\langle 1 \otimes y_i, 1 d_B \otimes a_\lambda^* \rangle = \langle y_i, a_\lambda^* \rangle,
$$
it follows that $1 d_B \otimes a_\lambda^* = 0$ for $\lambda \notin H$. Hence, for all $x \in P$,
$$
\langle x, a_\lambda^* \rangle = \langle 1 \otimes x, 1_B \otimes a_\lambda^* \rangle = 0
$$
for $\lambda \notin H$. This shows that the A-module P is generated by the $a_\lambda$ such that $\lambda \in H$.

### Exercises {#alg-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
