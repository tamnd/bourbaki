---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 6
section_title: The Hausdorff series
lang: ja
source: lie-i-iii
book_pages: 155-164, 201-204
pdf_pages: 0173-0182, 0219-0222
extraction: ocr
subsections:
    - "no": 1
      title: EXPONENTIAL AND LOGARITHM IN FILTERED ALGEBRAS
      page: 155
      pdf_page: 173
    - "no": 2
      title: HAUSDORFF GROUP
      page: 157
      pdf_page: 175
    - "no": 3
      title: LIE FORMAL POWER SERIES
      page: 158
      pdf_page: 176
    - "no": 4
      title: THE HAUSDORFF SERIES
      page: 160
      pdf_page: 178
    - "no": 5
      title: SUBSTITUTIONS IN THE HAUSDORFF SERIES
      page: 161
      pdf_page: 179
statements: 14
exercises: 6
content_sha256: 21def2f131143ec0c5e5047d8420a7421a65bc846c049946461371a219dad36a
translated_from: content/en/lie/II/06_s6_the_hausdorff_series.md
translation_method: google
source_content_sha256: 415bac69237edc26c3196e7b8c6ae4c55426a40b051a938d4b7c3803c5c86eba
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 5141a128cfd3e70df6cdcfb622334a6c715f81aef2bb96f55caecca4b7e575af
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。ハウスドルフ系列

*この段落では、$K$ が特性 0 の体であると仮定します。

### 1. フィルタリングされた代数の指数と対数

$A$ をハウスドルフである単一結合代数とし、実際の濾過 $(A_\alpha)$ で完成します。 $m = A_0^+ = \bigcup_{\alpha > 0} A_\alpha$と書きます。

$x \in m$ の場合、ファミリー $(x^n/n!)_{n \in \mathbf{N}}$ は合計可能です。私たちは書きます

$$
e^x = \exp x = \sum_{n \geqslant 0} x^n/n!.
$$

次に、$\exp(x) \in 1 + m$ と写像 $\exp : m \to 1 + m$ は、$A$ の *指数関数写像* と呼ばれます。

すべての $y \in 1 + m$ について、家族 $((-1)^{n-1}(y-1)^n/n)_{n \geqslant 1}$ は合計可能です。私たちは書きます

$$
\log y = \sum_{n \geqslant 1} (-1)^{n-1}(y-1)^n/n.
$$

次に、$\log y \in m$ と写像 $\log : 1 + m \to m$ は、$A$ の *対数写像* と呼ばれます。

#### 命題 1 {#lie-ii-s6-prop-1 .statement tag=0A61}

*指数関数写像は $m$ から $1 + m$ への準同型性であり、対数写像は逆準同型性です。*

$x \in A_\alpha$、$\frac{x^n}{n!} \in A_{n\alpha}$の場合。したがって、指数関数を定義する系列は、$\alpha > 0$ の集合 $A_\alpha$ のそれぞれで一様に収束します。 $A_\alpha$ は $m$ と $m = \bigcup_{\alpha > 0} A_\alpha$ でオープンなので、指数関数写像は連続です。対数写像が連続であることも同様に示すことができます。

$e$ と $l$ を、定数項を持たない正式な冪系列とします。

$$
e(X) = \sum_{n \geq 1} \frac{X^n}{n!}, \quad l(X) = \sum_{n \geq 1} (-1)^{n-1} X^n / n.
$$

私たちは (*代数*, 章 IV, § 6, no. 9) $e(l(X)) = l(e(X)) = X$ が $\hat{A}(\{X\}) = K[[X]]$ であることを知っています。代入 (§ 5, no. 1) により、次のように推測されます。

$$
e(l(x)) = l(e(x)) = x
$$

$x \in m$の場合。として

$$
\exp x = e(x) + 1, \quad \log(1 + x) = l(x)
$$

すぐにそうなります

$$
\log \exp x = x, \quad \exp \log(1 + x) = 1 + x
$$

$x$ の $m$、よって命題について。

