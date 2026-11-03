---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 2
section_title: Continuous functions
lang: ja
source: top-i-iv
book_pages: 25-35, 119-122
pdf_pages: 0031-0041, 0125-0128
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS FUNCTIONS
      page: 25
      pdf_page: 31
    - "no": 2
      title: COMPARISON OF TOPOLOGIES
      page: 28
      pdf_page: 34
    - "no": 3
      title: INITIAL TOPOLOGIES
      page: 30
      pdf_page: 36
    - "no": 4
      title: FINAL TOPOLOGIES
      page: 32
      pdf_page: 38
    - "no": 5
      title: PASTING TOGETHER OF TOPOLOGICAL SPACES
      page: 34
      pdf_page: 40
statements: 30
exercises: 11
content_sha256: 32dc4b40227751403be90f5d738256a13468457e354e8f4bde1ce4ff523ef020
translated_from: content/en/top/I/02_s2_continuous_functions.md
translation_method: google
source_content_sha256: 1967343889fcc981f4c5cd14526701e2a3a3c66ffbc62c0729eebd3c4a84398d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 33fcd2bbb0fa6384be693e4a8d7dda359ebe32bd43cda471a34c4558dae0afd3
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 連続写像

### 1. 連続写像

#### 定義 1 {#top-i-s2-def-1 .statement tag=0AZY}

トポロジカル空間 $X$ からトポロジカル空間 $X'$ への写像 $f$ は、$f(x_0)$ の近傍 $V'$ が与えられた場合、点 $x_0 \in X$ で連続であると言われます。 $X'$ には、$X$ に $x_0$ の近傍 $V$ があり、関係 $x \in V$ は $f(x) \in V'$ を暗示します。

定義 1 は、次のより直観的な形で言い換えることができます。 $f$ が点 $x_0$ で連続していると言うのは、$x$ が$x_0$ に十分に近いときはいつでも、$f(x)$ が$f(x_0)$ に限りなく近いことを意味します。

「各 $x \in V, f(x) \in V'$ について」の関係は、$f(V) \subset V'$、または再び $V \subset \overline{f}^{-1}(V')$ と同等です。近傍公理 ($V_I$) を考慮すると、定義 1 は次と同等であることがわかります。 $X'$ の $f(x_0)$ の各近傍 $V'$ について、$\overline{f}^{-1}(V')$ が $x_0$ の近傍である場合、$f : X \to X'$ は点 $x_0$ で連続であると言われます。 $X$。 さらに、$X'$ ($§ 1$、no. 3) の$f(x_0)$ の近傍の基本系に対して、近傍 $V'$ 所属の$x_0$ の近傍が$\overline{f}^{-1}(V')$ であれば十分です。

#### 命題 1 {#top-i-s2-prop-1 .statement tag=0AZZ}

$f$ をトポロジカル空間 $X$ の写像からトポロジカル空間 $X'$ にするとします。 $f$ が $x$ で連続し、$x$ が $X$ の部分集合 $A$ の閉包内にある場合、$f(x)$ は $f(A)$ の閉包内にあります。

$V'$ を $X'$ の $f(x)$ の近傍とします。 $f$は$x$で連続なので、$\overline{f}^{-1}(V')$は$X$の$x$の近傍です。したがって、$\overline{f}^{-1}(V')$ は $A$ と出会い、そこから $V'$ は $f(A)$ と出会い、したがって $f(x)$ は $f(A)$ の閉包内にあります。

#### 命題 2 {#top-i-s2-prop-2 .statement tag=0B00}

$X, X', X''$ を 3 つのトポロジー 空間とします。 $f$ を $X$ の写像から $X'$ にし、$x \in X$ で連続します。 $g$ を $X'$ の写像から $X''$ に、$f(x)$ で連続します。すると、合成 $h = g \circ f : X \to X''$ が$x$ で連続します。

$V''$を$X''$の$h(x) = g(f(x))$の近傍とします。 $g$は$f(x)$で連続なので、$\overline{g}^{-1}(V'')$は$X'$の$f(x)$の近傍になります。しかし、$f$は$x$で連続であるため、$\overline{f}^{-1}(\overline{g}^{-1}(V'')) = \overline{h}^{-1}(V'')$は$X$の$x$の近傍であり、したがって$h$は$x$で連続です。

#### 定義 2 {#top-i-s2-def-2 .statement tag=0B01}

トポロジカル空間 $X$ からトポロジカル空間 $X'$ への写像は、$X$ の各点で連続である場合、$X$ で連続である (または単に連続である) と言われます。

#### 例 1 {#top-i-s2-n1-exa-1 .statement tag=0B02}

それ自体へのトポロジカル空間 $X$ の恒等写像は連続です。

#### 例 2 {#top-i-s2-n1-exa-2 .statement tag=0B03}

トポロジー 空間からトポロジー 空間への定数写像は連続です。

#### 例 3 {#top-i-s2-n1-exa-3 .statement tag=0B04}

離散空間からトポロジカル空間へのすべての写像は連続です。

#### 定理 1 {#top-i-s2-thm-1 .statement tag=0B05}

