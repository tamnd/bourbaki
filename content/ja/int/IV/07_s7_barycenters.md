---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 7
section_title: Barycenters
lang: ja
source: int-i-vi
book_pages: INT IV.142-INT IV.148
pdf_pages: 0208-0225, 0249-0255
extraction: ocr
subsections:
    - "no": 1
      title: Definition of barycenters
      page: 101
      pdf_page: 208
    - "no": 2
      title: Extremal points and barycenters
      page: 102
      pdf_page: 209
    - "no": 3
      title: 'Applications: I. Vector spaces of continuous real functions'
      page: 106
      pdf_page: 213
    - "no": 4
      title: 'Applications: II. Vector spaces of continuous complex functions'
      page: 110
      pdf_page: 217
    - "no": 5
      title: 'Applications: III. Algebras of continuous functions'
      page: 111
      pdf_page: 218
    - "no": 6
      title: Uniqueness of integral representations
      page: 115
      pdf_page: 222
statements: 31
exercises: 10
content_sha256: 30cea19c0e164bb10d16edc40c1012ca39ece6dde0c7cf88cdcc04a6121e0724
translated_from: content/en/int/IV/07_s7_barycenters.md
translation_method: google
source_content_sha256: a0b29318ee51bbadb84b433570743b81dc51c686140364de87fd714982b23900
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: b563909b3396a8c7ab9a17032a537d9f13f2adaf8d6b5d2aa3d892600f49b893
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 7。重心

### 1. 重心の定義

