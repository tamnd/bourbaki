---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 5
section_title: Groups operating on a set
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 52-65, 140-147
pdf_pages: 0076-0089, 0164-0171
extraction: ocr
subsections:
    - "no": 1
      title: MONOID OPERATING ON A SET
      page: 52
      pdf_page: 76
    - "no": 2
      title: STABILIZER, FIXER
      page: 54
      pdf_page: 78
    - "no": 3
      title: INNER AUTOMORPHISMS
      page: 55
      pdf_page: 79
    - "no": 4
      title: ORBITS
      page: 56
      pdf_page: 80
    - "no": 5
      title: HOMOGENEOUS SETS
      page: 58
      pdf_page: 82
    - "no": 6
      title: HOMOGENEOUS PRINCIPAL SETS
      page: 60
      pdf_page: 84
    - "no": 7
      title: PERMUTATION GROUPS OF A FINITE SET
      page: 61
      pdf_page: 85
statements: 32
exercises: 29
content_sha256: 89e9ab5a36e7d9760c9aaf3512b7d4ea74125046a8e316803aac2e69c88759dd
translated_from: content/en/alg/I/05_s5_groups_operating_on_a_set.md
translation_method: google
source_content_sha256: dfbb9d78abb1e74cb8df10a3c8d7099cfe102e2e7a75bb6d300412ab223621fa
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 88eda7f312f7384fb18d286b035bc7260a58c03d2799f150f1253531556160a5
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 5。 群集合で稼働中

### 1. 集合で動作するモノイド

#### 定義 1 {#alg-i-s5-def-1 .statement tag=05B1}

M をモノイドとし、法則を乗法で表し、単位元を e で表し、E 集合とします。すべての $\alpha, \beta \in M$ について $f_e = \mathrm{Id}_E$ と $f_{\alpha \beta} = f_\alpha \circ f_\beta$ (それぞれ $f_{\alpha \beta} = f_\beta \circ f_\alpha$) の場合、M on E の作用 $\alpha \mapsto f_\alpha$ は、M on E の左 (または右) 演算と呼ばれます。

他の語では、集合 E 上のモノイド M の左 (それぞれ右) 演算は、写像の合成を持つモノイド $E^E$ (それぞれ$E^E$ の反対のモノイド) への M のモノイド準同型です。 M の作用対応するから作用の法則を左 (それぞれ右) 乗法とすると、この作用が左 (それぞれ右) 演算であるという事実は、次の式で表すことができます。

(1)
$$
e.x = x; \quad \alpha.(\beta.x) = (\alpha \beta).x \quad \text{for } \alpha, \beta \in M \text{ and } x \in E.
$$
(それぞれ $x.e = x; \quad (x.\alpha).\beta = x.(\alpha \beta) \quad \text{for } \alpha, \beta \in M \text{ and } x \in E$)。

これらの条件の下では、M は左側 (右側) の E 上で作用し、作用の対応する法則は E 上のモノイド M の左側 (右側) の法則演算であると言われます。

M をモノイドとします。 集合 E と E 上の M の左 (右) 演算は、左 (右) M セットと呼ばれます。モノイド M は、M の $E^E$ への写像 $\alpha \mapsto f_\alpha$ が単射である場合、左 (それぞれ右) で忠実に動作すると言われます。

#### 例 {#alg-i-s5-n1-exa-1 .statement tag=05B2}

(1) E を集合とします。 E 上の $E^E$ の標準作用 (§ 3, no. 1、例 3) は左の演算です。

(2) M をモノイドとする。 M (§ 3, no. 3、例 7) 上の法則から派生した M 自体の左 (それぞれ右) 作用は、それ自体の M の左 (それぞれ右) 演算です。この演算を考慮すると、M は左 (または右) 変換によってそれ自体に作用すると言えます。

E を左 (または右) M セット、$M^0$ を M の反対のモノイドとします。同じ作用の下で、モノイド $M^0$ は右 (または左) の E に作用します。得られた$M^0$-セットはM-セットEの反対と呼ばれます。定義、左のM-セットに関連する結果は、移行の反対側の構造のときに右の$M^0$-セットに引き継がれます。

この段落の残りの部分では、〜でない限り特に明記されていない限り、残った M セットのみを考慮します。これを単に M セットと呼びます。 作用の法則は左の乗法で示されます。

Eを集合とします。 G を E 上で演算する群とします。 G のすべての $\alpha$ について、$\alpha$ によって定義される $E^E$ の元は E の置換 ($\S$ 2、no. 3、例 2) です。 したがって、E に G の演算が与えられることは、G の $\mathfrak{S}_E$ に G の準同型が与えられることになります。

$\S$ 3、no. 3 に準拠して、次の定義を作成します。

#### 定義 2 {#alg-i-s5-def-2 .statement tag=05B3}

*M をモノイド、E と E' の M 集合とする。 E の写像 f を E' に変換すると、すべての $x \in E$ とすべての $\alpha \in M$ に対して、$f(\alpha.x) = \alpha.f(x)$ は M 集合準同型 (または M 射、または M の演算と互換性のある写像) と呼ばれます。

M 集合の恒等写像は M 射です。 2 つの M 射の合成は M 射です。 他のへの 1 つの M 集合の写像が同型になるためには、それが全単射 M 射であり、その逆の写像が M 射であることが必要かつ十分です。

$(E_i)_{i \in I}$ を M 集合の族とし、E を $E_i$ の積集合とします。モノイド M は E に対して $\alpha.(x_i)_{i \in I} = (\alpha.x_i)_{i \in I}$ によって作用し、E はこの作用とともに M 集合になります。 E'をMセットとする。 E' から E への写像 f は、$pr_i \circ f$ がすべての $i \in I$ に対して E' から $E_i$ への M 射である場合に限り、M 射となります。

E を M セット、F を M の作用の下で E の安定な部分集合とする。誘導された法則では、F は M 集合であり、標準単射 $F \to E$ は M 射です。

E を M 集合とし、E 上の R 同値関係が M の作用と互換性があるとします。 商 $E/R$ と商作用は M 集合であり、標準写像 $E \to E/R$ は M 射です。

$\phi : M \to M'$ をモノイド準同型、E を M 集合、E' を $M'$ 集合とする。 写像 E の f を E' にすると、すべての $x \in E$ と $\alpha \in M$ について、

