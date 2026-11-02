---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 2
section_title: Bidual. Reflexive spaces
lang: ja
source: evt-i-v
book_pages: TVS IV.14-TVS IV.21, TVS IV.52-TVS IV.57
pdf_pages: 0196-0203, 0234-0239
extraction: ocr
subsections:
    - "no": 1
      title: Bidual
      page: 14
      pdf_page: 196
    - "no": 2
      title: Semi-reflexive spaces
      page: 15
      pdf_page: 197
    - "no": 3
      title: Reflexive spaces
      page: 16
      pdf_page: 198
    - "no": 4
      title: The case of normed spaces
      page: 17
      pdf_page: 199
    - "no": 5
      title: Montel spaces
      page: 18
      pdf_page: 200
statements: 32
exercises: 26
content_sha256: f1a33eda5b5a9855b2235b4e4eead428e15d62ef16711987f3e7b260ff65a6e3
translated_from: content/en/evt/IV/02_s2_bidual_reflexive_spaces.md
translation_method: google
source_content_sha256: b91386e65623979a9a9994a73c883cd7ba5db67a5bb1adc0fbb46df95c3c8a73
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: f43027fe77edaca6eea62eb9bff3b43fbe72fb5ad62830a42db99a9edca11607
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。バイデュアル。反射的空間

### 1. バイデュアル

#### 定義 1 {#evt-iv-s2-def-1 .statement tag=07S8}

— *$E$ を局所凸空間とし、$E'_b$ をその強力な双対とします。局所凸空間 $E'_b$ の双対は $E$ の双双と呼ばれ、$E''$ で表されます*。

For every $x \in E$, let $\tilde{x}$ be 線型形式 $x' \mapsto \langle x, x' \rangle$ on $E'$; it is continuous for the weak 位相 $\sigma(E', E)$, hence *なおさら*, for the strong 位相 on $E'$;したがって、すべての $x \in E$ に対して $\tilde{x} \in E''$ です。 写像 $c_E : x \mapsto \tilde{x}$ from $E$ into $E''$ is 線形写像, said to be *canonical*.

#### 命題 1 {#evt-iv-s2-prop-1 .statement tag=07S9}

— *$c_E : E \to E''$の核は、$E$の0の閉包です。 $E$ がハウスドルフの場合、$c_E$ は単射法です。*

構成までに、$c_E$の核は、$E$の連続線型形式の核の共通部分、つまり$E$の$\{0\}$の終結（II、p. 24、cor. 1)。

$E$ がハウスドルフの場合、写像 $c_E$ により、$E''$ の部分空間で同一視する $E$ になります。

バイデュアル。反射的空間

テレビ IV.15

$E''$ 上の強い位相は $\mathscr{S}$ トポロジーであり、$\mathscr{S}$ は$E'$ のすべての強く境界付けられた部分集合のファミリーです。 $E'$ のすべての等連続部分集合は強く有界されているため (III、p. 22、提案 9)、$E$ の最初の位相は、強い方程式の $c_E$ の下で逆像を取ることで得られる位相よりも粗くなります。 $E''$の位相。厳密にはもっと粗くすることもできます (IV、p. 52、演習 1)。しかし：

#### 命題 2 {#evt-iv-s2-prop-2 .statement tag=07SA}

— 空間 $E$ がボーンロジカルまたはバレルドであると仮定します。 $E$ の初期トポロジは、$E''$ の強力な位相の $c_E$ の下で逆像です。

なぜなら、強く有界された $E'$ のすべての部分集合は等連続だからです (III、p. 22、提案 10 および III、p. 24)。

#### 命題 3 {#evt-iv-s2-prop-3 .statement tag=07SB}

