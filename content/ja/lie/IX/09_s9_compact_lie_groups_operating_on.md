---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 9
section_title: Compact Lie groups operating on manifolds
lang: ja
source: lie-vii-ix
book_pages: 369-381, 419-424
pdf_pages: 0376-0388, 0426-0431
extraction: native
subsections:
    - "no": 1
      title: EMBEDDING OF A MANIFOLD IN THE NEIGHBOURHOOD OF A COMPACT SET
      page: 369
      pdf_page: 376
    - "no": 2
      title: EQUIVARIANT EMBEDDING THEOREM
      page: 373
      pdf_page: 380
    - "no": 3
      title: TUBES AND TRANSVERSALS
      page: 375
      pdf_page: 382
    - "no": 4
      title: ORBIT TYPES
      page: 377
      pdf_page: 384
statements: 19
exercises: 21
errata:
    - says: §5, no. 2, Cor. of Prop. 2
      read: §5, no. 2, Cor. 1 of Prop. 2
      why: No. 2 of section 5 prints three numbered corollaries of Proposition 2 and the reference does not say which. The sentence citing it has G simply-connected and A an alcove, and says that the composite map from A to $G_r/$Int(G) is a homeomorphism. That is Corollary 1 b), whose homeomorphisms run $A/H_A$ to $T_r/W$ to $G_r/$Int(G) and whose $H_A$ is trivial for a simply-connected group. Corollary 2 is the same statement for the Lie algebra, over a chamber rather than an alcove, and Corollary 3 is about existence and uniqueness and names no map at all.
content_sha256: 3908b3f8b5dae25a04fac5cdb6b16deae664224c255688f1840985863d91ecda
translated_from: content/en/lie/IX/09_s9_compact_lie_groups_operating_on.md
translation_method: google
source_content_sha256: dbd6a8fe77e36a2dde3d4d956d5fc6fd2a6bf284a5e6f34dca83531dabcebd7f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 251288a4fd5fc497b07a44e82cb555d62358d6b7701d69319ae42dffd1381d9c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 9。 コンパクト・リー群多様体に運行

この段落では、X は、類 $C^r(1\leq r\leq \omega )$ の分離された、局所的に有限次元の実数多様体を表します。

### 1. コンパクト集合の近傍に多様体を埋め込む

#### 補題 1 {#lie-ix-s9-lem-1 .statement tag=01HE}

T と $T'$ を 2 つのトポロジー 空間とし、A と $A'$ をそれぞれ T と $T'$ の部分集合をコンパクトにし、$T\times T'$ の $A\times A'$ の W 近傍とします。 T の A のオープン近傍 U と、$U\times U'\subset W$ となる $T'$ の $A'$ のオープン近傍 $U'$ が存在します。

$x\in A$ にしましょう。 T のオープン部分集合 $U_x$ と $T'$ の $U'_x$ が存在し、$\{x\} \times A'\subset U_x\times U'_x\subset W:$ 確かに、$T\times T'$ のコンパクト部分集合 $\{x\} \times A'$ は、以下に含まれるオープン集合の有限数でカバーできます。 W、形 $U_i\times U'_i$、$x\in U_i$ と。 $U_x=\bigcap_iU_i$と$U'_x=\bigcup_iU'_i$を取るだけで十分です。

A はコンパクトなので、$A\subset \bigcup_iU_{x_i}$ となるような A の点 $x_1, . . . , x_m$ が存在します。 $U =\bigcup_iU_{x_i}$と$U'=\bigcap_iU'_{x_i}$を入れます。すると$A\times A'\subset U\times U'\subset W$、したがって補題になります。

この数の残りで、Y は類 $C^r$ の分離された多様体を示します。

#### 命題 1 {#lie-ix-s9-prop-1 .statement tag=01HF}

$\varphi : X\rightarrow Y$ を類 $C^r$ の射とし、A を X の圧縮部分集合とします。次の条件は同等です。

(i) A に対する $\varphi$ の制限は単射であり、$\varphi$ は A の点ごとの浸漬です。

(ii) Y への U の埋め込み $\varphi$ 誘導するとなるような、A のオープン近傍 U が存在します。

これら条件が満たされるとき、$\varphi$はAの近傍への埋め込みであると言われます。

(i) が (ii) を意味し、他の意味が明らかであることを証明します。 (i) を仮定すると、$\varphi$ から V の制限が浸漬であるような、X 含む A のオープン近傍 V が存在します (Differentiable and Analytic 多様体、Results、5.7.1)。 $V\times V$ の点 $(x, y)$ の $\Gamma$ 集合を $\varphi (x) =\varphi (y)$ のように表し、$V\times V$ の対角線を $\Delta$ で表します。すると、$\Delta$ は $\Gamma :$ のオープン部分集合で、実際、すべての $x\in V$ に対して、$\varphi$ から $U_x$ の制限が単射となるように、$x$ のオープン近傍 $U_x$ が存在します。つまり、$\Gamma \cap (U_x\times U_x) =$ $\Delta \cap (U_x\times U_x)$ になります。

Y が分離されているため、$\Gamma$ は $V\times V$ で閉じられます。その結果、$V\times V$ の $\Gamma$ **--** $\Delta$ の補数 W がオープンになります。 仮定、W 含む $A\times A$ 著。 補題 1 は、$U'\times U'\subset W$ となるような、V 含むの開いた部分集合 $U'$ が存在することを意味します。つまり、$\varphi$ から $U'$ の制限が単射であるようなものです。さらに、A の開いた近傍 U が存在し、その閉包はコンパクトで、$U'($General 位相、Chap. 10 に含まれています。 I, §9, no. 7、提案 10)。次に、$\varphi$ 誘導する U から $\varphi$(U) への同型写像、従って U から $\varphi (U)$ への同型写像。 U への $\varphi$ の制限は埋め込みであるということになります (Differentiable and Analytic 多様体、結果、5.8.3)。

#### 命題 2 {#lie-ix-s9-prop-2 .statement tag=01HG}

多様体 Y がパラコンパクトであると仮定します。 A を X の部分集合とし、$\varphi :X\rightarrow Y$ を類 $C^r$ の射とし、誘導する A から $\varphi (A)$ までの同相写像とし、それは A の点ごとにエタールであるとします。 U から Y の開部分多様体まで $\varphi$ 誘導する同型となるような A の近傍 U。

