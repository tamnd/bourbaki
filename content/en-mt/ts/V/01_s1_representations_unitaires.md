---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 1
section_title: Représentations unitaires
lang: en
source: ts-iii-v-fr
book_pages: TS V.373-TS V.398, TS V.483-TS V.486
pdf_pages: 0386-0411, 0496-0499
extraction: native
subsections:
    - "no": 1
      title: Rappels concernant les représentations linéaires continues
      page: 374
      pdf_page: 387
    - "no": 2
      title: Un critère de continuité
      page: 377
      pdf_page: 390
    - "no": 3
      title: Représentations continues de dimension finie
      page: 378
      pdf_page: 391
    - "no": 4
      title: Représentations irréductibles
      page: 378
      pdf_page: 391
    - "no": 5
      title: Représentations unitaires
      page: 379
      pdf_page: 392
    - "no": 6
      title: Somme directe hilbertienne et produit tensoriel de représentations unitaires
      page: 383
      pdf_page: 396
    - "no": 7
      title: Coefficients matriciels
      page: 385
      pdf_page: 398
    - "no": 8
      title: Le lemme de Schur
      page: 386
      pdf_page: 399
    - "no": 9
      title: Semi-simplicité
      page: 390
      pdf_page: 403
    - "no": 10
      title: Classes de représentations unitaires
      page: 392
      pdf_page: 405
    - "no": 11
      title: Composantes isotypiques
      page: 394
      pdf_page: 407
statements: 50
exercises: 7
content_sha256: f1149d81aaad2860301eff5572205d32a2e9786cc132ddd1dbc63f7daad65029
translated_from: content/fr/ts/V/01_s1_representations_unitaires.md
source_lang: fr
translation_method: machine
source_content_sha256: 0b9d89e50b374d026341ed3020e40b83eb74d40a7f3184e3d685e9d2b6f18a27
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-5568f40d
glossary_version: 34
glossary_terms_sha256: f9f59956862f1007be408558c51589817d8f2cb968513dd2fd46819f007339df
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. UNITARY REPRESENTATIONS

In this paragraph, the vector spaces are over $K =\mathbf{R}$ or $\mathbf{C}$.

Recall that a linear representation of a group G in a K-vector space E is a homomorphism $\varrho$ of G into the group $\mathbf{G}\mathbf{L}(E)$ of automorphisms of E (A, VIII, p. 387, Definition 1). One says that E is the space of the representation $\varrho$, and that the dimension of E is the dimension of $\varrho$, which is also denoted dim($\varrho$ ).

One can identify a representation of G in a K-vector space with a K[G]-module (loc. cit.), and the corresponding terminology will be used, for example concerning direct sums of representations, morphisms of representations, or the representation over $\mathbf{C}$ obtained from a representation in an $\mathbf{R}$-vector space by extension of scalars.

A representation $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ is said to be faithful if it is an injective homomorphism.

Care must be taken that this does not mean that the K[G]-module associated with $\varrho$ is a faithful K-module (A, II, p. 28).

The character of a representation of G in a finite-dimensional K-vector space is the mapping $\chi_{\varrho}$ of G into K such that $\chi_{\varrho}(g) =$ Tr($\varrho (g)$) for every $g\in G$, cf. A, VIII, p. 388.

### 1. Reminders concerning continuous linear representations

Let G be a topological group. Recall that a continuous linear representation of G in a topological K-vector space E is a linear representation $\varrho$ of G in E such that the mapping of $G\times E$ into E defined by $(g, x)\mapsto \varrho (g)x$ is continuous (INT, VIII, p. 128, § 2, No.$^o1$, Definition 1). This mapping defines an action of G on E and the image of $\varrho$ is contained in $\mathscr{L}(E)$. A continuous representation $\varrho$ is said to be bounded if its image is bounded in the space $\mathscr{L}(E)$ endowed with the topology of bounded convergence.

#### Remark {#ts-v-s1-n1-rem-1 .statement tag=038J}

If $K =\mathbf{R}$ and if $\varrho$ is a continuous linear representation of G in an $\mathbf{R}$-vector space E, then the mapping $\varrho_{(\mathbf{C})}:g\mapsto 1\otimes \varrho (g)$ is a continuous linear representation of G in $E_{(\mathbf{C})}$; if $\varrho$ is bounded, then $\varrho_{(\mathbf{C})}$ is bounded.

For every topological K-vector space E, the homomorphism which associates $1_E$ with every $g\in G$ is a continuous linear representation of G in E, called the trivial representation of G in E.

Let H be a subgroup of G. The restriction of $\varrho$ to H is a continuous linear representation of H in E, denoted Res$^G_H(\varrho )$.

Let $\varrho_1$ and $\varrho_2$ be continuous linear representations of G in topological K-vector spaces $E_1$ and $E_2$. A G-morphism $u$ of $\varrho_1$ into $\varrho_2$ is a morphism of linear representations which is continuous, that is to say a continuous linear mapping $u: E_1\rightarrow E_2$ such that $u\circ \varrho_1(g) =\varrho_2(g)\circ u$ for every $g\in G$. The vector space of G-morphisms of $\varrho_1$ into $\varrho_2$ is denoted by Hom$_G(\varrho_1, \varrho_2)$. It is a closed subspace of the space $\mathscr{L}(E_1; E_2)$ endowed with the topology of simple convergence.

Let $\varrho$ be a continuous linear representation of a group G in a topological K-vector space E. The identity mapping $1_E$ of E is a G-morphism of $\varrho$ into $\varrho$, denoted by $1_{\varrho}$. If $\varrho_1,\varrho_2$ and $\varrho_3$ are continuous linear representations of G in topological K-vector spaces $E_1, E_2, E_3$ respectively, and if $u: E_1\rightarrow E_2$ and $v: E_2\rightarrow E_3$ are G-morphisms, then $v\circ u$ is a G-morphism.

A G-morphism $u$ from $\varrho_1$ into $\varrho_2$ is a G-isomorphism if there exists a G-morphism $v$ from $\varrho_2$ into $\varrho_1$ such that $v\circ u= 1_{\varrho_1}$ and $u\circ v= 1_{\varrho_2}$. It is necessary and sufficient for this that $u$ be a G-morphism and an isomorphism of topological vector spaces from the space of $\varrho_1$ onto the space of $\varrho_2$; its inverse $v=u^{-1}$ is then in fact a G-morphism. If there exists a G-isomorphism from $\varrho_1$ onto $\varrho_2$, one says that these representations are isomorphic.

#### Definition 1 {#ts-v-s1-def-1 .statement tag=038K}

Let $\varrho$ be a continuous linear representation of a topological group G in a topological vector space E. A continuous linear representation $\pi$ of G in F is a subrepresentation of $\varrho$ if F is a closed subspace of E and if, for every $g\in G$, the space F is stable under $\varrho (g)$ and $\pi (g)$ is the endomorphism of F deduced from $\varrho (g)$ by passing to subspaces.

Let $\varrho$ be a continuous linear representation of a topological group G in a topological vector space E. The closure of $\{0\}$ in E is a subrepresentation of $\varrho$. More generally, the closure of a subspace stable under the endomorphisms $\varrho (g)$ is a subrepresentation of $\varrho$.

A subrepresentation $\pi$ of $\varrho$ is determined in a unique manner by a closed subspace F, stable under all the endomorphisms $\varrho (g)$. This latter condition will often be stated in the form “F is a G-invariant subspace of E”. One will then also say that F defines a subrepresentation of $\varrho$, or sometimes, by abuse of language, that F is a subrepresentation of $\varrho$, or of E.

Let F be a subspace of E defining a subrepresentation $\pi$ of $\varrho$. For every $g\in G$, the linear mapping $\varrho (g)$ defines, by passing to the quotient, an endomorphism $\widetilde{\varrho}(g)$ of $E/F$. The mapping $g\mapsto \widetilde{\varrho}(g)$ is a continuous linear representation of G in $E/F$ and the canonical projection of E onto $E/F$ is a G-morphism. One says that $\widetilde{\varrho}$ is the quotient representation of G on $E/F$; it is also denoted by $\varrho /\pi$.

The subspace of the elements of E invariant under the action of G is a trivial subrepresentation of $\varrho$. It is denoted by $\varrho^G$ or else $E^G$.

Let A be a subset of E. The closed subspace F generated by the elements $\varrho (g)x$, where $g\in G$ and $x\in A$, is a subrepresentation of $\varrho$, called the subrepresentation of $\varrho$ generated by A; if F = E, one says that A generates $\varrho$. If the subrepresentation F is finite-dimensional, one says that the subset A is G-finite.

Suppose that A is reduced to a single element $x\in E$. If A generates $\varrho$, one says that $x$ is a cyclic vector of $\varrho$ and that $\varrho$ is a cyclic representation; one says that $x$ is a G-finite vector if A is G-finite.

The set of G-finite vectors of $\varrho$ is a vector subspace of E stable under $\varrho$; it is not necessarily closed.

Let $(\varrho_i)_{i\in I}$ be a family of continuous linear representations of G in locally convex topological K-vector spaces $(E_i)_{i\in I}$. Let E be the direct sum space of the spaces $E_i$. The mapping $g\mapsto (\varrho_i(g))$ is a linear representation of G in E, called the sum, or direct sum, of the representations $\varrho_i$. If I is finite, it is continuous.

