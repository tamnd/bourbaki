---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 4
section_title: Perturbations dans les espaces de Banach
lang: en
source: ts-iii-v-fr
book_pages: TS III.55-TS III.70, TS III.123-TS III.124
pdf_pages: 0069-0084, 0137-0138
extraction: native
subsections:
    - "no": 1
      title: Morphismes directs
      page: 55
      pdf_page: 69
    - "no": 2
      title: Perturbation des applications de Fredholm
      page: 58
      pdf_page: 72
    - "no": 3
      title: Perturbation des endomorphismes de Riesz
      page: 59
      pdf_page: 73
    - "no": 4
      title: Conorme d’une application linéaire continue
      page: 61
      pdf_page: 75
    - "no": 5
      title: Sous-espaces vectoriels de dimension finie d’un espace normé
      page: 64
      pdf_page: 78
    - "no": 6
      title: Perturbations des applications linéaires continues injectives ou surjectives
      page: 67
      pdf_page: 81
statements: 30
exercises: 9
content_sha256: 910670a80334f4bc17a1ba846cbcae9dfc4d7bd9a3a996a8e9e2f73e3cf9c369
translated_from: content/fr/ts/III/04_s4_perturbations_dans_les_espaces_de_banach.md
source_lang: fr
translation_method: machine
source_content_sha256: 0639defbb25ee13675790dcd9d8ab04b2e73b080a6a0283ed9c065af1acacc79
translation_model: gpt-5.4
translation_run: translate-en-mt-e24029f1
glossary_version: 34
glossary_terms_sha256: 95b20cad76419b8a0e2842306ab481825c4cff149059a28d9e27f23c0fc83b0d
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. PERTURBATIONS IN BANACH SPACES

### 1. Direct morphisms

#### Definition 1 {#ts-iii-s4-def-1 .statement tag=02SH}

Let E be a topological vector space. A vector subspace of E is said to be direct if it admits a topological supplement.

In order that a vector subspace F of E be direct, it is necessary and sufficient that there exist in $\mathscr{L}(E)$ a projector with image F. If $p$ is such a projector, E is the topological direct sum of F and the kernel of $p$. The kernel of $1_E-p$ is F; if E is separated, F is therefore closed.

Let F be a direct vector subspace of E and let $E_1$ be a vector subspace of E containing F; then F is a direct vector subspace of $E_1$.

Every closed vector subspace of finite codimension in E is direct (TVS, I, p. 15, prop. 3), and every vector subspace F of E contained in the closure of $\{0\}$ is direct (for, there exists a projector with image F, and such a projector is necessarily continuous).

#### Proposition 1 {#ts-iii-s4-prop-1 .statement tag=02SI}

Let E be a locally convex space. Every finite-dimensional vector subspace of E is direct.

Let F be a finite-dimensional vector subspace of E. Let S denote a topological supplement of the closure of $\{0\}$ in F, which is a direct subspace of E. The space $F_2= F\cap S$ is separated and finite-dimensional; there therefore exists an integer $n\geqslant 0$ such that $F_2$ is isomorphic to $K^n$ (TVS, I, p. 14, th. 2). There then exists a continuous linear mapping $p: S\rightarrow F_2$ extending the identity mapping of $F_2$ (TVS, II, p. 26, remark). The kernel of $p$ is a topological supplement of $F_2$ in S, and also of F in E.

#### Definition 2 {#ts-iii-s4-def-2 .statement tag=02SJ}

Let E and F be locally convex spaces, and let $u$ be a continuous linear mapping of E into F. One says that $u$ is a direct morphism if $u$ is a strict morphism whose kernel is a direct vector subspace of E and whose image is a direct vector subspace of F.

Let $u\in \mathscr{L}(E; F)$. In order that the kernel and image of $u$ be direct vector subspaces of E and F respectively, it is necessary and sufficient that there exist decompositions $E = E_1\oplus E_2$ and $F = F_1\oplus F_2$ into topological direct sums such that $u$ be represented by a matrix $\begin{pmatrix} u_1 & 0 \\ 0 & 0 \end{pmatrix}$ where $u_1\in \mathscr{L}(E_1; F_1)$ is bijective. Since the kernel of $u$ is then $E_2$, since the canonical linear mapping of $E_1$ onto $E/E_2$ is an isomorphism, and since the image of $u$ is $F_1$, we see that $u$ is a strict morphism if and only if $u_1$ is an isomorphism of $E_1$ onto $F_1$. Let us denote by $v$ the element of $\mathscr{L}(F; E)$ represented by the matrix $\begin{pmatrix} u_1^{-1} & 0 \\ 0 & 0 \end{pmatrix}$ . Then the linear mapping $u\circ v$ is the projector in F with kernel $F_2$ and image $F_1$, the linear mapping $v\circ u$ is the projector in E with kernel $E_2$ and image $E_1$, and one has $u\circ v\circ u=u$.

Conversely, one has the following result:

#### Proposition 2 {#ts-iii-s4-prop-2 .statement tag=02SK}

Let E and F be locally convex spaces, let $u\in \mathscr{L}(E; F)$ and $v\in \mathscr{L}(F; E)$. Suppose that $u=u\circ v\circ u$. Then $u$ is a direct morphism. Moreover, $v\circ u$ is a continuous projector in E with kernel Ker($u$), and $u\circ v$ is a continuous projector in F with image Im($u$).

Put $p=v\circ u$ and $q=u\circ v$. One has

$$
p^2=v\circ (u\circ v\circ u) =v\circ u=p ,q^2= (u\circ v\circ u)\circ v=u\circ v=q
$$

therefore $p$ and $q$ are projectors. They are continuous. Let $E_1$ and $E_2$ be the image and the kernel of $p$, and let $F_1$ and $F_2$ be the image and the kernel of $q$. Since $u\circ v\circ u=u$, we have

Ker($u$)$\subset$ Ker($v\circ u$)$\subset$ Ker($u\circ v\circ u$) $=$ Ker($u$),

therefore Ker($u$) $=$ Ker($v\circ u$) $=$ Ker($p$) $= E_2$. Similarly, it follows from the inclusions

