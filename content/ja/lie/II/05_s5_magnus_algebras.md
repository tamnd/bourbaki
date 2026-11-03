---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 5
section_title: Magnus algebras
lang: ja
source: lie-i-iii
book_pages: 149-155, 193-201
pdf_pages: 0167-0173, 0211-0219
extraction: ocr
subsections:
    - "no": 1
      title: MAGNUS ALGEBRAS
      page: 149
      pdf_page: 167
    - "no": 2
      title: MAGNUS GROUP
      page: 150
      pdf_page: 168
    - "no": 3
      title: MAGNUS GROUP AND FREE GROUP
      page: 151
      pdf_page: 169
    - "no": 4
      title: LOWER CENTRAL SERIES OF A FREE GROUP
      page: 152
      pdf_page: 170
    - "no": 5
      title: '*p*-Filtration of Free Groups'
      page: 154
      pdf_page: 172
statements: 14
exercises: 12
content_sha256: af341f918cce0ffd73d365e62713af5c5e7f7d686174023bf63ef85c2769e782
translated_from: content/en/lie/II/05_s5_magnus_algebras.md
translation_method: google
source_content_sha256: 6bac6bb784fbb4b199b3afb36bd212ba5f589bd833743b3d4385ed3b9a405428
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b0ad2f6a9fd0c58c7f45c3ae27fe0dabc8e03f22ba8113dd9978ff24fa1a4645
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。マグナス代数

この段落では、Xは集合、F(X)はX(代数、章I, § 7, no. 5)に構築された自由群、A(X)は代数に構築された自由結合群を表します。 X とその合計目盛$(A^n(X))_{n \geq 0}$ (cf. 代数, 章 III, § 3, no. 1, 例 3)。 X は、F(X) および A(X) の像と識別されます。

### 1. マグナス代数

$\hat{A}(X)$ を積加群 $\prod_{n \geq 0} A^n(X)$ とします。ルールにより、私たちは $\hat{A}(X)$ 乗法に定義するです

$$
(a \cdot b)_n = \sum_{i=0}^n a_i \cdot b_{n-i}
$$

ここで、$a = (a_n)$ と $b = (b_n)$ は $\hat{A}(X)$ にあります。 可換代数、章 III, § 2, no. 12、例 1) は、$\hat{A}(X)$ が結合代数であり、$A(X)$ が $\hat{A}(X)$ の部分代数 、数列のからなると同一視されることを知っています。有限の数を除いて、そのすべての項は零です。

$\hat{A}(X)$ には、因子上の離散トポロジーの積位相が与えられます

あ^ン(X);この位相は、 環 K が離散位相を持ち、 $A(X)$ が $\hat{A}(X)$ で密であるとき、 $\hat{A}(X)$ を完全なハウスドルフ位相幾何学代数にします。

$a = (a_n) \in \hat{A}(X)$ にしましょう。家族 $(a_n)_{n \geq 0}$ は合計可能であり、 $a = \sum_{n \geq 0} a_n$ です。

すべての整数 $m \geq 0$ に対して、$\hat{A}_m(X)$ は、すべての $n \geq m$ に対して $a_n \in A^n(X)$ となるように、系列 $a = \sum_{n \geq m} a_n$ の理想的なからなるを表します。この理想の数列は、$\hat{A}(X)$ の 0 の近傍の基本的な系と、$\hat{A}(X)$ の積分フィルタです。上記の濾過に関連する位数写像は$\omega$で示されます。すべての $n \geq m$ と $a_m \neq 0$ (§ 4、番号 1 と 2) に対して $a_n \in A^n(X)$ が含まれる $a = \sum_{n \geq m} a_n$ の場合、$\omega(0) = +\infty$ と $\omega(a) = m$ になります。

$\hat{A}(X)$ は、K の係数を持つ集合 X の *マグナス代数* と呼ばれます。K に曖昧さがある場合は、$\hat{A}_K(X)$ と書きます。

