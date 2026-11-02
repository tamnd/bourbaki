---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 1
section_title: Semi-norms
lang: ja
source: evt-i-v
pdf_pages: 0038-0044
extraction: ocr
subsections:
    - "no": 1
      title: Definition of semi-norms
      page: 0
      pdf_page: 38
    - "no": 2
      title: Topologies defined by semi-norms
      page: 2
      pdf_page: 39
    - "no": 3
      title: Semi-norms in quotient spaces and in product spaces
      page: 4
      pdf_page: 41
    - "no": 4
      title: Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms
      page: 5
      pdf_page: 42
statements: 15
exercises: 0
content_sha256: cf7052e3164f3366c6f230115c5a7ac8fb3531338ecf5a31931bfd68d5628dc5
translated_from: content/en/evt/II/01_s1_semi_norms.md
translation_method: google
source_content_sha256: 99701b6427e2fc51eea6f3f407ebff4fb20d627e99dfd31c75d611b17f9e8d84
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: b17c9a06f4d43d865d8b5a0e077d55f6570987d4c3daff518d1108b6b9252d08
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。準規範

この段落全体を通じて、$\mathbf{K}$ は非離散値の除算環を示します。

### 1. 準規範の定義

#### 定義 1 {#evt-ii-s1-def-1 .statement tag=07AP}

E を $\mathbf{K}$ 以上左ベクトル空間とします。 $\mathbf{R}_+ = \{ 0, + \infty \}$ の E の写像 $p$ は、次の公理を満たす場合、E の準ノルムと呼ばれます。
(SN_I) $x \in \mathrm{E}$ と $\lambda \in \mathbf{K}$ の場合、$p(\lambda x) = |\lambda| \, p(x)$。
(SN_II) $x \in \mathrm{E}$ と $y \in \mathrm{E}$ の場合、$p(x + y) \leq p(x) + p(y)$。

$p(x) \leq p(y) + p(x - y)$ と $p(y) \leq p(x) + p(y - x)$ なので、$p(y - x) = p(x - y)$ から、
$$
|p(x) - p(y)| \leq p(x - y) .
$$

#### 例 1 {#evt-ii-s1-n1-exa-1 .statement tag=07AQ}

E のノルムは、関係 $p(x) = 0$ が $x = 0$ (I, p. 3) を意味するような準ノルム $p$ です。

#### 例 2 {#evt-ii-s1-n1-exa-2 .statement tag=07AR}

E 上のすべての線型形式 $f$ に対して、写像 $x \mapsto |f(x)|$ は E 上の準ノルムです。

#### 例 3 {#evt-ii-s1-n1-exa-3 .statement tag=07AS}

$p_i (1 \leq i \leq n)$ が E 上の準ノルムの有限集合である場合、明らかに $p'(x) = \sup_{1 \leq i \leq n} p_i(x)$
と $p''(x) = \sum_{i=1}^n \alpha_i p_i(x)$ ($\alpha_i$ は $\geq 0$) は両方とも E の準規範です。

$\mathbf{R}_+$ の E の写像 $p$ は、(SN$_I$) と次の公理を満たす場合、*超準ノルム* と呼ばれます。

(SN$_{II}'$) *$x \in E$と$y \in E$の場合、$p(x + y) \leq \sup(p(x), p(y))$。

超準標準が準標準であることは明らかです。

K 上の絶対的な値が *ウルトラメトリック* (CA, VI, § 6.2) であると言うことは、それが左ベクトル空間 $K_s$ 上の超準標準であり、同一の零ではないことを意味します。

#### 命題 1 {#evt-ii-s1-prop-1 .statement tag=07AT}

*E を K 上の左トポロジー ベクトル空間とし、p を E 上の準ノルムとします。次の条件は同等です :*
  *a)* *p は E で連続です。*
  *b)* *p は点 0 で連続です。*
  *c)* *p は一様連続です。*
  *d)* *各実数 $\alpha > 0$、集合 W(p, $\alpha$) のうち、$p(x) < \alpha$ の $x \in E$ は E で開いています。*
  *e)* *W(p, $\alpha$) が E の 0 の近傍となる実数 $\alpha > 0$ が存在します。*
  *f)* *すべての実数 $\alpha > 0$、集合 V(p, $\alpha$) について、$p(x) \leq \alpha$ の$x \in E$ は、E の 0 の近傍です。*

