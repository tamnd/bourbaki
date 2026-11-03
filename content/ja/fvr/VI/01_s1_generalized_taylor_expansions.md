---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 1
section_title: GENERALIZED TAYLOR EXPANSIONS
lang: ja
source: fvr-i-vii
book_pages: 269-283, 291-292
pdf_pages: 0284-0298, 0306-0307
extraction: ocr
subsections:
    - "no": 1
      title: COMPOSITION OPERATORS ON AN ALGEBRA OF POLYNOMIALS
      page: 269
      pdf_page: 284
    - "no": 2
      title: APPELL POLYNOMIALS ATTACHED TO A COMPOSITION OPERATOR
      page: 272
      pdf_page: 287
    - "no": 3
      title: GENERATING SERIES FOR THE APPELL POLYNOMIALS
      page: 274
      pdf_page: 289
    - "no": 4
      title: BERNOULLI POLYNOMIALS
      page: 275
      pdf_page: 290
    - "no": 5
      title: COMPOSITION OPERATORS ON FUNCTIONS OF A REAL VARIABLE
      page: 277
      pdf_page: 292
    - "no": 6
      title: INDICATRIX OF A COMPOSITION OPERATOR
      page: 278
      pdf_page: 293
    - "no": 7
      title: THE EULER-MACLAURIN SUMMATION FORMULA
      page: 282
      pdf_page: 297
statements: 21
exercises: 3
content_sha256: 6ae51717471b2c1e7362106e1419ed5fc0d7eac11fd24bbe3b3fcca854baa372
translated_from: content/en/fvr/VI/01_s1_generalized_taylor_expansions.md
translation_method: google
source_content_sha256: 7b62ad591ac33887b2cec9de99a553da0d73b1a05da4f701901b379dc016e8a0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 10e90b6db591838f8441b6ecdad394f29b89cafbaf454d9ad7089cae9f32f3fe
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。一般化されたテイラー拡張

### 1. 多項式の代数の合成演算子

K を標数 0 の可換体とし、K 上の 1 つの不定多項式の K[X] 代数とします (Alg.、IV. 1)。この切断を通じて K[X] 上の演算子によって、それ自体へのベクトル空間 K[X] (K 上の) の線形写像 U を意味します。この空間に対して単項式 $X^n \ (n \geqslant 0)$ 形基底があるため、U は多項式 $U(X^n)$ によって決定されます。具体的には、$f(X) = \sum_{k=0}^\infty \lambda_k X^k$ と $\lambda_k \in K$ の場合、
$$
U(f) = \sum_{k=0}^\infty \lambda_k U(X^k).
$$
G が K より可換代数で、単位元である場合、G 加群 G[X] は、ベクトル空間 K[X] のスカラー K の体を G に拡張することによって取得されます。 K[X] 拡大する上のすべての演算子 U を、それ自体に対する G モジュール G[X] の線形写像に一意の方法で変換し、これを再び U (Alg., II, p. 278) で表します。 元 $g(X) = \sum_{k=0}^\infty \gamma_k X^k$ ごとに、$\gamma_k \in G$ と 1 つは $U(g) = \sum_{k=0}^\infty \gamma_k U(X^k)$ になります。

特に G = K[Y] の場合を考えてみましょう。この場合、G[X] は K 上の 2 つの不定数の多項式の環 K[X,Y] です。混乱を避けるために、U ～ G[X] の拡大を $U_X$ で表します。したがって、$\gamma_k(Y) \in K[Y]$ である多項式 $g(X, Y) = \sum_{k=0}^\infty \gamma_k(Y) X^k$ については、$U_X(g) = \sum_{k=0}^\infty \gamma_k(Y) U(X^k)$ になります。 $U_X$ は線形なので、$g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ と書けば、$U_X(g) = \sum_{h=0}^\infty U(\beta_h) Y^h$ もあることがわかります。

Y を X に関連付ける K[Y] 上の K[X] の標準同型の下で、演算子 U 変換を K[Y] 上の演算子に結合します。混乱を避けるために、これを $U_Y$ とします。そのため、$U_Y(f(Y))$ は置き換えることによって得られる多項式になります。 X は多項式 $U(f(X)) = U_X(f(X))$ の Y によって計算されます。この演算子 $U_Y$ は、K[X,Y] 上の演算子 (再び $U_Y$ で示される) に拡張できます: if $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ then
$$
U_Y(g(X, Y)) = \sum_{h=0}^\infty \beta_h(X) U_Y(Y^h).
$$

これら拡大のうちの例として、K[X] 上の導分演算子 D (Alg., IV.6) を引用します。これにより、K[X,Y] 上の部分導分演算子 D_X および D_Y が得られます。

任意の多項式 $f \in K[X]$ について、K[X,Y] の多項式 $f(X + Y)$ を $T_Y(f)$ で表します。 写像 $T_Y$ は、K[X] から K[X,Y] への K 線形写像であり、変換演算子と呼ばれます。

#### 定義 1 {#fvr-vi-s1-def-1 .statement tag=08HO}

*K[X] 上の演算子 U は、変換演算子と交換できる場合、つまり $U_X T_Y = T_Y U$ の場合、合成演算子であると言われます。*

他の語では、$f$ が K[X] の任意の多項式である場合、および $g = U(f)$ の場合、$g(X + Y) = U_X(f(X + Y))$ が必要です。