必要に応じて X と Y を制限すると、$\varphi$ はエタールかつ全射であると仮定できます。 $\varphi |A$ の逆同型写像を $\sigma :\varphi (A)\rightarrow A$ で表します。 Y は計化可能であるため (微分可能と解析多様体、結果、5.1.6)、$\varphi (A)$ はパラコンパクト近傍の基本的な系を認めます。従って、将軍位相、第2章によって。 XI、Y には $\varphi (A)$ の開いた近傍 V と、$\varphi (A)$ に $\sigma$ が付いている一致するという連続写像 $s: V\rightarrow X$ が存在し、すべての $y\in V$ に対して $\varphi (s(y)) =y$ となるようなものです。さらに、$s$ はトポロジー的にエタールであるため、$s(V)$ は開いた集合 U 含む A です。すると、$\varphi$ 誘導するは U から V までの同相写像 $\varphi '$ です。微分可能および分析多様体によると、結果$, 5.7.8,\varphi '$ は同型です。

この数の残りの部分では、$r\not=\omega$ と仮定します。

#### 命題 3 {#lie-ix-s9-prop-3 .statement tag=01HH}

A を X のコンパクト部分集合とする。 A の近傍に埋め込まれている射 $\varphi \in \mathscr{C}^r(X;Y)$ の集合 $\mathscr{P}$ は、コンパクト $C^r$-収束 (§ 6, no. 4) の位相の $\mathscr{C}^r(X;Y)$ で開かれています。

明らかに、$r= 1$ に対して命題を証明するだけで十分です。

a) まず、A の点ごとの浸漬である $\mathscr{C}^1(X;Y)$ からなるの射の部分集合 J が開いていることを示します。 写像 $j_A:\mathscr{C}^1(X;Y)\times A\rightarrow J^1(X;Y)$ が $j_A(\varphi , x) =j_x^1(\varphi ) ($ 微分可能かつ解析的多様体、結果、12.1) となるように考えてください。

$\mathscr{C}^1$(X;Y)の位相の定義までに、$\mathscr{C}^1(X;Y)$から$\mathscr{C}(A;J^1(X;Y))$までの写像$\widetilde{j}_A:\varphi \rightarrow j_A(\varphi , .)$は連続です。これは、一般位相、第 4 章から続きます。 X, §3, no. 4、木。 3、その$j_A$は連続です。

一方、M を $J^1(X;Y)$ のジェット $j$ の集合とし、その接線写像 $T(j) : T_{\mathbf{s}(j)}(X)\rightarrow T_{\mathbf{b}(j)}(Y) ($ 微分可能かつ解析的多様体、結果、12.3.4) が単射であるとします。 集合Mは$J^1(X;Y)$にオープンしています。実際、X が有限次元ベクトル空間 E の開部分集合であり、Y がバナッハ空間 F の開部分集合である場合、この主張を検証するだけで十分です。次に、単射連続線形写像の集合が $\mathscr{L}$(E;F) で開いているという証明に還元されます (微分可能と解析多様体、結果、12.3.1)。これは、スペクトル理論、第 3 章から続きます。 III, §2, no. 7、提案 16。

前述のことから、結論する集合 $j_A^{-1}(M)$ は $\mathscr{C}^1(X;Y)\times A$ で開いているため、その補数 $\mathscr{F}$ は閉じています。 A はコンパクトなので、射影 pr$_1:\mathscr{C}^1(X;Y)\times A\rightarrow \mathscr{C}^1(X;Y)$ は適切な射であり、したがって閉じられます。従って、$\mathscr{C}^1(X;Y)$ **--** pr$_1(\mathscr{F})$ に等しい集合 J は、$\mathscr{C}^1(X;Y)$ でオープンになります。

b) H を、$f(x) =f(y)$ となるような要素 $(f, x, y)$ から構成される $J\times A\times A$ の部分集合とする。 H 含む $J\times \Delta$ であることは明らかです。ここで、$\Delta$ は積 $A\times A$ の対角線を示します。 $H'= H$ **--** $(J\times \Delta )$ が $J\times A\times A$ に閉じられることがわかります。 $\mathscr{P}$ は、適切な射影 pr$_1: J\times A\times A\rightarrow J$ の下で $H'$ の像の J の補数であるため、これは命題を意味します。

The topology of $\mathscr{C}^1(X;Y)$ being finer than the topology of compact convergence, the map $(\varphi , x) \rightarrow \varphi (x)$ from $\mathscr{C}^1(X;Y)\times A$ to Y is continuous (General Topology, Chap. X, §3, no. 4, Cor. 1 of Th. 3); it follows that H is closed in $J\times A\times A$. Hence, it suffices to show that $J\times \Delta$ is open in H, in other words, that for all $\varphi \in J$ and all $x\in A$ there exists a neighbourhood $\Omega$ of $\varphi$ in J and a neighbourhood B of $x$ in X such that, for any morphism $\psi$ in $\Omega$, the restriction of $\psi$ to $A\cap B$ is injective.

したがって、命題は次の補題から導かれます。

#### 補題 2 {#lie-ix-s9-lem-2 .statement tag=01HI}

$x$ を X$,\varphi : X\rightarrow Y$ 射の類 $C^1$ の点とします。これは、$x$ での浸漬です。 $\mathscr{C}^1(X;Y)$ の $\varphi$ の近傍 $\Omega$ と X の $x$ の近傍 B が存在し、すべての $\psi \in \Omega$ に対して、$\psi$ の制限は単射になります。

U を、有限次元ベクトル空間に同型の $x$ の比較的コンパクトな開いた近傍とし、$\varphi (U)$ がチャートの領域 V に含まれるようにします。 $\psi (U)\subset V$ が $\mathscr{C}^1$(X;Y) で開いており、制限写像 $\Omega_0\rightarrow \mathscr{C}^1(U;V)$ が連続しているような、$\psi \in \mathscr{C}^1(X;Y)$ の集合 $\Omega_0$。したがって、X = U および Y = V の場合、証明補題に還元されますが、他の語では、X は有限次元ベクトル空間で、Y はバナッハ空間であると仮定できます。 X の選ぶノルムと Y.