実際、c) $\Rightarrow$ a) $\Rightarrow$ b) $\Rightarrow$ d) $\Rightarrow$ e) $\Rightarrow$ f) $\Rightarrow$ c) は (SN$_I$) と不等式 (1) からすぐに続きます。

#### 系 {#evt-ii-s1-n1-cor-1 .statement tag=07AU}

*p が E 上の連続半ノルムで、q が $q \leq p$ のような半ノルムである場合、q は E 内で連続です。*

p が E 上の *超準ノルム* である場合、集合 W(p, $\alpha$) と V(p, $\alpha$) は *開と閉の両方* になります。なぜなら、W(p, $\alpha$) が開いていることがわかりました。一方、z が W(p, $\alpha$) のクラスター 点である場合、$p(y - z) < \alpha$ となるような $y \in W(p, \alpha)$ が存在し、(SN$_{II}'$) から $p(z) < \alpha$ が得られるため、W(p, $\alpha$) は閉じます。また、V(p, $\alpha$) は、p が連続であるため閉じています。さらに、$p(x) \leq \alpha$ と $p(y) \leq \alpha$ の場合、(SN$_{II}'$) により $p(x + y) \leq \alpha$ となり、これは V(p, $\alpha$) がオープンであることを示します。

### 2. 準規範によって定義されたトポロジー

p を K 上のベクトル空間 E の準ノルムとする。すべての $\alpha > 0$ について、V(p, $\alpha$) を、$p(x) \leq \alpha$ となる E の x の部分集合とします。 明らかに、$x \in V(p, \alpha)$ と $\lambda \in K$ が $|\lambda| \leq 1$ である場合、$\lambda x \in V(p, \alpha)$、その他の語 V(p, $\alpha$) は *バランス* です。 さらに、すべての $x_0 \in E$ に対して、$|\mu| \geq p(x_0) \alpha^{-1}$、したがって $\mu^{-1} x_0 \in V(p, \alpha)$、つまり V(p, $\alpha$) が *吸収* となるようなゼロ以外のスカラー $\mu \in K$ が存在します。 最後に、(SN$_{II}$) から $V(p, \alpha/2) + V(p, \alpha/2) \subset V(p, \alpha)$ が得られ、(SN$_I$) から K のすべての非ゼロ スカラー $\lambda$ に対して $\lambda V(p, \alpha) = V(p, |\lambda| \alpha)$ が得られます。 これら注意から、I、p. 7、プロップによって結論するが決まります。 4、つまり、$\alpha$ が数 $> 0$ の集合で変化する場合 (または厳密に正の数の数列でのみ 0 になる傾向がある場合)、集合 V(p, $\alpha$) は、次の基本的な系を構成します。 位相の 0 の近傍は E のベクトル空間構造と互換性があります。この位相は *半ノルム p* によって定義されていると言います。 このような位相を持つベクトル空間 E は *半正規化空間* と呼ばれます。 W(p, $\alpha$) が $p(x) < \alpha$ のような E の x の部分集合である場合、W(p, $\alpha$) は ($\alpha > 0$ または $\alpha$ は零の傾向にある数の厳密に正の数列で変化する) を構成することに注意してください。 $p$ によって定義された位相の 0 の近傍の系。

$\Gamma$ が $E$ 上の準ノルムの集合である場合、準ノルム $p \in \Gamma$ によって定義されたトポロジーの *上界* は、ベクトル空間構造 (I、p. 10、cor. 4) と互換性があります。 この位相の 0 の近傍の基本系は、$p_i \in \Gamma$ と $\alpha_i > 0$ の有限共通部分 $\bigcap_i V(p_i, \alpha_i)$ によって与えられます。 この位相は、*半規範* $\Gamma$の集合によって定義されると言われています。 これは、すべての変換の下で不変であり、半ノルム $p \in \Gamma$ が連続であるものの中で、$E$ 上の *最も粗い* 位相です。

Let $E$ be a topological vector space over $K$: a system of semi-norms on $E$, say $\Gamma$, is called a *fundamental system of semi-norms* if the topology on $E$ is the same as the topology defined by $\Gamma$.

