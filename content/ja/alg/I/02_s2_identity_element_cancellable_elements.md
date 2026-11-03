---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 2
section_title: Identity element; cancellable elements; invertible elements
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 12-24, 126-129
pdf_pages: 0036-0048, 0150-0153
extraction: ocr
subsections:
    - "no": 1
      title: IDENTITY ELEMENT
      page: 12
      pdf_page: 36
    - "no": 2
      title: CANCELABLE ELEMENTS
      page: 14
      pdf_page: 38
    - "no": 3
      title: INVERTIBLE ELEMENTS
      page: 15
      pdf_page: 39
    - "no": 4
      title: MONOID OF FRACTIONS OF A COMMUTATIVE MONOID
      page: 17
      pdf_page: 41
    - "no": 5
      title: 'APPLICATIONS: I. RATIONAL INTEGERS'
      page: 20
      pdf_page: 44
    - "no": 6
      title: 'APPLICATIONS: II. MULTIPLICATION OF RATIONAL INTEGERS'
      page: 22
      pdf_page: 46
    - "no": 7
      title: 'APPLICATIONS: III. GENERALIZED POWERS'
      page: 23
      pdf_page: 47
    - "no": 8
      title: NOTATION
      page: 23
      pdf_page: 47
statements: 26
exercises: 17
content_sha256: 77de053c2b63e46edb88a04a307e60a1d1c1533baaaac2824e37536d0a5be482
translated_from: content/en/alg/I/02_s2_identity_element_cancellable_elements.md
translation_method: google
source_content_sha256: 4e4d1e772eb5f248a858ce2f9c1dbddee958a8fa5c19120df031143b30855c75
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 479e3131ec9eafdad8eb5e14cc085109670ce86f33826dd364541e66b8476c41
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 単位元;キャンセル可能元; 可逆元

### 1. 単位元

#### 定義 1 {#alg-i-s2-def-1 .statement tag=056M}

集合 $E$ 上の合成法則 $\top$ の下で、すべて $x \in E$、$e \top x = x \top e = x$ である場合、$E$ の要素 $e$ は恒等要素と呼ばれます。

特定の法則 $\top$ の下には、$e$ と $e'$ が単位元の場合、$e = e \top e' = e'$ が存在するのは最大でも 1 つの単位元です。 単位元はすべての元と置換可能です。これは中心となる元です。

#### 定義 2 {#alg-i-s2-def-2 .statement tag=056N}

単位元のマグマをユニタルマグマといいます。 $E, E'$ がユニタルマグマの場合、マグマ $E$ の準同型がマグマ $E'$ に入る$E$ の写像単位元から$E'$ の単位元をユニタル準同型 (または射) の $E$ を $E'$ に変換します。結合性のある単位マグマはモノイドと呼ばれます。

$E, E'$ がモノイドの場合、$E$ から $E'$ へのユニタル射はモノイド準同型または $E$ から $E'$ へのモノイド射と呼ばれます。

#### 例 {#alg-i-s2-n1-exa-1 .statement tag=056O}

(1) 自然数の集合 $\mathbf{N}$ では、0 は加法の下の単位元であり、1 は乗法の下の単位元です。 これら 2 つの法則はそれぞれ、$\mathbf{N}$ に可換モノイド構造 (集合理論, III, § 3, no. 3) を与えます。

(2) 集合 $E$ の部分集合の集合では、$\varnothing$ は法則 $\cup$ の下で単位元 、法則 $\cap$ の下で $E$ です。より一般的には、格子内で最小の元が存在する場合、それは法則 sup の下の単位元です。逆に、この法則の下に単位元が存在する場合、それは集合の最小の元になります。 最大の元および法則 inf についても同様です。

(3) 集合 $\mathbf{N}$ には、法則 $(x, y) \mapsto x^y$ の下に単位元がありません。 $E \times E$ の部分集合の間の法則 $(X, Y) \mapsto X \circ Y$ では、対角線 $\Delta$ は単位元です。 法則 $(f, g) \mapsto f \circ g$ の下では、$E$ の写像から $E$ の $E$ 恒等写像と $E$ の間は単位元です。

(4) $E$ をマグマとし、$E$ の $R$ 同値関係が $E$ (§ 1, no. 6) の法則と互換性があるとします。 $e$が$E$の単位元である場合、$E/R$の$e$の標準像はマグマ$E/R$の単位元です。

ユニタル マグマの単位元はユニタル準同型です。 2 つの単位の合成準同型も 1 つです。 写像が単位マグマ同型であるためには、それが全単射単位準同型であることが必要かつ十分であり、その逆の写像が単位準同型になります。 $E$ と $E'$ を単体マグマ、$e'$ 単位元を $E'$ とします。 $E$ から $E'$ 写像 $E$ から $e'$ への定数写像は単位準同型であり、自明準同型と呼ばれます。

ユニタルマグマ (それぞれモノイド) のファミリーの積は、ユニタルマグマ (それぞれモノイド) です。

単位マグマ (それぞれモノイド) のすべての商マグマは単位マグマ (それぞれモノイド) です。

$E$ を単体マグマ、$e$ をその単位元とします。 $e \in A$ となるような $E$ のサブマグマ $A$ を $E$ のユニットサブマグマと呼びます。明らかに$e$はマグマ$A$の単位元です。 $E$ の単位サブマグマのすべての共通部分は、$E$ の単位サブマグマです。 $X$ が $E$ の部分集合である場合、$E$ 含む $X$ の最小ののユニットサブマグマが存在します。それは$X$によって生成された$E$のユニタルサブマグマと呼ばれます。 $X$ が空の場合、それは $\{e\}$ と等しくなります。 $E$ がモノイドの場合、$E$ のユニタルサブマグマは $E$ の部分モノイドと呼ばれます。

