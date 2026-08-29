---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 6
section_title: Propriétés spectrales des endomorphismes des espaces de Banach
lang: en
source: ts-iii-v-fr
book_pages: TS III.82-TS III.101, TS III.128-TS III.142
pdf_pages: 0096-0115, 0142-0156
extraction: native
subsections:
    - "no": 1
      title: Points isolés et points sensibles du spectre
      page: 82
      pdf_page: 96
    - "no": 2
      title: Une partition du spectre
      page: 85
      pdf_page: 99
    - "no": 3
      title: Spectre du transposé d’un endomorphisme
      page: 88
      pdf_page: 102
    - "no": 4
      title: Perturbation par un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 5
      title: Spectre d’un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 6
      title: Cas des espaces hilbertiens
      page: 92
      pdf_page: 106
    - "no": 7
      title: Le théorème de Krein–Rutman
      page: 93
      pdf_page: 107
statements: 36
exercises: 30
content_sha256: ccef81be0b51793e31aeb322d53ffa1bccb3187f62d1475d741e2c9c623ce0f4
translated_from: content/fr/ts/III/06_s6_proprietes_spectrales_des.md
source_lang: fr
translation_method: machine
source_content_sha256: b0d3fa65dcee06679bd7d8f0d92a22736e960414410b5164bd45681a0831abf7
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-d46fbcf4
glossary_version: 34
glossary_terms_sha256: 28da9b9d2dcb190acb78f6ad7e56c5ce29bf3c71c6a41c04870505c132c6f359
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 6. SPECTRAL PROPERTIES OF ENDOMORPHISMS OF BANACH SPACES

Unless otherwise stated, the vector spaces considered in this paragraph are vector spaces over $\mathbf{C}$. The spectrum of an endomorphism of a complete normable space E is the spectrum relative to the unital algebra $\mathscr{L}(E) ($cf. n$^o7$ of I, p. 127).

### 1. Isolated points and sensitive points of the spectrum

Let E be a complete normable space and let $u$ be an endomorphism of E. Let $\lambda$ be an isolated point of the spectrum of $u$. We recall that $e_{\lambda}(u)$ denotes the spectral projector associated with $u$ and with the closed and open set $\{\lambda \}$ of the spectrum of $u$ (n$^o3$ of I, p. 131). The endomorphism $u-\lambda 1_E$ induces an automorphism of Ker($e_{\lambda}(u)$) and a quasinilpotent endomorphism of Im($e_{\lambda}(u)$) $($loc. cit.).

#### Definition 1 {#ts-iii-s6-def-1 .statement tag=02UE}

One says that $\lambda$ is of finite spectral multiplicity for $u$ if the spectral projector $e_{\lambda}(u)$ is of finite rank; in this case, the integer $m_{\lambda}(u) =$ dim(Im($e_{\lambda}(u)$)) is called the spectral multiplicity of $\lambda$ for $u$.

#### Definition 2 {#ts-iii-s6-def-2 .statement tag=02UF}

The isolated points of Sp($u$) of finite spectral multiplicity are called the sensitive points of the spectrum of $u$. The set of sensitive points of Sp($u$) is called the sensitive spectrum of $u$ and is denoted by Sp$_s(u)$.[^1] The complementary set Sp($u$) - Sp$_s(u)$ is called the essential spectrum of $u$ and is denoted by Sp$_e(u)$.

Since the set Sp$_s(u)$ consists of isolated points of Sp($u$), it is open in Sp($u$), discrete, and countable (III, p. 78, lemma 3); it is also bounded. The set Sp$_e(u)$ is closed in Sp($u$), hence compact.

By Prop. 14 of III, p. 54, the sensitive points of the spectrum of $u$ are the complex numbers $\lambda$ such that $u-\lambda 1_E$ is a Riesz endomorphism of E which is not an automorphism of E.

For every complex number $\lambda$, let $N_{\lambda}(u)$ and $I_{\lambda}(u)$ denote the nilspace and the conilspace of the endomorphism $u-\lambda 1_E$ of E. Since E is a Fréchet space, $u-\lambda 1_E$ is a Riesz endomorphism if and only if $N_{\lambda}(u)$ is of finite dimension and $I_{\lambda}(u)$ is of finite codimension (prop. 13 of III, p. 53); when this is so, $u-\lambda 1_E$ is invertible if and only if $N_{\lambda}(u)$ is reduced to 0 (III, p. 47, prop. 6). The sensitive points of the spectrum of $u$ are therefore the complex numbers $\lambda$ such that $N_{\lambda}(u)$ is of nonzero finite dimension and $I_{\lambda}(u)$ is of finite codimension in E (III, p. 54, prop. 14). The spectral multiplicity $m_{\lambda}(u)$ of $\lambda$ is then the dimension of $N_{\lambda}(u)$, the endomorphism $u-\lambda 1_E$ defines by restriction an automorphism of $I_{\lambda}(u)$ and a nilpotent endomorphism of $N_{\lambda}(u)$. Since $N_{\lambda}(u)$ is not reduced to 0, it follows that $\lambda$ is an eigenvalue of $u$. The smallest integer $n\geqslant 1$ such that Ker(($u-\lambda 1_E$)$^n$) is equal to $N_{\lambda}(u)$ is the order of the pole of the resolvent of $u$ at the point $\lambda$ (No.$^o3$ of I, p. 131), which is bounded above by $m_{\lambda}(u)$.

In particular, we have therefore proved:

#### Proposition 1 {#ts-iii-s6-prop-1 .statement tag=02UG}

The sensitive points of the spectrum of $u$ are eigenvalues of finite spectral multiplicity.

The essential spectrum of $u$ consists of the complex numbers $\lambda$ such that $u-\lambda 1_E$ is not a Riesz endomorphism of E. In particular, if $u$ is compact, then every $\lambda \in$ Sp($u$)$-\{0\}$ is a sensitive point of the spectrum (cor. 2 of III, p. 77).

#### Proposition 2 {#ts-iii-s6-prop-2 .statement tag=02UH}

Let E be a complete normable space and $u$ an endomorphism of E. Let H be a finite subset of Sp$_s(u)$. The set H is open and closed in Sp($u$). The spectral projector $e_H(u)$ is of finite rank, has image $\sum_{\lambda\in H}N_{\lambda}(u)$ and kernel $\bigcap_{\lambda\in H}I_{\lambda}(u)$.

This follows from No.$^o3$ of I, p. 131 since, for every $\lambda \in$ Sp$_s(u)$, the subspaces $N_{\lambda}(u)$ and $I_{\lambda}(u)$ are respectively the image and the kernel of the spectral projector $e_{\lambda}(u)$.

#### Corollary 1 {#ts-iii-s6-prop-2-cor-1 .statement tag=02UI}

Let V be a neighbourhood of Sp$_e(u)$.

a) There exists a decomposition of E into a topological direct sum $F\oplus$ G such that F is of finite dimension, that F and G are stable under every endomorphism commuting with $u$, and that the spectrum of the endomorphism of G induced by $u$ is contained in V;

b) Suppose V nonempty. There exists an element $v$ of the bicommutant of $u$ in $\mathscr{L}(E)$ whose spectrum is contained in V and such that $v-u$ is of finite rank.

Let H = Sp($u$)$\cap (\mathbf{C}-\mathring{V})$. The set H is contained in Sp$_s(u)$, hence is discrete; since it is closed in the compact space Sp($u$), it is finite. One can take for F and G the image and the kernel of the spectral projector $e_H(u)$ (Prop. 2).