$f$ をトポロジカル空間 $X$ の写像からトポロジカル空間 $X'$ にします。したがって、次の主張は同等です。

a) $f$ は $X$ で連続しています。

b) $X$ の部分集合 $A$ ごとに、$f(\overline{A}) \subset \overline{f(A)}$。

c) $X'$ のすべてのクローズド部分集合の $f$ の下の逆像は、$X$ のクローズド部分集合です。

d) $X'$ のすべてのオープン部分集合の $f$ の下の逆像は、$X$ のオープン部分集合です。

a) が b) を暗示していることはすでに見ました (命題 1)。 b) が c) を暗黙的に示すために、$F'$ を $X'$ の閉じた部分集合とし、$F = \overline{f^{-1}(F')}$ とします。その後、仮定 $f(\overline{F}) \subset \overline{f(F)} \subset \overline{F'} = F'$ までに、したがって $\overline{F} \subset \overline{f^{-1}(F')} = F \subset \overline{F}$ となり、$F = \overline{F}$ と $F$ が閉じられます。 $X'$ のすべての部分集合 $A'$ に対する関係 $\overline{f^{-1}(A')} = \overline{f^{-1}(CA')}$ により、c) は d) を意味します。最後に、d) が満たされるとします。 $x$ を $X$ の任意の点とし、$V'$ を $X'$ の $f(x)$ の任意の近傍とします。次に、$X'$ にオープンの集合 $A'$ があります。

$$
f(x) \in A' \subset V'
$$

したがって $x \in \overline{f^{-1}(A')} \subset \overline{f^{-1}(V')}$ です。 仮定までに、$\overline{f^{-1}(A')}$は$X$でオープンするため、$\overline{f^{-1}(V')}$は$X$の$x$の近傍になります。したがって、d) は a) を意味します。

#### 注意 {#top-i-s2-n1-rem-4 .statement tag=0E95}

1) $\mathfrak{B}$ を $X'$ の位相の基底 (§ 1, no. 3) とします。次に、$f : X \to X'$ が連続するためには、$U' \in \mathfrak{B}$ ごとに $X$ で $\overline{f^{-1}(U')}$ が開いていることが必要かつ十分です。

#### 例 {#top-i-s2-n1-exa-4 .statement tag=0B06}

$a$ を任意の有理数数とします。 有理線 $\mathbf{Q}$ のそれ自体への写像 $x \to a + x$ は、$\mathbf{Q}$ 上で連続します。この開区間の写像の下での逆像 $]b, c[$ が開区間です。

$$
]b - a, c - a[.
$$

同様に、写像 $x \to ax$ は $\mathbf{Q}$ で連続します。これは、$a = 0$ であれば、すべての $x$ に対して $ax = 0$ であることが明らかです。 $a \neq 0$ の場合、オープン区間 $]b, c[$ のこの写像の下にある逆像は、エンドポイント $b/a$ と $c/a$ を持つオープン区間です。

2) 連続マッピング $f : X \to X'$ の下での $X$ の開いた (または閉じた) セットの直接イメージは、 $X'$ (cf. § 5) で必ずしも開いた (または閉じた) とは限りません。

#### 例 {#top-i-s2-n1-exa-5 .statement tag=0B07}

\* $\mathbf{R}$ のそれ自体へのマッピング $f : x \to 1/(1 + x^2)$ は連続的ですが、$f(\mathbf{R})$ は半開区間 $]0, 1]$ であり、$\mathbf{R}$ では開いていても閉じていません。 \*

#### 定理 2 {#top-i-s2-thm-2 .statement tag=0B08}

1) $f : X \to X'$ と $g : X' \to X''$ が 2 つ連続する写像の場合、$g \circ f : X \to X''$ は連続します。

2) 位相空間 $X$ の位相空間 $X'$ への全単射 $f$ が同相同型であるためには、$f$ と $f$ の逆行列が連続であること (または、言われているように、$f$ が共連続であること) が必要かつ十分です。

最初の主張は命題 2 の明らか帰結です。 2 番目は、同型写像 (§ 1, no. 1) の定理 1, d) と定義から続きます。

#### 注意 1 {#top-i-s2-n1-rem-1 .statement tag=0B09}

共連続ではないトポロジカル空間 $X'$ にトポロジカル空間 $X$ の連続全単射を持たせることは可能です。たとえば、$X'$ を有理線 $\mathbf{Q}$ とし、$X$ を集合 $\mathbf{Q}$ とします。個別の位相を使用します。この場合、恒等式写像 $X \to X'$ は連続ですが、同型ではありません。

#### 注意 2 {#top-i-s2-n1-rem-2 .statement tag=0B0A}

連続全単射 $f : X \to X'$ が同型であることを検証するには、各 $x \in X$ と $x$ の各近傍 $V$ について、$f(V)$ が $X'$ の $f(x)$ の近傍であることを示すだけで十分です。

#### 注意 3 {#top-i-s2-n1-rem-3 .statement tag=0B0B}

