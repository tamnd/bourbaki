---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 6
section_title: Topological groups with operators; topological rings division rings and fields
lang: ja
source: top-i-iv
book_pages: 271-283, 315-324
pdf_pages: 0277-0289, 0321-0330
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS WITH OPERATORS
      page: 271
      pdf_page: 277
    - "no": 2
      title: TOPOLOGICAL DIRECT SUM OF STABLE SUBGROUPS
      page: 272
      pdf_page: 278
    - "no": 3
      title: TOPOLOGICAL RINGS
      page: 274
      pdf_page: 280
    - "no": 4
      title: SUBRINGS; IDEALS; QUOTIENT RINGS; PRODUCTS OF RINGS
      page: 276
      pdf_page: 282
    - "no": 5
      title: COMPLETION OF A TOPOLOGICAL RING
      page: 276
      pdf_page: 282
    - "no": 6
      title: TOPOLOGICAL MODULES
      page: 278
      pdf_page: 284
    - "no": 7
      title: TOPOLOGICAL DIVISION RINGS AND FIELDS
      page: 281
      pdf_page: 287
    - "no": 8
      title: UNIFORMITIES ON A TOPOLOGICAL DIVISION RING
      page: 282
      pdf_page: 288
statements: 24
exercises: 26
content_sha256: ad3009422cd833fb0020a19015ed487382315aac2e6a6e96379841f34a7ea2c9
translated_from: content/en/top/III/06_s6_topological_groups_with_operators.md
translation_method: google
source_content_sha256: bbc4c9265a358c8a03dba09dd6f583c1d3176c59f530f843e58111b9bb22ab18
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 974909e0cd55d360bdda0dcbb5700e107576cacc6aa061528a354d40dc97551a
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 6. 演算子を使用したトポロジカル群;トポロジカル環、分割環および体

### 1. 演算子を使用したトポロジカル群

集合$G$において、$G$のトポロジーと群構造が互換性があり(§ 1, no. 1)、さらに演算子によって生成される$G$の準同型性が連続である場合、演算子を含む群の構造とトポロジーは互換性があると言われます。 集合 $G$ は、演算子付きの群の指定された位相と構造とともに、演算子付きのトポロジカル群であると言われます。

$H$ が演算子を含むトポロジカル群 $G$ の安定な部分群である場合、$G$ の位相によって $H$ に誘導される位相は、$H$ の演算子を含む群の構造と互換性があります。さらに：

#### 命題 1 {#top-iii-s6-prop-1 .statement tag=0BN2}

*$H$ が演算子を含むトポロジカル群 $G$ の安定な部分群である場合、$G$ の $H$ の閉包 $\overline{H}$ は $G$ の安定な部分群です。

$\overline{H}$ が $G$ の部分群であることはすでにわかっています (§ 2, no. 1、命題 1)。また、$\alpha$ が $G$ 上の任意の演算子である場合、連続写像 $x \to x^\alpha$ の下の $H$ の像は $H$ に含まれるため、$\overline{H}$ の像は $\overline{H}$ (章) に含まれます。 I, § 2, no. 1、定理 1)。

$H$ を、演算子を使用したトポロジカル群 $G$ の安定した法線部分群とします。次に、$G$ の各演算子 $\alpha$ について、$x \to x^\alpha$ によって誘導された $G/H$ の写像は連続 (§ 2, no. 8、注意 3) であり、$G/H$ の演算子を持つ群の構造は、次と互換性があります。 $G/H$の商位相。

$(G_i)_{i \in I}$ を演算子を持つトポロジー 群の族とします。ここで、各 $G_i$ は同じ演算子集合 $\Omega$ を持つと仮定します。それぞれの $\alpha \in \Omega$、写像 $G = \prod_{i \in I} G_i$ の $x \to ((\mathrm{pr}_i x)^\alpha)$ は連続しており (章 I, § 4, no. 1、命題 1)、$G$ の演算子を持つ群の構造は積と互換性があります。 $G$の位相。

$G$ が演算子を含むハウスドルフ トポロジ群で、$G$ に補完 $\hat{G}$ (§ 3, no. 4) がある場合、$G$ の演算子によって定義された $G$ のすべての自己準同型 $x \to x^\alpha$ は、連続性によって次のように拡張できます。 $\hat{G}$ の自己準同型 (§ 3, no. 3、命題 5)。したがって、$\hat{G}$ は演算子を備えたトポロジカル群の構造を持ち、演算子集合は $\hat{G}$ についても $G$ と同じです。

### 2. 安定した部分群のトポロジカル直和

演算子を伴う可換群の研究は加群の研究と同等であるため、演算子を伴う任意の可換群に対して加群に適切な用語を使用することをときどきに許可します。したがって、演算子を使用した可換群の準同型の代わりに *線形写像* について話すことができ、演算子を使用した可換群の冪等自己準同型を表すために語 *射影子* を使用することもできます。

演算子 (加法的に書かれた) を伴う可換位相群 $E$ が *有限* 族の直和 $(M_i)_{1 \leq i \leq n}$ の安定な部分群である場合、積群 $\prod_{i=1}^n M_i$ の正規の全単射 $(x_i) \to \sum_{i=1}^n x_i$ は次のようになります。 $E$ は *連続* ですが、*必ずしも同型ではありません*。

#### 定義 1 {#top-iii-s6-def-1 .statement tag=0BN3}