線形写像 $D\varphi (x) : X\rightarrow$ Y は単射です。その一致を$q($スペクトル理論、第2章で示します。 III, §2, no. 6) なので、定義までに、すべての $t\in X$ に対して $\|D\varphi (x).t\| \geq q\|t\|$ が得られます。 $\varepsilon \in \mathbf{R}$ が $0< \varepsilon  < q/2$ となるようにし、B が中心 $x$ ですべての $u\in B$ に対して $\|D\varphi (u)-D\varphi (x)\| \leq \varepsilon$ となるクローズドボールであるとします。 $\mathscr{C}^1(X;Y)$ からなる射 $\psi$ ですべての $u\in B$ に対して $\|D\psi (u)-D\varphi (u)\| \leq \varepsilon$ となるように、$\Omega$ 部分集合で表します。 $\mathscr{C}^1(X;Y)$の位相の定義までに開いています。 $\psi \in \Omega$には$\psi_0=\psi -D\varphi (x)$を入れてください。 すべての $u\in B$ に対して $\|D\psi_0(u)\| \leq 2\varepsilon$ があり、その結果、B のすべての $u$ と $v$ に対して $\|\psi_0(u)-\psi_0(v)\| \leq 2\varepsilon \|u-v\|$ が得られます (微分可能および解析多様体、結果、2.2.3)。 従って、

$$
\|\psi (u)-\psi (v)\| \geq  \|D\varphi (x).(u-v)\| - \|\psi_0(u)-\psi_0(v)\| \geq (q-2\varepsilon )\|u-v\|
$$

従って、B に対する $\psi$ の制限は単射なので、補題になります。

#### 命題 4 {#lie-ix-s9-prop-4 .statement tag=01HJ}

A を X のコンパクト部分集合とします。 A の近傍の埋め込みである有限次元ベクトル空間 E と射 $\varphi \in \mathscr{C}^r(X;E) (r\not=\omega )$ が存在します。

$(U_i, \varphi_i,E_i)_{i\in I}$ を、定義域が A をカバーする X のチャートの有限族とします。 $x \notin U_i$ に $\varphi_i(x) = 0$ を代入することで、X から $E_i$ まで ($\varphi_i$ でも示されます) 拡大する $\varphi_i$ から写像になります。 $(V_i)_{i\in I}$ を、すべての $i\in I$ に対して $\overline{V}_i\subset U_i$ となるように、X の部分集合を開くことで A のカバーとします (そのようなカバーの存在は、コンパクト空間に適用される、一般位相、IX, §4, no. 3 章、Th. 3 の Cor. 1 に従います) $X'$ は無限遠でX 点に隣接し、開いた集合 $U_i(i\in I)$ と$X'$ **--** A) をカバーする$X'$ からなるによって得られます。すべての $i\in I$ について、$\alpha_i$ を X の類 $C^r$ の数値写像とし、$V_i$ のすべての点で 1 に等しく、$U_i($Differentiable and Analytic に含まれるサポートを使用します。 多様体、結果、5.3.6)。

によって定義された写像 $\varphi : X\rightarrow \bigoplus_{i\in I}(E_i\oplus \mathbf{R})$ を考えてみましょう。

$$
\varphi (x) = (\alpha_i(x)\varphi_i(x), \alpha_i(x))_{i\in I}
$$

すべての $i\in I$ について、写像 $\alpha_i\varphi_i$ は類 $C^r$ であり (その制限から $U_i$ と $\alpha_i$ のサポートの補数であるため)、その制限から $V_i$ は埋め込みです。したがって、$\varphi$ は類 $C^r$ の射であり、A の点ごとに浸漬されます。A に対する $\varphi$ の制限は単射であることがわかります。 $x, y$ を $\varphi (x) =\varphi (y)$ となるような A の 2 つの点とし、$i\in I$ を $x\in V_i$ となるようにします。次に $\alpha_i(x) = 1$ なので $\alpha_i(y) = 1$ となり、これは $y\in U_i$ を意味します。しかし、$\varphi_i(x) =\varphi_i(y)$ もあるので、$\varphi_i$ 誘導するから $U_i$ を $E_i$ に埋め込んだので、$x=y$ になります。

すべての分離された多様体は無限大で可算であることを示すことができます$^9$

純粋な次元 $n$、$\mathbf{R}^{2n}$ に埋め込まれます。弱い結果の場合は、cf. 練習問題 2.

$^9$ H. WHITNEY の「$2n$ 空間における滑らかな$n$ 多様体の自己交差」を参照してください。

アン。 of Math.、45 (1944)、220-246 ページ。

### 2. 等変埋め込み定理

この数では$r\not=\omega$とします。

#### 補題 3 {#lie-ix-s9-lem-3 .statement tag=01HK}

G をトポロジカル空間 X で連続的に動作するコンパクトなトポロジカル群とします。 A を G の下で安定な X の部分集合、A の W 近傍とします。すると、G の下で安定で、$_{\circ}W$ に含まれる A の開いた近傍 V が存在します。

F = X **--** W および V = X**--** GF と置きます。 Then V is open (General Topology, Chap. III, §4, no. 1, Cor. 1 of Prop. 1), stable under G, and $A\subset V\subset W$.

#### 定理 1 {#lie-ix-s9-thm-1 .statement tag=01HL}

G をコンパクトなリー群、$(g, x) \rightarrow gx$ を X 上の G のクラス $C^r$ の左演算の法則、A を X のコンパクトな部分集合とする。 有限次元ベクトル空間 E 上に G の解析的線型表現 $\rho$ が存在し、G の演算と互換性のある類 $C^r$ の射 $\varphi : X\rightarrow E$、および G の下で安定な A の開いた近傍 U が存在します。 Uへの$\varphi$の制限は埋め込みです。

置き換えること A をコンパクトな集合 GA により、A が G の下で安定している場合に帰着します。

$E_0$ を有限次元ベクトル空間とし、A の近傍に埋め込みである $\mathscr{C}^r(X;E_0)$ の要素が存在するようにします (no. 1、提案 4)。この性質を持つ射の集合 $\mathscr{P}$ は、 $\mathscr{C}^r(X;E_0)$ の空でない開いた部分集合です (no. 1、提案 3)。 空間 $\mathscr{C}^r(X;E_0) ($§6, no. 4、補題 4) 上のコンパクト群 G の連続線型表現を考えてみましょう。 Peter-Weyl の定理 (スペクトル理論、準備中) によれば、G のもとで安定な有限次元部分空間の結合は $\mathscr{C}^r(X;E_0)$ で密になります。したがって、$g\in G$ の写像 $x \rightarrow \varphi_0(gx)$ が $\mathscr{C}^r(X;E_0)$ の有限次元ベクトル部分空間 $E_1$ を生成するように、$\mathscr{P}$ の要素 $\varphi_0$ が存在します。これは G の操作下で明らかに安定しています。

