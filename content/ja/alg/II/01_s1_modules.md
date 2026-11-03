---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 1
section_title: Modules
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 191-227, 380-386
pdf_pages: 0215-0251, 0404-0410
extraction: ocr
subsections:
    - "no": 1
      title: MODULES; VECTOR SPACES; LINEAR COMBINATIONS
      page: 191
      pdf_page: 215
    - "no": 2
      title: LINEAR MAPPINGS
      page: 194
      pdf_page: 218
    - "no": 3
      title: SUBMODULES; QUOTIENT MODULES
      page: 196
      pdf_page: 220
    - "no": 4
      title: EXACT SEQUENCES
      page: 197
      pdf_page: 221
    - "no": 5
      title: PRODUCTS OF MODULES
      page: 200
      pdf_page: 224
    - "no": 6
      title: DIRECT SUM OF MODULES
      page: 202
      pdf_page: 226
    - "no": 7
      title: INTERSECTION AND SUM OF SUBMODULES
      page: 205
      pdf_page: 229
    - "no": 8
      title: DIRECT SUMS OF SUBMODULES
      page: 208
      pdf_page: 232
    - "no": 9
      title: SUPPLEMENTARY SUBMODULES
      page: 210
      pdf_page: 234
    - "no": 10
      title: MODULES OF FINITE LENGTH
      page: 212
      pdf_page: 236
    - "no": 11
      title: FREE FAMILIES. BASES
      page: 214
      pdf_page: 238
    - "no": 12
      title: ANNIHILATORS. FAITHFUL MODULES. MONOGENOUS MODULES
      page: 219
      pdf_page: 243
    - "no": 13
      title: CHANGE OF RING OF SCALARS
      page: 221
      pdf_page: 245
    - "no": 14
      title: MULTIMODULES
      page: 224
      pdf_page: 248
statements: 88
exercises: 27
content_sha256: 5f18eada75df17efa83e17d532d14c94188627b45e0178cb60b0722e0705bb8f
translated_from: content/en/alg/II/01_s1_modules.md
translation_method: google
source_content_sha256: 7b2cea857b009f809085412ca64248b0f317359a2bcbd7a3a189e12a6f0b01fe
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 713212ffec8e365b5c80d577312c456a8a41f3f452c9069b381ede868ba3e78f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 加群

### 1. 加群; ベクトル空間; 線形結合

#### 定義 1 {#alg-ii-s1-def-1 .statement tag=05JO}

*与えられた環* $\mathbf{A}$, *左加群以上* $\mathbf{A}$ (*または左* $\mathbf{A}$-*加群*) *は集合* $\mathbf{E}$ *与えることによって定義された代数構造を使用*:

(1) *$\mathbf{E}$ 上で可換群法則 (*以下は加法的に書かれています*);

(2) *作用* $(\alpha, x) \mapsto \alpha \top x$ の *法則、 *演算子の定義域は環* $\mathbf{A}$ *次の公理を満たす*:

$$
\begin{align*}
(\mathbf{M_I})\quad & \alpha \top (x + y) = (\alpha \top x) + (\alpha \top y) \text{ for all } \alpha \in \mathbf{A}, x \in \mathbf{E}, y \in \mathbf{E}; \\
(\mathbf{M_{II}})\quad & (\alpha + \beta) \top x = (\alpha \top x) + (\beta \top x) \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{III}})\quad & \alpha \top (\beta \top x) = (\alpha \beta) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{IV}})\quad & 1 \top x = x \text{ for all } x \in \mathbf{E}.
\end{align*}
$$

公理$(\mathbf{M_I})$は、左$\mathbf{A}$加群$\mathbf{E}$の外部法則が$\mathbf{E}$上の加法に関して*分配*であることを意味します。したがって、加群は演算子と可換な群です。

定義 1 の場合、公理 $(\mathbf{M_{III}})$ は次のように置き換えられます。

