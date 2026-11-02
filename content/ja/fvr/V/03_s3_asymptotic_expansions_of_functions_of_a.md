---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 3
section_title: ASYMPTOTIC EXPANSIONS OF FUNCTIONS OF A REAL VARIABLE
lang: ja
source: fvr-i-vii
book_pages: 227-236, 260-261
pdf_pages: 0242-0251, 0275-0276
extraction: ocr
subsections:
    - "no": 1
      title: 'INTEGRATION OF COMPARISON RELATIONS: **I. WEAK RELATIONS**'
      page: 228
      pdf_page: 243
    - "no": 2
      title: 'APPLICATION: LOGARITHMIC CRITERIA FOR CONVERGENCE OF INTEGRALS'
      page: 229
      pdf_page: 244
    - "no": 3
      title: 'INTEGRATION OF COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 230
      pdf_page: 245
    - "no": 4
      title: DIFFERENTIATION OF COMPARISON RELATIONS
      page: 232
      pdf_page: 247
    - "no": 5
      title: PRINCIPAL PART OF A PRIMITIVE
      page: 233
      pdf_page: 248
    - "no": 6
      title: ASYMPTOTIC EXPANSION OF A PRIMITIVE
      page: 235
      pdf_page: 250
statements: 24
exercises: 7
content_sha256: 13004b1947f95c11a7e0fcc3efb1502a1db3da89433592d5bb10f9d20b31f2fd
translated_from: content/en/fvr/V/03_s3_asymptotic_expansions_of_functions_of_a.md
translation_method: google
source_content_sha256: 8e759b487c91cd2169288cb7a854bc7596023e144f6eac992de79d1711257975
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 96a65a6ac8aa0fe18cd029508ed4473ec7fa4e8b2398c43477377872fa683844
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。実数変数の写像の漸近展開

In this section we shall consider only the case where the set $E$ is an open interval in the extended real line $\overline{\mathbf{R}}$, and $\mathfrak{F}$ is a base for the trace on $E$ of the filter of neighbourhoods of the left or right-hand endpoint $\alpha$ of $E$; further, we shall study above all the (finite) real functions defined on a set in $\mathfrak{F}$ (depending on the function under consideration).

必要に応じて変数 $x' = -x,\ x' = \frac{1}{x-\alpha},\ x' = -\frac{1}{x-\alpha}$ の変更の 1 つを使用すると、E が形 ]$a, +\infty[$ の区間である場合に常に簡約するを適用でき、$\mathfrak{F}$ は区間 $[t, +\infty[$ と $t > a$ で形成されます。私たちは主に後者の場合に限定し、いくつかの特に重要な結果を除いて、(上記の変数の変更によって) 得られる命題のほとんどを翻訳するタスクを読者に任せます。

言葉の乱用を利用して、$\mathfrak{F}$の集合を「$+\infty$の近傍」と呼ぶと便利です。

### 1. 比較関係: **I の統合。弱い関係**

#### 命題 1 {#fvr-v-s3-prop-1 .statement tag=08F4}