E を $E_1$ の作用によって誘導される E 上の G の表現である空間 Hom$_{\mathbf{R}}(E_1,E_0),\rho$ とし、$\varphi : X\rightarrow E$ を $x\in X$ から線形写像 $\psi  \rightarrow \psi (x)$ に関連する写像とします。 $E_1$から$E_0$まで。これは類 $C^r$ の射です。 $x\in X,g\in G,\psi \in E_1$ については、次のようになります ($\tau (g)$ 自己同型 $x \rightarrow gx$ または X で示されます):

$$
\varphi (gx)(\psi )-\psi (gx) =\varphi (x)(\psi \circ \tau (g)) = (\rho (g)\varphi (x))(\psi )
$$

$\alpha :$ Hom$_{\mathbf{R}}(E_1,E_0)\rightarrow E_0$ を線形写像 $u \rightarrow u(\varphi_0)$ とします。 $\alpha \circ \varphi =\varphi_0$ があるため、$\varphi_0$ は 1 であるため、$\varphi$ は A の近傍への埋め込みになります。したがって、U に対する $\varphi$ の制限が埋め込みとなるような A のオープン近傍 U が存在します。 選ぶ U は補題 3 までに G の下で安定するので、定理になります。

#### 系 1 {#lie-ix-s9-thm-1-cor-1 .statement tag=01HM}

X がコンパクトであると仮定します。有限次元ベクトル空間 E 上に G の解析線型表現 $\rho$ と、$g\in G, x\in X$ に対して $\varphi (gx) =\rho (g)\varphi (x)$ となるような埋め込み $\varphi : X\rightarrow E$ が存在します。

#### 系 2 {#lie-ix-s9-thm-1-cor-2 .statement tag=01HN}

H を G の閉じた部分群とします。固定子 H を持つ有限次元ベクトル空間 E および点 $v\in E$ 上に G の解析的線型表現が存在します。

Corを適用します。 1 からコンパクト多様体 $G/H$ の G の標準演算 。これにより、分析線型表現 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ と、$\varphi (gx) =\rho (g)\varphi (x),g\in G, x\in G/H$ のような埋め込み $\varphi : G/H\rightarrow E$ が得られます。 $\overline{e}\in G/H$ を $e\in G$ の類とし、$v=\varphi (\overline{e})$ をその像とします。すべての$g\in G$に対して、$\rho (g)v=v\Leftarrow \Rightarrow \varphi (g\overline{e}) =\varphi (\overline{e})\Leftarrow \Rightarrow g\overline{e}= \overline{e}\Leftarrow \Rightarrow g\in H$があります。

#### 系 3 {#lie-ix-s9-thm-1-cor-3 .statement tag=01HO}

X がパラコンパクトであると仮定します。実ヒルベルト空間 E、G on E の連続ユニタリー 表現 $^{10}\rho$、およびすべての $g\in G$ とすべての $x\in X$ に対して $\varphi (gx) =\rho (g)\varphi (x)$ となるような類 $C^r$ の埋め込み $\varphi : X\rightarrow E$ が存在します。

空間 $X/G$ は局所的にコンパクトです (一般位相、章 III, §4, no. 5、提案 11)。その接続された成分は、Xの接続された成分の像であり、無限に数えることができます（一般位相、第5章I, §9, no. 10、第5章）。したがって、それら自体は無限大で可算であり、これは $X/G$ がパラコンパクトであることを意味します (前述)。したがって、比較的コンパクトなオープン集合による$X/G$の局所的に有限なカバー$(U'_{\alpha})_{\alpha\in I}$と、すべての$\alpha \in I ($一般位相に対して$\overline{V}'_{\alpha}\subset U'_{\alpha}$となるようなカバー$(V'_{\alpha})_{\alpha\in I}$が存在します。 IX, §4, no. 3、コル。 Thの1 3); 逆像を取ると、G の下で安定した比較的コンパクトなオープン集合によって、X の 2 つの局所有限被覆 $(U_{\alpha})_{\alpha\in I}$ と $(V_{\alpha})_{\alpha\in I}$ が得られ、すべての $\alpha \in I$ に対して $\overline{V}_{\alpha}\subset U_{\alpha}$ になります。

すべての $\alpha \in I$ について、有限次元実数ベクトル空間 $E_{\alpha}$ および射 $\varphi_{\alpha}\in \mathscr{C}^r(X;E_{\alpha})$ 上に G の表現 $\rho_{\alpha}$ が存在し、G の演算と互換性があり、制限から $U_{\alpha}$ が埋め込みです(第1弾)。 $\alpha \in I$ について、$a_{\alpha}$ を X の類 $C^r$ の数値写像とし、$V_{\alpha}$ では 1 に等しく、$U_{\alpha}($ 微分可能および解析多様体の外側では 0 に等しくします。結果、5.3.6)。 $x\in X$に$b_{\alpha}(x) =\int_Ga_{\alpha}(gx)dg$を入れます。 写像 $b_{\alpha}$ は類 $C^r$ のもので、G (§6, no. 4、Cor. 2) の下で不変で、$V_{\alpha}$ では 1 に等しく、$U_{\alpha}$ の外では 0 に等しい。それぞれの $E_{\alpha}$ に G (§1, no. 1) の下でのヒルベルト スカラー 積を与え、$\mathbf{R}$ にその標準ヒルベルト構造を与えます。 E を家族 $(E_{\alpha}\oplus \mathbf{R})_{\alpha\in I}$ のヒルベルト和とし、$\rho$ を $\rho_{\alpha}$ と $\mathbf{R}$ の G の自明な作用によって引き起こされる E 上の G の表現とします。 $x\in X$には$\varphi (x) = (b_{\alpha}(x)\varphi_{\alpha}(x), b_{\alpha}(x))_{\alpha\in I}$を入れてください。すると、$\varphi$はXからEまでの類$C^r$の射であり、Gの演算と互換性があります。提案 4 (no. 1) の証明のように、$\varphi$ が埋め込みであることを検証します。これは系を意味します。

$^{10}$それは、演算子 $\rho (g)$ がすべてに対して単一であるような連続線形表現 (スペクトル理論、準備中) (積分、VIII, §2, no. 1 章) です。

$$
g\in G
$$

### 3. チューブとトランスバーサル

#### 補題 4 {#lie-ix-s9-lem-4 .statement tag=01HP}

