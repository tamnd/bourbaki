---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 10
section_title: Inverse and direct limits
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 118-123, 179
pdf_pages: 0142-0147, 0203-0203
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE SYSTEMS OF MAGMAS
      page: 118
      pdf_page: 142
    - "no": 2
      title: INVERSE LIMITS OF ACTIONS
      page: 119
      pdf_page: 143
    - "no": 3
      title: DIRECT SYSTEMS OF MAGMAS
      page: 120
      pdf_page: 144
    - "no": 4
      title: DIRECT LIMIT OF ACTIONS
      page: 123
      pdf_page: 147
statements: 5
exercises: 2
content_sha256: 274f61d5cd7919fabb7305b65446272718fd350a88d0fbc681e4df5d4e7acf9b
translated_from: content/en/alg/I/10_s10_inverse_and_direct_limits.md
translation_method: google
source_content_sha256: 3a49dcd1591d3ccd8d3da36eb91e210dee0ffea0f51202486e0a783d55ffe2f0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 68e03c36c18f5a46177209fbaa2818b50fb2201e35b44a39028f07b94a76c7fb
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 10。逆数と正数極限

この段落全体を通じて、I は空ではない予約注文集合、$\alpha \leq \beta$ は I の予約注文を示します。 インデックス集合 I に対する逆集合系 (直接) の概念は、*集合理論*、III, § 7, no. 1 (I が右向きであるという仮説の下で、*集合理論*、III, § 7, no. 5) で定義されます。

### 1. マグマの逆系

#### 定義 1 {#alg-i-s10-def-1 .statement tag=05JH}

*指数付け集合 I に対するマグマの逆数系は、 集合* $(\mathbf{E}_\alpha, f_{\alpha\beta})$ の逆数系です。 *I に対して、それぞれ* $\mathbf{E}_\alpha$ * はマグマ構造を持ち、それぞれ* $f_{\alpha\beta}$ * は存在しますマグマ準同型.*

$(\mathbf{E}_\alpha, f_{\alpha\beta})$ をマグマの逆数系とし、その法則は乗算的に書かれます。逆数極限集合 $E = \lim_{\leftarrow} \mathbf{E}_\alpha$ は、$(x_\alpha)_{\alpha \in I}$ 族の積マグマ $\prod_{\alpha \in I} \mathbf{E}_\alpha$ からなるの部分集合であり、$\alpha \leq \beta$ に対して $x_\alpha = f_{\alpha\beta}(x_\beta)$ になります。 $(x_\alpha)$ と $(y_\alpha)$ 属するが E の場合、$\alpha \leq \beta$、$x_\alpha = f_{\alpha\beta}(x_\beta)$、$y_\alpha = f_{\alpha\beta}(y_\beta)$ については、$x_\alpha y_\alpha = f_{\alpha\beta}(x_\beta) f_{\alpha\beta}(y_\beta) = f_{\alpha\beta}(x_\beta y_\beta)$ になります。したがって、E は $\prod_{\alpha \in I} \mathbf{E}_\alpha$ のサブマグマです。 E には $\prod_{\alpha \in I} \mathbf{E}_\alpha$ の結果によって誘発される法則が与えられます。得られたマグマはと呼ばれます

† ポジティブが $> 0$ を意味する現在の用語は避けます。

マグマ $E_\alpha$ の逆極限マグマ。次の普遍性をお楽しみいただけます。

(a) すべての$\alpha \in I$、標準写像 $f_\alpha$ の $E$ から $E_\alpha$ は、 $E$ の $E_\alpha$ へのマグマ準同型です。 $\alpha \leq \beta$の場合は$f_\alpha = f_{\alpha \beta} \circ f_\beta$。

(b) マグマ $F$ と準同型 $u_\alpha : F \to E_\alpha$ が与えられ、$\alpha \leq \beta$ に対して $u_\alpha = f_{\alpha \beta} \circ u_\beta$ が得られるとします。すべての $\alpha \in I$ (つまり $x \mapsto u(x) = (u_\alpha(x))_{\alpha \in I}$) に対して $u_\alpha = f_\alpha \circ u$ となる準同型 $u : F \to E$ が 1 つだけ存在します。