$X$ をトポロジー 空間とし、各 $x \in X$ について、$\mathfrak{B}(x)$ を $x$ のすべての近傍の集合とします。 $x_0$ を $X$ の点とします。 $X$ の部分集合の各 $x \in X$、定義する集合 $\mathfrak{B}_0(x)$ については次のようになります: $\mathfrak{B}_0(x_0) = \mathfrak{B}(x_0)$、$x \neq x_0$ の場合、$\mathfrak{B}_0(x)$ はすべての部分集合の集合になります。 $X$ と含む $x$。 集合 $\mathfrak{B}_0(x)$ は、$X$ の位相に対して、$X$ の近傍の点の集合であることがすぐに検証されます (§ 1, no. 2、命題 2)。 $X_0$ はこのようにして得られたトポロジー 空間を表し、$j : X_0 \to X$ は連続であるが一般に共連続ではない恒等式写像を表します。 $X$ の位相空間 $X'$ への写像 $f$ は、合成 $X_0 \xrightarrow{j} X \xrightarrow{f} X'$ が $X_0$ で連続している場合に限り、点 $x_0$ で連続します。これは定義からすぐにわかります。

### 2. トポロジの比較

no. 1 の定理 2 は、連続写像を位相幾何学構造 (集合理論, 章 IV, § 2, no. 1) の射として取ることができることを示しています。これからは、これを射の選択にしたと仮定します。一般的な定義 (集合理論、章 IV, § 2, no. 2) に従って、これにより、特定の集合 $X$ でトポロジの集合での順序付けが定義する可能になります。

#### 定義 3 {#top-i-s2-def-3 .statement tag=0B0C}

同じ集合 $X$ 上の 2 つのトポロジ $\mathfrak{T}_1, \mathfrak{T}_2$ が与えられ、$X_i$ 集合で示される場合、$\mathfrak{T}_1$ は $\mathfrak{T}_2$ よりもより細かい (そして $\mathfrak{T}_2$ は $\mathfrak{T}_1$ より粗い) であると言います。 $X$と位相$\mathfrak{T}_i$($i = 1, 2$)、恒等写像$X_1 \to X_2$は連続です。 加法 $\mathfrak{T}_1 \neq \mathfrak{T}_2$ の場合、$\mathfrak{T}_1$ は$\mathfrak{T}_2$ よりも厳密により細かいであると言います (そして、$\mathfrak{T}_2$ は$\mathfrak{T}_1$ より厳密に粗いです)。

2 つのトポロジーは、一方が他方よりより細かい高く、同等であると言われています。

写像が連続であるための基準 (no. 1、定義 1 および定理 1) は、次の命題を与えます。

#### 命題 3 {#top-i-s2-prop-3 .statement tag=0B0D}

集合 $X$ に 2 つのトポロジ $\mathfrak{T}_1, \mathfrak{T}_2$ がある場合、次の主張は同等です。
a) $\mathfrak{T}_1$ は $\mathfrak{T}_2$ よりより細かいです。
b) 各 $x \in X$ について、$\mathfrak{T}_2$ に対する $x$ の各近傍は、$\mathfrak{T}_1$ に対する $x$ の近傍です。
c) $X$ の各部分集合 $A$ について、位相 $\mathfrak{T}_1$ の $A$ の閉包は、位相 $\mathfrak{T}_2$ の $A$ の閉包に含まれます。
d) $\mathfrak{T}_2$ でクローズされる $X$ のすべての部分集合は、$\mathfrak{T}_1$ でクローズされます。
e) $\mathfrak{T}_2$ にオープンする $X$ のすべての部分集合は、$\mathfrak{T}_1$ にオープンします。

#### 例 {#top-i-s2-n2-exa-1 .statement tag=0B0E}

\* ヒルベルト空間 $H$ からなる of 数列 $x = (x_n)$ of 実数では、次のようになります
$$
\|x\|^2 = \sum_{n=0}^\infty x_n^2 < +\infty,
$$
$H$の強い位相の点$x_0$の近傍は集合で、含むは$x_0$を中心としたオープンボール$\|x - x_0\| < \alpha$です。 $H$ の弱い位相の $x_0$ の近傍は、形 $\sup_{1 \leq i \leq n} |(x - x_0|a_i)| \leq 1$ の関係によって定義される集合含む集合で、$a_i$ は$H$中点と
$$
(x|y) = \sum_{n=0}^\infty x_n y_n
$$
$x = (x_n)$ と $y = (y_n)$ の場合。ここで、$\beta = \sup_{1 \leq i \leq n} \|a_i\|$、関係 $\|x - x_0\| \leq 1 / \beta$ は、$1 \leq i \leq n$ に対して $|(x - x_0|a_i)| \leq \|x - x_0\| \cdot \|a_i\| \leq 1$ を意味します。したがって、$H$の強い位相は、弱い位相よりもより細かいになります。一方、$H$の点の有限族$(a_i)_{1 \leq i \leq n}$が与えられると、$1 \leq i \leq n$に対して$(x - x_0|a_i) = 0$が成り、$\|x - x_0\|$が任意に大きくなるような$H$には点$x$が存在します。これは、強い位相が弱い位相よりも厳密により細かいであることを示しています。 \*

#### 注意 1 {#top-i-s2-n2-rem-1 .statement tag=0B0F}

