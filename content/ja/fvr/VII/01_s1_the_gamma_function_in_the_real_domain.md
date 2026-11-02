---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 1
section_title: THE GAMMA FUNCTION IN THE REAL DOMAIN
lang: ja
source: fvr-i-vii
book_pages: 305-314, 325-327
pdf_pages: 0320-0329, 0340-0342
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE GAMMA FUNCTION
      page: 305
      pdf_page: 320
    - "no": 2
      title: PROPERTIES OF THE GAMMA FUNCTION
      page: 307
      pdf_page: 322
    - "no": 3
      title: THE EULER INTEGRALS
      page: 310
      pdf_page: 325
statements: 8
exercises: 6
content_sha256: ee972b075aaa74761f8f96bfc057a60d470201e9faea53982d333e255f7e5f34
translated_from: content/en/fvr/VII/01_s1_the_gamma_function_in_the_real_domain.md
translation_method: google
source_content_sha256: c14b2d3b10b39cdfef4ea9acb546a2878e81232b29d6cdb8928fc7269171f7f2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: fecdd1549db3e8bce33143a1f69b04f6b80acbbcb397d48cbbd59d1cc8ebdc85
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。実領域のガンマ写像

### 1. ガンマ写像の定義

整数 $n \geq 0$ ごとに (集合理論, III, p. 179) 写像 $n!$ を積 $\prod_{0 \leq k < n} (n - k)$ と等しいものとして定義しました。つまり、$n \geq 0$ の場合は $0! = 1$ と $(n + 1)! = (n + 1)\, n!$ です。

整数 $n \geq 1$ ごとに集合 $\Gamma(n) = (n - 1)!$ となります。私たちは、実数 $x > 0$ の集合上で整数 $\geq 1$ の集合で定義された写像 $\Gamma$ を延長する連続写像 $\Gamma(x)$ で定義するを提案します。

そのような写像が無数に存在することは明らかです。 整数 $n \geq 1$ ごとに $\Gamma(n + 1) = n\Gamma(n)$ から、拡大する $\Gamma$ の連続写像のうち、満たすの方程式を満たすものを考慮することに限定します。

$$
f(x + 1) = x f(x)
$$

$x > 0$ごとに。

この方程式の解が$\Gamma(n)$の拡大となるためには、$f(1) = 1$も満たすことが必要かつ十分です。

$f$ が (1) を満たす場合、$n$ の再帰により、

$$
f(x + n) = x(x + 1)(x + 2) \ldots (x + n - 1)\, f(x)
$$

すべての整数 $n > 1$ とすべての $x > 0$ について。この関係は、特に、区間 $]n, n + 1]$ ($n$ 整数 $\geq 1$) の $f$ の値が、区間 $]0, 1]$ の値によって決定されることを示しています。逆に、$\varphi$ を、$]0, 1]$ 満たす条件 $\varphi(1) = 1$、$\lim_{x \to 0} x \varphi(x) = 1$ のみで連続する写像とします。 整数 $n \geq 1$ ごとに区間 $]n, n + 1]$ に関係までに定義する $f$ にしましょう

$$
f(x) = (x - 1)(x - 2) \ldots (x - n)\, \varphi(x - n);
$$

