---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 8
section_title: Norms and traces
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.47-A V.51, A V.153
pdf_pages: 0161-0165, 0267-0267
extraction: ocr
subsections:
    - "no": 1
      title: Recall
      page: 47
      pdf_page: 161
    - "no": 2
      title: Norms and traces in etale algebras
      page: 47
      pdf_page: 161
    - "no": 3
      title: Norms and traces in extensions of finite degree
      page: 50
      pdf_page: 164
statements: 9
exercises: 2
content_sha256: beec54746842797327901d9336f4541b2458290b2f3da4c0122c6d3b7444e885
translated_from: content/en/alg/V/08_s8_norms_and_traces.md
translation_method: google
source_content_sha256: c2e7557b98c678b7ab7b76840a046be64717fd2ef2e68d0dbcc702987b154e2d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 790071fa0463ec54fc8d098e388f615bae3511fbcced9cd01bd96c2cc4b625fd
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 8。 ノルムと痕跡

この段落全体を通じて、K は体を表します。

### 1. リコール

A を K 上の有限次数 $n$ の代数とします。それぞれの $x \in A$ を、A の $L_x$ 線形写像 $a \mapsto xa$ でそれ自体に表します。 (III, p. 543) $L_x$ のトレースは A に対する x のトレースと呼ばれ、$\mathrm{Tr}_{A/K}(x)$ と書かれることを思い出してください。同様に、$L_x$の行列式は、Aを基準としたxのノルムと呼ばれ、$N_{A/K}(x)$で表されます。 A の n 元の数列 $(x_1, ..., x_n)$ の判別式は、行列 $(\mathrm{Tr}_{A/K}(x_i x_j))_{1 \leq i,j \leq n}$ の定義行列式 $D_{A/K}(x_1, ..., x_n)$ (III, p. 549) です。

K' を K の拡大とし、$A' = A_{(K')}$ をスカラーの拡大によって A から導出された K'-代数とします。公式はあります

(1) $$
\mathrm{Tr}_{A'/K'}(1 \otimes x) = \mathrm{Tr}_{A/K}(x) . 1 , \quad N_{A'/K'}(1 \otimes x) = N_{A/K}(x) . 1
$$
$x \in A$ (III、p. 544) 全員に。 A の数列 $(x_1, ..., x_n)$ の元ごとに、

(2) $$
D_{A'/K'}(1 \otimes x_1, ..., 1 \otimes x_n) = D_{A/K}(x_1, ..., x_n) . 1 ,
$$
最初の公式 (1) からは以下の通り。

### 2. ノルムそしてエターレの痕跡代数

A を K 上の (有限) 次数 $n$ のエタール代数とします。定義までに、K の拡大 L と、以下の特性を持つ A の別個の準同型 $u_1, ..., u_n$ が L に存在します。

a) $A$ から $L$ への各準同型は、$u_i$ (V、p. 29、Cor.) の 1 つに等しい。
b) 次のような $L$-代数同型性 $u : A_{(L)} \to L^n$ が存在します。

$$
u(1 \otimes x) = (u_1(x), \ldots, u_n(x)) \quad \text{for all } x \in A .
$$

さらに、$K$ のすべての代数閉拡大 $L$ は上記の特性を持ちます (V、p. 30、提案 2)。

以下の$L, u_1, \ldots, u_n$を修正します。 $x \in A$ にしましょう。公式を証明しましょう

$$
\text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) , \quad \text{N}_{A/K}(x) \cdot 1 = \prod_{i=1}^n u_i(x) .
$$

$v$ を $A_{(L)}$ の $l \otimes x$ までに乗法とします。 $L^n$の標準基底の$u^{-1}$の下にある像である$A_{(L)}$の基底に関して、線形写像$v$の行列は対角線元と対角線です。 $u_1(x), \ldots, u_n(x)$。私たち結論するはそれを

$$
Tr_{A_{(L)}/L}(1 \circ x) \cdot 1 = \sum_{r=1}^n u_i(x) , \quad \text{whence} \quad \text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) \text{ by (1)} ;
$$

