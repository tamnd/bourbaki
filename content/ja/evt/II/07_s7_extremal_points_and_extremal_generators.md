---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 7
section_title: Extremal points and extremal generators
lang: ja
source: evt-i-v
book_pages: TVS II.54-TVS II.60, TVS II.87-TVS II.95
pdf_pages: 0091-0097, 0124-0132
extraction: ocr
subsections:
    - "no": 1
      title: Extremal points of compact convex sets
      page: 54
      pdf_page: 91
    - "no": 2
      title: Extremal generators of convex cones
      page: 57
      pdf_page: 94
    - "no": 3
      title: Convex cones with compact sole
      page: 59
      pdf_page: 96
statements: 25
exercises: 41
content_sha256: 73a84bae5c9abdb05eec2228074cbe575abb8608b952fa4f782912283971b49b
translated_from: content/en/evt/II/07_s7_extremal_points_and_extremal_generators.md
translation_method: google
source_content_sha256: 34250eb8b3431aeea58b08571a7b95394319981a39c9d593e7466689b9edb3b6
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2a89d20cd5a24d4438a7297cfa91e9cb1975f6958183e8a278d023bba3ecba85
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。極値点および極値生成元

### 1. コンパクト凸集合の極値点

#### 定義 1 {#evt-ii-s7-def-1 .statement tag=07IP}

$A$ をアフィン空間 $E$ の凸集合とします。次に、$A$ と含む $x$ に含まれる開いたセグメントが存在しない場合、点 $x \in A$ は $A$ の極値点であると言います。

他の語、関係、$x = \lambda y + (1 - \lambda)z,\ y \in A,\ z \in A,\ y \neq z$、$0 \leq \lambda \leq 1$ は $\lambda = 0$ または $\lambda = 1$ (したがって $x = y$ または $x = z$) を暗示します。 This implies that $x$ cannot be the barycentre of a set of $n$ points $x_i$ of $A$ carrying positive masses unless $x$ is one of the $x_i$; for this is just the definition when $n = 2$; for arbitrary $n$ argue by induction on $n$, as $x$ is the barycentre of $x_1$ and of the barycentre $y_1$ of the $x_i$ with $2 \leq i \leq n$, therefore $x$ is identical with $x_1$ or $y_1$, and in the second case it is sufficient to apply the induction hypothesis.

$x$ が $A$ の極値点であるということは、$A - \{x\}$ が凸であることも意味します。

#### 例 1 {#evt-ii-s7-n1-exa-1 .statement tag=07IQ}

空間 $\mathbf{R}^n$ では、球 $S_{n-1}$ のすべての点は、閉じた球 $B_n$ の極値点です。 $\sum_i y_i^2 \leq 1,\ \sum_i z_i^2 \leq 1$ と $0 < \lambda < 1$ の場合、関係
$$
\lambda^2 \sum_i y_i^2 + (1 - \lambda)^2 \sum_i z_i^2 + 2\lambda(1 - \lambda) \sum_i y_i z_i = 1 = (\lambda + (1 - \lambda))^2
$$
場合にのみ可能です
$$
\sum_i y_i^2 = \sum_i z_i^2 = \sum_i y_i z_i = 1.
$$
しかし、これは$\sum_i (y_i - z_i)^2 = 0$、したがってすべての$i$に対して$y_i = z_i$を意味し、これは私たちの主張を証明します。

#### 例 2 {#evt-ii-s7-n1-exa-2 .statement tag=07IR}

実数 (I, p. 4) の有界数列の標準空間 $\mathscr{B}(\mathbf{N})$ では、単位元ボールの極値点は点 $x = (\xi_n)$ となり、すべてで$|\xi_n| = 1$ になります。 $n$。 なぜなら、すべての $n$ に対して $|\xi_n| \leq 1$ があり、1 つの添字 $p$ に対して $|\xi_p| < 1$ があったと仮定します。 その後、次のように書くことができます
$$
x = \frac{1 + \xi_p}{2} y + \frac{1 - \xi_p}{2} z
$$
ここで、$y$ (それぞれ $z$) は点であり、その座標はすべて添字が同じ $x$ の座標と等しくなります。ただし、座標が 1 (それぞれ $-1$) に等しい添字 $p$ の場合は除きます。 これは、$\|y\| \leq 1$ と $\|z\| \leq 1$ があるため、$x$ が極値ではないことを示しています。 逆に、すべての $n$ に対して $|\xi_n| = 1$ の場合、$x$ は極値であり、関係の $\xi_n = \lambda \eta_n + (1 - \lambda) \zeta_n$ と $|\eta_n| \leq 1,\ |\zeta_n| \leq 1$ および $0 < \lambda < 1$ は $\xi_n = \eta_n = \zeta_n$ を意味します。

