---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 1
section_title: Construction of a Haar measure
lang: ja
source: int-vii-ix
pdf_pages: 0007-0032, 0084-0093
extraction: ocr
subsections:
    - "no": 1
      title: Definitions and notations
      page: 0
      pdf_page: 7
    - "no": 2
      title: The existence and uniqueness theorem
      page: 6
      pdf_page: 12
    - "no": 3
      title: Modulus
      page: 10
      pdf_page: 16
    - "no": 4
      title: Modulus of an automorphism
      page: 13
      pdf_page: 19
    - "no": 5
      title: Haar measure of a product
      page: 14
      pdf_page: 20
    - "no": 6
      title: Haar measure of an inverse limit*
      page: 15
      pdf_page: 21
    - "no": 7
      title: Local definition of a Haar measure
      page: 18
      pdf_page: 24
    - "no": 8
      title: Relatively invariant measures
      page: 19
      pdf_page: 25
    - "no": 9
      title: Quasi-invariant measures
      page: 20
      pdf_page: 26
    - "no": 10
      title: Locally compact fields
      page: 21
      pdf_page: 27
    - "no": 11
      title: Finite-dimensional algebras over a locally compact field
      page: 25
      pdf_page: 31
statements: 42
exercises: 30
content_sha256: f969fec965a30042c581af20e62f88f67d934845f153f62b5ecf132092324b7b
translated_from: content/en/int/VII/01_s1_construction_of_a_haar_measure.md
translation_method: google
source_content_sha256: e46166486e36efa944d66af30ebaacb93e9bc8f019659598c1d03449537e5e11
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 9108dbe4829157586353a57a1e0f56c10925bad80bc4e54ffdfa934e81d1c713
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。ハール単位の構成

### 1. 定義と記法

G を、局所的にコンパクトな空間 X 内で左側 (GT、III, §2, No. 4) で連続的に動作するトポロジカル群とします。 $s \in G$ と $x \in X$ について、$sx$ を $x$ の変換 $s$ とします。 $\gamma_X(s)$ または $\gamma(s)$ で、次のように定義される X の X への同写写像を表します。

(1)
$$
\gamma(s)x = sx.
$$

私たちは持っています

(2)
$$
\gamma(st) = \gamma(s)\gamma(t).
$$

$f$ が $X$ に定義された写像である場合、$\gamma(s)f$ は構造の輸送、つまり公式 $(\gamma(s)f)(\gamma(s)x) = f(x)$ によって定義されます。他の語では、

(3)
$$
(\gamma(s)f)(x) = f(s^{-1}x).
$$

$\mu$ が $X$ に定義されたメジャーである場合、$\gamma(s)\mu$ は構造の輸送によっても定義され、次のようになります。

(4)
$$
\langle f, \gamma(s)\mu \rangle = \langle \gamma(s^{-1})f, \mu \rangle \quad \text{for } f \in \mathscr{K}(X).
$$

その他語では、

(5)
$$
\int_X f(x) d(\gamma(s)\mu)(x) = \int_X f(sx) d\mu(x).
$$

$A$ が $(\gamma(s)\mu)$ 積分可能集合である場合、$s^{-1}A$ は $\mu$ 積分可能であり、

(6)
$$
(\gamma(s)\mu)(A) = \mu(s^{-1}A).
$$

$\gamma(s)\mu$ という尺度は、$\gamma(s)$ の下の $\mu$ の *像* として定義されることもあります。

$d(\gamma(s)\mu)(x)$ と書く代わりに、ときどき $d\mu(s^{-1}x)$ と書くと便利です。 公式 (5) は次の形を受け取ります。

$$
\int_X f(x) d\mu(s^{-1}x) = \int_X f(sx) d\mu(x);
$$

次に、右側の式は、「置き換えること $x$ by $sx$」によって左側の式から推定できます。

#### 定義 1 {#int-vii-s1-def-1 .statement tag=09CY}

*$\mu$を$X$のメジャーとします。*
a) $\mu$ *は、$\gamma(s)\mu = \mu$ *すべての* $s \in G$ であれば、$G$* の下で不変であると言われます。
b) $\mu$ *は、$\gamma(s)\mu$ *が $\mu$ *すべての* $s \in G$ に比例する*場合、$G$* では比較的不変であると言われます。
c) $\mu$ *は、$\gamma(s)\mu$ *が $\mu$ *すべての* $s \in G$ と等しい場合、 $G$* の下で準不変であると言われます。

#### 注意 {#int-vii-s1-n1-rem-1 .statement tag=09CZ}

— 1) $\mu$ が不変であると仮定します。この場合、$|\mu|$、$\mathscr{R}(\mu)$、$\mathscr{I}(\mu)$ は不変です。 $\mu$ が実数の場合、$\mu^+$ と $\mu^-$ は不変です。
2) $\mu$ が比較的不変であり、非零と仮定します。 $s \in G$ ごとに、次のような固有の複素数 $\chi(s)$ が存在します。

(7)
$$
\gamma(s)\mu = \chi(s)^{-1}\mu,
$$

そして、$G$の写像$\chi$は、$\mathbf{C}^*$の$G$の表現であり、$\mu$の*乗数*と呼ばれます。 公式 (5) すると、次のようになります。

$$
(8) \quad \int_X f(sx)\, d\mu(x) = \chi(s)^{-1} \int_X f(x)\, d\mu(x),
$$

そして公式 (6) は次のようになります。

$$
(9) \quad \mu(sA) = \chi(s) \mu(A).
$$

上記の規則に従って、(7) は次のように書くこともできます。

$$
(10) \quad d\mu(sx) = \chi(s)\, d\mu(x).
$$

3) $|\gamma(s)\mu| = \gamma(s)(|\mu|)$ なので、$\mu$ が準不変であると言うのは、$|\mu|$ が準不変であるというというに相当します。

$\mu$ が準不変で、$\mu'$ が $\mu$ に等しい $X$ の他のである場合、$\gamma(s)\mu'$ は $\gamma(s)\mu$ に相当し、したがって $\mu$、したがって $\mu'$ に相当します。 $\mu'$ は準不変です。したがって、$\mu$ が $G$ の下で準不変であるということは、$\mu$ の *類* が $G$ の下で不変であることを意味します。

$\mu$ が準不変であるためには、$X$ の局所的な $\mu$ のうち無視できる部分集合の集合が $G$ (Ch. V, §5, No. 5、Th. 2) の下で不変であること、または再び、すべての$\mu$-無視できるコンパクト部分集合 $K$ の $X$ と、すべての $s \in G$、$sK$ は $\mu$-無視可能になります (*loc. cit.*、*注意*)。

$\mu$ が準不変である場合、$\mu$ のサポートは $G$ の下で不変です。特に、$G$ が $X$ (A、I, §5, No. 5、定義 6) の *推移的* である場合、このサポートは空 ($\mu = 0$ の場合) または $X$ ($\mu \neq 0$ の場合) のいずれかになります。

#### 補題 1 {#int-vii-s1-lem-1 .statement tag=09D0}

— *$X, Y, Z$ を 3 つのトポロジー 空間とし、$Y$ を局所的にコンパクトにします。 $(x, y) \mapsto xy$ を $X \times Y$ の $Z$ への連続写像とし、$X$ の定義する写像 $x \mapsto u_x$ を関係 $u_x(y) = xy$ で $\mathscr{F}(Y; Z)$ にします。 $f$ を $\mathbf{R}$ の値またはバナッハ空間での$Z$ の連続写像とし、S を$f$ のサポート、$\mu$ を$Y$ の小節とします。 すべての $x_0 \in X$ について、$X$ の $x_0$ の近傍 $V$ が存在し、$\bigcup_{x \in V} u_x^{-1}(S)$ が $Y$ で比較的コンパクトになると仮定します。 次に:
a) $x \in X$ ごとに、$f \circ u_x$ は$Y$ で連続し、コンパクトなサポートが付きます。
b) a) で定義される写像 $x \mapsto \int_Y f(xy)\, d\mu(y)$ は、$X$ で連続します。

主張 a) は明らかです。 b)を証明しましょう。連続性はローカルな性質なので、$\bigcup_{x \in X} u_x^{-1}(S)$が$Y$のコンパクトな部分集合$Y'$に含まれる場合には簡約するとなります。 写像 $(x, y) \mapsto f(xy)$ は $X \times Y$ で連続しているため、 $x$ が $x_0$ になる傾向があるのと同様に、 $f \circ u_x$ は $Y'$ で一律に $f \circ u_{x_0}$ になる傾向があります。

(GT、X, §3, No. 4、Th. 3) したがって、$\mu(f \circ u_x)$ は $\mu(f \circ u_{x_0})$ になる傾向があります。 よって補題。

先ほどの記法に戻りましょう。

#### 命題 1 {#int-vii-s1-prop-1 .statement tag=09D1}

— *G が局所的にコンパクトであると仮定します。 $\mu$ を X に関して比較的不変な測度非零とします。次に、その乗数 $\chi$ は G 上で連続する写像です。*

$f \in \mathscr{K}(X)$, S を G の $f$, $s_0$ 点のサポート、および G の $s_0$ のコンパクトな近傍を V とします。それでは、集合

$$
\bigcup_{s \in V} \gamma(s)^{-1}(S) = V^{-1}S
$$

Xでコンパクトです。 補題 1 と公式 (8) により、$\chi(s^{-1}) \langle \mu, f \rangle$ は継続的に $s$ に依存します。 $\langle \mu, f \rangle \neq 0$ となるように $f$ が選択された場合、$\chi$ が連続であることがわかります。

ここで、G を局所的にコンパクトな空間 X 内で右側で連続的に動作するトポロジー 群とします。 $s \in G$ と $x \in X$ について、$xs$ を $x$ の $s$ の変換とします。 $\delta_X(s)$ または $\delta(s)$ で、次のように定義される X の準同型性を表します。

(1分)
$$
\delta(s)x = xs^{-1}.
$$

我々は持っています

(2分)
$$
\delta(st) = \delta(s)\delta(t).
$$

構造の輸送、写像の$\delta(s)$の1つの定義する作用、およびXの対策:

(3分)
$$
(\delta(s)f)(x) = f(xs)
$$
(4分)
$$
\langle f, \delta(s)\mu \rangle = \langle \delta(s^{-1})f, \mu \rangle
$$
(5分)
$$
\int_X f(x) d(\delta(s)\mu)(x) = \int_X f(xs^{-1}) d\mu(x)
$$
(6分)
$$
(\delta(s)\mu)(A) = \mu(As).
$$

