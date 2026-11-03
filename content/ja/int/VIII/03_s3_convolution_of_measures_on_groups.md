---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 3
section_title: Convolution of measures on groups
lang: ja
source: int-vii-ix
book_pages: INT VIII.18-INT VIII.24, INT VIII.61-INT VIII.65
pdf_pages: 0118-0124, 0161-0165
extraction: ocr
subsections:
    - "no": 1
      title: Algebras of measures
      page: 18
      pdf_page: 118
    - "no": 2
      title: The case of a group operating on a space
      page: 21
      pdf_page: 121
    - "no": 3
      title: Convolution and linear representations
      page: 22
      pdf_page: 122
statements: 16
exercises: 13
content_sha256: ef17c71def5d96fd6003a19cb2a526e6619abff094bc895c4959e2e7322797f8
translated_from: content/en/int/VIII/03_s3_convolution_of_measures_on_groups.md
translation_method: google
source_content_sha256: fbb17d2d8dfca6f7e44cfa7592c87c0769532c38cc2550dc3a50ed837fd6ab29
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1fdddacf71539469be2504a767a035da4782491228409949ac6000717b81fca3
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。 群でのメジャーの畳み込み

### 1. 対策の代数

G を局所コンパクト群とします。 G の測度 $\mu_1, \ldots, \mu_n$ は、写像についても同様である場合、畳み込み可能であると言われることが、きっぱりと理解されるでしょう。

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \cdots x_n;
$$

そして、この写像によって、畳み込み積 $*_{i} \mu_i$ が常に取得されます。 $s \in G, t \in G$ の場合、

(1)
$$
\varepsilon_s * \varepsilon_t = \varepsilon_{st}.
$$

$s \in G$ と $\mu \in \mathscr{M}(G)$ の場合、

(2)
$$
\varepsilon_s * \mu = \gamma(s) \mu
$$
(3)
$$
\mu * \varepsilon_s = \delta(s^{-1}) \mu
$$

by §1, No. 1, 例 3. G がアーベルの場合、$\mu_1$ と $\mu_2$ が畳み込み可能であると言うのは、$\mu_2$ と $\mu_1$ が畳み込み可能であるというというと同等であり、その場合、1 つは $\mu_1 * \mu_2 = \mu_2 * \mu_1$ になります。 G がアーベルではない場合、$\mu_2$ と $\mu_1$ は畳み込み可能ではなく、$\mu_1$ と $\mu_2$ は畳み込み可能であることが起こります (Exer. 12)。

#### 命題 1 {#int-viii-s3-prop-1 .statement tag=09JB}

— G を局所コンパクト群とし、$\lambda, \mu, \nu$ は G 上の $\neq 0$ を測定します。

(i) $\lambda, \mu, \nu$ が畳み込み可能であれば、$\lambda$ と $\mu$、$|\lambda| * |\mu|$ と $\nu$、$\mu$ と $\nu$、$\lambda$ と $|\mu| * |\nu|$ も畳み込み可能です。

$$
\lambda * \mu * \nu = (\lambda * \mu) * \nu = \lambda * (\mu * \nu).
$$

(ii) $\lambda$ と $\mu$ が、$|\lambda| * |\mu|$ と $\nu$ と同様に畳み込み可能である場合、$\lambda, \mu, \nu$ も畳み込み可能です。同様に、$\mu$ と $\nu$、および $\lambda$ と $|\mu| * |\nu|$ が畳み込み可能である場合も同様です。

これは、§1, No. 2 の提案 1 に続きます。

畳み込み積 $\lambda * \mu$、$(\lambda * \mu) * \nu$、$\mu * \nu$、$\lambda * (\mu * \nu)$ がすべて定義されているにもかかわらず、$(\lambda * \mu) * \nu \neq \lambda * (\mu * \nu)$ (cf. Exer. 4) となるような G 上のメジャー $\lambda, \mu, \nu$ が存在する可能性があります。