$$
(\mathbf{M'_{III}})\quad \alpha \top (\beta \top x) = (\beta \alpha) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E},
$$

このように定義された代数構造を持つ E は、A または右A-加群に対する権利加群です。

A-加群 (左または右) について話すとき、環 A の元はスカラーと呼ばれることがよくあります。

通常、外部法則または合成または左A-加群 (または右A-加群) は乗算的に書かれ、演算子は左側 (または右側) に書かれます。 条件 (M_{III}) は $\alpha(\beta x) = (\alpha\beta)x$ と書き込まれ、条件 (M'_{III}) は $(x\beta)\alpha = x(\beta\alpha)$ と書き込まれます。

$A^0$ が A (I, § 8, no. 3) に対して反対環を表す場合、環 A 上のすべての右加群 E は、環 $A^0$ に対して左加群となります。したがって、左加群または右側の加群に系統的に注意を限定しながら、加群の特性を説明することができます。 §§ 1 と 2 では、一般に左加群について説明します。加群について話すときは (どの型であるかは特定せずに) 左加群を意味し、その外部法則は乗法で記述されます。 環 A が可換なとき、A に対する右辺加群と左加群の概念は同一です。

A-加群 E のすべての $\alpha \in A$、写像 $x \mapsto \alpha x$ をそれ自体にすると、E の比率 $\alpha$ (I, § 4, no. 2) のホモテティー と呼ばれます。 (M_I) によるホモテティー は、E 上の可換群構造 (演算子なし) の自己準同型ですが、一般的には E 上の加群構造 (I, § 4, no. 2; cf. II, § 1, no. 2 および no. 13) ではありません。したがって、$\alpha 0 = 0$ と $\alpha(-x) = -(\alpha x)$ です。 $\alpha$ が A の可逆元である場合、ホモテティー $x \mapsto \alpha x$ は E 上の可換群構造 (演算子なし) の自己同型である場合、関係 $y = \alpha x$ は (M_IV) によって暗示されます。 $x = \alpha^{-1}(\alpha x) = \alpha^{-1}y$。

同様に、(M_{II}) により、すべての $x \in E$、写像 $\alpha \mapsto \alpha x$ は、加法群 A の準同型を可換群 (演算子なし) E に変換します。したがって、$0x = 0$ と $(-\alpha)x = -(\alpha x)$ です。さらに、(M_IV) によって、整数 $n \in \mathbf{Z}$、$n.x = (n.1)x$ ごとに。

環 A が元 0 のみで構成される場合、すべての A-加群 E は元 0 のみで構成され、そのとき A の $1 = 0$、よって、すべての $x \in E$、
$x = 1.x = 0.x = 0$。

#### 例 {#alg-ii-s1-n1-exa-1 .statement tag=05JP}

(1) $\phi$ を環 A の準同型から環 B にします。 $A \times B$ の写像 $(a, x) \mapsto \phi(a)x$ (それぞれ $(a, x) \mapsto x\phi(a)$) を、B の左 (右) A-加群構造の B 定義するに入れます。特に、$\phi$ が A 上の恒等写像であるとみなされる場合、標準的な左 (それぞれ右) A-加群構造が A 上で取得されます。混乱を避けるため、集合 A とこの構造は、$A_s$ (それぞれ $A_d$) で表されます。

(2) 外部法則 $(n, x) \mapsto n.x$ (I, § 3, no. 1) で定義される演算子構造をもつ可換群 G (加法的に書かれた) 群では、加群構造は有理数の環 $\mathbf{Z}$ を超えます。 整数。

(3) E を加法的に書かれた可換群とし、E の $\mathscr{E}$ 自己準同型環 (I, § 8, no. 3: 2 つの自己準同型の積 $fg$ は合成定義によるものであることを思い出してください) 自己準同型 $f \circ g$)。 E 上の演算子 $f \in \mathscr{E}$ と元 $x \in E$ 定義するの間の外部法則 $(f, x) \mapsto f(x)$ は、正規の左 $\mathscr{E}$ モジュール構造です。

ここで環 A を考え、E に左 (右) A-加群構造が与えられていると仮定します。すべての $\alpha \in A$、ホモテティー $h_\alpha : x \mapsto \alpha x$ (それぞれ $x \mapsto x\alpha$) 属する ～ $\mathscr{E}$。 写像 $\phi : \alpha \mapsto h_\alpha$ は、環 A (それぞれ反対環 $A^0$) の準同型を環 $\mathscr{E}$ に、そして定義 $\alpha x = (\phi(\alpha))(x)$ (それぞれ $x\alpha = (\phi(\alpha))(x)$) によって変換されます。逆に、上記の式により、E の環準同型 $\phi : A \to \mathscr{E}$ (それぞれ $\phi : A^0 \to \mathscr{E}$) 定義するに左 (それぞれ右) A-加群構造を与えます。他の語では、加法群 E に加法法則を加えて左 (右) A-加群構造が与えられると、与えられた群法則は環準同型 $A \to \mathscr{E}$ (それぞれ右) が与えられるのと同等です。 $A^0 \to \mathscr{E}$）。

#### 定義 2 {#alg-ii-s1-def-2 .statement tag=05JQ}

*左 (右) ベクトル空間上体 K は左 (右) K-加群です。*

ベクトル空間の元は、*ベクトル* と呼ばれるときどきです。

#### 例 {#alg-ii-s1-n1-exa-2 .statement tag=05JR}

(4) 体は、その部分体のいずれかに対して左であり、右ベクトル空間の両方です。

*(5)* 3 つの次元 $\mathbf{R}^3$ のうち実数空間は、実数 $\mathbf{R}$、積 $tx$ の体に対してベクトル空間です実数 $t$ と点 $x$ の座標 $x_1, x_2, x_3$ は点で座標 $tx_1, tx_2, tx_3$ です。同様に、任意の集合 F 上で定義された実数値写像の集合は、実数 $t$ の $\mathbf{R}$、積 $tf$ に関してベクトル空間となります。 写像 $f$ は、実数値写像 $x \mapsto tf(x)$ です。*

2 つのファミリー $(x_i)_{i \in I}, (y_i)_{i \in I}$ of 元 of A-加群 E of 有限台 (I, § 2, no. 1) では、次の方程式が成り立ちます。

(1)
$$
\sum_{i \in I} (x_i + y_i) = \sum_{i \in I} x_i + \sum_{i \in I} y_i
$$

(2)
$$
\alpha \cdot \sum_{i \in I} x_i = \sum_{i \in I} (\alpha x_i) \quad \text{for all } \alpha \in A;
$$
方程式は、I 含むのサポート $(x_i)$ と $(y_i)$ の有限部分集合 H を考慮することにより、有限和の類似方程式に直ちに還元されます。

#### 定義 3 {#alg-ii-s1-def-3 .statement tag=05JS}

* A-加群 E の元 x は、A の元の有限台の家族元の家族 $(\lambda_i)_{i \in I}$ が存在する場合、E の家族元の $(a_i)_{i \in I}$ の A に係数が含まれる線形結合であると言われます。 $x = \sum_{i \in I} \lambda_i a_i$.*

一般に、$(\lambda_i)$ 満たす、この条件 (cf. no. 11) という異なるファミリーがいくつかあります。

0 は、E の元の空の族の唯一の線形結合であることに注意してください (I, § 2, no. 1 の規則により)。

### 2. 線形写像

#### 定義 4 {#alg-ii-s1-def-4 .statement tag=05JT}

E と F を、同じ環 A に関して 2 つ (左) 加群とします。 E から F への線形写像 (または A-線型写像、または準同型、または A 準同型射) は、次のような任意の写像 u : E → F です。

(3) $x \in E, y \in E;$ の場合は $u(x + y) = u(x) + u(y)$

(4G) $u(\lambda . x) = \lambda . u(x)$ の $\lambda \in A, x \in E.$

E と F が 2 つの右A-加群である場合、線形写像 $u : E \to F$ は写像満たす (3) および

(4D) $u(x . \lambda) = u(x) . \lambda$ 対 $\lambda \in A, x \in E.$

#### 注意 {#alg-ii-s1-n2-rem-1 .statement tag=05JU}

E と F が 2 つの可換群で、環 $\mathbf{Z}$ (no. 1) 上の加群とみなされる場合、群 E (演算子なし) から群 F (演算子なし) へのすべての準同型 $u$ も同様です。 n 整数 > 0 の場合、関係 $u(n . x) = n . u(x)$ は、n の帰納法によって $u(x + y) = u(x) + u(y)$ から続き、$n = -m < 0$ では、E の線形写像を F に変換します。
$$
u(n . x) = u(-(m . x)) = -u(m . x) = -(m . u(x)) = n . u(x).
$$

#### 例 {#alg-ii-s1-n2-exa-1 .statement tag=05JV}

(1) E を A-加群および E の元とする。 A-加群 $A_s$ の写像 $\lambda \mapsto \lambda a$ を E にすると、線形写像 $\theta_a$ となり、$\theta_a(1) = a.$
*(2) I を実直線 $\mathbf{R}$ の開区間、I 上の微分可能な実数値写像の E ベクトル空間、および上で定義されたすべての実数値写像の F ベクトル空間とします。 I。 写像 $x \mapsto x'$ は、微分可能なすべての写像 x と関連付けられ、その導関数は E から F までの線形写像です。*

A-加群 E 上のホモテティー $x \mapsto \alpha x$ は必ずしも線形写像ではないことに注意してください。他の語、関係 $\alpha(\lambda x) = \lambda(\alpha x)$ は、必ずしもすべての $\lambda \in A$ と $x \in E$ に当てはまります。ただし、この関係は、A の $\alpha$ 属するから中心の場合に当てはまります。その後、$x \mapsto \alpha x$ は中央のホモテティー (cf. no. 13) と呼ばれます。

$u : E \to F$ が線形写像である場合、E の元のすべての家族 $(x_i)_{i \in I}$ と A の元のすべての家族 $(\lambda_i)_{i \in I}$ について、家族 $(\lambda_i x_i)_{i \in I}$ の支援が有限であるように、

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i)
$$

家族$(\lambda_i x_i)$のサポート基数の帰納法により、(3)と(4G)からすぐに次のようになります。

#### 命題 1 {#alg-ii-s1-prop-1 .statement tag=05JW}

E、F、G を 3 つの A-加群、E から F への u 線形写像、F から G への v 線形写像とします。すると、合成写像 $v \circ u$ は線形になります。

(1) *u:E → F と v:F → E が 2 つの線形写像で、v ∘ u が E 上で恒等写像で、u ∘ v が F 上で恒等写像である場合、u は F 上で E の同型で、v は逆同型です。*

(2) *すべての全単射線形写像 u:E → F は、E から F への同型です。*

これらの命題は、定義 4 の直後に続きます。

命題 1 と 2 は、線形写像が A-加群構造 (*集合理論*, IV, § 2, no. 1) の種の *射* として解釈できることを示しています。今後は常にこの射の選択が作成されたものと仮定します。

2 つの左 (それぞれ右) A-加群 E と F が与えられた場合、Hom(E, F) または Hom_A(E, F) が E の線形写像の集合を F に表すものとします。

集合 Hom(E, F) は、E のすべての写像を F (I, § 4, no. 8) に変換する *可換環*、部分群積の可換群 F^E です。 F^E の 2 つの元 u, v とすべての x ∈ E について、

$$(u + v)(x) = u(x) + v(x), \quad (-u)(x) = -u(x)$$

よって u と v が線形であれば、u + v と −u も線形であることがすぐにわかります。 G が Hom(E, F) の 3 番目の左 (それぞれ右) A-加群, f, f_1, f_2 元と Hom(F, G) の g, g_1, g_2 元である場合、次の関係が直ちに検証されます。

(6) $$g \circ (f_1 + f_2) = g \circ f_1 + g \circ f_2$$
(7) $$(g_1 + g_2) \circ f = g_1 \circ f + g_2 \circ f$$
(8) $$g \circ (-f) = (-g) \circ f = -(g \circ f).$$

特に、Hom(E, E) 定義する上の合成 (f, g) ↦ f ∘ g の法則と、上記加法群構造 a *環* 構造 on Hom(E, E) の単位元は、1_E またはで示されます。 Id_E は E の恒等写像です。 E の線形写像はそれ自体に含まれる A-加群 E の *自己準同型* とも呼ばれ、環 Hom(E, E) は End(E) または End_A(E) とも表されます。 A-加群 E の *自己同型* は、End(E) (命題 2) の *可逆* 元です。それら形は Aut(E) または GL(E) で示される乗法 *群* であり、E に対する *線形群* とも呼ばれます。

(6) と (7) から、2 つの A-加群 E, F に対して、Hom(E, F) は、環 Hom(F, F) 上の *左加群* と Hom(E, E) 上の *正しい加群* の正規構造を持つことがわかります。

E、F、E'、F' を 4 つ (左) A-加群、u:E' → E および v:F → F' A-線型写像とします。すべての元 f ∈ Hom(E, F) が元 v ∘ f ∘ u ∈ Hom(E', F') に関連付けられている場合、写像

$$\operatorname{Hom}(E, F) \to \operatorname{Hom}(E', F')$$

が定義されており、$\mathbf{Z}$-線形であり、$\mathrm{Hom}(u, v)$ または $\mathrm{Hom}_A(u, v)$ で表されます。 $u, u_1, u_2$ 属するから $\mathrm{Hom}(E', E)$ および $v, v_1, v_2$ から $\mathrm{Hom}(F, F')$ の場合、

$$
\begin{cases}
\mathrm{Hom}(u_1 + u_2, v) = \mathrm{Hom}(u_1, v) + \mathrm{Hom}(u_2, v) \\
\mathrm{Hom}(u, v_1 + v_2) = \mathrm{Hom}(u, v_1) + \mathrm{Hom}(u, v_2)
\end{cases}
$$

$E'', F''$ を 2 つの $A$ モジュール、$u': E'' \to E'$ と $v': F' \to F''$ 線形写像とします。それから

$$
\mathrm{Hom}(u \circ u', v' \circ v) = \mathrm{Hom}(u', v') \circ \mathrm{Hom}(u, v).
$$

$u$ が $E'$ の $E$ への同型写像であり、$v$ が $F$ の $F'$ への同型写像である場合、$\mathrm{Hom}(u, v)$ は $\mathrm{Hom}(E, F)$ の $\mathrm{Hom}(E', F')$ への同型写像であり、その逆同型は (10) により $\mathrm{Hom}(u^{-1}, v^{-1})$ になります。

$h$ (それぞれ $k$) が $E$ (それぞれ $F$) の準同型である場合、$\mathrm{Hom}(h, 1_F)$ (それぞれ $\mathrm{Hom}(1_E, k)$) は、リング上の右 (それぞれ左) モジュール構造の比 $h$ (それぞれ $k$) との相似です。 $\mathrm{End}(E)$ (それぞれ $\mathrm{End}(F)$) は上記で定義されています。

### 3. 部分加群; 商加群

$E$ を $A$ モジュール、$M$ を $E$ のサブセットとします。 $E$の$A$加群構造が$M$の$A$加群構造を誘導するには、$M$が$E$(I, § 4, no. 3)の安定な部分群であることが必要かつ十分です。なぜなら、そうであれば、$M$で誘導された演算子を含む群の構造は明らかになります。公理 ($M_{II}$)、($M_{III}$)、および ($M_{IV}$) を満たします。この構造を持つ $M$ (または、言葉の乱用により、セット $M$ 自体) は、$E$ のサブモジュールと呼ばれます。正規注入 $M \to E$ は線形マッピングです。 $E$ がベクトル空間の場合、その部分加群はベクトル部分空間 (または、混乱が生じない場合は単に部分空間 ) と呼ばれます。

#### 例 {#alg-ii-s1-n3-exa-1 .statement tag=05JX}

(1) 0 の任意の加群 $E$ 集合からなるは部分加群 (零部分加群、記法の乱用により 0 で表されることがよくあります) です。
(2) $A$ を環とします。 $A_s$ (それぞれ $A_d$) の部分加群は、環 $A$ の左の理想 (それぞれ右の理想) にすぎません。
(3) $E$ を $A$ 加群、$x$ 元を $E$、$a$ を $A$ の左イデアルとする。 $\alpha$ が $a$ を通る元 $\alpha x$ の集合は、$ax$ で示される $E$ の部分加群です。
(4) 可換群 $G$ を $\mathbf{Z}$ 加群 (no. 1) とみなすと、$G$ のすべての部分群も部分加群になります。

*(5) $I$ を実直線 $\mathbf{R}$ のオープン区間とします。 $I$ で定義され連続する実数値写像の集合 $C$ は、$I$ で定義されたすべての実数値写像のベクトル空間 $\mathbf{R}^I$ のベクトル部分空間です。同様に、$I$ 上の微分可能写像の集合 $D$ は、$C_*$* のベクトル部分空間です

$E$ を $A$ モジュールとします。 $E$ 上の加群構造と互換性のあるすべての同値関係 (I, § 1, no. 6) は、形 $x - y \in M$ です。ここで、$M$ は E (I, § 4, no. 4) の安定した部分群、つまり E の部分加群です。 剰余群に演算子を使用した群の構造 E/M (I, § 4, no. 4) は A-加群構造であり、その下では標準写像 $E \to E/M$ は線形です。この構造により、E/M は部分加群 M によって E の *商加群* と呼ばれます。 ベクトル空間 E の商加群は E の *商ベクトル空間* (または単に *商空間*) と呼ばれます。

*例* (6)。 左A-加群 $A_s$ の環定義する商加群 $A_s/a$ の左すべての理想 $a$。 記法の乱用により、この商加群は$A/a$で表されることがよくあります。

E、F を 2 A-加群とします。演算子 (I, § 4, no. 5) を使用した群 (または直接定義) から、$u : E \to F$ が線形写像の場合、E の部分加群の $u$ の下の像は F の部分加群であり、逆像であることがわかります。 F の任意の部分加群の $u$ は E の部分加群です。特に、*核* $N = \overline{u}^{-1}(0)$ は E の部分加群であり、$u$ の下の E の像 $u(E)$ は F の部分加群です(I, § 4, no. 6、命題 7);言葉の乱用により、$u(E)$ は u* の *像と呼ばれます。 商加群 $E/N$ は $u$ の *商加群 $F/u(E)$ は $u$ の *余核* とも呼ばれます。 $u$ (I, § 4, no. 5) の *標準分解*

$$
u : E \xrightarrow{p} E/N \xrightarrow{v} u(E) \xrightarrow{i} F
$$

$v$ は、$u$ (no. 2、命題 2) の像上に $u$ の共像の *同型* です。 $u$ が*単射*であるためには、その核が零であることが必要かつ十分です。 $u$ が*全射*であるためには、その余核が零であることが必要かつ十分です。

$u$ の核、像、coimage、余核は、それぞれ Ker $u$、Im $u$、Coim $u$、Coker $u$ で表されます。

#### 注意 {#alg-ii-s1-n3-rem-1 .statement tag=05JY}

M を A-加群 E および $\phi : E \to E/M$ 標準準同型の部分加群とします。 A-線型写像 $u : E \to F$ が形 $v \circ \phi$ になるためには、$v$ が E/M の線形写像を F に変換したものであるため、$M \subset \mathrm{Ker}(u)$ であることが必要かつ十分です。なぜなら、もしこの条件が成り立つなら、関係$x - y \in M$は$u(x) = u(y)$を意味するので、$u$はこの同値関係と互換性があり、商を取ることによって$u$から導出された写像$v : E/M \to F$は明らかに線形であるからです。

### 4. 完全系列

#### 定義 5 {#alg-ii-s1-def-5 .statement tag=05JZ}

*F、G、H を 3 つ A-加群とします。 f を F から G への準同型とし、G から H への g 準同型とします。順序付けられた対 (f, g) は完全系列と呼ばれます。

$$
g^{-1}(0) = f(F)
$$

*その他の語では、g の核が f の像と等しい場合。*

図式

(12)
$$
F \xrightarrow{f} G \xrightarrow{g} H
$$
は *完全系列* とも呼ばれます。

4 つの A-加群と 3 つの準同型のうち図式からなるも同様に考えます。

(13)
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

図式 $E \xrightarrow{f} F \xrightarrow{g} G$ が正確である場合、この図式は *正確な* F と呼ばれます。 $F \xrightarrow{g} G \xrightarrow{h} H$ が正確である場合、それは *G で正確であると呼ばれます。 図式 (13) が *F * および * G で *正確である場合、それは単に *正確*、または *完全系列* と呼ばれます。 項の任意の数を含む完全系列も同様に定義されます。

#### 注意 {#alg-ii-s1-n4-rem-1 .statement tag=05K0}

(1) 注文した対 $(f, g)$ が完全系列の場合、$g \circ f = 0$。しかしもちろん、この性質は完全系列を特徴付けるものではなく、$f$の像が$g$の核に*含まれる*ことを意味するだけだからです。

以下の主張では、E、F、G は A-加群、0 A-加群はその単位元に縮小されます。矢印は A-加群準同型を表します。 As there is only one 準同型 from 加群 0 to 加群 E (resp. of E to 0), there is no 点 in giving these 準同型 a name in 完全系列 where they appear.

#### 命題 3 {#alg-ii-s1-prop-3 .statement tag=05K1}

(a) *対象*
$$
0 \longrightarrow E \xrightarrow{f} F
$$
*完全系列であるためには、* $f$ *単射的*であることが必要かつ十分です。

(b) *対象*
$$
E \xrightarrow{f} F \longrightarrow 0
$$
*完全系列であるためには、* $f$ *全射的*であることが必要かつ十分です。

(c) *対象*
$$
0 \longrightarrow E \xrightarrow{f} F \longrightarrow 0
$$
*完全系列であるためには、* $f$ *全単射*であることが必要かつ十分です (他の語 (no. 2、命題 2) では、$f$ は E から F への *同型* である)。

(d) *F * が * E * の部分加群で、* $i : F \to E$ * が標準単射である場合、* $p : E \to E/F$ *標準準同型、図式*
(14)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0
$$
*は完全系列です*

(e) *$f : E \to F$が準同型の場合、図式*

$$
0 \longrightarrow f^{-1}(0) \overset{i}{\longrightarrow} E \overset{f}{\longrightarrow} F \overset{p}{\longrightarrow} F/f(E) \to 0
$$

*($i$ は標準単射および $p$ 標準全射) は完全系列です。*

命題は、no. 2 の定義と命題 2 の直後に続きます。

#### 注意 {#alg-ii-s1-n4-rem-2 .statement tag=05K2}

(2) 完全系列があると言う事

$$
0 \longrightarrow E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \longrightarrow 0
$$

は、$f$ が単射的で、$g$ が全射的であり、$g$ に関連付けられた正規の全単射が $G$ に対する $F/f(E)$ の *同型* であることを意味します。トリプル$(F, f, g)$は、加群Gの加群E*(I, § 6, no. 7)の*拡大であるとも言われています。

(3) 項が4つで完全系列がある場合

$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \overset{h}{\longrightarrow} H
$$

$f$の余核は$F/f(E) = F/g^{-1}(0)$、$h$の核は$g(F)$です。したがって、$g$ に関連付けられた正規の全単射は *同型* です

$$
\operatorname{Coker} f \to \operatorname{Ker} h.
$$

(4) A-加群準同型の順序付き対を考えます

$$(15)$$
$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G.
$$

図式 (15) が完全系列であるためには、2 つの A-加群 S、T と準同型 $a : E \to S,\ b : S \to F,\ c : F \to T,\ d : T \to G$ が存在し、3 つの数列が成立することが必要かつ十分です。

$$(16)$$
$$
\begin{cases}
E \overset{a}{\longrightarrow} S \longrightarrow 0 \\
0 \longrightarrow S \overset{b}{\longrightarrow} F \overset{c}{\longrightarrow} T \longrightarrow 0 \\
0 \longrightarrow T \overset{d}{\longrightarrow} G
\end{cases}
$$

は *正確* で、$f = b \circ a$ と $g = d \circ c$ です。

(15) が完全系列の場合、$f$ と同じグラフで、$S = f(E) = g^{-1}(0)$ と $T = g(F)$、$b$ と $d$ が標準単射と $a$ (それぞれ $c$) 準同型になります。 (それぞれ $g$)。逆に、S、T、a、b、c、d 満たすが上記の条件である場合、$f(E) = b(a(E)) = b(S)$ と $g^{-1}(0) = c(d(0)) = c(0)$ となるため、(16) の正確性は $f(E) = g^{-1}(0)$ を示します。

完全系列の準同型を示す明示的な文字の使用は、引数に必要がない場合には省略されることがよくあります。

#### 注意 {#alg-ii-s1-n4-rem-3 .statement tag=05K3}

(5) 完全系列拡大するの定義から群への直接変換は必ずしも可換ではありません。この場合はもちろん、乗法記法が式内で 0 を 1 に置き換えて使用されます (混乱が生じない場合)。 命題 3 の部分 (a)、(b)、(c) は依然として有効であり、(d) F が E の正規部分群の場合も有効です。 注意 2 および命題 3(e) $f(E)$ が正規である条件が保持されます。 Fの部分群; 注意 3 と 4 はそのまま有効です。

### 5. 積/加群

$(E_i)_{i \in I}$ を同じ環 A 上の加群の族とします。$E_i$ ($I, § 4,$ no. 8) 上の加群構造の積がA-加群構造であることがすぐに検証されます。 積集合 $E = \prod_{i \in I} E_i$。これにより、構造集合 E は加群 $E_i$ の積加群と呼ばれます。 $x = (x_i), y = (y_i)$ が E の 2 つの元である場合、

$$
\begin{cases}
x + y = (x_i + y_i) \\
\lambda \cdot x = (\lambda x_i)
\end{cases}
$$
すべての$\lambda \in A$のために。

式 (17) は、射影 $pr_i : E \to E_i$ が線形写像であることを表します。これらの写像は明らかに全主観的です。

インデックス集合 I が空の場合、積集合 $\prod_{i \in I} E_i$ は単一の元で構成されることを思い出してください。この集合上の積加群構造は、この一意元が 0 となるものです。

#### 命題 4 {#alg-ii-s1-prop-4 .statement tag=05K4}

*$E = \prod_{i \in I} E_i$ *A-加群* $(E_i)_{i \in I}$ の家族の積としましょう。 *すべての A-加群* F * と線形写像* $f_i : F \to E_i$ のすべての族に対して、 *1 つだけの写像* f *of* F *into* E *が存在します* $pr_i \circ f = f_i$ *すべてについて* $i \in I$ *そしてこの写像は線形*です。

これは定義から直接続きます。

加群の積は「連想」です: $(J_\lambda)_{\lambda \in L}$ が I の分割である場合、標準写像
$$
\prod_{i \in I} E_i \to \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} E_i \right)
$$
同型です。

#### 命題 5 {#alg-ii-s1-prop-5 .statement tag=05K5}

(i) *$(E_i)_{i \in I}, (F_i)_{i \in I}$ * を、同じインデックス集合* I を持つ A-加群の 2 つのファミリーとします。 *線形写像* $f_i : E_i \to F_i$ ($i \in I$)、*写像* $f : (x_i) \to (f_i(x_i))$ *の* $\prod_i E_i$ *に* $\prod_i F_i$ *(ときどきは* $\prod_i f_i$で示される) *線型*です。

(ii) *$(G_i)_{i \in I}$ *を A-加群の 3 番目の族とし、* I * をインデックスとして集合とし、すべての * $i \in I,$ を $g_i : F_i \to G_i$ を線形写像とする。 $g = \prod_i g_i$ にしましょう。正確には、数列 $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ のそれぞれについて、数列であることが必要かつ十分です。

