---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 3
section_title: Fonctions de type positif
lang: en
source: ts-iii-v-fr
book_pages: TS V.431-TS V.456, TS V.492-TS V.504
pdf_pages: 0444-0469, 0505-0517
extraction: native
subsections:
    - "no": 1
      title: Noyaux universellement positifs
      page: 432
      pdf_page: 445
    - "no": 2
      title: Complément sur le calcul fonctionnel holomorphe
      page: 435
      pdf_page: 448
    - "no": 3
      title: Formes linéaires positives
      page: 436
      pdf_page: 449
    - "no": 4
      title: Représentations des algèbres stellaires
      page: 441
      pdf_page: 454
    - "no": 5
      title: Fonctions de type positif sur un groupe topologique
      page: 442
      pdf_page: 455
    - "no": 6
      title: Dual unitaire d’un groupe localement compact
      page: 446
      pdf_page: 459
    - "no": 7
      title: Existence de représentations irréductibles
      page: 450
      pdf_page: 463
    - "no": 8
      title: Fonctions de type positif sur un groupe localement compact commutatif
      page: 454
      pdf_page: 467
statements: 39
exercises: 23
content_sha256: a6b6b45dafab3a0447148b0aad242724b9c02290041f3925c9ca84a89191bfc2
translated_from: content/fr/ts/V/03_s3_fonctions_de_type_positif.md
source_lang: fr
translation_method: machine
source_content_sha256: cae424d484ec79cb50886a7a6c8ffab98c2adb1922d5abc7d86afcc90df08f8a
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-d0a32535
glossary_version: 34
glossary_terms_sha256: 7da66d6f1f2e8c06e1cd2bda7c3be7aa3d99aa559506435c66e5ec71a51d7816
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. FUNCTIONS OF POSITIVE TYPE

In this paragraph, all vector spaces, as well as all Hilbert spaces and algebras considered, are over $\mathbf{C}$, unless the contrary is stated.

### 1. Universally positive kernels

In this number, X is a separated topological space.

#### Theorem 1 {#ts-v-s3-thm-1 .statement tag=03BX}

Let $f\in \mathscr{C}(X\times X)$. The following conditions are equivalent:

(i) For every compact subset Y of X and every positive measure $\mu$ on Y, the endomorphism of $L^2(Y, \mu)$ defined by the kernel $f|(Y\times Y)$ (Def. 1 of III, p. 29) is positive; in other words, one has

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)\geqslant 0
$$

for every $h\in \mathscr{L}^2(Y, \mu)$;

(ii) For every integer $n\in \mathbf{N}$, every family $(x_i)_{0\leqslant i\leqslant n}$ in X and every family $(t_i)_{0\leqslant i\leqslant n}$ of complex numbers, one has

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

(iii) There exist a complex Hilbert space E and a continuous mapping $g: X\rightarrow E$ with total image such that $f(x, y) =\langle g(x)|g(y)\rangle$ for all $x$ and $y$ in X;

(iv) There exist a complex Hilbert space E and a continuous mapping $g: X\rightarrow E$ such that $f(x, y) =\langle g(x)|g(y)\rangle$ for all $x$ and $y$ in X.

It is apparent that (iii) implies (iv), and one sees that (i) implies (ii) by considering the discrete measure $\mu$ which is the image of the counting measure on $\{0, . . . , n\}$ under the mapping $i\mapsto x_i$ and the function $h$ such that

$$
h(x) =\sum_{0\leqslant i\leqslant n}t_i
$$

$x_i=x$

Let us prove that (iv) implies (i). Suppose that there exist a complex Hilbert space E and a continuous mapping $g: X\rightarrow E$ such that $f(x, y) =\langle g(x)|g(y)\rangle$ for every $(x, y)\in X\times X$. Let Y be a compact subset of $X,\mu$ a positive measure on Y and $h\in \mathscr{L}^2(Y, \mu)$. One has

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)
$$

$$
=\int_{Y\times Y}\overline{h(x)}h(y)\langle g(x)|g(y)\rangle d(\mu\otimes \mu)(x, y)
$$

$$
=\langle\int_Yh(x)g(x)d\mu(x)|\int_Yh(y)g(y)d\mu(y)\rangle\geqslant 0
$$

by INT, V, p. 97, § 8, no$^o4$, Prop. 9.

Finally, let us prove that (ii) implies (iii). Let $\widetilde{E}$ be the space of complex measures with finite support on X. For $\mu_1$ and $\mu_2$ in $\widetilde{E}$, put

$$
\langle \mu_1|\mu_2\rangle =\int_{X\times X}f(x, y) (\overline{\mu}_1\otimes \mu_2)(x, y)
$$

The sesquilinear form resulting on $\widetilde{E}$ is a positive Hermitian form. In fact, let $\mu\in \widetilde{E}$; there exist a finite family $(x_i)_{0\leqslant i\leqslant n}$ in X and complex numbers $(t_i)_{0\leqslant i\leqslant n}$ such that $\mu=\sum^n_{i=0}t_i\varepsilon_{x_i}$. One then has

$$
\langle \mu|\mu\rangle =\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

by hypothesis. Define $\widetilde{g}: X\rightarrow \widetilde{E}$ by $\widetilde{g}(x) =\varepsilon_x$. The image of the mapping $\widetilde{g}$ generates $\widetilde{E}$. Moreover, for every $(x, y)\in X\times X$, one has on the one hand $f(x, y) =\langle \widetilde{g}(x)|\widetilde{g}(y)\rangle$ and on the other hand

$$
\|\widetilde{g}(x)-\widetilde{g}(y)\|^2=f(x, x) +f(y, y)-f(x, y)-f(y, x)
$$

which implies that $\widetilde{g}$ is continuous since $f$ is continuous.

Let E be the separated-completed Hilbert space of $\widetilde{E}$ (EVT, V, p. 8, cor. of the prop. 4) and $g: X\rightarrow E$ the composition of $\widetilde{g}$ and of the canonical mapping $\widetilde{E}\rightarrow E$. Then the mapping $g$ is continuous, its image is total in E, and one has $f(x, y) =\langle g(x)|g(y)\rangle$ for all $(x, y)\in X\times X$.

The method used to prove that (ii) implies (iii) is called the Gelfand–Naimark–Segal construction.

#### Definition 1 {#ts-v-s3-def-1 .statement tag=03BY}

A function $f\in \mathscr{C}(X\times X)$ is said to be a universally positive kernel on X if it satisfies the equivalent conditions of Theorem 1.

If $f$ is a universally positive kernel on X, a pair $(E, g)$ satisfying condition (iv) of loc. cit. is called a Hilbert realization of $f$; if condition (iii) is satisfied, it is said to be a cyclic Hilbert realization.

We denote by Noy$_+(X)$ the set of universally positive kernels on X.

