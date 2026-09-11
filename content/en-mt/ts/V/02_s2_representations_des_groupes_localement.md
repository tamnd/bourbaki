---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 2
section_title: Représentations des groupes localement compacts
lang: en
source: ts-iii-v-fr
book_pages: TS V.399-TS V.431, TS V.486-TS V.492
pdf_pages: 0412-0444, 0499-0505
extraction: native
subsections:
    - "no": 1
      title: Continuité de certaines représentations
      page: 399
      pdf_page: 412
    - "no": 2
      title: Extension de représentations à des espaces de mesures
      page: 400
      pdf_page: 413
    - "no": 3
      title: Critère de semi-simplicité
      page: 402
      pdf_page: 415
    - "no": 4
      title: Représentations régulières
      page: 405
      pdf_page: 418
    - "no": 5
      title: Fonctions équivariantes
      page: 407
      pdf_page: 420
    - "no": 6
      title: Représentations induites
      page: 415
      pdf_page: 428
    - "no": 7
      title: Cas d’un sous-groupe fermé central
      page: 416
      pdf_page: 429
    - "no": 8
      title: Représentations de carré intégrable
      page: 419
      pdf_page: 432
    - "no": 9
      title: Sous-représentations de la représentation régulière d’un groupe commutatif
      page: 425
      pdf_page: 438
    - "no": 10
      title: Représentations unitaires du groupe R
      page: 427
      pdf_page: 440
statements: 45
exercises: 20
content_sha256: c28075aaca88e73a217d743e0f90dd1d3d6c62e0ddbc8b6f5c6252e65c430bf4
translated_from: content/fr/ts/V/02_s2_representations_des_groupes_localement.md
source_lang: fr
translation_method: machine
source_content_sha256: f35f594201c7156dde4597f94f43df4226aa2d4af3cf832fbc825c8eb90246ae
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-6443289f
glossary_version: 34
glossary_terms_sha256: ace3286462839540aa6ef83cd4fd62483d4bdb4e29bd4455e42c2b6b1fc6cfd0
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. REPRESENTATIONS OF LOCALLY COMPACT GROUPS

In this paragraph, the vector spaces are over the field $K =\mathbf{R}$ or $\mathbf{C}$. We denote by G a locally compact group endowed with a left Haar measure $\mu$. We shall write $\mathscr{L}^p(G) =\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ and $L^p(G) = L^p_{\mathbf{C}}(G, \mu)$ for every $p\in [1,+\infty ]$.

### 1. Continuity of certain representations

#### Proposition 1 {#ts-v-s2-prop-1 .statement tag=03A4}

Let H be a locally compact group. Let $\varrho_1$ (resp. $\varrho_2$) be a continuous representation of G (resp. of H) in a separated locally convex K-vector space $E_1$ (resp. $E_2$). Let F denote the space $\mathscr{L}(E_1; E_2)$ endowed with the topology of compact convergence. The representation $\varrho$ of $G\times H$ in F defined by $\varrho (g, h)u=\varrho_2(h)\circ u\circ \varrho_1(g^{-1})$ for $(g, h)\in G\times H$ is continuous.

Let $\mathscr{L}_c(E_1; E_2)$ denote the space $\mathscr{L}(E_1; E_2)$ endowed with the topology of compact convergence. Let $\mathfrak{F}_1$ (resp. $\mathfrak{F}_2,\mathfrak{F}_3$) be a filter in G converging to $e$ (resp. a filter in $\mathscr{L}_c(E_1; E_2)$ converging to 0, a filter in H converging to $e$). Since G and H are locally compact, there exist elements $C\in \mathfrak{F}_1$ and $D\in \mathfrak{F}_3$ which are relatively compact. The set $\varrho_1(C^{-1})$ is equicontinuous in $\mathscr{L}(E_1) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2, a$'))$. By prop. 9 of EVT, III, p. 33 and prop. 4 of EVT, III, p. 31, the mapping defined by $(u, v)\mapsto u\circ v$ of $\mathscr{L}_c(E_1; E_2)\times \varrho_1(C^{-1})$ into $\mathscr{L}_c(E_1; E_2)$ is continuous. The filter base $\mathfrak{F}_2\circ \varrho_1(\mathfrak{F}^{-1}_1)$ therefore converges to 0 in $\mathscr{L}_c(E_1; E_2)$. The set $\varrho_2(D)$ is equicontinuous in $\mathscr{L}(E_2) ($cf. INT, VIII, p. 129, § 2, n$^o1$, rem. 2), and for every $x\in E_2$, the set $\varrho_2(D)x\subset E_2$ is relatively compact. Consequently, $\varrho_2(D)$ is relatively compact in $\mathscr{L}(E_2)$ endowed with the topology of compact convergence (TG, X, p. 18, cor. 1). The mapping defined by $(u, v)\mapsto u\circ v$ of $\overline{\varrho_2(D)}\times \mathscr{L}_c(E_1; E_2)$ into $\mathscr{L}_c(E_1; E_2)$ is continuous by prop. 9 of EVT, III, p. 33 and prop. 4 of EVT, III, p. 31. Hence the filter base $\varrho (\mathfrak{F}_1\times \mathfrak{F}_3)(\mathfrak{F}_2)$ converges to 0 in $\mathscr{L}_c(E_1; E_2)$. This implies the assertion.

#### Corollary {#ts-v-s2-n1-cor-1 .statement tag=03A5}

Let $\varrho$ be a continuous representation of G in a separated locally convex K-vector space E. The contragredient representation $\breve{\varrho}$ is continuous when $E'$ is endowed with the topology of compact convergence.

This results from the proposition by taking $H =\{e\},\varrho_1=\varrho$ and $\varrho_2$ the trivial representation on K.

#### Remark {#ts-v-s2-n1-rem-1 .statement tag=03A6}

The contragredient representation is not necessarily continuous when $E'$ is endowed with the strong topology (cf. INT, VIII, p. 191, § 2, exercise 3, d)). One can show that it is so if the space E is semi-reflexive (loc. cit., c)).

### 2. Extension of representations to spaces of measures

In this number, it is assumed that $K =\mathbf{C}$.

Let $\varrho$ be a continuous linear representation of G in a separated quasi-complete locally convex space E. Let $\mathscr{M}_c(G)$ denote the space of measures with compact support on G endowed with the topology of compact convergence; this is the dual of the space $\mathscr{C}(G)$. For every measure $\nu \in \mathscr{M}_c$(G), put

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

This is an element of $\mathscr{L}(E)$. In particular, one has $\varrho (\varepsilon_g) =\varrho (g)$ for every $g\in G$.

According to INT, VIII, p. 136, § 2, n$^o6$, the mapping $\nu \mapsto \varrho (\nu )$ is a continuous linear mapping from $\mathscr{M}_c(G)$ into the space $\mathscr{L}(E)$ endowed with the topology of compact convergence. According to INT, VIII, p. 145, § 3, n$^o3$, prop. 11, it is a morphism of unital algebras.

Let $x\in E$. The mapping from $\mathscr{M}_c(G)$ into E defined by $\nu \mapsto \varrho (\nu )x$ is continuous when $\mathscr{M}_c(G)$ is endowed with the topology of compact convergence (INT, VI, p. 27, § 1, n$^o$ 7, prop. 16 and EVT, III, p. 31, prop. 4).

For $f\in \mathscr{L}^1(G)$ null outside a compact subset of G, the measure $f\cdot \mu$ has compact support and we shall denote by $\varrho^\mu(f)$, or by $\varrho (f)$ when no ambiguity is possible, the endomorphism $\varrho (f\cdot \mu)$ of E. This endomorphism depends only on the class $\widetilde{f}$ of $f$ in $L^1$(G), and it will also be denoted by $\varrho^\mu(\widetilde{f})$ or $\varrho (\widetilde{f})$.

Analogously, let $\varrho$ be a continuous and bounded linear representation of G in a Banach space E. For every bounded measure $\nu \in \mathscr{M}^1$(G), put

$$
\varrho (\nu ) =\int_G\varrho (g)d\nu (g)
$$

According to INT, VIII, loc. cit., the mapping $\nu \mapsto \varrho (\nu )$ is a continuous unital morphism of Banach algebras from the algebra $\mathscr{M}^1(G)$ of bounded complex measures on G into the Banach algebra $\mathscr{L}(E)$.

Let $\rho$ be the function $g\mapsto  \|\varrho (g)\|$ on G; the algebra denoted $\mathscr{M}^{\rho}$ in INT, VIII, p. 145, prop. 11 (whose elements are the measures $\nu$ such that $\rho \in \mathscr{L}^1(\nu )$) coincides with the Banach algebra $\mathscr{M}^1(G)$. Indeed, put M = sup $\rho$. We have $M>0$ since $\rho (e) = 1$, and $M^{-1}\leqslant \rho \leqslant M$ since $\|\varrho (e)\|\leqslant \|\varrho (g)\| \|\varrho (g^{-1})\|$ for every $g\in G$; thus $\rho \in \mathscr{L}^1(\nu )$ if and only if $\nu$ is a bounded measure.

If $f\in \mathscr{L}^1$(G), we shall also denote by $\varrho^\mu(f)$ or simply $\varrho (f)$ the endomorphism $\varrho (f\cdot \mu)$, and analogously for the class $\widetilde{f}$ of $f$ in $L^1(G)$.

#### Lemma 1 {#ts-v-s2-lem-1 .statement tag=03A7}

Let $\varrho$ be a unitary representation of G in a Hilbert space E. The mapping $\nu \mapsto \varrho (\nu )$ from $\mathscr{M}^1(G)$ into $\mathscr{L}(E)$ is a unital morphism of involutive Banach algebras.

From what precedes, it suffices to prove that the morphism $\nu \mapsto \varrho (\nu )$ is involutive. Let $\nu \in \mathscr{M}^1(G)$. The measure $\nu^*$ is the conjugate measure of the measure $\check{\nu}($I, p. 99, example 4). According to the definition of the conjugate measure (INT, III, p. 52, § 1, n$^o5$), one calculates

$$
\langle x|\varrho (\nu )y\rangle =\int\langle x|\varrho (g)y\rangle d\nu (g)
$$

$$
=\int^G_G\langle \varrho (g^{-1})x|y\rangle d\nu (g) =\int_G\langle \varrho (g)x|y\rangle d\check{\nu}(g)
$$

$$
=\int_G\langle y|\varrho (g)x\rangle d\nu^*(g) =\langle \varrho (\nu^*)x|y\rangle
$$

for all $x$ and $y$ in E, whence $\varrho (\nu )^*=\varrho (\nu^*)$.

Let $\varrho$ be a continuous linear representation (resp. continuous and bounded) of G in a quasi-complete locally convex space E (resp. a Banach space E). If F is a closed subspace of E defining a subrepresentation $\varrho_F$ of $\varrho$, then for every measure $\nu \in \mathscr{M}_c(G)$ (resp. $\nu \in \mathscr{M}^1(G)$) the linear mapping $\varrho (\nu )$ leaves the subspace F stable and coincides with $\varrho_F(\nu )$ on F.

Conversely, let $F\subset E$ be a closed subspace, stable under the linear mappings $\varrho (f)$ for every function $f\in \mathscr{K}(G)$. Then F defines a subrepresentation of $\varrho$ (INT, VIII, p. 139, § 2, n$^o7$, prop. 10).

Recall (A, VIII, p. 388) that a function $f: G\rightarrow \mathbf{C}$ is said to be central if, for all $g$ and $h$ in G, one has $f(gh) =f(hg)$. This amounts to saying that $f$ is invariant under conjugation.

#### Definition 1 {#ts-v-s2-def-1 .statement tag=03A8}

A bounded measure $\nu \in \mathscr{M}^1(G)$ is said to be central if one has $\varepsilon_g*\nu =\nu *\varepsilon_g$ for every $g\in G$.

If G is unimodular and $f\in \mathscr{C}(G)$ is $\mu$-integrable, the measure $f\cdot \mu$ is central if and only if $f$ is central.

Let $\varrho$ be a bounded continuous representation of G in a Banach space E (resp. a continuous representation of G in a separated quasi-complete locally convex space E). For every bounded central measure $\nu$ on G (resp. every central measure with compact support $\nu$ on G), the linear mapping $\varrho (\nu )$ is a G-morphism from $\varrho$ into $\varrho$. In fact, for every $g\in G$, one has

$$
\varrho (\nu )\varrho (g) =\varrho (\nu *\varepsilon_g) =\varrho (\varepsilon_g*\nu ) =\varrho (g)\varrho (\nu )
$$

### 3. Criterion for Semisimplicity

#### Proposition 2 {#ts-v-s2-prop-2 .statement tag=03A9}

Let $\varrho$ be a unitary representation of G in a complex Hilbert space E. Let $\mathfrak{F}$ be a basis of filter on $\mathscr{M}_c(G)$ converging to the measure $\varepsilon_e$ for the topology of compact convergence. Suppose that there exists $M\in \mathfrak{F}$ such that $\varrho (\nu )$ is a compact endomorphism of E for every $\nu \in M$.

Then the unitary representation $\varrho$ is semisimple and every irreducible unitary representation of G has finite multiplicity in $\varrho$.

Let us first prove a lemma.

#### Lemma 2 {#ts-v-s2-lem-2 .statement tag=03AA}