E を $\mathbf{R}$ 上の局所凸ハウスドルフ空間、その双対 $E'$、および $E'$ の代数双対 ${E'}^*$ とし、E は ${E'}^*$ の線形部分空間で正規同定されます。 K を E の圧縮部分集合とします。 K から E への標準単射はコンパクトなサポートで連続しているため、K 上の各小節 $\mu$ に対して積分 $\int x\, d\mu(x)$ が定義され、${E'}^*$ の元になります (Ch. III, §3, No. 1)。さらに、K では、弱い位相 $\sigma({E'}^*, E')$ によって誘発された位相は元の位相と同一です。最後に、C が $\sigma({E'}^*, E')$ を装備した ${E'}^*$ の K の閉じた凸包絡線である場合、$C \cap E$ は元の位相 (または弱体化された位相 $\sigma(E, E')$) の E の K の閉じた凸包絡線です。

#### 定義 1 {#int-iv-s7-def-1 .statement tag=08YJ}

*K を局所凸ハウスドルフ空間 E のコンパクト部分集合とします。総質量の K が 1 に等しいすべての正の尺度 $\mu$ に対して、ベクトル $b_\mu = \int x\, d\mu(x)$ (所属から ${E'}^*$) は $\mu$ の重心と呼ばれます。

#### 例 {#int-iv-s7-n1-exa-1 .statement tag=08YK}

— $\mu$ を、正で総質量 1 の K に関する *離散* 尺度とします。したがって、それは形 $\mu = \sum_{i=1}^n \lambda_i \varepsilon_{x_i}$ であり、$x_i \in K$ と $\lambda_i$ は実数となり、すべての $i$ と $\sum_{i=1}^n \lambda_i = 1$ に対して $\lambda_i \geq 0$ になります。 $\int x\, d\varepsilon_y(x) = y$ (Ch. III, §3, No. 1、*例 3*) 以降、$b_\mu = \int x\, d\mu(x) = \sum_i \lambda_i x_i$。特に、すべての $x \in K$ について、x はメジャー $\varepsilon_x$ の重心です。

#### 命題 1 {#int-iv-s7-prop-1 .statement tag=08YL}

*E を局所凸ハウスドルフ空間、K を E のコンパクト部分集合、E における K の閉じた凸包絡線 C とします。集合 C は、K 上の質量 1 の少なくとも 1 つの正の測度の重心である E の点で構成されます。

これは第 4 章の提案 5 にほかなりません。 III, §3, No. 2 を K の標準単射に E に適用します。

#### 系 {#int-iv-s7-n1-cor-1 .statement tag=08YM}

*E の K の閉じた凸包絡線 C がコンパクトな場合、K 属する上の総質量 1 のすべての正の測度の重心は E になります。

なぜなら、C は、弱い位相 $\sigma(E', E')$ を備えた${E'}^*$ の K の閉じた凸包絡線でもあり、K の標準単射を E に適用するだけで十分です。 III, §3, No. 2。

#### 注意 {#int-iv-s7-n1-rem-1 .statement tag=08YN}

コル。提案 1 は、特に K が凸である場合、または E が準完全である場合に適用できます。

#### 命題 2 {#int-iv-s7-prop-2 .statement tag=08YO}

— K を局所凸ハウスドルフ空間 E のコンパクト凸部分集合、K 上の総質量 1 の正の尺度 $\mu$、その重心 $b_\mu$ とします。 K 上の半連続の下側にあるすべての凸数値写像 $f \geq 0$ について、
$$
f(b_\mu) \leq \int^* f d\mu.
$$
$f$ は、連続アフィン線形写像 $h_\alpha : x \mapsto c_\alpha + \langle x, z'_\alpha \rangle$ の制限から K までの族の上包絡線であることが知られています (TVS、II, §5, No. 4、提案 5)。それから
$$
\int h_\alpha(x) d\mu(x) \leq \int^* f(x) d\mu(x)
$$
$\alpha$ごとに; $\mu$ の総質量は 1 なので、今、$\int h_\alpha(x) d\mu(x) = c_\alpha + \int \langle x, z'_\alpha \rangle d\mu(x)$ です。しかし重心の定義までに$\int \langle x, z'_\alpha \rangle d\mu(x) = \langle b_\mu, z'_\alpha \rangle$。したがって、$\sup_\alpha \int h_\alpha(x) d\mu(x) = \sup_\alpha h_\alpha(b_\mu) = f(b_\mu)$、よってが結論です。

$\mu$ が総質量 1 の K 上の離散正の測度である場合、提案 2 は、K 上の凸写像を定義するとする不等式を新たに導き出します。

#### 系 {#int-iv-s7-n1-cor-2 .statement tag=08YP}

— 有界で下位の半連続である K 上のすべての凸数値写像写像 g について、$g(b_\mu) \leq \int g d\mu$。

$\inf_{x \in K} g(x) = a$ が有限であることに注意し、提案 2 を $g - a$ に適用するだけで十分です。

### 2. 極値点と重心

#### 命題 3 {#int-iv-s7-prop-3 .statement tag=08YQ}

— K をハウスドルフの局所凸型空間 E のコンパクト凸部分集合とし、K の x 点とする。総質量 1 の正の K 上のすべての測度 $\mu$ は、x を重心として認めるが、x を認める総質量 1 の離散正測度の漠然とした閉包集合の中にある。重心として。

曖昧な位相に対して、$\mu$の近所にしましょう。 U は次のような K 上のメジャー $\nu$ で構成されていると仮定できます。
$$
|\mu(f_i) - \nu(f_i)| \leq \delta
$$
写像 $f_i \in \mathscr{C}(K; \mathbf{C})$ ($1 \leq i \leq p$) と数 $\delta > 0$ の有限数の場合。すべての点 $a \in K$ に対して、E に次のような 0 の閉じた凸近傍 $V_a$ が存在します。
$$
|f_i(y) - f_i(a)| \leq \delta/2
$$

$1 \leq i \leq p$ とすべての $y \in W_a = K \cap (a + V_a)$ について。 $K$ はコンパクトなので、$W_{a_j}$ 形が $K$ ($1 \leq j \leq r$) を覆うような、$K$ の点 $a_j$ ($1 \leq j \leq r$) の有限の数が存在します。 $K$ の単位元 $(g_j)_{1 \leq j \leq r}$ の連続分割がカバー$(W_{a_j})$ に従属し、すべての $j$ に対して集合 $\alpha_j = \mu(g_j)$ が発生すると考えます。 $\alpha_j \neq 0$ 集合 $\mu_j = \alpha_j^{-1} g_j \cdot \mu$ の場合、および $\alpha_j = 0$ 集合 $\mu_j = \varepsilon_{a_j}$ の場合。それぞれの尺度 $\mu_j$ は正であり、総質量 1 であり、そのサポートはコンパクトな凸面集合 $W_{a_j}$ に含まれています。さらに、定義までに、

$$
\mu = \sum_{j=1}^r \alpha_j \mu_j
$$

$g_j \cdot \mu = 0$ 以降、$\mu(g_j) = 0$ の場合。 $\alpha_j$ は $\geq 0$ であり、

$$
\sum_{j=1}^r \alpha_j = \sum_{j=1}^r \mu(g_j) = \mu \left( \sum_{j=1}^r g_j \right) = \mu(1) = 1 .
$$

$x_j$ を属するから $W_{a_j}$ までの $\mu_j$ の重心とし (No. 1、提案 1)、離散尺度 $\nu = \sum_{j=1}^r \alpha_j \varepsilon_{x_j}$ を考慮します。それは正で総質量 1 であり、その重心は $\sum_{j=1}^r \alpha_j x_j$ であり、(3) により $\mu$ の重心でもあるため、$x$ と等しくなります。さらに、(2)により、$\operatorname{Supp}(\mu_j) \subset W_{a_j}$以降、$y \in W_{a_j}$はすべて$|f_i(y) - f_i(a_j)| \leq \delta/2$、$i$、よっては$1 \leq i \leq p$は$|\mu_j(f_i) - f_i(a_j)| \leq \delta/2$となります。一方、$x_j \in W_{a_j}$ 以降、また、

$$
|\varepsilon_{x_j}(f_i) - f_i(a_j)| \leq \delta/2
$$

$1 \leq i \leq p$、よって $|\mu_j(f_i) - \varepsilon_{x_j}(f_i)| \leq \delta$、すべての $i$ および $j$。 $\alpha_j$ は $\geq 0$ で、和 1 を持つため、$\nu$ の (3) と定義から、$\nu$ は不等式 (1) を満たすことがわかります。

Q.E.D.

#### 系 {#int-iv-s7-n2-cor-1 .statement tag=08YR}

— *$K$ が $K'$ の閉じた凸包絡線となるように、$K'$ を $K$ の圧縮部分集合とします。 $x \in K'$ が $K$ の極値点であるという位数では、$x$ を重心として、総質量 1 の $K'$ に対する唯一の正の尺度が $\varepsilon_x$ であることが必要かつ十分です。

Suppose $x$ is an extremal point of $K$; to prove that $\varepsilon_x$ is the only positive measure on $K'$, of total mass 1, having $x$ as barycenter, it suffices, by Prop. 3, to see that the set of *discrete* measures $\nu$ on $K'$ that are positive, of total mass 1, and have $x$ as barycenter, reduces to $\varepsilon_x$. しかし、そのような尺度$\nu$は、$1 \leq i \leq r$と$\sum_{i=1}^{r} \lambda_i = 1$に$\lambda_i > 0$を加えた形$\sum_{i=1}^r \lambda_i \varepsilon_{x_i}$であり、$x$が$\nu$の重心である仮定は、$x = \sum_{i=1}^{r} \lambda_i x_i$と書くことができます。 $x$ は極値であるため、これはすべての $i$、よって $\nu = \varepsilon_x$ に対して $x_i = x$ であることを意味します。

逆に、$\varepsilon_x$ が、$x$ を重心とする、総質量 1 の$K'$ における唯一の正の測度であると仮定し、$x$ が極値であることを示しましょう。逆の場合、$0 < \lambda < 1$ と $x = \lambda x' + (1 - \lambda) x''$ のように、$K$ と実数 $\lambda$ の 2 つの異なる点 $x', x''$ が存在します。提案 1 により、$x'$ (それぞれ $x''$) は、総質量 1 の $K'$ 上の正の測度 $\mu'$ (それぞれ $\mu''$) の重心であり、$x$ は $\lambda \mu' + (1 - \lambda) \mu''$ の重心です。したがって$\lambda \mu' + (1 - \lambda) \mu'' = \varepsilon_x$。したがって、$\mu'$ と $\mu''$ は、$\varepsilon_x$、よって $x' = x'' = x$ に比例しますが、これは不合理です。

#### 定理 1 (チョケ) {#int-iv-s7-thm-1 .statement tag=08YS}

— *E を $\mathbf{R}$ 上の局所凸ハウスドルフ空間とし、K を E の計量可能コンパクト凸部分集合、K の極値点の M 集合とする。 集合 M は、K の開集合の可算族の共通部分であり、すべてK の点は、$\mu(K - M) = 0$ となるような K 上のメジャー $\mu$ の重心です。*

最初の主張を証明するには、$\mathbf{R}$ の I 区間 $[0, 1]$ で表します。 K はコンパクトで計量可能であるため、$K \times K \times I$ も同様です。 $x \neq y$ と $0 < \lambda < 1$ が $K \times K \times I$ でオープンであるようなトリプル $(x, y, \lambda)$ によって形成された $K \times K \times I$ の部分集合 U は、$K \times K \times I$ にクローズされた集合の数列 $(F_n)$ が存在し、その和集合は U です(GT、IX, §2, No. 5、提案 7)。 $q(x, y, \lambda) = \lambda x + (1 - \lambda) y$ によって定義される写像 $q : K \times K \times I \to K$ は連続であり、極値点、$K - M = q(U) = \bigcup_n q(F_n)$ の定義によって定義されます。しかし、$F_n$ は $K \times K \times I$ で閉じているためコンパクトです。したがって、$q(F_n)$ はコンパクトであり、したがって K で閉じています。したがって、K では集合 $U_n = K - q(F_n)$ がオープンしており、$M = \bigcap_n U_n$ がございます。

In the continuation of the proof, we shall denote by $u$ a continuous and *convex* numerical function on K, by $G \subset E \times \mathbf{R}$ the graph of $u$, and by S the *closed convex envelope* of G in $E \times \mathbf{R}$.

#### 補題 1 {#int-iv-s7-lem-1 .statement tag=08YT}

— *$\overline{u}$を、K上の$\geq u$であるE上の連続アフィン線形写像の下側包絡線とします。その場合、Sは、$a \in K$と$u(a) \leq b \leq \overline{u}(a)$のように、点$(a, b) \in E \times \mathbf{R}$の集合になります。

ハーン・バナッハ定理によれば、$(a, b)$ から S までの属するについて、$E \times \mathbf{R}$ 上のすべての連続アフィン線形写像 $h$ に対して $h(a, b) \geq 0$ が、$x \in K$ に対して $h(x, u(x)) \geq 0$ であることが必要かつ十分です。 Setting $h(x, t) = f(x) - \lambda t$, where $f$ is a continuous affine linear function on E, we see that the relation $(a, b) \in S$ is equivalent to the following property: the relation

$$
f(x) \geq \lambda u(x) \quad \text{for all } x \in K
$$

暗示する

(5)
$$
f(a) \geq \lambda b .
$$

最初集合 $\lambda = 0$; $E$ 上のすべての連続アフィン線形写像 $f$ に対して (4) が (5) を意味するという事実は、ハーン・バナッハ定理による関係 $a \in K$ と同等です。次に、$-f$による集合 $\lambda = -1$と置き換える $f$。その場合、$K$ の関係 $f(x) \leq u(x)$ は $f(a) \leq b$ を暗示する必要があります。しかし、$u$は$K$上で凸連続であるため、$u(a)$は$E$上の連続アフィン線形写像$f$の$f(a)$の上限に等しく、$K$上の$f(x) \leq u(x)$になります（TVS、 II, §5, No. 4、提案 5);したがって、関係 $b \geq u(a)$ が得られます。最後に、集合 $\lambda = 1$; (4) が (5) を意味すると言うことは、定義によって $b \leq \overline{u}(a)$ を意味します。 関係 (4) (それぞれ (5)) は両辺にスカラー $> 0$ を乗算して得られるものと等しいため、これは補題であることが証明されます。

#### 補題 2 {#int-iv-s7-lem-2 .statement tag=08YU}

*$u$ が厳密に $K$ に凸である場合、$K$ の極値ではないすべての点 $x$ に対して $u(x) < \overline{u}(x)$ になります。*

なぜなら、$u$ は厳密に凸であるため、$x = (y + z)/2$、よって $u(x) < (u(y) + u(z))/2$ など、$K$ の 2 つの異なる点 $y, z$ が存在するからです。 $f$ が $E$ 上のアフィン線形写像である場合、$f(x) = (f(y) + f(z))/2$。 適用この関係を $K$ 上の $\geq u$ である連続アフィン線形写像 $f$ にすると、次のようになります。

$$
\overline{u}(x) \geq (\overline{u}(y) + \overline{u}(z))/2 \geq (u(y) + u(z))/2 > u(x) .
$$

これらの補題が確立されたため、(補題 1) すべての $a \in K$ に対して $(a, \overline{u}(a)) \in S$ が得られます。 $G$ はコンパクトであり、連続写像 $x \mapsto (x, u(x))$ の下で $K$ の像であるため、No. 1 の提案 1 により、総質量 1 の$G$ に対する正の測度 $\nu$ が存在し、次のように $(a, \overline{u}(a))$ を持ちます。重心。 射影 $pr_1$ から $G$ の制限は $K$ への $G$ の準同型写像であるため、測度 $\nu$ はこの準同型写像によって移送され、$K$ に対する測度 $\mu$ が得られます（正）および総質量 1 ) は次のようになります

(6)
$$
a = \int x \, d\mu(x) \quad \text{and} \quad \overline{u}(a) = \int u(x) \, d\mu(x) .
$$

関係 (6) の最初は、$a$ が $\mu$ の重心であることを意味します。 写像 $\overline{u}$ は上部半連続で、$K$ で境界があるため、$\mu$ 積分可能です (§4, No. 4、提案 5 の Cor. 1)。さらに、写像 $-\overline{u}$ は定義によって凸であるため、Cor によって、次のようになります。 No. 1の提案2、

(7)
$$
\overline{u}(a) \geq \int \overline{u}(x) \, d\mu(x) ,
$$

よって、公式 (6) の 2 番目と比較すると、

$$
\int u(\mathbf{x})\, d\mu(\mathbf{x}) \geq \int \overline{u}(\mathbf{x})\, d\mu(\mathbf{x}) .
$$

しかし、K の $u(\mathbf{x}) \leq \overline{u}(\mathbf{x})$ 以来、関係 (8) は、$\mu$ のほぼどこでも $u(\mathbf{x}) = \overline{u}(\mathbf{x})$ であることを意味します。 補題 2 を考慮すると、次の補題が確立されると、定理 1 が証明されることがわかります。

#### 補題 3 {#int-iv-s7-lem-3 .statement tag=08YV}

*E を $\mathbf{R}$ 上の局所的に凸なハウスドルフ空間とし、K を E の計量可能コンパクト凸部分集合とします。すると、K 上に厳密に凸な数値写像が存在します。

なぜなら、Banach 空間 $\mathscr{C}(K; \mathbf{R})$ は分離可能 (GT, X, §3, No. 3, Th. 1) であるため、* E 上の*連続アフィン線形写像の K に対する制限によって形成される $\mathscr{C}(K; \mathbf{R})$ の部分空間 $\mathscr{A}$ も分離可能です。 $(h_n)$ は $\mathscr{A}$ で数列密になり、$\alpha_n > \sup_{\mathbf{x} \in K} |h_n(\mathbf{x})|$ とします。次に、それぞれの写像 $h_n^2 / n^2 \alpha_n^2$ は K に凸であり (TVS、II, §2, No. 8、*例*)、一般的な項 $h_n^2 / n^2 \alpha_n^2$ を伴う系列は通常収束するため、その和 $u$ は連続で K に凸です。 $u$ が厳密に凸であることを確認するには、K の任意の 2 つの異なる点 $\mathbf{x}, \mathbf{x}'$ に対して、端点 $\mathbf{x}, \mathbf{x}'$ を持つセグメントに対する $h_n^2$ の制限が厳密に凸であるような整数 $n$ が存在することを証明すれば十分です。しかし、これについては、$h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$ (*loc. cit.*) で十分です。さて、$h(\mathbf{x}) \neq h(\mathbf{x}')$ (TVS、II, §4, No. 1、提案 2 の Cor. 1) となるような写像 $h \in \mathscr{A}$ が存在し、数列 $(h_n)$ が $\mathscr{A}$ に密集しているため、$h_n(\mathbf{x}) \neq h_n(\mathbf{x}')$ となるような $n$ が存在します。

Q.E.D.

#### 系 {#int-iv-s7-n2-cor-2 .statement tag=08YW}

*E を、$\mathbf{R}$ 上の局所的に凸なハウスドルフ空間とし、C 頂点 0 をもつ E 内の適切な凸円錐、これは E の弱体化された均一構造によって引き起こされる均一構造に対して完全かつ計量化可能です。M を極値の和集合としますC中生成元。すべての $\mathbf{x} \in C$ に対して、C のコンパクトな凸面部分集合 K と、総質量 1 の K 上の測度 $\lambda \geq 0$ が存在し、$K - (M \cap K)$ は $\lambda$ 無視でき、$\lambda$ の重心は $\mathbf{x}$ に等しくなります。

たとえば、$\mathbf{x}$ 属するをC (TVS、II, §7, No. 2、提案 5) の上限 K に、および K の極値点の $M \cap K$ 含む集合 (*上記引用*、提案 4 の Cor. 1)。その後、Th を適用するだけで十分です。 1.

### 3. アプリケーション: I。連続実数のベクトル空間写像

X を空でないコンパクト空間、$\mathscr{H}$ をバナッハ空間 $\mathscr{C}(X; \mathbf{R})$ の線形部分空間とし、含むを定数とし、X の点を *分離* します。 X, §4, No. 1、定義 1)。 $\mathscr{H}$ には、$C(X; \mathbf{R})$ の規範によって誘発された規範空間位相が備わっており、この規範空間の双対を $\mathscr{H}'$ で表します。すべての $x \in X$ について、写像 $f \mapsto f(x)$ は $\mathscr{H}$ で連続する線型形式 (ディラック測度 $\varepsilon_x$ の制限から $\mathscr{H}$) であるため、$\mathscr{H}'$ の元が表されます。 $i_{\mathscr{H}}(x)$、つまり

$$
\langle f, i_{\mathscr{H}}(x) \rangle = f(x)
$$

写像 $f \in \mathscr{H}$ および $x \in X$ ごとに。

$\mathscr{H}'$ に弱い位相 $\sigma(\mathscr{H}', \mathscr{H})$ が装備されている場合、X の $\mathscr{H}'$ への写像 $i_{\mathscr{H}}$ は単射的で連続的です。 2 番目の主張は、定義と (9) からすぐに続きます。最初のものに関しては、$x, x'$ が X の 2 つの異なる点である場合、仮定によって $h(x) \neq h(x')$ となるような写像 $h \in \mathscr{H}$ が存在することに注意してください。したがって、(9)、$\langle h, i_{\mathscr{H}}(x) \rangle \neq \langle h, i_{\mathscr{H}}(x') \rangle$ および *なおさら* $i_{\mathscr{H}}(x) \neq i_{\mathscr{H}}(x')$ によります。 したがって、像 $i_{\mathscr{H}}(X)$ は、$\mathscr{H}'$ (弱い位相の場合) の *コンパクト* 部分集合であり、$i_{\mathscr{H}}$ は、$i_{\mathscr{H}}(X)$ への X の *同相同型* です。

#### 命題 4 {#int-iv-s7-prop-4 .statement tag=08YX}

(i) *閉じた凸型封筒* C *of* $i_{\mathscr{H}}(X)$ *in* $\mathscr{H}'$ *(弱者向け位相* $\sigma(\mathscr{H}', \mathscr{H})$) *コンパクト*。