ノルムの場合も同様に扱われます。

さらに、$(x_1, \ldots, x_n)$ を $A$ の元の数列とし、U を行列とします

$$
(u_i(x_j))_{1 \leq i,j \leq n}
$$

そして$(t_{ij}) = 'U . U$にしましょう。最初の公式 (3) までに、

$$
\text{Tr}_{A/K}(x_i x_j) \cdot 1 = \sum_{k=1}^n u_k(x_i x_j) = \sum_{k=1}^n u_k(x_i) u_k(x_j) = t_{ij} ;
$$

移行から行列式を取得します。

$$
D_{A/K}(x_1, \ldots, x_r) \cdot 1 = [\det u_i(x_j)]^2 .
$$

#### 命題 1 {#alg-v-s8-prop-1 .statement tag=06L9}

— *$A$を$K$以上の有限次数の可換代数とします。したがって、次の条件は同等です*:
a) *代数 $A$ はエターレです。*
b) *判別式が非ゼロである $A$ のうち基底が存在します。
c) *$A$ の各 $x \neq 0$ に対して、$A$ には $\text{Tr}_{A/K}(xy) \neq 0$ となる $y$ が存在します。*
*さらに、これらの条件が満たされる場合、$A$のいずれかの基底の判別式は非ゼロになります。

$A$ が etale であると仮定した場合、$A$ の$K$ の任意の基底 $(x_1, \ldots, x_n)$ に関する $A$ の判別式は非ゼロであることを示します。これは特に $a) \Rightarrow b)$ の含意を確立します。 (4) により、上記の記法を使用して、行列 U が可逆であること、または同等に線形方程式の系を示すだけで十分です。

$$
\sum_{i=1}^n \lambda_i u_i(x_j) = 0 \quad (\text{for } 1 \leq j \leq n)
$$

Lには解$\lambda_1 = \cdots = A, = 0$しかありません。ここで、関係 (5) は、準同型 (V、p. 27、Th. 1) の線形独立性に関する定理によって、すべての $x \in A$ に対して $\sum_{i=1}^n \lambda_i u_i(x) = 0$、$1 \leq i \leq n$ に対してよって $\lambda_i = 0$ を意味します。

b) および c) の同値は、次の一般補題の帰結です。

#### 補題 1 {#alg-v-s8-lem-1 .statement tag=06LA}

V を K および B 上の有限次元のベクトル空間とし、* V x V 上の双線形 *形とします。 $(v_1, \ldots, v_n)$ *を * V *K * と * $\Delta = \det B(v_i, v_j)$ の基底とします。 そして、*if* の場合に限り、V の各 $x \neq 0$ に対して V に $B(x, y) \neq 0$ となる y が存在する場合、$A \neq 0$ となります。

線形方程式が系である場合に限り、 $A \neq 0$ が得られます。

$$
\sum_{i=1}^n \lambda_i B(v_i, v_j) = 0 \quad (1 \leq j \leq n)
$$

K には解 $A, = \cdots = A, = 0$ しかありません。$x = \sum_{i=1}^n \lambda_i v_i$ を置くと、上記の系は $1 \leq j \leq n$ の $B(x, v_j) = 0$ に相当します。また、$(v_1, \ldots, v_n)$ は K 上のV の基底なので、すべての$B(x, y) = 0$ になります。 $y \in V$、よって補題。

条件 c) は A が減少することを意味することを示しましょう。 x を A の冪零元とします。 : 任意の $y \in A$ 元 xy に対して nilpotent であるため、 ベクトル空間 A の自己準同型 $L_{xy}$ も nilpotent です。ここで、次の補題は、仮定 c) の下のすべての $y \in A$、よって $x = 0$ に対して $\mathrm{Tr}(xy) = 0$ を意味します。

#### 補題 2 {#alg-v-s8-lem-2 .statement tag=06LB}

V を K 上の有限次元のベクトル空間と V の $u$ 冪零自己準同型として、$\mathrm{Tr}(u) = 0$ とします。

