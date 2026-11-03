---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 10
section_title: Extensions of a valuation to a transcendental extension
lang: ja
source: ac-i-vii
book_pages: 434-440, 471-473
pdf_pages: 0452-0458, 0489-0491
extraction: ocr
subsections:
    - "no": 1
      title: THE CASE OF A MONOGENOUS TRANSCENDENTAL EXTENSION
      page: 434
      pdf_page: 452
    - "no": 2
      title: THE RATIONAL RANK OF A COMMUTATIVE GROUP
      page: 437
      pdf_page: 455
    - "no": 3
      title: THE CASE OF ANY TRANSCENDENTAL EXTENSION
      page: 438
      pdf_page: 456
statements: 14
exercises: 2
content_sha256: 25c0b69b829cd054e34f6df669a25f746857a11ba14e214ed0ef985cc7338e4c
translated_from: content/en/ac/VI/10_s10_extensions_of_a_valuation_to_a.md
translation_method: google
source_content_sha256: d3545f7135c1b975d777e05ac5e9cc067935aed03dd234e1d2fffc43e8d3d49f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 7939d0311a0f51789e7628c04c5a44ddb4418d1acb090fcdad39442f2ab8a754
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 10. 拡大の超越的な評価拡大

### 1. 単一超越論の場合拡大

#### 補題 1 {#ac-vi-s10-lem-1 .statement tag=04Y5}

$K$ を *体*、$v$ を $K$ の評価、$\Gamma$ *その* 位数群、$\Gamma'$ を完全に注文した群含む $\Gamma$ とします。 $\xi$ *元/* $\Gamma'$。 $K(X)$ に *それ*、*に対して* $P = \sum_j a_j X^j$ ($a_j \in K$)、$w(P) = \inf_j (v(a_j) + j\xi)$ には *独自の評価が存在します。

§ 3, no. 2 の命題 4 までに、公式であることを示すだけで十分です

$$
w\left( \sum_j a_j X^j \right) = \inf_j (v(a_j) + j\xi)
$$

定義する環 $K[X]$ の評価。として

$$
v(a_j + b_j) + j\xi \geq \inf(v(a_j), v(b_j)) + j\xi = \inf(v(a_j) + j\xi, v(b_j) + j\xi),
$$

それは次のとおりです

$$
w(P + Q) \geq \inf(w(P), w(Q))
$$

$K[X]$の$P, Q$の場合、$w(P) \neq w(Q)$の場合は等式を保持します。私たちはそれを示します

$$
w(PQ) = w(P) + w(Q)
$$

$P = \sum a_j X^j$と$Q = \sum b_j X^j$の場合。 $i$ (それぞれ $k$) を整数 $j$ の最小値とし、$v(a_j) + j\xi$ (それぞれ $v(b_j) + j\xi$) が最小値に達するとします。 $a$ (それぞれ $\beta$) がこの最小値を表すものとします。 $\mathbf{N}$の$j, j'$については、

