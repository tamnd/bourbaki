---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 3
section_title: Uniform structures on groups
lang: ja
source: top-i-iv
book_pages: 242-250, 306-307
pdf_pages: 0248-0256, 0312-0313
extraction: ocr
subsections:
    - "no": 1
      title: THE RIGHT AND LEFT UNIFORMITIES ON A TOPOLOGICAL GROUP
      page: 242
      pdf_page: 248
    - "no": 2
      title: UNIFORMITIES ON SUBGROUPS, QUOTIENT GROUPS AND PRODUCT GROUPS
      page: 244
      pdf_page: 250
    - "no": 3
      title: COMPLETE GROUPS
      page: 245
      pdf_page: 251
    - "no": 4
      title: COMPLETION OF A TOPOLOGICAL GROUP
      page: 246
      pdf_page: 252
    - "no": 5
      title: UNIFORMITY AND COMPLETION OF A COMMUTATIVE TOPOLOGICAL GROUP
      page: 248
      pdf_page: 254
statements: 18
exercises: 12
content_sha256: 45c62c807c8fdf9c74f3d1aed027f140bd5d18e45769f2be81041ba4471f0ce4
translated_from: content/en/top/III/03_s3_uniform_structures_on_groups.md
translation_method: google
source_content_sha256: ccad26133e828ceb3575a2c0a99aca5048899ccdf5ec5a7789d9d8ec80447527
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f66319f040d47ef028ed9d786e59dec2f7a68bef35edc18fc368217801a5d96f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 群のユニフォーム構造

### 1. トポロジカル群上の左右の均一性

