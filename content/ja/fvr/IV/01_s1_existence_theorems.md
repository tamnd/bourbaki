---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 1
section_title: EXISTENCE THEOREMS
lang: ja
source: fvr-i-vii
book_pages: 163-177, 199-204
pdf_pages: 0178-0192, 0214-0219
extraction: ocr
subsections:
    - "no": 1
      title: THE CONCEPT OF A DIFFERENTIAL EQUATION
      page: 163
      pdf_page: 178
    - "no": 2
      title: DIFFERENTIAL EQUATIONS ADMITTING SOLUTIONS THAT ARE PRIMITIVES OF REGULATED FUNCTIONS
      page: 164
      pdf_page: 179
    - "no": 3
      title: EXISTENCE OF APPROXIMATE SOLUTIONS
      page: 166
      pdf_page: 181
    - "no": 4
      title: COMPARISON OF APPROXIMATE SOLUTIONS
      page: 168
      pdf_page: 183
    - "no": 5
      title: EXISTENCE AND UNIQUENESS OF SOLUTIONS OF LIPSCHITZ AND LOCALLY LIPSCHITZ EQUATIONS
      page: 171
      pdf_page: 186
    - "no": 6
      title: CONTINUITY OF INTEGRALS AS FUNCTIONS OF A PARAMETER
      page: 174
      pdf_page: 189
    - "no": 7
      title: DEPENDENCE ON INITIAL CONDITIONS
      page: 176
      pdf_page: 191
statements: 29
exercises: 18
content_sha256: b1ea4e41e4e923faf6f26b1ac29345edc521df09993928aa38e7f94eebddb8a1
translated_from: content/en/fvr/IV/01_s1_existence_theorems.md
translation_method: google
source_content_sha256: 0e1758ad98dd52ed21cb9dc147ffdbd0f25ec001d00ee20b8f91629799eb1263
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 61d04e0863df982f7b3f494af8ec46145d6db847f3febc4bdc92d712d70b5640
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。存在定理

### 1. 微分方程式の概念

I を 1 つの点に還元せず、$\mathbf{R}$ に含まれる区間とし、E を $\mathbf{R}$ 上の *位相幾何学的ベクトル空間* とし、A と B の 2 つが E の部分集合を開くとします。 $(x, y, t) \mapsto g(x, y, t)$ を E への $A \times B \times I$ の連続写像とする。 I の A へのすべての*微分可能な* 写像 u の導関数が B の値を取るものに対して、I の写像 $t \mapsto g(u(t), u'(t), t)$ を E に関連付け、それを $\tilde{g}(u)$ で表します。したがって、$\tilde{g}$ は、導関数が B に値を持つ I の B への微分可能関数の集合 $\mathscr{D}(A, B)$ で定義されます。 方程式 $\tilde{g}(u) = 0$ は (*実数* 変数 t に対する) u の *微分方程式* であると言いましょう。この方程式の *解* は、微分方程式 (区間 I) の *整* とも呼ばれます。それは、A への I の微分可能な写像であり、その導関数は B で値を取り、*すべての* $t \in I$ に対して $g(u(t), u'(t), t) = 0$ となります。 言葉の乱用により、微分方程式 $\tilde{g}(u) = 0$ を形に書きます。

