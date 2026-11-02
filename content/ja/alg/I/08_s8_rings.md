---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 8
section_title: Rings
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 96-114, 171-174
pdf_pages: 0120-0138, 0195-0198
extraction: ocr
subsections:
    - "no": 1
      title: RINGS
      page: 96
      pdf_page: 120
    - "no": 2
      title: CONSEQUENCES OF DISTRIBUTIVITY
      page: 98
      pdf_page: 122
    - "no": 3
      title: EXAMPLES OF RINGS
      page: 101
      pdf_page: 125
    - "no": 4
      title: RING HOMOMORPHISMS
      page: 102
      pdf_page: 126
    - "no": 5
      title: SUBRINGS
      page: 103
      pdf_page: 127
    - "no": 6
      title: IDEALS
      page: 103
      pdf_page: 127
    - "no": 7
      title: QUOTIENT RINGS
      page: 105
      pdf_page: 129
    - "no": 8
      title: SUBRINGS AND IDEALS IN A QUOTIENT RING
      page: 106
      pdf_page: 130
    - "no": 9
      title: MULTIPLICATION OF IDEALS
      page: 107
      pdf_page: 131
    - "no": 10
      title: PRODUCT OF RINGS
      page: 108
      pdf_page: 132
    - "no": 11
      title: DIRECT DECOMPOSITION OF A RING
      page: 110
      pdf_page: 134
    - "no": 12
      title: RINGS OF FRACTIONS
      page: 112
      pdf_page: 136
statements: 32
exercises: 16
content_sha256: 14a989e3037ea029175495b2bf7a063425efef02e5e288ca4a8ea8ea3659ef53
translated_from: content/en/alg/I/08_s8_rings.md
translation_method: google
source_content_sha256: 9e2e678718b8b04bcfb806c30df7ec34dec70b897c7a14a41eee1a9ca40499a1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 762abc32293dc7343a56ad5df095edb633535216efe27c087d038bd33e841068
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。 環

### 1. 環

#### 定義 1 {#alg-i-s8-def-1 .statement tag=05H2}

*環は集合* $\mathbf{A}$ *合成の 2 つの法則は、それぞれ加法および乗法、満たすと呼ばれ、次の公理* です。

(AN I) *加法* の下で $\mathbf{A}$ *は可換群* です。
(AN II) *乗法は結合性があり、単位元* を所有しています。
(AN III) *乗法は加法* に関して分配的です。
*環* $\mathbf{A}$ *その乗法が可換* である場合、それは可換であると言われます。

以下では、$(x, y) \mapsto x + y$ は加法と $(x, y) \mapsto xy$ 乗法を表します。 $0$は加法の場合は単位元、乗法の場合は$1$を表します。最後に、$-x$ は、加法の下の $x$ のマイナスを示します。したがって、環の公理は次の恒等式で表されます。

$$
\begin{array}{ll}
(1) & x + (y + z) = (x + y) + z \quad \text{(associativity of addition)} \\
(2) & x + y = y + x \quad \text{(commutativity of addition)} \\
(3) & 0 + x = x + 0 = x \quad \text{(zero)} \\
(4) & x + (-x) = (-x) + x = 0 \quad \text{(negative)} \\
(5) & x(yz) = (xy)z \quad \text{(associativity of multiplication)} \\
(6) & x.1 = 1.x = x \quad \text{(unit element)} \\
(7) & (x + y).z = xz + yz \\
(8) & x.(y + z) = xy + xz \quad \text{(distributivity)}
\end{array}
$$

最後に、$\mathbf{A}$ の $x, y$ に対して $xy = yx$ であれば、環 $\mathbf{A}$ は可換です。

加法だけでは、$\mathbf{A}$ は、$\mathbf{A}$ の *加法群* と呼ばれる可換群です。すべての $x \in \mathbf{A}$ について、左ホモテティー $\gamma_x$ と右ホモテティー $\delta_x$ を $\gamma_x(y) = xy$、$\delta_x(y) = yx$ で定義するとします。式(7)と(8)により、$\gamma_x$と$\delta_x$は$\mathbf{A}$の加法群の自己準同型であるため、写像零から零となり、負から負になります。したがって、

$$
\begin{align*}
(9) & \quad x.0 = 0.x = 0 \\
(10) & \quad x.(-y) = (-x).y = -xy;
\end{align*}
$$
したがって、$(-x)(-y) = -((-x).y) = -(-xy)$、よって
$$(11) \quad (-x)(-y) = xy.$$
式 (10) と (11) は * 符号規則 * を構成します。したがって、
$$-x = (-1)x = x(-1)$$
そして$(-1)(-1) = 1$。

(11) から、$n$ の帰納法によって、
$$(12) \quad (-x)^n = \begin{cases} x^n & \text{if } n \text{ is even} \\ -x^n & \text{if } n \text{ is odd.} \end{cases}$$

*消去可能* 元、*反転可能* 元、*置換可能* 元、*中心的* 元、*セントラライザー* または環 $\mathbf{A}$ の *中心* について話すとき、これらすべて概念 $\mathbf{A}$の乗法を参照します。 $x, y \in \mathbf{A}$ と $y$ が可逆である場合、$\mathbf{A}$ が可換である場合、$\mathbf{A}$ の元 $xy^{-1}$ も $x/y$ で表されます。 $\mathbf{A}$の可逆元の集合は乗法で安定しています。 乗法によって誘発された法則では、$\mathbf{A}$ の *乗法群* と呼ばれる群となり、$\mathbf{A}^*$ で示されるときどきになります。

$x, y$ を $\mathbf{A}$ に入れます。 $x = y'y$ (または $x = yy'$) となる $y' \in \mathbf{A}$ が存在する場合、$x$ は $y$ の *左* (または *右*) *倍数* であると言われます。 $y$ は *権利* であるとも言われています (それぞれ

左)xの因子。 A が可換である場合、「左」と「右」を区別する必要はありません。

上記の用語に従って、すべての元 $y \in \mathbf{A}$ は 0 の右側と左側の因子とみなされます。しかし、言葉の乱用により、一般に項「0 の右 (左) 因子」は元 $y$ のために予約されており、満たす関係 $xy = 0$ (それぞれ 0) には $x \neq 0$ が存在します。 $yx = 0$）。他の語では、零の右(それぞれ左)因子は、右(それぞれ左)キャンセル不可の元です。

$x \in \mathbf{A}$ にしましょう。 $x^n = 0$ とともに整数 $n > 0$ が存在する場合、$x$ は nilpotent と呼ばれます。 元 $1 - x$ は反転可能であり、その逆数は次と等しくなります。
$$
1 + x + x^2 + \cdots + x^{n-1}.
$$

A は加法の下で可換群であるため、$n \in \mathbf{Z}$ と $x \in \mathbf{A}$ に対して元 $nx$ が定義されています (§ 2, no. 8)。 $\gamma_x$と$\delta_x$は加法群Aの自己準同型であるため、$\gamma_x(ny) = n\gamma_x(y)$と$\delta_y(nx) = n\delta_y(x)$、よって
$$
x.(ny) = (nx).y = n.(xy).
$$
特に$nx = (n.1)x$。

乗法のもとで単位元の存在を保証するものを除いて、環の公理を加法と乗法満たすを組み合わせた集合 A は、擬似環と呼ばれます。

### 2. 分配性の帰結

加法に対する乗法の分配により、§ 3, no. 4 の 1 が命題を適用するとなり、次のようになります。
$$
\prod_{i=1}^n \left( \sum_{\lambda \in L_i} x_{i,\lambda} \right) = \sum_{\alpha_1, \ldots, \alpha_n} \prod_{i=1}^n x_{i, \alpha_i}
$$
ここで、和拡大するは数列 $(\alpha_1, \ldots, \alpha_n)$ 所属から $L_1 \times \cdots \times L_n$ までであり、$i = 1, \ldots, n$ では、環 A の元の家族 $(x_{i,\lambda})_{\lambda \in L_i}$ は有限台です。