マグマ $E_\alpha$ が結合性 (それぞれ可換性) であれば、$E$ も同様です。 各マグマ $E_\alpha$ が単位元 $e_\alpha$ を受け入れ、準同型 $f_{\alpha \beta}$ が単体であると仮定します。 次に、$e = (e_\alpha)_{\alpha \in I}$ 属するから $E$ 、$e_\alpha = f_{\alpha \beta}(e_\beta)$ 、$\alpha \leq \beta$ となり、マグマ $E$ の単位元になります。上記の記法、準同型 $f_\alpha$ は単体であり、$u_\alpha$ が単体である場合、$u$ も単体です。 さらに、$E$ の要素 $x = (x_\alpha)_{\alpha \in I}$ は、$x_\alpha$ のそれぞれが対応するマグマ $E_\alpha$ と $x^{-1} = (x_\alpha^{-1})_{\alpha \in I}$ で反転可能な場合にのみ反転可能です。これは、$\alpha \leq \beta$ に対する式 $f_{\alpha \beta}(x_\beta^{-1}) = f_{\alpha \beta}(x_\beta)^{-1} = x_\alpha^{-1}$ から導き出されます。

これらの注意から、マグマ $E_\alpha$ がモノイド (それぞれ群) で、$f_{\alpha \beta}$ がモノイド準同型である場合、マグマ $E$ はモノイド (それぞれ群) であると推定できます。この場合、モノイドの逆系 (それぞれ群) について話します。 普遍性は直ちにこの件に移ります。

環 $(E_\alpha, f_{\alpha \beta})$ の逆系を定義し、$E = \lim \leftarrow E_\alpha$ が積環 $\prod_{\alpha \in I} E_\alpha$ の部分環であることを検証するのは読者に任されており、これは環 $E_\alpha$ の逆限界環と呼ばれます。普遍的な性質がこの場合にも当てはまることが確認できます。

$\mathfrak{C} = (E_\alpha, f_{\alpha \beta})$ と $\mathfrak{C}' = (E'_\alpha, f'_{\alpha \beta})$ を、同じ指数付け集合に対するマグマの 2 つの逆数系 (それぞれモノイド、群、環) とします。 $\mathfrak{C}$ の $\mathfrak{C}'$ への準同型は、写像 $u_\alpha : E_\alpha \to E'_\alpha$ の逆系 $(u_\alpha)_{\alpha \in I}$ であり、それぞれの $u_\alpha$ は準同型になります。 これら条件, 写像 $\lim \leftarrow E_\alpha$ の $\lim \leftarrow E'_\alpha$ への$u = \lim \leftarrow u_\alpha$ は準同型 (cf. 集合理論 , III, § 7, no. 2) です。

### 2. 作用の逆極限

同じインデックス集合 $I$ に対して、集合 $(\Omega_\alpha, \phi_{\alpha \beta})$ と $(E_\alpha, f_{\alpha \beta})$ の 2 つの逆数系が与えられたとします。 $E_\alpha$ 上の $\Omega_\alpha$ のすべての $\alpha \in I$ 作用に対して次のように与えられるとします。