集合 $X$、位相のすべてのトポロジの順序付き集合では、開いている集合のみが $\varnothing$ であり、$X$ が最も粗く、離散位相が最も細かくなります。

#### 注意 2 {#top-i-s2-n2-rem-2 .statement tag=0B0G}

より細かい位相、集合が開くほど、集合と近傍は閉じます。 より細かい位相、集合の閉鎖部 (内部) が小さくなる (それぞれ大きくなる)。 より細かい位相ほど、密度は低くなります集合。

#### 注意 3 {#top-i-s2-n2-rem-3 .statement tag=0B0H}

$f : X \to X'$ が連続的な写像である場合、$X$ の位相がより細かい位相に置き換えられ、$X'$ の位相がより粗い位相 (no. 1、 定理 2）。他の $X$ の語、より細かい位相、および $X'$ の粗い位相では、$X$ から $X'$ への写像がより連続します。

### 3. 初期トポロジー

#### 命題 4 {#top-i-s2-prop-4 .statement tag=0B0I}

$X$ を集合とし、$(Y_i)_{i \in I}$ をトポロジカル空間の族とし、それぞれの $i \in I$ について、$f_i$ を $X$ の写像から$Y_i$ にします。 $\mathscr{S}$ を形の $X$ $\overline{f}_i^{-1}(U_i)$ の部分集合の集合 ($i \in I$、$U_i$ は $Y_i$ にオープン)、$\mathfrak{B}$ を有限共通部分の集合とします。 $\mathscr{S}$中集合。 次に、$\mathfrak{B}$ は、$X$ 上の位相 $\mathfrak{T}$ の基底であり、これは、ファミリー $(f_i)$ (集合理論、章 IV, § 2, no. 3) の $X$ 上の初期トポロジー 構造であり、特に、$X$ の最も粗い位相は、写像 $f_i$ が連続しています。 より正確には、$g$ がトポロジカル空間 $Z$ から $X$ への写像である場合、$g$ は点 $z \in Z$ (X 位相 $\mathfrak{T}$ を運ぶ) で連続します。 写像 $f_i \circ g$は$z$で連続です。

$\mathscr{D}$ を、$\mathfrak{B}$ に属する集合のすべての和集合の集合とします。共用体の形成は結合的であるため、$\mathscr{D}$ は公理 $(O_1)$ を明らかに満たします。そして、$\mathscr{D}$ は、$\mathfrak{B}$ の定義と、有限交差が任意の和集合に対して分配的であるという事実により、公理 $(O_{II})$ を満たします [集合論、R § 4、式 (37)]。 したがって、集合 $\mathscr{D}$ は、位相 $\mathfrak{T}$ に対して、$X$ のオープン部分集合の集合であり、そのうち $\mathfrak{B}$ は基底です。 初期構造 (集合理論、章 IV, § 2, no. 3、基準 CST 9) の一般的性質により、その他を暗示する命題の最後の主張を証明します。 そもそも、$\mathscr{S}$の定義は、$f_i$が$X$(no. 1、定理1)で連続していることを示しています。したがって、$g$ が $z$ で連続である場合、写像 $f_i \circ g$ (no. 1, 命題 2) も連続です。 逆に、すべての写像 $f_i \circ g$ が $z$ で連続し、$V$ が $X$ の $g(z)$ の近傍であるとします。 定義までに、$I$ の有限部分集合 $J$ があり、各 $i \in J$ には、$V$ 含む集合 $\bigcap_{i \in J} \overline{f}_i^{-1}(U_i)$ のように、$Y_i$ のオープン部分集合 $U_i$ が存在します。そして$g(z)$属するからこれ集合まで。 したがって、
$$
\overline{g}^{-1}(V) \supset \bigcap_{i \in J} \overline{g}^{-1}(\overline{f}_i^{-1}(U_i)),
$$
そして、仮定は、集合 $\overline{g}^{-1}(\overline{f}_i^{-1}(U_i))$ のそれぞれが $Z$ の $z$ の近傍であることを意味します。したがって、$\overline{g}^{-1}(V)$ は、$Z$ の $z$ の近傍でもあります。 これで証明は完了です。

$\mathfrak{B}_i$ を $Y_i (i \in I)$ のトポロジーのベースとします。 $\mathscr{S}'$ は、$i \in I$ については $\overline{f}_i^{-1}(U_i)$、各 $i \in I$ については $U_i \in \mathfrak{B}_i$ という形式の $X$ の部分集合の集合を表すものとします。 $\mathfrak{B}'$ が $\mathscr{S}'$ の集合の有限交差の集合である場合、$\mathfrak{B}'$ がトポロジー $\mathfrak{T}$ の基底であることは明らかです。

初期構造 (集合理論、章 IV, § 2, no. 3、基準 CST 10) の一般的な特性は、特に次の推移性性質 (その直接の証明は非常に簡単です) を意味します。

#### 命題 5 {#top-i-s2-prop-5 .statement tag=0B0J}

$X$ を集合、$(Z_i)_{i \in I}$ をトポロジカル空間のファミリー、$(J_\lambda)_{\lambda \in L}$ 分割の $I$、および $(Y_\lambda)_{\lambda \in L}$ を $L$ でインデックス付けされた集合のファミリーとします。 また、それぞれの $\lambda \in L$ について、$h_\lambda$ を $X$ の写像を $Y_\lambda$ にします。それぞれの$\lambda \in L$とそれぞれの$i \in J_\lambda$について、$g_{i\lambda}$を$Y_\lambda$の写像として$Z_i$に入れ、$f_i = g_{i\lambda} \circ h_\lambda$を代入します。 各 $Y_\lambda$ が写像 $g_{i\lambda} (i \in J_\lambda)$ が連続する最も粗い位相を保持する場合、$f_i$ が連続する $X$ の最も粗い位相は、$h_\lambda$ が連続する最も粗い位相と同じになります。

#### 例 1 {#top-i-s2-n3-exa-1 .statement tag=0B0K}

位相中逆像。 $X$ を集合、$Y$ をトポロジー 空間、$f$ 写像を $X$ から $Y$ にするとします。 $f$ が連続である $X$ 上の最も粗い位相 $\mathfrak{T}$ は、$Y$ の位相の $f$ の下で逆像と呼ばれます。 命題 4 と、和集合と交差の逆像の公式 [集合論、R、§ 4、式 (34) と (46)] から、トポロジー $\mathfrak{T}$ の開いた (それぞれ閉じた) 集合は、$Y$ の開いた (それぞれ閉じた) 集合の $f$ の下での逆像であることがわかります。その結果、各 $x \in X$ について、$W$ が $Y$ の $f(x)$ の基本近傍系を実行する集合 $f^{-1}(W)$ は、トポロジー $\mathfrak{T}$ の $x$ の基本近傍系を形成します。 § 3 では、誘導位相の名の下に、$X$ が $Y$ の部分集合であり、$f$ が標準単射 $X \to Y$ である特定のケースを研究します。 $X$ は、誘導された位相とともに、$Y$ の部分空間と呼ばれます。

位相空間 $X$ の位相空間 $X'$ への写像 $f$ が連続的であるためには、 $X$ のトポロジーが $X'$ のトポロジーの $f$ の下での逆像よりも細かいことが必要かつ十分です。

#### 例 2 {#top-i-s2-n3-exa-2 .statement tag=0B0L}

集合のトポロジーのうち最小の上界。 集合 $X$ のトポロジーの各ファミリー $(\mathfrak{T}_i)_{i \in I}$ は、$X$ のすべてのトポロジーの順序付けられた集合に少なくとも上界 $\mathfrak{T}$ を持ちます。つまり、$X$ にはすべてのトポロジーの中で最も粗い位相が存在します。 $X$は、それぞれの$\mathfrak{T}_i$よりもより細かいです。これを確認するには、$Y_i$ を集合 $X$ とし、位相 $\mathfrak{T}_i$ とし、$f_i$ を恒等式写像 $X \to Y_i$ として、命題を適用する 4 とします。 $\mathfrak{T}$ は最も粗い位相であり、すべての写像 $f_i$ は連続です。

$\mathfrak{S}$ を集合 $X$ の部分集合の任意の集合とします。 $\mathfrak{S}$ の集合が開いている $X$ 上のトポロジ $\mathfrak{T}$ の中には、他のすべてよりも粗い $\mathfrak{S}$ によって生成された位相と呼ばれる位相 $\mathfrak{T}_0$ があります。それぞれの集合 $U \in \mathfrak{S}$ について、$\mathfrak{T}_U$ を位相とし、そのオープン集合は $\varnothing, U$ と $X$ です [この $X$ の部分集合の集合は (O_I) と(O_{II})];この場合、$\mathfrak{T}_0$ は、トポロジ $\mathfrak{T}_U$ の最小の上界にすぎません。 命題 4 により、$\mathfrak{B}$ が集合所属 ～ $\mathfrak{S}$ の有限共通部分の集合である場合、$\mathfrak{B}$ は位相 $\mathfrak{T}_0$ の基底になります。 $\mathfrak{S}$ は $\mathfrak{T}_0$ の部分基底であると言います。

#### 例 3 {#top-i-s2-n3-exa-3 .statement tag=0B0M}

積位相。 $(X_i)_{i \in I}$ をトポロジー 空間の族とする。 射影 $\mathrm{pr}_i : X \to X_i$ が連続写像である積集合 $X = \prod_{i \in I} X_i$ 上の最も粗い位相は、$X_i$ のトポロジーの *積* と呼ばれます。でさらに詳しく勉強します

### 4. 最終的なトポロジ

#### 命題 6 {#top-i-s2-prop-6 .statement tag=0B0N}

*$X$ を集合とし、$(Y_i)_{i \in I}$ をトポロジカル空間の族とし、それぞれの $i \in I$ について、$f_i$ を $Y_i$ の写像から$X$ にします。 $\mathscr{D}$ を部分集合の集合 $U$ $X$ として、$i \in I$ ごとに $Y_i$ に$\overline{f}_i^{-1}(U)$ がオープンになるようにします。すると、$\mathscr{D}$は、$X$の$\mathfrak{T}$、$X$の位相のオープン部分集合の集合で、家族$(f_i)$（集合）の$X$の最後の構造になります理論、章 IV, § 2, no. 5)、特に$\mathfrak{T}$は写像 $f_i$が連続する$X$の最高級位相です。他の語では、$g$ が $X$ の写像をトポロジー 空間 $Z$ に変換した場合、$g$ は連続です ($X$ は位相 $\mathfrak{T}$ を運びます)。 写像 $g \circ f_i$ は連続です。*

