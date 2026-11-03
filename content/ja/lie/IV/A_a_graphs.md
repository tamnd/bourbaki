---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 0
section_title: Graphs
appendix: true
lang: ja
source: lie-iv-vi
pdf_pages: 0040-0043
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS
      page: 0
      pdf_page: 40
    - "no": 2
      title: CONNECTED COMPONENTS OF A GRAPH
      page: 0
      pdf_page: 40
    - "no": 3
      title: FORESTS AND TREES
      page: 0
      pdf_page: 42
statements: 6
exercises: 0
content_sha256: 8dd983060769b299988f507f612dee6c8312a3026e389facbf373aa6a66ef843
translated_from: content/en/lie/IV/A_a_graphs.md
translation_method: google
source_content_sha256: 7fa7ab5ecf248630c43ab97ab1126594432fdccc1695b2f5d4ac5a3b570217ea
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e5c132045a274457ac05c7b4cb155259acf66c59c30d53c5a2c2720a6feb9e07
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録
# グラフ

### 1. 定義

#### 定義 1 {#lie-iv-a0-def-1 .statement tag=0AOV}

*組み合わせグラフ (または、混乱の危険がない場合は単にグラフ) は対* $(\mathbf{A}, S)$、*ここで S は集合、A は $\mathfrak{P}(S)$ のからなるのうち集合の部分集合と 2 つの元です。*

$\Gamma = (\mathbf{A}, S)$ をグラフとします。 $\mathbf{A}$ の元は *エッジ* と呼ばれ、S のそれらは $\Gamma$ の *頂点* と呼ばれます。 $\{x, y\}$ がエッジの場合、2 つの頂点は *結合* されていると言われます。頂点が最大 1 つの頂点に結合されている場合、頂点は *ターミナル* と呼ばれ、少なくとも 3 つの頂点に結合されている場合は *分枝点* と呼ばれます。

一般的な定義 (*集合 R*, §8) によれば、グラフ $\Gamma$ からグラフ $\Gamma' = (\mathbf{A}', S')$ までの *同型* は、S から S' まで全単射で、$\mathbf{A}$ から $\mathbf{A}'$ かかります。 $S' \subset S$ と $\mathbf{A}' \subset \mathbf{A}$ の場合、グラフ $\Gamma' = (\mathbf{A}', S')$ は $\Gamma$ の *サブグラフ* と呼ばれます。 $S' \subset S$ と $\mathbf{A}' = \mathbf{A} \cap \mathfrak{P}(S)$ の場合、$\Gamma$ は $\Gamma$ の *完全な部分グラフ* と呼ばれます。 S のすべての部分集合が、$\Gamma$ の 1 つの完全な部分グラフの頂点の集合であることは明らかです。

引数を理解しやすくするために、頂点に点対応するをもつ図式によってグラフを表し、それらが表す頂点がグラフ内で結合されている場合にのみ、2 つの点が線で結合されます。たとえば、図式

