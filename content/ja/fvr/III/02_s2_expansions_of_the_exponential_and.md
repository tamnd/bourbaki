---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 2
section_title: EXPANSIONS OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS AND OF THE FUNCTIONS ASSOCIATED WITH THEM
lang: ja
source: fvr-i-vii
book_pages: 105-113, 125-128
pdf_pages: 0120-0128, 0140-0143
extraction: ocr
subsections:
    - "no": 1
      title: EXPANSION OF THE REAL EXPONENTIAL
      page: 105
      pdf_page: 120
    - "no": 2
      title: EXPANSIONS OF THE COMPLEX EXPONENTIAL, OF $\cos x$ AND $\sin x$
      page: 106
      pdf_page: 121
    - "no": 3
      title: THE BINOMIAL EXPANSION
      page: 107
      pdf_page: 122
    - "no": 4
      title: EXPANSIONS OF log(1 + x), OF Arc tan x AND OF Arc sin x
      page: 111
      pdf_page: 126
statements: 1
exercises: 9
content_sha256: 726a9a929ec2efc264bf763ad673f7275daf8d00994ab338cab5e6ae096e522a
translated_from: content/en/fvr/III/02_s2_expansions_of_the_exponential_and.md
translation_method: google
source_content_sha256: 9b4d042c915247a66706e89ec93b075b9470428497af056aac806e76d9a56cf9
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 94e9b510281a092ae905f16642c481fe71043d0fcaeb0fe264ae8e14f0a7a5cb
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。指数関数と循環関数写像、およびそれらに関連する写像の拡張

### 1. 実指数関数の拡張

$\mathrm{D}^n \left( e^x \right) = e^x$ から、$e^x$ に対する位数 $n$ のテイラー展開は次のようになります。

$$
e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + \int_0^x \frac{(x-t)^n}{n!} e^t \, dt. \tag{1}
$$

この公式の余りは、$x > 0$の場合は$> 0$で、$x < 0$のときは$(-1)^{n+1}$の符号を持ちます。さらに、平均値の不等式は次のことを示しています。

$$
\frac{x^{n+1}}{(n+1)!} < \int_0^x \frac{(x-t)^n}{n!} e^t \, dt < \frac{x^{n+1} e^x}{(n+1)!} \qquad \text{for } x > 0 \tag{2}
$$

$$
\frac{\left| x^{n+1} \right| e^x}{(n+1)!} < \left| \int_0^x \frac{(x-t)^n}{n!} e^t \, dt \right| < \frac{\left| x^{n+1} \right|}{(n+1)!} \qquad \text{for } x < 0 \tag{3}
$$

これで、$n$ が無限に増加すると、すべての $x \geqslant 0$ (*Gen. Top.*、IV、p. 365) について、数列 $\left( x^n / n! \right)$ は極限 0 になることがわかります。したがって、(1) では $x$ を固定し、$n$ を無限に成長させると、(2) と (3) から次のようになります。

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} \tag{4}
$$

そして、右辺の系列は、$\mathbf{R}$ のすべてのコンパクト区間上で *絶対的かつ一様に収束* します。特に、1 つは公式

$$
e = 1 + \frac{1}{1!} + \frac{1}{2!} + \cdots + \frac{1}{n!} + \cdots \tag{5}
$$

これにより、公式により、数 $e$ に限りなく近い有理近似を計算する行うことができます。人は得る

$$
e = 2.718\,281\,828\ldots
$$

$1/10^9$以内まで。さらに、公式 (5) は、$e$ が *無理数* 数 $^{2}$ (*Gen. Top.*、IV、p. 375) であることを証明します。

#### 注意 {#fvr-iii-s2-n1-rem-1 .statement tag=08B3}

公式 (1) の余りは $x > 0$ に対して $> 0$ なので、 $x > 0$ に対して 1 が得られます。

$$
e^x > 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^{n+1}}{(n+1)!}
$$

そして*なおさら*

