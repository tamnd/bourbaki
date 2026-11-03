---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 3
section_title: Special function spaces
lang: ja
source: top-v-x
pdf_pages: 0299-0314, 0333-0343
extraction: ocr
subsections:
    - "no": 1
      title: SPACES OF MAPPINGS INTO A METRIC SPACE
      page: 0
      pdf_page: 299
    - "no": 2
      title: SPACES OF MAPPINGS INTO A NORMED SPACE
      page: 0
      pdf_page: 301
    - "no": 3
      title: COUNTABILITY PROPERTIES OF SPACES OF CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 304
    - "no": 4
      title: THE COMPACT-OPEN TOPOLOGY
      page: 0
      pdf_page: 306
    - "no": 5
      title: TOPOLOGIES ON GROUPS OF HOMEOMORPHISMS
      page: 0
      pdf_page: 311
statements: 31
exercises: 29
content_sha256: 5b5ece68ce5029c1b4deb05c102a9bb3c39a993b5926aba9c2ae67f9939981e7
translated_from: content/en/top/X/03_s3_special_function_spaces.md
translation_method: google
source_content_sha256: a35a28b9c26f164aeaf3bf1e204cb5b3731409c5cea341ad50336a5b5719bb98
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c23b41cb23a280313cc990fa80925008e651493b455d9623b1ca833ab9eac94a
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. スペシャル写像空間

### 1. 写像の空間をメトリクス空間に変換

$X$ を集合、$Y$ を均一空間、$(f_i)_{i \in I}$ を $Y$ (章 IX, § 1, no. 4) の均一構造を定義する擬似統計のファミリー、$\mathscr{S}$ を集合/部分集合/$X$。 $X$ の各 $i \in I$、各集合 $A \in \mathscr{S}$、および写像の各対 $(u, v)$ を $Y$ に書き込みます

$$
g_{i, A}(u, v) = \sup_{x \in A} f_i(u(x), v(x));
$$

直ちに、$g_{i, A}$ が $\mathscr{F}(X; Y)$ 上の *擬似計量* であり、擬似計量の族 $(g_{i, A})_{i \in I, A \in \mathscr{S}}$ 定義するが $\mathscr{F}(X; Y)$ 上の $\mathscr{S}$-*収束* の一様性であることがわかります。特に：

#### 命題 1 {#top-x-s3-prop-1 .statement tag=0CD8}

*$Y$ が計化可能な一様性空間である場合、$\mathscr{F}(X; Y)$ 上の一様収束の一様性は計化可能です。*

$d$ がその均一構造と互換性のある $Y$ 上の計量である場合、$\mathscr{F}(X; Y)$ 上の均一収束の構造は単一の擬似計量によって定義されます。

$$
\varepsilon(u, v) = \sup_{x \in X} d(u(x), v(x));
$$

一般に、この擬似計量は有限ではありませんが、有限の擬計量 (章 IX, § 1, no. 2) と同等であり、一様収束の一様性はハウスドルフ (§ 1, no. 2, 命題 1) であるため、計量化可能です。

#### 系 {#top-x-s3-n1-cor-1 .statement tag=0CD9}

$X$ をトポロジー 空間とし、$Y$ をメトライズ可能なユニフォーム空間とします。 $X$ のコンパクト部分集合の数列 $(K_n)$ があり、$X$ のすべてのコンパクト部分集合がいくつかの $K_n$ に含まれるとします。この場合、$\mathscr{F}(X; Y)$ でのコンパクトな収束の均一性は計量化可能です。

$K_n$ カバー $X$ なので、$\mathscr{F}_c(X; Y)$ は $\prod_n \mathscr{F}_u(K_n; Y)$ ($§ 1$、no. 2、注意 3) の均一部分空間と同型であり、したがって系は命題 1 (章) から続きます。 IX, § 2, no. 4、定理 1、系 2)。

この系は、$X$ が *局所的にコンパクトかつ σ-コンパクト* (章 I, § 9, no. 9、命題 15、系 1) である場合に特に適用されることに注意してください。

ここで、$Y$ をメトリック空間とし、$d$ をそのメトリックとします。 $X$ がいずれかの集合と $\mathscr{S}$ が $X$ の部分集合のいずれかの集合である場合、すべての写像 $u : X \to Y$ のうち $\mathscr{B}_{\mathscr{S}}(X; Y)$ 集合で、$u(A)$ がそれぞれ *有界* であるように表します。 $A \in \mathscr{S}$。 〜でない限りその逆は、$\mathscr{B}_{\mathscr{S}}(X; Y)$ が $\mathscr{S}$ 収束の均一性を備えているとみなすものと明示的に述べられています。これは、$\mathscr{B}_{\mathscr{S}}(X; Y)$ に関する次の擬似計量系列によって定義されます。

$$
d_A(u, v) = \sup_{x \in A} d(u(x), v(x)) \tag{$A \in \mathscr{S}$}
$$

それは仮定による*有限*です。 $\mathscr{S} = \{X\}$の場合、$\mathscr{B}_{\mathscr{S}}(X; Y)$の代わりに$\mathscr{B}(X; Y)$を書き込みます。 A mapping $u : X \to Y$ is said to be *bounded* if it belongs to $\mathscr{B}(X; Y)$, i.e. if $u(X)$ is a bounded subset of $Y$.

#### 命題 2 {#top-x-s3-prop-2 .statement tag=0CDA}

$X$ を集合 、$Y$ を指標空間とします。有界写像の集合 $\mathscr{B}(X; Y)$ は、空間 $\mathscr{F}_u(X; Y)$ で開いており、閉じています。

$u$ が有界である場合、すべての写像 $v : X \to Y$ は、すべての $x \in X$ について、$d(u(x), v(x)) \leq 1$ が有界であることになります。

$$
d(v(x), v(x_0)) \leq d(u(x), u(x_0)) + 2;
$$

したがって$\mathscr{B}(X; Y)$は開いています。一方、$u$が$\mathscr{F}_u(X; Y)$の$\mathscr{B}(X; Y)$の閉包にある場合、すべての$x \in X$に対して$d(u(x), u_0(x)) \leq 1$となるような写像$u_0 \in \mathscr{B}(X; Y)$が存在します。したがって、$u$ は有界です。

#### 系 1 {#top-x-s3-prop-2-cor-1 .statement tag=0CDB}

$X$ を集合とし、$Y$ をメトリクス空間とします。その後、$\mathscr{B}_{\mathscr{S}}(X; Y)$は$\mathscr{F}_{\mathscr{S}}(X; Y)$で閉店となります。特に、$Y$ が完全であれば、$\mathscr{S}$ の収束の均一性に関しては、$\mathscr{B}_{\mathscr{S}}(X; Y)$ も完全です。

$\mathscr{B}_\mathfrak{S}(X; Y)$ は、部分集合の逆像積の $\prod_{A \in \mathfrak{S}} \mathscr{B}(A; Y)$ $\prod_{A \in \mathfrak{S}} \mathscr{F}_u(X; Y)$ は、$\mathscr{F}_\mathfrak{S}(X; Y)$ の標準写像の下で $\prod_{A \in \mathfrak{S}} \mathscr{F}_u(A; Y)$ になります。したがって、§ 1, no. 5 の定理 1 を考慮すると、最初の主張は § 1, no. 2、注意 3 から続き、2 番目は最初のものから続きます。

#### 系 2 {#top-x-s3-prop-2-cor-2 .statement tag=0CDC}