H をコンパクト・リー群、$\rho : H\rightarrow \mathbf{G}\mathbf{L}(V)$ を有限次元実数ベクトル空間上の H の連続 (したがって解析的) 表現、および V の原点の W 近傍とします。 W に含まれ、H のもとで安定な、原点の開いた近傍 B と、$u(0) = 0$ と $Du(0) =$ Id$_V$ のように、H の演算と互換性のある解析的同型 $u: V\rightarrow B$ が存在します。

選ぶ H (§1, no. 1) の下での不変式V 上のスカラー積。半径 $r$ の開球 B が W に含まれるように実数 $r >0$ が存在します。 H の下では明らかに安定しています。すべての $v\in V$ に $u(v) =r(r^2+\|v\|^2)^{-1/2}v$ を置きます。この場合、$u$ は V から B への全単射解析写像であり、H の演算と互換性があり、その逆写像 $w \rightarrow r(r^2- \|w\|^2)^{-1/2}w$ は解析的です。さらに、$u(0) = 0$と$Du(0) =$Id$_V$。

#### 命題 5 {#lie-ix-s9-prop-5 .statement tag=01HQ}

H をコンパクトなリー群、$(h, x) \rightarrow hx$ を X 上の H のクラス $C^r$ の左演算の法則、$x$ を H の演算の下で固定された X の点とする。 次に、群 H はベクトル空間 $T = T_x(X)$ で線形に動作します。 H の演算と互換性のある、類 $C^r$ のオープン埋め込み $\varphi : T\rightarrow X$ が存在し、$\varphi (0) =x$ と $T_0(\varphi )$ が T の同一性写像になります。

$(U, \psi ,E)$ を $x$ での X のチャートとし、U が H (no. 2、補題 3) の下で安定し、$\psi (x) = 0$ になるようにします。 同一視する E と T を $T_x(\psi )$ で入力し、

$y\in U$ の場合は $\psi^{\sharp}(y) =\int_Hh.\psi (h^{-1}y)dh$、

ここで、$dh$ は総質量 1 の H のハール測度です。

この場合、(§6, no. 4, Cor. $1$)$\psi^{\sharp}$ は、U から T までの類 $C^r$ の射であり、$\psi^{\sharp}(x) = 0$ と $d_x\psi^{\sharp}=$ Id$_T$ のように、H の演算と互換性があります。したがって、T には、オープン集合 $U'\subset U$ 含む $x$ と 0 のオープン近傍 V が存在し、$\psi^{\sharp}$ 誘導する同型 $\theta : U'\rightarrow V$ となります。必要に応じて $U'$ と V を制限すると、それらは H の下で安定しており、H の演算 (補題 4) と互換性のある同型 $u: T\rightarrow V$ が存在すると仮定できます。 $\varphi =\theta^{-1}\circ u$ も取れば十分です。

G がリー群、H が G の嘘部分群および H が左辺で作用する Y 多様体である場合、(微分可能および解析多様体、結果、6.5.1) を思い出してください。積の $G\times^HY$ 商で表されます。 H の右側多様体 $G\times Y$ 演算 $((g, y), h) \rightarrow (gh, h^{-1}y)$;これは多様体で、リー群 G は左側で自然に動作します。 射影 $G\times^HY\rightarrow G/H$ はファイバー Y のバンドルです。さらに、Y が H が線形に作用する有限次元ベクトル空間である場合、$G\times^HY$ は基底 $G/H ($ 微分可能で解析的なベクトル G バンドルの自然な構造を持ちます。 多様体、結果、7.10.2)。

G を、演算 $(g, x) \rightarrow gx$ の法則が類 $C^r$ となるように、多様体 X (一般位相、第 III, §4, no. 1、定義 1) で適切に動作するリー群とします。次に、X の各点 $x$ に対して、$x$ の軌道 $Gx$ は、X の閉部分多様体であり、同次リー 空間 $G/G_x$ と同型です。 $G_x$ は、G の $x$ の修正者です (cf. 章 III, §1, no. 7、提案 14 (ii)、および一般位相、章 III, §4, no. 2、提案 4)。こちらはコンパクト・リー群（上記参照）です。

#### 命題 6 {#lie-ix-s9-prop-6 .statement tag=01HR}

多様体 X がパラコンパクトであると仮定します。 $x$をXの点、$G_x$をそのフィクサーとします。有限次元解析線型表現 $\tau : G_x\rightarrow \mathbf{G}\mathbf{L}(W)$ と、G の演算と互換性のある類 $C^r$ のオープン埋め込み $\alpha : G\times^{G_x}W\rightarrow X$ が存在し、その写像類 $(e,0)\in G\times W$ は、 $x$。

$T = T_x(X)$を入れます。 W を、$G_x$ で安定な T の $T_x(Gx)$ の補数部分空間とします (たとえば、$G_x$ での T の不変スカラー 積に対する $T_x(Gx)$ の直交補数)。一方、$\varphi : T\rightarrow X$ を、提案 5 に記載されている特性を使用して ($H = G_x$ に対して) 射とします。 $\lambda (g, w) =g\varphi (w)$ によって定義される射 $\lambda : G\times W\rightarrow X$ を考えてみましょう。それは商射 $\mu: G\times^{G_x}W\rightarrow X$ の類 $C^r$ への通過による誘導するであり、G の演算と互換性があり、その写像類 $z$ $(e,0)$から$x$まで。

$\mu$ が点 $z$ でエタールであることを示します。私たちは持っています

寸法(G $\times^{G_x}W$) $=$ 寸法(G) + 寸法(W) $-$ 寸法(G$_x$)

= 寸法(G$x$) $+$ 寸法(W) = 寸法(T)、

したがって、$\mu$ が $z$ で水没していること、または同等に $\lambda$ が $(e,0)$ で水没していることを示せば十分です。ただし、接線写像 $T_{(e,0)}(\lambda ) : T_e(G)\oplus W\rightarrow T$ は $T_e(\rho (x)) +i$ に等しく、$\rho (x)$ は W から T までの軌道写像 $g \rightarrow gx$ と $i$ 標準単射です。 Im $T_e(\rho (x)) = T_x(Gx)$ なので、写像 $T_{(e,0)}(\lambda )$ は全射法であり、$\mu$ は $z$ のエタールです。

