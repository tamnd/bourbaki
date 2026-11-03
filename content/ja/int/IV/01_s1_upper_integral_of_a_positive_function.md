---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 1
section_title: Upper integral of a positive function
lang: ja
source: int-i-vi
pdf_pages: 0108-0118, 0225-0227
extraction: ocr
subsections:
    - "no": 1
      title: Upper integral of a lower semi-continuous positive function
      page: 0
      pdf_page: 108
    - "no": 2
      title: Outer measure of an open set
      page: 4
      pdf_page: 111
    - "no": 3
      title: Upper integral of a positive function
      page: 6
      pdf_page: 113
    - "no": 4
      title: Outer measure of an arbitrary set
      page: 10
      pdf_page: 117
statements: 34
exercises: 8
content_sha256: ab99358d7203074ee65ffe3a901cbed9115147b599f62b08cad6cfa296108f8f
translated_from: content/en/int/IV/01_s1_upper_integral_of_a_positive_function.md
translation_method: google
source_content_sha256: faecbc2539033964cc900d67680366e3bd2e09f8e66d8294cd0ca0a84e783552
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f629b4f275cb39de5e7dd2243251f490777e82467eb0b3e1dea059a82e08d76c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。正の上部積分写像

### 1. 下部の半連続正の上部積分写像

X を局所的にコンパクトな空間、$\mu$ を X の正の尺度とします。 $\mu$ は格子 $\mathscr{K}_+(X)$ ($\mathscr{K}_+$ とも表されます) 上では増加する写像であることがわかります。

X 上の数値写像の $\mathscr{I}_+(X)$ (または単に $\mathscr{I}_+$) 集合は、有限かどうかに関係なく、X で正で下位の半連続です。\footnote{1} 写像の任意の族の和を思い出してください。 $\mathscr{I}_+$ 属するから $\mathscr{I}_+$;有限数 $\alpha > 0$ 属するから $\mathscr{I}_+$ による $\mathscr{I}_+$ の写像の積; $\mathscr{I}_+$ の写像の *任意の* ファミリーの上部エンベロープと、 $\mathscr{I}_+$ の写像の *有限* ファミリーの下側エンベロープ、また属するから $\mathscr{I}_+$ (GT、IV, §6, No. 2、提案 2 および Th. 4)。次の補題も利用します。

#### 補題 {#int-iv-s1-n1-lem-1 .statement tag=08P2}

— *すべての写像* $f \in \mathscr{I}_+$ * は、集合* (関係 $\leq$ 向け) *すべての写像* $g \in \mathscr{K}_+$ *そのような* $g \leq f$ の上部エンベロープです。

$f(x) > 0$ のようなすべての $x \in X$ と、$0 < a < f(x)$ のようなすべての実数 $a$ に対して、V に $f(y) \geq a$ がくるような $x$ のコンパクトな近傍 V が仮定までに存在します。一方、点 $x$ および $\leq a$ で $a$ に等しい V にサポートが含まれる写像 $g \in \mathscr{K}_+$ が存在します。

(1) 「劣った」のような「I」。文字 $\mathscr{L}$ (「下位」など) は、§3 で説明する他の写像空間に優先されます。

V (GT、IX, §1, No. 5、Th. 2);したがって、$0 \leq g \leq f$ と $g(x) \geq a$ となり、補題が証明されます。

#### 定義 1 {#int-iv-s1-def-1 .statement tag=08P3}

*$X$ に正の測度 $\mu$ が与えられると、写像 $f \in \mathscr{J}_+$ ($\mu$ に関して) の正の数 (有限または$+\infty$ に等しい) の上積分と呼ばれます*

$$
\mu^*(f) = \sup_{g \in \mathscr{H}_+, g \leq f} \mu(g).
$$

すべての写像 $f \in \mathscr{H}_+$ について、$\mu^*(f) = \mu(f)$ が、他の語 $\mu^*$ が $\mu$ から $\mathscr{J}_+$ の *拡大* であることは明らかです。

#### 例 {#int-iv-s1-n1-exa-1 .statement tag=08P4}