$\mathscr{D}$ が公理 $(O_I)$ および $(O_{II})$ を満たすことがすぐに検証されます。 [集合理論、R、§ 4、式(34)および(46)]。最終的な構造 (集合理論、章 IV, § 2, no. 5、基準 CST 18) の理由により、他の主張を意味する命題の最後の主張を証明します。 $\mathscr{D}$ (no. 1, 定理 1) の定義により、$f_i$ が位相 $\mathfrak{T}$ で連続していることは明らかです。したがって、$g$ が連続であれば、それぞれの写像 $g \circ f_i$ (no. 1, 定理 2) も連続です。逆に、各 $g \circ f_i$ が連続であると仮定し、$V$ を $Z$ のオープン集合とします。 仮定まで、$\overline{f}_i^{-1}(\overline{g}^{-1}(V))$はそれぞれ$i \in I$の$Y_i$にオープンします。したがって、$\overline{g}^{-1}(V) \in \mathscr{D}$、そして証明が完了します。

#### 系 {#top-i-s2-n4-cor-1 .statement tag=0B0O}

*命題 6 の仮説の下では、$\overline{f}_i^{-1}(F)$ が各 $i \in I$ に対して $Y_i$ で閉じられる場合に限り、$X$ の部分集合 $F$ は位相 $\mathfrak{T}$ で閉じられます。

