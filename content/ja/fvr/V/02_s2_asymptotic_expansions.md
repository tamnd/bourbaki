---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 2
section_title: ASYMPTOTIC EXPANSIONS
lang: ja
source: fvr-i-vii
book_pages: 220-227
pdf_pages: 0235-0242
extraction: ocr
subsections:
    - "no": 1
      title: SCALES OF COMPARISON
      page: 220
      pdf_page: 235
    - "no": 2
      title: PRINCIPAL PARTS AND ASYMPTOTIC EXPANSIONS
      page: 221
      pdf_page: 236
    - "no": 3
      title: SUMS AND PRODUCTS OF ASYMPTOTIC EXPANSIONS
      page: 223
      pdf_page: 238
    - "no": 4
      title: COMPOSITION OF ASYMPTOTIC EXPANSIONS
      page: 224
      pdf_page: 239
    - "no": 5
      title: ASYMPTOTIC EXPANSIONS WITH VARIABLE COEFFICIENTS
      page: 226
      pdf_page: 241
statements: 12
exercises: 0
content_sha256: f5a6dcf5257f33068e794cc5483f30825ac51b768404ffe2efc061f3a217aec3
translated_from: content/en/fvr/V/02_s2_asymptotic_expansions.md
translation_method: google
source_content_sha256: 3913fa9ae08c74aef17f721c054e1ae91ca2d4d4ef6bc764fb678147ac681601
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b498ea02bb9bb35d55036710d9fdd6b25b7c8b3cd1bda159589262ac445468e1
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。漸近展開

### 1. 比較の尺度

E を基底 $\mathfrak{F}$ のフィルターでフィルター処理した集合とし、K を非離散値体 (ほとんどの場合、$K = \mathbf{R}$ または $K = \mathbf{C}$) とします。 $\mathscr{H}(\mathfrak{F}, K)$の写像の集合は、0モジュロ$R_\infty$と等価ではありません（つまり、$\mathfrak{F}$のすべての集合に、写像が消えない点が少なくとも1つあるもの）、関係」 $f \ll g$ または $f = g$」は位数関係です。

#### 定義 1 {#fvr-v-s2-def-1 .statement tag=08ES}

*ある人は、0モジュロ$R_\infty$に等価でない関数で構成される$\mathscr{H}(\mathfrak{F}, K)$の部分集合$\mathscr{E}$は、$\mathscr{E}$が関係「$f \ll g$または$f = g$」によって完全に順序付けされるときの比較スケールであると言います。

他の語では、$f$と$g$が$\mathscr{E}$の写像であれば、関係$f \ll g$、$g \ll f$、$f = g$のうちの1つ（そして1つだけ）が常に成り立ちます。その結果、$\mathscr{E}$ *関係* $f \asymp g$ (および *なおさら* $|f| \sim a\,|g|$、$a$ は数 $> 0$) *暗黙* $f = g$ になります。

比較スケールのすべての部分集合は明らかに比較スケールでもあります。

#### 例 1 {#fvr-v-s2-n1-exa-1 .statement tag=08ET}

$x$ が実際で、写像 $x^\alpha$ ($\alpha$ は任意の実数) の$+\infty$ 集合になる傾向があるため、比較スケールです。 $\mathfrak{F}$ が左側のエンドポイント $a$ でオープン区間の集合である場合、写像 $(x-a)^\alpha$ にも同じことが当てはまります。

#### 例 2 {#fvr-v-s2-n1-exa-2 .statement tag=08EU}

写像 $z^n$ の $\infty$ 集合 ($n$ 有理数整数) の傾向にある $z$ 複合体は比較尺度です。 $\mathfrak{F}$ がこの点の近傍のフィルターの点 $a \in \mathbf{C}$ の補数のトレースである場合、写像 $(z-a)^n$ も同様です。

#### 例 3 {#fvr-v-s2-n1-exa-3 .statement tag=08EV}

F を空間と正規化します。 写像 $\|x-\mathbf{a}\|^\alpha$ ($\alpha$ は任意の実数) のファミリーは、$\mathfrak{F}$ がこの点の近傍のフィルターの$\mathbf{a}$ の補数のトレースであるときの比較スケールです。 $p$ と $q$ が F 上の 2 つの異なるノルムである場合、2 つの比較スケール $(p(x-\mathbf{a}))^\alpha$ と $(q(x-\mathbf{a}))^\alpha$ の和集合は一般に比較スケールではないことに注意してください。

