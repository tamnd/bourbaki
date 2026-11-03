---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 0
section_title: Fixed points of groups of affine transformations
appendix: true
lang: ja
source: evt-i-v
pdf_pages: 0221-0229, 0254-0258
extraction: ocr
subsections:
    - "no": 1
      title: The case of solvable groups
      page: 0
      pdf_page: 221
    - "no": 2
      title: Invariant means
      page: 40
      pdf_page: 222
    - "no": 3
      title: Ryll-Nardzewski theorem
      page: 41
      pdf_page: 223
    - "no": 4
      title: Applications.
      page: 44
      pdf_page: 226
statements: 10
exercises: 8
content_sha256: 87cd693d89cd83980cc753327f931171839023ca6d60ec90cada574cab7e48c8
translated_from: content/en/evt/IV/A_a_fixed_points_of_groups_of_affine.md
translation_method: google
source_content_sha256: a3148232ea5c844b272b5847081786d07ced849332b19697c848a4c2a2b6e871
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 29aa0f4b4877af8c34aaa753621a5468eb4787b8b8976f231c8e167385ddee0c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録
# アフィン変換の群の点を修正

### 1. 解決可能な場合群

E を実数ベクトル空間、K を E の凸部分集合とします。 写像 $u : K \to K$ として、K の $x, y$ と $[0, 1]$ のすべての実数 $t$ について、次のようになります。

$$
u(t x + (1 - t) y) = t u(x) + (1 - t) u(y)
$$

をアフィン変換と言います。 関係 (1) から、次のように推測されます。

$$
u \left( \sum_{i \in I} t_i x_i \right) = \sum_{i \in I} t_i u(x_i)
$$

K のすべての有限集合 I、点 $x_i$ と、$\sum_{i \in I} t_i = 1$ となるような正の実数 $t_i$ に対して。

$u$ と $v$ を K 上の 2 つのアフィン変換とすると、写像 $u \circ v$ は K 上のアフィン変換です。 $v : E \to E$ が線形写像で、$v(K) \subset K$、写像 $u : K \to K$ が一致するになるとします。 K 上の $v$ はアフィン変換です。

#### 定理 1 (マルコフ-角谷) {#evt-iv-a0-thm-1 .statement tag=07WI}

— *E を体 $\mathbf{R}$ 上のハウスドルフ局所凸ベクトル空間とし、K を E の空でないコンパクト凸部分集合とします。 $\Gamma$ を K 上の連続アフィン変換の集合とし、ペアごとに置換可能とします。すると、すべての $u \in \Gamma$ に対して $u(a) = a$ となるような K に点 a が存在します。

すべての $u \in \Gamma$ について、$K_u$ をすべての $x \in K$ の集合とし、$u(x) = x$ とします。 $K_u$ が空ではないことを示します。 $x$ を K の点とします。すべての整数 $n \geq 1$ について、$x_n$ を E の元 $\frac{1}{n} \sum_{i=0}^{n-1} u^i(x)$ とします。K は、K に対して $u$、点 $x_n$ 属するの下で凸で安定しており、K がコンパクトであるため、 極限点 $a$/数列 $(x_n)_{n \geq 1}$。 K から E への写像 $y \mapsto u(y) - y$ は連続なので、$u(a) - a$ は数列 $(u(x_n) - x_n)_{n \geq 1}$ の極限点です。しかし、私たちには$u(x_n) - x_n = \frac{1}{n} (u^n(x) - x)$があります。

K はコンパクトであるため、有界 (III、p. 3、提案 2) もあり、数列 $(u^n(x) - x)_{n \geq 1}$ は有界です。その結果、数列 $\left( \frac{1}{n}(u^n(x) - x) \right)_{n \geq 1}$ は 0 になる傾向があり (III, p. 4、提案 3)、E はハウスドルフであるため、$u(a) - a = 0$ になります。従って$a \in K_u$。

