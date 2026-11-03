---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 7
section_title: Infinite sums and products of real numbers
lang: ja
source: top-i-iv
book_pages: 363-372, 397-401
pdf_pages: 0369-0378, 0403-0407
extraction: ocr
subsections:
    - "no": 1
      title: FAMILIES OF POSITIVE FINITE NUMBERS SUMMABLE IN $\mathbf{R}$
      page: 364
      pdf_page: 370
    - "no": 2
      title: FAMILIES OF FINITE NUMBERS OF ARBITRARY SIGN SUMMABLE IN $\mathbf{R}$
      page: 366
      pdf_page: 372
    - "no": 3
      title: PRODUCT OF TWO INFINITE SUMS
      page: 367
      pdf_page: 373
    - "no": 4
      title: FAMILIES MULTIPLIABLE IN $\mathbf{R}^*$
      page: 367
      pdf_page: 373
    - "no": 5
      title: SUMMABLE FAMILIES AND MULTIPLIABLE FAMILIES IN $\overline{\mathbf{R}}$
      page: 369
      pdf_page: 375
    - "no": 6
      title: INFINITE SERIES AND INFINITE PRODUCTS OF REAL NUMBERS
      page: 370
      pdf_page: 376
statements: 20
exercises: 22
content_sha256: 80e5b5f1ea72966ae5415219b040aa2e4e7ae8b5755f81de72c2e888153e2d8e
translated_from: content/en/top/IV/07_s7_infinite_sums_and_products_of_real.md
translation_method: google
source_content_sha256: 455d0ffdcd364c6ed9f0b7d02c710c2c2c96a2ff460df4ccbbd8a2f0e2e71d59
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 94121cbd87d85b2096225b93fba2778c830cd9d3a9ec8650555acebad10b1bea
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 7. 実数の無限和と積

$\mathbf{R}$ のすべての点には、近傍の *可算* 基本系 (§ 1, no. 4、系から命題 3) があるため、*有限* 実数の族 $(x_t)$ は次のように合計できます。 $\mathbf{R}$は、添字の集合が$x_t \neq 0$が*可算*である場合のみです(章 III, § 5, no. 2、系から命題 1)。 $\mathbf{R}$ での要約可能なファミリーの研究は、したがって簡約するで本質的に要約可能な *数列* の研究になります。ただし、後で、有限実数の無算族 $(x_t)$ を考慮する必要があります。その項はパラメータ $t$ の写像です。この族はすべての $t$ について合計可能ですが、添字 $i$ の (可算) 集合が $x_i \neq 0$ が $t$ に依存することが起こります。このため、以下では添字集合の冪に仮定を課すことはしません。

### 1. 正の有限の族数 $\mathbf{R}$ で要約可能

#### 定理 1 {#top-iv-s7-thm-1 .statement tag=0BT9}

*ファミリー* $(x_i)$ *有限実数* $\geqslant 0$ *は $\mathbf{R}$ で加算可能です *ファミリーの部分有限和の集合が * $\mathbf{R}$ で上に制限されている場合に限ります。 *もしそうなら、この集合の最小上界は、家族*の和$(x_i)$です。

添字集合 $I$ のそれぞれの有限部分集合 $H$ を $s_H = \sum_{i \in H} x_i$ とします。 $x_i$ は $\geqslant 0$ であるため、関係 $H \subset H'$ は $s_H \leqslant s_{H'}$ を意味します。他の語、写像 $H \to s_H$ は、$I$ の有限部分集合の有向集合 $\mathfrak{F}(I)$ の *増加する* 写像です。したがって (§ 5, no. 2、系から定理 2) は、*上に制限されている*場合に限り、有限の極限を持ちます。

#### 注意 {#top-iv-s7-n1-rem-1 .statement tag=0BTA}

$(H_\lambda)$ を $I$ の有限部分集合の族とし、$I$ の各有限部分集合 $H$ に対して、$H \subset H_\lambda$ となる添字 $\lambda$ が存在するようにします。その場合、$(x_i)$ は、$s_{H_\lambda}$ の族が $\mathbf{R}$ で *上に制限されている*場合に限り、加算可能です。特に、$(x_n)$ を有限実数 $\geqslant 0$ の数列とし、それぞれの整数 $n$ を $s_n = \sum_{p=0}^n x_p$ とします。その場合、数列 $(x_n)$ は、真に増加する整数 $(n_k)$ の *1 つの数列* について、部分数列 $(s_{n_k})$ が $\mathbf{R}$ の *上に境界がある*場合に限り、$\mathbf{R}$ で加算可能です。

