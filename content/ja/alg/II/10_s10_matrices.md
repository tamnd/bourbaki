---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 10
section_title: Matrices
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 338-363, 417-424
pdf_pages: 0362-0387, 0441-0448
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF MATRICES
      page: 338
      pdf_page: 362
    - "no": 2
      title: MATRICES OVER A COMMUTATIVE GROUP
      page: 339
      pdf_page: 363
    - "no": 3
      title: MATRICES OVER A RING
      page: 341
      pdf_page: 365
    - "no": 4
      title: MATRICES AND LINEAR MAPPINGS
      page: 342
      pdf_page: 366
    - "no": 5
      title: BLOCK PRODUCTS
      page: 346
      pdf_page: 370
    - "no": 6
      title: MATRIX OF A SEMI-LINEAR MAPPING
      page: 347
      pdf_page: 371
    - "no": 7
      title: SQUARE MATRICES
      page: 349
      pdf_page: 373
    - "no": 8
      title: CHANGE OF BASES
      page: 352
      pdf_page: 376
    - "no": 9
      title: EQUIVALENT MATRICES; SIMILAR MATRICES
      page: 354
      pdf_page: 378
    - "no": 10
      title: TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING
      page: 356
      pdf_page: 380
    - "no": 11
      title: TRACE OF A MATRIX
      page: 358
      pdf_page: 382
    - "no": 12
      title: MATRICES OVER A FIELD
      page: 359
      pdf_page: 383
    - "no": 13
      title: EQUIVALENCE OF MATRICES OVER A FIELD
      page: 360
      pdf_page: 384
statements: 35
exercises: 17
content_sha256: e4104ace66f7790ca228b3e62ca8d2d1716cf43e8043d498c449195c2833a61e
translated_from: content/en/alg/II/10_s10_matrices.md
translation_method: google
source_content_sha256: 9f20d99617c7f5aad6362a5f7207c5eb84fe7bf5906f6a9107df6de45c2d511a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: ff258d1d78c8918fcd64f80fa6e8a8af18a3596d3db4fbf78928372e30f47918
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 10。 行列

### 1. 行列中定義

#### 定義 1 {#alg-ii-s10-def-1 .statement tag=05WH}

$I, K, H$ を 3 集合とします。 $H$ に元が含まれる型 $(I, K)$ の行列 (または $H$ 上の型 $(I, K)$ の行列) は、$H$ の元の $M = (m_{i\kappa})_{(i, \kappa) \in I \times K}$ のファミリーです。 集合は積 $I \times K$ です。 すべての $i \in I$ について、ファミリー $(m_{i\kappa})_{\kappa \in K}$ は添字 $i$ の $M$ の行と呼ばれます。すべての $\kappa \in K$ に対して、家族 $(m_{i\kappa})_{i \in I}$ は列、$M$、添字 $\kappa$ と呼ばれます。

$I$ (それぞれ $K$) が有限である場合、$M$ は有限の行数 (それぞれ列) を持つ行列であると言われます。 The set of matrices of type $(I, K)$ over $H$ is identified with the product $HI^{I \times K}$.

「行」と「列」という名前は、$I$と$K$が$\mathbf{N}$の区間$[1, p], [1, q]$、行列の元が$p$行の長方形配列の集合として想定されるという事実から生じています。 (水平に配置) および $q$ 列 (垂直に配置):

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdots & \cdots & \cdots & \cdots \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

$p$ と $q$ が明示的に整数で実行可能である場合、上記の配列は問題の行列を効果的に表すシンボルであるというのが慣例です。この記法により、添字の使用を省略できます。元の添字は配列内の位置によって決定されることが理解されます。たとえば、行列について話すとき

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

行列 $(m_{ij})_{1 \leq i < 2, 1 \leq j < 3}$ という意味です

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

Instead of matrix of type $([1, p], [1, q])$, we also say matrix of type $(p, q)$, or matrix with $p$ rows and $q$ columns, if no confusion arises; the set of matrices of type $(p, q)$ over $H$ is sometimes denoted by $\mathbf{M}_{p, q}(H)$.

インデックス付け集合 $I, K$ の 1 つが空である、$H$ 上のすべての行列は、$H$ の元の空のファミリーと同一です。空の行列とも呼ばれます。 $I = \{i_0\}$ (それぞれ $K = \{k_0\}$) が 1 つの元の集合からなるであるとき、$M$ は行行列 (それぞれ列行列) とその行 (それぞれ列) と呼ばれます。 添字は記法で抑制できます。 $I$と$K$が両方とも集合で、片方が元である場合、型$(I, K)$の行列は、この行列の一意元と同一視されることがよくあります。

行列 $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$ のサブファミリー $M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L}$ は、そのインデックス付け集合が部分集合の積 $I$ の $J$ および $K$ の部分集合 $L$ であり、 行列 $M$;それは、添字 $\kappa \notin L$ の添字 $\iota \notin J$ と列の行 $M$ を *抑制*することで得られると言われています。逆に、$M$ は、$M'$ を添字 $\kappa \notin L$ の添字 $\iota \notin J$ と列の行で *境界付ける* ことによって得られると言われます。

#### 定義 2 {#alg-ii-s10-def-2 .statement tag=05WI}

*行列* $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$ の *転置、*で示される* $^tM$、*は行列* $(m'_{\kappa \iota})_{(\kappa, \iota) \in K \times I}$ *上* $H$ *によって与えられます* $m'_{\kappa \iota} = m_{\iota \kappa}$ *すべて* $(\iota, \kappa) \in K \times L$。

この定義から、型 $(I, K)$ の行列の転置は型 $(K, I)$ の行列であることがわかります。

(1)
$$
^t(^tM) = M.
$$

### 2. 可換群に対する行列

$G$ を可換群 (加法的に書く) とします。 $G$ 上の行列の集合は、指定されたインデックス集合 $I, K$ で、$I \times K$ から写像の集合であるため、*可換群* 構造になります。 $G$;この群は加法的に書かれているため、$M = (m_{\iota \kappa})$ と $M' = (m'_{\iota \kappa})$ がその元の 2 つである場合、
$$
M + M' = (m_{\iota \kappa} + m'_{\iota \kappa});
$$
したがって、この群の単位元は行列で、その元はすべて *零* (*零行列* と呼ばれます) です。明らかに
(2)
$$
^t(M + M') = ^tM + ^tM'.
$$

したがって、2 つの行列のうち和は、行のインデックス付け集合と列が 2 つの行列で *同じ* である場合にのみ定義されます。

$H', H''$ を 2 つの集合、$G$ を可換群 (加法的に書く)、および $H' \times H''$ から $G$ までの $f : (h', h'') \mapsto h'h''$ 写像とします。 2 つの行列を与えます
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \quad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
$M'$の列のインデックス付け集合$K$が*有限*であり、$M''$の行のインデックス付け集合、*の*積と等しいように、それぞれ$H'$と$H''$を超えます。 $M'M''$ または $f(M', M'')$ で示される $M'$ および $M''$ *経由* $f$ は、行列
(3)
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
$G$以上。

上記の定義は、$M'$ の列のインデックス付け集合が $M''$ の行のインデックス付け集合と等しいと仮定しています。特に積 $M''M'$ *$I \neq L$ の場合は意味がありません。 公式 (3) $M'$ の *同じ* 行の元に、右側の $M''$ の *同じ* 列の元を掛けます。 乗法は「列による行」と言われています。

$f^0$ を $H'' \times H'$ ～ $G$ の写像 $(h'', h') \mapsto h'h''$ とします。 定義からすぐに次のことが続きます。
$$
t(M'M'') = tM''.tM'
$$
ここで、左側 (右側) の積は、$f$ (それぞれ $f^0$) によって計算されます。

$H'$ と $H''$ がそれ自体可換群 (加法的に書かれる) であり、$f$ が $\mathbf{Z}$-*双線形* (§ 3, no. 1) である場合、分配公式は
$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$
和と積が出現するようにインデックス付け集合が定義されます。

ここで、$H_1, H_2, H_3, H_{12}, H_{23}$ と $H$ を可換群 (加法的に書く)、$f_{12}:H_1 \times H_2 \to H_{12}, f_{23}:H_2 \times H_3 \to H_{23}$ 写像とします。
$$
f_3:H_{12} \times H_3 \to H, \quad f_1:H_1 \times H_{23} \to H
$$
$\mathbf{Z}$-双線形写像;さらに、すべて $x_i \in H_i \ (i = 1, 2, 3)$ だと仮定します。
$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$
(上記 $(x_1 x_2)x_3 = x_1(x_2 x_3)$ のように書くこともできます);次に、$M' = (m'_{rs}), M'' = (m''_{st}), M''' = (m'''_{tu})$ がそれぞれ行列 $H_1, H_2, H_3$ を超えている場合、
$$
(M'M'')M''' = M'(M''M'''')
$$
両側の積 (それぞれ $f_{12}, f_3, f_{23}$ と $f_1$ で計算) が定義されている場合。のために
$$
\sum_t \left( \sum_s m'_{rs} m''_{st} \right) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} \left( \sum_t m''_{st} m'''_{tu} \right)
$$
立てられた仮説のおかげで。

(6) の両辺も$M'M''M'''$で表されます。 3 つ以上の因子のうちの積についても、同様の規則が作成されます。

#### 注意 {#alg-ii-s10-n2-rem-1 .statement tag=05WJ}

上記の式拡大するをより一般的な状況に当てはめます。正確に言うと:

(a) 各 $G_{\iota \kappa}$ が加法的に書かれた可換群である $H = \bigcup_{(\iota, \kappa) \in I \times K} G_{\iota \kappa}$ を仮定します。次に、和 $M + M'$ は、注文された対 $(\iota, \kappa)$、$m_{\iota \kappa} \in G_{\iota \kappa}$、$m'_{\iota \kappa} \in G_{\iota \kappa}$ ごとに定義される可能性があります。

(b) I、K、L を 3 集合とし、K を有限と仮定し、$H' = \bigcup_{(i, k) \in I \times K} H'_{ik}$、$H'' = \bigcup_{(k, l) \in K \times L} H''_{kl}$、$H = \bigcup_{(i, l) \in I \times L} H_{il}$ を 3 集合とします。各 $H_{il}$ が加法的に書かれた可換群であると仮定し、各トリプル $(i, k, l)$ について
$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$
写像になります。 次に、$M' = (m'_{ik})_{(i, k) \in I \times K}$、$M'' = (m''_{kl})_{(k, l) \in K \times L}$ が行列で、すべての $i, k, l$ に対して $m'_{ik} \in H'_{ik}$ と $m''_{kl} \in H''_{kl}$ が成り立つ場合、$f_{ikl}$ を介して定義する積 $M'M''$ ができます。 (4)、(5)、(6) に類似した式を書き留めて証明書く作業は読者に任せます。