それぞれの集合 $K_u$ は、コンパクト空間 K の閉じた凸型部分集合であり、共通部分 $\bigcap_{u \in \Gamma} K_u$ が空ではないことを証明します。このためには、$n \geq 1$ と $\Gamma$ の $u_1, ..., u_n$ について、集合 $K_{u_1} \cap ... \cap K_{u_n}$ が空ではないことを証明するだけで十分です。 $n = 1$ のケースを検討したので、$n$ について帰納法で議論します。 $n \geq 2$とすると、$L = K_{u_1} \cap ... \cap K_{u_{n-1}}$を入れます。 帰納法の仮定により、LはEの空でないコンパクト凸部分集合になります。$u_n$は$u_1, ..., u_{n-1}$と可換なので、$u_n(L) \subset L$が得られます。 適用証明の最初の部分を L で $u_n$ によって引き起こされるアフィン変換にすると、 L には $u_n(a) = a$ となる点 $a$ が存在すると結論する。次に、$a$ 属するから $K_{u_1} \cap ... \cap K_{u_n}$ となり、空ではなくなります。

#### 系 {#evt-iv-a0-n1-cor-1 .statement tag=07WJ}

— *G を K 上の連続アフィン変換の可解な群とします。その場合、K には G の下で不変である点が存在します。

可解な群 (A, I, § 6, No. 4) の定義により、$G_0 = G$、$G_n = \{e\}$ など、群 $G_{i-1}/G_i$ が *可換* であるような、G の別個の部分群の有限減少列 $(G_i)_{0 \leq i \leq n}$ が存在します。 $1 \leq i \leq n$。 $K_i$ が K の $G_i$ の固定点の集合を表すものとします。 次に$K_n = K$。 さらに、$1 \leq i \leq n$ については、$G_i$ 誘導するの元ごとに $K_i$ で恒等変換が行われます。従って、$K_i$ が空でない場合、K でアーベル群 $G_{i-1}/G_i$ の作用を推定します。それは th から続きます。 $K_i$の$G_{i-1}/G_i$の固定点の集合$K_{i-1}$が空ではないこと。 $i$ で帰納法を下降すると、$K_0$ が空ではないことが結論するわかり、したがって系になります。

### 2. 不変の意味

X をトポロジー 空間とします。 $\mathscr{B}(X; \mathbf{R})$ は、X から $\mathbf{R}$ までの連続有界写像の実数ベクトル空間からなるを表すものとします。 ノルム $\|f\| = \sup_{x \in X} |f(x)|$ を備えたこれは、Banach 空間 (GT、X, § 3, No. 1) です。また、順序付けられたベクトル空間です。ここで、関係 $f \geq g$ は、«すべての $x \in X$ に対して$f(x) \geq g(x)$» を意味します。

#### 定義 1 {#evt-iv-a0-def-1 .statement tag=07WK}

*空間 $\mathscr{B}(X; \mathbf{R})$ で正の線型形式 $\mu$、ここで X は位相幾何学空間であり、$\|\mu\| = 1$ は X の平均と呼ばれます。*

\* X がコンパクトな場合、X の平均は $\mu(X) = 1$ など、X の正の測度になります。 \*

#### 補題 1 {#evt-iv-a0-lem-1 .statement tag=07WL}

*X の意味の集合 K は、バナッハ空間 $E = \mathscr{B}(X; \mathbf{R})$ の元が線型形式 $\mu$ である$\mu(1) = 1$ の双対の単位元ボールの部分集合です。 $\sigma(E', E)$の凸でコンパクトな$E'$の部分集合です*。

$\mu$ を E 上の線型形式として、$\mu(1) = 1$ とします。 写像 $f \in E$ ごとに、定義する写像 $f' \in E$ を $f'(x) = \|f\| - f(x)$ ($x \in X$) とします。まず、$\mu$ が平均であると仮定します。 $f \in E$ ごとに $f' \geq 0$ があり、従って $\mu(f') \geq 0$、*つまり* $\mu(f) \leq \|f\|$ になります。従って$\|\mu\| \leq 1$。

