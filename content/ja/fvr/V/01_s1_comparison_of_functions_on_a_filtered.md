---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 1
section_title: COMPARISON OF FUNCTIONS ON A FILTERED SET
lang: ja
source: fvr-i-vii
book_pages: 211-220
pdf_pages: 0226-0235, 0274-0274
extraction: ocr
subsections:
    - "no": 1
      title: 'COMPARISON RELATIONS: I. WEAK RELATIONS'
      page: 211
      pdf_page: 226
    - "no": 2
      title: 'COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 214
      pdf_page: 229
    - "no": 3
      title: CHANGE OF VARIABLE
      page: 217
      pdf_page: 232
    - "no": 4
      title: COMPARISON RELATIONS BETWEEN STRICTLY POSITIVE FUNCTIONS
      page: 217
      pdf_page: 232
    - "no": 5
      title: NOTATION
      page: 219
      pdf_page: 234
statements: 38
exercises: 3
content_sha256: 305117d45e89d0153dd1c77592548de0281c1cd31932c6e7e31b48dda5f1660b
translated_from: content/en/fvr/V/01_s1_comparison_of_functions_on_a_filtered.md
translation_method: google
source_content_sha256: 8313e76e55f08fcd7dd783b09028bd3331bcb51b6229df45213a85cc59097f4a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 96191e8d9af4807218864924f793d44a223f730a807765fa706e938cfa103dcf
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 写像とフィルタリングされた集合の比較

E を基底 $\mathfrak{F}$ (*Gen.Top.*、I、p. 58) のフィルターで集合フィルターにかけます。この章では、フィルター 基底 $\mathfrak{F}$ (写像に応じて部分集合) に対する定義のドメインが E 所属の部分集合であり、その値を次のいずれかに取る写像を考えます。 実数 $\mathbf{R}$ の体、またはより一般的には、価値のある体 (*Gen. Top.*、IX、p. 170) を上回る標準のベクトル空間です。

アプリケーションでは、E は、ほとんどの場合、実数空間 $\mathbf{R}^n$ の部分空間、または延長線 $\overline{\mathbf{R}}$ であり、$\mathfrak{F}$ は、E の閉包点の近傍のフィルターの E 上のトレース、または E の比較的コンパクトな部分集合の補数のフィルターになります。 (「無限遠の点の近傍」)。

一般に、そのような写像が $\mathfrak{F}$ に沿った特定の極限に向かう傾向があり、この写像から形成される式の「$\mathfrak{F}$ に沿った極限への通過」のすべての問題を処理できることを知るだけでは十分ではありません。

たとえば、実変数 x が $+\infty$ になる傾向がある場合、3 つの写像 $x$、$x^2$、$\sqrt{x}$ はすべて $+\infty$ になる傾向がありますが、式の

$$
(x+1)^2 - x^2, \quad (x+1) - x, \quad \sqrt{x+1} - \sqrt{x},
$$

1 つ目は $+\infty$、2 つ目は 1、3 つ目は 0 になる傾向があります。

したがって、$\mathfrak{F}$ (この極限が存在する場合) に沿った写像の極限値だけでなく、写像がその極限に近づく「方法」も知ることが重要です。他の語では、同じ極限の傾向がある写像の集合を分類することになります。

### 1. 関係: I の比較。弱い関係

以下では、値フィールド K 上のノルム化ベクトル空間を V で表し、V の値を持つ関数のセットを $\mathscr{H}(\mathfrak{F}, V)$ で表します。各関数はフィルター ベース $\mathfrak{F}$ に属する E のサブセットで定義されます。 このような関数間で定義する関係は、ベース $\mathfrak{F}$ を持つフィルターに対して *ローカル* 特性を持ちます。これが何を意味するのかを明確にしましょう。 f と g が $\mathscr{H}(\mathfrak{F}, V)$ から 2 つの写像である場合、関係 「f と g が定義され、Z 上で等しいような集合 $Z \in \mathfrak{F}$ がある」は、$\mathscr{H}(\mathfrak{F}, V)$ 上の *同値関係 $R_\infty$ であることを思い出してください。 トップ。*、I、p. 66)。 そうなると、$\mathscr{H}(\mathfrak{F}, V)$ の写像 $f$ を含む関係 S は、同値関係 $R_\infty$ と *互換性* ($f$ で) ある場合、$f$ に対して *ローカル* 指標 ($\mathfrak{F}$ に沿って) であると言えます。 (*集合理論*、II、p. 117); $\tilde{f}$ が $\mathfrak{F}$、$R_\infty$ を法とする $f$ の同値類 (商集合 $\mathscr{H}_\infty(\mathfrak{F}, V) = \mathscr{H}(\mathfrak{F}, V)/R_\infty$ の元) に沿った $f$ の *胚芽* である場合、次のように S から導出できることがわかります。 $\tilde{f}$ と S の他の引数の間の商、関係、そして逆に、$f$ に対するローカル指標のこの性質のすべての関係定義する関係。

#### 例 {#fvr-v-s1-n1-exa-5 .statement tag=08DN}

$f$と$g$が$\mathscr{H}(\mathfrak{F}, \mathbf{R})$の2つの写像である場合、関係「$t \in X$ごとに$X$と$f(t) \leq g(t)$に$f$と$g$が定義されるような$X \in \mathfrak{F}$がある」はローカルのものです。 $f$ および $g$ に対する指標。 移行から商によって得られる $\tilde{f} \leq \tilde{g}$ 関係 ($f$ と $g$ の場合) で表します。 $\tilde{f} \leq \tilde{g}$ の場合、E の *すべて* で定義された写像 $f_1 \in \tilde{f}$ と写像 $g_1 \in \tilde{g}$ が存在し、すべての $t \in E$ に対して $f_1(t) \leq g_1(t)$ となることに注意してください。

