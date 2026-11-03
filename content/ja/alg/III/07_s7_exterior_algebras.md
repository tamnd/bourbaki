---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 7
section_title: Exterior algebras
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 507-522, 633-637
pdf_pages: 0531-0546, 0657-0661
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE EXTERIOR ALGEBRA OF A MODULE
      page: 507
      pdf_page: 531
    - "no": 2
      title: Functorial properties of the exterior algebra
      page: 508
      pdf_page: 532
    - "no": 3
      title: ANTICOMMUTATIVITY OF THE EXTERIOR ALGEBRA
      page: 510
      pdf_page: 534
    - "no": 4
      title: '*n*-th EXTERIOR POWER OF A MODULE AND ALTERNATING MULTILINEAR MAPPINGS'
      page: 511
      pdf_page: 535
    - "no": 5
      title: EXTENSION OF THE RING OF SCALARS
      page: 513
      pdf_page: 537
    - "no": 6
      title: DIRECT LIMITS OF EXTERIOR ALGEBRAS
      page: 514
      pdf_page: 538
    - "no": 7
      title: EXTERIOR ALGEBRA OF A DIRECT SUM. EXTERIOR ALGEBRA OF A GRADED MODULE
      page: 515
      pdf_page: 539
    - "no": 8
      title: EXTERIOR ALGEBRA OF A FREE MODULE
      page: 517
      pdf_page: 541
    - "no": 9
      title: CRITERIA FOR LINEAR INDEPENDENCE
      page: 519
      pdf_page: 543
statements: 31
exercises: 15
content_sha256: 1e1136595cd189bc7a1305a82fdac07e9347df06a80264f27844989d83910a08
translated_from: content/en/alg/III/07_s7_exterior_algebras.md
translation_method: google
source_content_sha256: 2ecded72dc27d27759b8e68470e35ec8930215e63753cc4598f26151e19c86fa
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 9869d27784b670e1053cda27a6c53122190989def994cd5bc5c27edfbe25de28
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。外観代数

### 1. 外観の定義代数の加群

#### 定義 1 {#alg-iii-s7-def-1 .statement tag=062S}

$A$ を可換環 、$M$ を $A$ モジュールとします。 $\bigwedge(M)$ または $\mathrm{Alt}(M)$ または $\bigwedge_A(M)$ で示される $M$ の外部代数は、両側イデアルによりテンソル代数 $T(M)$ の $A$ 商よりも代数です。 $\mathfrak{J}''$ ($\mathfrak{J}_{M}''$ とも表される) は、元 $x \otimes x$ によって生成され、$x$ から $M$ まで続きます。

イデアル $\mathfrak{J}''$ は次数 2 の同次元によって生成されるため、段階的イデアル (II, § 11, no. 3、命題 2) です。 $\mathfrak{J}_n'' = \mathfrak{J}'' \cap T^n(M)$と書きます。したがって、代数 $\bigwedge(M)$ は、$\bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$ の卒業 (正規と呼ばれます) からなるによって等級付けされます。次に、$\mathfrak{J}_0'' = \mathfrak{J}_1'' = \{0\}$、したがって $\bigwedge^0(M)$ は $A$ と同一視され、$\bigwedge^1(M)$ は $T^1(M) = M$ と同一視されます。以下では常にこれらの識別を行い、標準単射 $M \to \bigwedge(M)$ は $\phi''$ または $\phi_M''$ で表されます。

#### 命題 1 {#alg-iii-s7-prop-1 .statement tag=062T}

$E$ を次のような $A$-代数、$f : M \to E$ を $A$ 線形写像とします。
$$
(f(x))^2 = 0 \quad \text{for all } x \in M.
$$
$f = g \circ \phi''$ となるような $A$-代数準同型性 $g : \bigwedge(M) \to E$ が 1 つだけ存在します。

他の語では、$(\bigwedge(M), \phi'')$ は普遍写像問題 (集合理論, IV, § 3, no. 1) の解であり、$\Sigma$ は $A$-代数の種です。 構造、$\alpha$-マッピングは、$A$-モジュール $M$ から $A$-代数満たす (1) への線形写像です。

$g$ の一意性は、$\phi''(M) = M$ 生成する $\bigwedge(M)$ という事実から導き出されます。 $g$ の存在を証明するために、§ 5, no. 1, 命題 1 により、$f = g_1 \circ \phi$ となるような $A$-代数準同型性 $g_1 : T(M) \to E$ が存在することに注意します。 $g_1$ が理想 $\mathfrak{J}''$ 上では零であることを証明する必要があります。
$$
p : T(M) \to \bigwedge(M) = T(M)/\mathfrak{J}''
$$
が標準準同型である場合、$g_1 = g \circ p$ と書くことができます。$g : \bigwedge(M) \to E$ は代数準同型であり、結論は $p \circ \phi = \phi''$ という事実から得られます。さて、$g_1$の核は、(1)と関係$g_1 \circ \phi = f$のおかげで、$x \in M$に対して含む元$x \otimes x$となる両面理想です。これで証明は完了です。

#### 注意 {#alg-iii-s7-n1-rem-1 .statement tag=062U}

(1) E が、卒業 $(E_n)$ の型 $\mathbf{Z}$ の評価 A-代数であると仮定し、また、線形写像 $f$ (満たす (1) と仮定) が次のようであると仮定します。
$$
f(M) \subset E_1.
$$
次に、関係 $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ と $x_i \in M$ は、すべての $p \geq 0$ に対して $g(\bigwedge^p(M)) \subset E_p$ であることを示し、したがって $g$ はグレード代数準同型です。

(2) 混乱を避けるため、外面代数 $\bigwedge(M)$ の 2 つの元 $u, v$ のうちの積を通常 $u \wedge v$ で表し、$u$ の *外面積* を $v$ と呼びます。したがって、$\bigwedge^n(M)$ の元は、形 $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ の元の和と、$1 \leq i \leq n$ の $x_i \in M$ であり、*n ベクトル* と呼ばれることがよくあります。

### 2. 外装の機能特性代数

#### 命題 2 {#alg-iii-s7-prop-2 .statement tag=062V}