#### 例 3 {#evt-ii-s7-n1-exa-3 .statement tag=07IS}

$u : E \to E'$ をアフィン空間 $E'$ 内のアフィン空間 $E$ のアフィン写像とします。 $C \subset E,\ C' \subset E'$ を 2 凸集合とし、$u(C) \subset C'$ とします。 $x'$ が $C'$ の極値点で、$x$ が $u^{-1}(x') \cap C$ の極値点である場合、def からわかるように、$x$ は $C$ の極値点です。 1.

#### 命題 1 {#evt-ii-s7-prop-1 .statement tag=07IT}

$B$ を $A$ の極値点の集合、ハウスドルフ局所凸空間 $E$ の空でないコンパクト凸集合とし、$f$ を次で定義された凸写像とします。 $A$と上部の半連続。その後、$f$ は、$B$ の (少なくとも) 点の 1 つで、$A$ でその上界に達します。

$\mathscr{F}$ を使用して、*空ではなく閉じた、A の部分集合 X のファミリーを表し、A に含まれ、X と一致するすべての開いたセグメントが必ず X* に存在するようにします。これには次の特性があります。
(i) 属するから $\mathscr{F}$ まで。
(ii) 点 $a \in A$ は、$a$ が A の極値点である場合に限り、$\{a\} \in \mathscr{F}$ となる。
(iii) 家族の空でないすべての共通部分 X、$(X_\alpha)$、集合、$\mathscr{F}$、および属するから $\mathscr{F}$。

定義の直後にプロパティ (i)、(ii)、および (iii) が続きます。

(iv) $X \in \mathscr{F}$ とし、$h$ を A において凸で上半連続である写像とする。次に、制限 $h|X$ が X で上界に達するX の点の集合 Y は、Y 属するから $\mathscr{F}$ になります。

なぜなら、X で上位半連続である$h|X$ は、X の少なくとも 1 つの点でX を超えて上界 $\alpha$ に達します (GT、IV, § 6.2、th. 3)。したがって、Y は空ではなく、閉じています (GT, IV, § 6.2, prop. 1)。一方、$x, y$ を A の 2 つの異なる点とし、$z = \lambda x + (1 - \lambda) y$ を Y の点とし、$0 < \lambda < 1$ とします。 $Y \subset X$ と $X \in \mathscr{F}$ として、$x \in X$ と $y \in X$ があります。一方、$h$ は凸であるため、次のようになります。

$$
h(z) \leq \lambda h(x) + (1 - \lambda) h(y)
$$

しかし、$h(x) \leq \alpha, h(y) \leq \alpha$ と $h(z) = \alpha$ として、必然的に $h(x) = h(y) = \alpha$、つまり $x \in Y$ と $y \in Y$ になります。したがって$Y \in \mathscr{F}$。

これらの特性が確立されたので、M を $x \in A$ の集合とします。ここで、$f$ は A でその上界に達します。 (iv)、$M \in \mathscr{F}$による。一方、(iii) と、$\mathscr{F}$ の集合がコンパクト集合 A ではなく部分集合で閉じているという事実により、$\mathscr{F}$ は位数関係 $\supset$ に対して *帰納的* であることがわかります。までに。 S の 2、III, § 2.4、M 含む部分集合 N、つまり$\mathscr{F}$ の最小元。 N が単一の点で構成され、これで命題の証明が完成することを示します。 E は局所的に凸なハウスドルフ空間であるため、E 上のすべての連続線型形式 $u$ が N で定数であることを示すだけで十分です (II, p. 38, cor. 1)。さて、(iv) から、$u|N$ が N で上界に達する$x \in N$ の集合 $N'$ は、$N'$ 属するから $\mathscr{F}$ となる。 N は $\mathscr{F}$ で最小なので、必然的に $N' = N$ になります。

#### 系 {#evt-ii-s7-n1-cor-1 .statement tag=07IU}