#### 注意 {#lie-ii-s6-n1-rem-1 .statement tag=0A62}

(1) $x \in m, y \in m$ と $x$ と $y$ が通勤している場合、

$$
\exp(x + y) = \exp(x) \exp(y),
$$

ファミリ $\left( \frac{x^i}{i!} \cdot \frac{y^j}{j!} \right)_{i,j \in \mathbf{N}}$ は合計可能であるため (cf. *代数*, 章 IV, § 6, no. 9, 命題 11)。

(2) 系列 $e$ と $l$ には定数項が無く、$A_\alpha$ は$A$、$\exp A_\alpha \subset 1 + A_\alpha$、$\log(1 + A_\alpha) \subset A_\alpha$ よって $\exp A_\alpha = 1 + A_\alpha$、$\log(1 + A_\alpha) = A_\alpha$ の閉理想です。 $\alpha > 0$。

(3) $B$ を完全なハウスドルフ フィルタリングされたユニタル結合代数と $n = \bigcup_{\alpha > 0} B_\alpha$ とします。 $f$ を $A$ から $B$ への連続単位準同型とし、$f(m) \subset n$ とします。次に、$x \in m$ の場合は $f(\exp x) = \exp f(x)$、$y \in 1 + m$ の場合は $f(\log y) = \log f(y)$ です。たとえば、次の式の最初の式を示します。

$$
f(\exp x) = \sum_{n \geq 0} f(x^n)/n! = \sum_{n \geq 0} f(x)^n/n! = \exp f(x).
$$

(4) E を単位結合代数とする。 a が E の冪零元である場合、家族 $\left( \frac{a^n}{n!} \right)_{n \in \mathbf{N}}$ には有限台があり、$\exp a = \sum_{n \geq 0} a^n / n!$ と書きます。 $b - 1$ が無能である場合、元 b は単能性です。それから書きます

$$
\log b = \sum_{n \geq 1} (-1)^{n-1} (b - 1)^n / n.
$$

関係 $e(l(X)) = l(e(X)) = X$ から、写像 $a \mapsto \exp a$ は E の冪零元の集合の全単射を E の単能性元の集合に重ねたものであり、$b \mapsto \log b$ はその逆写像であると推測します。

### 2. ハウスドルフ群

Xを集合とします。 § 5の記法を使用します。 1 と 2。自由なリー代数 L(X) は、A(X) (§ 3, no. 1, 定理 1) の標準像と識別されます。 $\hat{A}(X)$ の L(X) の閉包を $\hat{L}(X)$ で表します。つまり、形の $\hat{A}(X)$ $a = \sum_{n \geq 1} a_n$ の元の集合で、すべての $n \geq 0$ に対して $a_n \in L^n(X)$ になります。これは$\hat{A}(X)$の嘘部分代数をフィルタリングしたものです。

#### 定理 1 {#lie-ii-s6-thm-1 .statement tag=0A63}

*$\hat{A}(X)$から$\hat{L}(X)$の指数関数写像の制限は、マグナス群$\Gamma(X)$の閉じた部分群に対する$\hat{L}(X)$の全単射です。

$A(X) = A, A^n(X) = A^n, \hat{A}(X) = \hat{A}, L^n(X) = L^n, \hat{L}(X) = \hat{L}, \Gamma(X) = \Gamma$と書きます。 B を $B^n = \sum_{i+j=n} A^i \otimes A^j$ で定義される型 $\mathbf{N}$ の目盛をもつ代数 $A \otimes A$ とします。 $\hat{B} = \prod_{n \geq 0} B^n$ を、関連する完全にフィルター処理された代数 (*可換代数*, 章 III, § 2, no. 12, *例* 1) とします。 § 3, no. 1、系 1 ～ 定理 1 で定義された余積 $c : A \to A \otimes A$ は、次数 0 に等級付けされるため、準同型 $\hat{c} : \hat{A} \to \hat{B}$ への連続性により拡大するとなります。

$$
\hat{c}\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} c(a_n) \quad \text{for } a_n \in A^n.
$$

