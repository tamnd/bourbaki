---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 4
section_title: Représentations des groupes compacts
lang: en
source: ts-iii-v-fr
book_pages: TS V.456-TS V.482, TS V.504-TS V.516
pdf_pages: 0469-0495, 0517-0529
extraction: native
subsections:
    - "no": 1
      title: Semi-simplicité des représentations de dimension finie
      page: 456
      pdf_page: 469
    - "no": 2
      title: Représentations irréductibles
      page: 457
      pdf_page: 470
    - "no": 3
      title: Le théorème de Peter–Weyl
      page: 462
      pdf_page: 475
    - "no": 4
      title: Coefficients matriciels et fonctions G-finies
      page: 464
      pdf_page: 477
    - "no": 5
      title: Représentations dans un espace séparé quasi-complet
      page: 464
      pdf_page: 477
    - "no": 6
      title: Caractères et classes de conjugaison
      page: 466
      pdf_page: 479
    - "no": 7
      title: La cotransformation de Fourier
      page: 470
      pdf_page: 483
    - "no": 8
      title: La transformation de Fourier
      page: 471
      pdf_page: 484
    - "no": 9
      title: Indicateur de Frobenius–Schur et alternative de Larsen
      page: 476
      pdf_page: 489
statements: 54
exercises: 32
content_sha256: 8b79212d5331d4bf78f506367fe72d2eeb57e31b3c25f268beebd4529fb3ad94
translated_from: content/fr/ts/V/04_s4_representations_des_groupes_compacts.md
source_lang: fr
translation_method: machine
source_content_sha256: a9ee1fff2b40271b3fe60868449572c80e2eec184c5df20afc5227cb6df4fb0b
translation_model: gpt-5.4
translation_run: translate-en-mt-233681f5
glossary_version: 34
glossary_terms_sha256: 68f0cf23c8013b524786fd4f94c11357606f22540f466f2f4cf9038fbce9d839
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. REPRESENTATIONS OF COMPACT GROUPS

In this paragraph, all topological vector spaces considered are complex, unless the contrary is explicitly stated.

Let G be a compact topological group, whose identity element is denoted by $e$. The group G is unimodular (INT, VII, p. 20, § 1, n$^o3$, cor. of prop. 3). Let $\mu$ denote the normalized Haar measure on G (that is to say such that $\mu(G) = 1$), and for $1\leqslant p\leqslant +\infty$, let $\mathscr{L}^p(G)$ (resp. $L^p(G)$) denote the space $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (resp. the space $L^p_{\mathbf{C}}(G, \mu)$). Convolutions will always be considered relative to the measure $\mu$. Let $p\in [1,+\infty ]$. We identify $\mathscr{C}(G)$ with a subspace of $L^p$(G), which is permissible since the support of $\mu$ is equal to G.

For every irreducible unitary representation $\pi \in \widehat{G}$, let $E_{\pi}$ denote the space of $\pi$.

### 1. Semisimplicity of finite-dimensional representations

We recall (INT, VII, p. 71, § 3, n$^o1$, lemma 1) that for every continuous representation $\varrho$ of G in a Hilbert space E, there exists a nondegenerate positive hermitian form $q$ on E such that the topological vector space structure of E defined by $q$ is identical with the initial structure of E, and such that $\varrho$ is a unitary representation of G in the Hilbert space E endowed with the scalar product $q$.

#### Proposition 1 {#ts-v-s4-prop-1 .statement tag=03DN}

Let $\varrho$ be a finite-dimensional linear representation of G in a separated topological vector space E. There exists a scalar product $q$ on E such that $\varrho$ is a unitary representation in the Hilbert space E endowed with $q$. In particular, $\varrho$ is semisimple.

Since E is finite-dimensional, there exists a Hilbert space structure on E. The result follows by applying the preceding remark and corollary 2 of V, p. 392.

#### Remark {#ts-v-s4-n1-rem-1 .statement tag=03DO}

We shall see later (cor. 4 of V, p. 466) that every unitary representation of G is semisimple.

#### Corollary {#ts-v-s4-n1-cor-1 .statement tag=03DP}

Let $\varrho_1$ and $\varrho_2$ be finite-dimensional representations of G. The representations $\varrho_1$ and $\varrho_2$ are isomorphic if and only if their characters are equal.

This follows from the proposition and corollary 3 of V, p. 392.

### 2. Irreducible representations

#### Lemma 1 {#ts-v-s4-lem-1 .statement tag=03DQ}

Every irreducible unitary representation of G is square-integrable.

In fact, the matrix coefficients of an irreducible unitary representation are continuous and bounded, and are therefore square-integrable on G, since G is compact.

#### Proposition 2 {#ts-v-s4-prop-2 .statement tag=03DR}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. The dimension of E is finite and equal to the formal degree of $\pi$.

Since the representation $\pi$ is square-integrable (lemma 1), its formal degree $c_\mu(\pi )$ relative to $\mu$ is defined (def. 4 of V, p. 423); it is a strictly positive real number. Let $(e_i)_{i\in I}$ be a finite orthonormal family in E. Let $x$ be an element of E of norm 1 (there exists one since E is nonzero). For $i\in I$, one has

$$
c_\mu(\pi )\int_G|\langle e_i|\pi (g)x\rangle |^2d\mu(g) = 1
$$

(prop. 8 of V, p. 424). Let us sum this formula over $i\in I$. We obtain

Card(I) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
\leqslant c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

by Bessel's inequality (EVT, V, p. 21, prop. 4). Hence the cardinal of I is bounded above by $c_\mu(\pi )$. This implies that the dimension of E is finite.

One may then apply the foregoing to an orthonormal basis $(e_i)_{i\in I}$ of E. One obtains, by EVT, V, p. 22, prop. 5,

dim(E) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
=c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

which completes the proof.

In particular, it is therefore permissible to speak of the character $\chi_{\pi}$ of an irreducible unitary representation $\pi$ of G. It is a continuous function on G.

#### Corollary 1 {#ts-v-s4-prop-2-cor-1 .statement tag=03DS}

Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. The character of $\pi$ is a hermitian element of the involutive algebra $L^1(G)$.

Let $x\in G$. Since G is unimodular, one has $\chi^*_{\pi}(x) =$ Tr($\pi (x^{-1})$), whence $\chi^*_{\pi}(x) =$ Tr($\pi (x)$) since $\pi$ is a unitary representation.

#### Corollary 2 {#ts-v-s4-prop-2-cor-2 .statement tag=03DT}

a) Let $\pi$ be an irreducible unitary representation of G in a Hilbert space E. One has

$\int'$ 1 $''$

$$
\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y\rangle d\mu(g) =\langle x|y\rangle  \langle x|y\rangle
$$

$_G$ dim(E)

for every $(x, y, x', y')\in E^4$;

b) Let $\pi_1($resp. $\pi_2)$ be an irreducible unitary representation of G in a Hilbert space $E_1($resp. $E_2)$. If $\pi_1$ and $\pi_2$ are not isomorphic, one has

$$
\int_G\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\mu(g) = 0
$$

for every $(x, x', y, y')\in E^2_1\times E^2_2$.

This follows at once from Prop. 8 of V, p. 424 and Prop. 9 of V, p. 424, taking into account Lemma 1 and the formula $c_\mu(\pi ) =$ dim(E) (Prop. 2).

#### Corollary 3 {#ts-v-s4-prop-2-cor-3 .statement tag=03DU}

Let $\pi_1$ and $\pi_2$ be irreducible representations of G. In the Hilbert space $L^2(G)$, one has $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 1$ if $\pi_1$ and $\pi_2$ are isomorphic and $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 0$ otherwise. In other words, the family of the characters of the classes $\pi \in \widehat{G}$ is an orthonormal family in $L^2(G)$.

This results from Proposition 1 of V, p. 457 and Corollary 2, noting that for every orthonormal basis $(e_i)_{i\in I}$ of the space of a finite-dimensional unitary representation $\pi$ of G, and for every $g\in G$, one has the formula

$$
\chi_{\pi}(g) =\sum_{i\in I}\langle e_i|\pi (g)e_i\rangle
$$

#### Corollary 4 {#ts-v-s4-prop-2-cor-4 .statement tag=03DV}

a) Let $\varrho$ be a finite-dimensional continuous representation of G. One has

$\chi_{\varrho}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho )$)$\chi_{\pi}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\varrho , \pi )$)$\chi_{\pi}$.

b) Let $\varrho_1$ and $\varrho_2$ be finite-dimensional continuous representations of G. One has

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =$ dim(Hom$_G(\varrho_1, \varrho_2)$) $=$ dim(Hom$_G(\varrho_2, \varrho_1)$).

c) A finite-dimensional continuous representation $\varrho$ of G is irreducible if and only if $\|\chi_{\varrho}\|^2= 1$.

Since $\varrho$ is semisimple, it is isomorphic to the direct sum of its $\pi$-isotypic components $M_{\pi}(\varrho )$ for $\pi \in \widehat{G}$. Denoting by $m_{\pi}(\varrho )$ the multiplicity of $\pi$ in $\varrho$ (Def. 10 of V, p. 398), one then has

$$
\chi_{\varrho}=\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho )\chi_{\pi}
$$

Assertion a) therefore results from the fact that

$m_{\pi}(\varrho ) =$ dim Hom$_G(\pi , \varrho ) =$ dim Hom$_G(\varrho , \pi )$

(formula (1) of V, p. 377 and Corollary 2 of V, p. 387).

By bilinearity and orthonormality of the characters, assertion a) implies that

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho_1)$) dim(Hom$_G(\pi , \varrho_2)$), and on the other hand one has canonical isomorphisms

Hom$_G(\varrho_1, \varrho_2)\rightarrow \bigoplus_{(\pi_1,\pi_2)\in\widehat{G}\times\widehat{G}}$ Hom$_G(M_{\pi_1}(\varrho_1),M_{\pi_2}(\varrho_2))$

$\rightarrow \bigoplus_{\pi\in\widehat{G}}$ Hom$_G(M_{\pi}(\varrho_1),M_{\pi}(\varrho_2))$

(formula (1) of V, p. 377), whence it follows that

dim(Hom$_G(\varrho_1, \varrho_2)$) $=\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho_1)m_{\pi}(\varrho_2)$,

whence assertion b). Assertion c) also results from a) and Schur’s Lemma (prop. 6 of V, p. 386).