$d(\delta(s)\mu)(x)$ の代わりに $d\mu(xs)$ を書くことに同意し、(5') には形がかかります

$$
\int_X f(x) d\mu(xs) = \int_X f(xs^{-1}) d\mu(x).
$$

1 つの定義するは、同様の方法で、G の下で X の不変、相対不変、および準不変の測度です。$\mu$ が相対不変の場合、その乗数 $\chi$ は公式によって定義されます。

$$
(7') \quad \delta(s)\mu = \chi(s)\mu
$$
$$
(8') \quad \int_X f(xs)\,d\mu(x) = \chi(s)^{-1} \int_X f(x)\,d\mu(x)
$$
$$
(9') \quad \mu(As) = \chi(s)\mu(A)
$$
$$
(10') \quad d\mu(xs) = \chi(s)\,d\mu(x).
$$

G の反対側の群 $G^0$ が $(x,s) \mapsto xs$ によって X で動作していると見なす場合、$\mu$ は同じ乗数 $\chi$ とともに $G^0$ の下で比較的不変です。

最後に、G を局所コンパクト群とします。 公式 $\gamma(s)x = sx$、$\delta(s)x = xs^{-1}$ に従って、左右の変換によってそれ自体で動作します。それから

$$
(11) \quad \gamma(s)\delta(t) = \delta(t)\gamma(s).
$$

前述のすべてがここに当てはまります。したがって、G には、*左不変*、*右不変*、*相対的に左不変*、*相対的に右不変*、*左準不変*、*右準不変*という測度の概念があります (ただし、番号 8 と 9 を参照)。

写像 $x \mapsto x^{-1}$ は G への G の同型写像です。G 上のすべての写像 $f$ に対して、G 上で定義する写像 $\check{f}$ は次のようになります。

$$
(12) \quad \check{f}(x) = f(x^{-1}).
$$

G 上のすべての小節 $\mu$ について、定義する小節 $\check{\mu}$ を計算します。

$$
(13) \quad \check{\mu}(f) = \mu(\check{f}) \quad \text{for } f \in \mathscr{K}(G).
$$

その他の語では、

$$
(14) \quad \int_G f(x)\,d\check{\mu}(x) = \int_G f(x^{-1})\,d\mu(x).
$$

A が $\check{\mu}$ 積分可能集合である場合、 $A^{-1}$ は $\mu$ 積分可能であり、

$$
(15) \quad \check{\mu}(A) = \mu(A^{-1}).
$$

$d\check{\mu}(x)$ の代わりに $d\mu(x^{-1})$ を書くことに同意し、(14) は形となります。

$$
\int_G f(x)\, d\mu(x^{-1}) = \int_G f(x^{-1})\, d\mu(x).
$$

### 2. 存在と一意性定理

#### 定義 2 {#int-vii-s1-def-2 .statement tag=09D2}

*G を局所コンパクト群とする。 非零左 (右) 不変量である G の正の測度は、G の左 (右) ハール測度と呼ばれます。*

#### 定理 1 {#int-vii-s1-thm-1 .statement tag=09D3}

*すべての局所コンパクト群には左 (右) のハール測度が存在し、定数因子までは 1 つだけ存在します。

A) *存在* — 集合 $\mathscr{K}(G) = \mathscr{K}$、$\mathscr{K}_+(G) = \mathscr{K}_+$、$\mathscr{K}_+^* = \mathscr{K}_+ - \{0\}$。 C が G の圧縮部分集合である場合、C をサポートする $f \in \mathscr{K}_+^*$ の $\mathscr{K}_+^*(C)$ 集合で表します。 $f \in \mathscr{K}$ と $g \in \mathscr{K}_+^*$ については、$f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ となるような G の数 $c_1, \ldots, c_n \geq 0$ と元 $s_1, \ldots, s_n$ が存在します。つまり、$\inf_{s \in U} g(s) > 0$ となるような G の中に空でないオープン集合 U が存在し、 $f$ は、U の左平行移動の有限数でカバーできます。$(f : g)$ を、数 $\geq 0$ のすべての系 $(c_1, \ldots, c_n, s_1, \ldots, s_n)$ に対する数 $\sum_{i=1}^n c_i$ の下限とします。 G の元は $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ になります。それから：

(i) $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$s \in G$ の場合は $(\gamma(s)f : g) = (f : g)$;
(ii) $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$\lambda \geq 0$ の場合は $(\lambda f : g) = \lambda(f : g)$。
(iii) $f \in \mathscr{K}$、$f' \in \mathscr{K}$、$g \in \mathscr{K}_+^*$ の場合は $((f + f') : g) \leq (f : g) + (f' : g)$。
(iv) $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$ の場合は $(f : g) \geq (\sup f)/(\sup g)$
(v) $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$、$h \in \mathscr{K}_+^*$ の場合は $(f : h) \leq (f : g)(g : h)$
(vi) $\mathscr{K}_+^*$ の $f, f_0, g$ に対して $0 < \frac{1}{(f_0 : f)} \leq \frac{(f : g)}{(f_0 : g)} \leq (f : f_0)$
(vii) $f, f', h$ を $f + f'$ のサポート上で $h(s) \geq 1$ とともに $\mathscr{K}_+$ に入れ、$\varepsilon > 0$ とする。 e のコンパクトな近傍 V が存在し、$g \in \mathscr{K}_+^*(V)$ ごとに、

$$
(f : g) + (f' : g) \leq ((f + f') : g) + \varepsilon(h : g).
$$

特性 (i)、(ii)、(iii) は明らかです。 $f \in \mathscr{K}$、$g \in \mathscr{K}_+^*$ としましょう。 $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ と $c_i \geq 0$ の場合、G の一部の s については $\sup f \leq \sum_{i=1}^n c_i g(s_i^{-1}s)$、従って $\sup f \leq (\sum_{i=1}^n c_i) \sup g$、よって (iv)。次に (v) を証明しましょう。 $f \in \mathscr{K}$、$g, h$を$\mathscr{K}_+^*$にしましょう。 $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ と $g \leq \sum_{j=1}^p d_j \gamma(t_j)h$ ($G$ の $c_i \geq 0, d_j \geq 0, s_i, t_j$) の場合、$f \leq \sum_{i,j} c_i d_j \gamma(s_i t_j)h$、従って $(f : h) \leq \sum_{i,j} c_i d_j = (\sum_i c_i)(\sum_j d_j)$;従って$(f : h) \leq (f : g)(g : h)$。 適用 (v) を一方では $f_0, f, g$ に、他方では $f, f_0, g$ にすると (vi) が得られます。最後に、$f, f', h$ を $f + f'$ のサポートで $h(s) \geq 1$ とともに $\mathscr{K}_+$ に入れ、$\varepsilon > 0$ とします。 集合 $F = f + f' + \frac{1}{2} \varepsilon h$; 写像 $\varphi, \varphi'$、その一致するはそれぞれ $f/F$ と $f'/F$ で$f + f'$ のサポート上にあり、零その外側、属するから $\mathscr{K}_+$ です。 $\eta > 0$ごとに、$s^{-1} t \in V$の$|\varphi(s) - \varphi(t)| \leq \eta$と$|\varphi'(s) - \varphi'(t)| \leq \eta$のように、$e$のコンパクトな近傍$V$が存在します。次に、$g \in \mathscr{K}_+^*(V)$ とします。 $s \in G$ごとに、

$$
\varphi \cdot \gamma(s)g \leq (\varphi(s) + \eta) \cdot \gamma(s)g;
$$

なぜなら、これは$\gamma(s)g$が零である点で明らかであり、従って$sV$の外側であるからです。そして$sV$、$\varphi \leq \varphi(s) + \eta$には。同様に、$\varphi' \cdot \gamma(s)g \leq (\varphi'(s) + \eta) \cdot \gamma(s)g$。これは、$c_1, \ldots, c_n$ を $G$ の数 $\geq 0$ と $s_1, \ldots, s_n$ 元とし、$F \leq \sum_{i=1}^n c_i \gamma(s_i)g$ とすることを示しています。それから

$$
f = \varphi F \leq \sum_{i=1}^n c_i \varphi \cdot \gamma(s_i)g \leq \sum_{i=1}^n c_i (\varphi(s_i) + \eta) \cdot \gamma(s_i)g
$$

$f'$ についても同様です。従って

$$
(f : g) + (f' : g) \leq \sum_{i=1}^n c_i (\varphi(s_i) + \varphi'(s_i) + 2\eta) \leq (1 + 2\eta) \sum_{i=1}^n c_i
$$

$\varphi + \varphi' \leq 1$以来。 $F$ の適用定義、そして (ii)、(iii)、(v) から、次のように推測されます。

$$
(f : g) + (f' : g) \leq (1 + 2\eta)(F : g) \leq
$$
$$
(1 + 2\eta)[((f + f') : g) + \frac{1}{2}\varepsilon(h : g)] \leq
$$
$$
(((f + f') : g) + \frac{1}{2}\varepsilon(h : g) + 2\eta((f + f') : h)(h : g) + \varepsilon\eta(h : g)
$$

そして、$\eta[2((f + f') : h) + \varepsilon] \leq \frac{1}{2}\varepsilon$ となるように $\eta$ が選択された場合、(vii) が得られます。

V が e のコンパクトな近傍の集合上を走るので、$\mathscr{K}_+^*$ 上のフィルター $\mathscr{B}$ の $\mathscr{K}_+^*(V)$ 形基底になります。 $\mathscr{F}$ を $\mathscr{B}$ ではなく $\mathscr{K}_+^*$ より細かいの限外フィルターにします。一方、$f \in \mathscr{K}_+^*$と$g \in \mathscr{K}_+^*$については、$f_0 \in \mathscr{K}_+^*$を固定して集合とします。

$$
I_g(f) = \frac{(f : g)}{(f_0 : g)}.
$$

(vi) により、コンパクトな空間 $[1/(f_0 : f), (f : f_0)]$ の中に $\lim_{g,\mathscr{F}} I_g(f) = I(f)$ が存在します。

(iii)までに、$I(f + f') \leq I(f) + I(f')$。 (vii) により、$h$ が $f + f'$ のサポート上で $\geq 1$ であることを条件として、すべての $\varepsilon > 0$ に対して $I(f) + I(f') \leq I(f + f') + \varepsilon I(h)$ が得られます。 $I(f + f') = I(f) + I(f')$ということになります。 Ch.によるII, §2, No. 1、提案 2、I は、$\mathscr{K}$ の線型形式まで拡張可能です。この線型形式は、G に関する正の測度非零であり、(i) によって左不変です。これは求められている左ハールの尺度です。 移行からその反対の群まで、これから右ハール尺度の存在が推測されます。

B) *一意性.* — $\mu$ を左ハール測度、$\nu$ を右ハール測度としましょう。すると$\check{\nu}$は左ハール対策です。 $\mu$ と $\check{\nu}$ が比例することを示します。これは、任意の 2 つの左ハール測度が実際に比例していることを証明します。

$f \in \mathscr{K}$ を $\mu(f) \neq 0$ となるようにします。 補題 1、写像 $D_f$ により、公式により G で定義されました

$$
D_f(s) = \mu(f)^{-1} \int f(t^{-1}s) d\nu(t)
$$

は G 上で連続です。$g \in \mathscr{K}$ とします。 写像 $(s, t) \mapsto f(s)g(ts)$ は、$G \times G$ のコンパクトなサポートと継続します。 Ch.によるIII, §4, No. 1、木曜日。 2、

$$
\begin{align*}
\mu(f)\nu(g) &= \left( \int f(s) d\mu(s) \right) \left( \int g(t) d\nu(t) \right) \\
&= \int d\mu(s) \int f(s)g(ts) d\nu(t) = \int d\nu(t) \int f(s)g(ts) d\mu(s) \\
&= \int d\nu(t) \int f(t^{-1}s)g(s) d\mu(s) \\
&= \int g(s) \left[ \int f(t^{-1}s) d\nu(t) \right] d\mu(s) = \mu(g \cdot \mu(f) D_f),
\end{align*}
$$

よって

$$
\nu(g) = \mu(D_f \cdot g).
$$

これは、まず、$D_f$ が $f$ に依存しないことを証明します。なぜなら、$f' \in \mathscr{K}$ が $\mu(f') \neq 0$ である場合、$D_f \cdot \mu = D_{f'} \cdot \mu$ であるため、$D_f$ と $D_{f'}$ は連続であり、$\mu$ のサポートは $G$ であるため、$\mu$ については局所的にほぼどこでも $D_f = D_{f'}$ となり、したがってどこでもです。したがって、$D_f = D$ と書くこともできます。 公式 (16) を与えます

$$
\mu(f)D(e) = \check{\nu}(f).
$$

公式 (19) は、$\mu(f) = 0$ のように、線形性によって写像 $f \in \mathscr{K}$ に拡張できます。 $\check{\nu} \neq 0$から$D(e) \neq 0$です。これにより、実際に $\mu$ と $\check{\nu}$ の比例関係が確立されます。

#### 系 {#int-vii-s1-n2-cor-1 .statement tag=09D4}

— *すべての左不変量* (それぞれ *右不変量*) *測定オン* $G$ *は左* (それぞれ *右*) *ハール測定*に比例します。

#### 例 {#int-vii-s1-n2-exa-1 .statement tag=09D5}

— 1) 加法群 $\mathbf{R}$ では、ルベーグ測度 $dx$ はハール測度です (Ch. III, §1, No. 3、*例*)。

2) 写像 $f \in \mathscr{K}(\mathbf{R}_+^*)$ ごとに、(FRV, II, §1, 公式 (12))

$$
\int_0^{+\infty} \frac{f(x)}{x} dx = \int_0^{+\infty} \frac{f(tx)}{tx} t dx = \int_0^{+\infty} \frac{f(tx)}{x} dx
$$

すべての$t > 0$;したがって、メジャー $x^{-1} dx$ は乗法群 $\mathbf{R}_+^*$ の Haar メジャーです。

3) $G$ トーラス $T = \mathbf{R}/\mathbf{Z}$ を考えてみましょう。 $\varphi$ を $T$ 上の $\mathbf{R}$ の標準写像とします。 $f \in \mathscr{K}(T)$、写像 $f \circ \varphi$ は連続かつ周期的で、$\mathbf{R}$ が周期 1 であり、積分は

$$
I(f) = \int_a^{a+1} f(\varphi(x)) dx
$$

$a \in \mathbf{R}$の選択から独立しています。翻訳下で不変であることは明らかです。したがって、定義するは $T$ のハール測度です。 構造の輸送により、これから $I(f) = \int_a^{a+1} f(e^{2\pi i t}) dt$ は絶対値 1 (GT、VIII, §2, No. 1) の複素数の乗法群 $U$ に対するハール測度であることが推測されます。

#### 命題 2 {#int-vii-s1-prop-2 .statement tag=09D6}

— *$G$ *を局所的にコンパクトな群*、$\mu$ *左または右のハール測度* $G$ とします。 *$G$ *離散的であるためには、* $\mu(\{e\}) > 0$ であることが必要かつ十分です。 *$G$ *コンパクトであるためには、* $\mu^*(G) < +\infty$ であることが必要十分です。

条件は明らかに必要です。 彼らの十分性を証明しましょう。 $V$ を $e$ のコンパクトな近傍とする。 $\mu(\{e\}) > 0$ の場合、$\mu(V) < +\infty$ から $V$ は有限の集合になります。 $G$ はハウスドルフであるため、離散的です。 たとえば、$\mu^*(G) < +\infty$ と $\mu$ が左不変であるとします。 $i \neq j$ に対して $s_i V \cap s_j V = \varnothing$ となるように、有限部分集合 $\{s_1, \ldots, s_n\}$ の $G$ の集合 $\mathscr{E}$ を考えてみましょう。それから

$$
n \mu(V) = \mu(s_1 V \cup \ldots \cup s_n V) \leq \mu^*(G),
$$

therefore $n \leq \mu^*(G)/\mu(V)$.したがって、$\mathscr{E}$ 極大元 $\{s_1, \ldots, s_n\}$ で選ぶになる可能性があります。そして、$s \in G$ごとに、$s V \cap s_i V \neq \varnothing$となるような$i$が存在し、したがって$s \in s_i V V^{-1}$となる。したがって、$G$ はコンパクトな集合 $s_i V V^{-1}$ の和集合であるため、コンパクトです。

### 3. 弾性率

$\mu$ を $G$ の左ハール測度とする。すべての $s \in G$、$\delta(s)\mu$ も左不変 (No. 1、公式 (11)) であるため、(Th. 1) $\delta(s)\mu = \Delta_G(s)\mu$ のような一意の数 $\Delta_G(s) > 0$ が存在します。 Th のおかげで。 1、数 $\Delta_G(s)$ は $\mu$ の選択から独立しています。

#### 定義 3 {#int-vii-s1-def-3 .statement tag=09D7}

*$G$ の写像 $\Delta_G$ は、$G$ のモジュラス (またはモジュラー 写像) と呼ばれます。 $\Delta_G = 1$、群 $G$ はユニモジュラーであると言われます。*

$\mu$ は乗数 $\Delta_G$ と相対的に右不変であるとも言えます。したがって、$\Delta_G$ は、$\mathbf{R}_+^*$* の $G$ の *連続表現です (No. 1、提案 1)。

#### 注意 {#int-vii-s1-n3-rem-1 .statement tag=09D8}

— $\varphi$ が局所的にコンパクトな群 $G'$ 上で $G$ の同型である場合、$\Delta_{G'} \circ \varphi = \Delta_G$。特に:
1) $x \mapsto x^{-1}$ は、反対側の群 $G^0$ の$G$ の同型なので、$\Delta_{G^0} = \Delta_G^{-1}$ になります。
2) $\varphi$ が $G$ の自己同型の場合、$\Delta_G \circ \varphi = \Delta_G$ です。

$s \in G$ にしましょう。次に:

$$
\delta(s)(\Delta_G^{-1} \cdot \mu) = (\delta(s)\Delta_G^{-1}) \cdot (\delta(s)\mu) = (\Delta_G(s)^{-1}\Delta_G^{-1}) \cdot (\Delta_G(s)\mu) = \Delta_G^{-1} \cdot \mu,
$$

したがって、$\Delta_G^{-1} \cdot \mu = \mu'$ は正しいハール単位です。このことから、$\gamma(s)\mu' = (\gamma(s)\Delta_G^{-1}) \cdot \mu = \Delta_G(s)(\Delta_G^{-1} \cdot \mu) = \Delta_G(s)\mu'$ であるため、すべての適切なハール測度 $\nu$ に対して、$\gamma(s)\nu = \Delta_G(s)\nu$ が得られます。 $\dot{\mu}$ は正しいハール測度なので、$\dot{\mu} = a \Delta_G^{-1} \cdot \mu$ と定数 $a > 0$;それは次のとおりです

$$
\mu = a(\Delta_G^{-1} \cdot \mu)^{\vee} = a \Delta_G \cdot \dot{\mu} = a^2 \mu,
$$

したがって、$a = 1$、そして最後に$\dot{\mu} = \Delta_G^{-1} \cdot \mu$となります。 $\dot{\nu} = \Delta_G \cdot \nu$ も同様にわかります。

したがって、次のような結果が得られます。

公式集。 — G を局所的にコンパクトな群、その係数 $\Delta$、左ハール測度 $\mu$、右ハール測度 $\nu$ とする。

1) ある人は

$$
\gamma(s)\mu = \mu \quad \delta(s)\mu = \Delta(s)\mu \quad \check{\mu} = \Delta^{-1} \cdot \mu .
$$

$f$ が G 上で $\mu$ 積分可能である場合、$f$ の左と右の変換は $\mu$ 積分可能であり、

$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
(21)
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x) .
$$

