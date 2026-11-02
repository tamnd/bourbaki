---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 9
section_title: Affine spaces and projective spaces
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 325-337, 410-417
pdf_pages: 0349-0361, 0434-0441
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AFFINE SPACES
      page: 325
      pdf_page: 349
    - "no": 2
      title: BARYCENTRIC CALCULUS
      page: 326
      pdf_page: 350
    - "no": 3
      title: AFFINE LINEAR VARIETIES
      page: 327
      pdf_page: 351
    - "no": 4
      title: AFFINE LINEAR MAPPINGS
      page: 329
      pdf_page: 353
    - "no": 5
      title: DEFINITION OF PROJECTIVE SPACES
      page: 331
      pdf_page: 355
    - "no": 6
      title: HOMOGENEOUS COORDINATES
      page: 331
      pdf_page: 355
    - "no": 7
      title: PROJECTIVE LINEAR VARIETIES
      page: 332
      pdf_page: 356
    - "no": 8
      title: PROJECTIVE COMPLETION OF AN AFFINE SPACE
      page: 333
      pdf_page: 357
    - "no": 9
      title: EXTENSION OF RATIONAL FUNCTIONS
      page: 334
      pdf_page: 358
    - "no": 10
      title: PROJECTIVE LINEAR MAPPINGS
      page: 335
      pdf_page: 359
    - "no": 11
      title: PROJECTIVE SPACE STRUCTURE
      page: 337
      pdf_page: 361
statements: 12
exercises: 19
content_sha256: 9ec405c9c2bc207c1af5be029bef84392e88f4835ed116cca7afb6e29a9584e0
translated_from: content/en/alg/II/09_s9_affine_spaces_and_projective_spaces.md
translation_method: google
source_content_sha256: deaf2e284f8df7e22f7c5da850928b8f961fc09326f976f2aed34d10f8f21e0e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 231d5568a25ed08e25e75363dda30c72682f94cdcc29a32d2caed361d09fb61e
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 9。アフィン空間と射影空間

### 1. アフィンの定義空間

#### 定義 1 {#alg-ii-s9-def-1 .statement tag=05VM}

*体 K 上の左 (それぞれ右) ベクトル空間 T が与えられると、T に付加されたアフィン空間は、加法群 T* (I, § 5, no. 5) の任意の同次空間 E になります *0 が T の唯一の演算子であり、E* のすべての元は不変になります (つまりつまり、T * は E* に対して忠実かつ推移的に動作します)。 *これらの条件の下で、TはEの翻訳空間と呼ばれ、その元はE*（またはE*の*自由ベクトル）の翻訳と呼ばれます。

以下では、T が K 上で左ベクトル空間である場合に注意を限定します。 アフィン空間 E の変換ベクトル空間 T の次元 (K 上) は、E (K 上) の *次元* と呼ばれ、dim E または $\dim_K E$ で表されます。 次元 1 (それぞれ 2) のアフィン空間は、*アフィン ライン* (それぞれ *アフィン プレーン*) と呼ばれます。アフィン空間の元は *点* とも呼ばれます。

定義 1 の条件では、$t \in T$ と $a \in E$ については、t の下の点の $t + a$ または $a + t$ 変換で表します。それから関係

$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$

$s \in T, t \in T, a \in E$ を押し続けます。 写像 $x \mapsto x + t$ は、それ自体に対する E の全単射であり、これを t と同一視するします。さらに、定義 1 は、すべての $a \in E$、写像 $t \mapsto t + a$ が E に対する T の *全単射* であることを意味します。他の語では、E の 2 つの点 $a, b$ が与えられると、次のような翻訳 t が 1 つだけ存在します。 $b = t + a$;この翻訳を$b - a$で表すことにします。それから数式

$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a
$$
$$
(c - b) + (b - a) = c - a
$$

$a \in E, b \in E, c \in E$ まで押し続けてください。 E の 4 つの点 $a, b, a', b'$ が $b - a = b' - a'$、公式となる場合

$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$

T の加法の可換性は $b' - b = a' - a$ を示します。

点 $a \in E$ とすると、写像 $x \mapsto x - a$ は $E$ の $T$ 上の全単射です。この写像のもとで$E$が$T$と同一視されるとき、$E$は$E$の$a$を原点として＊得られたベクトル空間とみなされるといいます。逆に、すべてのベクトル空間 $T$ には、標準的に $T$ に結合されたアフィン空間の構造が含まれます。つまり、同種の空間構造対応するから部分群です。 $T$の$\{0\}$ (I, § 5, no. 6)。

#### 注意 {#alg-ii-s9-n1-rem-1 .statement tag=05VN}

この番号の定義拡大するの直後に続く結果の一部は、ベクトル空間 $T$ の代わりに、演算子* $T$ を使用した任意の *可換群を考慮した場合です。

### 2. 重心計算

#### 命題 1 {#alg-ii-s9-prop-1 .statement tag=05VO}

*$(x_i)_{i \in I}$ *アフィン内の点の族空間* $E$ *そして* $(\lambda_i)_{i \in L}$ *元の* $K$ *有限台のような* $\sum_{i \in I} \lambda_i = 1$ とする*(*それぞれ $\sum_{i \in I} \lambda_i = 0$*)。 ** $a$ * が * $E$ のいずれかの点である場合、*点* $x \in E$ *定義:
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(それぞれ、自由なベクトル* $\sum_{i \in I} \lambda_i (x_i - a)$) *点とは独立して考慮されます。*