$\rho$ を、$G$ のすべての $s, t$ に対して $\rho(st) \leq \rho(s)\rho(t)$ となるような、$G$ における下位の半連続有限写像 $> 0$ とします。 $\rho$ が $\lambda$ 可積分となるような $G$ の測度 $\lambda$ の $\mathscr{M}^\rho(G)$ ベクトル空間を、これに対する $\| \lambda \|_\rho$ (または単に $\| \lambda \|$) ノルム $\int_G \rho(s) d|\lambda|(s)$ で表します。 空間。 $\rho = 1$ のとき、$G$ に制限付きメジャーの集合 $\mathscr{M}^1(G)$ を回復します。

#### 命題 2 {#int-viii-s3-prop-2 .statement tag=09JC}

(i) *$\mathscr{M}^\rho(G)$ の任意の 2 つの元は畳み込み可能です。*
(ii) *畳み込みの場合、およびノルム $\| \lambda \|$ の場合、$\mathscr{M}^\rho(G)$ は完全な正規化代数であり、$\varepsilon_e$ を単位元元として認めます。*
(iii) $\mathscr{C}'(G)$ * は $\mathscr{M}^\rho(G)$* の部分代数です。

$\lambda, \mu$ が $\mathscr{M}^\rho(G)$ にあるとして、$\lambda$ と $\mu$ が畳み込み可能であることを示します。 $f \in \mathscr{K}_+(G)$ にしましょう。 $\rho$は$> 0$以下の半連続なので、$f \leq k\rho$となるような定数$k > 0$が存在します。それから

$$
\int^* f(st) d|\lambda|(s) d|\mu|(t) \leq k \int^* \rho(st) d|\lambda|(s) d|\mu|(t)
$$
$$
\leq k \int^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= k \left( \int^* \rho(s) d|\lambda|(s) \right) \left( \int^* \rho(t) d|\mu|(t) \right)
$$

(Ch. V, §8, No. 3、提案 8 の Cor. 1)。したがって、$(s,t) \mapsto f(st)$ は $(\lambda \otimes \mu)$ 積分可能であるため、$\lambda$ と $\mu$ は畳み込み可能です。一方、Ch. V (§1、提案 4、§6、提案 2、§8、提案 8 の訂正 1)、および $(s,t) \mapsto \rho(s)\rho(t)$ が $G \times G$ の下位半連続であるという事実により、

$$
\int_G^* \rho(s) d|\lambda * \mu|(s) = \int_G^* \rho(s) d|\lambda * \mu|(s)
$$
$$
\leq \int_{G \times G}^* \rho(st) d|\lambda|(s) d|\mu|(t) \leq \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t) = \| \lambda \| \cdot \| \mu \|.
$$

$\lambda * \mu \in \mathscr{M}^\rho(G)$ と $\| \lambda * \mu \| \leq \| \lambda \| \cdot \| \mu \|$ がわかります。提案 1 を考慮すると、$\mathscr{M}^\rho(G)$ は代数になります。 写像 $\lambda \mapsto \rho \cdot \lambda$ は、$\mathscr{M}^\rho(G)$ を $\mathscr{M}^1(G)$ に等角投影した線形写像 $\theta$ です。 $\mu \in \mathscr{M}^1(G)$ の場合、局所的に有界で上部半連続である $1/\rho$ は局所的に $\mu$ 積分可能であり、$\rho$ は $(1/\rho) \cdot \mu$ 積分可能であるため、$(1/\rho) \cdot \mu \in \mathscr{M}^\rho(G)$ になります。これは、$\theta$ が全射であることを証明します。したがって、$\mathscr{M}^\rho(G)$ は完全な標準である代数です。最後に、$\varepsilon_e$ は $\mathscr{M}^\rho(G)$ の単位元元であり、$\mathscr{C}'(G)$ は $\mathscr{M}^\rho(G)$ の部分代数であることが明らかです (提案 5 の§1, No. 4)。

$\rho = 1$ の場合、提案 2、(i) および (ii) も、§1、提案 2 に従います。

#### 命題 3 {#int-viii-s3-prop-3 .statement tag=09JD}

*$\mu_1, \ldots, \mu_n$ を G 上のメジャーとします。多くても 1 つを除くすべての $\mu_i$ がコンパクト サポートを持っている場合、$\mu_i$ は畳み込み可能です。