If the representations $\varrho_i$ are all equal to a representation $\varrho$ for every $i\in I$, one says that the direct sum of the representations $\varrho_i$ is the sum of Card(I) copies of the representation $\varrho$, and it is also denoted by $\varrho^{Card(I)}$, or Card(I) $\varrho$.

Let $(\varrho_i)_{i\in I}$ and $(\pi_j)_{j\in J}$ be finite families of continuous linear representations of G in topological K-vector spaces $(E_i)_{i\in I}$ and $(F_j)_{j\in J}$, respectively. The canonical isomorphism of K-vector spaces

Hom$_K(\bigoplus_{i\in I}E_i,\bigoplus_{j\in J}F_j)\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_K(E_i,F_j)$ (A, II, p. 13, Corollary 1) induces, by passing to the subspaces, an isomorphism

(1) Hom$_G(\bigoplus_{i\in I}\varrho_i,\bigoplus_{j\in J}\pi_j)\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_G(\varrho_i, \pi_j)$

which is likewise said to be canonical.

Let $\varrho_1$ and $\varrho_2$ be linear representations of G in topological K-vector spaces $E_1$ and $E_2$. For $u\in \mathscr{L}(E_1; E_2)$ and $g\in G$, one sets $\varrho (g)u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. The mapping $g\mapsto \varrho (g)$ is a linear representation of G in $\mathscr{L}(E_1; E_2)$. The space of the elements invariant under this representation coincides with Hom$_G(\varrho_1, \varrho_2)$.

Let $\varrho$ be a continuous linear representation of G in a locally convex space E. Recall (INT, VIII, p. 131, § 2, n$^o2$) that the contragredient representation $\breve{\varrho}$ of $\varrho$ is the linear representation of G in the dual $E'$ of E defined by $\breve{\varrho}(g) =^t\varrho (g^{-1})$.

### 2. A criterion for continuity

The following result makes it possible to verify that certain linear representations of a direct product of topological groups are continuous.

#### Lemma 1 {#ts-v-s1-lem-1 .statement tag=038L}

Let G and H be topological groups and E a Banach space. Let $\varrho$ be a bounded representation of G in E and $\pi$ a bounded representation of H in E. Suppose that $\varrho (g)$ commutes with $\pi (h)$ for every $(g, h)\in G\times H$. The mapping $\varpi$ of $G\times H$ into $\mathbf{G}\mathbf{L}(E)$ defined by $(g, h)\mapsto \varrho (g)\circ \pi (h)$ is a continuous bounded linear representation of $G\times H$ in E.

The mapping $\varpi$ is a linear representation of $G\times H$ in E; let us verify that it is continuous. Since $\|\varpi (g, h)\|\leqslant \|\varrho (g)\|\|\pi (h)\|$ for every $(g, h)\in G\times H$, the representation $\varpi$ is bounded, and therefore its image is equicontinuous in $\mathscr{L}(E)$. It then suffices to prove that, for every $x\in E$, the mapping $(g, h)\mapsto \varpi (g, h)x$ is continuous (Remark 2 of INT, VIII, p. 129, § 2, n$^o1$). Let $(g_0, h_0)\in G\times H$. Put $y=\pi (h_0)x$. For every $(g, h)\in G\times H$, one has

$$
\|\varpi (g, h)x-\varpi (g_0, h_0)x\|\leqslant \|\varrho (g)(\pi (h)x-y)\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

$$
\leqslant \|\varrho (g)\| \|\pi (h)x-y\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

Since $\varrho$ is bounded and since $\varrho$ and $\pi$ are continuous, this implies the assertion.

### 3. Continuous finite-dimensional representations

Let $\varrho$ be a continuous linear representation of a topological group G in a separated topological K-vector space E of finite dimension. We endow $\mathscr{L}(E)$ with its unique structure of separated topological vector space over K; the morphism $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ is then continuous since the topology of $\mathbf{G}\mathbf{L}(E)$ is induced by the topology of $\mathscr{L}$ (E), which coincides with the topology of simple convergence (TVS, I, p. 14, Theorem 2). Consequently, the character of $\varrho$ is continuous. If G is a real Lie group, then the character of $\varrho$ is an analytic function on G (LIE, III, p. 225, § 8, No. $^o1$, Theorem 1). The contragredient representation is likewise continuous when $E'$ is endowed with its unique topology of separated topological vector space over K. Moreover, for every integer $n\geqslant 0$, the representations $\mathsf{T}^n(\varrho ),\mathsf{S}^n(\varrho )$ and $\wedge^n(\varrho ) ($loc. cit.) are continuous, when the corresponding spaces are endowed with their topologies of separated topological vector spaces over K.

Let $\varrho_1$ and $\varrho_2$ be continuous representations of a topological group G in separated topological vector spaces $E_1$ and $E_2$ of finite dimension. The linear representation $\varrho_1\otimes \varrho_2$ of G in $E_1\otimes E_2$ (LIE, III, p. 256, Appendix) is continuous, the space $E_1\otimes E_2$ being endowed with its topology of separated topological vector space over K.

### 4. Irreducible representations

In this No., G is a topological group.

#### Definition 2 {#ts-v-s1-def-2 .statement tag=038M}

A representation $\varrho$ of G in a topological K-vector space E is said to be irreducible if $\{0\}$ is not dense in E and if the only subrepresentations of $\varrho$ are $\varrho$ and the representation in the closure of $\{0\}$.

If $\varrho$ is an irreducible representation of G in a separated topological vector space E, then every nonzero element of E is a cyclic vector for $\varrho$.

#### Lemma 2 {#ts-v-s1-lem-2 .statement tag=038N}

Let $\pi$ and $\varrho$ be continuous linear representations of G in separated topological K-vector spaces. Suppose that $\pi$ is irreducible. Every nonzero G-morphism from $\pi$ into $\varrho$ is injective, and every nonzero G-morphism from $\varrho$ into $\pi$ has dense image.

In particular, if $\pi$ and $\varrho$ are irreducible and finite-dimensional, then every nonzero G-morphism from $\pi$ into $\varrho$ is an isomorphism.

Since the space of $\varrho$ is separated, the kernel of a G-morphism $u$ from $\pi$ into $\varrho$ is closed, and gives rise to a subrepresentation of $\pi$. If the morphism $u$ is nonzero, its kernel must therefore be reduced to 0, since $\pi$ is an irreducible representation in a separated topological vector space. Similarly, the closure of the image of a nonzero G-morphism from $\varrho$ into $\pi$ is a nonzero subrepresentation of $\pi$, and is therefore equal to the space of $\pi$.

The last assertion follows from the preceding.

#### Lemma 3 {#ts-v-s1-lem-3 .statement tag=038O}

Let $\varrho$ be a continuous linear representation of G in a separated topological K-vector space E of finite dimension. If E is nonzero, then there exists an irreducible subrepresentation of $\varrho$.

Since E is finite-dimensional and nonzero, there exists a G-invariant subspace F of E which is nonzero and of minimal dimension. This subspace is closed in E and defines a subrepresentation of E; every subrepresentation of F is also a subrepresentation of E, and the representation F is therefore irreducible by minimality.

#### Remark {#ts-v-s1-n4-rem-1 .statement tag=038P}

A nonzero representation E of G does not always contain an irreducible subrepresentation (cf. V, p. 426, remark). We shall see, however, that this is the case if G is compact and if $K =\mathbf{C}$ and if E is a separated quasi-complete nonzero locally convex space over K (Proposition 7 of V, p. 464).

### 5. Unitary representations

#### Definition 3 {#ts-v-s1-def-3 .statement tag=038Q}

Let G be a topological group and E a Hilbert space over K. A unitary representation of G in E is a continuous linear representation $\varrho$ of G in E such that, for every $g$ in G, the endomorphism $\varrho (g)$ of E is a unitary endomorphism (TVS, V, p. 40) of E.

In other words, a unitary representation is an isometric representation in a Hilbert space. In particular, a unitary representation is bounded.

The trivial representation of a topological group in a Hilbert space is unitary. Every subrepresentation of a unitary representation is unitary. The restriction of a unitary representation to a subgroup is unitary.

#### Definition 4 {#ts-v-s1-def-4 .statement tag=038R}

Let G be a topological group, and let $\varrho$ and $\pi$ be unitary representations of G in Hilbert spaces E and F respectively. A G-invariant sesquilinear form on $E\times F$ is a continuous sesquilinear form $q$ on $E\times F$ such that

$$
q(x, y) =q(\varrho (g)x, \pi (g)y)
$$

for every $g\in G$ and every $(x, y)\in E\times F$.

The vector space of G-invariant sesquilinear forms on $E\times F$ is denoted by Sesq$_G(\varrho , \pi )$ or Sesq$_G(E,F)$.

#### Example {#ts-v-s1-n5-exa-1 .statement tag=038S}

Let G be a topological group, and let $\varrho$ be a unitary representation of G in E. The scalar product $q$ on E is a G-invariant sesquilinear form on $E\times E$.

#### Lemma 4 {#ts-v-s1-lem-4 .statement tag=038T}