この定義から、すべての多項式 $f(X) \in K[X]$ について、上記の記法では、次のことがすぐにわかります。

$$
U_X(f(X + Y)) = U_Y(f(X + Y)).
$$

(1)

#### 例 1 {#fvr-vi-s1-n1-exa-1 .statement tag=08HP}

すべての $\lambda \in K$ に対して、すべての多項式 $f(X)$ と多項式 $f(X + \lambda)$ を関連付ける演算子は、合成演算子です。

#### 例 2 {#fvr-vi-s1-n1-exa-2 .statement tag=08HQ}

K[X] の導分 D は合成演算子 (*cf.* prop. 1) です。

#### 注意 {#fvr-vi-s1-n1-rem-1 .statement tag=08HR}

K は無限体なので、K[X] の演算子 U は、すべての多項式 $f \in K[X]$ とすべての元 $\alpha \in K$ について、$g = U(f)$ を置くと、$g(X + \alpha) = U(f(X + \alpha))$ となる場合に限り、合成演算子になります。 (Alg.、IV.16、cor.)。

K に係数を含む、合成演算子のすべての線形結合が合成演算子であることは明らかです。 2 つの合成演算子のうちの合成にも同じことが当てはまります。他の語、合成演算子では、形部分代数 $\Gamma$ の代数の自己準同型のベクトル空間 K[X]。

#### 命題 1 {#fvr-vi-s1-prop-1 .statement tag=08HS}

*K[X] 上の演算子 U が合成演算子であるためには、K[X] 上の導分 D と可換であることが必要かつ十分です。*

実際、テイラー 公式は、すべての多項式 $f \in K[X]$ に対して、

$$
U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k f(X) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k U(D^k f(X));
$$

$g = U(f)$ と置くと、

$$
g(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k g(X) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k (U(f(X)));
$$

U が合成演算子であるためには、すべての整数 $k \geq 1$、特に $UD = DU$ に対して $UD^k = D^k U$ が必要です。逆に、この関係が成り立つ場合、$k$ の帰納法までに、整数 $k \geq 1$ ごとに $UD^k = D^k U$ が発生することを意味します。テイラー 公式は $g(X + Y) = U_X(f(X + Y))$ を示します。

すべての多項式 $f \in K[X, Y]$ を、多項式 $U_X(f)$ の X から *独立して $U_0(f)$ 項で表します。特に、$f \in K[X]$ の場合、$U_0(f)$ は $U(f)$ の *定数項* であり、$U_0$ は $K[X]$ の *線型形式* です。すべての多項式 $f \in K[X]$ について $g = U(f)$ とします。間違いなく。 VI、p. 270 の 1 つ

$$
g(X + Y) = U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} X^k D^k f(Y) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} U(X^k) D^k f(Y)
$$

そして、この公式で 1 つの置き換える X を 0 にすると、次の結果が得られます。

$$
g(Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U_0(X^k) D^k f(Y).
$$

したがって、次のことがわかります

$$
U(f(X)) = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k f(X) \tag{2}
$$

ここで、$\mu_k$ * は多項式 * $U(X^k)$ の定数項です。

この公式は、$\mu_k$ 決定する合成演算子 $U$ が完全に機能することを示しています。逆に、$(\mu_n)$ が K の元の*任意の* 数列である場合、公式 (2) 定義するは明らかに D と可換な演算子 $U$ であるため、(VI, p. 270, 定理 1) は合成演算子です。これから形に(2)を書きます。

$$
U = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k. \tag{3}
$$

この公式は位相言語で次のように解釈できます。 $K[X]$ 上の離散位相と、$K[X]$ の自己準同型の $\mathrm{End}(K[X])$ 、および代数上の *単純* 収束の位相を考慮すると、 Top.*, X, p. 277)、系列と一般的な項 $\frac{1}{k!} \mu_k D^k$ は $\mathrm{End}(K[X])$ で可換収束し、和 $U$ を持ちます (*Gen. トップ。*、III、p. 269)。

公式 (3) は、K (*Alg.*, IV. 41) 上の 1 つの不定数におけるすべての *形式系列* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ に合成演算子 $U = \sum_{k=0}^{\infty} \alpha_k D^k$ を関連付けることができることを示しており、将来的にはこれを $u(D)$ で表すことになります。この注意は次のように明確にできます。

#### 定理 1 {#fvr-vi-s1-thm-1 .statement tag=08HT}

*写像は、すべての正式な系列* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ *1 つの不定上* K *関連する合成演算子* $u(D) = \sum_{k=0}^{\infty} \alpha_k D^k$ *on* $K[X]$ *は代数* $K[[S]]$ *正式な系列の同型代数* $\Gamma$ *合成演算子中*

この写像が準同型であることがすぐに確認されます。他の語では、関係 $\sum_{k=0}^{\infty} \alpha_k D^k = 0$ がすべての $k$ に対して $\alpha_k = 0$ を暗示することは単射的であることがわかります。ここで、$h! \alpha_h$ は、適用 $\sum_{k=0}^{\infty} \alpha_k D^k$ から $X^h$、よって定理によって得られる多項式の定数項です。

#### 系 {#fvr-vi-s1-n1-cor-1 .statement tag=08HU}

*$K[X]$ の合成演算子の代数 $\Gamma$ は可換です。*