なぜなら、$S_i$ を $\mu_i$ のサポートとし、$S_i$ が $i \neq i_0$ に対してコンパクトであると仮定します。 K を G の圧縮部分集合とします。 すべての $i$、$x_1 x_2 \cdots x_n \in K$ に対して条件 $x_i \in S_i$ が意味するため、$x_1 x_2 \cdots x_n \in K$ がコンパクトになるような $(x_1, \ldots, x_n) \in \prod_i S_i$ の集合

$$
x_{i_0} \in S_{i_0-1}^{-1} \cdots S_1^{-1} K S_n^{-1} \cdots S_{i_0+1}^{-1} .
$$

したがって、$\mu_i$ は畳み込み可能です (§1, No. 4、提案 4)。

#### 命題 4 {#int-viii-s3-prop-4 .statement tag=09JE}

*写像 $(\lambda, \mu) \mapsto \lambda * \mu$ (それぞれ $(\lambda, \mu) \mapsto \mu * \lambda$)、ここで、$\lambda \in \mathscr{C}'(G)$、$\mu \in \mathscr{M}(G)$、定義するは、代数 $\mathscr{C}'(G)$ の上の$\mathscr{M}(G)$ 構造 (それぞれ右) 加群です。*

これは Props からの続きです。 1と3。

#### 命題 5 {#int-viii-s3-prop-5 .statement tag=09JF}

*$\lambda$ を G の左 (右) ハール測度、$\mu \in \mathscr{M}^1(G)$ とします。次に、$\mu$ と $\lambda$ (それぞれ $\lambda$ と $\mu$) は畳み込み可能で、$\mu * \lambda = \mu(1)\lambda$ (それぞれ $\lambda * \mu = \mu(1)\lambda$) は畳み込み可能です。*

$\mu \geqslant 0$ と仮定できます。 $f \in \mathscr{K}_+(G)$ にしましょう。 $\lambda$ が左ハール測度の場合、

$$
\int^* d\mu(x) \int^* f(xy)\, d\lambda(y) = \int^* d\mu(x) \int f(y)\, d\lambda(y) = \lambda(f)\|\mu\| ,
$$

したがって、写像 $(x, y) \mapsto f(xy)$ は $(\mu \otimes \lambda)$ 積分可能であり、$\mu \otimes \lambda$ の積分は $\lambda(f)\|\mu\|$ です。 $\lambda$ が正しいハール尺度である場合も同様に議論されます。

#### 命題 6 {#int-viii-s3-prop-6 .statement tag=09JG}

*$\mu$ と $\nu$ を G 上の 2 つの畳み込み可能なメジャーとします。 $\chi$ を $\mathbf{C}^*$ の G の連続する表現とします。次に、$\chi \cdot \mu$ と $\chi \cdot \nu$ は畳み込み可能で、$(\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu)$* になります。

$f \in \mathscr{K}(G)$ にしましょう。すると $f\chi \in \mathscr{K}(G)$、したがって写像

$$
(x, y) \mapsto f(xy)\chi(xy) = f(xy)\chi(x)\chi(y)
$$

$G \times G$ は $\mu \otimes \nu$ に対して積分可能です。したがって、写像 $(x, y) \mapsto f(xy)$ は $(\chi \cdot \mu) \otimes (\chi \cdot \nu)$ に対して積分可能です。したがって、$\chi \cdot \mu$ と $\chi \cdot \nu$ は畳み込み可能です。さらに、

$$
\langle \chi \cdot \mu * \chi \cdot \nu, f \rangle = \int f(xy)\chi(x)\chi(y)\, d\mu(x)\, d\nu(y)
= \int (f\chi)(xy)\, d\mu(x)\, d\nu(y) = \langle \mu * \nu, \chi f \rangle ,
$$

よって $(\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu)$。

#### 命題 7 {#int-viii-s3-prop-7 .statement tag=09JH}

*G と G' を 2 つの局所的にコンパクトな群、U を G' 内の G の連続表現、G 上の $\mu_1, \ldots, \mu_n$ 小節、すべて $\neq 0$ とします。したがって、次の主張は同等です。
(i) $u$ はすべての i に対して $\mu_i$ が適切であり、尺度 $u(|\mu_i|)$ は畳み込み可能です。
(ii) $\mu_i$ は畳み込み可能であり、$u$ は $*_{i}(|\mu_i|)$ に対して適切です。
これら条件が満たされると、