#### 例 {#top-iv-s7-n1-exa-4 .statement tag=0EAD}

1) $0 \leqslant q < 1$、数列 $(q^n)$ (「比 $q$ の等比数列」) が成り立つような各数 $q$ について、次のようにして$\mathbf{R}$ で合計できます。
$$
s_n = \frac{1 - q^{n+1}}{1 - q} \leqslant \frac{1}{1 - q}
$$
この数列の和は$\lim_{n \to \infty} s_n = \frac{1}{1 - q}$です。

2) $a$ と $b$ を 2 数として、$0 \leqslant a < 1$ と $0 \leqslant b < 1$ とします。その場合、ファミリー $(a^m b^n)_{(m, n) \in \mathbf{N} \times \mathbf{N}}$ は $\mathbf{R}$ で要約できます。それぞれ $\mathbf{N} \times \mathbf{N}$ の有限部分集合は形 $[0, p] \times [0, p]$ の部分集合に含まれており、
$$
\sum_{m=0}^p \sum_{n=0}^p a^m b^n = \left( \sum_{m=0}^p a^m \right) \left( \sum_{n=0}^p b^n \right) = \frac{1 - a^{p+1}}{1 - a} \cdot \frac{1 - b^{p+1}}{1 - b} \leqslant \frac{1}{(1 - a)(1 - b)}.
$$

3) それぞれの整数 $p > 1$、数列 $(n^{-p})$ ($n > 0$) は合計可能です。
$$
s_{2^n + 1} - s_{2^n} = \sum_{k=1}^{2^n} (2^n + k)^{-p} < 2^n \cdot (2^n)^{-p}
$$
したがって、これらの不等式を合計すると、
$$
s_{2^n} < \frac{1}{1 - 2^{1-p}}.
$$

4) 数列 $(1/n)$ ($n > 0$) は $\mathbf{R}$ で合計できません。
$$
s_{2^{n+1}} - s_{2^n} = \sum_{k=1}^{2^n} \frac{1}{2^n + k} > \frac{2^n}{2^{n+1}} = \frac{1}{2}
$$
したがって、これらの不等式を合計すると、
$$
s_{2^n} > n/2
$$
そのため、定理 1 の基準は満たされません。

5) $(I_n)$ を、相互に空ではない開いた互いに素区間の数列とし、すべては有限長 $l$ の区間に含まれます。この族の区間の有限数の長さの和は $\leq l$ ($§ 1$, no. 5) であるため、$I_n$ の長さの族は $\mathbf{R}$ で要約可能であり、その和は$\leq l$です。

#### 定理 2 (比較の原則) {#top-iv-s7-thm-2 .statement tag=0BTB}

*$(x_i)_{i \in I}$ *と* $(y_i)_{i \in I}$ *を有限実数* $\geq 0$の2つの族とし、*そのように* $x_i \leq y_i$ *すべて* $i$ とします。 *もし* $(y_i)$ *が* $\mathbf{R}$ *その場合* $(x_i)$も*、*そして* $\sum_i x_i \leq \sum_i y_i$が得られます。 *加法に添字* $x$ *$x_x < y_x$ がある場合、*その後* $\sum_i x_i < \sum_i y_i$ になります。

仮定は次のことを意味します。
$$
\sum_{i \in H} x_i \leq \sum_{i \in H} y_i,
$$
$I$ のすべての有限部分集合 $H$ と、定理の最初の部分がこれに続きます。 和に関連する不等式は、不等式の拡大の原則 ($§ 5$、no. 2、定理 1) から導き出されます。 $x_x < y_x$ の場合、
$$
\sum_i x_i = x_x + \sum_{i \neq x} x_i < y_x + \sum_{i \neq x} y_i = \sum_i y_i.
$$

