---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 3
section_title: Endomorphismes de Fredholm et endomorphismes de Riesz
lang: en
source: ts-iii-v-fr
book_pages: TS III.39-TS III.55, TS III.120-TS III.122
pdf_pages: 0053-0069, 0134-0136
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et applications linéaires de rang fini
      page: 39
      pdf_page: 53
    - "no": 2
      title: Applications de Fredholm
      page: 40
      pdf_page: 54
    - "no": 3
      title: Indice d’une application de Fredholm
      page: 43
      pdf_page: 57
    - "no": 4
      title: Endomorphismes de Riesz
      page: 45
      pdf_page: 59
    - "no": 5
      title: Applications de Fredholm et applications de Riesz entre espaces de Fréchet
      page: 52
      pdf_page: 66
    - "no": 6
      title: Caractérisation spectrale des endomorphismes de Riesz
      page: 53
      pdf_page: 67
statements: 31
exercises: 8
content_sha256: 98281531585184fdb511b806baf9788ce825200769240d82ff23b99318d7a1d4
translated_from: content/fr/ts/III/03_s3_endomorphismes_de_fredholm_et.md
source_lang: fr
translation_method: machine
source_content_sha256: f0bf77fa9308554f60c7f8a07ca6130c6ad5b94df1f911389b5fdb30d78f3161
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-8f276bb3
glossary_version: 34
glossary_terms_sha256: 86b55dc4b721d1e25cc728a6b39fd06ee689628876c48607779afd6c6e66d9f5
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. FREDHOLM ENDOMORPHISMS AND RIESZ ENDOMORPHISMS

### 1. Strict morphisms and linear mappings of finite rank

#### Proposition 1 {#ts-iii-s3-prop-1 .statement tag=02RE}

Let E and F be locally convex spaces, $E_1$ a closed subspace of finite codimension of E and $u$ a continuous linear mapping of E into F. In order that $u$ be a strict morphism with closed image, it is necessary and sufficient that $u|E_1$ be one.

Suppose first that the linear mapping $u|E_1$ is injective. Then we have $E_1\cap$ Ker($u$) $=\{0\}$, so that Ker($u$) is of finite dimension. Let S be a vector subspace of E supplementary to $E_1+$ Ker($u$). The space E is a topological direct sum of $E_1$, Ker($u$) and S (EVT, I, p. 15, cor. 4 and prop. 3). If $u$ is a strict morphism with closed image, it defines by restriction an isomorphism of $E_1\oplus S$ onto a closed vector subspace of F, and fortiori an isomorphism of $E_1$ onto a closed vector subspace of F. Conversely, suppose that $u$ defines by restriction an isomorphism of $E_1$ onto $u(E_1)$ and that $u(E_1)$ is closed in F. We have $u(E) =u(E_1)\oplus u(S)$. It follows that $u(E)$ is a topological direct sum of $u(E_1)$ and $u$(S), and is closed in F (loc. cit.). Since $u(E_1)$ is closed and we have $u(E_1)\cap u(S) =\{0\}$, the space $u(S)$ is separated and $u$ defines by restriction an isomorphism of S onto $u(S)$ (EVT, I, p. 15, cor. de la prop. 3), hence also of $E_1\oplus S$ onto $u(E)$. This proves that $u$ is a strict morphism with closed image.

Passing to the general case. Put $N = E_1\cap$ Ker($u$) and $G = E/N$. The locally convex space $E_1/N$ identifies with a closed vector subspace of finite codimension $G_1$ of G. Let $v: G\rightarrow F$ be the continuous linear mapping deduced from $u$ by passing to the quotient. In order that $u$ (resp. $u|E_1$) be a strict morphism with closed image, it is necessary and sufficient that $v$ (resp. $v|G_1$) be one. This reduces us to the case already treated.

#### Corollary 1 {#ts-iii-s3-prop-1-cor-1 .statement tag=02RF}

Suppose that F is separated. Let $v\in \mathscr{L}^f(E; F)$. If $u$ is a strict morphism with closed image from E into F, then the same is true of $u+v$.

Since F is separated, the kernel of $v$ is a closed vector subspace of E; it is of finite codimension in E and $u+v$ has the same restriction as $u$ to Ker($v$). The corollary follows thus from the proposition.

#### Corollary 2 {#ts-iii-s3-prop-1-cor-2 .statement tag=02RG}

Let T be a separated vector subspace of finite dimension of F. Let $\pi : F\rightarrow F/T$ be the canonical surjection. In order that $u$ be a strict morphism with closed image, it is necessary and sufficient that $\pi \circ u$ be one.

The identical mapping of T onto itself extends to a continuous mapping $q: F\rightarrow T$ (EVT, II, p. 26, remark). The kernel S of $q$ is a closed topological supplementary subspace of T. Let $p: F\rightarrow F$ be the projector with image S associated with the decomposition $F = T\oplus S$. For $\pi \circ u$ to be a strict morphism with closed image, it is necessary and sufficient that $p\circ u$ be one. Now $p\circ u$ and $u$ have the same restriction to $\overset{-1}{u}$(S), which is a closed vector subspace of finite codimension of E, and the assertion follows from the proposition.

### 2. Fredholm mappings

Let E and F be locally convex spaces. In this number, we denote by $u\equiv v$ the congruence modulo $\mathscr{L}^f(E; F)$ of the elements $u$ and $v$ of $\mathscr{L}(E; F)$.

If G is a locally convex space, and if $u'$ and $v'$ are elements of $\mathscr{L}(F; G)$, the relations $u\equiv v$ and $u'\equiv v'$ imply the relation $u'\circ u\equiv v'\circ v$.

An element $w$ of $\mathscr{L}(F; E)$ is said to be a quasi-inverse of the element $u$ of $\mathscr{L}(E; F)$ if one has $w\circ u\equiv 1_E$ and $u\circ w\equiv 1_F$.

