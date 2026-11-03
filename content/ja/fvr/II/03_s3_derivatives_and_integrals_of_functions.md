---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 3
section_title: DERIVATIVES AND INTEGRALS OF FUNCTIONS DEPENDING ON A PARAMETER
lang: ja
source: fvr-i-vii
book_pages: 68-78, 86-90
pdf_pages: 0083-0093, 0101-0105
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A COMPACT INTERVAL
      page: 68
      pdf_page: 83
    - "no": 2
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A NON-COMPACT INTERVAL
      page: 69
      pdf_page: 84
    - "no": 3
      title: NORMALLY CONVERGENT INTEGRALS
      page: 72
      pdf_page: 87
    - "no": 4
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A COMPACT INTERVAL
      page: 73
      pdf_page: 88
    - "no": 5
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 75
      pdf_page: 90
    - "no": 6
      title: CHANGE OF ORDER OF INTEGRATION
      page: 76
      pdf_page: 91
statements: 18
exercises: 10
content_sha256: 54006fc541a9021a4c7baa8e923b2da91034316df57c3fb8a24041852db83a51
translated_from: content/en/fvr/II/03_s3_derivatives_and_integrals_of_functions.md
translation_method: google
source_content_sha256: 35c740d0a30b3f3ffd2d5f08cde90f87df1496bb44cbc74f5b2898276d078665
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 47348f0640e8f7d22b84f79d9a99ed7dce14b62506730300a4db493b56ea9732
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。パラメータに応じた写像の微分と積分

### 1. コンパクトな区間に写像の極限を統合

Th. II、p. 52 の 1 は、コンパクトな区間で規制されている写像の特定のケースに適用され、次のように積分に適切な記法に変換されます。

#### 命題 1 {#fvr-ii-s3-prop-1 .statement tag=088Y}

A をフィルター $\mathfrak{F}$ でフィルターした集合と、コンパクトな区間 $I = [a, b]$ 上の規制された写像のファミリー $(f_\alpha)_{\alpha \in A}$ とします。 写像 $f_\alpha$ がフィルター $\mathfrak{F}$ に関してI で (調整された) 写像 f に一様に収束する場合、

$$
\lim_{\mathfrak{F}} \int_a^b f_\alpha(t) \, dt = \int_a^b f(t) \, dt.
$$

これに対する 2 つの帰結命題がアプリケーションでは重要です。

#### 系 1 {#fvr-ii-s3-prop-1-cor-1 .statement tag=088Z}

$(f_n)$ をコンパクト区間 $I = [a, b]$ の規制写像の数列とします。 数列 $(f_n)$ が I で (規制された) 写像 f に一様に収束する場合、

$$
\lim_{n \to \infty} \int_a^b f_n(t) \, dt = \int_a^b f(t) \, dt.
$$

特に、一般項 $u_n$ が I の規制された写像である系列が I の f に一様に収束する場合、系列と一般項 $\int_a^b u_n(t) \, dt$ は収束し、その和は $\int_a^b f(t) \, dt$ (「一様収束系列の項ごとの積分」)。

#### 系 2 {#fvr-ii-s3-prop-1-cor-2 .statement tag=0890}

$A$ をトポロジー 空間 $F$ の部分集合とし、$I \times A$ から $\mathbf{R}$ 上の完全なノルム空間 $E$ に$f$ 写像をそれぞれ次のようにします。 $\alpha \in A$、写像 $x \mapsto f(x, \alpha)$は$I$に規制されます。 $\alpha$ が $A$ に留まりながら点 $\alpha_0 \in \overline{A}$ になる傾向があるように、写像 $x \mapsto f(x, \alpha)$ が$I$ で（規制された）写像 $x \mapsto g(x)$ に一様に収束する場合、

$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_a^b f(x, \alpha)\, dx = \int_a^b g(x)\, dx.
$$

特に:

#### 命題 2 (「パラメーターに関する積分の連続性」) {#fvr-ii-s3-prop-2 .statement tag=0891}

$F$ をコンパクト空間とし、$I = [a,\ b]$ を $\mathbf{R}$ のコンパクト区間とし、$f$ を $I \times F$ の完全ノルム空間 $E$ への連続写像とする$\mathbf{R}$;その場合、写像 $h(\alpha) = \int_a^b f(x, \alpha)\, dx$ は $F$ で連続します。

確かに、$f$ はコンパクト空間 $I \times F$ 上で一様連続であるため、$\alpha$ が任意の点に向かう傾向があるとき、写像 $f(x, \alpha)$ は$I$ 上の$f(x, \alpha_0)$ に一様に収束します。 $\alpha_0 \in F$。