$$
*_{i} u(\mu_i) = u(*_{i} \mu_i).
$$

これは、§1, No. 2、Cor. からの続きです。提案 1 の。

#### 系 {#int-viii-s3-n1-cor-1 .statement tag=09JI}

*G を局所的にコンパクトな群、$\mu_1, \ldots, \mu_n$ の G 上の測定値とする。数列 $(\mu_i)_{1 \leq i \leq n}$ が畳み込み可能であるためには、数列 $(\check{\mu}_{n-i})_{0 \leq i \leq n-1}$ が畳み込み可能であることが必要かつ十分であり、その場合*

$$
(\mu_1 * \cdots * \mu_n)^{\vee} = \check{\mu}_n * \cdots * \check{\mu}_1.
$$

これは、G の同型 $x \mapsto x^{-1}$ を反対側の群に考慮するという提案 7 から続きます。

### 2. 群が空間で動作する場合

X を局所コンパクト空間とし、その上で局所コンパクト群 G が左に連続的に作用するようにします。

$$
(s, x) \mapsto s \cdot x.
$$

$\mu_1, \ldots, \mu_n$ が G 上のメジャーであり、$\nu$ が X 上のメジャーである場合、$G^n \times X$ の $(s_1, \ldots, s_n, x) \mapsto s_1 \cdots s_n x$ を X にマッピングする場合、これらは畳み込み可能であると言われ、それらの畳み込み積はこのマッピングの意味で理解されます。

$s \in G$ と $x \in X$ の場合、

(4)
$$
\varepsilon_s * \varepsilon_x = \varepsilon_{sx}.
$$

$s \in G$ と $\mu \in \mathscr{M}(X)$ の場合、

(5)
$$
\varepsilon_s * \mu = \gamma(s)\mu
$$
§1, No. 1、例 3 より。

#### 命題 8 {#int-viii-s3-prop-8 .statement tag=09JJ}

— $\mu$ を $G$ のメジャー、$\nu$ を $X$ のメジャーとします。
(i) $\mu$ がコンパクトなサポートを持っている場合、$\mu$ と $\nu$ は畳み込み可能です。
(ii) $\nu$ がコンパクトなサポートを持ち、$G$ が $X$ で適切に動作する場合、$\mu$ と $\nu$ は畳み込み可能です。
これは§1, No. 4の提案4から続きます。

#### 命題 9 {#int-viii-s3-prop-9 .statement tag=09JK}

— 畳み込みの場合、$\mathscr{M}^1(X)$ は $\mathscr{M}^1(G)$ に対する左加群であり、$\mathscr{M}(X)$ と $\mathscr{C}'(X)$ は $\mathscr{C}'(G)$ に対する左加群です。
これは、提案 8 と、§1 の提案に続きます。 1、3、およびコル。提案 5 の。

#### 命題 10 {#int-viii-s3-prop-10 .statement tag=09JL}

— $\mu$ を $G$ のメジャー、$\nu$ を $X$、$\mu$、および $\nu$ のメジャーとし、畳み込み可能とします。 加法で、$X$ に正の測度 $\beta$ が存在し、$\gamma(s)\nu$ が $s \in G$ ごとに基底 $\beta$ になるとします。すると、$\mu * \nu$ は基底 $\beta$ になります。
$K$を$X$の$\beta$-無視できるコンパクト部分集合とする。すると、$K$ は、$s \in G$ ごとに $\gamma(s)|\nu|$ が無視できます。さて、
$$
|\mu| * |\nu| = \int_G (\varepsilon_s * |\nu|) d|\mu|(s)
$$
(§1, No. 5、提案 7)、写像 $s \mapsto \varepsilon_s * |\nu|$ は漠然と連続しています (§2、提案 6)。したがって、$K$ は Ch によって $|\mu| * |\nu|$ が無視できます。 V, §3, No. 3、木曜日。 1. したがって、$|\mu| * |\nu|$ は基底 $\beta$ になります (Ch. V, §5, No. 5、Th. 2)。