$$
f(\alpha.x) = \phi(\alpha).f(x)
$$

は E から E' への $\phi$-射 (cf. $\S$ 3, no. 1) と呼ばれます。

*拡大、法則、演算.* (たとえば) 3 つの集合 $F_1, F_2, F_3$、置換 $f_1, f_2, f_3$ $F_1, F_2, F_3$ と、基底集合 $F_1, F_2, F_3$ の階層 F が与えられたとします。 (*集合理論*、IV、$\S$ 1、no. 1)、定義する、段階 F の構成、F の *標準拡大* と呼ばれる F の置換を段階的に進めることができます。 $f_1, f_2, f_3$ から F (*集合理論*、IV、$\S$ 1、no. 2);それを$\phi_F(f_1, f_2, f_3)$で表すことにします。

次に、G を $F_i$ ($i = 1, 2, 3$) の対称群に、G の群と $h_i$ 準同型を、$F_i$ 上の G の他の語演算にします。 写像 $x \mapsto x_F = \phi_F(h_1(x), h_2(x), h_3(x))$ は、G の $\mathfrak{S}_F$ への G の準同型であり、F 上の G の他の語演算であり、F に対する $h_1, h_2, h_3$ の *拡大* と呼ばれます。 P を F の部分集合とし、すべての $x \in G$ について、 $x_F(P) = P$; $x_P$ を $x_F$ の制限にします

P;その場合、写像 $x \mapsto x_P$ は P 上の G の演算であり、P に対する $h_1, h_2, h_3$ の拡大とも呼ばれます。

たとえば、K と L を $F_1, F_2, F_3$ の 2 つの階層とします。 F を $K \times L$ の部分集合の集合とし、P を K の写像の集合としてL にし、グラフで識別します。 $w \in P$ と $x \in G$ の場合、$x_P(w)$ は K の写像 $k \mapsto x_L(w(x_K^{-1}(k)))$ から L になります。

### 2. 固定群、フィクサー

#### 定義 3 {#alg-i-s5-def-3 .statement tag=05B4}

*M を、集合 E、A、および E の B 部分集合で動作するモノイドとする。$\alpha \in M$ の集合で、$\alpha A \subset B$ (それぞれ $\alpha A = B$) を A から B へのトランスポーター (それぞれ厳密トランスポーター) と呼びます。A から A へのトランスポーター (それぞれ厳密トランスポーター) を固定群と呼びます。 (それぞれ厳密な固定群)。すべての $a \in A$ に対する $\alpha a = a$ が A のフィクサーと呼ばれるような、$\alpha \in M$ の集合 。

