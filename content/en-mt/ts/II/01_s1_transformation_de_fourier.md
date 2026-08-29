---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 1
section_title: Transformation de Fourier
lang: en
source: ts-i-ii-fr
book_pages: TS II.201-TS II.243, TS II.262-TS II.304
pdf_pages: 0213-0255, 0274-0316
extraction: native
subsections:
    - "no": 1
      title: Caractères unitaires d’un groupe localement compact commutatif
      page: 201
      pdf_page: 213
    - "no": 2
      title: Définition de la transformation de Fourier
      page: 206
      pdf_page: 218
    - "no": 3
      title: Le théorème de Plancherel
      page: 210
      pdf_page: 222
    - "no": 4
      title: La formule d’inversion de Fourier
      page: 217
      pdf_page: 229
    - "no": 5
      title: Le théorème de dualité de Pontryagin
      page: 220
      pdf_page: 232
    - "no": 6
      title: Propriétés fonctorielles de la dualité
      page: 224
      pdf_page: 236
    - "no": 7
      title: La formule de Poisson
      page: 229
      pdf_page: 241
    - "no": 8
      title: Exemples de dualité
      page: 232
      pdf_page: 244
    - "no": 9
      title: Transformée de Fourier euclidienne et séries de Fourier
      page: 237
      pdf_page: 249
statements: 95
exercises: 68
content_sha256: 4709ffeb6bc4b8d9e3cb7310b2947b2de94e621599ed95e7d680b38ec7f2f419
translated_from: content/fr/ts/II/01_s1_transformation_de_fourier.md
source_lang: fr
translation_method: machine
source_content_sha256: 44d8e1262e651735e5764e1dec2d575d432840d199837a351570f025a680a83d
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-0af303bf
glossary_version: 34
glossary_terms_sha256: 21cf7c45c852a3c48da6932f217b966bfb8a07a7a6bc4286e41c6dfe9bd85bad
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. FOURIER TRANSFORM

### 1. Unitary characters of a locally compact commutative group

#### Definition 1 {#ts-ii-s1-def-1 .statement tag=02HQ}

A continuous homomorphism of G into the multiplicative group $\mathbf{U}$ of complex numbers of modulus 1 is called a unitary character of G.

In other words, a unitary character is a continuous complex-valued function $\chi$ on G such that:

$$
\chi (xy) =\chi (x)\chi (y),|\chi (x)|= 1(x, y\in G)
$$

In this chapter, we shall often say simply "character" instead of "unitary character".

Let E be a Hilbert space of dimension 1, and let $\chi$ be a unitary character of G. The mapping which to $x\in G$ associates the homothety of ratio $\chi (x)$ in E is a continuous isometric linear representation of G in E. Conversely, every bounded continuous linear representation of G in E is obtained by this process, and in particular is unitary.

It is immediate that the product of two unitary characters, the inverse of a unitary character, and the constant function equal to 1 are unitary characters. Hence the set $\widehat{G}$ of unitary characters of G is a group for multiplication. This group is commutative. On the other hand, the mapping $(\chi_1, \chi_2)\mapsto \chi_1\chi^{-1}_2=\chi_1\overline{\chi}_2$ is continuous for the topology of compact convergence, and $\widehat{G}$ endowed with the topology of compact convergence is a topological group (TG, X, p. 6, Corollary 2 and Remark 1).

#### Definition 2 {#ts-ii-s1-def-2 .statement tag=02HR}

The topological group $\widehat{G}$ is called the dual group of G.

Since G is locally compact, the mapping $(x, \chi )\mapsto \chi (x)$ is continuous on $G\times \widehat{G}$ (TG, X, p. 28, th. 3).

Recall that $\mathscr{M}^1(G)$ denotes the unital involutive Banach algebra of bounded complex measures on G (Example 4 of I, p. 99). For every bounded complex measure $\mu\in \mathscr{M}^1(G)$ and every $\chi \in \widehat{G}$, we write

$$
\chi (\mu) =\int_G\chi (x)d\mu(x) \tag{1}
$$

(cf. INT, VIII, §2, No$^o6$).

#### Lemma 1 {#ts-ii-s1-lem-1 .statement tag=02HS}

For every $\chi \in \widehat{G}$, the mapping $\mu\mapsto \chi (\mu)$ is a hermitian character of the involutive Banach algebra $\mathscr{M}^1(G)$.

By INT, VIII, §3, No$^o3$, Prop. 11, the mapping $\mu\mapsto \chi (\mu)$ is a character of the involutive Banach algebra $\mathscr{M}^1(G)$. Further, we have:

$$
\chi (\mu^*) =\int_G\chi (x^{-1})d\mu(x) =\int_G\overline{\chi(x)}d\mu(x) =\overline{\chi(\mu)}
$$

and therefore this character is hermitian.

Thus we have defined a mapping of $\widehat{G}$ into $\mathsf{X}(\mathscr{M}^1(G))$; it will be called canonical.

Let $\chi \in \widehat{G}$. The restriction of $\mu\mapsto \chi (\mu)$ to $L^1(G)$ is non-zero (cf. INT, VIII, §2, No$^o7$, Prop. 10). By restriction to the involutive Banach subalgebra $L^1(G)$, we therefore obtain a mapping of $\widehat{G}$ into $\mathsf{X}(L^1(G))$, called canonical. It associates to $\chi \in \widehat{G}$ the hermitian character

$$
f\mapsto \chi (f) =\chi (f\cdot dx) =\int_Gf(x)\chi (x)dx(f\in L^1(G)) \tag{2}
$$

of $L^1(G)$.

#### Proposition 1 {#ts-ii-s1-prop-1 .statement tag=02HT}

The canonical mapping of $\widehat{G}$ into $\mathsf{X}(L^1(G))$ is a homeomorphism.

Let us denote this canonical mapping by ev and, for $\chi \in \widehat{G}$, let us denote by ev$_{\chi}$ the image of the character $\chi$ under ev, that is to say, the hermitian character $f\mapsto \chi (f)$ of $L^1(G)$. Considered as a mapping of $\widehat{G}$ into the dual of $L^1(G)$, the mapping ev is the composite of the injection of $\widehat{G}$ into $L^{\infty}(G)$, endowed with the weak topology $\sigma (L^{\infty}(G),L^1(G))$, and the injection of $L^{\infty}(G)$ into the dual of $L^1(G)$, endowed with the topology of simple convergence. Since $\widehat{G}$ is a bounded subset of $L^{\infty}(G)$, the first mapping is continuous by the Lebesgue theorem (INT, IV, §3, No$^o7$, Th. 6). The second is likewise continuous, by definition. This proves that the mapping ev is continuous.

If $\chi \in \widehat{G}$ and if $f\in L^1(G)$, we have ev$_{\chi}(\varepsilon_x*f) =\chi (x$)ev$_{\chi}(f)$. Taking $f$ such that ev$_{\chi}(f)\not= 0$, we deduce that the mapping ev is injective.

Let $\zeta \in \mathsf{X}(L^1(G))$ and let $f\in L^1(G)$ be such that $\zeta (f)\not= 0$. Define a mapping $\chi : G\rightarrow \mathbf{C}$ by putting, for $x\in G$:

$$
\chi (x) =\frac{\zeta(\varepsilon_x*f)}{\zeta(f)} \tag{3}
$$

We have $\chi (e) = 1$. Since the mapping $x\mapsto \varepsilon_x*f=\boldsymbol{\gamma }(x)(f)$ of G into $L^1(G)$ is continuous (INT, VIII, §2, n$^o5$, Proposition 8), the mapping $\chi$ is continuous. It is bounded because, for every $x\in G$, we have

$$
|\chi (x)|\leqslant \frac{\|\varepsilon_x*f\|}{|\zeta(f)|}=\frac{\|f\|}{|\zeta(f)|}
$$

(Theorem 1 of I, p. 29 and INT, VIII, loc. cit.).

Now let $\mathfrak{B}$ be a basis of the filter of neighbourhoods of $e$ consisting of compact neighbourhoods. For every $V\in \mathfrak{B}$, let $g_V$ be a positive continuous function, zero outside V and of integral equal to 1 (Lemma 1 of II, p. 200). For every function $h\in L^1(G)$, one then has

$\varepsilon_x*h=$ lim$_{V,\mathfrak{B}}(\varepsilon_x*h)*g_V=$ lim$_{V,\mathfrak{B}}(\varepsilon_x*g_V*h)$,

in $L^1(G)$, the limit being taken with respect to the filter of sections of $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, Proposition 20). In particular, since $\zeta (\varepsilon_x*g_V*f) =$ $\zeta (\varepsilon_x*g_V)\zeta (f)$, it follows that

$\chi (x) =$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V)$.

For every $h\in L^1(G)$, we obtain

$\zeta (\varepsilon_x*h) =$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V*h) =\zeta (h)$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V) =\chi (x)\zeta (h)$.

Consequently, for $x, y\in G$ we have:

$$
\chi (xy) =\frac{\zeta(\varepsilon_x*\varepsilon_y*f)}{\zeta(f)}=\frac{\chi(x)\zeta(\varepsilon_y*f)}{\zeta(f)}=\chi (x)\chi (y)
$$

which proves that $\chi$ is a homomorphism of G into $\mathbf{C}^*$. Since $\chi$ is bounded and continuous, it is a unitary character of G. Moreover, if $g\in L^1(G)$, we have

$$
g*f=\int_G(\varepsilon_x*f)g(x)dx
$$

in $L^1(G)$ (INT, VIII, §1, n$^o5$, Proposition 7), whence

$$
\zeta (g)\zeta (f) =\zeta (g*f) =\int_G\zeta (\varepsilon_x*f)g(x)dx
$$

$=\zeta (f)\int_G\chi (x)g(x)dx=$ ev$_{\chi}(g)\zeta (f)$ (INT, VI, §1, n$^o1$, Proposition 1), which shows that $\zeta =$ ev$_{\chi}$. Consequently, ev is surjective, hence bijective.

Finally, let us show that the reciprocal mapping ev$^{-1}$ is continuous. Let $\zeta \in \mathsf{X}(L^1(G))$. Let $f\in L^1(G)$ be a function such that $\zeta (f)\not= 0$. The set W of $\xi \in \mathsf{X}(L^1(G))$ such that $\xi (f)\not= 0$ is an open neighbourhood of $\zeta$ in $\mathsf{X}(L^1(G))$. For every $\xi \in W$, what precedes shows that ev$^{-1}(\xi )$ is the character

$$
x\mapsto \frac{\xi(\varepsilon_x*f)}{\xi(f)}
$$

Let $\mathfrak{F}$ be a filter on $W\subset \mathsf{X}(L^1(G))$ converging to $\zeta$. Since the set $\mathsf{X}(L^1(G))$ is bounded, hence equicontinuous, in $L^{\infty}(G)$, the uniform structure of simple convergence coincides with the uniform structure of compact convergence (TG, X, p. 16, Theorem 1). Let K be a compact subset of G. The set of the $\varepsilon_x*f$ for $x\in K$ is compact in $L^1(G)$ (INT, VIII, §2, No.$^o5$, Proposition 8). We have therefore

lim$_{\xi ,\mathfrak{F}}\xi (\varepsilon_x*f) =\zeta (\varepsilon_x*f)$

uniformly for $x\in K$. It follows that

lim$_{\xi ,\mathfrak{F}}$ ev$^{-1}(\xi ) =$ ev$^{-1}(\zeta )$,

hence ev$^{-1}$ is continuous at $\zeta$. This completes the proof of the proposition.

Henceforth we shall identify a unitary character $\chi$ of G with the character $f\mapsto \int_Gf(x)\chi (x)dx$ of $L^1(G)$.

#### Remark 1 {#ts-ii-s1-n1-rem-1 .statement tag=02HU}

*The bijectivity of the mapping from $\widehat{G}$ into $\mathsf{X}(L^1(G))$ of Proposition 1 is a particular case of the correspondence between continuous representations of a locally compact group H (not necessarily commutative) and continuous representations of the algebra $L^1(H)$.*

#### Remark 2 {#ts-ii-s1-n1-rem-2 .statement tag=02HV}

The canonical mapping from $\widehat{G}$ into $\mathsf{X}(\mathscr{M}^1(G))$ is not surjective in general (II, p. 308, exercise 14).

#### Corollary 1 {#ts-ii-s1-prop-1-cor-1 .statement tag=02HW}

Every character of $L^1(G)$ is hermitian. The canonical mapping from $\mathsf{X}$(Stell(G)) (Definition 9 of I, p. 125) into $\mathsf{X}(L^1(G))$ is a homeomorphism.

The first assertion follows from Proposition 1 and Lemma 1 by restriction to $L^1(G)$. The second follows from the first and from the corollary of Proposition 20 of I, p. 124.

#### Corollary 2 {#ts-ii-s1-prop-1-cor-2 .statement tag=02HX}

The topological group $\widehat{G}$ is locally compact.

In fact, $\mathsf{X}(L^1(G))$ is locally compact (corollary of Theorem 1 of I, p. 29).

We shall identify $\widehat{G}$ with $\mathsf{X}(L^1(G))$ and $\mathsf{X}$(Stell(G)). For $x\in G$ and $\chi \in \widehat{G}$, we shall denote by $\langle \chi , x\rangle$ the complex number $\chi (x)$, which belongs to $\mathbf{U}$.

We say that $x$ and $\chi$ are orthogonal if $\langle \chi , x\rangle = 1$. Let A be a subset of G (resp. of $\widehat{G}$); the set of elements of $\widehat{G}$ (resp. of G) orthogonal to A is a closed subgroup of $\widehat{G}$ (resp. of G), called the orthogonal of A and denoted by $A^{\bot}$. The orthogonal of G is reduced to $e$.

For $x\in G$, let us denote by $\eta (x)$ the mapping of $\widehat{G}$ into $\mathbf{U}$ defined by $\chi \mapsto$ $\langle \chi , x\rangle$. By definition of the multiplication in $\widehat{G}$, the mapping $\eta (x)$ is a group homomorphism. It is continuous since the mapping $(x, \chi )\mapsto  \langle \chi , x\rangle$ of $G\times \widehat{G}$ into $\mathbf{U}$ is continuous (TG, X, p. 28, th. 3). Thus we have defined a mapping $\eta$, called canonical, of G into the bidual group $\widehat{\widehat{G}}$; it is a group homomorphism. Moreover, the mapping $\eta$ is continuous (TG, X, p. 28, th. 3). We shall prove later (II, p. 220, th. 2) that $\eta$ is a group isomorphism of G onto $\widehat{\widehat{G}}$.

Let G and H be locally compact commutative groups, and let $\varphi : G\rightarrow H$ be a morphism of topological groups. For every $\chi \in \widehat{H}$, the mapping $\chi \circ \varphi$ is a character of G, denoted by $\widehat{\varphi}(\chi )$. This definition is expressed by the formula

$$
\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle \tag{4}
$$

for every $\chi \in \widehat{H}$ and every $x\in G$. It follows that $\widehat{\varphi}$ is a morphism of the topological group $\widehat{H}$ into the topological group $\widehat{G}$; one says that $\widehat{\varphi}$ is the dual of the morphism $\varphi$.

Let K be a locally compact commutative group and let $\psi : H\rightarrow K$ be a morphism of topological groups. The definition shows that $\widehat{\psi}\circ \varphi =\widehat{\varphi}\circ \widehat{\psi}$. If $\varphi$ is the identity mapping of G, then $\widehat{\varphi}$ is the identity mapping of $\widehat{G}$. In particular, if $\varphi$ is a group isomorphism, the same is true of $\widehat{\varphi}$, and $\widehat{\varphi}^{-1}$ is the dual of $\varphi^{-1}$.

#### Lemma 2 {#ts-ii-s1-lem-2 .statement tag=02HY}

Let G and H be locally compact commutative groups and let $f: H\rightarrow G$ be a morphism of topological groups. The kernel of $\widehat{f}$ is the orthogonal of the image of $f$.

By definition, we have $\chi \in$ Ker($\widehat{f}$) if and only if the restriction of $\chi$ to the image of $f$ is trivial.

#### Proposition 2 {#ts-ii-s1-prop-2 .statement tag=02HZ}

Let $n\geqslant 0$ be an integer and let $G_1, . . . ,G_n$ be locally compact commutative groups. Let G be the product group of the groups $G_j$ for $1\leqslant j\leqslant n$. For $1\leqslant j\leqslant n$, let $\lambda_j$ be the injection of $G_j$ into G which associates to $x\in G_j$ the element $(x_k)$ such that $x_k=e$ if $k\not=j$ and $x_j=x$. The mapping

$$
(\widehat{\lambda}_j)_{1\leqslant j\leqslant n}:\widehat{G}\rightarrow \prod_{1\leqslant j\leqslant n}\widehat{G}_j
$$