また、$\hat{A}$ の定義する連続準同型 $\delta'$ と $\delta''$ を $\hat{B}$ に変換します。

$$
\delta'\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (a_n \otimes 1), \qquad \delta''\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (1 \otimes a_n) \quad \text{for } a_n \in A^n.
$$

§ 3, no. 1 の系 2 から定理 1 までにより、$L^n$ は $a_n \in A^n$ の集合となり、$c(a_n) = a_n \otimes 1 + 1 \otimes a_n$ となります。したがって、$\hat{L}$ は $a \in \hat{A}$ の集合となり、次のようになります。

$$
\hat{c}(a) = \delta'(a) + \delta''(a).
$$

$\Delta$ を 1 に等しい定数項の $b \in \hat{A}$ の集合および満たす関係とします

$$
\hat{c}(b) = \delta'(b) \cdot \delta''(b),
$$

他の $b = \sum_{n \geq 0} b_n$ の語、集合では、すべての $n \geq 0$、$b_0 = 1$、$c(b_n) = \sum_{i+j=n} b_i \otimes b_j$ が $n \geq 0$ に対して $b_n \in \mathbf{A}^n$ になります。後者の特徴付けは、$\Delta$が$\Gamma$の閉じた部分集合であることを示しています。 $\hat{\epsilon}$、$\delta'$、$\delta''$ は環準同型であり、$\delta'(\hat{\mathbf{A}})$ のすべての元は、$\delta''(\hat{\mathbf{A}})$、制限から $\Gamma$ のすべての元と交換します。 写像 $c$ と $\delta'\delta''$ は群準同型で、$\Delta$ は $\Gamma$ の部分群です。

no. 1の命題1により、$\hat{\mathbf{A}}$の指数写像は、集合の全単射、$\hat{\mathbf{A}}$の元の$\hat{\mathbf{A}}^+$となり、$\Gamma$への定数項はありません。 $a \in \hat{\mathbf{A}}^+$と$b = \exp a$としましょう。 $\hat{\epsilon}$ は連続する環準同型なので、

$$
\hat{\epsilon}(b) = \hat{\epsilon}\left( \sum_{n \geq 0} a^n/n! \right) = \sum_{n \geq 0} \hat{\epsilon}(a)^n/n! = \exp \hat{\epsilon}(a).
$$

関係

$$
\delta'(b) = \exp \delta'(a), \quad \delta''(b) = \exp \delta''(a)
$$

も同様に証明され、$\delta'(a)$ は $\delta''(a)$ (no. 1, 注意 1) と可換であるため、

$$
\delta'(b) \delta''(b) = \exp (\delta'(a) + \delta''(a)).
$$

したがって、$a$ は、$b$ が (4) を満たす場合に限り、(3) を満たします。これは、定理を証明します。

#### 注意 {#lie-ii-s6-n2-rem-1 .statement tag=0A64}

上の証明は、$\exp(\hat{\mathbf{L}})$が$b$満たすの$\Gamma$からなるの部分群$\Delta$であることを示しています。

したがって、$\Delta$ の群法則は、指数関数写像によって $\hat{\mathbf{L}}$ に輸送できます。他の語では、$\hat{\mathbf{L}}$ は、次の式で与えられる合成 $(a, b) \mapsto a \mathbin{\mathbf{h}} b$ の法則を含む完全なトポロジー 群です。

$$
a \mathbin{\mathbf{h}} b = \log(\exp a \cdot \exp b).
$$

このようにして得られたトポロジカル群は *Hausdorff 群* (K を基準とした X から導出) と呼ばれます。

$g$ を自由な群 $F = F(X)$ の準同型を $\Gamma$ にすると、$g(x) = \exp x$ は $x \in X$ になります。 $\exp x - 1 - x = \sum_{n \geq 2} x^n/n!$ は位数 $\geq 2$ であるため、$g$ は § 5, no. 3 の定理 1 による単射法です。したがって、*写像 $\log \circ g$ は、拡大する標準単射 $X \to \hat{\mathbf{L}}$* であるハウスドルフ群に、$F$ の単射準同型が入ります。

