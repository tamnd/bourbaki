---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 8
section_title: Fourier transform
lang: en
source: lie-vii-ix
book_pages: 359-369, 417-418
pdf_pages: 0366-0376, 0424-0425
extraction: native
subsections:
    - "no": 1
      title: FOURIER TRANSFORMS OF INTEGRABLE FUNCTIONS
      page: 360
      pdf_page: 367
    - "no": 2
      title: FOURIER TRANSFORMS OF INFINITELY-DIFFERENTIABLE FUNCTIONS
      page: 362
      pdf_page: 369
    - "no": 3
      title: FOURIER TRANSFORMS OF CENTRAL FUNCTIONS
      page: 366
      pdf_page: 373
    - "no": 4
      title: CENTRAL FUNCTIONS ON G AND FUNCTIONS ON T
      page: 368
      pdf_page: 375
statements: 9
exercises: 6
content_sha256: b13b9ed9613c7bd66a8b27991afc9484e741ec478bff10547efbaab20cbb58f3
---

## § 8. FOURIER TRANSFORM

We retain the notations and conventions of the preceding paragraph.

$^5$ The proof of loc. cit., which has been stated only for split semi-simple Lie algebras,

is valid without change in the case of split reductive Lie algebras.

### 1. FOURIER TRANSFORMS OF INTEGRABLE FUNCTIONS

In this number, we recall some definitions and results from Spectral Theories$^6$.

Denote by $\widehat{G}$ the set of classes of irreducible representations of G (on finite dimensional complex vector spaces). For all $u\in \widehat{G}$, denote by $Eu$ the space of $u$ and $d(u)$ its dimension. There exist separating positive hermitian forms on $E_u$ invariant under $u$, and any two such forms are proportional. Denote by $A^*$ (resp. $\|A\|_{\infty})$ the adjoint (resp. the norm) of an element A of End(E$_u)$ relative to one of these forms; for all $g\in G$, we have $u(g)^*=u(g)^{-1}=u(g^{-1})$ and $\|u(g)\|_{\infty}= 1$; for all $x\in \mathfrak{g}$, we have $u(x)^*=-u(x) =u(-x)$.

Give End(E$_u)$ the Hilbert space structure for which the scalar product is

$\langle A|B\rangle =d(u$)Tr(A$^*B) =d(u$)Tr(BA$^*)$, (1)

and put

$\|A\|_2=\langle A|A\rangle^{1/2}= (d(u$)Tr(A$^*A))^{1/2}$. (2)

We have

$$
\surd\overline{d(u)}\|A\|_{\infty}\leq  \|A\|_2\leq d(u)\|A\|_{\infty} \tag{3}
$$

so

$$
|\langle A|B\rangle | \leq d(u)^2\|A\|_{\infty}\|B\|_{\infty} \tag{4}
$$

For all $g\in G$, we have $\|u(g)\|_2=d(u)$.

Denote by $F( \widehat{G})$ the algebra $\prod_{u\in\widehat{G}}$ End(E$_u)$. Denote by $L^2( \widehat{G})$ the Hilbert sum of the Hilbert spaces End(E$_u)$; this is the space of families $A= (A_u)\in F( \widehat{G})$ such that $\sum_u\|A_u\|^2_2<\infty$, with the scalar product

$\langle A|B\rangle =\sum_{u\in\widehat{G}}\langle A_u|B_u\rangle =\sum_{u\in\widehat{G}}d(u$)Tr(A$^*_uB_u)$. (5)

Denote the Hilbert norm on $L^2( \widehat{G})$ also by $\| \|_2$, so that $\|A\|^2_2=\sum_{u\in\widehat{G}}\|A_u\|^2_2$ for $A\in L^2( \widehat{G})$.

If $f$ is an integrable complex function on G, put

$u(f) =\int_Gf(g)u(g)dg\in$ End(E$_u)$ (6)