#### Corollary 5 {#ts-v-s4-prop-2-cor-5 .statement tag=03DW}

Let $\pi_1$ and $\pi_2$ be irreducible unitary representations of G. One has $\pi_1(\overline{\chi}_{\pi_2}) = 0$ if $\pi_1$ is not isomorphic to $\pi_2$, and $\pi_1(\overline{\chi}_{\pi_1})$ is multiplication by $1/$ dim($\pi_1$).

The character of $\pi_2$ is a continuous central function on G, hence the linear mapping $u$ = $\pi_1(\overline{\chi}_{\pi_2})$ is defined and belongs to the space Hom$_G(\pi_1, \pi_1)$. It is a homothety by Schur’s Lemma (prop. 6 of V, p. 386), whose trace is

Tr($u$) $=$ Tr$(\int_G\overline{\chi_{\pi_2}(g)}\pi_1(g)d\mu(g))$

$$
=\int_G\overline{\chi_{\pi_2}(g)}\chi_{\pi_1}(g)d\mu(g)
$$

By the orthogonality relations, the trace of $u$ is therefore zero if $\pi_1$ is not isomorphic to $\pi_2$, and equal to 1 otherwise. The assertion follows.

#### Remark {#ts-v-s4-n2-rem-1 .statement tag=03DX}

When G is finite, Schur’s orthogonality relation (resp. the orthogonality formula for characters) coincides with that of A, VIII, p. 399 (resp. that of A, VIII, p. 400, prop. 4). On the other hand, the “second orthogonality relation” for the characters of finite groups (A, VIII, p. 402, formula (32)) has no exact analogue when G is compact.

For finite G, the particular case of the second orthogonality formula corresponding to the conjugacy class of $e$ is the formula

Card G1 $\sum_{\pi\in\widehat{G}}$ dim($\pi$ )$\chi_{\pi}(g) =$ 10 sisinon$g=,e$ which is also interpreted as the calculus of the character of the regular representation $\boldsymbol{\gamma }_G$ of G, and which is equivalent to the formula Tr($\boldsymbol{\gamma }_G(f)$) $=f(e)$ for every function $f$ from G into $\mathbf{C}$.

Let G again be any compact group. For every function $f\in \mathscr{C}$(G), the endomorphism $\boldsymbol{\gamma }_G(f)$ of $L^2(G)$ coincides with the endomorphism $\varphi \mapsto f*\varphi$, and it is of finite trace (lemma 4 of V, p. 407 and corollary 2 of III, p. 33). By loc. cit. and Theorem 2 of IV, p. 177, one also has

Tr($\boldsymbol{\gamma }_G(f)$) $=\int_Gf(x^{-1}x)d\mu(x) =f(e)$.

#### Proposition 3 {#ts-v-s4-prop-3 .statement tag=03DY}

Suppose that $G = G_1\times G_2$ where $G_1$ and $G_2$ are compact groups. The mapping $b$ from $\widehat{G}_1\times \widehat{G}_2$ into $\widehat{G}$ which to $(\pi_1, \pi_2)$ associates the class of $\pi_1\boxtimes \pi_2$ is a bijection.

By cor. 6 of V, p. 389, the mapping $b$ is well defined.

Let $\pi_1$ and $\pi_2$ be elements of $\widehat{G}$. Let $\pi \in \widehat{G}$. The $\pi$-isotypical component of the restriction $\varpi$ of $\pi_1\boxtimes \pi_2$ to $G_1\times  \{e\}$ is equal to $\varpi$ if $\pi_1=\pi$ and is zero in the contrary case (lemma 8 of V, p. 384). Thus, the unitary representation $\pi_1\boxtimes \pi_2$ determines $\pi_1$ up to isomorphism; analogously, it determines $\pi_2$, which proves that $b$ is injective.

Let us prove that $b$ is surjective. Let $\pi$ be an irreducible unitary representation of $G_1\times G_2$ in a Hilbert space E. It is finite-dimensional (prop. 2). Let $\pi_1$ be an irreducible unitary representation of $G_1$ in a Hilbert space $E_1$ such that the restriction of $\pi$ to $G_1\times  \{e\}$ contains a subrepresentation isomorphic to $\pi_1$ (lemma 3 of V, p. 379). Let F = Hom$_{G_1}(\pi_1, \pi )$. It is a nonzero finite-dimensional vector space. For $h\in G_2$ and $u\in F$, let $\varrho (h)(u)$ be the linear mapping from $E_1$ into E defined by $x\mapsto \pi (e, h)(u(x))$. Since $G_1\times  \{e\}$ and $\{e\} \times G_2$ commute in G, the mapping $\varrho (h)(u)$ belongs to the space F. The mapping $\varrho$ is a linear representation of $G_2$ in the space F; it is continuous. Since F is not reduced to 0, there exists an irreducible subrepresentation $\pi_2$ of $\varrho$ (lemma 3 of V, p. 379). Let $E_2$ be the space of $\pi_2$. The linear mapping $v: E_1\otimes E_2\rightarrow E$ such that $x\otimes u\mapsto u(x)$ for $x\in E_1$ and $u\in E_2$ is then a nonzero G-morphism of $\pi_1\boxtimes \pi_2$ into $\pi$; since the representations $\pi$ and $\pi_1\boxtimes \pi_2$ are irreducible and finite-dimensional, the morphism $v$ is an isomorphism (lemma 2 of V, p. 378).

This proposition is to be compared with theorem 1 of A, VIII, p. 208.

### 3. The Peter–Weyl theorem

Recall that Θ(G) denotes the space of matrix coefficients of the finite-dimensional unitary representations of G. The space Θ(G) is a unital subalgebra of $\mathscr{C}(G)$ stable under complex conjugation (prop. 5 of V, p. 386).

For $\pi \in \widehat{G}$, let $\boldsymbol{\varrho }_G(\pi )$ denote the subspace of $\mathscr{C}(G)$ generated by the matrix coefficients of $\pi$. We identify it with a subspace of $L^2(G)$.

The space Θ(G) coincides with the sum of the spaces $\boldsymbol{\varrho }_G(\pi )$ for $\pi \in \widehat{G}$ (in fact, every element of Θ(G) is a sum of matrix coefficients of irreducible representations of G since the finite-dimensional representations of G are semisimple by prop. 1 of V, p. 457). Moreover, this sum is direct since, by cor. 2 of V, p. 458, the spaces $\boldsymbol{\varrho }_G(\pi )$ are pairwise orthogonal.

#### Proposition 4 {#ts-v-s4-prop-4 .statement tag=03DZ}

The space Θ(G) is dense in $\mathscr{C}(G)$ and in $L^2(G)$.

The unital subalgebra Θ(G) of $\mathscr{C}(G)$ is stable under conjugation. It coincides with the subalgebra Υ(G) by prop. 2 of V, p. 457, hence it separates the points of G (cor. of theorem 4 of V, p. 454). Consequently, it is dense in $\mathscr{C}(G)$ by TG, X, p. 40, cor. 2, and, fortiori, it is dense in the space $L^2(G) ($cf. INT, IV, p. 155, §4, n$^o7$, prop. 13).

Recall that the unitary biregular representation of G is the representation $\boldsymbol{\varrho }_G$ of $G\times G$ in $L^2(G)$ such that $(g_1, g_2)\mapsto \boldsymbol{\gamma }_G(g_1)\boldsymbol{\delta }_G(g_2)$.

#### Proposition 5 {#ts-v-s4-prop-5 .statement tag=03E0}

Let $\pi \in \widehat{G}$. The space $\boldsymbol{\varrho }_G(\pi )$ is a subrepresentation of $\boldsymbol{\varrho }_G$ which is isomorphic to $\overline{\pi}\boxtimes \pi$. In particular, it is an irreducible representation of $G\times G$.

By prop. 7 of V, p. 422 (applied with $Z =\{e\}$), the space $\boldsymbol{\varrho }_G(\pi )$ is a subrepresentation of $\boldsymbol{\varrho }_G$ and the linear mapping from $\overline{E}_{\pi}\otimes E_{\pi}$ into $L^2(G)$ which associates to $x\otimes y$ the matrix coefficient $g\mapsto  \langle x|\pi (g)y\rangle$ is a $(G\times$ G)-isomorphism of $\overline{\pi}\boxtimes \pi$ onto $\boldsymbol{\varrho }_G(\pi )$. The subrepresentation $\boldsymbol{\varrho }_G(\pi )$ is therefore irreducible (prop. 3 of V, p. 461).

#### Theorem 1 (Peter–Weyl) {#ts-v-s4-thm-1 .statement tag=03E1}

Let G be a compact topological group. The biregular representation $\boldsymbol{\varrho }_G$ of G is the Hilbert sum of the subrepresentations $\boldsymbol{\varrho }_G(\pi )$ for $\pi \in \widehat{G}$.

The spaces $\boldsymbol{\varrho }_G(\pi )$ are pairwise orthogonal; they are irreducible subrepresentations of the biregular representation of G (prop. 5) which are pairwise non-isomorphic (prop. 3 of V, p. 461). The theorem then results from the fact that the sum Θ(G) of the spaces $\boldsymbol{\varrho }_G(\pi )$ for $\pi$ ranging over $\widehat{G}$ is dense in $L^2(G)$ (prop. 4).

#### Corollary 1 {#ts-v-s4-thm-1-cor-1 .statement tag=03E2}

For every $\pi \in \widehat{G}$, the subrepresentation $\boldsymbol{\varrho }_G(\pi )$ is the $(\overline{\pi}\boxtimes \pi )$-isotypical component of $\boldsymbol{\varrho }_G$.

Let F be the $(\overline{\pi}\boxtimes \pi$)-isotypical component of $\boldsymbol{\varrho }_G$. The space F contains $\boldsymbol{\varrho }_G(\pi )$ (prop. 5). Moreover, for every $\tau \in \widehat{G}$ different from $\pi$, the intersection of F and $\boldsymbol{\varrho }_G(\tau )$ is zero (prop. 3 of V, p. 461). It follows that $F =\boldsymbol{\varrho }_G(\pi )$ by applying the theorem.

#### Corollary 2 {#ts-v-s4-thm-1-cor-2 .statement tag=03E3}

Let $\pi_1$ and $\pi_2$ be non-isomorphic irreducible representations of G. The $(\overline{\pi}_1\boxtimes \pi_2)$-isotypical component of $\boldsymbol{\varrho }_G$ is zero.