それぞれの整数 $n \geq 0$ について、$V_n$ を $u^n$ の像とします。 $u$ はゼロポテントなので、$0 \leq i < r - 1$ に対して $V_0 = V, V_r = 0$ と $V_i \neq V_{i+1}$ となるような整数 $r \geq 0$ が存在します。 $d_i$ を $V_{i-1}$ の次元とします ($1 \leq i \leq r$ の場合)。 V の基底 $(x_1, \ldots, x_d)$ は、$V_{i-1}$ の $d - d_i < j \leq d$ 形基底とベクトル $x_j$ が存在します ($1 \leq i \leq r$ の場合)。 $u(V_{i-1}) \subset V_i$ があるので、基底 $(x_1, \ldots, x_d)$ の $u$ の行列の対角線元は零です。したがって、$\mathrm{Tr}(u) = 0$ と補題が続きます。

最後に、b) が a) を意味することを示しましょう。 $(x_1, \ldots, x_n)$ を、$D_{A/K}(x_1, \ldots, x_n) \neq 0$ となるような K 上の A の基底とします。 K'をKの拡大、A'をスカラーの拡大と$1 \leq i \leq n$の$x'_i = 1 \otimes x_i$によってAから導出されたK'代数とする。 公式 (2) (V, p. 47) までに $D_{A'/K'}(x'_1, \ldots, x'_n) \neq 0$ になります。 適用 A' に対する前の結果から、A' が還元されることがわかります。したがって、代数 A はエターレ (V, p. 34, Th. 4) です。

#### 系 {#alg-v-s8-n2-cor-1 .statement tag=06LC}

— E を K の *有限* 次数拡大とします。 E が分離可能であるためには、E に $\mathrm{Tr}_{E/K}(a) \neq 0$ となるような a が存在することが必要かつ十分です。

条件は提案 1 により必要ですが、逆に、$\mathrm{Tr}_{E/K}(a) \neq 0$ となるような$a \in E$ が存在すると仮定します。 E に $x \neq 0$ が与えられた場合、$y = a x'$ を置くと、$\mathrm{Tr}_{E/K}(xy) \neq 0$ になります。さて、提案 1 は、E が K 上のエタール代数、したがって K の分離拡大であることを示しています。

### 3. ノルムと有限次数の拡大の痕跡

代数(III、p. 548)の推移性式は、有限次数の拡大の場合、次の命題を意味します。

#### 命題 2 {#alg-v-s8-prop-2 .statement tag=06LD}

— F を K の有限次数の拡大とし、E を F の部分拡張とします。すると、すべての $x \in F$ について次のようになります。
$$
\text{Tr}_{F/K}(x) = \text{Tr}_{E/K}(\text{Tr}_{F/E}(x)) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(\text{N}_{F/E}(x)) .
$$

#### 系 {#alg-v-s8-n3-cor-1 .statement tag=06LE}

— $m = [F : E]$ を入れます。 $x \in E$ごとに、
$$
\text{Tr}_{F/K}(x) = m \cdot \text{Tr}_{E/K}(x) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(x)^m .
$$

#### 命題 3 {#alg-v-s8-prop-3 .statement tag=06LF}