#### 注意 {#fvr-v-s1-n1-rem-3 .statement tag=0E5L}

1) $V_i$ ($1 \leq i \leq n$) を K に対してベクトル空間でノルム化した $n$ とし、$V_1 \times V_2 \times \cdots \times V_n$ で値をV に定義して$\varphi$ 写像とします。 $R_\infty$ 写像 $\varphi$ 定義する写像沿いに移行から商まで
$$
\mathscr{H}_\infty(\mathfrak{F}, V_1) \times \cdots \times \mathscr{H}_\infty(\mathfrak{F}, V_n)
$$
$\mathscr{H}_\infty(\mathfrak{F}, V)$ に変換され、最も多くの場合、$\varphi(\tilde{f}_1, \ldots, \tilde{f}_n)$ で表されます (*Gen. トップ。*、I、p. 67)。 たとえば、$\varphi$ を写像 $(x, y) \mapsto x + y$ および $x \mapsto x\lambda$ ($\lambda \in K$) とすると、$\mathscr{H}_\infty(\mathfrak{F}, V)$、元 $\tilde{f} + \tilde{g}$、$\tilde{f}\lambda$ の任意の 2 つの細菌 $\tilde{f}, \tilde{g}$ について、1 つは定義するとなり、すぐに検証されます。 $\mathscr{H}_\infty(\mathfrak{F}, V)$ 上の合成 $(\tilde{f}, \tilde{g}) \mapsto \tilde{f} + \tilde{g}$ と $(\lambda, \tilde{f}) \mapsto \tilde{f}\lambda$ 定義するのルールは体 K を超える *ベクトル空間* 構造です。この空間 $\tilde{O}$ は、$\mathfrak{F}$ の集合に 0 に等しい写像によって形成された類であり、$-\tilde{f}$ は、$-f$ に等しい写像によって形成された類です。 $\mathfrak{F}$の集合。 同様に、V が K 上の *代数* である場合、$\mathscr{H}_\infty(\mathfrak{F}, V)$ 上の 1 つの定義するは、$\varphi(x, y) = xy$ を取ることで合成 $(\tilde{f}, \tilde{g}) \mapsto \tilde{f}\tilde{g}$ の 2 番目の内部規則になります。前述の 2 つのルールと組み合わせると、この定義するは $\mathscr{H}_\infty(\mathfrak{F}, V)$ の K に対する *代数* 構造になります。 V に単位元 e がある場合、$\mathscr{H}_\infty(\mathfrak{F}, V)$ は、$\mathfrak{F}$ の一部の集合で e に等しい写像によって形成される単位元類 $\tilde{e}$ になります。 $\tilde{f}$が$\mathscr{H}_\infty(\mathfrak{F}, V)$で*反転可能であるためには、一部の$f \in \tilde{f}$に対して、$t \in Z$ごとに$f(t)$がVで反転可能であるような$Z \in \mathfrak{F}$が存在することが必要かつ十分である（この場合、この条件はすべての写像によって満たされる） 類 $\tilde{f}$）。

2) 同じ記法で、$\psi$を$\prod_{i=1}^n V_i$の部分集合の写像をVとします。 $f_i(t)$ が定義されている点 $t \in E$ および $\psi$ が定義されている点 $(f_i(t))$ 属するから集合ごとに $\psi(f_1(t), f_2(t), \ldots, f_n(t))$ に等しい $\psi(f_1, f_2, \ldots, f_n)$ 写像で表します。 $^1$。たとえば、$f$ と $g$ が両方とも定義されている場合、$f + g$ は点 $t \in E$ ごとに写像と $f(t) + g(t)$ に等しくなります。 $f$ がすべての E で定義されていない場合、$f + g = 0$ のような写像 $g \in \mathscr{H}(\mathfrak{F}, V)$ は存在しないため、$\mathscr{H}(\mathfrak{F}, V)$ では写像 $(f, g) \mapsto f + g$ *が群法則* ではないことに注意してください。

#### 定義 1 {#fvr-v-s1-def-1 .statement tag=08DO}

*2 つの実数写像* $f, g$ *所属から* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ が与えられ、*これらは* $\geq 0$ *集合の* $\mathfrak{F}$、*$f$ *が支配的* $g$、*またはそれ* $g$ *優勢* $f$ *($\mathfrak{F}$*に沿って*)、* $f \preceq g$ *または* $g \succeq f$、*集合* $X \in \mathfrak{F}$ *と数* $k > 0$ *そのような* $f(t) \leq k\ g(t)$ *すべて* $t \in X$ *(他の語に* $k > 0$ *そのような* $\tilde{f} \leq k\ \tilde{g}$ が存在する場合)

$^1$ 特に、以下のすべてにおいて、$\mathscr{H}(\mathfrak{F}, V)$ の写像 $f$ が与えられた場合、属するから $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ までを$\|f\|$ 写像 $t \mapsto \|f(t)\|$ で表し、$f$ と同じ集合で定義します。この章 $\|f\|$ は *数* ではなく *写像* であるという事実に明確に注意してください。

2 つの正規化ベクトル空間 $V_1, V_2$ と、2 つの写像 $f_1, f_2$ 所属がそれぞれ $\mathscr{H}(\mathfrak{F}, V_1)$ と $\mathscr{H}(\mathfrak{F}, V_2)$ であるとすると、$f_1$ は ($\mathfrak{F}$ とともに) $f_2$ によって支配されていると言い、$f_1 \preccurlyeq f_2$ と書きます。 $\|f_1\| \preccurlyeq \|f_2\|$の場合は、$f_2 \succeq f_1$。