これは、補数を取ることで、位相 $\mathfrak{T}$ のオープン集合の定義から続きます。

最終的な構造 (集合理論、章 IV, § 2, no. 5、基準 CST 19) の一般特性は、次のことを意味します *推移性* 性質 (その直接の証明も簡単です):

#### 命題 7 {#top-i-s2-prop-7 .statement tag=0B0P}

*$X$ を集合、$(Z_i)_{i \in I}$ をトポロジカル空間のファミリー、$(J_\lambda)_{\lambda \in L}$ 分割の $I$、$(Y_\lambda)_{\lambda \in L}$ を $L$ でインデックス付けされた集合のファミリーとします。また、それぞれの $\lambda \in L$ について、$h_\lambda$ を $Y_\lambda$ の写像から $X$ にします。それぞれの$\lambda \in L$とそれぞれの$i \in J_\lambda$について、$g_{\lambda i}$を$Z_i$の写像として$Y_\lambda$に入れ、$f_i = h_\lambda \circ g_{\lambda i}$を代入します。それぞれの $Y_\lambda$ が写像 $g_{\lambda i} (i \in J_\lambda)$ が連続する最高の位相を保持する場合、$f_i$ が連続する $X$ の最高の位相は、$h_\lambda$ が連続する最高の位相と同じになります。

例

1) 商位相。 $X$ を、関係 $R$, $\varphi : X \to Y$ に対する $X$ の $X$, $Y = X/R$ 商集合のトポロジカル空間, $R$ 同値関係とします。 標準写像。 $\varphi$が連続する$Y$の最高の位相は、関係$R$によって$X$の位相の商と呼ばれます。 § 3 で詳しく学びます。

2) トポロジーの最大の下界の集合。 集合 $X$ のトポロジーのすべてのファミリー $(\mathfrak{T}_i)_{i \in I}$ は、$X$ のすべてのトポロジーの集合に最大の下界 $\mathfrak{T}$ を持っています。つまり、$\mathfrak{T}$ は、それぞれより粗い $X$ のすべてのトポロジーの中で最も細かいものです。 $\mathfrak{T}_i$。 これを確認するには、$Y_i$ を集合 $X$ に位相 $\mathfrak{T}_i$ を加えて命題を適用する 6 とし、$f_i$ を恒等写像 $Y_i \to X$ とします。 $\mathscr{D}_i$ が位相 $\mathfrak{T}_i$ にオープンしている $X$ の部分集合の集合である場合、集合 $\bigcap_{i \in I} \mathscr{D}_i$ は$X$ にオープンしている部分集合の集合です$\mathfrak{T}$。 $\mathfrak{T}$ は、トポロジー $\mathfrak{T}_i$ の共通部分とも呼ばれます。

3) トポロジカル空間の和。 $(X_i)_{i \in I}$ を、$X_i$ (集合理論, 章 II, § 4, no. 8, 定義 8) の和であるトポロジカル空間, $X$ 集合の族とします。それぞれの $i \in I$ について、$j_i$ を $X_i$ から $X$ への正規 (単射法) 写像とします。 写像 $j_i$が連続する$X$上の最も細かい位相 $\mathfrak{T}$を$X_i$のトポロジーの和と呼び、これに位相を加えた$X$をトポロジーの和と言います空間 $X_i$。 $j_i$ を使って、$X$ の部分集合と $X_i$ をそれぞれ同一視するしましょう。その場合、集合 $A \subset X$ は位相 $\mathfrak{T}$ で開いています (それぞれ閉じています)。 集合 $A \cap X_i$ が $X_i$ で開いている (それぞれ閉じています) 場合に限ります。特に、$X_i$ はそれぞれ開いているものと閉じているものの両方があります。