Let $\varrho_1$ be a nonzero unitary representation of G isomorphic to a subrepresentation of $\varrho$. There exists a measure $\nu \in M$ such that $\varrho_1(\check{\nu}*\nu )$ is a nonzero hermitian compact endomorphism of the space of $\varrho_1$. In particular, there exists a nonzero real number $\lambda$ such that the eigensubspace of $\varrho_1(\check{\nu}*\nu )$ corresponding to $\lambda$ is nonzero.

One may suppose that $\varrho_1$ is a subrepresentation of $\varrho$. Let $E_1$ be its space. For every measure $\nu \in M$, the endomorphism $\varrho_1(\nu )$ is deduced from $\varrho (\nu )$ by passing to subspaces. The hypothesis and prop. 3 of III, p. 5 therefore imply that $\varrho_1(\nu )$ is compact.

Since $\mathfrak{F}$ converges to the measure $\varepsilon_e$ in $\mathscr{M}_c(G)$ endowed with the topology of compact convergence and since the space $E_1$ is nonzero, there exists $\nu \in M$ such that $v=\varrho_1(\nu )$ is a nonzero endomorphism of $E_1$ (cf. No.$^o2$ of V, p. 400). The endomorphism $u=\varrho_1(\check{\nu}*\nu )$ is equal to $v^*\circ v$ (lemma 1 of V, p. 401); it is therefore nonzero (EVT, V, p. 39, prop. 2), hermitian and compact, since $v$ is compact.

Since $u$ is hermitian and nonzero, its spectrum is not reduced to zero (example 1 of I, p. 110). Finally, since $u$ is compact, every $\lambda \in$ Sp($u$)$-\{0\}$ is an eigenvalue of $u$ (prop. 2 of III, p. 83).

Let us now prove the proposition.

We shall use prop. 7 of V, p. 391 to establish that $\varrho$ is semisimple. Let $\varrho_1$ be a nonzero subrepresentation of $\varrho$, and $E_1\subset E$ its space; we must prove that $\varrho_1$ contains an irreducible subrepresentation.

Let $\nu \in M$ be such that $u=\varrho_1(\check{\nu}*\nu )$ is a nonzero compact hermitian endomorphism of the space of $\varrho_1$, and let $\lambda$ be nonzero such that the eigensubspace F of $u$ relative to $\lambda$ is nonzero (lemma 2). The space F is of finite dimension (prop. 5 of III, p. 90). There exists a subrepresentation $\varrho_2$ of $\varrho_1$ on a subspace $E_2$ of $E_1$ such that $E_2\cap F$ is nonzero and of minimal dimension. Let $x$ be a nonzero element of $E_2\cap F$, and let $E_3$ be the subrepresentation of $\varrho_1$ generated by $x$. Then $E_3\subset E_2$, whence $E_3\cap F = E_2\cap F$ by minimality of the dimension of $E_2\cap F$.

Let us prove that the representation $E_3$ is irreducible. Let $E_4\subset E_3$ be a closed subspace stable under G. We have $E_2\cap F = (E_4\cap F)\oplus (E^{\circ}_4\cap F)$, where $E^{\circ}_4$ denotes the orthogonal of $E_4$ in $E_3$ (in fact, if $y\in E_2\cap F$, let $y_4\in E_4$ be its orthogonal projection on $E_4$; since $E_4$ and $E^{\circ}_4$ are stable under $u$, the vector $u(y_4)$ is the orthogonal projection of $u(y) =\lambda y$ on $E_4$, whence $u(y_4) =\lambda y_4$, which means that $y_4\in E_4\cap F$, and the assertion follows). The minimality of the dimension of $E_2\cap F$ then implies that either $E_4\cap F = E_2\cap F$, or $E^{\circ}_4\cap F = E_2\cap F$. In the first case, we have $x\in E_4$, whence $E_4= E_3$, and in the second, we have $x\in E^{\circ}_4$, whence $E^{\circ}_4= E_3$ and $E_4=\{0\}$. The representation $E_3$ is therefore irreducible.

It follows from Prop. 7 of V, p. 391 that the representation $\varrho$ is semisimple.

Let $\pi$ be an irreducible unitary representation of G whose multiplicity in $\varrho$ is nonzero; let $E_{\pi}$ be its space. There exist a measure $\nu \in M$ and a nonzero real number $\lambda$ such that $u=\pi (\check{\nu}*\nu )$ is a nonzero compact hermitian endomorphism of $E_{\pi}$ and that the proper subspace of $u$ corresponding to $\lambda$ is nonzero (Lemma 2). Let F be the proper subspace of $v=\varrho (\check{\nu}*\nu )$ corresponding to $\lambda$. For every subrepresentation $E_1$ of E isomorphic to $\pi$, the endomorphism of $E_1$ deduced from $v$ by passing to the subspaces is identified with $u$, hence the intersection of $E_1$ and F is nonzero. Thus, the multiplicity of $\pi$ in $\varrho$ is less than the dimension of the space F, which is finite (Prop. 5 of III, p. 90).

#### Example {#ts-v-s2-n3-exa-1 .statement tag=03AB}

Suppose that G is unimodular, for example that G is a real semisimple Lie group. Let $\Gamma \subset G$ be a discrete subgroup such that the quotient $X = \Gamma \backslash G$ is compact. The group G acts on the right by multiplication on X. Let $\beta$ denote the counting measure on Γ and put $\widetilde{\mu}=\mu/\beta$ (INT, VII, p. 44, § 2, No.$^o2$, Def. 1); it is a bounded G-invariant measure on X.

For every $f\in \mathscr{L}^2(X,\widetilde{\mu})$ and every $g\in$ G, one defines the function $\varrho (g)f\in \mathscr{L}^2(X,\widetilde{\mu})$ by $\varrho (g)f(x) =f(x\cdot g)$. The mapping $\varrho (g)$ is a continuous linear mapping, which induces by passing to quotients a unitary mapping on $L^2(X,\widetilde{\mu})$, again denoted by $\varrho (g)$. The mapping $\varrho$ is a unitary representation of G in $L^2(X,\widetilde{\mu})$ (INT, VII, p. 135, § 2, No.$^o5$, Prop. 8).

Let $\varphi \in \mathscr{K}(G)$. For all compact subsets $L_1$ and $L_2$ of G, the intersection T of Γ and the compact set $L_1$Supp($\varphi$ )$L^{-1}_2$ is finite. For every $(g, h)\in L_1\times L_2$, the series $\sum_{\gamma\in\Gamma}\varphi (g^{-1}\gamma h)$ coincides with the sum

finite $\sum_{\gamma\in T}\varphi (g^{-1}\gamma h)$. Since G is locally compact, the sum of

this series, denoted by $k_{\varphi}(g, h)$, is a continuous function on $G\times G$.

Let $g\in G$ and let $(\gamma , \eta )\in \Gamma \times \Gamma$. One has $k_{\varphi}(\gamma g, \eta h) =k_{\varphi}(g, h)$, hence $k_{\varphi}$ defines by passing to the quotient a continuous function on $X\times X$, which is denoted by $\widetilde{k}_{\varphi}$. One has moreover $\widetilde{k}_{\varphi}\in \mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, since the space X is assumed compact.

One denotes by $\dot{x}$ the image in X of an element $x$ of G under the canonical projection. Let $\varphi \in \mathscr{K}(G)$. For $f\in \mathscr{L}^2(X,\widetilde{\mu})$ and $x\in G$, one has

$$
\varrho (\varphi )f( \dot{x}) =\int_G\varphi (g) (\varrho (g)f)( \dot{x})d\mu(g) =\int_G\varphi (g)f( \dot{x}\cdot g)d\mu(g)
$$

$$
=\int_G\varphi (x^{-1}y)f( \dot{y})d\mu(y) =\int_{\Gamma\backslash G}((\sum_{\gamma\in\Gamma}\varphi (x^{-1}\gamma y))f( \dot{y})d\widetilde{\mu}( \dot{y})
$$

(INT, VII, p. 46, § 2, No.$^o3$, Prop. 5). Since $\widetilde{k}_{\varphi}$ belongs to the space $\mathscr{L}^2(X\times X,\widetilde{\mu}\otimes \widetilde{\mu})$, it follows that the endomorphism $\varrho (\varphi )$ of $L^2(X,\widetilde{\mu})$ coincides with the Hilbert-Schmidt endomorphism of kernel $\widetilde{k}_{\varphi}$; this endomorphism is therefore compact (Cor. 1 of III, p. 33)

There exists a sequence $(\varphi_n)_{n\in\mathbf{N}}$ of functions in $\mathscr{K}_+(G)$ of integral 1 such that $\varphi_n\cdot \mu$ converges to $\varepsilon_e$ in $\mathscr{M}_c(G)$ endowed with the topology of compact convergence (INT, VIII, p. 139, § 2, No.$^o7$, Cor. 2). Prop. 2 therefore implies that the representation $\varrho$ is semisimple and that the multiplicities of the irreducible unitary representations of G in $\varrho$ are finite.

The irreducible unitary representations of G whose multiplicity in $\varrho$ is not zero are called Γ-automorphic representations of the group G.

### 4. Regular Representations

Let $p$ be a real number $\geqslant 1$ and $\mu'$ a right Haar measure on G.

For every $g\in G$ and every function $f\in \mathscr{L}^p(G, \mu)$, we denote by $\boldsymbol{\gamma }^{(p)}_G(g)f$ the function $x\mapsto f(g^{-1}x)$ on G. The mapping $g\mapsto \boldsymbol{\gamma }^{(p)}_G(g)$ is a continuous linear representation of G in $\mathscr{L}^p(G)$. By passing to quotients, it induces a continuous isometric linear representation of G in $L^p(G)$ (INT, VIII, p. 135, § 2, n$^o5$, Prop. 8), denoted by $\boldsymbol{\gamma }^{(p)}_G$.

Analogously, for every $g\in G$ and every function $f\in \mathscr{L}^p(G, \mu')$, we denote by $\boldsymbol{\delta }^{(p)}_G(g)f$ the function $x\mapsto f(xg)$ on G. The mapping $g\mapsto \boldsymbol{\delta }^{(p)}_G(g)$ is a continuous linear representation of G in $\mathscr{L}^p(G, \mu')$. By passing to quotients, it induces a continuous isometric linear representation of G in $L^p(G, \mu') ($cf. INT, VIII, p. 136, § 2, n$^o5)$.

We say that $\boldsymbol{\gamma }_G^{(p)}$ is the left regular representation of G in $\mathscr{L}^p(G)$ or $L^p(G)$ and that $\boldsymbol{\delta }^{(p)}_G$ is the right regular representation of G in $\mathscr{L}^p(G, \mu')$ or $L^p(G, \mu')$.

#### Lemma 3 {#ts-v-s2-lem-3 .statement tag=03AC}

Let $p$ be a real number $\geqslant 1$. The left (resp. right) regular representation of G in $L^p(G, \mu) ($resp. in $L^p(G, \mu'))$ is faithful.

More precisely, let $q$ be the conjugate exponent of $p$ and let $g$ be an element of G such that $g\not =e$.

a) There exists a function $\varphi \in \mathscr{K}(G)$, positive and nonzero in $L^q(G, \mu)$, such that $\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle = 0$;

b) There exists a function $\varphi \in \mathscr{K}(G)$, positive and nonzero in $L^q(G, \mu')$, such that $\langle \varphi ,\boldsymbol{\delta }^{(p)}_G(g)\varphi \rangle = 0$.

Let us consider the case of the left regular representation $\boldsymbol{\gamma }^{(p)}_G$, that of the right regular representation being similar. Assertion a) implies that $\boldsymbol{\gamma }^{(p)}_G$ is faithful, for if $g\not =e$ is an element of G, and if $\varphi$ is as in a), one has $\varphi \not =\boldsymbol{\gamma }^{(p)}_G(g)\varphi$ since $\langle \varphi , \varphi \rangle =\int_G\varphi^2>0$.

Let us therefore prove a). Let $g\not =e$ in G. Let C be a symmetric compact neighbourhood of $e$ such that $g \notin C^2$ and let $\varphi \in \mathscr{K}(G)$ be a positive continuous function of integral 1 with support contained in C; the function $\varphi$ is nonzero in $L^p(G, \mu)$. Since $C\cap g^{-1}C =\emptyset$, one has

$$
\langle \varphi ,\boldsymbol{\gamma }^{(p)}_G(g)\varphi \rangle =\int_G\varphi (x)\varphi (g^{-1}x)d\mu(x) = 0
$$

Let $\varrho$ be a continuous bounded representation of G in a Banach space E. For every $f\in L^1(G)$ (resp. $f'\in L^1(G, \mu')$) and every $g\in G$, one has

(1) $\varrho (g)\varrho (f\cdot \mu) =\varrho (\varepsilon_g*(f\cdot \mu)) =\varrho (\boldsymbol{\gamma }^{(1)}_G(g)f\cdot \mu)$,

(2) $\varrho (f'\cdot \mu')\varrho (g) =\varrho ((f'\cdot \mu')*\varepsilon_g) =\varrho (\boldsymbol{\delta }^{(1)}_G(g^{-1})f'\cdot \mu')$

(INT, VIII, p. 144, § 3, n$^o2$, formula (5)).

Suppose G unimodular, and put $\mu'=\mu$. The biregular representation of G in $\mathscr{L}^p(G)$ (resp. in $L^p(G)$) is the representation $\boldsymbol{\varrho }^{(p)}_G$ of $G\times G$ in $\mathscr{L}^p(G)$ (resp. in $L^p(G)$) such that

