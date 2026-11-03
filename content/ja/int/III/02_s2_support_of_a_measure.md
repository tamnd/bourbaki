---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 2
section_title: Support of a measure
lang: ja
source: int-i-vi
book_pages: INT III.23-INT III.32, INT III.59
pdf_pages: 0068-0077, 0104-0104
extraction: ocr
subsections:
    - "no": 1
      title: Restriction of a measure to an open set. Definition of a measure by means of local data
      page: 23
      pdf_page: 68
    - "no": 2
      title: Support of a measure
      page: 25
      pdf_page: 70
    - "no": 3
      title: Characterization of the support of a measure
      page: 27
      pdf_page: 72
    - "no": 4
      title: Point measures. Measures with finite support
      page: 29
      pdf_page: 74
    - "no": 5
      title: Discrete measures
      page: 31
      pdf_page: 76
statements: 26
exercises: 5
content_sha256: 70e8dfb8ab6171a18da058ae2c20dbc5391f61d22bba671db6c57cbf21d10a59
translated_from: content/en/int/III/02_s2_support_of_a_measure.md
translation_method: google
source_content_sha256: 1e58e2cf7e28f71e344d5832fbb288579da1f287b87e4bdbaf8b730a89a6bea7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d178c3cb91ea860c7d5ba9cdfcb03a81c515355acdc48f0794f7525b72c39e95
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。対策の支援

### 1. 小節の制限からオープン集合まで。ローカルデータによる測定の定義

X を局所的にコンパクトな空間とし、Y を X のオープン集合とします。 X の部分空間 Y は局所的にコンパクトであり、トポロジー ベクトル空間 E で値と連続するすべての写像は、Y で定義され、コンパクトなサポートを備えており、$\mathbf{C}Y$ に値 0 を与えることで、連続性によって X のすべてに拡張できます。したがって、このように同一視する空間 $\mathscr{K}(Y;E)$ は、Y に含まれる* コンパクトなサポートを持つ連続写像によって形成される $\mathscr{K}(X;E)$ の線形部分空間を使用して$\mu$ がX のメジャーである場合、制限が$\mu$ から $\mathscr{K}(Y;\mathbf{C})$ は、オープン部分空間 Y に対する $\mu$ の *制限*、または $\mu$ によって Y に *誘導された* メジャーであり、$\mu|Y$ で示されます。 $|\mu|$、$\mathscr{R}\mu$、$\mathscr{I}\mu$ の Y に対する制限は、§1 の 5 番と 6 番により、それぞれ $|\mu|Y|$、$\mathscr{R}(\mu|Y)$、$\mathscr{I}(\mu|Y)$ になります。 $\mu$ が本物の場合、 Y に対する $\mu^+$ と $\mu^-$ の制限は、§1, No. 5 の公式により、それぞれ $(\mu|Y)^+$ と $(\mu|Y)^-$ になります。

Y と Z が $Y \supset Z$ のように X で 2 つ開いた集合であり、$\mu|Y$ と $\mu|Z$ が Y と Z に対して $\mu$ の制限である場合、$\mu|Z$ もまた制限であることがわかります。 $\mu|Y$ をローカルにコンパクトな空間 Y のオープン部分空間 Z にします。

Chでは、 IV, §5, No. 7 この定義を、Y が X の局所的にコンパクトな部分空間である場合に一般化します。

Y に関するメジャーは *必ずしも * ではない* ことに注意してください。X 上の何らかのメジャーの制限 (cf. 第 V, §7, No. 2、提案 3)。