Suppose that V is nonempty. Let $\mu\in V$ and let $v$ denote the endomorphism of E which agrees with the homothety of ratio $\mu$ in F and with $u$ in G. Its spectrum is contained in $\{\mu\} \cup$ (Sp($u$) - H), hence in V, and $v-u$ is of finite rank since F is finite-dimensional.

For every compact subset S of $\mathbf{C}$, let $\mathscr{O}(S)$ denote the algebra of germs of holomorphic functions in a neighbourhood of S with values in $\mathbf{C}$ (I, p. 49, §4, No. $1$).

#### Corollary 2 {#ts-iii-s6-prop-2-cor-2 .statement tag=02UJ}

Let $f\in \mathscr{O}$(Sp($u$)) and let $\mu$ be a complex number. Let H be the set of $\lambda \in$ Sp($u$) such that $f(\lambda ) =\mu$. Then $\mu$ is a point of the discrete spectrum of $f(u)$ if and only if H is finite, nonempty, and contained in the discrete spectrum of $u$. Under these conditions, the spectral projector $e_\mu(f(u))$ is equal to the projector $e_H(u)$ associated with $u$ and H. One has

$$
N_\mu(f(u)) =\bigoplus_{\lambda\in H}N_{\lambda}(u),I_\mu(f(u)) =\bigcap_{\lambda\in H}I_{\lambda}(u)
$$

and the spectral multiplicity of $\mu$ for $f(u)$ is the sum of the spectral multiplicities of the elements of H, that is to say

$$
m_\mu(f(u)) =\sum_{\lambda\in H}m_{\lambda}(u)
$$

The complex number $\mu$ belong to $f$(Sp($u$)), and hence to the spectrum of $f(u)$ (Prop. 8 of I, p. 75), if and only if H is nonempty. One then has $e_\mu(f(u)) =e_H(u)$ (No. $1$ of I, p. 127). The other assertions are deduced from this by Prop. 2.

#### Example 1 {#ts-iii-s6-n1-exa-1 .statement tag=02UK}

Let E be a finite-dimensional vector space and $u$ an endomorphism of E. The spectrum of $u$ is finite and coincides with Sp$_s(u)$. Its elements are the roots of the characteristic polynomial $\chi_u$ of $u$; they are the eigenvalues of $u$. The spectral multiplicity $m_{\lambda}(u)$ of an element $\lambda \in$ Sp($u$) is the multiplicity of $\lambda$ as a root of the polynomial $\chi_u$ (A, VII, p. 36, cor.). By Corollary 2 above, one has

$$
\chi_{f(u)}(T) =\prod_{\lambda\in Sp(u)}(T-f(\lambda ))^{m_{\lambda}}
$$

for every $f\in \mathscr{O}$(Sp($u$)). This generalizes Prop. 10 of A, VII, p. 36.

#### Example 2 {#ts-iii-s6-n1-exa-2 .statement tag=02UL}

Let X be a compact subset of $\mathbf{C}$, and $\mathscr{C}(X)$ the Banach space of continuous complex-valued functions on X. Let $u$ denote the endomorphism of $\mathscr{C}(X)$ which to $f\in \mathscr{C}(X)$ associates the function $z\mapsto zf(z)$ of $\mathscr{C}(X)$. The spectrum of $u$ is equal to X, its points of the discrete spectrum are the isolated points of X, and their spectral multiplicities are equal to 1.

### 2. A partition of the spectrum

Let $\overline{\mathbf{Z}}$ denote the subset $\mathbf{Z}\cup  \{-\infty ,+\infty \}$ of $\overline{\mathbf{R}}$. If $u$ is a linear mapping whose kernel or cokernel is of finite dimension, the index of $u$ is the element ind($u$) of $\overline{\mathbf{Z}}$ defined by

ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$)

(cf. No$^o6$ of III, p. 67).

#### Definition 3 {#ts-iii-s6-def-3 .statement tag=02UM}

Let E be a complete normable space and $u$ an endomorphism of E. For every $n\in \overline{\mathbf{Z}}$, denote by Sp$_n(u)$ the set of complex numbers $\lambda \in$ Sp$_e(u)$ such that $u-\lambda 1_E$ is a strict morphism whose kernel or cokernel is of finite dimension, and whose index is $n$. Denote by Sp$_{\omega}(u)$ the complement in Sp$_e(u)$ of the union of the subsets Sp$_n(u)$ for $n\in \mathbf{Z}$.

The sets Sp$_s(u)$, Sp$_n(u)$ for $n\in \overline{\mathbf{Z}}$, and Sp$_{\omega}(u)$ form a partition of the spectrum of $u$.

Every endomorphism of E whose cokernel is of finite dimension is strict (III, p. 52, Lemma 6). The Fredholm endomorphisms of E are the endomorphisms of E whose kernel and cokernel are of finite dimension (III, p. 52, Prop. 11). The set $\mathbf{C}-$ Sp$_e(u)$ consists of the $\lambda \in \mathbf{C}$ such that $u-\lambda 1_E$ is a Riesz endomorphism of E, and such an endomorphism is a Fredholm endomorphism of E of index 0.

Consequently, for $\lambda \in \mathbf{C}$ and for $n\in \mathbf{Z}-\{0\}$, we have:

$\lambda \in \mathbf{C}-$ Sp($u$)$\Leftarrow \Rightarrow u-\lambda 1_E$ is an automorphism ;

$\lambda \in$ Sp$_s(u)\Leftarrow \Rightarrow u-\lambda 1_E$ is a Riesz endomorphism, but

is not an automorphism ;

$\lambda \in$ Sp$_0(u)\Leftarrow \Rightarrow u-\lambda 1_E$ is a Fredholm endomorphism

of index 0 of E but is not a Riesz endomorphism of E ;

$\lambda \in$ Sp$_n(u)\Leftarrow \Rightarrow u-\lambda 1_E$ is a Fredholm endomorphism

$(n\not = 0)$ of index $n$ of E ;

$\lambda \in$ Sp$_{-\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ is strict, its kernel is of dimension

infinite and its cokernel is of finite dimension ; $\lambda \in$ Sp$_{+\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ is strict, its kernel is of dimension

finite and its cokernel is of dimension infinite ; $\lambda \in$ Sp$_{\omega}(u)\Leftarrow \Rightarrow$ either $u-\lambda 1_E$ is not strict, or its kernel

and its cokernel are of dimension infinite.

#### Remark {#ts-iii-s6-n2-rem-1 .statement tag=02UN}

Let $\pi$ denote the canonical homomorphism of $\mathscr{L}(E)$ onto the Calkin algebra $\mathscr{C}$alk(E) of E (cf. No. 4 of III, p. 75). The spectrum of $\pi (u)$ relative to the algebra $\mathscr{C}$alk(E) is sometimes called the stable spectrum of $u$. Its elements are the complex numbers $\lambda$ such that $u-\lambda 1_E$ is not a Fredholm endomorphism of E (cor. 1 of theorem 3 of III, p. 73). It is therefore equal to Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$.

Let A be the set of endomorphisms of E which commute with $u$. The closure B of $\pi (A)$ in $\mathscr{C}$alk(E) is a complete normable algebra and the spectrum of $\pi (u)$ relative to B is the essential spectrum Sp$_e(u)$ of $u$ (III, p. 77, prop. 3). By the cor. of prop. 6 of I, p. 28, applied to the subalgebra B of $\mathscr{C}$alk(E), the set Sp$_e(u)$ is the union of Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$ and of certain bounded connected components of its complement.

#### Theorem 1 {#ts-iii-s6-thm-1 .statement tag=02UO}

Let E be a complete normable space and $u$ an endomorphism of E.

a) The set Sp$_{\omega}(u)$ is compact. It is non-empty if E is infinite-dimensional;

b) Let $n\in \overline{\mathbf{Z}}$. The set Sp$_n(u)$ is the union of a family of bounded connected components of $\mathbf{C}-$ Sp$_{\omega}(u)$. It is open in $\mathbf{C}$, and its boundary in $\mathbf{C}$ is contained in Sp$_{\omega}(u)$.