すべての整数 $m \geq 1$ について、$\hat{\mathbf{L}}$ の次数 $\geq m$ の要素の集合を $\hat{\mathbf{L}}_m$ で表し、$u - 1$ が次数 $\geq m$ であるような $u \in \Gamma$ の集合を $\Gamma_m$ で表します。 次に、$\hat{\mathbf{L}}_m = \exp(\Gamma_m)$ by 注意 2/no. 1; $(\Gamma_m)_{m \geq 1}$ は $\Gamma$ (§ 4, no. 5 命題 2) の統合中央フィルタであるため、$(\hat{\mathbf{L}}_m)_{m \geq 1}$ * は群 $\hat{\mathbf{L}}$* の統合中央フィルタです。

### 3. フォーマルな嘘をつく冪系列

#### 補題 1 {#lie-ii-s6-lem-1 .statement tag=0A65}

*$\mathfrak{g}$ をフィルターされたリー代数 (§ 4, no. 1)、$(\mathfrak{g}_\alpha)_{\alpha \in \mathbf{R}}$ をそのフィルター、$\alpha \in \mathbf{R}$ とします。 P を不定数 $(\Gamma_i)_{i \in I}$ (§ 2, no. 4) の次数 n の同次リー多項式とする。次に、家族ごとに $P((a_i)) \in \mathfrak{g}_{n\alpha}$ $(a_i)_{i \in I}$ の元の $\mathfrak{g}_\alpha$*。

次数 $n \geqslant 2$ のすべてのリー多項式は、形 $[Q, R]$ の項の有限和です。ここで、$Q$ と $R$ は、次数 $< n$ と和の有限です。 次数は $n$ (§ 2, no. 7、命題 7) に等しい。 補題の後に、$n$ に帰納法が続きます。

A *正式な嘘冪系列*† ($K$ に係数を含む) *不確定語* $(T_i)_{i \in I}$ は、リー代数 $\hat{L}((T_i)_{i \in I}) = \hat{L}(I)$ のいずれかの元です。このような元 $u$ は、$u_\nu \in L^\nu(I)$ である加算可能な族 $(u_\nu)_{\nu \in \mathbf{N}^{(I)}}$ の和として一意に書くことができます。

$I$ が *有限* であると仮定します。 $g$ を、$g = \bigcup_{\alpha > 0} g_\alpha$ となるような完全なハウスドルフ フィルタリングされたリー代数とします。 $t = (t_i)_{i \in I}$ を $g$ の元の家族とします。

#### 命題 2 {#lie-ii-s6-prop-2 .statement tag=0A66}

*準同型* $f_t : L(I) \to g$ *そのような* $f_t(T_i) = t_i$ (§ 2, no. 4) *連続性によって 1 つだけの連続準同型* $\hat{f}_t$ *of* $\hat{L}(I)$ *into* $g$ に拡張できます。

すべての $i \in I$ に対して $t_i \in g_\alpha$ となるような $\alpha > 0$ が存在します。したがって、すべての $\nu$ (補題 1) に対して $f_t(L^\nu(I)) \subset g_{|\nu| \wedge \alpha}$ となり、これは $\hat{f}_t$ の連続性を意味します。

$u \in \hat{L}(I)$の場合は、$u((t_i)) = \hat{f}_t(u)$と書きます。特に、$g = \hat{L}(I)$、$u = u((T_i))$ を取ると、一般的な場合、$u((t_i))$ は、Lie 形式冪系列 $u((T_i))$ の $T_i$ を $t_i$ に置き換えた結果と呼ばれます。 $u = \sum_{\nu \in \mathbf{N}^{(I)}} u_\nu$ の場合、$u_\nu \in L^\nu(X)$ の場合、ファミリー $(u_\nu((t_i)))_{\nu \in \mathbf{N}^{(I)}}$ は合計可能であり、
$$
u((t_i)) = \sum_{\nu \in \mathbf{N}^{I}} u_\nu((t_i)).
$$