— $X$ を *離散* 空間、$\mu$ を $X$ の正の測度、およびすべての $x \in X$ について集合 $\alpha(x) = \mu(\varphi_{\{x\}})$ とします。 $X$ で定義されたすべての数値写像 $f$ は連続です。 写像 $f \geq 0$、$\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$ については、$\alpha(x) = 0$ と $f(x) = +\infty$ の場合は常に集合 $\alpha(x)f(x) = 0$ に同意します。 のために、
$$
\sum_{x \in X} \alpha(x)f(x) = \sup_M \left( \sum_{x \in M} \alpha(x)f(x) \right),
$$
ここで、$M$ は、$X$ のすべての有限部分集合のうち集合を上回ります。 $f(x_0) = +\infty$ と $\alpha(x_0) > 0$ のような $x_0 \in X$ が存在する場合、$x_0 \in M$ の場合は常に $\sum_{x \in M} \alpha(x)f(x) = +\infty$ となり、逆に、整数 $n > 0$ ごとに $f \geq n \cdot \varphi_{\{x_0\}}$ となるため、$\mu^*(f) \geq n \alpha(x_0)$ となり、$\mu^*(f) = +\infty$ となります。 逆に、$f(x) = +\infty$ で$\alpha(x) = 0$ 点の場合、写像 $g$ は、点 $x \in M$ で$f$ に等しく、$\alpha(x) > 0$ およびその他の場所では 0 属するから $\mathscr{H}_+$ に等しくなります。定められた慣習のおかげで、$\mu(g) = \sum_{x \in M} \alpha(x)f(x)$、これも関係 $\mu^*(f) = \sum_{x \in X} \alpha(x)f(x)$ であることがわかります。

#### 命題 1 {#int-iv-s1-prop-1 .statement tag=08P5}

*すべての有限実数 $\alpha > 0$ およびすべての写像 $f \in \mathscr{J}_+$ に対して、*
$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### 命題 2 {#int-iv-s1-prop-2 .statement tag=08P6}

*集合 $\mathscr{J}_+$ では、写像 $\mu^*$ は増加するです。*
証明はDFの明らかです。 1.

#### 定理 1 {#int-iv-s1-thm-1 .statement tag=08P7}

*$H$ を $\mathscr{J}_+$ の写像の空でない集合とし、関係 $\leq$ に向けます。 $X$ に$\mu$ のポジティブな指標が発生するたびに、*
$$
\mu^*\left( \sup_{g \in H} g \right) = \sup_{g \in H} \mu^*(g) = \lim_{g \in H} \mu^*(g).
$$

$f = \sup_{g \in H} g$ にしましょう。 まず、写像 $g \in H$ とその上部包絡線 $f$ *属するから* $\mathscr{H}_+$ という特殊な場合の定理を証明します。 次に、Dini の定理 (GT, X, §4, No. 1, Th. 1) から、$H$ の切断フィルターは、$X$ のすべてのコンパクト部分集合、特に$f$ のサポート K で *一様に* $f$ に収束します。 写像 $g \in \mathbf{H}$ ごとに $0 \leq g \leq f$ があるため、$\mathbf{H}$ のすべての写像のサポートは $K$ に含まれます。しかし、定義までに、$\mu$は、$K$に含まれるサポートにより、一様収束の位相に対して、連続写像のベクトル空間$\mathscr{K}(X, K; \mathbf{C})$で連続になります。 よって関係この場合は (2) です。

一般的なケースに移りましょう。 写像 $g \in \mathbf{H}$ ごとに $\mu^*(g) \leq \mu^*(f)$ であることは明らかです。デフによる。 1、すべては、$\psi \leq f$ などの写像 $\psi \in \mathscr{K}_+$ ごとに、

$$
\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g).
$$

すべての写像 $g \in \mathbf{H}$ について、$\Phi_g$ を写像 $\varphi \in \mathscr{K}_+$ の集合とし、$\varphi \leq g$ とし、$\Phi$ を集合 $\Phi_g$ の $g$ の和集合とします。 $\mathbf{H}$ を越えます。 $\mathbf{H}$ が指示されているため、$\Phi$ と $f = \sup_{\varphi \in \Phi} \varphi$ も指示されます。 $\psi \leq f$ なので、$\varphi$ が $\Phi$ を超えるため、$\psi$ は写像 $\inf(\psi, \varphi)$ の集合の上位エンベロープになります。しかし、$\psi$ と写像 $\inf(\psi, \varphi)$ 属するから $\mathscr{K}_+$ までなので、証明の最初の部分は $\mu(\psi) = \sup_{\varphi \in \Phi} \mu(\inf(\psi, \varphi))$ を示します。さて、それぞれ $\varphi \in \Phi$ 属するから集合 $\Phi_g$ なので、