### 3. 行列環

数学で最も重要な行列は、環 A 上の行列です。集合行列の $A^{I \times K}$ 対応するから集合 I をインデックスすると、K は標準的に (A, A) バイモジュール構造 (§ 1, no. 14) になります。

注文されたすべての対 $(i, k) \in I \times K$ について、$E_{ik}$ を行列 $(a_{jl})$ とし、$(j, l) \neq (i, k)$ に対して $a_{ik} = 1$ と $a_{jl} = 0$ を定義します。 $E_{ik}$ は、行列 $A^{I \times K}$ の集合では行列単位と呼ばれます。 I と K が有限であれば、この集合の左の形標準基底または右A-加群構造 (§ 1, no. 11) になります。明らかに
$$
tE_{ik} = E_{ki}.
$$

Unless otherwise mentioned, the product $M'M''$ of two matrices over A (assumed to be defined) will always be understood to be relative to the multiplication $(x, y) \mapsto xy$ in A (or, as is also said, will be "calculated in A"). 次に、 (no. 2) 結合性と分配性の公式が得られます。

(7)
$$(XY)Z = X(YZ)$$

(8)
$$
\begin{cases}
X(Y + Z) = XY + XZ \\
(X + Y)Z = XZ + YZ
\end{cases}
$$
3 つの行列 X、A 上の Y、Z については、これらの式に現れる和と積が定義されている場合に限ります。

特に、$E_{ik}$ (それぞれ $E'_{kl}, E''_{il}$) がそれぞれ $A^{I \times K}$ (それぞれ $A^{K \times L}, A^{I \times L}$) で行列単位である場合、$I = \{1, p\}, K = \{1, q\}, L = \{1, r\}$ を使用すると、次の式が得られます。
$$
\begin{cases}
E_{ik}E'_{jl} = 0 & \text{if } k \neq j \\
E_{ik}E'_{kl} = E''_{il}.
\end{cases}
$$

$A^0$ を A の反対環とし、$a * b \ (= ba)$ を $A^0$ の a と b の積とします。次に、2 つの行列 X について、積が定義されている A 上の Y、
$$(10)$$
$$
t(XX) = tY * tX
$$

ここで、右側の$^tY$と$^tX$は、$\mathbf{A}^0$の元を含む行列と見なされます。 $\mathbf{A}$ が *可換* の場合、

$$(11)$$
$$
^t(XY) = ^tY.^tX
$$

#### 命題 1 {#alg-ii-s10-prop-1 .statement tag=05WK}

*$\mathbf{A}, \mathbf{B}$ を 2 つの環と $M = (m_{ik})_{(i,k) \in I \times K}$ とし、*
$$
M' = (m'_{ik})_{(i,k) \in I \times K}
$$
* 2 つの行列と、* $(\mathbf{A}, \mathbf{B})$*-bimodule* $G$ 上の有限インデックス付け集合 。 *すべての行列単位* $L = (a_i)_{i \in I}$ *1 つの行と元が $\mathbf{A}$ * およびすべての行列単位* $C = (b_k)_{k \in K}$ * 1 つの列と元が* $\mathbf{B}$、$L.M.C = L.M'.C$ であると仮定します。 (*積は、* $(\mathbf{A}, \mathbf{B})$* モジュール* $G$ の外部法則を介して計算されます);それから* $M = M'$。

$L$を行列単位$(a_s)$とし、$s \neq i$を$a_i = 1, a_s = 0$とし、$C$行列単位$(b_t)$を$t \neq k$を$b_k = 1, b_t = 0$とすると、積 $L.M.C$ と $L.M'.C$ は行列で、単一の元はそれぞれ $m_{ik}$ と $m'_{ik}$ に等しくなります。

$\mathbf{A}, \mathbf{B}$ を 2 つの環と $\sigma : \mathbf{A} \to \mathbf{B}$ 準同型とします。

$\mathbf{A}$ 上のすべての行列 $M = (m_{ik})$ を、$\mathbf{B}$ 上の $\sigma(M)$ 行列 $(\sigma(m_{ik}))$ で表します。明らかに $a \in \mathbf{A}$ に対して $\sigma(aM) = \sigma(a)\sigma(M)$、$\sigma(Ma) = \sigma(M)\sigma(a)$、また $\sigma(^tM) = (^t(\sigma(M)))$ と

$$(12)$$
$$
\begin{cases}
\sigma(M + M') = \sigma(M) + \sigma(M') \\
\sigma(MM') = \sigma(M)\sigma(M')
\end{cases}
$$
*考慮される演算が定義されている場合、(12) の左側と右側の積は * $\mathbf{A}$ * と* $\mathbf{B}$ * でそれぞれ計算されます。* $\sigma$ が $x \mapsto x^\sigma$ で表される場合、$\sigma(M)$ の代わりに $M^\sigma$ と書きます。

特に、$\mathbf{A}$ の *反同型性* $\sigma$、つまり $\mathbf{A}$ から反対環 $\mathbf{A}^0$ の準同型、または $\mathbf{A}$ の写像を次のように考えます。
$$
\sigma(a + a') = \sigma(a) + \sigma(a'), \qquad \sigma(aa') = \sigma(a')\sigma(a)
$$
*全員に* $a, a'$ *in* $\mathbf{A}$;次に、積 $MM'$ が定義されている $\mathbf{A}$ 上の 2 つの行列 $M, M'$ について、
$$(13)$$
$$
\sigma(MM') = (^t(\sigma(^tM')).\sigma(^tM))
$$
*ここで、両側の積は * $\mathbf{A}$ で計算されます。 *これは (10) と (12) の直後に続きます。*

### 4. 行列と線形写像

$\mathbf{A}$ を環とし、$E$ を *(右または左)* $\mathbf{A}$* モジュール* として基底 $(e_i)_{i \in I}$ を許容します。すべての元 $x \in E$ について、基底* $(e_i)$ に対する * $x$ の *行列は、$M(x)$ または $\mathbf{x}$ (または、混乱が生じない場合はときどきは単に $x$) で示されます。 *列行列* $(e_i)$ (§ 1, no. 11) に関しては、成分のからなる $x$ の $x_i \ (i \in I)$。計算では、ときどきが便利です。位数では、添字$i$が行添字であることを覚えて、それに隣接する列添字を1つだけ取り、値を1つだけ取り、行列$M(x)$と書くと便利です。 $(x_{i0})$として。

ここで、2 つの (左または右) A-加群 E および F と、それぞれ基底 $(e_i)_{i \in I}$ および $(f_k)_{k \in K}$ を考えます。 $(f_k^*)$ を形対応するから $(f_k)$ までの座標系とする。 E から F への線形写像 $u$ について、次の各ケースで、基底* $(e_i), (f_k)$ に関して u の定義する *行列を計算します。

(D) E と F は右A-加群、$u$ は A-linear です。
(G) E と F は左A-加群、$u$ は A-linear です。

以下では、式適用の右 (左) 加群に文字 (D) (それぞれ (G)) を付けます。

#### 定義 3 {#alg-ii-s10-def-3 .statement tag=05WL}

*上記 2 つのケースのそれぞれで、基底* $(e_i), (f_k)$ に対する u の行列は行列* $M(u) = (u_{ki})_{(k, i) \in K \times I}$ *そのような*

$$
u_{ki} = f_k^*(u(e_i))
$$

*それぞれ*と書かれます

(14D)
$$
u_{ki} = \langle f_k^*, u(e_i) \rangle
$$
(14G)
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$

したがって、添字 $i$ の $M(u)$ の *列* は $M(u(e_i))$ に等しいです。

明らかに、$u, v$ が E の 2 つの線形写像を F に変換し、$M(u), M(v)$ の行列を同じ基底に対して結合したものである場合、次のようになります。

$$
M(u + v) = M(u) + M(v)
$$
そして
$$
M(\gamma u) = \gamma M(u)
$$
A の *中心* $\Gamma$ のすべての元 $\gamma$ に対して。他の語では、基底 $(e_i), (f_k)$ が固定されると、写像 $u \mapsto M(u)$ は、A の *$\Gamma$ モジュール同型* になります。 $\mathrm{Hom}_A(E, F)$ を集合 $A^{K \times I}$ の部分集合に、K が *有限* の場合、$A^{K \times I}$ に等しい。

#### 命題 2 {#alg-ii-s10-prop-2 .statement tag=05WM}

*I と K が有限であると仮定します。すべての元* $x \in E$、*行列* $M(u(x))$ *基底* $(f_k)$ * は公式* で与えられます

(17D)
$$
M(u(x)) = M(u) . M(x)
$$
(17G)
$$
{}^t M(u(x)) = {}^t M(x) . {}^t M(u).
$$