次の命題は、例 3 の状況を一般化したものです。

#### 命題 8 {#top-i-s2-prop-8 .statement tag=0B0Q}

$X$を集合、$(X_\lambda)_{\lambda \in L}$を$X$の部分集合の家族とします。それぞれの $X_\lambda$ が位相 $\mathfrak{T}_\lambda$ を運び、添字 $(\lambda, \mu)$ のそれぞれの対について:
1) $X_\lambda \cap X_\mu$ は、各トポロジー $\mathfrak{T}_\lambda, \mathfrak{T}_\mu$ でオープン (それぞれクローズ) です。
2) $\mathfrak{T}_\lambda$ および $\mathfrak{T}_\mu$ 一致するによって $X_\lambda \cap X_\mu$ に誘導されたトポロジー。 単射 $j_\lambda : X_\lambda \to X$ が連続する $X$ 上の最高の位相を $\mathfrak{T}$ とします。次に、それぞれの $\lambda \in L$ では、位相 $\mathfrak{T}$ の $X$ で $X_\lambda$ がオープン (それぞれクローズ) され、位相は $\mathfrak{T}_\lambda$ で $X_\lambda$ 一致するの $\mathfrak{T}$ によって誘導されます。

命題 6 とその系を考慮すると、各 $\lambda$ と $X_\lambda$ の各部分集合 $A_\lambda$ について、次の主張が同等であることを示すだけで十分です。
(i) 位相 $\mathfrak{T}_\lambda$ では、$A_\lambda$ は開いています (それぞれ閉じています)。
(ii) 各$\mu \in L$、$A_\lambda \cap X_\mu$ は、位相 $\mathfrak{T}_\mu$ で開いています (それぞれ閉じています)。

$\mu = \lambda$ を取ることで (ii) が (i) を暗示していることは明らかです。逆に、(i) が満たされる場合、$\mathfrak{T}_{\lambda}$ によって $X_{\lambda} \cap X_{\mu}$ に誘導された位相 $\mathfrak{T}_{\lambda \mu}$ では、$A_\lambda \cap X_\mu$ は $X_\lambda \cap X_\mu$ でオープン (それぞれクローズ) になります。しかし、$\mathfrak{T}_{\lambda \mu}$は$\mathfrak{T}_{\mu}$によって$X_{\lambda} \cap X_{\mu}$に位相も誘発されます。したがって、$A_{\lambda} \cap X_{\mu}$ は、$X_{\lambda} \cap X_{\mu}$ の共通部分と、$X_{\mu}$ の部分集合 $B_{\mu}$ が位相 $\mathfrak{T}_{\mu}$ に開いています (それぞれ閉じています)。 $X_{\lambda} \cap X_{\mu}$は$\mathfrak{T}_{\mu}$に開いている(それぞれ閉じている)ため、$A_{\lambda} \cap X_{\mu}$も同様です。これで証明は完了です。

$X_{\lambda}$ の和集合が $X$ と異なる場合、$X - \left( \bigcup_{\lambda \in L} X_{\lambda} \right)$ 上の $\mathfrak{T}$ によって誘起される位相は *離散* であることに注意してください。たとえば、$x \in X$ 属するが $X_{\lambda}$ のどれにも当てはまらない場合、$\{ x \} \cap X_{\lambda} = \varnothing$ はそれぞれの位相 $\mathfrak{T}_{\lambda}$ でオープンになり、したがって $\{ x \}$ は位相 $\mathfrak{T}$ でオープンになります。

### 5. トポロジカル空間の貼り合わせ

$(X_{\lambda})_{\lambda \in L}$ を集合の族とし、$X$ を $X_{\lambda}$ (*集合理論*, 章 II, § 4, no. 8, 定義 8) の *和* である集合とします。 標準単射 $j_{\lambda} : X_{\lambda} \to X$ を使って、$X$ の部分集合をそれぞれ $X_{\lambda}$ 同一視するにします。

$R$ を $X$ の同値関係として、* $R$ の *それぞれの同値類が *それぞれ* $X_{\lambda}$ に最大 1 つの元を持つようにします。 添字 $(\lambda, \mu)$ のそれぞれ対に対して、 $A_{\lambda \mu}$ を $X_{\lambda}$ の部分集合元 $x$ のからなるとし、元 $y \in X_{\mu}$ と属するを計算します。 $X$中同値類。明らかに、それぞれの $x \in A_{\lambda \mu}$ 対応するは、$x$ mod $R$ と一致する固有の $y \in A_{\mu \lambda}$ です。 写像 $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ は次のように定義されています満たす次の条件:

(i) それぞれの $\lambda \in L$ について、$h_{\lambda \lambda}$ は $A_{\lambda \lambda} = X_{\lambda}$ の恒等写像です。

(ii) $L$ の添字 $(\lambda, \mu, \nu)$ と各 $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$ の各トリプルには、$h_{\mu \lambda}(x) \in A_{\mu \nu}$ があり、

