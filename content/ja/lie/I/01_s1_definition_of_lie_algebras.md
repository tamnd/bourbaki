---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 1
section_title: Definition of Lie algebras
lang: ja
source: lie-i-iii
book_pages: 1-12, 73-83
pdf_pages: 0019-0030, 0091-0101
extraction: ocr
subsections:
    - "no": 1
      title: ALGEBRAS
      page: 1
      pdf_page: 19
    - "no": 2
      title: LIE ALGEBRAS
      page: 3
      pdf_page: 21
    - "no": 3
      title: COMMUTATIVE LIE ALGEBRAS
      page: 5
      pdf_page: 23
    - "no": 4
      title: IDEALS
      page: 5
      pdf_page: 23
    - "no": 5
      title: DERIVED SERIES, LOWER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 6
      title: UPPER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 7
      title: EXTENSIONS
      page: 7
      pdf_page: 25
    - "no": 8
      title: SEMI-DIRECT PRODUCTS
      page: 8
      pdf_page: 26
    - "no": 9
      title: CHANGE OF BASE RING
      page: 11
      pdf_page: 29
statements: 20
exercises: 27
content_sha256: f1fa284749a1957cdaafc27f4541e4a114398a73d3342e98a265d9fbf521c94f
translated_from: content/en/lie/I/01_s1_definition_of_lie_algebras.md
translation_method: google
source_content_sha256: 58f1eb6f89ce2afeeacfc62b6731300e79cd58a2c1821a7f29f1c6e2d9168f15
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 2c8a328acf51520600384bee5c2e1aba6e9b3a7b0cb7f4c64cfeaeb5de4c622c
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。 リー代数中定義

### 1. 代数

M を、M への $M \times M$ の双線形写像 $(x, y) \mapsto xy$ を持つ K 上のユニタリー 加群とします。乗法の結合性を除いて、代数のすべての公理が満たされます。言葉の乱用により、M は K に対して必ずしも結合的ではない代数、または混乱が生じない場合にはときどき、K に対して代数と呼ばれます。後者の記法を使用します。

K-加群 M を与えると乗法 $(x, y) \mapsto yx$ 代数が得られます。これは、上記の代数の逆と呼ばれます。

乗法で安定な M のサブ K 加群 N は、明らかな方法で K 上で代数の構造が与えられます。 N は M の部分代数と呼ばれます。条件 $x \in N, y \in M$ が $yx \in N$ (または $xy \in N$) を暗示する場合、N は M の左 (または右) イデアルと呼ばれます。 N が M の左イデアルと右イデアルの両方である場合、N は M の両側イデアルと呼ばれます。この場合、M 上の乗法により、移行から商までの定義する、商加群 $M/N$ 上の双線形乗法が可能になり、$M/N$ は次のようになります。 代数構造。 $M/N$ は N によって M の商代数と呼ばれます。

† この章で証明された命題は、書籍 I から VI で確立された特性と、可換代数、章 III, § 2 の特定の結果にのみ依存します。

$M_1$と$M_2$を$K$と$\phi$写像の$M_1$を$M_2$に2つ代数とします。 $\phi$ が $K$-線形の場合、$\phi$ は *準同型* と呼ばれ、$x \in M_1, y \in M_1$ の場合は $\phi(xy) = \phi(x)\phi(y)$ と呼ばれます。 The kernel $N$ of $\phi$ is a two-sided ideal of $M_1$ and the image of $\phi$ is a subalgebra of $M_2$. 移行から商、代数 $M_1/N$ の $\phi$ 定義する同型が代数 $\phi(M_1)$ に。

$M$を$K$以上の代数とします。 $M$ の $M$ への写像 $D$ は、$K$-線形で、すべての $x \in M$ と $y \in M$ に対して $D(xy) = (Dx)y + x(Dy)$ であれば、$M$ の *導分* と呼ばれます。この定義は、*代数*、章 IV, § 4, no. 3 の定義 3 を一般化します。 $M$の導分の核は、$M$の部分代数です。 $D_1$ と $D_2$ が $M$ の導分である場合、$D_1D_2 - D_2D_1$ は $M$ の導分 (cf. *代数*, 章 IV, § 4, no. 3, 命題 5: この命題の証明は、代数の結合性を使用しません)。

$M_1$ と $M_2$ を $K$ の 2 つ代数とします。 積 $K$ モジュール $M = M_1 \times M_2$ で、定義する乗法を書くことで

$$
(x_1, x_2)(y_1, y_2) = (x_1y_1, x_2y_2),
$$

