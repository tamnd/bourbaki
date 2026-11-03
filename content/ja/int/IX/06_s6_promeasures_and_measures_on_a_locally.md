---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 6
section_title: Promeasures and measures on a locally convex space
lang: ja
source: int-vii-ix
book_pages: INT IX.72-INT IX.101, INT IX.117
pdf_pages: 0254-0283, 0299-0299
extraction: ocr
subsections:
    - "no": 1
      title: Promeasures on a locally convex space
      page: 72
      pdf_page: 254
    - "no": 2
      title: Image of a promeasure
      page: 74
      pdf_page: 256
    - "no": 3
      title: Fourier transform of a promeasure
      page: 75
      pdf_page: 257
    - "no": 4
      title: Calculation of Gaussian integrals
      page: 77
      pdf_page: 259
    - "no": 5
      title: Gaussian promeasures and measures
      page: 78
      pdf_page: 260
    - "no": 6
      title: Examples of Gaussian promeasures
      page: 82
      pdf_page: 264
    - "no": 7
      title: Wiener measure
      page: 85
      pdf_page: 267
    - "no": 8
      title: Continuity of the Fourier transform
      page: 92
      pdf_page: 274
    - "no": 9
      title: Minlos’s lemma
      page: 93
      pdf_page: 275
    - "no": 10
      title: Measures on the dual of a nuclear space
      page: 96
      pdf_page: 278
    - "no": 11
      title: Measures on a Hilbert space
      page: 97
      pdf_page: 279
statements: 33
exercises: 1
content_sha256: f7e904ba4d54d8d46741dd09405e3d09df410827e1cda51f1671746559f5eaaa
translated_from: content/en/int/IX/06_s6_promeasures_and_measures_on_a_locally.md
translation_method: google
source_content_sha256: e617c5fb964b4dfa4c93d927e10519f76530432982d0dd1d298de1585dc144da
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: a9700545f759764dc3bc2fae7f2ffe605e05b02f33224380bdfd47a5e906a164
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。局部凸の対策と対策空間

この切断を通じて、実数のうち体を超えるベクトル空間のみが考慮されます。局所的に凸な空間とは、$\mathbf{R}$ 上のトポロジカルなベクトル空間、つまりハウスドルフで局所的に凸であることを意味します。局所的に凸な空間 E の位相双対は $E'$ で示されます。 $x \in E$ と $x' \in E'$ には、$\langle x, x' \rangle = x'(x)$ と書きます。

### 1. 局所凸面での対策空間

E を局所凸空間とします。 関係 $\supset$ で順序付けされた有限余次元の E の閉じた線形部分空間の $\mathscr{F}(E)$ 集合で表します。 $V \in \mathscr{F}(E)$ ごとに、$p_V$ は E の $E/V$ 上の標準写像を表します。 V と W を $\mathscr{F}(E)$ の 2 つの元とし、$V \supset W$ とします。 $E/W$ の $p_{VW}$ 写像を、E の恒等写像から商を経て推定される $E/V$ と表します。 ファミリ $\mathscr{Q}(E) = (E/V, p_{VW})$ は、局所凸型空間の逆行列系であり、$\mathscr{F}(E)$ によってインデックスが付けられます。 これは、E* の有限次元商の * 逆数系と呼ばれます。

逆行列系 $\mathscr{Q}(E)$ の逆行列極限は、弱い位相 $\sigma(E'{}^*, E')$ を備えた $E'$ の代数双対 $E'{}^*$ と正準的に同型であることが示されます。

#### 定義 1 {#int-ix-s6-def-1 .statement tag=09S6}

*$E$を局所凸空間とする。 $E$ の有限次元商の逆数系上のメジャー (§ 4, No. 2、定義 1) の逆数系$^{(1)}$ ごとに、$E$ で promeasure を呼び出します。

他の語では、$E$ 上のプロメジャー $\mu$ は族 $(\mu_V)_{V \in \mathscr{F}(E)}$ であり、$\mu_V$ は有限次元空間 $E/V$ 上の有界 (正の) メジャーであり、$V \supset W$ のとき $\mu_V = p_{VW}(\mu_W)$ です。すべてのメジャー $\mu_V$ の合計質量は同じであり、これをプロメジャー $\mu$ の *合計質量* と呼びます。

$E$ ～ 属する ～ $\mathscr{F}(E)$ の部分空間 $V$ については、$V$ が $x \in E$ から構成されるような、元 $x'_1, \ldots, x'_n$ の$E'$ の有限数が存在することが必要かつ十分です。 満たす $\langle x, x'_i \rangle = 0$ は $1 \leq i \leq n$ に対して (TVS、II, § 6, No. 3、Th. 1 の Cor. 2 および No. 5、Prop. 7 の Cor. 2)。さらに、有限次元ベクトル空間には、ハウスドルフ トポロジカルベクトル空間位相 (TVS、I, § 2, No. 3、Th. 2) が 1 つだけ存在します。従って、$E$ の対策の概念は、$E$ の双対である $E'$ にのみ依存します。

$\lambda$ を $E$ の有界メジャーとします。 For every $V \in \mathscr{F}(E)$, let us denote by $\widetilde{\lambda}_V$ the image of $\lambda$ under the canonical mapping $p_V$ of $E$ onto $E/V$. 1 つは、$\mathscr{F}(E)$ の 2 つの元 $V$ と $W$ に対して $p_V = p_{VW} \circ p_W$ を持ち、$V \supset W$ になります。従って、家族 $\widetilde{\lambda} = (\widetilde{\lambda}_V)_{V \in \mathscr{F}(E)}$ は $E$ の予定です。 $\widetilde{\lambda}$ は、メジャー $\lambda$ に *関連付けられた* プロメジャーであるとします。 $\lambda$ と $\widetilde{\lambda}$ の合計質量が同じであることがすぐにわかります。

#### 命題 1 {#int-ix-s6-prop-1 .statement tag=09S7}

*$E$を局所的に凸な空間とします。 The mapping $\lambda \mapsto \widetilde{\lambda}$ is a bijection of the set of bounded measures on $E$ onto the set of promeasures $(\mu_V)_{V \in \mathscr{F}(E)}$ on $E$ satisfying the following condition:

すべての $\varepsilon > 0$ に対して、すべての $V \in \mathscr{F}(E)$ に対して $\mu_V(E/V - p_V(K)) \leq \varepsilon$ となるような、$E$ のコンパクトな部分集合 $K$ が存在します。

$E$ 上の連続線型形式の核の共通部分が 0 に等しいことがわかります (TVS、II, § 4, No. 1、提案 2 の Cor. 1)。その結果、$\bigcap_{V \in \mathscr{F}(E)} V = \{0\}$ と家族 $(p_V)_{V \in \mathscr{F}(E)}$ は一貫性を持ち、分離しています。 命題は Th から続きます。 § 4, No. 2 の 1 つ。

特に、写像 $\lambda \mapsto \widetilde{\lambda}$ は単射法です。 $\mu$ が $E$ の予定尺度であり、$E$ に $\mu = \widetilde{\lambda}$ となるような限定された尺度 $\lambda$ が存在する場合、言葉の乱用により、$\mu$ が尺度であると言うことにします。 $E$ が有限次元の場合、すべてのプロメジャー $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ はメジャーです。つまり、$\{0\} \in \mathscr{F}(E)$、$E/\{0\} = E$、$p_{V,\{0\}} = p_V$、よって $\mu_V = p_V(\mu_{\{0\}})$ のすべての $V \in \mathscr{F}(E)$ についてです。他の語、$\mu = \widetilde{\lambda}$と$\lambda = \mu_{\{0\}}$。

(1) 「射影系」とも呼ばれます。

#### 命題 2 {#int-ix-s6-prop-2 .statement tag=09S8}

— T を可算集合とし、点ごとの収束位相を備えた T 上の実数写像の E ベクトル空間とします。 E 上のすべてのプロメジャーはメジャーです。

すべての $t \in T$ について、$\varepsilon_t$ を E 上の線型形式 $f \mapsto f(t)$ とします。家族 $(\varepsilon_t)_{t \in T}$ はベクトル空間 $E'$ の基底であることがわかります (TVS、II, §6, No. 6、提案 8 の Cor. 2)。 「T」の有限部分集合の $\Phi$ 集合で表し、すべての $J \in \Phi$ について、$E_J$ を T 上の写像の集合とし、J のすべての点で零とします。$F \in \mathscr{F}(E)$ とします。 F の直交 $F^\circ$ は $E'$ の有限次元部分空間であるため、$t \in J$ の $\varepsilon_t$ によって生成される$E'$ の線形部分空間 G に $F^\circ$ が含まれるような $J \in \Phi$ が存在します。 $F^\circ \subset G$ なので、$E_J = G^\circ \subset F^{\circ\circ} = F$ があり、可算家族 $(E_J)_{J \in \Phi}$ は $\mathscr{F}(E)$ の最終です。 命題は Th から続きます。 §4, No. 3の2。

### 2. 計画の像

E と $E_1$ を 2 つの局所的に凸な空間とし、$u$ を E の $E_1$ への連続線形写像とする。 E 属するから $\mathscr{F}(E)$ までの $V_1 \in \mathscr{F}(E_1)$、部分空間 $V = \overline{u}^{-1}(V_1)$、および $u$ 定義するごとに、$E/V$ の商、線形写像 $u_{V_1}$ への通過により、 $E_1/V_1$。 $\mathscr{F}(E_1)$ の $V_1$ と $W_1$ が $V_1 \supset W_1$ になるようにします。 集合 $V = \overline{u}^{-1}(V_1)$ と $W = \overline{u}^{-1}(W_1)$ $V \supset W$ と可換な図式があります。

$$
\begin{array}{ccccc}
E & \xrightarrow{pw} & E/W & \xrightarrow{pvw} & E/V \\
\downarrow u & & \downarrow u_{W_1} & & \downarrow u_{V_1} \\
E_1 & \xrightarrow{pw_1} & E_1/W_1 & \xrightarrow{pv_{1W_1}} & E_1/V_1
\end{array}
$$

ここで、$\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ を E のプロメジャーとします。すべての $V_1 \in \mathscr{F}(E_1)$、集合について

(1)
$$
\nu_{V_1} = u_{V_1}(\mu_{u^{-1}(V_1)}).
$$

前の図式の可換性は、家族$\nu = (\nu_{V_1})_{V_1 \in \mathscr{F}(E_1)}$が$E_1$の対策であることを示しています。 $\nu$は$u$の下の$\mu$の像であると言い、それを$u(\mu)$で表します。

$\lambda$ を E 上の有界メジャー、$u(\lambda)$ を $E_1$ 上のメジャー、つまり $u$ の下の $\lambda$ の像とします。手順 $\mu$ が $\lambda$ に関連付けられている場合、手順 $u(\mu)$ は $u(\lambda)$ に関連付けられます。これは、前の図式の可換性からの続きです。

$V \in \mathscr{F}(E)$ にしましょう。 標準写像$p_V : E \to E/V$の$\mu$の$E/V$の像の施策が$\mu_V$の施策に関連付けられているのが明らかです。

$u_1$ を、局所的に凸な空間 $E_2$ への $E_1$ の連続線形写像とします。難なく確立できます関係