$F$ が単位元を持たないマグマである場合、$F$ のサブマグマは単位元を有する可能性があります。たとえば、$F$ が結合的で、$h$ が $F$ (I, § 1, no. 4) のべき等元である場合、$h \uparrow x \uparrow h$ の集合 ($x$ が $F$ を通過する) は、 $F$ と $h$ は単位元となります。

$E$ が単位元 $e$ を持つマグマである場合、$E$ のサブマグマ $A$ は、$e \notin A$ がまだ単位元を所有している可能性があります。

#### 定義 3 {#alg-i-s2-def-3 .statement tag=056P}

$E$ を単体マグマとします。 $E$の単位元は、$E$の元の空家族の合成と呼ばれます。

$(x_\alpha)_{\alpha \in \varnothing}$ が E の元の空族である場合、その合成 $e$ は $\prod_{\alpha \in \varnothing} x_\alpha$ によっても表されます。たとえば、次のように書きます。
$$
\prod_{q \leq i \leq p} x_i = e
$$
$p < q$ ($p, q \in \mathbf{N}$) のとき。同様に、任意の $x$ に対して $\prod^0 x = e$ と書きます。 *これらの定義定理では、集合 A と B_i が空ではないという仮定であれば、§ 1 の 1 と 3 は真のままになります。* 同様に、式 $\prod^{m+n} x = \left( \prod^m x \right) \prod^n \left( \prod^n x \right)$ と $\prod^{mn} x = \prod^m \left( \prod^n x \right)$ は $m \geq 0, n \geq 0$ に対して真になります。

E を、法則が $\top$ で表され、$e$ がその単位元で表される単位マグマであるとします。 E の元の家族 $(x_i)_{i \in I}$ の *サポート* は、添字 $i \in I$ の集合で、$x_i \neq e$ になります。 $(x_i)_{i \in I}$ を、E *with 有限台* の元の家族とする。次の 2 つの場合には、定義する合成 $\prod_{i \in I} x_i$ となります。

(a) 集合 I は完全に順序付けされています。
(b) E は結合的であり、$x_i$ はペアごとに変更可能です。

これら 2 つのケースでは、S を家族 $(x_i)$ の扶養者とします。 J が I 含む S の有限部分集合である場合、J の元の数上の帰納法からわかるように、$\prod_{i \in J} x_i = \prod_{i \in S} x_i$、ケース (a) では適用定理 1 の § 1 および(b) の場合、定理 3/§ 1。 $\prod_{i \in I} x_i$ が I 含む S のすべての有限部分集合に対して、共通の値合成 $\prod_{i \in J} x_i$ を表すとします。 I が $\mathbf{N}$ の区間 $[p, \to]$ であるとき、 $\prod_{i = p}^\infty x_i$ とも書きます。

これらの定義と記法、定理の§ 1と注意の1と3、定理3拡大するが有限台の家族に続きます。

*加法的に*書かれた法則の単位元は通常0で表され、*零*または*ヌルの元* (またはときどき *原点*)と呼ばれます。 *乗法*で書かれた法則では、通常は1で表され、*単位元* (または*単位元*) と呼ばれます。

### 2. キャンセル可能元

#### 定義 4 {#alg-i-s2-def-4 .statement tag=056Q}

*集合 E 上で合成 $\top$ の法則が与えられると、E の写像 $x \mapsto a \top x$ (それぞれ $x \mapsto x \top a$) を元 $a \in E$ によって左変換 (または右変換) と呼ばれます。

移行の反対側の法則では、左の翻訳が右の翻訳になり、その逆になります。

$\gamma_a, \delta_a$ (または $\gamma(a), \delta(a)$) が $a \in E$ による左右の平行移動を表すものとします。それから
$$
\gamma_a(x) = a \top x, \qquad \delta_a(x) = x \top a.
$$

#### 命題 1 {#alg-i-s2-prop-1 .statement tag=056R}

*法則* $\mathsf{T}$ *が結合している場合、すべて* $x \in E$ *および* $y \in E$

$$
\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y, \qquad \delta_{x \mathsf{T} y} = \delta_y \circ \delta_x.
$$

$z \in E$ の皆様へ:

$$
\gamma_{x \mathsf{T} y}(z) = (x \mathsf{T} y) \mathsf{T} z = x \mathsf{T} (y \mathsf{T} z) = \gamma_x(\gamma_y(z))
$$
$$
\delta_{x \mathsf{T} y}(z) = z \mathsf{T} (x \mathsf{T} y) = (z \mathsf{T} x) \mathsf{T} y = \delta_y(\delta_x(z))
$$

他の語、写像 $x \mapsto \gamma_x$は、マグマ$E$から集合写像の$E$の$E^E$が法則と法則で集合に準同型です。 $(f, g) \mapsto f \circ g$; 写像 $x \mapsto \delta_x$ は、$E$ の準同型を集合 $E^E$ に、反対の法則を加えます。 $E$ がモノイドの場合、これらの準同型はユニタルです。

#### 定義 5 {#alg-i-s2-def-5 .statement tag=056S}

*元* $a$ *マグマの* $E$ * $a$ * による左 (または右) の翻訳が単射である場合、左 (または右) はキャンセル可能 (または通常) と呼ばれます。左右のキャンセル可能元をキャンセル可能（またはレギュラー）元と呼びます。

