---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 5
section_title: Formal calculations in Lie groups
lang: ja
source: lie-i-iii
book_pages: 297-304, 382-383
pdf_pages: 0315-0322, 0400-0401
extraction: ocr
subsections:
    - "no": 1
      title: THE COEFFICIENTS $c_{\alpha \beta \gamma}$
      page: 297
      pdf_page: 315
    - "no": 2
      title: BRACKET IN THE LIE ALGEBRA
      page: 298
      pdf_page: 316
    - "no": 3
      title: POWERS
      page: 300
      pdf_page: 318
    - "no": 4
      title: EXPONENTIAL
      page: 303
      pdf_page: 321
statements: 5
exercises: 2
content_sha256: 60008f5cab4a27b0874c151743225dded6f3542426d340cb5b27298365960dcc
translated_from: content/en/lie/III/05_s5_formal_calculations_in_lie_groups.md
translation_method: google
source_content_sha256: 11ac709b8f3f88dc9c56e0725f4895fcc0f9592e0b472ff993cd89dad5d027d2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: fe2f32b897eb2ceaa7e456e6fbf838cd1b84158db67e4def0371689c628abccf
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。 リー群での正式な計算

$f, g$ を、同じ不確定項の $K$ に係数を含む 2 つの形式的な冪系列とします。$f_i$ (それぞれ $g_i$) を、$f$ (それぞれ $g$) の同次成分とします。 次数 $i$ の。書きましょう
$$
f \equiv g \mod \deg p
$$
$f_i = g_i$ の場合は $i < p$ です。

この§では、G は有限次元 $n$ のリー群胚芽を表します。 基礎体 $K$ は標数0 であると仮定されます。チャートを使って、同一視するを、G の $e$ のオープン近傍と、$K^n$ の 0 のオープン近傍 U を決定します。そのため、$e$ は 0 で識別されます。U の $x, y$ と $n \in \mathbf{Z}$ の場合、$x.y$ は次のことを示します$x$ と $y$ および $x^{[m]}$ の積 G の $x$ の m 番目の冪 (定義されている場合)。 $x \in U$の座標は$x_1, x_2, \ldots, x_n$で表されます。

### 1. ザ係数 $c_{\alpha \beta \gamma}$

$\Omega$ を $(x, y) \in U \times U$ の集合として、$x.y$ が定義され、属するが U になるようにします。 このとき、$\Omega$ は $U \times U$ で開かれており、$\Omega$ の U へのマッピング $(x, y) \mapsto x.y$ は解析的です。 したがって、$z = x.y$ の座標 $z_1, \ldots, z_n$ は、$x_1, \ldots, x_n, y_1, \ldots, y_n$ の冪の原点を中心とした積分系列としての展開を認めます。 したがって、明確に定義された定数 $c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} \in K$ が存在します。
$$
z_1^{\gamma_1} \cdots z_n^{\gamma_n} = \sum_{\alpha_1, \ldots, \beta_n \in \mathbf{N}} c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} x_1^{\alpha_1} \cdots x_n^{\alpha_n} y_1^{\beta_1} \cdots y_n^{\beta_n}
$$
$\mathbf{N}$の$\gamma_1, \ldots, \gamma_n$用。 Differentiable と Analytic 多様体, R の規則を採用して、これらの式をより簡潔に書きます。
$$
(x.y)^{\gamma} = \sum_{\alpha, \beta \in \mathbf{N}^n} c_{\alpha, \beta, \gamma} x^{\alpha} y^{\beta} \quad (\gamma \in \mathbf{N}^n).
$$
$x.0 = 0.x = x$ から $x \in U$ まで、
$$
c_{\alpha, 0, \gamma} = c_{0, \alpha, \gamma} = \delta_{\alpha \gamma}
$$
ここで、$\delta_{\alpha \gamma}$ はクロネッカー 添字です。 特に、$k = 1, \ldots, n$ を $\varepsilon_k$ の代わりに $k$ と書くと、
$$
(x.y)_k = x_k + y_k + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha, \beta, k} x^{\alpha} y^{\beta}.
$$
$c_{\alpha \beta} = (c_{\alpha \beta 1}, c_{\alpha \beta 2}, \ldots, c_{\alpha \beta n}) \in K^n$と書くと、次のようになります。
$$
x.y = x + y + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$

(5) の右側では、次数 2 の同次成分を考慮します。

$$
B(x, y) = \sum_{i,j=1}^n c_{ij} x_i y_j
$$