*$E$ を演算子をもつ可換位相群とし、$(M_i)_{1 \leq i \leq n}$ を $E$ が $M_i$ の直和となるように、$E$ の安定な部分群の有限族とする。次に、積群 $\prod_{i=1}^n M_i$ の $E$ に対する標準写像 $(x_i) \to \sum_{i=1}^n x_i$ が同相写像* である場合、$E$ は $M_i$ のトポロジカル直和であると言われます (したがって、トポロジカルの同型 ) 群オペレーター付き)。

#### 命題 2 {#top-iii-s6-prop-2 .statement tag=0BN4}

*$E$ を、安定な部分群 $M_i$ ($1 \leq i \leq n$) の直和である演算子を備えた可換位相幾何学群とします。 $(p_i)_{1 \leq i \leq n}$ を、分解 $E = \sum_{i=1}^n M_i$ に関連付けられた射影子の家族とします。この場合、$p_i$ が連続である場合に限り、$E$ は $M_i$ の位相幾何学的な直和になります。*

写像の場合、$x \to (p_i(x))$ は写像 $(x_i) \to \sum_{i=1}^n x_i$ の逆数です。

$1 = \sum_{i=1}^n P_i$ (ここで、$1$ は $E$ の恒等写像を表します) なので、位数で射影子 $p_i$ の $n - 1$ が連続していれば、$n$ 番目も連続である必要があります。

$E$ が 2 つの安定な部分群 $M, N$ のトポロジカル直和である場合、$N$ は $E$ の $M$ の *トポロジカル補体* であると言われます。これは、$E/M$ の標準写像が演算子を含むトポロジカル群の *同型* である場合にのみ当てはまります。

#### 系 {#top-iii-s6-n2-cor-1 .statement tag=0BN5}

*$E$ を演算子を伴う可換トポロジー 群とし、$M$ を $E$ の安定な部分群とします。したがって、次の条件は同等です:*

a) $M$ は $E$ に位相補数があります。

b) *$E$ から $E$ への連続射影子 $p$ があり、$p(E) = M$ になります。*

c) *$M$の恒等写像は、$E$の連続した線形写像から$M$に拡張できます。*

命題 2 から、a) は b) を意味し、b) は c) を意味することは明らかです。 最後に、$p$ が $E$ の $M$ への連続線形写像で、$M$ の拡大する恒等写像である場合、$p$ は連続射影子、射影子 $p$ であり、 $1 - p$ は直和分解 $E = M + N$ に関連付けられており、$N = \overline{p}(0)$ です。

#### 注意 1 {#top-iii-s6-n2-rem-1 .statement tag=0BN6}

混乱を避けるため、ときどきは、$M$ の補数である $E$ の安定な部分群 (演算子あり、位相なしの群の構造という意味で) は、$M$ の *代数的補数* であるとします。

#### 注意 2 {#top-iii-s6-n2-rem-2 .statement tag=0BN7}

演算子を伴う *ハウスドルフ* 可換位相幾何学群が安定部分群の族 $(M_i)_{1 \leq i \leq n}$ の位相幾何学直和である場合、部分群 $M_i$ のそれぞれは $E$ で *閉じられ*、$M_i$ はすべての集合であるため、 $x \in E$ は $p_i(x) = x$ (章 I, § 8, no. 1, 命題 2) となります。

#### 命題 3 {#top-iii-s6-prop-3 .statement tag=0BN8}

*$E, F$ を演算子をもつ 2 つの可換位相群とし、$u$ を $E$ から $F$ への連続線形写像とする。 位数では、$u \circ v$ が $F$ の恒等写像となるような、$F$ から $E$ への連続した線形写像 $v$ が存在する必要があります (この場合、$u$ は右可逆であると言われ、$v$ は *右であると言われます) $u$ の逆*) $u$ が $F$ に対する $E$ の厳密な射 (§ 2, no. 8) であり、$\overline{u}(0)$ が $E$ にトポロジー的補数を持つことが必要かつ十分です。

条件は*必須*です。 というのは、$u(v(F)) = F$ と *なおさら* $u(E) = F$ があるからです。さらに、$p = v \circ u$ の場合、$p$ は$E$ の連続線形写像であり、$p^2 = p$ になります。したがって (系から命題 2) $p(E) = v(u(E)) = v(F)$ は $E$ に位相補数 $\overline{p}(0)$ を持ちます。しかし、$u(p(x))) = u(x)$から仮定までなので、$\overline{u}(0) = \overline{p}(0)$になります。 最後に、$u$ に関連付けられた $E/\overline{u}(0)$ の $F$ への全単射写像は、$p$ に関連付けられた $E/\overline{u}(0)$ の $v(F)$ への全単射写像と、$u$ から $v(F)$ への制限の合成です。 $v$ は連続であるため、これらの写像は両方とも同型写像であり、したがって、$u$ は $E$ から $F$ への厳密な写像になります。

条件で *十分* です。なぜなら、$\varphi$ が $E/\overline{u}^1(o)$ 上の E の標準準同型である場合、$\overline{u}^1(o)$ が E に位相補数 M を持っているということは、M に対する $\varphi$ の制限が $E/\overline{u}^1(o)$ 上の M の同型であると言うのと同じです。一方、$u = w \circ \varphi$、ここで w は F 上の $E/\overline{u}^1(o)$ の同型であるため、M に対する u の制限は F 上の M の同型であり、したがって逆同型 v は、$u \circ v$ 自体に対する F の恒等写像であることがわかります。

