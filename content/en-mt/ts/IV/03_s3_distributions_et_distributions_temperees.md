---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 3
section_title: Distributions et distributions tempérées
lang: en
source: ts-iii-v-fr
book_pages: TS IV.196-TS IV.223, TS IV.330-TS IV.344
pdf_pages: 0209-0236, 0343-0357
extraction: native
subsections:
    - "no": 1
      title: Dérivation sous le signe somme
      page: 197
      pdf_page: 210
    - "no": 2
      title: Critères d’intégrabilité dans R$^n$ et Z$^n$
      page: 199
      pdf_page: 212
    - "no": 3
      title: Fonctions test
      page: 200
      pdf_page: 213
    - "no": 4
      title: Distributions
      page: 203
      pdf_page: 216
    - "no": 5
      title: Interprétation de fonctions comme distributions
      page: 206
      pdf_page: 219
    - "no": 6
      title: Dérivation des distributions
      page: 208
      pdf_page: 221
    - "no": 7
      title: Fonctions de Schwartz
      page: 209
      pdf_page: 222
    - "no": 8
      title: Inclusions d’espaces fonctionnels dans l’espace des fonctions de Schwartz
      page: 212
      pdf_page: 225
    - "no": 9
      title: Fonctions à croissance polynomiale
      page: 214
      pdf_page: 227
    - "no": 10
      title: Distributions tempérées
      page: 214
      pdf_page: 227
    - "no": 11
      title: Interprétation de fonctions comme distributions tempérées
      page: 216
      pdf_page: 229
    - "no": 12
      title: Transformation de Fourier des distributions tempérées
      page: 217
      pdf_page: 230
    - "no": 13
      title: Distributions et distributions tempérées sur un espace vectoriel
      page: 221
      pdf_page: 234
    - "no": 14
      title: Espaces de Sobolev
      page: 221
      pdf_page: 234
statements: 46
exercises: 33
content_sha256: 83403e096a36131af4fc93cdae5fe789686d4fc6631978a38c0948a981a7d65d
translated_from: content/fr/ts/IV/03_s3_distributions_et_distributions_temperees.md
source_lang: fr
translation_method: machine
source_content_sha256: 3d17c966d69171e8d653683de206a3ba30cca6eb8de3f8fd0cd8b5105dcf851c
translation_model: gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-78efe726
glossary_version: 34
glossary_terms_sha256: 94c6c4c6c4065d4d98a334362c53670e67b0da5e3e653a829f0895b4ed7172e9
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. DISTRIBUTIONS AND TEMPERED DISTRIBUTIONS

In this paragraph, $n$ denotes a natural number. We shall denote by $\mu$ the Lebesgue measure on $\mathbf{R}^n$, as well as its restriction to every locally compact set of $\mathbf{R}^n$.

We denote

$$
x\cdot y=\sum_{i=1}^nx_iy_i
$$

the scalar product on the euclidean space $\mathbf{R}^n$; the euclidean norm is denoted by $x\mapsto  \|x\|$ (TG, VI, p. 7). We recall that the group $\mathbf{R}^n$ is in duality with itself relative to the mapping $(x, y)\mapsto$ exp(2$i\pi  x\cdot y$) and that the dual measure of the Lebesgue measure is then identified with the Lebesgue measure (corollary 3 of II, p. 236). We denote by $\mathscr{F}$ (resp. $\overline{\mathscr{F}}$) the Fourier transform (resp. the Fourier cotransform) of $\mathbf{R}^n$ (cf. n$^o9$ of II, p. 237).

For every $\alpha = (\alpha_i)_{1\leqslant i\leqslant n}\in \mathbf{N}^n$, we shall denote by $X^{\alpha}$ the function of $\mathbf{R}^n$

into $\mathbf{R}$ defined by $x= (x_i)_{1\leqslant i\leqslant n}\mapsto x^{\alpha}=\prod_{i=1}^nx^{\alpha_i}_i$.

Let $\alpha$ and $\beta$ be elements of $\mathbf{N}^n$. We denote

$$
^n(\alpha )^n(\alpha_i)
$$

$$
|\alpha |=\sum\alpha_i,=\prod
$$

$$
\beta \beta_i
$$

$i=1i=1$

#### Lemma 1 {#ts-iv-s3-lem-1 .statement tag=030C}

Let U be an open subset of $\mathbf{R}^n$.

a) Let K be a compact subset of U and V an open neighbourhood of K in U. There exists a function $\varphi \in \mathscr{C}^{\infty}(U)$ with compact support contained in V such that $0\leqslant \varphi \leqslant 1$ and such that $\varphi (x) = 1$ for every $x\in K$;

b) For every locally finite open covering of U, there exists a partition of unity formed of functions of class $C^{\infty}$ which is subordinate to it.

This results from VAR, R1, p. 40, 5.3.6.

#### Proposition 1 {#ts-iv-s3-prop-1 .statement tag=030D}

Let U be an open subset of $\mathbf{R}^n$ and $k\in \mathbf{N}$. Let E, F and G be topological vector spaces and let $b: E\times F\rightarrow G$ be a continuous bilinear mapping. Let $f$ and $g$ be functions of class $C^k$ from U into E and F respectively. Then the mapping $h:x\mapsto b(f(x), g(x))$ is of class $C^k$ in U; moreover, for every $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant k$ and for every $x\in U$, we have

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial h(x) =\sum b(\partial f(x), \partial g(x))
$$

$$
_{\beta\in\mathbf{N}^n}\beta
$$

$\beta \leqslant \alpha$

The mapping $h$ is the composite of the mapping $(f, g) : U\rightarrow E\times F$, which is of class $C^k$, and of the mapping $b: E\times F\rightarrow G$ which is of class $C^{\infty}$. It is therefore of class $C^k$. The expression for its partial derivatives results from Leibniz's formula (FVR, I, p. 28, prop. 2, cf. A, III, p. 122, corollary).

We recall that a separated locally convex topological vector space is a Montel space if it is barrelled and if every bounded subset is relatively compact (EVT, IV, p. 18, def. 4).

We also recall that if E and F are locally convex spaces, and if E is bornological (EVT, III, p. 12, def. 1), a linear mapping $u: E\rightarrow F$ is continuous if and only if the image by $u$ of every bounded subset of E is bounded in F (EVT, III, p. 11, prop. 1, (iiibis), when F is semi-normed, the general case resulting formally from this, cf. EVT, II, p. 7, prop. 5, b)).

### 1. Derivation under the sum sign

Let X be a locally compact topological space and $\nu$ a measure on X. Let E be a Banach space.

#### Proposition 2 {#ts-iv-s3-prop-2 .statement tag=030E}

Let I be an interval of $\mathbf{R}$ and $f$ a mapping from $X\times I$ into E such that

(i) For every $t\in I$, the mapping $x\mapsto f(x, t)$ of X into E is $\nu$-integrable;

(ii) For every $x\in X$, the mapping $t\mapsto f(x, t)$ of I into E admits a derivative, denoted by $t\mapsto f'(x, t)$;

(iii) There exists a positive $\nu$-integrable function $g$ on X such that $\|f'(x, t)\|\leqslant g(x)$ for every $(x, t)\in X\times I$.

Then the mapping F of I into E defined by

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

is differentiable in I, and for every $t\in I$, one has

$$
F'(t) =\int_Xf'(x, t)d\nu (x)
$$

Let $t_0\in I$ and let J be an interval of $\mathbf{R}$ contained in I which is a neighbourhood of $t_0$ in I. Let $h: X\times J\rightarrow E$ be the mapping defined by $(x, t)\mapsto (f(x, t)-f(x, t_0))/(t-t_0)$ for $(x, t)\in X\times (J-\{t_0\})$ and $(x, t_0)\mapsto f'(x, t_0)$ for $x\in X$. Let $x\in X$. One has $\|h(x, t_0)\|\leqslant g(x)$ and, for every $t\not =t_0$, one has $\|h(x, t)\|\leqslant g(x)$ by FVR, I, p. 23, th. 2. By definition of the derivative, the proposition follows from corollary 1 of INT, IV, p. 144, § 4, n$^o3$, applied to the mapping $h$.

Let us resume the notation of VAR, R1, 2.4, p. 19 concerning partial derivatives.

#### Corollary 1 {#ts-iv-s3-prop-2-cor-1 .statement tag=030F}

Let U be an open set of $\mathbf{R}^n$. Let $k\in \mathbf{N}$ and $f$ be a mapping of $X\times U$ into E satisfying the following conditions:

(i) For every $t\in U$, the mapping $x\mapsto f(x, t)$ of X into E is $\nu$-integrable;

(ii) For every $x\in X$, the mapping $t\mapsto f(x, t)$ of U into E is of class $C^k$, with partial derivatives denoted by $\partial^{\alpha}f(x, t)$ for every $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant k$;

(iii) There exists a $\nu$-integrable function $g$ on X such that for every $\alpha \in \mathbf{N}^n$ satisfying $|\alpha |\leqslant k$ and for every $(x, t)\in X\times U$, one has $\|\partial^{\alpha}f(x, t)\|\leqslant g(x)$.

Then the mapping F of U into E defined by

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

is of class $C^k$ in U, and for every $\alpha \in \mathbf{N}^n$ satisfying $|\alpha |\leqslant k$ and every $t\in U$, one has

$$
\partial^{\alpha}F(t) =\int_X\partial^{\alpha}f(x, t)d\nu (x)
$$

This follows from the proposition by induction on $k$.

#### Corollary 2 {#ts-iv-s3-prop-2-cor-2 .statement tag=030G}

Let $k$ be a natural number. Let $f\in \mathscr{L}^1(\mathbf{R}^n, \mu)$ and $g\in \mathscr{C}^k(\mathbf{R}^n)$. Suppose that for every $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant k$, the function $\partial^{\alpha}g$ is bounded. Then the convolution product $f*g$ belong to $\mathscr{C}^k(\mathbf{R}^n)$ and for every $\alpha$ such that $|\alpha |\leqslant k$, one has $\partial^{\alpha}(f*g) =f*\partial^{\alpha}g$.

One can apply corollary 1 to the space $X =\mathbf{R}^n$, to Lebesgue measure and to the mapping $h$ defined by $(x, t)\mapsto f(x)g(t-x)$ from $\mathbf{R}^n\times \mathbf{R}^n$ into $\mathbf{C}$; indeed, for every $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant k$, one has the inequality

$|\partial^{\alpha}h(x, t)|\leqslant ($sup$_{|\beta|\leqslant k}$ sup$_{y\in\mathbf{R}^n}|\partial^{\beta}g(y)|)|f(x)|$

whose right-hand side is an integrable function on $\mathbf{R}^n$.

### 2. Integrability Criteria in R$^n$ and Z$^n$

#### Proposition 3 {#ts-iv-s3-prop-3 .statement tag=030H}

Let N be a norm on $\mathbf{R}^n,r$ a real number and $p\in [1,+\infty [$.

a) The function $(1 + N)^r$ belong to $\mathscr{L}^p(\mathbf{R}^n, \mu)$ if and only if $rp <-n$;

a$')$ The restriction to $\mathbf{Z}^n$ of the function $(1 + N)^r$ belong to $\ell^p(\mathbf{Z}^n)$ if and only if $rp <-n$;

b) Let V be a bounded measurable neighbourhood of 0 in $\mathbf{R}^n$. The function $N^r$ belong to $\mathscr{L}^p(\mathbf{R}^n-V, \mu)$ if and only if $rp <-n$.