is a group isomorphism.

Let $m$ be the product mapping of $\widehat{G}^n$ into $\widehat{G}$, and for every $j$ such that $1\leqslant j\leqslant n$, let $\pi_j$ be the projection of G onto $G_j$. Let $\mu$ be the morphism of topological groups $m\circ (\widehat{\pi}_j)_j$ from $\prod\widehat{G}_j$ into $\widehat{G}$, such that

$$
\langle \mu((\chi_j)),(x_j)\rangle =\prod_{j=1}^n\langle \chi_j, x_j\rangle
$$

The mapping $\mu$ is continuous, and one verifies that $\mu$ and $(\widehat{\lambda}_j)$ are reciprocal bijections of one another. The proposition follows.

#### Remark {#ts-ii-s1-n1-rem-3 .statement tag=02I0}

The calculation of the dual group of an infinite product of commutative compact groups is the object of Corollary 4 of II, p. 234 below. The case of a commutative locally compact group which is an arbitrary product of locally compact groups follows from these two statements, since in such a product, all the factors except a finite number are compact (TG, I, p. 66, prop. 14, b)).

### 2. Definition of the Fourier transform

#### Definition 3 {#ts-ii-s1-def-3 .statement tag=02I1}

Let $\mu\in \mathscr{M}^1(G)$ be a bounded complex measure on G. The Fourier transform of $\mu$ is called the function $\mathscr{F}_G(\mu)$ on $\widehat{G}$ defined by

$$
\mathscr{F}_G(\mu)(\widehat{x}) =\int_G\overline{\langle\widehat{x}, x\rangle}d\mu(x) \tag{5}
$$

The Fourier cotransform of $\mu$ is called the function $\overline{\mathscr{F}}_G(\mu)$ on $\widehat{G}$ defined by

$$
\overline{\mathscr{F}}_G(\mu)(\widehat{x}) =\int_G\langle \widehat{x}, x\rangle d\mu(x) \tag{6}
$$

When there is no ambiguity concerning the group G considered, one shall also write $\mathscr{F}(\mu)$ and $\overline{\mathscr{F}}(\mu)$. One also sometimes denotes $\widehat{\mu}=\mathscr{F}_G(\mu)$.

#### Proposition 3 {#ts-ii-s1-prop-3 .statement tag=02I2}

For every measure $\mu\in \mathscr{M}^1(G)$, the functions $\mathscr{F}_G(\mu)$ and $\overline{\mathscr{F}}_G(\mu)$ are continuous and bounded. The mappings $\mathscr{F}_G:\mu\mapsto$ $\mathscr{F}_G(\mu)$ and $\overline{\mathscr{F}}_G:\mu\mapsto \overline{\mathscr{F}}_G(\mu)$ are continuous morphisms of the involutive algebra $\mathscr{M}^1(G)$ into the involutive algebra of bounded continuous functions on $\widehat{G}$ (Example 1 of I, p. 99).

Let $\mu\in \mathscr{M}^1(G)$. For every $\chi \in \widehat{G}$, one has

$$
|\mathscr{F}(\mu)(\chi )|=|\int_G\overline{\langle\chi , x\rangle}d\mu(x)|\leqslant \|\mu\|_1 \tag{7}
$$

therefore the Fourier transform of $\mu$ is bounded. Analogously, one verifies that $\overline{\mathscr{F}}(\mu)$ is bounded.

If $\chi$ tends to $\chi_0$ in $\widehat{G}$, the function $\chi$ on G tends to $\chi_0$ uniformly on every compact while remaining bounded by the constant function 1 which belongs to $L^1(G, \mu)$. By the Lebesgue theorem (INT, IV, §3, n$^o7$, th. 6), it follows that $\mathscr{F}(\mu)(\chi )$ tends to $\mathscr{F}(\mu)(\chi_0)$. Hence $\mathscr{F}(\mu)$ is continuous. The same is true of $\overline{\mathscr{F}}(\mu)$.

For every $\chi \in \widehat{G}$, the mapping $\mu\mapsto \chi (\mu) =\int\langle \chi , x\rangle d\mu(x)$ is a hermitian character of $\mathscr{M}^1(G)$ (Lemma 1 of II, p. 202). This implies that $\mathscr{F}$ and $\overline{\mathscr{F}}$ are morphisms of involutive algebras from $\mathscr{M}^1(G)$ into the involutive algebra of bounded continuous functions on $\widehat{G}$. Inequality (7) proves that these morphisms are continuous.

The Fourier transform of G (resp. the Fourier cotransform of G) is the mapping $\mu\mapsto \mathscr{F}_G(\mu)$ (resp. the mapping $\mu\mapsto$ $\overline{\mathscr{F}}_G(\mu)$) of $\mathscr{M}^1(G)$ into $\mathscr{C}_b(\widehat{G})$.

Let us note some useful formulae for $\mu\in \mathscr{M}^1(G),x\in G$ and $\chi \in \widehat{G}:$

$$
\overline{\mathscr{F}}(\mu)(\chi ) =\mathscr{F}(\mu)(\chi^{-1}) =\overline{\mathscr{F}(\overline{\mu})(\chi)} \tag{8}
$$

$$
\|\mathscr{F}(\mu)\|_{\infty}=\|\overline{\mathscr{F}}(\mu)\|_{\infty}\leqslant \|\mu\|_1 \tag{9}
$$

$$
\mathscr{F}(\varepsilon_x)(\chi ) =\overline{\langle\chi , x\rangle}
$$

(10)

$$
\overline{\mathscr{F}}(\varepsilon_x)(\chi ) =\langle \chi , x\rangle
$$

(in particular $\mathscr{F}(\varepsilon_e) =\overline{\mathscr{F}}(\varepsilon_e) = 1$),

$$
\mathscr{F}(\varepsilon_x*\mu)(\chi ) =\overline{\langle\chi , x\rangle}\mathscr{F}(\mu)(\chi )
$$

(11)

$$
\overline{\mathscr{F}}(\varepsilon_x*\mu)(\chi ) =\langle \chi , x\rangle \overline{\mathscr{F}}(\mu)(\chi )
$$

$$
\mathscr{F}(\chi \cdot \mu) =\varepsilon_{\chi}*\mathscr{F}(\mu)
$$

(12)

$$
\overline{\mathscr{F}}(\chi \cdot \mu) =\varepsilon_{\chi^{-1}}*\overline{\mathscr{F}}(\mu)
$$

Formulae (8), (9), (10) and (11) follow from the definitions. Let us prove the first of formulae (12), the second being analogous. For every $\xi$ in $\widehat{G}$ one has the equalities

$$
\mathscr{F}(\chi \cdot \mu)(\xi ) =\int_G\langle \xi , x\rangle \langle \chi , x\rangle d\mu(x) =\int_G\overline{\langle\xi \chi^{-1}, x\rangle}d\mu(x)
$$

$$
=\mathscr{F}(\mu)(\xi \chi^{-1}) = (\varepsilon_{\chi}*\mathscr{F}(\mu))(\xi )
$$

Let us note moreover that for every $\chi \in \widehat{G}$ and every measures $\mu$ and $\nu$ in $\mathscr{M}^1(G)$, one has

$$
(\varepsilon_{\chi}*\mathscr{F}(\mu))(\varepsilon_{\chi}*\mathscr{F}(\nu )) =\varepsilon_{\chi}*(\mathscr{F}(\mu)\mathscr{F}(\nu )) \tag{13}
$$

since the two members of this equality are functions on $\widehat{G}$ whose value at $\xi \in \widehat{G}$ is

$$
\mathscr{F}(\mu)(\xi \chi^{-1})\mathscr{F}(\nu )(\xi \chi^{-1})
$$

Let H be a locally compact commutative group and let $\varphi : G\rightarrow H$ be a continuous morphism. Let $\mu\in \mathscr{M}^1(G)$. The image measure $\varphi (\mu)$ is defined (INT, V, §6, n$^o1$, remark 1), and one gets $\mathscr{F}_H(\varphi (\mu)) =\mathscr{F}_G(\mu)\circ$ $\widehat{\varphi}($cf. INT, V, §6, n$^o4$, prop. 7).

By restriction to the subalgebra $L^1(G)$ of $\mathscr{M}^1(G)$, one obtains the definition of the Fourier transform and of the Fourier cotransform on $L^1(G)$. One thus has for $f\in L^1(G)$ and $\chi \in \widehat{G}:$

$$
(14)\mathscr{F}_G(f)(\chi ) =\int_G\overline{\langle\chi , x\rangle}f(x)dx,\overline{\mathscr{F}}_G(f)(\chi ) =\int_G\langle \chi , x\rangle f(x)dx
$$

In particular, $\mathscr{F}_G(f) =\overline{\overline{\mathscr{F}}_G(\overline{f})}$. One also has

$$
\overline{\mathscr{F}}(f)(\chi ) =\chi (f) \tag{15}
$$

for every $f\in L^1(G)$ and every $\chi \in \widehat{G}$.

Let $\sigma$ be an automorphism of G and Δ the module of $\sigma$ (INT, VII, §1, n$^o4$, def. 4). For $f\in L^1(G)$, one has

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1} \tag{16}
$$

(cf. loc. cit., formula (31)).

If one identifies $\widehat{G}$ and $\mathsf{X}(L^1(G))$ (prop. 1 of II, p. 202), the Fourier cotransform is nothing but the Gelfand transform of the Banach algebra $L^1(G)$ (I, p. 7, def. 5).

#### Proposition 4 {#ts-ii-s1-prop-4 .statement tag=02I3}

The Fourier transform and the Fourier cotransform are injective morphisms of involutive algebras of $L^1(G)$ into the algebra $\mathscr{C}_0(\widehat{G})$ of continuous functions vanishing at infinity on $\widehat{G}$.

The Fourier cotransform is a morphism of involutive algebras of $L^1(G)$ into the algebra of bounded continuous functions on $\widehat{G}$ (prop. 3). Since it identifies with the Gelfand transform, its image is contained in $\mathscr{C}_0(\widehat{G})$ (I, p. 37, prop. 5), and its kernel is the radical of $L^1(G)$ (prop. 8 of I, p. 38), which is zero (cor. of prop. 22 of I, p. 126).

We shall see later (corollary to proposition 13 of II, p. 221) that the cotransform of Fourier on $\mathscr{M}^1(G)$ is also injective.

#### Remark {#ts-ii-s1-n2-rem-1 .statement tag=02I4}

The Fourier transform on the space $L^1(G)$ depends on the choice of the Haar measure $dx$, unlike the Fourier transform on $\mathscr{M}^1(G)$. If one replaces $dx$ by the measure $a\cdot dx$ (with $a >0$), then for every integrable function $f$ on G, the Fourier transform of $f$ is $a\widehat{f}$, where $\widehat{f}$ is the Fourier transform defined relative to the measure $dx$.

Consider the stellar algebra Stell(G) of the group G (def. 9 of I, p. 125), and identify $L^1(G)$ with a dense subalgebra of Stell(G) (prop. 22 of I, p. 126).

#### Proposition 5 {#ts-ii-s1-prop-5 .statement tag=02I5}

By continuity, the Fourier transform and the cotransform of Fourier extend uniquely to isomorphisms of stellar algebras of Stell(G) onto $\mathscr{C}_0(\widehat{G})$.

The cotransform of Fourier extends by continuity to a morphism of stellar algebras from Stell(G) into $\mathscr{C}_0(\widehat{G})$. If one identifies $\widehat{G}$ with $\mathsf{X}$(Stell(G)) (cor. 1 of II, p. 204 and prop. 1 of II, p. 202), this extension is the Gelfand transform of Stell(G). By th. 1 of I, p. 108, it is an isomorphism. The assertion concerning the Fourier transform follows from this.

We shall always denote by $\overline{\mathscr{F}}$ and $\mathscr{F}$ the isomorphisms of prop. 5.

#### Corollary {#ts-ii-s1-n2-cor-1 .statement tag=02I6}

The image of $L^1(G)$ under the Fourier transform of G is dense in $\mathscr{C}_0(\widehat{G})$.

Since $L^1(G)$ is dense in Stell(G), this follows from proposition 5.

#### Proposition 6 {#ts-ii-s1-prop-6 .statement tag=02I7}

Suppose that G is compact. The normalized Haar measure $dx$ belongs to $\mathscr{M}^1(G)$, and its Fourier transform is $\varphi_e$, the characteristic function of $\{e\}$.

Let $\chi \in \widehat{G}$. Since $\varepsilon_y*dx=dx$ for every $y\in G$, one has

$$
\mathscr{F}(dx)(\chi ) =\overline{\langle\chi , y\rangle}\mathscr{F}(dx)(\chi )
$$

by formula (11). If $\chi \not= 1$, there exists $y\in G$ such that $\langle \chi , y\rangle  \not= 1$, hence $\mathscr{F}(dx)(\chi ) = 0$. If $\chi = 1$, then $\mathscr{F}(dx)(\chi ) =\int_Gdx= 1$ since the measure $dx$ is normalized.

### 3. The Plancherel theorem

Denote by A(G) the subspace of $L^1(G)$ generated by the functions $f*g$ for $f, g\in L^1(G)\cap L^2(G)$.

#### Proposition 7 {#ts-ii-s1-prop-7 .statement tag=02I8}

The space A(G) is a self-adjoint ideal of $L^1(G)$. It is contained in $L^1(G)\cap L^2(G)$, and in the image of $\mathscr{C}(G)$ in $L^1(G)$.

Let $f\in L^1(G)$. For every $g\in L^2(G)$, one has $f*g\in L^1(G)$ (INT, VIII, §4, n$^o5$, prop. 12). Consequently, the space $L^1(G)\cap L^2(G)$ is an ideal of $L^1(G)$, and the same is true of the space A(G). The ideal A(G) is self-adjoint.

Let $f$ and $g$ be in $L^2(G)$. The convolution product $f*g$ is then the class of the continuous function given by

$$
y\mapsto \int_Gf(yx^{-1})g(x)dx
$$

(INT, VIII, §4, n$^o5$, prop. 15). The second assertion follows.

Since $\chi (f*g) = (\chi f)*(\chi g)$ for $\chi \in \widehat{G},f\in L^1(G)$ and $g\in L^1(G)$ (INT, VIII, §3, No.$^o1$, prop. 6), one has $\chi h\in A(G)$ for every $h\in A(G)$ and $\chi \in \widehat{G}$. Since $\varepsilon_x*f=\boldsymbol{\gamma }(x)f$ and the linear representation $\boldsymbol{\gamma }$ is isometric on $L^p(G)$ for every $p$ (INT, VIII, §2, No.$^o5$, prop. 8), one has $\varepsilon_x*f\in A(G)$ for all $x\in G$ and $f\in A(G)$.

We denote by $\widehat{A}(G)$ the image of A(G) under the Fourier transform. It is a subspace of $\mathscr{C}_0(\widehat{G})$.

#### Proposition 8 {#ts-ii-s1-prop-8 .statement tag=02I9}

There exists a filter basis $\mathfrak{B}$ on $A(G)\cap \mathscr{K}_+(G)$ such that the following conditions are satisfied:

(i) For every element $\varphi$ of a set of $\mathfrak{B}$, one has $\|\varphi \|_1= 1$ and $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$ ;

(ii) One has

lim$_{\varphi ,\mathfrak{B}}\varphi \cdot dx=\varepsilon_e$

in the space $\mathscr{C}'(G)$ of measures with compact support on G endowed with the topology of uniform convergence on compact parts of $\mathscr{C}(G)$ ;

(iii) One has

lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$

for the topology of compact convergence on $\widehat{G}$;

(iv) For $p= 1$ or $p= 2$, and for every $f\in L^p(G)$, one has $\varphi *f\in$ A(G) for every $\varphi$ belonging to a set of $\mathfrak{B}$ and

lim$_{\varphi ,\mathfrak{B}}\varphi *f=f$

in $L^p(G)$.

Let $K_0$ be a fixed compact neighbourhood of $e$ in G. Let $\mathfrak{B}_0$ be a basis of the filter of neighbourhoods of $e$ in G consisting of symmetric compact neighbourhoods contained in $K_0$ (cf. TG, III, p. 4). For K $\in \mathfrak{B}_0$, let $X'_K$ be the set of functions $\psi \in \mathscr{K}_+(G)$ such that Supp$(\psi )\subset K$ and $\int\psi (x)dx= 1$ ; it is nonempty (lemma 1 of II, p. 200). Let $X_K$ be the set of functions $\psi *\psi$ for $\psi \in X'_K$. It is nonempty and contained in $A(G)\cap \mathscr{K}_+(G)$. The set $\mathfrak{B}$ whose elements are the sets $X_K$ for K varying in $\mathfrak{B}_0$ is a filter basis on $A(G)\cap \mathscr{K}_+(G)$. Let us prove that $\mathfrak{B}$ satisfies the required properties.