#### 命題 1 {#alg-i-s8-prop-1 .statement tag=05H3}

A を可換環および $(x_\lambda)_{\lambda \in L}$ を A の元の有限族とします。正の整数 $\beta = (\beta_\lambda)_{\lambda \in L}$ のすべての族について、$|\beta| = \sum_{\lambda \in L} \beta_\lambda$ とします。それから
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}.
$$
$L_i = L$ と $x_{i,\lambda} = x_\lambda$ を$1 \leq i \leq n$ に適用して、公式 (13) を適用します。それから
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{\alpha_1, \ldots, \alpha_n} x_{\alpha_1} \cdots x_{\alpha_n},
$$
和は数列 $\alpha = (\alpha_1, \ldots, \alpha_n) \in L^n$ 全体に広がります。

$\alpha$ を $L^n$ にしましょう。すべての $\lambda \in L$ について、$U_\lambda^\alpha$ は整数 $i$ の集合を表し、$1 \leq i \leq n$ と $\alpha_i = \lambda$ を$\Phi(\alpha) = (U_\lambda^\alpha)_{\lambda \in L}$ とします。 $\Phi$ が $L^n$ の全単射を $L$ でインデックス付けされた $\{1, 2, \ldots, n\}$ の分割の集合に重ねたものは明らかです。 $|\beta| = n$ のようなすべての $\beta \in \mathbf{N}^L$ について、すべての $\lambda \in L$ について $\mathrm{Card}\ U_\beta^\alpha = \beta_\lambda$ となるような $\alpha \in L^n$ の集合を $L_\beta^n$ で表します。したがって、家族 $(L_\beta^n)_{|\beta|=n}$ は $L^n$ の分割であり、

$$
\mathrm{Card}\ L_\beta^n = \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!}
$$

(§ 5, no. 5)。

最後に、$\alpha \in L_\beta^n$については、

$$
x_{\alpha_1} \cdots x_{\alpha_n} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_{\alpha_i} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_\lambda = \prod_{\lambda \in L} x_\lambda,
$$

よって

$$
\sum_{(\alpha_1, \ldots, \alpha_n)} x_{\alpha_1} \cdots x_{\alpha_n} = \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} x_{\alpha_1} \cdots x_{\alpha_n}
= \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}
= \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} x_\lambda^{\beta_\lambda}
$$

したがって、公式 (14) は (15) から導かれます。

#### 系 1 (二項公式) {#alg-i-s8-prop-1-cor-1 .statement tag=05H4}

*x と y を可換環 A の 2 つの元とします。すると*:

$$
(x + y)^n = \sum_{p=0}^n \binom{n}{p} x^p y^{n-p}.
$$

公式 (14) を $L = \{1, 2\}$、$x_1 = x$、$x_2 = y$ に適用すると、次のようになります。

$$
(x + y)^n = \sum_{p+q=n} \frac{n!}{p! q!} x^p y^q,
$$

和は、正の整数 $p, q$ の順序付けられた対を $p + q = n$ と拡張します。二項式公式はこれからすぐに続きます (*集合理論*, III, § 5, no. 8)。

#### 系 2 {#alg-i-s8-prop-1-cor-2 .statement tag=05H5}

*A を、A の元の 2 つのファミリーである可換環、X 集合、$\mathbf{u} = (u_x)_{x \in X}$、$\mathbf{v} = (v_x)_{x \in X}$ とします。$\mathbf{u} + \mathbf{v}$ がファミリー $(u_x + v_x)_{x \in X}$ を表すものとします。すべての $\lambda \in \mathbf{N}^{(X)}$ に対して、$\lambda! = \prod_{x \in X} \lambda(x)!$ と書きます。次に、§ 7, no. 8 の記法のすべての $\alpha \in \mathbf{N}^{(X)}$ について、

$$
(\mathbf{u} + \mathbf{v})^\alpha = \sum_{\beta + \gamma = \alpha} \frac{\alpha!}{\beta! \gamma!} \mathbf{u}^\beta \mathbf{v}^\gamma.
$$

$x \in X$の場合、

$$
(u_x + v_x)^{\alpha(x)} = \sum_{m+n=\alpha(x)} \frac{\alpha(x)!}{m! n!} u_x^m v_x^n
$$

系による 1. $x \in X$ に対してこれらの方程式の積を取り、(13) を使用すると、系が得られます。

#### 命題 2 {#alg-i-s8-prop-2 .statement tag=05H6}

※$A$を$A$と$I = \{1, 2, \ldots, n\}$の環、$x_1, \ldots, x_n$元とします。 $H \subset I$の場合は、$x_H = \sum_{i \in H} x_i$と書きます。それから*

$$
(-1)^n \sum_{\sigma \in S_n} x_{\sigma(1)} \cdots x_{\sigma(n)} = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

*特に、$A$ が可換の場合、

$$
(-1)^n n! x_1 x_2 \cdots x_n = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

$C$を$I$の写像の集合を$\{0, 1\}$とします。それぞれの $H \subset I$ をその特性写像にマッピングすると、$\mathscr{P}(I)$ から $C$ に全単射が得られます。したがって、(16) の右辺は次と等しくなります。

$$
\sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \left( \sum_{i \in I} a(i) x_i \right)^n
$$
$$
= \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \sum_{(i_1, \ldots, i_n) \in I^n} a(i_1) \ldots a(i_n) x_{i_1} \ldots x_{i_n}
$$
$$
= \sum_{(i_1, \ldots, i_n) \in I^n} c_{i_1 \ldots i_n} x_{i_1} \ldots x_{i_n}
$$

どこで

$$
c_{i_1 \ldots i_n} = \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n).
$$

(1) $(i_1, \ldots, i_n)$が$I$の置換ではないとします。 $i_1, \ldots, i_n$とは異なる$j \in I$が存在します。 $C'$ を $a \in C$ の集合として、$a(j) = 0$ とします。すべての $a \in C'$ について、$a^*$ を $a$ の和と $\{j\}$ の特性写像とします。次に $a^*(1) + \cdots + a^*(n) = a(1) + \cdots + a(n) + 1$ 以降