Im($u$)$\supset$ Im($u\circ v$)$\supset$ Im($u\circ v\circ u$) $=$ Im($u$)

that the image of $u$ is $F_1$. The spaces $E_2$ and $F_1$ are direct vector subspaces of E and F respectively.

The vector space E is the topological direct sum of $E_1$ and $E_2$, and $u$ defines by restriction a bijective linear mapping $u_1$ of $E_1$ onto $F_1$. For every $x\in E_1$, we have $v(u(x)) =p(x) =x$, and the mapping $u^{-1}_1$ of $F_1$ onto $E_1$ coincides with $v$ on $F_1$. Consequently, $u_1$ is an isomorphism of $E_1$ onto $F_1$ and $u$ is a strict morphism of E into F.

Let E and F be locally convex spaces and let $u\in \mathscr{L}(E; F)$. In order that $u$ be a direct injective morphism (resp. surjective), it is necessary and sufficient that there exist $v$ in $\mathscr{L}(F; E)$ such that $v\circ u= 1_E$ (resp. $u\circ v= 1_F$) (cf. TG, III, p. 47 and 48).

#### Proposition 3 {#ts-iii-s4-prop-3 .statement tag=02SL}

Let E and F be Banach spaces. The following sets are open subsets of the Banach space $\mathscr{L}(E; F):$

a) The set $\mathscr{I}(E; F)$ of the isomorphisms of E onto F ;

b) The set $\mathscr{M} \mathscr{D}(E; F)$ of injective direct morphisms of E into F, and more precisely, for every closed vector subspace $F_1$ of F, the set $\mathscr{M}_{F_1}(E; F)$ of elements of $\mathscr{M} \mathscr{D}(E; F)$ whose image is a topological complement of $F_1$;

c) The set $\mathscr{E} \mathscr{D}(E; F)$ of surjective direct morphisms of E onto F, and more precisely, for every closed vector subspace $E_1$ of E, the set $\mathscr{E}_{E_1}(E; F)$ of elements of $\mathscr{E} \mathscr{D}(E; F)$ whose kernel is a topological complement of $E_1$.

Moreover, the mapping $u\mapsto u^{-1}$ of $\mathscr{I}(E; F)$ onto $\mathscr{I}(F; E)$ is analytic.

By definition, $\mathscr{I}(E; E)$ is the set of invertible elements of the complete normed algebra $\mathscr{L}(E)$. By TG, IX, p. 40, Prop. 14, it is an open subset of $\mathscr{L}(E)$. The mapping $u\mapsto u^{-1}$ of $\mathscr{I}(E; E)$ into $\mathscr{I}(E; E)$ is analytic (LIE, III, § 1, n$^o1$, Example 2).

If the set $\mathscr{I}(E; F)$ is empty, it is open. Otherwise, let $u_0$ be an isomorphism of E onto F. The mapping $v\mapsto u_0\circ v$ is then an isomorphism of $\mathscr{L}(E)$ onto $\mathscr{L}(E; F)$ which transforms $\mathscr{I}(E; E)$ into $\mathscr{I}(E; F)$. Therefore the set $\mathscr{I}(E; F)$ is open in $\mathscr{L}(E; F)$. Moreover, if $u=u_0\circ v$ is an element of $\mathscr{I}(E; F)$, one has $u^{-1}=v^{-1}\circ u^{-1}_0$, and therefore the mapping $u\mapsto u^{-1}$ of $\mathscr{I}(E; F)$ onto $\mathscr{I}(F; E)$ is analytic.

Let $F_1$ be a closed vector subspace of F. For every $u\in \mathscr{L}(E; F)$, let $\overline{u}$ be the element of $\mathscr{L}(E\times F_1; F)$ defined by $\overline{u}(x, y) =u(x) +y$. The mapping $u\mapsto \overline{u}$ of $\mathscr{L}(E; F)$ into $\mathscr{L}(E\times F_1; F)$ is continuous, and $\mathscr{M}_{F_1}(E; F)$ is the set of elements $u$ of $\mathscr{L}(E; F)$ such that $\overline{u}$ belongs to $\mathscr{I}(E\times F_1; F)$. Since $\mathscr{I}(E\times F_1; F)$ is open in $\mathscr{L}(E\times F_1; F)$ by what precedes, the set $\mathscr{M}_{F_1}(E; F)$ is open in $\mathscr{L}(E; F)$. The same is true of $\mathscr{M} \mathscr{D}(E; F)$, which is the union of the $\mathscr{M}_{F_1}(E; F)$ when $F_1$ ranges over the set of closed vector subspaces of F.

Let $E_1$ be a closed vector subspace of E, and let $p$ be the canonical mapping of E onto the quotient Banach space $E/E_1$. In order that an element $u$ of $\mathscr{L}(E; F)$ belong to $\mathscr{E}_{E_1}(E; F)$, it is necessary and sufficient that the mapping $(u, p)$ of E into $F\times E/E_1$ belong to $\mathscr{I}(E; F\times E/E_1)$. As above, it follows that $\mathscr{E}_{E_1}(E; F)$ is open in $\mathscr{L}(E; F)$; the same is true of $\mathscr{E} \mathscr{D}(E; F)$, which is the union of the $\mathscr{E}_{E_1}(E; F)$.

### 2. Perturbation of Fredholm mappings

#### Theorem 1 {#ts-iii-s4-thm-1 .statement tag=02SM}

Let E and F be Banach spaces. The set $\mathscr{F}(E; F)$ of Fredholm mappings of E into F is open in the Banach space $\mathscr{L}(E; F)$, and the mapping $u\mapsto$ ind($u$) of $\mathscr{F}(E; F)$ into $\mathbf{Z}$ is locally constant.

The theorem follows from the following more precise statement:

#### Proposition 4 {#ts-iii-s4-prop-4 .statement tag=02SN}