(ii) *点* $i_{\mathscr{H}}(x)$ *が C の極値点であるためには、 *唯一の肯定的な尺度* $\lambda$ *オン* X *そのような* であることが必要かつ十分です

$$
h(x) = \int h \, d\lambda
$$

*すべての写像* $h \in \mathscr{H}$ (これは、$1 \in \mathscr{H}$ 以降、特に $\lambda$ の総質量が 1 であることを意味します) *ディラック測度* $\varepsilon_x$ となります。

したがって、各 $h \in \mathscr{H}$、C の写像 $z' \mapsto \langle h, z' \rangle$ は、C (TVS、II, §7, No. 1、提案 1) の少なくとも 1 つの極値点で最高値に達し、この点属するは、 $i_{\mathscr{H}}(X)$ (*引用箇所*、提案 2 の補足)。

(i) (9) により、標準的な空間 $\mathscr{H}'$ では $\| i_{\mathscr{H}}(x) \| \leq 1$、その他の語 $i_{\mathscr{H}}(X)$ は制限されており、弱い位相 $\sigma(\mathscr{H}', \mathscr{H})$ を備えた $\mathscr{H}'$ が *準完全* であるという事実から主張が導き出されます。 III, §4, No. 2、コリント 5、1)。

(ii) Every positive measure $\mu$ of mass 1 on $i_{\mathscr{H}}(X)$ arises, by transport of structure by means of the homeomorphism $i_{\mathscr{H}}$, from a positive measure $\lambda$ of mass 1 on X, the Dirac measure $\varepsilon_{i_{\mathscr{H}}(x)}$ arising from $\varepsilon_x$. $\mu$ が $i_{\mathscr{H}}(x)$ を重心として認めるということは、定義によって次のことを意味します。