Let $X'$ be a separated topological space and $h: X\rightarrow X'$ a continuous mapping. The mapping $f\mapsto f\circ (h, h)$ from $\mathscr{C}(X'\times X')$ into $\mathscr{C}(X\times X)$ induces, by passing to the subspaces, a mapping Noy$_+(X')\rightarrow$ Noy$_+(X)$.

#### Proposition 1 {#ts-v-s3-prop-1 .statement tag=03BZ}

Let $f$ be a universally positive kernel on X. Let $(E_1, g_1)$ and $(E_2, g_2)$ be Hilbert realizations of $f$. Suppose that $(E_1, g_1)$ is a cyclic Hilbert realization. There then exists a unique continuous linear mapping $u: E_1\rightarrow E_2$ such that $g_2=u\circ g_1$. This mapping is isometric. If $(E_2, g_2)$ is also cyclic, then $u$ is an isomorphism.

The uniqueness of $u$ results from the fact that the image of $g_1$ is total in $E_1$. Let $F =\mathbf{C}^{(X)}$ and let $(e_x)_{x\in X}$ be the canonical basis of F. For $j= 1$ and $j= 2$, denote by $u_j$ the linear mapping from F into $E_j$ determined by $u_j(e_x) =g_j(x)$, and denote by $F_j$ its image; the space $F_1$ is dense in $E_1$.

Let $t=\sum t_xe_x$ be an element of F. One has

$$
\|u_1(t)\|^2=\sum_{x,y}\overline{t}_xt_y\langle g_1(x)|g_1(y)\rangle =\sum_{x,y}\overline{t}_xt_yf(x, y)
$$

$$
=\sum_{x,y}\overline{t}_xt_y\langle g_2(x)|g_2(y)\rangle =\|u_2(t)\|^2
$$

Consequently, there exists an isometric linear mapping $v$ from $F_1$ into $F_2$ such that $u_2=v\circ u_1$, and in particular $g_2(x) =v(g_1(x))$ for all $x\in X$. Since the image of $g_1$ is total in $E_1$, this mapping extends to an isometric linear mapping $u$ from $E_1$ into $E_2$ such that $g_2=u\circ g_1$.

By Lemma 8 of I, p. 107, the image of $u$ is closed in $E_2$. If $(E_2, g_2)$ is a cyclic Hilbertian realization, the image of $u$ is also dense in $E_2$ and $u$ is therefore an isomorphism.

#### Proposition 2 {#ts-v-s3-prop-2 .statement tag=03C0}

The set Noy$_+(X)$ is a self-adjoint cone in the space $\mathscr{C}(X\times X)$; it is stable under product and it is closed when $\mathscr{C}(X\times X)$ is endowed with the topology of simple convergence.

real numberIt is elementary that if$t\geqslant 0$, and that $\frac{f}{f}\in \in$ NoyNoy$_{++}(X)$.(X), then $tf\in$ Noy$_+(X)$ for every

If $(E_1, g_1)$ and $(E_2, g_2)$ are Hilbertian realizations of universally positive kernels $f_1$ and $f_2$ on X, then the pair $(E_1\oplus E_2, g_1+g_2)$ (resp. the pair $(E_1\widehat{\otimes}_2E_2, g_1\otimes g_2)$) is a Hilbertian realization of $f_1+f_2$ (resp. of $f_1f_2$); these are therefore universally positive kernels.

Characterization (ii) of Noy$_+(X)$ (Theorem 1) implies that this set is closed in $\mathscr{C}(X\times X)$ endowed with the topology of simple convergence.

### 2. Supplement on the holomorphic functional calculus

For every subset X of $\mathbf{C}$, $X^*$ denotes the image of X under complex conjugation. Let U be an open subset of $\mathbf{C}$ and $g: U\rightarrow \mathbf{C}$ a holomorphic function. The function $f^*:z\mapsto g(\overline{z})$ is then defined and holomorphic on $U^*$. The mapping $f\mapsto f^*$ is a continuous bijection of $\mathscr{O}(U)$ onto $\mathscr{O}(U^*)$ such that $(f_1f_2)^*=f_1^*f_2^*$ and $(f_1+f_2)^*=f_1^*+f_2^*$ for $f_1$ and $f_2$ in $\mathscr{O}(U)$.

Let C be a compact subset of $\mathbf{C}$. The mappings $f\mapsto f^*$ of $\mathscr{O}(U)$ into $\mathscr{O}(U^*)$, for U ranging over the open subsets of $\mathbf{C}$ containing C, induce a continuous bijection of the space $\mathscr{O}(C)$ onto $\mathscr{O}(C^*)$(I, p. 49, n$^o1$), which is also denoted by $f\mapsto f^*$ and which satisfies $(f_1f_2)^*=f_1^*f_2^*$ and $(f_1+f_2)^*=f_1^*+f_2^*$ for $f_1$ and $f_2$ in $\mathscr{O}(C)$.

#### Proposition 3 {#ts-v-s3-prop-3 .statement tag=03C1}

Let A be a unital involutive Banach algebra. Let $a\in A$. The spectrum of $a^*$ is the image Sp$_A(a)^*$ of Sp$_A(a)$ under complex conjugation. For every $f\in \mathscr{O}$(Sp$_A(a)$), one has $f(a)^*=f^*(a^*)$.

The first assertion follows from I, p. 97. From what precedes, the mapping $\varphi$ of $\mathscr{O}$(Sp$_A(a)$) into A defined by $f\mapsto (f^*(a^*))^*$ is a continuous unital morphism of $\mathscr{O}$(Sp$_A(a)$) into A such that the image of the germ in a neighbourhood of Sp$_A(a)$ of the identity function of $\mathbf{C}$ is equal to $a$. Consequently, $\varphi$ is the mapping $f\mapsto f(a)$ of the holomorphic functional calculus (I, p. 74, th. 5).

#### Lemma 1 {#ts-v-s3-lem-1 .statement tag=03C2}

Let D be the open unit disk in $\mathbf{C}$. There exists a unique holomorphic function $f$ defined on D such that $f(z)^2= 1-z$ for every $z\in D$ and $f(0) = 1$. One has $f^*=f$.

The radius of convergence of the power series

$$
^{+\infty}(1/2)_n
$$

$$
\sum(-z)
$$

$$
n
$$

$n=0$

is equal to 1 and its sum $f$ defines a holomorphic function on D (VAR,

$$
\surd
$$

R1, p. 27, 3.2.9) taking the value 1 at 0. It satisfies $f(x) =1-x$ for every $x\in D\cap \mathbf{R}$ (FVR, III, p. 19), hence $f(z)^2= 1-z$ for $z\in D$ since the difference $f(z)^2-(1-z)$ is a holomorphic function all of whose successive derivatives vanish at 0 (VAR, R1, p. 27, 3.2.5). By definition, one verifies that $f^*=f$.

Let $g$ be a holomorphic function on D such that $g(z)^2= 1-z$ for every $z\in D$ and such that $g(0) = 1$. The function $g$ does not vanish and the continuous function $f /g$ on D takes its values in $\{-1,1\}$; since D is connected and $f(0) =g$(0), one has $f=g$.

### 3. Positive linear forms

#### Definition 2 {#ts-v-s3-def-2 .statement tag=03C3}

Let A be an involutive algebra. A linear form $\lambda$ on A is said to be positive if $\lambda (a^*a)\in \mathbf{R}_+$ for every $a\in A$.

If A is an involutive Banach algebra, one denotes by $A'_+$ the set of continuous positive linear forms on A.

Let A be an involutive Banach algebra. The set $A'_+$ is a pointed convex cone in the real vector space of $\mathbf{C}$-linear forms on A.

#### Lemma 2 {#ts-v-s3-lem-2 .statement tag=03C4}

Let A be an involutive Banach algebra and $\lambda$ a positive linear form on A.

a) For all $a$ and $b$ in A, one has $\lambda (a^*b) =\overline{\lambda(b^*a)}$ and

$$
|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)
$$

b) If A is unital, then the linear form $\lambda$ is continuous and its norm is equal to $\lambda (1)$.

The mapping $(a, b)\mapsto \lambda (a^*b)$ is a positive Hermitian form on A; it therefore satisfies $\lambda (a^*b) =\lambda (b^*a)$ and $|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)$ for all $a$ and $b$ in A (EVT, V, p. 2, remark and p. 3, prop. 2).

Let us prove b). Let $a\in A$ be a hermitian element of norm $<1$. The spectral radius of $a$ is less than $\|a\|$, hence the spectrum of $a$ is contained in the open unit disc D of $\mathbf{C}$ (Theorem 1 of I, p. 24). Let $f$ be a holomorphic function on D such that $f(z)^2= 1-z$ for all $z\in D$ (Lemma 1 of V, p. 435). Applying the holomorphic functional calculus to the element $a$ and to the function $f$, the element $b=f(a)$ satisfies $b^2= 1-a($I, p. 74, Theorem 5). By Prop. 3 of V, p. 435, one moreover has $f(a)^*=f^*(a^*) =f(a)$, hence $b$ is hermitian. We then have $\lambda (1-a) =\lambda (b^*b)\geqslant 0$, whence $\lambda (a)\leqslant \lambda (1)$.

Now let $b\in A$ be of norm $<1$. The element $b^*b$ is hermitian and $\|b^*b\|<1$, hence applying a) with $a= 1$, we find

$$
|\lambda (b)|^2\leqslant \lambda (1)\lambda (b^*b)\leqslant \lambda (1)^2
$$

with equality if $b= 1$. The linear form $\lambda$ is therefore continuous, and its norm is equal to $\lambda (1)$. Assertion b) is proved.

#### Example {#ts-v-s3-n3-exa-1 .statement tag=03C5}

Let X be a compact topological space and let A be the star-algebra $\mathscr{C}(X)$. Positive linear forms on A are identified with positive measures on X (INT, III, p. 52, § 1, n$^o6$, Theorem 1).

#### Lemma 3 {#ts-v-s3-lem-3 .statement tag=03C6}

Let A be a unital involutive Banach algebra admitting an approximate unit (I, p. 120, Definition 7). Let $\lambda$ be a continuous positive linear form on A.

a) For every $a$ in A, one has $\lambda (a^*) =\overline{\lambda(a)}$ and $|\lambda (a)|^2\leqslant \|\lambda \|\lambda (a^*a)$;

b) Let $\widetilde{A}$ be the involutive algebra obtained from A by adjunction of a unit element, and let $e$ be its unit element. There exists a continuous positive linear form $\widetilde{\lambda}$ on $\widetilde{A}$ extending $\lambda$ and such that $\widetilde{\lambda}(e) =\|\lambda \|$;

c) For all $a$ and $b$ in A, one has $|\lambda (b^*ab)|\leqslant \|a\|\lambda (b^*b)$.

Let us prove a). Let $\mathfrak{F}$ be an approximate unit of A. Let $a\in A$. Using Lemma 2, a) and the definition of an approximate unit, one finds

$\lambda (a^*) =$ lim$_{f,\mathfrak{F}}\lambda (f a^*) =$ lim$_{f,\mathfrak{F}}\lambda (af^*) =$ lim$_{f,\mathfrak{F}}\lambda ((f a^*)^*) =\overline{\lambda(a)}$,

whence (loc. cit.)

$|\lambda (a)|^2=$ lim$_{f,\mathfrak{F}}|\lambda (f a)|^2\leqslant \lambda (a^*a)$ lim sup$_{f,\mathfrak{F}}\lambda (f f^*)\leqslant \|\lambda \|\lambda (a^*a)$,

since $\mathfrak{F}$ is a filter on the unit ball of A.

To prove b), one may suppose that $\lambda$ is not zero, then that $\|\lambda \|= 1$. For $a\in A$ and $z\in \mathbf{C}$, let us put $\widetilde{\lambda}(a+z\cdot e) =\lambda (a) +z$. The mapping $\widetilde{\lambda}$ is a continuous linear form on $\widetilde{A}$ which extends $\lambda$ and satisfies $\widetilde{\lambda}(e) = 1$. It is positive: for all $a\in A$ and $z\in \mathbf{C}$, by a), we calculate

$$
\widetilde{\lambda}((a+z\cdot e)^*(a+z\cdot e)) =\lambda (a^*a) +z\lambda (a) +z\lambda (a^*) +|z|^2
$$

$$
=|z+\lambda (a)|^2+\lambda (a^*a)- |\lambda (a)|^2\geqslant 0
$$

Finally, let $b$ be an element of A. The mapping $a\mapsto \widetilde{\lambda}(b^*ab)$ is a positive linear form on the unital involutive Banach algebra $\widetilde{A}$. It is therefore continuous of norm equal to its value at $e$ (Lemma 2, b)), which is equal to $\lambda (b^*b)$, whence assertion c).

