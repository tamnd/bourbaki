---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 1
section_title: Definition of real numbers
lang: ja
source: top-i-iv
book_pages: 329-334, 378-381
pdf_pages: 0335-0340, 0384-0387
extraction: ocr
subsections:
    - "no": 1
      title: THE ORDERED GROUP OF RATIONAL NUMBERS
      page: 329
      pdf_page: 335
    - "no": 2
      title: THE RATIONAL LINE
      page: 330
      pdf_page: 336
    - "no": 3
      title: THE REAL LINE AND REAL NUMBERS
      page: 331
      pdf_page: 337
    - "no": 4
      title: PROPERTIES OF INTERVALS IN $\mathbf{R}$
      page: 332
      pdf_page: 338
    - "no": 5
      title: LENGTH OF AN INTERVAL
      page: 333
      pdf_page: 339
    - "no": 6
      title: ADDITIVE UNIFORMITY OF $\mathbf{R}$
      page: 334
      pdf_page: 340
statements: 10
exercises: 4
content_sha256: 0e21ccb34e916f7012e482c1bd2c1e1a7224bb1215a9cf4a492867fc76580592
translated_from: content/en/top/IV/01_s1_definition_of_real_numbers.md
translation_method: google
source_content_sha256: f4c12bd1cb845b5f3c66dbac6fe917b0b8b7c5cafbedd83622f13c0a4a7e7248
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1f744647799faa60ce0e636b6340f58eccd15497466deb3b4c3a4667d485194a
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 定義/実数

### 1. 有理数数の順序付けられた群

有理数数の集合 $\mathbf{Q}$ の順序 $x \leq y$ を定義しました。この順序付けにより、$\mathbf{Q}$ が *線形順序付け* 集合になり、それが $\mathbf{Q}$ の *加法群* 構造と *互換性* があることがわかりました。つまり、各 $z \in \mathbf{Q}$ 関係 $x \leq y$ が $x + z \leq y + z$ と同等です (つまり、 *順序は翻訳下でも不変です*)。 記法 (線形順序の群で使用されます) を思い出します。

$$
x^+ = \sup (x, 0), \\
x^- = \sup (-x, 0) = (-x)^+, \\
|x| = \sup (x, -x);
$$

$|x|$ は $x$ の *絶対値* と呼ばれ、

$$
x = x^+ - x^-, \qquad |x| = x^+ + x^-
$$

そして *三角形不等式*

(1)
$$
|x + y| \leq |x| + |y|,
$$
不等式と一緒に
(2)
$$
||x| - |y|| \leq |x - y|
$$
これは (1) の明らか帰結です。さらに
(3)
$$
|x^+ - y^+| \leq |x - y|.
$$

関係 $x \geq 0,\ x = x^+,\ x^- = 0,\ |x| = x$ (それぞれ $x \leq 0,\ x = -x^-,\ x^+ = 0,\ |x| = -x$) は *同等*です。 関係 $|x| = 0$ は $x = 0$ と同等です。 $a \geq 0$ の場合、関係 $|x| \leq a$ は $-a \leq x \leq a$ に相当し、関係 $|x| \geq a$ は「$x \geq a$ または $x \leq -a$」に相当します。 $\mathbf{Q}$ のすべての $x, y$ については、

(4)
$$
\sup (x, y) + z = \sup (x + z, y + z),
$$
(5)
$$
\inf (x, y) = - \sup (-x, -y),
$$

そして、具体的なケースとしては、

(6)
$$
\sup (x, y) = x + (y - x)^+ = x + (x - y)^-,
$$
(7)
$$
\inf (x, y) = x - (y - x)^- = x - (x - y)^+.
$$

最後に、$\mathbf{Q}_+$ が有理数数 $\geq 0$ の集合を表すものとします。それから私たちは持っています

(8)
$$
\mathbf{Q}_+ + \mathbf{Q}_+ \subset \mathbf{Q}_+,
$$
(9)
$$
\mathbf{Q}_+ \cap (- \mathbf{Q}_+) = \{ 0 \},
$$
(10)
$$
\mathbf{Q}_+ \cup (- \mathbf{Q}_+) = \mathbf{Q}.
$$

