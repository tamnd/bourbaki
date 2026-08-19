---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 1
section_title: The Lie algebra sl(2, k) and its representations
lang: en
source: lie-vii-ix
book_pages: 69-77, 219-226
pdf_pages: 0077-0085, 0227-0234
extraction: native+ocr
subsections:
    - "no": 1
      title: CANONICAL BASIS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)
      page: 69
      pdf_page: 77
    - "no": 2
      title: PRIMITIVE ELEMENTS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MODULES
      page: 70
      pdf_page: 78
    - "no": 3
      title: THE SIMPLE MODULES V($\boldsymbol{m}$)
      page: 72
      pdf_page: 80
    - "no": 4
      title: LINEAR REPRESENTATIONS OF THE GROUP SL(2$\boldsymbol{, k}$)
      page: 74
      pdf_page: 82
    - "no": 5
      title: SOME ELEMENTS OF SL(2$\boldsymbol{, k}$)
      page: 76
      pdf_page: 84
statements: 23
exercises: 18
content_sha256: b250a236646a2094c99621b8d48c76e7dbf544dadaf2900324a770b228b036bf
---

## § 1. THE LIE ALGEBRA $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$) AND ITS REPRESENTATIONS

### 1. CANONICAL BASIS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)

#### Lemma 1 {#lie-viii-s1-lem-1 .statement tag=00XS}

Let A be an associative algebra over $k,H$ and $X$ elements of A such that $[H, X] = 2X$.

(i) $[H, X^n] = 2nX^n$ for any integer $n\geq 0$.

(ii) If $Z$ is an element of A such that $[Z, X] =H$, then, for any integer $n >0$,

$$
[Z, X^n] =nX^{n-1}(H+n-1) =n(H-n+ 1)X^{n-1}
$$

The map $T \rightarrow [H, T]$ from A to A is a derivation, which implies (i). With the assumptions in (ii),

$$
[Z, X^n] =\sum_{i+j=n-1}X^iHX^j
$$

$$
=\sum_{i+j=n-1}(X^iX^jH+X^i2jX^j)
$$

$$
=nX^{n-1}H+ 2X^{n-1}\frac{n(n- 1)}{2}
$$

$$
=nX^{n-1}(H+n-1)
$$

On the other hand, $X^{n-1}(H+n-1) = (H-n+ 1)X^{n-1}$ by (i). Q.E.D.

Recall that we denote by $\mathfrak{s}\mathfrak{l}(2, k)$ the Lie algebra consisting of the square matrices of order 2, trace zero, and with entries in $k$. This Lie algebra is simple of dimension 3 (Chap. I, §6, no. 7, Example). The canonical basis of $\mathfrak{s}\mathfrak{l}(2, k)$ is the basis $(X_+, X_-, H)$, where

$(01)($ 0 $0)(1$ 0 $)$

$X_+=$ 0 0 $X_-=-1$ 0 $H=$ 0 $-1$.

We have

$$
[H, X_+] = 2X_+[H, X_-] =-2X_-[X_+, X_-] =-H \tag{1}
$$

Since the identity representation of $\mathfrak{s}\mathfrak{l}(2, k)$ is injective, $H$ is a semi-simple element of $\mathfrak{s}\mathfrak{l}(2, k)$ and $X_+, X_-$ are nilpotent elements of $\mathfrak{s}\mathfrak{l}(2, k)$ (Chap. I, §6, no. 3, Th. 3). By Chap. VII, §2, no. 1, Example $4,kH$ is a Cartan subalgebra of $\mathfrak{s}\mathfrak{l}(2, k)$. The map $U \rightarrow  -^tU$ is an involutive automorphism of the Lie algebra $\mathfrak{s}\mathfrak{l}(2, k)$, called the canonical involution of $\mathfrak{s}\mathfrak{l}(2, k)$; it transforms $(X_+, X_-, H)$ into $(X_-, X_+,-H)$.

#### Lemma 2 {#lie-viii-s1-lem-2 .statement tag=00XT}

