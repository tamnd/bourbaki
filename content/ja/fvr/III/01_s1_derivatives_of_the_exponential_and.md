---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 1
section_title: DERIVATIVES OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS
lang: ja
source: fvr-i-vii
book_pages: 91-104, 115-125
pdf_pages: 0106-0119, 0130-0140
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF THE EXPONENTIAL FUNCTIONS; THE NUMBER $e$
      page: 91
      pdf_page: 106
    - "no": 2
      title: DERIVATIVE OF $\log_a x$
      page: 93
      pdf_page: 108
    - "no": 3
      title: DERIVATIVES OF THE CIRCULAR FUNCTIONS; THE NUMBER $\pi$
      page: 94
      pdf_page: 109
    - "no": 4
      title: INVERSE CIRCULAR FUNCTIONS
      page: 95
      pdf_page: 110
    - "no": 5
      title: THE COMPLEX EXPONENTIAL
      page: 97
      pdf_page: 112
    - "no": 6
      title: PROPERTIES OF THE FUNCTION $e^z$
      page: 98
      pdf_page: 113
    - "no": 7
      title: THE COMPLEX LOGARITHM
      page: 100
      pdf_page: 115
    - "no": 8
      title: PRIMITIVES OF RATIONAL FUNCTIONS
      page: 101
      pdf_page: 116
    - "no": 9
      title: COMPLEX CIRCULAR FUNCTIONS; HYPERBOLIC FUNCTIONS
      page: 102
      pdf_page: 117
statements: 9
exercises: 39
content_sha256: 6f933f2dc1702b89b86ab1a16ec6f8bd9b93b41981fdecc69cffd6c2e6027357
translated_from: content/en/fvr/III/01_s1_derivatives_of_the_exponential_and.md
translation_method: google
source_content_sha256: 4ac8e46f4200ac7e7f332753e43fe2ec6dc6c4857b2b82b1a42df8d051c7b1e2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 86201050fe027fc1c3b6942942d4fda097a21f0ff0214dda70e4937274861e9b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。指数関数と循環関数写像の導関数

### 1. 指数写像の導関数;ザ数 $e$

加法群 $\mathbf{R}$ から乗法群 $\mathbf{R}^*$ 実数 $\neq 0$ へのすべての連続準同型は、形 $x \mapsto a^x$ の写像 (指数関数写像と呼ばれます) であることがわかっています。 $a$ は数 $> 0$ (TG、V、p.11); $a \neq 1$なら$\mathbf{R}$の同型から乗法群の数の$\mathbf{R}_+^*$、$> 0$、$\mathbf{R}_+^*$から$\mathbf{R}$の逆同型は$\log_a x$で表され、 基底 $a$ の対数。