(1)
$$
f_{\alpha \beta}(\omega_\beta x_\beta) = \phi_{\alpha \beta}(\omega_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
$\alpha \leq \beta, x_\beta \in E_\beta, \omega_\beta \in \Omega_\beta$の場合。そして、考慮されている作用の族は、作用の逆系であると言われます。 $\Omega = \lim \leftarrow \Omega_\alpha$ と $E = \lim \leftarrow E_\alpha$ としましょう。 $x = (x_\alpha)_{\alpha \in I}$ 属するから $E$ および $\omega = (\omega_\alpha)_{\alpha \in I}$ 属するから $\Omega$ の場合、(1) により $\omega . x = (\omega_\alpha . x_\alpha)_{\alpha \in I}$ 属するが E になります。したがって、E 上の $\Omega$ の作用は、$E_\alpha$* 上の $\Omega_\alpha$ の作用の *反転極限と呼ばれます。

上記は、$\Omega_\alpha$ がモノイドであり、$E_\alpha$ 上の $\Omega_\alpha$ の各作用が演算である場合に特に当てはまります。すると、これら演算の逆元極限はE上のモノイドの演算になります。

群の逆数系の逆数極限を演算子で定義する計算し、この極限が演算子で群であることを検証するのは読者に委ねられています。

### 3. マグマの直接系

このNo.そして以下では、I が *右向き* であると仮定します。

#### 定義 2 {#alg-i-s10-def-2 .statement tag=05JI}

*インデックス集合Iに対するマグマの直接系は、集合*の直接系です* $(E_\alpha, f_{\beta\alpha})$ *Iと比較して、それぞれ* $E_\alpha$ *マグマ構造があり、それぞれ* $f_{\beta\alpha}$ *マグマです準同型.*

$(E_\alpha, f_{\beta\alpha})$をマグマの直接系とします。 E は、E への $E_\alpha$ の直接の極限集合 $\lim_{\longrightarrow} E_\alpha$ と $f_\alpha$ 標準写像を表します。

(2)
$$
f_\beta \circ f_{\beta\alpha} = f_\alpha \quad \text{for } \alpha \leq \beta,
$$

(3)
$$
E = \bigcup_{\alpha \in I} f_\alpha(E_\alpha).
$$

(2)によっても、

(4)
$$
f_\alpha(E_\alpha) \subset f_\beta(E_\beta) \quad \text{for } \alpha \leq \beta.
$$

$x_\alpha, y_\alpha \in E_\alpha$ が $f_\alpha(x_\alpha) = f_\alpha(y_\alpha)$ である場合、$f_{\beta\alpha}(x_\alpha) = f_{\beta\alpha}(y_\alpha)$ であるような $\beta \geq \alpha$ が存在します。

#### 命題 1 {#alg-i-s10-prop-1 .statement tag=05JJ}

*E には、写像* $f_\alpha : E_\alpha \to E$ * が準同型であるマグマ構造が 1 つだけ存在します。マグマ* $E_\alpha$ * が結合性 (可換性) であれば、E も同様です。マグマ* $E_\alpha$ * と準同型* $f_{\beta\alpha}$ * が単体である場合、マグマ* E * と準同型* $f_\alpha$ も同様です。

マグマ $E_\alpha$ は乗算的に書かれます。

Eに$x, y$があるとします。Iには$\alpha$、$E_\alpha$には$x_\alpha, y_\alpha$が存在し、$x = f_\alpha(x_\alpha)$と$y = f_\alpha(y_\alpha)$が存在します。 $f_\alpha$ が準同型であるマグマ構造が E 上に存在する場合、$x.y = f_\alpha(x_\alpha y_\alpha)$、よってはこのマグマ構造の *一意性* になります。

存在を証明するために、Iの$\alpha, \beta$、$E_\alpha$の$x_\alpha, y_\alpha$、$E_\beta$の$x'_\beta, y'_\beta$、関係について証明しなければならない

(5)
$$
f_\alpha(x_\alpha) = f_\beta(x'_\beta), \qquad f_\alpha(y_\alpha) = f_\beta(y'_\beta)
$$
$f_\alpha(x_\alpha y_\alpha) = f_\beta(x'_\beta y'_\beta)$を暗示します。 $\gamma \geq \alpha$ と $\gamma \geq \beta$ の場合、集合 $x_\gamma = f_{\gamma\alpha}(x_\alpha)$、$y_\gamma = f_{\gamma \alpha}(y_\alpha), x'_\gamma = f_{\gamma \beta}(x'_\beta), y'_\gamma = f_{\gamma \beta}(y'_\beta)$ となります。直接極限の定義により、$\gamma \geq \alpha, \gamma \geq \beta, x_\gamma = x'_\gamma, y_\gamma = y'_\gamma$と$I$に$\gamma$が存在します。それから
$$
f_\alpha(x_\alpha y_\alpha) = f_\gamma(f_{\gamma \alpha}(x_\alpha y_\alpha)) = f_\gamma(x_\gamma y_\gamma) = f_\gamma(x'_\gamma y'_\gamma) = f_\gamma(f_{\gamma \beta}(x'_\beta y'_\beta)) \\
= f_\beta(x'_\beta y'_\beta).
$$
マグマ $E_\alpha$ が結合していると仮定します。 $x, y, z$ を $E$ に入れます。 $E_\alpha$ には、$\alpha \in I$ と元 $x_\alpha, y_\alpha, z_\alpha$ が存在します。
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad z = f_\alpha(z_\alpha).
$$
次に、$xy = f_\alpha(x_\alpha y_\alpha)$、よって、$(xy)z = f_\alpha((x_\alpha y_\alpha)z_\alpha)$;同様に
$$
x(yz) = f_\alpha(x_\alpha(y_\alpha z_\alpha)),
$$
よって $(xy)z = x(yz)$ は $(x_\alpha y_\alpha)z_\alpha = x_\alpha(y_\alpha z_\alpha)$ です。可換マグマの場合も同様に扱われます。

