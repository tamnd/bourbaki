---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 1
section_title: Polynomials
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0010-0023, 0095-0096
extraction: ocr
subsections:
    - "no": 1
      title: Definition of polynomials
      page: 0
      pdf_page: 10
    - "no": 2
      title: Degrees
      page: 2
      pdf_page: 11
    - "no": 3
      title: Substitutions
      page: 4
      pdf_page: 13
    - "no": 4
      title: Differentials and derivations
      page: 6
      pdf_page: 15
    - "no": 5
      title: Divisors of zero in a polynomial ring
      page: 9
      pdf_page: 18
    - "no": 6
      title: Euclidean division of polynomials in one indeterminate
      page: 10
      pdf_page: 19
    - "no": 7
      title: Divisibility of polynomials in one indeterminate [^1]
      page: 11
      pdf_page: 20
    - "no": 8
      title: Irreducible polynomials
      page: 13
      pdf_page: 22
statements: 30
exercises: 6
content_sha256: 1d8f9c22a127a64c14957180d868f7958bcc11142cd0d8fc8cb9430fbfe5e39c
translated_from: content/en/alg/IV/01_s1_polynomials.md
translation_method: google
source_content_sha256: f94b9470c6da2e74358afdf52f506465ae49993b41748514c1bc1d675c01f9e6
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 4916995e8c886f052def319f18a78d3e2e806d33252bc54c0661bf0899128a2c
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。多項式

### 1. 多項式の定義

$I$を集合とします。 (III、p. 452)、$I$ 上の$\mathbf{A}$ 上の自由な可換代数は $\mathbf{A}[(X_i)_{i \in I}]$ または $\mathbf{A}[X_i]_{i \in I}$ で表されることを思い出してください。 この代数の元は、$\mathbf{A}$の係数を含む不定数$X_i$（または不定数$X_i$）に関して*多項式*と呼ばれます。 Let us recall that the indeterminate $X_i$ is the canonical image of $i$ in the free commutative algebra on $I$ over $\mathbf{A}$; sometimes it is convenient to denote this image by another symbol such as $X'_i, Y_i, T_i$, etc. This convention is often introduced by a phrase such as: « Let $Y = (Y_i)_{i \in I}$ be a family of indeterminates »; in this case the algebra of polynomials in question is denoted by $\mathbf{A}[Y]$. $I = \{1, 2, \ldots, n\}$の場合、$\mathbf{A}[(X_i)_{i \in I}]$の代わりに$\mathbf{A}[X_1, X_2, \ldots, X_n]$を書き込みます。

$\nu \in \mathbf{N}^{(I)}$ には、

$$
X^\nu = \prod_{i \in I} X_i^{\nu_i}.
$$

すると、$(X^\nu)_{\nu \in \mathbf{N}^{(I)}}$ は $\mathbf{A}$ モジュール $\mathbf{A}[(X_i)_{i \in I}]$ の基底になります。 $X^\nu$ は不定数 $X_i$ の *単項式 * と呼ばれます。 $\nu = 0$ の場合、$\mathbf{A}[(X_i)_{i \in I}]$ の単位元が得られます。すべての多項式 $u \in \mathbf{A}[(X_i)_{i \in I}]$ は、形で正確に 1 つの方法で書くことができます。

$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$

ここで、$a_\nu \in \mathbf{A}$ と $\alpha_\nu$ は、有限の数を除いて零です。 $a_\nu$ は $u$ の *係数* と呼ばれます。 $\alpha_\nu X^\nu$ は、$u$ の *項* と呼ばれます (多くの場合、元 $\alpha_\nu X^\nu$ は、$X^\nu$ では項と呼ばれます)。特に、$a_0$ と識別される $\alpha_0 X^0$ の項は、*定数と呼ばれます$u$中項*。 $\alpha_\nu = 0$のとき、$X^\nu$では$u$*含むいいえ元*と言葉の乱用で言います。特に $\alpha_0 = 0$ の場合、$u$ は *定数項* (III, p. 453) を含まない多項式であると言います。 1 のスカラー 倍数は *定数多項式* と呼ばれます。

B を可換環および $\rho : A \to B$ 環準同型とします。 $B[(X_i)_{i \in I}]$を$\rho$によりA-代数とみなします。 Thus the mapping $\sigma$ of $A[(X_i)_{i \in I}]$ into $B[(X_i)_{i \in I}]$ which transforms $\sum \alpha_\nu X^\nu$ into $\sum \rho(\alpha_\nu) X^\nu$ is a homomorphism of A-algebras; if $u \in A[(X_i)_{i \in I}]$, we sometimes denote by $^\rho u$ the image of $u$ by this homomorphism. The homomorphism of $B \otimes_A A[(X_i)_{i \in I}]$ into $B[(X_i)_{i \in I}]$ canonically defined by $\sigma$ transforms, for every $i \in I$, $1 \otimes X_i$ into $X_i$; this is an isomorphism of B-algebras (III, p. 449).