$$
\boldsymbol{\varrho }_G^{(p)}(g_1, g_2) =\boldsymbol{\gamma }_G^{(p)}(g_1)\boldsymbol{\delta }_G^{(p)}(g_2) =\boldsymbol{\delta }_G^{(p)}(g_2)\boldsymbol{\gamma }_G^{(p)}(g_1)
$$

It is a continuous linear representation (Lemma 1 of V, p. 377). It satisfies

$$
(\boldsymbol{\varrho }_G^{(p)}(g_1, g_2)f)(x) =f(g_1^{-1}xg_2)
$$

for every $f\in \mathscr{L}^p$(G), every $(g_1, g_2)\in G\times G$ and every $x\in G$.

#### Remark {#ts-v-s2-n4-rem-1 .statement tag=03AD}

The biregular representation of G in $L^p(G, \mu)$ is not necessarily faithful; its kernel is the image of the center of G under the mapping $g\mapsto (g, g)$ (exercise 4 of V, p. 487).

When $p= 2$, the left regular representation $\boldsymbol{\gamma }^{(2)}_G$ of G in the complex Hilbert space $L^2(G, \mu)$ is unitary, since it is isometric. Analogously, the right regular representation $\boldsymbol{\delta }^{(2)}_G$ in $L^2(G, \mu')$ is unitary.

We shall write simply $\boldsymbol{\gamma }_G=\boldsymbol{\gamma }^{(2)}_G$ and $\boldsymbol{\delta }_G=\boldsymbol{\delta }^{(2)}_G$, and we shall call these representations the left and right regular representations of G.

If G is unimodular, the biregular representation $\boldsymbol{\varrho }^{(2)}_G$ of $G\times G$ in $L^2(G, \mu)$ is unitary. We shall write it simply $\boldsymbol{\varrho }_G$.

#### Lemma 4 {#ts-v-s2-lem-4 .statement tag=03AE}

Let $p$ be a real number $\geqslant 1$. For $f\in \mathscr{L}^1(G)$, the linear mapping $\boldsymbol{\gamma }^{(p)}_G(f)$ coincides with the endomorphism of $L^p(G)$ defined by $\varphi \mapsto f*^\mu\varphi$.

This follows from INT, VIII, p. 157, § 4, No.$^o2$, Prop. 6, taking account of formula (14) of INT, VIII, p. 165.

#### Remark {#ts-v-s2-n4-rem-2 .statement tag=03AF}

Recall that, for every function $f$ on G, one defines the function $\check{f}$ on G by $\check{f}(g) =f(g^{-1})$ for every $g\in G$ (INT, VII, p. 12, § 1, No.$^o1$, formula (12)).

One verifies that if $f\in \mathscr{L}^1$(G), the linear mapping $u=\boldsymbol{\delta }^{(p)}_G(f)$ satisfies the relation

$$
u(\widecheck{\varphi}) =f*\check{\varphi}
$$

for every $\varphi \in L^p(G, \mu')$.

### 5. Equivariant functions

In this number, a closed subgroup H of G is fixed. One denotes by $\varpi$ the canonical projection of G onto $G/H$.

In addition to the Haar measure $\mu$ on G, a left Haar measure $\beta$ on H is fixed.

According to INT, VII, p. 56, § 2, n$^o5$, th. 2, there exists a continuous function $\kappa : G\rightarrow \mathbf{R}_+^*$ such that $\kappa (xh) = \Delta_H(h)\Delta_G(h)^{-1}\kappa (x)$ for every $(x, h)\in G\times H$. We fix such a function $\kappa$. We denote by $\nu$ the measure $(\kappa \cdot \mu)/\beta$ on $G/H$; according to loc. cit., this is a non-zero positive measure quasi-invariant by G. Its support is equal to $G/H$ (INT, VII, p. 10, § 1, n$^o1$). According to INT, VII, p. 43, § 2, n$^o2$, prop. 4, the measure $\nu$ is the unique measure on $G/H$ such that the measure $\nu^{\sharp}$ on G is equal to $\kappa \cdot \mu$. We endow the space $G/H$ with the measure $\nu$ (so that we write, for example, $\mathscr{L}^p(G/H) =\mathscr{L}^p(G/H, \nu )$).

We shall say that a set $S\subset G$ is negligible modulo H if $\varpi (S)$ is $\nu$-negligible. This condition does not depend on the choice of the Haar measures on G and on H. It implies that S is locally $\mu$-negligible (INT, VII, p. 47, § 2, n$^o3$, prop. 6, a)). We shall say that a property of an element of G is true almost everywhere modulo H if the set of elements of G for which this property does not hold is negligible modulo H.

Let $\pi$ be a unitary representation of H in a Hilbert space E. We denote by $\mathscr{F}_{\pi}(G)$ the vector space of functions $f$ on G with values in E such that $f(xh) =\pi (h)f(x)$ for all $(x, h)\in G\times H$. The elements of $\mathscr{F}_{\pi}(G)$ are said to be the $\pi$-equivariant functions on G.

The space $\mathscr{F}_1(G)$ associated with the trivial representation of G on $\mathbf{C}$ is identified with the space $\mathscr{F}(G/H)$ of complex-valued functions on $G/H$ by the mapping $f\mapsto f\circ \varpi$ of $\mathscr{F}(G/H)$ into $\mathscr{F}_1(G)$.

For every function $f$ in $\mathscr{F}_{\pi}$(G), the function $\|f\|$ belongs to $\mathscr{F}_1(G)$ since $\pi$ is unitary. This makes it possible to identify $\|f\|$ with a function on $G/H$, and we shall write for example $\|f(xH)\|$ for the value of this function at an element $xH$ of $G/H$.

A function $f$ of $\mathscr{F}_{\pi}(G)$ will be said to be zero outside a compact set modulo H if $\|f\|$ is zero outside a compact subset of $G/H$. It amounts to the same to say that there exists a compact subset K of G such that $f$ is zero outside $K\cdot H$ (TG, III, p. 33, prop. 10).

We denote by $\mathscr{K}_{\pi}(G)$ the space of continuous functions on G belonging to $\mathscr{F}_{\pi}(G)$ which have compact support modulo H.

A space analogous to $\mathscr{K}_{\pi}(G)$ was defined in INT, VII, p. 39, §2, n$^o1$, when $\pi$ is a continuous homomorphism of H into $\mathbf{R}^*_+$.

Let $p\in [1,+\infty [$. For every $f\in \mathscr{F}_{\pi}$(G), one sets

$$
N_p(f) =(\int_{G/H}^*\|f\|^pd\nu )^{1/p}
$$

This is a real number or $+\infty$. One denotes by $\mathscr{F}_{\pi}^p(G, \nu )$, or simply $\mathscr{F}_{\pi}^p$(G), the subspace of the functions $f\in \mathscr{F}_{\pi}(G)$ such that $N_p(f)$ is finite. The space $\mathscr{F}_{\pi}^p(G)$ endowed with the mapping $N_p$ is a semi-normed space.

The space $\mathscr{K}_{\pi}(G)$ is contained in $\mathscr{F}_{\pi}^p(G)$. Its closure in $\mathscr{F}_{\pi}^p(G)$ is denoted by $\mathscr{L}_{\pi}^p(G, \nu )$, or simply $\mathscr{L}_{\pi}^p(G)$; one says that this is the space of $\pi$-equivariant functions on G whose $p^e$ power is integrable modulo H.

The assertions of the following proposition are, when $\pi$ is the trivial representation of dimension 1, consequences of INT, IV, p. 128, § 3, n$^o3$, prop. 6 and p. 131, §3, n$^o4$, th. 3.

#### Proposition 3 {#ts-v-s2-prop-3 .statement tag=03AG}

a) Let $(f_n)_{n\in\mathbf{N}}$ be a sequence in $\mathscr{F}_{\pi}^p(G)$ such that the series

$$
\sum_{n=0}^{+\infty}N_p(f_n)
$$

converges. Then the series with general term $f_n(g)$ is absolutely convergent for $g$ outside a set T which is negligible modulo H. Let $f$ be the function on G with values in E which is equal to the sum of this series on G - T and equal to 0 on T. Then one has $f\in \mathscr{F}_{\pi}^p(G)$ and the series with general term $f_n$ converges to $f$ in the space $\mathscr{F}_{\pi}^p(G)$;

b) Let $(f_n)$ be a sequence converging in $\mathscr{L}_{\pi}^p(G)$ to a function $f$. There exists a subsequence $(f_{n_k})$ extracted from $(f_n)$ such that $f_{n_k}(g)$ converges to $f(g)$ for every $g$ outside a set negligible modulo H;

c) The semi-normed spaces $\mathscr{F}_{\pi}^p(G)$ and $\mathscr{L}_{\pi}^p(G)$ are complete.

In assertion a), to say that the series with general term $f_n$ converges to $f$ in the space $\mathscr{F}_{\pi}^p(G)$ means that the sequence of partial sums $f_0+\cdots +f_n$ converges to $f$ in $\mathscr{F}_{\pi}^p(G)$. One then also says that $f$ is a sum of this series.

Let us prove a). By prop. 6 of INT, IV, p. 128, § 3, n$^o3$, there exists a $\nu$-negligible set $S\subset G/H$ such that the series with general term $\|f_n(gH)\|$ converges absolutely for $gH\notin S$. Moreover, the function $h$ which is equal to the sum of this series for $gH\notin S$ and which is zero for $gH\in S$ satisfies $N_p(h)<+\infty$.

The set $T =\overset{-1}{\varpi}(S)$ is negligible modulo H. For every $g \notin T$, the series with general term $f_n(g)$ is absolutely convergent in E. Define $f(g) =\sum f_n(g)$ for $g \notin T$ and $f(g) = 0$ otherwise. We have $f\in$ $\mathscr{F}_{\pi}(G)$. Note that $\|f(gH)\|\leqslant h(gH)$ for every $g\in G$, whence $N_p(f)\leqslant$ $N_p(h)<+\infty$. Thus $f\in \mathscr{F}_{\pi}^p(G)$. Similarly, we obtain

$$
N_p(f-\sum_{n=0}^kf_n)\leqslant \sum_{n=k+1}^{+\infty}N_p(f_n)
$$

for every $k\in \mathbf{N}$, hence the series $\sum f_n$ converges to $f$ in $\mathscr{F}_{\pi}^p(G)$. Assertion a) is proved.

Let us prove b). The sequence $(\|f_n-f\|)_{n\in\mathbf{N}}$ converges to 0 in the space $\mathscr{L}^p(G/H)$. By INT, IV, p. 131, § 4, n$^o3$, th. 3, there exists a subsequence $(\|f_{n_k}-f\|)_{k\in\mathbf{N}}$ which converges $\nu$-almost everywhere to 0. The sequence $(f_{n_k}(g))_{k\in\mathbf{N}}$ then converges to $f(g)$ for every $g$ outside a set negligible modulo H.

Finally, let us prove c). Let $(f_n)_{n\in\mathbf{N}}$ be a Cauchy sequence in $\mathscr{F}_{\pi}^p(G)$. There exists a strictly increasing sequence of integers $(n_k)_{k\in\mathbf{N}}$ such that $N_p(f_{n_{k+1}}-f_{n_k})\leqslant 2^{-k}$ for every $k\in \mathbf{N}$. For every $k\in \mathbf{N}$, put $h_k$ = $f_{n_{k+1}}-f_{n_k}\in \mathscr{F}_{\pi}^p(G)$. By a), the series with general term $h_k$ converges in $\mathscr{F}_{\pi}^p(G)$; let $h$ denote its sum. For every $\ell \in \mathbf{N}$, we obtain

$$
f_{n_0}+\sum_{k=0}^{\ell}h_k=f_{n_{\ell+1}}
$$

hence $f_{n_0}+h$ is a cluster value of the sequence $(f_n)$. It therefore converges (TG, II, p. 14, cor. 2 of prop. 5). Thus the space $\mathscr{F}_{\pi}^p(G)$ is complete; since the space $\mathscr{L}_{\pi}^p(G)$ is closed in $\mathscr{F}_{\pi}^p$(G), it is likewise complete.

#### Corollary {#ts-v-s2-n5-cor-1 .statement tag=03AH}

Let $(f_n)_{n\in\mathbf{N}}$ be a Cauchy sequence in $\mathscr{L}_{\pi}^p(G)$ and let $f\in \mathscr{F}_{\pi}(G)$ be such that $f_n(g)$ converges to $f(g)$ almost everywhere modulo H. Then $f\in \mathscr{L}_{\pi}^p(G)$ and $(f_n)_{n\in\mathbf{N}}$ converges to $f$ in $\mathscr{L}_{\pi}^p(G)$.

In fact, the function $f$ coincides almost everywhere modulo H with the limit of the sequence $(f_n)$ in $\mathscr{L}_{\pi}^p(G)$.

We denote by $L^p_{\pi}(G)$ the associated separated normed topological vector space of the semi-normed space $\mathscr{L}_{\pi}^p(G)$; it is a Banach space.

Let $f$ be a function on G with values in E. Denote by $S_f$ the set of $x\in G$ such that the function $h\mapsto f(xh)$ on H does not belong to $\mathscr{L}_E^1(H)$. One has $S_f\cdot h= S_f$ for every $h\in H$.