*X をトポロジカル空間とし、Y を計量空間とします。次に、Y への X のすべての有界連続写像のうちの空間は、$C_u(X; Y)$ で開いており、閉じています。 Y が完了すると完了します。*

問題の空間は$\mathscr{B}(X; Y) \cap C_u(X; Y)$です。最初の主張は命題 2 から続きます。 2 番目は最初の後に続きます ($§ 1$、no. 6、定理 2、系 1)。

### 2. 写像の空間を標準の空間に

より具体的には、Y が非離散値除算環 K (章 IX, § 3, no. 3) に対する *ノルム* ベクトル空間である状況を考えてみましょう。 $y \in Y$の$||y||$ノルムで表しましょう。 集合 $\mathscr{F}(X; Y) = Y^X$ には、標準的に K-ベクトル空間構造が与えられます。 写像 $u : X \to Y$ は、実数値写像 $x \mapsto ||u(x)||$ が X で制限される場合に限り、制限されます。 $u, v$ が X の写像で Y に制限されている場合、$u + v$ と $\lambda u (\lambda \in K)$ が制限されていることは明らかです。他の語では、$\mathscr{B}(X; Y)$ は $\mathscr{F}(X; Y)$ の *ベクトル部分空間* です。さらに、$||u|| = \sup_{x \in X} ||u(x)||$ は $\mathscr{B}(X; Y)$ の *ノルム* です。というのは、三角形不等式を満たし、$||u|| = 0$ は $u = 0$ を意味し、それぞれの $\lambda \in K$ について、

$$
||\lambda u|| = \sup_{x \in X} ||\lambda u(x)|| = \sup_{x \in X} |\lambda| \cdot ||u(x)|| = |\lambda| \cdot \sup_{x \in X} ||u(x)|| = |\lambda| \cdot ||u||.
$$

また、このノルムで定義される$\mathscr{B}(X; Y)$ 上の均一性が一様収束の均一性であることが直ちに検証されます。 〜でない限りその反対は明示的に述べられており、$\mathscr{B}(X; Y)$ が規範的な空間とみなされる場合、問題となるのは上で定義されたノルムです。

#### 命題 3 {#top-x-s3-prop-3 .statement tag=0CDD}

*正規化された空間 Y が完全な場合、X の有界写像のすべての系列 $(u_n)$ は、正規化された空間 $\mathscr{B}(X; Y)$ に絶対収束します (すなわち、$\sum_{n=0}^\infty ||u_n|| < +\infty$ となるようなものです)。 cf. 章 IX, § 3, no. 6) は X で一様収束します。*

なぜなら、$\mathscr{B}(X; Y)$ は完全 (no. 1、命題 2、系 1) であるため、結果は一様に収束する系列の章 IX, § 3, no. 6、命題 11 および定義から続きます。

#### 注意 1 {#top-x-s3-n2-rem-1 .statement tag=0CDE}

$\sum_{n=0}^{\infty} \|u_n\| < +\infty$ の場合、$\sum_{n=0}^{\infty} |u_n(x)| \leq \sum_{n=0}^{\infty} |u_n| < +\infty$
それぞれの$x \in X$;他の語では、各 $x \in X$ 系列と一般的な項 $u_n(x)$ は空間 $Y$ に絶対収束します。 逆は誤りです。あらゆる混乱を避けるため、ときどきは、系列と一般的な項 $u_n$ は *通常収束* であるとします。これは、系列と一般的な項 $\|u_n\|$ が収束することを意味します。 系列は、通常は収束せずに、$X$ で一様に収束する可能性があります。これは、たとえば、空間 $\mathscr{B}(\mathbf{R}, \mathbf{R})$ の系列 $(u_n)$ に当てはまり、次のように定義されます。
$x \in [n\pi, (n+1)\pi]$の場合は$u_n(x) = (1/n) \sin x$、それ以外の場合は$u_n(x) = 0$。

$Y$ が非離散値体 $K$ に対する *ノルム化された代数* (章 IX, § 3, no. 7) である場合、$\mathscr{B}(X; Y)$ は $K$-代数であり、ノルム $\|u\|$ は代数構造と互換性があります。
$$
\|uv\| = \sup_{x \in X} \|u(x)v(x)\| \leq \sup_{x \in X} \|u(x)\| \cdot \|v(x)\|
\leq \sup_{x \in X} \|u(x)\| \cdot \sup_{x \in X} \|v(x)\| = \|u\| \cdot \|v\|.
$$
したがって、$\mathscr{B}(X; Y)$ は、$K$ よりも *標準化された代数* になります。

#### 命題 4 {#top-x-s3-prop-4 .statement tag=0CDF}

*$X_i$ ($1 \leq i \leq n$) と $Y$ を非離散値の除算環 $K$ で正規化ベクトル空間とし、$X = \prod_{i=1}^n X_i$ とします。次に、$X$ のすべての多重線形写像から $Y$ への集合は、空間 $\mathscr{F}_s(X; Y)$ で閉じられます。*