M を基底 $(e_i)_{i \in I}$ で自由A-加群とします。対称代数 $S(M)$ を代数 $A[(X_i)_{i \in I}]$ に変換する単位準同型 $\varphi$ が正確に 1 つ存在し、各 $i \in I$ に対して $\varphi(e_i) = X_i$ となり、この準同型は同型 (III, p. 506）。この同型が正統であると言われています。これにより、対称代数の特定の特性を多項式代数に適用することができます。たとえば、$(I_1), \ldots, L$ を I の分割とします。 $\varphi_\lambda$を$P_\lambda = A[(X_i)_{i \in I_\lambda}]$の準同型を$P = A[(X_i)_{i \in I}]$に、変換$X_i$（$P_\lambda$の元）を$X_i$（Pの元に相当）とします。次に、代数 $\bigotimes_{h \in L} P_\lambda$ の $\varphi_\lambda$ 定義する準同型を代数 P に、
そして、この準同型は同型 (III、p. 503、提案 9) です。

EをA-加群とし、$E \otimes_A A[(X_i)_{i \in I}] = E[(X_i)_{i \in I}]$とします。 A-加群 $E[(X_i)_{i \in I}]$ の元は、E に係数を含む不定多項式 $X_i$ と呼ばれます。このような多項式は、$\sum_{\nu \in \mathbf{N}^{(I)}} e_\nu \otimes X^\nu$ のように 1 つの方法で書くことができます。ここで、$e_\nu \in E$ と $e_\nu$ は、a を除くすべてで零になります。有限の数の接尾辞。 $e_\nu \otimes X^\nu$ の代わりに $e_\nu X^\nu$ と書くことがよくあります。

### 2. 次数

$P = A[(X_i)_{i \in I}]$ を多項式代数とします。 それぞれの整数 $n \in \mathbf{N}$ について、$P_n$ を、$|\nu| = \sum_{i \in I} \nu_i$ が n に等しいような単項式 $X^\nu$ によって生成された P の部分加群とします。 次に、$(P_n), \ldots$ は、$A[(X_i)_{i \in I}]$ を型 $\mathbf{N}$ (III、p. 459) の段階的な代数に変える卒業です。 The homogeneous elements of degree $n$ in $A[(X_i)_{i \in I}]$ are sometimes called forms of degree $n$ with respect to the indeterminates $X_i$.

When we are dealing with the degree of inhomogeneous polynomials, we shall agree to adjoin to the set $\mathbf{N}$ of natural numbers, an element written $-\infty$ and to extend the order relation and the addition of $\mathbf{N}$ to $\mathbf{N} \cup \{-\infty\}$ by the following conventions, where $n \in \mathbf{N}$,

$$
-\infty < n , \quad (-\infty) + n = n + (-\infty) = -\infty , \quad (-\infty) + (-\infty) = -\infty .
$$

$u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu$ を多項式とします。 $u$ の次数 n の同次成分 $u_n$ (上で定義した型 N の目盛りの場合) は $\sum_{|\nu|=n} \alpha_\nu X^\nu$ に等しく、明らかに $u = \sum_{n \in \mathbf{N}} u_n$ が得られます。 $u \neq 0$ の場合、$u_n$ はすべて零ではなく、$u$ の *次数* (または *合計次数*) を定義するとして、数の最大のとして$\deg u$ と書きます。 $n$ は $u_n \neq 0$ になります。他の語 (III、p. 453) では、$u$ の次数は、$a_\nu \neq 0$ などのマルチインデックス $\nu$ の整数 $|\nu|$ の最大のです。 $u = 0$ の場合、$u$ の次数は慣例により $-\infty$ になります。 したがって、すべての整数 $p \in \mathbf{N}$ について、関係 $\deg u \leq p$ は、« $|\nu| > p$ を含むすべてのマルチインデックス $\nu$ について $a_\nu = 0$ » と等価です。 $\deg u \leq p$ が $A[(X_i)_{i \in I}]$ の A-部分加群となるような多項式 $u$ の集合は、上記の記法と$P_0 + P_1 + \ldots + P_p$ に等しくなります。

EをA-加群とします。ファミリ $(E \otimes P_n)_{n \in \mathbf{N}}$ は、E に係数をもつ多項式の加群 $E[(X_i)_{i \in I}] = E \otimes_A A[(X_i)_{i \in I}]$ の型 N の目盛です。この場合、不均一多項式の次数に対して上記で採用した規則を拡大する適用します。

#### 命題 1 {#alg-iv-s1-prop-1 .statement tag=069O}

*$u$ と $v$ を 2 つの多項式としましょう。*

(i) $\deg u \neq \deg v$ の場合、*持っています*
$$
u + v \neq 0 \quad \text{and} \quad \deg(u + v) = \sup(\deg u, \deg v).
$$
$\deg u = \deg v$ *私たちには* $\deg(u + v) \leq \deg u$ がある場合。

(ii) *$\deg(uv) \leq \deg u + \deg v$ があります*。
証明は明らかです。

$J \subset I$ と $B = A[(X_i)_{i \in I - J}]$ としましょう。 同一視する $A[(X_i)_{i \in I}]$ を $B[(X_i)_{i \in J}]$ (III, p. 453 f.) とします。 $u \in A[(X_i)_{i \in I}]$の次数、$B[(X_i)_{i \in J}]$の元と同様に、添字$i \in J$の$X_i$(III、p. 454)に関して$u$の次数と呼ばれます。

$u = \sum_{k=0}^n a_k X^k \in A[X]$ を 1 つの不定数における次数 $n$ の非ゼロ多項式とします。 仮定による$\neq 0$である係数 $a_n$は、$u$の*先頭の係数*と呼ばれます。先頭の係数が 1 に等しい *A* 多項式 $u \neq 0$ は、*首一多項式* と呼ばれます。

In $A[X_1, X_2, \ldots, X_q]$ 数 of monomials of total 次数 $p$ is equal to 数 of 元 $(n_k)_{1 \leq k \leq q}$ of $\mathbf{N}^q$ such that $\sum_{k=1}^q n_k = p$, that is $\binom{q+p-1}{p}$
(集合 III、提案 15、p. 182)

より一般的には、A を可換モノイド、および A の元の族である $(\delta_i)_{i \in I}$ とします。 各単項式 $X^\nu$ が次数 $\sum_{i \in I} \nu_i \delta_i$ (III、p. 458、例 3) となるように、代数 $A[(X_i)_{i \in I}]$ の型 A という固有の目盛りが存在します。 上で検討したケースは、$A = \mathbf{N}$ と $\delta_i = 1$ の場合です。 一般的な場合、混乱を避けるために、« 次数 » の代わりに語 « 重み » を使用し、« 均一» の代わりに« 等圧» を使用します。 たとえば、整数 $i \geq 1$ ごとに $X_i$ が重み $i$ となるような、代数 $A[(X_i)_{i \geq 1}]$ の型 N という固有の目盛りが存在します。 重み $n$ の等圧元は、形 $\sum a_{\nu} X^{\nu}$ の多項式であり、$\sum_{i \geq 1} i \cdot \nu_i \neq n$ の場合は $a_{\nu} = 0$ です。

### 3. 交代

E を $\mathscr{A}$ 上の単位結合代数とし、$x = (x_i)_{i \in I}$ を E のペアごとに置換可能な元の族とする。 $X = (X_i)_{i \in I}$ を不定値の族とする。 III、提案 7、p. 449 により、$i \in I$ ごとに $f(X_i) = x_i$ となるような、$\mathscr{A}[X]$ から $E$ への一意のユニタル準同型 $f$ が存在します。 The image of an element $u$ of $\mathscr{A}[X]$ under $f$ is written $u(x)$ and is called *the element of E obtained by substituting $x_i$ for $X_i$ in $u$*, or also *the value of $u$ for $X_i = x_i$*. 特に$u = u((X_i)_{i \in I})$。 $I = \{1, \ldots, n\}$ の場合、$u((x_i)_{i \in I})$ の代わりに $u(x_1, \ldots, x_n)$ を書き込みます。 より一般的には、M が A-加群で、o が の元である場合、

$$
M[(X_i)_{i \in I}] = M \otimes_A \mathscr{A}[(X_i)_{i \in I}],
$$

写像 $1_M \otimes f$ の下の $M \otimes_A E = M_{(E)}$ の $v$ の像を $v(x)$ で表します。

$\mathscr{A}[X]$ の E への準同型 $u \mapsto u(x)$ が単射である場合、族 $x$ は $\mathscr{A}$ に対して *代数的に自由* である、または $x_i$ は $\mathscr{A}$ に対して *代数的に独立* であると言います。これは、単項式 $x^{\nu}$ ($\nu \in \mathbf{N}^{(I)}$) が $\mathscr{A}$ 上で線形独立であることも意味します。

$\lambda$ が E の単位結合 A-代数 E' への単位結合準同型である場合、次のようになります。

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i)_{i \in I})) ,
$$