写像 $f(x) = a^x$ は、すべての $x \in \mathbf{R}$ に対して、形 $c.a^x$ (明らかに $c = f'(0)$) の導関数を持つことがわかります。これは、次の一般的な定理から得られます。

#### 定理 1 {#fvr-iii-s1-thm-1 .statement tag=089Q}

*E を、単位元 $\mathbf{e}$ を伴う完全ノルム代数体 $\mathbf{R}$ とし、$\mathbf{f}$ を、E の可逆元の乗法群 G への加法群 $\mathbf{R}$ の連続群準同型とする。 写像 $\mathbf{f}$ は $x \in \mathbf{R}$ ごとに微分可能であり、*

$$
\mathbf{f}'(x) = \mathbf{f}(x)\mathbf{f}'(0).
$$

まず、E は完全な代数であり、G は E で開いていることに注意します (*Gen. Top.*, IX, p. 179, prop. 14)。 写像 $g(x) = \int_0^a \mathbf{f}(x + t)\,dt$ を考えてみましょう。ここで、$a > 0$ は数であり、後で選ぶになります。 $\mathbf{f}(x + t) = \mathbf{f}(x)\mathbf{f}(t)$ から仮定までなので、$g(x) = \int_0^a \mathbf{f}(x)\mathbf{f}(t)\,dt = \mathbf{f}(x) \int_0^a \mathbf{f}(t)\,dt$ (I、p. 6、提案 3) になります。 $\alpha > 0$ を、ボール $\|x - \mathbf{e}\| \leq \alpha$ が G に含まれるようにする。 $\mathbf{f}(0) = \mathbf{e}$ と $\mathbf{f}$ は仮定まで連続しているため、$a$ は$[0, a]$ で $\|\mathbf{f}(t) - \mathbf{e}\| \leq \alpha$ となるほど十分小さいと想定できます。従って (II, p. 61, 公式 (16)) は次のようになります。

$$
\left\| \frac{1}{a} \int_0^a \mathbf{f}(t)\,dt - \mathbf{e} \right\| \leq \alpha,
$$

そして $\frac{1}{a} \int_0^a f(t) \, dt$ 属するを G に。他の語では、反転可能です。 $b = \int_0^a f(t) \, dt$ も同様で、$f(x) = g(x)b^{-1}$ と書くことができます。従って、 g が微分可能であることを示すだけで十分です。さて、変数 $x + t = u$ の変更により、$g(x) = \int_x^{x+a} f(u) \, du$ が得られます。 f は連続なので、g はすべての $x \in \mathbf{R}$ (II, p. 56、提案 3) に対して微分可能です。

$$
g'(x) = f(x+a) - f(x) = f(x)(f(a) - e).
$$

従って、$f'(x) = g'(x)b^{-1} = f(x)c$、ここでは$c = (f(a) - e)b^{-1}$、そして明らかに$f'(0) = c$です。

逆に、直接 (III、p. 115、演習 1)、または線形微分方程式 (IV、p. 188) の理論を使用して、$\mathbf{R}$ のすべての微分可能な写像 f が完全な正規化された代数 E になることを示すことができます。 $f'(x) = f(x)c$ と $f(0) = e$ は、加法群 $\mathbf{R}$ の準同型を乗法群 G に変換します。

#### 命題 1 {#fvr-iii-s1-prop-1 .statement tag=089R}

*すべての数 $a > 0$ と $\neq 1$ について、指数関数写像 $a^\lambda$ は、すべての点 $x \in \mathbf{R}$ で $(\log_e a)a^\lambda$ に等しい導関数を許容します。ここで、e は数 $> 1$ ($a$ とは独立しています)。

適用番目。 E が体 $\mathbf{R}$ である場合の 1 自体は、$a^\lambda$ が点ごとに $\varphi(a).a^\lambda$ に等しい導関数を持つことを示しています。ここで、$\varphi(a)$ は $a$ のみに依存して実数 $\neq 0$ です。 $b$ を 2 番目の数 $> 0$ と $\neq 1$ とします。 写像 $b^\lambda$ は、上記から $\varphi(b).b^\lambda$ に等しい導関数を持ちます。一方、$b^\lambda = a^\lambda \log_a b$ があるため、(I, p. 9、提案 5) $b^\lambda$ の導関数は $\log_a b.\varphi(a)b^\lambda$ に等しくなります。これら 2 つの式を比較すると、次のようになります。

$$
\varphi(b) = \varphi(a).\log_a b.
$$ (2)

$\varphi(b) = 1$ となるような固有の数 $b$ が 1 つあると推測します。 (2) により、この関係は $b = a^{1/\varphi(a)}$ に相当します。 e によって得られた実数を表すのが慣習的です。 (2) から 1 つは $\varphi(a) = \log_e a$ を持ち、これで prop の証明が完成します。 1.

$e^x$ の代わりに $\exp x$ と書くことがよくあります。

数 e の定義は次のことを示しています

$$
D(e^\lambda) = e^\lambda
$$ (3)

これは、$e^\lambda$ が真に増加する、したがって $e > 1$ であることを証明します。

§2 (III, p. 105) では、計算する任意に e に近似する方法を見ていきます。

#### 定義 1 {#fvr-iii-s1-def-1 .statement tag=089S}

*基底 e までの対数は、ネイペリアン対数 (または自然対数) と呼ばれます。

通常、ネイペリアン対数では記法の基底を省略します。 〜でない限り逆に、記法 $\log x$ ($x > 0$) は $x$ の *ネーペリアン対数* を表します。これで記法、小道具。 1 を ID として書くことができます

$$
D(a^\lambda) = (\log a)a^\lambda
$$ (4)

$a > 0$ ($a = 1$ の場合は $\log a = 0$) に有効です。

この関係は、 $a^x$ が *すべての位数* の導関数を持ち、
$$
D^n(a^x) = (\log a)^n a^x.
$$
(5)

特に、$a > 0$ と $\neq 1$ については、すべての $x \in \mathbf{R}$ に対して $D^2(a^x) > 0$ があり、したがって、$a^x$ は $\mathbf{R}$ (I、p. 31、系) に *厳密に凸* となります。このことから、次のことが導き出されます命題:

#### 命題 2 (「幾何平均不等式」) {#fvr-iii-s1-prop-2 .statement tag=089T}

*任意の数* $z_i > 0$ ($1 \leq i \leq n$) *および数* $p_i > 0$ *そのような* $\sum_{i=1}^n p_i = 1$、*1 つは*
$$
z_1^{p_1} z_2^{p_2} \cdots z_n^{p_n} \leq p_1 z_1 + p_2 z_2 + \cdots + p_n z_n.
$$
(6)
*さらに、(6) の 2 つの辺は * $z_i$ * が等しい場合にのみ等しい*。

$z_i = e^{x_i}$ を入れましょう。そうすると不等式 (6) と書くことができます
$$
\exp(p_1 x_1 + p_2 x_2 + \cdots + p_n x_n) \leq p_1 e^{x_1} + p_2 e^{x_2} + \cdots + p_n e^{x_n}.
$$
(7)
したがって、命題は prop から続きます。 I、p. 26の1が写像 $e^x$に適用され、厳密には$\mathbf{R}$に凸です。

(6) の左辺 (または右辺) は、*重み* $p_i$ ($1 \leq i \leq n$) に対する $n$ 数 $z_i$ の *加重幾何平均* (それぞれ *加重算術平均*) であると言われています。 $1 \leq i \leq n$ に対して $p_i = 1/n$ の場合、対応するの算術幾何平均は、$z_i$ の *通常の* 算術幾何平均と呼ばれます。すると、不等式 (6) と書くことができます。
$$
(z_1 z_2 \cdots z_n)^{1/n} \leq \frac{1}{n}(z_1 + z_2 + \cdots + z_n).
$$
(8)

### 2. $\log_a x$の導関数

$a^x$ は$a \neq 1$, 適用に対して$\mathbf{R}$ 上で厳密に単調であるため、逆微分規則写像 (I, p. 17, 提案 6) は、すべての $x > 0$ に対して次のようになります。
$$
D(\log_a x) = \frac{1}{x \log a}
$$
(9)
そして特に
$$
D(\log x) = \frac{1}{x}.
$$
(10)

$u$ が点 $x_0$ で導関数を認める実数写像で、$u(x_0) > 0$ である場合、写像 $\log u$ は点 $x_0$ で $u'(x_0)/u(x_0)$ に等しい導関数を認めます。特に、$x > 0$ の場合は $D(\log |x|) = 1/|x| = 1/x$ があり、
$$
D(\log |x|) = -\frac{1}{|x|} = \frac{1}{x}
$$
$x < 0$の場合;その他の語、$D(\log |x|) = 1/x$ はいずれかの $x \neq 0$ です。 1 つ目の結論するは、区間 $I$ において、実数写像 $u$ が零ではなく、有限導関数を認める場合、$\log |u(x)|$ は $I$ で $u'/u$ に等しい導関数を認めます。この導関数は、$u$ の *対数導関数* と呼ばれます。 $|u|^{\alpha}$ の対数導関数は $\alpha u'/u$ であり、積の対数導関数は因子の対数導関数の和に等しいことは明らかです。これらのルールは、多くの場合、写像の導関数計算するを最速で求める方法を提供します。彼らは特に、公式を再び与えます。
$$
D(x^{\alpha}) = \alpha x^{\alpha-1} \qquad (\alpha \text{ an arbitrary real number, } x > 0)
$$
これはすでに他の方法 (II、p. 69) によって示されています。

#### 例 {#fvr-iii-s1-n2-exa-1 .statement tag=089U}

$u$ が区間 $I$ 上の写像 $\neq 0$ で、$v$ が実数写像である場合、$\log(|u|^v) = v \cdot \log |u|$ なので、$u$ と $v$ が微分可能である場合
$$
\frac{1}{|u|^v} D(|u|^v) = v' \log |u| + v \frac{u'}{u}.
$$

