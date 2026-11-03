---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 8
section_title: Convergence of the Hausdorff series (ultrametric case)
lang: ja
source: lie-i-iii
book_pages: 170-176, 205-207
pdf_pages: 0188-0194, 0223-0225
extraction: ocr
subsections:
    - "no": 1
      title: $p$-adic upper bounds of the series exp, log and $\mathbf{H}$
      page: 171
      pdf_page: 189
    - "no": 2
      title: NORMED LIE ALGEBRAS
      page: 172
      pdf_page: 190
    - "no": 3
      title: GROUP DEFINED BY A COMPLETE NORMED LIE ALGEBRA
      page: 172
      pdf_page: 190
    - "no": 4
      title: EXPONENTIAL IN COMPLETE NORMED ASSOCIATIVE ALGEBRAS
      page: 174
      pdf_page: 192
statements: 9
exercises: 4
content_sha256: f0dd946116759dc4284b500afee5505226667fccc84cbb980e36f69630020d17
translated_from: content/en/lie/II/08_s8_convergence_of_the_hausdorff_series.md
translation_method: google
source_content_sha256: 4e23a56fb861bed945b01d7c816d0a6e594b96b17aad3c28c11640248838980a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 677e466803662ed1d9d6eafb6dd8ea388bc8cd01d0e246951f2fbe1cffe95d0b
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。ハウスドルフ系列の収束 (ウルトラメトリック ケース)

この段落では、K が標数0* の非離散 *完全値体であり、*超*絶対値値であると仮定します。 K の剰余体の特性 (*可換代数*, 章 VI, § 3, no. 2) を $p$ で表します。
$p \neq 0$ の場合、$a = |p|$ と書きます。私たちは (*可換代数*、章 VI, § 6、番号 2 と 3) $0 < a < 1$ と、K に $\mathbf{R}$ の値を持つ唯一の評価 $v$ が存在することを知っています。その制限から $\mathbf{Q}$ は、 $p$-進数評価 $v_p$ は、すべての $x \in K$ に対して $|x| = a^{v(x)}$ となります。また、次のようにも書きます。
(1) $\theta = \frac{1}{p-1}.$

$p = 0$ の場合、$a$ 実数で$0 < a < 1$ となり、$v$ で$\mathbf{R}$ に値を含む$\mathbf{K}$ の評価を表し、すべての$x \in \mathbf{K}$ について$|x| = a^{v(x)}$ となります (*loc. cit.*)。次に、$x \in \mathbf{Q}^*$の場合は$v(x) = 0$です。また、次のようにも書きます。
$$
\theta = 0.
$$

### 1. $p$-進数上界/系列 exp、log および $\mathbf{H}$

※このNo. $p \neq 0$.* と仮定します。

#### 補題 1 {#lie-ii-s8-lem-1 .statement tag=0A6Q}

*Let $n$ be an integer $\geqslant 0$ and let $n = n_0 + n_1 p + \cdots + n_k p^k$, with $0 \leqslant n_i \leqslant p - 1$, be the $p$-adic expansion of $n$. $S(n) = n_0 + n_1 + \cdots + n_k$ にしましょう。 それから*
$$
v_p(n!) = \frac{n - S(n)}{p - 1}.
$$
1 と $n$ の間の整数 $i$ の $v_p(n!) = \sum_{i=1}^n v_p(i)$ と数について、$v_p(i) \geqslant j$ は $n/p^j$ の積分部分 $[n/p^j]$ に等しい。 それから
$$
v_p(n!) = \sum_{j \geqslant 0} j ([n/p^j] - [n/p^{j+1}]) = \sum_{j \geqslant 1} [n/p^j].
$$
$[n/p^j] = \sum_{i \geqslant j} n_i p^{i-j}$、補題と続きます。

#### 補題 2 {#lie-ii-s8-lem-2 .statement tag=0A6R}

