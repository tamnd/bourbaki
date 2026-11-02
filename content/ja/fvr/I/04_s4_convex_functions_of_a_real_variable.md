---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 4
section_title: CONVEX FUNCTIONS OF A REAL VARIABLE
lang: ja
source: fvr-i-vii
book_pages: 23-33, 45-49
pdf_pages: 0038-0048, 0060-0064
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A CONVEX FUNCTION
      page: 24
      pdf_page: 39
    - "no": 2
      title: FAMILIES OF CONVEX FUNCTIONS
      page: 27
      pdf_page: 42
    - "no": 3
      title: CONTINUITY AND DIFFERENTIABILITY OF CONVEX FUNCTIONS
      page: 27
      pdf_page: 42
    - "no": 4
      title: CRITERIA FOR CONVEXITY
      page: 30
      pdf_page: 45
statements: 23
exercises: 25
content_sha256: 647de879ee35700e3aed4f2f884d0765d43907480c8c078366f319f3b43122ca
translated_from: content/en/fvr/I/04_s4_convex_functions_of_a_real_variable.md
translation_method: google
source_content_sha256: f3bb356dcd01c2f124b6edbcb7551016f358669cd0b6cfe2c6628e4d9303177e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 8ed618fa41365d275d28c1bf0d26119ce19461c93dd3882311b3214f9d80c735
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。実数変数の凸写像

$H$ を $\mathbf{R}$ の部分集合とします。 $f$ $H$ で定義された有限実数写像を、$G$ を *グラフ* または $\mathbf{R} \times \mathbf{R} = \mathbf{R}^2$、点 $M_x = (x, f(x))$ の集合における写像 $f$ の代表集合とします。 $x$ は $H$ を通過します。 It is convenient to say that a point $(a, b)$ of $\mathbf{R}^2$ such that $a \in H$ lies *above* (resp. *strictly above*, *below*, *strictly below*) $G$ if one has $b \geq f(a)$ (resp. $b > f(a)$, $b \leq f(a)$, $b < f(a)$). $A = (a, a')$ と $B = (b, b')$ が $\mathbf{R}^2$ の 2 つの点である場合、端点 $A$ と $B$ を持つ閉じたセグメントを $AB$ で表します。 $a < b$ の場合、$AB$ は $[a, b]$ で定義された線形写像 $a' + \frac{b' - a'}{b - a} (x - a)$ のグラフです。このセグメントの傾き $\frac{b' - a'}{b - a}$ を $p(AB)$ で表し、次の補題を使用します。その検証は明らかです。

#### 補題 {#fvr-i-s4-n0-lem-1 .statement tag=085O}

*$A = (a, a')$、$B = (b, b')$、$C = (c, c')$を$\mathbf{R}^2$の3つの点とし、$a < b < c$とします。次の主張は同等です:*

a) *B は AC を下回ります。*
b) *C は A と B を通る線移行の上にあります。*
c) *B と C を通る線移行の上にあります;*
d) $p(AB) \leq p(AC)$;
e) $p(AC) \leq p(BC)$。

補題は、置き換えるが「上」（または「下」）×「厳密に上」（または「厳密に下」）、および記号 $\leq$ が < である場合でも成立します（図 1）。

![点 A、B、C、および x でラベル付けされたセグメント値 a、b、c を示すグラフ](../images/fig_1.png)

図1

### 1. 凸の定義写像

#### 定義 1 {#fvr-i-s4-def-1 .statement tag=085P}

区間 $I \subset \mathbf{R}$ で定義された有限数値写像 $f$ は、$I$ の点 $x, x'$、($x < x'$)、点ごとに、$I$ に凸であると言います。 $x \leq z \leq x'$ がセグメント $M_xM_{x'}$ の下にあるように、$f$ のグラフ $G$ の $M_z$ (または、このセグメントのすべての点が $G$ の上にある場合も同じになります) (図 2)。