$E$ を $K$ 上のベクトル空間とし、位相を準ノルム $\Gamma$ の集合によって定義します。すべての準ノルム $p$ に対して、$p(x - z) \leq p(x - y) + p(y - z)$ が得られます。これは、写像 $(x, y) \mapsto p(x - y)$ が $E$ (GT, IX, § 1.1) 上の *疑似測定* であることを示しています。 定義から、$p$ が $\Gamma$ で変化するとき、これらの擬似計量の集合定義するトポロジカルベクトル空間 $E$ の均一構造。

#### 注意 {#evt-ii-s1-n2-rem-1 .statement tag=07AV}

— 1) $E$ 上の *有限* 半ノルム $p_i$ ($1 \leq i \leq n$) 集合によって定義される位相は、*単一* 半ノルム $p = \sup_{1 \leq i \leq n} p_i$ によって定義できます。しかし、半ノルムできないの無限の集合によって定義される位相は、一般に、単一の半ノルム (III、p. 37、演習 2) によって定義されます。

2) $(\mathscr{T}_i)_{i \in I}$ を、$K$ 上のベクトル空間 $E$ 上のトポロジーのファミリーとし、それぞれが準ノルム $\Gamma_i$ のファミリーによって定義されます。すると、半ノルム $\Gamma = \bigcup_{i \in I} \Gamma_i$ の集合によって定義される位相は、トポロジー $\mathscr{T}_i$ の上界になります。

3) $\Gamma_0$ が、増加する* 位数関係によって $E$ 上の 2 つの準規範 $p, q$ の間に、« $p \leq \lambda q$ となる$\lambda > 0$ が存在する» によって定義された半規範の集合である場合、基本的な$\Gamma_0$ で定義される位相の 0 の近傍の系は、$p \in \Gamma_0$ と $\alpha > 0$ である集合 $V(p, \alpha)$ を取ることによって取得されます。 $\Gamma$ が $E$ 上の半ノルムのいずれかの集合である場合、$\Gamma$ と同じ位相を定義するフィルタリングされた半ノルムの集合は、半ノルムのすべての有限族の上部エンベロープの集合 $\Gamma_0$ になります。 所属から$\Gamma$まで。

4) たとえ $K$ できない上の位相幾何学ベクトル空間の $K = \mathbf{R}$, 位相が常に半ノルム (*cf.* II, p. 24, 系) の集合によって定義されます。

#### 例 {#evt-ii-s1-n2-exa-1 .statement tag=07AW}

— $\mathscr{C}^\infty(\mathbf{R})$ を、$\mathbf{R}$ で無限微分可能な実数値写像の $\mathbf{R}$ を超えるベクトル空間とします。 整数 $n \geq 0$、$m \geq 1$ のすべての写像とすべての対に対して、

$$
p_{n,m}(f) = \sup_{-m \leq t \leq m} |f^{(n)}(t)|
$$

$f^{(0)} = f$と。明らかに、$p_{n,m}$ は $\mathscr{C}^\infty(\mathbf{R})$ の準標準です。 位数において、写像 $f_\alpha$ が 0 になる傾向があること (添字の集合にフィルタ $\mathfrak{F}$ に従って) 位相 $\mathscr{T}$ の$\mathscr{C}^\infty(\mathbf{R})$ は、準規範 $p_{n,m}$ によって定義されており、必要かつ十分です。すべての整数 $n \geq 0$、写像 $f_\alpha^{(n)}$ は、* $\mathbf{R}$ のすべてのコンパクト部分集合で一律に ($\mathfrak{F}$ に続く) 0 になる傾向があります。 $\mathscr{T}$ は、写像* $f \in \mathscr{C}^\infty(\mathbf{R})$ * およびそのすべての導関数* (*cf.* III、p. 9) のコンパクトな収束の *位相であると言います。

#### 命題 2 {#evt-ii-s1-prop-2 .statement tag=07AX}

*On a vector space* $E$, *let* $\mathscr{T}$ *be the topology defined by a set of semi-norms* $\Gamma$.

(i) *E の {0} の閉包は、$\mathscr{T}$ について、$x \in E$ の部分集合であり、各半ノルム $p \in \Gamma$ に対して $p(x) = 0$ です。*

(ii) *$\mathscr{T}$ がハウスドルフであり、$\Gamma$ が数えられる場合、$\mathscr{T}$ は数えられる*。

命題は、 定義と GT、 IX, § 2 の直後に続きます。 4、コル。 1.

$\mathscr{T}$ が計量可能である場合、$\mathscr{T}$ できないは単一のノルムによって定義される可能性があることに注意してください。これは、上記の例 (*cf.* IV、p. 18、*例 4*) の場合です。