トポロジカルな群 G では、次のように操作することで、「点に十分に近い」概念を定義する可能性、したがって一様な構造を定義することができます。x と y が G の任意の 2 つの点である場合、それらの 1 つ、たとえば x を送信する変換を両方の点に適用します。 単位元 e; x と y の「近接性」は、y が変換された e の近傍 V によって、ある意味で評価されます。 x と y の両方に $x^{-1}$ を乗算するこの変換は、右側でも左側でも実行できます。どちらの場合でも、G の位相と互換性のある G 上の均一性が効果的に得られることがわかります。変換が右側で実行される場合を考えてみましょう。次に、e の各近傍 V に対応する集合 $V_d$ の対 $(x, y) \in G \times G$ があり、$yx^{-1} \in V$ になります。 V が e の近傍フィルター $\mathfrak{B}$ を通過するため、$\mathfrak{G}_d$ を集合 $V_d$ のファミリーとします。次に、$\mathfrak{G}_d$ は側近の基本系 (章 II, § 1, no. 1) です。 $e \in V$ 以降、$G \times G$ の対角線 $\Delta$ は各 $V \in \mathfrak{B}$ の $V_d$ に含まれるため、$\mathfrak{G}_d$ はフィルター 基底となり、公理 $(U'_1)$ を満たします。 関係 $yx^{-1} \in V$ と $xy^{-1} \in V^{-1}$ は等しいので、$\overline{V}_d^1 = (V^{-1})_d$ があり、したがって (GV$_{\text{II}}$) によって $\overline{V}_d^1 \in \mathfrak{G}_d$ が得られ、(U'$_{\text{II}}$) が満たされます。そして最後に、関係 $zx^{-1} \in V$ と $yz^{-1} \in V$ は $yx^{-1} \in V.V$ を暗示します。したがって、$V_d \circ V_d$ は (V.V)$_d$ に含まれており、(GV$_{\text{I}}$) は、$\mathfrak{G}_d$ が (U'$_{\text{III}}$) を満たすことを示しています。

$\mathfrak{G}_d$ によって定義される均一性は、G の位相と互換性があります。関係 $y \in V_d(x)$ と $y \in V.x$ は定義と同等です。その他語 $V_d(x) = V.x$ で。

翻訳が左側にある場合もこの議論は類似しているため、次の定義を行うことができます。

#### 定義 1 {#top-iii-s3-def-1 .statement tag=0BJX}

*The right (resp. left) uniformity on a topological group G is the uniformity for which a fundamental system of entourages is obtained by making correspond to each neighbourhood V of the identity element e, the set V$_d$ (resp. V$_s$) of pairs $(x, y)$ such that $yx^{-1} \in V$ (resp. $x^{-1}y \in V$).*

V が e の近傍の基本系を通過する場合、集合 V$_d$ (それぞれ V$_s$) 形右 (それぞれ左) の均一性の側近の基本系です。

ユニフォーム空間の位相の各命題に、群の位相に対応する命題がいます。変換は、定義 1 と、定義の明らか帰結である式 $V_d(x) = V.x,\ V_d(A) = V.A,\ V_s(x) = x.V,\ V_s(A) = A.V,$ に従って行われます。たとえば、A が G の空でない部分集合である場合、(章 II, § 1, no. 2, 系 1 ～ 命題 2) となります。

$$
\overline{A} = \bigcap_{V \in \mathfrak{B}} V.A = \bigcap_{V \in \mathfrak{B}} A.V.
$$

繰り返します (章 II, § 1, no. 2、系 3 から命題 2)、*すべてのハウスドルフ群は通常です*。

トポロジカル群上の左右の均一性は、一般に異なります (練習問題 4 を参照)。明らかに、群が *可換* であれば、$V_d = V_s$ なので、一致するになります。また、群が *コンパクト* (章 II, § 4, no. 1, 定理 1) の場合、それらは一致するになります。

一般に、集合 G に左 (または右) の均一性を与えることによって得られる *均一な空間* を $G_s$ (または $G_d$) で表すことにします。

#### 命題 1 {#top-iii-s3-prop-1 .statement tag=0BJY}

*左と右の変換は、それ自体に対する右の均一性の同型です。*

正しい翻訳に関しては、関係 $yx^{-1} \in V$ は $(ya)(xa)^{-1} \in V$ と同等であるため、結果は明らかです [他の語、写像 $(x, y) \to (xa, ya)$ は $V_d$ 固定のままです]。左の翻訳の場合、結果は $(GV_{\text{III}})$ に従います。 $yx^{-1} \in V$ については、$(ay)(ax)^{-1} \in aV a^{-1}$ の場合に限ります。したがって、$x \to ax$ は $G_d$ 上で一様連続です。

同様に、右と左の変換は、それ自体に対する左の均一性の同型です。

したがって、$G$ のすべての *内部自己同型* $x \to axa^{-1}$ は、$G$ の群構造、$G$ の位相、および $G$ の両方の均一性に対して自己同型になります。

#### 命題 2 {#top-iii-s3-prop-2 .statement tag=0BJZ}

*対称* $x \to x^{-1}$ *右の均一性の同型と左の均一性です。*

これは定義 1 の明らか帰結です。

読者は、一様空間 $G_d \times G_d$ から一様空間 $G_d$ への写像 $(x, y) \to xy$ が一般に一様連続であると仮定することに注意してください。同様に、$G_d$ に対する $G_d$ の写像とみなされる対称性 $x \to x^{-1}$ は、一般に均一に連続していません (練習問題 3 および 4 を参照)。

#### 命題 3 {#top-iii-s3-prop-3 .statement tag=0BK0}

*位相的群* $G$ *位相的群* $G'$ *すべての連続準同型* $f$ *は、* $G_d$ * $G'_d$ *(または* $G_s$) の写像とみなした場合、一様連続です。 *に* $G'_s$)。

なぜなら、$V'$ が $G'$ および $V = \overline{f}^{-1}(V')$ の単位元の近傍である場合、関係 $yx^{-1} \in V$ は次のことを意味します。
$$
f(y)(f(x))^{-1} = f(yx^{-1}) \in V'.
$$

### 2. 部分群、剰余群、積群の均一性

$H$ がトポロジー 群 $G$ の部分群である場合、$G$ の正しい均一性によって $H$ に誘発される均一性は、トポロジー 群 $H$ の正しい均一性に他なりません。

$H$ が $G$ の通常の部分群であり、$\varphi$ が $G/H$ 上の $G$ の標準写像である場合、それぞれを関連付けることにより、剰余群 $G/H$ の正しい均一性の側近の基本系が得られます。 近傍 $G$ の単位元の $V$、すべての対の集合 $G/H$ の $(\dot{x}, \dot{y})$ は、$\dot{x}\dot{y}^{-1} \in \varphi(V)$ (§ 2, no. 6、命題 17) になります。 This condition means that there is at least one point $x \in \dot{x}$ and at least one point $y \in \dot{y}$ such that $yx^{-1} \in V$ [i.e. such that $(x, y) \in V_d$]. 特に、$N$ が $G$ の部分集合 $\{e\}$ の閉包である場合、$G/N$ の右一様性は、$G$ (cf. 章 II, § 3, no. 8) の右一様性と *付随した* ハウスドルフ一様性と同型です。

最後に、トポロジカル群の族 $(G_i)$ の積では、右一様性は $G_i$ (cf. 章 II, , no. 6) の右一様性の *積* です。

左の均一性についても同様の結果があります。

積群 $\prod_{i \in I} G_i$ の左右の均一性は、各因子 $G_i$ 一致するの左右の均一性が同じである場合にのみ同一になります。 $G_i$ の一部が可換で、その他がコンパクトな場合、これは常に当てはまります。

### 3. 群を完了する

#### 定義 2 {#top-iii-s3-def-2 .statement tag=0BK1}

*トポロジー 群は、その左右の均一性が完全空間の構造である場合に完全であると言われます。*

no. 1の命題 2から、群が完全であるためには、その均一性の*1*が完全な空間の構造であれば十分です。 $G$ は、関連するハウスドルフ群 ($§\ 2$、no. 6) が完了した場合にのみ完了します。

完全な群のすべての *クローズ済み* 部分群が完了します (章 II, § 3, no. 4、命題 8)。完了した群のすべての積が完了しました (章 II, § 3, no. 5、命題 10)。

一方、$G$ が完全な群で、$H$ が $G$ の閉じた法線部分群である場合、剰余群 $G/H$ は必ずしも完全ではありません (ただし、章 IX, § 3, no. 1、命題 4 を参照)。

#### 命題 4 {#top-iii-s3-prop-4 .statement tag=0BK2}

*トポロジー 群 $G$ において、右または左の一様性に関して完全な $e$ の近傍 $V$ が存在する場合、$G$ は完全です。

たとえば、$V$ が正しい均一性に関して完全であると仮定し、$\mathfrak{F}$ を $G_d$ のコーシー フィルターとします。その場合、$\mathfrak{F}$ 含むは $V_d$-小さい集合 $M$ となり、$x_1 \in M$ であれば、$M \subset Vx_1$ になります。したがって、$G_d$ の完全な部分空間 $Vx_1$ 上の $\mathfrak{F}$ のトレースはコーシー フィルターであり、点 $x_0$ に収束します。 $x_0$ は $\mathfrak{F}$ のクラスター 点であるため、$\mathfrak{F}$ の極限 (章 II, § 3, no. 2、系 2 ～ 命題 5) です。

#### 系 1 {#top-iii-s3-prop-4-cor-1 .statement tag=0BK3}

*ローカルコンパクト群が完了しました。*

すべてのコンパクト空間は、その固有の均一性に関して完全です (章 II, § 4, no. 1、定理 1)。

#### 系 2 {#top-iii-s3-prop-4-cor-2 .statement tag=0BK4}

*ハウスドルフ トポロジカル群 $G$ の局所的にコンパクトなすべての部分群は $G$ で閉じられます。*

ハウスドルフのユニフォーム部分空間が完了するたびに、空間が閉じられます (章 II、 、no. 4、命題 8)

#### 命題 5 {#top-iii-s3-prop-5 .statement tag=0BK5}

$G_1$ を位相位相群とし、$G_2$ を完全なハウスドルフ位相位相群とし、$H_1$ (それぞれ $H_2$) を $G_1$ (それぞれ $G_2$) の密集部分群とします。次に、$H_1$ から $H_2$ へのすべての連続準同型 $u$ は、$G_1$ から $G_2$ への連続準同型 $\bar{u}$ に一意に拡張できます。さらに、$G_1$ がハウスドルフで完全であり、$u$ が $H_2$ 上の $H_1$ の同型である場合、$\bar{u}$ は $G_2$ 上の $G_1$ の同型です。

$\bar{u}$ は、$H_1$ と $H_2$ (no. 1、命題 3) の正しい均一性に関して一様連続であるため、$G_1$ から $G_2$ への一意の拡大から写像 $\bar{u}$ が認められます。これら群 (章 II, § 3, no. 6、定理 2) の正しい均一性。 さらに、アイデンティティの拡大の原則 (章 I, § 8, no. 1、系 1 から命題 2) により、$\bar{u}$ は $G_1$ の準同型から $G_2$ になり、よっては最初の主張になります。 命題。 2番目の主張を証明するには、$u$の逆である$H_2$の$H_1$への同型$v$と、$G_2$から$G_1$への連続準同型への拡張$\bar{v}$を考慮するだけで十分です。拡張の一意性により、$\bar{v} \circ \bar{u}$ と $\bar{u} \circ \bar{v}$ はそれぞれ $G_1$ と $G_2$ の恒等写像であるため、(集合論、R、§ 2, no. 12) $\bar{u}$ は全単射です。

#### 注意 {#top-iii-s3-n3-rem-1 .statement tag=0BK6}

連続する準同型 $u$ が全単射である場合、一般に $\bar{u}$ が単射または全射であるということにはなりません (cf. 練習問題 12)。ただし、no. 5、命題 9 を参照してください。

### 4. トポロジカル群の完成

$G$ をハウスドルフ トポロジカル群とします。ユニフォーム空間 $G_d$ は、完成した $\hat{G}_d$ の濃厚な部分空間と考えることができます。 $G$ が完全なハウスドルフ群 $G'$ の稠密な部分群とみなせるかどうかを調査します。そうであれば、均一空間 $G'_d$ は $\hat{G}_d$ (章 II, § 3, no. 6、系から定理 2) と同型である必要があり、従って、トポロジカル群構造で $\hat{G}_d$ 上で定義するができなければなりません。 誘導する $G$ 上の指定されたトポロジ群構造。従って、次のことを検討する必要があります。
1) 継続性によって拡大する写像 $xy$ と $x^{-1}$ をそれぞれ $\hat{G}_d \times \hat{G}_d$ と $\hat{G}_d$ にできるかどうか。 2) このように拡張された写像が $\hat{G}_d$ 上で実際に定義する群構造となるかどうか (その場合、$\hat{G}_d$ 上で必然的に定義するトポロジカル群構造となり、$G$ 上で指定された構造を誘導します)。次に、3) 前述の演算が​​可能であれば、それら定義するが含むトポロジー 群が完成することを確立する必要があります。最後に、4) 指定された条件に完全な群満たすがある場合、それは同型まで一意であることがわかります。