関係 $f_1 \preccurlyeq f_2$ は明らかに $f_1$ と $f_2$ のローカル指標です。したがって、これは、移行から商によって導出される関係 $\tilde{f}_1 \preccurlyeq \tilde{f}_2$ と等価です。 $f$ と $g$ が実際の写像である場合、関係 $\tilde{f} \preccurlyeq \tilde{g}$ と $\tilde{f} \leq \tilde{g}$ を混同しないように注意する必要があります。

すべてのスカラー $\lambda \neq 0$ 関係 $f_1 \preccurlyeq f_2 \lambda$ は $f_1 \preccurlyeq f_2$ と *同等* であることに注意してください。 $f_1 \preccurlyeq f_2$ の場合、$f_2(x) = 0$ の点 $x \in X$ ごとに $f_1(x) = 0$ となる集合 $X \in \mathfrak{F}$ が存在します。

#### 例 {#fvr-v-s1-n1-exa-6 .statement tag=0E5I}

1) 関係 $f \preccurlyeq 1$ は、$f$ が $\mathfrak{F}$ の集合で *境界がある* ことを意味します。

2) $\mathscr{H}(\mathfrak{F}, V)$ のすべての写像 $f$、およびすべてのスカラー $\lambda \neq 0$ に対して、1 つは $f \preccurlyeq f \lambda$ を持ちます。
3) $x$ が $+\infty$ になる傾向があるときは、$\sin^2 x \preccurlyeq \sin x$ になります。
4) $(x, y)$ が $\mathbf{R}^2$ で $(0, 0)$ になる傾向があるとき、人は
$$
xy \preccurlyeq x^2 + y^2.
$$

次の命題はdefの明らか帰結です。 1:

#### 命題 1 {#fvr-v-s1-prop-1 .statement tag=08DP}

*もし* $f, g, h$ * $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ に写像が 3 つある場合 * 関係* $f \preccurlyeq g$ * そして* $g \preccurlyeq h$ * $f \preccurlyeq h$ を * 暗示します。

#### 命題 2 {#fvr-v-s1-prop-2 .statement tag=08DQ}

*$f_1, f_2$ *2 写像を * $\mathscr{H}(\mathfrak{F}, V)$ * と* $g$ *写像を * $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ とします。 *関係* $f_1 \preccurlyeq g$ *そして* $f_2 \preccurlyeq g$ *暗示* $f_1 + f_2 \preccurlyeq g$。

さらに:

#### 命題 3 {#fvr-v-s1-prop-3 .statement tag=08DR}

*$V_1, V_2, V$ *同じ値体* で 3 つの正規化空間とし、$(x, y) \mapsto [x.y]$ * $V_1 \times V_2$ *から * $V$ に *双線形写像とします。 *もし* $f_1$ *と* $f_2$ *が写像に* $\mathscr{H}(\mathfrak{F}, V_1)$ *そして* $\mathscr{H}(\mathfrak{F}, V_2)$ *それぞれ、そして* $g_1, g_2$ *2つの写像が* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ *そのような* $f_1 \preccurlyeq g_1$ *そして* $f_2 \preccurlyeq g_2$ *その後* $[f_1.f_2] \preccurlyeq g_1 g_2$。

確かに (*Gen. Top.*, IX, p. 173, th. 1) 次のような数 $a > 0$ が存在します。
$$
|[f_1.f_2]| \leq a \|f_1\| \|f_2\|.
$$

#### 系 {#fvr-v-s1-n1-cor-1 .statement tag=08DS}

*場合* $V$ *が正規の代数*である場合、*場合* $f_1, f_2$ *$\mathscr{H}(\mathfrak{F}, V)$に2つの写像がある*、*および* $g_1, g_2$ *$\mathscr{H}(\mathfrak{F}, \mathbf{R})$に2つの写像がある場合、*その後、関係* $f_1 \preccurlyeq g_1, f_2 \preccurlyeq g_2$ *暗示* $f_1 f_2 \preccurlyeq g_1 g_2$。

$\mathscr{H}(\mathfrak{F}, V)$ の写像の間の関係 $f \preccurlyeq g$ は、prop により *推移的* です。 1; *再帰的* 関係 "*f \preccurlyeq g and g \preccurlyeq f*" は、$\mathscr{H}(\mathfrak{F}, V)$ 上の *同値関係* (*集合理論*, II, p. 113) であるため。

#### 定義 2 {#fvr-v-s1-def-2 .statement tag=08DT}

*2 つの写像* $f, g$ *of* $\mathscr{H}(\mathfrak{F}, V)$ *私たちは、* $f$ * と* $g$ * は ($\mathfrak{F}$ に沿って*) 似ていると言い、 *そして書きます* $f \simeq g$、 *if* $f \preccurlyeq g$ *and* $g \preccurlyeq f$。

すべてのスカラー $\lambda \neq 0$ 関係 $f \simeq g$ は $f \simeq g \lambda$ と同等です。 これは、$f(x) = 0$ の点の$X$ のサブセットが $g(x) = 0$ の点の $X$ のサブセットと同一であるような集合 $X \in \mathfrak{F}$ の存在を意味します。

#### 例 1 {#fvr-v-s1-n1-exa-1 .statement tag=08DU}

実際の写像 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ 関係 $f \simeq 1$ は、2 つの数 $a > 0,\ b > 0$ があり、$\mathfrak{F}$ の集合に $a \leq |f(x)| \leq b$ があるか、写像 $\log |f|$ が境界にあることを意味します。 $\mathfrak{F}$の集合: 次に、$f$は$\mathfrak{F}$の集合で*対数的に制限されている*と言います。

#### 例 2 {#fvr-v-s1-n1-exa-2 .statement tag=08DV}

$V$ を非離散値体 $K$ に対するノルム空間とし、$f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ を変数 $x \in K$ の多項式とし、$V$ に係数が含まれる、$a_0 \neq 0$ となるようにします。 ベクトル $b \neq 0$ ごとに $f(x) \simeq b x^n$ があり、$|x|$ は $+\infty$ になる傾向があります。