E を K 上のベクトル空間とし、位相を準ノルム $\Gamma$ の集合によって定義します。 Let $\hat{E}$ be the Hausdorff completion of E (I, p. 6), and $\hat{\Gamma}$ be the set of mappings $\hat{p}$ of $\hat{E}$ in $\mathbf{R}_+$ where $p$ varies in $\Gamma$ (GT, II, § 3 . 7, prop. 15). By the principle of extending inequalities, the functions $\hat{p} \in \hat{\Gamma}$ are semi-norms on $\hat{E}$, and the functions $\hat{p}(x - y)$ form a set of pseudometrics defining the uniform structure of $\hat{E}$ (GT, IX, § 1 . 3, prop. 1). したがって、$\hat{\Gamma}$ は、$\hat{E}$ の位相を定義する準規範の基本的な集合であることがわかります。

### 3. 商空間および積空間の準規範

E を K 上のトポロジカルベクトル空間とし、その位相は準ノルムの $\Gamma$、集合によって定義されます。明らかに、E の部分空間 M の$\Gamma$ からベクトルの半規範の制限、定義する位相が E の部分空間によって M に誘発されました。

$\phi$ をベクトル商空間 E/M の E の標準写像とします。 E 上のすべての準ノルム $p$ に対して、写像であることを示します。

$$
\dot{p}(z) = \inf_{\phi(x) = z} p(x)
$$

E/M では準標準です。実際、$\dot{p}$ が条件 (SN$_1$) を満たすことは明らかです。一方、$z', z''$ が E/M の 2 つのベクトルである場合、次のようになります。