$$
\prod_i E_i \xrightarrow{f} \prod_i F_i \xrightarrow{g} \prod_i G_i
$$

正確に言ってください。

主張 (i) は定義の直後に続きます。一方、$y = (y_i)$ 属するから $\operatorname{Ker}(g)$ と言うと、すべての $i \in I$ に対して $g_i(y_i) = 0$ となり、したがってすべての $i \in I$ に対して $y_i \in \operatorname{Ker}(g_i)$ となることを意味します。同様に、$y$ 属するから $\operatorname{Im}(f)$ ということは、$y = f(x)$ のような $x = (x_i) \in \prod_i E_i$ が存在することを意味します。これは、すべての $i \in I$ に対して $y_i = f_i(x_i)$、またはすべての $i \in I$ に対して $y_i \in \operatorname{Im}(f_i)$ であるというと同等です。 よって (ii)。

#### 系 {#alg-ii-s1-n5-cor-1 .statement tag=05K6}

命題 5 の条件の下で、(i)、

$$
\operatorname{Ker}(f) = \prod_{i \in I} \operatorname{Ker}(f_i), \qquad \operatorname{Im}(f) = \prod_{i \in I} \operatorname{Im}(f_i)
$$

そして標準同型があります

$$
\operatorname{Coim}(f) \to \prod_{i \in I} \operatorname{Coim}(f_i), \qquad \operatorname{Coker}(f) = \prod_{i \in I} \operatorname{Coker}(f_i)
$$

それぞれ、$\prod_i E_i$、mod $\operatorname{Ker}(f)$ の要素 $x = (x_i)$ のクラス、(それぞれ $\prod_i F_i$、mod. $\operatorname{Im}(f)$ の要素 $y = (y_i)$ のクラス) $x_i$ mod のクラスのファミリーと関連付けることによって取得されます。 $\operatorname{Ker}(f_i)$ (それぞれ、$y_i$ mod. $\operatorname{Im}(f)$ のクラスのファミリー)。

特に、$f$ が単射法 (それぞれ全単射、全単射、零) であるためには、すべての $i \in I$、$f_i$ が単射法 (それぞれ全単射、全単射、零) であることが必要かつ十分です。

すべての $i \in I$ について、$E_i$ の部分加群 $F_i$ を考慮すると、加群 $\prod_{i \in I} F_i$ は $\prod_{i \in I} E_i$ の部分加群であり、系から命題 5 により、標準同型が存在します。

$$
\prod_{i \in I} (E_i/F_i) \to \left( \prod_{i \in I} E_i \right) / \left( \prod_{i \in I} F_i \right).
$$

重要な加群の積の例は、すべての因子加群が同じ加群$F$に等しいということです。彼らの積 $F^I$ は、$I$ の写像の集合が $F$ になります。 $I$ の $x$ に等しい定数写像への対角線写像 $F \to F^I$ 写像 $x \in F$ は線形です。 $(E_i)_{i \in I}$ が $A$ モジュールのファミリーで、すべての $i \in I$ について、$f_i : F \to E_i$ が線形写像である場合、線形写像 $F$ の $x \mapsto (f_i(x))$ を $\prod_{i \in I} E_i$ に加えると、写像の合成になります。 $F^I$の$(x_i) \mapsto (f_i(x_i))$を$\prod_{i \in I} E_i$と対角写像$F \to F^I$にします。

### 6. 加群中直和

$(E_i)_{i \in I}$ を A-加群と $F = \prod_{i \in I} E_i$ の積の家族としましょう。 添字の有限の数を除いて $\mathrm{pr}_i x = 0$ が明らかに $F$ の部分加群であるような $x \in F$ の集合 $E$ は、次の族の外部直和 (または単に直和) と呼ばれます。 加群 $(E_i)$ であり、$\bigoplus_{i \in I} E_i$ (I, § 4, no. 9) で示されます。 I が有限の場合、$\bigoplus_{i \in I} E_i = \prod_{i \in I} E_i$; $I = \{p, q\}$ ($\mathbf{Z}$ の区間) の場合は、次のようにも書きます

$$
\bigoplus_{i \in I} E_i = E_p \oplus E_{p+1} \oplus \cdots \oplus E_q.
$$

すべての $\kappa \in I$ について、$j_\kappa$ を、$i \neq \kappa$ と $\mathrm{pr}_\kappa(j_\kappa(x_\kappa)) = x_\kappa$ に対して $\mathrm{pr}_i(j_\kappa(x_\kappa)) = 0$ となるように、$F$ の各 $x_\kappa \in E_\kappa$ に関連付けるマッピング $E_\kappa \to F$ とします。 $j_\kappa$ が $E_\kappa$ の $E_i$ の直和 $E$ への単射線形写像であることがすぐに分かります。これを正準射出と呼びます。 $E$ のサブモジュール $j_\kappa(E_\kappa)$ は、$E_\kappa$ と同型で、インデックス $\kappa$ の $E$ のコンポーネントサブモジュールと呼ばれます。 $j_\kappa$ によって $E_\kappa$ と識別されることがよくあります。

したがって、すべての $x \in E = \bigoplus_{i \in I} E_i$ にとって、私たちは

$$
x = \sum_{i \in I} j_i(\mathrm{pr}_i x).
$$

(20)

#### 命題 6 {#alg-ii-s1-prop-6 .statement tag=05K7}

*$(E_i)_{i \in I}$ * を A-加群*、$M$ *A-加群の家族とし、* $i \in I$ 全員を * $f_i : E_i \to M$ * 線形写像* とします。 *そして、唯一の線形写像* $g : \bigoplus_{i \in I} E_i \to M$ *すべてに対して* $i \in I$:

$$
g \circ j_i = f_i.
$$

(21)

(20) により、$g$ が存在する場合、必然的にすべての $x \in \bigoplus_{i \in I} E_i$ について、

$$
g(x) = \sum_i g(j_i(\mathrm{pr}_i(x))) = \sum_i f_i(\mathrm{pr}_i(x)),
$$

$g$ のよって一意性。逆に、すべての $x \in \bigoplus_{i \in I} E_i$ に対して設定 $g(x) = \sum_i f_i(\mathrm{pr}_i(x))$ があれば、線形写像が主張の満たす条件に定義されていることが直ちに検証されます。

混乱が生じない場合は、$g = \sum_{i \in I} f_i$ と書きます (これは、家族 $(f_i)$ が有限台ではない場合、I, § 2, no. 1 の規則に反します)。

In particular, if J is any subset of I, the canonical injections $j_i$ for $i \in J$ define a canonical linear mapping $j_J : \bigoplus_{i \in J} E_i \to \bigoplus_{i \in I} E_i$, which associates with each $(x_i)_{i \in I}$ the element $(x'_i)_{i \in I}$ such that $x'_i = x_i$ for $i \in J$, $x'_i = 0$ for $i \notin J$; this mapping is obviously injective. さらに、$(J_\lambda)_{\lambda \in L}$がIの分割である場合、命題6による家族$(j_{J_\lambda})$に対する写像$i : \bigoplus_{\lambda \in L} \left( \bigoplus_{i \in J_\lambda} E_i \right) \to \bigoplus_{i \in I} E_i$対応するは正準（直和の「結合性」）と呼ばれる*同型*です。

#### 系 1 {#alg-ii-s1-prop-6-cor-1 .statement tag=05K8}

※$(E_i)_{i \in I}, (F_\lambda)_{\lambda \in L}$をA-加群の2つの家族とします。 写像*
$$
\text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) \to \prod_{(i, \lambda) \in I \times L} \text{Hom}_A(E_i, F_\lambda)
$$
*それぞれの $g \in \text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right)$ ファミリー $(\operatorname{pr}_\lambda \circ g \circ j_i)$ に関連する、 $\mathbf{Z}$ モジュール同型 (正規と呼ばれます)。

これは、命題 6 と no. 5、命題 4 から続きます。

#### 系 2 {#alg-ii-s1-prop-6-cor-2 .statement tag=05K9}

*$(E_i)_{i \in I}$ を A-加群、F A-加群の家族とし、それぞれの $i \in I$ について、$f_i : E_i \to F$ を線形写像とします。 $f = \sum_{i \in I} f_i$ が F 上で $E = \bigoplus_{i \in I} E_i$ の同型になるためには、以下の特性を持つ各 $i \in I$ 線形写像 $g_i : F \to E_i$ が存在することが必要かつ十分です:*
(1) $i \in I$ 全員に対して $g_i \circ f_i = 1_{E_i}$。
(2) $i \neq \kappa$の場合は$g_i \circ f_\kappa = 0$。
(3) *すべての $y \in F$ に対して、家族 $(g_i(y))$ には有限台があり、*
$$
y = \sum_{i \in I} f_i(g_i(y)).
$$
I が有限の場合、最後の条件は次のように書くこともできることに注意してください。
$$
\sum_{i \in I} f_i \circ g_i = 1_F.
$$
$g_i = \operatorname{pr}_i \circ f_i^{-1}$ で満足するには、明らかに条件が必要です。逆に、それらが成り立つ場合、すべての $y \in F$ について、$g(y) = \sum_i j_i(g_i(y))$ が定義され、$g$ は F から E への線形写像であることは明らかです。すべての $y \in F$、$f(g(y)) = \sum_i f_i(g_i(y)) = y$ は仮定によります。一方、すべての $x \in E$、$g_\kappa(f(x)) = g_\kappa \left( \sum_i f_i(\operatorname{pr}_i(x)) \right) = g_\kappa(f_\kappa(\operatorname{pr}_\kappa(x))) = \operatorname{pr}_\kappa(x)$ については、仮定によるものです。

したがって $g(f(x)) = \sum_i j_i(g_i(f(x))) = \sum_i j_i(\mathrm{pr}_i(x)) = x$ となり、系が証明されます。

#### 命題 7 {#alg-ii-s1-prop-7 .statement tag=05KA}

(i) *$(E_i)_{i \in I}, (F_i)_{i \in I}$ *同じインデックス集合* $I$ を持つ* $A$* モジュールの 2 つのファミリーとします。 *線形写像* $f_i : E_i \to F_i$ ($i \in I$)、*制限から* $\bigoplus_{i \in I} E_i$ *線形写像* $(x_i) \mapsto (f_i(x_i))$ *は線形写像* $f : \bigoplus_{i \in I} E_i \to \bigoplus_{i \in I} F_i$ *で表されます* $\bigoplus_{i \in I} f_i$ *または* $\bigoplus_i f_i$ *(ここで* $f = f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ *if* $I = [p, q]$ *は区間 in* $\mathbf{Z}$*).*

(ii) *$(G_i)_{i \in I}$ * を 3 番目のファミリー * $A$* モジュールとし、* $I$ * インデックスとして集合を使用し、すべての * $i \in I$ を * $g_i : F_i \to G_i$ * 線形写像とします。 * $g = \bigoplus_i g_i$ と書きます。 *それぞれの数列* $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ *正確には、 数列* であることが必要十分です
$$
\bigoplus_i E_i \xrightarrow{f} \bigoplus_i F_i \xrightarrow{g} \bigoplus_i G_i
$$
*正確に*。

明らかに、すべての $(x_i) \in \bigoplus_i E_i$ に対して、ファミリー $(f_i(x_i))$ には有限台、よって (i) があります。一方、$\bigoplus_i F_i$ 属するから $\mathrm{Ker}(g)$ の元 $y = (y_i)$ は、$i \in I$ (no. 5, 命題 5) 全てに対して $y_i \in \mathrm{Ker}(g_i)$ を意味します。同様に、すべての $i \in I$ に対して $y_i \in \mathrm{Im}(f_i)$ の場合、各 $i \in I$ には $y_i = f_i(x_i)$ のような $x_i \in E_i$ が存在し、$y_i = 0$ の場合は $x_i = 0$ であると考えられます。したがって、$y \in \mathrm{Im}(f)$ と逆は明らかです。

#### 系 1 {#alg-ii-s1-prop-7-cor-1 .statement tag=05KB}

*命題 7 の条件の下、(i)、*
$$
\mathrm{Ker}(f) = \bigoplus_{i \in I} \mathrm{Ker}(f_i), \qquad \mathrm{Im}(f) = \bigoplus_{i \in I} \mathrm{Im}(f_i)
$$
*そして標準同型*もあります
$$
\mathrm{Coim}(f) \to \bigoplus_{i \in I} \mathrm{Coim}(f_i), \qquad \mathrm{Coker}(f) \to \bigoplus_{i \in I} \mathrm{Coker}(f_i)
$$
*no. 5、系 ～ 命題のように定義されます。 5. 特に、* $f$ * が単射詞 (それぞれ全単射、全単射、零) であるためには、* $f_i$ * がそれぞれ単射詞 (それぞれ全単射、全単射、 零)*。

すべての $i \in I$ について、$E_i$ の部分加群 $F_i$ を考慮すると、加群 $\bigoplus_{i \in I} F_i$ は $\bigoplus_{i \in I} E_i$ の部分加群であり、系 1 ～ 命題 7 により、標準同型が存在します。
$$
\bigoplus_{i \in I} (E_i/F_i) \to \left( \bigoplus_{i \in I} E_i \right) / \left( \bigoplus_{i \in I} F_i \right).
$$

#### 系 2 {#alg-ii-s1-prop-7-cor-2 .statement tag=05KC}

$(E_i)_{i \in I}, (E'_i)_{i \in I}, (F_\lambda)_{\lambda \in L}, (F'_\lambda)_{\lambda \in L}$ を 4 つの $A$ モジュールのファミリーとし、各 $i \in I$ (それぞれ $\lambda \in L$)、$u_i : E'_i \to E_i$ (それぞれ $v_\lambda : F_\lambda \to F'_\lambda$) 線形写像とします。それから図式

$$
\begin{array}{ccc}
\operatorname{Hom}\left( \bigoplus_{i \in I} E'_i, \prod_{\lambda \in L} F'_\lambda \right) & \xrightarrow{\phi'} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E'_i, F'_\lambda) \\
\uparrow & & \uparrow \\
\operatorname{Hom}\left( \bigoplus_i u_i, \prod_\lambda v_\lambda \right) & & \prod \operatorname{Hom}(u_i, v_\lambda) \\
\operatorname{Hom}\left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) & \xrightarrow{\phi} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E_i, F_\lambda)
\end{array}
$$