#### 例 {#fvr-vi-s1-n1-exa-3 .statement tag=08HV}

$U$ が各多項式 $f(X)$ に $f(X + \lambda)$ ($\lambda \in K$) を関連付ける演算子である場合、$U_0(X^k) = \lambda^k$ があり、したがって $U = \sum_{k=0}^{\infty} \frac{1}{k!} (\lambda D)^k$ になります。 $e^{\lambda}$ (III、p. 105) の系列拡張との類推により、環 $K[[S]]$ の正式な系列 $\sum_{n=0}^{\infty} \frac{1}{n!} S^n$ に対して $e^S$ または $\exp(S)$ を書きます。したがって、$U = e^{\lambda D}$ と書くことができます。この引数では、有理分数 $K(Y)$ の体による置き換えること体 $K$ からも、同様に *翻訳演算子* $T_Y$ が $e^{YD}$ と記述できることが分かります。

さらに、形式的な系列の環 $K[[S, T]]$ では、$K$ に関する 2 つの不定数のうち、1 つは

$$
(\exp S)(\exp T) = \sum_{p,q} \frac{S^p}{p!} \frac{T^q}{q!}
$$
$$
= \sum_{n=0}^{\infty} \frac{1}{n!} \left( \binom{n}{0} S^n + \binom{n}{1} S^{n-1} T + \cdots + \binom{n}{n} T^n \right)
$$
$$
= \exp(S + T)
$$

そして特に
$$
(\exp S)(\exp(-S)) = 1
$$
これは、私たちが導入した記法を正当化します。

#### スクリウム {#fvr-vi-s1-n1-sch-1 .statement tag=08HW}

形式級数の代数 $K[[S]]$ と $K[X]$ 上の合成演算子の代数 $\Gamma$ の同型性により、対応する合成演算子 (*cf.* VI, p. 274, prop. 6) を証明することにより、形式級数の命題を最も簡単に証明できることがあります。

### 2. 合成演算子に多項式を適用します

合成演算子 $U = \sum_{k=0}^{\infty} \alpha_k D^k \neq 0$ が与えられた場合、$p$ を $\alpha_k \neq 0$ となるような整数 $k$ の最小値とします。 $p$ は演算子 $U$ の *位数* であるとします。

#### 命題 2 {#fvr-vi-s1-prop-2 .statement tag=08HX}

位数 0 のすべての合成演算子は、$\mathbf{K}[X]$ の合成演算子の代数 $\Gamma$ で反転可能です。

実際、$\alpha_0 \neq 0$ が環 $\mathbf{K}[[S]]$ で可逆であるような形式的な系列 $\sum_{k=0}^{\infty} \alpha_k S^k$ (Alg.、IV. 41)。したがって、命題は th から続きます。 VI、p. 271 の 1 つ。

#### 命題 3 {#fvr-vi-s1-prop-3 .statement tag=08HY}

$U$ を位数 $p$ の合成演算子とします。次に、次数 $< p$ のすべての多項式 $f$ に対して $U(f) = 0$ を計算します。 次数 $n \geq p$ のすべての多項式 $f \neq 0$ に対して、$U(f)$ は次数 $n - p$ の多項式 $\neq 0$ です。

これは、VI、p. 271 の式 (2) と $U$ の次数の定義の直接の結果です。

位数 $p$ のすべての演算子 $U$ は、$U = D^p V = V D^p$ として独自の方法で書くことができることは明らかです。ここで、$V$ は位数 0 の演算子です (したがって反転可能です)。

#### 定義 2 {#fvr-vi-s1-def-2 .statement tag=08HZ}

$U = D^p V$ を $\mathbf{K}[X]$ 上の位数 $p$ の合成演算子とします。多項式$u_n(X) = V^{-1}(X^n)$は、演算子$U$に付加された添字$n$のAppell多項式と呼ばれます。

$V^{-1} = \sum_{k=0}^{\infty} \frac{1}{k!} \beta_k D^k$ ($\beta_0 \neq 0$ 付き) の場合、次のようになります。
$$
u_n(X) = \sum_{k=0}^{n} \binom{n}{k} \beta_k X^{n-k}.
$$
(6)

$u_n$ が次数 $n$ の多項式であることを検証します (提案 3)。さらに
$$
u_n(0) = \beta_n.
$$

#### 命題 4 {#fvr-vi-s1-prop-4 .statement tag=08I0}

$U$ 満たす関係に付加された Appell 多項式
$$
\frac{d u_n}{d X} = n \, u_{n-1}
$$
(7)
$$
u_n(X + Y) = \sum_{k=0}^{n} \binom{n}{k} u_{n-k}(X) Y^k
$$
(8)
$$
U(u_n(X)) = \frac{n!}{(n-p)!} X^{n-p}.
$$
(9)

これらの式は、実際にはそれぞれ次の関係と等価です (定義 2 を念頭に置きます)。

$$
DV^{-1} = V^{-1}D \tag{10}
$$
$$
(\exp(YD_X))V_X^{-1} = V_X^{-1}\exp(YD_X) \tag{11}
$$
$$
UV^{-1} = D^p. \tag{12}
$$

#### 命題 5 {#fvr-vi-s1-prop-5 .statement tag=08I1}

*すべての多項式 $f \in K[X]$ と位数 $p$ のすべての合成演算子について、次の式が得られます*