1) 連続性による$xy$と$x^{-1}$の拡大。 写像 $xy$ と $x^{-1}$ は一般に一様連続ではないため、できないは一様連続写像 (章 II, § 3, no. 6, 定理 2) の拡大の定理を適用します。それにもかかわらず、章 II, § 3, no. 6 と次の命題の命題 11 のおかげで、拡大する $xy$ を実現できます。

#### 命題 6 {#top-iii-s3-prop-6 .statement tag=0BK7}

$\mathfrak{F}$ と $\mathfrak{G}$ を $G_d$ 上の 2 つの Cauchy フィルターとします。次に、写像 $(x, y) \to xy$ の下にあるフィルター $\mathfrak{F} \times \mathfrak{G}$ の像は、$G_d$ 上の Cauchy フィルター 基底になります。

$G_d$における$xy$と$x'y'$の「近接性」を評価してみましょう。他の語では、形積 $(x'y')(xy)^{-1} = x'y'y^{-1}x^{-1}$ にしましょう。それぞれの $a \in G$ に対して、$(x'y')(xy)^{-1} = (x'a^{-1})(ay'y^{-1}a^{-1})(ax^{-1})$ と書くこともできます。 $a$ の適切な選択によって、この積の 3 つの因子は、対 $(x, y)$ および $(x', y')$ 属するから十分に小さい集合まで非常に小さいことがわかります。 $\mathfrak{F} \times \mathfrak{G}$。 $V$ を $G$ の $e$ のいずれかの近傍とします。次に、$V_d$-小さい集合 $A \in \mathfrak{F}$ があります。 $A$ の選ぶ $a$ の場合、$x$ と $x'$ が $A$ のいずれか 2 つの点である場合、$x'a^{-1} \in V$ と $ax^{-1} \in V$ が得られます。一方、関係 $ay'y^{-1}a^{-1} \in V$ は、
$$
y'y^{-1} \in a^{-1}Va = W,
$$
そして、$W$ は $e$ の近傍であるため、$W_d$ の小さい集合 $B \in \mathfrak{G}$ が存在します。従って、$A \times B$ のすべての $(x, y)$ と $(x', y')$ に対して、$(x'y')(xy)^{-1} \in V^3$ があり、これで証明が完成します。

