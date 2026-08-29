---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 2
section_title: Exemples d’applications linéaires compactes
lang: en
source: ts-iii-v-fr
book_pages: TS III.23-TS III.39, TS III.118-TS III.120
pdf_pages: 0037-0053, 0132-0134
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes de trace finie, de Hilbert–Schmidt et de puissance $p^{\mathbf{e}}$ nucléaire
      page: 23
      pdf_page: 37
    - "no": 2
      title: Opérateurs diagonaux dans des espaces de suites
      page: 23
      pdf_page: 37
    - "no": 3
      title: Applications linéaires à valeurs dans un espace de fonctions continues définies par un noyau
      page: 25
      pdf_page: 39
    - "no": 4
      title: Applications linéaires entre espaces de Lebesgue définies par un noyau
      page: 26
      pdf_page: 40
    - "no": 5
      title: Restriction d’applications différentiables
      page: 34
      pdf_page: 48
    - "no": 6
      title: Restriction de sections différentiables d’un fibré vectoriel
      page: 35
      pdf_page: 49
    - "no": 7
      title: Restriction de sections analytiques d’un fibré vectoriel
      page: 37
      pdf_page: 51
statements: 26
exercises: 4
content_sha256: 4e5b73807c51c43f4658e3d4c0aa12802558831c80f1a39336cae718bffa14c0
translated_from: content/fr/ts/III/02_s2_exemples_d_applications_lineaires.md
source_lang: fr
translation_method: machine
source_content_sha256: ce4ce9d83c98563dff461a7865fc78d6acf0d80bc0a904609a959cabb48b3cf0
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-cccb3ab6
glossary_version: 34
glossary_terms_sha256: dd8e6c0df30e47d3aa54e0c099f26d3874e95d07c8bbec6487a404817945e7fb
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. EXAMPLES OF COMPACT LINEAR MAPPINGS

### 1. Endomorphisms of finite trace, of Hilbert–Schmidt, and of nuclear power $p^{\mathbf{e}}$

*Let E and F be Hilbert spaces. Every endomorphism of E of finite trace (EVT, V, p. 49, Def. 7 and p. 50, Def. 8) is compact (IV, p. 165, Corollary 1); every Hilbert–Schmidt mapping of E into F (EVT, V, p. 51, Def. 9) is compact (IV, p. 165, Corollary 2).

For every real number $p\geqslant 1$, the vector space $\mathscr{L}_p(E; F)$ of linear mappings of E into F of nuclear power $p^e$ is contained in $\mathscr{L}^c(E; F) ($cf. IV, p. 169, Remark 2 for $p= 1).*$

### 2. Diagonal operators in spaces of sequences

Let I be a nonempty set. Recall (EVT, I, p. 4 and p. 5) that the vector space of bounded families $x= (x_i)_{i\in I}$ of elements of $\mathbf{C}$, endowed with the norm $\|x\|=$ sup$_i|x_i|$, is a Banach space denoted by $\ell^{\infty}_{\mathbf{C}}(I)$.

Let $p$ be an element of $[1,+\infty [$. The space $\ell^p_{\mathbf{C}}(I)$ of families $x= (x_i)_{i\in I}$ of elements of $\mathbf{C}$ such that the family $(|x_i|^p)$ is summable is a vector space on which the mapping $x\mapsto  \|x\|= (\sum_i|x_i|^p)^{1/p}$ is a norm which makes it into a Banach space. If one endows the space I with the discrete topology and with the measure for which $\mu(\{x\}) = 1$ for every $x\in I$, this space is none other than the Banach space $L^p_{\mathbf{C}}(I, \mu)$. When $p= 1$ or $p= 2$, this notation thus coincides with that of EVT, I, p. 4 and EVT, V, p. 18 (cf. INT, IV, p. 141, §4, No.$^o1$, example).

For families $x= (x_i)_{i\in I}$ and $y= (y_i)_{i\in I}$ of complex numbers, one denotes by $xy$ the family $(x_iy_i)_{i\in I}$.

#### Proposition 1 {#ts-iii-s2-prop-1 .statement tag=02QK}

Let $\lambda = (\lambda_i)_{i\in I}$ be a bounded family of elements of $\mathbf{C}$. Let $p$ be an element of $[1,+\infty ]$. Let E be the Banach space $\ell^p_{\mathbf{C}}(I)$.

a) For every $x\in E$, one has $\lambda x\in E$ and the mapping $u:x\mapsto \lambda x$ is a continuous endomorphism of E, whose spectrum in the Banach algebra $\mathscr{L}(E)$ is equal to the closure in $\mathbf{C}$ of the set of the $\lambda_i$, and whose norm is equal to sup$_i|\lambda_i|$;

b) The endomorphism $u$ is compact if and only if for every real number $\varepsilon  >0$, the set of elements $i\in I$ such that $|\lambda_i|\geqslant \varepsilon$ is finite.

With the notation of the proposition, the endomorphism $x\mapsto \lambda x$ is called a diagonal endomorphism of $\ell^p_{\mathbf{C}}(I)$.

Let us prove the proposition. Let C = sup$_i|\lambda_i|$. Let $x\in E$. One has the inequalities

$\sum_{i\in I}|\lambda_ix_i|^p\leqslant C^p\|x\|^p$, if $p\not = +\infty$

sup$_{i\in I}|\lambda_ix_i|\leqslant C\|x\|$, if $p= +\infty$.

This proves that $\lambda x\in E$. The mapping $x\mapsto \lambda x$ is therefore an endomorphism of E, and these inequalities prove that it is of norm $\leqslant C$.

For $j\in I$, denote by $e_j$ the element $(x_i)_{i\in I}$ of $\ell^p_{\mathbf{C}}(I)$ such that $x_j= 1$ and $x_i= 0$ if $i\not =j$. We then have $u(e_j) =\lambda_je_j$ for all $j\in I$, which shows that $\lambda_j$ belongs to the spectrum of $u$. Since the spectrum of $u$ is closed, the closure in $\mathbf{C}$ of the set of the $\lambda_i$ is contained in the spectrum of $u$. Since the spectrum of $u$ is contained in the disk centered at 0 and of radius $\|u\|($I, p. 24, Theorem 1 and formula (3) of I, p. 21), we deduce the inequality $C\leqslant \|u\|$, whence $\|u\|= C$.