$$
\int_X \langle h, i_{\mathscr{H}}(z) \rangle \, d\lambda(z) = \langle h, i_{\mathscr{H}}(x) \rangle
$$

写像 $h \in \mathscr{H}$ ごとに。 (9) を考慮すると、主張 (ii) は、No. 2, Cor. $i_{\mathscr{H}}(x)$ が C の極値点になるという提案 3 の。

提案 4 の点 $x \in X$ 満たす条件 (ii) は $\mathscr{H}$ 極値であると言えます。これら点のうち $\mathrm{Ch}_{\mathscr{H}}(X)$ (または単に $\mathrm{Ch}(X)$) 集合で、$X$ の $\mathrm{Ch}_{\mathscr{H}}(X)$ の終結を $\check{S}_{\mathscr{H}}(X)$ (または単に $\check{S}(X)$) で表します。

#### 命題 5 {#int-iv-s7-prop-5 .statement tag=08YY}

*すべての写像* $h \in \mathscr{H}$ *少なくとも 1 つ* $\mathscr{H}$* から極値点* で最高値に達します。

$x$ を $X$ の点、$\mathscr{H}$ の $h$ 写像とします。 すべての $z \in X$ に対する関係 $h(z) \leq h(x)$ は、すべての $z \in X$ に対して $\langle h, i_{\mathscr{H}}(z) \rangle \leq \langle h, i_{\mathscr{H}}(x) \rangle$ と書くことができ、したがって、方程式 $\langle h, t' \rangle = \langle h, i_{\mathscr{H}}(x) \rangle$ で弱く閉じられた $\mathscr{H}'$ の超平面が $i_{\mathscr{H}}(X)$ の *サポート超平面* であることを意味します。 It is known (TVS, II, §7, No. 1, Cor. of Prop. 1) that such a hyperplane contains at least one extremal point of the closed convex envelope of $i_{\mathscr{H}}(X)$, and such a point $i_{\mathscr{H}}(y)$ is the image of an $\mathscr{H}$-extremal point $y$ by definition; $h(y)$ is therefore equal to the supremum of $h$ in $X$.

#### 命題 6 {#int-iv-s7-prop-6 .statement tag=08YZ}

*すべての点* $x \in X$ について、*次のプロパティは同等です*:

a) $x$ *は* $\mathscr{H}$*-極端*。

b) *すべての開いた近隣* $U$ *の* $x$ *in* $X$ *およびすべての* $\varepsilon > 0$、*存在します写像* $h \geq 0$ *in* $\mathscr{H}$ *そのような* $h(x) \leq \varepsilon$ *および* $h(y) \geq 1$ *すべての* $y \in X - U$。

$x$ を、$\mathscr{C}(X; \mathbf{R})$ の $X$、$f$ 写像のいずれかの点とします。既知 (TVS、II, §3, No. 1、提案 1) 写像 $h \in \mathscr{H}$ ごとに $\lambda(h) = h(x)$ となるような $X$ のすべての肯定的な尺度に対する数 $\lambda(f)$ の下限は数の上限に等しい$h(x)$、ここで $h$ は写像 $h \in \mathscr{H}$ の集合を超え、$h \leq f$ になります。 $x$ が $\mathscr{H}$ 極値であると仮定します。次に、提案 4、(ii) 写像 $f \in \mathscr{C}(X; \mathbf{R})$ ごとに、

$$
f(x) = \sup_{h \in \mathscr{H}, h \leq f} h(x).
$$

*a)* が *b)* を意味することを示すために、$f$ に対して、$X$ の連続写像を $[0, 1]$ に取り、$U$ に含まれるサポートを使用して、$f(x) = 1$ とします。すると、(11) により、$h' \leq f$ と $h'(x) \geq 1 - \varepsilon$ となるような写像 $h' \in \mathscr{H}$ が存在します。 $1 \in \mathscr{H}$ なので、写像 $h = 1 - h'$ は *b)* の条件と一致します。

逆に、条件 *b)* が検証されたとします。この条件は $1 - h \leq \varphi_U$ を意味します。したがって、$X$ 満たす条件 (10) のすべての肯定的な測定値 $\lambda$ について、

$$
\lambda(U) = \lambda(\varphi_U) \geq \lambda(1 - h) = 1 - h(x) \geq 1 - \varepsilon.
$$

仮定までに、この関係はすべての $\varepsilon > 0$ と $x$ のすべてのオープン近隣 $U$ に当てはまりますので、次のようになります。

$$
\lambda(\{x\}) = \inf_U \lambda(U) \geq 1 - \varepsilon
$$

$\varepsilon > 0$ ごとに、したがって $\lambda(\{x\}) = 1$ になります。 $\lambda$ は正で総質量 1 であるため、必然的に $\lambda = \varepsilon_x$ となり、提案 4 (ii) により、$x$ が $\mathscr{H}$ 極値であることが証明されます。

#### 命題 7 {#int-iv-s7-prop-7 .statement tag=08Z0}

*F を X の閉じた部分集合とします。次のプロパティは同等です:*

a) *F 含む $\check{S}_{\mathscr{H}}(X)$.*

b) *すべての写像 $h \in \mathscr{H}$ に対して、集合 F は X の点の集合と交差し、h はその最高値に達します。*

c) *すべての点 $x \in X$ に対して、X の総質量 1 の正の尺度 $\mu$ が存在し、写像 $h \in \mathscr{H}$ ごとに $\operatorname{Supp}(\mu) \subset F$ と $h(x) = \int h \, d\mu$ が存在します。*

$G = i_{\mathscr{H}}(F)$ にしましょう。 条件 *a)* は、C の極値点の G 含む集合を意味します。 条件 *b)* は、G が $i_{\mathscr{H}}(X)$ の各クローズドサポート超平面と $i_{\mathscr{H}}(X)$ の共通部分を満たすことを意味します。 最後に、条件 *c)* は、$i_{\mathscr{H}}(X)$ のすべての点が G に含まれるサポートを持つメジャーの重心であることを意味します。 No. 1、提案 1 によると、これは、$i_{\mathscr{H}}(X)$ の閉じた凸包絡線が G の閉じた凸包絡線に等しいというというにも等価です。 The equivalence of the conditions *a)*, *b)* and *c)* therefore follows from TVS, II, §7, No. 1, Cor. of Prop. 2.