関係 $x \leq y$ は $y - x \in \mathbf{Q}_+$ と *同等* です。

この順序を、加法群構造* と互換性のある $\mathbf{Q}$ の定義する *位相に使用します。

### 2. 合理的なライン

*対称オープン区間* $]-a, +a[$ の集合 $\mathfrak{F}$ を考えてみましょう。ここで、$a$ は有理数数 $> 0$ の集合を通過します。 $\mathfrak{F}$ は、$\mathbf{Q}$ の加法群構造と互換性のある、位相の * $0$ の近傍の * 基本的な系であることを示します。

群 $\mathbf{Q}$ は可換であり、公理 $(\mathrm{GV}'_{\mathrm{II}})$ は明らかに満たされます。したがって、公理 $(\mathrm{GV}'_{\mathrm{I}})$ が他の語でも満たされ、各 $a > 0$ に対して条件 $|x| < b$ と $|y| < b$ が一緒になって $|x + y| < a$ を暗示するような $b > 0$ が存在することを示すだけで十分です。三角形不等式は、$b = a/2$を取る可能性があることを示しています。

#### 定義 1 {#top-iv-s1-def-1 .statement tag=0BP1}

*有理線は、集合 $\mathbf{Q}$ のトポロジカル空間からなると加法群位相を組み合わせたものであり、その対称開いた区間 $]-a, +a[$ $(a > 0)$ 形が基本となります。 系/近傍/$0$.*

*このように定義された位相幾何学的群 $\mathbf{Q}$ を有理直線の加法群と呼びます。

$a$ が任意の有理数数 $> 0$ である場合、$1/n < a$ となるような整数 $n > 0$ が存在します。したがって、有理線上の$0$の近傍の基本的な系のオープン区間$]-\frac{1}{n}, +\frac{1}{n}[$$(n = 1, 2, \ldots)$形。

任意の点 $x \in \mathbf{Q}$ の近傍の基本系を、オープン区間 $]x - a, x + a[$ を取得します。ここで、$a$ は有理数数 $> 0$ (または集合) の集合を通過します。 数 $1/n$）。

したがって、定義 1 は、章 I, § 1, no. 2 で与えられるものと等価です。

$a < b$ となるような有理数数 $(a, b)$ のそれぞれの対に対して、$a < c < b$ となるような $c \in \mathbf{Q}$ [例えば $c = (a + b)/2$] が存在します。したがって、有理直線は非離散ハウスドルフ空間であることがわかります。

それぞれの $a > 0$ について、$U_a$ を $\mathbf{Q} \times \mathbf{Q}$ の対 $(x, y)$ の集合とし、$|x - y| < a$ とします。 $a$ は有理数数 $> 0$ の集合 (または数 $1/n$ の集合) を通過するため、集合 $U_a$ 形は取り巻きの基本系有理直線の加法群 $\mathbf{Q}$ の均一性。 関係 (2) と (3) は、$|x|, x^+$ と $x^-$ が $\mathbf{Q}$ 上で一様連続であることを示しています。したがって、写像 $\sup(x, y)$ と $\inf(x, y)$ は $\mathbf{Q} \times \mathbf{Q}$ 上で一様連続です。

### 3. 実直線と実数

#### 定義 2 {#top-iv-s1-def-2 .statement tag=0BP2}

$\mathbf{R}$ を有理直線の加法群 $\mathbf{Q}$ の完成である位相幾何学群とします。 $\mathbf{R}$ のうち元は実数と呼ばれます。トポロジー 空間として、$\mathbf{R}$ は実直線と呼ばれます。トポロジカルな群として、$\mathbf{R}$ は実直線の加法群と呼ばれます。

私たちは常に同一視する $\mathbf{Q}$ を、正準的に同型である $\mathbf{R}$ の密な部分群とします。この規則では、すべての有理数数は実数になります。合理的でないすべての実数は非合理的であると言われます。 章 II, § 3, no. 3 で、そのような数が存在することを確認しました (この章の § 3, no. 3 でこれを他ので示します。練習問題 2 から § 2 も参照してください)。したがって、無理数数の (章 III, § 2, no. 1) 集合 $\mathbf{CQ}$ は $\mathbf{R}$ に密です。

$\mathbf{Q}$ の位数構造は、拡張順序が $\mathbf{R}$ の加法群構造と互換性があるような方法で $\mathbf{R}$ まで拡張できることを示します。

#### 命題 1 {#top-iv-s1-prop-1 .statement tag=0BP3}

関係 $y - x \in \overline{\mathbf{Q}}_+$ は $\mathbf{R}$ での順序であり、$\mathbf{R}$ は線形順序の集合になります。は、$\mathbf{R}$ の加法群構造、および $\mathbf{Q}$ の $x \leq y$ の順序付けである誘導すると互換性があります。

まず、関係 $y - x \in \overline{\mathbf{Q}}_+$ と $z - y \in \overline{\mathbf{Q}}_+$ が $z - x \in \overline{\mathbf{Q}}_+$ を暗示していることを示します。実際、写像 $x + y$ は $\mathbf{R} \times \mathbf{R}$ で連続であるため、(8) により $\overline{\mathbf{Q}}_+ + \overline{\mathbf{Q}}_+ \subset \overline{\mathbf{Q}}_+$ (章 I, § 2, no. 1, 定理 1) が得られます。次に、関係 $y - x \in \overline{\mathbf{Q}}_+$ と $x - y \in \overline{\mathbf{Q}}_+$ が $x = y$ を暗示していることを示します。これにより、$y - x \in \overline{\mathbf{Q}}_+$ が $\mathbf{R}$ の注文であることが確立されます。 $\overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+) = \{0\}$ を示すだけで十分です。現在、写像 $x \to x^+$ と $x \to x^-$ は $\mathbf{Q}$ で一様連続であるため、連続性によって $\mathbf{R}$ (章 II, , no. 6, 定理 2) まで拡張できます。 $f$ と $g$ をそれぞれの拡大とします。 拡大までに、すべての$x \in \mathbf{R}$に対して$x = f(x) - g(x)$ができます。 $x \in \overline{\mathbf{Q}}_+$ の場合は $g(x) = 0$ で、$-\overline{\mathbf{Q}}_+$ は $-x$ の連続性による $-\mathbf{Q}_+$ の終結であるため、$x \in -\overline{\mathbf{Q}}_+$ の場合は $f(x) = 0$ となります。したがって、$x \in \overline{\mathbf{Q}}_+ \cap (-\overline{\mathbf{Q}}_+)$ の場合、$f(x) = g(x) = 0$ があり、したがって $x = 0$ となります。