If $X\in \mathfrak{B}$ and $\varphi \in X$, one has $\|\varphi \|_1=\int_G\varphi (x)dx= 1$, whence $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$, which establishes property (i).

Property (ii) follows from INT, VIII, § 2, No.$^o7$, Corollary 1 to Lemma 4. A compact subset of $\widehat{G}$ is a compact subset of $\mathscr{C}(G)$, hence (ii) implies lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$ for the topology of compact convergence on $\widehat{G}$, that is, (iii).

Finally, let $p= 1$ or $p= 2$. Let $f\in L^p(G)$. We have $\varphi *f\rightarrow f$ in $L^p(G)$ with respect to the filter $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, prop. 20). Moreover, for every K in $\mathfrak{B}_0$ and $\varphi \in X_K$, there exists $\psi \in X'_K$ such that $\varphi =\psi *\psi$, whence $\varphi *f=\psi *(\psi *f)$. We have $\psi \in L^1(G)\cap L^2(G)$ and $\psi *f\in L^1(G)\cap L^2(G)$, hence $\varphi *f\in A(G)$.

#### Corollary 1 {#ts-ii-s1-prop-8-cor-1 .statement tag=02IA}

The space A(G) is dense in $L^1(G)$ and in $L^2(G)$. It is also dense in Stell(G), and its image $\widehat{A}(G)$ under the Fourier transform is dense in $\mathscr{C}_0(\widehat{G})$.

Assertion (iv) of the proposition provides the first assertion. Since $L^1(G)$ is dense in Stell(G), the second follows from it, and the last then follows from Prop. 5 of II, p. 209.

#### Corollary 2 {#ts-ii-s1-prop-8-cor-2 .statement tag=02IB}

For $f\in A(G)$, let $\Omega_f$ be the set of $\chi \in \widehat{G}$ such that $\mathscr{F}(f)(\chi )\not= 0$. The sets $\Omega_f$ form an open covering of $\widehat{G}$.

This follows from the preceding corollary since, for every $\chi \in \widehat{G}$, the mapping $f\mapsto \mathscr{F}(f)(\chi )$ is a nonzero character of $L^1(G)$.

Recall that the left regular representation $\boldsymbol{\gamma }$ of Stell(G) on $L^2(G)$ (cf. I, p. 125, n$^o13$) is denoted by $\boldsymbol{\gamma }(\varphi )f$ = $\varphi *f$ for $\varphi \in$ Stell(G) and $f\in L^2(G)$.

#### Lemma 3 {#ts-ii-s1-lem-3 .statement tag=02IC}

For every $f\in A(G)$, there exists a unique bounded measure $\mu_f$ on $\widehat{G}$ such that

$$
(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )d\mu_f \tag{17}
$$

for every $\varphi \in$ Stell(G).

Moreover, for every $f$ and $g$ in A(G), we have the equality

$$
\mathscr{F}(f)\cdot \mu_g=\mathscr{F}(g)\cdot \mu_f \tag{18}
$$

between the measure with density $\mathscr{F}(f)$ with respect to $\mu_g$ and the measure with density $\mathscr{F}(g)$ with respect to $\mu_f$.

Let $f,g$ be elements of $L^1(G)\cap L^2(G)$. For every $\varphi \in$ Stell(G), one has $\varphi *f\in L^2(G)$ and $\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2($I, p. 126, formula (8)). Moreover, one has $\varphi *(f*g) = (\varphi *f)*g($loc. cit., formula (9)). This latter function belongs to the closure $\mathscr{C}_0(G)$ of $\mathscr{K}(G)$ in $\mathscr{C}(G)$ (INT, VIII, §4, n$^o5$, prop. 15). Moreover, one has

$$
\|\varphi *(f*g)\|_{\infty}\leqslant \|\varphi *f\|_2\|g\|_2\leqslant \|\varphi \|_*\|f\|_2\|g\|_2
$$

Since the functions $f*g$ for $f$ and $g$ in $L^1(G)\cap L^2(G)$ generate A(G), it follows that $\varphi *f\in \mathscr{C}_0(G)$ for all $f\in A(G)$ and $\varphi \in$ Stell(G), and that the mapping $\varphi \mapsto (\varphi *f)(e)$ is a continuous linear form on Stell(G). Since $\mathscr{F}$ is an isomorphism of Stell(G) onto $\mathscr{C}_0(\widehat{G})$ (prop. 5 of II, p. 209), the first assertion follows.

Now let $f$ and $g$ be in A(G). For $\varphi \in L^1(G)$, one has

$$
(\mathscr{F}(f)\cdot \mu_g)(\mathscr{F}(\varphi )) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\mu_g=\int_{\widehat{G}}\mathscr{F}(\varphi *f)d\mu_g
$$

$$
= ((\varphi *f)*g)(e) \tag{19}
$$

Since $(\varphi *f)*g= (\varphi *g)*f$ and since the image of $L^1(G)$ under the Fourier transform is dense in $\mathscr{C}_0(\widehat{G})$ (cor. of II, p. 210), one deduces from formula (19) that formula (18) is satisfied for all $f$ and $g$ in A(G).

#### Lemma 4 {#ts-ii-s1-lem-4 .statement tag=02ID}

There exists a unique measure $\nu$ on $\widehat{G}$ such that

$$
\mu_f=\mathscr{F}(f)\cdot \nu
$$

for every $f\in A(G)$. For $f\in A(G)$, one has $\mathscr{F}(f)\in L^1(\widehat{G}, \nu )\cap L^2(\widehat{G}, \nu )$.

Let $f\in A(G)$. Let $\Omega_f$ denote the open set in $\widehat{G}$ formed by the $\chi \in \widehat{G}$ such that $\mathscr{F}(f)(\chi )\not= 0$. Let $\varphi$ be the characteristic function of $\widehat{G}-\Omega_f$. Then for every $g\in A(G)$, one has

$$
\int_{\widehat{G}}\mathscr{F}(g)d(\varphi \cdot \mu_f) =\int_{\widehat{G}}\varphi \mathscr{F}(f)d\mu_g= 0
$$

in view of formula (18).

By corollary 1 of II, p. 212, the image $\widehat{A}(G)$ of A(G) under the Fourier transform is dense in $\mathscr{C}_0(\widehat{G})$. One then deduces from the preceding formula that $\varphi \cdot \mu_f= 0$, hence that $\mu_f$ is concentrated on $\Omega_f$ (INT, IV, §4, n$^o7$, def. 4). Let $\nu_f$ be the measure on $\Omega_f$ with density $\mathscr{F}(f)^{-1}$ with respect to $\mu_f|\Omega_f$.

The sets $\Omega_f$, for $f\in A(G)$, form an open covering of $\widehat{G}$ (cor. 2). For all $f$ and $g$ in A(G), formula (18) shows that $\nu_f|(\Omega_f\cap \Omega_g) =\nu_g|(\Omega_f\cap \Omega_g)$. Consequently, there exists a unique measure $\nu$ on $\widehat{G}$ such that one has $\nu_f=\nu |\Omega_f$ for every $f\in A(G)$ (INT, III, §2, No.$^o1$, prop. 1).

If $f\in A(G)$, the measures $\mu_f$ and $\mathscr{F}(f)\cdot \nu$ are concentrated on $\Omega_f$, and their restrictions to $\Omega_f$ are equal to $\mathscr{F}(f)\cdot \nu_f$; these measures are therefore equal.

Since $\mu_f$ is a bounded measure, the Fourier transform $\mathscr{F}(f)$ belongs to the space $L^1(\widehat{G}, \nu )$. Since moreover $\mathscr{F}(f)$ belongs to $\mathscr{C}_0(\widehat{G})$, one has also $\mathscr{F}(f)\in L^2(\widehat{G}, \nu )$.

Formula (17) now takes the form, for $\varphi \in$ Stell(G) and $f\in A(G)$: (20) $(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\nu$.

In particular, for $f$ and $g$ in A(G), one has

$$
\int_{\widehat{G}}\mathscr{F}(f)\mathscr{F}(g)d\nu = (f*g)(e) =\int_Gf(x)g(x^{-1})dx \tag{21}
$$

#### Proposition 9 {#ts-ii-s1-prop-9 .statement tag=02IE}

The measure $\nu$ characterized by lemma 4 is a Haar measure on $\widehat{G}$.

Let $\chi \in \widehat{G}$. For $f$ and $g$ in A(G), let us apply formula (21) to $\chi  f$ and $\chi  g$. The right-hand side is unchanged, whence

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\mathscr{F}(\chi  f)\mathscr{F}(\chi  g))
$$

From formulas (12) of II, p. 208 and (13) of II, p. 208, one gets

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\varepsilon_{\chi}*(\mathscr{F}(f)\mathscr{F}(g)))
$$

One then deduces from INT, VIII, §4, No.$^o3$, prop. 7 that

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) = (\varepsilon_{\chi^{-1}}*\nu )(\mathscr{F}(f)\mathscr{F}(g))
$$

that is to say

$$
(\mathscr{F}(f)\cdot \nu )(\mathscr{F}(g)) = (\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu ))(\mathscr{F}(g))
$$

Since the space $\widehat{A}(G)$ is dense in $\mathscr{C}_0(\widehat{G})$ (cor. 1), it follows that one has the equality

$$
\mathscr{F}(f)\cdot \nu =\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu )
$$

The measures $\nu$ and $\varepsilon_{\chi^{-1}}*\nu$ therefore coincide on the open set $\Omega_f$ where $\mathscr{F}(f)$ is not zero. By corollary 2 and INT, III, §2, No.$^o1$, cor. of prop. 1, these measures are therefore equal.

This shows that the measure $\nu$ is proportional to a Haar measure on $\widehat{G}$. Let $f\in A(G)$. Take $g=\widetilde{f}$ in formula (21). It then takes the form

$$
\int_{\widehat{G}}|\mathscr{F}(f)|^2d\nu =\int_G|f|^2dx \tag{22}
$$

which shows that the measure $\nu$ is not zero. The measure $\nu$ is therefore a Haar measure on $\widehat{G}$.

#### Definition 4 {#ts-ii-s1-def-4 .statement tag=02IF}

The Haar measure $\nu$ on $\widehat{G}$ of proposition 9 is called the dual measure of the given Haar measure $dx$ on G.

We shall often denote by $d\chi$ or $d\widehat{x}$ the Haar measure on $\widehat{G}$ which is dual to the Haar measure $dx$.

#### Remark {#ts-ii-s1-n3-rem-3 .statement tag=02IG}

Let $a$ be a real number $>0$. If one replaces $dx$ by the measure $a\cdot dx$, the convolution product of the functions $f$ and $g\in L^1(G)$ is replaced by $a(f*g)$. We have seen (II, p. 209, remark) that $\mathscr{F}(f)$ is replaced by $a\mathscr{F}(f)$. Hence $\mu_f$ is unchanged and $\nu$ is replaced by $a^{-1}\cdot \nu$. In particular, the measure $dx\otimes d\widehat{x}$ on $G\times \widehat{G}$ is independent of the choice of the Haar measure on G.

#### Lemma 5 {#ts-ii-s1-lem-5 .statement tag=02IH}

The space $A(\widehat{G})$ is dense in $L^2(\widehat{G})$.

Let $h$ be an element of $L^2(\widehat{G})$ orthogonal to $\widehat{A}(G)$. For $f$ and $g$ in A(G), one has $\mathscr{F}(f)\cdot \mathscr{F}(g) =\mathscr{F}(f*g)\in \widehat{A}(G)$, hence $h\cdot \overline{\mathscr{F}(f)}$ is orthogonal to $\mathscr{F}(g)$. Thus, for every $f\in A(G)$, the function $h\cdot \mathscr{F}(f)$ is orthogonal to $\widehat{A}(G)$. But $h\cdot \mathscr{F}(f)\in L^1(\widehat{G})$, and $\widehat{A}(G)$ is dense in $\mathscr{C}_0(\widehat{G})$, therefore the measure $h\mathscr{F}(f)\cdot \nu$ is zero, that is to say that $h\mathscr{F}(f)$ is $\nu$-locally negligible (INT, V, §5, n$^o3$, cor. 2 of prop. 3). In particular, $h$ is $\nu$-locally negligible on the set $\Omega_f$ of characters $\chi$ such that $\mathscr{F}(f)(\chi )\not= 0$. By Corollary 2, it follows that $h$ is $\nu$-locally negligible, hence zero since $h$ belongs to $L^2(\widehat{G})$. This concludes the proof.

#### Theorem 1 (Plancherel) {#ts-ii-s1-thm-1 .statement tag=02II}

The restriction of the Fourier transform to the subspace A(G) of $L^2(G)$ extends in a unique way to an isometry Φ of $L^2(G)$ onto $L^2(\widehat{G})$.

Moreover, if $f\in L^1(G)\cap L^2(G)$, its Fourier transform belongs to $L^2(\widehat{G})$ and coincides in $L^2(\widehat{G})$ with $\Phi (f)$.

By formula (22), the restriction of $\mathscr{F}$ to A(G) is an isometry of the subspace A(G) of $L^2(G)$ onto the subspace $\widehat{A}(G)$ of $L^2(\widehat{G})$. Since A(G) is dense in $L^2(G)$ (cor. 1 of II, p. 212), the Fourier transform extends uniquely to an isometry Φ of $L^2(G)$ onto a closed subspace of $L^2(\widehat{G})$. But since its image contains $\widehat{A}(G)$, which is dense in $L^2(\widehat{G})$ (lemma 5), the mapping Φ is surjective.

Let now $f\in L^1(G)\cap L^2(G)$; let us show that its Fourier transform belongs to $L^2(\widehat{G})$. By prop. 8, (iv) of II, p. 211, and the fact that A(G) is an ideal of $L^1(G)$, there exists a filter basis $\mathfrak{B}$ on A(G) which converges to $f$ both in $L^1(G)$ and in $L^2(G)$. We then have

$\Phi (f) =$ lim$_{g,\mathfrak{B}}\Phi (g) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ in $L^2(\widehat{G})$ and $\mathscr{F}(f) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ in $\mathscr{C}_0(\widehat{G})$. There therefore exists a

sequence $(g_n)$ in A(G) such that $\mathscr{F}(g_n)$ converges to $\Phi (f)$ in $L^2(\widehat{G})$ and to $\mathscr{F}(f)$ in $\mathscr{C}_0(\widehat{G})$. By INT, IV, §3, No.$^o4$, th. 3 and cor. 1, we have $\mathscr{F}(f) = \Phi (f)$, and in particular $\mathscr{F}(f)\in L^2(\widehat{G})$. This completes the proving of the theorem.

We still denote by $\mathscr{F}$ the isometry of $L^2(G)$ onto $L^2(\widehat{G})$ defined in theorem 1, and we call it the Fourier transform in $L^2(G)$. Analogously, the inverse Fourier transform admits a unique isometric extension to $L^2(G)$, still called the inverse Fourier transform and denoted by $\overline{\mathscr{F}}$.

#### Corollary {#ts-ii-s1-n3-cor-1 .statement tag=02IJ}

Suppose that G is compact and that $dx$ is the normalized Haar measure on G. Then the family of unitary characters of G is an orthonormal basis of $L^2(G)$.

Since G is compact, the characters of G belong to $L^2(G)$. For $\chi$ and $\xi$ in $\widehat{G}$, we have

$$
\int_G\langle \chi , x\rangle \langle \xi , x\rangle dx=\mathscr{F}_G(dx)(\chi \xi^{-1})
$$

therefore the family of characters of G is orthonormal (prop. 6 of II, p. 210). It is moreover total because the scalar product of $\chi \in \widehat{G}$ and of $f\in L^2(G)$ is equal to $\mathscr{F}_G(f)(\chi )$, and therefore $f$ is orthogonal to $\widehat{G}$ if and only if $\mathscr{F}_G(f)$ is zero in $L^2(\widehat{G})$, if and only if $f$ is zero (th. 1).

#### Remark 1 {#ts-ii-s1-n3-rem-1 .statement tag=02IK}

Certain formulas concerning the Fourier transform on $L^1(G)$ extend to the Fourier transform on $L^2(G)$. In particular, for $f\in L^2(G)$ and $\chi \in \widehat{G}$, we have

$$
\overline{\mathscr{F}}(f) = (\chi \mapsto \mathscr{F}(f)(\chi^{-1})) =\overline{\mathscr{F}(\overline{f})}
$$

$$
\mathscr{F}(\varepsilon_x*f) =\eta (x^{-1})\mathscr{F}(f),\overline{\mathscr{F}}(\varepsilon_x*f) =\eta (x)\mathscr{F}(f)
$$