逆に、$\mu$ 属するが $E'$ になり、$\| \mu \| \leq 1$ になるとします。正の写像 $f \in E$ ごとに、$\mu(f') \leq \| f' \|$ が得られます。

$$
\| f \| - \mu(f) = \mu(f') \leq \| f' \| \leq \| f \|,
$$

そして最後に$\mu(f) \geq 0$;従って、$\mu$ は平均値です。

$K$ が凸であることは明らかです。 $\sigma(E', E)$ についてはコンパクトであることが cor からわかります。 III、p. 17 の 3 つ。

Q.E.D.

$\Gamma$ を $X$ から $X$ までペアで交換する連続写像の集合とします。 $\gamma \in \Gamma$ にしましょう。 写像 $f \in E$ ごとに、$f \circ \gamma \in E$ が得られます。したがって、$X$ 上の平均の定義する集合 $K$ に対するアフィン変換 $u_{\gamma}$ ができます。

$$
u_{\gamma} \mu(f) = \mu(f \circ \gamma) \quad (\mu \in K, f \in E).
$$

$\sigma(E', E)$ によって$K$ に位相が割り当てられた場合、写像 $u_{\gamma}$ は連続です。 $\gamma$ が同型写像である場合、$\mu$ から構造の輸送によって $u_{\gamma} \mu$ を演繹できます。最後に、$\Gamma$ のすべての $\gamma, \gamma'$ に対して $u_{\gamma} u_{\gamma'} = u_{\gamma' \gamma} u_{\gamma}$ ができました。マルコフ・カクタニ著。 (IV, p. 39, th. 1)、*$X$ には平均 $\mu$ が存在し、すべての $\gamma \in \Gamma$ に対して $u_{\gamma} \mu = \mu$ となります。その他の語* では、$\mu$ は $f \in E$ と $\gamma \in \Gamma$ に対して関係 $\mu(f) = \mu(f \circ \gamma)$ を満たします。

同様に、系も同様です。 1 (IV, p. 40) は次の結果を意味します。

#### 命題 1 {#evt-iv-a0-prop-1 .statement tag=07WM}

*$X$をトポロジカルな空間、$G$を可溶な群とする。すべての $g \in G$、$X$ から $X$ までの写像 $x \mapsto g.x$ が連続するように、$G$ が左側の $X$ で動作すると仮定します。次に、$X$ には、$G$ の下で不変となる平均が存在します。

#### 系 {#evt-iv-a0-n2-cor-1 .statement tag=07WN}

*$G$を可解な位相幾何学的群とする。次に、$G$ には、左と右の変換の下で不変の平均が存在します。*

プロップを適用するだけで十分です。 1 から $(g.g').x = {gxg'}^{-1}$ によって $G$ に作用する、解ける群 $G \times G$ になります。

### 3. リル・ナルシェフスキー 定理

この切断において、$E$ は、体 $\mathbf{R}$ と $\mathscr{T}$ 上のノルム *空間* を表し、$E$ に局所的に凸なハウスドルフ位相を表し、$E$ のノルムは*下部半連続*。これらの仮説は、特に次の場合に満たされます。

a) $\mathscr{T}$ は、標準値空間 $E$ のノルムによって引き起こされた位相です。
b) $\mathscr{T}$ は、標準の空間 $E$ を弱めた位相 $\sigma(E, E')$ です。
c) $E$ は、標準の空間 $F$ と $\mathscr{T} = \sigma(F', F)$ の双数です。
d) $E = \mathscr{L}(F_1 ; F_2)$ と $\mathscr{T}$ が単純収束の位相となるような 2 つの正規化空間 $F_1$ と $F_2$ が存在します。

*〜でない限り明示的に記載されている場合、トポロジカル概念は位相 $\mathscr{T}$ を指します。*

$K$を$E$の凸部分集合とします。 $K$ が (位相 $\mathscr{T}$ に対して) コンパクトで、$K$ が $E$ のノルムによって定義される距離に対する可算性の最初の公理を満たすとします。

#### 補題 2 {#evt-iv-a0-lem-2 .statement tag=07WO}

$K$ 含むが少なくとも 2 つの点であるとします。すべての $\varepsilon > 0$ に対して、2 つの空ではない部分集合 $K_1$ および $K_2$ に $K$ の分割が存在し、次のプロパティがあります。

a) $K_1$ は凸状でコンパクトです。
b) $K_2$ の $x_1$ と $x_2$ ごとに $\| x_1 - x_2 \| < \varepsilon$ があります。