(10) までに $\overline{\mathbf{Q}}_+ \cup (-\overline{\mathbf{Q}}_+) = \mathbf{R}$ が得られるため、$\mathbf{R}$ は順序付け $y - x \in \overline{\mathbf{Q}}_+$ によって *線形順序付け* されます。

さらに、関係 $y - x \in \overline{\mathbf{Q}}_+$ と $(y + z) - (x + z) \in \overline{\mathbf{Q}}_+$ は同等であるため、$y - x \in \overline{\mathbf{Q}}_+$ の順序は $\mathbf{R}$ の加法群構造と互換性があります。

最後に、$x$ と $y$ 属するから $\mathbf{Q}$ 関係 $y - x \in \overline{\mathbf{Q}}_+$ と $y - x \in \mathbf{Q}_+$ が等しい場合、関係 $y - x \in \overline{\mathbf{Q}}_+$ 誘導する関係 $\mathbf{Q}$の$x \leq y$。これで証明は完了です。

関係 $y - x \in \overline{\mathbf{Q}}_+$ は再び $x \leq y$ で表されます。 集合 $\overline{\mathbf{Q}}_+$ は、$\mathbf{R}$ のすべての $x \geq 0$ の集合であり、$\mathbf{R}_+$ で示されます。 *閉店しました集合*です。すべての $x > 0$ のうち集合は $\mathbf{R}_+^*$ で示されます。これは $-\mathbf{R}_+$ の補数であるため、$\mathbf{R}$ では *オープン* になります。