位数では、$x^{-1}$ が連続性によって $\hat{G}_d$ まで拡張できるということは、$G_d$ 上のコーシー フィルターの *像が、対称性* $x \to x^{-1}$ の下で、$G_d$* (章 II, § 3, no. 6, 命題 11）。この条件が満たされない位相幾何学群の例があります (cf. 章 X, § 3, 練習問題 16)。この証明の残りの部分は満たされていると仮定します。

2) *拡張写像* $xy$ および $x^{-1}$ *定義する群構造を * $\hat{G}_d$ に拡張します。なぜなら、恒等式の拡大の原則 (章 I, § 8, no. 1、命題 2、系 1) を $\hat{G}_d \times \hat{G}_d \times \hat{G}_d$ で定義され、密な部分空間で等しい写像 $x(yz)$ および $(xy)z$ に適用するとします。 $G_d \times G_d \times G_d$ では、合成 $(x, y) \to xy$ の法則が $\hat{G}_d$ に *結合* していることがわかります。同じ理由で、写像 $x, ex, xe$ は $\hat{G}_d$ で同一であり、写像 $e, xx^{-1}, x^{-1}x$ は $\hat{G}_d$ で同一です。

3) *トポロジカル群* $\hat{G}_d$ *完備*。 $\mathfrak{U}_d$ をその *正しい均一性* とし、$\mathfrak{U}$ を $G$ の正しい均一性を *完成*することによって得られる $\hat{G}_d$ の均一性とします。次に、$\mathfrak{U}$ と $\mathfrak{U}_d$ 誘導するは $G$ で *同じ* 均一性になるため、すべてのコーシー フィルター 基底 $\mathfrak{B}$ *on* $G$ *に関して* $\mathfrak{U}_d$ *は*に関してもコーシー フィルター 基底 $\mathfrak{U}$。 $\mathfrak{U}$ は完全な一様性なので、$\mathfrak{B}$ は $\hat{G}_d$ に収束します。そして、$\mathfrak{U}$ と $\mathfrak{U}_d$ 誘導するは $\hat{G}_d$ の位相と同じであるため、(章 II, , no. 4, 命題 9) $\mathfrak{U}_d$ は完全な一様性であることがわかります。この結論は、$\mathfrak{U}$ と $\mathfrak{U}_d$ 一致する (章 II, § 3, no. 6、系から定理 2) も示しています。

