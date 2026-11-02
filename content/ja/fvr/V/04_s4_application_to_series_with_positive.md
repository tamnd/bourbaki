---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 4
section_title: APPLICATION TO SERIES WITH POSITIVE TERMS
lang: ja
source: fvr-i-vii
book_pages: 236-246, 261-263
pdf_pages: 0251-0261, 0276-0278
extraction: ocr
subsections:
    - "no": 1
      title: CONVERGENCE CRITERIA FOR SERIES WITH POSITIVE TERMS
      page: 236
      pdf_page: 251
    - "no": 2
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL SUMS OF A SERIES
      page: 238
      pdf_page: 253
    - "no": 3
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL PRODUCTS OF AN INFINITE PRODUCT
      page: 243
      pdf_page: 258
    - "no": 4
      title: 'APPLICATION: CONVERGENCE CRITERIA OF THE SECOND KIND FOR SERIES WITH POSITIVE TERMS'
      page: 244
      pdf_page: 259
statements: 13
exercises: 11
content_sha256: 6b9a9cb255bea335749586c3b49fe42d452f68e9d90df70ff67d687d5b9caff8
translated_from: content/en/fvr/V/04_s4_application_to_series_with_positive.md
translation_method: google
source_content_sha256: c18bf105a0a19fb75952b1cd2547b25be59f3bbcc6840083c077e38c89496107
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 3591c9a01ba40daffc00c8d6d56c10e3ad8675554086e548f015f134c83fc5c9
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。 項が正の系列への申請

### 1. 系列と正の項の収束基準