### 4. $\mathbf{R}$の区間の物件

#### 命題 2 {#top-iv-s1-prop-2 .statement tag=0BP4}

*$\mathbf{R}$ のすべてのクローズ (またはオープン) 区間は、$\mathbf{R}$ のクローズ (またはオープン) 集合です。

集合 $[a, \to[ = a + \mathbf{R}_+$ と $]\leftarrow, a] = a - \mathbf{R}_+$ は、それぞれ $\mathbf{R}_+$ と $-\mathbf{R}_+$ からの変換によって得られるため、閉じています (章 III, § 1, no. 1)。 集合 $]\leftarrow, a[$ と $]a, \to[,$ はその補数であり、オープンです。最後に、クローズド区間 $[a, b]$ (オープン区間 $]a, b[$) は、$[a, \to[$ の共通部分と $]\leftarrow, b]$ ($]a, \to[$ と $]\leftarrow, b[$ のそれぞれ) であるため、クローズド (オープン) です。 集合。

したがって、$\mathbf{R}$ の閉じた区間 $[-a, +a]$ ($a > 0$) は 0 の近傍です。 $a$ が $\mathbf{R}_+^*$ を通過するとき、それらが形 0 の近傍* の *基本的な系であることを示しましょう。このためには、次の命題を確立するだけで十分です。

#### 命題 3 {#top-iv-s1-prop-3 .statement tag=0BP5}

*$r$ は有理数数 $> 0$ の集合、$\mathbf{R}$ 形の基本系の 0 の近傍で区間 $s_r = [-r, +r]$ を通過します。

章 III, § 3, no. 4 の命題 7 により、区間の $\mathbf{R}$ の *クロージャ* を取得することで、$\mathbf{R}$ の 0 の近傍の基本的な系が得られます。

S_r \cap \mathbf{Q} = [-r, +r] \textit{of} \mathbf{Q}。 S_r が S_r \cap \mathbf{Q} の閉包であることを示せば、証明は完了します。ここで、S_r は \mathbf{R} で閉じられているため、x が実数で -r < x < r である場合、x は S_r \cap \mathbf{Q} の閉包内にあることを証明するだけで済みます。 区間 ]-r, +r[ は \mathbf{R} の開集合なので、\mathbf{R} の o の十分に小さいすべての近傍 V に対して x + V \部分集合 ]-r, +r[;しかし \mathbf{Q} は \mathbf{R} 内で密であるため、x + V には有理数数 r' \ があり、 -r < r' < r となり、したがって r' \in S_r \cap \mathbf{Q} となります。

#### 系 {#top-iv-s1-n4-cor-1 .statement tag=0BP6}

*実直線のすべての点には、近傍の可算基本系があります。*

#### 命題 4 {#top-iv-s1-prop-4 .statement tag=0BP7}

*(x, y) が、x < y となるような実数のいずれかの対である場合、x < r < y となる有理数数 r が存在します。*

\mathbf{Q} は \mathbf{R} 内で密であるため、]x, y[ が空ではないことを示すだけで十分です。翻訳により、x = 0 および y > 0 と仮定することができます。 ここで、 \mathbf{R} はハウスドルフ空間であるため、 命題 3 によって、 y \notin ]-r, +r[ となるような有理数数 r > 0 が存在し、これは 0 < r < y を意味します。

#### 命題 5 {#top-iv-s1-prop-5 .statement tag=0BP8}

*I を \mathbf{R} の任意の区間とします。次に、\mathbf{R} の位相によって I に誘導された位相は、I の開いた区間によって生成されます (ここで、I は関係 x \leq y によって線形順序付けされていると見なされます)*。

I のすべてのオープン区間は、\mathbf{R} のオープン区間の I 上のトレースです。これは有界の区間については明らかであり、I の無界の区間 ]a, \to[ は \mathbf{R} の無界の区間 ]a, \to[ のトレースです。したがって、I = \mathbf{R}; の場合に限定することができます。しかしこの場合、点 x \in \mathbf{R} 含むのすべての近傍が開いた区間 ]x - a, x + a[ であるため、結果は命題 3 から導き出されます。

#### 注意 {#top-iv-s1-n4-rem-1 .statement tag=0BP9}

A が \mathbf{R} の密な部分集合である場合、\mathbf{R} の位相は A の終点属するを終点とする開いた区間によって生成されます。

$$ ]x - a, x + a[ $$

が開いた区間含む x である場合、x - a < y < x および x < z < x + a となるような A の 2 つの点 y、z が存在します。したがって、]y, z[ 含む x であり、]x - a, x + a[ に含まれます。 さらに、この証明は、考慮中の区間が \mathbf{R} のトポロジーの基礎 (第 I, § 1, no. 3 章) を形成していることを示しています。 特に、A = \mathbf{Q} とすると、\mathbf{R} の位相には可算な基底があることがわかります。

### 5. 区間中長さ

#### 定義 3 {#top-iv-s1-def-3 .statement tag=0BPA}

*端点 a と b (a \leq b) を持つ有界区間の長さは b - a と定義されます。*

したがって、複数の点含むを含むすべての有界区間は長さ > 0 になります。 $a \leq b$ の場合、4 つの区間 $[a, b], ]a, b[, [a, b[$ と $]a, b[$ はすべて同じ長さを持ちます。エンドポイント $a + c$ と $b + c$ を持つ区間は、エンドポイント $a$ と $b$ を持つ区間と同じ長さを持ちます。他の語では、区間の *長さは翻訳下で不変です*。

$a \leq c \leq d \leq b$ の場合、$d - c \leq b - a$ になります。したがって、有界区間 $I$ が有界区間 $I'$ に含まれる場合、$I$ の長さは $I'$ の長さ以下になります。

$n$ が相互に互いに素開いている区間 $I_1, I_2, \ldots, I_n$ が区間 $[a, b]$ ($a < b$) に含まれている場合、$n$ の帰納法によって、$I_k = ]c_k, d_k[$ であれば置換があることが簡単にわかります。 添字 $k$ ($1 \leq k \leq n$) の $\sigma$ は、$1 \leq k \leq n - 1$ に対して $d_{\sigma(k)} \leq c_{\sigma(k+1)}$ になります。直ちに、区間 $I_k$ の長さの和は、$[a, b]$ の長さに等しく、$1 \leq k \leq n - 1$ に対して $c_{\sigma(1)} = a, d_{\sigma(n)} = b$ と $d_{\sigma(k)} = c_{\sigma(k+1)}$ が存在する場合に限り、等式が成り立ちます。

### 6. $\mathbf{R}$の相加的均一性

群 $\mathbf{R}$ は線形順序であるため、写像 $x^+, x^-$ と $|x|$ は、$\mathbf{Q}$ について上にリストした$\mathbf{Q}$ と満たすのすべての関係、特に関係と同じ方法で、$\mathbf{R}$ で定義されます。 (1)から(7)までです。 $a$ を実数 > 0 とし、$U_a$ をすべての対 $(x, y) \in \mathbf{R} \times \mathbf{R}$ のうち集合とし、$|x - y| < a$ とします。 $a$ は、実数 > 0 の集合 (または数 $1/n$ の集合) を通過するため、集合 $U_a$ 形は、均一性の側近の基本系です。 加法群 $\mathbf{R}$ の実直線 (実直線* の *加法均一性と呼ばれます)。

写像 $|x|$、$x^+$、$x^-$ は $\mathbf{R}$ で *一様連続*、写像 $\sup(x, y)$ と $\inf(x, y)$ は $\mathbf{R} \times \mathbf{R}$ で *一様連続* です。これらの写像したがって、一致するは、$\mathbf{Q}$ と $\mathbf{Q} \times \mathbf{Q}$ でそれぞれ定義された連続性によって拡張された対応する写像となります。

### 練習問題 {#top-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