$\sigma$ を $g$ の連続準同型として、$g' = \bigcup_{\alpha > 0} g'_\alpha$ となるような完全なハウスドルフ フィルタリングされたリー代数 $g'$ とします。すべての *有限* 家族 $t = (t_i)_{i \in I}$、元、$g$、およびすべての $u \in \hat{L}(I)$ について、
$$
\sigma(u((t_i))) = u((\sigma(t_i))),
$$
準同型 $\sigma \circ \hat{f}_t$ は連続し、$i \in I$ の場合写像 $T_i$ から $\sigma(t_i)$ までです。

$u = (u_j)_{j \in J}$ を $\hat{L}(I)$ の元の *有限* 族とし、$v \in \hat{L}(J)$ とします。 $v$ の $T_j$ を $u_j$ に置き換えることで、$v \circ u$ で示される $\hat{L}(I)$ の元 $w = v((u_j)_{j \in J})$ が得られます。それから
$$
w((t_i)_{i \in I}) = v((u_j((t_i)_{i \in I}))_{j \in J})
$$
方程式 $w = v((u_j)_{j \in J})$ で連続準同型 $\hat{f}_t$ を操作することでわかるように、すべての *有限* ファミリ $t = (t_i)_{i \in I}$ of 元 of $g$ について。

$u = \sum_{\nu \in \mathbf{N}^{I}} u_\nu \in \hat{L}(I)$、ここで$u_\nu \in L^\nu(I)$とします。 $g^I$ から $g$ への写像 $\tilde{u}$ $(t_i) \mapsto u((t_i))$ は *連続*: $\alpha > 0$ と開いた集合 $g_\alpha$ のそれぞれにおいて、$\tilde{u}_\alpha$ の族は一様に合計可能であり、それぞれが次のことを証明するだけで十分です。 $\tilde{u}_\nu$は連続で、$|\nu|$の帰納法による明らかです。

† 嘘の正式な冪系列は、一般に *代数*、章 IV, § 6 の意味での正式な冪系列ではありません。

### 4. ハウスドルフ系列

{U, V} を 2 つの元からなる集合とします。

#### 定義 1 {#lie-ii-s6-def-1 .statement tag=0A67}

*元* $H = U \circledast V = \log(\exp U \cdot \exp V)$ (no. 2) *of リー代数* $\hat{L}_\mathbf{Q}(\{U, V\})$ *は不定数* U *と* V のハウスドルフ系列と呼ばれます。

合計次数 n (それぞれ多次 $(r, s)$) の H の同次成分を $H_n$ (それぞれ $H_{r,s}$) で表します。それから

$$
H = \sum_{n \geq 0} H_n = \sum_{r, s \geq 0} H_{r,s}, \quad H_n = \sum_{r+s=n \atop r, s \geq 0} H_{r,s}.
$$

#### 定理 2 {#lie-ii-s6-thm-2 .statement tag=0A68}

*r と s が 2 正の整数で、* $r + s \geq 1$ の場合、 *then* $H_{r,s} = H'_{r,s} + H''_{r,s}$、 *where*

$$
(r + s)H'_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s-1 \\ 1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} (V)
$$

$$
(r + s)H''_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) (U).
$$

$\hat{A}_\mathbf{Q}(\{U, V\})$、$\exp U \cdot \exp V = 1 + W$ では、$W = \sum_{r+s \geq 1} \frac{U^r V^s}{r! s!}$、よって

$$
H = \sum_{m \geq 1} (-1)^{m-1} W^m / m \text{ (no. 2)}, \text{ that is:}
$$

$$
H_{r,s} = \sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_m + s_m \geq 1}}
\prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!}.
$$