この集合は、すべての $u \in F(X; Y)$ と満たすすべての関係で構成されています
$$
\begin{align*}
u(x_1, \ldots, x_i' + x_i'', \ldots, x_n) &= u(x_1, \ldots, x_i', \ldots, x_n) \\
&\quad + u(x_1, \ldots, x_i'', \ldots, x_n), \\
u(x_1, \ldots, \lambda x_i, \ldots, x_n) &= \lambda u(x_1, \ldots, x_i, \ldots, x_n)
\end{align*}
$$
($1 \leq i \leq n,\ x_i,\ x_i',\ x_i''$ $X_i$ の任意の元、$\lambda$ $K$ の任意の元); 関係 (1) の両辺は $\mathscr{F}_s(X; Y)$ 上で $u$ の写像と連続しているため (§ 1, no. 2, 注意 6)、結果は (章 I, § 8, no. 1, 命題 2) になります。

#### 命題 5 {#top-x-s3-prop-5 .statement tag=0CDG}

*命題 4 の仮説の下では、$X$ の写像から$Y$ への集合 $\mathscr{L}(X_1, \ldots, X_n; Y)$ は、有界収束の位相に関して$\mathscr{F}(X; Y)$ で閉じられます。 $Y$ が完全であれば、有界収束の一様性に関して完全です。*

$\mathscr{G}$ が $X$ のすべての有界部分集合の集合である場合、$\mathscr{L}(X_1, \ldots, X_n; Y)$ は $X$ から $Y$ へのすべての多重線形写像の集合の共通部分であり、 集合 $\mathscr{B}_\mathscr{G}(X; Y)$ (章 IX, § 3, no. 5, 定理 1);したがって、結果は命題 4 および命題 2、系 1 となります。

この小節の残りについて、$K$ は非離散値体を表します。

すると、$\mathscr{L}(X_1, \ldots, X_n; Y)$は$\mathscr{F}(X; Y)$のベクトル部分空間になります。 $B$ を、すべての $(x_i)_{1 \leq i \leq n}$ のうち $X$、集合の単位元ボールとし、$\sup_{1 \leq i \leq n} \|x_i\| \leq 1$ とします。

この場合、$\mathscr{L}(X_1, \ldots, X_n; Y)$ の $\mathscr{B}(B; Y)$ への写像 $u \to u|B$ は単射法です。さらに、この写像の下で、$\mathscr{B}(B; Y)$における一様収束の一様性の逆像は、$\mathscr{L}(X_1, \ldots, X_n; Y)$における有界収束の一様性である。 $X$ のすべての有界部分集合は、形 $\mu B$ の集合 (一部の $\mu \in K^*$) に含まれており、$u$ が $\mathscr{L}(X_1, \ldots, X_n; Y)$ の元である場合、すべての$\|u(z)\| \leq a$ と言えます。 $z \in \mu B$ は、すべての $z \in B$ の $\|u(z)\| \leq a/|\mu|^n$ であるというに相当します。 数であることは簡単に検証できます。
$$
\|u\| = \sup_{z \neq 0} \frac{\|u(z)\|}{\|z\|}
$$
は $\mathscr{L}(X_1, \ldots, X_n; Y)$ と定義する上のノルムであり、この集合に対する有界収束の一様性であり、明らかに
$$
(2) \quad \|u(x_1, \ldots, x_n)\| \leq \|u\| \cdot \|x_1\| \cdots \|x_n\|.
$$

〜でない限りその逆が明示的に述べられており、$\mathscr{L}(X_1, \ldots, X_n; Y)$ が標準的な空間とみなされる場合、問題となるのは上で定義されたノルムです。

#### 命題 6 {#top-x-s3-prop-6 .statement tag=0CDH}

*多重線形マッピング*
$$
(u, x_1, \ldots, x_n) \to u(x_1, \ldots, x_n)
$$
*正規化された空間* $\mathscr{L}(X_1, \ldots, X_n; Y) \times X_1 \times \cdots \times X_n$ *into* $Y$ *は連続*です。

これは、不等式 (2) (章 IX, § 3, no. 5、定理 1) の明らか帰結です。

#### 命題 7 {#top-x-s3-prop-7 .statement tag=0CDI}

*$X, Y, Z$ *3 を標準値空間以上* $K$ とします。 *正規化された空間* の標準写像 $\mathscr{L}(X, Y; Z)$ * の線形写像の空間に * $X$ * に * $\mathscr{L}(Y; Z)$ *それぞれを送信します* $u \in \mathscr{L}(X, Y; Z)$ * 写像* $x \to u(x, .)$ *はのアイソメトリです* $\mathscr{L}(X; Y; Z)$ *上* $\mathscr{L}(X; \mathscr{L}(Y; Z))$。

これは、定義と関係の直後に続きます。
$$
\sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} \|u(x, y)\| \right) = \sup_{\|x\| \leq 1, \|y\| \leq 1} \|u(x, y)\|.
$$

#### 命題 8 {#top-x-s3-prop-8 .statement tag=0CDJ}

$X, Y, Z$ を $K$ の 3 ノルム空間とします。 $\mathscr{L}(X; Y) \times \mathscr{L}(Y; Z)$ から $\mathscr{L}(X; Z)$ への双線形写像 $(u, v) \to v \circ u$ は連続です。

$u \in \mathscr{L}(X; Y)$ と $v \in \mathscr{L}(Y; Z)$ の場合、
$$
||v \circ u|| \leq ||u|| \cdot ||v||,
$$
なぜなら、(2) の理由により、すべての $x \in X$ に対して $||v(u(x))|| \leq ||v|| \cdot ||u(x)|| \leq ||v|| \cdot ||u|| \cdot ||x||$ があるからです。

特に、$K$ 上の正規化空間 $X$ の連続自己準同型の集合 $\mathscr{L}(X)$ において、ノルム $||u||$ は$\mathscr{L}(X)$ の$K$-代数構造と互換性があります。

#### 注意 2 {#top-x-s3-n2-rem-2 .statement tag=0CDK}

$\mathbf{R}^m$ から $\mathbf{R}^n$ への線形 (必然的に連続) マッピングのセット $\mathscr{L}(\mathbf{R}^m; \mathbf{R}^n)$ は、$\mathbf{R}$ の係数を持つ$n$ 行と$m$ 列の行列のセット$M_{n,m}(\mathbf{R})$ と識別できるため、$\mathbf{R}^{mn}$ と識別できます。 $\mathscr{L}(\mathbf{R}^m; \mathbf{R}^n)$ では、有界収束 ($\mathbf{R}^m$ のユークリッド計量に関して)、コンパクト収束、および点単位収束の均一性が、$\mathbf{R}^{mn}$ の *加法的* 均一性で識別されます。 $x = (x_i) \in \mathbf{R}^n$ の標準を次のようにします。
$$
||x|| = \sup_i |x_i|,
$$
そして、$(e_j)$ を $\mathbf{R}^m$ の正規の基礎とします。 $u$ と $v$ が $1 \leq j \leq m$ に対して $\|u(e_j) - v(e_j)\| \leq \epsilon$ となるような $\mathbf{R}^m$ から $\mathbf{R}^n$ への 2 つの線形写像である場合、各ペア $(i, j)$ に対して $|\alpha_{ij} - \beta_{ij}| \leq \epsilon$ が得られます [$U = (\alpha_{ij})$ と $V = (\beta_{ij})$ は次の行列ですそれぞれ$u, v$];逆に、これらの不等式が満たされる場合、$\mathbf{R}^m$ の中心 o と辺 $a$ の立方体の各点 $x$ に対して $\|u(x) - v(x)\| \leq ma\epsilon$ が得られます。

### 3. 連続写像の空間の可算性

#### 定理 1 {#top-x-s3-thm-1 .statement tag=0CDL}

$X$ をコンパクト空間とします。
a) *$X$ が計量可能であり、$Y$ が可算型* (章 IX, § 2, no. 8) の計量可能均一空間である場合、*その後、連続写像の計量可能空間 $C_u(X; Y)$ $X$ を $Y$ に変換すると、一様収束の位相が与えられ、可算型* になります。
b) *逆に、計量可能空間 $C_u(X; \mathbf{R})$ が可算型である場合、$X$ は計量可能です*。

a) $d$ (それぞれ $d'$) を、$X$ の位相 (それぞれ $Y$ の均一性) と互換性のあるメトリクスとする。このとき、$\delta(f, g) = \sup_{x \in X} d'(f(x), g(x))$ は、$X$ がコンパクト (no. 1) であるため、$C(X; Y)$ の写像が有界である、空間 $C(X; Y)$ における一様収束の均一性を定義するメトリックです。 整数 $m > 0, n > 0$ のそれぞれの対について、$G_{mn}$ を写像 $f \in \mathscr{C}(X; Y)$ の集合とし、関係 $d(x, x') \leq 1/m$ が $d(f(x), f(x')) \leq 1/n$ を意味するようにします。すべての写像 $f \in \mathscr{C}(X; Y)$ は一様連続 (章 II, § 4, no. 1、定理 2) であるため、各 $n > 0$ について、$\mathscr{C}(X; Y)$ は集合 $G_{mn}$ の和集合になります。 ($m > 0$)。 $\{a_1, \ldots, a_{p(m)}\}$ を $X$ の有限部分集合とし、中心 $a_i$ と半径 $1/m$ のオープンボールが $X$ ($1 \leq i \leq p(m)$) をカバーするようにします。そして、$(b_r)_{r \in \mathbf{N}}$ を、$Y$ で密な可算数の数列とします。それぞれの写像 $\varphi : [1, p(m)] \to \mathbf{N}$ について、$H_\varphi$ を $f \in G_{mn}$ の集合とし、$1 \leq k \leq p(m)$ に対して $d'(f(a_k), b_{\varphi(k)}) \leq 1/n$ とします。 $b_r$の定義により、$G_{mn}$は$\varphi \in \mathbf{N}^{p(m)}$の集合$H_\varphi$の和集合になります。 $C_{mn}$ を写像 $\varphi \in \mathbf{N}^{p(m)}$ の集合とし、$H_\varphi \neq \emptyset$ とし、それぞれの $\varphi \in C_{mn}$ について $g_\varphi$ を $H_\varphi$ の元とします。最後に、$L_{mn}$ は、$\varphi \in C_{mn}$ に対する $g_\varphi$ の可算数集合を表すものとします。 $f \in G_{mn}$ を、$\varphi$ を $C_{mn}$ の元とし、$f \in H_\varphi$ とします。次に、定義からすぐに、すべての $x \in X$ に対して $d'(f(x), g_\varphi(x)) \leq 4/n$、つまり $\delta(f, g_\varphi) \leq 4/n$ が得られます。したがって、集合 $L_{mn}$ の和集合は、$\mathscr{C}_u(X; Y)$ で密です。なぜなら、すべての整数 $n > 0$ とすべての $f \in \mathscr{C}(X; Y)$ には、$f \in G_{mn}$ となるような $m$ が存在し、$f$ から$L_{mn}$は$\leq 4/n$です。