なぜなら、$\lambda \circ f$は$\mathscr{A}[X]$の準同型をE'に変換し、写像$X_i$を$\lambda(x_i)$に変換するからです。

$u \in \mathscr{A}[X]$ にしましょう。 $E$ が可換である場合、$E^1$ の E への写像 $x \mapsto u(x)$ は、$u$ (および代数 $E$) によって定義される *多項式関数* と呼ばれます。 ときどきを $\tilde{u}$ (または単に $u$) で表すことにします。

$Y = (Y_j)_{j \in J}$ を不定数族他のとし、E に多項式代数 $\mathscr{A}[Y]$ をとります。 $u \in \mathscr{A}[X]$ が与えられた場合、$i \in I$ に対して $g_i \in \mathscr{A}[Y]$ を取り、$g = (g_i)_{i \in I}$ を代入します。 $u$ の $X_i$ を多項式 $g_i$ に置き換えて得られる多項式を $u(g) \in \mathscr{A}/[Y]$ とします。 $y = (y_j)_{j \in J}$ を、単位結合 A-代数 E' のペアごとに置換可能な元の族とします。 適用 (1) と $E$ の $\mathscr{A}$ 準同型 $g \mapsto g(y)$ を $E'$ にすると、次のようになります。

$$
(u(g))(y) = u((g_i(y))) .
$$