#### Proposition 4 {#ts-v-s3-prop-4 .statement tag=03C7}

Let A be an involutive Banach algebra.

a) For every Hilbert space E, every morphism of involutive algebras $\varphi : A\rightarrow \mathscr{L}(E)$ and every vector $x\in E$, the linear form defined on A by $\lambda (a) =\langle x|\varphi (a)x\rangle$ is a continuous positive linear form;

b) Let $\lambda \in A'_+$. The mapping $f$ of $A\times A$ into $\mathbf{C}$ defined by $f(a, b) =$ $\lambda (a^*b)$ for every $(a, b)\in A\times A$ is a universally positive kernel on A.

Let us prove a). For every $a\in A$, one has

$$
\lambda (a^*a) =\langle x|\varphi (a^*a)x\rangle =\|\varphi (a)x\|^2\geqslant 0
$$

therefore $\lambda$ is a positive linear form on A; it is continuous since $\varphi$ is continuous (Prop. 2 of I, p. 104).

Let us prove b). The function $f$ is continuous. For every $n\in \mathbf{N}$, every family $(a_i)_{0\leqslant i\leqslant n}$ in A and every family $(t_i)_{0\leqslant i\leqslant n}$ of complex numbers, one has

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(a_i, a_j) =\lambda ((\sum_{i=0}^nt_ia_i)^*(\sum_{j=0}^nt_ja_j))\geqslant 0
$$

whence the result (Def. 1 of V, p. 433).

#### Definition 3 {#ts-v-s3-def-3 .statement tag=03C8}

Let A be an involutive Banach algebra. Let $\lambda \in A'_+$ be a continuous positive linear form on A. A Hilbertian realization of $\lambda$ is by definition a triple $(E, x, \varphi )$ consisting of a Hilbert space E, an element $x$ of E and a morphism of involutive algebras $\varphi$ of A into $\mathscr{L}(E)$, such that $\lambda (b^*a) =\langle \varphi (b)x|\varphi (a)x\rangle$ for every $(a, b)\in A^2$.

If the set of elements $\varphi (a)x$ for $a\in A$ is total in E, one says that $(E, x, \varphi )$ is a cyclic Hilbertian realization of $\lambda$.

#### Proposition 5 {#ts-v-s3-prop-5 .statement tag=03C9}

Let A be an involutive Banach algebra admitting an approximate unit. Every continuous positive linear form on A admits a cyclic Hilbertian realization $(E, x, \varphi )$. If A is unital, then there exists such a realization in which the morphism $\varphi$ is unital.

One may suppose that A is a unital algebra (Lemma 3, b)).

Let $\lambda$ be a continuous positive linear form on A. Let $(E, g)$ be a cyclic Hilbertian realization of the universally positive kernel $f$ on A defined by $f(a, b) =\lambda (a^*b)$ (Prop. 4 and Theorem 1). The mapping $g$ is continuous, its image is total in E, and one has $\lambda (a^*b) =\langle g(a)|g(b)\rangle$ for every $(a, b)\in A^2$. Put $x=g(1)\in E$.

The mapping $g$ of A into E is linear: in fact, for $(a, b, c)\in A^3$ and $(s, t)\in \mathbf{C}^2$, we have

$$
\langle g(c)|g(sa+tb)\rangle =\lambda (c^*(sa+tb))
$$

$$
=s\lambda (c^*a) +t\lambda (c^*b) =\langle g(c)|sg(a) +tg(b)\rangle
$$

whence the assertion, since the image of $g$ is total in E.

In particular, the image F of $g$ is a dense vector subspace of E. The kernel of $g$ is a left ideal of A: if $g(b) = 0$, then for all $a$ and $c$ in A, we have

$$
\langle g(ab)|g(c)\rangle =\lambda ((ab)^*c) =\lambda (b^*(a^*c)) =\langle g(b)|g(a^*c)\rangle = 0
$$

therefore $g(ab) = 0$ since F is dense in E.

Let $a\in A$. Since the kernel of $g$ is a left ideal of A, there exists a linear mapping $\widetilde{\varphi}(a) : F\rightarrow F$ such that $\widetilde{\varphi}(a)(g(b)) =g(ab)$ for every $b\in A$. Moreover, for every $b\in A$, we have

$$
\|\widetilde{\varphi}(a)(g(b))\|^2=\|g(ab)\|^2=\lambda (b^*a^*ab)\leqslant \|a^*a\|\lambda (b^*b)\leqslant \|a\|^2\|g(b)\|^2
$$

(lemma 3, c)), therefore $\widetilde{\varphi}(a)$ is continuous and of norm $\leqslant \|a\|$. Consequently, there exists a unique endomorphism $\varphi (a)\in \mathscr{L}(E)$ which induces $\widetilde{\varphi}(a)$ by passing to the subspaces.

Let $a$ and $b$ be in A. We have

$$
(\varphi (a)\circ \varphi (b))(g(c)) =g(abc) =\varphi (ab)(g(c))
$$

for every $c$ in A, therefore $\varphi (ab) =\varphi (a)\circ \varphi (b)$ since F is dense in E.

The mapping $\varphi$ of A into $\mathscr{L}(E)$ is linear: in fact, for every $(a, b)\in A^2$ and every $(s, t)\in \mathbf{C}^2$, we have

$$
\varphi (sa+tb)(g(c)) =g((sa+tb)c) = (s\varphi (a) +t\varphi (b))g(c)
$$

for every $c\in A$, whence $\varphi (sa+tb) =s\varphi (a) +t\varphi (b)$ since F is dense in E. Since $\|\varphi (b)\|\leqslant \|b\|$ for every $b\in A$, the mapping $\varphi$ is continuous. We also have $\varphi (1) = 1_E$ since $\varphi (1)(g(a)) =g(a)$ for every $a\in A$ and F is dense in E.

Lastly, let $a,b,c$ be in A. We have

$$
\langle g(c)|\varphi (a^*)(g(b))\rangle =\langle g(c)|g(a^*b)\rangle =\lambda (c^*a^*b)
$$

$$
=\langle g(ac)|g(b)\rangle =\langle \varphi (a)(g(c))|g(b)\rangle
$$

whence $\varphi (a^*) =\varphi (a)^*$ since F is dense in E.

In conclusion, the mapping $\varphi$ is a continuous morphism of involutive algebras of A into $\mathscr{L}(E)$ and $g(a) =\varphi (a)x$ for every $a\in A$; consequently, the triplet $(E, x, \varphi )$ is a cyclic Hilbertian realization of $\lambda$.

#### Proposition 6 {#ts-v-s3-prop-6 .statement tag=03CA}

Let A be an involutive Banach algebra and let $\lambda$ be a continuous positive linear form on A. Let $(E_1, x_1, \varphi_1)$ and $(E_2, x_2, \varphi_2)$ be Hilbertian realizations of $\lambda$. Suppose that $(E_1, x_1, \varphi_1)$ is a cyclic Hilbertian realization.

a) There exists a unique continuous linear mapping $u$ from $E_1$ into $E_2$ which is a morphism of representations of $\varphi_1$ into $\varphi_2($I, p. 11) and which satisfies $u(\varphi_1(a)x_1) =\varphi_2(a)x_2$ for every $a\in A$;

b) The linear mapping $u$ is isometric;

c) If $(E_2, x_2, \varphi_2)$ is cyclic, then $u$ is an isomorphism;

d) If $(E_2, x_2, \varphi_2)$ is cyclic and if A is unital, then $u(x_1) =x_2$.

For $j\in  \{1,2\}$, define $\gamma_j: A\rightarrow E_j$ by $\gamma_j(a) =\varphi_j(a)x_j$ for every $a\in A$. By definition, the pairs $(E_j, \gamma_j)$ are Hilbertian realizations of the universally positive kernel $f$ on A defined by $(a, b)\mapsto \lambda (a^*b)$. The Hilbertian realization $(E_1, \gamma_1)$ is cyclic; by prop. 1 of V, p. 434, there exists therefore a unique continuous linear mapping $u: E_1\rightarrow E_2$ such that $\gamma_2=u\circ \gamma_1$, and this mapping is isometric. Moreover, if $(E_2, x_2, \varphi_2)$ is also cyclic, then $u$ is an isomorphism. To prove a), b) and c), it is enough to prove that $u$ is a morphism of representations of $\varphi_1$ into $\varphi_2$.

Let $a\in A$. For every $b\in A$, we have

$$
(u\circ \varphi_1(a))(\gamma_1(b)) = (u\circ \varphi_1(ab))x_1= (u\circ \gamma_1)(ab)
$$

$$
=\gamma_2(ab) =\varphi_2(a)(\gamma_2(b)) =\varphi_2(a)(u(\gamma_1(b)))
$$

therefore the continuous linear mappings $u\circ \varphi_1(a)$ and $\varphi_2(a)\circ u$ coincide on the subspace of $E_1$ generated by the image of $\gamma_1$; this subspace is dense in $E_1$ by hypothesis, whence $u\circ \varphi_1(a) =\varphi_2(a)\circ u$.

Finally, let us prove d). Suppose therefore that A is unital and that $(E_2, x_2, \varphi_2)$ is cyclic. There exists a cyclic Hilbertian realization $(E_3, x_3, \varphi_3)$ of $\lambda$ such that $\varphi_3$ is a unital morphism (prop. 5). Let $j\in  \{1,2\}$. Applying the foregoing to $(E_j, x_j, \varphi_j)$ and $(E_3, x_3, \varphi_3)$, we see that there exists an isometric isomorphism $\widetilde{u}_j$ of $E_j$ into $E_3$ such that $\widetilde{u}_j\circ \varphi_j(a) =\varphi_3(a)\circ \widetilde{u}_j$ for every $a\in A$. Taking $a= 1_A$, we see that $\varphi_j$ is unital. We then have $x_2=\varphi_2(1_A)x_2=u(\varphi_1(1_A)x_1) =u(x_1)$.