#### 命題 1 {#lie-ii-s5-prop-1 .statement tag=0A5B}

*B を、B がハウスドルフで完全であるような実濾過 $(B_\alpha)_{\alpha \in \mathbf{R}}$ を伴う単一結合代数とする (§ 4、番号 1 と 2)。 f を B の X の写像として、$f(X) \subset B_\lambda$ に対して $\lambda > 0$ が存在するようにします。次に、f は 1 つだけの方法で、$\hat{A}(X)$ の連続単位準同型 $\hat{f}$ を B に拡張できます。

$f'$ を、$A(X)$ を B に拡張して $f$ に拡張した固有単位代数準同型とします (*代数*, 章 III, § 2, no. 7, 命題 7)。 $f'$ が *連続* であることを示します: $f'(A^n(X)) \subset B_{n\lambda}$ よって $f'(\hat{A}_n(X) \cap A(X)) \subset B_{n\lambda}$。したがって、$f'$ は、連続性によって準同型 $\hat{f} : \hat{A}(X) \to B$ まで、ただ 1 つの方法で拡張できます。

仮説と命題 1 の記法を保存し、$u \in \hat{A}(X)$ とします。 元 $\hat{f}(u)$ は $u((f(x))_{x \in X})$ で表され、*f(x) を u の x に代入した結果* と呼ばれます。特に$u((x)_{x \in X}) = u$。ここで、$u = (u_y)_{y \in Y}$ を $\hat{A}_1(X)$ の元の家族とし、$v \in \hat{A}(Y)$ とします。上記により、定義する元 $v((u_y)_{y \in Y}) \in \hat{A}(X)$ が可能になります。 $v \circ u$で表されます。 $u_y((f(x))) \in B_\lambda$ として、元 $u_y((f(x)))$ を v の y に置き換えることができます。 写像 $v \mapsto (v \circ u)((f(x)))$ と $v \mapsto v((u_y((f(x))))))$ は、$\hat{A}(X)$ の単位代数の 2 つの連続する準同型で、同じ値を B に変換します。 $u_y((f(x)))$ 元 $y \in Y$。したがって (命題 1)

$$
(v \circ u)((f(x))) = v((u_y((f(x))))))
$$

$v \in \hat{A}(Y)$の皆さんへ。

### 2. マグナス群

$\hat{A}(X)$ のすべての $a = (a_n)_{n \geq 0}$ に対して、K の元 $a_0$ は a の *定数項* と呼ばれ、$\varepsilon(a)$ で表されます。 公式 (1) は、$\varepsilon$ が $\hat{A}(X)$ の代数準同型を K に変換することを示しています。

#### 補題 1 {#lie-ii-s5-lem-1 .statement tag=0A5C}

*$\hat{A}(X)$ の元 a が可逆であるためには、その定数項が K で可逆であることが必要かつ十分です。

$a$ が $\hat{\mathbf{A}}(\mathbf{X})$ で可逆である場合、$\varepsilon(a)$ は $K$ で可逆です。逆に、$\varepsilon(a)$ が $K$ で可逆である場合、$a = \varepsilon(a)(1-u)$ となるような $u \in \hat{\mathbf{A}}_1(\mathbf{X})$ が存在します。 $b = \left( \sum_{n \geq 0} u^n \right) \varepsilon(a)^{-1}$と書きます。すると、$ab = ba = 1$ と $a$ は反転可能です。

したがって、定数項 1の$\hat{\mathbf{A}}(\mathbf{X})$の元の集合は、乗法モノイド$\hat{\mathbf{A}}(\mathbf{X})$の部分群であり、$\mathbf{X}$上に構築された*マグナス群*と呼ばれます（$K$を基準にして）。この章では、$\Gamma(\mathbf{X})$または単に$\Gamma$で表されます。すべての整数 $n \geq 1$ について、$\omega(a-1) \geq n$ のように $a \in \Gamma$ の $\Gamma_n$ 集合で表します。 § 4, no. 5 の命題 2 により、数列 $(\Gamma_n)_{n \geq 1}$ は $\Gamma$* の *統合集中濾過です。