整数 $n \geqslant 1$ ごとに $v(n) \leqslant v(n!) \leqslant (n - 1)\theta$ と $v(n) \leqslant (\log n)/(\log p)$。
$v(n!) = v_p(n!) = (n - S(n))\theta \leqslant (n - 1)\theta$ by 補題 1.
一方、$n \geqslant p^{v(n)}$、よって $v(n) \leqslant (\log n)/(\log p)$。
$I = \{ U, V \}$ を 2 つの元の集合として、
$$
\mathbf{H} = \sum_{r,s \geqslant 0} H_{r,s}(U, V) \in \hat{\mathbf{L}}_{\mathbf{Q}}(I)
$$
ハウスドルフ系列 (§ 6, no. 4, 定義 1) になります。 Let $\mathbf{Z}_{(p)}$ be the local ring of $\mathbf{Z}$ relative to the prime ideal $(p)$ and $(e_b)_{b \in B}$ a basis of $\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$ over $\mathbf{Z}$ (§ 2, no. 11, Theorem 1). また、$\mathbf{Q}$ を超える $\mathbf{L}_{\mathbf{Q}}(I)$ の基底です。

#### 命題 1 {#lie-ii-s8-prop-1 .statement tag=0A6S}

*$r$ と $s$ を 2 整数 $\geqslant 0$ とします。 $\lambda_b \in \mathbf{Q}$ である $H_{r,s} = \sum_{b \in B} \lambda_b e_b$ が、基底 $(e_b)_{b \in B}$ に関して $\mathbf{H}$ の分解である場合、*
$$
v_p(\lambda_b) \geqslant -(r + s - 1)\theta \quad \text{for all } b \in B.
$$
環 $\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$ は、語 $w \in \mathrm{Mo}(I)$ によって生成された $\mathbf{A}_{\mathbf{Q}}(I)$ のサブ$\mathbf{Z}_{(p)}$ モジュールと識別されます。 $\mathbf{L}_{\mathbf{Z}_{(p)}}(I)$は$\mathbf{A}_{\mathbf{Z}_{(p)}}(I)$の直因子なので、
$$
\mathbf{L}_{\mathbf{Z}_{(p)}}(I) = \mathbf{A}_{\mathbf{Z}_{(p)}}(I) \cap \mathbf{L}_{\mathbf{Q}}(I).
$$

$f$ を整数とし、$f \leq (r + s - 1)\theta < f + 1$ とします。 関係 (4) は、すべての $b \in B$ に対する $v_p(\lambda_b) \geq -f$、つまり $H_{r,s} \in p^{-f}L_{\mathbf{Z}(p)}$ に相当します。ただし、これは$H_{r,s} \in p^{-f}A_{\mathbf{Z}(p)}(I)$に対して(5)でも等価です。

§ 6, no. 4 の公式 (11) までに、すべての整数 $m \geq 1$ とすべての整数 $r_1, \ldots, r_m, s_1, \ldots, s_m$ について、次のことが示されれば十分です。
$$
r_1 + \cdots + r_m = r, \quad s_1 + \cdots + s_m = s,
$$
$$
r_i + s_i \geq 1 \quad \text{for } 1 \leq i \leq m,
$$
私たちは持っています
$$
v_p(m!r!\ldots r_m!s_1!\ldots s_m!) \leq f.
$$
しかし、補題 2、$v_p(r_i!s_i!) \leq (r_i + s_i - 1)\theta$、$v_p(m!) \leq v_p(m!) \leq (m - 1)\theta$までには。したがって、(7) の左辺は上で次のように制限されます。
$$
\theta(m - 1 + \sum_{i=1}^m (r_i + s_i - 1)) = \theta(r + s - 1);
$$
整数であるため、$\leq f$ となり、証明が完成します。

### 2. ノルドリー代数

#### 定義 1 {#lie-ii-s8-def-1 .statement tag=0A6T}

*K* 上の正規化リー代数はノルムを伴うリー代数であり、次のようになります
$$
\|x + y\| \leq \sup(\|x\|, \|y\|)
$$
$$
\|[x, y]\| \leq \|x\| \cdot \|y\|
$$
$g$ のすべての $x, y$ に対して。