#### Corollary 3 {#ts-v-s4-thm-1-cor-3 .statement tag=03E4}

The right (resp. left) regular representation of G is isomorphic to the Hilbert sum

$\pi \bigoplus\in \widehat{G}\pi$dim($\pi$ ).

By the theorem and proposition 5, the restriction of the biregular representation of G to the subgroup $H =\{e\} \times G$ is isomorphic to the Hilbert sum of the restrictions to H of the representations $\overline{\pi}\boxtimes \pi$ for $\pi \in \widehat{G}$. These are isomorphic to the direct sum of dim($\pi$ ) copies of $\pi$ (lemma 8 of V, p. 384). This implies the result for the right regular representation, and the case of the left regular representation is similar.

#### Corollary 4 {#ts-v-s4-thm-1-cor-4 .statement tag=03E5}

Let $\pi \in \widehat{G}$. The $\pi$-isotypical component of $\boldsymbol{\delta }_G$ (resp. the $\overline{\pi}$-isotypical component of $\boldsymbol{\gamma }_G$) is equal to $\boldsymbol{\varrho }_G(\pi )$.

The argument is similar to that of the preceding corollary, considering $\boldsymbol{\varrho }_G(\pi )$ as a subrepresentation of $\boldsymbol{\delta }_G$ (resp. of $\boldsymbol{\gamma }_G$).

#### Remark 1 {#ts-v-s4-n3-rem-1 .statement tag=03E6}

If G is finite, these statements correspond to the results of A, VIII, p. 398, remark.

#### Remark 2 {#ts-v-s4-n3-rem-2 .statement tag=03E7}

Suppose that G is commutative. The set $\widehat{G}$ is identified with the dual group of G (V, p. 393, remark). For every $\chi \in \widehat{G}$, the space of $\boldsymbol{\varrho }_G(\chi )$ is the 1-dimensional subspace of $L^2(G)$ generated by $\chi$. Theorem 1 for G is therefore then equivalent to the corollary of theorem 1 of II, p. 215.

#### Remark 3 {#ts-v-s4-n3-rem-3 .statement tag=03E8}

If there exists an integer $n\geqslant 0$ such that G is a compact subgroup of $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$, the identical representation of G in $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$ suffices to separate the points of G, and one can therefore then prove proposition 4 directly, and then the Peter–Weyl theorem, without appealing to the Gelfand–Raikov theorem.

#### Remark 4 {#ts-v-s4-n3-rem-4 .statement tag=03E9}

The Peter–Weyl theorem implies in particular that the natural continuous homomorphism of G into $\prod_{\pi\in\widehat{G}}\mathbf{U}(E_{\pi})$ is injective.

### 4. Matrix coefficients and G-finite functions

#### Proposition 6 {#ts-v-s4-prop-6 .statement tag=03EA}

The following subspaces of $L^2(G)$ are equal:

a) The space Θ(G) ;

b) The algebraic direct sum of the subspaces $\boldsymbol{\varrho }_G(\pi )$ of $L^2(G)$;

c) The space of G-finite vectors (cf. V, p. 376) of $\boldsymbol{\gamma }_G$;

d) The space of G-finite vectors of $\boldsymbol{\delta }_G$;

e) The space of $(G\times G)$-finite vectors of $\boldsymbol{\varrho }_G$.

In particular, every G-finite vector of $\boldsymbol{\gamma }_G,\boldsymbol{\delta }_G$ or $\boldsymbol{\varrho }_G$ belongs to $\mathscr{C}(G)$.

Let us denote by $F_a$ (resp. $F_b, F_c, F_d, F_e$) the space defined by condition a) (resp. b), c), d), e)). We have already observed that $F_a= F_b$.

We have $F_b\subset F_c$ because $\boldsymbol{\varrho }_G(\pi )$ is a finite-dimensional subrepresentation of $\boldsymbol{\gamma }_G$ for every $\pi \in \widehat{G}$. Conversely, let $f$ be a G-finite vector of $\boldsymbol{\gamma }_G$. The subspace $E_f$ generated by the functions $\boldsymbol{\gamma }_G(g)f$ for $g\in G$ is a finite-dimensional subrepresentation of $\boldsymbol{\gamma }_G$. It is equal to the direct sum of its $\pi$-isotypic components for $\pi \in \widehat{G}$ (Prop. 1 of V, p. 457). By Cor. 4 of V, p. 463, this implies that $E_f$ is contained in the sum of the spaces $\boldsymbol{\varrho }_G(\pi )$, hence $F_c\subset F_b$.

By analogous reasoning, one obtains $F_b= F_d$, and since $\boldsymbol{\varrho }_G(\pi )$ is a subrepresentation of $\boldsymbol{\varrho }_G$, one establishes in the same way that $F_b= F_e$.

#### Corollary {#ts-v-s4-n4-cor-1 .statement tag=03EB}

Let $E\subset L^2(G)$ be a finite-dimensional vector subspace defining a subrepresentation of $\boldsymbol{\gamma }_G($resp. of $\boldsymbol{\delta }_G$, of $\boldsymbol{\varrho }_G)$. Then E is contained in $\mathscr{C}(G)$.

In fact, every element of E is a G-finite vector of the representation $\boldsymbol{\gamma }_G$.

### 5. Representations in a separated quasi-complete space

#### Proposition 7 {#ts-v-s4-prop-7 .statement tag=03EC}

Let $\varrho$ be a continuous representation of G in a separated locally convex quasi-complete space E. The sum of the finite-dimensional subrepresentations of E is dense in E.

Let $x\in E$ and let U be an open neighbourhood of $x$. The set of measures $\nu \in \mathscr{M}(G)$ such that $\varrho (\nu )x\in U$ is open in $\mathscr{M}(G)$ for the topology of compact convergence (cf. n$^o2$ of V, p. 400). It contains $\varepsilon_e$, hence it contains a measure of the form $\nu =f_1\cdot \mu$ where $f_1\in \mathscr{C}(G)$ (INT, VIII, p. 171, § 4, n$^o7$, Prop. 19) and, consequently, it contains a measure of the form $f_2\cdot \mu$ where $f_2$ is a G-finite function (Prop. 6 of V, p. 464 and Prop. 4 of V, p. 462).

The subrepresentation F of $\boldsymbol{\gamma }_G$ generated by $f_2$ is finite-dimensional. Let $\widetilde{F}$ be the image of the linear mapping $f\mapsto \varrho (f)x$ of F into E. The space $\widetilde{F}$ is finite-dimensional, and it contains the element $\varrho (f_2)x$ of U. Since $\varrho (g)\varrho (f) =\varrho (\boldsymbol{\gamma }_G(g)f)$ for every $g\in G$ and every $f\in F$ (formula (1) of V, p. 406), the space $\widetilde{F}$ is a subrepresentation of $\varrho$ which meets U. The proposition is proved.

#### Corollary 1 {#ts-v-s4-prop-7-cor-1 .statement tag=03ED}

Let $\pi$ be an irreducible continuous representation of G in a separated quasi-complete locally convex space E. The space E is finite-dimensional.

#### Corollary 2 {#ts-v-s4-prop-7-cor-2 .statement tag=03EE}

Let $\varrho$ be a continuous representation of G in a separated quasi-complete locally convex space E and let $\pi$ be an irreducible continuous representation of G.

a) The G-morphism $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ of E into E is a continuous projector of E whose image is the $\pi$-isotypical component of $\varrho$;

b) If $\varrho$ is a unitary representation, then the projector $p_{\pi}$ is the orthoprojector of E with image $M_{\pi}(\varrho )$.

Let us prove a). The linear mapping $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ is well-defined, since E is quasi-complete and G is compact (V, p. 401). It is an element of Hom$_G(\varrho , \varrho )$ since the character of $\pi$ is a continuous central function on G.

Let $\varpi$ be a finite-dimensional subrepresentation of E and F its space. The mapping $p_{\pi}$ induces, by passing to subspaces, the endomorphism (dim $\pi$ )$\varpi (\overline{\chi}_{\pi})$ of F. This endomorphism is therefore zero if $\varpi$ is not isomorphic to $\pi$, and is the identity mapping of F otherwise (in fact, this is the case if $\varpi$ is irreducible by Cor. 5 of V, p. 460, and the general case follows from this since $\varpi$ is semisimple by Prop. 1 of V, p. 457).

Finally, since the sum of the finite-dimensional subrepresentations of E is dense in E (Prop. 7) and $p_{\pi}$ is continuous, it follows that $p_{\pi}$ is a projector whose image is the $\pi$-isotypical component of $\varrho$. If E is Hilbert space, the projector $p_{\pi}$ is hermitian by Cor. 1 of V, p. 458, hence it is an orthoprojector (Lemma 3, (ii) of I, p. 133).

#### Corollary 3 {#ts-v-s4-prop-7-cor-3 .statement tag=03EF}

Let $\varrho$ be a continuous representation of G in a separated quasi-complete locally convex space E. The endomorphism

$$
x\mapsto \int_G\varrho (g)x d\mu(g)
$$

of E is a projector of E whose image is the space $E^G$ of invariant vectors in E. In particular, if E is finite-dimensional, then

dim(E$^G$) $=\int_G\chi_{\varrho}(g)d\mu(g)$.

The first assertion is the particular case of the preceding corollary when $\pi$ is the trivial representation of dimension 1 of G. The second follows from it since the dimension of $E^G$ is the trace of the orthoprojector onto $E^G$, that is,

dim(E$^G$) $=$ Tr$(\int_G\varrho (g)d\mu(g))=\int_G\chi_{\varrho}(g)d\mu(g)$.

In particular, when E is finite-dimensional, there exists a vector $x\not = 0$ in E such that $\varrho (g)x=x$ for every $g\in G$ if and only if

$$
\int_G\chi_{\varrho}(g)d\mu(g)\not = 0
$$

#### Corollary 4 {#ts-v-s4-prop-7-cor-4 .statement tag=03EG}

Let $\varrho$ be a unitary representation of G in a Hilbert space E. The space E is the Hilbert sum of the $\pi$-isotypical components $M_{\pi}(\varrho )$ for $\pi \in \widehat{G}$. In particular, the representation $\varrho$ is semisimple.