$$
c_{i_1 \ldots i_n} = \sum_{a \in C'} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n) + (-1)^{a^*(1)+\cdots+a^*(n)} a^*(i_1) \ldots a^*(i_n)
$$
$$
= \sum_{a \in C'} ((-1)^{a(1)+\cdots+(n)} + (-1)^{a(1)+\cdots+a(n)+1}) a(i_1) \ldots a(i_n) = 0.
$$

(2) $i_1 = \sigma(1), \ldots, i_n = \sigma(n)$ となるような $\sigma \in S_n$ が存在するとします。すると、$a(i_1) \ldots a(i_n) = 0$ 〜でない限り $a$ は値 1 しかかかりません。したがって、$c_{i_1 \ldots i_n} = (-1)^n$ になります。

### 3. 例/環

I。 零環。 Aを環とします。 A の $0 = 1$ については、A が 1 つの元で構成されていれば必要十分です。 条件で十分であることは明らかです。一方、$0 = 1$ の場合、すべての$x \in A$、$x = x.1 = x.0 = 0$ になります。このような環を零環と呼びます。

II。合理的整数の環。 § 2, no. 5 で定義された加法、および § 2, no. 6 で定義された乗法では、$\mathbf{Z}$ は可換環になります。 記法 0、1、$-x$は先に紹介した記法に準じます。

*III。実質値写像の環。 I を実数の集合 $\mathbf{R}$ の区間とし、A を実数値で I に定義された連続写像の集合とします。 2 つの写像 $f$ と $g$ のうち、和 $f + g$ と積 $f.g$ は次のように定義されます。
$$(f + g)(t) = f(t) + g(t), \quad (fg)(t) = f(t)g(t) \quad (t \in I).$$
単位元が定数 1 である可換環が得られます。*

*IV。畳み込み擬似リング。 E を $\mathbf{R}$ 上の実数値連続写像の集合とし、これは有界区間の外側にある零です。 2 つの写像のうち和は III のように定義されますが、積は次のように定義されます。
$$(fg)(t) = \int_{-\infty}^{\infty} f(s)g(t-s)\ ds$$
(「畳み込み積」)。したがって、環 (cf. 積分、VIII, §4) ではない可換擬似環が得られます。

V。 環の反対環 A. Aを環とします。 A と同じ加法と乗法 $(x, y) \mapsto yx$ を持つ集合 A は、$A^0$ で表されることがよくあります。それは、A と同じ零と同じ単位元を持ち、A が可換である場合に限り、A と一致するをもつ環 (A の反対環と呼ばれる) です。

VI。可換群の自己準同型環。 G を加法的に書かれた可換性群とする。 E を G の自己準同型の集合とします。E に $f$ と $g$ が与えられると、G の G の写像 $f + g$ と $fg$ は次のように定義されます。
$$(f + g)(x) = f(x) + g(x), \quad (fg)(x) = f(g(x)) \quad (x \in G).$$
§ 1, no. 5、命題 5 により、$f + g$ は G の自己準同型であるため、明らかに $fg = f \circ g$ でもあります。 § 4, no. 8 までに、E は加法の下で (可換) 群になります。 乗法は明らかに連想的であり、単位元 $\mathrm{Id}_G$ があります。また、E の $f, g$ と $h$ については、$\phi = f.(g + h)$ と書きます。 $x \in G$の皆さん、
$$\phi(x) = f((g + h)(x)) = f(g(x) + h(x)) = f(g(x)) + f(h(x))$$
$f$ は G の自己準同型です。したがって$\phi = fg + fh$、そして明らかに
$$(g + h)f = gf + hf.$$

したがって、E は G* の *自己準同型環と呼ばれる (一般に可換ではない) 環です。

VII。 *零平方の擬似環。* すべての $x, y \in A$ に対して $xy = 0$ であれば、擬似環 A は零平方であると言われます。 G を可換群とする。 集合 G に群 G と乗法 $(x, y) \mapsto 0$ の加法を与えると、零平方の擬似環が得られます。 $G = \{0\}$の場合は環のみで、その場合は零環になります。

### 4. 環準同型

#### 定義 2 {#alg-i-s8-def-2 .statement tag=05H7}

※AとBを2つの環とします。 A から B への射または準同型は、A から B への任意の写像 f 満たす関係:*

$$
f(x + y) = f(x) + f(y), \quad f(xy) = f(x) \cdot f(y), \quad f(1) = 1,
$$

*全員に* $x, y$ *A* で。

2 つの環準同型のうち合成は環準同型です。 A と B を、A を B に変換した 2 つの環と $f$ 写像とします。 $f$ が同型であるためには、それが全単射準同型であることが必要かつ十分です。この場合、$f^{-1}$ は B の準同型を A に変換したものです。 A の環の準同型を A の *自己準同型* と呼びます。

$f : A \to B$ を環準同型とします。 写像 $f$ は、A の加法群の準同型が B の加法群になります。特に、$f(0) = 0$ と $f(-x) = -f(x)$ はすべての $x \in A$ に当てはまります。 The image under $f$ of an invertible element of A is an invertible element of B and $f$ induces a homomorphism of the multiplicative group of A into the multiplicative group of B.

#### 例 {#alg-i-s8-n4-exa-1 .statement tag=05H8}

(1) A を環とします。 It is immediately seen that the mapping $n \mapsto n \cdot 1$ of $\mathbf{Z}$ into A is the unique homomorphism of $\mathbf{Z}$ into A. 特に、$\mathbf{Z}$ の恒等写像は、環 $\mathbf{Z}$ の一意な自己準同型です。

特に、A を加法群 $\mathbf{Z}$ の自己準同型環 (no. 3, 例 VI) とします。 The mapping $n \mapsto n \cdot 1$ of $\mathbf{Z}$ into A is an isomorphism of $\mathbf{Z}$ onto A by the very construction of multiplication in $\mathbf{Z}$ (§ 2, no. 6).

(2) $a$ を環 A の可逆元とします。 写像 $x \mapsto axa^{-1}$ は、A の自己準同型です。

$$
a(x + y)a^{-1} = axa^{-1} + aya^{-1},
$$
$$
a(xy)a^{-1} = (axa^{-1})(aya^{-1}).
$$

これは全単射であり、関係 $x' = axa^{-1}$ は $x = a^{-1}x'a$ と同等です。したがって、これは環 A の自己同型であり、$a$ に関連付けられた *内部自己同型* と呼ばれます。

### 5. 部分環

#### 定義 3 {#alg-i-s8-def-3 .statement tag=05H9}

$A$を環とします。 A subring of $A$ is any subset $B$ of $A$ which is a subgroup of $A$ under addition, which is stable under multiplication and which contains the unit of $A$.

上記の条件は次のように書くことができます

$$
0 \in B, \quad B + B \subset B, \quad -B \subset B, \quad B.B \subset B, \quad 1 \in B.
$$

$B$が$A$の部分環であれば、$A$のものによって加法と乗法が与えられ、環になります。 $B$の$A$の標準単射は環準同型です。

#### 例 {#alg-i-s8-n5-exa-1 .statement tag=05HA}

(1) 含む 1 が $\mathbf{Z}$ に等しい、加法群 $\mathbf{Z}$ の各部分群 。したがって、$\mathbf{Z}$ は $\mathbf{Z}$ の唯一の部分環です。

(2) $A$ を環とし、$(A_t)_{t \in I}$ を $A$ の部分環の家族とする。 $\bigcap_{t \in I} A_t$が$A$の部分環であるのは明らかです。 In particular, the intersection of the subrings of $A$ containing a subset $X$ of $A$ is a subring called the subring of $A$ generated by $X$.

(3) $X$ を環 $A$ の部分集合とします。 $A$の$X$のセントラライザーは$A$の部分環です。特に、$A$の中心は$A$の部分環です。

(4) Let $G$ be a commutative group with operators; let $\Omega$ denote the set of operators and $\alpha \mapsto f_\alpha$ the action of $\Omega$ on $G$. Let $E$ be the endomorphism ring of the group without operators $G$ and $F$ the set of endomorphisms of the group with operators $G$. 定義までに、$F$ は $G$ の自己準同型 $\phi$ で構成され、すべての $\alpha \in \Omega$ に対して $\phi \cdot f_\alpha = f_\alpha \cdot \phi$ になります。 したがって、$F$ は環 $E$ の部分環です。 $F$ は、$G$ (cf. II, § 1, no. 2) の演算子を使用して、群の自己準同型環と呼ばれます。 $F_1$ を、$f_\alpha$ によって生成された $E$ の部分環とします。 次に、$F$ は $E$ の $F_1$ のセントラライザーです。

### 6. 理想

#### 定義 4 {#alg-i-s8-def-4 .statement tag=05HB}

$A$ を環とします。 部分集合 $a$ の $A$ は、$A$ の加法群の部分群であり、関係 $a \in A, x \in a$ が $ax \in a$ (それぞれ $xa \in a$) を暗示している場合、左 (または右) イデアルと呼ばれます。 $a$ は、$A$ の左イデアルと右イデアルの両方である場合、$A$ の両側イデアルと呼ばれます。

左イデアルの定義は関係で表現できます

$$
0 \in a, \quad a + a \subset a, \quad A.a \subset a
$$

公式 $(-1).x = -x$ と $A.a \subset a$ に続く関係 $-a \subset a$。すべての $x \in A$ について、$\gamma_x$ を $A$ の写像 $a \mapsto xa$ を $A$ にします。 作用 $x \mapsto \gamma_x$ は、演算子の集合として $A$ を使用して、$A$ の加法群 $A^+$ 群の構造を与えます。 $A$ の左の理想は、この作用の下で安定する $A^+$ の部分群だけです。

環 $A$ の左の理想は、反対環 $A^0$ の右の理想です。 可換環では、3 種類の理想は同じです。それらは単に理想と呼ばれます。

#### 例 {#alg-i-s8-n6-exa-1 .statement tag=05HC}

(1) $A$ を環とします。 集合 $A$ は $A$ の両面の理想です。 0 の集合からなるも同様で、これは零理想と呼ばれ、ときどきは $\{0\}$ の代わりに 0 または $(0)$ で表されます。

(2) $A$ の各元 $a$ に対して、$a$ の左倍数の集合 $A.a$ が左イデアルです。同様に、集合 $a.A$ も正しい理想です。 $a$が$A$、$A.a = a.A$の中心にある場合。このイデアルは、$a$ によって生成される主イデアルと呼ばれ、$(a)$ で示されます。 $(a) = A$ は、$a$ が反転可能な場合に限ります。

(3) $M$ を $A$ の部分集合とします。 The set of elements $x \in A$ such that $xy = 0$ for all $y \in M$ is a left ideal of $A$ called the left annihilator of $M$. $M$ の右零化イデアルも同様に定義されます。

(4) $A$ の左 (それぞれ右、両側) のすべての共通部分は、左 (それぞれ右、両側) のイデアルです。 $A$ の部分集合 $X$ が与えられると、したがって、左 (それぞれ右、両側) 最小のの理想含む $X$ が存在します。それは、$X$ によって生成される左 (または右、両側) イデアルと呼ばれます。

$a$を$A$の左イデアルとします。 条件 $1 \notin a, a \neq A$ は明らかに同等です。

#### 定義 5 {#alg-i-s8-def-5 .statement tag=05HD}

※$A$を環とします。言葉の乱用により、左理想 $a$ は、$A$ とは異なる左理想の集合のうち極大元である場合に最大であると言われます。

他の語では、$a \neq A$の場合に$a$が最大となり、$A$含む$a$の唯一残っている理想は$a$と$A$です。

#### 定理 1 (クルル) {#alg-i-s8-thm-1 .statement tag=05HE}

*$A$を環、$a$を$A$とは異なる$A$の左理想とする。 $A$ 含む $a$ の最大理想 $m$ が存在します。

$A$ は、左乗法によって $A$ の加法群 $A^+$ 上で操作されると考えてください。すると$A$の左理想は$A^+$の安定した部分群になります。したがって、定理は、§ 4, no. 3 から続き、命題 3 が $A^+$ の部分集合 $P = \{1\}$ に適用されます。

#### 命題 3 {#alg-i-s8-prop-3 .statement tag=05HF}

*$A$ を環とし、$(x_\lambda)_{\lambda \in L}$ を $A$ の元と $a$ (それぞれ $b$) 和の集合 $\sum_{\lambda \in L} a_\lambda x_\lambda$ とします。ここで、$(a_\lambda)_{\lambda \in L}$ は$A$の元の有限台を持つ家族（それぞれ$\sum_{\lambda \in L} a_\lambda x_\lambda b_\lambda$、ここで$(a_\lambda)_{\lambda \in L}, (b_\lambda)_{\lambda \in L}$は$A$の元の有限台を持つ家族）。このとき、$a$ (それぞれ $b$) は、元 $x_\lambda$ によって生成された $A$ の左側 (それぞれ両側) イデアルです。

数式

$$
0 = \sum_{\lambda \in L} 0.x_\lambda
$$
$$
\sum_{\lambda \in L} a_\lambda x_\lambda + \sum_{\lambda \in L} a'_\lambda x_\lambda = \sum_{\lambda \in L} (a_\lambda + a'_\lambda)x_\lambda
$$
$$
a.\sum_{\lambda \in L} a_\lambda x_\lambda = \sum_{\lambda \in L} (aa_\lambda)x_\lambda
$$

$a$ が左イデアルであることを証明します。 $a'$ をすべての $\lambda \in L$ に対して $x_\lambda \in a'$ となるような左イデアルとし、$(a_\lambda)_{\lambda \in L}$ を $A$ の有限台との家族とする。次に、すべての $\lambda \in L$、よって $\sum_{\lambda \in L} a_\lambda x_\lambda \in a'$ に対して $a_\lambda x_\lambda \in a'$。したがって$a \subset a'$です。したがって、$a$ は、$x_\lambda$ によって生成された $A$ の左イデアルです。 $b$ の議論も同様です。

#### 命題 4 {#alg-i-s8-prop-4 .statement tag=05HG}

*$A$を環、$(a_\lambda)_{\lambda \in L}$を$A$の左理想の家族とする。 $\bigcup_{\lambda \in L} a_\lambda$ によって生成される左イデアルは、和 $\sum_{\lambda \in L} y_\lambda$ で構成されます。ここで、$(y_\lambda)_{\lambda \in L}$ は、すべての $\lambda \in L$ に対して $y_\lambda \in a_\lambda$ となるような有限台を持つ族です。

$a$ を和 $\sum_{\lambda \in L} y_\lambda$ の集合とし、すべての $\lambda \in L$ に対して $y_\lambda \in a_\lambda$ を加えます。式$\sum_{\lambda \in L} x_\lambda + \sum_{\lambda \in L} y_\lambda = \sum_{\lambda \in L} (x_\lambda + y_\lambda)$と$a \cdot \sum_{\lambda \in L} x_\lambda = \sum_{\lambda \in L} a x_\lambda$は、$a$が$A$の左イデアルであることを示しています。 $\lambda \in L$ と $x \in a_\lambda$ としましょう。 $\mu \neq \lambda$には$y_\lambda = x$と$y_\mu = 0$を書きます。次に$x = \sum_{\lambda \in L} y_\lambda$、よって $x \in a$、そして最後に$a_\lambda \subset a$です。すべての $\lambda \in L$ に対する左イデアル $a'$ 含む $a_\lambda$ の場合、明らかに含む $a$ となり、したがって $a$ は $\bigcup_{\lambda \in L} a_\lambda$ によって生成されます。

$\bigcup_{\lambda \in L} a_\lambda$によって生成されたイデアル$a$を左イデアル*$a_\lambda$の*和と呼び、$\sum_{\lambda \in L} a_\lambda$(cf.II, § 1, no. 7)で表します。特に、左の 2 つの理想のうち和 $a_1 + a_2$ は、$a_1 \in a_1$ と $a_2 \in a_2$ である和 $a_1 + a_2$ で構成されます。

### 7. 商環

$A$ を環とします。 $a$ が $A$ の両側イデアルである場合、$A$ の 2 つの元 $x$ と $y$ は、$x \equiv y$ (mod. $a$) または $x \equiv y(a)$ と書かれた *合同法* $a$ であると言われます。 $x - y \in a$。こちらは$A$の同値関係です。 関係 $x \equiv y(a)$ と $x' \equiv y'(a)$ は $x + x' \equiv y + y'(a)$ を暗示し、$a$ の $xx' \equiv xy'(a)$ は左の理想、$a$ の $xy' \equiv yy'(a)$ は右の理想、よって $xx' \equiv yy'(a)$ を意味します。逆に、$R$が加法と乗法と互換性のある$A$の同値関係であれば、$x \equiv 0$modの集合$a$になります。 $R$ は両面の理想であり、$x \equiv y$ は修正です。 $R$ は $x \equiv y$ mod と同等です。 $a$。

Let $A$ be a ring and $a$ a two-sided ideal of $A$. $A/a$ denotes the quotient set of $A$ by the equivalence relation $x \equiv y(a)$, with addition and multiplication the quotients of those on $A$ ($§ 1$, no. 6, Definition 11). $A/a$ が環であることを示します。

(a) Under addition, $A/a$ is the quotient commutative group of the additive group of $A$ by the subgroup $a$.

(b) 乗法では、$A/a$ はモノイド ($§ 2$, no. 1) です。

(c) $\xi, \eta, \zeta$ を $A/a$ とし、$\pi : A \to A/a$ を標準写像とします。 $A$ では選ぶ元 $x, y, z$ が$\pi(x) = \xi, \pi(y) = \eta$ と $\pi(z) = \zeta$ になります。それから
$$
\xi(\eta + \zeta) = \pi(x)\pi(y + z) = \pi(x(y + z)) = \pi(xy + xz)
= \pi(x)\pi(y) + \pi(x)\pi(z) = \xi\eta + \xi\zeta
$$
関係 $(\xi + \eta)\zeta = \xi\zeta + \eta\zeta$も同様に成立します。

#### 定義 6 {#alg-i-s8-def-6 .statement tag=05HH}

$A$を環、$a$を$A$の両面理想とする。 The quotient ring of $A$ by $a$, denoted by $A/a$, is the quotient set of $A$ by the equivalence relation $x \equiv y(a)$, with addition and multiplication the quotients of those on $A$.

環 $A/\{0\}$ は $A$ と同型で、$A/A$ は零環です。

#### 定理 2 {#alg-i-s8-thm-2 .statement tag=05HI}

Let $A$ be a ring and $a$ a two-sided ideal of $A$.
(a) The canonical mapping $\pi$ of $A$ onto $A/a$ is a ring homomorphism.
(b) Let $B$ be a ring and $f$ a homomorphism of $A$ into $B$. $f(a) = \{0\}$ の場合、$A/a$ の $B$ には $f = \bar{f} \circ \pi$ となる準同型 $\bar{f}$ が 1 つだけ存在します。

$A$ の $x, y$ に対して構成、$\pi(x + y) = \pi(x) + \pi(y)$、$\pi(xy) = \pi(x)\pi(y)$ まで。また、$\pi(1)$ は、$A/a$、よって (a) の単位元 $\varepsilon$ です。

Let $A^+$ be the additive group of $A$ and $B^+$ that of $B$; as $f$ is a homomorphism of $A^+$ into $B^+$, zero on the subgroup $a$ of $A^+$, there exists (§ 4, no. 4, Proposition 5) one and only one homomorphism $\bar{f}$ of $A^+/a$ into $B^+$ such that $f = \bar{f} \circ \pi$. $\xi, \eta$ を $A/a$ に入れます。 $A$ に $\pi(x) = \xi$ と $\pi(y) = \eta$ が入った選ぶ $x, y$。その後、$\xi \eta = \pi(xy)$、よって

$$
\bar{f}(\xi \eta) = \bar{f}(\pi(xy)) = f(xy) = f(x)f(y) = \bar{f}(\xi)\bar{f}(\eta)
$$

そして $\bar{f}(\varepsilon) = f(\pi(1)) = f(1)$ なので、$\bar{f}$ は環準同型になります。

#### 定理 3 {#alg-i-s8-thm-3 .statement tag=05HJ}

$A$と$B$を$A$の環と$f$準同型を$B$にします。
(a) $f$ の核 $a$ は、$B$ の両面の理想です。
(b) $f$ の像 $B' = f(B)$ は、$B$ の部分環です。
(c) $\pi : A \to A/a$ と $i : B' \to B$ を正規の射とします。 $A/a$ の $B'$ には、$f = i \circ \bar{f} \circ \pi$ と $\bar{f}$ が同型となる射 $\bar{f}$ が 1 つだけ存在します。

As $f$ is a morphism of the additive group of $A$ into that of $B$, $a$ is a subgroup of $A$. $x \in a$ と $a \in A$ の場合、$f(ax) = f(a)f(x) = 0$、したがって $ax \in a$、同様に $xa \in a$ になります。したがって、$a$ は $A$ の両面の理想です。 主張 (b) は明らかです。 As $f$ is zero on $a$, there exists a morphism $\bar{f}$ of $A/a$ into $B'$ such that $f = i \circ \bar{f} \circ \pi$ (Theorem 2). The uniqueness of $\bar{f}$ and the fact that $\bar{f}$ is an isomorphism follow from Set Theory, II, § 6, no. 4.

### 8. 部分環と商環の理想

#### 命題 5 {#alg-i-s8-prop-5 .statement tag=05HK}

$A$と$A'$を、$A$の環、$f$準同型を、$f$の$A'$と$a$核にします。
(a) $B'$ を $A'$ の部分環とします。すると、$B = f^{-1}(B')$は$A$含む$a$の部分環になります。 $f$が全射であれば、$B/a$の移行から商同型を$B'$にすると、$f(B) = B'$と$f|_B$定義するになります。
(b) $b'$ を、$A'$ の左 (それぞれ右、両側) イデアルとします。この場合、$b = f^{-1}(b')$ は、$A$ 含む $a$ の左 (または右、両側) イデアルです。

(c) *If $b'$ is a two-sided ideal of $A'$, the composite mapping of the canonical morphism $A' \to A'/b'$ and $f : A \to A'$ defines, when passing to the quotient, an injective morphism $\bar{f}$ of $A/b$ into $A'/b'$. $f$ が全射であれば、$\bar{f}$ は $A/b$ の $A'/b'$ 上の同型です。

(d) *$f$ が全射であると仮定します。 $\Phi$ を $A$ 含む $a$ の部分環 (それぞれ左の理想、右の理想、両側の理想) の集合とします。 $\Phi'$ を $A'$ の部分環 (それぞれ左の理想、右の理想、両側の理想) の集合とします。 写像 $B \to f(B)$ と $B' \mapsto \bar{f}(B')^{-1}$ は、$\Phi$ の $\Phi'$ と $\Phi'$ の $\Phi$ の逆全単射です。

(a) と (b) は明らかですが、no. 7、定理 3 から続く (a) の最後の主張を除きます。

(c) で考慮された合成射 $g : A \to A' \to A'/b'$ には核 $b$ があり、したがって $\bar{f}$ は $A/b$ から $A'/b'$ (§ 8, no. 7, 定理 3) への単射射です。 $f$ が全射である場合、$g$ は全射であり、したがって $\bar{f}$ は全射です。

$f$ が全射であると仮定します。以上により、写像 $\theta : B' \mapsto \bar{f}(B')^{-1}$ は $\Phi'$ の写像が $\Phi$ になります。明らかに、写像 $\eta : B \mapsto f(B)$ は、$\Phi$ の写像が $\Phi'$ になります。次に、$\theta \circ \eta = \mathrm{Id}_{\Phi}, \eta \circ \theta = \mathrm{Id}_{\Phi'},$ よって (d)。

#### 注意 {#alg-i-s8-n8-rem-1 .statement tag=05HL}

上記では、記法、$\theta$、$\eta$ は集合同型に順序付けされます ($\Phi$ と $\Phi'$ は包含により順序付けされます)。

#### 系 {#alg-i-s8-n8-cor-1 .statement tag=05HM}

*$A$を環、$a$を$A$の両面理想とする。
(a) $A/a$ のすべての左 (または右、両面) イデアルは、形 $b/a$ で一意に書くことができます。ここで、$b$ は、$A$ 含む $a$ の左 (右、両面) イデアルです。
(b) $b$ が両面の場合、移行から商同型に$A/b$ を$(A/a)/(b/a)$ に合成した準同型 $A \to A/a \to (A/a)/(b/a)$ 定義する。

$A$ の正規化射を $A/a$ に命題を適用する 5 を足すだけで十分です。

### 9. 理想の乗法

$A$を環、$a$、$b$を$A$の両面理想とする。 The set of elements of the form $x_1 y_1 + \cdots + x_n y_n$ with $n \geq 0, x_i \in a$ and $y_i \in b$ for $1 \leq i \leq n$, is obviously a two-sided ideal of $A$, which is denoted by $ab$ and called the *product* of the two-sided ideals $a$ and $b$. この乗法のもとでは、$A$の両側イデアルの集合は、単位元の両側イデアル$A$とのモノイドです。 $a, b, c$ が $A$ の両面の理想である場合、$a(b+c) = ab + ac, (b+c)a = ba + ca$ です。 $A$ が可換であれば、イデアルの乗法も可換です。

$ab \subset aA \subset a$ と $ab \subset Ab \subset b$、したがって

$$
ab \subset a \cap b.
$$

(21)

#### 命題 6 {#alg-i-s8-prop-6 .statement tag=05HN}

※$a, b_1, \ldots, b_n$を$A$の両面の理想とする。すべての $i$ に対して $A = a + b_i$ の場合、$A = a + b_1 b_2 \ldots b_n = a + (b_1 \cap b_2 \cap \cdots \cap b_n)$。*

(21) までに、$A = a + b_1 b_2 \ldots b_n$ を証明すれば十分です。 帰納法までに$n = 2$の場合を考えれば十分です。 仮定までに、$1 = a + b_1 = a' + b_2$となるような$a, a' \in a, b_1 \in b_1, b_2 \in b_2$が存在します。それから
$$
1 = a' + (a + b_1) b_2 = (a' + a b_2) + b_1 b_2 \in a + b_1 b_2,
$$
よって $A = a + b_1 b_2$。

#### 命題 7 {#alg-i-s8-prop-7 .statement tag=05HO}

*$b_1, \ldots, b_n$を、$i \neq j$に対して$b_i + b_j = A$となるような$A$の両側理想とする。次に$b_1 \cap b_2 \cap \cdots \cap b_n = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$。特に、$A$ が可換の場合、$b_1 \cap b_2 \cap \cdots \cap b_n = b_1 b_2 \ldots b_n$ (cf. 練習問題 2)。*

まず$n = 2$とします。 $a_1 + a_2 = 1$ となるような $a_1 \in b_1, a_2 \in b_2$ が存在します。 $x \in b_1 \cap b_2$の場合は、$x = x(a_1 + a_2) = x a_1 + x a_2 \in b_2 b_1 + b_1 b_2$。したがって$b_1 \cap b_2 = b_1 b_2 + b_2 b_1$です。

ここで、すべての整数 $< n$ に対して命題の方程式が成立するとします。 命題 6、$b_n + (b_1 b_2 \ldots b_{n-1}) = A$までに、そしてそれ以降
$$
b_1 \cap b_2 \cap \cdots \cap b_n = (b_1 \cap b_2 \cap \cdots \cap b_{n-1}) b_n + b_n (b_1 \cap b_2 \cap \cdots \cap b_{n-1})
$$
$$
= \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right) b_n
$$
$$
+ b_n \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right)
$$
$$
\subset \sum_{\tau \in S_n} b_{\tau(1)} b_{\tau(2)} \cdots b_{\tau(n)} \subset b_1 \cap b_2 \cap \cdots \cap b_n.
$$