($\phi$ と $\phi'$ は系 1 から命題 6 で定義された標準同型です) は可換です。

検証は定義からすぐに続きます。

すべての $E_i$ が同じ $A$ モジュール $E$ に等しい場合、直和 $\bigoplus_{i \in I} E_i$ も $E^{(I)}$ で表されます。その元は、$I$ の写像が有限台で $E$ になります。すべての $i$、$f_i$ が恒等写像 $E \to E$ であるとすると、命題 6 によって、線形写像 $E^{(I)} \to E$ が得られ、*共対角* と呼ばれ、これは、すべての家族 $(x_i)_{i \in I}$ の元と関連付けられます。 $E$、有限台の*和* $\sum_{i \in I} x_i$。

#### 注意 {#alg-ii-s1-n6-rem-1 .statement tag=05KD}

直和拡大するの定義が *群* の族 $(E_i)_{i \in I}$ に直接結合することを思い出してください。これは必ずしも可換ではなく、乗法記法もちろん置き換えること加法記法です。その場合、「*直和*」 (I, § 4, no. 9) の代わりに、「*制限付き積*」 または 「*制限付き和*」 と言います。

$E$ は積 $F = \prod_{i \in I} E_i$ の *通常* 部分群であり、それぞれの $j_k(E_k)$ は $F$ の *通常* 部分群であることに注意してください。さらに、2 つの異なる添字 $\lambda, \mu$ では、$j_\lambda(E_\lambda)$ のすべての元は、$j_\mu(E_\mu)$ のすべての元と *置換可能* です。 命題 6 拡大するを、仮定の一般的なケースに当てはめます。つまり、2 つの異なる添字 $\lambda, \mu$ について、$f_\lambda(E_\lambda)$ のすべての元は、$f_\mu(E_\mu)$ のすべての元とともに、$M$ で *置換可能* になります。 (I, § 4, no. 9、命題12)。この直後に、制限付き和の「*結合性*」の性質が続きます。 命題 7 とその系 1 および 2 は修正なしで成立します。

### 7. 部分加群の共通部分と和

$A$ モジュール $E$ の各ファミリー $(M_i)_{i \in I}$ の部分加群では、共通部分 $\bigcap_{i \in I} E_i$ は $E$ の部分加群です。 それぞれの $i \in I$、$\phi_i$ が正準準同型 $E \to E/M_i$ を表す場合、$\bigcap_{i \in I} M_i$ は $E$ から $\prod_{i \in I} (E/M_i)$ への準同型 $\phi : x \mapsto (\phi_i(x))$ の *カーネル* です。つまり、*正確なシーケンス* が存在します。

$$
0 \longrightarrow \bigcap_{i \in I} M_i \longrightarrow E \xrightarrow{\phi} \prod_{i \in I} (E/M_i).
$$

線形写像 $\phi$ と写像
$$
E / \left( \bigcap_{i \in I} M_i \right) \to \prod_{i \in I} (E / M_i)
$$
移行から商によって得られるものを正規と呼びます。

特に：

#### 命題 8 {#alg-ii-s1-prop-8 .statement tag=05KE}

*家族* $(M_i)_{i \in I}$ *of 部分加群 of* $E$ *が共通部分を* $0$ *E は正準的に $\prod_{i \in I} (E / M_i)$ の部分加群と同型です。

$A$ モジュール $E$ の部分集合 $X$ の場合、$E$ 含む $X$ の部分加群の共通部分 $F$ は、$X$ によって部分加群 *生成* と呼ばれます。 $X$ は、$F$ (I, § 4, no. 3) の *生成する集合* (または *生成する系*) と呼ばれます。 $E$の元の家族$(a_i)_{i \in I}$の場合、$a_i$の集合によって生成された部分加群は、家族$(a_i)$によって生成された部分加群と呼ばれます。

$A$ モジュールは、*有限* 生成する集合を持つ場合、*有限生成* と呼ばれます。

#### 命題 9 {#alg-ii-s1-prop-9 .statement tag=05KF}

*The submodule generated by a family* $(a_i)_{i \in I}$ *of elements of an* $A$*-module* $E$ *is the set of linear combinations of the family* $(a_i)$.

$E$ のすべての部分加群と $a_i$ のすべての含む、および $a_i$ の含む線形結合。逆に、no. 1 の式 (1) と (2) は、$a_i$ の線形結合の集合が $E$ の部分加群であり、明らかに含むはすべて $a_i$ であり、したがって最小の部分加群であることを証明します。 含む彼ら。

#### 系 1 {#alg-ii-s1-prop-9-cor-1 .statement tag=05KG}

*$u : E \to F$ *を線形写像、S 部分集合 of* $E$ *および* $M$ *部分加群 of* $E$ *$S$によって生成されます。 *その後* $u(M)$ *は $F$ の部分加群です* $u(S)$ によって生成されます。

特に、$E$ の有限生成された部分加群の $u$ の下の像は、$F$ の有限生成された部分加群です。

#### 注意 {#alg-ii-s1-n7-rem-1 .statement tag=05KH}

すべての $x \in S$ に対して $u(x) = 0$ の場合、すべての $x \in M$ に対して $u(x) = 0$ もなります。 ときどきこの結果を *「線形恒等性の拡大の原理」* または *「線形性による拡大の原理」* と呼ぶことにします。

特に、線形写像 $u : E \to F$ が形 $v \circ \phi$ のものであることを検証するには、$v : E / M \to F$ が線形であり、$\phi : E \to E / M$ が正規の射影である場合、$u(S) = 0$ を検証するだけで十分です。

#### 系 2 {#alg-ii-s1-prop-9-cor-2 .statement tag=05KI}

*部分加群は家族の和集合によって生成されます* $(M_i)_{i \in I}$ * 加群の部分加群の $E$ * は和* の集合と同一です* $\sum_{i \in I} x_i$、*ここで* $(x_i)_{i \in I}$ * の集合を通過します元* $E$ *有限台の家族* $x_i \in M_i$ *全員* $i \in I$。

明らかに、$\bigcup_{i \in I} M_i$ の元のすべての線形結合は上記の形に属します。 逆は明らかです。

E のサブモジュールのファミリー $(M_i)_{i \in I}$ の結合によって生成される E のサブモジュールは、ファミリー $(M_i)$ の*合計* と呼ばれ、$\sum_{i \in I} M_i$ で表されます。

すべての $i \in I$、$h_i$ が標準単射 $M_i \to E$ と $\bigoplus_{i \in I} M_i$ の $h : (x_i) \mapsto \sum_i h_i(x_i)$ 線形写像を家族 $(h_i)$ (no. 6、命題 6) に E 対応するにすると、$\sum_{i \in I} M_i$ は次のようになります。 $h$の*像*。他の語には*完全系列*があります

$$
\bigoplus_{i \in I} M_i \xrightarrow{h} E \longrightarrow E / \left( \sum_{i \in I} M_i \right) \longrightarrow 0.
$$

#### 系 3 {#alg-ii-s1-prop-9-cor-3 .statement tag=05KJ}

*もし* $(M_\lambda)_{\lambda \in L}$ * が A-加群 E の部分加群の右向き族である場合、 和* $\sum_{\lambda \in L} M_\lambda$ * は和集合* $\bigcup_{\lambda \in L} M_\lambda$ と同一です。

$\bigcup_{\lambda \in L} M_\lambda \subset \sum_{\lambda \in L} M_\lambda$ *は仮定がなければ常に true です。一方、すべての有限サブファミリー* $(M_\lambda)_{\lambda \in J}$ *of* $(M_\lambda)_{\lambda \in L}$ に対して、*仮定 a* $\mu \in L$ *そのような* $M_\lambda \subset M_\mu$ *すべて* $\lambda \in J$, *したがって* $\sum_{\lambda \in L} M_\lambda \subset M_\mu$ *そして、系 2 から次のことが得られます* $\sum_{\lambda \in L} M_\lambda \subset \bigcup_{\lambda \in L} M_\lambda$。

#### 系 4 {#alg-ii-s1-prop-9-cor-4 .statement tag=05KK}

*$0 \to E \xrightarrow{f} F \xrightarrow{g} G \to 0$ *を A-加群の完全系列、* E の S 生成する系、* G の *T 生成する系とする。 *T' が * $g(T') = T$ となるような F の部分集合である場合、*T' \cup f(S) は生成する系の * F.

T' \cup f(S) 含む $f(E)$ によって生成された F の部分加群 F'、そして $g(F')$ 含む T として、$g(F') = G$;したがって $F' = F$ です。

#### 系 5 {#alg-ii-s1-prop-9-cor-5 .statement tag=05KL}

*完全系列* $0 \to E \to F \to G \to 0$ *A-加群では、E と G が有限に生成される場合、F も有限に生成されます。*

#### 命題 10 {#alg-ii-s1-prop-10 .statement tag=05KM}

*M、N *を A-加群 E の 2 つの部分加群とします。すると、2 つの完全系列* になります。

$$
\begin{align*}
&0 \longrightarrow M \cap N \xrightarrow{u} M \oplus N \xrightarrow{i-j} M + N \longrightarrow 0 \\
&0 \longrightarrow E/(M \cap N) \xrightarrow{v} (E/M) \oplus (E/N) \xrightarrow{p-q} E/(M + N) \longrightarrow 0
\end{align*}
$$

*ここで* $i : M \to M + N$、$j : N \to M + N$ *は標準単射、*
$$
p : E/M \to E/(M + N) \quad \text{and} \quad q : E/N \to E/(M + N)
$$

*標準全射、準同型 u と v は次のように定義されます:*

$f : M \cap N \to M \to M \oplus N$ と $g : M \cap N \to N \to M \oplus N$ が標準単射、$u = f + g$ の場合、および $r : E/(M \cap N) \to E/M \to (E/M) \oplus (E/N)$ の場合、
$$
s : E/(M \cap N) \to E/N \to (E/M) \oplus (E/N)
$$
は標準写像、$v = r + s$です。

(29) の正確性を証明します。明らかに、$i - j$ は全射的であり、$u$ は単射的です。一方、$x \in M$と$y \in N$が$(i - j)(x, y) = 0$であるということは、$i(x) - j(y) = 0$、したがって$i(x) = j(y) = z \in M \cap N$、定義$x = f(z), y = g(z)$によりよってとなり、$\operatorname{Ker}(i - j) = \operatorname{Im} u$が証明されます。

(30) の正確性を証明します。明らかに $p - q$ は全射です。一方、$t \in E/(M \cap N)$ の$v(t) = 0$ は $r(t) = s(t) = 0$ を意味するため、$t$ は類 mod になります。 元 $z \in E$ の $(M \cap N)$ の類 mod。 $M$とmod。 $N$ は零で、これは $z \in M \cap N$ と $t = 0$ を意味します。最後に、$(p - q)(x, y) = 0$ ($x \in E/M, y \in E/N$ は $p(x) = q(y)$ を意味します)、または類 mod を持つ $E$ の 2 つの元 $z', z''$ が存在すると言うこともできます。 $M$とmod。 $N$ はそれぞれ $x$ と $y$ であり、$z' - z'' \in M + N$ となります。したがって、$z' - z'' = t' - t''$、よってのような $t' \in M, t'' \in N$ が存在します。
$$
z' - t' = z'' - t'' = z.
$$
$w$ を類 mod とします。 $z; r(w)$ の $(M \cap N)$ は類 mod です。 $z$の$M$、したがって$z'$のそれも、つまり$x$です。同様に$s(w) = y$、これで$\operatorname{Ker}(p - q) = \operatorname{Im} v$の証明が完成します。

### 8. 直和/部分加群

#### 定義 6 {#alg-ii-s1-def-6 .statement tag=05KN}

*A-加群* $E$ *ある家族の直和であると言われています* $(M_\iota)_{\iota \in I}$ *の部分加群の* $E$ *標準写像* $\bigoplus_{\iota \in I} M_\iota \to E$ *(no. 6)* *は同型* です。

すべての $x \in E$ を形 $x = \sum_{\iota \in I} x_\iota$ で *独自の方法* で書くことができ、すべての $\iota \in I$ を $x_\iota \in E_\iota$ とすると言うのと同じことになります。 元 $x_\iota$ したがって、対応するから $x$ は、$E_\iota$ の $x$ の *成分* と呼ばれます。 写像 $x \mapsto x_\iota$ は *線型* です。

#### 注意 {#alg-ii-s1-n8-rem-1 .statement tag=05KO}

(1) $(M_\iota)_{\iota \in I}, (N_\iota)_{\iota \in I}$ を、同じインデックス集合を持つ加群 $E$ の部分加群の 2 つのファミリーとします。 $E$ は、家族 $(M_\iota)$ と家族 $(N_\iota)$ の *両方* 直和であり、すべての $\iota \in I$ に対する *それ* $N_\iota \subset M_\iota$ であると仮定します。次に、$N_\iota = M_\iota$ *すべて* $\iota \in I$、次のように、no. 6、系 1 から命題 7 が標準単射 $f_\iota : N_\iota \to M_\iota$ に適用されます。

#### 命題 11 {#alg-ii-s1-prop-11 .statement tag=05KP}

*$(M_\iota)_{\iota \in I}$ *A-加群* $E$ の部分加群の家族としましょう。 *次のプロパティは同等です*:

(a) *部分加群* $\sum_{\iota \in I} M_\iota$ *家族の直和* $(M_\iota)_{\iota \in I}$です。

(b) *関係* $\sum_{i \in I} x_i = 0$、*ここで* $x_i \in M_i$ *すべて* $i \in I$、*暗黙* $x_i = 0$ *すべて* $i \in I$。

(c) *すべて* $\kappa \in I$、*共通部分のうち* $M_\kappa$ *および* $\sum_{i \neq \kappa} M_i$ *簡約するから* 0。

関係 $\sum_i x_i = \sum_i y_i$ は $\sum_i (x_i - y_i) = 0$ と等しいので、(a) と (b) が等しいというのは明らかです。一方、定義 6 により、(a) は、$\bigoplus_{i \in I} M_i$ の元を元 $x_i \in M_i$ の直和として表現する一意性によって、(c) を意味します。最後に、関係 $\sum_i x_i = 0$ (すべての $i$ に対して $x_i \in M_i$) は、すべての $\kappa \in I$、$x_\kappa = \sum_{i \neq \kappa} (-x_i)$ に対して書くことができます。 条件 (c) はすべての $\kappa \in I$ に対して $x_\kappa = 0$ を意味するため、(c) は (b) を意味します。

#### 定義 7 {#alg-ii-s1-def-7 .statement tag=05KQ}

A-加群 E の *自己準同型 e は、* $e \circ e = e$ * (他の語では、e が環 End(E) でべき等である場合) の場合、射影子と呼ばれます。 射影子の * $\operatorname{End}(E)$ *ファミリー* $(e_\lambda)_{\lambda \in L}$ は、* $e_\lambda \circ e_\mu = 0$ *for* $\lambda \neq \mu$ であれば直交と呼ばれます。

#### 命題 12 {#alg-ii-s1-prop-12 .statement tag=05KR}

*E を A-加群とします。*

(i) *E が族の直和* 部分加群の $(M_\lambda)_{\lambda \in L}$ で、すべて* $x \in E$ である場合、$e_\lambda(x)$ * は x の成分* $M_\lambda$、$(e_\lambda)$ * は射影子の直交族ですそのような* $x = \sum_{\lambda \in L} e_\lambda(x)$ *すべて* $x \in E$。

(ii) *逆に、* $(e_\lambda)_{\lambda \in L}$ * が * $\operatorname{End}(E)$ の射影子の直交族である場合* $x = \sum_{\lambda \in L} e_\lambda(x)$ *すべて* $x \in E$ について、*E は部分加群* $M_\lambda = e_\lambda(E)$ の族の直和です。

性質 (i) は定義から続き、(ii) は no. 6、系 2 ～ 命題 6 の特殊なケースで、標準単射 $M_\lambda \to E$ および写像 $e_\lambda : E \to M_\lambda$ に適用されます。

L が有限の条件である場合、すべての $x \in E$ に対する $x = \sum_{\lambda \in L} e_\lambda(x)$ も $\operatorname{End}(E)$ に書き込まれる可能性があることに注意してください。

(31)
$$
1_E = \sum_{\lambda \in L} e_\lambda.
$$

#### 系 {#alg-ii-s1-n8-cor-1 .statement tag=05KS}

*E のすべての射影子 e について、E は e の像* $M = e(E)$ * および核* $N = e^{-1}(0)$ * の直和です。すべて* $x = x_1 + x_2 \in E$ *with* $x_1 \in M$ *and* $x_2 \in N$、$x_1 = e(x)$; *1 − e は像 N と核 M* の E の射影子です。