$$
\mathscr{F}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f),\overline{\mathscr{F}}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f)
$$

If $\sigma$ is an automorphism of G and Δ the module of $\sigma$ (INT, VII, §1, No.$^o4$, def. 4), then for $f\in L^2(G)$, one has

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1}
$$

in $L^2(G)$.

#### Remark 2 {#ts-ii-s1-n3-rem-2 .statement tag=02IL}

The formulas

$$
\|\overline{\mathscr{F}}(f)\|^2=\|f\|^2 \tag{23}
$$

for $f\in L^2(G)$, or else

$$
\int_Gf(x)\overline{g(x)}dx=\int_{\widehat{G}}\mathscr{F}(f)(\chi )\overline{\mathscr{F}(g)(\chi)}d\chi \tag{24}
$$

for $f$ and $g$ in $L^2(G)$, are called "Plancherel formulas".

#### Proposition 10 {#ts-ii-s1-prop-10 .statement tag=02IM}

Let $n\geqslant 0$ be an integer and let $G_1,\cdots ,G_n$ be locally compact commutative groups. Let $\mu_j$, for $1\leqslant j\leqslant n$, be Haar measures on $G_j$. Let G be the product group of the groups $G_j$ for $1\leqslant j\leqslant n$. Let $\beta$ be the isomorphism of $\widehat{G}$ onto $\prod\widehat{G}_j$ of Prop. 2 of II, p. 206. The Haar measure on $\widehat{G}$ dual to the product Haar measure $\mu=\mu_1\otimes  \cdots  \otimes \mu_n$ on G identifies with the product of the Haar measures $\widehat{\mu}_j$.

In fact, for every family $(f_j)$ of non-zero elements of $\mathscr{L}^2(G_j)$, the function $f$ on G defined by $(x_j)\mapsto \prod f_j(x_j)$ belong to $\mathscr{L}^2(G)$, and satisfies

$$
\int_G|f|^2d\mu=\prod_j\int_{G_j}|f_j|^2d\mu_j=\prod_j\int_{\widehat{G}_j}|\mathscr{F}_{G_j}(f)|^2d\widehat{\mu}_j
$$

by the Plancherel formula, which proves that the product Haar measure of the $\widehat{\mu}_j$ identifies with the Haar measure dual to $\mu$.

### 4. The fourier inversion formula

Recall that every element $f$ of A(G) is the class of a unique continuous function (Prop. 7, b) of II, p. 210). For $x\in G$, we denote by $f(x)$ the value of this function at $x$.

#### Proposition 11 {#ts-ii-s1-prop-11 .statement tag=02IN}

Let $f\in A(G)$. Then $\mathscr{F}(f)\in L^1(\widehat{G})$ and, for every $x\in G$, one has

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}(f)(\widehat{x})d\widehat{x} \tag{25}
$$

In other words, for $f\in A(G)$, one has

$$
f=\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))\circ \eta \tag{26}
$$

where $\eta$ denotes the canonical mapping of G into the bidual group $\widehat{\widehat{G}}$.

By Lemma 4 of II, p. 213 and Proposition 9 of II, p. 214, one has $\mathscr{F}(f)\in L^1(\widehat{G})$ for every function $f\in A(G)$. By the Plancherel formula (24), for $f$ and $g$ in $L^2(G)$, one has

$$
(f*\widetilde{g})(e) =\int_{\widehat{G}}\mathscr{F}(f)(\chi )\overline{\mathscr{F}(g)(\chi)}d\widehat{x}(\chi ) \tag{27}
$$

Let $f$ and $g$ be in $L^1(G)\cap L^2(G)$ and let $h=f*\widetilde{g}\in A(G)$. Since the Fourier transform is an involutive morphism, formula (27) is assertion (25) for the function $h$ at the point $x=e$. By linearity, one deduces that formula (25) is valid at the point $x=e$ for every function $h\in A(G)$.

Let $x\in G$ and $h\in A(G)$. Let $h_1=\varepsilon_{x^{-1}}*h$. Then $h_1\in A(G)$ and $h_1(e) =h(x)$. Since moreover $\mathscr{F}(h_1)(\chi ) =\overline{\langle\chi , x\rangle}\mathscr{F}(f)(\chi )$ for every $\chi \in \widehat{G}($cf. formula (11) of II, p. 208), formula (25) for the function $h_1$ at the point $e$ implies formula (25) for $h$ at the point $x$.

#### Lemma 6 {#ts-ii-s1-lem-6 .statement tag=02IO}

Let $\varphi \in L^1(\widehat{G})\cap L^2(\widehat{G})$. Then $f=\overline{\mathscr{F}}_{\widehat{G}}(\varphi )\circ \eta$ belongs to $L^2(G)$ and $\mathscr{F}_G(f) =\varphi$ in $L^2(\widehat{G})$.

The function $f$ is continuous and bounded on G since $\varphi \in L^1(\widehat{G})$. For every function $g\in L^1(G)\cap L^2(G)$, one has

$$
\int_Gg(x)f(x)dx=\int_Gg(x)(\int_{\widehat{G}}\langle \chi , x\rangle \varphi (\chi )d\widehat{x}(\chi ))dx
$$

$$
=\int_{\widehat{G}}\overline{\mathscr{F}}_G(g)(\chi )\varphi (\chi )d\widehat{x}(\chi ) \tag{28}
$$

applying the Lebesgue-Fubini theorem (INT, V, §8, n$^o4$, th. 1, a)) to the function $(x, \chi )\mapsto g(x)\varphi (\chi )\langle \chi , x\rangle$ which is integrable on $G\times \widehat{G}$ with respect to the product measure $dx\otimes d\widehat{x}$. It follows that

$$
|\int_Gg(x)f(x)dx|\leqslant \|\overline{\mathscr{F}}_G(g)\|_2\|\varphi \|_2=\|g\|_2\|\varphi \|_2
$$

by Plancherel's formula. The linear form $g\mapsto \int_Gf g$ is therefore continuous on $L^1(G)\cap L^2(G)$, and since $L^1(G)\cap L^2(G)$ is dense in the Hilbert space $L^2(G)$, it follows that $f$ belongs to $L^2(G)$.

Applying then Theorem 1 of II, p. 215, one obtains on the other hand

$$
\int_Gg(x)f(x)dx=\int_{\widehat{G}}\overline{\mathscr{F}_G(\overline{g})(\chi)}\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\overline{\mathscr{F}}_G(g)(\chi )\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

for every $g\in L^2(G)$. Comparing with (28), one concludes that $\varphi =\mathscr{F}_G(f)$ in $L^2(\widehat{G})$, since A(G) is contained in $L^1(G)\cap L^2(G)$ and $\widehat{A}(G)$ is dense in $L^2(\widehat{G})$ (Lemma 5 of II, p. 215).

Proposition 12 (Fourier inversion formula)

Let $f\in L^2(G)$ be such that $\mathscr{F}_G(f)\in L^1(\widehat{G})$. Then one has $f$ = $\overline{\mathscr{F}}_G(\mathscr{F}_G(f))\circ \eta$ in $L^2(G)$. In other words, for almost every $x\in G$, one has

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}_G(f)(\widehat{x})d\widehat{x}
$$

The function $\varphi =\mathscr{F}_G(f)$ belongs to $L^1(\widehat{G})\cap L^2(\widehat{G})$, and the desired formula is obtained by applying the lemma.

#### Corollary 1 {#ts-ii-s1-lem-6-cor-1 .statement tag=02IP}

For every closed subset P of $\widehat{G}$ and every $\chi \in \widehat{G}$ not belonging to P, there exists a function $f\in L^1(G)$ such that $\mathscr{F}(f)$ is zero on P and non-zero at $\chi$.

Since, by (12), one has $\mathscr{F}(\chi f) =\varepsilon_{\chi}*\mathscr{F}(f)$ for every $\chi \in \widehat{G}$, it is enough to consider the case where $\chi$ is the identity element of $\widehat{G}$.

Let U be a compact symmetric neighbourhood of $e\in \widehat{G}$ such that $U^2\cap P =\emptyset$. Let $\varphi$ be a positive continuous function on $\widehat{G}$, zero outside U and such that $\varphi (e) = 1$. The function $\varphi_1=\varphi *\varphi$ is then zero on P and $\varphi_1(e)>0$. It is enough therefore to prove that $\varphi_1$ belongs to the image of the Fourier transform on $L^1(G)$. Now $\varphi$ and $\varphi_1$ belong to $L^1(\widehat{G})\cap L^2(\widehat{G})$. Put $f=\overline{\mathscr{F}}(\varphi )\circ \eta$ and $f_1=\overline{\mathscr{F}}(\varphi_1)\circ \eta$. Lemma 6 implies that $f$ and $f_1$ belong to $L^2(G)$ and satisfy $\varphi =\mathscr{F}(f)$ and $\varphi_1=\mathscr{F}(f_1)$. Moreover

$$
f_1=\overline{\mathscr{F}}(\varphi *\varphi )\circ \eta = (\overline{\mathscr{F}}(\varphi )\circ \eta )^2=f^2
$$

and therefore $f_1\in L^1(G)$. Thus $\varphi_1=\mathscr{F}(f_1)$ does indeed belong to the image of $L^1(G)$ by the Fourier transform.

#### Corollary 2 {#ts-ii-s1-lem-6-cor-2 .statement tag=02IQ}

The Banach algebra $L^1(G)$ is regular (I, p. 89, def. 1).

By Prop. 1 of I, p. 88 and the identification of the Gelfand transform of $L^1(G)$ with the Fourier cotransform of G, this follows from the preceding corollary.

### 5. The Pontryagin Duality Theorem

#### Theorem 2 (Pontryagin) {#ts-ii-s1-thm-2 .statement tag=02IR}

The canonical mapping $\eta$ of G into $\widehat{\widehat{G}}$ is an isomorphism of topological groups. It transforms the Haar measure $dx$ into the bidual Haar measure $d\widehat{\widehat{x}}$.

Let us first prove that $\eta$ is injective and strict. For this it is enough to show that for every neighbourhood U of $e$ in G, there exists a neighbourhood W of $e$ in $\widehat{\widehat{G}}$ such that $\overset{-1}{\eta}(W)\subset U$ (Lemma 2 of II, p. 200). Now let V be a compact symmetric neighbourhood of $e$ in G such that $V^2\subset U$, let $f$ be a positive continuous function on G, with support contained in V, and such that $f(e)>0$. Let $g=\widetilde{f}*f$. Then $g$ belongs to A(G), its support is contained in U and $g(e)>0$. Moreover, $\mathscr{F}_G(g)\in L^1(\widehat{G})$ by Prop. 11 of II, p. 217. The set W of the $\xi$ in $\widehat{\widehat{G}}$ such that

$$
|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(\xi )-\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(e)|<\frac{1}{2}g(e)
$$

is a neighbourhood of $e$ in $\widehat{\widehat{G}}$ since the function $\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))$ is continuous on $\widehat{\widehat{G}}$. Let $x\in \overset{-1}{\eta}(W)$. By formula (26), we have

$$
\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(\eta (x)) =g(x)
$$

and therefore $|g(x)-g(e)|<\frac{1}{2}g(e)$. This implies that $g(x)\not= 0$ and therefore $x\in U$, since the support of $g$ is contained in U. Thus $\overset{-1}{\eta}(W)\subset U$.

Let us prove that the mapping $\eta$ is surjective. Since this mapping is a homeomorphism onto its image, the group $\eta (G)$ is a locally compact subgroup of $\widehat{\widehat{G}}$. It is therefore closed in $\widehat{\widehat{G}}$ (TG, III, p. 22, Cor. 2). Arguing by contradiction, suppose that there exists a character $\xi \in \widehat{\widehat{G}}$ such that $\xi \notin \eta (G)$. Then there exists (Corollary 1 of II, p. 219) a nonzero element $f$ of $L^1(\widehat{G})$ such that $\mathscr{F}_{\widehat{G}}(f)$ is zero on $\eta (G)$. Let $g\in L^1(G)$. The function $(x, \chi )\mapsto g(x)f(\chi )\langle \chi , x\rangle$ belong to $L^1(G\times \widehat{G})$. By Lebesgue-Fubini's theorem (INT, V, §8, n$^o4$, th. 1, a)), there follows therefore

$$
\int_{\widehat{G}}f(\chi )\mathscr{F}_G(g)(\chi )d\chi =\int_Gg(x)(\int_{\widehat{G}}f(\chi )\overline{\langle\chi , x\rangle}d\chi )dx
$$

$$
=\int_Gg(x)\mathscr{F}_{\widehat{G}}(f)(\eta (x))dx= 0
$$

Since the image of the Fourier transform is dense in $\mathscr{C}_0(\widehat{G})$ (corollary of Prop. 5 of II, p. 209), it follows that the measure $f\cdot d\chi$ is zero. This contradicts the fact that $f\not= 0$ in $L^1(\widehat{G})$, and proves that $\eta$ is surjective.

The image measure $\eta (dx)$ and the measure $\nu$ dual to the measure $d\chi$ are Haar measures on $\widehat{\widehat{G}}$. Let $f$ be a nonzero element of A(G) ; in particular $f\in L^2(G)$. By Prop. 12 of II, p. 219$,\mathscr{F}_G(f)\in L^1(\widehat{G})$ and one has

$$
\int_{\widehat{\widehat{G}}}|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))|^2\eta (dx) =\int_G|f|^2dx=\int_{\widehat{\widehat{G}}}|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))|^2d\nu
$$

where the second equality follows from two applications of the Plancherel formula, hence the Haar measure dual to $d\chi$ is the measure $\eta (dx)$.

Henceforth we shall identify G and $\widehat{\widehat{G}}$ by means of the isomorphism $\eta$. One then has:

#### Corollary {#ts-ii-s1-n5-cor-1 .statement tag=02IS}

The Fourier cotransform of $L^2(\widehat{G})$ onto $L^2(G)$ and the Fourier transform of $L^2(G)$ onto $L^2(\widehat{G})$ are reciprocal isometries of one another.

#### Remark {#ts-ii-s1-n5-rem-1 .statement tag=02IT}

Let $f\in L^2(G)$ and $g\in L^2(\widehat{G})$. Applying the Plancherel formula (24) to $f$ and $\overline{\mathscr{F}_{\widehat{G}}(g)}$, one obtains the formula

$$
\int_Gf(x)\mathscr{F}_{\widehat{G}}(g)(x)dx=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )g(\chi )d\widehat{x}(\chi ) \tag{29}
$$

since one has $\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(g)) =\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\overline{g})) =\overline{g}$.

The Fourier transform and cotransform defined on $\mathscr{M}^1(\widehat{G})$ take their values in the space of bounded continuous functions on G. For $\beta \in \mathscr{M}^1(\widehat{G})$ and $x\in G$, one has

$$
\mathscr{F}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\overline{\langle\chi , x\rangle}d\beta (\chi ),\overline{\mathscr{F}}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\langle \chi , x\rangle d\beta (\chi )
$$

The Fourier transforms of G and $\widehat{G}$ are also transposes of one another. More precisely:

#### Proposition 13 {#ts-ii-s1-prop-13 .statement tag=02IU}

Let $\alpha \in \mathscr{M}^1(G)$ and $\beta \in \mathscr{M}^1(\widehat{G})$. Then one has (30) $\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ) =\beta *\mathscr{F}_G(\alpha )$

and in particular

$$
\int_G\mathscr{F}_{\widehat{G}}(\beta )(x)d\alpha (x) =\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi )d\beta (\chi ) \tag{31}
$$

Formula (30) implies formula (31) by evaluating both sides of the identity at $\chi = 1$. Let us prove (30). Let $\chi \in \widehat{G}$. There follows