By virtue of the equivalence of norms on $\mathbf{R}^n$ (EVT I, p. 14, th. 2 and TG, IX, p. 32, prop. 8), we may suppose that the norm N is given by $N(x) =$ sup$|x_i|$ for $x= (x_i)\in \mathbf{R}^n$. Let B denote the unit ball of $\mathbf{R}^n$ for this norm.

Let V be a bounded measurable neighbourhood of 0 in $\mathbf{R}^n$. The function $N^r$ is continuous and bounded on (B- $V$)$\cup (V$- B), which shows that assertion b) is valid if and only if it is so when V = B, which we shall henceforth suppose. Since the function $(1 + N)^r$ is continuous and bounded on B, and satisfies the inequalities $N^r\leqslant (1 + N)^r\leqslant 2^rN^r$ on $\mathbf{R}^n-$ B, we see that assertions a) and b) are equivalent.

Let us prove b) when V = B. We may suppose that $p= 1$. Since the case where $r >0$ is elementary, suppose that $r\leqslant 0$. For every integer $j\geqslant 1$, the set

$$
C_j=\{x\in \mathbf{R}^n|2^{j-1}\leqslant N(x)<2^j\}
$$

is of measure $2^{nj}(2^n-1)$. The sets $(C_j)_{j\geqslant 1}$ form a partition of $\mathbf{R}^n-$ B. According to INT, V, p. 4, § 1, No.$^o1$, cor., one therefore has

$$
\int^*N^rd\mu=\sum\int^*N^rd\mu
$$

$\mathbf{R}^{n-}Bj\geqslant 1C_j$

$\leqslant \sum_{j\geqslant 1}2^{n+nj}2^{r(j-1)}= 2^{n-r}\sum_{j\geqslant 1}2^{(n+r)j}$ which is finite if $r <-n$. On the other hand, one has (loc. cit.)

$$
\int^*N^rd\mu\geqslant \sum 2^{rj}2^{nj}(2^n-1) = (2^n-1)\sum 2^{(r+n)j}
$$

$\mathbf{R}^{n-}Bj\geqslant 1j\geqslant 1$

which is infinite if $r\geqslant -n$.

One proves a$')$ similarly by considering the sets $C_j\cap \mathbf{Z}^n$ which cover $\mathbf{Z}^n-\{0\}$ and satisfy

Card(C$_j\cap \mathbf{Z}^n$) $= (2^{j+1}-1)^n-(2^j-1)^n$,

which belongs to the interval $[(1-2^{-n})(2^{j+1}-1)^n,2^{n(j+1)}]$.

### 3. Test functions

In this No., U denotes an open subset of $\mathbf{R}^n$. For $p\in [1,+\infty ]$, we shall write $\mathscr{L}^p(U)$ and $L^p(U)$ rather than $\mathscr{L}^p(U, \mu)$ and $L^p(U, \mu)$. We identify the continuous functions belonging to $\mathscr{L}^p(U)$ with their image in $L^p(U)$.

Let us endow the space $\mathscr{C}^{\infty}(U)$ of indefinitely differentiable complex-valued functions in U with the topology defined by the family of seminorms $p_{\alpha ,K}$ defined for $\alpha \in \mathbf{N}^n$ and $K\subset U$ by

$p_{\alpha ,K}(\varphi ) =$ sup$_{x\in K}|\partial^{\alpha}\varphi (x)|$.

This space is complete (cf. EVT, III, p. 9, example b)).

For every compact subset K of U, we denote by $\mathscr{C}_K^{\infty}(U)$ the subspace of $\mathscr{C}^{\infty}(U)$ formed by the functions with support in K. The space $\mathscr{C}_K^{\infty}(U)$ is endowed with the topology induced by that of $\mathscr{C}^{\infty}(U)$. It is a Fréchet space, a countable family of seminorms defining its topology being the family $(p_{\alpha ,K})_{\alpha\in\mathbf{N}^n}$. In particular, it is a bornological space (EVT, III, p. 12, prop. 2).

We denote by $\mathscr{D}(U)$ the vector space $\mathscr{K}(U)\cap \mathscr{C}^{\infty}(U)$ of functions of class $C^{\infty}$ with compact support in U. We say that $\mathscr{D}(U)$ is the space of test functions in U. The space $\mathscr{D}(U)$ is the inductive limit of the spaces $\mathscr{C}_K^{\infty}(U)$ and is endowed with the corresponding inductive limit locally convex topology (EVT, II, p. 31).

This space is denoted by $\mathscr{C}_{\circ}^{\infty}(U)$ in EVT, III, p. 9.

Let $(K_m)$ be an increasing sequence of compact subsets of U whose interiors form a covering of U. The space $\mathscr{D}(U)$ is then the strict inductive limit of the spaces $\mathscr{C}_{K_m}^{\infty}(U)$ (EVT, III, p. 9). It is therefore a complete space (EVT, II, p. 35, prop. 9). Every bounded subset of $\mathscr{D}(U)$ is contained in one of the subspaces $\mathscr{C}_{K_m}^{\infty}(U)$ (EVT, III, p. 5, prop. 6). This means that $B\subset \mathscr{D}(U)$ is bounded if and only if there exist a compact subset K of U and a family $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ in $\mathbf{R}_+$ such that B is contained in the set of functions $\varphi \in \mathscr{C}_K^{\infty}(U)$ satisfying

$$
p_{\alpha ,K}(\varphi )\leqslant M_{\alpha}
$$

for every $\alpha \in \mathbf{N}^n$.

The space $\mathscr{D}(U)$ is a bornological space (EVT, III, p. 12, example 3) and a Montel space (EVT, IV, p. 18, example 4).

Let V be an open subset of $\mathbf{R}^n$ contained in U. If $K\subset V$ is compact, then restriction of functions to V defines a continuous surjective linear mapping of $\mathscr{C}_K^{\infty}(U)$ onto $\mathscr{C}_K^{\infty}(V)$. Extension by zero of a function defined on V induces an injective continuous linear mapping, called canonical, of $\mathscr{D}(V)$ into $\mathscr{D}(U)$.

#### Remark {#ts-iv-s3-n3-rem-1 .statement tag=030I}

One defines analogously the space $\mathscr{D}_{\mathbf{R}}(U)$ of real-valued test functions in U. The linear mapping such that $z\otimes \varphi \mapsto z\varphi$ for every $z\in \mathbf{C}$ and every $\varphi \in \mathscr{D}_{\mathbf{R}}(U)$ is an isomorphism of $\mathbf{C}\otimes \mathscr{D}_{\mathbf{R}}(U)$ onto $\mathscr{D}(U)$.

#### Lemma 2 {#ts-iv-s3-lem-2 .statement tag=030J}

Let $\mathscr{U}$ be an open covering of U. There exists a locally finite open covering of U finer than $\mathscr{U}$ and formed of relatively compact sets.

Since U is locally compact, there exists a covering $\mathscr{V}$ of U finer than $\mathscr{U}$ consisting of open sets relatively compact in U. Since U is paracompact (TG, IX, p. 51, th. 4), there exists a locally finite open covering $\mathscr{W}$ finer than $\mathscr{V}$. Then $\mathscr{W}$ is finer than $\mathscr{U}$ and consists of open sets relatively compact.

#### Lemma 3 {#ts-iv-s3-lem-3 .statement tag=030K}

Let $f\in \mathscr{K}(\mathbf{R}^n)$ and let V be an open neighbourhood of the support K of $f$. There exists an integer $m_0\geqslant 1$ such that, for every $x\in K$, the set V contains the ball of radius $m^{-1}_0$ with centre at $x$. For every integer $m > m_0$, let $V_m$ be the closed ball of radius $m^{-1}$ with centre at 0 in $\mathbf{R}^n$ and let $\varphi_m$ be a test function with support in $V_m$, positive and of integral 1. Put $f_m=\varphi_m*f$.

a) One has $f_m\in \mathscr{D}(\mathbf{R}^n)$ and the support of $f_m$ is contained in V ;

b) Let $p\in [1,+\infty ]$. The sequence $(f_m)_{m>m_0}$ converges to $f$ in $L^p(\mathbf{R}^n)$.

By TG, IX, p. 14, remark, one has $d(K,\mathbf{R}^n-V)>0$. Let $m_0\geqslant 1$ be an integer such that $m^{-1}_0< d(K,\mathbf{R}^n-$ V) ; it satisfies the required condition. For every $m > m_0$, the function $f_m$ is continuous (INT, VIII, p. 166, § 4, n$^o5$, prop. 11) and with support contained in $K + V_m$ (INT, VIII, p. 126, § 1, n$^o4$, prop. 5), hence in V. By Corollary 2 of IV, p. 198, one has $f_m\in \mathscr{D}(\mathbf{R}^n)$. If $p\not = +\infty$, then the sequence $(f_m)$ converges to $f$ in $L^p(\mathbf{R}^n)$ (INT, VIII, p. 172, § 4, n$^o7$, prop. 20).[^1]

Suppose that $p= +\infty$. Let $\varepsilon  >0$. The function $f$ is uniformly continuous on $\mathbf{R}^n$, therefore there exists an integer $m_1> m_0$ such that, for every $m\geqslant m_1$ and all $x\in \mathbf{R}^n$ and $y\in V_m$, one has $|f(x)-f(x-y)|< \varepsilon$.

For every $m\geqslant m_1$, the function $\varphi_m$ vanishes outside $V_m$, is positive and of integral 1. One therefore deduces the inequality

$$
|f(x)-f_m(x)|=|\int_{\mathbf{R}^n}(f(x)-f(x-y))\varphi_m(y)d\mu(y)|\leqslant \varepsilon
$$

for every $x\in \mathbf{R}^n$, whence the result.

#### Proposition 4 {#ts-iv-s3-prop-4 .statement tag=030L}

a) The canonical injection of $\mathscr{D}(U)$ into $\mathscr{K}(U)$ is continuous and $\mathscr{D}(U)$ is dense in $\mathscr{K}(U)$;