さらに、$\check{f}$ は $\Delta^{-1} \cdot \mu$ に対して積分可能であり、

$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x) .
$$
(22)

A が G の $\mu$ 積分可能部分集合である場合、sA と As は $\mu$ 積分可能であり、

$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A) .
$$
(23)

2) ある人は

$$
\delta(s)\nu = \nu \quad \gamma(s)\nu = \Delta(s)\nu \quad \check{\nu} = \Delta \cdot \nu .
$$

$f$ が G 上で $\nu$ 積分可能である場合、$f$ の左と右の変換は $\nu$ 積分可能であり、

$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\nu(x)
$$
(25)
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x) .
$$

さらに、$\check{f}$ は $\Delta \cdot \nu$ に対して積分可能であり、

$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x) .
$$
(26)

A が G の $\nu$ 積分可能部分集合である場合、sA と As は $\nu$ 積分可能であり、

$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s)^{-1} \nu(A) .
$$
(27)

3) $\nu$ は $\Delta^{-1} \cdot \mu$ に比例し、$\mu$ は $\Delta \cdot \nu$ に比例します。

4) G が *ユニモジュラー* であると仮定します。 $\mu$ を G の Haar 測度とする。すると、次のようになります。

$$
\gamma(s)\mu = \delta(s)\mu = \dot{\mu} = \mu .
$$

$f$ が G 上で $\mu$ 積分可能である場合、$f$ の左と右の変換は、$\check{f}$ と同様に $\mu$ 積分可能であり、

$$
\int f(sx)\,d\mu(x) = \int f(xs)\,d\mu(x) = \int f(x^{-1})\,d\mu(x) = \int f(x)\,d\mu(x) .
$$

A が G の $\mu$ 積分可能部分集合である場合、sA、As および $A^{-1}$ は $\mu$ 積分可能であり、

$$
\mu(sA) = \mu(As) = \mu(A^{-1}) = \mu(A) .
$$

本質的な積分の類似の性質が成り立つ。

#### 命題 3 {#int-vii-s1-prop-3 .statement tag=09D9}

*G に内部自己同型の下で e 不変式のコンパクトな近傍 V が存在する場合、G は単モジュールです。*

というのは、$\mu$ を G の左ハール測度とする。すべての $s \in G$ について、