これは、この命題の応用です: 写像 $(x, \alpha) \mapsto x^\alpha$ は積 $I \times J$ で連続です。ここで、$I = [a,\ b]$ は $0 < a < b$ のようなコンパクト区間で、$J$ は $\mathbf{R}$ の任意のコンパクト区間です。 1 つの結論するは、$\int_a^b x^\alpha\, dx$ が $\mathbf{R}$ の $\alpha$ の連続する写像です。さて、$\alpha$ 有理数と $\neq -1$ の場合、この写像は $\frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ に等しく、写像 $\alpha \mapsto \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ は含む $-1$ ではなく、$\mathbf{R}$ の区間ごとに連続します。したがって、すべての実数 $\alpha \neq -1$ に対して、人は (アイデンティティの拡大) $\int_a^b x^\alpha\, dx = \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ を持ちます。これは、すべての実数 $\alpha$ に対して、$x^\alpha$ の導関数は $\alpha x^{\alpha-1}$ (cf. III, p. 94) であることを意味します。

### 2. 非コンパクト区間の写像の極限を積分

Th. II、p. 52 の 1 は、写像がプリミティブを認めると単に仮定しているため、規制されている写像よりも一般的な写像に適用されます。特にその小道具がわかります。 II、p. 68 の 1 は、区間 $I \subset \mathbf{R}$、写像 $f_\alpha$ が *区分的に規制* され、$I$ にわたる *整* が認められるとのみ仮定される場合にも適用されます。ただし、この結果は、prop の他の 2 つの仮説を前提としています。 1 は満たされています。つまり、次のとおりです。
1. $I$ は *有界* 区間; 2' $f_\alpha$ は *一様に* $I$ から $f$ に収束します。 II、p. 68 の公式 (1) は、これら条件のいずれかが満たされなくなったときに *失敗する可能性があります*。これら 2 つの項のどちらかが存在しないか、両方が存在しても値が異なることが起こります。

たとえば、$f_n$ が $]0,\ 1[$ の規制された写像で、$0 < x < 1/n$ の$f_n(x) = n$ と $1/n \leq x \leq 1$ の$f_n(x) = 0$ によって定義される場合、数列 $(f_n)$ は、それに含まれるすべてのコンパクト区間で均一に 0 に収束します。 ]0, 1[ ですが、[0, 1] には一律ではなく、$n$ ごとに $\int_0^1 f_n(t) \, dt = 1$ があります。 1 つは例ですが、$\int_0^1 f_n(t) \, dt$ は置き換えること上の極限の傾向がなく、その前の数列 $(f_n)$ は数列 $((-1)^n f_n)$ によって再び均一に 0 に収束します。これは、]0, 1] に含まれるすべての圧縮区間で一様に 0 に収束します。

On the other hand, on the *unbounded* interval $I = [0, +\infty[$, let $f_n$ be the regulated function such that $f_n(x) = 1/n$ for $n^2 \leq x \leq (n+1)^2$ and $f_n(x) = 0$ for every other value of $x$ in $I$ ($n \geq 1$); the sequence $(f_n)$ converges uniformly to 0 on $I$, but the integral $\int_0^{+\infty} f_n(t) \, dt = (2n+1)/n$ tends to 2 as $n$ increases indefinitely.

他の語では、$I$ が制限されていないとき、$I$ の規制された写像 $\mathbf{f}$ によって形成され、$E$ に値が含まれ、$I$ にわたる積分を認める$\mathscr{I}$ ベクトル空間で表される場合、 写像 $\mathbf{f} \mapsto \int_I \mathbf{f}(t) \, dt$ は、$\mathscr{I}$ に $I$ の一様収束の位相を与えると *cf.* II, p. 53, cor. 2) になります。

私たちは、提案の有効性を保証するために *十分な * 条件を求めます。 1、以下の仮説のもとに、

1. $I$ は $\mathbf{R}$ の任意の区間、写像 $\mathbf{f}_\alpha$ は $I$ で規定され、$I$ にわたる積分を認めます。
2. ファミリ $(\mathbf{f}_\alpha)$ は、$I$ に含まれるすべてのコンパクト区間のフィルター $\mathfrak{F}$ に関して一様に $\mathbf{f}$ に収束します。

$I$(II、p. 64)に含まれるコンパクト区間の有向集合を$\mathfrak{K}(I)$と書くと、II、p. 68の公式(1)の左辺は$\lim_{\delta} \left( \lim_{J \in \mathfrak{K}(I)} \int_J \mathbf{f}_\alpha(t) \, dt \right)$と書けます。一方、プロップを考慮すると。 1 (II. p. 68)、および族 $(\mathbf{f}_\alpha)$ がすべてのコンパクト区間 $J \subset I$ に一様に収束するという事実により、(1) (II, p. 68) の右辺は $\lim_{J \in \mathfrak{K}(I)} \left( \lim_{\delta} \int_J \mathbf{f}_\alpha(t) \, dt \right)$ と書くことができます。 したがって、人はその小道具を理解します。 $\mathfrak{F}$ のフィルターと、有向集合 $\mathfrak{K}(I)$ の切断のフィルター $\Phi$ に関して、写像$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ の極限* を *交換できる場合、II、p. 19 拡大するの 1。 さて、この交換が正当化されるのに *十分な* 条件、つまり *積フィルター* $\Phi \times \mathfrak{F}$ に関して写像 $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ の極限が存在することが分かりました。 トップ.*、I、p. 81、cor.へ。 1)。 この条件を同等の、より管理しやすい条件に変換します。