$$
\mu(\inf(\psi, \varphi)) \leq \mu(\varphi) \leq \mu^*(g) \leq \sup_{g \in \mathbf{H}} \mu^*(g),
$$

そこからすぐに $\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g)$ が導き出されます。したがって、私たちは $\mu^*(f) = \sup_{g \in \mathbf{H}} \mu^*(g)$ を証明しました。 関係 $\mu^*(f) = \lim_{g \in \mathbf{H}} \mu^*(g)$ は、モノトーン極限定理 (GT、IV, §5, No. 2、Th. 2) の帰結になります。

#### 定理 2 {#int-iv-s1-thm-2 .statement tag=08P8}

*$f_1$ と $f_2$ が $\mathscr{I}_+$ の 2 つの写像である場合*

$$
\mu^*(f_1 + f_2) = \mu^*(f_1) + \mu^*(f_2).
$$

$\varphi_1$ (それぞれ $\varphi_2$) が $\mathscr{K}_+$ で写像の集合を超えるため、 $\varphi_1 \leq f_1$ (それぞれ $\varphi_2 \leq f_2$)、 写像 $\varphi_1 + \varphi_2$ 形有向集合 （$\leq$の場合）その上部エンベロープは$f_1 + f_2$です。したがって、Th によって。 1、

$$
\mu^*(f_1 + f_2) = \sup \mu(\varphi_1 + \varphi_2) = \sup (\mu(\varphi_1) + \mu(\varphi_2)),
$$

ここで、$(\varphi_1, \varphi_2)$ は、$\varphi_1 \leq f_1$ と $\varphi_2 \leq f_2$ のように、$\mathscr{K}_+$ の対の写像の集合を超えます。それ以来

$$
\sup (\mu(\varphi_1) + \mu(\varphi_2)) = \sup \mu(\varphi_1) + \sup \mu(\varphi_2)
$$

(GT、IV, §5, No. 7、Prop. 12 の Cor. 2)、定理が証明されます。

#### 命題 3 {#int-iv-s1-prop-3 .statement tag=08P9}

— *すべての家族* $J_+$の写像中$(f_\iota)_{\iota \in I}$、

$$
\mu^*\left( \sum_{\iota \in I} f_\iota \right) = \sum_{\iota \in I} \mu^*(f_\iota).
$$

$I$ の有限部分集合 $J$ ごとに、Th から続きます。 2 ($J$ の元の数の帰納法まで) $\mu^*\left( \sum_{\iota \in J} f_\iota \right) = \sum_{\iota \in J} \mu^*(f_\iota)$; $J$ は $I$ の有限部分集合の集合、写像 $g_J = \sum_{\iota \in J} f_\iota$ 属するから $J_+$ および関係 $\leq$ の形有向集合を超え、その上部エンベロープは写像 $\sum_{\iota \in I} f_\iota$;したがって、命題は Th から続きます。 1.

#### 命題 4 {#int-iv-s1-prop-4 .statement tag=08PA}

— *$f$ *写像を* $J_+$にしましょう。 *写像* $\mu \mapsto \mu^*(f)$ *集合* $\mathscr{M}_+(X)$ *ポジティブな措置の* $X$、*拡張実直線* $\overline{\mathbf{R}}$へ、*曖昧な位相の* $\mathscr{M}_+(X)$ *(Ch. III, §1, No. 9)*。

なぜなら、この写像は定義による写像$\mu \mapsto \mu(g)$の上側包絡線であり、$g$は$\mathscr{K}_+$の写像の集合を超え、$g \leq f$になります。そして曖昧な位相の定義により、写像$\mu \mapsto \mu(g)$は$\mathscr{M}(X)$に連続します。

### 2. 開いた状態の外側の寸法集合

*オープン* 集合 $G \subset X$ とすると、その特性写像 $\varphi_G$ は、$X$ で *下半連続* になります (GT、IV, §6, No. 2、提案 1 の Cor.)。したがって、次の定義を作成できます。

#### 定義 2 {#int-iv-s1-def-2 .statement tag=08PB}

— *プラスの尺度* $\mu$ *を* $X$ に与えると、 *すべてのオープン集合* $G \subset X$ *上積分* $\mu^*(\varphi_G)$ *は* $G$ の外側の尺度と呼ばれ、* $\mu^*(G)$ と表されます。