M の元 $\alpha$ は安定するといわれます (それぞれ厳密に安定、それぞれ固定) 部分集合 E の A が $\alpha$ 属するから固定群の場合 (それぞれ厳密固定群、それぞれ固定) 部分集合 M の P は安定すると言われます (それぞれ厳密に安定、固定、 P のすべての元が安定する場合、E の部分集合 A (それぞれ厳密に安定、それぞれ固定) A. A の固定子は、A の厳密な固定群に含まれており、それ自体は A の固定群に含まれています。

#### 命題 1 {#alg-i-s5-prop-1 .statement tag=05B5}

*M を集合 E と E の A 部分集合上で動作するモノイドとします。*
(a) *固定群、厳格な固定群、および A のフィクサーは M の部分モノイドです。
(b) *$\alpha$をMの可逆元とする。 A の厳密な固定群 (それぞれフィクサー) に対して $\alpha$ 属するの場合、$\alpha^{-1}$ も同様です。*

e を M の単位元とします。次に、元 $a \in A$ ごとに $ea = a$ となり、したがって A の固定子に e 属するが与えられます。 $\alpha$ と $\beta$ を A を安定させる E の元とします。そのとき、$(\alpha \beta)A = \alpha(\beta A) \subset \alpha A \subset A$ なので A の固定群は M の部分モノイドになります。厳格な固定群と A のフィクサー、よって (a) の場合。 $\alpha A = A$の場合は、$A = \alpha^{-1}(\alpha A) = \alpha^{-1}A$。すべて $a \in A$、$\alpha a = a$ の場合、$a = \alpha^{-1}(\alpha a) = \alpha^{-1}a$、よって (b)。

#### 系 {#alg-i-s5-n2-cor-1 .statement tag=05B6}

*G を集合 E 上で動作する群とし、A を E の部分集合とします。A の厳密な固定群 S と固定子 F は G の部分群であり、F は S の通常の部分群です。*

最初の主張は命題から続き、F は S の準同型の核で、A 上の S の演算に関連付けられた $\mathfrak{S}_A$ になります。

群 G は、E の固定子が G の単位元で構成されている場合に限り、集合 E に対して忠実に動作します。E の固定子は、指定された G の準同型の $\mathfrak{S}_E$ への核です。この準同型は、その核が単位元 (§ 4, no. 5, 定理 3) で構成されている場合にのみ単射的です。

M をモノイド、E を M 集合、E の $a$ 元とします。フィクサー、厳密な固定群と $\{a\}$ の固定群は等しいです。このモノイドは、フィクサーまたは $a$ の固定群と同様に呼ばれます。 E の部分集合 A の固定子は、A の元の固定子のうちの共通部分です。 $a$ の固定子がモノイド M である場合、$a$ は E の不変量元と呼ばれます。 E のすべての元が不変であれば、M は E 上で自明に動作するといわれます。

#### 命題 2 {#alg-i-s5-prop-2 .statement tag=05B7}

*G を集合 E 上で動作する群とし、すべての $x \in E$ について、$S_x$ を x の固定群とします。すべての$\alpha \in G$、$S_{\alpha x} = \alpha S_x \alpha^{-1}$.*

$s \in S_x$ の場合、$\alpha s \alpha^{-1}(\alpha x) = \alpha s x = \alpha x$、よって $\alpha S_x \alpha^{-1} \subset S_{\alpha x}$。 $x = \alpha^{-1}(\alpha x)$、$\alpha^{-1} S_{\alpha x} \alpha \subset S_x$、よって $S_{\alpha x} \subset \alpha S_x \alpha^{-1}$ として。

同様に、A と B が E の 2 つの部分集合で、T が A から B へのトランスポーター (それぞれ厳密なトランスポーター) である場合、$\alpha A$ から $\alpha B$ のトランスポーター (それぞれ厳密なトランスポーター) は $\alpha T \alpha^{-1}$ に等しいことがわかります。

### 3. 内部自己同型

G を群とします。 群 G の自己同型の集合 Aut(G) は、$\mathscr{G}_G$ の部分群 (§ 4, no. 1、例 2) です。

#### 命題 3 {#alg-i-s5-prop-3 .statement tag=05B8}

※Gを群とします。 G のすべての元 x について、写像 Int(x): それ自体への G の $y \mapsto xyx^{-1}$ は G の自己同型です。 写像 Int: Aut(G) への G の $x \mapsto \operatorname{Int}(x)$ は群準同型で、その核は G の中心であり、その像はAut(G)の通常の部分群です*。

$x, y$ と $z$ が G の元である場合、$(xyx^{-1})(xz x^{-1}) = xyz x^{-1}$、したがって Int(x) は G の自己準同型になります。 G の $x$ と $y$ 元の場合、

$$
\operatorname{Int}(x) \circ \operatorname{Int}(y) = \operatorname{Int}(xy):
$$

すべての$z \in G$、$x(yzy^{-1})x^{-1} = (xy)z(xy)^{-1}$。一方、$\operatorname{Int}(e)$ は G の恒等写像です。 したがって、写像 Int は G から群 G の自己準同型のモノイド End(G) までのモノイド準同型です。 G の元は可逆であるため、写像 Int はその集合 Aut(G) の可逆元の End(G) (§ 2, no. 3) の値。ここで、$x$ と $y$ が通勤している場合に限り、$xyx^{-1} = y$ は、$x$ が中央の元である場合に限り、$\operatorname{Int}(x)$ は G の恒等写像になります。最後に、$\alpha$ を G の自己同型とし、$x \in G$ とします。それから

$$
\operatorname{Int}(\alpha(x)) = \alpha \circ \operatorname{Int}(x) \circ \alpha^{-1}.
$$

$y \in G$の場合、

$$
\alpha(x) \cdot y \cdot \alpha(x)^{-1} = \alpha(x) \cdot \alpha(\alpha^{-1}(y)) \cdot \alpha(x)^{-1} = \alpha(x \cdot \alpha^{-1}(y) \cdot x^{-1}).
$$

したがって、$\alpha \cdot \operatorname{Int}(G) \cdot \alpha^{-1} \subset \operatorname{Int}(G)$です。

#### 定義 4 {#alg-i-s5-def-4 .statement tag=05B9}

※Gを群と$x \in G$とする。 自己同型 $y \mapsto xyx^{-1}$ は、x で定義される G の内部自己同型と呼ばれ、$\operatorname{Int} x$ で表されます。*

$x, y \in G$ の場合は、$x^y = y^{-1}xy = (\operatorname{Int} y^{-1})(x)$ とも書きます。

G の部分群は、G のすべての内部自己同型 (§ 4, no. 4、定義 5) の下で安定している場合に限り、正常です。 G の部分群が G のすべての自己同型の下で安定している場合、特性と呼ばれます。 群 G の中心は特性部分群 (公式 (2)) です。

群 G の中心は、G のすべての自己準同型 (練習問題 22) の下で必ずしも安定しているとは限りません。特に、演算子を使用した群の中心は必ずしも安定した部分群とは限りません。

#### 命題 4 {#alg-i-s5-prop-4 .statement tag=05BA}

G を群、H を G の特性 (それぞれ正規) 部分群、K を H の特性部分群とします。すると、K は G の特性 (それぞれ正規) 部分群となります。

G の自己同型 (それぞれ内部自己同型) の H に対する制限は H の自己同型であるため、K は不変のままになります。

G を群、A $\subset$ G、および $b \in G$ とします。 b は、$bAb^{-1} = A$ の場合に A を正規化すると言われます。すべて $a \in A$, $bab^{-1} = a$ の場合、b は A を集中化すると言われます。 A と B を G の部分集合とします。 B のすべての元が A を正規化 (または集中化) する場合、B は A を正規化 (または集中化) していると言われます。

The set of $g \in G$ which normalize (resp. centralize) A is called the normalizer (resp. centralizer) of A (cf. § 1, no. 5, Definition 9); it is often denoted by $N_G(A)$ or simply $N(A)$ (resp. $C_G(A)$ or $C(A)$). Gの部分群です。 A が G の部分群であるとき、$N_G(A)$ は、A が含む A であり、A が正常である G の最大の部分群として特徴付けることができます。

#### 注意 {#alg-i-s5-n3-rem-1 .statement tag=05BB}

(1) G がそれ自体に対して内部自己同型によって作用するとき、A のノーマライザー (またはセントラライザー) は A の厳密な固定群 (それぞれフィクサー) です。特にセントラライザーはノーマライザーの通常の部分群です。

(2) $bAb^{-1} \subset A$ が G の部分モノイドとなるような元 $b \in G$ の集合 。A が G の部分群である場合でも、この集合は必ずしも G の部分群であるとは限りません (練習問題 27)。

### 4. 軌道

#### 定義 5 {#alg-i-s5-def-5 .statement tag=05BC}

G を群、E を G セット、$x \in G$ とします。 $y = \alpha x$となるような元$\alpha \in G$が存在する場合、元$y \in E$はGの演算の下のxに共役になります。 x の共役元の集合は、E では x の軌道と呼ばれます。

関係「yはxに対して共役」は同値関係です。 $x = ex$の場合; $y = \alpha x$ の場合は $x = \alpha^{-1} y$; $y = \alpha x$ と $z = \beta y$ の場合、$z = \beta \alpha x$。 軌道はこの関係の下に同値類があります。

E の部分集合 X は、共役の関係に関して飽和している場合にのみ安定します。

The mapping $\alpha \mapsto \alpha x$ of G into E is sometimes called the orbital mapping defined by x. これは G の E への G 射です (左変換により G の演算が付加されます)。 この写像の下にあるGの像$G . x$はxの軌道です。

すべての $x \in E$ について、x によって定義される軌道写像が単射である場合、または $G \times E$ から $E \times E$ への写像 $(g, x) \mapsto (gx, x)$ が単射である場合、G は E 上で自由に動作するといわれます。

#### 例 {#alg-i-s5-n4-exa-1 .statement tag=05BD}

(1) G を群とし、G の演算を内部自己同型で考える。この演算の下の共役にあるGの2つの元は、内部自己同型の下の共役、または単に共役と呼ばれます。 軌道は共役類と呼ばれます。同様に、G の 2 つの部分集合 H と H' は、$H' = \alpha . H . \alpha^{-1}$ のような元 $\alpha \in G$ が存在する場合、つまり、それ自体が G の拡大から演算の $\mathscr{P}(G)$ の下にある共役である場合、共役と呼ばれます。 内部自己同型。

(2) ※空間$\mathbf{R}^n$において、点の軌道×直交群$\mathbf{O}(n, \mathbf{R})$の作用の下は、半径$\|x\|_*$のユークリッド球です。

E の 2 つの共役元のうち固定群は、G の共役部分群 (no. 2、命題 2) です。

活用の関係の下での E の商集合は、E の軌道の集合です。それは、E/G または G\|E で示されるときどきです。 (ときどき記法 E/G は E が右 G セットの場合に予約され、記法 G\|E は E が左 G セットの場合に予約されます。)

G を、右側の集合 E に作用する群とします。 H を G の正規の部分群とします。 群 G は右側の E/H で動作し、右作用の対応する法則は $(xH, g) \mapsto xHg = xgH$ です。この演算の下では、H は自明に動作し、よって E/H 上の G/H の権利演算になります。 $\phi$ を E/H から E/G への標準写像とします。 E/Gの点の$\phi$の下の逆像は、E/HのG（またはG/H）の軌道です。 したがって、E/G 上の $(E/H)/G = (E/H)/(G/H)$ の移行から商全単射が正準と呼ばれるとき、$\phi$ 定義するになります。

G (それぞれ H) を、左側 (それぞれ右側) の集合 E に作用する群とします。 G と H の作用が E に通勤しているとします。

$$
(g.x).h = g.(x.h) \quad \text{for } g \in G, x \in E \text{ and } h \in H.
$$

E 上の H の作用は、H の反対側の群 $H^0$ の左演算です。その後、§ 4, no. 9、命題 12 から写像が続き、元 $(g, h) \in G \times H^0$ 写像と関連付けられます。 E の$x \mapsto g . x . h$ は、E 上の$G \times H^0$ の左演算です。この演算の下の元 $x \in E$ の軌道は、集合 $GxH$ です。この軌道のうち集合は $G\|E/H$ で表されます。一方、G (それぞれ H) の演算は、H (それぞれ G) の演算に対する共役の関係と互換性があり、軌道 $G\|(E/H)$ (それぞれ $(G\|E)/H$) の集合は $G\|E/H$ と同一視されます。 図式

$$
\begin{array}{ccc}
& & E \\
& \swarrow_{\alpha} & \searrow_{\beta} \\
G\|E & & E/H \\
& \downarrow_{\varepsilon} & \\
& & G\|E/H \\
& \searrow_{\delta} & \swarrow_{\gamma}
\end{array}
$$

($\alpha, \beta, \gamma, \delta, \varepsilon$ は商を取ることの標準写像を表します)、$\gamma \circ \alpha = \delta \circ \beta = \varepsilon$。

G を G の群、H 部分群とします。G 上の H の右側演算を右変換 (no. 1, 例 2) で考えます。 軌道 $G/H$ の集合は、H を法とする左剰余類の集合です。 G は、左側の $G/H$ に対して法則 $(g, xH) \mapsto gxH$ (cf. no. 5) によって演算されることに注意してください。同様に、H を法とする右剰余類の集合は、左変換により G 上の H の左演算の軌道の集合 $H\backslash G$ になります。 K が G 含む H の部分群で、$\Gamma$ が H を法とする左 (または右) 剰余類である場合、$\Gamma K$ (それぞれ $K\Gamma$) は K を法とする左 (または右) 剰余類です。 写像 $\Gamma \mapsto \Gamma K$ (それぞれ $\Gamma \mapsto K\Gamma$) $G/H$の$G/K$の標準写像（それぞれ$H\backslash G$の$K\backslash G$）と呼ばれます。それは客観的です。

G を群とし、H と K を G の 2 つの部分群とします。H が左の移動によって左側の G に作用し、右の移動によって右側の K に作用するとします。これら 2 つの演算通勤により、集合 $H\backslash G/K$ を考慮することができます。 $H\backslash G/K$の元は、HとKを法とするGの二重剰余類と呼ばれます。$K = H$の場合、単にHを法とする二重剰余類と呼ばれます。$G/H$の$H\backslash G/H$上の標準写像が全単射となるためには、HがGの正規の部分群であることが必要かつ十分です。

### 5. 均質集合

#### 定義 6 {#alg-i-s5-def-6 .statement tag=05BE}

※Gを群とします。 集合 E 上の G の演算は、軌道が E である元 $x \in E$ が存在する場合、推移的と呼ばれます。E 上の G の演算が推移的である場合、G 集合 E は同次と呼ばれます。*

G は E に対して *推移的に動作*するとも言われます。または、E は G のもとで *同種の集合であるということ。E は *空ではない*、そして E のすべての元 $x$ と $y$ に対して、$\alpha.x = y$ となるような元 $\alpha \in G$ が存在する、ということは同じことになります。

#### 例 {#alg-i-s5-n5-exa-1 .statement tag=05BF}

E が G 集合である場合、E の各軌道は、誘導された演算とともに、G の下で同次の集合になります。

G を G の群および H 部分群とします。H を法とする左剰余類の集合 $G/H$ を考えます。 群 G は、左の $G/H$ に $(g, xH) \mapsto gxH$ を掛けて演算します。 N を H のノーマライザーとします。群 N は、$(xH, n) \mapsto xHn = xnH$ によって右側の $G/H$ に作用します。 H 上のこの演算誘導するは自明な演算であるため、移行から商では、$N/H$ は右側の $G/H$ に作用します。 $\phi : (N/H)^0 \to S_{G/H}$を準同型対応するからこの演算とします。

#### 命題 5 {#alg-i-s5-prop-5 .statement tag=05BG}

※上記記法により、G/Hは同次Gセットとなります。 写像 $\phi$ 誘導する $(N/H)^0$ の同型を G セット G/H の自己同型の群に追加します。*

元 $e = H$ の $G/H$ の軌道は $G/H$、 よっては最初の主張です。ここで 2 番目を証明します。 $G/H$ で恒等写像を右変換すると $n \in N$ 定義するであれば、$e.n = e$、つまり $H.n = H$、よって $n \in H$ となります。したがって

N/H は右側の G/H に忠実に作用し、$\phi$ は単射的です。 G/H 上の G の左演算と N/H の右演算は可換であり、したがって G/H のそれ自体への N/H 定義する G 射の演算子は全単射であるため必然的に G 自己同型となります。したがって、$\phi$ は、G/H の G 自己同型の群 $\Phi$ でその値をとります。 $\phi$の像は$\Phi$であることがわかります。 $f \in \Phi$ にしましょう。 構造を移送すると、G の $f(\dot{e})$ の固定群は $\dot{e}$ の固定群に等しく、したがって H に等しくなります。 $n \in G$ を $f(\dot{e}) = n\dot{e}$ となるようにします。 G の $n\dot{e}$ の固定群は、$nHn^{-1}$ (no. 2、命題 2)、よって $nHn^{-1} = H$、$n \in N$ です。 G/H のすべての元 $xH$、$f(xH) = f(x.\dot{e}) = x.f(\dot{e}) = xnH = xHn$ および $f$ 一致するについて、$n$ によって定義される写像 。

#### 注意 {#alg-i-s5-n5-rem-1 .statement tag=05BH}

(1) G を G の群、H 部分群、G/H 上の G の$\phi : G \to \mathscr{S}_{G/H}$ 準同型対応する ～ 演算とする。 $\phi$ の核は、H の共役の共通部分です (no. 2、命題 2)。 H(no. 3)に含まれる最大の通常の部分群でもあります。特に、G は、H 簡約するから $\{e\}$ の共役の共通部分の場合に限り、G/H で忠実に動作します。

(2) G を群、H および K 部分群とし、H が K の正規部分群となるようにします。すると、K/H は右側の G セット G/H に作用し、G/H の標準写像は移行から商の G セット同型上で G/K 定義するに作用します。 $(G/H)/(K/H) \to G/K$ (cf. no. 4)。

#### 命題 6 {#alg-i-s5-prop-6 .statement tag=05BI}

*G を群、E を同次 G 集合、$a \in E$、a の H 固定群、H に含まれる G の K 部分群とする。$f(e.K) = a$ となるような G/K の E への G 射 f はただ 1 つだけ存在します。 K = H の場合、f は同型です。*

f が解の場合、G のすべての x について $f(x.K) = x.a$、よって一意性;私たちは存在を示します。 a によって定義される軌道写像は、G 上の同値関係 $y \in xK$ と互換性があります。 というのは、$y = xk, k \in K$ の場合、
$$
y.a = xk.a = x.a.
$$
したがって、写像 f は G/K から、G のすべての x について $f(x.K) = x.a$ を満たす H に導出されます。 この写像はG射であり、$f(K) = a$です。 この写像は、その像が E の空ではない安定した部分集合であるため、全射的です。 ここで、K = H であると仮定し、f が単射であることを示しましょう。 $f(x.H) = f(y.H)$ の場合、$x.a = y.a$、よって $x^{-1}y.a = a$、$x^{-1}y \in H$、よって $x.H = y.H$。

#### 定理 1 {#alg-i-s5-thm-1 .statement tag=05BJ}

*G を群とします。*
(a) *すべての同次 G セットは、H が G の部分群である形 G/H の同次 G セットと同型です。*
(b) *H と H' を G の 2 つの部分群とします。G 集合 G/H と G/H' は、H と H' が共役である場合にのみ同型です。*

同次 G セットは空ではないため、主張 (a) は命題 6 から続きます。 (b)を示します。 $f : G/H \to G/H'$ を G セット同型とします。 部分群 H は H の固定群であるため、構造の輸送、$G/H'$ の元の固定群です。 したがって、部分群 $H$ と $H'$ は共役 (no. 2、命題 2) になります。 If $H' = \alpha H \alpha^{-1}$, $H'$ is the stabilizer of the element $\alpha . H$ of $G/H$ (no. 2, Proposition 2) and hence $G/H'$ is isomorphic to $G/H$ (Proposition 6).

#### 例 {#alg-i-s5-n5-exa-2 .statement tag=05BK}

(1) $E$ を空ではない集合とします。 群 $S_E$ は $E$ に対して推移的に動作します。 If $x$ and $y$ are two elements of $E$, the mapping $\tau : E \to E$ such that $\tau(x) = y$, $\tau(y) = x$ and $\tau(z) = z$ for $z \neq x, y$, is a permutation of $E$. $a \in E$ にしましょう。 $a$ の固定群は $S_F$ と識別されます ($F = E - \{a\}$)。 したがって、同次 $G$-集合 $E$ は $S_E / S_F$ と同型です。

(2) $E$ を $n$ 元の集合および $(p_i)_{i \in I}$ を $\sum_i p_i = n$ となるような整数 $> 0$ の有限族とする。 $X$ を分割の集合、$E$ の $(F_i)_{i \in I}$ とし、すべての $i$ に対して $\mathrm{Card}(F_i) = p_i$ とします。 群 $S_E$ は $X$ に対して推移的に動作します。 The stabilizer $H$ of an element $(F_i)_{i \in I}$ of $X$ is canonically isomorphic to $\prod_{i \in I} S_{F_i}$ and is hence of order $\prod_{i \in I} p_i!$. 適用定理 1 と § 4, no. 4、系から命題 4 により、新しい証明が得られます。

$$
\mathrm{Card}(X) = \frac{n!}{\prod_{i \in I} p_i!}
$$

特に、$I = \{1, 2, \ldots, r\}$、$E = \{1, 2, \ldots, n\}$、

$$
F_i = \{p_1 + \cdots + p_{i-1} + 1, \ldots, p_1 + \cdots + p_i\}
$$

$1 \leq i \leq r$の場合。 $S$ を $\tau \in S_E$ の集合とし、$\tau|_{F_i}$ が $1 \leq i \leq r$ に対して増加するとなるようにします。 $(G_1, \ldots, G_r) \in X$ の場合、写像 $(F_1, \ldots, F_r)$ から $(G_1, \ldots, G_r)$ までの $\tau \in S$ は 1 つだけ存在します。他の語では、$H$ を法とする $S_E$ の各左剰余類は 1 つだけの点で $S$ と一致します。

(3) ※$n$を整数$\geq 1$とします。直交群 $O(n, \mathbf{R})$ は、$\mathbf{R}^n$ の単位元球面 $S_{n-1}$ 上で推移的に作用します。 点 $(0, \ldots, 0, 1)$ の固定群は、直交する群 $O(n-1, \mathbf{R})$ と同一視されます。したがって、同次 $O(n, \mathbf{R})$-集合 $S_{n-1}$ は $O(n, \mathbf{R})/O(n-1, \mathbf{R})$ と同型です。*

### 6. 同種プリンシパル集合

#### 定義 7 {#alg-i-s5-def-7 .statement tag=05BL}

※$G$を群とします。 集合 $E$ 上の $G$ の演算は、$x$ によって定義される軌道写像が全単射となるような $E$ の元 $x$ が存在する場合、単に推移的と呼ばれます。 集合 $E$ は、$E$ 上の $G$ の単純推移左作用とともに、左同次主$G$ 集合 (または $G$ の下の左同次主集合) と呼ばれます。

$G$ が $E$ 上で自由かつ推移的に動作する、あるいは、$x$ によって定義される軌道写像が $G$ 集合 $G$ の同型となるような元 $x \in E$ が存在するということは、同じことになります（ここで、$G$左の移動によって動作します) $E$ へ。または、次の 2 つの条件が満たされることも意味します。