Suppose that $w$ is a quasi-inverse of $u$. If $u_1$ is an element of $\mathscr{L}(E; F)$ and $w_1$ is an element of $\mathscr{L}(F; E)$ such that $u_1\equiv u$ and $w_1\equiv w$, then $w_1$ is a quasi-inverse of $u_1$ since $w\circ u\equiv w_1\circ u_1$ and $u\circ w\equiv u_1\circ w_1$.

If $w$ and $w_1$ are quasi-inverses of $u$, then $w_1\equiv w$ since

$$
w_1= 1_E\circ w_1\equiv w\circ u\circ w_1\equiv w\circ 1_F=w
$$

#### Definition 1 {#ts-iii-s3-def-1 .statement tag=02RH}

Let E and F be locally convex spaces. An element $u$ of $\mathscr{L}(E; F)$ is said to be a Fredholm mapping[^1] if it possesses a quasi-inverse. A Fredholm mapping from E into E is called a Fredholm endomorphism of E.

We shall denote by $\mathscr{F}(E; F)$ the set of Fredholm mappings from E into F, and by $\mathscr{F}(E)$ the set of Fredholm endomorphisms of E.

#### Remark {#ts-iii-s3-n2-rem-1 .statement tag=02RI}

Let E, F and G be locally convex spaces, $u: E\rightarrow F$ and $v: F\rightarrow G$ continuous linear mappings.

1) Suppose that $u$ is a Fredholm mapping and let $u_1$ be a quasi-inverse of $u$. Since $u$ is a quasi-inverse of $u_1$, the mapping $u_1$ is a Fredholm mapping.

2) Suppose that $u$ and $v$ are mappings of Fredholm, and let $u_1$ (resp. $v_1$) be a quasi-inverse of $u$ (resp. $v$). Then $v\circ u$ is a mapping of Fredholm from E into G and $u_1\circ v_1$ is a quasi-inverse of $v\circ u$. Indeed, one calculates

$$
(u_1\circ v_1)\circ (v\circ u) =u_1\circ (v_1\circ v)\circ u\equiv u_1\circ 1_F\circ u=u_1\circ u\equiv 1_E
$$

$$
(v\circ u)\circ (u_1\circ v_1) =v\circ (u\circ u_1)\circ v_1\equiv v\circ 1_F\circ v_1=v\circ v_1\equiv 1_G
$$

3) Suppose that $u$ and $v\circ u$ are mappings of Fredholm, and let $w_1$ be a quasi-inverse of $v\circ u$. Then $v$ is a mapping of Fredholm and $u\circ w_1$ is a quasi-inverse of $v$.

Indeed, $w_1$ is a mapping of Fredholm according to the first remark. Let $u_1$ be a quasi-inverse of $u$; according to the second remark, $u\circ w_1$ is a mapping of Fredholm and $(v\circ u)\circ u_1$ is a quasi-inverse of it. We have $u\circ u_1\equiv 1_F$, whence $v\circ u\circ u_1\equiv v$; this proves the assertion.

4) Suppose that $v$ and $v\circ u$ are mappings of Fredholm, and let $w_1$ be a quasi-inverse of $v\circ u$. Then $u$ is a mapping of Fredholm and $w_1\circ v$ is a quasi-inverse of $u$.

The proof is analogous to that of the preceding remark.

#### Lemma 1 {#ts-iii-s3-lem-1 .statement tag=02RJ}

Let E and F be locally convex spaces and let $u$ be a mapping of Fredholm from E into F. The kernel and the cokernel of $u$ are of finite dimension.

Let $v: F\rightarrow E$ be a quasi-inverse of $u$. The kernel of $u$ is contained in the image of the finite rank linear mapping $1_E-v\circ u$, hence is of finite dimension. The image of $u$ contains the kernel of the finite rank linear mapping $1_F-u\circ v$, hence is of finite codimension in F.

#### Proposition 2 {#ts-iii-s3-prop-2 .statement tag=02RK}

Let E and F be separated locally convex spaces and let $u$ be an element of $\mathscr{L}(E; F)$. The following properties are equivalent:

(i) The mapping $u$ is a mapping of Fredholm;

(ii) The mapping $u$ is a strict morphism, its kernel is of finite dimension, its image is closed and of finite codimension in F ;

(iii) There exist closed vector subspaces of finite codimension $E_1$ of E and $F_1$ of F such that $u$ defines by passing to the subspaces an isomorphism of $E_1$ onto $F_1$;

(iv) There exist decompositions into topological direct sum $E = E_1\oplus E_2$ and $F = F_1\oplus F_2$ such that $E_2$ and $F_2$ are of finite dimension, that $u$ vanishes on $E_2$ and defines by passing to the subspaces an isomorphism of $E_1$ onto $F_1$.

(i) $=\Rightarrow$ (iii): Let $v$ be a quasi-inverse of $u, E_1$ the kernel of $1_E-v\circ u$ and $F_1$ that of $1_F-u\circ v$. Since the linear mappings $1_E-v\circ u$ and $1_F-u\circ v$ are continuous and of finite rank, $E_1$ and $F_1$ are closed vector subspaces of finite codimension of E and F respectively. Let $x\in E_1$. We have

$$
(1_F-u\circ v)(u(x)) =u((1_E-v\circ u)(x)) =u(0) = 0
$$

whence $u(x)\in F_1$. Therefore $u(E_1)\subset F_1$; analogously, $v(F_1)\subset E_1$. The continuous linear mappings $u_1: E_1\rightarrow F_1$ and $v_1: F_1\rightarrow E_1$ induced by $u$ and $v$ are then isomorphisms inverse to one another, since $v\circ u$ and $1_E$ (resp. $u\circ v$ and $1_F$) coincide on $E_1$ (resp. on $F_1$).

