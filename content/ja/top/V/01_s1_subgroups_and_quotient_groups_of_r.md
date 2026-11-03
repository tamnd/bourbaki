---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 1
section_title: Subgroups and quotient groups of R
lang: ja
source: top-v-x
pdf_pages: 0013-0017, 0030-0031
extraction: ocr
subsections:
    - "no": 1
      title: CLOSED SUBGROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 2
      title: QUOTIENT GROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}$ INTO ITSELF
      page: 0
      pdf_page: 15
    - "no": 4
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 15
statements: 13
exercises: 3
content_sha256: d98a61fee9ceca1938b17c0a167f1bd5cfc6311c1eea6a7cd3647dbf9456babb
translated_from: content/en/top/V/01_s1_subgroups_and_quotient_groups_of_r.md
translation_method: google
source_content_sha256: 1e96322726cdb481cae00351a70dc8c5c1282af2de71cdb8ab479eeee32a02d2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: ae28f5ba6fcccc807338c3286737a39a8d8e79a770041175fca391728514d36f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. $\mathbf{R}$ の部分群と剰余群

### 1. 閉店 $\mathbf{R}$中部分群

#### 命題 1 {#top-v-s1-prop-1 .statement tag=0BV0}

*$\mathbf{R}$ と $\{0\}$ を除く、加法群 $\mathbf{R}$ のすべての閉じた部分群は、形 $a.\mathbf{Z}$ の離散群であり、$a > 0$* (他の語では、整数で構成されます) $a$中倍数）。

まず、$\mathbf{R}$ のすべての非離散部分群が $\mathbf{R}$ に密集していることを示します。 $\mathbf{R}$ の部分群 $G$ が離散的でない場合、$\varepsilon > 0$ ごとに $G$ に点 $x \neq 0$ があり、属するから区間 $[-\varepsilon, +\varepsilon]$ になります。 $x$ 属するから $G$ までのすべての整数倍数と、$G$ の長さ $> \varepsilon$ 含む元のすべての区間なので、$G$ $\mathbf{R}$は密です。

したがって、$\mathbf{R}$ 自体を除く$\mathbf{R}$ のすべての閉じた部分群は離散的です。 $\{0\}$ を除く$\mathbf{R}$ のすべての離散部分群 $G$ が形 $a.\mathbf{Z}$ であり、$a > 0$ であることを示すことが残っています。ここで、関係 $-G = G$ は、$G$ の元 $> 0$ の集合 $H$ が空ではないことを示しています。 区間 $[0, b]$ および $G$ の $b \in H$、共通部分が *コンパクトかつ離散* であるため、*有限* です。 $a$ を $[0, b]$ に含まれる $H$ の最小の元とし、$x \in G$ ごとに $m = [x/a]$、$x/a$ の整数部分を代入します。次に、$x - ma \in G$ と $0 \leq x - ma < a$ があります。 $a$の定義により、$x - ma = 0$となり、したがって$G = a.\mathbf{Z}$となります。

### 2. $\mathbf{R}$ の剰余群

$\mathbf{R}$ のすべての *ハウスドルフ* 剰余群は形 $\mathbf{R}/H$ のもので、$H$ は $\mathbf{R}$ (章 III, § 2, no. 6, 命題 18) の *閉じた* 部分群です。したがって、命題 1/no. 1 まで:

#### 命題 2 {#top-v-s1-prop-2 .statement tag=0BV1}

*ハウスドルフ剰余群のうち * $\mathbf{R}$、*以外* $\{0\}$、* は群* $\mathbf{R}/a\mathbf{Z}$ ($a \geqslant 0$) です。
*もし* $a$ *と* $b$ *が* $> 0$、*自己同型* $x \to b/a\,x$ *の* $\mathbf{R}$ *変換* $a\mathbf{Z}$ *が* $b\mathbf{Z}$、*したがって* (章) III, § 2, no. 8、注意 3) *剰余群* $\mathbf{R}/a\mathbf{Z}$ * と* $\mathbf{R}/b\mathbf{Z}$ * は同型です。その他の語*:

#### 命題 3 {#top-v-s1-prop-3 .statement tag=0BV2}

*$\mathbf{R}$ の *すべてのハウスドルフ剰余群、*以外* $\mathbf{R}$ * および* $\{0\}$、 *は群* $\mathbf{R}/\mathbf{Z}$ と同型です。

#### 定義 1 {#top-v-s1-def-1 .statement tag=0BV3}