b) For every $p\in [1,+\infty [$, the canonical injection of $\mathscr{D}(U)$ into $\mathscr{L}^p(U)$ is continuous and $\mathscr{D}(U)$ is dense in $L^p(U)$.

Every continuous seminorm on $\mathscr{K}(U)$ is continuous on $\mathscr{D}$(U), hence the canonical injection of $\mathscr{D}(U)$ into $\mathscr{K}(U)$ is continuous.

Let $f\in \mathscr{K}(U)$. There exists a sequence $(f_m)_{m\in\mathbf{N}}$ in $\mathscr{D}(U)$ which converges uniformly to $f$ on U and such that the supports of the $f_m$ are contained in a fixed relatively compact neighbourhood of the support of $f$ (Lemma 3). The sequence $(f_m)$ therefore converges to $f$ in $\mathscr{K}(U)$. This concludes the proof of a).

Let $p\in [1,+\infty [$. Let $f\in \mathscr{D}(U)$ and let K be the support of $f$. One then has the inequality $N_p(f)\leqslant \mu(K)^{1/p}$ sup$_{x\in K}|f(x)|$, hence the canonical injection of $\mathscr{D}(U)$ into $\mathscr{L}^p(U)$ is continuous. The last part of assertion b) then results from a).

Since the product of two test functions is again a test function, Leibniz's formula (FVR, I, p. 28, prop. 2) shows that the space $\mathscr{D}(U)$ is a topological algebra.

More generally, let $f\in \mathscr{C}^{\infty}(U)$. The linear mapping $\varphi \mapsto f \varphi$ of $\mathscr{D}(U)$ into $\mathscr{D}(U)$ is then continuous. In fact, for every compact subset K of U and every $\alpha \in \mathbf{N}^n$, one has

$$
(\alpha )
$$

$$
p_{\alpha ,K}(f \varphi )\leqslant \sum p_{\beta ,K}(f)p_{\alpha-\beta ,K}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

(cf. loc. cit.).

### 4. Distributions

We retain the notation of the preceding number; U therefore denotes an open subset of $\mathbf{R}^n$.

#### Definition 1 {#ts-iv-s3-def-1 .statement tag=030M}

The dual space of $\mathscr{D}(U)$, endowed with the topology of bounded convergence, is called the space of distributions on U. It is denoted by $\mathscr{D}'(U)$.

A distribution on U is therefore a continuous linear form on $\mathscr{D}(U)$.

If $f$ is a linear form on $\mathscr{D}(U)$ (and in particular if $f$ is a distribution) and if $\varphi$ belongs to $\mathscr{D}$(U), we shall denote by $\langle f, \varphi \rangle$ the value of $f$ at $\varphi$.

Since $\mathscr{D}(U)$ is bornological, the space $\mathscr{D}'(U)$ is complete (EVT, III, p. 24, cor. 1). Since $\mathscr{D}(U)$ is a Montel space, the same is true of $\mathscr{D}'(U)$ (EVT, IV, p. 19, prop. 9). In particular, the space $\mathscr{D}'(U)$ is reflexive (EVT, IV, p. 16, th. 2).

#### Lemma 4 {#ts-iv-s3-lem-4 .statement tag=030N}

Let $f$ be a linear mapping of $\mathscr{D}(U)$ into $\mathbf{C}$. Then $f$ is a distribution if and only if, for every compact subset K of U and every family $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ in $\mathbf{R}_+$, the linear form $f$ is bounded on the set of functions $\varphi \in \mathscr{C}_K^{\infty}(U)$ such that, for every $\alpha \in \mathbf{N}^n$, one has

sup$_{x\in K}|\partial^{\alpha}\varphi (x)|\leqslant M_{\alpha}$.

In fact, the space $\mathscr{D}(U)$ is bornological and every bounded subset of $\mathscr{D}(U)$ is contained in one of the bounded sets described in the statement.

#### Lemma 5 {#ts-iv-s3-lem-5 .statement tag=030O}

Let $\mathfrak{F}$ be a filter on $\mathscr{D}'(U)$ having a countable basis or containing a simply bounded set. Then $\mathfrak{F}$ converges to a distribution if and only if $\langle f, \varphi \rangle$ converges according to $\mathfrak{F}$ for every test function $\varphi$ on U.

In particular, a sequence $(f_m)_{m\in\mathbf{N}}$ of distributions converges to a distribution $f$ if and only if, for every $\varphi \in \mathscr{D}(U)$, the sequence $(\langle f_m, \varphi \rangle )_{m\in\mathbf{N}}$ converges to $\langle f, \varphi \rangle$.

Since $\mathscr{D}'(U)$ is a Montel space, hence barrelled, this follows from the Banach-Steinhaus theorem (EVT, III, p. 26, cor. 3 of th. 1).

Let V be an open set contained in U. The transpose of the canonical linear mapping of $\mathscr{D}(V)$ into $\mathscr{D}(U)$ is a continuous linear mapping of $\mathscr{D}'(U)$ into $\mathscr{D}'$(V), called the restriction of distributions from U to V and denoted by $r_{VU}$, or sometimes $r_{V,U}$.

One has $r_{VV}= 1_{\mathscr{D}'(V)}$. If $W\subset V\subset U$ are open sets in U, then one has $r_{WV}\circ r_{VU}=r_{WU}$. In other words, if $\mathscr{T}$ denotes the topology on U, the projective system $\mathscr{D}'(U) = ((\mathscr{D}'(V))_{V\in\mathscr{T}},(r_{WV}))$ is a presheaf on U with values in the Species of structures of locally convex topological vector spaces (TA, I, p. 42, def. 1 and p. 66, §10).

#### Proposition 5 {#ts-iv-s3-prop-5 .statement tag=030P}

The presheaf $\mathscr{D}'(U)$ is a sheaf.

Let us recall (TA, I, p. 43, def. 2) that this means that for every open subset V of U and every open covering $(V_i)_{i\in I}$ of V, the following conditions are satisfied:

(i) The mapping $(r_{V_iV})_{i\in I}:\mathscr{D}'(V)\rightarrow \prod_{i\in I}\mathscr{D}'(V_i)$ is injective;

(ii) For every family $(f_i)\in \prod_{i\in I}\mathscr{D}'(V_i)$ such that

$$
r_{(V_i\cap V_{i'})V_i}(f_i) =r_{(V_i\cap V_{i'})V_{i'}}(f_{i'})
$$

for every pair $(i, i')\in I\times I$, there exists a distribution $f\in \mathscr{D}'(V)$ such that for every $i\in I$, one has $r_{V_iV}(f) =f_i$.

Let V be an open set of U and $\mathscr{V}= (V_i)_{i\in I}$ an open covering of V. Let $(W_j)_{j\in J}$ be a locally finite open covering of V, finer than $\mathscr{V}$ and formed of relatively compact subsets (lemma 2 of IV, p. 201). Let us fix a partition of unity $(\varphi_j)_{j\in J}$ subordinate to the covering $(W_j)_{j\in J}$ such that the support of $\varphi_j$ is contained in $W_j$ for every $j\in J$ (lemma 1 of IV, p. 196).

Let $\varphi \in \mathscr{D}(V)$. Since the set of $j\in J$ such that $W_j$ meets the support of $\varphi$ is finite (TG, I, §9, n$^o1$, p. 59), one has

$$
\varphi =\sum_{j\in J}\varphi \varphi_j
$$

where the sum consists of only a finite number of non-zero terms.

Let us prove (i). Suppose that $f\in \mathscr{D}'(V)$ satisfies $r_{V_iV}(f) = 0$ for every $i\in I$. This means that $\langle f, \varphi \rangle = 0$ for every test function $\varphi$ whose support is contained in one of the open sets $V_i$. This is fortiori true if the support of $\varphi$ is contained in one of the open sets $W_j$. But then, for every $\varphi \in \mathscr{D}$(V), we have

$$
\langle f, \varphi \rangle =\langle f,\sum_{j\in J}\varphi \varphi_j\rangle =\sum_{j\in J}\langle f, \varphi \varphi_j\rangle = 0
$$

hence $f= 0$.

Let us prove (ii). Let $(f_i)_{i\in I}$ be a family such that $f_i\in \mathscr{D}'(V_i)$ for every $i\in I$ and $r_{V_i\cap V_{i'},V_i}(f_i) =r_{V_i\cap V_{i'},V_{i'}}(f_{i'})$ for all $i$ and $i'$ in I. Let $\iota : J\rightarrow I$ be a mapping such that $W_j\subset V_{\iota(j)}$ for every $j\in J$. For every $j\in J$, put $\widetilde{f}_j=r_{W_j,V_{\iota(j)}}(f_{\iota(j)})$. We then have

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)}))
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}}(f_{\iota(j)})
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}\cap V_{\iota(j')}}\circ r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)})
$$

Exchanging the role of $j$ and $j'$ and noting that

$$
r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j')}}(f_{\iota(j')})
$$

by assumption, we deduce that

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(\widetilde{f}_{j'}) \tag{1}
$$

for all $(j, j')\in J^2$.

For $\varphi \in \mathscr{D}$(V), put

$$
\lambda (\varphi ) =\sum_{j\in J}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

where the sum is finite since only a finite number of terms can be non-zero.

The mapping $\lambda$ is a linear form on $\mathscr{D}(V)$. Let us prove that it is a distribution. Let B be a bounded subset of $\mathscr{D}(V)$ and let K be a compact subset of V such that $B\subset \mathscr{C}_K^{\infty}(V)$. By TG, I, §9, n$^o1$, p. 59, there exists a finite subset $J'$ of J such that

$$
\lambda (\varphi ) =\sum_{j\in J'}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

for every $\varphi \in B$. Since $\widetilde{f}_j$ is a distribution for every $j\in J'$ and $\mathscr{D}(V)$ is a topological algebra, we deduce that $\lambda$ is bounded on B, whence the result (lemma 4).

Let $j\in J$ and let $\varphi \in \mathscr{D}(V)$ whose support is contained in $W_j$. We then have

$$
\langle \lambda , \varphi \rangle =\sum_{j'\in J}\langle \widetilde{f}_{j'}, \varphi \varphi_{j'}|W_j\rangle =\sum_{j'\in J}\langle \widetilde{f}_j, \varphi \varphi_{j'}|W_j\rangle
$$

by (1), since $\varphi \varphi_{j'}$ has support contained in $W_j\cap W_{j'}$. Consequently

$$
\langle \lambda , \varphi \rangle =\langle \widetilde{f}_j,\sum_{j'\in J}\varphi \varphi_{j'}|W_j\rangle =\langle \widetilde{f}_j, \varphi |W_j\rangle
$$

whence $r_{W_jV}(\lambda ) =\widetilde{f}_j$ for every $j\in J$.

Let $i\in I$. Let us show finally that the restriction of $\lambda$ to $V_i$ coincides with $f_i$. By condition (i), applied to the covering of $V_i$ by the open sets $W_j$, it is enough to verify that for every $j\in J$, the restriction of $\lambda$ to $V_i\cap W_j$ coincides with that of $f_i$. By what precedes, it is a question of verifying that the restriction of $f_i$ to $V_i\cap W_j$ is that of $\widetilde{f}_j$. Now one has

$$
r_{V_i\cap W_j,V_i}(f_i) =r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_i}(f_i))
$$

$$
=r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)})
$$

where one has used the assumption concerning the family $(f_i)$. But then

$$
r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)})) =r_{V_i\cap W_j,W_j}(\widetilde{f}_j)
$$

which permits one to conclude.

### 5. Interpretation of functions as distributions

#### Proposition 6 {#ts-iv-s3-prop-6 .statement tag=030Q}

Let $\nu$ be a measure on U. The restriction of $\nu$ to $\mathscr{D}(U)$ is a distribution, which is zero if and only if the measure $\nu$ is zero.

Let K be a compact subset of U. For every function $\varphi \in \mathscr{C}_K^{\infty}$(U), one has $|\langle \nu , \varphi \rangle |\leqslant p_{0,K}(\varphi )|\nu |$(K), hence the restriction of $\nu$ to $\mathscr{D}(U)$ is continuous. Since $\mathscr{D}(U)$ is dense in $\mathscr{K}(U)$ (prop. 4, a) of IV, p. 202), the restriction of $\nu$ to $\mathscr{D}(U)$ is zero if and only if $\nu$ is zero.