b) $I = [0, 1]$ とします。 $\mathscr{C}_u(X; I)$は$\mathscr{C}_u(X; \mathbf{R})$の等倍部分空間なので、可算型です。 $(f_n)$ を $\mathscr{C}_u(X; I)$ で密な数列とします。 $X$ の積空間 $K = \mathbf{N}$ と写像 $\psi : x \to (f_n(x))$ を $K$ に変換することを考えてください。これは明らかに連続です。 マッピング $\psi$ は単射的です。なぜなら、数列 $(f_n)$ の定義により、すべての $n$ に対する関係 $f_n(x) = f_n(x')$ は、極限に達すると、すべての関数 $f \in \mathscr{C}(X; I)$ に対して $f(x) = f(x')$ を意味します。しかし、公理(OIV)により$x \neq x'$が点$x$と、$x'$を含まない$x$の近傍$V$に適用される場合、これは不可能です(IX, § 1, no. 5章、定理2)。 従って、コンパクト空間 $X$ は $K$ (章 I, § 9, no. 4, 定理 2, 系 2) の部分空間 $\psi(X)$ と同相です。 $K$ は計数可能で可算型であるため、$\psi(X)$ も同様であり、従って $X$ も同様です。

Q.E.D.

#### 系 {#top-x-s3-n3-cor-1 .statement tag=0CDM}

$X$ を、位相が可算基底を許容する局所コンパクト空間とし、$Y$ を可算型の計量可能均一空間とします。

a) $X$ から $Y$ への連続写像の無限遠極限を持つ空間 $\mathscr{L}$ は、$X$ における一様収束のトポロジーを備えており、可算型の計量化可能空間である。

b) $X$ から $Y$ への連続写像の空間 $\mathscr{C}_c(X; Y)$ は、コンパクトな収束の位相を備え、可算型の計量可能空間です。

a) $X'$ を、$X$ に無限遠で隣接する点によって得られるコンパクト空間とします (章 I, § 9, no. 8, 定理 4)。 定義により、すべての写像 $f \in \mathscr{L}$ は連続する写像 $\overline{f} : X' \to Y$ に一意に拡張でき、従って $f \to \overline{f}$ は L の全単射から $C(X'; Y)$ になります。そして、この全単射は、§ 1, no. 6の命題6による$C_u(X'; Y)$への空間Lの同型写像です。 $X'$ は計量可能 (章 IX, § 2, no. 9、命題 16、系) であるため、結果は定理 1 から得られ、$X'$ と Y に適用されます。

b) $(U_n)$ を、比較的コンパクトなオープン集合による X のカバーとし、X のすべてのコンパクト部分集合がいくつかの $U_n$ (章 I, § 9, no. 9、命題 15、系) に含まれるようにする1)。 $S$ が $\overline{U}_n$ の集合である場合、$C(X; Y)$ 上のコンパクト収束の位相は、$S$ 収束の位相と同じです。従って ($§ 1,$ no. 2, 注意 3) 空間 $C_c(X; Y)$ は積 $\prod_n C_u(\overline{U}_n; Y)$ の部分空間と同相です。それぞれのコンパクト空間 $\overline{U}_n$ は可算基底を持っているため、計量可能です (章 IX, § 2, no. 9、命題 16)。従って、$C_u(\overline{U}_n; Y)$ はそれぞれ計量可能であり、型定理 1 で数えられます。従って、$C_c(X; Y)$ も同様です。

$\mathbf{R}$ 上のすべての有界連続実数値写像のうち空間は、一様収束性位相を備えており、可算型 (練習問題 4) ではないことに注意してください。

### 4. コンパクトオープン位相

#### 定理 2 {#top-x-s3-thm-2 .statement tag=0CDN}

*Xを位相幾何学的な空間、Yを均一な空間とする。 X の各コンパクト部分集合 K と Y の各オープン部分集合 U について、T(K, U) は $u(K) \subset U$ のようなすべての連続写像 $u : X \to Y$ の集合を表すものとします。次に、集合 $T(K, U)$ 生成する位相は $C(X; Y)$ にコンパクトに収束します。*