Let G be a topological group, and let $\varrho$ be a homomorphism of G into the unitary group $\mathbf{U}(E)$ of a Hilbert space E. Then $\varrho$ is a unitary representation of G if and only if $\varrho$ is continuous at the element $e$ of G for the topology of simple convergence on $\mathbf{U}(E)$. It is enough that this property be valid for every $x$ in a total subset of E.

The condition is obviously necessary. It is sufficient by Remark 2 of INT, VIII, p. 129, § 2, n$^o1$, since the image of $\varrho$ is equicontinuous in $\mathscr{L}(E)$ and since the continuity of the mapping $g\mapsto \varrho (g)x$ at $e$ implies its continuity on G.

Let G be a topological group. If $\varrho_1$ and $\varrho_2$ are unitary representations of G and if $u$ belong to Hom$_G(\varrho_1, \varrho_2)$, then $u^*$ belong to Hom$_G(\varrho_2, \varrho_1)$. In fact, since $\varrho_1$ and $\varrho_2$ are unitary representations, one has for every $g\in G$

$$
u^*\circ \varrho_2(g) =u^*\circ \varrho_2(g^{-1})^*= (\varrho_2(g^{-1})\circ u)^*
$$

$$
= (u\circ \varrho_1(g^{-1}))^*=\varrho_1(g)\circ u^*
$$

#### Lemma 5 {#ts-v-s1-lem-5 .statement tag=038U}

Let G be a topological group, and let $\varrho$ be a unitary representation of G in a complex Hilbert space E. The space Hom$_G(\varrho , \varrho )$ is a unital involutive subalgebra of $\mathscr{L}(E)$.

What precedes shows that Hom$_G(\varrho , \varrho )$ is a unital self-adjoint subalgebra of $\mathscr{L}(E)$. Since it is closed in $\mathscr{L}$ (E), it is an involutive subalgebra of $\mathscr{L}(E)$.

#### Lemma 6 {#ts-v-s1-lem-6 .statement tag=038V}

Let $\pi$ and $\varrho$ be unitary representations of a topological group G in Hilbert spaces E and F respectively. Let D be a dense subspace of E which is stable under $\pi$. Let $u$ be a closed partial operator from E into F with domain D such that $u\circ \pi (g) =\varrho (g)\circ u$ for every $g\in G$. Then the domain of $u^*$ is stable under $\varrho$ and one has the relation $u^*\circ \varrho (g) =\pi (g)\circ u^*$ for every $g\in G$.

Let $g\in G$ and $x\in$ dom($u^*$). For every $y\in$ dom($u$), one has

$$
\langle \varrho (g)x|u(y)\rangle =\langle x|\varrho (g^{-1})u(y)\rangle =\langle x|u(\pi (g^{-1})y)\rangle
$$

$$
=\langle u^*(x)|\pi (g^{-1})y\rangle =\langle \pi (g)(u^*(x))|y\rangle
$$

since $\varrho (g)^*=\varrho (g)^{-1}=\varrho (g^{-1})$. This proves that $\varrho (g)x\in$ dom($u^*$) and that $u^*(\varrho (g)x) =\pi (g)(u^*(x))$. In particular, the domain of $u^*\circ \varrho (g)$ contains the domain of $u^*$, and $\pi (g)\circ u^*\subset u^*\circ \varrho (g)$.

But moreover, if $x\in$ dom($u^*\circ \varrho (g)$), then $x=\varrho (g^{-1})(\varrho (g)x)$ belongs to dom($u^*$) by what precedes applied to $g^{-1}$. It follows that $u^*\circ \varrho (g) =\pi (g)\circ u^*$.

#### Proposition 1 {#ts-v-s1-prop-1 .statement tag=038W}

Let $\varrho_1$ and $\varrho_2$ be unitary representations of a topological group G in Hilbert spaces $E_1$ and $E_2$. The mapping from Hom$_G(\varrho_1, \varrho_2)$ into Sesq$_G(\varrho_2, \varrho_1)$ which to $u$ associates the sesquilinear form $q_u$ defined by $q_u(x, y) =\langle x|u(y)\rangle$ is an isomorphism of vector spaces.

If $u$ is a G-morphism, then one has

$$
q_u(\varrho_2(g)x, \varrho_1(g)y) =\langle \varrho_2(g)x|u(\varrho_1(g))y\rangle
$$

$$
=\langle \varrho_2(g)x|\varrho_2(g)u(y)\rangle =\langle x|u(y)\rangle =q_u(x, y)
$$

for all $g\in G$ and all $(x, y)\in E_2\times E_1$, hence the indicated mapping is a linear mapping from Hom$_G(\varrho_1, \varrho_2)$ into Sesq$_G(\varrho_2, \varrho_1)$. By EVT, V, p. 16, Corollary 2, it is injective.

Conversely, let $q$ be a G-invariant sesquilinear form and $u$ the unique linear mapping from $E_1$ into $E_2$ such that $q(x, y) =\langle x|u(y)\rangle$ for all $(x, y)\in E_2\times E_1($loc. cit.). For every $g$ in G and every $(x, y)$ in $E_2\times E_1$, one has

$$
\langle x|(\varrho_2(g)\circ u\circ \varrho_1(g^{-1}))(y)\rangle =\langle \varrho_2(g^{-1})x|u(\varrho_1(g^{-1})y)\rangle
$$

$$
=q(\varrho_2(g^{-1})x, \varrho_1(g^{-1})y) =q(x, y) =\langle x|u(y)\rangle
$$

hence $u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. Consequently, $u\in$ Hom$_G(\varrho_2, \varrho_1)$. The proposition follows.

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. If $K =\mathbf{C}$, let $\overline{E}$ denote the conjugate space of E (EVT, V, p. 6). If $K =\mathbf{R}$, put $\overline{E}= E$. The conjugate representation $\overline{\varrho}$ is the representation of G in $\overline{E}$ defined by $\overline{\varrho}(g) =\varrho (g)$ for all $g\in G$. It is a unitary representation of G; by definition, a subspace of $\overline{E}$ is a subrepresentation of $\overline{E}$ if and only if it is a subrepresentation of E.

#### Proposition 2 {#ts-v-s1-prop-2 .statement tag=038X}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. Let $u$ denote the isometric isomorphism of $\overline{E}$ onto $E'$ which associates to $x$ the linear form $y\mapsto  \langle x|y\rangle$.

a) The mapping $u$ is an isomorphism of the conjugate representation $\overline{\varrho}$ onto the contragredient representation $\breve{\varrho}$;

b) Endow $E'$ with the structure of a Hilbert space obtained by transport of structure by means of $u$; the contragredient representation $\breve{\varrho}$ is a unitary representation of G in $E'$.

By EVT, V, p. 15, Theorem 3 and the following remark, the mapping $u$ is an isometric isomorphism.

For every $g$ in G, every $x$ in $\overline{E}$ and every $y$ in E, one has

$$
\langle y,( \breve{\varrho}(g)\circ u)(x)\rangle =\langle \varrho (g^{-1})y, u(x)\rangle
$$

$$
=\langle x|\varrho (g^{-1})y\rangle =\langle \varrho (g)x|y\rangle =\langle y, u(\overline{\varrho}(g)x)\rangle
$$

hence $\breve{\varrho}(g)\circ u=u\circ \overline{\varrho}(g)$, which proves a); assertion b) follows immediately.

#### Corollary {#ts-v-s1-n5-cor-1 .statement tag=038Y}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. The following conditions are equivalent:

(i) The representation $\varrho$ is irreducible;

(ii) The contragredient representation $\breve{\varrho}$ is irreducible;

(iii) The conjugate representation $\overline{\varrho}$ is irreducible.

This results from Proposition 2, and from the remark preceding it concerning the subrepresentations of E.

#### Proposition 3 {#ts-v-s1-prop-3 .statement tag=038Z}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. Let $\pi$ be a subrepresentation of E and F the space of $\pi$. The orthogonal complement $F^{\circ}$ of F in E is a subrepresentation of E such that $E = F\oplus F^{\circ}$ and $F^{\circ}$ is isomorphic to $E/F$.

The space $F^{\circ}$ is closed. For every $x\in F^{\circ}$, every $g\in G$ and every $y\in F$, one has $\langle \varrho (g)x|y\rangle =\langle x|\varrho (g^{-1})y\rangle = 0$ since $\varrho$ is unitary and F is a subrepresentation. Hence $\varrho (g)x\in F^{\circ}$.

The canonical projection of E onto $E/F$ is a G-morphism, hence the mapping of $F^{\circ}$ into $E/F$ which is deduced from it by passing to the subspace is a G-morphism of $F^{\circ}$ into $E/F$; by EVT, V, p. 13, it is an isometric isomorphism.

We shall also denote by $\pi^{\circ}$ the representation of G in $F^{\circ}$.

#### Proposition 4 {#ts-v-s1-prop-4 .statement tag=0390}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. A closed subspace F of E is a subrepresentation of $\varrho$ if and only if the orthogonal projector $p$ of E with image F is a G-morphism of $\varrho$ into $\varrho$.

Suppose that F is a subrepresentation of $\varrho$. Let $x\in E$ and write $x=p(x) +y$ where $y\in F^{\circ}$. For every $g$ in G, one has