$f = (f_i)_{i \in I} \in (\mathscr{A}[(X_j)_{j \in J}])^I$ と $g = (g_j)_{j \in J} \in (\mathscr{A}[(Y_k)_{k \in K}])^J$ の場合、多項式族 $(f_i(g))_{i \in I} \in (\mathscr{A}[(Y_k)_{k \in K}])^I$ を $f \circ g$ または $f(g)$ で表します。 ${E'}^J$ の $\tilde{f}$ 写像 $x \mapsto (f_i(x))_{i \in I}$ を ${E'}^I$ (ここで $E'$ は単位結合および可換 $A$-代数である) で表すと、関係 (2) は次のことを意味します。

$$(3)$$
$$(\mathrm{fog})'' = \tilde{f} \circ \tilde{g}.$$

$h = (h_k)_{k \in K} \in (A[(Z_l)_l \bullet_L])^K$ の場合、(2) から次のようになります。

$$(4)$$
$$f \circ (g \circ h) = (f \circ g) \circ h.$$

#### 命題 2 {#alg-iv-s1-prop-2 .statement tag=069P}

*$a = (a_i)_{i \in I}$を$A$の元の家族とし、$u \in A[X]$とします。 $v$ が、各 $i \in I$ の $X_i$ を $X_i + a_i$ に代入して得られる多項式である場合、$v$ の定数項は $u(a)$ に等しくなります。

$v$の定数項は、各$i \in I$の$v$の$X_i$に0を代入することで得られます。したがって、結果は (2) に従います。

#### 系 1 {#alg-iv-s1-prop-2-cor-1 .statement tag=069Q}

*$m$ を、$u(a) = 0$ となるような多項式 $u \in A[X]$ のイデアルとします。次に、$m$ は多項式 $X_i - a_i$ ($i \in I$ の場合) によって生成されます。*

$i \in I$ ごとに $X_i - a_i \in m$ であることは明らかです。 $u \in m$ と $v$ を提案 2 のようにします。 $v$ には定数項がないので、$A[X]$ と有限台の多項式の族 $(P_i)_{i \in I}$ が存在します。

$$
v(X) = \sum_{i \in I} X_i \cdot P_i(X).
$$

上式の各 $i \in I$ に対して置き換える $X_i$ を $X_i - a_i$ すると、形 $u(X) = \sum_{i \in I} (X_i - a_i) \cdot P'_i(X)$、よって系の関係が得られます。

#### 系 2 {#alg-iv-s1-prop-2-cor-2 .statement tag=069R}

*$X = (X_i)_{i \in I}$ と $Y = (Y_i)_{i \in I}$ を不定数の 2 つの族とする。 $u(X,X) = 0$ が多項式 $X_i - Y_i$ ($i \in I$ の場合) によって生成される $A[X,Y]$ の理想となるような多項式 $u \in A[X,Y]$ の集合。*

この系は Cor から直接生じたものです。 $A[Y]$ による置き換えること $A$ と $Y_i$ による $a_i$ で、$A[X,Y]$ を $X_i$ の多項式環として、$A[Y]$ の係数として解釈します。

#### 命題 3 {#alg-iv-s1-prop-3 .statement tag=069S}

*$u \in A[X]$ と $X.Z$ を、多項式環 $A[X][Z]$ の元の家族 $(X_iZ)_{i \in I}$ とします。 $u(X.Z)$ の $Z^k$ の係数は、正の整数 $k$ ごとに、次数 $k$ の$u$ の同次成分です。*

$u$ が単項式の場合、この Prop. を証明すれば十分であり、この場合、結果は明らかです。

#### 系 {#alg-iv-s1-n3-cor-1 .statement tag=069T}

*多項式 $u \in A[X]$ が次数 $k$ と同次であるためには、次のことが必要かつ十分です:*

$$
u(X.Z) = u(X) \cdot Z^k.
$$

#### 注意 {#alg-iv-s1-n3-rem-1 .statement tag=069U}

— $x \in A^I$ と $f$ を $A[X]$ の写像 $u \mapsto u(x)$ を $A$ にします。 $A$ モジュール $M$ が与えられた場合、$M[X] = M \otimes_A A[X]$ の準同型 $1 \otimes f$ を $M \otimes_A A = M$ に考慮します。それぞれの $v \in M[X]$ には $(1 \otimes f)(v) = v(x)$ があります。 $v = \sum_{\nu \in \mathbf{N}^{(I)}} e_\nu X^\nu$なら$v(x) = \sum_{\nu \in \mathbf{N}^{(I)}} x^\nu e_\nu$。

### 4. ディファレンシャルと導分

$B = A[(X_i)_{i \in I}]$ とすると、III、p. 569 により、各 $i \in I$ に対して、次のような B の A 導出$D_i$ が 1 つだけ存在します。
$$
D_i X_i = 1 , \quad D_i X_j = 0 \quad \text{for} \quad j \neq i
$$
多項式 $D_i P$ は、$X_i$ に関する * $P$ の *偏微分* と呼ばれます。また、$D_{X_i} P$ または $\frac{\partial P}{\partial X_i}$ または $P'_{X_i}$ で表すこともあります。 III、p. 558、公式 (21) までに、$\nu = (\nu,) \in \mathbf{N}^{(I)}$ については、
$$
D_i (X^\nu) = \begin{cases}
\nu_i X_i^{\nu_i - 1} \prod_{j \in I - \{i\}} X_j^{\nu_j} & \text{if } \nu_i > 0 \\
0 & \text{if } \nu_i = 0
\end{cases}
$$
(6) から、任意の $i, j \in I$ に対して $D_i D_j = D_j D_i$ が得られます。 $\nu = (\nu_i)_{i \in I} \in \mathbf{N}^{(I)}$ には、$D^\nu = \prod_{i \in I} D_i^{\nu_i}$ と $\nu! = \prod_{i \in I} (\nu_i!)$ を入れます。 積が $\mathbf{N}^{(I)}$ に注文すると、
$$
D^\nu(X^\mu) = \begin{cases}
\frac{\mu!}{(\mu - \nu)!} X^{\mu - \nu} & \text{if } \nu \leq \mu , \\
0 & \text{if not .}
\end{cases}
$$
$P$ が単一の不定数 $X$ の多項式である場合、$P$ の一意の偏導関数は $DP$ または $\frac{dP}{dX}$ または $P'$ と書かれ、単に $P$ の *導関数* と呼ばれます。

もう一度 $B = A[(X_i)_{i \in I}]$ とします。 $B$、$\Omega_A(B)$ の A 差動の III、p. 569 B-加群は、基底として $X_i$ の差動のファミリー $(dX_i)_{i \in I}$ を持ちます。 $\partial_i$ を、$\Omega_A(B)$ 上のこの基底に対する添字 $i$ の座標形とします。すると、B の写像 $u \mapsto (\partial_i, du)$ は、B の導分となり、$j \neq i$ に対して写像 $X_i$ が 1 になり、$X_j$ が 0 になるので、$D_i$ になります。他の語では、
$$
du = \sum_{i \in I} (D_i u) dX_i
$$
それぞれ$u \in B$。 I が有限である場合、$(D_i)_{i \in I}$ は B の B-加群の導分の基底です。

#### 命題 4 {#alg-iv-s1-prop-4 .statement tag=069V}

*E を結合的、可換的、単位的な A-代数、$x = (x_i)_{i \in I}$ を E の元の族、u $A[(X_i)_{i \in I}]$ と $y = u(x)$ の元とする。次に、E の導分 D を E モジュールに入れるごとに*
$$
Dy = \sum_{i \in I} (D_i u)(x) \cdot Dx_i .
$$

$u$ が単項式の場合、命題を証明すれば十分であり、その場合、III、p. 558、提案 6 に従います。

#### 系 {#alg-iv-s1-n4-cor-1 .statement tag=069W}

— *$1 \leq i \leq p$を$f \in A[X_1, ..., X_p]$と$g_i \in A[Y_1, ..., Y_q]$とし、$h = f(g_1, ..., g_p)$と書くと、$1 \leq j \leq q$は次のようになります*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j}.
$$

これは、提案 4 の特殊なケース $E = A[Y_1, ..., Y_r]$、$x_i = g_i$、および $D = \partial / \partial Y_j$ です。

$X = (X_i)_{i \in I}$、$Y = (Y_i)_{i \in I}$ を不定数の 2 つの互いに素族とし、その族 $(X_i + Y_i)_{i \in I}$ を $X + Y$ と書きます。 $u \in A[X]$ が与えられた場合、$A[X, Y]$ の元 $u(X + Y)$ を検討します。 For $\nu \in \mathbf{N}^{(I)}$ we denote by $A^\nu u$ the coefficient of $Y_\nu$ in $u(X + Y)$, considered as polynomial in the $Y_i$ with coefficients in $A[X]$. 定義までに$A^\nu u \in A[X]$があり、

$$
u(X + Y) = \sum_\nu (\Delta^\nu u)(X) Y^\nu.
$$

(この番号のここと残りの部分では、合計は添字集合 $\mathbf{N}^{(I)}$ 〜でない限りにわたって拡張されており、その逆が述べられています。)