他の語では、法則 $\mathsf{T}$ の下で $a$ がキャンセル可能であるためには、関係 $a \mathsf{T} x = a \mathsf{T} y, x \mathsf{T} a = y \mathsf{T} a$ のそれぞれが $x = y$ を含意することが必要かつ十分です (これらの等式のそれぞれから「a はキャンセルできる」と言われます)。 法則 $\mathsf{T}$ の下に単位元 $e$ が存在する場合、この法則の下でキャンセル可能です。つまり、翻訳 $\gamma_e$ と $\delta_e$ は、$E$ の恒等写像になります。

#### 例 {#alg-i-s2-n2-exa-1 .statement tag=056T}

(1) すべての自然数は加法の下でキャンセル可能です。 自然数 $\neq 0$ はすべて乗法でキャンセル可能です。

(2) ラティスでは、単位元 (少なくとも元) 以外に、法則 sup の下でキャンセル可能な元が存在することはありません。 inf についても同様です。特に、集合 $E$ の部分集合の集合では、法則 $\cup$ の下でキャンセル可能な元は$\varnothing$ のみであり、$E$ の下で唯一キャンセル可能な元です。 法則 $\cap$。

#### 命題 2 {#alg-i-s2-prop-2 .statement tag=056U}

*集合キャンセル可能 (それぞれ左キャンセル可能、それぞれ右キャンセル可能) 元の結合マグマはサブマグマです。

$\gamma_x$ と $\gamma_y$ が単射であれば、 $\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y$ (命題 1) も単射です。 $\delta_{x \mathsf{T} y}$も同様です。

### 3. 可逆元

#### 定義 6 {#alg-i-s2-def-6 .statement tag=056V}

*$E$ * を単一マグマ、$\mathsf{T}$ を合成の法則、e を単位元、* $x$ * および* $x'$ * $E$ の 2 つの元とします。 $x'$ *は、* $x$ *if* $x' \mathsf{T} x = e$ *(それぞれ $x \mathsf{T} x' = e$、それぞれ $x' \mathsf{T} x = x \mathsf{T} x' = e$)* の左逆行列 (それぞれ右逆行列、それぞれの逆行列) と呼ばれます。

*元* $x$ *of* $E$ *左反転 (それぞれ右反転、それぞれ反転) がある場合、左反転 (それぞれ右反転、それぞれ反転) と呼ばれます。

*すべての元が可逆であるモノイドを群と呼びます。*

対称と対称可能は、反転と可逆の代わりにときどき使用されます。 E の法則が加法的に書かれる場合、通常は逆ではなく負といいます。

#### 例 {#alg-i-s2-n3-exa-1 .statement tag=056W}

(1) 単位元はそれ自体の逆数です。

(2) E の写像から E 元への集合において、 f が全射 (それぞれ単射) の場合、 f は左可逆 (それぞれ右可逆) です。左の逆行列 (それぞれ右の逆行列) は、f (集合理論, II, § 3, no. 8, 定義 11) に関連付けられた後退 (それぞれ切断) になります。 f が可逆であるためには、f が全単射であることが必要かつ十分です。その一意の逆数は f の逆全単射になります。

E と F を 2 つの単位マグマ、f を E から F への単位準同型とする。x' が E における x の逆数である場合、f(x') は F における f(x) の逆数である。したがって、x が E の可逆元である場合、f(x) は F の可逆元である。

特に、R がユニタルマグマ E 上の法則と同値関係互換性がある場合、E の可逆元の標準像は E/R で反転可能です。

#### 命題 3 {#alg-i-s2-prop-3 .statement tag=056X}

E をモノイドとし、E の x 元とします。

(i) x が左 (または右) 可逆であるためには、x による右 (または左) の変換が全射的であることが必要かつ十分です。

(ii) x が可逆であるためには、それが左右に可逆であることが必要かつ十分です。その場合、x は一意の逆行列を持ち、それはまたその一意の左 (または右) 逆行列でもあります。

x' が x の左逆行列の場合 (命題 1)

$$
\delta_x \circ \delta_{x'} = \delta_{x' \top x} = \delta_e = \mathrm{Id}_E
$$

そして$\delta_x$は全射です。逆に、$\delta_x$ が全射であれば、$\delta_x(x') = e$ と $x'$ が $x$ の左逆元となるような E の元 $x'$ が存在します。 (i) のもう 1 つの主張も同様です。

$x'$ (または $x''$) が $x$ の左 (または右) 逆数である場合、

$$
x' = x' \top e = x' \top (x \top x'') = (x' \top x) \top x'' = e \top x'' = x'',
$$

よって (ii)。

#### 注意 {#alg-i-s2-n3-rem-1 .statement tag=056Y}

E をモノイドとし、E の x 元とします。x が可逆のままであれば、それはキャンセル可能のままになります。なぜなら、$x'$ が $x$ の左逆行列である場合、

$$
\gamma_{x'} \circ \gamma_x = \gamma_{x' \top x} = \gamma_e = \mathrm{Id}_E
$$