$$
e^x > \frac{x^{n+1}}{(n+1)!}
$$

すべての整数 $n$ について: このことから、$e^x / x^n$ は $x$ とともに $+\infty$ になる傾向があることが推測されます。すべての整数 $n$ について: この結果は 2 章で再び見つけることになります。 V by 他の方法 (V、p. 231)。

$^{2}$ CH. HERMITE は 1873 年に、$e$ が有理数数の体 $\mathbf{Q}$ を超える *超越論的* 数であることを証明しました (他の語では、有理数係数をもつ多項式の根ではありません)。 (*āuvres*、t. III, p. 150、パリ (ゴティエ ヴィラール)、1912 年)。

### 2. $\cos x$ と $\sin x$ の複素指数の展開

$z$ を任意の複素数とし、実変数 $t$ の写像 $\varphi(t) = e^{zt}$ を考慮します。 $D^n \varphi(t) = z^n e^{zt}$ と $e^z = \varphi(1)$ があります。 点 $t = 0$ (II, p. 62) について、位数 $n$ のテイラー 系列を使って $\varphi(1)$ を表現すると、次のようになります。

$$
e^z = 1 + \frac{z}{1!} + \frac{z^2}{2!} + \cdots + \frac{z^n}{n!} + z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

公式は、$z$ が実数の場合の (1) に相当します。残り

$$
r_n(z) = z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

この公式は、平均値の不等式を使用することで、絶対値値より上に制限することができます。 $z = x + i y$ の場合は $|e^{zt}| = e^{xt}$ なので、$x \leq 0$ の場合は $|e^{zt}| \leq 1$、$x > 0$ の場合は $|e^{zt}| \leq e^x$ になります。したがって

$$
|r_n(z)| \leq \frac{|z|^{n+1}}{(n+1)!} \text{ if } x \leq 0
$$
$$
|r_n(z)| \leq \frac{|z|^{n+1} e^x}{(n+1)!} \text{ if } x > 0.
$$

上記のように、私たちは結論する

$$
e^z = \sum_{n=0}^\infty \frac{z^n}{n!}
$$

系列は、$\mathbf{C}$ のすべてのコンパクト部分集合に *絶対的かつ一様に収束* します。

(6) から特に次のことが推測されます。

$$
e^{ix} = 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \cdots + \frac{i^n x^n}{n!} + i^{n+1} \int_0^x \frac{(x-t)^n}{n!} e^{it} \, dt
$$

そこから、$\cos x$ と $\sin x$ のテイラー展開を導き出します。 (10) の実数部分を位数 $2n+1$ にすると、次のようになります。

$$
\cos x = 1 - \frac{x^2}{2!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!} + (-1)^{n+1} \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

余りを境界とする

$$
\left| \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt \right| \leq \frac{|x|^{2n+2}}{(2n+2)!}.
$$

同様に、(10) の虚数部分を位数 $2n$ にすると、次のようになります。

$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!}
$$
$$
+ (-1)^n \int_0^1 \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt
$$

余りを境界とする

$$
\left| \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt \right| \leq \frac{|x|^{2n+1}}{(2n+1)!}.
$$

さらに、(11) の位数 $2n+1$ と $2n+3$ の余りを比較すると、次のようになります。

$$
\int_0^1 \frac{(x-t)^{2n+3}}{(2n+3)!} \cos t \, dt = \frac{x^{2n+2}}{(2n+2)!} - \int_0^1 \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

そして、(12) を考慮すると、(11) の剰余は、$x$ に関係なく、$(-1)^{n+1}$ と *同じ符号* を持つことがわかります。同様に、(13) の剰余が $(-1)^n x$ と *同じ符号* を持つことを示すことができます。特に、(11) の $n=0$ と $n=1$ 、および (13) の $n=1$ と $n=2$ については、次の不等式が得られます。

$$
1 - \frac{x^2}{2} \leq \cos x \leq 1 \quad \text{for all } x
$$
(15)