そもそも、$E$が完全なので、$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$が$\Phi \times \mathfrak{F}$に関して極限を持つはずである位数において、$\varepsilon > 0$ごとに、そのようなコンパクトな区間$J_0 \subset I$と集合$M \in \mathfrak{F}$が存在することが必要十分です。つまり、$M$ の任意の元 $\alpha, \beta$ と、$I$ に含まれるコンパクトな区間 $J \supset J_0$ について、

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\beta(t) \, dt \right| \leq \varepsilon.
$$

一方、この条件自体が次の条件と同等であることを示します。すべての $\varepsilon > 0$ に対して、コンパクト区間 $J_0 \subset I$ および集合 $M \in \mathfrak{F}$ が存在し、$M$ の任意の $\alpha$ および任意のコンパクト区間について、 $J \supset J_0$ は $I$ に含まれており、1 つは

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\alpha(t) \, dt \right| \leq \varepsilon.
$$

この最後の条件が必要であることは確かに明らかです。逆に、それが満たされる場合、(すべてのコンパクト区間での $(\mathbf{f}_\alpha )$ の一様収束によって) 集合 $N \in \mathfrak{F}$ が存在し、$N$ の任意の $\alpha,\ \beta$ について、

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_{J_0} \mathbf{f}_\beta(t)\,dt \right| \leq \varepsilon;
$$

したがって、$M \cap N \in \mathfrak{F}$ の任意の $\alpha$ と $\beta$、および任意のコンパクト区間 $J \supset J_0$ は $\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_J \mathbf{f}_\beta(t)\,dt \right| \leq 2\varepsilon$ となります。

最後に、II、p. 65 の補題により、この最後の条件を次の同等の形に入れることができます: *すべての $\varepsilon > 0$ に対して、コンパクトな区間 $J_0 \subset I$ と集合 $M \in \mathfrak{F}$ が存在します (依存関係に応じて)。 $\varepsilon$) 共通のの内部に点がないすべてのコンパクト区間 $K \subset I$ に $J_0$ があり、すべての $\alpha \in M$ には $\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon$ があります*。

ほとんどの場合、最後の主張、集合 $M$ * が $\varepsilon$* に依存しないと仮定して得られる、より制限的な条件を使用します。

#### 定義 1 {#fvr-ii-s3-def-1 .statement tag=0892}

*One says that the integral $\int_I \mathbf{f}_\alpha(t)\,dt$ is uniformly convergent for $\alpha \in A$ (or uniformly convergent over $A$) if, for every $\varepsilon > 0$ there exists a compact interval $J_0 \subset J$ such that, for every compact interval $K \subset I$ with no interior point in common with $J_0$, and every $\alpha \in A$, one has*

$$
\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon.
$$

この定義は、$\mathscr{K}(I)$ の切断 $\Phi$ のフィルターに関して、写像 $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$ の族が $A$* (写像 $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$ に向かって) に *一様に収束するというというと同等です。それぞれの積分 $\int_I \mathbf{f}_\alpha(t)\,dt$ は *なおさら* 収束します (逆は false)。さらに、私たちが今見たことから (または *Gen. Top.*、X、p. 281、cor. 2):

#### 命題 3 {#fvr-ii-s3-prop-3 .statement tag=0893}

*$(\mathbf{f}_\alpha )$ * を、区間* $I$ 上で規制された写像の族とします: フィルタに関して 1* $\mathfrak{F}$ *族* $(\mathbf{f}_\alpha )$ *一様に写像* $f$ *(規制されている*) $I$) *$I$ に含まれるすべてのコンパクト区間; *2* 整 $\int_I \mathbf{f}_\alpha(t)\,dt$ *すべての* $\alpha \in A$ について一様に収束します。 *これらの仮説の下では、整* $\int_I f(t)\,dt$ *は収束しており、*