### 10. 環中積

$(A_i)_{i \in I}$ を環の家族とします。 $A$ を積集合 $\prod_{i \in I} A_i$ とします。 $A$ 加法と乗法は次の式で定義されます
$$
(x_i) + (y_i) = (x_i + y_i), \quad (x_i)(y_i) = (x_i y_i).
$$
$A$ は、環 $A_i$ の *積* と呼ばれる環であり、零元 $0 = (0_i)_{i \in I}$ で、$0_i$ は $A_i$ の零であることがすぐに検証されます。 単位元 $1 = (1_i)_{i \in I}$、ここで、$1_i$ は $A_i$ の単位元です。 $A_i$ が可換であれば、$A$ も可換です。 $C_i$が$A_i$の中心であれば、$A$の中心は$\prod_{i \in I} C_i$です。

すべての $i \in I$、射影 $A$ の $A_i$ 上の$\mathrm{pr}_i$ は、環準同型です。 $B$ が環で、$f_i : B \to A_i$ が準同型の族である場合、すべての $i \in I$ に対して $f_i = \mathrm{pr}_i \circ f$ となるような一意な準同型 $f : B \to A$ が存在します。それは$f(b) = (f_i(b))_{i \in I}$によって与えられます。

すべての $i \in I$ について、$a_i$ を $A_i$ の左イデアルとします。すると、$a = \prod_{i \in I} a_i$は$A$の左イデアルになります。右イデアル、両側の理想、および部分環についても同様の結果が得られます。