![頂点 a、b、c、d、e と辺 {a, b}、{b, c}、{c, d}、{c, e} を持つグラフの図式](https://i.imgur.com/3Q5z5QG.png)

は頂点が$a, b, c, d, e$、辺が$\{a, b\}, \{b, c\}, \{c, d\}$と$\{c, e\}$であるグラフを表します。

### 2. グラフの成分を接続しました

$\Gamma = (\mathbf{A}, S)$ をグラフにします。 $a$と$b$が2つの頂点である場合、$a$と$b$を結ぶ*パス*は、$\Gamma$の頂点と$x_0 = a, x_n = b$、頂点$x_i$と$x_{i+1}$を結ぶ数列$(x_0, \ldots, x_n)$になります。 $0 \leq i < n$ に参加中です。 整数 $n \geq 0$ はパスの *長さ* です。パス $(x_0, \ldots, x_n)$ は、$x_i \neq x_j$ の場合、$i \neq j$ の場合は単射的であると言われます。 $a$ と $b$ を結合するパス $(x_0, \ldots, x_n)$ がそのようなパスの中で最小の長さである場合、それは必然的に単射的です。なぜなら、そうでない場合は、$i$と$j$が$0 \leq i < j \leq n$と$x_i = x_j$、そして数列が存在することになるからです。

$$
(x_0, \ldots, x_i, x_{j+1}, \ldots, x_n)
$$

$a$ と $b$ を結合する長さ $< n$ のパスになります。

関係「$\Gamma$」の2つの頂点$a$と$b$の間に「$a$と$b$を結ぶパスが存在します」は、頂点の集合$S$上の同値関係$R$です。 $R$ の同値類は、$\Gamma$ の *接続された成分* と呼ばれます。そして、$S$ に接続されている成分が最大 1 つある場合、つまり $\Gamma$ の任意の 2 つの頂点が少なくとも 1 つのパスで結合できる場合、$\Gamma$ は *接続されている* と言われます。

#### 命題 1 {#lie-iv-a0-prop-1 .statement tag=0AOW}

*$\Gamma = (A, S)$ をグラフとし、$(S_\alpha)_{\alpha \in L}$ を接続された成分のファミリーとします。 $S_\alpha$ を頂点の集合とする $\Gamma$ の完全な部分グラフを $\Gamma_\alpha$ で表します。

(i) *$L$の任意の$\alpha$について、グラフ$\Gamma_\alpha$が接続されます。*
(ii) *$\Gamma' = (A', S')$ が $\Gamma$ の接続された部分グラフである場合、$\Gamma' \subset \Gamma_\alpha$ のように $L$ に $\alpha$ が存在します。
(iii) *$\alpha \neq \beta$ の場合、$S_\alpha$ の元は、$S_\beta$ のどの元にも$\Gamma$ で結合されません (同様に、$\Gamma$ のすべてのエッジは、$\Gamma_\alpha$ のいずれかのエッジになります)。
(iv) *$(S'_\lambda)_{\lambda \in M}$を$S$の分割とし、$\lambda \neq \mu$の場合、$S'_\lambda$の元が$S'_\mu$の元に$\Gamma$で結合されないようにします。この場合、それぞれの集合 $S'_\lambda$ は、$\Gamma$ の成分の和集合となります。*

(i) $\alpha$ が $L$ にあり、$a$ と $b$ が $S_\alpha$ にあるとします。そして、$\Gamma$には$a$と$b$を結ぶパス$c = (x_0, \ldots, x_n)$が存在します。 $0 \leq i \leq n$ を含む任意の $i$ の場合、パス $(x_0, \ldots, x_i)$ は $\Gamma$ で $a$ と $x_i$ を結合するため、$x_i \in S_\alpha$ になります。したがって、$c$ は、$a$ と $b$ を結合する $\Gamma_\alpha$ 内のパスです。 $\Gamma_\alpha$ が接続されることになります。

(ii) $\Gamma' = (A', S')$ を $\Gamma$ の空でない接続された部分グラフとし、$a$ を $S'$ の元とし、$S_\alpha$ を $S$ 含む $a$ の接続された成分とします。 $S'$ の任意の $b$ については、$\Gamma'$ の $a$ と $b$、および $\Gamma$ の *なおさら* を結合するパス $c$ が存在します。 $S' \subset S_\alpha$ となります。

(iii) $L$ の個別の元 $\alpha$ と $\beta$、および頂点 $a \in S_\alpha$ と $b \in S_\beta$ が与えられると、$a$ と $b$ を結ぶパスは存在せず、特に $a$ と $b$ を結ぶエッジは存在しません。

(iv) $a$ を $S'_\lambda$ に置き、$S_\alpha$ を $\Gamma$ 含む $a$ の接続された成分とします。次に、$S_\alpha$ の任意の $b$ については、$\Gamma$ の $a$ と $b$ を結ぶパス $(x_0, \ldots, x_n)$ が存在します。 $i$ が $0 \leq i < n$ となる整数である場合、および $x_i \in S'_\lambda$ である場合、$x_i$ が $x_{i+1}$ に結合されるため、$x_{i+1} \in S'_\lambda$ になります。 帰納法の後には $0 \leq i \leq n$ の $x_i \in S'_\lambda$ が続き、特に $b = x_n$ は $S'_\lambda$ にあります。したがって、$S_\alpha \subset S'_\lambda$。

#### 系 1 {#lie-iv-a0-prop-1-cor-1 .statement tag=0AOX}

*グラフ $\Gamma = (A, S)$ は、$S$ の 2 つの空でないサブセットへのパーティション $(S', S'')$ が存在しない場合に限り、$S'$ の要素が $\Gamma$ の $S''$ の要素に結合されない場合にのみ接続されます。

$\Gamma$ が接続されていないと仮定し、$S'$ を接続されている成分の 1 つとします。 集合 $S'' = S - S'$ は、提案 1、(i) により空ではなく、提案 1、(iii) により、$S'$ の元が $S''$ のどの元にも結合されません。

ここで、$\Gamma$ が接続されており、$(S', S'')$ が性質で示されている分割であるとします。提案 1、(iv) により、集合 $S'$ 含むの少なくとも 1 つは成分に接続されているため、$S' = S$ と $S'' = \varnothing$ は矛盾します。

#### 系 2 {#lie-iv-a0-prop-1-cor-2 .statement tag=0AOY}

*$S$ のサブセット $S'$ は、$S'$ に属する頂点が $S - S'$ に属する頂点に結合されていない場合に限り、接続されたコンポーネントの結合になります。*

提案 1 (iv) により、条件で十分です。提案1の(iii)により必要となります。

### 3. 森と木々

$\Gamma = (A, S)$ をグラフとします。 $\Gamma$ の *回路* は数列

$$
(x_1, \ldots, x_n)
$$

$n \geq 3$、$x_i$ が $1 \leq i < n$ の $x_{i+1}$ に結合され、$x_n$ が $x_1$ に結合されるように、$\Gamma$ の個別の頂点の。 $\Gamma$ に回路がない場合、$\Gamma$ は *フォレスト* と呼ばれます。 $\Gamma$ のすべての部分グラフも森になります。接続されたフォレストは *ツリー* と呼ばれます。したがって、森のつながった成分は木になります。

#### 命題 2 {#lie-iv-a0-prop-2 .statement tag=0AOZ}

*$\Gamma = (A, S)$ を、有限の数個の頂点のみを持つ森とします。*

(i) *$\Gamma$ に少なくとも 1 つの頂点がある場合、終端頂点があります。*
(ii) *$\Gamma$ に少なくとも 2 つの頂点がある場合、その頂点セットの 2 つの空でないサブセットへの分割 $(S', S'')$ が存在し、両方とも $S'$ に属するか、両方とも $S''$ に属する 2 つの異なる頂点が結合されることはありません。

$\Gamma$ に少なくとも 1 つの頂点があり、$(x_0, \ldots, x_n)$ を $\Gamma$ の最大長さの単射パスとします。頂点 $x_0$ できないは、$x_0, x_1, \ldots, x_n$ とは異なる頂点 $y$ に結合されます。そうしないと、長さ $n + 1$ の $\Gamma$ 、つまり $(y, x_0, \ldots, x_n)$ に単射パスが存在することになります。頂点 $x_0$ は、頂点 $x_i$ と $2 \leq i \leq n$ で結合されていません。そうしないと、$(x_0, x_1, \ldots, x_i)$ が森 $\Gamma$ 内の回路になってしまうからです。したがって、$x_0$ はターミナルです。

(ii) を、$\Gamma$ の頂点の数 $m$ の帰納法によって証明します。$m = 2$ の場合は自明です。次に、$m - 1$ 頂点を持つグラフに対して $m \geq 3$ と主張 (ii) が証明されたとします。 $a$を$\Gamma$(cf.(i))の終端頂点とする。 $\Gamma$ の頂点 $x \neq a$ を頂点とする $\Gamma$ の部分グラフ全体に帰納法の仮定を適用します。したがって、$S'_1 \cup S''_1 = S - \{a\}$ を持つ $S$ の 2 つの空ではない互いに素部分集合 $S'_1$ と $S''_1$ が存在し、$S'_1$ (それぞれ $S''_1$) の 2 つの異なる頂点が結合されることはありません。 $a$ は $\Gamma$ の最大 1 つの頂点に結合しているため、たとえば、$S'_1$ のどの頂点にも結合していないと仮定できます。 分割 $(S'_1, S''_1 \cup \{a\})$ には、必要な性質が含まれます。 Q.E.D.

任意の整数 $n \geq 1$ について、頂点が整数 $1, 2, \ldots, n$ で、辺が対 $\{i, j\}$ と $i - j = \pm 1$ であるグラフを $A_n$ で表します。

$$
\begin{array}{cccccc}
1 & 2 & 3 & n-1 & n \\
\circ & \circ & \circ & \cdots & \circ
\end{array}
$$

グラフ $\Gamma$ が $A_{m+1}$ と同型であれば、長さ $m \geq 0$ の連鎖であると言われます。 これは、単射パス $(x_0, \ldots, x_m)$ 含むのすべての頂点が $\Gamma$ に存在し、$|i - j| > 1$ の場合、頂点 $x_i$ と $x_j$ が結合されていないことに相当します。

#### 命題 3 {#lie-iv-a0-prop-3 .statement tag=0AP0}

*グラフは、その頂点の数が有限で非ゼロであり、分岐点のないツリーである場合にのみチェーンです。*

グラフ $\Gamma$ が、提案 3 の前に主張にリストされたプロパティを持つチェーン $(x_0, \ldots, x_m)$ であると仮定します。$\Gamma$ の任意の頂点が最大 2 つの頂点に結合していることは明らかです。 $i < j$ の場合、パス $(x_0, \ldots, x_m)$ から抽出されたパス $(x_i, \ldots, x_j)$ が $x_i$ と $x_j$ を結合します。したがって、$\Gamma$ が接続されます。最後に、$(x_{p_1}, \ldots, x_{p_n})$を$\Gamma$の回路とし、$p_k$を相異なる整数$p_1, \ldots, p_n$の最小のとします。 $x_{p_k}$ が $x_{p_i}$ と $x_{p_j}$ に結合されるように、別個の添字 $i$ と $j$ が存在します。これは回路の定義から続きます。 $p_k < p_i$ と $p_k < p_j$ があるため、必然的に $p_i = p_j = p_k + 1$ が存在しますが、$p_1, \ldots, p_n$ は別個であるため、これは矛盾します。したがって、$\Gamma$には回路はありません。

逆に、$\Gamma$ を分岐点がなく、有限の非ゼロの頂点数を持つ木とし、$(x_0, \ldots, x_m)$ を $\Gamma$ の最大長さの単射パスとします。 $x_0, \ldots, x_m$以外の頂点の$T$集合で表します。頂点 $b \in T$ できないは、任意の頂点 $x_i$ に結合されます。

a) $i = 0$ ですが、その場合、$(b, x_0, \ldots, x_m)$ は $\Gamma$ の長さ $m + 1$ の単射パスになります、または
b) $i = m$ ですが、その場合、$(x_0, \ldots, x_m, b)$ は $\Gamma$ の長さ $m + 1$ の単射パスになります、または
c) $0 < i < m$ ですが、その場合、$x_i$ は 3 つの異なる頂点 $x_{i-1}$、$x_{i+1}$、$b$ に結合されます。

$\Gamma$が接続されているため、Corにより$T$は空になります。さらに、$j - i > 1$と$x_i, x_j$を結合した$i, j$があると、$\Gamma$に回路$(x_i, x_{i+1}, \ldots, x_j)$ができます。したがって、$\Gamma$ はチェーンです。 Q.E.D.