たとえば、Y を $X = \mathbf{R}$ のオープン区間 ]0,1[ とします。 写像

$$
f \mapsto \int_0^1 \frac{f(x)}{x} dx
$$

は $Y$ のメジャーです。なぜなら、$\mathscr{K}(Y; \mathbf{C})$ のすべての写像は、$\mathbf{R}$ の 0 の近傍では零であるからです。ただし、この尺度できないは、$\mathbf{R}$ の小節まで拡張されます。これは、逆の場合、写像 $f \in \mathscr{K}(Y; \mathbf{C})$ の制限から集合が$\|f\| \leq 1$ に制限されるためです。しかし、これは誤りです。

ただし、次の命題があります。

#### 命題 1 {#int-iii-s2-prop-1 .statement tag=08MR}

*$(Y_\alpha)_{\alpha \in A}$ * を * $X$ のオープンカバー* とし、* の各部分空間* $Y_\alpha$ で *$\mu_\alpha$ を *測定* し、* の対* ごとに $(\alpha, \beta)$、*制限が得られるようにします。 $\mu_\alpha$ * と* $\mu_\beta$ * から* $Y_\alpha \cap Y_\beta$ * は同一です。これらの条件の下には、添字* $\alpha$ ごとに、制限から* $Y_\alpha$ * $\mu_\alpha$ * に等しい* $X$ に、唯一のメジャー* $\mu$ が存在します。

まず、すべての写像 $f \in \mathscr{K}(X; \mathbf{C})$ は、有限和 $f = \sum_i f_i$ の形で記述できることを示しましょう。ここで、写像 $f_i \in \mathscr{K}(X; \mathbf{C})$ のそれぞれに対して、$\operatorname{Supp}(f_i) \subset Y_{\alpha_i}$ となる添字 $\alpha_i$ が存在します。 $K = \operatorname{Supp}(f)$ の場合、添字 $\alpha_i$ ($1 \leq i \leq n$) の有限数が存在し、$Y_{\alpha_i}$ 形は $K$ を覆います。 $h_i$ ($1 \leq i \leq n$) を $X$ の写像から $[0, 1]$ に連続させ、$h_i$ のサポートがコンパクトで、$1 \leq i \leq n$ の$Y_{\alpha_i}$ に含まれ、$\sum_{i=1}^n h_i(x) = 1$ が$K$ になるようにします。 (§ 1, No. 2, 補題 1); 写像 $f_i = f h_i$ は要件を満たしています。 これは、まず、要件を満たすメジ​​ャー $\mu$ が存在する場合、それは *一意* であることを示しています。なぜなら、すべての有限和 $f = \sum_{i=1}^n f_i$ に対して、$f_i \in \mathscr{K}(Y_{\alpha_i}; \mathbf{C})$ は必然的に $\mu(f) = \sum_{i=1}^n \mu_{\alpha_i}(f_i)$ になるからです。 さらに、次の性質を証明する限り、$\mathscr{K}(X; \mathbf{C})$ 上の線形形式 $\mu$ の存在を示したことになります。その各部分空間 $\mathscr{K}(Y_\alpha; \mathbf{C})$ への制限は $\mu_\alpha$ です。$(g_i)_{1 \leq i \leq m}$ と $(h_j)_{1 \leq j \leq n}$ が、$1 \leq i \leq m$ に対して $g_i \in \mathscr{K}(Y_{\alpha_i}; \mathbf{C})$ となるような $\mathscr{K}(X; \mathbf{C})$ の 2 つの有限関数列である場合、 $1 \leq j \leq n$の場合は$h_j \in \mathscr{K}(Y_{\beta_j}; \mathbf{C})$、
$$
\sum_{i=1}^m g_i(x) = \sum_{j=1}^n h_j(x) = 1
$$
$K$、その後
$$
\sum_{i=1}^m \mu_{\alpha_i}(f g_i) = \sum_{j=1}^n \mu_{\beta_j}(f h_j).
$$
さて、
$$
f g_i = \sum_{j=1}^n f g_i h_j,
$$

よって
$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{i=1}^{m} \sum_{j=1}^{n} \mu_{\alpha_i}(f g_i h_j).
$$
同様に、
$$
\sum_{j=1}^{n} \mu_{\beta_j}(f h_j) = \sum_{j=1}^{n} \sum_{i=1}^{m} \mu_{\beta_j}(f g_i h_j).
$$
しかし、$f g_i h_j$のサポートが$Y_{\alpha_i} \cap Y_{\beta_j}$に含まれているため、$\mu_{\alpha_i}(f g_i h_j) = \mu_{\beta_j}(f g_i h_j)$があり、これにより主張が確立されます。

$\mu$ が $X$ のメジャーであることを確認する必要があります。現在、$X$ のすべての点には、$Y_\alpha$ のいずれかに含まれるコンパクトな近隣地域が認められています。したがって、結論は$\mu$の定義と§1, No. 3の提案6からすぐに得られます。

#### 系 (定位の原則) {#int-iii-s2-n1-cor-1 .statement tag=08MS}

— *$\mu$ と $\nu$ を $X$ の 2 小節とし、$(Y_\alpha)$ を $X$ のオープン集合の族とし、$\alpha$ ごとに、$\mu$ と $\nu$ の制限から $Y_\alpha$ が次のようになります。等しい;その場合、$\mu$ の制限と $\nu$ ～ $Y = \bigcup_\alpha Y_\alpha$ は等しい*。

### 2. 対策の支援

$\mu$ をローカルコンパクト空間 $X$ のメジャーとし、$\mathscr{G}$ をオープン集合 $U \subset X$ の集合とし、$\mu$ から $U$ の制限は次のようにします。 零;局所化の原理 (No. 1、提案 1 の補正) から、$U_0$ が集合 $U \in \mathscr{G}$ の和集合である場合、$U_0$ 自体は属するから $\mathscr{G}$ であり、したがって、最大のであることがすぐにわかります。 $\mathscr{G}$中集合。

#### 定義 1 {#int-iii-s2-def-1 .statement tag=08MT}

*$\mu$がローカルコンパクト空間$X$のメジャーである場合、$\operatorname{Supp}(\mu)$で示される$\mu$のサポート定義するは、オープン集合の最大のを補完するクローズド集合になります。 $X$ の $\mu$ の制限は零です*。

点 $x \in X$ が $\mu$ のサポートに対して属するを持たないということは、$\mu$ から $V$ の制限が零となるような、$x$ の開いた近傍 $V$ が存在することを意味します。したがって、$\mu$ のサポートに対する $x$ 属するは、$x$ の *すべての* 近傍 $V$ に対して、写像 $f \in \mathscr{K}(X; \mathbf{C})$ が存在し、そのサポートは $\mu(f) \neq 0$ のように $V$ に含まれることを意味します。

#### 例 {#int-iii-s2-n2-exa-1 .statement tag=08MU}

— 1) $X$ のメジャーが *零* であるためには、そのサポートが *空* であることが必要かつ十分です。
2) $\mathbf{R}$ 上のルベーグ測度のサポートは、ライン $\mathbf{R}$ 全体です。なぜなら、それは空でないであり、どの翻訳においても不変だからです。