*$A$ を可換環、$M$、$N$ の 2 つの $A$ モジュールと $u : M \to N$ の $A$ 線形マッピングとします。 $A$-代数準同型性は 1 つだけ存在します*
$$
u'' : \bigwedge(M) \to \bigwedge(N)
$$
*そのような図式*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M'' & & \downarrow \phi_N'' \\
\bigwedge(M) & \xrightarrow{u''} & \bigwedge(N)
\end{array}
$$

*は可換です。さらに、$u''$ はグレード代数準同型です。*

$u'$ の存在と一意性は、代数 $\bigwedge(N)$ と $f = \phi_N'' \circ u : M \to \bigwedge(N)$ に適用される no. 1、命題 1 から続きます。 $f(M) \subset N$ の場合、したがって $f$ は、$\mathfrak{g}_N''$ の定義によって条件 (1) を満たします。 $f(M) \subset \bigwedge^1(N) = N$ と同様、$u''$ が等級付けされた代数準同型であるという事実は、no. 1 の *注意* 1 から導き出されます。

命題 2 の準同型 $u''$ は、以降、$\bigwedge(u)$ で表されます。 $P$ が $A$ モジュールで、$v : N \to P$ が $A$ 線形マッピングの場合、
$$
\bigwedge(v \circ u) = \bigwedge(v) \circ \bigwedge(u)
$$
$\bigwedge(v) \circ \bigwedge(u)$ は代数準同型で、図式が可換になります

$$
\begin{array}{ccc}
M & \xrightarrow{v \quad u} & P \\
\downarrow \phi_M' & & \downarrow \phi_P' \\
\bigwedge(M) & \xrightarrow{\bigwedge(v) \circ \bigwedge(u)} & \bigwedge(P)
\end{array}
$$

$\Lambda(M)$ 含む $M = \Lambda^1(M)$ であるため、$\Lambda(u)$ はときどきであり、$u$ から $\Lambda(M)$ の正規の拡大と呼ばれます。 制限 $\Lambda^n(u): \Lambda^n(M) \to \Lambda^n(N)$ は次のとおりです
$$
\Lambda^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
$x_i \in M$ では、$\Lambda(u)$ は代数準同型と $\Lambda^1(u) = u$ であるため、 制限 $\Lambda^0(u)$ から $A$ は恒等写像です。 $\Lambda^n(u)$ は、$T^n(u): T^n(M) \to T^n(N)$ から移行から商によって得られることに注意してください。

#### 命題 3 {#alg-iii-s7-prop-3 .statement tag=062W}

*$u: M \to N$ が全射 $A$ 線形写像である場合、準同型 $\Lambda(u): \Lambda(M) \to \Lambda(N)$ は全射であり、その核は $u$ の核 $P \subset M \subset \Lambda(M)$ によって生成される $\Lambda(M)$ の両側イデアルです。

証明は、§ 6, no. 2、命題4、置き換えること$S$は$\Lambda$、$\mathfrak{g}'$は$\mathfrak{g}''$から導出されます。

$u: M \to N$ が単射詞線形写像である場合、$\Lambda(u)$ が単射詞写像 (§ 6、練習問題 3) であるとは限りません (ただし、以下の no. 9、系 ～ 命題 12 を参照)。ただし、これは、$u$ が単射で、$u(M)$ が $N$ の直因子であり、$\Lambda(u)$ の像 ($\Lambda(M)$ と同型) が $\Lambda(N)$ の直因子である場合に当てはまります。 証明は、$\Lambda$ による $T(u)$ (§ 5, no. 2) 置き換えること $T$ に対する類似の主張と同じです。

#### 命題 4 {#alg-iii-s7-prop-4 .statement tag=062X}

*$N$ と $P$ を $A$ モジュール $M$ の 2 つの部分加群とし、それらの和 $N + P$ が $M$ の直因子であり、共通部分 $N \cap P$ が$N$と$P$の直因子。次に、準同型 $\Lambda(N) \to \Lambda(M)$、$\Lambda(P) \to \Lambda(M)$、$\Lambda(N \cap P) \to \Lambda(M)$、標準単射の正規拡大は単射法です。 $\Lambda(N)$、$\Lambda(P)$、$\Lambda(N \cap P)$ が、準同型によって $\Lambda(M)$ の部分代数と識別される場合、*
$$
\Lambda(N \cap P) = \Lambda(N) \cap \Lambda(P).
$$
証明は、$\Lambda$ によって、§ 5, no. 2、命題 4 置き換えること $T$ から派生します。 命題 4 の仮説は、$A$ が体のとき、$M$ の任意の部分加群 $N, P$ によって常に満たされます。

#### 系 {#alg-iii-s7-n2-cor-1 .statement tag=062Y}

※$K$を可換体、$M$をベクトル空間を$K$とします。すべての元 $z \in \Lambda(M)$ に対して、$M$ の最小のベクトル部分空間 $N$ が存在し、$z \in \Lambda(N)$ と $N$ は有限次元になります。*

証明は、§ 5, no. 2、系から命題 4 置き換えること $T$ から$\Lambda$ によって推定されます。

$N$ は、$\Lambda(M)$ の元 $z$ に関連付けられて、$M$ のベクトル部分空間と呼ばれます。

### 3. 外部の反可換性代数

#### 命題 5 {#alg-iii-s7-prop-5 .statement tag=062Z}

(i) $(x_i)_{1 \leq i \leq n}$ を加群 $M$ の元の有限列とします。対称群 $S_n$ の各置換 $\sigma$ に対して、

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

ここで、$\varepsilon_\sigma$ は置換 $\sigma$ の署名を表します。

(ii) $x_i = x_j$、積のような 2 つの異なる添字 $i, j$ が存在する場合

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

零です。

(i) まず、理想$\mathfrak{g}'$の定義によるすべての$x \in M$に対する$x \wedge x = 0$から、$M$の$x, y$についても、

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

これにより、$n = 2$の場合には(6)が成立します。一般的なケースは、§ 4, no. 6、補題 3 から続きます。

(ii) (ii) の仮定には、$\sigma(1) = i$ と $\sigma(2) = j$ のような置換 $\sigma \in S_n$ が存在します。この場合、(6) の左側はこの置換に対して零となり、したがって右側も同様になります。