#### 命題 4 {#top-iii-s6-prop-4 .statement tag=0BN9}

*E、F を演算子を持つ 2 つの可換位相群とし、u を E から F への連続線形写像とする。 位数では、$v \circ u$ がそれ自身上で E の恒等写像となるように、F から E への連続線形写像 v が存在する必要がある* (この場合、u は *左可逆* であり、v は a であると言われる) u の *左逆*) *u が u(E) 上の E の (トポロジカルな) 同型であり、u(E) が F でトポロジカルな補数を持つことが必要かつ十分です。*

条件は *十分* です。なぜなら、それらが満たされる場合、u(E) の同型の合成を u の逆数である E に取り込み、u(E) に F の連続射影子を取り込むことによって、u の左逆逆 v を取得します。

条件は*必須*です。 関係 $v(u(x)) = x$ は $\overline{u}^1(o) = \{ o \}$ を示します。したがって、u は u(E) 上の E の全単射であり、v から u(E) への制限は連続であるため、u は u(E) 上の E の同型になります。一方、$q = u \circ v$ を置くと、q は $q^2 = q$ となるような u(E) 上の F の連続線形写像となり、u(E) が F において位相補数を持つことが (系から命題 2) 証明されます。

### 3. トポロジカル環

#### 定義 2 {#top-iii-s6-def-2 .statement tag=0BNA}

*トポロジカル環は、以下の公理環構造および位相満たすを運ぶ集合 A です:*

*(AT$_\mathrm{I}$)*。 *写像* $(x, y) \to x + y$ *of* $A \times A$ *into* A *は連続です*。
*(AT$_\mathrm{II}$)*。 *写像* $x \to -x$ *of* A *into* A *は連続です*。
*(AT$_\mathrm{III}$)*。 *写像* $(x, y) \to xy$ *of* $A \times A$ *into* A *は連続です*。

最初の 2 つの公理は、A の位相がその *加法群* 構造 (§ 1, no. 1) と互換性があることを表します。

環構造と位相が集合 A で与えられた場合、満たすの公理 (AT$_\mathrm{I}$)、(AT$_\mathrm{II}$)、および (AT$_\mathrm{III}$) であれば *互換性がある* と言われます。

#### 例 1 {#top-iii-s6-n3-exa-1 .statement tag=0BNB}

どの環 A でも、*ディスクリート* 位相は環構造と互換性があります。 位相が離散であるトポロジカル環は *離散* 環と呼ばれます。

#### 例 2 {#top-iii-s6-n3-exa-2 .statement tag=0BNC}

章 IV で、有理線 Q (それぞれ実直線 R) の位相が Q (それぞれ R) の環構造と互換性があることがわかります。

位相幾何学的環では、左すべてのホモテティー $x \to ax$ (それぞれ右すべてのホモテティー $x \to xa$) は連続です (そして、$a$ が $A$ の単位元である場合、同相写像です)。

同じように書けるので、
$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0)
$$
公理 (AT_{III}) [(AT_I) と (AT_{II}) を考慮すると] は、次の 2 つの公理の結合と等価です。
(AT_{III a})。 *任意の* $x_0 \in A$、*写像* $x \to x_0 x$ *および* $x \to xx_0$ *は点* $x = 0$で連続します。
(AT_{III b})。 *写像* $(x, y) \to xy$ *of* $A \times A$ *into* $A$ *は点* $(0, 0)$ で連続します。

このことから、環 $A$ の$0$ の近傍のフィルタ $\mathfrak{B}$ は、位数 ～ 定義するの満たすでなければならない条件の必要十分な集合を推定できます。 $A$ 上の位相は、その環構造と互換性があります: $\mathfrak{B}$ は、§ 1 の満たす公理 (GA_I) および (GA_{II})、および次の 2 つの公理を必要とします。
(AV_I)。 *すべて* $x_0 \in A$ *そしてすべて* $V \in \mathfrak{B}$、*存在します* $W \in \mathfrak{B}$ *そのような* $x_0 W \subset V$ *そして* $W x_0 \subset V$。
(AV_{II})。 *すべて* $V \in \mathfrak{B}$、*存在します* $W \in \mathfrak{B}$ *そのような* $WW \subset V$。

#### 注意 {#top-iii-s6-n3-rem-1 .statement tag=0BND}

分析では、満たすの公理 (AT_I)、(AT_{II})、および (AT_{III a}) である環には頻繁に遭遇しますが、(AT_{III b}) には遭遇しません。 *例はコンパクトな群上のメジャーの環で、乗法は畳み込み、位相は曖昧な位相です。*

*例 3).* $\mathfrak{B}$ を、*両面理想* の環 $A$、からなるに対するフィルター 基底とします。 $\mathfrak{B}$ は、$A$ の加法群構造と互換性のある位相の $0$ の近傍の基本的な系であり、(AV_I) と (AV_{II}) からすぐに次のことがわかります。 位相は、$A$ の *環* 構造と互換性があります。