3) $\mathbf{R}$ の区間 $X = [0,1]$ について、数列 $(a_n)$ に配置された可算密集部分集合を考え、$\mu$ を各点 $a_n$ に質量$2^{-n}$ を置くことによって定義される尺度とします。 $n \geq 0$ (§ 1, No. 3、例 I)。 $\mu$ のサポートは $X$ のすべてです。 $x$ を $X$ の任意の点、$V$ $x$ の近傍、$f$ を $X$ 上の連続実数値写像 $\geq 0$ とし、点で 1 に等しいとします。 $x$、そのサポートは $V$ (§ 1, No. 2、補題 1) に含まれています。 $y \in V$ の集合は、$f(y) > 0$ が $X$ に開くため、含む点 $a_n$、従って $\mu(f) \geq f(a_n)2^{-n} > 0$ になります。

#### 命題 2 {#int-iii-s2-prop-2 .statement tag=08MV}

*メジャー $\mu$ のサポートはメジャー $|\mu|$ のサポートと同じです。 $\mu$ が本物である場合、そのサポートは$\mu^+$ と $\mu^-$ のサポートの和集合です。

なぜなら、オープン集合 $U$に対する$\mu$の制限が零であれば、$|\mu|$（$\mu$が実数の場合、それぞれ$\mu^+$と$\mu^-$）の制限も同様です。またその逆も同様です。

$\mu^+$ と $\mu^-$ のサポートは、空でないと *同一* である可能性があることに注意してください (cf. Ch. V, § 5、Exer. 5)。

#### 命題 3 {#int-iii-s2-prop-3 .statement tag=08MW}

*$\mu$ と $\nu$ が、$|\mu| \leq |\nu|$ のように局所的にコンパクトな空間 $X$ 上の 2 小節である場合、$\mathrm{Supp}(\mu) \subset \mathrm{Supp}(\nu)$。

なぜなら、オープン集合に対する$\nu$の制限が零であれば、$\mu$の制限も同様だからです。

#### 命題 4 {#int-iii-s2-prop-4 .statement tag=08MX}

*2 つの措置のうち和の支持は、それらの支持の和集合に含まれます。

なぜなら、オープン集合までの 2 小節の制限が零である場合、その和の制限にも同じことが当てはまります。

$\mu$ と $\nu$ が 2 つの *正 * 指標である場合、 $\lambda = \mu + \nu$ のサポートは $\mu$ と $\nu$ のサポートの和集合に * 等しい* です。なぜなら、$x_0$ が和集合の点で、$V$ が $x_0$ の近傍である場合、$V$ に含まれるサポートを伴う連続写像 $f \geq 0$ が存在し、数の 1 つが成立するためです。 $\mu(f)$、$\nu(f)$ は $> 0$ です。 *なおさら*、$\lambda(f) = \mu(f) + \nu(f) > 0$。

#### 命題 5 {#int-iii-s2-prop-5 .statement tag=08MY}

*メジャー $\mu$ の制限のサポート集合 $U$ は、$\mu$ のサポートの $U$ 上のトレースです。

命題は定義から明らかです。

#### 命題 6 {#int-iii-s2-prop-6 .statement tag=08MZ}