#### Remark {#ts-v-s3-n3-rem-1 .statement tag=03CB}

Retain the notation of the proposition. It is possible that $u(x_1)$ is different from $x_2$ (exercise 3, b) of V, p. 493). However, the triplet $(E_2, u(x_1), \varphi_2)$ is also a Hilbert representation of $\lambda$.

### 4. Representations of star algebras

Let A be a star algebra. Let $A_+$ denote the closed convex cone of positive elements of A (def. 6 of I, p. 115). A linear form $\lambda$ on A is positive if and only if $\lambda (A_+)\subset \mathbf{R}_+($I, p. 118, th. 2).

#### Proposition 7 {#ts-v-s3-prop-7 .statement tag=03CC}

Let A be a star algebra. Every positive linear form $\lambda$ on A is continuous.

Let us first prove that $\lambda$ is bounded on the intersection of $A_+$ and the unit ball of A. Suppose this is not so. Then there exists a sequence $(x_n)_{n\geqslant 1}$ in $A_+$ such that $\|x_n\|\leqslant 1$ and $\lambda (x_n)\geqslant n$ for every integer $n\geqslant 1$. The series with general term $n^{-2}x_n$ converges to an element $x$ of A (cf. TG, IV, p. 33, Example 3). For every integer $N\geqslant 1$, since

$+\infty$

$\sum\frac{1}{n^2}x_n\in A_+$,

$n=N+1$

(I, p. 116, Prop. 14), it follows that

N N $+\infty$

$\sum\frac{1}{n}\leqslant \sum\frac{1}{n^2}\lambda (x_n) =\lambda (x)-\lambda (\sum\frac{1}{n^2}x_n)\leqslant \lambda (x)$,

$n=1n=1n=N+1$

which is absurd (TG, IV, p. 33, Example 4).

Since every element of the unit ball of A is a linear combination with coefficients bounded by 1 of at most four positive elements of A of norm $\leqslant 1$(I, p. 96, Lemma 2 and formula (4) of I, p. 117), we conclude that $\lambda$ is continuous.

There exist involutive Banach algebras which admit positive linear forms that are not continuous (Exercise 3, (a) of V, p. 493).

#### Proposition 8 {#ts-v-s3-prop-8 .statement tag=03CD}

Let A be a stellar algebra and $a$ a nonzero element of A. There exists a positive linear form $\lambda \in A'_+$ such that $\lambda (a^*a)>0$.

Consider the real Banach space $A_h$ of hermitian elements of A. The set $A_+$ is a salient pointed closed convex cone in $A_h$ (Prop. 14 of I, p. 116). The element $a^*a$ is positive (Theorem 2 of I, p. 118) and nonzero; hence the hermitian element $-a^*a$ is therefore not positive. By EVT, II, p. 42, Cor. 5, there exists a continuous real linear form $\lambda \in A'_h$ such that $\lambda (-a^*a)<0$ and $\lambda (A_+)\subset \mathbf{R}_+$. The linear form $\lambda$ extends to a hermitian $\mathbf{C}$-linear form on A (cf. I, p. 98), which is positive and has the required property.

#### Theorem 2 (Gelfand–Naimark) {#ts-v-s3-thm-2 .statement tag=03CE}

Let A be a stellar algebra. There exist a Hilbert space E and an isometric morphism of involutive algebras $\varphi$ of A into $\mathscr{L}(E)$. If A is unital, there exists such a unital morphism.

For every $b\in A-\{0\}$, let $\lambda_b$ be a continuous positive linear form on A such that $\lambda_b(b^*b)>0$ (Prop. 8). Since A admits an approximate unit (I, p. 121, Prop. 18), there exists a Hilbert realization $(E_b, x_b, \varphi_b)$ of $\lambda_b$ (Prop. 5). If A is unital, one may suppose that $\varphi_b$ is unital (loc. cit.). We have $\|\varphi_b(b)\|^2=\lambda_b(b^*b)\not = 0$.

Let E be the external Hilbert sum of the spaces $E_b$ for $b$ belonging to A $-\{0\}$. For every $a\in A$, let us denote by $\varphi (a)\in \mathscr{L}(E)$ the unique continuous linear mapping whose restriction to $E_b$ coincides with $\varphi_b(a)$ for every $b\in A-\{0\}$. The mapping $a\mapsto \varphi (a)$ is a morphism of involutive algebras; it is injective, hence isometric (Prop. 9 of I, p. 112), and satisfies $\varphi (1) = 1_E$ if A is unital. This completes the proof.

*The category whose objects are stellar algebras and whose morphisms are morphisms of involutive algebras is therefore equivalent to the category whose objects are closed involutive subalgebras of the algebras of endomorphisms of Hilbert spaces, and whose morphisms are morphisms of involutive algebras.*

### 5. Functions of positive type on a topological group

In this number, G is a topological group whose unit element is denoted by $e$. The Hilbert spaces considered are complex.

#### Definition 4 {#ts-v-s3-def-4 .statement tag=03CF}

A continuous function $\varphi \in \mathscr{C}(G)$ is said to be of positive type on G if the function $f$ defined by $f(g, h) =\varphi (g^{-1}h)$ on $G\times G$ is a universally positive kernel on G.

Pos(G) denotes the set of functions of positive type on G, and Pos$_1(G) ($resp. Pos$_{\leqslant 1}(G))$ denotes the subset of $\varphi \in$ Pos(G) such that $\varphi (e) = 1 ($resp. such that $\varphi (e)\leqslant 1)$.

#### Example {#ts-v-s3-n5-exa-1 .statement tag=03CG}

Let $\varrho$ be a unitary representation of G in a Hilbert space E and let $x\in E$. Let $\varphi$ be the diagonal matrix coefficient defined by $\varphi (g) =\langle x|\varrho (g)x\rangle$ for all $g\in G$; the function $\varphi$ is continuous. We have

$$
\varphi (g^{-1}h) =\langle x|\varrho (g)^*\varrho (h)x\rangle =\langle \varrho (g)x|\varrho (h)x\rangle
$$

for all $(g, h)\in G\times G$. Consequently $\varphi \in$ Pos(G) (Theorem 1 of V, p. 432, (iv)). One has $\varphi \in$ Pos$_1(G)$ if and only if $\|x\|= 1$.

#### Definition 5 {#ts-v-s3-def-5 .statement tag=03CH}

Let $\varphi$ be a function of positive type on G. A Hilbert realization of $\varphi$ is a pair $(\varrho , x)$ where $\varrho$ is a unitary representation of G in a Hilbert space E and $x\in E$, such that $\varphi (g) =\langle x|\varrho (g)x\rangle$ for all $g\in G$.

If $x$ is a cyclic vector of $\varrho$, one says that this is a cyclic Hilbert realization of $\varphi$.

#### Proposition 9 {#ts-v-s3-prop-9 .statement tag=03CI}

Let $\varphi \in \mathscr{C}(G)$. The following conditions are equivalent:

(i) The function $\varphi$ is of positive type on G;

(ii) There exists a cyclic Hilbert realization of $\varphi$;

(iii) There exists a Hilbert realization of $\varphi$.

Condition (ii) implies condition (iii), and condition (iii) implies (i) by the above example.

Let us prove finally that (i) implies (ii). Let $(E, \gamma )$ be a cyclic Hilbert realization of the universally positive kernel defined by $f(g, h) =\varphi (g^{-1}h)$ for $(g, h)\in G\times G$. Let $k\in G$. The continuous function $\gamma_k:g\mapsto \gamma (kg)$ on G satisfies

$$
\langle \gamma_k(g)|\gamma_k(h)\rangle =\langle \gamma (kg)|\gamma (kh)\rangle =f(kg, kh) =\varphi ((kh)^{-1}kg) =f(g, h)
$$

for all $(g, h)\in G\times G$, hence $(E, \gamma_k)$ is a Hilbert realization of $f$. By Prop. 1 of V, p. 434, there exists a unique unitary element $\varrho (k)$ in $\mathscr{L}(E)$ such that $\gamma_k=\varrho (k)\circ \gamma$. For all $g\in G$, and all $(k_1, k_2)\in G\times G$, we have

$$
\varrho (k_1k_2)(\gamma (g)) =\gamma (k_1k_2g) =\varrho (k_1)(\varrho (k_2)(\gamma (g)))
$$

whence $\varrho (k_1k_2) =\varrho (k_1)\varrho (k_2)$ since the image of $\gamma$ is a total subset of E.

Let $k\in G$. For all $g\in G$, one has $\varrho (g)(\gamma (k)) =\gamma (gk)$, and the mapping from G into E defined by $g\mapsto \varrho (g)(\gamma (k))$ is therefore continuous. Since the endomorphism $\varrho (g)$ is unitary, it follows that $\varrho$ is a unitary representation of G in E (Lemma 4 of V, p. 380). Put then $x=\gamma (e)$. The set of vectors $\varrho (g)x=\varrho (g)(\gamma (e)) =\gamma (g)$ for $g$ ranging over G is total in E, therefore $x$ is a cyclic vector of $\varrho$. Since

$$
\langle x|\varrho (g)x\rangle =f(e, g) =\varphi (g)
$$

for all $g\in G$, the pair $(\varrho , x)$ is a cyclic Hilbert realization of $\varphi$.

#### Proposition 10 {#ts-v-s3-prop-10 .statement tag=03CJ}