### 3. マグナス群とフリー 群

#### 定理 1 {#lie-ii-s5-thm-1 .statement tag=0A5D}

*$r$を$\mathbf{X}$の写像を$\hat{\mathbf{A}}(\mathbf{X})$にすると、すべての$x \in \mathbf{X}$が$\omega(r(x)) \geq 2$になります。自由な群 $F(\mathbf{X})$ の一意な準同型 $g$ をマグナス群 $\Gamma(\mathbf{X})$ に変換すると、すべての $x \in \mathbf{X}$ に対する $g(x) = 1 + x + r(x)$ が単射になります。*

まず 3 つの補題を証明します。

#### 補題 2 {#lie-ii-s5-lem-2 .statement tag=0A5E}

*$n$をゼロ以外の有理数整数とします。正式な冪系列 $K[[t]]$ の環には $(1+t)^n = \sum_{j \geq 0} c_{j,n} t^j$ と書きます。 $c_{j,n} \neq 0$ となるような整数 $j \geq 1$ が存在します。

$n > 0$ の場合、二項式公式により $c_{n,n} = 1$ になります。
$n < 0$ として、$m = -n$ とします。すべての $j \geq 1$ に対して $c_{j,n} = 0$ の場合、$(1+t)^n = 1$、よっての逆数、$(1+t)^m = 1$ は、矛盾する公式 $c_{m,m} = 1$ となります。*

#### 補題 3 {#lie-ii-s5-lem-3 .statement tag=0A5F}

*$x_1, \ldots, x_s$を$\mathbf{X}$の元とし、$s \geq 1$と$x_i \neq x_{i+1}$を$1 \leq i \leq s-1$とします。 $n_1, \ldots, n_s$ をゼロ以外の有理数整数とします。すると、$\hat{\mathbf{A}}(\mathbf{X})$の元$\prod_{i=1}^s (1+x_i)^{n_i}$は$\neq 1$になります。

$m$ を $K$ と $k$ 体 $K/m$ の最大理想とする。 $p : \hat{\mathbf{A}}_K(\mathbf{X}) \to \hat{\mathbf{A}}_k(\mathbf{X})$ を、$x \in \mathbf{X}$ (no. 1, 命題 1) に対して $p(x) = x$ となるような単位$K$-代数の一意の連続準同型とします。 $p\left( \prod_{i=1}^s (1+x_i)^{n_i} \right) \neq 1$ と問題が、$K$ が体である場合に帰着されることを証明すれば十分です。

補題 2 の記法:

$$
\prod_{i=1}^s (1+x_i)^{n_i} = \sum_{b_1 \geq 0} \cdots \sum_{b_s \geq 0} c_{b_1, n_1} \cdots c_{b_s, n_s} x_1^{b_1} \cdots x_s^{b_s}.
$$

補題 2 までに、$c_{a_i, n_i} \neq 0$ ($1 \leq i \leq s$) となる整数 $a_i > 0$ が存在します。 *代数*、章 I, § 7, no. 4、命題 6 により、$b_i \geq 0$ と $(b_1, \ldots, b_s) \neq (a_1, \ldots, a_s)$ が $x_1^{a_1} \ldots x_s^{a_s}$ に等しくなるような単項式 $x_1^{b_1} \cdots x_s^{b_s}$ はありません。したがって、$\prod_{i=1}^s (1 + x_i)^{n_i}$ の $x_1^{a_1} \ldots x_s^{a_s}$ の係数は $c_{a_1, n_1} \ldots c_{a_s, n_s} \neq 0$ となり、結果が暗示されます。

#### 補題 4 {#lie-ii-s5-lem-4 .statement tag=0A5G}