$Y'$ を Y (章 II, § 3, no. 8) に関連付けられたハウスドルフ制服空間とし、$i : Y \to Y'$ を $Y'$ に対する Y の標準写像とします。 コンパクト収束のトポロジーは、K が X ($§ 1,$ no. 4、命題 4) のすべてのコンパクトなサブセットの集合を通過するため、$C(X; Y)$ から $C_u(K; Y')$ へのマッピング $u \to (i \circ u)|K$ が連続である最も粗いトポロジーです。 したがって、X の各コンパクト部分集合 K に対して $C_c(K; Y')$ の位相の部分基底を取得し、次に $C(X, Y)$ でこれらの部分基底の逆像の和集合 [$\mathfrak{B}(C(X; Y))$] を取得することにより、$C_c(X; Y)$ の位相の部分基底を取得します。 一方、Y のすべてのオープン部分集合は形 $\overline{i}^{-1}(U')$ であり、$U'$ は $Y'$ (章 II, § 3, no. 7, 命題 12) でオープンです。したがって、各コンパクト部分集合 $K' \supset K$ について、$T(K, \overline{i}^{-1}(U'))$ は写像の下の $T(K, U')$ の逆像になります。

$$
C(X; Y) \to C_a(K'; Y').
$$

したがって、X が *コンパクト* で、Y が *ハウスドルフ* であるとき、定理を証明することが残っています。これから仮定を作ります。

まず、$T(K, U)$ が $C_c(X; Y)$ で開いていることを示しましょう。 $u_0$ をこの集合の点とします。 $u_0(K)$ はコンパクト (章 I, § 9, no. 4、定理 2、系 1) であり、開いた集合 $U$ に含まれているため、$V(u_0(K)) \subset U$ のような$Y$ の対称的な取り巻き$V$ が存在します。 (章 II, § 4, no. 3、命題 4、系)。 $W$ を、すべての $x \in K$ に対して $(u(x), u_0(x)) \in V$ となるように、すべての連続写像 $u : X \to Y$ の $C_c(X; Y)$ からなるにおける $u_0$ の近傍とします。そのような写像には、明らかに $u(K) \subset V(u_0(K)) \subset U$ があります。したがって$u \in T(K, U)$、したがって$W \subset T(K, U)$となり、これは私たちの主張を証明します。

逆に、$W$ が点 $u_0 \in C_c(X; Y)$ の近傍である場合、形 $T(K, U)$ の近傍の有限数の $W$ 含む共通部分であることを示しましょう。 $W$ はすべての $u \in C(X; Y)$ の集合であり、すべての $x \in X$ に対して $(u(x), u_0(x)) \in V$ となり、$V$ は$Y$ の与えられた側近であると仮定できます。 $u_0$は$X$に連続なので一様連続です(章 II, § 4, no. 1, 定理 2)。 $V_1$ を $Y$ の対称的な取り巻きとし、$Y \times Y$ で開き、$V_1^2 \subset V$ になるようにします。 $X$ は、各 $u_0(K_i)$ が $V_1$ 小さい ($1 \leq i \leq n$) となるように、コンパクトな集合 $K_i$ ($1 \leq i \leq n$) の有限数でカバーできます。 $U_i$ をオープン集合 $V_1(u_0(K_i))$ とし、$u : X \to Y$ を $n$ 集合 $T(K_i, U_i)$ (これらは近傍である) の共通部分に含まれる連続写像とする$u_0$）。次に、$x \in K_i$、$u(x)$ 属するから $U_i$ ごとに、$u_0(x)$ と $u(x)$ は $V_1^2$ でクローズ、つまり $V$ でクローズとなります。それぞれの $x \in X$ 属するからいくつかの $K_i$ までなので、$u \in W$ があり、証明が完成します。

この結果から、次の定義が得られます。

#### 定義 1 {#top-x-s3-def-1 .statement tag=0CDO}

*$X, Y$ を 2 つのトポロジー 空間とします。必ずしも均一化できるわけではありません。 $X$ の各コンパクト部分集合 $K$ と $Y$ の各オープン部分集合 $U$ について、$T(K, U)$ をすべての $u \in C(X; Y)$ の集合とし、$u(K) \subset U$ とします。 集合 $T(K, U)$ によって生成された $C(X; Y)$ 上の位相は、コンパクト収束の位相またはコンパクトオープン位相と呼ばれます。そして、$C(X; Y)$にこの位相を与えることで得られるトポロジカル空間を$C_c(X; Y)$で表します。

$Y$ が均一空間である場合、定理 2 から、この定義は § 1, no. 3 で与えられたものと一致することがわかります。

$H$ が $C(X; Y)$ の部分集合である場合、$C_c(X; Y)$ の$H$ で誘発される位相は、$H$ のコンパクトオープン位相であると言えます。

#### 例 {#top-x-s3-n4-exa-1 .statement tag=0CDP}

$I$ を $\mathbf{R}$ の区間 $[0, 1]$ とします。 $Y$ が任意のトポロジー 空間である場合、空間 $C_c(I; Y)$ は、$Y$ のパス* の *空間と呼ばれます。パス $u$ の $C_c(I; Y)$ からなるの各 $y \in Y$、部分空間 $\Omega_y(Y)$ について、$u(0) = u(1) = y$ はループ* の *空間 ($Y$) *at 点* と呼ばれます。 $y$。

#### 注意 1 {#top-x-s3-n4-rem-1 .statement tag=0CDQ}

同様に、$Y^X = \mathscr{F}(X; Y)$ の積位相によって $C(X; Y)$ に誘発された位相は、点ごとの収束 * 位相と呼ばれます ($Y$ は必ずしも均一化可能ではありません)。これは、$x$ が $X$ を通過し、$U$ が $Y$ のすべてのオープン部分集合の集合を通過するため、形 $T(\{x\}, U)$ の集合によって生成され、したがってコンパクトオープンよりも粗くなります。 位相。 *$Y$ がハウスドルフの場合、空間 $C_c(X; Y)$ はハウスドルフ* (章 I, § 8, no. 1, 命題 5, 系) であると推測します。

#### 注意 2 {#top-x-s3-n4-rem-2 .statement tag=0CDR}

$\mathscr{S}$ を $Y$ の位相の部分基底とし、$\mathscr{K}$ を次の性質を持つ $X$ のコンパクト部分集合の集合とします。

(R) $L$ が $X$ の任意のコンパクト部分集合で、$V$ が $L$ の任意の近傍である場合、$L \subset \bigcup_i K_i \subset V$ のような集合 $K_i \in \mathscr{K}$ の *有限* 数が存在します。

次に、集合 $T(K, U)$、$K \in \mathscr{K}$ と $U \in \mathscr{S}$、形は、$C(X; Y)$ 上のコンパクトオープン位相の *サブベース* です。これを証明するには、$L$ が $X$ の任意のコンパクト部分集合と $V$ $Y$ の任意の開いた部分集合である場合、および $u \in T(L, V)$ の場合、対の有限数が存在することを示さなければなりません。 $(K_i, U_i)$ は、$K_i \in \mathscr{K}$、$U_i \in \mathscr{S}$、$u \in \bigcap_i T(K_i, U_i) \subset T(L, V)$ のようになります。 注意まず、$\mathscr{S}$ の集合のすべての有限列 $(s_k)$ と、$X$ のすべてのコンパクト部分集合 $M$ について、定義によって $T\left(M, \bigcap_k S_k\right) = \bigcap_k T(M, S_k)$ が得られます。したがって、まず第一に、$\mathscr{S}$の集合の有限共通部分の集合によって置き換える $\mathscr{S}$を求めることができます。つまり、$\mathscr{S}$は、位相の*基底*であると仮定できます。 $Y$。 仮定までに、$u(L)$は準コンパクトになり、$V$に含まれるため、$u(L)$をカバーする$V$に含まれる集合$U_i \in \mathscr{S}$の有限数が存在します。

集合 $\overline{u}^{-1}(U_i)$ は $X$ で開き、$L$ をカバーします。したがって、それぞれの $x \in L$ には、$L$ の $x$ の圧縮近傍 $N_x$ があり、$\overline{u}^{-1}(U_i)$ のいずれかに含まれます。 集合 $N_{x_j} = L_j$ のうちの有限の数で $L$ をカバーできます。それぞれの $j$ について、$L_j \subset \overline{u}^{-1}(U_i)$ となるように、添字 $i$ の 1 つを $i(j)$ で表します。そうなると、各添字 $j$ に対して、$L_j$ をカバーする集合 $K_{jk} \subset \overline{u}^{-1}(U_{i(j)})$、所属から $\mathscr{K}$ までの有限の数が [(R) により] 存在します。それぞれの $v \in \bigcap_{j,k} T(K_{jk}, U_{i(j)})$ には $\bigcup_k v(K_{jk}) \subset U_{i(j)}$ があり、したがって $v(L_j) \subset U_{i(j)}$ と $v(L) = \bigcup_j v(L_j) \subset \bigcup_j U_{i(j)} \subset V$ になります。したがって、私たちの主張が証明されました。

#### 定理 3 {#top-x-s3-thm-3 .statement tag=0CDS}

*$X, Y, Z$を3つのトポロジー空間とし、$f$を$X \times Y$の$Z$への写像とする。 $f$ が連続である場合、$\tilde{f}: x \to f(x, .)$ は $X$ から $C_c(Y; Z)$ への連続写像です。 $Y$ が局所的にコンパクトである場合、逆は true です。*

$f$ が連続であると仮定します。 $\tilde{f}$ が連続であることを示すには、$Y$ の各コンパクトサブセット $K$ と $Z$ の各開いたサブセット $U$ について、$\tilde{f}$ の下にある $T(K, U)$ の逆像 $V$ が $X$ で開いていることを証明する必要があります。 $x_0 \in V$ にしましょう。それぞれの $y \in K$ には $f(x_0, y) \in U$ があり、$f$ は連続であるため、$X$ の $x_0$ の近傍 $V_y$ と、$Y$ の $y$ の近傍 $W_y$ があり、$f(V_y \times W_y) \subset U$ になります。 $K$ はコンパクトなので、集合 $W_{y_i} (1 \leq i \leq n)$ が $K$ を覆うような、点 $y_i \in K$ の有限数が存在します。 $V'$ を近傍の共通部分 $x_0$ の $V_{y_i}$、つまり $x_0$ の近傍とします。 $x \in V'$ と $y \in K$ の場合、$y$ は $W_{y_i}$ のいずれかに含まれ、$x$ はそれぞれの $V_{y_i}$ に含まれるため、$f(x, y) \in U$ になります。従って、$V' \subset V$、従って、$V$は、それぞれの点の近傍となり、その結果、$X$にオープンします。

逆に、$\tilde{f}$ が連続で、$Y$ が局所的にコンパクトであると仮定し、$f$ が連続であることを示しましょう。 $x_0 \in X$、$y_0 \in Y$、$U$ を $Z$ の $f(x_0, y_0)$ のオープン近隣とする。 $X$ には $x_0$ の近傍 $V$ があり、$Y$ には $y_0$ の近傍 $W$ があり、$f(V \times W) \subset U$ となることがわかります。 $y \to f(x_0, y)$ は連続なので、$f(\{x_0\} \times W) \subset U$ のような $y_0$ の *コンパクト* 近傍 $W$ が存在します。 一方、$\tilde{f}$ は連続なので、$x \in X$ の集合 $V$ は $f(x, .) \in T(W, U)$ [つまり、 $f(x, y) \in U$ for all $y \in W$] は $X$ のオープン部分集合であるため、$x_0$ の近傍になります。そして$f(V \times W) \subset U$です。

Q.E.D.

#### 系 1 {#top-x-s3-thm-3-cor-1 .statement tag=0CDT}

*$X$ をローカルコンパクト空間、$Y$ をトポロジカル空間、$H$ 部分集合の $C(X; Y)$ とします。次に、$H$ のコンパクトオープン位相が最も粗く、$H \times X$ から $Y$ への写像 $(u, x) \to u(x)$ が連続します。

なぜなら、定理 3 により、標準単射 $H \to C_c(X; Y)$ が連続である場合に限り、この写像は連続です。

#### 注意 3 {#top-x-s3-n4-rem-3 .statement tag=0CDU}

$X$ を局所コンパクト空間とし、$Y$ をハウスドルフ トポロジカル空間とします。 $\mathscr{T}$ が $C(X; Y)$ の部分集合 $H$ で位相で、写像 $(u, x) \to u(x)$ が $H \times X$ で連続し、$H$ も $\mathscr{T}$ に関して *コンパクト* である場合、$\mathscr{T}$ はコンパクトオープン位相。なぜなら、それは後者よりも系 1 だけより細かいであり、コンパクトオープン位相はハウスドルフであるため、2 つのトポロジーは同一です。 加法で $Y$ が *完全に正規* である場合、$H$ は $Y$ (§ 2, no. 5、定理 2、系 3) の位相と互換性のあるすべての均一性に関して *等連続* であることに注意してください。 部分集合 $K$/$X$ 集合

$$
H(K) = \bigcup_{x \in K} H(x)
$$

は、連続する写像 $(u, x) \to u(x)$ の下の $H \times K$ の像なので、コンパクトです。

#### 系 2 {#top-x-s3-thm-3-cor-2 .statement tag=0CDV}

*$X, Y, Z$ を 3 つのトポロジー 空間とし、$X$ がハウスドルフであり、$Y$ が局所的にコンパクトであるとします。すると、正準全単射 $\mathscr{F}(X \times Y; Z) \to \mathscr{F}(X; \mathscr{F}(Y; Z))$ (集合理論, R, § 4, no. 14) の制限から $C(X \times Y; Z)$ は、$C_c(X \times Y; Z)$ から $C_c(X; C_c(Y; Z))$ への同型写像です。

この制限は確かに全単射です

$$
\rho : \mathscr{C}(X \times Y; Z) \to \mathscr{C}(X; \mathscr{C}_c(Y; Z))
$$

定理 3まで;したがって、$\mathscr{C}(X \times Y; Z)$ のコンパクトオープン位相が、$\mathscr{C}(X; \mathscr{C}_c(Y; Z))$ のコンパクトオープン位相の $\rho$ の下で逆像であることが示される必要があります。 集合 $T(K, U)$、ここで、$K$ は $Y$ のコンパクト部分集合であり、$U$ は $Z$ のオープン部分集合、形は $\mathscr{C}_c(Y; Z)$ の位相のサブベースであるため、次のようになります。 注意 2 では、$\mathscr{C}_c(X; \mathscr{C}_c(Y; Z))$ の位相は形 $T(J, T(K, U))$ の集合によって生成されます。ここで、$K$ と $U$ は上記の通りで、$J$ は $X$ の圧縮部分集合です。ここで、$\rho$ の下の $T(J, T(K, U))$ の像は正確に $T(J \times K, U)$ であるため、オープン集合です。したがって、$\rho$ が連続であることが示されました。 $\rho$ が同型であることを証明するには、まず、$X \times Y$ の形 $J \times K$ の集合に注目します (ここで、$J$ は $X$ の圧縮部分集合であり、$K$ は圧縮部分集合です) $Y$) 満たす条件 (R) の注意 2: $L$ が $X \times Y$ のコンパクト部分集合で、$V$ が $L$ の近傍である場合$X \times Y$、射影 $M = \operatorname{pr}_1(L)$、$N = \operatorname{pr}_2(L)$ は、$X$ と $Y$ がハウスドルフであり、$V \cap (M \times N)$ がコンパクト空間の $L$ の近傍であるため、コンパクトです。 $M \times N$、つまり、$L$ のすべての点には、形 $J \times K \subset V$ の $M \times N$ に近傍が含まれます。ここで、$J \subset M$ と $K \subset N$ はコンパクトです。 $L$ はこれら近傍の有限の数でカバーできるので、主張が証明されます。したがって、形 $T(J \times K; U)$ の集合、ここで、$J$ は $X$ のコンパクト部分集合、$K$ は $Y$ のコンパクト部分集合、および $U$ はオープン部分集合です。 $Z$、生成する位相/$\mathscr{C}_c(X \times Y; Z)$。しかし、$\rho$ の下の $T(J \times K, U)$ の像が $\mathscr{C}_c(X; \mathscr{C}_c(Y; Z))$ のオープン集合 $T(J, T(K, U))$ であることはすでに見ました。したがって、$\rho$ は準同型写像です。