この定理は、実数 $\geq 0$ の数列 $(x_n)$ が $\mathbf{R}$ で合計可能かどうかを決定するために最も一般的に使用される基準を提供します。つまり、指定された数列を、すでに知っているより単純な数列 $(y_n)$ と *比較* しようとします。それが集計可能かどうか。特定の点以降のすべての $n$ に対して $x_n \leq a y_n$ となるような有限の数 $a > 0$ が存在し、$(y_n)$ が加算可能である場合、$(x_n)$ は加算可能です。一方、特定の点以降のすべての $n$ に対して $x_n \geq b y_n$ となるような有限の数 $b > 0$ があり、$(y_n)$ が $\mathbf{R}$ で合計可能でない場合、$(x_n)$ は $\mathbf{R}$ で合計可能ではありません。最も頻繁に起こるケースにおいて、そのような比較数列がどのように得られるかを後の巻で見ていきます。

#### 例 1 {#top-iv-s7-n1-exa-1 .statement tag=0BTC}

$a$ を有限の実数 $> 0$ として、数列 $\left( \frac{a^n}{n!} \right)$ を考えます。 $n_0$ を最小の整数として、$a < n_0$ とします。次に、各 $n \geq n_0$ について、次のようになります。
$$
\frac{a^n}{n!} \leq \frac{a^{n_0}}{n_0!} \cdot \left( \frac{a}{n_0} \right)^{n-n_0};
$$
$q = \frac{a}{n_0} < 1$, 数列 $(q^{n-n_0})$ は加算可能であるため、数列 $\left( \frac{a^n}{n!} \right)$ も加算可能です。

#### 例 2 {#top-iv-s7-n1-exa-2 .statement tag=0BTD}

$(a_n)$ を正の数の合計可能な数列とします。以来
$$
\lim_{n \to \infty} a_n = 0,
$$
$n \geq n_0$ になるたびに $a_n \leq 1$ となるような整数 $n_0$ が存在します。従って、各 $n \geq n_0$ には $a_n^2 \leq a_n$ があり、したがって数列 $(a_n^2)$ は $\mathbf{R}$ で合計できます。 整数 $p > 1$ それぞれの数列 $(a_n^p)$ も同様です。

#### 例 3 {#top-iv-s7-n1-exa-3 .statement tag=0BTE}

$a$ と $b$ を 2 数 $< 1$ とします。それから
$$
\frac{1}{a^m + b^n} \leq \frac{1}{2(\sqrt{a})^m (\sqrt{b})^n}
$$
従って、ファミリー $\left( \frac{1}{a^m + b^n} \right)$ は $\mathbf{R}$ で要約できます。

#### 系 {#top-iv-s7-n1-cor-1 .statement tag=0BTF}

*$(x_i)_{i \in I}$ *を有限数* $\geq 0$ *in* $\mathbf{R}$ の加算可能な族とします。 *もし* $H$ *が* $I$のいずれかの部分集合であれば、 *私たちは*
$$
\sum_{i \in H} x_i \leq \sum_{i \in I} x_i,
$$
*そして等式は、* $x_i = 0$ *すべて* $i \in \complement H$ の場合にのみ成立します。

### 2. $\mathbf{R}$ で合計できる任意の記号の有限数の族

#### 定理 3 {#top-iv-s7-thm-3 .statement tag=0BTG}

*$(x_i)_{i \in I}$ *有限の実数の族とします。その場合、次の主張は同等です*:

a) *家族* $(x_i)$ *は* $\mathbf{R}$ で要約できます。
b) *家族* $(|x_i|)$ *は* $\mathbf{R}$ で要約できます。
c) 族* $(x_i)$ の有限部分和の *集合は、 * $\mathbf{R}$ で囲まれています*。

$I_1$ *すべての集合* $i \in I$ *そのような* $x_i \geq 0$、*および* $I_2$ *すべての集合* $i \in I$ *そのような* $x_i < 0$ とします。 *家族* $(x_i)_{i \in I}$ *[それぞれ$(|x_i|)_{i \in I}$] *各ファミリー* $(x_i)_{i \in I_1}$ *および* $(x_i)_{i \in I_2}$ *[それぞれの場合にのみ合計可能です。 $(|x_i|)_{i \in I_1}$ および $(|x_i|)_{i \in I_2}$] *加算可能* (章 III, § 5, no. 3、命題 2 および 3)。 *ここで、* $(x_i)_{i \in I_1}$ * は加算可能である、または* $(|x_i|)_{i \in I_1}$ * は加算可能である、または* 族 $(x_i)_{i \in I_1}$ の有限部分和の集合は有界 (no. 1, 定理 1) であると言うのと同じことになります。 $I_1$ を $I_2$ に置き換えても同様です。 定理がすぐに続きます。