for all $u\in \widehat{G}$. We have $\|u(f)\|_{\infty}\leq \int_G|f(g)|dg=\|f\|_1$. The Fourier cotransform of $f$, denoted by $\mathscr{F}(f)$, is the family $(u(f))_{u\in\widehat{G}}\in F( \widehat{G})$. If $f\in L^2( \widehat{G})$,

$^6$ See note $^1$, §7, p. 66.

$$
\|f\|^2_2=\sum_{u\in\widehat{G}}\langle u(f)|u(f)\rangle =\|\overline{\mathscr{F}}(f)\|^2_2
$$

so $\overline{\mathscr{F}}$ induces an isometric linear map from the Hilbert space $L^2(G)$ to the Hilbert space $L^2( \widehat{G}):$ in other words, for $f$ and $f'$ in $L^2$(G), we have

$\int_G\overline{f(g)}f'(g)dg=\langle \overline{\mathscr{F}}(f)|\overline{\mathscr{F}}(f')\rangle =\sum_{u\in\widehat{G}}d(u$)Tr($u(f)^*u(f')$). (7)

For $f$ and $f'$ in $L^1$(G), the convolution product $f*f'$ of $f$ and $f'$ is defined by

$$
(f*f')(h) =\int_Gf(hg^{-1})f'(g)dg=\int_Gf(g)f'(g^{-1}h)dg
$$

(the integral makes sense for almost all $h\in G)$.

We have $f*f'\in L^1(G)$ and, for all $u\in \widehat{G},u(f*f') =u(f)u(f')$, so

$$
\overline{\mathscr{F}}(f*f') =\overline{\mathscr{F}}(f).\overline{\mathscr{F}}(f') \tag{8}
$$

Conversely, let $A = (A_u)_{u\in\widehat{G}}$ be an element of $F( \widehat{G})$; for all $u\in \widehat{G}$, let $\mathscr{F}_uA$ be the (analytic) function on G defined by

$(\mathscr{F}_uA)(g) =\langle u(g)|A_u\rangle =d(u$)Tr(A$_uu(g)^{-1})$. (9)

If $A\in L^2( \widehat{G})$, the family $(\mathscr{F}_uA)_{u\in\widehat{G}}$ is summable in $L^2(G)$; the Fourier transform of A, denoted by $\mathscr{F}$(A), is the sum of this family. The maps $\mathscr{F}$ and $\mathscr{F}$ are inverse isomorphisms between the Hilbert spaces $L^2(G)$ and $L^2( \widehat{G})$.

In other words:

#### Proposition 1 {#lie-ix-s8-prop-1 .statement tag=01GZ}

Every square integrable complex function $f$ on G is the sum in the Hilbert space $L^2(G)$ of the family $(f_u)_{u\in\widehat{G}}$ where, for all $h\in G$ and all $u\in \widehat{G}$,

$$
f_u(h) =\langle u(h)|u(f)\rangle
$$

$=d(u)\int_Gf(g$)Tr($u(gh^{-1})$)$dg=d(u)\int_Gf(gh$)Tr($u(g)$)$dg$. (10)

For all $u\in \widehat{G}$ choose an orthonormal basis $Bu$ of $E_u$, and denote by $(u_{ij}(g))$ the matrix of $u(g)$ in this basis. Prop. 1 also means that the family of functions $\surd\overline{d(u)}u_{ij}$, for $u$ in $\widehat{G}$ and $i, j$ in $B_u$, is an orthonormal basis of the space $L^2(G)$.

If $f$ is an integrable function on G such that the family $(f_u)$ is uniformly summable, then the sum of this family is a continuous function which coincides almost everywhere with $f$; in other words, if we assume in addition that $f$ is continuous, then for all $h\in G$,

$f(h) =\sum_{u\in\widehat{G}}d(u)\int_Gf(gh$)Tr($u(g)$)$dg$. (11)

Conversely, let $A\in F( \widehat{G})$; if the family $(\mathscr{F}_uA)_{u\in\widehat{G}}$ is uniformly summable, the function

$g \rightarrow \sum_{u\in\widehat{G}}(\mathscr{F}_uA)(g) =\sum_{u\in\widehat{G}}d(u$)Tr(A$_uu(g)^{-1})$

is a continuous function on G whose Fourier cotransform is A.

Let $f$ be an integrable function on G, and let $s\in G$. Denote by $\gamma (s)f$ and $\delta (s)f$ the functions on G defined by $\gamma (s)f=\varepsilon_s*f,\delta (s)f=f*\varepsilon_{s^{-1}}$, that is,

$(\gamma (s)f)(g) =f(s^{-1}g),(\delta (s)f)(g) =f(gs)$ for $g\in G$,

(Chap. III, §3, no. 4 and Integration, Chap. VII, §1, no. 1). We have

$$
u(\gamma (s)f) =\int_Gf(s^{-1}g)u(g)dg=\int_Gf(g)u(sg)dg
$$

so

$$
u(\gamma (s)f) =u(s)u(f) \tag{12}
$$

and similarly

$$
u(\delta (s^{-1})f) =u(f)u(s) \tag{13}
$$

When G is commutative, $\widehat{G}$ is the underlying set of the dual group of G (Spectral Theories, Chap. II, §1, no. $1),d(u) = 1$ for all $u\in \widehat{G}$, and we recover the definitions of the Fourier transform given in Spectral Theories, Chap. II.

### 2. FOURIER TRANSFORMS OF INFINITELY-DIFFERENTIABLE FUNCTIONS

Recall (Chap. III, §3, no. 1, Def. 2) that U(G) denotes the algebra of distributions on G with support contained in $\{e\}$. The canonical injection of $\mathfrak{g}$ into U(G) extends to an isomorphism from the enveloping algebra of the Lie algebra $\mathfrak{g}$ to U(G) (loc. cit., no. 7, Prop. 25); from now on we identify these two algebras by this isomorphism. If $f$ is an infinitely-differentiable complex function on G and if $t\in U(G)$, we denote by $L_tf$ and $R_tf$ the functions on G defined by

$$
L_tf(g) =\langle \varepsilon_g*t, f\rangle ,R_tf(g) =\langle t*\varepsilon_g, f\rangle
$$

(cf. loc. cit., no. 6). For all $g\in G$,

$$
L_t\circ \gamma (g) =\gamma (g)\circ L_t,R_t\circ \delta (g) =\delta (g)\circ R_t
$$

Let $u\in \widehat{G}$; denote by $Eu$ the space of $u$. The morphism of Lie groups $u: G\rightarrow \mathbf{G}\mathbf{L}(E_u)$ gives by differentiation a homomorphism of (real) Lie algebras $\mathfrak{g}\rightarrow$ End(E$_u)$, hence a homomorphism of algebras, also denoted by $u$, from U(G) to End(E$_u)$. If $t\in U(G)$ and if $f$ is an infinitely-differentiable function on G, then

$$
u(L_tf) =u(f)u(t^{\vee}), u(R_tf) =u(t^{\vee})u(f) \tag{14}
$$

where $t^{\vee}$ denotes the image of $t$ under the principal anti-automorphism of U(G) (Chap. I, §2, no. 4); indeed, it suffices to verify this for $t\in \mathfrak{g}$, in which case it follows by differentiation from formulas (12) and (13) (cf. Chap. III, §3, no. 7, Prop. 27).

For all $u\in \widehat{G}$, denote by $\lambda (u)$ the highest weight of $u($§7, no. 2, Th. 1), so $u \rightarrow \lambda (u)$ is a bijective map from $\widehat{G}$ to the set $X_{++}$ of dominant elements of X(T).

Let $\Gamma \in U(G)$ be a Casimir element of G (§7, no. 6); for all $u\in \widehat{G}$, the endomorphism $u(\Gamma )$ of $E_u$ is a homothety, whose ratio we denote by $\widetilde{\Gamma}(u)$, so we have a map $u \rightarrow \widetilde{\Gamma}(u)$ from $\widehat{G}$ to $\mathbf{C}$.

If $\varphi$ and $\psi$ are two functions on $\widehat{G}$ with positive real values, denote by “$\varphi \preccurlyeq \psi$” or “$\varphi (u)\preccurlyeq \psi (u$)” the relation “there exists $M>0$ such that $\varphi (u)\leq M\psi (u)$ for all $u\in \widehat{G}$”; this is a pre-order relation on the set of functions on $\widehat{G}$ with positive real values.

#### Proposition 2 {#lie-ix-s8-prop-2 .statement tag=01H0}

Let $m \rightarrow  \|m\|$ be a norm on the $\mathbf{R}$-vector space $\mathbf{R}\otimes X(T)$ and $\Gamma$ a Casimir element of G. Let $\varphi$ be a function on $\widehat{G}$ with positive real values.

a) The following conditions are equivalent:

(i) There exists an integer $n >0$ such that $\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^n$ (resp. for every integer $n >0$, we have $\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^{-n})$.

(ii) There exists an integer $n >0$ such that $\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^n$ (resp. for every integer $n >0$, we have $\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^{-n})$.

b) If G is semi-simple, conditions (i) and (ii) are also equivalent to:

(iii) There exists an integer $n >0$ such that $\varphi (u)\preccurlyeq d(u)^n$ (resp. for every integer $n >0$, we have $\varphi (u)\preccurlyeq d(u)^{-n})$.

Note first of all that condition (i) is clearly independent of the choice of norm. Thus we can use the norm defined by the quadratic form $Q_{\Gamma}$ associated to $\Gamma ($§7, no. 6, Prop. 4). Then

$$
0\leq \widetilde{\Gamma}(u) =\|\lambda (u) +\rho \|^2- \|\rho \|^2
$$

so $\widetilde{\Gamma}(u) + 1\preccurlyeq (\|\lambda (u)\|+ 1)^2\preccurlyeq \widetilde{\Gamma}(u) + 1$, hence $a)$.