この切断を *系列と正の項* で表すと、n の *$u_n \geq 0$ *ある特定のものから始まる* 値というように、実数項の系列 $(u_n)$ を (言葉の乱用によって) 理解することになります。このような系列についてこれから言うことはすべて、系列への符号の変更によって直ちに拡大するになります。そのすべての項は、n の特定の値から始まる $\leq 0$ です。 (II, p. 64, 例 3) は、ノルム空間 E における点のすべての数列 $(\mathbf{u}_n)_{n \geq 1}$ に、$[1, +\infty[$ で定義されたステップ写像 $\mathbf{u}$ を関連付けることができることを確認しました。 $n \leq x < n+1$ に対する条件 $\mathbf{u}(x) = \mathbf{u}_n$: 整 $\int_1^{+\infty} \mathbf{u}(t)\,dt$ が収束する場合に限り、系列 $(\mathbf{u}_n)$ は収束します。

$(u_n)$ と $(v_n)$ を、正の項を持つ 2 つの系列とし、$u$ と $v$ として、関連するステップ写像: 関係 $u_n \leq v_n$ $n \geq n_0$ は次と同等です。 $x \geq n_0$の$u(x) \leq v(x)$。したがって、関係 $u_n \preccurlyeq v_n, u_n \ll v_n, u_n \sim v_n$ はそれぞれ $u(x) \preccurlyeq v(x), u(x) \ll v(x)$ と $u(x) \sim v(x)$ に相当します。この注意により、命題 1 (V, p. 228) と 6 (V, p. 230) を次のように変換できます。

#### 命題 1 {#fvr-v-s4-prop-1 .statement tag=08FZ}

*$(u_n)$ *と* $(v_n)$ *2 系列と正の項とします。 * $u_n \preccurlyeq v_n$ *かつ系列* $(v_n)$ *が収束した場合* $(u_n)$ *は収束します。もし* $u_n \succ v_n$ *そしてもし* $\sum_{n=1}^{\infty} v_n = +\infty$なら、*その後* $\sum_{n=1}^{\infty} u_n = +\infty$。

#### 命題 2 {#fvr-v-s4-prop-2 .statement tag=08G0}

*$(u_n)$ *と* $(v_n)$ *2 系列と正の項* とします:
1. *系列* $(v_n)$ *が収束すると、関係* $u_n \ll v_n$ *(それぞれ* $u_n \sim v_n$) *暗黙* $\sum_{p=n}^{\infty} u_p \ll \sum_{p=n}^{\infty} v_p$ *(それぞれ* $\sum_{p=n}^{\infty} u_p \sim \sum_{p=n}^{\infty} v_p$)。
2. *もし* $\sum_{n=1}^{\infty} v_n = +\infty$ *その後、関係* $u_n \ll v_n$ *(それぞれ* $u_n \sim v_n$) *暗黙的に* $\sum_{p=1}^{n} u_p \ll \sum_{p=1}^{n} v_p$ *(それぞれ* $\sum_{p=1}^{n} u_p \sim \sum_{p=1}^{n} v_p$)。

prop で系列 $(v_n)$ を比較することにより、便利な収束基準が得られます。 1 系列の項は形 $v_n = f(n)$ であり、$f$ は実数 $x > x_0$ および減少するごとに定義された写像 $\geq 0$ です。 区間 $[x_0, +\infty[$;確かに：

#### 命題 3 (コーシー-マクローリン基準) {#fvr-v-s4-prop-3 .statement tag=08G1}

*もし* $f$ *が写像* $\geq 0$ *かつ減少するが $[x_0, +\infty[$ である場合、 *一般的な項* $v_n = f(n)$ を使用した系列 *整* $\int_{x_0}^{+\infty} f(t)\,dt$ の場合にのみ収束します。 *収束*。

これを証明するには、$v$ が系列 $(v_n)$ に関連付けられたステップ写像である場合、$f$ は減少するであるため、$x \geq x_0$ ごとに $v(x+1) \leq f(x) \leq v(x)$ になることに注意するだけで十分です。したがって、命題は比較原理の帰結です (II、p. 66、提案 3)。

積分の対数収束基準 (V、p. 229、prop. 2、3、および 4) の特徴である写像は、区間 $[x_0, +\infty[$、適用の減少するであるため、 V、p. 237 の 1 と 3 は、次の基準を示します。

#### 命題 4 (「位数 0 の対数基準」) {#fvr-v-s4-prop-4 .statement tag=08G2}

$(u_n)$ を系列とし、正の項をとります。ある $\mu < -1$ に対して $u_n \preccurlyeq n^\mu$ の場合、 系列 $(u_n)$ は収束します。ある $\mu \geq -1$ に対して $u_n \succcurlyeq n^\mu$ がある場合、系列 $(u_n)$ は無限の和になります。

#### 命題 5 (「位数 $p$ の対数基準」) {#fvr-v-s4-prop-5 .statement tag=08G3}

$(u_n)$ を系列とし、項を正とします。ある $\mu > 1$ に対して $u_n \preccurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ の場合、 系列 $(u_n)$ は収束します。ある $\mu \leq 1$ に対して $u_n \succcurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ がある場合、系列 $(u_n)$ は無限の和になります。

$0 \leq q < 1$ の場合、いずれかの $\mu > 0$ に対して $q^n \preccurlyeq n^{-\mu}$ があります。 適用位数 0 の対数基準は、$|q| < 1$ に対する幾何学的系列 $\sum_{n=0}^\infty q^n$ の収束を再度証明します (Gen. トップ。、IV、p. 364）。 If one applies prop. 1 with $v_n = q^n$ one obtains a criterion which may be put in the following form ("Cauchy's criterion"): *Let $(u_n)$ be a series with positive terms; if $\limsup_{n \to \infty}(u_n)^{1/n} < 1$ then the series $(u_n)$ converges; if $\limsup_{n \to \infty}(u_n)^{1/n} > 1$ then the series $(u_n)$ has infinite sum.* Indeed, if $\limsup_{n \to \infty}(u_n)^{1/n} = a < 1$ then $u_n \preccurlyeq q^n$ for every $q$ such that $a < q < 1$. 一方、$\limsup_{n \to \infty}(u_n)^{1/n} = a > 1$ の場合は、$n$ の無限多くの値に対して、$1 < q < a$ のような任意の $q$ に対して $u_n \succcurlyeq q^n > 1$ になります。 $u_n$ は 0 になる傾向がないので、$\sum_{n=1}^\infty u_n = +\infty$ になります。

この基準は、*全体系列* の理論で非常に役立ちます。これについては後で検討します。しかし、それでも、系列 $(1/n^\alpha)$ の収束を決定することはできず、他の語では、その体の適用は対数基準の適用よりもはるかに制限されています。

### 2. 系列の部分和の漸近展開

$x$ の実際の傾向が $+\infty$ である場合、$\mathscr{E}$ を写像によって形成される比較スケールとし、それぞれの区間* $[x_0, +\infty[$ (写像に応じて) で定義され、この区間では $\geq 0$ になります。 $(\mathbf{u}_n)$ を系列とし、その項属するを完全正規化空間 $\mathbf{E}$ にすると、$\mathbf{u}_n$ は、制限のスケール $\mathscr{E}'$ に関して精度 $g_\alpha$ への漸近展開が認められます。 $\mathscr{E}$の写像中$\mathbf{N}$:

$$
\mathbf{u}_n = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda(n) + \mathbf{r}_\alpha(n).
$$

すべての部分和 $\sum_{m=1}^n g(m)$ ($g \in \mathscr{E}$) が $\mathscr{E}'$ に対して漸近展開できるとします。次に、$\mathscr{E}'$ に関して$s_n = \sum_{m=1}^n \mathbf{u}_m$ の漸近展開を得ることができます。ここでも 2 つのケースを区別します。

1° $\sum_{n=1}^{\infty} g_{\alpha}(n) = +\infty$。すると (V, p. 237, 提案 2) $\sum_{m=1}^{n} r_{\alpha}(m) \ll \sum_{m=1}^{n} g_{\alpha}(m)$ が得られます。
仮定までに、次の漸近展開を得ることができます。
$$
\sum_{\lambda \leq \alpha} a_{\lambda} \left( \sum_{m=1}^{n} g(m) \right)
$$
(V, p. 222) 特定の精度 $g_{\sigma}$; $c g_{\sigma}(n)$ が $\sum_{m=1}^{n} g_{\alpha}(m)$ の主部分である場合、$s_{n}$ から精度 $g_{\min(\rho,\sigma)}$ まで漸近展開します。

2° $\sum_{n=1}^{\infty} g_{\alpha}(n)$ が収束します。次に、$\beta$ を $a_{\lambda} \neq 0$ となり、$\sum_{n=1}^{\infty} g_{\lambda}(n)$ が収束するように、添字 $\lambda \leq \alpha$ の最小のとします。 系列
$$
C = \sum_{n=1}^{\infty} \left( u_{n} - \sum_{\lambda < \beta} a_{\lambda} g_{\lambda}(n) \right)
$$
その後絶対収束し、次のように書くことができます。
$$
s_{n} = \sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right) - \sum_{m=n+1}^{\infty} r_{\alpha}(m).
$$
さらに、$\sum_{m=n+1}^{\infty} r_{\alpha}(m) \ll \sum_{m=n+1}^{\infty} g_{\alpha}(m)$; $c g_{\sigma}(n)$ が $\sum_{m=n+1}^{\infty} g_{\alpha}(m)$ のプリンシパル部分である場合、
そして、次の漸近展開がある場合、
$$
\sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right)
$$
従って、精度 $g_{\rho}$ までは、精度 $g_{\min(\rho,\sigma)}$ への $s_{n}$ の漸近展開が得られます。

従って、$g \in \mathscr{E}$ である系列 $(g(n))$ という特定のケースに導かれます。特定の条件を条件として、$s_{n} = \sum_{m=1}^{n} g(m)$ ($\sum_{n=1}^{\infty} g(n) = +\infty$ のとき) または $r_{n} = \sum_{m=n+1}^{\infty} g(m)$ ($\sum_{n=1}^{n} g(n) < +\infty$ のとき) の元本部分をすぐに取得できる方法を見ていきます。

#### 命題 6 {#fvr-v-s4-prop-6 .statement tag=08G4}

* g を、区間 [x_0, +\infty[ (x_0 \leq 1 ) で定義された実数写像, > 0 で単調な値とし、log g と x が位数 1 に匹敵するものとする。*

1° *g が e* に対して無限大位数である場合、次のようになります。

$$
s_n = \sum_{m=1}^n g(m) \sim g(n) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{1}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim g(n+1) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty. \tag{2}
$$

2° *g が有限の場合、$e^x$ に対して位数 $\mu$ となります*

$$
s_n = \sum_{m=1}^n g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_{\lambda_0}^n g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{3}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_n^\infty g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty \tag{4}
$$

($\mu = 0$の場合、数 $\frac{\mu}{1 - e^{-\mu}}$は(3)と(4)の1に置き換えられます。)

1° g が $e^x$ に対して位数 $+\infty$ である場合、仮定までに $\log g \gg x$ よって $g'/g \gg 1$ または $g' \gg g$ になります。従って、g は増加するとなり、$x$、よって $\sum_{n=1}^\infty g(n) = +\infty$ では $+\infty$ になる傾向があります。 $u$ が系列 $(g(n))$ (V、p. 237) に関連付けられたステップ写像である場合、$x$ の特定の値から始まる $u(x) \leq g(x)$ があるため、$u \ll g$ となり、結果として

$$
s_{n-1} = \int_1^n u(t) \, dt \ll \int_1^n g(t) \, dt \ll \int_1^n g'(t) \, dt \sim g(n);
$$

$s_n = s_{n-1} + g(n)$ 以降は $s_n \sim g(n)$ になります。 証明は、g が $e^x$ に対して位数 $-\infty$ である場合に類似します。従って、公式 (2) が得られます。

2° g が $e^x$ に対して有限の位数 $\mu$ である場合、$g(x) = e^{\mu x} h(x)$ と書くことができます。ここで、h は $e^x$ に対して位数 0 です。さらに、仮定により、$\mu \neq 0$ の $\log g \sim \mu x$ ($\mu = 0$ の$\log g \ll x$) は $h' \ll h$ を意味します。まず、$\sum_{n=1}^\infty g(n) = +\infty$ (これは、$\mu > 0$ の場合は常に $\mu \geq 0$; 逆が成り立ち、それ以降、$g(x)$ は $x$ では $+\infty$ になる傾向があることを意味します)。 $\int_{n-1}^n g(t) \, dt$ の元本部分を評価してみましょう。書くことができる

$$
\int_{n-1}^n g(t) \, dt = \int_{n-1}^n e^{\mu t} h(t) \, dt
$$
$$
= h(n) \int_{n-1}^n e^{\mu t} \, dt + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt
$$
$$
= \frac{1 - e^{-\mu}}{\mu} g(n) + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt.
$$

ここで、関係 $h' \ll h$ は、$\varepsilon > 0$ ごとに $n_0$ が存在することを意味し、関係 $x \geq n_0$ は $|h'(x)/h(x)| \leq \varepsilon$ を意味します。 $n \geq n_0$, よっての場合、平均値定理から、$n-1 \leq t \leq n$ に対して $-\varepsilon \leq \log |h(t)/h(n)| \leq \varepsilon$ が推定されます。

$$
|h(t) - h(n)| \leq (e^\varepsilon - 1)h(n)
$$

そしてその結果として

$$
\left| \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt \right| \leq (e^\varepsilon - 1)e^{\mu n}h(n) = (e^\varepsilon - 1)g(n)
$$

$e^{\mu t}$ は増加するなので。 $e^\varepsilon - 1$ は $\varepsilon$ で任意に小さくなるので、次のように書けることがわかります。

$$
\int_{n-1}^n g(t) \, dt = \frac{1 - e^{-\mu}}{\mu} g(n) + o(g(n))
$$

$\left( \frac{1 - e^{-\mu}}{\mu} \text{ being replaced by } 1 \text{ when } \mu = 0 \right)$。 命題はプロップの帰結になります。 V、p. 237の2つ。 $\sum_{n=1}^\infty g(n)$ が有限である場合も同様に議論できます。

適用プロップにより。 V、p. 239 の 6 を繰り返し、ときどきで $s_n = \sum_{m=1}^n g(m)$ の *漸近展開* を得ることができます。まず、$g$ が $e^\lambda$ に対して位数 $+\infty$ であると仮定します。 $p$ の *固定* 値ごとに、prop によって書き込むことができます。 6、

$$
s_n = g(n) + g(n-1) + \cdots + g(n-p) + o(g(n-p))
$$

そして、$s_n$ の拡張を取得するには、拡張の精度を $g(n-p)$ の主部分に制限しながら、写像 $g(n-k)$ ($0 \leq k \leq p$) をそれぞれ ($\mathscr{E}'$ に対して) 拡張するだけで十分です。

#### 例 {#fvr-v-s4-n2-exa-1 .statement tag=08G5}

位数 $+\infty$ を $e^\lambda$ に対して相対的に $g(x) = x^\lambda = \exp(\lambda \log x)$ とします。 $p = 2$ を取ると、

$$
(n-1)\log(n-1) = (n-1)\log n - 1 + \frac{1}{2n} + o\left( \frac{1}{n} \right)
$$

よって (V, p. 225)

$$
(n-1)^{n-1} = \frac{1}{e} n^{n-1} + \frac{1}{2e} n^{n-2} + o_1\left( n^{n-2} \right)
$$

そして同様に

$$
(n-2)^{n-2} = \frac{1}{e^2} n^{n-2} + o_2\left( n^{n-2} \right);
$$

従って

$$
s_n = n^n + \frac{1}{e} n^{n-1} + \left( \frac{1}{2e} + \frac{1}{e^2} \right) n^{n-2} + o_3\left( n^{n-2} \right).
$$

$g$ が $e^\lambda$ に対して位数 $-\infty$ である場合も、同様に進みます ($r_n$ の場合)。

ここで、$g$ が $e^x$ に対して有限の位数 $\mu$ であり、たとえば $\sum_{n=1}^\infty g(n) = +\infty$ の場合、次のように書くことができます。
$$
s_n = \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt + \sum_{m=1}^n f_1(m)
$$
ここで$f_1(n) = g(n) - \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt \ll g(n)$は小道具によるものです。 V、p. 239の6。 $\mathscr{E}'$ に対して$f_1(n)$ のプリンシパル部分 $c g_1(n)$ があり、再びプロップを適用できる場合。 6 から写像 $g_1$ まで、$\sum_{n=1}^\infty g_1(n) = +\infty$ の場合は $\sum_{m=1}^n f_1(m)$ と同等のプリミティブが得られ、その逆の場合は $\sum_{m=n+1}^\infty f_1(m)$ と同等のプリミティブが得られます (後者の場合、$C = \sum_{n=1}^\infty f_1(n)$ を使用して $\sum_{m=1}^n f_1(m) = C - \sum_{m=n+1}^\infty f_1(m)$ と書きます)。

したがって、ステップバイステップで、最終的には、それぞれが前のものに対して無視できるプリミティブの特定の数の和、最後に書き込まれたプリミティブと比較して無視できるままの項、そして最後に定数（残りの項が0になる傾向がある場合）として$s_n$の式を得ることができます。次に、得られた各プリミティブを $\mathscr{E}'$ (cf. V、p. 235) に関して拡張することが残ります。

#### 例 {#fvr-v-s4-n2-exa-2 .statement tag=08G6}

$g(n) = \frac{1}{n}$ にしましょう。それから
$$
s_n = \sum_{m=1}^n \frac{1}{m} \sim \int_1^n \frac{dt}{t} = \log n
$$
それから
$$
\frac{1}{n} - (\log n - \log(n-1)) \sim -\frac{1}{2n^2}
$$
よって
$$
s_n = \log n + \gamma + \frac{1}{2n} + o\left(\frac{1}{n}\right).
$$
この公式に登場する定数$\gamma$ は、分析において重要な役割を果たします (cf. 章、VI および VII)。それは *オイラー定数*として知られています。 1つは持っています
$$
\gamma = 0.577\,215\,664\ldots
$$
$1/10^9$以内に。

VI、p. 288 で、*オイラー・マクローリン和公式* が、最も重要な場合に、$s_n$ (または $r_n$) に対して *任意の* 位数の漸近展開を与える様子を見ていきます。

### 3. 無限積の部分積の漸近展開

一般因子 $1 + u_n$ ($u_n > -1$) を持つ無限積が収束する (可換収束する) ためには、一般項を持つ系列が必要かつ十分であることがわかっています (Gen. Top.、V. p. 22 および 23)。 $\log(1 + u_n)$ は収束する (可換収束する) 必要があり、その場合、関係が得られます。

$$
\log \prod_{n=1}^{\infty} (1 + u_n) = \sum_{n=1}^{\infty} \log(1 + u_n).
$$

無限の積が収束すると、$u_n$ が 0 になる傾向があることがわかります。したがって、$\log(1 + u_n) \sim u_n$;今では、実数の系列が可換収束するには、それが絶対的に収束することが必要かつ十分であることがわかります (Gen. Top.、IV、p. 372、提案 5)。プロップによって。したがって、積と一般因子 $1 + u_n$ は、系列と一般項 $u_n$ が完全に収束する場合に限り、可換収束するという事実がわかります (Gen. Top.、IV、p. 368、th. 4)。

同様の議論が、一般因子が複素数 $1 + u_n$ ($u_n \neq -1$) である無限積にも当てはまります。 実際、そのような積が可換的に収束するためには、それが必要かつ十分です (創世記 2:00)。 トップ、VIII、p. 115、プロップ。 2) 一般的な因子 $|1 + u_n|$ を伴う無限積はそうなるはずであり、さらに、$\theta_n$ が $1 + u_n$ ($-\pi$ と $+\pi$ の間で取られる) である場合、$\theta_n$ の系列は可換収束するはずです。 $u_n$ は 0 になる傾向があるため、$\log(1 + u_n)$ は $n$ (III、p. 100) の特定の値から開始して定義されます。

$$
\log(1 + u_n) = \log |1 + u_n| + i \theta_n;
$$

したがって、積と一般因子 $1 + u_n$ が可換収束するには、系列と一般項 $|\log(1 + u_n)|$ が絶対収束することが必要かつ十分です (Gen Top.、VII、p. 84、th. 1)。現在$\log(1 + u_n) \sim u_n$ (I, p. 18, prop. 5) なので、系列と一般項 $u_n$ は絶対に収束するはずであるという条件が得られます (Gen. Top., VIII, p. 116, th. 1)。

実数ときどきの無限積と系列の間の関係により、部分積 $p_n = \prod_{k=1}^{n} (1 + u_k)$ の漸近展開を得ることができます。部分和 $s_n = \sum_{k=1}^{n} \log(1 + u_k)$ を漸近展開してから、 $p_n = \exp(s_n)$ を展開するだけで十分です。したがって、1 つは、以前に調べた 2 つの問題 (V、p. 238、および p. 226) に戻されます。

#### 例 {#fvr-v-s4-n3-exa-1 .statement tag=08G7}

*スターリングの公式.* $n!$ の漸近展開を求めてみましょう。これにより、$s_n = \sum_{p=1}^{n} \log p$、次に $\exp(s_n)$ が展開されます。 n 2 の方法は連続的に与えます

$$
s_n = \sum_{p=1}^{n} \log p \sim \int_{1}^{n} \log t \, dt = n \log n - n + 1
$$

それから
$$
\log n - \int_{n-1}^{n} \log t \, dt = \log n - (n \log n - (n-1) \log(n-1) - 1) \sim \frac{1}{2n}
$$
よって
$$
s_n = n \log n - n + \frac{1}{2} \log n + o(\log n).
$$
それから
$$
\log n - \int_{n-1}^{n} \log t \, dt - \frac{1}{2} (\log n - \log(n-1)) \sim -\frac{1}{12n^2}
$$
よって
$$
s_n = n \log n - n + \frac{1}{2} \log n + k + \frac{1}{12n} + o_1 \left( \frac{1}{n} \right) \quad (k \text{ constant})
$$
そして最後に推測する (V, p. 226)
$$
n! = e^k \, n^{n+1/2} \, e^{-n} \left( 1 + \frac{1}{12n} + o_2 \left( \frac{1}{n} \right) \right). \tag{5}
$$
VII、p. 322、その$e^k = \sqrt{2\pi}$で示します。 公式 (5) (これと $k$ の値) は *スターリングの公式* と呼ばれます。同様に、整数 $> 0$ ではなく、すべての実数 $a$ について、次のことがわかります。
$$
(a+1)(a+2)\ldots(a+n) \sim K(a) \, n^{n+a+\frac{1}{2}} \, e^{-n}. \tag{6}
$$
私たちも決定する写像 $K(a)$ になります (VII、p. 18)。式 (5) と (6) から、特に次のことが導き出されます。
$$
\binom{a}{n} \sim (-1)^n \varphi(a) \, n^{-a-1} \tag{7}
$$
整数 $> 0$ ではなく、実数 $a$ ごとに、$\varphi(a)$ は VII、p. 322 で指定される $a$ の写像です。

### 4. 適用: 系列と正の項の第 2 種収束基準

ある点から $u_n > 0$ が系列 $(u_n)$ になることがよくあり、$u_{n+1}/u_n$ は決定するになりやすい漸近展開を持っています。このような系列にとって、系列が$u_{n+1}/u_n$の形のみから収束するかどうかを決定する可能にする基準（*第2種基準*と呼ばれる）を持つと便利です。そのような基準としては次のようなものがあります。

#### 命題 7 (「ラーベのテスト」) {#fvr-v-s4-prop-7 .statement tag=08G8}

※$(u_n)$を系列とし、点以降は項$> 0$とします。ある段階から、一部の $\alpha > 1$ に対して $u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$ があった場合、系列 $(u_n)$ は収束します。ある点から $u_{n+1}/u_n \geqslant 1 - \frac{1}{n}$ であれば、系列 $(u_n)$ は無限の和になります。*

実際、$u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$ と $\alpha > 1$ の場合、すべての $n \geqslant n_0$ に対して、1 つは $u_n \preccurlyeq p_n = \prod_{k=n_0}^{n} \left( 1 - \frac{\alpha}{k} \right)$ になります。さて、$\log \left( 1 - \frac{\alpha}{n} \right) = -\frac{\alpha}{n} - \frac{\alpha^2}{2n^2} + o \left( \frac{1}{n^2} \right)$、よって $\log p_n =$ $-\alpha \log n + k + o(1/n)$ ($k$ 定数)、および $p_n \sim e^k \frac{1}{n^\alpha}$; $\alpha > 1$ からは、対数基準位数 0 により終了できます。

一方、ある点から$u_{n+1}/u_n \geq 1 - \frac{1}{n}$であれば、同じ計算で$u_n \geq \frac{1}{n}$、よって命題であることがわかります。

証明できるも同様に、位数 $> 0$ の対数基準、次の第 2 種基準を使用します。

#### 命題 8 {#fvr-v-s4-prop-8 .statement tag=08G9}

※ある点から項$> 0$を$(u_n)$を系列とします。ある点から、* があるとします。

$$
\frac{u_{n+1}}{u_n} \leq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)} - \frac{\alpha}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*一部の $\alpha > 1$ では、系列 $(u_n)$ が収束します。 点以降、* があった場合

$$
\frac{u_{n+1}}{u_n} \geq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*その後、系列 $(u_n)$ は無限大の和になります。*

#### 例 {#fvr-v-s4-n4-exa-1 .statement tag=08GA}

一般的な項を使用した *超幾何系列* を考えてみましょう。

$$
u_n = \frac{\alpha(\alpha+1)\ldots(\alpha+n-1)\,\beta(\beta+1)\ldots(\beta+n-1)}{1.2\ldots n.\gamma(\gamma+1)\ldots(\gamma+n-1)}
$$

ここで、$\alpha, \beta, \gamma$ は任意の実数であり、整数 $\leq 0$ ではありません。$u_n$ は、ある段階では $> 0$ であるか、ある段階以降では $< 0$ であることは明らかです。 1つは持っています

$$
\begin{align*}
\frac{u_{n+1}}{u_n} &= \frac{(\alpha+n)(\beta+n)}{(n+1)(\gamma+n)} \\
&= \left(1 + \frac{\alpha+\beta}{n} + \frac{\alpha\beta}{n^2}\right) \left(1 + \frac{\gamma+1}{n} + \frac{\gamma}{n^2}\right)^{-1} \\
&= 1 + \frac{\alpha+\beta-\gamma-1}{n} \\
&\quad + \frac{\alpha\beta-(\alpha+\beta)(\gamma+1)+\gamma^2+\gamma+1}{n^2} + o\left(\frac{1}{n^2}\right).
\end{align*}
$$

ラーベのテストでは、系列は $\alpha + \beta < \gamma$ に収束し、$\alpha + \beta > \gamma$ には無限の和が存在することが示されています。 prop で示されているように、$\alpha + \beta = \gamma$ 系列も無限の和を持ちます。 8.

#### 注意 1 {#fvr-v-s4-n4-rem-1 .statement tag=08GB}

ラーベのテストの特定の例として、$\limsup_{n \to \infty} u_{n+1}/u_n < 1$ 系列 $(u_n)$ が収束することがわかります。一方、$\liminf_{n \to \infty} u_{n+1}/u_n > 1$, 系列 $(u_n)$ の場合、和は無限大になります (*ダランベールの検定*)。

#### 注意 2 {#fvr-v-s4-n4-rem-2 .statement tag=08GC}

第 2 種の基準は、$n$ が $+\infty$ になる傾向があるように、一般的な項が非常に規則的な方法で動作する系列にのみ適用できます。他の語では、その範囲は対数基準の範囲よりもはるかに制限されており、特に適した特殊なケースを超えてそれらを使用しようとするのは間違いです。たとえば、$u_{2m} = 2^{-m}$、$u_{2m+1} = 3^{-m}$ によって定義される系列 $(u_n)$ の場合、$u_{2m+1}/u_{2m} = \left(\frac{2}{3}\right)^m$、$u_{2m+2}/u_{2m+1} = \frac{1}{2} \left(\frac{3}{2}\right)^m$ があります。 $m$ が無限に増加するにつれて、これらの比率の最初の比率は 0 になり、2 番目の比率は $+\infty$ になる傾向があるため、2 番目の種類の基準は適用できません。それにもかかわらず、$u_n \preccurlyeq 2^{-n/2}$ 以降、系列が収束するのは明らかです。

$u_{n+1}/u_n$ が単純な式を持っている場合でも、$u_n$ のプリンシパル部分を直接評価すると、多くの場合、第 2 種の基準と同じくらい早く結果が得られます。たとえば、超幾何系列の場合、スターリングの公式は $u_n \sim a n^{\alpha + \beta - \gamma - 1}$ を示します。ここで、$a$ は定数 $\neq 0$ であり、対数基準位数 0 が適用されます。

### 練習問題 {#fvr-v-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