$$
\varrho (g)x=\varrho (g)(p(x)) +\varrho (g)y
$$

and as $\varrho (g)(p(x))$ belongs to F and $\varrho (g)y$ to $F^{\circ}$ (Prop. 3), one has $p(\varrho (g)x) =\varrho (g)(p(x))$. Hence $p$ belongs to Hom$_G(\varrho , \varrho )$.

Conversely, if $p\in$ Hom$_G(\varrho , \varrho )$ then $1_E-p$ is a G-morphism, hence F = Ker(1$_E-p$) is a subrepresentation of $\varrho$.

### 6. Hilbert Direct Sum and Tensor Product of Unitary Representations

Let G be a topological group. Let $(\varrho_i)_{i\in I}$ be a family of unitary representations of G in Hilbert spaces $E_i$. Let E be the external Hilbert direct sum space of the $E_i$ (EVT, V, p. 18, Def. 1). For every $g$ in G and every $x= (x_i)_{i\in I}$ in E, one has

$$
\sum_i\|\varrho_i(g)x_i\|^2=\sum_i\|x_i\|^2=\|x\|^2
$$

which proves that $(\varrho_i(g)x_i)_{i\in I}$ is in E and has the same norm as $x$. Thus the element $\varrho (g) : (x_i)_{i\in I}\mapsto (\varrho_i(g)x_i)_{i\in I}$ is a unitary element of $\mathscr{L}(E)$.

#### Lemma 7 {#ts-v-s1-lem-7 .statement tag=0391}

The mapping $g\mapsto \varrho (g)$ is a unitary representation of G in E.

By Lemma 4 of V, p. 380, it is enough to prove that for every $i$ in I and every $x$ in $E_i$, the mapping $g\mapsto \varrho (g)x$ is continuous at the identity element $e$ of G. This mapping is the composition of the continuous mapping $g\mapsto \varrho_i(g)x_i$ and the canonical injection of $E_i$ into E. It is therefore continuous.

The representation $\varrho$ is called the Hilbert sum of the unitary representations $(\varrho_i)_{i\in I}$; it is denoted by $\varrho =\bigoplus_{i\in I}\varrho_i$.

Let G and H be topological groups. Let $\varrho_1$ (resp. $\varrho_2$) be a unitary representation of G (resp. H) in a Hilbert space $E_1$ (resp. $E_2$). Let $E = E_1\widehat{\otimes}_2E_2$ be the Hilbert tensor product space of $E_1$ and $E_2$ (EVT, V, p. 28, Def. 1). For $(g, h)\in G\times H$, let $\varrho (g, h)$ be the continuous endomorphism $\varrho_1(g)\widehat{\otimes}_2\varrho_2(h)$ of E (EVT, V, p. 28) ; it will be denoted simply by $\varrho_1(g)\otimes \varrho_2(h)$ when there is no danger of ambiguity.

#### Lemma 8 {#ts-v-s1-lem-8 .statement tag=0392}

a) The mapping $\varrho : (g, h)\mapsto \varrho (g, h)$ is a unitary representation of $G\times H$ in E ;

b) For every orthonormal basis $(e_i)_{i\in I}$ of $E_1$, the mapping from the Hilbert sum $\bigoplus_{i\in I}E_2$ into E defined by $(y_i)_{i\in I}\mapsto \sum_{i\in I}e_i\otimes y_i$ is an isometric H-isomorphism of the Hilbert sum $\bigoplus_{i\in I}\varrho_2$ onto Res$^{G\times H}_{\{e\}\times H}(\varrho )$;

c) For every orthonormal basis $(f_j)_{j\in J}$ of $E_2$, the mapping from the Hilbert sum $\bigoplus_{j\in J}E_1$ into E defined by $(x_j)_{j\in J}\mapsto \sum_{j\in J}x_j\otimes f_j$ is an isometric G-isomorphism of the Hilbert sum $\bigoplus_{j\in J}\varrho_1$ onto Res$^{G\times H}_{G\times \{e\}}(\varrho )$.

The mapping $(g, h)\mapsto \varrho (g, h)$ is a homomorphism of G into $\mathbf{G}\mathbf{L}(E) ($cf. EVT, V, p. 28, n$^o2)$. Let $(e_i)_{i\in I}$ be an orthonormal basis of $E_1$. By EVT, V, p. 29, prop. 3 and cor. 2, the mapping

$$
u: (y_i)\mapsto \sum_{i\in I}e_i\otimes y_i
$$

is an isometry of the Hilbert direct sum $F_2=\bigoplus_{i\in I}E_2$ onto E. By means of this isometry, the representation $\varrho_H:h\mapsto \varrho (e, h)$ of H in E is identified with the direct-sum representation of the representations $(\varrho_2)_{i\in I}$ in $F_2$. In particular, it is a unitary representation of H in E (lemma 7). Analogously, the homomorphism $\varrho_G:g\mapsto \varrho (g, e)$ is a unitary representation of G in E.

Let $(g, h)\in G\times H$. We have $\varrho (g, h) =\varrho_G(g)\circ \varrho_H(h)$; therefore $\varrho (g, h)$ is unitary; moreover, $\varrho_G(g)$ and $\varrho_H(h)$ commute, hence lemma 1 of V, p. 377 implies that $\varrho$ is a unitary representation of $G\times H$.

Finally, the assertions concerning the restriction of $\varrho$ to the subgroups $\{e\} \times H$ and $G\times  \{e\}$ were obtained in the course of the preceding argument.

The representation $(g, h)\mapsto \varrho_1(g)\otimes \varrho_2(h)$ of $G\times H$ is called the external tensor product of the unitary representations $\varrho_1$ and $\varrho_2$, and is denoted by $\varrho_1\boxtimes \varrho_2$.

Let $n\in \mathbf{N}$ and let $(G_i)_{1\leqslant i\leqslant n}$ be a finite family of topological groups. Let $\varrho_i$ be a unitary representation of $G_i$ in a Hilbert space $E_i$ for $1\leqslant i\leqslant n$. One defines analogously a representation

$$
\varrho_1\boxtimes \cdots \boxtimes \varrho_n
$$

of $G_1\times  \cdots  \times G_n$ in the Hilbert space $E = E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n$ (EVT, V, p. 27).

Suppose that $G_i= G$ for $1\leqslant i\leqslant n$. Let $\Delta_n: G\rightarrow G^n$ be the homomorphism defined by $g\mapsto (g, . . . , g)$ for every $g\in G$. One denotes by $\varrho_1\otimes  \cdots  \otimes \varrho_n$ the unitary representation $(\varrho_1\boxtimes \cdots \boxtimes \varrho_n)\circ \Delta_n$ of G. One says that it is the tensor product of the unitary representations $\varrho_i$.

For every permutation $\sigma$ of $\{1, . . . , n\}$, the canonical isomorphism

$$
E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n\rightarrow E_{\sigma(1)}\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_{\sigma(n)}
$$

(EVT, V, p. 28) is an isometric isomorphism

$$
\varrho_1\otimes  \cdots  \otimes \varrho_n\rightarrow \varrho_{\sigma(1)}\otimes  \cdots  \otimes \varrho_{\sigma(n)}
$$

of representations of G.

If $\varrho_i=\varrho$ for $1\leqslant i\leqslant n$, where $\varrho$ is a unitary representation of G, one also denotes by $\varrho^{\otimes n}$ the tensor-product representation of the $\varrho_i$, and one says that it is the $n^e$ tensor power of $\varrho$.

### 7. Matrix coefficients

#### Definition 5 {#ts-v-s1-def-5 .statement tag=0393}

Let G be a topological group and let $\varrho$ be a unitary representation of G in a Hilbert space E. Let $x$ and $y$ be elements of E. The function from G into K given by $g\mapsto  \langle x|\varrho (g)y\rangle$ is called a matrix coefficient of $\varrho$, or a representative function. If $x=y$, it is said to be a diagonal matrix coefficient. If $\varrho$ is finite-dimensional, it is said to be a finite-dimensional matrix coefficient.

The matrix coefficients of $\varrho$ are continuous bounded functions on G. We denote by Υ(G) (resp. Θ(G)) the set of matrix coefficients of complex unitary representations (resp. complex finite-dimensional unitary representations) of G.

#### Proposition 5 {#ts-v-s1-prop-5 .statement tag=0394}

Let G be a topological group. The sets Θ(G) and Υ(G) are unital involutive subalgebras of $\mathscr{C}_b(G)$.

The constant function 1 is a matrix coefficient of the trivial representation of G on $\mathbf{C}$. Let $\varrho$ be a unitary representation of G and let $x$ and $y$ be vectors of the space of $\varrho$. For every $\lambda \in \mathbf{C}$ and every $g\in G$, we have $\lambda \langle x|\varrho (g)y\rangle =\langle x|\varrho (g)(\lambda y)\rangle$. Moreover, we have

$$
\langle x|\varrho (g)y\rangle =\langle \varrho (g^{-1})x|y\rangle =\overline{\langle y|\varrho(g^{-1})x\rangle}
$$

for every $g\in G$. Consequently, the sets Θ(G) and Υ(G) are stable under multiplication by scalars and under conjugation.