Conversely, if $\lambda \in \mathbf{C}$ is not adherent to the set of the $\lambda_i$, then the family $((\lambda_i-\lambda )^{-1})_{i\in I}$ is bounded. What precedes therefore shows that the linear mapping $x\mapsto ((\lambda -\lambda_i)^{-1}x_i)_{i\in I}$ is an endomorphism of E. It is inverse to $u-\lambda 1_E$, and hence $\lambda$ does not belong to the spectrum of $u$. This proves a).

Let us now prove b). Suppose that the endomorphism $u$ is compact. Let $\varepsilon  >0$. Denote by J the set of the $i\in I$ such that $|\lambda_i|\geqslant \varepsilon$. The set of elements $e_i$ for $i\in J$ is bounded in E. Its image by $u$, formed by the elements $\lambda_ie_i$ for $i\in J$, is therefore relatively compact in E (Remark 1 of III, p. 2). Since $\|\lambda_ie_i-\lambda_je_j\|\geqslant \varepsilon$ for every pair of elements $i\not =j$ in J, this is possible only if the set J is finite.

Let us prove the converse assertion. Let J be a finite subset of I and denote by $z_J= (z_{J,i})_{i\in I}$, where $z_{J,i}=\lambda_i$ for $i\in J$ and $z_{J,i}= 0$ for $i\in I$- J ; the family $z_J$ defines an endomorphism of finite rank $u_J:x\mapsto z_Jx$ of E. According to what precedes, the norm of the linear mapping $u-u_J$ is bounded above by the upper bound in $\mathbf{R}_+$ of the family $(|\lambda_i|)_{i\in I-J}$. The assumption implies that for every $\varepsilon  >0$, there exists a finite subset $J\subset I$ such that this upper bound is $\leqslant \varepsilon$. It follows that the mapping $u$ is adherent to $\mathscr{L}^f$(E), and hence that it is compact (III, p. 4, cor. of Prop. 2).

#### Remark 1 {#ts-iii-s2-n2-rem-1 .statement tag=02QL}

The assumption of assertion b) is always valid if I is finite. When the set I is infinite, it means that the family $(\lambda_i)_{i\in I}$ tends to 0 according to the filter of complements of finite subsets of I; in particular, the set of the $i\in I$ such that $\lambda_i\not = 0$ is then countable.

#### Remark 2 {#ts-iii-s2-n2-rem-2 .statement tag=02QM}

*It will be seen later (cf. IV, p. 149, theorem 1) that when $p= 2$, every normal compact endomorphism of the Hilbert space $\ell^2_{\mathbf{C}}(I)$ is of the form $u=w\circ v\circ w^{-1}$, where $v$ is a diagonal compact endomorphism and $w$ is a unitary endomorphism (EVT, V, p. 40) of the Hilbert space $\ell^2_{\mathbf{C}}(I).*$

### 3. Linear mappings with values in a space of continuous functions defined by a kernel

We take here $K =\mathbf{C}$. Let X and Y be locally compact topological spaces. Let $\mu$ be a complex measure on X and $k$ a mapping of $X\times Y$ into $\mathbf{C}$ having the following two properties:

(i) For every $y\in Y$, the function $k_y:x\mapsto k(x, y)$ of X into $\mathbf{C}$ is $\mu$-integrable;

(ii) The mapping $y\mapsto k_y$ of Y into $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ is continuous.

Endow the space $\mathscr{C}(Y)$ of continuous functions on Y with complex values with the topology of compact convergence. For $f$ in $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, define $\widetilde{k}(f) : Y\rightarrow \mathbf{C}$ by

$$
\widetilde{k}(f)(y) =\int_Xk(x, y)f(x)d\mu(x) =\int_Xk_yf d\mu \tag{1}
$$

The mapping $h\mapsto \int_Xhf d\mu$ is a continuous linear form on $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$, so condition (ii) shows that the function $\widetilde{k}(f)$ is continuous.

#### Proposition 2 {#ts-iii-s2-prop-2 .statement tag=02QN}

The mapping $\widetilde{k}$ of $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ into $\mathscr{C}(Y)$ is compact.

For every $y$ and $y'$ in Y, one has

$$
|\widetilde{k}(f)(y)|\leqslant \|k_y\|_1\|f\|_{\infty},|\widetilde{k}(f)(y)-\widetilde{k}(f)(y')|\leqslant \|k_y-k_{y'}\|_1\|f\|_{\infty}
$$

By Ascoli's theorem (TG, X, p. 18, cor. 2), it follows that the image under $\widetilde{k}$ of the unit ball of $\mathscr{L}_{\mathbf{C}}^{\infty}(X;\mu)$ is relatively compact in $\mathscr{C}(Y)$.

#### Corollary {#ts-iii-s2-n3-cor-1 .statement tag=02QO}

Let X be a compact topological space, Y a locally compact topological space, $\mu$ a complex measure on X, and $k$ a continuous mapping of $X\times Y$ into $\mathbf{C}$. Then formula (1) defines a compact linear mapping, again denoted by $\widetilde{k}$, of $\mathscr{C}(X)$ endowed with the topology of uniform convergence into $\mathscr{C}(Y)$ endowed with the topology of compact convergence.