In the enveloping algebra of $\mathfrak{s}\mathfrak{l}(2, k)$,

$$
[H, X_+^n] = 2nX_+^n[H, X_-^n] =-2nX_-^n
$$

for any integer $n\geq 0$, and

$$
[X_-, X_+^n] =nX_+^{n-1}(H+n-1) =n(H-n+ 1)X_+^{n-1}
$$

$$
[X_+, X_-^n] =nX_-^{n-1}(-H+n-1) =n(-H-n+ 1)X_-^{n-1}
$$

if $n >0$.

The first and third relations follow from Lemma 1. The others can be deduced from them by using the canonical involution of $\mathfrak{s}\mathfrak{l}(2, k)$.

### 2. PRIMITIVE ELEMENTS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MODULES

Let E be an $\mathfrak{s}\mathfrak{l}(2, k$)-module. If $A\in \mathfrak{s}\mathfrak{l}(2, k)$ and $x\in E$, we shall often write $Ax$ instead of $A_Ex$. Let $\lambda \in k$. If $Hx=\lambda x$ we say, by abuse of language, that $x$ is an element of E of weight $\lambda$, or that $\lambda$ is the weight of $x$. If E is finite dimensional, $H_E$ is semi-simple, so the set of elements of weight $\lambda$ is the primary subspace of E relative to $H_E$ and $\lambda$ (cf. Chap. VII, §1, no. 1).

#### Lemma 3 {#lie-viii-s1-lem-3 .statement tag=00XU}

If $x$ is an element of weight $\lambda$, then $X_+x$ is an element of weight $\lambda + 2$ and $X_-x$ is an element of weight $\lambda -2$.

Indeed, $HX_+x= [H, X_+]x+X_+Hx= 2X_+x+X_+\lambda x= (\lambda + 2)X_+x$, and similarly $HX_-x= (\lambda -2)X_-x$ (cf. also Chap. VII, §1, no. 3, Prop. 10 (ii)).

#### Definition 1 {#lie-viii-s1-def-1 .statement tag=00XV}

Let E be an $\mathfrak{s}\mathfrak{l}(2, k)$-module. An element of E is said to be primitive if it is a non-zero eigenvector of $H_E$ and belongs to the kernel of $X_{+E}$.

A non-zero element $e$ of E is primitive if and only if $ke$ is stable under the operation of $kH+kX_+$; this follows for example from Lemma 3.

Examples The element $X_+$ is primitive of weight 2 for the adjoint representation of $\mathfrak{s}\mathfrak{l}(2, k)$. The element $(1,0)$ of $k^2$ is primitive of weight 1 for the identity representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $k^2$.

#### Lemma 4 {#lie-viii-s1-lem-4 .statement tag=00XW}

Let E be a non-zero finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-module. Then E has primitive elements.

Since $X_+$ is a nilpotent element of $\mathfrak{s}\mathfrak{l}(2, k),X_{+E}$ is nilpotent. Assume that $X_{+E}^{m-1}\not= 0$ and $X_{+E}^m$ = 0. By Lemma 2,

$$
m(H_E-m+ 1)X_{+E}^{m-1}= [X_{-E}, X_{+E}^m] = 0
$$

and hence the elements of $X_+^{m-1}(E)$**--** $\{0\}$ are primitive.

#### Proposition 1 {#lie-viii-s1-prop-1 .statement tag=00XX}

Let E be an $\mathfrak{s}\mathfrak{l}(2, k)$-module, and $e$ a primitive element of E of weight $\lambda$. Put $e_n=\frac{(-1)^n}{n}X_-^ne$ for $n\geq 0$, and $e_{-1}= 0$. Then

$$
He_n= (\lambda -2n)e_n
$$

$$
X_-e_n=-(n+ 1)e_{n+1} \tag{2}
$$

$$
X_+e_n= (\lambda -n+ 1)e_{n-1}
$$

The first formula follows from Lemma 3, and the second from the definition of the $e_n$. We prove the third by induction on $n$. It is satisfied for $n= 0$ since $e_{-1}= 0$. If $n >0$,