(iii) $=\Rightarrow$ (ii): Let $E_1$ and $F_1$ satisfy the hypothesis of (iii). We have $E_1\cap$ Ker($u$) $=\{0\}$ and $F_1\subset$ Im($u$), hence Ker($u$) is finite-dimensional and Im($u$) is closed and of finite codimension in F. It follows from Prop. 1 of III, p. 39 that the mapping $u$ is a strict morphism.

(ii) $=\Rightarrow$ (iv): Suppose condition (ii) satisfied. The closed vector subspace $E_2=$ Ker($u$) of E is finite-dimensional, and there exists a vector subspace $E_1$ of E which is a topological supplement of $E_2$ (TVS, II, p. 27, Cor. 2). The vector subspace $F_1=$ Im($u$) of F is closed and of finite codimension, and admits a topological supplement $F_2$ in F. By Prop. 1 of III, p. 39, the mapping $u|E_1$ is a strict morphism, hence $u$ induces an isomorphism of $E_1$ onto $F_1$.

(iv) $=\Rightarrow$ (i): Under the hypotheses of (iv), the linear mapping of F into E which coincides with $u^{-1}_1$ on $F_1$ and is zero on $F_2$ is a quasi-inverse of $u$.

#### Remark 5 {#ts-iii-s3-n2-rem-5 .statement tag=02RL}

Let E, F be separated locally convex spaces and $u: E\rightarrow F$ a Fredholm mapping. If $u$ is bijective, then $u$ is an isomorphism (in fact, $u$ is a strict morphism by Prop. 2, (ii)).

### 3. Index of a Fredholm Mapping

Let E, F and G be locally convex spaces.

Let $u: E\rightarrow F$ be a Fredholm mapping. The vector spaces Ker($u$) and Coker($u$) are finite-dimensional (Lemma 1 of III, p. 41). Recall that the integer number

(1) dim Coker($u$)$-$ dim Ker($u$) $=$ codim$_F$ Im($u$)$-$ dim Ker($u$)

is called the index of $u$ and is denoted by ind($u$) (A, V, p. 126).

If $u: E\rightarrow F$ and $v: F\rightarrow G$ are Fredholm mappings, the same is true of $v\circ u($III, p. 41, remark 2), and one has (A, V, p. 127, lemma 2)

(2) ind($v\circ u$) $=$ ind($v$) $+$ ind($u$).

Suppose that E and F are separated and let $u: E\rightarrow$ F be a Fredholm mapping; adopt the notations of condition (iv) of prop. 2 of III, p. 42. Then we have ind($u$) $=$ dim(F$_2$)$-$ dim(E$_2$). Equip the dual of each of these spaces with the weak topology (resp. the compact topology, the topology of bounded convergence). Then $E'$ is identified with the topological direct sum of $E'_1$ and $E'_2$, and $F'$ with that of $F'_1$ and $F'_2$, and $^tu$ induces an isomorphism of $F'_1$ onto $E'_1$ and vanishes on $F'_2$. Hence the transpose $^tu: F'\rightarrow E'$ is a Fredholm mapping (loc. cit.). The kernel of $^tu$ is $F'_2$, and its dimension is that of $F_2$, that is to say that of the cokernel of $u$. Hence

(3) ind($u$) $=$ dim Ker($^tu$)$-$ dim Ker($u$). Moreover, the image of $^tu$ is $E'_1$, and the dimension of the cokernel of $^tu$ is therefore equal to the dimension of $E'_2$, which is that of the kernel $E_2$ of $u$. We deduce

(4) ind($^tu$) $=-$ ind($u$).

Suppose that E and F are separated and let $u: E\rightarrow$ F be a Fredholm mapping of index 0. Then $u$ is a strict morphism according to prop. 2 of III, p. 42. Since dim Ker($u$) $=$ codim$_F$ Im($u$), the mapping $u$ is an isomorphism as soon as it is injective or surjective.

#### Proposition 3 {#ts-iii-s3-prop-3 .statement tag=02RM}

Let E and F be locally convex spaces and $u\in \mathscr{L}(E; F)$. Let $E_1($resp. $F_1)$ be a closed subspace of finite codimension of E (resp. F). We suppose that $u$ maps $E_1$ into $F_1$ and denote by $u_1\in \mathscr{L}(E_1; F_1)$ the mapping which coincides with $u$ on $E_1$. For $u$ to be a Fredholm mapping, it is necessary and sufficient that $u_1$ be one. We then have

(5) ind($u$)$-$ ind($u_1$) $=$ codim$_F(F_1)-$ codim$_E(E_1)$.

Let $i: E_1\rightarrow E$ and $j: F_1\rightarrow F$ be the canonical injections. They are Fredholm mappings, and we have

ind($i$) $=$ codim$_E(E_1)$, ind($j$) $=$ codim$_F(F_1)$.

Since $j\circ u_1=u\circ i$, we see that $u$ is a Fredholm mapping if and only if $u_1$ is one (Remarks 3 and 4 of III, p. 41). If this is so, we have

ind($j$) $+$ ind($u_1$) $=$ ind($j\circ u_1$) $=$ ind($u\circ i$) $=$ ind($u$) $+$ ind($i$),

whence formula (5).

#### Proposition 4 {#ts-iii-s3-prop-4 .statement tag=02RN}

Let E and F be separated locally convex spaces, $u: E\rightarrow F$ a Fredholm mapping, and $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ the extension of $u$ to the completions. Then $\widehat{u}$ is a Fredholm mapping and we have Ker($\widehat{u}$) $=$ Ker($u$) and ind($\widehat{u}$) $=$ ind($u$).

Let us adopt the notation of condition (iv) of Prop. 2 of III, p. 42. Since the vector spaces $E_2$ and $F_2$ are finite-dimensional, they are complete. The completion of $E_1$ (resp. $F_1$) is identified with the closure of $E_1$ in $\widehat{E}$ (resp. of $F_1$ in $\widehat{F}$), and $\widehat{E}$ (resp. $\widehat{F}$) is the topological direct sum of $\widehat{E}_1$ and $E_2$ (resp. $\widehat{F}_1$ and $F_2$). The linear mapping $\widehat{u}$ defines by restriction an isomorphism of $\widehat{E}_1$ onto $\widehat{F}_1$ and vanishes on $E_2$. The proposition then follows from implication (iv)$\Rightarrow$(i) of loc. cit.

