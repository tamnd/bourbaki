---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 6
section_title: Algèbres stellaires
lang: en
source: ts-i-ii-fr
book_pages: TS I.95-TS I.127, TS I.180-TS I.187
pdf_pages: 0108-0140, 0193-0200
extraction: native
subsections:
    - "no": 1
      title: Involutions semi-linéaires
      page: 95
      pdf_page: 108
    - "no": 2
      title: Algèbres involutives
      page: 96
      pdf_page: 109
    - "no": 3
      title: Algèbres normées involutives
      page: 100
      pdf_page: 113
    - "no": 4
      title: Algèbres stellaires
      page: 102
      pdf_page: 115
    - "no": 5
      title: Algèbres stellaires commutatives
      page: 107
      pdf_page: 120
    - "no": 6
      title: Calcul fonctionnel dans les algèbres stellaires unifères
      page: 109
      pdf_page: 122
    - "no": 7
      title: Applications du calcul fonctionnel
      page: 112
      pdf_page: 125
    - "no": 8
      title: Calcul fonctionnel dans une algèbre non unifère
      page: 114
      pdf_page: 127
    - "no": 9
      title: Éléments positifs dans les algèbres stellaires
      page: 115
      pdf_page: 128
    - "no": 10
      title: Unités approchées dans les algèbres stellaires
      page: 120
      pdf_page: 133
    - "no": 11
      title: Quotient par un idéal bilatère fermé
      page: 122
      pdf_page: 135
    - "no": 12
      title: Algèbre stellaire enveloppante d’une algèbre de Banach involutive
      page: 123
      pdf_page: 136
    - "no": 13
      title: Algèbre stellaire d’un groupe localement compact
      page: 125
      pdf_page: 138
statements: 94
exercises: 32
content_sha256: 418c15132f405d471cda0725f703ed4fefdfc3b5f9396eba1fce2ac8cbf4f2cb
translated_from: content/fr/ts/I/06_s6_algebres_stellaires.md
source_lang: fr
translation_method: machine
source_content_sha256: 17da09a7326bcbfc25b9a06206337ce1110eacbaceefbe881fa374e9211b60aa
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-0ae29cb4
glossary_version: 34
glossary_terms_sha256: b900b3139e8e6ae9a917c8a6e18342edcd240f1d77b78b80a5bd6371ab01660d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. STELLAR ALGEBRAS

In this paragraph, the base field is $\mathbf{C}$.

### 1. Semilinear involutions

Let E be a complex vector space. A semilinear involution on E is a $\mathbf{R}$-linear mapping of E into E such that $u\circ u=$ Id$_E$ and $u(\lambda x) =\lambda u(x)$ for all $\lambda \in \mathbf{C}$ and all $x\in E$. We then denote by $E^u$ the real vector subspace of E formed by the elements $x\in E$ such that $u(x) =x$.

#### Lemma 1 {#ts-i-s6-lem-1 .statement tag=02CI}

Let E be a complex vector space and $u$ a semilinear involution on E. Let $x\in E$; put

$$
x_1=\frac{1}{2}(x+u(x)),x_2=\frac{1}{2i}(x-u(x))
$$

The pair $(x_1, x_2)$ is the unique element of $E^u\times E^u$ such that $x=x_1+ix_2$.

The elements $x_1$ and $x_2$ satisfy $x_1+ix_2=x$ and belong to $E^u$ since $u(u(x)) =x$. Conversely, if $y_1$ and $y_2$ in $E^u$ satisfy $x=y_1+iy_2$, it follows that $u(x) =u(y_1) +u(iy_2) =y_1-iy_2$, hence

$$
y_1=\frac{1}{2}(x+u(x)) =x_1,iy_2=\frac{1}{2}(x-u(x)) =ix_2
$$

#### Proposition 1 {#ts-i-s6-prop-1 .statement tag=02CJ}

Let $E_1$ and $E_2$ be complex vector spaces, and let $u_1$ and $u_2$ be semilinear involutions on $E_1$ and $E_2$ respectively. Let $f$ be a linear mapping of $E_1$ into $E_2$. Then $f\circ u_1=u_2\circ f$ if and only if $f(E^{u_1}_1)\subset E^{u_2}_2$.

If $f\circ u_1=u_2\circ f$, we obtain immediately $f(E^{u_1}_1)\subset E^{u_2}_2$. Conversely, suppose that this condition is satisfied. Let $x\in$ E. Write $x=x_1+ix_2$ with $(x_1, x_2)\in E^{u_1}_1\times E^{u_1}_1$ (lemma above). We then have $f(u_1(x)) =f(x_1)-if(x_2)$ and $u_2(f(x)) =u_2(f(x_1))-iu_2(f(x_2)) =$ $f(x_1)-if(x_2) =f(u_1(x))$.

### 2. Involutive algebras

#### Definition 1 {#ts-i-s6-def-1 .statement tag=02CK}

Let A be an algebra over $\mathbf{C}$. An involution in A is called a mapping $x\mapsto x^*$ of A into A such that:

$$
(x^*)^*=x,(x+y)^*=x^*+y^*,(\lambda x)^*=\lambda x^*
$$

$$
(xy)^*=y^*x^*
$$

for all $x, y\in A$ and $\lambda \in \mathbf{C}$. An algebra over $\mathbf{C}$ endowed with an involution is called an involutive algebra.

An involution on A is in particular an isomorphism of the ring A onto the opposite ring $A^{\circ}$.

Let A be an involutive algebra. One says that $x^*$ is the adjoint of $x$. A subset of A stable under the involution is said to be self-adjoint. If A possesses a unit element $e$, one has $e^*=e$; one says that $(A, e)$ is a unital involutive algebra. An element $u$ of a unital involutive algebra is said to be unitary if $uu^*=u^*u=e$, in other words if $u$ is invertible and if its inverse is $u^*$.

An element $x\in A$ is said to be hermitian if $x=x^*$ and normal if $xx^*=$ $x^*x$. This terminology generalizes that of A, IX, § 7, No.$^o3$. Every hermitian element is normal, every unitary element is normal. The set $A_h$ of hermitian elements of A is a real vector subspace of A. If $x$ and $y$ are hermitian and permutable, one has $(xy)^*$ = $y^*x^*=yx=xy$, hence $xy$ is hermitian. For every $x\in A$, the elements $xx^*$ and $x^*x$ of A are hermitian.

If $A =\mathbf{C}$ endowed with the involution $z\mapsto \overline{z}$, one has $A_h=\mathbf{R}$.

#### Lemma 2 {#ts-i-s6-lem-2 .statement tag=02CL}

Let A be an involutive algebra and $x\in A$. The elements

$$
x_1=\frac{1}{2}(x+x^*),x_2=\frac{1}{2i}(x-x^*)
$$

are hermitian and satisfy $x=x_1+ix_2$. If $x=y_1+iy_2$ with $y_1$ and $y_2$ hermitian, then $x_1=y_1$ and $x_2=y_2$. Moreover, the element $x$ is normal if and only if $x_1$ and $x_2$ are permutable.

The first two assertions follow from Lemma 1 of I, p. 95. One computes that $xx^*-x^*x= 2i(x_2x_1-x_1x_2)$, hence $x$ is normal if and only if $x_1$ and $x_2$ are permutable.

Let A be a unital involutive algebra. In order that $x\in A$ be invertible, it is necessary and sufficient that $x^*$ be so, and one then has $(x^*)^{-1}= (x^{-1})^*$. Since $(x-\lambda e)^*=x^*-\lambda e$ for every $\lambda \in \mathbf{C}$, one deduces that Sp$_A(x^*) =$ Sp$_A(x)$.

Let A be an involutive algebra and $\widetilde{A}$ the algebra deduced from A by adjunction of a unit element. There exists in $\widetilde{A}$ a unique involution extending that of A, given by $(\lambda , x)^*= (\lambda , x^*)$ for $\lambda \in \mathbf{C}$ and $x\in A$. If $x\in A$, one has Sp$'_A(x^*) =$ Sp$'_A(x)$.

Let A and B be involutive algebras. By a morphism of A into B is meant an algebra morphism $\varphi$ of A into B such that $\varphi (x^*) =\varphi (x)^*$ whatever $x$ and $y$ in A may be. The identity mapping of A is a morphism of involutive algebras. If C is an involutive algebra and $\pi : B\rightarrow C$ a morphism of involutive algebras, then $\pi \circ \varphi$ is a morphism of involutive algebras. If $\varphi$ is an algebra isomorphism, then $\varphi^{-1}$ is a morphism of involutive algebras, and one says that $\varphi$ is an isomorphism of involutive algebras.

By prop. 1 of I, p. 95, if A and B are involutive algebras, an algebra morphism $\varphi$ of A into B is a morphism of involutive algebras if and only if $\varphi (A_h)\subset B_h$. By an involutive subalgebra of A is meant a self-adjoint subalgebra. The center of A is an involutive subalgebra. If $A_1$ is a self-adjoint two-sided ideal of A, the involution of A defines, by passing to the quotient, an involution in the algebra $A/A_1$, and the canonical mapping of A onto $A/A_1$ is a morphism of involutive algebras.

Let A be an involutive algebra. The radical of A is equal to the radical of the opposite algebra (A, VIII, p. 431, prop. 7), and is therefore self-adjoint.

Let A be an involutive algebra. If $M\subset A$ is self-adjoint, its commutant $M'$ is an involutive subalgebra of A. If $x\in A$, the bicommutant of $\{x, x^*\}$ is an involutive subalgebra containing $x$ and $x^*$, and this subalgebra is commutative if and only if $x$ is normal (n$^o5$ of I, p. 5).

#### Remark {#ts-i-s6-n2-rem-1 .statement tag=02CM}

Let A be an involutive algebra and B a maximal commutative involutive subalgebra of A. Then B is a maximal commutative subalgebra. In particular, if A is unital, then the algebra B is full.

In fact, let $x\in A$ be an element permutable with B. Then $x^*$ is permutable with B. Write $x=x_1+ix_2$ with $x_1$ and $x_2$ hermitian; the elements $x_1$ and $x_2$ are permutable with B (lemma 2). The subalgebra of A generated by B and $x_1$ is therefore commutative and involutive. Consequently, it is equal to B, so that $x_1\in B$. Analogously, one has $x_2\in B$, and therefore finally $x\in B$.

Let A be an involutive algebra. If $f$ is a linear form on A, the mapping $x\mapsto \overline{f(x^*)}$ on A is a linear form on A, denoted by $f^*$. The mapping $f\mapsto f^*$ is a semilinear involution on $A'$. One says that $f$ is hermitian if $f=f^*$. By lemma 1 of I, p. 95, every linear form $f$ on A has a unique representation $f=f_1+if_2$ where $f_1$ and $f_2$ are hermitian, namely $f_1=\frac{1}{2}(f+f^*)$ and $f_2=\frac{1}{2i}(f-f^*)$.

For a linear form $f$ to be hermitian, it is necessary and sufficient that the restriction of $f$ to $A_h$ be real-valued (proposition 1 of I, p. 95). The mapping $f\mapsto f|A_h$ is an isomorphism of the real vector space of hermitian forms onto the dual vector space of the real vector space $A_h$.

In particular, $\mathsf{X}'(A)_h$ (resp. $\mathsf{X}(A)_h$) will denote the set of hermitian characters of A (resp. the set of nonzero hermitian characters of A). A character is therefore hermitian if its restriction to $A_h$ is real-valued.

If A is commutative and if $\chi$ is a character of A, then $\chi^*$ is a character of A, and the mapping $\chi \mapsto \chi^*$ is a homeomorphism of $\mathsf{X}'(A)$ onto $\mathsf{X}'(A)$.

#### Lemma 3 {#ts-i-s6-lem-3 .statement tag=02CN}

Let A be a commutative involutive algebra. The Gelfand transform of A into $\mathscr{C}_0(\mathsf{X}(A))$ is a morphism of involutive algebras if and only if every character of A is hermitian.

In fact, to say that $\mathscr{G}_A$ is a morphism of involutive algebras amounts to saying that, for all $x\in A$ and $\chi \in \mathsf{X}(A)$, one has

$$
\chi (x^*) =\mathscr{G}_A(x^*)(\chi ) =\mathscr{G}_A(x)(\chi ) =\overline{\chi(x)}
$$

that is to say, that every $\chi$ is hermitian.

#### Example 1 {#ts-i-s6-n2-exa-1 .statement tag=02CO}