Let us verify conditions (i) and (ii) for $k$. For every $y\in Y$, the mapping $k_y$ is continuous on the compact space X, hence $\mu$-integrable. Moreover, the mapping $y\mapsto k_y$ is continuous from Y into $\mathscr{C}(X)$ since X is compact (TG, X, p. 28, th. 3). Since $\|k_y-k_{y'}\|_1\leqslant \|\mu\| \|k_y-k_{y'}\|$ for every $(y, y')\in Y^2$, this mapping of Y into $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ is continuous. By prop. 2, the mapping $\widetilde{k}$ of $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ into $\mathscr{C}(Y)$ is compact. By composition with the canonical mapping $\mathscr{C}(X)\rightarrow \mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, one obtains a compact linear mapping of $\mathscr{C}(X)$ into $\mathscr{C}(Y)$.

### 4. Linear mappings between Lebesgue spaces defined by a kernel

Here we take $K =\mathbf{C}$. Let X be a locally compact topological space endowed with a positive measure $\mu$. For every $r\in [1,+\infty ]$, we write $\mathscr{L}^r(X) =\mathscr{L}_{\mathbf{C}}^r(X, \mu)$ and $L^r(X) = L^r_{\mathbf{C}}(X, \mu)$. When $r\in [1,+\infty [$, we identify the dual of $L^r(X)$ with $L^{r'}(X)$, where $r'$ is the conjugate exponent of $r$, such that $1/r+ 1/r'= 1$ (INT, V, p. 61, § 5, n$^o8$, th. 4). We write $\|f\|_r$ for the norm (or semi-norm) of $f\in L^r(X)$ (or $f\in \mathscr{L}^r(X)$).

We recall that a subset A of X is said to be $\mu$-moderate (INT, V, p. 4, § 1, n$^o2$) if it is contained in the union of a sequence of $\mu$-integrable sets, and that a function $f$ defined on X with values in a vector space or in $\overline{\mathbf{R}}$ is $\mu$-moderate if it is zero in the complement of a $\mu$-moderate subset of X. If 1 $\leqslant p <+\infty$ and $f\in \mathscr{L}^p$(X), then $f$ is moderate (INT, V, p. 9, § 1, n$^o3$, cor.). If $f$ is $\mu$-moderate, then $f g$ is $\mu$-moderate for every function $g$.

Let $p$ and $q$ be elements of$]1,+\infty [$. Let X and Y be locally compact topological spaces, endowed with positive measures $\mu$ and $\nu$, respectively. We endow the space $X\times Y$ (resp. $Y\times X$) with the product measure $\mu\otimes \nu$ (resp. $\nu \otimes \mu$).

We write $\mathscr{N}^{p,q}(X\times Y, \mu\otimes \nu )$, or simply $\mathscr{N}^{p,q}(X\times Y)$, for the set of $(\mu\otimes \nu$)-measurable mappings $k$ from $X\times Y$ into $\mathbf{C}$ such that there exists a real number $C\geqslant 0$ satisfying

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )(x, y)\leqslant C\|f\|_p\|g\|_q \tag{2}
$$

for all functions $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^q(Y)$. We then write $\|k\|_{p,q}$ for the greatest lower bound of the set of real numbers C having this property.

#### Remark {#ts-iii-s2-n4-rem-1 .statement tag=02QP}

Let $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^q(Y)$. Since $p <+\infty$ and $q <+\infty$, the functions $f$ and $g$ are moderate, and the function defined by $(x, y)\mapsto f(x)g(y)$ is $(\mu\otimes \nu$)-moderate (cf. INT, V, p. 92, § 8, n$^o3$, Corollary 2). Consequently, the function $(x, y)\mapsto k(x, y)f(x)g(y)$ is $(\mu\otimes \nu$)-moderate, and in particular the upper integral of its absolute value coincides with the essential upper integral (INT, V, p. 6, § 1, n$^o3$, Proposition 7).

The set $\mathscr{N}^{p,q}(X\times Y)$ is a vector subspace of the space of functions from $X\times Y$ into $\mathbf{C}$ and the mapping defined by $k\mapsto  \|k\|_{p,q}$ is a semi-norm on $\mathscr{N}^{p,q}(X\times Y)$.

#### Lemma 1 {#ts-iii-s2-lem-1 .statement tag=02QQ}

Let $k\in \mathscr{N}^{p,q}(X\times Y)$. The function $k$ is locally $(\mu\otimes \nu )$-integrable.

The mapping $k$ is $(\mu\otimes \nu$)-measurable by hypothesis. Let A be a compact subset of $X\times Y$. There exist compact subsets $B\subset X$ and $C\subset Y$ such that $A\subset B\times C$. Applying (2) to the characteristic functions $\varphi_B$ of B and $\varphi_C$ of C, one obtains

$$
\int_{X\times Y}^*|k(x, y)|\varphi_A(x, y)d(\mu\otimes \nu )(x, y)
$$

$$
\leqslant \int_{X\times Y}^*|k(x, y)|\varphi_B(x)\varphi_C(y)d(\mu\otimes \nu )(x, y)<+\infty
$$

whence the result (INT, V, p. 41, §5, n$^o1$, Proposition 1 and Definition 1).

#### Proposition 3 {#ts-iii-s2-prop-3 .statement tag=02QR}

a) Let $k\in \mathscr{N}^{p,q}(X\times Y)$. For $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^q(Y)$, the function

$$
(x, y)\mapsto k(x, y)f(x)g(y)
$$

is $(\mu\otimes \nu )$-integrable and there exists a unique mapping $u_k$ from $L^p(X)$ into $L^{q'}(Y)$ such that

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

for all $f\in L^p(X)$ and $g\in L^q(Y)$. The mapping $u_k$ is linear and continuous, and its norm is $\leqslant \|k\|_{p,q}$;

b) Let $k\in \mathscr{N}^{p,q}(X\times Y)$. One has $u_k= 0$ if and only if $k$ is locally $(\mu\otimes \nu )$-negligible;

c) The mapping which associates $u_k$ with $k$ is a continuous linear mapping of the semi-normed space $\mathscr{N}^{p,q}(X\times Y)$ into the Banach space $\mathscr{L}(L^p(X); L^{q'}(Y))$, such that $\|u_k\|\leqslant \|k\|_{p,q}$ for every $k\in \mathscr{N}^{p,q}(X\times Y)$.

Let $k\in \mathscr{N}^{p,q}(X\times X)$. By definition, the function from $X\times Y$ into $\mathbf{C}$ defined by $(x, y)\mapsto k(x, y)f(x)g(y)$ is $(\mu\otimes \nu$)-integrable when $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^q$(Y), and the mapping

$$
b_k: (f, g)\mapsto \int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

is a continuous bilinear mapping from $L^p(X)\times L^q(Y)$ into $\mathbf{C}$. For every $f\in L^p$(X), there therefore exists a unique $h\in L^{q'}(Y)$ such that $b_k(f, g) =$ $\langle g, h\rangle$ for every $g\in L^q(Y)$; let us write $u_k(f) =h$. By (2), one has $\|u_k(f)\|_{q'}\leqslant \|k\|_{p,q}\|f\|_p$; the mapping $u_k$ is linear and continuous, of norm $\leqslant \|k\|_{p,q}$. Moreover, the mapping $k\mapsto u_k$ is linear, and assertions a) and c) follow from this.

Let us prove b). Suppose that $k$ is locally $(\mu\otimes \nu$)-negligible. Let $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^q(Y)$; the function defined on $X\times Y$ by $(x, y)\mapsto k(x, y)f(x)g(y)$ is $(\mu\otimes \nu$)-moderate. Since it is locally $(\mu\otimes \nu$)-negligible, it is negligible (INT, V, p. 7, § 1, No.$^o2$, Corollary 1). Thus, one has $\langle u_k(f), g\rangle =b_k(f, g) = 0$. It follows that $u_k= 0$.