### 4. Riesz Endomorphisms

Let E be a vector space and let $u$ be an endomorphism of E.

The sequence (Ker($u^n$))$_{n\in\mathbf{N}}$ of vector subspaces of E is increasing; their union is a subspace of E stable under $u$ which is called the nilespace of $u$.

The sequence (Im($u^n$))$_{n\in\mathbf{N}}$ of vector subspaces of E is decreasing; their intersection is a subspace of E stable under $u$ which is called the conilespace of $u$.

#### Lemma 2 {#ts-iii-s3-lem-2 .statement tag=02RO}

Let E be a vector space and let $u$ be an endomorphism of E which possesses an index (A, V, p. 126).

If two of the following properties are satisfied, so is the third:

(i) The endomorphism $u$ is of index 0;

(ii) The nilespace N of $u$ is finite-dimensional;

(iii) The conilespace I of $u$ is of finite codimension.

For every integer $n\geqslant 0$, the endomorphism $u^n$ possesses an index, equal to $n$ ind($u$) (A, V, p. 127, Lemma 2). The sequence (dim(Ker($u^n$)))$_{n\in\mathbf{N}}$ of natural integers is increasing; for it to be stationary, it is necessary and sufficient that the nilespace of $u$ be finite-dimensional. The sequence (codim$_E$(Im($u^n$)))$_{n\in\mathbf{N}}$ of natural integers is increasing; for it to be stationary, it is necessary and sufficient that the conilespace of $u$ be of finite dimension. Suppose condition (i) satisfied; the relation

dim(Ker($u^n$))$-$ codim$_E$(Im($u^n$)) $=$ ind($u^n$) $=n$ ind($u$) $= 0$

then entails the equivalence of conditions (ii) and (iii). Conversely, if conditions (ii) and (iii) are satisfied, this formula entails that the sequence $(n$ ind($u$))$_{n\in\mathbf{N}}$ is stationary, hence $u$ is of index zero.

#### Lemma 3 {#ts-iii-s3-lem-3 .statement tag=02RP}

Let E be a vector space and let $u$ be an endomorphism of E which possesses an index. Suppose that the index of $u$ is zero. Let N be the nilespace of $u$ and I its conilespace.

a) The space E is then the direct sum of the subspaces N and I (Weyr-Fitting decomposition, cf. A, VIII, §2, n$^o2$, p. 25).

b) The endomorphism $u$ induces, by passing to the subspaces, a nilpotent endomorphism of N and an automorphism $u_I$ of I.

c) Let $v$ denote the endomorphism of E which is zero on N and which coincides with $u^{-1}_I$ on I. One has $u\circ v=v\circ u$ and the endomorphism $1_E-u\circ v$ is the projector with image N and kernel I.

d) Every endomorphism of E which commutes with $u$ stabilises N and I, and commutes with $v$.

The endomorphism $u$ satisfies the properties of the preceding lemma.

Let $n\in \mathbf{N}$ be such that Ker($u^n$) $= N$. Then Ker($u^m$) $=$ Ker($u^n$) for every integer $m\geqslant n$; since ind($u^m$) $=m$ ind($u$) $= 0$, this implies Im($u^m$) $=$ Im($u^n$) for $m\geqslant n$, hence I = Im($u^n$). It follows from A, VIII, p. 25, prop. 2 that assertions a) and b) are satisfied.

For every $x\in N$, one has $v(x) = 0$ and $u(x)\in N$, hence $u(v(x)) = 0$ and $v(u(x)) = 0$. For every $x\in I$, one has $u(v(x)) =v(u(x)) =x$. This implies that $u\circ v=v\circ u$ and that $1_E-u\circ v$ is the projector with image N and kernel I.

Let $w$ be an endomorphism of E which commutes with $u$. Let $n\in \mathbf{N}$ be such that N = Ker($u^n$) and I = Im($u^n$). Let $x\in N$; one has $u^n(w(x)) =w(u^n(x)) = 0$, hence $w(x)\in N$. Let $x\in I$; there exists $y\in E$ such that $x=u^n(y)$; then, $w(x) =w(u^n(y)) =u^n(w(y))\in I$. This proves that $w$ stabilises N and I.

Let us prove finally that $w$ and $v$ are permutable. For every $x$ in N, one has $v(w(x)) = 0 =w(v(x))$. Let $x\in I$; the elements $v(w(x))$ and $w(v(x))$ of E belong to I and their images under $u$ are both equal to $w(x)$, hence they are equal. By linearity, this implies that $v$ and $w$ commute.

#### Remark {#ts-iii-s3-n4-rem-1 .statement tag=02RQ}

Suppose there exists an integer $n\geqslant 0$ such that Ker($u^n$) $=$ Ker($u^{n+1}$) (resp. Im($u^n$) $=$ Im($u^{n+1}$)); one then has Ker($u^m$) $=$ Ker($u^n$) (resp. Im($u^m$) $=$ Im($u^n$)) for every integer $m\geqslant n$.

Suppose $u$ of index zero. For every integer $n\geqslant 0$, one has

$n$ ind($u$) $=$ ind($u^n$) $=$ codim$_E$(Im($u^n$))$-$ dim(Ker($u^n$)).

The conditions Ker($u^n$) $=$ Ker($u^{n+1}$) and Im($u^n$) $=$ Im($u^{n+1}$) are therefore equivalent. When they are satisfied, the vector space E is the direct sum of Ker($u^n$) and of Im($u^n$) (A, VIII, p. 25, prop. 2), the space Ker($u^n$) is finite-dimensional, and $u$ induces, by passing to the subspace, an automorphism of Im($u^n$).