$M_1$ のすべての $x_1, y_1$、$M_2$ の$x_2, y_2$。このように定義された代数は、$M_1$と$M_2$の*積代数*と呼ばれます。 写像 $x_1 \mapsto (x_1, 0)$ (それぞれ $x_2 \mapsto (0, x_2)$) は、$M$ の両面理想上で $M_1$ (それぞれ $M_2$) の同型です。これらの同型 $M_1$ と $M_2$ は、$M$ の両面の理想と同一視されます。 $K$ モジュール $M$ は、$M_1$ と $M_2$ の直和になります。逆に、$M$ を $K$ と $M_1, M_2$ の 2 つの両面理想である $M$ より上の代数とし、$M$ が $M_1$ と $M_2$ の直和となるようにします。それから$M_1M_2 \subset M_1 \cap M_2 = \{0\}$;次に、$x_1, y_1$ 属するから $M_1$ および $x_2, y_2$ から $M_2$ の場合、$(x_1 + x_2)(y_1 + y_2) = x_1y_1 + x_2y_2$ となり、$M$ は積代数 $M_1 \times M_2$ と識別されます。 $M_1$ のすべての左 (それぞれ右、両側) イデアルは、$M$ の左 (それぞれ右、両側) イデアルです。 代数の任意の有限族の場合に同様の結果を定式化する作業は読者に任せます。

$M$ を $K$ よりも代数とし、$K$ モジュール $M$ が基底 $(a_\lambda)_{\lambda \in L}$ を許容すると仮定します。 $L$ のすべての $\lambda, \mu$ に対して $a_\lambda a_\mu = \sum_v \gamma_{\lambda \mu v} a_v$ となるような、$K$ の元の固有の系 $(\gamma_{\lambda \mu \nu})_{(\lambda, \mu, \nu) \in L \times L \times L}$ が存在します。 $\gamma_{\lambda \mu \nu}$ は、基底* $(a_\lambda)$ に対する $M$ の構造の * 定数と呼ばれます。

$M$ を $K$、$K_0$ 可換環に単位元と $K_0$ の $\rho$ 準同型を加えて $K$ 写像単位元に代数とします。 単位元。すると、$\alpha \in K_0, x \in M$を$\alpha.x = \rho(\alpha).x$と書くことで、$M$は$K_0$の上の代数と考えることができます。これは特に、$K_0$ が $K$ 含む単位元の部分環であり、$\rho$ が $K_0$ の写像を $K$ に含めたものであるとみなされる場合に当てはまります。

$M$ を $K$、$K_1$ 可換環に単位元と $K$ の $\sigma$ 準同型を加えて $K_1$ 写像単位元に代数とします。 単位元。 $M_{(K_1, \sigma)} = M_{(K_1)}$ を、スカラーの環を $K_1$ (*代数*, 章 II, § 5) に拡張することによって、$M$ から導出された $K_1$ モジュールとします。 $M$ 定義する上の積は、正準的に $M_{(K_1)} \times M_{(K_1)}$ の $K_1$ 双線形写像を $M_{(K_1)}$ (*代数*, 章 IX, § 1, no. 4) に変換し、$M_{(K_1)}$ は次のようになります。 $K_1$ に対して代数の構造が与えられます (これは、スカラーの環を $K_1$ に拡張することにより、$M$ から *導出されると言われています)。これは特に、$K$ が $K_1$ 含む単位元の部分環であり、$\sigma$ が $K$ の写像を$K_1$ に含めたものである場合に当てはまります。

### 2. リー代数

#### 定義 1 {#lie-i-s1-def-1 .statement tag=09TJ}

*代数 g over K は、乗法 ($(x, y) \mapsto [x, y]$ で示される) が次の恒等式を満たす場合、リー代数 over K と呼ばれます。

(1) $$ [x, x] = 0 $$

(2) $$ [x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0 $$

*すべて* $x, y, z$ *g*。

積 $[x, y]$ は、$x$ と $y$ の * 括弧 * と呼ばれます。恒等式 (2) は、*ヤコビ恒等式*と呼ばれます。

ブラケット $[x, y]$ は、$x$ と $y$ の交代的双線形写像です。私たちはアイデンティティを持っています:

(3) $$ [x, y] = -[y, x] $$

ヤコビ恒等式を次のように書くことができます。

(4) $$ [x, [y, z]] = [[x, y], z] + [y, [x, z]]. $$

リー代数のすべての部分代数とすべての商代数はリー代数です。 リー代数のすべての積はリー代数です。 If $g$ is a Lie algebra, the opposite algebra $g^0$ is a Lie algebra and the mapping $x \mapsto -x$ an isomorphism of $g$ onto $g^0$, by virtue of identity (3).

#### 例 1 {#lie-i-s1-n2-exa-1 .statement tag=09TK}

$L$ を $K$ に対する結合代数とします。括弧 $[x, y] = xy - yx$ は、$x$ と $y$ の双線形写像です。 $K$ モジュール $L$ の合成 $(x, y) \mapsto [x, y]$ の法則により、$L$ が $K$ を超えてリー代数になることが簡単に検証されます。

#### 例 2 {#lie-i-s1-n2-exa-2 .statement tag=09TL}

例 1 選ぶ $L$ は、$K$ モジュール $E$ の自己準同型の結合代数になります。 $gl(E)$ で示される * $E$ の自己準同型の * リー代数を取得します。 ($E = K^n$の場合、リー代数 $gl(E)$は$gl(n, K)$で表されます。)

$gl(E)$ のすべての嘘部分代数は、$K$ を超えるリー代数です。 特に:
(1) $E$ に (必ずしも結合的ではない) 代数構造、$E$ 形リー代数の $K$ に対する導分が与えられた場合。
(2) $E$ が有限の基底を認める場合、零の $E$ の自己準同型は、$sl(E)$ ($E = K^n$ の場合は $sl(n, K)$) で示される $K$ 上で形リー代数を追跡します。

#### 例 3 {#lie-i-s1-n2-exa-3 .statement tag=09TM}

位数 $n$ の正方行列の集合 $M_n(K)$ は、K 上のリー代数として gl(n, K) と正準的に同型であると考えることができます。 $(E_{ij})$ を $\mathbf{M}_n(K)$ の標準基底 (代数、章 II, § 10, no. 3) とします。次のことが簡単にわかります。

$$
\begin{cases}
[E_{ij}, E_{kl}] = 0 & \text{if } j \neq k \text{ and } i \neq l \\
[E_{ij}, E_{jl}] = E_{il} & \text{if } i \neq l \\
[E_{ij}, E_{kt}] = -E_{kj} & \text{if } j \neq k \\
[E_{ij}, E_{ji}] = E_{ii} - E_{jj}
\end{cases}
$$

(5)

三角形行列の$\mathbf{M}_n(K)$からなるのライ部分代数(それぞれ零トレースの三角形行列、零対角線の三角形行列)は、$t(n, K)$(それぞれst(n, K)、それぞれ1)で表されます。 n(n, K)) (代数, 章 II, § 10; no. 7)。