Let $x\in$ G - $S_f$. Since $\pi$ is a unitary representation, the function $h\mapsto \pi (h)^*f(xh)$ is measurable (as the composition of the mapping $h\mapsto (h, f(xh))$ of H into $H\times E$, which is then measurable, and of the continuous mapping $(g, x)\mapsto \pi (g)^*x$ of $H\times E$ into E, cf. INT, IV, p. 174, § 5, n$^o3$, Th. 1), and it is integrable on H.

One defines a function $f^{\pi}$ on G by putting

$$
f^{\pi}(x) =\int_H\pi (h)^*f(xh)d\beta (h) \tag{3}
$$

for $x\in G$ - $S_f$ and $f^{\pi}(x) = 0$ if $x\in S_f$.

#### Proposition 4 {#ts-v-s2-prop-4 .statement tag=03AI}

Let $f\in \mathscr{L}_E^1(G)$.

a) The set $S_f$ is negligible modulo H and $f^{\pi}\in \mathscr{F}_{\pi}(G)$;

b) Let C be a compact subset of G. If $f$ is continuous and has support contained in C, then $S_f$ is empty, the function $f^{\pi}$ belongs to $\mathscr{K}_{\pi}(G)$ and its support is contained in $C\cdot H$.

The first part of a) follows from INT, VII, p. 57, § 2, n$^o5$, c). Let $w\in H$. If $x\in G$ - $S_f$, then $xw\in G$ - $S_f$ and

$$
f^{\pi}(xw) =\int_H\pi (h)^*f(xwh)d\beta (h)
$$

$$
=\int_H\pi (w^{-1}y)^*f(xy)d\beta (y) =\pi (w)f^{\pi}(x)
$$

whereas if $x\in S_f$, then $f^{\pi}(xw) = 0 =\pi (w)^*f^{\pi}(x)$. The function $f^{\pi}$ therefore belongs to $\mathscr{F}_{\pi}(G)$.

Suppose now that $f$ is continuous and has support contained in C. For every $x\in G$, the mapping $h\mapsto f(xh)$ then belongs to $\mathscr{K}$ (H), hence is integrable, which proves that $S_f=\emptyset$.

Let us prove that $f^{\pi}$ is continuous. Let $x\in G$. Let U be a relatively compact open neighbourhood of $x$ in G.

For every $y\in U$, one has

$$
\|f^{\pi}(y)-f^{\pi}(x)\|\leqslant \int_H\|f(yh)-f(xh)\|d\beta (h)
$$

$$
=\int\|f(yh)-f(xh)\|d\beta (h)
$$

$H\cap (y^{-1}C\cup x^{-1}C)$

$\leqslant \beta (H\cap U^{-1}C)$ sup$_{h\in U^{-1}C}\|f(yh)-f(xh)\|$,

and the continuity of $f^{\pi}$ then follows from the uniform continuity of $f$ on G.

Finally, if $x\in G$ satisfies $f^{\pi}(x)\not = 0$, there exists $h\in H$ such that $f(xh)\not = 0$; thus $xh$ belong to C and $x$ belong to $C\cdot H$. Since $C\cdot H$ is closed in G, one concludes that the support of $f^{\pi}$ is contained in $C\cdot H$.

Let C be a compact subset of G. Let $u\in \mathscr{K}_+(G)$ be a function such that $u(x)>0$ for every $x\in C$. Let $v$ be the function on G defined by

$$
v(x) =\int_Hu(xh)d\beta (h) \tag{4}
$$

for every $x\in G$; with the preceding notation, one has $v=u^1$, corresponding to the trivial representation of dimension 1 of H. The function $v$ is continuous and positive; it belong to $\mathscr{F}_1$(G), its support is contained in Supp($u$)$\cdot H$ and one has

(5) $x$inf$^{\in}_{C\cdot H}v(x)>0$

(INT, VII, p. 39–40, § 2, n$^o1$, prop. 1 and lemma 1, a)).

#### Lemma 5 {#ts-v-s2-lem-5 .statement tag=03AJ}

Let $f\in \mathscr{F}_{\pi}(G)$ be a $\mu$-measurable function equal to zero outside $C\cdot H$ such that the function $\|f\|$ is $\nu$-integrable on $G/H$. Let $s$ be the E-valued function on G such that

$v(x)^{-1}f(x)$ if $x\in C\cdot H$

$$
s(x) =
$$

0 if $x\in G$ - $C\cdot H$.

a) The function $s$ is $\mu$-measurable; it belong to $\mathscr{F}_{\pi}(G)$ and is equal to zero outside $C\cdot H$;

b) The function $us$ belong to $\mathscr{L}^1(G)$ and $(us)^{\pi}=f$ almost everywhere modulo H.

The function $s$ is equal to zero outside $C\cdot H$ by definition; it is $\mu$-measurable since the function $f$ is $\mu$-measurable and $v(x)>0$ for every $x\in C\cdot H$ (INT, IV, p. 193, § 5, n$^o10$, prop. 16). One has $s\in \mathscr{F}_{\pi}(G)$ because $v\in \mathscr{F}_1(G)$.

The function $f$ is locally $\mu$-integrable, since $\|f\|$ is a $\nu$-integrable function (INT, VII, p. 47, § 2, No.$^o3$, prop. 6, c), noting that the measure $\nu^{\sharp}=\kappa \cdot \mu$ is equivalent to $\mu)$, hence the function $s$ is also so by formula (5). The function $us$ is measurable and zero outside a compact subset of G; since $u$ is bounded, it follows that $us$ is $\mu$-integrable.

For all $x\in G$ - $S_{us}$, we have

$$
(us)^{\pi}(x) =\int_H\pi (h)^*(u(xh)s(xh))d\beta (h)
$$

$$
=\int_Hu(xh)s(x)d\beta (h) =v(x)s(x)
$$

since $s(xh) =\pi (h)s(x)$; the last assertion follows from prop. 4, a).

When $H =\{e\}$ and $\pi$ is of dimension 1, the following proposition is none other than INT, IV, p. 184, § 5, No.$^o6$, th. 5.

#### Proposition 5 {#ts-v-s2-prop-5 .statement tag=03AK}

Let $p\in [1,+\infty [$. The space $\mathscr{L}_{\pi}^p(G)$ is the space of functions $f\in \mathscr{F}_{\pi}(G)$ such that $f$ is $\mu$-measurable and the function $\|f\|$ belong to $\mathscr{L}^p(G/H)$.

Let $f\in \mathscr{L}_{\pi}^p(G)$. It is the limit in $\mathscr{L}_{\pi}^p(G)$ of a sequence of elements of $\mathscr{K}_{\pi}(G)$. By prop. 3, b) and Egoroff's theorem (INT, IV, p. 175, § 5, No.$^o4$, th. 2), the function $f$ is therefore $\mu$-measurable; consequently, the function $\|f\|$ on $G/H$ is $\nu$-measurable (INT, VII, p. 47, § 2, No.$^o3$, prop. 6, b)). Since $N_p(f)$ is finite, the function $\|f\|$ belong to $\mathscr{L}^p(G/H)$ (INT, IV, p. 184, § 5, No.$^o6$, th. 5).

Let us prove the converse assertion. Let $f$ be a $\mu$-measurable function belonging to $\mathscr{F}_{\pi}(G)$ such that $\|f\| \in \mathscr{L}^p(G/H)$. Let $\varepsilon  >0$. Let us prove that there exists $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ such that

$$
N_p(f-\widetilde{f})^p=\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

which will conclude the proof.

Suppose first that there exists a compact subset C of G such that $f$ is zero outside $C\cdot H$. Let $u\in \mathscr{K}_+(G)$ be a function such that $u(x)>0$ for all $x\in C$ and define $v=u^1$ as above. Let us denote by $\varphi$ the characteristic function of the support of $u$.

Let $q$ be the conjugate exponent of $p$. If $p= 1$, let $w$ be the constant function on G equal to sup$_{x\in G}u(x)$. If $p >1$, define

$$
w(x)=\left(\int_Hu(xh)^q\,d\beta(h)\right)^{1/q}
$$

for every $x\in G$. In both cases, the function $w$ is continuous and positive; it belongs to $\mathscr{K}_1(G)$ (Prop. 4 applied to the trivial representation of dimension 1 and to the function $u^q$), hence it is bounded on G. Put W = sup$_{x\in G}w(x)$.

Let $s$ be the function on G with values in E defined by Lemma 5 applied to $f$. Put $g=\varphi s$. The function $g$ is $\mu$-measurable, and satisfies $\|g\|\leqslant \|f\|/$ inf$_{x\in C\cdot H}v(x)$. Since $g$ vanishes outside the support of $u$ and $\kappa$ is continuous, we have $g\in \mathscr{L}_E^p(G, \kappa \cdot \mu)$. Let $\widetilde{g}$ be a function in $\mathscr{K}_E(G)$ such that

$$
\int^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon_p
$$

$_G$ W

We have $us=ug$, hence $f= (us)^{\pi}= (ug)^{\pi}$ almost everywhere modulo H (Lemma 5, b)). Let $\widetilde{f}= (u\widetilde{g})^{\pi}$; we have $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ (Prop. 4, b)). For every $x\in G$ - $S_{ug}$, we obtain

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|\leqslant \int_H^*u(xh)\|g(xh)-\widetilde{g}(xh)\|d\beta (h)
$$

whence

$$
\|(ug)^{\pi}(x)-(u\widetilde{g})^{\pi}(x)\|^p\leqslant w(x)^p\int_H^*\|g(xh)-\widetilde{g}(xh)\|^pd\beta (h)
$$

by Hölder's inequality in the case $p >1$. Since $S_{ug}$ is negligible modulo H, it follows that

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant W^p\int_{G/H}^*(\int_H^*\|g(xh)-\widetilde{g}(xh)\|d\beta (h))^pd\nu (xH)
$$

$$
= W^p\int_G^*\|g-\widetilde{g}\|^p\kappa  d\mu\leqslant \varepsilon
$$

by INT, VII, p. 46, § 2, n$^o3$, Prop. 5, b), which is applicable since $g-\widetilde{g}$ vanishes outside a compact subset of G. This implies the required property when $f$ vanishes outside a compact subset modulo H.

Consider now the general case. Since $\|f\| \in \mathscr{L}^p(G/H)$ by hypothesis, there exists a compact subset L of $G/H$ such that

$$
\int^*p\varepsilon
$$

$$
\|f\|d\nu \leqslant
$$

$(G/H)-L$ 2

(cf. INT, IV, p. 152, § 4, n$^o6$, th. 4). Let $\varphi_L$ be the characteristic function of L and put $f_L= (\varphi_L\circ \varpi )f$. We have

$$
\int^*p\int^*p\varepsilon
$$

$$
\|f-f_L\|d\nu =\|f\|d\nu \leqslant
$$

$G/H(G/H)-L$ 2

The function $f_L$ is $\mu$-measurable and vanishes outside a compact set modulo H. It belongs to $\mathscr{L}_{\pi}^p$(G), hence by the preceding case, there exists $\widetilde{f}\in \mathscr{K}_{\pi}(G)$ such that $N_p(f_L-\widetilde{f})\leqslant (\frac{\varepsilon}{2})^{1/p}$, whence

$$
\int_{G/H}^*\|f-\widetilde{f}\|^pd\nu \leqslant \varepsilon
$$

as desired.

Let us consider the case $p= 2$. For $f_1$ and $f_2$ in $\mathscr{F}_{\pi}$(G), the function $x\mapsto  \langle f_1(x)|f_2(x)\rangle$ belongs to $\mathscr{F}_1(G)$ since the representation $\pi$ is unitary, and therefore defines by passing to the quotient a function on $G/H$, which is identified as above with $\langle f_1|f_2\rangle$. One has the majorization $|\langle f_1|f_2\rangle |\leqslant \|f_1\|\|f_2\|$ in $\mathscr{F}(G/H)$.

If $f_1$ and $f_2$ belong to $\mathscr{L}_{\pi}^2$(G), then the function $\langle f_1|f_2\rangle$ belongs to $\mathscr{L}_1^1(G)$. In particular, it is integrable on $G/H$. The mapping

$$
(f_1, f_2)\mapsto \int_{G/H}\langle f_1|f_2\rangle d\nu
$$

is a positive Hermitian form on $\mathscr{L}_{\pi}^2(G)$; the associated seminorm is the seminorm $N_2$. In particular, the space $\mathscr{L}_{\pi}^2(G)$ is a prehilbertian space and $L^2_{\pi}(G)$ is the Hilbert space associated with $\mathscr{L}_{\pi}^2(G)$.

### 6. Induced representations

We retain the notations and conventions of the preceding number concerning the measures $\beta$ on H and $\nu$ on $G/H$, as well as the function $\kappa : G\rightarrow \mathbf{R}^*_+$.

There exists a continuous function $\eta$ of $G\times G/H$ into $\mathbf{R}_+^*$ such that

$$
\eta (x, yH) =\frac{\kappa(xy)}{\kappa(x)}
$$

for every $(x, y)\in G\times G$, and $\boldsymbol{\gamma }_{G/H}(x)\nu = (y\mapsto \eta (x^{-1}, y))\cdot \nu$ for $x\in G$ (INT, VII, p. 56, § 2, n$^o5$, th. 2, c)).