#### Definition 2 {#ts-iii-s3-def-2 .statement tag=02RR}

Let E be a separated locally convex space. A Riesz endomorphism of E means any Fredholm endomorphism of E whose nilspace is finite-dimensional and whose conilspace is of finite codimension.

#### Proposition 5 {#ts-iii-s3-prop-5 .statement tag=02RS}

Let E be a separated locally convex space. Every Riesz endomorphism of E is of index zero.

This follows from the definition and lemma 2.

#### Example 1 {#ts-iii-s3-n4-exa-1 .statement tag=02RT}

Every automorphism of E is a Riesz endomorphism of E. If E is finite-dimensional, every element of $\mathscr{L}(E)$ is a Riesz endomorphism of E.

#### Example 2 {#ts-iii-s3-n4-exa-2 .statement tag=02RU}

If $(E_i)_{i\in I}$ is a finite family of separated locally convex spaces and $u_i$ an element of $\mathscr{L}(E_i)$ for every $i$ in I, the endomorphism $u=\bigoplus_{i\in I}u_i$ of the locally convex space $\bigoplus_{i\in I}E_i$ is a Riesz endomorphism if and only if $u_i$ is one for every $i$.

#### Example 3 {#ts-iii-s3-n4-exa-3 .statement tag=02RV}

Let E be a separated locally convex space over $\mathbf{R}$, and let $E_{(\mathbf{C})}$ be its complexification. Let $u$ be an endomorphism of E. In order that $u$ be a Riesz endomorphism, it is necessary and sufficient that its complexification $u_{(\mathbf{C})}$ be a Riesz endomorphism of $E_{(\mathbf{C})}$.

#### Proposition 6 {#ts-iii-s3-prop-6 .statement tag=02RW}

Let E be a separated locally convex space and let $u$ be a Riesz endomorphism of E. Let N denote the nilspace of $u$ and I its conilspace.

a) The subspaces N and I of E are closed and stable under $u$, and the space E is their topological direct sum;

b) The endomorphism $u$ defines by restriction an automorphism $u_I$ of I;

c) The vector space N is finite-dimensional and $u$ defines by restriction a nilpotent endomorphism $u_N$ of N;

d) Let $v$ be the element of $\mathscr{L}(E)$ which is zero on N and coincides with $u^{-1}_I$ on I. It is a Riesz endomorphism of E and a quasi-inverse of $u$ which commutes with $u$. The endomorphism $1_E-u\circ v$ of E is the projector with image N and kernel I. Every element of $\mathscr{L}(E)$ which commutes with $u$ stabilizes N and I, and commutes with $v$.

Let $n$ be a natural number such that Ker($u^n$) $= N$ and Im($u^n$) $= I$. Since E is separated and $u$ is continuous, N = Ker($u^n$) is closed in E. Since $u$ is a Fredholm endomorphism, the same is true of $u^n$, and I = Im($u^n$) is closed (III, p. 42, prop. 2). By lemma 2, the space E is the direct sum of N and I and assertion a) then follows from prop. 3 of EVT, I, p. 15.

Since I is closed, of finite codimension in E and stable under $u$, the mapping $u_I: I\rightarrow I$ deduced from $u$ is a Fredholm endomorphism (III, p. 44, prop. 3); it is also bijective, hence it is an automorphism of I (III, p. 42, prop. 2). This proves b), and the remaining assertions follow from lemma 2.

The endomorphism $v$ defined in assertion d) of the proposition is a quasi-inverse of $u$, called the canonical quasi-inverse of $u$.

Riesz endomorphisms have certain of the stability properties of Fredholm mappings.

#### Proposition 7 {#ts-iii-s3-prop-7 .statement tag=02RX}

Let E be a separated locally convex space and let $u$ be an endomorphism of E.

a) Let $E_1$ be a closed subspace of finite codimension of E, stable under $u$. Let $u_1$ denote the element of $\mathscr{L}(E_1)$ which coincides with $u$ on $E_1$. Then $u$ is a Riesz endomorphism if and only if $u_1$ is one;

b) Suppose that $u$ is a Fredholm endomorphism of index 0. Let $\widehat{E}$ be the completion of E and let $\widehat{u}\in \mathscr{L}(\widehat{E})$ be the extension of $u$ by continuity. Then $u$ is a Riesz endomorphism if and only if $\widehat{u}$ is one;

c) Endow the dual $E'$ of E with the topology of bounded convergence, the topology of compact convergence, or the weak topology. If $u$ is a Riesz endomorphism of E, then $^tu$ is a Riesz endomorphism of $E'$.

a) In order that $u$ be a Fredholm endomorphism of index zero, it is necessary and sufficient that $u_1$ be one (III, p. 44, prop. 3). On the other hand, for every $n\in \mathbf{N}$, one has Ker($u^n_1$) $= E_1\cap$ Ker($u^n$), whence

dim Ker($u^n_1$)$\leqslant$ dim Ker($u^n$)$\leqslant$ dim Ker($u^n_1$) $+$ codim$_E(E_1)$,

therefore the sequence (dim Ker($u^n$))$_{n\in\mathbf{N}}$ is bounded if and only if the sequence (dim Ker($u^n_1$))$_{n\in\mathbf{N}}$ is. Hence, $u$ is a Riesz endomorphism of E if and only if $u_1$ is a Riesz endomorphism of $E_1$ (lemma 2).

b) By prop. 4 of III, p. 44, for every $n\in \mathbf{N}$, the mapping $\widehat{u}^n$ is a Fredholm endomorphism of $\widehat{E}$ such that Ker($\widehat{u}^n$) $=$ Ker($u^n$) and ind($\widehat{u}^n$) $=$ ind($u^n$) $=n$ ind($u$). Hence, $u$ is a Riesz endomorphism if and only if $\widehat{u}$ is a Riesz endomorphism.