Further, if G is semi-simple,

$\|\lambda (u) +\rho \|\preccurlyeq d(u)\preccurlyeq \|\lambda (u) +\rho \|^N$, where $N = 1/$2(dim $G-$ dim T)

(§7, no. 5, Cor. 1 of Th. 3), so $\|\lambda (u)\|+ 1\preccurlyeq d(u)\preccurlyeq (\|\lambda (u)\|+ 1)^N$, hence $b)$.

It follows from Prop. 2 that condition (i) is independent of the choice of maximal torus, chamber, and norm, and that condition (ii) is independent of the choice of Casimir element. A function $\varphi$ satisfying conditions (i) and (ii) is said to be moderately increasing (resp. rapidly decreasing). The product of two moderately increasing functions is moderately increasing; the product of a moderately increasing function and a rapidly decreasing function is rapidly decreasing. If $\varphi$ is rapidly decreasing, the family $(\varphi (u))_{u\in\widehat{G}}$ is summable.

#### Example {#lie-ix-s8-n2-exa-1 .statement tag=01H1}

The function $u \rightarrow d(u)$ is moderately increasing (§7, no. 5, Cor. 1 of Th. 3); for any norm $\| \|$ on $\mathbf{R}\otimes X(T)$, the function $u \rightarrow  \|\lambda (u)\|$ is moderately increasing. For any Casimir element $\Gamma$, the function $u \rightarrow \widetilde{\Gamma}(u)$ is moderately increasing; more generally:

#### Proposition 3 {#lie-ix-s8-prop-3 .statement tag=01H2}

For all $t\in$ U(G), the functions $u \rightarrow  \|u(t)\|_{\infty}$ and $u \rightarrow  \|u(t)\|_2$ on $\widehat{G}$ are moderately increasing.

Since the product of two moderately increasing functions is moderately increasing, it suffices to prove this when $t\in \mathfrak{g}:$ in that case the assertion follows from the Remark in §7, no. 6 and the inequality

$$
\|u(t)\|_2\leq d(u)\|u(t)\|_{\infty}
$$

#### Theorem 1 {#lie-ix-s8-thm-1 .statement tag=01H3}

a) Let $f$ be an infinitely-differentiable complex function on G. Then the family $(f_u)_{u\in\widehat{G}}$, where $f_u(g) =\langle u(g)|u(f)\rangle$, is uniformly summable on G and, for all $h\in G$,

$f(h) =\sum_{u\in\widehat{G}}\langle u(h)|u(f)\rangle =\sum_{u\in\widehat{G}}d(u)\int_Gf(g$)Tr($u(gh^{-1})$)$dg$.

b) Let $f$ be an integrable function on G; then $f$ is equal almost everywhere to an infinitely-differentiable function if and only if the function $u \rightarrow  \|u(f)\|_{\infty}$ is rapidly decreasing on $\widehat{G}$.

