---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 7
section_title: Limits
lang: ja
source: top-i-iv
book_pages: 68-74, 132-133
pdf_pages: 0074-0080, 0138-0139
extraction: ocr
subsections:
    - "no": 1
      title: LIMIT OF A FILTER
      page: 68
      pdf_page: 74
    - "no": 2
      title: CLUSTER POINT OF A FILTER BASE
      page: 69
      pdf_page: 75
    - "no": 3
      title: LIMIT POINT AND CLUSTER POINT OF A FUNCTION
      page: 70
      pdf_page: 76
    - "no": 4
      title: LIMITS AND CONTINUITY
      page: 72
      pdf_page: 78
    - "no": 5
      title: LIMITS RELATIVE TO A SUBSPACE
      page: 73
      pdf_page: 79
    - "no": 6
      title: LIMITS IN PRODUCT SPACES AND QUOTIENT SPACES
      page: 74
      pdf_page: 80
statements: 23
exercises: 7
content_sha256: f68ee3622771de327072950545221fa120563c815b3f066df6e1e03aff7edeea
translated_from: content/en/top/I/07_s7_limits.md
translation_method: google
source_content_sha256: 2a27ef734a6a1ff91fe8d3fb848961a85b666a83e64858598552c6dd593c2d9d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 94b1f408ef7d17dc2db5fd7b99c41fb38ac9a4d7ac0a544c15f71354266a428d
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 7. 極限

### 1. フィルターの極限

#### 定義 1 {#top-i-s7-def-1 .statement tag=0B5B}

$X$ をトポロジー 空間とし、$\mathfrak{F}$ を $X$ のフィルターとします。 $\mathfrak{F}$ が $x$ の近傍フィルター $\mathfrak{B}(x)$ より細かい場合、点 $x \in X$ は $\mathfrak{F}$ の限界点 (または単に限界) であると言われます。 $\mathfrak{F}$は$x$に収束する（または収束する）とも言われています。 *点* $x$ *フィルター 基底* の極限であると言われます $\mathfrak{B}$ *on* $X$、*および* $\mathfrak{B}$ *基底が * $\mathfrak{B}$ であるフィルターの場合、* $x$ に収束すると言われます* $x$ に収束します。

この定義は、§ 6, no. 3 の命題 4 と合わせて、次の基準を与えます。

#### 命題 1 {#top-i-s7-prop-1 .statement tag=0B5C}