最後に、各マグマ $E_\alpha$ には単位元 $e_\alpha$ があり、$\alpha \leq \beta$ には $f_{\beta \alpha}(e_\alpha) = e_\beta$ があるとします。 $I$の$\alpha, \beta$の場合、$\gamma \geq \alpha$と$\gamma \geq \beta$、よってを含む$I$には$\gamma$が存在します。
$$
f_\alpha(e_\alpha) = f_\gamma(f_{\gamma \alpha}(e_\alpha)) = f_\gamma(e_\gamma) = f_\gamma(f_{\gamma \beta}(e_\beta)) = f_\beta(e_\beta)
$$
したがって、$E$ には元 $e$ が存在し、すべての $\alpha \in I$ に対して $f_\alpha(e_\alpha) = e$ が存在します。 $x$ を $E$ に入れます。 選ぶ $\alpha \in I$ と $x_\alpha \in E_\alpha$ は $x = f_\alpha(x_\alpha)$ となります。それから
$$
ex = f_\alpha(e_\alpha) \cdot f_\alpha(x_\alpha) = f_\alpha(e_\alpha \cdot x_\alpha) = f_\alpha(x_\alpha) = x
$$
同様に $x \cdot e = x$ なので、$e$ は $E$ の単位元になります。

マグマ $E$ はマグマ $E_\alpha$ の *直接極限と呼ばれます。

#### 命題 2 {#alg-i-s10-prop-2 .statement tag=05JK}

*$(E_\alpha, f_{\beta \alpha})$ * をマグマの直接系とし、* $E$ * をその直接の極限* $f_\alpha : E_\alpha \to E$ *標準準同型とします。マグマ* $F$ * と準同型* $u_\alpha : E_\alpha \to F$ * が * $\alpha \leq \beta$ に対して* $u_\alpha = u_\beta \circ f_{\beta \alpha}$ になるように与えられたとします。 *唯一の準同型* $u : E \to F$ *そのような* $u_\alpha = u \circ f_\alpha$ *すべて* $\alpha \in I$ が存在します。 *マグマ* $E_\alpha$ * と* $F$ * と準同型* $f_{\beta \alpha}$ * と* $u_\alpha$ * が単体である場合、 準同型* $u$ * は単体です*。