![点 M_x、M_z、M_{x'}、および曲線 G を示すグラフ](../images/fig_2.png)

図2

セグメントのパラメトリック表現を考慮すると (Gen. Top.、VI、p. 35)、$f$がIに凸になるのは不等式があるということです条件

$$
f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')
$$

点の対、Iの$(x, x')$、および$\lambda \in [0, 1]$ごとに。

定義 1 は以下と同等です: * $f$ のグラフ G の上にある $\mathbf{R}^2$ の点の集合は凸です*。実際、この条件は、$f$ が I に凸であるためには明らかに十分です。また、$f$ が I に凸で、$(x, y), (x', y')$ が G の上にある 2 つの点である場合、1 つは $y \geq f(x),\ y' \geq f(x')$ を持ち、そこから $0 \leq \lambda \leq 1$ については、これも必要です。

$$
\lambda y + (1 - \lambda)y' \geq \lambda f(x) + (1 - \lambda)f(x') \geq f(\lambda x + (1 - \lambda)x')
$$

(1) により、端点 $(x, y)$ と $(x', y')$ を持つセグメントのすべての点が G の上にあることがわかります。

#### 注意 {#fvr-i-s4-n1-rem-1 .statement tag=085Q}

On は、G の *厳密に上* にある点の集合が凸であることと同じように見えます。逆に、この集合が凸の場合、

$$
\lambda y + (1 - \lambda)y' > f(\lambda x + (1 - \lambda)x')
$$

$0 \leq \lambda \leq 1$ と $y > f(x),\ y' > f(x')$ の場合。この公式で y を $f(x)$ と $y'$ が $f(x')$ に近づく傾向にすると、$f$ が凸であることがわかります。

#### 例 1 {#fvr-i-s4-n1-exa-1 .statement tag=085R}

すべての (実) アフィン線形写像 $ax + b$ は $\mathbf{R}$ に凸です。

#### 例 2 {#fvr-i-s4-n1-exa-2 .statement tag=085S}

写像 $x^2$ は $\mathbf{R}$ に凸です。