*$\sigma$ を $\hat{A}(X)$ の連続自己準同型とし、$x \in X$ に対して $\sigma(x) = x + r(x)$ (no. 1, 命題 1) とします。すると、$\sigma$ はすべての $m \in \mathbf{N}$ に対して自己同型と $\sigma(\hat{A}_m(X)) = \hat{A}_m(X)$ になります。

$x \in X$、よって、$X$の$n \geq 1$、$x_1, \ldots, x_n$の場合は$\sigma(x) \equiv x \mod \hat{A}_2(X)$、
$$
\sigma(x_1) \ldots \sigma(x_n) \equiv x_1 \ldots x_n \mod \hat{A}_{n+1}(X);
$$
すべての $a \in A^n(X)$、特に $\sigma(A^n(X)) \subset \hat{A}_n(X)$ について $\hat{A}_{n+1}(X)$ を法とする $\sigma(a) \equiv a$ という線形性が続きます。したがって、$m \geq n$、よって $\sigma(\hat{A}_n(X)) \subset \hat{A}_n(X)$ は $\sigma(A^n(X)) \subset \hat{A}_n(X)$ となります。他の語では、$\sigma$は$A(X)$の濾過$(\hat{A}_m(X))$と互換性があり、その制限と関連するグレードの環が同一です。したがって、$\sigma$ は全単射です (*可換代数*、章 III, § 2, no. 8、系 3 から定理 1)。

最後に定理 1 を証明します。 $w \neq 1$ を $F(X)$ の元とします。 By *Algebra*, Chapter I, § 7, no. 5, Proposition 7, there exist $x_1, \ldots, x_s$ in $X$ and non-zero rational integers $n_1, \ldots, n_s$ such that $s \geq 1$, $x_i \neq x_{i+1}$ ($1 \leq i \leq s-1$) and
$$
w = x_1^{n_1} \ldots x_s^{n_s}.
$$
In the notation of Lemma 4,
$$
g(w) = \prod (1 + \sigma(x_i))^{n_i} = \sigma(\prod (1 + x_i)^{n_i}),
$$
hence $g(w) \neq 1$ by Lemmas 3 and 4.

### 4. フリー 群の中央下部系列

次の 2 つを証明します定理:

#### 定理 2 {#lie-ii-s5-thm-2 .statement tag=0A5H}

*環 $K$ 関係 $n.1 = 0$ は、整数 $n$ ごとに $n = 0$ を意味するとします。 $r$ を $X$ の写像から $\hat{A}(X)$ に、$x \in X$ に対して $\omega(r(x)) \geq 2$ を計算し、$g$ を $F(X)$ の準同型としてマグナス群 $\Gamma(X)$ にします。 $x \in X$の場合は$g(x) = 1 + x + r(x)$。すべての $n \geq 1$ について、$C^n F(X)$ は部分群の $g$ および $\Gamma(X)$ の $1 + \hat{A}_n(X)$ の下にある逆像です。*

#### 定理 3 {#lie-ii-s5-thm-3 .statement tag=0A5I}

※すべての$x \in X$について、$c(x)$を$F(X)/(F(X), F(X))$の$x$の標準像とします。 $g$ を、$F(X)$ (§ 4, no. 6) の濾過 $(C^n F(X))_{n \geq 1}$ に関連付けられた段階的リー $\mathbf{Z}$-代数とします。 自由リー $\mathbf{Z}$-代数 $L_\mathbf{Z}(X)$ の一意な準同型を $g$ にすると、 拡大する $c$ は同型になります。*

大まかに言うと、自由群 $F(X)$ (下部中央系列) に関連付けられた段階付きリー $\mathbf{Z}$-代数は、自由 リー $\mathbf{Z}$-代数 $L_\mathbf{Z}(X)$ です。