Let $\varrho_1$ and $\varrho_2$ be unitary representations of G; let $(x_1, y_1)$ be vectors of the space of $\varrho_1$ and $(x_2, y_2)$ vectors of the space of $\varrho_2$. For every $g\in G$, we then have

$$
\langle x_1|\varrho_1(g)y_1\rangle +\langle x_2|\varrho_2(g)y_2\rangle =\langle (x_1, x_2)|(\varrho_1\oplus \varrho_2)(g)(y_1, y_2)\rangle
$$

$$
\langle x_1|\varrho_1(g)y_1\rangle \langle x_2|\varrho_2(g)y_2\rangle =\langle x_1\otimes x_2|(\varrho_1\otimes \varrho_2)(g)(y_1\otimes y_2)\rangle
$$

which proves that Θ(G) and Υ(G) are stable under addition and multiplication. The proposition follows.

### 8. Schur’s Lemma

In this No., the Hilbert spaces are complex.

#### Proposition 6 (Schur’s Lemma) {#ts-v-s1-prop-6 .statement tag=0395}

Let $\varrho$ be a unitary representation of a topological group G in a nonzero Hilbert space E. Then $\varrho$ is irreducible if and only if Hom$_G(\varrho , \varrho )$ is equal to $\mathbf{C}\cdot 1_E$.

The space Hom$_G(\varrho , \varrho )$ is a unital stellar subalgebra of $\mathscr{L}(E)$ (lemma 5 of V, p. 380). For every subrepresentation F of E, the orthogonal projector $p$ with image F is an idempotent element of the stellar algebra Hom$_G(\varrho , \varrho )$ (prop. 4 of V, p. 383). If the latter is equal to $\mathbf{C}\cdot 1_E$, this means that $p= 0$ or $p= 1_E$, which means that F = 0 or F = E. Hence $\varrho$ is irreducible.

Conversely, suppose $\varrho$ irreducible. Let $u$ and $v$ be permutable elements of the stellar algebra Hom$_G(\varrho , \varrho )$ such that $uv= 0$. Suppose $u$ nonzero. Then the kernel F of $u$ defines a subrepresentation of $\varrho$ different from E, hence F is reduced to 0; since F contains the image of $v$, it follows that $v= 0$. By proposition 10 of I, p. 113, we therefore have Hom$_G(\varrho , \varrho ) =\mathbf{C}\cdot 1_E$.

#### Corollary 1 {#ts-v-s1-prop-6-cor-1 .statement tag=0396}

Let $\pi$ be an irreducible unitary representation of a topological group G in a Hilbert space E. Let $u$ be a closed partial operator on E. Suppose that $u$ has dense domain, that dom($u$) is stable under $\pi$ and that $u\circ \pi (g) =\pi (g)\circ u$ for all $g\in G$. Then dom($u$) $= E$ and $u$ is a homothety.

The partial operator $u^*\circ u$ is a positive self-adjoint partial operator on E (Prop. 12 of IV, p. 241); the same is true of $v= 1_E+u^*\circ u$, and the latter is injective since $-1\notin$ Sp($u^*\circ u$) (Prop. 17 of IV, p. 248). We have $u^*\circ \pi (g) =\pi (g)\circ u^*$ for all $g\in G$ (Lemma 6 of V, p. 381), whence $v\circ \pi (g) =\pi (g)\circ v$ for all $g\in G$. Since $v$ is injective, it follows that $v^{-1}\circ \pi (g) =\pi (g)\circ v^{-1}$ for all $g\in G$. But $v^{-1}$ belongs to $\mathscr{L}$ (E), hence by Prop. 6 there exists $\lambda \in \mathbf{C}$ such that $v^{-1}=\lambda 1_E$. Necessarily $\lambda \not = 0$, which implies that E = Im($v^{-1}$) $=$ dom($v$)$\subset$ dom($u$), whence dom($u$) $= E$. Since $u$ is closed, we have $u\in \mathscr{L}(E)$ (TVS, I, p. 19, Cor. 5), hence $u\in$ Hom$_G(\pi , \pi )$ and $u$ is a homothety by Prop. 6.

#### Corollary 2 {#ts-v-s1-prop-6-cor-2 .statement tag=0397}

Let $\varrho$ and $\pi$ be irreducible unitary representations of a topological group G in Hilbert spaces E and F respectively. The space Hom$_G(\varrho , \pi )$ is of dimension 1 if $\varrho$ is isomorphic to $\pi$, and is zero otherwise. In particular, if $\varrho$ is isomorphic to $\pi$, every nonzero G-morphism of $\varrho$ into $\pi$ is an isomorphism.

Suppose there exists a nonzero G-morphism $u$ of $\varrho$ into $\pi$. The linear mapping $u^*\circ u$ is an element of Hom$_G(\varrho , \varrho )$, hence there exists a complex number $\lambda$ such that $u^*\circ u=\lambda \cdot 1_E$ (Prop. 6). We then have

$$
\langle u(x)|u(y)\rangle =\langle x|u^*u(y)\rangle =\lambda \langle x|y\rangle
$$

for all $x$ and $y$ in E. In particular, $\lambda \not = 0$ since $u$ is nonzero. Since $\|u(x)\|=|\lambda |^{1/2}\|x\|$ for all $x\in E$, the linear mapping $u$ is injective, and the image of $u$ is closed in F (Lemma 8 of I, p. 107); it is therefore a nonzero subrepresentation of the irreducible representation $\pi$, whence one deduces that $u$ is surjective. Thus, $u$ is an isomorphism of $\varrho$ onto $\pi$. The mapping $v\mapsto u^*\circ v$ is then an isomorphism of the space Hom$_G(\varrho , \pi )$ onto the space Hom$_G(\varrho , \varrho )$, which is of dimension 1 (Prop. 6).

#### Corollary 3 {#ts-v-s1-prop-6-cor-3 .statement tag=0398}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. The representation $\varrho$ is irreducible if and only if the space Sesq$_G(\varrho , \varrho )$ is of dimension 1. This space is then generated by the scalar product on E.

In view of Prop. 1 of V, p. 381, this follows from Prop. 6.

#### Corollary 4 {#ts-v-s1-prop-6-cor-4 .statement tag=0399}

Let $\varrho_1$ and $\varrho_2$ be non-isomorphic irreducible unitary representations of a topological group G in Hilbert spaces $E_1$ and $E_2$. The space Sesq$_G(\varrho_1, \varrho_2)$ is zero.

According to Prop. 1 of V, p. 381, this follows from Cor. 2.

#### Corollary 5 {#ts-v-s1-prop-6-cor-5 .statement tag=039A}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. Let $\pi$ be an irreducible unitary representation of G in a Hilbert space F.

a) For every nonzero G-morphism $u$ of $\pi$ into $\varrho$, there exists $\lambda \in \mathbf{R}^*_+$ such that $\lambda u$ is isometric;

b) Every G-morphism $u$ of $\pi$ into $\varrho$ has closed image;

c) Every nonzero G-morphism $v$ of $\varrho$ into $\pi$ is surjective.

Let us prove assertion a), which implies assertion b) (Lemma 8 of I, p. 107). Since the morphism $u$ is nonzero, it is injective (Lemma 2 of V, p. 378). The formula $q(x, y) =\langle u(x)|u(y)\rangle$ for $x$ and $y$ in F then defines a continuous sesquilinear form on F. Since $u$ is a G-morphism, one has $q(\pi (g)x, \pi (g)y) =q(x, y)$ for all $g$ in G and $(x, y)\in F\times F$, hence $q$ is G-invariant. By Cor. 3, there exists $\alpha \in \mathbf{R}^*_+$ such that

$$
q(x, y) =\langle u(x)|u(y)\rangle =\alpha \langle x|y\rangle
$$

for every $(x, y)\in F\times F$, and therefore $\alpha^{-1/2}u$ is isometric.

Let us finally prove assertion c). Since $\pi$ is irreducible, the image of $v$ is dense in F (Lemma 2 of V, p. 378), hence the adjoint $v^*$ is injective (TVS, V, p. 41, Prop. 4). By b), the image H of $v^*$ is a closed subspace of E; it is therefore a subrepresentation of $\varrho$, and $v^*$ induces by passing to the subspaces a G-isomorphism of F onto H. The restriction $w$ of $v$ to H defines a G-morphism of H into F, which is injective since its kernel is the intersection of H and Ker($v$) $= H^{\circ}$ (loc. cit.). The mapping $w$ is therefore an isomorphism (Corollary 2); in particular, $v$ is surjective.

#### Corollary 6 {#ts-v-s1-prop-6-cor-6 .statement tag=039B}

Let $G_1$ and $G_2$ be topological groups. Let $\varrho_1$ be an irreducible unitary representation of $G_1$ in a Hilbert space $E_1$ and $\varrho_2$ an irreducible unitary representation of $G_2$ in a Hilbert space $E_2$. The external tensor product $\varrho_1\boxtimes \varrho_2$ is an irreducible unitary representation of $G_1\times G_2$ in $E_1\widehat{\otimes}_2E_2$.