$$
x - \frac{x^3}{6} \leq \sin x \leq x \quad \text{for all } x \geq 0.
$$
(16)

最後に、(9) に $z = i x$ を入れると、次のようになります。

$$
\cos x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
$$
(17)

$$
\sin x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$
(18)

これら系列は、すべてのコンパクト区間に絶対的かつ均一に収束します。

さらに、式 (17) と (18) は、右辺のすべての*複素数* $x$、系列に対して有効であり、$\mathbf{C}$ のすべてのコンパクト部分集合に絶対的かつ一様に収束することは明らかです。特に、すべての $x$ (実数または複素数) について

$$
\cosh x = \sum_{n=0}^\infty \frac{x^{2n}}{(2n)!}
$$
$$
\sinh x = \sum_{n=0}^\infty \frac{x^{2n+1}}{(2n+1)!}.
$$

### 3. 二項展開

$m$ を *任意の* 実数とします。 $x > 0$ については、

$$
D^n (x^m) = m(m-1)\ldots(m-n+1) x^{m-n};
$$

写像 $(1 + x)^m$ に対する位数 $n$ の Taylor 公式は点 $x = 0$ について、$x > -1$ ごとにそれを示しています

$$
(1 + x)^m = 1 + \binom{m}{1} x + \binom{m}{2} x^2 + \cdots + \binom{m}{n} x^n + r_n(x)
$$

と

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt
$$

$\binom{m}{n} = \frac{m(m-1)\ldots(m-n+1)}{n!}$ を入れたところ。 $m$ が整数 $> 0$ および $n \geq m$ である場合、公式 (19) 簡約するを二項公式 (Alg.、I、p. 99) に変換します。 拡大では、これを *二項公式* と呼び、係数 $\binom{m}{n}$ は、$m$ が *任意* 実数で、$n$ が任意の場合、*二項係数* と呼ばれます。 整数 $> 0$。

(19) の剰余は、$x > 0$ の場合は $\binom{m}{n+1}$ と同じ符号を持ち、$-1 < x < 0$ の場合は $(-1)^{n+1} \binom{m}{n+1}$ と同じ符号を持ちます。エンドポイント 0 と $x$ を持つ区間の $t > -1$ に対する $\left| \frac{x-t}{1+t} \right| \leq |x|$ から、残り、$m$ と $n$ 任意、および $x > -1$ については次の境界が得られます。

$$
\left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} \, dt \right|
$$
$$
\leq \left| \binom{m-1}{n} x^n ((1+x)^m - 1) \right|.
$$

$x \geq 0$ と $n \geq m-1$ を仮定すると、積分の区間では $(1+t)^{n-m+1} \geq 1$ となるので、

$$
0 \leq \int_0^x \frac{(x-t)^n}{(1+t)^{n-m+1}} \, dt \leq \int_0^x (x-t)^n \, dt = \frac{x^{n+1}}{n+1}
$$

推定値が得られます

$$
|r_n(x)| \leq \left| \binom{m}{n+1} \right| x^{n+1} \quad (x \geq 0,\ n \geq m-1)
$$

残りについては。一方、$-1 \leq m < 0$; と仮定します。積分 (19) で変数 $u = \frac{x-t}{x(1+t)}$ を変更とすると、次のようになります。

$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} (1+x)^m x^{n+1} \int_0^1 \frac{u^n \, du}{(1+ux)^{m+1}}.
$$

$x > -1$ の積分を推定するには、$m + 1 < 1$ 以降、積分 $\int_0^1 \frac{u^n \, du}{(1-u)^{m+1}}$ が収束し、$1 + u x > 1 - u$ 以降 (22) の右辺を制限することに注意します。さて、$m$ 上の $-1 < x < 0$ 仮定は、(19) の右辺に現れるすべての項 $\binom{m}{1} x, \binom{m}{2} x^2, \ldots, \binom{m}{n} x^n$ が $\geq 0$ であることを意味し、従って $r_n(x) \leq (1 + x)^m$ を $(1 + x)^m$ で割ると、