例えば(17G)を確認します。 $x = \sum_i x_{i0} e_i, \quad u(x) = \sum_k y_{k0} f_k$ を $x_{i0} \in A, \ y_{k0} \in A$ とします。次に$u(x) = u\left( \sum_i x_{i0} e_i \right) = \sum_i x_{i0} u(e_i) = \sum_{i, k} x_{i0} u_{ki} f_k$; よって y_{k0} = \和_i x_{i0} u_{ki}。 位数では、2 つの添字 $i$ を 1 つの他のと並べて、転置行列 ${}^t M(x) = (x'_{0i})$ を考慮します。ここで、$x'_{0i} = x_{i0}$ と
$$
{}^t M(u) = (u'_{ik}),
$$
ここで$u'_{ik} = u_{ki}$;次に $y_{k0} = \sum_i x'_{0i} u'_{ik}$ で、右側は添字の元行列の $k$ で、${}^t M(x) \cdot {}^t M(u)$、よってが 1 行あります (17 G)。

A が可換のとき、(17 G) 簡約するは、no. 2 の公式 (4) によって (17 D) になります。

#### 系 {#alg-ii-s10-n4-cor-1 .statement tag=05WN}

*Let E, F, G be three right (resp. left) modules over a ring A, $(e_i)_{i \in I}$, $(f_k)_{k \in K}$, $(g_l)_{l \in L}$ respective finite bases of E, F, G, $u : E \to F$, $v : F \to G$ two linear mappings, $M(u)$ the matrix of u relative to the bases $(e_i)$, $(f_k)$, $M(v)$ the matrix of v relative to the bases $(f_k)$, $(g_l)$ and $M(v \circ u)$ the matrix of $v \circ u$ relative to the bases $(e_i)$, $(g_l)$; then*

(18D)
$$
M(v \circ u) = M(v) M(u)
$$
(18G)
$$
{}^t M(v \circ u) = {}^t M(u) {}^t M(v).
$$

たとえば (18 G) を証明します。すべての $x \in E$ の場合、(17 G) で:
$$
{}^t M(x) \cdot {}^t M(v \circ u) = {}^t M(v(u(x))) = {}^t M(u(x)) \cdot {}^t M(v) = {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(v)
$$
結合性による。 行列 ${}^t M(x)$ の 1 行は任意であるため、no. 3、命題 1 から系が続きます。

*注意 (1)*。 公式 (17 D) は (18 D) の特殊なケースと考えることができます。というのは、$x \in E$ 線形写像 $\theta_x : A_d \to E$ 写像それぞれの $\alpha \in A$ から $x \alpha$ (§ 2, no. 1) には、標準的に対応するがあるからです。 $A_d$ の基底 1 と E の基底 $(e_i)$ に対して行列 $M(\theta_x)$ は行列 $M(x)$ であるのは明らかです。同様に、$M(\theta_{u(x)}) = M(u(x))$ と公式 (17 D) は、関係の翻訳と考えることができます。
$$
\theta_{u(x)} = u \circ \theta_x.
$$

#### 命題 3 {#alg-ii-s10-prop-3 .statement tag=05WO}

*E、FをそれぞれEとFの右(それぞれ左)2つA-加群と$(e_i)_{i \in I}$、$(f_k)_{k \in K}$有限基底とする。 E から F へのすべての線形写像 u について、基底 $(e_i)$ および $(f_k)$ に関して、$M(u)$ を u の行列とします。この場合、双対基底 $(f_k^*)$ と $(e_i^*)$ に関して ${}^t u : F^* \to E^*$ の行列は ${}^t M(u)$ に等しくなります。*

E は、正準的に、その双対の $E^{**}$ および $(e_i)$ と $(e_i^*)$ の双対基底で識別されます。次に (たとえば、E と F が正しいと仮定します加群)
$$
\langle {}^t u(f_k^*), e_i \rangle = \langle f_k^*, u(e_i) \rangle,
$$
よって命題。

#### 注意 {#alg-ii-s10-n4-rem-1 .statement tag=05WP}

(2) E と F を 2 つの左A-加群とし、それぞれ基底 $(e_i)_{i \in I}$ と $(f_k)_{k \in K}$ とします。 A-線型写像 $u : E \to F$ ごとに (14 G)、$u(e_i) = \sum_k u_{ki} f_k$;これらの関係は、というによって、列行列 $(u(e_i))_{i \in I}$ (F に元が含まれる) は積 $^tM(u) \cdot (f_k)$ に等しいと解釈できます。ここで、$(f_k)_{k \in K}$ は列行列と見なされます。 F に元を使用し、A-加群 F (no. 2) で作用の法則を定義する写像 $A \times F \to F$ に対して積が計算されます。

(3) A, B を 2 つ可換環と $\sigma : A \to B$ 環準同型とする。 命題 3 の記法では、$(e_i \otimes 1)$ と $(f_k \otimes 1)$ はそれぞれ $E_{(B)} = E \otimes_A B$ と $F_{(B)} = F \otimes_A B$ の基底 (§ 5, no. 1、命題 4) です。さらに、$(e_i^*)$ と $(f_k^*)$ がそれぞれ $(e_i)$ と $(f_k)$ の二重基底である場合、$(e_i^* \otimes 1)$ と $(f_k^* \otimes 1)$ はそれぞれ $(e_i \otimes 1)$ と $(f_k \otimes 1)$ の二重基底になります。 (§ 5, no. 4)。すべてのA-線型写像 $u : E \to F$ について、$M(u)$ と $M(u \otimes 1)$ を、$(e_i)$ に関して$u$ の行列とし、$(f_k)$ と行列をB-線型写像 $u \otimes 1$ とします。 $(e_i \otimes 1)$と$(f_k \otimes 1)$。 § 5, no. 4, 公式 (20) から次のようになります。
$$
M(u \otimes 1) = \sigma(M(u)).
$$

有限な未知数数における右スカラー線形方程式の有限数の系を考えてみましょう。
$$
\sum_{i \in I} a_{kt} x_i = b_k \quad (k \in K)
$$
Aに$a_{kt}, x_i, b_k$が入っています。

$(e_i)_{i \in I}, (f_k)_{k \in K}$ を $E = A_d^I$ と $F = A_d^K$ の正規の基底とします。 系 (19) は方程式 $u(x) = b$ と等価です。ここで、$x = \sum_i e_i x_i$、$b = \sum_k f_k b_k$、$u : E \to F$ は線形写像であるため、基底 $(e_i)$ および $(f_k)$ に関して行列 $M(u)$ は次と等しくなります。 $A = (a_{kt})_{(k, i) \in K \times L}$。この行列を一次方程式(19)の系の行列と呼びます。 (§ 2, no. 8、注意 2 および 3) を思い出してください。$c_i = \sum_k f_k a_{kt}$, 系 (19) を書くことは、固有のベクトル方程式と同等です。
$$
\sum_i c_i x_i = b,
$$
そして、$c_i$ は行列 $A$ の添字 $i$ の列であるため、系 (19) が解を認めると言うのは、行列がというになることになることがわかります。 $b = (b_{k0})$ と 1 つの列は、行列 $A$ の列の線形結合です。

左一次方程式の系に対する類似の定義と注意を定式化する作業は読者に任せます。

### 5. ブロック積

no. 4 の定義は次のように一般化できます。 E を、部分加群の家族 $(E_i)_{i \in I}$ の (右または左) A-加群、直和とします。 すべての $x \in E$ について、すべての $i \in I$ について $x_i \in E_i$ を使用して $x = \sum_{i \in I} x_i$ とします。 E の元を含む列行列 $M(x) = (x_i)_{i \in I}$ は、E の分解 $(E_i)_{i \in I}$ である直和* に対して x の *行列であると言えます。

Let F be another A-module (E and F being both right A-modules or both left A-modules) and suppose that F is the direct sum of a family $(F_k)_{k \in K}$ of submodules. For all $u \in \mathrm{Hom}(E, F)$ and all $x_i \in E_i$, let $u(x_i) = \sum_k u_{ki}(x_i)$ with $u_{ki}(x_i) \in F_k$ for all $k \in K$; then $u_{ki} \in \mathrm{Hom}(E_i, F_k)$; we shall say that the matrix $M(u) = (u_{ki})_{(k, i) \in K \times I}$ of type $(K, I)$ with elements in the set H the sum of the $\mathrm{Hom}(E_i, F_k)$ is *the matrix of u with respect to the decompositions $(E_i)$ and $(F_k)$ of E and F as direct sums*.

これらの定義により、$u, v$がEの2つのA-線型写像をFにすると、行列は同じ分解と直和に関して明らかです。

$$
M(u + v) = M(u) + M(v), \qquad M(\gamma u) = \gamma M(u)
$$

A の中心の元 $\gamma$ ごとに (no. 2、*注意*)。

さらに、$u_{ki}$ の定義は、K が有限である場合、次のように書けることを示しています。

$$
M(u(x)) = M(u) . M(x)
$$

where $M(u(x))$ is the matrix of $u(x)$ with respect to the decomposition $(F_k)$, the product on the right hand side of (22) being calculated for the mappings $(t, z) \mapsto t(z)$ of $\mathrm{Hom}(E_i, F_k) \times E_i$ into $F_k$ (no. 2, *Remark*).

G を部分加群の家族 $(G_l)_{l \in L}$ の 3 番目の A-加群、直和とすると、分解 $(F_k)$ に関して、すべての A-線型写像 $v : F \to G$ 行列 $M(v) = (v_{lk})$ に対応するが存在します。 $(G_l)$。 I、K および L が *有限* の場合、

$$
M(v \circ u) = M(v) . M(u)
$$

where the left hand side is the matrix $(w_{li})$ of $w = v \circ u$ with respect to the decomposition $(E_i)$ and $(G_l)$ and the product on the left hand side is calculated for the mappings $(t, s) \mapsto t \circ s$ of $\mathrm{Hom}(F_k, G_l) \times \mathrm{Hom}(E_i, F_k)$ into $\mathrm{Hom}(E_i, G_l)$ (no. 2, *Remark*). これは、§ 1, no. 8の公式(32)を行列の項で表したものにすぎません。

最後に、I と K が有限であると仮定すると、$E^*$ (それぞれ $F^*$) は、加群 $E_i^*$ (それぞれ $F_k^*$) (§ 2, no. 6, 命題 10) の直和と正規的に識別されます。すると、分解 $(F_k^*)$ と $(E_i^*)$ に対する $^t u$ の行列がちょうど $(^t u_{ki})_{(k, i) \in K \times I}$ であることがすぐに検証されます。

ここで、I と K が有限であり、さらに各 E_i (それぞれ F_k) が有限の基底を許容すると仮定します。 E (または F) が基底 (e_r)_{r \in R} (それぞれ (f_s)_{s \in S}) を認め、R (または S) が分割 (R_i)_{i \in I} (それぞれ (S_k)_{k \in K}) を認め、すべての i \in についてI (それぞれ k \in K)、(e_r)_{r \in R_i} は E_i の基底です (それぞれ (f_s)_{s \in S_k} は F_k の基底です)。次に、X = M(u) が基底 (e_r)_{r \in R} および (f_s)_{s \in S} に関して u の行列である場合、基底 (e_r)_{r \in R_i} に関して行列 X_{kt} = M(u_{kt}) となります。そして (f_s)_{s \in S_k} は、S_k の添字 s \notin と R_i の添字 r \notin の列の行を抑制することによって得られる X の部分行列です。したがって、私たちは定義する 1 対 1 対応

$$
X \mapsto (X_{kt})_{(k, t) \in K \times I}
$$

between the set of matrices of type (S, R) with elements in A and the set of matrices of matrices $(X_{kt})_{(k, t) \in K \times I}$ of type K \times I, where each X_{kt} is a matrix over A of type (S_k, R_i). さらに G が有限の基底 (g_t)_{t \in T} を許容し、T = (T_l)_{l \in L} が T の分割であり、各 l \in L に対して (g_t)_{t \in T_l} が G_l の基底であると仮定します。 Y = M(v) を基底 (f_s)_{s \in S} および (g_t)_{t \in T} に関して v の行列とし、Y_{lk} = M(v_{lk}) を基底 (f_s)_{s \in S_k} および (g_t)_{t \in T_l} に関して v_{lk} とします。 Z = M(w) 基底 (e_r)_{r \in R} および (g_t)_{t \in T} に関する w = v \circ u の行列および基底 (e_r)_{r \in R_i} および (g_t)_{t \in に関する w_{li} の Z_{li} = M(w_{li}) T_l};次に、(23) から、Z = YX の部分行列 Z_{li} は次の式で与えられることがわかります。

$$
Z_{li} = \sum_k Y_{lk} X_{kt}
$$

in other words, the one-to-one correspondence (24) transforms products into products when all the products in question are defined (products of matrices of matrices being defined in the sense of no. 2, Remark); when the submatrices Z_{li} of the product YX are calculated thus, this product is said to be carried out "in blocks".

この名前は、I = {1, p} および K = {1, q} のとき、行列 X を表す表が「行列の配列」を形成する「ブロック」に分割されると想定されるという事実に由来しています。

$$
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{q1} & X_{q2} & \ldots & X_{qp}
\end{pmatrix}
$$

これは、p と q が特定の整数であり、これが実行可能なほど十分に小さい場合、X を示す記号と見なされます。

### 6. 半線形マッピングの行列

A、B を 2 つの環とすると、 \sigma : A の A \to B 準同型を B に、E を右 (それぞれ左) A-加群に基底 (e_i)_{i \in I} を、F を右 (それぞれ左) B-加群に基底を加えます。 $(f_k)_{k \in K}$。 $u : E \to F$ を、$\sigma$ と $u(e_i) = \sum_{k \in K} f_k u_{ki}$ (それぞれ $u(e_i) = \sum_{k \in K} u_{ki} f_k$) に対して *半線形* 写像とします。したがって、$u_{ki}$ は B の元です。 定義、行列型 $K \times I$ の $M(u) = (u_{ki})$ は、基底* $(e_i)$ および $(f_k)$ に対して u の *行列とも呼ばれます。 no. 4 の命題 2 と同じ計算により、すべての $x \in E$ について、I と K が *有限* である場合、

(26D)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
(それぞれ

(26G)
$$
{}^t M(u(x)) = \sigma({}^t M(x)) \cdot {}^t M(u)).
$$

C を 3 番目の環、$\tau : B \to C$ 準同型、G を、基底 $(g_l)_{l \in L}$ および $v$ を持つ右 (それぞれ左) C モジュールとし、$\tau$ を基準とした F から G への半線形マッピングとします。 $M(v)$ が $(f_k)$ と $(g_l)$ に対して$v$ の行列であり、$M(v \circ u)$ が $(e_i)$ と $(g_l)$ に対して$v \circ u$ の行列である場合、I の場合、K とL は有限です、

(27D)
$$
M(v \circ u) = M(v) \cdot \tau(M(u))
$$
(それぞれ

(27G)
$$
{}^t M(v \circ u) = \tau({}^t M(u)) \cdot {}^t M(v)).
$$

たとえば (27 D) を表示するには、(26 D) までのすべての $x \in E$ について、
$$
M(v \circ u) \cdot \tau(\sigma(M(x))) = M(v(u(x)))
$$
$$
= M(v) \cdot \tau(M(u(x))) = M(v) \cdot \tau(M(u)) \cdot \tau(\sigma(M(x))),
$$
よって (27 D) 命題 1/no. 3 による。

最後に、$\sigma : A \to B$ が *同型* であると仮定します。次に、${}^t u : F^* \to E^*$ は $\sigma^{-1}$ (§ 2, no. 5) に対する半線形マッピングであることを思い出してください。 I と K が有限のとき、双対基底 $(f_k^*)$ と $(e_i^*)$ に関して行列 ${}^t u$ は次のように与えられます。

(28)
$$
M({}^t u) = \sigma^{-1}({}^t M(u))
$$
というのは、定義までに、例えばEとFが正しい加群と仮定すると、
$$
\langle {}^t u(f_k^*), e_i \rangle^\sigma = \langle f_k^*, u(e_i) \rangle
$$
$\sigma$ が $x \mapsto x^\sigma$ で表される場合。

#### 注意 {#alg-ii-s10-n6-rem-1 .statement tag=05WQ}

A を環および $\sigma$ を A (no. 3) の *反同型* とします。次の 2 つの状況を考えてみましょう。

(GD) E は左A-加群、F 右A-加群、および $u$ は、$a \in A,\ x \in E$ に対して $u(ax) = u(x)\sigma(a)$ となるような E から F への $\mathbf{Z}$ 線形写像です。他の語では、$u$ は、右側の $A^0$ モジュール E から右A-加群 F の $\sigma$ に対して *半線形* 写像です。

(DG) E は、右A-加群、F 左A-加群、および $u$ で、$a \in A,\ x \in E$ に対して $u(xa) = \sigma(a)u(x)$ となるような E から F への $\mathbf{Z}$ 線形写像です。他の語では、$u$ は、左側の $A^0$ モジュール E から左A-加群 F の $\sigma$ に対して *半線形* 写像です。

In the two cases, the matrix $M(u)$ of $u$ relative to bases of E and F has its elements in A; if these bases are finite, then, for all $x \in E$, we have the respective formulae

(17 GD) $$
M(u(x)) = M(u) . \sigma(M(x))
$$
(17 DG) $$
{}^t M(u(x)) = \sigma({}^t M(x)) . {}^t M(u),
$$
*A で計算される 2 つの辺の積。これは、それぞれ (26 D) と (26 G) の直後に続きます。

### 7. 正方行列

#### 定義 4 {#alg-ii-s10-def-4 .statement tag=05WR}

*行列と同じインデックス付け集合を持つ行列は、平方行列と呼ばれます。*

$n$ 行と $n$ 列を持つ平方行列は、位数* $n$ の *行列と呼ばれます。

#### 注意 {#alg-ii-s10-n7-rem-1 .statement tag=05WS}

行のインデックス付け集合と列が *同じ基数* を持っているが * 同一ではない* 行列は、平方行列と見なされてはならないことに注意してください。特に、環を超える 2 つの行列のうち積は *定義されていません*。

明らかに、A 上の正方行列の加法と乗法は、行の集合のインデックスとして有限の集合を持ち、これら行列の集合には列、定義するが *環* となります。 構造式 (7)、(8)、(9) のため (no. 3)。 行列 $(\delta_{ij})$、$\delta_{ij}$ はクロネッカー添字 ($i \in I, j \in I$ の場合) であり、この環の単位元であり、I が $n$ である場合、$I_n$ または $l_n$ で表されます。 元。このように定義された$I = \{1, n\}$、行列の環を単に$\mathbf{M}_n(A)$と表記します。 $\mathbf{M}_n(A)$の可逆元の群は$\mathbf{GL}_n(A)$または$\mathbf{GL}(n, A)$で表されます。

For a square matrix $U = (a_{ij})$ of order $n$ over A to be right (resp. left) invertible, it is necessary and sufficient that, for every system $(b_i)_{1 \leq i \leq n}$ of elements of A, the system of $n$ equations in $n$ unknowns

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq n)
$$

(それぞれ $\sum_{j=1}^n x_j a_{ji} = b_i$)

A に * 1 つの解* $(x_i)$ があります。

I を有限インデックス集合、A 環および E を右 (それぞれ左) A-加群と基底 $(e_i)_{i \in I}$ とします。 E のすべての *自己準同型* $u$ について、* $(e_i)$ と同じ *2 つの基底に関して、$u$ の行列 $M(u)$ は平方行列です。もっと簡単に言うと、基底* $(e_i)$ に対して、$u$ の行列と呼ばれます。

$I = \{1, n\}$ と仮定します。 写像 $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) is an *同型* of 環 $\mathrm{End}_A(E)$ onto $\mathbf{M}_n(A)$ (resp. onto 反対環 of $\mathbf{M}_n(A)$, as follows from formulae (18 D) (resp. 18 G)) (no. 4)。 The invertible elements of the ring $\mathbf{M}_n(\mathbf{A})$ called *invertible matrices*, correspond under the mapping $u \mapsto M(u)$ (resp. $u \mapsto {}^t M(u)$) to the *automorphisms* of E; the group $\mathbf{GL}(n, \mathbf{A})$ is therefore canonically identified with the group $\mathbf{GL}(\mathbf{A}_d^n)$.

If $u$ is 自己同型 of E, its *contragredient* $\check{u}$ is 自己同型 of the left (resp. right) A-加群 $E^*$, such that $\check{u} = ({}^t u)^{-1} = {}^t (u^{-1})$ (§ 2, no. 5, 定義 6); $M(\check{u})$ が双対基底 $(e_i^*)$ に関して $\check{u}$ の行列である場合、 命題 3 (no. 4) により、

$$
M(\check{u}) = ({}^t M(u))^{-1} = {}^t M(u^{-1}).
$$

したがって、すべての可逆行列 $X$ については、${}^t (X^{-1}) = ({}^t X)^{-1}$ になります。この行列は${}^t X^{-1}$でも表され、行列$X$の*対比*と呼ばれます。

$\sigma$ を環 $\mathbf{A}$ の *自己同型* とします。 for every *semi-linear* 写像 $u : E \to E$ relative to $\sigma$, 行列 $M(u)$ of this 写像 with respect to 基底 $(e_i)$ of E is also 平方行列. (27 D) (no. 6) から、$u$ が全単射である場合、次のことがすぐにわかります。

$$
M(u^{-1}) = (\sigma^{-1}(M(u)))^{-1}.
$$

E を部分加群の有限族 $(E_i)_{i \in I}$ の *直和* である A-加群とします。 E のすべての自己準同型 $u$ に対して、$(E_i)$ (no. 5) と同一の E の 2 つの分解に関して、$u$ の行列 $M(u) = (u_{ki})$ は *平方行列です。 線形写像*。 位数では、すべての $i \in I$ に対して $u(E_i) \subset E_i$ が、$k \neq i$ に対して $u_{ki} = 0$ であることが必要十分です。 $I = \{1, n\}$、関係のとき

$$
u(E_i) \subset E_i + E_{i+1} + \cdots + E_n \qquad (1 \leq i \leq n)
$$

$k < i$ の関係 $u_{ki} = 0$ に相当します。

*正方行列中*例。* I。 *斜め行列*。 平方行列

$$
M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times I},
$$