$(1 - e)^2 = 1 - 2e + e^2 = 1 - e$ *in* $\operatorname{End}(E)$ *したがって* $1 - e$ *はプロジェクターです。同様に* $e(1 - e) = (1 - e)e = e - e^2 = 0$、*E はイメージ* $M$ *and* $N$ *e と* $1 - e$ *命題 12 による。 最後に、すべての* $x \in E$、*関係* $x \in M$ *は$x = e(x)$と同等です。 *for* $x = e(x)$ *定義* $x \in M$ を意味します *そして逆に、* $x = e(x')$ *with* $x' \in E$、*then* $e(x) = e^2(x') = e(x') = x;$

したがって、これは M が $1 - e$ の核であることを示し、$e$ と $1 - e$ の役割を交換すると、同様に N が $e$ の核であることがわかります。

#### 注意 {#alg-ii-s1-n8-rem-2 .statement tag=05KT}

(2) E, F を 2 A-加群とし、E が部分加群の有限族 $(M_i)_{1 \leq i \leq m}$ の直和と、部分加群の有限族 $(N_j)_{1 \leq j \leq n}$ の F 直和とする。次に、$\mathrm{Hom}_A(E, F)$ が正規的に積 $\prod_{i,j} \mathrm{Hom}_A(M_i, N_j)$ と識別されることがわかります (no. 6、系 1 から命題 6)。正確には、家族 $(u_{ji})$ に対して、$u_{ji} \in \mathrm{Hom}_A(M_i, N_j)$ 対応する線形写像 $u : E \to F$ は次のように定義されます。 $u$ のそれぞれの $M_i$ とそれぞれの $x_i \in M_i$ に定義する制限を加えるだけで十分です。
$$
u(x_i) = \sum_{j=1}^n u_{ji}(x_i).
$$
ここで、G を部分加群の有限族 $(P_k)_{1 \leq k \leq p}$ の 3 番目の A-加群、直和とします。 $v$ を F から G の線形写像とし、$(v_{kj}) \in \prod_{j,k} \mathrm{Hom}_A(N_j, P_k)$ を標準的にそのファミリー 対応するとします。 $x_i \in M_i$の皆様、
$$
v(u(x_i)) = \sum_{j=1}^n v(u_{ji}(x_i)) = \sum_{k=1}^p \sum_{j=1}^n v_{kj}(u_{ji}(x_i)).
$$
したがって、次のように書くと、
$$
w_{ki} = \sum_{j=1}^n v_{kj} \circ u_{ji} \in \mathrm{Hom}_A(M_i, P_k)
$$
ファミリ $(w_{ki})$ 対応するは、E から G (cf. § 10, no. 5) までの複合線形写像 $w = v \circ u$ に標準的に変換されます。

### 9. 補部分加群

#### 定義 8 {#alg-ii-s1-def-8 .statement tag=05KU}

A-加群 E では、E が $M_1$ と $M_2$ の直和である場合、2 つの部分加群 $M_1, M_2$ が補足的であると言われます。

no. 8 の命題 11 は、$M_1$ と $M_2$ を補足するには、$M_1 + M_2 = E$ と $M_1 \cap M_2 = \{0\}$ (cf. I, § 4, no. 9, 命題 15) が必要かつ十分であることを示しています。

#### 命題 13 {#alg-ii-s1-prop-13 .statement tag=05KV}

$M_1, M_2$をA-加群Eの2つの補部分加群とします。標準写像の制限から$M_1$まで$E \to E/M_2$は$E/M_2$上の$M_1$の同型です。

この線形写像は$M_1 + M_2 = E$から全射であり、その核は$M_1$の共通部分と$E \to E/M_2$の核$M_2$、したがって簡約するから$\{0\}$であるため単射です。

#### 系 {#alg-ii-s1-n9-cor-1 .statement tag=05KW}

$M_2$ と $M_2'$ が E の同じサブモジュール $M_1$ の 2 つの補足である場合、$x - x' \in M_1$ が $M_2'$ への $M_2$ の同型写像のグラフとなる順序ペア $(x, x') \in M_2 \times M_2'$ のセット。

同型 $M_2 \to E/M_1 \to M'_2$ を合成したグラフであるのが明らかです。

#### 定義 9 {#alg-ii-s1-def-9 .statement tag=05KX}

* $A$ モジュール $E$ の部分加群 $M$ は、$E$ に補部分加群がある場合、$E$ の直因子と呼ばれます。

この場合、$E/M$ は $M$ の補充 (命題 13) と同型です。

部分加群は必ずしも補充 (練習問題 11) を認めるとは限りません。 部分加群が直因子である場合、一般にいくつかの異なる補充があります。ただし、これらの補充は 1 つの他の (系から命題 13) と正準的に同型です。

#### 命題 14 {#alg-ii-s1-prop-14 .statement tag=05KY}

*モジュール$E$のサブモジュール$M$が直接要因となるためには、画像が$M$である$E$のプロジェクター、またはカーネルが$M$である$E$のプロジェクターが存在することが必要十分です。

これは、no. 8、命題 12、系の直後に続きます。

#### 命題 15 {#alg-ii-s1-prop-15 .statement tag=05KZ}

*与えられた $A$ モジュールのうち完全系列*
$$
(33)\quad 0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$
*次の命題は同等です:*
(a) *$F$の部分加群$f(E)$は直因子です*。
(b) *$f$ (集合理論、II, § 3, no. 8、定義 11) に関連する線形後退 $r : F \to E$ が存在します。
(c) *$g$ (集合理論, II, § 3, no. 8, 定義 11) に関連付けられた線形切断 $s : G \to F$ が存在します。*
*この場合、$f + s : E \oplus G \to F$は同型になります。*

$e(F) = f(E)$ となる射影器 $e$ が $\mathrm{End}(F)$ に存在する場合、準同型射影 $f^{-1} \circ e : F \to E$ は $f$ に関連付けられた線形後退です。逆に、そのような後退$r$が存在する場合、$f \circ r$は$F$の投影機であり、その画像は$f(E)$であるため、(a)と(b)は等価である(命題14)。 $f(E)$ が $F$ で補充 $E'$ を認め、$j : E' \to F$ が標準単射である場合、$g \circ j$ は $E'$ の $G$ と逆同型の同型であり、写像と見なされます。 $G$ を $F$ に変換すると、$g$ に関連付けられた線形の切断になります。 逆に、そのような切断 $s$ が存在する場合、核が $f(E)$ である$F$ の$s \circ g$ は射影子であるため、(a) と (c) は等価です (命題 14)。 さらに、$s$は$s(G)$上の$G$の全単射であり、$s(G)$は$f(E)$の補足であるため、$f + s$は同型になります。

$r$ (それぞれ $s$) が与えられることは、$F$ の $f(E)$ の補充、つまり $r$ の核 (それぞれ $s$ の像) が与えられることと同等であることに注意してください。

完全系列(33)が命題15の条件を満たすとき、分裂*、または$(F, f, g)$は$E$(I, § 6, no. 1)によって$G$の*自明*拡大と言われます。

#### 系 1 {#alg-ii-s1-prop-15-cor-1 .statement tag=05L0}

$u : E \to F$を線形写像とします。 $u \circ v = 1_F$ のような線形写像 $v : F \to E$ が存在するには ($u$ が右反転であると言われ、$v$ が $u$ の右逆であると言われる場合)、$u$ が全射的であり、そのカーネルが $E$ の直接因子であることが必要かつ十分です。 $E$ の部分加群 $\operatorname{Im}(v)$ は、$\operatorname{Ker}(u)$ の補充になります。

$u$ が全射的であることが明らかに必要です。 $v$ は切断と $u$ に関連付けられるため、結論は命題 15 から得られます。

#### 系 2 {#alg-ii-s1-prop-15-cor-2 .statement tag=05L1}

$u : E \to F$を線形写像とします。 $v \circ u = 1_E$ のような線形写像 $v : F \to E$ が存在するには ($u$ が左反転であると言われ、$v$ が $u$ の左反転であると言われる場合)、$u$ が単射であり、その像が次であることが必要かつ十分です。 $F$の直因子。 $F$ の部分加群 $\operatorname{Ker}(v)$ は、$\operatorname{Im}(u)$ の補充になります。

$u$ が単射であることが明らかに必要です。 $v$ は $u$ に関連付けられた撤回であるため、命題 15 からも結論が導き出されます。

#### 注意 {#alg-ii-s1-n9-rem-1 .statement tag=05L2}

(1) Let $M, N$ be two supplementary submodules in an $A$-module $E$, $p, q$ the projectors of $E$ onto $M$ and $N$ respectively, corresponding to the decomposition of $E$ as a direct sum of $M$ and $N$. すべての $A$ モジュール $F$ について、写像 $(u, v) \mapsto u \circ p + v \circ q$ は次の同型であることが知られています (no. 6、命題 6 の系 1)。
$$
\operatorname{Hom}_A(M, F) \oplus \operatorname{Hom}_A(N, F)
$$
$\operatorname{Hom}_A(E, F)$へ。 この同型の下にある $\operatorname{Hom}_A(M, F)$ の像は、線形写像 $w : E \to F$ の集合であり、すべての $x \in N$ に対して $w(x) = 0$ になります。

(2) If $M, N$ are two submodules of $E$ such that $M \cap N$ is a direct factor of $M$ and $N$, then $M \cap N$ is also a direct factor of $M + N$: if $P$ (resp. $Q$) is a supplement of $M \cap N$ in $M$ (resp. $N$), $M + N$ is the direct sum of $M \cap N, P$ and $Q$, as is immediately verified.

### 10. 有限長中加群

(I, § 4, no. 4, 定義 7) を思い出してください。$A$ モジュール $M$ が 0 に還元されず、$M$ や $\{0\}$ と区別される場合、含む部分加群は単純と呼ばれます。 $A$ モジュール $M$ は、この系列の商の Jordan-Hölder 系列 $(M_i)_{0 \leq i \leq n}$ と数 $n$ があれば、有限長であると言われます (これは、Jordan-Hölder に依存しません) $M$ の系列は考慮されます) は、$M$ の長さ (I, § 4, no. 7、定義 11) と呼ばれます。それを$\operatorname{long}(M)$ または $\operatorname{long}_A(M)$ で表します。 0 に削減された $A$ モジュールは長さ 0 になります。 $M$ が有限長の非ゼロ $A$ 加群の場合、$\operatorname{long}(M) > 0$。

#### 命題 16 {#alg-ii-s1-prop-16 .statement tag=05L3}

$M$ を $A$ モジュール、$N$ 部分加群を $M$ とします。 $M$ が有限長であるためには、$N$ と $M/N$ がそうであることが必要かつ十分であり、その場合、
$$
\operatorname{long}(N) + \operatorname{long}(M/N) = \operatorname{long}(M).
$$
証明はI, § 4, no. 7、命題10で与えられました。

#### 系 1 {#alg-ii-s1-prop-16-cor-1 .statement tag=05L4}

$M$ を有限長の $A$ 加群とする。 $M$ のサブモジュール $N$ が $M$ に等しいためには、$\operatorname{long}(N) = \operatorname{long}(M)$ であることが必要かつ十分です。

#### 系 2 {#alg-ii-s1-prop-16-cor-2 .statement tag=05L5}

$u : M \to N$ を $A$ モジュール準同型とします。 $M$ または $N$ が有限長の場合、$\operatorname{Im}(u)$ も同様です。 $M$ が有限長の場合、$\operatorname{Ker}(u)$ も同様であり、
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Ker}(u)) = \operatorname{long}(M).
$$
$N$ が有限長の場合、$\operatorname{Coker}(u)$ も同様であり、
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Coker}(u)) = \operatorname{long}(N).
$$

#### 系 3 {#alg-ii-s1-prop-16-cor-3 .statement tag=05L6}