加法 $Z$ が均一化可能であると仮定される場合、系 2 は § 1, no. 4、命題 2 の自明な帰結であることに注意してください。

#### 命題 9 {#top-x-s3-prop-9 .statement tag=0CDW}

*$X, Y, Z$ を 3 つのトポロジー 空間とし、$Y$ を局所的にコンパクトにします。次に、$\mathscr{C}_c(X; Y) \times \mathscr{C}_c(Y; Z)$ から $\mathscr{C}_c(X; Z)$ への写像 $(u, v) \to v \circ u$ は連続です。*

$X$ のすべてのコンパクト部分集合 $K$ と $Z$ のすべてのオープン部分集合 $U$、対 $(u, v)$ の集合 $R$ について、$v(u(K)) \subset U$ が でオープンであることを示さなければなりません。 $\mathscr{C}_c(X; Y) \times \mathscr{C}_c(Y; Z)$。 $(u_0, v_0) \in R$ にしましょう。この場合、$u_0(K)$ は、ローカルコンパクト空間 $Y$ のコンパクト部分集合であり、オープン集合 $\overline{v_0^{-1}}(U)$ に含まれるため、$\overline{v_0^{-1}}(U)$ (章) に含まれる $u_0(K)$ のコンパクト近傍 $L$ が存在します。 I, § 9, no. 7、命題10）。 $u(K) \subset L$ が $u_0$ の近傍であるような、すべての $u \in \mathscr{C}_c(X; Y)$ の集合 $V$、および $v(L) \subset U$ が $v_0$ の近傍であるような、すべての $v \in \mathscr{C}_c(Y; Z)$ の集合 $W$。さらに、関係 $(u, v) \in V \times W$ は $v(u(K)) \subset U$ を意味します。 したがって、結果は次のとおりです。