#### 命題 8 {#int-iv-s7-prop-8 .statement tag=08Z1}

*X が metrizable であると仮定します。 すると、Xの$\mathscr{H}$-極値点の集合$\operatorname{Ch}_{\mathscr{H}}(X)$は、Xの開集合の可算族の共通部分であり、すべての$x \in X$に対して、総質量1の正の尺度$\mu$が存在します。 X そのような*

$$
\mu(X - \operatorname{Ch}_{\mathscr{H}}(X)) = 0 \quad \text{and} \quad \int h \, d\mu = h(x)
$$

*$h \in \mathscr{H}$ごとに。*

Thさんの訳です。提案 5 のように、同型写像 $x \mapsto i_{\mathscr{H}}(x)$ を使用して、No. 2 の 1 を構造の輸送で生成します。

A certain number of results of this No. may be extended when $\mathscr{H}$ is replaced by a set $\mathscr{P}$ of functions defined on X, with values in $\mathbf{R} \cup \{+\infty\}$, that are lower semi-continuous, $\mathscr{P}$ being assumed to contain the constants and to satisfy $\mathscr{P} + \mathscr{P} \subset \mathscr{P}$ (Exer. 2).

#### 例 {#int-iv-s7-n3-exa-1 .statement tag=08Z2}

— Take X to be the unit ball $\|x\| \leq 1$ in $\mathbf{R}^3$, and let $\mathscr{H}$ be a vector space of continuous functions on X, containing the restrictions to X of the affine linear functions on $\mathbf{R}^3$ and satisfying the *maximum principle*, that is, for every non-constant function $h \in \mathscr{H}$, the set of points of X where h attains its supremum is contained in the sphere $S_2$. 次に、Props から簡単に実行します。 5と7は$\operatorname{Ch}_{\mathscr{H}}(X) = \check{S}_{\mathscr{H}}(X) = S_2$です。 An important example of a vector space $\mathscr{H}$ satisfying the preceding conditions is the set of functions continuous on X and *harmonic* in the open ball $\|x\| < 1$. これらの写像について、$\|x\| < 1$ の場合、すべての $h \in \mathscr{H}$ に対して $\operatorname{Supp}(\mu) \subset S_2$ と $h(x) = \int h \, d\mu$ となるような質量 1 の正の測度 $\mu$ が、ポアソンの公式によって与えられることが証明されます。

$$
d\mu(z) = \frac{1 - \|z\|^2}{\|z - x\|^3} d\sigma(z),
$$

ここで、$\sigma$ は、直交群の下で不変である $S_2$ に関する測度であり、$\sigma(S_2) = 1$ (Ch. VII, §3、Exer. 8)* です。

### 4. アプリケーション: II。 ベクトル空間連続複合体写像

$X$ を空でないコンパクト空間、 $\mathscr{H}$ を複素バナッハ空間 $\mathscr{C}(X; \mathbf{C})$ の線形部分空間とし、含むを定数とし、$X$ の点を分離します。 The set of real parts $\Re(f)$ of the functions $f \in \mathscr{H}$ is a linear subspace $\mathscr{H}_r$ of the real vector space $\mathscr{C}(X; \mathbf{R})$; for every $f \in \mathscr{H}$, the set $\mathscr{H}_r$ also contains $\mathscr{I}(f) = \Re(-if)$; it follows that $\mathscr{H}_r$ separates the points of $X$, because the relation $h(x) = h(y)$ for all $h \in \mathscr{H}_r$ implies that $\Re(f(x)) = \Re(f(y))$ and $\mathscr{I}(f(x)) = \mathscr{I}(f(y))$ and so $f(x) = f(y)$ for all $f \in \mathscr{H}$. $X$ の $\mathscr{H}_r$ 極値点は再び $\mathscr{H}$ 極値と呼ばれ、そのうちの集合は $\mathrm{Ch}_{\mathscr{H}}(X)$ で示され、後者集合の閉包は $\check{S}_{\mathscr{H}}(X)$ で示されます。 Props の類似物。 5と7は以下の通りです。

#### 命題 9 {#int-iv-s7-prop-9 .statement tag=08Z3}

*すべての写像 $f \in \mathscr{H}$ に対して、$\mathrm{Ch}_{\mathscr{H}}(X)$ は点の集合と交差し、$|f|$ が最高値になります。*

$f$ が定数 0 ではない場合に極限を当てはめることができます。$a$ を、$|f|$ が最高値に達する$X$ の点とし、集合 $g = f/f(a)$ とします。次に、$x \in X$、よってに対して $g(a) = 1$ と $|g(x)| \leq 1$

$$
\Re(g(a)) = 1 \quad \text{and} \quad \Re(g(x)) \leq 1 \quad \text{for all } x \in X.
$$

No. 3 の提案 5 を$\mathscr{H}_r$ に適用すると、$\Re((g(x))$ がその最高値 1 に達する$b \in \mathrm{Ch}_{\mathscr{H}}(X)$ が存在し、$|g(b)| \leq 1$ からよって $|g(b)| = 1$ が存在します。つまり、すべての $x \in X$ に対して $|f(b)| = |(f(a)| \geq |f(x)|$ ということになります。

#### 命題 10 {#int-iv-s7-prop-10 .statement tag=08Z4}

*$F$を$X$の閉じた部分集合とします。次のプロパティは同等です。
a) $F$ 含む $\check{S}_{\mathscr{H}}(X)$。
b) 写像 $f \in \mathscr{H}$ ごとに、$F$ は $X$ の点の集合と交差し、$|f|$ がその最高点に達します。
c) 点 $x \in X$ ごとに、$X$ の総質量 1 の正の尺度 $\mu$ が存在し、写像 $f \in \mathscr{H}$ ごとに $\mathrm{Supp}(\mu) \subset F$ と $f(x) = \int f d\mu$ が存在します。
条件 a) と c) の同値を証明してみましょう: $f = f_1 + i f_2$ を $\mathscr{H}_r$ で $f_1, f_2$ とします。 関係 $f(x) = \int f d\mu$ は 2 つの関係 $f_1(x) = \int f_1 d\mu$ と $f_2(x) = \int f_2 d\mu$ に相当します。したがって、No. 3 の提案 7 の条件 a) および c) に$\mathscr{H}_r$ 同値を適用するだけで十分です。 a) が b) を意味するという事実は、提案 9 から導かれます。b) が a) を意味することを示しましょう。これは、b) が検証された場合、$h \in \mathscr{H}_r$ ごとに、F が点の集合と交差し、$h$ が X で下限に達することを確認することです。 条件 b) F が空でないであることを意味します。 F はコンパクトなので、すべての $y \in F$ に対して $h(a) \leq h(y)$ となるような $a \in F$ が存在します。 $f \in \mathscr{H}$ を $h = \mathscr{R}(f)$ となるようにします。 $\varepsilon > 0$、写像 $g = f - h(a) + \varepsilon$ 属するから $\mathscr{H}$ ごと、および
$$
\mathscr{R}(g(y)) = h(y) - h(a) + \varepsilon \geq \varepsilon
$$
$y \in F$ 全員のために。 $c$ を X の $|g|$ と集合 $b = c^2 / 2\varepsilon$ の上限とします。 $y \in F$ごとに、
$$
|g(y) - b|^2 = |g(y)|^2 - 2b \mathscr{R}((g(y))) + b^2 \leq c^2 - 2b\varepsilon + b^2 = b^2,
$$
他の語では、写像 $|g - b|$ の F の最高値は $\leq b$ です。 F の $g - b \in \mathscr{H}$、仮定は、$|g - b| \leq b$、よってを意味します。
$$
b^2 \geq |g - b|^2 = |g|^2 - 2b \mathscr{R}(g) + b^2
$$
それで $\mathscr{R}(g) \geq |g|^2 / 2b \geq 0$; $\mathscr{R}(g) = h - h(a) + \varepsilon$、$\varepsilon > 0$ は任意なので、$h \geq h(a)$ があり、$h(a)$ はX の$h$ の下限であり、証明が完成します。