4) *一意性.* これは、no. 3 の命題 5 から続きます。

和までに、次の定理を証明しました。

#### 定理 1 {#top-iii-s3-thm-1 .statement tag=0BK8}

*ハウスドルフ トポロジカル群 $G$ は、$G$ の正しい均一性に関してコーシー フィルターの対称性 $x \to x^{-1}$ の下で、像が完全な群 $\hat{G}$ の密な部分群と同型です。この均一性に。完全な群 $\hat{G}$ (これは $G$ の完了と呼ばれます) は一意になります (同型まで)*。

#### 命題 7 {#top-iii-s3-prop-7 .statement tag=0BK9}

*$G$ を、完備 $\hat{G}$ を持つハウスドルフ トポロジカル群とします。 次に、$G$ の単位要素の近傍の $\hat{G}$ の閉包が、$\hat{G}$ の単位要素の近傍の基本システムを形成します。

$\hat{G}$ は規則的であるため、$\hat{G}$ 含むの単位元の各近傍は、$\hat{G}$ の $e$ のオープン近傍 $U$ の閉鎖 $V$ であり、$V$ は、トレースの閉鎖でもあります。 $G$の$U$。

$G$ を群とします。これは必ずしもハウスドルフではありません。 $N = \overline{\{e\}}$ を、$G' = G/N$ を $G$ (§ 2, no. 6) に関連付けられたハウスドルフ群とします。 $G'$ に補完 $\hat{G}'$ がある場合、この補完は $G$ の *ハウスドルフ補完* と呼ばれ、$\hat{G}$ で示されます。 $\hat{G}'_d$ (それぞれ $\hat{G}'_s$) は、ユニフォーム空間 $G_d$ (それぞれ $G_s$) の *ハウスドルフ完成* (章 II, § 3, no. 7) です。

#### 命題 8 {#top-iii-s3-prop-8 .statement tag=0BKA}

*$G$ を、ハウスドルフ補完 $\hat{G}'$ を持つトポロジカル群とします。 次に、完全なハウスドルフ群 $H$ への $G$ のすべての連続準同型 $u$ は、$u = v \circ \varphi$ に一意に因数分解できます。ここで、$v$ は $\hat{G}'$ から $H$ への連続準同型であり、$\varphi$ は $G$ からの正規写像です。 $\hat{G}'$ ($G'$ の $\hat{G}'$ への正準注入と $G$ の $G/N = G'$ への正準準同型性 $\psi$ の合成)。