したがって、$(x, y) \mapsto B(x, y)$ は $K^n \times K^n$ から $K^n$ への双線形写像になります。それから

(6)
$$
x.y \equiv x + y + B(x, y) \mod \deg 3.
$$

公式 (4) は、一方で、次のことを意味します。

(7)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| < |\gamma|
$$

そして、$z^\gamma$ の展開における合計次数 $|\gamma|$ のうちの項は、$(x_1 + y_1)^{\gamma_1}(x_2 + y_2)^{\gamma_2} \ldots (x_n + y_n)^{\gamma_n} = \sum_{\alpha + \beta = \gamma} ((\alpha, \beta)) x^\alpha y^\beta$ (cf. *微分可能および解析的多様体*、R、記法および規約) のものでもあります。したがって、次のようになります。

(8)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| = |\gamma| \quad \text{but } \alpha + \beta \neq \gamma
$$
(9)
$$
c_{\alpha, \beta, \alpha + \beta} = ((\alpha, \beta)).
$$

積の結合性は関係を意味します
$$
\sum_{\xi} c_{\alpha \xi n} x^\alpha \left( \sum_{\beta, \gamma} c_{\beta \gamma \xi} y^\beta z^\gamma \right) = \sum_{\xi, \gamma} c_{\xi \gamma n} \left( \sum_{\alpha, \beta} c_{\alpha \beta \xi} x^\alpha y^\beta \right) z^\gamma
$$
すべての $x, y, z$ が 0 に十分近い、よって

(10)
$$
\sum_{\xi} c_{\alpha \xi n} c_{\beta \gamma \xi} = \sum_{\xi} c_{\xi \gamma n} c_{\alpha \beta \xi} \quad (\alpha, \beta, \gamma, \eta \text{ in } \mathbf{N}^n).
$$

群ジャーム G は、$\mathbf{N}^n$ のすべての $\alpha, \beta, \gamma$ に対して $c_{\alpha \beta \gamma} = c_{\beta \alpha \gamma}$ である場合に限り、可換開部分群ジャームを認めます。

### 2. ブラケットインリー代数

$\alpha \in \mathbf{N}^n$の場合、$e_\alpha$を原点の点分布$\frac{1}{\alpha!} \frac{\partial^\alpha}{\partial x^\alpha}$とします。特に、
$$
e_k = e_{e_k} = \frac{\partial}{\partial x_k}.
$$
ベクトル空間 $U(G)$ の $e_\alpha$ 形基底。 $f$ が G の 0 の開近傍上の解析的写像であり、$f(x) = \sum \lambda_\alpha x^\alpha$ が原点に関する積分系列としてのその展開である場合、
$$
\langle e_\alpha, f \rangle = \lambda_\alpha.
$$
特に、
$$
\langle e_\alpha, x^\gamma \rangle = \delta_{\alpha \gamma}.
$$

したがって、
$$
\langle e_\alpha * e_\beta, x^\gamma \rangle = \langle e_\alpha \otimes e_\beta, (x.y)^\gamma \rangle \\
= \langle e_\alpha \otimes e_\beta, \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} x^{\alpha'} y^{\beta'} \rangle \\
= \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} \langle e_\alpha, x^{\alpha'} \rangle \langle e_\beta, y^{\beta'} \rangle = c_{\alpha\beta\gamma}
$$
したがって
$$
e_\alpha * e_\beta = \sum_\gamma c_{\alpha\beta\gamma} e_\gamma.
$$
(公式 (10) は$U(G)$ で結合性を表現します。)
特に$L(G)$はブラケット下で安定しているので。
$$
[e_i, e_j] = \sum_k (c_{ijk} - c_{jik}) e_k.
$$
したがって、基底 $(e_1, \ldots, e_n)$ に対する $L(G)$ の構造の定数は、$c_{ijk} - c_{jik}$ になります。他の語では、$L(G)$ を $K^n$ と正規的に識別すると、次のようになります。
$$
[x, y] = B(x, y) - B(y, x).
$$

#### 命題 1 {#lie-iii-s5-prop-1 .statement tag=0AE1}