#### 例 3 {#fvr-v-s1-n1-exa-3 .statement tag=08DW}

$x$ として $\sin^2 x \preccurlyeq \sin x$ は $+\infty$ になる傾向があることがわかりましたが、*私たちには $\sin^2 x \simeq \sin x$ がありません*、さらにはけれどもこれらの写像が同時に点で消滅します。

#### 例 4 {#fvr-v-s1-n1-exa-4 .statement tag=08DX}

$(x,\ y)$ が $\mathbf{R}^2$ で $(0,\ 0)$ になる傾向があるとき、$x^2 + xy + y^2 \simeq x^2 + y^2$ がありますが、$xy \simeq x^2 + y^2$ には*なりません*。

prop の直後に続きます。 V、p. 213 の 3、つまり $f_1,\ f_2,\ g_1,\ g_2$ が $\mathscr{H}(\mathfrak{F}, K)$ の写像 ($K$ は任意の値体) である場合、関係 $f_1 \simeq g_1$ と $f_2 \simeq g_2$ は $f_1 f_2 \simeq g_1 g_2$ を意味します。

対照的に、関係 $f_1 \simeq g_1$ と $f_2 \simeq g_2$ は、例 $f_1(x) = g_1(x) = x^2,\ f_2(x) = -(x^2 + x),\ g_2(x) = -(x^2 - 1)$ で示されているように、実際の変数 $x$ が $+\infty$ になる傾向があるため、*$f_1 + f_2 \simeq g_1 + g_2$ を意味するものではないことに注意します。

比較関係 $f \preccurlyeq g,\ f \simeq g$ は *弱い* と言われます。 $\mathscr{H}(\mathfrak{F}, V)$ の 2 つの写像 $f,\ g$ は、関係 $f \preccurlyeq g,\ g \preccurlyeq f$ の 1 つ (少なくとも) 満たすであれば *弱比較* できると言います。

#### 注意 1 {#fvr-v-s1-n1-rem-1 .statement tag=08DY}

写像 1 と $x \sin x$ の例が示すように、$x$ は $+\infty$ になる傾向があるため、$\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の 2 つの写像は弱比較である必要はありません。

#### 注意 2 {#fvr-v-s1-n1-rem-2 .statement tag=08DZ}

$\mathscr{H}(\mathfrak{F}, V)$ では $R_0$ 関係 $f \simeq g$ で表し、$\mathscr{H}_0(\mathfrak{F}, V)$ 商集合 $\mathscr{H}(\mathfrak{F}, V)/R_0$ で表します。 関係 $R$ *暗黙* $R_0$ に注意してください。 移行から商関係 $f \preccurlyeq g$ は、prop によって与えられます。 V、p. 213、$\mathscr{H}_0(\mathfrak{F}, V)$ の *位数関係* (*集合理論*、III、p. 134) の 1 つ。前の例は、$\mathscr{H}_0(\mathfrak{F}, V)$ がこの関係によって *完全に順序付けされていない* ことを示しています。

### 2. 比較関係:II。強い関係

#### 定義 3 {#fvr-v-s1-def-3 .statement tag=08E0}

*2 つの実数写像* $f,\ g$ *所属から* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ が与えられ、 *これらは * $\geq 0$ * $\mathfrak{F}$ の集合で、 *1 人は * $f$ * は $g$ に比べて無視できると言い、 * またはそれ* $g$ *が優勢* $f$ *(とともに* $\mathfrak{F}$)、*そして人は* $f \ll g$ *または* $g \gg f$ *すべて* $\varepsilon > 0$に対して、*集合* $X \in \mathfrak{F}$ *が存在する場合* $f(t) \leq \varepsilon g(t)$ *すべて* $t \in X$。

*2 つの正規化空間* $V_1,\ V_2$ * と 2 つの写像* $f_1,\ f_2$ *所属から* $\mathscr{H}(\mathfrak{F}, V_1)$ * と* $\mathscr{H}(\mathfrak{F}, V_2)$ *それぞれ、ある人は* $f_1$ * は$f_2$ と比べて無視できると言います。 *($\mathfrak{F}$に沿って)、*そして人は* $f_1 \ll f_2$ *または* $f_2 \gg f_1$、*場合* $\|f_1\| \ll \|f_2\|$と書きます。

すべてのスカラー $\lambda \neq 0$ 関係 $f_1 \ll f_2 \lambda$ は $f_1 \ll f_2$ と *同等* です。 関係 $f_1 \ll f_2$ は $f_1 \preccurlyeq f_2$ を暗示しますが、それと同等ではありません。

関係 $f_1 \preccurlyeq f_2$ は決して関係 「$f_1 \ll f_2$ または $f_1 \asymp f_2$」を意味するものではないことに注意してください。$x$ は $+\infty$ になる傾向があるため、$\sin x \preccurlyeq 1$ になりますが、関係 $\sin x \ll 1$ または$\sin x \asymp 1$は本当です。

#### 例 {#fvr-v-s1-n2-exa-8 .statement tag=0E5N}

1) 関係 $f \ll 1$ は、$f$ *$\mathfrak{F}$* に沿って 0 になる傾向があることを意味します。

2) $\alpha$ と $\beta$ が 2 つの実数であるとき、$\alpha < \beta$ は $x$ が $+\infty$ になる傾向があるため、1 つは $x^\alpha \ll x^\beta$ になります。同様に、$m$ と $n$ が 2 つの有理数整数である場合、$m < n$ は複素数として $z^m \ll z^n$ を持ち、$z$ は $\infty$ になる傾向があります。

3) $x$ は $+\infty$ になる傾向があるため、整数 $n$ (III、p. 105) ごとに $x^n \ll e^x$ になります。