#### 例 4 {#fvr-v-s2-n1-exa-4 .statement tag=08EW}

$x$ 実数の傾向が $+\infty$ の場合、形 $\exp(p(x))$ の写像の家族 $\mathscr{E}$ では、$p$ は定数項* なしの * 多項式 (実数係数あり) の集合を実行し、比較になります。スケール: $\mathscr{E}$ の 2 つの写像のうち商が再び $\mathscr{E}$ にあること、および $p \neq 0$ の場合、写像 $\exp(p(x))$ は 0 または $+\infty$ のいずれかになる傾向があることに注意するだけで十分です。確かに、$p(x) \sim \alpha x^n$ ここで、$n > 0$ と $\alpha \neq 0$; $\alpha > 0$ の場合、$x$ 十分大きいの場合は $p(x) > \frac{1}{2} \alpha x^n$。 $\alpha < 0$ の場合、$x$ 十分大きいの場合は $p(x) < \frac{1}{2} \alpha x^n$。最初のケースでは $\exp(p(x))$ は $+\infty$ になる傾向があり、2 番目のケースでは 0 になる傾向があります。

#### 例 5 {#fvr-v-s2-n1-exa-5 .statement tag=08EX}

$x$ の実質は $+\infty$ 集合 $\mathscr{E}$ の写像の形 $x^\alpha (\log x)^\beta$ ($x > 1$ で定義) の場合、$\alpha$ と $\beta$ は任意です実数は比較スケールです。実際、ここでも、$\mathscr{E}$ の 2 つの写像のうち商は、$\mathscr{E}$ では写像です。 $\alpha$ と $\beta$ が両方とも零ではない場合、$x^\alpha (\log x)^\beta$ は 0 または $+\infty$ になる傾向があることを示すだけで十分です。 $\alpha = 0, \beta \neq 0$ であればこれは明らかです。 $\alpha > 0$ の場合は $(\log x)^{-\beta} \ll x^\alpha$ があり、$\alpha < 0$ の場合は $\beta$、よって命題のいずれかに対して $(\log x)^\beta \ll x^{-\alpha}$ があります。

この最後の比較スケールは完全に順序付けられた集合 (関係 "f $\ll$ g" または $f = g$" の場合) であり、その位数構造は $\mathbf{R}^2$ (*集合の *辞書編集* 位数) と同型であることに注意してください。 理論*、III、p. 157); この構造関係 $(\alpha, \beta) < (\gamma, \delta)$ は「$\alpha < \gamma$、または $\alpha = \gamma$ および $\beta < \delta$」を意味することを思い出してください。

同様に、写像 $\exp(p(x))$ によって形成されるスケールは、$p$ が定数項を持たない多項式の集合 $P_0$ を通過し、位数構造は次の位数構造と同型です。 $P_0$、ここで関係 $p < q$ は、多項式 $q - p$ の支配的な項が係数 $> 0$ (*cf. Alg.*, VI. 19, *例) を持つことを意味します。 2*)。

$\varphi$ を集合 F から E までの写像とし、$\varphi^{-1}(\mathfrak{F})$ が F のフィルター 基底であるようにします。 $\mathscr{E}$ が E の比較スケール (フィルター 基底 $\mathfrak{F}$ の場合) である場合、写像 $f \circ \varphi$ は次のようになります。 $f$ は、F の比較スケール $\mathscr{E}$、形を実行します (フィルター 基底 $\varphi^{-1}(\mathfrak{F})$ の場合)。

### 2. 主部分と漸近展開