*局所的にコンパクトな空間$X$上のメジャーの集合は、閉じた集合$F$にサポートが含まれており、$\mathscr{M}(X; \mathbf{C})$の漠然と閉じた線形部分空間です。

なぜなら、それは方程式$\mu(f) = 0$で漠然と閉じた超平面の共通部分であり、$f$は$F$と交差しない$\mathscr{H}(X; \mathbf{C})$の写像の集合を超えます。

$X$ が *コンパクトではない* と仮定します。$X$ のメジャーの空間 $\mathscr{M}(X; \mathbf{C})$ にフィルター $\Phi$ が与えられると、すべてのコンパクト部分集合について、メジャー $\mu$ のサポートが $\Phi$ *に沿って無限に後退すると言えます。 $X$ の $K$ には、各小節 $\mu \in M$ に対して $\mathrm{Supp}(\mu) \cap K = \varnothing$ となる集合 $M \in \Phi$ が存在します。

#### 命題 7 {#int-iii-s2-prop-7 .statement tag=08N0}

— *$\Phi$が$\mathscr{M}(X; \mathbf{C})$のフィルターで、$\mu$のサポートが$\Phi$に沿って無限に後退する場合、$\mu$は$\Phi$に関して漠然と0に収束します。

$f$ を $\mathscr{K}(X; \mathbf{C})$ の任意の写像とし、$K$ をそのサポートとします。 仮定までに、集合 $M \in \Phi$ が存在し、各小節に対して $\mu \in M$、$\operatorname{Supp}(\mu) \cap K = \varnothing$ が発生します。すべての $\mu \in M$ に対して $\mu(f) = 0$ となり、命題が証明されます。

### 3. 対策の支援の特徴付け

定義までに、写像 $f \in \mathscr{K}(X; \mathbf{C})$ のサポートがメジャー $\mu$ のサポートと *交差しない*場合、$\mu(f) = 0$ になります。ただし、次のより正確な結果は true です。

#### 命題 8 {#int-iii-s2-prop-8 .statement tag=08N1}

— *$\mu$を局所的にコンパクトな空間$X$のメジャーとします。 写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、$\operatorname{Supp}(\mu)$、$\mu(f) = 0$ では零になります。*

集合 $K = \operatorname{Supp}(f)$、$S = \operatorname{Supp}(\mu)$。 数 $\varepsilon > 0$ が与えられた場合、$V$ を $|f(x)| < \varepsilon$ となるような $x \in X$ の集合とします。 $V$ は仮定によるオープン集合含む $S$ であるため、$CS$ はコンパクト集合 $CV$ の近傍です。従って、$X$ から $[0, 1]$ までの連続した写像 $h$ が存在し、$CV$ の 1 に等しく、$CS$ (§ 1, No. 2、補題 1) に含まれるサポートが存在します。 $fh$のサポートが$S$、$\mu(fh) = 0$と交わらないので。一方、$K \cap CV$は$f = fh$、$X$は$|fh| \leq |f|$なので、$V$の選択までに$X$は$|f - fh| \leq 2\varepsilon$となります。最後に、サポートが $K$ に含まれるすべての写像 $g \in \mathscr{K}(X; \mathbf{C})$ に対して $|\mu(g)| \leq M_K \|g\|$ となるような数 $M_K$ が存在することに注目してください。 $f - fh$のサポートは$K$、$|\mu(f - fh)| \leq 2M_K \varepsilon$、そしてその結果$|\mu(f)| = |\mu(f - fh)| \leq 2M_K \varepsilon$に含まれるため。 $\varepsilon$ は任意なので、$\mu(f) = 0$。

#### 系 1 {#int-iii-s2-prop-8-cor-1 .statement tag=08N2}

— *$\mathscr{K}(X; \mathbf{C})$ の 2 つの写像 $f, g$ が $\operatorname{Supp}(\mu)$ で等しい場合、$\mu(f) = \mu(g)$。*

#### 系 2 {#int-iii-s2-prop-8-cor-2 .statement tag=08N3}

— *$\mu$を$X$に対するプラスの指標とします。 $f \in \mathscr{K}(X; \mathbf{C})$ が $\operatorname{Supp}(\mu)$ 上の $f(x) \geq 0$ である場合、$\mu(f) \geq 0$。*

$f = |f|$ が $\operatorname{Supp}(\mu)$ の場合、$\mu(f) = \mu(|f|) \geq 0$ by 系 1.

#### 系 3 {#int-iii-s2-prop-8-cor-3 .statement tag=08N4}