$$
(\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_G\overline{\langle\chi , x\rangle}\overline{\mathscr{F}}_{\widehat{G}}(\beta )(x)d\alpha (x)
$$

$$
=\int_G\overline{\langle\chi , x\rangle}(\int_{\widehat{G}}\langle \xi , x\rangle d\beta (\xi ))d\alpha (x)
$$

The function $(x, \xi )\mapsto  \langle \chi , x\rangle \langle \xi , x\rangle$ is continuous and bounded, hence integrable on $G\times \widehat{G}$ with respect to the measure $\alpha \otimes \beta$. By Lebesgue-Fubini's theorem (INT, V, §8, n$^o4$, th. 1, a)), one obtains

$$
(\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_{\widehat{G}}(\int_G\overline{\langle\chi \xi^{-1}, x\rangle}d\alpha (x))d\beta (\xi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi \xi^{-1})d\beta (\xi ) = (\beta *\mathscr{F}_G(\alpha ))(\chi )
$$

as desired.

#### Corollary {#ts-ii-s1-n5-cor-2 .statement tag=02IV}

The Fourier transform $\mathscr{F}_G$ is injective on $\mathscr{M}^1(G)$.

In fact, if $\alpha \in \mathscr{M}^1(G)$ satisfies $\mathscr{F}_G(\alpha ) = 0$, one deduces from (31) that $\alpha (\mathscr{F}_G(f)) = 0$ for every $f\in L^1(\widehat{G})$; since the image of $L^1(\widehat{G})$ under the Fourier tran$\widehat{s}$form is dense in $\mathscr{C}_0(G)$ (corollary to Proposition 5 of II, p. 209), it follows that $\alpha = 0$.

There exist function spaces on G and $\widehat{G}$, other than $L^2(G)$ and $L^2(\widehat{G})$, on which $\mathscr{F}$ and $\overline{\mathscr{F}}$ are inverse isomorphisms of one another. The following theorem gives an example of this. We denote by B(G) the vector subspace of $L^1(G)$ consisting of the elements $f\in L^1(G)$ such that $\mathscr{F}_G(f)\in L^1(\widehat{G})$. This is a subalgebra of $L^1(G)$. In fact, let $f$ and $g$ be in B(G). Then $f*g\in L^1(G)$ and $\mathscr{F}_G(f*g) =\mathscr{F}_G(f)\mathscr{F}_G(g)\in L^1(\widehat{G})$, since $\mathscr{F}_G(f)\in L^1(\widehat{G})$ and $\mathscr{F}_G(g)\in \mathscr{C}_0(\widehat{G})$.

#### Theorem 3 {#ts-ii-s1-thm-3 .statement tag=02IW}

The restriction of the Fourier transform to B(G) induces an isomorphism of vector spaces of B(G) onto $B(\widehat{G})$, whose inverse is induced by the restriction of the co-Fourier transform to $B(\widehat{G})$.

Let $f\in B(G)$. Put $g=\mathscr{F}_G(f)$. Then $g\in L^1(\widehat{G})\cap \mathscr{C}_0(\widehat{G})\subset$ $L^1(\widehat{G})\cap L^2(\widehat{G})$. Put $f_1=\overline{\mathscr{F}}_{\widehat{G}}(g)\in L^2(G)$. For every continuous function with compact support $h\in \mathscr{K}(\widehat{G})$, one has $h\in L^1(\widehat{G})\cap L^2(\widehat{G})$ and

$$
\int_Gf_1(x)\mathscr{F}_{\widehat{G}}(h)(x)dx=\int_G\overline{\mathscr{F}}_{\widehat{G}}(g)(x)\overline{\overline{\mathscr{F}}_{\widehat{G}}(\overline{h})(x)}dx
$$

$$
=\int_{\widehat{G}}g(\chi )h(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )h(\chi )d\widehat{x}(\chi ) =\int_Gf(x)\mathscr{F}_{\widehat{G}}(h)(x)dx
$$

by using the Plancherel theorem and formula (31). Since $\mathscr{K}(\widehat{G})$ is dense in $L^2(\widehat{G})$, its image under the Fourier transform is dense in $L^2(G)$. Consequently, one has $f_1=f$ in $L^1(G)$; this proves that $g\in B(\widehat{G})$.

The formula $f_1=f$ means that the restriction to B(G) of the composition $\overline{\mathscr{F}}_{\widehat{G}}\circ \mathscr{F}_G$ is the identity mapping of B(G). By exchanging the roles of G and $\widehat{G}$, one sees that $\mathscr{F}_G\circ \mathscr{F}_{\widehat{G}}$ is the identity mapping of $B(\widehat{G})$, which completes the proof of the theorem.

#### Corollary 1 {#ts-ii-s1-thm-3-cor-1 .statement tag=02IX}

Let $f\in L^1(G)$. Then $f\in B(G)$ if and only if $f$ belongs to the image of the Fourier transform $\mathscr{F}_{\widehat{G}}$ on $L^1(\widehat{G})$. In particular, one has $A(G)\subset B(G)$.

Theorem 3 proves that if $f\in B(G)$, then $f=\mathscr{F}_{\widehat{G}}(\overline{\mathscr{F}}_G(f))$, where $\mathscr{F}_G(f)$ belong to $L^1(\widehat{G})$. Conversely, if $f=\mathscr{F}_{\widehat{G}}(g)$, where $g\in L^1(\widehat{G})$, then one has $g\in B(\widehat{G})$ and therefore $f\in B(G)$ by the theorem. The last assertion then results from prop. 11 of II, p. 217.

#### Corollary 2 {#ts-ii-s1-thm-3-cor-2 .statement tag=02IY}

The vector space B(G) is an algebra both for multiplication and for convolution. The Fourier transform exchanges convolution and multiplication in B(G) and $B(\widehat{G})$.

We have already seen that B(G) is a subalgebra of $L^1(G)$. On the other hand, if $f$ and $g$ belong to B(G), then $f g\in L^1(G)$ since $f\in L^1(G)$ and $g$ belong to the image of the Fourier transform on $L^1(\widehat{G})$ (Corollary 1). Since there exist $f_1$ and $g_1$ in $L^1(\widehat{G})$ such that $f$ = $\mathscr{F}_{\widehat{G}}(f_1)$ and $g=\mathscr{F}_{\widehat{G}}(g_1)$ (loc. cit.), one has $f g=\mathscr{F}_{\widehat{G}}(f_1*g_1)$, and therefore $f g\in B(G)$ again by the preceding corollary.

#### Proposition 14 {#ts-ii-s1-prop-14 .statement tag=02IZ}

Let $f$ and $g$ be in $L^2(G)$. Then $\mathscr{F}_G(f g) =$ $\mathscr{F}_G(f)*\mathscr{F}_G(g)$.

The equality is true if $f$ and $g$ belong to B(G) (Corollary 2), and in particular if $f$ and $g$ belong to A(G) since $A(G)\subset B(G)$ (Cor. 1). Since A(G) is dense in $L^2(G)$ (Cor. 1 of II, p. 212), it is enough to prove that the two sides of the equality are continuous functions of $(f, g)\in L^2(G)\times L^2(G)$ with values in $\mathscr{C}_0(\widehat{G})$. Now the map $(f, g)\mapsto \mathscr{F}_G(f g)$ is obtained by composing the continuous map $(f, g)\mapsto f g$ of $L^2(G)\times L^2(G)$ into $L^1(G)$ and the Fourier transform $\mathscr{F}_G$ of $L^1(G)$ into $\mathscr{C}_0(\widehat{G})$, which is also continuous. Analogously, the map $(f, g)\mapsto \mathscr{F}_G(f)*\mathscr{F}_G(g)$ is obtained by composing the continuous maps $(f, g)\mapsto (\mathscr{F}_G(f),\mathscr{F}_G(g))$ of $L^2(G)\times L^2(G)$ into $L^2(\widehat{G})\times L^2(\widehat{G})$ and $(h_1, h_2)\mapsto h_1*h_2$ of $L^2(\widehat{G})\times L^2(\widehat{G})$ into $\mathscr{C}_0(\widehat{G})$ (INT, VIII, §4, n$^o5$, prop. 15).

#### Remark {#ts-ii-s1-n5-rem-2 .statement tag=02J0}

See n$^o9$ and exercises 22 of II, p. 270 and 31 of II, p. 275 for other examples of function spaces on which the Fourier transform is an isomorphism, in the case of particular groups G.

### 6. Functorial properties of duality

Let G and H be commutative locally compact groups. Recall that if $\varphi : G\rightarrow H$ is a morphism of topological groups, the dual morphism $\widehat{\varphi}:\widehat{H}\rightarrow \widehat{G}$ is defined by $\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle$ for all $\chi \in \widehat{H}$ and $x\in G$. This definition shows that $\widehat{\widehat{\varphi}}=\varphi$ with the identifications of G (resp. H) and $\widehat{\widehat{G}}$ (resp. $\widehat{\widehat{H}}$) of Theorem 2 of II, p. 220.

Let $\theta$ be a mapping of $G\times H$ into $\mathbf{U}$. For each $x\in G$ (resp. each $y\in H$), let $\theta_x$ (resp. $\theta^y$) be the function from G into $\mathbf{U}$ defined by $y\mapsto$ $\theta (x, y)$ (resp. the function from H into $\mathbf{U}$ defined by $x\mapsto \theta (x, y)$). Suppose that the mapping $\alpha :x\mapsto \theta_x$ is an isomorphism of the topological group G onto the topological group $\widehat{H}$. For every $y\in H$ and $x\in G$, one has

$$
\theta^y(x) =\theta (x, y) =\langle \alpha (x), y\rangle =\langle x,\widehat{\alpha}(y)\rangle
$$

that is, $\theta^y=\widehat{\alpha}(y)$. By Theorem 2 of II, p. 220, the mapping $\beta :y\mapsto \theta^y$ is therefore an isomorphism of the topological group H onto the topological group $\widehat{G}$. Under these conditions, we shall say that $\theta$ puts G and H in duality, or that G and H are in duality relative to $\theta$. We shall then identify each of the groups G and H with the dual of the other. The Haar measure on H obtained by transport of structure from the dual measure of $dx$ will be called the dual measure of the Haar measure $dx$.

#### Lemma 7 {#ts-ii-s1-lem-7 .statement tag=02J1}

Let $(G_i)_{i\in I}$ and $(H_i)_{i\in I}$ be finite families of locally compact topological groups. For $i\in I$, let $\theta_i: G_i\times H_i\rightarrow \mathbf{U}$ be a mapping which puts the groups $G_i$ and $H_i$ in duality. The mapping $\theta$ defined by

$$
\theta ((g_i),(h_i)) =\prod_{i\in I}\theta_i(g_i, h_i)
$$

puts the groups $\prod G_i$ and $\prod H_i$ in duality.

This results from Proposition 2 of II, p. 206 and from the preceding definition.

#### Definition 5 {#ts-ii-s1-def-5 .statement tag=02J2}

Let G, H and K be topological groups. Let $f: H\rightarrow G$ and $g: G\rightarrow K$ be morphisms of topological groups. The pair $(f, g)$ is said to be an exact sequence of topological groups if it is an exact sequence of groups (A, II, p. 10, Remark 5) and if $f$ and $g$ are strict morphisms.

An exact sequence will be represented by the diagram

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

and one will say that a diagram

$$
G_1\longrightarrow^{f_1}G_2\longrightarrow^{f_2}G_3\rightarrow  \cdots  \rightarrow G_n\longrightarrow^{f_n}G_{n+1}
$$

is exact if each pair $(f_i, f_{i+1})$ for $1\leqslant i\leqslant n-1$ is exact.

A sequence

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

is exact if and only if $f$ is a strict injective morphism, $g$ is a strict surjective morphism, and the kernel of $g$ is equal to the image of $f$. If K is separated, the image of $f$ is a closed subgroup of G.

#### Example 1 {#ts-ii-s1-n6-exa-1 .statement tag=02J3}

Let $f: H\rightarrow$ G be a strict injective morphism whose image is a distinguished subgroup. The sequence

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{p}{\longrightarrow}G/f(H)\rightarrow 1
$$

where $p$ is the canonical projection, is exact. In particular, if H is a closed distinguished subgroup of G, the sequence of topological groups

$$
1\rightarrow H\overset{j}{\longrightarrow}G\overset{p}{\longrightarrow}G/H\rightarrow 1
$$

where $j$ is the inclusion and $p$ the canonical projection, is exact.

#### Example 2 {#ts-ii-s1-n6-exa-2 .statement tag=02J4}

Let $g: G\rightarrow K$ be a strict surjective morphism. The sequence

$1\rightarrow$ Ker($g$)$\overset{j}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1$,

where $j$ is the inclusion, is exact

#### Theorem 4 {#ts-ii-s1-thm-4 .statement tag=02J5}

A sequence

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

of commutative locally compact topological groups is exact if, and only if, the dual sequence

$$
\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}
$$

is exact.

We shall begin by proving a few lemmas. It will be noted that each of them is moreover an easy consequence of the assertion of theorem 4.

#### Lemma 8 {#ts-ii-s1-lem-8 .statement tag=02J6}

Let $g: G\rightarrow K$ be a morphism of commutative locally compact topological groups. If the morphism $g$ is surjective and strict, then $\widehat{g}$ is injective and strict.

Since $g$ is surjective, the morphism $\widehat{g}$ is injective (lemma 2 of II, p. 205). To prove that $\widehat{g}$ is a strict morphism, it is enough to prove that for every neighbourhood U of $e$ in $\widehat{K}$, there exists a neighbourhood V of $e$ in $\widehat{G}$ such that $\overset{-1}{\widehat{g}}(V)\subset U$ (lemma 2 of II, p. 200). Let U be such a neighbourhood of $e$ in $\widehat{K}$. By definition of the topology of $\widehat{K}$, there exist a compact subset X of K and a number $\varepsilon  >0$ such that U contains the set of $\widehat{z}\in \widehat{K}$ which, for every $z\in X$, satisfy $|\langle \widehat{z}, z\rangle  -1|< \varepsilon$. Since $g$ is strict and surjective, there exists, by TG, I, p. 80, prop. 10, a compact subset $X_0$ of G such that $g(X_0) = X$. Let V be the neighbourhood of $e$ in $\widehat{G}$ formed by the elements $\chi \in \widehat{G}$ such that,

for every $x\in X_0$, one has $|\langle \chi , x\rangle  -1|< \varepsilon$. One then has $\overset{-1}{\widehat{g}}(V)\subset U$. This proves the assertion.

#### Lemma 9 {#ts-ii-s1-lem-9 .statement tag=02J7}

Let $f: H\rightarrow G$ be a morphism of locally compact topological groups. If the morphism $f$ is injective and strict, then $\widehat{f}$ is surjective and strict.

Suppose that $f$ is injective and strict. The morphism $\widehat{f}$ induces by passing to the quotient a morphism $q:\widehat{G}/$ Ker($\widehat{f}$)$\rightarrow \widehat{H}$. What has to be proved is that this is an isomorphism of topological groups; by duality, it is enough for this to prove that its dual $\widehat{q}$ is an isomorphism.

Let L denote the dual group of $\widehat{G}/$ Ker($\widehat{f}$) and $p:\widehat{G}\rightarrow \widehat{G}/$ Ker($\widehat{f}$) the canonical projection. We shall first prove that $\widehat{p}$ induces, by passing to subspaces, an isomorphism of L onto $f(H)$.

One has $q\circ p=\widehat{f}$, whence $\widehat{p}\circ \widehat{q}=f$. The image of $\widehat{p}$ therefore contains $f(H)$.

Since $f$ is strict, its image $f(H)$ is a locally compact subgroup of G, and is therefore closed (TG, III, p. 22, cor. 2). Let K = $G/f(H)$ and consider the exact sequence

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

associated (Example 1). By duality, the morphism $\widehat{f}\circ \widehat{g}$ is trivial and therefore the image of $\widehat{g}$ is contained in Ker($\widehat{f}$) $=$ Ker($p$). Thus $p\circ \widehat{g}$ is the trivial morphism and, again by duality, $g\circ \widehat{p}$ is also trivial. It follows that the image of $\widehat{p}$ is contained in the kernel of $g$, which is equal to $f(H)$. One concludes that the image of $\widehat{p}$ is equal to $f(H)$.

Moreover, since $p$ is a strict surjective morphism, the dual morphism $\widehat{p}$ is a strict injective morphism of L into G (Lemma 8). It follows that $\widehat{p}$ induces a topological group isomorphism of L onto $f(H)$. Since $\widehat{p}\circ \widehat{q}=f$, and $f$ induces an isomorphism of H onto its image $f(H)$, the morphism $\widehat{q}$ is an isomorphism.

#### Lemma 10 {#ts-ii-s1-lem-10 .statement tag=02J8}

Let

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

be an exact sequence of commutative locally compact groups. The kernel of $\widehat{f}$ is equal to the image of $\widehat{g}$.

The homomorphism $\widehat{f}\circ \widehat{g}$ is trivial by duality, hence the image of $\widehat{g}$ is contained in the kernel of $\widehat{f}$. Conversely, let $\chi$ be in the kernel of $\widehat{f}$. This means that Im($f$) $=$ Ker($g$) is contained in the kernel of $\chi$, hence that there exists a character $\eta$ of Im($g$) such that $\eta \circ g=\chi$. Since the inclusion of Im($g$) into K is strict, the dual restriction mapping of characters of K to Im($g$) is surjective (Lemma 9). There therefore exists a character $\beta$ of K such that $\eta$ is the restriction of $\beta$, and then $\chi =\beta \circ g=\widehat{g}(\beta )$. One concludes that the kernel of $\widehat{f}$ is contained in the image of $\widehat{g}$.

Let us now prove Theorem 4. By duality, it is enough to prove that the sequence $\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}$ is exact when the sequence $H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K$ is so. Now, by Lemmas 8 and 9, the morphisms $\widehat{f}$ and $\widehat{g}$ are strict, and by Lemma 10, the kernel of $\widehat{f}$ is equal to the image of $\widehat{g}$.