$$
\lim_{\mathfrak{F}} \int_I \mathbf{f}_\alpha(t)\,dt = \int_I f(t)\,dt.
$$

プロップの仮説。 3 は、たとえば、$I$ が *有界* 区間で、$\mathbf{f}_\alpha$ が $I$ で *一様に有界* で、$I$ に含まれるすべてのコンパクト区間で一様に $f$ に収束する場合に満たされます。実際、すべての $x \in I$ とすべての $\alpha$ に対して $\| \mathbf{f}_\alpha(x) \| \leq h$ があり、$J_0$ が $I$ の長さと $J_0$ の差が $\leq \varepsilon / h$ である場合、すべての区間について条件 (7) が満たされます。 $K \subset I$ 内装なし点に共通ので $J_0$ が付いています。

プロップと同様に。 II、p. 68 の 1、つまり 2 つの結果が当てはまります。アプリケーションでは 3 つが重要です。

#### 系 1 {#fvr-ii-s3-prop-3-cor-1 .statement tag=0894}

*$(f_n)$ * を任意の区間* $I$ 上で規制された写像の数列とし、* $I$ に含まれる各コンパクト区間上で *一様に写像* $f$ に収束します。 *整* $\int_I f_n(t)\,dt$ *一様収束の場合、整* $\int_I f(t)\,dt$ *は収束し、*
$$
\lim_{n \to \infty} \int_I f_n(t)\,dt = \int_I f(t)\,dt.
$$
(9)

#### 注意 {#fvr-ii-s3-n2-rem-1 .statement tag=0895}

この結果に課せられた仮説は、式 (9) の妥当性にとって十分ですが、必須ではありません。この式を後で積分の概念と同時に一般化し (INT、IV を参照)、より制限の少ない条件を取得します。

#### 系 2 {#fvr-ii-s3-prop-3-cor-2 .statement tag=0896}

*$A$ を位相空間の部分集合* $F$、*および* $f$ *のマップ* $I \times A$ *完全な規範空間* $E$ *上* $\mathbf{R}$、*すべての* $\alpha \in A$について、*関数* $x \mapsto f(x, \alpha)$ *が規制される* $I$。 *一方で、関数* $x \mapsto f(x, \alpha)$ * に含まれるすべてのコンパクトな区間で一様に収束する* $I$ *関数に* $x \mapsto f(x)$ *として* $\alpha$ * $A$ に留まりながら* $\alpha_0 \in \overline{A}$ * になる傾向がある*。 *一方、整* $\int_I f(x, \alpha)\,dx$ *が一様に収束* $A$ の場合、*整* $\int_I f(x)\,dx$ *は収束し、次の結果が得られます*
$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_I f(x, \alpha)\,dx = \int_I f(x)\,dx.
$$
(10)

特に：

#### 命題 4 (「パラメーターに関する不適切な積分の連続性」) {#fvr-ii-s3-prop-4 .statement tag=0897}

*$F$ * をコンパクトな空間とし、* $I$ * $\mathbf{R}$ の任意の区間とし、* $f$ * $I \times F$ から * 完全なノルム空間* $E$ に *連続する写像とします。 *以上* $\mathbf{R}$; *整* $h(\alpha) = \int_I f(x, \alpha)\,dx$ *が $F$ に一様収束する場合、 *それは * $\alpha$ *on* $F$ の連続写像です。

プロップの観点から。 II、p. 69 の 2、この命題も、連続する写像 (*Gen. Top.*、X、p. 282、th. 2) の均一極限の連続性から続きます。

### 3. 通常は収束する積分

$(f_\alpha)_{\alpha \in A}$ を、任意の区間 $I \subset \mathbf{R}$ 上にある規制された写像の族とし、値を完全に標準化した空間 $E$ を $\mathbf{R}$ 上に持つものとします。 $I$ 上に規制された有限実数写像 $g$ が存在し、すべての $x \in I$ とすべての $\alpha \in A$、$\|f_\alpha(x)\| \leq g(x)$、そして積分 $\int_I g(t)\,dt$ が収束すると仮定します。これらの条件の下で、整 $\int_I f_\alpha(t)\,dt$ は $A$ に *絶対的かつ一様に収束* します。実際、$I$ に含まれるすべてのコンパクト区間 $K$ について、
$$
\left\| \int_K f_\alpha(t)\,dt \right\| \leq \int_K g(t)\,dt
$$