$(M_i)_{0 \leq i \leq n}$ を有限長の $A$ 加群の有限族とする。 線形写像の完全系列が存在する場合
$$
0 \longrightarrow M_0 \xrightarrow{u_0} M_1 \xrightarrow{u_1} M_2 \longrightarrow \cdots \longrightarrow M_{n-1} \xrightarrow{u_{n-1}} M_n \longrightarrow 0
$$
それから
$$
\sum_{k=0}^n (-1)^k \operatorname{long}(M_k) = 0.
$$
系は $n = 1$ にとっては明らかですが、$n = 2$ にとっては単なる命題 16 です。私たちは$n$の帰納法までに議論します。 $M'_{n-1} = \operatorname{Im}(u_{n-2})$ の場合、帰納法の仮定までに、
$$
\sum_{k=0}^{n-2} (-1)^k \operatorname{long}(M_k) + (-1)^{n-1} \operatorname{long}(M'_{n-1}) = 0.
$$
一方、完全系列 $0 \to M'_{n-1} \to M_{n-1} \to M_n \to 0$ は次のようになります。
$$
\operatorname{long}(M'_{n-1}) + \operatorname{long}(M_n) = \operatorname{long}(M_{n-1}),
$$
よって関係 (38)。

#### 系 4 {#alg-ii-s1-prop-16-cor-4 .statement tag=05L7}

$M$ と $N$ を、$A$ モジュール $E$ の有限長の 2 つの部分加群とします。その場合、$M + N$ は有限長のものであり、
$$
\operatorname{long}(M + N) + \operatorname{long}(M \cap N) = \operatorname{long}(M) + \operatorname{long}(N).
$$
系を適用する 3 ～ 完全系列 (29) (no. 7) で十分です。
$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$
(34) によって $\operatorname{long}(M \oplus N) = \operatorname{long}(M) + \operatorname{long}(N)$ という事実を使用します。

#### 系 5 {#alg-ii-s1-prop-16-cor-5 .statement tag=05L8}

$M$ を、有限長の部分加群のファミリー $(N_i)$ の $A$ モジュール和とします。すると、$M$ は有限長のものとなり、
$$
\operatorname{long}(M) \leq \sum_i \operatorname{long}(N_i).
$$

さらに、(40) の 2 つの辺が等しいためには、M が $N_i$ の直和であることが必要かつ十分です。

標準的な全射法線形写像 $h : \bigoplus_i N_i \to M$ が存在することがわかっています (no. 7, 公式 (28))。したがって、(35) から系が得られます。

#### 系 6 {#alg-ii-s1-prop-16-cor-6 .statement tag=05L9}

*M と N を 2 つの部分加群の A-加群 E とし、E/M と E/N が有限長の加群となるようにします。この場合、E/(M \cap N) は有限長であり、*

$$
\text{(41)} \quad \text{long}(E/(M \cap N)) + \text{long}(E/(M + N)) = \text{long}(E/M) + \text{long}(E/N).
$$

系を適用する 3 ～ 完全系列 (30) で十分です

$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$

という事実を利用して

$$
\text{long}((E/M) \oplus (E/N)) = \text{long}(E/M) + \text{long}(E/N).
$$

#### 系 7 {#alg-ii-s1-prop-16-cor-7 .statement tag=05LA}

*$(M_i)$をA-加群Eの部分加群の有限族とし、$E/M_i$が有限長の加群となるようにします。次に、$E/(\bigcap_i M_i)$ は有限長であり、*

$$
\text{(42)} \quad \text{long}\left(E/(\bigcap_i M_i)\right) \leq \sum_i \text{long}(E/M_i).
$$

標準的な単射詞線形写像 $E/(\bigcap_i M_i) \to \bigoplus_i (E/M_i)$ が存在することが確認されています (公式 (27))。

#### 注意 {#alg-ii-s1-n10-rem-1 .statement tag=05LB}

no. 7、命題 9 を除き、*すべて* nos. 2 ～ 10 は、演算子* を使用した任意の *可換群に対して有効です。部分加群 (それぞれ商加群) は、主張で安定した部分群 (それぞれ剰余群は安定した部分群) に置き換えられます。また、群の準同型を演算子 "線形写像" で呼び出すという規則も作ります。 no. 7、命題 9 の系は、演算子を使用した可換群にも有効です。これは系 4 と 5 については明らかです。また、系 2 についても明らかです。なぜなら、すべての演算子 $\alpha$ に対して $\alpha \left( \sum_{i \in I} x_i \right) = \sum_{i \in I} \alpha x_i$ があり、そこから系 3 が続くからです。 系 1 については、N が F 含む $u(S)$ の安定した部分群である場合、$u^{-1}(N)$ は E 含む S の安定した部分群であるため、$u^{-1}(N)$ であることに注意するだけで十分です。 含む M なので $u(M) \subset N$ です。

### 11. 自由な家族。 基底

A を環、T を集合として、A-加群 $A_s^{(T)}$ を考えます。 定義によって、それはA-加群の家族$(M_t)_{t \in T}$の外部直和であり、すべて$A_s$に等しく、すべての$t \in T$に対して、標準単射$j_t : A_s \to A_s^{(T)}$(no. 6)が存在します。 j_t(1) = e_t となるように、$e_t = (\delta_{tt'})_{t' \in T}$ と書きます。ここで、$\delta_{tt'}$ は、$t' \neq t$ の場合は 0、$t' = t$ の場合は 1 になります (「クロネッカー記号」; $(t, t') \mapsto \delta_{tt'}$ は、$T \times T$ の対角線の特性写像にすぎません)。すべての $x = (\xi_t)_{t \in T} \in A_s^{(T)}$ は一意に記述できます。
$$
x = \sum_{t \in T} \xi_t e_t.
$$
写像 $\phi : t \mapsto e_t$ から $T$ を $A_s^{(T)}$ に変換したものを標準と呼びます。 $A$ がゼロ以外の場合は単射です。順序付けられた対 $(A_s^{(T)}, \phi)$ は、ユニバーサル写像問題 (集合理論, IV, § 3, no. 1) の解であることがわかります。

#### 命題 17 {#alg-ii-s1-prop-17 .statement tag=05LC}

*すべての A-加群 E とすべての写像 $f : T \to E$ に対して、$f = g \circ \phi$ となる A-線型写像 $g : A_s^{(T)} \to E$ が 1 つだけ存在します。*

条件 $f = g \circ \phi$ は、すべての $t \in T$ の $g(e_t) = f(t)$ を意味し、これはすべての $\xi \in A$ とすべての $t \in T$ の $g(\xi e_t) = \xi f(t)$ に相当し、また、$g \circ j_t$ が線形写像 $\xi \mapsto \xi f(t)$ であることも意味します。 $A_s$ をすべての $t \in T$ に対して $E$ にします。したがって、命題は、no. 6、命題 6 の特殊なケースです。

線形写像 $g$ は、元の $E$ の家族 $(f(t))_{t \in T}$ によって *決定された* と言われています。 定義により
$$
g\left( \sum_{t \in T} \xi_t e_t \right) = \sum_{t \in T} \xi_t f(t).
$$

$g$ の核 $R$ は $(\xi_t) \in A_s^{(T)}$ の集合であり、$\sum_t \xi_t f(t) = 0$ になります。 加群 $R$ は、家族の元の間* $(f(t))_{t \in T}$ の間の線形関係の * 加群であると言われているときどきです。 完全系列
$$
0 \longrightarrow R \longrightarrow A_s^{(T)} \overset{g}{\longrightarrow} E
$$
家族$(f(t))_{t \in T}$によって*決定*されると言われています。

#### 系 1 {#alg-ii-s1-prop-17-cor-1 .statement tag=05LD}

*$T, T'$ を 2 つの集合、$g : T \to T'$ 写像とします。すると、図式* を可換にする A-線型写像 $f : A^{(T)} \to A^{(T')}$ が 1 つだけ存在します。
$$
\begin{array}{ccc}
T & \overset{g}{\longrightarrow} & T' \\
\downarrow \phi & & \downarrow \phi' \\
A^{(T)} & \overset{f}{\longrightarrow} & A^{(T')}
\end{array}
$$
*ここで、$\phi$と$\phi'$は標準写像です。*

写像 $T \overset{g}{\to} T' \overset{\phi'}{\to} A^{(T')}$ を命題を適用する 17 にすれば十分です。

#### 系 2 {#alg-ii-s1-prop-17-cor-2 .statement tag=05LE}

* A-加群 E の元の族 $(a_t)_{t \in T}$ が E の生成する系であるためには、この族によって決定される線形写像 $A_s^{(T)} \to E$ が全射であることが必要かつ十分です。

これは、no. 7 の命題 9 を他の表現する方法にすぎません。

#### 定義 10 {#alg-ii-s1-def-10 .statement tag=05LF}

*ファミリー* $(a_t)_{t \in T}$ *$\mathbf{A}$*モジュールの元 $E$ *自由ファミリーと呼ばれます* (それぞれ* $E$の*基底) *線形写像* $A_s^{(T)} \to E$ *このファミリーによって決定されるものが単射である場合* (それぞれ*客観的*)。 *加群は、基底*がある場合、フリーと呼ばれます。

特に、$G$ (加法的に書かれた) が *free* $\mathbf{Z}$*-module* (cf. I, § 7, no. 7) である場合、可換群 $G$ は *free* と呼ばれます。

定義 10 は、系 2 ～ 命題 17 と合わせて、$\mathbf{A}$ モジュール $E$ の基底が $E$ の *自由な生成するファミリ* であることを示します。したがって、$E$の元の各自由家族は、部分加群の基底、つまり生成するになります。

定義までに、$\mathbf{A}$ モジュール $A_s^{(T)}$ は無料になり、ファミリー $(e_t)_{t \in T}$ はこの $\mathbf{A}$ モジュールの基底 (*正規* と呼ばれます) になります。 $\mathbf{A} \neq \{0\}$、$T$ は、正規の全単射 $t \mapsto e_t$ によって、$e_t$ の集合と識別されることがよくあります。これは、$A_s^{(T)}$ の元を $\sum_{t \in T} \xi_t a_t$ ではなく $\sum_{t \in T} \xi_t \cdot t$ と書くことになります。この規則が採用されると、$A_s^{(T)}$ の元は *正式な線形結合* ($\mathbf{A}$ に係数) が * $T$ の元と呼ばれます。

定義 10 と命題 17 は、すぐに次の結果を返します。

#### 系 3 {#alg-ii-s1-def-10-cor-3 .statement tag=05LG}

*$E$ *無料* $\mathbf{A}$* モジュール*、$(a_t)_{t \in T}$ *基底 of* $E$、$F$ *an* $\mathbf{A}$* モジュール、および* $(b_t)_{t \in T}$ *元 of* $F$ のファミリーとします。 *唯一の線形写像* $f : E \to F$ *そのような* が存在します
$$
f(a_t) = b_t \quad \text{for all } t \in T.
$$
*$f$ *単射的*であること* (*全射的*)、*$(b_t)$ *$F$において自由な家族であること*が必要かつ十分です* (*$F$の*生成する系)。

家族 $(a_t)_{t \in T}$ が自由ではない場合、それは *関連* と呼ばれます。 定義 10 は次のように表すこともできます。家族 $(a_t)_{t \in T}$ が *自由* であると言うのは、関係 $\sum_{t \in T} \lambda_t a_t = 0$ (家族 $(\lambda_t)$ は有限台である) は、すべての $t \in T$ に対して $\lambda_t = 0$ を意味します。 $(a_t)_{t \in T}$ が $E$ の *基底* であるということは、すべての $x \in E$ が形 $x = \sum_{t \in T} \xi_t a_t$ で 1 つの方法でのみ記述できることを意味します。すべての $t \in T$ について、$\xi_t$ は、*$x$ *の添字* $t$ *基底* $(a_t)$ に関して *成分* (または *座標*) と呼ばれます。 $E$ から $A_s$ までの写像 $x \to \xi_t$ は *直線* です。

$\mathbf{A} \neq \{0\}$; と仮定します。次に、$\mathbf{A}$-モジュール $E$ では、インデックスが異なる自由ファミリ $(a_t)_{t \in T}$ の 2 つの要素は、それ自体 *別個* です。つまり、$t' \neq t''$ に対して $a_{t'} = a_{t''}$ の場合、次の要素に対して $\lambda_{t'} = 1$、$\lambda_{t''} = -1$、および $\lambda_t = 0$ を持つ $\sum_{t \in T} \lambda_t a_t = 0$ になります。 $T$ は、$t'$ および $t''$ とは異なります。 $S$ の恒等写像によって定義されたファミリが自由である場合 (それぞれ $E$ の基底)、$E$ の部分集合 $S$ は *自由部分集合* (それぞれ $E$ の *基底*) と呼ばれます。 $S$ への索引付け集合の全単射語写像によって定義されるすべてのファミリーは、自由になります (それぞれ基底)。 $E$ の自由な部分集合の元は *一次独立* とも呼ばれます。

E の部分集合が自由でない場合、それは関連している、または関連している系とその元は線形依存していると言われます。

無料の部分集合のすべての部分集合は無料です。特に、空の部分集合は自由であり、E の部分加群 {0} の基底です。

#### 命題 18 {#alg-ii-s1-prop-18 .statement tag=05LH}

*加群 E の族 $(a_t)_{t \in T}$ が自由であるためには、$(a_t)_{t \in T}$ のすべての有限サブファミリーが自由であることが必要かつ十分です。

これは定義の直後に続きます。

命題 18 は、包含順に並べた E の自由部分集合の集合が帰納的であることを示します (*集合理論*、III, § 2, no. 4)。空ではないので ($\varnothing$ 属するから)、Zorn の補題による極大元 $(a_l)_{l \in I}$ があります。 ($A \neq \{0\}$の場合) すべての $x \in E$ に対して、A の元 $\mu \neq 0$ と、$\mu x = \sum_l \xi_l a_l$ (cf. § 7, no. 1) となる元 A の家族 $(\xi_l)$ が存在することになります。

#### 命題 19 {#alg-ii-s1-prop-19 .statement tag=05LI}

*E を部分加群の家族 $(M_\lambda)_{\lambda \in L}$ のA-加群、直和とします。それぞれの $\lambda \in L$、$S_\lambda$ が $M_\lambda$ のフリーの部分集合 (それぞれ生成する集合、基底) である場合、$S = \bigcup_{\lambda \in L} S_\lambda$ はフリーの部分集合 (それぞれ生成する) です。 集合、基底) の E.*

命題は、定義と関係 $A_s^{(S)} = \bigoplus_{\lambda \in L} A_s^{(S_\lambda)}$ から続きます (直和、cf. no. 6 の結合性)。

#### 注意 {#alg-ii-s1-n11-rem-1 .statement tag=05LJ}

(1) 定義 10 までに、$A \neq \{0\}$ と $(a_l)_{l \in I}$ が自由な家族である場合、元 $a_\kappa$ は添字 $l \neq \kappa$ の $a_l$ の線形結合と等しくなりません。しかし逆に、$(a_l)$ 満たすこの条件という家族は必ずしも自由な家族ではありません。たとえば、A を整域と $a, b$ の 2 つの異なる非ゼロ元とします。 A では、$(-b)a + ab = 0$ 以降、A-加群、$a$、$b$ 形が関連する系と見なされます。しかし一般に、$b = xa$の$a = xb$のような元 $x \in A$は存在しません（cf.、ただし§ 7, no. 1、*注意*）。

$\{x\}$ がフリーの部分集合である場合、つまり関係 $\alpha x = 0$ が $\alpha = 0$ を暗示する場合、加群 E の元 $x$ は *free* と呼ばれます。フリー 部分集合のすべての元はフリーであり、特に 0 できない属するから $A \neq \{0\}$ の場合はフリー 部分集合までです。

#### 注意 {#alg-ii-s1-n11-rem-2 .statement tag=05LK}

(2) 自由加群は、自由ではない元 $\neq 0$ を持つことができます。たとえば、A-加群 $A_s$ は自由ですが、A の零の右側因子は、$A_s$ の元として自由ではありません。

(3) $\mathbf{Z}$モジュールとみなされる加法群 $\mathbf{Z}/(n)$ ($n$ 整数 $\geq 2$) では、空いている元はなく、*なおさら* $\mathbf{Z}/(n)$ は自由加群ではありません。

(4) 加群が空いていなくても、A-加群のすべての元 $\neq 0$ が空いていることが起こります。たとえば、有理数数の体 $\mathbf{Q}$ は、この性質を持つ $\mathbf{Z}$ 加群であり、$\mathbf{Q}$ の 2 つの元 $\neq 0$ は常に形の関連する系と基底です。したがって、$\mathbf{Q}$ は単一の元 $a$ に対して含むしかできません。ただし、$\mathbf{Q}$ の元は、$n \in \mathbf{Z}$ (cf. VII, § 3) を含む形 $na$ のすべてではありません。

#### 命題 20 {#alg-ii-s1-prop-20 .statement tag=05LL}

*すべての A-加群 E は自由A-加群の商加群と同型です。*

T が E の生成する集合である場合、全射法線形写像 $A_s^{(T)} \to E$ (系 2 ～ 命題 17) が存在し、R がこの写像の核である場合、E は $A_s^{(T)}/R$ と同型です。

特に、$T = E$ を取ることができます。次に、*canonical* と呼ばれる全射法線形写像 $A_s^{(E)} \to E$ があります。

特に、A-加群 E が *有限生成* (no. 7) であるということは、それが自由A-加群の商と *有限基底* と同型であるか、または形の完全系列が存在することを意味します。

$$
A_s^n \to E \to 0 \quad (n \text{ an integer } > 0).
$$

*有限生成* 自由加群 E の基底ごとに $A \neq \{0\}$ が必ず *有限* である場合、S が E の有限生成系と B 基底である場合、S の各元は有限数の線形結合であることに注意してください。 B の元があり、B' が B のすべての元の集合である場合、これは S の元の式で示され、B' は有限であり、すべての $x \in E$ は B' の元の線形結合であるため、$B' = B$ になります。

#### 命題 21 {#alg-ii-s1-prop-21 .statement tag=05LM}

*A-加群* の完全系列ごと

$$
0 \longrightarrow G \xrightarrow{g} E \xrightarrow{f} F \longrightarrow 0
$$

*ここで、F は自由A-加群、分裂* (no. 9) です。 *正確に言うと、* $(b_\lambda)_{\lambda \in L}$ * が F の基底で、それぞれ* $\lambda \in L$、$a_\lambda$ * が E の元である場合、* $f(a_\lambda) = b_\lambda$、*家族* $(a_\lambda)_{\lambda \in L}$ * は自由で、生成する補部分加群は g(G)* になります。

すべての $\lambda \in L$ (系 3 ～ 命題 17) に対して $h(b_\lambda) = a_\lambda$ となるような線形写像 $h : F \to E$ が 1 つだけ存在します。 h は f に関連付けられた線形切断であるため、I, § 4, no. 9、命題 15 から命題が続きます。

#### 注意 {#alg-ii-s1-n11-rem-3 .statement tag=05LN}

(5) $(a_i)_{1 \leq i \leq n}$ を A-加群 E の *基底* とし、$(b_i)_{1 \leq i \leq n}$ を関係で与えられる E の元の族とする

$$
b_i = \lambda_{1i} a_1 + \cdots + \lambda_{ii} a_i \quad (1 \leq i \leq n)
$$

ここで、$\lambda_{ii}$ は A で *反転可能*です。その場合、$(b_i)_{1 \leq i \leq n}$ は E の *基底* です。$n$ については帰納法によって議論するだけで十分で、命題は $n = 1$ にとって明らかです。 E' が家族 $(a_i)_{1 \leq i \leq n-1}$ によって生成された E の部分加群である場合、帰納法の仮定から $(b_i)_{1 \leq i \leq n-1}$ は E' の基底であることがわかります。一方、(46) から、$\mu b_n \in E'$ と $\mu \in A$ の場合、$\lambda_{nn}$ は可逆であるため、$\mu \lambda_{nn} a_n \in E'$、よって $\mu = 0$ も成り立ちます。家族$(b_i)_{1 \leq i \leq n}$はこうして自由になり、
$$
a_n = -\lambda_{nn}^{-1}\lambda_{1n}a_1 - \cdots - \lambda_{nn}^{-1}\lambda_{n-1,n}a_{n-1} + \lambda_{nn}^{-1}b_n
$$
$(b_i)_{1 \leq i \leq n}$ は E の生成する系であることがわかり、証明が完成します。この結果は、インデックス付け集合 I が適切に順序付けられているファミリー $(a_i)_{i \in I}$ に簡単に一般化できます。

### 12. 消滅子。忠実加群。単一種加群

#### 定義 11 {#alg-ii-s1-def-11 .statement tag=05LO}

* A-加群 E の部分集合の消滅子は、元の $\alpha \in A$ の集合であり、すべての $x \in S$ に対して $\alpha x = 0$ となります。*

S の消滅子は通常、Ann(S) で表されます。単一の元 x の部分集合 S からなるの場合、Ann(\{x\}) の代わりに Ann(x) と書き、x* の Ann(x) *消滅子を呼び出します。

関係 $\alpha x = 0$ は、*x が $\alpha$* によって消滅することをというによって表現することもできます。

E の任意の部分集合 S の消滅子が A の *左イデアル* であるのは明らかです。それが A に等しいためには、((M_IV) により) $S = \{0\}$ であることが必要かつ十分です。 E の 2 つの部分集合 S、T が、S の消滅子に T の $S \subset T$、消滅子が含まれる場合、$(S_i)_{i \in I}$ が E の部分集合、和集合の消滅子の任意の族である場合$\bigcup_i S_i$は$S_i$の消滅子の共通部分です。特に、E の部分集合 S の消滅子は、S の元の消滅子の共通部分です。E の元が *free* であると言うのは、その消滅子が であるというというと同等です。 $\{0\}$。すべての $x \in E$ とすべての $\alpha \in A$ について、$\alpha x$ の消滅子は $\beta \in A$ の集合であり、$\beta \alpha \in \mathrm{Ann}(x)$ となります。

*部分加群* M の E の消滅子は、A の *両面理想* です。すべての $x \in M$ に対して $\alpha x = 0$ の場合、すべての $x \in M$ とすべての $\beta \in A$ に対しても $\alpha (\beta x) = 0$ となるため、すべての $\beta \in A$ に対して M の $\alpha \beta$ 属するから消滅子となります。特に E の消滅子は A の両面イデアルです。

すべての $\alpha \in A$ について、$h_\alpha$ をホモテティー $x \mapsto \alpha x$ とします。 A の写像 $\alpha \mapsto h_\alpha$ を可換群 (演算子なし) E の自己準同型環 $\mathscr{E} = \mathrm{Hom}_\mathbf{Z}(E, E)$ にすると、*環準同型* (§ 2, no. 5) になることが知られています。この準同型の下にある 0 の逆像は E の *消滅子* $a$ です。したがって、準同型 $\alpha \mapsto h_\alpha$ の下の A の像は、商環 $A/a$ と同型です。 加群 E は、消滅子 $a$ 簡約するが 0 の場合、*忠実* と呼ばれます。

E を Ann(E) に含まれる A の両側イデアル A-加群、$a$ とし、$\dot{\alpha}$ を商環 $A/a$ の元とします。すべての $x \in E$、元 $\alpha x$ は、$\alpha \in A$ 所属から類 $\dot{\alpha}$ のすべての mod で同じです。 $a$;この元を $\dot{\alpha} x$ で表すと、写像 (α, x) ↦ αx 定義する (E に加法がある) E 上の (A/α) 加群構造であることがすぐにわかります。 α = Ann(E) のとき、このように定義された (A/α) 加群 E は次のようになります。 *忠実*;それは、A-加群 E に *関連付けられている*信者加群であると言います。 A-加群 E のすべての部分加群は、関連付けられた信者加群の部分加群でもあり、またその逆であることに注目してください。

#### 定義 12 {#alg-ii-s1-def-12 .statement tag=05LP}

*加群は、単一の元によって生成される場合、単一と呼ばれます。*

命題 9 of no. 7 は、E が単種 A-加群で、a が元生成する E である場合、E は ξa の集合 A.a と同一であり、ξ は A を通過することを示しています。

#### 例 {#alg-ii-s1-n12-exa-1 .statement tag=05LQ}

(1) すべての単次群は、可換 (I, § 4, no. 10、命題 18) であるため、単次 $\mathbf{Z}$ 加群です。
(2) A が可換環である場合、A-加群 A の単一属部分加群は、環 A の*主イデアル* (I, § 8, no. 6) にすぎません。
(3) E の元 ≠ 0 によって生成される E の部分加群は必ず E に等しいため、すべての*単純* A-加群 E は単次です。

#### 命題 22 {#alg-ii-s1-prop-22 .statement tag=05LR}

※Aを環とします。 $A_s$ のすべての商加群は単一です。逆に、E を単一の A-加群、E の c 生成元、および a の消滅子とする。 線形写像 $\xi \mapsto \xi c$ 定義する、移行から商のとき、$A_s/a$ の同型が E.* に

$A_s$ はそれ自体単次であり、1 によって生成されるため、最初の主張は no. 7、系 1 から命題 9 に続きます。 $\xi \mapsto \xi c$ は仮定全射であり、核 a があるため、2 番目は明らかです。

A が可換でない場合、2 つの別個の生成元 c の消滅子、単種 A-加群 E の c' は一般に *別個* であり、加群 E の消滅子とも別個であることに注意してください。一方、A が *可換* である場合、E の生成元 c の消滅子が含まれます。 E のすべての元の消滅子にあるため、E 全体の消滅子になります。

#### 系 {#alg-ii-s1-n12-cor-1 .statement tag=05LS}

*単次 A-加群 E のすべての部分加群は商加群 b/a と同型です。ここで、a と b は、a ⊂ b となる A の 2 つの左イデアルです。単一種 A-加群のすべての商加群は単一種です。*

2 番目の主張は明らかで、最初の命題 22 と I, § 4, no. 6、定理 4 が続きます。

一方、注意は、単種加群の部分加群は必ずしも単種であるわけではありません。 たとえば、A が非主イデアル (VII, § 1, no. 1) が存在する可換環である場合、これらのイデアルは単次 A 加群 A の非単次副加群になります。

定義から、E の元の家族 $(a_i)$ によって生成された A-加群 E の部分加群は、単一種部分加群の *和* であることがわかります。

EのAa_i; (a_i) が E の基底であるためには、各 a_i が E の自由な元であり、Aa_i の和が直接であることが必要かつ十分です。

#### 命題 23 {#alg-ii-s1-prop-23 .statement tag=05LT}

E を非ゼロ部分加群の無限族 (M_i)_{i \in I} の A-加群、直和とします。 E の生成する系 S ごとに、Card(S) \geq Card(I)。

S のすべての x について、M_i の x の成分が \neq 0 となるように、C_x を添字 i \in I の有限集合とし、C = \bigcup_{x \in S} C_x とします。 S 属するのすべての x \in C と仮定に対する M_i の E 直和の定義から部分加群まで、S 生成する E は、C = I を意味します。 I は仮定までで無限であるため、S (集合理論, III, § 5, no. 1, 系 1 ～ 命題 1) も同様です。したがって、Card(I) = Card(C) \leq Card(S) (集合理論, III, § 6, no. 3, 系 3 ～ 定理 2)。

#### 系 1 {#alg-ii-s1-prop-23-cor-1 .statement tag=05LU}

命題 23 の仮説の下で、各 M_i は単次であり、E は非ゼロ単次部分加群の 2 番目の族 (N_\lambda)_{\lambda \in L} の直和であると仮定します。すると、カード(L) = カード(I)となります。

b_\lambda が N_\lambda の生成元である場合、b_\lambda の集合は E の生成する系であるため、Card(L) \geq Card(I) となります。特にLは無限であり、(M_i)と(N_\lambda)の役割を交換すると、同様にCard(I)\geq Card(L)、よって系となります。

#### 系 2 {#alg-ii-s1-prop-23-cor-2 .statement tag=05LV}

加群 E が無限の基底 B を認める場合、E のすべての生成する系は基数 \geq Card(B) を持ち、E のすべての基底は B と等価になります。

### 13. スカラーの環の変更

A、B を 2 つの環と環 B の \rho 準同型から環 A にします。すべての A-加群 E に対して、外部法則 (\beta, x) \mapsto \rho(\beta)x 定義する (加法と) B-加群構造は \rho と E の A-加群構造に関連付けられていると言われています。この B-加群は \rho_*(E) または E_{[B]} (混乱が生じなければ単に E でも) で表されます。特に、B が A の部分環で、 \rho : B \to A が標準単射の場合、E_{[B]} はスカラー A の環を B に制限することによって得られる B-加群と呼ばれます。言葉の乱用により、この表現は準同型 \rho が任意の場合にも使用されます。

F が A-加群 E の部分加群である場合、\rho_*(F) は \rho_*(E) の部分加群であり、\rho_*(E/F) は \rho_*(E)/\rho_*(F) に等しくなります。

E、F を 2 A-加群とします。すべての A-線型写像 u : E \to F は B-線型写像 E_{[B]} \to F_{[B]} でもあり、\rho_*(u) で表されます。他の語には、\mathbf{Z} モジュールの標準単射があります

(47)
$$
\operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{[B]}, F_{[B]}).
$$

この写像は必ずしも全単射ではありません。他の語 B-線型写像 E_{[B]} \to F_{[B]} は必ずしも A 線形であるとは限りません。たとえば、E_{[B]} のサブ B モジュールは必ずしも E のサブ A モジュールであるとは限りません。A が体で、B が $A$ の部分体である場合、ベクトル部分空間 $B_s$ ベクトル $B$-space $(A_s)_{[B]}$ $B \neq A$ の場合、ベクトルサブ$A$ スペースではありません。

$A$ モジュールのすべてのファミリー $(E_i)_{i \in I}$ について、$B$ モジュール $\rho_*\left(\prod_{i \in I} E_i\right)$ (それぞれ $\rho_*\left(\bigoplus_{i \in I} E_i\right)$) が $\prod_{i \in I} \rho_*(E_i)$ (それぞれ $\bigoplus_{i \in I} \rho_*(E_i)$) に等しいことは、明らかです。

$\rho_*(E)$ のすべての生成する系は、$E$ の生成する系ですが、逆は必ずしも真ではありません。

#### 命題 24 {#alg-ii-s1-prop-24 .statement tag=05LW}

*$A, B$ を 2 つの環と $\rho : B \to A$ 環準同型とします。*

(i) *$\rho$ が全単射の場合、標準写像 (47) は全単射です。すべての $A$ モジュール $E$ について、$\rho_*(E)$ のすべてのサブ $B$ モジュールは $E$ のサブ $A$ モジュールです。 $E$ のすべての生成する系は、$\rho_*(E)$ の生成する系です。*

(ii) *$\rho$ が単射の場合、$A$ モジュール $E$ 内のすべての自由ファミリーは、$B$ モジュール $\rho_*(E)$ の自由ファミリーになります。*

命題は定義の直後に続きます。

たとえ$\rho$が単射的であっても、$\rho_*(E)$の自由な家族は必ずしも$E$でも自由であるとは限らないことに注意してください。

*例えば、1と$\sqrt{2}$は、ベクトル$\mathbf{R}$空間として考えた$\mathbf{R}$では自由系を形成しませんが、ベクトル$\mathbf{Q}$空間として考えた$\mathbf{R}$では自由系を形成します(cf.備考1)。

#### 命題 25 {#alg-ii-s1-prop-25 .statement tag=05LX}

*$A, B$ を 2 つの環、$\rho : B \to A$ 環準同型、および $E$ の $A$ モジュールとします。 $(\alpha_\lambda)_{\lambda \in L}$ を、左の $B$ モジュールとみなされる $A$ の生成する系 (それぞれ元、基底の自由ファミリー) とします。 $(a_\mu)_{\mu \in M}$ を $A$ モジュール $E$ の生成する系 (それぞれ元、基底の自由ファミリー) とします。この場合、$(\alpha_\lambda a_\mu)_{(\lambda, \mu) \in L \times M}$ は、$B$ モジュール $\rho_*(E)$ の生成する系 (それぞれ ($\rho$ が単射の場合) 元、基底の自由族) です。

$\gamma_\mu \in A$ と $(\alpha_\lambda)$ が $A$ の生成する系である $x = \sum_{\mu \in M} \gamma_\mu a_\mu$ の場合、すべての $\mu \in M$、よって $x = \sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu$ に対して、$\beta_{\lambda \mu} \in B$ を付けて $\gamma_\mu = \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda$ と書くことができます。一方、$(\alpha_\lambda)$ と $(a_\mu)$ がフリー ファミリの場合、関係 $\sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu = 0$ は $\beta_{\lambda \mu} \in B$ とともに $\sum_{\mu \in M} \left( \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda \right) a_\mu = 0$ と記述できます。したがって、$\rho$ が単射の場合、すべての $\mu \in M$ に対して $\sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda = 0$ を意味し、したがってすべての $\lambda, \mu$ に対して $\beta_{\lambda \mu} = 0$ を意味します。

#### 系 {#alg-ii-s1-n13-cor-1 .statement tag=05LY}

*$A$ が有限生成された左 $B$ モジュールであり、$E$ が有限生成された左 $A$ モジュールである場合、$\rho_*(E)$ は有限生成された左 $A$ モジュールです。

$C$ を 3 番目の環、$\rho' : C \to B$ 環準同型、そして $\rho'' = \rho \circ \rho'$ を合成準同型とします。 定義の直後に、すべての $A$ モジュール $E$ に対して $\rho''_*(E) = \rho'_*(\rho_*(E))$ が続きます。特に、$\rho$ が $A$ 上の $B$ の *同型* である場合、$E = \rho'_*(\rho_*(E))$ になります。ここで、$\rho'$ は $\rho$ の逆同型を表します。

#### 注意 {#alg-ii-s1-n13-rem-1 .statement tag=05LZ}

(1) $K$ を体および $K$ の $A$ 部分環を次の性質とします: $K$ の元のすべての有限族 $(\xi_i)_{1 \leq i \leq n}$ に対して、非ゼロで次のような $\gamma \in A$ が存在します。 $1 \leq i \leq n$ に対する $\gamma \xi_i \in A$ ($A$ が *可換* で、$K$ が $A$ の分数の体であるときに常に満たされる仮定)。 $E$ を $K$ と $E_{[A]}$ のスカラーの環を $A$ に制限することで得られる $A$ 加群のベクトル空間とします。次に、$(x_\lambda)_{\lambda \in L}$ の家族が $E_{[A]}$ に *自由* であれば、 $E$ にも *自由* です。注意は、$L = \{1, n\}$; の場合に限定されるかもしれません。 関係 $\sum_{i=1}^n \xi_i x_i = 0$ と $\xi_i \in K$ があり、すべての零ではなく $\xi_i$ があれば、すべての $\beta \in A$、$\sum_{i=1}^n (\beta \xi_i) x_i = 0$ についても同様になります。 仮定までに、すべての $i$ に対して $\beta \xi_i = \alpha_i$ 属するから $A$ になるように、$A$ で $\beta \neq 0$ を仮定できます。しかし、関係 $\sum_{i=1}^n \alpha_i x_i = 0$ は仮定に反しており、$\alpha_i$ がすべて零ではありません。

(2) 環準同型 $\rho : B \to A$ が全射で、$b$ がその核である場合 (したがって、$A$ は $B/b$ と標準的に識別されます)、すべての $A$ モジュール $E$ について、 $b$ は $\rho_*(E)$ の消滅子に含まれており、$E$ は、no. 12 で定義されたプロセスによって $\rho_*(E)$ から派生した $A$ モジュールです。

$A, B$ を 2 つの環と $\rho : B \to A$ 準同型とします。 $E$ を $A$ モジュール、$F$ を $B$ モジュールとします。 *B 線形* 写像 $u : F \to \rho_*(E)$ (混乱がなければ、* $F$ *into* $E$ の *B-線型写像とも呼ばれます) は、$B$ モジュール $F$ への *半線形マッピング* ($\rho$ に対して) とも呼ばれます。 $A$-モジュール$E$;順序付けられた対 $(u, \rho)$ は $F$ から $E$ への *二型性 * であるとも言われています。したがって、これは、$x \in F, y \in F$ と $\beta \in B$ について、

$$
\begin{cases}
u(x + y) = u(x) + u(y) \\
u(\beta x) = \rho(\beta) u(x).
\end{cases}
$$

混乱が生じない限り、$F$ から $E$ への$B$ の線形マッピングの集合 $\mathrm{Hom}_B(F, \rho_*(E))$ は、$\mathrm{Hom}_B(F, E)$ とも書かれます。

$\rho$ が $A$ 上の $B$ の *同型* である場合、すべての $\beta \in B$ に対する関係 $u(\beta x) = \rho(\beta) u(x)$ は、すべての $\alpha \in A$ に対する $u(\rho'(\alpha)x) = \alpha x$ として書くこともできます。ここで、$\rho'$ は、逆同型を表します$\rho$; $u$ が $\rho$ に対して半線形であると言うのは、 $u$ が $\rho'_*(F)$ の *A-線型写像を *$E$ に * したものであるというと等価です。

#### 例 {#alg-ii-s1-n13-exa-1 .statement tag=05M0}

$A$ モジュール $E$ のホモテティー $h_\alpha : x \mapsto \alpha x$ は必ずしも線形写像ではないことが確認されています (no. 1)。しかし、$\alpha$ が *可逆* である場合、$h_\alpha$ は、$\alpha(\lambda x) = (\alpha \lambda \alpha^{-1})(\alpha x)$ について、$A$ の内部自己同型 $\xi \mapsto \alpha \xi \alpha^{-1}$ に対して *半線形* 写像 (さらに全単射) です。

C を 3 番目の環、$\rho': C \to B$ 準同型、G を C モジュールとします。 $v: G \to F$ が $\rho'$ に対する半線形写像である場合、合成 $w = u \circ v$ は、準同型 $\rho'' = \rho \circ \rho'$ に対する G から E への半線形写像です。 $\rho$ が *同型* で、$u: F \to E$ が $\rho$ に対する *全単射 * 半線形写像である場合、逆の写像 $u': E \to F$ は、$\rho$ の逆同型* $\rho': A \to B$ に対する * 半線形写像です。

したがって、A の集合環構造と E の左A-加群構造の順序付き対 (A, E) を与えることによって定義される構造の種について、*二型* $(u, \phi)$ は *射* (*集合) として解釈できることがわかります。 理論*、IV, § 2, no. 1);以下では常に、この射の選択が作成されたと仮定します。

*注意 (3)*。 $A_1, A_2$ を 2 つの環、$A = A_1 \times A_2$ の積、そして A の $e_1 = (1, 0),\ e_2 = (0, 1)$ とすることで、$A_1$ と $A_2$ は A の両側の理想 $Ae_1$ と $Ae_2$ で標準的に同一視されます。すべての A-加群 E について、 $e_1E$ と $e_2E$ は E のサブ A モジュール $E_1,\ E_2$ で、それぞれ $e_2$ と $e_1$ によって消滅するため、$A/Ae_2$ は $A_1$ と、$A/Ae_1$ は $A_2$ と標準的に識別され、 $E_1$ (それぞれ $E_2$) には、$A_1$ モジュール (それぞれ $A_2$ モジュール) 構造が与えられます。さらに、E は $E_1$ と $E_2$ の *直和* であり、すべての $x \in E$ は $x = e_1x + e_2x$ と書くことができ、関係 $e_1x = e_2y$ は $e_1x = e_1^2x = e_1e_2y = 0$ を意味します。逆に、$A_1$ モジュール $F_1$ および $A_2$ モジュール $F_2$ の注文されたすべての対からなるについて、$E_1$ を A-加群 $(p_1) * (F_1)$、$E_2$ とします。 A-加群 $(p_2) * (F_2)$、$p_1$、および $p_2$ は、それぞれ $A_1$ と $A_2$ 上の A の射影です。それからA-加群 $E = E_1 \oplus E_2,\ E_1 = e_1E,\ E_2 = e_2E$。したがって、A-加群の学習は、$A_1$ モジュールの学習と $A_2$ モジュールの学習に減らされます。特に、E のすべての部分加群 M は形 $M_1 \oplus M_2$ であり、$M_1 = e_1M$ と $M_2 = e_2M$ です。

### 14. マルチモジュール

A、B を 2 つの環とし、集合 E で *同じ* 加法法則を持ち、演算子の環がそれぞれ A と B である 2 つの左加群構造を考えます。 $\mathscr{E}$ を加法群 E の自己準同型環とし、すべての $\alpha \in A$ (それぞれ $\beta \in B$) について、$h_\alpha$ (それぞれ $h'_\beta$) を元 $x \mapsto \alpha x$ (それぞれ $x \mapsto \beta x$) とします。 $\mathscr{E}$の。明らかに、次の 3 つのプロパティは同等です: (a) $\alpha$ と $\beta$ のすべてに対して $h_\alpha \circ h'_\beta = h'_\beta \circ h_\alpha$。 (b) 準同型 $a \mapsto h_\alpha$ の下の A の像は $\mathrm{Hom}_B(E, E)$ に *含まれています*。 (c) 準同型 $\beta \mapsto h'_\beta$ の下の B の像は $\mathrm{Hom}_A(E, E)$ に *含まれます*。問題のA-加群 (またはB-加群) 構造が権利加群構造である場合、環 A (または B) は (b) (または (c)) で $A^0$ (または $B^0$) に置き換えられなければなりません。上記のプロパティは、E で定義された 2 つの (左または右) 加群構造が *互換性がある* というというによって表現できます。

#### 定義 13 {#alg-ii-s1-def-13 .statement tag=05M1}

*$(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$ *環の 2 つの家族としましょう。 * $((A_\lambda),\ (B_\mu))$*-マルチモジュール* (または、*環* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$ ファミリの *マルチモジュール) *は集合* E *それぞれ* $\lambda \in L$、*左* $A_\lambda$* モジュール構造、およびそれぞれ* $\mu \in M$、*右* $B_\mu$* モジュール構造。これらすべての加群構造は 1 つの他の.* と互換性があります。

ファミリ $(B_\mu)$ (それぞれ $(A_\lambda)$) が空の場合、E は *left* (それぞれ *right*) *multimodule* と呼ばれます。 Card(L) + Card(M) = 2 の場合、「*multimodule*」の代わりに「*両側加群*」と言います。その場合、(その反対の演算子の置き換えること環によって常に実行できるように、cf. no. 1) 両側加群が環 A および *正しい加群* に関して *左加群* 構造を持つと考えると便利な場合がよくあります。 環 B に対する構造、法則の順列性は関係で表されます。

$$
\alpha(x\beta) = (\alpha x)\beta \quad \text{for } x \in E, \alpha \in A, \beta \in B.
$$

そして、E は *(A, B)*-*両側加群* であるとも言われます。

集合 E 上の 2 つの *マルチモジュール* 構造は、E 上のすべての加群構造と、これらのマルチモジュール構造のいずれか定義するが 1 つの他のと互換性がある場合、*互換性がある*と言われます。

#### 例 {#alg-ii-s1-n14-exa-1 .statement tag=05M2}

(1) 環では、$A_s$ と $A_d$ の加群構造は互換性があるため、A は標準的に (A, A)-bimodule と見なすことができます。

(2) 左A-加群 E には、環 $\operatorname{End}_A(E)$ に対する正規の左加群構造があり、E の A-加群および $\operatorname{End}_A(E)$ モジュール構造は *互換性* があります。

明らかに、E が環の 2 つのファミリー $(A_\lambda)_{\lambda \in L}, (B_\mu)_{\mu \in M}$ にわたるマルチモジュールである場合、E は任意の 2 つのサブファミリー $(A_\lambda)_{\lambda \in L'}, (B_\mu)_{\mu \in M'}$ にわたるマルチモジュールでもあります。ここで、$\lambda \in L'$ と $\mu \in M'$ の $A_\lambda$ モジュール構造と $B_\mu$ モジュール構造は、最初に与えられたものです。

マルチモジュールは演算子と可換な群の特定の例であるため、nos の結果は次のようになります。 2 ～ 10 (cf. no. 10、*注意*) が適用できます。特に、E、F が 2 つの $((A_\lambda), (B_\mu))$ マルチモジュールの場合、 *準同型* $u : E \to F$ は写像であり、すべての $\lambda \in L$ については $A_\lambda$ 準同型であり、すべての $\mu \in M$ については $B_\mu$ 準同型です。 $((A_\lambda), (B_\mu))$ マルチモジュールの安定した部分群は $((A_\lambda), (B_\mu))$ マルチモジュール (*サブマルチモジュール* と呼ばれる) であり、同様に部分群 (*商マルチモジュール* と呼ばれる) による商も同様です。 積と直和についても同様です。

E を $((A_\lambda), (B_\mu))$ マルチモジュールとし、各 $\lambda \in L$ (それぞれ $\mu \in M$) について $\phi_\lambda : A'_\lambda \to A_\lambda$ (それぞれ $\psi_\mu : B'_\mu \to B_\mu$) を環準同型とします。明らかに、E で指定された $\phi_\lambda$ と $A_\lambda$ モジュール構造に関連付けられた $A'_\lambda$ モジュール構造、および E で指定された $\psi_\mu$ と$B_\lambda$ モジュール構造に関連付けられた $B'_\mu$ モジュール構造は、1 つの他のおよびしたがって定義すると互換性があります。 E では、指定された $((A_\lambda), (B_\mu))$ マルチモジュール構造と $\phi_\lambda$ および $\psi_\mu$ に *関連付けられている*と言われている $((A'_\lambda), (B'_\mu))$ マルチモジュール構造。

E、F が 2 つの $((A_\lambda), (B_\mu))$ マルチモジュールの場合、F への E の準同型の加法群は、$\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ (または単に $\operatorname{Hom}(E, F)$) で表されます。 no. 2 の式 (6) から (8) は明らかに $((A_\lambda), (B_\mu))$ マルチモジュール準同型に有効であり、特に $\operatorname{Hom}(E, E) = \operatorname{End}(E)$ には *環* 構造があります。

さらに、Hom(E, F) には標準的な *左* End(F) モジュール構造と *右* End(E) モジュール構造があり、これら 2 つの構造には互換性があります。他の語では、Hom(E, F) には正規 (End(F), End(E))-**両側加群** 構造があります。

ここで、E がマルチモジュール構造を持っており、その左 (右) 演算子の環が、一方で $\lambda \in L$ の $A_\lambda$ (それぞれ $\mu \in M$ の $B_\mu$) であり、他方で他のファミリー $(A'_{\lambda'})_{\lambda' \in L'}$ の環 (それぞれ$(B'_{\mu'})_{\mu' \in M'}$）。 同様に、F がマルチモジュール構造を持っており、その左 (または右) 演算子の環が、一方で $\lambda \in L$ の $A_\lambda$ (それぞれ $\mu \in M$ の $B_\mu$) であり、他方で他のファミリー $(A''_{\lambda''})_{\lambda'' \in L''}$ の環であると仮定します。 $(B''_{\mu''})_{\mu'' \in M''}$);略して、E は (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$)) マルチモジュール、F は (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$)) マルチモジュールであると言います。 E と F を (($A_\lambda$), ($B_\mu$)) マルチモジュールとみなして、演算子をサブファミリー ($A_\lambda$) と ($B_\mu$) に *制限*します。 この番号の冒頭で述べたことによると、E と F 定義するで与えられるマルチモジュール構造は標準的に環準同型

$$
A'_{\lambda'} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E), \qquad {B'_{\mu'}}^0 \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E),
$$
$$
A''_{\lambda''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F), \qquad B''_{\mu''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F);
$$