$$
(u_1 \circ u)(\mu) = u_1(u(\mu))
$$

*(対策の像中推移性)*。

### 3. プロメジャーのフーリエ変換

$E$ を局所凸空間とし、$\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ を $E$ 上のプロメジャーとします。 $E$ の連続するすべての線型形式 $x'$ について、$E$ のプロメジャー $\mu$ の $x'$ の下にある $\mathbf{R}$ の像を $\mu_{x'}$ で表します。 $\mu$ のフーリエ変換は、$E'$ 上の写像 $\mathscr{F}\mu$ であり、次のように定義されます。

$$
(\mathscr{F}\mu)(x') = \int_{\mathbf{R}} e^{it} d\mu_{x'}(t).
$$

$\lambda$ を $E$ の有界メジャーとします。 $\lambda$ のフーリエ変換は、$E'$ では写像であり、次のように定義されます。

$$
(\mathscr{F}\lambda)(x') = \int_E e^{i\langle x, x' \rangle} d\lambda(x).
$$

$\mu$ を $\lambda$ に関連付けられたプロメジャーとします。 $x' \in E'$ ごとに、$\mathbf{R}$ の$\mu_{x'}$ は、$E$ の$\lambda$ の$x' : E \to \mathbf{R}$ の下にある像です。 公式 (2) と (3) から、直ちに $\mathscr{F}\mu = \mathscr{F}\lambda$ が推測されます。

$\mu$ を $E$ 上の任意の指標とし、$u$ を局所的に凸な空間 $E_1$ への $E$ の連続線形写像とする。 Denote by $^t u$ the linear mapping of $E'_1$ into $E'$ that is the transpose of $u$, and by $\nu$ the promeasure $u(\mu)$ on $E_1$. $x'_1 \in E'_1$ ごとに、$^t u(x'_1) = x'_1 \circ u$、よってがあります。

$$
\nu_{x'_1} = x'_1(\nu) = x'_1(u(\mu)) = (x'_1 \circ u)(\mu) = \mu_{^t u(x'_1)}.
$$

その結果、

$$
\mathscr{F}(u(\mu)) = (\mathscr{F}\mu) \circ {}^t u.
$$

特に、$E$ の $u$ 標準写像 $p_V$ を $E/V$ ($V \in \mathscr{F}(E)$ の場合) に取り込みます。 $E/V$ のプロメジャー $p_V(\mu)$ はメジャー $\mu_V$ に関連付けられており、$^t p_V$ は、$V$ に直交する $E'$ の部分空間 $V^\circ$ 上の $E/V$ の双対の同型です。 $(E/V)'$ が $^t p_V$ によって $V^\circ$ と識別される場合、

$$
(\mathscr{F}\mu)(x') = \int_{E'/V} e^{i\langle x, x' \rangle} d\mu_V(x)
$$

すべての$x' \in V^\circ$に。 1 つは $E' = \bigcup_{V \in \mathscr{F}(E)} V^\circ$ なので、その前の公式は $E'$ の写像 $\mathscr{F}\mu$ を特徴づけます。最後に、(5) の集合 $x' = 0$ の場合、$\mu$ の総質量は $(\mathscr{F}\mu)(0)$ に等しいことがわかります。

#### 命題 3 {#int-ix-s6-prop-3 .statement tag=09S9}

*$E$を局所的に凸な空間とします。 The mapping $\mu \mapsto \mathscr{F}\mu$ of the set of promeasures on $E$ into the set of functions on $E'$ is injective.*

公式 (5) により、$E$ が有限次元である場合に帰着できます。すべての有限次元空間は空間 $\mathbf{R}^n$ と同型であるため、$E = \mathbf{R}^n$ のような整数 $n \geqslant 0$ が存在すると仮定することもできます。したがって、$\mu$ が $\mathbf{R}^n$ に関する制限された尺度 (必ずしも正であるとは限りません) であるかどうか、および

$$
\int_{\mathbf{R}^n} e^{i\langle x, y \rangle} d\mu(x) = 0
$$

$\mathbf{R}^n$ の線型形式 $y$ ごとに、次に $\mu = 0$ です。

整数 $m \geqslant 0$ ごとに、$G_m$ を $\mathbf{R}^n$ の部分群 $m \cdot \mathbf{Z}^n$ とします。 $\mathbf{R}^n$ で連続する写像 $f$ の $\mathscr{C}_m$ ベクトル空間で、$x \in \mathbf{R}^n$ と $a \in G_m$ が $f(x + a) = f(x)$ になるように表します。 By Prop. 8 of GT, X, §4, No. 4, every function in $\mathscr{C}_m$ is the uniform limit of finite linear combinations of functions of the type $x \mapsto e^{2\pi i \langle x, q \rangle}$ with $q \in m^{-1} \cdot \mathbf{Z}^n$. したがって、写像 $f \in \mathscr{C}_m$ ごとに $\mu(f) = 0$ となります。

$f$ をコンパクトなサポートを備えた $\mathbf{R}^n$ で連続する写像とします。 整数 $m \geqslant 0$、集合 $f_m(x) = \sum_{q \in G_m} f(x + q)$ ごとに。 明らかでは、すべての $x \in \mathbf{R}^n$ に対して、その前の系列には有限の項しかなく、$f_m$ 属するから $\mathscr{C}_m$ までがあります。さらに、数列 $(f_m)$ はすべてのコンパクト集合で一様に $f$ になる傾向があり、すべての $m$ に対して $|f_m| \leqslant C$ となるような定数 $C \geqslant 0$ が存在することも簡単にわかります。従って、§5, No. 6の提案12による$\mu(f) = \lim_{m \to \infty} \mu(f_m)$。 $f_m \in \mathscr{C}_m$から、$\mu(f_m) = 0$、よって、最後に$\mu(f) = 0$です。従って$\mu = 0$。

#### 注意 {#int-ix-s6-n3-rem-1 .statement tag=09SA}

— $E$ が有限次元の場合、$E$ のすべての指標は、$x' \in E'$ を伴う形 $x \mapsto e^{i\langle x, x' \rangle}$ になります (*Théor.spect.*、Ch.II, §1, No. 9、提案 12 の Cor.3)。この場合、提案 3 はフーリエ変換の一意性定理から続きます (*上記引用*、§1, No. 6、提案 6 の補正)*。

### 4. ガウス積分の計算

#### 補題 1 {#int-ix-s6-lem-1 .statement tag=09SB}

整数 $n \geqslant 0$ ごとに、

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2^{n+1 \over 2} \Gamma \left( {n+1 \over 2} \right)
$$
(6)

$$
\int_{\mathbf{R}} x^{2n} e^{-x^2/2} dx = (2\pi)^{1/2} \frac{(2n)!}{2^n n!}
$$
(7)

$$
\int_{\mathbf{R}} x^{2n+1} e^{-x^2/2} dx = 0.
$$
(8)

公式を思い出してください

$$
\Gamma(s) = \int_0^\infty u^{s-1} e^{-u} du
$$
(9)

実数 $s > 0$ ごとに有効です (FRV、VII, §1, No. 3、提案 3)。変数 $x = (2u)^{1/2}$ の変更を作成すると、(9) から次のようになります。

$$
\int_0^\infty x^n e^{-x^2/2} dx = \int_0^\infty (2u)^{n/2} e^{-u} {1 \over 2} 2^{1/2} u^{-1/2} du = 2^{n-1 \over 2} \Gamma \left( {n+1 \over 2} \right),
$$

よって公式 (6) 以来

$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2 \int_0^\infty x^n e^{-x^2/2} dx.
$$

公式 (7) は (6) と関係から続きます

$$
\Gamma \left( n + \frac{1}{2} \right) = \pi^{1/2} \frac{(2n)!}{2^{2n} n!}.
$$
(10)

$n = 0$の場合、この関係簡約するを$\Gamma(\frac{1}{2}) = \pi^{1/2}$、つまりFRVの公式(21)、VII, §1, No. 3にします。次に、一般的なケースでは、関係 $\Gamma(x+1) = x \cdot \Gamma(x)$ を考慮して、$n$ で帰納法が続きます (上記引用、§1, No. 1)。

最後に、写像 $x \mapsto x^{2n+1} e^{-x^2/2}$ が奇数であるという事実から、公式 (8) が得られます。

#### 補題 2 {#int-ix-s6-lem-2 .statement tag=09SC}

複素数 $y$ ごとに、

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = e^{-y^2/2}.
$$
(11)

特に、

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} dx = 1.
$$

変数 $x \mapsto -x$ の変更の利回り

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{-ixy} dx;
$$

複素数 $u$ ごとに $\cos u = \frac{e^{iu} + e^{-iu}}{2}$ から、次のようになります。

$$
(12) \quad (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{i xy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx .
$$

整数 $n \geqslant 0$、集合ごとに

$$
g_n(x) = (-1)^n (2\pi)^{-1/2} \frac{(xy)^{2n}}{(2n)!} e^{-x^2/2}.
$$

(7)により、

$$
(13) \quad \int_{\mathbf{R}} |g_n(x)| \, dx = \frac{1}{n!} \left( \frac{|y|^2}{2} \right)^n
$$
$$
(14) \quad \int_{\mathbf{R}} g_n(x) \, dx = \frac{1}{n!} \left( -\frac{y^2}{2} \right)^n,
$$

よって

$$
\sum_{n=0}^{\infty} \int_{\mathbf{R}} |g_n(x)| \, dx = e^{|y|^2/2} < +\infty.
$$

さらに、

$$
(2\pi)^{-1/2} e^{-x^2/2} \cos xy = \sum_{n=0}^{\infty} g_n(x),
$$

この等式は項、よってによって項を統合できます

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy \, dx = \sum_{n=0}^{\infty} \int_{\mathbf{R}} g_n(x) \, dx = e^{-y^2/2}
$$

(14)による。 公式 (11) は (12) から続きます。

### 5. ガウスの手法と尺度

#### 命題 4 {#int-ix-s6-prop-4 .statement tag=09SD}

*E を局所凸空間とする。 E' 上の正の二次方程式形 Q ごとに、$\mathscr{F} \Gamma_Q = e^{-Q/2}$ となるような E 上のプロメジャー $\Gamma_Q$ が 1 つだけ存在します。 $\Gamma_Q$ の合計質量は 1 に等しくなります。*

$\Gamma_Q$の一意性は、No. 3の提案3から続きます。 $\Gamma_Q$ の総質量は $(\mathscr{F}\Gamma_Q)(0) = e^{-Q(0)/2} = 1$ に等しい。段階的に存在を証明していきます。

A) 有限次元 n の E、および Q は非縮退です。

No. 4の補題 2により、稠密度 $t \mapsto (2\pi)^{-1/2}e^{-t^2/2}$を持つ$\mathbf{R}$の測度$\gamma_1$は、総質量1の有界です。集合 $\gamma = \gamma_1 \otimes \cdots \otimes \gamma_1$ (n 因子)。 No. 4 の補題 2 から、1 つは推測します

$$
\int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n) = \prod_{j=1}^n \int_{\mathbf{R}} e^{ia_j t} d\gamma_1(t)
$$
$$
= \prod_{j=1}^n (2\pi)^{-1/2} \int_{\mathbf{R}} e^{ia_j t} e^{-t^2/2} dt
$$
$$
= \prod_{j=1}^n e^{-a_j^2/2}
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right).
$$

Q は正で非縮退であるため、Q の正規直交 E' の基底 $(e'_1, \ldots, e'_n)$ が存在します (Alg.、Ch. IX, §7, No. 1)。 $\mathbf{R}^n$ 上の E の f 同型 $x \mapsto (e'_1(x), \ldots, e'_n(x))$ を、E 上のメジャー $f^{-1}(\gamma)$ を $\Gamma_Q$ で表しましょう。$x' = a_1 e'_1 + \cdots + a_n e'_n$ が E' にあるとします。次に $x'(f^{-1}(t_1, \ldots, t_n)) = \sum_{j=1}^n t_j a_j$ は $t_1, \ldots, t_n$ 実数、よって

$$
\int_E e^{i\langle x, x' \rangle} d\Gamma_Q(x) = \int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n)
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right) = \exp \left( -\frac{1}{2}Q(x') \right).
$$

結果として、$\mathscr{F}\Gamma_Q = e^{-Q/2}$。

B) E 有限次元。

N を、$Q(x') = 0$ となるような $x'$ によって形成される E' の線形部分空間とします。 E における N の直交を M で表し、E への M の j 標準単射で表します。 線形写像 ${}^t j : E' \to M'$ は核 N で全射であるため、$M'$ 上には $Q = q \circ {}^t j$ となるような非縮退正二次方程式形 q が存在します。上記により、M には $\mathscr{F}\Gamma = e^{-q/2}$ となるような制限された尺度 $\Gamma$ が存在します。 設定 $\Gamma_Q = j(\Gamma)$、私たちは持っています

$$
\mathscr{F}\Gamma_Q = (\mathscr{F}\Gamma) \circ {}^t j = \exp(-q \circ {}^t j/2) = e^{-Q/2}
$$

No. 3 の公式 (4) によって。

C) *一般的なケース*
$V \in \mathscr{F}(E)$ にしましょう。 Denote by $p_V$ the canonical mapping of $E$ onto $E/V$, and by $Q_V$ the positive quadratic form $Q \circ {}^t p_V$ on $(E/V)'$; finally, let $\mu_V$ be the measure on $E/V$ with Fourier transform $e^{-Q_V/2}$ (cf. B)). $W \in \mathscr{F}(E)$が$V$に含まれる場合、$p_V = p_{VW} \circ p_W$、よって、$Q_V = Q_W \circ {}^t p_{VW}$。 No. 3 の公式 (4) により、測度 $p_{VW}(\mu_W)$ はフーリエとして変換写像 $(e^{-Q_W/2}) \circ {}^t p_{VW} = e^{-Q_V/2}$ となるため、$\mu_V$ に等しくなります。 従って、ファミリー $(\mu_V)_{V \in \mathscr{F}(E)}$ は、$E$ のプロメジャー $\mu$ です。 No. 3 の公式 (5) は、$\mathscr{F}\mu$ が $e^{-Q/2}$ に等しいことを示しています。

#### 定義 2 {#int-ix-s6-def-2 .statement tag=09SE}

*$E$を局所凸空間とする。 $E'$ 上のすべての正の 2 次方程式形 $Q$ について、フーリエ変換が $e^{-Q/2}$ に等しい $E$ のプロメジャーは、分散 $Q$ を持つ $E$ のガウスプロメジャーと呼ばれ、$\Gamma_Q$ と表されます。 $\mu = \Gamma_Q$ となるような正の二次方程式形 $Q$ が $E'$ に存在する場合、$E$ のプロメジャー $\mu$ はガウスであると言われます。

言葉の乱用により、関連するプロメジャー $\widetilde{\mu}$ が $\Gamma_Q$ に等しい場合、$E$ 上の有界メジャー $\mu$ は分散 $Q$ を伴うガウスであると言われます。

#### 注意 {#int-ix-s6-n5-rem-1 .statement tag=09SF}

— 1) $E$ を有限次元ベクトル空間とし、$\mu$ を質量 1 の $E$ に対する正の尺度とし、$E$ 属するから $\mathscr{L}^2(E, \mu)$ までのすべての線型形式を計算します。 $E$ の 1 つの定義する元 $m$ と、公式による $E'$ 上の正の二次関数形 $V$
$$
\langle m, x' \rangle = \int_E \langle x, x' \rangle d\mu(x), \quad V(x') = \int_E \langle x - m, x' \rangle^2 d\mu(x).
$$
確率理論の伝統的な用語では、$m$は$\mu$の*平均*、$V$は*分散*と呼ばれます。 $m = 0$ の場合、$\mu$ は *中央にある* と言われます。

ここで、$a$ を $E$ の元とし、$Q$ を $E'$ 上の正の 2 次式形とします。 $x \mapsto x + a$ の翻訳の下で、$\Gamma_Q$ の小節を $\Gamma_{a,Q}$ 像で表すことにします。 $\Gamma_{a,Q}$ は質量 1 の $E$ に対する正の尺度であり、フーリエ変換 $x' \mapsto e^{i\langle a, x' \rangle - \frac{1}{2} Q(x')}$ と平均 $a$ であることが容易にわかります。さらに、以下の提案 6 は、$Q$ が $\Gamma_{a,Q}$ の分散であることを意味します。伝統的に、$\Gamma_{a,Q}$ は平均 $a$ と分散 $Q$ をもつガウス測度であり、$\Gamma_Q = \Gamma_{0,Q}$ は分散 $Q$ をもつ *中心の* ガウス測度であると言われています。 *中心の* ガウス測度のみを考慮するため、この修飾子は省略します。

2) $Q$ を、局所凸型空間 $E$ の双対 $E'$ 上の二次方程式形とします。 If there exists a promeasure on $E$ with Fourier transform $e^{-Q/2}$, the quadratic form $Q$ is necessarily positive: for, the function $e^{-Q/2}$ is bounded on $E'$; therefore, for every $x' \in E'$, the function $t \mapsto e^{-t^2 Q(x')/2} = e^{-Q(tx')/2}$ on $\mathbf{R}$ is bounded, whence $Q(x') \geq 0$.

3) $\mathbf{R}$ の双対は $\mathbf{R}$ と正準同型であり、$\mathbf{R}$ 上の正の二次方程式形は形 $t \mapsto at^2$ と $a \geq 0$ の写像です。したがって、すべての $a \geq 0$ に対して、$\mathbf{R}$ 上に唯一の有界測度 $\gamma_a$ が存在し、そのフーリエ変換は写像 $t \mapsto e^{-at^2/2}$ に等しくなります。言葉の乱用により、$\gamma_a$ は、分散 $a$* を伴う $\mathbf{R}$ の *ガウス測度であると言われます。

$\gamma_0$ のフーリエ変換は定数 1、よって $\gamma_0 = \varepsilon_0$ ($\mathbf{R}$ の原点における質量単位元) です。 $a > 0$ を仮定し、$u_a$ 線形写像 $x \mapsto a^{1/2} x$ で表します。次に、$\mathscr{F}\gamma_a = \mathscr{F}\gamma_1 \circ {}^t u_a$、よって、$\gamma_a = u_a(\gamma_1)$。 補題 2 は、$\gamma_1$ がルベーグ測度に関して稠密度 $x \mapsto (2\pi)^{-1/2} e^{-x^2/2}$ を伴う測度であることを示します。このことから、簡単に推測できます

$$
(15) \quad d\gamma_a(x) = (2\pi a)^{-1/2} e^{-x^2/2a} dx .
$$

連続線形写像の下でのガウス測度の像はガウス測度です。より正確には、次の結果が得られます。

#### 命題 5 {#int-ix-s6-prop-5 .statement tag=09SG}

*E と E₁ を 2 つの局所的に凸な空間とし、u を E から E₁ への連続線形写像とします。 Q を E' 上の正の 2 次式形とし、Q1 を E'₁ 上の正の 2 次式形 Q $\circ {}^t u$ とします。次に、$u(\Gamma_Q) = \Gamma_{Q_1}$.*

集合 $\mu = u(\Gamma_Q)$。 No. 3 の公式 (4) により、

$$
\mathscr{F}\mu = (\mathscr{F}\Gamma_Q) \circ {}^t u = e^{-Q/2} \circ {}^t u = e^{-Q_1/2} = \mathscr{F}\Gamma_{Q_1} ,
$$

No. 3の提案3によるよって $\mu = \Gamma_{Q_1}$。

#### 系 {#int-ix-s6-n5-cor-1 .statement tag=09SH}

*E を局所凸空間とし、Q を E' 上の正の二次方程式形とします。 $x'$ の下の $\Gamma_Q$ のすべての $x' \in E'$、像は、分散 $Q(x')$ を伴う $\mathbf{R}$ のガウス測度です。*

#### 命題 6 {#int-ix-s6-prop-6 .statement tag=09SI}

*E を局所凸空間とし、分散 Q を持つ E 上のガウス測度 $\mu$ とします。すべての整数 $n \geq 0$ とすべての $x' \in E'$ について、1 つは関係* になります

$$
\begin{align*}
(16) & \quad \int_E |\langle x, x' \rangle|^n d\mu(x) = \pi^{-1/2} 2^{n/2} \Gamma\left( \frac{n+1}{2} \right) Q(x')^{n/2} \\
(17) & \quad \int_E \langle x, x' \rangle^{2n} d\mu(x) = \frac{(2n)!}{2^n n!} Q(x')^n \\
(18) & \quad \int_E \langle x, x' \rangle^{2n+1} d\mu(x) = 0 .
\end{align*}
$$

*特に、*

$$
(19) \quad \int_E \langle x, x' \rangle^2 d\mu(x) = Q(x') \qquad (x' \in E') .
$$

これらの公式が $E'$ の元 $x'$ に当てはまる場合、その倍数 $t \cdot x'$ (実数の $t$ を含む) のすべてに当てはまります。したがって、$Q(x')$ が 0 または 1 に等しい場合にそれらを確立することに満足するかもしれません。

a) $Q(x') = 0$ と仮定します。尺度 $x'(\mu)$ は $\gamma_0 = \varepsilon_0$ に等しいため、$x'$ はほぼどこでも零 $\mu$ になります。 公式 (16) ～ (19) は明らかです。

b) $Q(x') = 1$、よって $x'(\mu) = \gamma_1$ と仮定します。それから
$$
\int_E |\langle x, x' \rangle|^n d\mu(x) = \int_{\mathbf{R}} |t|^n d\gamma_1(t) = (2\pi)^{-1/2} \int_{\mathbf{R}} |t|^n e^{-t^2/2} dt
$$
(16) は (6) の直後に続きます (No 4、補題 1)。同様に、公式 (17) と (18) は (7) と (8) から続きます。最後に、(17) の設定 $n = 1$ により、(19) が得られます。

これでコルの逆を証明できます。提案 5 の。

#### 命題 7 {#int-ix-s6-prop-7 .statement tag=09SJ}

*E を局所凸空間および $\mu$ を E 上のプロメジャーとします。$x'(\mu)$ がすべての $x' \in E'$ に対する $\mathbf{R}$ 上のガウスメジャーであると仮定します。したがって、$\mu$ は E に関するガウスプロメジャーです。*

すべての $x' \in E'$ について、$Q(x')$ を $\mathbf{R}$ のガウス測度 $x'(\mu)$ の分散とします。 1 つは $x'(\mu) = \gamma_{Q(x')}$、よってです
$$
(\mathscr{F}\mu)(x') = \int_{\mathbf{R}} e^{it \cdot 1} d\gamma_{Q(x')}(t) = e^{-Q(x') \cdot 1^2 / 2}
$$
$\mathscr{F}\mu$ の定義による (No. 3、公式 (2))。他の語、$\mathscr{F}\mu = e^{-Q/2}$、そして$Q$が$E'$上の正の二次方程式形であることを証明することが残っています。

For every closed linear subspace V of E with finite codimension, denote by $p_V$ the canonical mapping of E onto $E/V$, by $\mu_V$ the measure $p_V(\mu)$ on $E/V$, and set $Q_V = Q \circ {}^t p_V$. $E' = \bigcup_{V \in \mathscr{F}(E)} \operatorname{Im}({}^t p_V)$ と ${}^t p_V$ は単射なので、$Q_V$ が $(E/V)'$ 上の正の二次方程式形であることを証明すれば十分です。 $u \in (E/V)'$ と $x' = {}^t p_V(u)$ としましょう。 私たちは持っています
$$
u(\mu_V) = u(p_V(\mu)) = x'(\mu) = \gamma_{Q(x')} ;
$$
提案 6 は次のことを意味します。
$$
Q_V(u) = Q(x') = \int_{\mathbf{R}} t^2 d\gamma_{Q(x')}(t) = \int_{E/V} u(x)^2 d\mu_V(x),
$$
したがって、$Q_V$ は $(E/V)'$ 上の正の二次方程式形です。