Let $p\in [1,+\infty [$ and let $\pi$ be a unitary representation of H in a complex Hilbert space E.

#### Lemma 6 {#ts-v-s2-lem-6 .statement tag=03AL}

Let $f\in \mathscr{K}_{\overline{\pi}}(G)$. For every $g\in G$, the function

$$
\widetilde{f}:x\mapsto \eta (g^{-1}, xH)^{1/p}f(g^{-1}x)
$$

of G into E belongs to $\mathscr{K}_{\overline{\pi}}(G)$ and satisfies $N_p(\widetilde{f}) = N_p(f)$.

It is verified without difficulty that $\widetilde{f}\in \mathscr{K}_{\overline{\pi}}(G)$. Since

$$
N_p(\widetilde{f})^p=\int_{G/H}^*\|\widetilde{f}\|^pd\nu =\int_{G/H}^*\gamma_{G/H}(g)(\|f\|^p)(y)\eta (g^{-1}, y)d\nu (y)
$$

and since $(y\mapsto \eta (g^{-1}, y))\cdot \nu =\boldsymbol{\gamma }_{G/H}(g)\nu$, one obtains $N_p(\widetilde{f}) = N_p(f)$.

It follows from this lemma that there exists a continuous isometric representation $\widetilde{\pi}$ of G in $L^p_{\overline{\pi}}(G)$ such that for $f\in \mathscr{K}_{\pi}(G)$ and $g\in G$, the element $\widetilde{\pi}(g)f$ is the class of the function $\widetilde{f}$ defined above. If $p= 2$, then this representation is unitary.

#### Definition 2 {#ts-v-s2-def-2 .statement tag=03AM}

One says that the unitary representation of G in the space $L^2_{\overline{\pi}}(G)$ thus defined is the unitary representation of G induced by the representation $\pi$ of H relative to $\kappa$. It is denoted by Ind$^G_H(\pi , \kappa )$, or simply Ind$^G_H(\pi )$.

#### Remark 1 {#ts-v-s2-n6-rem-1 .statement tag=03AN}

Let $\varrho$ be a unitary representation of H in a complex Hilbert space F and let $u:\pi \rightarrow \varrho$ be an H-morphism. For every function $f\in \mathscr{K}_{\overline{\pi}}$(G), let $v(f)$ denote the function $g\mapsto u(f(g))$ from G into F; it belongs to $\mathscr{K}_{\overline{\varrho}}(G)$ and satisfies $N_p(v(f))\leqslant \|u\|N_p(f)$. The linear mapping from $\mathscr{K}_{\overline{\pi}}(G)$ into $\mathscr{K}_{\overline{\varrho}}(G)$ which associates $v(f)$ with $f$ therefore extends to a continuous H-morphism from Ind$^G_H(\pi )$ into Ind$^G_H(\varrho )$ which is denoted by Ind$^G_H(u)$. We have Ind$^G_H(1_{\pi}) = 1_{Ind^G_H(\pi)}$. Let $\sigma$ be a unitary representation of H and let $v:\varrho \rightarrow \sigma$ be an H-morphism; we have Ind$^G_H(v\circ u) =$ Ind$^G_H(v)\circ$ Ind$^G_H(u)$.

*In other words, the construction which associates Ind$^G_H(\pi )$ with $\pi$ and Ind$^G_H(u)$ with $u$ is a functor from the category of unitary representations of H into that of unitary representations of G (cf. CAT, I, § 2, in preparation).*

#### Remark 2 {#ts-v-s2-n6-rem-2 .statement tag=03AO}

Let $\kappa ': G\rightarrow \mathbf{R}_+^*$ be such that

$$
\frac{\kappa'(xh)}{\kappa'(x)}=\frac{\Delta_H(h)}{\Delta_G(h)}=\frac{\kappa(xh)}{\kappa(x)}
$$

for every $(x, h)\in G\times H$. Let $\nu '$ be the quasi-invariant measure $(\kappa '\cdot \mu)/\beta$ on $G/H$. The function $\kappa '\kappa^{-1}$ defines, by passing to quotients, a continuous function $\xi : G/H\rightarrow \mathbf{R}_+^*$ such that $\nu '=\xi \cdot \nu$. The endomorphism $\alpha$ of $\mathscr{K}_{\pi}(G)$ defined by $f\mapsto (\kappa '\kappa^{-1})^{1/p}f$ satisfies

$$
\int_{G/H}^*\|f\|^pd\nu '=\int_{G/H}^*\|\alpha (f)\|^pd\nu
$$

and makes it possible to identify the spaces $\mathscr{L}_{\pi}^p(G, \nu ')$ and $\mathscr{L}_{\pi}^p(G, \nu )$, as well as the spaces $L^p_{\pi}(G, \nu ')$ and $L^p_{\pi}(G, \nu )$. Moreover, $\alpha$ induces an isometric isomorphism of the representations Ind$^G_H(\pi , \kappa ')$ and Ind$^G_H(\pi , \kappa )$.

### 7. Case of a central closed subgroup

In this No., it is assumed that the group G is unimodular.

Consider a closed subgroup Z of the center of G, and let $dz$ denote a Haar measure on Z. The quotient group $G/Z$ is endowed with the Haar measure $\nu =\mu/dz$. Let $\chi$ be a unitary character of Z. The quotient group $G/Z$ is unimodular by INT, VII, p. 61, § 2, n$^o7$, cor. of prop. 11.

#### Lemma 7 {#ts-v-s2-lem-7 .statement tag=03AP}

We have

$$
N_1(\check{f}) = N_1(f),\langle f_1|f_2\rangle =\langle \check{f}_1|\check{f}_2\rangle \tag{6}
$$

for every $f\in \mathscr{F}_{\chi}(G)$ and all $f_1$ and $f_2$ in $\mathscr{L}_{\chi}^2(G)$.

These formulas are consequences of the definitions.

For every $g\in G$ and every $f\in \mathscr{F}_{\chi}$(G), the functions $x\mapsto f(g^{-1}x)$ and $x\mapsto f(xg)$ belong to $\mathscr{F}_{\chi}(G)$. They are denoted respectively by $\boldsymbol{\gamma }_{G,\chi}(g)f$ and $\boldsymbol{\delta }_{G,\chi}(g)f$. The mappings $\boldsymbol{\gamma }_{G,\chi}$ and $\boldsymbol{\delta }_{G,\chi}$ are linear representations of G in $\mathscr{F}_{\chi}(G)$. For every $z\in Z$, one has

$$
\boldsymbol{\gamma }_{G,\chi}(gz) =\overline{\chi(z)}\boldsymbol{\gamma }_{G,\chi}(g),\boldsymbol{\delta }_{G,\chi}(gz) =\chi (z)\boldsymbol{\delta }_{G,\chi}(g) \tag{7}
$$

Let $f\in \mathscr{F}_{\chi}(G)$ and $g\in G$; one has

$$
|\boldsymbol{\gamma }_{G,\chi}(g)f|=\boldsymbol{\gamma }_{G/Z}(gZ)|f|,|\boldsymbol{\delta }_{G,\chi}(g)f|=\boldsymbol{\delta }_{G/Z}(gZ)|f| \tag{8}
$$

where all the functions occurring in these equalities are identified with functions on $G/Z$.

The subspace $\mathscr{K}_{\chi}(G)$ of $\mathscr{F}_{\chi}(G)$ is stable under $\boldsymbol{\gamma }_{G,\chi}$ and $\boldsymbol{\delta }_{G,\chi}$. Let $p$ be a real number $\geqslant 1$. Formulae (8) imply that the representations $\boldsymbol{\gamma }_{G,\chi}$ and $\boldsymbol{\delta }_{G,\chi}$, restricted to $\mathscr{K}_{\chi}$(G), extend to continuous isometric linear representations of G in $\mathscr{L}_{\chi}^p$(G), which will be denoted by $\boldsymbol{\gamma }^{(p)}_{G,\chi}$ and $\boldsymbol{\delta }^{(p)}_{G,\chi}$. By passing to quotients, these representations also define isometric representations of G in $L^p_{\chi}$(G), denoted in the same way.

The representations $\boldsymbol{\gamma }^{(2)}_{G,\chi}$ and $\boldsymbol{\delta }^{(2)}_{G,\chi}$ in $L_{\chi}^2(G)$ are unitary, and will be denoted simply by $\boldsymbol{\gamma }_{G,\chi}$ and $\boldsymbol{\delta }_{G,\chi}$, respectively, whenever no confusion with the representations in $\mathscr{F}_{\chi}(G)$ is possible. One also denotes by $\boldsymbol{\varrho }_{G,\chi}$ the continuous representation of $G\times G$ in $\mathscr{L}_{\chi}^2(G)$ or $L^2_{\chi}(G)$ defined by

$$
\boldsymbol{\varrho }_{G,\chi}(g, h) =\boldsymbol{\gamma }_{G,\chi}(g)\circ \boldsymbol{\delta }_{G,\chi}(h) =\boldsymbol{\delta }_{G,\chi}(h)\circ \boldsymbol{\gamma }_{G,\chi}(g)
$$

for every $(g, h)\in G\times G ($cf. Lemma 1 of V, p. 377).

The representation $\boldsymbol{\gamma }_{G,\chi}$ on $L^2_{\chi}(G)$ is none other than the induced representation Ind$^G_Z(\overline{\chi})$.

When $Z =\{e\}$, the following lemma results from INT, VIII, p. 166, § 4, n$^o5$, Prop. 12, since G is unimodular.

#### Lemma 8 {#ts-v-s2-lem-8 .statement tag=03AQ}

Let $f_1\in \mathscr{K}_{\chi}(G)$ and $f_2\in \mathscr{L}_{\chi}^2(G)$.

a) The function $f$ on G defined by $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ for every $g\in G$ belong to $\mathscr{L}_{\overline{\chi}}^2(G)$ and satisfies $N_2(f)\leqslant N_1(f_1)N_2(f_2)$;

b) The function $f$ on G defined by $f(g) =\langle f_1|\boldsymbol{\delta }_{G,\chi}(g)f_2\rangle$ for every $g\in G$ belong to $\mathscr{L}_{\chi}^2(G)$ and satisfies $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Let us prove a), the proof of assertion b) being similar. The function $f$ is continuous, hence $\mu$-measurable. For every $z\in Z$ and every $g\in G$, we have

$$
f(gz) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(gz)f_2\rangle =\overline{\chi(z)}\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

(formula (7), p. 417), hence $f\in \mathscr{F}_{\overline{\chi}}(G)$. Prop. 5 of V, p. 413 implies that it now suffices to prove that $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

Suppose first that $f_2$ belongs to $\mathscr{K}_{\chi}(G)$. For every $g\in G$, by definition we have

$$
f(g) =\int_{G/Z}\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2d\nu
$$

where the function $\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2$ is identified with a function on $G/Z$.

Define a function $f_3$ on G by putting $f_3(g) = 0$ if $f_1(g) = 0$ and $f_3(g) =f_1(g)|f_1(g)|^{-1/2}$ otherwise. The function $f_3$ belongs to $\mathscr{F}_{\chi}(G)$ and satisfies $f_1=|f_1|^{1/2}f_3$; it is $\mu$-measurable and zero outside a compact modulo Z, since $f_1$ is. Since $|f_1|^{1/2}\in \mathscr{K}_1$(G), it follows that

$$
\overline{f_1}\boldsymbol{\gamma }_{G,\chi}(g)f_2=|f_1|^{1/2}\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2
$$

$$
|\overline{f_3}\boldsymbol{\gamma }_{G,\chi}(g)f_2|=|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|
$$

for every $g\in G$.

Let $g\in G$. By the Cauchy-Schwarz inequality, we have

$$
|f(g)|^2\leqslant (\int_{G/Z}|f_1|^{1/2}|f_3| |\boldsymbol{\gamma }_{G,\chi}(g)f_2|d\nu )^2
$$

$$
\leqslant (\int_{G/Z}|f_1|d\nu )(\int_{G/Z}|f_3|^2|\boldsymbol{\gamma }_{G,\chi}(g)f_2|^2d\nu )
$$

Since we have $|f_3|^2=|f_1|$ in $\mathscr{K}(G/Z)$, it follows, on integrating over $G/Z$, that

$$
\int_{G/Z}|f(g)|^2d\nu (g)\leqslant N_1(f_1)\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

The function on $G/Z\times G/Z$ deduced from the function

$$
(g, x)\mapsto  |f_1(x)| |f_2(g^{-1}x)|^2
$$

by passing to quotients is $(\nu \otimes \nu$)-measurable and has compact support, hence it is $(\nu \otimes \nu$)-moderate (INT, V, p. 4, § 5, No.$^o2$, Def. 2). By Prop. 7 of INT, V, p. 93, § 8, No.$^o3$, it follows that

$$
\int_{G/Z}(\int_{G/Z}|f_1(x)| |f_2(g^{-1}x)|^2d\nu (x))d\nu (g)
$$

$$
=\int_{G/Z}|f_1(x)|(\int_{G/Z}|f_2(g^{-1}x)|^2d\nu (g))d\nu (x) = N_1(f_1)N_2(f_2)^2
$$

Consequently, we have $N_2(f)^2\leqslant N_1(f_1)^2N_2(f_2)^2$, which establishes the required property in this case.