#### 系 1 {#alg-iii-s7-prop-5-cor-1 .statement tag=0630}

$H, K$を区間の2つの相補的な部分集合、$[1, n]$の$\mathbf{N}$とし、$(i_h)_{1 \leq h \leq p}, (j_k)_{1 \leq k \leq n-p}$を増加するに配置された$H$と$K$の元の数列とします。 位数;私たちは書きます

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

それから

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

ここで、$\nu$ は、対 $(i, j) \in H \times K$ の数であり、$i > j$ になります。

命題 5までにこの簡約するから証明まで

#### 補題 1 {#alg-iii-s7-lem-1 .statement tag=0631}

$\sigma \in S_n$ が置換で、$1 \leq h \leq p$ の場合は $\sigma(h) = i_h$、$p + 1 \leq h \leq n$ の場合は $\sigma(h) = j_{n-p}$ となり、$\varepsilon_\sigma = (-1)^\nu$ になります。

$1 \leq h < h' \leq p$ または $p + 1 \leq h < h' \leq n$ の場合、対 $(h, h')$ の$\sigma(h') > \sigma(h)$ および数は、$1 \leq h \leq p < h' \leq n$ と $\sigma(h) > \sigma(h')$ が $\nu$ に等しくなります。

#### 系 2 {#alg-iii-s7-lem-1-cor-2 .statement tag=0632}

グレード付けされた代数 $\bigwedge(M)$ は交代的 ($§ 4$、no. 9) です。

生成する系集合 $M$ とし、命題 5 を使用して、$§ 4$、no. 9 ～ $\bigwedge(M)$ の命題を適用する 13 とすれば十分です。

#### 命題 6 {#alg-iii-s7-prop-6 .statement tag=0633}

*M が有限生成A-加群の場合、$\bigwedge(M)$ は有限生成A-加群です。また、M が元で生成する系を認める場合、$p > n$ は $\bigwedge^p(M) = \{0\}$ になります。*

$(x_i)_{1 \leq i \leq n}$ を M の生成する系とします。 $\bigwedge^p(M)$ のすべての元は、形の元の線形結合です。
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
ここで、添字 $i_k$ 属するから $\{1, n\}$; 命題 5 により、これらの添字は別個であると仮定できます (そうでない場合、対応する元は零になります)。 $p > n$ の場合、添字のような数列は存在しないため、$\bigwedge^p(M) = \{0\}$ になります。 $p \leq n$ の場合、これらの数列は数で有限になり、証明が完成します。

### 4. 加群および交代的マルチリニア写像の *n* 番目の外装冪

可換リング A 上の 2 つのモジュール M、N があるとすると、$M^n$ から N への *交互の n* 線形* マッピングは、すべての $p \leq n - 2$ について、次のような任意の *n* 線形マッピング $f : M^n \to N$ になります。
$$
f(u_1, \ldots, u_p, x, x, v_1, \ldots, v_{n-p-2}) = 0
$$
すべての x については、M の $u_i$ ($1 \leq i \leq p$) と $v_j$ ($1 \leq j \leq n - p - 2$) です。

#### 命題 7 {#alg-iii-s7-prop-7 .statement tag=0634}

※Aを可換環、MとNを2つA-加群とします。すべての A-線型写像 $g : \bigwedge^n(M) \to N$ ($n \geq 2$) が n 線形マッピング* に関連付けられている場合、
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 \wedge x_2 \wedge \cdots \wedge x_n)
$$
*全単射 A-線型写像は、 A-加群 $\operatorname{Hom}_A(\bigwedge^n(M), N)$ から交代的の A-加群への $M^n$ の N への n 線形写像で得られます。

$M^n$ から N への *すべての * n 線形写像の A-加群 $\operatorname{Hom}_A(T^n(M), N)$ から A-加群 $\mathscr{L}_n(M, \ldots, M; N)$ への正準全単射を、すべての A-線型写像 $f : T^n(M) \to N$ の n 線形写像と関連付けることによって得られます。
$$
\tilde{f} : (x_1, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n)
$$
(II, § 3, no. 9)。一方、A-線型写像 $g : \bigwedge^n(M) \to N$ は A-線型写像 $f : T^n(M) \to N$ と 1 対 1 の対応であり、*f は g 写像 $f = g \circ p_n$ と関連付けることにより、$\mathfrak{g}_n''$* 上の零になります。
$$
p_n : T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{g}_n''
$$

は標準準同型 (II, § 2, no. 1, 定理 1) です。しかし、$\mathfrak{J}_n''$ は形の元の線形結合であるため
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$
$M$の$(x, u_i, v_j$)、$f$が形 $g \circ p_n$であるということは、対応する$n$-線形写像$\bar{f}$が(8)を満たすことを意味し、他の語では、 *交代的*。

A-加群 $\bigwedge^n(M)$ は、M の *n 番目の外部冪* と呼ばれます。 A-加群準同型 $u : M \to N$、写像ごとに
$$
\bigwedge^n(u) : \bigwedge^n(M) \to \bigwedge^n(N)
$$
$\bigwedge^n(M)$ 上に $\bigwedge(u)$ がある一致するは、u* の *n 番目の外部冪と呼ばれます。

#### 系 1 {#alg-iii-s7-prop-7-cor-1 .statement tag=0635}

*すべての交代的 n 線形マッピング* $g : M^n \to N$ について、*すべての置換* $\sigma \in \mathfrak{S}_n$ について、
$$
g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma \cdot g(x_1, x_2, \ldots, x_n)
$$
*全員に* $x_i \in M$; *さらに、* $x_i = x_j$ *2 つの異なる添字* $i, j$ の場合、*その後*
$$
g(x_1, x_2, \ldots, x_n) = 0.
$$
これは明らかな命題 7 と no. 3、命題 5 の帰結です。

#### 系 2 {#alg-iii-s7-prop-7-cor-2 .statement tag=0636}

*$(x_i)_{1 \leq i \leq n}$ *を n の数列元の M とする*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0;
$$
*その後、交代的 n 線形マッピング*ごとに $g : M^n \to N$、$g(x_1, \ldots, x_n) = 0$ となります。

#### 系 3 {#alg-iii-s7-prop-7-cor-3 .statement tag=0637}