c) The transpose $^tu$ is a Fredholm endomorphism of index 0 of $E'($III, p. 43, n$^o3$). Since the kernel of $(^tu)^n$ is the orthogonal of the image of $u^n$ (EVT, IV, p. 27, prop. 2), the sequence (Ker($^tu$)$^n$)$_n$ is stationary. This proves that $^tu$ is a Riesz endomorphism of $E'$.

#### Proposition 8 {#ts-iii-s3-prop-8 .statement tag=02RY}

Let E be a separated locally convex space and $u$ an endomorphism of E. The following conditions are equivalent:

(i) $u$ is a Riesz endomorphism of E;

(ii) There exists a quasi-inverse $v$ of $u$ which commutes with $u$;

(iii) There exists a closed vector subspace $E_1$ of E, of finite codimension, stable under $u$, such that $u$ induces an automorphism of $E_1$.

The implication (i) $=\Rightarrow$ (ii) follows from prop. 6, d).

Suppose that $u$ possesses a quasi-inverse $v$ which is permutable with $u$. The kernel $E_1$ of $1_E-u\circ v$ is a closed vector subspace of E, of finite codimension, stable under $u$ and $v$. Since one has $u(v(x)) =v(u(x)) =x$ for every $x\in E_1$, the mappings $u$ and $v$ induce automorphisms of $E_1$ inverse to one another. Thus (ii) implies (iii).

Finally, the implication (iii) $=\Rightarrow$ (i) follows from assertion a) of prop. 7 and from the fact that an automorphism is a Riesz endomorphism.

#### Proposition 9 {#ts-iii-s3-prop-9 .statement tag=02RZ}

Let E be a separated locally convex space and let $u,v$ be permutable elements of $\mathscr{L}(E)$. The following conditions are equivalent:

(i) The endomorphisms $u$ and $v$ are Riesz endomorphisms;

(ii) The endomorphism $u\circ v$ is a Riesz endomorphism.

Suppose that $u$ and $v$ are Riesz endomorphisms; let $u'$ and $v'$ denote their canonical quasi-inverses. The endomorphisms $u,v,u'$ and $v'$ of E commute (prop. 6, d)). The endomorphism $v'\circ u'$ is a quasi-inverse of $u\circ v$ which commutes with $u\circ v$, hence $u\circ v$ is a Riesz endomorphism (prop. 8).

Suppose conversely that $u\circ v$ is a Riesz endomorphism, and let $w$ be its canonical quasi-inverse. Since $u$ commutes with $u\circ v$, the endomorphisms $u$ and $w$ commute by prop. 6, d). Analogously $v$ and $w$ commute. Hence the endomorphisms $u,v$ and $w$ of E commute; it follows that the endomorphism $v\circ w$ of E is a quasi-inverse of $u$ and that $w\circ u$ is a quasi-inverse of $v$. By prop. 8$,u$ and $v$ are Riesz endomorphisms.

Let $u$ be a Riesz endomorphism of E. If $v$ is an automorphism of E, the endomorphism $u\circ v$ of E is not necessarily a Riesz endomorphism of E, even if $u\circ v-v\circ u$ is of finite rank. If $h$ is an endomorphism of finite rank of E, the endomorphism $u+h$ is not necessarily a Riesz endomorphism (cf. III, p. 120, exercise 3).

#### Proposition 10 {#ts-iii-s3-prop-10 .statement tag=02S0}

Let E and F be locally convex spaces, $p\in \mathscr{L}(E; F)$ and $q\in \mathscr{L}(F; E)$. Put $u= 1_E-q\circ p$ and $v= 1_F-p\circ q$.

a) Let $n\in \mathbf{N}$. The mapping $p$ defines by restriction an isomorphism of topological vector spaces of Ker($u^n$) onto Ker($v^n$) and defines by passing to the quotients an isomorphism of topological vector spaces of Coker($u^n$) onto Coker($v^n$);

b) If the image of $u$ is closed in E, that of $v$ is closed in F;

c) If Ker($u$) has a topological complement in E, then Ker($v$) has one in F. If Im($u$) has a topological complement in E, then Im($v$) has one in F;

d) If $u$ is a strict morphism, then $v$ is a strict morphism;

e) If $u$ is an automorphism of E, then $v$ is an automorphism of F;

f) If $u$ is a Fredholm endomorphism of E, then $v$ is a Fredholm endomorphism of F, and one has ind($u$) $=$ ind($v$);

g) Suppose E and F separated. If $u$ is a Riesz endomorphism of E, then $v$ is a Riesz endomorphism of F.

First of all, let us note the formulas

$$
q\circ v=u\circ q,v\circ p=p\circ u \tag{6}
$$

We then prove two lemmas.

#### Lemma 4 {#ts-iii-s3-lem-4 .statement tag=02S1}

Let $n\in \mathbf{N}$. Put

$ni-1(n)i-1$

$q_n=\sum(-1)q\circ (p\circ q)$.

$$
i
$$

$i=1$

We have $u^n= 1_E-q_n\circ p$ and $v^n= 1_F-p\circ q_n$.

We have $(q\circ p)^i=q\circ (p\circ q)^{i-1}\circ p$ for every integer $i\geqslant 1$. We then calculate

$nnni-1(n)i$

$u= (1_E-q\circ p)= 1_E-\sum(-1)(q\circ p)= 1_E-q_n\circ p$

$$
i
$$

$$
i=1
$$

$nnni-1(n)i$

$v= (1_F-p\circ q)= 1_F-\sum(-1)(p\circ q)= 1_F-p\circ q_n$,

$$
i
$$

$i=1$

whence the result.

#### Lemma 5 {#ts-iii-s3-lem-5 .statement tag=02S2}

Let $u'$ be an element of $\mathscr{L}(E)$. Put $v'= 1_F+p\circ u'\circ q$. If $u'$ is an inverse of $u$, then $v'$ is an inverse of $v$. If $u'$ is a quasi-inverse of $u$, then $v'$ is a quasi-inverse of $v$. If $u'$ commutes with $u$, then $v'$ commutes with $v$.