The set $\mathbf{C}-$ Sp$_{\omega}(u)$ consists of the complex numbers $\lambda \in \mathbf{C}$ such that $u-\lambda 1_E$ is a strict morphism, whose kernel or cokernel has finite dimension. By props. 11 of III, p. 67 and 13 of III, p. 70, it is open. The set Sp$_{\omega}(u)$ is therefore closed. Since it is bounded, it is compact.

Let us prove b). Let $n\in \overline{\mathbf{Z}}$. The set Sp$_n(u)$ is contained in $\mathbf{C}-$Sp$_{\omega}(u)$. Let U be a connected component of $\mathbf{C}-$ Sp$_{\omega}(u)$ which meets Sp$_n(u)$. The mapping $\lambda \mapsto$ ind($u-\lambda 1_E$) from $\mathbf{C}-$ Sp$_{\omega}(u)$ into $\overline{\mathbf{Z}}$ being locally constant (cor. 1 of prop. 12 of III, p. 68 and cor. 1 of prop. 13 of III, p. 70), the index of $u-\lambda 1_E$ is equal to $n$ for every $\lambda \in U$. If $n\not = 0$, this implies that U is contained in Sp$_n(u)$. If $n= 0$, remark that the set U is a connected component of $\mathbf{C}-$ (Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$). Since U meets Sp$_0(u)$ and hence Sp$_e(u)$, it follows then from Remark 2 that the set U is contained in Sp$_e(u)$, and consequently in Sp$_0(u)$. In all cases we conclude that Sp$_n(u)$ is the union of the connected components of $\mathbf{C}-$ Sp$_{\omega}(u)$ which meet Sp$_n(u)$. These are necessarily bounded since the set Sp($u$) is bounded. Consequently, Sp$_n(u)$ is open in $\mathbf{C}$ and its boundary is contained in Sp$_{\omega}(u)$. This proves b).

Suppose finally that the set Sp$_{\omega}(u)$ is empty. According to b), each of the sets Sp$_n(u)$, for $n\in \overline{\mathbf{Z}}$, is then empty. We therefore have Sp($u$) $=$ Sp$_s(u)$. The spectrum of $u$ is consequently discrete and compact, hence finite, and since all its points are of finite spectral multiplicity, the vector space E is finite-dimensional (III, p. 83, prop. 2). This completes the proof of a).

#### Corollary {#ts-iii-s6-n2-cor-1 .statement tag=02UP}

a) Let Ω be the unbounded connected component of $\mathbf{C}-$ Sp$_{\omega}(u)$. We have $\Omega \cap$ Sp($u$)$\subset$ Sp$_s(u)$;

b) Any point adherent to Sp$_s(u)$ which does not belong to Sp$_s(u)$ belongs to Sp$_{\omega}(u)$.

Assertion a) is a direct consequence of assertion b) of th. 1. Let $\lambda$ be a point adherent to Sp$_s(u)$ which does not belong to Sp$_s(u)$. It belongs to the spectrum of $u$, since the latter is closed. It does not belong to any of the sets Sp$_n(u)$, for $n\in \overline{\mathbf{Z}}$, since these are open (loc. cit.) and disjoint from Sp$_s(u)$. We therefore have $\lambda \in$ Sp$_{\omega}(u)$, whence b).

#### Proposition 3 {#ts-iii-s6-prop-3 .statement tag=02UQ}

Let E and F be complete normed spaces, $u: E\rightarrow F$ and $v: F\rightarrow E$ continuous linear mappings.

a) The traces on $\mathbf{C}-\{0\}$ of the sets Sp($v\circ u$) and Sp($u\circ v$) $($resp. Sp$_s(v\circ u)$ and Sp$_s(u\circ v)$, resp. Sp$_n(v\circ u)$ and Sp$_n(u\circ v)$ for $n\in \overline{\mathbf{Z}}$, resp. Sp$_{\omega}(v\circ u)$ and Sp$_{\omega}(u\circ v))$ are equal;

b) Let $\lambda$ be an element of Sp$_s(v\circ u)$ distinct from 0. The spectral multiplicities of $\lambda$ for $v\circ u$ and for $u\circ v$ are equal.

Let $\mu$ be a nonzero complex number and let $n\in \overline{\mathbf{Z}}$. In order that $\mu1_E-v\circ u$ be an automorphism (resp. a Riesz endomorphism, resp. a strict morphism whose kernel or cokernel is of finite dimension and whose index is $n$), it is necessary and sufficient that $\mu1_F-u\circ v$ be one (III, p. 49, prop. 10). Assertion a) then follows from the definitions.

Let $\lambda$ be a point of Sp$_s(v\circ u)$ distinct from 0. One has

dim Ker(($\lambda 1_E-v\circ u$)$^n$) $=$ dim Ker(($\lambda 1_F-u\circ v$)$^n$)

for every $n\geqslant 0 ($loc. cit.), therefore the spectral multiplicities of $\lambda$ for $v\circ u$ and $u\circ v$ are equal.

### 3. Spectrum of the transpose of an endomorphism

#### Proposition 4 {#ts-iii-s6-prop-4 .statement tag=02UR}

Let E be a complete normed space, $E'$ the dual space of E and $u$ an endomorphism of E.

a) One has Sp$_s(u) =$ Sp$_s(^tu)$, Sp$_n(u) =$ Sp$_{-n}(^tu)$ for every $n\in \overline{\mathbf{Z}}$ and Sp$_{\omega}(u) = Sp_{\omega}(^tu)$;

b) Every point of Sp$_s(u)$ has the same spectral multiplicity for $u$ and for $^tu$.

Assertion a) of prop. 3 of I, p. 131 proves that Sp($u$) $=$ Sp($^tu$), and assertion c) of loc. cit. implies that Sp$_s(u) =$ Sp$_s(^tu)$ and that assertion b) is valid.

For every $\lambda \in \mathbf{C}$, lemma 4 of III, p. 69 implies that $u-\lambda 1_E$ is a strict morphism if and only if $^tu-\lambda 1_{E'}$ is one, and that

dim Coker($^t(u-\lambda 1_E)$) $=$ dim Ker($u-\lambda 1_E$)

dim Ker($^t(u-\lambda 1_E)$) $=$ dim Coker($u-\lambda 1_E$)

in $\overline{\mathbf{Z}}$. Assertion a) follows from this, taking account of the definitions of the various parts of the spectrum (def. 3 of III, p. 85).

### 4. Perturbation by a compact operator

#### Theorem 2 {#ts-iii-s6-thm-2 .statement tag=02US}

Let E be a complete normable space, $u$ an endomorphism of E and $h$ a compact endomorphism of E. One has Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ and Sp$_n(u+h) =$ Sp$_n(u)$ for every $n\in \overline{\mathbf{Z}}-\{0\}$.

Let $\lambda \in \mathbf{C}$. In order that $u+h-\lambda 1_E$ be a strict morphism whose kernel (resp. cokernel) is of finite dimension, it is necessary and sufficient that $u-\lambda 1_E$ be so, by Theorem 1 of III, p. 72 (resp. Theorem 2 of III, p. 73).

The equalities

Sp$_{-\infty}(u+h) =$ Sp$_{-\infty}(u)$, Sp$_{+\infty}(u+h) =$ Sp$_{+\infty}(u)$,

Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$