4) $\mathbf{R}^2$ には、$(x, y)$ が $(0, 0)$ になる傾向があるように、
$$
x^2 + y^2 \ll |x| + |y|.
$$

次の命題は def からすぐに推測できます。 3:

#### 命題 4 {#fvr-v-s1-prop-4 .statement tag=08E1}

*$f, g, h$ が $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の 3 つの写像である場合、関係 $f \preccurlyeq g$ と $g \ll h$ (それぞれ $f \ll g$ と $g \preccurlyeq h$) は $f \ll h$ を意味します。

#### 命題 5 {#fvr-v-s1-prop-5 .statement tag=08E2}

※$f_1, f_2$を$\mathscr{H}(\mathfrak{F}, V)$の写像と$\mathscr{H}(\mathfrak{F}, \mathbf{R})$の$g$写像を2つとします。次に、関係 $f_1 \ll g$ と $f_2 \ll g$ は $f_1 + f_2 \ll g$ を暗示します。*

また、prop と同じ引数。 V、p. 213 の 3 は次のことを示しています。

#### 命題 6 {#fvr-v-s1-prop-6 .statement tag=08E3}

※支柱記法付き。 3、関係 $f_1 \ll g_1$ および $f_2 \preccurlyeq g_2$ (それぞれ $f_1 \preccurlyeq g_1$ および $f_2 \ll g_2$) は $[f_1.f_2] \ll g_1g_2$ を意味します。*

提案 4 は、$\mathscr{H}(\mathfrak{F}, V)$ の写像の間の関係 $f \ll g$ が *推移的*であることを示しています。しかし *これは再帰的ではありません*: 正確に言うと、関係 $f \ll f$ は、$f$ *$\mathfrak{F}$* の集合で消えることを意味します (他の語では、$f$ は 0 モジュロ $R_\infty$ と同等です)。実際、$0 < \varepsilon < 1$ のような $\varepsilon$ に対して、$x \in X$ ごとに $\|f(x)\| \leq \varepsilon \|f(x)\|$ となるような $X \in \mathfrak{F}$ が存在します。これは、$x \in X$ ごとに $f(x) = 0$ である場合にのみ可能です。したがって、関係 "f \ll g and g \ll f" は推移的かつ対称ですが、再帰的ではありません。したがって、同値関係ではありません (すべての $x \in X$ に対して $f(x) = g(x) = 0$ となるような集合 $X \in \mathfrak{F}$ が存在することを意味します)。

#### 命題 7 {#fvr-v-s1-prop-7 .statement tag=08E4}

*$f$と$g$が$\mathscr{H}(\mathfrak{F}, V)$の2つの写像である場合、関係$f - g \ll f$は$f - g \ll g$と同等です。

実際、$f - g \ll f$ は、$\varepsilon > 0$ ごとに $X \in \mathfrak{F}$ が存在し、$x \in X$ ごとに $\|f(x) - g(x)\| \leq \varepsilon \|f(x)\|$ が存在することを意味します。しかしその後、$(1 - \varepsilon) \|f(x)\| \leq \|g(x)\|$、その結果、$f \preccurlyeq g$、よって (V、p. 215、提案 4) $f - g \ll g$ になります。

#### 系 {#fvr-v-s1-n2-cor-1 .statement tag=08E5}

*関係 $f - g \ll f$ は $\mathscr{H}(\mathfrak{F}, V)$ の同値関係です。*

確かに、$f - g \ll f$ と $g - h \ll g$ の場合、$f - g \ll g$、よって (V、p. 215、提案 5) $f - h \ll g$、その結果、$g \preceq f$ 以降、$f - h \ll f$ となり、これは次のことを示しています。 関係は推移的です。プロップによって対称になっています。 7、そして明らかに反射的です、よって系。

#### 定義 4 {#fvr-v-s1-def-4 .statement tag=08E6}

*2 つの写像* $f, g$ *of* $\mathscr{H}(\mathfrak{F}, V)$ が与えられたとき、*1 人は、* $f$ * と* $g$ * は ($\mathfrak{F}$ に沿って) 同等であると言い、 * $f \sim g$、*if* $f - g \ll f$ と書きます。

関係 $f \sim g$ は $f \asymp g$ を暗示しますが、それと同等ではありません。

#### 例 1 {#fvr-v-s1-n2-exa-1 .statement tag=08E7}

$a$が定数写像、$E$の$\neq 0$、関係 $f \sim a$は、$f$が$\mathfrak{F}$に*沿って*$a$になる傾向があることを意味します。

#### 例 2 {#fvr-v-s1-n2-exa-2 .statement tag=08E8}

$V$ を非離散値体 $K$ に対するノルム空間とし、$f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ を変数 $x \in K$ の多項式とし、$V$ に係数が含まれる、$a_0 \neq 0$ となるようにします。次に、$|x|$ は $+\infty$ になる傾向があるため、$f(x) \sim a_0 x^n$ になります。

#### 例 3 {#fvr-v-s1-n2-exa-3 .statement tag=08E9}

実数 $x$ が $+\infty$ になる傾向があるとき、人は $\left( 1 + \frac{1}{x} \right) \sin x \sim \sin x$ になります。

#### 例 4 {#fvr-v-s1-n2-exa-4 .statement tag=08EA}

複素変数 $z$ は 0 になる傾向があるため、$e^z - 1 \sim z$ になります。より一般的には、$V$ が値体 $K$ に対する正規化空間であり、$f$ が $x_0 \in K$ の近傍で定義された写像で、$V$ に値が含まれ、微分を認める場合、 $f'(x_0) \neq 0$ 点 $x_0$ では、$x$ が $x_0$ に近づくと、$f(x) - f(x_0) \sim f'(x_0)(x - x_0)$ (I、p. 3、def. 1) になります。