$a_i$ がすべての $i \in I$ の両側イデアルであると仮定し、$f_i$ が $A_i$ から $A_i / a_i$ への標準写像を表すとします。 Then the mapping $f : (x_i)_{i \in I} \mapsto (f_i(x_i))_{i \in I}$ of $\prod_{i \in I} A_i$ onto $\prod_{i \in I} (A_i / a_i)$ is a ring homomorphism of kernel $\prod_{i \in I} a_i$ and hence defines when passing to the quotient an isomorphism of $\left( \prod_{i \in I} A_i \right) / \left( \prod_{i \in I} a_i \right)$ onto $\prod_{i \in I} (A_i / a_i)$.

$(I_\lambda)_{\lambda \in L}$ を $I$ の分割とします。 $\prod_{i \in I} A_i$ の $\prod_{\lambda \in L} \left( \prod_{i \in I_\lambda} A_i \right)$ に対する正規の全単射は環同型であり、その下にこれら 2 つの環が識別されます。

$J \subset I$ にしましょう。 $e_J$ は、$i \in J$ の場合は $x_i = 1_i$、$i \in I - J$ の場合は $x_i = 0_i$ によって定義される $A$ の元 $(x_i)_{i \in I}$ を表すものとします。次に、$e_J$ は $A$ の中心冪等 ($§ 1$、no. 4) です。次の式がすぐに続きます。