私たちは (*集合理論*, III, § 7, no. 6, 命題 6)、すべての $\alpha \in I$ に対して $u_\alpha = u \circ f_\alpha$ となる写像 $u : E \to F$ が 1 つだけ存在することを知っています。 $u$ が準同型であることを確認します。$x, y$ を $E$ に、$\alpha$ を $I$ に、$x_\alpha, y_\alpha$ を $E_\alpha$ にすると、$x = f_\alpha(x_\alpha)$ と $y = f_\alpha(y_\alpha)$ になります。その後、$xy = f_\alpha(x_\alpha y_\alpha)$、よって
$$
u(xy) = u(f_\alpha(x_\alpha y_\alpha)) = u_\alpha(x_\alpha y_\alpha) = u_\alpha(x_\alpha)u_\alpha(y_\alpha) \\
= u(f_\alpha(u_\alpha))u(f_\alpha(y_\alpha)) = u(x)u(y).
$$
ここで単体の場合を考え、$e_\alpha$ は $E_\alpha$ の単位元を、$e$ は $E$ のそれを、$e'$ は $F$ の単位元を表すものとします。 選ぶ $\alpha \in I$、その後 $e = f_\alpha(e_\alpha)$、よって
$$
u(e) = u(f_\alpha(e_\alpha)) = u_\alpha(e_\alpha) = e'
$$
$u_\alpha$ は単一です。したがって、$u$ は単一です。

マグマの直接系の概念との類推により、モノイドの直接系または群を定式化できます。 命題 1は、モノイド$(E_\alpha, f_{\beta\alpha})_{\alpha, \beta \in I}$の直接系の極限であるマグマEがモノイドであることを示しています。 $E_\alpha$ が群である場合、E は群であることを示します。 $x \in E, \alpha \in I$ と $x_\alpha \in E_\alpha$ を $x = f_\alpha(x_\alpha)$ となるようにします。 E の元 $y = f_\alpha(x_\alpha^{-1})$ は x (§ 2, no. 3) の逆数です。モノイドの直接系や群の場合、命題2の普遍性はすぐにオーバーします。

読者は定義する直接系の環に任されています。 $(A_\alpha, f_{\beta\alpha})$ をそのような直接系とします。 $A = \lim \overrightarrow{A_\alpha}$ と $f_\alpha : A_\alpha \to A$ 標準準同型とします。 A には、$A_\alpha$ と $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$ の $\alpha \in I, x_\alpha, y_\alpha$ に対して $x + y = f_\alpha(x_\alpha + y_\alpha), xy = f_\alpha(x_\alpha y_\alpha)$ によって特徴付けられる唯一の加算と乗算が存在します。 加法では、A は可換群であり、乗法は結合的かつ単体です。 最後に、A の $x, y, z$、I の選ぶ $\alpha$、および $A_\alpha$ の $x_\alpha, y_\alpha$ と $z_\alpha$ について、
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha) \quad \text{and} \quad z = f_\alpha(z_\alpha).
$$
それから
$$
(x + y) \cdot z = f_\alpha(x_\alpha + y_\alpha)f_\alpha(z_\alpha) = f_\alpha((x_\alpha + y_\alpha)z_\alpha)
= f_\alpha(x_\alpha z_\alpha + y_\alpha z_\alpha) = f_\alpha(x_\alpha z_\alpha) + f_\alpha(y_\alpha z_\alpha) = xz + yz
$$
関係 $x(y + z) = xy + xz$ も同様に証明されます。 他の語では、Aは環の構造を持ち、$f_\alpha$がすべての$\alpha \in I$に対して環準同型であるという事実によって特徴付けられます。

環 A は、環 $A_\alpha$ の直接極限と呼ばれます。 命題 2 拡大するすぐに環の場合。

#### 命題 3 {#alg-i-s10-prop-3 .statement tag=05JL}

(a) *$A_\alpha$ がゼロ以外の場合、A はゼロ以外になります。*
(b) *$A_\alpha$が整域の場合、Aは整域です。*
(c) *$A_\alpha$が体の場合、Aは体です。*

$0_\alpha, 1_\alpha$を$A_\alpha$の零と単位元、Aの0、1零、単位元とします。$f_\alpha(0_\alpha) = 0, f_\alpha(1_\alpha) = 1$となるような$\alpha \in I$が存在します。 $0 = 1$ の場合、$f_{\beta\alpha}(0_\alpha) = f_{\beta\alpha}(1_\alpha)$、つまり $0_\beta = 1_\beta$ となるような $\beta \geq \alpha$ が存在します。これは (a) を証明します。