$G\times^{G_x}W$ に、G の下で安定した、$Gz$ のオープン近傍 $\Omega$ が存在し、$\Omega$ から X のオープン部分集合に$\mu$ 誘導する同型が存在することを示します。これは、命題を意味します。実際、$G\times W$ の $\Omega$ の逆像は G の下で安定しており、したがって形 $G\times B$ になります。ここで、B は原点である W 含むのオープン部分集合であり、$G_x$ の下で安定です。必要に応じて $\Omega$ を制限すると、$G_x$ (補題 4) の演算と互換性のある同型 $u: W\rightarrow B$ が存在すると仮定できます。合成射 $\alpha : G\times^{G_x}W\overset{(Id,u)}{\longrightarrow}G\times^{G_x}B\longrightarrow^\mu$ X が命題の主張で条件を満たすことは明らかです。

したがって、命題は次の補題の帰結です。

#### 補題 5 {#lie-ix-s9-lem-5 .statement tag=01HS}

Z を、クラス $C^r$ の左演算法則 $m: G\times Z\rightarrow Z$ と G の演算と互換性のある射 (クラス $C^r$ の) $\mu: Z\rightarrow X$ を備えたクラス $C^r$ の分離多様体とする。 $z$をZの点、および$x=\mu(z)$とします。 $\mu$ が $z$ でエタールであり、G の $z$ のフィクサーが $x$ のフィクサー $G_x$ に等しいと仮定します。 次に、G の下で安定した、$\Omega$ から X のオープン部分集合への $\mu$ 誘導する同型のような、軌道 $Gz$ のオープン近傍 $\Omega$ が存在します。

$\mu$ は G の演算と互換性があるため、$Gz$ の点ごとにエターレになります。正準写像 $G/G_x\rightarrow Gx$ は同型写像であるため、$\mu$ によって誘導される $Gz$ から $Gx$ への写像も同型写像です。したがって、no. 1 の提案 2 から、$\mu$ 誘導するの U の X へのオープン埋め込みとなるように、Z に $Gz$ のオープン近傍 U が存在することがわかります。

G は X で適切に動作するため、$g \notin K ($ 一般位相に対して $gV\cap V =\emptyset$ となるような、$x$ のオープン近傍 V とコンパクトな G の部分集合 K が存在します。 III, §4, no. 4、提案 7);特に$e\in K$。 集合点 $y\in Z$ の $W_1$ は、$Ky\subset U$ が Z で開いているようになります。確かに、Z**--** $W_1$ は、適切な条件の下で、閉じた集合 $(K\times Z)$ **--** $m^{-1}(U)$ の像です。 射影 pr$_2: K\times Z\rightarrow Z$。 $W = W_1\cap \mu^{-1}(V)$を入れてください。これは、Z のオープン部分集合、含む $z$、および次の条件の満たすです。

(i) KW $\subset U$、特に $W\subset U$;

(ii) $\mu(W)\subset V$。

$\Omega =$ GW として、$\mu$ から $\Omega$ の制限を考えます。これはエタール射です。$\Omega$ のすべての点は、G の下で U の点までの共役であるからです。これが単射であることを示します。G の $g, h$ と W の $u, v$ が $\mu(gu) =$ $\mu(hv)$ となるようにします。 $k=g^{-1}h$を入れてください。次に$\mu(u) =k\mu(v)$なので、(ii)により$k\in K$になります。ただし、$kv$ と $u$ 属するは (i) によって U に送信されます。従って、$u=kv$は、$\mu$からVの制限が単射なので、$gu=hv$となります。従って、$\mu$ から $\Omega$ の制限は単射的であり、その結果 (微分可能および解析多様体、結果、5.7.8) は X の開部分多様体上で同型となり、証明が完成します。

提案6の条件のもとでは、$\alpha$の像は、$x$の軌道Aのオープン近傍Tであり、基底Aとベクトルの構造のバンドルが装備されており、そのために零切断は軌道 Aそのもの。 このような近傍をリニアチューブと呼びます（問題の軌道あたり）。 各点 $a\in A$ について、このベクトルバンドルのファイバー $Y_a$ は X の部分多様体であり、$a$ の定着器 $G_a$ の下で安定しており、射が $G\times^{G_a}Y_a$ から X になるように、 写像類の $(g, y)\in G\times Y_a$ から $gy\in X$ 誘導する射の類 $C^r$ $G\times^{G_a}Y_a$ から T. 次に、$Y_a$ はチューブ T の$a$ における横線であると言われます。 $Y_a$の$a$における接線空間は$Y_a$と正準的に同型であり、$T_a(X)$の$T_a(A)$の補数であることに注目します。従って、ベクトルバンドル T と基底 A は、X の A の正規バンドルと正準的に同型です (微分可能および解析多様体、結果、8.1.3)。

### 4. 軌道型

G を、分離されたトポロジカル空間 E 上で連続的に動作するトポロジカル群とする。E のすべての点 $x$ について、G の $x$ の固定子を $G_x$ で表し、標準写像 $G/G_x\rightarrow Gx$ が同相同型であると仮定する。これは特に次の 2 つの状況に当てはまります。

a) G と E のトポロジーは離散的です。

$b) G$ は E (一般位相、章 III, §4, no. 2、提案 4) で適切に動作します。たとえば、G はコンパクトです (一般位相、章 III, §4, no. 1、提案 2)。

G の閉じた部分群の共役類の $\mathscr{T}$ 集合で表します。 For every $x\in E$, we call the orbit type of $x$, or sometimes the type of $x$, the class of $G_x$ in $\mathscr{T}$; two points of the same orbit are of the same orbit type (Algebra, Chap. I, §5, no. 2, Prop. 2); two orbits are of the same type if and only if they are isomorphic as G-sets (Algebra, Chap. I, §5, no. 5, Th. 1). すべての $t\in \mathscr{T}$ について、型 $t$ の E の点の $E_{(t)}$ 集合、つまり型 $t$ の軌道の和集合で表します。これはEの安定した部分集合です。 $H\in t$ の場合は、$E_{(t)}$ の場合は $E_{(H)}$ とも書きます。たとえば、$E_{(G)}$ は、G によって固定された点の E からなるの閉じた部分空間です。

$\mathscr{T}$ に次の予約注文関係を与えます:

$t\leq t'\Leftarrow \Rightarrow$ には、$H\supset H'$ となるような $H\in t$ と $H'\in t'$ が存在します。

$\Omega$ と $\Omega '$ を、$E,t$ と $t'$ の型上の G の 2 つの軌道とします。次に、$\Omega '$ から $\Omega$ までの G 射 (必ず全射連続) が存在する場合に限り、$t\leq t'$ になります。