$a \in A'$ として、(9) の $X$ に $a$ を、$Y$ に $X - a$ を代入すると、次のようになります。

$$
u(X) = \sum_\nu (\Delta^\nu u)(a)(X - a)^\nu.
$$

特に私たちは、

$$
u(X) = \sum_\nu (\Delta^\nu u)(0) X^\nu.
$$

$u, v \in A[X]$ の場合、

$$
(uv)(X + Y) = \left( \sum_\nu (\Delta^\nu u)(X) Y^\nu \right) \left( \sum_\rho (\Delta^\rho v)(X) Y^\rho \right)
= \sum_\sigma \left[ \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(X)(\Delta^\rho v)(X) \right] Y^\sigma
$$

したがって

$$
\Delta^\sigma(uv) = \sum_{\nu + \rho = \sigma} (\Delta^\nu u)(\Delta^\rho v).
$$

$Z = (Z_i)_{i \in I}$ を不定数の家族他のとします。

我々は持っています：

$$
\sum_{\nu} (\Delta^\nu u)(\mathbf{X})(\mathbf{Y} + \mathbf{Z})^\nu = u(\mathbf{X} + \mathbf{Y} + \mathbf{Z})
$$
$$
= \sum_{\sigma} (Au u)(\mathbf{X} + \mathbf{Y})Zu
$$
$$
= \sum_{\rho, \sigma} (\Delta^\rho \Delta^\sigma u)(\mathbf{X}) Y^\rho Z^\sigma u,
$$

したがって、I、p. 99、Cor によって作成されます。 2:

(13)
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u.
$$

#### 命題 5 {#alg-iv-s1-prop-5 .statement tag=069X}

— *すべての場合* $u \in \mathbf{A}[\mathbf{X}]$ *および* $\nu \in \mathbf{N}^{(I)}$ *私たちは*

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

まず、 $\nu$ に長さ 1 があると仮定します。その場合、I のすべての $j \neq i$ に対して $\nu = \varepsilon_i$、つまり $\nu_i = 1$ と $\nu_j = 0$ が存在するような I の元 $i$ が存在します。 公式 (12) は、$A''$ が A-代数 $\mathbf{A}[\mathbf{X}]$ の導分であることを示しています。これは明らかに、$j \neq i$ に対して $X_j$ に値零があり、$X_i$ に値 1 があります。したがって、それぞれの $i \in I$ に対して $\Delta^{\varepsilon_i} = D_i$ が得られます。

(13) までに、

(14)
$$
(\rho! \; \Delta^\rho) \cdot (\sigma! \; \Delta^\sigma) = (\rho + \sigma)! \; \Delta^{\rho + \sigma}
$$

A-加群 $\mathbf{A}[\mathbf{X}]$ の自己準同型環で。 $\nu$の長さに$\nu! \; A'' = D^\nu$の帰納法が続きます。

$\mathbf{A}$ が Q 代数である場合、式 (9)、(10)、(11) は次のように書くことができます。