$$
\frac{m(m-1) \ldots (m-n)}{n!} x^{n+1} \int_0^1 \frac{u^n \, du}{(1 + u x)^{m+1}} \leq 1.
$$

さらに、$-1 < x < 0$ 因子の積分の前は $\geq 0$ なので、$x$ を $-1$ に近づけると、

$$
\left| \frac{m(m-1) \ldots (m-n)}{n!} \int_0^1 \frac{u^n \, du}{(1-u)^{m+1}} \right| \leq 1
$$

その結果、$-1 \leq m < 0$ と $x > -1$ については次のようになります。

$$
|r_n(x)| \leq (1 + x)^m |x|^{n+1}.
$$ (23)

これらの不等式から、まず、$|x| < 1$ について次のことが推測できます。

$$
(1 + x)^m = \sum_{n=0}^\infty \binom{m}{n} x^n
$$ (24)

右側 (二項系列と呼ばれる) は、$]-1, +1[$ のすべてのコンパクト部分集合に絶対的かつ一様に収束します。確かに人は書くことができる

$$
\binom{m}{n} = (-1)^n \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n} \right)
$$ (25)

よって

$$
\left| \binom{m}{n} \right| \leq \left( 1 + \frac{|m+1|}{1} \right) \left( 1 + \frac{|m+1|}{2} \right) \ldots \left( 1 + \frac{|m+1|}{n} \right).
$$

$|x| \leq r < 1$ の場合、$1 + \frac{|m|}{n_0} < \frac{1}{r'}$ となる $n_0$ があり、ここで $r < r' < 1$ です。 よって、パッティング

$$
k = \left( 1 + \frac{|m|}{1} \right) \left( 1 + \frac{|m|}{2} \right) \ldots \left( 1 + \frac{|m|}{n_0} \right)
$$

私たちは持っています

$$
\left| \binom{m-1}{n} x^n \right| \leq k |x|^{n_0} \left( \frac{r}{r'} \right)^{n - n_0},
$$

これは命題を証明します。一方、$x > 1$ については、系列 (24) の一般的な項の絶対値は、$m$ が整数 $\geq 0$ でない場合、$n$ と無限に増加します。確かに、(25) から、$n > n_1 \geq |m+1|$ になります。

$$
\left| \binom{m}{n} \right| \geq \left| \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right|
$$
$$
\left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n} \right).
$$

$n_0 \geq n_1$ を、$n \geq n_0$ に対して $1 - \frac{|m+1|}{n} > \frac{1}{x'}$ が得られるようにします。ここで、$1 < x' < x$ です。入れたら
$$
k' = \left| \left( 1 - \frac{m+1}{1} \right) \ldots \left( 1 - \frac{m+1}{n_1} \right) \right| \left( 1 - \frac{|m+1|}{n_1+1} \right) \ldots \left( 1 - \frac{|m+1|}{n_0} \right)
$$
そうすると、$n > n_0$で、
$$
\left| \binom{m}{n} x^n \right| \geq k' |x|^{n_0} \left( \frac{x}{x'} \right)^{n-n_0}
$$
そこから命題が続きます。

$m = -1$ について、代数恒等式は
$$
\frac{1}{1+x} = 1 - x + x^2 - \cdots + (-1)^{n-1} x^{n-1} + (-1)^n \frac{x^n}{1+x}
$$
積分することなく、一般的な公式 (19) の剰余の式を与えます。 公式 (23) 簡約するこの場合、幾何学的な系列 (または進行) の和の式になります (Gen. Top., IV, p. 364)。

次に、$x = 1$ または $x = -1$ (自明なケース $m = 0$ を除く) の二項系列の収束を調べてみましょう。

$a) \ m \leq -1$。 積と一般項 $1 - \frac{m+1}{n}$ は、$m < -1$ であれば $+\infty$ に、$m = -1$ であれば 1 に収束するため、(25) から、$x = \pm 1$ については二項系列の一般項は 0 になる傾向がないことがわかります。