Let A be the algebra of complex-valued functions on a set X. The mapping $f\mapsto \overline{f}$ is an involution in A. The subalgebra of bounded functions on X is an involutive subalgebra of A. If X is a locally compact topological space, the subalgebras $\mathscr{C}(X),\mathscr{C}_b(X),\mathscr{C}_0(X)$ and $\mathscr{K}(X)$ are involutive subalgebras of A.

#### Example 2 {#ts-i-s6-n2-exa-2 .statement tag=02CP}

Let X be a locally compact topological space and $\mu$ a positive measure on X. The mapping $f\mapsto \overline{f}$ is an involution on the algebra $\mathscr{L}^{\infty}(X, \mu)$; by passing to the quotient it induces an involution on the unital algebra $L^{\infty}(X, \mu)$.

#### Example 3 {#ts-i-s6-n2-exa-3 .statement tag=02CQ}

Let E be a complex Hilbert space. On the Banach algebra $\mathscr{L}(E)$, the mapping $x\mapsto x^*$ (EVT, V, p. 37, prop. 1) is an involution.

#### Example 4 {#ts-i-s6-n2-exa-4 .statement tag=02CR}

Let G be a locally compact group. Let $\mathscr{M}^1(G)$ be the Banach algebra of bounded complex measures on G (example 6 of I, p. 19).

The mapping $x\mapsto x^{-1}$ of G onto G transforms every measure $\mu\in$ $\mathscr{M}^1(G)$ into a measure $\check{\mu}\in \mathscr{M}^1(G)$ (INT, VII, p. 12, formula (13)). We denote by $\mu^*$ the complex conjugate measure of $\check{\mu}$. The mapping $\mu\mapsto \check{\mu}$ is an isometric isomorphism of the Banach algebra $\mathscr{M}^1(G)$ onto the Banach algebra $\mathscr{M}^1(G^{\circ})$ (INT, VIII, §3, n$^o1$, cor. of prop. 7), hence $\mu\mapsto \mu^*$ is an isometric involution of the Banach algebra $\mathscr{M}^1(G)$.

The set A of bounded measures admitting a density with respect to a Haar measure is a closed subalgebra of $\mathscr{M}^1(G)$ stable under the involution (cf. INT, VIII, §4, n$^o5$); it does not depend on the choice of a Haar measure.

Let $\nu$ be a left Haar measure on G and let us denote by Δ the modulus ofvolution$Gf$. We endow$\mapsto f^*=\widetilde{f}L\overset{1}{\cdot}(G\Delta^-, \nu_1$, where) with the product$\widetilde{f}(x) =\frac{(f, g)}{f(x^{-1})}\mapsto$for every$f*^{\nu}g$ and the in-$x\in G$. Then the mapping $f\mapsto f\cdot \nu$ is an isomorphism of the involutive algebra $L^1(G, \nu )$ onto A. This isomorphism is isometric. In particular, $L^1(G, \nu )$ is identified with an involutive subalgebra of $\mathscr{M}^1(G)$.

#### Example 5 {#ts-i-s6-n2-exa-5 .statement tag=02CS}

Let U be an open subset of $\mathbf{C}$ stable under complex conjugation. Consider the algebra $\mathscr{O}(U)$ of complex-valued holomorphic functions on U. For every function $f\in \mathscr{O}(U)$, the mapping $f^*:z\mapsto f(\overline{z})$ is a holomorphic function on U. The mapping $f\mapsto f^*$ is an involution on $\mathscr{O}(U)$.

Similarly, let S be a compact subset of $\mathbf{C}$ stable under complex conjugation. Consider the algebra $\mathscr{O}(S)$ of germs of complex-valued holomorphic functions in a neighbourhood of S. The mapping $f\mapsto f^*$ is an involution on $\mathscr{O}(S)$.

The subalgebra $\mathscr{O}_{\mathbf{R}}(U)$ (resp. the subalgebra $\mathscr{O}_{\mathbf{R}}(S)$) defined in n$^o13$ of I, p. 85 is the set of hermitian elements of $\mathscr{O}(U)$ (resp. of $\mathscr{O}(S)$).

### 3. Involutive Normed Algebras

#### Definition 2 {#ts-i-s6-def-2 .statement tag=02CT}

An involutive normed algebra is a normed algebra A endowed with an involution $x\mapsto x^*$ such that $\|x^*\|=\|x\|$ for every $x$. If A is a Banach algebra, one says that A is an involutive Banach algebra.

#### Example 1 {#ts-i-s6-n3-exa-1 .statement tag=02CU}

Let X be a locally compact topological space. The Banach algebra $\mathscr{C}_b(X)$ of complex-valued continuous bounded functions on X, endowed with the norm $\|f\|$ = sup$_{x\in X}|f(x)|$ and the involution $f\mapsto \overline{f}$, is an involutive Banach algebra. The subalgebra $\mathscr{C}_0(X)$ of continuous functions tending to 0 at infinity is a closed involutive subalgebra of $\mathscr{C}_b(X)$.

#### Example 2 {#ts-i-s6-n3-exa-2 .statement tag=02CV}

Let X be a locally compact topological space and $\mu$ a positive measure on X. The involutive algebra $L^{\infty}(X, \mu)$ (example 2 of I, p. 99) is an involutive Banach algebra, since $|f|=|\overline{f}|$ for every element $f\in L^{\infty}(X, \mu)$.

#### Example 3 {#ts-i-s6-n3-exa-3 .statement tag=02CW}

The involutive algebra $\mathscr{L}(E)$ of continuous endomorphisms of a complex Hilbert space E (I, p. 99, example 3), endowed with the norm

$\|u\|=$ sup$_{\|xx\in\|\leqslant E1}\|u(x)\|$

(EVT, III, p. 14) is an involutive Banach algebra (EVT, V, p. 37, prop. 1).

#### Example 4 {#ts-i-s6-n3-exa-4 .statement tag=02CX}

The involutive algebra $\mathscr{M}^1(G)$ of bounded measures on a locally compact group (I, p. 99, example 4), endowed with the usual norm (example 6 of I, p. 19), is an involutive Banach algebra. Let $\nu$ be a left Haar measure on G. The involutive Banach algebra $L^1(G, \nu )$ is identified with a closed subalgebra of $\mathscr{M}^1(G)$.

#### Example 5 {#ts-i-s6-n3-exa-5 .statement tag=02CY}

Let $(A_i)$ be a family of involutive normed algebras. Let A be the product normed algebra of the $A_i$ (No.$^o1$ of I, p. 15). The algebra A, endowed with the involution $(x_i)^*= (x^*_i)$, is an involutive normed algebra. If each of the algebras $A_i$ is an involutive Banach algebra, then A is an involutive Banach algebra. One says that A is the product involutive normed algebra (resp. the product involutive Banach algebra) of the $A_i$.

#### Example 6 {#ts-i-s6-n3-exa-6 .statement tag=02CZ}

Let A be an involutive normed algebra and let $\widetilde{A}$ be the normed algebra deduced from A by adjunction of a unit element. Endowed with the involution defined in No.$^o2$, the algebra $\widetilde{A}$ is an involutive normed algebra. If A is an involutive Banach algebra, then $\widetilde{A}$ is likewise an involutive Banach algebra.

If A is an involutive normed algebra, the closure of an involutive subalgebra is an involutive subalgebra. If $M\subset A$, the smallest closed involutive subalgebra containing M is called the closed involutive subalgebra generated by M; it is the closure of the subalgebra generated by $M\cup M^*$. If M reduces to a normal element, the closed involutive algebra generated by M is commutative, and all its elements are normal.

Analogously, if A is a unital involutive normed algebra and M a subset of A, the smallest closed involutive unital subalgebra containing M is called the closed involutive unital subalgebra generated by M; it is the closure of the unital subalgebra generated by $M\cup M^*$. If M reduces to a normal element, the closed involutive unital algebra generated by M is commutative, and all its elements are normal.

The quotient of an involutive normed algebra by a closed self-adjoint two-sided ideal, the completion, and the opposite of an involutive normed algebra are naturally involutive normed algebras.

If A is an involutive normed algebra, the set $A_h$ of hermitian elements of A is a normed real vector space.

#### Lemma 4 {#ts-i-s6-lem-4 .statement tag=02D0}

Let A be an involutive normed algebra. For every continuous linear form $f$ on A, one has $\|f^*\|=\|f\|$. If moreover $f$ is hermitian, then $\|f\|=\|f|A_h\|$.

The first assertion follows from the definitions. For the second, let $g$ denote the restriction of $f$ to $A_h$. One has $\|f\|\geqslant \|g\|$. Let us prove the converse inequality. For every $\varepsilon  >$ 0, there exists $x\in$ A such that $\|x\|\leqslant 1$ and $|f(x)|\geqslant \|f\| -\varepsilon$. Multiplying $x$ by a complex number of modulus 1, we may suppose $f(x)\geqslant 0$. Then the element $\frac{1}{2}(x+x^*)$ belongs to $A_h$ and has norm $\leqslant 1$. One has

$|(1_*)|$ 1 $*$

$$
g(x+x)|=|f(x) +f(x)|=f(x)\geqslant \|f\| -\varepsilon
$$

2 2

hence $\|g\|\geqslant \|f\| -\varepsilon$. It follows that $\|g\|\geqslant \|f\|$.

In the sequel, hermitian continuous linear forms on A and real continuous linear forms on $A_h$ will be identified.

#### Lemma 5 {#ts-i-s6-lem-5 .statement tag=02D1}

Let A be an involutive Banach algebra.

a) For every $x\in A$, one has exp($x$)$^*=$ exp($x^*$) ;

b) Let $x\in A_h$ be a hermitian element. Then exp($ix$) is unitary.

In fact, since the involution on A is continuous, one has

exp($x$)$^*=(\sum_{n=0}^{\infty}xn^n$! $)^*=\sum_{n=0}^{\infty}(x\overset{*}{n}$!$)^n=$ exp($x^*$)

for every $x\in A$ (formula (9) of I, p. 78). If $x\in A_h$, there follows

exp($ix$)$^*=$ exp(($ix$)$^*$) $=$ exp($-ix$) $=$ exp($ix$)$^{-1}$

(formula (11) of I, p. 78).

### 4. Stellar Algebras

#### Definition 3 {#ts-i-s6-def-3 .statement tag=02D2}

A Banach involutive algebra A such that $\|x\|^2=\|x^*x\|$ for every $x\in A$ is called a stellar algebra.

If A and B are stellar algebras, a morphism, or morphism of stellar algebras, from A into B is a morphism of involutive algebras from A into B. An isomorphism from A onto B is an isomorphism of involutive algebras from A onto B.

Some authors speak of a "$C^*$-algebra".

Let A be a stellar algebra. A stellar subalgebra of A is a closed involutive subalgebra of A.

#### Example 1 {#ts-i-s6-n4-exa-1 .statement tag=02D3}

The Banach involutive algebra of continuous endomorphisms of a complex Hilbert space (example 3 of I, p. 100) is a stellar algebra (EVT, V, p. 39, prop. 2).

#### Example 2 {#ts-i-s6-n4-exa-2 .statement tag=02D4}

Let X be a locally compact topological space. The Banach involutive algebra $\mathscr{C}_b(X)$ of continuous bounded complex-valued functions on X (example 1 of I, p. 100) is a stellar algebra. In fact, for every function $f\in \mathscr{C}_b(X)$, one has $f^*f=|f|^2$, and therefore $\|f^*f\|=\||f|^2\|=\|f\|^2$.

Let $A =\mathscr{C}_0(X)$ be the Banach involutive subalgebra of functions tending to 0 at infinity. It is a stellar subalgebra of $\mathscr{C}_b(X)$. For every function $f\in A$, one has $\|f\|=\varrho (f)$, since Sp$'_A(f) =f(X)\cup  \{0\}$.

Let X and Y be locally compact topological spaces. For every proper partial mapping $\varphi$ from X into Y (def. 1 of I, p. 33), the algebra morphism $\varphi^*$ from $\mathscr{C}_0(Y)$ into $\mathscr{C}_0(X)$ (prop. 3 of I, p. 34) is a morphism of involutive algebras. Conversely, every morphism of stellar algebras $\pi :\mathscr{C}_0(Y)\rightarrow \mathscr{C}_0(X)$ is of this form (loc. cit.).

#### Example 3 {#ts-i-s6-n4-exa-3 .statement tag=02D5}