添字が両方とも等しい元は*対角線元*と呼ばれ、家族$(m_{\iota \iota})_{\iota \in I}$は$M$の*対角線*と呼ばれます。対角線元以外の元が零である環上の平方行列$M = (m_{\iota \kappa})$を*対角行列*と呼びます。 For every family $(a_\iota)_{\iota \in I}$ of 元 of 環 $\mathbf{A}$, 対角行列 $(m_{\iota \kappa})$ such that $m_{\iota \iota} = a_\iota$ for all $\iota \in I$ is denoted by $\operatorname{diag}(a_\iota)_{\iota \in I}$ (or $\operatorname{diag}(a_1, a_2, \ldots, a_n)$ when $I = \{1, n\}$）。 位数 $n$ の正方行列の $\mathbf{A}$ 上の集合 $\mathbf{M}_n(\mathbf{A})$ では、単位元行列 $I_n$ は対角行列であり、またすべての倍数この行列をスカラー $a$ で乗算した $a I_n = I_n a$ (対角行列 (*スカラー* と呼ばれる) の対角線元はすべて $a$ に等しい)。

For every family $(d_i)_{1 \leq i \leq n}$ of 元 of $\mathbf{A}$ and every 行列 $X = (x_{ij})$ of 型 $(n, q)$ (resp. $(p, n)$) over $\mathbf{A}$, writing $D = \operatorname{diag}(d_i)$,

$$
\begin{cases}
DX = (d_i x_{ij}) \\
XD = (x_{ij} d_j).
\end{cases}
$$

特に、位数 $n$ の 2 つの対角線行列については、

$$
\text{diag}(a_i) + \text{diag}(b_i) = \text{diag}(a_i + b_i)
$$
(31)
$$
\text{diag}(a_i) \cdot \text{diag}(b_i) = \text{diag}(a_i b_i).
$$

したがって、$\mathbf{M}_n(\mathbf{A})$ の対角行列形部分環は積環 $\mathbf{A}^n$ と同型です。スカラー 行列形部分環は $\mathbf{A}$ と同型です。

II。 *置換行列;単項式行列.* $\pi$ を有限集合 $\mathbf{I}$ の任意の *置換* とし、$(e_i)_{i \in \mathbf{I}}$ を $\mathbf{A}$ 加群 $\mathbf{E} = \mathbf{A}_d^\mathbf{I}$ の標準基底とします。すべての $i \in \mathbf{I}$、$u_\pi(e_i) = e_{\pi(i)}$ (§ 1, no. 11、系 3 から命題 17) に対して、$\mathbf{E}$ のうち自己準同型 $u_\pi$ は 1 つだけ存在します。 基底 $(e_i)$ に関する行列 $M(u_\pi)$ の添字 $i$ のすべての $i \in \mathbf{I}$、列には、添字の行を除くすべての元零が含まれます。 $\pi(i)$ は 1 に等しい。言葉の乱用により、$M(u_\pi)$ は置換* $\pi$ の *行列と呼ばれる。 $\mathbf{I}$、$u_{\sigma \tau} = u_\sigma \circ u_\tau$ の任意の 2 つの置換 $\sigma, \tau$ については明らかであり、同一性置換 $\varepsilon$、$u_\varepsilon$ については同一性です。したがって、写像 $\pi \mapsto M(u_\pi)$ は、置換行列の群上に対称な群 $\mathfrak{S}_\mathbf{I}$ の *同型* です。

各行と置換行列含むの各列には、元 $\neq 0$ が 1 つだけあります。非ゼロ環 $\mathbf{A}$ 上の有限平方行列 $R$ と、この性質は *単項式行列* と呼ばれます。 $r_i$ を添字 $i$ の $R$ の列の一意元 $\neq 0$ とし、$\pi(i)$ をこの元が存在する行の添字とします。明らかに、$\pi$ は、集合 $\mathbf{I}$ および $R = M(u_\pi)D$ の置換であり、$D = \text{diag}(r_i)$ です。

III。 *三角形行列.* 環正方行列位数 $n$ 環 $\mathbf{A}$ の環 $\mathbf{M}_n(\mathbf{A})$ で、$i > j$ に対して $a_{ij} = 0$ となるような行列 $(a_{ij})$ (それぞれ $i < j$) は *上* (それぞれ *下*) *三角形行列* と呼ばれます。また、そのような行列 *下* (それぞれ *上*) *対角線*は零のみであるとも言われます。 $\mathbf{M}_n(\mathbf{A})$、$S \cap T$の上（それぞれ下）三角形行列形部分環$S$（それぞれ$T$）は、明らかに対角線行列の環であることがすぐに証明されます。

$S$ (それぞれ $T$) の行列の集合 $S'$ (それぞれ $T'$) は、その対角線元が *反転可能* であり、 *上* (*下*) *全三角形と呼ばれる行列の乗法 *群* です。 群*、これは § 1, no. 11、*注意* 5 の直後に続きます。 The set $S_1$ (resp. $T_1$) of matrices in $S$ (resp. $T$) whose diagonal elements are all equal to 1 is a *subgroup* of the above group, called the *upper* (resp. *lower*) *strict triangular group*, and every matrix $M \in S'$ (resp. $M \in T'$) whose diagonal is $(d_i)$, may be written as $M = DM_1 = M'_1D$, where $D = \text{diag}(d_i)$ and $M_1$ and $M'_1$ matrices belonging to $S_1$ (resp. $T_1$).