Let $\varphi$ be a function of positive type on G and let $(\varrho_1, x_1)$ and $(\varrho_2, x_2)$ be Hilbertian realizations of $\varphi$, the Hilbertian representation $(\varrho_1, x_1)$ being cyclic. There exists a unique isometric G-morphism $u$ of $\varrho_1$ into $\varrho_2$ such that $u(x_1) =x_2$. If $(\varrho_2, x_2)$ is also cyclic, then $u$ is an isomorphism.

For $1\leqslant j\leqslant 2$, let us denote by $E_j$ the space of $\varrho_j$ and by $\gamma_j$ the function on G defined by $\gamma_j(g) =\varrho_j(g)x_j$ for every $g\in G$. The pairs $(E_1, \gamma_1)$ and $(E_2, \gamma_2)$ are Hilbertian realizations of the function of positive type $(g, h)\mapsto \varphi (g^{-1}h)$, and $(E_1, \gamma_1)$ is a cyclic Hilbertian realization. By Prop. 1 of V, p. 434, there exists a unique isometric linear mapping $u: E_1\rightarrow E_2$ such that $\gamma_2=u\circ \gamma_1$. In particular, one has $x_2=\gamma_2(e) =u(\gamma_1(e)) =u(x_1)$. Moreover, for all $g$ and $h$ in G, one has

$$
\varrho_2(g)u(\gamma_1(h)) =\varrho_2(g)\gamma_2(h) =\gamma_2(gh) =u(\gamma_1(gh)) =u(\varrho_1(g)\gamma_1(h))
$$

and since the set of elements $\gamma_1(h)$ for $h\in G$ is total in $E_1$, this means that $u$ is a G-morphism. By loc. cit., it is an isometric isomorphism if $(\varrho_2, x_2)$ is also cyclic.

#### Proposition 11 {#ts-v-s3-prop-11 .statement tag=03CK}

Let $\varphi \in$ Pos$_1(G)$ and let $(\varrho , x)$ be a cyclic Hilbertian realization of $\varphi$. Then $\varrho$ is an irreducible representation of G if and only if $\varphi$ is an extreme point (EVT, II, p. 57, def. 1) of Pos$_1(G)$.

Let E be the space of $\varrho$. Suppose first that $\varrho$ is not irreducible. Let F be a nonzero closed subspace of E, stable under $\varrho$, and different from E. Let us write $x=x_1+x_2$, where $x_1\in F$ and $x_2\in F^{\circ}$. Then one has $1 =\|x\|^2=\|x_1\|^2+\|x_2\|^2$. The subrepresentation of E generated by $x_1$ is contained in F, hence $x_1\not =x$ since $x$ is a cyclic vector of $\varrho$, whence $x_2\not = 0$. Analogously one verifies that $x_1\not = 0$.

For $j= 1$ and $j= 2$, let us denote by $\varphi_j$ the continuous function on G such that

$$
\varphi_j(g) =\frac{1}{\|x_j\|^2}\langle x_j|\varrho (g)x_j\rangle
$$

for all $g\in G$. One has $\varphi_j\in$ Pos$_1(G)$(V, p. 443, example). Since $\varphi =\|x_1\|^2\varphi_1+\|x_2\|^2\varphi_2$, it is enough to verify that $\varphi_1\not =\varphi_2$ in order to prove that $\varphi$ is not an extreme point of Pos$_1(G)$; for this it is enough to prove that $\varphi \not =\varphi_1$.

Arguing by contradiction, suppose that $\varphi =\varphi_1$. Since one has $\langle x_1|\varrho (g)x_2\rangle = 0$ for all $g\in G$, it would follow that

$$
\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x\rangle =\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x_1\rangle =\varphi_1(g) =\varphi (g) =\langle x|\varrho (g)x\rangle
$$

for all $g\in G$, whence $\langle x_1|y\rangle =\langle \|x_1\|^2x|y\rangle$ for every element $y$ of the vector subspace of E generated by the elements $\varrho (g)x$ for $g\in G$, hence for all $y\in E$ since $x$ is a cyclic vector of $\varrho$. This would imply that $x_1=\|x_1\|^2x$ is also a cyclic vector of $\varrho$, which is a contradiction, whence the assertion.

Now suppose that $\varrho$ is irreducible, and prove that $\varphi$ is an extreme point of Pos$_1(G)$. Let $\varphi_1\not =\varphi_2$ be elements of Pos$_1(G)$ and let $t_1,t_2\in [0,1]$ be such that $t_1+t_2= 1$ and $\varphi =t_1\varphi_1+t_2\varphi_2$. For $j\in  \{1,2\}$, let $(\varrho_j, x_j)$ denote a cyclic Hilbert realization of $\varphi_j$, and let $E_j$ denote the space of $\varrho_j$. Let $x_3=t^{1/2}_1x_1+t^{1/2}_2x_2$. Then $(\varrho_1\oplus \varrho_2, x_3)$ is a Hilbert realization of $\varphi$. Since $(\varrho , x)$ is cyclic, there exists an isometric G-morphism $u: E\rightarrow E_1\oplus E_2$ such that $u(x) =x_3$ (Prop. 10).

Let $j= 1$ or $j= 2$. Since $\varrho$ is irreducible, there exists $\lambda_j\geqslant 0$ such that the G-morphism $u_j=$ pr$_j\circ u$ of E into $E_j$ satisfies