— * $\mu$ を $X$ での制限された尺度とします。 $f \in \mathscr{K}(X; \mathbf{C})$ が $\operatorname{Supp}(\mu)$ 上の $|f(x)| \leq a$ である場合、$|\mu(f)| \leq a \|\mu\|$。*

$\operatorname{Supp}(|\mu|) = \operatorname{Supp}(\mu)$ の場合、$h$ が $X$ から $[0, 1]$ への連続写像で、$\operatorname{Supp}(f)$ の 1 に等しく、コンパクトなサポートがある場合、$\operatorname{Supp}(\mu)$ で $|f(x)| \leq ah(x)$ になります。

$$
|\mu|(|f|) \leq a|\mu|(h) \leq a\|\mu\|
$$

系 2 著;結論は § 1, No. 6 の公式 (13) から導き出されます。

#### 命題 9 {#int-iii-s2-prop-9 .statement tag=08N5}

— $\mu$ を $X$ に対する前向きの尺度とします。 $f$ が $\mathscr{K}_+(X)$ で写像で、$\mu(f) = 0$ である場合、$f$ は $\mathrm{Supp}(\mu)$ で零になります。

$x$ を $X$ の点として、$f(x) > 0$ とします。 $x$ が属するから $\mathrm{Supp}(\mu)$ にならないことを示しましょう。なぜなら、$x$と数$a > 0$のコンパクトな近傍$V$が存在し、$V$に$f(y) \geq a$が存在するからです。 $g$ が、$V$ に含まれるサポートを持つ連続写像 $\geq 0$ である場合、$\mu(g) = 0$ であることを示しましょう。確かに、集合 $b = \|g\|$ の場合、$g \leq bf/a$、よって $\mu(g) \leq b\mu(f)/a = 0$ となります。

#### 命題 10 {#int-iii-s2-prop-10 .statement tag=08N6}

— $\mu$ を局所的にコンパクトな空間 $X$ のメジャーとします。 写像 $g \in \mathscr{C}(X; \mathbf{C})$ ごとに、メジャー $g \cdot \mu$ のサポートは、点 $x \in \mathrm{Supp}(\mu)$ の集合の閉包 $T$ であり、$g(x) \neq 0$ になります。

集合 $S = \mathrm{Supp}(\mu)$; $x_0$ を所属から $T$ ではなく点にします。 $x_0$ の開いた近傍 $V$ が存在し、$V \cap S$ の点ごとに $g$ が零になります。 $f \in \mathscr{K}(X; \mathbf{C})$ が $V$ に含まれるサポートを持っている場合、$fg$ は $S$ で零であるため、(提案 8) $\mu(gf) = 0$;その他の語、$g \cdot \mu$～$V$の制限は零です。

逆に、点 $x_0 \in X$ の開いた近傍 $W$ に対する $g \cdot \mu$ の制限が零であると仮定すると、$g$ が $\neq 0$ である$W \cap S$ の点が存在しないことを示しましょう。実際、そのような点 $y$ が存在する場合、点 $x$ のうち $g(x) \neq 0$ ごとに、$W$ に含まれる$y$ のコンパクトな近傍 $U$ が存在することになります。しかし、その後、$U$ に含まれるサポートを持つすべての写像 $f \in \mathscr{K}(X; \mathbf{C})$ は、$f = gh$ と書くことができます。ここで、$h \in \mathscr{K}(X; \mathbf{C})$ は $U \subset W$ に含まれるサポートを持ちます。その後、仮定 $y \in S$ とは逆に、$\mu(f) = \mu(gh) = 0$ が続きます。

なお、$T$は$\mu$のサポート$S$と$g$のサポートの共通部分に含まれていますが、必ずしもこの共通部分と等しいわけではありません。たとえば、$X = \mathbf{R}$、$\mu$ が点 0、および $g(x) = x$ でのディラック指標である場合、$g$ と $\mu$ 簡約するのサポートのけれども共通部分も$g \cdot \mu = 0$ になります。 点 0、つまり空でないです。

#### 系 {#int-iii-s2-n3-cor-1 .statement tag=08N7}

— $g \cdot \mu$ が零である位数では、$\mu$ のサポートに基づいて $g$ が零であることが必要かつ十分です。

#### 命題 11 {#int-iii-s2-prop-11 .statement tag=08N8}

— コンパクトなサポートを備えたすべてのメジャーには制限があります。

なぜなら、$|\mu|$ もコンパクトなサポートを持つメジャーであるため、$\mu \geq 0$ の場合に注意を限定することができます。 $h$ が $X$ から $[0, 1]$ への連続写像で、コンパクトなサポートがあり、$\mathrm{Supp}(\mu)$ で 1 に等しい場合、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、$\mathrm{Supp}(\mu)$ に $|f(x)| \leq \|f\| h(x)$ が存在します。 8) $\mu(|f|) \leq \mu(h)\|f\|$、これは命題 (§ 1, No. 8) を証明します。