*この段落の残りの部分では、g は完全な標準リー代数を示します。*

有限の集合 I ごとに、 § 7, no. 1 のように定義するを$\hat{L}(I)$ の連続リー代数準同型 $u \mapsto \tilde{u}$ から $\hat{P}(g^I; g)$ にします。 § 7 のように、$v \in \mathbf{N}^I$ に対して $u_v \in L^v(I)$ を使用して $u = \sum_v u_v$ の場合、$\tilde{u} = \sum_v \tilde{u}_v$ になります。ここで、$\tilde{u}_v$ は、§ 2, no. 4 で定義された多項式写像 $(t_i)_{i \in I} \mapsto u_v((t_i))$ です。 合成公式 § 7, no. 1 の (2) は引き続き有効です。

### 3. 群は完全な規格リー代数によって定義されます

$H = \sum_{r, s \geq 0} H_{r,s} \in \hat{L}(\{U, V\})$ をハウスドルフ系列 (§ 6, no. 4, 定義 1) とします。 対応する形式的冪系列が連続成分であることを示します。
$$
\tilde{H} = \sum_{r, s \geq 0} \tilde{H}_{r,s} \in \hat{P}(g \times g, g)
$$
は収束します (*微分可能かつ解析的多様体*、R、4.1.1)。

$r \geq 0, s \geq 0$ を $r + s \neq 0$ となるようにし、$\| \tilde{H}_{r,s} \|$ を連続多項式 $\tilde{H}_{r,s}$ (微分可能および解析的多様体, R, 付録, no. 2) のノルムとします。

#### 補題 3 {#lie-ii-s8-lem-3 .statement tag=0A6U}

$$
\| \tilde{H}_{r,s} \| \leq a^{-(r+s-1)\theta}.
$$

B を I に対するホール集合とし、$H_{r,s} = \sum_{b \in B} \lambda_b e_b$ を $L(\{U, V\})$ の対応する基底に対して $H_{r,s}$ の分解とします。それから
$$
|\lambda_b| \leq a^{-(r+s-1)\theta}.
$$
これは、$p = 0$ や $\lambda_b \in \mathbf{Q}$ にとっては簡単です。そして、命題 1 of no. 1 から$p \neq 0$ が続きます。

さらに、
$$
\| \tilde{e}_b \| \leq 1 \quad \text{for } b \in B.
$$
より一般的には、$n$ の帰納法によって、2 つの次数 $n$ のすべての代替$b$ について、U と V (§ 2, no. 6)、$\| \tilde{b} \| \leq 1$ が決定されることを示します。 $n = 1$ の場合、$\tilde{b}$ は $g \times g$ の $g$ の射影の 1 つであるため、ノルム $\leq 1$ になります。 $n > 1$ の場合、$b = [b_1, b_2]$ となる次数 $< n$ の 2 つの代替案 $b_1$ と $b_2$ が存在します。 $g \times g$ から $g$ への写像 $\gamma : (x, y) \mapsto [x, y]$ はノルム $\leq 1$ の双線形であるため、 (微分可能および解析的多様体, R, 付録, no. 4)
$$
\| \tilde{b} \| = \| \gamma \circ (\tilde{b}_1, \tilde{b}_2) \| \leq \| \tilde{b}_1 \| \cdot \| \tilde{b}_2 \| \leq 1.
$$
関係 (11) と (12) は補題を暗示します。

#### 命題 2 {#lie-ii-s8-prop-2 .statement tag=0A6V}

形式的な冪系列 $\tilde{H}$ は収束する系列 (微分可能および解析的多様体、R、4.1.1)。 G がボール $\{ x \in g \mid \| x \| < a^\theta \}$ である場合、$\tilde{H}$ の絶対収束領域 (微分可能および解析多様体、R、4.1.3) 含む $G \times G$。