IV。 *対角線と三角形行列の行列.* $(I_k)_{1 \leq k \leq p}$ を有限集合 $\mathbf{I}$ の分割とします。 環 $\mathbf{A}$ 上のすべての平方行列は、集合 $\mathbf{I}$ のインデックス付きで、行列* 対応するの *平方行列の形に同じように書き込むことができます。行のインデックス作成分割 $(\mathbf{I}_k)$ 行のインデックス作成集合および列 (no. 5) のインデックス作成集合

$$
(32)
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{p1} & X_{p2} & \ldots & X_{pp}
\end{pmatrix}
$$

ここで、各 $X_{kk}$ は平方行列で、行の集合と列のインデックスとして $\mathbf{I}_k$ が付けられます。

この記法により、$i \neq j$ (それぞれ $i > j$、それぞれ $i < j$) が零となるようなすべての行列 $X_{ij}$ の場合、(32) は行列の対角線 (それぞれ上三角、それぞれ下三角) 行列と呼ばれます。 The interpretation of endomorphisms $u$ whose matrix is a diagonal, resp. triangular, matrix of matrices has been seen earlier, by considering the corresponding matrix $M(u)$ of linear mappings. The lower triangular (resp. upper triangular, diagonal) matrices of matrices for a given partition $(\mathbf{I}_k)$ of I form subrings of the ring of matrices $\mathbf{A}^{I \times I}$. 特に、分割 $(\mathbf{I}_k)$ に対する行列の対角行列の環は積 $\prod_{k=1}^p \operatorname{End}_\mathbf{A}(E_k)$ と同型です。

### 8. 基底中変更

#### 命題 4 {#alg-ii-s10-prop-4 .statement tag=05WT}

*E を右A-加群とし、n 元の有限基底 $(e_i)_{1 \leq i \leq n}$ とする。 n の族元 $e'_i = \sum_{j=1}^n e_j a_{ji} (1 \leq i \leq n)$ が E の基底であるためには、 位数 n の平方行列 $P = (a_{ji})$ が可逆であることが必要かつ十分です。*

$P$ は、$u(e_i) = e'_i (1 \leq i \leq n)$ によって定義される E の自己準同型 $u$ の基底 $(e_i)$ に関して、ちょうど行列です。さて、$u$ が E の自己同型であるためには、$(u(e_i))$ が E の基底 (§ 1, no. 11、系 3 ～ 命題 17) であることが必要かつ十分です。 よって命題。