$f$ が $]0, +\infty[$ で連続であり、式 (1) を満たし、拡大する $\Gamma(n)$ を満たしていることは明らかです。

$f$ が (1) の連続解で、$]0, 1]$ で値 $> 0$ がかかる場合、(2) により、$]0, +\infty[$ で値 $> 0$ がかかります。次に、写像 $g(x) = \log f(x)$ が定義され、]0、+∞[ で連続し、次の方程式を満たします。

$$
g(x+1) - g(x) = \log x
$$

(3)

この区間で。

$g_1$ が ]0, +∞[ 上の (3) の 2 番目の連続解であり、$h = g_1 - g$ の場合、$x > 0$ ごとに $h(x+1) - h(x) = 0$ が得られます。他の語、$h$ は、周期 1 の連続周期写像であり、]0、+∞[ で定義されます。逆に、この性質のすべての $h$ に対して、 $g + h$ は (3) の連続した解になります。

#### 命題 1 {#fvr-vii-s1-prop-1 .statement tag=08IX}

*凸型写像* $g$ *上で定義* ]0, +∞[ *方程式* (3) を満たし、 * $x = 1$ に対して値 0 をとります* が 1 つだけ存在します。

まず、写像 $g$ 満たす条件が指定されている場合、それは区間 ]0, 1] でよく決まり、その結果区間 ]0, +∞[ でよく決まることを示します。 Indeed, for every integer $n > 1$ the gradient of the line joining the point $(n, g(n))$ to the point $(x, g(x))$ is an increasing function of $x$, since $g$ is convex (I, p. 27, prop. 5); one thus must have, for $0 < x \leq 1$,

$$
\frac{g(n-1) - g(n)}{(n-1) - n} \leq \frac{g(n+x) - g(n)}{(n+x) - n} \leq \frac{g(n+1) - g(n)}{(n+1) - n}
$$

つまり、(3) により、

$$
x \log(n-1) \leq g(x+n) - g(n) \leq x \log n.
$$

さて、(3)により、

$$
g(x+n) - g(n) = g(x) + \log x + \sum_{k=1}^{n-1} (\log(x+k) - \log k).
$$

さらに、$\log n = \sum_{k=2}^n \log \frac{k}{k-1}$ と書けるので、不等式 (4) と書くことができます。

$$
x \sum_{k=2}^{n-1} \log \frac{k}{k-1} \leq g(x) + \log x + \sum_{k=2}^n (\log(x+k-1) - \log(k-1))
$$
$$
\leq x \sum_{k=2}^n \log \frac{k}{k-1}.
$$

$n \geq 2$ ごとに、

$$
u_n(x) = x \log \frac{n}{n-1} - \log(x+n-1) + \log(n-1)
$$

(5)

そして

$$
g_n(x) = -\log x + \sum_{k=2}^n u_k(x).
$$

$0 < x \leq 1$ の場合、次のようになります。
$$
g_n(x) - x \log \frac{n}{n-1} \leq g(x) \leq g_n(x).
$$
(6)

$n$ が $+\infty$ になる傾向があるのと同様に、$\log \frac{n}{n-1}$ は 0 になる傾向があるため、解 $g$ が存在する場合、$]0, 1]$ において$g_n(x)$ の *極限* と必然的に等しいことが (6) から推測されます。

ここで、(5) から、$x$ が固定され、$> 0$ については次のことがすぐに推測されます。
$$
u_n(x) = -x \log \left( 1 - \frac{1}{n} \right) - \log \left( 1 + \frac{x-1}{n} \right) + \log \left( 1 - \frac{1}{n} \right) \sim \frac{x(x-1)}{2n^2}
$$
$n$ は $+\infty$ になる傾向があるため、系列と一般的な項 $u_n(x)$ が $x > 0$ ごとに収束することが証明されます。 写像 $u_n(x)$ はそれぞれ$]0, +\infty[$ に凸であり、$-\log x$ と同様に、写像 $g(x) = -\log x + \sum_{n=2}^{\infty} u_n(x)$ はこの区間に凸です (I、p. 27、提案 2 および提案 4)。最後に、$u_n(1) = 0$、よって $g(1) = 0$、そして
$$
u_n(x+1) = u_{n+1}(x) + x \left( \log \frac{n}{n-1} - \log \frac{n+1}{n} \right)
$$
よって
$$
g(x+1) = -\log(x+1) + x \log 2 + \sum_{n=3}^{\infty} u_n(x) = \log x + g(x);
$$
その他の語、$g$はVII、p. 306の式(3)を満たします。

#### 定義 1 {#fvr-vii-s1-def-1 .statement tag=08IY}

*$\Gamma(x)$ *写像* $> 0$ *これは区間* $]0, +\infty[$ で定義され、 *方程式を満たす*
$$
\Gamma(x+1) = x \Gamma(x),
$$
*(7)*
*そしてそれは* $\Gamma(1) = 1$ *そしてそれ* $\log \Gamma(x)$ *は* $]0, +\infty[$に凸です。

### 2. ガンマ写像の特性

#### 命題 2 {#fvr-vii-s1-prop-2 .statement tag=08IZ}

*すべて* $x > 0$ *1 つは持っています*
$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x n!}{x(x+1)\ldots(x+n)}
$$
*(ガウスの公式)*、*および*
$$
\Gamma(x) = e^{-\gamma x} \frac{1}{x} \prod_{n=1}^{\infty} \frac{e^{x/n}}{1 + \frac{x}{n}}
$$
(9) ここで、$\gamma$ はオイラー定数を表し、(9) の右辺の無限大積は、含む整数 $< 0$ ではなく、$\mathbf{R}$ のすべてのコンパクト区間に絶対的かつ一様に収束します (ヴァイエルシュトラスの公式)。