$$
\begin{align*}
e_I &= 1; \\
e_\varnothing &= 0; \\
e_{J \cap K} &= e_J e_K & \text{for } J \subset I, K \subset I; \\
e_{J \cup K} &= e_J + e_K & \text{for } J \subset I, K \subset I, J \cap K = \varnothing; \\
\sum_\lambda e_{J_\lambda} &= 1 & \text{if } (J_\lambda) \text{ is a finite partition of } I.
\end{align*}
$$

$A_J = \prod_{i \in J} A_i$ にしましょう。 $\eta_J$ を $A$ の $A_J$ に対する正規の射影とします。 $x = (x_i)_{i \in J} \in A_J$ の場合、$\varepsilon_J(x)$ を $i \in J$ の場合は $y_i = x_i$、$i \in I - J$ の場合は $y_i = 0_i$ によって定義される $A$ の元 $(y_i)_{i \in I}$ とします。 次に、$\eta_J$ は $A$ の環準同型から $A_J$ に、$\varepsilon_J$ は $A_J$ の加法群から $A$ に、そして図式では単射準同型になります。

$$
A_J \xrightarrow{\varepsilon_J} A \xrightarrow{\eta_{I-J}} A_{I-J}
$$

$\eta_{I-J}$ の核 $a_J$ は $\varepsilon_J$ の像に等しい。次に、すべての $x, x' \in A_J$ に対して $\varepsilon_J(xx') = \varepsilon_J(x)\varepsilon_J(x')$ です。ただし、$\varepsilon_J$ は一般に $\varepsilon_J(1) = e_J$ の環準同型ではありません。明らかに$a_J = e_J A = A e_J$。

すべての $i \in I$ を $e_{(i)} = e_i$ と $a_i = a_{(i)} = e_i A = A e_i$ とします。次に、$e_i^2 = e_i$、

$$
e_i e_j = e_j e_i = 0
$$

$i \neq j$の場合。 $I$ が有限である場合、$\sum_{i \in I} e_i = 1$、加法群 $A$ は、両面理想 $a_i$ の直和であり、$x \in A$ の場合、$a_i$ の成分は $x e_i$ です。次の命題がすぐに推測されます。

#### 命題 8 {#alg-i-s8-prop-8 .statement tag=05HP}

*$I$が有限であると仮定します。 $b$ が $A$ の左または右の理想である場合、$b$ は $b \cap a_i$ の直和です。

### 11. 直接分解/環

$A$ を環と $(b_i)_{i \in I}$ を $A$ の両面の理想のファミリーとします。 準同型に電話します

$$
x \mapsto (\phi_i(x))_{i \in I},
$$

where $\phi_i$ is the canonical homomorphism of $A$ onto $A/b_i$, the canonical homomorphism of $A$ into $\prod_{i \in I} (A/b_i)$.

#### 命題 9 {#alg-i-s8-prop-9 .statement tag=05HQ}

*$A$を環、$(b_1, \ldots, b_n)$を$i \neq j$に対して$b_i + b_j = A$となるような$A$の両側理想とする。 $A$ の $\prod_{i=1}^n (A/b_i)$ への標準準同型は核 $\bigcap_{i=1}^n b_i = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}.$* の全射です