*$f : M^{n-1} \to A$ *を交代的* $(n-1)$*-線形* とします。 *もし* $(x_i)_{1 \leq i \leq n}$ *が n の数列元 M で、* $x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$ になる場合、 *その後*
$$
\sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i = 0
$$
*(ここでは* $f(x_1, \ldots, \hat{x}_i, \ldots, x_n) = f(x_1, \ldots, x_{i-1}, x_{i+1}, \ldots, x_n)$ *for* $1 \leq i \leq n$と書きます。

$n$ 線形写像が次のことを証明すれば十分です。
$$
(x_1, \ldots, x_n) \mapsto \sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i
$$
$M^n$ から $M$ までは *交代的* です。さて、$x_i = x_{i+1}$の場合、$f$は交代的であるため、$x_i$と$x_{i+1}$を除く、右側の和のすべての項は零係数になります。一方、$x_i$の係数は
$$
(-1)^i f(x_1, \ldots, x_{i-1}, x_{i+1}, x_{i+2}, \ldots, x_n)
$$

そして$x_{i+1}$のそれは$(-1)^{i+1} f(x_1, \ldots, x_i, x_{i+2}, \ldots, x_n)$であり、それらは仮定によって逆数になります。

#### 注意 {#alg-iii-s7-n4-rem-1 .statement tag=0638}

$T^n(M)$ の元 $z$ は、置換 $\sigma \in S_n$ (cf.) ごとに $\sigma.z = \varepsilon_\sigma z$ の場合、位数* の$n$ (反変) *歪対称テンソルと呼ばれます。 § 6, no. 3、注意);これらの元形は、$T^n(M)$ のサブ A モジュール $A'_n(M)$ です。すべての $z \in T^n(M)$ について、$a.z = \sum_{\sigma \in S_n} \varepsilon_\sigma(\sigma.z)$ と書き、$a.z$ を $z$ の *歪み対称化* と呼びます。 $\varepsilon_{\sigma\tau} = \varepsilon_\sigma \varepsilon_\tau$ と同様に、$a.z$ は斜対称テンソルであることがすぐにわかります。したがって、$z \mapsto a.z$ は $T^n(M)$ の自己準同型であり、像 $A''_n(M)$ は $A'_n(M)$ に含まれます。一般的には $A''_n(M) \neq A'_n(M)$ (練習問題 8) です。 $z$ が斜対称テンソルの場合、$a.z = n!z$。したがって、*とき* $n!$ *が $A$ で反転可能*、自己準同型 $z \mapsto (n!)^{-1}a.z$ が像の $T^n(M)$ の *射影子* である

$$
A'_n(M) = A''_n(M).
$$

さらに、この射影子の*核*はちょうど$\mathfrak{J}_n''$です。なぜなら、注意は明らかに、$n \geqslant 2$、したがって 2 ($n!$ の因子) が $A$ と $x \otimes x = 2^{-1}(x \otimes x + x \otimes x)$ で可逆である場合に限定されるからです。したがって、$\mathfrak{J}_n''$ は元 $z + \rho.z$ によって生成されます。ここで、$\rho$ は、$\{1, n\}$ の 2 つの連続する数を交換する転置です。さらに、$S_n$ の 2 つの置換 $\sigma, \tau$ については、次のように書くことができます。

$$
z - \varepsilon_{\sigma\tau}((\sigma\tau).z) = z - \varepsilon_\tau(\tau.z) + \varepsilon_\tau(\tau.z - \varepsilon_\sigma \sigma.(\tau.z))
$$

よってということは、すべての $z \in T^n(M)$ と $\sigma \in S_n$ に対して $z - \varepsilon_\sigma(\sigma.z) \in \mathfrak{J}_n''$ ということになります。したがって (常に $n!$ が $A$ で可逆であると仮定すると)、次のようになります。

$$
z - (n!)^{-1}a.z = \sum_{\sigma \in S_n} (n!)^{-1}(z - \varepsilon_\sigma(\sigma.z)) \in \mathfrak{J}_n''
$$

すべての $z \in T^n(M)$ が、私たちの主張を確立します。

$n!$ が $A$ で可逆である場合、$T^n(M)$ のサブモジュール $A'_n(M)$ と $\mathfrak{J}_n''$ は *補足* であり、正準準同型性 $T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$ の $A'_n(M)$ への制限は A モジュール *同型* であり、問題のケースで次のことを識別できます。 $M$ の $n$ 番目の外部べき乗の要素を持つ次数 $n$ の歪対称テンソル。 注意ここで、この識別は、一般に斜対称ではない 2 つの斜対称テンソルの $T(M)$ における乗法、積と互換性がないこともわかります。

### 5. スカラーの環の拡大