follow from this. Moreover, one has Sp$_n(u+h) =$ Sp$_n(u)$ by Theorem 3 of III, p. 73 for every $n\in \mathbf{Z}-\{0\}$.

#### Corollary {#ts-iii-s6-n4-cor-1 .statement tag=02UT}

Suppose that the unbounded connected component of the complement of Sp$_{\omega}(u)$ contains 0. Then $u+h$ is a Riesz endomorphism of E.

One has Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ (Theorem 2), hence 0 belong to the unbounded connected component of $\mathbf{C}-$ Sp$_{\omega}(u+h)$. By the corollary to Theorem 1 of III, p. 87, either 0 does not belong to the spectrum of $u+h$, or else it is a sensitive point of this spectrum. In both cases, $u+h$ is a Riesz endomorphism of E.

### 5. Spectrum of a compact operator

#### Lemma 1 {#ts-iii-s6-lem-1 .statement tag=02UU}

Let E be a separated topological vector space of dimension $\geqslant 2$ over $\mathbf{R}$, and let X be a denumerable subset of E. The complementary set E - X is connected.

Suppose first that E is of dimension 2. One may suppose that $E =\mathbf{R}^2$ endowed with the euclidean norm (TVS, I, p. 14, Theorem 2). Since X is denumerable, there exists a real number $r\in \mathbf{R}_+^*$ such that the circle C with center 0 and radius $r$ does not meet X. Let $x\in E$ - X; if $x \notin C$, there exists a point $y\in C$ such that the straight line $L_x$ joining $x$ and $y$ does not meet X, since X is denumerable. The set E - X is the union of C, which is connected, and of the connected sets $L_x\cup C$ for $x\in E$- $(X\cup C)$; these sets all contain C, and therefore E- X is connected (TG, I, p. 81, Proposition 2).

Consider the general case. Replacing X by $X-x$ for an element $x\in E$ - X, one is reduced to the case where $0\notin X$. Since E - X is the union of the sets F - $(X\cap F)$ when F runs through the set of 2-dimensional subspaces of E, and since these are connected by the preceding case and contain 0, the set E - X is connected (loc. cit.).

#### Lemma 2 {#ts-iii-s6-lem-2 .statement tag=02UV}

Let $S\subset \mathbf{C}$ be an infinite, discrete, bounded and closed set in $\mathbf{C}-\{0\}$. Then S is the set of values of a sequence $(\lambda_n)_{n\in\mathbf{N}}$ of non-zero complex numbers, pairwise distinct, such that the sequence $(|\lambda_n|)_{n\in\mathbf{N}}$ is decreasing and converges to 0.

For every integer $i\geqslant 1$, the set $A_i$ of complex numbers $\lambda \in S$ such that $|\lambda |\geqslant \frac{1}{i}$ is compact and discrete in $\mathbf{C}$, hence finite. Let $a_i$ be its cardinal. Since S is infinite, the sequence $(a_i)$ tends to $+\infty$. Put $A_0=\emptyset$ and $a_0= 0$. For every $i\geqslant 1$, choose a bijection $n\mapsto \lambda_n$ of the interval $[a_{i-1}, a_i[$ of $\mathbf{N}$ onto $A_i-A_{i-1}$ such that the mapping $n\mapsto  |\lambda_n|$ is decreasing on $[a_{i-1}, a_i[$. The sequence $(\lambda_n)_{n\in\mathbf{N}}$ satisfies the required properties.

Let E be a complete normable space of infinite dimension. The algebra $\mathscr{L}^c(E)$ is a non-unital subalgebra of $\mathscr{L}(E)$. Recall that for every compact endomorphism $u\in \mathscr{L}^c$(E), the spectrum Sp$'_{\mathscr{L}^c(E)}(u)$ is the spectrum of $u$ relative to the unital subalgebra $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ of $\mathscr{L}(E) ($I, p. 4, No.$^o4$).

#### Proposition 5 {#ts-iii-s6-prop-5 .statement tag=02UW}

Let E be a complete normable space and let $u$ be a compact endomorphism of E. Every element of Sp$_s(u)$ is an eigenvalue of finite spectral multiplicity. Moreover:

a) If E is finite-dimensional, then Sp($u$) $=$ Sp$_s(u)$;

b) If E is infinite-dimensional, then Sp$_s(u) =$ Sp($u$)$-\{0\}$ and Sp$_{\omega}(u) =\{0\}$;

c) If Sp$_s(u)$ is infinite, it is the set of values of a sequence $(\lambda_n)_{n\in\mathbf{N}}$ of nonzero complex numbers, pairwise distinct, such that the sequence $(|\lambda_n|)_{n\in\mathbf{N}}$ is decreasing and converges to 0 ;

d) If E is infinite-dimensional, then Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

Every element of Sp$_s(u)$ is an eigenvalue of finite spectral multiplicity (prop. 1 of III, p. 83).

Assertion a) is elementary (III, p. 85, example 1). Suppose now that E is infinite-dimensional.

Let $\lambda \in$ Sp($u$)$-\{0\}$. Then $u-\lambda 1_E$ is a Riesz endomorphism of E (cor. 2 of prop. 2 of III, p. 75), hence $\lambda$ belongs to Sp$_s(u)$. If E is infinite-dimensional, then Sp$_{\omega}(u)$ is not empty (III, p. 87, th. 1, a)). Necessarily one has Sp$_{\omega}(u) =\{0\}$, whence b).

The set Sp$_s(u)$ is discrete and bounded. Moreover, one has Sp$_s(u) =$ Sp($u$)$\cap (\mathbf{C}-\{0\})$ by b), hence Sp$_s(u)$ is closed in $\mathbf{C}-\{0\}$. Assertion c) therefore follows from Lemma 2.

The spectrum of $u$ is denumerable, and its complement in $\mathbf{C}$ is therefore connected (lemma 1). By the cor. to prop. 6 of I, p. 28, applied to the unital subalgebra $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ of $\mathscr{L}$ (E), one concludes that Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

#### Proposition 6 {#ts-iii-s6-prop-6 .statement tag=02UX}

Let E be a complete normed space over $\mathbf{C}$ and $u$ a compact endomorphism of E.

a) Let $f\in \mathscr{O}$(Sp($u$)) be such that $f(0) = 0$. The endomorphism $f(u)$ is compact;

b) Suppose that E is a complex Hilbert space and that $u$ is normal. Let $f$ be a continuous function on Sp($u$) such that $f(0) = 0$. The normal endomorphism $f(u)$ is compact.

Moreover, the converse assertions are valid if E is infinite-dimensional, and the condition $f(0) = 0$ is not necessary if E is finite-dimensional.

We may suppose that E is infinite-dimensional.

Let us prove a) and its converse. The endomorphism $u$ is an element of the Banach algebra $\mathscr{L}^c(E)$. Since E is infinite-dimensional, one has the equality Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$ by prop. 5, d). The element $f(u)$ of the holomorphic functional calculus of the unital Banach algebra deduced from $\mathscr{L}^c(E)$ by adjunction of a unit element belongs to $\mathscr{L}^c(E)$ if and only if $f(0) = 0$ (I, p. 88). But moreover this element coincides with the element $f(u)$ of $\mathscr{L}(E)$ (prop. 7 of I, p. 75), hence $f(u)$ is compact if and only if $f(0) = 0$.

The proof of assertion b) and of its converse is exactly the same if one considers the continuous functional calculus of the involutive algebra $\mathscr{L}^c(E)$ (I, p. 110, def. 5).

#### Corollary {#ts-iii-s6-n5-cor-1 .statement tag=02UY}

Let E and F be Hilbert spaces and let $u$ be a continuous linear mapping from E into F. The linear mapping $u$ is compact if and only if the endomorphism $|u|$ of E is compact.