写像 $\Gamma(x)$ は $]0, +\infty[$ で無限微分可能であり、1 は

$$
\frac{\Gamma'(x)}{\Gamma(x)} = -\gamma - \frac{1}{x} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{x+n} \right)
$$

そして

$$
\mathrm{D}^k (\log \Gamma(x)) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(x+n)^k} \quad \text{for} \quad k \geq 2,
$$

(10) と (11) の右辺の系列は、すべてのコンパクト区間含む整数 $\leq 0$ に絶対的かつ一様に収束します。

確かに、プロップの証明。 VII、p. 306 の 1 は、次のことを示します

$$
\Gamma(x) = \lim_{n \to \infty} \frac{n^x (n-1)!}{x(x+1)\ldots(x+n-1)}
$$

よってガウスの公式は、$n$ が $+\infty$ になる傾向があるのと同様に、$\frac{n}{x+n}$ が 1 になる傾向があるためです。書くこともできます

$$
\log \frac{n}{n-1} = \frac{1}{n-1} + \left( \log \frac{n}{n-1} - \frac{1}{n-1} \right).
$$

したがって (提案 1 の記法で)

$$
\exp(u_n(x)) = e^{(\log \frac{n}{n-1} - \frac{1}{n-1})} \frac{e^{x/(n-1)}}{1 + \frac{x}{n-1}}
$$

そして、系列と一般的な項 $\log \frac{n}{n-1} - \frac{1}{n-1}$ は絶対収束し、和 $-\gamma$ を持ちます。ここで、$\gamma$ はオイラー定数 (V、p. 242) を表し、よってはワイエルシュトラスの公式を取得します。

$|x| \leq a$ では、一度 $|1/(x+n)^k| \leq 1/(n-a)^k$ が $n > a$ になるため、公式 (11) の右辺の系列は、含む整数 $\leq 0$ ではなく、$\mathbf{R}$ のすべてのコンパクト区間に絶対的かつ一様に収束します。どれか整数 $k \geq 2$; $|x| \leq a$ と $n > a$ の $\left| \frac{1}{n} - \frac{1}{x+n} \right| \leq \frac{a}{n(n-a)}$ なので、同じ議論が (10) の右辺にも当てはまります。この系列は系列を微分して得られるので、

$$
\log \Gamma(x) = -\gamma x - \log x + \sum_{n=1}^{\infty} \left( \frac{x}{n} - \log \left( 1 + \frac{x}{n} \right) \right)
$$

項ごとに、これはすべての $x > 0$、系列で一般的な項 $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ は [0, +∞[ に含まれるすべてのコンパクト区間で絶対的かつ一様に収束し、1 つは VII の関係 (10) と (11) を持ちます。 p. 308、すべての x > 0 (II、p. 52、th. 1)。さらに、すべての x ∈ $\mathbf{R}$ について、n が十分に大きくなると、式 $\frac{x}{n} - \log \left( 1 + \frac{x}{n} \right)$ が定義されます。 II、p. 52 の 1 は、(9) の右辺の無限積 (VII、p. 307) がすべてのコンパクト区間含むいいえ整数 $\leq 0$ に絶対的かつ一様に収束することを示しています。

$x > 0$ に対して定義された写像 $\Gamma(x)$ は、整数 $\leq 0$ とは異なる点の集合全体に拡張でき、これに基づいて VII、p. 307 の満たす式 (7) が成り立ちます。 集合: $-(n+1) < x < -n$ については、次のようにするだけで十分です
$$
\Gamma(x) = \frac{1}{x(x+1)\ldots(x+n)} \Gamma(x+n+1).
$$
プロップにより。 VII、p. 307の2、VII、p. 307、308の式(8)、(9)、(10)、(11)、(11)の$D^k(\log |\Gamma(x)|)$ 置き換えること $D^k(\log \Gamma(x))$は、この集合でも有効です。 Formula (9) (VII, p. 307) shows that $\Gamma(x) \sim 1/x$ as x tends to 0, whence, by (7) of VII, p. 307,
$$
\Gamma(x) \sim \frac{(-1)^n}{n! (x+n)}
$$
as x tends to $-n$ ($n$ an integer $\geq 0$). 写像 $1/\Gamma(x)$ は、$\mathbf{R}$ のすべてへの連続性によって拡張でき、整数 $\leq 0$ で値 0 を割り当てます。それでは、皆さん $x \in \mathbf{R}$
$$
\frac{1}{\Gamma(x)} = \lim_{n \to \infty} \frac{x(x+1)\ldots(x+n)}{n^n n!}
$$
そして
$$
\frac{1}{\Gamma(x)} = e^{y_1 x} x \prod_{n=1}^{\infty} \left( 1 + \frac{x}{n} \right) e^{-y_1/n}
$$
そして 1 つは prop のように表示されます。 VII、p. 307の2、(13)の右側の無限積が$\mathbf{R}$のすべてのコンパクト区間に絶対的かつ一様に収束すること。

Since $\Gamma(x) > 0$ for $x > 0$, equation (7) of VII, p. 307, shows that $\Gamma(x) < 0$ for $-(2n-1) < x < -(2n-2)$ and $\Gamma(x) > 0$ for
$$
-2n < x < -(2n-1)
$$
($n$ an integer $\geq 1$); also $\Gamma(x)$ has right limit $+\infty$ at the points $-2n$ and $-\infty$ at the points $-(2n+1)$, and has left limit $-\infty$ at the points $-2n$ and $+\infty$ at the points $-(2n+1)$ (for all $n \in \mathbf{N}$). VII、p. 308 の公式 (11) は、$k = 2$ の定義時に右辺が常に $\geq 0$ であることを示しています。
$$
\Gamma''(x) \Gamma(x) - (\Gamma'(x))^2 \geq 0,
$$

and consequently $\Gamma''(x)$ has the same sign as $\Gamma(x)$; thus $\Gamma$ is *convex* for $x > 0$ and for $-(2n+2) < x < -(2n+1)$, and *concave* for $-(2n+1) < x - 2n \ (n \in \mathbf{N})$; one deduces from this that, on the intervals where $\Gamma$ is convex, $\Gamma'(x)$ increases from $-\infty$ to $+\infty$, and on the intervals where $\Gamma$ is concave, $\Gamma'(x)$ decreases from $+\infty$ to $-\infty$. よって $\Gamma$ のグラフ (図 1)。

**イチジク。 1**

### 3. オイラー積分

簡潔にするために、区間 $I \subset \mathbf{R}$ で定義された写像 $f$ と、この区間で定義された $> 0$ は、$\log f$ が $I$ に凸である場合、$I$ に *対数的に凸* であると言います。 $\Gamma(x)$の定義は、この写像が$]0, +\infty[$に対数的に凸であることを示しています。

$I$ 上で対数的に凸な 2 つの写像の *積* は、$I$ 上でも対数的に凸であることは明らかです。さらに遠く：

#### 補題 1 {#fvr-vii-s1-lem-1 .statement tag=08J0}

*$f$ と $g$ を 2 つの写像 $> 0$ とし、開区間 $I$ で 2 回微分可能とします。 $f$ と $g$ が $I$ に対数的に凸写像である場合、$f + g$ は $I$ に対数的に凸です。*

関係 $D^2 (\log f(x)) \geq 0$ は $f(x)f''(x) - (f'(x))^2 \geq 0$ と書くことができます。私たちは、関係 $a > 0, a' > 0, ac - b^2 \geq 0, a'c' - {b'}^2 \geq 0$ が $(a + a')(c + c') - (b + b')^2 \geq 0$ を暗示していることを示すことに帰着します。さて、$a > 0$、関係 $ac - b^2 \geq 0$ は、二次方程式形 $ax^2 + 2bxy + cy^2$ が $\mathbf{R}^2$ 上で $\geq 0$ であるという事実と同等であり、次のことが明らかです。

$$
ax^2 + 2bxy + cy^2 \geq 0 \quad \text{and} \quad a'x^2 + 2b'xy + c'y^2 \geq 0
$$

$\mathbf{R}^2$ では、$\mathbf{R}^2$ では $(a + a')x^2 + 2(b + b')xy + (c + c')y^2 \geq 0$ も発生します。

#### 補題 2 {#fvr-vii-s1-lem-2 .statement tag=08J1}

$f$ を有限実数写像、$> 0$ とし、2 つの積 $I \times J$ と $\mathbf{R}$ の区間で定義され連続し、すべての $t \in J$ 写像 $x \mapsto f(x, t)$ が対数的に凸で 2 倍になるようにします。 $I$ で微分可能です。 これらの仮説の下では、整 $g(x) = \int_J f(x, t) dt$ が $x \in I$ ごとに収束すると、$g$ は$I$ に対数的に凸になります。

まず、すべてのコンパクト区間 $K \subset J$ 写像 $g_K(x) = \int_K f(x, t) dt$ が対数的に凸であることを示します。確かに、写像の $K = [a, b]$、数列の場合

$$
g_n(x) = \frac{b-a}{n} \sum_{k=0}^{n-1} f\left(x, a + k \frac{b-a}{n}\right)
$$

$I$ (II、p. 57、提案 5) 上の $g_K(x)$ に単純に収束するため、$\log g_n$ は単純に $\log g_K$ に収束します。 by 補題 VII, p. 310, $\log g_n$ の 1 は$I$ に凸なので、(I, p. 27, 提案 4) $\log g_K$ についても同様です。

一方、$g$ は、$I$ (II、p. 64) のコンパクトな部分区間の有向集合に沿った $g_K$ の点単位の極限であるため、$\log g$ は $\log g_K$ の点単位の極限です。これらの最後の写像は $I$ に凸であり、$\log g$ も同様です (I、p. 27、提案 4)。

写像が 2 回微分可能であると仮定しない場合でも、補題 1 と 2 が依然として有効であることを簡単に示すことができます (VII、p. 327、演習 5)。

#### 補題 3 {#fvr-vii-s1-lem-3 .statement tag=08J2}

$\varphi$ を、$[0, +\infty[$ に含まれる開いた区間 $J$ 上の連続する写像と $> 0$ とします。 $I$ が開区間で、整 $g(x) = \int_J t^{x-1} \varphi(t) dt$ がすべての $x \in I$ に対して収束する場合、$g$ は$I$ に対数的に凸になります。

確かに、$\log t^{x-1} = (x-1) \log t$ は $x$ の写像であり、凸であり、すべての $t > 0$ に対して 2 回微分可能であるため、補題 2 が当てはまります。

#### 命題 3 {#fvr-vii-s1-prop-3 .statement tag=08J3}

皆様へ $x > 0$

$$
\Gamma(x) = \int_0^\infty e^{-t} t^{x-1} dt
$$

(2 番目のオイラー積分)。

Now the function $g(x) = \int_0^\infty e^{-t} t^{x-1} dt$ is defined for all $x > 0$ (V, p. 229); lemma 3 of VII, p. 311, then shows that it is *logarithmically convex* on ]$0, +\infty[$. さらに、部分で積分すると、

$$
g(x+1) = \int_0^\infty e^{-t} t^x \, dt = -e^{-t} t^x \Big|_0^\infty + x \int_0^\infty e^{-t} t^{x-1} dt = x \, g(x).
$$

その他の語、$g$は、VII、p. 305の式(1)の解です。最後に、

$$
g(1) = \int_0^\infty e^{-t} \, dt = 1;
$$

したがって、命題は prop から続きます。 VII、p. 306の1。

変数 $e^{-t} = u$ の変更により、(14) (VII, p. 311) 公式から推定されます。

$$
\Gamma(x) = \int_0^1 \left( \log \frac{1}{t} \right)^{x-1} dt.
$$

同様に、変数$u = t^{1/x}$の変更から、

$$
x \, \Gamma(x) = \int_0^\infty e^{-t^{1/x}} \, dt
$$

もう一度、(7) (VII, p. 3) を考慮すると、

$$
\Gamma \left( 1 + \frac{1}{x} \right) = \int_0^\infty e^{-t^x} \, dt
$$

特に$x = 2$については

$$
\Gamma \left( \frac{3}{2} \right) = \frac{1}{2} \Gamma \left( \frac{1}{2} \right) = \int_0^\infty e^{-t^2} \, dt.
$$

#### 命題 4 {#fvr-vii-s1-prop-4 .statement tag=08J4}

*$x > 0$ と $y > 0$ の積分*

$$
\mathbf{B}(x, y) = \int_0^1 t^{x-1} (1-y)^{y-1} \, dt
$$

(*第一オイラー積分*) *は値*

$$
\mathbf{B}(x, y) = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$

実際、この積分は $x > 0$ と $y > 0$ (V, p. 229) について収束します。 補題により、I、p. 311、写像の 3 $x \mapsto \mathbf{B}(x, y)$ は、$x > 0$ に対して *対数的に凸* になります。さらに、

$$
\mathbf{B}(x+1, y) = \int_0^1 (1-t)^{x+y-1} \left( \frac{t}{1-t} \right)^x \, dt
$$

したがって、部分で積分すると、

$$
\mathbf{B}(x+1, y) = -\frac{(1-t)^{x+y}}{x+y} \left( \frac{t}{1-t} \right)^x \Bigg|_0^1
+ \frac{x}{x+y} \int_0^1 (1-t)^{x+y} \left( \frac{t}{1-t} \right)^{x-1} \frac{dt}{(1-t)^2} = \frac{x}{x+y} \mathbf{B}(x, y).
$$

したがって、$f(x) = \mathbf{B}(x, y) \Gamma(x+y)$ は VII、p. 305 の恒等式 (1) を満たすことがわかります。
さらに、この写像は対数的に凸であり、2つの対数的に凸な写像の積です。最後に、$f(1) = \mathbf{B}(1, y) \Gamma(y+1)$、$\mathbf{B}(1, y) = \int_0^1 (1-t)^{y-1} dt = 1/y$、よって $f(1) = \frac{1}{y} \Gamma(y+1) = \Gamma(y)$ があります。したがって、写像 $f(x)/\Gamma(y)$ は、プロップにより $\Gamma(x)$ と等しくなります。 VII、p. 306 の 1、これは (18) を証明します。

変数$t = \frac{u}{u+1}$ 公式の変更により (18) となります。

$$
\int_0^\infty \frac{t^{x-1}}{(1+t)^{x+y}} dt = \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}
$$
(19)

変数 $t = \sin^2 \varphi$ の変更による

$$
\int_0^{\pi/2} \sin^{2x-1} \varphi \cos^{2y-1} \varphi d\varphi = \frac{1}{2} \frac{\Gamma(x) \Gamma(y)}{\Gamma(x+y)}.
$$
(20)

この最後の公式に$x = y = \frac{1}{2}$を入れると、次のようになります。

$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$
(21)

よって、(17) により、

$$
\int_0^\infty e^{-t^2} dt = \frac{1}{2} \sqrt{\pi}.
$$
(22)

VII, p. 307 の関係 (7) から、漸近展開が起こります。

$$
\begin{align*}
\Gamma(x) &= \frac{1}{x} \Gamma(x+1) \\
&= \frac{1}{x} + \Gamma'(1) + \frac{1}{2!} \Gamma''(1)x + \cdots + \frac{1}{n!} \Gamma^{(n)}(1)x^{n-1} + O(x^n)
\end{align*}
$$
(23)

$\Gamma(x)$、0 の近傍の場合。

同様に、すべての $y$ 固定と $> 0$ について、次のように書くことができます。

$$
\begin{align*}
\frac{1}{\Gamma(x+y)} &= \frac{1}{\Gamma(y)} + D \left( \frac{1}{\Gamma(y)} \right) x \\
&\quad + \frac{1}{2!} D^2 \left( \frac{1}{\Gamma(y)} \right) x^2 + \cdots + \frac{1}{n!} D^n \left( \frac{1}{\Gamma(y)} \right) x^n + O_1(x^{n+1})
\end{align*}
$$

そして、公式 (18) は、$y$ 固定に対して、漸近展開を与えます。

$$
\mathbf{B}(x, y) = \frac{1}{x} + \left( \Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} \right)
+ \left( \frac{\Gamma''(1)}{2} - \Gamma'(1) \frac{\Gamma'(y)}{\Gamma(y)} + \frac{2{\Gamma'}^2(y) - \Gamma(y)\Gamma''(y)}{2\Gamma^2(y)} \right) x + O(x^2)
$$
$x = 0$の近傍に。

さらに、$x > 0$ と $y > 0$ については、
$$
\mathbf{B}(x, y) = \int_0^1 \left( t^{x-1} + t^x \frac{(1-t)^{y-1} - 1}{t} \right) dt
= \frac{1}{x} + \int_0^1 t^x \frac{(1-t)^{y-1} - 1}{t} dt.
$$
写像 $\varphi(t) = \frac{(1-t)^{y-1} - 1}{t}$ はコンパクト区間 $[0, 1]$ で連続します。それ以来
$$
t^x = e^{x \log t} = 1 + x \log t + \frac{x^2}{2!} (\log t)^2 + \cdots + \frac{x^n}{n!} (\log t)^n + r_n(x, t)
$$
$|r_n(x, t)| \leq \frac{x^{n+1}}{(n+1)!} |\log t|^{n+1}$ ($\log t \leq 0$ と $x > 0$ なので)、公式 (25) は漸近展開を与えます。
$$
\mathbf{B}(x, y) = \frac{1}{x} + \int_0^1 \varphi(t) dt + x \int_0^1 \varphi(t) \log t \, dt + \cdots
+ \frac{x^n}{n!} \int_0^1 \varphi(t) (\log t)^n \, dt + O_2(x^{n+1})
$$
0 の近傍で $\mathbf{B}(x, y)$ の場合。

$n = 1$ の場合、この展開を (24) で特定すると、特に次のことが得られます。
$$
\Gamma'(1) - \frac{\Gamma'(y)}{\Gamma(y)} = \int_0^1 \frac{(1-t)^{y-1} - 1}{t} dt.
$$

さらに、公式 (10) は $\Gamma'(1) = \Gamma'(1)/\Gamma(1) = -\gamma$ となるので、(*ガウスの積分*)
$$
\frac{\Gamma'(x)}{\Gamma(x)} + \gamma = \int_0^1 \frac{1 - (1-t)^{x-1}}{t} dt.
$$

### 練習問題 {#fvr-vii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