さらに、$\operatorname{End}_{(A_\lambda), (B_\mu)}(E)$ の 2 つの元 (それぞれ $\operatorname{End}_{(A_\lambda), (B_\mu)}(F)$)、$A'_{\lambda'}$ または ${B'_{\mu'}}^0$ (それぞれ $A''_{\lambda''}$ または $B''_{\mu''}$) のうちの 2 つの異なる環の元の像は置換可能です。つまり、上記の準同型定義するは、$\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ 上の *マルチモジュール* 構造であり、*left* 演算子の環は $A''_{\lambda''}$ ($\lambda'' \in L''$) と $B'_{\mu'}$ ($\mu' \in M'$) であり、*right* 演算子の環であるということになります。 $A'_{\lambda'}$ ($\lambda' \in L'$) と $B''_{\mu''}$ ($\mu'' \in M''$) です。

現在、$E'$ が (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$)) マルチモジュールであり、$F'$ が (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$)) マルチモジュールである場合、 $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')$は

$$
((A''_{\lambda''}), (B'_{\mu'}); (A'_{\lambda'}), (B''_{\mu''}))\text{-multimodule};
$$

$u : E' \to E, v : F \to F'$ がマルチモジュール準同型の場合、

$$
\operatorname{Hom}(u, v) : \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F) \to \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')
$$