### 4. 点対策。 有限台による対策

#### 命題 12 {#int-iii-s2-prop-12 .statement tag=08N9}

— $a_i$ ($1 \leq i \leq n$) を、局所的にコンパクトな空間 $X$ 内で区別できる点とします。 $a_i$ の集合にサポートが含まれている $X$ の各小節は、$\varepsilon_{a_i}$ ($1 \leq i \leq n$) の小節の線形結合です。

なぜなら、そのような尺度 $\mu$ は、写像 $f \in \mathscr{K}(X; \mathbf{C})$ 満たす $n$ 関係 $f(a_i) = 0$ ごとに零となるからです (No. 3、提案 8)。これらの関係は $\varepsilon_{a_i}(f) = 0$ と書かれる可能性があるため、$\mu$ は $\varepsilon_{a_i}$ の線形結合です (A、II, §7, No. 5、Th. 7 コリント 1)。

特に、サポートが空であるか、単一の点 $x$ に減らされているすべての小節は、形 $\alpha \varepsilon_x$ であり、$\alpha$ は複素数です。このような尺度は *点尺度*と言われます。したがって、サポートが有限であるすべてのメジャーは、点メジャーの和です。

#### 定理 1 {#int-iii-s2-thm-1 .statement tag=08NA}

— *すべてのメジャー* $\mu$ *局所的にコンパクトな空間* $X$ *は、ベクトル空間* $V$ *サポートが有限であり* $\mathrm{Supp}(\mu)$に含まれるメジャーの曖昧な終結の中にあります。

$\mu$ が $V$ (TVS、II, §6, No. 3、Th. 1 の Cor. 2) に直交する $\mathscr{K}(X; \mathbf{C})$ の部分空間 $V^\circ$ に直交する、つまり関係 $\langle f, \varepsilon_a \rangle = 0$ を証明すれば十分です。 $a$ は $\mu$ のサポートを上回り、$\langle f, \mu \rangle = 0$ を暗示します。しかし、これはNo. 3の提案8にすぎません。

#### 系 1 {#int-iii-s2-thm-1-cor-1 .statement tag=08NB}

— *すべての有界メジャー* $\mu$ *on* $X$ *は、凸型集合* $A$ *サポートが有限であり、* $\mu$ のサポートに含まれるメジャーの曖昧な閉包の中にあり、*そのノルムは* $\leq \| \mu \|$ です。 *さらに、* $\nu$ * $A$ に留まりながら * 漠然と $\mu$ になる傾向がある場合*、*その後* $\| \nu \|$ * $\| \mu \|$ になる傾向* があります。

最初の主張を証明するには、測度 $\mu$ が $\mathscr{K}(X; \mathbf{C})$ (TVS、II, §6, No. 3、Th. 1 および §8, No. 4) の $A$ の極集合 $A^\circ$ に属することを確立するだけで十分です。これは、$f \in \mathscr{K}(X; \mathbf{C})$ について、すべての $a \in \mathrm{Supp}(\mu)$ に対する関係 $|\langle f, \varepsilon_a \rangle| \leq 1/\| \mu \|$ が $|\langle f, \mu \rangle| \leq 1$ を意味することを意味します。しかし、これはコルの結果です。 No. 3の提案8の3。

2 番目の主張を証明するには、次のことに注意してください。

$$
\liminf_{\nu \to \mu, \nu \in A} \| \nu \| \geq \| \mu \|
$$

写像 $\nu \mapsto \| \nu \|$ は曖昧な位相に対して下位半連続であるため (§1, No. 9、提案 15 の Cor. 4)、結論は定義による $\nu \in A$ に対する $\| \nu \| \leq \| \mu \|$ という事実から得られます。

#### 系 2 {#int-iii-s2-thm-1-cor-2 .statement tag=08NC}

— *すべての制限された測度* $\mu$ *on* $X$ *は、サポートが有限で* $\mu$ * のサポートに含まれており、そのノルムが* $\| \mu \|$ に等しい一連の測度の曖昧な終結の中にあります。