$$
w(a_j b_{j'} X^{j+j'}) = v(a_j) + j\xi + v(b_{j'}) + j'\xi \geq a + \beta,
$$

(2)によるよって $w(PQ) \geq a + \beta$。ここで、$PQ$ の次数 $i + k$ の項 $c X^{i+k}$ を考えてみましょう。次に$c = \sum_{n \in \mathbf{Z}} a_{i+n} b_{k-n}$; $i$ と $k$、元の選択による

$$
w(a_{i+n} b_{k-n} X^{i+k}) = v(a_{i+n}) + (i+n)\xi + v(b_{k-n}) + (k-n)\xi
$$

最小値値 $a + \beta$ は 1 回と、$n = 0$ で 1 回のみとなります。したがって、(1) により、$w(c X^{i+k}) = a + \beta$、よって、

$$
w(PQ) = \alpha + \beta = w(P) + w(Q).
$$

#### 命題 1 {#ac-vi-s10-prop-1 .statement tag=04Y6}

$K$ を *体*、$v$ *評価* $K$、$\Gamma$ *その位数群*、$\Gamma'$ *合計注文群含む* $\Gamma$ *そして* $\xi$ *元 of* $\Gamma'$ *そのような関係* $n\xi \in \Gamma, n \in \mathbf{Z}$ *暗黙* $n = 0$。そして、*上* $K(X)$ *値を* $\Gamma'$ *さらに拡張* $v$ *そのような* $w(X) = \xi$ という *独自の評価が存在します。 * w *の*剰余体は* $v$ *の*位数群は部分群* $\Gamma + \mathbf{Z}\xi$ *of* $\Gamma'$です。

wの最初の一意性をお見せします。 $P = \sum_j a_j X^j$を$K[X]$の元とします。次に $w(a_j X^j) = v(a_j) + j\xi$ は、$a_j \neq 0$ のような単項式 $a_j X^j$ が w に対して明確な値を持つことを示しています。したがって、$w(P) = \inf_j (v(a_j) + j\xi)$ は、$K[X]$ 上の w の一意性 (したがって、$K(X)$ も) と、w の位数群が $\Gamma + \mathbf{Z}\xi$ であるという事実の両方を示します。さらに、$P \neq 0$ の場合、$a \in K^*, n \in \mathbf{N}, u \in K(X)$ と $w(u) > 0$ を、$P = a X^n (1 + u)$ と書くことができることがわかります。したがって、$K(X)$ のすべての元 $R \neq 0$ は形で書くことができます
$$
R = b X^n (1 + u'),
$$
ここで、$b \in K^*, n \in \mathbf{Z}, u' \in K(X)$ と $w(u') > 0$; $w(R) = v(b) + n \xi$ なので、$v(b) = 0$ と $n = 0$ の場合に限り、$w(R) = 0$ になります。したがって、$w(R) = 0$、$R$、$b$ が$w$ のイデアルを法として合同である場合、$w$ の剰余体が $v$ の剰余体に等しいことがわかります。

最後に、補題 1 から$w$ の存在が続きます。

#### 命題 2 {#ac-vi-s10-prop-2 .statement tag=04Y7}

*$K$を体、$v$を$K$、$\Gamma$を位数群、$k$を剰余体とします。 $w$の剰余体$k'$における$X$の$w(X) = 0$と像$t$が$k$を超越するように、$v$を拡張する$K(X)$に独自の評価$w$が存在します。 $w$ の位数群は $v$ と等しく、その剰余体は $k(t)$ です。*

$w$ の一意性を示すには、$P = \sum_j a_j X^j$ が $K[X]$ の非ゼロ元である場合、次のことを示すだけで十分です。
$$
w(P) = \inf_j (v(a_j)).
$$
$K^*$ の元によって割る $P$ が得られ、すべての $j$ に対して $v(a_j) \geq 0$ があり、$v(a_j)$ の 1 つが零であると仮定します。 $w(X) = 0$ として、$P$ は $w$ のリングに属します。 $k$ の $a_j$ の正準イメージに $\bar{a}_j$ を書き込むと、剰余フィールド $k'$ の $P$ の正準イメージは $\sum_j \bar{a}_j t^j$ になります。 $t$ は $k$ を超越していて、$\bar{a}_j$ の 1 つが非ゼロであるため、この画像は非ゼロです。
$$
w(P) = 0 = \inf_j (v(a_j)).
$$
ここで$w$の存在を示します。 公式 $w(P) = \inf_j (v(a_j))$ ($P = \sum_j a_j X^j$ の場合) 定義するは、補題 1 により、$K(X)$ の評価$w$ となり、$w$ は明らかに $v$ と同じ位数群になります。 次に$w(X) = 0$。 $w$の剰余体$k'$における$X$の標準像$t$が$k$に対して超越的であることを示します: $\sum_j \bar{a}_j t^j = 0$の場合、すべての$j$に対して$\bar{a}_j \in k$である場合、代表元$a$で表します$\bar{a}_j$の環の$v$、$w \left( \sum_j a_j X^j \right) > 0$。 よって $v(a_j) > 0$ はすべての $j$ に対して、したがって $\bar{a}_j = 0$ はすべての $j$ に対してなります。 最後に、$k' = k(t)$: $K(X)$ のすべての要素 $R$ は $R = c \left( \sum_j a_j X^j \right) / \left( \sum_j b_j X^j \right)$ で記述できることを示します。ここで、$c, a_j, b_j$ はすべての $j$ に対して $K$、$v(a_j) \geq 0$、$v(b_j) \geq 0$ にあり、$v(a_j)$ の 1 つと $v(b_j)$ の 1 つがゼロ。 $v(c) \geq 0$の場合に限り、$w(R) \geq 0$。 $f$ によって $w$ の環の $k'$ への正準準同型性を表し、
$$
f(R) = f(c) \left( \sum_j f(a_j) t^j \right) / \left( \sum_j f(b_j) t^j \right),
$$

それは私たちの主張を証明します。

#### 注意 {#ac-vi-s10-n1-rem-1 .statement tag=04Y8}

私たちが出会ったばかりの v の拡大から K(X) までの 2 つの型が唯一のものであると考えるべきではありません。 拡大の 3 番目の型が存在する可能性があります。ここで、$\Gamma'/\Gamma$ は捩れ群であり、$k'$ は $k$ の (必ずしも有限ではない) 代数拡大です。この 3 番目の型は、補題 1 (cf. § 3、練習問題 1) で説明されている手順によって必ずしも提供されるわけではありません。

### 2. 可換性群の有理数階数

#### 定義 1 {#ac-vi-s10-def-1 .statement tag=04Y9}

可換群 G の *有理階数は、ベクトル Q 空間* $G \otimes_{\mathbf{Z}} \mathbf{Q}$ の次元です。

This dimension may also be defined as the least upper bound (finite or infinite) of the cardinals $r$ such that there exist $r$ elements of G which are linearly independent over $\mathbf{Z}$ (*Algebra*, Chapter II, § 7, no. 10, Proposition 26). G の有理数階数は、G が捩れ群である場合に限り、*零* になります。 加法群 $\mathbf{R}^n$ の部分群、有理数階数一致するの概念については、*一般位相*、章 VII, § 1 で定義されています。

この段落の残りの部分では、可換群 G の有理数階数を $r(G)$ で表します。 $G'$ が G の部分群である場合、($\mathbf{Q}$ はフラット $\mathbf{Z}$ 加群であるため)、加法方程式が得られます。

$$
r(G) = r(G') + r(G/G').
$$

#### 命題 3 {#ac-vi-s10-prop-3 .statement tag=04YA}

*G を G の全順序可換群と H 部分群とします。$h(G)$ と $h(H)$ が G と H* の高さを表す場合 ($§ 4$, no. 4)、*その後不等式*

$$
h(G) \leq h(H) + r(G/H)
$$

*成り立ちます*。

実際、$G_0 \subset G_1 \subset \ldots \subset G_n$ を G の孤立した部分群の真に増加する数列とします。不等式を確立する必要があります。

$$
n \leq h(H) + r(G/H).
$$

$n = 0$の場合は明らかです。 $n \geq 1$として、$n$について帰納法で議論してみましょう。 適用帰納法の仮定から群 $G_{n-1}$ とその部分群 $H \cap G_{n-1}$ を取得します。

$$
n - 1 \leq h(H \cap G_{n-1}) + r(G_{n-1}/(H \cap G_{n-1})).
$$

次に、2 つの場合を区別します。

(a) $H \cap G_{n-1} = H$、その他の語 $H \subset G_{n-1}$。 不等式 (7) と書かれる場合があります

$$
n \leq h(H) + r(G_{n-1}/H) + 1.
$$

ここで、$G/G_{n-1}$ は 0 に減らされていない完全に順序付けられた群です。したがって、捩れ群および $r(G/G_{n-1}) \geq 1$ ではありません。 よって by (4)、$r(G/H) \geq r(G_{n-1}/H) + 1$。 (8) に代入すると、確かに目的の不等式 (6) が得られます。

(b) $H \cap G_{n-1} \neq H$。 $H \cap G_{n-1}$ は $H$ の孤立した部分群であるため、$h(H) > h(H \cap G_{n-1}) + 1$ を結論するとします。一方、明らかに$r(G/H) \geq r(G_{n-1}/(H \cap G_{n-1}))$。 (7) に代入すると、再び (6) が得られます。

#### 系 {#ac-vi-s10-n2-cor-1 .statement tag=04YB}

*完全に順序付けられた可換性群 G、$h(G) \leq r(G)$ に対して。* 命題 3 で集合 $H = (0)$ となります。

#### 命題 4 {#ac-vi-s10-prop-4 .statement tag=04YC}

* G を全順序可換群とする。 G が有限生成され、$h(G) = r(G)$ であるとします。この場合、G は辞書順に並べられた $\mathbf{Z}^{r(G)}$ と同型です。*

$r = r(G) = h(G)$と書きましょう。 $r = 0$の場合は、$G = (0)$。有限生成可換群の $r = 1$, 構造は、Z 上に G の同型 $j$ が存在することを示します (*代数*, 章 VII, § 4, no. 6, 定理 3)。ここで、Z には、その群構造と互換性のある合計 2 つの順序付け、つまり通常の順序付けとその逆の順序付けしかありません。したがって、$j$ または $-j$ は、通常の順序で Z に順序付けされた群 G の同型になります。

今、$r \geq 2$と仮定して、$r$について帰納法によって議論してみましょう。 H を高さ $r - 1$ の G の孤立した部分群とします。 次に、$r(H) + r(G/H) = r$ (公式 (4))、$r(H) \geq h(H) = r - 1$、$r(G/H) \geq h(G/H) = 1$ (系 ～ 命題 3)、よって $r(H) = r - 1$、$r(G/H) = 1$。 帰納法の仮定は、H が辞書順に並べられた $\mathbf{Z}^{r-1}$ と同型であることを示し、$r = 1$ の場合は、$G/H$ が Z と同型であることを示します。 Z は自由な Z モジュールであるため、H は G の *直因子* (*代数*、章 11、§ 1, no. 11、命題 21) です。 次に、次の補題は、G が辞書編集上の積 $H \times (G/H)$ と同型 (正準ではない) であることを示し、これで証明が完成します。

#### 補題 2 {#ac-vi-s10-lem-2 .statement tag=04YD}

*H を全順序可換群 G の孤立した部分群とします。H が G の直因子である場合、順序付き群 G は辞書編集的に順序付けされた群 $(G/H) \times H$ と同型です。

$j$ を G 上の $(G/H) \times H$ の同型とし、すべての $x \in H$ と $j(y, x)$ 属するについて H の剰余類に対して $j(0, x) = x$ となるようにします。 $(G/H) \times H$ は完全に順序付けされているため、$j$ が *増加する* であることを示すことになります。 (*集合理論*、章 III, § 1, no. 12、命題 11)。 $(y, x)$ を辞書順に並べた $(G/H) \times H$ の元 $\geq 0$ とします。 $y > 0$ の場合、H 含む $j(y, x)$ の剰余類は、元 $> 0$、よって $j(y, x) > 0$、それ以外の場合、$y \leq 0$ (§ 4, no. 2、命題 3) です。 $y = 0$と$x \geq 0$の場合、$j(y, x) = x \geq 0$。したがって、$j$ は確かに増加するです。

### 3. あらゆる超越的な拡大の場合

このNo.次の記法を使用します: $K$ は体、$K'$ 拡大は $K$、$v$ は $K$、$v'$ 拡大 $v$ の評価です。 $K$、$\Gamma$、$k$ (それぞれ $\Gamma'$ と $k'$) 位数群と $v$ の剰余体 (それぞれ $v'$)。次のように書きます。

$$
d(K'/K) = \dim.\mathrm{al},\ K' = \text{transcendence degree of } K' \text{ over } K;
$$
$$
s(v'/v) = \dim.\mathrm{al},\ k' = \text{transcendence degree of } k' \text{ over } k;
$$
$$
r(v'/v) = r(\Gamma'/\Gamma) = \text{rational rank of } \Gamma'/\Gamma,
$$

右辺が有限の場合。それ以外の場合は、$d(K'/K) = +\infty$ (それぞれ $s(v'/v) = +\infty, r(v'/v) = +\infty$) という規則を作成します。

#### 定理 1 {#ac-vi-s10-thm-1 .statement tag=04YE}

*$x_1, \ldots, x,$ を $v'$ の環の元とします。その $k'$ の標準像 $\overline{x}_i$ は、$K'$ の $k$ および $y_1, \ldots, y_r$ 元に対して代数的に独立しています。 $\Gamma'/\Gamma$ の $v'(y_j)$ の標準像は、$\mathbf{Z}$ に対して線形独立です。すると、$K'$ の $r+s$ 元 $x_1, \ldots, x, y_1, \ldots, y_r$ は、$K$ に対して代数的に独立です。 $v'$ から $K(x_1, \ldots, x, y_1, \ldots, y_r)$ の制限は、$k(\overline{x}_1, \ldots, \overline{x}_s)$ を剰余体として認め、*

$$
\Gamma + \mathbf{Z}v'(y_1) + \ldots + \mathbf{Z}v'(y_r)
$$

*位数群* として。

$r+s = 0$ であれば、私たちの主張は明らかです。 $r+s$の帰納法までに議論します。 $r' \leq r, s' \leq s$ と $r'+s' < r+s$ の場合、帰納法の仮定は、$K$ を $K(x_1, \ldots, x_s, y_1, \ldots, y_{r'})$ に置き換え、家族 $(x_1, \ldots, x_s), (y_1, \ldots, y_r)$ を $(x_{s'+1}, \ldots, x_s), (y_{r'+1}, \ldots, y_r)$ に置き換えると、定理 1 の仮説が成り立つことを示します。したがって、問題は次の 2 つのケースのいずれかに帰着します。

(a) 環 $v'$ には元 $x$ があり、$\overline{x}$ は $k$ を超越しています。その場合、$x$が$K$に対して超越的であり、$v'$から$K(x)$の制限が$k(\overline{x})$を剰余体として、$\Gamma$を位数群として認めることを示す必要があります。

(b) $K'$ には元 $y$ があり、関係 $nv'(y) \in \Gamma$ と $n \in \mathbf{Z}$ は $n = 0$ を暗示します。 $y$が$K$に対して超越的であり、$v'$から$K(y)$の制限が$k$を剰余体として、$\Gamma + \mathbf{Z}v'(y)$を位数群として認めることを示す必要がある。

ここで、§ 8, no. 1 の命題 1 は、$x$ (それぞれ $y$) できないが $K$ に対して代数的であることを示しています。 (a) の他の主張 (それぞれ (b)) のすぐ後に、no. 1 の命題 2 (それぞれ命題 1) が続きます。

#### 系 1 {#ac-vi-s10-thm-1-cor-1 .statement tag=04YF}

*不等式*

$$
s(v'/v) + r(v'/v) \leq d(K'/K)
$$

*成り立ちます。*

*さらに、$K'$が$K$の有限生成された拡大であり、等式が(9)で成立する場合、$\Gamma'/\Gamma$は有限生成された$\mathbf{Z}$加群であり、$k'$は有限生成された拡大である$k$.*

$r$ と $s$ を自然数として、 $r \leq r(v'/v)$ と $s \leq s(v'/v)$ が成り立つようにします。 $r+s \leq d(K'/K)$ を示し、これで (9) が証明されます。 仮定までに、満たす定理 1 の仮説である $K'$ のうち、元 $x_1, \ldots, x, y_1, \ldots, y$ が存在します。

したがって、それらは $K$ 上で代数的に独立しており、これは不等式 $r + s < d(K'/K)$ を示します。

$K'$ が $K$ の有限生成された拡大である場合、$d(K'/K)$ は有限であるため、$s(v'/v)$ と $r(v'/v)$ も有限です。それらを$s$と$r$で表します。 $K'$ の元 $x_1, \ldots, x_s, y_1, \ldots, y_r$ と定理 1 の仮説満たすが存在します。 $r + s = d(K'/K)$ の場合、これらの元形は $K$ に対する $K'$ の超越基底であり、したがって $K'$ は $K'' = K(x_1, \ldots, y_r)$ の有限代数拡大です。 $\Gamma''$と$k''$を$v'$から$K''$の制限の位数群と剰余体とします。 定理 1 により、$\Gamma''/\Gamma$ は有限生成された $\mathbf{Z}$ モジュールであり、$k''$ は有限生成された$k$ の純粋な拡大です。 一方、$K'$は$K$の有限代数拡大であるため、$\Gamma'/\Gamma$は有限群、$k'$は$k''$(§ 8, no. 1、補題2)の有限代数拡大です。 これは系を証明します。

#### 系 2 {#ac-vi-s10-thm-1-cor-2 .statement tag=04YG}

*h と h' を v と v' の高さとします。それから*
$$
s(v'/v) + h' \leq d(K'/K) + h.
$$
命題 3、$h' \leq r(v'/v) + h$までに。

#### 系 3 {#ac-vi-s10-thm-1-cor-3 .statement tag=04YH}

*$K'$ が $K$ の有限生成された拡大であり、$\Gamma$ が $\mathbf{Z}^{h'}$ (辞書順に並べられている) と同型で、公式 (10) に等式があるとします。次に、$\Gamma'$ は (辞書編集順に) $\mathbf{Z}^{h'}$ と同型であり、$k'$ は $k$ の有限生成された拡大です。*

(10) に等式がある場合、(9) には等式があり、$k'$ は $k$ の有限生成拡大であり、$\Gamma''$ は有限生成 $\mathbf{Z}$ 加群であるという事実がよって存在します。さらに、(9) と (10) を比較すると、$h' - h = r(\Gamma'/\Gamma)$、よって $h' = r(\Gamma')$、および命題 4 (no. 2) は、$\Gamma'$ が辞書順に並べられた $\mathbf{Z}^{h'}$ と同型であることがわかります。

#### 系 4 {#ac-vi-s10-thm-1-cor-4 .statement tag=04YI}

*v が不適切であるとします (この場合、$k = K$)。それから*
$$
h(\Gamma') + d(k'/K) \leq r(\Gamma') + D(k'/K) \leq d(K'/K).
$$
*特に v' の高さが 1 の場合、*
$$
d(k'/K) \leq d(K'/K) - 1;
$$
*さらに、$K'$が$K$の有限生成された拡大で、(12)に等式がある場合、$v'$は離散評価であり、$k'$は$K$の有限生成された拡大です。

系1、2、3の特殊な場合の系列です。

### 練習問題 {#ac-vi-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