Let $f$ be an infinitely-differentiable function on G, and let $\Gamma$ be a Casimir element for G; by formula (14),

$$
\widetilde{\Gamma}(u)^nu(f) =u(f)u(\Gamma )^n=u((L_{\Gamma})^nf)
$$

for all $n\geq 0$, and consequently

$\widetilde{\Gamma}(u)^n\|u(f)\|_{\infty}\leq  \|(L_{\Gamma})^nf\|_1\leq$ sup$_{g\in G}|((L_{\Gamma})^nf)(g)|$; (15)

thus, the function $u \rightarrow  \|u(f)\|_{\infty}$ is indeed rapidly decreasing.

Conversely, let $A = (A_u)_{u\in\widehat{G}}$ be an element of $F( \widehat{G})$ such that the function $u \rightarrow  \|A_u\|_{\infty}$ is rapidly decreasing. Put $f_u(g) =\langle u(g)|A_u\rangle$; the function $g \rightarrow f_u(g)$ is analytic, hence infinitely-differentiable. By Chap. III, §3, no. 7, Prop. 27,

$$
(L_xf_u)(g) =\langle u(g)u(x)|A_u\rangle
$$

for all $x\in \mathfrak{g}$. Let $t\in U(G)$; by the preceding formula,

$$
(L_tf_u)(g) =\langle u(g)u(t)|A_u\rangle
$$

and consequently

$$
|(L_tf_u)(g)|=|\langle u(g)u(t)|A_u\rangle  \leq d(u)^2\|u(t)\|_{\infty}\|u(g)\|_{\infty}\|A_u\|_{\infty}
$$

$$
=d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}
$$

Since $d(u)$ and $\|u(t)\|_{\infty}$ are moderately increasing (Prop. 3) and $\|A_u\|_{\infty}$ is rapidly decreasing, the function $u \rightarrow$ sup$_g|(L_tf_u)(g)|$ is rapidly decreasing; thus, the family $(L_tf_u)_{u\in\widehat{G}}$ is uniformly summable. It follows$^7$ that the sum of the family $(f_u)$ is an infinitely-differentiable function on G, whose Fourier cotransform is $(A_u)$, hence the theorem.