$\mu \neq 0$ と仮定できます。 $V$ を曖昧な位相の 0 の開いた近傍とします。コルのおかげで、$0 < \varepsilon < 1$ となるようなすべての $\varepsilon$ が存在します。 1、メジャー $\nu_0$ のサポートは有限であり、$\mathrm{Supp}(\mu)$ に含まれており、そのために $\nu_0 - \mu \in V$ と $\| \mu \| \geq \| \nu_0 \| \geq (1 - \varepsilon) \| \mu \|$ が含まれます。 設定 $\nu = (\| \mu \| / \| \nu_0 \|) \nu_0$、$\| \nu \| = \| \mu \|$ と $\| \nu - \nu_0 \| \leq \| \mu \|$ があります。 $\varepsilon$ が十分小さいため、結論は $\nu - \mu \in V + V$、よってになります。

#### 系 3 {#int-iii-s2-thm-1-cor-3 .statement tag=08ND}

*$X$上のすべての有界ポジティブ測度$\mu$は、ポジティブ測度の凸型集合の曖昧な閉包の中にあり、そのサポートは有限であり、$\mu$のサポートに含まれており、そのノルムは$\| \mu \|$に等しい。

コルと同じ推論。 2 は、$\mathrm{Supp}(\mu)$ に含まれる有限台とノルム $\leq \| \mu \|$ による積極的な手段によって形成された凸型集合 $B$ の曖昧な閉包の中に、$\mu$ が証明に極限できることを示しています。 繰り返しになりますが、$\mu$ が $B^\circ$ の極集合、$B$ の極集合に *空間* $\mathscr{K}(X; \mathbf{R})$ (TVS、II, §6, No. 3、Th. 1) に属していることを確立するだけで十分です。しかし、これは、$f \in \mathscr{K}(X; \mathbf{R})$ について、すべての $a \in \mathrm{Supp}(\mu)$ に対する関係 $\langle f, \varepsilon_a \rangle \geq -1 / \| \mu \|$ が $\langle f, \mu \rangle \geq -1$ を暗示し、これは No. 3 の結果であることを意味します。提案 8 の 2。

#### 系 4 {#int-iii-s2-thm-1-cor-4 .statement tag=08NE}

*空間 $\mathscr{M}(X; \mathbf{C})$ では、点対策の集合は、厳密にコンパクトな収束* (§1, No. 10) の位相の合計です。

円錐 $\mathscr{M}_+(X)$ では、厳密にコンパクトな収束の位相は曖昧な位相 (§1, No. 10、提案 18) と同一であり、$X$ 上のすべての尺度は $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$ と書くことができ、$\mu_j$ ($1 \leq j \leq 4$) は肯定的な尺度です。したがって、結論は Th から得られます。 1.

#### 命題 13 {#int-iii-s2-prop-13 .statement tag=08NF}

*$\mu$ を局所的にコンパクトな空間 $X$ のメジャーとします。 点 $x_0$ から属する 〜 $\mathrm{Supp}(\mu)$ の場合、点の測定$\varepsilon_{x_0}$ が$g \cdot \mu$ の測定集合のあいまいな終結の中にあり、$g$ が継続的な測定集合を超えることが必要かつ十分です。 写像は、$\| g \cdot \mu \| \leq 1$.* のようなコンパクトなサポートを備えています。

No. 2 の提案 6 により、条件は明らかに十分です。それが必要であることを確認するには、$x_0 \in \mathrm{Supp}(\mu)$ と仮定します。 $\mathscr{K}(X; \mathbf{C})$ の写像 $f_k$ ($1 \leq k \leq n$) の有限数と、任意の数 $\delta > 0$ を考えてみましょう。私たちは、$\| g \cdot \mu \| \leq 1$ などの写像 $g \in \mathscr{K}(X; \mathbf{C})$ が存在することを証明する必要があります。
$$
|f_k(x_0) - \mu(g f_k)| \leq \delta
$$
$1 \leq k \leq n$の場合。 $U$ を、$U$ 上の各$f_k$ ($1 \leq k \leq n$) の振動が $\leq \delta / 2$ となるように、$x_0$ の比較的コンパクトな開いた近傍とします。 $x_0 \in \mathrm{Supp}(\mu)$ 以来、仮定までに、$U$ にサポートが含まれている$\mu(g_0) \neq 0$ が含まれる写像 $g_0 \in \mathscr{K}(X; \mathbf{C})$ が存在します。 $U$、$\nu(f) = \mu(g_0) \neq 0$ ではすべての写像 $f \in \mathscr{K}(X; \mathbf{C})$ が 1 に等しいため、メジャー $\nu = g_0 \cdot \mu$ は零ではありません。さらに、$\nu$ は有界です (No. 3、提案 11)。

$g_0$ にスカラーを乗算すると、$\| \nu \| = 1$ と仮定できます。したがって、設定 $\alpha_k = f_k(x_0)$ $1 \leq k \leq n$ とすべての写像 $h \in \mathscr{K}(X; \mathbf{C})$ について、次のように書くことができます。