明らかに核は$\bigcap_{i=1}^n b_i$です。全射性を証明するには、$A$の元の各家族$(x_i)_{1 \leq i \leq n}$に対して、すべての$1 \leq i \leq n$に対して$x \equiv x_i (b_i)$となるような$x \in A$が存在することを示す必要があります。この主張を $I$ の $n$ の基数で帰納法によって証明します。$n \leq 1$ の場合は自明です。 帰納法の仮定までに、$1 \leq i \leq n-1$に対して$y \equiv x_i (b_i)$となるような$y \in A$が存在します。 $z \in A$ で形 $y + z$ の $x$ を探します。 $i < n$ の場合は必然的に $z \equiv 0 (b_i)$、つまり $z \in b = \bigcap_{i=1}^{n-1} b_i$ となり、逆に $z \equiv x_n - y (b_n)$ になります。現在、$b_n + b = A$ は、no. 9、命題 6、よってによって$z$ の存在を示しています。最後に、no. 9、命題 7 から核の 2 番目の式が続きます。

#### 定義 7 {#alg-i-s8-def-7 .statement tag=05HR}

※$A$を環とします。 $A$ の $\prod_{i \in I} (A/b_i)$ への標準準同型が同型となるような、$A$ の両面イデアの有限族 $(b_i)_{i \in I}$ を、$A$ の直接分解と呼びます。

#### 命題 10 {#alg-i-s8-prop-10 .statement tag=05HS}

*$A$を環、$A'$をその中心、$(b_i)_{i \in I}$を$A$の両面理想の有限族とする。次の条件は同等です。