Denote by $\mathscr{S}( \widehat{G})$ the vector subspace of $L^2( \widehat{G})$ consisting of the families $A = (A_u)_{u\in\widehat{G}}$ such that the function $u \rightarrow  \|A_u\|_{\infty}$ is rapidly decreasing on $\widehat{G}$. It follows from the theorem that the maps $\mathscr{F}:f \rightarrow (u(f))_{u\in\widehat{G}}$ and $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ induce inverse isomorphisms between the complex vector spaces $\mathscr{C}^{\infty}(G;\mathbf{C})$ and $\mathscr{S}( \widehat{G})$. Give the space $\mathscr{C}^{\infty}(G;\mathbf{C})$ the topology of uniform $C^{\infty}$-convergence (§6, no. 4) which can be defined by the family of semi-norms $f \rightarrow$ sup$_{g\in G}|L_tf(g)|$ for $t\in U(G)$, and the space $\mathscr{S}( \widehat{G})$ the topology defined by the sequence of semi-norms $p_n: A \rightarrow$ sup$_{u\in\widehat{G}}( \widetilde{\Gamma}(u) + 1)^n\|A_u\|_{\infty}$. Formula (15) of the preceding proof shows that $\overline{\mathscr{F}}$ is continuous. Let $t\in U(G)$, and let $A = (A_u)_{u\in\widehat{G}}$ be an element of $\mathscr{S}( \widehat{G})$; put $f_n(g) =\langle u(g)|A_u\rangle$. Let $p$ be an integer such that $\sum_{u\in\widehat{G}}\widetilde{\Gamma}(u)^{-p}= M<\infty$. By the preceding proof, there exists a positive integer $m$ such that, for all $g\in G$,

$$
|(L_tf_u)(g)| \leq d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}\leq m.(1 + \widetilde{\Gamma}(u))^m\widetilde{\Gamma}(u)^{-p}\|A_u\|_{\infty}
$$

so $|(L_t\mathscr{F}(A))(g)| \leq mMp_m(A)$; this proves that $\mathscr{F}$ is continuous. Consequently:

#### Corollary {#lie-ix-s8-n2-cor-1 .statement tag=01H4}

The maps $\overline{\mathscr{F}}:f \rightarrow (u(f))_{u\in\widehat{G}}$ and $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ induce inverse isomorphisms between the topological vector spaces $\mathscr{C}^{\infty}(G;\mathbf{C})$ and $\mathscr{S}( \widehat{G})$.

$^7$ This follows from the fact that the space $\mathscr{C}^{\infty}(G;\mathbf{C})$, with the topology of uniform

$C^{\infty}$-convergence (§6, no. 4), is complete.

### 3. FOURIER TRANSFORMS OF CENTRAL FUNCTIONS

For all $u\in \widehat{G}$, denote by $\chi_u$ the character of $u$; thus,

$\chi_u(g) =$ Tr($u(g)$)$,(g\in G)$. (16)

Recall from Spectral Theory the formulas

$$
\chi_u*\chi_v= 0(u, v\in \widehat{G}, u\not=v) \tag{17}
$$

1

$$
\chi_u*\chi_u=\chi_u(u\in \widehat{G}) \tag{18}
$$

$$
d(u)
$$

For all $u\in \widehat{G}$, denote by $\varepsilon_u$ the identity map of $E_u$. Recall (§7, no. 4) that ZL$^2(G)$ denotes the subspace of $L^2(G)$ consisting of the classes of the functions $f$ that are central, that is, such that $f\circ$ Int $s=f$ for all $s\in G$, or equivalently that $\gamma (s)f=\delta (s^{-1})f$ for all $s\in G$.

#### Proposition 4 {#lie-ix-s8-prop-4 .statement tag=01H5}

Let $f\in L^2(G)$. Then $f$ is central if and only if $u(f)$ is a homothety for all $u\in \widehat{G}$. In that case

$$
\varepsilon_u\int
$$

$$
u(f) =f(g)\chi_u(g)dg \tag{19}
$$

$$
d(u)_G
$$

By Prop. 1 (no. 1), to say that $f$ is central means that $u(\gamma (s)f) =$ $u(\delta (s^{-1})f)$ for all $s\in G$ and all $u\in \widehat{G}$; but this can also be written as $u(s)u(f) =u(f)u(s)$ for all $s\in G$ and all $u\in \widehat{G}$ (formulas (12) and (13)), hence the first assertion of Prop. 4 (Schur’s lemma). If $u(f)$ is a homothety, then $u(f) =\lambda_u\varepsilon_u$ with