$$
f^{(p)}(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U \left( f^{(k)}(X) \right) u_k(Y) \tag{13}
$$
*(一般化されたテイラー展開)*。

確かに、$U = D^p V = V D^p$ を置くと (VI, p. 270, 公式 (1)) になります。

$$
V_X^{-1}(f(X + Y)) = V_Y^{-1}(f(X + Y)) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(X) u_k(Y) \tag{14}
$$
テイラー 公式そして間違いなく。 VI、p. 273 の 2 つ。 (13) を得るには、公式 (14) の最初と最後の項に演算子 $U$ を適用するだけで十分です。

### 3. 生成する系列はアピール多項式の場合

E を不定 S の *形式的系列* の環とし、多項式 $K[X]$ (*Alg.*, IV. 41) の環内の係数とします。正式な系列 $g(X, S) = \sum_{n=0}^{\infty} \alpha_n(X) S^n$ の他の語、環では、$\alpha_n$ 属するから $K[X]$ までです。 $K[X]$ 上のすべての演算子 $U$ に対して、$U_X(g(X, S)) = \sum_{n=0}^{\infty} U(\alpha_n) S^n$ を代入することで、E の定義する写像 $U_X$ をそれ自体に代入します。 E は、S の正式な系列の環 $K[[S]]$ と、$K$ の係数よりも加群であることは明らかです。 $K[X]$ 上の $U$ の線形性により、すべての元 $\theta \in K[[S]]$ とすべての $g \in E$ について$U_X(\theta g) = \theta U_X(g)$ があることがすぐに検証されます。他の語では、$U_X$ は加群 E の線形写像をそれ自体に変換したものです。

#### 命題 6 {#fvr-vi-s1-prop-6 .statement tag=08I2}

*$U = D^p V = u(D)$ を $K[X]$ の位数 $p$ の合成演算子とし、$u(S)$ を $K[[S]]$ の位数 $p$ の正式な冪系列とします。それから*

$$
U_X \left( \exp(XS) \right) = u(S) \exp(XS) \tag{15}
$$
$$
\frac{S^p}{u(S)} \exp(XS) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n \tag{16}
$$
*n は U* に付加された添字 n のアペル多項式です。

スコリウムからthまで。 1 (VI, p. 271)、(15) を確立するには、すべての多項式 $f(Y) \in K[Y]$ について、

$$
U_X \left( \exp(XD_Y)(f(Y)) \right) = u(D_Y)(\exp(XD_Y)(f(Y))).
$$

ここで、(17) の最初の項は $U_X(f(X + Y))$ で、$U = u(D)$ 以降、(17) の 2 番目の項は $U_Y(f(X + Y))$ となるため、(1) に対する恒等式 (17) 簡約するは (VI, p. 270) となります。

(16) を得るには、(15) を合成演算子 $V^{-1} = D^p / u(D)$ に適用するだけで十分です。なぜなら、定義までに、

$$
V^{-1}(\exp(XS)) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n.
$$

(16) は、(6) を考慮して、形式的な系列 $S^p / u(S)$ と $\exp(XS)$ を乗算することによっても得られることに注意してください。

正式な系列 (16) は、$U$ に付加された Appell 多項式の生成する系列であると言われています。

### 4. ベルヌーイ多項式

によって定義された合成演算子 $U$ を考えてみましょう。

$$
U(f(X)) = f(X + 1) - f(X);
$$

$U = e^D - 1$ (VI, p. 270, 例 1) と書くことができます。これは位数 1 の演算子で、$U = DV$ を入れると $V^{-1} = \frac{D}{e^D - 1}$ になります。演算子 $U$ に対するアペル多項式次数 $n$ 対応するは、次数 $n$ のベルヌーイ多項式と呼ばれ、$B_n(X)$ で表されます。 $b_n = B_n(0)$ と置くと、次の式が得られます。

$$
B_n(X) = \sum_{k=0}^{n} \binom{n}{k} b_{n-k} X^k
$$
(18)

$$
\frac{S \, e^{XS}}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} B_n(X) S^n
$$
(19)

そして特に

$$
\frac{S}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} b_n S^n
$$
(20)

VI、p. 273 の式 (7) と (9) は、ベルヌーイ多項式に対して、関係を与えます。

$$
\frac{dB_n}{dX} = n B_{n-1}(X)
$$
(21)

$$
B_n(X + 1) - B_n(X) = n X^{n-1}.
$$
(22)

特に、$n > 1$ に対して $B_n(1) - B_n(0) = 0$ があり、(18) を考慮すると、帰納法関係が得られます。

$$
\sum_{m=0}^{n-1} \binom{n}{m} b_m = 0 \quad \text{(for } n > 1)
$$

これにより、計算するから $b_n$ を段階的に実行できるようになります。これらの数は明らかに *有理 * です。書けるので

$$
\frac{S}{e^S - 1} = -\frac{S}{2} + \frac{S}{2} \frac{e^S + 1}{e^S - 1}
$$

そしてそれ以来 (VI, p. 272, 公式 (5))

$$
\frac{e^{-S} + 1}{e^{-S} - 1} = -\frac{e^S + 1}{e^S - 1}
$$

$\frac{S}{2} \frac{e^S + 1}{e^S - 1}$ の正式な系列では、*奇数* 次数のすべての項が係数零であることがわかります。だから人は持っています