$$
\mu(V) = \mu(s^{-1}Vs) = \Delta_G(s)\mu(V) ,
$$

$0 < \mu(V) < +\infty$ からよって $\Delta_G(s) = 1$。

このことから、すぐに次のように推測できます。

#### 系 {#int-vii-s1-n3-cor-1 .statement tag=09DA}

*G が離散的、コンパクト、または可換である場合、G はユニモジュラーです。*

さらに、G が *可換* である場合、これは自明です。 注意また、G が *離散* の場合、各点が質量 1 を持つ G 上の測度は、明らかに G 上の左右のハール測度であり、G 上の *正規化された* ハール測度と呼ばれます。G が *コンパクト* の場合、$\mu(G) = 1$ のような G 上のハール測度が 1 つだけ存在します。これは、G の *正規化された * Haar 測度と呼ばれます。G が離散的かつコンパクトな、つまり有限である場合、前述の 2 つの規則は一致しません。この場合、正規化されたハール測度が何を意味するかを常に明示的に指定する必要があります。

ユニモジュラー 群の部分群と剰余群は必ずしもユニモジュラーであるとは限りません (§ 2、Exer. 5)。ただし、§ 2, No. 7 の提案 10 を参照してください。

*後ほど、半単純または nilpotent 接続されたリー群がユニモジュラーであることがわかります。

### 4. 自己同型の係数

G を G の局所的にコンパクトな群、$\varphi$ 自己同型、および G の左ハール測度 $\mu$ とします。 $\varphi^{-1}(\mu)$ も G の左ハール対策であることは明らかです。 従って、$\varphi^{-1}(\mu) = a \mu$ となるような数 $a > 0$ が 1 つだけ存在します (No. 2, Th. 1)。 No. 2 様、Th. 1、この数は$\mu$の選択とは独立しています。 正しい Haar 測度、たとえば $\Delta_G^{-1} \cdot \mu$ (No. 3) から始めた場合、同じスカラー $a$ に到達することに注意してください。なぜなら、$\varphi^{-1}$ は $\Delta_G$ 不変のままであるため (No. 3, 注意)、$\varphi^{-1}(\Delta_G^{-1} \cdot \mu) = \Delta_G^{-1} \cdot \varphi^{-1}(\mu) = a \Delta_G^{-1} \cdot \mu$ になります。

#### 定義 4 {#int-vii-s1-def-4 .statement tag=09DB}

*数 $a > 0$ で、$\varphi^{-1}(\mu) = a \mu$ は自己同型 $\varphi$ の法と呼ばれ、$\operatorname{mod}_G \varphi$ または単に $\operatorname{mod} \varphi$ と表されます。*

$f$ が G 上の $\mu$ 可積分関数である場合、

$$
\int f(\varphi^{-1}(x)) d\mu(x) = (\operatorname{mod} \varphi) \int f(x) d\mu(x).
$$

A が G の $\mu$ 可積分部分集合である場合、

$$
\mu(\varphi(A)) = (\operatorname{mod} \varphi) \mu(A).
$$

特に、$s \in G$ については、$i_s$ を内部自己同型 $x \mapsto s^{-1} x s$ とします。そうすると $i_s^{-1} = \delta(s) \gamma(s)$ なので、

$$
i_s^{-1}(\mu) = \delta(s) \mu = \Delta_G(s) \mu,
$$

その結果

$$
\operatorname{mod} i_s = \Delta_G(s).
$$

G が離散またはコンパクトの場合、その正規化されたハール測度は、構造の輸送からすぐに分かるように、G の自己同型 $\varphi$ ごとにそれ自体に変換されます。従って、離散またはコンパクト群の *自己同型は法 1* を持ちます。

#### 命題 4 {#int-vii-s1-prop-4 .statement tag=09DC}

*G を、G の自己同型の群 $\mathscr{G}$ への局所的コンパクト群、トポロジカル群 $\Gamma$、および $\Gamma$ の $\gamma \mapsto u_\gamma$ 準同型とし、$(\gamma, x) \mapsto u_\gamma(x)$ が連続写像となるようにします。 $\Gamma \times G$をGに。 すると、写像 $\gamma \mapsto \operatorname{mod}(u_\gamma)$ は、$\mathbf{R}_+^*$ の $\Gamma$ の連続表現です。

この写像は明らかに $\mathbf{R}_+^*$ の $\Gamma$ の表現 (代数) です。その連続性を証明するには十分です。 $f \in \mathscr{K}(G)$ とし、S をそのサポートとします。*

$\gamma_0 \in \Gamma$ と $U$ を $u_{\gamma_0}^{-1}(S)$ の比較的コンパクトな近傍とする。 写像 $\gamma \mapsto u_\gamma$ は、コンパクトコンバージェンス (GT、X, §3, No. 4、Th. 3) の位相を備えた $\Gamma$ から $\mathscr{G}$ への連続的な写像です。したがって、$\gamma$ は $\gamma_0$ に十分近いため、$u_\gamma^{-1}(S) \subset U$ になります。 No. 1 の補題 1 は、$\int f(u_\gamma(x)) d\mu(x)$ (ここで、$\mu$ は左ハール測度 $G$ を示します) が継続的に $\gamma$ に依存することを証明します。 よって命題。

### 5. 積のハール測定

#### 命題 5 {#int-vii-s1-prop-5 .statement tag=09DD}

— *$(G_\iota)_{\iota \in I}$ *を局所的にコンパクトな群* の族とします。 *すべて* $\iota \in I$ *let* $\mu_\iota$ * $G_\iota$ を左 (または右) のハール測定にします。 *$I$ のうち * 有限部分集合* $J$ が存在し、*すべての* $\iota \in I - J$ に対して、$G_\iota$ * がコンパクトで* $\mu_\iota(G_\iota) = 1$ になると仮定します。 *次に積を測定します* $\bigotimes_{\iota \in I} \mu_\iota$ * は左 (右) のハール測定です* $G = \prod_{\iota \in I} G_\iota$。 *もし* $x = (x_\iota) \in G$ *その後*
$$
\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota).
$$
$I$ のすべての有限部分集合 $J$ について、定義からすぐに続くように、$\bigotimes_{\iota \in J} \mu_\iota$ は $\prod_{\iota \in J} G_\iota$ の左 (それぞれ右) ハール測度です。 したがって、$\bigotimes_{\iota \in I} \mu_\iota$ は、$G$ (Ch. III, §4, No. 6、提案 9)。 一方、$\mu_\iota$ がハール対策のままの場合、
$$
\delta(x) \left( \bigotimes_{\iota \in I} \mu_\iota \right) = \bigotimes_{\iota \in I} \delta(x_\iota) \mu_\iota = \bigotimes_{\iota \in I} (\Delta_{G_\iota}(x_\iota) \mu_\iota) = \left( \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota) \right) \bigotimes_{\iota \in I} \mu_\iota,
$$
よって $\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota)$。

#### 例 {#int-vii-s1-n5-exa-1 .statement tag=09DE}

— 1) $\mathbf{R}^n$ のルベーグ測度は、加法群 $\mathbf{R}^n$ のハール測度です。