*トポロジー 群* $\mathbf{R}/a\mathbf{Z}$ ($a > 0$) * 実数モジュロ* $a$ の加法群と呼ばれます。 *トポロジカル群* $\mathbf{R}/\mathbf{Z}$ *は* $\mathbf{T}$ で表されます。 *トポロジカル空間として、* $\mathbf{T}$ * は 1 次元トーラス* と呼ばれます (言葉の乱用により、トポロジカル群 $\mathbf{T}$ は 1 次元トーラスとも呼ばれます)。

#### 注意 1 {#top-v-s1-n2-rem-1 .statement tag=0BV4}

*関係* $x \equiv y \pmod{a\mathbf{Z}}$ *通常は* $x \equiv y \pmod{a}$、*または単に* $x \equiv y (a)$、*そして*「xとyはaを法として合同である」と読みます*。 *それは* $x - y$ * が* $a$ の整数倍数であることを意味します。 *とき* $a$ *が整数であるとき、 関係は* $\mathbf{Z}$ *によって、 関係は正確に合同法* $a$ になります。 *これは記法* を正当化します。

#### 注意 2 {#top-v-s1-n2-rem-2 .statement tag=0BV5}

\* *章 VI, § 2, no. 4 でわかるように、トポロジカル空間* $\mathbf{T}$ *実数平面* $\mathbf{R}^2$ では、円* $x^2 + y^2 = 1$ と同相です。 *積空間* $\mathbf{T}^2$ *は * $\mathbf{R}^3$ *(章 VII, § 1, 練習問題 15)* の回転 * トーラスと同同型です。 *これが名前の由来* 「一次元トーラス」 *for* $\mathbf{T}$ *(章 VII, § 1 では、* $\mathbf{T}^n$ *n 次元トーラス)* * と呼びます。

#### 命題 4 {#top-v-s1-prop-4 .statement tag=0BV6}

*トーラス* $\mathbf{T}$ *は、* $\mathbf{R}$ *の形* $[a, a+1]$ *この区間の端点を特定することによって得られる、任意の閉じた区間の商空間と準同型です。コンパクトでローカル接続が可能です*。