The isotypical components of $\varrho$ corresponding to non-isomorphic irreducible representations of G are orthogonal (prop. 8 of V, p. 394). Since every finite-dimensional unitary representation of G is semisimple (prop. 1 of V, p. 457), the sum of the isotypical components $M_{\pi}(\varrho )$ for $\pi \in \widehat{G}$ is dense in E (prop. 7). The corollary follows.

### 6. Characters and Conjugacy Classes

Let $\varrho$ be a unitary representation of G in a finite-dimensional Hilbert space E. The character of $\varrho$ satisfies $|\chi_{\varrho}|\leqslant$ dim(E). Let $(e_i)_{i\in I}$ be an orthonormal basis of E; the character $\chi_{\varrho}$ is the sum of the diagonal matrix coefficients $g\mapsto  \langle e_i|\varrho (g)e_i\rangle$ of $\varrho$. In particular, the character of $\varrho$ is a G-finite function, and if $\varrho$ is irreducible, then $\chi_{\varrho}\in \boldsymbol{\varrho }_G(\varrho )$.

We have the following formulas

$$
\chi_{\varrho_1\oplus\varrho_2}=\chi_{\varrho_1}+\chi_{\varrho_2},\chi_{\varrho_1\otimes\varrho_2}=\chi_{\varrho_1}\chi_{\varrho_2},\chi_{\breve{\varrho}}=\chi_{\overline{\varrho}}=\overline{\chi}_{\varrho}
$$

(cf. A, VIII, p. 388–389).

#### Proposition 8 {#ts-v-s4-prop-8 .statement tag=03EH}

One has

(1) $\chi_{\pi}*\chi_{\sigma}= 0$ for all $\pi , \sigma$ belonging to $\widehat{G}, \pi \not =\sigma$,

(2) $\chi_{\pi}*\chi_{\pi}=$ dim($1\pi$ )$\chi_{\pi}$ for every $\pi$ belonging to $\widehat{G}$.

Let $\pi$ and $\sigma$ be irreducible representations of G. One has

dim($\pi$ )$(\chi_{\pi}*\chi_{\sigma}) =$ dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$

(lemma 4 of V, p. 407). The function dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$ is the orthogonal projection of $\chi_{\sigma}$ on the $\overline{\pi}$-isotypical component of $\boldsymbol{\gamma }_G$ (cor. 2 of V, p. 465), that is, on $\boldsymbol{\varrho }_G(\pi )$ (cor. 4 of V, p. 463). Since $\chi_{\sigma}$ belongs to $\boldsymbol{\varrho }_G(\sigma )$, the result follows from theorem 1 of V, p. 462.

#### Lemma 2 {#ts-v-s4-lem-2 .statement tag=03EI}

The graph of the equivalence relation “ $x\in G$ and $y\in G$ and $x$ is conjugate to $y$ ” in G is closed.

In fact, this graph is the image of the continuous mapping of the compact space $G\times G$ into itself defined by $(x, y)\mapsto (x, yxy^{-1})$.

We denote by $G^{\sharp}$ the space of conjugacy classes of G endowed with the quotient topology; it is a compact space by lemma 2 and TG, I, p. 78, prop. 8. Let $\varpi : G\rightarrow G^{\sharp}$ be the canonical projection. The mapping of $\mathscr{C}(G^{\sharp})$ into $\mathscr{C}(G)$ defined by $f\mapsto f\circ \varpi$ identifies the involutive algebra $\mathscr{C}(G^{\sharp})$ with the involutive subalgebra of $\mathscr{C}(G)$ formed by the continuous central functions.

The measures on $G^{\sharp}$ are identified with the central measures on G (V, p. 402, def. 1).

The linear form on $\mathscr{C}(G^{\sharp})$ defined by $f\mapsto \int_Gf$ is then a positive measure of mass 1 on $G^{\sharp}$, denoted by $\mu^{\sharp}$. For every $p\in [1,+\infty ]$, we denote by $\mathscr{L}^p(G^{\sharp})$ (resp. $L^p(G^{\sharp})$) the space $\mathscr{L}_{\mathbf{C}}^p(G^{\sharp}, \mu^{\sharp})$ (resp. $L^p_{\mathbf{C}}(G^{\sharp}, \mu^{\sharp})$). We identify $L^p(G^{\sharp})$ with the closure of $\mathscr{C}(G^{\sharp})$ in $L^p(G)$; in particular, it is a closed subspace of $L^p(G)$.

We also denote by $\Theta (G^{\sharp}) = \Theta (G)\cap \mathscr{C}(G^{\sharp})$ the space of central matrix coefficients of G. It is a unital involutive subalgebra of $\mathscr{C}(G^{\sharp})$.

When G is a Lie group, the space $\Theta (G^{\sharp})$ is also denoted by ZΘ(G) in LIE, IX, p. 71.

#### Lemma 3 {#ts-v-s4-lem-3 .statement tag=03EJ}

Let $\pi$ be an irreducible unitary representation of G. The vector space $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ has dimension one and is generated by the character of $\pi$.

Consider the unitary representation $\sigma$ of G in the space $\boldsymbol{\varrho }_G(\pi )$ defined by $\sigma (g) =\boldsymbol{\varrho }_G(g, g)$. Since the unitary representation $\boldsymbol{\varrho }_G(\pi )$ of $G\times G$ is isomorphic to $\overline{\pi}\boxtimes \pi$ (prop. 5 of V, p. 462), its character is given by

$$
\chi_{\sigma}(g) =\chi_{\overline{\pi}\boxtimes\pi}(g, g) =|\chi_{\pi}(g)|^2
$$

for every $g\in G$. The space $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ is the subspace of the elements invariant under this representation, and its dimension is equal to

$$
\int_G\chi_{\sigma}(g)d\mu(g) =\int_G|\chi_{\pi}(g)|^2d\mu(g) = 1
$$

(cor. 3 of V, p. 466 and cor. 3 of V, p. 459). Since the character of $\pi$ is a nonzero element of $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$, it is a basis of this space.

#### Proposition 9 {#ts-v-s4-prop-9 .statement tag=03EK}

The family $(\chi_{\pi})_{\pi\in\widehat{G}}$ of the characters of the irreducible unitary representations of G is an orthonormal basis of $L^2(G^{\sharp})$.

By the Peter-Weyl theorem (th. 1 of V, p. 462), the closed subspace $L^2(G^{\sharp})$ of $L^2(G)$ formed by the elements invariant under the unitary representation $g\mapsto \boldsymbol{\varrho }_G(g, g)$ of G is the Hilbert sum of the subspaces $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ for $\pi \in \widehat{G}$. The proposition therefore follows from the preceding lemma and cor. 3 of V, p. 459.

#### Corollary 1 {#ts-v-s4-prop-9-cor-1 .statement tag=03EL}

The vector space $\Theta (G^{\sharp})$ is dense in $\mathscr{C}(G^{\sharp})$ and in $L^2(G^{\sharp})$.

The second assertion follows from prop. 9. As to the first assertion, consider the linear representation $\varrho$ of G on the Banach space $\mathscr{C}(G)$ defined by

$$
\varrho (g)f(x) =f(g^{-1}xg)
$$

for every $f\in \mathscr{C}(G)$ and every $x\in G$. It is a continuous isometric representation, and $\mathscr{C}(G^{\sharp})$ is the space of the elements invariant under this representation. The continuous projector $p=\varrho (1)$ of $\mathscr{C}(G)$ therefore has image $\mathscr{C}(G^{\sharp})$ (cor. 3 of V, p. 466); it has norm $\leqslant 1$.

Let $f\in \mathscr{C}(G^{\sharp})$ and let $\varepsilon  >0$. There exists $\widetilde{f}\in \Theta (G)$ such that $\|f-\widetilde{f}\|\leqslant \varepsilon$ (prop. 4 of V, p. 462), and then $\|f-p(\widetilde{f})\|=\|p(f-\widetilde{f})\|\leqslant \varepsilon$; since $p(\widetilde{f})\in \mathscr{C}(G^{\sharp})$, we conclude that $\Theta (G^{\sharp})$ is dense in $\mathscr{C}(G^{\sharp})$.

Let $R(G)$ denote the Grothendieck ring of continuous representations of $G$ in finite-dimensional separated complex vector spaces (cf. LIE, IX, p. 70 and A, VIII, p. 182, applied to the additive class of continuous representations of $G$ in finite-dimensional separated complex vector spaces, viewed as $\mathbf{C}$[G]-modules). Since every continuous linear representation of $G$ in a finite-dimensional separated topological vector space is semisimple (prop. 1 of V, p. 457), the abelian group $R(G)$ is free and the classes of irreducible unitary representations $\pi \in \widehat{G}$ form a basis of it (A, VIII, p. 186, prop. 7).

#### Corollary 2 {#ts-v-s4-prop-9-cor-2 .statement tag=03EM}

a) The family of characters of the irreducible representations of $G$ is a basis of $\Theta (G^{\sharp})$;

b) The mapping $u: R(G)\otimes_{\mathbf{Z}}\mathbf{C}\rightarrow \Theta (G^{\sharp})$ such that $u(\pi \otimes 1) =\chi_{\pi}$ for every $\pi \in \widehat{G}$ is an isomorphism of algebras over $\mathbf{C}$.

The first assertion results from Proposition 9 and Corollary 1.

Since the classes of the representations $\pi \in \widehat{G}$ form a basis of the free $\mathbf{Z}$-module $R(G)$, the mapping $u$ is well-defined. It is a morphism of $\mathbf{C}$-algebras, and it is an isomorphism by a).

#### Corollary 3 {#ts-v-s4-prop-9-cor-3 .statement tag=03EN}

Let $H$ be a locally compact topological group such that $G$ is a compact subgroup of $H$. Let $\varrho$ be a unitary representation of $H$ in a Hilbert space $E$. If the $\pi$-isotypical component of the restriction of $\varrho$ to $G$ is finite-dimensional for every $\pi \in \widehat{G}$, then the representation $\varrho$ of $H$ is semisimple and every irreducible unitary representation of $H$ occurs with finite multiplicity in $\varrho$.

Let us denote by $\sigma$ the restriction of $\varrho$ to the compact subgroup $G$ of $H$. Let $\pi$ be an irreducible representation of $G$. The endomorphism $\sigma (\chi_{\pi})\in \mathscr{L}(E)$ is of finite rank, since its image is the $\overline{\pi}$-isotypical component of $\sigma$ (cor. 2 of V, p. 465) and this is finite-dimensional by hypothesis. Consequently, the endomorphism $\sigma (f)$ is of finite rank for every $f\in \Theta (G^{\sharp})$ and is compact for every $f\in \mathscr{C}(G^{\sharp})$ (cor. 1 of V, p. 468 and cor. of prop. 2 of III, p. 4).