#### 注意 {#int-iv-s7-n4-rem-1 .statement tag=08Z5}

$f$ が連続実数写像である場合、$|f|$ が最高値に達する点は、写像 $f, -f$ のいずれかが最高値に達する点です。連続実数写像満たすのベクトル空間 $\mathscr{H}$ について、No. 3 の仮説、Props。したがって、9 と 10 は Props の自明な帰結です。それぞれ5と7。

### 5. アプリケーション: III。 代数の連続写像

#### 補題 4 {#int-iv-s7-lem-4 .statement tag=08Z6}

X をコンパクト空間、$\mathscr{H}$ をバナッハ空間 $\mathscr{C}(X; \mathbf{C})$ (それぞれ $\mathscr{C}(X; \mathbf{R})$) の閉じた線形部分空間とします。 a を近傍の可算基本系を認める X の点とします。 $0 < c < d < 1$ となるような任意の数 c と d および a の任意の開いた近傍 U に対して、次のような $f \in \mathscr{H}$ が存在すると仮定します。
$$
|f| \leq 1,\quad |f(a)| \geq d,\quad |f(x)| \leq c \text{ for all } x \in X - U.
$$
次に、すべての $x \neq a$ に対して $|u(x)| < |u(a)|$ となるような写像 $u \in \mathscr{H}$ が存在します。

$(V_n)$ ($n \geq 1$) を $a$ の近傍の基本系とし、$\lambda, \mu, \varepsilon$ を次のような数とします。
$$
0 < \lambda < 1,\quad 1 < \mu < \mu + \varepsilon \leq 1 + \lambda.
$$
したがって$0 < \lambda / \mu < 1 / \mu < 1$。 $n$ ($n \geq 1$) の帰納法までに $a$ のオープンネイバーフッドの減少列 $(U_n)$ までに定義するに行き、すべての $n$ に対して$U_n \subset V_n$、そして数列 $\mathscr{H}$ 満たす関係の写像の $(h_n)$
$$
\begin{align*}
(13_n) &\quad |h_n(x)| \leq \mu \quad \text{for all } x \in X \\
(14_n) &\quad h_n(a) = 1 \\
(15_n) &\quad |h_n(x)| \leq \lambda \quad \text{for all } x \in X - U_n \\
(16_n) &\quad \left| \sum_{j=1}^n \lambda^j h_j(y) \right| < \sum_{j=1}^{n+1} \lambda^j \quad \text{for all } y \in X.
\end{align*}
$$
条件の前の 4 つである $1 \leq m < n$、満たすに対して $h_m$ と $U_m$ が定義されているとします ($n$ は $m$ に置き換えられます)。一方、集合 $U_0 = X$。
写像 $\sum_{j=1}^{n-1} \lambda^j h_j$ ($n = 1$ の場合は 0 に等しい) は連続であり、点 $a$ で値 $\sum_{j=1}^{n-1} \lambda^j$ かかります。したがって、$U_{n-1} \cap V_n$ に含まれる、$a$ の開いた近傍 $U_n$ が存在します。
$$
\left| \sum_{j=1}^{n-1} \lambda^j h_j(y) \right| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n \quad \text{for all } y \in U_n.
$$
仮定までに、次のような写像 $f \in \mathscr{H}$ が存在します。
$$
\begin{align*}
|f(x)| &\leq 1 \quad \text{for all } x \in X , \quad |f(a)| \geq 1 / \mu , \\
|f(x)| &\leq \lambda / \mu \quad \text{for } x \in X - U_n .
\end{align*}
$$
集合 $h_n = f / f(a)$; 関係 $(13_n)$、$(14_n)$、$(15_n)$ を押し続けます。 集合
$$
g = \sum_{j=1}^n \lambda^j h_j = \sum_{j=1}^{n-1} \lambda^j h_j + \lambda^n h_n .
$$
(17) と $(13_n)$ により、$y \in U_n$ は次のようになります。
$$
|g(y)| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n + \mu \lambda^n \leq \sum_{j=1}^{n+1} \lambda^j ,
$$

$\varepsilon + \mu \leq 1 + \lambda$以来。 $x \in X - U_n$には$|h_p(x)| \leq \lambda$、$1 \leq p \leq n$にはよってもございます
$$
|g(x)| \leq \sum_{j=2}^{n+1} \lambda^j < \sum_{j=1}^{n+1} \lambda^j,
$$
これで$(16_n)$の証明が完了します。

そうなると、系列 $\sum_{n=1}^{\infty} \lambda^n h_n$ は、すべての $n$ とすべての $x \in X$ について、$\lambda < 1$ と $|h_n(x)| \leq \mu$ 以来、通常は $X$ に収束します。 $u$ をその和とします。$\mathscr{H}$ が閉まっているため、属するから $\mathscr{H}$ になります。 関係 $(14_n)$ までに、$u(a) = \sum_{n=1}^{\infty} \lambda^n$ になります。一方、$x \neq a$ の場合、$x \notin U_{n+1}$ となるような整数 $n$ が存在します。したがって、関係 $(15_n)$ によるすべての $k \geq 1$ に対して $|h_{n+k}(x)| \leq \lambda$ です。 $(16_n)$ を使用すると、次のようになります。
$$
|u(x)| \leq \left| \sum_{j=1}^n \lambda^j h_j(x) \right| + \left| \sum_{j=n+1}^{\infty} \lambda^j h_j(x) \right| < \sum_{j=1}^{n+1} \lambda^j + \lambda \sum_{j=n+1}^{\infty} \lambda^j
$$
$$
= \sum_{j=1}^{\infty} \lambda^j = |u(a)|.
$$

#### 定理 2 (E. ビショップ) {#int-iv-s7-thm-2 .statement tag=08Z7}

— *$X$ を複素バナハ代数 $\mathscr{C}(X; \mathbf{C})$ のコンパクト空間、$\mathscr{A}$ を閉じた部分代数とします。 $\mathscr{A}$ 含むが定数であり、$X$ の点を区切るものとします。 $a$ を $X$ の点とします。次の条件は同等です。

a) すべての $x \neq a$ に対して $|f(x)| < |f(a)|$ となるような写像 $f \in \mathscr{A}$ が存在します。

b) 点 $a$ は $\mathscr{A}$ 極値であり、近傍の可算基本系を認めます。

a) $\Rightarrow$ b): $f \in \mathscr{A}$ を $x \neq a$ に対して $|f(a)| > |f(x)|$ となるようにします。 No. 4 の提案 9 により、$a$ は $\mathscr{A}$ の極値点です。一方、$U_n$ が $|f(x)| > |f(a)| - 1/n$ となるような $x \in X$ の集合である場合、$U_n$ は $a$ の開いた近傍であり、$U_n$ 簡約するから $a$ の共通部分です。 $X$ はコンパクトなので、$U_n$ 形は $a$ (GT、I, §9, No. 1、Th. 1) の近傍の基本的な系です。

b) $\Rightarrow$ a): b) が補題 4 の仮説を暗示していることを検証するだけで十分です。 補題のうち記法で、集合 $\varepsilon = \log d / \log c$。したがって、$0 < \varepsilon < 1$。 $a$ は $\mathscr{A}_r$ 極値点であるため、次のような写像 $g \in \mathscr{A}$ が存在します。
$$
\mathscr{R}(g) \geq 0,\quad \mathscr{R}(g(a)) \leq \varepsilon,\quad \mathscr{R}(g(x)) \geq 1 \text{ for } x \in X - U
$$

(No. 3、提案 6、b))。 集合 $f = c^g$; $f$ は通常収束する系列 $\sum_{n=0}^{\infty} (\log c)^n g^n / n!$ の和であるため、 $f \in \mathscr{A}$ があり、

$$
|f| \leq 1,\quad |f(a)| \geq c^{\varepsilon} = d,\quad |f(x)| \leq c \text{ for } x \in X - U.
$$