$\gamma_x$ は単射です。特に、x が左可逆である場合、x による左および右の変換は全単射になります。逆に、$\gamma_x$ が全単射であると仮定します。 $xx' = \gamma_x(x') = e$ となるような $x' \in E$ が存在します。次に $\gamma_x(x'x) = (xx')x = x = \gamma_x(e)$、したがって $x'x = e$ となるため、x は可逆です。同様に、$\delta_x$ が全単射である場合、x は可逆であることがわかります。

#### 命題 4 {#alg-i-s2-prop-4 .statement tag=056Z}

E をモノイドとし、E の x と y 可逆元をそれぞれ逆 x' と y' とします。すると、y' $\top$ x' は x $\top$ y の逆数になります。

関係の続きです
$$
(y' \top x') \top (x \top y) = y' \top (x' \top x) \top y = y' \top y = e
$$
(x $\top$ y) $\top$ (y' $\top$ x') の同様の計算。

#### 系 1 {#alg-i-s2-prop-4-cor-1 .statement tag=0570}

E をモノイドとします。 E の要素の順序列 $(x_\alpha)_{\alpha \in A}$ の各要素 $x_\alpha$ が逆数 $x'_\alpha$ を持つ場合、合成 $\prod_{\alpha \in A} x_\alpha$ は逆数 $\prod_{\alpha \in A'} x'_\alpha$ を持ちます。ここで、A' は、A の順序を反対の順序で置き換えることによって A から導出された完全な順序集合です。

この系は、Aの元の数で帰納法によって命題4から続きます。

特に、x と x' が逆数の場合、$\prod^n x$ と $\prod^n x'$ はすべての整数 $n \geq 0$ について逆数になります。

#### 系 2 {#alg-i-s2-prop-4-cor-2 .statement tag=0571}

モノイドでは可逆元の集合が安定です。

#### 命題 5 {#alg-i-s2-prop-5 .statement tag=0572}

モノイド内で x と x' が逆数であり、x が y と可換である場合、x' も同様です。

$x \top y = y \top x$ から $x' \top (x \top y) \top x' = x' \top (y \top x) \top x'$ が導き出され、したがって $(x' \top x) \top (y \top x') = (x' \top y) \top (x \top x')$、つまり $y \top x' = x' \top y$ が導き出されます。

#### 系 1 {#alg-i-s2-prop-5-cor-1 .statement tag=0573}

E をモノイド、E の X 部分集合、および X のセントラライザーである X' とします。 X' 属するから X' のすべての可逆元の逆数。

#### 系 2 {#alg-i-s2-prop-5-cor-2 .statement tag=0574}

モノイドでは、中心可逆元の逆は中心元です。

### 4. 可換モノイドの分数のモノイド

この番号では、e はモノイドの単位元を表し、x* は E の可逆元 x の逆数を表します。

E を可換モノイド、E の S 部分集合と S によって生成される E の S' 部分モノイドとします。

#### 補題 1 {#alg-i-s2-lem-1 .statement tag=0575}

E $\times$ S' 関係 R$\mathscr{R}$x、y$\mathscr{R}$ では、次のように定義されます。

「$x = (a, p), y = (b, q)$と$aqs = bps$のような$a, b \in E$と$p, q, s \in S'$が存在します。」

同値関係は、積モノイド E $\times$ S' 上の法則と互換性があります。

R が再帰的かつ対称であるのは明らかです。 $x = (a, p), y = (b, q)$ と $z = (c, r)$ を、R$\mathscr{R}$x, y$\mathscr{R}$ と R$\mathscr{R}$y, z$\mathscr{R}$ が成り立つような E $\times$ S' の元とする。すると、次のような S' の 2 つの元 s と t が存在します。
$$
aq s = bps, \quad br t = cqt,
$$
よってつまり、
$$
ar(stq) = bpsrt = cp(stq)
$$

したがって、$stq$ 属するから $S'$ まで、$R \{ x, z \}$ が成り立ちます。したがって、関係 $R$ は推移的です。

さらに、$R \{ x, y \}$と$R \{ x', y' \}$が成り立つように、$x = (a, p), y = (b, q), x' = (a', p'),$と$y' = (b', q')$を$E \times S'$の元とする。 $S'$ には、次のような $s$ と $s'$ が存在します。
$$
aqs = bps, \qquad a'q's' = b'p's',
$$
よってから、$(aa')(qq')(ss') = (bb')(pp')(ss')$ となり、したがって $ss' \in S'$ は $R \{ xx', yy' \}$ になります。したがって、同値関係 $R$ は、$E \times S'$ の合成の法則と互換性があります。

商マグマ $(E \times S')/R$ は可換モノイドです。

#### 定義 7 {#alg-i-s2-def-7 .statement tag=0576}

*$E$ を可換モノイド、$E$ の $S$ 部分集合と $S$ によって生成された $E$ の $S'$ 部分モノイドとします。 同値関係$R$が補助定理1で説明されている商モノイド$(E \times S')/R$は$E_S$で表され、$S$（または$S$の分母）に関連付けられた$E$の分数†のモノイドと呼ばれます*。

$a \in E$ と $p \in S'$ の場合、 $R$ を法とする $(a, p)$ の類は、一般に $a/p$ で表され、分子 $a$ と分母 $p$ を持つ分数と呼ばれます。その後、定義 $(a/p).(a'/|p') = aa'/|pp'$までに。 分数 $a/p$ と $a'/|p'$ は、$S'$ と$spa' = sp'a$ に $s$ が存在する場合にのみ等しくなります。もしそうなら、$S'$には$a\sigma = a'\sigma'$と$p\sigma = p'\sigma'$がある$\sigma$と$\sigma'$が存在します。特に$a \in E$の$a/p = sa/sp$と$S'$の$s, p$。 $E_S$の単位元は分数$e/e$です。