Let X be a compact topological space and let $x_0\in X$ be a fixed element of X. The subalgebra $\mathscr{C}'(X)$ of $\mathscr{C}(X)$ consisting of continuous functions $f: X\rightarrow$ $\mathbf{C}$ such that $f(x_0) = 0$ is a stellar algebra.

#### Example 4 {#ts-i-s6-n4-exa-4 .statement tag=02D6}

Let X be a Hausdorff topological space and $\mu$ a positive measure on X. The Banach involutive algebra $L^{\infty}(X, \mu)$ is a commutative unital stellar algebra.

#### Example 5 {#ts-i-s6-n4-exa-5 .statement tag=02D7}

Let $(A_i)$ be a family of stellar algebras. The Banach involutive algebra A product of the $A_i$ (example 5 of I, p. 101) is a stellar algebra, called the product stellar algebra of the $A_i$.

#### Example 6 {#ts-i-s6-n4-exa-6 .statement tag=02D8}

Let A be a stellar algebra. If B is a closed involutive subalgebra of A, then B is a stellar algebra. We shall see (V, to appear) that every stellar algebra is isomorphic to a closed involutive subalgebra of the stellar algebra of endomorphisms of a Hilbert space (example 1).

#### Example 7 {#ts-i-s6-n4-exa-7 .statement tag=02D9}

Let A be a stellar algebra. If $M\subset A$ is any subset, then the closed involutive subalgebra of A generated by M is a stellar algebra, called the stellar subalgebra of A generated by M. If A is moreover unital, then the closed involutive unital subalgebra generated by M is a unital stellar algebra, called the unital stellar subalgebra of A generated by M.

#### Example 8 {#ts-i-s6-n4-exa-8 .statement tag=02DA}

In general, the Banach involutive algebra $\mathscr{M}^1(G)$ (example 4 of I, p. 100) is not a stellar algebra (I, p. 181, exerc. 8).

#### Lemma 6 {#ts-i-s6-lem-6 .statement tag=02DB}

Let A be a Banach algebra endowed with an involution satisfying

$$
\|x\|^2\leqslant \|x^*x\| \tag{1}
$$

for every $x\in A$. Then A is a stellar algebra.

Let $x\in A$. Then $\|x\|^2\leqslant \|x^*\| \cdot  \|x\|$, whence $\|x\|\leqslant \|x^*\|$. By interchanging the roles of $x$ and $x^*$, one sees that $\|x\|=\|x^*\|$. Thus $\|x^*x\|\leqslant$ $\|x^*\|\|x\|\leqslant \|x\|^2$ and the hypothesis implies the equality $\|x\|^2=\|x^*x\|$.

#### Lemma 7 {#ts-i-s6-lem-7 .statement tag=02DC}

Let A be a stellar algebra.

a) The regular representation $\boldsymbol{\gamma }$ of A (def. 1 of I, p. 16) is isometric, that is to say

$\|x\|=$ sup$_{\|y\|\leqslant 1}\|xy\|$,

for all $x\in A$;

b) For all $x\in A_h$, one has

$$
\varrho (x) =\|x\| \tag{2}
$$

Let $x\in A$. One has sup$_{\|y\|\leqslant 1}\|xy\|\leqslant \|x\|$. To prove that $\|x\|\leqslant$ sup$_{\|y\|\leqslant 1}\|xy\|$, one may suppose that $\|x\|= 1$. Then the element $y$ = $x^*$ satisfies $\|y\|=\|x^*\|= 1$, and $\|xy\|=\|x\|^2= 1$, whence assertion a).

Suppose that $x$ is hermitian. Then $\|x^2\|=\|x^*x\|=\|x\|^2$, whence by induction $\|x^{2^n}\|^{2^{-n}}=\|x\|$ for every integer $n\geqslant 1$, whence assertion b) by prop. 1 of I, p. 20.

#### Remark 1 {#ts-i-s6-n4-rem-1 .statement tag=02DD}

Let A be a unital stellar algebra. One has

$$
\|1\|^2=\|1^*1\|=\|1\|
$$

therefore the norm $\|1\|$ is zero or equal to 1. If $A\not=\{0\}$, one deduces that $\|1\|= 1$. Consequently, for every unitary element $u$ of A, one has $\|u\|=$ $\|u^*u\|^{1/2}= 1$.

#### Remark 2 {#ts-i-s6-n4-rem-2 .statement tag=02DE}

Let A be a normed involutive algebra. If $\|x\|^2=\|x^*x\|$ for all $x\in A$, the completion $\widehat{A}$ of A is a stellar algebra.

#### Proposition 2 {#ts-i-s6-prop-2 .statement tag=02DF}

Let A be an involutive Banach algebra, let B be a stellar algebra, and let $\pi$ be a morphism of involutive algebras from A into B. One has $\|\pi (x)\|\leqslant \|x\|$ for all $x\in A$, and in particular $\pi$ is continuous.

For every $x\in A$, one has Sp$'_B(\pi (x))\subset$ Sp$'_A(x)$, therefore $\varrho (\pi (x))\leqslant \varrho (x)\leqslant$ $\|x\|$. Since $\pi (x^*x)\in B_h$, one has $\|\pi (x^*x)\|=\varrho (\pi (x^*x))$ (formula (2)), therefore

$$
\|\pi (x)\|^2=\|\pi (x^*x)\|=\varrho (\pi (x^*x))\leqslant \|x^*x\|=\|x\|^2
$$

#### Proposition 3 {#ts-i-s6-prop-3 .statement tag=02DG}

Let A be a stellar algebra and let $\widetilde{A}$ be the involutive algebra deduced from A by adjunction of a unit element. There exists a unique norm on $\widetilde{A}$ extending that of A and making $\widetilde{A}$ into a stellar algebra.

The uniqueness of such a norm results from prop. 2. Let us now prove its existence. Let $\widetilde{e}$ denote the unit element of $\widetilde{A}$.

Suppose first that A possesses a unit element $e$. The product of the normed involutive algebras A and $\mathbf{C}(\widetilde{e}-e)$ is identified with $\widetilde{A}$ and is a stellar algebra (example 5). The norm on $\widetilde{A}$ extends that of A, whence the assertion.

Suppose henceforth that A does not possess a unit element. For every $x\in \widetilde{A}$, let $\boldsymbol{\gamma }_x$ be the multiplication operator $y\mapsto xy$ from A into A, and set $\|x\|_{\widetilde{A}}=\|\boldsymbol{\gamma }_x\|$. The mapping $x\mapsto  \|x\|_{\widetilde{A}}$ is a seminorm on $\widetilde{A}$. For all $x$ and $x'$ in $\widetilde{A}$, one has $\|xx'\|_{\widetilde{A}}\leqslant \|x\|_{\widetilde{A}}\|x'\|_{\widetilde{A}}$. Moreover, by lemma 7, one has $\|x\|_{\widetilde{A}}=\|x\|$ for all $x\in A$.

Let us show that the mapping $x\mapsto  \|x\|_{\widetilde{A}}$ is a norm on $\widetilde{A}$. Let $\lambda \in \mathbf{C}$ and $x\in A$ be such that $\|\lambda \widetilde{e}+x\|_{\widetilde{A}}$ = 0. If $\lambda \not= 0$, the condition $(\lambda \widetilde{e}+x)y= 0$ for every $y\in A$ implies that $-\lambda^{-1}x$ is a left unit element in A. Analogously, the element $-\overline{\lambda}^{-1}x^*$ is a right unit element. Thus the algebra A would then possess a unit element, contrary to the assumption. Hence $\lambda = 0$. But then $0 =\|x\|_{\widetilde{A}}=$ $\|x\|$, and therefore $x= 0$.

Since A is complete and of codimension 1 in $\widetilde{A}$, the space $\widetilde{A}$ endowed with the norm $x\mapsto  \|x\|_{\widetilde{A}}$ is complete. To conclude, it is therefore sufficient to show that one has $\|x\|^2_{\widetilde{A}}\leqslant \|x^*x\|_{\widetilde{A}}$ for every $x\in \widetilde{A}$ (Lemma 6). One may suppose that $\|x\|_{\widetilde{A}}= 1$. For every real number $r <1$, there therefore exists $y\in A$ such that $\|y\|=\|y^*\|\leqslant 1$ and $\|xy\|^2\geqslant r$. Since $xy\in A$, one has

$$
\|x^*x\|_{\widetilde{A}}\geqslant \|x^*xy\|\geqslant \|y^*(x^*x)y\|=\|(xy)^*(xy)\|=\|xy\|^2\geqslant r
$$

It follows that $\|x^*x\|_{\widetilde{A}}\geqslant 1$, and therefore the involutive algebra $\widetilde{A}$ endowed with the norm $x\mapsto  \|x\|_{\widetilde{A}}$ is a star algebra.

#### Definition 4 {#ts-i-s6-def-4 .statement tag=02DH}

One says that $\widetilde{A}$, endowed with the norm of Prop. 3, is the star algebra deduced from A by adjunction of a unit element.

When $A\not=\{0\}$, the norm of star algebra on the normed involutive algebra $\widetilde{A}$ is not the one considered in Example 6 of I, p. 101 (cf. Exercise 10 of I, p. 181).

#### Proposition 4 {#ts-i-s6-prop-4 .statement tag=02DI}

Let A be a star algebra.

a) If A possesses a unit element and if $u$ is a unitary element of A, then Sp($u$)$\subset \mathbf{U}$;

b) If $h$ is a hermitian element of A, then Sp$'(h)\subset \mathbf{R}$.

One may suppose that A is nonzero. Let us prove assertion a). Let $u$ be a unitary element of A. One has $\|u\|=\|u^{-1}\|= 1$ (Remark 1), hence Sp($u$)$\subset \mathbf{U}($I, p. 26, Cor. 3). To prove b), one may suppose that A is unital (Prop. 3). Let $h$ be a hermitian element of A. Then exp($ih$) is unitary (Lemma 5 of I, p. 102). Thus, by Cor. 2 of I, p. 67 and a), one has exp($i$ Sp($h$)) $=$ Sp(exp($ih$))$\subset \mathbf{U}$, which means that Sp($h$)$\subset \mathbf{R}$.

#### Proposition 5 {#ts-i-s6-prop-5 .statement tag=02DJ}

Let A be a unital star algebra and B a star subalgebra of A containing the unit element of A. Then B is a full subalgebra of A. In particular, one has Sp$_B(x) =$ Sp$_A(x)$ for every $x$ in B.

Let $x$ be a hermitian element of B. Since Sp$_B(x)\subset \mathbf{R}$ (Prop. 4), Prop. 6 of I, p. 28 shows that Sp$_B(x) =$ Sp$_A(x)$. In particular, $x$ is invertible in B if and only if it is invertible in A.

Let now $x$ be any element of B invertible in A. Then $x^*$ is invertible in A, and $xx^*$ is invertible in A. Since $xx^*$ is hermitian, what precedes shows that $xx^*$ is invertible in B. This implies that $x$ is right-invertible in B. Analogously, one verifies that $x$ is left-invertible in B, and hence that $x$ is invertible in B. Thus, B is a full subalgebra of A.

#### Corollary {#ts-i-s6-n4-cor-1 .statement tag=02DK}

Let A be a star algebra and let B be a star subalgebra of A. Then one has Sp$'_B(x) =$ Sp$'_A(x)$ for every $x$ in B.

By adjoining a unit element (prop. 3), this follows from prop. 5.

Proposition 6 (Fuglede–Putnam Theorem)

Let A be a unital star algebra. Let $a$ and $b$ be normal elements of A. If $c\in A$ satisfies $ac=cb$, then $a^*c=cb^*$.

The hypothesis implies $(wa)^kc=c(wb)^k$ for every integer $k\geqslant 0$ and every $w\in \mathbf{C}$, hence $e^{wa}c=ce^{wb}$ (formula (9) of I, p. 78). Consider the function $f$ from $\mathbf{C}$ into A defined by $z\mapsto e^{-za^*}ce^{zb^*}$. It is a holomorphic function on $\mathbf{C}$, whose derivative satisfies

$$
f'(z) =-a^*e^{-za^*}ce^{zb^*}+e^{-za^*}cb^*e^{zb^*}
$$

for every $z\in \mathbf{C}$. Since $c=e^{-za}ce^{zb}$, one can write

$$
f(z) =e^{-za^*}e^{za}c e^{-zb}e^{zb^*}
$$