#### Corollary 1 {#ts-ii-s1-lem-10-cor-1 .statement tag=02J9}

Let

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

be an exact sequence of commutative locally compact topological groups. The morphism $\widehat{g}$ induces an isomorphism between $\widehat{K}$ and $f(H)^{\bot}$, and $\widehat{f}$ induces by passing to the quotient an isomorphism between $\widehat{G}/f(H)^{\bot}$ and $\widehat{H}$.

By Theorem 4, the sequence

$$
1\rightarrow \widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}\rightarrow 1 \tag{32}
$$

is exact. The morphism $\widehat{g}$ therefore induces an isomorphism of $\widehat{K}$ onto Ker($\widehat{f}$) $=f(H)^{\bot}$ (Lemma 2 of II, p. 205), and $\widehat{f}$ induces by passing to the quotient an isomorphism of $\widehat{G}/Ker(\widehat{f}) =\widehat{G}/f(H)^{\bot}$ onto $\widehat{H}($loc. cit.).

#### Corollary 2 {#ts-ii-s1-lem-10-cor-2 .statement tag=02JA}

Let $f: G\rightarrow H$ be a morphism of locally compact commutative topological groups. The morphism $f$ is strict if and only if $\widehat{f}$ is strict.

In view of the canonical decomposition (E, II, p. 44) of a strict morphism, this follows from Lemmas 8 and 9.

#### Corollary 3 {#ts-ii-s1-lem-10-cor-3 .statement tag=02JB}

Let H be a subgroup of G. Then $(H^{\bot})^{\bot}= H$.

Since $H^{\bot}$ = $\overline{H}^{\bot}$, we may suppose that H is closed. Let $f: H\rightarrow G$ be the canonical injection and $p: G\rightarrow G/H$ the canonical projection. We have $H^{\bot}=$ Ker($\widehat{f}$) (Lemma 10). Let $k$ be the canonical injection of $H^{\bot}$ into $\widehat{G}$. By Theorem 4, the morphism $\widehat{p}$ induces an isomorphism $\widehat{p}_H:\widehat{G}/H\rightarrow H^{\bot}$ of topological groups and we have $k\circ \widehat{p}_H=\widehat{p}$. Consequently (Corollary 1), we obtain

$(H^{\bot})^{\bot}=$ Ker($\widehat{k}$) $=$ Ker( $\widehat{\widehat{p}}_H\circ \widehat{k}$) $=$ Ker($p$) $= H$.

#### Corollary 4 {#ts-ii-s1-lem-10-cor-4 .statement tag=02JC}

Let I be a set and let $(H_i)_{i\in I}$ be a family of closed subgroups of G. The orthogonal of the closed subgroup generated by the $H_i$ is $\bigcap_{i\in I}H^{\bot}_i$. The orthogonal of $\bigcap_iH_i$ is the closed subgroup generated by the subgroups $H^{\bot}_i$.

The first assertion follows from the definition of the orthogonal. Applying this result and Corollary 3 to the family of closed subgroups $(H^{\bot}_i)_{i\in I}$ of $\widehat{G}$, we see that $\bigcap_iH_i$ is the orthogonal of the closed subgroup generated by the subgroups $H^{\bot}_i$, and the second assertion is then obtained by duality.

#### Corollary 5 {#ts-ii-s1-lem-10-cor-5 .statement tag=02JD}

Let $\varphi : G\rightarrow H$ be a morphism of locally compact commutative groups. Then the subgroup Im($\varphi$ ) of H and the subgroup Ker($\widehat{\varphi}$) of $\widehat{H}$ are orthogonal to one another. In particular, in order that $\widehat{\varphi}$ be injective, it is necessary and sufficient that the image of $\varphi$ be dense in H.

We have Ker($\widehat{\varphi}$) $=\varphi (G)^{\bot}$ (Lemma 2 of II, p. 205), whence the result by Corollary 3.

#### Corollary 6 {#ts-ii-s1-lem-10-cor-6 .statement tag=02JE}

Let $k\in \mathbf{Z}$. Then the kernel of the homomorphism $x\mapsto x^k$ of G into G and the closure of the image of the morphism $\chi \mapsto \chi^k$ of $\widehat{G}$ into $\widehat{G}$ are orthogonal to one another.

This follows from the preceding Corollary since the morphisms $x\mapsto x^k$ of G into G and $\chi \mapsto \chi^k$ of $\widehat{G}$ into $\widehat{G}$ are dual to one another.

Recall (A, X, p. 17) that a commutative group A is divisible if, for every nonzero $n\in \mathbf{Z}$, the mapping $a\mapsto a^n$ of A into A is surjective.

#### Corollary 7 {#ts-ii-s1-lem-10-cor-7 .statement tag=02JF}

Let G be a locally compact commutative group.

a) If G is divisible, then the dual group $\widehat{G}$ is torsion-free ;

b) If the dual group $\widehat{G}$ is torsion-free, and if $k\in \mathbf{Z}$ is nonzero, then the image of the homomorphism $x\mapsto x^k$ of G into G is dense in G ;

c) Suppose G discrete or compact. For G to be divisible it is necessary and sufficient that $\widehat{G}$ be torsion-free.

Assertions a) and b) follow from Cor. 6. If G is discrete or compact, the image of the morphism $x\mapsto x^k$ of G into G is closed, and c) follows from a) and b).

#### Remark {#ts-ii-s1-n6-rem-1 .statement tag=02JG}

There exist commutative locally compact groups G which are not divisible and such that $\widehat{G}$ is torsion-free (Exercise 63 of II, p. 299).

### 7. The Poisson formula

In this No., we consider a closed subgroup H of G. We denote by $\beta =dx$ the Haar measure on G and by $\widehat{\beta}$ the dual Haar measure on $\widehat{G}$. We denote by $\alpha$ a Haar measure on H and by $\widehat{\alpha}$ the dual Haar measure on the dual group $\widehat{H}$, which is identified with $\widehat{G}/H^{\bot}$ (Theorem 4 of II, p. 226). We also identify $\widehat{G}/H$ with $H^{\bot}$ by the dual mapping of the canonical projection $G\rightarrow G/H$ (loc. cit.).

We shall denote by $\dot{x}$ the canonical image of an element $x$ of G in $G/H$ and by $\dot{\chi}$ the canonical image of an element $\chi$ of $\widehat{G}$ in $\widehat{G}/H^{\bot}$.

We denote by $\gamma$ the Haar measure $\beta /\alpha$ on $G/H$ (INT, VII, §2, n$^o2$, Def. 1 and n$^o7$, Prop. 10), and by $\widehat{\gamma}$ the dual Haar measure on $H^{\bot}$. Recall (INT, VII, §2, n$^o3$, Prop. 5, c)) that the measure $\gamma$ is characterised by the following property: for every $f\in \mathscr{L}^1(G)$, the function $y\mapsto f(xy)$ on H is $\alpha$-integrable for $\beta$-almost every $x\in G$ ; its integral depends only on $\dot{x}$ and the function defined $\gamma$-almost everywhere on $G/H$ by

$$
f^{\flat}: \dot{x}\mapsto \int_Hf(xh)d\alpha (h)
$$

belongs to $L^1(G/H, \gamma )$ and satisfies

$$
\int_{G/H}f^{\flat}d\gamma =\int_Gf d\beta \tag{33}
$$

#### Proposition 15 {#ts-ii-s1-prop-15 .statement tag=02JH}

Let $f\in L^1(G)$ be such that the restriction to $H^{\bot}$ of the continuous function $\mathscr{F}_G(f)$ is integrable with respect to $\widehat{\gamma}$. Then, for almost every $x\in G$, the function $y\mapsto f(xy)$ on H is $\alpha$-integrable, and one has:

$$
\int_Hf(xy)d\alpha (y) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

From the above, the function $f^{\flat}$ defined almost everywhere on $G/H$ by

$$
f^{\flat}( \dot{x}) =\int_Hf(xy)d\alpha (y)
$$

belongs to $L^1(G/H)$. The Fourier transform of $f^{\flat}$ is identified with the function on $H^{\bot}=\widehat{G}/H$ given for $\chi \in H^{\bot}$ by

$$
\mathscr{F}_{G/H}(f^{\flat})(\chi ) =\int_{G/H}\overline{\langle\chi ,\dot{x}\rangle}f^{\flat}( \dot{x})d\gamma ( \dot{x})
$$

$$
=\int_G\overline{\langle\chi , x\rangle}f(x)d\beta (x) =\mathscr{F}_G(f)(\chi )
$$

by formula (33), applied to the integrable function $x\mapsto$ $\overline{\langle\chi , x\rangle}f(x)$. By hypothesis, the function $\mathscr{F}(f)|H^{\bot}=\mathscr{F}_{G/H}(f^{\flat})$ belong to $L^1(H^{\bot})$, and therefore the function $f^{\flat}$ belong to the space $B(G/H)$. It follows (Theorem 3 of II, p. 222) that $f^{\flat}$ coincides almost everywhere with $\overline{\mathscr{F}}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$. For almost all $\dot{x}\in G/H$, one therefore has

$$
f^{\flat}( \dot{x}) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_{G/H}(f^{\flat})(\chi )d\widehat{\gamma}(\chi ) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

This completes the proof.

#### Corollary (Poisson Formula) {#ts-ii-s1-n7-cor-1 .statement tag=02JI}

Let $f\in \mathscr{L}^1(G)$. Suppose that the following conditions are satisfied:

(i) The restriction of $\mathscr{F}_G(f)$ to $H^{\bot}$ is integrable;

(ii) For every $x\in G$, the function $y\mapsto f(xy)$ on H is integrable;

(iii) The mapping $x\mapsto \int_Hf(xy)d\alpha (y)$ is continuous on G.

Then one has

$$
\int_Hf(y)d\alpha (y) =\int_{H^{\bot}}\mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi ) \tag{34}
$$

Indeed, with the notation of the proof of the preceding proposition, the functions $f^{\flat}$ and $\overline{\mathscr{F}}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$ on $G/H$ are continuous and equal almost everywhere. They are therefore equal everywhere and in particular at $e$, which gives formula (34).

#### Proposition 16 {#ts-ii-s1-prop-16 .statement tag=02JJ}

The measure $\widehat{\alpha}$ on $\widehat{H} =\widehat{G}/H^{\bot}$ is equal to $\widehat{\beta /}\widehat{\gamma}$.

Let us fix a nonzero $f\in \mathscr{K}(G)$. For $x\in G$ and $\chi \in \widehat{G}$, put

$$
\varphi (x, \chi ) =\int_Hf(xy)\langle \chi , y\rangle d\alpha (y)
$$

The function $\varphi$ is continuous on $G\times \widehat{G}$ (INT, IV, §4, n$^o3$, cor. 1 of Theorem 2). For fixed $x$, $\varphi (x, \chi )$ depends only on the class of $\chi$ in $\widehat{G}/H^{\bot}=\widehat{H}$. For fixed $\chi$, $\langle \chi , x\rangle \varphi (x, \chi )$ depends only on the class of $x$ in $G/H$, and the function $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ on $G/H$ has compact support.

Let $x\in G$. The function $\dot{\chi}\mapsto \varphi (x, \chi )$ on $\widehat{H}$ is the Fourier cotransform of the function $y\mapsto f(xy)$ on H. The latter is square-integrable, hence by the Plancherel formula (23) of II, p. 217, one has

$$
\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi}) =\int_H|f(xy)|^2d\alpha (y) \tag{35}
$$

Let $\chi \in \widehat{G}$. The function $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ belongs to $\mathscr{K}(G/H)$, hence to $L^1(G/H)$. Its Fourier cotransform is the function on $H^{\bot}$ whose value at $\xi \in H^{\bot}$ is

$$
\int_{G/H}\langle \xi ,\dot{x}\rangle \langle \chi , x\rangle \varphi (x, \chi )d\gamma ( \dot{x}) =\int_{G/H}(\int_H\langle \chi \xi , xy\rangle f(xy)d\alpha (y))d\gamma ( \dot{x})
$$

$$
=\int_G\langle \chi \xi , x\rangle f(x)d\beta (x) =\overline{\mathscr{F}}_G(f)(\chi \xi )
$$

by formula (33). Therefore

$$
\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x}) =\int_{H^{\bot}}|\overline{\mathscr{F}}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi ) \tag{36}
$$

by the Plancherel formula again.

One then finally computes

$\int_{\widehat{G}}|\overline{\mathscr{F}}_G(f)|^2d\widehat{\beta}=\int_G|f|^2d\beta$ (by (23))

$=\int_{G/H}d\gamma ( \dot{x})\int_H|f(xy)|^2d\alpha (y)$ (by (33))

$=\int_{G/H}d\gamma ( \dot{x})\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi})$ (by (35))

$$
=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x})
$$

$=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{H^{\bot}}|\overline{\mathscr{F}}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi )$ (by (36)),

where INT, V, §8, No.$^o3$, prop. 5 has been applied to the positive continuous function $( \dot{x},\dot{\chi})\mapsto  |\varphi (x, \chi )|^2$ on $G/H\times \widehat{G}/H^{\bot}$.

Comparing this equality with the integration formula (33) for the group $\widehat{G}$, one then concludes that the Haar measures $\widehat{\alpha}$ and $\widehat{\beta /}\widehat{\gamma}$ coincide.

### 8. Examples of duality

#### Proposition 17 {#ts-ii-s1-prop-17 .statement tag=02JK}

Let $n\geqslant 1$ be an integer. Let us denote by $\boldsymbol{\mu}_n$ the group of $n$-th roots of unity in $\mathbf{C}$. The groups $\mathbf{Z}/n\mathbf{Z}$ and $\boldsymbol{\mu}_n$ are in duality relative to the mapping induced by passing to the quotient from the mapping $\mathbf{Z}\times \boldsymbol{\mu}_n\rightarrow \mathbf{U}$ defined by $(m, z)\mapsto z^m$.

The group $\mathbf{Z}\widehat{/n}\mathbf{Z}$ coincides with the set of homomorphisms $\chi$ of $\mathbf{Z}/n\mathbf{Z}$ into $\mathbf{U}$. These are of the form $m\mapsto \chi (1)^m$, where $\chi (1)$ is an arbitrary element of $\mathbf{U}$ such that $\chi (1)^n= 1$, whence the result.

#### Corollary 1 {#ts-ii-s1-prop-17-cor-1 .statement tag=02JL}

Let G be a finite commutative group. The dual group $\widehat{G}$ is isomorphic to G.

The group G is isomorphic to a finite product of cyclic groups (A, VII, p. 22, th. 3), and its dual group is isomorphic to the product of the dual groups of these (prop. 2 of II, p. 206). One is therefore reduced to the case where G is cyclic, which comes under proposition 17 since the group $\boldsymbol{\mu}_n$ is cyclic of order $n$ (A, V, p. 75, th. 1).

#### Corollary 2 {#ts-ii-s1-prop-17-cor-2 .statement tag=02JM}

Let G be a locally compact commutative group. The group G is finite if and only if $\widehat{G}$ is finite. A closed subgroup H of G is of finite index if and only if its orthogonal is finite.

By duality, the first assertion follows from the fact that the dual of a finite group is finite (corollary 1). The second results from it, since $\widehat{G}/H$ is identified with $H^{\bot}$ (th. 4 of II, p. 226).

#### Proposition 18 {#ts-ii-s1-prop-18 .statement tag=02JN}

In order that $\widehat{G}$ be compact, it is necessary and sufficient that G be discrete. If G is discrete, the dual measure of the counting measure on G is the normalised Haar measure on $\widehat{G}$. If G is compact, the dual measure of the normalised Haar measure is the counting measure on $\widehat{G}$.

Suppose G discrete, and let $\alpha$ be the counting measure on G. Let $\varphi$ be the characteristic function of $e\in G$. One has $\mathscr{F}_G(\varphi ) = 1$ on $\widehat{G}$. Since $\mathscr{F}_G(\varphi )$ tends to 0 at infinity, the group $\widehat{G}$ is compact.

Moreover, for the dual measure $\widehat{\alpha}$ of $\alpha$, the function $\mathscr{F}_G(\varphi )$ must have integral $\varphi (e) = 1$ (prop. 12 of II, p. 219). Hence $\widehat{\alpha}(\widehat{G}) = 1$.

Suppose G compact. Then the Haar measure $dx$ belong to $\mathscr{M}^1(G)$. Its Fourier transform is strictly positive at $\chi =e$ and zero for $\chi \not= 0$ (prop. 6 of II, p. 210). Since it is continuous on $\widehat{G}$, the group $\widehat{G}$ is discrete. If the measure of G is 1, one deduces by duality from the preceding case that the dual measure of the measure $dx$ is the counting measure on $\widehat{G}$.