$A, A'$ を 2 つの可換環、$\rho : A \to A'$ 環準同型、$M$ $A$ 加群、$M'$ $A'$ 加群、$f : M \to M'$ を *A 準同型* ( $\rho$) の $M$ を $M'$ にします。合成写像 $M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} \bigwedge_{A'}(M')$ は、$M$ の A-線型写像を A-代数 $\bigwedge_{A'}(M')$ に変換し、f(M) ⊂ M' の元が $\bigwedge_{A'}(M')$ の零平方であるように、 (no. 1, 命題 1) 代数 $f'' : \bigwedge_A(M) \to \bigwedge_{A'}(M')$ を可換にする唯一の $A$-準同型性図式

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M'' & & \downarrow \phi_{M'}'' \\
\bigwedge_A(M) & \xrightarrow{f''} & \bigwedge_{A'}(M')
\end{array}
$$

$f''$ はグレード代数準同型です。 $\sigma : A' \to A''$ が他の環準同型である場合、$M''$ は $A''$ 加群、$g : M' \to M''$ は $A'$ 準同型 ($\sigma$ に対して) および $g'' : \bigwedge_{A'}(M') \to \bigwedge_{A''}(M'')$ であるとすぐに推測されます。 対応する $A''$-代数の準同型、次に代数の合成 $A$-準同型

$$
\bigwedge_A(M) \xrightarrow{f''} \bigwedge_{A'}(M') \xrightarrow{g''} \bigwedge_{A''}(M'')
$$

対応するを合成 $A$-準同型性 $g \circ f : M \to M''$ ($\sigma \circ \rho$ に対して)。

#### 命題 8 {#alg-iii-s7-prop-8 .statement tag=0639}

*$A, B$ を 2 つの可換環、$\rho : A \to B$ 環準同型、および $M$ の $A$ モジュールとします。正規の拡大*

$$
\psi : \bigwedge_B(B \otimes_A M) \to B \otimes_A \bigwedge_A(M)
$$

*$B$-線形写像* の $1_B \otimes \phi_M'' : B \otimes_A M \to B \otimes_A \bigwedge_A(M)$ *は等級付けされた $B$-代数同型写像です。*

証明は、$\bigwedge$による§ 5, no. 4、命題5置き換えること$T$、$\phi_M''$による$\phi_M$から導出されます。

### 6. 外装代数の直接極限

$(A_\alpha, \phi_{\beta \alpha})$ を、$A_\alpha$ モジュール、$A = \lim \to A_\alpha$、$M = \lim \to M_\alpha$ の可換環、$(M_\alpha, f_{\beta \alpha})$ 直接系の有向直接系とします。 $\alpha \leq \beta$ については、$A_\alpha$-準同型 $f_{\beta \alpha} : M_\alpha \to M_\beta$ から $A_\alpha$-代数準同型 (no. 5, 公式 (12)) $f_{\beta \alpha}' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_{A_\beta}(M_\beta)$ が導出され、(13) から $(\bigwedge_{A_\alpha}(M_\alpha), f_{\beta \alpha}')$ は *直接系であることがわかります。グレード* $A_\alpha$*-モジュール*。一方、$f_\alpha : M_\alpha \to M$ を標準的な $A_\alpha$ 準同型写像とします。我々は (no. 5, 公式 (12)) 段階的な $A_\alpha$-代数準同型性 $f_\alpha'' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_A(M)$ を導出し、また (13) から、$f_\alpha''$ が $A_\alpha$-準同型性の直接系を構成することもわかります。

#### 命題 9 {#alg-iii-s7-prop-9 .statement tag=063A}

*A-準同型* $f'' = \varprojlim f''_\alpha : \varprojlim \Lambda_{A_\alpha}(M_\alpha) \to \Lambda_A(M)$ *は等級付けされた代数同型* です。

証明は、$\Lambda$ による T 全体の§ 5, no. 4、命題 6 置き換えることと$\phi''$ による$\phi$ と同じであり、交代的代数の直接極限が交代的。

### 7. 直和の代数の外観。外装代数のグレード加群

A を A-加群および $j_\lambda : M_\lambda \to M$ 標準単射の家族の可換環、$M = \bigoplus_{\lambda \in L} M_\lambda$ 直和とします。等級付けされた代数 $\Lambda(j_\lambda) : \Lambda(M_\lambda) \to \Lambda(M)$ の A 準同型性が導出されます。 $\Lambda(M)$ は反可換であるため、§ 4, no. 7 の命題 10 (または必要に応じて、L が無限である場合に一般化する必要がある場合、cf. § 4, no. 8、*Reamrk* 1) を準同型 $\Lambda(j_\lambda)$ に適用できます。そうすると一意な代数準同型が存在します

$$
g : \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda) \to \Lambda(M)
$$

($g_M$ によっても示されます) $\Lambda(j_\lambda) = g \circ f_\lambda$ となるように、ここで

$$
f_\lambda : \Lambda(M_\lambda) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

は標準準同型を表します。

#### 命題 10 {#alg-iii-s7-prop-10 .statement tag=063B}

*標準準同型* g (*公式 (14)*) *はグレード代数同型* です。

g が全単射であることを証明するために、定義する a を採点代数準同型します。

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

$g \circ h$ と $h \circ g$ は、それぞれ $\Lambda(M)$ と $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ の恒等写像になります。それぞれの $\lambda \in L$ について、合成線形写像を考慮します。

$$
u_\lambda : M_\lambda \xrightarrow{\phi''_{M_\lambda}} \Lambda(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda).
$$

すべての $\lambda \in L$ に対して $u \circ j_\lambda = u_\lambda$ となるような A-線型写像 $u : M \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ が 1 つだけ存在します。スキュー テンソル積 $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ は *交代的* 代数: L 有限の場合、これは § 4, no. 9、命題 14 から求まり、L 任意の場合、これは次のとおりです。この積の定義は、§ 4, no. 8、*注意* 1 で与えられ、交代的の直接の極限が代数と評価されるという事実は、交代的です。また、$u(M)$ は、等級付けされた代数 $\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$ の次数 1 の元の部分加群に含まれているため、no. 1、命題 1 および *注意* 1 から、固有の値が存在することがわかります。評価は代数準同型。

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L} \Lambda(M_\lambda)
$$

$h \circ \phi''_M = u$ のようになります。 $g \circ h$ と $h \circ g$ が恒等写像であるという事実の検証は、§ 6, no. 6、命題 9 置き換えること $S$ が $\Lambda$ によって、$\phi'$ が$\phi''$ のように実行されます。

#### 注意 {#alg-iii-s7-n7-rem-1 .statement tag=063C}

$N = \bigoplus_{\lambda \in L} N_\lambda$ を集合のインデックスとして $L$ を持つ $A$ モジュールの他のファミリの直和とし、すべての $\lambda \in L$ について、$v_\lambda : M_\lambda \to N_\lambda$ を $A$ 線形マッピングとします。 よってには $A$ 線形マッピング $v = \bigoplus_\lambda v_\lambda : M \to N$ (II, § 1, no. 6, 命題 7) があります。それから図式

$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} \Lambda(M_\lambda) & \xrightarrow{g_M} & \Lambda(M) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(v_\lambda) & & \Lambda(v) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(N_\lambda) & \xrightarrow{g_N} & \Lambda(N)
\end{array}
$$

は可換です (cf. § 4, no. 5、系 ～ 命題 8)。