$F(X) = F, \Gamma(X) = \Gamma, \hat{A}(X) = \hat{A}, \hat{A}_\mathbf{Z}(X) = \hat{A}_\mathbf{Z}, C^n F(X) = C^n, \Gamma_n = 1 + \hat{A}_n(X)$と書き、$\alpha : L_\mathbf{Z}(X) \to g$を定理3の主張で紹介した準同型とします。

(A) 予備的な削減。

$\gamma$ は、$F$ の準同型を $x \in X$ の $\gamma(x) = 1 + x$ によって定義される $\Gamma$ に代入することを表します。 補題 4 までに、$\hat{A}$ の濾過と互換性のある代数 $\hat{A}$ の自己同型 $\sigma$ が存在し、すべての $x \in X$ に対して $\sigma(1 + x) = g(x)$ になります。次に、すべての $n$ に対して $\sigma(\Gamma_n) = \Gamma_n$ です。 $F$ の準同型 $g$ と $\sigma \circ \gamma$ が $X, g = \sigma \circ \gamma$ の $\Gamma$ 一致するになり、したがって $g^{-1}(\Gamma_n) = \gamma^{-1}(\Gamma_n)$ になります。 定理 2 の仮説の下では、$\mathbf{Z}$ は $K$ の部分環と識別できます。したがって、マグヌス代数 $\hat{A}_\mathbf{Z}$ は $\hat{A}$ の部分環と識別され、$\hat{A}_\mathbf{Z}$ の濾過は $\hat{A}$ の濾過によって引き起こされます。 $\gamma$ 写像 $F$ を $\hat{A}_\mathbf{Z}$ にすると、補足仮説 $K = \mathbf{Z}, r = 0$ と従って $g = \gamma$ の下で定理 2 と 3 を証明するだけで十分であることが分かります。

(B) $\alpha$ の全射性。

$X$ 生成する群 $F = C^1$、集合 $c(X)$ 生成するとして $\mathbf{Z}$ モジュール $g^1 = C^1/C^2$。しかし、$g^1$ 生成する嘘 $\mathbf{Z}$-代数 $g$ (§ 4, no. 6, 命題 5) したがって、$c(X)$ 生成する $g$ は、$\alpha$ が全射であることを証明します。

(C) 標準同型 $A^n(X) \to \hat{A}_n/\hat{A}_{n+1}$ の下で $A(X)$ を付けて代数 $\mathrm{gr}(\hat{A})$ を同一視する採点しました。 整数 $n \geq 1$ ごとに、$F^n = \gamma^{-1}(\Gamma_n)$ と書きます。私たちは (§ 4, no. 5) $(F^n)_{n \geq 1}$ が $F$ の統合された中央濾過であることを知っています。 $g'$ は、関連する段階的リー $\mathbf{Z}$-代数 (§ 4, no. 4) を表すものとします。 $f$ を $g'$ のリー代数準同型を $\gamma$ に関連付けられた $A(X)$ にします (§ 4, no. 5、命題 3)。これで、整数 $n \geq 1$ (§ 4, no. 6、命題 4) ごとに $C^n \subset F^n$ となり、$g = \bigoplus_{n \geq 1} C^n/C^{n+1}$ のうち $g' = \bigoplus_{n \geq 1} F^n/F^{n+1}$ には標準準同型 $\varepsilon$ が入ります。

$$
L_\mathbf{Z}(X) \xrightarrow{\alpha} g \xrightarrow{\varepsilon} g' \xrightarrow{f} A(X).
$$

$\beta = f \circ \varepsilon$と書きます。 $\beta$ を次のように明示的に与えます。 $u$ が $C^n$ の要素 $w$ の $C^{n+1}$ を法とするクラスである場合、 $\gamma(w) - 1$ は $\hat{A}$ の次数 $\geq n$ であり、 $\beta(u)$ は次数 $\gamma(w) - 1$ の同次成分です$n$。 特に、

$$
\beta(c(x)) = x \quad \text{for all } x \in X.
$$