$L$ を、$K$ のすべての極値点の集合の閉包とします。クライン・ミルマン著。 (II, p. 55, th. 1)、$K$ は $L$ の閉じた凸包絡線です。 $K$ 含むは少なくとも 2 つの点なので、$L$ も同様です。すべての $x \in L$ について、$A_x$ をすべての $y \in L$ の集合とし、$\| x - y \| \leq \varepsilon / 4$ とします。 $K$ の仮定までに、$L$ のうち $L = \bigcup_{x \in D} A_x$ となる可算な部分集合 $D$ が存在します。 ノルムは下位半連続なので、集合$A_x$はそれぞれクローズです。 適用バイレの 3 番目。 (GT, IX, § 5, No. 3, th. 1) コンパクト空間 $L$ に対して、$D$ には点 $a$ が存在し、$E$ にはオープン部分集合 $U$ が存在し、$L \cap U$ は次のようになります。空ではなく、$A_a$ に含まれています。 $L$ 含む少なくとも 2 つの点があり、$E$ はハウスドルフであるため、$L \notin U$ になるように選ぶ $U$ ができます。

$M$ を $L \cap \complement U$ の閉じた凸包絡線とします。 $0 < t < 1$ となるすべての実数 $t$ について、$x_1 \in M$ と $x_2 \in K$ を含む形 $tx_1 + (1 - t) x_2$ のすべてのベクトルの集合を$M_t$ とします。これは空ではなく、$K$のコンパクトな凸部分集合です。 $M_t \neq K$ を不合理な還元によって証明します。 $M_t = K$; と仮定します。 $K$ 属するから $M_t$ のすべての極値点 $x$ は、$x_1 \in M$ と $x_2 \in K$ を使用して形 $x = tx_1 + (1 - t) x_2$ に書き込むことができます。これは、$x = x_1 = x_2$、つまり $x \in M$ を意味します。クライン・ミルマン著(II, p. 55, th. 1)、$K = M$ があり、$K$ は$L \cap \complement U$ の閉じた凸包絡線です。 II、p. 56、系により、これは $L \subset L \cap \complement U$、つまり矛盾する関係 $L \cap U \neq \varnothing$ を意味します。

$d = \sup_{x \in K, y \in K} \| x - y \|$ と選ぶ実数 $t$ を$0 < t < 1$ と $t < \varepsilon / 4d$ になるように置きます。 $K_1 = M_t$と$K_2 = K - M_t$を入れます。前の引数により、集合 $K_1$ と $K_2$ は空ではなく、$K_1$ は凸でコンパクトです。 $M'$ を $L \cap U$ の閉じた凸包絡線とします。 $K$ は集合 $L = (L \cap \complement U) \cup (L \cap U)$ の閉じた凸包絡線であるため、$M \cup M'$ の閉じた凸包絡線でもあります。 $x_1$ と $x_2$ を $K_2$ の 2 つの点とします。 $i = 1, 2$ には、$0 \leq \alpha_i \leq 1$ と $x_i = \alpha_i y_i + (1 - \alpha_i) z_i$ のように、$y_i \in M$、$z_i \in M'$、実数 $\alpha_i$ が存在します。 $\alpha_i \geq t$ の場合、
$$
x_i = t y_i + (1 - t) \left\{ \frac{\alpha_i - t}{1 - t} y_i + \frac{1 - \alpha_i}{1 - t} z_i \right\}
$$
;これ矛盾する仮定それ $x_i \notin M_i$。したがって、$\alpha_i < t$、$i = 1, 2$ などとなります。
$$
\| x_i - z_i \| = \| \alpha_i (y_i - z_i) \| = \alpha_i \| y_i - z_i \| \leq \alpha_i d < dt < \varepsilon / 4 .
$$
$M'$ のすべての点 $z$ には、$L \cap U \subset A_a$ 以降、$\| z - a \| \leq \varepsilon / 4$ があり、特に $\| z_i - a \| \leq \varepsilon / 4$ になります。したがって、
$$
\| x_1 - x_2 \| \leq \sum_{i=1}^2 (\| x_i - z_i \| + \| z_i - a \|) < \varepsilon .
$$
これで証明は完了です。