(i) $E$ は空ではありません。
(ii) $E$ のすべての元 $x$ と $y$ に対して、$\alpha x = y$ となる元 $\alpha \in G$ が 1 つだけ存在します。

条件 (ii) は、次の条件と同等です。

(iii) 写像 $(\alpha, x) \mapsto (\alpha x, x)$ は、$G \times E$ の $E \times E$ 上の全単射です。

適切な同次主 G セットを定義するタスクは読者に任せます。

#### 例 {#alg-i-s5-n6-exa-1 .statement tag=05BM}

(1) G 自体を左 (右) 変換によって操作します。したがって、左 (右) の同次主 G セット構造が G 上で定義され、これは $G_s$ (それぞれ $G_d$) で示されるときどきです。

(2) E を *可換* 群 G の下で同次集合とする。G が E に対して忠実に動作する場合、後者は同次主 G セットです。

(3) E と F を同じ種の構造と 2 つの同型集合とし、Isom(E, F) を F に対する E の同型の集合とします (与えられた構造を使用)。 E の自己同型の群 Aut(E) (指定された構造を使用) は、右側の Isom(E, F) に対して法則 $(\sigma, f) \mapsto f \circ \sigma$ だけ演算され、Isom(E, F) は右同次主 Aut(E) 集合です。同様に、群 Aut(F) は、左の Isom(E, F) に対して法則 $(\sigma, f) \mapsto \sigma \circ f$ によって演算され、Isom(E, F) は左の同次主 Aut(F) セットです。