#### 例 5 {#fvr-v-s1-n2-exa-5 .statement tag=08EB}

$(x, y)$ が $\mathbf{R}^2$ の $(0, 0)$ に近づくと、
$$
\sqrt{\sin^2 x + \sin^2 y} \sim \sqrt{x^2 + y^2}.
$$

#### 例 6 {#fvr-v-s1-n2-exa-6 .statement tag=08EC}

$f(x, y)$ を、定数項を持たない、2 つの実数変数 $x, y$ の実数係数を持つ多項式とします。 $> 0$ が残ったまま $x$ が 0 に近づくと、区間 $[0, a]$ で連続する写像 $\varphi(x)$ があり、$0 \leq x \leq a$ に対して $\varphi(0) = 0$ と $f(x, \varphi(x)) = 0$ が存在する場合、合理的な関係があることを示すことができます。 数 $r$ と実数 $\lambda \neq 0$ は $\varphi(x) \sim \lambda x^r$ になります (V、p. 259、演習 3)。

#### 例 7 {#fvr-v-s1-n2-exa-7 .statement tag=08ED}

すべての $x > 0$ について、$\pi(x)$ は $\leq x$ である素数数の数を表します。 $\pi(x) \sim x / \log x$ $^2$ と $x$ は $+\infty$ になる傾向があることが証明されています。

#### 注意 {#fvr-v-s1-n2-rem-3 .statement tag=08EE}

関係 $f \sim g$ は、$f - g$ の差が $\mathfrak{F}$ に沿って 0 になる傾向があることを決して意味するものではないことに注意してください。 $x$ が $+\infty$ になる傾向があるのに対し、例 $x^2 + x \sim x^2$ で示されているように、この差は *無制限* になることもあります。

#### 命題 8 {#fvr-v-s1-prop-8 .statement tag=08EF}

*$K$ *を値体とし、* $f_1, f_2, g_1, g_2$ *4 つの写像を * $\mathscr{H}(\mathfrak{F}, K)$ とします。 *その後、関係* $f_1 \sim g_1$ *そして* $f_2 \sim g_2$ *暗示* $f_1 f_2 \sim g_1 g_2$。

確かに、私たちは $f_1 f_2 - g_1 g_2 = f_1 (f_2 - g_2) + (f_1 - g_1) g_2$ を持っています。 $f_1 \preceq g_1$、$f_1 - g_1 \ll g_1$、$f_2 - g_2 \ll g_2$ なので、$f_1 f_2 - g_1 g_2 \ll g_1 g_2$ (V、p. 215、提案 5 と 6) になります。

対照的に、V, p. 214 で例を与えましたが、$f_1 = g_1$, $f_2 \sim g_2$ はありますが、関係 $f_1 + f_2 \asymp g_1 + g_2$ は成り立ちません (つまり、*なおさら* も成り立ちません)
$$
f_1 + f_2 \sim g_1 + g_2).
$$
2 たとえば、A. E. INGHAM、*distribution of prime 数* (Cambridge Tracts、n 30)、Cambridge University Press、1932 年を参照。

比較関係 $f \ll g, f \sim g$ は強い関係と呼ばれます。 $\mathscr{H}(\mathfrak{F}, V)$ の 2 つの写像 $f, g$ は、満たす 3 つの関係: $f \ll g, f \gg g$ の 1 つである場合、または「$f \sim g\lambda$ となるような $\lambda \neq 0$ が存在する」場合、比較可能 (または、考えられる混乱を避けたい場合は強く比較可能) と呼ばれます。

#### 注意 1 {#fvr-v-s1-n2-rem-1 .statement tag=08EG}

2 つの写像は弱く比較できますが、けれどもは強く比較できません。たとえば、写像 1 と $\sin x$ は、$x$ が $+\infty$ になる傾向があるためです。

#### 注意 2 {#fvr-v-s1-n2-rem-2 .statement tag=08EH}

空間 $V_1, V_2$ 上の関係 $f_1 \preccurlyeq f_2$ と $f_1 \ll f_2$ ノルムの定義では、$f_1$ と $f_2$ はそれぞれ値をとりますが、明らかに関係しているだけです。実際には、$V_1$ と $V_2$ のトポロジのみが関係します。$V_1$ または $V_2$ 上の 1 つの置き換えるノルムが同等のものによって置き換えられると、関係 $f_1 \preccurlyeq f_2$ と $f_1 \ll f_2$ は同等のもの関係に置き換えられます。 ノルム (\emph{将軍トップ}、IX、p. 170、デフォルト 7)。

### 3. 変数の変更

$\varphi$ を集合 $E'$ から $E$ への写像とし、$\varphi^{-1}(\mathfrak{F})$ が $E'$ のフィルター 基底となるようにします。 $f_1, f_2$ がそれぞれ $\mathscr{H}(\mathfrak{F}, V_1)$ と $\mathscr{H}(\mathfrak{F}, V_2)$ で写像である場合、それぞれ $f_1 \circ \varphi, f_2 \circ \varphi$ 属するから $\mathscr{H}(\varphi^{-1}(\mathfrak{F}), V_1)$ と $\mathscr{H}(\varphi^{-1}(\mathfrak{F}), V_2)$ になり、関係 $f_1 \preccurlyeq f_2$ になることは明らかです。 $f_1 \ll f_2$) は $f_1 \circ \varphi \preccurlyeq f_2 \circ \varphi$ (それぞれ $f_1 \circ \varphi \ll f_2 \circ \varphi$) と同等です。

### 4. 厳密に陽性の写像と関係の比較