$\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$ のサブモジュール $A$ は、同型 $g$ によって$\Lambda^n(M)$ が識別されるため、より正確に記述することができます。 $L$ の有限部分集合 $J$ ごとに $E_J = \bigotimes_{\lambda \in J} \Lambda(M_\lambda)$ を書き、$\bigotimes_{\lambda \in L} \Lambda(M_\lambda) = \lim \to E_J$ が $L$ の有向集合有限部分集合の $\mathscr{F}(L)$ に対して、定義 ($§ 4$, no. 8、*注意* 1)。 $\sum_{\lambda \in L} n_\lambda = n$ と $L$ 含むの家族 $\nu$ のすべての有限部分集合 $J$ のように、すべての家族 $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ (したがって *有限* サポート) について、次のように書きます。

$$
\Lambda^{J,\nu}(M) = \bigotimes_{\lambda \in J} \Lambda^{n_\lambda}(M_\lambda)
$$

したがって、$E_J$の次数$n$の元の部分加群$E_{J,n}$は、$J$に含まれるすべての家族$\nu$の$\Lambda^{J,\nu}(M)$の*直和*になります。

$$
\sum_{\lambda \in L} n_\lambda = n
$$

($§ 4$、no. 7、命題 10、no. 8)。慣例として、$J$に支援が含まれていない家族$\nu$には$\Lambda^{J,\nu}(M) = \{0\}$と書きます。それから