Let $(j,|u|)$ be the polar decomposition of $u$ (def. 4 of I, p. 140). Since

$$
\surd
$$

$u=j|u|$ and $|u|=u^*u$ (prop. 10 of I, p. 139), the equivalence results from prop. 3 of III, p. 5 and assertion b) of the preceding proposition.

### 6. Case of Hilbert spaces

In this No., E denotes a Hilbert space over $\mathbf{C}$. We denote by $\pi$ the canonical homomorphism of $\mathscr{L}(E)$ onto the involutive algebra $\mathscr{C}$alk(E).

#### Proposition 7 {#ts-iii-s6-prop-7 .statement tag=02UZ}

Let $u\in \mathscr{L}(E)$.

a) If $u$ is normal, then $u$ is a Riesz endomorphism if and only if $u$ is a Fredholm endomorphism of index 0.

b) If $u$ is hermitian, then $u$ is a Fredholm endomorphism if and only if $u$ is a Riesz endomorphism.

Every Riesz endomorphism is a Fredholm endomorphism of index 0 (proposition 5 of III, p. 46). Conversely, suppose that $u$ is a Fredholm endomorphism of index 0, and that $u$ is normal. Its nilspace then coincides with its kernel (EVT, V, p. 43, prop. 8), and is therefore of finite dimension. It then results from lemma 2 of III, p. 45 and from the definition that $u$ is a Riesz endomorphism.

Let us prove b). By a), it is enough to verify that the index of a hermitian Fredholm endomorphism $u$ is zero. But the orthogonal complement of the image of $u$ (which is closed) is then equal to the kernel of $u$ (EVT, V, p. 41, prop. 4), whence the assertion.

#### Corollary {#ts-iii-s6-n6-cor-1 .statement tag=02V0}

Let $u\in \mathscr{L}(E)$. If $u$ is normal, then Sp$_0(u)$ is empty, and if $u$ is hermitian, then Sp$_e(u)$ coincides with the spectrum of $\pi (u)$ relative to the algebra $\mathscr{C}$alk(E).

Both assertions result from the proposition and from the definition of the sets Sp$_n(u)$ for $n\in \overline{\mathbf{Z}}$ and of Sp$_{\omega}(u)$, which form a partition of the essential spectrum of $u$ (def. 2 of III, p. 83).

#### Theorem 3 (Weyl) {#ts-iii-s6-thm-3 .statement tag=02V1}

Let $u\in \mathscr{L}(E)$ be a normal endomorphism of $u$. The essential spectrum of $u$ is the intersection of the sets Sp($u+h$), where $h$ ranges over $\mathscr{L}^c(E)$.

Let $h\in \mathscr{L}^c(E)$. Since Sp$_0(u)$ is empty (corollary above), Theorem 2 of III, p. 89 implies that Sp$_e(u+h) =$ Sp$_e(u)$. The intersection of the sets Sp($u+h$) therefore contains Sp$_e(u)$.

Let $\lambda \in$ Sp$_s(u)$. Let $E_{\lambda}$ denote the proper subspace of $u$ relative to $\lambda$, and $F_{\lambda}$ the image of the spectral projector associated with $u$ and $\mathbf{C}-\{\lambda \}$. The space E is the topological direct sum of $E_{\lambda}$ and $F_{\lambda}$. Let $h$ be the finite-rank endomorphism of E which is zero on $F_{\lambda}$ and coincides on $E_{\lambda}$ with the identity. The endomorphism $u+h$ is invertible, therefore $\lambda  \notin$ Sp($u+h$). The theorem follows.

Thus, if $u$ is a normal endomorphism of E, and if $h\in \mathscr{L}^c$(E), the spectrum of $u+h$ can differ from the spectrum of $u$ only by isolated points having finite spectral multiplicity.

### 7. The Krein-Rutman theorem

#### Lemma 3 {#ts-iii-s6-lem-3 .statement tag=02V2}

Let $(a_n)_{n\geqslant 0}$ be a sequence of positive real numbers such that the power series

$$
f(z) =\sum_{n\geqslant 0}a_nz^n
$$

has a finite radius of convergence $r >0$. Let $D\subset \mathbf{C}$ be the open disc with center 0 and radius $r$. There does not exist a holomorphic function $\widetilde{f}$ defined on an open neighbourhood U of $r$ in $\mathbf{C}$ which coincides with $f$ on $U\cap D$.

Suppose there exists such a holomorphic function $\widetilde{f}$ defined on an open neighbourhood U of $r$. There exist real numbers $s < r$ and $\delta  >0$ such that $s+\delta  > r$ and such that the open disk $D'$ with center $s$ and radius $\delta$ is contained in U. The power series expansion of $\widetilde{f}$ at the point $s$ (VAR, R1, p. 26, 3.2.1) then converges for every $z$ in the disk with center 0 and radius $\delta$ (VAR, R1, p. 29, 3.3.4). This series is

$+\infty (n)+\infty (n)$

$\widetilde{f}_s(z) =\sum\widetilde{f}n$!$(s)z^n=\sum fn$!$(s)z^n$

$n=0n=0$ (VAR, R1, p. 27, 3.2.4). Since $s\in D$, we have

$$
f^{(n)}(s) =\sum_{k=n}^{+\infty}k(k-1)\cdots (k-n+ 1)a_ks^{k-n}
$$

(VAR, R1, p. 28, 3.2.11). Let us take $z$ such that $0< z < \delta$. Since $a_k\geqslant 0$, we have

$\widetilde{f}_s(z) =\sum^{+\infty}(\sum^{+\infty}k(k-1)\cdots n($!$k-n+ 1)a_ks^{k-n})z^n$

$n=0k=n$ $+\infty k+\infty$

$=\sum(a_k\sum n$!($kk-$! $n$)! $s^{k-n}z^n)=\sum a_k(s+z)^k$

$k=0n=0k=0$

(TG, III, p. 40). When $s+z > r$, the convergence of this expression contradicts the assumption that the radius of convergence of the power series $f$ is equal to $r$.

Let E be a real Banach space. Let C be a pointed convex cone in E. The vector space generated by C is equal to $C-C$ (EVT, II, p. 12, cor. 1). In particular, the cone C is total in E if and only if $C-C$ is dense in E. Recall that C is said to be salient if $C\cap (-C)$ is reduced to 0 (EVT, II, p. 11).

The polar $C^{\circ}$ of C is the set of continuous linear forms $\ell \in E'$ such that $\ell (x)\geqslant 0$ for all $x\in C$ (EVT, II, p. 47, prop. 4). By the bipolar theorem (EVT, II, p. 48, th. 1), if C is a closed pointed convex cone, one has $C^{\circ \circ}= C$.

#### Lemma 4 {#ts-iii-s6-lem-4 .statement tag=02V3}

Let E be a real Banach space and $u\in \mathscr{L}(E_{(\mathbf{C})})$ a nonzero endomorphism of $E_{(\mathbf{C})}$. Let C be a total convex cone in E. There exists $x\in C$ such that $u(x)\not = 0$.

Indeed, if $u$ vanishes on C, then $u$ vanishes on $C-C$, hence on E, and therefore on $E_{(\mathbf{C})}$.

#### Theorem 4 (Krein–Rutman) {#ts-iii-s6-thm-4 .statement tag=02V4}

Let E be a complete normed space over $\mathbf{R}$. Let C be a closed total salient convex cone in E and let $u\in \mathscr{L}(E)$ be a compact linear mapping such that $u(C)\subset C$. If the spectral radius $\varrho (u)$ is $>0$, then $\varrho (u)$ is an isolated point of the spectrum of $u$, and there exists a nonzero eigenvector $x\in C$ of $u$ for the eigenvalue $\varrho (u)$.