$$
b_0 = 1, \qquad b_1 = -\frac{1}{2}, \qquad b_{2n-1} = 0 \quad \text{for } n > 1.
$$

有理数数 $b_{2n}$ ($n \geq 1$) は *ベルヌーイ数* と呼ばれます。 (VI、p. 288) $b_{2n}$ には $(-1)^{n-1}$ の符号があることがわかります。 公式 (23) は、$n$ の最初の値に対して、

$$
\begin{align*}
b_2 &= \frac{1}{6}, & b_4 &= -\frac{1}{30}, & b_6 &= \frac{1}{42}, & b_8 &= -\frac{1}{30}, \\
b_{10} &= \frac{5}{66}, & b_{12} &= -\frac{691}{2730}, & b_{14} &= \frac{7}{6}, \\
b_{16} &= -\frac{3617}{510}, & b_{18} &= \frac{43867}{798}, & b_{20} &= -\frac{174611}{330}, & b_{22} &= \frac{854513}{138}, \\
b_{24} &= -\frac{236364091}{2730}, & b_{26} &= \frac{8553103}{6}, & b_{28} &= -\frac{23749461029}{870}.
\end{align*}
$$

分子 691、3617、43867 は素数であることに注意してください。他のものの素因数分解は次のとおりです。

$$
\begin{align*}
174611 &= 283 \times 617 \\
854513 &= 11 \times 131 \times 593 \\
236364091 &= 103 \times 2294797 \\
8553103 &= 13 \times 657931 \\
23749461029 &= 7 \times 9349 \times 362903.
\end{align*}
$$

これらから、最初のベルヌーイ多項式の式を導き出します。

$$
\begin{align*}
B_0(X) &= 1, & B_1(X) &= X - \frac{1}{2}, & B_2(X) &= X^2 - X + \frac{1}{6}, \\
B_3(X) &= X^3 - \frac{3}{2}X^2 + \frac{1}{2}X, & B_4(X) &= X^4 - 2X^3 + X^2 - \frac{1}{30}.
\end{align*}
$$

### 5. 実数変数の写像に対する合成演算子