#### Corollary 1 (Orthogonality relations) {#ts-ii-s1-prop-18-cor-1 .statement tag=02JO}

Suppose G discrete and endowed with the counting measure. For $x$ and $y$ in G, one has

$\int$ 0 if $x\not=y$

$$
\chi (x)\chi (y)d\chi =
$$

$_{\widehat{G}}$ 1 if $x=y$.

This results from the cor. to th. 1 of II, p. 215 and from duality.

#### Corollary 2 {#ts-ii-s1-prop-18-cor-2 .statement tag=02JP}

Let H be a closed subgroup of G.

a) In order that H be compact, it is necessary and sufficient that $H^{\bot}$ be open in $\widehat{G}$ ;

b) In order that H be open, it is necessary and sufficient that $H^{\bot}$ be compact in $\widehat{G}$.

a) To say that $H^{\bot}$ is open amounts to saying that $\widehat{G}/H^{\bot}$ is discrete, now $\widehat{G}/H^{\bot}$ is isomorphic to $\widehat{H}$ (Theorem 4 of II, p. 226); the assertion therefore follows from Proposition 18. Assertion b) results by duality from assertion a) applied to $H^{\bot}$.

#### Corollary 3 {#ts-ii-s1-prop-18-cor-3 .statement tag=02JQ}

Let $(H_i)_{i\in I}$ be a decreasing filtered family of compact subgroups of G. In order that G be identified with the projective limit of the groups $G/H_i$, it is necessary and sufficient that $\widehat{G}$ be the union of the open subgroups $H^{\bot}_i$.

To say that G is identified with the projective limit of the $G/H_i$ amounts to saying that $\bigcap_iH_i=\{e\}$ (TG, III, p. 60, Proposition 2), that is, that $\bigcup_iH^{\bot}_i$ is dense in $\widehat{G}$ (Corollary 4 of Theorem 4 of II, p. 226). Now $\bigcup_iH^{\bot}_i$ is an open subgroup, hence closed, of $\widehat{G}$.

#### Corollary 4 {#ts-ii-s1-prop-18-cor-4 .statement tag=02JR}

Let I be a set and let $(H_i)_{i\in I}$ be a family of compact groups. The dual of the product group of the $H_i$ is the discrete direct sum group of the groups $\widehat{H}_i$.

This is a particular case of Corollary 3.

#### Proposition 19 {#ts-ii-s1-prop-19 .statement tag=02JS}

Let K be a locally compact non-discrete field, not necessarily commutative, and let G be the additive group of K, whose group law is denoted additively. Let $\chi$ be a unitary character of G distinct from 1. For $x, y\in G$, put $\theta (x, y) =\chi (xy)$. Then G is in duality with itself relative to $\theta$.

For $y\in G$, let $\chi_y$ be the mapping of G into $\mathbf{U}$ such that $\chi_y(x) =$ $\chi (xy)$. We have $\chi_y\in \widehat{G}$, and it is necessary to prove that $\beta :y\mapsto \chi_y$ is an isomorphism of topological groups of G onto $\widehat{G}$.

The map $\beta$ is an injective homomorphism of G into $\widehat{G}$; it is continuous (TG, X, p. 28, Theorem 3 applied to the continuous map $\theta$ of $G\times G$ into $\mathbf{C}$). Let us prove that $\theta$ is a homeomorphism onto its image. It is enough (Lemma 2 of II, p. 200) to prove that for every neighbourhood U of 0 in K, there exists a neighbourhood V of $e$ in $\widehat{G}$ such that $\overset{-1}{\beta}(V)\subset U$. Let $x\mapsto  |x|$ be an absolute value on K defining the topology of K (AC, VI, §9, No$^o1$, Proposition 1), and let $x_0\in K$ be such that $\chi (x_0)\not= 1$; let us set $\eta =|\chi (x_0)-1|>0$. Let U be a neighbourhood of 0 in K. There exists $\delta  >0$ such that U contains the set of $y\in K$ such that $|y|< \delta$. Let V be the set of characters $\xi \in \widehat{G}$ such that $|\langle \xi , x\rangle  -1|< \eta$ for every element $x\in K$ satisfying $|x|\leqslant |x_0|/\delta$. This is a neighbourhood of $e$ in $\widehat{G}$. If $y\not= 0$ is such that $\beta (y)$ belongs to V, we therefore have $|\chi (xy)-1|<|\chi (x_0)-1|$ for every $x$ such that $|x|\leqslant |x_0|/\delta$. Consequently, we have $|x_0y^{-1}|>|x_0|/\delta$, and therefore $|y|< \delta$, so that $y\in U$.

Since $\beta$ is a homeomorphism onto its image, the latter is closed in $\widehat{G}$ (TG, III, p. 22, Corollary 2). But moreover the orthogonal of the image of $\beta$ is the set of elements $x$ of G such that $\chi (xy) = 1$ for all $y\in G$, and is therefore reduced to $\{0\}$. The image of $\beta$ is therefore dense in $\widehat{G}$ (Corollary 3 of II, p. 228). We conclude that $\beta$ is surjective.

#### Corollary 1 {#ts-ii-s1-prop-19-cor-1 .statement tag=02JT}

Let K be a locally compact non-discrete field not necessarily commutative and $\chi$ a nontrivial unitary character of the additive group of K. Let E be a finite-dimensional topological vector space over K. The map $\theta$ of $E\times E'$ into $\mathbf{U}$ defined by $\theta (x, \lambda ) =\chi (\langle \lambda , x\rangle )$ for $(\lambda , x)\in E'\times E$ puts the topological groups E and $E'$ in duality.

Let $n$ be the dimension of E and $(e_1, . . . , e_n)$ a basis of E. It makes it possible to identify E and $K^n$ (EVT, I, p. 14, Theorem 2). The result then follows from Proposition 19 and Proposition 2 of II, p. 206.

We denote by $\mathbf{T}$ the group $\mathbf{R}/\mathbf{Z}$.

#### Corollary 2 {#ts-ii-s1-prop-19-cor-2 .statement tag=02JU}

a) The group $\mathbf{R}$ is in duality with itself relative to the map $(x, y)\mapsto$ exp(2$i\pi xy$), and the dual measure of Lebesgue measure is Lebesgue measure ;

b) The groups $\mathbf{Z}$ and $\mathbf{T}$ are in duality with respect to the mapping obtained by passing to the quotient from the mapping of $\mathbf{Z}\times \mathbf{R}$ into $\mathbf{U}$ such that $(n, x)\mapsto$ exp(2$i\pi nx$). The dual Haar measure of the counting measure on $\mathbf{Z}$ is the normalised Haar measure on $\mathbf{R}/\mathbf{Z}$.

The group $\mathbf{R}$ is in duality with itself with respect to the mapping $(x, y)\mapsto$ exp(2$i\pi xy$), by Proposition 19. Let us identify $\widehat{\mathbf{R}}$ with $\mathbf{R}$. The orthogonal of $\mathbf{Z}$ in $\widehat{\mathbf{R}}=\mathbf{R}$ is then $\mathbf{Z}$, and b) results from Theorem 4 of II, p. 226.

Let $\alpha$ be the counting measure on $\mathbf{Z}$ and $\gamma$ the normalised Haar measure on $\mathbf{T}$. If $\beta$ denotes Lebesgue measure on $\mathbf{R}$, one has $\gamma =\beta /\alpha$, since these two Haar measures on $\mathbf{R}/\mathbf{Z}$ have mass 1. The Haar measure $\widehat{\alpha}$ on $\widehat{\mathbf{Z}}=\mathbf{T}$ is the normalised Haar measure (Proposition 18), and the Haar measure $\widehat{\gamma}$ is the counting measure on $\mathbf{Z}($loc. cit.). By Proposition 16 of II, p. 231, the dual measure of $\beta$ is therefore the measure $\beta$.

#### Remark {#ts-ii-s1-n8-rem-1 .statement tag=02JV}

In particular one recovers the determination of $\mathsf{X}(L^1(\mathbf{Z}))$ given in Example 4 of I, p. 36.

For every integer $n\geqslant 0$ and $(x, y)\in \mathbf{R}^n\times \mathbf{R}^n$, we write

$$
x\cdot y=\sum_{j=1}^nx_jy_j
$$

#### Corollary 3 {#ts-ii-s1-prop-19-cor-3 .statement tag=02JW}

Let $n\geqslant 1$ be an integer. The group $\mathbf{R}^n$ is in duality with itself with respect to the mapping $(x, y)\mapsto$ exp(2$i\pi  x\cdot y$), and the dual measure of Lebesgue measure on $\mathbf{R}^n$ is Lebesgue measure. The groups $\mathbf{Z}^n$ and $\mathbf{T}^n=\mathbf{R}^n/\mathbf{Z}^n$ are in duality with respect to the mapping obtained by passing to the quotient from the mapping $(n, x)\mapsto$ exp(2$i\pi  x\cdot y$), and the dual Haar measure of the counting measure on $\mathbf{Z}^n$ is the normalised Haar measure on $(\mathbf{R}/\mathbf{Z})^n$.

This results from Lemma 7 of II, p. 225, Proposition 10 of II, p. 217 and Corollary 2.

#### Remark {#ts-ii-s1-n8-rem-2 .statement tag=02JX}

Given a subgroup H of $\mathbf{R}^n$, there corresponds to it its orthogonal $H^{\bot}$, a subgroup of $\widehat{\mathbf{R}}^n=\mathbf{R}^n$, which is none other than the subgroup associated with H defined in TG, VII, p. 6, n$^o3$.

In the sequel, one will identify the dual of $\mathbf{R}^n$ (resp. of $\mathbf{T}^n$) with $\mathbf{R}^n$ (resp. with $\mathbf{Z}^n$) by the duality of the corollary. In particular, for $f\in L^1(\mathbf{R}^n)$, its Fourier transform is identified with the function from $\mathbf{R}^n$ into $\mathbf{C}$ which to $y\in \mathbf{R}^n$ associates

$\mathscr{F}(f)(y) =\int_{\mathbf{R}^n}f(x)$ exp($-2i\pi  x\cdot y$)$dx$.

#### Corollary 4 {#ts-ii-s1-prop-19-cor-4 .statement tag=02JY}

The group $\mathbf{R}^*$ is in duality with the group $\{-1,1\} \times \mathbf{R}$ by the mapping $(x,(\sigma , t))\mapsto \sigma (x/|x|)|x|^{it}$. The group $\mathbf{R}^*_+$ is in duality with $\mathbf{R}$ by the mapping $(x, t)\mapsto x^{it}$.

In fact, the mapping $x\mapsto (x/|x|$, log($|x|$)) is a topological group isomorphism of $\mathbf{R}^*$ onto $\{-1,1\} \times \mathbf{R}$. The assertion then follows from lemma 7 of II, p. 225, from corollary 2, and from the fact that the unitary characters of $\{-1,1\}$ are 1 and $x\mapsto x$.

Let $p$ be a prime number. The field $\mathbf{Q}_p$ of $p$-adic numbers is the completion of $\mathbf{Q}$ for the $p$-adic valuation (INT, VII, § 1, No.$^o6$, example, and AC, VI, § 3, No.$^o4$, example 4). For every $x\in \mathbf{Q}_p$, there exist a unique integer $\nu \geqslant 0$ and a unique integer $q$ satisfying $0\leqslant q < p^{\nu}$ such that $qp^{-\nu}-x\in \mathbf{Z}_p$ (A, VII, p. 10, Theorem 2, applied to the principal ideal domain $\mathbf{Z}_p$ and to the set $R_p$ of integers $j$ such that $0\leqslant j < p$). We put $\lambda (x) =qp^{-\nu}$.

#### Proposition 20 {#ts-ii-s1-prop-20 .statement tag=02JZ}

The mapping $x\mapsto$ exp(2$i\pi \lambda (x)$) is a unitary character of $\mathbf{Q}_p$ whose kernel is $\mathbf{Z}_p$.

For $x_1$ and $x_2$ in $\mathbf{Q}_p$, one has by definition $\lambda (x_1+x_2)-\lambda (x_1)-\lambda (x_2)\in$ $\mathbf{Z}_p\cap \mathbf{Q}=\mathbf{Z}$. The mapping $\lambda$ is moreover locally constant since $\lambda (x+y) =\lambda (x)$ if $y\in \mathbf{Z}_p$. It then follows that $x\mapsto$ exp(2$i\pi \lambda (x)$) is a unitary character of $\mathbf{Q}_p$. Since $\lambda (x)\in \mathbf{Z}$ if and only if $x\in \mathbf{Z}_p$, the kernel of this character is $\mathbf{Z}_p$.

We recall that the normalised Haar measure on the additive group of $\mathbf{Q}_p$ is the unique Haar measure $\mu$ such that $\mu(\mathbf{Z}_p) = 1$ (INT, VII, §1, No.$^o6$, example).

#### Corollary {#ts-ii-s1-n8-cor-1 .statement tag=02K0}

a) The group $\mathbf{Q}_p$ is in duality with itself with respect to the mapping $(x, y)\mapsto$ exp(2$i\pi \lambda (xy)$). The normalised Haar measure on $\mathbf{Q}_p$ is then its own dual ;

b) The groups $\mathbf{Z}_p$ and $\mathbf{Q}_p/\mathbf{Z}_p$ are in duality relative to the mapping obtained by passing to the quotient from the mapping defined by $(z, x)\mapsto$ exp(2$i\pi \lambda (zx)$), and the dual measure of the normalized Haar measure on $\mathbf{Z}_p$ is the counting measure on $\mathbf{Q}_p/\mathbf{Z}_p$.

The proof follows step by step that of Cor. 2 of Prop. 19.

### 9. Euclidean Fourier Transform and Fourier Series

$*$ Let $n\in \mathbf{N}$. We identify $\mathbf{R}^n$ with its dual as in Cor. 3 of II, p. 236. The dual measure of the Lebesgue measure is then the Lebesgue measure. We endow $\mathbf{R}^n$ with the euclidean norm. For every multi-index $\alpha \in \mathbf{N}^n$, and every $x= (x_1, . . . , x_n)\in \mathbf{R}^n$, we write $x^{\alpha}=x^{\alpha_1}_1\cdots x^{\alpha_n}_n$, and we denote by $X^{\alpha}$ the function $x\mapsto x^{\alpha}$ on $\mathbf{R}^n$.

Let $m\in \mathbf{R}^m$. Every continuous morphism of commutative groups from $\mathbf{R}^m$ into $\mathbf{R}^n$ is a linear mapping $\sigma \in \mathscr{L}(\mathbf{R}^n,\mathbf{R}^m)$ (TG, VII, p. 11, Prop. 1). The dual morphism $\widehat{\sigma}$ is identified with the linear mapping $^t\sigma$.

The Fourier transform on $\mathbf{R}^n$ takes a particularly convenient form in the setting of the space of Schwartz functions and of its dual (IV, to appear). We summarize here its principal results.

Let $\mathscr{S}(\mathbf{R}^n)$ be the space of indefinitely differentiable complex-valued functions $\varphi$ on $\mathbf{R}^n$ such that, for every multi-index $\alpha \in \mathbf{N}^n$ and every integer $k\in \mathbf{N}$, the function

$$
x\mapsto  \|x\|^k\partial^{\alpha}\varphi (x)
$$

is bounded on $\mathbf{R}^n$. We endow $\mathscr{S}(\mathbf{R}^n)$ with the locally convex topology defined by the seminorms

$p_{k,\alpha}:\varphi \mapsto$ sup$_{x\in\mathbf{R}^n}\|x\|^k|\partial^{\alpha}\varphi (x)|$.

One says that $\mathscr{S}(\mathbf{R}^n)$ is the space of Schwartz functions on $\mathbf{R}^n$.

For every $\alpha \in \mathbf{N}^n$, the mappings $\varphi \mapsto \partial^{\alpha}\varphi$ and $\varphi \mapsto X^{\alpha}\varphi$ are continuous from $\mathscr{S}(\mathbf{R}^n)$ into itself. The space $\mathscr{S}(\mathbf{R}^n)$ is a topological algebra; it is a Fréchet space and a Montel space (TVS IV, p. 18, Def. 4). For every $p\in [1,+\infty ]$, the space $\mathscr{S}(\mathbf{R}^n)$ is contained in $\mathscr{L}^p(\mathbf{R}^n)$ and the canonical injection of $\mathscr{S}(\mathbf{R}^n)$ into $\mathscr{L}^p(\mathbf{R}^n)$ is continuous. The image of $\mathscr{S}(\mathbf{R}^n)$ in $L^p(\mathbf{R}^n)$ is dense if $p\not= +\infty$.