Let E and F be Banach spaces, let $u_0: E\rightarrow F$ be a Fredholm mapping and $v_0$ a quasi-inverse of $u_0$. There exist an open neighbourhood U of $u_0$ in $\mathscr{L}(E; F)$ and an analytic mapping $\varphi : U\rightarrow \mathscr{L}(F; E)$ such that

(i) One has $\varphi (u_0) =v_0$;

(ii) For every $u$ in U, the mapping $\varphi (u)$ is a quasi-inverse of $u$, and in particular $u$ is a Fredholm mapping;

(iii) For every $u$ in U, one has ind($u$) $=$ ind($u_0$).

By prop. 2 of III, p. 42, (ii), there exist topological direct sum decompositions $E = E_1\oplus E_2$ and $F = F_1\oplus F_2$, and there exists $\alpha_0\in \mathscr{I}(E_1; F_1)$, such that $E_2$ and $F_2$ are finite-dimensional and that $u_0$ is represented by the matrix $\begin{pmatrix} \alpha_0 & 0 \\ 0 & 0 \end{pmatrix}$ relative to these decompositions.

Let U be the set of elements $u$ of $\mathscr{L}(E; F)$ such that, in the matrix representation $\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ of $u$ with respect to these decompositions, one has $\alpha \in \mathscr{I}(E_1; F_1)$. Since $\mathscr{I}(E_1; F_1)$ is open in $\mathscr{L}(E_1; F_1)$ (prop. 3 of III, p. 57), U is an open neighbourhood of $u_0$ in $\mathscr{L}(E; F)$. For $u=\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ in U, put

$$
\varphi (u) =v_0+\begin{pmatrix} \alpha^{-1}-\alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix} \tag{1}
$$

One has $\varphi (u_0) =v_0$ and the mapping $\varphi$ is analytic (loc. cit.). Modulo continuous linear mappings of finite rank, one has the congruences

$$
u\equiv \begin{pmatrix} \alpha & 0 \\ 0 & 0 \end{pmatrix},v_0\equiv \begin{pmatrix} \alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix},\varphi (u)\equiv \begin{pmatrix} \alpha^{-1} & 0 \\ 0 & 0 \end{pmatrix}
$$

Consequently, $\varphi (u)$ is a quasi-inverse of $u$. Every element $u$ of U defines by restriction an isomorphism of $E_1$ onto a topological supplement of $F_2$ in F. By prop. 3 of III, p. 44, one therefore has

ind($u$) $=$ codim$_F(u(E_1))-$ codim$_E(E_1)$

= dim(F$_2$)$-$ dim(E$_2$) $=$ ind($u_0$),

which concludes the proof.

### 3. Perturbation of Riesz endomorphisms

#### Lemma 1 {#ts-iii-s4-lem-1 .statement tag=02SO}

Let E be a Banach space. Let $p$ and $q$ be continuous projectors of E such that $\|q-p\|<1$. Then $p$ induces an isomorphism of Im($q$) onto Im($p$), and $1_E-p$ induces an isomorphism of Ker($q$) onto Ker($p$).

Consider the continuous linear mappings $u:x\mapsto p(x)$ of Im($q$) into Im($p$) and $v:y\mapsto q(y)$ of Im($p$) into Im($q$). For every $x\in$ Im($q$), we have $x=q(x)$, whence

$$
(q-p)^2(x) =q^2(x)-q(p(x))-p(q(x)) +p^2(x)
$$

$$
=x-q(p(x)) =x-v(u(x))
$$

Hence $\|1_E-v\circ u\|\leqslant \|q-p\|^2<1$. By Corollary 1 of I, p. 22$,v\circ u$ is an automorphism of Im($q$). One proves analogously that $u\circ v$ is an automorphism of Im($p$). This implies that $u$ is an isomorphism of Im($q$) onto Im($p$), whence the first assertion of the lemma. The second follows by replacing $p$ and $q$ by $1_E-p$ and $1_E-q$ respectively.

#### Theorem 2 {#ts-iii-s4-thm-2 .statement tag=02SP}

Let E be a Banach space. The set $\mathscr{R}(E)$ of Riesz endomorphisms of E is open in $\mathscr{L}(E)$. The mapping which associates with an element of $\mathscr{R}(E)$ the dimension of its nilspace is upper semi-continuous on $\mathscr{L}(E)$.

The theorem follows from the following more precise statement:

#### Proposition 5 {#ts-iii-s4-prop-5 .statement tag=02SQ}

Let E be a Banach space and $u_0$ a Riesz endomorphism of E. Let N (resp. I) be the nilspace (resp. the conilspace) of $u_0$. Let us denote by $d$ the dimension of N. There exist an open neighbourhood U of $u_0$ in $\mathscr{L}(E)$ and an analytic mapping $\pi : U\rightarrow \mathscr{L}(E)$ such that

(i) The endomorphism $\pi (u_0)$ is the projector with image N and kernel I;

(ii) For every $u\in U$, the linear mapping $\pi (u)$ is a projector of rank $d$ belonging to the bicommutant of $u$ and, in particular, commuting with $u$. Moreover, $u$ induces an automorphism of Ker($\pi (u)$);

(iii) Every element of U is a Riesz endomorphism whose nilspace has dimension $\leqslant d$.

If K = $\mathbf{C}$, let Sp($u_0$) denote the spectrum of $u_0$ relative to the algebra $\mathscr{L}(E)$. When K = $\mathbf{R}$, let Sp($u_0$) denote the complex spectrum Sp$_{\mathscr{L}(E_{(\mathbf{C})})}((u_0)_{(\mathbf{C})})$ of $u_0($I, p. 85, n$^o13$). By prop. 14 of III, p. 54, the point 0 is isolated in $\{0\} \cup$ Sp($u_0$). Let $r >0$ be a real number such that every element of Sp($u_0$)$-\{0\}$ has modulus $> r$. Let V denote the open set in $\mathbf{C}$ consisting of the complex numbers of absolute value $\not =r$; let $f$ be the holomorphic function on V defined by $f(z) = 0$ if $|z|> r$ and $f(z) = 1$ if $|z|< r$. If $K =\mathbf{C}$ (resp. $K =\mathbf{R}$), let $U'$ denote the set of elements $u$ of $\mathscr{L}(E)$ whose spectrum (resp. whose complex spectrum) is contained in V. The set $U'$ is an open neighbourhood of $u_0$ in $\mathscr{L}(E)$ and the mapping $u\mapsto f(u)$ of $U'$ into $\mathscr{L}(E)$ is holomorphic (I, p. 76, prop. 10 and I, p. 85, n$^o13$).