Let $j$ denote the canonical injection of $G$ into $H$. It is a continuous mapping which is $\nu$-proper for every measure $\nu$ on $G$ (INT, V, p. 69, § 6, No.$^o1$, Remark 1). Let $\mathfrak{B}$ be the filter of compact neighbourhoods of the element $e$ in $G$. For every $V\in \mathfrak{B}$, there exists a positive continuous central function $f_V$ on $G$ with support contained in $V$ whose integral over $G$ is equal to $1$. Let $\beta_V$ denote the image measure $j(f_V\cdot \mu)$; it is a positive measure with compact support on $H$ such that $\varrho (\beta_V) =\sigma (f_V)$ (INT, V, p. 71, § 6, No.$^o2$, Theorem 1). From the foregoing, the filter basis on $\mathscr{M}_c(H)$ which is the image of $\mathfrak{B}$ under the mapping $V\mapsto \beta_V$ satisfies the conditions of Proposition 2 of V, p. 402, and the assertion follows.

Corollary 4 (Weyl's criterion for equidistribution)

Let $M$ be a set of positive central measures on $G$ such that $\nu (G) = 1$ for every $\nu \in M$. Let $\mathfrak{F}$ be a filter on $M$. In order that the filter $\mathfrak{F}$ converge vaguely to the measure $\mu^{\sharp}$ on $G^{\sharp}$, it is necessary and sufficient that, for every non-trivial irreducible unitary representation $\pi$, one have

lim$_{\nu ,\mathfrak{F}}\int_G\chi_{\pi}(x)d\nu (x) = 0$.

Since $\nu (G^{\sharp}) = 1 =\mu^{\sharp}(G^{\sharp})$ for $\nu \in M$, the hypothesis means that

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}\chi_{\pi}(x)d\nu (x) =\int_{G^{\sharp}}\chi_{\pi}(x)d\mu^{\sharp}(x)$

for every representation $\pi \in \widehat{G}$, hence it is equivalent to the condition

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}f(x)d\nu (x) =\int_{G^{\sharp}}f(x)d\mu^{\sharp}(x)$

for every function $f\in \Theta (G^{\sharp})$ by linearity. Since the space $\Theta (G^{\sharp})$ is dense in $\mathscr{C}(G^{\sharp})$ (Corollary 1), the hypothesis is therefore equivalent to the convergence of the filter $\mathfrak{F}$ to $\mu^{\sharp}$ in $\mathscr{M}(G^{\sharp})$ endowed with the topology of simple convergence in $\mathscr{C}$ (G), which coincides with the topology of vague convergence since G is compact (cf. INT, III, p. 59, § 1, No.$^o9$).

### 7. The Fourier cotransform

The set $\widehat{G}$ is endowed with the discrete topology. We denote by $F(\widehat{G})$ the product algebra of the End(E$_{\pi}$) for $\pi$ belonging to $\widehat{G}$ and by $F_b(\widehat{G})$ the $*$-product algebra of the End(E$_{\pi}$) (Example 5 of I, p. 103); it is the set of families $(u_{\pi})_{\pi\in\widehat{G}}$ such that sup$_{\pi\in\widehat{G}}\|u_{\pi}\|<+\infty$.

We denote by $F_0(\widehat{G})$ the closed $*$-subalgebra of $F_b(\widehat{G})$ formed by the families $(u_{\pi})_{\pi\in\widehat{G}}$ such that $\|u_{\pi}\|$ tends to 0 at infinity.

Let $\nu \in \mathscr{M}^1(G)$. For every $\pi \in \widehat{G}$, we have $\|\pi (\nu )\|\leqslant \|\nu \|$, hence the family $(\pi (\nu ))_{\pi\in\widehat{G}}$ belongs to $F_b(\widehat{G})$.

#### Definition 1 {#ts-v-s4-def-1 .statement tag=03EO}

For every measure $\nu \in \mathscr{M}^1(G)$, the element $(\pi (\nu ))_{\pi\in\widehat{G}}$ of $F_b(\widehat{G})$ is denoted by $\mathscr{F}_G(\nu )$. The map of $\mathscr{M}^1(G)$ into $F_b(\widehat{G})$ thus defined is called the Fourier cotransform of G, and $\overline{\mathscr{F}}_G(\nu )$ is called the Fourier cotransform of the measure $\nu$.

For $f\in L^1$(G), we shall write $\overline{\mathscr{F}}_G(f) =\overline{\mathscr{F}}_G(f\cdot \mu)$.

For every representation $\pi \in \widehat{G}$, the map $\nu \mapsto \pi (\nu )$ is a unital morphism of involutive Banach algebras of $\mathscr{M}^1(G)$ into End(E$_{\pi}$) (Lemma 1 of V, p. 401). The Fourier cotransform is therefore a unital morphism of involutive Banach algebras of $\mathscr{M}^1(G)$ into $F_b(\widehat{G})$.

### 8. The Fourier transform

We retain the notation of the preceding number.

Let $\pi \in \widehat{G}$. We endow the vector space End(E$_{\pi}$) with the structure of a Hilbert space whose scalar product is given by

$\langle u_1|u_2\rangle =$ dim($\pi$)Tr($u^*_1u_2$) $=$ dim($\pi$)Tr($u_2u^*_1$)

for $u_1,u_2$ in End(E$_{\pi}$) $($cf. EVT, V, p. 52, Theorem 1).

We denote by $\|u\|_2$ = $\surd\overline{\langle u|u\rangle}$ the norm of an element $u$ of End(E$_{\pi}$) for $\pi \in \widehat{G}$. For every $g\in G$, one has $\|\pi (g)\|_2=$ dim($\pi$ ) since $\pi (g)$ is unitary.

The norm here denoted by $\|u\|_2$ differs by a factor dim($\pi$ ) from the norm defined in EVT, V, p. 52 on the space of Hilbert-Schmidt mappings of $E_{\pi}$.

#### Lemma 4 {#ts-v-s4-lem-4 .statement tag=03EP}

Let $\pi$ be an irreducible representation of G. The mapping $f\mapsto \pi (f)$ defines by passing to the subspaces an isometric isomorphism of $\boldsymbol{\varrho }_G(\overline{\pi})$ into End(E$_{\pi}$).

Put $\varepsilon_{\pi}(g, h)u=\pi (g)\circ u\circ \pi (h^{-1})$ for every $(g, h)\in G\times G$ and for every $u\in$ End(E$_{\pi}$). The mapping $\varepsilon_{\pi}$ is a continuous representation of $G\times G$ in End(E$_{\pi}$). It is unitary. In fact, since $\pi$ itself is unitary, one obtains

$\|\varepsilon_{\pi}(g, h)u\|^2_2=$ dim($\pi$ ) Tr$((\pi (g)u\pi (h^{-1}))^*\pi (g)u\pi (h^{-1}))$

= dim($\pi$ ) Tr($\pi (h)u^*u\pi (h)^{-1}$) $=$ dim($\pi$ ) Tr($u^*u$) $=\|u\|^2_2$ for every $(g, h)\in G\times G$ and every $u\in$ End(E$_{\pi}$).

The mapping Ψ defined by $f\mapsto \pi (f)$ is a $(G\times$ G)-morphism of $\boldsymbol{\varrho }_G(\overline{\pi})$ into End(E$_{\pi}$), since

$$
\pi (\boldsymbol{\varrho }_G(g, h)f) =\int_Gf(g^{-1}xh)\pi (x)d\mu(x) =\pi (g)\pi (f)\pi (h^{-1})
$$

for every $(g, h)\in G\times G$ and every $f\in \boldsymbol{\varrho }_G(\overline{\pi})$. Since $\boldsymbol{\varrho }_G(\overline{\pi})$ is an irreducible representation (th. 1, a) of V, p. 462), there exists $\lambda \in \mathbf{C}^*$ such that the mapping $\lambda \Psi$ is zero or isometric (cor. 5, a) of V, p. 388).

Let $f=$ dim($\pi$ )$\overline{\chi}_{\pi}\in \boldsymbol{\varrho }_G(\overline{\pi})$. Then $\pi (f) = 1_{E_{\pi}}$ (cor. 2 of V, p. 465), whence $\|\pi (f)\|_2=$ dim($\pi$ ) $=\|f\|$ (cor. 3 of V, p. 459). Consequently, the mapping Ψ is isometric. Since $\boldsymbol{\varrho }_G(\overline{\pi})$ and End(E$_{\pi}$) are of the same dimension, Ψ is an isometric isomorphism.

We denote by $F^2(\widehat{G})$ the Hilbert sum of the Hilbert spaces End(E$_{\pi}$). The norm of an element $x\in F^2(\widehat{G})$ is again denoted by $\|x\|_2$.

In LIE, IX, p. 79, this space is denoted $L^2(\widehat{G})$, a notation which we prefer to avoid here so as not to create confusion with the space $\ell^2(\widehat{G})$.

Let $(u_{\pi})$ be an element of $F^2(\widehat{G})$. Since

$^{\pi\in\widehat{G}}\sum_{\pi\in\widehat{G}}\|u_{\pi}\|^2_2=\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($u^*_{\pi}u_{\pi}$)$<+\infty$

and $\|u_{\pi}\|^2\leqslant$ Tr($u^*_{\pi}u_{\pi}$) $($cf. EVT, V, p. 52, formula (33)), the norm in $\mathscr{L}(E_{\pi})$ of the endomorphism $u_{\pi}$ tends to 0 at infinity. One can therefore identify $F^2(\widehat{G})$ with a subspace of $F_0(\widehat{G})$.

Let $\pi \in \widehat{G}$ and $u\in$ End(E$_{\pi}$). We denote by $\mathscr{F}_{\pi}(u)$ the function on G defined by $\mathscr{F}_{\pi}(u)(g) =\langle \pi (g)|u\rangle =$ dim($\pi$)Tr($\pi (g)^*u$) for every $g\in G$. This is a continuous function on G. If G is a compact real Lie group, then the function $\mathscr{F}_{\pi}(u)$ is analytic on G (LIE, III, § 8, n$^o1$, th. 1).

Since G is compact, one can identify $L^2(G)$ with a subspace of $L^1(G)$.