### 5. 準同型写像の群上のトポロジー

#### 命題 10 {#top-x-s3-prop-10 .statement tag=0CDX}

$X$ を均一空間とし、$H$ をそれ自体に対する $X$ の同型写像の等連続集合とする。 $H$ と $H^{-1}$ に $X$ での点収束の位相が与えられている場合、$H^{-1}$ から $H$ への写像 $u \to u^{-1}$ は連続です。

それぞれの $x_0 \in X$、写像 $u \to u^{-1}(x_0)$ から $H^{-1}$ への $X$ が点 $u_0 \in H^{-1}$ ごとに連続していることを示すだけで十分です。 $V$ を $X$ の対称的な取り巻きとし、$y_0 = u_0^{-1}(x_0)$ とします。 仮定までに、$X$ の対称的な取り巻き $U$ が存在し、関係 $(x, x_0) \in U$ はすべての $u \in H^{-1}$ に対して $(u^{-1}(x), u^{-1}(x_0)) \in V$ を意味します。 $u_0$に近い$W(\{y_0\}, U)$である元$u \in H^{-1}$に乗ります。次に、$(u(y_0), u_0(y_0)) \in U$、つまり $(u(y_0), x_0) \in U$ になります。したがって、$(y_0, u^{-1}(x_0)) \in V$、つまり $(u_0^{-1}(x_0), u^{-1}(x_0)) \in V$ となります。これで証明は完了です。

#### 系 {#top-x-s3-n5-cor-1 .statement tag=0CDY}

$X$ を均一空間とし、$H$ をそれ自体に対する $X$ の同型写像の等連続群とする。すると、$X$ の点ごとの収束の位相は、$H$ の群構造と互換性があります。

これは、§ 2, no. 1、命題 1、系 5 と合わせて、命題 10 の帰結です。

#### 命題 11 {#top-x-s3-prop-11 .statement tag=0CDZ}

$X$ を圧縮空間とし、$\Gamma$ を $X$ のすべての同型写像の群とします。すると、$X$の一様収束の位相は、$\Gamma$の群構造と互換性があります。

$\Gamma \times \Gamma$ から $\Gamma$ への写像 $(u, v) \to v \circ u$ は、この位相に関して連続であることはすでにわかっています (no. 4, 命題 9)。したがって、$u \to u^{-1}$ が $\Gamma$ の点 $u_0$ ごとに連続であることを示さなければなりません。 $u_0^{-1}$ は $X$ 上で一様連続であるため、$X$ の対称な取り巻き $V$ が与えられると、関係 $(x, x') \in W$ が $(u_0^{-1}(x), u_0^{-1}(x')) \in V$ を暗示するような $X$ の取り巻き $W$ が存在します。したがって、$u \in \Gamma$ がすべての $x \in X$ に対して $(u_0(x), u(x)) \in W$ である場合、すべての $x \in X$ に対して $(x, u_0^{-1}(u(x))) \in V$ となり、したがって ($u$ は全単射であるため) すべての $x \in X$ に対して $(u^{-1}(x), u_0^{-1}(x)) \in V$ となります。これで証明は完了です。

ここで、$X$ を局所的にコンパクトな空間とし、$\Gamma$ をそれ自体に対する $X$ のすべての同型写像の群とします。 $X$ のコンパクト収束の位相は、$\Gamma$ (練習問題 17) の群構造と必ずしも互換性がありません。 $X'$ を$\omega$ から $X$ まで無限遠で点を隣接させることによって得られるコンパクト空間を表すとします。 Every homeomorphism $u$ of $X$ onto itself extends uniquely to a homeomorphism $u'$ of $X'$ onto itself such that $u'(\omega) = \omega$ (Chapter I, § 10, no. 3, Corollary to Proposition 7), so that $\Gamma$ can be identified with the subgroup of the group $\Gamma'$ of all homeomorphisms of $X'$ onto itself, consisting of all homeomorphisms which leave $\omega$ fixed. したがって、$C_u(X'; X')$ の$\Gamma$ によって誘発された位相は、$\Gamma'$ (命題 11) の群構造と互換性があり、$\Gamma$ は、次のように定義されるため、[$C_u(X'; X')$ の誘発によって位相に関して] $\Gamma'$ で閉じられます。方程式$u(\omega) = \omega$ (§ 1, no. 2, 注意 6)。 このように $\Gamma$ で定義された $\mathscr{T}_\beta$ 群位相で表します。それはコンパクトな収束の位相よりもより細かいであり、$X$が$X'$の固有の均一性によって引き起こされる均一性を備えている場合、(§ 1, no. 6、命題6のおかげで)$X$の一様収束の位相として定義することもできます。

位相 $\mathscr{T}_\beta$ は次のように特徴付けることができます。

#### 命題 12 {#top-x-s3-prop-12 .statement tag=0CE0}

*局所的にコンパクトな空間 $X$ のすべての同型写像の群 $\Gamma$ では、位相 $\mathscr{T}_\beta$ が最も粗く、$\Gamma$ から $C_c(X; X)$ への写像 $u \to u$ と $u \to u^{-1}$ は連続*

後者の位相を今のところ$\mathscr{C}'$で表すことにします。 $u \to u^{-1}$は$\mathscr{T}_\beta$に関して連続であり、$\mathscr{T}_\beta$はコンパクト収束の位相よりより細かいであるため、$\mathscr{T}_\beta$は$\mathscr{C}'$よりより細かいであることが明らかです。 逆を証明するには、$X'$ に独自の均一性を与えます。 $u_0 \in \Gamma$ と $V$ を $X'$ の取り巻きとする。次に、関係となるような、$X$ のコンパクトな部分集合 $K$ と $X'$ の対称的な取り巻き $W$ が存在することを証明する必要があります。