Since $a$ and $b$ are normal, the elements $e^{-za^*}e^{za}=e^{-za^*+za}$ and $e^{-zb}e^{zb^*}=e^{-zb+zb^*}$ of A are unitary for every $z\in \mathbf{C}$ (lemma 5 of I, p. 102), hence of norm 1. Consequently, one has $\|f(z)\|\leqslant \|c\|$ for every $z\in \mathbf{C}$. The function $f$ is therefore constant (VAR, R1, 3.3.6, p. 29), that is to say that $f(z) =f(0) =c$ for every $z\in \mathbf{C}$. But then $-a^*c+cb^*=f'(0) = 0$.

#### Corollary {#ts-i-s6-n4-cor-2 .statement tag=02DL}

Let A be a star algebra and $a$ a normal element of A. The commutant (resp. the bicommutant) of $\{a, a^*\}$ coincides with the commutant (resp. the bicommutant) of $a$.

It suffices to take $b=a$ in the proposition.

### 5. Commutative Star Algebras

#### Lemma 8 {#ts-i-s6-lem-8 .statement tag=02DM}

Let X and Y be metric spaces, the space X being complete. Let $f$ be a mapping from X into Y such that

$$
d(f(x), f(y))\geqslant d(x, y)
$$

for every $x$ and $y$ in X and such that the graph of $f$ is closed in $X\times Y$. Then $f$ is a closed mapping.

Let F be a closed subset of X and let $(y_n)_{n\in\mathbf{N}}$ be a sequence in $f(F)$ which converges to $y\in Y$. For every $n\in \mathbf{N}$, let $x_n\in F$ be such that $f(x_n) =y_n$. The assumption implies that the sequence $(x_n)_{n\in\mathbf{N}}$ is a Cauchy sequence; let $x\in X$ be its limit; it is an element of F, since F is closed. Moreover, one has $(x_n, f(x_n))\rightarrow (x, y)$ in $X\times Y$. Since the graph of $f$ is closed, it follows that $y=f(x)$ belongs to $f(F)$.

#### Lemma 9 {#ts-i-s6-lem-9 .statement tag=02DN}

Let A be a commutative star algebra. Every character of A is hermitian and the Gelfand transform is a morphism of star algebras of A into $\mathscr{C}_0(\mathsf{X}(A))$.

It is enough to prove the first assertion (proposition 7 of I, p. 38 and lemma 3 of I, p. 98). Let $\chi$ be a character of A. For every hermitian element $y$ of A, one has $\chi (y) =\mathscr{G}_A(y)(\chi )\in$ Sp$'(y)\subset \mathbf{R}$ (prop. 4 of I, p. 106). Consequently, the character $\chi$ is hermitian (prop. 1 of I, p. 95).

#### Theorem 1 {#ts-i-s6-thm-1 .statement tag=02DO}

Let A be a commutative star algebra. The Gelfand transform is an isometric isomorphism of the star algebra A onto the star algebra $\mathscr{C}_0(\mathsf{X}(A))$ of continuous functions on $\mathsf{X}(A)$ tending to 0 at infinity.

The Gelfand transform is a morphism of involutive algebras of A into $\mathscr{C}_0(\mathsf{X}(A))$ (lemma 9). Let B be its image. It is an involutive subalgebra of $\mathscr{C}_0(\mathsf{X}(A))$. The elements of B separate the points of $\mathsf{X}(A)$ by definition. Let $\chi \in \mathsf{X}(A)$. There exists $x\in A$ such that $\chi (x)\not= 0$, hence $f=\mathscr{G}(x)$ is an element of B such that $f(\chi )\not= 0$. By TG, X, p. 40, cor. 2, the subalgebra B is therefore dense in $\mathscr{C}_0(\mathsf{X}(A))$.

For every hermitian element $y$ of A, one has $\|\mathscr{G}(y)\|=\varrho (y) =\|y\|$ (prop. 7 of I, p. 38 and formula (2) of I, p. 104), whence, for every $x\in A$, the equalities

$$
\|x\|^2=\|x^*x\|=\|\mathscr{G}(x^*x)\|=\|\overline{\mathscr{G} (x)}\cdot \mathscr{G}(x)\|=\|\mathscr{G}(x)\|^2
$$

Thus $\mathscr{G}$ is isometric, and its image B is therefore closed (lemma 8). One concludes that $B =\mathscr{C}_0(\mathsf{X}(A))$.

#### Corollary 1 {#ts-i-s6-thm-1-cor-1 .statement tag=02DP}

Let A be a star algebra and $x$ a normal element of A. Then $\|x\|=\varrho (x)$.

Since the star subalgebra of A generated by $x$ and $x^*$ is commutative, one may suppose that A is commutative. In this case, the cor. results from th. 1, from example 2 of I, p. 102 and from th. 1 of I, p. 24.

#### Corollary 2 {#ts-i-s6-thm-1-cor-2 .statement tag=02DQ}

Let A be a commutative star algebra.

a) There exists a locally compact topological space X such that A is isomorphic to the star algebra $\mathscr{C}_0(X)$;

b) Let B be a commutative star algebra. The mapping $\pi \mapsto$ $\mathsf{X}'(\pi )$ is a bijection of the set of morphisms of star algebras of A into B onto the set of proper partial mappings of $\mathsf{X}(B)$ into $\mathsf{X}(A)$ (def. 1 of I, p. 33).

Theorem 1 establishes the first assertion, and the second assertion follows from prop. 3 of I, p. 34 and from example 2 of I, p. 102.

#### Corollary 3 {#ts-i-s6-thm-1-cor-3 .statement tag=02DR}

Let A be a commutative unital star algebra.

a) There exists a compact topological space X such that A is isomorphic to the star algebra $\mathscr{C}(X)$;

b) Let B be a commutative unital star algebra. The mapping $\pi \mapsto \mathsf{X}(\pi )$ is a bijection of the set of unital morphisms of star algebras $A\rightarrow B$ onto the set of continuous mappings of $\mathsf{X}(B)$ into $\mathsf{X}(A)$.

This follows from the foregoing and from prop. 4 of I, p. 35.

#### Remark {#ts-i-s6-n5-rem-1 .statement tag=02DS}

*Let $\mathbf{G}$ be the category whose objects are the locally compact spaces and whose morphisms are the proper partial mappings (def. 1 of I, p. 33), and let $\mathbf{S}$ be the category of commutative star algebras, whose morphisms are the morphisms of involutive algebras. Consider the functor from $\mathbf{S}$ into the opposite category $\mathbf{G}^{\circ}$ which associates with a commutative star algebra A the locally compact space $\mathsf{X}(A)$ of nonzero characters of A, and with a morphism $\varphi : A\rightarrow B$ of commutative star algebras the continuous mapping $\mathsf{X}'(\varphi )$. Th. 1 and cor. 2 mean that this functor is an equivalence of categories, and that a quasi-inverse of this functor is the functor which associates with a locally compact topological space X the commutative star algebra $\mathscr{C}_0(X)$.

Analogously, corollary 3 means that the opposite category of the category of compact spaces is equivalent to the category of commutative unital star algebras.*

### 6. Functional calculus in unital star algebras

In this number, A is a unital star algebra and $x$ is a normal element of A.

Let B be the unital star-subalgebra of A generated by $x$; it is commutative and contained in the bicommutant of $\{x, x^*\}$, hence in the bicommutant of $x$ (cor. to prop. 6 of I, p. 106). The Gelfand transform $\mathscr{G}_B: B\rightarrow \mathscr{C}(\mathsf{X}(B))$ is an isomorphism of star-algebras (th. 1 of I, p. 108). We have Sp$_B(x) =$ Sp$_A(x)$ (prop. 5 of I, p. 106).

#### Lemma 10 {#ts-i-s6-lem-10 .statement tag=02DT}

The mapping ev$_x:\chi \mapsto \chi (x)$ induces a homeomorphism of $\mathsf{X}(B)$ onto Sp$_A(x)$.

The mapping $x\mapsto \chi (x)$ of $\mathsf{X}(B)$ into $\mathbf{C}$ is continuous, and its image is equal to Sp$_B(x)$ by prop. 6 of I, p. 37, hence to Sp$_A(x)$. Since the characters of B are Hermitian (lemma 9 of I, p. 107), characters of B which coincide at $x$ are also equal at $x^*$, hence are equal on the unital star-subalgebra B generated by $x$. This proves that the mapping ev$_x$ is injective. Since $\mathsf{X}(B)$ is compact and $\mathbf{C}$ is separated, it induces a homeomorphism of $\mathsf{X}(B)$ onto its image, whence the lemma.

From the lemma one deduces an isomorphism of star-algebras $\varphi_x:\mathscr{C}$(Sp$_A(x)$)$\rightarrow \mathscr{C}(\mathsf{X}(B))$. It carries a function $f\in \mathscr{C}$ (Sp$_A(x)$) to the function $\chi \mapsto f(\chi (x))$. The mapping $\mathscr{G}_B^{-1}\circ \varphi_x$ is an isomorphism of the star-algebra $\mathscr{C}$(Sp$_A(x)$) onto B.

#### Definition 5 {#ts-i-s6-def-5 .statement tag=02DU}

The involutive morphism $f\mapsto (\mathscr{G}_B^{-1}\circ \varphi_x)(f)$ of $\mathscr{C}$(Sp$_A(x)$) into A is called the mapping of continuous functional calculus of $x$ in A. It is denoted by $f\mapsto f(x)$.

#### Remark {#ts-i-s6-n6-rem-1 .statement tag=02DV}

The mapping $f\mapsto f(x)$ is isometric; its image is the unital star-subalgebra B generated by $x$, which is contained in the bicommutant of $x$.

If $f$ is the restriction to Sp$_A(x)$ of a function of the form $z\mapsto$ $P(z, z)$, where $P\in \mathbf{C}[X,Y]$ is a polynomial, then one has $f(x) = P(x, x^*)$ in the usual algebraic sense.

#### Example 1 {#ts-i-s6-n6-exa-1 .statement tag=02DW}

Suppose that there exists $\lambda \in \mathbf{C}$ such that Sp$_A(x)$ is reduced to $\lambda$. Then one has $x=\lambda \cdot 1$. In fact, the identity function of Sp$_A(x)$ is equal to $\lambda$, therefore its image under the functional calculus mapping, that is to say $x$, is equal to $\lambda \cdot 1$.

#### Example 2 {#ts-i-s6-n6-exa-2 .statement tag=02DX}

For $x$ to be hermitian, it is necessary and sufficient that Sp$_A(x)$ be contained in $\mathbf{R}$. In fact, let $f$ be the continuous mapping on Sp$_A(x)$ given by $f(z) =z-\overline{z}$. Then $x$ is hermitian if and only if $f(x) = 0$, that is, if $f$ is zero, that is, if Sp$_A(x)$ is contained in $\mathbf{R}$.

#### Example 3 {#ts-i-s6-n6-exa-3 .statement tag=02DY}

For $x$ to be unitary, it is necessary and sufficient that its spectrum be contained in the unit circle of $\mathbf{C}$. In fact, let $f\in \mathscr{C}$ (Sp$_A(x)$) be the function defined by $f(z) =zz-1$; the element $x$ is unitary if and only if $f(x) = 0$, that is, if $f$ is zero.

#### Proposition 7 {#ts-i-s6-prop-7 .statement tag=02DZ}

The mapping $f\mapsto f(x)$ is the unique unital morphism of involutive algebras from $\mathscr{C}$ (Sp$_A(x)$) into A such that the identity mapping $z$ of Sp$_A(x)$ has image $x$.

In fact, the unital subalgebra of $\mathscr{C}$ (Sp$_A(x)$) generated by the elements $z$ and $\overline{z}$ of $\mathscr{C}$(Sp$_A(x)$) is dense in $\mathscr{C}$ (Sp$_A(x)$) (TG, X, p. 40, cor. 1). Since every morphism of involutive algebras from $\mathscr{C}$ (Sp$_A(x)$) into A is continuous (I, p. 104, prop. 2), there exists at most one morphism of involutive algebras from $\mathscr{C}$(Sp$_A(x)$) into A which maps $z$ to $x$.

The following corollary shows that when $f$ is the restriction of a holomorphic function in a neighbourhood of Sp$_A(x)$, the definition of $f(x)$ coincides with that of the holomorphic functional calculus in one variable of No. 9 of I, p. 74.

