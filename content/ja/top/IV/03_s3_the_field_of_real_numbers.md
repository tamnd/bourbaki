---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 3
section_title: The field of real numbers
lang: ja
source: top-i-iv
book_pages: 339-342, 387-388
pdf_pages: 0345-0348, 0393-0394
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLICATION IN $\mathbf{R}$
      page: 339
      pdf_page: 345
    - "no": 2
      title: THE MULTIPLICATIVE GROUP $\mathbf{R}^*$
      page: 340
      pdf_page: 346
    - "no": 3
      title: '*n*TH ROOTS'
      page: 341
      pdf_page: 347
statements: 2
exercises: 3
content_sha256: b1736544ecd2b8e8046375ab339021686180cbb7bc22b76d867a5504ff722625
translated_from: content/en/top/IV/03_s3_the_field_of_real_numbers.md
translation_method: google
source_content_sha256: afbf19bbf21fbfe05f4ab076c9028768c17367d06c4224c3286d307ed17aa711
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 509005ef0c3677a38fc26ef1f733791c53ad9b21e9e02581ea960b1e09515dea
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 体/実数

### 1. 乗法 $\mathbf{R}$

有理線$\mathbf{Q}$の位相は、$\mathbf{Q}$の*加法群* 構造だけでなく、*体* 構造とも互換性があります。 写像の場合、$xy$ は $(0, 0) \in \mathbf{Q} \times \mathbf{Q}$ で連続です。各整数 $n > 0$ 関係 $|x| \leq 1/n$ と $|y| \leq 1/n$ は一緒に $|xy| \leq 1/n^2 \leq 1/n$ を意味するためです。一方、$a$ がゼロ以外の有理数数である場合、整数 $n > 0$ 関係 $|x| \leq 1/|n|a|$ は $|ax| \leq 1/n$ を意味するため、写像 $ax$ は $x = 0$ で連続です。これは、$xy$が$\mathbf{Q} \times \mathbf{Q}$の点ごとに連続していることを示しています（章III, § 6, no. 3）。

$1/x$ が $\mathbf{Q}^*$ で連続であることを示すために、$1/x$ が 0 の任意の近傍 V の補数で *一様連続* (加法構造に関して) であることをより正確に確立します。つまり、$$
\left| \frac{1}{x} - \frac{1}{y} \right| = \frac{|x-y|}{xy}
$$ があります。 $x \in \mathfrak{G}_V$ ごとに $|x| \geq 1/m$ となるような整数 $m > 0$ が存在します。 $x$ と $y$ が $|x-y| \leq 1/m^2 n$ となるような $\mathfrak{G}_V$ のいずれか 2 つの点である場合、$$
\left| \frac{1}{x} - \frac{1}{y} \right| \leq \frac{1}{n}.
$$ が得られます。

クラスター 点として 0 を持たない $\mathbf{Q}^*$ 上の任意のコーシー フィルターの、写像 $1/x$ の下の像は、コーシー フィルター (加法均一性に関して) です。したがって (章 III, , no. 8, 命題 7)

#### 命題 1 {#top-iv-s3-prop-1 .statement tag=0BQF}

*$\mathbf{Q} \times \mathbf{Q}$ と $\mathbf{Q}^*$ でそれぞれ定義された写像 xy と $1/x$ は、連続性によってそれぞれ $\mathbf{R} \times \mathbf{R}$ と $\mathbf{R}^*$ に拡張でき、$\mathbf{R}$ では定義する体構造に拡張できます。この構造を備えた$\mathbf{R}$は、実数の体と呼ばれます。

章 III の § 6 で確立されたトポロジカル体のすべての特性は、もちろん適用できます。特に、実数係数を持つ実数変数 $n$ のすべての *有理数写像* は、分母が消えない $\mathbf{R}^n$ の点ごとに *連続* します。

### 2. 乗法群 $\mathbf{R}^*$

章 III, § 6, no. 7 から、実直線の位相によって $\mathbf{R}^*$ に誘発された位相は、$\mathbf{R}^*$ の乗法群構造と *互換性* があることがわかります。 $\mathbf{R}^*$ はローカルにコンパクトな空間 $\mathbf{R}$ の *オープン* 部分集合であるため、$\mathbf{R}^*$ は *ローカルにコンパクトな* トポロジ群 (章 I, § 9, no. 7, 命題 13) であることがわかり、 *完全* (章 III, § 3, no. 3、系 1 から命題 4。これは章 III, § 6, no. 8、命題 8 からも続きます);もちろん、この後者の性質は $\mathbf{R}^*$ の *乗法的* 均一性に関係しており、 $\mathbf{R}$ の加法的均一性によって $\mathbf{R}^*$ に誘発される均一性ではありません。

写像 $xy$ 写像集合 $\mathbf{Q}_+ \times \mathbf{Q}_+$ は $\mathbf{Q}_+$ に変換され、写像 $\mathbf{R}_+ \times \mathbf{R}_+$ は $\mathbf{R}_+$ (章 I, § 2, no. 1, 定理 1) になります。他の語では、2 つの実数 $\geqslant 0$ のうち *積は $\geqslant 0$* です。式 $(-x)y = -xy$ と $(-x)(-y) = xy$ は、数 $\geqslant 0$ と数 $\leqslant 0$ の積が $\leqslant 0$ であり、2 つの数 $\leqslant 0$ のうち積が$\geqslant 0$;このことから次のことがわかります

$$(1)$$
$$|xy| = |x| \cdot |y|$$

(これは、$\mathbf{Q} \times \mathbf{Q}$ の対応する関係の拡大によっても取得された可能性があります)。