$\mathbf{R}$ 含む区間 $\mathbf{R}_+ = [0, +\infty[$ で I を区間とします。 E を体 $\mathbf{C}$ 上のベクトル空間とし、I で定義された複素数値を持つ実数変数の写像で形成されます。すべての $a \geqslant 0$ とすべての写像 $f \in E$ 写像 $x \mapsto f(x + a)$ 属するが E になると仮定します。さらに、複素数係数* と *指数関数* $e^{\lambda x}$ を含む *多項式の E 含む制限から I と仮定します。ここで、$\lambda$ は任意の *複素数* 数です。 I から複素数の体 $\mathbf{C}$ へのすべての写像の空間への E の線形写像 $U$ は、E の *演算子* と呼ばれます。 $f \in E$ と $g = U(f)$ の場合は記法を使用すると便利です

$$
g(x) = U_{\xi}^{\xi}(f(\xi))
$$

ここで、$\xi$ は、右辺項 (*cf.* II, p. 58) の関数記号における *ダミー* 変数です。 $a \geqslant 0$ ごとに、写像 $x \mapsto f(x + a)$ の制限 I を任意の写像 $f \in E$ に関連付ける演算子を、a* による * 変換演算子と呼びます。

#### 定義 3 {#fvr-vi-s1-def-3 .statement tag=08I3}

*すべての $a \geqslant 0$ について、a* による変換演算子で置換可能である場合、E 上の演算子 U は合成演算子であると言われます。

上で紹介した記法では、この定義がアイデンティティとなります。

$$
U_{x+a}^{\xi}(f(\xi)) = U_x^{\xi}(f(\xi + a))
$$

$x$ と $a$ ($x \in I, a \geqslant 0$) で。このアイデンティティで $x$ と $a$ の役割を交換できます。$x \geqslant 0$ の場合は、$a = 0$ を置きます。したがって、$x \geqslant 0$ が得られます

$$
U_x^{\xi}(f(\xi)) = U_0^{\xi}(f(\xi + x))
$$

ここで、$U_0$ は E の *線型形式* で、各写像 $f \in E$ が $g = U(f)$ の値 $g(0)$ に関連付けられます。

$f$ が多項式の場合、$f(\xi + x) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(\xi) x^k$ があり、式 (26) は $U(f)$ も多項式であることを示しています。 $x$ の多項式の集合、$\mathbf{C}$ の係数 (代数 $\mathbf{C}[X]$ で識別できる集合) に限定されている場合、演算子 $U$ は def の意味で合成演算子です。 I、VI、p. 270、および前のセクションのすべての結果を適用できます。

演算子 $U$ に関連付けられた Appell 多項式を再度 $u_n$ と書きます。多項式 (VI, p. 274, 公式 (13)) の一般化されたテイラー展開には対応する、より一般的な写像には、次の結果が得られます。

#### 定理 2 {#fvr-vi-s1-thm-2 .statement tag=08I4}

*f を I および所属での連続 $(n + 1)^{th}$ 微分を認め、$1 \leq m \leq n$ に対するすべての導関数 $f^{(m)}$ を E に認める写像とします。U が E 上の位数 $p \leq n$ の合成演算子である場合、$x \geq 0$ については次のようになります。 $h \geq 0$*

$$
f^{(p)}(x + h) = \sum_{m=0}^{n} \frac{1}{m!} u_m(x) U_h^\xi \left( f^{(m)}(\xi) \right) + R_n(x, h)
$$
(27)

と
$$
R_n(x, h) = -U_h^\xi \left( \int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta \right)
$$
(28)
*(一般化されたテイラー展開)*。

すべての $\xi \in I$ に対して定義された積分 $\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta$ を考えてみましょう。
そして、位数 $n + 1$ (II, p. 59, 公式 (11)) の部分による統合のために公式を適用します。 関係を考慮して
$$
u_n^{(k)} = n(n-1)\ldots(n-k+1)u_{n-k}
$$
(7) (VI, p. 273) から再帰的に導出され、次の結果が得られます。
$$
\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta
$$
$$
= \sum_{m=0}^{n} \frac{1}{m!} u_m(x) f^{(m)}(\xi) - \sum_{m=0}^{n} \frac{1}{m!} u_m(\xi - h) f^{(m)}(x + h).
$$
(29)

演算子 $U$ を (29) の両側に適用し、$\xi$ の写像とみなして、変数 $\xi$ の値 $h$ に対して得られた写像の値を取得します。式 (26) (VI, p. 277) と (9) (VI, p. 272) により、
$$
U_h^\xi (u_m(\xi - h)) = U_0^\xi (u_m(\xi)) = \begin{cases} 0 & \text{for } m \neq p \\ p! & \text{for } m = p \end{cases}
$$
最終的には (27) が得られます。

### 6. 合成演算子の指標

n° 5 と同じ仮説を使用すると、(VI, p. 277) の公式 (26) が写像 $e^{\lambda x}$ に適用され、次のようになります。
$$
U_\lambda^\xi (e^{\lambda \xi}) = U_0^\xi (e^{\lambda x} e^{\lambda \xi}) = e^{\lambda x} U_0^\xi (e^{\lambda \xi}) = u(\lambda) e^{\lambda x}
$$
(30)
$u(\lambda) = U_0^\xi (e^{\lambda \xi})$を装着中。 $\mathbf{C}$ で複素数値で定義された写像 $u(\lambda)$ は、合成演算子 $U$ の *指標* であると言われています。多項式の $U$ から環 $\mathbf{C}[X]$ の制限が系列に等しい場合に注意してください。
$$
D^p \sum_{n=0}^{\infty} \alpha_n D^n
$$
(VI, p. 271, th. 1) (VI, p. 271 で $u(D)$ と表しました)、一般的な項 $\alpha_n \lambda^{n+p}$ と *複素数項* の系列 *は必ずしも収束するわけではありません* $\lambda \neq 0$、そして、$\lambda$ の値に一定の収束があったとしても、和 *U* の屈折率関数* $u(\lambda)$ (VI、p. 291、演習 2) に必ずしも等しいわけではありません。 $\mathbf{C}$ に 0 の近傍が存在する場合、合成演算子 $U$ は *正規* であり、系列と一般的な項 $\alpha_n \lambda^{n+p}$ が *絶対収束* であり、 和 *指数関数に等しい* を持つとします。この近傍$^1$の$u(\lambda)$。 VI、p. 278の公式 (27)を写像 $e^{\lambda x}$に適用して、$h = 0$を作りましょう。 $D^m(e^{\lambda x}) = \lambda^m e^{\lambda x}$ からは $U_0^\xi \left( D^m(e^{\lambda x}) \right) = \lambda^m u(\lambda)$ になります。次に、すべての複素数 $\lambda$ について、 $u(\lambda) \neq 0$ が成り立つことがわかります。

$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{m=0}^n u_m(x) \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi-x} \frac{1}{n!} u_n(x+\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

特に $x = 0$ については

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{m=0}^n \beta_m \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi} \frac{1}{n!} u_n(\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

$\beta_m = u_m(0)$と。

$U$ が *正規* 演算子である場合、系列 $u(\lambda) = \sum_{n=0}^\infty \alpha_n \lambda^{n+p}$ と $\sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}$ が絶対収束$^2$ となるようなすべての $\lambda \in \mathbf{C}$ について、2 つの絶対収束する系列のうちの積については、公式 (16) と公式が続きます。 (*Gen.Top.*、VIII、p. 115、提案 1)

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}.
$$

同様に、$e^{\lambda x}$ のテイラー展開はすべての $\lambda \in \mathbf{C}$ とすべての $x \in \mathbf{C}$ (III, p. 106) について絶対収束するため、すべてについて (式 (6) (VI, p. 273) および (16) (VI, p. 274)) も成り立ちます。 値を考慮し、すべての$x \in \mathbf{C}$

$$
\frac{\lambda^n e^{\lambda x}}{u(\lambda)} = \sum_{n=0}^\infty u_n(x) \frac{\lambda^n}{n!}.
$$

#### 注意 {#fvr-vi-s1-n6-rem-1 .statement tag=08I5}

系列全体で次の補題を使用することで、公式 (33) (それぞれ (34)) を計算する $\beta_n$ (それぞれ $u_n(x)$) に使用できます。