The external tensor product $\varrho =\varrho_1\boxtimes \varrho_2$ is a unitary representation of $G = G_1\times G_2$ in the space $E = E_1\widehat{\otimes}_2E_2$ by Lemma 8 of V, p. 384.

Let $q$ be a $(G_1\times G_2$)-invariant sesquilinear form on E. For every pair $(x_1, y_1)\in E^2_1$, the mapping $(x_2, y_2)\mapsto q(x_1\otimes x_2, y_1\otimes y_2)$ belong to Sesq$_{G_2}(\varrho_2, \varrho_2)$. Let us denote by $b(x_1, y_1)$ the unique complex number such that

$$
q(x_1\otimes x_2, y_1\otimes y_2) =b(x_1, y_1)\langle x_2|y_2\rangle
$$

for every $(x_2, y_2)\in E^2_2$ (Cor. 3). Let $\varepsilon \in E_2$ be of norm 1, so that $b(x_1, y_1) =q(x_1\otimes \varepsilon , y_1\otimes \varepsilon )$ for every $(x_1, y_1)\in E^2_1$. This formula implies that the mapping $b$ is sesquilinear on $E_1$. Moreover

$$
\|b(x_1, y_1)\|\leqslant \|q\| \|x_1\otimes \varepsilon \| \|y_1\otimes \varepsilon \|=\|q\| \|x_1\| \|y_1\|
$$

for every $(x_1, y_1)\in E^2_1$ (TVS, V, p. 26, formula (5)), hence $b$ is continuous.

Let $g\in G$ and $(x_1, y_1)\in E^2_1$. Since $\varrho_2$ is unitary and $q$ is invariant, we get

$$
b(\varrho_1(g)x_1, \varrho_1(g)y_1) =q(x_1\otimes \varrho_2(g^{-1})\varepsilon , y_1\otimes \varrho_2(g^{-1})\varepsilon ) =b(x_1, y_1)
$$

so that $b\in$ Sesq$_{G_1}(\varrho_1, \varrho_1)$. There therefore exists a unique $\lambda \in \mathbf{C}$ such that $b(x_1, y_1) =\lambda \langle x_1|y_1\rangle$ for every $(x_1, y_1)\in E^2_1$ (Cor. 3), that is to say

$$
q(x_1\otimes x_2, y_1\otimes y_2) =\lambda \langle x_1|y_1\rangle \langle x_2|y_2\rangle
$$

for every $(x_1, y_1, x_2, y_2)\in E^2_1\times E^2_2$. It follows that the space Sesq$_{G_1\times G_2}(\varrho , \varrho )$ is of dimension 1, which implies that the representation $\varrho =\varrho_1\boxtimes \varrho_2$ is irreducible (loc. cit.).

We recall that $\mathbf{U}$ denotes the group of complex numbers of modulus 1.

#### Corollary 7 {#ts-v-s1-prop-6-cor-7 .statement tag=039C}

Let $\pi$ be an irreducible unitary representation of a topological group G in a Hilbert space E. There exists a continuous homomorphism $\chi$ of the center C of G into $\mathbf{U}$ such that $\pi (z) =\chi (z)\cdot 1_E$ for all $z\in C$. In particular, if G is commutative, one has dim(E) = 1.

For $z\in C$, the mapping $\pi (z)$ belong to Hom$_G(\pi , \pi )$; it is therefore of the form $\chi (z)\cdot 1_E$ for a certain complex number $\chi (z)$ (prop. 6). Since $\pi (z)$ is a unitary mapping, one has $|\chi (z)|= 1$. Moreover, since $\pi$ is a homomorphism, the mapping $z\mapsto \chi (z)$ is a homomorphism. Let us fix $v\not = 0$ in E; the mapping $z\mapsto \chi (z)v=\pi (z)v$ of C into $\mathbf{U}$ is continuous, and therefore the homomorphism $\chi$ is continuous.

Finally, if G is commutative, one has C = G, hence $\pi (g) =\chi (g)\cdot 1_E$ for all $g$ in G; every subspace of dimension 1 of E is then a subrepresentation of $\pi$, and since $\pi$ is irreducible, the space E must be of dimension 1.

#### Definition 6 {#ts-v-s1-def-6 .statement tag=039D}

Let $\pi$ be an irreducible unitary representation of a topological group G in a Hilbert space E. The homomorphism $\chi$ of the center C of G into $\mathbf{U}$ such that $\pi (z) =\chi (z)\cdot 1_E$ for all $z$ in C is called the central character of $\pi$.

#### Remark {#ts-v-s1-n8-rem-1 .statement tag=039E}

Let $\pi$ (resp. $\varrho$ ) be an irreducible unitary representation of a topological group G (resp. H) in a Hilbert space E (resp. F). Let $\chi$ (resp. $\eta$ ) denote the central character of $\pi$ (resp. $\varrho$ ). The central character of the representation $\overline{\pi}$ is $\overline{\chi}$, and the central character of the irreducible unitary representation $\pi \boxtimes \varrho$ of $G\times H$ (cor. 6) is the character $\chi \boxtimes \eta : (g, h)\mapsto \chi (g)\eta (h)$ of $G\times H$.

### 9. Semisimplicity

#### Definition 7 {#ts-v-s1-def-7 .statement tag=039F}

Let $\varrho$ be a unitary representation of a topological group G in a Hilbert space E. One says that $\varrho$ is semisimple if there exists a family $(F_i)_{i\in I}$ of irreducible subrepresentations of $\varrho$ such that E is the Hilbert sum of the subspaces $F_i$.

One sometimes also says that a semisimple unitary representation admits a discrete decomposition or is discretely decomposable.

If $(\varrho_i)_{i\in I}$ is a family of semisimple unitary representations of a topological group G, then the Hilbert sum of the representations $\varrho_i$ is semisimple.

#### Proposition 7 {#ts-v-s1-prop-7 .statement tag=039G}

Let G be a topological group and let $\varrho$ be a unitary representation of G in a complex Hilbert space E. The representation $\varrho$ is semisimple if and only if every non-zero subrepresentation of $\varrho$ contains an irreducible subrepresentation.

Suppose that $\varrho$ is semisimple. Let $(F_i)_{i\in I}$ be a family of irreducible subrepresentations of $\varrho$ such that E is the Hilbert sum of the subspaces $F_i$. Let F be a nonzero subrepresentation of E. There exists $i\in I$ such that the restriction to F of the orthogonal projector with image $F_i$ is nonzero. This orthogonal projector then defines by passing to subspaces a nonzero G-morphism $p_i$ of F into $F_i$ (Prop. 4 of V, p. 383). By Schur’s Lemma, the G-morphism $p_i$ is surjective (Cor. 5 of V, p. 388). The orthogonal complement in F of the kernel of $p_i$ is a subrepresentation of F isomorphic to $F_i$ (Prop. 3 of V, p. 383), hence irreducible.

Let us prove the converse assertion. Let $\mathscr{F}$ be the set of closed subspaces F of E stable under G such that the subrepresentation of $\varrho$ in F is irreducible. Let $\mathscr{O}$ be the set of subsets $\mathscr{G}$ of $\mathscr{F}$ such that the subspaces belonging to $\mathscr{G}$ are pairwise orthogonal.

The set $\mathscr{O}$ is of finite character (E, III, p. 34, Def. 2). Let then $\mathscr{G}$ be a maximal element of $\mathscr{O}$ (E, III, p. 35, Th. 1). Let $E_1$ be the subspace of E which is the Hilbert sum of the irreducible subrepresentations F of $\mathscr{G}$. If one had $E_1\not = E$, the orthogonal complement of $E_1$ would not be zero, and the subrepresentation of G in $E^{\circ}_1$ would contain by hypothesis an irreducible subrepresentation. The space F of the latter would be orthogonal to the elements of $\mathscr{G}$, so that $\mathscr{G}\cup  \{F\} \in \mathscr{O}$; this contradicts the maximality of $\mathscr{G}$, therefore $E = E_1$, which completes the proof.

#### Corollary 1 {#ts-v-s1-prop-7-cor-1 .statement tag=039H}

Let G be a topological group and let $\varrho$ be a semisimple unitary representation of G in a complex Hilbert space E. Every subrepresentation of $\varrho ($resp. every quotient representation of $\varrho )$ is semisimple.

If $\varrho_1$ is a subrepresentation of $\varrho$, then every nonzero subrepresentation of $\varrho_1$ contains an irreducible subrepresentation (Prop. 7), hence $\varrho_1$ is semisimple (loc. cit.).

By Prop. 3 of V, p. 383, every quotient representation of $\varrho$ is isomorphic to a subrepresentation of $\varrho$, hence is semisimple.

#### Corollary 2 {#ts-v-s1-prop-7-cor-2 .statement tag=039I}

Every finite-dimensional unitary representation $\varrho$ of a topological group G is semisimple.

This follows from Prop. 7 and Lemma 3 of V, p. 379.

#### Corollary 3 {#ts-v-s1-prop-7-cor-3 .statement tag=039J}

Let $\varrho_1$ and $\varrho_2$ be finite-dimensional unitary representations of a topological group G. The representations $\varrho_1$ and $\varrho_2$ are isomorphic if and only if $\chi_{\varrho_1}=\chi_{\varrho_2}$.