Let us consider the general case. Let $u$ denote the linear mapping of $\mathscr{K}_{\chi}(G)$ into $\mathscr{L}_{\overline{\chi}}^2(G)$ which associates $f$ to $f_2$. Let $f_2\in \mathscr{L}_{\chi}^2(G)$ and let $(f_{2,n})_{n\in\mathbf{N}}$ be a sequence in $\mathscr{K}_{\chi}(G)$ converging to $f_2$ in $\mathscr{L}_{\chi}^2(G)$. Let $f_n=u(f_{2,n})$; the sequence $(f_n)_{n\in\mathbf{N}}$ is a Cauchy sequence in $\mathscr{L}_{\overline{\chi}}^2(G)$ since the preceding case implies that $N_2(f_n-f_m)\leqslant N_1(f_1)N_2(f_{2,n}-f_{2,m})$ for all $n$ and $m$ in $\mathbf{N}$. Let $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ be such that $(f_n)$ converges to $f$ (Prop. 3, c) of V, p. 409). Since $N_2(f_n)\leqslant N_1(f_1)N_2(f_{2,n})$ for every $n\in \mathbf{N}$, it follows that $N_2(f)\leqslant N_1(f_1)N_2(f_2)$.

There exists a subsequence $(f_{n_k})_{k\in\mathbf{N}}$ such that $f_{n_k}(g)$ converges to $f(g)$ for every $g\in G$ outside a subset of G negligible modulo Z (loc. cit., b)). But on the other hand, for every $g\in G$, one has

$$
f_{n_k}(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_{2,n_k}\rangle  \rightarrow  \langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle
$$

Consequently, one has $f(g) =\langle f_1|\boldsymbol{\gamma }_{G,\chi}(g)f_2\rangle$ for every $g$ outside a subset of G negligible modulo Z. Since $f\in \mathscr{L}_{\overline{\chi}}^2(G)$ and $N_2(f)\leqslant N_1(f_1)N_2(f_2)$, the lemma is proved.

### 8. Square-integrable representations

In this No., the Hilbert spaces considered are complex. It is assumed that G is unimodular, and C denotes its center. For every closed subgroup Z of C, let $\beta_Z$ denote a Haar measure on Z, and endow $G/Z$ with the Haar measure $\nu_Z=\mu/\beta_Z$ (INT, VII, p. 44, § 2, n$^o2$, Def. 1).

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E, and let $\chi \in \widehat{C}$ be its central character (Def. 6 of V, p. 390). For all $x$ and $y$ in E, let $f_{x,y}$ denote the matrix coefficient $g\mapsto  \langle x|\pi (g)y\rangle$; this is a continuous complex-valued function on G.

Let $x$ and $y$ be in E. For $z\in C$ and $g\in G$, one has

$$
f_{x,y}(zg) =\langle x|\pi (zg)y\rangle =\langle x|\chi (z)\pi (g)y\rangle =\chi (z)f_{x,y}(g) \tag{9}
$$

therefore $f_{x,y}$ belong to the space $\mathscr{F}_{\chi}(G) ($V, p. 408). Moreover, for every $(g_1, h_1)\in G\times G$ and every $g\in G$, one has

$$
f_{\pi(g_1)x,\pi(h_1)y}(g) =\langle \pi (g_1)x|\pi (g)\pi (h_1)y\rangle =f_{x,y}(g_1^{-1}gh_1) \tag{10}
$$

Relation (9) justifies the following definition.

#### Definition 3 {#ts-v-s2-def-3 .statement tag=03AR}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. One says that $\pi$ is square-integrable modulo the center if the function on $G/C$ deduced from the function $|f_{x,y}|$ by passing to the quotient belong to $\mathscr{L}^2(G/C)$ for every $(x, y)\in E\times E$.

This condition does not depend on the choice of a Haar measure on $G/C$.

If the matrix coefficients of $\pi$ belong to $\mathscr{L}^2$(G), one says that $\pi$ is square-integrable; the existence of an irreducible unitary square-integrable representation of G implies that the center of G is compact (exercise 5 of V, p. 487).

There exist groups G which admit no square-integrable representation, even modulo the center (cf. exercise 32 of V, p. 516).

#### Proposition 6 {#ts-v-s2-prop-6 .statement tag=03AS}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. Let $\chi$ be the central character of $\pi$. Then $\pi$ is square-integrable modulo the center if and only if there exist non-zero elements $x_0$ and $y_0$ of E such that the function on $G/C$ deduced from $|f_{x_0,y_0}|$ by passing to the quotient belongs to $\mathscr{L}^2(G/C)$.

Suppose that there exist non-zero elements $x_0$ and $y_0$ of E such that $|f_{x_0,y_0}| \in \mathscr{L}^2(G/C)$. It is enough to prove that $\pi$ is then square-integrable modulo the center.

Let F be the set of elements $x\in E$ such that $|f_{x,y_0}|$ belongs to $\mathscr{L}^2(G/C)$. It is a vector subspace of E; it contains $x_0$, hence is non-zero. Relation (10) above implies that F is stable under $\pi$; since the representation $\pi$ is irreducible, the space F is therefore dense in E.

Let $x\in F$. Since $f_{x,y_0}$ belongs to $\mathscr{F}_{\chi}(G)$ and is $\mu$-measurable, and since $|f_{x,y_0}| \in \mathscr{L}^2(G/C)$, one has $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ (Prop. 5 of V, p. 413 applied to Z = C). Let $u$ denote the partial operator from E into $L^2_{\chi}(G)$ whose domain is F and which associates to $x\in F$ the class of $f_{x,y_0}$ in $L^2_{\chi}(G)$.

Let us prove that the partial operator $u$ is closed. Let $(x_n, u(x_n))_{n\in\mathbf{N}}$ be a sequence of elements of the graph of $u$ which converges in $E\times L^2_{\chi}(G)$. Let $x$ be the limit of $(x_n)$ and let $f\in \mathscr{L}_{\chi}^2(G)$ be a function whose class is the limit of the sequence $(u(x_n))$.

The function $u(x_n)$ is the class of the matrix coefficient $f_{x_n,y_0}$. For every $g\in G$, one has

$$
f_{x_n,y_0}(g) =\langle x_n|\pi (g)y_0\rangle  \rightarrow  \langle x|\pi (g)y_0\rangle =f_{x,y_0}(g)
$$

when $n\rightarrow +\infty$. Hence $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$ and $f=f_{x_0,y}$ almost everywhere modulo C (cor. of Prop. 3 of V, p. 409); this means that $u(x)$ is the class of $f$ in $L^2_{\chi}(G)$. Thus we have proved that $u$ is closed.

The domain F of $u$ is stable under $\pi$, and relation (10) proves that $u$ satisfies $u\circ \pi (g) =\boldsymbol{\gamma }_{G,\chi}(g)\circ u$ for all $g\in G$. Consequently one also has the equality $u^*\circ \boldsymbol{\gamma }_{G,\chi}(g) =\pi (g)\circ u^*$ for all $g\in G$ (lemma 6 of V, p. 381), whence $(u^*\circ u)\circ \pi (g) =\pi (g)\circ (u^*\circ u)$. Now the partial operator $u^*\circ u$ is self-adjoint (prop. 12 of IV, p. 241), and in particular closed (prop. 7 of IV, p. 236), hence cor. 1 of V, p. 387 implies that the domain of $u^*\circ u$ is equal to E. A fortiori, one has F = E, that is to say that the function $|f_{x,y_0}|$ belongs to $\mathscr{L}^2(G/C)$ for all $x\in E$.

Let $(x, y)\in E\times E$. One has $f_{x,y_0}\in \mathscr{L}_{\chi}^2(G)$. One proves mutatis mutandis, using the representation $\boldsymbol{\delta }_{G,\chi}$ instead of $\boldsymbol{\gamma }_{G,\chi}$, that the set of $y\in E$ such that the function $|f_{x,y}|$ belongs to $\mathscr{L}^2(G/C)$ is equal to E. The proposition follows.

In the remainder of this No., we fix a closed subgroup Z of C such that $C/Z$ is compact.

#### Lemma 9 {#ts-v-s2-lem-9 .statement tag=03AT}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E which is square-integrable modulo the center. Let $\chi$ be the restriction to Z of the central character of $\pi$. For all $x$ and $y$ in E, one has $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$.

The function $f_{x,y}$ is continuous, hence $\mu$-measurable. One has $f_{x,y}\in \mathscr{F}_{\chi}(G)$ by formula (9), p. 420. Moreover, by INT, VII, p. 64, § 2, No.$^o8$, cor. 1, c), one has $N_2(f_{x,y})<+\infty$ since $C/Z$ is compact and $|f_{x,y}| \in \mathscr{L}^2(G/C)$. The assertion therefore follows from proposition 5 of V, p. 413.

#### Proposition 7 {#ts-v-s2-prop-7 .statement tag=03AU}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E which is square-integrable modulo the center. Let $\chi$ be the restriction to Z of the central character of $\pi$.

There exist a real number $c >0$ and a unique isometric $(G\times G)$-morphism $w$ of the unitary representation $\overline{\pi}\boxtimes \pi$ into $L^2_{\chi}(G)$ such that, for all $(x, y)\in \overline{E}\times E$, the element $w(x\otimes y)$ is the class in $L^2_{\chi}(G)$ of the function $c^{1/2}f_{x,y}$.

For all $(x, y)\in E\times E$, one has $f_{x,y}\in \mathscr{L}_{\chi}^2(G)$ (lemma 9). Let $v$ denote the unique linear mapping of $\overline{E}\otimes E$ into $L^2_{\chi}(G)$ such that $v(x\otimes y)$ is the class of $f_{x,y}$ for all $(x, y)\in E\times E$.

We shall prove below the following lemma.

#### Lemma 10 {#ts-v-s2-lem-10 .statement tag=03AV}

There exists a real number $c >0$ such that the linear mapping $w=c^{1/2}v$ is isometric.

This lemma being assumed valid, let us remark that formula (10), p. 420, may be written

$$
v(\overline{\pi}(g_1)x\otimes \pi (h_1)y) =\boldsymbol{\varrho }_{G,\chi}(g_1, h_1)v(x\otimes y) \tag{11}
$$

for all $(g_1, h_1)\in G\times G$ and all $(x, y)\in \overline{E}\times E$. The isometric linear mapping $w$ of $\overline{E}\otimes E$ into $L^2_{\chi}(G)$ admits a continuous extension, still denoted by $w$, to $E\widehat{\otimes}_2E$. By continuity and linearity, formula (11) implies that $w$ is a $(G\times$ G)-morphism of $\overline{\pi}\boxtimes \pi$ into $L^2_{\chi}$(G), which concludes the proof of the proposition.

Let us prove the lemma. For every $x\in E$, let $u_x$ denote the linear mapping $y\mapsto v(x\otimes y) =f_{x,y}$ of E into $L^2_{\chi}(G)$. We have $u_x\in$ Hom$_G(\pi ,\boldsymbol{\gamma }_{G,\chi})$ (formula (10)). By cor. 5 of V, p. 388, there exists a real number $\lambda_x\geqslant 0$ such that $\lambda_xu_x$ is isometric.

Let $x$ and $y$ be in E. We have

$$
\|f_{x,y}\|^2=\int_{G/Z}\overline{f}_{x,y}f_{x,y}d\nu_Z=\int_{G/Z}\overline{\check{f}}_{x,y}\check{f}_{x,y}d\nu_Z
$$

since $G/Z$ is unimodular (lemma 7 of V, p. 417). Noting that $\check{f}_{x,y}=f_{y,x}$, we obtain

$$
\lambda_x\|y\|^2=\|f_{x,y}\|^2=\int_{G/Z}f_{y,x}\overline{f}_{y,x}d\nu_Z=\|f_{y,x}\|^2=\lambda_y\|x\|^2
$$

This means that the positive real number $\lambda_x/\|x\|^2$ is independent of the choice of the nonzero element $x$ of E. It is strictly positive since, for every nonzero $x$, the function $f_{x,x}$ is continuous and takes the value $\|x\|^2>0$ at $e$, whence $\|u_x(x)\|=\|f_{x,x}\|>0$. Let us denote this real number by $c^{-1}$.

For every $(x, y)\in E\times E$, it follows that

$$
\|v(x\otimes y)\|^2=\|f_{x,y}\|^2=\lambda_x\|y\|^2=c^{-1}\|x\|^2\|y\|^2=c^{-1}\|x\otimes y\|^2
$$

Using EVT, V, p. 29, cor. 1, we deduce that the linear mapping $w=c^{1/2}v$ of $\overline{E}\widehat{\otimes}_2E$ into $L^2_{\chi}(G)$ is isometric, as required.

#### Corollary {#ts-v-s2-n8-cor-1 .statement tag=03AW}

Let $\pi$ be an irreducible unitary representation of G and let $\chi$ be the restriction to Z of its central character. The representation $\pi$ is square-integrable modulo the center if and only if it is isomorphic to a subrepresentation of the representation $\boldsymbol{\gamma }_{G,\chi}$ of G in $L^2_{\overline{\chi}}(G)$ (resp. of the representation $\boldsymbol{\delta }_{G,\chi}$ of G in $L^2_{\chi}(G)$).

Let us prove the assertion concerning $\boldsymbol{\gamma }_{G,\chi}$, the second being proved in a similar way.