$n \geq 1$ の $P_n(x_1, \ldots, x_n) = \frac{1}{n} \left( \prod_{i=1}^{n-1} (\mathrm{ad}\, x_i) \right)(x_n)$ と $\{U, V\}$ の $x_1, \ldots, x_n$ によって定義される線形写像 $P_n$ は、$A^n_\mathbf{Q}(\{U, V\})$ から $L^n_\mathbf{Q}(\{U, V\})$ への射影子 (§ 3, no. 2、系から命題 1); $H_{r,s}$ 属するから $L^{r+s}_\mathbf{Q}(\{U, V\})$、$H_{r,s} = P_{r+s}(H_{r,s})$ のように。今

$$
P_{r+s} \left( \prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!} \right)
= \frac{1}{r+s} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} \frac{(\mathrm{ad}\, V)^{s_{m-1}}}{s_{m-1}!} (V)
$$

$s_m \geqslant 1$のときと

$$
(13)\quad P_{r+s}\left(\prod_{i=1}^{m} \frac{U r_i}{r_i!} \frac{V s_i}{s_i!}\right) = \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m-1}}{r_m!} \right)(U)
$$

$r_m \geqslant 1$ と $s_m = 0$ のとき。さらに、$p \geqslant 2$と$(\mathrm{ad}\ t)^0.t = t$であれば、明らかに$(\mathrm{ad}\ t)^{p-1}.t = 0$です。したがって、$s_m \geqslant 2$ のとき (12) の両辺は零となり、$r_m \geqslant 2$ のとき (13) の両辺は零となります。 $H'_{r,s}$ は型の項の和であり、$H''_{r,s}$ は型の項の和であるため、次に定理が続きます。

#### 注意 {#lie-ii-s6-n4-rem-1 .statement tag=0A69}

(1) $A(X)$ の (§ 3, no. 2, 注意) 射影子 $Q$ を $L(X)$ に定義し、$a \in L(X)$ と $m \geqslant 2$ および $Q(1) = 0$ に対して $Q(a^m) = 0$ を定義しました。それからすぐに$H = Q(\exp H) = Q(\exp U.\exp V)$、よって

$$
(14)\quad H_{r,s} = Q \left( \frac{U^r V^s}{r! s!} \right) \quad \text{for } r + s \geqslant 1.
$$

(2) 私たちは、

$$
(15)\quad H(U, V) \equiv U + V + \frac{1}{2}[U, V] + \frac{1}{12}[U, [U, V]] \\
+ \frac{1}{12}[V, [V, U]] - \frac{1}{24}[U, [V, [U, V]]]
$$
モジュロ$\sum_{n \geqslant 5} L^n(\{U, V\})$。

(3) 整数 $n \neq 1$、よってごとに $H_{0,n} = H_{n,0} = 0$

$$
(16)\quad H(U, 0) = H(0, U) = U.
$$

一方、$[U, -U] = 0$としては、

$$
(17)\quad H(U, -U) = 0.
$$

### 5. ハウスドルフでの選手交代系列

$K$ は体含む $\mathbf{Q}$ であるため、ハウスドルフ系列は、$K$ に係数が入ったリー形式冪系列と考えることができます。したがって、$g$ が $g = \bigcup_{\alpha > 0} g_\alpha$ でリー代数をフィルタリングした完全なハウスドルフである場合、$g$ の $a, b$ は、$a$ と $b$ で$U$ と $V$ を置き換えることができます。 $H$ (cf. no. 3 および § 2, no. 5、注意)。

特に、$A$ を完全なハウスドルフ フィルター処理されたユニタル結合代数とします。 $\alpha \in \mathbf{R}$ を $m = \bigcup_{\alpha > 0} A_\alpha$ と $m_\alpha = A_\alpha \cap m$ と書きます。したがって、$\alpha > 0$ は $m_\alpha = A_\alpha$、$\alpha \leqslant 0$ は $m_\alpha = m$ となります。ブラケット $[a, b] = ab - ba$ を使用すると、$m$ は完全なハウスドルフ フィルター付きのリー代数となり、上記を適用できます。この記法により、no. 1 の 1 つである命題が​​完成する次の結果が得られます。

#### 命題 3 {#lie-ii-s6-prop-3 .statement tag=0A6A}