2) 写像 $(r, u) \mapsto ru$ は、$\mathbf{R}_+^* \times \mathbf{U}$ の同型を$\mathbf{C}^*$ (GT、VIII, §1, No. 3) に変換します。この同型によって$\mathbf{C}^*$が$\mathbf{R}_+^* \times \mathbf{U}$と同一視され、$du$が$\mathbf{U}$のハール測度を示す場合、$r^{-1} dr du$はNo. 2の例2による$\mathbf{C}^*$のハール測度になります。一方、$[0, 1[$の全単射$\theta \mapsto e^{2i\pi \theta}$は$\mathbf{U}$変換に、$[0, 1[$のルベーグ測度$d\theta$は、No. 2の例3によって$\mathbf{U}$のハール測度に変換されます。したがって、$f \in \mathscr{H}(\mathbf{C}^*)$ の場合、積分は
$$
\int_0^{+\infty} \int_0^1 f(re^{2i\pi \theta}) r^{-1} dr\, d\theta
$$
定義する $\mathbf{C}^*$ のハール測定。

### 6. 逆数のハール測度極限*

G を局所的にコンパクトな群 (したがって完全) とします。 $(K_\alpha)_{\alpha \in A}$ を、共通部分 $\{e\}$ を持つ、G のコンパクト法線部分群の有向族減少するとします ($K_\alpha$ によって形成されるフィルター 基底が e に収束するように)。 集合 $G_\alpha = G / K_\alpha$; $\varphi_\alpha : G \to G_\alpha$ と $\varphi_{\beta \alpha} : G_\alpha \to G_\beta \ (\alpha \geq \beta)$ を標準準同型とします。次に、逆数系 $(G_\alpha, \varphi_{\beta \alpha})$ の逆数極限は G と同一視され、この逆数極限の $G_\alpha$ の逆数標準写像は $\varphi_\alpha$ と同一視されます (GT、III, §7, No. 3、提案 2)。 写像 $\varphi_\alpha$ と $\varphi_{\beta \alpha}$ は適切です (*上記引用*、§4, No. 1、提案 1 の Cor. 2)。これらの仮定は、この小節を通じて固定されたままになります。

\* 補題 2. — a) *$f \in \mathscr{K}_+(G)$、S を G 含むのコンパクト部分集合、補足 $f$、U を G 内の S の開いた近傍、および $\varepsilon > 0$ とします。 U の外側に $\alpha \in A$ と写像 $g \in \mathscr{K}_+(G)$、零が存在し、$K_\alpha$ の剰余類には $|f - g| \leq \varepsilon$ となる定数が存在します。

b) *$\mu$ と $\mu'$ を G 上の 2 小節とし、すべての $\alpha \in A$ に対して $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ となるようにします。次に$\mu = \mu'$。

$K_{\alpha_1} S \cap K_{\alpha_1}(G - U) = \emptyset$ となるような $\alpha_1 \in A$ が存在します (GT、II, §4, No. 3、提案 4)。 したがって、S を増加させ、U を減少させると、S と U は $K_{\alpha_1}$ の剰余類の和集合であると仮定できます。 次の性質を持つ S 上の連続数値写像 $h$ を考えてみましょう: $h$ が $K_\alpha$ の剰余類上で定数となるような $\alpha \geq \alpha_1$ が存在します。 These functions form a subalgebra of $\mathscr{K}(S)$ (because $(K_\alpha)$ is a decreasing directed family) that contains the constants and separates the points of S: for, let $x, y$ be two distinct points of S; since the intersection of the $K_\alpha$ is $\{e\}$, there exists an $\alpha \geq \alpha_1$ such that $\varphi_\alpha(x) \neq \varphi_\alpha(y)$, then a numerical function $u$ continuous on $\varphi_\alpha(S)$ such that $u(\varphi_\alpha(x)) \neq u(\varphi_\alpha(y))$. ストーン・ヴァイエルシュトラス定理によれば、S 上には $K_\alpha$ の剰余類上で定数である $\alpha \geq \alpha_1$ と連続する写像 $h \geq 0$ が存在し、S 上では $|f - h| \leq \frac{\varepsilon}{2}$ となる。 $t \in \mathbf{R}$、集合 $\delta(t) = \left( t - \frac{\varepsilon}{2} \right)^+$、集合 $h' = \delta \circ h$ ごとに。 この場合、$h'$ は写像 $\geq 0$ であり、S では連続、$K_\alpha$ の剰余類では定数、S では $|h - h'| \leq \frac{\varepsilon}{2}$ であるため、S では $|f - h'| \leq \varepsilon$ になります。 一方、G の S の境界に x 属するを加えると、$h(x) \leq \frac{\varepsilon}{2}$ となるため、$h'(x) = 0$ となります。 $h'$ を S の補数で 0 拡張すると、要件を満たす写像 $g$ が得られ、a) が証明されます。

ここで、$\mu, \mu'$ を G 上の 2 小節とし、すべての $\alpha \in A$ に対して $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ となるようにします。 $v \in \mathscr{K}(G)$ を、$\alpha \in A$ について$K_\alpha$ の剰余類で定数写像とし、$v = w \circ \varphi_\alpha$ を $w \in \mathscr{K}(G_\alpha)$ で書くことができます。それから

\* 参照。 Ch. III, §4, No. 5。

$$
\mu(v) = (\varphi_\alpha(\mu))(w) = (\varphi_\alpha(\mu'))(w) = \mu'(v); \text{ it follows that } \mu = \mu' \text{ by virtue of a)}.
$$

#### 命題 6 {#int-vii-s1-prop-6 .statement tag=09DF}

*すべて* $\alpha \in A$ について、*$\mu_\alpha$ を *$G_\alpha$ に対する前向きな指標とします。 *$\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$ *$\alpha \geq \beta$ の場合* と仮定します。 *そして、ポジティブな対策は 1 つだけ存在します* $\mu$ *on* $G$ *そのような* $\varphi_\alpha(\mu) = \mu_\alpha$ *すべてに対して* $\alpha \in A$。

一意性は補題 2 b) の直後に続きます。 $\mu$ の存在を証明しましょう。 $V$ を写像所属から $\mathscr{K}(G)$ のベクトル空間とし、いくつかの $K_\alpha$ の剰余類で定数とします ($\alpha$ は写像に依存する可能性があります)。 補題 2 a) から、$V$ は第 1 章の条件 (P) を満たすことがわかります。 III, §1, No. 7、提案9: $K$を、$G$と選ぶ$f \in \mathscr{K}_+(G)$の$f(x) > 0$をすべての$x \in K$でコンパクトにした集合とする。 $a > 0$ を $K$ の $f$ の最小の値とします。 補題 2 a) により、$|f - g| \leq a/2$ となるような写像 $g \in V \cap \mathscr{K}_+(G)$ が存在するため、すべての $x \in K$ に対して $g(x) > 0$ となり、条件 (P) が検証されます。 $f \in V$ にしましょう。 $f$ が $K_\alpha$ の剰余類上で定数となるような $\alpha \in A$ が存在します。 商、$f$ 定義する写像 $f_\alpha \in \mathscr{K}(G_\alpha)$ への通過により。 数 $\mu(f) = \mu_\alpha(f_\alpha)$ は $\alpha$ の選択に依存しません。つまり、$\beta$ を、$f$ が $K_\beta$ の剰余類で定数となるような任意の添字とします。 $\gamma \in A$ を $\gamma \geq \alpha, \gamma \geq \beta$ となるようにします。次に、$f$ 定義する写像 $f_\beta \in \mathscr{K}(G_\beta)$、$f_\gamma \in \mathscr{K}(G_\gamma)$ は $f = f_\beta \circ \varphi_\beta = f_\gamma \circ \varphi_\gamma$ になります。次に$f_\alpha \circ \varphi_{\alpha\gamma} = f_\gamma$、したがって$\mu_\gamma(f_\gamma) = (\varphi_{\alpha\gamma}(\mu_\gamma))(f_\alpha) = \mu_\alpha(f_\alpha)$、そして同様に$\mu_\gamma(f_\gamma) = \mu_\beta(f_\beta)$、よってが私たちの主張になります。 これにより、$\mu$ は $V$ では線型形式であり、$f \geq 0$ では $\mu(f) \geq 0$ であることが明らかです。 第 9 章の提案による。 III, §1, No. 7、$\mu$ は、$G$ でプラスの測定値に拡張される可能性があり、これを再び $\mu$ で示します。 $\mu$ のちょうど構成までに、すべての $\alpha \in A$ に対して $\varphi_\alpha(\mu) = \mu_\alpha$ があります。

#### 定義 5 {#int-vii-s1-def-5 .statement tag=09DG}

*メジャー* $\mu$ *は* $\mu_\alpha$の逆数極限 (または射影極限) であると言われています。

#### 命題 7 {#int-vii-s1-prop-7 .statement tag=09DH}

*提案 6 の記法を維持します。それぞれ* $\mu_\alpha$ * が $G_\alpha$ 上の左 (または右) ハール測定値である場合、* $\mu$ * は * $G$ 上の左 (または右) ハール測定値です。

たとえば、$\mu_\alpha$ が左 Haar メジャーであると仮定します。 $s \in G$ にしましょう。 $x \in G$ ごとに、

$$
(\varphi_\alpha \circ \gamma(s))(x) = \varphi_\alpha(sx) = \varphi_\alpha(s)\varphi_\alpha(x) = (\gamma(\varphi_\alpha(s)) \circ \varphi_\alpha)(x);
$$

したがって$\varphi_\alpha(\gamma(s)\mu) = \gamma(\varphi_\alpha(s))\mu_\alpha = \mu_\alpha$。したがって、$\gamma(s)\mu = \mu$ by 補題 2 b)、したがって、$\mu$ は左ハール測度です。

今後、$K_\alpha$ はコンパクトなだけでなく、$G$ にオープンになると仮定します。 $G_\alpha$ は離散的であり、$\beta \geq \alpha$ の場合、$K_\alpha/K_\beta$ はコンパクトで離散的な群であるため、有限です。 群 $G$ はユニモジュラーです (提案 3)。

#### 命題 8 {#int-vii-s1-prop-8 .statement tag=09DI}

a) *$\mu$ *と* $\mu'$ *を* $G$ *すべての* $\alpha$ *およびすべての剰余類* $C$ *の* $K_\alpha$、$\mu(C) = \mu'(C)$ に対する2つの肯定的な測度とする。 *それでは* $\mu = \mu'$。

b) *$\alpha_0 \in A$ を修正します。 *すべて* $\alpha \geq \alpha_0$ * $n_\alpha$ * 数の元の有限群* $K_{\alpha_0}/K_\alpha$ になります。 *正の測度は 1 つだけ存在します* $\mu$ *上* $G$ *すべての* $\alpha \geq \alpha_0$ について、*$K_\alpha$ の各剰余類は *測度* $n_\alpha^{-1}$ を持ちます。 *さらに、$\mu$ は $G$ のハール測度であり、*$\mu(K_{\alpha_0}) = 1$ となります。

$\mu$ と $\mu'$ を $G$ 満たす条件 a) に対する 2 つの前向きの尺度とします。離散群 $G_\alpha$ の点は、$\varphi_\alpha(\mu)$ と $\varphi_\alpha(\mu')$、よって $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ について同じメジャーを持ち、これはすべての $\alpha$ についても同様です。したがって、$\mu = \mu'$ (補題 2 b))。

b)を証明しましょう。すべての $\alpha \geq \alpha_0$ について、すべての点が測定値 $n_\alpha^{-1}$ を持つように、$\mu_\alpha$ を離散群 $G_\alpha$ のハール測定値とします。 $\alpha, \beta$ を $\alpha \geq \beta \geq \alpha_0$ となるようにします。すると、$K_\beta/K_\alpha$ は $n_\alpha/n_\beta$ 元になります。したがって、$\varphi_{\beta\alpha}(\mu_\alpha)$ は $G_\beta$ のメジャーであり、各点にはメジャー $n_\alpha^{-1} \cdot \frac{n_\alpha}{n_\beta} = n_\beta^{-1}$ が含まれます。他には語、$\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$。その後、Props を適用するだけで十分です。 6と7。

#### 例 {#int-vii-s1-n6-exa-1 .statement tag=09DJ}

— $\mathbf{Q}_p$ を $p$ 進数体とし、$p$ 進絶対数値 $|x|_p = p^{-v_p(x)}$ (GT, IX, §3, No. 2, *例 3*) の$\mathbf{Q}$ の完成とします。 $\mathbf{Q}_p$ の元は *$p$*-*進数数* と呼ばれます。 $p$ 進絶対値値から $\mathbf{Q}_p$ の連続拡大を再び $|x|_p$ で表します。 1つは持っています

$$
|x + y|_p \leq \sup(|x|_p, |y|_p)
$$

$\mathbf{Q}$ の $x, y$ (*loc. cit.*)、したがって $\mathbf{Q}_p$ の $x, y$ になります。さらに、$|y|_p < |x|_p$なら$|x + y|_p = |x|_p$、なぜなら$|x|_p = |(x + y) - y|_p \leq \sup(|x + y|_p, |y|_p)$だからです。 $(x_n)$ が $\mathbf{Q}_p$ の点の数列で、$x \in \mathbf{Q}_p^*$ の傾向がある場合、$|x - x_n|_p < |x|_p$ と $|x - x_n|_p < |x_n|_p$ は $n$ 十分大きいであるため、$|x|_p = |x_n|_p$ になります。これは、すべての $x \in \mathbf{Q}_p^*$ に対して、$|x|_p$ は $p$ の冪であることを証明します。

$\mathbf{Z}_p$ を $\mathbf{Q}_p$ の $\mathbf{Z}$ の閉包とします。これは $\mathbf{Q}_p$ の部分環です。その元は *$p$*-*進数整数* と呼ばれます。 $x \in \mathbf{Z}_p$ ごとに 1 つが $|x|_p \leq 1$ になります。 逆に、$x$ を $|x|_p \leq 1$ となるような $\mathbf{Q}_p$ の元とし、$x \in \mathbf{Z}_p$ であることを示しましょう。上で見たことから、$n$ 十分大きいに対して $x$ と $|x_n|_p \leq 1$ の傾向がある $\mathbf{Q}$ の元のうち数列 $(x_n)$ が存在します。 $n$ 十分大きいに対して $x_n$ 属するから $\mathbf{Z}_p$ であることを示すだけで十分です。他の語では、$x \in \mathbf{Q}$ の場合に帰着します。次に $x = a/b$ と $b$ は $p$ と互いに素です。 整数 $n > 0$ ごとに、$bb'_n + h_n p^n = 1$、よって $x = \frac{abb'_n + ah_n p^n}{b} = ab'_n + \frac{ah_n p^n}{b}$、$|x - ab'_n|_p \leq p^{-n}$ となるように $b'_n \in \mathbf{Z}$ と $h_n \in \mathbf{Z}$ が存在するため、$ab'_n$ は $x$ になる傾向があります。