Conversely, let $k\in \mathscr{N}^{p,q}(X\times Y)$ be such that $u_k= 0$. The function $k$ is locally $(\mu\otimes \nu$)-integrable (Lemma 1). For all functions $f\in \mathscr{K}(X)$ and $g\in \mathscr{K}$ (Y), one has

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}f(x)g(y)k(x, y)d(\mu\otimes \nu )(x, y)
$$

therefore the measure $k\cdot (\mu\otimes \nu )$ on $X\times Y$ is zero (cf. INT, III, p. 82, § 4, No.$^o1$, Theorem 1). This means that $k$ is locally $(\mu\otimes \nu$)-negligible (INT, V, p. 46, §5, No.$^o3$, Corollary 2).

#### Definition 1 {#ts-iii-s2-def-1 .statement tag=02QS}

Let $k\in \mathscr{N}^{p,q}(X\times Y)$. One says that the mapping $u_k$ is the integral operator with kernel $k$ from $L^p(X)$ into $L^{q'}(Y)$.

For $k\in \mathscr{N}^{p,q}(X\times Y)$ and $f\in \mathscr{L}^p$(X), one will sometimes also denote by $u_k(f)$ the image under $u_k$ of the class of $f$ in $L^p(X)$.

#### Proposition 4 {#ts-iii-s2-prop-4 .statement tag=02QT}

Let $k\in \mathscr{N}^{p,q}(X\times Y)$ and $f\in \mathscr{L}^p(X)$. The mapping defined on X by $x\mapsto k(x, y)f(x)$ is $\mu$-integrable for every $y$ outside a locally $\nu$-negligible set, and $u_k(f)$ coincides with the class of the function

$$
y\mapsto \int_Xk(x, y)f(x)d\mu(x)
$$

defined locally $\nu$-almost everywhere.

Let $Y'$ denote the set of $y\in Y$ such that the mapping $x\mapsto k(x, y)f(x)$ is not $\mu$-integrable. Let $y\in Y$ and let C be a compact neighbourhood of $y$, whose characteristic function is denoted by $\varphi$. By condition (2) applied to $f$ and $\varphi$, the function $(x, y)\mapsto k(x, y)f(x)\varphi (y)$ is integrable on $X\times Y$ with respect to the measure $\mu\otimes \nu$. By the Lebesgue-Fubini theorem (INT, V, p. 96, § 8, No.$^o4$, Theorem 1, a)), the function $x\mapsto k(x, y)f(x)\varphi (y)$ is $\mu$-integrable for $y$ outside a $\nu$-negligible set $Y_C$. Since $Y'\cap C\subset Y_C$, it follows that $Y'$ is locally $\nu$-negligible in Y (INT, IV, p. 172, § 5, No.$^o2$, Definition 3).

Let $h$ denote the mapping defined locally $\nu$-almost everywhere on Y by $y\mapsto \int k(x, y)f(x)d\mu$. It is locally $\nu$-integrable (INT, V, loc. cit.). Let $g\in \mathscr{K}(Y)$. We have

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

$$
=\int_Y\int_Xk(x, y)f(x)g(y)d\mu(x)d\nu (y)
$$

$$
=\int_Yg(y)h(y)d\nu (y)
$$

(INT, V, loc. cit.). Hence $u_k(f) =h$ locally $\nu$-almost everywhere (cf. INT, V, p. 46, § 5, No.$^o3$, Corollary 2).

#### Proposition 5 {#ts-iii-s2-prop-5 .statement tag=02QU}

The space $\mathscr{L}^{p'}(X\times Y)$ is contained in $\mathscr{N}^{p,p}(X\times Y)$. The linear mapping from $\mathscr{L}^{p'}(X\times Y)$ into $\mathscr{L}(L^p(X); L^{p'}(Y))$ defined by $k\mapsto u_k$ induces, after passing to the quotient, a continuous injective linear mapping from $L^{p'}(X\times Y)$ into $\mathscr{L}(L^p(X); L^{p'}(Y))$.

Let $k\in \mathscr{L}^{p'}(X\times Y)$. The mapping $k$ is measurable (INT, IV, p. 84, § 5, No.$^o6$, Theorem 5). Let $f\in \mathscr{L}^p(X)$ and $g\in \mathscr{L}^p(Y)$. The function $h: (x, y)\mapsto f(x)g(y)$ belong to $\mathscr{L}^p(X\times Y)$ and $\|h\|_p=\|f\|_p\|g\|_p$ (INT, V, p. 95, § 8, No.$^o3$, Corollary 2). The function $hk$ is therefore integrable on $X\times Y$ and we have

$$
(\mu\otimes \nu )^*(|hk|)\leqslant \|k\|_{p'}\|h\|_p=\|k\|_{p'}\|f\|_p\|g\|_p
$$

by Hölder's inequality (INT, IV, p. 208, § 6, No.$^o4$, Theorem 2), which proves that $k\in \mathscr{N}^{p,p}(X\times Y)$ with $\|k\|_{p,p}\leqslant \|k\|_{p'}$.

Since $p'\not = +\infty$, every function $k\in \mathscr{L}^{p'}(X\times Y)$ is moderate (INT, V, p. 9, § 1, No.$^o3$, Corollary), and the last assertion then results from Proposition 3, b) and c).

For every function $k: X\times Y\rightarrow \mathbf{C}$ and every $y\in Y$, we denote by $k_y$ the mapping of X into $\mathbf{C}$ defined by $k_y(x) =k(x, y)$, and we denote by $k_{\circ}$ the mapping of Y into $\mathscr{F}(X;\mathbf{C})$ defined by $y\mapsto k_y$. Analogously, we shall denote by the same symbol the mapping of Y into the space of functions defined $\mu$-almost everywhere on X which associates to $y$ the class of $k_y$.

For every function $k$ of $X\times Y$ into $\mathbf{C}$, we put

$$
N_{p',q'}(k)=\left(\int_Y^\bullet N_{p'}(k_y)^{q'}d\nu(y)\right)^{1/q'}.
$$

It is an element of $[0,+\infty ]$.

#### Lemma 2 {#ts-iii-s2-lem-2 .statement tag=02QV}

For every $k\in \mathscr{L}^{p'}(X\times Y)$, one has $N_{p', p'}(k) =\|k\|_{p'}$.

Let $k\in \mathscr{L}^{p'}(X\times Y)$. By INT, V, p. 96, § 8, No.$^o4$, Theorem 1, a), the set $Y'$ of elements $y\in Y$ such that the function $|k_y|^{p'}$ is not $\mu$-integrable is $\nu$-negligible; moreover, the function defined by $y\mapsto \mu(|k_y|^{p'})$ on Y - $Y'$ and zero on $Y'$ is $\nu$-integrable and satisfies

$$
\|k\|^{p'}_{p'}=\int_{X\times Y}|k(x, y)|^{p'}d(\mu\otimes \nu )(x, y) =\int_Y\mu(|k_y|^{p'})d\nu = N_{p', p'}(k)^{p'}
$$

We denote by $\mathscr{L}^{p',q'}(X,Y, \mu, \nu )$, or simply by $\mathscr{L}^{p',q'}(X,Y)$, the complex vector space of $(\mu\otimes \nu$)-measurable functions $k$ of $X\times Y$ into $\mathbf{C}$ such that, for $\nu$-almost every $y\in Y$, the mapping $k_y$ belongs to $\mathscr{L}^{p'}$(X), and such that the mapping $k_{\circ}$ belongs to $\mathscr{L}_{L^{p'}(X)}^{q'}(Y, \nu )$ (INT, IV, p. 129, § 3, No.$^o4$, Definition 2). We endow $\mathscr{L}^{p',q'}(X,Y)$ with the seminorm $k\mapsto N_{p',q'}(k)$; note that one then has $N_{p',q'}(k) =\|k_{\circ}\|_{q'}$, where $k_{\circ}$ is regarded as a mapping with values in the Banach space $L^{p'}(X)$.

#### Proposition 6 {#ts-iii-s2-prop-6 .statement tag=02QW}

a) The space $\mathscr{L}^{p'}(X\times Y)$ is contained in $\mathscr{L}^{p',p'}(X,Y)$, and for $k\in \mathscr{L}^{p'}(X\times Y)$, one has $N_{p', p'}(k) =\|k\|_{p'}$;

b) The space $\mathscr{L}^{p',q'}(X,Y)$ is contained in $\mathscr{N}^{p,q}(X\times Y)$ and for $k\in \mathscr{L}^{p',q'}(X,Y)$, one has $\|k\|_{p,q}\leqslant N_{p',q'}(k)$.

Let us prove assertion a). Let $k\in \mathscr{L}^{p'}(X\times Y)$. By INT, V, p. 96, § 8, n$^o4$, th. 1, a), the function $k_y$ belongs to $\mathscr{L}^{p'}(X)$ for $\nu$-almost all $y\in Y$.