#### Corollary 1 {#ts-i-s6-prop-7-cor-1 .statement tag=02E0}

Let $f\in \mathscr{O}$(Sp$_A(x)$) be a germ of a holomorphic function in a neighbourhood of Sp$_A(x)$ and let $\widetilde{f}\in \mathscr{C}$(Sp$_A(x)$) be the continuous function on Sp$_A(x)$ associated with $f$. Then $\widetilde{f}(x) =f(x)$, where $f(x)$ is the element of A given by the holomorphic functional calculus.

In fact, the mapping $f\mapsto \widetilde{f}(x)$ is a continuous unital morphism from $\mathscr{O}$(Sp$_A(x)$) into A which maps the germ of the identity function in a neighbourhood of Sp$_A(x)$ to $x$. The result is then a consequence of theorem 5 of I, p. 74.

#### Corollary 2 {#ts-i-s6-prop-7-cor-2 .statement tag=02E1}

Let $f\in \mathscr{C}$ (Sp$_A(x)$).

a) We have

Sp$_A(f(x)) =f$(Sp$_A(x)$) ;

b) For every $g\in \mathscr{C}$ (Sp$_A(f(x))$), one has $(g\circ f)(x) =g(f(x))$.

Since $f(x)$ belong to the full subalgebra B of A, one has Sp$_A(f(x)) =$ Sp$_B(f(x))$ (Prop. 5 of I, p. 106). The isomorphism $f\mapsto f(x)$ of $\mathscr{C}$(Sp$_A(x)$) into B preserves the spectrum; hence one has Sp$_B(f(x)) =$ Sp$_{\mathscr{C}(Sp_A(x))}(f) =f$(Sp$_A(x)$) (Example 3 of I, p. 17). This proves assertion a).

The mapping $g\mapsto (g\circ f)(x)$ is a unital morphism of involutive algebras of $\mathscr{C}$(Sp$_A(f(x))$) into A which transforms the identical function on Sp$_A(f(x))$ into $f(x)$. By Prop. 7, one has therefore $(g\circ f)(x) =g(f(x))$ for every $g\in \mathscr{C}$ (Sp$_A(f(x))$).

#### Example 4 {#ts-i-s6-n6-exa-4 .statement tag=02E2}

Let X be a locally compact space and let $A =\mathscr{C}_b(X)$ be the commutative unital star algebra of continuous bounded functions on X (Example 2 of I, p. 102). Let $g\in A$; its spectrum S is the closure in $\mathbf{C}$ of the set $g(X)$ of values of $g$ (Example 3 of I, p. 17). The functional calculus mapping of $g$ is then the mapping $f\mapsto f\circ g$, for $f\in \mathscr{C}(S)$. In fact, this mapping is a unital morphism of star algebras such that the identical mapping on S has image $g$.

In the case where X is compact, one has $A =\mathscr{C}(X)$ and $S =g(X)$.

Let $\pi : A\rightarrow A'$ be a unital morphism of unital star algebras. The element $\pi (x)$ of $A'$ is normal and its spectrum relative to $A'$ is contained in Sp$_A(x)$. One then has:

#### Proposition 8 {#ts-i-s6-prop-8 .statement tag=02E3}

Let $f\in \mathscr{C}$(Sp$_A(x)$). Denoting again by $f$ the restriction of $f$ to Sp$_{A'}(\pi (x))$, one has the equality $\pi (f(x)) =f(\pi (x))$. In particular, for every $\chi \in \mathsf{X}(A)$, one has $\chi (f(x)) =f(\chi (x))$.

Let $z$ be the identical mapping on Sp$_A(x)$. The mappings defined by $f\mapsto \pi (f(x))$ and $f\mapsto f(\pi (x))$ are continuous unital morphisms of involutive algebras of $\mathscr{C}$(Sp$_A(x)$) into B which map $z$ onto $\pi (x)$. These morphisms therefore coincide on the unital involutive subalgebra of $\mathscr{C}$ (Sp$_A(x)$) generated by $z$. Since the latter is dense in $\mathscr{C}$(Sp$_A(x)$) (TG, X, p. 40, Cor. 1), these morphisms are equal.

#### Corollary {#ts-i-s6-n6-cor-1 .statement tag=02E4}

Suppose that A is commutative. For every $f\in$ $\mathscr{C}$(Sp$_A(x)$), one has $\mathscr{G}_A(f(x)) =f\circ \mathscr{G}_A(x)$.

It is enough to apply Proposition 8 to the Gelfand transform $\mathscr{G}_A$ of A into $\mathscr{C}(\mathsf{X}(A))$ and to remark (example above) that $f(\mathscr{G}_A(x)) =f\circ \mathscr{G}_A(x)$.

### 7. Applications of the functional calculus

#### Proposition 9 {#ts-i-s6-prop-9 .statement tag=02E5}

Every injective morphism of stellar algebras is isometric and, in particular, has closed image.

Let A and $A'$ be stellar algebras and let $\pi : A\rightarrow A'$ be a morphism of involutive algebras from A into $A'$.

Suppose first that A and $A'$ are unital and that $\pi$ is unital. One has $\|\pi \|\leqslant 1$ (Proposition 2). Suppose there exists $x$ in A such that $\|\pi (x)\|<\|x\|$. Put $y=x^*x$; this is a hermitian element of A. Since A and $A'$ are stellar algebras, one has $\|\pi (y)\|=\|\pi (x)\|^2<\|x\|^2=$ $\|y\|$, that is, $\varrho (\pi (y))< \varrho (y)$ (Lemma 7 of I, p. 104). In particular, Sp$_{A'}(\pi (y))$ is a closed subset of Sp$_A(y)$, distinct from Sp$_A(y)$ (Remark 6 of I, p. 3 and Theorem 1 of I, p. 24). There then exists a non-zero function $f\in \mathscr{C}$(Sp$_A(y)$) such that $f|$ Sp$_{A'}(\pi (y)) = 0$ (TG, IX, p. 13, Proposition 3). Put $w=f(y)\in$ A. One has $w\not= 0$ since $f\not= 0$, but $\pi (w) =\pi (f(y)) =f(\pi (y)) = 0$ since $f$ vanishes on Sp$_{A'}(\pi (y))$ (Proposition 8). Hence $\pi$ is not injective.

Let us now treat the general case. Let $\widetilde{A}$ and $\widetilde{A}'$ be the stellar algebras deduced from A and $A'$ respectively by adjunction of a unit element (Definition 4 of I, p. 106). There exists a unique unital morphism of involutive algebras $\widetilde{\pi}:\widetilde{A}\rightarrow \widetilde{A}'$ extending $\pi$. This morphism is injective, hence is isometric by what precedes. For every $x\in A$, one then has $\|\pi (x)\|=\|\widetilde{\pi}(x)\|=\|x\|$.

#### Lemma 11 {#ts-i-s6-lem-11 .statement tag=02E6}

Let X be a completely regular topological space, that is to say uniformizable and separated (TG, IX, p. 8, Definition 4), containing at least two points. There exist non-zero continuous functions $f$ and $g$ in $\mathscr{C}(X)$ such that $f g= 0$.

Let $x\not=y$ be distinct points of X. Let U and V be open neighbourhoods of $x$ and $y$, respectively, such that U and V are disjoint. Since X is uniformizable, by TG, IX, p. 7, Theorem 2, there exists a function $f\in \mathscr{C}(X)$ such that $f(x) = 1$ and $f|X$ - U = 0. Analogously, there exists $g\in \mathscr{C}(X)$ such that $g(y) = 1$ and $g|X$ - V = 0. One then has $f g= 0$.

#### Proposition 10 {#ts-i-s6-prop-10 .statement tag=02E7}

Let A be a unital stellar algebra. Suppose that for every pair $(x, y)$ of permutable elements of A, the condition $xy= 0$ implies that $x= 0$ or $y= 0$. Then $A =\mathbf{C}\cdot 1$.

If A is not equal to $\mathbf{C}\cdot 1$, there exists a hermitian element $x$ in A which does not belong to $\mathbf{C}\cdot 1$ (Lemma 2 of I, p. 96). Let B be the unital involutive subalgebra of A generated by $x$. It is commutative, and isomorphic to $\mathscr{C}$ (Sp$_A(x)$) (I, p. 110, Remark). Since $x$ is not scalar, its spectrum in B is not reduced to a single element (Example 1 of I, p. 110). There therefore exist continuous nonzero functions $f$ and $g$ on Sp$_A(x)$ such that $f g= 0$ (Lemma 11). The elements $f(x)$ and $g(x)$ of A are nonzero, commuting, and satisfy $f(x)g(x) = 0$ in A.

#### Proposition 11 {#ts-i-s6-prop-11 .statement tag=02E8}

Let A be a unital involutive algebra, and let $a,x$ and $y$ be elements of A. Suppose that $x$ and $y$ are normal. If $xa=$ $ay$, then one has $f(x)a=af(y)$ for every function $f$ continuous in the union of the spectrum of $x$ and the spectrum of $y$. In particular, one has $f(aa^*)a=af(a^*a)$ for every function $f\in \mathscr{C}$ (Sp$'(a^*a)$).

Let S = Sp($x$)$\cup$ Sp($y$). Proposition 6 of I, p. 106 implies that $x^*a=ay^*$. Consequently, one has $f(x)a=af(y)$ for every function $f$ of the form $z\mapsto P(z, z)$, where $P\in \mathbf{C}[X,Y]$ is a polynomial. Since the set of functions $f\in \mathscr{C}(S)$ satisfying $f(x)a=$ $af(y)$ is a closed subalgebra of $\mathscr{C}(S)$, it coincides with $\mathscr{C}(S)$ by TG, X, p. 40, Cor. 1.

The second assertion is a consequence of the first, applied to the hermitian elements $x=aa^*$ and $y=a^*a$, having regard to the fact that Sp$'(a^*a) =$ Sp$'(aa^*)$ (Prop. 1 of I, p. 5).

### 8. Functional Calculus in a Non-unital Algebra

Let A be an involutive algebra and let $\widetilde{A}$ be the unital involutive algebra deduced from A by adjunction of a unit element $e$. Let us denote by $\pi$ the hermitian character $x+\lambda e\mapsto \lambda$ of $\widetilde{A}$ into $\mathbf{C}$; one has Ker($\pi$ ) $= A$.

Let $x\in A$ be a normal element. It is normal in $\widetilde{A}$ and Sp$_{\widetilde{A}}(x) =$ Sp$'_A(x)$. Let $\mathscr{C}'$(Sp$'_A(x)$) denote the stellar algebra of continuous functions $f$ on Sp$'_A(x)$ such that $f(0) = 0$.

Let $f\in \mathscr{C}$ (Sp$'_A(x)$). Since $\pi (f(x)) =f(\pi (x))$ (prop. 8 of I, p. 112), we have $f(x)\in A$ if and only if $f(0) = 0$. The mapping $f\mapsto f(x)$ defines a morphism of involutive algebras from the stellar algebra $\mathscr{C}'$(Sp$'_A(x)$) into A for which the image of the identity mapping $z$ of Sp$'_A(x)$ is $x$. This morphism is isometric and its image is the stellar subalgebra of A generated by $x$.

#### Proposition 12 {#ts-i-s6-prop-12 .statement tag=02E9}

The mapping $f\mapsto f(x)$ is the unique morphism of involutive algebras from the stellar algebra $\mathscr{C}'$(Sp$'_A(x)$) into A such that the identity mapping $z$ of Sp$'_A(x)$ has image $x$.

The elements $z$ and $\overline{z}$ of $\mathscr{C}'$(Sp$'_A(x)$) generate a dense subalgebra of $\mathscr{C}'$(Sp$'_A(x)$) (cf. TG, X, p. 40, cor. 2). Since every morphism of involutive algebras from the stellar algebra $\mathscr{C}'$(Sp$'_A(x)$) into the stellar algebra A is continuous (I, p. 104, prop. 2), the result follows.

The results of the preceding number concerning the functional calculus extend to the general case. We shall merely state them and leave it to the readers to complete the proofs, mutatis mutandis.

#### Proposition 13 {#ts-i-s6-prop-13 .statement tag=02EA}

We have the following properties:

a) For every $f\in \mathscr{C}'$(Sp$'_A(x)$), we have Sp$'_A(f(x)) =f$(Sp$'_A(x)$) ;