$u$ の核が閉じており、含む $e$ なので、含む $N$ となり、$u$ は $u = w \circ \psi$ と書くことができます。ここで、$w$ は $G'$ の連続準同型です。 $H$;現在命題を適用する no. 3 から $w$ の 5 です。

### 5. 可換トポロジーの均一性と完成群

可換位相群 $G$ 上の左右の均一性一致するはすでに述べました。私たちが$G$の*均一性*について話すときは常に、この独特の均一性を指します。

#### 定理 2 {#top-iii-s3-thm-2 .statement tag=0BKB}

$G$ を可換位相ベクトル群とします。次に、写像 $x^{-1}$ と $xy$ はそれぞれ $G$ と $G \times G$ で一様に連続します。さらに、$G$ はハウスドルフ完了 $\hat{G}$ を認め、$\hat{G}$ は可換です。

$x^{-1}$ の一様連続性は no. 1 の命題 2 から続き、$xy$ の一様連続性は no. 1 の命題 3 から続きます。これは、$(x, y) \to xy$ が $G \times G$ から $G$ への連続準同型であるためです。 $G$ がハウスドルフの場合、定理の条件と no. 4 の 1 を満たします (左右の均一性が一致するであるすべてのハウスドルフ群も同様です)。さらに、恒等式の拡大の原則により、写像 $xy$ と$yx$ は$\hat{G} \times \hat{G}$ 上で等しくなります。したがって、一般的なケースでハウスドルフ群が $G$ に関連付けられることを考慮すると、定理の 2 番目の部分になります。

特にこの定理から、$f$と$g$が、一様空間$X$の可換群$G$に加法的に書かれた2つの一様連続写像である場合、写像$-f$となります。 $f + g$ は一様連続です。

#### 命題 9 {#top-iii-s3-prop-9 .statement tag=0BKC}

$G$ を可換群とし、$\mathfrak{T}_1, \mathfrak{T}_2$ を $G$ の群構造と互換性のある 2 つのハウスドルフ トポロジとします。 $\mathfrak{T}_1$が$\mathfrak{T}_2$よりより細かいで、$\mathfrak{T}_1$の$o$の近傍の基本系があり、$\mathfrak{T}_2$にはクローズされているとします。 $G_1, G_2$ をそれぞれトポロジー $\mathfrak{T}_1, \mathfrak{T}_2$ に対する $G$ の完成とし、$f : G_1 \to G_2$ を $G$ の拡大する恒等写像 (no. 3, 命題 5) の連続準同型とします。すると$f$は単射法です。