$\mathscr{E}$ を、非離散値体 K の写像と値によって形成される比較スケールとします。V を K 上の標準値空間とし、$\mathbf{f}$ を $\mathscr{H}(\mathfrak{F}, V)$ の写像とします。 V に $\mathbf{f} \sim \mathbf{a}g$ となる写像 $g \in \mathscr{E}$ と元 $\mathbf{a} \neq 0$ がある場合、$\mathbf{a}g$ はスケール $\mathscr{E}$ に対して $\mathbf{f}$ の *主部分* であると言います。デフから。 V、p. 10、$\mathbf{f}$ の 1 は、$\mathscr{E}$ に対して *1 つだけ* のプリンシパル部分を持つことができます。これは、$g_1,\ g_2$ が $\mathscr{E}$ で 2 つの写像であり、$\mathbf{a}_1,\ \mathbf{a}_2$ が 2 つの $\neq 0$ である場合です。 V の元は、関係 $\mathbf{a}_1 g_1 \sim \mathbf{a}_2 g_2$ は $|g_1| \asymp |g_2|$ を意味し、その結果、$g_1 = g_2$、よって $(\mathbf{a}_2 - \mathbf{a}_1)g_1 \ll g_1$ となり、$g_1$ はどの点でも同じ零ではないため、 $\mathscr{E}$ の集合は、$\mathbf{a}_2 = \mathbf{a}_1$ を意味します。

$\mathbf{f}$ が比較スケール $\mathscr{E}$ に対して主成分部分を持つ場合、すべての比較スケール $\mathscr{E}' \supset \mathscr{E}$ に対して *同じ* 主成分部分を持ちます。

#### 例 1 {#fvr-v-s2-n2-exa-1 .statement tag=08EY}

$+\infty$ (それぞれ $\infty$) に傾向する$x$ 実数 (それぞれ複素数) の場合、V で係数を含むすべての多項式 $a_0 x^n + a_1 x^{n-1} + \ldots + a_n$ は、$a_0 \neq 0$ となり、スケールに関して主部分 $a_0 x^n$ を持ちます。 $x^n$ (または任意のスケール含むまたは $x^n$)。従って、$a_0 b_0 \neq 0$ が同じスケールに関して主部分 $\frac{a_0}{b_0} x^n$ を持つような実数または複素数係数を持つすべての有理分数 $\frac{a_0 x^n + \cdots + a_m}{b_0 x^n + \cdots + b_n}$ が得られます。

#### 例 2 {#fvr-v-s2-n2-exa-2 .statement tag=08EZ}

写像は、スケールのすべての写像に匹敵する可能性がありますが、このスケールに関して主要な部分は認められません。たとえば、実質 $x$ が $+\infty$ に向かう傾向がある場合、$\sqrt{x}$ にはスケール $x^n$ に関して元本部分がありません。ここで、$n$ は有理数整数です。 $\log x$ には、$x^\alpha$ ($\alpha$ 任意の実数) のスケールに関して元本部分がありません。 $\exp(\sqrt{\log x})$ と $x' = e^{x \log x}$ には、$x^\alpha (\log x)^\beta$ のスケールに関しても、$\exp(p(x))$ のスケールに関しても主部分がありません ($p$ 定数項を持たない多項式)。

プリンシパル部分の概念は広範な一般化を認めます。 写像 $f \in \mathscr{H}(\mathfrak{F}, V)$ がスケール $\mathscr{E}$ に関して主成分部分 $a_1 g_1$ を持っていると仮定します。 関係 $f \sim a_1 g_1$ は $f - a_1 g_1 \ll g_1$ (V、p. 216、デフォルト 4) と同等です。 写像 $f$ をより詳しく研究すると、写像 $f - a_1 g_1$ を検討するようになります。この写像に $\mathscr{E}$ に関してプリンシパル部分 $a_2 g_2$ がある場合、$g_2 \ll g_1$ と $f - a_1 g_1 - a_2 g_2 \ll g_2$ がなければなりません。

より一般的には、スケール $\mathscr{E}$ が形 $(g_\alpha)$ でパラメトリックに書かれており、$\alpha$ が添字 $A$ の集合を通過し、位数の *反対* と同型の完全に順序付けられた構造を備えていると仮定します。 $\mathscr{E}$ の構造: 関係 $\alpha < \beta$ は、$g_\beta \ll g_\alpha$ と同等です。このような状況では:

#### 定義 2 {#fvr-v-s2-def-2 .statement tag=08F0}

*ある人は、 写像* $f \in \mathscr{H}(\mathfrak{F}, V)$ *精度への漸近展開を認める* $g_\alpha$ *(スケール* $\mathscr{E}$* に対して) *家族が存在する場合* $(a_\lambda)_{\lambda \leq \alpha}$ *of 元 of* $V$、 *有限を除くすべて数そのうち* $0$、*そのような* $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$。 *ある人は* $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ * は* $f$ * 正確に* $g_\alpha$ の漸近展開であり、 * $a_\lambda g_\lambda$ ($\lambda \leq \alpha$) * はその項であり、* $a_\lambda$ * は係数であり、 写像* $r_\alpha = f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ *この拡張の残り*。