#### Theorem 2 {#ts-v-s4-thm-2 .statement tag=03EQ}

The Fourier cotransformation of G induces by passing to the subspaces an isometric isomorphism of $L^2(G)$ onto $F^2(\widehat{G})$. Its inverse $\mathscr{F}_G$ associates with an element $(u_{\pi})_{\pi\in\widehat{G}}$ of $F^2(\widehat{G})$ the sum of the series

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

which converges in $L^2(G)$.

By the Peter-Weyl theorem (th. 1 of V, p. 462), the Hilbert space $L^2(G)$ is the Hilbert sum of the spaces $\boldsymbol{\varrho }_G(\overline{\pi})$ for $\pi \in \widehat{G}$. For every $\pi \in \widehat{G}$, the linear mapping $f\mapsto \pi (f)$ of $\boldsymbol{\varrho }_G(\overline{\pi})$ into End(E$_{\pi}$) is an isometric isomorphism (lemma 4). Consequently, the restriction to $L^2(G)$ of the Fourier cotransformation defines an isometric isomorphism of $L^2(G)$ onto $F^2(\widehat{G})$.

Let $f\in L^2(G)$. Let $\pi \in \widehat{G}$, and let $f_{\overline{\pi}}\in \mathscr{C}(G)$ be the orthogonal projection of $f$ onto $\boldsymbol{\varrho }_G(\overline{\pi})$ (th. 1 of V, p. 462). Since this space is the $\overline{\pi}$-isotypical component of $\boldsymbol{\delta }_G$ (cor. 4 of V, p. 463), one has $f_{\overline{\pi}}=$ dim($\pi$ )$\boldsymbol{\delta }_G(\chi_{\pi})(f)$ by cor. 2 of V, p. 465. For every $x\in G$, this gives

$f_{\overline{\pi}}(x) =$ dim($\pi$ )$\int_G\chi_{\pi}(g)(\boldsymbol{\delta }_G(g)f)(x)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(g)f(xg)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(x^{-1}y)f(y)d\mu(y)$

= dim($\pi$)Tr($\pi (x^{-1})\pi (f)$) $=\langle \pi (x)|\pi (f)\rangle$,

that is to say $f_{\overline{\pi}}=\mathscr{F}_{\pi}(\pi (f))$.

Since $f$ is the sum in $L^2(G)$ of the family $(f_{\overline{\pi}})$ by the Peter–Weyl theorem, we obtain

$$
f=\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(\pi (f))
$$

where the series converges in $L^2(G)$. This proves the theorem.

#### Definition 2 {#ts-v-s4-def-2 .statement tag=03ER}

The isometric isomorphism $\mathscr{F}_G$ of $F^2(\widehat{G})$ onto $L^2(G)$ inverse to the isomorphism induced by the Fourier cotransform is called the Fourier transform of G. The image of an element of $F^2(\widehat{G})$ is called its Fourier transform.

#### Remark 1 {#ts-v-s4-n8-rem-1 .statement tag=03ES}

The Fourier transform of $(u_{\pi})_{\pi\in\widehat{G}}\in F^2(\widehat{G})$ is therefore the class in $L^2(G)$ of the series

$g\mapsto \sum_{\pi\in\widehat{G}}\langle \pi (g)|u_{\pi}\rangle =\sum_{\pi\in\widehat{G}}$ dim($\pi$)Tr($u_{\pi}\circ \pi (g)^{-1}$).

#### Remark 2 {#ts-v-s4-n8-rem-2 .statement tag=03ET}

Let $f\in L^2(G)$. One then has the Plancherel formula

$$
\|f\|^2=\|\overline{\mathscr{F}}_G(f)\|^2=\sum_{\pi\in\widehat{G}}\|\pi (f)\|^2
$$

Moreover, by Theorem 2$,f$ is the sum in $L^2(G)$ of the family $(f_{\pi})_{\pi\in\widehat{G}}$ where

$$
f_{\pi}(x) =\mathscr{F}_{\pi}(\pi (f))(x)
$$

$=\langle \pi (x)|\pi (f)\rangle =$ dim($\pi$ )$\int_Gf(g)\chi_{\pi}(x^{-1}g)d\mu(g)$

for every $x\in G$ and every $\pi \in \widehat{G}$.

Suppose that G is commutative. Since the irreducible representations of G are of dimension 1 (cor. 7 of V, p. 390) and the dual group $\widehat{G}$ is discrete (prop. 18 of II, p. 233), the algebras $F_b(\widehat{G})$ and $F_0(\widehat{G})$ are identified, respectively, with the algebra $\mathscr{C}_b(\widehat{G})$ of bounded continuous functions on $\widehat{G}$ and the algebra $\mathscr{C}_0(\widehat{G})$ of continuous functions tending to 0 at infinity on $\widehat{G}$. Since G is compact, the Haar measure on $\widehat{G}$ dual to $\mu$ is the counting measure $\widehat{\mu}$ (prop. 18 of II, p. 233). The Hilbert sum $F^2(\widehat{G})$ of the spaces End(E$_{\pi}$) for $\pi \in \widehat{G}$ is identified with the Hilbert space $L^2(\widehat{G},\widehat{\mu})$.

Let $\nu \in \mathscr{M}^1(G)$. Then, for every unitary character $\chi \in \widehat{G}$, one has

$$
\chi (\nu ) =\int_G\chi  \nu
$$

which proves that the Fourier cotransform defined above coincides with the Fourier cotransform of G defined in II, p. 206.

Every $f\in \mathscr{L}^2(G)$ is integrable and the formula $\|\overline{\mathscr{F}}_G(f)\|_2=\|f\|$ is the Plancherel formula (II, p. 215, Theorem 1).

#### Proposition 10 {#ts-v-s4-prop-10 .statement tag=03EU}

The Fourier cotransform is an injective morphism of involutive Banach algebras of $\mathscr{M}^1(G)$ into $F_b(\widehat{G})$ which maps $L^1(G)$ into $F_0(\widehat{G})$.

Since G is compact, the space $\mathscr{C}(G)$ is included in and dense in $\mathscr{L}^1(G)$ and $\mathscr{L}^2(G)$.

Let $\nu \in \mathscr{M}^1(G)$ be such that $\overline{\mathscr{F}}_G(\nu ) = 0$. Then for every continuous function $f$ on G, one has $\overline{\mathscr{F}}_G(\nu *f) = 0$. Now $\nu *f$ belongs to $\mathscr{C}(G)$ (INT, VIII, p. 152, § 4, No.$^o2$, prop. 3). Since, by Theorem 2, the Fourier cotransform is injective on $L^2$(G), and a fortiori on the space $\mathscr{C}$ (G), one has $\nu *f= 0$ for $f\in \mathscr{C}(G)$. In particular, it follows that

$$
\int_Gf(x)d\nu (x) = (\nu *\check{f})(e) = 0
$$

for every function $f\in \mathscr{C}(G)$ (INT, VIII, loc. cit.), hence the measure $\nu$ is zero.

The image of $\mathscr{C}(G)$ under the Fourier cotransform is contained in $F^2(\widehat{G})$, and a fortiori in $F_0(\widehat{G})$. Since $F_0(\widehat{G})$ is closed in $F_b(\widehat{G})$ and $\mathscr{C}(G)$ is dense in $L^1$(G), the image of $L^1(G)$ under the Fourier cotransform is likewise contained in $F_0(\widehat{G})$.

#### Proposition 11 {#ts-v-s4-prop-11 .statement tag=03EV}

a) Let $u= (u_{\pi})_{\pi\in\widehat{G}}$ be an element of $F(\widehat{G})$. If the family $(\mathscr{F}_{\pi}(u_{\pi}))_{\pi\in\widehat{G}}$ is uniformly summable in $\mathscr{C}(G)$, then its sum $f$ is a continuous function on G whose Fourier cotransform is $u$;

b) Let $f\in L^1(G)$. If the family $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ is uniformly summable in $\mathscr{C}(G)$, then its sum is a continuous fun$\widehat{c}$tion on G whose class in $L^1(G)$ is equal to $f$.

Let us prove assertion a). Since G is compact, the sum $f$ of the family $(\mathscr{F}_{\pi}(u_{\pi}))$ belongs to $L^2(G)$ and the series

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

converges in $L^2(G)$ to $f$ (INT, IV, p. 127, § 3, No.$^o3$, prop. 4). Hence one has $\mathscr{F}_G((u_{\pi})_{\pi}) =f$ in $L^2$(G), whence $(u_{\pi})_{\pi\in\widehat{G}}=\overline{\mathscr{F}}_G(f)$ (Theorem 2).

Let us prove assertion b). Assertion a) may be applied to the family $(\pi (f))_{\pi\in G}$. The sum $g$ of the family $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ is a continuous function, hence belonging to $L^2$(G), such that $\mathscr{F}_G(g) = (\pi (f))_{\pi\in G}$. Since $\mathscr{F}_G$ is injective on $L^2$(G), one has $f=g$ in $L^2$(G), hence in $L^1(G)$.

The algebra $\mathscr{C}(\widehat{G})$ of complex-valued functions on $\widehat{G}$ is identified with the center of the algebra $F(\widehat{G})$ by the mapping which to $f:\widehat{G}\rightarrow \mathbf{C}$ associates the central element $(f(\pi )1_{E_{\pi}})_{\pi\in\widehat{G}}$ of $F(\widehat{G})$. Let us denote by $\mathscr{M}^1(G^{\sharp})$ the space of bounded central measures on G. It is a closed subspace of the Banach algebra $\mathscr{M}^1(G)$. For every measure $\nu \in \mathscr{M}^1(G^{\sharp})$ and every representation $\pi \in \widehat{G}$, one has $\pi (\nu )\in$ End$_G(E_{\pi})$ hence $\pi (\nu )$ is a multiple of the identity mapping of $E_{\pi}$ by Schur’s Lemma (Prop. 6 of V, p. 386). The restriction of the Fourier cotransform to $\mathscr{M}^1(G^{\sharp})$ is therefore identified with a unital morphism of involutive Banach algebras from $\mathscr{M}^1(G^{\sharp})$ into $\mathscr{C}(\widehat{G})$. This morphism is injective; the image of $L^1(G^{\sharp})$ is contained in $\mathscr{C}_b(\widehat{G})$ and its restriction to $L^2(G^{\sharp})$ is an isometric isomorphism onto $L^2(\widehat{G},\widehat{\mu})$.