#### 補題 3 {#evt-iv-a0-lem-3 .statement tag=07WP}

G を K 上の連続 ($\mathscr{T}$ の) アフィン変換の群とします。K が空ではなく、K のすべての x、y と G のすべての g に対して $\|gx - gy\| = \|x - y\|$ であるとします。その場合、K には G のもとで不変である点が存在します。

$\mathfrak{J}$ を、閉じた凸で G に対して安定な K の空でない部分集合の族とします。 $(L_\alpha)_{\alpha \in I}$ が包含によって完全に順序付けされた $\mathfrak{J}$ の元の族である場合、集合 $L = \bigcap_{\alpha \in I} L_\alpha$ 属するから $\mathfrak{J}$ になります。その結果 (S, III, § 3, No. 4, th. 2)、$\mathfrak{J}$ には関係の包含に対して最小である元 L が存在します。 L 簡約するから点を証明します。

L 含む少なくとも 2 つの異なる点 $x_1$ と $x_2$ を仮定して、$x = (x_1 + x_2)/2$ と $\varepsilon = \|x_1 - x_2\|/2$ を置くという不合理な還元によって議論します。凸型でコンパクトな集合 L は、ノルム (GT, IX, § 2, No. 8) で定義される距離の可算性の最初の公理を満たします。従って、補題 2 を適用すると、$\varnothing$ や L とは異なり、次の性質を持つ、L のコンパクトで凸の部分集合 $L_1$ を見つけることができます。

(A) *$L - L_1$ の $y_1$ と $y_2$ ごとに、$\|y_1 - y_2\| < \varepsilon$ があります。*

*すべての $g \in G$ に対して $gx \in L_1$ であることを、不合理な還元によって証明します。* $g \in G$ を $gx \in L - L_1$ とすると、次のようになります。

$$
\|gx_i - gx\| = \|x_i - x\| = \|x_1 - x_2\|/2 = \varepsilon ,
$$

$i = 1, 2$の場合。 性質 (A) までに、$gx_i \in L_1$ になります。 $L_1$は凸なので、$gx = (gx_1 + gx_2)/2$属するを$L_1$に結論するし、矛盾する仮定となります。

$L'$ を x の軌道 $Gx$ の閉じた凸包絡線とします。 集合 $L'$ 属するから $\mathfrak{J}$前の議論により、$L' \subset L_1$ が得られるため、$L' \subset L, L' \neq L$ となります。この矛盾する、Lと証明の最小限の指標が完成しました。

#### 定理 2 (リル・ナルシェフスキー) {#evt-iv-a0-thm-2 .statement tag=07WQ}