*$\mathbf{f}$ を規制のベクトル写像、$g$ を規制の写像 $\geqslant 0$ として区間 $[a, +\infty[$ に$\int_a^{+\infty} g(t)\,dt > 0$ とする。 $x$ が $+\infty$ になる傾向があるため、関係 $\mathbf{f} \preccurlyeq g$ は $\int_a^x \mathbf{f}(t)\,dt \preccurlyeq \int_a^x g(t)\,dt$ を暗示します。整 $\int_a^{+\infty} g(t)\,dt$ が収束すると、整 $\int_a^{+\infty} \mathbf{f}(t)\,dt$ は絶対に収束します。*

実際、仮定までに、次のような $b \geqslant a$ と数 $c' > 0$ が存在します。
$$
\| \mathbf{f}(x) \| \leqslant c' g(x) \quad \text{for } x \geqslant b,
$$
よって
$$
\left\| \int_b^x \mathbf{f}(t)\,dt \right\| \leqslant \int_b^x \| \mathbf{f}(t) \| \,dt \leqslant c' \int_b^x g(t)\,dt;
$$
さらに、$b$ は $\int_a^b g(t)\,dt > 0$ よりも大きいと想定できるため、$\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leqslant c'' \int_a^b g(t)\,dt$ となるような $c'' > 0$ が存在するからです。 $c = \max(c', c'')$ を置くと、このようになります
$$
\left\| \int_a^x \mathbf{f}(t)\,dt \right\| \leqslant c \int_a^x g(t)\,dt
$$
$x \geqslant b$、よって命題ごとに。

#### 系 1 {#fvr-v-s3-prop-1-cor-1 .statement tag=08F5}

*$f$と$g$が区間$[a, +\infty[$に写像と$\geqslant 0$が規制されている場合、$f \succcurlyeq g$、$\int_a^{+\infty} g(t)\,dt = +\infty$の場合は$\int_a^{+\infty} f(t)\,dt = +\infty$となります。

#### 系 2 {#fvr-v-s3-prop-1-cor-2 .statement tag=08F6}

*$f$ と $g$ が $\geqslant 0$ で、$[a, +\infty[$ では零と同一ではなく、$f \succeq g$ である場合、$\int_a^x f(t)\,dt \succeq \int_a^x g(t)\,dt$ となります。*

### 2. 応用: 積分の収束のための対数基準

写像 g を適切に選択することで、写像 $f \geq 0$ の積分 $\int_a^{+\infty} f(t) \, dt$ が収束するか無限であるかを決定するための基準を prop から推測できます。 V、p. 228、cor の 1 つ1 これに対して、プリミティブが既知の g 写像に対して選ぶで十分です。特に、$x^\mu$ は、$\mu \neq -1$ のときは原始的な $\frac{x^{\mu+1}}{\mu+1}$ を持ち、$\mu = -1$ のときは $\log x$ を持つため、次の基準があります。

#### 命題 2 (「位数 0 の対数基準」) {#fvr-v-s3-prop-2 .statement tag=08F7}

*f を区間 $[a, +\infty[$ で規制されている写像 $\geq 0$ とします。ある $\mu < -1$ に対して $f(x) \preccurlyeq x^\mu$ であれば、積分 $\int_a^{+\infty} f(t) \, dt$ は収束します。ある$\mu \geq -1$に対して$f(x) \succcurlyeq x^\mu$であれば、積分$\int_a^{+\infty} f(t) \, dt$は無限大です。*

この基準は、たとえば、$f(x) = 1/x(\log x)^\mu$ ($\mu > 0$) の場合のように、*すべて* 指数 $\alpha > 0$ が $1/x^{1+\alpha} \ll f(x) \ll 1/x$ の場合には決定的ではありません。しかし、この最後のケースでは、 f は、$\mu \neq 1$ の場合は原始 $\frac{1}{1-\mu} (\log x)^{1-\mu}$ を持ち、$\mu = 1$ の場合は $\log \log x$ を持ちます。したがって:

#### 命題 3 (「位数 1 の対数基準」) {#fvr-v-s3-prop-3 .statement tag=08F8}

* f を区間 $[a, +\infty[$ で規制されている写像 $\geq 0$ とします。ある $\mu > 1$ に対して $f(x) \preccurlyeq 1/x(\log x)^\mu$ であれば、積分 $\int_a^{+\infty} f(t) \, dt$ は収束します。ある $\mu \leq 1$ に対して $f(x) \succcurlyeq 1/x(\log x)^\mu$ がある場合、積分 $\int_a^{+\infty} f(t) \, dt$ は無限大です。*

一般に、すべての整数 $n \geq 0$ について、$n \geq 1$ に対して関係 $l_0(x) = x$、$l_n(x) = \log(l_{n-1}(x))$ によって帰納的に (x が十分大きい場合) 定義された $l_n(x)$ 写像で表します。ある人は、$l_n(x)$ は x* の *n* 回目の *反復対数 (cf. 付録) であると言います。 $\frac{1}{1-\mu} (l_n(x))^{1-\mu}$ が次のプリミティブであることがすぐに検証されます。

$$
\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}
$$

$\mu \neq 1$ の場合、$l_{n+1}(x)$ は $\frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) l_n(x)}$ のプリミティブです。したがって、次のようになります。

#### 命題 4 (「位数 n の対数基準」) {#fvr-v-s3-prop-4 .statement tag=08F9}

* f を区間 $[a, +\infty[$ で規制されている写像 $\geq 0$ とします。ある $\mu > 1$、$f(x) \preccurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}$ について、積分 $\int_a^{+\infty} f(t) \, dt$ は収束します。ある$\mu \leq 1$に対して$f(x) \succcurlyeq \frac{1}{x l_1(x) l_2(x) \ldots l_{n-1}(x) (l_n(x))^\mu}$であれば、積分$\int_a^{+\infty} f(t) \, dt$は無限大です。*

したがって、各対数基準は、下位の位数の基準が決定的ではない写像 (*cf.* V、p. 264、練習問題 5 b) および V、p. 265、練習問題 5 b) に適用できます。 8)。

その有用性のため、$f$ が規制されている積分 $\int_{\alpha}^{a} f(t) \, dt$ および非コンパクト区間 $]\alpha, a]$ の $\geq 0$ の基準位数 0 を変換します。

#### 命題 5 (「位数 0 の対数基準」) {#fvr-v-s3-prop-5 .statement tag=08FA}

*$\alpha$ の近傍で、一部の $\mu < 1$ に対して $f(x) \leq 1/(x-\alpha)^{\mu}$ がある場合、積分 $\int_{\alpha}^{a} f(t) \, dt$ は収束します。ある $\mu \geq 1$ に対して $f(x) \geq 1/(x-\alpha)^{\mu}$ であれば、積分 $\int_{\alpha}^{a} f(t) \, dt$ は無限大です。*

位数 $n$ の対数基準を同様に翻訳するかどうかは読者に任せます。

対数基準の適用は、これらの基準の特徴である比較スケール含む写像に関して $f$ の *主部分* を取得する方法を知っている場合、明らかです: $f_1$ が主部分である場合、積分 $\int_{\alpha}^{+\infty} f(t) \, dt$収束するか、$\int_{\alpha}^{+\infty} f_1(t) \, dt$ とともに無限となり、対数基準がこの最後の積分に直ちに適用されます。

#### 例 1 {#fvr-v-s3-n2-exa-1 .statement tag=08FB}

$p < 0$ または $q < 0$ の場合、写像 $t^p(1-t)^q$ は $]0, 1[$ で制限されません。 点 0 と 1 の近傍に適用される位数 0 の対数基準により、$p > -1$ と $q > -1$ の場合に限り、整$\int_{0}^{1} t^p(1-t)^q \, dt$ は収束します。そうである場合、この積分は *第一種オイラー積分* と呼ばれ、$\mathbf{B}(p+1, q+1)$ (*cf.* VII, p. 312) で表されます。

#### 例 2 {#fvr-v-s3-n2-exa-2 .statement tag=08FC}

整$\int_{0}^{+\infty} t^{\lambda-1} e^{-t} \, dt$を考えてみましょう。 0 の近傍に $e^{-t} \sim 1$ があるため、この積分が収束するには $\lambda > 0$ が必要です。 $+\infty$ の近傍では、任意の $\mu > 0$ に対して $e^{-t} \ll t^{-\mu}$ があるため、この条件でも十分です。 $x > 0$ のとき、積分は *第 2 種オイラー積分* と呼ばれ、$\Gamma(x)$ (*cf.* VII, p. 311) で表されます。

### 3. 比較関係:IIの統合。強い関係

#### 命題 6 {#fvr-v-s3-prop-6 .statement tag=08FD}

*$\mathbf{f}$ を規制のベクトル写像とし、$g$ を $[a, +\infty[$ の規制の写像 $\geq 0$ とします。

1. *整 $\int_{a}^{+\infty} g(t) \, dt$ が収束すると、関係 $\mathbf{f} \ll g$ (それぞれ $\mathbf{f} \sim c g$、$c$ は定数) は $\int_{x}^{+\infty} \mathbf{f}(t) \, dt \ll \int_{x}^{+\infty} g(t) \, dt$ (それぞれ $\int_{x}^{+\infty} \mathbf{f}(t) \, dt \sim c \int_{x}^{+\infty} g(t) \, dt$) を意味します。

2. *整 $\int_{a}^{+\infty} g(t) \, dt$ が無限である場合、関係 $\mathbf{f} \ll g$ (それぞれ $\mathbf{f} \sim c g$) は次のことを意味します*
$$
\int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \ll \int_{\beta}^{\gamma} g(t) \, dt \quad \text{(resp. } \int_{\alpha}^{\gamma} \mathbf{f}(t) \, dt \sim c \int_{\beta}^{\gamma} g(t) \, dt),
$$
*$[a, +\infty[$* の任意の $\alpha$ と $\beta$。

$c \neq 0$ の場合、関係 $\mathbf{f} \sim c g$ は $\mathbf{f} - c g \ll g$ と同等であるため、関係 $\mathbf{f} \ll g$ に対して命題を証明するだけで十分です。

最初の部分は、値定理の平均値明らか帰結です。なぜなら、$x \geq x_0$ に対して $\| \mathbf{f}(x) \| \leq \varepsilon g(x)$ を仮定すると、次のように推測できるからです。

$$
\left\| \int_{x}^{+\infty} \mathbf{f}(t) \, dt \right\| \leq \int_{x}^{+\infty} \| \mathbf{f}(t) \| \, dt \leq \varepsilon \int_{x}^{+\infty} g(t) \, dt \quad \text{for } x \geq x_0.
$$

次に$\int_{a}^{+\infty} g(t) \, dt = +\infty$とします。 $\| \mathbf{f}(x) \| \leq \varepsilon g(x)$ が $x \geq x_0 \geq \max(\alpha, \beta)$ の場合、1 つは

$$
\begin{align*}
\int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt &= \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \int_{x_0}^{x} \| \mathbf{f}(t) \| \, dt \\
&\leq \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt + \varepsilon \int_{x_0}^{x} g(t) \, dt \\
&= \varepsilon \int_{\beta}^{x} g(t) \, dt + \left( \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right).
\end{align*}
$$

現在、$x \geq x_1$ ごとに次のような $x_1 \geq x_0$ が存在します。

$$
\left| \int_{\alpha}^{x_0} \| \mathbf{f}(t) \| \, dt - \varepsilon \int_{\beta}^{x_0} g(t) \, dt \right| \leq \varepsilon \int_{\beta}^{x} g(t) \, dt
$$

よって、$x \geq x_1$

$$
\left\| \int_{\alpha}^{x} \mathbf{f}(t) \, dt \right\| \leq \int_{\alpha}^{x} \| \mathbf{f}(t) \| \, dt \leq 2\varepsilon \int_{\beta}^{x} g(t) \, dt
$$

$\varepsilon > 0$ は任意なので、これで証明が完成します。

他の語では、$g$が区間$[a, +\infty[$で正であり、関係が2つの項のプリミティブの間に持続する場合、強い関係$\mathbf{f} \ll g$、$\mathbf{f} \sim \mathbf{a}g$の2つの項を統合できます。ただし、$\int_{a}^{+\infty} g(t) \, dt$ が収束する場合は $x$ から $+\infty$ まで、逆の場合は $\alpha$ から $x$ ($[a, +\infty[$ のすべての $\alpha$ について) を積分するように注意する必要があります。

小道具に注意してください。 1 (V、p. 228) および 6 (V、p. 230) は、可算集合の補数の区間 $[t, +\infty[$ ($t > a$) のトレースフィルターに対して、$\mathfrak{F}$ が基底の場合に有効のままです。 (cf. I、p. 15、th. 2)。

#### 例 1 {#fvr-v-s3-n3-exa-1 .statement tag=08FE}

適用プロップ上。 V, p. 230 の 6 を関係 $1/x \ll x^{\alpha-1}$ にすると、$\alpha > 0$ は再び $\alpha > 0$ ごとに関係 $\log x \ll x^{\alpha}$ を取得します。これは、III で証明された関係 $y^{1/\alpha} \ll e^y$ に相当します。 p. 105。

#### 例 2 {#fvr-v-s3-n3-exa-2 .statement tag=08FF}

$\left( \frac{e^t}{x} \right)' = \frac{e^t}{x} \left( 1 - \frac{1}{x} \right) \sim e^t / x$ があります。 $e^t / x$ は $x$ では $+\infty$ になる傾向があるため、prop から推測できます。 V、p. 230、その$\int_{1}^{x} \frac{e^t}{t} \, dt \sim e^x / x$の6。

#### 注意 {#fvr-v-s3-n3-rem-1 .statement tag=08FG}

$g$ が区間 $[a, +\infty[$ で $\geq 0$ に留まるとは想定されておらず (または、区間で $\leq 0$ に留まる)、$\int_{a}^{+\infty} g(t) \, dt$ が収束しない場合、次のように、関係 $f \sim g$ は必ずしも $\int_{a}^{x} f(t) \, dt \sim \int_{a}^{x} g(t) \, dt$ を意味するわけではありません。 例ここで、$g(x) = \sin x$ と $f(x) = \left( 1 + \frac{\sin x}{x} \right) \sin x$;ここ

$$
\int_{n\pi}^{(n+1)\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{(n+1)\pi} \int_{0}^{\pi} \sin^2 t \, dt \geq \frac{1}{2} \int_{n+1}^{n+2} \frac{dt}{t},
$$

よって
$$
\int_{\pi}^{n\pi} \frac{\sin^2 t}{t} \, dt \geq \frac{1}{2} \int_2^{n+1} \frac{dt}{t}
$$
整 $\int_1^{+\infty} dt/t$ は無限で、けれども $\int_{\frac{\pi}{2}}^x g(t) \, dt = -\cos x$ は有界のままです (V、p. 260、演習 4 を参照)。

### 4. 比較の微分関係

命題 1 (V, p. 228) と 6 (V, p. 230) には逆: の近傍で微分可能な 2 つの写像間の比較関係 $f \preccurlyeq g,\ f \ll g,\ f \sim cg$ が存在します。 $+\infty$ は、実際の単調写像 $f$ と $g$ であっても、導関数間の同じ比較関係を意味しません。

たとえば、写像 $x^2 + x \sin x + \cos x$ は単調で $x^2$ と同等ですが、その導関数 $x(2 + \cos x)$ は $2x$ と同等ではありません。

一方、考慮されている写像の導関数が比較可能であるとアプリオリに仮定すると、比較関係を導き出すことができます (V、p. 217)。一般に、区間 $[a, +\infty[$ で定義された 2 つの実数写像 $f$ と $g$ は、$+\infty$ の近傍でそれぞれが一致する場合、$+\infty$ の近傍の位数 $k$ に匹敵すると言えます。 点の可算集合を除いて規制された $k^{th}$ 導関数があり、この近傍上で、$f^{(k)}$ と $g^{(k)}$ が定数符号 (それらが定義されている集合上で) を持ち、比較できる場合。

私たちは、2 つの比較可能な実質写像 (V、p. 217) は位数 0 に匹敵すると言うことに同意します。

#### 命題 7 {#fvr-v-s3-prop-7 .statement tag=08FH}

2 つの実数写像 $f,\ g$ が位数 1 に匹敵する場合、それらは匹敵します。さらに、関係 $f \ll g$ (それぞれ $f \sim cg$、$c$ 定数) は、$f' \ll g'$ (それぞれ $f' \sim cg'$) 〜でない限り $g$ が非零定数と同等であることを意味します。

さて、$f'$ と $g'$ は区間 $[x_0, +\infty[$ で定数符号であるため、$f$ と $g$ は両方ともこの区間では単調であるため、$x$ が $+\infty$ になる傾向があるように、有限または無限の極限になる傾向があります。これら極限の一方が有限で $\neq 0$ である場合、または一方が零でもう一方が無限である場合、$x$ は $+\infty$ になる傾向があるため、$f$ と $g$ が比較できることは明らかです。 $f$ と $g$ の両方が 0 になる傾向がある場合は、$f(x) = -\int_x^{+\infty} f'(t) \, dt,\ g(x) = -\int_x^{+\infty} g'(t) \, dt$ と書くことができます。 $f'$ と $g'$ は比較可能なため、$f$ と $g$ にも同じことが当てはまり、$f$ と $g$ の間の比較関係は、プロパティによる $f'$ と $g'$ の間の比較と同じです。 6 (V、p. 20)。同様に、$f$ と $g$ が両方とも無限の極限を持つ場合、一方は $f(x) = f(x_0) + \int_{x_0}^x f'(t) \, dt,\ g(x) = g(x_0) + \int_{x_0}^x g'(t) \, dt$ になります。またプロップ。 6 (V、p. 230) は、$f$ と $g$ が比較可能であり、$f$ と $g$ の比較関係が $f'$ と $g'$ の比較と同じであることを示しています。 証明を完成するには、$g$ が $\pm \infty$ と $f$ が定数になる傾向にある場合を考慮する必要があります。つまり、1 つのできないが $f' \succcurlyeq g'$ になるため、prop から推測できます。 1 (V, p. 218) 整$\int_{x_0}^{+\infty} g'(t) \, dt$ が収束したこと。 $f'$ と $g'$ は同等であると想定されているため、$f' \ll g'$ が必要です。

#### 系 {#fvr-v-s3-n4-cor-1 .statement tag=08FI}

*2 つの実数写像 $f, g$ が位数 $k \geqslant 1$ に匹敵する場合、それらは $0 \leqslant p \leqslant k$ の位数 $p$ に匹敵します。さらに、関係 $f \ll g$ (それぞれ $f \sim cg$) は、$f^{(k)} \ll g^{(k)}$ (それぞれ $f^{(k)} \sim cg^{(k)}$) 〜でない限り導関数 $g^{(p)}$ ($0 \leqslant p \leqslant k - 1$) の 1 つが定数 $\neq 0$ と同等であることを意味します。

確かに、$f^{(k)}$ と $g^{(k)}$ は区間 $[x_0, +\infty[$ で定数符号を持つため、$f^{(k-1)}$ と $g^{(k-1)}$ はこの区間で単調であるため、$+\infty$ の近傍で定数符号を持つことになります。さらに、プロップ。 V、p. 232 の 7 は、$f^{(k-1)}$ と $g^{(k-1)}$ が同等であることを示しているため、系は適用プロパティから続きます。 7 を再帰的に実行します。

#### 注意 1 {#fvr-v-s3-n4-rem-1 .statement tag=08FJ}

プロップで$g$の制限。 7は必須です。たとえば、$\frac{1}{x} \ll 1 + \frac{1}{x}$ さえけれどもであり、両辺の導関数は等価です。同様に$1 + \frac{1}{x} \sim 1 + \frac{1}{x^2}$ですが、$1/x^2 \gg 2/x^3$です。

#### 注意 2 {#fvr-v-s3-n4-rem-2 .statement tag=08FK}

けれども $f$ と $g$ は位数 $k$ 写像 $f_1$ $f$ は位数 $k$ から $g$ と比較できる必要はありません。しかし、$f_1$ が位数 $k$ から $f$ に匹敵し、微分$f^{(p)}$ ($0 \leqslant p \leqslant k - 1$) が非零定数と等価ではないと仮定すると、そうなります。

#### 注意 3 {#fvr-v-s3-n4-rem-3 .statement tag=08FL}

$f$ と $g$ が位数 $k$ に匹敵する場合、モノトーンの写像 $h$ であっても、$hf$ と $hg$ が$h(x) = x$ (V, p. 260、練習問題 3)。同様に、$1/f$ と $1/g$ は、必ずしも位数 $k$ (V、p. 259、演習 1) と比較できるわけではありません。

### 5. プリミティブのプリンシパル部分

$f$ を、区間 $[a, +\infty[$ に定数符号を持つ規制された実数写像 $\neq 0$ とします。次の命題により、特定の場合に $\int_a^{+\infty} f(t)\,dt$ が収束する場合はプリミティブ $\int_a^{+\infty} f(t)\,dt$ の主成分部分を、また、$\int_a^{+\infty} f(t)\,dt$ が無限である場合はプリミティブ $\int_a^x f(t)\,dt$ の主成分部分を取得できます。

#### 命題 8 {#fvr-v-s3-prop-8 .statement tag=08FM}

*Put* $F(x) = \int_x^{+\infty} f(t)\,dt$ *if* $\int_a^{+\infty} f(t)\,dt$ *収束*、*および* $F(x) = \int_a^x f(t)\,dt$ *if* $\int_a^{+\infty} f(t)\,dt$ *が無限*。 ** $\log|f|$ * と* $\log x$ * が位数* 1 に匹敵すると仮定します。

1 *もし* $f$ *が有限である位数* $\mu \neq -1$ *に関して* $x$ *あるものがある*
$$
F(x) \sim \frac{1}{|\mu+1|} x f(x).
$$
(1)

2 *もし* $f$ *が* $x$に対して無限大の位数である場合*、そしてもし* $f/f'$ *および* $x$ *が位数* 1に匹敵すると、*そして*
$$
F(x) \sim \frac{(f(x))^2}{|f'(x)|}.
$$
(2)

仮定は、$f(x)$ が $x$ (V、p. 219) に対して決定的な位数を持つことを意味していることに注意する必要があります。

1 *場合* $f$ *が位数* $\mu \neq 0$ *相対* $x$ *1 が* $\log|f| \sim \mu \log x$ であるため、*従って* $\log|f|$ *および* $\log x$ *は位数* 1と比較でき、*プロパティにより。 V、p. 232 の 7 つには * $f'/f \sim$ μ/x、よって $x f' \sim \mu f$ があります。 $\mu > -1$ の場合、$\varepsilon > 0$ ごとに $f(x) \gg x^{\mu-\varepsilon}$ があり、従って (V, p. 229, 定理 2) 整 $\int_a^{+\infty} f(t)\,dt$ は無限大です。 One can write $F(x) = \int_a^x f(t)\,dt = x f(x) - af(a) - \int_a^x t f'(t)\,dt$, よって again
$$
\int_a^x (f(t) + t f'(t))\,dt = x f(x) - af(a);
$$
$\mu \neq -1$ なので、$f(x) + x f'(x) \sim (\mu + 1) f(x)$ があるので、(V、p. 230、提案 6)
$$
\int_a^x (f(t) + t f'(t))\,dt \sim (\mu + 1) F(x),
$$
which proves (1) in this case. $\mu = 0$ の場合、同様に $x f'(x) \ll f(x)$ があり、再び $f(x) + x f'(x) \sim f(x)$ が得られます。 $\int_a^{+\infty} f(t)\,dt$ が収束する場合、$\mu < -1$ の場合も同様に議論できます。

2) $f$ が $x$ に対して位数 $+\infty$ である場合、$\log |f| \gg \log x$ があるため、(V, p. 232, prop. 7) $f'/f \gg 1/x$、またはもう一度$g(x) = f(x)/f'(x)$, $g(x) \ll x$ を代入します。さらに、$\alpha > 0$ごとに$f(x) \gg x^\alpha$なので、整$\int_a^{+\infty} f(t)\,dt$は無限大です。書くことができる
$$
F(x) = \int_a^x f(t)\,dt = \int_a^x g(t) f'(t)\,dt = g(x) f(x) - g(a) f(a) - \int_a^x f(t) g'(t)\,dt;
$$
$g$ と $x$ は位数 1 に相当するため、関係 $g(x) \ll x$ から、$g'(x) \ll 1$、従って $f g' \ll f$ であると推測できます (V、p. 232、提案 7)。 (V, p. 230, prop.6)
$$
\int_a^x f(t) g'(t)\,dt \ll F(x),
$$
which establishes 関係 (2). $\int_a^{+\infty} f(t)\,dt$が収束する場合、$x$に対して$f$が位数$-\infty$の場合、証明は類似します。

Let $\mathscr{E}$ be a comparison scale (for real $x$ tending to $+\infty$) formed of 非零 real 写像 that are of constant sign on 近傍 of $+\infty$, such that $x \in \mathscr{E}$ and such that 積 and 商 of two $\mathscr{E}$の写像は再び属するから$\mathscr{E}$ (V、p. 221、p. 224)。 If a regulated 写像 $f$ with constant sign on 近傍 of $+\infty$ has a principal 部分 $c g$ relative to $\mathscr{E}$, then $\int_x^{+\infty} f(t)\,dt$ (resp. $\int_a^x f(t)\,dt$ according to the case) will be equivalent to $c \int_x^{+\infty} g(t)\,dt$ (それぞれ $c \int_a^x g(t)\,dt$); 写像 $g$ が prop の仮説を満たしている場合。 8 of V, p. 233, and if (when 公式 (2) of V, p. 233, applies) one knows a principal 部分 of $g'$ relative to $\mathscr{E}$, one will thus have a principal 部分 of $\mathscr{E}$ に対する $\int_x^{+\infty} f(t)\,dt$ (それぞれ $\int_a^x f(t)\,dt$)。

#### 例 1 {#fvr-v-s3-n5-exa-1 .statement tag=08FN}

写像 $1/\log x$ は、$x$ に対して位数 0 であり、prop の条件を満たします。 V、p. 233の8;したがって
$$
\int_a^x \frac{dt}{\log t} \sim \frac{x}{\log x}.
$$

#### 例 2 {#fvr-v-s3-n5-exa-2 .statement tag=08FO}

写像 $e^{t^2}$ は、$x$ に対して位数 $+\infty$ であり、prop の条件を満たします。 8、それで
$$
\int_a^x e^{t^2}\,dt \sim \frac{1}{2x}\,e^{x^2}.
$$

付録 (V, p. 252) では、どのプロップに対して写像の定義する集合を実行します。 7とプロップ。 8 は常に適用されます。

#### 注意 {#fvr-v-s3-n5-rem-1 .statement tag=08FP}

提案 8 は、$x$ に対する位数 $-1$ の写像 $f$ には直接適用されません。しかし、その場合、$x$ に対して位数 0 の $f_1$ を使用して、$f(x) = f_1(x)/x$ と書くことができます。たとえば、$\int_a^{+\infty} f(t)\,dt$ が無限であると仮定します。それから

$$
F(x) = \int_a^x f(t)\,dt = \int_a^x \frac{1}{t} f_1(t)\,dt = \int_{\log a}^{\log x} f_1(e^u)\,du.
$$

写像 $f_1(e^t)$ が prop の仮説を満たす場合。 8 and has 位数 $\neq -1$ relative to $y$ (that is, if $f_1(x)$ has 位数 $\neq -1$ relative to $\log x$) the formulae (1) and (2) again allow us to obtain a principal 部分 for $F(x)$。たとえば、$f(x) = \frac{\exp(\sqrt{\log x})}{x \log x}$; とします。 $\exp(\sqrt{\log x})$ は $x$ に対して位数 0 であるため、$f$ は位数 $-1$ です。ここでは $f_1(e^t) = e^{\sqrt{t}}/y$ があり、この写像は $y$ に対して位数 $+\infty$ です。小道具。 8 を適用すると、$\int_a^x e^{\sqrt{u}}/u\,du \sim 2e^{\sqrt{y}}/\sqrt{y}$ が得られます。変数 $x$ に戻ると、$\int_a^x \frac{\exp(\sqrt{\log t})}{t \log t}\,dt \sim \frac{2\exp(\sqrt{\log x})}{\sqrt{\log x}}$ になります。

### 6. プリミティブの漸近展開

$\mathscr{E}$ を、$+\infty$ の近傍上の定数記号の実数写像 $\neq 0$ で形成された $+\infty$ の近傍上の比較スケールとします。 $\mathbf{f}$ を、区間 $[a,\,+\infty[$ で定義された規制されたベクトル写像とし、値を完全な正規化空間 $E$ に置き、漸近展開を認めます。

$$
\mathbf{f} = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda + \mathbf{r}_\alpha
$$

$\mathscr{E}$ を基準にして $g_\alpha$ の精度に。さらに、写像 $g \in \mathscr{E}$ のすべての原始関数 $\int_a^x g(t)\,dt$ が $\mathscr{E}$ に関して漸近展開できると仮定します。このような状況では、$\mathscr{E}$ に関して $F(x) = \int_a^x \mathbf{f}(t)\,dt$ の漸近展開が得られることがわかります。次の 2 つのケースを区別します。

1. $\int_a^{+\infty} g_\alpha(t)\,dt$ は無限です。その場合、1 つは $\int_a^x \mathbf{r}_\alpha(t)\,dt \ll \int_a^x g_\alpha(t)\,dt$ (V, p. 230, prop. 6) になります。 仮定までに、$\sum_{\lambda \leq \alpha} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt$ を一定の精度 $g_\rho$ (V, p. 222) まで漸近展開することができます。 $c g_\sigma$ が $\int_a^x g_\alpha(t)\,dt$ の主部分である場合、$\int_a^x \mathbf{f}(t)\,dt$ は精度 $g_{\min(\rho,\sigma)}$ に漸近展開され、すべての項は無限に増加するノルムを持ちます。

2. $\int_a^{+\infty} g_\alpha(t)\,dt$ が収束する。 $\beta$ を添字 $\lambda \leq \alpha$ の最小のとして、$\mathbf{a}_\lambda \neq 0$ が収束し、$\int_a^{+\infty} g_\lambda(t)\,dt$ が収束するようにします。整

$$
C = \int_a^{+\infty} \left( \mathbf{f}(t) - \sum_{\lambda < \beta} \mathbf{a}_\lambda g_\lambda(t) \right) dt
$$

は収束し、次のように書くことができます。

$$
F(x) = \sum_{\lambda < \beta} \mathbf{a}_\lambda \int_a^x g_\lambda(t)\,dt + C - \sum_{\beta \leq \lambda \leq \alpha} \mathbf{a}_\lambda \int_a^{+\infty} g_\lambda(t)\,dt - \int_a^{+\infty} \mathbf{r}_\alpha(t)\,dt.
$$

それから$\int_a^{+\infty} r_\alpha(t) \, dt \ll \int_1^{+\infty} g_\alpha(t) \, dt$; $c g_\sigma$ が $\int_1^{+\infty} g_\alpha(t) \, dt$ の主部分であり、 の漸近展開がある場合

$$
\sum_{\lambda < \beta} a_\lambda \int_a^\lambda g_\lambda(t) \, dt + C - \sum_{\beta \leq \lambda \leq \alpha} a_\lambda \int_\lambda^{+\infty} g_\lambda(t) \, dt
$$

精度 $g_\rho$ までは、結果として精度 $g_{\min(\rho, \sigma)}$ まで $F$ の漸近展開になります。

したがって、それはすべて、* $\mathscr{E}$ の * 写像の * プリミティブの $\mathscr{E}$ に関して漸近展開を見つけることになります。私たちは、$\mathscr{E}$ に関する特定の仮説を前提として、どのように有効かを見てきました。 V、p. 233 の 8 は、そのようなプリミティブの主成分部分を与えます。さらにプロップの証明。 8 は、写像 $\frac{1}{|\mu + 1|} (x f'(x) + f(x)) - f(x)$ (それぞれ $f(x) g'(x)$ と $g = f/f'$) のプリミティブの形における V、p. 233 の公式 (1) (それぞれ (2)) の式を示します。この新しいプリミティブの主部分を (1) の右側 (それぞれ (2)) の漸近展開として形成すると、求められた展開の右側が得られます (V、p. 247-255 を参照)。

#### 例 1 {#fvr-v-s3-n6-exa-1 .statement tag=08FQ}

$f(x) = 1/\log x$ ($x > 1$) にしましょう。 $\int_a^\lambda dt / \log t \sim x / \log x$ とその差 $\int_a^\lambda \frac{dt}{\log t} - \frac{\lambda}{\log \lambda}$ が $1/(\log x)^2$ のプリミティブであることがわかりました。プロップを適用できます。この写像に再び8を加えて、$\int_a^\lambda dt / (\log t)^2 \sim x / (\log x)^2$を取得します。再帰により、このように展開が得られます。

$$
\int_a^\lambda \frac{dt}{\log t} = \frac{x}{\log x} + \frac{x}{(\log x)^2}
+ \frac{2x}{(\log x)^3} + \cdots + (n-1)! \frac{x}{(\log x)^n} + o \left( \frac{x}{(\log x)^n} \right).
$$

$n$ に関係なく、この拡張のすべての項は $x$ で $+\infty$ になる傾向があることに注意してください。

#### 例 2 {#fvr-v-s3-n6-exa-2 .statement tag=08FR}

$f(x) = \frac{e^x}{x^2 + 1}$ にしましょう。 $f(x) = \frac{e^x}{x^2} - \frac{e^x}{x^4} + o_1 \left( \frac{e^x}{x^4} \right)$ と書くことができます。提案 8 は次の展開を与えます

$$
\int_a^\lambda \frac{e^t}{t^2} \, dt = \frac{e^x}{x^2} + \frac{2e^x}{x^3} + \frac{6e^x}{x^4} + o_2 \left( \frac{e^x}{x^4} \right), \quad \int_a^\lambda \frac{e^t}{t^4} \, dt = \frac{e^x}{x^4} + o_3 \left( \frac{e^x}{x^4} \right)
$$

よって、追加すると、

$$
\int_a^\lambda \frac{e^t}{t^2 + 1} \, dt = \frac{e^x}{x^2} + 2 \frac{e^x}{x^3} + 5 \frac{e^x}{x^4} + o_4 \left( \frac{e^x}{x^4} \right).
$$

### 練習問題 {#fvr-v-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