Q.E.D.

#### 系 {#int-iv-s7-n5-cor-1 .statement tag=08Z8}

— *加法で $X$ が metrizable であると仮定します。したがって、次のプロパティは同等です*。

a) *$a$は、$X$*の$\mathscr{A}$極値点です。

b) *すべての$x \neq a$*に対して$|u(x)| < |u(a)|$となるような$u \in \mathscr{A}$が存在します。

c) *$\mathfrak{M}$ を部分集合の $M$ $X$ の集合とし、写像 $f \in \mathscr{A}$ ごとに、$|f|$ が $X$ の少なくとも 1 つの点で最高値に達するようにします。 $M$。次に、$a$ 属するから集合 $M \in \mathfrak{M}$* までです。

d) *$\mathfrak{N}$を、部分集合の$N$、$X$の集合とし、写像$f \in \mathscr{A}$ごとに、$\mathscr{R}(f)$が少なくとも1つの点で$X$で最高値に達するようにします。 $N$の。次に、$a$ 属するから集合 $N \in \mathfrak{N}$* までです。

*その他語*では、

$$
\mathrm{Ch}_{\mathscr{A}}(X) = \bigcap_{M \in \mathfrak{M}} M = \bigcap_{N \in \mathfrak{N}} N.
$$

計数可能な空間では、すべての点が近傍の可算基本系を許容するため、a) と b) の同値は Th から続きます。 2. b) が c) を意味することを示しましょう。実際、$a$ は、$|u|$ が最高値となる一意の点です。一方、c) は a) を意味します。なぜなら、$f \in \mathscr{A}$ ごとに、$\mathrm{Ch}_{\mathscr{A}}(X)$ が点の集合と交差し、$|f|$ がその最高値に達するからです (No. 4、提案 9)。同じ推論は、No. 3 の提案 5 を使用して、d) が a) を意味することを示しています。最後に、b) が d) を意味することを確認するには、$X$ が単一の点 $a$ に簡約するしない場合に限定することができ、したがって $u(a) \neq 0$ になります。 写像 $v = u/u(a)$ 次に、属するから $\mathscr{A}$ となり、$x \neq a$ には $v(a) = 1$ と $|v(x)| < 1$、$x \neq a$ にはよって $\mathscr{R}(v(a)) = 1$ と $\mathscr{R}(v(x)) < 1$ があります。 写像 $\mathscr{R}(v)$ は点 $a$ でのみ最高値に達するため、$N \in \mathfrak{N}$ ごとに実際に $a \in N$ が得られます。

#### 例 {#int-iv-s7-n5-exa-1 .statement tag=08Z9}

— $X_1$ を $|z_1|^2 + |z_2|^2 \leq 1$ (単位元ボールイン $\mathbf{R}^4$) となるような点 $(z_1, z_2) \in \mathbf{C}^2$ の集合とし、$\mathscr{A}_1'$ を正則写像の制限から $X_1$ の集合とする写像、$\mathbf{C}$の値は、$\mathbf{C}^2$の$X_1$の近傍で定義されます（写像に依存する近傍が考慮されます）。 $\mathscr{A}_1$を$\mathscr{C}(X_1; \mathbf{C})$における$\mathscr{A}_1'$の閉包とします。これは明らかに$\mathscr{C}(X_1; \mathbf{C})$の閉じた複合体部分代数であり、$X_1$の点を分離します。正則写像に「最大原理」を適用すると、$\mathrm{Ch}_{\mathscr{A}_1}(X_1)$ が球 $S_3$ であることがわかります。

前の定義で、関係 $|z_1| \leq 1$ と $|z_2| \leq 1$ によって定義される「ポリディスク」$X_2$ によって置き換える $X_1$ を計算すると、部分代数 $\mathscr{A}_2'$ と $\mathscr{A}_2$ (次の$\mathscr{A}_2'$ の閉包) が得られます。 $\mathscr{C}(X_2; \mathbf{C})$。 ここで、最大原理は、$\mathrm{Ch}_{\mathscr{A}_2}(X_2)$ が関係 $|z_1| = 1$ と $|z_2| = 1$ によって定義される 'トーラス' であることを示しています。

これらの結果から、$X_1$ の開いた近傍から $X_2$ の開いた近傍への *変換* $X_1$ *into* $X_2$ への *分析的な同型* は存在しないと推測されます。なぜなら、もし $v$ がそのような写像の制限から $X_1$ だったら、 $\mathscr{A}_2 = v \mathscr{A}_1 v^{-1}$ があり、したがって $v$ は変換 $S_3$ から $T^2$ と同型の空間になるからです。 $S_3$ は単純に接続されていますが、$T^2$ は接続されていません。しかし、空間 $X_1$ と $X_2$ は *同相* であり、どちらも $\mathbf{R}^4$ の凸型集合と空でないの内部* が有界であることがわかります。

### 6. 積分表現の一意性

E を局所的に凸なハウスドルフの弱い空間 (TVS、II, §6, No. 2)、E の適切な尖った凸円錐 C とします。 C は、位数関係に対して E の元 $\geqslant 0$ の集合であることがわかります。 E のベクトル空間構造。 C が格子順序であると言われるとき、当然理解される E のC に位数が誘導されます。

#### 補題 5 {#int-iv-s7-lem-5 .statement tag=08ZA}

※Cは弱完了であると仮定します。 $\mathscr{A}$ を E 上の連続線型形式の制限から C の集合とする。 $(f_\lambda)_{\lambda \in \Lambda}$ を $\mathscr{A}$ と $f = \sup(f_\lambda)$ の元の有限族とする。 $x \in C$、定義する*ごとに

$$
\overline{f}(x) = \sup \left( f(x_1) + f(x_2) + \cdots + f(x_n) \right),
$$

*supremum は数列の集合 $S_x$ $(x_1, x_2, \ldots, x_n)$ の元 C のように $x_1 + x_2 + \cdots + x_n = x$ のように引き継がれます。 $\mathrm{Card}\, \Lambda = p$ にしましょう。 そして、$\overline{f}(x) = f(y_1) + \cdots + f(y_p)$となるような$(y_1, \ldots, y_p) \in S_x$が存在します。

ファミリ $(f_\lambda)$ の $f_1, f_2, \ldots, f_p$ 元で表します。 $k = 1, 2, \ldots, p$ の場合、$C_k$ を $y \in C$ の集合とします。

$$
f_1(y) < f(y),\ f_2(y) < f(y),\ \ldots,\ f_{k-1}(y) < f(y),\ f_k(y) = f(y).
$$

$C_k$ は、和集合 C を備えた互いに素の凸円錐です。 C の $x_1, x_2, \ldots, x_n$ が $x_1 + x_2 + \cdots + x_n = x$ となるようにします。 $y_k$ を属するから $C_k$ までの $x_i$ の和とします。次に$y_1 + y_2 + \cdots + y_p = x$。 $f$は$C_k$、$f(y_1) + \cdots + f(y_p) = f(x_1) + \cdots + f(x_n)$にアフィンであるため。したがって

$$
f(x) = \sup \left( f(y_1) + \cdots + f(y_p) \right),
$$

ここで、$(y_1, y_2, \ldots, y_p)$ は、$y_1 + y_2 + \cdots + y_p = x$ のように、$p$ の数列点の C の集合を超えます。 集合 $D = C \cap (x - C)$。 Since D is compact (TVS, II, §6, No. 8, Cor. 2 of Prop. 11), so is the set of elements $(y_1, \ldots, y_p)$ of $D^p$ such that $y_1 + \cdots + y_p = x$, thus the supremum (19) is attained.

#### 補題 6 {#int-iv-s7-lem-6 .statement tag=08ZB}

仮説と補題 5 の記法を維持し、$f_\lambda$ が正であると仮定します。 写像 $\overline{f}$ は正に均質で、$C$ では凹型で上部の半連続です。 $C$ が格子順序であればアフィンです。