は no. 2 のように定義されており、*マルチモジュール* 準同型です。

#### 注意 {#alg-ii-s1-n14-rem-1 .statement tag=05M3}

(1) F を A-加群および C を環 A の *中心* とします。中心相似関数はすべての相似関数と可換であるため、F は *両側加群* 構造を持ち、その左演算子の環は A と C です。 E が他の A-加群の場合、$\operatorname{Hom}_A(E, F)$ は正規の C-*加群* 構造になります (ここで、$f \in \operatorname{Hom}_A(E, F)$ と $\gamma \in C$ の場合、$\gamma f$ は準同型 $x \mapsto \gamma f(x)$ です)。 E'、F' が 2 つの A-加群、$u : E' \to E, v : F \to F'$ 2 つの A 準同型である場合、写像 $\operatorname{Hom}(u, v)$ は C-*線型* です。

(2) E を左A-加群とします。 A は標準的な (A, A) バイモジュール構造を持っているため、インデックス付け集合 T に対して直和 $A^{(T)}$ があります。上記により、$\mathrm{Hom}_A(A_s^{(T)}, E)$ には、$A_s^{(T)}$ の *右* A-加群構造から生じる正規 *左A-加群* 構造があります。$f \in \mathrm{Hom}_A(A_s^{(T)}, E)$ と $\alpha \in A$ の場合、$\alpha f$ は線形写像です$x \mapsto f(x\alpha)$。 系 2 から命題 17 の no. 11 定義する標準写像 $j_{E, T}$ 積加群 $E^T$ から $\mathrm{Hom}_A(A_s^{(T)}, E)$、像以下家族$(x_t)_{t \in T}$の$j_{E, T}$は線形写像$f : A_s^{(T)} \to E$で、すべての$t \in T$に対して$f(e_t) = x_t$になります（$(e_t)$は$A_s^{(T)}$の標準基底です）。 $j_{E, T}$ は *全単射 * であることが知られており (*loc. cit.*)、$\mathrm{Hom}_A(A_s^{(T)}, E)$ における A-加群構造の上記の定義から、$j_{E, T}$ は *A-linear* であることがわかります。最後に、$u : E \to F$ が A-加群準同型の場合、図式

$$
\begin{array}{ccc}
E^T & \xrightarrow{j_{E, T}} & \mathrm{Hom}_A(A_s^{(T)}, E) \\
u^T \downarrow & & \downarrow \mathrm{Hom}(1, u) \\
F^T & \xrightarrow{j_{F, T}} & \mathrm{Hom}_A(A_s^{(T)}, F)
\end{array}
$$

は*可換*です。

T が単一の元で構成される場合、$j_E : E \to \mathrm{Hom}_A(A_s, E)$ は no. 2, *例* 1 で定義された写像 $x \mapsto \theta_x$ であることに注意してください。

### 練習問題 {#alg-ii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