$X$ をトポロジー 空間とし、$f$ と $g$ を $X$ の 2 つの写像としてトポロジー 環 $A$ とします。 $f$と$g$が点$x_0 \in X$で連続している場合、$f + g$、$-f$、$fg$はこの点で連続しています。 その結果、$X$ の連続写像が $A$ 形に、環 $A^X$ の *部分環* が $X$ のすべての写像から $A$ に続きます。 また、$A$ が *可換* である場合、$A$ に係数があり、$A^n$ で定義されている n 個の変数内のすべての *多項式* は、$A^n$ 上で *連続* であることもわかります。 もう一度、$f$ と $g$ を集合 $X$ の 2 つの写像とし、フィルター $\mathfrak{F}$ で *フィルターして * ハウスドルフ* トポロジカル環 $A$ にします。 $\lim_{\mathfrak{F}} f$ と $\lim_{\mathfrak{F}} g$ が存在する場合、$\lim_{\mathfrak{F}} (f + g)$、$\lim_{\mathfrak{F}} (-f)$、$\lim_{\mathfrak{F}} (fg)$ も存在し、(章 I, § 7, no. 4、命題 9、系 1、§ 8, no. 1、命題) が存在します。 1)

(1) $$ \lim_{\mathfrak{F}} (f + g) = \lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g, $$
(2) $$ \lim_{\mathfrak{F}} (-f) = -\lim_{\mathfrak{F}} f, $$
(3) $$ \lim_{\mathfrak{F}} (fg) = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g). $$

### 4. 部分環;理想。 商環; 環中積

$H$ がトポロジー 環 $A$ の部分環である場合、$A$ の$H$ によって誘導された位相は $H$ の環構造と互換性があります。 $H$ でこのように定義されたトポロジカル環構造は、$A$ のトポロジカル環構造によって *誘導*されると言われます。

#### 命題 5 {#top-iii-s6-prop-5 .statement tag=0BNE}

*$H$ をトポロジー 環 $A$ の稠密部分環とし、$K$ を $H$ の部分環 (それぞれ左イデアル、右イデアル、両側イデアル) とします。すると、$A$の$K$の閉包$\overline{K}$は、$A$の部分環(それぞれ左イデアル、右イデアル、両側イデアル)になります。

証明は、§ 2の命題8、nと同じです。 3 : たとえば、$K$ が $H$ の左イデアルである場合、写像 $(z, x) \to zx$ は $A \times A$ および写像 $H \times K$ から $K$ まで連続します。したがって、写像 $A \times K = \overline{H} \times K$ は $\overline{H}$ になります。

$H$ をトポロジカル環 $A$ の *両側* イデアルとします。 剰余群と同じ議論により、関係 $x - y \in H$ による $A$ の位相の *商* は $A/H$ の環構造と互換性があることがわかります。特に、$A$ がハウスドルフでない場合、$A$ における $\{0\}$ の閉包 $N$ は、命題 5 による *閉両側イデアル* になります。ハウスドルフ ($\S$ 2、no. 5、命題 13) である商環は、* $A$ に関連付けられた * ハウスドルフ環と呼ばれます。

$(A_i)_{i \in I}$ をトポロジカル環の族とする。 集合 $A = \prod_{i \in I} A_i$ では、$A_i$ のトポロジの *積* は、$A_i$ の環構造の積と互換性があります (積群と同じ証明)。このように定義されたトポロジー 環 $A$ は、トポロジー 環 $A_i$ の *積* と呼ばれます。

### 5. トポロジカル環の完成

私たちがトポロジー 環の *均一性について話すとき、私たちは常にその *加法群* の均一性を意味しますが、〜でない限りその逆は明示的に述べられています。特に、$A$の加法群が完全であれば、$A$は*完全*な環であると言われます。

$A$ を *Hausdorff* トポロジカル環とします。 加法群 $A$ は、*完全ハウスドルフ可換* 群 $\hat{A}$ の密な部分群と考えることができ、これは同型 ($\S$ 3, no. 5, 定理 2) まで決定されます。 位数において、$A$ を *完全な環* の *部分環* として考えることができるようにするには、空間 $\hat{A} \times \hat{A}$ への連続性によって拡大する写像 $xy$ ができる必要があります。この拡大の可能性は、次のより一般的な定理から導き出されます。

#### 定理 1 {#top-iii-s6-thm-1 .statement tag=0BNF}

E、F、G を 3 つの完全なハウスドルフ可換群とします。 A を E の密な部分群とし、B を F の密な部分群とします。 f が $A \times B$ の $\mathbf{Z}$ 連続 $\mathbf{Z}$-双線形 (*) 写像を G に変換すると、f は連続性によって連続 $\mathbf{Z}$-双線形に拡張できます。 $E \times F$の写像をGに。

$(x_0, y_0)$ を $E \times F$ の任意の点とし、$\mathfrak{U}, \mathfrak{B}$ を $x_0, y_0$ の近傍フィルターの A、B 上のトレースとします ($\mathfrak{U}, \mathfrak{B}$ は仮定によるフィルター)。 f が連続性によって拡張できることを示すには、$f(\mathfrak{U} \times \mathfrak{B})$ が G (章 II, § 3, no. 6, 命題 11) のコーシー フィルター ベースであることを示すだけで十分です。アイデンティティを考える

$$
f(x', y') - f(x, y) = f(x' - x, y_1) + f(x_1, y' - y) + f(x' - x, y' - y_1).
$$