This follows from Corollary 2 and A, VIII, p. 389, Prop. 1, b).

### 10. Classes of unitary representations

#### Lemma 9 {#ts-v-s1-lem-9 .statement tag=039K}

Let E be a Hilbert space over K. Let $F\subset E$ be a vector subspace dense in E. Then the Hilbert dimension of E is less than or equal to the dimension of F.

If E is of finite Hilbert dimension, this is equal to the dimension of E. Suppose that E is of infinite Hilbert dimension. Then the subspace F is of infinite dimension. Let B be an orthonormal basis of E and let $B'$ be a basis of F. For every $x\in B$, there exists an element $f(x)\in B'$ such that $\langle x|f(x)\rangle  \not = 0$, since otherwise one would have $x\in F^{\circ}=\{0\}$. Thus one defines a mapping $f: B\rightarrow B'$.

For every $y\in B'$, the set $\overset{-1}{f}(y)$ is contained in the set of $x\in B$ such that $\langle x|y\rangle  \not = 0$, hence is denumerable (EVT, V, p. 21, Prop. 4). By E, III, p. 50, Prop. 4, one obtains Card(B) = Card($f(B)$)$\leqslant$ Card(B$'$).

Let us denote by $Is_G(\pi_1, \pi_2)$ the relation

“G is a topological group and $\pi_1,\pi_2$ are isomorphic unitary representations

of G in Hilbert spaces over K”.

With respect to $\pi_1$ and $\pi_2$, this is an equivalence relation. For every unitary representation $\pi$ of G in a Hilbert space over K, we denote by cl($\pi$ ) the equivalence class of $\pi ($cf. E, II, p. 47); thus it is a unitary representation of G isomorphic to $\pi$; one says that cl($\pi$ ) is the class of $\pi$. Unitary representations $\pi_1$ and $\pi_2$ in Hilbert spaces over K are isomorphic if and only if cl($\pi_1$) $=$ cl($\pi_2$).

Let G be a topological group. Let $\mathfrak{c}$ be a cardinal. The relation

" $\lambda$ is a class of unitary representation of G in

a complex Hilbert space of Hilbert dimension $\leqslant \mathfrak{c}$ "

is collectivizing in $\lambda$ (E, II, p. 3). In fact, every Hilbert space over K of dimension $\leqslant \mathfrak{c}$ is isometrically isomorphic to a Hilbert subspace of $\ell^2(\mathfrak{c})$ (EVT, V, p. 23, cor. 2), and the assertion then follows from E, II, p. 47.

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. Let $x$ be a nonzero element of E. Since $\pi$ is irreducible, the vector $x$ is a cyclic vector of $\pi$, which implies that the Hilbert dimension of E is $\leqslant$ Card(G) (lemma 9, applied to the dense subspace generated by the elements $\pi (g)x$ for $g\in G$). The classes of irreducible unitary representations of G in a Hilbert space over K therefore belong to the set of classes of unitary representations of G in a Hilbert space over K of Hilbert dimension $\leqslant$ Card(G) ; consequently, they form a set.

#### Definition 8 {#ts-v-s1-def-8 .statement tag=039L}

We denote by $\widehat{G}$ the set of classes of irreducible unitary representations of G in a complex Hilbert space. One says that $\widehat{G}$ is the unitary dual of G.

For every irreducible unitary representation $\pi$ of G in a complex Hilbert space, one therefore has cl($\pi$ )$\in \widehat{G}$.

#### Remark 1 {#ts-v-s1-n10-rem-1 .statement tag=039M}

Suppose that G is a commutative group. By corollary 7 of V, p. 390, every irreducible unitary representation of G in a complex Hilbert space is of dimension 1. If G is locally compact, the set $\widehat{G}$ is identified with the set of unitary characters of G (def. 1 of II, p. 201), and the notation $\widehat{G}$ is therefore compatible with that introduced in def. 2 of II, p. 201.

#### Remark 2 {#ts-v-s1-n10-rem-2 .statement tag=039N}

If G is finite, the set $\widehat{G}$ is in bijection with the set of classes of simple $\mathbf{C}$[G]-modules (A, VIII, p. 47), which is also denoted by $\widehat{G}$ in A, VIII, p. 396.

#### Remark 3 {#ts-v-s1-n10-rem-3 .statement tag=039O}

For $\pi \in \widehat{G}$, we shall identify $\overline{\pi}$ with the class in $\widehat{G}$ of the conjugate representation of $\pi$.

#### Remark 4 {#ts-v-s1-n10-rem-4 .statement tag=039P}

If $\pi$ is an irreducible unitary representation of G in a finite-dimensional complex Hilbert space, its character $\chi_{\pi}$ depends only on the class of $\pi$. One may therefore speak of the set of characters of finite-dimensional complex irreducible unitary representations of G.

### 11. Isotypical Components

#### Definition 9 {#ts-v-s1-def-9 .statement tag=039Q}

Let G be a topological group and let $\pi$ be an irreducible continuous representation of G. Let $\varrho$ be a continuous representation of G in a separated locally convex space E. The $\pi$-isotypical component of $\varrho$ is the closure in E of the sum of the spaces of all the subrepresentations of $\varrho$ isomorphic to $\pi$. This subspace is denoted by $M_{\pi}(\varrho )$.

The space $M_{\pi}(\varrho )$ is a closed subspace of E, which defines a subrepresentation of $\varrho$. This space depends only on the class of $\pi$ in $\widehat{G}$.

#### Proposition 8 {#ts-v-s1-prop-8 .statement tag=039R}

Let G be a topological group. Let $\varrho$ be a unitary representation of G in a complex Hilbert space E.

a) Let $\pi_1$ and $\pi_2$ be non-isomorphic irreducible unitary representations of G. The subspaces $M_{\pi_1}(\varrho )$ and $M_{\pi_2}(\varrho )$ are orthogonal;

b) Let $\varrho '$ be a unitary representation of G and $u$ a G-morphism of $\varrho$ into $\varrho '$. For every irreducible unitary representation $\pi$ of G, one has $u(M_{\pi}(\varrho ))\subset M_{\pi}(\varrho ')$.

Let $E_1$ and $E_2$ be subspaces of E defining subrepresentations isomorphic to $\pi_1$ and $\pi_2$ respectively. The orthogonal projector of E with image $E_2$ defines, by passing to the subspaces, an element of Hom$_G(\pi_1, \pi_2)$, which is zero (Cor. 2 of V, p. 387), and this proves that $E_2$ is orthogonal to $E_1$. This implies assertion a).

As for assertion b), note that $M_{\pi}(\varrho )$ is, by definition, the closure in E of the space generated by the elements $x\in E$ belonging to a closed subspace $F\subset E$ stable under $\varrho$ such that the subrepresentation $\varrho_F$ of $\varrho$ in F is isomorphic to $\pi$. It is therefore enough to prove that, in this case, one has $u(x)\in M_{\pi}(\varrho ')$. Let $H =u(F)$; it is a closed subspace of the space of $\varrho '$ (Cor. 5 of V, p. 388) stable under $\varrho '$, and $u$ induces, by passing to the subspaces, a surjective G-morphism of F onto H. If H is non-zero, then this G-morphism is an isomorphism by Corollary 2 of V, p. 387. The representation of G on H is therefore isomorphic to $\pi$, whence it follows that $u(x)$ belongs to $M_{\pi}(\varrho ')$.

For every vector space H and every family $(H_i)_{i\in I}$ of subspaces of H, one says that the spaces $(H_i)_{i\in I}$ are in direct sum if the family $(H_i)_{i\in I}$ satisfies the equivalent conditions of Prop. 11 of A, II, p. 18.

#### Proposition 9 {#ts-v-s1-prop-9 .statement tag=039S}

Let G be a topological group and let $\varrho$ be a unitary representation of G in a complex Hilbert space E. Let $\pi$ be an irreducible unitary representation of G in a complex Hilbert space $E_{\pi}$. Let us denote by $v$ the linear mapping of Hom$_G(\pi , \varrho )\otimes E_{\pi}$ into E such that $v(u\otimes x) =u(x)$ for every $(u, x)\in$ Hom$_G(\pi , \varrho )\times E_{\pi}$.

The linear mapping $v$ is injective, and its image is the sum of the spaces of all the subrepresentations of $\varrho$ which are isomorphic to $\pi$. In particular, the image of $v$ is dense in $M_{\pi}(\varrho )$.

Cor. 5 of V, p. 388 implies that the image of $v$ is the sum of the spaces of all the subrepresentations of $\varrho$ which are isomorphic to $\pi$.

Let us prove that $v$ is injective. Let $(u_i)_{i\in I}$ be a basis of the vector space Hom$_G(\pi , \varrho )$. For $i\in I$, let us denote by $F_i$ the image of $u_i$ and by $\widetilde{u}_i: E_{\pi}\rightarrow F_i$ the G-isomorphism deduced from $u_i$ by passing to the subspaces.

Let us first prove, by induction on the cardinal of a finite subset J of I, that the subspaces $(F_i)_{i\in J}$ are in direct sum.

The case where J is empty is immediate. Suppose that J is nonempty and that the required property holds for the subsets of I of cardinal at most Card(J) $-1$.