したがって、開いた集合 $G$ の外側の尺度は数 $\geq 0$ となり、有限であるか、$+\infty$ に等しくなります。明らかに$\mu^*(\varnothing) = 0$。また、$\mu^*(X) = \| \mu \|,$ は、第 3 章の公式 (22) に示されているとおりです。 III, §1, No. 8。

#### 命題 5 {#int-iv-s1-prop-5 .statement tag=08PC}

— *比較的コンパクトなオープン集合* $G$ の外側の寸法は *有限です*。

なぜなら、この場合、$\varphi_G \leq f$ (Ch. III, §1, No. 2, 補題 1), よってのような写像 $f \in \mathscr{K}_+$ が存在するからです。

$$
\mu^*(G) = \mu^*(\varphi_G) \leq \mu^*(f) = \mu(f) < +\infty.
$$

有限の外部メジャーの開いた集合は、必ずしも比較的コンパクトであるとは限りません (例 3)。

#### 命題 6 {#int-iv-s1-prop-6 .statement tag=08PD}

— *もし* G₁ と G₂ が * G₁ ⊂ G₂ となるような 2 つの開いた集合である場合、* μ*(G₁) ≤ μ*(G₂) となります。
なぜなら、関係 G₁ ⊂ G₂ は φG₁ ≤ φG₂ と同等です。

#### 命題 7 {#int-iv-s1-prop-7 .statement tag=08PE}

— *関係* ⊂ に向けられた* X * のオープン部分集合の集合を * $\mathfrak{B}$ * とします。 *その後*

$$
\mu^*\left(\bigcup_{G \in \mathfrak{B}} G\right) = \sup_{G \in \mathfrak{B}} \mu^*(G).
$$

写像 φ_G 形有向集合 (≤の場合) $\mathscr{I}_+$ とその上部エンベロープは、集合 G ∈ $\mathfrak{B}$ の和集合の特性写像です。したがって、命題は Th の帰結です。 1.

#### 命題 8 {#int-iv-s1-prop-8 .statement tag=08PF}

— *(G_ι)_{ι \in I} *オープン集合の族とする;それから*

$$
\mu^*\left(\bigcup_{\iota \in I} G_\iota\right) \leq \sum_{\iota \in I} \mu^*(G_\iota).
$$

*さらに、* G_ι * がペアで互いに素である場合、*

$$
\mu^*\left(\bigcup_{\iota \in I} G_\iota\right) = \sum_{\iota \in I} \mu^*(G_\iota).
$$

G = $\bigcup_{\iota \in I} G_\iota$ の場合、 φ_G = sup_{ι \in I} φ_{G_ι} ≤ $\sum_{\iota \in I} \varphi_{G_\iota}$; G_ι がペアで互いに素の場合、φ_G = $\sum_{\iota \in I} \varphi_{G_\iota}$;したがって、命題は Props の帰結です。 2と3。

#### 例 {#int-iv-s1-n2-exa-1 .statement tag=08PG}