Let $u\in U'$. The endomorphism $f(u)$ is the spectral projector $e_0(u)$; it commutes with $u$, and $u$ induces by passing to the subspaces an automorphism of Ker($e_0(u)$) $($cf. III, p. 53, n$^o6$).

The projector $e_0(u_0)$ has image N and kernel I (III, p. 54, prop. 14); its rank is $d$. By lemma 1, the set U of elements $u\in U'$ such that $e_0(u)$ is of rank $d$ is an open neighbourhood of $u_0$. The set U and the mapping $\pi :u\mapsto e_0(u)$ of U into $\mathscr{L}(E)$ satisfy conditions (i) and (ii) of the proposition.

Let $u\in U$. Since $u$ induces an automorphism of Ker($e_0(u)$), which is a closed subspace of finite codimension of E, the endomorphism $u$ is a Riesz endomorphism of E (III, p. 48, prop. 8), the nilspace of $u$ is contained in the image of $\pi (u) =e_0(u)$, and is of dimension $\leqslant d$.

### 4. Conorm of a continuous linear mapping

Let E and F be normed spaces, $u: E\rightarrow F$ a continuous linear mapping, N the kernel of $u$ and I its image. Let us denote by $p$ the canonical surjection of E onto $E/N$ and by $i$ the canonical injection of I into F. Let $\widetilde{u}$ be the bijective linear mapping of $E/N$ onto I such that $u=i\circ \widetilde{u}\circ p$. The vector space $E/N$ is endowed with the quotient norm, that is to say that

(2) $\|y\|=$ inf$_{x\in\overset{-1}{p}(y)}\|x\|$

for every $y\in E/N$. The mapping $\widetilde{u}$ is continuous and $\|u\|=\|\widetilde{u}\|$, whence (3) $\|u\|=$ sup$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

the least upper bound being taken in $\overline{\mathbf{R}}_+$. The number

(4) $((u)) =$ inf$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

the greatest lower bound being taken in $\overline{\mathbf{R}}_+$. Hence

$$
((u))\|y\|\leqslant \|\widetilde{u}(y)\|\leqslant \|u\| \|y\| \tag{5}
$$

for every element $y$ of $E/N$. Put $v=i\circ \widetilde{u}$. Then $u=v\circ p$ and

(6) $((u)) =$ inf$_{y\in E/N}\frac{\|v(y)\|}{\|y\|}=$ inf$_{y\in E/N}\|v(y)\|$.

$y\not =0\|y\|=1$

When $u$ is the zero mapping, the space $E/N$ reduces to 0 and one has $((u)) = +\infty$ and $\|u\|= 0$. When $u\not = 0$, one deduces from (3) and (4) the inequalities

$$
0\leqslant ((u))\leqslant \|u\|<+\infty \tag{7}
$$

When $u$ is injective, one has

(8) $((u)) =$ inf$_{xx\in\not=0E}\frac{\|u(x)\|}{\|x\|}$,

and, for every $x\in E$, one has

$$
((u))\|x\|\leqslant \|u(x)\|\leqslant \|u\| \|x\| \tag{9}
$$

Let us denote by $j$ the canonical injection of the normed space F into its completion $\widehat{F}$. One has $((u)) = ((j\circ u))$.

#### Remark {#ts-iii-s4-n4-rem-1 .statement tag=02SR}

By definition, in order that one have $((u))>0$, it is necessary and sufficient that the bijective linear mapping $\widetilde{u}$ be bicontinuous, that is to say, that $u$ be a strict morphism (TG, III, p. 16). One then has

$$
((u)) =\|\widetilde{u}^{-1}\|^{-1} \tag{10}
$$

#### Lemma 2 {#ts-iii-s4-lem-2 .statement tag=02SS}

Let $c$ be a real number. If $c <((u))$, then for every element $z\in$ Im($u$), there exists an element $x$ of E such that $u(x) =z$ and $c\|x\|\leqslant \|z\|$. Conversely, if for every $z\in$ Im($u$) there exists $x\in E$ such that $u(x) =z$ and $c\|x\|\leqslant \|z\|$, then $c\leqslant ((u))$.

This is a consequence of formulas (2) and (5) and of the definition of the conorm of $u$.

#### Proposition 6 {#ts-iii-s4-prop-6 .statement tag=02ST}

Let E and F be normed spaces and $u\in \mathscr{L}(E; F)$. Let B denote the set of elements of E of norm $<1$. Put

$P =u(E)-u(B),Q =u(E)$ - $(\overline{u(B)}\cap u(E))$.

The conorm of $u$ is equal to the distance from 0 to P in F. If the normed space E is complete or if $u$ is a strict morphism, the conorm of $u$ is equal to the distance from 0 to Q in F.

Let N be the kernel of $u$; let $p: E\rightarrow E/N$ be the canonical surjection and let $v: E/N\rightarrow F$ be the mapping deduced from $u$ by passing to the quotient. The set $p(B)$ is the set of elements of $E/N$ of norm $<1$. We have

$$
P =u(E)-u(B) =v(E/N)-v(p(B)) =v((E/N)-p(B))
$$

since the mapping $v$ is injective. In other words, P is made up of the elements of F of the form $v(y)$ with $y\in E/N$ and $\|y\|\geqslant 1$. Let $d_P$ denote the distance from 0 to P in F. We have

$d_P=$ inf$_{y\|\in yE\|\geqslant/N1}\|v(y)\|=$ inf$_{y\|\in yE\|=1/N}\|v(y)\|= ((u))$ by (6).