$a'$ が $E$ の他の点である場合、
$$
\sum_i \lambda_i (x_i - a') = \sum_i \lambda_i ((x_i - a) + (a - a')) = \sum_i \lambda_i (x - a) + \left( \sum_i \lambda_i \right) (a - a').
$$
$\sum_i \lambda_i = 1$ の場合、$\sum_i \lambda_i (x_i - a) = (x - a) + (a - a') = x - a'$。 $\sum_i \lambda_i = 0$ の場合は $\sum_i \lambda_i (x - a') = \sum_i \lambda_i (x - a)$; よって命題。

命題 1 の条件の下では、点 $x$ によって定義されます
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(それぞれ、フリーのベクトル* $\sum_{i \in I} \lambda_i (x_i - a)$) * は * $\sum_{i \in I} \lambda_i x_i$ で示されます。

したがって、特に no. 1 で導入された記法 $b - a$ が回復されます。 $\sum_i \lambda_i = 1$、点 $x = \sum_i \lambda_i x_i$ は、点* $x_i$ *質量を考慮して* $\lambda_i$ の *重心 と呼ばれます。

$E$ の $m$ 点 $a_1, \ldots, a_m$ が与えられ、その数 $m$ が $K$ (V, § 1) の特性の倍数ではない場合、点 $g = \sum_{i=1}^m \frac{1}{m} a_i$ が呼び出されます (乱用により)

言語) 点* $a_i$ ($1 \leq i \leq m$) の *重心 ($m = 2$ については、「重心」の代わりに「中点」と言います)。 関係が特徴です
$$
\sum_{i=1}^m (a_i - g) = 0.
$$

### 3. アフィン線形多様体

#### 定義 2 {#alg-ii-s9-def-2 .statement tag=05VP}

*アフィン空間* $E$、*部分集合* $V$ *of* $E$ *はアフィン線形多様体* (または単に *線形多様体* または $E$ の *アフィン部分集合* と呼ばれます) *すべての家族の場合* $(x_i)_{i \in I}$ *of 点 of* $V$ *そしてすべての家族* $(\lambda_i)_{i \in I}$ *of 元 of* $K$ *of 有限台そのような* $\sum_{i \in I} \lambda_i = 1$, *重心* $\sum_{i \in I} \lambda_i x_i$ *属するから* $V$。

定義 2 の条件が $V$ の点のすべての *有限* 族に当てはまると言うのと同じことになります。

空の集合は線形多様性です。線形品種のすべての共通部分は線形品種です。

$V$ を空ではない $E$ の部分集合および $V$ の $a$ 点とします。 関係
$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$
$x$ は、$x_i$ と $a$ の家族からなるの重心 $\sum_{i=1}^n \lambda_i x_i + \left(1 - \sum_{i=1}^n \lambda_i\right)a$ であることを意味します。したがって:

#### 命題 2 {#alg-ii-s9-prop-2 .statement tag=05VQ}

*空ではない部分集合* $V$ *アフィン空間* $E$ *線形多様体であるためには、$V$ *ベクトル空間構造に対してベクトル部分空間であることが必要かつ十分です* $E$ *$V$ の点を原点として取得*

特に、ベクトル空間 $T$ (アフィン空間とみなされる) の空ではないアフィン線形多様体は、$T$ のベクトル部分空間の * 変換* にすぎません。したがって、$T$ のベクトル部分空間は、線形多様体含む 0 です。

$V$ をアフィン空間 $E$ の空ではない線形多様体とします。 $x$ と $y$ が $V$ を通るフリー ベクトル $x - y$ の集合は、$E$ の空間 $T$ のベクトル部分空間 $D$ です。 $V$ の *方向*: $a \in V$ の場合、
$$
x - y = (x - a) - (y - a)
$$
そして、私たちの主張は命題 2 から続きます。 $D$ が $V$ で忠実かつ推移的に動作するのは明らかであり、したがって、標準的には * $D$ に * アフィン空間の構造が付加されています。アフィン多様体 $V$ の *次元* とは、このアフィン空間構造を使用した $V$ の次元、つまりベクトル空間 $D$ の次元を意味します。 次元 0 の線形品種は $E$ の点です。 次元 1 (それぞれ 2) のものは、$E$ の *線* (それぞれ *平面*) と呼ばれます。

線の方向へのすべてのベクトル $\neq 0$ 所属は、この線の *方向ベクトル* と呼ばれます。その成分は、問題の行の *方向パラメータ* の系と呼ばれるもの、T 形の基底に関してです。

E における線形多様体 V の *余次元* は、T におけるその方向 D の余次元です。 E の余次元 1 の線形多様体は、E の (アフィン) *超平面* と呼ばれます。

同じ方向を持つ 2 つの線形品種は *並列* と呼ばれます。それは、一方が他方から翻訳によって派生したと言うのと同じことになります。 V が T の線形多様体 (アフィン空間とみなされる) の場合、その方向は V および含む 0 に平行な線形多様体です。

#### 命題 3 {#alg-ii-s9-prop-3 .statement tag=05VR}

*族* $(a_i)_{i \in I}$ *アフィン空間* の点の *集合* V *重心* $\sum_{i \in I} \lambda_i a_i$ *((\lambda_i) の有限台, $\sum_{i \in I} \lambda_i = 1$) は * E の線形多様体です。

ファミリ $(a_i)$ が空の場合、条件 $\sum_i \lambda_i = 1$ により $V = \varnothing$ になります。したがって、族 $(a_i)$ は空ではなく、この場合、$a_i$ の 1 つを E の原点として取ると、命題は明らかであると想定できます。

多様体 V は明らかに最小の線形多様体含む $a_i$ です。それはファミリー$(a_i)$によって*生成*され、このファミリーはVの*生成する系*と呼ばれます。

In the notation of Proposition 3, assuming the family $(a_i)$ is non-empty, for the expression for every point $x \in V$ in the form $x = \sum_i \lambda_i a_i$ to be *unique*, it is necessary and sufficient that, denoting an arbitrary index of I by $\kappa$, the family of vectors $a_i - a_\kappa$, where $i$ runs through the set of indices $\neq \kappa$, be free in T. 次に、E の点の族 $(a_v)_{v \in I}$ は *アフィン的に自由* (またはその元形は *アフィン的に自由系*、または *アフィン的に独立*) であり、 $\lambda_i$ は添字の $x$ の *重心座標* であると言われます。 $i$、自由な家族$(a_i)$に関して。

アフィン自由ではない E の点の族 $(a_i)_{i \in I}$ は、*アフィン的に関連している*と言われます。

#### 命題 4 {#alg-ii-s9-prop-4 .statement tag=05VS}

*For a non-empty family* $(a_i)_{i \in I}$ *of points in an affine space* E *to be affinely related, it is necessary and sufficient that there exist a family* $(\lambda_i)_{i \in I}$ *of elements not all zero in* K, *of finite support, such that* $\sum_{i \in I} \lambda_i = 0$ *and* $\sum_{i \in I} \lambda_i a_i = 0$.

添字 $\kappa \in I$ が与えられた場合、$i$ が添字 $\neq \kappa$ の集合を通るベクトル $(a_i - a_\kappa)$ の族が T で関連していると言うのは、すべての零がそのようなものではないスカラー $(\lambda_i)_{i \neq \kappa}$ の族が存在することを意味します。 $\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$、$\sum_{i \in I} \lambda_i a_i = 0$、$\lambda_\kappa = -\sum_{i \neq \kappa} \lambda_i$、他の語 $\sum_{i \in I} \lambda_i = 0$ とも書かれます。

#### 命題 5 {#alg-ii-s9-prop-5 .statement tag=05VT}

For a non-empty family $(a_i)_{i \in I}$ of points of an affine space $E$ to be affinely free, it is necessary and sufficient that, for every index $\kappa \in I$, $a_\kappa$ do not belong to the linear variety generated by the $a_i$ of index $\neq \kappa$.

$I$ に元が 1 つしかない場合、命題は明らかです。それ以外の場合は、添字 $\neq \kappa$ の $a_i$ のいずれかを$E$ を起点として、§ 7, no. 1、注意から命題が続きます。

### 4. アフィン線形写像

#### 定義 3 {#alg-ii-s9-def-3 .statement tag=05VU}

2 つのアフィン空間 $E, E'$ が同じ体 $K$ 上の 2 つのベクトル空間 $T, T'$ に接続されているとすると、$E$ の $E'$ への写像 $u$ はアフィン線形写像 (またはアフィン写像) すべての家族 $(x_i)_{i \in I}$、点、$E$、およびすべての家族 $(\lambda_i)_{i \in I}$ について、$\sum_{i \in I} \lambda_i = 1$ が成立する場合、

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

(3)

#### 命題 6 {#alg-ii-s9-prop-6 .statement tag=05VV}

$u$ を $E$ から $E'$ へのアフィン写像とします。 $T'$ には、$T$ の線形写像 $v$ が 1 つだけ存在します。

$$
u(x + t) = u(x) + v(t)
$$

すべての$x \in E, t \in T$に。

$a$ を $E$ のいずれかの点とします。 写像

$$
t \mapsto u(a + t) - u(a)
$$

$T$ の線形写像 $v_a$ を $T'$ にすると、次のように書くことができます。

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a \\
a + s + t = (a + s) + (a + t) - a
$$

(3) から、$v_a(\lambda t) = \lambda v_a(t)$ と $v_a(s + t) = v_a(s) + v_a(t)$ が導かれます。さらに、$b$が$E$の他の点であれば、$v_a = v_b$です。 関係用

$$
(a + t) - a + b = b + t
$$

暗示する

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

それは$u(a + t) - u(a) = u(b + t) - u(b)$です。 よって $v$ の存在。 一意性は明らかです。

$v$ は、$T$ の線形写像が $u$ に関連付けられた $T'$ に呼び出されます。逆に、$T$ から $T'$ へのすべての線形写像 $v$ と、点 $a \in E, a' \in E'$ のすべての注文された対については、次のことが即座に検証されます。

$$
x \mapsto a' + v(x - a)
$$

は、E から E' へのアフィン写像で、その関連する線形写像は v です。したがって、u が E から E' へのアフィン写像であるということは、E の任意の点 a と E' の点 u(a) を原点とすると、u はその 2 つに対して線形写像であることも意味します。こうしてベクトル空間が得られました。

E'' を 3 番目のアフィン空間、T'' の変換空間、u' を E' から E'' へのアフィン写像、v' を u' に関連付けられた T'' へのアフィン線形写像とします。明らかに、u' o u は E から E'' へのアフィン写像です。さらに、a \in E と t \in T の場合、
$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$
したがって、v' o v は、u' o u に関連付けられた T から T'' への線形写像です。アフィン写像 u が全単射であるためには、関連する線形写像 v が全単射であることが必要かつ十分であり、そのとき u^{-1} は、関連する線形写像が v^{-1} であるアフィン写像になります。

特に、E のそれ自体形群 G への E のアフィン全単射は、E のアフィン群と呼ばれます。 u \in G 線形写像 v に関連付けられた写像は、上記により、線形群上の G の準同型になります。 \mathbf{GL}(T)。 u が翻訳の場合、v は恒等式であり、その逆も同様です。したがって、上記の準同型の核は E の翻訳群 T であり、したがって G の正規の部分群です。

u \in G の場合、T の自己同型 t \mapsto utu^{-1} (t は変換 x \mapsto x + t で識別されます) は、u に関連付けられた線形写像 v です。 x \in E および t \in T の場合、定義による
$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t)
$$
したがって、utu^{-1} = v(t) となります。

a \in E と G_a を、u(a) = a となるように、G の部分群からなる u \in G とします。 a を原点として E を T と同定すると、G_a は \mathbf{GL}(T) と同定されます。 G 内のすべての u \は形 u = t_1u_1 (それぞれ形 u = u_2t_2) で一意に表現できます。ここで、u_1、u_2 は G_a にあり、t_1、t_2 は T にあります。つまり、 t_1 = u(a) - a, u^{-1}t_1 \in G_a と書くと、よっての存在がわかります。 u_1 と t_1 の; u_2 と t_2 の存在も同様に取得されます。 一意性は、G_a \cap T 簡約するから G の単位元であるという事実から得られます。
$$
t_1u_1 = u_1(u_1^{-1}t_1u_1)
$$
よって u_2 = u_1、t_2 = u_1^{-1}t_1u_1。最後に、u に関連付けられた線形写像と u_1 は同じであるため、上記のように G_a が \mathbf{GL}(T) で識別される場合、u_1 は T から u に関連付けられたそれ自体まで線形写像になります。したがって、G は T (I, § 6, no. 1) による G_a の半直接積であることがわかります。

E、E' を K 上の 2 つのアフィン空間とします。E から E' へのアフィン写像 u の下での E (それぞれ E') の線形多様体の直接 (または逆) 像は、E' (それぞれ E) の線形多様体です。 u の階数は u(E) の定義次元によるものです。それは、u に関連付けられた線形写像の階数に等しいです。 V、V' がそれぞれ E、E' の同じ有限次元 m の線形多様体である場合、$E$ の $E'$ へのアフィン写像 $u$ が存在します。そのような$u(V) = V'$: $E$ を原点とし、それぞれ $V$ と $V'$ の $E'$ 点、次に $E$ (それぞれ $E'$) 基底を取り込み、その最初の $m$ ベクトル形基底 $V$ (それぞれ $V'$)、§ 1, no. 11、系 3 から命題 17 のすぐ後に命題が続きます。

体 $K$ は$K$ に対して正準的に左ベクトル空間構造 (次元 1 のうち) を持っているため、次元 1 のアフィン空間と考えることができます。 アフィン空間 $D$ ($K$ 以上) からアフィン空間 $K$ へのアフィン写像は、*アフィン線形写像* (または *アフィン写像*) とも呼ばれます。 点 $a$ が $E$ の原点として取られる場合、$E$ 上のすべてのアフィン写像は$x \mapsto \alpha + v(x)$ として一意に書くことができます。ここで、$\alpha \in K$ と $v$ はベクトル空間 $E$ 上の線型形式になります。取得しました。 $E$ のアフィン写像したがって、形は次元 $1 + \dim E$ の *右ベクトル空間 $K$ を超えます。 If $u$ is a non-constant affine function on $E$ and $\lambda \in K$, the set of $x \in E$ satisfying the equation $u(x) = \lambda$ is a hyperplane; conversely, for every hyperplane $H$ in $E$, there exists an affine function $u_0$ on $E$ such that $H = u_0^{-1}(0)$ and every affine function $u$ such that $H = u^{-1}(0)$ is of the form $u_0 \mu$, where $\mu \in K$ (§ 7, no. 5, Proposition 11). $u$ が $E$ 上のアフィン写像である場合、方程式 $u(x) = \alpha$ と $u(x) = \beta$ を持つ超平面は平行です。

### 5. 射影空間の定義

#### 定義 4 {#alg-ii-s9-def-4 .statement tag=05VW}

*左 (右) ベクトル空間* $V$ *上体* $K$、*左 (右) 射影空間は $V$ から導出され、* $\mathbf{P}(V)$ で示され、* 補数の商です* $V - \{0\}$ *の* $\{0\}$ *で* $V$ *同値関係*によって $\Delta(V)$ *「存在します* $\lambda \neq 0$ *で* $K$ *そのような* $y = \lambda x$ *(それぞれ* $y = x \lambda$ ) *間に* $x$ *と* $y$ *で* $V - \{0\}$。

$V = K_s^{n+1}$の場合、$\mathbf{P}(K_s^{n+1})$の代わりに$\mathbf{P}_n(K)$、$\Delta(V)$の代わりに$\Delta_n(K)$と書きます。

Definition 4 can also be expressed by saying that $\mathbf{P}(V)$ is the set of lines (passing through 0) in $V$ with the origin removed; $\mathbf{P}(V)$ is therefore canonically identified with the set of lines (passing through 0) in $V$. 射影空間の元は、その空間の *点* と呼ばれます。

$V$ が次元 $n$ であるとき、$n$ が有限であれば、整数 $n - 1$ は射影空間 $\mathbf{P}(V)$ の *次元* と呼ばれ、それ以外の場合は基数 $n$ と呼ばれます。この基数は$\dim_K \mathbf{P}(V)$または$\dim \mathbf{P}(V)$で表されます。したがって、次元 $-1$ の射影空間は空であり、次元 0 の射影空間は単一の点です。 次元 1 (それぞれ 2) の射影空間は *射影線* (それぞれ *射影平面*) と呼ばれます。

以降、左射影空間のみを考慮します。

### 6. 同次座標

$V$ を $K$ 上の有限次元 $n + 1$ のベクトル空間、 $\mathbf{P}(V)$ の $V$ と $(e_i)_{0 \leq i \leq n}$ 基底から導出された次元 $n$ の射影空間とします。 $V$。 $\pi$ が $V - \{0\}$ の標準写像を商集合 $\mathbf{P}(V)$ に表すとします。 $V - \{0\}$ のすべての点 $x = \sum_{i=0}^{n} \xi_i e_i$ に対して、$(\xi_0, \xi_1, \ldots, \xi_n)$ は、$V$ の基底 $(e_i)$ に関して、点 $\pi(x)$ の同次座標の *系と呼ばれます。 Every system $(\xi_i)$ of $n + 1$ elements *not all zero* of $K$ is therefore a system of homogeneous coordinates of a point of $P(V)$ with respect to $(e_i)$; for two such systems $(\xi_i)$, $(\xi'_i)$ to be systems of homogeneous coordinates of the same point of $P(V)$ with respect to the same basis $(e_i)$, it is necessary and sufficient that there exists an element $\lambda \neq 0$ of $K$ such that $\xi'_i = \lambda \xi_i$ for $0 \leq i \leq n$.

この定義は、$V$が無限次元である場合に直ちに一般化されます。

Given another basis $(\tilde{e}_i)$ of $V$ such that $e_i = \sum_{j=0}^{n} \alpha_{ij} \tilde{e}_j$ ($0 \leq i \leq n$) and a system $(\xi_i)$ of homogeneous coordinates of $\pi(x)$ with respect to the basis $(e_i)$, for a system $(\bar{\xi}_i)$ of $n + 1$ elements of $K$ to be a system of homogeneous coordinates of $\pi(x)$ with respect to the basis $(\tilde{e}_i)$, it is necessary and sufficient that there exist $\lambda \neq 0$ in $K$ such that

$$
\lambda \bar{\xi}_i = \sum_{j=0}^{n} \xi_j \alpha_{ji} \quad \text{for } 0 \leq i \leq n.
$$

特に、$e_i = \gamma_i \tilde{e}_i$ と $\gamma_i \neq 0$ ($0 \leq i \leq n$) の場合、$\mu \neq 0$ である$\bar{\xi}_i = \mu \xi_i \gamma_i$ になります。

### 7. 射影線形多様体

$W$ をベクトル空間 $V$ のベクトル部分空間とします。 $V$ から導出された射影空間 $P(V)$ の $W - \{0\}$ の標準像は、*射影線形多様体* (または、混乱を恐れない場合は単に *線形多様体*) と呼ばれます。 $W - \{0\}$ の同値関係 $\Delta(W)$ が関係 $\Delta(V)$ によって誘導されるため、$P(V)$ の $W - \{0\}$ の射影線形多様体像は、$W$ から導出された射影空間 $P(W)$ と識別できます。したがって、私たちはそのような多様な次元について話すことができます。射影空間 $P(V)$ では、$V$ の超平面 (原点が削除されたもの) の標準像は *射影超平面* (または単に *超平面*) と呼ばれる線形多様体です。 $P(V)$ が有限次元 $n$ 超平面の $P(V)$ は、次元 $n - 1$ の線形多様体です。

ベクトル空間のベクトル部分空間に関するすべての命題は、射影線形多様体に関する命題に移ります。たとえば、射影空間 $P(V)$ が有限次元 $n$ で、$(e_i)_{0 \leq i \leq n}$ が $V$ の基底である場合、次元 $r$ のすべての線形多様体 $L \subset P(V)$ は、系によって定義できます。 $n - r$ 等次一次方程式

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \qquad (1 \leq j \leq n - r)
$$

基底 $(e_i)$ に関する同次座標 $\xi_i$ ($0 \leq i \leq n$) の $\mathbf{P}(V)$ の点の間で、(4) の左辺は V 上で線形独立形です。特に、射影超平面は、すべての零が係数である単一の同次線形方程式によって定義されます。逆に、$\mathbf{P}(V)$ 満たす $\xi_i$ 形線形多様体 L に関する任意の同次一次方程式系の点。 系が $k \leq n + 1$ 方程式で構成されていると考えると、L は次元 $\geq n - k$ になります。

$\mathbf{P}(V)$ の線形品種のすべての共通部分は線形品種です。 $\mathbf{P}(V)$ のすべての部分集合 A に対して、最小の線形多様体 L 含む A が存在します。それは A によって *生成された線形多様性と呼ばれ、A は L の *生成する系* と呼ばれます。

W が $\pi^{-1}(A)$ によって生成された V のベクトル部分空間である場合、$L = \mathbf{P}(W)$ です。

L と M が $\mathbf{P}(V)$ と $L \cup M$ によって生成された品種 N 内の任意の 2 つの線形品種である場合、(§ 7, no. 3, 系 3 ～ 命題 4)

$$
\text{dim } L + \text{dim } M = \text{dim}(L \cap M) + \text{dim } N.
$$

特に、$\mathbf{P}(V)$ が有限次元であり、$\text{dim } L + \text{dim } M \geq \text{dim } \mathbf{P}(V)$ である場合、(5) から $L \cap M$ は空ではないことがわかります。

$(x_i), (y_i)$ を、同じインデックス付け集合を持つベクトル空間 V の 2 つの点ファミリーとし、$y_i = \lambda_i x_i$ とし、すべての $i$ に対して $\lambda_i \neq 0$ を指定します。家族 $(x_i)$ が自由であれば、$(y_i)$ も自由であり、その逆も可能です。その場合、$\mathbf{P}(V)$の点$\pi(x_i)$の家族は*投影的に自由*(または単に*自由*)であると言われます。すべての添字 $\kappa$ について、点 $\pi(x_\kappa)$ は、$i \neq \kappa$ の $\pi(x_i)$ によって生成される線形多様性に属するしないと言うのと同じことになります。射影自由ではない $\mathbf{P}(V)$ の点の族は、*射影関連* (または単に *関連*) と呼ばれます。

$V - \{0\}$の点の家族$(x_i)$が、家族$(\pi(x_i))$が射影的に自由であり、生成する$\mathbf{P}(V)$となるようにするには、$(x_i)$がVの基底であることが必要かつ十分です。 $\mathbf{P}(V)$ が次元 $n$ である場合、そのような家族の元の数は、したがって $n + 1$ になります。 $\mathbf{P}(V)$ でこのような族 $(\pi(x_i))$ を与えることは、V の基底 $(y_i)$ に関して、$\mathbf{P}(V)$ の指定された点の同次座標を決定する (左の因子内であっても) $\pi(y_i) = \pi(x_i)$ のようにならないことに注意してください。すべて$i$ (cf. no. 6)。

### 8. アフィン空間の射影完了

V を体 K 上の (左) ベクトル空間とし、K 上のベクトル空間 $K_s \times V$ を考えます。射影空間 $\mathbf{P}(K_s \times V)$ は、ベクトル空間 V と *正準的に関連付けられた* 射影空間と呼ばれます。 V が次元 $n$ である場合、$\mathbf{P}(K_s \times V)$ は同じ次元 $n$ です。 $K_s \times V$ で、方向 (no. 3) が部分空間 $V_0 = \{0\} \times V$ であるアフィン超平面 $V_1 = \{1\} \times V$ を考えてみましょう。 $K_s \times V$ の行 (移行 ～ 0) が $V_0$ に含まれていない場合、含む点 $(\alpha, x)$ と $\alpha \neq 0$ および $x \in V$ であるため、含むはまた、点 $\alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x)$ になります。 $V_1$; 逆は明らかであり、$V_1$ の点と$V_0$ に含まれない$K_s \times V$ の行 (移行から 0) の間には 1 対 1 の対応があり、後者のそれぞれは $V_1$ と 1 対 1 で会合していることがわかります。 点は 1 つだけです。 したがって、写像 $x \mapsto \phi(x) = \pi(1, x)$ は、射影空間 $P(K_s \times V)$ への $V$ の単射 (正準と呼ばれます) になります。 $V$ は、この単射の下にある像と同一視されることがよくあります。 $P(K_s \times V)$ の $\phi(V)$ の補数は、$P(K_s \times V)$ (または言葉の乱用により $V$) の無限遠で超平面と呼ばれる射影超平面 $P(V_0)$ です。その点は、$P(K_s \times V)$（または$V$）の「無限大の点」とも呼ばれます。 If $(a_i)$ is a basis of $V$ and in $K_s \times V$ the basis is taken consisting of the elements $e_i = (0, a_i)$ and the element $e_\omega = (1, 0)$, the points at infinity in $P(K_s \times V)$ are those whose homogeneous coordinate of index $\omega$ is 0.

Let $M$ be an affine linear variety in $V$ (no. 3) and $D$ its direction; the canonical image $\phi(M)$ of $M$ in $P(K_s \times V)$ is contained in the canonical image $\overline{M} = \pi(M_2)$ of the vector subspace $M_2$ of $K_s \times V$ generated by the affine variety $M_1 = \{1\} \times M$ of $K_s \times V$. More precisely, if $(a_i)$ is an affinely free system of $M$ generating $M$, the elements $(1, a_i)$ form a basis of $M_2$ and therefore $\overline{M}$ is just the projective linear variety generated by $\phi(M)$; if $M$ is finite-dimensional, $\overline{M}$ has the same dimension as $M$. $\overline{M}$ の $\phi(M)$ の補数は、$\overline{M}$ と超平面の共通部分であり、標準像 $\pi(M_0)$ に等しくなります ($M_0 = \{0\} \times D$)。

逆に、$N$ を無限遠で超平面に含まれない射影線形多様体とし、$R = \pi^{-1}(N)$ とします。 $R \cap V_1$ は、形 $\{1\} \times M$ の $K \times V$ のアフィン線形多様体であり、$M$ は $V$ のアフィン線形多様体であり、$N$ は $\phi(M)$ によって生成されたアフィン線形多様体 $\overline{M}$ であることがすぐにわかります。

したがって、$V$ のアフィン線形多様体と、無限遠で超平面に含まれない$P(K_s \times V)$ の射影線形多様体の間には 1 対 1 の対応が存在します。 $V$ の 2 つのアフィン線形多様体が平行であるためには、それら生成するが無限遠で超平面と同じ共通部分を持つことが必要かつ十分です (これは、問題の 2 つのアフィン線形多様体が無限遠で同じ点を持つことをというで表すときどきです)。

### 9. 合理的写像の拡大

If the results of no. 8 are applied to the vector space $V = K_s$ of dimension 1, it is seen that there exists a canonical injection $\phi$ of $K_s$ into the projective line $P_1(K) = P(K_s \times K_s)$; for all $\xi \in K$, $\phi(\xi)$ is the point with homogeneous coordinates $(1, \xi)$ with respect to the canonical basis (§ 1, no. 11) of $K_s \times K_s$. $P_1(K)$ の $\phi(K)$ の補数は、上記の基底に関して同次座標 $(0, 1)$ を持つ単一の点で構成されます。それは「無限遠の点」と呼ばれます。 $P_1(K)$ は、$K$ に関連付けられた射影体とも呼ばれ、$\tilde{K}$ で示され、$\tilde{K}$ の無限遠にある点は $\infty$ で示されます。

*特に、$K$ が可換体であり、K(X) の f \in を K (IV, § 4) 上の 1 つの不定数における有理数写像とする場合を考えてみましょう。 $f \neq 0$ の場合、一意の式 $f = \alpha p/q$ が存在します。ここで、$\alpha \in K^*$、$p$、$q$ は 2 つの比較的素な多項式 (VII, § 1) です。 $m$ と $n$ をそれぞれの次数とし、$r = \sup(m, n)$ とします。私たちは書きます
$$
p_1(T, X) = T^r p(X/T), \qquad q_1(T, X) = T^r q(X/T);
$$
$p_1$ と $q_1$ は、$p(X) = p_1(1, X)$、$q(X) = q_1(1, X)$ など、$K$ に対する次数 $r$ の 2 つの同次多項式です。したがって、$q(X)$ の零ではないすべての元 $\xi \in K$ について、$f(\xi) = \alpha p(\xi)/q(\xi)$ が定義され、次のように書くことができます。
$$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$
$K$のすべての$\lambda \neq 0$に。それでは写像を考えてみましょう
$$
(\eta, \xi) \mapsto (q_1(\eta, \xi), p_1(\eta, \xi))
$$
$K^2$ のそれ自体へ。 同値関係 $\Delta(K^2)$ と互換性があるため、定義する、移行が商になると、$\tilde{K}$ の写像 $\tilde{f}$ が点で$\xi \mapsto f(\xi)$ と一致するになります。有理数写像が定義されています。言葉の乱用により、$\tilde{f}$ は $f$ から $\tilde{K}$ の正規の拡大であると言われています。

たとえば、$f = 1/X$ の場合は、$\tilde{f}(0) = \infty$ と $\tilde{f}(\infty) = 0$ です。もし
$$
f = (aX + b)/(cX + d)
$$
$ad - bc \neq 0$なら$\tilde{f}(-d/c) = \infty$、$c \neq 0$なら$\tilde{f}(\infty) = a/c$、$c = 0$なら$\tilde{f}(\infty) = \infty$。 $f = a_0 X^n + \cdots + a_n$ が次数 $n > 0$ の多項式である場合、$\tilde{f}(\infty) = \infty$*

### 10. 射影線形写像

$V, V'$を体$K$、$f$線形写像の$V$を$V'$、$N = \overline{f}(0)$を核に2つ左ベクトル空間とします。 $N$に含まれない$V$の行(移行～0)の$f$下の像が$V'$の行(移行～0)であることは明らかです。したがって、移行から商まで、$f$ 定義する写像 $P(V) - P(N)$ の $g$ が $P(V')$ になります。このような写像は射影線形写像 (または単に射影写像) と呼ばれます。 $P(V)$ ($N \neq \{0\}$ のとき) ではなく $P(V) - P(N)$ に定義されていますが、言葉の乱用により、$g$ は $P(V)$ の $P(V')$ への射影写像であると言えます。 $g$ が定義されていない射影線形多様体 $P(N)$ は、$g$ の中心と呼ばれます。

$g$が$P(V)$全体で定義されている場合（つまり$N = \{0\}$の場合）、$g$は$P(V)$の単射が$P(V')$になることに注意してください。

$V$と$V'$にそれぞれ基底$(a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M}$が与えられると、$P(V)$の写像は$P(V)$の$P(V')$写像点に同次座標$\xi_\lambda$で射影されます。 ($\lambda \in L$) から $\mathbf{P}(V')$ の点と同次座標の系形の $\eta_\mu$ ($\mu \in M$)

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

$g$ の中心は、方程式で定義される線形多様体です。

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

$C$が$g$の中心で、$M$が$\mathbf{P}(V)$の線形多様体である場合、$M - (M \cap C)$の$g$の下にある像は、$g(M)$で（言葉の乱用により）表される$\mathbf{P}(V')$の線形多様体です。それから

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

(§ 7, no. 4、公式 (12))。 $M'$ が $\mathbf{P}(V')$ の線形多様体である場合、$g^{-1}(M') \cup C$ は $\mathbf{P}(V)$ の線形多様体であり、

$$
\dim(g^{-1}(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

言葉の乱用により、$g^{-1}(M') \cup C$ は $g$ の下の $M'$ の *逆像* であると言われています。

$V$の基底$(e_i)$で線形写像がとった値は$V'$で任意に選択できるので、$\mathbf{P}(V)$の$\mathbf{P}(V')$への射影線形写像が*任意の*値を取ることがわかります。 点 $\pi(e_i)$。 ただし、($g$ がどこでも定義されている場合でも) $g(\pi(e_i))$ を指定しても、決定する $g$ は一意に (練習問題 10) にはなりません。

全単射である 2 つの射影写像のうち合成は射影写像です。 全単射の逆数写像も同様です。射影空間 $\mathbf{P}(V)$ の全単射射影写像は、形群となり、$\mathbf{P}(V)$ の*射影群* と呼ばれ、$\mathbf{PGL}(V)$ で表されます。 $\mathbf{PGL}(K^n_s)$ の代わりに $\mathbf{PGL}_n(K)$ または $\mathbf{PGL}(n, K)$ と書きます。

#### 注意 {#alg-ii-s9-n10-rem-1 .statement tag=05VX}

体 $K$ に対する射影空間 $\mathbf{P}(V)$ では、$H = \mathbf{P}(W)$ を超平面とします。 $f(W) = W$ となるような $K_s \times W$ 上への $V$ の全単射線形写像 $f$ が存在します。 $g$ を $f$ から移行から商までに得られる射影写像とします。 $\mathbf{P}(K_s \times W)$ の $\mathbf{P}(W)$ の補数は、翻訳空間が $W$ であるアフィン空間と識別できることがわかりました (no. 8)。 $\mathbf{P}(V)$が$g$によって$\mathbf{P}(K_s \times W)$と同一視されると、$\mathbf{P}(V)$では$H$が*無限遠の超平面とみなされた*と言われます。 $\mathbf{P}(V)$ の $H$ の補数は、翻訳空間が $W$ であるアフィン空間で識別されます。

### 11. 射影空間構造

集合 E と体 K が与えられると、体 K に関する E 上の (左) 射影空間構造は、射影空間の全単射の部分集合の空でない集合 $\Phi$ を与えることによって定義されます。 $\mathbf{P}(K_s^{(E)})$ を E 満たすに次の公理を適用します。

$$(\mathrm{EP}_I)$$ *すべての写像 $f \in \Phi$ の定義の集合は、$\mathbf{P}(K_s^{(E)})$ の線形多様体です。*

$$(\mathrm{EP}_{II})$$ *線形品種 $\mathbf{P}(V)$ と $\mathbf{P}(W)$ でそれぞれ定義された元 $f, g$ の $\Phi$ のすべての順序対について、$\mathbf{P}(W)$ への $\mathbf{P}(V)$ の全単射 $h = g^{-1} \circ f$ は射影です写像.*

$$(\mathrm{EP}_{III})$$ *Conversely, if $f \in \Phi$ is defined on the linear variety $\mathbf{P}(V)$ and $h$ is a bijective projective mapping of $\mathbf{P}(V)$ onto a linear variety $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, then $f \circ h^{-1} \in \Phi$.*

E を K 上のベクトル空間の族である集合、$(V_\lambda)_{\lambda \in L}$ とし、$\mathbf{P}(V_\lambda)$ の各 $\lambda \in L$ 全単射 $f_\lambda$ が E に与えられると仮定します。その結果、添字 $\lambda, \mu, f_\lambda^{-1} \circ f_\mu$ のすべての順序対が *射影になります$\mathbf{P}(V_\mu)$ の写像* を $\mathbf{P}(V_\lambda)$ に。次に、次のように、K に関する射影空間構造を E 上で定義するできます。 $(e_i)_{i \in I}$ を空間 $V_\lambda$ の基底として、$a_i = f_\lambda(\pi(e_i))$ と書きます。 $b_i$ を $K_s^{(E)}$ (§ 1, no. 11) の標準基底の添字 $a_i$ の元とします。 関係 $i \neq \kappa$ は、仮定により $f_\lambda$ が全単射であるため、$b_i \neq b_\kappa$ を暗示します。したがって、ベクトル部分空間 $W_0$ の $K_s^{(E)}$ の $b_i$ 形基底は、$\mathbf{P}(V_\lambda)$ への $\mathbf{P}(W_0)$ の全単射射影写像 $h$ が存在します。 $h(\pi(b_i)) = \pi(e_i)$ はすべての $i \in I$ に当てはまります。 $\Phi$ がすべての全単射射影写像 $f_\lambda \circ h \circ g^{-1}$ の集合であるとみなされる場合、$g$ はすべての全単射射影写像 $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$ の集合を通過し、$\Phi$ が満たされることが直ちに検証されます。公理 (EP_I)、(EP_{II})、および (EP_{III})。さらに、$\Phi$ は、添字 $\lambda \in L$ の選択にも、$V_\lambda$ の基底 $(e_i)$ の選択にも、選択にも依存しないのは、明らかです。 $h$。

特に (L を単一の元から構成すると)、ベクトル空間 V (no. 5, 定義 4) から導出されるすべての射影空間 $\mathbf{P}(V)$ には、よく決定された「射影空間」があります。 構造」は、この番号に示されている定義の意味です。したがって、射影空間構造をもつ集合は *射影空間* と呼ぶことができます。

同じ記法では、射影空間 E の *線形多様体* は E の部分集合 M であるため、$\mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)})$ で定義された少なくとも *1 つ* 全単射 $f \in \Phi$ について、$f^{-1}(M)$ は次の意味で $\mathbf{P}(V)$ の線形多様体になります。 no. 7 (この性質は *すべて* $f \in \Phi$ に当てはまります)。上記のことから、射影空間のすべての線形多様体には標準的に射影空間構造があることがわかります。

すべての $f \in \Phi, f^{-1}(E)$ が次元 n の線形多様体である場合、射影空間 E は *of 次元 n* であると言われます (これが *1* 写像 $f \in \Phi$ に当てはまれば十分です)。

### 練習問題 {#alg-ii-s9-exercises}

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