$\mathfrak{U} \times \mathfrak{B}$ の十分に小さい集合で $(x, y)$ と $(x', y')$ を取り、$x_1$ と $y_1$ を適切に選択することで、右側のそれぞれの項を非常に小さくできることを示します。 W を G の 0 の任意の近傍とします。 f は $(0, 0) \in A \times B$ で連続なので、 $x \in U, x' \in U, y \in V, y' \in V$ のときはいつでも $f(x' - x, y' - y) \in W$ となるように、 集合 $U \in \mathfrak{B}$ と集合 $V \in \mathfrak{B}$ が存在します。 点 $x_1 \in U$ と点 $y_1 \in V$ に乗ります。次に、U のすべての $x, x'$ と V のすべての $y, y'$ について、次のようになります。

$$
f(x' - x, y' - y_1) + f(x - x_1, y' - y) \in W + W.
$$

一方、部分写像 $x \to f(x, y_1)$ は A 上で連続しています。従って、集合 $U' \subset U$、所属から $\mathfrak{U}$ があり、$x$ と $x'$ 属するから $U'$ までは、$f(x' - x, y_1) \in W$ になります。同様に、$V' \subset V$ 所属から $\mathfrak{B}$ までが存在し、$y$ と $y'$ 属するから $V'$ までは、$f(x_1, y' - y) \in W$ になります。従って、$(x, y)$ と $(x', y')$ が $U' \times V'$ のいずれか 2 つの点である場合、

$$
f(x', y') - f(x, y) \in W + W + W + W;
$$

これは f の拡大 $\overline{f}$ の存在を証明します。 $\overline{f}$ が $\mathbf{Z}$ 双線形であるという事実は、恒等式 (章 I, § 8, no. 1, 系 1 ～ 命題 2) の拡大の原理の明らか帰結です。

Q.E.D.

この定理をハウスドルフ トポロジカル環 A に適用すると、E、F、G は $\hat{A}$、A と B は環 A、f は次のようになります。

(*) A のすべての元 $x, x'$ とすべての元 $y, y' \in B$ が次の場合、$f$ は $\mathbf{Z}$-双線形であると言われます。

$$
f(x + x', y) = f(x, y) + f(x', y)
$$
そして
$$
f(x, y + y') = f(x, y) + f(x, y').
$$

$\mathbf{Z}$-双線形写像 $(x, y) \to xy$、これは仮定まで連続です。 $\hat{A} \times \hat{A}$ の拡張写像の $xy$ 値で再度表します。この写像は$\hat{A}$の合成の法則であり、$\mathbf{Z}$双線形であるということは、加法に関して両側に分布的であることを意味します。そしてそれはまた、アイデンティティの拡大の原理により *連想的*でもあります。その結果:

#### 命題 6 {#top-iii-s6-prop-6 .statement tag=0BNG}

*ハウスドルフ位相幾何学環* $A$ * は、完全なハウスドルフ環* $\hat{A}$ の稠密部分環と同型であり、 * 同型* まで決定されます (そして、$A$ の *完全* と呼ばれます)。

$A$ が *可換* である場合 (それぞれ * が単位元* である)、同じことが $\hat{A}$ にも当てはまります (恒等の拡大の原理)。

Let $A$ be a topological 環, not necessarily Hausdorff; let $N$ be the closure of $\{0\}$ in $A$, and let $A' = A/N$ be the Hausdorff 環 associated with $A$. Then $\hat{A}'$, the completion of $A'$, is called the *Hausdorff completion* of $A$ and is also denoted by $\hat{A}$. § 3, no. 4、命題 8 のように、*完全ハウスドルフ* トポロジカル環 $C$ をもつ $A$ のすべての連続環準同型 $u$ は $u = v \circ \varphi$ として一意に因数分解できることがわかります。 $v$ is a continuous 準同型 of $\hat{A}$ into $C$ and $\varphi$ is 標準写像 of $A$ into $\hat{A}$. $A, B$ が 2 つのトポロジー 環で、$u : A \to B$ が連続準同型である場合、図式となるような一意の連続準同型 $\hat{u} : \hat{A} \to \hat{B}$ が存在します。

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
\varphi \downarrow & & \psi \downarrow \\
\hat{A} & \xrightarrow{\hat{u}} & \hat{B}
\end{array}
$$

is commutative ($\varphi$ and $\psi$ being 標準写像);前の結果を $\psi \circ u$ に適用するだけです。

### 6. トポロジカル加群

#### 定義 3 {#top-iii-s6-def-3 .statement tag=0BNH}

*Given a topological 環* $A$ *with 単位元, a topological left* $A$*-module is 集合* $E$, *together with*:

1) *左* $A$*-モジュール構造*;
2) *位相 compatible with 加法群構造 of* $E$, *and 満たす the following axiom*:
(MT) *写像* $(\lambda, x) \to \lambda x$ *of* $A \times E$ *into* $E$ *is continuous*.

We 定義する similarly 概念 of a topological right $A$-module;すべての右側の $A$ モジュールは左側の $A^0$ モジュールと見なすことができ、$A^0$ は $A$ の反対環であり、$A$ の位相は $A^0$ の環構造と互換性があるため、両者を区別する必要はありません。トポロジカル右 $A$ モジュールとトポロジカル左 $A^0$ モジュール。

#### 例 1 {#top-iii-s6-n6-exa-1 .statement tag=0BNI}

A topological ベクトル空間 over $\mathbf{R}$ (resp. $\mathbf{C}$) is a topological $\mathbf{R}$ (resp. $\mathbf{C}$) 加群.

#### 例 2 {#top-iii-s6-n6-exa-2 .statement tag=0BNJ}