$$
nX_+e_n=-X_+X_-e_{n-1}=-[X_+, X_-]e_{n-1}-X_-X_+e_{n-1}
$$

$$
=He_{n-1}-X_-(\lambda -n+ 2)e_{n-2}
$$

$$
= (\lambda -2n+ 2 + (n-1)(\lambda -n+ 2))e_{n-1}
$$

$$
=n(\lambda -n+ 1)e_{n-1}
$$

#### Corollary {#lie-viii-s1-n2-cor-1 .statement tag=00XY}

The submodule of E generated by $e$ is the vector subspace generated by the $e_n$.

This follows from the formulas (2).

The integers $n\geq 0$ such that $e_n\not= 0$ constitute an interval in $\mathbf{N}$, and the corresponding elements $e_n$ form a basis over $k$ of the submodule generated by $e$ (indeed, they are linearly independent because they are non-zero elements of distinct weights). This basis will be said to be associated to the primitive element $e$.

#### Proposition 2 {#lie-viii-s1-prop-2 .statement tag=00XZ}

If the submodule V of E generated by the primitive element $e$ is finite dimensional, then:

(i) the weight $\lambda$ of $e$ is integral and equal to dim $V-1$;

(ii) $(e_0, e_1, . . . , e_{\lambda})$ is a basis of V, and $e_n= 0$ for $n > \lambda$;

(iii) the eigenvalues of $H_V$ are $\lambda , \lambda -2, \lambda -4, . . . ,-\lambda$; they are all of multiplicity 1;

(iv) every primitive element of V is proportional to $e$;

(v) the commutant of the module V is reduced to the scalars; in particular, V is absolutely simple.

Let $m$ be the largest integer such that $e_m\not= 0$. Then $0 =X_+e_{m+1}=$ $(\lambda -m)e_m$, so $\lambda =m$; since $(e_0, e_1, . . . , e_m)$ is a basis of V, this proves (i) and (ii). Assertion (iii) follows from the equality $He_n= (\lambda -2n)e_n$. We have $X_+e_n\not= 0$ for $1\leq n\leq m$, hence (iv). Let $c$ be an element of the commutant of the module V. Then $Hc(e) =cH(e) =\lambda c(e)$, so there exists $\mu\in k$ such that $c(e) =\mu e$; then

$$
cX_-^qe=X_-^qce=\mu X_-^qe
$$

for all $q\geq 0$, so $c=\mu.1$, proving (v).

#### Corollary {#lie-viii-s1-n2-cor-2 .statement tag=00Y0}

Let E be a finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-module.

(i) The endomorphism $H_E$ is diagonalizable and its eigenvalues are rational integers.

(ii) For any $p\in \mathbf{Z}$, let $E_p$ be the eigenspace of $H_E$ corresponding to the eigenvalue $p$. Let $i$ be an integer $\geq 0$. The map $X_{-E}^i|E_p: E_p\rightarrow E_{p-2i}$ is injective for $i\leq p$, bijective for $i=p$, and surjective for $i\geq p$. The map $X_{+E}^i|E_{-p}: E_{-p}\rightarrow E_{-p+2i}$ is injective for $i\leq p$, bijective for $i=p$, and surjective for $i\geq p$.

(iii) The length of E is equal to dim Ker$X_{+E}$ and to dim Ker$X_{-E}$.

(iv) Let $E'$ (resp. $E'')$ be the sum of the $E_p$ for $p$ even (resp. odd). Then $E'$ (resp. $E'')$ is the sum of the simple submodules of E of odd (resp. even) dimension; and $E = E'\oplus E''$. The length of $E'$ is dim $E_0$, and that of $E''$ is dim $E_1$.

(v) Ker$X_{+E}\cap$ Im$X_{+E}\subset \sum_{p>0}E_p$ and Ker$X_{-E}\cap$ Im$X_{-E}\subset \sum_{p<0}E_p$.