そして、整 $\int_I g(t) \, dt$ の収束は、$J$ からのすべてのコンパクト区間 $K \subset I$ 互いに素について、$\int_K g(t) \, dt \leq \varepsilon$ が含まれるように、すべての $\varepsilon > 0$ に対してコンパクト区間 $J \subset I$ が存在することを意味します。前述の性質を持つ実数写像 $g$ が存在するとき、整 $\int_I f_\alpha(t) \, dt$ は通常 $A$ (cf. Gen. Top., X, p. 296) に収束すると言えます。

積分は、通常は収束しなくても、$A$ に一様に収束することがあります。 *これは、$n \leq x \leq n+1$の条件$f_n(x) = 1/x$によって定義される実際の写像の数列$(f_n)$、および$I = [0, +\infty[$の$x$の他の値で$f_n(x) = 0$に発生します。積分$\int_1^\infty f_n(t) \, dt$が一様に収束するのは明らかですが、各$x \in I$とすべての$n$について関係$g(x) \geq f_n(x)$は$g(x) \geq 1/x$を含意するため、$g$の積分は次のようになります。 $I$ は収束していません。

特に、一般的な項 $u_n$ が区間 $I$ の規制された写像である系列を考えてみましょう。また、系列が一般的な項 $\|u_n(x)\|$ (これは規制されている写像である) であると仮定します。 $I$) は、$I$ に含まれるすべてのコンパクト区間に一様に収束し、系列と一般的な項 $\int_I \|u_n(t)\| \, dt$ が収束します。すると (II, p. 66, 提案 2) 系列と一般項 $\|u_n(x)\|$ の (規制された) 写像 $g(x)$, 和は、積分 $\int_I g(t) \, dt$ が収束するようなものです。 $f_n = \sum_{p=1}^n u_p$ を置くと、積分 $\int_I f_n(t) \, dt$ は通常収束します。

$$
\|f_n(x)\| \leq \sum_{p=1}^n \|u_p(x)\| \leq g(x)
$$

すべての $x \in I$ とすべての $n$ に対して。 系列の帰結、和 $f$ と一般的な項 $u_n$ は、積分 $\int_I f(t) \, dt$ が収束するように $I$ で調整された写像であり、

$$
\int_I f(t) \, dt = \sum_{n=1}^\infty \int_I u_n(t) \, dt
$$

(「非コンパクト区間上の系列の用語ごとの統合」)。

### 4. コンパクト区間上の積分のパラメータに関する導関数

$A$ を体 $\mathbf{R}$ (それぞれ体 $\mathbf{C}$) の点 $\alpha_0$ のコンパクト近傍とし、$I = [a, b]$ を $\mathbf{R}$ のコンパクト区間とし、 $f$ $I \times A$ の連続する写像が、$\mathbf{R}$ (それぞれ $\mathbf{C}$) を超える完全な標準の空間 $E$ になります。私たちは、これらの条件 $g(\alpha) = \int_a^b f(t, \alpha) \, dt$ が $A$ で連続する写像であることを見てきました (II、p. 69、提案 2)。 $g$ が点 $\alpha_0$ で導関数を受け入れるのに十分な条件を求めましょう。 1 つは、$\alpha \neq \alpha_0$ で、

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_a^b \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0} \, dt
$$

したがって (II, p. 69, cor. 2)、写像 $x \mapsto \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ が I で (必然的に連続) 写像 $x \mapsto \mathbf{h}(x)$ に一様に収束する場合、$\alpha$ は (残りながら) $\alpha_0$ になる傾向があるため、 $\neq \alpha_0$)、その後、$g$ は点 $\alpha_0$ で $\int_a^b \mathbf{h}(t)\,dt$ に等しい導関数を認めます。さらに、各 $x \in I$、$\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ は $\mathbf{h}(x)$ になる傾向があるため、$\mathbf{h}(x)$ は写像 $\alpha \mapsto \mathbf{f}(x, \alpha)$ の点 $\alpha_0$ での導関数です。この導関数 (*$\alpha$ に関して* $\mathbf{f}$ の *偏導関数と呼ばれる) を記法 $\mathbf{f}'_{\alpha}(x, \alpha_0)$ で表します。私たちが立てた仮説が意味するのは、

$$
g'(\alpha_0) = \int_a^b \mathbf{f}'_{\alpha}(t, \alpha_0)\,dt.
$$

(12)

次の命題は、公式 (12) の妥当性を示す非常に単純な十分な条件を与えます。

#### 命題 5 {#fvr-ii-s3-prop-5 .statement tag=0898}