$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ が $f$ の精度への漸近展開であるという事実を表現するには、$g_\alpha$ が最も頻繁に制限するを書くことになります。

$$
f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o(g_\alpha) \quad \text{(or } f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o_k(g_\alpha)
$$

V、p. 219、220 の記法に続く証明に複数の写像がある場合。

同じスケール$\mathscr{E}$に対する2つの漸近展開（異なるかどうかにかかわらず、2つの写像）のうち、精度が添字より大きい方が*より正確*であると言われます。

$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ が $f$ の精度 $g_\alpha$ への漸近展開である場合、$\beta < \alpha$ ごとに、$\sum_{\lambda \leq \beta} a_\lambda g_\lambda$ は $f$ の精度 $g_\beta$ への漸近展開になります (V, p. 215、prop. 5): $f$ から $g_\beta$ への与えられた展開 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ の *精度を下げる* ことによって得られると言われています。

$\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ と $\sum_{\lambda \leq \alpha} b_\lambda g_\lambda$ が 2 つの写像 $f_1, f_2$ の *同じ* 精度 $g_\alpha$ への漸近展開である場合、$\sum_{\lambda \leq \alpha} (a_\lambda + b_\lambda) g_\lambda$ は、$f_1 + f_2$ の精度 $g_\alpha$ (V, p. 215,提案5）。そして、すべてのスカラー $c$ について、$\sum_{\lambda \leq \alpha} a_\lambda c g_\lambda$ は、$f_1 c$ を精度 $g_\alpha$ に漸近展開します。したがって、写像が精度 $g_\alpha$ への漸近展開を許容する場合、この展開は *ユニーク* であるということになります。 写像 0 が係数 $\neq 0$ を持つ精度 $g_\alpha$ での漸近展開を許容しないことがわかるだけで十分です。というのは、$0 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$ と、$\gamma$ が添字 $\lambda \leq \alpha$ の最小値で、$a_\lambda \neq 0$ だったら、$a_\gamma g_\gamma = - \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda - r_\alpha \ll g_\gamma$ になるからですが、これは不合理です。

写像 $f$ が、係数がすべて *零* である精度 $g_\alpha$ への漸近展開を認めると言うのは、$f \ll g_\alpha$ のというと同等です。 $f$ が、係数がすべて零ではない精度 $g_\alpha$ への漸近展開 $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ を許容し、$\gamma$ が $a_\lambda \neq 0$ となる添字 $\lambda$ の最小のである場合、$a_\gamma g_\gamma$ $f - a_\gamma g_\gamma = \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha \ll g_\gamma$ があるため、スケール $\mathscr{E}$ に対する $f$ の *主部分* です。同様に、$\mu \leq \alpha$ が $a_\mu \neq 0$ となるような添字である場合、$a_\mu g_\mu$ は $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$ の主部分になります。

アプリケーションにおける最も重要な漸近展開は、$x^{-n}$ (それぞれ $z^{-n}$) のスケールに関連したもので、$n$ は正または負の整数です。$x$ は $+\infty$ または $-\infty$ (複素数 $z$ が$\infty$)、または実数 $x$ が右または左から $c$ になる傾向がある場合 (それぞれ、複素数 $z$ が $c$ になる傾向がある場合) は、$(x - c)^n$ (または $(z - c)^n$) のスケールに相対します。 I, p. 21 で、点 $c \in \mathbf{R}$ で $k$ 回微分可能である実変数 $x$ のすべてのベクトル写像は、この点で位数 $k$ のテイラー展開を許容します。つまり、$(x - c)^n$ のスケールに関して精度 $(x - c)^k$ に漸近拡張します。

### 3. 漸近展開の和と積

$f_1, f_2$ が、比較スケール $\mathscr{E}$ と比較して、精度 $g_\alpha$ と $g_\beta$ への漸近展開をそれぞれ認める場合、2 つの展開をこの精度に *制限*することで、精度 $g_{\min(\alpha, \beta)}$ への展開を推定します。 V、p. 222 で、$f_1 + f_2$ を精度 $g_{\min(\alpha, \beta)}$ まで漸近展開する方法を見てきました。

$V_1, V_2$ と $V$ を体 $K$ 上の 3 ノルム空間とし、$(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}. \mathbf{y}]$ を $V_1 \times V_2$ から $V$ までの*連続双線形写像* とします。さらに、この切断の残りについて、スケール $\mathscr{E}$ は、$\mathscr{E}$ の任意の 2 つの写像の *積* が再び $\mathscr{E}$ になるようなものであると仮定します (これは、例 (V では、 p. 220))。

ここで、$f_1, f_2$ をそれぞれ $\mathscr{H}(\mathfrak{F}, V_1)$ と $\mathscr{H}(\mathfrak{F}, V_2)$ の 2 つの写像とし、スケール $\mathscr{E}$ に関して、それぞれ精度 $g_\alpha$ と$g_\beta$ に漸近拡張$f_1 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$ と$f_2 = \sum_{\mu \leq \beta} b_\mu g_\mu + r_\beta$ を持たせます。さらに、$a_\lambda$ も $b_\mu$ もすべて零ではないと仮定し、$a_\gamma g_\gamma$ と $b_\delta g_\delta$ を $f_1$ と $f_2$ の主部分とします。 仮定までに、$g_\gamma g_\beta = g_\rho$ と $g_\delta g_\alpha = g_\sigma$ を書くことができます。 和 $\sum [\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$ がすべての対 $(\lambda, \mu)$ を引き継ぎ、$g_{\min(\rho, \sigma)} \ll g_\lambda g_\mu$ が $[f_1.f_2]$ の *正確さ* $g_{\min(\rho, \sigma)}$ の *漸近展開であることを示しましょう。さて、$[f_1.f_2]$ とこの和の差は、項の有限数の和であり、それぞれは形 $[\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$ と $g_\lambda g_\mu \ll g_{\min(\rho, \sigma)}$ 、または形 $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda$ のいずれかです。 $\lambda \geq \gamma$、または形 $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu$ の場合、$\mu \geq \delta$;しかし $[\mathbf{x}. \mathbf{y}]$ は連続なので、(V, p. 213, prop. 3 と V, p. 215, prop. 6) から $\lambda \geq \gamma$ に対して $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda \preccurlyeq \mathbf{r}_\beta g_\lambda \ll g_\beta g_\gamma = g_\rho$ が得られ、同様に $\mu \geq \delta$ に対して $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu \preccurlyeq \mathbf{r}_\alpha g_\mu \ll g_\alpha g_\delta = g_\sigma$ が得られます。 よって命題 (V、p. 215、提案 5)。

すべての $\mathbf{a}_\lambda$ が零の場合、1 つは $[f_1.f_2] \ll g_\alpha g_\delta$ になります。他の語では、零項で精度 $g_\alpha g_\delta$ までの $[f_1.f_2]$ が漸近展開されます。同様に、すべての $\mathbf{a}_\lambda$ と $\mathbf{b}_\mu$ が零である場合、零項の精度 $g_\alpha g_\beta$ で $[f_1.f_2]$ が漸近展開されます。

前述の結果を主に、V が K 上の *ノルム代数* であり、双線形写像 $[\mathbf{x}. \mathbf{y}]$ がこの代数の積 xy である場合に適用します。最も重要なケースは、V が $\mathbf{R}$ または $\mathbf{C}$ に等しい場合です。

特に、$f_i$ ($1 \leq i \leq n$) が $\mathscr{H}(\mathfrak{F}, K)$ の n 写像であり、それぞれが $\mathscr{E}$ に関して漸近展開できる場合、$f_i$ のすべての*多項式* $\sum_{(v_i)} \mathbf{a}_{v_1 v_2} v_n f_1^{v_1} \ldots f_n^{v_n}$ について、$\mathscr{E}$ に関して漸近展開を得ることができます。正規の空間 V の係数;さらに、前述の規則により、写像 $f_i$ の展開の精度がわかっていれば、得られる展開の精度を決定する知ることができます。

### 4. 漸近展開の合成

$f$ を $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ (それぞれ $\mathscr{H}(\mathfrak{F}, \mathbf{C})$) で写像とし、スケール $\mathscr{E}$ に関して精度 $g_\alpha$ への漸近拡張を認め、基底 $\widetilde{\mathfrak{F}}$ のフィルターに沿って * 極限* 0 を持ちます。一方、$\mathbf{h}$ を $\mathbf{R}$ の点 0 の近傍で定義された、$\mathbf{R}$ 上の正規化空間 V (それぞれ $\mathbf{C}$) で値を伴う写像とします。 (それぞれ $\mathbf{C}$)、この近傍では *n 回微分可能*です。それから

$$
\mathbf{h}(t) = c_0 + c_1 t + \cdots + c_n t^n + o(t^n)
$$

この近傍 (I、p. 21)、よって、$\widetilde{\mathfrak{F}}$ の適切な集合

$$
\mathbf{h} \circ f = c_0 + c_1 f + \cdots + c_n f^n + o(f^n).
$$

n 3 では、$f$ の展開の精度によって決まる精度 $g_\rho$ まで $c_0 + c_1 f + \cdots + c_n f^n$ を漸近展開する方法形を見てきました。さらに、$f$の漸近展開の係数がすべて零ではなく、$a_\gamma g_\gamma$が$f$の主部分であると仮定し、$g_\sigma = g_\gamma^n$とします。 $\sigma < \rho$ の場合、$\sum_{k=0}^n c_k f^k$ の展開をこの精度に制限すると、$\mathbf{h} \circ f$ の展開が精度 $g_\sigma$ になります。逆に、$\rho \leq \sigma$ の場合、$\sum_{k=0}^n c_k f^k$ の展開は、$\mathbf{h} \circ f$ の精度 $g_\rho$ への展開でもあります。

$f$ の漸近展開のすべての項が零で、$g_\alpha \ll 1$ の場合、$f \ll g_\alpha$ となり、整数 $k > 0$ ごとに $f^k \ll g_\alpha^k \ll g_\alpha$ となります。 $c_m$ が零ではない添字 $> 0$ の最初の係数である場合 (添字 $k > 0$ の $c_k$ がすべて 0 ではないと仮定して)、$c_0$ は次の漸近展開です。 $h \circ f$ から精度 $g_\alpha^m$ まで。

この切断の残りでは、$\mathscr{E}$の写像が実数値を持ち、$\mathfrak{F}$の集合に対して厳密に正である場合に限定し、$\mathscr{H}(\mathfrak{F}, \mathbf{R})$の写像の漸近展開のみを考慮します。まず、すべての写像 $g \in \mathscr{E}$ とすべての実数 $\nu$、$g^\nu$ が再び属するから $\mathscr{E}$ まで: この条件は、たとえば $x^\alpha$ のスケールまたは $x^\alpha |\log x|^\beta$ のスケールによって満たされるとします。 ($\alpha$ と $\beta$ は任意の実数) $+\infty$ の近傍または $\mathbf{R}$ の 0 の近傍。この性質は、$\mathscr{E}$の2つの写像の商が再び属するから$\mathscr{E}$になることを意味します。そうなると、写像 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ の $\mathscr{E}$ に対する漸近展開から、精度 $g_\alpha$ まで、実数 $\nu$ ごとに $|f|^\nu$ の展開を導出できます。 $f$ の展開の係数がすべて零ではない場合に限定し、$a_\gamma g_\gamma$ を $f$ の主部分とします。 $|f|^\nu = |a_\gamma|^\nu g_\gamma^\nu (1 + h)^\nu$ と書くことができます。
$$
h = \sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} + o \left( \frac{g_\alpha}{g_\gamma} \right).
$$
私たちの仮説では、$\sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma}$ は $h$ の漸近展開であり、精度は $g_\alpha / g_\gamma$ になります。 $h$ は $\mathfrak{F}$ 方法に沿って 0 になる傾向があるため、上記で説明した $(1 + h)^\nu$ の漸近展開が得られ、その後 $|a_\gamma|^\nu g_\gamma^\nu$ を乗算すると $|f|^\nu$ の展開が得られます。

$f$ についても同じ仮説を立てて次のように書くことができます。
$$
\log |f| = \log |a_\gamma g_\gamma| + \log (1 + h)
$$
そして、上で述べたように、$\log (1 + h)$ は拡張でき、写像 $\log (1 + t)$ は 0 の近傍で無限に微分可能です。さらに、$\log g_\gamma$ が $\mathscr{E}$ に関して、またはスケール $\mathscr{E}_1 \supset \mathscr{E}$ に関して漸近展開を認める場合、2 つの漸近展開を加算すると、$\log |f|$ の漸近展開が得られます。

#### 例 {#fvr-v-s2-n4-exa-1 .statement tag=08F1}

$(1 + x)^{1/x} = \exp \left( \frac{1}{x} \log (1 + x) \right)$: $x$ が $+\infty$ になる傾向があるとき、$x^\alpha (\log x)^\beta$ のスケールに対する $\frac{1}{x} \log (1 + x)$ の漸近展開は $\log (1 + x) = \log x + \log \left( 1 + \frac{1}{x} \right)$、よってになります。
$$
\frac{1}{x} \log (1 + x) = \frac{\log x}{x} + \frac{1}{x^2} - \frac{1}{2x^3} + o_1 \left( \frac{1}{x^3} \right).
$$
この展開とテイラー展開から
$$
e^u = 1 + u + \frac{u^2}{2} + \frac{u^3}{6} + o(u^3)
$$

$u = 0$ の近傍では、漸近展開が推定されます。

$$
(1 + x)^{1/x} = 1 + \frac{\log x}{x} + \frac{1}{2} \frac{(\log x)^2}{x^2} + \frac{1}{x^2}
+ \frac{1}{6} \frac{(\log x)^3}{x^3} + \frac{\log x}{x^3} - \frac{1}{2x^3} + o_2 \left( \frac{1}{x^3} \right)
$$

上で説明した$x^\alpha (\log x)^\beta$×方法のスケールに関して。

同じ仮説と記法を維持すると、$e^f$ の漸近展開は、$f \gg 1$ の場合を除いて、新しい問題を提起しません。次に、2 つの場合を $g_\alpha \gg 1$ または $g_\alpha \ll 1$ として区別する必要があります。最初のケースでは、$f$ の拡張を行っても、$\mathscr{E}$ に対する$e^f$ の元本部分を取得することはできません。これは、剰余 $r_\alpha$ が 0 になる傾向があるかどうか、つまり、$e^{r_\alpha}$ が 1 になる傾向があるかどうかが一般にわからないためです。逆に、$g_\alpha \ll 1$ の場合は、 $r_\sigma \ll 1$ そして$e^f \sim \exp \left( \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \right)$。この結果をより正確にすることができます。$a_\gamma g_\gamma$ を $f$ の主部分とし、$\delta$ を $g_\delta = 1$ の$\gamma < \delta \leq \alpha$ である添字とします。 $f_1 = \sum_{\lambda \leq \delta} a_\lambda g_\lambda$、$f_2 = \sum_{\delta < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$を置きます。 $f = f_1 + f_2$ があるので、$e^f = e^{f_1} e^{f_2}$ となり、この小節の冒頭で説明した一般的な方法により、$e^{f_2}$ の漸近展開形が可能になります (点 $t = 0$ での $e^t$ のテイラー展開から始まります)。次に、$e^{f_1} = \prod_{\lambda \leq \delta} \exp(a_\lambda g_\lambda)$ 属するから $\mathscr{E}$ まで、またはスケール $\mathscr{E}_1$ 含む $\mathscr{E}$ の場合、$e^f$ は漸近展開します。

#### 例 {#fvr-v-s2-n4-exa-2 .statement tag=08F2}

$x^{1/1} = \exp \left( \log x \cdot \exp \left( \frac{1}{x} \log x \right) \right)$ があります。 $x$ が $+\infty$ になる傾向がある場合、スケール $x^\alpha (\log x)^\beta$ に関して $\log x \cdot \exp \left( \frac{1}{x} \log x \right)$ の漸近展開が $\log x \ll x$、よってになります。

$$
\log x \cdot \exp \left( \frac{1}{x} \log x \right) = \log x + \frac{(\log x)^2}{x} + \frac{1}{2} \frac{(\log x)^3}{x^2} + o \left( \frac{(\log x)^3}{x^2} \right).
$$

この展開のすべての項は 2 番目から始まり 0 になる傾向があります。この展開と、$u = 0$ の近傍上の Taylor 展開 $e^u = 1 + u + u^2/2 + o(u^2)$ から、次のように推測できます。

$$
x^{1/1} = 1 + (\log x)^2 + \frac{1}{2} \frac{(\log x)^4}{x} + \frac{1}{2} \frac{(\log x)^3}{x} + o \left( \frac{(\log x)^3}{x} \right).
$$

### 5. 変数係数による漸近展開

主部分の概念と漸近展開の概念は、次のように一般化できます。 $\mathscr{E}$ を、実数 (または複素数) 写像で形成された比較スケールとし、それぞれについて、$\mathfrak{F}$ に集合があり、その上で写像 * がどの点* でも消えないようにします。さらに、$C$を次の3つの条件$\mathscr{H}(\mathfrak{F}, V)$満たすの写像の集合とします。

(CO₁) 写像 $a \in C$ ごとに 1 つが $a \preccurlyeq 1$ になります。
(CO₂) 写像 $a \in C$ の関係 $a \ll 1$ は $a = 0$ を意味します。
(CO₃) $C$ は $\mathbf{R}$ (それぞれ $\mathbf{C}$) よりベクトル空間です。

ここで、$f$ を $\mathscr{H}(\mathfrak{F}, V)$ の任意の写像とします。 $f - ag \ll g$ となるような写像 $g \in \mathscr{E}$ と非零写像 $a \in C$ が存在する場合、$ag$ は、比較スケール $\mathscr{E}$ および定義域に対して、$f$ の主部分であると言うでしょう。 係数 $C$。このようなプリンシパル部分が存在する場合、それは一意です。たとえば、2 つのプリンシパル部分 $a_1 g_1$ と $a_2 g_2$ があるとします。 1 つのできないは $g_1 \ll g_2$ です。(CO₁) から $a_1 g_1 \ll g_2$ と $f - a_1 g_1 \ll g_1 \ll g_2$ が推測できるため、$f \ll g_2$ です。しかし、$a_2 g_2 \ll g_2$ もあり、その結果、$a_2 \ll 1$ は仮定 $a_2 \neq 0$ と (CO₂) と矛盾します。従って、$g_1 = g_2$ が必要です。 関係 $f - a_1 g_1 \ll g_1, f - a_2 g_1 \ll g_1$ から、(CO₂) と (CO₃) により、$(a_2 - a_1)g_1 \ll g_1$ よって $a_2 - a_1 \ll 1$、そして結果として $a_2 = a_1$ が導き出されます。

#### 例 {#fvr-v-s2-n5-exa-1 .statement tag=08F3}

$x$ の実質は $+\infty$ になる傾向があり、同じ周期 $\tau$、満たす条件 (CO₁)、(CO₂) および (CO₃) を持つ周期写像が $\mathbf{R}$ に限定されます: $\lim_{x \to +\infty} a(x) = 0$ の場合、すべての$\varepsilon > 0$ には、$x \geq x_0$ ごとに $|a(x)| \leq \varepsilon$ となる $x_0$ があります。 $x + n\tau \geq x_0$ と $a(x) = a(x + n\tau)$ のような整数 $n$ が存在するので、$0 \leq x \leq \tau$ についても $|a(x)| \leq \varepsilon$ であると推測します。 $\varepsilon$ は任意であるため、$[0, \tau]$ には $a(x) = 0$ があり、したがってどこにでもあります。

V、p. 222 の記法では、$a_\lambda$ 属するから $C$ と、そのうちの有限の数を除くすべてが零である $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ は、 $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$の場合、$C$の係数を含む$f$、精度$g_\alpha$。 $a_\mu \neq 0$ となるようなすべての添字 $\mu$ について、$\mathscr{E}$ および $C'$ に対して、$a_\mu g_\mu$ が $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$ の主部分となり、$f$ の漸近展開の一意性が証明されます。 (精度 $g_\alpha$) 存在する場合。

$f_1 + f_2$ または $[f_1 . f_2]$ の漸近展開を形成するための n 3 (V、p. 223) で指定された方法は、$f_1$ および $f_2$ の漸近展開から開始して、$[a_\lambda . b_\mu]$ が係数の領域に属している限り、可変係数による展開に再度適用できます。 $C$ は正規空間 $V$ に対応するか、$C$ の係数による漸近展開を認めます。