このことから、中心 0 および半径 $p^{-n}$ のクローズド ボールは、中心 0 および半径 $p^{-n+1}$ のオープン ボールと同一で、$p^n \mathbf{Z}_p$ であることがわかります。したがって、トポロジカル空間 $\mathbf{Q}_p$ は 0 次元であるため、完全に切り離されています (GT、IX, §6, No. 4)。

整数 $0, 1, \ldots, p^n - 1$ が $\mathbf{Z}_p$ モジュロ $p^n \mathbf{Z}_p$ の代表の系を構成することを示しましょう。まず、2 つの整数 $k$ と $k'$ の $|k - k'|_p > p^{-n}$ なので、これら整数の $p^n \mathbf{Z}_p$ を法とする類は別個です。一方、$x \in \mathbf{Z}_p$; としましょう。 $|x - k|_p \leq p^{-n}$ となるような $k \in \mathbf{Z}$ が存在します。 $p^n$ の適切な倍数を $k$ に追加すると、$k \in [0, p^n - 1]$ と $x$ は $p^n \mathbf{Z}_p$ を法とする $k$ と合同であると仮定できます。 よって私たちの主張。これは、$\mathbf{Z}_p / p^n \mathbf{Z}_p$ が正規的に $\mathbf{Z}/p^n \mathbf{Z}$ と同型であることを示しています。さらに、$\mathbf{Z}_p$ は事前コンパクトであり、完成しているので *コンパクト* であることがわかります。 $\mathbf{Z}_p$ は $\mathbf{Q}_p$ の開いた部分群であるため、$\mathbf{Q}_p$ は *局所的にコンパクト* です。 $\mathbf{Q}_p$ の位相には可算数の基底があります (GT、IX, §2, No. 9、提案 16 の Cor.)。 加法群 $\mathbf{Q}_p$ は、離散群 $\mathbf{Q}_p / p^n \mathbf{Z}_p$ の逆数極限と識別される場合があります。

加法群 $\mathbf{Q}_p$ には、$\alpha(\mathbf{Z}_p) = 1$ となるハール測度 $\alpha$ が 1 つだけ存在します。それは、$\mathbf{Q}_p$ の *正規化ハール測度* と呼ばれます。 $\mathbf{Z}_p$ は $p^n \mathbf{Z}_p$ ($n$ 整数 $\geq 0$) の $p^n$ 互いに素剰余類の和集合なので、$\alpha(p^n \mathbf{Z}_p) = p^{-n}$ になります。同様に $\alpha(p^{-n} \mathbf{Z}_p) = p^n$ なので、最終的には $n \in \mathbf{Z}$ ごとに $\alpha(p^n \mathbf{Z}_p) = p^{-n}$ になります。提案 8 b) によれば、$\alpha$ *は $\mathbf{Q}_p$ に対する唯一の正の測度であり、* $p^n \mathbf{Z}_p$ のすべての剰余類 (*n* *整数* $\geq 0$) * は *測度* $p^{-n}$ を持ちます。

$\alpha$ から $\mathbf{Z}_p$ の制限は、明らかに $\mathbf{Z}_p$ の Haar 尺度です。

### 7. ハール単位のローカル定義

#### 命題 9 {#int-vii-s1-prop-9 .statement tag=09DK}

*G を局所的にコンパクトな群、G のオープン部分集合である V、および以下の性質を持つ V の正の測度 $\mu$ 非零とする: U が V のオープン部分集合であり、$s \in G$ が$sU \subset V$、すると、sU に対する U の同型写像 $x \mapsto sx$ の下で、U の $\mu$ によって誘導される測度 $\mu_U$ の像は $\mu_{sU}$ になります。すると、G には V に誘導する $\mu$ が残るハール小節 $\alpha$ が 1 つだけ存在します。

すべての $s \in G$ について、sV 上の V の同型写像 $x \mapsto sx$ の下で、$\mu_s$ を $\mu$ の像とします。 $\mu_s$ ～ $V \cap sV$ の制限は、$x \mapsto sx$ ～ $s^{-1}V \cap V$ の制限の下にある $\mu_{s^{-1}V \cap V}$ の像です。 仮定によって、この像は $\mu_{V \cap sV}$ になります。 翻訳すると、この中から 1 つの結論するは、$\mu_s$ と $\mu_t$ が、どの $s, t$ についても同じ制限から $sV \cap tV$ を持ちます。 したがって、第 1 章の提案 1 により、 III, §2, No. 1、G には $s$ ごとに sV で誘導する $\mu_s$ という尺度 $\alpha$ が存在します。 $\alpha$ が、V で $\mu$ を誘導する、G でのユニークな左ハール測度であることは明らかです。

#### 系 {#int-vii-s1-n7-cor-1 .statement tag=09DL}

*G、G' を 2 つの局所的にコンパクトな群、V (それぞれ V')、G (それぞれ G') のニュートラル元の開いた近傍、および $\varphi$ を G (GT、III, §1, No. 3、定義 2) で定義された G' のローカル同型とします。 V'、つまり $\varphi(V') = V$ になります。 $\alpha'$ を G' の左ハール測度とし、$\alpha'_V$ をその制限から $V'$ とします。次に、$\varphi(\alpha'_{V'})$ は、$G$ の左ハール固有のメジャー $\alpha$ の制限から $V$ です。

$V_1$ を、$V_1 V_1^{-1} \subset V$ となるような $G$ の $e$ の開いた近傍とする。 $\mu$を$\varphi(\alpha'_{V'})$から$V_1$の制限とします。 $U$ を $V_1$ のオープン部分集合とし、$s \in G$ を $sU \subset V_1$ となるようにします。 そうすると、$s \in V_1 V_1^{-1} \subset V$、したがって、$s' \in V'$ については $s = \varphi(s')$ になります。 $x \in U$ にしましょう。 次に、一部の $x' \in V'$ に対して $x = \varphi(x')$、つまり $sx \in sU \subset V$ から $sx = \varphi(s')\varphi(x') = \varphi(s'x')$ になります。 $G'$ の左の翻訳は $\alpha'$ を保持しているため、提案 9 の $V_1$ と $\mu$ 満たす条件がわかります。 $\alpha$ を $G$ の左ハール測度として、$V_1$ で $\mu$ を誘導します。 すべての $t \in V$ に対して、$tW \subset V$ のような、$V_1$ の $e$ のオープン近傍 $W$ が存在します。 その場合、$\varphi(\alpha'_{V'})$ から $tW$ の制限は、$\mu$ から $W$ の制限からの変換によって演繹され、したがって $\alpha$ から $tW$ の制限となります。 したがって、$\varphi(\alpha'_{V'})$は$\alpha$から$V$の制限です。

ある人は、$\alpha$ *はローカルの同型* $\varphi$ によって *$\alpha'$ から推定される* と言います。

#### 例 {#int-vii-s1-n7-exa-1 .statement tag=09DM}

— No. 2、*例 3* で得られた $T$ のハール測度は、$T$ を使用した $R$ のローカル同型によって、$R$ のルベーグ測度から推定できます。

### 8. 比較的不変な尺度

#### 命題 10 {#int-vii-s1-prop-10 .statement tag=09DN}

*$G$を局所的にコンパクトな群、$\mu$を乗数$\chi$を持つ$G$の比較的左不変測度とする。 $\chi_1$ が $\mathbf{C}^*$ の $G$ の連続表現である場合、測度 $\chi_1 \cdot \mu$ は乗数 $\chi_1 \chi$ と相対的に左不変です。*

のために、

$$
\gamma(s)(\chi_1 \cdot \mu) = (\gamma(s)\chi_1) \cdot (\gamma(s)\mu) = (\chi_1(s^{-1})\chi_1) \cdot (\chi(s)^{-1}\mu)
= (\chi_1 \chi)(s)^{-1}(\chi_1 \cdot \mu).
$$

#### 系 1 {#int-vii-s1-prop-10-cor-1 .statement tag=09DO}

*$\mu$を$G$の左ハールメジャーとします。 $G$ の非零測定 $\nu$ が相対的に左不変であるためには、それが形 $a \chi \cdot \mu$ であることが必要かつ十分です。ここで、$a \in \mathbf{C}^*$ と $\chi$ は $\mathbf{C}^*$ の $G$ の連続表現です。その乗数は $\chi$ になります。*

条件で十分です (提案 10)。一方、$\nu$ が乗数 $\chi$ に対して相対的に左不変の測度である非零である場合、$\chi^{-1} \cdot \nu$ は左不変であり (提案 10)、したがって $a \in \mathbf{C}^*$ に対して形 $a \mu$ になります。 (No. 2、Th. 1 の Cor.)。

#### 系 2 {#int-vii-s1-prop-10-cor-2 .statement tag=09DP}

*相対的に左が不変なメジャーはすべて、相対的に右が不変です。*

というのは、コルの記法と。 1、

$$
\delta(s)(\chi \cdot \mu) = (\delta(s)\chi) \cdot (\delta(s)\mu) = (\chi(s)\chi) \cdot (\Delta_G(s)\mu)
= (\chi \Delta_G)(s)(\chi \cdot \mu).
$$

コルのせいで。 2 では、これ以降は、G 上の *比較的不変な測度について、特に説明せずに説明します。比較的不変な測定では、特別な場合として左ハール測定と右ハール測定が認められます。 G に比較的不変な測度 $\nu$ が与えられると、その *左乗数* $\chi$ と、$\gamma(s)\nu = \chi(s)^{-1}\nu$、$\delta(s)\nu = \chi'(s)\nu$ によって定義される *右乗数* $\chi'$ を区別するのが便利です。 (34) までに、これら乗数満たす関係

$$
\chi' = \chi \Delta_G.
$$

まだ $\mu$ で左ハール測度を示しています。

$$
\nu' = (\chi \cdot \mu)' = \dot{\chi} \cdot \dot{\mu} = (\chi^{-1} \Delta_G^{-1}) \cdot \mu,
$$

したがって、$\nu'$ は左乗数 $\chi^{-1} \Delta_G^{-1}$ と右乗数 $\chi^{-1}$ に対して比較的不変です。

無視できる、局所的に無視できる、測定可能、および局所的可積分関数の概念は、比較的不変なすべての尺度で同じです。

### 9. 準不変の尺度

#### 命題 11 {#int-vii-s1-prop-11 .statement tag=09DQ}

*G を局所的にコンパクトな群、G 上の左 Haar 測度 $\mu$ とする。G 上の測度 $\nu \neq 0$ が左準不変であるためには、$\nu$ が $\mu$ と等価であることが必要かつ十分である。*