(4) ベクトル空間の加法群の下にある *同次プリンシパル集合は *アフィン空間* (cf. II, § 9, no. 1)* と呼ばれます。

同次主 G セット $G_s$ (例 1) の自己同型の群は、$G^0$ (no. 5, 命題 5) で識別される G の右変換の群です。 E を同次主 G セットおよび E の $a$ 元とします。 $a$ によって定義される軌道写像 $\omega_a$ は、E 上の G セット $G_s$ の同型です。 構造同型を輸送することにより、 $\psi_a$ は $G^0$ から Aut(E) に導出されます。 $\psi_a$ *一般に a* に依存することに注意してください。より正確には、$\alpha \in G$ の場合、

$$
\psi_{\alpha a} = \psi_a \circ \operatorname{Int}_{G^0}(\alpha) = \psi_a \circ \operatorname{Int}(\alpha^{-1}).
$$

G に翻訳 $x \mapsto x \alpha$ の $\delta_a$ を書くと、

$$
\omega_{\alpha a} = \phi \omega_a \circ \delta_\alpha
$$
そして
$$
\psi_a(x) = \omega_a \circ \delta_x \circ \omega_a^{-1}, \quad x \in G,
$$
よって
$$
\psi_{\alpha a}(x) = \omega_a \circ \delta_\alpha \circ \delta_x \circ \delta_\alpha^{-1} \circ \omega_a^{-1} = \omega_a \circ \delta_{\alpha^{-1} x \alpha} \circ \omega_a^{-1} = \psi_a(\alpha^{-1} x \alpha).
$$