— X = \mathbf{R} とし、μ を \mathbf{R} のルベーグ測度とする (第 III, §1, No. 3)。 *open 区間* G = ]a, b[ (−∞ ≤ a < b ≤ +∞) の外側の尺度決定するを計算します。まず、a と b が有限であると仮定します。 f ≤ φ_G となる $\mathscr{K}_+$ のすべての写像 f について、平均 (FRV, II, §1, No. 5, 提案 6) の定理により、

$$
\int_{-\infty}^{+\infty} f(x)\, dx = \int_a^b f(x)\, dx \leq b - a,
$$

よって $\mu^*(G) \leq b - a$。一方、$\varepsilon > 0$ ごとに写像 $f \in \mathscr{K}_+$ が存在し、$a + \varepsilon \leq x \leq b - \varepsilon$、よって $\mu^*(G) \geq b - a - 2\varepsilon$ には $f \leq \varphi_G$ と $f(x) = 1$ が存在します。 $\varepsilon$ は任意なので、$\mu^*(G) = b - a$;他の語では、$G$ の外側の尺度は *長さ* に等しくなります。この結果は、$G$ が無制限のオープン区間である場合に即座に拡大するになります。これは、その後、任意に大きい長さの有界オープン区間が含むであるためです。従って、この場合は $\mu^*(G) = +\infty$ となります。

ここで、$G$ を $\mathbf{R}$ のオープン集合とします。 $G$ は、ペアワイズ互いに素開区間 $]a_k, b_k[$ (GT、IV, §2, No. 5、提案 2) の可算集合 (有限または無限) の和集合です。

$$
\mu^*(G) = \sum_k (b_k - a_k)
$$

(提案8);その他語:

#### 命題 9 {#int-iv-s1-prop-9 .statement tag=08PH}

*$\mathbf{R}$のルベーグ測度の場合、$\mathbf{R}$のオープン集合の外側の測度は、接続されている成分の長さの和に等しい。

注意特に、$G$ が $\mu^*(G) = 0$ のように $\mathbf{R}$ でオープンな集合である場合、$G$ は *空* です。

### 3. 正の上部積分写像

$X$ で定義されたすべての数値写像 $f \geq 0$ (有限であるかどうかに関係なく) に対して、$f \leq h$ のような写像 $h \in \mathscr{I}_+$ が存在し、他に定数 $+\infty$ が存在します。

#### 定義 3 {#int-iv-s1-def-3 .statement tag=08PI}

*$\mu$を$X$のプラスの指標とします。 $X$ で定義されたすべての数値写像 $f \geq 0$ (有限かどうか) に対して、正の数*

$$
\mu^*(f) = \inf_{h \geq f, h \in \mathscr{I}_+} \mu^*(h)
$$

(*有限または$+\infty$に等しい) *これは、$f$($\mu$に関して)の上積分と呼ばれます。

このように定義された $f \in \mathscr{I}_+$、数 $\mu^*(f)$ は、定義で定義された上積分と等しくなります。 1、$\mu^*$ は $\mathscr{I}_+$ の増加するであるため。

記法 $\mu^*(f)$ の代わりに、記法 $\int^* f d\mu$、$\int^* f(x) d\mu(x)$、$\int^* f \mu$、$\int^* f(x) \mu(x)$ も使用します。

#### 例 {#int-iv-s1-n3-exa-1 .statement tag=08PJ}

— $X$ が*離散* 空間の場合、$\mu$ は $X$ の正の測度であり、集合 $\alpha(x) = \mu(\varphi_{\{x\}})$ の場合、上で定義されたすべての数値写像 $f \geq 0$ に対して $\mu^*(f) = \sum_{x \in X} \alpha(x) f(x)$ 写像は連続なので、$X$ (No. 1, *例*)。

#### 命題 10 {#int-iv-s1-prop-10 .statement tag=08PK}

— *f と g が、$f \leqslant g$ のように X で定義された 2 つの数値写像 $\geqslant 0$ の場合、$\mu^*(f) \leqslant \mu^*(g)$ になります。*

#### 命題 11 {#int-iv-s1-prop-11 .statement tag=08PL}

— *すべての有限実数 $\alpha > 0$ と X で定義されたすべての数値写像 $f \geqslant 0$ について、

$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### 命題 12 {#int-iv-s1-prop-12 .statement tag=08PM}

— *$f_1$ と $f_2$ が X で定義された 2 つの数値写像 $\geqslant 0$ である場合、

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(f_1) + \mu^*(f_2).
$$

$f_1 \leqslant h_1$ のようなすべての写像 $h_1 \in \mathscr{I}_+$ と $f_2 \leqslant h_2$ のようなすべての写像 $h_2 \in \mathscr{I}_+$ について、Th によって次のようになります。 2、

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(h_1 + h_2) = \mu^*(h_1) + \mu^*(h_2),
$$
よって (GT、IV, §5, No. 7、提案 12 の Cor. 2)

$$
\mu^*(f_1 + f_2) \leqslant \inf_{h_1 \geqslant f_1, h_1 \in \mathscr{I}_+} \mu^*(h_1) + \inf_{h_2 \geqslant f_2, h_2 \in \mathscr{I}_+} \mu^*(h_2),
$$
それは他ならぬ不等式 (9) です。

小道具。 10、11、および 12 は、$\mu^*$ が *増加する、正に均一* であり、X で定義された数値写像 $\geqslant 0$ の集合に *凸* 写像であることを表しています (Ch. I、No. 1)。 $f_1$ と $f_2$ が任意の 2 つの正の写像である場合、(9) の 2 つの要素は必ずしも等しいわけではないことに注意してください (§ 4、Exer. 8 d))。 §5, No. 6 では、等式が成り立つ条件を与えます。