Let $E_{(\mathbf{C})}$ be the complexified space of E and $u_{(\mathbf{C})}$ the endomorphism of $E_{(\mathbf{C})}$ obtained by extension of the scalars from $u$. The spectral radius of $u_{(\mathbf{C})}$ is equal to $\varrho (u) ($I, p. 86); we denote it simply by $\varrho$. Since $\varrho  >0$, the complex spectrum of $u$ is not reduced to 0. There therefore exists $\lambda_0\in$ Sp$_s(u_{(\mathbf{C})})$ such that $|\lambda_0|=\varrho$ (Prop. 5 of III, p. 90). Let $e_0$ be the spectral projector of $u_{(\mathbf{C})}$ associated with $\lambda_0$.

The resolvent $\lambda \mapsto R(u_{(\mathbf{C})}, \lambda ) = (\lambda -u_{(\mathbf{C})})^{-1}$ is holomorphic on the complement of the spectrum of $u_{(\mathbf{C})}$ (Theorem 1 of I, p. 24). The complex number $\lambda_0$ is a pole of the resolvent and its residue is the spectral projector $e_0($I, p. 131).

Let $y$ and $y'$ be elements of E such that $y+iy'\in E_{(\mathbf{C})}$ is an eigenvector of $u_{(\mathbf{C})}$ for the eigenvalue $\lambda_0$. Since $e_0(y+iy') =y+iy'\not = 0$, there exists an element $x_0\in C$ such that $e_0(x_0)\not = 0$ (Lemma 4). Since C is closed and salient, its polar $C^{\circ}$ is total (EVT, II, p. 48, Corollary 1), and there then exists a linear form $\ell_0\in C^{\circ}$ such that $\langle e_0(x_0), \ell_0\rangle  \not = 0$.

Consider the function $f$ defined by $f(0) = 0$ and by

$$
f(z) =\langle R(u_{(\mathbf{C})}, z^{-1})x_0, \ell_0\rangle
$$

for $z\in \mathbf{C}$ such that $z^{-1}\notin$ Sp($u_{(\mathbf{C})}$). This function satisfies

$$
f(z) =\ell_0((\sum^{+\infty}_{n=0}z^{n+1}u^n_{(\mathbf{C})})x_0)=\sum_{n=0}^{\infty}\langle u^n(x_0), \ell_0\rangle z^{n+1} \tag{1}
$$

for $|z|<1/\varrho$ (Theorem 1 of I, p. 24, d)) and is therefore holomorphic in the disc with centre 0 and radius $1/\varrho$.

There exists a holomorphic function $\widetilde{R}$ defined on an open neighbourhood U of $\lambda_0$ and with values in $\mathscr{L}(E)$ such that for $z$ belonging to U$-\{\lambda_0\}$, one has

$$
R(u_{(\mathbf{C})}, z) =\widetilde{R}(z) +\sum_{n=0}^{+\infty}(z-\lambda_0)^{-n-1}(u_{(\mathbf{C})}-\lambda_0)^ne_0
$$

(Prop. 17 of I, p. 83). For $z$ such that $z^{-1}\in U$ and $z\not = 1/\lambda_0$, one therefore has

$$
f(z) =\langle \widetilde{R}(z^{-1})x_0, \ell_0\rangle +\sum_{n=0}^{+\infty}(z^{-1}-\lambda_0)^{-n-1}\langle (u_{(\mathbf{C})}-\lambda_0)^ne_0(x_0), \ell_0\rangle
$$

The term of the series corresponding to $n= 0$ is $(z^{-1}-\lambda_0)^{-1}\langle e_0(x_0), \ell_0\rangle$. Since $\langle e_0(x_0), \ell_0\rangle  \not = 0$, the uniqueness of the Laurent expansion (VAR, R1, p. 30, 3.3.9) implies that $f$ cannot be prolonged to a holomorphic function in a neighbourhood of $1/\lambda_0$. In particular, the radius of convergence of the power series expansion (1) of the function $f$ at the point 0 is equal to $1/\varrho$.

The coefficients of the power series (1) are $\langle u^n(x_0), \ell_0\rangle \geqslant 0$ since $u(C)\subset C$ and $\ell_0\in C^{\circ}$. By Lemma 3, the function $f$ cannot be extended to a holomorphic function in a neighbourhood of $1/\varrho$. The resolvent of $u_{(\mathbf{C})}$ therefore cannot be extended to a holomorphic function in a neighbourhood of $\varrho$, that is to say, $\varrho \in$ Sp($u$). This implies that $\varrho$ is an eigenvalue of $u_{(\mathbf{C})}$ (prop. 5 of III, p. 90). Since $\varrho$ is real, it is also an eigenvalue of $u$.

Let $d\geqslant 1$ be the order of the pole of the resolvent of $u_{(\mathbf{C})}$ at $\varrho$. Let $e$ be the endomorphism

$e=$ lim$_{z\rightarrow\varrho}(z-\varrho )^dR(u_{(\mathbf{C})}, z)$.

It is nonzero and commutes with $u_{(\mathbf{C})}$, and its image is contained in the eigenspace of $u_{(\mathbf{C})}$ corresponding to $\varrho ($cf. No.$^o3$ of I, p. 131). Let now $\ell$ be an element of $C^{\circ}$ and $x$ an element of C. By Theorem 1 of I, p. 24, d), one has

$\langle e(x), \ell \rangle =$ lim$_{zz>\varrho\rightarrow\varrho}(z-\varrho )^d\sum_{n\geqslant 0}\langle u^n(x), \ell \rangle z^{-n-1}\geqslant 0$.

The bipolar theorem (EVT, II, p 48, th. 1) implies that $e(x)\in C$ for all $x\in C$. Since C is total, there exists $x\in C$ such that $e(x)\not = 0$ (Lemma 4), and then $e(x)$ belongs to C and is an eigenvector of $u$ for the eigenvalue $\varrho$, as required.

#### Corollary {#ts-iii-s6-n7-cor-1 .statement tag=02V5}

Let E be a complete normable space over $\mathbf{R}$. Let C be a total salient closed convex cone in E and $u\in \mathscr{L}(E)$ a compact linear mapping such that $u(C)\subset C$. If the spectral radius $\varrho (u)$ of $u$ is $>0$, then $\varrho (^tu) =\varrho (u)$ is an eigenvalue of $^tu$, and $^tu$ admits an eigenvector corresponding to $\varrho (u)$ in $C^{\circ}$.

One has $\varrho (^tu) =\varrho (u)$ (prop. 3 of I, p. 131). By Corollary 1 of III, p. 9, the endomorphism $^tu$ of $E'$ is compact. Moreover, one has $^tu(C^{\circ})\subset C^{\circ}$; the assertion then follows from the Krein-Rutman theorem applied to $^tu$, and to the closed convex cone $C^{\circ}$, since the latter is salient (because C is total) and total (because C is salient).

#### Remark {#ts-iii-s6-n7-rem-1 .statement tag=02V6}

The assumption $\varrho (u)>0$ cannot in general be omitted in the Krein-Rutman theorem. For example, let V be the endomorphism of the Banach space $\mathscr{C}([0,1])$ defined by

$$
V(f)(x) =\int_0^xf(y)dy
$$

for $f\in \mathscr{C}([0,1])$. The mapping V is compact and its spectral radius is zero (Exercise 1 of I, p. 187). It preserves the total salient closed convex cone in $\mathscr{C}([0,1])$ formed by the positive functions, and has no eigenvalue (loc. cit.).