### 7. 有限の集合の置換群

E が $n$ 元を持つ有限集合である場合、対称群 $\mathfrak{S}_E$ (§ 4, no. 1) は位数 $n!$ の有限群です。 E が集合 $\mathbf{N}$ の自然数の区間 $\{1, n\}$ のとき、対応する対称群は $\mathfrak{S}_n$ で表されます。 $n$ 元と任意の集合の対称群は $\mathfrak{S}_n$ と同型です。

#### 定義 8 {#alg-i-s5-def-8 .statement tag=05BN}

E を、E の有限集合、$\zeta \in \mathfrak{S}_E$ 置換、および $\zeta$ によって生成された $\mathfrak{S}_E$ の $\bar{\zeta}$ 部分群とします。 E 上の $\bar{\zeta}$ の演算の下に、単一の元に還元されない唯一の軌道が存在する場合、$\zeta$ はサイクルと呼ばれます。この軌道を$\zeta$のサポートといいます。

$\zeta$ をサイクルとします。 $\zeta$ のサポート $\operatorname{supp}(\zeta)$ は $x \in E$ の集合であり、$\zeta(x) \neq x$ になります。

サイクル$\zeta$の位数は、そのサポートの基数に等しい。 $\zeta$ によって生成された部分群 $\bar{\zeta}$ は、$\operatorname{supp}(\zeta)$ で推移的かつ忠実に動作します。 $\zeta$ は可換であるため、$\operatorname{supp}(\zeta)$ は $\bar{\zeta}$ (no. 6、例 2) の下で主集合となり、したがって $\operatorname{Card}(\operatorname{supp}(\zeta)) = \operatorname{Card}(\bar{\zeta})$ になります。