すべての$a \in E$を$a/e = \varepsilon(a)$とします。上記は、$\varepsilon$ が正規と呼ばれる $E$ の準同型である $E_S$ であることを示しています。すべての $p \in S'$、$(p/e).(e/p) = e/e$、したがって $e/p$ は $\varepsilon(p) = p/e$ の逆になります。したがって、$\varepsilon(S')$ のすべての元は反転可能です。次に、$a/p = (a/e).(e/p)$、よって
$$
a/p = \varepsilon(a)\varepsilon(p)^*
$$
したがって、$a \in E$ と $p \in S'$ の場合、モノイド $E_S$ は $\varepsilon(E) \cup \varepsilon(S)^*$ によって生成されます。

#### 命題 6 {#alg-i-s2-prop-6 .statement tag=0577}

※記法は定義7の$\varepsilon$は$E$の$E_S$の標準準同型を表します。
(i) $a$ と $b$ を $E$ に入れる。 位数の $\varepsilon(a) = \varepsilon(b)$ には、$sa = sb$ とともに $s \in S'$ が存在することが必要十分です。
(ii) $\varepsilon$ が単射的であるためには、$S$ のすべての元がキャンセル可能であることが必要かつ十分です。
(iii) $\varepsilon$ が全単射であるためには、$S$ のすべての元が可逆であることが必要かつ十分です。*

主張 (i) は明確であり、$S'$ のすべての元がキャンセル可能な場合に限り、$\varepsilon$ が単射であることを示しています。しかし、$E$ のキャンセル可能な元の集合は、$E$ の部分モノイド (no. 2, 命題 2) であるため、$S$ のすべての元がキャンセル可能であると言うのは同じことになります。

† $E$ 上の法則を加法的に書く場合、*差分モノイド* とも呼ばれます。

If $\varepsilon$ is bijective every 元 of S is invertible, for $\varepsilon(S)$ is composed of 可逆元 of $E_S$. Conversely, suppose every 元 of S is invertible; then every 元 of $S'$ is invertible (no. 3, 系 2 to 命題 4) and hence cancellable.このとき、$\varepsilon$は(ii)によって単射的であり、$a/p = \varepsilon(a.p^*)$は(1)によって単射的であるため、$\varepsilon$は全射的です。

#### 定理 1 {#alg-i-s2-thm-1 .statement tag=0578}

*E を可換モノイド、S 部分集合 E 、$E_S$ を S と $\varepsilon : E \to E_S$ 標準準同型に関連付けられた分数のモノイドとする。 Further let f be 準同型 of E into a monoid F (not necessarily commutative) such that every 元 of $f(S)$ is invertible in F. There exists one and only one 準同型 $\bar{f}$ of $E_S$ into F such that $f = \bar{f} \circ \varepsilon$.*

$\bar{f}$ が $E_S$ の準同型を F に変換して $f = \bar{f} \circ \varepsilon$ となる場合、
$$
\bar{f}(a/p) = \bar{f}(\varepsilon(a)\varepsilon(p)^*) = \bar{f}(\varepsilon(a))\bar{f}(\varepsilon(p))^* = f(a)f(p)^*
$$
$a \in E$と$p \in S'$、$\bar{f}$のよって一意性。