### 3. 円形写像の派生語。ザ数 $\pi$

一般位相 (*Gen. Top.*、VIII、p. 106) では、加法群 $\mathbf{R}$ から乗法群 $\mathbf{U}$ の複素数までの連続準同型 $x \mapsto \mathbf{e}(x)$ を定義しました。 値 1;これは、主期間 1 と $\mathbf{e}\left(\frac{1}{4}\right) = i$ を持つ定期的な写像です。 $\mathbf{R}$ から $\mathbf{U}$ に続くすべての準同型は形 $x \mapsto \mathbf{e}(x/a)$ であることがわかっており (*loc. cit.*)、$\cos_a x = \mathscr{R}(\mathbf{e}(x/a)), \sin_a x = \mathscr{I}(\mathbf{e}(x/a))$ (*三角関数写像*、または *円周写像* を基底に代入する) $a$);これらの最後の写像は $\mathbf{R}$ から $[-1, +1]$ まで連続する写像であり、主期間 $a$ を持ちます。 $\sin_a(x + a/4) = \cos_a x, \quad \cos_a(x + a/4) = -\sin_a x$があり、写像 $\sin_a x$は区間 $[-a/4, a/4]$の増加するです。

#### 命題 3 {#fvr-iii-s1-prop-3 .statement tag=089V}

*The function* $\mathbf{e}(x)$ *has a derivative equal to* $2\pi i \mathbf{e}(x)$ *at every point of* $\mathbf{R}$, *where* $\pi$ *is a constant* $> 0$.

さて、th。 III、p. 51 の 1、E が複素数の体 $\mathbf{C}$ である場合に適用すると、関係 $\mathbf{e}'(x) = \mathbf{e}'(0) \mathbf{e}(x)$ が得られます。さらに、$\mathbf{e}(x)$ は定数ユークリッドノルムを持つため、$\mathbf{e}'(x)$ は$\mathbf{e}(x)$ と直交します (I, p. 7, *例 3*)。したがって、1 つは $\mathbf{e}'(0) = \alpha i$ となり、実数は $\alpha$ になります。 $\sin_1 x$ は $[-\frac{1}{4}, \frac{1}{4}]$ の増加するであるため、$x = 0$ の導関数は $\geqslant 0$ であるため、$\alpha \geqslant 0$ となり、$e(x)$ は定数ではないため、$\alpha > 0$ になります。 $2\pi$ によって得られる数 $\alpha$ を表すのが慣例です。

§2 (III、p. 23) では、数 $\pi$ に任意に計算する近似値を近づけることができる方法を示します。

したがって、公式となります。

$$
D \left( e \left( \frac{x}{a} \right) \right) = \frac{2\pi i}{a} e \left( \frac{x}{a} \right).
$$

この公式が $a = 2\pi$ の場合に単純化されることがわかります。これが、分析においてのみ、基底 $2\pi$ に対する循環写像を使用する理由です。これらの写像については、記法の基底を省略することに同意します。 〜でない限りは明示的に反対に言及されており、記法 $\cos x$、$\sin x$、$\tan x$ はそれぞれ $\cos_{2\pi} x$、$\sin_{2\pi} x$、$\tan_{2\pi} x$ を表します。