$$
f_k(x_0) - \nu(f_k h) = \alpha_k (1 - \nu(h)) + \nu((\alpha_k - f_k)h) .
$$

$\nu$ は $U$ でサポートされているため、制限から $U$ まで同一視するすることができます。 仮定 $\| \nu \| = 1$ は、$U$ にサポートが含まれる写像 $h \in \mathscr{K}(X; \mathbf{C})$ が存在することを暗示します。つまり、$\| h \| \leq 1$ や $1 \leq k \leq n$ に対して $| \alpha_k (1 - \nu(h)) | \leq \delta / 2$ が含まれます。さらに、$U$ の定義は、すべての $x \in U$ に対して $| (\alpha_k - f_k(x)) h(x) | \leq \delta / 2$ であることを示しています。 $\| \nu \| = 1$ と $\operatorname{Supp}(\nu) \subset U$ なので、$| \nu((\alpha_k - f_k)h) | \leq \delta / 2$ となり、設定 $g = g_0 h$、

$$
| f_k(x_0) - \mu(g f_k) | \leq \delta \quad \text{for } 1 \leq k \leq n .
$$

これは、$\| g \cdot \mu \| = \| (g_0 h) \cdot \mu \| \leq \| g_0 \cdot \mu \| = 1$ なので、命題であることが証明されます。

#### 系 {#int-iii-s2-n4-cor-1 .statement tag=08NG}

*$\mu$を$X$のメジャーとします。 $X$ の$\nu$ が、$g$ が $\mathscr{K}(X; \mathbf{C})$ を超える$g \cdot \mu$ の集合の漠然とした終結の中にあるためには、$\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$ であることが必要かつ十分です。*

$\operatorname{Supp}(g \cdot \mu) \subset \operatorname{Supp}(\mu)$ by No. 3、提案 10;したがって、形 $g \cdot \mu$ のあらゆるあいまいな極限の支持は、$\operatorname{Supp}(\mu)$ (No. 2、提案 6) にも含まれています。 逆に、$\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$ の場合、$\nu$ は、$\operatorname{Supp}(\mu)$ (Th. 1) に含まれる *有限* サポートを伴う措置の曖昧な限界であり、したがって、提案 13 による一連の措置 $g \cdot \mu$ の曖昧な終結に含まれます。

### 5. 個別の対策

#### 命題 14 {#int-iii-s2-prop-14 .statement tag=08NH}

*局所的にコンパクトな空間 $X$ 上のメジャー $\mu$ が離散メジャー (§ 1, No. 3、例 I) であるためには、$\operatorname{Supp}(\mu)$ が $X$ の離散閉じた部分空間であることが必要かつ十分です。

$\mu$ を、$X$ の離散的な閉じた部分空間 $N$ の点 $x$ に配置された質量 $h(x) \neq 0$ によって定義される、$X$ 上の離散測度であるとします。 $\operatorname{Supp}(\mu) = N$ を示してみましょう。 $a$ のすべての $a \in N$ とすべての近傍 $V$ には、$V$ に含まれるサポートを持つ写像 $f \in \mathscr{K}(X; \mathbf{C})$ が存在し、点 $a$ では 1 に等しく、$N$ のもう一方の点では 0 に等しくなります。 よって $\mu(f) = h(a) \neq 0$。一方、$b \notin N$ の場合、$N$ と交わらない$b$ の近傍$W$ が存在します。したがって、$W$ に含まれるサポートを含むすべての写像 $g \in \mathscr{K}(X; \mathbf{C})$ に対して、$\mu(g) = 0$ が得られ、これは $b \notin \operatorname{Supp}(\mu)$ であることを証明します。

逆に、$\mu$ を、$\operatorname{Supp}(\mu)$ が $X$ の離散的に閉じた部分空間 $N$ となるような尺度とします。すべての $a \in N$ には、$a$ とは異なる $N$ の含む点が存在する、$a$ のオープン近隣 $V_a$ が存在します。したがって、$\mu$ から $V_a$ の制限は、$\{a\}$ (No. 2、提案 5) をサポートする点の測定値であるため、(No. 4、提案 12) は形 $h(a)\varepsilon_a$ になります。 $h(a) \neq 0$。 $\mathbf{C}\mathbf{N}$の点における設定$h(x) = 0$、そして大衆によって定義された尺度$h(x)$を$\nu$で表すと、ローカリゼーションの原理は$\nu = \mu$を示します。

したがって、*離散* 空間 $X$ では、すべてのメジャーが *離散* であることがわかります。

### 練習問題 {#int-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