$$
u \in \Gamma, \ (u_0(x), u(x)) \in W \text{ and } (u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K
$$

暗示する

$$
(u_0(x), u(x)) \in V \text{ for all } x \in X.
$$

$V_1$ を、$\overset{2}{V}_1 \subset V$ となるような $X'$ の対称な開いた取り巻きとします。この場合、$K_1 = X' - V_1(\omega)$ は $X$ のコンパクトな部分集合です。 選ぶ $W \subset V$ と $W(\omega) \cap W(u_0^{-1}(K_1)) = \emptyset$ のような、$X'$ の対称的な開いた取り巻き $W$。これは、章 II, § 4, no. 3 の命題 4 までに可能です。 $X$の部分集合をコンパクトにした$K_2 = X' - W(\omega)$とします。 $W$ とコンパクトな集合 $K = K_1 \cup K_2$ が必要なことを行うことがわかります。 $W \subset V$ なので、関係であることを示すだけで十分です。

$$
(u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K_1 \quad (u \in \Gamma)
$$

ということを暗示します

$$
(u(y), \omega) \in V_1 \text{ for all } y \in W(\omega);
$$

なぜなら、そのとき私たちは$(u_0(y), \omega) \in V_1$も持つことになるからです。

$$
(u_0(y), u(y)) \in \overset{2}{V}_1 \subset V
$$

$y \in W(\omega) = X' - K_2$の皆さんへ。さて、$y \in W(\omega)$ があったとしたら、

$$
u(y) \in X' - V_1(\omega) = K_1,
$$

$W$の選択とは逆に、$y \in u^{-1}(K_1) \subset W(u_0^{-1}(K_1))$になります。したがって、証明は完了です。

一般に、$\mathscr{T}_\beta$ を備えた群 $\Gamma$ は局所的にコンパクトではありません。しかし、次の基準があります。

#### 定理 4 {#top-x-s3-thm-4 .statement tag=0CE1}

*$G$ を局所コンパクト空間 $X$ のすべての同型写像の群 $\Gamma$ の部分群とします。 空間 $C_c(X; X)$ に、恒等写像 $e$ の近傍 $V$ があり、$V \cap G = H$ は $G$ では対称で、$C_c(X; X)$ では比較的コンパクトであるとします。次に、位相 $\mathscr{T}_\beta$ に対する $\Gamma$ の$G$ の閉包 $\overline{G}$ は、$\mathscr{T}_\beta$ によって引き起こされる位相に関して局所的にコンパクトな群です。この $\overline{G}$ に誘起された位相はコンパクト収束の位相と同じであり、これに対して $C_c(X; X)$ の $H$ の閉包 $\overline{H}$ は、$\overline{G}$ の $e$ の近傍です。 位相.*

まず、$\overline{H}$ が $\Gamma$ に含まれていること、および $\mathscr{T}_\beta$ によって $\overline{H}$ に誘導される位相が *コンパクト収束の位相と同じ*であることを示しましょう。 $u_0 \in \overline{H}$ にしましょう。したがって、$u_0$ は、$C_c(X; X)$ の$H$ の限外濾過器 $\Phi$ の極限です。 $\Phi^{-1}$ ($u \to u^{-1}$ の下の $\Phi$ の像) は、$H \subset \overline{H}$ の限外フィルター 基底であるため、$C_c(X; X)$ から元 $v_0$ のコンパクトな部分空間 $\overline{H}$ に収束します。 写像 $(u, v) \to uv$ は、$\Phi \times \Phi^{-1}$ (no. 4、命題 9) に関して$u_0 v_0$ に収束します。 *なおさら*、$u \to uu^{-1} = e$は$\Phi$に関して$u_0 v_0$に収束します。したがって、$C_c(X; X)$はハウスドルフであるため、$u_0 v_0 = e$になります。 同様に $v_0 u_0 = e$;したがって、$u_0$ は $X$ の同型写像、つまり $u_0 \in \Gamma$ です。 したがって、$\overline{H}$ は $\Gamma$ に含まれます。 さらに、この議論は、$\overline{H}^{-1} = \overline{H}$ と、$u_0$ に収束する$\overline{H}$ のすべての限外濾過器 $\Phi$ について、$\Phi^{-1}$ が $C_c(X; X)$ から $u_0^{-1}$ に収束することを示しています。したがって、$\overline{H}$ から $C_c(X; X)$ への写像 $u \to u^{-1}$ は、$\overline{H}$ がコンパクトな収束のトポロジーを運ぶ場合、連続的になります (I, § 7, no. 4 章、命題 9、系 1)。 次に、命題 12 は、$\overline{H}$ において、コンパクト収束の位相が $\mathscr{T}_\beta$ によって引き起こされた位相と同じであることを示します。

さらに、$\Gamma$上のトポロジー$\mathscr{T}_\beta$はコンパクト収束のトポロジーよりも細かいため、$\overline{H}$は$\mathscr{T}_\beta$に対する$H$の閉包でもあります。 しかし、$H$はコンパクト収束の位相に関しては$G$の$e$の近傍であり、$\mathscr{T}_\beta$によって誘導された位相に関しては*なおさら*です。 (章 I, § 3, no. 1, 命題 2) により、$\mathscr{T}_\beta$ によって誘導された位相に関して、$\overline{H}$ は $\overline{G}$ の $e$ の近傍であるため、この中で $\overline{G}$ は局所的にコンパクトになります。 位相。 $W$ がコンパクト収束の位相に関して $V$ の内部である場合、$W \cap \Gamma$ は $\mathscr{T}_\beta$ で開いているため、$W \cap \overline{G}$ は $\mathscr{T}_\beta$ に関して$H = V \cap G$ の閉包に含まれます (章 I, § 1, no. 6, 命題 5);これは、コンパクト収束の位相に関して、$\overline{H}$ は $\overline{G}$ の $e$ の近傍でもあることを示しています。 最後に、各 $u_0 \in \Gamma$、全単射 $v \to u_0 \circ v$、$C_c(X; X)$ の $v \to u_0^{-1} \circ v$ は連続しています (no. 4、命題 9)。したがって、$u_0 \in \overline{G}$ の場合、$u_0 \overline{H}$ は$u_0$ の近傍になります。コンパクトコンバージェンスの位相に対して$\overline{G}$。 これで証明は完了です。

#### 系 {#top-x-s3-n5-cor-2 .statement tag=0CE2}

*$G$を局所コンパクト空間$X$の準同型写像の群とする。 $C_c(X; X)$ の $G$ の閉包 $\overline{G}$ がコンパクトであれば、 $\overline{G}$ は $X$ の同型写像の群であり、コンパクトな収束の位相は $\overline{G}$ の群構造と互換性があるため、コンパクトなトポロジカルになります。 群.*

局所的にコンパクトではあるが、コンパクト収束のトポロジーに関してはコンパクトではない、局所的にコンパクトな空間 $X$ の同型写像の群は、I, § 9, no. 7 章、命題 12 のおかげで、$C_c(X; X)$ で *局所的に閉じられています*が、*必ずしも閉じているわけではありません*。

たとえば、$\mathbf{R}^n$の自己準同型の環$\mathscr{L}(\mathbf{R}^n)$では、$\mathbf{R}$以上の平方$n \times n$行列の環$M_n(\mathbf{R})$と同一視され、コンパクトな収束の位相を備えています。 群 $GL(n, \mathbf{R})$ は、非単数行列の群と同一視され、局所的にコンパクトですが密度が高くなります (章 VI, § 1, no. 6、命題 6)。

### 練習問題 {#top-x-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
