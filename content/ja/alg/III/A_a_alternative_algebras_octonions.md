---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: Alternative algebras. Octonions
appendix: true
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 611-617, 654
pdf_pages: 0635-0641, 0678-0678
extraction: ocr
subsections:
    - "no": 1
      title: ALTERNATIVE ALGEBRAS
      page: 611
      pdf_page: 635
    - "no": 2
      title: ALTERNATIVE CAYLEY ALGEBRAS
      page: 613
      pdf_page: 637
    - "no": 3
      title: OCTONIONS
      page: 615
      pdf_page: 639
statements: 11
exercises: 3
content_sha256: cbf2cdd868dd3cdb3a47271372f08d5296fb2a5b8ec426108624915c2c11fb71
translated_from: content/en/alg/III/A_a_alternative_algebras_octonions.md
translation_method: google
source_content_sha256: ae041bbfaebb6710b823bdc0661c24a1124357966f753025f28bd48ab4086bed
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 56687a2d32eb179f8483e849fde945b5ced7678073b5d92e645cc7001aebd677
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 付録

# 代替案代数。八角数

### 1. 代替案代数

A を可換環 、F を (必ずしも結合的ではない) A-代数とします。 F の任意の 3 つの元 $x, y, z$ について、次のように書きます。

$$
a(x, y, z) = x(yz) - (xy)z
$$

($x, y, z$のアソシエイター); $a$ は明らかに、$F \times F \times F$ から $F$ への A-trilinear 写像です。

#### 補題 1 {#alg-iii-a0-lem-1 .statement tag=069A}

*代数 $F$ のすべての $p, q, r, s$、*

$$
a(pq, r, s) - a(p, qr, s) + a(p, q, rs) = a(p, q, r)s + pa(q, r, s).
$$

検証は定義 (1) からすぐに続きます。

#### 命題 1 {#alg-iii-a0-prop-1 .statement tag=069B}

*A-代数 $F$ の場合、次の条件は同等です:*
(a) *順序付けられた対、元、$x, y$、$F$ ごとに、$x$ と $y$ によって生成された部分代数は結合します。
(b) *三線形写像 $(x, y, z) \mapsto a(x, y, z)$ は交代的 (§ 7, no. 3) です。*
(c) *注文した対、元、$x, y$、$F$、$x^2y = x(xy)$、$yx^2 = (yx)x$ごとに。*

明らかに (a) は (c) を意味します。 (c) が (b) を含意していることを示します。(b) を証明するには、定義 (§ 7, no. 3) によって、$a(x, x, y) = 0$ と $a(x, y, y) = 0$ が正確に (c) であることを検証するだけで十分です。

(b) が (a) を意味することを証明するには、次の 4 補題を使用します。

#### 補題 2 {#alg-iii-a0-lem-2 .statement tag=069C}

*$E$ を A-代数として、トライリニア写像 $(x, y, z) \mapsto a(x, y, z)$ が交代的、$S$ 生成する系の$E$ および$U$ が$E$ のサブ A モジュールであるとします。 含む $S$ など、すべての $s \in S$ に対して $sU \subset U$ と $Us \subset U$ が続きます。それから$U = E$.*

The set $U'$ of $x \in E$ such that $xU \subset U$ and $Ux \subset U$ is obviously a sub-A-module of $E$, which contains $S$ by hypothesis. 一方、$U'$と$u \in U$の$x, y$については、仮定により

$$
(xy)u = x(yu) + a(x, y, u) = x(yu) - a(x, u, y) = x(yu) - (xu)y + x(uy) \in U;
$$

移行から反対多元環も同様に $u(xy) \in U$ になります。したがって、$U'$ は $E$ の部分代数であり、含む $S$ であるため、$U' = E$ です。したがって、$EU \subset U$ と *なおさら* $UU \subset U$ は、$U$ が $E$ の部分代数であることを証明します。 含む $S$、$U = E$ となり、補題が証明されます。

$F$ の部分集合 $H$ は、元 $u, v, w$ 属するから $H$ の *少なくとも 2 つ* の場合、$a(u, v, w) = 0$ は *強結合* と呼ばれます。

#### 補題 3 {#alg-iii-a0-lem-3 .statement tag=069D}

※写像 $a$ が交代的であるとします。 $H$ が $F$ の部分集合の強結合である場合、$H$ によって生成された $F$ の部分代数は強結合です。*