Suppose first that there exists a subrepresentation E of the representation $\boldsymbol{\gamma }_{G,\chi}$ isomorphic to $\pi$. Since the space E is nonzero, there exists a function $f_1\in \mathscr{K}_{\overline{\chi}}(G)$ whose class $\widetilde{f}_1$ is not orthogonal to E. We have $f_1\in \mathscr{L}_{\overline{\chi}}^1(G)$. Let $\widetilde{f}_{1,E}$ denote the orthogonal projection of $\widetilde{f}_1$ on E; it is a nonzero element of E. Let moreover $\widetilde{f}_2\in E$ be nonzero. The mapping $h:g\mapsto  \langle \widetilde{f}_{1,E}|\boldsymbol{\gamma }_{G,\chi}(g)\widetilde{f}_2\rangle$ is a matrix coefficient of $\pi$. For every $g\in G$, we have $h(g) =\langle \widetilde{f}_1|\boldsymbol{\gamma }_{G\overline{,\chi}}(g)\widetilde{f}_2\rangle$ since $\widetilde{f}_1-\widetilde{f}_{1,E}$ is orthogonal to E. By Lemma 8 of V, p. 418, the function $h$ belongs to $\mathscr{L}_{\chi}^2$(G), hence Proposition 6 implies that $\pi$ is square-integrable modulo the center.

Conversely, suppose that $\pi$ is square-integrable modulo the center. Let $x_0\in E$ be a nonzero vector. By Prop. 7 and formula (10), the mapping $y\mapsto \check{f}_{x_0,y}$ is an injective G-morphism of $\pi$ into $\boldsymbol{\gamma }_{G,\chi}$.

#### Definition 4 {#ts-v-s2-def-4 .statement tag=03AX}

Let Z be a closed subgroup of C such that $C/Z$ is compact. Let $\pi$ be an irreducible unitary representation of G which is square-integrable modulo the center. The unique real number $c >0$ which satisfies the property of Proposition 7 is called the formal degree of $\pi$ relative to Z. It is denoted by $c_Z(\pi )$.

The formal degree depends on the choice of the Haar measure on Z. If the Haar measure $\beta_Z$ on Z is multiplied by a real number $t >0$, then the measure $\nu_Z=\mu/\beta_Z$ on $G/Z$ is multiplied by $t^{-1}$, and the formal degree of $\pi$ is multiplied by $t$.

The formal degree is characterized by the following property:

#### Proposition 8 (Orthogonality relations) {#ts-v-s2-prop-8 .statement tag=03AY}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E which is square-integrable modulo the center. One has

$$
c_Z(\pi )\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle x|y\rangle \langle x'|y'\rangle
$$

for every $(x, y, x', y')\in E^4$.

Let $w$ denote the morphism of Prop. 7. One has

$$
\int_{G/Z}\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y'\rangle d\nu_Z(g) =\langle f_{x,x'}|f_{y,y'}\rangle
$$

and by loc. cit., it follows that

$$
\langle f_{x,x'}|f_{y,y'}\rangle =\frac{1}{c_Z(\pi)}\langle w(x\otimes x')|w(y\otimes y')\rangle
$$

$$
=\frac{1}{c_Z(\pi)}\langle x\otimes x'|y\otimes y'\rangle =\frac{1}{c_Z(\pi)}\langle x|y\rangle_{\overline{E}}\langle x'|y'\rangle_E
$$

whence the result.

As a complement to the preceding proposition, one also has the following relations for nonisomorphic irreducible square-integrable representations.

#### Proposition 9 {#ts-v-s2-prop-9 .statement tag=03AZ}

Let $\pi_1$ and $\pi_2$ be nonisomorphic irreducible unitary representations of G in Hilbert spaces $E_1$ and $E_2$. Suppose that $\pi_1$ and $\pi_2$ are square-integrable modulo the center and that the restrictions to Z of their central characters coincide. Then

$$
\int_{G/Z}\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\nu_Z(g) = 0
$$

for every $(x, x', y, y')\in E^2_1\times E^2_2$.

For $i= 1, 2$, let $w_i$ denote the morphism of Proposition 7 for the representation $\pi_i$. By Lemma 8, b) of V, p. 384 and assertion b) of Proposition 8 of V, p. 394, the image of $w_i$ is contained in the $\pi_i$-isotypical component of $\boldsymbol{\delta }_{G,\chi}$. By assertion a) of loc. cit., the image of $w_1$ is therefore orthogonal to the image of $w_2$. Consequently, one has $\langle w_1(x\otimes x')|w_2(y\otimes y')\rangle = 0$ for every $(x, x', y, y')\in E^2_1\times E^2_2$, which is the required formula.

#### Remark {#ts-v-s2-n8-rem-1 .statement tag=03B0}

The orthogonality relations of Props. 8 and 9 generalize those of A, VIII, p. 399 (see also the case where G is compact in § 2 of V, p. 457).

### 9. Subrepresentations of the regular representation of a commutative group

In this number, G is a locally compact commutative group and $\mu$ a Haar measure on G. We denote by $\widehat{G}$ the dual group of G (Definition 2 of II, p. 201) and by $\widehat{\mu}$ the dual Haar measure of $\mu$ on $\widehat{G}$ (Definition 4 of II, p. 214). The notions of measurability will always be relative to $\mu$ and $\widehat{\mu}$.

We propose to determine all the subrepresentations of the left regular representation $\boldsymbol{\gamma }_G$ of G in $L^2(G, \mu)$. Since G is commutative, one has moreover $\boldsymbol{\delta }_G(g) =\boldsymbol{\gamma }_G(g^{-1})$, so that these subrepresentations are also the subrepresentations of the right regular representation.

For every measurable subset M of $\widehat{G}$, we denote by $E_M$ the set of the $f\in L^2(G, \mu)$ such that the Fourier transform $\mathscr{F}_G(f)$ is zero almost everywhere on M (cf. No.$^o3$ of II, p. 210). It is the kernel of the continuous linear mapping $f\mapsto \varphi_M\mathscr{F}_G(f)$ of $L^2(G, \mu)$ into $L^2(\widehat{G},\widehat{\mu})$, where $\varphi_M$ denotes the characteristic function of M (cf. Theorem 1 of II, p. 215), and is therefore a closed subspace of $L^2(G, \mu)$.

We say that measurable subsets M and N of $\widehat{G}$ are equal up to a locally negligible set if $(M\cup N)$- $(M\cap N)$ is locally negligible. Equivalently, measurable subsets M and N are equal up to a locally negligible set if and only if the characteristic functions of M and N are equal in $L^{\infty}(\widehat{G},\widehat{\mu})$.

#### Proposition 10 {#ts-v-s2-prop-10 .statement tag=03B1}

a) Let M be a measurable subset of $\widehat{G}$. The space $E_M$ is a subrepresentation of the representation $\boldsymbol{\gamma }_G$;

b) Let M and N be measurable subsets of $\widehat{G}$. One has $E_M= E_N$ if and only if M and N are equal up to a locally negligible set;

c) Every subrepresentation of $\boldsymbol{\gamma }_G$ is of the form $E_M$ for a measurable subset M of $\widehat{G}$.

Let $\eta$ be the canonical mapping of G into $\widehat{\widehat{G}} ($cf. II, p. 216, Remark 1). Since $E_M$ is closed, assertion a) follows from the formulae

$$
\boldsymbol{\gamma }_G(x)(f) =\varepsilon_x*f,\mathscr{F}_G(\varepsilon_x*f) =\eta (x)\mathscr{F}_G(f)
$$

for $x\in G$ and $f\in L^2(G, \mu)$.

Let M and N be measurable subsets equal up to a locally negligible set. Since $\varphi_M$ is then equal to $\varphi_N$ in $L^{\infty}(\widehat{G},\widehat{\mu})$, this condition implies that $E_M= E_N$.

Suppose conversely that M and N are not equal up to a locally negligible set. Possibly interchanging the roles of M and N, there then exists a compact subset K such that the set $L = K\cap (M$ - $(M\cap N))$ is not negligible. Let $\varphi_L\in L^2(\widehat{G},\widehat{\mu})$ be the class of the characteristic function of L, and put $f=\overline{\mathscr{F}}_{\widehat{G}}(\varphi_L)\in L^2(G, \mu)$; one has $\mathscr{F}_G(f) =\varphi_L$ (Corollary to Theorem 2 of II, p. 220). Then $f$ belongs to $E_N$, since $L\cap N$ is empty, but not to $E_M$, since $\varphi_M\mathscr{F}(f) =\varphi_M\varphi_L=\varphi_L$. Hence $E_M\not = E_N$, which proves b).

Let now E be a subrepresentation of $\boldsymbol{\gamma }_G$. Let $p_E$ be the orthogonal projector of $L^2(G, \mu)$ with image E and let $q_E=\mathscr{F}_G\circ p_E\circ \mathscr{F}_G^{-1}$. The projector $p_E$ belong to Hom$_G(\boldsymbol{\gamma }_G,\boldsymbol{\gamma }_G)$ (prop. 4 of V, p. 383), hence it commutes with $\boldsymbol{\gamma }_G(f)$ for every $f\in L^1(G, \mu) ($cf. V, p. 401). This means that it commutes with the endomorphisms $\varphi \mapsto f*\varphi$ for $f\in L^1(G, \mu)$ (lemma 4 of V, p. 407). Consequently, the endomorphism $q_E$ of $L^2(\widehat{G},\widehat{\mu})$ commutes with the multiplication endomorphism by $g$ for every function $g\in \mathscr{C}_0(\widehat{G})$ belonging to the image of the Fourier transform of $L^1(G, \mu)$ in $\mathscr{C}_0(\widehat{G})$ (prop. 14 of II, p. 223). Since the image of the Fourier transform is dense in $\mathscr{C}_0(\widehat{G})$ (corollary of prop. 5 of II, p. 209), the continuity of the morphism $g\mapsto m_g$ implies that $q_E$ commutes with $m_g$ for every function $g\in \mathscr{C}_0(\widehat{G})$.

By the corollary of proposition 7 of IV, p. 188, there therefore exists a function $\varphi \in \mathscr{L}^{\infty}(\widehat{G},\widehat{\mu})$ such that $q_E=m_{\varphi}$. Since $q_E=q^2_E$, we have $m_{\varphi}=m^2_{\varphi}=m_{\varphi^2}$, whence $\varphi =\varphi^2$ in $L^{\infty}(\widehat{G},\widehat{\mu})$ (prop. 5 of IV, p. 186); this means that $\varphi$ is equal in $L^{\infty}(\widehat{G},\widehat{\mu})$ to the class of the characteristic function of a measurable subset N of $\widehat{G}$. Put $M =\widehat{G}-$ N. Let $f\in L^2(G, \mu)$. We have $f\in E$ if and only if $p_E(f) =f$, if and only if $\varphi \mathscr{F}_G(f) =\mathscr{F}_G(f)$, which is equivalent to $f\in E_M$.

#### Remark {#ts-v-s2-n9-rem-1 .statement tag=03B2}

Let $\chi$ be a character of G. If G is not compact, the $\chi$-isotypical component of the regular representation of G in $L^2(G)$ is trivial. If G is compact, the $\chi$-isotypical component of the regular representation of G is of dimension 1 and the function $\chi \in L^2(G)$ is a basis of it.

### 10. Unitary representations of the group R

In this number, E denotes a complex Hilbert space. The group $\mathbf{R}$ is endowed with Lebesgue measure.

#### Lemma 11 {#ts-v-s2-lem-11 .statement tag=03B3}

Let $u$ be a self-adjoint partial operator on E. For $t\in \mathbf{R}$, put $\varrho (t) =e^{itu}\in \mathscr{L}(E)$. Then the mapping $\varrho$ is a unitary representation of $\mathbf{R}$.

The operator $\varrho (t)$ is defined by the universally measurable functional calculus (def. 5 of IV, p. 272); it is an endomorphism of E since the function $x\mapsto e^{itx}$ is bounded on Sp($u$) (prop. 5, a) of IV, p. 275).

By Prop. 5 of IV, p. 275, we have $\varrho (0) = 1_E,\varrho (t)^*=\varrho (-t)$ for every $t\in \mathbf{R}$ and $\varrho (t_1+t_2) =\varrho (t_1)\varrho (t_2)$ for all $t_1$ and $t_2$ in $\mathbf{R}$. In particular, the endomorphism $\varrho (t)$ is unitary for every $t\in \mathbf{R}$. For every $x\in E$, the mapping of $\mathbf{R}$ into E defined by $x\mapsto \varrho (t)x$ is continuous at $t= 0$ by Prop. 6 of IV, p. 276, hence $\varrho$ is a unitary representation of $\mathbf{R}$ in E (V, p. 380, Lemma 4).

#### Lemma 12 {#ts-v-s2-lem-12 .statement tag=03B4}

Let $\varrho$ be a unitary representation of $\mathbf{R}$ in E. Let D be the set of elements $x$ of E such that the mapping $\psi_x:t\mapsto \varrho (t)x$ is differentiable at 0. The mapping $u$ of D into E given by $x\mapsto i^{-1}\psi '_x(0)$ defines a symmetric partial operator on E.

Let $f\in \mathscr{D}(\mathbf{R})$ and $x\in E$. Put $y=\varrho (f)x$. For every $h\in \mathbf{R}$, we have

$$
\psi_y(h) =\varrho (h)\varrho (f)x=\varrho (f)\varrho (h)x
$$

$$
=\int_{\mathbf{R}}f(t)\varrho (t+h)x dt=\int_{\mathbf{R}}f(t-h)\psi_x(t)dt
$$

