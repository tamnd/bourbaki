---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 0
section_title: Hardy Fields. (H) Functions
appendix: true
lang: ja
source: fvr-i-vii
book_pages: 247-258, 263-267
pdf_pages: 0262-0273, 0278-0282
extraction: ocr
subsections:
    - "no": 1
      title: HARDY FIELDS
      page: 247
      pdf_page: 262
    - "no": 2
      title: EXTENSION OF A HARDY FIELD
      page: 248
      pdf_page: 263
    - "no": 3
      title: COMPARISON OF FUNCTIONS IN A HARDY FIELD
      page: 250
      pdf_page: 265
    - "no": 4
      title: (H) FUNCTIONS
      page: 252
      pdf_page: 267
    - "no": 5
      title: EXPONENTIALS AND ITERATED LOGARITHMS
      page: 253
      pdf_page: 268
    - "no": 6
      title: INVERSE FUNCTION OF AN (H) FUNCTION
      page: 255
      pdf_page: 270
statements: 21
exercises: 15
content_sha256: d5732e0cfa190aebd7aa74aa48a20aa365ccd49ce5d56cfef0851bfa125fdf81
translated_from: content/en/fvr/V/A_a_hardy_fields_h_functions.md
translation_method: google
source_content_sha256: 90e02e3632c6ecc96144815961457f749d0c9a6edf475780ab90b36dc9feca0f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 04d6af1eba93fb780feff008252c4a4653ab142f0cadd2754522e8da5e5c1b48
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録

# ハーディ体。 (ひ) 写像

### 1. ハーディ体