*偏導関数* $\mathbf{f}'_{\alpha}(x, \alpha)$ *すべて* $x \in I$ *およびすべて* $\alpha$ *開近傍* $V$ *of* $\alpha_0$, *そしてそれがすべて* $\alpha \in V$, *写像* に対して存在すると仮定します。 $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *$I$ に規制されています*。 *これらの条件の下で、* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ * に一様に収束する* $I$ * $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha_0)$ *として* $\alpha$ * $\alpha_0$ に * なる傾向がある* 場合、 *then 写像* $g(\alpha) = \int_a^b \mathbf{f}(t, \alpha)\,dt$ *次のように導関数が認められます。 公式* (12)、*時刻点* $\alpha_0$。

実際、すべての $\varepsilon > 0$ に対して、仮定までに $r > 0$ が存在し、$|\alpha - \alpha_0| \leq r$ は *すべての* $x \in I$ に対して $\| \mathbf{f}'_{\alpha}(x, \alpha) - \mathbf{f}'_{\alpha}(x, \alpha_0) \| \leq \varepsilon$ を意味します。小道具によって。 I、p. 17 の 3 と 5 には、$|\alpha - \alpha_0| \leq r$ ($\alpha \neq \alpha_0$) とすべての $x \in I$ が含まれます

$$
\left\| \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0} - \mathbf{f}'_{\alpha}(x, \alpha_0) \right\| \leq \varepsilon
$$

これは、$\alpha$ が $\alpha_0$ (残りは $\neq \alpha_0$) になる傾向があるため、I 上で $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ から $\mathbf{f}'_{\alpha}(x, \alpha_0)$ への一様収束が証明され、公式 (12) が確立されます。

#### 系 {#fvr-ii-s3-n4-cor-1 .statement tag=0899}

*偏微分* $\mathbf{f}'_{\alpha}(x, \alpha)$ *が* $I \times V$ *上に存在し、* $(x, \alpha)$ *この集合上での連続写像である場合、写像* $g$ *は公式* (12) *で与えられる微分を認めます。 点* $\alpha_0$。

実際、W が V に含まれる $\alpha_0$ のコンパクト近傍である場合、写像 $(x, \alpha) \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ はコンパクト集合 $I \times W$ 上で *一様連続* であるため、$\mathbf{f}'_{\alpha}(x, \alpha)$ は上で一様に $\mathbf{f}'_{\alpha}(x, \alpha_0)$ になる傾向があります。 $\alpha$ として I は $\alpha_0$ になる傾向があります。

プロップから。 5 より一般的な命題を導き出すと、被積分関数 $\mathbf{f}$ だけでなく、積分の極限もパラメータ $\alpha$ に依存する場合、積分の導関数を評価できるようになります。

#### 命題 6 {#fvr-ii-s3-prop-6 .statement tag=089A}

※propの仮説を仮定します。 5 つが満たされているとします。* $a(\alpha)$、$b(\alpha)$ *2 写像を * $V$、*値を * $I$ に定義します。 *導関数* $a'(\alpha_0),\ b'(\alpha_0)$ が存在し、有限である場合、写像 $g(\alpha) = \int_{a(\alpha)}^{b(\alpha)} f(t, \alpha)\, dt$ は $\alpha_0$ で公式によって与えられる導関数を許容します。

$$
g'(\alpha_0) = \int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt + b'(\alpha_0)f(b(\alpha_0), \alpha_0) - a'(\alpha_0)f(a(\alpha_0), \alpha_0).
$$

実際、$\alpha_0$ と異なるすべての $\alpha \in V$ について、次のように書くことができます。

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_{a(\alpha_0)}^{b(\alpha_0)} \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0}\, dt + \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt
$$
$$
- \frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt.
$$

プロップにより。 II、p. 74 の 5、右側の最初の積分は、$\alpha$ が $\alpha_0$ になる傾向があるのと同様に、$\int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt$ になる傾向があります。 2 番目の積分では、置き換える $f(t, \alpha)$ by $f(b(\alpha_0), \alpha_0)$ を実行し、差が 0 になる傾向があることを示します。 $M = \max (\|f(b(\alpha_0), \alpha_0)\|, |b'(\alpha_0)| + 1)$ を入れます。 写像 $b(\alpha)$ は点 $\alpha_0$ と写像 $f$ 点 $(b(\alpha_0), \alpha_0)$ で連続し、$0 < \varepsilon < 1$ となるように $\varepsilon$ ごとに関係となるような $r > 0$ が存在します。 $|\alpha - \alpha_0| \leq r$ は、エンドポイント $b(\alpha_0)$ および $b(\alpha)$ を持つすべての $t$ 所属から区間に対して $\|f(t, \alpha) - f(b(\alpha_0), \alpha_0)\| \leq \varepsilon$ を伴います。従って、関係 $|\alpha - \alpha_0| \leq r$ は $\left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} - b'(\alpha_0) \right| \leq \varepsilon$ を含意すると考えることもできます。

つまり、値公式 (II、p 62、公式 (17)) ということになります。

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} f(b(\alpha_0), \alpha_0) \right| \leq \left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \right| \varepsilon
$$