$x, x'$ を E に、$t, t'$ をその型にします。 $aG_{x'}a^{-1}\subset G_x$ となるような $a\in G$ が存在する場合に限り、$t\leq t'$ になります。

#### 補題 6 {#lie-ix-s9-lem-6 .statement tag=01HT}

G をリー群とします。

a) G のコンパクト部分群のすべての減少列は静止しています。

b) H と $H'$ を、$H\subset H'$ となり、$H'$ から H まで (トポロジカル群の) 同型が存在するような G の 2 つのコンパクト部分群とします。すると、$H = H'$ となります。

c) With the relation $t\leq t'$, the set $\mathscr{T}$ is a noetherian ordered set (Theory of Sets, Chap. III, §6, no. 5, text preceding Prop. 7).

a) Let $(H_i)_{i\geq 1}$ be a decreasing sequence of compact subgroups of G; these are Lie subgroups of G (Chap. III, §8, no. 2, Th. 2). 整数 (暗さ$H_i$)$_{i\geq 1}$ の数列は減少するなので静止しているため、部分群 $H_i$ が $i\geq N$ に対して同じ同一性成分を持つような整数 N が存在します。 すると、正の整数 $(H_i: (H_i)_0)_{i\geq N}$ の減少列は静止しているので、 $i$ 十分大きいに対して $H_i= H_{i+1}$ です。

b) $f$ を $H'$ から H までの同型とします。 数列 $(f^n(H))_{n\geq 0}$ は G のコンパクト部分群の減少列であるため、a) により $n$ 十分大きいに対して $f^n(H) =f^{n+1}(H)$ となります。 $f$ は同型であるため、これは $f(H) = H =f(H')$、つまり $H = H'$ を意味します。

c) $t, t'\in \mathscr{T}$ を $t\leq t'$ と $t'\leq t$ となるようにします。すると、$H\supset H'$と$H_1\subset H'_1$が存在するような$H,H_1\in t$と$H',H'_1\in t'$が存在します。 $g$ と $g'$ を、$H_1=gHg^{-1}$ と $H'_1=g'H'g^{'-1}$ となるような G の 2 つの元とします。 $u=g^{'-1}g$を入れます。それから

$$
uHu^{-1}\subset H'\subset H
$$

b) により、これは $uHu^{-1}= H$、つまり $H'= H$ と $t'=t$ を意味します。したがって、集合 $\mathscr{T}$ が順序付けされ、a) によりネーター になります。

#### 定理 2 {#lie-ix-s9-thm-2 .statement tag=01HU}

G を X で適切に動作するリー群とし、演算 $(g, x) \rightarrow gx$ の法則が類 $C^r$ となるようにします。 X がパラコンパクトであると仮定します。

a) X の任意の点に関連する写像の軌道型は次の半連続性性質を持ちます。$x\in X$ と$t\in \mathscr{T}$ をその軌道型とします。 $x$ の安定したオープン近傍 U が存在し、任意の $u\in U$ に対して、$u$ の型は $\geq t$ になります。

b) すべての $t\in \mathscr{T},X_{(t)}$ は X の部分多様体であり、G の演算によって誘導される $X_{(t)}$ 上の同値関係は正則であり (微分可能および解析多様体、結果、5.9.5)、射 $X_{(t)}\rightarrow X_{(t)}/G$ は aバンドル。

c) $X/G$ が接続されていると仮定します。すると、軌道の集合、Xの元の型は最大の元$\tau$になります。さらに、$X_{(\tau)}$はXの密なオープン部分集合と$X_{(\tau)}/G$が接続されています。

$x$ を X の点とし、$t\in \mathscr{T}$ をその型とします。 a) と b) を証明するには、安定したオープン集合含む $x$ によって置き換える X ができ、したがって (提案 6) X は形 $G\times^HW$ であると仮定できます。ここで、W は a の空間です。 G のコンパクト部分群 H の有限次元解析線型表現、正規射影 $p: G\times W\rightarrow G\times^HW$ の下で、点 $x$ は $(e,0)\in G\times W$ の像 $p(e,0)$ です。 $u=p(g, y)\in G\times^HW$ と $a\in G$ の場合、$(ag, y) = (gh^{-1}, hy)$ とともに $h\in H$ が存在する場合、つまり $a\in gH_yg^{-1}$ の場合に限り、$au=u$ になります。したがって、$G_u=gH_yg^{-1}$;特に $G_x= H$ なので、$G_u$ は $G_x$ の共役から部分群であり、$u$ の型が $\geq t$ であることが証明されます。したがって、a)。

さらに、$G_u$ が G の H に対して共役であるか、または等価に $H_y$ が G の H に対して共役である場合に限り、$u$ は型 $t$ です。 補題 $6b)$ により、これは $H_y= H$ となり、従って $y$ が H によって固定されることを意味します。 $W'$ が W のベクトル部分空間元のからなるが H によって固定される場合、$X_{(t)}$ は次のように識別できることになります。 $G\times^HW'$、従って $G/H\times W'$ もあり、従って b)。

c)を証明するには、$X/G$が接続されている仮定は、Xが有限次元から純粋であることを意味していることを観察してください。実際、すべての$k\geq 0$について、点$x\in X$の$X_k$集合で示され、$_xX =k$が薄暗くなります。この場合、$X_k$ は X で開閉し、G の下で安定しているため、X は $X_k$ の 1 つと等しくなります。

ここで、c) を X の次元で帰納法により証明し、主張は薄暗い X = 0 に対して明確です。 $\tau$ を軌道型の点の X のうち極大元とします ( 元は補題 $6c$)$)$ までに存在します。次のことを証明します。

$c')$ $X_{(t)}$ の部分集合 A ごとに、$X_{(\tau)}$ で開閉し、G の下で安定している場合、X の A の閉鎖 $\overline{A}$ が開いています。

この主張は c) を意味します。確かに、$X_{(\tau)}$ が最初に注意 X にオープンするのは、a) によるものです。 主張 $c')$ は、$\overline{X}_{(\tau)}$ が X で開いて閉じていることを意味します。従って、G の下で安定しており、$X/G$ が接続されているため、X と等しくなります。 A を G の下で安定した空ではない開いた閉じた $X_{(\tau)}$ の部分集合とします。 $c'),\overline{A}$ までは X で開閉し、G の下で安定しているため、X に等しい。これは、A が $X_{(\tau)}$ で密であるため、$X_{(\tau)}$ に等しいことを意味します。従って、$X_{(\tau)}/G$ の空でない開いた部分集合と閉じた部分集合はすべて $X_{(\tau)}/G$ に等しく、$X_{(\tau)}/G$ が接続されていることを証明します。最後に、$X_{(\tau)}$ は X で密であるため、a) から、X のすべての点は型 $\leq \tau$ であることがわかります。他の語、$\tau$は、Xの点の軌道型のうち、最大の元です。