Using formulas (6), we calculate

$$
v-v'\circ v=-p\circ u'\circ q\circ v=-p\circ u'\circ u\circ q
$$

$$
v-v\circ v'=-v\circ p\circ u'\circ q=-p\circ u\circ u'\circ q
$$

whence

$$
1_F-v'\circ v=p\circ (1_E-u'\circ u)\circ q
$$

$$
1_F-v\circ v'=p\circ (1_E-u\circ u')\circ q
$$

which proves the lemma.

Let us prove Prop. 10. Taking Lemma 4 into account, it is enough to prove assertion a) for $n= 1$. By formulas (6), the mappings $p$ and $q$ define by passing to the subspaces continuous linear mappings $p':$ Ker($u$)$\rightarrow$ Ker($v$) and $q':$ Ker($v$)$\rightarrow$ Ker($u$), and by passing to the quotients continuous linear mappings $p'':$ Coker($u$)$\rightarrow$ Coker($v$) and $q'':$ Coker($v$)$\rightarrow$ Coker($u$).

Since $1_E-u=q\circ p$ and $1_F-v=p\circ q$, the mappings $p'$ and $q'$ on the one hand, $p''$ and $q''$ on the other hand, are isomorphisms reciprocal to one another. This proves a).

For the image of a continuous linear mapping to be closed, it is necessary and sufficient that the cokernel of this mapping be a separated space. Thus b) results from a).

Let us denote by $i: Ker(u)\rightarrow E$ and $j:$ Ker($v$)$\rightarrow F$ the canonical injections. Suppose that Ker($u$) possesses a topological complement in E, and let $r: E\rightarrow$ Ker($u$) be a continuous linear retraction of $i$. Put $r'=p'\circ r\circ q$. We have $r'\in \mathscr{L}(F$; Ker($v$)) and

$$
r'\circ j=p'\circ r\circ q\circ j=p'\circ r\circ i\circ q'=p'\circ q'= 1_{Ker(v)}
$$

therefore $r'$ is a continuous linear retraction of $j$ and Ker($v$) possesses a topological complement in F. This proves the first assertion of c). The second is proved similarly, by remarking that if $s:$ Coker($u$)$\rightarrow E$ is a continuous linear section of the canonical surjection of E onto Coker($u$), then $p\circ s\circ q''$ is one of the canonical surjection of F onto Coker($v$).

Let us denote by $\overline{u}: E/$ Ker($u$)$\rightarrow$ Im($u$) and $\overline{v}: F/$ Ker($v$)$\rightarrow$ Im($v$) the bijective continuous linear mappings induced by $u$ and $v$. By formulas (6), the mapping $p$ defines, by passing to quotients, a continuous linear mapping $p_1: E/$ Ker($u$)$\rightarrow F/$ Ker($v$), and $p,q$ define, by passing to subspaces, continuous linear mappings $p_0:$ Im($u$)$\rightarrow$ Im($v$) and $q_0:$ Im($v$)$\rightarrow$ Im($u$).

Let $t:$ Im($v$)$\rightarrow F/$ Ker($v$) denote the composed mapping of the canonical injection Im($v$)$\rightarrow F$ and the canonical surjection $F\rightarrow F/$ Ker($v$); it is continuous. We have $\overline{v}\circ t= 1_{Im(v)}-p_0\circ q_0$ and $\overline{v}\circ p_1=p_0\circ \overline{u}$, whence

$$
\overline{v}\circ (t+p_1\circ \overline{u}^{-1}\circ q_0) =\overline{v}\circ t+p_0\circ q_0= 1_{Im(v)}
$$

This proves that $t+p_1\circ \overline{u}^{-1}\circ q_0$ is the inverse bijection of $\overline{v}$. If $u$ is strict, the mapping $\overline{u}^{-1}$ is continuous, and the same is true of $\overline{v}^{-1}$, which proves that $v$ is strict. This proves d).

By lemma 5, if $u$ is an automorphism of E, then $v$ is one of F. Analogously, if $u$ is a Fredholm endomorphism of E, then $v$ is one of F, and one then has ind($u$) $=$ ind($v$) by a). This proves e) and f). Finally, if E and F are separated and if $u$ is a Riesz endomorphism of E, then $v$ is one of F by lemma 5 and condition (ii) of prop. 8; this is assertion g).

### 5. Fredholm mappings and Riesz mappings between Fréchet spaces

#### Proposition 11 {#ts-iii-s3-prop-11 .statement tag=02S3}

Let E and F be Fréchet spaces. In order that a continuous linear mapping $u$ of E into F be a Fredholm mapping, it is necessary and sufficient that its kernel and its cokernel be finite-dimensional.

This results from the characterization of Fredholm mappings given by condition (ii) of prop. 2 of III, p. 42 and from the following lemma:

#### Lemma 6 {#ts-iii-s3-lem-6 .statement tag=02S4}

Let E and F be Fréchet spaces and $u\in \mathscr{L}(E; F)$. Suppose that the image of $u$ is of finite codimension in F. Then the image of $u$ is closed in F and $u$ is a strict morphism.

Let G be a vector subspace of F supplementary to Im($u$); the subspace G is closed (TVS, I, p. 14, cor. 1), hence the quotient space $F/G$ is a Fréchet space (TG, IX, p. 25, prop. 4). Let $\pi : F\rightarrow F/G$ be the canonical surjection. The mapping $\pi \circ u$ is surjective, hence strict (TVS, I, p. 19, cor. 3). The assertion then results from cor. 2 of III, p. 40.

#### Proposition 12 {#ts-iii-s3-prop-12 .statement tag=02S5}