(D) 定理 2 および 3 の証明。

$X$ に限定されたリー代数準同型 $\beta \circ \alpha : L_\mathbf{Z}(X) \to A(X)$ は (3) による同一性であるため、標準単射 (§ 3, no. 1) になります。したがって、$\alpha$ は単射であり、したがって (B) によって全単射です。これは定理 3 を証明します。 $\beta \circ \alpha = f \circ \varepsilon \circ \alpha$ は単射、$\alpha$ は全単射であるため、$\varepsilon$ は単射です。 $n \geq 1$ 全員にとって、

$$
\varepsilon_n : C^n/C^{n+1} \to F^n/F^{n+1}
$$

は単射なので、

$$
C^n \cap F^{n+1} = C^{n+1}.
$$

C^1 = F = F^1; C^n = F^n の場合、C^n \cap F^{n+1} = F^{n+1} よって C^{n+1} = F^{n+1}
これは、n \geqslant 1 上の帰納法によって定理 2 を証明します。

#### 系 {#lie-ii-s5-n4-cor-1 .statement tag=0A5J}

$$
\bigcap_{n \geqslant 1} C^n F(X) = \{e\}.
$$

適用定理 2 (K = \mathbf{Z} および r = 0)、
$$
\bigcap_{n \geqslant 1} C^n F(X) = \bigcap_{n \geqslant 1} g^{-1}(1 + \hat{A}_n(X)) = g^{-1}\left(\bigcap_{n \geqslant 1} (1 + \hat{A}_n(X))\right) = g^{-1}(1) = \{e\}.
$$

#### 注意 {#lie-ii-s5-n4-rem-1 .statement tag=0A5K}