定理 3 は、有限実数の族の $\mathbf{R}$ における総和可能性が、その絶対的な値の族の総和可能性にのみ依存することを示しています。

(章 III, § 5, no. 5, 命題 6) $(x_i)$ と $(y_i)$ が有限実数の 2 つの加算可能な族である場合、族 $(x_i + y_i)$ は加算可能であり、$\sum (x_i + y_i) = \sum x_i + \sum y_i$ であることを思い出します。さらに、$(x_i)$ が有限実数の加算可能な族で、$a$ が任意の有限実数である場合、族 $(ax_i)$ は $\mathbf{R}$ で加算可能で、$\sum ax_i = a \cdot \sum x_i$ が得られます。

### 3. 積 2 つの無限和

#### 命題 1 {#top-iv-s7-prop-1 .statement tag=0BTH}

*有限実数の族* $(x_\lambda)_{\lambda \in L}$ *と* $(y_\mu)_{\mu \in M}$ が* $\mathbf{R}$ で合計可能である場合、*そのとき族* $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ *そして次のようになります*

(1)
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu).
$$

$L \times M$ のすべての有限部分集合は形 $H \times K$ の有限部分集合に含まれます。ここで、$H$ は $L$ の有限部分集合であり、$K$ は $M$ の有限部分集合です。 仮定までに、$L$ と $M$ のすべての有限部分集合 $H$ と $K$ に対して $\sum_{\lambda \in H} |x_\lambda| \leq a$ と $\sum_{\mu \in K} |y_\mu| \leq a$ が存在するような数 $a > 0$ が存在します。したがって
$$
\sum_{(\lambda, \mu) \in H \times K} |x_\lambda y_\mu| = (\sum_{\lambda \in H} |x_\lambda|) (\sum_{\mu \in K} |y_\mu|) \leq a^2,
$$
これは、族 $(x_\lambda y_\mu)$ が定理 1 と 3 によって $\mathbf{R}$ で合計可能であることを示しています。結合性により、[章 III, § 5, no. 3, 公式 (2)] と書くことができます。
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \sum_{\lambda \in L} (\sum_{\mu \in M} x_\lambda y_\mu) = \sum_{\lambda \in L} x_\lambda (\sum_{\mu \in M} y_\mu) = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu);
$$
したがって結果です。

### 4. 家族は$\mathbf{R}^*$で乗算可能

有限非ゼロ実数の乗法群 $\mathbf{R}^*$ では、族 $(x_i)_{i \in I}$ は、$I$ (章 III, § 5, no. 2, 命題 1) の有限部分集合の補数のフィルターに関して $\lim x_i = 1$ の場合にのみ乗算可能です。 特に、$x_i < 0$ のような添字 $i$ の *有限* 数のみが存在し得ます。 したがって、私たちは、すべての条件が厳密に肯定的な家族 $x_i$ のみを考慮することに限定するかもしれません。次に、$x_i = 1 + u_i$ を置くと便利です。ここで、$u_i$ は、すべての $i$ に対して不等式 $-1 < u_i < +\infty$ の影響を受けます。 $\mathbf{R}^*$ のそれぞれの点には、近傍の可算基本系、添字 $i$ の集合があるため、家族 $(1 + u_i)$ が $\mathbf{R}^*$ で乗算できる場合、$u_i \neq 0$ は可算になります。

#### 定理 4 {#top-iv-s7-thm-4 .statement tag=0BTI}

*ファミリー* $(1 + u_i)$ *は乗算可能* $\mathbf{R}^*$ *ファミリー* $(u_i)$ *が加算可能* $\mathbf{R}$である場合に限ります。
#### 補題 (i) {#top-iv-s7-n4-lem-1 .statement tag=0BTJ}

*もし* $(a_i)_{1 \leq i \leq p}$ *が数* $> 0$ の有限列である場合、 *その後*
$$
\prod_{i=1}^p (1 + a_i) \geq 1 + \sum_{i=1}^p a_i.
$$
(ii) *また* $a_i < 1$ *それぞれ* $i$、*その後*
$$
\prod_{i=1}^p (1 - a_i) \geq 1 - \sum_{i=1}^p a_i.
$$