$$
\begin{align*}
\inf_{\phi(x) = z' + z''} p(x) &\leq \inf_{\phi(x') = z', \phi(x'') = z''} p(x' + x'') \\
&\leq \inf_{\phi(x') = z', \phi(x'') = z''} (p(x') + p(x'')) \\
&= \inf_{\phi(x') = z'} p(x') + \inf_{\phi(x'') = z''} p(x'')
\end{align*}
$$

これは、$\dot{p}$ が (SN$_2$) を検証することを示しています。 $\dot{p}$ は M による $p$ の *商準正規* であると言います。

同じ推論は、$p$ が *超準標準* である場合、$\dot{p}$ も同様であることを証明します。

そうなると、(No. 2 の記法)

$$
\phi(\mathrm{W}(p, \alpha)) = \mathrm{W}(\dot{p}, \alpha)
$$

$\alpha > 0$ごとに。実際、$\dot{p}(z) < \alpha$ということは、$\phi(x) = z$と$p(x) < \alpha$のような$x \in E$が存在し、そこから関係(4)が続くことを意味します。

このことから、準規範 $\Gamma$ の集合が *指示* (II、p. 3、*注意 3*) である場合、$E/M$ の商位相は準規範の集合によって定義されると推測します。 $p$が$\Gamma$で変化する場合、$\dot{p}$。

$N$ が $E$ の $\{0\}$ の閉包である場合、$E/N$ の位相は商準ノルム $\dot{p}$ によって定義されます。ここで、$p$ は $\Gamma$ で変化します ($\Gamma$ がフィルターされていない場合でも): ここ$x$ 所属から類 $\dot{x} \mod N$ ごとに $\dot{p}(\dot{x}) = p(x)$。 $E/N$ は、$E$ (I、p. 4) に関連付けられたハウスドルフ空間に他ならないことに注意してください。

$E$ を $K$ 上のベクトル空間とし、$(E_i)_{i \in I}$ を $K$ 上のベクトル空間の族とします。ここで、$E_i$ は半規範の集合によって定義される位相 $\mathscr{T}_i$ です。 $\Gamma_i$。それぞれの $i \in I$ について、$f_i$ を $E_i$ の $E$ の線形写像とします。明らかに、$p_i$ が集合 $\Gamma_i$ で変化すると、$E$ の準標準の $p_i \circ f_i$ 形集合 $\Gamma'_i$ が変化します。 $E$ 上の位相 $\mathscr{T}$ は、すべての写像 $f_i$ を連続にするすべてのI、p. 9 の中で最も粗いものとして定義され、準ノルム $\Gamma' = \bigcup_{i \in I} \Gamma'_i$ の集合によって定義されます。これは次のとおりです。 $\mathscr{T}$ の 0 の近傍の定義 (GT、I, § 2.3、提案 4)。

$p_i$ が超準標準であるなら、$p_i \circ f_i$ も同様です。

$E$ を $K$ 上のベクトル空間とし、位相 $\mathscr{T}$ を準規範 $(p_i)_{i \in I}$ の族によって定義します。すべての $i \in I$ について、$\mathscr{T}_i$ を単一の半ノルム $p_i$ によって定義される位相とし、位相 $\mathscr{T}_i$ を使用して $E$ から得られる $E_i$ 空間で表します。このとき、位相 $\mathscr{T}$ は、$\prod_{i \in I} E_i$ 上の積位相の対角写像 $\Delta : E \to \prod_{i \in I} E_i$ により、逆像になります (I、p. 9、提案 7)。それぞれの $i \in I$ について、$E_i$ の $\{0\}$ の終結として $N_i$ を書き込み、$F_i = E_i / N_i$ までに、ノルム $p_i$ 対応するから $p_i$ によって定義される *標準* 空間を書き込みます。 (II、p. 4、公式 (3)); $\phi_i : E_i \to F_i$ が標準写像かつ $\phi : (x_i) \mapsto (\phi_i(x_i))$ 積写像の場合、$\prod_{i \in I} E_i$ の積位相は、積の $\phi$ により逆像であることがわかります。 位相、$\prod_{i \in I} F_i$ (GT、II, § 3.9、prop. 18)。したがって、位相 $\mathscr{T}$ は、$\prod_{i \in I} F_i$ 上の積位相の合成写像 $\phi \circ \Delta$ の下にある逆像です。特に、$\mathscr{T}$ が *Hausdorff* である場合、それは II、p. 3、prop から続きます。 2 写像 $\phi \circ \Delta$ は *単射* であるため、次のようになります。

#### 命題 3 {#evt-ii-s1-prop-3 .statement tag=07AY}

*位相が半ノルムの集合によって定義される、*$K$ 上のすべてのハウスドルフ位相位相ベクトル空間* $E$ は、バナッハ空間* の積の部分空間と同型です。

さらに、$E$ の位相が *数えられる* 集合の半ノルムによって定義される場合、$E$ は *計量可能* (I, p. 16) です。

### 4. 半ノルムによって定義されたトポロジの多重線形写像の等連続性基準

#### 命題 4 {#evt-ii-s1-prop-4 .statement tag=07AZ}

*$E_i$ ($1 \leq i \leq n$) *および* $F$ *トポロジカルベクトル空間以上* $K$ とします。 *すべての* $i$ について、* $E_i$ の *位相は * 半規範* $\Gamma_i$ の有向集合によって定義され、* $F$ の位相 * は半規範* の集合によって定義されると仮定します* $\Gamma$。 *その後、集合* $H$、F の $\prod_{i=1}^n E_i$ の * 多線形写像が等連続であるのは、各半ノルム $q \in \Gamma$ および各添字 i に対して、半ノルム $p_i \in \Gamma_i$ が存在する場合に限ります。 数 $a > 0$、それぞれ写像 $u \in \mathbf{H}$ と点 $(x_i) \in \prod_{i=1}^n E_i$ について、

$$
q(u(x_1, x_2, ..., x_n)) \leq a \cdot p_1(x_1)\ p_2(x_2) ... p_n(x_n) .
$$

条件は、H が (0, 0, ..., 0) で等連続であること、したがってどこでも (I, p. 9, 提案 6) であることを意味するため、十分です。

条件が必要であることがわかります。 仮定までに、すべての準ノルム $q \in \Gamma$ とすべての数 $\beta > 0$ について、写像 $u \in \mathbf{H}$ ごとに $q(u(x_1, x_2, ..., x_n)) \leq \beta$ が得られます。ただし、添字 $i$、$1 \leq i \leq n$、および特定の各$p_i(x_i) \leq \alpha_i$ が真である場合に限ります。適切に選択された数 $\alpha_i > 0$ と準標準 $p_i \in \Gamma_i$ です。 K は非離散であるため、$i$ ごとに、$\lambda_i \in \mathbf{K}$ に対して $\alpha_i = |\lambda_i| < 1$ があると仮定することもできます。次に、$(x_1, x_2, ..., x_n)$ を $\prod_{i=1}^n E_i$ のいずれかの点とし、各添字 $i$ について、$m_i \in \mathbf{Z}$ を $p_i(x_i) \leq |\lambda_i|^{m_i + 1}$ となる整数とします。これは $p_i(\lambda_i^{-m_i} x_i) \leq |\lambda_i|$ ($1 \leq i \leq n$) と書くことができるため、仮定までに次のようになります。

$$
q(u(x_1, x_2, ..., x_n)) \leq \beta |\lambda_1|^{m_1} |\lambda_2|^{m_2} ... |\lambda_n|^{m_n} .
$$

まず、$p_i(x_i)$ の 1 つが零であると仮定します。その後、$m_i \in \mathbf{N}$ を任意に大きくすることができるため、$q(u(x_1, x_2, ..., x_n)) = 0$ となります。逆に、すべての $p_i(x_i)$ が $\neq 0$ である場合は、$i$ ごとに $|\lambda_i|^{m_i + 2} < p_i(x_i) \leq |\lambda_i|^{m_i + 1}$ となるように整数 $m_i$ を取ります。次に、$|\lambda_i|^{m_i} < |\lambda_i|^{-2} p_i(x_i)$ があり、そこから (6) により、関係 (5) が続きます。

$$
a = \beta (|\lambda_1| \cdot |\lambda_2| ... |\lambda_n|)^{-2} .
$$

Q.E.D.

#### 系 {#evt-ii-s1-n4-cor-1 .statement tag=07B0}

— *集合 H が等連続であるのは、すべての半ノルム $q \in \Gamma$ について、$\prod_{i=1}^n E_i$ に 0 の近傍が存在し、その中で写像 $q \circ u$ ($u \in \mathbf{H}$ の場合) が均一に制限されている場合に限ります。*

条件は明らかに必要であり、プロップのデモンストレーション。 4 は、すべての $u \in \mathbf{H}$ に対して形 (5) の不等式を意味し、したがって H の等連続性を示します。

prop の特定のケースを明示的に述べます。 線形写像の場合は 4。

#### 命題 5 {#evt-ii-s1-prop-5 .statement tag=07B1}

— *E、F を非離散値の除算環 K 上の 2 つのトポロジー ベクトル空間とします。 E (それぞれ F) の位相が半ノルム $\Gamma$ (それぞれ $\Gamma'$) の集合によって定義されるとします。 H を F の E の線形写像の集合とします。次の条件は同等です :*
    a) H は等連続です。

b) For every semi-norm $q \in \Gamma'$, there exists a finite family $(p_i)_{1 \leq i \leq n}$ of semi-norms belonging to $\Gamma$ and a number $a > 0$ such that, for all $x \in E$ and all $u \in H$,

$$
q(u(x)) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) .
$$

c) すべての半ノルム $q \in \Gamma'$ について、写像 $\sup_{u \in H} (q \circ u)$ は $E$ 上の連続的な半ノルムです。

#### 系 1 {#evt-ii-s1-prop-5-cor-1 .statement tag=07B2}

— $\mathscr{T}, \mathscr{T}'$ が、$K$ 上のベクトル空間 $E$ 上の 2 つのトポロジーであり、それぞれ、半ノルム $\Gamma$ と $\Gamma'$ の 2 つの集合によって定義されているとします。 $\mathscr{T}$ は、$\mathscr{T}'$ よりもより細かいですが、それは、すべての準規範 $q \in \Gamma'$ に対して、すべての半規範所属から $\Gamma$ および数 $a > 0$ の有限族 $(p_i)_{1 \leq i \leq n}$ が存在する場合に限ります。 $x \in E$、$q(x) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x)$があります。

In fact this shows that the identity mapping of $E$ with topology $\mathscr{T}$, on $E$ with topology $\mathscr{T}'$, is continuous.

#### 系 2 {#evt-ii-s1-prop-5-cor-2 .statement tag=07B3}

— $K$ 上のトポロジカルベクトル空間 $E$ の位相 $\mathscr{T}$ が半ノルム $\Gamma$ の有向集合によって定義されるとします。各準ノルム $p \in \Gamma$ について、$p$ で定義された位相を使用して $E$ から得られた空間を $E_p$ とします。 The set $E'$ of linear forms on $E$ that are continuous for $\mathscr{T}$ is the union of the sets $E'_p$, where $E'_p$ is the set of continuous linear forms in $E_p$ ($p \in \Gamma$).