Suppose that $u$ is a strict morphism. Let $\varepsilon  >0$. The set $\varepsilon u(B)$ is a neighbourhood of 0 in $u(E)$. The closure of $u(B)$ in $u(E)$ is equal to $\overline{u(B)}\cap u(E)$. It is contained in the set $u(B) +\varepsilon u(B)$, which is equal to $(1 +\varepsilon )u(B)$ since $u(B)$ is convex. Hence we have $(1 +\varepsilon )P\subset Q\subset P$, and the distance $d_Q$ from 0 to Q in F satisfies the inequalities $d_P\leqslant d_Q\leqslant (1 +\varepsilon )d_P$. Since this holds for every $\varepsilon  >0$, we have $d_Q=d_P= ((u))$.

Suppose that $u$ is not a strict morphism, but that the normed space E is complete. Then $((u)) = 0$ (remark above). The closure of $u(B)$ in $u$(E), which is equal to $\overline{u(B)}\cap u$(E), is not a neighbourhood of 0 in $u(E)$ (EVT, I, p. 17, th. 1). There then exist points of Q arbitrarily near 0, whence $d_Q= 0 = ((u))$.

#### Proposition 7 {#ts-iii-s4-prop-7 .statement tag=02SU}

Let E be a Banach space and F a normed space. The mapping $u\mapsto ((u))$ from $\mathscr{L}(E; F)$ into $\overline{\mathbf{R}}$ is upper semi-continuous.

Let $u\in \mathscr{L}(E; F)$. We have to prove that for every real number $c >((u))$, the set of elements $v\in \mathscr{L}(E; F)$ such that $((v))< c$ is a neighbourhood of $u$. Let B denote the set of elements of E of norm $<1$. By Prop. 6, there exists $y\in E$ such that $u(y)\notin u(B)$ and $\|u(y)\|< c$. The distance $d$ from $u(y)$ to the closed set $u(B)$ is strictly positive. The set V of elements $v$ of $\mathscr{L}(E; F)$ satisfying the relations $\|v(y)\|< c$ and $\|u-v\|(1 +\|y\|)< d$ is a neighbourhood of $u$ in $\mathscr{L}(E; F)$. Let $v\in V$. For every $x\in B$, one has

$$
d\leqslant \|u(y)-u(x)\|\leqslant \|v(y)-v(x)\|+\|u-v\|(\|y\|+\|x\|)
$$

$$
<\|v(y)-v(x)\|+d
$$

Consequently $v(y)$ does not belong to $v$(B), and one has $((v))\leqslant \|v(y)\|< c$ by Prop. 6.

#### Proposition 8 {#ts-iii-s4-prop-8 .statement tag=02SV}

Let E be a Banach space, F a normed space. For every $u\in \mathscr{L}(E; F)$, one has $((u)) = ((^tu))$.

Let $j$ denote the canonical injection of the normed space F into its completion $\widehat{F}$. One has $((u)) = ((j\circ u))$. Since the linear mapping $^tj: (\widehat{F})'\rightarrow F'$ is bijective and isometric, one has likewise $((^tu)) = ((^t(j\circ u)))$. It is therefore enough to prove the proposition when the normed space F is complete, which we shall assume in the rest of the proof.

If $u$ is zero, one has $((u)) = ((^tu)) = +\infty$. If $u$ is not a strict morphism, then $^tu$ is not one either (EVT, IV, p. 29, Cor. 3), and one has $((u)) = ((^tu)) = 0$.

Assume henceforth that $u$ is a strict nonzero morphism. Let N denote the kernel of $u$ and I its image, and consider the canonical decomposition of $u:$

$$
E\overset{p}{\longrightarrow}E/N\longrightarrow^vI\longrightarrow^iF
$$

The kernel of $^tu$ is the orthogonal $I^{\circ}$ of I in $F'$ (EVT, IV, p. 27, Prop. 2), and $^ti$ defines by passing to the quotient an isometry $\iota$ of $F'/I^{\circ}$ onto $I'$ (EVT, IV, p. 9, Prop. 10). Moreover, $^tp$ defines an isometry $\pi$ of $(E/N)'$ onto the orthogonal $N^{\circ}$ of N in $E'$ (EVT, IV, p. 8, Prop. 9). The canonical decomposition of $^tu$ is therefore