これらの不等式は $p = 1$ であれば明らかであり、$p$ の帰納法によって証明されます。もし
$$
\prod_{i=1}^{p-1} (1 + a_i) \geq 1 + \sum_{i=1}^{p-1} a_i,
$$
私たちは持っています
$$
\prod_{i=1}^p (1 + a_i) \geq (1 + a_p) \left( 1 + \sum_{i=1}^{p-1} a_i \right) = 1 + \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 + \sum_{i=1}^p a_i.
$$
もう一度言いますが、
$$
\prod_{i=1}^{p-1} (1 - a_i) \geq 1 - \sum_{i=1}^{p-1} a_i,
$$
私たちは持っています
$$
\prod_{i=1}^p (1 - a_i) \geq (1 - a_p) \left( 1 - \sum_{i=1}^{p-1} a_i \right) = 1 - \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 - \sum_{i=1}^p a_i.
$$

補題を証明したので、$\mathbf{R}^*$ は完全な群 (章 III, § 5, no. 3, 命題 2) であるため、族 $(1 + u_i)$ が乗算可能な場合、族 $(1 + u_i^+)$ と $(1 - u_i^-)$ も乗算可能であることに注意してください。逆に、族 $(1 + u_i^+)$ と $(1 - u_i^-)$ が乗算可能な場合、$(1 + u_i)$ (章 III, § 5, no. 3, 命題 3) も乗算可能です。したがって、すべての$u_i$が$\geq 0$である場合と、すべてが$\geq 0$である場合のみを考慮する必要があります。

まず、すべての $i$ に対して $u_i \geq 0$ であると仮定します。ファミリ $(1 + u_i)$ が乗算可能な場合、各 $\varepsilon > 0$ には、$I$ の添字集合の有限部分集合 $J$ が存在し、それぞれの有限部分集合 $H$ の $I$ が成立します。 $J$ から互いに素は $1 \leq \prod_{i \in H} (1 + u_i) \leq 1 + \varepsilon$ になります。 (2) により、$\sum_{i \in H} u_i \leq \varepsilon$ となり、コーシーの基準 (章 III, § 5, no. 2, 定理 1) により、$(u_i)$ が $\mathbf{R}$ で合計可能であることがわかります。

逆に、$(u_i)$ が $\mathbf{R}$ で合計できるとします。 $0 < \varepsilon < 1$ のような各 $\varepsilon$ には、$I$ の有限部分集合 $J$ があり、$J$ からの $I$ 互いに素のそれぞれの有限部分集合 $H$ について、次のようになります。 $0 \leq \sum_{i \in H} u_i \leq \varepsilon$。したがって、(3) により、$\prod_{i \in H} (1 - u_i) \geq 1 - \varepsilon$ が得られます。しかし、$0 \leq u < 1$ などの数 $u$ ごとに $1 + u \leq \frac{1}{1 - u}$ なので、次のようになります。

$$
1 \leq \prod_{i \in H} (1 + u_i) \leq \frac{1}{1 - \varepsilon},
$$

これは、$(1 + u_i)$ が乗算可能であることを示しています (コーシーの基準)。

証明は、$u_i$ がすべて $\leq 0$ の場合に似ています。 $(1 + u_i)$ が乗算可能な場合に $(u_i)$ が加算可能であることを示すには、公式 (2) と不等式 $1 - u \leq \frac{1}{1 + u}$ ($0 \leq u < 1$) を使用します。 $(u_i)$ が加算可能である場合に $(1 + u_i)$ が乗算可能であることを示すには、公式 (3) を使用します。

章 V (§ 4) では、群 $\mathbf{R}^*$ のトポロジカルな研究により、対数写像の助けを借りて、$\mathbf{R}^*$ における族の乗算性に対する他のの基準を与えることができます。後の巻では、対数の微分特性を使用して、この基準と上記の基準の同値を確立します。

### 5. $\overline{\mathbf{R}}$ の加算可能な家族と重複可能な家族

$\overline{\mathbf{R}}$ の区間 $[0, + \infty]$ では、加法は合成 (§ 4, no. 3) の結合および可換法則です。したがって、この区間の数の *加算可能な* ファミリの概念が定義されます (章 III, § 5, no. 1, 注意 3)。

#### 命題 2 {#top-iv-s7-prop-2 .statement tag=0BTK}

*すべての家族* $(x_i)$ *のうち実数* $\geq 0$ *は $\overline{\mathbf{R}}$ で合計できます。

有向集合 $\mathfrak{F}(I)$ の写像 $H \to s_H$ を $\overline{\mathbf{R}}$ にすると *増加する* になります。したがって (§ 5, no. 2, 定理 2) は極限になります。