$A_\alpha$ が整域であるとします。すると、(a) により A は可換で非ゼロになります。 $x, y$ を A の元とし、$xy = 0$ とします。 $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$ となるような $\alpha \in I$ と $x_\alpha, y_\alpha \in A_\alpha$ が存在します。次に$f_\alpha(x_\alpha y_\alpha) = xy = 0 = f_\alpha(0_\alpha)$。したがって、$f_{\beta\alpha}(x_\alpha y_\alpha) = f_{\beta\alpha}(0_\alpha)$ となるような $\beta \geq \alpha$ が存在します。 $A_\beta$ は整域なので、$f_{\beta\alpha}(x_\alpha) = 0_\beta$ または $f_{\beta\alpha}(y_\alpha) = 0_\beta$ となり、$x = 0$ または $y = 0$ になります。これは (b) を証明します。

$A_\alpha$ が体であるとします。次に(a)で$A \neq \{0\}$。 $x$ を A の非ゼロ元とします。 $x = f_\alpha(x_\alpha)$ となるような $\alpha \in I$ と $x_\alpha \in A_\alpha$ が存在します。すると、$x_\alpha \neq 0$ と $f_\alpha(x_\alpha^{-1})$ は A の $x$ の逆数になります。これは (c) を証明します。

$\mathfrak{E} = (E_\alpha, f_{\beta\alpha})$ と $\mathfrak{E}' = (E'_\alpha, f'_{\beta\alpha})$ を 2 つのマグマ直接系とします (それぞれモノイド、群、環)。 $\mathfrak{E}$ の準同型を $\mathfrak{E}'$ にすると、写像 $u_\alpha : E_\alpha \to E'_\alpha$ の直接系 $(u_\alpha)_{\alpha \in I}$ となり、それぞれの $u_\alpha$ は準同型になります。この条件, 写像 $u = \lim u_\alpha$ $E = \lim E_\alpha$ から $E' = \lim E'_\alpha$ は、準同型 (cf. *集合理論*, III, § 7, no. 6) です。

### 4. 直接極限/作用

同じインデックスセット $I$ に対して、セットの 2 つの直接システム $(\Omega_\alpha, \phi_{\beta \alpha})$ と $(E_\alpha, f_{\beta \alpha})$ があり、各 $\alpha \in I$ に対して $E_\alpha$ に対する $\Omega_\alpha$ のアクションが与えられているとします。 次のように仮定します。

$$
f_{\beta \alpha}(\omega_\alpha \cdot x_\alpha) = \phi_{\beta \alpha}(\omega_\alpha) \cdot f_{\beta \alpha}(x_\alpha)
$$

$\alpha \leq \beta, \omega_\alpha \in \Omega_\alpha$ と $x_\alpha \in E_\alpha$ の場合。 すると、検討中の作用の家族は作用*の*直接系であると言われます。 It is easily verified as in Proposition 2 that there exists an action $h$ of $\Omega = \lim \Omega_\alpha$ on $E = \lim E_\alpha$ which is described as follows: let $\omega \in \Omega$ and $x \in E$; choose $\alpha \in I$ and $\omega_\alpha \in \Omega_\alpha, x_\alpha \in E_\alpha$ such that $\omega = \phi_\alpha(\omega_\alpha)$ and $x = f_\alpha(x_\alpha)$ ($\phi_\alpha : \Omega_\alpha \to \Omega$ and $f_\alpha : E_\alpha \to E$ denote the canonical mappings); then $\omega \cdot x = f_\alpha(\omega_\alpha \cdot x_\alpha)$. $E$の$\Omega$の作用は、$E_\alpha$の$\Omega_\alpha$の作用の*直接極限と呼ばれます。

$\Omega_\alpha$ がモノイドで、$E_\alpha$ 上の $\Omega_\alpha$ のそれぞれの作用が演算である場合、直接の極限作用は演算です。

演算子を使用して直接系または群の直接極限を定義するにし、演算子を使用してこの極限が群であることを確認するのは読者に委ねられています。

### 練習問題 {#alg-i-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