g を $g(a,p) = f(a)f(p)^*$ で定義される F に $E \times S'$ の写像とします。 g が F の $E \times S'$ の準同型であることを示します。 まず第一に、
$$
g(e,e) = f(e)f(e)^* = e.
$$
$(a,p)$ と $(a',p')$ を $E \times S'$ の 2 つの元とします。 $a'$ と $p$ は E で通勤し、$f(a')$ と $f(p)$ は F で通勤し、よって $f(a')f(p)^* = f(p)^*f(a')$ は no. 3、命題 5 で通勤します。 さらに$f(pp')^* = f(p'p)^* = (f(p')f(p))^* = f(p)^*f(p')^*$ by no. 3、命題 4、よって
$$
g(aa',pp') = f(aa')f(pp')^* = f(a)f(a')f(p)^*f(p')^* = f(a)f(p)^*f(a')f(p')^*
= g(a,p)g(a',p').
$$
$(a,p)$ と $(a',p')$ が合同 mod である場合、 g は $E \times S'$ 上の同値関係 R と互換性があることを示します。 R、$spa' = sap'$、よって $f(s)f(p)f(a') = f(s)f(a)f(p')$ を伴う $s \in S'$ が存在します。 $f(s)$ は可逆であるため、$f(p)f(a') = f(a)f(p')$ が続き、左乗法 $f(p)^*$ と右乗法 $f(p')^*$ が続きます。
$$
g(a',p') = f(a')f(p')^* = f(p)^*f(a) = f(a)f(p)^* = g(a,p).
$$
したがって、$\bar{f}(a/p) = g(a,p)$、よって $\bar{f}(\varepsilon(a)) = \bar{f}(a/e) = f(a)f(e)^* = f(a)$ となるような F に $E_S$ の準同型 $\bar{f}$ が存在します。 したがって、$\bar{f} \circ \varepsilon = f$です。

#### 系 {#alg-i-s2-n4-cor-1 .statement tag=0579}

*E と F を 2 つの可換モノイド、それぞれ E と F の S と T 部分集合、E の f 準同型を F にすると、$f(S) \subset T$ と $\varepsilon : E \to E_S, \eta : F \to F_T$ 標準準同型になります。 $g \circ \varepsilon = \eta \circ f$ となるような準同型 $g : E_S \to F_T$ は 1 つだけ存在します。*

E の準同型 $\eta \circ f$ を、S の元から $F_T$ の可逆元ごとに $F_T$ 写像に変換します。

#### 注意 {#alg-i-s2-n4-rem-1 .statement tag=057A}

(1) 定理 1 は、$(E_S, \varepsilon)$ が E に対する普遍写像問題の解であるというというによって、モノイドに対して、E のモノイド準同型と準同型をモノイドにして、写像元となるというによって表すこともできます。 S から可逆元 (*集合理論*、IV、 、no. 1)。したがって、この問題の他のすべての解は、独特の方法で $(E_S, \varepsilon)$ と同型であることがわかります (*loc. cit.*)。

(2) 上記の普遍写像問題に対する解の存在については、*集合理論*, IV, § 3, no. 2 (cf. 練習問題 17) からわかるように、モノイド E が可換であると仮定する必要はありません。

分数のモノイドの 2 つの重要な特殊なケースについて説明します。

(a) $\overline{E} = E_E$ とします。モノイド $\overline{E}$ は可逆元から構成される集合 $\varepsilon(E) \cup \varepsilon(E)^*$ によって生成されるため、$\overline{E}$ のすべての元は可逆です (no. 3、系 2 ～ 命題 4)。他の語では、$\overline{E}$ は可換群です。さらに、定理 1 により、E の準同型 $f$ を群 G に変換すると、形 $f = \bar{f} \circ \varepsilon$ で一意に因数分解できます。ここで、$\bar{f}: \overline{E} \to G$ は準同型です。 $\overline{E}$ は、* E の分数の *群 (加法記法の場合は、* E の差の *群) と呼ばれます。

(b) $\Phi = E_{\Sigma}$ とします。ここで、$\Sigma$ は E のキャンセル可能な元から構成されます。命題 6, (ii) により、E の標準準同型から $\Phi$ は単射法です。 $\Phi$の像で同一視するEまで利益が出ます。したがって、E は $\Phi$ の部分モノイドであり、E のすべてのキャンセル可能な元は $\Phi$ に逆数を持ち、$\Phi$ のすべての元は $a \in E$ と $p \in \Sigma$ を伴う形 $a/p = a.p^*$ になります。 $ap' = pa'$の場合に限り、$a/p = a'/p'$になります。 $\Phi$ の可逆元は分数 $a/p$ であることが簡単にわかります。ここで、$a$ と $p$ はキャンセル可能で、$p/a$ は $a/p$ の逆数です。

ここで、S をキャンセル可能な E の元の集合とし、$S'$ を S によって生成された E の部分モノイドとします。$a/p$ と $a'/p'$ が $E_S$ の 2 つの元である場合、$a/p = a'/p'$ は次の場合に限ります。 $ap' = pa'$ ($sap' = spa'$ の場合は、すべての $s \in S'$ の $ap' = pa'$ を意味します)。したがって、$E_S$ は、$E \cup S^*$ によって生成された $\Phi$ の部分モノイドと識別される可能性があります。

E のすべての元がキャンセル可能である場合、$\Phi = \overline{E}$ および E は可換群 $\Phi$ の部分モノイドになります。逆に、E が群の部分モノイドと同型の場合、E のすべての元はキャンセル可能です。

### 5. アプリケーション: I。合理的整数

合成加法の法則を持つ自然数の可換モノイド $\mathbf{N}$ を考えてみましょう。この法則 (*集合理論*、III, § 5, no. 2、系 3) では、$\mathbf{N}$ のすべての元がキャンセル可能です。 $\mathbf{N}$の差分の群は$\mathbf{Z}$で表されます。その元は *有理数整数* と呼ばれます。その法則は有理数整数*の*加法と呼ばれ、+でも表されます。 $\mathbf{N}$ から $\mathbf{Z}$ までの標準準同型は単射法であり、$\mathbf{N}$ の各元を $\mathbf{Z}$ の像と同一視するします。 $\mathbf{Z}$ の元は、$(m_1, n_1)$ と $(m_2, n_2)$ の間の関係によって$\mathbf{N} \times \mathbf{N}$ で定義同値類によって決定され、$m_1 + n_2 = m_2 + n_1$ と書かれます。 $\mathbf{N}$ の元 $m$ は、元 $(m + n, n)$ の類からなると識別されます。ここで、$n \in \mathbf{N}$; 元 $(n, m + n)$ の $\mathbf{Z}$ 類で陰性であることを認めます。 $\mathbf{N} \times \mathbf{N}$ のすべての元 $(p, q)$ は、$p \geq q$ の場合は形 $(m + n, n)$ に、$p \leq q$ の場合は形 $(n, m + n)$ に書き込まれます。したがって、$\mathbf{Z}$ は $\mathbf{N}$ の *和集合と、$\mathbf{N}$* の元のマイナスの集合です。 単位元 0 は、$\mathbf{N}$ のうち、マイナスの属するから $\mathbf{N}$ までの唯一の元です。

すべての自然数 $m$ について、$-m$ は $m$ の負の有理数整数を表し、$-\mathbf{N}$ は $m \in \mathbf{N}$ の元 $-m$ の集合を表します。それから

$$
\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N}) \quad \text{and} \quad \mathbf{N} \cap (-\mathbf{N}) = \{0\}.
$$

$m \in \mathbf{N}$、$m = -m$ は、$m = 0$ の場合にのみ。

$m$ と $n$ を 2 つの自然数とします。