E_{J,n} は、すべての $\bigwedge^{J,\nu}(M)$ の直和と呼ぶこともできます。ここで、$\nu$ は、$\sum_{\lambda \in L} n_\lambda = n$ のように、すべてのファミリー $\nu = (n_\lambda)_{\lambda \in L}$ の集合 $H_n$ を通過します。 $\bigwedge^0(M_\lambda)$ は $A$ と同一視されるため、明らかに $L$ の 2 つの有限部分集合 $J \subset J'$ と、$J$、標準写像 $\bigwedge^{J,\nu}(M) \to \bigwedge^{J',\nu}(M)$ (標準写像の制限) に含まれる家族 $\nu$ も対象となります。 $E_J \to E_{J'}$ ～ $\bigwedge^{J,\nu}(M)$) は全単射です。 $\nu \in H_n$ 全員に対して、次のように書くと、

$$
\bigwedge^\nu(M) = \lim_{\longrightarrow} \bigwedge^{J,\nu}(M)
$$

II, § 6, no. 2、命題 5 を考慮すると、次のようになることがわかります。

#### 系 {#alg-iii-s7-n7-cor-1 .statement tag=063D}

*A-加群 $\bigwedge^n(M)$ は、* $\bigotimes_{\lambda \in L} \bigwedge(M_\lambda)$* の部分加群の同型 (14) の下の像です * * 部分加群* の直和 $\bigwedge^\nu(M)$* *すべての家族向け* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$* * そのような* $\sum_{\lambda \in L} n_\lambda = n$; *if* $J$* が* $\nu$、$\bigwedge^\nu(M)$* のサポートである場合、 * $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$ と標準的に同型です。

一般に、$\bigwedge^\nu(M)$、$\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$、および$\bigwedge^n(M)$ の像が識別されます。この規約により、次のようになります。

#### 命題 11 {#alg-iii-s7-prop-11 .statement tag=063E}

*$\Delta$ を可換モノイド、$M$ を型 $\Delta$ の等級付けされた A-加群、および* $(M_\alpha)_{\alpha \in \Delta}$* *その卒業であるものとします。注文した対* $(\alpha, n) \in \Delta \times \mathbf{N}$ ごとに、*$\bigwedge^{\alpha,n}(M)$* * $\bigwedge^n(M)$* の部分加群 * 部分加群* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_{\alpha_\lambda})$ の直和、*ここで* $(n_\lambda)_{\lambda \in L}$* * の家族の集合を実行します整数* $\geq 0$* *そのような* $\sum_{\lambda \in L} n_\lambda = n$、$J$* *はそのサポートであり、それぞれ* $(n_\lambda)$、$(\alpha_\lambda)_{\lambda \in J}$* *は* $\Delta^J$* *そのような* $\sum_{\lambda \in J} \alpha_\lambda = \alpha$ の家族の集合を通過します。 *その後* $(\bigwedge^{\alpha,n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$* *は型* $\Delta \times \mathbf{N}$* の唯一の卒業式です * 代数構造の卒業* $\bigwedge(M)$* * そして、誘導するの卒業* $M = \bigwedge^1(M)$* * と互換性があります。

$\bigwedge(M)$ が $\bigwedge^{\alpha,n}(M)$ の直和であるという事実は、系から命題 10 に続きます。 証明の残りは、§ 5, no. 5、命題 7の証明の終わりと同じです。

### 8. 外観代数/自由加群

#### 定理 1 {#alg-iii-s7-thm-1 .statement tag=063F}

*$M$* *A-加群と基底* $(e_\lambda)_{\lambda \in L}$ とします。 *完全に順序付けられた集合* (集合理論, III, § 2, no. 3, 定理 1)* のうち $L$* * 構造が与えられるようにします* *そして、すべての有限部分集合* $J$* * の* $L$* *を書きます*

$$
e_J = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}
$$

ここで、$(\lambda_k)_{1 \leq k \leq n}$ は、増加する位数 (集合理論, III, § 5, no. 3, 命題 6) に配置された J の元の数列です。 Aの$e_\varnothing = 1$、単位元と書きます。 次に、J が L の有限部分集合の集合 $\mathscr{F}(L)$、外装代数 $\bigwedge(M)$ の形基底を通過する $e_J$ です。

$e_\lambda$ は A モジュール M を生成するため、$\bigwedge(M)$ のすべての要素は要素 $e_\lambda$ の有限数の積の線形結合であり、したがって (no. 3 の命題 5 を考慮すると) $J \in \mathscr{F}(L)$ に対する有限数の要素 $e_J$ の線形結合になります。 簡約するから証明まで、$e_J$ は A 上で線形独立です。 そうしないと、これらの要素間に、係数がすべてゼロではない線形関係が存在することになります。この関係の係数が $\neq 0$ である $e_J$ に対応するサブセット J の和集合は、L の有限サブセット K になります (有限数の係数 $\neq 0$ しかないため)。 N を、$\lambda \in K$ となるように $e_\lambda$ によって生成された M の部分加群とします。 N は M の直因子であるため、(no. 2) $\bigwedge(N)$ は $\bigwedge(M)$ の部分代数と同一視され、$e_J$ が $\bigwedge(N)$ の $J \subset K$ 形基底であることを示せば、望ましい矛盾が得られます。

したがって、M の基底が有限である場合、簡約するは定理 1 を提供します。したがって、$L = \{1, m\} \subset N$ と仮定することができます。それぞれの $i \in L$ について、$M_i$ を M の自由な部分加群 $Ae_i$ とします。 Mは$M_i$の直和、$\bigwedge(M_i)$は$\bigwedge^0(M_i) = A$と$\bigwedge^1(M_i) = M_i$の直和（no. 3、命題6）です。 $\bigwedge(M)$ を、$\bigwedge(M_i)$ (no. 7、命題 10) の A-加群テンソル積と正規に識別するとします。後者は、基底 $(1, e_i)$ の $\bigwedge(M_i)$ (II, § 3, no. 7、系 2 ～ 命題 7) の基底テンソル積です。したがって、すべての元を取得します

$$
u_1 \otimes u_2 \otimes \cdots \otimes u_m
$$

ここで、$u_i = 1$ または $u_i = e_i$ のいずれかです。 J が添字の集合である場合、$u_i = e_i$、$u_1 \otimes u_2 \otimes \cdots \otimes u_m$ は $e_J$ と同一となり、証明が完成します。

#### 系 1 {#alg-iii-s7-thm-1-cor-1 .statement tag=063G}

$L = \{1, m\}$ だと仮定します。すると、$\bigwedge(M)$ の基底 $(e_J)_{J \in \mathscr{P}(L)}$ は $2^m$ 元になります。 $p > m$、$\bigwedge^p(M) = \{0\}$の場合。 $\bigwedge^m(M)$ には、単一の元 $e_L$ のうち基底からなるがあります。 $e_J$ の基底 $(e_J)$ $\bigwedge^p(M)$ からなるの元の $0 \leq p \leq m$ 数では、$\mathrm{Card}(J) = p$ は次のようになります

$$
\binom{m}{p} = \frac{m!}{p!(m-p)!}
$$

これは、集合理論、III, § 3, no. 5、命題 12 および集合理論、III, § 5, no. 8、系 1 から命題 11 と続きます。

定理 1 の集合 L が任意である場合に戻り、基底 $(e_J)$ の乗法表 (§ 1, no. 7) を明示的に与えます。完全に順序付けられた集合 $L$ のうち 2 つの有限部分集合 $J, K$ が与えられると、次のようになります。
$$
\begin{cases}
\rho_{J, K} = 0 & \text{if } J \cap K \neq \varnothing \\
\rho_{J, K} = (-1)^v & \text{if } J \cap K = \varnothing
\end{cases}
$$
ここで、$v$ は、対 $(\lambda, \mu) \in J \times K$ の数を表し、$\lambda > \mu$ となります。次に、no. 2 の系 1 から命題 4 は、すぐに関係を意味します。
$$
e_J \wedge e_K = \rho_{J, K} e_{J \cup K}.
$$
注意公式
$$
\rho_{J, K} \rho_{K, J} = (-1)^{jk}
$$
$J \cap K = \varnothing, j = \mathrm{Card}(J), k = \mathrm{Card}(K)$ (no. 3、系 2 ～ 命題 5) のとき

#### 系 2 {#alg-iii-s7-thm-1-cor-2 .statement tag=063H}

*M が射影 A-加群の場合、$\bigwedge(M)$ は射影 A-加群です。*

証明は、§ 5, no. 5、系～定理 1 置き換えること T by $\bigwedge$と同じです。

#### 系 3 {#alg-iii-s7-thm-1-cor-3 .statement tag=063I}

*M を M の元の射影 A-加群および $(x_i)_{1 \leq i \leq n}$ 有限列とします。 M 交代的の n 線形形式 f が存在するには、*
$$
f(x_1, x_2, \ldots, x_n) \neq 0,
$$
*それは必要かつ十分です* $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$。

条件が必要であることは (M に仮定がないので) すでにわかっています (no. 4、命題 7)。ここで、M が射影であると仮定します。
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0.
$$
この場合、$\bigwedge^n(M)$ は射影 (系 2) であるため、標準写像
$$
\bigwedge^n(M) \to (\bigwedge^n(M))^{**}
$$
単射法です (II, § 2, no. 7、系 4 ～ 命題 13)。私たち結論するには、$g(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \neq 0$のような線型形式$g : \bigwedge^n(M) \to A$が存在します。 $f$ が交代的の n 線形形式対応するから $g$ (no. 4、命題 7) である場合、$f(x_1, \ldots, x_n) \neq 0$。

### 9. 線形独立性の基準

#### 命題 12 {#alg-iii-s7-prop-12 .statement tag=063J}

*M を射影 A-加群とします。 M の元 $x_1, x_2, \ldots, x_n$ が線形従属であるためには、A に次のような $\lambda \neq 0$ が存在することが必要かつ十分です*
$$
\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0.
$$

条件は必要です (M に仮定はありません)。たとえば、$\lambda x_1$ ($\lambda \neq 0$ あり) が $x_2, \ldots, x_n$ の線形結合である場合、関係 (22) が成り立ちます (no. 3, 命題 5)。 $n$ の帰納法によって条件で十分であることがわかります。 $n = 1$ の場合、それは定義の簡単な帰結です。従って、$n > 1$ と条件 (22) がいくつかの $\lambda \neq 0$ に当てはまると仮定します。もし
$$
\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n = 0,
$$
この場合、帰納法の仮定は、$x_2, \ldots, x_n$ が線形従属であることを意味し、従って *なおさら* $x_1, x_2, \ldots, x_n$ も線形従属であることを意味します。 $\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n \neq 0$ の場合、no. 8、系 3 から定理 1 から、$f(\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n) = \mu \neq 0$ のような交代的 $(n - 1)$ 線形形式 $f$ が存在することがわかります。以来
$$
x_1 \wedge (\lambda x_2) \wedge \cdots \wedge x_n = 0,
$$
no. 8、系 3 から定理 1 から、$\mu x_1$ は $\lambda x_2, x_3, \ldots, x_n$ の線形結合であることがわかります。従って、$x_1, x_2, \ldots, x_n$ は線形従属です。

#### 系 {#alg-iii-s7-n9-cor-1 .statement tag=063K}

*M と N を 2 つの射影 A-加群と $f : M \to N$ A-線型写像とします。 f が単射の場合、$\Lambda(f) : \Lambda(M) \to \Lambda(N)$ は単射です。*

これを最初に仮定の下でMが*自由*であることを証明します。 $(e_\lambda)_{\lambda \in L}$ を M の基底とすると、$(e_J)_{J \in \mathfrak{B}(L)}$ (公式 (18)) は $\Lambda(M)$ の基底になります。 $\Lambda(f)$ 含む元 $u = \sum_J \alpha_J e_J \neq 0$ の核とします。 K を $\alpha_J \neq 0$ となる有限部分集合 J の中で最小の元とし、H を K からの L 互いに素の有限部分集合とし、$K \cup H$ 含むすべての J (数で有限) とする。 $\alpha_J \neq 0$; $\alpha_J \neq 0$ などのすべての $J \neq K$ について、従って、定義 $J \cap H \neq 0$ までに、結果として (no. 8, 公式 (20)) になります。
$$
u \wedge e_H = +\alpha_K e_{K \cup H}
$$
$\Lambda(M)$、$\Lambda(f)$の核の両面理想に対して属する。 $e_{K \cup H} = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}$と書きます。次に$\alpha_K f(e_{\lambda_1}) \wedge f(e_{\lambda_2}) \wedge \cdots \wedge f(e_{\lambda_n}) = 0$; 命題 12、元 $f(e_{\lambda_i})$ ($1 \leq i \leq n$) により、N は線形従属になります。しかし、この矛盾する仮定と $f$ は単射法です (II, § 1, no. 11、系 3 から命題 17)。

ここで一般的なケースを考えます。 $M'$ を A-加群として、$M \oplus M' = P$ が自由になるようにします (II, § 2, no. 2, 命題 4)。 線形写像 $g : M \oplus M' \to N \oplus M \oplus M'$ が $g(x, y) = (f(x), 0, y)$ となるように、可換図式が存在することを考えます。
$$
\begin{array}{ccc}
M & \xrightarrow{f} & N \\
j \downarrow & & j' \downarrow \\
P & \xrightarrow{g} & N \oplus P
\end{array}
$$

ここで、垂直矢印は標準単射です。 $g$ は単射であり、$P$ は自由であるため、上で見たように、$\Lambda(g)$ は単射準同型です。さて、$M$は$P$(no. 2)の直因子なので、$\Lambda(j): \Lambda(M) \to \Lambda(P)$は単射準同型になります。合成準同型

$$
\Lambda(M) \xrightarrow{\Lambda(j)} \Lambda(P) \xrightarrow{\Lambda(g)} \Lambda(N \oplus P)
$$

従って、これは単射的であり、合成準同型にも等しいため、

$$
\Lambda(M) \xrightarrow{\Lambda(f)} \Lambda(N) \xrightarrow{\Lambda(g')} \Lambda(N \oplus P)
$$

私たち結論するその $\Lambda(f)$ は単射です。

#### 命題 13 {#alg-iii-s7-prop-13 .statement tag=063L}

*$M$を$A$モジュール、次元$p$と$\Lambda^p(N)$の$\{u\}$基底を含まない$M$の$N$直和因子部分加群とする。 元 $x \in M$ ～ 属する ～ $N$ の場合、$u \wedge x = 0$ であることが必要十分です。*

$P$ を $N$ と相補的な $M$ の部分加群とし、$y \in N,\ z \in P$ を $x = y + z$ となるようにします。次に$u \wedge x = u \wedge z$。 $\Lambda^p(N)$ は次元 1、写像 $\phi: P \to P \otimes \Lambda^p(N)$ を含まないので、$\phi(p) = p \otimes u$ は全単射 (II, § 3, no. 4、命題 4) になります。一方 (no. 7、命題 10)、標準準同型の合成

$$
\psi: P \otimes \Lambda^p(N) \to \Lambda(P) \otimes \Lambda(N) \to \Lambda(M)
$$

は単射です。したがって、写像 $\psi \circ \phi$ は単射法、よって命題です。

#### 定理 2 {#alg-iii-s7-thm-2 .statement tag=063M}

*$M$を有限基底$(e_i)_{1 \leq i \leq n}$を持つ$A$加群とする。 $n$ の数列 $(x_i)_{1 \leq i \leq n}$ $M$ の元から $M$ の形基底については、次のような元 $\lambda \in A$ が必要かつ十分です。

$$
x_1 \wedge x_2 \wedge \ldots \wedge x_n = \lambda \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

$A$ で反転可能。*

$e_1 \wedge e_2 \wedge \cdots \wedge e_n$ は $\Lambda^n(M)$ の基底の一意元 (no. 8, 系 1 ～ 定理 1) であるため、元 $\lambda \in A$ 満たす (23) は一意に決定されます。 $(x_i)_{1 \leq i \leq n}$ が $M$ の基底で、$x_1 \wedge x_2 \wedge \cdots \wedge x_n$ が $\Lambda^n(M)$ (no. 8) の基底の一意元である場合、$\lambda$ は可逆です。逆に、$\lambda$ が可逆であると仮定します。次に、交代的 $n$-線形形式 $f$ 対応するから線形写像 $g: \Lambda^n(M) \to A$ のようになります

$$
g(e_1 \wedge e_2 \wedge \cdots \wedge e_n) = \lambda^{-1}
$$

$f(x_1, x_2, \ldots, x_n) = 1$ のようなものです。 $x \in M$ 全員にとって、明らかに

$$
x \wedge x_1 \wedge \cdots \wedge x_n = 0
$$

(no. 3、命題 6); 適用 no. 8、系 3 から定理 1 を取得します。

$$
f(x_1, x_2, \ldots, x_n) \cdot x = \sum_{i=1}^n (-1)^{i-1} f(x, x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i.
$$

$f(x_1, \ldots, x_n) = 1$ として、これは、すべての $x \in M$ が $x_1, x_2, \ldots, x_n$ の線形結合であり、後者は線形独立であることを示しています (

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0),
$$

彼らは $M$ の形基底です。

### 練習問題 {#alg-iii-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