$$
h_{\nu \lambda}(x) = h_{\nu \mu}(h_{\mu \lambda}(x)).
$$

*逆に*、添字 $(\lambda, \mu)$ の各対に対して、$X_{\lambda}$ と写像 $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ 満たす条件の (i) と (ii) の部分集合 $A_{\lambda \mu}$ が与えられるとします。まず、(ii) トリプル $(\lambda, \mu, \lambda)$ と $(\mu, \lambda, \mu)$ に適用されることから、$h_{\lambda \mu} \circ h_{\mu \lambda}$ (それぞれ $h_{\mu \lambda} \circ h_{\lambda \mu}$) は、$h_{\lambda \lambda}$ (それぞれ $h_{\mu \mu}$) から $A_{\lambda \mu}$ (それぞれ $A_{\mu \lambda}$) の制限であることがわかります。したがって、(i) から、$h_{\lambda \mu}$ と $h_{\mu \lambda}$ は、互いに逆数である *全単射* であると推定されます。さて、$R \{ x, y \}$を関係とします。「$x \in A_{\lambda \mu}$、$y \in A_{\mu \lambda}$、$y = h_{\mu \lambda}(x)$のような$\lambda, \mu$が存在します」。 (i) とその前の内容から、$R$ は *再帰的* かつ *対称的 * であることがわかります。一方、$x \in A_{\lambda \mu}$ の場合、

$$
y = h_{\mu \lambda}(x) \in A_{\mu \lambda} \cap A_{\mu \nu} \quad \text{and} \quad z = h_{\nu \mu}(y),
$$

次に、$x = h_{\lambda \mu}(y)$ もあり、したがって (ii) により、$x \in A_{\lambda \mu} \cap A_{\lambda \nu}$;したがって、関係 (i) は、$R$ が *推移的* であること、したがって $R$ は $X$ 上の同値関係であることを示しています。また、(i) と $R$ の定義から、各同値類 mod $R$ のそれぞれの集合 $X_\lambda$ には最大 1 つの元が含まれ、$A_{\lambda \mu}$ はすべての $x \in X_\lambda$ の集合であることがわかります。 $x$ mod $R$ に合同な元 $y \in X_\mu$ があります。 商集合 $X/R$ は、$X_\lambda$ を *$A_{\lambda \mu}$ に沿って * 全単射* $h_{\mu \lambda}$ によって *貼り付けることによって得られると言います。 $\varphi : X \to X/R$ が標準写像の場合、各 $X_\lambda$ に対する $\varphi$ の制限は、$\varphi(X_\lambda)$ への $X_\lambda$ の *全単射* です。

ここで、それぞれの $X_\lambda$ が *トポロジー 空間* であると仮定し、$\mathfrak{T}_\lambda$ をその位相とします。 写像 $\varphi \circ j_\lambda$ が連続する集合 $X/R$ 上の最高の位相を $\mathfrak{T}$ とします。 $\mathfrak{T}$ は、トポロジー $\mathfrak{T}_\lambda$ の *和* である $X$ 上の位相の $R$ による商です。 We say that the topological 空間 $X/R$ (with 位相 $\mathfrak{T}$) is obtained by *pasting together the topological 空間* $X_\lambda$ *along the* $A_{\lambda \mu}$ *by means of 全単射* $h_{\mu \lambda}$. The *open* (resp. *closed*) 部分集合 of $X/R$ are thus 標準像 of 部分集合 $B$ of $X$ which are *saturated* with respect to $R$ and are such that $B \cap X_\lambda$ is *open* (resp. *closed*) $\lambda \in L$ごとに$X_\lambda$に。

Since 制限 of $\varphi$ to each $X_\lambda$ is 全単射 onto 部分集合 $X'_\lambda = \varphi(X_\lambda)$ of $X/R$, we can 輸送位相 $\mathfrak{T}_\lambda$ to $X'_\lambda$ by means of this 全単射、つまり $X'_\lambda$ は位相 $\mathfrak{T}'_\lambda$ を運びます。 $X/R$ の位相 $\mathfrak{T}$ は、標準単射 $X'_\lambda \to X/R$ が連続する *最高* です。一般に、$X'_\lambda$ で $\mathfrak{T}$ によって引き起こされる位相は、$\mathfrak{T}'_\lambda$ よりも *粗い* ですが、後者と同一ではありません。たとえ $h_{\mu \lambda}$ が同相同型 (§ 3, 練習問題 15) であっても。ただし、no. 4、命題 8 から、その前の記法と合わせて次のことがわかります。

#### 命題 9 {#top-i-s2-prop-9 .statement tag=0B0R}

** $h_{\mu \lambda}$ * が同相写像であり、それぞれ* $A_{\lambda \mu}$ * が * $X_\lambda$ で * 開いている (それぞれ閉じている)* と仮定します。 *then each* $\varphi(X_\lambda)$ *is open (resp. closed)* *in* $X/R$ *and 制限 of* $\varphi$ *to* $X_\lambda$ *is a homeomorphism of* $X_\lambda$ *onto 部分空間* $\varphi(X_\lambda)$ *of* $X/R$。

### 練習問題 {#top-i-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