— E を K の有限次数 n の拡大および E の x 元、K 上の次数 d であるとします。K 上の X の最小多項式として $f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ を書きます。
$$
\text{Tr}_{E/K}(x) = - \frac{n}{d} a_1 \\
\text{N}_{E/K}(x) = (((-1)^d a_d)^{n/d} = (-1)^n a_d^{n/d} .
$$

提案 3 は、Cor. から直接続くものです。提案 2 と補題:

#### 補題 3 {#alg-v-s8-lem-3 .statement tag=06LG}

R を可換環、$f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ $\mathbf{R}[X]$、A R-代数 $\mathbf{R}[X]/(f)$ および A の X の x 剰余類とします。次に、$\text{Tr}_{A/R}(x) = -a_1$ と $\text{N}_{A/R}(x) = (-1)^d a_d$ です。

コルによって。 (IV, p. 11) 数列 $(1, x, ..., x^{d-1})$ は A の基底です。さらに私たちは持っています
$$
x \cdot 1 = x , \quad x \cdot x = x^2 , \ldots , x \cdot x^{d-2} = x^{d-1} ,
$$
$$
x \cdot x^{d-1} = -a_d \cdot 1 - a_{d-1} \cdot x - \ldots - a_1 \cdot x^{d-1}
$$

$A$の基底$(1, x, ..., x^{d-1})$に関して乗法をxで表す行列は、以下の形になります（アイデアを修正するために$d = 5$を採用しました）。

$$
\begin{pmatrix}
0 & 0 & 0 & 0 & -a \\
1 & 0 & 0 & 0 & -a \\
0 & 1 & 0 & 0 & -a_3 \\
0 & 0 & 1 & 0 & -a_2 \\
0 & 0 & 0 & 1 & -a_1
\end{pmatrix}
$$

この行列の痕跡は明らかに$-a$です。 行列式は最初の行で展開することで計算でき、次のことがわかります。

$$
(-1)^{d-1} (-a_d) = (-1)^d a_d .
$$

この No. の残りについては、K の有限次数の E 拡大と E の $x$ 元で表します。さまざまな場合の計算するノルムと $x$ のトレース方法を示します。

a) *分離拡大* の場合: E が K 上で次数 $n$ から分離可能であると仮定します。K の $\Omega$ 代数閉包と、E から R への$n$ の異なる $K$ 準同型性を $\sigma_1, \ldots, \sigma_n$ で表します。公式 (3) ($V$, p. 48) R にあります

$$
\text{Tr}_{E/K}(x) = \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \prod_{i=1}^n \sigma_i(x) .
$$

b) *p ラジカル拡張の場合*: K が特性 $p > 0$ であり、拡大 E が p ラジカルであると仮定します。 $[E:K] = p^e$ となるような整数 $e \geq 0$ が存在します ($V$, p. 26、提案 4)。 $f$ が K 上の $x$ の高さである場合、K 上の $x$ の最小多項式は $X^{p^f} - x^{p^f}$ ($V$, p. 24、提案 1) です。提案 3 により、$N_{E/K}(x) = (x^{p^f})^{p^e/p^f}$、よってが得られます。

$$
N_{E/K}(x) = x^{p^e} = x^{[E:K]}
$$

トレースでは、$\text{Tr}_{E/K}(x) = -p^{e-f} a$ を見つけます。ここで、$a$ は多項式 $X^{p^f} - x^{p^f}$ の $X^{p^f-1}$ の係数です。他の語では、

$$
\text{Tr}_{E/K}(x) = p^e \cdot x = [E:K] x = \begin{cases} x & \text{if } [E:K] = 1 \\ 0 & \text{if } [E:K] > 1 . \end{cases}
$$

c) *一般的なケース*: ノルムの計算を要約し、次の命題でトレースできます。

#### 命題 4 {#alg-v-s8-prop-4 .statement tag=06LH}

*p を K の特性指数と K の有限次数の E 拡大とします。$\sigma_1, \ldots, \sigma_n$ を K の代数閉包 $\Omega$ への E の個別の K 準同型性とし、$p^e = [E:K]_i$ とします。それぞれの $x \in E$ には $\Omega$* があります

$$
\text{Tr}_{E/K}(x) = p^e \cdot \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \left( \prod_{i=1}^n \sigma_i(x) \right)^{p^e} .
$$

E を E における K の相対分離閉包とします。その場合、$E_s$ は K の次数 $n$ の分離拡大と E の異なる K 準同型性の $\sigma_1, \ldots, \sigma_n$ 誘導するを R に変換します。さらに、E は E の ap-radical 拡張であり、次数 p$^e$ ($V$、p. 44、提案 13 および p. 46) です。したがって、式 (6)、(7)、(13)、(14)、(12) から提案 4 が得られます。

### 練習問題 {#alg-v-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