— *E をノルム空間 、K を E の空でない凸型部分集合とします。これは、弱体化した位相 $\sigma(E, E')$ にとってコンパクトです。 G を K の等尺性アフィン変換の群とします。そのとき、G の下で不変である K には点が存在します。

すべての $g \in G$ について、$K_g$ が $gx = x$ となるような K のすべての点 x の集合を表すものとします。 K に弱体化した位相を割り当てます。それぞれの集合 $K_g$ は凸であり、コンパクトな空間 K 内で閉じています。 共通部分 $\bigcap_{g \in G} K_g$ が空ではないことを証明します。このためには、G のすべての $g_1, ..., g_n$ に対して集合 $K_{g_1} \cap ... \cap K_{g_n}$ が空ではないことを証明するだけで十分です。 $g_1, ..., g_n$ を修正し、H を $\{ g_1, ..., g_n \}$ によって生成された G の部分群とします。 K の選ぶ点 a を、a の軌道 Ha の閉じた凸包絡線を L で表します。 D を、形 $\lambda_1 h_1 a + \cdots + \lambda_m h_m a$ の元の可算集合とします。ここで、$\lambda_1, ..., \lambda_m$ は、H で $\lambda_1 + \cdots + \lambda_m = 1$ と $h_1, ..., h_m$ が元となるような正の有理数数です。強い位相のDの$\overline{D}$は凸であるため、$\sigma(E, E')$については閉じられています（IV、p. 4、提案2）。従って $\overline{D} = L$ となり、これは L が距離 $(x, y) \mapsto \|x - y\|$ の可算性の最初の公理である計量空間満たすであることを証明します。ここで、補題 2 を適用できます。L には、H の下で不変である点 b が存在します。従って、$b \in K_{g_1} \cap ... \cap K_{g_n}$ になります。

#### 系 {#evt-iv-a0-n3-cor-1 .statement tag=07WR}

— E を再帰バナッハ空間、規範化された空間 E の自己同型の G 群、E の K 部分集合とする。K が空ではなく、凸で、閉じていて、有界であり、G のもとで安定していると仮定する。そのとき、K には不変である点が存在する。 Gの下で

E は再帰的であるため、K は $\sigma(E, E')$ (IV, p. 15, th. 1) に対してコンパクトです。また、G属する～$\mathscr{L}(E)$の各元。

### 4. アプリケーション。

\* A) ユニタリ表現の群 :
E を複素ヒルベルト空間、G 群、および $\pi$ を E 上の G のユニタリー 表現、つまり準同型を G から E の自己同型の群とする。$E^G$ を$\pi(G)$ の下ですべてのベクトルの E からなるのヒルバーティアン部分空間は不変です。すべての $x \in E$ について、$K_x$ を x の軌道の閉じた凸包絡線とします。 Eの点 xを修正します。

$\pi(G)$ の下で不変である一意の点が $K_x$ に存在すること、つまり $E^G$ 上の x の射影が存在することを示します。 IV、p. 44、系 (基礎となる実数ベクトル空間から E に適用) により、$\pi(G)$ の下で不変である $K_x$ には点が存在します。 点のようにしましょう。次に$a \in E^G$。 P を、$y - x$ が $E^G$ に直交するように、すべての $y \in E$ の集合とします。 P が $\pi(G)$ の下で閉じており、凸であり、不変であることがすぐにわかります。従って$x \in P$、従って$K_x \subset P$、そして最後に$a \in P$です。他の語では、$a - x$は$E^G$と直交します。従って、a は x の $E^G$ に対する射影になります。 \*

\* B) ヒルバーシアン内の演算子のトレース空間 :
表現 $\pi$ が既約であると仮定します。つまり、$\{0\}$ や $\pi(G)$ で不変である E とは異なり、E のヒルバーシアン部分空間が存在しないとします。 $F = \mathscr{L}^2(E)$ を E のすべてのヒルベルト・シュミット自己準同型のヒルベルト空間とし、スカラー 積 $\langle u|v \rangle = \operatorname{Tr}(u^*v)$ とします。私たちは定義する統一体表現 $\lambda$ 公式によって G から F へ

$$
\lambda(g).u = \pi(g)\ u\pi(g)^{-1} \quad (u \in F,\ g \in G)
$$

$\lambda(G)$ の下での E の不変式すべての元の空間 $F^G$ は、すべての $g \in G$ について $\pi(g)$ と可換である E のヒルベルト・シュミット自己準同型 $u$ から構成されます。 シュールの補題によれば、そのような$u$はホモテティーになります。 従って、次の 2 つのケースを考慮する必要があります。
1) E が無限次元の場合、$F^G = \{0\}$;
2) E が有限次元の場合、$F = \mathscr{L}(E)$ と $F^G = \mathbf{C}.1_E$。