We shall identify the space $\mathscr{M}(U;\mathbf{C})$ of complex measures on U with a subspace of $\mathscr{D}'(U)$. We shall also identify the space $L^1_{loc}(U)$ with a subspace of $\mathscr{D}'(U)$ by the mapping deduced by passing to quotients from the mapping which associates to $f\in \mathscr{L}_{loc}^1(U)$ the measure $f\cdot \mu$ (INT, V, p. 44, § 5, No.$^o2$, def. 2). In other words, for $f\in L^1_{loc}(U)$ and $\varphi \in \mathscr{D}$(U), one has

$$
\langle f, \varphi \rangle =\int_Uf \varphi  d\mu
$$

In particular, for $p\in [1,+\infty ]$, this permits one to identify the space $L^p(U)$ with a subspace of $\mathscr{D}'(U) ($cf. INT, V, p. 43, § 5, No.$^o1)$.

#### Proposition 7 {#ts-iv-s3-prop-7 .statement tag=030R}

Let $p\in [1,+\infty ]$. The injection of $L^p(U)$ into $\mathscr{D}'(U)$ is continuous.

Let $f\in L^p(U)$. Let K be a compact subset of U, and denote by $\varphi_K$ its characteristic function. For every test function $\varphi$ with support contained in K, Hölder's inequality implies

$$
|\langle f, \varphi \rangle |=|\int_Uf \varphi  d\mu|\leqslant N_p(f)N_q(\varphi )\leqslant N_p(f)N_q(\varphi_K)p_{0,K}(\varphi )
$$

where $q$ is the conjugate exponent of $p$.

In particular one can identify $\mathscr{D}(U)$ with a subspace of $\mathscr{D}'(U)$.

#### Proposition 8 {#ts-iv-s3-prop-8 .statement tag=030S}

The space $\mathscr{D}(U)$ is dense in $\mathscr{D}'(U)$.

Let $\lambda$ be a linear form on $\mathscr{D}'(U)$ which is zero on $\mathscr{D}(U)$. Since $\mathscr{D}(U)$ is reflexive, there exists a test function $\varphi \in \mathscr{D}(U)$ such that $\lambda (f) =\langle f, \varphi \rangle$ for every $f\in \mathscr{D}'(U)$. Hence

$$
0 =\lambda (\overline{\varphi}) =\langle \varphi , \varphi \rangle =\int_U|\varphi |^2d\mu
$$

whence $\varphi = 0$. The proposition then follows from the Hahn–Banach theorem (EVT, II, p. 49, cor. 3 (ii)).

For $h\in \mathscr{C}^{\infty}$(U), the transpose of the continuous linear mapping $\varphi \mapsto h\varphi$ of $\mathscr{D}(U)$ into itself is a continuous linear mapping of $\mathscr{D}'(U)$ into itself, which is denoted by $f\mapsto hf$. This definition is justified because if $f$ is the distribution associated with a measure $\nu$ on U, then $hf$ is associated with the measure $h\cdot \nu$. In fact, for every test function $\varphi \in \mathscr{D}$(U), one computes

$$
\langle hf, \varphi \rangle =\langle f, h\varphi \rangle =\int_Uh\varphi d\nu =\int_U\varphi  d(h\cdot \nu )
$$

### 6. Derivation of distributions

Let $\alpha \in \mathbf{N}^n$. The linear mapping $\varphi \mapsto \partial^{\alpha}\varphi$ is continuous from $\mathscr{D}(U)$ into $\mathscr{D}(U)$. Its transpose $^t\partial^{\alpha}$ is a continuous linear mapping of $\mathscr{D}'(U)$ into $\mathscr{D}'(U)$ (EVT, IV, p. 6, cor., b)).

The continuous linear mapping $(-1)^{|\alpha|t}\partial^{\alpha}$ of $\mathscr{D}'(U)$ into itself is denoted by $\partial^{\alpha}$.

#### Definition 2 {#ts-iv-s3-def-2 .statement tag=030T}

If $f\in \mathscr{D}'(U)$ is a distribution, $\partial^{\alpha}f$ is called the iterated partial derivative of order $\alpha$ of $f$.

Thus, by definition,

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

for every function $\varphi \in \mathscr{D}(U)$. One has $\partial^{\alpha+\beta}=\partial^{\alpha}\circ \partial^{\beta}$ for all $\alpha$ and $\beta$ in $\mathbf{N}^n$.

If $n= 1$, the derivative of a distribution $f\in \mathscr{D}'(U)$ will also be denoted by $f'$.

The definition is justified by the following lemma.

#### Lemma 6 {#ts-iv-s3-lem-6 .statement tag=030U}

Let $k$ be a natural number. Let $f\in \mathscr{C}^k(U)$ and let $\lambda$ be the distribution associated with $f$. For every $\beta \in \mathbf{N}^n$ such that $|\beta |\leqslant k$, the distribution $\partial^{\beta}\lambda$ is the distribution associated with the function $\partial^{\beta}f$.

By induction on $k$, it is enough to prove this property when $\beta$ satisfies $|\beta |= 1$, and one may even suppose that $\beta = (0, . . . ,0,1)$. Since distributions define a sheaf (prop. 5 of IV, p. 204), it is enough to verify the assertion when there exist an open set $V\subset \mathbf{R}^{n-1}$ and an open interval $I\subset \mathbf{R}$ such that $U = V\times I$.

For every test function $\varphi \in \mathscr{D}$(U), one has by definition

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =-\int_Uf(x)\partial^{\beta}\varphi (x)dx=-\int_V(\int_If(y, t)\partial^{\beta}\varphi (y, t)dt)dy
$$

from the Lebesgue–Fubini theorem (INT, V, p. 96, § 8, n$^o4$, th. 1). By integration by parts (FVR, II, p. 10), one has

$$
-\int_If(y, t)\partial^{\beta}\varphi (y, t)dt=\int_I\partial^{\beta}f(y, t)\varphi (y, t)dt
$$

since $t\mapsto \varphi (y, t)$ has compact support in I. One therefore obtains

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =\int_V(\int_I\partial^{\beta}f(y, t)\varphi (y, t)dt)dy=\langle \partial^{\beta}f, \varphi \rangle
$$

#### Proposition 9 (Leibniz Formula) {#ts-iv-s3-prop-9 .statement tag=030V}

Let $f$ be a distribution on U and $g$ an indefinitely differentiable function on U. Let $\alpha \in \mathbf{N}^n$. One has the relation

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial (f g) =\sum\partial f \partial g
$$

$$
\beta
$$

$\beta \leqslant \alpha$

Proceeding by induction on $|\alpha |$ as in the proof of FVR, I, p. 28, prop. 2, it is enough to consider the case where $|\alpha |= 1$. The result then follows from the calculation

$$
\langle \partial^{\alpha}(f g), \varphi \rangle =\langle f g,-\partial^{\alpha}\varphi \rangle =\langle f,-g\partial^{\alpha}\varphi \rangle
$$

$$
=\langle f,-\partial^{\alpha}(g\varphi ) +\varphi \partial^{\alpha}g\rangle =\langle g\partial^{\alpha}f+f \partial^{\alpha}g, \varphi \rangle
$$

valid for $\varphi \in \mathscr{D}(U)$.

### 7. Schwartz Functions

One denotes by $\mathscr{S}(\mathbf{R}^n)$ the space of indefinitely differentiable functions $\varphi$ on $\mathbf{R}^n$, with complex values, such that, for all $\alpha$ and $\beta$ in $\mathbf{N}^n$, the function $X^{\beta}\partial^{\alpha}\varphi$ is bounded on $\mathbf{R}^n$. One endows $\mathscr{S}(\mathbf{R}^n)$ with the locally convex topology defined by the countable family of seminorms $(q_{\alpha ,\beta})_{(\alpha ,\beta)\in\mathbf{N}^n\times\mathbf{N}^n}$, where $q_{\alpha ,\beta}$ is defined by

$q_{\alpha ,\beta}(\varphi ) =$ sup$_{x\in\mathbf{R}^n}|x^{\beta}\partial^{\alpha}\varphi (x)|=\|X^{\beta}\partial^{\alpha}\varphi \|_{\infty}$

for $\varphi \in \mathscr{S}(\mathbf{R}^n)$. This topology is separated. It is also defined by the seminorms $\widetilde{q}_{\alpha ,k}$ defined by

$\widetilde{q}_{\alpha ,k}(\varphi ) =$ sup$_{x\in\mathbf{R}^n}\|x\|^k|(\partial^{\alpha}\varphi )(x)|$.

for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$, where $k\in \mathbf{N}$ and $\alpha \in \mathbf{N}^n$.

One says that $\mathscr{S}(\mathbf{R}^n)$ is the Schwartz space or the space of Schwartz functions on $\mathbf{R}^n$.

#### Remark {#ts-iv-s3-n7-rem-1 .statement tag=030W}

Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. For every $k\in \mathbf{N}$, one has

lim$_{\|x\|\rightarrow+\infty}\|x\|^k\varphi (x) = 0$,

since the function $x\mapsto  \|x\|^{k+1}\varphi (x)$ is bounded.

#### Example {#ts-iv-s3-n7-exa-1 .statement tag=030X}

The function $\gamma_n$ defined on $\mathbf{R}^n$ by $\gamma_n(x) =$ exp($-\|x\|^2$) belongs to $\mathscr{S}(\mathbf{R}^n)$. In fact, one proves by induction on $k$ that, for every integer $k\in \mathbf{N}$, there exists a polynomial $P_k\in \mathbf{R}[X]$ such that $\partial_k\gamma_1= P_k\gamma_1$.

For all $\alpha = (\alpha_i)\in \mathbf{N}^n$ and $\beta = (\beta_i)\in \mathbf{N}^n$, and every $x= (x_i)\in \mathbf{R}^n$, one then has

$$
|(X^{\beta}\partial^{\alpha}\gamma_n)(x)|=\prod_{i=1}^n|x_i|^{\beta_i}|P_{\alpha_i}(x_i)|\gamma_1(x_i)
$$

which is a bounded quantity when $x$ varies in $\mathbf{R}^n$.

Let $\alpha \in \mathbf{N}^n$ and $\beta \in \mathbf{N}^n$. If $\varphi \in \mathscr{S}(\mathbf{R}^n)$, then $X^{\beta}\partial^{\alpha}(\varphi )$ is again a Schwartz function; the resulting mapping $\varphi \mapsto X^{\beta}\partial^{\alpha}\varphi$ of $\mathscr{S}(\mathbf{R}^n)$ into itself is continuous.

The space $\mathscr{S}(\mathbf{R}^n)$ is a topological algebra. More precisely, if $\varphi_1$ and $\varphi_2$ belong to $\mathscr{S}(\mathbf{R}^n)$, then $\varphi_1\varphi_2$ is a Schwartz function such that

$$
(\alpha )
$$

$$
q_{\alpha ,\beta}(\varphi_1\varphi_2)\leqslant \sum q_{\gamma ,\beta}(\varphi_1)q_{\alpha-\gamma ,0}(\varphi_2) \tag{2}
$$

$$
\gamma
$$

$0\leqslant \gamma \leqslant \alpha$

for all $\alpha$ and $\beta \in \mathbf{N}^n$ (prop. 1 of IV, p. 196).