If E is simple, E is generated by a primitive element (Lemma 4), and it suffices to apply Propositions 1 and 2. The general case follows since every finite dimensional $\mathfrak{s}\mathfrak{l}(2, k$)-module is semi-simple.

### 3. THE SIMPLE MODULES V($\boldsymbol{m}$)

Let $(u, v)$ be the canonical basis of $k^2$. For the identity representation of $\mathfrak{s}\mathfrak{l}(2, k)$,

$$
X_+u= 0Hu=uX_-u=-v
$$

$$
X_+v=uHv=-vX_-v= 0
$$

Consider the symmetric algebra $\mathbf{S}(k^2)$ of $k^2($Algebra, Chap. III, §6, no. 1, Def. 1). The elements of $\mathfrak{s}\mathfrak{l}(2, k)$ extend uniquely to derivations of $\mathbf{S}(k^2)$, giving $\mathbf{S}(k^2)$ the structure of an $\mathfrak{s}\mathfrak{l}(2, k$)-module (Chap. I, §3, no. 2). Let $V(m)$ be the set of homogeneous elements of $\mathbf{S}(k^2)$ of degree $m$. Then $V(m)$ is an $\mathfrak{s}\mathfrak{l}(2, k$)-submodule of $\mathbf{S}(k^2)$ of dimension $m+ 1$, the $m$th symmetric power of $V(1) =k^2$ (Chap. III, Appendix). If $m, n$ are integers such that $0\leq n\leq m$, put

$$
e^{(m)}_n=(m)u^{m-n}v^n\in V(m)
$$

$$
n
$$

#### Proposition 3 {#lie-viii-s1-prop-3 .statement tag=00Y1}

For any integer $m\geq 0$, $V(m)$ is an absolutely simple $\mathfrak{s}\mathfrak{l}(2, k)$-module. In this module, $e^{(m)}_0=u^m$ is primitive of weight $m$.

We have $X_+u^m= 0$ and $Hu^m=mu^m$, so $u^m$ is primitive of weight $m$. The submodule of $V(m)$ generated by $u^m$ is of dimension $m+ 1$ (Prop. 2 (i)) and so is equal to $V(m)$. By Prop. 2 (v), $V(m)$ is absolutely simple.

#### Theorem 1 {#lie-viii-s1-thm-1 .statement tag=00Y2}

Every simple $\mathfrak{s}\mathfrak{l}(2, k)$-module of finite dimension $n$ is isomorphic to $V(n-1)$. Every finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-module is a direct sum of submodules isomorphic to the modules $V(m)$.

This follows from Lemma 4 and Prop. 1, 2 and 3.

#### Remark 1 {#lie-viii-s1-n3-rem-1 .statement tag=00Y3}

The adjoint representation of $\mathfrak{s}\mathfrak{l}(2, k)$ defines on $\mathfrak{s}\mathfrak{l}(2, k)$ the structure of a simple $\mathfrak{s}\mathfrak{l}(2, k$)-module. This module is isomorphic to V(2) by an isomorphism that takes $u^2$ to $X_+, 2uv$ to $-H$, and $v^2$ to $X_-$.

#### Remark 2 {#lie-viii-s1-n3-rem-2 .statement tag=00Y4}

For $n\geq 0$ and $m > n$,

$$
X_-e^{(m)}_n=-(m-n)(m)u^{m-n-1}v^{n+1}=-(n+ 1)e^{(m)}_{n+1}
$$

$$
n
$$

Hence, $(e_0^{(m)}, e_1^{(m)}, . . . , e_m^{(m)})$ is the basis of $V(m)$ associated to the primitive element $e_0^{(m)}$.

#### Remark 3 {#lie-viii-s1-n3-rem-3 .statement tag=00Y5}

Let $\Phi$ be the bilinear form on $V(m)$ such that