#### 定理 3 {#int-iv-s1-thm-3 .statement tag=08PN}

— *X で定義された数値写像 $\geqslant 0$ の各増加する数列 $(f_n)$ について、

$$
\mu^*\left( \sup_n f_n \right) = \sup_n \mu^*(f_n).
$$

写像 $f_n$ はそれぞれ $\sup_n f_n$ 以下なので、すべては $\mu^*(\sup_n f_n) \leqslant \sup_n \mu^*(f_n)$ である証明になります。 不等式の 2 番目のメンバーが $+\infty$ であれば、これは明らかです。逆の場合、すべての $n$ に対して $\mu^*(f_n) < +\infty$。 $\varepsilon > 0$ごとに、$\mathscr{I}_+$に$f_n \leqslant g_n$と$\mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon$のような*増加する*数列$(g_n)$の写像が存在することを示します。 $g$ が数列 $(g_n)$ の上部エンベロープである場合、$\mu^*(g) = \sup_n \mu^*(g_n)$ (No. 1、Th. 1)、よって $\mu^*(g) \leqslant \sup \mu^*(f_n) + \varepsilon$ になります。 $\sup f_n \leqslant g$ と $\varepsilon$ は任意なので、定理が証明されます。

仮定までに、$f_n \leq h_n$ と $\mu^*(f_n) \leq \mu^*(h_n) \leq \mu^*(f_n) + \varepsilon/2^n$ のような写像 $h_n \in \mathscr{J}_+$ が存在します。 写像 $g_n = \sup(h_1, h_2, \ldots, h_n)$ が要件を満たしていることを示しましょう。それらは属するから$\mathscr{J}_+$、形増加する数列、$n$すべてに対して満たす$f_n \leq g_n$です。私たちはそれを証明してみます

$$
\mu^*(g_n) \leq \mu^*(f_n) + \varepsilon \left( 1 - \frac{1}{2^n} \right).
$$

$n$の帰納法までに議論しましょう。 $n = 1$ の場合は簡単です。一方、$g_{n+1} = \sup(g_n, h_{n+1})$、$g_n \geq f_n$、$h_{n+1} \geq f_{n+1} \geq f_n$、よって $\inf(g_n, h_{n+1}) \geq f_n$;以来

$$
\inf(g_n, h_{n+1}) + \sup(g_n, h_{n+1}) = g_n + h_{n+1},
$$

それはThから導かれます。 No. 1 の 2 つ

$$
\begin{align*}
\mu^*(g_{n+1}) &= \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(\inf(g_n, h_{n+1})) \\
&\leq \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(f_n) \\
&\leq \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^n} \right) + \frac{\varepsilon}{2^{n+1}} \\
&= \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^{n+1}} \right).
\end{align*}
$$

Q.E.D.

#### 系 {#int-iv-s1-n3-cor-1 .statement tag=08PO}

— *$\mathfrak{F}$ を数値写像 $\geq 0$ の集合とし、関係 $\leq$ に向け、$\mathfrak{F}$* (S, III, §1, No. 7) の可算余末​​部分集合 $\mathfrak{G}$ が存在するようにします。それから

$$
\mu^*\left( \sup_{f \in \mathfrak{F}} f \right) = \sup_{f \in \mathfrak{F}} \mu^*(f).
$$

なぜなら、$\mathfrak{G}$ には、$\mathfrak{F}$ と同じ上部エンベロープを持つ関数の増加シーケンスが存在します。$(f_n)$ が任意の順序で配置された$\mathfrak{G}$ の関数シーケンスである場合、$(f_{n_k})$ を条件 $n_1 = 1$、$f_{n_{k+1}} \geq \sup(f_{n_k}, f_k)$ によって再帰的に定義される部分シーケンスとします。この部分列が示された特性を持っていることは明らかです。

#### 注意 {#int-iv-s1-n3-rem-1 .statement tag=08PP}

— 1) $\mathfrak{F}$ が下半連続ではない写像 $\geq 0$ の *不可算* 有向集合である場合、関係 (11) は必ずしも成り立ちません。たとえば、$\mathbf{R}$ のルベーグ測度である $X = \mathbf{R}$、$\mu$ を取り上げ、$\mathbf{R}$ のすべての *有限* 部分集合 M の特性写像 $\varphi_M$ の有向 ($\leq$ の) 集合 $\mathfrak{F}$ を考えます。次に、有限部分集合 M ごとに $\mu^*(\varphi_M) = 0$ です。これは、点が任意に小さい長さの開いた区間に含まれており、集合の特性写像が点に縮小されるため、定義により上積分零が得られます。 No. 2の3および提案9。しかし、$\mathscr{F}$ の上部エンベロープは、1 に等しい定数写像と $\mu^*(1) = +\infty$ です。