Let $j$ be a fixed element of J. The induction hypothesis implies that the subspaces $F_i$ for $i\in J-\{j\}$ are in direct sum. Let $F'$ be their sum; it remains now to prove that $F_j\cap F'=\{0\}$.

Suppose that the intersection of $F_j$ and $F'$ is not reduced to 0; this intersection is a subrepresentation of $F_j$, and since the latter is irreducible, we therefore have $F_j\cap F'= F_j$, whence $F_j\subset F'$.

For $i\in J-\{j\}$, denote by pr$_i: F'\rightarrow F_i$ the projection and by $\iota_i: F_i\rightarrow F'$ the inclusion. We have a canonical isomorphism

Hom$_G(F_j,F')\rightarrow \bigoplus_{i\in J-\{j\}}$ Hom$_G(F_j,F_i)$

(formula (1), p. 377) such that $u: F_j\rightarrow F'$ has as image the family (pr$_i\circ u$)$_{i\in J-\{j\}}$ (A, II, p. 13, cor. 1). Corollary 2 of V, p. 387 implies that $\widetilde{u}_i\circ \widetilde{u}^{-1}_j$, which is nonzero, is a basis of the space Hom$_G(F_j,F_i)$. Consequently, the family of G-morphisms $(\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j)_{i\in J-\{j\}}$ is a basis of Hom$_G(F_j,F')$.

Denote by $\iota$ the inclusion of $F_j$ in $F'$; it is an element of Hom$_G(F_j,F')$, hence it is a linear combination of the G-morphisms $\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j$ for $i\in J-\{j\}$. It follows that $u_j$ is a linear combination of the mappings $u_i$ for $i\not =j$, which contradicts the linear independence of the family $(u_i)_{i\in I}$. The assertion is therefore proved by induction.

Let us now prove that $v$ is injective. Let $w$ be an element of Hom$_G(\pi , \varrho )\otimes E_{\pi}$. There exists a unique family $(x_i)_{i\in I}$ in $E_{\pi}$ with finite support such that

$$
w=\sum_{i\in I}u_i\otimes x_i
$$

(A, II, p. 62, cor. 1) and we then have

$$
v(w) =\sum_{i\in I}u_i(x_i)
$$

From what precedes, the condition $v(w) = 0$ therefore implies that $u_i(x_i) = 0$ for every $i\in I$, whence $x_i= 0$ for every $i$ since $u_i$ is injective, and therefore $w= 0$.

#### Proposition 10 {#ts-v-s1-prop-10 .statement tag=039T}

Let G be a topological group. Let $\pi$ be an irreducible unitary representation of G in a complex Hilbert space $E_{\pi}$ and let $\varrho$ be a unitary representation of G in a complex Hilbert space E.

There exist families $(E_i)_{i\in I}$ of closed invariant subspaces of E such that the subrepresentation of $\varrho$ in $E_i$ is isomorphic to $\pi$ for every $i\in I$ and such that $M_{\pi}(\varrho )$ is the Hilbert sum of the spaces $E_i$. Moreover, the cardinal of I is independent of the family $(E_i)_{i\in I}$ satisfying these properties.

Let us prove the existence of families satisfying the indicated conditions. Let $\mathscr{O}$ be the set of subsets C of Hom$_G(\pi , \varrho )-\{0\}$ such that the subspaces $u(E_{\pi})$ for $u\in C$ are pairwise orthogonal. The set $\mathscr{O}$ is ordered by inclusion. It is nonempty since the empty set is one element, and it is of finite character (E, III, p. 34, Def. 2) since C belong to $\mathscr{O}$ if and only if the sets containing two elements of C belong to $\mathscr{O}$. By E, III, p. 35, Theorem 1, there exists a maximal element C of $\mathscr{O}$. Let F be the closure of the subspace generated by the spaces $u(E_{\pi})$ for $u\in C$; it is the Hilbert sum of the spaces $u(E_{\pi})$ for $u\in C$. We shall prove that $F = M_{\pi}(\varrho )$, which will prove that the family $(u(E_{\pi}))_{\pi\in C}$ has the required properties.

By definition, $u(E_{\pi})\subset M_{\pi}(\varrho )$ for every $u\in C$, hence F is contained in $M_{\pi}(\varrho )$. To prove the converse inclusion, it is enough to prove that if $v$ is a G-morphism of $\pi$ into $\varrho$, then its image is contained in F. Let $p$ be the orthogonal projector of E with image $F^{\circ}$; it is a G-morphism, since F is a subrepresentation of E (Proposition 4 of V, p. 383). The image of the G-morphism $p\circ v$ is orthogonal to F; it is therefore zero (otherwise $C\cup  \{p\circ v\} \in \mathscr{O}$, which contradicts the maximality of C), and consequently the image of $v$ is contained in F.

Let now $(E_i)_{i\in I}$ and $(F_j)_{j\in J})$ be families of closed invariant subspaces of E, pairwise orthogonal, such that the subrepresentation of G in $E_i$ (resp. in $F_j$) is isomorphic to $\pi$ for every $i\in I$ (resp. for every $j\in J$), and such that $M_{\pi}(\varrho )$ is the Hilbert sum of the family $(E_i)_{i\in I}$ and of the family $(F_j)_{j\in J}$.

If I is finite, then

dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ dim Hom$_G(E_{\pi},\bigoplus_{i\in I}E_i)=$ Card(I)

(formula (1) of V, p. 377 and Corollary 2 of V, p. 387). For every finite subset L of J, one then has

Card(L) = dim Hom$_G(E_{\pi},\bigoplus_{i\in L}F_j)$

$\leqslant$ dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ Card(I)

(loc. cit.). This proves that J is then finite and that Card(I) = Card(J), as desired. Analogously, if J is finite, then I is finite and has the same cardinal.

Suppose now that I and J are infinite. For $j\in J$, let $p_j$ denote the orthogonal projector of E with image $F_j$. For $i\in I$, let $x_i$ be a nonzero element of $E_i$; it is a cyclic vector of $E_i$. Observe that since $p_j$ induces by passing to the subspaces a G-morphism of $E_i$ into $F_j$, the space $p_j(E_i)$ is zero if and only if $p_j(x_i) = 0$ (in fact, the space $E_i\cap$Ker($p_j$) is either zero, or equal to $E_i$).

For every $j\in J$, there exists an element $f(j)\in I$ such that $p_j(E_{f(j)})$ is not reduced to 0 (otherwise, the orthogonal projector $p_j$ would be zero on $M_{\pi}(\varrho )$). Thus a mapping $f$ of J into I has been defined. For

$-1$

every $i\in I$, the set $f(i)$ is countable. In fact, this set is contained in the set of $j\in J$ such that $p_j(E_i)$ is nonzero, that is, such that $p_j(x_i)\not = 0$. Now (EVT, V, p. 20, cor. 2), one has

$$
\sum_{j\in J}\|p_j(x_i)\|^2=\|x_i\|^2
$$

therefore the set of $j\in J$ such that $p_j(x_i)\not = 0$ is countable. By E, III, p. 50, prop. 4, it follows that Card(J) = Card($f(J)$)$\leqslant$ Card(I). By interchanging the roles of I and J, one concludes that Card(I) = Card(J).

#### Corollary {#ts-v-s1-n11-cor-1 .statement tag=039U}

Let G be a topological group and $\varrho$ a unitary representation of G in a complex Hilbert space E. The Hilbert sum of the $\pi$-isotypical components of G for $\pi \in \widehat{G}$ is the greatest semisimple subrepresentation of $\varrho$.

In fact, the $\pi$-isotypical components of G for $\pi \in \widehat{G}$ are pairwise orthogonal (prop. 8, a)), and each is semisimple (prop. 10, a)); hence the Hilbert sum F of the spaces $M_{\pi}(\varrho )$ for $\pi \in \widehat{G}$ defines a semisimple subrepresentation of $\varrho$. Since moreover every irreducible subrepresentation of $\varrho$ is a subrepresentation of an isotypical component of $\varrho$, the corollary follows.

#### Definition 10 {#ts-v-s1-def-10 .statement tag=039V}

Let G be a topological group. Let $\varrho$ be a unitary representation of G in a complex Hilbert space E and $\pi$ an irreducible unitary representation of G in a complex Hilbert space.

The **multiplicity** of $\pi$ in $\varrho$ is defined to be the cardinal of the set I for any family $(E_i)_{i\in I}$ of closed subspaces of E stable under G such that the subrepresentation of $\varrho$ induced in $E_i$ is isomorphic to $\pi$ for every I and such that $M_{\pi}(\varrho )$ is the Hilbert sum of the subspaces $E_i$.

If the multiplicity of $\pi$ in $\varrho$ is finite, then it is equal to the dimension of the space Hom$_G(\pi , \varrho )$ (resp. to the dimension of Hom$_G(\varrho , \pi )$) by formula (1) of V, p. 377 and corollary 2 of V, p. 387. This is not always the case in general.

#### Remark {#ts-v-s1-n11-rem-1 .statement tag=039W}

It is possible for a unitary representation $\varrho$ to be nonzero, but for all the isotypical components of $\varrho$ relative to all the irreducible representations of G to be zero (cf. V, p. 426, remark).

## EXERCISES {#ts-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