*例 3. V を無限微分可能な実数多様体とします。 無限微分可能な実数係数を持つ微分演算子は、$\mathbf{R}$ 上の結合代数を構成し、したがって例 1、リー代数 $\Delta$ による $\mathbf{R}$ の結合を構成します。 The bracket of two infinitely differentiable vector fields on V is an infinitely differentiable vector field and hence the infinitely differentiable vector fields on V constitute a Lie subalgebra $\mathfrak{f}$ of $\Delta$. V が実数 *リー群* である場合、左不変式ベクトル体は、V の *リー代数* と呼ばれる $\mathfrak{f}$ の嘘部分代数 $g$ を構成します。 ベクトル空間 $g$ は、$e$ (V の単位元) で V への接線空間と識別されます。 V' を他の実リー群、$e'$ を単位元、$g'$ をリー代数とします。 V のすべての解析準同型を $e$ での接線空間から V へ、$e'$ での接線空間から V へ、V' 定義する線形写像に変換します。この写像は、リー代数$g$の準同型がリー代数$g'$になります。 V が有限次元実数ベクトル空間 E の線形群である場合、V のリー代数 $g$ 上に $gl(E)$ の標準同型が存在し、その下で $g$ は $gl(E)$ と識別されます。

#### 定義 2 {#lie-i-s1-def-2 .statement tag=09TN}

*g をリー代数とし、g の x 元とします。 g から g への線形写像 $y \mapsto [x, y]$ は、x の随伴物線形写像と呼ばれ、$\operatorname{ad}_g x$ または $\operatorname{ad} x$ で表されます。

#### 命題 1 {#lie-i-s1-prop-1 .statement tag=09TO}

※gをリー代数とします。 すべての $x \in g$ に対して、$\operatorname{ad} x$ は導分です。 The mapping $x \mapsto \operatorname{ad} x$ is a homomorphism of the Lie algebra g into the Lie algebra $\mathfrak{d}$ of derivations of g. $D \in \mathfrak{d}$ と $x \in g$ の場合、$[D, \operatorname{ad} x] = \operatorname{ad}(Dx)$。

恒等式 (4) は次のように記述できます。

$$
(\operatorname{ad} x) \cdot [y, z] = [(\operatorname{ad} x) \cdot y, z] + [y, (\operatorname{ad} x) \cdot z]
$$

または：

$$
(\operatorname{ad}[x, y]) \cdot z = (\operatorname{ad} x) \cdot ((\operatorname{ad} y) \cdot z) - (\operatorname{ad} y) \cdot ((\operatorname{ad} x) \cdot z)
$$

よって最初の 2 つ主張。一方、$D \in \mathfrak{d}$、$x \in g$、$y \in g$ の場合は、$[D, \operatorname{ad} x] \cdot y = D([x, y]) - [x, Dy] = [Dx, y] = (\operatorname{ad} Dx) \cdot y$、よって最後の主張となります。

写像 $\operatorname{ad} x$ は、$x$ によって定義される *内部導分* とも呼ばれます。

### 3. 可換リー代数

#### 定義 3 {#lie-i-s1-def-3 .statement tag=09TP}

*[x, y] = 0 の場合、リー代数の 2 つの元 x、y は置換可能であると言われます。 g は、その元のいずれか 2 つが置換可能である場合、可換であると言われます。

#### 例 1 {#lie-i-s1-n3-exa-1 .statement tag=09TQ}