Let $\varepsilon  >0$. There exists $h\in \mathscr{K}(X\times Y)$ such that $\|k-h\|_{p'}< \varepsilon$. The function $h_{\circ}$ is a continuous function with compact support from Y into $L^{p'}(X)$ satisfying

$$
\|k_{\circ}-h_{\circ}\|_{p'}= N_{p',p'}(k-h) =\|k-h\|_{p'}< \varepsilon
$$

by Lemma 2. It follows that $k_{\circ}$ belongs to $\mathscr{L}_{L^{p'}(X)}^{p'}(Y, \nu )$, that is to say that $k$ belongs to $\mathscr{L}^{p',p}(X,Y)$. Lemma 2 then proves that $N_{p', p'}(k) =\|k\|_{p'}$.

Let us prove assertion b). Let $k\in \mathscr{L}^{p',q'}(X,Y)$ and let $f\in \mathscr{L}^p(X)$. For every $y\in Y$, Hölder's inequality (INT, IV, p. 208, § 6, n$^o4$, th. 2) applied to $k_y$ implies

$$
\int_X^*|k(x, y)f(x)|d\mu(x)\leqslant \|k_y\|_{p'}\|f\|_p
$$

Let $g\in \mathscr{L}^{q'}(Y)$. The mappings $f$ and $g$ are moderate, since $p$ and $q'$ are finite. Consequently, the mapping $(x, y)\mapsto f(x)g(y)$ is $(\mu\otimes \nu )$-moderate (cf. INT, V, p. 92, § 8, n$^o3$, cor. 2), and therefore the mapping $(x, y)\mapsto k(x, y)f(x)g(y)$ is $(\mu\otimes \nu$)-moderate. By INT, V, p. 93, § 8, n$^o3$, prop. 7, a), it follows that

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )
$$

$$
=\int_Y^*|g(y)|(\int_X^*|k(x, y)f(x)|d\mu(x))d\nu (y)
$$