そしてその結果として

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - b'(\alpha_0) f(b(\alpha_0), \alpha_0) \right| \leq 2M \varepsilon
$$

これは、$\frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt$ が $b'(\alpha_0) f(b(\alpha_0), \alpha_0)$ になる傾向があることを示しています。同様に、$\frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt$ は $a'(\alpha_0) f(a(\alpha_0), \alpha_0)$ になる傾向があることがわかります。

### 5. 非コンパクト区間上の積分のパラメータに関する導関数

集合 $V$ は prop と同じ意味です。 II、p. 74 の 5 について、I が $\mathbf{R}$ の *任意の* 区間であり、$f$ が $I \times V$ から E への *連続* 写像であるとします。整 $g(\alpha) = \int_I f(t, \alpha)\, dt$ がすべての $\alpha \in V$ に対して存在し、$\alpha$、写像 $g$ の連続写像である場合、$f'_\alpha(x, \alpha)$ が収束したとしても、*$\int_I f'_\alpha(t, \alpha_0)\, dt$ *点* $\alpha_0$ に等しい導関数を持つ必要はありません。 I に含まれるすべてのコンパクト区間で一律に $f'_\alpha(x, \alpha_0)$ となり、整 $\int_I f'_\alpha(t, \alpha) \, dt$ がすべての $\alpha \in V$ に存在する場合 (cf. II、p. 87、練習問題 3)。

公式 (12) (II, p. 74) が有効なままとなるのに十分な条件は、次の命題で与えられます。

#### 命題 7 {#fvr-ii-s3-prop-7 .statement tag=089B}

I を $\mathbf{R}$ の任意の区間とし、$f$ を $I \times V$ の連続する写像とします。次のように仮定します。
1. 偏導関数 $f'_\alpha(x, \alpha)$ はすべての $x \in I$ とすべての $\alpha \in V$ に対して存在し、すべての $\alpha \in V$ について、写像 $x \mapsto f'_\alpha(x, \alpha)$ は I に規制されます。
2. すべての $\alpha \in V$、$f'_\alpha(x, \beta)$ は、$\beta$ が $\alpha$ になる傾向があるため、I に含まれるすべてのコンパクト区間で一様に $f'_\alpha(x, \alpha)$ に収束します。
3. 整$\int_I f'_\alpha(t, \alpha) \, dt$ は$V$ に一様に収束します。
4. 整$\int_I f(t, \alpha_0) \, dt$ は収束します。

このような状況では、整 $g(\alpha) = \int_I f(t, \alpha) \, dt$ は $V$ に一様に収束し、写像 $g$ は $V$ の点ごとに公式によって与えられる微分を許容します。

$$
g'(\alpha) = \int_I f'_\alpha(t, \alpha) \, dt.
$$

$V$ での $\int_I f'_\alpha(t, \alpha) \, dt$ の一様収束は、含まれるコンパクト区間 $J$ の有向集合 $\mathfrak{K}(I)$ の切断 $\Phi$ のフィルタに対して、写像 $\alpha \mapsto \int_J f'_\alpha(t, \alpha) \, dt$ が $V$ で一様収束することを意味します。 Iに。 $u_J(\alpha) = \int_J f(t, \alpha) \, dt$ を入れてみましょう。仮説は、一方では$u_J(\alpha_0)$が$\Phi$に関して極限を持ち、他方ではpropにより極限を持っていることを示しています。 IIの5、p. 74、すべての$\alpha \in V$の$u'_J(\alpha) = \int_J f'_\alpha(t, \alpha) \, dt$。 したがって、次のことを適用できます。 IIの1、p. 52から写像$u_J$、添字の集合の役割は$\mathfrak{K}(I)$によってここに取られ、この集合のフィルターの役割はフィルター$\Phi$によって行われます。すぐに命題が続きます。

#### 注意 1 {#fvr-ii-s3-n5-rem-1 .statement tag=089C}

条件プロップの 1 と 2。 $f'_\alpha(x, \alpha)$が$I \times V$で$(x, \alpha)$の連続写像であるとき、7はなおさらを満たす。

#### 注意 2 {#fvr-ii-s3-n5-rem-2 .statement tag=089D}