b) For every $f\in \mathscr{C}'$(Sp$'_A(x)$) and for every $g\in \mathscr{C}'$(Sp$'_A(f(x))$), we have $(g\circ f)(x) =g(f(x))$ ;

c) Let $A'$ be a stellar algebra and let $\pi$ be a morphism from A into $A'$; then $\pi (x)$ is normal in $A'$, we have Sp$'_{A'}(\pi (x))\subset$ Sp$'_A(x)$ and $\pi (f(x)) =f(\pi (x))$ for every $f\in \mathscr{C}'$(Sp$'_A(x)$);

d) If A is commutative, and if $f\in \mathscr{C}'$(Sp$'_A(x)$), then $\mathscr{G}'_A(f(x)) =$ $f\circ \mathscr{G}'_A(x)$.

#### Remark {#ts-i-s6-n8-rem-1 .statement tag=02EB}

Let A be a unital involutive algebra and let $\widetilde{A}$ be the unital involutive algebra deduced from A by adjunction of a unit element $e$. For every $x\in A$, one has Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. Let $x$ be a normal element of A. Then it is a normal element of $\widetilde{A}$, and therefore one has two mappings of functional calculus in A, the first defined on $\mathscr{C}$ (Sp$_A(x)$) and the second on $\mathscr{C}'$(Sp$'_A(x)$). Let $f'\in \mathscr{C}'$(Sp$'_A(x)$); if $f$ denotes its restriction to Sp$_A(x)$, one then has $f'(x) =f(x)$.

### 9. Positive Elements in Involutive Algebras

#### Definition 6 {#ts-i-s6-def-6 .statement tag=02EC}

Let A be an involutive algebra. An element $x$ of A is said to be positive if it is hermitian and if Sp$'_A(x)\subset \mathbf{R}_+$. The set of positive elements of A is denoted by $A_+$. It is a subset of $A_h$.

One writes $x\geqslant y$ if $x-y\in A_+$.

If the involutive algebra A is unital, its unit element is positive.

If B is an involutive subalgebra of A, one has $B_+= B\cap A_+$ (cor. of prop. 5 of I, p. 106).

If $\pi : A\rightarrow$ B is a morphism of involutive algebras, then $\pi (A_+)\subset B_+$.

#### Example 1 {#ts-i-s6-n9-exa-1 .statement tag=02ED}

Let X be a locally compact space. In the involutive algebra $\mathscr{C}_0(X)$ of continuous functions on X tending to 0 at infinity, resp. in the involutive algebra $\mathscr{C}_b(X)$ of bounded continuous functions, a function $f$ is a positive element if and only if it is real-valued and if $f(x)\geqslant 0$ for every $x\in X$ (cf. example 3 of I, p. 17).

#### Example 2 {#ts-i-s6-n9-exa-2 .statement tag=02EE}

Let A be a commutative involutive algebra. Let $a$ be in A. Since Sp$'_A(x)$ is the union of $\{0\}$ and of the image of the Gelfand transform $\mathscr{G}(a)$ (prop. 6 of I, p. 37), the element $a$ is positive if, and only if, the Gelfand transform $\mathscr{G}(a)$ is a positive function.

#### Example 3 {#ts-i-s6-n9-exa-3 .statement tag=02EF}

Let E be a complex Hilbert space. An element $x$ of the involutive algebra $\mathscr{L}(E)$ (example 1 of I, p. 102) is positive if and only if it is a positive endomorphism of E in the sense of EVT, V, p. 45, def. 6 (prop. 8 of I, p. 138).

#### Lemma 12 {#ts-i-s6-lem-12 .statement tag=02EG}

Let A be a unital involutive algebra and let $x\in A$ be a hermitian element.

a) The element $x$ is positive if and only if $\|\|x\| \cdot 1-x\|\leqslant \|x\|$;

b) If $\|x\|\leqslant 1$, then $x$ is positive if and only if $\|1-x\|\leqslant 1$ ;

c) If $x$ is positive, then $1-x$ is positive if and only if $\|x\|\leqslant 1$ ;

d) If $x$ is positive and if $y\in A_+$ commutes with $x$, then $xy$ is positive.

The element $x$ is hermitian, hence normal. By considering the involutive subalgebra generated by $x$, which is commutative, one is reduced to the case where the algebra A is commutative, that is, to the case where A = $\mathscr{C}_0(X)$ for a locally compact topological space X (th. 1 of I, p. 108). The first three assertions then follow immediately from example 1 above. Analogously, to now prove assertion d), one may consider the involutive subalgebra generated by $x$ and $y$, which is commutative.

#### Proposition 14 {#ts-i-s6-prop-14 .statement tag=02EH}

Let A be an involutive algebra. The set $A_+$ is a salient closed pointed convex cone in the real Banach space $A_h$ (EVT, II, p. 11).

Let $\widetilde{A}$ be the star-algebra deduced from A by adjunction of a unit element. Since $A_+= A\cap \widetilde{A}_+$, it is enough to prove the proposition for $\widetilde{A}$. We may therefore suppose that A has a unit element.

We have $0\in A_+$. For every $\lambda \in \mathbf{R}_+^*$ and every $x\in A$, we have Sp$'_A(\lambda x) =$ $\lambda$ Sp$'_A(x)$, which implies that $A_+$ is a cone in the real Banach space $A_h$.

To show that $A_+$ is convex, it is enough to show that if $x$ and $y$ are positive, then $x+y\geqslant 0$ (EVT, II, p. 11, prop. 10). By homothety, it is enough to prove that if $x\geqslant 0$ and $y\geqslant 0$ satisfy moreover $\|x\|\leqslant 1$, $\|y\|\leqslant 1$, then the element $\frac{1}{2}(x+y)$ is positive. Now we have

$$
\|1-\frac{1}{2}(x+y)\|\leqslant \frac{1}{2}\|1-x\|+\frac{1}{2}\|1-y\|\leqslant 1
$$

by assertion b) of lemma 12, and that same assertion then shows that $\frac{1}{2}(x+y)$ is positive.

Finally, assertion a) of lemma 12 also implies that $A_+$ is closed.

Since $A_+$ is a pointed cone in $A_h$, it is salient if and only if $A_+\cap (-A_+)$ is reduced to 0. But if $x\in A_+\cap (-A_+)$, we have Sp$'_A(x) =$ $\{0\}$, hence $\varrho (x) = 0$, and $\|x\|= 0$ since $x$ is hermitian (lemma 7, (2) of I, p. 104), whence $x= 0$.

Proposition 14 means that the relation “ $x\geqslant y$ ” is an order relation on $A_h$ (EVT, II, p. 13, prop. 13).

#### Proposition 15 {#ts-i-s6-prop-15 .statement tag=02EI}

Let A be a star-algebra. Let $x$ be a normal element of A.

a) Suppose that A is unital and let $f$ be a continuous function from Sp$_A(x)$ into $\mathbf{C}$. In order that $f(x)$ be positive, it is necessary and sufficient that the image of $f$ be contained in $\mathbf{R}_+$;

b) Let $f$ be a continuous function from Sp$'_A(x)$ into $\mathbf{C}$ such that $f(0) =$ 0. In order that $f(x)$ be a positive element of A, it is necessary and sufficient that the image of $f$ be contained in $\mathbf{R}_+$.

Assertion a) follows from assertion a) of cor. 2 of I, p. 111, and assertion b) follows from prop. 13 of I, p. 114.

Let $x$ be a hermitian element of the star-algebra A. Its spectrum is contained in $\mathbf{R}$ (prop. 4 of I, p. 106). Consider the continuous functions from Sp$'_A(x)$ into $\mathbf{R}$ defined by

$f_1:t\mapsto$ sup($t,0$)$,f_2:t\mapsto$ sup($-t,0$)$,f_3:t\mapsto  |t|$.

We put

$$
x^+=f_1(x),x^-=f_2(x),|x|=f_3(x) \tag{3}
$$

Since the functions $f_1,f_2,f_3$ take positive real values and vanish at 0, the elements $x^+,x^-$ and $|x|$ are positive elements of A (Prop. 15, a)) which belong to the stellar subalgebra of A generated by $x$.

One has $f_1(t)-f_2(t) =t$ for every $t\in \mathbf{R}$, as well as the relations $f_1+f_2=f_3$ and $f_1f_2= 0$. Hence the relations:

$$
x=x^+-x^-,|x|=x^++x^-,x^+x^-=x^-x^+= 0 \tag{4}
$$

Since the functional calculus mapping is isometric, one has

$$
\| |x| \|=\|x\|,\|x^+\|\leqslant \|x\|,\|x^-\|\leqslant \|x\|
$$

Let $x$ be a positive element of A. It is hermitian, hence normal. Let $\alpha \in \mathbf{R}^*_+$, and let $g$ be the restriction to Sp$'_A(x)$ of the function $t\mapsto t^{\alpha}$; one writes $x^{\alpha}=g(x)$. It is a positive element of the stellar subalgebra of A generated by $x$. Let $\alpha$ and $\beta$ be in $\mathbf{R}^*_+$. Since the functional calculus mapping is an algebra morphism, and by Prop. 13 of I, p. 114, one has

$$
x^{\alpha}x^{\beta}=x^{\alpha+\beta}(x^{\alpha})^{\beta}=x^{\alpha \beta} \tag{5}
$$

$$
\surd_/
$$

One shall also write $\overline{x}=x^{12}$.

#### Proposition 16 {#ts-i-s6-prop-16 .statement tag=02EJ}

Let $x$ be a positive element of A. Let $\alpha \in \mathbf{R}^*_+$. Then $x^{1/\alpha}$ is the unique positive element $y$ of A such that $y^{\alpha}=x$.

It was seen above that $x^{1/\alpha}$ satisfies the required properties. Conversely, let $y$ be a positive element of A such that $y^{\alpha}=x$. By formula (5), one has $y= (y^{\alpha})^{1/\alpha}=x^{1/\alpha}$, which was to be proved.

#### Lemma 13 {#ts-i-s6-lem-13 .statement tag=02EK}

Let A be a unital stellar algebra. Every element of A is a sum of unitary elements.

By the lemmaLet $x$ be a hermitian element of12, c), one has $1-\frac{1}{4}Ax$. Suppose first that$_2\in A_+$. Let $y=\frac{1}{2}x+i\surd\|1x-\|\leqslant_{1\overline{4}}x2_2$..

One has $y^*=\frac{1}{2}x-i\surd\overline{1 -\frac{1}{4}x^2}$, hence $yy^*= 1$ and $x=y+y^*$ is a sum of two unitary elements. In the general case, let $k$ be an integer such that $\|\frac{1}{k}x\|\leqslant 2$ ; the element $x$ is then a sum of $2k$ unitary elements. By Lemma 2 of I, p. 96, the lemma follows.

#### Theorem 2 {#ts-i-s6-thm-2 .statement tag=02EL}

Let A be a stellar algebra. An element $x$ of A is positive if and only if there exists $y\in A$ such that $x=y^*y$.

Suppose that $x$ is positive. Let $y=x^{1/2}$; it is a hermitian element of A and one has $y^*y=y^2=x$.

Conversely, let $y$ be an element of A and put $x=y^*y$. It is a hermitian element of A. Let us show that $x$ is positive. For this, let us write $z=x^-$ and put $w=yz$. One then has

$$
w^*w=z^*y^*yz=zxz=z(x^+-z)z=-z^3
$$

Since $z\geqslant 0$, we have $z^3\geqslant 0$, and it follows that Sp$'_A(w^*w)\subset \mathbf{R}_-$. Let us write $w=w_1+iw_2$ where $w_1$ and $w_2$ are hermitian (Lemma 2 of I, p. 96). The elements $w^2_1$ and $w_2^2$ are positive. We have $ww^*+w^*w=$ $2w^2_1+ 2w_2^2$, and Prop. 14 therefore shows that $ww^*= 2w_1^2+ 2w^2_2+ (-w^*w)$ is positive. Since Sp$'_A(ww^*) =$ Sp$'_A(w^*w)$ (I, p. 5, Prop. 1), which is contained in $\mathbf{R}_-$, we conclude that Sp$'_A(w^*w) =\{0\}$. Since $w^*w$ is hermitian, this implies (Cor. 1 of I, p. 108) that $\|w^*w\|=\varrho (w^*w) = 0$, hence that $z^3= 0$. Since $z$ is hermitian, we have $z= 0$. Thus, $x=x^+$ is positive.