*A をハウスドルフ局所凸空間 E のコンパクト凸集合とします。次に、A の少なくとも 1 つの極値点の含むのすべての閉じたサポート超平面 H とします。

なぜなら、$f(x) = \alpha$ が A の H と $f(x) \leq \alpha$ の方程式である場合、prop を適用するだけで十分です。 1から$f$まで。

#### 定理 1 (クライン・ミルマン) {#evt-ii-s7-thm-1 .statement tag=07IV}

— *ハウスドルフの局所凸空間 E では、すべてのコンパクトな凸集合 A は、その極点の集合の閉じた凸包絡線です。

なぜなら、C を A の極値点の集合の閉じた凸包絡線とします。明らかに$C \subset A$。 $A \subset C$ を確認するには、$u$ が E で連続のアフィン線形写像である場合、および C で $u(x) \geq 0$ である場合、A (II, p. 39, cor. 4) でも $u(x) \geq 0$ であることを証明すれば十分です。しかし、これはプロップから続きます。 1 は $-u$ に適用されます。

#### 命題 2 {#evt-ii-s7-prop-2 .statement tag=07IW}

*x を、ハウスドルフ* 局所凸空間 E のコンパクト凸集合 A の極値点とします。すると、E の x のすべての開いた近傍 V に対して、$x \in F \cap A \subset V \cap A$ (他の語では、オープンハーフスペース含む x、形 A の x の近傍の基本的な系 。

E 含む x のすべての開いた半空間 D について、集合 $A \cap \overline{D}$ は A の x のコンパクトな近傍であり、これらすべての近傍のうち共通部分は正確に点 x です (任意の 2 つの異なる点は閉じた超平面によって厳密に分離できます) (II、p. 38、提案 4)。 プロップにより。 GT の 1、I, § 9.2 は、集合 $A \cap \overline{D}$ 形がフィルター 基底であることを証明するのに十分です。 さて、$L_D = A \cap (E - D)$ と書くと、集合 $L_D$ は凸でコンパクトで、凸の集合 $A - \{x\}$ に含まれます。 $D_1, D_2$ が E 含む x の 2 つの開いた半空間である場合、$L_{D_1} \cup L_{D_2}$ の凸包絡線 B は、$A - \{x\}$ に含まれます。しかし、B はコンパクト集合 (II, p. 14, 提案 15) であるため、x を B から厳密に分離する閉じた超平面 H が存在します (II, p. 38, 提案 4)。H と含む x によって決定される開いた半空間が D である場合、次のようになります。 $L_{D_1} \cup L_{D_2} \subset L_D$、したがって$A \cap \overline{D} \subset (A \cap \overline{D_1}) \cap (A \cap \overline{D_2})$。

#### 系 {#evt-ii-s7-n1-cor-2 .statement tag=07IX}

— ハウスドルフ局所凸空間では、K をコンパクト凸集合 A のコンパクト部分集合とします。すると、次の条件は等価です。

a) A は K の閉じた凸包絡線です。

b) K は、A の共通部分であるすべての集合とそのサポート超平面の 1 つを満たします。

c) A の極値点の K 含む集合。

a) $\Rightarrow$ b)。方程式が $f(x) = \alpha$ である A のサポート超平面 H が存在し、$(H \cap A) \cap K = \varnothing$ が成り立つと仮定します。たとえば、A に $f(x) \geq \alpha$ があるとします。すべての $x \in K$ by 仮定に対して $f(x) - \alpha > 0$ として、K がコンパクトであるため、次のようになります。

$$
\beta = \inf_{x \in K} f(x) > \alpha ,
$$

したがって、K は閉じた半空間 $f(x) \geq \beta$ に含まれます。したがって、K の閉じた凸包絡線 A にも同じことが当てはまり、これは不合理です。

b) $\Rightarrow$ c)。 A の極値点 x が K に対して属するにならないとします。 E には $V \cap A \cap K = \varnothing$ となるような x の近傍 V があります。ただし小道具による。 2 では、V は方程式 $f(z) = \alpha$ を使用して超平面 H によって定義される開いた半空間であると仮定できます。たとえば、$f(x) > \alpha$ の場合、すべての $y \in K$ に対して、$f(y) \leq \alpha$ が得られます。したがって、K は A の共通部分と H に平行なサポート超平面 $f(z) = \gamma > \alpha$ を満たしません (II、p. 37、提案 2)。これは不合理です。