### 3. コンボリューションと線型表現

#### 命題 11 {#int-viii-s3-prop-11 .statement tag=09JM}

— $G$ を局所コンパクト群、$E$ 準完全局所凸空間、$U$ を $E$ における $G$ の連続表現とする。
(i) $\lambda \in \mathscr{C}'(G)$、$\mu \in \mathscr{C}'(G)$ の場合、$U(\lambda * \mu) = U(\lambda)U(\mu)$。
(ii) $E$ がバナハ空間であると仮定し、$s \in G$ を $\rho(s) = \|U(s)\|$ とします。 $\lambda \in \mathscr{M}^\rho(G)$、$\mu \in \mathscr{M}^\rho(G)$の場合は、$U(\lambda * \mu) = U(\lambda)U(\mu)$。
$\lambda, \mu$ を $\mathscr{C}'(G)$ に入れます。 $x \in E$ については、適用までに特に Props を持っています。第 1 章と第 4 章VI, §1, No. 1、
$$
U(\lambda * \mu)x = \int_G U(s)x\, d(\lambda * \mu)(s)
$$
$$
= \int_{G \times G} U(st)x\, d\lambda(s)\, d\mu(t) = \int_{G \times G} U(s)U(t)x\, d\lambda(s)\, d\mu(t)
$$
$$
= \int_G U(\lambda)U(t)x\, d\mu(t) = U(\lambda) \int_G U(t)x\, d\mu(t) = U(\lambda)U(\mu)x ,
$$
よって (i)。同様の議論が (ii) の場合にも適用されます。

G が局所的にコンパクトな群のままで、G が局所的にコンパクトな空間 X 内で左側で連続的に動作すると仮定します。この定義する(§2, No. 4)は$\mathscr{M}(X)$のGの連続線型表現$\gamma$($\mathscr{H}(X)$にはコンパクトコンバージェンスの位相を搭載)です。

#### 命題 12 {#int-viii-s3-prop-12 .statement tag=09JN}

*$\lambda \in \mathscr{C}'(G)$ と $\mu \in \mathscr{M}(X)$ の場合、*

$$
\gamma(\lambda)\mu = \lambda * \mu.
$$

§1, No. 5の提案7により、

$$
\lambda * \mu = \int_G (\varepsilon_s * \mu) d\lambda(s).
$$

さて、$\varepsilon_s * \mu = \gamma(s)\mu$ (No. 2, 公式 (5)) と

$$
\int_G (\gamma(s)\mu) d\lambda(s) = \gamma(\lambda)\mu
$$

$\gamma(\lambda)$の定義による。

#### 系 {#int-viii-s3-n3-cor-1 .statement tag=09JO}

*$\mathscr{C}'(G) \times \mathscr{M}(X)$の$(\lambda, \mu) \mapsto \lambda * \mu$の$\mathscr{M}(X)$へのマッピングは、$\mathscr{C}'(G)$の等連続サブセットおよび$\mathscr{M}(X)$のコンパクトサブセットと比べて非連続です（$\mathscr{C}'(G)$と$\mathscr{M}(X)$には$\mathscr{C}(G)$と$\mathscr{H}(X)$のコンパクト収束のトポロジーが装備されており、それぞれ）。*

というのは、$\mathscr{M}(X)$は$\mathscr{H}(X)$にコンパクトコンバージェンスの位相を搭載して、準完成品です。したがって、$\mathscr{C}'(G) \times \mathscr{M}(X)$ の $\mathscr{M}(X)$ への写像 $(\lambda, \mu) \mapsto \gamma(\lambda)\mu$ は、$\mathscr{C}'(G)$ の等連続部分集合および$\mathscr{M}(X)$ (§2, No. 6) のコンパクトな部分集合と比較して非連続です。その場合、提案 12 を適用すれば十分です。

#### 注意 {#int-viii-s3-n3-rem-1 .statement tag=09JP}

— 1) $\lambda_0 \in \mathscr{C}'(G)$ とします。 $\mathscr{M}(X)$ から $\mathscr{M}(X)$ への写像 $\mu \mapsto \lambda_0 * \mu$ は漠然と連続しています。というのは、$f \in \mathscr{H}(X)$としましょう。 1つは持っています