$$
g(x, x', t) = 0,
$$

x 属するから集合 $\mathscr{D}(A, B)$ であることを理解した上で。

たとえば、$I = E = \mathbf{R}$ 関係の場合

$$
x' = 2t, \qquad tx' - 2x = 0, \qquad {x'}^2 - 4x = 0, \qquad x - t^2 = 0
$$

は微分方程式であり、4 つすべてが写像 $x(t) = t^2$ を解として認めます

この章では、原則として、E が $\mathbf{R}$ 上の *完全ノルム空間* であり、微分方程式が特定の形である場合のみを考慮します。

$$
x' = f(t, x)
$$

(「$x'$の明示的な方程式」)、ここで、fはEの値で$I \times H$に定義された写像を表し、HはEの*開いた*空でない部分集合です。さらに、そのような方程式の*解*(または*整*)の概念を少し広げます。方程式 (区間 I): 次のような I の *可算* 部分集合 A が存在する場合、H に値を持ち、I で定義され連続する写像 u は方程式 (I) の解 (または積分) であると言えます。 I 写像における A の補数の点 t ごとに、u は $u'(t) = f(t, u(t))$ となる導関数 $u'(t)$ を認めます。 $u$ が微分可能であり、すべての点 $t \in I$ に対して上記の関係を満たす場合、それは I における方程式 (1) の厳密な解であると言えます。

形 $x' = f(t)$ の微分方程式の特別な場合、$f$ は I の写像を E に変換したもので、解は上記の意味で写像 $f$ (II, p. 51) の原始関数であり、厳密な方程式です。 解は厳密なプリミティブです。

E が完全正規化空間 $E_i$ ($1 \leq i \leq n$) の積であるとき、$x = (x_i)_{1 \leq i \leq n}$ と $f = (f_i)_{1 \leq i \leq n}$ を書くことができます。ここで、$x_i$ は I から $E_i$ への写像であり、$f_i$ は$I \times H$から$E_i$への写像。方程式 (1) は微分方程式の系と等価です
$$
x'_i = f_i(t, x_1, x_2, \ldots, x_n) \qquad (1 \leq i \leq n).
$$
(2)

最も重要なケースは、$E_i$ が $\mathbf{R}$ または $\mathbf{C}$ に等しい場合です。次に、(2) はスカラー微分方程式の系であると言います。

簡約する関係の形の研究を簡約する行うことができます。
$$
x^{(n)} = f(t, x, x', \ldots, x^{(n-1)})
$$
系 (2) のそれに対して、$x$ は I でベクトル写像を $n$ 回微分可能です。 $x_1 = x$ と $2 \leq p \leq n$ の $x_p = x^{(p-1)}$ を置く場合、関係 (3) は系と同等です
$$
\begin{cases}
x'_i = x_{i+1} & (1 \leq i \leq n-1) \\
x'_n = f(t, x_1, x_2, \ldots, x_n).
\end{cases}
$$
(4)

形 (3) の関係は、位数 $n$ の微分方程式と呼ばれます ($x^{(n)}$ について明示的に解決されます)。対照的に、形 (1) の方程式は、最初の位数の微分方程式と呼ばれます。

同様に、形の任意の「微分方程式の系」を簡約する作成できます。
$$
D^{n_i} x_i = f_i(t, x_1, Dx_1, \ldots, D^{n_1} x_1, \ldots, x_p, Dx_p, \ldots, D^{n_p-1} x_p)
$$
形の $(1 \leq i \leq p)$ から系 (2)、ここで、$x_i$ は I 上の写像であり、I で $n_i$ 回微分可能です ($1 \leq i \leq p$ の場合)。

### 2. 規制された写像のプリミティブである解を認める微分方程式

区間 $I \subset \mathbf{R}$ で定義されたベクトル写像 $u$ は、すべてのコンパクト部分集合でステップ写像の均一極限である場合に規制されると言われることを思い出してください (II、p. 54、定義 3)。 I;等価な条件は、I 写像 $u$ のすべての内部点に右と左極限があり、また、I の左端点に右極限があり、左端極限があることです。これら 2 つの点属するから I (II、p. 54、th. 3) のとき、I の右側の終点。 この章では、すべての解が I で規制された写像のプリミティブである微分方程式 (1) に限定します。 この条件は、H への I の連続写像 $u$ ごとに、写像 $f(t, u(t))$ が I で規制される場合、明らかに満たされます。次の補題は、これに十分な条件を与えます。

#### 補題 1 {#fvr-iv-s1-lem-1 .statement tag=08BD}

Let $f$ be a map from $I \times H$ into $E$ such that, on writing $f_x$ (for every $x \in H$) for the map $t \mapsto f(t, x)$ of $I$ into $E$, the following conditions are satisfied: 1° $f_x$ is regulated on $I$ for every $x \in H$; 2° the map $x \mapsto f_x$ of $H$ into the set $\mathscr{F}(I, E)$ of maps from $I$ into $E$ is continuous when one endows $\mathscr{F}(I, E)$ with the topology of compact convergence (Gen. トップ。、X、p. 278）。 これらの条件の下:

1° $I$ $H$ 写像 $t \mapsto f(t, u(t))$ への写像 $u$ が$I$ に規制されます。より正確には、点 $t_0 \in I$ におけるこの写像の右 (それぞれ左) 極限は、点 $t_0$ における写像 $t \mapsto f(t, u(t_0))$ の右 (それぞれ左) 極限に等しい。

2° $(u_n)$ が $I$ の写像から $H$ への数列で、$I$ のすべてのコンパクト部分集合で $I$ から $H$ への連続写像 $u$ に一様に収束する場合、次に、写像 $t \mapsto f(t, u_n(t))$ の数列は、$I$ のすべてのコンパクト部分集合で$f(t, u(t))$ に一様に収束します。

1 $c$ を点 $t_0$ における $f(t, u(t_0))$ の右側極限とします。 $\varepsilon > 0$ ごとに、$I$ の $t_0$ のコンパクトな近傍 $V$ があり、$t \in V$ と $t > t_0$ では $\|f(t, u(t_0)) - c\| \leq \varepsilon$ になります。一方、関係となるような$\delta > 0$が存在します。

$$
x \in H, \quad \|x - u(t_0)\| \leq \delta
$$

すべての $s \in V$ に対して $\|f(s, x) - f(s, u(t_0))\| \leq \varepsilon$ を暗示します。 $W \subset V$ が $I$ の $t_0$ の近傍で、$t \in W$ ごとに $\|u(t) - u(t_0)\| \leq \delta$ となり、$t \in W$ と $t > t_0$ には $\|f(t, u(t)) - c\| \leq 2\varepsilon$ となり、$c$ が次の極限であることが証明されます。 $f(t, u(t))$ 点 $t_0$。

2 $K$ を $I$ の圧縮部分集合とします。 $u$ は $I$ で連続であるため、$u(K)$ は $H$ の圧縮部分集合です。 $\varepsilon > 0$ と $x \in u(K)$ ごとに数 $\delta_x$ が存在し、$y \in H, \|y - x\| \leq \delta_x$ と $t \in K$ ごとに $\|f(t, y) - f(t, x)\| \leq \varepsilon$ が存在します。 点 $x_i \in u(K)$ の有限数があり、中心 $x_i$ と半径 $\frac{1}{2}\delta_{x_i}$ 形の閉じたボールは $u(K)$ をカバーします。 $\delta = \operatorname{Min}(\delta_{x_i})$ にしましょう。 仮定までに整数 $n_0$ が存在し、$n \geq n_0$ では $t \in K$ ごとに $\|u_n(t) - u(t)\| \leq \frac{1}{2}\delta$ が存在します。さて、すべての $t \in K$ に対して、次のような添字 $i$ が存在します。

$$
\|u(t) - x_i\| \leq \frac{1}{2}\delta_{x_i};
$$

従って、すべての $t \in K$ およびすべての $n \geq n_0$ に対して $\|u_n(t) - x_i\| \leq \delta_x$、よって $\|f(t, u_n(t)) - f(t, u(t))\| \leq 2\varepsilon$ が得られます。

この残りの切断 I は、$\mathbf{R}$ に含まれる区間を表し、単一の点、$H$ は、標準の空間 $E$、$f$ に含まれるオープン空でない集合を表します。 $I \times H$ から $E$ 満たすへの写像補題の仮説 1.

#### 命題 1 {#fvr-iv-s1-prop-1 .statement tag=08BE}

$t_0$ を $I$ の点および $H$ の $x_0$ 点とします。連続写像 $u$ が$I$ で式 (1) の解となり、点 $t_0$ で値 $x_0$ がとられる場合、関係を満たすことが必要かつ十分です。

$$
u(t) = x_0 + \int_{t_0}^t f(s, u(s))\, ds
$$

$t \in I$ごとに。

実際、補題 1 までに、$u$ が$I$ の (1) の解である場合、$f(t, u(t))$ が規制されるため、(6) の右辺が定義され、$t \in I$ ごとに $u(t)$ に等しくなります。逆に、$u$ が (6) を満たす連続写像である場合、$f(t, u(t))$ は補題 1 によって制御されるため、$u$ は、$I$ の可算部分集合の点を除いて、$f(t, u(t))$ に等しい導関数を持ちます。

#### 系 {#fvr-iv-s1-n2-cor-1 .statement tag=08BF}

*この区間の左 (それぞれ右) 端点とは異なる I のすべての点で、I 上の (1) のすべての解 u は、この点での $f(t, u(t))$ の左 (右) 極限に等しい左 (右) 導関数を許容します。

#### 命題 2 {#fvr-iv-s1-prop-2 .statement tag=08BG}

*f が $I \times H$ から E まで連続する写像である場合、I 上の (1) のすべての解は厳密な解です。*

実際、そのような解 $u$ は、連続写像 $f(t, u(t))$ (II, p. 66、提案 3) のプリミティブです。

さらに、$I \times H$ の連続写像 $f$ は、補題 1 の条件を満たすことに注意します (*Gen. Top.*、X、p. 286、cor. 3)。

続編では、選ぶ $t_0 \in I$ と $x_0 \in H$ を任意に計算し、値 $x_0$ を取って、$I$ の (1) の解 (または $I$ の $t_0$ の近傍) が存在するかどうかを調べます。 点 $t_0$ (または、同様に (6) の解)。

### 3. およそ解の存在

数 $\varepsilon > 0$ が与えられると、$I$ の $H$ への連続写像 $u$ は、微分方程式の $\varepsilon$ 以内の *近似解であると言えます。

$$
x' = f(t, x)
$$

$I$ の *可算* 部分集合の補数の点が、条件を満たす導関数を認める場合、写像 $u$

$$
\|u'(t) - f(t, u(t))\| \leq \varepsilon.
$$

$(t_0, x_0)$ を $I \times H$ の点とします。 $f$ は補題 1 (IV, p. 165) の仮説を満たすため、$I$ に $t_0$ のコンパクト近傍 $J$ が存在し、$f(t, x_0)$ は $J$ で制限され、オープンボール $S$ に中心 $x_0$ が $H$ に含まれており、$f(t, x) - f(t, x_0)$ が $J \times S$ で囲まれるようになります。つまり、$f(t, x)$ は $J \times S$ に *境界がある* ということになります。 *この全体を通じて、小節 J は、I の t_0 の近傍であるコンパクト区間を表し、S は、H に含まれる中心 x_0 と半径 r を持つオープンボールになります。f が J × S で制限されるような J と S です。 M は \|f(t, x)\| の上限を表します。 J×S以上*

#### 命題 3 {#fvr-iv-s1-prop-3 .statement tag=08BH}

*左 (または右) 端点 t_0 が J に含まれ、長さが r/(M + ε) より小さいすべてのコンパクト区間には、方程式 (1) の ε 内に近似解が存在し、S に値が含まれ、t_0 で x_0 に等しい*。

$t_0$ が J の右側の端点ではないと仮定し、左側の端点 $t_0$ を使用して区間に対する命題を証明します。 $\mathscr{M}$を(1)の解の集合から$\varepsilon$以内とし、それぞれSで値を取り、$t_0$で$x_0$に等しく、Jに含まれる半開区間$[t_0, b[$で定義します。 (検討中のおおよその解に応じて区間 )。まず、$\mathscr{M}$ が空ではないことを示します。 c が $t_0$ における $f(t, x_0)$ の正しい極限であるとします。 by 補題 1 (IV, p. 165) 写像 $f(t, x_0 + c(t - t_0))$ は、$t_0$ で c に等しい権利極限を持っているため、写像 $x_0 + c(t - t_0)$ の制限は十分に小さい半分が開いています区間 $[t_0, b[$ は属するから $\mathscr{M}$ になります。

関係 「u は v の制限である」によって位数集合 $\mathscr{M}$ を計算し、$\mathscr{M}$ が帰納的であることを示します (集合理論, III, p. 154)。 $(u_\alpha)$ を、$\mathscr{M}$ と $[t_0, b_\alpha[$ 区間の完全に順序付けられた部分集合とします。ここで、$u_\alpha$ は定義されています。$b_\alpha \leq b_\beta$ 写像の場合、$u_\beta$ は、$u_\alpha$ の拡大になります。 区間 $[t_0, b_\alpha[$ の和集合は J に含まれる区間 $[t_0, b[$ であり、$[t_0, b[$ で定義された写像 u はそれぞれ $[t_0, b_\alpha[$ で $u_\alpha$ を持つ一致するが 1 つだけ存在します。 $\alpha$; $b_\alpha$ の中には、増加する数列 $(b_{\alpha_n})$ があり、b の傾向があります。あなたは、$[t_0, b_{\alpha_n}[$ 写像で $u_{\alpha_n}$ に同意するので、$[t_0, b[$ の可算部分集合の補数の導関数満たす (7) 点を認めます。また、集合 $(u_\alpha)$ の最高値も同様です$\mathscr{M}$。

ゾーンの補題 (集合理論, III, p. 154, th. 2) によれば、$\mathscr{M}$ は極大元 $u_0$ を認めます。 $[t_0, t_1[$ が $u_0$ が定義されている区間である場合、$t_1$ が J の右側の端点であるか、そうでない場合は $t_1 - t_0 \geq r/(M + \varepsilon)$ であることを示します。私たちは、これらの条件のどちらも成り立たないと仮定して、矛盾によって議論します。まず、点 $t_1$ での連続性によって拡大する $u_0$ ができることを示します。実際、$[t_0, t_1[$ の s と t については、

$$
\|u_0(s) - u_0(t)\| \leq (M + \varepsilon)|s - t|
$$

ちなみに値定理;コーシーの基準は、$u_0$ が点 $t_1$ で左極限 $x_1 \in S$ を認めることを示しています。さて、写像 $f(t, x_1)$ の $t_1$ にある極限を $c_1$ とします。 1 つは $\|c_1\| \leq M$ です。 証明の最初の引数と同じ引数は、左側の端点 $t_1$ を写像 $x_1 + c_1(t - t_1)$ として、拡大する $u_0$ を半開区間にできることを示しており、拡張された写像属するは$\mathscr{M}$、それは不条理です。これは命題を証明します。

f が $J \times S$ 1 つの証明できる支柱上で一様連続であるとき。 Zorn の補題 (IV、p. 199、演習 1a)) を使用せずに 3 を実行します。

#### 命題 4 {#fvr-iv-s1-prop-4 .statement tag=08BI}

*(1)の近似解から$\varepsilon$以内の集合は、同じ区間$K \subset J$で定義され、Sで値を取ると、一様等連続です。

実際、u がこの集合のいずれかの写像で、s と t が K の 2 つの点である場合、平均により値定理

$$
\|u(s) - u(t)\| \leq (M + \varepsilon)|s - t|.
$$

#### 系 (ペアノの定理) {#fvr-iv-s1-n3-cor-1 .statement tag=08BJ}

*E が $\mathbf{R}$ 以上の有限次元である場合、S に値を持ち、$t_0$ で $x_0$ に等しい (1) の解が、J に含まれる左 (または右) 端点 $t_0$ を持つすべてのコンパクト区間 K 上に存在します。 長さ $< r/M$.*

確かに、プロップによって。 3、$n$ が十分に大きくなると、(1) の $1/n$ 以内までのおおよその解 $u_n$ が$K$ で定義され、$S$ の値が$t_0$ の$x_0$ に等しくなります。さらに、$n$ の値あたりから、$u_n(K)$ は、$n$ とは独立して、中心 $x_0$ と半径 $< r$ の *閉じた* ボールに含まれます。 $u_n$ の集合は等連続であり (提案 4)、$E$ は有限次元であるため集合 $S$ は $E$ 内で比較的コンパクトです。したがって、$t \in K$ 集合の $u_n(t)$ は、$E$ では比較的コンパクトになります。 Ascoli の定理 (*Gen. Top.*、X、p. 290、th. 2) によると、$u_n$ の集合は、$K$ から写像の空間 $\mathscr{F}(K; E)$ に比べて比較的コンパクトです。 $E$にはノルムのユニフォームが与えられました。したがって、$(u_n)$の$(u_{n_k})$から抽出された数列があり、これは$K$で連続写像$u$に一様に収束します。 1 つは $u(K) \subset S$ なので、$t \mapsto f(t, u(t))$ は $K$ に定義されます。 補題 1 (IV, p. 165) により、$f(t, u_{n_k}(t))$ は$K$ で$f(t, u(t))$ に一様に収束します。 (IV, p. 4, 公式 (7)) により、$u_{n_k}$ は $K$ で一様に $f(t, u(t))$ になる傾向がある写像のプリミティブであるため、(II, p. 52, th. 1) $u$は$K$の(1)の解であり、点$t_0$の$x_0$に等しい。

#### 注意 1 {#fvr-iv-s1-n3-rem-1 .statement tag=08BK}

与えられた点において同じ値を取る微分方程式 (1) の積分は *無限に多く* 存在する可能性があります。たとえば、スカラー微分方程式 $x' = 2\sqrt{|x|}$ には、すべての写像が次のように定義されます。

$$
\begin{array}{ll}
u(t) = 0 & \text{for } -\beta \leq t \leq \alpha \\
u(t) = -(t + \beta)^2 & \text{for } t \leq -\beta \\
u(t) = (t - \alpha)^2 & \text{for } t \geq \alpha
\end{array}
$$

任意の正の数 $\alpha$ および $\beta$ に対して、点 $t = 0$ で値 0 を取る積分として。

#### 注意 2 {#fvr-iv-s1-n3-rem-2 .statement tag=08BL}

ペアノの定理は、$E$ が *無限* 次元の任意の完全ノルム空間 (IV、p. 204、演習 18) である場合、もはや成り立ちません。

### 4. おおよその解の比較

以下では、I と $H$ は、上記のように、それぞれ $\mathbf{R}$ に含まれる区間と、正規化された空間 $E$ の開いた集合を示します。 $t_0$ は I の点です。

#### 定義 1 {#fvr-iv-s1-def-1 .statement tag=08BM}

*正の実数写像* $t \mapsto k(t)$ *定義されている* $I$ とすると、 *ある人は写像* $f$ *から* $I \times H$ *into* $E$ *は写像* $k(t)$ *if、for each* に関してリプシッツであると言う$x \in H$、*写像* $t \mapsto f(t, x)$ *は$I$に規制されており、*すべて* $t \in I$ *および点* $x_1, x_2$ *の* $H$のすべての対について、*1つが（「リプシッツ」 条件")*

$$
\| f(t, x_1) - f(t, x_2) \| \leq k(t) \| x_1 - x_2 \|.
$$

(8)

ある *定数* $k \geq 0$ に対して、この集合上のリプシッツである場合、$f$ は $I \times H$ 上の *リプシッツ* (詳しくは述べませんが) であると言えます。 $I \times H$ のリプシッツ写像が IV、p. 165 の補題 1 (逆は偽) の仮説を満たすのは明らかです。 $f$ がリプシッツ ($I \times H$ 上) のとき、微分方程式は次のようになります。

$$
x' = f(t, x)
$$

(1)

*リプシッツ* ($I \times H$)です。

#### 例 {#fvr-iv-s1-n4-exa-1 .statement tag=08BN}

$E = \mathbf{R}$ と $H$ が $\mathbf{R}$ の区間であるとき、 写像 $f(t, x)$ が点 $(t, x)$ ごとに *偏導関数* $f'_x$ (II, p. 74) を認める場合、 $I \times H$ の場合、$I \times H$ に $|f'_x(t, x)| \leq k(t)$ となると、条件 (8) が満たされ、平均では値定理になります。この例が、$E$ が任意のノルム空間である場合にどのように一般化されるかについては、後で説明します。

$f$ が $I \times H$ 上のリプシッツである場合、$f$ は、すべてのコンパクトな部分区間 $J \subset I$ とすべてのオープンボール $S \subset H$ について、$J \times S$ で *有界* になります。したがって、プロップ。 3 (IV、p. 166) が適用でき、式 (1) の近似解が存在することがわかります。しかし、次の命題もあり、2 つの近似解を *比較* できます。

#### 命題 5 {#fvr-iv-s1-prop-5 .statement tag=08BO}

*$k(t)$ を実際の規制された写像と $I$ の $> 0$ とし、$f(t, x)$ を$I \times H$ の $k(t)$ に関して定義されている写像とします。 $u$ と $v$ が (1) の 2 つの近似解で、それぞれ $\varepsilon_1$ と $\varepsilon_2$ 以内で、$H$ の値を使用して $I$ に定義される場合、すべての $t \in I$ について、次のようになります。 $t \geq t_0$、

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\| \Phi(t) + (\varepsilon_1 + \varepsilon_2)\Psi(t)
$$

どこで

$$
\begin{cases}
\Phi(t) = 1 + \int_{t_0}^t k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds \\
\Psi(t) = t - t_0 + \int_{t_0}^t (s - t_0)k(s) \exp \left( \int_s^t k(\tau) d\tau \right) ds.
\end{cases}
$$

可算数集合の補数で有効な関係 $\|u'(t) - f(t, u(t))\| \leq \varepsilon_1$ から、平均値定理から次のことが推測されます。

$$
\left\| u(t) - u(t_0) - \int_{t_0}^t f(s, u(s))\, ds \right\| \leq \varepsilon_1 (t - t_0)
$$

そして同様に

$$
\left\| v(t) - v(t_0) - \int_{t_0}^t f(s, v(s))\, ds \right\| \leq \varepsilon_2 (t - t_0)
$$

よって

$$
\|u(t) - v(t)\| \leq \|u(t_0) - v(t_0)\|
$$
$$
+ \left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| + (\varepsilon_1 + \varepsilon_2)(t - t_0).
$$

リプシッツ条件による (8) 1 つは

$$
\left\| \int_{t_0}^t (f(s, u(s)) - f(s, v(s)))\, ds \right\| \leq \int_{t_0}^t \|f(s, u(s)) - f(s, v(s))\|\, ds
$$
$$
\leq \int_{t_0}^t k(s) \|u(s) - v(s)\|\, ds
$$

よって、$w(t) = \|u(t) - v(t)\|$を入れて、

$$
w(t) \leq w(t_0) + (\varepsilon_1 + \varepsilon_2)(t - t_0) + \int_{t_0}^t k(s)w(s)\, ds.
$$

したがって、命題は次の補題の帰結です。

#### 補題 2 {#fvr-iv-s1-lem-2 .statement tag=08BP}

*w が区間 [t_0, t_1] 上の連続実数写像で、不等式を満たす場合*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} k(s) w(s) \, ds
$$
(12)

*ここで、$\varphi$ は、$[t_0, t_1]$ で規制されている写像 $\geq 0$ であり、$t_0 \leq t \leq t_1$ については、*

$$
w(t) \leq \varphi(t) + \int_{t_0}^{t} \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds.
$$
(13)

$y(t) = \int_{t_0}^t k(s) w(s) \, ds$を入れてください。 関係 (12) は次のことを意味します。

$$
y'(t) - k(t) y(t) \leq \varphi(t) k(t)
$$
(14)

可算集合の補数。

$z(t) = y(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right)$を入れてください。この場合、(14) は次と同等です

$$
z'(t) \leq \varphi(t) k(t) \exp \left( - \int_{t_0}^t k(s) \, ds \right).
$$

適用で、この不等式に対する平均値定理 (I, p. 15, th.2) を計算し、$z(t_0) = 0$ に注目すると、次のようになります。

$$
z(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( - \int_{t_0}^s k(\tau) \, d\tau \right) \, ds
$$

よって

$$
y(t) \leq \int_{t_0}^t \varphi(s) k(s) \exp \left( \int_s^t k(\tau) \, d\tau \right) \, ds
$$

$w(t) \leq \varphi(t) + y(t)$ なので、(13) が得られます。

#### 系 {#fvr-iv-s1-n4-cor-1 .statement tag=08BQ}

*$\mathbf{f}$ を、$\mathbf{I} \times \mathbf{H}$ で定義された定数 $k > 0$ のリプシッツ写像とします。 $\mathbf{u}$ と $\mathbf{v}$ が、それぞれ $\varepsilon_1$ と $\varepsilon_2$ 以内にある (1) の 2 つの近似解であり、$\mathbf{I}$ で定義され、その値を $\mathbf{H}$ でとると、すべての $t \in \mathbf{I}$ について、*

$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k |t - t_0|} + (\varepsilon_1 + \varepsilon_2) \frac{e^{k |t - t_0|} - 1}{k}.
$$
(15)

この不等式は、実際には $t \geq t_0$ のとき (9) の明らか帰結です。 $t \leq t_0$ について証明するには、それを方程式に適用するだけで十分です

$$
\frac{d \mathbf{x}}{ds} = -\mathbf{f}(-s, \mathbf{x})
$$

(1) から変数 $t = -s$ の変更によって得られます。

#### 注意 1 {#fvr-iv-s1-n4-rem-1 .statement tag=08BR}

$k = 0$ 不等式 (15) を不等式に置き換える場合
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| + (\varepsilon_1 + \varepsilon_2) |t - t_0|
$$
その証明は明らかです。

#### 注意 2 {#fvr-iv-s1-n4-rem-2 .statement tag=08BS}

E が有限次元であり、$\mathbf{f}$ が $I \times H$ 上のリプシッツである場合、選択公理 (IV, p. 199, 演習 1 b)) を使用せずに、(1) の近似解の存在を示すことができます (IV, p. 166, prop. 3)。

#### 命題 6 {#fvr-iv-s1-prop-6 .statement tag=08BT}

*$\mathbf{f}$と$\mathbf{g}$を、$I \times H$、満たすで定義された2つの写像、IV、p. 165の1である補題の仮説、および$I \times H$で、
$$
\| \mathbf{f}(t, \mathbf{x}) - \mathbf{g}(t, \mathbf{x}) \| \leq \alpha.
$$
(16)

さらに、$\mathbf{g}$ が $I \times H$ 上の定数 $k > 0$ に対するリプシッツであると仮定します。このような状況では、$\mathbf{u}$ が $I$ で定義された $H$ の値から $\varepsilon_1$ 以内までのおおよそ $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ の解であり、$\mathbf{v}$ が $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ から解のおおよその解である場合、 $\varepsilon_2$、$I$ に定義され、$H$ に値が含まれ、すべての $t \in I$ に対して
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq \| \mathbf{u}(t_0) - \mathbf{v}(t_0) \| e^{k|t-t_0|} + (\alpha + \varepsilon_1 + \varepsilon_2) \frac{e^{k|t-t_0|} - 1}{k}.
$$
(17)

確かに
$$
\left\| \mathbf{u}'(t) - \mathbf{g}(t, \mathbf{u}(t)) \right\| \leq \alpha + \varepsilon_1
$$
$I$ の可算部分集合の $I$ の補数内のすべての $t$ について。他の語では、$\mathbf{u}$ は $\mathbf{x}' = \mathbf{g}(t, \mathbf{x})$ から $\alpha + \varepsilon_1$ 以内までの近似解であるため、不等式 (17) は適用のプロップに続きます。 IV、p. 169の5。

### 5. リプシッツ方程式と局所リプシッツ方程式の存在と解の一意性

#### 定理 1 (コーシー) {#fvr-iv-s1-thm-1 .statement tag=08BU}

*$\mathbf{f}$ を $I \times H$ 上のリプシッツ写像とし、J を $I$ のコンパクトな部分区間とし、J の単一の点、$t_0$ 点、S に含まれる中心 $\mathbf{x}_0$ と半径 r の開いた球H と M は、$J \times S$ の $\| \mathbf{f}(t, \mathbf{x}) \|$ の中で最も少ない上界です。このような状況では、単一の点に簡約するを持たず、$]t_0 - r/M, t_0 + r/M[$ および含む $t_0$ を含む J の共通部分に含まれるすべてのコンパクト区間 K に対して、K 上で定義された微分方程式 $\mathbf{x}' = \mathbf{f}(t, \mathbf{x})$ の解が 1 つだけ存在します。 S に値があり、点 $t_0$ では $\mathbf{x}_0$ に等しい。

確かに、$\varepsilon > 0$ が十分に小さい場合、(1) の近似解の $\varepsilon$ 以内の集合 $F_\varepsilon$ は、K で定義され、S の値で、点 $t_0$ の $\mathbf{x}_0$ に等しく、空ではありません。 (IV、p. 166、提案 3);さらに、$\mathbf{u}$ と $\mathbf{v}$ 属するから $F_\varepsilon$ の場合、(15) によって (IV. p. 170)
$$
\| \mathbf{u}(t) - \mathbf{v}(t) \| \leq 2\varepsilon \frac{e^{k|t-t_0|} - 1}{k}
$$

すべての $t \in K$ に対して、集合 $F_\varepsilon$ 形 $K$ で連続写像 $w$ に均一に収束するフィルター 基底 $\mathscr{G}$ は、$t_0$ での $x_0$ に等しい。また、$w$ は $S$ に値を取り込みます。なぜなら、$\varepsilon$ が十分小さいため、写像 $u \in F_\varepsilon$ は、$S$ に含まれる閉じたボールに値を取り込むからです。 $f(t, u(t))$は$\mathscr{G}$に沿って$K$から$f(t, w(t))$まで一様に傾向があるので、$w$はIV、p. 165の式(6)を満たし、同様に(1)の解も満たします。 解の一意性は、IVの不等式(15)、p. 170からすぐに続き、$\varepsilon_1 = \varepsilon_2 = 0$と$u(t_0) = v(t_0)$をとります。

$I \times H$ で定義された写像 $f$ は、$I \times H$ の点 $(t, x)$ ごとに、$t$ の近傍 $V$ ($I$ に関して) が存在し、 $f$ が $V \times S$ 上のリプシッツであるような $x$ の近傍 $S$ (定数 $k$ は $V$ と $S$ に応じて)。ボレル・ルベーグ定理によれば、すべてのコンパクト区間 $J \subset I$ およびすべての点 $x_0 \in H$ に対して、$H$ に含まれる中心 $x_0$ を含むオープンボール $S$ が存在し、$f$リプシッツは$J \times S$です。したがって、$f$ は、IV、p. 3 の 1、補題の仮説を満たします。 $f$ が $I \times H$ 上で局所的にリプシッツであるとき、方程式 $x' = f(t, x)$ は $I \times H$ 上で局所的にリプシッツであると言えます。

これを一般化して明確にします。局所的なリプシッツ方程式の IV、p. 10 の 1。 $t_0$ が区間 $I$ の左端点である場合に限定します。 $t_0$ が $I$ の任意の点 (cf. IV, §IV ??, p. 9, 系) である場合に簡単に移行できます。

#### 定理 2 {#fvr-iv-s1-thm-2 .statement tag=08BV}

*$I \subset \mathbf{R}$ を区間 (単一の点に減らさない) とし、左側のエンドポイント $t_0 \in I$ を、$H$ を空でないとし、$E$ で集合を開き、$f$ をローカルのリプシッツ写像とします。 $I \times H$.*

$1^\circ$ *$x_0 \in H$ には、左端点 $t_0 \in J$ を持つ最大の区間 $J \subset I$ が存在します。その上に、$H$ で値を取り、$x_0$ に等しい方程式 $x' = f(t, x)$ の積分 $u$ が存在します。 点 $t_0$;この積分は一意です。*

$2^\circ$ *$J \neq I$ の場合、$J$ は有限長の半開区間 $[t_0, \beta[$ です。さらに、すべてのコンパクト部分集合 $K \subset H$ 集合 $\overline{u}(K)$ は、$\mathbf{R}$ のコンパクト部分集合です。*

$3^\circ$ *$J$ が制限され、$f(t, u(t))$ が $J$ で制限されている場合、$u(t)$ は $J$ の右側の端点に左極限 $c$ を持ちます。さらに、$J \neq I$ の場合、$c$ は $E$ の $H$ の境界点になります。

$1^\circ$ $\mathfrak{M}$ を区間 $L$ の集合 (単一の点に減らない) とし、左側の端点 $t_0 \in L$ は $I$ に含まれており、$L$ には解が存在します。 (1) (IV, p. 163) の $H$ の値と、$t_0$ の $x_0$ に等しい。までに。 1 (IV, p. 171) 集合 $\mathfrak{M}$ は空ではありません。 $L$ と $L'$ を 2 つの区間所属から $\mathfrak{M}$ とし、たとえば $L \subset L'$ と仮定します。 $u$ と $v$ が、$L$ と $L'$ でそれぞれ定義された (1) の 2 つの積分であり、$H$ で値が、$t_0$ での $x_0$ に等しい場合、$v$ は次のようになります。 $u$の拡大。確かに、$t_1$ を $t \in L$ の集合の最高値とし、$t_0 \leq s \leq t$ に対して $u(s) = v(s)$ となるようにします。 $t_1$ が $L$ の右側の終点であることを示します。そうでない場合、連続性により $u(t_1) = v(t_1)$ が得られ、$x_1 = u(t_1)$ は属するから $H$ になります。 $f$ は地元のリプシッツなので、 1 は、$H$ の値で $t_1$ の近傍に定義され、$t_1$ の $x_1$ に等しい (1) の積分が 1 つだけ存在し得ることを示しています。したがって、$t_1$ が $L$ の右側の終点ではないと仮定することは矛盾します。ここで、$J$ が区間 $L \in \mathfrak{M}$ の和集合である場合、(1) の積分 $u$ が 1 つだけ存在し、$J$ で定義され、$H$ の値が$x_0$ に等しいことがわかります。 $t_0$。

2) J ≠ I と仮定し、β を J の右端点とします。 β が I の右側の端点である場合、β ∈ I (したがって β は有限です) となり、J = [t_0, β[ by 仮定] となります。次に、β が I の右側の端点ではないと仮定します。 β ∈ J の場合、u(β) = c 属する to H;までに。 1 区間で定義される、H の値を含む (1) の積分が存在します。

$$ [\beta, \beta_1[ \subset I $$

β で c に等しい。その場合、J は $\mathfrak{M}$ の区間の最大のにはなりませんが、これは不合理です。したがって、J = [t_0, β[。

K が H の圧縮部分集合である場合、$\bar{u}^{-1}(K)$ は J で閉じられます。 $\bar{u}^{-1}(K)$ が [t_0, γ ] に含まれるような γ ∈ J が存在することがわかり、$\bar{u}^{-1}(K)$ がコンパクトであることが証明されます。そうでない場合、(β, c) が t < β かつ u(t) ∈ K となるように、(β, c) が点 (t, u(t)) の集合のクラスター 点となるような点 c ∈ K が存在します。 β ∈ I および c ∈ H であるため、存在します。 I の β の近傍 V、および H に含まれる中心 c および半径 r のオープンボール S。f はリプシッツであり、V × S で有界されます。 M をこの集合に対する $\|f(t, x)\|$ の最高値とする。 仮定までに、$\beta - t_1 < r/2M$、$t_1 \in V$、$\|u(t_1) - c\| \leq r/2$ のような t_1 ∈ J が存在します。番目。 1 は、(1) の積分が 1 つだけ存在し、H に値が存在し、区間 [t_1, t_2] 含む β で定義され、t_1 での u(t_1) に等しいことを示しています。この区間一致すると u が区間 [t_1, β[ であるため、J = [t_0, β[ は $\mathfrak{M}$ では最大の区間ではないということになりますが、これは不合理です。

3 J が有界であり、J 上で $\|f(t, u(t))\| \leq M$ があるとします。次に、J の可算部分集合の補数の $\|u'(t)\| \leq M$。次に、J の任意の s と t について、平均値定理、$\|u(s) - u(t)\| \leq M |s - t|$ となります。コーシー基準によれば、u は J の右端点 β に左極限 c を持ちます。J ≠ I の場合、c できない属するは、β での連続性によって u を拡張すると、u は、区間で定義される H の値との (1) の積分になります。 [t_0, β] であり、t_0 での x_0 に等しい。その場合、 J = [t_0, β] となり、 2 で見たことと矛盾します。

#### 系 1 {#fvr-iv-s1-thm-2-cor-1 .statement tag=08BW}

*H = E かつ J ≠ I の場合、f(t, u(t)) は J で制限されず、さらに E が有限次元である場合、$\|u(t)\|$ は J の右側の端点で極限 $+\infty$ を残します。

最初の部分は 3 番目の部分の明らか帰結です。 2 E が有限次元の場合、すべての閉じた球 S ⊂ E はコンパクトなので、 の 2 番目の部分は小さくなります。図 2 は、t > γ の場合 u(t) ∉ S となるような γ ∈ J が存在することを示しています。

E が有限次元の場合、J ≠ I になる可能性がありますが、t が J の右側の端点に向かう傾向があるため、$\|u(t)\|$ は *有界* のままになります (IV、p. 200、演習 5)。

#### 系 2 {#fvr-iv-s1-thm-2-cor-2 .statement tag=08BX}

*I × H 上で、写像 f が規制された写像 k(t) に関してリプシッツであり、J 属するからI の右側の端点 β である場合、u は β で左側の極限を持ちます。 H = E で、f が I × E で規定された写像 k(t) に関してリプシッツである場合、J = I.*

実際、β ∈ I の場合、I に β のコンパクトな近傍 V が存在し、f(t, x_0) と k(t) は V で制限されます。次に、$V \times H$ で $\|f(t, x)\| \leq m \|x\| + h$ (m と h 定数)、$V \cap J$ の可算部分集合の補数でよって $\|u'(t)\| \leq m \|u(t)\| + h$ となり、$V \cap J$ で $\|u(t)\| \leq m \int_{t_0}^t \|u(s)\|\ ds + q$ ($q$ 定数) になります。 補題 2 (IV, p. 170) は、$V \cap J$ で $\|u(t)\| \leq c\ e^{mt} + d$ ($c$ および $d$ 定数) であるため、$f(t, u(t))$ は $J$ で *有界* のままであり、その結果系が得られることを示しています。 IV、p. 172の2つ。

#### 例 1 {#fvr-iv-s1-n5-exa-1 .statement tag=08BY}

形 $x' = g(t)$ の微分方程式では、$g$ が $I$ で規定され、すべての積分 $u$ はすべての $I$ で明確に定義されます。 $g(t)$ がそうでなくても、$u$ は $I$ で制限される可能性があることに注意する必要があります。

#### 例 2 {#fvr-iv-s1-n5-exa-2 .statement tag=08BZ}

スカラー方程式 $x' = \sqrt{1 - x^2}$ の場合、 $I = \mathbf{R},\ H = ] - 1, +1[$ が得られます。 $t_0 = x_0 = 0$ 対応するを取ると、積分は最大の区間含む 0 で $\sin t$ になります。ここで、$\sin t$ の導関数は正です*、つまり $] - \pi/2, +\pi/2[$ です。この区間の終点では、積分は $H$ の終点に向かう傾向があります。

#### 例 3 {#fvr-iv-s1-n5-exa-3 .statement tag=08C0}

スカラー方程式 $x' = 1 + x^2$ の場合、$I = H = \mathbf{R}$ があります。$t = 0$ で消える積分は $\tan t$ で、最大の区間含む 0 で、この写像が連続である場合は $J = ] - \pi/2, +\pi/2[$ です。そして、$|\tan t|$ は、$J$ のエンドポイントで $+\infty$ になる傾向があります (*cf.* IV、p. 173、cor. 1)。

#### 例 4 {#fvr-iv-s1-n5-exa-4 .statement tag=08C1}

スカラー方程式 $x' = \sin tx$ の場合、$I = H = \mathbf{R}$ があり、右辺は $I \times H$ で制限されているため、(IV, p. 173, cor. 1) すべての積分は $\mathbf{R}$ のすべてで定義されます。

### 6. パラメータの写像としての積分の連続性

提案 6 (IV, p. 171) は、微分方程式が次の場合に次のことを示しています。

$$
x' = f(t, x)
$$

はリプシッツ方程式 $x' = g(t, x)$ に「近く」、*両方の* 方程式が同じ区間上で近似解を持つと仮定すると、これらの近似解は「近い」ことになります。 区間上のリプシッツ方程式 $x' = g(t, x)$ の解の存在は、同じ区間上で $x' = f(t, x)$ の近似解が存在することを *暗示します * が、後者について、 解の値 $x' = g(t, x)$ は、$H$ の *境界* に「近すぎ」ません。

#### 命題 7 {#fvr-iv-s1-prop-7 .statement tag=08C2}

*$f$と$g$を、$I \times H$、満たすIVの補題1の仮説で定義された2つの写像とします。 p. 165 など、$I \times H$*

$$
\|f(t, x) - g(t, x)\| \leq \alpha .
$$
(16)

*さらに、$g$ が $I \times H$ 上の定数 $k > 0$ に関してリプシッツであり、 $f$ が $I \times H$ 上で局所的にリプシッツであるか、あるいは $E$ が有限次元であると仮定します。 $(t_0, x_0)$ を $I \times H$、$\mu$ 数 $> 0$ の点とし、*

$$
\varphi(t) = \mu\ e^{k(t-t_0)} + \alpha\ \frac{e^{k(t-t_0)} - 1}{k} .
$$

*$u$ を、$I$ に含まれる区間 $K = [t_0, b[$ で定義された方程式$x' = g(t, x)$ の積分とし、点 $t_0$ における$x_0$ に等しく、すべての$t \in K$ に対して中心で閉じたボールとなるようにします。 $u(t)$ と半径 $\varphi(t)$ は $H$ に含まれます。これらの条件では、$\|y - x_0\| \leq \mu$ のようなすべての $y \in H$ に対して、$K$ に定義され、$H$ では値が定義され、点では$y$ に等しい$x' = f(t, x)$ の積分$v$ が存在します。 $t_0$;さらに、$K$には$\|u(t) - v(t)\| \leq \varphi(t)$。*

$\mathscr{M}$ を、$H$ で値を取り、$t_0$ で$y$ に等しく、$I$ に含まれる半開区間 $[t_0, \tau[$ で定義される$x' = f(t, x)$ の積分群とします。 区間検討中）。までに。 IV、p. 171 ($f$ が局所的にリプシッツの場合) または IV、p. 167 系 ($E$ が有限次元の場合)、$\mathscr{M}$ は空ではなく、同じ推論小道具。 IV、p. 166の3は、$\mathscr{M}$が位数に対して*帰納的*であることを示しています。「vはwの制限」です。 $v_0$を$\mathscr{M}$の極大元、および$v_0$の定義の区間を$[t_0, t_1[$とします。プロップによって。 IV、p. 171の6、すべては$t_1 \geq b$の証明に帰着します。そうでない場合は、

$$
\| u(t) - v_0(t) \| \leq \varphi(t)
$$

区間 $[t_0, t_1[$ にてプロップにより。 6;現在、コンパクト区間 $[t_0, t_1]$ では、規制されている写像 $g(t, u(t))$ が制限されているため、写像 $g(t, v_0(t))$ は区間 $[t_0, t_1[$ で制限されており、この区間では $\| g(t, v_0(t)) \| \leq \| g(t, u(t)) \| + k \varphi(t)$ が制限されています。 $v_0$ は $[t_0, t_1[$ の $\alpha$ 以内までの $x' = g(t, x)$ の近似解であるため、可算数の点を除いて、この区間上に $\| v_0'(t) \| \leq M$ となるような数 $M > 0$ が存在します。 集合;平均値定理は、$[t_0, t_1[$ の点 $s, t$ のすべての対に対して $\| v_0(s) - v_0(t) \| \leq M |s - t|$ であることを示しています。したがって、(コーシーの基準による) $v_0(t)$ は、次の時点で左極限 $c$ になります。 点 $t_1$、そして連続性により、$\| c - u(t_1) \| \leq \varphi(t_1)$ があり、したがって $c \in H$ になります。さて、IV、p. 171から、th。 1 または IV、p. 167、系、区間 $[t_1, t_2[$ で定義された $x' = f(t, x)$ の積分が存在し、$t_1$ での $c$ に等しい、つまり矛盾する定義 $v_0$。

#### 定理 3 {#fvr-iv-s1-thm-3 .statement tag=08C3}

*F をトポロジカル空間とし、f を I × H × F から E への写像とする。その結果、すべての $\xi \in F$ に対して、写像 $(t, x) \mapsto f(t, x, \xi)$ は I × H 上のリプシッツとなり、$\xi$ が$\xi_0$、$f(t, x, \xi)$ は、I × H で$f(t, x, \xi_0)$ になる傾向があります。$u_0(t)$ は、I に含まれる区間 $J = [t_0, b[$ で定義された$x' = f(t, x, \xi_0)$ の積分であり、H に値が含まれており、次と等しいものとします。 $x_0$、$t_0$。 J に含まれるすべての圧縮区間 $[t_0, t_1]$ に対して、F には $\xi_0$ の近傍 V が存在し、すべての $\xi \in V$ について、方程式 $x' = f(t, x, \xi)$ は $[t_0, t_1]$ で定義された積分 (そして 1 つだけ) $u(t, \xi)$ を持ちます。 H では値、$t_0$ では $x_0$ に等しい。さらに、$\xi$ が $\xi_0$ 解 $u(t, \xi)$ になると、$[t_0, t_1]$ には一律に $u_0(t)$ になる傾向があります。*

実際、$r > 0$ を、$t_0 \leq t \leq t_1$ に対して、中心 $u_0(t)$ と半径 $r$ の閉じた球が $H$ に含まれるようなものとします。 $I \times H$ 上の定数 $k > 0$ に関して $f(t, x, \xi)$ がリプシッツである場合、$\alpha \frac{e^{k(t_1-t_0)} - 1}{k} < r$ となるほど十分に小さい $\alpha$ を採用します。 $\xi \in V$ ごとに $I \times H$ に $\| f(t, x, \xi) - f(t, x, \xi_0) \| \leq \alpha$ が存在するように $V$ を取ると、prop を適用できます。 IV、p. 174の7;さらに、

$$
\| u(t, \xi) - u_0(t) \| \leq \alpha \frac{e^{k(t_1-t_0)} - 1}{k}
$$

$[t_0, t_1]$ で、定理の証明が完了します。

#### 注意 {#fvr-iv-s1-n6-rem-1 .statement tag=08C4}

IV、p. 174 の$H = E$ と条件 (16) が $I \times E$ で満たされるとき、prop。 IV の 7、p. 174 は、この解が定義されている *すべての* 区間上の $x' = g(t, x)$ の *すべての* 解 $u$ に適用されます。 $g(t, x)$ は、必ずしもこの区間に限定されない、規制された写像 $k(t)$ けれどもに関してリプシッツであると考える人もいるかもしれません。

### 7. 最初の条件への依存

$x' = f(t, x)$ を $I \times H$ 上の局所的なリプシッツ方程式とする。までに。 2 (IV、p. 172)、$I \times H$ のすべての点 $(t_0, x_0)$ に対して、*最大の区間* $J(t_0, x_0) \subset I$ が存在し、単一の点、含む $t_0$ などには減りません。この方程式の積分 (そして 1 つだけ) が存在し、$t_0$ における $x_0$ に等しい。この積分と、それが定義されている区間 $J(t_0, x_0)$ が点 $(t_0, x_0)$ にどのように依存するかを明らかにします。

#### 定理 4 {#fvr-iv-s1-thm-4 .statement tag=08C5}

*$f$を、$I \times H$と$(a, b)$、$I \times H$の任意の点上の局所的なリプシッツ関数とします。

1 *区間 $K \subset I$、$I$ の $a$ の近傍、$H$ の $b$ の近傍 $V$ が存在し、$K \times V$ のすべての点 $(t_0, x_0)$ に対して、上で定義された積分 (そして 1 つだけ) $u(t, t_0, x_0)$ が存在します。 $K$、$H$ の値が$t_0$ の点で$x_0$ に等しい (つまり、すべての $(t_0, x_0) \in K \times V$ に対して $J(t_0, x_0) \supset K$)。*

2 *$K \times K \times V$ から $H$ への写像 $(t, t_0, x_0) \mapsto u(t, t_0, x_0)$ は一様連続です。*

3 *There exists a neighbourhood $W \subset V$ of $b$ in $H$ such that, for every point*
$$
(t, t_0, x_0) \in K \times K \times W,
$$
*the equation $x_0 = u(t_0, t, x)$ has a unique solution $x$ on $V$ equal to $u(t, t_0, x_0)$* ("resolution of the integral with respect to the constant of integration").

1 $S$ を、$H$ に含まれる中心 $b$ と半径 $r$ 、$I$ の$I$、$a$ の近傍に含まれる$J_0$ 区間の球とします。 $f$ は有界であり、リプシッツ (ある定数 $k$ に関して) $J_0 \times S$ にあります。 $M$ は、$J_0 \times S$ における $\|f(t, x)\|$ の最高値を示します。 次に、$I$ に $a$ の (IV, p. 171, th. 1) 区間 $J \subset J_0$、近傍が存在し、$J$ で定義された $x' = f(t, x)$ の積分 $v$ が存在し、値が値に含まれます。 $S$ で、$a$ では $b$ に等しい。 中心 $b$ と半径 $r/2$ を持つオープンボール $V$ と、区間 $]a - l, a + l[$ を持つ $J$ の共通部分 $K$ ($l$ は *十分に小さい*) が必要とされることがわかります。 確かに、プロップ。 IV、p. 174 の 7 (集合 $J_0 \times S$ および $\alpha = 0$ の場合に適用) は、$K$ に *定義された* $x' = f(t, x)$ の積分が存在し、$S$ には値があり、$x_0$ に等しいことが示されています。 点 $t_0 \in K$、ただし、
$$
\|v(t) - b\| + \|v(t_0) - x_0\| e^{k|t-t_0|} < r
$$
$t \in K$ごとに。 さて、平均して値定理は、
$$
\|v(t) - b\| \leq M |t - a| \leq Ml
$$
$t \in K$ ごとに; $\|x_0 - b\| < r/2$ から、次のように $l$ を取るだけで十分であることがわかります。
$$
Ml + (Ml + r/2)e^{2kl} < r
$$
または関係 (18) は、$K \times K \times V$ の $(t, t_0, x_0)$ ごとに満たされます。

2) ちなみに、値定理は

$$
\| \mathbf{u}(t_1, t_0, \mathbf{x}_0) - \mathbf{u}(t_2, t_0, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

(20)

K のすべての $t_0, t_1, t_2$ と V の $\mathbf{x}_0$ です。さて、小道具。 5 (IV, p. 169) は次のことを示します

$$
\| \mathbf{u}(t, t_0, \mathbf{x}_1) - \mathbf{u}(t, t_0, \mathbf{x}_2) \| \leq e^{2kt} \ \| \mathbf{x}_2 - \mathbf{x}_1 \|
$$

(21)

K のすべての $t$ と $t_0$、および V の $\mathbf{x}_1$ と $\mathbf{x}_2$ に対して。最後に、$t_1$ と $t_2$ が K の任意の 2 つの点である場合、

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{u}(t_2, t_2, \mathbf{x}_0) \| \leq M |t_2 - t_1|
$$

ちなみに値定理、つまり

$$
\| \mathbf{u}(t_1, t_2, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t_2 - t_1| ;
$$

$\mathbf{u}(t, t_2, \mathbf{x}_0)$ は点 $t_1$ で値 $\mathbf{u}(t_1, t_2, \mathbf{x}_0)$ を取る積分と同じであるため、prop。 5 (IV, p. 169) は次のことを示します

$$
\| \mathbf{u}(t, t_1, \mathbf{x}_0) - \mathbf{u}(t, t_2, \mathbf{x}_0) \| \leq Me^{2kl} |t_2 - t_1|
$$

(22)

K のすべての $t, t_1, t_2$ と V の $\mathbf{x}_0$ です。従って、3 つの不等式 (20)、(21)、(22) は、$K \times K \times V$ における写像 $(t, t_0, \mathbf{x}_0) \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ の一様連続性を証明します。

3 (20) までに、$\| \mathbf{u}(t, t_0, \mathbf{x}_0) - \mathbf{x}_0 \| \leq M |t - t_0| \leq 2Ml$ が終了します

$$
K \times K \times V.
$$

$l$ が十分小さく取られ、$2Ml < r/4$ になると、$\mathbf{x}_0$ が中心 $\mathbf{b}$ と半径 $r/4$ を持つオープンボール W の任意の点である場合、任意の $t$ に対して$\mathbf{u}(t, t_0, \mathbf{x}_0) \in V$ が得られ、 K の $t_0$。$\mathbf{x} = \mathbf{u}(t, t_0, \mathbf{x}_0)$ の場合、写像 $s \mapsto \mathbf{u}(s, t, \mathbf{x})$ は K 上で定義され、点 $t$ で値 $\mathbf{x}$ を取る (1) の積分、つまり $\mathbf{u}(s, t_0, \mathbf{x}_0)$ に等しくなります。特に

$$
\mathbf{x}_0 = \mathbf{u}(t_0, t_0, \mathbf{x}_0) = \mathbf{u}(t_0, t, \mathbf{x}).
$$

さらに、$y \in V$ が $\mathbf{x}_0 = \mathbf{u}(t_0, t, y)$ である場合、整 $s \mapsto \mathbf{u}(s, t, y)$ は $t_0$ で値 $\mathbf{x}_0$ をとるため、$s \mapsto \mathbf{u}(s, t_0, \mathbf{x}_0)$ と同じになり、その結果、$t$ で値 $\mathbf{x}$ がかかります。 $y = \mathbf{x}$ と結論する証明を示します。

### 練習問題 {#fvr-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