$g$ を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の写像とします。これは、$\mathfrak{F}$ の集合に対して厳密に正です。 $g$ を特徴とする比較関係は、他のの方法で定式化できます。 関係 $f \preccurlyeq g$ は、$\|f\|/g$ ($\mathfrak{F}$ の集合で定義される) が集合で境界付けられるというと同等です。 $\mathfrak{F}$; 関係 $f \ll g$ は、$\mathfrak{F}$ に沿って $\|f\|/g$ が 0 になる傾向があるというと同等です。 $f$ が $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の関数である場合、$f \asymp g$ の関係は、$f/g$ が $\mathfrak{F}$ の集合で対数的に制限されていることを意味し、$f \sim g$ の関係は、$f/g$ が $\mathfrak{F}$ に沿って 1 になる傾向があることを意味します。 $f$ が $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ で写像で、$\mathfrak{F}$ で集合が正である場合、$f$ と $g$ が同等であるということは、$f/g$ が極限 (有限または$+\infty$ に等しい) になる傾向があることを意味します。 $\mathfrak{F}$。

#### 命題 9 {#fvr-v-s1-prop-9 .statement tag=08EI}

$f$ と $g$ を、$\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の 2 つの写像とし、$\mathfrak{F}$ の集合は厳密に正とします。 $f$ と $g$ が比較可能であるためには、最大 1 つの例外を除いて、すべての数 $t \geqslant 0$ について、写像 $f - tg$ が $\mathfrak{F}$ の集合に定数符号 $^3$ を持っていることが必要かつ十分です。

条件が必要です。確かに、$f \ll g$ の場合、$t = 0$ を除いて $f - tg \sim -tg$ があるため、$f - tg$ は、$t = 0$ を除いて、$\mathfrak{F}$ の集合に対して厳密に負になります。 $f \gg g$ の場合、$f - tg$ はすべての $t$ に対して $\mathfrak{F}$ の集合で厳密に正になります。最後に、$f \sim kg$ ($k$ 定数 $> 0$) の場合、$t = k$ を除いて $f - t g \sim (k - t)g$ となるため、おそらく$t = k$ を除いて、$f - t g$ は$\mathfrak{F}$ の集合に$k - t$ の符号を持ちます。

条件で十分です。実際、比率 $f/g$ が $\mathfrak{F}$ に沿って 2 つの異なるクラスター 点 $\alpha < \beta$ を持っていると仮定します。 $\alpha < t < \beta$ のような *すべての* 数 $t$ に対して、*すべての* 集合 $X \in \mathfrak{F}$ には 2 つの点 $x_1, x_2$ が存在し、$f(x_1)/g(x_1) < t$ と $f(x_2)/g(x_2) > t$ が存在します。従って、$f(x) - t g(x)$ には $X$ の定数符号がありません。私たちは仮定と矛盾する結論に達しました。従って、$f/g$ は、基底 $\mathfrak{F}$ のフィルターに沿って *1 つだけ* クラスター 値 (有限または無限) を持つことができ、その結果、(*Gen. Top.*, I, p. 85, 系) はこの値をそのクラスターとして持ちます。 *極限* $\mathfrak{F}$沿い。

#### 命題 10 {#fvr-v-s1-prop-10 .statement tag=08EJ}

*$f$ と $g$ を、$\mathfrak{F}$ の集合に対して厳密に正である $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の 2 つの写像とします。すべての $\alpha$ 実数と $\neq 0$ 関係 $f \asymp g$ (それぞれ $f \sim g$) は $f^\alpha \asymp g^\alpha$ (それぞれ $f^\alpha \sim g^\alpha$) と同等です。 $\alpha > 0$ 関係 $f \preccurlyeq g$ (それぞれ $f \ll g$) が $f^\alpha \preccurlyeq g^\alpha$ (それぞれ $f^\alpha \ll g^\alpha$) と等しい場合。 $\alpha < 0$ の場合、$f^\alpha \succcurlyeq g^\alpha$ (それぞれ $f^\alpha \succ g^\alpha$) と同等です。*

証明は明らかです。

写像の $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 集合 $I'$ は、$\mathfrak{F}$ の集合に対して厳密に正であるため、$\Gamma/\mathbf{R}_\infty$ は $\mathscr{H}_\infty(\mathfrak{F}, \mathbf{R})$ の *乗法群* $\Gamma_\infty$ となることに注意してください。 $\Gamma/\mathbf{R}_0$ は、$\Gamma$ の対数境界写像の類 (mod. $\mathbf{R}_\infty$) の部分群による $\Gamma_\infty$ の剰余群と同一です。 $\Gamma/\mathbf{R}_0$ 位数関係から商への通過によって関係 $f \preccurlyeq g$ から推定される関係は、$\Gamma/\mathbf{R}_0$ の群構造と *互換性* があるため、順序付き群になります。

#### 命題 11 {#fvr-v-s1-prop-11 .statement tag=08EK}

*$g$ を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ で写像とし、$\lim_{\mathfrak{F}} g = +\infty$ とします。 関係 $f \ll g$ は $e^f \ll e^g$ を意味します。 関係 $f \sim g$ は $\log f \sim \log g$ を意味します。*

確かに、$f \ll g$ の場合、$f - g = g \left( \frac{f}{g} - 1 \right)$ は $\mathfrak{F}$ に沿って $-\infty$ になる傾向があります。同様に、$f \sim g$ に $\log f = \log g + \log \frac{f}{g}$ がある場合、$\log f - \log g$ は 0 になる傾向があり、$\frac{\log f}{\log g} - 1 = \frac{\log f - \log g}{\log g}$ についても同様です。

一方、関係 $f \sim g$ は *$e^f \sim e^g$ を暗示しているわけではなく、$e^f \asymp e^g$ さえも暗示していないことに注意してください。例で示されているように、$x$ として $f(x) = x^2, \ g(x) = x^3 + x$ は $+\infty$ になる傾向があります。同様に、関係 $f \ll g$ は *$\log f \ll \log g$ を暗示しません*。 例 $f(x) = x, \ g(x) = x^2$ で示されるように、$x$ は $+\infty$ になる傾向があります。