$u$ と $v$ が 2 つの実数 $> 0$ で、$u < a^\theta$ と $v < a^\theta$ である場合、(補題 3)
$$
\| \tilde{H}_{r,s} \| u^r v^s \leq a^\theta (u a^{-\theta})^r (v a^{-\theta})^s
$$
そして、$r + s$ が無限大になる傾向があるとき、$\| H_{r,s} \| u^r v^s$ は 0 になる傾向があります。

$\tilde{H}$、つまり公式によって定義された解析的写像 (微分可能および解析的多様体、R、4.2.4) を $h : G \times G \to g$ で表します。
$$
h(x, y) = \sum_{r, s \geq 0} \tilde{H}_{r,s}(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y) \quad \text{for } (x, y) \in G \times G.
$$
この写像は、$g$のハウスドルフ写像と呼ばれます。

$(x, y) \in G \times G$ にしましょう。それから
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \sup(\| x \|, \| y \|) \\
\| h(x, y) \| \leq \sup(\| x \|, \| y \|).
$$

(17) は (16) の直後に続き、(16) は $r = s = 0$ にとって自明です。 $r \geq 1$ の場合、
$$
\| \tilde{H}_{r,s}(x, y) \| \leq \| \tilde{H}_{r,s} \| \| x \|^{r} \| y \|^{s}
$$
$$
\leq \| x \| \left( \frac{\| x \|}{a^{\theta}} \right)^{r-1} \left( \frac{\| y \|}{a^{\theta}} \right)^{s}
$$
$$
\leq \| x \|;
$$
$s \geq 1$ の場合も同様に議論します。

特に、$(x, y) \in G \times G$の$\| h(x, y) \| < a^{\theta}$。

#### 命題 3 {#lie-ii-s8-prop-3 .statement tag=0A6W}

※$G$をボール$\{ x \in g | \| x \| < a^{\theta} \}$とします。分析家写像*
$$
h : G \times G \to G
$$
*$G$ を群にします。ここで、$0$ は単位元で、$-x$ はすべての $x \in G$ の $x$ の逆数です。さらに、$R$ が実数で、$0 < R < a^{\theta}$ になる場合、ボール*
$$
\{ x \in g | \| x \| < R \}
$$
*(それぞれ $\{ x \in g | \| x \| \leq R \}$) は $G$* のオープン部分群です。

$H(U, -U) = 0$ と $H(0, U) = H(U, 0) = U$、$h(x, -x) = 0$ および
$$
h(0, x) = h(x, 0) = x
$$
$x \in G$ 全員のために。したがって、結合性公式を証明することはまだ残っています。
$$
h(h(x, y), z) = h(x, h(y, z)) \quad \text{for } x, y, z \text{ in } G.
$$
として
$$
H(H(U, V), W) = H(U, H(V, W))
$$
$\hat{L}(\{ U, V, W \})$ (§ 6, no. 5, 命題 4) では、
$$
\tilde{H} \circ (\tilde{H} \times \mathrm{Id}_g) = \tilde{H} \circ (\mathrm{Id}_g \times \tilde{H})
$$
$\hat{P}(g \times g \times g; g)$ (no. 2) および (19) は、(18) by (16) および *微分可能および解析的多様体*、R、4.1.5 を意味します。

※他の語(章III, § 1)、ハウスドルフ写像との$G$はリー群です。

### 4. 完全ノルム結合における指数関数代数

このNo. A は、ノルム $x \mapsto \| x \|$ 満たす条件との単位結合代数を表します。
$$
\| x + y \| \leq \sup(\| x \|, \| y \|) \\
\| xy \| \leq \| x \| \cdot \| y \| \\
\| 1 \| = 1
$$

$A$の$x, y$は、このノルムで*完備*します。 § 7, no. 3 の 2 番目と 3 番目の段落の結果は引き続き有効です。

$I = \{ U \}$ をとり、$\hat{P}(A; A)$ の系列 $e(U) = \sum_{n \geq 1} \frac{U^n}{n!}$ と $l(U) = \sum_{n \geq 1} (-1)^{n-1} \frac{U^n}{n}$ の像 $\tilde{e}$ と $\tilde{l}$ を検討します。次に:

$$
\left\| \left( \frac{U^n}{n!} \right)^{\sim} \right\| \leq a^{-(n-1)\theta}
$$
$$
\left\| \left( \frac{U^n}{n} \right)^{\sim} \right\| \leq a^{-\frac{\log n}{\log p}}
$$

補題 2/no. 1 作。したがって、系列 $\tilde{e}$ (それぞれ $\tilde{l}$) の *絶対収束の半径* は $\geq a^\theta$ (それぞれ $\geq 1$) です (*微分可能および解析的多様体*、R、4.1.3)。 $R > 0$ の場合は、$G_R = \{ x \in A \mid \|x\| < R \}$ とします。 $G = G_0$と書きます。 系列 $\tilde{e}$ (それぞれ $\tilde{l}$) 定義する写像 $e_A$ (それぞれ $l_A$) の $G$ (それぞれ $G_1$) を $A$ に変換します。私たちはこう書きます：
$$
\exp_A(x) = 1 + e_A(x) = \sum_{n \geq 0} \frac{x^n}{n!} \quad \text{for } x \in G
$$
$$
\log_A(x) = l_A(x-1) = \sum_{n \geq 1} (-1)^{n-1} \frac{(x-1)^n}{n} \quad \text{for } x-1 \in G_1'
$$
(混乱が生じない場合は、添字 $A$ を省略します)。 $x \in G_R$と$n \geq 1$の場合、
$$
\left\| \frac{x^n}{n} \right\| \leq \left\| \frac{x^n}{n!} \right\| < R^n a^{-(n-1)\theta} = R \left( \frac{R}{a^\theta} \right)^{n-1}
$$
したがって、$e_A(G_R) \subset G_R$、$l_A(G_R) \subset G_R$ は $R \leq a^\theta$ になります。

#### 命題 4 {#lie-ii-s8-prop-4 .statement tag=0A6X}

*$R$ を実数として、$0 < R \leq a^\theta$ とします。 写像 $\exp_A$ 定義する $G_R$ の $1 + G_R$ に対する分析同型と逆同型は、$\log_A$ から $1 + G_R$ の制限です。

$e(l(X)) = l(e(X)) = X$。 (20)、(21) および *微分可能および分析多様体*、R、4.1.5 により、$x \in G_R$ に対して $e_A(l_A(x)) = l_A(e_A(x))$ が推定されます。それから
$$
\exp_A(\log_A x) = x \quad \text{for } x \in 1 + G_R \\
\log_A(\exp_A x) = x \quad \text{for } x \in G_R
$$
これで証明が完了します。

$A$ に括弧 $[x, y] = xy - yx$ が与えられると、$A$ は $\|xy - yx\| \leq \sup(\|xy\|, \|yx\|) \leq \|x\| \cdot \|y\|$ の完全な正規化リー代数になります。 no. 3の命題 2は、$\tilde{H}$含む$G \times G$と$\tilde{H}$の絶対収束領域が定義する解析的写像$h : G \times G \to A$であることを意味します。それから
$$
h(x, y) = \sum_{r, s \geq 0} H_{r,s}(x, y).
$$

#### 命題 5 {#lie-ii-s8-prop-5 .statement tag=0A6Y}

G の x、y について、
$$
\exp_A \cdot \exp_A y = \exp_A h(x, y).
$$
$e^{U e^V} = e^{H(U, V)}$ そしてそれ以降
$$
m \circ (1 + \tilde{\epsilon}, 1 + \tilde{\epsilon}) = (1 + \tilde{\epsilon}) \circ \tilde{H}
$$
$\tilde{H}(A \times A; A)$ (ここで、m は A の乗法を示します)。 命題は、命題 2、補題 3 および微分可能および分析多様体、R、4.1.5 から続きます。

### 練習問題 {#lie-ii-s8-exercises}

体 $K$ の残差特性 $p$ が >0 であると仮定します。 $K$の評価$v$の$\mathfrak{o}_K$環で表します。

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