The canonical inclusion of $\mathscr{S}(\mathbf{R}^n)$ in the space $\mathscr{C}^{\infty}(\mathbf{R}^n)$, endowed with the topology described in No.$^o3$ of IV, p. 200, is continuous, since

sup$_{x\in K}|\partial^{\alpha}\varphi (x)|\leqslant q_{\alpha ,0}(\varphi )$

for every compact subset K of $\mathbf{R}^n$, every $\alpha \in \mathbf{N}^n$ and every Schwartz function $\varphi$.

#### Lemma 7 {#ts-iv-s3-lem-7 .statement tag=030Y}

Let $k\in \mathbf{N}$ and $\alpha \in \mathbf{N}^n$. For every function $\varphi \in \mathscr{S}(\mathbf{R}^n)$ and every real number $T>0$, one has

$_k\alpha$ 1

(3) $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant T$ sup $|\partial \varphi (x)|+\widetilde{q}_{\alpha ,k+1}(\varphi )$.

$\|x\|\leqslant T$ T

In fact, one has

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant$ sup$_{\|x\|\leqslant T}\|x\|^k|\partial^{\alpha}\varphi (x)|+$ sup$_{\|x\|>T}\|x\|^k|\partial^{\alpha}\varphi (x)|$

$\leqslant T^k$ sup$_{\|x\|\leqslant T}|\partial^{\alpha}\varphi (x)|+\frac{1}{T}$ sup$_{\|x\|>T}\|x\|^{k+1}|\partial^{\alpha}\varphi (x)|$.

#### Proposition 10 {#ts-iv-s3-prop-10 .statement tag=030Z}

Let B be a bounded subset of $\mathscr{S}(\mathbf{R}^n)$. The topology induced on B by $\mathscr{S}(\mathbf{R}^n)$ coincides with the topology induced by $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Since the inclusion of $\mathscr{S}(\mathbf{R}^n)$ in $\mathscr{C}^{\infty}(\mathbf{R}^n)$ is continuous, it is enough to prove that, for every open subset V of $\mathscr{S}(\mathbf{R}^n)$, the intersection $V\cap B$ is open in B for the topology induced by $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Let V be an open subset of $\mathscr{S}(\mathbf{R}^n)$. Let $\varphi_0\in V\cap B$. There exist a finite set I, a family $(\alpha_i, k_i)_{i\in I}\in (\mathbf{N}^n\times \mathbf{N})^I$ and a real number $\varepsilon  >0$ such that V contains the set of $\varphi \in \mathscr{S}(\mathbf{R}^n)$ satisfying

sup$_{i\in I}\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \varepsilon$.

Since B is bounded in $\mathscr{S}(\mathbf{R}^n)$, there exists $M>0$ such that the seminorms $\widetilde{q}_{\alpha_i,k_i+1}$ for $i\in I$ are bounded by M on B. Let $\delta  >0$ and $T>0$ be real numbers. By inequality (3), as soon as $\varphi \in B$ satisfies the bound

(4) sup$_{i\in I}$ sup$_{\|x\|\leqslant T}|\partial^{\alpha_i}(\varphi -\varphi_0)|\leqslant \delta$,

one has

$_k$ 2M

sup $\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \delta T$ +.

$_{i\in I}$ T

Let $T =\frac{4M}{\varepsilon}$, then $\delta =\frac{\varepsilon}{2T^k}$. One sees that $V\cap B$ contains the neighbourhood of $\varphi_0$ in B for the induced topology of $\mathscr{C}^{\infty}(\mathbf{R}^n)$ which is defined by (4). This concludes the proof.

#### Corollary {#ts-iv-s3-n7-cor-1 .statement tag=0310}

Let $(\varphi_m)_{m\in\mathbf{N}}$ be a bounded sequence in $\mathscr{S}(\mathbf{R}^n)$. For every function $\varphi \in \mathscr{S}(\mathbf{R}^n)$, the following assertions are equivalent:

a) The sequence $(\varphi_m)$ converges to $\varphi$ in $\mathscr{S}(\mathbf{R}^n)$;

b) The sequence $(\varphi_m)$ converges to $\varphi$ in $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Remark {#ts-iv-s3-n7-rem-2 .statement tag=0311}

A sequence $(\varphi_m)$ in $\mathscr{C}^{\infty}(\mathbf{R}^n)$ converges if and only if, for every $\alpha \in \mathbf{N}^n$, the sequence $(\partial^{\alpha}\varphi_m)$ converges to a function $\varphi^{(\alpha)}$ in $\mathscr{C}(\mathbf{R}^n)$ endowed with the topology of compact convergence. One then has $\varphi^{(\alpha)}=\partial^{\alpha}\varphi$ and $(\varphi_m)$ converges to $\varphi$[^0].

In fact, the condition is necessary. Conversely, if the sequences $(\partial^{\alpha}\varphi_m)$ converge to functions $\varphi^{(\alpha)}$ for every $\alpha \in \mathbf{N}^n$, then it follows from FVR, II, p. 2, th. 1, that $\varphi^{(\alpha)}=\partial^{\alpha}\varphi$[^0], which means that the sequence $(\varphi_m)$ converges to $\varphi$[^0] in $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Proposition 11 {#ts-iv-s3-prop-11 .statement tag=0312}

The space $\mathscr{S}(\mathbf{R}^n)$ is a Fréchet space and a Montel space.

Since the space $\mathscr{C}^{\infty}(\mathbf{R}^n)$ is complete (EVT, III, p. 9, example b)), the corollary to proposition 10 implies that every Cauchy sequence in $\mathscr{S}(\mathbf{R}^n)$ converges in $\mathscr{S}(\mathbf{R}^n)$ since it is bounded and converges in $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

The space $\mathscr{S}(\mathbf{R}^n)$ is therefore a Fréchet space; in particular, it is barrelled (EVT, III, p. 25, cor. to prop. 2). Let B be a bounded subset of $\mathscr{S}(\mathbf{R}^n)$ and $(\varphi_m)_{m\in\mathbf{N}}$ a sequence with values in B. Since $\mathscr{C}^{\infty}(\mathbf{R}^n)$ is a Montel space (EVT, IV, p. 18, example (4)), there exists a subsequence of $(\varphi_m)_{m\in\mathbf{N}}$ which converges in $\mathscr{C}^{\infty}(\mathbf{R}^n)$, hence in $\mathscr{S}(\mathbf{R}^n)$ (proposition 10). Therefore B is relatively compact in $\mathscr{S}(\mathbf{R}^n)$. It follows that $\mathscr{S}(\mathbf{R}^n)$ is a Montel space.

### 8. Inclusions of Function Spaces in the Space of Schwartz Functions

#### Proposition 12 {#ts-iv-s3-prop-12 .statement tag=0313}

The space $\mathscr{D}(\mathbf{R}^n)$ is contained in $\mathscr{S}(\mathbf{R}^n)$, and the inclusion of $\mathscr{D}(\mathbf{R}^n)$ in $\mathscr{S}(\mathbf{R}^n)$ is continuous with dense image.

Let $B\subset \mathscr{D}(\mathbf{R}^n)$ be a bounded subset, and let K be a compact subset of $\mathbf{R}^n$ such that $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. Let $\alpha \in \mathbf{N}^n$ and $k\in \mathbf{N}$. For every function $\varphi \in B$, one has

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant ($sup$_{x\in K}\|x\|^k)p_{\alpha ,K}(\varphi )$,

therefore B is bounded in $\mathscr{S}(\mathbf{R}^n)$. The continuity of the inclusion then follows from the fact that the spaces $\mathscr{S}(\mathbf{R}^n)$ and $\mathscr{D}(\mathbf{R}^n)$ are bornological.

Let us prove that $\mathscr{D}(\mathbf{R}^n)$ is dense in $\mathscr{S}(\mathbf{R}^n)$. Let B be the unit ball of $\mathbf{R}^n$ and let $\eta \in \mathscr{D}(\mathbf{R}^n)$ be a test function with support contained in 2B such that $0\leqslant \eta \leqslant 1$ and $\eta (x) = 1$ for every $x\in B$ (lemma 1, a) of IV, p. 196).

Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. For every integer $m\geqslant 1$ and every $x\in \mathbf{R}^n$, put $\eta_m(x) =\eta (x/m)$. Finally define $\varphi_m=\eta_m\varphi$; we have $\varphi_m\in \mathscr{D}(\mathbf{R}^n)$. Since $\partial^{\alpha}\eta_m=m^{-|\alpha|}(\partial^{\alpha}\eta )(x/m)$ for all $\alpha \in \mathbf{N}^n$ and $x\in \mathbf{R}^n$, one deduces from formula (2) of IV, p. 210 that the sequence $(\varphi_m)$ is bounded in $\mathscr{S}(\mathbf{R}^n)$.

Let C be a compact subset of $\mathbf{R}^n$. The sequence $(\varphi_m)_{m\geqslant 1}$ converges to $\varphi$ in $\mathscr{C}_K^{\infty}(\mathbf{R}^n)$ since $\varphi_m$ coincides with $\varphi$ on C for every sufficiently large $m$. Thus the sequence $(\varphi_m)$ converges to $\varphi$ in $\mathscr{C}^{\infty}(\mathbf{R}^n)$, and the corollary to proposition 10 of IV, p. 211 makes it possible to conclude that the sequence $(\varphi_m)$ converges to $\varphi$ in $\mathscr{S}(\mathbf{R}^n)$.

#### Lemma 8 {#ts-iv-s3-lem-8 .statement tag=0314}

Let B be a bounded subset of $\mathscr{D}(\mathbf{R}^n)$. The topology induced on B by the topology of $\mathscr{S}(\mathbf{R}^n)$ coincides with the topology induced by $\mathscr{D}(\mathbf{R}^n)$.

Since the inclusion of $\mathscr{D}(\mathbf{R}^n)$ in $\mathscr{S}(\mathbf{R}^n)$ is continuous, the topology on B induced by $\mathscr{D}(\mathbf{R}^n)$ is finer than that induced by $\mathscr{S}(\mathbf{R}^n)$. On the other hand, there exists a compact subset K of $\mathbf{R}^n$ such that $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. For every $\alpha \in \mathbf{N}^n$, one then has $p_{\alpha ,K}(\varphi )\leqslant \widetilde{q}_{\alpha ,0}(\varphi )$, which implies that the topology induced by $\mathscr{S}(\mathbf{R}^n)$ is finer than that induced by $\mathscr{D}(\mathbf{R}^n)$.

#### Proposition 13 {#ts-iv-s3-prop-13 .statement tag=0315}

Let $p\in [1,+\infty ]$. The space $\mathscr{S}(\mathbf{R}^n)$ is contained in $\mathscr{L}^p(\mathbf{R}^n)$ and the canonical injection of $\mathscr{S}(\mathbf{R}^n)$ into $\mathscr{L}^p(\mathbf{R}^n)$ is continuous. The image of $\mathscr{S}(\mathbf{R}^n)$ in $L^p(\mathbf{R}^n)$ is dense if $p\not = +\infty$.