(15)
$$
u(\mathbf{X} + \mathbf{Y}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(\mathbf{X}) \mathbf{Y}^\nu
$$
(16)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(a)(\mathbf{X} - a)^\nu
$$
(17)
$$
u(\mathbf{X}) = \sum_{\nu} \frac{1}{\nu!} (D^\nu u)(0) \; X^\nu
$$

式 (15)、(16)、(17) はいずれも « Taylor の公式 » と呼ばれる 3 つです。

#### 命題 6 (*« オイラーの恒等式 »*) {#alg-iv-s1-prop-6 .statement tag=069Y}

— *$u \in \mathbf{A}[\mathbf{X}]$ * を次数 r の同次多項式としましょう。我々は持っています*

$$
\sum_{i \in I} X_i \cdot D_i u = ru.
$$

D をそれ自体に $A[X]$ の A-線型写像とし、v が次数 s と同次のときに $D(v) = sv$ となるようにします。私たちは (III、p. 554、例 6) D が $A[X]$ の導分であることを知っています。したがって、提案 6 は提案 4 の系 (IV, p. 6) です。

### 5. 多項式環の零の因子

#### 命題 7 {#alg-iv-s1-prop-7 .statement tag=069Z}

— *$f \in A[X]$ を不定の非ゼロ多項式とし、$a$ をその先頭の係数とします。 $a$ が A でキャンセル可能である場合 (特にモニックである場合)、$A[X]$ の非ゼロの元'g が存在します。*

$$
fg \neq 0 \quad \text{and} \quad \deg(fg) = \deg f + \deg g
$$

$g \in A[X]$ をゼロ以外の多項式、$\beta$ をその先頭の係数、$n = \deg f$、$p = \deg g$ とします。すると、$fg$の$X^{n+p}$の係数は、消えない$\alpha \beta$、よって命題になります。

#### 命題 8 {#alg-iv-s1-prop-8 .statement tag=06A0}

— *A が整域の場合、$A[(X_i)_{i \in I}]$ も同様です。*

$u, v$ を $A[(X_i)_{i \in I}]$ の 2 つの非ゼロ元とします。 $uv \neq 0$ ということを示さなければなりません。ここで、$u$ と $v$ 属するから環 $A[(X_j)_{j \in J}]$ ここで、J は I の有限部分集合です。したがって、I が有限で、$\{1, 2, ..., p\}$ に等しい場合を極限知ることができます。一方、環 $A[X_1, ..., X_p]$ は、$A[X_1, ..., X_{p-1}]$ の係数と $X_p$ の多項式環と同型です。したがって、$p$ の帰納法までに、$A[X]$ では証明命題に減らされるので、提案 7 を適用するだけで十分です。

#### 系 1 {#alg-iv-s1-prop-8-cor-1 .statement tag=06A1}

— *A が整域で、$u, v$ が $A[(X_i)_{i \in I}]$ の元である場合、$\deg(uv) = \deg u + \deg v$ です。*

$u$ と $v$ がゼロ以外の場合は、極限で解決できます。 $m = \deg u, n = \deg v$ にしましょう。私たちは持っています

$$
u = u_0 + u_1 + \cdots + u_m, \quad v = v_0 + v_1 + \cdots + v_n
$$

ここで、$u_h$ (それぞれ $v_h$) は、次数 $h$ の $u$ (それぞれ v) の同次成分です。 $u_m \neq 0$ と $v_n \neq 0$ なので、$u_m v_n \neq 0$ になります (提案 8)。現在、$uv = u_m v_n + w$ と $\deg w < m + n$、よっての結果です。

#### 系 2 {#alg-iv-s1-prop-8-cor-2 .statement tag=06A2}

— *A が整域の場合、$A[(X_i)_{i \in I}]$ の可逆元は A の可逆元です。*

これはコルからすぐに続きます。 1.

#### 命題 9 {#alg-iv-s1-prop-9 .statement tag=06A3}

— *$u \in A[(X_i)_{i \in I}]$ としましょう。したがって、あなたが環 $A[(X_i)_{i \in I}]$ で nilpotent であるためには、すべての係数が環 A で nilpotent であることが必要かつ十分です。*

提案 8 の証明と同様に、1 つの変数 X の多項式の場合に帰着できます。 $u$ のすべての係数が nilpotent である場合、$u$ は nilpotent です (I、p. 99、Cor. 1)。 $u$ は零能ですが、零はそうではなく、$n$ をその次数とします。 $n$の帰納法までに議論します。 $a$ を $u$ の先頭の係数とします。 $u^m = 0$ となるような整数 $m > 0$ が存在します。 $u^m$ の先頭の係数は $a^m$ であるため、$a^m = 0$ になります。現在、$u - \alpha X^n$ は nilpotent であり (I、前述)、帰納法の仮定は $u - \alpha X^n$ のすべての係数が nilpotent であることを示しています。したがって、$u$ のすべての係数は無能です。

#### 注意 {#alg-iv-s1-n5-rem-1 .statement tag=06A4}

$u$と$v$を$A[(X_i)_i \in ,]$の元とし、$A$が整域、$v$が$u$の非ゼロ倍数、$v$が同次であると仮定します。その場合、$u$ も同次です。というのは、$u' \in A[(X_i)_i ,_1]$ を $v = uu'$ のようにするとします。 $u \neq 0$、$u' \neq 0$ があり、もし
$$
u = u_h + u_{h+1} + \cdots + u_k \\
u' = u_{h'} + u_{h'+1} + \cdots + u_{k'}
$$
$u$ と $u'$ の分解は、$u_h \neq 0$、$u_k \neq 0$、$u_{h'} \neq 0$、$u_{k'} \neq 0$ と同次の成分になり、その後、$v = u_h u_{h'} + u_h u_{h'+1} + \ldots + u_k u_{k'}$ と $u_h u_{h'}$ はゼロ以外の同次になります次数 $h + h'$ 一方、$u_k u_{k'}$ は次数 $k + k'$ と非ゼロ同次です (提案 8)。 $v$ は同次なので、$h + h' = k + k'$ よって $h = k$、$h' = k'$ となります。

### 6. ユークリッド 1 つの不定数での多項式の除算

#### 命題 10 {#alg-iv-s1-prop-10 .statement tag=06A5}

*$f$と$g$をそれぞれゼロ以外の元、$A[X]$、次数、$m$、$n$とします。 $\alpha_0$ を $f$ と $\mu = \sup(n - m + 1, 0)$ の先頭の係数とします。そのような$u, v \in A[X]$が存在します*
$$
\alpha_0^\mu g = uf + v, \quad \deg v < m.
$$
*$\alpha_0$が$A$でキャンセル可能な場合、$u$と$v$はこれらのプロパティによって一意に決定されます。

$n < m$ のとき、$u = 0$ と $v = g$ が取れるので、$u$ と $v$ の存在は明らかです。 $n \geq m$ については、$n$ に帰納法を用いるを実行します。 $\beta$ を $g$ の先頭の係数とします。 $f = \sum_{k=0}^m \alpha_k X^{m-k}$ の場合、$g_1 \in A[X]$ と $\deg g_1 < n$ を、$\alpha_0^\mu g = \alpha_0^\mu \beta X^n \cdot f + \alpha_0^{\mu-1} g_1$ と書くことができます。 帰納法の仮定までに、$\alpha_0^{\mu-1} g_1 = u_1 f + v$と$\deg v < m$のような$u_1, v \in A[X]$が存在します。したがって、
$$
\alpha_0^\mu g = (\alpha_0^{\mu-1} \beta X^{n-m} + u_1) f + v
$$
$u = \alpha_0^{\mu-1} \beta X^{n-m} + u_1$ を入れるだけで十分です。

$\alpha_0$が$A$でキャンセル可能であると仮定して、$u$と$v$の一意性を証明しましょう。 $u, v, u_1, v_1 \in A[X]$ を次のようにしましょう
$$
\alpha_0^\mu g = uf + v = u_1 f + v_1, \quad \deg v < m, \quad \deg v_1 < m
$$

$(u - u_1) f = v_1 - v$ と $\deg(v_1 - v) < m$ があるため、$u - u_1 = 0$ (IV、p. 9、提案 7)、したがって $v_1 - v = 0$ となります。

#### 系 (« ユークリッド多項式の除算 ») {#alg-iv-s1-n6-cor-1 .statement tag=06A6}

— Let $f$ be a non-zero element of $A[X]$ whose leading *coefficient* is invertible and $m = \deg f$.
(i) For every $g \in A[X]$ there exist $u,\ v \in A[X]$ such *that*
$$
g = uf + v , \quad \deg v < m .
$$
Moreover, these conditions determine $u$ and $v$ uniquely.
(ii) The sub-A-modules $A + AX + \ldots + AX^{m-1}$ and $fA[X]$ of $A[X]$ are supplementary in $A[X]$.
(iii) Assume $f$ non-constant and consider $A[X]$ as an $A[T]$-*module* by means of the homomorphism $u(T) \mapsto u(f(X))$ of $A[T]$ into $A[X]$. 次に、$A[X]$ は、基底 $(1, X, \ldots, X^{m-1})$ を含む無料の $A[T]$-*加群* です。
主張 (i) および (ii) は、提案 10 の明らか帰結です。
(iii) を証明しましょう。 $\psi$ を $A[T, X]$ の準同型 $v \mapsto v(f(X), X)$ を $A[X]$ にします。 まず、$A[T, X]$ を $T$ の多項式環と $A[X]$ の係数として考えます。 コル。 IV、p. 5の1は、$\psi$の核$a$が$A[T, X]$の理想的な$(T - f(X))$であることを示しています。 ここで、$A[T, X]$ を $X$ の多項式環と $A[T]$ の係数として考えてみましょう。この場合、$\psi$ は、$A[T][X]$ から $A[X]$ への $A[T]$ 線形マッピングです。 上記の主張 (ii) ($X$ の多項式 $f(X) - T$ と$A[T]$ の係数に適用) は、$(1, X, \ldots, X^{m-1})$ が $a$ を補足する $A[T, X]$ の $A[T]$ サブモジュールの基底であることを示しています。 整数 $i \geq 0$ ごとに $\psi(X^i) = X^i$ なので、(iii) がすぐに続きます。

(i) の記法について、$u$ は商であり、$v$ は $g$ を $f$ でユークリッド割った余りです。残りが消えるためには、$f$ が割る $g$ になることが必要かつ十分です。

### 7. 1 つの不定数における多項式の割り算 [^1]

#### 命題 11 {#alg-iv-s1-prop-11 .statement tag=06A7}

— $K$ を可換 *体* とします。
(i) $K[X]$ のゼロ以外のすべての理想値 $a$ に対して、 $a = (f )$ となるような 1 つの *モニック* 多項式 $f$ が $K[X]$ に存在します。
(ii) $f_1$ と $f_2$ を $K[X]$ に入れる。 $(f_1) = (f_2)$ が成立するには、$f_2 = \lambda f_1$ となるような $K$ の非ゼロ元 $\lambda$ が存在することが必要かつ十分です。
(ii) を証明しましょう。記載された条件の十分性は明らかです。 $f_1$ と $f_2$ 生成する零が理想的な場合は自明です。したがって、非ゼロ多項式 $f_1$ と $f_2$ 生成するは、同じ理想の $K[X]$ であると仮定します。次に、$f_1 = u_1 f_2$ と $f_2 = u_2 f_1$ のような多項式 $u_1$ と $u_2$ が存在します。 u_1 u_2 = 1、よって $\deg u_1 + \deg u_2 = 0$ となり、$\deg u_2 = 0$ となります。したがって、$u_2$ は $K$ の非ゼロ元であることが示されました。

(i) を証明するには、$f$ を、最小可能性のある次数の $a$ におけるモニック多項式とする。 $a$で$g$が与えられた場合、$u$と$v$を商と、$g$を$f$で割ったユークリッドの余りとします。次に、$v = g - u f$ 属するから $a$ となり、$\deg v < \deg f$ になります。 $v$ がゼロ以外の場合、$\lambda v$ がモニックとなるような $K$ の非ゼロ元 $A$ が存在し、$\lambda v \in a$ 以降、これは定義オフと矛盾します。 したがって、$a = (f)$ になります。首一多項式 $f$ の一意性により、(ii) から $a = (f)$ が得られます。

#### 命題 12 {#alg-iv-s1-prop-12 .statement tag=06A8}

*$K$を可換体、$f, g$を$K[X]$の2つの元とします。 $K[X]$ のすべての多項式 $d$ について、次のプロパティは同等です*:

(i) *多項式 $d$ 割る $f$ および $g$ と、$f$ と $g$ 割る $d$* の両方である割るのすべての多項式。

(ii) *多項式 $d$ 割る $f$ および $g$ と、$d = u f + v g$* となる 2 つの多項式 $u$ および $v$ が存在します。

(iii) $K[X]$* の理想の間には *関係 $(d) = (f) + (g)$ が成り立ちます。

*多項式 $d$ は、これらの性質により、$K$ の非ゼロ元によって乗法まで決定されます。 $f$ と $g$ が両方とも零ではない場合、$d$ の $d \neq 0$ と次数は、$f$ と $g$* を分割するすべての多項式の次数を多数決します。

$f$と$g$が零のとき、(i)～(iii)の各性質は$d = 0$についてのみ満たされるため、等価になります。以降、$f, g$ は両方とも 0 ではないと仮定し、$K[X]$ の理想的な $(f) + (g)$ を $a$ で表します。

$K[X]$ の多項式 $u$ と $v$ について、プロパティ $(u) \supset (v)$ と « $u$ 割る $v$ » は同等であることに注意してください。したがって、主張 (ii) は、« $(d) \supset (f)$ および $(d) \supset (g)$ および $d \in (f) + (g)$ »、つまり (iii) と同等です。 (ii) が (i) を意味することは明らかです。最後に、(i) が成り立つと仮定します。 $(d) \supset (f)$ と $(d) \supset (g)$、よって $(d) \supset a$ があります。一方、提案 11 (IV, p. 12) により、$a = (d_1)$ のような多項式 $d_1$ が存在します。 $d_1$ 割る $f$ と $g$ の両方から、仮定、よって $(d) \subset a$ によって割る $d$、そして最後に$(d) = a$、つまり (iii) が得られます。

提案 12 の他の主張は、提案 11 の明らか帰結を理想 $a = (f) + (g)$ に適用したものです。

#### 定義 1 {#alg-iv-s1-def-1 .statement tag=06A9}

*提案 12 の記法により、$d$ は $f$ と $g$ の最大の共通の因子 (略して gcd) であると言えます。 $f$ と $g$ は相対的に素である、または $1$ が $f$ と $g$* の gcd である場合、$f$ は $g$ に対して素であると言います。

$f$ と $g$ が相対的に素であるということは、$K[X]$ に $u f + v g = 1$ となるような多項式 $u$ と $v$ が存在することを意味します。

#### 系 1 {#alg-iv-s1-def-1-cor-1 .statement tag=06AA}

*$d$ を $f$ と $g$ の gcd とし、$K'$ 可換体含む $K$ を部分体とします。この場合、$d$ は $f$ の gcd であり、$g$ は $K'[X]$* の元と見なされます。

これは提案 12、(iii) から導き出されます。

#### 系 2 {#alg-iv-s1-def-1-cor-2 .statement tag=06AB}

— d を gcd off とし、g とします。
    (i) $u \in K[X]$ の場合、du は fu と gu の gcd です。
    (ii) $v \in K[X]$ が f と g の因子 ($\neq 0$) である場合、$d/v$ は $f/v$ と $g/v$ の gcd です。
    これは提案 12 の (ii) から導き出されます。

#### 系 3 {#alg-iv-s1-def-1-cor-3 .statement tag=06AC}

— w を f と g の共通の因子とします。 w が gcd off および g であるためには、$f/w$ と $g/w$ が互いに素であることが必要かつ十分です。
    これはコルからの続きです。 2.

#### 系 4 {#alg-iv-s1-def-1-cor-4 .statement tag=06AD}

— $f, g, h \in K[X]$ にしましょう。 f 割る gh で g に対して素数の場合、f 割る h です。
    f 割る gh および fh の場合、したがって、gh および fh のすべての gcd、特に h (Cor. 2、(i)) は f 割るになります。

#### 系 5 {#alg-iv-s1-def-1-cor-5 .statement tag=06AE}

— $f, g \in K[X]$ にしましょう。 fand g が相対的に素であるためには、$K[X]/(f)$ の g の標準像が可逆であることが必要かつ十分です。
    この条件は、$uf + vg = 1$のような$u, v \in K[X]$が存在することを意味します。

#### 系 6 {#alg-iv-s1-def-1-cor-6 .statement tag=06AF}

— $f, g_1, g_2, ..., g_n \in K[X]$ としましょう。 f が $g_1, g_2, ..., g_n$ に対して素数である場合、f は $g_1g_2...g_n$ に対して素数です。

\* 系 7. — f と g が互いに素であるためには、それらが K のどの拡大にも共通の根を持たないことが必要かつ十分です。
    なぜなら、d が f の gcd である場合、g から f への根共通のと、K の拡大 K' における g は、K' における d の根です。ここで、系は、V、p. 21、提案 4 から続きます。

### 8. 既約多項式

#### 定義 2 {#alg-iv-s1-def-2 .statement tag=06AG}

— K を可換体とします。 $\deg f \geq 1$ があり、f が $0 < \deg g < \deg f$ のような多項式 g で割り切れない場合、$f \in K[X]$ は既約であると言います。
    $K[X]$ の f の $\deg f \geq 1$ と唯一の因子は、スカラー $\neq 0$ による f のスカラー $\neq 0$ と積であると言うのも同じことになります。 関係 $(f) \subset (g)$ は g 割る f を意味するので、$K[X]$ の既約多項式も、理想 $(f)$ が最大 (I, p. 104) となるような多項式 f として定義できることがわかります。

    $f, g \in K[X]$ にしましょう。 ff が既約であれば、f と g が互いに素であるか、f 割る g であることが明らかです。 f と g が既約の場合、f と g は互いに素であるか、またはそれぞれがスカラー $\neq 0$ だけ他方の積になります。特に、2 つの異なる既約モニック多項式は比較的素です。

#### 命題 13 {#alg-iv-s1-prop-13 .statement tag=06AH}

— $\mathscr{I}$ を $K[X]$ の既約モニック多項式の集合とします。 f を 0 以外の元または $K[X]$ とその先頭の係数とします。その場合、有限台を含む正の整数 $(v_p)_{p \in \mathscr{S}}$ のファミリーが正確に 1 つ存在し、分解が得られます。

$$
f = \alpha \prod_{p \in \mathscr{S}} p^{v_p}.
$$

$f$ がモニックのとき、つまり $\alpha = 1$ のとき、命題を証明すれば十分です。 次数 $n$ オフの帰納法までに議論することにしますが、$n = 0$ のケースは自明です。次に、次数 $< n$ のすべての多項式に対して $n \geq 1$ と命題が確立されたとします。

$E$ をモニック多項式 $\neq 1$ の集合とし、割る $f$ とします。 $f \in E$ があるため、$E$ は空ではなく、$E$ には最小次数の多項式$g$ が存在します。 $g$ が既約であり、$f = gh$ となるような次数 $< n$ のモニック多項式 $h$ が存在することは明らかです。 帰納法の仮定による $h$ は、既約モニック多項式の有限族の積であるため、$f$ は同じ性質を持ちます。これは分解 (18) の存在を証明します。

分解の一意性 (18) を証明しましょう。 $(w_p)_{p \in \mathscr{S}}$ を有限台を含む正の整数の族とし、$f = \prod_{p \in \mathscr{S}} p^{w_p}$ とします。 $f$ は次数 $n \geq 1$ であるため、$w_p > 0$ となるような $p \in \mathscr{S}$ が存在します。 $v_p = 0$ があった場合、$f$ は、$p$ とは異なる $\mathscr{S}$ の元の族の積となるため、次の事実に反して、$p$ (IV, p. 13, Cor. 6) に対して素数になります。 $p$ 割る $f$。 帰納法の仮定までに、多項式 $f/p$ は型 (18) の一意の分解を認めます。したがって、$q \in \mathbf{4}$ ごとに結論する等式 $w_q = v_q$ となります。

$f$ を $\mathbf{K}[X]$ の非ゼロ多項式とする。 分解 (18) の指数 $v_p$ がすべて $\leq 1$ である場合、$f$ には倍数因子がないと言えます。 $f$ はペアごとに別個の既約多項式の有限列の積である、あるいは、$f$ は非定数多項式 $\mathbf{K}[X]$ の平方で割り切れない、ということも同じことになります。

### 練習問題 {#alg-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。

[^1]: 読者は、この番号と次の番号の結果の類似性と、整数 (I、p. 112) の環 $Z$ の割り算特性に注目するでしょう。 それらは本質的に、章 VII, § 1 でわかるように、環 $Z$ と $K[X]$ ではすべての理想が主要であるという事実に依存しています。