Since every Schwartz function $\varphi$ is integrable on $\mathbf{R}^n$, it admits a Fourier transform denoted by $\widehat{\varphi}$ which is identified with the continuous function on $\mathbf{R}^n$ defined by

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$dx$.

The Fourier cotransform of $\varphi$ is, for its part, identified with the continuous function defined by

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y$)$dx$.

Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Let $\alpha \in \mathbf{N}^n$ be a multi-index. One has

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

#### Proposition 21 {#ts-ii-s1-prop-21 .statement tag=02K1}

The restriction of the Fourier transform to $\mathscr{S}(\mathbf{R}^n)$ is an automorphism of topological vector spaces whose inverse is the restriction of the Fourier cotransform.

Let $\Lambda \subset \mathbf{R}^n$ be a lattice (TG, VII, p. 4), and let $\Lambda^*\subset \mathbf{R}^n$ be the associated lattice (TG, VII, p. 6), also sometimes called the dual lattice.

The covolume of the lattice Λ is, by definition, the measure of $\mathbf{R}^n/\Lambda$ for the Haar measure induced by Lebesgue measure on $\mathbf{R}^n($cf. INT, VIII, §5, n$^o5$, example), and is denoted by V(Λ). For every function $f\in$ $\mathscr{S}(\mathbf{R}^n)$ and every $y\in \mathbf{R}^n$, one has the Poisson formula

1

$\sum f(x+y) =\sum\widehat{f}(z)$ exp(2$i\pi  y\cdot z$).

V(Λ) $_*$

$x\in \Lambda z\in \Lambda$

#### Remark 1 {#ts-ii-s1-n9-rem-1 .statement tag=02K2}

More generally, by the corollary to proposition 15 of II, p. 230, this formula is valid for every integrable complex function on $\mathbf{R}^n$ such that

$$
\sum_{x\in\Lambda}|f(x+y)|<+\infty
$$

for every $y\in \mathbf{R}^n$ and such that the function on $\mathbf{T}^n$ defined by

$$
y\mapsto \sum_{x\in\Lambda}f(x+y)
$$

is continuous and admits an absolutely convergent Fourier series (cf. below).

#### Remark 2 {#ts-ii-s1-n9-rem-2 .statement tag=02K3}

There exist functions $f\in B(\mathbf{R})$ such that the series $\sum_{n\in\mathbf{Z}}f(n)$ diverges (exercise 4 of II, p. 263).

#### Example {#ts-ii-s1-n9-exa-1 .statement tag=02K4}

Let Q be a positive definite quadratic form on $\mathbf{R}^n$. The function defined by $\varphi (x) =$ exp($-\pi Q(x)$) belong to $\mathscr{S}(\mathbf{R}^n)$. There exists $\sigma \in$ GL($n,\mathbf{R}$) such that $Q(x) =\|\sigma (x)\|^2$ for every $x\in \mathbf{R}^n$. The Fourier transform of $\varphi$ is given for every $y\in \mathbf{R}^n$ by

$\widehat{\varphi}(y) =|$det($1\sigma$ )$|$ exp($-\pi Q^*(y)$)

where $Q^*(y) =\|^t\sigma^{-1}(y)\|^2($cf. INT, IX, §6, n$^o$ 4–5 and exercise 1, c) of II, p. 262).

#### Definition 6 {#ts-ii-s1-def-6 .statement tag=02K5}

The space of tempered distributions on $\mathbf{R}^n$ is, by definition, the dual space of $\mathscr{S}(\mathbf{R}^n)$ endowed with the topology of bounded convergence. It is denoted by $\mathscr{S}'(\mathbf{R}^n)$.

Since $\mathscr{S}(\mathbf{R}^n)$ is bornological, the space $\mathscr{S}'(\mathbf{R}^n)$ is complete and bornological (EVT, III, p. 24, cor. 1 and 2). Since $\mathscr{S}(\mathbf{R}^n)$ is a Montel space, the same is true of $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, prop. 9).

Let $\alpha \in \mathbf{N}^n$. The transpose of the endomorphism $\varphi \mapsto X^{\alpha}\varphi$ of $\mathscr{S}(\mathbf{R}^n)$ is again denoted by $f\mapsto X^{\alpha}f$, and $f\mapsto \partial^{\alpha}f$ denotes the endomorphism of $\mathscr{S}'(\mathbf{R}^n)$ defined by

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

for $f\in \mathscr{S}'(\mathbf{R}^n)$ and $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Let $f$ be a linear mapping of $\mathscr{S}(\mathbf{R}^n)$ into $\mathbf{C}$. Then $f$ is a tempered distribution if, and only if, for every family $(M_{k,\alpha})_{(k,\alpha)\in\mathbf{N}\times\mathbf{N}^n}$ in $\mathbf{R}_+$, the linear form $f$ is bounded on the set of functions $\varphi \in \mathscr{S}(\mathbf{R}^n)$ such that for every $(k, \alpha )\in \mathbf{N}\times \mathbf{N}^n$, one has $p_{k,\alpha}(\varphi )\leqslant M_{k,\alpha}$.

A sequence $(f_m)_{m\in\mathbf{N}}$ of tempered distributions converges to a tempered distribution $f$ if, and only if, one has $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Example {#ts-ii-s1-n9-exa-2 .statement tag=02K6}

A measure $\nu$ on $\mathbf{R}^n$ is said to be tempered if there exists a positive integer $r$ such that the continuous mapping $x\mapsto (1+\|x\|)^{-r}$ is $\nu$-integrable on $\mathbf{R}^n$. The restriction of $\nu$ to $\mathscr{S}(\mathbf{R}^n)$ is a tempered distribution. It is zero if and only if the measure $\nu$ is zero.

Let $p\in [1,+\infty ]$ and $f\in \mathscr{L}^p(\mathbf{R}^n)$. Then the measure $f\cdot dx$ with density $f$ with respect to Lebesgue measure is tempered. In particular, Lebesgue measure $\mu$ on $\mathbf{R}^n$ is tempered, and every bounded measure on $\mathbf{R}^n$ is tempered.

For every $p\in [1,+\infty ]$, one can identify $L^p(\mathbf{R}^n)$ with a subspace of $\mathscr{S}'(\mathbf{R}^n)$ by the linear mapping $f\mapsto f\cdot dx$; this mapping is continuous.

#### Definition 7 {#ts-ii-s1-def-7 .statement tag=02K7}

The transpose of the Fourier transform on $\mathscr{S}(\mathbf{R}^n)$ (resp. of the inverse Fourier transform) is called the Fourier transform on $\mathscr{S}'(\mathbf{R}^n)$, and is denoted by $\mathscr{F}$ (resp. is called the inverse Fourier transform, and is denoted by $\overline{\mathscr{F}}$).

For $f\in \mathscr{S}'(\mathbf{R}^n)$, the tempered distribution $\mathscr{F}(f)$ (resp. $\overline{\mathscr{F}}(f)$) is defined by $\varphi \mapsto  \langle f,\mathscr{F}(\varphi )\rangle$ for $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (resp. by $\varphi \mapsto$ $\langle f,\overline{\mathscr{F}}(\varphi )\rangle$ ).

The Fourier transform on $\mathscr{S}'(\mathbf{R}^n)$ is an automorphism of topological vector spaces whose inverse is the inverse Fourier transform $\overline{\mathscr{F}}$.

#### Proposition 22 {#ts-ii-s1-prop-22 .statement tag=02K8}

Let $f$ be a tempered distribution belonging to $\mathscr{M}^1(\mathbf{R}^n)$ (resp. to $L^2(\mathbf{R}^n)$). The Fourier transform of $f$ in $\mathscr{S}'(\mathbf{R}^n)$ is the tempered distribution associated with the Fourier transform of $f$ in $\mathscr{C}_0(\mathbf{R}^n)$ (resp. in $L^2(\mathbf{R}^n)$). Analogously for the inverse Fourier transform.

#### Remark {#ts-ii-s1-n9-rem-3 .statement tag=02K9}

The elementary formulas concerning the Fourier transform of measures remain valid for the Fourier transform of tempered distributions.

Thus, if $\alpha \in \mathbf{N}^n$ and $f\in \mathscr{S}'(\mathbf{R}^n)$, one has

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

Let $y\in \mathbf{R}^n$. Let us denote by $\boldsymbol{\gamma }(y)$ the endomorphism of $\mathscr{S}'(\mathbf{R}^n)$ defined by

$$
\langle \boldsymbol{\gamma }(y)f, \varphi \rangle =\langle f,\boldsymbol{\gamma }(-y)\varphi \rangle
$$

for $f\in \mathscr{S}'(\mathbf{R}^n)$ and $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Let $e_y$ be the character of $\mathbf{R}^n$ such that $e_y(x) =$ exp(2$i\pi x\cdot y$). Then $e_y\in \mathscr{S}'(\mathbf{R}^n)$. We have $\mathscr{F}(e_y) =\varepsilon_y$, and more generally

$$
\mathscr{F}(e_yf) =\boldsymbol{\gamma }(y)\mathscr{F}(f)
$$

for every $f\in \mathscr{S}'(\mathbf{R}^n).*$

Let $n\geqslant 1$ be an integer, and let $G =\mathbf{T}^n$, endowed with the normalized Haar measure. The dual group of G is identified with $\mathbf{Z}^n$ by the mapping $h\mapsto \chi_h$, where $\chi_h$ is the unitary character of $\mathbf{T}^n$ obtained by passing to the quotient from the character $x\mapsto$ exp(2$i\pi h\cdot x$) of $\mathbf{R}^n$ (Corollary 3 of II, p. 236). The Fourier transform of a measure $\mu$ on $\mathbf{T}^n$ is identified with the family $(\widehat{\mu}(h))_{h\in\mathbf{Z}^n}$ where

$$
\widehat{\mu}(h) =\int_{\mathbf{T}^n}e^{-2i\pi h\cdot x}d\mu(x)
$$

The series

$$
\sum_{h\in\mathbf{Z}^n}\widehat{\mu}(h)\chi_h
$$

is called the Fourier series of $\mu$.

If $f\in L^1(\mathbf{T}^n)$ is such that its Fourier series converges absolutely in $L^1(\mathbf{Z}^n)$, then $f\in \mathscr{C}(\mathbf{T}^n)$ and

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

for every $x\in \mathbf{T}^n$ (Theorem 3 of II, p. 222), where

$$
\widehat{f}(h) =\int_{\mathbf{T}^n}f(x)e^{-2i\pi h\cdot x}dx,h\in \mathbf{Z}^n
$$

For $f\in L^2(\mathbf{T}^n)$, the fourier inversion formula (Proposition 12 of II, p. 219) says that, if the series with general term $\widehat{f}(h)$ converges absolutely, one has

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

for almost every $x$ in $\mathbf{T}^n$.

However, even if $f$ is continuous, the Fourier series of $f$ does not generally converge to $f(x)$ for every $x$ (Exercise 30 of II, p. 274). The following result is all the more useful.

#### Proposition 23 (Fejér's theorem) {#ts-ii-s1-prop-23 .statement tag=02KA}

Let $n\geqslant 1$ be an integer. For every $h= (h_i)\in \mathbf{Z}^n$, put $|h|=$ sup$_i|h_i|$. Let $f\in \mathscr{C}(\mathbf{T}^n)$. For every integer $N\geqslant 1$, let us denote by $f_N$ the function on $\mathbf{T}^n$ such that

$$
f_N(x) =\sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}\widehat{f}(h)e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right)
$$

for $x\in \mathbf{T}^n$. Then $f_N$ converges to $f$ in $\mathscr{C}(\mathbf{T}^n)$.

#### Lemma 11 {#ts-ii-s1-lem-11 .statement tag=02KB}

For every $N\geqslant 1$, let $\mu_N$ be the measure on $\mathbf{T}^n$ with density the continuous mapping

$$
F_N:x\mapsto \sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right).
$$

The sequence of measures $(\mu_N)_{N\geqslant 1}$ converges to $\varepsilon_0$ in the space $\mathscr{M}^1(\mathbf{T}^n)$ endowed with the topology of compact convergence in $\mathscr{C}(\mathbf{T}^n)$.

We are reduced to the case $n= 1$ by observing that $\mu_N$ is the product of measures of the same type for $n= 1$. It is then enough to verify that the sequence $(\mu_N)$ satisfies the hypotheses of lemma 4 of INT, VIII, §2, No.$^o7$ with $a= 0$.

For this, let us first observe that $F_N$ is the Fourier cotransform of the mapping $\varphi_N:h\mapsto (1- |h|/N)$ on $\mathbf{Z}$. This may be written $\varphi_N=$ $N^{-1}\psi_N*\widetilde{\psi}_N$, where $\psi_N$ is the characteristic function of the set defined by $-N/2<|h|\leqslant N/2$. Consequently, $F_N= N^{-1}|\mathscr{F}(\psi_N)|^2\geqslant 0$. Thus, $\mu_N$ is a positive measure; we have $\mu_N(\mathbf{T}) = 1$, which proves (i) and (iii) in loc. cit.

Let us prove condition (ii) of loc. cit. Let U be an open neighbourhood of 0 in $\mathbf{T}$. It is enough to prove that $\mu_N(U)\rightarrow 1$ when $N\rightarrow +\infty$. Let K be a symmetric compact neighbourhood of 0 such that $K^2\subset U$ and let $\psi$ be the characteristic function of K. Put $\varphi =\psi *\psi$. It is an element of $A(\mathbf{T})$ with support contained in U. The real number $m=\varphi (0)$ is the measure of the set K and hence $m >0$. Moreover, we have $0\leqslant \varphi \leqslant m$ since $\varphi (x)$ is the measure of the set $K\cap xK$. We have

$$
\mu_N(U)\geqslant \frac{1}{m}\int_{\mathbf{T}}\varphi (x)\mu_N(x) =\frac{1}{m}\sum\mathscr{F}(\varphi )(h)\varphi_N(h)
$$

$h\in \mathbf{Z}$

by the transposition properties of the Fourier transform (prop. 13 of II, p. 221). Since $\varphi \in A(\mathbf{T})$, its Fourier transform belongs to $L^1(\mathbf{Z})$ and $\varphi$ satisfies the fourier inversion formula (prop. 11 of II, p. 217). Since $\varphi_N(h)\rightarrow 1$ for every $h\in \mathbf{Z}$ and $|\varphi_N(h)|\leqslant 1$, the Lebesgue theorem (INT, IV, §3, n$^o7$, th. 6) and the fourier inversion formula imply that

lim inf$_{N\rightarrow+\infty}\mu_N(U)\geqslant \frac{1}{m}$ lim$_{N\rightarrow+\infty}\sum_{h\in\mathbf{Z}}\mathscr{F}(\varphi )(h)\varphi_N(h) =$

1 $\sum\mathscr{F}(\varphi )(h) =1\varphi (0) = 1$.

$$
m_{h\in\mathbf{Z}}m
$$

Let us prove the proposition. We have $f*F_N=f_N$ for $N\geqslant 1$. The regular representation $\boldsymbol{\gamma }$ of $\mathbf{T}^n$ in $\mathscr{C}(\mathbf{T}^n)$ (INT, VIII, §2, No.$^o3$) is continuous and satisfies $f*F_N=\boldsymbol{\gamma }(\mu_N)f$ (INT, VIII, §4, No.$^o5$, prop. 5 (iv)). The mapping $\mu\mapsto \boldsymbol{\gamma }(\mu)f$ is continuous from $\mathscr{M}^1(\mathbf{T}^n)$ into $\mathscr{C}(\mathbf{T}^n)$ (INT, VI, §1, No.$^o6$, prop. 14). By the lemma, we therefore have

lim$_{N\rightarrow+\infty}f_N=$ lim$_{N\rightarrow+\infty}f*F_N=$ lim$_{N\rightarrow+\infty}\boldsymbol{\gamma }(\mu_N)f=\boldsymbol{\gamma }(\varepsilon_0)(f) =f$

in $\mathscr{C}(\mathbf{T}^n)$.

#### Remark {#ts-ii-s1-n9-rem-4 .statement tag=02KC}

There exist functions $f\in L^1(\mathbf{T})$ whose Fourier series diverges at every point $x\in \mathbf{T}$ (Kolmogorov's theorem, cf. exercise 51 of II, p. 289).

A theorem of Carleson[^1] shows that the symmetric partial sums of the Fourier series of $f$ converge to $f(x)$ for almost all $x\in \mathbf{T}$ if $f\in \mathscr{L}^2(\mathbf{T})$.

## EXERCISES {#ts-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: L. Carleson, On convergence and growth of partial sums of Fourier series, Acta Mathematica 116 (1), 1966, p. 135–157.