The first assertion is immediate for $p= +\infty$. Henceforth suppose that $p\in [1,+\infty [$. Let $m$ be an integer such that $n+ 1< mp$. For every $\varphi \in \mathscr{S}(\mathbf{R}^n)$ and $x\in \mathbf{R}^n$, one has

$$
\|x\|^{n+1}|\varphi (x)|^p\leqslant \widetilde{q}_{0,m}(\varphi )^p
$$

hence $\varphi \in \mathscr{L}^p(\mathbf{R}^n)$ by Prop. 3 of IV, p. 199. Moreover, one obtains

$$
N_p(\varphi )\leqslant a^{1/p}_n\widetilde{q}_{0,0}(\varphi ) +b_n\widetilde{q}_{0,m}(\varphi )
$$

where

$$
a_n=\int d\mu(x),b_n=\int 1_{n+1}d\mu(x)
$$

$$
_{\|x\|\leqslant 1}\|_{x\|\geqslant 1}\|x\|
$$

hence the injection of $\mathscr{S}(\mathbf{R}^n)$ into $\mathscr{L}^p(\mathbf{R}^n)$ is continuous.

As the space $\mathscr{D}(\mathbf{R}^n)$ is contained in $\mathscr{S}(\mathbf{R}^n)$, Proposition 4 of IV, p. 202 implies that $\mathscr{S}(\mathbf{R}^n)$ is dense in $L^p(\mathbf{R}^n)$ if $p\not = +\infty$.

### 9. Functions with polynomial growth

#### Definition 3 {#ts-iv-s3-def-3 .statement tag=0316}

A function $f:\mathbf{R}^n\rightarrow \mathbf{C}$ has polynomial growth if there exists an integer $k\geqslant 1$ such that the mapping defined by $x\mapsto (1 +\|x\|)^{-k}f(x)$ is bounded on $\mathbf{R}^n$.

Every function with polynomial growth is locally bounded. Every polynomial function on $\mathbf{R}^n$ has polynomial growth.

#### Proposition 14 {#ts-iv-s3-prop-14 .statement tag=0317}

Let $f\in \mathscr{C}^{\infty}(\mathbf{R}^n)$. Suppose that for every $\alpha$ in $\mathbf{N}^n$, the function $\partial^{\alpha}f$ has polynomial growth. The linear mapping of the space $\mathscr{S}(\mathbf{R}^n)$ into itself defined by $\varphi \mapsto f \varphi$ is continuous.

For every $\varphi$ in $\mathscr{S}(\mathbf{R}^n)$, the function $f \varphi$ belongs to $\mathscr{C}^{\infty}(\mathbf{R}^n)$. By hypothesis, for every $\alpha \in \mathbf{N}^n$, there exist an integer $k_{\alpha}\geqslant 0$ and a real $C_{\alpha}$ such that $|\partial^{\alpha}f(x)|\leqslant C_{\alpha}(1 +\|x\|)^{k_{\alpha}}$ for every $x$ in $\mathbf{R}^n$. Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Let $\alpha \in \mathbf{N}^n$ and $k\in \mathbf{N}$. By Prop. 1 of IV, p. 196, there follows

$$
(\alpha )k\beta \alpha -\beta
$$

$\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum$ sup $\|x\||\partial f(x)\partial \varphi (x)|$

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

$$
(\alpha )kk\alpha -\beta
$$

$\leqslant \sum C_{\beta}$ sup $\|x\|(1 +\|x\|)^{^{\beta}}|\partial \varphi (x)|$.

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

Let $\beta \in \mathbf{N}^n$ be such that $0\leqslant \beta \leqslant \alpha$. For every $x\in \mathbf{R}^n$, one has

$\|x\|^k(1 +\|x\|)^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|\leqslant$ sup$_{\|x\|\leqslant 1}2^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$

+ sup$_{x\in\mathbf{R}^n}2^{k_{\beta}}\|x\|^{k+k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$ whence finally

$$
(\alpha )_k()
$$

$$
\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum 2^{^{\beta}}C_{\beta}\widetilde{q}_{\alpha-\beta ,0}(\varphi ) +\widetilde{q}_{\alpha-\beta ,k+k_{\beta}}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

which implies the proposition.

### 10. Tempered distributions

#### Definition 4 {#ts-iv-s3-def-4 .statement tag=0318}

The dual space of $\mathscr{S}(\mathbf{R})$ endowed with the topology of bounded convergence is called the space of tempered distributions on $\mathbf{R}^n$. It is denoted by $\mathscr{S}'(\mathbf{R}^n)$.

Since $\mathscr{S}(\mathbf{R}^n)$ is bornological, the space $\mathscr{S}'(\mathbf{R}^n)$ is complete (EVT, III, p. 24, cor. 1). Since $\mathscr{S}(\mathbf{R}^n)$ is a Montel space, the same is true of $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, prop. 9). The space $\mathscr{S}'(\mathbf{R}^n)$ is therefore reflexive (EVT, IV, p. 16, th. 2).

#### Lemma 9 {#ts-iv-s3-lem-9 .statement tag=0319}

A linear mapping $f$ of $\mathscr{S}(\mathbf{R}^n)$ into $\mathbf{C}$ is a tempered distribution if and only if for every family $(M_{\alpha ,k})_{(\alpha ,k)\in\mathbf{N}^n\times\mathbf{N}}$ in $\mathbf{R}_+$, the linear form $f$ is bounded on the set of functions $\varphi \in \mathscr{S}(\mathbf{R}^n)$ such that $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant M_{\alpha ,k}$ for every $(\alpha , k)\in \mathbf{N}^n\times \mathbf{N}$.

In fact, the space $\mathscr{S}(\mathbf{R}^n)$ is bornological (EVT, III, p. 12, prop. 2), and every bounded subset of $\mathscr{S}(\mathbf{R}^n)$ is contained in one of the bounded sets described in the statement.

#### Lemma 10 {#ts-iv-s3-lem-10 .statement tag=031A}

Let $\mathfrak{F}$ be a filter on $\mathscr{S}'(\mathbf{R}^n)$ having a countable base or containing a simply bounded set. Then $\mathfrak{F}$ converges to a tempered distribution if and only if $\langle f, \varphi \rangle$ converges along $\mathfrak{F}$ for every Schwartz function $\varphi$.

In particular, a sequence $(f_m)_{m\in\mathbf{N}}$ of tempered distributions converges to a tempered distribution $f$ if and only if one has $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Since $\mathscr{S}'(\mathbf{R}^n)$ is a Fréchet space, hence barrelled, (EVT, III, p. 25, cor. of prop. 2) the lemma results from the Banach-Steinhaus theorem (EVT, III, p. 26, cor. 3 of th. 1).

The canonical injection $j$ of $\mathscr{D}(\mathbf{R}^n)$ into $\mathscr{S}(\mathbf{R}^n)$ is continuous, and its image is dense (lemma 12 of IV, p. 212); hence the transpose of $j$, which is the restriction mapping of tempered distributions to the subspace $\mathscr{D}(\mathbf{R}^n)$, is an injective continuous linear mapping of $\mathscr{S}'(\mathbf{R}^n)$ into $\mathscr{D}'(\mathbf{R}^n)$. We shall identify $\mathscr{S}'(\mathbf{R}^n)$ with a subspace of $\mathscr{D}'(\mathbf{R}^n)$ by means of this mapping.

Let $\alpha \in \mathbf{N}^n$. The linear mapping $\varphi \mapsto \partial^{\alpha}\varphi$ of $\mathscr{S}(\mathbf{R}^n)$ into $\mathscr{S}(\mathbf{R}^n)$ is continuous. Its transpose is therefore a continuous linear mapping of $\mathscr{S}'(\mathbf{R}^n)$ into $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 6, cor., b)). The continuous linear mapping $(-1)^{|\alpha|t}\partial^{\alpha}$ of $\mathscr{S}'(\mathbf{R}^n)$ into $\mathscr{S}'(\mathbf{R}^n)$ is denoted by $\partial^{\alpha}$. This definition is compatible with Definition 2 of IV, p. 208 for distributions.

Let $h\in \mathscr{C}^{\infty}(\mathbf{R}^n)$ be a function such that $\partial^{\alpha}h$ has polynomial growth for every $\alpha \in \mathbf{N}^n$. The transpose of the continuous linear mapping $\varphi \mapsto h\varphi$ (prop. 14 of IV, p. 214) is a continuous linear mapping on $\mathscr{S}'(\mathbf{R}^n)$, denoted by $f\mapsto hf$.

### 11. Interpretation of functions as tempered distributions

#### Definition 5 {#ts-iv-s3-def-5 .statement tag=031B}

A measure $\nu$ on $\mathbf{R}^n$ is said to be tempered if there exists an integer $r\in \mathbf{N}$ such that the continuous mapping $x\mapsto (1 +\|x\|)^{-r}$ is $\nu$-integrable on $\mathbf{R}^n$.

In other words, a measure $\nu$ is tempered if there exists $r\in \mathbf{N}$ such that the function defined by $x\mapsto  \|x\|^{-r}$ is $\nu$-integrable on the complement of the unit ball in $\mathbf{R}^n$. In particular, every bounded measure on $\mathbf{R}^n$ is tempered. More generally, if $f$ is a $\mu$-measurable function of polynomial growth and if $\nu$ is tempered, then the measure $f\cdot \nu$ is tempered.

The set $\mathscr{M}^t(\mathbf{R}^n)$ of tempered measures on $\mathbf{R}^n$ is a subspace of the vector space $\mathscr{M}(\mathbf{R}^n;\mathbf{C})$ of complex measures on $\mathbf{R}^n$.

#### Proposition 15 {#ts-iv-s3-prop-15 .statement tag=031C}

Let $\nu$ be a tempered measure on $\mathbf{R}^n$. The restriction of $\nu$ to $\mathscr{S}(\mathbf{R}^n)$ is a tempered distribution. It is zero if and only if the measure $\nu$ is zero.

Since $\nu$ is tempered, there exists a positive integer $k$ such that the mapping $x\mapsto  \|x\|^{-k}$ is $\nu$-integrable on the complement of the unit ball in $\mathbf{R}^n$. For every Schwartz function $\varphi \in \mathscr{S}(\mathbf{R}^n)$, one has

$$
|\langle \nu , \varphi \rangle |\leqslant (\int_{\|x\|\leqslant 1}d\nu )\widetilde{q}_{0,0}(\varphi ) +(\int_{\|x\|>1}\|x\|^{-k}d\nu )\widetilde{q}_{0,k}(\varphi )
$$

therefore the restriction of $\nu$ to $\mathscr{S}(\mathbf{R}^n)$ is a tempered distribution.

The last assertion follows from Prop. 6 of IV, p. 206 since $\mathscr{D}(\mathbf{R}^n)$ is contained in $\mathscr{S}(\mathbf{R}^n)$.

We shall identify the space $\mathscr{M}^t(\mathbf{R}^n)$ with a subspace of $\mathscr{S}'(\mathbf{R}^n)$.

#### Proposition 16 {#ts-iv-s3-prop-16 .statement tag=031D}

Let $p\in [1,+\infty ]$ and $f\in \mathscr{L}^p(\mathbf{R}^n)$. Then the measure $f\cdot \mu$ with density $f$ with respect to Lebesgue measure is tempered. The mapping $f\mapsto f\cdot \mu$ of $L^p(\mathbf{R}^n)$ into $\mathscr{S}'(\mathbf{R}^n)$ resulting is continuous.

Let $q$ be the conjugate exponent of $p$ and let $r\geqslant 0$ be such that $rq > n$. For every $x\in \mathbf{R}^n$, let us write $g(x) = (1 +\|x\|)^{-r}$. The function $g$ belongs to $\mathscr{L}^q(\mathbf{R}^n)$ by Prop. 3 of IV, p. 199. By Hölder's inequality, one has

$$
\int_{\mathbf{R}^n}^*(1 +\|x\|)^{-r}|f(x)|d\mu(x)\leqslant N_q(g)N_p(f)<+\infty
$$

therefore the measure $f\cdot \mu$ is tempered.

Let $f\in L^p(\mathbf{R}^n)$ and $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Hölder's inequality implies

$$
|\langle f\cdot \mu, \varphi \rangle |=|\int_{\mathbf{R}^n}f(x)\varphi (x)d\mu(x)|\leqslant \|f\|_p\|\varphi \|_q
$$

and the continuity of the mapping $f\mapsto f\cdot \mu$ then follows from Prop. 13 of IV, p. 213.

For every $p\in [1,+\infty ]$, we shall identify $L^p(\mathbf{R}^n)$ with a subspace of $\mathscr{S}'(\mathbf{R}^n)$ by the linear mapping $f\mapsto f\cdot \mu$.

#### Proposition 17 {#ts-iv-s3-prop-17 .statement tag=031E}

The spaces $\mathscr{D}(\mathbf{R}^n)$ and $\mathscr{S}(\mathbf{R}^n)$ are dense in $\mathscr{S}'(\mathbf{R}^n)$.

It is enough to prove that $\mathscr{D}(\mathbf{R}^n)$ is dense in $\mathscr{S}'(\mathbf{R}^n)$. Let $\lambda$ be a continuous linear form on $\mathscr{S}'(\mathbf{R}^n)$ which is zero on $\mathscr{D}(\mathbf{R}^n)$. Since the space $\mathscr{S}(\mathbf{R}^n)$ is reflexive, there exists a function $\varphi \in \mathscr{S}(\mathbf{R}^n)$ such that $\lambda (f) =\langle f, \varphi \rangle$ for every $f\in \mathscr{S}'(\mathbf{R}^n)$. Hence

$$
0 =\lambda (\psi ) =\langle \psi , \varphi \rangle =\int_{\mathbf{R}^n}\psi \varphi  d\mu
$$

for every $\psi \in \mathscr{D}(\mathbf{R}^n)$. The measure $\varphi \cdot \mu$ on $\mathbf{R}^n$ is therefore zero (prop. 6 of IV, p. 206), whence $\varphi = 0$. The proposition then follows from the Hahn–Banach theorem (EVT, II, p. 46, cor. 1).

### 12. Fourier Transform of Tempered Distributions

Since every Schwartz function $\varphi$ is integrable on $\mathbf{R}^n$ (prop. 13 of IV, p. 213), it admits a Fourier transform $\mathscr{F}(\varphi )$ (resp. a Fourier cotransform $\overline{\mathscr{F}}(\varphi )$) which is identified with the continuous bounded function on $\mathbf{R}^n$ defined by

$y\mapsto \int\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$

(resp. with the function $y\mapsto \int^{\mathbf{R}^n}_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y$)$d\mu(x)$).

#### Lemma 11 {#ts-iv-s3-lem-11 .statement tag=031F}

Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. The function $\mathscr{F}(\varphi )$ is indefinitely differentiable on $\mathbf{R}^n$ and one has

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

for every $\alpha$ in $\mathbf{N}^n$.

One may suppose that $n\geqslant 1$. Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. The function defined by $(x, y)\mapsto \varphi (x)$ exp(2$i\pi x\cdot y$) from $\mathbf{R}^n\times \mathbf{R}^n$ into $\mathbf{C}$ satisfies the hypotheses of Corollary 1 of IV, p. 198 for every integer $k$. The Fourier transform of $\varphi$ is therefore indefinitely differentiable and satisfies

$\partial^{\alpha}(\mathscr{F}\varphi )(y) = (-2i\pi )^{|\alpha|}\int_{\mathbf{R}^n}x^{\alpha}\varphi (x)$ exp($-2i\pi x\cdot y$)$d\mu(x)$

for every $y\in \mathbf{R}^n$, which implies the first formula.

Let us prove the second formula. By induction on $|\alpha |$, it is enough to do so when $|\alpha |= 1$, and one is easily reduced to the case $\alpha = (1,0, . . . ,0)$. Write every $x\in \mathbf{R}^n$ in the form $x= (x_1, x')$ with $x'\in \mathbf{R}^{n-1}$, and denote by $\mu_1$ (resp. $\mu'$) the Lebesgue measure on $\mathbf{R}^{n-1}$ (resp. $\mathbf{R}$). By the Lebesgue-Fubini theorem (INT, V, p. 96, § 8, n$^o4$, th. 1), for every $y= (y_1, y')\in \mathbf{R}\times \mathbf{R}^{n-1}$, we get

$\mathscr{F}(\partial_1\varphi )(y) =\int$ exp($-2i\pi  x'\cdot y'$)

$\times^{\mathbf{R}^n}(\int^{^{-1}}_{\mathbf{R}}(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1))d\mu'(x')$.

For every compact interval $[a, b]$ in $\mathbf{R}$ and every $x'\in \mathbf{R}^{n-1}$, one has

$\int_a^b(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1) =$

$[\varphi (x_1, x')$ exp($-2i\pi  x_1y_1$)$]^b_a$

$+ 2i\pi y_1\int_a^b\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ by integration by parts (FVR, II, p. 10, formula (10)). When $a$ tends to $-\infty$ and $b$ tends to $+\infty$, the first term of the second member converges to 0 since $\varphi \in \mathscr{S}(\mathbf{R}^n)$. The second term converges, by the Lebesgue theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6), to

$2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$,

since the mapping $x_1\mapsto \varphi (x_1, x')$ is integrable on $\mathbf{R}$. As $x_1\mapsto \partial_1\varphi (x_1, x')$ is also integrable on $\mathbf{R}$, one deduces that

$\int_{\mathbf{R}}\partial_1\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$

$= 2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ and finally, applying the Lebesgue-Fubini theorem again, one concludes that

$\mathscr{F}(\partial_1\varphi )(y) = 2i\pi y_1\int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$,

as desired.

#### Proposition 18 {#ts-iv-s3-prop-18 .statement tag=031G}

The restriction to $\mathscr{S}(\mathbf{R}^n)$ of the Fourier transform is an automorphism of topological vector spaces whose inverse is the restriction of the cotransform of Fourier.

Let $\varphi \in \mathscr{S}(\mathbf{R}^n)$. By the preceding lemma, the Fourier transform of $\varphi$ belong to $\mathscr{C}^{\infty}(\mathbf{R}^n)$. Moreover, for $\alpha \in \mathbf{N}^n$ and $\beta \in \mathbf{N}^n$, one has

$$
X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi )) = (-2i\pi )^{|\alpha|}X^{\beta}\mathscr{F}(X^{\alpha}\varphi )
$$

$$
= (-1)^{|\alpha|}(2i\pi )^{|\alpha|-|\beta|}\mathscr{F}(\partial^{\beta}(X^{\alpha}\varphi ))
$$

In particular, the function $X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi ))$ is bounded. Since $\alpha$ and $\beta$ are arbitrary in $\mathbf{N}^n$, this means that $\mathscr{F}(\varphi )$ belongs to $\mathscr{S}(\mathbf{R}^n)$. Moreover, this calculation implies