### 6. ガウスプロメジャーの例

1) E を実際のヒルベルト空間とします。 写像 $x' \mapsto \|x'\|^2$ は、$E'$ 上の正の 2 次式形です。 対応するガウス プロメジャーは、E に関する *標準ガウス プロメジャー* と呼ばれます。E が無限次元の場合、このプロメジャーはメジャーではないことが示されます。

$A$ を $E$ 上の連続線形演算子とします。 写像 $x' \mapsto \|{}^tA \cdot x'\|^2$ は、$E'$ 上の正の 2 次式形です。 $E$ の対応するプロメジャー $\mu_A$ は、$A$ がヒルベルト・シュミット演算子 (cf. No. 11、Th. 3 の Cor. 2) である場合に限り、メジャーです。

2) 正の型の*核.* $T$を集合、$T$の実数写像の$E = \mathbf{R}^T$ベクトル空間とし、点収束の位相を装備します。 $t \in T$ ごとに、1 は $E$ の $\varepsilon_t$ 線型形式 $f \mapsto f(t)$ を表します。ファミリー $(\varepsilon_t)_{t \in T}$ は $E'$ の基底です (TVS、II, §6, No. 6、提案 8 の Cor. 2)。

$T \times T$ 満たす関係の実数値写像 $K$ ごとに、$T$ で正の型の (実数) 核を呼び出します。