これで $c')$ が証明されました。 A は空ではないと仮定できます。 $x\in A$ にしましょう。 A が $x$ の近傍であることを証明すれば十分です。このために、上記のように、H コンパクトで $X = G\times^HW$、$x$ が $(e,0)$ の標準像であると仮定できます。まず、H が W に対して自明に作用すると仮定します。その場合、X は $(G/H)\times W$ と識別でき、$X_{(\tau)}/G = X/G$ は W と同相であるため接続されます。従って、$A/G = X/G$、つまり A = X となります。これから H は W 上で自明に動作しないと仮定します。 選ぶはコンパクトな群 H の下で W 上のスカラー 積は不変です。 S を W の単位元球体とします (ノルム 1 のベクトルの集合)。 $S/H$ が接続されていることに注意してください。実際、dim(W) $\geq 2, S$ が接続され、dim(W) = 1 の場合、S は 2 つの点の空間であり、H は自明ではありません。 $Y = G\times^HS$を入れてください。これは余次元 1 の G のもとで安定な X の閉部分多様体であり、$S/H$ と同相である $Y/G$ が接続されています。従って、帰納法の仮定までに、Yには最大軌道型$\theta$が存在し、集合$Y_{(\theta)}$はYで開いていて密であり、$Y_{(\theta)}/G$は接続されています。

$G\times W$ の $\mathbf{R}^*_+$ の演算法則 $(\lambda ,(g, w)) \rightarrow (g, \lambda w)$ による商への通過によって引き起こされる X の $\mathbf{R}^*_+$ の演算を考えてみましょう。 この演算の下にある X 共役の 2 つの点は同じ軌道型です。結果として、$X_{(\theta)}$ 含む $\mathbf{R}^*_+Y_{(\theta)}$ は、X の密なオープン部分集合です。 しかし、$X_{(\tau)}$ は a) によって開いているので、$X_{(\theta)}$ を満たすため、$\theta =\tau$ になります。

一方、$\mathbf{R}^*_+\times S$ から W **--** $\{0\}($ 一般位相までの同相同型 $(\lambda , w) \rightarrow \lambda w$ は、第 1 章で定義されています。 VI, §2, no. 3、提案 3) 誘導するは $\mathbf{R}^*_+\times (S/H)$ から $(\mathbf{R}^*_+S)/H$ までの同型写像、従って $\mathbf{R}^*_+\times (Y/G)$ から $(\mathbf{R}^*_+Y)/G$ および $\mathbf{R}^*_+\times (Y_{(\theta)}/G)$ から $(\mathbf{R}^*_+Y_{(\theta)})/G$ も同様です。 Thus, $(\mathbf{R}^*_+Y_{(\theta)})/G$ is connected, and $X_{(\tau)}/G$, which contains a connected dense subset, is itself connected (General Topology, Chap. I, §11, no. 1, Prop. 1). その結果、A は $X_{(\tau)}$ に等しいため、X では密になり、A は $x$ の近傍になります。 これで定理の証明が完成です。

Thの記法と。 $X_{(\tau)}$ の $2c)$、点はプリンシパルと呼ばれ、その軌道はプリンシパル軌道と呼ばれます。 $x$ が X の点で、$G\times^{G_x}W$ が $x$ の軌道付近の X の線形チューブである場合、点 $x$ は、$G_x$ が W 上で自明に動作する場合、つまりチューブが形 $(G/G_x)\times W$。

#### 例 1 {#lie-ix-s9-n4-exa-1 .statement tag=01HV}

G を接続されたコンパクト・リー群とし、内部自己同型によってそれ自体で動作します。 G の元 $x$ のフィクサーは、単に G の $x$ のセントラライザー $Z(x)$ です。それは含む最大値トーラス含む $x$ です。従って、最大の軌道型 $\tau$ は、G の最大トーラスの共役類です。開いた集合 $G_{(\tau)}$ は、G のまさに正則元の集合 (§5, no. 1, 注意）。 G が単純接続されていると仮定します。この場合、$G_{(\tau)}$ は G (§5, no. 2, 注意 2) の正則元の集合 $G_r$ に等しくなります。 A が $\mathfrak{g}= L(G)$ のカルタン部分代数 $\mathfrak{t}$ のアルコーブである場合、合成写像 $\pi : A\longrightarrow^{exp}G_r\longrightarrow G_r/$Int(G) は解析的多様体の同型です。実際、これは同型写像です (§5, no. 2、提案 2 の補正)。 $a\in A$ とすると、$\gamma (t)$ という変換によって $t=$ exp $a$ と同一視する $T_t(G)$ を $\mathfrak{g}$ に置き換えます。接線写像 $T_a(\pi )$ は、標準単射 $\mathfrak{t}\rightarrow \mathfrak{g}$ と商写像 $\mathfrak{g}\rightarrow \mathfrak{g}/$Im(Ad $t^{-1}-1$) の合成で識別できます。 $t$ は正則であるため、$T_a(\pi )$ は同型となり、記載された結果になります (微分可能および解析多様体、結果、5.7.8)。

#### 例 2 {#lie-ix-s9-n4-exa-2 .statement tag=01HW}

Eを、Eの超平面の実ユークリッドアフィン空間、$\mathfrak{H}$集合、$\mathfrak{H}$の超平面に関して直交反射によって生成されるEの変位のW群とする。 $\mathfrak{H}$ が W で安定しており、群 W が離散位相とともに E で適切に動作すると仮定します。

前述のことは、E 上の W の演算にも適用できます。E の点 $x$ の固定子は、$\mathfrak{H}$ 含む $x$ の超平面に対する反射によって生成された W の部分群です（V, §3, no. 3 章、Prop. 2)。従って、最大の軌道型 $\tau$ は部分群 $\{$Id$_E\}$ の類であり、$E_{(\tau)}$ は E の部屋の和集合です。この場合、カバー$E_{(\tau)}\rightarrow E_{(\tau)}/W$ は自明であり、特に $\mathfrak{H}$ が空でない場合、$E_{(\tau)}$ は接続されません。

### 練習問題 {#lie-ix-s9-exercises}

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