$\overline{f}$ が確実に均一であることは明らかです。 $x, y$ 属するを $C$ にします。 $C$ の $x_1, \ldots, x_m, y_1, \ldots, y_n$ が $x_1 + \cdots + x_m = x,\ y_1 + \cdots + y_n = y$ となる場合、$x_1 + \cdots + x_m + y_1 + \cdots + y_n = x + y$ となるため、

$$
f(x_1) + \cdots + f(x_m) + f(y_1) + \cdots + f(y_n) \leq \overline{f}(x + y);
$$

$\overline{f}(x) + \overline{f}(y) \leq \overline{f}(x + y)$ であるため、$\overline{f}$ は凹面になります。 $L$ (それぞれ $L_\lambda$) を、$x \in C$ と $0 \leq t \leq \overline{f}(x)$ (それぞれ $0 \leq t \leq f_\lambda(x)$) となるように、$(t, x) \in \mathbf{R} \times E$ の集合とします。それぞれの $L_\lambda$ は弱く完全な固有の凸円錐 $\mathbf{R}_+ \times C$ で閉じられているため、 和 $\sum_{\lambda \in \Lambda} L_\lambda$ は閉じています (TVS、II, §6, No. 8、提案 11 の Cor. 2)。 補題 5 までに、この和は $L$ に等しくなります。したがって、$L$は閉じており、$\overline{f}$が上半連続であることが証明されます。最後に、$C$ が格子順序であると仮定し、$\overline{f}$ が凸であることを証明しましょう。 $x, y$ 属するを $C$ とし、$\varepsilon > 0$ とします。 $C$には$f(z_1) + \cdots + f(z_n) \geq \overline{f}(x + y) - \varepsilon$と$z_1 + \cdots + z_n = x + y$のような$z_1, z_2, \ldots, z_n$が存在します。 ベクトル空間 $C - C$ は、$E$ の格子順序によって誘起された位数の格子順序です (A、VI, §1, No. 9、提案 8)。 分解定理 (*loc. cit.*, No. 10, Th. 1) までに、$C$ には次のような $x_1, \ldots, x_n, y_1, \ldots, y_n$ が存在します。

$$
x_1 + y_1 = z_1,\ \ldots,\ x_n + y_n = z_n,\ x_1 + \cdots + x_n = x,\ y_1 + \cdots + y_n = y.
$$

すると、$f$ は正に均一で凸なので、

$$
\begin{align*}
\overline{f}(x + y) &\leq \varepsilon + f(z_1) + \cdots + f(z_n) \\
&\leq \varepsilon + f(x_1) + f(y_1) + \cdots + f(x_n) + f(y_n) \\
&\leq \varepsilon + \overline{f}(x) + \overline{f}(y).
\end{align*}
$$

$\varepsilon$ は任意の数 $> 0$ であるため、$\overline{f}$ が実際に凸であることが証明されました。

#### 定理 3 (チョケ) {#int-iv-s7-thm-3 .statement tag=08ZC}

*$E$ を、$C$、$K$ の極値生成元の$E$、$G$ 和集合の頂点 0 を持つ弱く完全な固有の凸円錐であるハウスドルフ弱い局所凸空間、$C$ とします。 $C$、$\lambda$、$\lambda'$ の凸部分集合は、$K$ 上の質量 1 の正の測度であり、$\lambda^*(K - (K \cap G)) = {\lambda'}^*(K - (K \cap G)) = 0$ などの同じ重心を認めます。 $C$ が格子順序であると仮定します。次に、$C$、$\lambda^*(f|K) = {\lambda'}^*(f|K)$ 上の半連続で正に均質な凸面ごとに、写像 $f \geq 0$ となります。*

$\mathscr{A}$ (それぞれ $\mathscr{A}'$) を、$E$ 上の連続線型形式 (それぞれアフィン写像) の制限から $C$ の集合とします。私たちは (TVS、II, §5, No. 4、注意 2)、$f$ が $\leq f$ である $\mathscr{A}$ の元の集合の上部エンベロープであることを知っています。 形 $\sup(f_1, \ldots, f_p)$ の写像の集合は、$f_1, \ldots, f_p$ 属するから $\mathscr{A}$、$f_1 \geq 0, \ldots, f_p \geq 0$ は増加する有向集合であり、その上部エンベロープとして $f$ があります。 §1, No. 1 を考慮すると、Th. 1、$f$ が前の形のものである場合、等式 $\lambda(f|K) = \lambda'(f|K)$ を検証すれば十分です。

補題のように定義する $\overline{f}$ 5. $y \in G$ であれば $\overline{f}(y) = f(y)$ であることは明らかです。 $\lambda^*(K - (K \cap G)) = 0$ なので、$\lambda(f|K) = \lambda(\overline{f}|K)$ になります。 補題 6 までに、$\overline{f}$ はアフィンで上部半連続になります。したがって、$\overline{f}|K$ は、K に対する $\mathscr{A}'$ の元の制限の減少する有向集合の下側エンベロープです (TVS、II, §5, No. 4、提案 6)。 $x \in K$を$\lambda$の重心とします。 $g \in \mathscr{A}$なら$\lambda(g|K) = g(x)$。したがって、$\lambda(\overline{f}|K) = \overline{f}(x)$ (§ 4, No. 4、提案 5 の Cor. 2)。したがって、$\lambda(f|K) = \overline{f}(x)$、そして$\lambda'(f|K) = \overline{f}(x)$も同様にわかります。

#### 系 {#int-iv-s7-n6-cor-1 .statement tag=08ZD}

*Eをハウスドルフの局所凸型空間、CをEの頂点0を持つ適切な凸円錐とし、コンパクトソールMを認め、GをCの極値生成元の和集合とする。 $x \in M$ にしましょう。 C が格子順序である場合、$\lambda^*(M - (G \cap M)) = 0$ など、M 上の質量 1 の正の測度 $\lambda$ が最大 1 つ存在し、x を重心として認めます。*

E の置き換えること位相が弱化された位相 (M の変更位相ではない) によって、E は弱い空間であると仮定できます。 $\lambda$ と $\lambda'$ を、指定された特性を持つ M 上の 2 つの測定値とし、h を、方程式 $h(x) = 1$ により M が C と超平面の共通部分となるような E 上の連続的な線型形式とします。 $\mathscr{S}$ を、C 上の正に均質で連続した凸型写像 $\geq 0$ の M に対する $\mathscr{C}(M)$ からなるの制限の部分集合とします。錐体 C は弱く完全です (TVS、II, §7, No. 3)。 Thさんより3、$f \in \mathscr{S}$ごとに$\lambda(f) = \lambda'(f)$。

$f_1, f_2, f_3, f_4$ 属するから $\mathscr{S}$ の場合、
$$
\begin{align*}
\sup(f_1 - f_2, f_3 - f_4) &= \sup(f_1 + f_4, f_3 + f_2) - (f_2 + f_4) \in \mathscr{S} - \mathscr{S} \\
\inf(f_1 - f_2, f_3 - f_4) &= -\sup(f_2 - f_1, f_4 - f_3) \in \mathscr{S} - \mathscr{S}.
\end{align*}
$$
$h|M \in \mathscr{S}$、$\mathscr{S} - \mathscr{S}$ 含むから、定数写像になります。 x と y が M の 2 つの異なる点である場合、x と y を分離する連続する線型形式が E 上に存在し、この形は、C で正である 2 つの連続する線型形式の差です (TVS、II, §6, No. 8、補題 1)。上記のことから、実際の $\alpha, \beta$ に対して、$f(x) = \alpha, f(y) = \beta$ となるような $f \in \mathscr{S} - \mathscr{S}$ が存在することがわかります。この場合、$\mathscr{S} - \mathscr{S}$ は一様収束の位相に対して $\mathscr{C}(M)$ 内で密になります (GT、X, §4, No. 1、提案 2 の補正)。 $\mathscr{S} - \mathscr{S}$の$\lambda$と$\lambda'$一致するなので、$\lambda = \lambda'$になります。

練習問題

### 練習問題 {#int-iv-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