The function of $\mathbf{R}^2$ into $\mathbf{C}$ defined by $(t, h)\mapsto f(t-h)$ is indefinitely differentiable; its derivative with respect to $h$ is the function defined by $(t, h)\mapsto$ $-f'(t-h)$, which is bounded by $\|f'\|_{\infty}$. When $h= 0$, this derivative is zero for $t$ outside a compact set. Since $\|\psi_x(t)\|=\|x\|$ for every $t$, we deduce from Prop. 2 of IV, p. 197 that the function $\psi_y$ is differentiable at 0 and that its derivative is given by

$$
\psi '_y(0) =-\int_{\mathbf{R}}f'(t)\psi_x(t)dt=-\varrho (f')x
$$

Hence $y\in D$. Since the space $\mathscr{D}(\mathbf{R})$ is dense in $L^1(\mathbf{R})$ (Prop. 4 of IV, p. 202), we deduce from INT, VIII, p. 139, § 2, n$^o7$, Prop. 10 that the space D is dense in E.

Let $x_1$ and $x_2$ be in D. We compute

$$
i
$$

$\langle u(x_1)|x_2\rangle =$ lim $\langle (\varrho (h)-1_E)x_1|x_2\rangle$

$$
_{h\rightarrow 0}h
$$

$$
i
$$

= lim $\langle x_1|(\varrho (-h)-1_E)x_2\rangle =\langle x_1|u(x_2)\rangle$.

$$
_{h\rightarrow 0}h
$$

Consequently, the partial operator $u$ is symmetric.

#### Definition 5 {#ts-v-s2-def-5 .statement tag=03B5}

Let $\varrho$ be a unitary representation of $\mathbf{R}$ in E. The symmetric partial operator defined in Lemma 12 is called the infinitesimal generator of $\varrho$.

#### Theorem 1 (Stone) {#ts-v-s2-thm-1 .statement tag=03B6}

The mapping $\sigma$ which to a unitary representation $\varrho$ of $\mathbf{R}$ in E associates its infinitesimal generator $u$ defines a bijection of the set of unitary representations of $\mathbf{R}$ in E onto the set of self-adjoint partial operators on E. The reciprocal bijection $\tau$ associates to a self-adjoint partial operator the unitary representation $t\mapsto e^{itu}$.

Let us first prove some lemmas.

#### Lemma 13 {#ts-v-s2-lem-13 .statement tag=03B7}

Let $\varrho$ be a unitary representation of $\mathbf{R}$ in E and let $u$ be its infinitesimal generator.

a) The domain of $u$ is the set of $x\in E$ such that the mapping $\psi_x:t\mapsto \varrho (t)x$ is differentiable on $\mathbf{R}$;

b) For every $t\in \mathbf{R}$ and every $x\in$ dom($u$), one has $\varrho (t)x\in$ dom($u$) and $\psi '_x(t) =iu(\varrho (t)x)$;

c) The partial operator $u$ is essentially self-adjoint.

For every $x\in E$, let us denote by $\psi_x$ the mapping of $\mathbf{R}$ into E defined by $\psi_x(t) =\varrho (t)x$. For every $t\in \mathbf{R}$ and every $h\in \mathbf{R}$, one has

$$
\psi_x(t+h)-\psi_x(t) =\varrho (t)(\psi_x(h)-\psi_x(0))
$$

which proves that dom($u$) is the space of elements $x\in E$ such that $\psi_x$ is differentiable on $\mathbf{R}$ and establishes that $\psi '_x(t) =\varrho (t)\psi '_x(0) =i\varrho (t)(u(x))$ for every $t\in \mathbf{R}$.

Let $x\in$ E and $t\in \mathbf{R}$. One has $\psi_{\varrho(t)x}(s) =\psi_x(s+t)$ for every $s\in \mathbf{R}$. Consequently, one has $\varrho (t)x\in$ dom($u$) if $x\in$ dom($u$), and moreover $u(\varrho (t)x) =i^{-1}\psi '_x(t) =\varrho (t)u(x)$ by a). One then obtains assertion b).

Let us prove c). Let $x\in$ Ker($u^*-i1_E$). Let us prove that $x= 0$. Let $y\in$ dom($u$), and let $f$ be the function on $\mathbf{R}$ defined by $f(t) =\langle \psi_y(t)|x\rangle$ for $t\in \mathbf{R}$. The function $f$ is bounded since $\|\psi_y(t)\|=\|y\|$ for every $t\in \mathbf{R}$; it is differentiable in $\mathbf{R}$ and, for every $t\in \mathbf{R}$, assertion b) implies

$$
f'(t) =\langle \psi '_y(t)|x\rangle =\langle iu(\varrho (t)y)|x\rangle
$$

$$
=-i\langle \varrho (t)y|u^*(x)\rangle =-i\langle \psi_y(t)|ix\rangle =f(t)
$$

since $u^*(x) =ix$. Hence $f(t) =f(0)e^t$ for all $t\in \mathbf{R}$ (FVR, IV, p. 27). Since $f$ is bounded, the function $f$ is zero and, in particular, we have $\langle y|x\rangle =f(0) = 0$. As the space dom($u$) is dense in E, we conclude that $x= 0$. Analogously, one proves that Ker($u^*+i1_E$) is reduced to 0. By Corollary 3 of IV, p. 261, the partial operator $u$ is therefore essentially self-adjoint.

#### Lemma 14 {#ts-v-s2-lem-14 .statement tag=03B8}

Let $u$ be a self-adjoint partial operator on E and let $\varrho (t) =e^{itu}$ be the unitary representation of $\mathbf{R}$ defined by $u$. The infinitesimal generator of $\varrho$ is equal to $u$.

Let $x\in$ dom($u$). Put $\psi_x(t) =\varrho (t)x$ for all $t\in \mathbf{R}$. For every nonzero real number $h$, we have

$$
\frac{1}{h}(\psi_x(t+h)-\psi_x(t)) =(\frac{1}{h}(e^{ihu}-1_E))e^{itu}x=(\frac{1}{h}(e^{ihu}-1_E))\varrho (t)x
$$

When $h$ tends to 0, we have

1 $_{iht}$

$$
(e-1)\rightarrow it
$$

$$
h
$$

for all $t\in \mathbf{R}$. Moreover,

$$
|\frac{1}{h}(e^{iht}-1)|=|t||\frac{1}{h}\int_0^he^{its}ds|\leqslant |t|
$$

It then follows from Proposition 6 of IV, p. 276 that the function $\psi_x$ is differentiable on $\mathbf{R}$ and satisfies $\psi '_x(t) =iu(\varrho (t)x)$ for all $t\in \mathbf{R}$. Consequently, the domain of $u$ is included in the set of $x\in E$ such that $\psi_x$ is differentiable at 0 and one then has $\psi '_x(0) =iu(x)$. This means by definition that the infinitesimal generator of $\varrho$ is an extension of $u$. These two operators are therefore equal since they are symmetric and $u$ is self-adjoint (IV, p. 238, Remark 5).

#### Lemma 15 {#ts-v-s2-lem-15 .statement tag=03B9}

Let $\varrho$ be a unitary representation of $\mathbf{R}$ in E. Then the infinitesimal generator $u$ of $\varrho$ is self-adjoint and $\varrho (t) =e^{itu}$ for all $t\in \mathbf{R}$.

By Lemma 13, c), the partial operator $u$ is essentially self-adjoint. Its closure $\overline{u}$ is therefore a self-adjoint operator. Let $\pi$ denote the unitary representation of $\mathbf{R}$ defined by $\pi (t) =e^{itu}$ (Lemma 11).

For every $x\in E$, let $\psi_x$ (resp. $\widetilde{\psi}_x$) denote the mapping of $\mathbf{R}$ into E defined by $\psi_x(t) =\varrho (t)x$ (resp. by $\widetilde{\psi}_x(t) =\pi (t)x$).

By lemma 13, a) and b), the space dom($u$) is the subspace of E consisting of the elements $x\in E$ such that the mapping $\psi_x$ is differentiable on $\mathbf{R}$, and for every $x\in$ dom($u$) and every $t\in \mathbf{R}$, one has $\psi '_x(t) =iu(\psi_x(t))$. Analogously, the space dom($\overline{u}$) is the subspace of E consisting of the elements $x\in E$ such that the mapping $\widetilde{\psi}_x$ is differentiable on $\mathbf{R}$, and for every $x\in$ dom($\overline{u}$) and every $t\in \mathbf{R}$, one has $\widetilde{\psi}'_x(t) =iu(\widetilde{\psi}_x(t))$.

Let $x\in$ dom($u$)$\subset$ dom($\overline{u}$). Put $f=\psi_x-\widetilde{\psi}_x$. This is a differentiable function from $\mathbf{R}$ into E. For every $t\in \mathbf{R}$, we have

$$
f'(t) =iu(\psi_x(t))-iu(\widetilde{\psi}_x(t)) =iu(f(t))
$$

since $\psi_x(t)\in$ dom($u$) and $u\subset \overline{u}$. Put $g=\|f\|^2$; this is a differentiable mapping from $\mathbf{R}$ into $\mathbf{R}$ such that $g(0) = 0$. For $t\in \mathbf{R}$, we obtain from FVR, I, p. 28, Prop. 2

$$
g'(t) =\langle f'(t)|f(t)\rangle +\langle f(t)|f'(t)\rangle
$$

$$
=\langle iu(f(t))|f(t)\rangle +\langle f(t)|iu(f(t))\rangle = 0
$$

since $\overline{u}$ is self-adjoint. Hence $f= 0$, whence $\varrho (t)x=\pi (t)x$ for every $t\in \mathbf{R}$. The continuous endomorphisms $\varrho (t)$ and $\pi (t)$ of E coincide on dom($u$), and are therefore equal for every $t\in \mathbf{R}$. Thus one has $\pi =\varrho$; since $\overline{u}$ is the infinitesimal generator of $\pi$ (lemma. 14), one has $\overline{u}=u$, which proves that $u$ is self-adjoint.

We can now prove Theorem 1.

The mappings $\sigma$ and $\tau$ are well defined (lemma 15 and lemma 11, respectively).

Let $\varrho$ be a unitary representation of $\mathbf{R}$. Let $u$ denote its infinitesimal generator. The relation $\varrho (t) =e^{itu}$ for every $t\in \mathbf{R}$ (lemma 15) proves that $\tau \circ \sigma$ is the identity mapping.

Let $u$ be a self-adjoint partial operator on E. Lemma 14 proves that the infinitesimal generator of the unitary representation $t\mapsto e^{itu}$ is equal to $u$, hence $\sigma \circ \tau$ is the identity mapping.

Let $u$ be a self-adjoint partial operator on E and let $\varrho (t) =e^{itu}$ for $t\in \mathbf{R}$ be the unitary representation of $\mathbf{R}$ in E associated with it. Let $x\in$ dom($u$). The equation $\partial_t\varrho (t)x=iu(\varrho (t)x)$ which is then satisfied (Lemma 13, b)) is called Schrödinger's equation.

#### Corollary {#ts-v-s2-n10-cor-1 .statement tag=03BA}

Let $\varrho$ be a unitary representation of $\mathbf{R}$ in a Hilbert space E. There exist a locally compact space X, a positive measure $\mu$ on X and a continuous function $g$ on X with real values such that $\varrho$ is isomorphic to the representation $\pi$ of $\mathbf{R}$ in $L^2(X, \mu)$ defined by $\pi (t)f=e^{itg}f$ for every $t\in \mathbf{R}$ and every $f\in L^2(X, \mu)$.

Let $u$ be the self-adjoint operator on E such that $\varrho (t) =e^{itu}$ for every $t\in \mathbf{R}$ (Theorem 1). There exist a locally compact space X, a positive measure $\mu$ on X, an isometric isomorphism $\theta$ of $L^2(X, \mu)$ onto E and a continuous function $g$ on X with real values such that $u=\theta \circ m_g\circ \theta^{-1}$ (Th. 1 of IV, p. 266). The assertion follows from the formula $e^{itu}=\theta \circ e^{itm_g}\circ \theta^{-1}=\theta \circ m_{e^{itg}}\circ \theta^{-1}$ (Lemma 4 of IV, p. 269).

#### Remark {#ts-v-s2-n10-rem-1 .statement tag=03BB}

Suppose that $u$ is an endomorphism of E. The unitary representation of $\mathbf{R}$ in E defined by $\varrho (t) =e^{itu}$ then satisfies the inequality $\|\varrho (t)-1_E\|\leqslant |t| \|u\|$ for every $t\in \mathbf{R}$, and the mapping $\varrho$ of $\mathbf{R}$ into the Banach space $\mathscr{L}(E)$ is the unique solution of the linear differential equation

$$
1d\varrho
$$

$$
=u\circ \varrho
$$

$$
idt
$$

(cf. FVR, IV, p. 26, §6).

#### Example {#ts-v-s2-n10-exa-1 .statement tag=03BC}

Let $\varrho$ be the regular representation of $\mathbf{R}$ in $L^2(\mathbf{R})$. The infinitesimal generator of $\varrho$ is the closure of the differential operator with domain $\mathscr{D}(\mathbf{R})$ defined by $f\mapsto  -if'$.

## EXERCISES {#ts-v-s2-exercises}

In the exercises of this paragraph, unless otherwise stated, G denotes a locally compact topological group, endowed with a left Haar measure denoted by $\mu$.

See the [exercises for § 2](exercises/s2/).