1 1 $\int$ 1 $\int$

$\lambda_u=$ Tr($u(f)$) $=f(g$)Tr($u(g)$)$dg=f(g)\chi_u(g)dg$.

$$
d(u)d(u)_Gd(u)_G
$$

Consequently, for $f\in$ ZL$^2(G)$ we have

$$
\varepsilon_u
$$

$$
u(f) =\langle \overline{\chi}_u|f\rangle \rangle \tag{20}
$$

$$
d(u)
$$

so

$$
(\varepsilon_u)
$$

$$
\overline{\mathscr{F}}(f) =\langle \chi_u|f\rangle \tag{21}
$$

$$
d(u)_{u\in\widehat{G}}
$$

with

$$
_2\varepsilon_{u2}
$$

$$
\|\overline{\mathscr{F}}(f)\|_2=\sum))))\langle \chi_u|f\rangle ))))_2=\sum|\langle \overline{\chi}_u|f\rangle |^2
$$

$$
d(u)
$$

$uu$

Conversely, if $\varphi$ is a square-integrable complex function on $\widehat{G}$, the element $(\frac{\varphi(u)}{d(u)}\varepsilon_u)_{u\in\widehat{G}}$ of $F( \widehat{G})$ belongs to $L^2( \widehat{G})$, and we have (formula (9))

$$
((\varphi (u)))(\varphi (u)-)
$$

$\mathscr{F}_u\varepsilon_u(g) =d(u$)Tr $\varepsilon_uu(g)^1=\varphi (u)\overline{\chi}_u(g)$,

$$
d(u)d(u)
$$

so

$$
\mathscr{F}((\varphi (u)\varepsilon_u))=\sum\varphi (u)\overline{\chi}_u \tag{22}
$$

$$
d(u)
$$

$u\in \widehat{G}$

Note, in particular, that formulas (20) and (21) give, for $u, v$ in $\widehat{G},^8$

$u(\overline{\chi}_v) = 0$ if $u\not=v$, (23)

$$
\varepsilon_u
$$

$u(\overline{\chi}_u) =\in$ End(E$_u)$, (24)

$$
d(u)
$$

$\overline{\mathscr{F}}(\chi_u) =\varepsilon^u\in$ End(E$_u)\subset F( \widehat{G})$. (25)

$$
d(u)
$$

#### Proposition 5 {#lie-ix-s8-prop-5 .statement tag=01H6}

Let $f$ be a continuous central function on G. Then $f$ is infinitely-differentiable if and only if the function $u \rightarrow  |\langle \chi_u|f\rangle |$ is rapidly decreasing on $\widehat{G}$; in that case,

$$
f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)
$$

for all $g\in G$.

By Th. $1b)$, the function $\overline{f}$ is infinitely-differentiable if and only if the function $u \rightarrow  \|u(\overline{f})\|_{\infty}$ is rapidly decreasing; but, by (20),

$\|u(\overline{f})\|_{\infty}=$ 1 $|\langle \chi_u|f\rangle |$,

$$
d(u)
$$

hence the first assertion, since the functions $d(u)$ and $\frac{1}{d(u)}$ are moderately increasing.

Assume that $f$ is infinitely-differentiable; by Th. $1a),f(g) =\sum_{u\in\widehat{G}}f_u(g)$ for all $g\in G$, so

$$
_-(_-\varepsilon_u)
$$

$f_u(g) =\langle u(g)|u(f)\rangle =d(u$)Tr($u(g)^1.u(f)$) $=d(u$)Tr $u(g)^1\langle \chi_u|f\rangle$

$$
d(u)
$$

$=\langle \overline{\chi}_u|f\rangle$Tr($u(g)^{-1}$) $=\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$.

Hence, $f(g) =\sum_{u\in\widehat{G}}\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$; but, for all $u\in \widehat{G}$, the contragredient representation $u'$ of $u$ satisfies $\overline{\chi}_u=\chi_{u'}$ and the map $u \rightarrow u'$ is a permutation of $\widehat{G}$; so we also have $f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)$, hence the proposition.