$A$ を環とし、$\mathfrak{B}$ を$A$ の両面理想の $A$ からなるに対するフィルター 基底とします。 $E$ を左の $A$ モジュールとします。 $A$ に、$\mathfrak{B}$ が $0$ (no. 3、例 3) の近傍の基本系であるトポロジー (そのリング構造と互換性がある) と、$a$ が $\mathfrak{B}$ を通る集合 $aE$ が含まれるトポロジー (その加法群構造と互換性がある) $E$ を与えると、次のようになります。 $0$ ($§ 1$、no. 2、例) の近傍の基本システムでは、$E$ がトポロジカルな $A$ 加群であることがすぐに検証されます。

#### 注意 {#top-iii-s6-n6-rem-1 .statement tag=0BNK}

トポロジー 環 $A$ が与えられた場合、左側の $A$ モジュール $E$、位相が $E$ の加法群構造と互換性があると考えてください。アイデンティティのおかげで
$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0)x_0 + \lambda_0(x - x_0) + (\lambda - \lambda_0)(x - x_0)
$$
公理 (MT) は、次の 3 つの公理の結合と等価です。
(MT$_I'$)。 *それぞれ* $x_0 \in E$、*写像* $\lambda \to \lambda x_0$ *は点* $\lambda = 0$で連続します。
(MT$_{II}'$)。 *それぞれ* $\lambda_0 \in A$、*写像* $x \to \lambda_0 x$ *は点* $x = 0$で連続します。
(MT$_{III}'$)。 *写像* $(\lambda, x) \to \lambda x$ *は点* $(0, 0)$で連続します。

We deduce from this a necessary and sufficient set of conditions that the *filter* $\mathfrak{B}$ *of neighbourhoods of* $0$ *in an* $A$*-module* $E$ *must satisfy in order to define a topology on* $E$ *compatible with its module structure;* $\mathfrak{B}$ *must satisfy the axioms* (GA$_I$) *and* (GA$_{II}$) *of* $§ 1$, *no. 2*, *and in addition must satisfy the following three axioms:*
(MV$_I$). *それぞれ* $x_0 \in E$ *と* $V \in \mathfrak{B}$、*近傍* $S$ *の* $0$ *in* $A$ *そのような* $S.x_0 \subset V$。
(MV$_{II}$)。 *それぞれ* $\lambda_0 \in A$ *および* $V \in \mathfrak{B}$、*存在します* $W \in \mathfrak{B}$ *そのような* $\lambda_0 W \subset V$。
(MV$_{III}$)。 *それぞれ* $V \in \mathfrak{B}$ *存在します* $U \in \mathfrak{B}$ *と近傍* $T$ *の* $0$ *中に* $A$ *そのような* $T.U \subset V$。

環 $\mathbf{Z}$ に離散位相が与えられると、すべての可換トポロジカル群はトポロジカル $\mathbf{Z}$ 加群になります。

$M$ がトポロジカル $A$ 加群 $E$ の部分加群である場合、$E$ の位相によって $M$ に誘導された位相が $M$ の加群構造と互換性があることは明らかです。 また、商$A$モジュール$E/M$では、$E$の位相の$M$により商となる位相が$A$モジュール構造と互換性があります。 これを確認するには、$A \times (E/M)$ の $E/M$ への写像 $(\lambda, x) \to \lambda x$ が連続であることを示すだけで十分です (ここで、$x \to x'$ は $E/M$ への $E$ の標準写像を示します)。 ここで、加法的な位相群 $A \times (E/M)$ と $(A \times E)/(\{0\} \times M)$ (§ 2, no. 9、命題 26 の帰結) を識別できるので、$A \times E$ の $E/M$ への写像 $(\lambda, x) \to \lambda x'$ が連続的であることを示すだけで十分です。問題のマッピングは $x \to x'$ と $(\lambda, x) \to \lambda x$ の合成であるため、これはすぐにわかります。

$(E_i)_{i \in I}$ をトポロジカル $A$ 加群の任意の族とし、$E = \prod_{i \in I} E_i$ を $E_i$ の積である $A$ 加群とする。 すると、$E$ の積位相は、$E$ の $A$ モジュール構造と互換性があります。 これを証明するには、$A \times E$ の $E$ への写像 $(\lambda, x) \to (\lambda \cdot \mathrm{pr}_i x)_{i \in I}$ が連続であること、または (I, § 4, no. 1 章の命題 1 により) 各指標 $x \in I$ の写像 $(\lambda, x) \to \lambda \cdot \mathrm{pr}_x x$ が $A \times E$ から $E_x$ への連続写像であることを示すだけで十分です。しかし、このマッピングは $(\lambda, x_x) \to \lambda x_x$ と $(\lambda, x) \to (\lambda, \mathrm{pr}_x x)$ の合成であり、どちらも連続しています。

$A$ をハウスドルフ トポロジカル環とし、$E$ をハウスドルフ トポロジカル $A$ 加群とする。 $\hat{E}$ を加法群とします。これは、可換トポロジー 群 $E$ (§ 3, no. 5, 定理 2) の完成です。 $\mathbf{Z}$-双線形写像 $(\lambda, x) \to \lambda x$ の積 $A \times E$ 加法群 $A, E$ から加法群 $E$ は、連続性によって次の $\mathbf{Z}$-双線形写像に拡張できます。 $\hat{A} \times \hat{E}$ を $\hat{E}$ (no. 5, 定理 1) に変換し、この写像を引き続き $(\lambda, x) \to \lambda x$ で表します。アイデンティティの拡大の原則により、$\lambda \in \hat{A}, \mu \in \hat{A}$ と $x \in \hat{E}$ には $\lambda (\mu x) = (\lambda \mu) x$ が、すべての $x \in \hat{E}$ には $1 \cdot x = x$ が与えられます。 外部法則 $(\lambda, x) \to \lambda x$ したがって、定義するは、位相と互換性のある $\hat{E}$ 上の $\hat{A}$ モジュール構造になります。このように定義された位相的 $\hat{A}$ モジュール $\hat{E}$ は、位相的 $A$ モジュール $E$ の*完成*と呼ばれます。

$E$ をトポロジー 環 $A$ 上のトポロジー 加群とします。ここで、$A$ も $E$ も必ずしもハウスドルフではありません。 $N$ (それぞれ $F$) を、$A$ (それぞれ $E$) の $\{0\}$ の終結とします。 $N$ は、$A$ (no. 4、命題 5) の両側イデアルであり、$F$ は、$E$ (no. 1、命題 1) のサブ$A$ 加群です。さらに、連続性により、$\lambda \in N$ または $x \in F$ のときはいつでも $\lambda x \in F$ になります。したがって、定義する、移行から商、写像 $(A/N) \times (E/F)$ の $(\dot{\lambda}, \dot{x}) \to \dot{\lambda} \dot{x}$ は $E/F$ になります。この写像が連続であること、したがって $E/F$ 上のトポロジカル $(A/N)$ 加群の定義する構造は、(§ 2, no. 9 の系から命題 26 を使用することによって) 簡単に検証されます。 $B = A/N$ と $L = E/F$ を置くと、$B$ モジュール $L$ は、$E$ に *関連付けられた* ハウスドルフ加群と呼ばれます。その完成 $\hat{L}$ は、$A$ (no. 5) のハウスドルフ完成 $\hat{A}$ (定義から $\hat{B}$ に等しい) 上の位相的加群であり、この加群 $\hat{L}$ は *ハウスドルフ完成 * と呼ばれます。 $E$ の であり、$\hat{E}$ で示されます。 , no. 4, 命題 8 のように、$E$ のすべての連続準同型 $u : E \to G$ は、完全なハウスドルフ $\hat{A}$ 加群 $G$ が一意に $u = v \circ \varphi$ に因数分解されます。ここで、$v$ は連続です。 $\hat{E}$の準同型は$G$になり、$\varphi$は$E$の標準写像は$\hat{E}$になります。 結論する、$E, E'$ が 2 つのトポロジカル $A$ 加群で、$u : E \to E'$ が連続準同型である場合、図式となるような一意の連続準同型 $\hat{u} : \hat{E} \to \hat{E}'$ が存在します。

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow \varphi & & \downarrow \varphi' \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{E}'
\end{array}
$$

は可換であり、$\varphi$ と $\varphi'$ は標準写像です。

定義とこの切断の結果は、環の単位元に関するすべての記述を削除することで、任意のトポロジー 環上の *疑似モジュール* に同様に適用されます。

### 7. 位相分割環と体

以下の章 IV と V では、$K$ が *除算環* である場合、$K$ の非ゼロ元の *乗法群* を $K^*$ で表します。

#### 定義 4 {#top-iii-s6-def-4 .statement tag=0BNL}

*トポロジカルな割り算環は集合* $K$ *割り算環構造と位相を持ち、* $K$ の環構造、* および加法の満たすと互換性があります:*

(KT) *写像* $x \to x^{-1}$ *of* $K^*$ *into* $K^*$ *連続です*

*可換位相分割環は位相分割体と呼ばれます。

集合 $K$ の除算環構造と位相は、対応する環構造と位相が互換性があり、加法の公理 (KT) が満たされる場合、*互換性がある*と言われます。

#### 例 1 {#top-iii-s6-n7-exa-1 .statement tag=0BNM}

任意の除算環 $K$ で、*離散* 位相は除算環構造と互換性があります。 位相が離散である位相分割環を *離散* 分割環と呼びます。

#### 例 2 {#top-iii-s6-n7-exa-2 .statement tag=0BNN}

\* 有理直線 $Q$ (それぞれ実直線 $R$) の位相は、$R$ (それぞれ $R$) の体構造と互換性があります (章 IV, § 3 を参照)。 \*

定義 4 は、$K$ が位相分割環である場合、乗法群 $K^*$ 上の $K$ の分割によって *誘導*された位相が $K^*$ の群構造と互換性があることを示しています。

$a \neq 0$ の場合、相似関係 $x \to ax$ と $x \to xa$ はそれ自体に対する $K$ の同型写像です。そして、すべての $b \in K$ に対して写像 $x \to ax + b$ も同様です。相似関係 $x \to ax$ と $x \to xa$ は、$a \neq 0$ の場合、$K$ の (トポロジカル) *加法群* の *自己同型* であることに注意してください。 $V$ が $K$ の $o$ のいずれかの近傍である場合、$aV$ と $Va$ はすべての $a \neq 0$ について $o$ の近傍であるということになります。

$X$ を位相的空間とし、$f$ を位相的分割環 $K$ への $X$ の写像とします。 $f$ が点 $x_0 \in X$ で連続し、$f(x_0) \neq 0$ の場合、$f^{-1}$ は $x_0$ で連続します。特に、$K$ がトポロジカル *体* である場合、$K$ に係数を含む $n$ 変数のすべての *有理数写像* は、分母が消えない $K^n$ の点ごとに連続します。

同様に、$f$ が集合 $X$ の写像で、フィルタ $\mathfrak{F}$ でハウスドルフ位相分割環 $K$ にフィルタリングされ、$\lim_{\mathfrak{F}} f$ が存在し、$0$ ではない場合、$\lim_{\mathfrak{F}} f^{-1}$ が存在し、次のようになります。

$$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}.
$$

$H$ が位相分割環 $K$ の *分割部分環* である場合、$K$ の位相によって $H$ に誘導される位相は、$H$ の分割環構造と互換性があります。このように$H$で定義された位相分割環の構造は、$K$の分割によって*誘導*されると言われます。さらに、$\overline{H}$ は、$K$ の *除算部分環* でもあります (証明は、命題 5 の除算に類似しています)。

位相分割環 $K$ では、集合 $\{0\}$ の閉包は命題 5 による両側イデアルであるため、$\{0\}$ または $K$ のいずれかでなければなりません。他の語では、$K$の位相が最も粗い位相(章I, § 2, no. 2)でない場合、ハウスドルフ(§ 1, no. 2、命題2)になります。

### 8. 位相分割上の均一性環

$K$ が位相分割環である場合、以下を区別する必要があります。
1) $K$ の *加法群* の均一性。これは $K$ で定義され、$K$ の *加法均一性* と呼ばれます。 2) *乗法群* $K^*$ の左右の均一性。これらは $K^*$ で定義され、(言葉の乱用により) $K$ の *乗法的*均一性と呼ばれます。

$K$ の加法的均一性によって $K^*$ に *誘発される*均一性は、一般に $K$ の乗法的均一性とは *異なります (練習問題 17 を参照)。

命題 6 までに、ハウスドルフ位相分割環 $K$ は *完全なハウスドルフ環* $\hat{K}$ の *稠密部分環* と考えることができます。 位数では、$\hat{K}$ が *位相分割環* である必要があり、写像 x \to x^{-1} が (\hat{K})^* への連続性によって拡張可能である必要があります。そして、この必要な条件も十分です。 写像 xx^{-1} の場合、x^{-1}x と 1 は、恒等式の拡大の原理により、(\hat{K})^* 上で等しくなります。従って、拡張された写像の値は、各 $x \neq 0$ の x の逆数になります。 $\hat{K}$で。その他語 (cf. 章 II, , no. 6, 命題 11)

#### 命題 7 {#top-iii-s6-prop-7 .statement tag=0BNO}

*ハウスドルフ位相分割リング K の完成 $\hat{K}$ は、クラスター点 0 を持たないすべてのコーシー フィルター (加法構造に関して) のマッピング $x \to x^{-1}$ の下にある画像が (加法構造に関して) コーシー フィルターである場合に限り、トポロジカル分割リングです。*

この条件が満たされず、環 $\hat{K}$ が零因子となる位相分割環があります (練習問題 26 を参照)。さらに、たとえ完成 $\hat{K}$ が位相分割環であっても、$\hat{K}$ の *乗算* 構造が *完全 * 空間の構造であると仮定する*先験的* 理由はありません。ただし、これは、$\hat{K}$ が *局所的にコンパクト* であるような除算環 K (章 I, § 9, no. 7、命題 13、および章 III, § 3, no. 3、命題 4 を参照) とトポロジカル *体* の場合に当てはまります。後者の場合、次の命題があります。

#### 命題 8 {#top-iii-s6-prop-8 .statement tag=0BNP}

*トポロジカル体 K の加法均一構造が完全ハウスドルフ空間の構造である場合、K* の乗法構造は完全空間の構造です。

$\mathfrak{F}$ が K* 上の *乗算* 構造に関するコーシー フィルターである場合、 $\mathfrak{F}$ は K* 上の *加法* 構造に関するコーシー フィルターであり、0 に収束しないことを示します。これにより結果が確定します。 U を K の 0 の任意の近傍とし、V を $V \subset U, VV \subset U$ [公理 (AV$_\text{II}$)] および $-1 \notin V$ となる 0 の閉じた近傍とします。次に、仮定までに集合 $A \in \mathfrak{F}$ があり、すべての $x \in A$ と $y \in A$ に対して、$x^{-1}y \in 1 + V$ が得られます。 $a \in A$、次に $A \subset a + aV$ とすると、$a + aV$ は閉じた集合であり、含む 0 ではありません。従って、0 は A の閉包に含まれず、従って $\mathfrak{F}$ のクラスター 点ではありません。 W を 0 の近傍とし、$aW \subset V$ [公理 (AV$_\text{I}$)] とします。次に、仮定までに $B \subset A$ となる集合 $B \in \mathfrak{F}$ があり、すべての $x \in B$ と $y \in B$ に対して、$x^{-1}y \in 1 + W$ が得られます。従って$y - x \in xW \subset AW \subset aW + aVW$;しかし、K は可換なので、$aVW = aWV \subset VW \subset U$;従って、$y - x \in U + U$ と命題が証明されます。

同じ証明は、命題 8 が、K の乗法構造の *1* に関するすべてのコーシー フィルターが、他の乗法構造に関してもコーシー フィルターである場合に拡張できることを示しています。

### 練習問題 {#top-iii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