$G$ が加法的に書かれたとします。 Let $\mathfrak{U}_1$ be the uniformity on $G$ corresponding (no. 1) to the topology $\mathfrak{T}_1$: it will suffice to show that if $\mathfrak{F}$ and $\mathfrak{F}'$ are two minimal Cauchy filters (Chapter II, § 3, no. 2) with respect to $\mathfrak{U}_1$, which converge in $G_2$ to the same point $a$, then $\mathfrak{F} = \mathfrak{F}'$ (Chapter II, § 3, no. 7). このためには、$\mathfrak{F} \cap \mathfrak{F}'$ が $\mathfrak{U}_1$ に関してコーシー フィルターであることを示すだけで十分です。 $V$ を $\mathfrak{T}_1$ に関して $G$ の $o$ の近傍とし、$V$ が $\mathfrak{T}_2$ で閉じられるようにし、$W$ を $G$ に関して対称な $o$ の近傍とします。 $\mathfrak{T}_1$ は $W + W \subset V$ になります。 仮定までに、$\mathfrak{F}$ (それぞれ $\mathfrak{F}'$) に $W_d$-小さい集合 $M$ (それぞれ $M'$) が存在します。 $x \in M$ と $y \in M$ の場合、$y - x \in W$、つまり $y \in x + W$ になります。 $\overline{W}$ と $\overline{V}$ が $G_2$ の $W$ と $V$ の閉包である場合、$y \in x + \overline{W}$ となり、したがって、$a$ は $M$ の閉包内にあるので、各 $x \in M$ に対して $a \in x + \overline{W}$ になります。 同様に、各 $x' \in M'$ に対して $a \in x' + \overline{W}$、したがって $x - x' \in \overline{W} + \overline{W}$;しかし、$(x, y) \to x + y$は$G_2 \times G_2$の$G_2$への連続した写像なので、$\overline{W} + \overline{W} \subset \overline{W} + \overline{W} \subset \overline{V}$になります。 $x \in M$ と $x' \in M'$ の場合、$V$ は $\mathfrak{T}_2$ で閉じているため、$x - x' \in \overline{V} \cap G = V$ になります。これで証明は完了です。

#### 系 1 {#top-iii-s3-prop-9-cor-1 .statement tag=0BKD}

命題 9 の仮説の下で、$A$ が$G$ の部分集合であり、$U_2$ 対応する ～ $\mathfrak{T}_2$ に関して完全な部分空間である場合、$A$ も均一性に関して完全な部分空間です。 $U_1$ 対応するから $\mathfrak{T}_1$ まで。

$A_1$ が $G_1$ の $A$ の閉包である場合、$f(A_1)$ は $G_2$ の $A$ の閉包に含まれており、仮定までに $A$ に等しくなります。 $f(A) = A$ by 定義と $f$ は単射なので、$A_1 = A$ になります。

#### 系 2 {#top-iii-s3-prop-9-cor-2 .statement tag=0BKE}

$G$ を可換な群とし、$\mathfrak{T}_1, \mathfrak{T}_2$ を $G$ の群構造と互換性のある 2 つのトポロジとします。 $\mathfrak{T}_1$ が $\mathfrak{T}_2$ よりもより細かいであり、$\mathfrak{T}_1$ に関して近傍の$O$ の基本系 $\mathfrak{B}$ があり、均一性$U_2$ 対応するに関して完全であると仮定します。 $\mathfrak{T}_2$。次に、$U_1$ 対応するから $\mathfrak{T}_1$ までの均一性に関して $G$ が完成します。

$\mathfrak{B}$ の集合は位相 $\mathfrak{T}_2$ で閉じられているため、系 1 によって$U_1$ の均一性が完了します。したがって、結果は no. 3 の命題 4 から得られます。

### 練習問題 {#top-iii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