適用 A) の結果をユニタリ表現 $\lambda$ にすると、次の定理が得られます。

$u \in \mathscr{L}^2(E)$ とし、$A_u$ を E の自己準同型 $\pi(g)\ u\pi(g)^{-1}$ の集合の$\mathscr{L}^2(E)$ の閉じた凸包絡線とします。ここで、g は G を通過します。E が無限次元の場合、$0 \in A_u$ が得られます。 E が次元 d で有限次元である場合、$A_u$ には一意のホモテティー、つまり、$\mathscr{L}^2(E)$ の部分空間 $\mathbf{C}.1_E$ 上に u の射影 $\frac{1}{d}\ \operatorname{Tr}(u).\ 1_E$ が存在します。 \*

C) コンパクト群のハール測定:

G をコンパクト群とし、E = $\mathscr{C}(G, \mathbf{R})$ を G 上のすべての実数値連続写像のバナッハ空間とし、ノルムを付与します。

$$
\| f \| = \sup_{x \in G} |f(x)| .
$$

すべての $x \in G$ に対して、E の定義する自己同型 $\gamma_x$ と $\delta_x$ を公式で計算します。

$$
\gamma_x f(y) = f(x^{-1}y) , \quad \delta_x f(y) = f(yx)
$$

($y \in G,\ f \in E$の場合)。

*$f \in E$、$\Gamma_f$ (それぞれ $\Delta_f$) が閉じた凸包絡線 i を表すものとします。 x が G を超える範囲にあるとき、すべての写像 $\gamma_x f$ (それぞれ $\delta_x f$) のうちの集合の E。一意の定数写像 $\mu(f)$ 所属から $\Gamma_f$、一意の定数写像 $\mu'(f)$ が存在することを証明します。 所属から $\Delta_f$ であり、これらの定数が等しいこと。*

G 上の連続写像は、それが定数である場合に限り、E の自己同型 $\gamma_x$ (それぞれ $\delta_x$) の下で不変であることは明らかです。ここで、G の x に対するすべての写像 $\gamma_x f$ (それぞれ $\delta_x f$) のうちの集合は、G から E への写像 $x \mapsto \gamma_x f$ (それぞれ $x \mapsto \delta_x f$) が連続であるため、E ではコンパクトです (GT, X, § 3, No. 4, th. 3)。 (II, p. 25、提案 3) $\Gamma_f$ (それぞれ $\Delta_f$) は、ノルムによって定義される位相に対する E のコンパクト集合であり、したがって $\sigma(E, E')$ に対するものになります。 Ryll-Nardzewski 著(IV、p. 43、th.2)、$\Gamma_f$と$\Delta_f$には定数写像が存在します。 $c_1 \in \Gamma_f$ と $c_2 \in \Delta_f$ が定数であれば、$c_1 = c_2$ であることを証明する必要があります。

$\varepsilon > 0$ にしましょう。 仮定までに、G には点 $x_1, ..., x_n,\ y_1, ..., y_n$ が存在し、正の実数 $\lambda_1, ..., \lambda_n,\ \mu_1, ..., \mu_m$ は次のようになります。

$$
\lambda_1 + \cdots + \lambda_n = \mu_1 + \cdots + \mu_m = 1 .
$$
$$
\sup_{x \in G} \left| \sum_{i=1}^n \lambda_i f(x_i x) - c_1 \right| \leq \varepsilon ,
$$
$$
\sup_{x \in G} \left| \sum_{j=1}^m \mu_j f(xy_j) - c_2 \right| \leq \varepsilon .
$$

$r = \sum_{i,j} \lambda_i \mu_j f(x_i y_j)$を入れてください。次に、$r - c_1 = \sum_{j=1}^m \mu_j a_j$ と $a_j = \sum_{i=1}^n \lambda_i f(x_i y_j) - c_1$。 (7) により、$1 \leq j \leq m$ に対して $|a_j| \leq \varepsilon$ が得られ、したがって $|r - c_1| \leq \varepsilon$ になります。同様に、不等式 $|r - c_2| \leq \varepsilon$ であるため、$|c_1 - c_2| \leq 2\varepsilon$ を証明します。 $\varepsilon$ は任意なので、アサートされたように $c_1 = c_2$ が得られます。

$\mu(f)$の定義により、すべての$\varepsilon > 0$に対して、和 1と元 $x_1, ..., x_n$を含む正の数 $\lambda_1, ..., \lambda_n$をGで見つけることができ、すべての$x \in G$に対して$\left| \sum_{i=1}^n \lambda_i f(x_i x) - \mu(f) \right| \leq \varepsilon$が得られます。

E の $f, g$ とすべてのスカラー $\lambda$ に対して、$\Gamma_{f+g} \subset \Gamma_f + \Gamma_g$ と $\Gamma_{\gamma f} = \lambda \Gamma_f$ があり、したがって関係 $\mu(f+g) = \mu(f) + \mu(g)$ と $\mu(\lambda f) = \lambda \mu(f)$ が得られるのは明らかです。したがって、E から $\mathbf{R}$ への写像 $\mu : f \mapsto \mu(f)$ は、コンパクト空間 G (IV, p. 40) の平均です。 *その他の語 $\mu$ は、$\mu(G) = 1$* などの G の正の尺度です。

$\mu$ が $G$ の左翻訳の下で不変であることは明らかであり、等式 $\mu(f) = \mu'(f)$ は、$\mu$ が右翻訳の下でも不変であることを意味します。 \* 他の語では、$\mu$ は $G$ の左右のメジャーです (INT、VII, § 1, No. 2、デフォルト 2)。 \*

*D) 不変手段の存在:

$X$ をハウスドルフ トポロジカル空間、$\mu$ を $X$ の正の有界測度、$X$ の同型写像の $G$ 群とします。すべての $g \in G$ について、写像 $g : X \to X$ の下の $\mu$ の$g.\mu$、像が基底 $\mu$ であるとします。 $u_g$ を、$g.\mu = u_g.\mu$ となるような、$X$ 上の正の $\mu$ 積分可能な関数とします。また、$X$ に 2 つの正の $\mu$ 可積分関数 $\phi$ と $\psi$ が存在し、これらは $\mu$ ヌルではなく、$\phi \leq u_g \leq \psi$ $\mu$ - すべての $g \in G$ に対してほぼどこにでも存在するものであるとします。 $X$ には正の有界測度 $\nu \neq 0$ が存在し、基底 $\mu$ が存在し、$G$ では不変であることを証明します。

$P$ を、バナッハの部分集合空間 $E = L^1(X, \mu)$ からなるの類写像 $f$ として、ほぼどこでも $\phi \leq f \leq \psi$ $\mu$ となるようにします。 次に、$P$ は弱体化した位相 $\sigma(E, E')$ に対してコンパクトです。 $P$ から $X$ の有界実測度のバナッハ空間 $F = \mathscr{M}^b(X)$ への写像 $h \mapsto h.\mu$ は、$P$ から部分集合 $P_1$ への $E$ の凸でコンパクトな全単射です。 位相 $\sigma(F, F')$。 仮定までに、$g \in G$ 全員に対して $g.\mu \in P_1$。 $K$ をすべてのメジャー $g.\mu$ の集合の閉じた凸包絡線とします。 すべての $g \in G$ に対して、写像 $\nu \mapsto g.\nu$ は $K$ の等長アフィン変換です。 Ryll-Nardzewski 著(IV, p. 43, th. 2) では、$G$ の下で不変である測度 $\nu \in K$ が存在します。 $\phi.\mu \leq \nu$ があるため、$\nu \neq 0$ になります。 \*

練習問題

### 練習問題 {#evt-iv-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