$$
F'\longrightarrow F'/I^{\circ}\longrightarrow^{v'}N^{\circ}\longrightarrow E'
$$

where $v'=\pi \circ^tv\circ \iota$. One then has

$$
\|(v')^{-1}\|=\|(^tv)^{-1}\|=\|^t(v^{-1})\|=\|v^{-1}\|
$$

(EVT, IV, p. 7, prop. 8), whence $((u)) = ((^tu))$ after formula (10).

### 5. Finite-dimensional vector subspaces of a normed space

The following statement will be proved in TA, to appear, as a corollary of the Borsuk–Ulam theorem.

#### Theorem 3 {#ts-iii-s4-thm-3 .statement tag=02SW}

Let $n$ be a positive integer, V a real normed vector space of dimension $n+ 1$ and W a vector subspace of V of dimension $n$. Let S be the unit sphere of V. There does not exist a continuous mapping $f: S\rightarrow W$ such that $\|f(x)-x)\|<1$ for all $x\in S$.

#### Theorem 4 (Krein, Krasnoselskii, Milman) {#ts-iii-s4-thm-4 .statement tag=02SX}

Let E be a normed space, and let F and G be vector subspaces of E. Suppose that the dimension of G is finite and strictly less than that of F. There exists an element of F of norm 1 whose distance to G is equal to 1.

It is enough to treat the case where the field K is equal to $\mathbf{R}$. Let $n$ be the dimension of G. Replacing F by a vector subspace of F of dimension $n+ 1$ containing G, we are reduced to the case where dim(F) $=n+ 1$. Let us reason by contradiction, supposing that the conclusion of the theorem is not satisfied. Let S be the unit sphere of F. For every $x\in S$, the distance from $x$ to G is then strictly less than $\|x\|= 1$, and one can choose an element $y(x)$ of G such that $\|x-y(x)\|<1$. Let $V_x$ denote the set of elements $z$ of S such that $\|z-y(x)\|<1$; this is an open neighbourhood of $x$ in S. There exists a continuous locally finite partition of unity $(\varphi_x)_{x\in S}$ on S subordinate to the covering $(V_x)_{x\in S}$ of S (TG, IX, p. 46, prop. 3 and p. 51, prop. 6). Let $f: S\rightarrow G$ be the continuous mapping given by

$$
f(z) =\sum_{x\in S}\varphi_x(z)y(x)
$$

for every $z\in S$. Let $z\in S$. One has $\varphi_x(z)\geqslant 0$ for every $x\in S$, and there exists $x\in S$ such that $\varphi_x(z)>0$, since $\sum_{x\in S}\varphi_x(z) = 1$, hence

$$
\|z-f(z)\|=\|\sum_{x\in S}\varphi_x(z)(z-y(x))\|\leqslant \sum_{x\in S}\varphi_x(z)\|z-y(x)\|
$$

$$
<\sum_{x\in S}\varphi_x(z) = 1
$$

This property of $f$ contradicts Theorem 3.

#### Proposition 9 {#ts-iii-s4-prop-9 .statement tag=02SY}

Let E and F be normed spaces, $n\in \mathbf{N}$ and $u$ a continuous linear mapping from E into F whose kernel is of dimension $n$. The conorm of $u$ is equal to the distance $d$ from $u$ to the set of mappings $v\in \mathscr{L}(E; F)$ whose kernel is of dimension at least $n+ 1$.

When $u= 0$, one has $((u)) = +\infty$ and dim(E) $=n$, whence $d= +\infty$. Suppose henceforth that $u$ is non-zero, and therefore that $((u))<+\infty$. Let $v$ be an element of $\mathscr{L}(E; F)$ such that $\|u-v\|<((u))$ and let us prove that its kernel is of dimension $\leqslant n$. Let $x$ be an element of norm 1 of Ker($v$) and $y$ its image in $E/$ Ker($u$). One has (formula (5) of III, p. 61)

$$
((u))\|y\|\leqslant \|u(x)\|=\|(u-v)(x)\|\leqslant \|u-v\|<((u))
$$

whence $\|y\|<1$. Now $\|y\|$ is the distance from $x$ to Ker($u$). Theorem 4 then implies that one has dim Ker($v$)$\leqslant$ dim Ker($u$) $=n$. This proves the inequality $((u))\leqslant d$. The converse inequality $d\leqslant ((u))$ results from the more precise lemma that follows.

#### Lemma 3 {#ts-iii-s4-lem-3 .statement tag=02SZ}

Let $c$ be a real number such that $c >((u))$. There exists a continuous linear mapping $h: E\rightarrow F$, of rank 1 and norm $< c$ such that the kernel of $u+h$ contains that of $u$ and is of dimension $n+ 1$.

Let $p$ denote the canonical mapping of E onto $E/$ Ker($u$). There exists $a\in E$ such that $\|p(a)\|= 1$ and $\|u(a)\|< c$ (formula (6) of III, p. 61). By the Hahn–Banach theorem (EVT, II, p. 24, cor. 2), there exists a continuous linear form $f$ on the normed space $E/$ Ker($u$) such that $f(p(a)) = 1$ and $\|f\|= 1$. The linear mapping $h:x\mapsto  -(f\circ p)(x)u(a)$ of E into F is continuous, of rank 1, and one has $\|h\|\leqslant \|f\| \|p\| \|u(a)\|< c$. The kernel of the mapping $u+h$ contains that of $u$ and $a$; since $a\not \in$ Ker($u$), its dimension is therefore at least $n+ 1$. On the other hand, the linear mapping $u$ induces, by passing to subspaces, a linear mapping of Ker($u+h$) into Im($h$) with kernel Ker($u$)$\cap$ Ker($u+h$), so that dim(Ker($u+h$))$\leqslant$ dim(Ker($u$)) $+ 1$. The conclusion follows.

#### Corollary 1 {#ts-iii-s4-lem-3-cor-1 .statement tag=02T0}

Let E and F be normed spaces, and let $u,v$ be non-zero continuous linear mappings of E into F whose kernels have the same finite dimension. One then has

$$
|((u))-((v))|\leqslant \|u-v\|
$$

Let $n$ be the common dimension of the kernels of $u$ and $v$. Let A be the set of continuous linear mappings of E into F whose kernel is of dimension $\geqslant n+ 1$. Since $u\not = 0$, one has dim(E) $> n$ and the set A contains 0. By proposition 9, $((u))$ and $((v))$ are respectively the distances from $u$ and from $v$ to the set A in $\mathscr{L}(E; F)$. It then suffices to apply the formula $|d(u,A)-d(v,A)|\leqslant \|u-v\|($cf. TG, IX, p. 13).

#### Corollary 2 {#ts-iii-s4-lem-3-cor-2 .statement tag=02T1}

Let E and F be Banach spaces, and let $u$ and $v$ be non-zero continuous linear mappings of E into F whose images have the same finite codimension in F. Then

$$
|((u))-((v))|\leqslant \|u-v\|
$$

The morphism $u$ is strict (III, p. 52, lemma 6). The kernel of the continuous linear mapping $^tu$ is the orthogonal (Im($u$))$^{\circ}$ of Im($u$) (EVT, IV, p. 27, prop. 2), hence dim(Ker($^tu$)) $=$ codim$_F$(Im($u$)), and analogously dim(Ker($^tv$)) $=$ codim$_F$(Im($v$)). The kernels of $^tu$ and $^tv$ therefore have the same finite dimension. Since

$$
\|^tu-^tv\|=\|u-v\|,((^tu)) = ((u)),((^tv)) = ((v))
$$

(EVT, IV, p. 7, prop. 8 and prop. 8 of III, p. 63), the assertion follows from corollary 1, applied to $^tu$ and $^tv$.

### 6. Perturbations of injective or surjective continuous linear mappings

In this number, the following conventions are adopted: if E is a finite-dimensional vector space, dim(E) denotes its dimension; if E is an infinite-dimensional vector space, one sets dim(E) $= +\infty  \in \overline{\mathbf{R}}$. If $u$ is a linear mapping whose kernel or cokernel is of finite dimension, one sets ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$), the calculus being carried out in $\overline{\mathbf{R}}$.