L を連想代数とし、それによって定義される g リー代数 (no. 2, 例 1) とします。 2 つの元 x、y は、L で xy = yx である場合に限り、g で置換可能です。

#### 例 2 {#lie-i-s1-n3-exa-2 .statement tag=09TR}

*実リー群 G が可換であれば、そのリー代数も可換です。*

すべての K-加群には、明らかに K に対する一意の可換リー代数構造を与えることができます。

g がリー代数の場合、g のすべての単次部分加群は g の可換リー 部分代数です。

### 4. 理想

恒等式 (3) から、リー代数 g では左の理想と右の理想の間に区別はなく、すべての理想には両面があることがわかります。したがって、私たちは単に理想について話します。

#### 例 {#lie-i-s1-n4-exa-1 .statement tag=09TS}

*G をリー群、g をリー代数とし、H を G の部分群とします。H 定義する上のすべての左不変式ベクトル体は標準的に G 上の左不変式ベクトル体、よってには標準単射がありますリー代数 h を g に変換します。 h は、こ​​の単射の下にある g の Lie 部分代数と識別されます。 H が G において正規である場合、g における h の標準像は g のイデアルです。*

g の理想は部分加群の g であり、これは内部導分の g の下で安定します。

#### 定義 4 {#lie-i-s1-def-4 .statement tag=09TT}

*g のすべての導分の下で安定な g の部分加群を g の特性イデアルと呼びます。*

#### 命題 2 {#lie-i-s1-prop-2 .statement tag=09TU}

* g をリー代数とし、a を g のイデアル (それぞれ特性イデアル)、b を a の特性イデアルとします。この場合、b は g のイデアル (それぞれ特性イデアル) になります。*

g のすべての内部導分 (それぞれ導分ごと) は安定したものを残し、 導分の誘導するは安定したものを残します。

g をリー代数とします。 a と b が g のイデアルである場合、a + b と a ∩ b は g のイデアルです。

a と b を g の 2 つの部分加群とします。 形 [x, y] (x ∈ a, y ∈ b) の元によって生成された g の記法, 部分加群を [a, b] と表記します。恒等式 (3) より [a, b] = [b, a] が得られます。 z ∈ g、[z, a]、または [a, z] の場合、 は部分加群 [Kz, a] = (ad z)(a) を表します。

#### 命題 3 {#lie-i-s1-prop-3 .statement tag=09TV}

* a と b が g のイデアル (それぞれ特性イデアル) である場合、[a, b] は g のイデアル (それぞれ特性イデアル) です。*

D を g の内部導分 (それぞれ導分) とします。 $x \in a$ と $y \in b$ の場合、
$$
D([x, y]) = [Dx, y] + [x, Dy] \in [a, b].
$$
したがって命題です。

a が g の部分加群、$x \in g$ の集合で、$(\mathrm{ad}\ x).a \subset a$ が g の部分代数 n である場合、g における a の *ノーマライザー* と呼ばれます。さらに a が g の部分代数であれば、$a \subset n$ となり、a は n のイデアルになります。

### 5. 派生系列、中央下部系列

特性イデアル $[g, g]$ は、リー代数 g の*導出イデアル* と呼ばれ、$\mathscr{D}g$ で表されます。

g 含む $\mathscr{D}g$ のすべての部分加群は g のイデアルです。

The *derived series* of g is the decreasing sequence $\mathscr{D}^0g, \mathscr{D}^1g, \ldots$ of characteristic ideals of g defined inductively as follows: (1) $\mathscr{D}^0g = g$; (2) $\mathscr{D}^{p+1}g = [\mathscr{D}^pg, \mathscr{D}^pg]$.

g の *下中央系列* は、次のように帰納的に定義される g の特性イデアルの減少列 $\mathscr{C}^1g, \mathscr{C}^2g, \ldots$ です: (1) $\mathscr{C}^1g = g$; (2) $\mathscr{C}^{p+1}g = [g, \mathscr{C}^pg]$。次に、$p$ の帰納法ですぐにわかるように、すべての $p$ に対して $\mathscr{C}^2g = \mathscr{D}g$ と $\mathscr{C}^{p+1}g \supset \mathscr{D}^pg$ が続きます。

#### 命題 4 {#lie-i-s1-prop-4 .statement tag=09TW}

*g と h を K 上の 2 リー代数とし、g から h 上の f 準同型とします。次に、$f(\mathscr{D}^pg) = \mathscr{D}^pf, f(\mathscr{C}^pg) = \mathscr{C}^ph$.*

a と b が g の部分加群である場合、次のことがすぐにわかります。
$$
f([a, b]) = [f(a), f(b)].
$$
命題は、$p$ の帰納法によって明らかになります。

#### 系 {#lie-i-s1-n5-cor-1 .statement tag=09TX}

*g をリー代数とし、g のイデアルを a とします。 リー代数 $g/a$ が可換であるためには、$a \supset \mathscr{D}g$ であることが必要かつ十分です。*