これらの規則を使用すると、$a = 2\pi$、公式 (12) と書くことができます。

$$
D(\cos x + i \sin x) = \cos \left( x + \frac{\pi}{2} \right) + i \sin \left( x + \frac{\pi}{2} \right),
$$

これは以下と同等です

$$
D(\cos x) = -\sin x, \qquad D(\sin x) = \cos x,
$$

どちらから推測するか

$$
D(\tan x) = 1 + \tan^2 x = \frac{1}{\cos^2 x}.
$$

3 つの円形写像 $\cos x$、$\sin x$、および $\tan x$ に加えて、数値計算では 3 つの補助的な写像も使用します: コタンジェント、セカント、コセカント。次の式で定義されます。

$$
\cot x = \frac{1}{\tan x}, \qquad \sec x = \frac{1}{\cos x}, \qquad \operatorname{cosec} x = \frac{1}{\sin x}.
$$

(Gen. Top.、VIII、p. 109) 対応するから基底 $2\pi$ までの角度がラジアンと呼ばれることを思い出してください。

### 4. 逆循環写像

写像 $\sin x$ から区間 $[-\pi/2, +\pi/2]$ の制限は真に増加するです。 1 つはその逆を $\operatorname{Arc}\sin x$ で表し、したがって区間 $[-1, +1]$ の写像が $[-\pi/2, +\pi/2]$ に連続する真に増加するになります (図 6)。 公式逆微分写像 (I, p. 9, prop. 6) は、この写像の導関数を与えます。

$$
D(\operatorname{Arc}\sin x) = \frac{1}{\cos(\operatorname{Arc}\sin x)}.
$$

$-\pi/2 \leq \operatorname{Arc}\sin x \leq \pi/2$ から $\cos(\operatorname{Arc}\sin x) \geq 0$ があり、

$$
\sin(\operatorname{Arc}\sin x) = x,
$$
$\cos(\operatorname{Arc}\sin x) = \sqrt{1 - x^2}$ があり、そこから
$$
\mathrm{D}(\operatorname{Arc}\sin x) = \frac{1}{\sqrt{1 - x^2}}.
$$
同様に、$\cos x$ から区間 $[0, \pi]$ の制限は真に減少するです。 1 つはその逆写像を $\operatorname{Arc}\cos x$ で表し、これは $[-1, +1]$ の真に減少する写像を $[0, \pi]$ に表します (図 6)。さらに