c) $\Rightarrow$ a)。これは明らかなクライン・ミルマン定理の帰結です。

#### 注意 1 {#evt-ii-s7-n1-rem-1 .statement tag=07IY}

たとえベクトル空間 E が有限次元であっても、緻密な凸面集合の極値点の集合は必ずしも閉じているとは限りません (II、p. 89、演習 11)。

#### 注意 2 {#evt-ii-s7-n1-rem-2 .statement tag=07IZ}

K が非完全ハウスドルフ局所凸空間のコンパクト集合であり、K の閉じた凸包絡線である A がコンパクトではない場合、K に対して属するを持たない A の極値点が存在する可能性があります (II、p. 87、演習 2)。

#### 注意 3 {#evt-ii-s7-n1-rem-3 .statement tag=07J0}

無限次元の Banach 空間 E では、中心 0、半径 1 の閉じた球が極値点を持たないことが起こります (II、p. 89、練習問題 14)。

#### 注意 4 {#evt-ii-s7-n1-rem-4 .statement tag=07J1}

A がハウスドルフ局所凸空間のコンパクト凸集合である場合、A の極値点が A のサポート超平面に対して属するにならないことが起こります (II、p. 78、演習 11)。 定理 1 (II, p. 56) の証明は、いずれの場合でも A が、サポート超平面に対する属するである A の極値点の集合の凸閉包絡線であることを示しています。

### 2. 凸円錐の極値生成元

C をベクトル空間 E の頂点 0 を持つ凸円錐とします。明らかに、頂点以外の C の点は極値点になり得ません。 C が尖っていて適切である場合にのみ、頂点は C の極値点になります。

#### 定義 2 {#evt-ii-s7-def-2 .statement tag=07J2}

C をベクトル空間 E の頂点 0 の凸円錐とします。 0 から始まる半線 D ⊂ C は、すべての開いたセグメントが含む 0 ではなく C に含まれ、出会い D が D に含まれる場合、C の極値生成元であると言います。

x ≠ 0 であるすべての x ∈ D について、y ≠ 0、y' ≠ 0 が C の 2 点であり、x = y + y' である場合、必ず y ∈ D および y' ∈ D であると言えることは同じことになります。

#### 注意 1 {#evt-ii-s7-n2-rem-1 .statement tag=07J3}

C を E の尖った固有の凸円錐とし、C が元 ≥ 0 の集合である E 位数構造を考えます (II, p. 12, 提案 13)。 位数で、E の元で、x > 0、属するから C の極値生成元まで、x で囲まれたすべての元 y ≥ 0 が、0 ≤ λ で形 λx であることが必要かつ十分です。 ≤ 1 : 実際、y が x によって上に制限されていると言うことは、x = y + y' ここで、y' ∈ C, よってという結論が続きます。

#### 命題 3 {#evt-ii-s7-prop-3 .statement tag=07J4}

ベクトル空間 E では、C を頂点 0 の凸円錐とし、x₀ ≠ 0 を C の点とし、D を 0 と含む x₀ から始まる C に含まれる半線とします。 H を移行 ～ 0 ではなく、超平面含む x₀ とします。その場合、x₀ が H ∩ C の極値点である場合に限り、D は C の極値生成元になります。

条件は明らかに必要です。逆に、それが満たされているとします。 含む D, 移行から x₀ までではなく、D' ∩ C 含むが x₀ 属するに至る開セグメントであるような線分 D' があるとします。 y ≠ 0 を D' の方向ベクトルとする。仮説は、 |λ| に対して点 (1 + λ)x₀ + μy 属するから C であることを意味します。と |μ|十分に小さい。しかし、D と D' によって決定され、正準位相を運ぶ平面 P では、x₀ は P ∩ C の内部点であり、線分 P ∩ H 含むは H ∩ C に含まれる開セグメントであり、それに x₀ 属するが接続されるということになります。これ矛盾する仮定。

#### 定義 3 {#evt-ii-s7-def-3 .statement tag=07J5}

C をハウスドルフ位相幾何学ベクトル空間 E の凸集合とします。C のコンパクトな凸の空でない集合 A は、C の A の補数 C − A が凸である場合、C のキャップと呼ばれます。