整 $\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt$ において、区間の端点がパラメーターの有限写像である場合、$\alpha$ の写像としてのこの積分の研究は、$[0, 1]$ にわたる積分の研究と関連付けることができます。実際、変数 $t = a(\alpha)(1 - u) + b(\alpha)u$ の変更により、

$$
\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt = \int_0^1 f(a(\alpha)(1 - u) + b(\alpha)u, \alpha) (b(\alpha) - a(\alpha)) \, du.
$$

### 6. 統合の位数の変更

$I = [a, b]$ と $A = [c, d]$ を $\mathbf{R}$ の 2 つのコンパクトな区間とします。 $f$ を $\mathbf{R}$ 上の完全正規化空間 E の値を伴う $I \times A$ 上の連続写像とする。プロップによって。 II、p. 69、$\int_a^b f(x, \alpha) \, dx$ の 2 は、$A$ の $\alpha$ の連続する写像です。簡単にするために、その積分 $\int_c^d \left( \int_a^b f(x, \alpha) \, dx \right) d\alpha$ も $\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx$ で表されます。

#### 命題 8 {#fvr-ii-s3-prop-8 .statement tag=089E}

*f が I × A で連続である場合、1 は*

$$
\int_c^d d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^d f(x, \alpha) d\alpha
$$

(「統合の交換すること位数に対して公式」)。

すべての $y \in A$ について、人は

$$
\int_c^y d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^y f(x, \alpha) d\alpha.
$$

(16) の両辺は $y$ の写像であり、$y = c$ に等しいので、これらが $]c, d[$ で微分可能であり、その導関数がこの区間のすべての点で等しいことを証明すれば十分です。 $g(\alpha) = \int_a^b f(x, \alpha) dx$と$h(x, y) = \int_c^y f(x, \alpha) dx$を入れると、関係 (16) が書けます

$$
\int_c^y g(\alpha) d\alpha = \int_a^b h(x, y) dx.
$$

さて、$y$ に関する最初の項の導関数は $g(y)$ ですが、$h_y'(x, y) = f(x, y)$ は $I \times A$ で連続であるため、2 番目の導関数は $\int_a^b h_y'(x, y) dx$ で、II、p. 74、系になります。このようにして得られた 2 つの式は同一です。

ここで、$A = [c, d]$ が $\mathbf{R}$ の *コンパクト* 区間であり、I が $\mathbf{R}$ の *任意* 区間であると仮定します。 $f$ を、E に値を伴う、$I \times A$ 上の連続写像とし、整 $g(\alpha) = \int_I f(t, \alpha) dt$ がすべての $\alpha \in A$ について収束するようにします。たとえ$g(\alpha)$が$A$で連続であっても、できないは常に積分$\int_c^d d\alpha \int_I f(t, \alpha) dt$の積分の位数を交換します。なぜなら、整$\int_I dt \int_c^d f(t, \alpha) d\alpha$は存在しないか、整$\int_c^d d\alpha \int_I f(t, \alpha) dt$と異なる可能性があります(*cf.* II, p. 87、練習問題 7)。ただし、次のような結果が得られます。

#### 命題 9 {#fvr-ii-s3-prop-9 .statement tag=089F}

*写像 f が I × A 上で連続で、整 $\int_I f(t, \alpha) dt$ が A に一様収束する場合、整 $\int_I dt \int_c^d f(t, \alpha) d\alpha$ は収束し、*

$$
\int_c^d d\alpha \int_I f(t, \alpha) dt = \int_I dt \int_c^d f(t, \alpha) d\alpha.
$$

I に含まれるコンパクト区間 J ごとに、$u_J(\alpha) = \int_J f(t, \alpha) dt$ を置きます。 仮定は、有向集合 $\mathscr{K}(I)$ の切断 $\Phi$ のフィルタに関して、連続写像 $u_J$ が A から$\int_I f(t, \alpha) dt$ まで一様に収束することを意味します。したがって (II, p. 68、提案 1)、$\int_c^d d\alpha \int_J f(t, \alpha) dt$ は $\Phi$ に対して極限 $\int_c^d d\alpha \int_I f(t, \alpha) dt$ になります。ただし、小道具によって。 8 (II、p. 77)、1 つは

$$
\int_c^d d\alpha \int_J f(t, \alpha) dt = \int_J dt \int_c^d f(t, \alpha) d\alpha.
$$

したがって、前の結果は、整 $\int_1 dt \int_c^{d} f(t, \alpha) d\alpha$ が収束し、関係 (18) の $\Phi$ に関して移行から極限で、(17) が得られることを意味します。

### 練習問題 {#fvr-ii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