#### Remark {#ts-i-s6-n9-rem-1 .statement tag=02EM}

Let A be a star-algebra and let $x\in A$. The element $x^*x$ of A is positive; one then sets $|x|= (x^*x)^{1/2}$. We have $\|x\|^2=\|x^*x\|=$ $\||x|^2\|=\||x|\|^2$, hence $\|x\|=\||x|\|$.

When $x$ is normal, we have also $|x|=f(x)$, where $f$ is the mapping of $\mathbf{C}$ into $\mathbf{C}$, zero at 0, given by $f(z) =|z|$. In particular, when $x$ is hermitian, $|x|$ coincides with the element defined by formula (3).

Suppose moreover that A is unital and that $x$ is invertible. Then $|x|$ is likewise invertible, the element $u=x|x|^{-1}$ is unitary and one has $x=u|x|$ ("polar decomposition"; see also I, p. 139, n$^o8$ for the case of endomorphisms of hilbert spaces).

#### Lemma 14 {#ts-i-s6-lem-14 .statement tag=02EN}

Let A be a star-algebra, and let $x$ and $y$ be hermitian elements of A.

a) If $x\leqslant y$, then for every element $w$ of A, we have $w^*xw\leqslant w^*yw$. In particular, if $y\geqslant 0$, we have $w^*yw\geqslant 0$;

b) Suppose that A is unital. If $0\leqslant x\leqslant y$ and if $x$ is invertible, then $y$ is invertible and $y^{-1}\leqslant x^{-1}$;

c) If $0\leqslant x\leqslant y$ then $\|x\|\leqslant \|y\|$.

Let $u= (y-x)^{1/2}$. We have $w^*yw-w^*xw=w^*u^2w= (uw)^*(uw)$, and assertion a) follows from Theorem 2.

Let us prove assertion b). Suppose first that $x= 1$. Let B be the unital *-subalgebra generated by $y$. By the Gelfand isomorphism, $y$ corresponds to a continuous function $\geqslant 1$ on the compact space $\mathsf{X}(B)$. This function is therefore invertible and its inverse is $\leqslant 1$. This implies that $y$ is invertible and $y^{-1}\leqslant 1 =x^{-1}$. In the general case, we observe that $0\leqslant 1\leqslant x^{-1/2}yx^{-1/2}$ by a), hence the preceding case implies that $z=x^{-1/2}yx^{-1/2}$ is invertible and $z^{-1}\leqslant 1$. Thus $y$ is invertible and $y^{-1}\leqslant x^{-1}$ by a) again.

To prove assertion c), one may suppose that A is unital (Proposition 3 of I, p. 105). Suppose first that $y$ is invertible. Put

$$
\surd -_{1-1}
$$

$b=y$. By a), the conditions $0\leqslant x\leqslant y$ imply $0\leqslant bxb\leqslant$ $b^{-1}yb^{-1}= 1$, hence $\|b^{-1}xb^{-1}\|\leqslant 1$ by Lemma 12, c) of I, p. 116. We then have

$$
\|x\|=\|b(b^{-1}xb^{-1})b\|\leqslant \|b\|\|b^{-1}xb^{-1}\|\|b\|\leqslant \|b\|^2=\|b^2\|=\|y\|
$$

In the general case, for every real $\varepsilon  >0$, the element $y+\varepsilon$ is invertible and $0\leqslant x\leqslant y+\varepsilon$. By what precedes, we therefore have $\|x\|\leqslant \|y+\varepsilon \|$ for every real number $\varepsilon  >0$, whence the result.

#### Remark {#ts-i-s6-n9-rem-2 .statement tag=02EO}

In general, if $x$ and $y$ are positive elements of a *-algebra A, the condition $0\leqslant x\leqslant y$ does not imply $x^2\leqslant y^2($cf. exercise 15 of I, p. 182).

### 10. Approximate Units in *-Algebras

#### Definition 7 {#ts-i-s6-def-7 .statement tag=02EP}

Let A be a normed algebra. An approximate unit of A is a filter basis $\mathfrak{F}$ on the unit ball of A such that, for every $x$ in A, the filter bases $x\mathfrak{F}$ and $\mathfrak{F}x$ on A converge to $x$, in other words:

lim$_{f,\mathfrak{F}}f x=$ lim$_{f,\mathfrak{F}}xf=x$.

If A is a *-algebra, an approximate unit $\mathfrak{F}$ is said to be increasing if $\mathfrak{F}$ is a filter basis on $A_+$.