— $E$ を局所凸ハウスドルフ空間とします。 位数では、$E$ の強力な双対 $E'_b$ がバレル化されるため、$\sigma(E'', E')$ に限定される $E''$ のすべての部分集合が、$E$ の限定された部分集合の$\sigma(E'', E')$ のクロージャに含まれることが必要かつ十分です。

$E''$の等連続部分集合は、部分空間の有界部分集合、$E$の$E''$の双極性（$E''$と$E'$の間の双極性の場合）に含まれる部分集合です。これで、バイポーラの定理 (II、p. 45、cor. 3) とバレル付きの空間 (III、p. 24) の定義を適用するだけで十分です。

#### 注意 {#evt-iv-s2-n1-rem-1 .statement tag=07SC}

$E$ を局所凸ハウスドルフ空間、$E'$ を双対、$E''$ を双双とする。 $E \subset E'' \subset {E'}^*$ があり、${E'}^*$ は $E'$ の代数双対です。 If $B$ is a bounded subset of $E$, its closure $\overline{B}$ in ${E'}^*$ endowed with $\sigma({E'}^*, E')$ is contained in $E''$: for, the polar $U = B^\circ$ of $B$ in $E'$ is a neighbourhood of 0 in $E'_b$, and we have $\overline{B} \subset U^\circ \subset E''$.

### 2. 半反射型空間

#### 定義 2 {#evt-iv-s2-def-2 .statement tag=07SD}

— $E$ を局所的に凸な空間とします。 $E$ から $E''$ への標準写像 $c_E$ が全単射である場合、$E$ は半再帰的であると言います。

これは、$E$ がハウスドルフであり、$E'$ 上のすべての線型形式は、強い位相 $\beta(E', E)$ に対して連続であり、形 $x' \mapsto \langle x, x' \rangle$ と $x \in E$ である、つまり、弱い位相 $\sigma(E', E)$ に対して連続であることを意味します。

#### 定理 1 {#evt-iv-s2-thm-1 .statement tag=07SE}

— 局所的に凸なハウスドルフ空間は、$E$ のすべての有界部分集合が弱化された位相 $\sigma(E, E')$ にとって比較的コンパクトである場合に限り、半再帰的になります。 $E$ が半反射的である場合、$E$ の強力なデュアル $E'_b$ はバレル化されます。

2 番目の主張はプロップから続きます。 3 (IV、p. 15)、および最初の位相と $E$ の弱められた位相の有界部分集合 (III、p. 27、cor. 3) の間の同一性。

To say that $E$ is semi-reflexive means that the topology on $E'_b$ is compatible with the duality between $E$ and $E'$, in other words, by Mackey's theorem (IV, p. 2, th. 1) that the topology on $E'_b$ is coarser than $\tau(E', E)$ (and in fact is identical with it); by definition (IV, p. 2), this means that every closed, convex and bounded subset of $E$ is compact for $\sigma(E, E')$, and this is equivalent to saying that every bounded subset of E is relatively compact for $\sigma(E, E')$, because the closed convex envelope of a bounded subset of E is bounded (III, p. 3, prop. 1).

#### 系 {#evt-iv-s2-n2-cor-1 .statement tag=07SF}

— *E を局所凸半反射空間とします。 E のすべての閉じたベクトル部分空間 M は半再帰的です。さらに、$E'/M^\circ$ の強い位相 (M の双対とみなされる) は、E' の強い位相の商です。

B を M の有界部分集合とする。B は E で有界であり、M 上の弱められた位相 $\sigma(M, M')$ は $\sigma(E, E')$ (IV, p. 10, prop. 11) によって誘発されるため、$\sigma(M, M')$ を備えた M における B の閉包はコンパクトである。従って、 th までに。 1、M は半反射です。 系の最後の主張はプロップから続きます。 IV、p. 9 の 10 は、E のすべての閉じた、凸型、有界の部分集合の集合 $\mathscr{S}$ に適用されます。

#### 注意 1 {#evt-iv-s2-n2-rem-1 .statement tag=07SG}

E が半反射的であると仮定します。最初の位相に対して凸で、閉じていて有界である E のすべての部分集合は、位相 $\sigma(E, E')$ に対してコンパクトです (IV、p. 1、提案 1)。 *一方、無限次元ヒルバーシアン空間 E の単位元球面 (方程式 $\|x\| = 1$ による) は、初期位相に対して閉じて有界ですが、たとえ E が半反射的であっても、弱められた位相に対しては閉じません。 \*

#### 注意 2 {#evt-iv-s2-n2-rem-2 .statement tag=07SH}

IV、p. 5 の注意 3 までに、 を再定式化できます。 *ハウスドルフ空間 E は、弱化された位相に対して準完全である場合に限り、半再帰的です。* 半再帰的である場合、最初の位相* (IV、p. 5、注意 2) に対して *準完全です。

#### 注意 3 {#evt-iv-s2-n2-rem-3 .statement tag=07SI}

上記系、空間の仮説のもとでは、E/M は必ずしも半再帰的ではありません (IV、p. 63、演習 10)。

### 3. 反射的空間

#### 定義 3 {#evt-iv-s2-def-3 .statement tag=07SJ}

— *A locally convex space E is said to be reflexive if the canonical mapping $c_E$ from E into $E''$ is a topological vector space isomorphism from E onto the strong dual of $E'_b$.*

特に、再帰的空間は半再帰的であるため、ハウスドルフとなります。

#### 命題 4 {#evt-iv-s2-prop-4 .statement tag=07SK}

— *再帰的な空間の強い双対は再帰的です。*

これは def の直後に続きます。 3.

#### 定理 2 {#evt-iv-s2-thm-2 .statement tag=07SL}

— *局所的に凸なハウスドルフ空間 E が再帰的である位数において、それが樽型であり、E のすべての境界部分集合が弱められた位相 $\sigma(E, E')$ にとって比較的コンパクトであることが必要かつ十分です。

までに。 1 (IV, p. 15)、これは、E が *半再帰的かつバレル化されている*場合にのみ再帰的であるというというと同じです。

E が再帰的である場合、$E'_b$ は再帰的であり (提案 4)、その結果 E はバレル化されます (IV, p. 15, th. 1)。逆に、E が半再帰的でバレル型の場合、$c_E$ は全単射で、IV、p. 15、prop によって共連続になります。 2 であるため、E は再帰的です。

#### 注意 1 {#evt-iv-s2-n3-rem-1 .statement tag=07SM}

E を無限次元の実ヒルバーティアン空間とする。 F を、弱体化された位相を備えた空間 E とします。 空間 E と F は同じ二重 E' を持ち、E は再帰的バナッハ空間 (V, p. 17) です。従って、F は *半反射* になります。

ただし、E の強い位相と弱められた位相は別個であるため、F は *再帰的ではありません*。

#### 注意 2 {#evt-iv-s2-n3-rem-2 .statement tag=07SN}

E を再帰的空間とし、M を E の閉じたベクトル部分空間とします。M も E/M も再帰的空間ではない場合もあります (IV、p. 63、練習問題 10)。 \* 正規化空間の場合については、prop を参照してください。 IV、p. 17の7。 \*

### 4. 正規化空間の場合

E をノルム空間とします。 E の双対 E' 上の強い位相はノルムによって定義されます

(1)
$$
\|x'\| = \sup_{x \in E, \|x\| \leq 1} |\langle x, x' \rangle|,
$$
そして E の強い双対は Banach 空間 (III, p. 24, cor. 2) です。このとき、E の双対 E'' も、次のように定義されるノルムに対する Banach 空間です。

(2)
$$
\|x''\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x', x'' \rangle|.
$$

プロップにより。図 8、IV、p. 7 の (i)、標準線形写像 $c_E : E \to E''$ はアイソメトリです。今後は、*2 連 E''* の正規化された部分空間を使用して同一視する E とします。

#### 命題 5 {#evt-iv-s2-prop-5 .statement tag=07SO}

— *E を標準空間とし、E' を双対、E'' を双双とする。 E'' の (クローズされた) 単位元ボールは、弱い位相 $\sigma(E'', E')$ の E の単位元ボール B のクローズです。*

公式 (1) と (2) により、E'' の単位元ボールは B の双極子 $B^{\circ \circ}$ です。提案 5 は、双極子 (II、p. 45、cor. 3) の定理から続きます。

#### 注意 {#evt-iv-s2-n4-rem-1 .statement tag=07SP}

— Banach 空間 E は、強い位相に対しては二連 E'' で閉じていますが、弱い位相に対しては密です (提案 5)。

規範化された空間が *再帰的*であるという位数では、それが *半再帰的 * であることが必要かつ十分です。なぜなら、E の最初の位相は常に E'' の強い位相によって引き起こされるからです。 Th. 1 (IV, p. 15) は次の結果を意味します。

#### 命題 6 {#evt-iv-s2-prop-6 .statement tag=07SQ}

— *規範的な空間 E が反射的である位数において、E の単位元ボールが弱化された位相 $\sigma(E, E')$ にとってコンパクトであることが必要かつ十分です。*

再帰的ノルム空間が完全であるため Banach 空間であり、その双対が prop による再帰的 Banach 空間であることが観察されます。 IV、p. 16 の 4 つ。

#### 命題 7 {#evt-iv-s2-prop-7 .statement tag=07SR}

— *E を再帰的バナッハ空間とし、M を E の閉じたベクトル部分空間とします。すると、M と E/M は再帰的バナッハ空間となります。*

E' を E の双対、および E' における M の直交を $M^\circ$ とします。規範的な空間として、M の双対 $M'$ により同一視できる空間 $E'/M^\circ$ となります (IV、p. 9、提案 10)。 M は半再帰的 (IV、p. 16、系) なので再帰的であり、従って $E'/M^\circ$ も同様です。同様に、$M^\circ$ は再帰的であり、二重の $E/M^{\circ \circ} = E/M$ も同様です。

#### 例 {#evt-iv-s2-n4-exa-1 .statement tag=07SS}

— 1) $\ell^\infty(\mathbf{N})$ を、有界スカラー 数列 $x = (x_n)_{n \in \mathbf{N}}$ の Banach 空間を、ノルムで表すものとします。

(3) $$
\| \mathbf{x} \| = \sup_{n \in \mathbf{N}} |x_n| \quad (\text{I, p. 4}) .
$$

Let $c_0(\mathbf{N})$ be the closed vector subspace of $\ell^\infty(\mathbf{N})$ consisting of sequences tending to 0. 最後に、$\ell^1(\mathbf{N})$ を合計可能な数列のベクトル空間とし、ノルムを付与します。

(4) $$
\| \mathbf{x} \|_1 = \sum_{n \in \mathbf{N}} |x_n| .
$$

次のような方法で、$c_0(\mathbf{N})$ の双対が $\ell^1(\mathbf{N})$ と同一視できることを示すことができます (IV、p. 47、練習問題 1)。

(5) $$
\langle \mathbf{x}, \mathbf{x}' \rangle = \sum_{n \in \mathbf{N}} x_n x'_n
$$

すべての $\mathbf{x} \in c_0(\mathbf{N})$ と $\mathbf{x}' \in \ell^1(\mathbf{N})$ に対して。同様に、$\ell^1(\mathbf{N})$ の双対は、すべての $\mathbf{x} \in \ell^1(\mathbf{N})$ とすべての $\mathbf{x}' \in \ell^\infty(\mathbf{N})$ に対して関係 (5) が得られるように、$\ell^\infty(\mathbf{N})$ と識別できます。従って、$\ell^\infty(\mathbf{N})$ は $c_0(\mathbf{N})$ の二双対であり、この後者の空間は再帰的ではありません。

\* 2) すべてのヒルバーティアン空間は再帰的バナハ空間 (V, p. 17) です。
\* 3) X をハウスドルフ位相幾何学空間とし、$\mu$ を X の複素測度とする。すべての実数 $p > 1$ に対して、バナッハ空間 $L^p(X, \mu)$ は再帰的であり、その双対は $p^{-1} + q^{-1} = 1$ を伴う $L^q(X, \mu)$ と識別できます (INT、V、第 2 版、§ 5, No. 8 および IX, § 1, No. 10)。

### 5. モンテル空間

#### 定義 4 {#evt-iv-s2-def-4 .statement tag=07ST}

*すべての有界部分集合が比較的コンパクトである、局所的に凸のハウスドルフおよび樽型空間は、モンテル空間と呼ばれます。*

#### 例 1 {#evt-iv-s2-n5-exa-1 .statement tag=07SU}

すべての有限次元ハウスドルフ空間はモンテル空間です。モンテル空間であるノルム空間は局所的にコンパクトであるため、有限次元 (I, p. 15, th. 3) です。

#### 例 2 {#evt-iv-s2-n5-exa-2 .statement tag=07SV}

記法と仮定のプロップ付き。 III、p. 6、空間 E の 7 は、バナッハ空間の帰納的極限であり、バレル (III、p. 25) です。さらに、E のすべての有界部分集合は比較的コンパクトです (III、p. 6、提案 7)。他の語では、Eはモンテル空間です。特にジュヴレ空間(III、p. 10)はモンテル空間です。 \* これは、$\mathbf{C}^n$ (III, p. 10) のコンパクト部分集合 K の近傍における写像分析の細菌の空間 $\mathscr{H}(K)$ からなるに当てはまります。*

#### 例 3 {#evt-iv-s2-n5-exa-3 .statement tag=07SW}

$E_n$ がすべての n について $E_{n+1}$ で閉じられるような、モンテル空間 (II, p. 33) の数列 $(E_n)$ のすべての厳密な帰納極限 E は、モンテル空間です。実際、E はハウスドルフ (II, p. 32, prop. 9 (i))、バレル (III, p. 25, cor. 3) であり、E のすべての有界部分集合は $E_n$ (III, p. 5, prop. 9 (i)) の 1 つに含まれます。 6) 従って、$E_n$ では比較的コンパクトであり、その結果 E でも同様です。

#### 例 4 {#evt-iv-s2-n5-exa-4 .statement tag=07SX}

\* U を $\mathbf{R}^n$ の開集合とし、$\mathscr{C}^\infty(U)$ を U 上の無限微分可能な写像 (III, p. 9) のフレシェ空間とします。これがモンテル空間であることを証明してみます。 $\mathscr{C}^\infty(U)$はフレシェ空間なので樽詰め(III、p. 25、系)です。 B を $\mathscr{C}^\infty(U)$ の有界部分集合とし、K を U のコンパクト部分集合とします。$f$ が B を通過するので、すべての $\alpha \in \mathbf{N}^n$ について、$H_{\alpha, K}$ を制限の集合から写像 $\partial^\alpha f$ とします。 $\alpha \in \mathbf{N}^n$; $|\beta| = |\alpha| + 1$、集合 $H_{\alpha, K}$ は、B が $\mathscr{C}^\infty(U)$ に制限されているため、$\mathscr{C}(K)$ に制限されるようなすべての $\beta \in \mathbf{N}^n$ に対して。 by VAR, R., No. 2.2.3, 集合 $H_{\alpha, K}$ は等連続であるため、(GT, X, § 2, No. 5) は $\mathscr{C}(K)$ で比較的コンパクトです。しかし、$\mathscr{C}^\infty(U)$の位相は、$\mathscr{C}^\infty(U)$から$\mathscr{C}(K)$までのすべての写像$f \mapsto \partial^\alpha f|K$が連続しているトポロジの中で最も粗いため、Bは$\mathscr{C}^\infty(U)$では比較的コンパクトです（GT、I, § 4, No. 1、prop.3と§ 9, No. 5、系）。

同様に、U* (III, p. 9) * でのコンパクトサポートを備えたすべての無限微分可能な写像の *空間 $\mathscr{C}_0^\infty(U)$ はモンテル空間* です。なぜなら、$\mathscr{C}_0^\infty(U)$ はフレシェ空間 (III, p. 9) の数列 $\mathscr{C}_{H_n}^\infty(U)$ の厳密な帰納極限であり、空間 $\mathscr{C}_{H_n}^\infty(U)$ のそれぞれがモンテルであることがわかるだけで十分だからです。 空間 (*例 3*)。しかし、$\mathscr{C}_0^\infty(U)$ の有界で閉じた部分集合は、$\mathscr{C}^\infty(U)$ で閉じて有界であるため、$\mathscr{C}^\infty(U)$ でコンパクトになり、その結果、$\mathscr{C}_{H_n}^\infty(U)$ でコンパクトになります。 \*

#### 命題 8 {#evt-iv-s2-prop-8 .statement tag=07SY}

*E をモンテル空間および $\mathfrak{T}$ を E 上のフィルターとし、弱化された位相の E で点 $x_0$ に収束します。 $\mathfrak{T}$ が可算基底であるか、含むが有界集合である場合、$\mathfrak{T}$ は、最初の位相についても $x_0$ に収束します。*

まず、$\mathfrak{T}$ に有界の集合 $\overline{B}$ が存在すると仮定します。 E の最初の位相に対する B の閉包 $\overline{B}$ は有界です。 加法では、Eはモンテル空間なので、$\overline{B}$はコンパクトです。 $\sigma(E, E')$ によって誘導された $\overline{B}$ 上の位相はハウスドルフであり、最初の位相によって誘導された位相よりも粗いです。従って、それらは一致する (GT、I, § 9, No. 4) になります。この場合、これは命題を証明します。

次に、$\mathfrak{T}$ に可算数の基底があるとします。 (GT、I, § 6, No. 8、提案 11) 数列 $(x_n)_{n \geq 1}$ が $\sigma(E, E')$ に対して $x_0$ になる傾向がある場合を考慮するだけで十分です。 B を、$n \geq 0$ に対するすべての $x_n$ の集合とします。この集合は $\sigma(E, E')$ に制限されており、したがって最初の位相 (III、p. 27、cor. 3) も制限されています。従って、証明の最初のケースに戻りました。

*すべてのモンテル空間は再帰的です*: これは def から続きます。 4 番目から。 IV、p. 16の2つ。さらに:

#### 命題 9 {#evt-iv-s2-prop-9 .statement tag=07SZ}

*モンテル空間の強力なデュアルはモンテル空間です。*

E をモンテル空間と $E'_b$ の強力な双対とします。 E は再帰的であるため、$E'_b$ はバレル化されます (IV, p. 15, th. 1)。 E のすべての有界部分集合は比較的コンパクトであるため、$E'$ 一致する上の強力な位相はコンパクトな収束の位相となります。 B を $E'_b$ の有界部分集合とします。それは弱い位相 $\sigma(E', E)$ に限定されており、従って E がバレル化されているため等連続です。次に、Ascoli の定理 (GT、X, § 2, No. 4、cor. および § 2, No. 5、cor. 1) は、$\sigma(E', E)$ に対する B の閉包がコンパクト収束の位相に対してコンパクトであることを意味します。従って、B は $E'_b$ で比較的コンパクトです。

#### 命題 10 {#evt-iv-s2-prop-10 .statement tag=07T0}

*すべての計量可能なモンテル空間は、可算性の最初の公理を満たします。*

E を計量化可能なモンテル空間とします。 E が正規化空間の積の部分空間数列の $F = \prod_{n \in \mathbf{N}} F_n$ と同一視できること (II, p. 5) がわかっており、すべての $n \in \mathbf{N}$ に対して $\mathrm{pr}_n(E) = F_n$ があると仮定することもできます。計量可能空間 $F_n$ のそれぞれが可算性の最初の公理を満たす場合、F (GT, IX, § 2, No. 8) も満たされ、従って E も満たされます。

私たちは *不合理な還元* によって議論します。たとえば、$F_0$ が可算性の最初の公理満たすを満たさないと仮定します。 $B_0$ を $F_0$ の単位元ボール (クローズ) とします。これは計量空間であり、可算性の最初の公理満たすではありません。次の補題を使用します。

#### 補題 1 {#evt-iv-s2-lem-1 .statement tag=07T1}

*計量空間 X が可算性の最初の公理満たすを満たさないと仮定します。次に、X には実数 $\varepsilon > 0$ と数えられない部分集合 A が存在し、A 内のすべての異なる $x, y$ に対して $d(x, y) \geq \varepsilon$ が存在します。

すべての整数 $n \geq 1$ について、$\mathfrak{F}_n$ を X の部分集合 D の集合 (包含順) とし、D の異なる $x, y$ に対する $d(x, y) \geq \frac{1}{n}$ は有限です。 集合 $\mathfrak{F}_n$ は有限です指標、したがって、極大元 $D_n$ (S、III, § 4, No. 5) を所有します。次に、すべての $y \in X$ について、$D_n$ の最大値指標により、$d(x, y) < \frac{1}{n}$ となるように、$D_n$ には点 $x$ が存在します。

$D = \bigcup_n D_n$を入れてください。 集合 D は X で密であり、X は可算性の最初の公理である満たすを満たさないため、D は可算でなく、したがって $D_n$ の 1 つは可算ではありません。

Q.E.D.

$B_0$ に適用される補題 1 までに、$F_0$ と数 $\varepsilon > 0$ の数えられない部分集合 $A_0$ が存在し、$\|x\| \leq 1$ と $\|x - y\| \geq \varepsilon$ が別個の $x, y$ に対応します。 $A_0$。 $\mathrm{pr}_0(E) = F_0$ があるので、E には部分集合 A が存在し、A から $A_0$ まで $\mathrm{pr}_0$ 誘導する全単射になります。

#### 補題 2 {#evt-iv-s2-lem-2 .statement tag=07T2}

*A の別個の元の数列 $(x_m)_{m \geq 0}$ からなるが存在し、E で囲まれています。*

A の点を帰納法までに構成する数列 $(x_m)_{m \geq 0}$ とします。および減少列 $(C_m)_{m \geq 0}$ の部分集合の満たす次の条件 :
a) 集合 $C_m$ はどれも数えられません。
b) すべての $n \geq 0$ に対して、集合 $\mathrm{pr}_k(C_m)$ は $0 \leq k \leq m$ に対して $F_k$ で制限されます。
c) $m \geq 0$ ごとに、$x_m \in C_m - C_{m+1}$ があります。