*フィルター 基底* $\mathfrak{B}$ *トポロジー上の空間* $X$ *に収束* $x$ ** $x$ *含むの基本的な系の近傍のすべての集合がその場合にのみ集合/* $\mathfrak{B}$。

§ 1, no. 2 で紹介した用語に従って、命題 1 を次のように述べることができます: $\mathfrak{B}$ は、$\mathfrak{B}$ の集合が *できるだけ近い* $x$ である場合に限り、$x$ に収束します。

フィルター $\mathfrak{F}$ が $x$ に収束する場合、$\mathfrak{F}$ よりもすべてのフィルター *より細かい* も、定義 1 により $x$ に収束します。同様に、$X$ の位相が *粗い* に置き換えられた場合、 $x$ の位相、近傍フィルターは *粗い* フィルター ($\S$ 2、no. 2、命題 3) に置き換えられるため、この新しい位相でも $\mathfrak{F}$ は依然として $x$ に収束します。

したがって、*より細かい位相ほど、この位相* には収束フィルターが少なくなります。特に、離散位相では、唯一の収束フィルターは近傍フィルターです。これは、これらが $X$ ($\S$ 6、no. 4) の自明な限外フィルターであるためです。

$\Phi$ を $X$ のフィルターの集合とし、すべて同じ点 $x$ に収束します。 近傍フィルター $\mathfrak{B}(x)$ は $\Phi$ のすべてのフィルターより粗いため、これらのフィルターの *共通部分* $\mathfrak{J}$ よりも粗いです。他の語、$\mathfrak{J}$も$x$に収束します。

#### 命題 2 {#top-i-s7-prop-2 .statement tag=0B5D}

*フィルター* $\mathfrak{F}$ *トポロジー上の空間* $X$ *点* $x$ *$\mathfrak{F}$ よりもより細かいであるすべての限外フィルターが * $x$ に収束する場合に限ります。

これは、前の注意の明らか帰結と § 6, no. 4 の命題 7 です。

一般に、フィルターには *いくつかの異なる極限点* を含めることができます。この質問には§ 8, no. 1で戻ります。

### 2. フィルター 基底のクラスター 点

#### 定義 2 {#top-i-s7-def-2 .statement tag=0B5E}

*トポロジー 空間* $X$ では、*点* $x$ * はフィルター 基底* $\mathfrak{B}$ *on* $X$ *$\mathfrak{B}$ のすべての集合の閉包内にある場合、クラスター 点です。

$x$ がフィルター 基底 $\mathfrak{B}$ のクラスター 点である場合、§ 6, no. 3、系から命題 4 の理由により、すべての*同等* フィルター 基底のクラスター 点でもあります。特に、$x$ は、基底が $\mathfrak{B}$ である *フィルター* のクラスター 点です。

#### 命題 3 {#top-i-s7-prop-3 .statement tag=0B5F}

*点 x は、x の基本系の近傍のすべての集合が B のすべての集合と一致する場合に限り、フィルター 基底 B のクラスター 点です。

これは定義の直後に続きます。

この命題と、§ 6, no. 2 の命題 1 の系 2 は、「x がフィルター $\mathfrak{F}$ のクラスター点である」という性質が、「$\mathfrak{F}$ と x の近傍フィルターよりも細かいフィルターが存在する」という性質と同等であることを示しています。 その他語:

#### 命題 4 {#top-i-s7-prop-4 .statement tag=0B5G}

*点 x は、x に収束する$\mathfrak{F}$ よりもフィルター より細かいがある場合に限り、フィルター $\mathfrak{F}$ のクラスター 点です。*

特に、フィルター $\mathfrak{F}$ のすべての *極限点* は、$\mathfrak{F}$ の *クラスター 点* です。

#### 系 {#top-i-s7-n2-cor-1 .statement tag=0B5H}

*ultrafilter $\mathfrak{U}$ は、x が $\mathfrak{U}$ のクラスター 点である場合に限り、点 x に収束します。*

x がフィルター $\mathfrak{F}$ のクラスター 点である場合、それは $\mathfrak{F}$ より *粗い* すべてのフィルターのクラスター 点でもあります。同様に、*粗い* 位相で X の置き換える位相を作成すると、x は新しい位相の $\mathfrak{F}$ のクラスター 点のままになります。

X 上のフィルターベース $\mathfrak{B}$ のクラスター点のセットは、定義上、セット $\bigcap_{M \in \mathfrak{B}} \overline{M}$ です。

#### 命題 5 {#top-i-s7-prop-5 .statement tag=0B5I}

*トポロジカル空間 X 上のフィルター 基底のクラスター 点の集合は X で閉じられています。*

#### 命題 6 {#top-i-s7-prop-6 .statement tag=0B5J}

*$\mathfrak{B}$ をトポロジカル空間 X の部分集合 A 上のフィルター 基底とします。次に、X 属するから $\overline{A}$ の $\mathfrak{B}$ のすべてのクラスター 点。逆に、$\overline{A}$ のすべての点は、A のフィルターの極限点です。*

最初の主張は簡単です。一方、$x \in \overline{A}$ の場合、X の x の近傍フィルターの A 上のトレースは、明らかに x に収束する A 上のフィルターです。

#### 注意 {#top-i-s7-n2-rem-1 .statement tag=0B5K}

トポロジー 空間のフィルターにはクラスター 点が必要ありません (*なおさら* 極限点も必要ありません)。たとえば、*無限離散空間* では、有限部分集合の補数のフィルターにはクラスター 点がありません。すべてのフィルターにクラスター 点がある空間は数学で重要な役割を果たします。これらについては § 9 で学習します。

### 3. 極限点と写像のクラスター 点

#### 定義 3 {#top-i-s7-def-3 .statement tag=0B5L}

*f をトポロジカル空間 Y への集合 X の写像とし、$\mathfrak{F}$ を X のフィルターとします。 点 $y \in Y$ は、y が極限点 (それぞれクラスター) の場合、フィルター $\mathfrak{F}$ に関して f の極限点 (または単に極限) (それぞれクラスター 点) であると言われます。 点) フィルター 基底 $f(\mathfrak{F})$.*

関係「フィルター $\mathfrak{F}$ に関して、y は f の極限である」は、混乱の恐れがない場合、$\lim_{\mathfrak{F}} f = y$、$\lim_{x, \mathfrak{F}} f(x) = y$、または $\lim_x f(x) = y$ と書かれます。

定義 3 と命題 1 (no. 1) と 3 (no. 2) から、次の基準を推定します。

#### 命題 7 {#top-i-s7-prop-7 .statement tag=0B5M}

*点 $y \in Y$ は、$Y$ の $y$ の各近傍 $V$ に対して、次のような集合 $M \in \mathfrak{F}$ がある場合に限り、フィルター $\mathfrak{F}$ に関して$f$ の極限です。 $f(M) \subset V$ (つまり、$y$ の近傍 $V$ ごとに $\overline{f}(V) \in \mathfrak{F}$)*
*点 $y \in Y$ は、$y$ の各近傍 $V$ と、各 $M \in \mathfrak{F}$ に点 $x \in M$ が存在する場合に限り、$\mathfrak{F}$ に対する$f$ のクラスター 点です。 $f(x) \in V$.* など

#### 例 1 {#top-i-s7-n3-exa-1 .statement tag=0B5N}

位相空間の一連の点 $(x_n)_{n \in \mathbf{N}}$ は、$\mathbf{N}$ の $X$ への写像 $n \to x_n$ です。 分析では、極限点の概念と、そのような写像のクラスター 点を *$\mathbf{N}$ のフレシェフィルター* (§ 6, no. 1) に関して頻繁に使用します。フレシェフィルターに関して$y$が$n \to x_n$の極限である場合、$y$は数列* $(x_n)$の*極限であると言われ、*nは無限大になる傾向がある*ので、$\lim_{n \to \infty} x_n = y$と書きます。 Fréchet フィルターに関する写像 $n \to x_n$ のクラスター 点は、数列* $(x_n)$ の * クラスター 点と呼ばれます。

したがって、*elementary の極限点 (それぞれクラスター 点) である場合、点 $y \in X$ は、数列の $(x_n)$ 点の $X$ の極限 (それぞれクラスター 点) になります。 * $(x_n)$ (§ 6, no. 8) に関連付けられたフィルター。

点 $y$ は、$X$ の $y$ の *すべての* 近傍 $V$、*有限の数を除くすべてについて、$X$ の数列の $(x_n)$ の極限です数列* $(x_n)$ のうち項は * $V$ に含まれています。つまり、すべての $n \geq n_0$ に対して $x_n \in V$ となる整数 $n_0$ があります。同様に、$y$ は数列 $(x_n)$ のクラスター 点です。ただし、$X$ の $y$ の *すべて* 近傍 $V$ と、整数 $n_0$ の *すべて* について、 整数 $n \geq n_0$ は $x_n \in V$ になります。

#### 例 2 {#top-i-s7-n3-exa-2 .statement tag=0B5O}

より一般的には、$f$ をトポロジカルな空間 $X$ に *指示された* 集合 $A$ の写像とします。 $x \in X$ が $A$ の *切断フィルター* に対して $f$ の極限 (それぞれクラスター 点) である場合、 $x$ は $f$ の *極限* (それぞれ *クラスター 点*) であると言われます。 *有向集合* $A$ に関しては、$x = \lim_{z \in A} f(z)$ と書きます。

$X$ のフィルター $\mathfrak{F}$ に関して、$y$ が写像 $f : X \to Y$ の極限 (それぞれクラスター 点) である場合、$y$ は $f$ の極限 (それぞれクラスター 点) のままです。 $\mathfrak{F}$ に関して、$Y$ の置き換える位相を *粗い* 位相で置き換える $\mathfrak{F}$ を *より細かい* (それぞれ *粗い*) フィルターでフィルターします。

#### 命題 8 {#top-i-s7-prop-8 .statement tag=0B5P}

*$f$ を集合 $X$ の写像としてトポロジカル空間 $Y$ にします。この場合、$y \in Y$ は、$X$ にフィルター$\mathfrak{G}$ があり、$\mathfrak{F}$ よりより細かいであり、$y$ が$f$ の極限である場合に限り、$\mathfrak{F}$ に対する$f$ のクラスター点になります。 $\mathfrak{G}$に関して。*

$y$ が $\mathfrak{F}$ に対する $f$ のクラスター 点であり、$\mathfrak{B}$ が $y$ の近傍フィルターである場合、$\overline{f}^{-1}(\mathfrak{B})$ は、集合ごとに$X$ のフィルター基底になります$\overline{f}^{-1}(\mathfrak{B})$ は、$\mathfrak{F}$ (§ 6, no. 6) の集合ごとに満たされます。この注意は、$X$ にフィルター $\mathfrak{G}$ があることも示しています。これは、$\mathfrak{F}$ および基底 $\overline{f}^{-1}(\mathfrak{B})$ (§ 6, no. 2、命題 1、系 2) のフィルターの両方よりもより細かいです。 $y$ は、$\mathfrak{G}$ に対して $f$ の極限点です。

最後に、$f$ が集合 $X$ の写像をトポロジカル空間 $Y$ にすると、$X$ のフィルター $\mathfrak{F}$ に関して $f$ のクラスター 点の集合が *closed* であることに注意してください。 $Y$ (no. 2、命題 5)、おそらく空です。

#### 注意 {#top-i-s7-n3-rem-1 .statement tag=0B5Q}

$X$ のフィルター $\mathfrak{F}$ に関して、$y \in Y$ が写像 $f : X \to Y$ の極限 (それぞれクラスター 点) である場合、$y$ もすべての極限 (それぞれクラスター 点) になります。 写像 $g : X \to Y$ は、$\mathfrak{F}$ (§ 6, no. 9) に関して$f$ と *同じ細菌* を持っています。 $y$は、$\mathfrak{F}$に関して*極限* (*クラスター点*) *細菌* $\tilde{f}$ *の* $f$であると言われています。

### 4. 極限と継続性

$X, Y$ を、$X$ の 2 つのトポロジー 空間、$f$ 写像を $Y$、$\mathfrak{B}$ 近傍で点 $a \in X$ の $X$ にフィルターします。 フィルター $\mathfrak{B}$ に関して $y \in Y$ が $f$ の極限であるというの代わりに、 $y = \lim_{\mathfrak{B}} f$ を書く特別な記法を使用します。

$$
y = \lim_{i \in I} f(x),
$$

そして、$y$ は $f$ * 点* $a$ の *極限である、または $f(x)$ * $y$ * $x$ * $a$ * になる傾向がある* と言います。同様に、$y$ が $\mathfrak{B}$ に関して $f$ のクラスター 点であるというというの代わりに、$y$ * 点* $a$ における * $f$ のクラスター 点であると言います。

no. 3 の連続性 (§ 2, no. 1、定義 1) 命題 7 の定義を考慮すると、次のことがわかります。

#### 命題 9 {#top-i-s7-prop-9 .statement tag=0B5R}

*写像* $f$ *トポロジカル空間* $X$ *トポロジカル空間* $Y$ *点* $a \in X$ *$\lim_{i \in I} f(x) = f(a)$ の場合にのみ*。

#### 系 1 {#top-i-s7-prop-9-cor-1 .statement tag=0B5S}

* $X, Y$ * を、* $X$ * $Y$ * 点* $a \in X$ で連続する 2 つのトポロジー 空間、$f$ 写像とします。 *その後、すべてのフィルター 基底* $\mathfrak{B}$ *on* $X$ *これは $a$ に収束し、 *フィルター 基底* $f(\mathfrak{B})$ *は $f(a)$ に収束します。 *逆に、すべてのウルトラフィルター* $\mathfrak{U}$ *オン* $X$ *$a$に収束する場合、 *ウルトラフィルター 基底* $f(\mathfrak{U})$ *$f(a)$に収束すると、*その後* $f$ *は連続* $a$。

最初の主張は命題 9 の明らか帰結です。2 番目を証明するために、$f$ が $a$ で連続していないと仮定します。次に、Y には $f(a)$ の近傍 W があり、$\overline{f}^{-1}(W)$ はX の$a$ の近傍のフィルタ$\mathfrak{B}$ に属するを加えません。したがって (§ 6, no. 4, 命題 7) $\mathfrak{B}$ よりも限外濾過器 $\mathfrak{U}$, より細かいが存在しますが、含む $\overline{f}^{-1}(W)$ は存在しないため、含むその補数 $A = X - \overline{f}^{-1}(W)$ (§ 6, no. 4, 命題) 5); $f(A) \cap W = \varnothing$ なので、$f(\mathfrak{U})$ は $f(a)$ に収束しません。

#### 系 2 {#top-i-s7-prop-9-cor-2 .statement tag=0B5T}

*g を集合 Z の写像としてトポロジカル空間 X とし、Z のフィルター $\mathfrak{F}$ に関して極限 a を持ちます。 写像 $f : X \to Y$ が a で連続である場合、合成 $f \circ g$ は $\mathfrak{F}$ に関して極限点として $f(a)$ を持ちます。

### 5. 部分空間に対する極限

X, Y を 2 つのトポロジー 空間とし、A を X の部分集合とし、$a \in X$ を A の *閉包* の点とします (ただし、必ずしも A 内にあるとは限りません)。 $\mathfrak{F}$ を、X の $a$ の近傍フィルターの A の *トレース* とします。 $f$ が A の Y への写像である場合、$\mathfrak{F}$ に関して $y \in Y$ が $f$ の極限であるというというの代わりに、$y = \lim_{\mathfrak{F}} f$ と書くと、次のように書きます。

$$
y = \lim_{x \to a, x \in A} f(x)
$$

そして、$y$ は、部分空間* A に対して、a における f の *極限である、または、x が A に留まる間 * 傾向があるように、$f(x)$ * は y に向かう傾向があると言います。すると、$y \in f(A)$ が得られます。

$a$ が X の孤立した点ではない場合、$A = \mathbf{C}\{a\}$ は次のように書きます。

$$
y = \lim_{x \to a, x \neq a} f(x)
$$

$y = \lim_{x \to a, x \in A} f(x)$ の代わりに。

クラスター 点に対して同様の定義を作成します。

$f$ が写像 $g : X \to Y$ の A に対する *制限* である場合、$y$ の場合、$g$ は点 $a \in \overline{A}$ で A に対して極限 (それぞれクラスター 点) $y$ を持つと言います。 A を基準にして、$a$ にある $f$ の極限 (それぞれクラスター 点) です。

B を A の部分集合とし、$a \in X$ を B の閉包の点とします。 $y$ が写像 $f : A \to Y$ の *A に対して *$a$ で極限である場合、$y$ は $a$ で *B に対して *$f$ の極限です。 逆は必ずしも真実ではありません。

しかし、V が点 $a \in \overline{A}$ の X の *近傍* であり、$f$ が $a$ で *$V \cap A$ に対して * 極限 $y$ を持っている場合、 $y$ は、*A と比較して、$a$ においても $f$ の極限です。

$a$ を X の *非孤立* 点とし、$a$ が $\mathbf{C}\{a\}$ の閉包内にあるようにします。この場合、写像 $f : X \to Y$ は、$f(a) = \lim_{x \to a, x \neq a} f(x)$ がある場合に限り、$a$ で *連続* になります。これは定義の直後に続きます。

### 6. 積空間および商空間の極限

#### 命題 10 {#top-i-s7-prop-10 .statement tag=0B5U}

$X$ を集合とし、$(Y_i)_{i \in I}$ をトポロジー 空間の族とし、それぞれの $i \in I$ について、$f_i$ を $X$ の写像から $Y_i$ にします。 $X$ に、$f_i$ が連続する最も粗い位相 $\mathfrak{T}$ を与えます。この場合、$X$ のフィルター $\mathfrak{F}$ が $a \in X$ に収束するために必要かつ十分な条件は、各 $i \in I$ について、フィルター 基底 $f_i(\mathfrak{F})$ が $Y_i$ の $f_i(a)$ に収束する必要があるということです。

$f_i$ は連続しているため、条件が必要です (no. 4、命題 9、系 1)。逆に、条件が満たされていると仮定し、$V$を$X$の$a$のオープン近傍とします。 $\mathfrak{T}$ の定義 (§ 2, no. 3、命題 4) までに、$I$ の有限部分集合 $J$ があり、各 $i \in J$ に対して、$Y_i$ のオープン部分集合 $U_i$ があり、次のようになります。 $i \in J$ の場合は $f_i(a) \in U_i$ など、$V$ 含む集合
$$
\bigcap_{i \in J} f_i^{-1}(U_i).
$$
仮定は、$f_i^{-1}(U_i) \in \mathfrak{F}$ (no. 3、命題 7) を意味します。 $J$ は有限なので、次のようになります。
$$
M = \bigcap_{i \in J} f_i^{-1}(U_i)
$$
属するから$\mathfrak{F}$、そして$M \subset V$。これで証明は完了です。

#### 系 1 {#top-i-s7-prop-10-cor-1 .statement tag=0B5V}

積空間 $X = \prod_{i \in I} X_i$ のフィルタ $\mathfrak{F}$ は、$i \in I$ ごとにフィルタ基底 $\operatorname{pr}_i(\mathfrak{F})$ が $\operatorname{pr}_i(x)$ に収束する場合に限り、点 $x$ に収束します。

#### 系 2 {#top-i-s7-prop-10-cor-2 .statement tag=0B5W}

$f = (f_i)$ を集合 $X$ の写像から積空間 $Y = \prod_{i \in I} Y_i$ とします。次に、各 $i \in I$ $f_i$ が $\mathfrak{F}$ に対して極限 $y_i$ を持つ場合に限り、$X$ のフィルター $\mathfrak{F}$ に対して $f$ は極限 $y = (y_i)$ になります。

#### 命題 11 {#top-i-s7-prop-11 .statement tag=0B5X}

$R$ をトポロジー 空間 $X$ 上の開いた同値関係とし、$\varphi$ を標準写像 $X \to X/R$ とします。次に、各 $x \in X$ と、$\varphi(x)$ に収束する $X/R$ 上の各フィルター 基底 $\mathfrak{B}'$ に対して、$x$ に収束するフィルター $X$ にフィルター 基底 $\mathfrak{B}$ があり、次のようになります。 $\varphi(\mathfrak{B})$ は $\mathfrak{B}'$ と同等です。

$U$ が $X$ の $x$ のいずれかの近傍である場合、$\varphi(U)$ は $X/R$ (§ 5, no. 3、命題 5) の $\varphi(x)$ の近傍であるため、集合が存在します。 $M' \in \mathfrak{B}'$ は $M' \subset \varphi(U)$ になります。 $M = U \cap \varphi^{-1}(M')$とすると、$M' = \varphi(M)$になります。これは、$M'$ が $\mathfrak{B}'$ を通過し、$U$ が $x$ の近傍フィルターを通過すると、集合 $U \cap \varphi^{-1}(M')$ 形が $X$ のフィルター 基底 $\mathfrak{B}$ を通過することを示しています。明らかに、$\mathfrak{B}$ は $x$ に収束し、$\varphi(\mathfrak{B})$ は $\mathfrak{B}'$ に相当します。

### 練習問題 {#top-i-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