$^8$ We embed End(E$_u)$ in the product $F( \widehat{G}) =\prod_{v\in\widehat{G}}$ End(E$_v)$ by associating to any

$A\in$ End(E$_u)$ the family $(A_v)_{v\in\widehat{G}}$ such that $A_u= A$ and $A_v= 0$ for $v\not=u$.

#### Corollary {#lie-ix-s8-n3-cor-1 .statement tag=01H7}

Let $f$ be a continuous central function on G. Then $f$ is infinitely-differentiable if and only if the restriction of $f$ to T is infinitely-differentiable.

Indeed, by Cor. 4 of §7, no. 4,

$\langle \chi_u|f\rangle =\int_G\overline{\lambda(u)(t)}\varphi (t)dt$, where $\varphi (t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})f(t)$.

If $f|T$ is infinitely-differentiable, so is $\varphi$; by Prop. 5, applied to the group T, the function $\mu \rightarrow \int_T\overline{\mu(t)}\varphi (t)dt$ on $\widehat{T} = X(T)$ is then rapidly decreasing, and so is the function $u \rightarrow  \langle \chi_u|f\rangle$; hence the function $f$ is infinitely-differentiable (Prop. 5). The converse is clear.

### 4. CENTRAL FUNCTIONS ON G AND FUNCTIONS ON T

Denote by $\mathscr{C}(G)$ the space of continuous complex-valued functions on G and by $\mathscr{C}^{\infty}(G)$ the subspace of infinitely-differentiable functions. Then we have a sequence of inclusions

$$
\Theta (G)\subset \mathscr{C}^{\infty}(G)\subset \mathscr{C}(G)\subset L^2(G)
$$

Denote by $Z\Theta (G),Z\mathscr{C}^{\infty}(G),Z\mathscr{C}(G)$, ZL$^2$(G), respectively, the subspaces consisting of the central functions in these various spaces. Introduce similarly the spaces $\Theta (T),\mathscr{C}^{\infty}(T),\mathscr{C}(T),L^2(T)$; for any space E in this list, denote by $E^W$ (resp. $E^{-W})$ the subspace consisting of the invariant (resp. anti-invariant) elements for the operation of the Weyl group W. We have a commutative diagram

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W
$$

where the vertical arrows represent the canonical injections, and the maps $a_c, a_{\infty}, a_{\Theta}$ are induced by the restriction map from $\mathscr{C}(G)$ to $\mathscr{C}(T)$.

The maps $a_c, a_{\infty}, a_{\Theta}$ are bijective (§2, no. 5, Cor. 1 of Prop. 5, §8, no. 3, Cor. of Prop. 5, and §7, no. 3, Cor. of Prop. 2).

Assume now that the semi-sum $\rho$ of the positive roots belongs to X(T) and consider the map $b$ which to every continuous function $\varphi$ on T associates $\varphi .J(\rho )$. We have a commutative diagram

ZL$^2(G)--------------------\longrightarrow^uL^2(T)^{-W}$

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W\longrightarrow^{b_c}\mathscr{C}(T)^{-W}
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W\longrightarrow^{b_{\infty}}\mathscr{C}^{\infty}(T)^{-W}
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W\longrightarrow^{b_{\Theta}}\Theta (T)^{-W}
$$

where the vertical arrows are the canonical inclusions, the maps $b_c, b_{\infty}, b_{\Theta}$ are induced by $b$, and $u$ extends $b_c\circ a_c$ by continuity (§7, no. 4, Cor. 3 of Th. 2). The maps $u$ and $b_{\Theta}$ are bijective (loc. cit.); so is $b_{\infty}$ (Exerc. 5); on the other hand, $b_c$ is not surjective in general (Exerc. 6).

### Exercises {#lie-ix-s8-exercises}

See the [exercises for § 8](exercises/s8/).