$F$ の強結合性部分集合の集合は帰納的であるため、$H$ が $F$ の *最大* 強結合性部分集合である場合、$H$ は $F$ の *部分代数* であることを証明するだけで十分です。 $H$ は明らかに $F$ のサブ A モジュールであるため、$H$ の任意の 2 つの元 $u, v$ に対して、$H \cup \{uv\}$ も強い結合であることを検証するだけで十分です。なぜなら、$H$ の定義により、これは $uv \in H$ を意味するからです。 さて、すべての $z \in H$ とすべての $t \in F$ について、(2) によって

$$
a(uv, t, z) - a(u, vt, z) + a(u, v, tz) = 0
$$

$\mathbf{H}$ は結合性が強いため。 $u, v, z$ は $\mathbf{H}$ にもあるので、
$$
a(u, vt, z) = a(u, v, tz) = 0,
$$
よって $a(uv, t, z) = 0$。 $a$ が交代的であるという事実を使用すると、元 $p, q, r$ 属する ～ $\mathbf{H} \cup \{uv\}$ よって補題の少なくとも 2 つが満たされるたびに、$a(p, q, r) = 0$ になることがわかります。

#### 補題 4 {#alg-iii-a0-lem-4 .statement tag=069E}

※写像 $a$ が交代的であるとします。次に、すべての $x \in \mathbf{F}$ に対して、$x$ によって生成された $\mathbf{F}$ の部分代数は強く結合します。*

$a(u, v, w) = 0$ 3 つの元 $u, v, w$ のうち 2 つが $x$ に等しい場合、補題 3 を適用するだけで十分です。

#### 補題 5 {#alg-iii-a0-lem-5 .statement tag=069F}

*写像 $a$ が交代的であると仮定し、$\mathbf{X}, \mathbf{Y}$ を$\mathbf{F}$ の 2 つの強く結合する部分代数とします。すると、$\mathbf{X} \cup \mathbf{Y}$ によって生成された $\mathbf{E}$ の部分代数が結合します。*