Let E and F be normed spaces. We denote by $\mathscr{M}(E; F)$ the set of injective strict morphisms of E into F, and by $\mathscr{Q}\mathscr{M}(E; F)$ the set of strict morphisms of E into F whose kernel is of finite dimension.

#### Proposition 10 {#ts-iii-s4-prop-10 .statement tag=02T2}

Let E and F be normed spaces. The set $\mathscr{M}(E; F)$ is open in $\mathscr{L}(E; F)$. It is the interior of the set of mappings in $\mathscr{L}(E; F)$ which are injective.

Let A be the set of injective continuous linear mappings of E into F. For a mapping $u\in A$ to be a strict morphism, it is necessary and sufficient that its conorm $((u))$ be strictly positive (III, p. 62, remark). Now $((u))$ is the distance from $u$ to the complement of A in $\mathscr{L}(E; F)$(III, p. 65, prop. 9). The proposition follows.

#### Proposition 11 {#ts-iii-s4-prop-11 .statement tag=02T3}

Let E and F be Banach spaces. The set $\mathscr{Q}\mathscr{M}(E; F)$ is open in $\mathscr{L}(E; F)$. It is the interior of the set of mappings in $\mathscr{L}(E; F)$ whose kernel is of finite dimension.

Let A be the set of continuous linear mappings of E into F whose kernel is of finite dimension.

Let $u$ be an element of $\mathscr{Q}\mathscr{M}(E; F)$. Then $((u))>0$(III, p. 62, remark). Every element $v\in \mathscr{L}(E; F)$ whose distance from $u$ is $<((u))$ then belongs to A (III, p. 65, prop. 9), so that $u$ is an interior point of A.

Conversely, let $u$ be an element of A which is not a strict morphism. One has $((u)) = 0 ($III, p. 62, Remark). Let $v$ be an element of $\mathscr{L}(E; F)$ differing from $u$ by a linear mapping of finite rank; by Corollary 1 of III, p. 40, the morphism $v$ cannot be strict with closed image; since a strict morphism of E into F has a closed image in F (EVT, IV, p. 28, Theorem 1), this means that $v$ is not a strict morphism. Hence $((v)) = 0$. Let $\varepsilon$ be a real number $>0$. By the foregoing, Lemma 3 of III, p. 66 enables one to construct by induction a sequence $(u_m)_{m\in\mathbf{N}}$ of elements of $\mathscr{L}(E; F)$ satisfying the following conditions:

(i) One has $u_0=u$;

(ii) For every $m\geqslant 0,u_{m+1}-u_m$ is a continuous linear mapping of rank 1 and norm $\leqslant 2^{-m-1}\varepsilon$;

(iii) For every $m\geqslant 0$, the kernel of $u_m$ has dimension $n+m$ and is contained in that of $u_{m+1}$.

The sequence $(u_m)$ is a Cauchy sequence in the Banach space $\mathscr{L}(E; F)$. Let $u'$ be its limit. The kernel of $u'$ contains that of $u_m$ for every $m\geqslant 0$; it is infinite-dimensional. Since

$$
\|u'-u\|\leqslant \sum_{m=0}^{\infty}\|u_{m+1}-u_m\|\leqslant \varepsilon \sum_{m=0}^{\infty}2^{-m-1}=\varepsilon
$$

the distance from $u$ to the complement of A is less than $\varepsilon$. Since this holds for every $\varepsilon  >0$, one concludes that $u$ is not an interior point of A.

#### Proposition 12 {#ts-iii-s4-prop-12 .statement tag=02T4}

Let E and F be Banach spaces and $u$ an element of $\mathscr{Q}\mathscr{M}(E; F)$. Every $v\in \mathscr{L}(E; F)$ such that $\|v-u\|<((u))$ belong to $\mathscr{Q}\mathscr{M}(E; F)$ and satisfy the relations

dim Ker($v$)$\leqslant$ dim Ker($u$),

dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

Since $u$ is strict, one has $((u))>0$. Let B denote the open ball with center $v$ and radius $((u))$ in $\mathscr{L}(E; F)$. For every $v\in$ B, one has dim Ker($v$)$\leqslant$ dim Ker($u$)(III, p. 65, prop. 9) and $v\in \mathscr{Q}\mathscr{M}(E; F)$ (prop. 11).

For $r\in \mathbf{Z}\cup  \{+\infty \}$, let us denote by $B_r$ the set of elements $v\in B$ such that ind($v$) $=r$. If $r\in \mathbf{Z}$, the set $B_r$ is the set of Fredholm mappings from E into F of index $r$ which belong to B (III, p. 52, Prop. 11); it is open in B by Theorem 1 of III, p. 58.

Let us prove that the sets $B_r$ are closed in B. Let $v\in B$ be an adherent point of $B_r$. Since the sets $B_s$, for $s\in \mathbf{Z}$, are open in B and pairwise disjoint, we have $v\in B_r$ or $v\in B_{+\infty}$.

Suppose $v\in B_{+\infty}$. Let $n$ be the dimension of Ker($u$). Choose a vector subspace T of F of dimension $r+ 2n+ 1$ whose intersection with Im($v$) is reduced to 0, and a topological complement S of Ker($v$) in E (III, p. 55, Prop. 1). Consider the continuous linear mapping $f: (s, t)\mapsto v(s) +t$ of $S\times T$ into F. It is injective. The linear mapping $v$ is a strict morphism since $v$ belongs to $B\subset \mathscr{Q}\mathscr{M}(E; F)$. The image of $v$ is therefore closed (EVT, IV, p. 28, Theorem 1). By Prop. 1 of III, p. 39, the restriction of $v$ to S is a strict morphism with closed image from S into F, and $f$ is a strict morphism with closed image from $S\times T$ into F.