十分であることは明らかです。 $\nu \neq 0$ を左準不変測度とし、$\nu$ が $\mu$ と同等であることを示します。 $\nu > 0$ の場合に限定できます。 A を G の圧縮部分集合とします。命題を確立するのと同様に、条件 $\mu(A) = 0$、$\nu(A) = 0$ が同等であることを示します (Ch. V, §5, No. 5、Th. 2)。

a) すべての $f \in \mathscr{K}_+(G)$ について、$G \times G$ 上の写像 $(x, y) \mapsto f(x)\varphi_A(xy)$ は、上半連続で有界であり、集合 $K = \operatorname{Supp} f$ の場合、そのサポートがコンパクトな集合 $K \times K^{-1}A$ に含まれるため、$(\nu \otimes \mu)$ 積分可能です。したがって、ルベーグ・フビニ定理により、

$$
\int d\nu(y) \int \varphi_A(xy)f(x)\,d\mu(x) = \int f(x)\,d\mu(x) \int \varphi_A(xy)\,d\nu(y).
$$

b) $\nu(A) = 0$ と仮定します。 仮定により、すべての $x \in G$ に対して $\nu(xA) = 0$ となるため、(36) の右辺は零になります。したがって、$\nu$ が無視できる集合 $N_f$ が存在し、$y \notin N_f$ に対して、

$$
(37) \quad 0 = \int \varphi_A(xy)f(x)\,d\mu(x) = \Delta_G(y)^{-1} \int \varphi_A(x)f(xy^{-1})\,d\mu(x).
$$

B を $\nu(B) \neq 0$ となるような G の圧縮部分集合とし、$\mathscr{K}_+(G)$ の $f$ 写像を $AB^{-1}$ の 1 に等しいものとします。次に、(37) が検証されるような $y \in B$ が存在します。しかし、$y \in B$の$\varphi_A(x)f(xy^{-1}) = \varphi_A(x)$なので、これは$\mu(A) = 0$であることを証明します。

c) $\mu(A) = 0$ と仮定します。次に、すべての $f \in \mathscr{K}_+(G)$ について、(36) の左側は零となり、右側も同様になります。従って、$x \notin M$ に対して $\int \varphi_A(xy)\,d\nu(y) = 0$ となるような局所的に $\mu$ 無視できる集合 M が存在します。 $\mu \neq 0$ 以降、一部の $x \in G$、よって $\nu(A) = 0$ については、$\nu(xA) = 0$ となります。

適用提案 11 から$G^0$ を見ると、右の準不変測度が左の準不変測度と同一であることがわかります。それらは単に G 上の準不変測度と呼ばれます。

### 10. 局所的にコンパクト体

#### 定義 6 {#int-vii-s1-def-6 .statement tag=09DR}

— *K を局所コンパクト体*$^{(1)}$ とします。 *$a \in K^*$ については、a* の法を呼び出し、$\mathrm{mod}_K(a)$ または単に $\mathrm{mod}(a)$ で *自己同型* $x \mapsto ax$ *加法群* $K^+$ *基礎となる K を表します。 1 集合* $\mathrm{mod}(0) = 0$。

#### 例 {#int-vii-s1-n10-exa-1 .statement tag=09DS}

— 1) $K = \mathbf{R}$ としましょう。 $s > 0$ の場合は $s \cdot [0,1] = [0,s]$; $s < 0$、$s \cdot [0,1] = [s,0]$の場合。従って、すべての $t \in \mathbf{R}$ に対して $\mathrm{mod}_\mathbf{R} t = |t|$ となります。

2) $K = \mathbf{Q}_p$ とします。 $s \in \mathbf{Q}_p^*$ が $|s|_p = p^{-n}$ となる場合、$s \mathbf{Z}_p$ は $|x|_p \leq p^{-n}$ となる $x \in \mathbf{Q}_p$ の集合です。従って、$\mu$ が $\mathbf{Q}_p$ の正規化された Haar 測度を表す場合、$\mu(s \mathbf{Z}_p) = p^{-n}$ になります。従って、すべての $t \in \mathbf{Q}_p$ に対して $\mathrm{mod}_{\mathbf{Q}_p} t = |t|_p$ となります。

#### 命題 12 {#int-vii-s1-prop-12 .statement tag=09DT}

— *写像 mod は K 上で連続し、* $\mathrm{mod}(ab) = \mathrm{mod}(a)\mathrm{mod}(b)$ *すべて* $a, b$ *K 内*。

最後の主張は明らかです。 No. 4 の提案 4 は、写像 mod が $K^*$ の点ごとに連続であることを示しています。残るのは 0 での連続性を示すことだけです。これは離散 K では明らかです。従って、K が非離散であると仮定します。 $\alpha$を$K^+$のハール測度とし、Cを$\alpha(C) > 0$となるようなKのコンパクト部分集合とする。 $a \in K^*$ の場合、$\alpha(aC) = \mathrm{mod}(a)\alpha(C)$ があります。

(1) 軍団 (A、I, §9, No. 1)、「師団環」 (GT、III, §6, No. 7) とも訳されます。

K は離散的ではないため、 $\alpha(\{0\}) = 0$ (No. 2、提案 2);従って、$\varepsilon > 0$ ごとに、$\alpha(U) \leq \varepsilon$ のような 0 の開いた近傍 U が存在します。 K の積は連続なので、0 に十分近い $a$ に対して $aC \subset U$ 、次に $\mathrm{mod}(a) \leq \varepsilon / \alpha(C)$ です。

#### 命題 13 {#int-vii-s1-prop-13 .statement tag=09DU}

— *すべての* $M > 0$ について、* $V_M$ * $x \in K$ の集合を * $\mathrm{mod}(x) \leq M$ とします。 *K が非離散の場合、* $V_M$ *形* 0 *in* K のコンパクト近傍の基本系です。

$V_M$ は、提案 12 により 0 の閉じた近傍です。それらがコンパクトであることを示しましょう。 U を 0 のコンパクトな近傍とする。K には、すべての $n > 0$ に対して $\mathrm{mod}(r) < 1$ と $r^n \in U$ となるような $r \neq 0$ が存在する。つまり、W を $WU \subset U$ となる 0 の近傍とする。提案 12 により、K には $\mathrm{mod}(r) < 1$ と $r \in U \cap W$ となる $r \neq 0$ が存在します。次に、$n$の帰納法までに$n > 0$すべてに対して$r^2 \in WU \subset U$、$r^n \in U$が続きます。 $V_M$ が集合 $r^{-q}U$ ($q$ 整数 $\geq 0$) の有限和集合に含まれることを示し、$V_M$ が確かにコンパクトであることを証明します。 $x$ が数列 $(r^n)$ のクラスター 点である場合、$\mathrm{mod}(x)$ は数列 $(\mathrm{mod}(r)^n)$ のクラスター 点であるため、$\mathrm{mod}(x) = 0$、$x = 0$ になります。 U はコンパクトなので、(GT, I, §9, No. 1, Th. 1 の Cor.) $\lim_{n \to \infty} r^n = 0$ になります。では、$a \in V_M$ にしましょう。 数列 $(r^n a)_{n \geq 0}$ は 0 に向かう傾向があるため、$r^n a \in U$ となるような最小の整数 $n \geq 0$ が存在します。 $n > 0$ の場合、$r^{n-1} a \notin U$、したがって $r^n a \in U \cap C(rU)$; $U \cap C(rU)$ の閉包 X は U がコンパクトであるためコンパクトですが、$rU$ は 0 の近傍であるため含む 0 ではありません。したがって、X では、$\mathrm{mod}(x)$ は数 $m > 0$ によって下に制限されます。したがって、$n > 0$ の場合、$m \leq \mathrm{mod}(r^n a)$、よって $\mathrm{mod}(r^{-1})^n \leq M/m$ になります。 $\mathrm{mod}(r^{-1}) > 1$ なので、整数 $n$ は、$a$ に依存せず、値、数の有限の数のみを取ることができ、主張の証明が完成します。

そうなると、$V_M$ 簡約するの共通部分から $\{0\}$ までの $V_M$ 形は 0 の近傍の基本系 (GT、I, §9, No. 2、提案 1) になります。

#### 系 {#int-vii-s1-n10-cor-1 .statement tag=09DV}

— *位相の非離散局所コンパクト体は可算基底を許容します。*

なぜなら、K はコンパクト集合 $V_1, V_2, \ldots$ の和集合です。一方、K は GT の提案 1 IX, §3, No. 1 により計量化可能です。したがって、K の位相は可算基底を認めます (*上記引用*、§2, No. 9、提案 16 の訂正)。

#### 命題 14 {#int-vii-s1-prop-14 .statement tag=09DW}

— *$\alpha$ *$K^+$ のハール測度としましょう。 *次に、小節* $\beta = (\mathrm{mod}_K)^{-1} \cdot \alpha$ *on* $K^*$ *は、乗法群* $K^*$ の左ハール小節です。

たとえば、$b \in K^*$ の場合、K の写像 $a \mapsto b^{-1} a$ を K に変換し、変換 $\alpha$ を $(\mathrm{mod}_K b) \alpha$ に変換するため、$(\mathrm{mod}_K)^{-1} \cdot \alpha$ 自体がよって命題になります。

#### 系 {#int-vii-s1-n10-cor-2 .statement tag=09DX}

— *f を * $K^*$ に * 写像を定義し、 * $\overline{\mathbf{R}}$ * または Banach 空間で値を使用します。 * f *が $\beta$-*可積分であるためには、 $(\mathrm{mod}_K)^{-1} f$ が $\alpha$-可積分であることが必要かつ十分*であり、その場合

$$
\int_{K^*} f(x) d\beta(x) = \int_{K^+} (\mathrm{mod}_K(x))^{-1} f(x) d\alpha(x).
$$

これは、Cor. の提案 14 に従っています。提案 13、および第 6 章V, §5, No. 3、木曜日。 1.

#### 命題 15 {#int-vii-s1-prop-15 .statement tag=09DY}

— *K が可換であると仮定します。あなたをベクトル空間の自己同型 E = K^n とします。それから*

$$
\mathrm{mod}_E u = \mathrm{mod}_K(\det u).
$$

$u$ が $\mathbf{GL}(E)$ の生成元の系を超えるとき、公式を検証するだけで十分です。ここで、$\mathbf{GL}(E)$ は次の元 (A、II, §10, No. 13、提案 14 の Cor. 2) によって生成されます。
(a) 元 $u_1$/形

$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$

ここで$\sigma \in \mathfrak{S}_n$;
(b) 元 $u_2$/形

$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n)
$$

$a \in K^*$付き。
(c) 元 $u_3$ の形

$$
(x_1, \ldots, x_n) \mapsto (x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n).
$$

$f \in \mathscr{H}(E)$ の場合、$K^+$ でのハール測度を $\alpha$ で表すと、