### 9. Frobenius-Schur Indicator and Larsen’s Alternative

Recall (LIE, VIII, §7, No. $^o6$, Def. 2) that an irreducible representation of G in a complex vector space E of finite dimension is said to be of orthogonal type (resp. of symplectic type) if there exists a non-zero symmetric bilinear form on E invariant under G (resp. if there exists a non-zero alternating bilinear form on E invariant under G). It is said to be of complex type if there exists no non-zero bilinear form on E invariant under G.

When an irreducible representation in E is of orthogonal type (resp. symplectic), the space of symmetric (resp. alternating) G-invariant bilinear forms on E is of dimension 1 and every non-zero G-invariant bilinear form on E is non-degenerate.

A representation of orthogonal type is sometimes said to be of real type, and a representation of symplectic type is sometimes said to be of quaternionic type (cf. LIE, IX, App. II).

Let $\pi$ be an irreducible representation of G in a complex vector space E. The three possibilities above are distinguished by the value of the quantity

FS($\pi$ ) $=\int_G\chi_{\pi}(g^2)d\mu(g)$,

which is called the Frobenius-Schur indicator of $\pi$. One has in fact

1 if $\pi$ is of orthogonal type,

FS($\pi$ ) $=-1$ if $\pi$ is of symplectic type,

0 if $\pi$ is of complex type.

(LIE, IX, App. 2, p. 103, Prop. 3 and p. 105, Prop. 4).

When G is a Lie group, one can calculate FS($\pi$ ) with the aid of Prop. 1 of LIE, IX, p. 69.

#### Definition 3 {#ts-v-s4-def-3 .statement tag=03EW}

Let $\varrho$ be a finite-dimensional unitary representation of G in a Hilbert space E. Let $k$ be a positive integer. The absolute moment of order $2k$ of $\varrho$ is defined to be, and is denoted by $M_{2k}(\varrho )$, the dimension of the subspace of G-invariant elements in the representation $\overline{\varrho}^{\otimes k}\otimes \varrho^{\otimes k}$.

#### Theorem 3 (Larsen’s Alternative) {#ts-v-s4-thm-3 .statement tag=03EX}

Assume that G is infinite. Let $\pi$ be a faithful unitary representation of G in a Hilbert space E of finite dimension $\geqslant 2$.

a) Assume that the derived group of G is infinite. Then $M_4(\pi )\geqslant 2$ with equality if and only if G contains $\mathbf{S}\mathbf{U}(E)$;

b) Assume that dim(E) $\geqslant 3$, that $\pi$ is of orthogonal or symplectic type, and that dim(E) $\not = 4$ if $\pi$ is of orthogonal type. Then $M_4(\pi )\geqslant 3$ with equality if and only if the complexified Lie algebra of G is equal to the Lie algebra of a non-degenerate G-invariant bilinear form on E. *This is the case if and only if the identity component $G_0$ of G is a maximal compact subgroup of the automorphism group of such a bilinear form.*

We shall use the following lemmas in the proof.

#### Lemma 5 {#ts-v-s4-lem-5 .statement tag=03EY}

Let $\pi$ be a unitary representation of G in a Hilbert space E of finite dimension. Let $(\varrho_i)_{i\in I}$ be a family of non-zero unitary representations of G and $(n_i)_{i\in I}$ a family of integers $\geqslant 1$ such that the representation $\overline{\pi}\otimes \pi$ of G (resp. the representation $\pi \otimes \pi$ ) is isomorphic to the direct sum $\bigoplus_{i\in I}\varrho^{n_i}_i$. Then one has

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

with equality if and only if the representations $\varrho_i$ are irreducible and pairwise non-isomorphic.

Let us denote by $\chi_i$ the character of $\varrho_i$ for $i\in I$. One has

$|\chi_{\pi}|^2=\chi_{\overline{\pi}\otimes\pi}=\sum_{i\in I}n_i\chi_i$, (resp. $\chi^2_{\pi}=\chi_{\pi\otimes\pi}=\sum_{i\in I}n_i\chi_i$).

From the definition and Cor. 3 of V, p. 466, there follows

$$
M_4(\pi ) =\int_G|\chi_{\pi}|^4d\mu
$$

whence, in both cases, the formula

$M_4(\pi ) =\sum_{i,j}n_in_j\int_G\chi_i\overline{\chi}_jd\mu=\sum_{i,j}n_in_j$ dim Hom$_G(\varrho_i, \varrho_j)$

(Cor. 4, b) of V, p. 459). Let $i\in I$. Since the representation $\varrho_i$ is not zero, the space Hom$_G(\varrho_i, \varrho_i)$ is non-zero, and one deduces the lower bound

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

Moreover, since $n_i\geqslant$ 1, there is equality if and only if one has dim Hom$_G(\varrho_i, \varrho_j) = 0$ if $i\not =j$ and dim Hom$_G(\varrho_i, \varrho_i) = 1$ for all $i$. The second condition holds if and only if the representations $\varrho_i$ are irreducible (loc. cit.). The first is then satisfied if and only if the representations $\varrho_i$ are pairwise non-isomorphic, by Schur’s Lemma (V, p. 387, Cor. 2).

If E is a module over a commutative ring A, the a-module $\mathsf{S}^2(E)$ (resp. $\wedge^2E$) will be called the symmetric square (resp. exterior square) of E.

#### Lemma 6 {#ts-v-s4-lem-6 .statement tag=03EZ}

Let $q$ be a non-degenerate bilinear form on a finite-dimensional complex vector space E of dimension $\geqslant 3$.

a) If $q$ is symmetric, then the adjoint representation of the orthogonal Lie algebra $\mathfrak{s}\mathfrak{o}(q)$ is isomorphic to the exterior square $\wedge^2E$ of the natural representation $\mathfrak{s}\mathfrak{o}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$;

b) If $q$ is alternating, then the adjoint representation of the symplectic Lie algebra $\mathfrak{s}\mathfrak{p}(q)$ is isomorphic to the symmetric square $\mathsf{S}^2(E)$ of the natural representation $\mathfrak{s}\mathfrak{p}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$.

Let $\mathbf{C}$ be provided with the identical involutive automorphism. The bilinear form $q$ is then $\varepsilon$-Hermitian (A, IX, § 3, n$^o1$, Def. 1) with $\varepsilon = 1$ in case a) and $\varepsilon =-1$ in case b). For every $u\in$ End(E), let $^tu$ denote the adjoint of $u$ with respect to $q$. Thus one has $q(x, u(y)) =q(^tu(x), y)$ for every $(x, y)\in E\times E$. Let $v$ denote the unique automorphism of $E\otimes E$ such that $v(x\otimes y) =y\otimes x$ for every $(x, y)\in E^2$.

There exists a unique linear mapping $w$ of $E\otimes E$ into End(E) such that $w(a\otimes b)$ is the linear mapping defined by $x\mapsto q(a, x)b$ for every $(a, b, x)\in E^3$. The mapping $w$ is an isomorphism. For every $s\in E\otimes E$, one has

$$
t(w(s)) =\varepsilon  w(v(s)) \tag{3}
$$

In fact, for all $(x, y)$ and $(a, b)$ in $E\times E$, there follows

$$
q(x, w(a\otimes b)y) =q(a, y)q(x, b) =\varepsilon q(b, x)q(a, y) =q(\varepsilon w(b\otimes a)x, y)
$$

Finally, denote by $x\mapsto x^*$ the isomorphism of E onto $E'$ deduced from $q$, that is to say such that $\langle x^*, y\rangle =q(x, y)$ for every $(x, y)\in E^2$.

With these notations established, let H be the orthogonal group (resp. symplectic) of $q$. It is a Lie subgroup of $\mathbf{G}\mathbf{L}(E)$ whose Lie algebra $\mathfrak{h}$ is the subspace of End(E) consisting of the $u\in$ End(E) such that $^tu=-u$ (LIE, III, p. 146, cor. 1). Since the form $q$ is H-invariant, we have

$$
\langle (ga)^*, b\rangle =q(ga, b) =\langle a, g^{-1}b\rangle
$$

for every $g\in H$ and every $(a, b)\in E\times E$.

Equip End(E) with the adjoint representation Ad of H. The linear mapping $w$ is a morphism of representations of H: in fact, for every $g\in H$ and every $(a, b, x)\in E^3$, we have

$$
w(g(a\otimes b))(x) =\langle (ga)^*, x\rangle gb=\langle a, g^{-1}x\rangle gb
$$

$=g(\langle a, g^{-1}x\rangle b) =$ Ad($g$)$(w(a\otimes b))x$,

whence the conclusion by linearity.

Since $v$ is likewise a morphism of representations of H, the same is true of the linear mapping $\theta =w-\varepsilon  w\circ v$; the latter is therefore a morphism of $\mathfrak{h}$-modules.

Let F $\subset E\otimes E$ be the subspace of elements $s\in E\otimes E$ such that $v(s) =-\varepsilon s$. If $\varepsilon =-1$, the restriction to F of the canonical mapping of $E\otimes E$ into the symmetric square of E is an isomorphism of $\mathbf{C}$-vector spaces (A, III, p. 72); if $\varepsilon = 1$, the restriction to F of the canonical mapping of $E\otimes E$ into the exterior square of E is an isomorphism of $\mathbf{C}$-vector spaces (loc. cit., p. 82).

The image of F under $\theta$ is contained in $\mathfrak{h}:$ in fact, for every $s\in F$, formula (3) implies

$$
^t\theta (s) =^tw(s)-\varepsilon^tw(v(s)) =\varepsilon  w(v(s))-w(s) =-\theta (s)
$$

By definition of F, the restriction of the mapping $\theta$ to F coincides with that of $2w$ and the linear mapping $\theta$ is therefore injective on F. Since dim(F) = dim($\mathfrak{h}$) (A, III, p. 75, th. 1 and p. 87, cor. 1 and LIE, VIII, p. 192 and p. 201), one concludes that $\theta$ induces by passing to the subspaces an isomorphism of $\mathfrak{h}$-modules of F onto $\mathfrak{h}$, whence the lemma.

#### Lemma 7 {#ts-v-s4-lem-7 .statement tag=03F0}

Let $H_2$ be a real Lie group and let $H_1$ be a closed subgroup of $H_2$. The complexified Lie algebra of $H_1$ identifies with a subrepresentation of the adjoint representation of $H_1$ on the complexified Lie algebra of $H_2$.