C を E の頂点 0 を持つ尖った凸円錐とし、A を C のキャップとします。 B = C − A と書きます。0 から始まるすべての閉じた半直線 L ⊂ C について、集合 L ∩ A と L ∩ B は、L の補数である凸集合です。 和集合は L であり、L ∩ A はコンパクトです。 L ∩ A は少なくとも 1 つの半線 L に対して空ではないので、0 ∈ A であることが分かります。したがって、L ∩ A は 0 に終端点を持つ閉じた線分です。A が存在する場合、C が適切です。

#### 命題 4 {#evt-ii-s7-prop-4 .statement tag=07J6}

— C を E に頂点 0 を持つ尖った凸円錐、ハウスドルフの局所的に凸な空間とします。

a) A を C の上限とします。 pをAのゲージ(II、p. 20)の制限からCとする。 p(x) ≤ 1 となる x ∈ C の集合は集合 A です。 写像 p は下位半連続であり、次の特性があります。
(i) C の任意の x、y について、p(x + y) = p(x) + p(y) が得られます。
(ii) 任意の x ∈ C および λ ∈ R_+^* について、p(λx) = λp(x) が得られます。
(iii) x ∈ C の場合、関係 p(x) = 0 は x = 0 と同等です。

b) 逆に、p を、a) の条件 (i)、(ii) を満たす、[0, +∞] の値を持つ C で定義された関数とする。 A を x ∈ C の集合とし、p(x) ≤ 1 とします。 すると、A と C − A は凸になります。 A がコンパクトで空でない場合に限り、A はキャップです。

主張 b) は明らかです。 a) に記載されているプロパティは、前のプロパティの注意の帰結です。 4と支柱の。 II、p. 20、小道具の 22 個。 II、p. 20 のうち 23 個 (ただし、以下を除く)

$$
p(x + y) \geq p(x) + p(y).
$$

x ≠ 0 および y ≠ 0 の場合、これを最後に証明すれば十分です。したがって、p(x) > 0、p(y) > 0 となります。μ、λ を、λ < p(x)、μ < p(y) となる 2 つの数 > 0 とし、C における A の補数を B で表します。x ∈ λB, y ∈ μB であるため、x + y ∈ λB + μB となります。 B の凸性により、λB + μB ⊂ (λ + μ)B、よって p(x + y) > λ + μ が得られ、これは上記の不等式を意味します。

#### 系 1 {#evt-ii-s7-prop-4-cor-1 .statement tag=07J7}

— C を E の頂点 0 の尖った凸円錐、ハウスドルフの局所凸面空間とし、p を A のゲージ、キャップ C とします。 A の極値点は点 0 となり、C の極値生成元の点 x となり、p(x) = 1 となります。

0 が A の極値点であることは明らかです。 x を L 上の点、C の極値生成元とし、p(x) = 1 とする。 y, z を A の 2 つの点とし、x = $\frac{1}{2}(y + z)$ とします。 L が極値であるため、y = λx および z = μx が得られます。ここで、λ と μ は数 ≥ 0 で、$\frac{1}{2}(\lambda + \mu) = 1$、$\lambda = \lambda p(x) = p(y) \leq 1$、$\mu = \mu p(x) = p(z) \leq 1$ となり、そこから $\lambda = \mu = 1$ したがって、y = z = x となります。したがって、x は A の極値点です。 逆に、x ≠ 0 を A の極値点とします。 明らかに p(x) = 1 です。 y, y' を、x = y + y' となる 2 つの C の点とし、y, y' が x に比例することを示します。 一般性を失うことなく、数 $\lambda = p(y)$ と $\lambda' = p(y')$ は有限で > 0 であると仮定できます。 次にプロップで$\lambda^{-1}y \in A, {\lambda'}^{-1}y' \in A, \lambda + \lambda' = 1$。 4、(i) および等式 $x = \lambda(\lambda^{-1}y) + \lambda'({\lambda'}^{-1}y')$ は、仮定によって次のことを意味します。