(i) $$ x^{[-1]} \equiv -x + B(x, x) \mod \deg 3 $$
(ii) $$ x.y.x^{[-1]} \equiv y + [x, y] \mod \deg 3 $$
(iii) $$ y^{[-1]}.x.y \equiv x + [x, y] \mod \deg 3 $$
(iv) $$ x^{[-1]}.y^{[-1]}.x.y \equiv [x, y] \mod \deg 3 $$
(v) $$ x.y.x^{[-1]}.y^{[-1]} \equiv [x, y] \mod \deg 3. $$
((i) において、$x^{[-1]}$ はもちろん、写像 $x \mapsto x^{[-1]}$ を原点に関する積分系列として展開したものです。他の式も同様に解釈できます。)
$g_1$ と $g_2$ を次数 1 と 2 の $x^{[-1]}$ の同次成分とします。
$$
0 = x.x^{[-1]} \\
\equiv x + g_1(x) + B(x, g_1(x)) \mod \deg 2 \quad \text{(by (6))} \\
\equiv x + g_1(x) \mod \deg 2
$$
したがって $g_1(x) = -x$ です。それから
$$
0 = x.x^{[-1]} \\
\equiv x + (-x + g_2(x)) + B(x, -x + g_2(x)) \mod \deg 3 \\
\equiv g_2(x) - B(x, x) \mod \deg 3
$$

したがって $g_2(x) = B(x, x)$ です。これは(i)を証明します。次に、(i) を使用して、
$$
x.y.x^{[-1]} \equiv (x + y + B(x, y)).(-x + B(x, x)) \quad \text{mod deg 3}
$$
$$
\equiv x + y + B(x, y) + (-x + B(x, x)) + B(x + y, -x) \quad \text{mod deg 3}
$$
$$
\equiv y + B(x, y) - B(y, x) \quad \text{mod deg 3}
$$
$$
\equiv y + [x, y] \quad \text{mod deg 3 (by (13))}
$$
よって (ii)。 (iii) の証明も同様です。 (i) と (iii) を組み合わせると、次のようになります。
$$
x^{[-1]},y^{[-1]}.x.y \equiv (-x + B(x, x)).(x + [x, y]) \quad \text{mod deg 3}
$$
$$
\equiv -x + B(x, x) + x + [x, y] + B(-x, x) \quad \text{mod deg 3}
$$
$$
\equiv [x, y] \quad \text{mod deg 3}
$$
よって (iv)。 (v) の証明も同様です。

### 3. 冪

G の j 点を考えてみましょう。
$$
x(1) = (x(1)_1, x(1)_2, \ldots, x(1)_n)
$$
$$
x(2) = (x(2)_1, x(2)_2, \ldots, x(2)_n)
$$
$$
\ldots \ldots \ldots \ldots \ldots \ldots \ldots
$$
$$
x(j) = (x(j)_1, x(j)_2, \ldots, x(j)_n).
$$
写像 $(x(1), x(2), \ldots, x(j)) \mapsto x(1).x(2)\ldots x(j)$ は、原点に関する積分系列として展開を認めます。

$$
x(1).x(2)\ldots x(j) = \sum_{\alpha(1), \alpha(2), \ldots, \alpha(j) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(j)} x(1)^{\alpha(1)} \ldots x(j)^{\alpha(j)}
$$

ここで、$a_{\alpha(1), \ldots, \alpha(j)}$ は $\mathbf{K}^n$ の元です。 $j = 0, 1, 2, \ldots$ については、次のように書きます。

$$
\psi_j(x) = \sum_{\alpha(1) \neq 0, \ldots, \alpha(j) \neq 0} a_{\alpha(1), \ldots, \alpha(j)} x^{\alpha(1) + \ldots + \alpha(j)}
$$

ここで、右辺は変数 $x \in \mathbf{K}^n$ の収束積分系列です。この系列は、(14) 項で変数 $x(1), \ldots, x(j)$ の 1 つが明示的に出現しないことを抑制して、$x(1) = x(2) = \cdots = x(j) = x$ を記述することによって得られます。

$t \in \mathbf{K}$ の場合、G のすべての t 番目の冪写像は、0 の近傍上の任意の 2 つ一致するであるため、原点に関する積分系列と同じ展開を持ちます。この展開を $x^{[t]}$ による積分系列として表します。

#### 命題 2 {#lie-iii-s5-prop-2 .statement tag=0AE2}

(i) $\psi_j \equiv 0 \mod \deg j$。
(ii) *$t \in \mathbf{K}$ の場合、*
$$
x^{[t]} = \sum_{i=1}^8 \binom{t}{i} \psi_i(x)
$$
*ここで、右側の正式な冪系列は (i) により意味を持ちます。*

(私たちは書きます

$$
\binom{t}{i} = \frac{t(t-1)\ldots(t-i+1)}{i!}
$$

みんな$t \in \mathbf{K}$のために。)