$Z$ を $z \in \mathbf{E}$ の集合として、すべての $u \in \mathbf{X}$ と $v \in \mathbf{Y}$ に対して $a(u, v, z) = 0$ となるようにします。$\mathbf{X}$ と $\mathbf{Y}$ が強いので、これは明らかにサブ A モジュール含む $\mathbf{X}$ と $\mathbf{Y}$ です。連想的; 補題 2 により、$u \in \mathbf{X}$ と $v \in \mathbf{Y}$、$uZ \subset Z, vZ \subset Z, Zu \subset Z$ と $Zv \subset Z$ について検証するだけで十分です。さて、$\mathbf{X}$、$v \in \mathbf{Y}$、$z \in Z$の$u, u'$については、(2)によります。
$$
a(u'u, z, v) - a(u', uz, v) + a(u', u, zv) = a(u', u, z)v + u'a(u, z, v) = 0
$$
$\mathbf{X}$ と $Z$ の定義は強く結合しているという事実によって。しかし、$\mathbf{X}$ は結合性が強いので、$a(u', u, zv) = 0$ と $u'u \in \mathbf{X}$ から、$Z$ の定義によって $a(u'u, z, v) = 0$ になります。したがって、$a(u', uz, v) = 0$ は、$uZ \subset Z$ を示します。 適用 (2) を $(p, q, r, s) = (v, z, u, u')$ とすると、同様に $Zu \subset Z$ が得られます。 $\mathbf{X}$と$\mathbf{Y}$の役割を交換することし、$a$が交代的であるという事実を使用すると、$vZ \subset Z$と$Zv \subset Z$が得られます。 よって補題。

ここで、(b) が命題 1 の (a) を暗黙的に示すことを証明するには、補題 4 を使用して $\mathbf{X} = \{x\}$ と $\mathbf{Y} = \{y\}$ を取るだけで十分です。

#### 定義 1 {#alg-iii-a0-def-1 .statement tag=069G}

*代数 $\mathbf{F}$ は、命題 1 の同等の条件を満たす場合、代替と呼ばれます。*

関連する代数は明らかに代替手段です。 no. 3 では、結合性のない代替案代数の例を与えます。

$\mathbf{F}$ が代替 A-代数である場合、命題 1 の条件 (b) からわかるように、スカラー (§ 1, no. 5) を拡張して $\mathbf{F}$ から得られるすべての A-代数 $\mathbf{F} \otimes_A A'$ は代替 $A'$-代数です。

### 2. 別のケイリー 代数

#### 命題 2 {#alg-iii-a0-prop-2 .statement tag=069H}

*$\mathbf{A}$を環、$\mathbf{F}$をケイリー$\mathbf{A}$代数、その単位元、$s : x \mapsto \overline{x}$その共役、$\mathbf{N} : \mathbf{F} \to \mathbf{A}$をケイリーノルム(§ 3, no. 4)とする。

(i) $\mathbf{F}$ が代替であるためには、元の対 $\mathbf{F}$ の$x, y$ が注文されるたびに、$x^2y = x(xy)$ であることが必要かつ十分です。*

(ii) *F が代替の場合、F のすべての x、y に対して N(xy) = N(x)N(y) となります。*
(iii) ※F を代替とする。 元 x ∈ F が可逆であるためには、N(x) が Ae で可逆であることが必要かつ十分です。 x の逆数は一意であり、N(x)^{-1}\overline{x} と等しくなります。これを x^{-1},* で表します
$$
x^{-1}(xy) = x(x^{-1}y) = y
$$
*またはすべての y ∈ F.*

F が代替となるためには、条件 $x^2y = x(xy)$ が明らかに必要です (no. 1、命題 1)。逆に、F の元のすべての注文された対、適用が $\overline{x}$ および $\overline{y}$ に当てはまる場合、$\overline{x}^2\overline{y} = \overline{x}(\overline{xy})$ が得られます。この関係に対する適用の活用により、$yx^2 = (yx)x$ が得られ、命題 1 of no. 1 の条件 (c) が満たされます。

明らかに、F のすべての $x, y$ に対して $a(e, x, y) = 0$ です。F が代替である場合、したがって、命題 1 (no. 1) から、e、x、y によって生成される F の部分代数 G は結合的であると推定されます。 $\overline{x} = -x + T(x) \in -x + Ae, \overline{x} \in G$ と同様に $\overline{y} \in G$ となります。次に、$N(y) \in Ae$という事実を利用して、$N(xy) = (xy)(\overline{xy}) = xy.\overline{y}.\overline{x} = N(y)x\overline{x} = N(y)N(x)$。これは(ii)を証明します。

最後に(iii)を証明します。 $N(x)$ が Ae で可逆であり、$x' = N(x)^{-1}\overline{x}$ と書くと、$N(x) = x\overline{x} = \overline{x}x$ に対して $xx' = x'x = e$ となります。逆に、x が左逆 $x''$ を認める場合、(ii) により $N(x'')N(x) = N(e) = e$ となり、Ae では $N(x)$ が可逆になります。さらに、$x' = N(x)^{-1}\overline{x}$ は x と e によって生成された部分代数にあるため、x、$x''$、および e によって生成された連想部分代数に対して元 $x, x', x''$ 属するとなり、したがって $x'' = x''(xx') = (x''x)x' = x'$、よって一意性主張。式 $x^{-1}(xy) = x(x^{-1}y) = y$ は、$x^{-1}, x$ と y が x、y および e によって生成された部分代数の元であり、結合的であるという事実から導き出されます。

#### 命題 3 {#alg-iii-a0-prop-3 .statement tag=069I}

*E を A の Cayley A-代数、γ 元、F を γ と E の共役 (§ 2, no. 5, 命題 5) によって定義される E の Cayley 拡大とする。 F が代替的であるためには、E が結合的であることが必要かつ十分です。*

$u = (x, y), v = (x', y')$ を F の 2 つの元とします (x、y、$x', y'$ は E にあります)。それから (§ 2, no. 5, 公式 (27))

$$
\begin{cases}
u^2v = ((x^2 + \gamma \overline{y}y)x' + \gamma \overline{y}'(y\overline{x} + yx), (y\overline{x} + yx)\overline{x}' + y'(x^2 + \gamma \overline{y}y)) \\
u(uv) = (x(xx' + \gamma \overline{y}'y) + \gamma (x'\overline{y} + \overline{x}.\overline{y}')y, y(\overline{x}'\overline{x} + \gamma \overline{y}y') + (y\overline{x}' + y'x)x).
\end{cases}
$$

$\overline{y}y$ と $\overline{x} + x$ が Ae にあるという事実を使用して、これらの式を調べると、E の結合性は $u^2v = u(uv)$ を意味し、したがって F が代替であるという事実 (命題 2) が示されます。逆に、F が代替の場合、$y' = 0$ が次の場合に方程式 $u^2v = u(uv)$ が適用されます。
$$
(y\overline{x} + yx)\overline{x}' = y(\overline{x}'\overline{x}) + (y\overline{x}')x.
$$
これで、左辺は $(yT(x))\overline{x}' = y(\overline{x}'T(x)) = y(\overline{x}'x + \overline{x}'\overline{x});$ に等しくなります