#### 補題 1 {#alg-i-s5-lem-1 .statement tag=05BO}

$(\zeta_i)_{i \in I}$ を、サポートがペアごとに互いに素であるサイクルの族とします。したがって、$\zeta_i$ はペアごとに変更可能です。 $\sigma = \prod_{i \in I} \zeta_i$ と $\bar{\sigma}$ を $\sigma$ によって生成された部分群とします。次に、$x \in S_i, i \in I$の場合は$\sigma(x) = \zeta_i(x)$、$x \notin \bigcup_{i \in I} S_i$の場合は$\sigma(x) = x$です。 写像 $i \mapsto S_i$ は、単一の元のからなるではなく、$\bar{\sigma}$ 軌道の集合にある I の全単射です。

$\zeta$ と $\zeta'$ を 2 つのサイクルとし、そのサポートは互いに素です。もし
$$
x \notin \operatorname{supp}(\zeta) \cup \operatorname{supp}(\zeta'),
$$
次に$\zeta \zeta'(x) = \zeta' \zeta(x) = x$。 $\zeta$ のサポートに対して $x$ 属するの場合は、$\zeta'(x) = x$、$\zeta(x)$ 属するの場合、$\zeta$、よって $\zeta \zeta'(x) = \zeta' \zeta(x) = \zeta(x)$ のサポートになります。同様に、$x$ 属するから$\zeta'$ のサポートに、その後は$\zeta' \zeta(x) = \zeta \zeta'(x) = \zeta'(x)$ になります。したがって$\zeta \zeta' = \zeta' \zeta$です。したがって、$\zeta_i$ はペアごとに置換可能であり、$i \in I$ と $x \in S_i$ については、$\sigma(x) = \zeta_i(x) \in S_i$ になります。 $S_i$ の写像 $\sigma$ と $\zeta_i$ 一致するであるため、$S_i$ は、$\sigma$ の制限によって生成された $\sigma$ と $\mathfrak{S}_{S_i}$ の部分群では安定しています。 $S_i$ は $S_i$ で推移的に動作します。したがって、$S_i$ は $\bar{\sigma}$ 軌道です。 $S_i$ は空ではなく、ペアの互いに素であるため、写像 $i \mapsto S_i$ は単射です。 $\bigcup_i S_i$ は $x$ の集合であるため、$\sigma(x) \neq x$ は、単一の元のからなるではないすべての $\bar{\sigma}$ 軌道は $S_i$ の 1 つです。

#### 命題 7 {#alg-i-s5-prop-7 .statement tag=05BP}

E を E の有限集合および $\sigma$ 置換とします。 条件に続く 2 つのサイクル満たすの有限集合 C が 1 つだけ存在します。

(a) C の元のサポートはペアごとに互いに素です。

(b) $\sigma = \prod_{\zeta \in C} \zeta$ (C の元は補題 1 によってペアごとに変更可能)。

$\bar{\sigma}$ を $\sigma$ によって生成された部分群とし、S を単一の元のからなるではなく、$\bar{\sigma}$ 軌道の集合とします。 $s \in S$には、$x \in s$の場合は$\zeta_s(x) = \sigma(x)$、$x \notin s$の場合は$\zeta_s(x) = x$と書きます。すべての $s \in S$ に対して、$\zeta_s$ は、$s$ と $\sigma = \prod_{s \in S} \zeta_s$ がサポートとなるサイクルです。E の任意の元の両側適用からわかるように、C の一意性は、補題 1 から続きます。

#### 定義 9 {#alg-i-s5-def-9 .statement tag=05BQ}

*位数 2 のサイクルを転置といいます。*

$x$ と $y$ を E の 2 つの *別個の * 元とします。 $\tau_{x,y}$ はサポート $\{x, y\}$ を持つ一意の転置を表します。

E 置換 $\sigma \cdot \tau_{x,y} \cdot \sigma^{-1}$ のすべての置換 $\sigma$ は、サポートが $\{\sigma(x), \sigma(y)\}$ である転置です。したがって、次のようになります。

(4)
$$
\sigma \cdot \tau_{x,y} \cdot \sigma^{-1} = \tau_{\sigma(x), \sigma(y)}.
$$

したがって、形共役類を群 $\mathfrak{S}_E$ に移調します。

#### 命題 8 {#alg-i-s5-prop-8 .statement tag=05BR}

*E を有限集合とします。 群 $\mathfrak{S}_E$ は転置によって生成されます。*

置換 $\sigma$ ごとに、$F_\sigma$ を $x \in E$ の集合とし、$\sigma(x) = x$ とします。 $p$ で帰納法を下降することにより、$\mathrm{Card}(F_\sigma) = p$ が積となるようなすべての置換 $\sigma$ が転置されることを示します。 $p \geq \mathrm{Card}(E)$ の場合、置換 $\sigma$ は E の恒等写像です。それは移調の空の族の積です。 $p < \mathrm{Card}(E)$ の場合、$\mathrm{Card}(F_{\sigma'}) > p$ となるように、置換 $\sigma'$ ごとに性質が証明されるとします。現在 $E - F_\sigma \neq \varnothing$; $x \in E - F_\sigma$と$y \in \sigma(x)$としましょう。続いて$y \neq x$と$y \in E - F_\sigma$。 $\sigma' = \tau_{x,y} \cdot \sigma$ にしましょう。 集合 $F_{\sigma'}$ 含む $F_\sigma$ と $x$、したがって $\mathrm{Card}(F_{\sigma'}) > \mathrm{Card}(F_\sigma) = p$ です。 帰納法の仮定により、$\sigma'$ は転置の積となり、したがって $\sigma = \tau_{x,y} \cdot \sigma'$ は転置の積になります。

#### 命題 9 {#alg-i-s5-prop-9 .statement tag=05BS}

*n を整数 $\geq 0$ とします。 群 $\mathfrak{S}_n$ は、転​​置* $(\tau_{i, i+1})_{1 \leq i \leq n-1}$ によって生成されます。

命題 8 により、すべての転置 $\tau_{p,q}$、$1 \leq p < q \leq n$、属するから部分群 H が $\tau_{i, i+1}$、$1 \leq i \leq n-1$ によって生成されることを示すだけで十分です。 $q-p$の帰納法までにこれを表示します。 $q-p = 1$ については、それは明らかです。 $q-p > 1$なら、(公式(4))$\tau_{p,q} = \tau_{q-1,q} \tau_{p,q-1} \tau_{q-1,q}$。 帰納法の仮定 $\tau_{p,q-1} \in H$ までに、つまり $\tau_{p,q} \in H$ までに。

$\sigma \in \mathfrak{S}_n$ の場合、$i < j$ と $\sigma(i) > \sigma(j)$ が$\sigma$ の *反転* と呼ばれる、$\{1, n\}$ の元のすべての順序付けられた対 $(i, j)$ 。 $\nu(\sigma)$ が $\sigma$ の反転の数を表すものとします。

P を $\mathbf{Z}^n$ から $\mathbf{Z}$ までの写像の加法群とします。 $f \in P$ と $\sigma \in \mathfrak{S}_n$ について、$\sigma f$ を次のように定義される P の元とします。

(5)
$$
\sigma f(z_1, \ldots, z_n) = f(z_{\sigma(1)}, \ldots, z_{\sigma(n)}).
$$

このように定義された P の $\mathfrak{S}_n$ の作用は演算です。すべての$\sigma, \tau \in \mathfrak{S}_n$、$f \in P$、$\sigma f = f$、そして
$$
\begin{align*}
(\tau(\sigma f))(z_1, \ldots, z_n) &= \sigma f(z_{\tau(1)}, \ldots, z_{\tau(n)}) = f(z_{\tau \sigma(1)}, \ldots, z_{\tau \sigma(n)}) \\
&= ((\tau \sigma) f)(z_1, \ldots, z_n).
\end{align*}
$$
公式 (5) は、$\sigma \in \mathfrak{S}_n$ と $f \in P$ に対して $\sigma(-f) = -\sigma f$ であることを示しています。

$p$ を次のように定義される P の元とします。

$$
p(z_1, \ldots, z_n) = \prod_{i < j} (z_j - z_i).
$$

#### 補題 2 {#alg-i-s5-lem-2 .statement tag=05BT}

$p \neq 0$ と $\sigma p = (-1)^{\nu(\sigma)}$ は $\sigma \in \mathfrak{S}_n$ です。

$p(1, 2, \ldots, n) = \prod_{i < j} (j - i) \neq 0$、つまり $p \neq 0$ です。一方、$\sigma \in \mathfrak{S}_n$ の場合、

$$
\sigma p(z_1, \ldots, z_n) = p(z_{\sigma(1)}, \ldots, z_{\sigma(n)}) = \prod_{i < j} (z_{\sigma(j)} - z_{\sigma(i)}).
$$

C を、$1 \leq i \leq n,\ 1 \leq j \leq n,\ i < j$ となるように、注文された対 $(i, j)$ の集合とします。 置換 $\theta$ は、$(i, j)$ が反転でない場合は $\theta(i, j) = (\sigma(i), \sigma(j))$、$(i, j)$ が反転である場合は $\theta(i, j) = (\sigma(j), \sigma(i))$ によって設定によって C に定義されます。これは$\sigma p = (-1)^{\nu(\sigma)} p$を意味します。

#### 定理 2 {#alg-i-s5-thm-2 .statement tag=05BU}

*E を有限の集合とします。 $\mathfrak{S}_n$ から乗法群 $\{-1, +1\}$ には、転置 $\tau$ ごとに $\varepsilon(\tau) = -1$ となる準同型 $\varepsilon$ が 1 つだけ存在します。*

一意性は命題から続きます 8. 存在を示します。 構造を輸送することで、$E = \{1, n\}$ になると考えられます。上記の記法を使用して、$\varepsilon(\sigma) = (-1)^{\nu(\sigma)}$とします。それでは (補題 2)

$$
\sigma(\sigma' p) = \sigma(\varepsilon(\sigma') p) = \varepsilon(\sigma') (\sigma p) = \varepsilon(\sigma') \varepsilon(\sigma) p.
$$

一方、

$$
\sigma(\sigma' p) = (\sigma \sigma') p = \varepsilon(\sigma \sigma') p.
$$

$p \neq -p$ とすると、$\varepsilon(\sigma \sigma') = \varepsilon(\sigma) \varepsilon(\sigma')$ となり、$\varepsilon$ は準同型となります。ここで、すべての転置 $\tau$、$\varepsilon(\tau) = -1$ について、それを示します。 $\nu(\tau_{n-1, n}) = 1$、よって $\varepsilon(\tau_{n-1, n}) = -1$。すべての転置 $\tau$ は共役から $\tau_{n-1, n}$ であり、群 $\{-1, +1\}$ は可換です、$\varepsilon(\tau) = \varepsilon(\tau_{n-1, n}) = -1$。

#### 定義 10 {#alg-i-s5-def-10 .statement tag=05BV}

*定理 2 の記法では、数 $\varepsilon(\sigma)$ ($\varepsilon_\sigma$ とも表記) は、置換 $\sigma$ の署名と呼ばれます。 準同型 $\varepsilon$ の核は、E の交代的群と呼ばれます。

$\varepsilon(\sigma) = 1$ (または $\varepsilon(\sigma) = -1$) の場合、$\sigma$ は *偶数* (または *奇数*) と呼ばれます。 Eの交代的群は$\mathfrak{A}_E$で表されます。 $\mathfrak{S}_E$の通常の部分群です。 $E = \{1, n\}$の場合は、単に$\mathfrak{A}_n$と表記します。 E の基数 $n$ が $\geq 2$ のとき、それは添字 2 の部分群なので、位数 $n! / 2$ です。 $n = 3$ または $n \geq 5$ の場合、群 $\mathfrak{A}_n$ は単純な群 (*cf. 練習問題 16*) であることがわかります。

#### 例 {#alg-i-s5-n7-exa-1 .statement tag=05BW}

$\sigma$ が位数 $d$ のサイクルである場合、
$$
\varepsilon(\sigma) = (-1)^{d-1}.
$$
置換の反転の数
$$
(1, 2, 3, \ldots, d) \mapsto (d, 1, 2, \ldots, d-1)
$$
は$d-1$に等しい。

### 練習問題 {#alg-i-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