$$
\leqslant \|f\|_p\int_Y^*\|k_y\|_{p'}|g(y)|d\nu (y)\leqslant N_{p',q'}(k)\|f\|_p\|g\|_q
$$

again using Hölder's inequality. This concludes the proof.

#### Proposition 7 {#ts-iii-s2-prop-7 .statement tag=02QX}

Let $k\in \mathscr{L}^{p',q'}(X,Y)$. The linear mapping $u_k$ of $L^p(X)$ into $L^{q'}(Y)$ is compact.

Suppose first that $k$ is such that $k_{\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}$(X)), and denote by A the support of $k_{\circ}$. Let F be the subspace of $\mathscr{K}(Y,A;\mathscr{L}^{p'}(X, \mu))$ generated by the functions $y\mapsto f_2(y)f_1$, where $f_2\in \mathscr{K}(Y,A)$ and $f_1\in \mathscr{L}^{p'}(X)$. When $m\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ satisfies $m_{\circ}\in F$, the linear mapping $u_m$ is of finite rank, therefore compact. For $m_1$ and $m_2$ in $\mathscr{K}(Y,A;\mathscr{L}^{p'}$(X)), one has moreover

$\int'1/q'$

$$
\|u_{m_1}-u_{m_2}\|\leqslant \|m_1-m_2\|_{p',q'}=(_Y\|m_{1,y}-m_{2,y}\|^q_{p'}d\nu (y))
$$

$\leqslant \nu (A)^{1/q'}$ sup$_{y\in Y}N_{p'}(m_{1,y}-m_{2,y})$.

Since the space F is dense in $\mathscr{K}(Y,A; L^{p'}(X))$ for the topology of uniform convergence in A (INT, III, p. 41, § 1, n$^o1$, prop. 1 and INT, III, p. 46, § 1, n$^o2$, prop. 5), it follows that the linear mapping $u_k$ is the limit of a sequence of linear mappings of finite rank. It is therefore compact (cor. 1 of III, p. 4).

Consider the general case. Let $k\in \mathscr{L}^{p',q'}(X,Y)$. For every $\varepsilon  >0$, there exists a mapping $k_{\varepsilon ,\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ such that

$$
\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

The corresponding function $k_{\varepsilon}: X\times Y\rightarrow \mathbf{C}$ then satisfies

$$
\|u_k-u_{k_{\varepsilon}}\|\leqslant \|k-k_{\varepsilon}\|_{p,q}\leqslant N_{p',q'}(k-k_{\varepsilon}) =\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

Since $u_{k_{\varepsilon}}$ is compact by what precedes, the mapping $u_k$ is likewise compact (prop. 2 of III, p. 4).

Put $p= 1$ and suppose $q >1$. There may exist mappings $k: X\times Y\rightarrow \mathbf{C}$ such that $k_y\in \mathscr{L}^{\infty}(X)$ for every $y\in Y$, and such that the integral

$$
\int_Y^*\|k_y\|^{q'}_{\infty}d\nu (y)
$$

is finite (in particular, condition (2) of III, p. 27 is valid), but such that the linear mapping $u_k$ from $L^1(X)$ into $L^{q'}(X)$ is not compact (exercise 2 of III, p. 119).

In particular, one deduces from the proposition the following corollary:

#### Corollary 1 (Hilbert–Schmidt) {#ts-iii-s2-prop-7-cor-1 .statement tag=02QY}

Let $k\in \mathscr{L}^2(X\times Y)$. The linear mapping $u_k$ is compact from $L^2(X)$ into $L^2(Y)$.

By prop. 5, one has $k\in \mathscr{N}^{2,2}(X\times Y)$, hence the linear mapping $u_k$ is defined (prop. 3). One has $k\in \mathscr{L}^{2,2}(X\times Y)$ (prop. 6, a)), hence $u_k$ is compact (prop. 7).

#### Remark {#ts-iii-s2-n4-rem-2 .statement tag=02QZ}

In the case $p=q= 2$, it is generally more convenient to express the characterization of the integral operator $u_k$ by means of the scalar product: it is the unique mapping of $L^2(X)$ into $L^2(Y)$ such that

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)\overline{g(y)}d(\mu\otimes \nu )(x, y)
$$

for all $f\in L^2(X)$ and $g\in L^2(Y)$. Moreover, the adjoint of $u_k$ is the linear mapping $u_{k^*}$, where $k^*\in L^2(Y\times X)$ satisfies $k^*(y, x) =k(x, y)$ for almost every $(y, x)\in Y\times X$. In fact, for all $f\in L^2(X)$ and $g\in L^2$(Y), one has

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)\overline{g(y)}f(x)d(\mu\otimes \nu )(x, y) =\langle u_{k^*}(g)|f\rangle
$$

#### Corollary 2 {#ts-iii-s2-prop-7-cor-2 .statement tag=02R0}

Let G be a compact topological group endowed with a Haar measure $\mu$. Let $p$ be a real number such that $1< p <+\infty$ and $q$ the conjugate exponent of $p$. Let $f\in \mathscr{L}^q(G)$. Put $k(x, y) =f(x^{-1}y)$ for all $(x, y)\in G\times G$.

a) One has $k\in \mathscr{L}^{q,p}(G,G)$;

b) For $\varphi \in L^p(G)$, the convolution $\varphi *f$ belong to $L^p(G)$ and the linear mapping $v_f:\varphi \mapsto \varphi *f$ of $L^p(G)$ into itself is continuous. It coincides with the endomorphism $u_k$. In particular, the linear mapping $v_f$ is compact.

Since G is compact, the function $f$ belong to $\mathscr{L}^1(G)$. The linear mapping $v_f$ is therefore defined and continuous by INT, VIII, p. 167, § 4, No.$^o5$, Prop. 13.

The mapping $k$ is $(\mu\otimes \mu$)-measurable, and one has $\|k_y\|_q=\|f\|_q$ for every $y\in G$. Since the measure $\mu$ is bounded, it follows that

$$
\int_G\|k_y\|^p_qd\mu(y) =\mu(G)\|f\|^p_q
$$

hence $k\in \mathscr{L}^{q,p}(G,G)$. The linear mapping $u_k$ is therefore a compact linear mapping of $L^p(G)$ into $L^p(G)$ (Prop. 7).

Let $\varphi \in \mathscr{K}(G)$. By INT, VIII, p. 166, § 4, No.$^o5$, Prop. 11 and Prop. 4 of III, p. 29, one then has

$$
v_f(\varphi )(y) =\int_G\varphi (x)f(x^{-1}y)d\mu(x)
$$

$$
=\int_G\varphi (x)k(x, y)d\mu(x) =u_k(\varphi )(y)
$$

for almost every $y\in G$. This implies that $v_f=u_k$.

### 5. Restriction of differentiable mappings

Let $n$ and $r$ be positive integers, U an open subset of $\mathbf{R}^n$ and F a Banach space. Let us denote by $\mathscr{C}^r(U; F)$ the vector space of mappings of class $C^r$ of U into F, endowed with the topology of compact $C^r$-convergence. Let us recall that this is the upper bound of the topologies of uniform $C^r$-convergence on K (VAR, R2, 12.3.10, p. 56), when K runs through the set of compact subsets of U. The space $\mathscr{C}^0(U; F)$ is nothing but the space $\mathscr{C}(U; F)$ of continuous mappings of U into F, endowed with the topology of compact convergence.

#### Lemma 3 {#ts-iii-s2-lem-3 .statement tag=02R1}

Let A be the set of multi-indices $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant r$ and let $u$ be the linear mapping $f\mapsto (\partial^{\alpha}f)_{\alpha\in A}$ of $\mathscr{C}^r(U; F)$ into $\mathscr{C}(U; F)^A$.

a) The mapping $u$ is injective, continuous, strict, and its image is closed.

b) The topological vector space $\mathscr{C}^r(U; F)$ is complete.

The mapping $u$ is linear and injective. It is continuous and strict by definition of the topology of $\mathscr{C}^r(U; F)$.

Let $(g_{\alpha})_{\alpha\in A}$ be a point of $\mathscr{C}(U; F)^A$ adherent to the image of $u$. There exists a filter $\mathfrak{F}$ on $\mathscr{C}^r(U; F)$ such that one has $g_{\alpha}=$ lim$_{f,\mathscr{F}}\partial^{\alpha}f$ in $\mathscr{C}(U; F)$ for every $\alpha \in A$. Let $m$ be an integer such that $0\leqslant m\leqslant r$. Reasoning by induction on $m$, one deduces from Theorem 1 of FVR, II, p. 2, that the mapping $g_0$ is of class $C^m$ and that one has $g_{\alpha}=\partial^{\alpha}g_0$ for every $\alpha \in \mathbf{N}^n$ with $|\alpha |\leqslant m$. Thus $g_0$ belongs to the space $\mathscr{C}^r(U; F)$ and its image under $u$ is $(g_{\alpha})_{\alpha\in A}$. This proves that the image of $u$ is closed, and therefore establishes assertion a).

Assertion a) implies that the space $\mathscr{C}^r(U; F)$ is isomorphic to its image in $\mathscr{C}(U; F)^A$; since this image is closed and the space $\mathscr{C}(U; F)^A$ is complete (TG, X, p. 9, Corollary 3 of Theorem 2 and TG, II, p. 17, Proposition 10), the space $\mathscr{C}^r(U; F)$ is complete.

#### Proposition 8 {#ts-iii-s2-prop-8 .statement tag=02R2}

Suppose that F is finite-dimensional. Let $s$ be an integer such that $0\leqslant s < r$ and V a relatively compact open subset of U. The linear mapping $f\mapsto f|V$ of $\mathscr{C}^r(U; F)$ into $\mathscr{C}^s(V; F)$ is compact.

Let W be the set of functions $f\in \mathscr{C}^r(U; F)$ whose partial derivatives of order $\leqslant r$ take at every point of V a value of norm less than 1. The set W is a neighbourhood of 0 in the space $\mathscr{C}^r(U; F)$. Let $\alpha$ be a multi-index such that $|\alpha |\leqslant s$. Consider the set H of functions of the form $(\partial^{\alpha}f)|V$ for $f$ in W. The set H is an equicontinuous subset of $\mathscr{C}(V; F)$ (TG, X, p. 10) by the mean value theorem (VAR, R, 2.2.3). Moreover, for every $x\in V$, the image of H under the mapping $g\mapsto g(x)$ is a bounded subset, hence a relatively compact subset, of F. By Ascoli's theorem (TG, X, p. 18, Corollary 2), the set H is relatively compact in $\mathscr{C}(V; F)$. This proves that the linear mapping $f\mapsto (\partial^{\alpha}f)|V$ of $\mathscr{C}^r(U; F)$ into $\mathscr{C}(V; F)$ is compact. The proposition then follows from Lemma 3 and Remarks 5 and 6 of III, p. 3.

### 6. Restriction of differentiable sections of a vector bundle

Let $r$ be a positive integer, X a differentiable manifold of class $C^r$ locally of finite dimension and E a vector bundle (real or complex) with base X and of class $C^r$. For every open subset U of X, let us denote by $\mathscr{S}^r(U; E)$ the vector space (denoted by $\mathscr{S}_E^r(U)$ in VAR, R1, 7.4, p. 74) of sections of class $C^r$ of E over U, endowed with the topology of compact $C^r$-convergence.

#### Lemma 4 {#ts-iii-s2-lem-4 .statement tag=02R3}

Let $\mathscr{U}$ be an open covering of X. The mapping $u:f\mapsto (f|U)_{U\in\mathscr{U}}$ of $\mathscr{S}^r(X; E)$ into $\prod_{U\in\mathscr{U}}\mathscr{S}^r(U; E)$ is linear, injective, continuous and strict. Its image is closed.

The mapping $u$ is linear, injective and continuous. By virtue of TG, IX, p. 43, prop. 1 and p. 48, cor. 1, every compact subset of X has a finite covering $(C_i)_{i\in I}$ where, for each $i\in I$, the set $C_i$ is a compact subset of one of the open sets of the covering $\mathscr{U}$. It follows that the linear mapping $u$ is strict. Finally, its image is closed, since it consists of the families $(f_U)_{U\in\mathscr{U}}$ such that $f_U$ and $f_V$ coincide in $U\cap V$ for all U and V in $\mathscr{U}$.

#### Proposition 9 {#ts-iii-s2-prop-9 .statement tag=02R4}

The space $\mathscr{S}^r(X; E)$ is complete.

Suppose first that there exist an integer $n\geqslant 0$ and a Banach space F such that X is an open subset of $\mathbf{R}^n$ and E the trivial vector bundle $X\times F$ with base X and fibre F. In this case, the topological vector space $\mathscr{S}^r(X; E)$ is isomorphic to $\mathscr{C}^r(X; F)$, and the result follows from lemma 3 of III, p. 34.

In the general case, let $\mathscr{U}$ be an open covering of X by chart domains such that for every $U\in \mathscr{U}$, the restriction of E to U is trivializable. By the above lemma, the space $\mathscr{S}^r(X; E)$ is isomorphic to the image of the linear mapping $f\mapsto (f|U)_{U\in\mathscr{U}}$, which is closed in the product of the spaces $\mathscr{S}^r(U; E)$ for U in $\mathscr{U}$. By the preceding case, each of the spaces $\mathscr{S}^r(U; E)$ is complete, hence their product is complete (TG, II, p. 17, prop. 10). Consequently $\mathscr{S}^r(X; E)$ is complete.

#### Remark {#ts-iii-s2-n6-rem-1 .statement tag=02R5}

Let $\mathscr{U}$ be an open covering of X by chart domains $c_U= (U, \varphi_U,\mathbf{R}^{n_U})$ such that for every $U\in \mathscr{U}$, the restriction of E to U is trivializable of type $F_U$, where $F_U$ is a Banach space. For every $U\in \mathscr{U}$, a section $f$ of E over U is identified with a mapping $f_U$ of $\varphi_U(U)$ into $F_U$. It follows from the proof of prop. 9 that the topology of the space $\mathscr{S}^r(X; E)$ is defined by the family of semi-norms $p_{U,C,\alpha}$ such that

$p_{U,C,\alpha}(f) =$ sup$_{x\in C}\|(\partial^{\alpha}f_U)(x)\|$, where U ranges over $\mathscr{U}, C$ ranges over the set of compact subsets of $\varphi_U(U)$ and $\alpha \in \mathbf{N}^{n_U}$ ranges over the set of multi-indices such that $|\alpha |\leqslant r$.

#### Proposition 10 {#ts-iii-s2-prop-10 .statement tag=02R6}

Suppose that the vector bundle E is locally of finite rank. Let $s$ be an integer such that $0\leqslant s < r$ and Y a relatively compact open subset of X. The linear mapping $f\mapsto f|Y$ of $\mathscr{S}^r(X; E)$ into $\mathscr{S}^s(Y; E)$ is compact.

Suppose first that there exist an integer $n\geqslant 0$ and a finite-dimensional Banach space F such that X is an open subset of $\mathbf{R}^n$ and E the trivial vector bundle $X\times F$ with base X and fibre F. In this case, the topological vector spaces $\mathscr{S}^r(X; E)$ and $\mathscr{S}^s(Y; E)$ are isomorphic to $\mathscr{C}^r(X; F)$ and $\mathscr{C}^s(Y; F)$, respectively, and prop. 10 is a consequence of prop. 8.

Let us pass to the general case. Let C be a compact subset of X containing Y. For every point $x$ of C, choose an open neighbourhood $U(x)$ of $x$ in X which is a coordinate domain over which the vector bundle E is trivializable. Moreover, choose an open relatively compact neighbourhood $V(x)$ of $x$ in $U(x)$. Since the set C is compact, it is covered by a finite family $(V(x_1), . . . ,V(x_m))$ of such open sets. For every $i$, put $U_i= U(x_i)$ and $Y_i= V(x_i)\cap Y$. Then $Y_i$ is an open relatively compact subset of $U_i$ and one has $Y = Y_1\cup  \cdots  \cup Y_m$. The linear mappings $f\mapsto f|U_i$ of $\mathscr{S}^r(X; E)$ into $\mathscr{S}^r(U_i; E)$ are continuous and the linear mappings $g\mapsto g|Y_i$ of $\mathscr{S}^r(U_i; E)$ into $\mathscr{S}^s(Y_i; E)$ are compact by the first part of the proof. The linear mappings $f\mapsto f|Y_i$ of $\mathscr{S}^r(X; E)$ into $\mathscr{S}^s(Y_i; E)$ are therefore compact (prop. 3 of III, p. 5). Taking into account lemma 4, applied to the covering of Y by the open sets $Y_i$, and remarks 5 and 6 of III, p. 3, the linear mapping $f\mapsto f|Y$ of $\mathscr{S}^r(X; E)$ into $\mathscr{S}^s(Y; E)$ is compact, which completes the proof.

### 7. Restriction of analytic sections of a vector bundle

Let X be a complex analytic manifold locally of finite dimension and E an analytic vector bundle with base X (VAR, p. 35 and VAR, p. 70). Denote by $\mathscr{S}^{\omega}(X; E)$ the vector space of analytic sections of E on X, endowed with the topology of compact convergence.

#### Lemma 5 {#ts-iii-s2-lem-5 .statement tag=02R7}

Let $X_0$ be the underlying real analytic manifold of X and $E_0$ the complex vector bundle on $X_0$ underlying E.

a) The vector subspace $\mathscr{S}^{\omega}(X; E)$ of $\mathscr{S}^0(X_0; E_0)$ is closed, and the injection of $\mathscr{S}^{\omega}(X; E)$ into $\mathscr{S}^0(X_0; E_0)$ is continuous and strict ;

b) The canonical injection of $\mathscr{S}^{\omega}(X; E)$ into $\mathscr{S}^1(X_0; E_0)$ is continuous.