$\Phi (e^{(m)}_n, e^{(m)}_{n'}) = 0$ if $n+n'\not=m$

$$
\Phi (e^{(m)}_n, e^{(m)}_{m-n}) = (-1)^n(m)
$$

$$
n
$$

If $x=au+bv$ and $y=cu+dv$, then $\Phi (x^m, y^m) = (ad-bc)^m$. It is now easy to check that $\Phi$ is invariant, and that $\Phi$ is symmetric for $m$ even, and alternating for $m$ odd.

#### Proposition 4 {#lie-viii-s1-prop-4 .statement tag=00Y6}

Let E be a finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-module, $m$ an integer $\geq 0$, $P_m$ the set of primitive elements of weight $m$. Let L be the vector space of homomorphisms from the $\mathfrak{s}\mathfrak{l}(2, k)$-module $V(m)$ to the $\mathfrak{s}\mathfrak{l}(2, k)$-module E. The map $f \rightarrow f(u^m)$ from L to E is linear, injective, and its image is $P_m\cup  \{0\}$.

This map is clearly linear, and it is injective because $u^m$ generates the $\mathfrak{s}\mathfrak{l}(2, k$)-module $V(m)$. If $f\in L$,

$$
X_+(f(u^m)) =f(X_+u^m) = 0,H(f(u^m)) =f(Hu^m) =mf(u^m)
$$

so $f(u^m)\in P_m\cup  \{0\}$. Let $e\in P_m$, and V the submodule of E generated by $e$. By Prop. 1, there exists an isomorphism from the module $V(m)$ to the module V that takes $u^m$ to $e$. Then $L(u^m) = P_m\cup  \{0\}$.

#### Corollary {#lie-viii-s1-n3-cor-1 .statement tag=00Y7}

The isotypical component of E of type $V(m)$ has length

dim(P$_m\cup  \{0\}$.

### 4. LINEAR REPRESENTATIONS OF THE GROUP SL(2$\boldsymbol{, k}$)

Recall (Algebra, Chap. III, §8, no. 9) that we denote by $\mathbf{S}\mathbf{L}(2, k)$ the group of square matrices of order 2 with coefficients in $k$ whose determinant is equal to 1. If $x\in \mathfrak{s}\mathfrak{l}(2, k)$ is nilpotent, then $x^2= 0 ($Algebra, Chap. VII, §5, Cor. 3 of Prop. 5) and $e^x= 1 +x\in \mathbf{S}\mathbf{L}(2, k)$. If E is a finite dimensional vector space and $\rho$ is a linear representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on E, then $\rho (x)$ is nilpotent and so $e^{\rho(x)}$ is defined (Chap. I, §6, no. 3).

#### Definition 2 {#lie-viii-s1-def-2 .statement tag=00Y8}

Let E be a finite dimensional vector space, and $\rho$ (resp. $\pi )$ a linear representation of $\mathfrak{s}\mathfrak{l}(2, k)$ (resp. $\mathbf{S}\mathbf{L}(2, k))$ on E. Then $\rho$ and $\pi$ are said to be compatible if, for every nilpotent element $x$ of $\mathfrak{s}\mathfrak{l}(2, k),\pi (e^x) =e^{\rho(x)}$.

In other words, $\rho$ and $\pi$ are compatible if, for every nilpotent element $x$ of $\mathfrak{s}\mathfrak{l}(2, k)$, the restriction of $\rho$ to $kx$ is compatible with the restriction of $\pi$ to the group $1 +kx$ (Chap. VII, §3, no. 1).

If $\rho$ and $\pi$ are compatible, so are the dual representations, the $m$th tensor powers, and the $m$th symmetric powers of $\rho$ and $\pi$, respectively (Chap. VII, §5, no. 4, Lemma 1 (i) and (ii)). Similarly for the representations induced by $\rho$ and $\pi$ on a vector subspace stable under $\rho$ and $\pi ($loc. cit.).

In particular, the representation $\rho_m$ of $\mathfrak{s}\mathfrak{l}(2, k)$ on $V(m)$ (no. 3) is compatible with the $m$th symmetric power $\pi_m$ of the identity representation $\pi_1$ of $\mathbf{S}\mathbf{L}(2, k)$. Putting $e^{(m)}_n=(^m_n)u^{m-n}v^n$ as above, we have

$(m)(m)m-nn$

$\pi_m(s)e_n$ = $(su)(sv)$ (3)

$$
n
$$

for $s\in \mathbf{S}\mathbf{L}(2, k)$ and $0\leq n\leq m$.

#### Theorem 2 {#lie-viii-s1-thm-2 .statement tag=00Y9}

Let $\rho$ be a linear representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on a finite dimensional vector space E.

(i) There exists a unique linear representation $\pi$ of $\mathbf{S}\mathbf{L}(2, k)$ on E that is compatible with $\rho$.

(ii) A vector subspace F of E is stable under $\pi$ if and only if it is stable under $\rho$.

(iii) Let $x\in E$. Then $\pi (s)x=x$ for all $s\in \mathbf{S}\mathbf{L}(2, k)$ if and only if $x$ is invariant under $\rho ($that is, $\rho (a)x= 0$ for all $a\in \mathfrak{s}\mathfrak{l}(2, k))$.

The existence of $\pi$ follows from the preceding and Th. 1. On the other hand, we know that the group $\mathbf{S}\mathbf{L}(2, k)$ is generated by the elements of the form

$$
_{tX}(1t)_{-tX_-}(10)
$$

$e^+=e$ =

0 1 $t$ 1

where $t\in k($Algebra, Chap. III, §8, no. 9, Prop. 17). This proves the uniqueness of $\pi$.

Assertions (ii) and (iii) follow from what we have said, together with Chap. VII, §3, no. 1, Lemma 1 (i). Q.E.D.

Every finite dimensional $\mathfrak{s}\mathfrak{l}(2, k$)-module therefore has a unique $\mathbf{S}\mathbf{L}(2, k)$-module structure, which is said to be associated to its $\mathfrak{s}\mathfrak{l}(2, k$)-module structure.

#### Remark {#lie-viii-s1-n4-rem-1 .statement tag=00YA}

When $k$ is $\mathbf{R}$ or $\mathbf{C}$ or a complete non-discrete ultrametric field, $\mathfrak{s}\mathfrak{l}(2, k)$ is the Lie algebra of $\mathbf{S}\mathbf{L}(2, k)$. Let $\rho$ and $\pi$ be as in Th. 2. The homomorphism $\pi$ is a homomorphism of Lie groups from $\mathbf{S}\mathbf{L}(2, k)$ to $\mathbf{G}\mathbf{L}(E):$ this is clear when $E = V(m)$, and the general case follows, in view of Th. 1. By Chap. VII, §3, no. $1,\rho (X_+) = L(\pi )(X_+),\rho (X_-) = L(\pi )(X_-)$. Hence $\rho = L(\pi )$ (for a converse, see Exerc. 18).

#### Proposition 5 {#lie-viii-s1-prop-5 .statement tag=00YB}

Let E, F be finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-modules, and let $f\in$ Hom$_k(E,F)$. The following conditions are equivalent:

(i) $f$ is a homomorphism of $\mathfrak{s}\mathfrak{l}(2, k)$-modules;

(ii) $f$ is a homomorphism of $\mathbf{S}\mathbf{L}(2, k)$-modules.

Condition (i) means that $f$ is an invariant element of the $\mathfrak{s}\mathfrak{l}(2, k$)-module Hom$_k(E,F)$, and condition (ii) means that $f$ is an invariant element of the $\mathbf{S}\mathbf{L}(2, k$)-module Hom$_k(E,F)$. Since these module structures are associated by Chap. VII, §5, no. 4, Lemma 1 (iii), the proposition follows from Th. 2 (iii).

#### Definition 3 {#lie-viii-s1-def-3 .statement tag=00YC}

The adjoint representation of the group $\mathbf{S}\mathbf{L}(2, k)$ is the linear representation Ad of $\mathbf{S}\mathbf{L}(2, k)$ on $\mathfrak{s}\mathfrak{l}(2, k)$ defined by

Ad($s$)$.a=sas^{-1}$

for all $a\in \mathfrak{s}\mathfrak{l}(2, k)$ and all $s\in \mathbf{S}\mathbf{L}(2, k)$. When $k$ is $\mathbf{R}$ or $\mathbf{C}$ or a complete non-discrete ultrametric field, we recover Def. 7 of Chap. III, §3, no. 12 (cf. loc. cit., Prop. 49).

By Chap. VII, §5, no. 4, Lemma 1 (i) and (ii), the adjoint representations of $\mathfrak{s}\mathfrak{l}(2, k)$ and $\mathbf{S}\mathbf{L}(2, k)$ are compatible. By Chap. VII, §3, no. 1, Remark 2, Ad($\mathbf{S}\mathbf{L}(2, k)$) $=$ Aut$_e(\mathfrak{s}\mathfrak{l}(2, k))$.

### 5. SOME ELEMENTS OF SL(2$\boldsymbol{, k}$)

For any $t\in k^*$, put

$$
\theta (t) =e^{tX_+}e^{t^{-1}X_-}e^{tX_+}
$$

$(1t)(($ 1 $0)((1t)$

= 0 1 $-t^{-1}$ 1 0 1

$($ 0 $t)$

= $-t^{-1}$ 0

$$
=e^{t^{-1}X_-}e^{tX_+}e^{t^{-1}X_-}
$$

With the notations of no. 3,

$$
\theta (t)u=-t^{-1}v\theta (t)v=tu
$$

so

$$
\theta (t)e^{(m)}_n= (-1)^{m-n}t^{2n-m}e^{(m)}_{m-n} \tag{4}
$$

Hence, the element $\theta (t)^2=(-1$ 0 $)$ operates by $(-1)^m$ on $V(m)$. If

0 $-1$

E is an odd-dimensional simple $\mathfrak{s}\mathfrak{l}(2, k$)-module, $\theta (t)_E$ is thus an involutive automorphism of the vector space E. In particular, taking E to be the adjoint representation:

$$
\theta (t)_EX_+=t^{-2}X_-\theta (t)_EX_-=t^2X_+\theta (t)_EH=-H \tag{5}
$$

so that $\theta (1)_E=\theta (-1)_E$ is the canonical involution of $\mathfrak{s}\mathfrak{l}(2, k)$.

For any $t\in k^*$, put

$$
h(t) =(0tt^-0_1)=\theta (t)\theta (-1)
$$

Then $h(t)u=tu,h(t)v=t^{-1}v$, so

$$
h(t)e^{(m)}_n=t^{m-2n}e^{(m)}_n \tag{6}
$$

#### Proposition 6 {#lie-viii-s1-prop-6 .statement tag=01L4}

Let E be a finite dimensional $\mathfrak{s}\mathfrak{l}(2, k)$-module, and $t\in k^*$. Let $E_p$ be the set of elements of E of weight $p$.

(i) $\theta (t)_E|E_p$ is a bijection from $E_p$ to $E_{-p}$.

(ii) $h(t)_E|E_p$ is the homothety with ratio $t^p$ on $E_p$.

If $E = V(n)$, the proposition follows from formulas (4) and (6). The general case follows from Th. 1.

#### Corollary {#lie-viii-s1-n5-cor-1 .statement tag=00YD}

Let $E = E'\oplus E''$ be the decomposition of E defined in the Cor. of Prop. 2. The element $(-10)$ of $\mathbf{S}\mathbf{L}(2, k)$ operates by +1 on $E'$

0 $-1$

and by $-1$ on $E''$.

This follows from (ii), applied to $t=-1$.

### Exercises {#lie-viii-s1-exercises}

The base field $k$ is assumed to be of characteristic zero.

Unless explicitly stated otherwise, Lie algebras are assumed to be finite dimensional.

We denote by $\mathfrak{s}$ the Lie algebra $\mathfrak{s}\mathfrak{l}(2, k)$.

See the [exercises for § 1](exercises/s1/).
