---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 4
section_title: Exponentials and logarithms
lang: ja
source: top-v-x
pdf_pages: 0025-0029, 0034-0034
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 25
    - "no": 2
      title: BEHAVIOUR OF THE FUNCTIONS $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 27
    - "no": 3
      title: MULTIPLIABLE FAMILIES OF NUMBERS $> 0$
      page: 0
      pdf_page: 28
statements: 1
exercises: 2
content_sha256: 70e26478571c1a279b0d7f27b6132688ab8588161772668867655f84419d1782
translated_from: content/en/top/V/04_s4_exponentials_and_logarithms.md
translation_method: google
source_content_sha256: 55a9b7eecb6aa809fbac52ae103f840e9203fcdc0fe64340d7af904b5c851e60
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0e571bff04882bff4f2575eaa70d1a84c5f03f4e83e0774fa520d42c50f532bc
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 指数と対数

### 1. $a^x$ と $\log_a x$ の定義

#### 定理 1 {#top-v-s4-thm-1 .statement tag=0BW0}

*乗法群* $\mathbf{R}_+^*$ *of 実数* $> 0$ * は、加法群* $\mathbf{R}$ *of 実数* と同型のトポロジー 群です。

なぜなら、$\mathbf{R}_+^* = ]0, +\infty[$ は $\mathbf{R}$ の開区間であるため、$\mathbf{R}$ と *同相* です (章 IV, § 4, no. 1, 命題 1)。したがって、§ 3 の定理 2 により、それは $\mathbf{R}$ とトポロジカルな群 *同型* になります。

§ 1, no. 3 の系から命題 5 まで、各数 $a > 0$ には、$f_a(1) = a$ となる$\mathbf{R}$ から$\mathbf{R}_+^*$ への一意の連続準同型 $f_a$ があります。したがって、すべての $x \in \mathbf{R}$ とすべての $y \in \mathbf{R}$ について、

$$
f_a(x + y) = f_a(x) f_a(y), \qquad f_a(-x) = \frac{1}{f_a(x)},
$$

したがって、特にすべての $n \in \mathbf{Z}$ にとって、

$$
f_a(n) = a^n.
$$

このため、すべての $x \in \mathbf{R}$ に対して $f_a(x)$ を $a^x$ で表します。 写像 $a^x$ ($a > 0$ のすべての値) は *指数関数写像* と呼ばれます。すべての $x \in \mathbf{R}$ に対して $1^x = 1$ があります。 $a \neq 1$ の場合、$x \to a^x$ は群 $\mathbf{R}_+^*$ に対する群 $\mathbf{R}$ の *同型* です。

$a \neq 1$の場合、$x \to a^x$の逆数である$\mathbf{R}$に対する$\mathbf{R}_+^*$の同型を基底* $a$に対する*対数と呼び、その$x \in \mathbf{R}_+^*$における値は次のように表されます。 $\log_a x$。したがって、この記法では、

(1) $$
a^{x+y} = a^x a^y \qquad (x \in \mathbf{R}, y \in \mathbf{R}, a > 0);
$$
(2) $$
a^{-x} = \frac{1}{a^x} \qquad (x \in \mathbf{R}, a > 0);
$$
(3) $$
\log_a 1 = 0, \quad \log_a a = 1 \qquad (a > 0, a \neq 1);
$$
(4) $$
\log_a (xy) = \log_a x + \log_a y \qquad (x > 0, y > 0);
$$
(5) $$
\log_a \left( \frac{1}{x} \right) = -\log_a x \qquad (x > 0);
$$
(6) $$
a^{\log_a x} = x \qquad (x > 0);
$$
(7) $$
\log_a a^x = x \qquad (x \in \mathbf{R}).
$$

§ 1, no. 3 の命題 5 までに、$\mathbf{R}$ から $\mathbf{R}_+^*$ に至る連続するすべての準同型は形 $y \to a^{xy}$ であり、$x \in \mathbf{R}$ です。 $y = 1$ が $a^x$ のときの値なので、同じになります。

(8) $$
(a^x)^y = a^{xy} \qquad (x \in \mathbf{R}, \ y \in \mathbf{R}, \ a > 0),
$$
または、記法を変更すると、

(9) $$
x^y = a^{y \cdot \log_a x} \qquad (x > 0, y \in \mathbf{R}, a > 0, a \neq 1).
$$

公式 (8) は、整数 $n > 0$ ごとに $(a^{1/n})^n = a$ があり、章で定義された *n 番目の根* $\sqrt[n]{a}$ に導入された記法 $a^{1/n}$ が正当化されることを示しています。 IV, § 3, no. 3。

公式 (7) と (9) は次のことを示しています。

(10) $$
\log_a (x^y) = y \log_a x \qquad (x > 0, y \in \mathbf{R}),
$$
または、記法を変更すると、

(11) $$
\log_a x = \log_a b \cdot \log_b x \qquad (x > 0, a > 0, b > 0, a \neq 1, b \neq 1),
$$
これは、「基底の変更」の公式です。

最後に、トポロジカル群 $\mathbf{R}^*$ の *連続準同型* をすべてそれ自体に取得しましょう。 $g$ がそのような連続した準同型である場合、

$$
\log_a (g(a^x))
$$

は $\mathbf{R}$ から $\mathbf{R}$ への連続準同型であるため、(§ 1, no. 3, 命題 5) すべての $x \in \mathbf{R}$ に対して $\log_a (g(a^x)) = \alpha x$ となるような $\alpha \in \mathbf{R}$ が存在します。したがって、(8) により、すべての $x > 0$ に対して $g(x) = x^\alpha$ となります。したがって、同様に

(12) $$
(xy)^\alpha = x^\alpha y^\alpha \text{ for all } x > 0, y > 0 \text{ and } \alpha \in \mathbf{R}.
$$

公式 (4) が乗法から加法ごとに簡約する (通例の系がよく適用される唯一の演算) であるため、対数は長い間、数値計算に不可欠な手段でした (歴史的注意からこの章を参照)。

この目的で使用される場合、選択される基底は $a = 10$ です。そして、写像 $\log_{10} x$ のうち値を与える表があります (ある程度の近似値)。分析すると、$\lim_{x \to 1, x \neq 1} \frac{\log_e x}{(x - 1)} = 1$ (cf. 練習問題 1) のような、選ぶ別の基底 ($e$ で示されます) が導き出されます。

### 2. 写像 $a^x$ および $\log_a x$ の動作

$a \neq 1, x \to a^x$ が厳密に単調である場合、章 IV, § 2, no. 6 の定理 5 までに、$\mathbf{R}$ の区間 $\mathbf{R}_+^* = ]0, + \infty[$ への写像が入ります。 $a > 1$ の場合、$a^1 = a \geq 1 = a^0$ があるため、$a^x$ は真に増加するになります。さらに、$\mathbf{R}_+^*$ は上に有界ではないため、$a^x$ は $\mathbf{R}$ の上に有界ではないため、

$$
\lim_{x \to +\infty} a^x = +\infty \quad (a > 1)
$$

そして、(2)により、

$$
\lim_{x \to -\infty} a^x = 0 \quad (a > 1).
$$

一方、$a < 1$の場合、写像$a^x$は真に減少するで、$x$は$+\infty$になる傾向があるので0になる傾向があり、$x$は$-\infty$になる傾向があるので$+\infty$になる傾向があります（図1）。

![y = a^x (a > 1) および y = a^x (a < 1) を示すグラフ](https://i.imgur.com/1.png)

図1.

![y = log_a x (a > 1) および y = log_a x (a < 1) を示すグラフ](https://i.imgur.com/2.png)

図2.

これらの性質と (12) から、$0 < a < b$ の場合、$x > 0$ には $a^x < b^x$、$x < 0$ には $a^x > b^x$ があると推測します。 $x > 0$の場合は$\left(\frac{b}{a}\right)^x > 1$、$x < 0$の場合は$\left(\frac{b}{a}\right)^x < 1$。

$\mathbf{R}_+^*$ の $\log_a x$ の動作は、$\mathbf{R}$ の $a^x$ の動作から推定されます。 $a > 1$、写像 $\log_a x$ が真に増加するの場合、$x$ は $0$ になる傾向があるため、$-\infty$ になる傾向があり、$x$ は $+\infty$ になる傾向があるので、$+\infty$ になる傾向があります。 $a < 1$、写像 $\log_a x$が真に減少するの場合、$x$は$0$になる傾向があるため、$+\infty$になる傾向があり、$x$は$+\infty$になる傾向があるので、$-\infty$になる傾向があります（図2）。

写像 $a^x$ (それぞれ $\log_a x$) は、延長線 $\overline{\mathbf{R}}$ の部分集合で定義され、その値を $\overline{\mathbf{R}}$ に取り、 *連続性* により $\overline{\mathbf{R}}$ (それぞれ区間) に拡張できます。 $\overline{\mathbf{R}}$ の $[0, +\infty]$) に、点 $+\infty$ と $-\infty$ (それぞれ $0$ と $+\infty$) での制限値を割り当てます。

より一般的には、式 (9) は、関数 $x^y$ が $\overline{\mathbf{R}}^2$ の部分空間 $\mathbf{R}_+^* \times \mathbf{R}$ 上で連続であり、点 $(0, 0)$ を除き、$\mathbf{R}_+^* \times \mathbf{R}$ の閉包にある$\overline{\mathbf{R}}^2$ の任意の点 $(a, b)$ に$(x, y)$ が向かうときに極限に向かう傾向があることを示しています。 $(+\infty, 0)$、$(1, +\infty)$、$(1, -\infty)$。 したがって、極限が存在する $\overline{\mathbf{R}}^2$ の点への連続性により拡大する $x^y$ が可能です。アイデンティティの拡大の原則 (章 I, § 8, no. 1、命題 2、系 1)、公式 (1)、(4)、(8) は、両側に意味がある場合は常に有効です。

$x^y$ の連続性による拡大では、公式 $0^0 = 1$ を取得できないことに注意してください。

注意また、指数関数の定義により、すべての $a > 0$ について、$\mathbf{Z}$ で定義された拡大するから $\mathbf{R}$ 写像 $n \to a^n$ が可能になります。しかし、この方法では、$a < 0$のとき、この写像のうちの拡大は得られません。この写像の「自然な」 拡大は、分析写像の理論の項でのみ定義できます。

### 3. 数 $> 0$ の乗数家族

トポロジカル群 $\mathbf{R}$ と $\mathbf{R}_+^*$ の同型は、有限実数 $> 0$ の族 $(x_i)$ が *乗算可能* (章 IV, § 7, no. 4) であるためには、族 $(\log_a x_i)$ が次であることが必要かつ十分であることをすぐに示します。 *合計可能* ($a$ は数 $> 0$ および $\neq 1$ のいずれかです);そして私たちは持っています

$$
\prod_i x_i = a^{\sum \log_a x_i}.
$$

同様に、有限数 $> 0$ の数列 $(1 + u_n)$ によって定義される無限積は、一般項が $\log_a (1 + u_n)$ である系列が収束する場合に限り、*収束* (章 IV, § 7, no. 6) になります。私たちは持っています

$$
\prod_{n=0}^{\infty} (1 + u_n) = a^{S_{n=0}^{\infty} \log_a (1 + u_n)}.
$$

したがって、実数 $> 0$ の無限積の研究は、実数の無限系列の研究に還元され、その項は対数の形に現れます。この性質の和が対数の微分特性を使ってどのように簡単に研究できるかについては後で説明します。

### 練習問題 {#top-v-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