By Prop. 10, there exists a neighbourhood U of $v$ in B such that, for every $w\in U$, the linear mapping $(s, t)\mapsto w(s) +t$ of $S\times T$ into F is injective. Let $w$ be an element of U. Then Ker($w$)$\cap S =\{0\}$, so that $w$ defines by restriction and passing to the quotient an injective linear mapping of Ker($w$) into $E/S$, which implies that Ker($w$) is of dimension at most $n$. We also have $w(S)\cap T =\{0\}$, hence

codim$_F$(Im($w$))$\geqslant$ dim(T) $-$ codim$_E(S) =r+n+ 1$,

this yields ind($w$)$\geqslant r+ 1$ and contradicts the hypothesis that $v$ is adherent to $B_r$.

If $r$ is an element of $\mathbf{Z}$ such that $B_r$ is nonempty, one has $B_r= B$ since $B_r$ is open and closed in B and B is connected. If $B_r$ is empty for every $r\in \mathbf{Z}$, one has ind($v$) $= +\infty$ for every $v\in B$. The mapping $v\mapsto$ ind($v$) is therefore constant on B. Lastly, for every $v\in B$, one has

dim Coker($v$) $=$ ind($v$) $+$ dim Ker($v$)

$\leqslant$ ind($u$) $+$ dim Ker($u$) $=$ dim Coker($u$).

This concludes the proof.

#### Corollary 1 {#ts-iii-s4-prop-12-cor-1 .statement tag=02T5}

The functions defined by $u\mapsto$ dim Ker($u$) and by $u\mapsto$ dim Coker($u$) on $\mathscr{Q}\mathscr{M}(E; F)$ are upper semi-continuous. The function $u\mapsto$ ind($u$) is locally constant on $\mathscr{Q}\mathscr{M}(E; F)$.

#### Corollary 2 {#ts-iii-s4-prop-12-cor-2 .statement tag=02T6}

The function $u\mapsto$ dim Coker($u$) is locally constant on the set $\mathscr{M}(E; F)$ of strict injective morphisms of E into F.

Indeed, one has dim Coker($u$) $=$ ind($u$) for $u\in \mathscr{M}(E; F)$.

#### Lemma 4 {#ts-iii-s4-lem-4 .statement tag=02T7}

Let E and F be Banach spaces. In order that an element $u$ of $\mathscr{L}(E; F)$ be a strict morphism of E into F, it is necessary and sufficient that $^tu$ be a strict morphism of $F'$ into $E'$. In this case, one has dim Coker($^tu$) $=$ dim Ker($u$) and dim Ker($^tu$) $=$ dim Coker($u$).

For $u$ to be a strict morphism, it is necessary and sufficient that $^tu$ be one (EVT, IV, p. 29, cor. 3); in this case, the image of $u$ is closed (EVT, IV, p. 28, th. 1) and the vector space Ker($^tu$) (resp. Coker($^tu$)) is canonically isomorphic to the dual of the normed space Coker($u$) (resp. Ker($u$)) by EVT, IV, p. 27, prop. 2. The lemma follows.

Let E and F be Banach spaces. Denote by $\mathscr{E}(E; F)$ the set of continuous linear surjective mappings from E into F and by $\mathscr{Q}\mathscr{E}(E; F)$ the set of continuous linear mappings from E into F whose image is of finite codimension. Every element of $\mathscr{Q}\mathscr{E}(E; F)$ is a strict morphism with closed image (III, p. 52, lemma 6). It follows from lemma 4 that $\mathscr{E}(E; F)$ and $\mathscr{Q}\mathscr{E}(E; F)$ are the inverse images respectively of $\mathscr{M}(F'; E')$ and $\mathscr{Q}\mathscr{M}(F'; E')$ under the continuous mapping $u\mapsto^tu$ from $\mathscr{L}(E; F)$ into $\mathscr{L}(F'; E')$.

#### Proposition 13 {#ts-iii-s4-prop-13 .statement tag=02T8}

Let E and F be Banach spaces. The sets $\mathscr{E}(E; F)$ and $\mathscr{Q}\mathscr{E}(E; F)$ are open in $\mathscr{L}(E; F)$. More precisely, if $u$ is an element of $\mathscr{Q}\mathscr{E}(E; F)$ and $v$ an element of $\mathscr{L}(E; F)$ such that $\|v-u\|<((u))$, then $v\in \mathscr{Q}\mathscr{E}(E; F)$ and

dim Ker($v$)$\leqslant$ dim Ker($u$), dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

We have seen above that $^tu\in \mathscr{Q}\mathscr{M}(F'; E')$. Moreover, for every element $v$ of $\mathscr{L}(E; F)$, one has $\|^tv-^tu\|=\|v-u\|$ and $((^tu)) = ((u))$ (EVT, IV, p. 7, prop. 8 and III, p. 63, prop. 8). According to prop. 12, it follows from these relations that if $\|v-u\|<((u))$, then $^tv$ belongs to $\mathscr{Q}\mathscr{M}(F'; E')$ and that one has the inequalities

dim Ker($^tv$)$\leqslant$ dim Ker($^tu$), dim Coker($^tv$)$\leqslant$ dim Coker($^tu$)

as well as the equality ind($^tv$) $=$ ind($^tu$). The proposition then follows from lemma 4.

#### Corollary 1 {#ts-iii-s4-prop-13-cor-1 .statement tag=02T9}

The functions defined by $u\mapsto$ dim Ker($u$) and by $u\mapsto$ dim Coker($u$) on $\mathscr{Q}\mathscr{E}(E; F)$ are upper semi-continuous. The function $u\mapsto$ ind($u$) is locally constant on $\mathscr{Q}\mathscr{E}(E; F)$.

#### Corollary 2 {#ts-iii-s4-prop-13-cor-2 .statement tag=02TA}

The function defined by $u\mapsto$ dim Ker($u$) is locally constant on $\mathscr{E}(E; F)$.

Indeed, one has dim Ker($u$) $=-$ ind($u$) for every $u\in \mathscr{E}(E; F)$.

## EXERCISES {#ts-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