Suppose first that there exist an integer $n\geqslant 0$ and a Banach space F such that X is an open subset of $\mathbf{C}^n$ and E the trivial vector bundle $X\times F$. In this case, the topological vector spaces $\mathscr{S}^{\omega}(X; E)$, $\mathscr{S}^0(X_0; E_0)$ and $\mathscr{S}^1(X_0; E_0)$ are isomorphic to $\mathscr{C}^{\omega}(X; F),\mathscr{C}^0(X_0; F)$ and $\mathscr{C}^1(X_0; F)$ respectively, and the vector space $\mathscr{S}^0(X_0; E_0)$ is metrizable (TG, X, p. 20, cor. of prop. 1). The lemma then follows from VAR, 3.3.2, p. 28.

Let us pass to the general case. Let $\mathfrak{F}$ be a filter on $\mathscr{S}^{\omega}(X; E)$ which converges in the space $\mathscr{S}^0(X_0; E_0)$ to a limit $f$. It is a question of proving that $f$ belongs to $\mathscr{S}^{\omega}(X; E)$ and that the filter $\mathfrak{F}$ converges to $f$ in the space $\mathscr{S}^1(X_0; E_0)$. This statement is of a local nature, and therefore follows from the first part of the proof.

#### Proposition 11 {#ts-iii-s2-prop-11 .statement tag=02R8}