$$
\text{(20)} \qquad K(t, t') = K(t', t) \quad \text{for } t, t' \text{ in } T,
$$
$$
\text{(21)} \qquad \sum_{i,j=1}^p c_i c_j K(t_i, t_j) \geqslant 0
$$

$T$ のいずれかの正の整数 $p$、元 $t_1, \ldots, t_p$、および実数 $c_1, \ldots, c_p$ の場合。そうであれば、公式

$$
\text{(22)} \qquad q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t,t' \in T} c_t c_{t'} K(t, t')
$$

定義する $E'$ の正の二次方程式形。逆に、$q$ が $E'$ 上の正の 2 次式形である場合、公式

$$
\text{(23)} \qquad K(t, t') = \frac{1}{2} [q(\varepsilon_t + \varepsilon_{t'}) - q(\varepsilon_t) - q(\varepsilon_{t'})]
$$

$T$の型のポジティブの定義する核$K$。したがって、$T$ の正の型の核の集合と、$E'$ の正の二次方程式形の間で、相互に 2 つの逆全単射が得られます。

$K$ を $T$ の正の型の核とし、$q$ を $E'$ の関連二次方程式形とします。分散 $q$ を伴う $E$ のガウス プロメジャーは、共分散 $K$ を伴う $E$ の *ガウス プロメジャーとも呼ばれます。 $T$ が可算である場合、No. 1 の提案 2 は、この手順がメジャーであることを意味します。

3) $T$ を可算数集合とします。 型の$T$ 上の核 $\delta$ は、設定によって定義されます

$$
\text{(24)} \qquad \delta(t, t') = \begin{cases}
1 & \text{if } t = t' \\
0 & \text{if } t \neq t'.
\end{cases}
$$

対応する二次関数形は $q\left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t \in T} c_t^2$ で与えられます。すべての $t \in T$ について、分散 1 の $\mathbf{R}$ のガウス測度を $\mu_t$ で表します。

共分散 $\delta$ を伴う $\mathbf{R}^T$ のガウス測度が $\bigotimes_{t \in T} \mu_t$ に等しいことが簡単にわかります。

4) $n \geq 1$ を整数とします。 平方行列 $C = (c_{ij})$ の位数 $n$ は、対称であれば *正対称* であると言われ、実数 $x_1, \ldots, x_n$ の場合は $\sum_{i,j=1}^n c_{ij} x_i x_j \geq 0$ と言われます。 写像 $(i, j) \mapsto c_{ij}$ が集合 $\{1, 2, \ldots, n\}$ の正の型の核であると言うのと同じことになります。したがって、共分散 $C$ を伴う $\mathbf{R}^n$ 上のガウス測度 $\gamma_C$ について話すことができます。 公式が特徴です

$$
(25) \quad \int_{\mathbf{R}^n} e^{i(x_1 t_1 + \cdots + x_n t_n)} d\gamma_C(t_1, \ldots, t_n) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_{jk} x_j x_k \right),
$$

$x_1, \ldots, x_n$ 実質。 No. 5 (公式 (19)) の提案 6 から、次のように推測できます。

$$
(26) \quad \int_{\mathbf{R}^n} t_j t_k d\gamma_C(t_1, \ldots, t_n) = c_{jk} \quad (1 \leq j, k \leq n).
$$

No. 5 の提案 5 から、公式が推測されます。

$$
(27) \quad u(\gamma_C) = \gamma_{UC^t U},
$$

ここで、$u$ は、$\mathbf{R}^n$ の線形写像を行列 $U$ で$\mathbf{R}^m$ に変換します。さらに、$I_n$ が位数 $n$ の同一性行列である場合、測度 $\gamma_{I_n}$ が認めることは簡単にわかります (No. 5 の提案 4 の証明の最初の部分 cf.) 稠密度

$$
(2\pi)^{-n/2} \exp \left( - \frac{1}{2}(t_1^2 + \cdots + t_n^2) \right)
$$

$\mathbf{R}^n$ のルベーグ測度 $\lambda_n$ に関して。

行列 $C$ が逆$D = (d_{jk})$ を使用して可逆である場合、次のようになります。

$$
(28) \quad d\gamma_C(t_1, \ldots, t_n) =
(2\pi)^{-n/2} (\det D)^{1/2} \left( \exp \left( - \frac{1}{2} \sum_{j,k=1}^n d_{jk} t_j t_k \right) \right) dt_1 \cdots dt_n.
$$

なぜなら、$C$ が可逆である場合、$\mathbf{R}^n$ 上の二次方程式形 $q$ は次のように定義されます。

$$
q(x_1, \ldots, x_n) = \sum_{j,k=1}^n c_{jk} x_j x_k
$$

非退化です。 $q$ の正規直交 $\mathbf{R}^n$ の基底の存在を使用して、$C = U \cdot {}^tU$、よって $\gamma_C = u(\gamma_{I_n})$ のように、位数 $n$ の平方行列 $U$ の存在を証明します。 (27) (ここで、$u$ は $\mathbf{R}^n$ の自己同型と行列 $U$ を表します)。 $Q$ を、次のように定義される $\mathbf{R}^n$ 上の 2 次式形とします。
$$
Q(t_1, \ldots, t_n) = t_1^2 + \cdots + t_n^2;
$$
それから
$$
\gamma_{I_n} = (2\pi)^{-n/2} e^{-Q/2} \cdot \lambda_n,
$$
よって
$$
u(\gamma_{I_n}) = (2\pi)^{-n/2} e^{-(Qou^{-1})/2} \cdot u(\lambda_n).
$$
$\mathbf{R}^n$ 上の二次方程式形 $Q \circ u^{-1}$ が点 $(t_1, \ldots, t_n)$ で値 $\sum_{j,k=1}^n d_{jk} t_j t_k$ をとるのは明らかであり、第 3 章の提案 15 です。 VII, §1, No. 10 は次のことを示しています
$$
u(\lambda_n) = (\det U)^{-1} \cdot \lambda_n = (\det D)^{1/2} \cdot \lambda_n.
$$
公式 (28) が続きます。

### 7. ウィンナーメジャー

In this No., we denote by $T$ the interval $]0, 1]$ of $\mathbf{R}$ and by $\mathscr{H}$ the Hilbert space of real functions on $T$ square-integrable with respect to Lebesgue measure, where the scalar product is denoted $(f|g)$. また、$T$ 上の連続実数写像が点 0 で 0 になる傾向があることを $\mathscr{C}$ 空間で表します。 $\mathscr{C}$ にはノルム $\|f\| = \sup_{t \in T} |f(t)|$ を装備します。 コンパクト区間 $[0, 1] = T \cup \{0\}$ は、局所的にコンパクトではあるがコンパクトではない区間 $T$ を Alexandroff コンパクト化したものです。その結果、コンパクトなサポートを伴う$T$の連続写像の集合は$\mathscr{C}$に密集しており、$\mathscr{C}$の双対は$T$の限定されたメジャー（必ずしも正ではない）の空間$\mathscr{M}^1$と識別される可能性があります（Ch. III, §1, No. 8、デフォルト。 3)。