H を X (§ 2, no. 10) に対するホール集合とします。 M を、F(X) 上の合成 (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy の法則で定義されるマグマとし、$\phi$ を M(X) の準同型として、制限がXがアイデンティティです。 $\phi(H)$ の元は、ホール集合 H に関連付けられた F(X) の *基本交換子* と呼ばれます。 整数 n \geqslant 1 ごとに、H_n を H の部分集合からなるとします元/長さn;私たちは (§ 2, no. 11, 定理 1)、L_\mathbf{Z}(X) への H_n の標準写像はアーベル群 L_\mathbf{Z}^n(X) の基底であることを知っています。さらに、$\phi(H_n) \subset C^n$; H_n のすべての m \in について、$\phi_n(m)$ を類 mod とします。 C^{n+1}/$\phi(m) \in C^n$。 定理 3 は、$\phi_n$ がアーベル群* C^n/C^{n+1} の基底に対する H_n の *全単射であることを示します。すべての w \in F(X) とすべての i \geqslant 1 に対して、n \geqslant 1 に対して、 $\mathbf{Z}^{(H_i)}$ の一意元 $\alpha_i$ が存在することがすぐにわかります。

$$
w = \prod_{i=1}^n \prod_{m \in H_i} \phi(m)^{\alpha_i(m)} \mod. C^{n+1},
$$

ここで、積は H で指定された合計順序に従って計算されます。

#### 例 {#lie-ii-s5-n4-exa-1 .statement tag=0A5L}

X が 2 つの元 x, y を持つ集合であるとします。H_1 = \{x, y\}、H_2 = \{xy\} とします。したがって、F(X) のすべての元 w を書くことができます
$$
w \equiv x^a y^b (x, y)^c \mod. C^3 \quad \text{with } a, b, c \text{ in } \mathbf{Z}.
$$
w = (xy)^n、a = b = n、c = n(1 - n)/2 (cf. 練習問題 9)、よっての場合
$$
(xy)^n \equiv x^n y^n (x, y)^{n(1-n)/2} \mod. C^3.
$$

### 5. *p*-フリーのろ過群

この番号では、*p* は素数数を表し、K = \mathbf{F}_p と仮定します。 $\gamma$ を、X の x について $\gamma(x) = 1 + x$ によって定義される $\Gamma(X)$ への F(X) の準同型とします。 $F_n^{(p)}(X) = \gamma^{-1}(1 + \hat{A}_n(X))$と書きます。 数列 $(F_n^{(p)}(X))_{n \geqslant 1}$ は F(X) 上の統合された中央濾過であり、$\gamma$ が単射 (no. 3, 定理 1) であるため *分離* されます。これは、F(X) の *p* フィルタリングと呼ばれます。

#### 命題 2 {#lie-ii-s5-prop-2 .statement tag=0A5M}

※Xが有限であると仮定します。すべての整数 n \geqslant 1 に対して、群 F(X)/F_n^{(p)}(X) は零能類 \leqslant n* の有限 p 群です。

$n$ について帰納法によって議論すると、$F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ がすべての $n \geqslant 1$ に対して有限可換な $p$ 群であることを証明するだけで十分です。すべての $w \in F_n^{(p)}(X)$、元 $\gamma(w) - 1$ の $\hat{A}(X)$ は位数 $\geqslant n$ です。 次数 $n$ の $\gamma(w) - 1$ の同次成分を $\delta_n(w)$ で表します。 写像 $\delta_n : F_n^{(p)}(X) \to A^n(X)$ は準同型と核 $F_{n+1}^{(p)}(X)$ (§ 4, no. 5, 命題 3) であるため、$F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ は $A^n(X)$ の部分群と同型です。 $X$ は有限であるため、$A^n(X)$ は $\mathbf{F}_p$ 以上の有限次元ベクトル空間であり、したがって有限可換群 $p$ 群となり、$F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ も同様です。

#### 命題 3 {#lie-ii-s5-prop-3 .statement tag=0A5N}

*$F(X)$ のすべての $w \neq 1$ に対して、有限 $p$ 群 $G$ と、$f(w) \neq 1$ となるような $F(X)$ から $G$ への準同型性 $f$ が存在します。

$w = x_1^{n_1} \ldots x_r^{n_r}$となるような$X$と整数$n_1, \ldots, n_r$の元$x_1, \ldots, x_r$が存在します。 $Y = \{x_1, \ldots, x_r\}$ にしましょう。 $Y$ の標準単射を $X$ 拡大するから準同型 $\alpha : F(Y) \to F(X)$ に。一方、$\beta$ を $F(X)$ の準同型から $F(Y)$ とし、制限から $Y$ までを恒等とし、写像 $X - Y$ から $\{1\}$ にする。すると、$y \in Y$に対する$\beta(\alpha(y)) = y$、したがって$\beta \circ \alpha$は$F(Y)$の同一性自己同型になります。 $w = \alpha(w')$ となるような $F(Y)$ には明らかに $w'$ が存在します。それから$\beta(w) = w' \neq 1$;現在 $\bigcap_{n \geqslant 1} F_n^{(p)}(Y) = \{1\}$ なので、$\beta(w) \notin F_n^{(p)}(Y)$ のような整数 $n \geqslant 1$ が存在します。 命題 2 により、群 $G = F(Y)/F_n^{(p)}(Y)$ は有限の $p$ 群になります。 $f$が$\beta$の合成と$F(Y)$の標準準同型を$G$にすると、$f(w) \neq 1$になります。

#### 系 {#lie-ii-s5-n5-cor-1 .statement tag=0A5O}

*$F(X)$の有限添字の通常の部分群の共通部分は$\{1\}$です。

### 練習問題 {#lie-ii-s5-exercises}

以下の練習問題では、§ 5の仮説と記法を仮定します。 $F$ は、$F$ の空き群 $F(X)$ と $g$ 一意な準同型をマグナス群 $\Gamma(X)$ に変換し、すべての $x \in X$ (cf. 定理) に対して $g(x) = 1 + x$ を表します。 1)。

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