反転可能な行列 $P$ は、基底* $(e_i)$ * から基底* $(e'_i)$ への通過の *行列と呼ばれます。また、基底 $(e'_i)$ および $(e_i)$ (*その位数*) に関して恒等写像 $l_E$ の行列と解釈することもできます。そして明らかに、*基底* $(e'_i)$ *から基底* $(e_i)$ の行列は、$P$ の *逆* $P^{-1}$ です。

#### 命題 5 {#alg-ii-s10-prop-5 .statement tag=05WU}

※$(e_i)$から$(e'_i)$への通路のEとP行列のn元の2つの基底を$(e_i), (e'_i)$とします。 $(e_i^*)$ と $({e'_i}^*)$ がそれぞれ $(e_i)$ と $(e'_i)$ の双対基底である場合、$(e_i^*)$ から $({e'_i}^*)$ への通過の行列は P.* の対偶 $^tP^{-1}$ です。

The transpose of the identity mapping $l_E$ is the identity mapping $l_{E^*}$; by Proposition 3, no. 4, the matrix of $l_{E^*}$ with respect to the bases $({e'_i}^*)$ and $(e_i^*)$ (in that order) is the transpose of the matrix of $l_E$ with respect to the bases $(e_i)$ and $(e'_i)$ (in that order), that is the transpose of $P^{-1}$.

#### 命題 6 {#alg-ii-s10-prop-6 .statement tag=05WV}

*EとFを2つの右A-加群、$(e_i)$、$(e'_i)$とし、E*の2つの基底を$n$元、$(f_j)$、$(f'_j)$とし、$F$の2つの基底を$m$とします。 $(e_i)$から$(e'_i)$への通過の元、$P$ 行列、および$(f_j)$から$(f'_j)$への通過の$Q$ 行列。 For every linear mapping $u$ of $E$ into $F$, let $M(u)$ be the matrix of $u$ with respect to the bases $(e_i)$ and $(f_j)$ and $M'(u)$ the matrix of $u$ with respect to the bases $(e'_i)$ and $(f'_j)$; then

$$
M'(u) = Q^{-1} M(u) P.
$$

$u = l_F \circ u \circ l_E$と書く場合もあります。 公式 (33) は、$(e'_i)$ と $(e_i)$ に関して$l_E$ の行列が取られ、$(e_i)$ に関して$u$ が取られると、no. 4、系から命題 2 に続きます。 $(f_i)$と$(f'_j)$に関しては$(f_i)$と$l_F$のそれ。

#### 系 1 {#alg-ii-s10-prop-6-cor-1 .statement tag=05WW}

*$u$ が、それぞれ基底 $(e_i)$ と $(e'_i)$ に関して、$E$ と $M(u)$ の自己準同型であり、$M'(u)$ がその行列である場合、*

$$
M'(u) = P^{-1} M(u) P.
$$

#### 系 2 {#alg-ii-s10-prop-6-cor-2 .statement tag=05WX}

*$M(x)$と$M'(x)$が行列で、それぞれ基底$(e_i)$と$(e'_i)$に関して同じ元$x \in E$の列が1つある場合、*

$$
M(x) = P . M'(x).
$$

これは、$A_d$ から $E$ (no. 4、*注意 1*) の写像 $\theta_x : a \mapsto xa$ に適用される命題 6 の特殊なケースです。

公式 (35) は以下と同等です

$$
x_i = \sum_{j=1}^n a_{ij} x'_j \quad (1 \leq i \leq n)
$$

元 $x_i$ と $x'_i$ の行列 $M(x)$ と $M'(x)$ です。式(36 D)は*座標変更の式*と呼ばれます。 「古い」基底 $(e_i)$ に対する $x$ の成分が、「新しい」基底 $(e'_i)$ および元に対する $x$ の成分の写像として表されることに注目してください。 $P$、つまり、「古い」基底に対する「新しい」基底の成分です。

#### 注意 {#alg-ii-s10-n8-rem-1 .statement tag=05WY}

(1) 次に、*左* $A$ モジュール $E$ から始めます。2 つの基底 $(e_i), (e'_i)$ があり、それぞれが $n$ 元です。 $e'_i = \sum_{j=1}^n a_{ji} e_i$と書くと、$P = (a_{ji})$は、$(e_i)$から$(e'_i)$までの移行*の*行列とも呼ばれます。また、基底 $(e_i)$ に関しては $u(e_i) = e'_i$ となるような $E$ の自己同型の行列であり、基底 $(e'_i)$ および $(e_i)$ に関しては $l_E$ の行列です。 *その位数* で。上記の結果は、以下の修正を加えた場合のみ当てはまります: 式 (33 D) から (36 D) はそれぞれ次のように置き換えられます。

$$
\begin{align*}
(33\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t Q^{-1} \\
(34\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t P^{-1} \\
(35\text{ G}) &\quad {}^t M(u) = {}^t M'(u) . {}^t P.
\end{align*}
$$

リニア代数

(36G)
$$
x_i = \sum_{j=1}^n x_j' a_{ij} \quad (1 \leq i \leq n).
$$

(2) 命題 4 の仮説の下で、元 $x^* \in \mathbf{E}^*$ を検討します。 $(e_i^*)$ から $(e_{i'}^*)$ への通過の行列は $tP^{-1}$ (命題 5) であるため、これら 2 つの基底に関して、それぞれ $x^*$ の行列 $M(x^*)$ と $M'(x^*)$ は、

$$
tM(x^*) = tM'(x^*) . P^{-1}
$$

またはまた

(37D)
$$
tM'(x^*) = tM(x^*) . P
$$

これは方程式の系に相当します

(38D)
$$
x_{i'}^* = \sum_{j=1}^n x_j^* a_{ji} \quad (1 \leq i \leq n)
$$

元 $(x_i^*)$ と $(x_{i'}^*)$ の行列 $M(x^*)$ と $M'(x^*)$ 。 左A-加群 E の対応する式は次のとおりです。

(37G)
$$
M'(x^*) = tP . M(x^*)
$$

(38G)
$$
x_{i'}^* = \sum_{j=1}^n a_{ji} x_j^* \quad (1 \leq i \leq n).
$$

(3) A、B を、A の 2 つの環、$\sigma : A \to B$ 準同型を B、E を右 (それぞれ左) A-加群、$(e_i)$、$(e_i')$ 2 つの基底と E、F の$n$ 元を右 (それぞれ左) とする。 B-加群、$(f_j)$、$(f_j')$ 2 つの基底と、F の $m$ 元および $(e_i)$ から $(e_i')$ への通過の $P$ (それぞれ $Q$) 行列 $(f_j)$から$(f_j')$）。

すべての半線形マッピング $u : E \to F$ について、$\sigma$ を基準として、$M(u)$ を $(e_i)$ および $(f_j)$ および$M'(u)$ に関して$u$ の行列とし、$(e_i')$ および$(f_j')$ に関して行列とします。それから

(39D)
$$
M'(u) = Q^{-1} M(u) \sigma(P)
$$
(それぞれ
(39G)
$$
tM'(u) = \sigma(tP) . tM(u) . tQ^{-1}.
$$

証明は (33 D) と (33 G) の場合と同じですが、今回は式 (27 D) と (27 G) (no. 6) を使用します。

### 9. 行列に相当します。似ています行列

#### 定義 5 {#alg-ii-s10-def-5 .statement tag=05WZ}

*m 行の 2 つの行列* $X, X'$ * と環上の n 列は、位数 m の可逆平方行列* $P$ * と可逆平方行列* が存在する場合、等価と呼ばれます。 $Q$ *位数のうち *

(40)
$$
X' = PXQ.
$$

明らかに関係「X と X' は同等」は、A 上の集合 $A^{mn}$ 行列型 $(m, n)$ で同値関係 (集合理論, II, § 6, no. 1) であり、正当化されます。用語。

これにより、no. 8の定義、命題6は、というにより、基底を2つの右A-加群E、F（有限の基底付き）、線形写像$u : E \to F$の行列に変更すると、というによって述べることができます。 基底は、古い基底に関して、$u$ の行列に相当します。

逆に、関係 (40) が成立し、$u : A_d^n \to A_d^m$ が線形写像であり、その行列が、$A_d^n$ と $A_d^m$ のそれぞれの正規の基底 $(e_i)$ と $(f_j)$ に関して $X$ である場合、$X'$ 基底 $(e'_i)$ と $(f'_j)$ に関して $u$ の行列であるため、$Q$ は $(e_i)$ から $(e'_i)$ への通過の行列と、からの通過の $P^{-1}$ 行列になります。 $(f_j)$から$(f'_j)$まで。

行列に相当する例。 (1) $m$ 行と $n$ 列を持つ 2 つの行列 $X = (x_{ij})$ と $X' = (x'_{ij})$ は、置換 $\sigma$ の区間 $[1, m]$ が存在する場合、「行の位数のみが異なります」。 $\mathbf{N}$、添字 $(i, j)$ のすべての注文された対に対して、$x'_{ij} = x_{\sigma(i), j}$ になります ($X'$ は、$X$ の行で置換 $\sigma^{-1}$ を実行することによって得られるとも言います)。 行列 $X$ と $X'$ は、$X' = PX$ に関して等価になります。ここで、$P$ は、置換 $\sigma^{-1}$ の行列 (cf. no. 7, 例) II）。

同様に、$X$ と $X'$ は、添字 $(i, j)$ のすべての注文された対に対して $x'_{ij} = x_{i, \tau(j)}$ となるような $[1, n]$ の置換 $\tau$ が存在する場合、列の位数のみが異なると言われます。 $X$ と $X'$ も同等です。$X' = XQ$ では、$Q$ は置換 $\tau$ の行列です。

上記の記法 $P$ は、基底 $(f_j)_{1 \leq j \leq m}$ から基底 $(f_{\sigma^{-1}(j)})_{1 \leq j \leq m}$ までの経過の行列と、基底 $(e_i)_{1 \leq i \leq n}$ から基底までの経過の $Q$ 行列であることに注意してください。 $(e_{\tau(i)})_{1 \leq i \leq n}$。

(2) $j, k$ を $[1, n]$ の元と区別し、$a \in A$ とします。

$1 \leq i \leq m$、$x'_{ij} = x_{ij} + x_{ik}a$、$x'_{il} = x_{il}$ が $j \neq l$ と $1 \leq i \leq m$ であるとします。 $X'$は、添字の$X$の$j$列の添字$k$の列に右に$a$を掛けて、$X$から得られると言われています。この場合、$X$ と $X'$ も同等です。つまり、$Q = I_n + aE_{kj}$ (no. 7 に見られる逆三角形行列) の場合、$X' = XQ$ となります。

同様に、$h, i$ を、$[1, m]$ の 2 つの異なる元と $A$ の $a$ 元とします。 添字 $i$ の $X$ の行に添字 $h$ の行の左側に $a$ を掛けて$X'$ が $X$ から導出される場合、$X$ と $X'$ は等価です。 $X' = PX$、ここで$P = I_m + aE_{ih}$。

(3) 最後に、与えられた添字 $j$ に対して、$1 \leq i \leq m$ に対して $x'_{ij} = x_{ij}c$ がある場合、$c$ は可逆であり、$1 \leq i \leq m$ と $l \neq j$ に対して $x'_{il} = x_{il}$、$X$ と $X'$ は等価です。 $X' = XQ$の場合、$Q$は行列 $\operatorname{diag}(a_k)$、$a_j = c$、$k \neq j$の場合は$a_k = 1$です。そして、$X'$は、右側の添字$j$の$X$の列に$a$を掛けて、$X$から導かれると言われています。

Similarly, if $X'$ is derived from $X'$ by multiplying the row of $X$ of index $i$ on the left by an invertible element $c \in A$, $X'$ and $X$ are equivalent, for $X' = PX$ where $P$ is the matrix $\operatorname{diag}(b_h)$ with $b_i = c$, $b_h = 1$ for $h \neq i$.

#### 定義 6 {#alg-ii-s10-def-6 .statement tag=05X0}

*次のような位数 n の可逆な平方行列 P が存在する場合、環 A 上の位数 n の 2 つの正方行列 X、X' は類似と呼ばれます*

$$(41)$$
$$X' = PXP^{-1}$$

明らかに、関係「XとX'は似ている」は$M_n(A)$の*同値関係*で、XとX'がこの環の*内部自己同型*によって1つの他のに変換されることを意味します。

これにより、定義, 系 1 から no. 8 の命題 6 は、A-加群 E (有限の基底) の基底を変更すると、新しいものに関して自己準同型 u の行列が変更されるとというで表すことができます。 基底は、古い基底に関して、あなたの行列と*似ています*。

#### 注意 {#alg-ii-s10-n9-rem-1 .statement tag=05X1}

(1) 行の位数 (または列の位数) のみが異なる 2 つの正方行列は同等ですが、一般に *似ていません*。 平方行列 $X = (x_{ij})$ と同様の行列は、行で *同じ置換* $\sigma^{-1}$ を実行し、列を実行することによって取得できます。つまり、行列 $X' = (x'_{ij})$ を考慮することで、順序付けされたすべての$x'_{ij} = x_{\sigma(i), \sigma(j)}$ が計算されます。 添字中対;なぜなら、X が基底 $(e_i)_{1 \leq i \leq n}$ に関して、$A^n_d$ の自己準同型の行列である場合、$X'$ は、基底 $(e_{\sigma(i)})_{1 \leq i \leq n}$ に関して、u の行列です。

(2) X と $X'$ を、正方行列 (no. 7, 例 IV) の対角行列の形に書ける位数 n の 2 つの正方行列とします。

$$
X = \begin{pmatrix}
X_1 & 0 & \ldots & 0 \\
0 & X_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X_p
\end{pmatrix}
\qquad
X' = \begin{pmatrix}
X'_1 & 0 & \ldots & 0 \\
0 & X'_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X'_p
\end{pmatrix}
$$

対応するは、X と $X'$ のインデックス付け集合 $[1, n]$ の *同じ* 分割です。 $1 \leq i \leq p$、$X_i$、$X'_i$ が同等（それぞれ類似）である場合、X と $X'$ は同等（それぞれ類似）です。 $1 \leq i \leq p$ に対して $X'_i = P_i X_i Q_i$ の場合、$X' = PXQ$ ここで

$$
P = \begin{pmatrix}
P_1 & 0 & \ldots & 0 \\
0 & P_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & P_p
\end{pmatrix}
\qquad
Q = \begin{pmatrix}
Q_1 & 0 & \ldots & 0 \\
0 & Q_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Q_p
\end{pmatrix}
$$

「ブロック」積(no. 6)を計算すると以下のようになります。さらに、すべての i が $Q_i = P_i^{-1}$ であれば、$Q = P^{-1}$ になります。

### 10. 可換環を超える行列のうちテンソル積

C を可換環、E、F、U、V 4 つの C モジュールと $\phi : E \to U$、$\psi : F \to V$ 2 つの C 線形マッピングとします。 E、F、U、V がそれぞれ有限の基底 $(e_\lambda)_{\lambda \in L}, (f_\mu)_{\mu \in M}, (u_\rho)_{\rho \in R}, (v_\sigma)_{\sigma \in S}$ を持つと仮定します。 $A = (a_{\rho \lambda})$を、$(e_\lambda)$と$(u_\rho)$に関しては$\phi$の行列とし、$B = (b_{\sigma \mu})$は、$(f_\mu)$と$(v_\sigma)$に関しては$\psi$の行列とします。注文されたすべての対 $(\lambda, \mu) \in L \times M = N$ に対して、$g_{\lambda \mu} = e_\lambda \otimes f_\mu$ とします。注文されたすべての対 $(\rho, \sigma) \in R \times S = T$ に対して $w_{\rho \sigma} = u_\rho \otimes v_\sigma$ とします。 $g_{\lambda \mu}$、$E \otimes F$の形基底、および$U \otimes V$の$w_{\rho \sigma}$ 基底 (§ 3, no. 6、系 2 ～ 命題 7)。 $A \otimes B$ で示される、$A$ の $B$ の *テンソル積* は、行列 $X = (x_{\tau v})_{(\tau, v) \in T \times N}$ であり、その元は次のように与えられます。

$$
x_{(\rho, \sigma), (\lambda, \mu)} = a_{\rho \lambda} b_{\sigma \mu}.
$$

すると、$A \otimes B$ は、基底* $(g_{\lambda \mu})$ * および* $(w_{\rho \sigma})$ に関して、* $\phi \otimes \psi$ の *行列になります。 定義 (§ 3, no. 2、公式 (3)) によって

$$
\begin{align*}
(\phi \otimes \psi)(g_{\lambda \mu}) &= (\phi \otimes \psi)(e_\lambda \otimes f_\mu) = \phi(e_\lambda) \otimes \psi(f_\mu) \\
&= \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} (u_\rho \otimes v_\sigma) = \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} w_{\rho \sigma}.
\end{align*}
$$

$A \otimes B$の元の定義(42)は、この行列対応するが行列$(a_{\rho \lambda} B)_{(\rho, \lambda) \in R \times L}$の行列、また行列$(A b_{\sigma \mu})_{(\sigma, \mu) \in S \times M}$(no. 5)と全射的に一致することを示しています。

$(\phi, \psi) \mapsto \phi \otimes \psi$ が C 双線形写像であり、§ 3, no. 5 の公式 (9) であるという事実は、恒等式で表現できます。

$$
\begin{align*}
(A \otimes (B_1 + B_2)) &= A \otimes B_1 + A \otimes B_2 \\
((A_1 + A_2) \otimes B) &= A_1 \otimes B + A_2 \otimes B
\end{align*}
$$
(43)

$$(cA) \otimes B = A \otimes (cB) = c(A \otimes B) \quad \text{for } c \in \mathbf{C}$$
(44)

$$(A_1 \otimes B_1)(A_2 \otimes B_2) = (A_1 A_2) \otimes (B_1 B_2)$$
(45)

演算がいつ現れるかを定義します。 行列のテンソル積の転置は次のように与えられます。

$$(A \otimes B)^t = (A^t) \otimes (B^t).$$
(46)

If $A$ and $B$ are invertible square matrices over $\mathbf{C}$, $A \otimes B$ is invertible and

$$(A \otimes B)^{-1} = (A^{-1}) \otimes (B^{-1}).$$
(47)

$(e'_\lambda)_{\lambda \in L}$ を $E$ の他の基底および $F$ の $(f'_\mu)_{\mu \in M}$ 他の基底とします。 $P$ が基底 $(e_\lambda)$ から基底 $(e'_\lambda)$ への経過の行列と基底 $(f_\mu)$ から基底 $(f'_\mu)$ への経過の $Q$ 行列である場合、 基底 $(e_\lambda \otimes f_\mu)$ から基底 $(e'_\lambda \otimes f'_\mu)$ への通過の行列は $P \otimes Q$ です。 $A'$ が $A$ と *同等* (それぞれ *類似*)、$B'$ が $B$ と *同等* (それぞれ *類似*) である場合、$A' \otimes B'$ は $A \otimes B$ と *同等* (それぞれ *類似*) です。

行列のテンソル積の定義は、$\mathbf{C}$ 上の行列の任意の有限数に明白な方法で一般化できます。特に結合性公式があります

$$
\left( \bigotimes_{i \in I_1} X_i \right) \otimes \left( \bigotimes_{i \in I_2} X_i \right) = \bigotimes_{i \in I} X_i
$$

有限インデックス集合 $I$ のすべての *分割* $(I_1, I_2)$ に対して。

### 11. 行列の痕跡

$C$ を *可換* 環とします。 $C$ 対応するにわたるすべての平方行列 $X = (x_{ij})$ から有限インデックス集合 $I$ まで、$X$ の *トレース* は元です

$$
\operatorname{Tr}(X) = \sum_{i \in I} x_{ii}.
$$

$E$ を、有限基底 $(e_i)_{i \in I}$ を許容する $C$ 加群とする。 $E$ の自己準同型 $u$ ごとに、

$$
\operatorname{Tr}(u) = \operatorname{Tr}(M(u))
$$

$M(u)$ は、基底 $(e_i)$ に対して行列 $u$ です。これは、§ 4, no. 3, 公式 (17) の直後に続き、この公式が自己準同型 $x \mapsto \langle x, e_i^*\rangle e_j$ ($e_i^*$) は $(e_i)$ の双対基底に適用されます。ここから、線形性により一般的なケースに移ります。 公式 (49) は次のことを示しています

$$
\operatorname{Tr}(u) = \sum_i \langle u(e_i), e_i^* \rangle
$$

$E$ のすべての基底 $(e_i)$ (cf. § 4, no. 3, 公式 (17))。

$X$ が型の行列 $(m, n)$ $C$ および $Y$ 行列の型 $(n, m)$ $C$ である場合、

$$
\operatorname{Tr}(XY) = \operatorname{Tr}(YX)
$$

上記と命題 3 of § 4, no. 3 から次のようになります。 (52) は、$X = (x_{ij}), Y = (y_{ji})$ ($1 \leq i \leq m, 1 \leq j \leq n$) の場合、直接取得することもできます。

$$
\operatorname{Tr}(XY) = \sum_{i,j} x_{ij} y_{ji}
$$

(49) による。後者公式はさらに次のことを証明します。

#### 命題 7 {#alg-ii-s10-prop-7 .statement tag=05X2}

*Let $C$ be a commutative ring and for every matrix $P \in \mathbf{M}_n(C)$ let $f_P$ be the linear form $X \mapsto \operatorname{Tr}(PX)$ on $\mathbf{M}_n(C)$; the mapping $P \mapsto f_P$ is a $C$-linear bijection of $\mathbf{M}_n(C)$ onto its dual.*

#### 命題 8 {#alg-ii-s10-prop-8 .statement tag=05X3}

*$g$ が $C$ モジュール $\mathbf{M}_n(C)$ で線型形式で、$\mathbf{M}_n(C)$ のすべての行列 $X, Y$ に対して $g(XY) = g(YX)$ である場合、行列ごとに $g(X) = c \cdot \operatorname{Tr}(X)$ となるスカラー $c \in C$ が 1 つだけ存在します。 $X \in \mathbf{M}_n(C)$.*

$n = 1$ にとって命題は自明であるため、注意は $n \geqslant 2$ の場合に限定される場合があります。 $X = E_{ij},\ Y = E_{jk}$ と $i \neq k$ を組み合わせると、$g(E_{ik}) = 0$ が得られます。次に、$X = E_{ij},\ Y = E_{ji}$ と $i \neq j$ を組み合わせると、$g(E_{ii}) = g(E_{jj})$ が見つかります。 $\mathbf{M}_n(\mathbf{C})$ の $E_{ij}$ 形基底の直後に命題が続きます。

### 12. 行列体

$m$ 行と体 $K$ 上の $n$ 列を持つ有限行列は、右ベクトル空間 $E = K_d^n$ の線形写像と右ベクトル空間で 1 対 1 の対応になります。 $E$ と $F$ の正規の基底に関して、これらの写像のうち行列が取られたときの $K_d^m$。 定義までに、そのような行列 $X$ の *階数* は、線形写像 $u : E \to F$ 対応するの階数になります。この数は、部分空間の$u(E)$の$F$の定義次元によるものであるため、同じになります（$X$の列と、標準基底の$u$の下の像を識別します） $E$) 次の定義を与えます:

#### 定義 7 {#alg-ii-s10-def-7 .statement tag=05X4}

*Given a matrix $X$ with $m$ rows and $n$ columns over a field $K$, the dimension of the subspace of $K_d^m$ generated by the $n$ columns of $X$ is called the rank of $X$ with respect to $K$ and denoted by $\operatorname{rg}(X)$.*

また、$X$ の階数は、$X$* の線形独立列の * 最大値数であるとも言えます ($K_d^m$ の元として)。 明らかに $\operatorname{rg}(X) \leqslant \inf(m, n)$; $X$、$\operatorname{rg}(Y) \leqslant \operatorname{rg}(X)$ のすべての部分行列 $Y$ に対して。

$E$と$F$が、$K$と$u$の2つの有限次元ベクトル空間、$E$の線形写像を$F$にすると、任意の2つの基底に関して、行列$M(u)$の階数は次と等しい。 $u$中階数。

#### 命題 9 {#alg-ii-s10-prop-9 .statement tag=05X5}

*If the elements of a matrix $X$ with $m$ rows and $n$ columns belong to a subfield $K_0$ of a field $K$, the rank of $X$ with respect to $K_0$ is equal to the rank of $X$ with respect to $K$.*

$F_0$ を、右側ベクトル $K$-スペース $E = K_d^m$ の標準基底によって生成された右側ベクトル $K_0$ スペースとします。 仮定列のうち $X$ 属するから $E_0$ まで。 Let $V_0$ (resp. $V$) be the vector sub-$K_0$-space of $F_0$ (resp. the vector sub-$K$-space of $E$) generated by these columns. 次に、$V = V_0 \otimes_{K_0} K$ (§ 8, no. 2、命題 2)、したがって $\dim_K V = \dim_{K_0} V_0$ となります。

#### 命題 10 {#alg-ii-s10-prop-10 .statement tag=05X6}

* 体 $K$ の行列 $X$ の階数は、反対側の体 $K^0$ の転置 ${}^t X$ の階数に等しい。*

記法で前に定義 7 が導入され、$u$ の階数は ${}^t u$ (§ 7, no. 5、命題 10) の命題に等しいため、no. 4、命題 3 から続きます。

したがって、$X$ の階数は、$X$* の線形独立行の * 最大数としても定義できることがわかります (左のベクトル $K$ 空間 $K_s^n$ の元とみなします)。

The square matrices of order $n$ over a field $K$ correspond bijectively with the endomorphisms of $E = K_d^n$ and form a ring isomorphic to the ring

終了$_{\mathbf{K}}$ (E) (no. 7); Eの対応するから自己同型は反転可能な正方行列です。

#### 命題 11 {#alg-ii-s10-prop-11 .statement tag=05X7}

*X を体 K 以上の位数 n の平方行列とします。以下のプロパティは同等です:*

(a) *Xは$\mathbf{M}_n(\mathbf{K})$で反転可能です。*
(b) *Xは$\mathbf{M}_n(\mathbf{K})$において右反転可能です。*
(c) *Xは$\mathbf{M}_n(\mathbf{K})$では反転可能なままです。*
(d) *X は階数 n のものです。*

これは、§ 7, no. 4、系から命題 9 を翻訳しただけです。

#### 命題 12 {#alg-ii-s10-prop-12 .statement tag=05X8}

*n 個の未知数における m 個の線形方程式の系について*

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq m)
$$

*体 K にわたって少なくとも 1 つの解が必要な場合、$(b_i)$ に等しい$(n+1)$ 番目の列で A を境界とする系と行列 B の行列 $A = (a_{ij})$ が同じ行列であることが必要かつ十分です。 階数.*

(54) の解の存在は、列 $(b_i)$ が $A$ の列の線形結合であるという事実と同等であることがわかりました (no. 4)。したがって、命題は § 7, no. 3, 系 4 から命題 4.

$m = n$ と $A$ が反転可能な場合、つまり階数 $n$ (命題 11) の場合、命題 12 の条件は常に満たされることに注意してください。 $x$ と $b$ がそれぞれ 1 つの列 $(x_i)$ と $(b_i)$ で行列を表す場合、系 (54) は $A.x = b$ と等しく、その固有の解は $x = A^{-1}.b$ です。

### 13. 同値/行列以上体

#### 命題 13 {#alg-ii-s10-prop-13 .statement tag=05X9}

*E, F を体 K 上の 2 つの有限次元ベクトル空間とします。$u : E \to F$ が階数 r の線形写像であるとすると、これら基底に関して、次のような E と F の基底が存在します。

$$
M(u) = \begin{pmatrix} I_r & 0 \\ 0 & 0 \end{pmatrix}.
$$

K 上の型 $(m, n)$ および階数 r のすべての行列は、形 (55) の行列と同等です。*

2 番目の主張は最初のものと自明に等価です。後者を示すには、$\dim E = n$、$\dim F = m$ とします。 核 $N = u^{-1}(0)$ は次元 $n - r$ (§ 7, no. 4, 公式 (11)) です。 V を E の N の補足部分空間と E の $(e_i)_{1 \leq i \leq n}$ 基底とし、$(e_i)_{1 \leq i \leq r}$ が V の基底および N の $(e_i)_{r+1 \leq i \leq n}$ 基底となるようにします。すると、$u(e_j)$ $(1 \leq j \leq r)$ 形基底/$u(E)$;したがって、$1 \leq j \leq r$ (§ 7, no. 1, 定理 2) に対して $f_j = u(e_j)$ となるような F の基底 $(f_j)_{1 \leq j \leq m}$ が存在し、基底 $(e_i)$ および $(f_j)$ 行列に関しては明らかです$M(u)$ は (55) によって与えられます。

#### 系 {#alg-ii-s10-n13-cor-1 .statement tag=05XA}

*型 $(m, n)$ のうち、体上の 2 つの行列が同等であるためには、それらが同じ階数を持っていることが必要かつ十分です。

ここで、命題 13 を他のより明確な方法によって復元します。すべての環 $A$、すべての $\lambda \in A$、すべての整数 $m > 1$、および $[1, m]$ の *個別* 整数 $i, j$ のすべての注文された対について、次のように書きます。

$$
B_{ij}(\lambda) = I_m + \lambda E_{ij}
$$

no. 8 による位数 $m$ の反転行列。

#### 補題 1 {#alg-ii-s10-lem-1 .statement tag=05XB}

*$X = (\xi_{ij})$を環$A$に対する型$(m, n)$の行列とします。 $m \geqslant 2$ があり、$X$ の最初の列には$A$ で反転可能な元 $\xi_{i1}$ が存在するとします。このとき、$A$ 上に型 $(m - 1, n - 1)$ の 2 つの可逆正方行列 $P \in \mathbf{M}_m(A)$、$Q \in \mathbf{M}_n(A)$、行列 $Y$ が存在し、$P$ (それぞれ $Q$) は次のようになります。 積の行列の形 $B_{ij}(\lambda)$ の位数 $m$ (それぞれ $n$) および*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 \\
0 & & & \\
\vdots & & Y & \\
0 & & &
\end{pmatrix}.
$$

行列 $B_{ij}(\lambda)X$ は、添字 $i$ の $X$ の行に添字 $j$ の行を加算し、左側に $\lambda$ (no. 9, *例 2*) を乗算して得られます。 $\xi_{i1}$ が可逆であれば、行列 $X' = B_{1i}(\lambda)X = (\xi'_{kl})$, $\xi'_{11} = 1$ のような $\lambda \in A$ が存在します。左側の $X'$ に、位数 $m$ ($1 \leq k \leq m$ の場合) の適切に選択された行列 $B_{k1}(\mu_k)$ を乗算すると、$\xi''_{j1} = 1$、$\xi''_{k1} = 0$ となるように行列 $X'' = (\xi''_{kl})$ が得られます。 $k \neq 1$。次に、得られた行列に、*右側* の位数 $n$ $(2 \leq j \leq n)$ の適切な行列 $B_{1j}(v_j)$ を連続的に乗算し、形の行列が得られます (57)。

#### 命題 14 {#alg-ii-s10-prop-14 .statement tag=05XC}

*$X$ を体 $K$ に対する型 $(m, n)$ の行列とします。 $X$ が階数 $r$ である場合、$P$ (それぞれ $Q$) が位数の行列の積となるような 2 つの反転可能な正方行列 $P \in \mathbf{M}_m(K)$、$Q \in M_n(K)$ が存在します。 形 $B_{ij}(\lambda)$ および* の $m$ (それぞれ $n$)

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \delta_r & 0 & \cdots & 0 \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0
\end{pmatrix}
$$

(行列 $(\eta_{ij})$ の項はすべて零ですが、$1 \leq i \leq r$ の $\eta_{li}$ と $1 \leq i \leq r - 1$、$\eta_{rr} = \delta_r \neq 0$ の $\eta_{li} = 1$ が含まれます)。 ※$r \neq m$または$r \neq n$の場合は、$\delta_r = 1$とみなされる場合もあります。

$X = 0$ の場合、命題は明らかです。したがって $X \neq 0$ と仮定します。 $m = n = 1$ 命題が明らかな場合 ($P = I_m$、$Q = I_n$、$\delta_1 \neq 0$ は任意)。 $n = 1$、$m \geq 2$ の場合、補題 1 ($X \neq 0$ 以降) を適用でき、$r = 1$、$\delta_r = 1$ で希望の形 (58) が得られます。私たちは$n > 1$の帰納法までに議論します。 $X$ には元 $\xi_{ij} \neq 0$ が存在します。 $j = 1$ の場合、補題 1 が適用でき、$X$ が形である場合には簡約する問題が適用できます (57)。 帰納法の仮定は $Y$ に適用され、したがって反転可能な行列が存在します。

$$
P' \in \mathbf{M}_{m-1}(\mathbf{K}), \quad Q' \in \mathbf{M}_{n-1}(\mathbf{K})
$$

これは、形の行列の積、位数$m - 1$の$B_{ij}(\lambda)$（それぞれ$n - 1$）であり、$P'YQ'$は形のものになります（58）。ただし、たとえば $B_{ij}(\lambda)$ 属するから $\mathbf{M}_{m-1}(\mathbf{K})$ の場合、

$$
\begin{pmatrix}
1 & 0 \\
0 & B_{ij}(\lambda)
\end{pmatrix} = B_{i+1,\ j+1}(\lambda);
$$

公式 (58) は、公式からブロック積の書き込みに続きます。

$$
P = \begin{pmatrix} 1 & 0 \\ 0 & P' \end{pmatrix} \text{ and } Q = \begin{pmatrix} 1 & 0 \\ 0 & Q' \end{pmatrix}.
$$

最終的に$j \neq 1$であれば、上記の場合に行列$XB_{j1}(1)$～簡約するを考慮すれば十分です。

命題 14 はすぐに命題 13 を回復します。

#### 系 1 {#alg-ii-s10-prop-14-cor-1 .statement tag=05XD}

*If $X$ is an invertible square matrix of order $n$ over a field $\mathbf{K}$, there exist three invertible matrices $P, Q, D$ of order $n$ such that $X = PDQ$, $P$ and $Q$ being products of matrices of the form $B_{ij}(\lambda)$ and $D$ a diagonal matrix of the form*

$$
D = \operatorname{diag}(1, 1, \ldots, \delta),
$$

*ここで、$\delta \neq 0$ (cf. 練習問題 13)。*

#### 系 2 {#alg-ii-s10-prop-14-cor-2 .statement tag=05XE}

*反転可能な行列 $\mathbf{GL}(n, \mathbf{K})$ の各体 $\mathbf{K}$、群は、置換行列 (no. 7、例 2)、対角行列 $\operatorname{diag}(a, 1, \ldots, 1)$ によって生成されます。 ($a \neq 0$ の $\mathbf{K}$) および行列 $B_{12}(\lambda)$ ($\lambda \in \mathbf{K}$)。*

適切な転置の行列による行列の右側 (それぞれ左側) 積が、任意の 2 つの列 (それぞれの行) を交換することがわかりました (no. 9)。すると、行列 $\operatorname{diag}(1, \ldots, 1, a)$ は $\operatorname{diag}(a, 1, \ldots, 1)$ および置換行列の積に等しく、すべての行列 $B_{ij}(\lambda)$ は $B_{12}(\lambda)$ および置換行列の積に等しくなります。 よって系。

#### 注意 {#alg-ii-s10-n13-rem-1 .statement tag=05XF}

(1) 章 III では、$m = n = r$ と $K$ が *可換* である場合、$P$ と $Q$ 満たす条件命題 14 のすべての選択について、 元 $\delta_r$ は常に同じで、$X$ (III, § 8, no. 6) の *行列式* と等しくなります。

(2) 命題 14 の引数を少し変更すると、次のような置換行列 $R$ が存在することがわかります ($P$ にも同じ条件が付きます)

$$
PX R = \begin{pmatrix} I_r & N \\ 0 & 0 \end{pmatrix}
$$

$m = n = r$ が成立しない場合、および

$$
PX R = \operatorname{diag}(1, \ldots, 1, \delta)
$$

さもないと。また、$X$ が明示的に与えられた場合、証明の方法は行列 $P, Q, R$ の明示的な決定を与えることにも注目してください。

### 練習問題 {#alg-ii-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