Let E and F be Fréchet spaces. Endow their duals $E'$ and $F'$ with the weak topology, the topology of compact convergence, or the topology of bounded convergence. Let $u\in \mathscr{L}(E; F)$. In order that $u$ be a Fredholm mapping of E into F, it is necessary and sufficient that $^tu$ be a Fredholm mapping of $F'$ into $E'$.

The condition is necessary (III, p. 43, n$^o3$). Let us prove that it is sufficient. If $^tu$ is a Fredholm mapping, it is a strict morphism (III, p. 42, prop. 2), hence $u$ is a strict morphism with closed image (TVS, IV, p. 28, th. 1 and p. 29, cor. 3). In view of the canonical isomorphisms Coker($^tu$)$\rightarrow$ Ker($u$)$'$ and Ker($^tu$)$\rightarrow$ Coker($u$)$'$ (TVS, IV, p. 27, prop. 2), the vector spaces Ker($u$) and Coker($u$) are finite-dimensional and $u$ is a Fredholm mapping (prop. 2 of III, p. 42).

#### Proposition 13 {#ts-iii-s3-prop-13 .statement tag=02S6}

Let E be a Fréchet space and $u\in \mathscr{L}(E)$.

a) The endomorphism $u$ is a Riesz endomorphism if and only if its nilspace N is finite-dimensional and its conilspace I is of finite codimension ;

b) Endow $E'$ with the topology of bounded convergence, the topology of compact convergence, or the weak topology. If $^tu$ is a Riesz endomorphism of $E'$, then $u$ is a Riesz endomorphism of E.

a) Suppose that the nilspace N is finite-dimensional and that the conilspace I is of finite codimension. Since Ker($u$)$\subset N$ and $I\subset$ Im($u$), the kernel of $u$ is finite-dimensional and the image of $u$ is of finite codimension. By definition and Proposition 11, the mapping $u$ is a Riesz endomorphism. The converse follows from the definition.

b) According to Proposition 12, the hypothesis implies that $u$ is a Fredholm endomorphism of index ind($^tu$) $=-$ ind($u$) $= 0$ (No.$^o3$, formula (4)). Let $n\in \mathbf{N}$. Since the image of $u^n$ is closed and has as orthogonal the kernel of $^tu^n$ (EVT, IV, p. 27, Prop. 2), the sequence (Im($u^n$)) is stationary, and $u$ is therefore a Riesz endomorphism.

### 6. Spectral characterization of Riesz endomorphisms

Let E be a complex Banach space and $u$ an endomorphism of E. Recall that Sp($u$) denotes the spectrum of $u$ relative to the unital Banach algebra $\mathscr{L}(E) ($cf. § 7 of I, p. 127).

Suppose that 0 is an isolated point of Sp($u$); recall that one then denotes by $e_0(u)$ the spectral projector associated with $u$ and with the open and closed subset $\{0\}$ of the spectrum of $u($cf. No.$^o3$ of I, p. 131). One has $e_0(u) =f(u)$ for every germ of a holomorphic function $f$ in a neighbourhood of Sp($u$) which is equal to 1 in a neighbourhood of 0 and zero in a neighbourhood of Sp($u$)$-\{0\}$.

By passing to subspaces, the endomorphism $u$ induces a quasi-nilpotent endomorphism of the image of $e_0(u)$, whose spectrum reduces to $\{0\}$, and an automorphism of the kernel of $e_0(u)$, whose spectrum is Sp($u$)$-\{0\}($loc. cit.).

#### Proposition 14 {#ts-iii-s3-prop-14 .statement tag=02S7}

Let E be a complex Banach space. In order that an element $u$ of $\mathscr{L}(E)$ be a Riesz endomorphism of E, it is necessary and sufficient that one of the following two mutually exclusive conditions be satisfied:

(i) The endomorphism $u$ of E is an automorphism of E;

(ii) The point 0 is an isolated point of Sp($u$) and the projector $e_0(u)$ has finite rank.

When condition (ii) is satisfied, the image of $e_0(u)$ is the nilspace of $u$ and the kernel of $e_0(u)$ is the conilspace of $u$.

Every automorphism of E is a Riesz endomorphism of E (III, p. 47, remark 1). If $u$ satisfies condition (ii), the kernel F of $e_0(u)$ is a closed vector subspace of finite codimension of E, stable under $u$. Let $u_F$ be the endomorphism of F induced by $u$. Its spectrum is contained in $\mathbf{C}-\{0\}$ (No. 3 of I, p. 131), hence $u_F$ is an automorphism of F. It follows that $u$ is a Riesz endomorphism of E (III, p. 48, prop. 8).

Conversely, let $u$ be a Riesz endomorphism of E. Let N denote its nilspace and I its conilspace. By prop. 6 of III, p. 47, the space E is the topological direct sum of N and I, and the mapping $u$ defines, by passing to the subspaces, a nilpotent endomorphism $u_N$ of N and an automorphism $u_I$ of I. In particular, we have Sp($u_N$)$\subset  \{0\}$ and $0\not \in$ Sp($u_I$). If N is zero, then I = E and $u$ is an automorphism of E. Otherwise, 0 is an isolated point of Sp($u$) and $e_0(u)$ is the projector with image N and kernel I (prop. 2 of I, p. 129); in particular, it is of finite rank.

#### Remark {#ts-iii-s3-n6-rem-1 .statement tag=02S8}

Let E be a real Banach space and let $u$ be an endomorphism of E. Suppose that 0 is an isolated point of the complex spectrum of $u$, that is to say, of the spectrum of the endomorphism $1\otimes u$ of the complexified complete normable space $E_{(\mathbf{C})}$ of E (I, p. 85, No. 13). The subset $\{0\}$ of the complex spectrum of $u$ is open and closed, and invariant under conjugation; let us denote by $e_0(u)\in \mathscr{L}(E)$ the spectral projector associated with it (No. 13 of I, p. 85). Proposition 14 remains valid mutatis mutandis in this setting.

## EXERCISES {#ts-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: Some authors also say "index operator" or "quasi-isomorphism".