$$
\int \cdots \int_{K^n} f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1) d\alpha(x_2) \ldots d\alpha(x_n)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^n} f(x_1, \ldots, x_n) d\alpha(x_1) \ldots d\alpha(x_n),
$$

一方、$\mathrm{mod}_K(\det u_3) = \mathrm{mod}_K(1) = 1$、よっては $u_3$ の結果です。 $u_1$ と $u_2$ についても同様の方法で確立されます。

K を可換局所コンパクト体、K 上の有限次元 n の E ベクトル空間とする。$\varphi$ がベクトル空間 $K^n$ の同型をベクトル空間 E にすると、$\varphi$ 変換 $K^n$ の位相を E 上の位相に変換すると、E は局所的にコンパクトなベクトル空間になります。この位相 (正規と呼ばれます) は、ベクトル空間 $K^n$ のすべての自己同型が共連続であるため、$\varphi$ から独立しています。逆の明示的な言及がない限り、E をトポロジカルなベクトル空間として話すとき、位相は常に今定義されたものであると理解されます。 ベクトル空間 E のすべての自己同型 u は共連続であるため、$\mathrm{mod}_E u$ が定義されます。一方、u が E の非可逆自己準同型である場合、1 つの集合 $\mathrm{mod}_E u = 0$。次に:

#### 系 1 {#int-vii-s1-prop-15-cor-1 .statement tag=09DZ}

— *K を可換局所コンパクト体、K 上の E 有限次元ベクトル空間、およびベクトル空間 E の u 自己準同型とします。すると* $\mathrm{mod}_E(u) = \mathrm{mod}_K(\det u)$。

u が可逆であれば、これは提案 15 から導き出されます。u が可逆でない場合は、$\det u = 0$、したがって $\mathrm{mod}_K(\det u) = 0 = \mathrm{mod}_E u$ になります。

#### 系 2 {#int-vii-s1-prop-15-cor-2 .statement tag=09E0}

— *E を有限次元 n の実数ベクトル空間、E の $(e_1, e_2, \ldots, e_n)$ 基底、* $x = \sum_{i=1}^n \xi_i e_i \in E$ * の P 集合 *そのような* $0 \leq \xi_i \leq 1$ *すべての i* 、および $\mu$ * 上の固有のハール測度であるとします。 加法群 E そのような* $\mu(P) = 1$。 *$x_1, \ldots, x_n$ *を E の点とし、S を集合* $\{0, x_1, \ldots, x_n\}$ の E にある閉じた凸包絡線とします。 *書き込み中* $x_i = \sum_{j=1}^n \alpha_{ij} e_j$、*1人が持っています*

$$
\mu(S) = \mu(\dot{S}) = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

同型を使って同一視する E と $\mathbf{R}^n$ を変換 $(e_i)$ から $\mathbf{R}^n$ の標準基底に変換します。次に、$\mu$ は、$\mathbf{R}^n$ 上のルベーグ測度 $\mu_n$ と識別されます。

まず、すべての i が $x_i = e_i$ であると仮定します。すると、S は $\mathbf{R}^n$ の $x = (\xi_i)$ の集合 $S_n$ となり、次のようになります。

$$
\xi_i \geq 0 \text{ for all } i \quad \text{and} \quad \xi_1 + \cdots + \xi_n \leq 1.
$$

集合 $\mu_n(S_n) = a_n$。 $\lambda \in \mathbf{R}$ にしましょう。 $\mathbf{R}^n$ を $\mathbf{R}^{n-1} \times \mathbf{R}$ と同一視すると、$\lambda$ で $S_n$ の切断 $C_\lambda$ を考慮できます。 $\lambda < 0$ または $\lambda > 1$ の場合、この切断は空です。 $0 \leq \lambda \leq 1$、$C_\lambda$ が $(\xi_1, \ldots, \xi_{n-1}) \in \mathbf{R}^{n-1}$ の集合である場合、次のようになります

$$
\xi_1 \geq 0, \ldots, \xi_{n-1} \geq 0, \quad \xi_1 + \cdots + \xi_{n-1} \leq 1 - \lambda,
$$

したがって、$S_{n-1}$ から比率 $1 - \lambda$ のホモテティー によって、$\mu_{n-1}(C_\lambda) = (1 - \lambda)^{n-1} a_{n-1}$ が演繹される可能性があります。ルベーグ・フビニ定理より、

$$
a_n = \int_0^1 (1 - \lambda)^{n-1} a_{n-1} d\lambda = \frac{1}{n} a_{n-1}.
$$

$a_1 = 1$ なので、$a_n = \frac{1}{n!}$ であることがわかります。

系の一般的なケースに戻りましょう。 $u$ を、すべての $i$ に対して $u(e_i) = x_i$ となるように、$\mathbf{R}^n$ の自己準同型とします。 1 つは$u(S_n) = S$ です。 $u$ が可逆である場合、提案 15 は次のことを証明します。

$$
\mu_n(S) = \frac{1}{n!} |\det u| = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

$S - \overset{\circ}{S}$は超平面の有限数に含まれるので、$\mu(\overset{\circ}{S}) = \mu(S)$です。最後に、$u$ が可逆でない場合、$S$ は超平面に含まれるため、$\mu(S) = 0 = \det(\alpha_{ij})$ になります。

### 11. 局所的にコンパクトな体上の有限次元代数

$K$ を可換体、$A$ を有限階数と単位元元の $K$-代数とします。すべての $a \in A$ について、$L_a, R_a$ をベクトル空間 $A$ の自己準同型 $x \mapsto ax$、$x \mapsto xa$ とし、$N_{A/K}(a) \in K$、$N_{A^0/K}(a) \in K$ を正則表現の $a$ のノルムとします。 $A$ と反対多元環 $A^0$; $N_{A/K}(a) = \det(L_a)$、$N_{A^0/K}(a) = \det(R_a)$ (A、III, §9, No. 3) を思い出してください。次の条件は同等です: $a$ 反転可能、$L_a$ $\mathrm{Hom}_K(A, A)$ で反転可能、$R_a$ $\mathrm{Hom}_K(A, A)$、$N_{A/K}(a) \neq 0$、$N_{A^0/K}(a) \neq 0$ で反転可能。 $A^*$ 集合可逆元 $A$ で表します。

ここで、体 $K$ が局所的にコンパクトであると仮定します。したがって、代数 $A$ は局所的にコンパクトであると仮定します。すると、$N_{A/K}$と$N_{A^0/K}$は$A$の写像から$K$に連続するため、$A^*$は$A$でオープンになります。コル著No. 10の提案15の1、

$$
\mathrm{mod}_A L_a = \mathrm{mod}_K N_{A/K}(a), \quad \mathrm{mod}_A R_a = \mathrm{mod}_K N_{A^0/K}(a).
$$

#### 命題 16 {#int-vii-s1-prop-16 .statement tag=09E1}

— *$\alpha$を$A$の加法群のハール測度とする。対策*

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha(a), \quad (\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha(a)
$$

* $A^*$ は、それぞれ乗法群 $A^*$ の左ハール測定値と右ハール測定値です。

$\alpha'$ を $\alpha$ の制限からオープン集合 $A^*$ とします。 $a \in A^*$ の場合、$L_a(\alpha') = (\mathrm{mod}_K N_{A/K}(a))^{-1} \alpha'$ があるため、$(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha'(a)$ は $A^*$ の左ハール測度です (No. 8、提案 10 の Cor. 1)。 移行から反対多元環を見ると、$(\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha'(a)$ が $A^*$ の右ハール測度であることがわかります。

#### 命題 17 {#int-vii-s1-prop-17 .statement tag=09E2}

— *A が体 (局所的にコンパクト) であると仮定します。 $a \in A$、$\mathrm{mod}_A(a) = \mathrm{mod}_K N_{A/K}(a)$ごとに。*

(38) の最初の公式の翻訳です。

#### 例 {#int-vii-s1-n11-exa-1 .statement tag=09E3}

— 1) $K = \mathbf{R}$、$A = \mathbf{C}$ を取ります。 *Alg.* を考慮して、第 3 章を参照してください。 VIII, §12、番号 2、支柱。 4、すべての$z \in \mathbf{C}$に対して$\mathrm{mod}_\mathbf{C}(z) = |z|^2$を取得します。 (2)

2) $K = \mathbf{R}$ をとり、A については *四元数体* $\mathbf{H}$ (GT, VIII, §1, No. 4) をとります。次の $\mathbf{M}_2(\mathbf{C})$ の元を考慮してください。

$$
X_1 = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix} \quad X_2 = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \quad X_3 = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}
$$

これは、$\mathbf{C}$ の上に $\mathbf{M}_2(\mathbf{C})$ の $I_2$、形基底が加わります。それは簡単に検証できます

$$
X_1^2 = X_2^2 = X_3^2 = -I_2, \qquad X_1 X_2 = -X_2 X_1 = X_3,
$$
$$
X_2 X_3 = -X_3 X_2 = X_1, \qquad X_3 X_1 = -X_1 X_3 = X_2.
$$

したがって、写像 $a + b i + c j + d k \mapsto a I_2 + b X_1 + c X_2 + d X_3$ は、代数 $\mathbf{C} \otimes_\mathbf{R} \mathbf{H}$ の代数 $\mathbf{M}_2(\mathbf{C})$ の $\mathbf{C}$ 同型写像に拡張できます。 $[\mathbf{H} : \mathbf{R}] = 4$ なので、$\mathbf{C}$ は $\mathbf{H}$ の体 (*Alg.*、章 VIII, §10、n° 5) であり、$q = a + b i + c j + d k \in \mathbf{H}$ の被約ノルムは

$$
\mathrm{Nrd}(q) = \det(a I_2 + b X_1 + c X_2 + d X_3)
$$
$$
= \det \begin{pmatrix} a + i d & -c + i b \\ c + i b & a - i d \end{pmatrix} = a^2 + b^2 + c^2 + d^2 = \|q\|^2.
$$

*Alg.* による、第 4 章VIII, §12、番号 3、支柱。 8、1つは持っています

$$
\mathrm{N}_{\mathbf{H}/\mathbf{R}}(q) = (\mathrm{Nrd}_{\mathbf{H}/\mathbf{R}}(q))^2 = \|q\|^4.
$$

これは、提案 17 が次のことを示していると述べています。

$$
\mathrm{mod}_\mathbf{H}(q) = \|q\|^4.
$$

局所的にコンパクトな体の構造のより深い研究は、CA、VI, §9で行われます。

(2) これもコルから導き出されます。提案 15 の 1 と、$z = a + i b$ による左乗算は、$\mathbf{R}$ に対する $\mathbf{C}$ の標準基底 $1, i$ に関して行列 $\begin{pmatrix} a & -b \\ b & a \end{pmatrix}$ となるという事実。

### 練習問題 {#int-vii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