$b) \ -1 < m < 0$。今回の積と一般的な項 $1 - \frac{m+1}{n}$ は 0 に収束するため、不等式 (21) は $r_n(1)$ が 0 になる傾向があることを示しています。 したがって、二項系列は $x = 1$ について収束し、和 $2^m$ になります。さらに、二項式系列は、上で見たことと (21) のおかげで、すべての区間 $]x_0, 1]$ と $-1 < x_0 \leq 1$ で一様に収束します。一方、$x = -1$ の場合、(24) の右側のすべての項は $\geq 0$ であり、この系列が収束すると、二項系列は通常 $[-1, 1]$ に収束するため、その和についても連続となると推測できます。この区間では写像ですが、これは不合理です。なぜなら、$(1+x)^m$ は $m < 0$ に対して $[-1, 1]$ で制限されていないからです。 結論する $x = 1$ についても、二項系列は完全には収束しません。

$c) \ m > 0$。 $r_n(x)$ の定義は、$x$ が $-1$ になる傾向がある場合、$r_n(x)$ は極限 $r_n(-1)$ になる傾向があることを示しています。 (20) の移行から極限に対して 1 つの結論すると $|r_n(-1)| \leq \left| \binom{m-1}{n} \right|$ があり、$m-1 > -1$ 以降、$x = -1$ については二項系列が収束していることがわかります。さらに、$n > m+1$ については、この系列のすべての項は同じ符号を持ちます。したがって、二項式系列は通常区間 [−1, 1] に収束し、この区間上で和 (1 + x)^m を持ちます。

### 4. log(1 + x)、Arc Tan x、および Arc sin x の展開

(26) の 2 つの辺を 0 と x の間で積分しましょう。 log(1 + x) の位数 n のテイラー展開を取得します (x > −1 の場合に有効)

$$
\log(1 + x) = \frac{x}{1} - \frac{x^2}{2} + \frac{x^3}{3} + \cdots + (-1)^n \frac{x^n}{n} + (-1)^n \int_0^x \frac{t^n \, dt}{1 + t}.
$$ (27)

x > 0 の場合、剰余は (-1)^n と同じ符号を持ち、-1 < x < 0 の場合、< 0 になります。さらに、x > 0 の場合、0 ≤ t ≤ x で 1 + t ≥ 1 が成立し、−1 < x < 0 の場合、1 + t ≥ 1 − |x| になります。 x ≤ 0 の場合; よって残りの見積もり

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{n+1} \quad \text{for } x \geq 0 \tag{28}
$$

$$
\left| \int_0^x \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{(n+1)(1-|x|)} \quad \text{for } -1 < x \leq 0. \tag{29}
$$

これらの最後の 2 つの式から、−1 < x ≤ 1 の場合、次のことがすぐに推測されます。

$$
\log(1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n}
$$ (30)

系列は、]−1, +1] に含まれるすべてのコンパクト区間で一様に収束し、|x| については絶対収束します。 < 1.

一方、|x| の場合は、 > 1 (30) の右辺の系列の一般的な項は、n (III, p. 106) とともにサイズが無限に増加します。 x = −1 系列簡約するから高調波系列の場合、和 +∞ (Gen. Top.、IV、p. 365) になります。

同様に、(26) で置き換える x x^2 を計算し、0 と x の間の両辺を積分します。すべての実数 x に有効な、逆正接 x のテイラー展開位数 2n − 1 を取得します。

$$
\operatorname{Arc tan} x = \frac{x}{1} - \frac{x^3}{3} + \frac{x^5}{5} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{2n-1} + (-1)^n \int_0^x \frac{t^{2n} \, dt}{1 + t^2}. \tag{31}
$$

剰余は (−1)^n x の符号を持ち、すべての t について 1 + t^2 ≥ 1 であるため、推定値が得られます。