$$
\lambda x^2 + (1 - \lambda)(x')^2 - \left( \lambda x + (1 - \lambda)x' \right)^2 = \lambda(1 - \lambda)(x - x')^2 \geq 0
$$

$0 \leq \lambda \leq 1$の場合。

#### 例 3 {#fvr-i-s4-n1-exa-3 .statement tag=085T}

写像 $|x|$ は $\mathbf{R}$ に凸なので、

$$
|\lambda x + (1 - \lambda)x'| \leq \lambda |x| + (1 - \lambda)|x'|
$$

$0 \leq \lambda \leq 1$の場合。

$f$ が I に凸である場合、その制限から任意の区間 $J \subset I$ が J に凸であることは明らかです。

$f$ を I に凸の写像とし、 $x < x'$ となるように I の 2 つの点を$x, x'$ とします。 $z \in I$ が $[x, x']$ の *外側* であれば、$M_z$ は $M_x$ と $M_{x'}$ を結ぶ線 D の *上* にあります。こちらは補題の明らか帰結です。

このことから、$z$ が点で、$x < z < x'$ となり、$M_z$ がセグメント $M_x M_{x'}$ 上にある場合、*他の点* $z'$ については、$x < z' < x'$ 点となることが推測されます。 $M_{z'}$ もセグメント $M_x M_{x'}$ 上にあります。上記のことから、$M_{z'}$ は同時にこのセグメントの上と下の両方にあることがわかります。他の語では、$f$ は $[x, x']$ 上の *アフィン線形* 写像と等しくなります。

#### 定義 2 {#fvr-i-s4-def-2 .statement tag=085U}

*区間 $I \subset \mathbf{R}$ で定義される有限実数写像 $f$ は、I ($x < x'$) の任意の点 $x, x'$ について、すべての場合、I に厳密に凸であると言います。 $f$ のグラフ G の点 $M_z$ は、$x < z < x'$ がセグメント $M_x M_{x'}$ の厳密に下に位置します (または、端点を除いて、セグメントのすべての点が G の厳密に上にある場合も同様です)*。

他の語では、不等式が必要です

$$
f(\lambda x + (1 - \lambda)x') < \lambda f(x) + (1 - \lambda)f(x')
$$

$I$ の個別の点 $(x, x')$ のすべての対と、$0 < \lambda < 1$ のようなすべての $\lambda$ に対して。

def の前にあるコメント。 2 は、凸写像 $f$ が $I$ に厳密に凸であるためには、$I$ に含まれる区間が存在しない (単一の点に減らない) ことで、この区間に対する $f$ の制限が *アフィンであることが必要かつ十分であることを示しています。リニア*。

上記の例のうち、1 番目と 3 番目は厳密には凸ではありません。一方、$x^2$ は厳密に $\mathbf{R}$ に凸です。同様の計算により、$1/x$ は厳密に $[0, +\infty[$ に凸であることがわかります。

#### 命題 1 {#fvr-i-s4-prop-1 .statement tag=085V}

*$f$ を有限実数写像 、区間 $I \subset \mathbf{R}$ に凸（厳密に凸）であるものとします。 For every family $(x_i)_{1 \leq i \leq p}$ of $p \geq 2$ distinct points of $I$, and every family $(\lambda_i)_{1 \leq i \leq p}$ of $p$ real numbers such that $0 < \lambda_i < 1$ and $\sum_{i=1}^p \lambda_i = 1$, we have*

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i)
$$

(それぞれ

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i)).
$$

$p = 2$ に対して命題 (凸写像の場合) 簡約するから不等式 (1) なので、$p > 2$ に対して帰納法で議論します。 数 $\mu = \sum_{i=1}^{p-1} \lambda_i$ は $> 0$ です。 $a$と$b$が$x_i$の最小のと最大のであれば、$a \leq \frac{\sum_{i=1}^{p-1} \lambda_i x_i}{\sum_{i=1}^{p-1} \lambda_i} \leq b$は明らかです。他の語、点 $x = \frac{1}{\mu} \sum_{i=1}^{p-1} \lambda_i x_i$ 属するから $I$、および帰納法の仮定は $\mu f(x) \leq \sum_{i=1}^{p-1} \lambda_i f(x_i)$ を意味します。さらに、(1) から次のことがわかります。

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) = f(\mu x + (1 - \mu)x_p) \leq \mu f(x) + (1 - \mu)f(x_p) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

不等式 (2) から開始して、厳密に凸な写像についても同じ方法で議論します。

有限実数写像 $f$ は、$-f$ が $I$ 上で凸（つまり厳密に凸）である場合、$I$ 上で *凹*（つまり *厳密に凹*）であると言います。 $I$ の個別の点のすべての対 $(x, x')$ と、$0 < \lambda < 1$ となるすべての $\lambda$ について、同じことが言えます。

$$
f(\lambda x + (1 - \lambda)x') \geq \lambda f(x) + (1 - \lambda)f(x')
$$

(それぞれ $f(\lambda x + (1 - \lambda)x') > \lambda f(x) + (1 - \lambda)f(x')$)。

### 2. 凸族写像

#### 命題 2 {#fvr-i-s4-prop-2 .statement tag=085W}

Let $f_i$ ($1 \leq i \leq p$) be $p$ convex functions on an interval $I \subset \mathbf{R}$, and $c_i$ ($1 \leq i \leq p$) be $p$ arbitrary positive numbers; then the function $f = \sum_{i=1}^p c_i f_i$ is convex on $I$. さらに、少なくとも 1 つの添字 $j$ 写像 $f_j$ が $I$ と $c_j > 0$ に厳密に凸である場合、$f$ は $I$ に厳密に凸です。

これに続いて、各 $f_i$ に適用不等式 (1) (それぞれ (2)) が続き、$f_i$ の不等式に $c_i$ を乗算し、項ごとに加算します。

#### 命題 3 {#fvr-i-s4-prop-3 .statement tag=085X}

$(f_\alpha)$ を区間 $I \subset \mathbf{R}$ に凸な写像の族とします。この族の上部包絡線 $g$ が $I$ の点ごとに有限である場合、 $g$ は $I$ に凸です。

確かに、$g$のグラフの上にある点$(x, y) \in \mathbf{R}^2$の集合は、写像$f_\alpha$のそれぞれのグラフの上にある点によって形成される凸型集合の共通部分です。だから凸です。

#### 命題 4 {#fvr-i-s4-prop-4 .statement tag=085Y}

$H$ を区間 $I \subset \mathbf{R}$ に凸の写像の集合とします。 $\mathfrak{F}$ が $I$ で点的に有限実数写像 $f_0$ に収束する $H$ のフィルターである場合、この写像は $I$ に凸です。

これを確認するには、不等式 (1) の $\mathfrak{F}$ に沿って極限まで通過するだけで十分です。

### 3. 凸の連続性と微分可能性写像

#### 命題 5 {#fvr-i-s4-prop-5 .statement tag=085Z}

実際の有限写像 $f$ が区間 $I$ に凸（厳密に凸）であるためには、すべての $a \in I$ の勾配が次のとおりであることが必要かつ十分です。

$$
p(M_a M_x) = \frac{f(x) - f(a)}{x - a}
$$

$I \cap \mathbf{C}\{a\}$の$x$の増加する (それぞれ真に増加する) 写像になります。

この命題は、定義1と2の明らか帰結と、I、p. 23の補題です。

#### 命題 6 {#fvr-i-s4-prop-6 .statement tag=0860}

$f$ を区間 $I \subset \mathbf{R}$ に凸な有限実数写像とします。次に、$I$ 写像 $f$ の各内部点 $a$ は連続であり、左右の導関数が有限で、$f'_g(a) \leq f'_d(a)$ になります。

確かに、$x \in I$ と $x > a$ の場合、 写像 $x \mapsto \frac{f(x) - f(a)}{x - a}$ は増加する (提案 5) であり、$y < a$ と $y \in I$ の場合、次のようになります。

$$
\frac{f(y) - f(a)}{y - a} \leq \frac{f(x) - f(a)}{x - a}
$$
(5)

プロップによって。 5;したがって、この写像は点 $a$ で有限の権利極限を持ちます。他の語、$f'_d(a)$ は存在し、有限です。さらに、(5) において $x$ を $a$ ($x > a$) に近づけると、次のようになります。

$$
\frac{f(y) - f(a)}{y - a} \leq f'_d(a)
$$
(6)

$y < a$ 所属から I まで。同様に、$f'_g(a)$ が存在し、

$$
f'_d(a) \leq \frac{f(x) - f(a)}{x - a}
$$
(7)

$x \in I$ と $x > a$ 用。この最後の不等式で $x$ を $a$ ($x > a$) に近づけると、$f'_g(a) \leq f'_d(a)$ が得られます。 点 $a$ における左右の導関数の存在は、この点における $f$ の連続性を明らかに保証します。

#### 系 1 {#fvr-i-s4-prop-6-cor-1 .statement tag=0861}

*$f$をIの凸（厳密に凸）写像とします。 $a$ と $b$ が I の 2 つの内部点で、$a < b$ の 1 つが* になる場合 (図 3)

![点 a と b に接線を持つ凸型写像を示すグラフ。それぞれ M_a と M_b とラベル付けされています。](../images/fig_3.png)

図3

$$
f'_d(a) \leq \frac{f(b) - f(a)}{b - a} \leq f'_g(b)
$$
(8)

(それぞれ

$$
f'_d(a) < \frac{f(b) - f(a)}{b - a} < f'_g(b)
$$
(9)

ダブル不等式 (8) は、(6) と (7) から記法の単純な変更によって得られます。一方、$f$ が厳密に凸であり、$c$ が $a < c < b$ となるような場合、(8) と prop から、 5、

$$
f'_d(a) \leq \frac{f(c) - f(a)}{c - a} < \frac{f(b) - f(a)}{b - a} < \frac{f(b) - f(c)}{b - c} \leq f'_g(b)
$$

そこから（9）。

#### 系 2 {#fvr-i-s4-prop-6-cor-2 .statement tag=0862}

*$f$がIに凸（厳密に凸）の場合、$f'_d$と$f'_g$はIの内側の増加する（それぞれ真に増加する）になります。 $f$が微分不可能なIの点の集合は可算であり、$f$が微分可能な点ごとに$f'_d$と$f'_g$は連続です。

最初の部分は (8) (それぞれ (9)) と不等式の直後に続きます。

$$
f'_g(a) \leq f'_d(a).
$$

一方、E を I の内部点 $x$ の集合とします。ここで、$f$ は微分可能ではありません (つまり、$f'_g(x) < f'_d(x)$)。それぞれの $x \in E$ について、$J_x$ をオープン区間 $]f'_g(x), f'_d(x)[$ とします。 (8) から、$x$ と $y$ が $x < y$ となるような E の 2 つの点である場合、すべての $u \in J_x$ とすべての $v \in J_y$ に対して $u < v$ が得られます。他の語では、$x$ が E を通過するため、オープン空でない区間 $J_x$ はペアで互いに素になります。したがって、そのような区間の集合は可算であり、したがって E も同様です。 最後に、$f'_d$ (それぞれ $f'_g$) は増加するであるため、すべての内部点 $x$ に右極限と左極限があります。 I;小道具。 I、p. 18 の 6 は、点 $x$ の$f'_d$ (それぞれ $f'_g$) の右極限が $f'_d(x)$ に等しく、その左極限が $f'_g(x)$ であることを示しています。 系の最後の部分があります。

$f$をIの凸写像、$a$をIの内点、移行から点$M_a$までの直線を$y - f(a) = \alpha(x - a)$とします。不等式 (8) から、$f'_g(a) \leq \alpha \leq f'_d(a)$ の場合、グラフ G のすべての点は D の上にあり、$f$ が厳密に凸である場合、$M_a$ は D と G に対して唯一の点共通のであることがわかります。ある人は、D が点 $M_a$ の G への*サポートライン*であると言っています。逆に、G が D より上にある場合、すべての $x \in I$ に対して $f(x) - f(a) \geq \alpha(x - a)$ があり、そこから $x > a$ に対して $\frac{f(x) - f(a)}{x - a} \geq \alpha$、$x < a$ に対して $\frac{f(x) - f(a)}{x - a} \leq \alpha$ が得られます。これらの不等式において $x$ を $a$ にすると、$f'_g(a) \leq \alpha \leq f'_d(a)$ になります。

特に、$f$ が点 $a$ で微分可能である場合、点 $M_a$ での G への支持線が *1 つだけあり、それは $M_a$ での G への *接線* です。

#### 注意 {#fvr-i-s4-n3-rem-1 .statement tag=0863}

$f$ がオープン区間 I 上で厳密に凸の写像である場合、$f'_d$ は I 上の真に増加するであるため、プロップに従って 3 つのケースが考えられます。 I、p. 13 の 2:
1. $f$ は I の真に減少するです。
2. $f$ は I の真に増加するです。
3. $f$ は、$x \leq a$ では真に減少する、$x \geq a$ では真に増加するとなるような $a \in I$ があります。

$f$ が I に凸であるが厳密には凸ではない場合、$f$ は I に含まれる区間で定数になる可能性があります。 $J = ]a, b[$ を最大のとし、$f$ が定数である区間を開きます (つまり、$f'_d(x) = 0$ である区間の内部)。この場合、$f$ は、点 $x \in I$ によって形成された区間の真に減少するであり、$x \leq a$ (存在する場合) となり、点 $x \in I$ によって形成された区間の真に増加するは、$x \geq b$ になります (存在する場合)存在します）。

すべての場合において、$f$ は $I$ ($\overline{\mathbf{R}}$) の左側の端点に *right 極限* を持ち、右側の端点に *left 極限* を持っていることがわかります。これらの極限は有限または無限の場合があります (*cf.* I、p. 46、演習 5、6、および 7)。言語の乱用により、ときどきは、$I$ の内部の $f$ に等しく、$I$ の端点まで連続性によって拡張された連続写像 ($\overline{\mathbf{R}}$ に値が含まれる) は、$\overline{I}$ に *凸* であると述べています。

### 4. 凸性の基準

#### 命題 7 {#fvr-i-s4-prop-7 .statement tag=0864}

*$f$を区間$I \subset \mathbf{R}$で定義された有限実数写像とします。 $f$ が $I$ に凸であるためには、数 $a, b$ の $I$ のすべての対が $a < b$ となること、およびすべての実数 $\mu$、写像 $f(x) + \mu x$ が必要かつ十分です。 点 $a, b$ のいずれかで $[a, b]$ に最高値に達します。*

条件は *必須*です。実際、$\mu x$ は $\mathbf{R}$ に凸なので、写像 $f(x) + \mu x$ は $I$ に凸です。したがって、$\mu = 0$ の場合に限定することができます。それから、
$$
x = \lambda a + (1 - \lambda) b \quad (0 \leq \lambda \leq 1),
$$
1つは持っています
$$
f(x) \leq \lambda f(a) + (1 - \lambda) f(b) \leq \operatorname{Max}(f(a), f(b)).
$$

条件で * 十分 * です。 $\mu = -\frac{f(b) - f(a)}{b - a}$ と $g(x) = f(x) + \mu x$ を考えてみましょう。すべての $x \in [a, b]$ に対して $g(a) = g(b)$ があり、したがって $g(x) \leq g(a)$ があり、この不等式が不等式 (1) に相当することをすぐに確認できます。ここで、1 つの置き換える $z$ は $a$ で、$x'$ は $b$ です。

#### 命題 8 {#fvr-i-s4-prop-8 .statement tag=0865}

*有限実数写像 $f$ が開区間 $I \subset \mathbf{R}$ 上で凸（厳密に凸）であるためには、それが $I$ 上で連続であり、可算数の $I$ に対する補数 $B$ の点ごとに導関数があることが必要かつ十分です。この区間の部分集合と、導関数は $B$ の増加する (それぞれ真に増加する) になります。

条件はプロップから必要です。 6 とその系 2 (I、p. 27)。それが十分であることを示しましょう。したがって、$f'$ は $B$ で増加するであり、$f$ は凸ではないとします。すると、$I$ の 3 つの点 $a, b, c$ が存在し (I、p. 27、提案 5)、$a < c < b$ と $\frac{f(c) - f(a)}{c - a} > \frac{f(b) - f(c)}{b - c}$ になります。しかし、平均値定理 (I, p. 14, th. 1) から、
$$
\frac{f(c) - f(a)}{c - a} \leq \sup_{x \in B,\ a < x < c} f'(x) \quad \text{and} \quad \frac{f(b) - f(c)}{b - c} \geq \inf_{x \in B,\ c < x < b} f'(x).
$$

したがって、$f'$ が $B$ で増加するであるという仮定とは反対に、$\sup_{\lambda \in B,\ a < \lambda < c} f'(\lambda) > \inf_{\lambda \in B,\ c < \lambda < b} f'(\lambda)$ があります。

ここで、$f'$ が $B$ 上で真に増加するであると仮定すると、$f$ は凸であり、できないは $I$ に含まれる任意の開いた区間上のアフィン線形写像に等しいため、逆に、$f'$ はこの区間上で定数になるからです。 仮定まで。

#### 系 {#fvr-i-s4-n4-cor-1 .statement tag=0866}

*$f$ を有限実数写像とし、連続で区間 $I \subset \mathbf{R}$ で 2 回微分可能です。 $f$ が $I$ に凸であるためには、すべての $x \in I$ に対して $f''(x) \geqslant 0$ であることが必要かつ十分です。 $f$ が厳密に $I$ に凸であるためには、前の条件が満たされ、さらに点 $x \in I$ の集合が$I$ で$f''(x) > 0$ が密であることが必要かつ十分です。

これは、前の命題の直後、および系のI、p. 14に続きます。

#### 例 {#fvr-i-s4-n4-exa-1 .statement tag=0867}

区間 ]$0, +\infty$ [ 写像 $x^r$ ($r$ 任意の実数) の二次導関数は $r(r-1)x^{-2}$ に等しくなります。したがって、$r > 1$ または $r < 0$ の場合は厳密に凸であり、$0 < r < 1$ の場合は厳密に凹です。 \*

In order to be able to formulate another criterion for convexity we make the following definition: given the graph $G$ of a finite real function defined on an interval $I \subset \mathbf{R}$ and an interior point $a$ of $I$, we shall say that a line $D$ passing through $M_a = (a, f(a))$ is *locally above* (resp. *locally below*) $G$ if there exists a neighbourhood $V \subset I$ of $a$ such that every point of $D$ contained in $V \times \mathbf{R}$ is above (resp. below) $G$; we shall say that $D$ is *locally on* $G$ at the point $M_a$ if there is a neighbourhood $V \subset I$ of $a$ such that the intersection of $D$ and $V \times \mathbf{R}$ is identical to that of $G$ and $V \times \mathbf{R}$ (in other words, if $D$ is simultaneously locally above and locally below $G$).

#### 命題 9 {#fvr-i-s4-prop-9 .statement tag=0868}

*$f$ を、開いた区間 $I \subset \mathbf{R}$ の上半連続である実数有限写像とします。 $f$ が $I$ に凸であるためには、$f$ のグラフ $G$ のすべての点 $M_x$ が、この点で局所的に $G$ より上にあるすべての線が局所的に $G$ (点で) 上にあることが必要かつ十分です。 $M_x$).*

条件は*必要*: 確かに、$f$が$I$に凸の場合、$f$のグラフ$G$の点$M_a$ごとに*サポートライン*$\Delta$から$G$が存在します。 $\Delta$ は $G$ より下なので、*なおさら* ローカルでは $G$ (I, p. 29) より下です。ライン $D$ がローカルで $G$ の点 $M_a$ にある場合、それはローカルで $\Delta$ より上にあるため、$\Delta$ と一致するでなければならず、その結果、ローカルでは点 $M_a$ の $G$ にあります。

条件は *十分* です。確かに、それが満たされ、$f$ が $I$ に凸でないと仮定します。次に、$I$ ($a < b$) の 2 つの点 $a, b$ があり、セグメント $M_aM_b$ の厳密に上に $G$ の点 $M_x$ が存在します (図 4)。他の語、写像 $g(x) = f(x) - f(a) - \frac{f(b) - f(a)}{b - a}(x - a)$ は $[a, b]$ で値 $> 0$ かかります。このコンパクト区間では $g$ が有限で上部半連続であるため、$[a, b]$ 上の最小の上界 $k$ は有限で $> 0$ であり、集合 $g^{-1}(k)$ は閉じていて空ではありません (\emph{Gen. Top.}, IV、p. 361、第 3 および小道具 1)。 $c$ を $g^{-1}(k)$ の最大の下界とします。 $a < c < b$ があります。そして、点 $M_c$ では、方程式 $y = f(c) + \frac{f(b) - f(a)}{b - a}(x - c)$ の線 D は局所的に G の上にあります。しかし、できないはこの点で局所的に G 上にあります。なぜなら、$a < x < c$ には $g(x) < k$ があり、これは $M_x$ が厳密に D よりも小さいことを意味します。これにより、命題が確立される矛盾が生じました。

#### 系 1 {#fvr-i-s4-prop-9-cor-1 .statement tag=0869}

*実有限写像* $f$ *オープン区間* $I \subset \mathbf{R}$ *および上部半連続オン* $I$ *凸であること* $I$ *すべて* $x \in I$ *存在する必要がある* $\varepsilon > 0$ *次のような関係* $|h| \leq \varepsilon$ *含意*

$$
f(x) \leq \frac{1}{2} \left( f(x + h) + f(x - h) \right).
$$

条件が *十分* であることを示すだけで済みます。実際、$f$ のグラフ G の点 $M_a$ で線 D が局所的に G より上にある場合、この点では線 D は局所的に G 上にあります。なぜなら、逆の場合、例えば、点 $M_{a+h}$ は厳密に D よりも下にあり、点 $M_{a-h}$ は D よりも下にあるでしょう。 したがって、線分 $M_{a-h}M_{a+h}$ の中点は厳密に D よりも上になり (図 5)、そして仮定のおかげで、$M_a$ は次のようになります。 *なおさら* は厳密に D 未満である必要がありますが、これは不合理です。

![点 M_{a-h}、M_a、M_{a+h} を持つ凸型写像と D のラベルが付いた接線を示すグラフ。](https://i.imgur.com/3Q5z5QG.png)

図5

#### 系 2 {#fvr-i-s4-prop-9-cor-2 .statement tag=086A}

*$f$ を、開いた区間 $I \subset \mathbf{R}$ 上で定義された有限実数写像とします。 点 $x \in I$ ごとにオープン区間 $J_x \subset I$ 含む $x$ があり、$f$ ～ $J_x$ の制限が $J_x$ に凸である場合、$f$ は次のようになります。 $I$に凸。*

$f$ が prop の基準を満たしていることは明らかです。 9.

### 練習問題 {#fvr-i-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