$x > 0$ と $y > 0$ の場合、$xy \neq 0$ があり、したがって $xy > 0$ になります。同様に、$x < 0$ と $y > 0$ の場合は、$xy < 0$ になります。 $x < 0$ と $y < 0$ の場合は、$xy > 0$ です。特に、$x \neq 0$ の場合、$x^2 > 0$ があるため、実数できないの平方* の *和は零 〜でない限りとなり、それぞれの数は零になります。

$x > 0$ と $y \leqslant z$ (それぞれ $y < z$) の場合、他の語には $xy \leqslant xz$ (それぞれ $xy < xz$) があり、*ホモテティー の比率* $> 0$ *$\mathbf{R}$ では位数が維持されます。 $< 0$ 変更の比の $(-x)y = -xy$, ホモテティー なので、$\mathbf{R}$ の順序が逆の順序になります。

$x > 0$ の場合、$x.(1/x) = 1 > 0$ から、$1/x > 0$ になります。 $0 < x < y$ の場合、$xy > 0$ があるため、$x.(1/xy) < y.(1/xy)$、つまり $1/y < 1/x$ になります。したがって、実数 $> 0$ の集合 $\mathbf{R}_+^*$ の写像 $x \to 1/x$ は、真に減少するになります。

同様に、写像 $1/x$ は ]$\leftarrow, 0[$ では真に減少するであるため、写像 $\frac{1}{x-a}$ は区間 ]$\leftarrow, a[$ と $]a, \to[$ のそれぞれで真に減少するであることがわかります。

前の内容から、$\mathbf{R}_+^*$ は乗法群 $\mathbf{R}^*$ の部分群であることがわかります。さらに、位数関係 $x \leq y$ は、$\mathbf{R}_+^*$ の乗算群構造と互換性があります。他の語、$\mathbf{R}_+^*$ は線形順序の群です。

2 つの実数 $\geq 0$ の積が $\geq 0$ であるという事実は、$\mathbf{R}$ が順序体であるというというによって表現できます。上記のすべての性質は、共通のからすべての順序体です。

#### 命題 2 {#top-iv-s3-prop-2 .statement tag=0BQG}

* 実数 $\neq 0$ の乗法群 $\mathbf{R}^*$ は、その部分群 $\mathbf{R}_+^*$ および $\mathbf{U}_0$ の積と同型のトポロジー 群です。ここで*

$$
\mathbf{U}_0 = \{ -1, +1 \}.
$$

それぞれの $x \neq 0$ について、$\operatorname{sgn} x$ は $\frac{x}{|x|}$ (*符号* $x$) を表します。 写像 $\operatorname{sgn}$ は、$\mathbf{R}^*$ の $\mathbf{U}_0$ 上の準同型です。 $x = |x|\operatorname{sgn} x$ があり、この $x$ の分解は、$\mathbf{R}_+^*$ の元の積と $\mathbf{U}_0$ の元は一意です。したがって、$\mathbf{R}^*$の群構造は、$\mathbf{R}_+^*$と$\mathbf{U}_0$の群構造の積です。一方、写像 $x \to |x|$ は連続であり、$x \neq 0$ 以降、$x \to \operatorname{sgn} x = \frac{x}{|x|}$ も連続です。したがって、結果は次のとおりです。
$\mathbf{R}$ の全体に $\operatorname{sgn} 0 = 0$ を入れることで、拡大する写像 $\operatorname{sgn}$ になります。

章 V (§ 4, no. 1, 定理 1) で、トポロジカル群 $\mathbf{R}_+^*$ が *加法* 群 $\mathbf{R}$ と *同型* であることがわかります。これでトポロジー 群 $\mathbf{R}_*$ の構造の決定が完了します。

### 3. *n*TH 根

$n$ を任意の整数 $> 0$ とします。 関係 $0 < x < y$ から、$n$ の帰納法によって、$0 < x^n < y^n$ と推定されます。他の語、写像 $x \to x^n$ は、$x \geq 0$ に対して *真に増加する* です。それは明らかに点ごとに連続であるため、(§ 2, no. 6, 定理 5) 区間 $I$ に対する $\mathbf{R}_+$ の同相写像です。一方、$x \geqslant 1$ は $x^{n-1} \geqslant 1$、つまり $x^n \geqslant x$ を意味するため、$I$ は有界ではないため、$I = \mathbf{R}_+$ となります。 写像 $x \to x^n$ の逆数の $x \geqslant 0$ に対する値は、$x^{1/n}$ または $\sqrt[n]{x}$ で表され、$x$ ～ 冪 $1/n$ または n 番目の根と呼ばれます。 $x$ ($n = 2, 3$ の場合は平方根、立方体根と言います。$n = 2$ の場合は $\sqrt[2]{x}$ の代わりに $\sqrt{x}$ と書きます)。したがって、正の数 $x^{1/n}$ は、方程式の一意の正の解として定義されます。

$$
y^n = x \quad (x \geqslant 0).
$$

特に、$x^2 = 2$ となるような実数 $x$ が存在しますが、有理数数にはこの性質がありません。したがって、有理線 $\mathbf{Q}$ は完全な空間ではないという事実がわかります。

写像 $\mathbf{R}_+$ の $x \to x^{1/n}$ は、真に増加するで連続です。 (2) までに $0^{1/n} = 0, 1^{1/n} = 1$ もできます

$$
(xy)^{1/n} = x^{1/n} y^{1/n};
$$

したがって、$x \to x^{1/n}$ はトポロジカル群 $\mathbf{R}_+^*$ の自己同型です。

章 V, § 4, no. 1 では、乗法群 $\mathbf{R}_+^*$ のすべての自己同型を見つけることで、この結果を一般化します。

### 練習問題 {#top-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