The following proposition describes a sufficient condition for an endomorphism preserving a cone to have a strictly positive spectral radius, and then sharpens the Krein-Rutman theorem.

#### Proposition 8 {#ts-iii-s6-prop-8 .statement tag=02V7}

Let E be a nonzero complete normable space over $\mathbf{R}$. Let C be a closed salient convex cone with nonempty interior $\mathring{C}$ in E, and let $u\in \mathscr{L}(E)$ be a compact linear mapping such that $u(C-\{0\})\subset \mathring{C}$.

a) One has $\varrho (u)>0$ and there exists an eigenvector $x_0$ of $u$ in $\mathring{C}$ for the eigenvalue $\varrho (u)$;

b) The spectral projector of $u$ corresponding to $\varrho (u)$ is of rank 1;

c) For every eigenvalue $\lambda \not =\varrho (u)$ of $u_{(\mathbf{C})}$, one has $|\lambda |< \varrho (u)$;

d) Let F be a subspace of E stable under $u$ such that (C $-\{0\}$)$\cap F$ is nonempty. Then $x_0\in F$. In particular, the only eigenvectors of $u$ in C are the multiples of $x_0$.

Let us prove two preliminary lemmas.

#### Lemma 5 {#ts-iii-s6-lem-5 .statement tag=02V8}

Let E be a real Banach space, C a convex cone in E, and $u\in \mathscr{L}(E)$ such that $u(C-\{0\})\subset \mathring{C}$. Let $\ell \in C^{\circ}$ be an eigenvector of $^tu$. Then the kernel of $\ell$ is stable under $u$ and does not meet C $-\{0\}$.

Let $\lambda \in \mathbf{R}$ be such that $^tu(\ell ) =\lambda \ell$. For every $x\in$ Ker($\ell$ ), one has

$$
\langle u(x), \ell \rangle =\langle x,^tu(\ell )\rangle =\lambda \langle x, \ell \rangle = 0
$$

therefore Ker($\ell$ ) is stable under $u$.

Let $x$ be a nonzero element of Ker($\ell$ ). For every element $y$ of E such that $\langle y, \ell \rangle <0$, one has $\langle u(x) +y, \ell \rangle <0$, whence it follows that $u(x) +$ $y \notin C$ since $\ell \in C^{\circ}$. It follows that $u(x)$ does not belong to $\mathring{C}$. Since $u(C-\{0\})\subset \mathring{C}$, this implies that $x \notin C$.

#### Lemma 6 {#ts-iii-s6-lem-6 .statement tag=02V9}

Let E be a finite-dimensional real vector space and B a compact convex neighbourhood of 0 in E. Let $u$ be an endomorphism of E such that $u(B)\subset \mathring{B}$. Then the complex spectrum of $u$ is contained in the unit disk of $\mathbf{C}$ and, in particular, does not meet the circle with center 0 and radius 1 in $\mathbf{C}$.

Replacing B by $B\cap (-B)$, we are reduced to the case where B is balanced. The gauge $p$ of B (EVT, II, p. 28, ex. 3) is then a norm on E, which defines its topology (EVT, I, p. 14, th. 2). The hypothesis implies that $p(u(x))< p(x)$ for every element $x$ of E $-\{0\}$, hence that the spectral radius of $u$ is $<1$; as this is also the spectral radius of $u_{(\mathbf{C})}($cf. I, p. 86), the conclusion follows.

Let us now prove the proposition.

Let us denote by $x\preccurlyeq y$ the order relation on E associated with the convex cone C (EVT, II, p. 13, n$^o5$), that is to say, $x\preccurlyeq y$ if and only if $y-x\in C$. We have $u(x)\preccurlyeq u(y)$ if $x\preccurlyeq y$. Since $\mathring{C}$ is nonempty, the vector space $C-C$ generated by C (EVT, II, p. 12, cor. 1) contains a neighbourhood of 0, therefore the cone C is total.

Let us prove assertion a). Let $\varrho =\varrho (u)$. Let $y_0$ be an element of $\mathring{C}$. We have $y_0\not = 0$. Let $r >0$ be such that the closed ball with center $y_0$ and radius $r$ is contained in C. For every $y\in E-\{0\}$, we have $y_0-r\|y\|^{-1}y\in C$, hence $y\preccurlyeq r^{-1}\|y\|y_0$ for every $y\in E$.

Since $y_0\not = 0$, the hypotheses imply that $u(y_0)\in \mathring{C}$. There therefore exists $t >0$ such that $tu(y_0)-y_0\in C$. Let us put $v=tu$. It is a compact endomorphism of E such that $v(C)\subset C$ and $v(y_0)\succcurlyeq y_0$. For every integer $n\geqslant 1$, we have

$$
y_0\preccurlyeq v^n(y_0)\preccurlyeq r^{-1}\|v^n(y_0)\|y_0\preccurlyeq r^{-1}\|v^n\| \|y_0\|y_0
$$

therefore $(r^{-1}\|v^n\|\|y_0\| -1)y_0\in C$. Since C is salient, this implies that $t^n\|u^n\|=\|v^n\|\geqslant r/\|y_0\|$, whence $\varrho \geqslant t^{-1}>0 ($I, p. 20, prop. 1).

By the Krein-Rutman theorem (th. 4), the real number $\varrho$ is an eigenvalue of $u$, and there exists an eigenvector $x_0$ of $u$ in C for the eigenvalue $\varrho$. We have $\varrho x_0=u(x_0)\in \mathring{C}$ by hypothesis, therefore $x_0\in \mathring{C}$. This proves assertion a).

Let K be the intersection of the spectrum of $u_{(\mathbf{C})}$ and of the circle with center 0 and radius $\varrho$ in $\mathbf{C}$. Since $u$ is compact and $\varrho  >0$, the set K is finite and the image of the spectral projector $e_K$ is a subspace of $E_{(\mathbf{C})}$ of finite dimension (prop. 2 of III, p. 83 and prop. 5 of III, p. 90). Since K is stable under complex conjugation, the image of $e_K$ is a subspace of $E_{(\mathbf{C})}$ rational over $\mathbf{R}$ (A, V, p.60, prop. 6) ; let F be the subspace of E such that $F_{(\mathbf{C})}$ is equal to the image of $e_K$. The space F is stable under $u$ and contains the eigenspace of $u$ corresponding to $\varrho$, therefore F is nonzero.

To prove assertions b) and c), it is enough to prove that F is of dimension 1.

Let $v$ denote the endomorphism of F deduced from $u$ by passing to subspaces. Let $C_F= C\cap F$. This is a closed salient convex cone with nonempty interior in F (since $x_0\in \mathring{C}\cap F$), hence total; it satisfies $v(C_F-\{0\})\subset \mathring{C}_F$, and in particular is stable under $v$. Since $\varrho (v)\leqslant \varrho$ and $x_0\in F$, we have $\varrho (v) =\varrho$. From the corollary to Theorem 4, applied to $C_F$ and $v$, there exists an eigenvector $\ell$ of $^tv$ in $C^{\circ}_F$ for the eigenvalue $\varrho (v) =\varrho  >0$.

The subspace Ker($\ell$ ) of F is stable under $v$. Let $w$ denote the endomorphism of Ker($\ell$ ) deduced from $\varrho^{-1}v$ by passing to subspaces; its spectrum is contained in the unit circle. The set B of the $y\in$ Ker($\ell$ ) such that $x_0+y\in C_F$ is a closed convex neighbourhood of 0 in Ker($\ell$ ). For every $y\in B$ and every $z\in$ Ker($\ell$ ), we have

$$
x_0+ (w(y) +z) =\varrho^{-1}(v(x_0+y) +\varrho z)
$$