![y = Arc cos x および y = Arc sin x を示すグラフ](https://i.imgur.com/3Q5z5QG.png)

図6

$$
\sin \left( \frac{\pi}{2} - \operatorname{Arc}\cos x \right) = \cos(\operatorname{Arc}\cos x) = x
$$
$-\pi/2 \leq \pi/2 - \operatorname{Arc}\cos x \leq \pi/2$ 以来、
$$
\operatorname{Arc}\cos x = \frac{\pi}{2} - \operatorname{Arc}\sin x
$$
特にそこから次のことがわかります
$$
\mathrm{D}(\operatorname{Arc}\cos x) = -\frac{1}{\sqrt{1 - x^2}}.
$$

最後に、tan x の区間 ]−π/2, +π/2[ の制限は真に増加するです。 1 つはその逆関数を Arctan x で表し、これは \mathbf{R} から ]−π/2, +π/2[ への真に増加する写像 (図 7)。我々は持っています

$$
\lim_{x \to -\infty} \operatorname{Arc tan} x = -\frac{\pi}{2}, \quad \lim_{x \to +\infty} \operatorname{Arc tan} x = \frac{\pi}{2},
$$

そして、III、p. 95 の逆写像と公式 (15) を微分するための適用公式により、次のようになります。

$$
\mathrm{D}\left( \operatorname{Arc tan} x \right) = \frac{1}{1 + x^2}.
$$

![y = 逆正接 x を示すグラフ](https://i.imgur.com/3Q5z5QG.png)

図7

### 5. 複素指数関数

(Gen. Top., VIII, p. 106) 複素数の (加法的) トポロジー 群 \mathbf{C} のすべての連続準同型を、複素数の (乗法) トポロジー 群 \mathbf{C}^* 上に決定しました。 ≠ 0;これらは写像です

$$
x + i y \mapsto e^{\alpha x + \beta y} \mathbf{e}(\gamma x + \delta y)
$$

ここで、$\alpha, \beta, \gamma, \delta$ は、単一の条件 $\alpha \delta - \beta \gamma \neq 0$ に従う 4 つの実数です。ここで、これら準同型 $z \mapsto f(z)$ のどれが \mathbf{C} で*微分可能*であるかを決定するに提案します。まず、$f$ が点 $z = 0$ で微分可能であれば十分であることに注意します。実際、点 $z \in \mathbf{C}$ ごとに、人は

$$
\frac{f(z + h) - f(z)}{h} = f(z) \frac{f(h) - 1}{h}
$$

$f'(0)$ が存在する場合、$f'(z)$、$f'(z) = a f(z)$、$a = f'(0)$ も存在します。一方、$g$ が 2 階微分可能な準同型である場合、$g'(z) = b g(z)$ の場合、$g(a z / b) = f(z)$、1 つの注意に対して、商 $g(a z / b) / f(z)$ はどこでも零導関数を持ち、$z = 0$ では 1 に等しくなります。したがって、微分可能なすべての準同型は形 $z \mapsto f(\lambda z)$ になります。ここで、$f$ はそのうちの 1 つ (存在すると仮定)、$\lambda$ は任意の (複素) 定数です。

そうなると、$f$ が点 $z = 0$ で微分可能である場合、$\mathbf{R}$ の $\mathbf{C}$ へのそれぞれの写像 $x \mapsto f(x),\ y \mapsto f(iy)$ は必ず点 $0$ で微分可能であり、最初のものは導関数 $f'(0)$ を持ち、2 番目は微分可能です。 $if'(0)$。 ここで、点 $0$ における写像 $x \mapsto e^{\alpha x} \mathbf{e}(\gamma x),\ y \mapsto e^{\beta y} \mathbf{e}(\delta y)$ の導関数は、それぞれ $\alpha + 2\pi i \gamma$ と $\beta + 2\pi i \delta$ に等しく、そこから $\beta = -2\pi \gamma$ と $\alpha = 2\pi \delta$ が求められます。これらの条件は、特に準同型 $x + iy \mapsto e^z \mathbf{e}(y/2\pi)$ によって満たされます。これを暫定的に $f_0$ で表すことにします。 ここで、$f_0$ が実際に点 $z = 0$ で微分可能であることを示します。

$x \mapsto f_0(x)$ と $y \mapsto f_0(iy)$ にはすべての位数の導関数があることは明らかです。特に、テイラーの位数 1 の公式をこれらの写像に適用すると、すべての $\varepsilon > 0$ に対して次のような $r > 0$ が存在することがわかります。

$$
f_0(x) = 1 + x + \varphi(x)x,\qquad f_0(iy) = 1 + iy + \psi(y)y,
$$

次に、条件 $|x| \leq r,\ |y| \leq r$ は $|\varphi(x)| \leq \varepsilon$ と $|\psi(y)| \leq \varepsilon$ を意味します。そうなると、$f_0(x + iy) = f_0(x)f_0(iy) = 1 + (x + iy) + \theta(x,\ y)$ になります。

$$
\theta(x,\ y) = (i + \varphi(x)\psi(y))xy + (1 + x)y\psi(y) + (1 + iy)x\varphi(x);
$$

$|z| \leq r$ には、$|x| \leq r$ と $|y| \leq r$、よってがあります

$$
|\theta(x,\ y)| \leq (1 + \varepsilon^2)|z|^2 + 2\varepsilon|z|(1 + |z|)
$$

これは、商 $\frac{f_0(z) - 1 - z}{z}$ が $z$ で 0 になる傾向があることを証明します。つまり、写像 $f_0$ は点 $z = 0$ で 1 に等しい導関数を認めます。したがって、上記はすべての $z \in \mathbf{C}$ について、

$$
D(f_0(z)) = f_0(z).
$$

この性質は、$f_0$ と写像 $e^z$ の間の接続を確立します。さらに、実軸に対する $f_0$ の制限です。このため、次の定義を作成します。

#### 定義 2 {#fvr-iii-s1-def-2 .statement tag=089W}

*準同型* $x + iy \mapsto e^z \mathbf{e}(y/2\pi)$ *of* $\mathbf{C}$ *onto* $\mathbf{C}^*$ *は複素指数と呼ばれます。任意の複素数* $z$ におけるその値は * $e^z$ * または* $\exp z$ で表されます。

### 6. 写像 $e^z$ の特性

$z \mapsto e^z$ が $\mathbf{C}$ の $\mathbf{C}^*$ 上の準同型であるという事実は、恒等式によって表現される可能性があります。

$$
e^{z+z'} = e^z e^{z'},\qquad e^0 = 1.\qquad e^{-z} = 1/e^z.
$$

定義までに、$z = x + iy$ごとに、1人が、

$$
e^{x+iy} = e^x (\cos y + i \sin y)
$$

そして $e^{\lambda} > 0$ 以降、$e^z$ には *絶対値* $e^{\lambda}$ と *振幅* $y$ (モジュロ $2\pi$) があることが分かります。

特に、デフ。 2 (III, p. 98) を与える
$$
\mathbf{e}(x) = e^{2\pi i x}
$$
これにより、形で $\cos x$ と $\sin x$ を定義する式を書くことができます。
$$
\cos x = \frac{1}{2} (e^{i x} + e^{-i x}), \qquad \sin x = \frac{1}{2i} (e^{i x} - e^{-i x})
$$
*(オイラーの公式)*。

$2\pi$ は $\mathbf{e}(y/2\pi)$ の主期間であるため、$2\pi i$ は $e^z$ の *主期間* です。他の例では、$e^z$ の期間の語、群は、数 $2n\pi i$ の集合であり、$n$ は $\mathbf{Z}$ まで続きます。

最後に、III, p. 98 の公式 (21) が書けます
$$
\mathrm{D}(e^z) = e^z
$$
よって、複素数 $a$ごとに
$$
\mathrm{D}(e^{a z}) = a\, e^{a z}.
$$

#### 注意 {#fvr-iii-s1-n6-rem-1 .statement tag=089X}

公式 (27) で、制限する写像 $e^{a z}$ ($a$ 複素数) を実数軸にすると、$x$ 実数に対して、
$$
\mathrm{D}(e^{a x}) = a\, e^{a x}.
$$
この公式により、写像、$e^{\alpha x} \cos \beta x$、$e^{\alpha x} \sin \beta x$ ($\alpha$ および $\beta$ 実数) のそれぞれに対してプリミティブを計算する作成できます。確かに$e^{(\alpha + i \beta)x} = e^{\alpha x} \cos \beta x + i e^{\alpha x} \sin \beta x$があるので、(28)までに
$$
\mathrm{D}\left( \mathscr{R}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \cos \beta x
$$
$$
\mathrm{D}\left( \mathscr{I}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \sin \beta x.
$$
同様に、簡約する $x^n e^{\alpha x} \cos \beta x$ または $x^n e^{\alpha x} \sin \beta x$ (*n* *整数* $> 0$) のプリミティブの評価を $x^n e^{(\alpha + i \beta)x}$ のプリミティブの評価に変換します。さて、位数 $n + 1$ (II, p. 60, 公式 (11)) の部分による積分の公式は、この最後の写像のプリミティブが
$$
e^{(\alpha + i \beta)x} \left[ \frac{x^n}{\alpha + i \beta} - \frac{n x^{n-1}}{(\alpha + i \beta)^2} + \frac{n(n-1)x^{n-2}}{(\alpha + i \beta)^3} + \cdots + (-1)^n \frac{n!}{(\alpha + i \beta)^{n+1}} \right].
$$
一方、オイラーの公式では、$\cos x$ または $\sin x$ のすべての正の積分冪を、指数関数 $e^{ip x}$ ($p$ は正または負の整数) の線形結合として表すことができます。したがって、公式 (28) によって、形 $x^n e^{\alpha x} (\cos \beta x)' (\sin \gamma x)^s$ の写像のプリミティブを、形 $x^p e^{\alpha x} \cos \lambda x$ および $x^p e^{\alpha x} \sin \mu x$ および ($n, p, r, s$) の写像の線形結合として表現できます。 整数、$\alpha, \beta, \gamma, \lambda, \mu$ 本物）。

#### 例 {#fvr-iii-s1-n6-exa-1 .statement tag=089Y}

1つは持っています

$$
\sin^{2n} x = \frac{(-1)^n}{2^{2n}} \left( e^{i x} - e^{-i x} \right)^{2n} = \frac{(-1)^n}{2^{2n}} \left( e^{2n i x} - \binom{2n}{1} e^{(2n-2)i x} + \cdots + e^{-2n i x} \right)
$$

よって

$$
\int_0^1 \sin^{2n} t \, dt = \frac{(-1)^n}{2^{2n}} \left( \frac{1}{n} \sin 2n x - \binom{2n}{1} \frac{1}{n-1} \sin(2n-2)x + \cdots \right.
$$
$$
\left. + (-1)^{n-1} \binom{2n}{n-1} \sin 2x + (-1)^n \binom{2n}{n} x \right)
$$

そして特に

$$
\int_0^{\pi/2} \sin^{2n} t \, dt = \binom{2n}{n} \frac{1}{2^{2n}} \frac{\pi}{2} = \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{\pi}{2}.
$$ (29)

### 7. 複素対数

B を、$-\pi \leq y < \pi$ となるような点 $z = x + i y$ によって形成される「ストリップ」とします。 写像 $e^z$ は、B でそれぞれの値を 1 回だけ受け取ります。他の語では、$z \mapsto e^z$はBの$\mathbf{C}^*$への全単射連続写像です。 (半開き) セグメント $x = x_0,\ -\pi \leq y < \pi$ のこの写像の下にある像は円 $|z| = e^{x_0}$ です。ライン$y = y_0$の像は、$\mathrm{Am}(z) = y_0$（修正$2\pi$）で定義された（開いた）ハーフラインです。 B の内部 $\dot{B}$ の $z \mapsto e^z$ の下の像、つまり $z \in \mathbf{C}$ の集合の$|\mathscr{I}(z)| < \pi$ は、$\mathbf{C}$ の (閉じた) 負の実数半軸の補数 F です。 属するから $[-\pi, \pi[$ までの $z$ の振幅の尺度を $\mathrm{Am}(z)$ で表すことに同意する場合、集合 F は関係 $-\pi < \mathrm{Am}(z) < \pi$ で定義できます。 $z \mapsto e^z$ は $\mathbf{C}^*$ 像に対する $\mathbf{C}$ の厳密な準同型であるため、この写像の B のオープン部分集合 (つまり $\mathbf{C}$) は、$\mathbf{C}^*$ のオープン集合になります (つまり F)。他の語、制限では、B に対する $z \mapsto e^z$ の制限は、F に対する $\dot{B}$ の同型写像です。後者の逆である B に対する F の同型写像を $z \mapsto \log z$ で表します。 複素数 $z \in F$ の場合、$\log z$ は $z$ の対数の主値と呼ばれます。 $z = x + i y$ と $\log z = u + i v$ なら、$x + i y = e^{u+i v}$、よって $e^u = |z|$、$-\pi < v < \pi$ なので、$v = \mathrm{Am}(z)$ になります。さらに、$y \neq 0$ の場合は $\tan(v + \pi/2) = -x/y$ になります。したがって、次のように書くことができます

$$
\begin{cases}
u = \log |z| = \frac{1}{2} \log(x^2 + y^2) \\
v = \frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y > 0 \\
v = 0 & \text{if } y = 0 \\
v = -\frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y < 0.
\end{cases}
$$ (30)

$\log z$ は、正の開いた実半軸 $\mathbf{R}_+^*$ 上で定義された写像 $\log x$ の F に対する拡大であることは明らかです。 $z,\ z'$ が F の 2 つの点で、$zz'$ が実負でない場合、$\log(zz') = \log z + \log z' + 2\varepsilon \pi i$ が得られます。ここで、$\mathrm{Am}(z)$ と $\mathrm{Am}(z')$ の値に応じて、$\varepsilon = +1,\ -1$ または 0 になります。

負の実数半軸の点では、関数 $\log z$ には制限がないことに注意してください。正確に言うと、$x$ が $x_0 < 0$ になる傾向があり、$y$ が 0 残り > 0 (それぞれ < 0) になる傾向がある場合、$\log z$ は $\log |x_0| + \pi i$ (それぞれ $\log |x_0| - \pi i$) になる傾向があります。 $z$ が 0 に近づくと、$|\log z|$ は無限に増加します。

解析的写像の理論により、完全な一般性で拡大する写像 $\log z$ と複素対数定義するがどのように可能になるかについては後で説明します。

$\log z$ は $e^z$ の逆同型写像であるため、逆写像を微分するための公式 (I, p. 9, prop. 6) は、$\log z$ が点 $z \in \mathbf{F}$ ごとに微分可能であることを示し、
$$
\mathrm{D}(\log z) = \frac{1}{e^{\log z}} = \frac{1}{z}
$$
III、p. 93 の公式 (10) を一般化する公式。

### 8. 有理数のプリミティブ写像

公式 (31) により、実変数 $x$ の任意の有理数写像 $r(x)$ の原始関数を実数または複素数係数で評価できます。私たちは (A.VII.7)、そのような写像が項の有限和として (独自の方法で) 記述できることを知っています。

a) 形 $ax^p$ ($p$ 整数 $\geqslant 0$、$a$ 複素数) のいずれか。
b) または形 $a/(x-b)^m$ ($m$ 整数 $\geqslant 0$、$a$ および $b$ 複素数)。

これで、これら項のそれぞれのプリミティブを簡単に取得できます。
a) $ax^p$ のプリミティブは $a \frac{x^{p+1}}{p+1}$ です。
b) $a/(x-b)^m$ のプリミティブ $m > 1$ が $\frac{a}{(1-m)(x-b)^{m-1}}$ の場合。
c) 最後に、式 (10) (III, p. 93) と (31) (III, p. 101) から、$b$ が実数の場合、$\frac{a}{x-b}$ の原始関数は $a \log |x-b|$、$b$ が複素数の場合、$a \log(x-b)$ になります。最後の場合、$b = p + iq$ の場合、さらに (III, p. 100, 式 (30)) が成立します。
$$
\log(x-b) = \log \sqrt{(x-p)^2 + q^2} + i \operatorname{Arc tan} \frac{x-p}{q} \pm i \frac{\pi}{2}.
$$

数値計算に特化したこの研究の部分に明示的に与えられた有理数写像のプリミティブを明示的に決定するためのより実用的な方法の検討は延期します。

有理数写像のプリミティブの評価を簡約する行うことができます。

1° 形 $r(e^{a x})$ の写像のプリミティブの評価。ここで、$r$ は有理数写像および $a$ 実数です。実際、変数 $u = e^{a x}$ の変更 1 簡約するにより、$r(u)/u$ のプリミティブが見つかります。

2° 形 $f(\sin a x, \cos a x)$ の写像のプリミティブの評価。ここで、$f$ は 2 つの変数の有理数写像で、$a$ は実数です。 変更の変数 $u = \tan(a x/2)$ 簡約するこれは、次のプリミティブを見つけるためのものです。

$$
\frac{2}{1 + u^2} \int \left( \frac{2u}{1 + u^2}, \frac{1 - u^2}{1 + u^2} \right).
$$

### 9. 複雑な円形写像;双曲線写像

オイラーの公式 (25) (III, p. 99) と $e^z$ の定義により、すべての複素数 $z$ に対して、 拡大するから $\mathbf{C}$ 写像 $\cos x$ および $\sin x$ が $\mathbf{R}$ で定義されます。皆さんにとって、$z \in \mathbf{C}$

$$
\cos z = \frac{1}{2} (e^{i z} + e^{-i z}), \qquad \sin z = \frac{1}{2i} (e^{i z} - e^{-i z})
$$
(cf. III、p. 119、演習 19)。

これらの写像は主周期 $2 \pi$ で周期的です。つまり、1 つは $\cos(z + \pi/2) = -\sin z, \sin(z + \pi/2) = \cos z$ です。身元を確認することもできます

$$
\cos^2 z + \sin^2 z = 1 \\
\cos(z + z') = \cos z \cos z' - \sin z \sin z' \\
\sin(z + z') = \sin z \cos z' + \cos z \sin z'.
$$

より一般的には、実変数の循環写像間のすべての代数恒等式は、これらの変数に任意の複素数値 (III、p. 119、演習 18) を与えても真のままです。

$z \neq (2k + 1)\pi/2$の場合は$\tan z = \sin z / \cos z$、$z \neq k \pi$の場合は$\cot z = \cos z / \sin z$を置きます。これらは周期的写像で、主周期は $\pi$ です。

公式 (27) (III, p. 99) は、$\cos z$ と $\sin z$ が $\mathbf{C}$ で微分可能であることを示します。

$$
\mathrm{D}(\cos z) = -\sin z, \qquad \mathrm{D}(\sin z) = \cos z.
$$

$z = i x$ ($x$ 実数) の場合、式 (32) は次のようになります。

$$
\cos i x = \frac{1}{2} (e^i + e^{-i}), \qquad \sin i x = \frac{i}{2} (e^i - e^{-i}).
$$

このように導入された実際の写像に対して特定の記法を用意しておくと便利です。私たちは置きます

$$
\begin{cases}
\cosh x = \frac{1}{2} (e^x + e^{-x}) & \text{(hyperbolic cosine of } x \text{)} \\
\sinh x = \frac{1}{2} (e^x - e^{-x}) & \text{(hyperbolic sine of } x \text{)} \\
\tanh x = \frac{\sinh x}{\cosh x} = \frac{e^x - e^{-x}}{e^x + e^{-x}} & \text{(hyperbolic tangent of } x \text{)}
\end{cases}
$$

したがって、実数 $x$ ごとに、

$$
\cos i x = \cosh x, \quad \sin i x = i \sinh x.
$$

複素数 $z_k$ ($1 \leq k \leq n$) の特定の数における円形写像間のすべての同一性から、置き換えること $z_k$ $i x_k$ ($x_k$ 実数、$1 \leq k \leq n$) による双曲写像の同一性を推定できます。そして式（３４）を使用する。たとえば、ある人は

$$
\cosh^2 x - \sinh^2 x = 1
$$
$$
\cosh(x + x') = \cosh x \cosh x' + \sinh x \sinh x'
$$
$$
\sinh(x + x') = \sinh x \cosh x' - \cosh x \sinh x'.
$$

双曲線写像を使用すると、$z = x + i y$ に対する $\cos z$ と $\sin z$ の実数と虚数部分を表現できます。

$$
\cos(x + i y) = \cos x \cos i y - \sin x \sin i y = \cos x \cosh y - i \sin x \sinh y
$$
$$
\sin(x + i y) = \sin x \cos i y + \cos x \sin i y = \sin x \cosh y + i \cos x \sinh y.
$$

最後に、1つは、

$$
D(\cosh x) = \sinh x, \quad D(\sinh x) = \cosh x, \quad D(\tanh x) = 1 - \tanh^2 x = \frac{1}{\cosh^2 x}.
$$

すべての $x$ に対して $\cosh x > 0$ であるため、$\sinh x$ は $\mathbf{R}$ で真に増加するであると推測されます。 $\sinh 0 = 0$ なので、$\sinh x$ は $x$ と同じ符号を持つことになります。 帰結では、$\cosh x$は$x \leq 0$の真に減少する、$x \geq 0$の真に増加する、最後に、$\tanh x$は$\mathbf{R}$の真に増加するです。さらに

$$
\lim_{x \to -\infty} \sinh x = -\infty, \qquad \lim_{x \to +\infty} \sinh x = +\infty
$$
$$
\lim_{x \to -\infty} \cosh x = \lim_{x \to +\infty} \cosh x = +\infty
$$
$$
\lim_{x \to -\infty} \tanh x = -1, \qquad \lim_{x \to +\infty} \tanh x = +1 \qquad \text{(fig. 8 and 9)}.
$$

ときどきは、$\sinh x$の逆数写像、つまり$\mathbf{R}$から$\mathbf{R}$への真に増加する写像を$\operatorname{Arg} \sinh x$と書きます。この写像は、対数の項でも表すことができます。 関係 $x = \sinh y = \frac{1}{2}(e^y - e^{-y})$ から $e^{2y} - 2x e^y - 1 = 0$ が推定され、$e^y > 0$ から $e^y = x + \sqrt{x^2 + 1}$ が得られます。

$$
\operatorname{Arg} \sinh x = \log \left( x + \sqrt{x^2 + 1} \right).
$$

同様に、$\cosh x$ から $[0, +\infty[$ の制限の逆数を $\operatorname{Arg} \cosh x$ で表します。この写像は$]1, +\infty[$から$]0, +\infty[$への真に増加するです。 1つは上記のように示しています

$$
\operatorname{Arg} \cosh x = \log \left( x + \sqrt{x^2 - 1} \right).
$$

最後に、Arg Tanh $x$ によって、tanh $x$ の逆数写像を表します。これは、]$-1, +1$ [ から $\mathbf{R}$ への真に増加する写像です。さらに、

$$
\operatorname{Arg} \tanh x = \frac{1}{2} \log \frac{1 + x}{1 - x}.
$$

#### 注意 {#fvr-iii-s1-n9-rem-1 .statement tag=089Z}

複素数 $z$ の場合、1 つのときどきが書き込みます

$$
\cosh z = \frac{1}{2} (e^z + e^{-z}) = \cos iz \\
\sinh z = \frac{1}{2} (e^z - e^{-z}) = -i \sin iz.
$$

したがって、これらの写像は、$\mathbf{R}$ で定義された双曲線写像から拡大するに$\mathbf{C}$ になります。

### 練習問題 {#fvr-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