(1) 後で、系列を学習します。その一般的な項は形 $c_n z^n$ ($c_n \in \mathbf{C}, z \in \mathbf{C}$) であり、これを *全体系列* と呼びます。特に、そのような系列が $z = z_0$ に対して完全に収束するとき、それは $|z| \leq |z_0|$ に対して *通常収束* することがわかります。
(2) 系列全体の理論から、これら系列の 1 つが 0 の近傍 $V$ に絶対収束するとき、もう一方は 0 の近傍 $W \subset V$ に絶対収束することがわかります。

エマ。 **2 つの全体系列** $\sum_{n=0}^{\infty} c_n \lambda^n,\ \sum_{n=0}^{\infty} d_n \lambda^n$ **すべてについて絶対に収束する** $\lambda$ **in 近傍 of** $0$、**そして if** $\sum_{n=0}^{\infty} c_n \lambda^n = \sum_{n=0}^{\infty} d_n \lambda^n$ **これらの値 of** $\lambda$、** そして** $c_n = d_n$ **すべてについて整数** $n \geqslant 0$。

何らかの手順によって、$0$の近傍で$\lambda^p / u(\lambda)$に収束する系列全体を見つけることができれば、この系列の係数は必然的に$\beta_n / n!$と等しくなります。この手順は、次の例で適用されます。

#### 例 1 {#fvr-vi-s1-n6-exa-1 .statement tag=08I6}

$U$ が同一性写像である場合、$u(\lambda) = 1$ があり、演算子 $U$ は明らかに単数です。 $u_n(x) = x^n$ 公式 (27) の VI, p. 278 は、$\xi = \xi - \eta$ を入れて書くことができます

$$
f(x + h) = \sum_{n=0}^{\infty} \frac{1}{m!} f^{(m)}(h) x^m + \int_h^{x+h} f^{(n+1)}(t) \frac{(x + h - t)^n}{n!} dt
$$

つまり、テイラー 公式 (II, p. 62) に対して簡約するです。

#### 例 2 {#fvr-vi-s1-n6-exa-2 .statement tag=08I7}

$\mathbf{R}_+$ で定義されたすべての写像 $f$ に写像 $x \mapsto f(x + 1) - f(x)$ を関連付ける $U$ 合成演算子を考えてみましょう。それから

$$
U_{\lambda}^{\xi} (f(\xi)) = f(x + 1) - f(x);
$$

(VI, p. 275) $U$ から $\mathbf{C}[X]$ の制限が $e^D - 1$ に等しいことが分かりました。一方、$u(\lambda) = e^{\lambda} - 1$ なので、演算子 $U$ は *正規* です。収束する全体系列として $\frac{\lambda}{e^{\lambda} - 1}$ の展開を計算することで、ベルヌーイ数 $b_n$ を決定する計算する方法 (VI, p. 288) を見てみましょう。 VI, p. 278 の適用公式 (27) から写像 $f$ の *原始関数* に対して、$\mathbf{R}_+$ での連続 $n^{th}$ 導関数を認めると、次のようになります。

$$
f(x + h) = \int_h^{h+1} f(t) dt
$$
$$
+ \sum_{m=1}^n \frac{1}{m!} B_m(x) \left( f^{(m-1)}(h+1) - f^{(m-1)}(h) \right) + R_n(x, h)
$$

と

この補題は一般的な結果の特殊なケースであり、後で証明します。こちらが証明です。 系列 $\sum_{n=0}^{\infty} c_n \lambda^n$ 全体が $\lambda = \lambda_0$ に絶対収束する場合、すべての整数 $k \geqslant 0$ 系列 $\sum_{n=0}^{\infty} c_{n+k} \lambda^n$ は通常 $|\lambda| \leqslant |\lambda_0|$ に収束するため、このディスク上では連続です (*Gen. Top.*, X、p. 283); $0$の近傍にある$\sum_{n=k+1}^{\infty} c_n \lambda^n = o(\lambda^k)$の結論する。次に、補題は、係数の一意性から、$\lambda^n$ (V、p. 223) の項における写像の漸近展開に続きます。

$$
R_n(x, h) = - \int_0^{1-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h + 1 - \eta) d\eta \\
+ \int_0^{-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h - \eta) d\eta.
$$

(36)

#### 例 3 {#fvr-vi-s1-n6-exa-3 .statement tag=08I8}

E を写像 $f$ のベクトル空間として定義し、$\mathbf{R}$ で連続し、積分 $\int_{-\infty}^{+\infty} f(x + \xi) e^{-\xi^2/2} d\xi$ がすべての $x \geq 0$ について収束するようにします。演算子 U は次のように定義されます。

$$
U_\lambda^\xi \left( f(\xi) \right) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} f(x + \xi) d\xi
$$

次に、 は E で定義され、明らかに合成演算子です。 空間 E 含むすべての指数 $e^{\lambda x}$ ($\lambda$ 任意の複素数)、および 1 つは

$$
u(\lambda) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-(\xi^2/2) + \lambda \xi} d\xi \\
= \frac{1}{\sqrt{2\pi}} e^{\lambda^2/2} \int_{-\infty}^{+\infty} e^{-(\xi - \lambda)^2/2} d\xi = e^{\lambda^2/2}
$$

(cf. III、p. 120、演習 24、および VII、p. 313、公式 (22))。 1 つは$n! \alpha_n = U_0^\xi (\xi^n) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \xi^n d\xi$ です。 整数 $n$ ごとに、次のことができます