$g/a$ が可換であると言うのは、$\mathscr{D}(g/a) = \{0\}$ がというになることになります。
しかし、$\mathscr{D}(g/a)$は、命題4により、$g/a$の$\mathscr{D}g$の標準像になります。

### 6. 中央上部系列

g をリー代数とし、g の P 部分集合とします。 The *centralizer* of P in g is the set of elements of g which are permutable with those of P. This centralizer is the intersection of the kernels of the ad $y$, where $y$ runs through P; it is therefore a subalgebra of g.

#### 命題 5 {#lie-i-s1-prop-5 .statement tag=09TY}

* g をリー代数とし、a を g のイデアル (それぞれ特性イデアル) とします。 g の a のセントラライザー $a'$ は、g のイデアル (特性イデアル) です。*

D を g の内部導分 (それぞれ導分) とします。 $x \in a'$ と $y \in a$ の場合、
$$
[Dx, y] = D([x, y]) - [x, Dy] = 0;
$$
したがって $Dx \in a'$ です。したがって命題です。

$g$ をリー代数とします。 $g$ の $g$ のセントラライザーは $g$ の中心と呼ばれます。これは、すべての $y \in g$ に対して $[x, y] = 0$ となるような $x \in g$ の特徴的な理想です。 $g$の中心は、準同型の$x \mapsto \mathrm{ad}\, x$の核です。

The upper central series of $g$ is the increasing sequence $\mathscr{C}_0 g, \mathscr{C}_1 g, \ldots$ of characteristic ideals of $g$ defined inductively as follows: (1) $\mathscr{C}_0 g = \{0\}$; (2) $\mathscr{C}_{p+1} g$ is the inverse image under the canonical mapping of $g$ onto $g / \mathscr{C}_p g$ of the centre of $g / \mathscr{C}_p g$
The ideal $\mathscr{C}_1 g$ is the centre of $g$.

### 7. 拡大

#### 定義 5 {#lie-i-s1-def-5 .statement tag=09TZ}

$a$ と $b$ を $K$ の 2 つリー代数とします。 $a$ による $b$ の拡大は数列です:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

where $g$ is a Lie algebra over $K$, $\mu$ a surjective homomorphism of $g$ onto $b$ and $\lambda$ an injective homomorphism of $a$ onto the kernel of $\mu$.

$\mu$の核$n$は、拡大の核と呼ばれます。 The homomorphism $\lambda$ is an isomorphism of $a$ onto $n$ and the homomorphism $\mu$ defines an isomorphism of $g / n$ onto $b$ when passing to the quotient.
By an abuse of language, $g$ is also called an extension of $b$ by $a$.