$$
x = \lambda^{-1}y = {\lambda'}^{-1}y'.
$$

#### 系 2 {#evt-ii-s7-prop-4-cor-2 .statement tag=07J8}

— C の各点から C の上限までの属する、また C の極値生成元の和集合の凸状閉包絡線までの属する 。

これは cor の直後に続きます。 1 とクライン・ミルマン定理 (II、p. 55、th. 1)。

\* 例。 — X を、σ コンパクトである局所コンパクト空間とします。 C を、曖昧な位相を持つ $\mathscr{M}_+(X)$ の頂点 0 の閉じた凸円錐とします。 C がその上限の和集合であることを示します。 $(X_n)$ を、和集合が X であるX の、オープンで比較的コンパクトな集合の増加する数列とします。 μ を C の元 $\neq 0$ とします。 $\sum_n \alpha_n \mu(X_n) = 1$となるような$\alpha_n > 0$が存在します。

$v \in C$ の小節ごとに、$p(v) = \sum_n \alpha_n v(X_n) \in [0, +\infty]$ を入力します。 写像 C は、提案の条件 (i) および (ii) を満たします。 4. 曖昧な位相 (INT、IV、第 2 版、§ 1, No. 1、提案 4) については、下位の半連続です。したがって、$p(\gamma) \leq 1$ となる $\gamma \in C$ の集合 A は閉じており、空ではありません。一方で、X のすべてのコンパクト集合は $X_n$ の 1 つに含まれているため、漠然と境界づけられている A も漠然とコンパクトです (INT、III、第 2 版、§ 1, No. 9、提案 15)。したがって、集合 A は C 含む μ の上限となります。 \*

#### 命題 5 {#evt-ii-s7-prop-5 .statement tag=07J9}

C を E の頂点 0 を持つ適切な凸円錐、ハウスドルフ弱空間とします。 C は E の均一な構造に対して完全であり、C には 0 の近傍の数え切れない基本的な系があるとします。このとき、C はそのキャップの和集合であり、その極値生成元の閉じた凸包絡線和集合です。

2 番目の主張は、最初と cor から続きます。上記2。プロップを使用。 $E = \mathbf{R}^l$と$C \subset \mathbf{R}_+^l$の場合のII、p. 52、簡約する、命題の11。すべての $\alpha \in I$ について、E の射影 $pr_\alpha$ を $f_\alpha$ で表します。その場合、$f_\alpha$ は連続した線型形式になります。一方、$(V_n)_{n \in \mathbf{N}}$ を、C の 0 の近傍の数えられる基本的な系とします。 E の位相の定義により、各 $n \in \mathbf{N}$ に対して、I および数 $\varepsilon_n > 0$ の有限部分集合 $J_n$ が存在し、$V_n$ 含む集合 $x \in C$ のうち $W_n$ は、すべての $\alpha \in J_n$ に対して $f_\alpha(x) \leq \varepsilon_n$ になります。 $J = \bigcup_{n \in \mathbf{N}} J_n$を入れます。 $y \neq 0$ を C の点とし、p を写像 $\sum_{\alpha \in J} \lambda_\alpha (f_\alpha|C)$ とします。ここで、$p(y) = 1$ となるように $\lambda_\alpha > 0$ が選択されます。これは可能です。なぜなら、すべての $\alpha \in J$ に対して $f_\alpha(y) = 0$ であれば、すべての $n$ に対して $y \in V_n$ となり、これは $y = 0$ を意味し、これは仮定に反します。ここで、すべての $\alpha \in I$ について、写像 $f_\alpha|C$ は点 0 で連続であるため、$n \in \mathbf{N}$ が存在し、$f_\alpha$ は $W_n$ で境界付けられ、したがって、C は a の線形結合によって上に制限されることに注意してください。 写像 $f_\beta|C$ の有限数、ここで $\beta \in J$。したがって、$x \in C$ の集合の A が $p(x) \leq 1$ となる場合、$f_\alpha$ はすべての $\alpha \in I$ について A で制限されることになります。 C では p が下位半連続であるため、C では A が閉じていて空ではないため、コンパクトであることがわかります。 p が prop の条件 (i) と (ii) を検証することは明らかなので、 II、p. 58 の 4 を見ると、A は C と含む y のキャップであることがわかります。

#### 注意 2 {#evt-ii-s7-n2-rem-2 .statement tag=07JA}

完全性が弱く、極値生成元を持たない適切な凸錐体が存在します (II、p. 92、演習 31)。

### 3. コンベックスコーンとコンパクトソール

#### 命題 6 {#evt-ii-s7-prop-6 .statement tag=07JB}

E を局所的に凸なハウスドルフ空間とし、K を含む 0 ではない E の凸コンパクト集合とします。すると、頂点 0 の最小の尖った円錐 C は、含む $K$ が $E$ の適切な凸円錐となります。局所的にコンパクトで完全な $E$ の部分空間です。また、$E$には、含む 0ではなく、$H$が$C$に含まれる0から始まるすべての半線と一致し、$H \cap C$がコンパクトになるような、閉じた超平面$H$が存在します。さらに、$D$ が、これらのプロパティを持つ閉じた超平面である $H$ によって決定される半空間含む 0 である場合、$C \cap D$ は $C$ の上限であり、$C$ は、$\lambda(C \cap D)$ の和集合です。 $\lambda > 0$。

プロップにより。 II、p. 38 の 4 には、0 を $K$ から厳密に分離する閉じた超平面 $H$ が存在します。さて、$\{0\}$と$K$の和集合の凸包絡線$A$はコンパクト(II、p. 14、提案15)であり、$0 \leq \lambda \leq 1$を含む$\lambda K$の和集合です。 0 と $K$ は厳密に $H$ の反対側にあるため、$x \in K$ ごとに $0 < \lambda < 1$ と $\lambda x \in H$ のような $\lambda$ が存在します。 $C$は$\lambda \geq 1$に対する$\lambda A$の和集合であるため、$H$は$C$に含まれる0を起点とするすべての半線と一致し、$H \cap A = H \cap C$がコンパクトであることがわかります。さらに、$C$ は、$\lambda \geq 0$ に対する $\lambda(H \cap C)$ の和集合でもあります。 $C_n$を$0 \leq \lambda \leq n$の$\lambda(H \cap C)$の和集合とします。明らかに、$C_n$ は $\{0\}$ と $n(H \cap C)$ の和集合の凸包絡線であるため、コンパクトです。また、すべての $x \in E$ について、$E$ と整数 $n$ には、$V \cap C \subset C_n$ となる $x$ の閉じた近傍 $V$ があります。実際、$H$ が方程式 $f(z) = \alpha$ で定義されている場合、$\alpha > 0$ は、$nH$ と含む 0 で決定される閉じた半空間を$V$ にとれば十分です。ここで、$n$ は$n\alpha > f(x)$ よりも大きいです。これは、$C$ が局所的にコンパクト ($x \in C$ を取る) であり、$E$ で閉じていることを示しています。 $K$ は完成 $\hat{E}$ の部分集合であると考えることもできるので、$C$ も $\hat{E}$ で閉じられ、完成です。

ハウスドルフ位相幾何学ベクトル空間 $E$ の円錐 $C$ と閉じた超平面 $H$ が与えられると、$H$ 含むは$C$ と $C$ の頂点 $s$ は次のようになります。 $s$ 含む $H \cap C$ を頂点とする円錐最小のの場合、共通部分 $H \cap C$ を円錐 $C$ の« 底» と呼びます。提案 6 は、ハウスドルフの局所凸面空間 $E$、最小の頂点 0 の円錐、含むにおいて、0 が属するにならないコンパクトな凸面集合 $K$ がコンパクトなソールの円錐であり、すべての凸面がコンパクトなソール$S$を持つコーンは、局所的にコンパクトで完全です。

#### 例 1 {#evt-ii-s7-n3-exa-1 .statement tag=07JC}

$E$、ベクトル空間、有限次元のすべての適切な閉じた凸円錐には、コンパクトなソールがあります。実際、II、p. 52、プロップによって。 11 $E = \mathbf{R}^n$ と $C = \mathbf{R}_+^n$ の場合のみを考慮する必要があります。 $(e_i)_{1 \leq i \leq n}$が$\mathbf{R}^n$の標準基底であれば、$e_i$($1 \leq i \leq n$)の凸包絡であるコンパクト凸集合が$\mathbf{R}_+^n$のコンパクトソールであることが明らかです。

#### 例 2 {#evt-ii-s7-n3-exa-2 .statement tag=07JD}

\* $X$ がコンパクトな空間である場合、曖昧な位相を伴う $X$ の積極的措置のコーン $\mathscr{M}_+(X)$ は、コンパクトなソールを持つコーンです (INT、III、第 2 版、§ 1, No. 9、提案 15 の cor. 3)。 \*

### 練習問題 {#evt-ii-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