主張 (i) は、$\psi_j$ の定義から明らかです。

$t$ 整数 $\geq 0$ について (ii) を証明します。 (14)により、

$$
x^{[t]} = \sum_{\alpha(1), \ldots, \alpha(t) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

$\alpha = (\alpha(1), \ldots, \alpha(t)) \in (\mathbf{N}^n)^t$ について、$\sigma(\alpha)$ は $j \in \{1, 2, \ldots, t\}$ の集合を表し、$\alpha(j) \neq 0$ となるようにします。 和 (17) で、群項が一緒で、$\sigma(\alpha)$ が同じである場合、

$$
x^{[t]} = \sum_{\sigma \subset \{1, t\}} h_{t, \sigma}(x)
$$

どこで

$$
h_{t, \sigma}(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

$\sigma = \{j_1, j_2, \ldots, j_q\}$を$j_1 < j_2 < \ldots < j_q$にしましょう。 (14) ($j$ が $t$ に置き換えられる) では、$k \notin \sigma$ の $x(k)$ を 0 に置き換えます。 0 は $G$ の単位元であるため、原点に関する積分系列として $x(j_1) \cdot x(j_2) \ldots x(j_q)$ の展開が得られます。

$$
x(j_1) \cdot x(j_2) \ldots x(j_q) = \sum_{\sigma(\alpha) \subset \sigma} a_{\alpha(1), \ldots, \alpha(t)} x(j_1)^{\alpha(j_1)} x(j_2)^{\alpha(j_2)} \ldots x(j_q)^{\alpha(j_q)}
$$

したがって、$\psi_q$の定義までに:

$$
\psi_q(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(j_1) + \ldots + \alpha(j_q)}.
$$

(19) と (20) から、$h_{t, \sigma}(x) = \psi_{\mathrm{card}\,\sigma}(x)$ であることがわかります。すると (18) は次のことを意味します

$$
x^{[t]} = \sum_{i=0}^t \binom{t}{i} \psi_i(x) = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x).
$$

次に、すべての $t \in \mathbf{K}$ に対して $x^{[t]'} = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x)$ と書きます。積分系列 $x^{[t]}$ と $x^{[t]'}$ では、それぞれの係数は $t$ の多項式関数です。というのは、$x^{[t]'}$ にとってこれは明らかだからです。 $x^{[t]}$ に関する限り、すべての $u \in \mathrm{U}(G)$ について、$x \mapsto x^{[t]}$ の下の $u$ の像が $t$ の多項式関数であることを証明すれば十分です。さて、$u \in \mathrm{U}^m(G)$の場合、この像は$t^m u$ (§ 4, no. 3, 命題 7 (iv)) です。

$t$ 整数 $\geq 0$ に対して $x^{[t]} = x^{[t]'}$ とすると、すべての $t \in \mathbf{K}$ に対して $x^{[t]} = x^{[t]'}$ が続きます。

#### 注意 {#lie-iii-s5-n3-rem-1 .statement tag=0AE3}

(1) t 整数 $\geqslant 0$ に対して命題 2 の条件 (ii) を書きます。

$$
\begin{align*}
0 &= \psi_0(x) \\
x &= \psi_0(x) + \psi_1(x) \\
x^{[2]} &= \psi_0(x) + 2\psi_1(x) + \psi_2(x) \\
&\ldots \ldots \ldots \ldots \ldots \ldots \ldots
\end{align*}
$$

これらの式は、決定するを $\psi_i$ にするには十分です。

(2) $\psi_0(x) = 0, \psi_1(x) = x, \psi_2(x) = x^{[2]} - 2x$、

$$
x^{[-1]} = \sum_{i=1}^\infty (-1)^i \psi_i(x).
$$

(3) 上記の$\psi_2$ と公式の式 (6) は、次のことを証明します。

$$
\psi_2(x) \equiv \mathrm{B}(x, x) \mod \deg 3.
$$
命題 2、(i) および (ii) を使用すると、次のことがわかります。

$$
x^{[t]} \equiv tx + \binom{t}{2} \mathrm{B}(x, x) \mod \deg 3.
$$

(4) $\psi_{p,m}(x)$ と $h_{t,m}(x)$ が $\psi_p(x)$ の同次成分と次数 m の $x^{[t]}$ を表すものとします。次に、$m < p$の場合は$\psi_{p,m} = 0$です。一方、命題 2 (ii) は次のようになります。

$$
h_{t,m}(x) = \sum_{p \leq m} \frac{t(t-1)\ldots(t-p+1)}{p!} \psi_{p,m}(x)
$$
つまり

$$
h_{t,m}(x) = \sum_{1 \leq r \leq m} t^r \phi_{r,m}(x)
$$
ここで、$\phi_{r,m}$は、$\mathbf{K}^n$の次数mの$\mathbf{K}^n$の同次多項式写像です。特に、(23) により、

$$
\phi_{1,m}(x) = \sum_{p \leq m} \frac{(-1)^{p-1}}{p} \psi_{p,m}(x)
$$
$$
\phi_{m,m}(x) = \frac{1}{m!} \psi_{m,m}(x).
$$

(5) $\mathbf{K}$ が特性 $> 0$ の場合、nos の結果は次のようになります。 no. 2 の $e_\alpha$ が $\langle e_\alpha, \sum_\beta \lambda_\beta x^\beta \rangle = \lambda_\alpha$ で定義されている限り、1 と 2 は真のままです。 no. 3 では、$\psi_j$ が上記のように定義されている場合、議論は再び $t \in \mathbf{N}$ であれば $x^{[t]} = \sum_{i=1}^\infty \binom{t}{i} \psi_i(x)$ であることを証明します。

### 4. 指数関数的

$E(x)$ を、$G$ の指数写像を 0 の積分系列として展開したものとします。 $L(x)$ を、$G$ の単射指数写像の逆数写像を積分系列として展開したものとします。 0. 任意の指数写像に対する 0 での接線写像は、$L(G)$、$E(x) \equiv x \mod \deg 2$、$L(x) \equiv x \mod \deg 2$ の恒等式です。 $x$ に対する $E(L(x)) = L(E(x))$ は 0 に十分近いため、形式的な冪系列 $E$ と $L$ は $E(L(X)) = L(E(X)) = X$ となります。同様の議論は次のことを示しています
$$
E(tX) = (E(X))^{[t]}, \quad L(X^{[t]}) = tL(X)
$$
$t \in K$の場合。

#### 命題 3 {#lie-iii-s5-prop-3 .statement tag=0AE4}

(27)
$$
L = \sum_{p=1}^{\infty} \frac{(-1)^{p-1}}{p} \psi_p
$$
(28)
$$
E = \sum_{p=1}^{\infty} \frac{1}{p!} \psi_{p,p}
$$
($\psi_{p,p}$ は次数 $p$ の $\psi_p$ の同次成分であることを思い出してください。)

または、(24) により、
$$
E(tx) = (E(x))^{[t]}
$$

$t$と$x$は両面が正式な冪系列です。 $t$ の最初の次数の項を等しくすると、次のようになります。
$$
x = \sum_{m \geq 0} \phi_{1,m}(E(x)).
$$
ここで、正式な冪系列の系の反転は、可能な場合には、一方向でのみ可能です (代数、章 IV, § 6、系から命題 8)。それから
$$
L(x) = \sum_{m \geq 0} \phi_{1,m}(x) \quad \text{by (29)}
$$
$$
= \sum_{p,m} \frac{(-1)^p}{p} \psi_{p,m}(x) \quad \text{by (25)}
$$
$$
= \sum_p \frac{(-1)^p}{p} \psi_p(x),
$$
よって (i)。同様に、$t \neq 0$ については、
$$
L(tx) = tL((tx)^{[t^{-1}]})
$$
$$
= tL\left( \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^{m-r} \phi_{r,m}(x) \right) \quad \text{by (24)}.
$$

t の最初の次数の項を等しくすると、次のようになります。

$$
x = L \left( \sum_{m \geq 0} \phi_{m,m}(x) \right)
$$

よって

$$
E(x) = \sum_{m \geq 0} \phi_{m,m}(x)
$$
$$
= \sum_{m \geq 0} \frac{1}{m!} \psi_{m,m}(x) \quad \text{by (26).}
$$

#### 命題 4 {#lie-iii-s5-prop-4 .statement tag=0AE5}

*G のチャートが正規であった場合、$j \geq 2$ に対して $\psi_j = 0$ であることが必要十分です。*

これは、命題 3 までに十分です。チャートが正規であり、$2 \leq i < n$ に対して $\psi_i = 0$ であると仮定します。次に、$nx = x^{[n]} = \sum_{i=0}^n \binom{n}{i} \psi_i(x) = nx + \psi_n(x)$、よって、$\psi_n = 0$となります。したがって、$j$の帰納法による$j \geq 2$の$\psi_j = 0$。

### 練習問題 {#lie-iii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