写像 $f \in \mathscr{H}$ ごとに、$T$ に 1 つの定義する写像 $Pf$
$$
(Pf)(t) = \int_0^t f(x) \, dx = (f|I_t),
$$
ここで、$I_t$ は、区間 $]0, t]$ の特性写像です。コーシー＝シュワルツ不等式は不等式を暗示します
$$
|(Pf)(t)| \leq \|f\|_2 \cdot t^{1/2}
$$
$$
|(Pf)(t) - (Pf)(t')| \leq \|f\|_2 \cdot |t - t'|^{1/2};
$$

consequently, $Pf$ belongs to $\mathscr{C}$, and the linear mapping $P$ of $\mathscr{H}$ into $\mathscr{C}$ is continuous with norm $\leqslant 1$.

双対 (TVS、V, §1, No. 7、Th. 3) を持つヒルベルト空間 $\mathscr{H}$ を同一視するとし、$P : \mathscr{H} \to \mathscr{C}$ の $\Pi : \mathscr{M}^1 \to \mathscr{H}$ 転置で表します。すべてのメジャー $\mu \in \mathscr{M}^1$ とすべての写像 $f \in \mathscr{H}$ について、

$$
(\Pi \mu | f) = \mu(Pf) = \int_{\mathbf{T}} d\mu(t) \int_{\mathbf{T}} I_t(x) f(x) \, dx
$$
$$
= \int_{\mathbf{T}} f(x) \, dx \int_{\mathbf{T}} I_t(x) \, d\mu(t)
$$

ルベーグ・フビニ定理による。さて、

$$
I_t(x) = \begin{cases}
1 & \text{if } 0 < x \leq t \leq 1 \\
0 & \text{otherwise},
\end{cases}
$$

よってついに

(34) $$ (\Pi \mu)(x) = \mu([x, 1]) \quad \text{for } x \in \mathbf{T}. $$

$\mu, \nu$ を $\mathscr{M}^1$ に入れます。それから

$$
(\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \Pi \mu(x) \Pi \nu(x) \, dx = \int_{\mathbf{T}} dx \int_{\mathbf{T}} I_t(x) \, d\mu(t) \int_{\mathbf{T}} I_{t'}(x) \, d\nu(t')
$$
$$
= \int_{\mathbf{T}} \int_{\mathbf{T}} d\mu(t) \, d\nu(t') \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx.
$$

さて、$I_t \cdot I_{t'}$ はすぐに区間 $]0, t] \cap ]0, t']$、よっての特性写像になります

(35) $$ \int_{\mathbf{T}} I_t(x) I_{t'}(x) \, dx = \inf(t, t'). $$

したがって、

(36) $$ (\Pi \mu | \Pi \nu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\nu(t'). $$

前述の結果により、1 つの定義する形 $W$ $\mathscr{M}^1$ by 公式

(37) $$ W(\mu) = \int_{\mathbf{T}} \int_{\mathbf{T}} \inf(t, t') \, d\mu(t) \, d\mu(t') = \| \Pi \mu \|_2^2. $$

特に、$t_1, \ldots, t_n$ が T の元で、$c_1, \ldots, c_n$ が実数である場合、
$$
W \left( \sum_{j=1}^n c_j \varepsilon_{t_j} \right) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k)
$$
そして W が正であるため、写像 $(t, t') \mapsto \inf(t, t')$ は T の正の型の核です。

**定理 1 (ウィーナー).** — *w をヒルベルト空間 $\mathscr{H}$ の標準ガウス プロメジャーの $P : \mathscr{H} \to \mathscr{C}$ の下で像とします。この場合、w は分散 W* を持つ $\mathscr{C}$ のガウス測度です。

構成、$W(\mu) = \|^tP(\mu)\|_2^2$までに。 No. 5 の提案 5 は、w が分散 W を持つガウスプロメジャーであることを示しています。w が $\mathscr{C}$ 上のメジャーであることを証明することはまだ残っています。

A) 補助測定値空間*^{(2)} $(\Omega, m)$ の *構成:
整数 $n \geqslant 0$ ごとに、形 $k/2^n$ の数の $D_n$ 集合を $k = 1, 2, 3, \ldots, 2^n$ で表します。 集合 $D = \bigcup_{n \geqslant 0} D_n$ (T に含まれる二項数の集合) と $\Omega = \mathbf{R}^D$。 $t \in D$ ごとに、$\Omega$ に $X(t)$ 線型形式 $f \mapsto f(t)$ で示します。

D の $t, t'$ の場合、集合 $M(t, t') = \inf(t, t')$; M は D 上で正の型の核であることがわかりました。 集合 D は可算であるため、共分散 M (No. 6, *例 2*) を使用して $\Omega$ 上の m をガウス *測定* 定義するすることができます。

#### 補題 3 {#int-ix-s6-lem-3 .statement tag=09SK}

*D の任意の $t, t'$ については、
$$
\int_\Omega \left| X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2} \right|^3 dm = \frac{1}{(8\pi)^{1/2}} |t - t'|^{3/2}.
$$
D に対する $\frac{t + t'}{2}$ 属するに注意してください。(No. 6, *例 2*) ファミリ $(X(t))_{t \in D}$ が $\Omega$ の位相双対 $\Omega'$ の基底であることがわかっています。したがって、$\widehat{M}(X(t), X(t')) = \inf(t, t')$ を特徴とする対称的な双線形形式 $\widehat{M}$ が $\Omega' \times \Omega'$ 上に存在します。 構成までに、$\Omega$ 上のガウス測定の分散は、$\Omega'$ 上の 2 次式形 $\xi \mapsto \widehat{M}(\xi, \xi)$ になります。 集合、特に、
$$
\xi = X\left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2};
$$
簡単な計算で得られるのは
$$
\widehat{M}(\xi, \xi) = \frac{|t - t'|}{4}.
$$

(2) *エスパス測定*: 測定を備えた局部的にコンパクトな空間 (Ch. III、第 1 版、§2, No. 2、p. 52)。

No. 5 (公式 (16)) の提案 6 により、

$$
\int_{\Omega} |\xi|^3 \, dm = \pi^{-1/2} 2^{3/2} \Gamma(2) \widehat{M}(\xi, \xi)^{3/2};
$$

補題は、公式 (40) および (41) の直後に続きます。

B) *構成の写像uの$\Omega$を$\mathscr{C}$に変換:*
すべての整数 $n \geqslant 0$ について、$1 \leqslant k \leqslant 2^n$ の区間 $\left[ \frac{k-1}{2^n}, \frac{k}{2^n} \right]$ のそれぞれでアフィンである写像によって形成される $\mathscr{C}$ の $E_n$ 部分空間で表します。 $\mathbf{R}$ のコンパクト区間 I 上のアフィン写像は、I の端点で境界に達します。従って、

$$
\|f\| = \sup_{1 \leqslant k \leqslant 2^n} \left| f\left( \frac{k}{2^n} \right) \right|
$$

$f \in E_n$の場合。

すべての写像 $g \in \Omega$ とすべての整数 $n \geqslant 0$ には、属するから $E_n$ および一致するの点ごとに $g$ が含まれる写像 $u_n(g)$ が 1 つだけ存在します。 $D_n$; $T_n g = u_{n+1}(g) - u_n(g)$と書きます。 $D_n$ は有限であるため、$\Omega$ から $\mathscr{C}$ への写像 $T_n$ は連続であり、従って $m$ は可測です。

#### 補題 4 {#int-ix-s6-lem-4 .statement tag=09SL}

— *整数 $n \geqslant 0$ごとに、*

$$
\int_{\Omega} \|T_n g\|^3 \, dm(g) \leqslant \frac{1}{(8\pi)^{1/2}} 2^{-n/2}.
$$

$g \in \Omega$と$n \in \mathbf{N}$としましょう。 1 つは $E_n \subset E_{n+1}$ です。従って、写像 $T_n g$ 属するから $E_{n+1}$ となり、$D_n$ の点ごとに零になります。従って、(42) により、

$$
\|T_n g\|^3 = \sup_{1 \leqslant k \leqslant 2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \leqslant \sum_{k=1}^{2^n} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3.
$$

大会$g(0) = 0$を作りましょう。 $g$ の線形補間による $u_n(g)$ の構成は、関係を意味します

$$
T_n g\left( \frac{2k-1}{2^{n+1}} \right) = g\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( g\left( \frac{k-1}{2^n} \right) + g\left( \frac{k}{2^n} \right) \right)
$$

$1 \leqslant k \leqslant 2^n$の場合。これから、積分により次のように推測されます。

$$
\int_{\Omega} \left| T_n g\left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \, dm(g) = \int_{\Omega} \left| X\left( \frac{2k-1}{2^{n+1}} \right) - \frac{1}{2} \left( X\left( \frac{k-1}{2^n} \right) + X\left( \frac{k}{2^n} \right) \right) \right|^3 \, dm;
$$

![図1](../images/figure_1.png)

図1

次に、補題 3 を $t = \frac{k-1}{2^n}$、$t' = \frac{k}{2^n}$、よってに適用できます。

$$
\int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^{-\frac{3n}{2}} .
$$

(44) までに、次のようになります。

$$
\int_{\Omega} \| T_n g \|^3 dm(g) \leq \sum_{k=1}^{2^n} \int_{\Omega} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^n \cdot 2^{-\frac{3n}{2}} ,
$$

よって補題。

補題 4、写像 $T_n$ から $\Omega$ までに、バナッハ空間 $\mathscr{C}$ 属するから $L^3_{\mathscr{C}}(\Omega, m)$ および$N_3(T_n) \leq \frac{1}{(8\pi)^{1/6}} (2^{-1/6})^n$、よって $\sum_{n=0}^{\infty} N_3(T_n) < +\infty$ まで。第 6 章の提案による。 IV, §3, No. 3 では、$\Omega - \Omega_0$ が $m$ 無視でき、系列 $\sum_{n=0}^{\infty} T_n(g)$ が $g \in \Omega_0$ ごとに $\mathscr{C}$ に絶対収束するような集合 $\Omega_0 \subset \Omega$ が存在します。 1 つ目から定義するは、$\Omega$ の $m$ で測定可能な写像 $u$ を $\mathscr{C}$ に変換します。

$$
u(g) = \begin{cases}
\sum_{n=0}^{\infty} T_n g = \lim_{n \to \infty} u_n(g) & \text{for } g \in \Omega_0 \\
0 & \text{for } g \in \Omega - \Omega_0 .
\end{cases}
$$

$0 \leq m \leq n$の$D_m \subset D_n$の$u_n(g)$と$g$一致するなので、$u(g)$から$D$の制限が$g \in \Omega_0$ごとに$g$に等しいのは明らかです。

C) $\mathscr{C}$ のガウス測定の構成:
$w'$ を、$\mathscr{C}$ の境界メジャー、つまり、$m$ 可測写像 $u : \Omega \to \mathscr{C}$ の下で、$m$ の像とします。 $w'$ が $\mathscr{C}$ のガウス測度であり、分散 $W$、よって $w = w'$ があることを示します。 $t$ が $D$ を通過するための$\varepsilon_t$ の措置によって生成された $\mathscr{M}^1$ の線形部分空間を $\mathscr{D}$ で示します。

#### 補題 5 {#int-ix-s6-lem-5 .statement tag=09SM}

$\mu \in \mathscr{D}$ の小節ごとに、

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = e^{-W(\mu)/2}.
$$

集合 $\mu = c_1 \varepsilon_{t_1} + c_2 \varepsilon_{t_2} + \cdots + c_n \varepsilon_{t_n}$ で、$D$ には $t_1, \ldots, t_n$ が、$\mathbf{R}$ には $c_1, \ldots, c_n$ が入ります。 $g \in \Omega_0$、写像 $u(g)$ 一致するごとに、$D$ には $g$ が付きます。したがって

$$
\langle u(g), \mu \rangle = \sum_{j=1}^n c_j g(t_j) \qquad (g \in \Omega_0).
$$

また、

$$
W(\mu) = \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k),
$$

そして、$m$ は共分散 $M$ を伴う $\Omega$ のガウス測度であり、$\Omega - \Omega_0$ は $m$ 無視できるため、次のようになります。

$$
\int_{\Omega_0} e^{i \sum_{j=1}^n c_j g(t_j)} \, dm(g) = \exp \left( - \frac{1}{2} \sum_{j,k=1}^n c_j c_k \inf(t_j, t_k) \right).
$$

さて、$\Omega - \Omega_0$ は $m$ は無視でき、$w' = u(m)$ です。それは次のとおりです

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} \, dw'(f) = \int_{\Omega_0} e^{i \langle u(g), \mu \rangle} \, dm(g).
$$

公式 (48) は、公式 (49) から (52) のすぐ後に続きます。

#### 補題 6 {#int-ix-s6-lem-6 .statement tag=09SN}

$\mu \in \mathscr{M}^1$ にしましょう。すべての $f \in \mathscr{C}$ と $W(\mu) = \lim_{n \to \infty} W(\mu_n)$ に対して $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ となるようなメジャー $\mu_n \in \mathscr{D}$ の数列が存在します。

$I = [0, 1]$ にしましょう。 $T = ]0, 1[$ の制限付き措置の空間 $\mathscr{M}^1$ は、$0$ に重みを配置しない措置によって形成される $\mathscr{M}(I)$ の部分空間と識別されます。 (3) $\mathscr{M}(I)$に曖昧な位相を装備します。 写像

(3)つまり、$T = I - \{0\}$に集中した$I$の対策です。

$I$ から $\mathscr{M}(I)$ への $t \mapsto \varepsilon_t$ は連続です (Ch. III, §1, No. 9、提案 13)。 D は I で密であるため、$\mathscr{D}$ 含むの閉包 $\overline{\mathscr{D}}$ は点メジャーすべてに適用されます。 A を $\| \nu \| \leq \| \mu \|$ となるようなメジャー $\nu \in \mathscr{D}$ の集合とします。小節 $\mu$ は A の終わりにあります (Ch. III, §2, No. 4、Th. 1 の Cor. 1)。 集合 A は、$\mathscr{M}(I)$ (Ch. III, §1, No. 9、提案 15) で比較的コンパクトであり、$\mathscr{M}(I)$ のコンパクトな部分集合は計量化可能です (TVS、III, §3, No. 4、提案 6 (4) の Cor. 2 および GT、X, §3, No. 3、Th. 1)。したがって、$\mathscr{M}(I)$ で$\mu$ に収束する$\mu_n \in A$ の措置の数列が存在します。 $\mathscr{C}$ は原点でI 零に連続する写像の部分空間と同一視されるので、すべての $f \in \mathscr{C}$ に対して $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ が得られます。さらに、$\mathscr{C}(I) \otimes \mathscr{C}(I)$ は正規化された空間 $\mathscr{C}(I \times I)$ (Ch. III, §4, No. 1, 補題 1) で密であるため、関係 $\lim_{n \to \infty} \mu_n = \mu$ と $\| \mu_n \| \leq \| \mu \|$ は $\lim_{n \to \infty} (\mu_n \otimes \mu_n) = \mu \otimes \mu$ (Ch. III, §1, No. 10,提案 17);メジャー $\mu_n$ と $\mu$ では重みが 0 に配置されるため、次のようになります。

$$
W(\mu_n) = \int_I \int_I \inf(t, t') d\mu_n(t) d\mu_n(t'),
$$
$$
W(\mu) = \int_I \int_I \inf(t, t') d\mu(t) d\mu(t'),
$$

よって $\lim_{n \to \infty} W(\mu_n) = W(\mu)$。

$w'$ のフーリエ変換が $e^{-W/2}$ に等しいことを証明することはまだ残っています。 $\mu \in \mathscr{M}^1$ にしましょう。 選ぶメジャー $\mu_n \in \mathscr{D}$ は補題と同様です。 6. メジャー $w'$ は有界であり、すべての $n$ に対して $|e^{i \langle f, \mu_n \rangle}| = 1$ です。 補題 5 とルベーグの収束定理 (Ch. IV, §4, No. 3, Th. 2) は次のことを意味します。

$$
\int_{\mathscr{C}} e^{i \langle f, \mu \rangle} dw'(f) = \lim_{n \to \infty} \int_{\mathscr{C}} e^{i \langle f, \mu_n \rangle} dw'(f)
= \lim_{n \to \infty} e^{-W(\mu_n)/2} = e^{-W(\mu)/2}.
$$

Q.E.D.

フーリエ変換が $e^{-W/2}$ に等しい $\mathscr{C}$ 上の測度 $w$ は、$\mathscr{C}$* の *ウィーナー測度 と呼ばれます。

#### 注意 {#int-ix-s6-n7-rem-1 .statement tag=09SO}

— T に含まれるすべての半開区間 $J = ]a, b]$ について、集合 $l(J) = b - a$ (J の長さ) とし、$\mathscr{C}$ 上の $A_J$ 線型形式 $f \mapsto f(b) - f(a)$ で表します。ウィーナー測度は次の性質によって特徴付けられることがわかります。