同じ推論は、実数 $\leq 0$ のすべての族が $\overline{\mathbf{R}}$ で合計可能であることを示しています。

同様に、乗法は、区間 $[0, 1]$ と $\overline{\mathbf{R}}$ の$[1, + \infty]$ のそれぞれにおける合成の結合的かつ可換な法則であるため、乗法族の概念はこれらの区間のそれぞれに対して定義されます。

#### 命題 3 {#top-iv-s7-prop-3 .statement tag=0BTL}

すべての家族 $(1 + u_i)$ [それぞれ数 $\geq 1$ (それぞれ $\geq 0$ と $\leq 1$) の $(1 - u_i)$ は $\overline{\mathbf{R}}$ で乗算できます。

証明は命題 2 と同じです。

#### 系 {#top-iv-s7-n5-cor-1 .statement tag=0BTM}

積 $\prod (1 + u_i)$ [それぞれ数 $\geq 1$ (それぞれ $> 0$ および $\leq 1$) の $\prod (1 - u_i)$] は、$\sum u_i = + \infty$ の場合に限り、$+ \infty$ (それぞれ 0) に等しくなります。

なぜなら、$\sum u_i$ が有限である場合、$\prod (1 + u_i)$ と $\prod (1 - u_i)$ は $\mathbf{R}^*$ にあり、その逆は (no. 4、定理 4) であるからです。

#### 注意 {#top-iv-s7-n5-rem-1 .statement tag=0BTN}

結合性 (章 III, § 5, no. 3, 定理 2) の定理は、G が $\overline{\mathbf{R}}$ に置き換えられ、$x_i$ が $\geq 0$ であると仮定される場合でも有効です。 $\sum_{i \in I} x_i$ が有限であればこれは明らかです。逆に、$\sum_{i \in I} x_i = + \infty$ だったとします。次に、各有限 $a > 0$ に対して、$\sum_{i \in H} x_i \geq a$ となるような I の有限部分集合 H があります。 K を $H \subset \bigcup_{\lambda \in K} I_\lambda$ となるような L の有限部分集合とします。 $s_\lambda \geq \sum_{i \in I_\lambda \cap H} x_i$ 以降、すべての $\lambda \in K$ に対して、
$$
\sum_{\lambda \in K} s_\lambda \geq \sum_{i \in H} x_i \geq a,
$$
これは $\sum_{\lambda \in L} s_\lambda = + \infty$ を示しています。 $[0, 1]$ または $[1, + \infty]$ の数の乗法族に対して類似の命題を定式化する作業は読者に任せます。

### 6. 無限系列と実数の無限積

有限実数の系列は、$\mathbf{R}$で収束する場合、単に収束するといいます。

#### 定義 1 {#top-iv-s7-def-1 .statement tag=0BTO}

有限実数の系列は、その項の絶対値の系列が収束する場合、絶対収束するといいます。

#### 命題 4 {#top-iv-s7-prop-4 .statement tag=0BTP}

有限実数の系列は、絶対収束する場合に限り、可換収束します。

これは、no. 2 の章 III, § 5, no. 7、命題 9、および定理 3 から続きます。

他の語において、$(u_n)$が有限実数の数列であれば、一般項が$u_n$である系列が可換収束する、あるいは絶対収束する、あるいは数列が言えることは同じことになります。 $(u_n)$ は $\mathbf{R}$ で要約できます。したがって、章 III, § 5 で証明された加算可能な族のすべての特性は、絶対収束する系列に適用されます。特に、一般項が $u_n$ である系列が絶対収束する場合、$\mathbf{N}$ のすべての部分集合 $H$ に対して和 $\sum_{n \in H} u_n$ が存在します。そして、$(H_p)$ が $\mathbf{N}$ の分割である場合、次のようになります。
$$
\sum_{n=0}^{\infty} u_n = \sum_p \left( \sum_{n \in H_p} u_n \right)
$$
*(絶対収束系列の結合性*)。

章 III, § 5 ですでに述べたように、実数の系列は可換収束せずに、つまり絶対収束せずに収束する可能性があります。

#### 例 {#top-iv-s7-n6-exa-1 .statement tag=0BTQ}

*交代的系列.* 有限実数の数列 $(u_n)$ によって定義される系列は、$u_n = (-1)^n v_n$ の場合 *交代的* と呼ばれます。ここで、すべての $n$ に対して $v_n \geq 0$ となります。このような系列の収束に *十分な* 条件は、*数列* $(v_n)$ *減少し、その極限* として 0 * を持つことであることを示しましょう。 $s_n$ が示す場合
$$
\sum_{p=0}^{n} u_p,
$$
仮定 $(v_n)$ が減少するであるということは、次のことを意味します。
$$
s_{2n+1} \leq s_{2n+3} \leq s_{2n+2} \leq s_{2n}
$$
$n \geq 0$の皆さんへ。 数列 $(s_{2n})$ [それぞれ$(s_{2n+1})$] は減少するで下に境界があり (それぞれ増加するで上に境界がある)、したがって有限の極限 $a$ (それぞれ $b$) と $b \leq a$ があります。それ以来
$$
a - b = \lim_{n \to \infty} (s_{2n} - s_{2n+1}) = \lim_{n \to \infty} v_{2n+1} = 0,
$$
主張が証明されました。

$v_n = 1/n$ を例にとると、上記の条件が満たされるため、一般項が $(-1)^n / n$ (「交代的高調波系列」) である系列が収束します。 no. 1 で、一般的な項が​​ $1/n$ (「高調波系列」) である系列は収束せず、したがって交代的高調波系列は完全には収束しません。

(章 III, § 5, no. 6, 命題 7) $(u_n)$ と $(v_n)$ が有限実数の 2 つの収束系列である場合、系列 $(u_n + v_n)$ は収束することを思い出してください。
$$
\sum_{n=0}^{\infty} (u_n + v_n) = \sum_{n=0}^{\infty} u_n + \sum_{n=0}^{\infty} v_n;
$$
また、系列 $(u_n)$ が収束する場合、系列 $(au_n)$ はすべての有限実数 $a$ および $\sum_{n=0}^{\infty} au_n = a \cdot \sum_{n=0}^{\infty} u_n$ に対して収束します。

最後に、系列 $(u_n)$ と $(v_n)$ が収束し、すべての $n$ に対して $u_n \leq v_n$ であれば、拡大の不等式原理 (§ 5, no. 2, 定理 1) により $\sum_{n=0}^{\infty} u_n \leq \sum_{n=0}^{\infty} v_n$ が得られます。

系列 $(v_n)$ は収束するが完全には収束しないと仮定し、各 $n$ に対して $|u_n| \leq |v_n|$ を仮定した場合、$u_n = |v_n|$ をとればわかるように、系列 $(u_n)$ が収束するとは決して推論できないことに注意してください。

有限非ゼロ実数の無限積は、$\mathbf{R}^*$ で収束する場合、単純に収束すると言えます。その値は有限の非ゼロ実数になります。

#### 定義 2 {#top-iv-s7-def-2 .statement tag=0BTR}

*一般因子が $1 + u_n$ である無限積は、一般因子が $1 + |u_n|$ である積が収束する場合、絶対収束するといいます。

#### 命題 5 {#top-iv-s7-prop-5 .statement tag=0BTS}

*有限実数の無限積は、絶対収束する場合にのみ可換収束します。*

これは、上記の章 III, § 5, no. 7、命題 9、および定理 4 から続きます。

さらに、一般因子が $1 + u_n$ である積は、一般項が $u_n$ である系列が *絶対収束* である場合に限り、*絶対収束* になります。

非ゼロ実数の積は、可換収束せずに、つまり絶対収束せずに収束する可能性があります。

#### 例 {#top-iv-s7-n6-exa-2 .statement tag=0BTT}

$n \geq 2$ に対して $u_{2n-1} = -1/n$ と $u_{2n} = 1/n$ をとった場合、系列 $(u_n)$ は絶対的に収束しないため、積 $(1 + u_n)$ は絶対的に収束しません。しかしそれ以来

$$
\prod_{p=3}^{n} (1 + u_p) = \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
そして
$$
\prod_{p=3}^{2n+1} (1 + u_p) = \left(1 - \frac{1}{n+1}\right) \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
定理 4 から、積は収束し、その値は
$$
\prod_{n=2}^{\infty} \left(1 - \frac{1}{n^2}\right).
$$

さらに、一般的な項が$u_n$である系列の*収束*は、一般的な因子が$1 + u_n$である積の*収束*には*必要でも十分でもない*ことに注意する必要があります(練習問題21および22を参照)。

### 練習問題 {#top-iv-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