$$
\langle u_j(y)|u_j(y')\rangle =\lambda_j\langle y|y'\rangle
$$

for all $y$ and $y'$ in E (Cor. 5 of V, p. 388, if $u_j\not = 0$, and one may take $\lambda_j= 0$ otherwise). For all $g\in G$, one has

$$
t_j\varphi_j(g) =\langle t^{1/2}_jx_j|\varrho_j(g)(t^{1/2}_jx_j)\rangle =\langle u_j(x)|\varrho_j(g)(u_j(x))\rangle
$$

$$
=\langle u_j(x)|u_j(\varrho (g)x)\rangle =\lambda_j\varphi (g)
$$

Since $\varphi_j(e) =\varphi (e) = 1$, it follows that $\varphi_j=\varphi$ if $t_j\not = 0$. The assumption $\varphi_1\not =\varphi_2$ therefore implies that $t_1$ or $t_2$ must be zero, which proves that $\varphi$ is an extreme point of Pos$_1(G)$.

#### Lemma 4 {#ts-v-s3-lem-4 .statement tag=03CL}

Let $\varphi \in$ Pos(G). The function $\varphi$ is bounded on G and one has $\|\varphi \|_{\infty}=\varphi (e)$. Moreover, one has

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \surd\overline{2\varphi(e)(\varphi(e) -\mathscr{R}(\varphi(g)))} \tag{1}
$$

for every $(g, h)\in G\times G$.

Let $(\varrho , x)$ be a Hilbert realization of $\varphi$. One has $\varphi (e) =\|x\|^2$. For every $g\in G$, one therefore has $|\varphi (g)|=|\langle x|\varrho (g)x\rangle |\leqslant \varphi (e)$ by the Cauchy-Schwarz inequality. This proves the first assertion.

For every $(g, h)\in G\times G$, one has

$$
\varphi (g^{-1}h)-\varphi (h) =\langle x|\varrho (g^{-1}h)x\rangle  - \langle x|\varrho (h)x\rangle =\langle \varrho (g)x-x|\varrho (h)x\rangle
$$

since $\varrho$ is unitary, whence

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \|\varrho (g)x-x\|\|\varrho (h)x\|\leqslant \varphi (e)^{1/2}\|\varrho (g)x-x\|
$$

We conclude by observing that

$$
\|\varrho (g)x-x\|^2= 2\|x\|^2-2\mathscr{R}(\langle x|\varrho (g)x\rangle ) = 2(\varphi (e)-\mathscr{R}(\varphi (g)))
$$

#### Remark {#ts-v-s3-n5-rem-1 .statement tag=03CM}

The sets Pos(G) (resp. Pos$_1(G)$ and Pos$_{\leqslant 1}(G)$) are self-adjoint convex subsets of the involutive algebra $\mathscr{C}_b(G)$. They are closed in the space $\mathscr{C}_b(G)$ endowed with the topology of simple convergence. The set Pos(G) is a convex cone with vertex 0 in the real Banach space $\mathscr{C}_b(G)$.

### 6. Unitary Dual of a Locally Compact Group

Let G be a locally compact topological group. Endow G with a left Haar measure $\mu$. For $p\in [1,+\infty ]$, denote by $\mathscr{L}^p(G)$ (resp. $L^p(G)$) the space $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (resp. the space $L^p_{\mathbf{C}}(G, \mu)$). We identify the space $\mathscr{C}_b(G)$ with its image in $L^{\infty}(G)$.

Let Δ denote the module of G. Recall that $L^1(G)$ is an involutive Banach algebra whose involution is induced, by passing to quotients, by the mapping $f\mapsto f^*$ where $f^*(y) = \Delta^{-1}(y)f(y^{-1})$ for all $f\in \mathscr{L}^1(G)$ and $y\in G ($cf. I, p. 99, example 4). The Banach algebra $L^1(G)$ admits an approximate identity by INT, VIII, p. 172, §4, n$^o7$, prop. 20.

Let $\varrho$ be a unitary representation of G in a complex Hilbert space E. The mapping $f\mapsto \varrho (f)$ is a continuous morphism of involutive algebras from $L^1(G)$ into $\mathscr{L}(E)$ (lemma 1 of V, p. 401); it is a non-degenerate representation of $L^1(G)$ in E (INT, VIII, p. 139, § 2, n$^o7$, prop. 10, (i)).

#### Proposition 12 {#ts-v-s3-prop-12 .statement tag=03CN}

Let E be a complex Hilbert space and $\widetilde{\pi}$ an involutive algebra morphism from $L^1(G)$ into $\mathscr{L}(E)$. If the representation $\widetilde{\pi}$ is non-degenerate, then there exists a unique unitary representation $\pi$ of G in E such that $\widetilde{\pi}(f) =\pi (f)$ for every $f\in L^1(G)$.

The uniqueness follows from INT, VIII, p. 139, § 2, n$^o7$, cor. 3 of lemma 4.

Let us prove the existence of $\pi$. We have $\|\widetilde{\pi}\|\leqslant 1$ by Prop. 2 of I, p. 104. Let F be the subspace of E generated by the vectors of the form $\widetilde{\pi}(f)x$ for $f$ in $L^1(G)$ and $x$ in E; it is dense in E since the representation $\widetilde{\pi}$ is non-degenerate.

For every compact neighbourhood V of $e$, let $\varphi_V$ be a positive continuous function with support contained in V such that $\int\varphi_V\mu= 1$. Let $\mathfrak{B}$ be a base of the filter of compact neighbourhoods of $e$.

Let $g$ be in G and $f$ in $L^1(G)$. We have $(\varphi_V*\varepsilon_g)*f\rightarrow \varepsilon_g*f$ in $L^1(G)$ along the filter of sections of $\mathfrak{B}$ (INT, VIII, p. 172, § 4, n$^o7$, Prop. 20), hence $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ converges to $\widetilde{\pi}(\varepsilon_g*f)$ in $\mathscr{L}(E)$. This implies that $\widetilde{\pi}(\varphi_V*\varepsilon_g)$ converges simply along the filter of sections of $\mathfrak{B}$ to a linear mapping $\pi (g)$ of F into F; this mapping is continuous by EVT, III, p. 26, Cor. 3, since $\|\widetilde{\pi}(\varphi_V*\varepsilon_g)\|\leqslant 1$ for every compact neighbourhood V of $e$. There therefore exists a unique endomorphism of E which induces $\pi (g)$ by passing to subspaces. We again denote this endomorphism by $\pi (g)$; we have $\|\pi (g)\|\leqslant 1$.

Let $f\in L^1(G)$. Since $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ converges to $\widetilde{\pi}(\varepsilon_g*f)$, we have $\pi (g)\widetilde{\pi}(f) =\widetilde{\pi}(\varepsilon_g*f)$.

For $g=e$, this relation shows that $\pi (e)$ is the identity on F, hence $\pi (e) = 1_E$. Let $g_1$ and $g_2$ be in G. We have

$$
\pi (g_1)\pi (g_2)\widetilde{\pi}(f) =\pi (g_1)\widetilde{\pi}(\varepsilon_{g_2}*f) =\widetilde{\pi}(\varepsilon_{g_1g_2}*f) =\pi (g_1g_2)\widetilde{\pi}(f)
$$

whence $\pi (g_1)\pi (g_2) =\pi (g_1g_2)$ on F, and therefore on E. This proves that the mapping $g\mapsto \pi (g)$ is a representation of G in E. Since $\|\pi (g)\|\leqslant$ 1 and $\|\pi (g)^{-1}\|$ = $\|\pi (g^{-1})\|\leqslant$ 1, the endomorphisms $\pi (g)$ of E are isometric, hence unitary (EVT, V, p. 40, Prop. 3).

Let $f\in L^1(G)$ and $x\in E$. The mapping $g\mapsto \varepsilon_g*f$ of G into $L^1(G)$ is continuous (INT, VIII, p. 136, § 2, n$^o5$ and p. 144, § 3, n$^o2$, formula (5)), and $\widetilde{\pi}$ is continuous, hence the mapping $g\mapsto \widetilde{\pi}(\varepsilon_g*f)x=\pi (g)\widetilde{\pi}(f)x$ is continuous at $g=e$. Since F is dense in E, the representation $\pi$ is unitary (Lemma 4 of V, p. 380).

Let $f_1$ and $f_2$ be in $L^1(G)$. By INT, VIII, p. 127, §1, n$^o5$, Prop. 7, we have the relation

$$
f_1*f_2=\int_Gf_1(g)(\varepsilon_g*f_2)d\mu(g)
$$

in $L^1$(G), whence

$$
\widetilde{\pi}(f_1)\widetilde{\pi}(f_2) =\widetilde{\pi}(f_1*f_2) =\int_Gf_1(g)\widetilde{\pi}(\varepsilon_g*f_2)d\mu(g)
$$

$$
=\int_Gf_1(g)\pi (g)\widetilde{\pi}(f_2)d\mu(g) =(\int_Gf_1(g)\pi (g)d\mu(g))\widetilde{\pi}(f_2)
$$

using INT, VI, p. 9, § 1, n$^o1$, prop. 1. It follows that

$$
\widetilde{\pi}(f) =\int_Gf(g)\pi (g)d\mu(g) =\pi (f)
$$

for every $f\in L^1(G)$. The proposition is proved.

#### Proposition 13 {#ts-v-s3-prop-13 .statement tag=03CO}

Let $\varphi \in L^{\infty}(G)$. Denote by $\lambda_{\varphi}$ the continuous linear form $f\mapsto  \langle f, \varphi \rangle$ on $L^1(G)$. Then $\varphi$ is the class of a function of positive type on G if and only if $\lambda_{\varphi}$ is a positive continuous linear form on $L^1(G)$.

Suppose that $\lambda_{\varphi}$ is a positive continuous linear form on $L^1(G)$. Let $(E, x,\widetilde{\pi})$ be a cyclic Hilbert realization of $\lambda$ (prop. 5 of V, p. 438).

Let $\pi$ be a unitary representation of G in E such that $\pi (f) =\widetilde{\pi}(f)$ for every $f\in L^1(G)$ (prop. 12). Then $\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle$ for every $f\in L^1(G)$.

Since

$$
\pi (f) =\int_Gf(g)\pi (g)d\mu(g)
$$

for every $f\in L^1$(G), we get

$$
\int_Gf(g)\varphi (g)d\mu(g) =\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle =\int_Gf(g)\langle x|\pi (g)x\rangle d\mu(g)
$$

for every $f\in L^1(G)$ (INT, VI, p. 9, § 1, n$^o1$, prop. 1). Thus, $\varphi$ is the class in $L^{\infty}(G)$ of the function on G defined by $g\mapsto  \langle x|\pi (g)x\rangle$, which is a function of positive type on G (prop. 9 of V, p. 443).

Conversely, let $\varphi \in$ Pos(G). Let $f\in \mathscr{K}(G)$. Then we have

$$
\lambda_{\varphi}(f^**f) =\int_G\varphi (y)\int_G\Delta (z)^{-1}f(z^{-1})f(z^{-1}y)d\mu(z)d\mu(y)
$$

$$
=\int_G\varphi (y)\int_Gf(z)f(zy)d\mu(z)d\mu(y)
$$

(INT, VII, p. 19, § 1, n$^o3$, formula (22)). The continuous function on $G\times G$ defined by $(z, y)\mapsto \varphi (y)f(z)f(zy)$ is bounded and

$$
\int_G^*|\varphi(y)|\left(\int_G^*|\overline{f(z)}f(zy)|d\mu(z)\right)d\mu(y)
$$

$$
\leqslant\varphi(e)\int_G^*\int_G^*|f(z)||f(zy)|d\mu(z)d\mu(y)
$$

$$
=\varphi(e)\left(\int_G^*|f(z)|d\mu(z)\right)^2
$$

according to INT, V, p. 94, § 8, n$^o3$, prop. 8. We therefore deduce from the Lebesgue-Fubini theorem (INT, V, p. 96, § 8, n$^o4$, th. 1) that

$$
\lambda_{\varphi}(f^**f) =\int_Gf(z)\int_G\varphi (y)f(zy)d\mu(y)d\mu(z)
$$

$$
=\int_{G\times G}f(z)f(y)\varphi (z^{-1}y)d(\mu\otimes \mu)(z, y)
$$

This implies that $\lambda_{\varphi}(f^**f)\geqslant 0$ by Theorem 1, (i) of V, p. 432 applied to the measure induced by $\mu$ on the support of $f$ (INT, IV, p. 186, § 5, n$^o7$, def. 4). By continuity it follows that $\lambda_{\varphi}(f^**f)\geqslant 0$ for every $f\in L^1(G)$.

The spaces $L^{\infty}(G)$ and $\mathscr{C}_b(G)$ are endowed with their topologies as Banach spaces, whose norm is denoted by $f\mapsto  \|f\|_{\infty}$. Here we shall call weak topology on $L^{\infty}$(G), $\mathscr{C}_b(G)$ or Pos(G) the topology induced by the weak topology $\sigma (L^{\infty}(G),L^1(G))$.

Since $L^{\infty}(G)$ is identified with the dual of $L^1(G)$ (INT, V, p. 61, §5, n$^o8$, th. 4), every closed ball of $L^{\infty}(G)$ is compact for the weak topology (EVT, III, p. 17, cor. 3).

#### Corollary {#ts-v-s3-n6-cor-1 .statement tag=03CP}

In $L^{\infty}(G)$ endowed with the weak topology, the set Pos(G) is closed and the set Pos$_{\leqslant 1}(G)$ is compact.

The first assertion follows from the proposition, and the second then follows from EVT, III, loc. cit.

In general, Pos$_1(G)$ is not compact for the weak topology, as is shown by the example of the group $\mathbf{R}$ (exercise 10 of V, p. 497).

#### Proposition 14 {#ts-v-s3-prop-14 .statement tag=03CQ}

The set of extreme points of Pos$_{\leqslant 1}(G)$ is equal to the union of the set of extreme points of Pos$_1(G)$ and of the zero function. Moreover, the closed convex hull of the set of extreme points of Pos$_1(G)$ contains Pos$_1(G)$.

By cor. of prop. 13, the set Pos$_{\leqslant 1}(G)$ is a cap of the pointed convex cone Pos(G), which is defined by the gauge $\varphi \mapsto \varphi (e)$ (EVT, II, p. 61, def. 3 and prop. 4). Its extreme points are therefore the zero function and the elements $\varphi$ of Pos$_1(G)$ belonging to the extreme generators of Pos(G) (EVT, II, p. 62, cor. 1). These are the extreme points of Pos$_1(G)$ (EVT, II, p. 61, prop. 3). The first assertion follows.

Let us prove the second assertion. Let $\varphi \in$ Pos$_1(G)$. Since the set Pos$_{\leqslant 1}(G)$ is compact for the weak topology (cor. of prop. 13), there exists a filter $\mathfrak{F}$ on the convex hull of the extreme points of Pos$_{\leqslant 1}(G)$ which converges to $\varphi$ (EVT, II, p. 59, th. 1). Since the closed balls of the Banach space $L^{\infty}(G)$ are closed for the weak topology and since $\|\varphi \|_{\infty}= 1$, we have lim$_{\psi ,\mathfrak{F}}\|\psi \|_{\infty}= 1$ (indeed, otherwise there would exist a real number $c <1$ and a filter $\mathfrak{G}$ on the closed ball of radius $c$ in $L^{\infty}(G)$ which would be finer than $\mathfrak{F}$, which would imply that $\varphi$ belongs to this closed ball).

From the description of the extreme points of Pos$_{\leqslant 1}$(G), every element $\psi$ of the convex hull of the extreme points of Pos$_{\leqslant 1}(G)$ is a function of positive type on G of the form

$$
\psi =\sum_{i\in I}t_i\psi_i
$$

where I is a finite set, $\psi_i$ is an extreme point of Pos$_1(G)$ for every $i\in I$, and $t_i\in [0,1]$. We have $\sum_it_i=\psi (e) =\|\psi \|_{\infty}\leqslant 1$ (lemma 4 of V, p. 446). If $\psi \not = 0$, the function

$$
\frac{\psi}{\|\psi\|_{\infty}}=\sum_{i\in I}\frac{t_i}{\psi(e)}\psi_i
$$

therefore belongs to the convex hull of the extreme points of Pos$_1(G)$. Since lim$_{\psi ,\mathfrak{F}}\|\psi \|^{-1}_{\infty}\psi =\varphi$, we conclude that $\varphi$ belongs to the closed convex hull of the extreme points of Pos$_1(G)$. The assertion follows.

### 7. Existence of irreducible representations

We retain the notation of the preceding number.

#### Theorem 3 (Raikov) {#ts-v-s3-thm-3 .statement tag=03CR}

The weak topology on Pos$_1(G)$ coincides with the topology of compact convergence.

We shall first prove a few lemmas.

#### Lemma 5 {#ts-v-s3-lem-5 .statement tag=03CS}

Let X be a locally compact topological space and $\nu$ a positive measure on X. On every bounded subset of $\mathscr{C}_b(X)$, the topology induced by the weak topology $\sigma (L^{\infty}(X),L^1(X))$ is coarser than the topology of compact convergence.

Let B be a bounded subset of $\mathscr{C}_b(X)$ and let $M\in \mathbf{R}_+$ be such that $\|\varphi \|_{\infty}\leqslant M$ for every $\varphi \in B$. Let $\psi \in L^1(X, \nu )$ and $\varepsilon  >0$. Fix a compact subset K of X such that

$$
\int_{X-K}|\psi |d\nu  < \varepsilon
$$

For all $\varphi_1$ and $\varphi_2$ in B, we then have

$$
\langle \varphi_1-\varphi_2, \psi \rangle =\int_X\psi (\varphi_1-\varphi_2)d\nu
$$

$$
=\int_K\psi (\varphi_1-\varphi_2)d\nu +\int_{X-K}\psi (\varphi_1-\varphi_2)d\nu
$$

whence

$|\langle \varphi_1-\varphi_2, \psi \rangle |\leqslant$ sup$_{x\in K}|\varphi_1(x)-\varphi_2(x)| \|\psi \|_1+ 2M\varepsilon$,

and the lemma follows.

#### Lemma 6 {#ts-v-s3-lem-6 .statement tag=03CT}

Let $\psi \in L^1(G)$. Let B be a bounded subset of the Banach space $L^{\infty}(G)$. The mapping $\varphi \mapsto \psi *\varphi$ of B into $\mathscr{C}_b(G)$ is continuous when B is endowed with the weak topology and $\mathscr{C}_b(G)$ with the topology of compact convergence.

Let $\varphi \in L^{\infty}(G)$ and $\eta \in L^1(G)$. The function $\Delta^{-1}\check{\eta}$ belongs to $L^1(G)$ and $\langle \eta ,\check{\psi}\rangle =\langle \Delta^{-1}\check{\eta , \psi}\rangle ($cf. INT, VII, p. 19, § 1, n$^o3$, formula (22)). The mapping $\varphi \mapsto \check{\varphi}$ is therefore an automorphism of the space $L^{\infty}(G)$ endowed with the weak topology.

Let $\varphi \in L^{\infty}(G)$. By INT, VIII, p. 167, § 4, n$^o5$, prop. 14, the function $\psi *\varphi$ belongs to $\mathscr{C}_b(G)$ and satisfies

$$
(\psi *\varphi )(g) =\int_G\psi (h)\varphi (h^{-1}g)d\mu(h)
$$

$=\int_G\psi (gy)\check{\varphi}(y)d\mu(y) =\langle \check{\varphi ,}\boldsymbol{\gamma }$[^1]$_G(g^{-1})\psi \rangle$ for all $g\in G$. It follows that the linear mapping $u:\varphi \mapsto \psi *\varphi$ is a continuous mapping of the space $L^{\infty}(G)$ endowed with the weak topology into $\mathscr{C}_b(G)$ endowed with the topology of simple convergence.

Let $\varphi \in B$ and $(g, h)\in G\times G$. According to the above formula, we have

$|u(\varphi )(g)-u(\varphi )(h)|\leqslant \|\check{\varphi}\|_{\infty}\|(\boldsymbol{\gamma }$[^1]$_G(g^{-1})-\boldsymbol{\gamma }$[^1]$_G(h^{-1}))\psi \|_1$.

Since B is bounded and the left regular representation of G in $L^1(G)$ is continuous (No. 4 of V, p. 405), this implies that $u(B)$ is an equicontinuous subset of $\mathscr{C}_b(G)$. The assertion then results from the foregoing and from TG, X, p. 16, th. 1.

#### Lemma 7 {#ts-v-s3-lem-7 .statement tag=03CU}

Let $\psi \in L^1(G)$ be such that $\psi \geqslant 0$ and $\int\psi = 1$. Let us denote by $p$ the seminorm on $\mathscr{C}_b(G)$ defined by $p(\varphi ) =|\langle \varphi , \psi \rangle |$ for all $\varphi \in \mathscr{C}_b(G)$. For every $\varphi \in$ Pos$_1(G)$, one has

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \surd\overline{2p(1 -\varphi)}
$$

Let $\varphi \in$ Pos$_1(G)$ and $x\in G$. By INT, VIII, p. 167, § 4, n$^o5$, prop. 14, we obtain

$$
|\psi *\varphi (x)-\varphi (x)|=|\int_G(\varphi (y^{-1}x)-\varphi (x))\psi (y)d\mu(y)|
$$

$$
\leqslant \int_G|\varphi (y^{-1}x)-\varphi (x)|\psi (y)d\mu(y)
$$

$$
\leqslant \int_G\surd\overline{2(1 -\mathscr{R}\varphi(y))}\psi (y)d\mu(y)
$$

applying the majorization (1) of V, p. 446. The Cauchy-Schwarz inequality then implies

$\surd \int 1/2\int 1/2$

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \overline{2}(_G(1-\mathscr{R}(\varphi ))\psi  d\mu)(_G\psi  d\mu)
$$

$$
\surd \surd
$$

$\leqslant$ 2 $p(1-\varphi )$,

whence the result.

#### Lemma 8 {#ts-v-s3-lem-8 .statement tag=03CV}

Let K be a topological field and let E and F be topological vector spaces over K. Let $f$ be a mapping of E into F and X a subset of E. Let $x\in X$. The mapping $f|X$ is continuous at $x$ if, for every neighbourhood W of 0 in F, there exist a neighbourhood U of $x$ in E and a continuous mapping $g$ of X into F such that $(f-g)(U\cap X)\subset W$.

Let $W_0$ be a neighbourhood of 0 in F and let $V_0$ be a symmetric neighbourhood of 0 in F such that $V_0+V_0+V_0\subset W_0$. Let $U_0$ be a neighbourhood of $x$ in E and $g$ a continuous mapping of X into F such that $(f-g)(U_0\cap X)\subset V_0$. There exists a neighbourhood $U_1$ of $x$ in E such that $g(U_1\cap X)\subset g(x) + V_0$. For every $y\in U_0\cap U_1\cap X$, one has

$$
f(y)-f(x) = (f(y)-g(y)) + (g(y)-g(x))+
$$

$$
(g(x)-f(x))\in V_0+ V_0+ V_0\subset W_0
$$

hence $f(y)\in f(x) + W_0$, whence the result.

Let us now prove theorem 3. Let us denote by Pos$_1(G)_f$ (resp. Pos$_1(G)_c$) the set Pos$_1(G)$ endowed with the weak topology (resp. with the topology of compact convergence); analogously, let us denote by $\mathscr{C}_b(G)_f$ (resp. $\mathscr{C}_b(G)_c$) the space $\mathscr{C}_b(G)$ endowed with the weak topology (resp. with the topology of compact convergence).

The identity mapping of Pos$_1(G)_c$ into Pos$_1(G)_f$ is continuous (lemma 5). Conversely, let $\iota$ denote the inclusion of Pos$_1(G)_f$ into $\mathscr{C}_b(G)_c$. Let us prove that $\iota$ is continuous, to conclude the proof.

Let $\varphi_1\in$ Pos$_1(G)$. To verify that $\iota$ is continuous at $\varphi_1$, we apply lemma 8. Let W be a neighbourhood of 0 in $\mathscr{C}_b(G)_c$. It is enough to find a linear mapping $u$ of $\mathscr{C}_b(G)$ into $\mathscr{C}_b(G)$ which induces, by passing to subspaces, a continuous mapping of Pos$_1(G)_f$ into $\mathscr{C}_b(G)_c$, together with a neighbourhood U of 0 in Pos$_1(G)_f$, such that one has $(\iota -u)(U\cap$ Pos$_1(G))\subset W$.

There exists $\varepsilon  >0$ such that W contains the set of $\varphi \in \mathscr{C}_b(G)$ satisfying $\|\varphi \|_{\infty}\leqslant \varepsilon$. Since $\varphi_1(e) = 1$, there exists a compact neighbourhood V of $e$ in G such that

sup$_{x\in V}|1-\varphi_1(x)|\leqslant \frac{\varepsilon^2}{4}$.

Let $\varphi_V$ be the characteristic function of V, and put $\psi_V=\mu(V)^{-1}\varphi_V$. The linear mapping $u:\varphi \mapsto \psi_V*\varphi$ of Pos$_1(G)_f$ into $\mathscr{C}_b(G)_c$ is continuous (lemma 6).

Let $q_V$ denote the seminorm $\varphi \mapsto  |\langle \varphi , \psi_V\rangle |$ on $\mathscr{C}_b(G)$; it is continuous for the weak topology. Since $\psi_V$ vanishes outside V, we have $q_V(1-\varphi_1)\leqslant \varepsilon^2/4$; there therefore exists a neighbourhood U of $\varphi_1$ in $\mathscr{C}_b(G)_f$ such that $q_V(1-\varphi )\leqslant \varepsilon^2/2$ for every $\varphi \in U$.

Let $\varphi \in U\cap$ Pos$_1(G)$. By lemma 7, one has

$$
\|(\iota -u)(\varphi )\|_{\infty}\leqslant \surd\overline{2q_V(1 -\varphi)}\leqslant \varepsilon
$$

therefore $(\iota -u)(U)\subset W$. The theorem is proved.

In general, the weak topology on Pos$_{\leqslant 1}(G)$ does not coincide with the topology of compact convergence, as is shown by the example of the group $\mathbf{R}$.

We recall that $\widehat{G}$ denotes the set of classes of irreducible unitary representations of G (V, p. 393, def. 8).

#### Theorem 4 (Gelfand–Raikov) {#ts-v-s3-thm-4 .statement tag=03CW}

For every $x\not =e$ in G, there exists an irreducible unitary representation $\pi$ of G such that $\pi (x)$ is not the identity endomorphism of the space of $\pi$.

Let $x\in G$ be such that $\pi (x)$ is the identity for every $\pi \in \widehat{G}$. It follows that $\varphi (x) =\varphi (e) = 1$ for every extreme point $\varphi$ of Pos$_1(G)$ (prop. 11 of V, p. 444), hence for every $\varphi \in$ Pos$_1(G)$ by prop. 14 since the linear form $\varphi \mapsto \varphi (e)$ is continuous on Pos$_1(G)$ endowed with the weak topology (th. 3). But if $x\not =e$, there exists $f\in L^2(G)$ of norm 1 such that $\langle f|\boldsymbol{\gamma }_G(x)f\rangle = 0$(V, p. 406, lemma 3). Since the left-hand side of this equality is of the form $\varphi (x)$, where $\varphi \in$ Pos$_1$(G), this is a contradiction.

If G is not locally compact, it is not always true that the irreducible unitary representations of G separate the points of G.

#### Corollary {#ts-v-s3-n7-cor-1 .statement tag=03CX}

For every elements $g\not =h$ in G, there exists an irreducible representation $\pi \in \widehat{G}$ and a matrix coefficient $f$ of $\pi$ such that $f(g)\not =f(h)$. In particular, the subalgebra Υ(G) of $\mathscr{C}_b(G)$ separates the points of G.

Let $g\not =h$ in G. There exists an irreducible representation $\pi \in \widehat{G}$ such that $\pi (g)\not =\pi (h)$ (th. 4); hence there exist $x$ and $y$ in the space of $\pi$ such that $\langle x|\pi (g)y\rangle  \not =\langle x|\pi (h)y\rangle$.

### 8. Positive-definite functions on a locally compact commutative group

In this number, G is a locally compact commutative group and $\mu$ denotes a Haar measure on G. We denote by $\widehat{G}$ the dual group of G and by $\widehat{\mu}$ the measure dual to $\mu$ (def. 4 of II, p. 214). We denote by $\mathscr{F}$ the Fourier transform on the Banach space $\mathscr{M}^1(G)$ of bounded measures on G.

Since $\mathscr{C}_0(G)$ is the closure of $\mathscr{K}(G)$ in $\mathscr{C}_b$(G), the Banach space $\mathscr{M}^1(G)$ dual of $\mathscr{K}(G)$ endowed with the topology of $\mathscr{C}_b(G)$ is identified with the dual of $\mathscr{C}_0(G) ($cf. INT, III, p. 56, § 1, n$^o8)$. We endow $\mathscr{M}^1(G)$ with the weak topology associated with this duality.

#### Lemma 9 {#ts-v-s3-lem-9 .statement tag=03CY}

The Fourier transform is a continuous mapping of $\mathscr{M}^1(G)$ endowed with the weak topology into $\mathscr{C}_b(\widehat{G})$ endowed with the topology induced by the weak topology $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$.

Let $\mathfrak{F}$ be a filter on $\mathscr{M}^1(G)$ converging weakly to a bounded measure $\nu$ on G. For every $\varphi \in L^1(\widehat{G})$, one has $\mathscr{F}(\varphi )\in \mathscr{C}_0(G)$ (Prop. 4 of II, p. 209), hence

$$
\int_{\widehat{G}}\varphi \mathscr{F}(\nu )d\widehat{\mu}=\int_G\mathscr{F}(\varphi )d\nu
$$

= lim$_{\eta ,\mathfrak{F}}\int_G\mathscr{F}(\varphi )d\eta =$ lim$_{\eta ,\mathfrak{F}}\int_{\widehat{G}}\varphi \mathscr{F}(\eta )d\widehat{\mu}$,

by the transposition property of the Fourier transform (Prop. 13 of II, p. 221). The lemma follows.

#### Theorem 5 (Bochner) {#ts-v-s3-thm-5 .statement tag=03CZ}

A continuous function $\varphi$ on $\widehat{G}$ belongs to Pos($\widehat{G}$) if and only if there exists a bounded positive measure $\nu$ on G such that $\varphi =\mathscr{F}(\nu )$.

Let $\nu \in \mathscr{M}^1(G)$ be a positive measure. Its Fourier transform is continuous. For every finite family $(x_i)_{i\in I}$ in $\widehat{G}$ and every finite family $(t_i)_{i\in I}$ of complex numbers, one obtains

$$
\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\mathscr{F}(\nu )(x^{-1}_ix_j) =\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\int_Gx_i\overline{x}_jd\nu
$$

$$
=\int_G|\sum_{i\in I}\overline{t}_ix_i|^2d\nu \geqslant 0
$$

since $\nu$ is a positive measure. The Fourier transform of $\nu$ is therefore a function of positive type on $\widehat{G}$ (Th. 1 of V, p. 432, (ii)).

Let us prove the converse. Endow the set Pos$_{\leqslant 1}(\widehat{G})$ with the weak topology, induced as above by the weak topology $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$. The set Pos$_{\leqslant 1}(\widehat{G})$ is compact and convex (Cor. to Prop. 13 of V, p. 448). By Prop. 14 of V, p. 450, Prop. 11 of V, p. 444 and Cor. 7 of V, p. 390, the extreme points of Pos$_{\leqslant 1}(\widehat{G})$ are the zero function and the elements of $\widehat{G}$.

Let $\mathscr{N}$ be the set of bounded positive measures of mass $\leqslant 1$ on G; it is compact in $\mathscr{M}^1(G)$ endowed with the weak topology (EVT, III, p. 17, Cor. 3). By Lemma 9 and the first part of the proof, the Fourier transform on G defines, by passing to subspaces, a continuous mapping of $\mathscr{N}$ into Pos$_{\leqslant 1}(\widehat{G})$; by homogeneity, it is enough to prove that this mapping is surjective. The image $\mathscr{F}(\mathscr{N})$ of $\mathscr{N}$ under the Fourier transform is convex and compact; it contains the zero function and the elements of $\widehat{G}$ (in fact, these are of the form ev$_x:\chi \mapsto \chi (x)$ for an element $x$ of G by Th. 2 of II, p. 220, and one has ev$_x=\mathscr{F}(\varepsilon_{x^{-1}})$). The set $\mathscr{F}(\mathscr{N})$ therefore contains the extreme points of Pos$_{\leqslant 1}$(G), whence $\mathscr{F}(\mathscr{N}) =$ Pos$_{\leqslant 1}(G)$ by the Krein-Milman theorem (EVT, II, p. 59, Th. 1). This concludes the proof.

When $G =\mathbf{R}^k$ for an integer $k\in \mathbf{N}$, this theorem corresponds to Prop. 11 of INT, IX, p. 94, § 6, n$^o12$.

## EXERCISES {#ts-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