*$J_1, \ldots, J_n$をTに含まれるセミオープン区間とペアの互いに素とする。 線形写像 $f \mapsto (A_{J_1}(f), \ldots, A_{J_n}(f))$ から $\mathscr{C}$ を $\mathbf{R}^n$ に変換した小節の像は、 $1 \leq i \leq n$ に対する $a_i = l(J_i)^{1/2}$ を含む $\gamma_{a_1} \otimes \cdots \otimes \gamma_{a_n}$ に等しくなります。

### 8. フーリエの連続性変換

#### 命題 8 {#int-ix-s6-prop-8 .statement tag=09SP}

— E を局所凸空間、E 上のプロメジャー $\mu$、および $\mu$ のフーリエ変換を $\Phi$ とします。片方には不平等がある

$$
|\Phi(x')| \leq \Phi(0)
$$
$$
|\Phi(x') - \Phi(y')|^2 \leq 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right)
$$

$E'$の$x', y'$用。

No. 3 の公式 (5) により、E が有限次元であり、$\mu$ が測度である場合に帰着できます。それから

$$
|\Phi(x')| = \left| \int_E e^{i\langle x, x' \rangle} d\mu(x) \right| \leq \int_E |e^{i\langle x, x' \rangle}| d\mu(x) = \int_E d\mu(x) = \Phi(0),
$$

よって (53)。さらに、$a$ と $b$ が実数である場合、

$$
|e^{ia} - e^{ib}|^2 = |e^{ib}|^2|e^{i(a-b)} - 1|^2 = (e^{i(a-b)} - 1)(e^{-i(a-b)} - 1) = 2 - 2\cos(a - b);
$$

Cauchy–Schwarz 不等式により、次のようになります。

$$
|\Phi(x') - \Phi(y')|^2 = \left| \int_E (e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}) d\mu(x) \right|^2
$$
$$
\leq \int_E |e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}|^2 d\mu(x) \int_E 1^2 d\mu(x)
$$
$$
= \int_E (2 - 2\cos\langle x, x' - y' \rangle)) d\mu(x) \cdot \Phi(0)
$$
$$
= 2\Phi(0)\left(\Phi(0) - \Re \Phi(x' - y')\right),
$$

よって (54)。

#### 系 {#int-ix-s6-n8-cor-1 .statement tag=09SQ}

— $E'$ に、ベクトル空間構造と互換性のある位相を装備します。 $\Phi$ が連続であるためには、その実数部分 $\Re \Phi$ が原点で連続であることが必要かつ十分であり、その場合、$\Phi$ は一様連続になります。

これは不等式 (54) から続きます。

F を局所凸型空間とします。 Fのデュアル$F'$にはFと$F'$のデュアルと互換性のある位相を装備し、同一視するFには$F'$のデュアルを装備します。従って、$F'$ 上の有界測定値 $\mu$ のフーリエ変換は、次のように定義される F では写像 $\mathscr{F}\mu$ になります。

$$
(\mathscr{F}\mu)(x) = \int_{F'} e^{i\langle x, x' \rangle} d\mu(x').
$$

#### 命題 9 {#int-ix-s6-prop-9 .statement tag=09SR}

— *F がバレル化されている場合、F' 上のすべての制限されたメジャーのフーリエ変換は、F* 上で均一に連続する写像になります。

$\mu$ を $F'$ と $\Phi$ のフーリエ変換の有界測度とする。 $\varepsilon > 0$ にしましょう。 $\mu(F' - K) \leq \varepsilon$ となるような $F'$ のコンパクト部分集合 K が存在します。さて、K は弱い位相 $\sigma(F', F)$ に対してコンパクトであるため、F がバレル化されているため等連続です (TVS、III, §4, No. 2、Th. 1)。従って、極が $U^\circ$ 含む K である F に 0 の対称近傍 U が存在します。x を $\varepsilon U$ に置くとします。それから