#### 定義 5 {#fvr-v-s1-def-5 .statement tag=08EL}

*$g$ を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ の写像とし、$\mathfrak{F}$ の集合を厳密に正とし、$\lim_{\mathfrak{F}} g = 0$ または $\lim_{\mathfrak{F}} g = +\infty$ とします。 $\lim_{\mathfrak{F}} \log(|f|)/\log g = \rho$ の場合、写像 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ は $g$ に対して位数 $\rho$ (有限または無限) であると言われます*。

$f$ が $g$ に対して位数 $\rho$ である場合、$f$ は $1/g$ に対して位数 $-\rho$ であることに注意してください。したがって、$g(x)$ が $\mathfrak{F}$ に沿って $+\infty$ になる傾向がある場合のみを扱う必要があります。

#### 命題 12 {#fvr-v-s1-prop-12 .statement tag=08EM}

g を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ で写像とし、$\lim_{\mathfrak{F}} g = +\infty$ とします。 f を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ で写像とします。

a) g に対して f が位数 $+\infty$ であるためには、$\alpha \geq 0$ ごとに $f \gg g^\alpha$ であることが必要かつ十分です。

b) g に対して f が位数 $-\infty$ であるためには、すべての $\alpha > 0$ が $f \ll g^{-\alpha}$ であることが必要かつ十分です。

c) f が g に対して $\rho$ に等しい有限の位数であるためには、$\varepsilon > 0$ ごとに $g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$ が存在することが必要かつ十分です。

たとえばc)を証明しましょう。 g に対する f の位数が $\rho$ である場合、すべての $\varepsilon > 0$ に対して集合 $M \in \mathfrak{F}$ が存在し、すべての $x \in M$ について、次のようになります。

$$
\left( \rho - \frac{\varepsilon}{2} \right) \log g(x) \leq \log |f(x)| \leq \left( \rho + \frac{\varepsilon}{2} \right) \log g(x),
$$

または$(g(x))^{\rho - \frac{\varepsilon}{2}} \leq |f(x)| \leq (g(x))^{\rho + \frac{\varepsilon}{2}}$; $\lim_{\mathfrak{F}} g = +\infty$ なので、$\varepsilon > 0$ ごとに $g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$ になります。 逆は明らかです。 a)とb)の証明は類似しています。

f が g に対して有限位数 $\rho$ である場合、$fg^{-\rho}$ は g に対して位数 0 であり、その逆であることに注意してください。 $f_1$ (それぞれ $f_2$) が g に対して位数 $\rho_1$ (それぞれ $\rho_2$) であり、$\rho_1 + \rho_2$ が定義されている場合、$f_1 f_2$ は g に対して位数 $\rho_1 + \rho_2$ になります。

#### 注意 1 {#fvr-v-s1-n4-rem-1 .statement tag=08EN}

けれども f は g に対して有限の位数 $\rho$ であっても、比率 $f/g^\rho$ が極限になる傾向がある必要はないことに注意してください。たとえば、対数的に制限されたすべての写像は g に対して位数 0 になりますが、$\mathfrak{F}$ に沿って極限を持つ必要はありません。

#### 注意 2 {#fvr-v-s1-n4-rem-2 .statement tag=08EO}

$\mathfrak{F}$ の集合で定義された写像は、g に対して確定的な位数 (有限かどうか) を持つ必要はありません。g に対して確定的な位数を持つ写像は、最大 1 つの例外を除き、g のすべての冪と比較できます。さて、例 $g(x) = x,\ f(x) = 1 + x^2 \sin^2 x$ からわかるように、f はこれ性質を持つ必要はありません (x は $+\infty$ になる傾向があるため)。この例 f は、$\alpha < 0$ および $\alpha > 2$ の $g^\alpha$ に相当します。 $f(x) = e^x \sin^2 x + e^{-x} \cos^2 x$ を取る場合、f は g のどの冪 (正または負) とも比較できません。

### 5. 記法

実数写像 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ が与えられた場合、公式では、f が支配的な写像に対して $O(f)$ を、f に対して無視できる写像に対して $o(f)$ を書くのが便利であることがよくあります。 証明に、同じ写像 f (それぞれ f に対して無視できる) によって支配されるいくつかの写像の特徴がある場合、それらを $O_1(f),\ O_2(f)$ など (それぞれ $o_1(f),\ o_2(f)$ など) で表します。

多くの著者は、f (f に比べて無視できる) によって支配されている証明のすべての写像に対して無差別に $O(f)$ (それぞれ $o(f)$) と書いていますが、これは混乱を招く恐れのある乱用です。

この記法を使って小道具を表現することができます。 1、2、3 (V、p. 213) は次のようになります: $g = O_1(f)$ と $h = O(g)$ の場合は $h = O_2(f)$;書くことができます

$$
\sum_{i=1}^{n} \lambda_i O_i(f) = O_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{1}
$$
$$
O(f) \, O(g) = O(fg). \tag{2}
$$

同様に、プロップ。 4 (V、p. 215) は、$g = O_1(f)$ と $h = o(g)$ (それぞれ $g = o_1(f)$ と $h = O(g)$) の場合、$h = o_2(f)$ と小道具を示します。 5と6（V、p. 5）は形で表現できます
$$
\sum_{i=1}^{n} \lambda_i o_i(f) = o_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{3}
$$
$$
o(f) \, O(g) = o(fg). \tag{4}
$$

関係 $f \sim g$ は $f = g + o(g)$ と同等です。 記法 $O(1)$ (それぞれ $o(1)$) は、$\mathfrak{F}$ の集合で境界付けられる写像 (それぞれ写像が $\mathfrak{F}$ に沿って 0 になる傾向がある) を示します。

### 練習問題 {#fvr-v-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