*$a \in m, b \in m$の場合は、$\exp H(a, b) = \exp a . \exp b$。*

$a, b$ を $m$ に入れます。 $a \in A_\alpha$ と $b \in A_\alpha$ のような $\alpha > 0$ が存在します。 そして、マグナス代数 $\hat{A}(\{U, V\})$ $A$ 写像 $U$ から $a$ および $V$ から $b$ (§ 5, no. 1、命題 1) への連続する準同型 $\theta$ が存在します。

$\theta$ から $\hat{L}(\{U, V\})$ への制限は、$L(\{U, V\})$ から $m$ へのリー代数の連続準同型で、$U$ (それぞれ $V$) を $a$ (それぞれ $b$) に写像します。 no. 3 の公式 (6) により、$\theta(H) = H(a, b)$ になります。 次に、関係の両側に連続する準同型 $\theta$ を適用するだけで十分です。
$$
\exp H(U, V) = \exp U . \exp V
$$
no. 1 の *注意 3* を考慮します。

#### 注意 1 {#lie-ii-s6-n5-rem-1 .statement tag=0A6B}

$a$ と $b$ が可換である場合、次数 $\geq 2$ のすべての同次リー多項式に対して、$r + s \geq 2$ に対する $H_{r,s}(a, b) = 0$ は $(a, b)$ で零になります。その後、$H(a, b) = a + b$ と命題 3 が公式を回復します
$$
\exp(a + b) = \exp a . \exp b.
$$

#### 命題 4 {#lie-ii-s6-prop-4 .statement tag=0A6C}

*$g$ を、$g = \bigcup_{\alpha > 0} g_\alpha$ となるような完全なハウスドルフ フィルタリングされたリー代数とします。 写像 $(a, b) \mapsto H(a, b)$ は $g$ の群法則と $g$ の位相と互換性があり、その下では $0$ は単位元であり、$-a$ はすべての $a \in g$ の $a$ の逆です。*

$g \times g$ から $g$ への写像 $(a, b) \mapsto H(a, b)$ は連続です (no. 3)。 写像 $a \mapsto -a$ は明らかに連続であるため、関係を証明するだけで十分です
$$
\begin{align*}
(18) \quad & H(H(a, b), c) = H(a, H(b, c)) \\
(19) \quad & H(a, -a) = 0 \\
(20) \quad & H(a, 0) = H(0, a) = a
\end{align*}
$$
$g$の$a, b, c$用。 no. 3 の公式 (7) により、$a, b, c$ が 3 つの不定数と $g = \hat{L}(\{a, b, c\})$ の場合、これらの公式を証明するだけで十分です。現在、写像から$\hat{L}(\{a, b, c\})$までの指数関数制限は単射となり、命題3までにマグナス代数$\hat{A}(\{a, b, c\})$になります。
$$
\begin{align*}
\exp H(H(a, b), c) &= \exp H(a, b) . \exp c = \exp a . \exp b . \exp c \\
\exp H(a, H(b, c)) &= \exp a . \exp H(b, c) = \exp a . \exp b . \exp c \\
\exp H(a, -a) &= \exp a . \exp(-a) = \exp(a - a) = \exp 0 \\
\exp H(a, 0) &= \exp a . \exp 0 = \exp a \\
\exp H(0, a) &= \exp 0 . \exp a = \exp a.
\end{align*}
$$
これにより、関係 (18) ～ (20) が成立します。

#### 注意 {#lie-ii-s6-n5-rem-2 .statement tag=0A6D}

(2) $g$ をリー代数 $\hat{L}(X)$ とします。 群法則は上記の命題一致するで導入され、no. 2 で定義された法則が追加されます。その他の語では、
$$
a \mathbin{\mathbf{h}} b = H(a, b) \quad \text{for } a, b \text{ in } \hat{L}(X);
$$
したがって、ハウスドルフ群法則はハウスドルフ系列によって与えられます。