2) 写像 $\geqslant 0$ の *減少する* 数列 $(f_n)$ については、すべての $n$ に対して $\mu^*(f_n) < +\infty$ であっても、必ずしも $\mu^*(\inf_n f_n) = \inf_n \mu^*(f_n)$ を持っているわけではないことに注意してください (cf. §4、Exer. 8 c))。

#### 命題 13 {#int-iv-s1-prop-13 .statement tag=08PQ}

*すべての数列* $(f_n)$ *数値写像* $\geqslant 0$ *$X$ で定義されたもの、

$$
\mu^*\left( \sum_{n=1}^\infty f_n \right) \leqslant \sum_{n=1}^\infty \mu^*(f_n).
$$

It suffices to apply the relation (10) to the increasing sequence of functions $g_n = \sum_{k=1}^n f_k$ while taking into account that, by (9),

$$
\mu^*(g_n) \leqslant \sum_{k=1}^n \mu^*(f_k).
$$

§5, No. 6 では、(12) の 2 つの要素が等しい条件を与えます。

#### 命題 14 (ファトゥーの補題) {#int-iv-s1-prop-14 .statement tag=08PR}

— *数値写像* $\geqslant 0$ の数列* $(f_n)$ ごとに、

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \liminf_{n \to \infty} \mu^*(f_n).
$$

整数 $n$、集合 $g_n = \inf_{p \geqslant 0} f_{n+p}$ ごとに; 数列 $(g_n)$ は、(10) により、増加すると $\liminf_{n \to \infty} f_n = \sup_n g_n$、よって、

$$
\mu^*(\liminf_{n \to \infty} f_n) = \sup_n \mu^*(g_n);
$$

しかし、$p \geqslant 0$の$g_n \leqslant f_{n+p}$から、$\mu^*(g_n) \leqslant \mu^*(f_{n+p})$、よって $\mu^*(g_n) \leqslant \inf_{p \geqslant 0} \mu^*(f_{n+p})$、そして最後に

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \sup_n \left( \inf_{p \geqslant 0} \mu^*(f_{n+p}) \right) = \liminf_{n \to \infty} \mu^*(f_n).
$$

#### 系 {#int-iv-s1-n3-cor-2 .statement tag=08PS}

*$(f_n)$ *を数値写像* $\geqslant 0$ の数列とし、*すべて* $x \in X$、$\lim_{n \to \infty} f_n(x) = +\infty$ となるようにします。 ** $\mu$ *が零の尺度ではない場合*、* $\lim_{n \to \infty} \mu^*(f_n) = +\infty$。

$f_0$ が $+\infty$ に等しい定数写像である場合、$f_0$ は $\mathscr{K}_+$ のすべての写像の上部エンベロープであり、$\mu \neq 0$ 以降、$\mu^*(f_0) > 0$ になります。しかし、$\alpha > 0$ ごとに $f_0 = \alpha f_0$ なので、必然的に $\mu^*(f_0) = +\infty$ になります (提案 11)。 不等式 (13) は、$\mu^*(f_n)$ が $n$ とともに $+\infty$ になる傾向があることを示しています。

#### 命題 15 {#int-iv-s1-prop-15 .statement tag=08PT}

*すべてのスカラー $\alpha > 0$ および $X$ のポジティブ指標 $\mu, \nu$ のすべての対について、*

$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + \nu)^* = \mu^* + \nu^*.
$$

*さらに、関係 $\mu \leq \nu$ は $\mu^* \leq \nu^*$ を意味します。*