(a) $m \geq n$ の場合、$m + (-n) = p$、ここで、$p$ は $m = n + p$ となるような $\mathbf{N}$ の元です。
(b) $m \leq n$ の場合、$m + (-n) = -p$、ここで、$p$ は $m + p = n$ となる $\mathbf{N}$ の元です。
(c) $(-m) + (-n) = -(m + n)$。

プロパティ (b) と (c) は、no. 3、命題 4 から導き出されます。 $\mathbf{N}$ の $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$、加法とプロパティ (a)、(b)、(c) は $\mathbf{Z}$ の加法を完全に記述します。

より一般的には、$-x$ は、任意の有理数整数 $x$ の負を表すために使用されます。 合成 $x + (-y)$ は $x - y$ (cf. no. 8) と省略されます。

自然数の間の位数関係 $\leq$ は、次の性質によって特徴付けられます。 $m \leq n$ 整数 $p \in \mathbf{N}$ が存在する場合に限り、$m + p = n$ (*集合理論*, III, § 3, no. 6、命題 13 および § 5, no. 2、命題 2)。有理数整数 $x$ と $y$ の間の関係 $y - x \in \mathbf{N}$ は、$\mathbf{Z}$ の *合計位数* 関係と、拡大する位数関係 $\leq$ です。 $\mathbf{N}$。すべての $x \in \mathbf{Z}$、$x - x = 0 \in \mathbf{N}$ のために。 $y - x \in \mathbf{N}$ と $z - y \in \mathbf{N}$ の場合、

$$
z - x = (z - y) + (y - x) \in \mathbf{N},
$$

$\mathbf{N}$ は加法で安定しています。 $y - x \in \mathbf{N}$ と $x - y \in \mathbf{N}$ の場合、$y - x = 0$、0 は $\mathbf{N}$ の元のみで、$\mathbf{N}$ に対してマイナスの属するになります。任意の有理数整数 $x$ および $y$、$y - x \in \mathbf{N}$ または $x - y \in \mathbf{N}$ の場合、$\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$ の場合。最後に、$x$ と $y$ が自然数である場合、$x + p = y$ となる$p \in \mathbf{N}$ が存在する場合に限り、$y - x \in \mathbf{N}$ になります。この位数関係は $\leq$ とも表されます。

今後、$\mathbf{Z}$ が順序付けられた集合とみなされる場合、それは常に 〜でない限りになります。別の方法で定義した順序では、自然数は整数 $\geq 0$ と識別されます。それらは*ポジティブ* 整数とも呼ばれます。 整数 $\leq 0$、正の整数のマイナスは *マイナス* 整数と呼ばれます。 整数 $> 0$ (それぞれ $< 0$) は *厳密に正* (それぞれ *厳密に負*) と呼ばれます。 整数 $> 0$ の集合はときどきであり、$\mathbf{N}^*$ で表されます。

$x$、$y$、$z$ を 3 有理数整数とします。 x + z \leq y + z の場合に限り、$x \leq y$ となります。 x - y = (x + z) - (y + z) の場合。この性質は、$\mathbf{Z}$上の位数関係が翻訳下で不変であるというというによって表されます。

### 6. アプリケーション: II。合理的整数の乗法

#### 補題 2 {#alg-i-s2-lem-2 .statement tag=057B}

E をモノイドとし、E の x 元とします。
    (i) すべての $n \in \mathbf{N}$ に対して、$f(1) = x$ と $f(n) = \frac{n}{1} x$ を含む E に $\mathbf{N}$ の一意な準同型 f が存在します。
    (ii) x が可逆である場合、$\mathbf{N}$ に f を伴う $g(1) = x$ と g 一致するとなるように、E に $\mathbf{Z}$ の一意な準同型 g が存在します。

    すべての $n \in \mathbf{N}$ に対して $f(n) = \frac{n}{1} x$ を書く、数式
    $$
    \frac{0}{1} x = e \quad \text{and} \quad \left( \frac{m}{1} x \right) \cdot \left( \frac{n}{1} x \right) = \frac{m+n}{1} x
    $$
    (no. 1) f が $\mathbf{N}$ の準同型であることを E に表現すると、明らかに $f(1) = x$ になります。 $f'$ が $f'(1) = x$ となるような E への $\mathbf{N}$ の準同型である場合、§ 1, no. 4、命題 1 により、$f = f'$ になります (iv)。

ここで、x が可逆であると仮定します。 no. 3、系 2 から命題 4 まで、$f(n) = \frac{n}{1} x$ は整数 $n \geq 0$ ごとに反転可能です。 構成により、$\mathbf{Z}$ は $\mathbf{N}$ の差の群となり、したがって (no. 4, 定理 1) f 拡大するは $\mathbf{Z}$ の準同型 g に一意に E になります。 $g'$が$\mathbf{Z}$の準同型を$g'(1) = x$でEにすると、制限$f'$の$g'$から$\mathbf{N}$は、$\mathbf{N}$の準同型を$f'(1) = x$でEにします。 したがって、$f' = f$、よって $g' = g$ となります。

モノイド E が $\mathbf{Z}$ の場合に補題 2 を適用します。したがって、整数 $m \in \mathbf{Z}$ ごとに、$f_m(1) = m$ によって特徴付けられる $\mathbf{Z}$ の自己準同型 $f_m$ が存在します。 m が $\mathbf{N}$ にある場合、$\mathbf{N}$ の $\mathbf{N}$ に入る写像 $n \mapsto mn$ は、マグマ $\mathbf{N}$ の自己準同型 (集合理論, III, § 3, no. 3, 系まで) 命題 5);したがって、$\mathbf{N}$ のすべての $m, n$ は $f_m(n) = mn$ になります。