(a) 家族 $(b_i)_{i \in I}$ は $A$ の直接の分解です。
(b) $i \neq j$ に対して $e_i e_j = 0$、$1 = \sum_{i \in I} e_i$ および $i \in I$ に対して $b_i = A(1 - e_i)$ となるような、$A'$ のべき等の族 $(e_i)_{i \in I}$ が存在します。
(c) $i \neq j$ および $\bigcap_{i \in I} b_i = \{0\}$ の場合は $b_i + b_j = A$。
(d) $I$ の合計位数ごとに $i \neq j$ および $\prod_{i \in I} b_i = \{0\}$ に対して $b_i + b_j = A$。
(e) $i \in I$ に対して $b_i = A b'_i$ となるような、$A'$ の直接の分解 $(b'_i)_{i \in I}$ が存在します。

(a) $\Rightarrow$ (b)。 条件 (a) が成り立つ場合、$A$ は環 $\prod_{i \in I} (A/b_i)$ と、$b_i$ は $\mathrm{pr}_i$ の核と識別される可能性があります。 (b) の性質を持つ $e_i$ の存在は、no. 10 から続きます。

(b) $\Rightarrow$ (d)。 (b)の性質を持つ$e_i$が存在すると仮定します。 $i \neq j$、$1 - e_i \in b_i, \ e_i = e_i(1 - e_j) \in b_j$ の場合、$1 \in b_i + b_j$、$A = b_i + b_j$ となります。一方、I に全順序が与えられ、$(x_i)_{i \in I}$ が A の元の族である場合、$e_i$ が中心であるため、

$$
\prod_{i \in I} x_i (1 - e_i) = \left( \prod_{i \in I} x_i \right) \left( \prod_{i \in I} (1 - e_i) \right) = \left( \prod_{i \in I} x_i \right) \left( 1 - \prod_{i \in I} e_i \right) = 0
$$

したがって$\prod_{i \in I} b_i = \{0\}$です。

(d) $\Rightarrow$ (c)。これは、no. 9、命題 7 から続きます。

(c) $\Rightarrow$ (a)。これは命題9から続きます。

したがって、条件 (a)、(b)、(c)、および (d) は同等です。彼らが保持していると仮定してください。 (b) $\Rightarrow$ (a) により、$b'_i = A'(1 - e_i)$ の家族は $A'$ の直系の分解になります。次に、すべての $i \in I$ に対して $b_i = A(1 - e_i) = Ab'_i$ です。したがって、条件 (e) が成り立ちます。

最後に、条件 (e) が成り立つとします。 (a) $\Rightarrow$ (b) により、$i \neq j$ に対して $e_i e_j = 0$、$1 = \sum_{i \in I} e_i$ および $i \in I$ に対して $b'_i = A'(1 - e_i)$ となるような、$A'$ のべき等の族 $(e_i)_{i \in I}$ が存在します。すると $i \in I$ に対して $b_i = Ab'_i = A(1 - e_i)$ となるので、条件 (b) が成り立ちます。

#### 注意 {#alg-i-s8-n11-rem-1 .statement tag=05HT}

Aを環とします。 $(a_i)_{i \in I}$ を、$A^+$ が $a_i$ の直和となるような、A の加法群 $A^+$ の部分群の有限族とします。 $i \in I$ の場合は $a_i a_i \subset ai$、$i \neq j$ の場合は $a_i a_j = \{0\}$ であるとします。すると、$a_i$ は、すべての $i \in I$ にとって、A の両面理想です。A 上の人たちによって誘発された加法と乗法により、$a_i$ は、$a_i$ で $1 \in A$ の単位元成分を伴う環になります。 $b_i = \sum_{j \neq i} a_j$ の場合、明らかに命題 10 の $b_i$ 満たす条件 (c)、したがって $(b_i)_{i \in I}$ は A の直接の分解であり、これは $(a_i)_{i \in I}$ によって *定義される*と言われます。

#### 例 {#alg-i-s8-n11-exa-1 .statement tag=05HU}

*理想と* $\mathbf{Z}$の商環

$\mathbf{Z}$ の理想は $\mathbf{Z}$ の加法部分群であり、したがって $n \geqslant 0$ との形 $n.\mathbf{Z}$ です。逆に、すべての整数 $n \geqslant 0$ に対して、集合 $n.\mathbf{Z}$ は理想であり、主要な理想は $(n)$ です。したがって、$\mathbf{Z}$ のすべての理想は主要であり、形 $n\mathbf{Z}$ と $n \geqslant 0$ で一意に表現されます。理想 $(1)$ は $\mathbf{Z}$ に等しく、理想 $(0)$ は 0 で構成され、$\mathbf{Z}$ と $\{0\}$ とは異なる理想は、したがって $n > 1$ を伴う形 $n\mathbf{Z}$ になります。 $m \geqslant 1$ と $n \geqslant 1$、$m\mathbf{Z} \supset n\mathbf{Z}$ が $n \in m.\mathbf{Z}$ の場合に限り、つまり $m$ 割る $n$ になります。したがって、理想的な$n\mathbf{Z}$が最大であるためには、$n$と区別され、$n$を分割する整数$m > 1$が存在しないことが必要かつ十分です。他の語では、*最大イデアル* $\mathbf{Z}$ *は形* $p\mathbf{Z}$ のイデアルです。 *ここで* $p$ *は素数数* (§ 4, no. 10, 定義 16) です。

$m$ と $n$ を 2 つの整数 $\geqslant 1$ とします。理想的な$m\mathbf{Z} + n\mathbf{Z}$ が主要ですが、よってには $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$ を特徴とする整数 $d \geqslant 1$ があります。すべての整数 r \geqslant 1、関係 「r 割る d」は $r\mathbf{Z} \supset d\mathbf{Z}$ と同等であり、したがって「$r\mathbf{Z} \supset m\mathbf{Z}$ および $r\mathbf{Z} \supset n\mathbf{Z}$」、つまり「r 割る m および n」と同等です。したがって、m と n の共通の因子は d の因子であり、d は m と n に対して因子 $\geqslant 1$ 共通のの *極大* であることがわかります。 d は m と n の *最大の共通の因子* (g.c.d. と略記) と呼ばれます。 $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$として、$d = mx + ny$となるような2つの整数xとyが存在します。 m と n は、g.c.d. の場合、*相対的に素*であると言われます。は 1 に等しい。$mx + ny = 1$ に対して整数 x と y が存在すると仮定することは同じことになる。

理想 $m\mathbf{Z}$ と $n\mathbf{Z}$ の共通部分は、含む $mn$ にとってゼロではないため、$r \geqslant 1$ との形 $r\mathbf{Z}$ になります。上記のように議論すると、r の倍数は m と n の共通の倍数であり、r は m と n の共通の倍数である整数 $\geqslant 1$ の *最小* であることがわかります。これは、m と n の *最小共通の倍数* (l.c.m.) と呼ばれます。

理想$m\mathbf{Z}$と$n\mathbf{Z}$の積は、$x_1, \ldots, y_r \in \mathbf{Z}$に対する$\sum_{i=1}^{r} mx_i ny_i = mn \left( \sum_{i=1}^{r} x_i y_i \right)$の集合なので、$mn\mathbf{Z}$と等しくなります。

すべての整数 $n \geqslant 1$ に対して、商環 $\mathbf{Z}/n\mathbf{Z}$ は、整数モジュロ n* の *環と呼ばれます。 n 個の元は、整数 0, 1, 2, ..., $n - 1$ の類モジュロです。 $n = 1$ の場合、零環が得られます。

#### 命題 11 {#alg-i-s8-prop-11 .statement tag=05HV}

*$n_1, \ldots, n_d$ を対と $n = n_1 \ldots n_r$ で互いに素である整数 $\geqslant 1$ とします。 $\mathbf{Z}$ の標準準同型から積環 $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$ は、$\mathbf{Z}/n\mathbf{Z}$ の核 $n\mathbf{Z}$ と定義する環同型の $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$ への全射です。

$a_i = n_i\mathbf{Z}$を$i = 1, \ldots, r$にしましょう。 仮定、$a_i + a_j = \mathbf{Z}$までに$i \neq j$まで。 命題は命題 9 から続きます。

上記の結果は、分解から素数因子に関する結果と同様に、主イデアル整域の研究に特化した章 VII, § 1 と階乗ドメインの研究に特化した *可換代数*、章 VII, § 3 で一般化されます。

### 12. 環/分数

#### 定理 4 {#alg-i-s8-thm-4 .statement tag=05HW}

*A を A の可換環と S 部分集合とします。$A_S$ を S の分母 (§ 2, no. 4) を持つ A の分数のモノイド (乗法のみで提供) とします。 $\varepsilon : A \to A_S$ を正規の射とします。 $A_S$ 加法満たすには次の条件が 1 つだけ存在します。
(a) $A_S$ は、この加法とその乗法を合わせると、可換環になります。
(b) $\varepsilon$ は環準同型です。*

$A_S$ 満たす条件 (a) と (b) に対して加法が見つかったとします。

$x, y \in A_S$ にしましょう。 $S'$ を、$S$ によって生成された $A$ の安定乗算部分モノイドとします。 $x = a/p, y = b/q$となるような$a, b \in A$と$p, q \in S'$が存在します。それから

$$
x = \varepsilon(aq)\varepsilon(pq)^{-1}, \quad y = \varepsilon(bp)\varepsilon(pq)^{-1},
$$

よって

(23)
$$
\begin{align*}
x + y &= (\varepsilon(aq) + \varepsilon(bp))\varepsilon(pq)^{-1} \\
&= \varepsilon(aq + bp)\varepsilon(pq)^{-1} \\
&= (aq + bp)/pq.
\end{align*}
$$

これにより、加法の一意性が証明されます。

現在、*定義する* 加法、$A_S$、設定 $x + y = (aq + bp)/pq$ です。この定義が$a, b, p, q$の選択に依存していないことを示す必要があります。さて、$a', b' \in A, p', q' \in S'$ が $x = a'/p', y = b'/q'$ である場合、$S'$ には $ap's = a'ps, bq't = b'qt$、よってとなる$s$ と $t$ が存在します。

$$
(aq + bp)(p'q')(st) = (a'q' + b'p')(pq)(st)
$$

したがって

$$
(aq + bp)/pq = (a'q' + b'p')/p'q'.
$$

$A_S$ の加法が結合的かつ可換であること、$0/1$ が加法の単位元であること、$(-a)/p$ が $a/p$ の負数であること、およびすべての $x, y, z \in A_S$ について$x(y + z) = xy + xz$ であることは簡単に検証できます。 $a, b \in A$ の場合、

$$
\varepsilon(a + b) = (a + b)/1 = a/1 + b/1 = \varepsilon(a) + \varepsilon(b)
$$

したがって、$\varepsilon$ は環準同型となります。

#### 定義 8 {#alg-i-s8-def-8 .statement tag=05HX}

*定理4で定義された環は、$S$、または$S$の分母に関連付けられた分数の環と呼ばれ、$A[S^{-1}]$で表されます。

$A[S^{-1}]$の零は$0/1$、$A[S^{-1}]$の単位元は$1/1$です。

*可換代数*、章 II, § 2 の$A[S^{-1}]$ の性質に戻ります。

$S$が$A$のキャンセル可能な元の集合である場合、$A$の分数の合計環を環$A[S^{-1}]$といいます。次に、$A$ は、写像 $\varepsilon$ によって$A[S^{-1}]$ の部分環と同一視され、これは単射法になります (I, § 2, no. 4, 命題 6)。

#### 定理 5 {#alg-i-s8-thm-5 .statement tag=05HY}

*$A$を$A$の可換環、$S$部分集合、$A$の$B$環、$f$準同型を$B$にすると、すべての元が$f(S)$ は反転可能です。 $f = \bar{f} \circ \varepsilon$ となる $B$ には、$A[S^{-1}]$ の $\bar{f}$ が 1 つだけ存在します。*

私たちは (§ 2, no. 4, 定理 1) 、$f = \bar{f} \circ \varepsilon$ となるような乗法モノイド $B$ への乗法モノイド $A[S^{-1}]$ の射 $\bar{f}$ が 1 つだけ存在することを知っています。 $a, b \in A, p, q \in S'$ ($S$ によって生成される $A$ の安定乗算部分モノイド) とします。 $f(A)$ の元は対に通勤しています。
$$
\bar{f}(a/p + b/q) = \bar{f}((aq + bp)/pq) = f(aq + bp)f(pq)^{-1}
= (f(a)f(q) + f(b)f(p))f(p)^{-1}f(q)^{-1}
= f(a)f(p)^{-1} + f(b)f(q)^{-1}
= \bar{f}(a/p) + \bar{f}(b/q).
$$
したがって、$\bar{f}$ は環準同型です。

### 練習問題 {#alg-i-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