(3) $g$ を、中央下部系列によって定義される積分濾過 ($\mathscr{C}^n g$) を使用して、リー代数とします。 $\mathscr{C}^m g = \{0\}$となるような$m \geq 1$が存在するとします。濾過 $(\mathscr{C}^n g)_{n \geq 1}$ から派生した位相を使用すると、リー代数 $g$ はハウスドルフであり、完全であり、さらには離散的です。次に、$g$ の $a_1, \ldots, a_r$ と、次数 $\geq m$ のすべての同次リー多項式 $P$ に対して $P(a_1, \ldots, a_r) = 0$ が計算されます。特に、$r + s \geq m$ と系列 $H(a, b) = \sum_{r,s} H_{r,s}(a, b)$ の $H_{r,s}(a, b) = 0$ には、非ゼロ項の有限の数しかありません。 $g$ 上の群法則 $(a, b) \mapsto H(a, b)$ は、多項式写像 (§ 2, no. 4) になります。

#### 命題 5 {#lie-ii-s6-prop-5 .statement tag=0A6E}

*$K_{r,s}$を多度$(r, s)$の$H(U + V, -U)$の成分とします。それから*
$$
K_{n,1}(U, V) = \frac{1}{(n+1)!} (\operatorname{ad} U)^n(V) \quad \text{for } n \geq 0.
$$

$K(U, V) = H(U + V, -U)$、$K_1(U, V) = \sum_{n \geq 0} K_{n,1}(U, V)$と書きます。 $\hat{A}(\{U, V\})$ の$U$ によって左 (それぞれ右) 乗法によってL (それぞれ R) で表します。

書けます
$$
e^{U}V e^{-U} = \sum_{p, q} \frac{U^p}{p!} V \frac{(-U)^q}{q!}
= \sum_{n \geq 0} \frac{1}{n!} \left( \sum_{p+q=n} \frac{n!}{p!q!} (L^p(-R)^q) \cdot V \right)
= \sum_{n \geq 0} \frac{1}{n!} (L - R)^n V
$$
したがって
$$
e^{U}V e^{-U} = \sum_{n \geq 0} \frac{1}{n!} (\operatorname{ad} U)^n V.
$$
これで、$A(\{U, V\})$ の理想的な $\sum_{m \geq 0} \sum_{n \geq 2} A^{m,n}(\{U, V\})$ を法として計算するが得られます。 $n \geq 1$の皆さん、
$$
(U + V)^n \equiv U^n + \sum_{i=1}^{n-1} U^i V U^{n-1-i}
$$
よって
$$
(\operatorname{ad} U)(U + V)^n \equiv ((L - R) \sum_{i=1}^{n-1} L^i R^{n-i}) \cdot V \\
\equiv (L^n - R^n) \cdot V \\
\equiv U^n V - V U^n.
$$
したがって、
$$
(\operatorname{ad} U) \cdot e^{U+V} \equiv e^{U}V - V e^{U}
$$
$n$ を合計します。

一方、$K_1(U, V) \equiv K(U, V)$ と $e^{K_1(U, V)} \equiv 1 + K_1(U, V)$ なので
$$
K_1 \equiv e^K - 1 \equiv e^{U+V}e^{-U} - 1
$$
by 命題 3. 私たちは次のように推測します
$$
\begin{align*}
(\mathrm{ad}\ U)K_1 &\equiv Ue^{U+V}e^{-U} - e^{U+V}e^{-U}U \\
&\equiv (e^{UV} - Ve^U)e^{-U} \quad \text{(by (23))} \\
&\equiv e^{UV}e^{-U} - V \\
&\equiv \sum_{n \geq 1} \frac{1}{n!} (\mathrm{ad}\ U)^n V \quad \text{(by (22))} \\
&\equiv (\mathrm{ad}\ U)\left( \sum_{n \geq 0} \frac{(\mathrm{ad}\ U)^n}{(n+1)!} V \right).
\end{align*}
$$
その後、§ 2, no. 11の*注意*を適用すれば十分です。

### 練習問題 {#lie-ii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