したがって、$\mathbf{N}$ の乗法は、$\mathbf{Z}$ の $m, n$ に対して公式 $mn = f_m(n)$ によって、$\mathbf{Z}$ の乗法に拡張できます。次の式を確立します。

(2) $$ xy = yx $$
    (3) $$ (xy)z = x(yz) $$
    (4) $$ x(y+z) = xy + xz $$
    (5) $$ (x+y)z = xz + yz $$
    (6) $$ 0.x = x.0 = 0 $$
    (7) $$ 1.x = x.1 = x $$
    (8) $$ (-1).x = x.(-1) = -x $$

$\mathbf{Z}$の$x, y, z$用。 (*他の語では、$\mathbf{Z}$は可換環です。*) 式$x(y+z) = xy + xz$と$x.0 = 0$は、$f_x$が加法モノイド$\mathbf{Z}$の自己準同型であり、$f_x(1) = x$が$x.1 = x$と書けるという事実を表しています。 自己準同型 $f_x \circ f_y$ of $\mathbf{Z}$ 写像 1 から $xy$ なので、$f_{xy}$、よって (3) と等しくなります。今$f_x(-y) = -f_x(y)$、つまり$x(-y) = -xy$です。同様に、$\mathbf{Z}$ 写像 1 から $-x$、よって $(-x).y = -xy$ の自己準同型 $y \mapsto -xy$ なので、
$$
(-x)(-y) = -(x(-y)) = -(-xy) = xy.
$$
$\mathbf{N}$の$m, n$、$mn = nm$ (集合理論、III, § 3, no. 3、系 ～ 命題 5)、よって $(-m).n = n(-m)$、$(-m)(-n) = (-n)(-m)$。 $\mathbf{Z}$の$x, y$の$\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$、$xy = yx$として。そして、この公式は、(5)が(4)から続き、公式(6)から(8)の証明が完成することを意味します。

### 7. アプリケーション: III。一般化冪

E を単位元 $e$ と合成の法則を $\top$ で表すモノイドとする。 $x$ が E で可逆である場合、$g_x$ は $\mathbf{Z}$ の準同型を E 写像 1 ～ $x$ とします。すべての $n \in \mathbf{Z}$ を $g_x(n) = \frac{n}{\top} x$ とします。 by 補題 2 この記法は、以前に紹介した記法と $n \in \mathbf{N}$ と互換性があります。それから
$$
\begin{align*}
\text{(9)} \quad & \frac{m+n}{\top} x = \left( \frac{m}{\top} x \right) \top \left( \frac{n}{\top} x \right) \\
\text{(10)} \quad & \frac{0}{\top} x = e \\
\text{(11)} \quad & \frac{1}{\top} x = x
\end{align*}
$$
E の $x$ および $\mathbf{Z}$ の $m, n$ の場合。さらに、$\mathbf{Z}$の$y = \frac{m}{\top} x$, 写像 $n \mapsto g_x(mn)$をEに入れると、準同型写像 1から$y$, よって $g_x(mn) = g_y(n)$ となります。
$$
\text{(12)} \quad \frac{mn}{\top} x = \frac{n}{\top} \left( \frac{m}{\top} x \right).
$$
$-1$は$\mathbf{Z}$の1のマイナスであるため、$\frac{-1}{\top} x$はEの$x = \frac{1}{\top} x$の逆数です。(9)で$n = -m$と書くと、$\frac{-m}{\top} x$は$\frac{m}{\top} x$の逆数であることがわかります。

### 8. 記法

(a) 原則として、可換モノイドの法則は加法的に書かれます。したがって、$-x$ は $x$ の負の数を表すという規則になります。 記法 $x + (-y)$ は $x - y$ と省略され、同様に
$$
x + y - z, \quad x - y - z, \quad x - y + z - t, \quad \text{etc. . . .}
$$
それぞれを表す
$$
x + y + (-z), \quad x + (-y) + (-z), \quad x + (-y) + z + (-t), \quad \text{etc. . . .}
$$

$n \in \mathbf{Z}$ 記法の場合、$\overset{n}{\top} x$ は $nx$ に置き換えられます。式 (9) ～ (12) は次のようになります。

(13) $$
(m + n).x = m.x + n.x
$$
(14) $$
0.x = 0
$$
(15) $$
1.x = x
$$
(16) $$
m.(n.x) = (mn).x
$$

ここで、$m$ と $n$ 属するは $\mathbf{N}$ に、あるいは $x$ が陰性を認めた場合には $\mathbf{Z}$ にもなります。後者の場合も関係 $(-1).x = -x$ が成り立ちます。 公式にも注意してください

(17) $$
n.(x + y) = n.x + n.y.
$$

(b) E を乗法的に書かれたモノイドとする。 $n \in \mathbf{Z}$ 記法の場合、$\overset{n}{\top} x$ は $x^n$ に置き換えられます。 関係があります

$$
x^{m+n} = x^m.x^n \\
x^0 = 1 \\
x^1 = x \\
(x^m)^n = x^{mn}
$$

また、$x$ と $y$ が通勤する場合は $(xy)^n = x^ny^n$ となります。

$x$ に逆数がある場合、これは正確に $x^{-1}$ になります。 $x^{-1}$ の代わりに記法 $\frac{1}{x}$ も使用されます。最後に、モノイド E が可換である場合、$\frac{x}{y}$ または $x/y$ は $xy^{-1}$ にも使用されます。

### 練習問題 {#alg-i-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