$$
q_{\alpha ,\beta}(\mathscr{F}(\varphi ))\leqslant (2\pi )^{|\alpha|-|\beta|}\|\partial^{\beta}(X^{\alpha}\varphi )\|_1
$$

for $(\alpha , \beta )\in \mathbf{N}^n\times \mathbf{N}^n$ and $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Since the inclusion of the space $\mathscr{S}(\mathbf{R}^n)$ in $L^1(\mathbf{R}^n)$ is continuous (prop. 13 of IV, p. 213), the mapping $q_{\alpha ,\beta}\circ \mathscr{F}$ from $\mathscr{S}(\mathbf{R}^n)$ into $\mathbf{R}$ is continuous. It follows that the Fourier transform is continuous from the space $\mathscr{S}(\mathbf{R}^n)$ into itself (cf. EVT, II, p. 7, prop. 5, c)). One verifies analogously that the Fourier cotransform is continuous from the space $\mathscr{S}(\mathbf{R}^n)$ into itself. By the fourier inversion formula (theorem 3 of II, p. 222), the Fourier transform and the Fourier cotransform are reciprocal isomorphisms of one another.

#### Definition 6 {#ts-iv-s3-def-6 .statement tag=031H}

The transpose of the Fourier transform on $\mathscr{S}(\mathbf{R}^n)$ (resp. of the Fourier cotransform) is called the Fourier transform (resp. Fourier cotransform) on $\mathscr{S}'(\mathbf{R}^n)$.

The notation $\mathscr{F}$ (resp. $\overline{\mathscr{F}}$) is again used for the Fourier transform (resp. the Fourier cotransform) on $\mathscr{S}'(\mathbf{R}^n)$. The Fourier transform on $\mathscr{S}'(\mathbf{R}^n)$ is therefore an automorphism of topological vector spaces whose inverse is the Fourier cotransform. For every $f\in \mathscr{S}'(\mathbf{R}^n)$, the tempered distribution $\mathscr{F}(f)$ (resp. $\overline{\mathscr{F}}(f)$) is defined by the formula

$\langle \mathscr{F}(f), \varphi \rangle =\langle f,\mathscr{F}(\varphi )\rangle ($resp. $\langle \overline{\mathscr{F}}(f), \varphi \rangle =\langle f,\overline{\mathscr{F}}(\varphi )\rangle )$

for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Proposition 19 {#ts-iv-s3-prop-19 .statement tag=031I}

Let $f$ be a tempered distribution associated with a bounded measure $\nu \in \mathscr{M}^1(\mathbf{R}^n) ($resp. with $g\in L^2(\mathbf{R}^n))$. The Fourier transform of $f$ in $\mathscr{S}'(\mathbf{R}^n)$ is the tempered distribution associated with the Fourier transform of the measure $\nu ($resp. with the Fourier transform of g).

Let $\nu$ be a bounded measure on $\mathbf{R}^n$ and $f$ the tempered distribution associated with $\nu$. The Fourier transform $\mathscr{F}(\nu )$ is a continuous and bounded function on $\mathbf{R}^n$ (prop. 3 of II, p. 207). The tempered distribution associated with this function satisfies

$$
\langle \mathscr{F}(\nu ), \varphi \rangle =\int_{\mathbf{R}^n}\mathscr{F}(\nu )\varphi  d\mu=\int_{\mathbf{R}^n}\mathscr{F}(\varphi )d\nu =\langle f,\mathscr{F}(\varphi )\rangle =\langle \mathscr{F}(f), \varphi \rangle
$$

for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$, where the second equality is prop. 13 of II, p. 221, which is applicable here since the measure $\varphi \cdot \mu$ is bounded. The tempered distribution associated with $\mathscr{F}(\nu )$ is therefore $\mathscr{F}(f)$.

When $f$ is the tempered distribution associated with $g\in L^2(\mathbf{R}^n)$, one follows an entirely analogous procedure using formula (29) of II, p. 221.

A similar statement is also valid for the Fourier cotransform.

#### Remark {#ts-iv-s3-n12-rem-1 .statement tag=031J}

The elementary formulas concerning the Fourier transform of measures remain valid for the Fourier transform of tempered distributions. For example, for $f\in \mathscr{S}'(\mathbf{R}^n)$ and $\alpha \in \mathbf{N}^n$, one has

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

by lemma 11.

### 13. Distributions and tempered distributions on a vector space

Let $u$ be a bijective linear mapping of $\mathbf{R}^n$ into $\mathbf{R}^n$. The mapping $\varphi \mapsto \varphi \circ u$ is an automorphism of $\mathscr{S}(\mathbf{R}^n)$ (resp. of $\mathscr{D}(\mathbf{R}^n)$); its transpose is an automorphism of $\mathscr{S}'(\mathbf{R}^n)$ (resp. of $\mathscr{D}'(\mathbf{R}^n)$).