$$
\left| \int_0^x \frac{t^{2n} \, dt}{1 + t^2} \right| \leq \frac{|x|^{2n+1}}{2n+1} \tag{32}
$$

|x| については、そこから推測されます。 ≤ 1、

$$
\operatorname{Arc tan} x = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^{2n-1}}{2n-1} \tag{33}
$$

系列は [−1, +1] に一様収束し、|x| については絶対収束します。 < 1.

特に、x = 1 の場合、公式が得られます。

$$
\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} + \cdots + (-1)^n \frac{1}{2n+1} + \cdots .
$$

|x| の場合> 1 (33) の右辺の一般的な項は、n とともにサイズが無限に増加します。

最後に、Arc sin x のテイラー展開については、その導関数 (1 − x^2)^{-1/2} の展開から開始します。この最後の展開は、(1 + x)^{-1/2} の展開で置き換えること x by −x^2 を二項系列として取得します。 |x| の場合< 1 これで得られるのは

$$
(1 - x^2)^{-1/2} = 1 + \frac{1}{2} x^2 + \frac{1.3}{2.4} x^4 + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} x^{2n} + r_n(x)
$$

(23) により、制限付き

$$
0 \leq r_n(x) \leq \frac{x^{2n+2}}{\sqrt{1-x^2}}
$$

残りについては。

前の展開のプリミティブを取得すると、次のようになります。

$$
\text{Arc sin } x = x + \frac{1}{2} \frac{x^3}{3} + \frac{1.3}{2.4} \frac{x^5}{5} + \cdots + \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1} + R_n(x)
$$

ここで、R_n(x) は x の符号を持ち、不等式を満たします。

$$
|R_n(x)| \leq \int_0^x \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

さらに、関係 (35) は、x が 1 または −1 に近づくと R_n(x) が極限になる傾向があることを示しています。

$$
|R_n(1)| \leq \int_0^1 \frac{t^{2n+2} dt}{\sqrt{1-t^2}}.
$$

しかし、n が +∞ になる傾向がある場合、(37) の右辺は 0 になる傾向があります。つまり、整 $\int_0^1 dt / \sqrt{1-t^2}$ は収束するため、ε > 0 ごとに 0 < a < 1 および $\int_a^1 dt / \sqrt{1-t^2} \leq \varepsilon$ となる a が存在します。一方、私たちは持っています

$$
\int_0^a \frac{t^{2n+2} dt}{\sqrt{1-t^2}} \leq \frac{1}{\sqrt{1-a^2}} \int_0^a t^{2n+2} dt = \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}}
$$

したがって、n ≥ n_0 の場合、$\frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}} \leq \varepsilon$、よって、最後に |R_n(x)| となるような n_0 が存在します。 |x| の場合、≤ 2ε ≤ 1 かつ n ≥ n_0。したがって、人は

$$
\operatorname{Arc}\sin x = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{x^{2n+1}}{2n+1}
$$

(38)

右側は通常、コンパクト区間 [−1, 1] に収束します。

逆の場合、二項系列と同様に、(38) の右辺の系列の一般項が |x| の絶対値値で無限に増加することを示すことができます。 > 1.
たとえば、(38) に $x = \frac{1}{2}$ を入れると、数 $\pi$ の新しい式が得られます。

$$
\frac{\pi}{6} = \sum_{n=0}^{\infty} \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{1}{(2n+1)2^{2n+1}}
$$

これは、$\pi$ の近似値を計算するのに公式 (34) よりもはるかに適しています (数値計算を参照)。こうして得られるもの

$$
\pi = 3.141\,592\,653\ldots
$$

$1/10^9$.³以内の精度

3 数 $\pi$ は、無理数 (cf. III、p. 126、例題 5) であるだけでなく、1882 年にリンデマンによって初めて示されたように、有理数数の体 $\mathbf{Q}$ を超越さえします (参照たとえば、D Hilbert、Gesammelte Abhandlungen、v. 1、p. 1、ベルリン (Springer)、1932 年)。

### 練習問題 {#fvr-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