$$
\Phi(0) - \Re \Phi(x) = \int_{F'} (1 - \cos \langle x, x' \rangle) d\mu(x').
$$

さて、$x' \in F' - K$ごとに$0 \leq 1 - \cos \langle x, x' \rangle \leq 2$、そして

$$
1 - \cos \langle x, x' \rangle \leq \frac{1}{2} \langle x, x' \rangle^2 \leq \frac{\varepsilon^2}{2}
$$

$x' \in K \subset U^\circ$の場合。それは次のとおりです

$$
0 \leq \Phi(0) - \Re \Phi(x) \leq 2 \mu(F' - K) + \frac{\varepsilon^2}{2} \mu(K) \leq 2\varepsilon + \frac{\varepsilon^2}{2} \mu(F').
$$

この不等式の 2 番目のメンバーは、$\varepsilon$ では 0 になる傾向があります。従って、$\Re \Phi$ は 0 で連続し、命題は Cor から続きます。提案8の。

### 9. ミンロス補題

T を有限次元ベクトル空間および $\mu$ を $T'$ の有界メジャーとします。 $T'$ の双対で同一視する T を実行し、$\mu$ のフーリエ変換 $\Phi$ が T 上で写像になるようにします。T と数 $\varepsilon > 0$ に 2 つの正の二次方程式形 h と q が与えられたと仮定します。すべての実数 $r > 0$ について、すべての $x \in T$ に対して $\langle x, x' \rangle^2 \leq r^2 h(x)$ となるように、$x' \in T'$ の $C_r$ 集合で表します。

#### 命題 10 {#int-ix-s6-prop-10 .statement tag=09SS}

— *仮定 $\Phi(0) - \Re \Phi \leq \varepsilon + q$ の下では、*

$$
\mu(T' - C_r) \leq 3 (\varepsilon + r^{-2} \operatorname{Tr}(q/h))
$$

*すべて* $r > 0$。

h に関する q のトレースを $\operatorname{Tr}(q/h)$ と書きます (cf. Annex、No. 1)。 $\operatorname{Tr}(q/h)$ が無限大の場合、公式 (55) は自明です。今後、$\operatorname{Tr}(q/h)$ は有限であると仮定します。従って、$h(x) = 0$ は $x \in T$ に対して $q(x) = 0$ を意味します。

$a_1, \ldots, a_n$ を $T$ の元、および $x' \in T'$ の $D$ 集合として、$\sum_{j=1}^n \langle a_j, x' \rangle^2 > 1$ とします。実数 $t \geq 0$ ごとに $3(1 - e^{-t/2}) \geq 0$ があり、さらに

$$
3(1 - e^{-t/2}) \geq 3(1 - e^{-1/2}) \geq 3\left(1 - \left(\frac{9}{4}\right)^{-1/2}\right) = 1
$$

$t > 1$の場合、$e > \frac{9}{4}$のため。 適用これらの不等式を $t = \sum_{j=1}^n \langle a_j, x' \rangle^2$ にすると、次のようになります。

$$
\mu(D) \leq 3 \int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x').
$$

ルベーグ測度に関して稠密度 $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$ を持つ $\mathbf{R}$ の測度を $\gamma$ とします。 補題 2/No. 4 までに、

$$
\int_{\mathbf{R}} e^{iut} d\gamma(t) = e^{-u^2/2}
$$

すべて本物の $u$ です。その結果、

$$
\begin{align*}
1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right) \\
&= \int \cdots \int \left(1 - e^{i \sum_{j=1}^n \langle a_j, x' \rangle t_j}\right) d\gamma(t_1) \cdots d\gamma(t_n)
\end{align*}
$$

$x' \in T'$の皆さんへ。 2 番目のメンバーに統合される $x', t_1, \ldots, t_n$ の写像は連続であり、絶対値値よりも 2 だけ上に制限されており、メジャー $\mu$ と $\gamma$ は制限されています。従って、(57) の 2 つのメンバーを $d\mu(x')$ に関して統合し、$\mu$ と $\gamma$ に関して統合を交換することができます。人は得る

$$
\begin{align*}
\int_{T'} \left(1 - \exp \left(-\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2\right)\right) d\mu(x') \\
&= \int \cdots \int \left(\Phi(0) - \Phi\left(\sum_{j=1}^n t_j a_j\right)\right) d\gamma(t_1) \cdots d\gamma(t_n).
\end{align*}
$$

$q$ は $T$ 上の二次関数形であるため、次のような実数 $q_{jk}$ が存在します。
$$
q \left( \sum_{j=1}^n t_j a_j \right) = \sum_{j,k} q_{jk} t_j t_k
$$
$t_1, \ldots, t_n$ 実質。特に、$1 \leq j \leq n$の$q_{jj} = q(a_j)$。さらに、積分$\int_{\mathbf{R}} t^n d\gamma(t)$ は、$n = 0, 1, 2$ に対してそれぞれ値 1、0、1 になります (No. 4、補題 1)。このことから、すぐに推測できるのは、
$$
\int \cdots \int \left( \varepsilon + q \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n) = \varepsilon + \sum_{j=1}^n q(a_j).
$$
さて、(58) と $\Phi(0)$ の最初のメンバーは実数です。従って、(58) の 2 番目のメンバーの $\Re \Phi$ によって置き換える $\Phi$ が可能です。 不等式 $\Phi(0) - \Re \Phi \leq \varepsilon + q$ および公式 (56)、(58)、および (59) は、次のことを意味します。
$$
\mu(D) \leq 3 \left( \varepsilon + \sum_{j=1}^n q(a_j) \right).
$$
数 $r > 0$ を修正しましょう。二次方程式形 $h$ は正なので、0 と $n$ の間に $T$ と整数 $m$ の基底 $(e_1, \ldots, e_n)$ が存在します。
$$
h \left( \sum_{j=1}^n t_j e_j \right) = \sum_{j=1}^m t_j^2
$$
$t_1, \ldots, t_n$ 実数 (附属書、No. 1、提案 2)。従って、$C_r$ は次のような $x' \in T'$ で構成され、明らかになります。
$$
\sum_{j=1}^m \langle e_j, x' \rangle^2 \leq r^2, \qquad \sum_{j=m+1}^n \langle e_j, x' \rangle^2 = 0.
$$
すべての整数 $l \geq 1$ について、$D_l$ を $x' \in T'$ 満たす不等式の集合とします
$$
\sum_{j=1}^m \langle r^{-1} e_j, x' \rangle^2 + \sum_{j=m+1}^n \langle l e_j, x' \rangle^2 > 1.
$$
数列 $(D_l)_{l \geq 1}$ が増加すると和集合 $T' - C_r$、よってであることが簡単にわかります。
$$
\mu(T' - C_r) = \lim_{l \to \infty} \mu(D_l).
$$

しかし、(60)までに、

$$
\mu(D_l) \leq 3 \left( \varepsilon + \sum_{j=1}^m r^{-2} q(e_j) + \sum_{j=m+1}^n l^2 q(e_j) \right);
$$

$j = m+1, \ldots, n$ には $h(e_j) = 0$ があるため、$q(e_j) = 0$ になります。さらに、$\operatorname{Tr}(q/h) = \sum_{j=1}^m q(e_j)$（附属書、No. 1、提案2）。 関係 (55) は (61) と (62) から続きます。

Q.E.D.

### 10. 核の二重性への対策空間

F を局所凸空間とします。 $\mathscr{T}_s$ を、$F'$ 上の弱い位相 $\sigma(F', F)$ と、F のコンパクトな凸面部分集合上の一様収束の$\mathscr{T}_c$ 位相とします。Mackey の定理 (TVS、IV, §1, No. 1、Th. 1) により、 $F'$ のトポロジー $\mathscr{T}_s$ と $\mathscr{T}_c$ は、F と $F'$ の間の二重性と互換性があります。したがって、同じことが、$\mathscr{T}_s$ と $\mathscr{T}_c$ の中間の $F'$ にあるすべての局所的に凸な位相 $\mathscr{T}$ にも当てはまります。 $\mathscr{T}$が位相で、$F'_{\mathscr{T}}$が$\mathscr{T}$を備えた空間$F'$を表す場合、$F'_{\mathscr{T}}$の双数で同一視するFとします。したがって、$F'$ の手法は、前の型のすべてのトポロジ $\mathscr{T}$ で同じであり、$\mu$ がそのような手法である場合、そのフーリエ変換は F 上の写像になります。

F 上のサゾノフの位相を、連続セミノルム N 満たすによって定義される局所凸位相 $\mathscr{S}$ と呼びます。次の条件: $N^2$ は F 上の正の二次方程式形であり、次のような F 上に連続正の二次方程式形 H が存在します。 $\operatorname{Tr}(N^2/H) < +\infty$。 位相 $\mathscr{S}$ は、F で指定された位相より粗いです。これらのトポロジーが同一である場合、F は核であると言われます。この空間の類については、後で詳しく検討します。

#### 定理 2 (ミンロス) {#int-ix-s6-thm-2 .statement tag=09ST}

— *F を局所凸空間、$\mathscr{T}$ を $\mathscr{T}_s$ と $\mathscr{T}_c$ の中間の $F'$ に局所凸位相、$\mu$ を $F'_{\mathscr{T}}$ のプロメジャーとします。 $\mu$ のフーリエ変換 $\Phi$ がサゾノフ位相に対して F 上で連続であると仮定します。すると、$\mu$ は $F'_{\mathscr{T}}$ の小節になります。*

$\varepsilon > 0$ にしましょう。 Since $\Phi$ is continuous for the Sazonov topology on F, there exist two continuous positive quadratic forms Q and H on F such that $\operatorname{Tr}(Q/H) < +\infty$ and

$$
\Phi(0) - \mathscr{R}\Phi(x) \leq \varepsilon/6
$$

$Q(x) \leq 1$ などのすべての $x \in F$ に対して。 No. 8、$|\mathscr{R}\Phi(x)| \leq \Phi(0)$ の提案 8 による、すべての $x \in F$、よって

$$
\Phi(0) - \mathscr{R}\Phi(x) \leq \varepsilon/6 + 2\Phi(0)Q(x)
$$

すべての$x \in F$に。

集合 $r = (12\Phi(0)\operatorname{Tr}(Q/H)\varepsilon^{-1})^{1/2}$ を表し、すべての $x \in F$ に対して $\langle x, x' \rangle^2 \leq r^2 H(x)$ となるように $x' \in F'_\mathscr{T}$ の K 集合で表します。 $H^{1/2}$ は $F$ 上で連続半ノルムであるため、集合 K は等連続であり、$F'_\mathscr{T}$ で閉じられます。したがって、Ascoli の定理 (GT、X, §2, No. 5、Th. 2 の Cor. 1) による $F'_\mathscr{T}$ でコンパクトです。

V を $F'_\mathscr{T}$ と有限余次元の閉じた線形部分空間とします。このとき、V は F の有限次元線形部分空間 T の直交関数です。 $\mu_V$ を $T'$ の小節、つまり写像 $p_V$ の下の $F'_\mathscr{T}$ のプロメジャー $\mu$ の像、つまり T から F への標準単射の転置とします。そのフーリエ変換は、T に対する $\Phi$ の制限です。 最後に、ハーン・バナハ定理 (TVS、II, §3, No. 2、Th. 1 の Cor. 1) によれば、$p_V(K)$ は、すべての $x \in T$ に対して $\langle x, x' \rangle^2 \leq r^2 H(x)$ となるように、$x' \in T'$ の集合 $C_r$ に等しくなります。 不等式 (63) により、$2\Phi(0)Q$ の q 制限を T に、そして h を H に当てはめて、No. 9 の提案 10 を $T'$ の尺度 $\mu_V$ に適用できます。 次に、$\operatorname{Tr}(q/h) \leq 2\Phi(0)\operatorname{Tr}Q/H)$、よって

$$
\mu_V(T' - C_r) \leq 3 \left( \frac{\varepsilon}{6} + 2\Phi(0)\operatorname{Tr}(Q/H)\,r^{-2} \right) = \varepsilon.
$$

$p_V$ 定義するから、$F'_\mathscr{T}/V$ の商、同型から $T'$ への通過により、No. 1 の提案 1 は、$\mu$ が $F'_\mathscr{T}$ に関するメジャーであることを示します。

Q.E.D.

#### 系 {#int-ix-s6-n10-cor-1 .statement tag=09SU}

— *F をバレル核空間、$\mathscr{T}$ を $\mathscr{T}_s$ と $\mathscr{T}_c$ の中間$F'$ に局所凸位相、$\mu$ を $F'_\mathscr{T}$ のプロメジャー、$\Phi$ をフーリエ変換とします。 $\mu$。 $\mu$ がメジャーであるためには、$\Phi$ が F 上で連続していることが必要かつ十分です。*

必要性は No. 8 の提案 9 から、十分性は Th から得られます。 2.

#### 注意 {#int-ix-s6-n10-rem-1 .statement tag=09SV}

— F をバレル型の空間と、$\mathscr{T}$ を $\mathscr{T}_s$ と $\mathscr{T}_c$ の中間の $F'$ 上に局所的に凸型の位相とします。 $\mathscr{T}$ のコンパクトな $F'$ のすべての部分集合は、より粗い位相 $\mathscr{T}_s$ のコンパクトです。逆に、K を $\mathscr{T}_s$ に対してコンパクトな $F'$ の部分集合とする。 F はバレル化されているため、K は等連続です (TVS、III, §4, No. 2、Th. 1)。しかし、アスコリの定理によれば、$F'$の等連続部分集合は$\mathscr{T}_c$では比較的コンパクトであり、*なおさら*は$\mathscr{T}$では比較的コンパクトなので、Kは$\mathscr{T}$でコンパクトな$F'$の部分集合に含まれます。このことから、これら 2 つの空間に関する措置の集合の間に、$F'_\mathscr{T}$ の恒等写像が $F'_{\mathscr{T}_s}$ 定義する全単射に及ぶことを推測するのは難しくありません。

### 11. ヒルベルトの測定空間

E を実ヒルベルト空間とし、スカラー 積を $(x|y)$ で表します。その双対 $E'$ 上には E の同型 j が存在し、E の $x, y$ に対する公式 $\langle x, j(y) \rangle = (x|y)$ によって特徴付けられます (TVS、V, §1, No. 7、Th. 3)。 j を使って同一視する E と $E'$ を実行します。したがって、E 上のプロメジャー $\mu$ のフーリエ変換は、E では写像 $\mathscr{F}\mu$ です。 $\mu$ がメジャーの場合、

$$(64)$$
$$(\mathscr{F}\mu)(x) = \int_{E} e^{i(x|y)} d\mu(y) \quad (x \in E).$$

#### 定理 3 (プロホロフ – サゾノフ) {#int-ix-s6-thm-3 .statement tag=09SW}

※Eをヒルベルト空間、弱体化位相を装備したEs空間Eとする。 μ を E のプロメジャー、Φ をそのフーリエ変換とします。次の条件は同等です*:

a) *写像 Φ は Sazonov 位相* の E 上で連続です。

b) *すべての ε > 0 に対して、Φ(0) − $\Re \Phi$ ≤ ε + Q* となるような E 上の核正の二次方程式形 Q が存在します。

c) *promeasure μ は Es* の尺度です。