関係 (15) を証明しましょう。 集合 $\lambda = \mu + \nu$;したがって、$\lambda(f) = \mu(f) + \nu(f)$ は $f \in \mathscr{K}_+$ になります。 $f \in \mathscr{J}_+$、$\lambda^*(f)$の値（それぞれ$\mu^*(f)$、$\nu^*(f)$）は、$g$が有向集合を超えるため、$\lambda(g)$（それぞれ$\mu(g)$、$\nu(g)$）の極限になります。 $\leq$) すべての $g \in \mathscr{K}_+$ のうち $g \leq f$ となる;したがって$\lambda^*(f) = \mu^*(f) + \nu^*(f)$。 最後に、$f$ が $X$ で定義されたいずれかの写像 $\geq 0$ である場合、$\lambda^*(f)$ (それぞれ $\mu^*(f)$、$\nu^*(f)$) は、次のように $\lambda^*(h)$ (それぞれ $\mu^*(h)$、$\nu^*(h)$) の極限になります。 $h$ は、$h \geq f$ のように、すべての写像 $h \in \mathscr{J}_+$ のうち有向集合 ($\geq$ の場合) を実行します。再び、極限に進むと、$\lambda^*(f) = \mu^*(f) + \nu^*(f)$ が得られ、これは (15) を証明します。 関係 (14)も同様に成立します。 最後に、$\mu \leq \nu$ の場合、$\nu - \mu \geq 0$ である$\nu = \mu + (\nu - \mu)$ と書くことができ、したがって $\nu^* = \mu^* + (\nu - \mu)^*$ となり、$\mu^* \leq \nu^*$ であることがわかります。

### 4. 任意の集合の外側のメジャー

#### 定義 4 {#int-iv-s1-def-4 .statement tag=08PU}

*$\mu$ を $X$ に対するプラスの尺度とします。 $X$ の部分集合 $A$ ごとに、上部積分 $\mu^*(\varphi_A)$ は $A$ の外側の尺度 (尺度 $\mu$ に関して) と呼ばれ、$\mu^*(A)$ と表されます。

したがって、集合の外側のメジャーは数 $\geq 0$ であり、有限か、または $+\infty$ に等しいことになります。つまり、定義で定義された外側のメジャーを使用したオープン集合の場合、一致するです。 No. 2の2。

#### 命題 16 {#int-iv-s1-prop-16 .statement tag=08PV}

*$A$ と $B$ が $X$ の 2 つの部分集合で、$A \subset B$ である場合、$\mu^*(A) \leq \mu^*(B)$ です。*

#### 系 {#int-iv-s1-n4-cor-1 .statement tag=08PW}

*$X$ の比較的コンパクトなすべての集合には、有限の外側寸法があります。*

なぜなら、そのような集合は、比較的コンパクトな開いた集合 (GT、I, §9, No. 7、提案 10) に含まれており、その外側の尺度は有限です (No. 2、提案 5)。

#### 命題 17 {#int-iv-s1-prop-17 .statement tag=08PX}

— ** $(A_n)$ * が X* の部分集合の増加する数列である場合、$\mu^*(\bigcup_n A_n) = \sup_n \mu^*(A_n)$。

#### 命題 18 {#int-iv-s1-prop-18 .statement tag=08PY}

— *数列* $(A_n)$ *の部分集合の X* ごとに、

$$
\mu^*\left(\bigcup_n A_n\right) \leq \sum_n \mu^*(A_n).
$$

これらの命題は Props の翻訳です。 １０および１３およびＴｈ． 集合の特性写像に対して No. 3 の 3。

#### 命題 19 {#int-iv-s1-prop-19 .statement tag=08PZ}

— *X* の各部分集合 A について、$\mu^*(A)$ * はオープン集合含む A* の外側の寸法の下限です。

$\mu^*(A) = +\infty$なら命題は明らかです。逆の場合、$0 < \varepsilon < 1$ のようなすべての $\varepsilon$ に対して、$\varphi_A \leq f$ と $\mu^*(A) \leq \mu^*(f) \leq \mu^*(A) + \varepsilon$ のような写像 $f \in \mathscr{J}_+$ が存在します。 G を $f(x) > 1 - \varepsilon$ となるような $x \in X$ の集合とします。 $f$ は下半連続であるため、G は *オープン* (GT、IV, §6, No. 2、提案 1) および含む A;一方、$f \geq (1 - \varepsilon)\varphi_G$、よって

$$
\mu^*(G) \leq \frac{1}{1 - \varepsilon} \mu^*(f) \leq \frac{1}{1 - \varepsilon} (\mu^*(A) + \varepsilon);
$$

$\varepsilon$ は任意であるため、$\mu^*(G)$ は $\mu^*(A)$、よって命題と必要最小限の差があることがわかります。

### 練習問題 {#int-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