Suppose that the vector bundle E is locally of finite rank. Let Y be an open relatively compact subset of X. The restriction mapping $f\mapsto f|Y$ of $\mathscr{S}^{\omega}(X; E)$ into $\mathscr{S}^{\omega}(Y; E)$ is compact.

With the notation of lemma 5, one has a commutative diagram

$$
\mathscr{S}^{\omega}(X; E)\leftarrow_i\rightarrow \mathscr{S}^1(X_0; E_0)
$$

$$
\rightarrow \leftarrow_u\rightarrow \leftarrow_v \tag{3}
$$

$$
\mathscr{S}^{\omega}(Y; E)\leftarrow_j\rightarrow \mathscr{S}^0(Y_0; E_0)
$$

where $i$ and $j$ are the canonical injections and $u,v$ the restriction mappings. The mapping $i$ is continuous (Lemma 5, b)), and the mapping $u$ is compact (Proposition 10). Since the canonical injection $j$ is continuous, strict, and has closed image (Lemma 5, a)), the mapping $u$ is compact (Remark 5 of III, p. 3).

#### Corollary {#ts-iii-s2-n7-cor-1 .statement tag=02R9}

Let X be a compact complex analytic manifold and E an analytic vector bundle over X, locally of finite rank. The vector space $\mathscr{S}^{\omega}(X; E)$ is finite-dimensional.

Since it is compact, the analytic manifold X is locally finite-dimensional. By Proposition 11, the identity mapping of $\mathscr{S}^{\omega}(X; E)$ is a compact linear mapping. This implies that the space $\mathscr{S}^{\omega}(X; E)$ is finite-dimensional (Remark 3 of III, p. 2).

## EXERCISES {#ts-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