$b) \Rightarrow a)$: これは、No. 8 の提案 8 (cf. 不等式 (54)) に続きます。

$a) \Rightarrow c)$: これは、No. 10 の定理 2 から続きます。

$c) \Rightarrow b)$: μ が Es に関する尺度であると仮定します。 ε > 0 とします。ノルム $\leq n$ を含む$x \in E$ のすべての整数 $n \geq 1$、集合 $B_n$ について、$E_s$ および $E = \bigcup_{n \geq 1} B_n$ の閉じた部分集合です。したがって、$\mu(E - B_n) < \frac{\varepsilon}{2}$ となるような整数 $n \geq 1$ が存在します。 公式

$$(65)$$
$$ Q(x) = \frac{1}{2} \int_{B_n} (x|y)^2 d\mu(y) $$

定義する正の二次方程式形 E 上の Q。 集合 $C = \frac{n^2}{2} \mu(B_n)$。 $(e_1, \ldots, e_p)$ が E の有限正規直交関数数列である場合、

$$
\sum_{j=1}^p (e_j|y)^2 \leq \|y\|^2 \leq n^2
$$

$y \in B_n$ごとにベッセルの不等式。統合すると、次のようになります。

$$
\sum_{j=1}^p Q(e_j) = \frac{1}{2} \int_{B_n} \sum_{j=1}^p (e_j|y)^2 d\mu(y) \leq \frac{n^2}{2} \mu(B_n) = C,
$$

したがって、Q は核です。

さらに、実数 t ごとに $1 - \cos t \leq \inf \left( 2, \frac{t^2}{2} \right)$、よって

$$
\Phi(0) - \Re \Phi(x) = \int_{E} (1 - \cos(x|y)) d\mu(y)
$$
$$
\leq \int_{B_n} \frac{1}{2}(x|y)^2 d\mu(y) + \int_{E - B_n} 2 \cdot d\mu(y)
$$
$$
< Q(x) + \varepsilon
$$

$x \in E$の皆さんへ。したがって、b) が検証されます。

Q.E.D.

#### 系 1 {#int-ix-s6-thm-2-cor-1 .statement tag=09SX}

— *$E_1$と$E_2$を2つのヒルベルト空間、$u$を$E_1$の$E_2$へのヒルベルト・シュミット写像、$\mu$を$E_1$のプロメジャーとする。 $\mu$ のフーリエ変換 $\Phi$ が $E_1$ で連続すると仮定します。すると、$\nu = u(\mu)$ という対策は、弱い位相を装備した $E_2$ の対策になります。

この番号で紹介された$E_1$ と $E_2$ の双対を使用すると、$\nu$ のフーリエ変換は $\Phi \circ u^*$ に等しくなります。ここで、$u^*$ は $u$ の随伴です。さて、$u^*$ は、$E_2$ から $E_1$ (付録、No. 2) へのヒルベルト・シュミット写像であり、したがって、$E_2$ 上の二次方程式形 $y \mapsto \|u^*(y)\|^2$ は核です。 $(E_2)_\mathscr{S}$ がサゾノフ位相を装備した $E_2$ を表す場合、$u^*$ は$(E_2)_\mathscr{S}$ から $E_1$ への連続した線形写像であり、$\mathscr{F}_V = \Phi \circ u^*$ は$(E_2)_\mathscr{S}$ で連続したものになります。 定理 3 は、$\nu$ が弱い位相を備えた空間 $E_2$ のメジャーであることを示します。

#### 系 2 {#int-ix-s6-thm-2-cor-2 .statement tag=09SY}

— *$Q$ をヒルベルト空間 $E$ 上の核正の二次方程式形とします。分散 $Q$ を伴う $E$ 上のガウス プロメジャー $\Gamma_Q$ は、$E_s$ 上のメジャーです。*

$\Gamma_Q$ のフーリエ変換 $\Phi$ は $e^{-Q/2}$ に等しい。さて、実数 $t$、よって $\Phi(0) - \Re \Phi \leq Q/2$ ごとに $e^t \geq 1 + t$ です。従って、定理 3 の条件 b) が検証され、$\Gamma_Q$ は $E_s$ に関する対策になります。

#### 注意 {#int-ix-s6-n11-rem-1 .statement tag=09SZ}

— 1) $E$ をヒルベルト空間、$E_s$ 空間 $E$ に弱い位相を装備し、$E$ の $j$ 恒等写像を$E_s$ にするとします。 $E$ の手順の $j$ 定義する全単射の集合が $E_s$ の対応する集合に続くことはわかります。 Moreover, if $E$ is separable, it is a Polish space and $j$ defines a bijection of the set of bounded measures on $E$ onto the set of bounded measures on $E_s$ (§ 3, No. 3, *Remark*); it can be shown (the theorem of Phillips) that this theorem still holds if $E$ is not separable. 従って、定理 3 は、$E$ のプロメジャーがメジャーであるための基準を提供します。

2) ヒルベルト空間 $E$ 上のサゾノフ位相が型 $Q^{1/2}$ の半ノルムによって定義されることを示すことができます (付録、Exer. 7)。ここで、$Q$ は $E$ 上の *核* 正の 2 次式形です。

※12． 関係と写像のポジティブ型*

#### 定義 3 {#int-ix-s6-def-3 .statement tag=09T0}

— *$G$を群とします。 $G$ 上の複素数値写像 $\Phi$ は、不等式* の場合、正の型であると言われます。

$$
\sum_{j,k=1}^p c_j \overline{c_k} \Phi(x_j x_k^{-1}) \geq 0
$$

*任意の* $x_1, \ldots, x_p$ *in* $G$ *および任意の複素数* $c_1, \ldots, c_p$ に当てはまります。

この概念については、後で詳しく説明します。

#### 命題 11 {#int-ix-s6-prop-11 .statement tag=09T1}

— Eを有限次元ベクトル空間、$\mu$をEの有界(正の)測度、$\Phi$を$\mu$のフーリエ変換とする。 写像 $\Phi$ は連続で、$E'$ で正の型です。

$\Phi$ の連続性は、No. 8 の提案 9 から得られます。

$\Phi$ が正の型であることを示しましょう。 $x'_1, \ldots, x'_p$ を $E'$ と $c_1, \ldots, c_p$ 複素数に入れます。それから

$$
\sum_{j,k} c_j \overline{c_k} \Phi(x'_j - x'_k) = \int_E \sum_{j,k} c_j \overline{c_k} e^{i \langle x, x'_j - x'_k \rangle} \, d\mu(x)
$$
$$
= \int_E \left| \sum_{j=1}^p c_j e^{i \langle x, x'_j \rangle} \right|^2 \, d\mu(x) \geq 0.
$$

Q.E.D.

*ボフナーの定理* として知られる 1 つの証明できる逆: 正の型の $E'$ 上のすべての連続写像は、有界 (正) 測度のフーリエ変換です。 (*) 残りのNo. 12ではこの結果を仮定します。

#### 定理 4 {#int-ix-s6-thm-4 .statement tag=09T2}

— E を局所凸空間とします。 The Fourier transformation is a bijection of the set of promeasures on E onto the set of functions of positive type on $E'$ whose restriction to every finite-dimensional subspace is continuous.

フーリエ変換が単射であることはわかっています (No. 3、提案 3)。 $\mu = (\mu_V)_{V \in \mathscr{F}(E)}$ を E のプロメジャーとし、$\Phi$ をそのフーリエ変換とします。 T を $E'$ の有限次元部分空間とし、E における T の直交を V とします。$E/V$ の双対を持つ 1 つの同一視できる T。 T に対する $\Phi$ の制限 $\Phi_T$ は、$E/V$ 上の有界測定値 $\mu_V$ のフーリエ変換です。提案 11 により、$\Phi_T$ は連続であり、T に対して正の型です。T は任意であるため、$\Phi$ は $E'$ に対して正の型であることは明らかです。

逆に、$\Phi$ を $E'$ のすべての有限次元部分空間に対する制限が連続である $E'$ 上の正の型の写像とします。すべての $V \in \mathscr{F}(E)$ について、$E'$ の V の直交 $V^\circ$ と $E/V$ の双対を同一視する計算します。 $\Phi$ から $V^\circ$ の制限 $\Phi_V$ は連続で正の型であるため、ボホナーの定理により、$E/V$ に有界（正の）測度 $\mu_V$ が存在し、そのフーリエ変換は次のようになります。 $\Phi_V$。 $\mathscr{F}(E)$ の V と W が $W \subset V$ になるようにし、$p_{VW}$ を $E/W$ の $E/V$ 上の標準写像とします。識別が行われた場合、${}^t p_{VW}$ は $V^\circ$ の単射から $W^\circ$ になります。 No. 3 の公式 (4) までに、

$$
\mathscr{F}(p_{VW}(\mu_W)) = (\mathscr{F}\mu_W) \circ {}^t p_{VW} = \Phi_W \circ {}^t p_{VW} = \Phi_V = \mathscr{F}\mu_V,
$$

(*) この問題は、書籍 *理論スペクトル* の今後の章で研究される予定です。この主題については、読者は L.H の本を参照してください。 LOOMIS、*抽象高調波解析*、ヴァン ノストランド、ニューヨーク、1953 年。

よって $pvw(\mu_w) = \mu_v$ No. 3 の提案 3 により。従って、家族 $\mu = (\mu_v)_{v \in \mathscr{F}(E)}$ は $E$ の予定です。 $\Phi$ が $\mu$ のフーリエ変換であることは明らかです。

#### 系 {#int-ix-s6-n11-cor-1 .statement tag=09T3}

— *F をバレル付き核空間とします。 F' に、F のコンパクト凸部分集合上に一様収束の弱い位相 $\sigma(F', F)$ と位相の局所凸位相 $\mathscr{T}$ を装備します。フーリエ変換は、有界 (正) 測度の集合の全単射です。 F' で、F のポジティブ型の連続写像の集合に。

これは、定理 4 と Cor. Thの。 No. 10 の 2 つ。*

### 練習問題 {#int-ix-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