すべての $x \in \mathbf{R}$ *合同* $(\bmod\,1)$ *区間* $[a, a+1]$ の一部の数 、*つまり * $x - [x-a]$ です。 *したがって* $\mathbf{T}$ *この区間の標準写像* $\varphi$ *の* $\mathbf{R}$ *上* $\mathbf{R}/\mathbf{Z}$ の像であり、 *したがってコンパクトで接続されています* (章 I, § 9, no. 4、定理 2、および§ 11, no. 2、命題 4)。 *一方、区間* $[a, a+1]$ の 2 つの異なる元は *合同* $(\bmod\,1)$ *それらが区間の終点である場合に限ります。 * $\mathbf{T}$ *したがって、* $\mathbf{T}$ * は * $[a, a+1]$ の商空間と同相であることがわかります * 端点を特定することで得られます* (章 I, § 9, no. 4, 定理 2, 系 4、および § 10, no. 4、命題 8）。 *最後に、* $\mathbf{Z}$ * $\mathbf{R}$、$\mathbf{T} = \mathbf{R}/\mathbf{Z}$ の離散部分群である * は * $\mathbf{R}$ *(章 III, § 2, no. 6, 命題 19)* と * 局所的に同型であり、特にローカルに接続されています (この最後の事実も章 I, § 11, no. 6、命題 12）の帰結。

#### 注意 {#top-v-s1-n2-rem-3 .statement tag=0BV7}

$\mathbf{R}$ の $T = \mathbf{R}/\mathbf{Z}$ への標準写像 $\varphi$ は、半開区間 $[a, a+1[$ に限定されており、この区間の $T$ への連続全単射写像であることに注意してください。逆数写像は、$\varphi(a)$を除く$T$のすべての点で連続ですが、$\varphi(a)$では不連続です。 ときどき同一視する空間 $T$ に区間 $[a, a+1[$ を加え、$T$ の位相の $\varphi$ の下で逆像である位相を付与します。 (章 I, § 1, no. 3);もちろん、この位相は、$\mathbf{R}$の位相によって$[a, a+1[$に引き起こされたものと同じではありません。

### 3. $\mathbf{R}$ の連続準同型がそれ自身に

#### 命題 5 {#top-v-s1-prop-5 .statement tag=0BV8}

トポロジカル群 $\mathbf{R}$ のすべての連続準同型 $f$ は、それ自体内で形 $x \to ax$ になります。ここで、$a \in \mathbf{R}$; $a \neq 0$なら$\mathbf{R}$の自己同型です。

$x \in \mathbf{R}$ と整数 $p \in \mathbf{Z}$ ごとに、$f(px) = pf(x)$ があります。 置き換えること $x$ $(1/p)x$ により、次のようになります。

$$
f\left(\frac{1}{p}x\right) = \frac{1}{p} f(x) \quad \text{if } p \neq 0;
$$

したがって、すべての整数 $p$ と $q \neq 0$ について、

$$
f\left(\frac{p}{q}x\right) = \frac{p}{q} f(x).
$$

その他の語、$f(rx) = rf(x)$ では、すべての有理数数 $r$ が対象となります。今、$t$ がいずれかの実数である場合、$f$ の連続性により、次のようになります。

$$
f(tx) = \lim_{r \to t, r \in \mathbf{Q}} f(rx) = \lim_{r \to t, r \in \mathbf{Q}} rf(x) = \left( \lim_{r \to t, r \in \mathbf{Q}} r \right) f(x) = tf(x).
$$

特に、$a = f(1)$ の場合、$f(t) = at$ があり、命題が証明されます。

したがって、トポロジカル群 $\mathbf{R}$ の自己同型の群は、非ゼロ実数の乗法群 $\mathbf{R}^*$ と同型です。

#### 系 {#top-v-s1-n3-cor-1 .statement tag=0BV9}

$G$ を $\mathbf{R}$ と同型の位相位相群とします。それぞれの $a \in G$ には、$f_a(1) = a$ となる $\mathbf{R}$ の $G$ への連続する準同型 $f_a$ が 1 つあり、この準同型は、$a$ の場合、$\mathbf{R}$ の $G$ への同型です。 $G$ の零元ではありません。

### 4. $\mathbf{R}$ の連続準同型のローカル定義をトポロジカル群に変換

$G$ 生成する $G$ の群 $G$ と部分集合 $A$ が与えられた場合、$G$ の 2 つの準同型 $f, g$ が群 $G'$ になることは明らかです。 $A$の点ごとに同じ値を取った場合、一致する。しかし、準同型の$A$$G$の$f$の$G'$できないの値は、一般に恣意的に解釈されます。 $G$ と $G'$ が乗算的に書かれている場合、これらの値は、$x \in A, y \in A$ と $xy \in A$ のように、対 $(x, y)$ ごとに満たす条件 $f(xy) = f(x)f(y)$ でなければなりません。さらに、この必要な条件は一般に十分ではありません。

特に、トポロジカル群 $G'$ できないを伴うトポロジカル群 $G$ の *ローカル同型* は、常に $G$ の準同型 (連続かどうか) から $G'$ に拡張されます。 たとえば、$\mathbf{R}$ できないを含む$T$ のローカル同型 $f$ は、$T$ の準同型から $\mathbf{R}$ に拡張されます。なぜなら、$f$が$o$の近傍$V$で定義されている場合、$\frac{1}{p}$属するから$V$の類$x \pmod{\mathbf{Z}}$となる整数$p > 0$が存在します。 $x$ には $T$ に位数 $p$ があるため、$T$ の準同型ごとに $\mathbf{R}$ に入るその像は必然的に $o$ となり、したがって $f(x)$ とは仮定だけ区別されます。

この点で、トポロジー 群 $\mathbf{R}$ は次の性質を享受します。

#### 命題 6 {#top-v-s1-prop-6 .statement tag=0BVA}

*$I$ を $\mathbf{R}$ の区間と含む $o$ と少なくとももう 1 つの点とします。 $f$ を $I$ の連続写像としてトポロジカルな群 $G$ (乗算的に書かれる) とし、点 $(x, y)$ のそれぞれの対が $x \in I, y \in I$ となるように $f(x+y) = f(x)f(y)$ とする。 $x + y \in I$。次に、$\mathbf{R}$ から $G$ へのユニークな連続準同型があり、拡大する $f$.*。

$I$ 生成する群 $\mathbf{R}$ であるため、拡大の一意性 (存在する場合) は、前の注意の後に続きます。私たちはそのような拡大の存在を確立しなければなりません。

$n$ が整数 $> 0$ で、$x \in I$ と $nx \in I$ の場合、$n$ の帰納法までに $f(nx) = (f(x))^n$ が得られます (すべての整数 $m$ については $mx \in I$ なので、 $1 \leq m \leq n$）。 $J = \bigcup_{n \in \mathbf{N}} nI$を入れてください。 $J$ は、$o$ が $I$ の内部点であるかどうかに応じて、行全体 $\mathbf{R}$ か、区間 $[0, +\infty[$ または $[-\infty, 0]$ のいずれかです。 $x \in J$ の場合、$n$ が十分大きい整数 $> 0$ であるときは常に $x/n \in I$ になります。 $x \in J$ と $m, n$ を 2 つの整数 $> 0$ とし、$x/n \in I$ と $x/m \in I$ とします。それから$x/mn \in I$、したがって

$$
f\left( \frac{x}{m} \right) = \left( f\left( \frac{x}{mn} \right) \right)^n \quad \text{and} \quad f\left( \frac{x}{n} \right) = \left( f\left( \frac{x}{mn} \right) \right)^m;
$$

他の語、元、$G$の$(f(x/n))^n$は、$x/n \in I$のように、すべての整数$n > 0$で同じです。これを元を $f_1(x)$ で表しましょう。 $f_1$は、$J$の写像を$G$に変換したもので、$I$の$f$と一致し、したがって点$o$で連続します（$J$に関して）。 $x, y$ を J の 2 つの元とし、n を十分大きい整数 > 0 とし、$\frac{x}{n} \in I, \frac{y}{n} \in I$ と $\frac{x+y}{n} \in I$ とします。それから

$$
f\left( \frac{x+y}{n} \right) = f\left( \frac{x}{n} \right) f\left( \frac{y}{n} \right) = f\left( \frac{y}{n} \right) f\left( \frac{x}{n} \right),
$$

これは、$f\left( \frac{x}{n} \right)$ と $f\left( \frac{y}{n} \right)$ が通勤していることを示しています。 $f_1$ の定義までに、$f_1(x+y) = f_1(x) f_1(y)$ になります。 $J = \mathbf{R}$ の場合、証明は完了です。そうでない場合は、$J = [0, +\infty[$ と言い、$x < 0$ 定義する $f_1(x)$ をそれぞれ $(f_1(-x))^{-1}$ とします。その場合、関係 $f_1(x+y) = f_1(x) f_1(y)$ はすべての $x \in \mathbf{R}$ とすべての $y \in \mathbf{R}$ に対して有効のままです。 $x < 0$ と $y < 0$ の場合、これは明らかです。 $x \geqslant 0$、$y < 0$、$x + y \geqslant 0$ の場合は、$f_1(x) = f_1(x+y) f_1(-y)$ から続きます。同様に、$x \geqslant 0, y < 0$ と $x + y < 0$ の場合、次のようになります。

$$
f_1(-y) = f_1(-x-y) f_1(x);
$$

$x < 0$ と $y \geqslant 0$ の証明と同様です。したがって、$f_1$ は G の $\mathbf{R}$ の準同型であるため、G の $f_1(0) = e$、単位元であることがわかります。そして、$f_1$ は J に関して連続であるため、右側の 0 に極限があり、$e$ に等しいです。 $f_1(-x) = (f_1(x))^{-1}$ なので、$f_1$ の左側の 0 には極限があり、$e$ と等しくなります。したがって、$f_1$ は 0 で連続し、証明は完了します。

#### 系 {#top-v-s1-n4-cor-1 .statement tag=0BVB}

*f をトポロジカル群 G を持つ $\mathbf{R}$ のローカル同型とします。 次に、G のオープン部分群に、一意の厳密な $\mathbf{R}$ の射があり、これは f がすべて点の 0 の近傍と一致するなります。

$\overline{f}$ を、G への $\mathbf{R}$ の連続準同型とし、その一致するに $f$ が含まれる、開いた区間 I の点で、含む 0 で、集合に含まれます。 $f$ が定義されています。 G の単位元の仮定含む近傍による $\overline{f}(\mathbf{R})$、したがって (章 III, § 2, no. 1, 系から命題 4) は G のオープン部分群です。そして、$\overline{f}$ は、章 III, § 2, no. 8、命題 24 による、$\mathbf{R}$ の $\overline{f}(\mathbf{R})$ への厳密な射です。

#### 命題 7 {#top-v-s1-prop-7 .statement tag=0BVC}

*局所的に $\mathbf{R}$ と同型である接続されたすべての群 G は、$\mathbf{R}$ または $\mathbf{T}$ のいずれかと同型です。*

G 拡大するを伴う $\mathbf{R}$ のローカル同型から、G のオープン部分群 (系から命題 6) への $\mathbf{R}$ の厳密な射への場合、G が接続されているため、G 自体へ。 したがって、G は $\mathbf{R}$ の剰余群と同型です。 G はハウスドルフであり、単位元だけで構成されていないため (局所的に $\mathbf{R}$ と同型であるため)、no. 2 の命題 3 によって $\mathbf{R}$ または $\mathbf{T}$ のいずれかと同型です。

### 練習問題 {#top-v-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