In fact, the restriction to $H_1$ of the adjoint representation of $H_2$ on its Lie algebra identifies with the adjoint representation of $H_1$.

#### Lemma 8 {#ts-v-s4-lem-8 .statement tag=03F1}

Let E be a finite-dimensional complex Hilbert space of dimension $n$.

a) The groups $\mathbf{S}\mathbf{U}(E)$ and $\mathbf{U}(E)$ are connected;

b) The derived group of $\mathbf{S}\mathbf{U}(E)$ is equal to $\mathbf{S}\mathbf{U}(E)$;

c) The derived group of $\mathbf{U}(E)$ is equal to $\mathbf{S}\mathbf{U}(E)$.

We may suppose that $n\geqslant 1$ and that $E =\mathbf{C}^n$.

Let A be the subgroup of $\mathbf{U}(E)$ formed by the diagonal matrices; it is homeomorphic to $\mathbf{U}^n$, and therefore connected (TG, VI, p. 11, cor. 2 and I, p. 83, prop. 8). Its intersection with $\mathbf{S}\mathbf{U}(E)$ is homeomorphic to $\mathbf{U}^{n-1}$, and is therefore likewise connected.

By Theorem 1 of IV, p. 149, the group $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E)$) is the union of the connected subsets $gAg^{-1}$ for $g\in G$ (resp. of the connected subsets $g(A\cap \mathbf{S}\mathbf{U}(E))g^{-1}$); since the identity element belongs to each of these sets, the space $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E)$) is connected (TG, I, p. 81, prop. 2).

Let us prove b). The assertion is true when $n= 1$, since $\mathbf{S}\mathbf{U}(E)$ is then reduced to the identity element. Suppose therefore that $n\geqslant 2$. The Lie algebra of $\mathbf{S}\mathbf{U}(E)$ is then simple (LIE, IX, p. 20, § 3, No.$^o4$) and hence the derived group of $\mathbf{S}\mathbf{U}(E)$ has finite index in $\mathbf{S}\mathbf{U}(E)$. The result follows, since $\mathbf{S}\mathbf{U}(E)$ is connected by a).

Assertion c) follows from b), since the derived group of $\mathbf{U}(E)$ is contained in $\mathbf{S}\mathbf{U}(E)$.

Let us now prove Theorem 3. Let $n$ denote the dimension of the Hilbert space E. Since the representation $\pi$ is faithful, we may suppose that G is a compact subgroup of $\mathbf{U}(E)$. The group G is closed in the real Lie group $\mathbf{U}$(E), and is therefore a compact real Lie group (LIE, III, §8, No.$^o2$, Theorem 2). By hypothesis, G is infinite, and therefore of dimension $\geqslant 1$. Let $\mathfrak{g}$ be its Lie algebra; it is non-zero.

Let us prove a). Suppose that the derived group D(G) is infinite. We have the G-invariant decomposition End(E) $=\mathbf{C}1_E\oplus \mathfrak{s}\mathfrak{l}(E)$. The representations of G on $\mathbf{C}1_E$ and on $\mathfrak{s}\mathfrak{l}(E)$ are not isomorphic, since dim $\mathfrak{s}\mathfrak{l}(E)\geqslant 2$. By Lemma 5, we therefore have $M_4(\pi )\geqslant 2$ with equality if and only if the representation of G in $\mathfrak{s}\mathfrak{l}(E)$ is irreducible. Now, the derived group of G is contained in $\mathbf{S}\mathbf{L}$(E), and the complexification of the Lie algebra of D(G) may therefore be identified with a subspace of $\mathfrak{s}\mathfrak{l}$(E), which is a subrepresentation of the representation of G in $\mathfrak{s}\mathfrak{l}(E)$ (Lemma 7). This subrepresentation is non-zero, since D(G) is infinite. We therefore have $M_4(\pi ) = 2$ if and only if $(\mathscr{D}\mathfrak{g})_{(\mathbf{C})}=\mathfrak{s}\mathfrak{l}(E)$. Since D(G) is contained in $\mathbf{S}\mathbf{U}$(E), and since $\mathbf{S}\mathbf{U}(E) = D(\mathbf{S}\mathbf{U}(E))$ (Lemma 8), this condition is equivalent to $\mathbf{S}\mathbf{U}(E)\subset G$.

For the proof of assertion b), we resume the notation of LIE, VIII, §13, No.$^o$ 2–4.

Suppose that $\pi$ is of symplectic type and that dim(E) $\geqslant 3$. Let $q$ be a non-zero G-invariant alternating bilinear form on E; it is nondegenerate (LIE, IX, p. 103, App. 2, prop. 3) and G is a compact subgroup of the symplectic group $\mathbf{S}\mathbf{p}(q)$. Let us denote by $q^*\in \wedge^2E$ the element with which the alternating form $q$ is identified. The complexified Lie algebra $\mathfrak{g}_{(\mathbf{C})}$ of G is contained in $\mathfrak{s}\mathfrak{p}(q)$. Now, since dim(E) $\geqslant 3$, the representation of $\mathfrak{s}\mathfrak{p}(q)$ in $E\otimes E$ admits the direct-sum decomposition

$$
E\otimes E =\mathsf{S}^2(E)\oplus \wedge^2E =\mathsf{S}^2(E)\oplus E_2\oplus \mathbf{C}q^*
$$

where $E_2$ is the second fundamental representation of $\mathfrak{s}\mathfrak{p}(q)$ (LIE, VIII, p. 202, §13, No.$^o3$, (IV)). The representations $E_2$ and $\mathbf{C}q^*$ of $\mathfrak{s}\mathfrak{p}(q)$ are irreducible (loc. cit.) and the representation $\mathsf{S}^2(E)$ is non-zero.

After lemma 5, one therefore has $M_4(\pi )\geqslant 3$ with equality if and only if the representations of G in $\mathsf{S}^2$(E), $E_2$ and $\mathbf{C}q^*$ are irreducible and pairwise non-isomorphic.

Suppose that $M_4(\pi ) = 3$. Since the representation $\mathsf{S}^2(E)$ is identified with the adjoint representation of $\mathfrak{s}\mathfrak{p}(q)$ (lemma 6), it contains as subrepresentation the complexification of the adjoint representation of G (lemma 7). One therefore has $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$.

Conversely, suppose that $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$. The adjoint representation of $\mathfrak{s}\mathfrak{p}(q)$ and the representation $E_2$ of $\mathfrak{s}\mathfrak{p}(q)$ are irreducible, of dimensions $n(n+ 1)/2$ and $n(n-1)/2-1$ respectively (LIE, VIII, p. 202, §13, No.$^o3$, (IV)), which are different and $\geqslant 2$ since $n\geqslant 3$, whence $M_4(\pi ) = 3$.

Finally, suppose that $\pi$ is of real type and that dim(E) $\geqslant 3$ and dim(E) $\not = 4$. Let $q$ be a non-zero symmetric bilinear form, G-invariant on E; it is separating (LIE, IX, p. 103, App. 2, prop. 3) and G is a compact subgroup of the orthogonal group $\mathbf{O}(q)$. Let us denote by $q^*\in \mathsf{S}^2(E)$ the element with which $q$ is identified.

The complexified Lie algebra $\mathfrak{g}_{(\mathbf{C})}$ of G is contained in $\mathfrak{s}\mathfrak{o}(q)$. The representation of $\mathfrak{s}\mathfrak{o}(q)$ in $E\otimes E$ admits the decomposition into a direct sum

$$
E\otimes E =\wedge^2E\oplus \mathsf{S}^2(E) =\wedge^2E\oplus \mathsf{S}^2_0(E)\oplus \mathbf{C}q^*
$$

where $\mathsf{S}^2_0(E)$ is the orthogonal of $q^*$ in $\mathsf{S}^2(E)$. These representations are of dimension at least 2 since dim(E) $\geqslant 3$. After lemma 5, one has $M_4(\pi )\geqslant 3$ with equality if and only if the representations of G in $\wedge^2E$ and $\mathsf{S}^2_0(E)$ are irreducible and non-isomorphic.

Suppose that $M_4(\pi ) = 3$. Since the representation $\wedge^2E$ is identified with the adjoint representation of $\mathfrak{s}\mathfrak{o}(q)$ (lemma 6), it contains as subrepresentation the complexification of the adjoint representation of G (lemma 7). The condition $M_4(\pi ) = 3$ therefore implies that $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

Conversely, suppose that $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$. The adjoint representation of $\mathfrak{s}\mathfrak{o}(q)$ is irreducible, since dim(E) $\not = 4$ (LIE, VIII, § 13, p. 193, (I) and p. 206, (I)), and of dimension $n(n-1)/2$. The representation $\mathsf{S}^2_0(E)$ of $\mathfrak{s}\mathfrak{o}(q)$ has highest weight $2\varpi_1$. By comparing its dimension with that of the irreducible representation of $\mathfrak{s}\mathfrak{o}(q)$ of highest weight $2\varpi_1$, calculated by Weyl's formula (cf. LIE, VIII, §9, n$^o2$, th. 2 and LIE, VI, plates II and IV), one verifies that $\mathsf{S}^2_0(E)$ is irreducible. It follows therefore that $M_4(\pi ) = 3$ if $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

#### Remark 1 {#ts-v-s4-n9-rem-1 .statement tag=03F2}

The condition "G is infinite" is necessary in Theorem 3 (exercise 9 of V, p. 507).

#### Remark 2 {#ts-v-s4-n9-rem-2 .statement tag=03F3}

Let $n\in \mathbf{N}$. For every unitary representation $\varrho$ of a compact group in a Hilbert space of dimension $n$, one has $M_4(\varrho )\leqslant n^2$; equality is possible (exercise 15 of V, p. 508).

#### Remark 3 {#ts-v-s4-n9-rem-3 .statement tag=03F4}

One can prove (cf. R. Guralnick and P.H. Tiep, Decomposition of small tensor powers and Larsen’s conjecture, Representation Theory **9** (2005), 138–208) that the condition that G be infinite can be omitted if one assumes that E is of dimension $\geqslant 7$ and if one replaces the hypothesis $M_4(\pi ) = 2$ (resp. $M_4(\pi ) = 3$) by $M_8(\pi ) = 24$ (resp. $M_8(\pi ) = 105$).

## EXERCISES {#ts-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