$\mathfrak{F}$ を、形 $[x_0, +\infty[$ の区間によって形成される $\mathbf{R}$ のフィルター 基底とします。 同値関係 $R_\infty$ を定義したことを思い出してください: 集合所属から $\mathfrak{F}$ に定義された実数写像の集合 $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 上に、$f(x) = g(x)$ が成り立つような集合 $M \in \mathfrak{F}$ が存在します。 $M$” (V、p. 211)、そしてその商集合 $\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$ には、単位元を持つ *環* の構造が与えられます。

#### 定義 1 {#fvr-v-a0-def-1 .statement tag=08GO}

*$\mathscr{H}(\mathfrak{F}, \mathbf{R})$の部分集合$\mathfrak{K}$が与えられた場合、$\mathfrak{K}$が次の条件を満たす場合、$\mathfrak{K}/R_\infty$（$\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$の$\mathfrak{K}$の標準像）はハーディ体であると言えます。

1. $\mathfrak{K}/R_\infty$ は環 $\mathscr{H}(\mathfrak{F}, \mathbf{R})/R_\infty$ の部分体です。
2. *$\mathfrak{K}$ のすべての写像は連続であり、区間 $[a, +\infty[$ (写像に応じて)、および類の導関数属するから $\mathfrak{K}/R_\infty$ の $R_\infty$ に関して微分可能です。

$\mathfrak{K}/R_\infty$ が *フィールド* であるという仮説は、次の条件と同等です。 $f \in \mathfrak{K}$ と $g \in \mathfrak{K}$ の場合、$f + g$ と $fg$ は、$\mathfrak{F}$ の集合に対する $\mathfrak{K}$ の関数に等しい。さらに、$\mathfrak{F}$ の集合で$f$ が全く同じゼロではない場合、$\mathfrak{F}$ には$f$ *消滅せず*、$1/f$ は$M$ 上の$\mathfrak{K}$ からの関数に等しい集合$M$ が存在します。条件 2' により、$M$ が取られ、$f$ が $M$ で *連続* となり、その結果、この区間で *定数符号を持つ* と常に仮定できます。

言葉の乱用により、$\mathfrak{K}$ が $\mathfrak{K}/R_\infty$ が Hardy 体であるようなものである場合、以下では $\mathfrak{K}$ 自体が *Hardy 体* であると言うでしょう。

#### 例 1 {#fvr-v-a0-n1-exa-1 .statement tag=08GP}

*有理定数* のすべてのハーディ体含む体 (特性 0 の最小の体、*cf. Alg.*、V, §1)、そのうち同一視できると体 $\mathbf{Q}$;さらに、2 つの定数できないは $R_\infty$ 〜でない限りを法として合同であるため、それらは等しいので、$\mathbf{Q}/R_\infty$ は $\mathbf{Q}$ と同一です。 *実際の定数* も形とハーディ体で、これは同一視できると $\mathbf{R}$ です。

#### 例 2 {#fvr-v-a0-n1-exa-2 .statement tag=08GQ}

ハーディ体の非常に重要な例は、有理数写像と実数係数* の *集合であり、言葉の乱用により、$\mathbf{R}(x)$ で表します。 $f(x) = p(x)/q(x)$ が実数係数を持つ有理数写像であり、同一の零ではない場合、それは連続で微分可能であり、区間 $[a, +\infty[$ 上で $\neq 0$ になります。ここで、$a$ は厳密に実数根の最大のより大きくなります。多項式 $p(x)$ と $q(x)$;従って、0 以外の $\mathbf{R}(x)/R_\infty$ のすべての元は反転可能です。 2 つの有理数写像できないは $\mathbf{R}_\infty$ 〜でない限りを法として合同であり、等しいので、$\mathbf{R}(x)/\mathbf{R}_\infty$ は再び $\mathbf{R}(x)$ と同一視できることに再度注意します。

### 2. 丈夫な拡大体

Hardy 体 $\mathfrak{K}$ が与えられた場合、*隣接* (項、*cf. Alg.*、V の代数的な意味で) によって $\mathfrak{K}'/\mathbf{R}_\infty$ が得られるように、新しい Hardy 体 $\mathfrak{K}' \supset \mathfrak{K}$ をどのように形作成できるかを見てみましょう。 §2) 形のうちの新しい元を、正確には $\mathfrak{K}/\mathbf{R}_\infty$ にします。

#### 補題 1 {#fvr-v-a0-lem-1 .statement tag=08GR}

*$a(x), b(x)$ *を、区間* $[x_0, +\infty[$に変更が符号しない2つの連続する実数写像とします。 *この区間、写像* $y(x)$ が連続かつ微分可能であり、恒等式を満たす場合*

$$
y' = ay + b
$$

(1)

*その場合、区間* $[x_1, +\infty[$ *その上* $y$ *変更は符号しません*。

確かに、$z(x) = y(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$ (*cf. IV*, p. 183) と入れてみましょう。次に、(1) により、$z'(x) = b(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$ となります。 $x \geqslant x_0$ に対して $b(x) \geqslant 0$ の場合、$z$ はこの区間の増加するであるため、このすべての区間では $< 0$ であるか、区間 $[x_1, +\infty[$ では零であるか、そうでない場合は $> 0$ であることになります。 区間 $[x_1, +\infty[$; $y$ は $z$ と同じ符号なので、この場合命題が証明されます。 $x \geqslant x_0$ に対して $b(x) \leqslant 0$ の場合も同様の議論になります。

#### 注意 {#fvr-v-a0-n2-rem-1 .statement tag=08GS}

この非常に初歩的な性質は、 位数 $> 1$ の線形微分方程式に拡大する対応しません。たとえば、写像 $y = \sin x$ は $y'' + y = 0$ を満たしますが、変更は $+\infty$ のすべての近傍に署名します。

#### 補題 2 {#fvr-v-a0-lem-2 .statement tag=08GT}

*$a(x)$ *と* $b(x)$ *を、特定のハーディ体* 写像所属の 2 つにします $\mathfrak{K}$ *と* $y(x)$ *写像満たすをアイデンティティ* (1) *区間* $[x_0, +\infty[$ *ここで* $a$ *および* $b$ *は定義されており、連続しています*。 *もし* $p(u)$ * が* $u$ の多項式であり、その係数が* $x$ * 所属から* $\mathfrak{K}$ の写像である場合、 * $[x_0, +\infty[$ で * 定義され微分可能* である場合、 * 区間が存在します* $[x_1, +\infty[$ *その上で写像* $p(y)$ *は変更に署名しません*。

$p(u)$ に $[x_0, +\infty[$ で同じ零である係数がある場合、または $u$ で $p(u)$ が次数 0 である場合、$\mathfrak{K}$ の写像は定数符号オンであるため、命題は自明です。 区間 $[x_1, +\infty[$。 $p(u)$ が次数 $n > 0$ であると仮定します。 $p(u)$ の先頭の係数 $c$ は、区間 $[\alpha, +\infty[$ では $\neq 0$ になります。したがって、$p(u) = c(u^n + c_1 u^{n-1} + \cdots + c_n)$ と書くことができます。ここで、$c, c_1, c_2, \ldots, c_n$ は *写像* 所属から $\mathfrak{K}$ であり、$[\alpha, +\infty[$ で微分可能です。したがって、$c = 1$ に対して補題を証明するだけで十分です。私たちは$n$の帰納法までに議論します。 1つは持っています

$$
\frac{d}{dx} (p(y)) = (ay + b)(ny^{n-1} + (n-1)c_1 y^{n-2} + \cdots + c_{n-1})
$$
$$
+ c'_1 y^{n-1} + \cdots + c'_n = na\ p(y) + q(y)
$$

ここで、$q(u)$ は $\mathfrak{K}$ に係数を含む、次数 $\leq n - 1$ の多項式です。 仮定写像 $na(x)$ と $q(y(x))$ は、変更区間 $[ \beta, +\infty[$ に署名しません。したがって、補題は補題 1 の帰結です。

#### 定理 1 {#fvr-v-a0-thm-1 .statement tag=08GU}

*$a(x)$と$b(x)$を、区間$[ x_0, +\infty[$の特定のハーディ体$\mathfrak{K}$と$y(x)$写像満たす(1)に対する2つの写像所属とします。 $r(u) = p(u)/q(u)$ が $u$ の有理分数の集合と $\mathfrak{K}$ の係数を通過するとき、$q(y)$ は $+\infty$ 集合の近傍上の零と同一ではありません。 写像 $r(y)$ 形体の$\mathfrak{K}(y)$。*

確かに、補題 2 までに、$r(y)$ が定義され、連続であり、変更符号を持たない区間 $[ x_1, +\infty[$ が存在し、そこからすぐに$\mathfrak{K}(y)/\mathbf{R}_\infty$ が体であることがわかります。さらに、以来

$$
\frac{d}{dx}(r(y)) = r'(y)y' = r'(y)(ay + b)
$$

(ここで、$r'(y) = (p'(y)q(y) - p(y)q'(y))/(q(y))^2$ は $+\infty$ の近傍の仮定によって定義されます)、$\mathfrak{K}(y)$ 属するから $\mathfrak{K}(y)$ までのすべての写像の導関数であり、$\mathfrak{K}(y)$ が以下の条件を満たすことを証明します。間違いない。 V、p. 247 の 1 つ。

$\mathfrak{K}(y)/\mathbf{R}_\infty$ が、$y$ モジュロ $\mathbf{R}_\infty$ の類の $\mathfrak{K}/\mathbf{R}_\infty$ への代数 *随伴* によって得られることは明らかです。ここでも、$\mathfrak{K}(y)$ は $y$ を $\mathfrak{K}$ に*隣接させることによって得られると言われています。

#### 系 1 {#fvr-v-a0-thm-1-cor-1 .statement tag=08GV}

*$y$が$+\infty$の近傍の零ではなく、$\mathfrak{K}$の写像である場合、$\mathfrak{K}(\log|y|)$はハーディ体です。

確かに、$(\log|y|)' = y'/y$ は、区間 $[ x_0, +\infty[$ の $\mathfrak{K}$ の写像に等しいです。

系 2 *$y$ が $\mathfrak{K}$ のいずれかの写像である場合、$\mathfrak{K}(e^y)$ はハーディ体です。*

確かに、$(e^y)' = e^y y'$、および$y'$は、区間 $[ x_0, +\infty[$の$\mathfrak{K}$の写像に等しい。

系 3 *実定数が $\mathfrak{K}$ 含むで、$y$ が $\mathfrak{K}$ の写像であり、$+\infty$ の近傍の零ではない場合、$\mathfrak{K}(|y|^{\alpha})$ は次のようになります。 実数 $\alpha$ ごとに、丈夫な体。*

確かに、$\frac{d}{dx}(|y|^{\alpha}) = |y|^{\alpha} (\alpha y'/y)$、$\alpha y'/y$ は、区間 $[ x_0, +\infty[$ の $\mathfrak{K}$ の写像に等しいです。

最後に、$y$ が $\mathfrak{K}$ の任意の写像の *プリミティブ* である場合、$\mathfrak{K}(y)$ は再び Hardy 体であることに注意します。

### 3. 丈夫な体と写像の比較

#### 命題 1 {#fvr-v-a0-prop-1 .statement tag=08GW}

*同じハーディ体内の 2 つの写像は、どの位数* (V、p. 232) にも匹敵します。

確かに、$f$ 属するをハーディ体 $\mathscr{K}$ にすると、整数 $n > 0$ ごとに区間 $[x_0, +\infty[$ が存在し、$f$ は$n$ 回微分可能であり、その$n^{th}$ 導関数は等しい。この区間の$\mathscr{K}$の写像まで。したがって、$\mathscr{K}$ の任意の 2 つの写像 $f, g$ が *比較可能* であることを示すだけで十分です。これは、写像の 1 つが $+\infty$ の近傍の零と同じである場合に明らかです。したがって、両方とも$+\infty$の近傍が厳密に陽性である場合に限定することができます。しかし、その後、すべての実数 $t$ に対して、$f - tg$ は $+\infty$ の近傍上の $\mathscr{K}$ の写像に等しいため、$+\infty$ の近傍に定数符号があり、命題が証明されます。 (V、p. 217、提案9)。

この命題から、ハーディ体 $\mathscr{K}$ 含むが実定数 (以下で常に仮定するように) である場合、および $f$ と $g$ が $\mathscr{K}$ のいずれか 2 つの写像である場合、次のいずれか 2 つが推測されます。 写像 $e^f, e^g, \log |f|, \log |g|, |f|^{\alpha}, |g|^{\alpha}$ ($\alpha$ は任意の実数)、$\int_a f, \int_a g$ ($a$ は区間 $[x_0, +\infty[$ のいずれかの実数であり、$f$ と $g$ は規定されている) は *比較可能* (それらが存在する場合)定義済み);実際、これら写像属するのいずれか 2 つを、$\mathscr{K}$ に連続して隣接することによって得られる、特定の Hardy 体に変換します。

同様に、ハーディ体 $\mathscr{K}$ のすべての写像 $f(x)$ は、$x$ と $f(x)$ 属するから、隣接する$x$ によって得られるハーディ体から、$x$ と同等です。 $\mathscr{K}$まで。したがって、結論する (特に) $f$ は、すべての位数からすべての冪 $x^{\alpha}$、さらには $\log x$ および $e^x$ と同等です。

また、$f$ と $g$ 属するが同じハーディ体 $\mathscr{K}$ にある場合、$g(x) > 0$ が区間 $[x_0, +\infty[$ にある場合、$g(x)$ が 0 または$x$ が $+\infty$ になる傾向があるため、$+\infty$ であれば、$g$ (V, p. 219) に対する$f$ の *位数* が常に定義されます。

したがって、V、p. 233 の提案 8 は、ハーディ体のすべての写像 $f$ に適用でき、次のことを証明します。

1) $f$ が $x$ に対して位数 $+\infty$ である場合、$\int_a^x f(t)\,dt \sim (f(x))^2/f'(x)$。

2) $f$ が $x$ に対して位数 $\mu > -1$ である場合、$\int_a^x f(t)\,dt \sim \frac{1}{\mu+1} x f(x)$。

3) $f$ が $x$ に対して位数 $\mu < -1$ である場合、$\int_a^{+\infty} f(t)\,dt \sim -\frac{1}{\mu+1} x f(x)$。

4) $f$ が $x$ に対して位数 $-\infty$ である場合、$\int_a^{+\infty} f(t)\,dt \sim -(f(x))^2/f'(x)$。

さらに、次の命題があります。

#### 命題 2 {#fvr-v-a0-prop-2 .statement tag=08GX}

$f$ をハーディ体 $\mathscr{K}$ に対して写像所属とします。

1 $f$ が $x$ に対して無限大位数である場合、整数 $n > 0$ ごとに、
$$
f^{(n)}(x) \sim \frac{(f'(x))^n}{(f(x))^{n-1}}.
$$
(2)

2° $f$ が $x$ に対して有限位数 $\mu$ である場合、$n > 0$ ごとに、
$$
f^{(n)}(x) \sim \mu(\mu - 1) \ldots (\mu - n + 1) \frac{f(x)}{x^n}
$$
$$
\sim \frac{(\mu - 1) \ldots (\mu - n + 1)}{\mu^{n-1}} \frac{(f'(x))^n}{(f(x))^{n-1}}
$$
(3)
ただし、$\mu$ が整数 $\geqslant 0$ および $n > \mu$ の場合は除きます。

1 $f$ が $x$ に対して無限大位数である場合、$\log |f| \gg \log x$ が存在します。したがって、$\log |f|$ と $\log x$ はいずれの位数、$f'/f \gg 1/x$ にも匹敵します。 $g = f'/f$ を入れます。 $g$ は $+\infty$ の近傍上の $\mathscr{K}$ の写像に等しいので、$1/g \ll x$ から$g'/g^2 \ll 1$ が推測され、したがって $g'/g \ll g = f'/f$、または再び $fg' \ll gf'$ になります。 関係 $f' = fg$ から微分することで次のことが推測されます。
$$
f'' = fg' + gf' \sim gf'
$$
またはもう一度$f''/f' \sim f'/f$。同じ議論を、$f$ の代わりに $f^{(n)}$ に適用すると、$n$ 上の帰納法によって、$f^{(n)}/f^{(n-1)} \sim f'/f$ が示されます。 よって関係 (2)。

2 $f$ が $x$ に対して有限位数 $\mu$ であり、$\mu \neq 0$ の場合、$\log |f| \sim \mu \log x$、よって、微分すると $f'(x) \sim \mu \frac{f(x)}{x}$ になります。 $f'$ は $x$ に対して位数 $\mu - 1$ であると推測します。これにより、$\mu$ がそうでない場合、$\mu \neq n$, よって公式 (3) である限り、$n$ に帰納法によって同じ議論を適用することができます。 整数 $\geqslant 0$ と $< n$ 。

$f$ が $x$ に対して整数位数 $p \geqslant 0$ であるとき、$f(x) = x^p f_1(x)$ と書くことができます。ここで、$f_1$ は $x$ に対して位数 0 です。プロップにより。 2 あるものは
$$
f^{(p)} \sim p! f_1.
$$
位数 $n > p$ の導関数を評価するには、$p = 0$ の場合に限定することができます。すると、一方には $\log |f| \ll \log x$、よって $f'(x)/f(x) \ll 1/x$ があり、もう一方には語 $x f'(x) \ll f(x)$ があります。 $f$ が定数 $k \neq 0$ と等価でない場合、これを微分すると関係 (V, p. 232, prop. 7) $x f''(x) + f'(x) \ll f'(x)$ となり、これは $x f''(x) \sim -f'(x)$ を意味します。この公式を考慮すると、$n$ の帰納法によって、$f^{(n)}$ は $x$ に対して位数 $\leqslant -n$ であることが分かります。
$$
f^{(n)} \sim (-1)^{n+1} (n-1)! \frac{f'(x)}{x^{n-1}}.
$$
(4)

$f$ が定数 $k \neq 0$ と同等である場合、$f_2 \ll 1$ と$f(x) = k + f_2(x)$ があり、$f_2$ の導関数を調べると簡約するになります。

### 4. (ひ) 写像

#### 命題 3 {#fvr-v-a0-prop-3 .statement tag=08GY}

*$\mathscr{K}_0$ がハーディ体である場合、ハーディ体 $\mathscr{K}$ 含む $\mathscr{K}_0$ が存在し、写像 $z \in \mathscr{K}$ ごとに、近傍で同じ零が存在するわけではありません。 $+\infty$、$e^z$ と $\log |z|$ 属するから $\mathscr{K}$ まで*。

以下の特性を持つ関数 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ の集合を $\mathscr{K}$ で示します。各関数 $f \in \mathscr{K}$ には、$f \in \mathscr{K}_n$ のような有限数のハーディ フィールド $\mathscr{K}_1, \mathscr{K}_2, \ldots, \mathscr{K}_n$ (数 $n$ と $f$ に応じたフィールド $\mathscr{K}_i$) があり、$0 \leq i \leq n-1$ については、 $\mathscr{K}_{i+1} = \mathscr{K}_i(u_{i+1})$ ここで、$u_{i+1}$ は $e^{z_i}$ または $\log |z_i|$ に等しく、$z_i$ は $\mathscr{K}_i$ に属し、$+\infty$ の近傍で同じように消えません。 ある人は、体 $\mathscr{K}_n$ と写像 $f$ の $u_1, u_2, \ldots, u_n$ 形は *定義数列* であると言います。同じ写像に複数の定義数列を自然に認めることができます。

間違いなく。 $+\infty$の近傍上の零と同じではなく、すべての写像$f \in \mathscr{K}$のV、p. 247の1は定数符号を持ち、区間$[x_0, +\infty[$で微分可能です。 $f \in \mathscr{K}_n$ の場合、$1/f$ と $f'$ は $\mathscr{K}_n$ の写像に等しいため、$+\infty$ の近傍で、$\mathscr{K}$ の写像に等しくなります。 $\mathscr{K}$ がハーディ体であることを確認するには、$f$ と $g$ が $\mathscr{K}$ の 2 つの写像である場合、$f - g$ と $fg$ が $\mathscr{K}$ の写像に等しいことを証明すれば十分です。 $+\infty$中近傍。ここで、$u_1, u_2, \ldots, u_m$ を $f$ の場合は定義数列とし、$g$ の場合は $v_1, v_2, \ldots, v_n$ 定義数列とします。 数列 $(u_i)$ と $(v_i)$ を連結して得られる数列 $u_1, u_2, \ldots, u_m, v_1, v_2, \ldots, v_n$ は、再び Hardy 体 $\mathscr{K}_{m+n}$ の定義数列とこれ体含む $f$と$g$なので、$f - g$と$fg$は、$+\infty$の近傍の$\mathscr{K}_{m+n}$の写像と等しくなります。

ある人は、Hardy 体 $\mathscr{K}$ が prop の証明で定義されていると言います。 3 はハーディ体 $\mathscr{K}_0$ の (H) *拡大* です。

$\mathscr{K}'$ が他の Hardy 体であり、プロップに記載されている特性を備えている場合。 3、$\mathscr{K}$の構成から、$\mathscr{K}/\mathbf{R}_\sim$は$\mathscr{K}'/\mathbf{R}_\sim$に*含まれる*ことがわかります。言葉の乱用により、ハーディ体 $\mathscr{K}_0$ の (H) 拡大は、これらの特性を持つ *最小の* ハーディ体 $\mathscr{K}$ であると言われます。

#### 定義 2 {#fvr-v-a0-def-2 .statement tag=08GZ}

*(H)写像の体は、実数係数を持つ有理数写像のハーディ体$\mathbf{R}(x)$の(H)拡大と呼ばれます。 写像所属からこの拡大までを (H) 写像と呼びます。*

この定義に続き、$f$が$+\infty$の近傍の零ではなく、(H)写像であれば、$e^f$と$\log |f|$も(H)写像になります。より一般的には、$g$ が 2 番目 (H) 写像で、$g$ に対して $u_1, u_2, \ldots, u_n$ 定義数列で、$f(x)$ が $x$ で $+\infty$ になる傾向がある場合、帰納法までに帰納法になることがわかります。 $n$ 写像 $u_1 \circ f, u_2 \circ f, \ldots, u_n \circ f$ と $g \circ f$ が (H) 写像であること。

### 5. 指数関数と反復対数

すでに (V, p. 229) $n \geq 1$ に対する *反復対数* $l_n(x)$ by 条件 $l_0(x) = x, l_n(x) = \log(l_{n-1}(x))$ を定義しました。同様に、定義する *反復指数* $e_n(x)$ by 条件 $e_0(x) = x, e_n(x) = \exp(e_{n-1}(x))$ の $n \geq 1$ 。 $n$ の帰納法による明らかであり、$l_n(x)$ は $x > e_{n-1}(0)$ で定義された $e_n(x)$ の逆数写像であり、$e_m(e_n(x)) = e_{m+n}(x), l_m(l_n(x)) = l_{m+n}(x)$ です。 $\mu > 0$ごとに関係$\log x \ll x^\mu \ll e^x$までに、$n \geq 1$には、

$$
l_n(x) \ll (l_{n-1}(x))^\mu \quad \text{for every } \mu > 0 \tag{5}
$$

$$
e_{n-1}(x^{1+\beta}) \ll e_n(x^{1+\delta}) \ll e_n((1-\gamma)x) \ll (e_n(x))^\mu
$$
$$
\ll e_n((1+\alpha)x) \ll e_n(x^{1+\beta}) \tag{6}
$$

すべての $\mu > 0, \alpha > 0, \beta > 0, 0 < \gamma < 1, 0 < \delta < 1$ に対して、これらの数はその他の点では任意です (*cf.* V、p. 218、提案 11)。

すでに (V, p. 229) を見てきましたが、$n \geq 1$ については、

$$
\frac{d}{dx}(l_n(x)) = \prod_{i=0}^{n-1} \frac{1}{l_i(x)}. \tag{7}
$$

$n \geq 1$も同様

$$
\frac{d}{dx}(e_n(x)) = \prod_{i=1}^n e_i(x). \tag{8}
$$

よって、プロップによる。 $\mu > 0$ ごとに V、p. 233 の 8 個

$$
\int_a^x e_n(t^\mu) \, dt \sim \frac{x}{\mu} e_n(x^\mu) \prod_{i=0}^{n-1} \frac{1}{e_i(x^\mu)} \tag{9}
$$

$$
\int_x^{+\infty} \frac{dt}{e_n(t^\mu)} \sim \frac{x}{\mu} \prod_{i=0}^n \frac{1}{e_i(x^\mu)}. \tag{10}
$$

$f$ が $f \gg 1$ のような *任意の* (H) 写像である場合、次のような 2 つの整数 $m$ と $n$ が存在することがわかります。

$$
l_m(x) \ll f(x) \ll e_n(x)
$$

(V、p. 263、演習 1 および p. 264、演習 5) 一方、*ごとに $g(x) \gg e_n(x)$ となるような定義する増加する写像 $g(x)$ (これらはもはや (H) 写像ではありません) も可能です。 $n > 0$、または $1 \ll g(x) \ll l_m(x)$ ($m > 0$ ごとに) (V、p. 265、演習 8、9、10)。

反復対数の助けを借りて、(H) 関数の *比較スケール* $\mathscr{E}$ ($x$ が $+\infty$ の傾向にある) を定義できることを示します。これは、$+\infty$ の近傍で $> 0$ であり、次の条件を満たします。

a) $\mathscr{E}$ 属するから $\mathscr{E}$ のいずれか 2 つの写像のうち積;
b) 写像 $f \in \mathscr{E}$ および実数 $\mu$ ごとに $f^\mu \in \mathscr{E}$。

c) すべての写像 $f \in \mathscr{E}$ に対して、$\log f$ は $\mathscr{E}$ の写像の有限数の線形結合です。
d) 定数 1 を除いて、すべての写像 $f \in \mathscr{E}$ について、$e^f$ は $\mathscr{E}$ の写像と同等です。

まず、形 $\prod_{m=0}^{\infty} (l_m(x))^{\alpha_m}$ の写像の集合 $\mathscr{E}_0$ を検討します。ここで、$\alpha_m$ は、添字 $m$ の有限数を除いて、実数、零です。 (5) (V, p. 253) より、これら写像形は、条件 $a), b)$ と c) を満たす *比較スケール* であることは明らかです。ここで、$n$、集合 $\mathscr{E}_n$ ($n \geqslant 1$ の場合) の再帰により、定義するは定数 1 と形 $\exp \left( \sum_{k=1}^p a_k f_k \right)$ の写像によって形成されます。ここで、$p$ は任意の整数 $> 0$、写像 $f_k$ ($1 \leqslant k \leqslant p$) は、$\mathscr{E}_{n-1}$ では写像となり、$f_1 \gg f_2 \gg \cdots \gg f_p \gg 1$、$a_k$ は実数 $\neq 0$ になります。 帰納法によって、$\mathscr{E}_n$ が *比較スケール* 満たす $a), b)$ であること、および c) および含む $\mathscr{E}_{n-1}$ であることがわかります。まず、関係 $\mathscr{E}_{n-1} \subset \mathscr{E}_n$ は $n = 1$ に対して成り立ちます。$\mathscr{E}_0$ の非定数写像の対数は形 $\sum_{k=1}^p a_k f_k$ であり、$f_k$ は反復対数であるため、 $\gg 1$;一方、$\mathscr{E}_{n-2} \subset \mathscr{E}_{n-1}$ の場合、$\mathscr{E}_n$ の定義から $\mathscr{E}_{n-1} \subset \mathscr{E}_n$ が推測されます。この定義は、$\mathscr{E}_n$ が $a), b)$ と c) を満たすことを示しています。 $\mathscr{E}_n$ が比較スケールであることを確認する必要があります。$\mathscr{E}_n$ の 2 つの写像の商が再び属するから $\mathscr{E}_n$ になるため、定数 1 を除いて、$\mathscr{E}_n$ のすべての写像 $f$ が、 できないは定数 $\neq 0$ と同等です。現在、構成までに$\log f = \sum_{k=1}^p a_k f_k \sim a_1 f_1$があり、$f_1 \gg 1$以降、$\log f$は$\pm \infty$になる傾向があるため、$x$が$+\infty$になる傾向があるため、$f$は0または$+\infty$になる傾向があります。

したがって、$\mathscr{E}$ が $n \geqslant 0$ の $\mathscr{E}_n$ の *和集合* である場合、$\mathscr{E}$ は、$\mathscr{E}$ 属するの 2 つの写像を同じスケール $\mathscr{E}_n$ と比較するスケールです。同様の理由で、$\mathscr{E}$ は a) を満たし、b) および c) も満たすことは明らかです。最後に、$f \in \mathscr{E}$ の場合、$f \in \mathscr{E}_n$ となるような $n$ が存在します。 $f$ が定数 1 ではない場合、$x$ が $+\infty$ になる傾向があるのと同様に、$f(x)$ は 0 または $+\infty$ になる傾向があります。最初の場合は$e^f \sim 1$、2番目の場合は、$e^f$ 属するから定義までに$\mathscr{E}_{n+1}$、そして$\mathscr{E}$になります。

#### 注意 {#fvr-v-a0-n5-rem-1 .statement tag=08H0}

先ほど定義したスケール $\mathscr{E}$ の実際的な有用性にもかかわらず、$\mathscr{E}$ に関して*主部分* を持たない (H) 写像の例を与えるのは簡単です。実際、$f$ が $f \sim a g$ のような (H) 写像であり、$a$ が定数 $> 0$ と $g \in \mathscr{E}$ である場合、$\log f - \log g - \log a$ は $1/x$ では 0 になる傾向があるため、$\log f$ は、$\mathscr{E}$ と比較して、 性質までに *剰余が 0* になる傾向がある漸近展開 c)。さて、例えば (H) 写像 $f(x) = e_2 \left( x + \frac{1}{x} \right)$ を考えると、$\log f(x) = \exp \left( x + \frac{1}{x} \right)$ があるため、$\mathscr{E}$ に対する $\log f$ の漸近展開は形になります。

$$
\log f(x) = e^x + \frac{e^x}{x} + \frac{1}{2!} \frac{e^x}{x^2} + \cdots + \frac{1}{n!} \frac{e^x}{x^n} + o \left( \frac{e^x}{x^n} \right) \quad (n \text{ an integer } > 0).
$$

この展開の剰余は $\frac{1}{(n+1)!} \frac{e^x}{x^{n+1}}$ に等しいため、0 になる傾向がないことは明らかです。したがって、$f$ は $\mathscr{E}$ に対して主部分を持ちません。

### 6. (H) 写像の逆写像

$f$ が (H) 関数である場合、$f$ は区間 $[x_0, +\infty[$ で単調かつ連続であるため、この区間に対する $f$ の制限の逆関数 $\varphi$ は点 $a = \lim_{x \to +\infty} f(x)$ の近傍で単調かつ連続です。しかし、$a$ が $+\infty$ (または $-\infty$、有限) に等しい場合、$\varphi(y)$ (または $\varphi(-y)$、$\varphi \left( a + \frac{1}{y} \right)$、または $\varphi \left( a - \frac{1}{y} \right)$) が一般に $+\infty$ の近傍での (H) 関数と等しくないことがわかります。 それにもかかわらず、特定の重要なケースでは、$\varphi(y)$ (それぞれ $\varphi(-y)$、$\varphi \left( a + \frac{1}{y} \right)$、$\varphi \left( a - \frac{1}{y} \right)$) に相当する (H) 関数が得られ、場合によっては、V、p. 254 で定義されたスケール $\mathscr{E}$ に対するこの関数の漸近拡張さえも得られることがわかります。

次の命題を使用します。

#### 命題 4 {#fvr-v-a0-prop-4 .statement tag=08H1}

$p$ と $q$ を、区間 $[x_0, +\infty[$ に対して厳密に正である 2 (H) 写像とします。

1° $q \ll p/p'$ の場合、1 つは $p(x + q(x)) \sim p(x)$ になります。
2° $q \ll p/p'$ と $q(x) \ll x$ の両方の場合、$p(x - q(x)) \sim p(x)$。

この命題の 2 つの部分は、$p \sim k$ (定数 $\neq 0$) であればクリアです。したがって、$p(x) \ll 1$ と仮定することもできます (そうでない場合は、議論を $1/p$ に適用します)。次に、$p'(x) \ll 1$ を推測します。

1° $p(x + q(x)) = p(x) + q(x)p'(x + \theta q(x))$ を $0 \leq \theta \leq 1$ (I、p. 14、系) と書くことができます。 $x$ が $+\infty$ になる傾向があるのと同様に、$|p'(x)|$ は 0 になる傾向があり、$+\infty$ の近傍の (H) 写像に等しいため、区間 $[x_1, +\infty[$ では減少するになります。 $x \geq x_1$、1 つは $|p'(x + \theta q(x))| \leq |p'(x)|$ です。 $qp' \ll p$ 以降、1 つは $p(x + q(x)) \sim p(x)$ になります。

2° 条件 $q(x) \ll x$ により、$x - q(x)$ は $x$ とともに $+\infty$ になる傾向があります。ここでも 1 つは $0 \leq \theta \leq 1$ で $p(x - q(x)) = p(x) - q(x)p'(x - \theta p(x))$ を持っています。 証明の最初の部分と同じ議論は、$x$ 十分大きいについては、$|p'(x - \theta q(x))| \leq |p'(x - q(x))|$ であることを示しています。 簡約するは、$x$ が $+\infty$ になる傾向があるのと同様に、$q(x) \frac{p'(x - q(x))}{p(x - q(x))}$ が 0 になる傾向があることを示しています。 命題は、$p'/p \gg 1$ が true である場合、その後 $|p'/p|$ は、$x$ に対して十分に大きい (H) 写像、増加するです。したがって、$q(x) \frac{|p'(x - q(x))|}{|p(x - q(x))|} \leq q(x) \frac{|p'(x)|}{|p(x)|}$、および$qp' \ll p$ by 仮定。 $p'/p \sim k$ ($k$ 定数 $\neq 0$) の場合も同様です。

$$
\frac{p'(x - q(x))}{p(x - q(x))} \sim \frac{p'(x)}{p(x)}
$$

$x - q(x)$ は $+\infty$ になる傾向があるため。あとは$p'/p \ll 1$の場合を検討するだけです。まず、$p(x)$ が $x$ に対して *有限* 位数であると仮定します。したがって (V, p. 232、提案 7) $p'(x)/p(x) \ll 1/x$ です。次に、1つは
$$
\frac{p'(x-q(x))}{p(x-q(x))} = \frac{1}{x-q(x)} O_1(1),
$$
それで
$$
q(x) \frac{p'(x-q(x))}{p(x-q(x))} = \frac{q(x)}{x} \left( 1 - \frac{q(x)}{x} \right)^{-1} O_1(1) = \frac{q(x)}{x} O_2(1),
$$
そして、この場合、命題は、$q(x) \ll x$である仮定に*のみ*適用されることがわかります。最後に、$1/x \ll p'(x)/p(x) \ll 1$; の場合を検討します。 写像 $r = p'/p$ は、$x$ に対して有限の位数になります。前述の注意により、prop. V、p. 255の4つは写像に当てはまり、1つは$p'(x-q(x))/p(x-q(x)) \sim p'(x)/p(x)$、そして仮定$qp' \ll p$で証明を完成させることができます。

#### 注意 {#fvr-v-a0-n6-rem-3 .statement tag=08H2}

次の例が示すように、$q(x)$ に課せられた条件は改善されない可能性があります。

a)
$$
p(x) = e^x, \quad q(x) = 1 = \frac{p(x)}{p'(x)}, \quad p(x+q(x)) = ep(x)
$$

b)
$$
p(x) = \log x, \quad q(x) = x - \log x \ll \frac{p(x)}{p'(x)} = x \log x,
$$
$$
p(x-q(x)) = \log \log x \ll p(x).
$$

まず、特定の種類の (H) 写像の逆行列を学習します。

#### 命題 5 {#fvr-v-a0-prop-5 .statement tag=08H3}

*g を * (H) *写像は定数 $\neq 0$ と等価ではなく、* $g(x) \ll x$、*そして* $u(x)$ を* $x - g(x)$ の逆数写像とし、* $+\infty$ の近傍で定義するとします。 *$(u_n)$ *を写像の数列として定義します。* $n$ での再帰によって、*条件* $u_0(x) = x$、$u_n(x) = x + g(u_{n-1}(x))$ *for* $n \geqslant 1$; *その後* $u_n \gg 1$ *そして*
$$
u(x) - u_n(x) \sim g(x)(g'(x))^n.
$$ (11)

$y = u(x)$、$y_n = u_n(x)$ と置きましょう。次に$x = y - g(y)$、$y_0 = x$、$y_n = x + g(y_{n+1})$。まず、$x/y = 1 - \frac{g(y)}{y}$ と推測します。 $y$ は $x$ とともに $+\infty$ になる傾向があるため、仮定 $g(x) \ll x$ は $y = u(x) \sim x = y_0$ を示します。さらに、
$$
y - x = g(y) = g(x) + (y - x)g'(z)
$$
ここで、$z$ 属するから区間はエンドポイント $x, y$ です。 $x$ が $+\infty$ になる傾向がある場合、$z$ も同様であり、$g(x) \ll x$ から $g' \ll 1$ になるため、$g'(z)$ は 0 になる傾向があり、その結果、
$$
y - x = g(x) + o(y - x)
$$

よって
$$
u(x) - x \sim g(x).
$$
(12)

次に、$n$ の再帰によって、$x$ が $+\infty$ になる傾向がある場合、$u_n \gg 1$ になることがわかります。
$$
u(x) - u_n(x) \ll u(x) - u_{n-1}(x).
$$
(13)

実際、$y - y_n = g(y) - g(y_{n-1}) = (y - y_{n-1})g'(z_{n-1})$、$z_{n-1}$ 属するから区間 、エンドポイント $y$ と $y_{n-1}$ です。 帰納法の仮定により $z_{n-1}$ は $x$ と $+\infty$ になる傾向があるため、$g'(z_{n-1})$ は 0 になる傾向があり、これは (13) を証明します。この関係と (12) から、$u(x) - u_n(x) \ll u(x) - x \sim g(x) \ll x \sim u(x)$、よって $u_n(x) \sim u(x)$、そして結果として $u_n \gg 1$ が推測されます。最後に、関係 $u(x) - u_n(x) \ll u(x) - x$ は、$(u(x) - x) - (u_n(x) - x) \ll u(x) - x$、よってとも書くことができます
$$
u_n(x) - x \sim u(x) - x \sim g(x).
$$
(14)

(11) を証明するには、まず、$t(x)$ が $t(x) - x \sim g(x)$ となるような写像である場合、$g'(t(x)) \sim g'(x)$ があることに注意してください。確かに、どの$\varepsilon > 0$でも、$x$でも十分大きい$g'$は単調なので、$g'(t(x))$は$g'(x + (1 + \varepsilon)g(x))$と$g'(x + (1 - \varepsilon)g(x))$の間にあります。 V、p. 255 の提案 4 は、関係 $g \ll g'/g''$ が確立されていれば、$g'(t(x)) \sim g'(x)$ であることを示しています。さて、$g$ が $x$ に対して無限大位数である場合、(V, p. 251, prop. 2) $g''/g' \sim g'/g$ があり、$g' \ll 1, g \ll g/g' \sim g'/g''$ 以降、 $g$ が $x$ に対して有限位数 $\mu$ である場合、必然的に $\mu \leq 1$ になります。 $\mu < 1$ の場合、$g$ は定数 $\neq 0$ と等価ではないため、式 (3) と (4) (V, p. 251) は、$g''/g' \sim k/x$ ($k$ 定数 $\neq 0$)、よってを示します。 $g \ll g'/g''$;最後に、$\mu = 1$ の場合、$g'$ は $x$ に対して位数 0 であるため、$g''/g' \ll 1/x$、そして再び$g \ll g'/g''$ となります。

そうすると、$z_{n-1}$は$y$と$y_n$の間にあるので、(14)より上記より$z_{n-1} - x \sim g(x)$、よって$g'(z_{n-1}) \sim g'(x)$が求まります。したがって
$$
y - y_n \sim (y - y_{n-1})g'(x),
$$
よって $n$ で帰納法により (11) を取得します。

#### 注意 1 {#fvr-v-a0-n6-rem-1 .statement tag=08H4}

$g$ が $x$ に対して位数 $< 1$ である場合、$n$ が十分大きいになると、写像 $u(x) - u_n(x)$ は $x$ で 0 になる傾向があります。実際、逆の場合、$n$ごとに$g{g''}^n \gg 1$が存在するため、$g$は$1/g'$に対して無限位数になります。他の語では、$\log|g| \gg \log|g'|$、よって、微分すると $g'/g \gg g''/g'$ になります。しかし、$g$ が $x$ に対して位数 $\mu < 1$ である場合、$\mu = -\infty, \frac{g'}{g} \sim \frac{\mu}{\mu - 1} \frac{g''}{g'}$ のとき $\mu \neq 0$ のときは $g'/g \sim g''/g'$ となり、最後に $\mu = 0$ (V, p. 251, n) のときは $g'/g \ll g''/g'$ になります。 3)。

対照的に、$g$ が $x$ に対して位数 1 である場合、例 $g(x) = x/\log x$ が示すように、整数 $n > 0$ ごとに $g{g''}^n \gg 1$ を持つことができます。

#### 注意 2 {#fvr-v-a0-n6-rem-2 .statement tag=08H5}

$g(x)$ が定数 $k \neq 0$ と同等の (H) 写像である場合、$g_1 \ll 1$ を伴う $g(x) = k + g_1(x)$ になります。 写像 $u_1(x) = u(x) - k$ は写像 $x - g_1(x + k)$ の逆で、1 つは prop で扱われたケースに戻されます。 V、p. 256の5。

写像 $u$ の漸近展開を持つには、写像 $u_n$ のそのような展開があれば十分です: $g$ が考慮中のスケールに対して漸近展開を認める場合、(H) 写像の定義によって) 問題が検討されます。 V、p. 223 から 227 まで。

最も一般的なケースは、以下のように、prop で扱われるケースに簡約するとなります。 V、p. 256 の 5: 写像 $y = u(x)$ は満たす関係と見なされます
$$
\varphi(x) = \psi(y) - g(y)
$$
ここで、$\varphi$ は (H) 写像、$\psi$ は (H) 写像であり、$\psi \gg 1$ となり、$\psi$ の逆数写像 $\theta$ も (H) 写像となり、$g$ は(H) 写像は $g \ll \psi$ になります。 Let now $v(x)$ be the inverse function of $x - g(\theta(x))$; one has $u = \theta \circ v \circ \varphi$, and $g(\theta(x)) \ll x$; if one knows an asymptotic expansion for $v$ thanks to prop. 5 of V, p. 256, one can then deduce an asymptotic expansion for $u$ as in V, p. 223 to 227.

#### 例 1 {#fvr-v-a0-n6-exa-1 .statement tag=08H6}

$x^5 + x$ の逆写像 $v(x)$ の漸近展開を求めてみましょう ($x$ は $+\infty$ になる傾向があります)。 $x^5 = t$ を置くと、$t + t^{1/5}$ の逆数写像 $u(t)$ ($t$ が $+\infty$ になる傾向がある) の拡張を求めることになります。つまり、prop を適用することになります。 V、p. 256の5、$g(t) = -t^{1/5}$の場合まで。たとえば、計算する、$u_2(t)$ とします。 1つは持っています
$$
u_2(t) = t - \left( t - t^{1/5} \right)^{1/5} = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{2}{25} t^{-7/5} + o_1\left( t^{-7/5} \right).
$$
また、(11)(V、p. 256)により
$$
u(t) - u_2(t) \sim -\frac{1}{25} t^{-7/5}
$$
よって
$$
u(t) = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{1}{25} t^{-7/5} + o_2\left( t^{-7/5} \right)
$$
そして展開を推測します
$$
v(x) = u(x)^{1/5} = x^{1/5} - \frac{1}{5} x^{-3/5} - \frac{1}{25} x^{-7/5} + o_3\left( x^{-7/5} \right)
$$
求めた。

#### 例 2 {#fvr-v-a0-n6-exa-2 .statement tag=08H7}

写像 $x / \log x$ の逆写像の漸近展開を求めてみましょう。 $y = v(x)$ である$x = y / \log y$ から、$\log x = \log y - \log \log y$ が推測されます。 $z = \log y, t = \log x$ を置くと、$t = z - \log z$ があり、$t - \log t$ の逆数写像 $u(t)$ を展開するように導かれます。たとえば、ある人は
$$
u_2(t) = t + \log(t + \log t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + o_1\left( \frac{\log t}{t^2} \right)
$$
さらに、(11) (V、p. 256) によって
$$
u(t) - u_2(t) \sim \frac{\log t}{t^2}
$$
よって
$$
u(t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + \frac{\log t}{t^2} + o_2\left( \frac{\log t}{t^2} \right)
$$
そして元の問題に戻ると、漸近展開が得られます。
$$
v(x) = x \log x + x \log \log x + x \frac{\log \log x}{\log x} + o\left( x \frac{\log \log x}{\log x} \right).
$$

#### 注意 {#fvr-v-a0-n6-rem-4 .statement tag=08H8}

2 つの等価 (H) 写像は、2 つの写像 $\log x$ と $1 + \log x$ のうちの例が示すように、非等価の逆元を持つ可能性があることに注意してください。

### 練習問題 {#fvr-v-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