$$
\langle \lambda_0 * \mu, f \rangle = \int f(sx) d\lambda_0(s) d\mu(x) = \langle \mu, g \rangle,
$$

どこで$g(x) = \int f(sx) d\lambda_0(s)$。現在、$g$ は連続しています (Ch. VII, §1, No. 1、補題 1)。一方、S を$\lambda_0$ のサポート、K を$f$ のサポートとします。 条件 $sx \in K$ と $s \in S$ は $x \in S^{-1}K$ を暗示します。したがって、$g$ のサポートは $S^{-1}K$ に含まれるため、$g \in \mathscr{H}(X)$ になります。すると、$\langle \lambda_0 * \mu, f \rangle = \langle \mu, g \rangle$ は$\mu$ の漠然と連続した写像であり、主張であることが証明されます。

2) $\mu_0 \in \mathscr{M}(X)$ とします。 写像 $\mathscr{C}'(G)$ から $\mathscr{M}(X)$ への $\lambda \mapsto \lambda * \mu_0$ は、トポロジ $\sigma(\mathscr{C}'(G), \mathscr{C}(G))$ と $\sigma(\mathscr{M}(X), \mathscr{H}(X))$ で連続しています。というのは、$f \in \mathscr{K}(X)$としましょう。 設定 $h(s) = \int f(sx)\, d\mu_0(x)$、$\langle f, \lambda * \mu_0 \rangle = \langle h, \lambda \rangle$、$h \in \mathscr{C}(G)$ があります (Ch. VII, §1, No. 1、補題 1)。

#### 命題 13 {#int-viii-s3-prop-13 .statement tag=09JQ}

*写像* $(s, \mu) \mapsto \gamma(s)\mu$ *of* $G \times \mathscr{M}_+(X)$ *into* $\mathscr{M}_+(X)$ *は、集合* $\mathscr{M}_+(X)$ *ポジティブ対策の* $X$ *曖昧な位相* が装備されている場合に連続します。

$\gamma(s)\mu = \gamma(ss_0^{-1})\gamma(s_0)\mu$ なので、*注意 1* から、形 $(e, \mu_0)$ の点で検討中の写像と $\mu_0 \in \mathscr{M}_+(X)$ の連続性を証明すれば十分であることがわかります。 写像 $f \in \mathscr{K}(X)$ と数 $\varepsilon > 0$ を考えると、関係 $s \in U, \mu \in W$ が意味するように、G の e の近傍 U と $\mathscr{M}_+(X)$ の $\mu_0$ の近傍 W が存在することを示すことになります。

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon .
$$

V を X の $f$ のサポート K のコンパクトな近傍とし、$\varphi \in \mathscr{K}_+(X)$ を V 上の $\varphi(x) = 1$ となるようにします。 $a = \sup_{\mu \in W_0} \mu(V)$ が有限となるような $\mathscr{M}_+(X)$ の $\mu_0$ の近傍 $W_0$ が存在します。 $|\langle \varphi, \mu - \mu_0 \rangle| \leq 1$ となるような $\mu \in \mathscr{M}_+(X)$ の $W_0$ 集合をとれば十分です。 写像 $(s, x) \mapsto sx$ は連続であるため、一方で、すべての $s \in U_0$ に対して $sK \subset V$ となるような、G の e のコンパクトな近傍 $U_0$ が存在します。 写像 $(s, x) \mapsto f(sx)$ は $U_0 \times V$ で一様連続であるため、すべての $s \in U$ と $x \in V$ に対して $|f(sx) - f(x)| \leq \varepsilon / 2a$ となるような e の近傍 $U \subset U_0$ が存在します。したがって、$s \in U$ と $\mu \in W_0$ については、

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu(x) \right| \leq \varepsilon / 2 ;
$$

$W \subset W_0$ が $\mu \in W_0$ によって$\left| \int f(x)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon / 2$ となるように形成された $\mathscr{M}_+(X)$ の $\mu_0$ の近傍である場合、U と W は要件を満たします。

### 練習問題 {#int-viii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