2 拡大:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b, \quad a \xrightarrow{\lambda'} g' \xrightarrow{\mu'} b
$$

are said to be equivalent if there exists a homomorphism $f$ of $g$ into $g'$ such that the following diagram:

$$
\begin{array}{ccccc}
a & \xrightarrow{\lambda} & g & \xrightarrow{\mu} & b \\
& & f \downarrow & & \\
& & g' & \xrightarrow{\mu'} & b \\
a & \xrightarrow{\lambda'} & g' & \xrightarrow{\mu'} & b
\end{array}
$$

は可換です (つまり、$f \circ \lambda = \lambda', \mu' \circ f = \mu$ になります)。このような準同型は必然的に全単射であることを示します。最初の $f$ は単射です。というのは、$x \in g$ が $f(x) = 0$ である場合、$\mu(x) = \mu'(f(x)) = 0$、したがって一部の $y \in a$ では $x = \lambda(y)$ になります。次に$\lambda'(y) = f(\lambda(y)) = f(x) = 0$、したがって$y = 0$、したがって$x = 0$となります。一方、$f$は全射です。というのは、$\mu' \circ f = \mu$ は全射法なので、$f(g) + \lambda'(a) = g'$ です。一方$f(g) \supset f(\lambda(a)) = \lambda'(a)$。

このことから、$b$ の 2 つの拡大の間で $a$ によって定義された関係は同値関係であることがわかります。

#### 命題 6 {#lie-i-s1-prop-6 .statement tag=09U0}

しましょう

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

$b$の$a$と$n$の核の拡大になります。

(a) *g の n に補足的な g の部分代数 m が存在する場合、m に対するμの制限は b に対する m の同型になります。 ν がこの制限の逆同型を表す場合、ν は b の g への準同型であり、μ ∘ ν は b の単位自己同型です*。

(b) *逆に、μ ∘ ν が b の単位自己同型となるような g の中に b の準同型 ν が存在する場合、ν(b) は g の n の補足部分代数です。

(a)の主張は明らかです。一方、μ ∘ ν が b の恒等式自己同型となるように、ν を b の g への準同型とする。このとき、ν(b) は g の部分代数であり、g は ν(b) の直和と $\mu^{-1}(0) = n$ (*代数*, 章 VIII, § 1, no. 1) です。

#### 定義 6 {#lie-i-s1-def-6 .statement tag=09U1}

*しましょう*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

* a による b の拡大と n の核になります。 g の n を補足する g の部分代数 (またはイデアル) が存在する場合、この拡大は非本質的 (または自明) と呼ばれます。 g* の中心に n が含まれる場合、この拡大を中心と呼びます。

拡大が自明な場合、m を g の n を補足する g のイデアルとします。次に、(cf. no. 1) g は、リー代数 m × n で正規に識別され、したがってリー代数 a × b と識別されます。逆に、a と b を 2 リー代数とします。その場合、a × b は a by b の自明な拡大です。

重要ではない中央の拡大は取るに足らないものです。 g をリー代数とすると、n のイデアルは g の中心に含まれ、g の m 部分代数は n in g を補足します。この場合、[m, g] = [m, m] + [m, n] = [m, m] ⊂ m となり、m は g のイデアルになります。

### 8. セミダイレクト積

a と b を K 上の 2 つのリー代数とします。a で b のすべての拡大を構成するにするのは簡単ではありません。しかし、a による b のすべての *本質的* 拡大を非常に簡単に説明しましょう。

g を a による b の非本質的な拡大とします。 g のイデアルを持つ a 同一視する、a を補足する g の部分代数を持つ b、および加群 a × b を持つ加群 g です。すべての $b \in b$ について、$\phi_b$ を $\mathrm{ad}_g\ b$ に対して制限とします。これは a の導分であり、写像 $b \mapsto \phi_b$ は b の準同型であり、a の導分のリー代数になります。一方、a の $a, a'$ と b の $b, b'$ については、次のようになります。

$$
[(a, b), (a', b')] = [a + b, a' + b']
= [a, a'] + [a, b'] + [b, a'] + [b, b']
= ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b']).
$$

逆に、a と b が K よりもリー代数であり、b の $b \mapsto \phi_b$ 準同型が a の導分のリー代数になるとします。 積 *g の K-加群* a と b では、次のように書くことで定義する 2 つの元のかっこを作成します。

$$
[(a, b), (a', b')] = ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b'])
$$

$a$の$a, a'$、$b$の$b, b'$すべて。この括弧は $(a, b), (a', b')$ の交代的双線形写像であるのは明らかです。 $a \times b$ の 3 元 $(a, b), (a', b'), (a'', b'')$ が与えられた場合、次のことがわかります。

(7)
$$
[(a, b), [(a', b'), (a'', b'')]] + [(a', b'), [(a'', b''), (a, b)]] \\
+ [(a'', b''), [(a, b), (a', b')]] = 0.
$$

(7) の左辺は $(a, b), (a', b'), (a'', b'')$ の交代的トライリニア写像であるため、この元の系が以下の形のいずれかをとれば検証すれば十分です。

(8) $(a, 0), (a', 0), (a'', 0)$

(9) $(a, 0), (a', 0), (0, b'')$

(10) $(a, 0), (0, b'), (0, b'')$

(11) $(0, b), (0, b'), (0, b'')$。

(8) と (11) の場合、関係 (7) は、$a$ と $b$ のヤコビ恒等式の明らか帰結です。ケース (9) では、

$$
[(a, 0), [(a', 0), (0, b'')]] = [(a, 0), (-\phi_{b''}a', 0)] = (-[a, \phi_{b''}a'], 0)
$$
$$
[(a', 0), [(0, b''), (a, 0)]] = [(a', 0), (\phi_{b''}a, 0)] = ([a', \phi_{b''}a], 0)
$$
$$
[(0, b''), [(a, 0), (a', 0)]] = [(0, b''), ([a, a'], 0)] = (\phi_{b''}([a, a']), 0)
$$

関係 (7) は式から次のようになります。
$$
\phi_{b''}([a, a']) = [\phi_{b''}a, a'] + [a, \phi_{b''}a'].
$$

ケース (10) の場合、次のようになります。

$$
[(a, 0), [(0, b'), (0, b'')]] = [(a, 0), (0, [b', b''])] = (-\phi_{[b', b'']}a, 0)
$$
$$
[(0, b'), [(0, b''), (a, 0)]] = [(0, b'), (\phi_{b''}a, 0)] = (\phi_{b'}\phi_{b''}a, 0)
$$
$$
[(0, b''), [(a, 0), (0, b')]] = [(0, b''), (-\phi_{b'}a, 0)] = (-\phi_{b''}\phi_{b'}a, 0)
$$

関係 (7) は式から次のようになります。
$$
\phi_{[b', b'']} = \phi_{b'}\phi_{b''} - \phi_{b''}\phi_{b'}.
$$

したがって、リー代数構造は $g$ に定義されています。 $g$の$b$上の写像$(a, b) \mapsto b$は準同型$\mu$で、その核$n$は形$(a, 0)$の$g$の元の理想です。 写像 $a \mapsto (a, 0)$ は、$a$ の同型 $\lambda$ が $n$ に加わります。 したがって、次のようになります。

(12)
$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

is an extension of $b$ by $a$ of kernel $n$, which is said to be *canonically defined by* $a, b, \phi$. The mapping $b \mapsto (0, b)$ is an isomorphism $\nu$ of $b$ onto a subalgebra of $g$ supplementary to $n$ in $g$; hence the extension is inessential.

$a$ が $\lambda$ の下で $n$ と識別され、$b$ が $v$ の下で $v(b)$ と識別される場合、$a \in a$ と $b \in b$ については次のようになります。

$$
(\mathrm{ad}\ b).a = [(0, b), (a, 0)] = (\phi_b a, 0) = \phi_b a.
$$

$\phi = 0$、$g$は、$b$と$a$の積リー代数になります。一般に、$g$ は、$a$ による $b$ の *半直接積と呼ばれます (対応するから準同型 $b$ の $b \mapsto \phi_b$ から $a$ の導分のリー代数 )。

したがって、次の命題を確立しました。

#### 命題 7 {#lie-i-s1-prop-7 .statement tag=09U2}

*$a$ と $b$ を 2 リー代数 $K$ とします。*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*本質的な$b$の拡大を$a$, $\nu$ 同型の$b$を$g$の部分代数に加え、$\mu \circ \nu$が$b$と$\phi$の同一性自己同型となる$b$ の対応する準同型を $a$ の導分のリー代数にします。* しましょう

$$
a \xrightarrow{\lambda_0} g_0 \xrightarrow{\mu_0} b
$$

*$\phi$ によって標準的に定義された $a$ による $b$ の非本質的な拡大であること。* その場合、写像 $(a, b) \mapsto \lambda(a) + \nu(b)$ は、$g$ および次の図式に対する $g_0$ の同型 $f$ となる。

$$
\begin{array}{ccccc}
& & \\
a & \xrightarrow{\lambda_0} & g_0 & \xrightarrow{\mu_0} & b \\
& \searrow f & \downarrow & \nearrow \mu_0 \\
& & g & & \\
& \swarrow i & & \searrow \mu \\
& & & &
\end{array}
$$

*は可換であるため、2 つの拡大は同等です。*

#### 例 1 {#lie-i-s1-n8-exa-1 .statement tag=09U3}

$g$ を $K$ のリー代数と、$g$ の $D$ 導分とします。 $h$ を *可換* リー代数 $K$ とします。 写像 $\lambda \mapsto \lambda D (\lambda \in K)$ は、$h$ の準同型を $g$ の導分のリー代数に変換します。私たちは $h$ から $g$ までに形対応するセミダイレクト積 $t$ です。 $x_0$ を $t$ の元 $(0, 1)$ とします。 $x \in g$、$Dx = [x_0, x]$ のすべてに。

#### 例 2 {#lie-i-s1-n8-exa-2 .statement tag=09U4}

$g$を$K$のリー代数、$M$を$K$モジュール、$g$の$\rho$準同型を$\mathfrak{gl}(M)$とします。 $M$ を可換のリー代数とみなすと、$M$ の導分のリー代数は $\mathfrak{gl}(M)$ になります。したがって、$g$ の半直接積 $h$ を $M$ 対応するから $\rho$ まで形することができます。

特に、$g = \mathfrak{gl}(M)$と$\rho$を$\mathfrak{gl}(M)$の恒等写像とします。 $M$ による $g$ の半直接積は、$\mathfrak{af}(M)$ ($M = K^n$ の場合は $\mathfrak{af}(n, K)$) で表されます。 $\mathfrak{af}(M)$ の元は、対 $(m, u)$ の順序です。ここで、$m \in M, u \in \mathfrak{gl}(M)$;そして括弧は次のように定義されます

$$
[(m, u), (m', u')] = (u(m') - u'(m), [u, u']).
$$

*M が $\mathbf{R}$ を上回る有限次元ベクトル空間である場合、$\mathfrak{af}(M)$ は M の *アフィン群* のリー代数と正規識別されます。

$t$ を K 上のリー代数とします。線形写像 $t$ の $\theta$ を $\mathfrak{af}(M)$ に書き込むと、$x \mapsto ((\zeta(x), \eta(x)))$ と書くことができます。ここで、$\zeta$ は、$M$ と $\eta$ に$t$ の線形写像です。 $t$の線形写像が$gl(M)$に。 条件を調べると、$\theta$ が準同型になるためには、$\zeta$ と $\eta$ は満たすでなければならないことがわかります。 $x \in t, y \in t$ については、

$$
\theta([x, y]) = [\theta(x), \theta(y)]
$$

つまり

$$
(\zeta([x, y]), \eta([x, y])) = [(\zeta(x), \eta(x)), (\zeta(y), \eta(y))] \\
= (\eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x), [\eta(x), \eta(y)]).
$$

したがって、$\theta$が$t$の準同型から$\mathfrak{af}(M)$になるには、$\eta$が$t$の準同型から$gl(M)$になり、$\zeta$満たすになることが必要かつ十分です。 関係:

(13)
$$
\zeta([x, y]) = \eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x).
$$

N を K-加群 $M \times K$ とします。 $t$ を $w \in gl(N)$ の $gl(N)$ からなるの部分代数として$w(N) \subset M$ とします。すべての$w \in t$について、$\eta(w) \in gl(M)$を$w$から$M$の制限とし、$\zeta(w) = w(0, 1) \in M$とします。 $w_1 \in t, w_2 \in t$の場合、

$$
\zeta([w_1, w_2]) = w_1(\zeta(w_2)) - w_2(\zeta(w_1)) = \eta(w_1) \cdot \zeta(w_2) - \eta(w_2) \cdot \zeta(w_1).
$$

したがって、写像 $w \mapsto (\zeta(w)), \eta(w))$ は、$t$ の準同型 $\theta$ が $\mathfrak{af}(M)$ になります。明らかに $\theta$ は *全客観* です。 $\phi = \theta^{-1}$ にしましょう。 $(m, u) \in \mathfrak{af}(M)$ の場合、$\phi(m, u)$ は、次のように定義される $t$ の元 $w$ です。

$$
w(m', \lambda) = (u(m') + \lambda m, 0).
$$

$\mathfrak{af}(M)$ は、同型 $\phi$ の下の $gl(N)$ の部分代数 $t$ と識別されることがよくあります。

*Mが有限次元ベクトル空間が$\mathbf{R}$を超えている場合、アフィンの準同型$\mathfrak{af}(M)$の$\phi$が$gl(N)$に、対応するが標準準同型に$\psi$、Mの群Aが群に$\mathbf{GL}(N)$; $a \in A, \psi(a)$ が $\mathbf{GL}(N)$ の一意元 $g$ である場合、すべての $m \in M$ に対して $g(m, 1) = (a(m), 1)$ になります。この準同型は単射であり、 $\psi(A)$ は N の自己同型の集合であり、M に平行な N のすべての線形多様体が不変のままになります。*

### 9. 変更/基底環

$K_0$を可換環と$K_0$の単位元と$\rho$準同型をK写像単位元から単位元とします。 $g$ を K 上のリー代数とします。 $g'$ を、$g$ を $K_0$ 上の代数として、$\rho$ (cf. no. 1) によって得られる代数とします。すると$g'$はリー代数になります。 $g$ の部分代数 (それぞれの理想) は、$g'$ の部分代数 (それぞれの理想) です。 $a$ と $b$ が $g$ の部分加群である場合、括弧 $[a, b]$ は $g$ と $g'$ で同じです。 $[a, b]$ は形の元の集合です

$$
\sum_{i=1}^n [x_i, y_i]
$$

$x_i \in a, y_i \in b$ です。すべての $p$ に対して $\mathscr{D}^p g = \mathscr{D}^p g', \mathscr{C}^p g = \mathscr{C}^p g'$ ということになります。

部分集合のセントラライザーは、$g$ と $g'$ で同じです。したがって、すべての $p$ に対して $\mathscr{C}_p g = \mathscr{C}_p g'$ となります。

$K_1$を可換環とし、$K$の単位元と$\sigma$準同型を$K_1$写像単位元から単位元とします。 $g$を$K$以上のリー代数とします。 基底環 (cf. no. 1) を拡張して、$g$ から導出された $K_1$ を $g_{(K_1)}$ が代数とします。すると、$g_{(K_1)}$はリー代数になります。 $a$が$g$の部分代数（それぞれ理想）である場合、$g_{(K_1)}$の$a_{(K_1)}$の標準像は$g_{(K_1)}$の部分代数（それぞれ理想）です。 $a$と$b$が$g$の部分加群である場合、$[a, b]_{(K_1)}$の$g_{(K_1)}$の標準像は$a_{(K_1)}$と$b_{(K_1)}$の標準像のかっこに等しい。したがって、$\mathscr{D}^p(g_{(K_1)})$ は $(\mathscr{D}^p g)_{(K_1)}$ の標準像であり、$\mathscr{C}^p(g_{(K_1)})$ は $\mathscr{C}^p(g_{(K_1)})$ の標準像であることがわかります。

$K$ が体、$K$ の $K_1$ 拡大体、および $K$ の $\sigma$ 標準単射が $K_1$ になる場合、通常の識別を使用すると、次のようになります。
$$
[a, b]_{(K_1)} = [a_{(K_1)}, b_{(K_1)}], \quad \mathscr{D}^p(g_{(K_1)}) = (\mathscr{D}^p g)_{(K_1)},
$$
$$
\mathscr{C}^p(g_{(K_1)}) = (\mathscr{C}^p g)_{(K_1)}.
$$

これらの結果は§ 2, no. 9で完了します。

$M$ が体 $K$ よりも有限次元ベクトル空間である場合、$M_{(K_1)}$ は $K_1$ よりも有限次元ベクトル空間であり、結合代数 $\mathscr{L}(M_{(K_1)})$ は結合代数と標準的に識別されます。 $\mathscr{L}(M)_{(K_1)}$。したがって、リー代数 $gl(M_{(K_1)})$ は正規的にリー代数 $gl(M)_{(K_1)}$ と識別されます。

### 練習問題 {#lie-i-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