Let E be a finite-dimensional real vector space of dimension $n$. Let $v:\mathbf{R}^n\rightarrow E$ be an isomorphism of vector spaces. We denote by $\mathscr{S}(E)$ (resp. $\mathscr{D}(E)$) the set of mappings $\varphi : E\rightarrow \mathbf{C}$ such that $\varphi \circ v\in \mathscr{S}(\mathbf{R}^n)$ (resp. such that $\varphi \circ v\in \mathscr{D}(\mathbf{R}^n)$). From the preceding remark, this space does not depend on the choice of $v$; it is isomorphic to $\mathscr{S}(\mathbf{R}^n)$ (resp. $\mathscr{D}(\mathbf{R}^n)$). We denote by $\mathscr{S}'(E)$ (resp. $\mathscr{D}'(E)$) the dual of $\mathscr{S}(E)$ (resp. of $\mathscr{D}(E)$) endowed with the topology of bounded convergence. It is a topological vector space isomorphic to $\mathscr{S}'(\mathbf{R}^n)$ (resp. to $\mathscr{D}'(\mathbf{R}^n)$).

Let E and F be real vector spaces of dimension $n$, in duality relative to a bilinear form $b: E\times F\rightarrow \mathbf{R}$. The locally compact commutative group E is in duality with F relative to the mapping

$(x, y)\mapsto$ exp(2$i\pi b(x, y)$)

from $E\times F$ into $\mathbf{U}($cf. cor. 1 of II, p. 235). We endow E and F with Haar measures which are dual to one another relative to this mapping.

The space $\mathscr{S}(E)$ is contained in $L^1(E)$; the Fourier transform of E induces, by passing to subspaces and by duality, an isomorphism of topological vector spaces of $\mathscr{S}(E)$ onto $\mathscr{S}$ (F), whose transpose is an isomorphism of topological vector spaces of $\mathscr{S}'(F)$ onto $\mathscr{S}'(E)$.

### 14. Sobolev Spaces

Let U be an open set of $\mathbf{R}^n$. Let $p$ be a real number $\geqslant 1$ and $k$ a natural number. We denote by $W^{k,p}(U)$ the space of distributions $f\in \mathscr{D}'(U)$ such that, for every $\alpha \in \mathbf{N}^n$ with $|\alpha |\leqslant k$, the distribution $\partial^{\alpha}f$ is associated with an element of $L^p(U)$.

In particular, for $U =\mathbf{R}^n$, the elements of $W^{k,p}(U)$ are tempered distributions.

The mapping from $W^{k,p}(u)$ into $\mathbf{R}_+$ which associates to $f\in W^{k,p}(U)$

$$
\|f\|_{k,p}=((\sum_{|\alpha|\leqslant k}\|\partial^{\alpha}f\|^p_p)^{1/p}
$$

is a norm on $W^{k,p}(U)$. The space $W^{k,p}(U)$ will always be endowed with this norm; this normed space is called the Sobolev space of index $k$ and exponent $p$.

The space $\mathscr{D}(U)$ is contained in $W^{k,p}(U)$. We denote by $W^{k,p}_0$ (U) the closure of $\mathscr{D}(U)$ in $W^{k,p}(U)$. It is a closed subspace of $W^{k,p}(U)$.

We have $W^{k,p}_0(\mathbf{R}^n) = W^{k,p}(\mathbf{R}^n)$, but the spaces $W^{k,p}(U)$ and $W^{k,p}_0$ (U) are distinct in general (cf. Exercises 12 of IV, p. 334 and 14 of IV, p. 334).

We also denote by $H^k(U) = W^{k,2}(U)$ and $H^k_0(U) = W^{k,2}_0(U)$.

The norm of $H^k(U)$ is a prehilbertian norm, associated with the positive hermitian form on $H^k(U)$ defined by

$$
(f_1, f_2)\mapsto \sum_{|\alpha|\leqslant}\int_{kU}\overline{\partial^{\alpha}f_1}\partial^{\alpha}f_2d\mu
$$

The Hilbert space $H^k(U)$ coincides with the space denoted by $\mathscr{H}^k$ in EVT, V, p. 6, example (3).

One has $W^{0,p}(U) = L^p(U)$ and $H^0(U) = L^2(U)$ by definition; moreover $W^{0,p}_0(U) = L^p(U)$ by Proposition 4, b) of IV, p. 202.

#### Proposition 20 {#ts-iv-s3-prop-20 .statement tag=031K}

The Sobolev spaces $W^{k,p}(U)$ and $W^{k,p}_0$ (U) are Banach spaces of countable type. In particular, the spaces $H^k(U)$ and $H^k_0(U)$ are Hilbert spaces of countable type.

It is enough to prove the assertions concerning $W^{k,p}(U)$.

Let I be the set of $\alpha \in \mathbf{N}^n$ such that $|\alpha |\leqslant k$. The linear mapping $u$ of $W^{k,p}(U)$ into $L^p(U)^I$ which associates with $f$ the family $(\partial^{\alpha}f)_{\alpha\in I}$ is injective; it is continuous and strict by definition of the norm on $W^{k,p}(U)$. To prove that $W^{k,p}(U)$ is complete, it is enough to prove that its image under $u$ is closed. Now let $(f_n)_{n\in\mathbf{N}}$ be a sequence in $W^{k,p}(U)$ such that $(u(f_n))_{n\in\mathbf{N}}$ converges. Let $(g_{\alpha})_{\alpha\in I}\in L^p(U)^I$ be its limit. For $\alpha \in I$, the sequence $(\partial^{\alpha}f_n)_{n\in\mathbf{N}}$ converges in $L^p(U)$ to $g_{\alpha}$. A fortiori, the convergence takes place in $\mathscr{D}'(U)$. Put $f=g_0$. For every $\varphi \in \mathscr{D}$(U), one has

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

= lim$_{n\rightarrow+\infty}(-1)^{|\alpha|}\langle f_n, \partial^{\alpha}\varphi \rangle =$ lim$_{n\rightarrow+\infty}\langle \partial^{\alpha}f_n, \varphi \rangle =\langle g_{\alpha}, \varphi \rangle$.

This proves that $g_{\alpha}=\partial^{\alpha}f$ for every $\alpha \in I$, hence $(g_{\alpha})_{\alpha\in I}=u(f)$ belongs to the image of $u$.

The space $W^{k,p}(U)$ is identified by $u$ with a subspace of the space $L^p(U)^I$; the latter is of countable type (Proposition 2 of IV, p. 180 and TG, IX, p. 19, Corollary, (ii))), hence the same is true of $W^{k,p}(U) ($loc. cit., (i)).

#### Proposition 21 {#ts-iv-s3-prop-21 .statement tag=031L}

Let N be the euclidean norm on $\mathbf{R}^n$. Let $k$ be an integer $\geqslant 0$. The Sobolev space $H^k(\mathbf{R}^n)$ is the space of $f\in \mathscr{S}'(\mathbf{R}^n)$ such that $(1 + N^k)\mathscr{F}(f)$ belongs to $L^2(\mathbf{R}^n)$.

We proceed by induction on $k$. When $k= 0$, the result is a consequence of the Plancherel theorem (II, p. 215, th. 1). Suppose that $k= 1$. For $f\in \mathscr{S}'(\mathbf{R}^n)$, one has $(1 + N)\mathscr{F}f\in L^2(\mathbf{R}^n)$ if and only if $f\in L^2(\mathbf{R}^n)$ and $N\mathscr{F}f\in L^2(\mathbf{R}^n)$. Moreover, $N\mathscr{F}\in L^2(\mathbf{R}^n)$ if and only if, for every $\alpha \in \mathbf{N}^n$ such that $|\alpha |= 1$, one has $X^{\alpha}\mathscr{F}f\in L^2(\mathbf{R}^n)$. Since one has $\mathscr{F}(\partial^{\alpha}f) = 2i\pi X^{\alpha}\mathscr{F}f$, this condition means that $\mathscr{F}(\partial^{\alpha}f)\in L^2(\mathbf{R}^n)$ for every $\alpha$ with $|\alpha |= 1$, that is, $\partial^{\alpha}f\in L^2(\mathbf{R}^n)$ for every $\alpha$ with $|\alpha |= 1$. It follows that the assertion is true for $k= 1$.

Suppose now that $k\geqslant$ 2 and that the assertion concerning $H^{\ell}(\mathbf{R}^n)$ is valid for every positive integer $\ell \leqslant k-1$. Let $f\in \mathscr{S}'(\mathbf{R}^n)$. By definition, one has $f\in H^k(\mathbf{R}^n)$ if and only if $f\in L^2(\mathbf{R}^n)$ and, for every $\beta \in \mathbf{N}^n$ such that $|\beta |\leqslant 1$, the distribution $\partial^{\beta}f$ belongs to $H^{k-1}(\mathbf{R}^n)$. This is equivalent, by the induction hypothesis, to $f\in L^2(\mathbf{R}^n)$ and $(1 + N^{k-1})\mathscr{F}(\partial^{\beta}f)\in L^2(\mathbf{R}^n)$ for every $\beta \in \mathbf{N}^n$ such that $|\beta |\leqslant 1$. Since $\mathscr{F}(\partial^{\beta}f) = (2i\pi X)^{|\beta|}\mathscr{F}(f)$, the condition $f\in H^k(\mathbf{R}^n)$ is equivalent to saying that $\mathscr{F}f\in L^2(\mathbf{R}^n)$ and $(1 + N^{k-1})X^{\beta}\mathscr{F}f\in L^2(\mathbf{R}^n)$ for $\beta \in \mathbf{N}^n$ such that $|\beta |\leqslant 1$.

The inequalities

$$
1 + N^k\leqslant 1 + N^{k-1}\sum_{\beta|\beta\in|\mathbf{N}\leqslant 1^n}|X^{\beta}|\leqslant 1 +n^{1/2}N^k\leqslant (1 +n^{1/2})(1 + N^k)
$$

then imply that $f\in H^k(\mathbf{R}^n)$ if and only if $(1+N^k)\mathscr{F}\in L^2(\mathbf{R}^n)$.

## EXERCISES {#ts-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: Let us note that it is through an error that the statement of this proposition includes the case $p= +\infty$.