$$
\sum_{k=0}^n \int_{-\infty}^{+\infty} \frac{|\lambda \xi|^k}{k!} e^{-\xi^2/2} d\xi \leq 2 \int_0^{+\infty} e^{-(\xi^2/2) + |\lambda| \xi} d\xi.
$$

従って、系列 $\sum_{n=0}^{\infty} e^{-\xi^2/2} \frac{(\lambda \xi)^n}{n!}$ は、$\mathbf{R}$ (II、p. 72、cor. 1) にわたって項ごとに積分できます。これは、系列 $\sum_{n=0}^{\infty} \alpha_n \lambda^n$ がすべての $\lambda \in \mathbf{C}$ に対して絶対に収束し、和が以下に等しいことを証明します。 $u(\lambda) = e^{\lambda^2/2} = \sum_{n=0}^{\infty} \frac{\lambda^{2n}}{2^n n!}$;従って、演算子 $U$ は正規です。上記の適用補題は、$n \geq 0$ ごとに $\alpha_{2n} = 1/2^n n!,\ \alpha_{2n+1} = 0$ になることを示しています。従って、演算子 $U$ は位数 0 になります。

$$
\frac{1}{u(\lambda)} = e^{-\lambda^2/2} = \sum_{n=0}^{\infty} \frac{(-1)^n \lambda^{2n}}{2^n n!},
$$

系列はすべての $\lambda \in \mathbf{C}$ に対して絶対に収束します。 他のを補題に適用すると、$\beta_{2n} = \frac{(-1)^n (2n)!}{2^n n!},\ \beta_{2n+1} = 0$ が示されます。さらに、系列 $\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x)$ はすべての $\lambda \in \mathbf{C}$ とすべての $x \in \mathbf{R}$ に対して絶対収束し、次の式が得られます。

$$
\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x) = \exp \left( -\frac{\lambda^2}{2} + \lambda x \right) = \exp \left( \frac{x^2}{2} \right) \exp \left( -\frac{1}{2} (\lambda - x)^2 \right).
$$

適用のテイラー 公式から写像 $\exp(-x^2/2)$ では、多項式 $u_n(x)$ について次の式が得られます。

$$
u_n(x) = (-1)^n e^{\lambda^2/2} \frac{d^n}{dx^n} (e^{-x^2/2}).
$$

この多項式は、次数 $n$ の *エルミート多項式* と呼ばれ、多くの場合、$\mathrm{H}_n(x)$ で表されます。ここで、VI、p. 273 の式 (7)、(8)、(9) は次のようになります。

$$
\frac{d \mathrm{H}_n}{dx} = n \mathrm{H}_{n-1}(x)
$$

$$
\mathrm{H}_n(x+y) = \sum_{k=0}^n \binom{n}{k} \mathrm{H}_{n-k}(x) y^k
$$

$$
\frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \mathrm{H}_n(x+\xi) d\xi = x^n
$$

そして、VI, p. 278 の公式 (27) は、$h = 0$ に対して、

$$
\sqrt{2\pi} f(x) = \sum_{m=0}^n \left( \int_{-\infty}^{+\infty} e^{\xi^2/2} f^{(m)}(\xi) d\xi \right) \frac{\mathrm{H}_m(x)}{m!}
$$
$$
- \int_{-\infty}^{+\infty} d\xi \int_0^\xi \frac{\mathrm{H}_n(x+\eta)}{n!} e^{-(\xi+\eta)^2/2} f^{(n+1)}(x+\xi-\eta) d\eta.
$$

### 7. オイラーとマクローリンの和公式

VI、p. 280 の公式 (35) では、置き換える $x$ を 0 で、$h$ を $x$ で計算します。 $\mathrm{B}_m(0) = b_m$ から、VI、p. 276 の関係 (24) から、各整数 $p > 0$ について次のように書くことができます。

$$
f(x) = \int_x^{x+1} f(t) dt - \frac{1}{2} (f(x+1) - f(x))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+1) - f^{(2k-1)}(x) \right) + R_p(x)
$$
と
$$
R_p(x) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) f^{(2p+1)}(x+1-t) dt.
$$
この公式では、置き換える $x$ $x+1, x+2, \ldots, x+n$ を順に実行し、得られた式を 1 つずつ組み合わせてみましょう。私たちは得る

$$
\begin{cases}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t) dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x) \right) + T_p(x, n)
\end{cases}
$$
と
$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) \left( \sum_{k=0}^n f^{(2p+1)}(x+k+1-t) \right) dt.
$$

この公式の余り $T_p(x, n)$ は次の方法で書き換えることができます: 区間 $[0, 1[$ の $B_{2p+1}(t)$ に等しい、周期 1 を持つ *周期* 写像を $\overline{B}_{2p+1}(t)$ で表します。それから

$$
\int_0^1 B_{2p+1}(t) f^{(2p+1)}(x + k + 1 - t) \, dt = \int_k^{k+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) \, ds
$$

そしてその結果として

$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) ds.
$$ (41)

公式 (39) は *オイラー-マクローリン和公式* と呼ばれます。これは、区間 $[x_0, +\infty[$ 上の連続導関数 $(2p + 1)^{th}$ を持つすべての複素数写像 、すべての $x \geq x_0$ に適用できます。この公式の *余り* $T_p(x, n)$ を推定する方法 (VI, p. 288) を見てみましょう。

### 練習問題 {#fvr-vi-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