Let A be a *-algebra. We denote by $A^{\leqslant 1}_+$ (resp. $A^{<1}_+$) the set of positive elements of A of norm $\leqslant 1$ (resp. of norm $<1$); these are the Hermitian elements of A whose spectrum is contained in $[0,1]$ (resp. in $[0,1[$).

#### Proposition 17 {#ts-i-s6-prop-17 .statement tag=02EQ}

Let A be a *-algebra, and let $\mathfrak{F}$ be a filter basis on $A^{\leqslant 1}_+$. For $\mathfrak{F}$ to be an increasing approximate unit of A, it is necessary and sufficient that one have

lim$_{f,\mathfrak{F}}f x=x$

for every positive element $x$ of A.

The condition is obviously necessary; let us prove that it is sufficient. Let $\widetilde{A}$ be the *-algebra deduced from A by adjunction of a unit element. Let $x$ be an element of A and let $f\in A^{\leqslant 1}_+$. We have

$$
\|f x-x\|^2=\|(f x-x)(f x-x)^*\|=\|(f-1)xx^*(f-1)\|
$$

$$
\leqslant \|(f-1)xx^*\|
$$

because $\|f-1\|\leqslant 1$ (Lemma 12, c) of I, p. 116). We therefore have

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant$ lim sup$_{f,\mathfrak{F}}\|f xx^*-xx^*\|$. Since $xx^*$ is positive (Theorem 2 of I, p. 118), the assumption implies that

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant \|xx^*-xx^*\|= 0$,

so that

lim$_{f,\mathfrak{F}}f x=x$.

Since the involution of A is continuous and since $\mathfrak{F}$ is a filter basis on $A_h$, we have

lim$_{f,\mathfrak{F}}xf=$ lim$_{f,\mathfrak{F}}(f^*x^*)^*=$ lim$_{f,\mathfrak{F}}(f x^*)^*= (x^*)^*=x$.

The proposition follows.

#### Proposition 18 {#ts-i-s6-prop-18 .statement tag=02ER}

Let A be an involutive algebra. The ordered set $A^{<1}_+$ is directed to the right (E, III, p. 12, def. 7), and the filter of its sections (TG, I, p. 38, example 2) is an increasing approximate unit of A.

Let $\widetilde{A}$ be the involutive algebra deduced from A by adjunction of a unit element denoted by 1 (def. 4 of I, p. 106).

Let $g$ be the function from $[0,1[$ into $\mathbf{R}_+$ defined by $g(t) =t(1-t)^{-1}$. It is a continuous increasing bijection, its inverse bijection being given by $t\mapsto 1-(1 +t)^{-1}$.

Let us prove that the ordered set $A^{<1}_+$ is directed to the right. Let $x$ and $y$ be elements of $A^{<1}_+$. Since $g(0) = 0$ and since Sp$'_A(x)$ and Sp$'_A(y)$ are contained in $[0,1[$, the elements $g(x)$ and $g(y)$ are defined; they are positive, so that $g(x) +g(y)\geqslant 0$. We can therefore form the element $z=g^{-1}(g(x) +g(y))$ of A. We have Sp$'_A(z)\subset [0,1[$, and hence $z\in A^{<1}_+$.

We have $0\leqslant g(x)\leqslant g(z)$, whence $1\leqslant 1+g(x)\leqslant 1+g(z)$. Assertion b) of lemma 14 of I, p. 119 implies that $1 +g(x)$ and $1 +g(z)$ are invertible and that $(1 +g(z))^{-1}\leqslant (1 +g(x))^{-1}$. Consequently, $z= 1-(1 +g(z))^{-1}\geqslant$ $1-(1 +g(x))^{-1}=x$. Analogously, we have $z\geqslant y$. In consequence, $z$ majorizes $x$ and $y$ in $A^{<1}_+$. The ordered set $A^{<1}_+$ is therefore directed to the right. Let us denote by $\mathfrak{F}$ the filter of its sections

Let $x$ be a positive element of A. For every integer $n\geqslant 1$, let $e_n=$ $g^{-1}(nx)$; we have $e_n\in A^{<1}_+$. Let $h_n$ be the continuous function on $\mathbf{R}_+$ defined for every $t\in \mathbf{R}_+$ by $h_n(t) =t^2(1-g^{-1}(nt)) =t^2/(1 +nt)$. We have $|h_n(t)|\leqslant t/n$ for every $t\geqslant 0$, and hence $\|x(1-e_n)x\|=\|h_n(x)\|\leqslant$ $\|x\|/n$. In particular, $x(1-e_n)x$ tends to 0 when $n$ tends to infinity.

Let $\varepsilon  >0$ be a real number. Let $n$ be an integer such that $\|x(1-e_n)x\|< \varepsilon$. For every $f\in A^{<1}_+$ such that $f\geqslant e_n$, one has then

$$
\|x-f x\|^2=\|(1-f)x\|^2=\|((1-f)x)^*(1-f)x\|=\|x^*(1-f)^2x\|
$$

$$
=\|x(1-f)^2x\|
$$

Moreover, since $0\leqslant f\leqslant 1$, one has $(1-f)-(1-f)^2= (1-f)f\geqslant 0$ (Lemma 12, d) of I, p. 116), hence $(1-f)^2\leqslant 1-f$. Since $1-f\leqslant 1-e_n$, it follows that $0\leqslant (1-f)^2\leqslant 1-e_n$. By Lemma 14, a) and c) of I, p. 119, it follows that

$$
\|x-f x\|^2=\|x(1-f)^2x\|\leqslant \|x(1-e_n)x\|< \varepsilon
$$

Thus lim$_{f,\mathfrak{F}}f x=x$ for every $x\in A_+$. The filter $\mathfrak{F}$ is therefore an approximate unit of A by Proposition 17.

### 11. Quotient by a closed two-sided ideal

#### Lemma 15 {#ts-i-s6-lem-15 .statement tag=02ES}

Let A be a stellar algebra and let I be a closed two-sided ideal of A. Then I is self-adjoint.

Let $J = I\cap I^*$. The set J is a self-adjoint two-sided ideal of A, which contains $I^*I$. In particular, J is a stellar algebra. Let $\mathfrak{F}$ be an increasing approximate unit of J (Prop. 18 of I, p. 121). For every $x\in I$ and every $f\in J^{\leqslant 1}_+$, one has

$$
\|xf-x\|^2=\|(xf-x)^*(xf-x)\|=\|f(x^*xf-x^*x)-(x^*xf-x^*x)\|
$$

$$
\leqslant 2\|x^*xf-x^*x\|
$$

Since $x^*x\in J$, one has therefore

lim$_{f,\mathfrak{F}}\|xf-x\|^2= 0$.

Since $xf\in J$ for every $f\in J^{\leqslant 1}_+$ and since J is closed, this implies that $x\in J$. Hence I = J, and the ideal I is self-adjoint.

#### Proposition 19 {#ts-i-s6-prop-19 .statement tag=02ET}

Let A be a stellar algebra and let I be a closed two-sided ideal of A. Then the quotient involutive Banach algebra $A/I$ is a stellar algebra.

The ideal I is self-adjoint (Lemma 15). Consider the stellar algebra $\widetilde{A}$ deduced from A by adjunction of a unit element (Def. 4 of I, p. 106). In this algebra, the set I is a closed self-adjoint two-sided ideal, and $A/I$ identifies with a closed involutive subalgebra of $\widetilde{A}/I$. One may therefore suppose that A is unital.

The Banach algebra $A/I$ is involutive. Let $\pi : A\rightarrow A/I$ be the canonical projection. The self-adjoint two-sided ideal I is a stellar subalgebra of A. Let $\mathfrak{F}$ be an increasing approximate unit of I (Prop. 18 of I, p. 121). Let us first show that for every $x\in A$, one has

(6) $\|\pi (x)\|_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|$.

On the one hand, since $xf\in I$ for every $f\in I^{\leqslant 1}_+$, one has

$\|\pi (x)\|_{A/I}=$ inf$_{a\in I}\|x-a\|\leqslant$ lim inf$_{f,\mathfrak{F}}\|x-xf\|$.

On the other hand, for every $a\in I$, one has

$$
\|x-xf\|\leqslant \|(x-a)-(x-a)f\|+\|a-af\|
$$

$$
=\|(x-a)(1-f)\|+\|a-af\|
$$

and therefore, since $\|1-f\|\leqslant 1$ (Lemma 12 of I, p. 116) and $a\in I$, one deduces that

lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|x-a\|$.

Thus it follows that lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|\pi (x)\|_{A/I}$ since $a$ is arbitrary in I. Formula (6) is therefore proved.

Now let $x$ be an element of A. By formula (6), one has

$\|\pi (x)\|^2_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|^2=$ lim$_{f,\mathfrak{F}}\|x(1-f)\|^2$

= lim$_{f,\mathfrak{F}}\|(1-f)x^*x(1-f)\|\leqslant$ lim$_{f,\mathfrak{F}}\|x^*x(1-f)\|=\|\pi (x^*x)\|_{A/I}$.

Lemma 6 of I, p. 103 then implies that the quotient involutive Banach algebra $A/I$ is a stellar algebra.

### 12. Enveloping stellar algebra of an involutive Banach algebra

#### Lemma 16 {#ts-i-s6-lem-16 .statement tag=02EU}

Let A be an involutive algebra and let $p$ be a seminorm on A. The following conditions are equivalent :

(i) One has $p(xy)\leqslant p(x)p(y),p(x^*) =p(x)$ and $p(x)^2=p(x^*x)$ for all $x, y\in A$;

(ii) The set R of elements $x$ of A such that $p(x) = 0$ is a two-sided self-adjoint ideal of A, and the seminorm on $A/R$ induced by $p$ makes $A/R$ into a normed involutive algebra whose completion is a stellar algebra;

(iii) There exists a stellar algebra B and a morphism $\varphi$ of involutive algebras from A into B such that $p(x) =\|\varphi (x)\|$ for all $x\in A$.

The implications (i)$=\Rightarrow$ (ii)$=\Rightarrow$ (iii)$=\Rightarrow$ (i) are all elementary.

A seminorm satisfying the conditions of lemma 16 will be called a stellar seminorm on the involutive algebra A.

Let A be a normed involutive algebra and let S be the set of stellar seminorms on A. One has $p(x)\leqslant \|x\|$ for all $x\in A$ and all $p\in S$ (I, p. 104, prop. 2). The mapping $x\mapsto  \|x\|_*=$ sup$_{p\in S}p(x)$ is a

stellar seminorm on A. It is the greatest stellar seminorm on A.

Let R be the set of $x\in A$ such that $\|x\|_*= 0$. It is a closed two-sided ideal of A. We denote by Stell(A) the completed stellar algebra of $A/R$ for the norm induced by $x\mapsto  \|x\|_*$ (lemma 16, (ii)). The canonical mapping of A into Stell(A) is continuous, its image is dense in Stell(A) and its kernel is equal to R.

#### Definition 8 {#ts-i-s6-def-8 .statement tag=02EV}

The stellar algebra Stell(A) is called the enveloping stellar algebra of the normed involutive algebra A.

If A is commutative, then Stell(A) is commutative; if A is unital, then Stell(A) is unital.

#### Proposition 20 {#ts-i-s6-prop-20 .statement tag=02EW}

Let A be a normed involutive algebra and let $j$ be the canonical morphism of A into Stell(A). For every stellar algebra B and every morphism $\varphi$ of involutive algebras from A into B, there exists a unique morphism $\varphi '$ of stellar algebras from Stell(A) into B such that $\varphi =\varphi '\circ j$.

Let us denote by $x\mapsto  \|x\|_*$ the norm on Stell(A). Let R be the kernel of $j$. The mapping $x\mapsto  \|\varphi (x)\|$ is a stellar seminorm on A. Hence one has $\|\varphi (x)\|\leqslant \|x\|_*$ for all $x\in A$. The morphism $\varphi$ therefore defines, by passing to the quotient, a continuous morphism of $A/R$ into B, which extends by continuity to a morphism $\varphi '$ of Stell(A) into B satisfying $\varphi =\varphi '\circ j$. The uniqueness of $\varphi '$ follows from the fact that the image of $j$ is dense in Stell(A).

#### Corollary {#ts-i-s6-n12-cor-1 .statement tag=02EX}

Let A be a commutative involutive Banach algebra and $j$ the canonical morphism of A into Stell(A). The mapping $\mathsf{X}(j)$ is a homeomorphism of $\mathsf{X}$(Stell(A)) onto the subspace $\mathsf{X}(A)_h$ of $\mathsf{X}(A)$ formed by the Hermitian characters of A.

The Hermitian characters of A are the morphisms of involutive algebras from A into the stellar algebra $\mathbf{C}$. Prop. 20 therefore entails that $\mathsf{X}(j)$ is a bijection of $\mathsf{X}$(Stell(A)) onto $\mathsf{X}(A)_h$. Since $\mathsf{X}(j)$ is a homeomorphism onto its image (cf. I, p. 10), the corollary follows.

We identify $\mathsf{X}$(Stell(A)) with $\mathsf{X}(A)_h$ by means of the mapping $\mathsf{X}(j)$. For every $x\in$ A, the mapping $\mathscr{G}_{Stell(A)}(j(x))$ is none other than the restriction of $\mathscr{G}_A(x)$ to $\mathsf{X}(A)_h$.

#### Proposition 21 {#ts-i-s6-prop-21 .statement tag=02EY}

Let A be an involutive Banach algebra and $j$ the canonical morphism of A into Stell(A). The radical of A is contained in the kernel of $j$.

Let $x$ be an element of the radical of A. Then $x^*x$ belongs to the radical of A, and therefore Sp$'_A(x^*x) =\{0\}($I, p. 5, remark 3). Since Sp$'_{Stell(A)}(j(x^*x))\subset$ Sp$'_A(x^*x)$, we therefore have Sp$'_{Stell(A)}(j(x)^*j(x)) =\{0\}$, whence $\|j(x)\|^2=\|j(x)^*j(x)\|=\varrho (j(x)^*j(x)) = 0$ (formula (2) of I, p. 104), and therefore $j(x) = 0$.

### 13. Stellar algebra of a locally compact group

#### Definition 9 {#ts-i-s6-def-9 .statement tag=02EZ}

Let G be a locally compact group and let A be the involutive Banach algebra of bounded measures on G admitting a density with respect to a Haar measure on G (example 4 of I, p. 99). The **stellar algebra** of G is by definition the enveloping stellar algebra of the involutive Banach algebra A. It is denoted by Stell(G).

#### Remark {#ts-i-s6-n13-rem-1 .statement tag=02F0}

Let $\nu$ be a left Haar measure on G and let Δ be its module. The mapping $f\mapsto f\cdot \nu$ is an isometric isomorphism of the algebra $L^1(G, \nu )$ onto A (loc. cit.). Thus one may also define Stell(G) as the enveloping stellar algebra of the involutive normed algebra $L^1(G, \nu )$.

Let G be a locally compact group and let $\nu$ be a left Haar measure on G. For $\mu\in \mathscr{M}^1(G)$ and $f\in L^2(G, \nu )$, one has $\mu*f\in L^2(G, \nu )$ (INT, VIII, §4, prop. 6). Let us then denote by $\boldsymbol{\gamma }(\mu)$ the endomorphism $f\mapsto \mu*f$ of $L^2(G, \nu )$. The mapping $\mu\mapsto \boldsymbol{\gamma }(\mu)$ is a representation of the algebra $\mathscr{M}^1(G)$ in the Banach algebra $\mathscr{L}(L^2(G, \nu ))$ of continuous endomorphisms of $L^2(G, \nu )$ (INT, VIII, §4, cor. to prop. 6). On the other hand, $\boldsymbol{\gamma }(\check{\mu})$ is the transpose of the endomorphism $\boldsymbol{\gamma }(\mu)$ (INT, VIII, §4, n$^o3$, prop. 8). It follows that $\boldsymbol{\gamma }(\mu^*)$ is the adjoint endomorphism of $\boldsymbol{\gamma }(\mu)$, and therefore that the mapping $\boldsymbol{\gamma }:\mu\mapsto \boldsymbol{\gamma }(\mu)$ is a morphism of involutive algebras of $\mathscr{M}^1(G)$ into the stellar algebra $\mathscr{L}(L^2(G, \nu ))$, called the left regular representation of $\mathscr{M}^1(G)$ in $L^2(G, \nu )$. According to INT, VIII, §4, n$^o7$, prop. 19, this representation is faithful.

Let $j$ be the canonical mapping of $L^1(G, \nu )$ into Stell(G). By restriction to $L^1(G, \nu )$, the regular representation $\boldsymbol{\gamma }$ defines an injective morphism of involutive algebras of $L^1(G, \nu )$ into $\mathscr{L}(L^2(G, \nu ))$, called the left regular representation of $L^1(G)$ in $L^2(G)$. According to prop. 20, there exists a unique morphism $\boldsymbol{\gamma }':$ Stell(G) $\rightarrow \mathscr{L}(L^2(G, \nu ))$ such that $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$. One says that $\boldsymbol{\gamma }'$ is the left regular representation of Stell(G) in $L^2(G, \nu )$. By abuse of notation, we shall again write

$$
\boldsymbol{\gamma }'(\varphi )(f) =\varphi *f \tag{7}
$$

for $f\in L^2(G, \nu )$ and $\varphi \in$ Stell(G). One has

$$
\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2 \tag{8}
$$

#### Remark {#ts-i-s6-n13-rem-2 .statement tag=02F1}

In general, the left regular representation $\boldsymbol{\gamma }'$ of Stell(G) in $L^2(G, \nu )$ is not faithful. One can prove that it is so if and only if there exists on $L^{\infty}_{\mathbf{R}}(G)$ a positive linear form $f$ such that $f(1) = 1$ and $f(\boldsymbol{\gamma }(g)x) =f(x)$ for every $(g, x)\in G\times G$ (one then says that the group G is amenable, cf. EVT, IV, p. 73, exercise 4).

#### Proposition 22 {#ts-i-s6-prop-22 .statement tag=02F2}

The canonical mapping $j$ of $L^1(G, \nu )$ into Stell(G) is injective and has dense image.

The image of $j$ is dense by definition of the enveloping star algebra of an involutive normed algebra. Since the left regular representation $\boldsymbol{\gamma }$ is faithful, the injectivity of $j$ follows from the equality $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$.

#### Corollary {#ts-i-s6-n13-cor-1 .statement tag=02F3}

The algebra $L^1(G, \nu )$ is semisimple.

This follows from Prop. 21 of I, p. 125 and Prop. 22.

One may therefore identify $L^1(G, \nu )$ with a dense involutive subalgebra of Stell(G), and the canonical injection of $L^1(G, \nu )$ into Stell(G) is then continuous.

Suppose now that the group G is unimodular (INT, VII, §1, No.$^o3$, Def. 3). One may then repeat the same arguments starting from the right regular representation $(f, \mu)\mapsto \boldsymbol{\delta }(\mu)(f) =f*\check{\mu}$ of $L^2(G, \nu )\times \mathscr{M}^1(G)$ in $L^2(G, \nu )$. One then defines a morphism $\boldsymbol{\delta }'$ of Stell(G) into $\mathscr{L}(L^2(G, \nu ))$ such that $\boldsymbol{\delta }=\boldsymbol{\delta }'\circ j$, and one writes $\boldsymbol{\delta }'(\varphi )(f) =f*\varphi$ for $f\in L^2(G, \nu )$ and $\varphi \in$ Stell(G).

For $\varphi , \psi \in$ Stell(G), one has $\boldsymbol{\delta }'(\psi )\circ \boldsymbol{\gamma }'(\varphi ) =\boldsymbol{\gamma }'(\psi )\circ \boldsymbol{\delta }'(\varphi )$, that is to say

$$
(\varphi *f)*\psi =\varphi *(f*\psi ) \tag{9}
$$

for every $f\in L^2(G, \nu )$. In fact, this formula is true for $\varphi , \psi \in$ $L^1(G, \nu )$, and the mappings $(\varphi , \psi )\mapsto (\varphi *f)*\psi$ and $(\varphi , \psi )\mapsto \varphi *(f*\psi )$ are continuous bilinear mappings of Stell(G) $\times$ Stell(G) into $L^2(G, \nu )$.

## EXERCISES {#ts-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