右辺と比較すると、$x, y$ と $\bar{x}'$ は E の任意の元であるため、E の結合性を証明する $(y \bar{x}') x = y (\bar{x}' x)$ が得られます。

### 3. 八角数

E を A 上の型 $(\alpha, \beta, \gamma)$ の四元数代数とし ($§ 2$、no. 5、例 2)、$\delta \in A$ とします。 $\delta$ による E の Cayley 拡大 F と E の共役は、A 上の八元数代数と呼ばれ、型 $(\alpha, \beta, \gamma, \delta)$ であると言われます。 no. 2 の命題 3 により、F は代替代数になります。 8 元のうち基底 $(e_i)_{0 \leq i \leq 7}$ があり、次のように定義されています。
$$
\begin{align*}
e_0 &= (e, 0), & e_1 &= (i, 0), & e_2 &= (j, 0), & e_3 &= (k, 0) \\
e_4 &= (0, e), & e_5 &= (0, i), & e_6 &= (0, j), & e_7 &= (0, k)
\end{align*}
$$
ここで、$(e, i, j, k)$ は E 定義された loc の基底です。引用;明らかに $e_0$ ($e$ とも表される) は F の単位元です。 $u = \sum_{i=0}^{7} \xi_i e_i$ が F の元である場合 ($\xi_i \in A$ を使用)、$§ 2$、no. 5 の式 (23)、(24)、(31) は次のようになります。 共役、八角形$u$のトレースとノルム

$$
\left\{
\begin{aligned}
\bar{u} &= (\xi_0 + \beta \xi_1) e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 + \beta \xi_1 \\
N_F(u) &= \xi_0^2 + \beta \xi_0 \xi_1 - \alpha \xi_1^2 - \gamma (\xi_2^2 + \beta \xi_2 \xi_3 - \alpha \xi_3^2) \\
&\quad - \delta (\xi_4^2 + \beta \xi_4 \xi_5 - \alpha \xi_5^2) + \gamma \delta (\xi_6^2 + \beta \xi_6 \xi_7 - \alpha \xi_7^2).
\end{aligned}
\right.
$$

ここで、$u = (x, y)$、$u' = (x', y')$、$u'' = (x'', y'')$ を 3 つの八元数とします (元 $x, x', x'', y, y', y''$ 属するから E)。 $§ 2$、no. 5 の式 (24) と (27) は次のようになります。
$$
\begin{align*}
T_F((uu')u'') &= T(xx'x'') + \delta T(\bar{y}'y x'') + \delta T(\bar{y}''y \bar{x}') + \delta T(\bar{y}''y' x) \\
T_F(u(u'u'')) &= T(xx'x'') + \delta T(x''\bar{y}'y) + \delta T(\bar{x}'\bar{y}''y) + \delta T(x\bar{y}''y')
\end{align*}
$$
(ここで、T は E のトレースを示し、E が結合するという事実が利用されます)。すべての四元数 $x, y$ ($§ 2$, no. 4, 公式 (17)) に対する $T(xy) = T(yx)$ として、次のようになります。
$$
T_F((uu')u'') = T_F(u(u'u''))
$$
特に型 $(-1, 0, -1, -1)$ の八元数を研究します。式 (4) は次のように単純化されます。
$$
\left\{
\begin{aligned}
\bar{u} &= \xi_0 e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 \\
N_F(u) &= \sum_{i=0}^{7} \xi_i^2.
\end{aligned}
\right.
$$

*$\mathbf{A}$ を実数の体 $\mathbf{R}$ とすると、$\mathbf{R}$ 上の型 $(-1, 0, -1, -1)$ の八元数は *Cayley octonions* (または *octaves*) と呼ばれます。 no. 2 の命題 2 (ii) から、すべての Cayley 八元数 $\neq 0$ は *反転可能** であることがわかります。

#### 命題 4 {#alg-iii-a0-prop-4 .statement tag=069J}

*$F$ を $\mathbf{A}$ 上の型 $(-1, 0, -1, -1)$ の 8 倍数代数とします。 There exists a vector space $V$ of dimension 3 over the field with two elements $\mathbf{Z}/2\mathbf{Z}$ and a bijection $\lambda \mapsto e'_\lambda$ of $V$ onto the basis $(e_i)_{0 \leq i \leq 7}$ such that*
$$
e'_0 = e_0, \qquad e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}
$$
*for all $\lambda, \mu$ in $V$. 位数の $e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e_\mu) e'_\nu$ では、$V$ において、$\lambda, \mu, \nu$ が $\mathbf{Z}/2\mathbf{Z}$ に対して線形依存するだけで十分です。 $\mathbf{A}$ で $2 \neq 0$ の場合、この条件が必要です。*

この番号の先頭に記法を保存します。 § 2, no. 5 の式 (33) から、元 $\pm e_0, \pm e_1, \pm e_2, \pm e_3$ の集合 $S$ からなるは乗法で安定であることがわかります。また、$E$の$x, y, y'$については、§ 2, no. 5の公式(22)により、
$$
(x, 0)(0, y') = (0, y'x), \quad (0, y')(x, 0) = (0, y'\overline{x}), \quad (0, y)(0, y') = (-\overline{y}'y, 0)
$$
したがって、元 $\pm e_i$ ($0 \leq i \leq 7$) の集合 $T$ からなるは乗法で安定します。さらに、その乗法表は環 $\mathbf{A}$ から*独立*しています。

特に、$\mathbf{A}''$ を 2 つの元を含む体 $\mathbf{Z}/2\mathbf{Z}$ とし、$E''$ を $\mathbf{A}''$ と $F''$ 代数上の型 $(1, 0, 1)$ の四元数代数とします。 型 $(1, 0, 1, 1)$ $\mathbf{A}''$ を超えます。 $(e''_i)_{0 \leq i \leq 7}$ を上記のように形成された $F''$ の基底とします。 $-e''_i = e''_i$ 以降、$e''_i$ の集合 $T''$ は 8 元を持ち、乗法以下で安定します。さらに、上記からすぐに写像 $\theta : T \to T''$ が得られ、$0 \leq i \leq 7$ の $\theta(e_i) = \theta(-e_i) = e''_i$ は乗法の準同型になります。 さらに、この場合、四元数代数 $E''$ は可換であるため、$F''$ は結合です (§ 2, no. 5, 命題 5)。さらに、$F''$ の活用はこの場合恒等です。 したがって、$T''$ は *群* であり、式 (8) はそれが *可換*であることを示しています。これらの式と§ 2, no. 5の式(33)は、$T''$のすべての元の平方が単位元であることを示しています。 $V$ を使用して加法的に書かれた群 $T''$ を表す場合、$V$ には $\mathbf{Z}/2\mathbf{Z}$ に対して一意のベクトル空間構造を与えることができ、必然的に次元 3 になります。
$$
\operatorname{Card}(V) = 8 = 2^{\dim(V)}.
$$

すべての $\lambda \in V$ について、$e'_\lambda$ が $\theta(e'_\lambda) = \lambda$ となるように $(e_i)_{0 \leq i \leq 7}$ の元を表すものとします。次に$e'_0 = e_0$;さらに、$\theta$ は準同型であり、関係 $\theta(x) = \theta(y)$ は $x = \pm y$、$e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}$ に相当します。 $\lambda, \mu, \nu$ が $\mathbf{Z}/2\mathbf{Z}$ 上で線形独立である場合、$V$ の形基底、したがってすべての元 $e_i$ ($0 \leq i \leq 7$) は $e'_\lambda, e'_\mu$ によって生成される属するから部分代数になります。 $e'_\nu$; $\mathbf{A}$ の $2 \neq 0$ の場合、$e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e'_\mu) e'_\nu$ は不可能です。なぜなら、$F$ は結合的であり、したがって $E$ は可換 (§ 2, no. 5, 命題 5) となり、これは矛盾する関係 (33) となります。 § 2, no. 5。一方、$\lambda, \mu, \nu$ が V で線形従属である場合、3 つの元 $e'_\lambda, e'_\mu, e'_v$ 属するから部分代数は F の 2 つの生成元と結合します (no. 1, 命題 1)。 よって結論。

#### 注意 {#alg-iii-a0-n3-rem-1 .statement tag=069K}

$\lambda \neq 0$に対する$\bar{e}'_\lambda = -e'_\lambda$として、

$$
e'_\lambda{}^2 = -e_0 \quad \text{for } \lambda \neq 0,
$$
$$
e'_\mu e'_\lambda = -e'_\lambda e'_\mu \quad \text{for } \lambda \neq 0, \mu \neq 0 \text{ and } \mu \neq \lambda.
$$

### 練習問題 {#alg-iii-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