$C_0 = A$を入れます。 $0 \leq m \leq n$ の集合 $C_m$ が、$0 \leq m \leq n$ の満たす a) および b) と、$0 \leq m < n$ の $C_m - C_{m+1}$ の点 $x_m$ が定義されているとします。すべての整数 $r \geq 1$ について、$C_{n,r}$ をすべての $x \in C_n$ の集合とします。

$$
r - 1 \leq \| \mathrm{pr}_{n+1}(x) \| < r .
$$

$C_n$ は数えられないので、$C_{n,r}$ が数えられないような整数 $r \geq 1$ が存在します。 $C_{n,r}$ に選ぶ点 $x_n$ を入れ、$C_{n+1} = C_{n,r} - \{ x_n \}$ を入れます。明らかに、$C_{n+1} \subset C_n$ と $x_n \in C_n - C_{n+1}$、集合 $C_{n+1}$ は数えられず、$\mathrm{pr}_k(C_{n+1})$ は $0 \leq k \leq n + 1$ に対して $F_n$ に制限されます。

$x_m \in C_m$があるので、$m \geq n$が$x_m \in C_n$になります。したがって、$F_n$ 上の数列 $(x_m)_{m \geq 0}$ の射影は、すべての $n \geq 0$ に対して制限されます。他の語、数列 $(x_m)_{m \geq 0}$ は E で制限されており、これにより補題 2 が確立されます。

Q.E.D.

補題 2 の記法では、有界数列 $(x_m)_{m \geq 0}$ は E に極限点 $y$ を持ちます。 したがって、数列 $(\mathrm{pr}_0(x_m))_{m \geq 0}$ は極限点になります。 $F_0$の$\mathrm{pr}_0(y)$ですが、これは$A_0$の矛盾する構成です。

#### 系 {#evt-iv-s2-n5-cor-1 .statement tag=07T3}

— E を計量化可能なモンテル空間とします。そして、E の強い双対には可算密集集合が存在します。

E の双対 E' では、E はモンテル空間であるため、強い位相はコンパクトな収束のそれと同一です。これで、cor を適用するだけで十分です。プロップの1。 III、p. 18の6。

E が無限次元である場合、計量可能モンテル空間 E の強い双対は計量可能ではないことを示すことができます (IV、p. 57、例題 1)。

### 練習問題 {#evt-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