which belongs to $C_F$ if the norm of $z$ is sufficiently small, hence $w(y)\in \mathring{B}$.

The set B is bounded: in fact, if there existed a sequence $(y_n)_{n\in\mathbf{N}}$ in Ker($\ell$ ) such that $\|y_n\| \rightarrow +\infty$ and $x_0+y_n\in C_F$ then, by passing to a subsequence if necessary, we should have $y_n/\|y_n\| \rightarrow y$ where $y\in$ Ker($\ell$ ) is nonzero, and $y=$ lim $\|y_n\|^{-1}(x_0+y_n)$ would belong to $C_F$, contrary to Lemma 5. Hence the set B is compact.

It then follows from Lemma 6, applied to Ker($\ell$ ), to B and to $w$, that the complex spectrum of $w$ does not meet the circle with center 0 and radius 1; this implies that the spectrum of $w$ is empty, which means that Ker($\ell$ ) is reduced to $\{0\}$, hence that F has dimension 1. Assertions b) and c) are thus established.

The linear mapping $^tu$ is compact (Corollary 1 of III, p. 9) and $^tu(C^{\circ})\subset C^{\circ}$; moreover $\varrho (^tu) =\varrho  >0$ (prop. 3 of I, p. 131). From the corollary to Theorem 4, there exists in $C^{\circ}$ an eigenvector $\ell \not = 0$ of $^tu$ for the eigenvalue $\varrho$. The kernel of $\ell$ is stable under $u$ and does not meet C $-\{0\}$ (Lemma 5). In particular, we have $x_0\notin$ Ker($\ell$ ).

Let F be a subspace of E stable under $u$. We have the decomposition $F = (F\cap \mathbf{R}x_0)\oplus (F\cap$ Ker($\ell$ )). If F does not contain $x_0$, we therefore have $F\subset$ Ker($\ell$ ), hence F does not meet C$-\{0\}$. This establishes d) and concludes the proof of the proposition.

#### Corollary {#ts-iii-s6-n7-cor-2 .statement tag=02VA}

Let E be a nonzero complete normable space over $\mathbf{R}$. Let C be a closed salient convex cone with nonempty interior $\mathring{C}$ in E, and let $u$ be a compact endomorphism of E such that $u(C)\subset C$. Suppose that there exists an integer $k\geqslant 1$ such that $u^k(C-\{0\})\subset \mathring{C}$.

a) One has $\varrho (u)>0$ and there exists an eigenvector $x_0$ of $u$ in $\mathring{C}$ for the eigenvalue $\varrho (u)$;

b) The spectral projector of $u$ corresponding to $\varrho (u)$ is of rank 1;

c) For every eigenvalue $\lambda \not =\varrho (u)$ of $u_{(\mathbf{C})}$, one has $|\lambda |< \varrho (u)$;

d) The only eigenvectors of $u$ in C are the multiples of $x_0$.

Put $\varrho =\varrho (u)$. We may apply Theorem 4 to $u$ and Proposition 8 to $u^k$. There therefore exists an eigenvector $x_0$ of $u$ in C for the eigenvalue $\varrho$. Since $0< \varrho (u^k) =\varrho^k$ (formula (4) of I, p. 21), we have in particular $\varrho  >0$, and since $x_0$ is an eigenvector of $u^k$ for the eigenvalue $\varrho (u^k)$, we have $x_0\in \mathring{C}$.

We have Sp($u^k_{(\mathbf{C})}$) $=$ Sp($u_{(\mathbf{C})}$)$^k$ (remark 4 of I, p. 2), hence every eigenvalue $\lambda \in \mathbf{C}$ of $u_{(\mathbf{C})}$ such that $|\lambda |=\varrho$ satisfies $\lambda^k=\varrho^k$, and since every eigenvector corresponding to $\lambda$ is an eigenvector of $u^k$ for $\varrho^k$, hence proportional to $x_0$, we have $\lambda =\varrho$.

If the spectral projector of $u$ for the eigenvalue $\varrho$ were of rank at least 2, the same would be true of that of $u^k$ for the eigenvalue $\varrho^k($cf. No.$^o2$ of I, p. 129).

Finally, if $x\in C$ is an eigenvector of $u$, it is also one for $u^k$, hence is proportional to $x_0$.

Let $n$ be an integer $\geqslant 1$. The set $\mathbf{R}_+^n$ is a closed pointed salient convex cone in $\mathbf{R}^n$, with nonempty interior equal to $(\mathbf{R}_+^*)^n$.

Let A $= (a_{i,j})$ be a real matrix of type $(n, n)$, and $u_A$ the endomorphism $x\mapsto Ax$ of $\mathbf{R}^n$. Let $\varrho =\varrho (u_A)$ be its spectral radius.

#### Lemma 7 {#ts-iii-s6-lem-7 .statement tag=02VB}

We have $u_A(\mathbf{R}^n_+)\subset \mathbf{R}_+^n$ if and only if $a_{i,j}\geqslant 0$ for all $i$ and $j$, and $u_A(\mathbf{R}^n_+-\{0\})\subset (\mathbf{R}_+^*)^n$ if and only if $a_{i,j}>0$ for all $i$ and $j$.

Let $(e_1, . . . , e_n)$ be the canonical basis of $\mathbf{R}^n$. The vectors $e_i$ belong to $\mathbf{R}_+^n$ and $u_A(e_i)\in \mathbf{R}_+^n$ for every $i$ (resp. $u_A(e_i)\in (\mathbf{R}_+^*)^n$ for every $i$) if and only if $a_{i,j}\geqslant 0$ for all $i$ and $j$ (resp. $a_{i,j}>0$ for all $i$ and $j$). The result follows by linearity.

#### Theorem 5 (Perron–Frobenius) {#ts-iii-s6-thm-5 .statement tag=02VC}

a) If $a_{i,j}\geqslant 0$ for all $i$ and $j$ in $\{1, . . . , n\}$, then the real number $\varrho$ is an eigenvalue of A;

b) If $a_{i,j}>0$ for all $i$ and $j$ in $\{1, . . . , n\}$, then $\varrho  >0$ and the primary space of $u_A$ relative to $\varrho$, that is to say the nilespace of $A-\varrho 1_{\mathbf{R}^n}$, is of dimension 1 and is generated by a vector $x_0\in (\mathbf{R}_+^*)^n$. There exists no other eigenvalue of A having an eigenvector in $\mathbf{R}^n_+$, and all complex eigenvalues $\lambda \not =\varrho$ of A satisfy $|\lambda |< \varrho$.

If $\varrho = 0$, assertion a) is elementary, for 0 is then an eigenvalue of A. If $\varrho  >0$, assertion a) follows from theorem 4 in view of lemma 7. Assertion b) is, for the same reason, a consequence of proposition 8.

#### Remark {#ts-iii-s6-n7-rem-2 .statement tag=02VD}

Assume that there exists an integer $k\geqslant 1$ such that all the coefficients of $A^k$ are $>0$ (such a matrix is sometimes called primitive). Then, by the cor. to Prop. 8, the spectral radius $\varrho$ is an eigenvalue of A, the primary space of $u_A$ relative to $\varrho$ is of dimension 1, and is generated by a vector $x_0\in (\mathbf{R}^*_+)^n$. Moreover, there exists no other complex eigenvalue of A admitting an eigenvector in $\mathbf{R}_+^n$ and all the complex eigenvalues $\lambda \not =\varrho$ of A satisfy $|\lambda |< \varrho$.

## EXERCISES {#ts-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).

[^1]: Some authors speak of a "finite point" of the spectrum, or of a "discrete spectrum".
