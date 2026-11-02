---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 4
section_title: Groups and groups with operators
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 30-52, 132-140
pdf_pages: 0054-0076, 0156-0164
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS
      page: 30
      pdf_page: 54
    - "no": 2
      title: GROUPS WITH OPERATORS
      page: 31
      pdf_page: 55
    - "no": 3
      title: SUBGROUPS
      page: 32
      pdf_page: 56
    - "no": 4
      title: QUOTIENT GROUPS
      page: 34
      pdf_page: 58
    - "no": 5
      title: DECOMPOSITION OF A HOMOMORPHISM
      page: 37
      pdf_page: 61
    - "no": 6
      title: SUBGROUPS OF A QUOTIENT GROUP
      page: 38
      pdf_page: 62
    - "no": 7
      title: THE JORDAN-HÖLDER THEOREM
      page: 41
      pdf_page: 65
    - "no": 8
      title: PRODUCTS AND FIBRE PRODUCTS
      page: 45
      pdf_page: 69
    - "no": 9
      title: RESTRICTED SUMS
      page: 47
      pdf_page: 71
    - "no": 10
      title: MONOGENOUS GROUPS
      page: 48
      pdf_page: 72
statements: 63
exercises: 26
content_sha256: 9ae5b3ee394565f43fab28a677595a41f91f678e3ccec7ad2c776ae3595b2a77
translated_from: content/en/alg/I/04_s4_groups_and_groups_with_operators.md
translation_method: google
source_content_sha256: d6bc940de2b7bc4d5c77deed1610950a126e1ac53cd26ce4b8099a1f2945d150
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 60b1b16c7d9a5df96611c1edc89d255329be6ae7b9182f286fb9381dab6dbc11
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。 群と群演算子付き

### 1. 群

次の定義 (§ 2, no. 3、定義 6) を思い出してください。

#### 定義 1 {#alg-i-s4-def-1 .statement tag=058H}

*集合と合成の結合法則があり、単位元を持ち、その下ではすべての元が反転可能であり、群と呼ばれます。

他の語では、群は *モノイド* (§ 2, no. 1、定義 1) であり、すべての元が可逆です。 集合の合成のうち決定する群構造の法則を*群法則*と呼びます。 G と H が 2 つの群である場合、G から H へのマグマ準同型も *群準同型* と呼ばれます。 準同型 $f$ 写像単位元から単位元;なぜなら、$e$ (それぞれ $e'$) を G (それぞれ H) の単位元とします。 G と H の群法則を乗算して書き、$e \cdot e = e$、よって $f(e) \cdot f(e) = f(e)$、そして $f(e)^{-1}, f(e) = e'$ を乗算します。したがって、$f$ は単体です。次に、§ 2 の no. 3 から、すべての $x \in G$ に対して $f(x^{-1}) = f(x)^{-1}$ が続きます。

#### 例 {#alg-i-s4-n1-exa-1 .statement tag=058I}

任意のモノイド E では、E 上のものによって誘導される構造を伴う可逆元の集合は群です。 特に、集合 F の全単射写像 (または F の *置換* の集合) の集合は、法則 $(f, g) \mapsto f \circ g$ の下で群であり、集合* F の*対称群と呼ばれ、次のように表されます。 $\mathfrak{S}_F$。

この段落では、特に示されていない場合、〜でない限り、群の合成の法則は常に*乗算*で書かれ、$e$はそのような群法則の単位元を表します。

G の基礎となる集合が有限である場合、群 G は *有限* と呼ばれます。それ以外の場合は *infinite* と呼ばれます。 群の基数は、群の*位数*と呼ばれます。

G の合成の法則が G の決定する群構造の場合、その反対の法則も同様です。 The mapping of a group G onto itself which associates with each $x \in G$ the inverse of $x$ is an *isomorphism* of G onto the opposite group (§ 2, no. 3, Proposition 4).

一般的な規則 (*集合理論*、II, § 3, no. 1) に従って、写像 $x \mapsto x^{-1}$ の下の G の部分集合 A の $A^{-1}$ 像で表します。しかし、記法の類似にもかかわらず、$A^{-1}$はGの部分集合の間の合成$(X, Y) \mapsto XY$の法則の下でAの逆元ではないことに注意することが重要です（XYが$xy$の集合であることを思い出してください） $x \in X, y \in Y$): この法則の下の単位元は $\{e\}$ であり、この法則の下の $\mathscr{P}(G)$ の唯一の可逆元は、単一の元の集合からなるです (さらに、そのような A は確実に逆数を持ちます) $A^{-1}$）。アイデンティティ

$(AB)^{-1}=B^{-1}A^{-1}$ は $A\subset G$、$B\subset G$ に当てはまります。 $A=A^{-1}$の場合、$A$は$G$の対称部分集合と呼ばれます。すべての$A\subset G$、$A\cup A^{-1}$、$A\cap A^{-1}$、$AA^{-1}$ は対称です。

### 2. 群オペレーター付き

#### 定義 2 {#alg-i-s4-def-2 .statement tag=058J}

$\Omega$ を集合とします。 群 $G$ は、群法則に関して分配である $G$ 上の $\Omega$ の作用と合わせて、$\Omega$ の演算子を使用して群と呼ばれます。

以下の$x^\alpha$は$\alpha\in\Omega$と$x\in G$の合成を表します。この場合、分配性は恒等式 $(xy)^\alpha=x^\alpha y^\alpha$ によって表現されます。

In a group with operators $G$, each operator defines an *endomorphism* of the underlying *group structure*; these endomorphisms will sometimes be called the *homotheties* of the group with operators $G$.

演算子 $G$ を伴う群は、その群法則が可換である場合、*可換* (または *アーベル*) と呼ばれます。

以下では、群 $G$ は、$G$ の$\varnothing$ の一意の作用を $G$ に与えることで得られる $\varnothing$ の演算子を使用して、群で識別されます。これにより、群を演算子を使用した群の特別なケースとして考慮し、それらに定義を適用し、後者に関連する結果を述べることができます。

#### 例 {#alg-i-s4-n2-exa-1 .statement tag=058K}

In a commutative group $G$, written multiplicatively, $(xy)^n=x^ny^n$ for all $n\in\mathbf{Z}$ (§ 2, no. 8, equation (1)); the action $n\mapsto(x\mapsto x^n)$ of $\mathbf{Z}$ on $G$ therefore defines, together with the group law, the structure of a group with operators on $G$.

#### 定義 3 {#alg-i-s4-def-3 .statement tag=058L}

$G$ と $G'$ を $\Omega$ の演算子を使用して群とします。 A homomorphism of groups with operators of $G$ into $G'$ is a *homomorphism of the group* $G$ into the *group* $G'$ such that

$$
f(x^\alpha)=(f(x))^\alpha
$$

すべての $\alpha\in\Omega$ とすべての $x\in G$ に対して。

演算子 $G$ を使用した群の *自己準同型* は、群 $G$ の自己準同型であり、これは $G$ のすべての *相同性* と *置換可能* です。

群と演算子 $G$ の 2 つの相同性は必ずしも置換可能ではないため、一般に $G$ の *ホモテティー は演算子 $G$ を使用した群の自己準同型ではありません。

演算子を使用した場合の群の恒等写像は、演算子を使用した場合の群の準同型です。 合成の 2 準同型の群も演算子付きで 1 つです。 写像が演算子を使用して群の同型になるためには、それが演算子を使用して群の全単射準同型であり、その逆の写像が演算子を使用して群の同型であることが必要かつ十分です。

より一般的には、G (または G') を群とし、$\Omega$ (または $\Omega'$) に演算子を入れます。 $\phi$を$\Omega$の写像を$\Omega'$にします。 G から G' への $\phi$ 準同型性は、群 G から群 G' への準同型です。

$$
f(x^\alpha) = (f(x))^{(\phi(\alpha))}
$$

すべての $\alpha \in \Omega$ とすべての $x \in G$ に対して。

この段落の残りの部分では、集合 $\Omega$ が与えられます。 〜でない限り別途言及されている演算子を考慮した群は、$\Omega$ を演算子の集合として認めます。

### 3. 部分群

#### 定義 4 {#alg-i-s4-def-4 .statement tag=058M}

*演算子を使用して G を群とします。安定した G の部分群は、次の特性を持つ G の部分集合 H です*:

(i) $e \in H$;
(ii) $x, y \in H \implies xy \in H$;
(iii) $x \in H \implies x^{-1} \in H$;
(iv) $x \in H$ と $\alpha \in \Omega$ は $x^\alpha \in H$ を暗示します。

If H is a stable subgroup of G, the structure induced on H by the structure of a group with operators on G is the structure of a group with operators and the canonical injection of H into G is a homomorphism of groups with operators.

G を群とします。 $\varnothing$ (no. 2) の作用を伴う G の安定な部分群、つまり G の部分集合満たす条件 (i)、(ii)、(iii) の定義 4 は、G の *部分群* と呼ばれます。演算子の群の部分群は、常にGの基礎となる群の部分群を意味します。演算子Gを使用した群の部分群は、必ずしもGの安定した部分群ではありません。

*例* (1)。 Let $\Sigma$ be a species of structure (*Set Theory*, IV, § 1, no. 4) and S a structure of species $\Sigma$ on a set E (*loc. cit.*). Sの*自己同型*の集合は$\mathscr{G}_E$の部分群です。

#### 命題 1 {#alg-i-s4-prop-1 .statement tag=058N}

*演算子を使用して G を群とし、G の相似性のもとで安定な G の H 部分集合とします。次の条件は同等です*:

(a) *H は G* の安定した部分群です。
(b) *H は空ではなく、関係* $x \in H, y \in H \implies xy \in H$ *および* $x^{-1} \in H$。
(c) *H は空ではなく、関係* $x \in H, y \in H \implies xy^{-1} \in H$ です。
(d) *H は G 上の法則では安定であり、G 上の合成の法則によって H に誘導された合成の法則は群法則* です。

明らかに (a) は (b) を意味します。 (b) が (a) を意味することを示します。 G の H 含む単位元が示されれば十分です。部分集合 H は空ではないので、$x \in H$ とします。次に$x^{-1} \in H$と$e = xx^{-1} \in H$です。明らかに (b) は (c) を意味します。 (c) が (b) を意味することを示します。まず、H は空ではないので、含む元 x です。したがって、xx^{-1} = e は H の元です。H の元 x ごとに、H は $x^{-1} = ex^{-1}$ 属するになります。したがって、関係 $x \in H, y \in H$ は $x(y^{-1})^{-1} = xy \in H$ を暗示します。明らかに (a) は (d) を意味します。 (d) が (a) を意味していることを示します。H から G への標準単射は群準同型です。したがって、$e \in H$ と関係 $x \in H$ は $x^{-1} \in H$ (no. 1) を意味します。

#### 注意 {#alg-i-s4-n3-rem-1 .statement tag=058O}

(1) 同様に、条件 (b) は条件と同等であることが示されます。
(c') $H \neq \varnothing$ と関係 $x \in H$ と $y \in H$ は $y^{-1}x \in H$ を暗示します。
(2) G の部分群 H ごとに、次の関係が存在します。
$$(1)$$
$$H.H = H \quad \text{and} \quad H^{-1} = H.$$
$H.H \subset H$ と $H^{-1} \subset H$ の場合は (b) による。 $e \in H, H.H \supset e.H = H$ と逆数変換をとり、$H^{-1} \subset H$ を$H \subset H^{-1}$、よって式 (1) に含めます。

H が G の安定な部分群で、K が H の安定な部分群である場合、明らかに K は G の安定な部分群です。

集合 $\{e\}$ は G の最小の安定部分群です。G の安定部分群のファミリーの共通部分は安定部分群です。したがって、G の与えられた部分集合 X には、安定した最小の G の H 部分群含むが存在します。それは * X によって生成された * 安定な部分群と呼ばれ、X は H の *生成する系* (または *生成する集合*) と呼ばれます。

#### 命題 2 {#alg-i-s4-prop-2 .statement tag=058P}

*X を演算子 G を持つ群の空でない部分集合とし、$\hat{X}$ を X によって生成された G 上の $\Omega$ の作用の下で安定した部分集合とします。 X によって生成された安定した部分群は、集合 $Y = \hat{X} \cup \hat{X}^{-1}$ によって生成された G 上の法則の下で安定した部分集合です。

The latter subset Z is the set of compositions of finite sequences all of whose terms are elements of $\hat{X}$ or inverse of elements of $\hat{X}$: the inverse of such a composition is a composition of the same form (§ 2, no. 3, Corollary 1 to Proposition 5) and Z is stable under the action of $\Omega$, as is seen by applying § 3, no. 4, Proposition 1 to the homotheties of G, hence (Proposition 1) Z is a *stable subgroup* of G. 逆に、すべての安定した部分群含む X は明らかに含む Y であり、したがって Z です。

#### 系 1 {#alg-i-s4-prop-2-cor-1 .statement tag=058Q}

*演算子を使用して G を群とし、$\Omega$ の作用で安定する G の X 部分集合とします。 部分群は X によって生成され、安定した部分群は X 一致するによって生成されます。*

#### 系 2 {#alg-i-s4-prop-2-cor-2 .statement tag=058R}

*G をペアごとに置換可能な元の G からなるの群と X 部分集合とします。 X によって生成された G の部分群は可換です。*

集合 $Y = X \cup X^{-1}$ は、ペアごとに置換可能な元 (§ 2, no. 3、命題 5) と、Y によって生成された安定な部分集合上で誘導された法則は可換です (§ 1, no. 5、系 2)。

演算子を使用して G が群である場合、ペアごとに置換可能な元の G からなるの部分集合によって生成される安定な部分群は必ずしも可換であるとは限りません。

#### 系 3 {#alg-i-s4-prop-2-cor-3 .statement tag=058S}

$f : G \to G'$ を演算子付きの群の準同型と G の X 部分集合とします。 X によって生成された G の安定な部分群の f の下の像は、$f(X)$ によって生成された G' の安定な部分群です。

$X' = f(X)$ にしましょう。次に$\hat{X}' = f(\hat{X})$と${X'}^{-1} = f(X^{-1})$です。したがって、
$$
f(\hat{X} \cup \hat{X}^{-1}) = \hat{X}' \cup \hat{{X}'}^{-1}.
$$
§ 1, no. 4、命題 1 から系が続きます。

例 (2)。 G を群 、G の x 元とします。 $\{x\}$ によって生成された部分群 (より簡単に x によって生成された部分群と呼ばれます) は、$x^n, n \in \mathbf{Z}$ の集合です。 $\{x\}$ によって生成された安定した部分集合 (G の法則の下) は、$n \in \mathbf{N}^*$ である $x^n$ の集合です。これら 2 つの集合は一般に区別されます。

したがって、加法群 $\mathbf{Z}$ では、元 x によって生成される部分群は $xn, n \in \mathbf{Z}$ の集合 $x.\mathbf{Z}$ であり、x によって生成される安定した部分集合は $xn, n \in \mathbf{N}^*$ の集合です。これら 2 つの集合は、$x \neq 0$ の場合には常に区別されます。

G の安定した部分群の右方向ファミリーの和集合は明らかに安定した部分群です。その結果、P が G と H の部分集合である場合、P と一致しない G の安定な部分群、G 含む H の安定な部分群の集合は包含順序で帰納的です (集合理論, III, § 2, no. 4)。 適用 Zorn の補題 (集合理論, III, § 2, no. 4) を使用すると、次の結果が得られます。

#### 命題 3 {#alg-i-s4-prop-3 .statement tag=058T}

G を演算子で群とし、G と H の P 部分集合は P を満たさない安定な部分群 G とします。 G 含む H の安定な部分群の集合で P を満たさない極大元とします。

### 4. 剰余群

#### 定理 1 {#alg-i-s4-thm-1 .statement tag=058U}

演算子 G を使用して、R を群上の同値関係とします。 Rが左(または右)でGの群法則と互換性(§ 3, no. 3)で、$\Omega$の作用と互換性がある場合、eの同値類はGの安定した部分群Hであり、関係Rは$x^{-1}y \in H$(それぞれ$yx^{-1} \in H$)と同等です。逆に、H が G の安定した部分群である場合、関係 $x^{-1}y \in H$ (または $yx^{-1} \in H$) は同値関係であり、左 (または右) で G の群法則と互換性があり、$\Omega$ の作用と互換性があり、その下で H は G の同値類になります。 e.

関係 R が G 上の法則と互換性がある場合に注意を限定します (互換性のある右関係の後に、その逆の法則によって G 上で置き換えること法則が続きます)。 関係 $y \equiv x \pmod{R}$ は $x^{-1}y \equiv e \pmod{R}$ と等しく、$y \equiv x$ は $x^{-1}y \equiv x^{-1}x = e$ を暗示し、逆に $x^{-1}y \equiv e$ は $y = x(x^{-1}y) \equiv x$ を暗示します。 H が e の同値類を表す場合、関係 R は $x^{-1}y \in H$ と同等になります。 H が G の安定な部分群であることを示します。すべての演算子 $\alpha$ について、関係 $x \equiv e$ は $x^\alpha \equiv e^\alpha = e$ を意味するため、$H^\alpha \subset H$ となり、H は $\Omega$ の作用で安定です。 $x \in H$ と $y \in H$ は $x^{-1}y \in H$、つまり $x \equiv e$ と $y \equiv e$ は $x \equiv y$、つまり R の推移性の帰結を暗示すること (命題 1) を確立するだけで十分です。

逆に、H を G の安定な部分群とします。 関係 $x^{-1}y \in H$ は $x^{-1}x = e \in H$ から再帰的です。 $x^{-1}y \in H$ は $y^{-1}x = (x^{-1}y)^{-1} \in H$ を意味するので対称です。これは推移的であり、$x^{-1}y \in H$ と $y^{-1}z \in H$ は $x^{-1}z = (x^{-1}y)(y^{-1}z) \in H$ を暗示します。 G の合成の法則と、すべての $z \in G$ の $x^{-1}y = (zx)^{-1}(zy)$ との互換性が残されています。最後に、すべての演算子 $\alpha$ について、関係 $y \in xH$ は $y^\alpha \in x^\alpha H^\alpha \subset x^\alpha H$ を意味するため、同値関係 $x^{-1}y \in H$ は G の $\Omega$ の作用と互換性があります。

G を G の群、H を部分群とします。 関係 $x^{-1}y \in H$ (それぞれ $yx^{-1} \in H$) は、同等の形 $y \in xH$ (それぞれ $y \in Hx$) でも書かれます。 G のすべての部分群 H は、したがって定義する G 上の 2 つの等価な関係、つまり $y \in xH$ と $y \in Hx$ です。これらの関係の下で等価な類はそれぞれ集合 $xH$ であり、これらは H* の *左剰余類と呼ばれます (または*modulo H*)、および集合 $Hx$、これらは *H* の右剰余類 (または *modulo H*) と呼ばれます。これら関係 (*集合理論*, II, § 6, no. 4) に対して部分集合 $A \subset G$ を *飽和* することで、それぞれ集合 AH と HA が得られます。 写像 $x \mapsto x^{-1}$ 変換 H を法とする左剰余類を H を法とする右剰余類に変換し、その逆も行います。

左剰余類 (mod. H) の集合の基数は、G に関する部分群 H の *添字* と呼ばれ、$(G:H)$ で表されます。また、右剰余類の集合の基数にも等しい。

G 含む H の部分群 K なら、H の左 (または右) 剰余類の和集合です。K の左剰余類は K から左変換によって得られるので、K の左剰余類に含まれる H の左剰余類の集合は後者とは独立して基数を持ちます。したがって (*集合理論*, III, § 5, no. 8, 命題 9):

#### 命題 4 {#alg-i-s4-prop-4 .statement tag=058V}

*H と K を群 G の 2 つ部分群とし、H $\subset$ K とします。すると*
$$
(G:H) = (G:K)(K:H).
$$

#### 系 {#alg-i-s4-n4-cor-1 .statement tag=058W}

*G が位数 g の有限群で、H が位数 h の G の部分群である場合、*
$$
h \cdot (G:H) = g
$$
(特に、H の位数と添字は、G の位数の *因子* です)。

定理 1 により、演算子 G を使用して群の法則と互換性のある決定する同値関係が可能になります。R が関係の場合、G の群法則および G の作用と左右両方で互換性があります。 $\Omega$。したがって、H が $e$ (mod. R) の類である場合、H は安定な部分群となり、関係 $y \in xH$ と $y \in Hx$ は等価になります (両方とも R と等価であるため)。したがって、すべての $x \in G$ に対して $xH = Hx$ となります。逆に、そうであれば、この法則 ($\S$ 3、no. 4) と左右両方に互換性があり、$\Omega$ の作用と互換性があるため、同等の関係 $y \in xH, y \in Hx$ のいずれかが群法則と互換性があります。方程式$xH = Hx$は$xHx^{-1} = H$と等しいので、次の定義を作ります。

#### 定義 5 {#alg-i-s4-def-5 .statement tag=058X}

※演算子を使ってGを群とします。すべての $x \in G$ に対して $xHx^{-1} = H$ である場合、G の安定な部分群 H は、G の正規 (または不変) 安定部分群と呼ばれます。

$\Omega = \varnothing$ の場合、G の正規安定部分群は G の *正規* (または *不変量*) *部分群* と呼ばれます。可換群では、すべての部分群が正規です。

安定した部分群 H が正常であることを検証するには、すべての $x \in G$ について $xHx^{-1} \subset H$ を示すだけで十分です。もしそうなら、すべての $x \in G$ に対して $x^{-1}Hx \subset H$、つまり $H \subset xHx^{-1}$、したがって $H = xHx^{-1}$ となるからです。

H を、H によって定義される G および R 同値関係 $y \in xH$ の正規安定部分群とする。 商集合 $G/R$ では、群 G の法則の R による内部法則、商は結合します。 e の類は、この商法則の単位元です。 G の 2 つの逆行列元の類は、G 上の $\Omega$ の作用の R による $\Omega$、商の商法則と作用の下での逆行列です。 $G/R$ の内部法則 ($\S$ 3、no. 5)。したがって、得られた結果を要約すると、次のようになります。

#### 定理 2 {#alg-i-s4-thm-2 .statement tag=058Y}

*演算子を使用して G を群とします。 G 上の同値関係 R が $\Omega$ の群法則および作用と互換性があるためには、それが形 $x^{-1}y \in H$ であることが必要かつ十分です。ここで、H は G の通常の安定な部分群 (さらに、そのような場合には関係 $x^{-1}y \in H$ は $yx^{-1} \in H$ と同等です) 部分群）。 The law of composition on $G/R$ the quotient of that on G and the action of $\Omega$ on $G/R$ the quotient of that of $\Omega$ on G by such a relation R give $G/R$ the structure of a group with operators, called the quotient structure, and the canonical mapping of the passage to the quotient is a homomorphism of groups with operators.*

#### 定義 6 {#alg-i-s4-def-6 .statement tag=058Z}

* 商構造を伴う、G の通常の部分群 H によって定義される同値関係による演算子 G を持つ群の商は、G by H の演算子を持つ剰余群と呼ばれ、$G/H$ で表されます。 標準写像 $G \to G/H$ is called 標準準同型*

G を群、H を G の正規の部分群とします。 商 $G/H$ とその群構造は、H による G の *剰余群* と呼ばれます。 $G/H$ から群までの写像について、演算子は の準同型になります群演算子では、$G/H$ に G の標準写像を加えた合成が 1 つであることが必要かつ十分です。これにより、名前 "剰余群" (*集合理論*、IV、$\S$ 2、no. 6) が正当化されます。

G の正規安定部分群によって定義される同値関係は、$x \equiv y \pmod{H}$ または $x \equiv y(H)$ で表されます。

#### 命題 5 {#alg-i-s4-prop-5 .statement tag=0590}

Let $f : G \to G'$ be a homomorphism of groups with operators and $H$ and $H'$ normal stable subgroups of $G$ and $G'$ respectively such that $f(H) \subset H'$. 写像 $f$ は、$H$ および $H'$ によって定義される同値関係と互換性があります。 $\pi : G \to G/H$ と $\pi' : G' \to G'/H'$ を標準準同型とします。 $f$から移行から商まで導いた写像$\bar{f} : G/H \to G'/H'$は準同型です。

$x \equiv y \pmod{H}$ の場合、$x^{-1}y \in H$、よって
$$
f(x)^{-1}f(y) = f(x^{-1})f(y) = f(x^{-1}y) \in f(H) \subset H'
$$
したがって $f(x) \equiv f(y) \pmod{H'}$ です。 2 番目の主張は、商法則 ($§ 1$、no. 6) の普遍性から続きます。

#### 注意 {#alg-i-s4-n4-rem-1 .statement tag=0591}

(1) $A$ が群 $G$ のいずれかの部分集合で、$H$ が $G$ の通常の部分群である場合、$AH = HA$;この集合は、関係$x \equiv y \pmod{H}$に関して$A$を飽和させることで得られます。

(2) $H$ が有限添字の$G$ の正規部分群である場合、剰余群 $G/H$ は位数 $(G:H)$ の有限群です。

Note that if $H$ is a normal subgroup of a group $G$ and $K$ is a normal subgroup of $H$, $K$ is not necessarily a normal subgroup of $G$ (I, $§ 5$, Exercise 10).

演算子を使用して $G$ を群とします。 $G$ の各ファミリーの共通部分は通常の厩舎部分群が通常の厩舎部分群です。 したがって、$G$ のすべての部分集合 $X$ に対して、$X$ によって生成された通常安定部分群と呼ばれる最小の正常安定部分群含む $X$ が存在します。

演算子$G$を使用した群では、安定した部分群$G$と$\{e\}$が正常です。

#### 定義 7 {#alg-i-s4-def-7 .statement tag=0592}

*群演算子* $G$ *単純な if と呼ばれます* $G \neq \{e\}$ *そして、* $G$ * 以外* $G$ * および* $\{e\}$ の通常の安定な部分群が存在しません。

### 5. 準同型中分解

#### 命題 6 {#alg-i-s4-prop-6 .statement tag=0593}

*Let* $G$ *be a group with operators and* $G'$ *a magma with an action by* $\Omega$, *written exponentially*. *$f : G \to G'$ *マグナの準同型にしましょう* $G$ *マグマの中へ* $G'$ *すべて* $\alpha \in \Omega$ *そしてすべて* $x \in G$、$f(x^\alpha) = f(x)^\alpha$ になるようにします。 *その後* $f(G)$ *は* $G'$ * 法則の下* $G'$ * および* $\Omega$ の作用で安定した部分集合です。 *集合* $f(G)$ *誘導された法則は演算子付きの群であり、写像* $x \mapsto f(x)$ *of* $G$ *into* $f(G)$ *は演算子*付きの準同型群です。

$§ 1$、no. 4、命題 1 により、$f(G)$ は$G'$ の内部法則の下で$G'$ の安定した部分集合です。すべての元 $x \in G$ およびすべてのオペレーター $\alpha$ について、
$f(x)^\alpha = f(x^\alpha) \in f(G)$ したがって、$f(G)$ は、$G'$ の $\Omega$ の作用で安定します。 $G'$ の内部の法則を乗算的に書くと、
$$
(f(x)f(y))f(z) = f(xy)f(z) = f((xy)z) = f(x(yz)) = f(x)f(yz)
= f(x)(f(y)f(z))
$$
$G$ の元 $x, y, z$ 全員に対して。したがって、$f(G)$ に誘導された法則は結合的です。

$e$ を $G$ の単位元とします。その像 $f(e)$ は、$f(G)$ ($§ 2$、no. 1) の単位元です。 $f(G)$ のすべての元は、$f(G)$ ($§ 2$、no. 3) で反転可能です。したがって、$G'$ の内部法則によって$f(G)$ に誘発された法則は、群法則になります。 $G$ のすべての元 $x$ と $y$ およびすべての演算子 $\alpha$ について、

$$
(f(x)f(y))^\alpha = (f(xy))^\alpha = f((xy)^\alpha) = f(x^\alpha y^\alpha) = f(x^\alpha)f(y^\alpha) = (f(x))^\alpha(f(y))^\alpha
$$

これは、$\Omega$の作用が$f(G)$の群法則に関して分配的であることを示しています。したがって、誘導された法則を伴う $f(G)$ は、演算子を使用すると群となり、明らかに写像 $x \mapsto f(x)$ は演算子を使用すると群の準同型になります。

#### 定義 8 {#alg-i-s4-def-8 .statement tag=0594}

※演算子を使って$f : G \to G'$を群の準同型とします。 $G'$の単位元の逆像は、$f$の核と呼ばれます。*

The kernel of $f$ is often denoted by $\mathrm{Ker}(f)$ and the image $f(G)$ of $f$ is sometimes denoted by $\mathrm{Im}(f)$.

#### 定理 3 {#alg-i-s4-thm-3 .statement tag=0595}

*演算子を使用して、$f : G \to G'$を群の準同型とします。
(a) *$\mathrm{Ker}(f)$ は $G$ の通常の安定した部分群;*
(b) *$\mathrm{Im}(f)$ は $G'$ の安定した部分群;*
(c) *写像 $f$ は、$G$ で $\mathrm{Ker}(f)$ によって定義された同値関係と互換性があります。*
(d) *演算子を使用すると、移行から商によって$f$から導出された写像$\tilde{f} : G/\mathrm{Ker}(f) \to \mathrm{Im}(f)$は、群の同型になります。
(e) *$f = i \circ \tilde{f} \circ \pi$、ここで、$i$は$\mathrm{Im}(f)$の標準単射を$G'$に、$\pi$は$G$の標準準同型を$G/\mathrm{Ker}(f)$に変換します。

主張 (b) は、命題 6 から続きます。$G$ の同値関係 $f(x) = f(y)$ は、$G$ の演算子構造を使用した群と互換性があります。 定理 2 (no. 4) により、形 $y \in xH$ になります。ここで、$H$ は $G$ の通常の安定した部分群であり、$H$ は単位元、よっての類です。 $H = \mathrm{Ker}(f)$。 主張 (a)、(c)、(d) と続きます。 主張 (e) は明らかです (*集合理論*、II, § 6, no. 5)。

### 6. 剰余群中部分群

#### 命題 7 {#alg-i-s4-prop-7 .statement tag=0596}

*$G$と$H$を演算子で2つの群とし、$G$の$f$準同型を$f$の$H$と$N$核にします。
(a) *$H'$を$H$の安定した部分群とする。 $H$で$H'$が正常であれば、$G$では逆像$G' = f^{-1}(H')$が安定した部分群、$G$では$G'$が正常です。さらに$N$は$G'$の通常の部分群です。 $f$ が全射法の場合、$G'/N$ の $H' = f(G')$ と $f$ 定義する同型が移行から商の $H'$ になります。
(b) *$G'$を$G$の安定した部分群とする。 像 $H' = f(G')$ は、$H$ と $f^{-1}(H') = G'N = NG'$ の安定した部分群です。特に、$N \subset G'$ の場合に限り、$f^{-1}(H') = G'$ です。 $f$ が全射法で、$G$ で $G'$ が正規である場合、$H$ では $H'$ が正規です。*

(a) $x$ と $y$ を $G'$ と $\alpha \in \Omega$ に入れる。次に、$f(x) \in H'$ と $f(y) \in H'$、よって $f(xy^{-1}) = f(x)f(y)^{-1} \in H'$、つまり $xy^{-1} \in G'$ です。したがって、$G'$ は $G$ の部分群です。 現在、$f(x^\alpha) = f(x)^\alpha \in H'$、よって $x^\alpha \in G'$ であるため、$G'$ は安定しています。 $H$ では $H'$ が正常であると仮定し、$x \in G', y \in G$ とします。次に $f(x) \in H'$ と
$$
f(yxy^{-1}) = f(y)f(x)f(y)^{-1} \in H'
$$
よって $yxy^{-1} \in G'$;したがって、$G$ では $G'$ が正常です。 すべての $n \in N, f(n) = e \in H'$、よって $N \subset G'$; $N$が$G$では正常であるように、$G'$でも正常です。 最後に、$f$ が全射であれば、
$$
f(f^{-1}(A)) = A \text{ for every subset } A \text{ of } H,
$$
よって $H' = f(G')$; $f$ から $G'$ の制限は $G'$ の準同型 $f'$ から核 $N$ の $H'$ になるため、移行の $f'$ 定義するは、 商同型/$G'/N$ から $H'$ へ。

(b) Let $a$ and $b$ be in $H'$ and $\alpha$ in $\Omega$; there exist $x, y$ in $G'$ with $a = f(x)$ and $b = f(y)$, whence $ab^{-1} = f(xy^{-1}) \in H'$, hence $H'$ is a subgroup of $H$ which is stable, for $a^\alpha = f(x^\alpha) \in H'$. $x \in G$ にしましょう。 $x \in f^{-1}(H')$ は $f(x) \in H' = f(G')$ の場合に限り、つまり $f(x) = f(y)$ を含む $G'$ に $y$ が存在する場合にのみ、 関係 $f(x) = f(y)$ は、$x = yn$ とともに $n \in N$ が存在することと同等です。最後に、$x \in f^{-1}(H')$ は $x \in G'N = NG'$ と同等です。 明らかに、関係 $G' = G'N$ は $G' \supset N$ と同等です。 最後に、$G$ において $f$ が全射法であり、$G'$ が正規であると仮定します。 $a \in H'$ と $b \in H$ としましょう。 $x \in G'$と$y \in G$、$a = f(x)$と$b = f(y)$、よって$bab^{-1} = f(yxy^{-1}) \in f(G') = H'$が存在します。 したがって、$H$ では $H'$ が正常です。

#### 系 1 {#alg-i-s4-prop-7-cor-1 .statement tag=0597}

※$f$が全射であるとします。 Let $\mathscr{G}$ (resp. $\mathscr{G}'$) be the set of stable (resp. normal stable) subgroups of $G$ containing $N$ and $\mathfrak{H}$ (resp. $\mathfrak{H}'$) the set of stable (resp. normal stable) subgroups of $H$, these sets being ordered by inclusion. 写像 $G' \mapsto f(G')$ は、集合同型 $\Phi : \mathscr{G} \to \mathfrak{H}$ の順序です。 逆同型 $\Psi : \mathfrak{H} \to \mathscr{G}$ は写像 $H' \mapsto f^{-1}(H')$ です。 さらに$\Phi$と$\Psi$誘導する同型$\Phi' : \mathscr{G}' \to \mathfrak{H}'$と$\Psi' : \mathfrak{H}' \to \mathscr{G}'$。

#### 系 2 {#alg-i-s4-prop-7-cor-2 .statement tag=0598}

*$f : G \to H$を演算子付きの群の準同型、$N$核の$f$、$G'$を$G$の安定した部分群、$L$を通常の安定した部分群とする$G'$。この場合、$LN, L.(G' \cap N)$ と $f(L)$ は、それぞれ $G'N, G'$ と $f(G')$ の通常安定部分群であり、演算子 $G'N/LN, G'/L.(G' \cap N)$ と $f(G')/f(L)$ を含む 3 つの剰余群は同型です。

$H' = f(G')$と$f'$は、$G'$の$H'$上の一致すると$G'$の$f$の準同型を表します。 $f'$の核は$G \cap N$と$f'(L) = f(L)$です。 命題 7 により、$f'(L)$ は $H'$ の通常の安定した部分群であり、
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N)
$$
$G'$の通常安定の部分群です。 $\lambda$ を $H'/f'(L) = f(G')/f(L)$ 上で $H'$ の標準準同型とする: $\lambda \circ f'$ は核と全射であるため
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N),
$$

$G'/L\cdot(G'\cap N)$ の定義する同型を $f(G')/f(L)$ に移動します。 命題 7、(b)、$f^{-1}(H')=G'N$までに; $f''$が$H'$上の$G'N$の準同型で、$G'N$上の$f$を伴う一致するである場合、$f(G')/f(L)$上の$G'N$の準同型$\lambda\circ f''$は核と全射です。 $f^{-1}(f(L))=LN$;これは、$LN$ が $G'N$ の通常の安定した部分群であり、$G'N/LN$ の $f(G')/f(L)$ に対する $\lambda\circ f''$ 定義する同型であることを証明します。

#### 系 3 {#alg-i-s4-prop-7-cor-3 .statement tag=0599}

$f:G\to H$ を演算子で群の準同型とし、$N$ を核、$X$ 部分集合 $G$ として、$f(X)$ 生成する $H$ および $Y$ とします。 生成する $N$ のうち $N$ の部分集合 。次に、$X\cup Y$ 生成する $N$ です。

$G'$を、$X\cup Y$によって生成された$G$の安定した部分群とします。 $Y\subset G'$、$N\subset G'$として。

$f(X)\subset f(G')$、$f(G')=H$、よって $G'=f^{-1}(H)=G$ として。

#### 注意 {#alg-i-s4-n6-rem-1 .statement tag=059A}

命題 7 の記法では、$H$ の部分群の逆像が $G$ の部分群であるという事実は、次のより一般的な事実から導かれます。

$A$ と $B$ が $H$ の部分集合で、$f$ が全射である場合、

$$
f^{-1}(A\cdot B)=f^{-1}(A)\cdot f^{-1}(B),\qquad
f^{-1}(A^{-1})=f^{-1}(A)^{-1}.
$$

明らかに $f^{-1}(A)\cdot f^{-1}(B)\subset f^{-1}(A\cdot B)$;一方、$z\in f^{-1}(A\cdot B)$ の場合、$f(z)=ab$ となるような $a\in A$ と $b\in B$ が存在します。 $f$ は全射なので、$f(x)=a$ となるような $x\in G$ が存在します。 $y=x^{-1}z$、$f(y)=a^{-1}f(z)=b$、$z=xy$、よって $z\in f^{-1}(A)\cdot f^{-1}(B)$ と書きます。 関係 $x\in f^{-1}(A^{-1})$ は $f(x)\in A^{-1}$、したがって $f(x^{-1})\in A$、つまり $x^{-1}\in f^{-1}(A)$、そして最後に $x\in f^{-1}(A)^{-1}$ と同等です。

#### 命題 8 {#alg-i-s4-prop-8 .statement tag=059B}

$G$ を演算子と $G$ の 2 つの安定した部分群と $A$ と $B$ で群とします。 関係 $a\in A$ と $b\in B$ が $aba^{-1}\in B^{*}$ を暗示しているとします (他の語では、$A$ は $B$ を正規化します) $^{*}$。このとき、$AB=BA$ は $G$ の安定した部分群であり、$A\cap B$ は $A$ の通常の安定した部分群であり、$B$ は $AB$ の通常の安定した部分群です。 $A$の標準単射を移行の$AB$定義するに、$A/(A\cap B)$の商を$AB/B$に同型。

数式

$$
(ab)(a'b')=aa'({a'}^{-1}ba'\cdot b')
$$

$$
(ab)^{-1}=a^{-1}(ab^{-1}a^{-1})
$$

$$
(ab)^\alpha=a^\alpha b^\alpha
$$

$a,a'\in A$、$b,b'\in B$、および$G$ 上のすべての演算子 $\alpha$ について、$AB$ が $G$ の安定した部分群であることを示します。 $a\in A$ と $x\in A\cap B$ としましょう。次に、$A$ と $B$ で立てられた仮説により $axa^{-1}\in B$ となり、明らかに $axa^{-1}$ 属するから $A$ であるため、$A$ では $A\cap B$ が正常です。 $a\in A$ と $b,b'$ を $B$ に含めます。 公式 $(ab)b'(ab)^{-1}=a(bb'b^{-1})a^{-1}$ は、$AB$ では $B$ が正常であることを示します。 $\phi$ を AB/B 上の AB の標準準同型の制限から $A$ とします。すると$\phi(a) = aB$となり、$\phi$の核は$A \cap B$と等しくなります。明らかに $\phi$ は全射なので、$A/(A \cap B)$ の定義する同型は $AB/B$ になります。

#### 定理 4 {#alg-i-s4-thm-4 .statement tag=059C}

*G を演算子付きの群とし、N を G の通常の安定した部分群とします。*

(a) *写像 $G' \mapsto G'/N$ は、G/N の安定部分群の集合上に G 含む N の安定部分群の集合の全単射です。

(b) *$G'$ を G 含む N の安定な部分群とします。$G'/N$ が $G/N$ で正規であるためには、$G'$ が G で正規であり、群 $G/G'$ と $(G/N)/(G'/N)$ が次のようになることが必要十分です。同型。*

(c) *$G'$をGの安定な部分群とします。すると、$G'N$はGの安定な部分群であり、Nは$G'N$で正常です。さらに、$G' \cap N$ は $G'$ で正常であり、群 $G'/(G' \cap N)$ と $G'N/N$ は同型です。*

$f$ が $G/N$ に対する G の標準準同型を表すものとします。すべての $x \in G$、$f(x) \in xN$ について。したがって、G 含む N のすべての部分群 $G'$ に対して $f(G') = G'/N$ です。 $f$ は全射なので、主張 (a) は系 1 から命題 7 に続きます。 同値 "G' ノーマル" $\Leftrightarrow$ "G'/N ノーマル" も同様です。 $G'$ が G 含む N の正規安定部分群であるとします。 no. 4、命題 5 を $\mathrm{Id}_G$ に適用すると、$G/N$ の $G/G'$ に準同型 $u$ が存在します。 $x \in G$全員に対して$u(xN) = xG'$。 $u$が$(G/N)/(G'/N)$の希望同型を$G/G'$に核$G'/N$よってと全射するのが明らかです。最後に、命題 8 の直後に (c) が続きます。

### 7. ジョーダン ホルダー 定理

#### 定義 9 {#alg-i-s4-def-9 .statement tag=059D}

* 演算子 G を使用した群の組成列は、$G_0 = G$ と $G_n = \{e\}$ を伴う G の安定した部分群の有限列 $(G_i)_{0 \leq i \leq n}$ であり、$G_{i+1}$ は $0 \leq i \leq n-1$ に対する $G_i$ の通常の部分群です。 商 $G_i/G_{i+1}$ は系列の商と呼ばれます。 $\Sigma'$から$\Sigma$が系列である場合、組成列$\Sigma'$は組成列$\Sigma$よりより細かいと言われます。

$(G_i)_{0 \leq i \leq n}$ と $(H_j)_{0 \leq j \leq m}$ がそれぞれ、演算子 G と H を使用した 2 つの群の組成列である場合、$m = n$ で、区間の置換 $\phi$ $\mathbf{N}$ の $\{0, n-1\}$ が存在する場合、それらは同等であると言われます。 群と演算子 $G_i/G_{i+1}$ および $H_{\phi(i)}/H_{\phi(i)+1}$ は、すべての $i$ に対して同型です。

一般に、$j > i + 1$ の場合、$G_j$ は通常の $G_i$ の通常の部分群ではないため、組成列 $(G_i)$ から取られた系列は組成列ではないことに注意してください。

#### 定理 5 (シュライヤー) {#alg-i-s4-thm-5 .statement tag=059E}

*Given two composition series $\Sigma_1, \Sigma_2$ of a group with operators G, there exist two equivalent composition series $\Sigma'_1, \Sigma'_2$, finer respectively than $\Sigma_1$ and $\Sigma_2$.

$\Sigma_1 = (H_i)_{0 \leq i \leq n}$ と $\Sigma_2 = (K_j)_{0 \leq j \leq p}$ を組成列にそれぞれ $n + 1$ と $p + 1$ 項を与えた 2 つとします。 組成列 $\Sigma'_1$ は、H_i と H_{i+1} の間に $p - 1$ 部分群 $H'_{i,j}$ (1 \leq j \leq p - 1) を挿入することで形成できることがわかります。0 \leq i \leq n - 1 に対して、n - 1 を挿入することで系列 \Sigma_2' になります。 部分群 K_j と K_{j+1} の間の K_{j,i}' (1 \leq i \leq n - 1) 0 \leq j \leq p - 1;したがって、pn の 2 つの系列 + 安定した G の 1 つの部分群が得られます。挿入された安定な部分群を適切に選択することで、これらの系列が同等の組成列であることを示します。

この目的のために、H_i \cap K_j は H_i と K_j の安定した部分群であるため、 (定理 4) H_{i+1}.(H_i \cap K_j) は H_i 含む H_{i+1} と K_{j+1} の安定した部分群であることに注意してください。(H_i \cap K_j) はK_j 含む K_{j+1} の安定した部分群。 H_{i,j}' = H_{i+1}.(H_i \cap K_j) および K_{j,i}' = K_{j+1}.(H_i \cap K_j) と書くと、H_{i,j+1}' は H_{i,j}' (0 \leq j \leq p - 1) の安定な部分群であり、K_{j,i+1}' は安定なK_{j,i} の部分群 (0 \leq i \leq n - 1)。さらに、H_{i,0}' = H_i、H_{i,p}' = H_{i+1}、K_{j,0}' = K_j、K_{j,p}' = K_{j+1} となります。 定理を示すには、H_{i,j+1}' (それぞれ K_{j,i+1}') が H_{i,j}' (それぞれ K_{j,i}') の正規安定部分群であること、および剰余群 H_{i,j}'/H_{i,j+1}' であることを示すだけで十分です。 K_{j,i}'/K_{j,i+1}' は同型です (0 \leq i \leq n - 1, 0 \leq j \leq p - 1)。これは、H = H_i、H' = H_{i+1}、K = K_j、K' = K_{j+1} とすると、次の補題から導かれます。

#### 補題 1 (ザッセンハウス) {#alg-i-s4-lem-1 .statement tag=059F}

H と K を、演算子 G と H' および K' を使用して、群の 2 つの安定な部分群とし、それぞれ H と K の通常の安定な部分群とします。 H'.(H \cap K') は、H'.(H \cap K) の通常の安定な部分群であり、K'.(K \cap H') は、演算子 (H'.(H \cap K))/(H'.(H \cap K')) および (K'.(K \cap K) を使用した K'.(K \cap H) および剰余群の通常の安定な部分群です。 H))/(K'.(K \cap H')) は同型です。

定理 4 により、H' \cap K = H' \cap (H \cap K) は H \cap K の正規安定部分群になります。同様に、K' \cap H は K \cap H の正規安定部分群です。したがって、 (no. 6, 系 2) (H' \cap K)(K' \cap H) は、H \cap K の通常の安定な部分群です。 定理 4 を群 H に適用すると、

$$
H'.(H' \cap K).(K' \cap H) = H'.(H \cap K')
$$

は、H'.(H \cap K) および剰余群の通常の安定した部分群です。

$$
(H'.(H \cap K))/(H'.(H \cap K))
$$

と同型である

$$
(H \cap K)/((H' \cap K).(K' \cap H)).
$$

最後の商では、一方で H と H'、もう一方で K と K' が対称的に現れます。それらを並べ替えると、記載された結果が得られます。

#### 定義 10 {#alg-i-s4-def-10 .statement tag=059G}

演算子 G を持つ群のジョルダン ヘルダー 系列は真に減少する分解系列 \Sigma であるため、\Sigma と異なる真に減少する分解系列および \Sigma と異なるより細かいは存在しません。

#### 命題 9 {#alg-i-s4-prop-9 .statement tag=059H}

G の分解系列がジョーダン ヘルダー 系列であるためには、系列のすべての商が単純であることが必要かつ十分です。

分解系列は、連続する商が単位元に減らない場合に限り、 真に減少するになります。 真に減少する組成列 $\Sigma$ がヨルダン・ヘルダー 系列ではない場合、$\Sigma$ よりもより細かいであり、$\Sigma$ とは異なる真に減少する組成列 $\Sigma'$ が存在します。したがって、$\Sigma'$ では連続していない $\Sigma$ の 2 つの連続する項 $G_i, G_{i+1}$ があります。 $H$ を、$\Sigma'$ の $G_i$ に続く最初の項とします。 $H$ は、$G_i$、含む $G_{i+1}$ の通常の安定した部分群であり、後者とは異なります。したがって、$H/G_{i+1}$ は、$G_i/G_{i+1}$ の通常の安定した部分群であり、後者や単位元とは異なります。したがって、$G_i/G_{i+1}$ は単純ではありません。逆に、$\Sigma$ が真に減少する組成列で、その商 $G_i/G_{i+1}$ の 1 つが単純ではない場合、この商含むは、それ自体以外の通常の安定した部分群と、その逆像が含まれる $\{e\}$ です。 $G_i$ は、$G_i$ の通常の安定した部分群 $H$ であり、$G_i$ および $G_{i+1}$ (定理 4) とは異なります。 $\Sigma$ ではなく、$\Sigma$ やより細かいとは異なる真に減少する組成列を得るには、$G_i$ と $G_{i+1}$ の間に $H$ を挿入するだけで十分です。

#### 定理 6 (ジョーダン ヘルダー) {#alg-i-s4-thm-6 .statement tag=059I}

*演算子を含む 2 つの Jordan-Hölder 系列の群は同等です。*

Let $\Sigma_1, \Sigma_2$ be two Jordan-Hölder series of a group with operators $G$; by applying Theorem 5 two *equivalent* composition series $\Sigma'_1, \Sigma'_2$ are obtained which are respectively finer than $\Sigma_1$ and $\Sigma_2$; since the latter are Jordan-Hölder series, $\Sigma'_1$ is identical with $\Sigma_1$ or is derived from it by repeating certain terms; the series of quotients of $\Sigma'_1$ is derived from that for $\Sigma_1$ by inserting a number of terms isomorphic to the group $\{e\}$; since $\Sigma_1$ is strictly decreasing, the series of quotients of $\Sigma_1$ is derived from that of $\Sigma'_1$ by suppressing in the latter *all* the terms isomorphic to $\{e\}$. $\Sigma_2$ と $\Sigma'_2$ についても同様です。 $\Sigma'_1$の商の系列と$\Sigma'_2$は、項の位数のみが異なるため（同型まで）、$\Sigma_1$と$\Sigma_2$にも同じことが当てはまります。 定理が証明されました。

#### 系 {#alg-i-s4-n7-cor-1 .statement tag=059J}

*ジョルダン・ヘルダー系列が存在する演算子を使用して、$G$を群とします。 $\Sigma$ が $G$ のいずれかの真に減少する組成列である場合、$\Sigma$ よりもヨルダン・ヘルダー 系列より細かいが存在します。*

$\Sigma_0$ を $G$ のヨルダン・ヘルダー 系列とします。 定理 5 までには、$\Sigma$ と $\Sigma_0$ に相当する 2 つの組成列、$\Sigma'$、$\Sigma'_0$ がそれぞれより細かい存在します。 定理 6 の引数は、$\Sigma'$ からの繰り返しを抑制することで、$\Sigma_0$ と等価な数列 $\Sigma''$ が得られることを示しています。その商はすべて単純 (命題 9) であるため、したがってジョルダン・ヘルダー 系列となります。 $\Sigma$ は真に減少するであるため、$\Sigma''$ は $\Sigma$、よって系よりもより細かいです。

#### 注意 {#alg-i-s4-n7-rem-1 .statement tag=059K}

オペレーター付きの群は必ずしもジョルダン・ヘルダー 系列を所有しているわけではありません。 例は、有理数整数の加法群 $\mathbf{Z}$ によって与えられます。 数列 $(2^n \cdot \mathbf{Z})_{n \geq 0}$ は、$\mathbf{Z}$ の (正規) 部分群の真に減少する無限数列です。すべての $p$、この数列形の最初の $p$ 項と群 $\{0\}$ 真に減少する組成列。 $\mathbf{Z}$ に対してヨルダン・ヘルダー系列が存在した場合、系から定理 6 までに、少なくとも $p+1$ 項が存在することになります。 $p$ は任意なので不合理です。

On the other hand, there exists a Jordan-Hölder series in every *finite* group with operators G: if $G \ne \{e\}$, among the normal stable subgroups of G distinct from G, let $H_1$ be a maximal subgroup; similarly define $H_{n+1}$ by induction as a maximal element in the set of normal subgroups of $H_n$, distinct from $H_n$, when $H_n \ne \{e\}$; the sequence of orders of the $H_n$ is strictly decreasing, hence there exists $n$ such that $H_n = \{e\}$ and the sequence consisting of G and the $H_i$ ($1 \leq i \leq n$) is by its formation a Jordan-Hölder series.

#### 定義 11 {#alg-i-s4-def-11 .statement tag=059L}

演算子を使用して G を群とします。 G の長さは整数 $n$ の上界であるため、G $(G_i)_{0\leq i\leq n}$ の真に減少する組成列が存在します。

G がジョーダン ヘルダー 系列を認める場合、G の長さは、以下の系から定理のように、この系列の連続する商の数です。 6. G がジョルダン ヘルダー 系列を認めない場合、その長さは無限です。 命題 9 により、G のすべての真に減少する系列に対して、厳密により細かい真に減少する系列が存在します。 単位元の群からなるは、長さ零の演算子を持つ唯一の群です。演算子を使用した群は、長さ 1 の場合にのみ単純です。

G を演算子付きの群、H を G の通常の安定な部分群、K 商 G/H および $\pi:G\to K$ 標準準同型とします。させて

$$
\Sigma'=(H_i)_{0\leq i\leq n}
$$

H の分解系列と

$$
\Sigma''=(K_j)_{0\leq j\leq p}
$$

Kの組成列になります。$0\leq i\leq p$には$G_i=\pi^{-1}(K_i)$、$p\leq i\leq n+p$、組成列には$G_i=H_{i-p}$と書きます

$$
\Sigma=(G_i)_{0\leq i\leq n+p}
$$

Ｇが得られる。 $\Sigma$の商の数列は、$\Sigma''$の商の数列と$\Sigma'$の商の数列を並べることで得られます。 $\Sigma'$ と $\Sigma''$ がジョーダン ヘルダー 系列である場合、$\Sigma$ は命題による G のジョルダン ヘルダー 系列です。 9. H または K が任意の長さの組成列を認める場合、G も認められます。

#### 命題 10 {#alg-i-s4-prop-10 .statement tag=059M}

G を演算子付きの群とし、H を G の通常の安定な部分群とします。G の長さは、H および G/H の長さの和です。

#### 系 {#alg-i-s4-n7-cor-2 .statement tag=059N}

演算子と G の $(G_i)_{0\leq i\leq n}$ 組成列を使用して G を群とします。G の長さは、$G_i/G_{i+1}$、$0\leq i\leq n-1$ の長さの和です。

G と $G'$ が演算子付き同型群で、G がジョルダン ヘルダー 系列を認める場合、$G'$ も同様であり、G と $G'$ のジョルダン ヘルダー 系列は等価です。ただし、非同型群は同等の Jordan-Hölder 系列を持つことができます。 $\mathbf{Z}/4\mathbf{Z}$ と $(\mathbf{Z}/2\mathbf{Z})\times(\mathbf{Z}/2\mathbf{Z})$、cf. no. 10 にも同様です。

### 8. 積と食物繊維積

$(G_i)_{i \in I}$ を演算子を持つ群の家族とします。 $G$ を $G_i$ の積モノイドとします。によって定義された $G$ の $\Omega$ の作用を考えてみましょう。

$$
((x_i)_{i \in I})^\alpha = (x_i^\alpha)_{i \in I} \quad (\alpha \in \Omega, x_i \in G_i).
$$

これで構造 $G$ は演算子で群になります。すべての $i \in I$、射影写像 $\mathrm{pr}_i : G \to G_i$ は、演算子を使用すると群の準同型になります。

#### 定義 12 {#alg-i-s4-def-12 .statement tag=059O}

*群演算子* $G = \prod_{i \in I} G_i$ *上記で定義されているのは、* $G_i$ の演算子を持つ積群です。 *写像* $\mathrm{pr}_i : G \to G_i$ *射影準同型と呼ばれます。

A particular case of the product of groups with operators is the group $G^E$ consisting of the mappings of a set $E$ into a group with operators $G$, the laws being defined by:

$$
(fg)(x) = f(x)g(x) \quad (f, g \in G^E, x \in E)
$$
$$
f^\alpha(x) = f(x)^\alpha \quad (f \in G^E, \alpha \in \Omega, x \in E).
$$

$(\phi_i : H \to G_i)_{i \in I}$ を演算子付きの群の準同型の族とする。 The mapping $h \mapsto (\phi_i(h))_{i \in I}$ of $H$ into $\prod_{i \in I} G_i$ is a homomorphism of groups with operators. すべての $i$ に対して、それは唯一の準同型 $\Phi : H \to \prod_{i \in I} G_i$ 満たす $\mathrm{pr}_i \circ \Phi = \phi_i$ です。 これにより、「積群演算子付き」(*集合理論*、IV, § 2, no. 4) という名前が正当化されます。

$(\phi_i : H_i \to G_i)_{i \in I}$ を演算子付きの群の準同型の族とする。 The mapping $\prod_{i \in I} \phi_i : (h_i)_{i \in I} \mapsto (\phi_i(h_i))_{i \in I}$ of $\prod_{i \in I} H_i$ into $\prod_{i \in I} G_i$ is a homomorphism of groups with operators.

#### 命題 11 {#alg-i-s4-prop-11 .statement tag=059P}

*$(\phi_i : H_i \to G_i)_{i \in I}$ * を演算子付きの群の準同型の族とし、* $\Phi = \prod_{i \in I} \phi_i$ とします。 *それから：*

(a) $\mathrm{Ker}(\Phi) = \prod_{i \in I} \mathrm{Ker}(\phi_i)$; *特に、すべての* $\phi_i$ *が単射である場合、$\Phi$ *は単射*です。

(b) $\mathrm{Im}(\Phi) = \prod_{i \in I} \mathrm{Im}(\phi_i)$; *特に、すべての* $\phi_i$ *が全射である場合、$\Phi$ *は全射です*。

明らかです。

特に、$(G_i)_{i \in I}$ を演算子を持つ群の族とし、すべての $i$ について、$H_i$ を $G_i$ の安定 (それぞれ通常の安定) 部分群とします。 積 $\prod_{i \in I} H_i$ は、$\prod_{i \in I} G_i$ の部分群と $\prod_{i \in I} G_i$ の標準写像が、移行から商同型のとき、$\prod_{i \in I} (G_i / H_i)$ 定義するに安定します (それぞれ通常の安定)。
$$
\left( \prod_{i \in I} G_i \right) / \left( \prod_{i \in I} H_i \right)
$$
$\prod_{i \in I} (G_i / H_i)$へ。 たとえば、$J$ を $I$ の部分集合とします。 The subgroup $G_J$ of $\prod_{i \in I} G_i$ consisting of the $(x_i)_{i \in I}$ such that $x_i = e_i$ for $i \notin J$ is a normal stable subgroup. 写像 $\iota_J$ は、$i \notin J$ の場合は $y_i = e_i$、$i \in J$ の場合は $y_i = x_i$ となるように、$x = (x_j)_{j \in J}$ 元 $y = (y_i)_{i \in I}$ に関連付けられており、$\prod_{j \in J} G_j$ の $G_J$ の同型です。 移行から商同型 $\theta_J$ の剰余群 $G / G_J$ が $\prod_{i \in I-J} G_i$ に移行すると、写像 $\mathrm{pr}_{I-J}$ 定義するになります。 合成 $\mathrm{pr}_J \circ \iota_J$ は $\prod_{j \in J} G_j$ の恒等写像です。 $G / G_J$ は、$\theta_J$ により $\prod_{i \in I-J} G_i$ と同一視され、$\prod_{i \in J} G_i$ は $\iota_J$ により $G_J$ と同一視されることがよくあります。

$J_1$ と $J_2$ が $I$ の互いに素部分集合である場合、定義から、$G_{J_1}$ のすべての元は $G_{J_2}$ のすべての元と可換になります。

#### 定義 13 {#alg-i-s4-def-13 .statement tag=059Q}

*$G$ を演算子付きの群とし、$(H_i)_{i \in I}$ を $G$ の通常の安定した部分群のファミリーとします。 $p_i : G \to G / H_i$を標準準同型とします。 準同型 $g \mapsto (p_i(g))_{i \in I}$ が $\prod_{i \in I} G / H_i$ 上の $G$ の同型である場合、$G$ は、剰余群 $(G / H_i)$ のファミリーの内部積 (または積) と呼ばれます*。

$G$と$H$を演算子で群とし、$\phi$と$\psi$を$G$の2つの準同型を$H$にします。 The set of elements $x$ in $G$ such that $\phi(x) = \psi(x)$ is a stable subgroup of $G$, called the *coincidence group* of $\phi$ and $\psi$. 特に、演算子を使用して、$\phi_1 : G_1 \to H$ と $\phi_2 : G_2 \to H$ を群の準同型とします。 準同型 $\phi_1 \circ \mathrm{pr}_1$ と $G_1 \times G_2$ の $\phi_2 \circ \mathrm{pr}_2$ が $H$ になる偶然の群は、$\phi_1$ に対する$H$ 上の$G_1$ と $G_2$ の * 繊維積* と呼ばれます。 $\phi_2$。 $\phi_1$、$\phi_2$、制限、$p_1$、$\mathrm{pr}_1$、$\mathrm{pr}_2$～$G_1 \times_H G_2$の$p_2$を曖昧さのない場合は$G_1 \times_H G_2$と表記し、射影準同型とも呼ばれます。 次に$\phi_1 \circ p_1 = \phi_2 \circ p_2$。 $G_1 \times_H G_2$ の元は、$\phi_1(g_1) = \phi_2(g_2)$ となるように、対 $(g_1, g_2) \in G_1 \times G_2$ が順序付けされています。 If $f_i$ is a homomorphism of a group with operators $K$ into $G_i$ ($i = 1, 2$) and $\phi_1 \circ f_1 = \phi_2 \circ f_2$, there exist one and only one homomorphism $f$ of $K$ into $G_1 \times_H G_2$ such that $f_i = p_i \circ f$ for $i = 1, 2$.

### 9. 制限付き和

$(G_i)_{i \in I}$ を演算子を含む群の族とし、$i \in I$ について、$H_i$ を $G_i$ の安定した部分群とします。 The subset of $\prod_{i \in I} G_i$ consisting of the $(x_i)_{i \in I}$ such that the set of $i \in I$ with $x_i \notin H_i$ is finite is a stable subgroup of $\prod_{i \in I} G_i$ equal to $\prod_{i \in I} G_i$ if $I$ is finite. これは、$H_i$* に対する $G_i$ の *制限付き和と呼ばれます。 有限の数を除くすべての $i$ について、$H_i$ が $G_i$ の通常安定部分群である場合、制限付き和は積の通常安定部分群です。 すべての $i$、部分群 $H_i$ が $G_i$ の単位元、$H_i$ に対する $G_i$ の直和は、単に $G_i$* の *制限付き和と呼ばれ、次のようになります。 ときどきは$\prod_{i \in I} G_i$で示されます。 すべての $i_0 \in I$、写像 $\iota_{i_0}: G_{i_0} \to \prod_{i \in I} G_i$ は、$\iota_{i_0}(x) = (x_i)_{i \in I}$ で定義されます。$i \neq i_0$ の場合、$x_{i_0} = x$ と $x_i = e_i$ は、*標準単射* と呼ばれる演算子を使用した群の単射準同型です。 $G_i$ は安定した部分群 $\operatorname{Im}(\iota_i)$ と同一視されます。 部分群 $G_i$ は正常です。 $i \neq j$、$G_i$、$G_j$の元、通勤、$G_i \cap G_j = \{e\}$の場合。 群 $\prod_{i \in I} G_i$ は集合 $\bigcup_{i \in I} G_i$ によって生成されます。

#### 命題 12 {#alg-i-s4-prop-12 .statement tag=059R}

*Let $(\phi_i: G_i \to K)_{i \in I}$ be a family of homomorphisms of groups with operators such that, for all $i \in I$ and $j \in I$ with $i \neq j$, $x \in G_i$, $y \in G_j$, the elements $\phi_i(x)$ and $\phi_j(y)$ of $K$ commute; there exists one and only one homomorphism of groups with operators $\Phi$ of $\prod_{i \in I} G_i$ into $K$ such that $\phi_i = \Phi \circ \iota_i$ for all $i \in I$. $\prod_{i \in I} G_i$、$\Phi(x) = \prod_{i \in I} \phi_i(x_i)$ の元 $x = (x_i)_{i \in I}$ ごとに。*

$\Phi$ と $\Phi$ が解 ～ 問題の場合、$\bigcup_{i \in I} G_i$ では一致する、したがって $\Phi$ の $\prod_{i \in I} G_i$、よって一意性になります。ここで、$\Phi$ の存在を示します。$\prod_{i \in I} G_i$ のすべての元 $x = (x_i)_{i \in I}$ について、$\Phi(x) = \prod_{i \in I} \phi_i(x_i)$ (§ 1, no. 5) とします。すべての $i$ と $\Phi$ は明らかに $\Phi \circ \iota_i = \phi_i$ で同族性を持っています。 公式 $\Phi(xy) = \Phi(x)\Phi(y)$ は、§ 1, no. 5、公式 (9) から続きます。

#### 定義 14 {#alg-i-s4-def-14 .statement tag=059S}

*$G$ を演算子を持つ群とし、$(H_i)_{i \in I}$ を $G$ の安定した部分群のファミリーとします。 $G$ は、$H_i$ のすべての元が $j \neq i$ の $H_j$ のすべての元と置換可能である場合、部分群 $(H_i)$ のファミリーの内部制限和 (または制限和) と呼ばれます。 $\prod_{i \in I} H_i$ の一意な準同型を $G$ にすると、$H_i$ のそれぞれに対する制限は標準単射になり、同型になります。*

$I$ が有限である場合、言葉の乱用により、内部限定和の代わりに *内部直接積* (または *直接積*、または *積*) とも言います。 G が H の直接の積であり、H' であるような G の安定な部分群 H' が存在する G のすべての安定な部分群 H は、G の *直因子* と呼ばれます。

#### 命題 13 {#alg-i-s4-prop-13 .statement tag=059T}

*G を演算子付きの群と、$H_i$ のすべての元が $j \neq i$ の $H_j$ のすべての元で置換可能であるような G の安定な部分群の族である $(H_i)_{i \in I}$ とします。 G が部分群 $(H_i)_{i \in I}$ の族の制限された和であるためには、G のすべての元 x が形 $\prod_{i \in I} y_i$ で一意に表現可能であることが必要かつ十分です。ここで、$(y_i)_{i \in I}$ は元の有限台を持つ族です。 G のすべての i.* に $y_i \in H_i$

明らかです。

#### 命題 14 {#alg-i-s4-prop-14 .statement tag=059U}

*G を演算子付きの群と、G の安定な部分群の有限族である $(H_i)_{i \in I}$ とします。 G が部分群 $(H_i)$ の族の制限された和であるためには、それぞれの $H_i$ が正規であり、G が以下であることが必要かつ十分です。 剰余群 $(G/H^i)$ の積、ここで、$H^i$ は、$j \neq i$ に対して $H_j$ によって生成された部分群です。*

条件は明らかに必要です。逆に、G が $K_i = G/H^i$ の積であると仮定し、G を $K_i$ の積と識別するとします。次に、$H_i$ は $K_i$ の部分群と同一視されるため、$i \neq j$ では、$H_i$ のすべての元は、$H_j$ のすべての元と置換可能です。一方、$H^i$ は、$j \neq i$ に対する $K_j$ の積と同一視されるため、すべての $i$ に対して $H_i = K_i$ となり、G は $H_i$ の直接の積です。

#### 命題 15 {#alg-i-s4-prop-15 .statement tag=059V}

*演算子を使用して G を群とし、次のような G の通常の安定した部分群と $(H_i)_{1 \leq i \leq n}$ 数列とします*
$$
(H_1 H_2 \ldots H_i) \cap H_{i+1} = \{e\} \quad \text{for } 1 \leq i \leq n-1,
$$
*集合 $H_1 H_2 \ldots H_n$ は、G の通常の安定した部分群、$H_i$ の制限付き和です。

$n$ の帰納法までに、これはすぐに $n = 2$ の証明命題に減ります。まず、$x \in H_1$ と $y \in H_2$ の場合、x と y は *置換可能*であることを示します。 $xyx^{-1}y^{-1} = (xyx^{-1})y^{-1} = x(yx^{-1}y^{-1})$ の場合 ($H_1$ と $H_2$ が正常であるため) $xyx^{-1}y^{-1} \in H_1 \cap H_2$、つまり $xyx^{-1}y^{-1} = e$ は仮定までに計算されます。さらに、$H_1 H_2$ は G の等質性のもとで安定な G の部分集合です。 (no. 3, 命題 1 より) $H_1 H_2$ は G の安定な部分群であることがわかり、この部分群が正規であることがすぐに検証されます。最後に $xy = x'y'$ と $x \in H_1, x' \in H_1, y \in H_2, y' \in H_2$ を仮定します。次に${x'}^{-1}x = y'y^{-1}$、したがって${x'}^{-1} \in H_1 \cap H_2 = \{e\}$、$x' = x$、そして同様に$y' = y$。したがって、$H_1 H_2$ は、$H_1$ と $H_2$ の直接の積です。

群が可換であると考えられる場合、直接の積の代わりに項 *直和* が使用されます。

### 10. 単一種群

$a \in \mathbf{Z}$ にしましょう。 $a\mathbf{Z}$ は $\mathbf{Z}$ の部分群であるため、$\mathbf{Z}$ の元 $x, y$ の間の関係は、「$x - y = az$ が同値関係であるような$z \in \mathbf{Z}$ が存在する」ことを示しており、次のように書くことにきっぱり同意します。 $x \equiv y \pmod{a}$ または $x \equiv y(a)$ で、これは *合同モジュロ* $a$ と呼ばれます。 置き換えること $a$ $-a$ により、等価な関係が得られるため、$a \geqslant 0$ と仮定できます。 $a = 0$ の場合、$x \equiv y(0)$ は $x = y$ を意味するため、等式とは異なる関係は、$a \neq 0$ の場合にのみ取得されます。 したがって、以下では、$a > 0$ 〜でない限りが別の方法で示されていると仮定します。

$a > 0$ に対して、合同式 $x \equiv y(a)$ による $\mathbf{Z}$ の商、つまり群 $\mathbf{Z}/a\mathbf{Z}$ を、$a$ を法とする有理整数の *群と呼びます。

#### 命題 16 {#alg-i-s4-prop-16 .statement tag=059W}

*$a$を整数$> 0$とします。 整数 $r$ は、$\mathbf{Z}$ の同値関係 $x \equiv y \pmod{a}$ の代表者の$0 \leqslant r < a$ 形系となります。*

$x$ が整数 $\geqslant 0$ である場合、$x = aq + r$ $0 \leqslant r < a$ $x \equiv r \pmod{a}$ のように (*集合理論*, III, § 5, no. 6) 整数 $q$ と $r$ が存在します。 $x$ が整数 $\leqslant 0$ である場合、整数 $-x$ は $\geqslant 0$ であり、上記により、$0 \leqslant r < a$ と $-x \equiv r \pmod{a}$ となる整数 $r$ が存在します。 $r = 0$なら$r' = 0$、$r > 0$なら$r' = a - r$と書くと、

$$
x \equiv -r \equiv r' \pmod{a}
$$

そして$0 \leqslant r' < a$。ここで、$0 \leqslant r < r' < a$ の場合は $r \not\equiv r' \pmod{a}$ であることがわかります。現在、$n \geqslant 1$は$r' - r < na$、$n \leqslant 0$は$r' - r > na$、$r' - r \notin a\mathbf{Z}$はよってです。

#### 系 {#alg-i-s4-n10-cor-1 .statement tag=059X}

※$a$を整数$> 0$とします。有理数整数モジュロ $a$ の群 $\mathbf{Z}/a\mathbf{Z}$ は、位数 $a$ の群です。*

#### 命題 17 {#alg-i-s4-prop-17 .statement tag=059Y}

※$\mathrm{H}$を$\mathbf{Z}$の部分群とします。 $\mathrm{H} = a\mathbf{Z}$ となる整数 $a \geqslant 0$ は 1 つだけ存在します。*

$\mathrm{H} = \{0\}$ の場合は、$\mathrm{H} = 0\mathbf{Z}$。 $\mathrm{H} \neq \{0\}$ と仮定します。 部分群 $\mathrm{H}$ には元 $x \neq 0$ があります。次に、$x > 0$ または $-x > 0$、したがって、$\mathrm{H}$ は元 $> 0$ になります。 $a$ を $\mathrm{H}$ の最小の元 $> 0$ とします。 $a$ によって生成された部分群 $a\mathbf{Z}$ は $\mathrm{H}$ に含まれます。 $\mathrm{H} \subset a\mathbf{Z}$ を示します。 $y \in \mathrm{H}$ にしましょう。 命題 16 までに、$y \equiv r \pmod{a}$ と $0 \leqslant r < a$ のような整数 $r$ が存在します。 *なおさら* $y \equiv r \pmod{\mathrm{H}}$、よって $r \in \mathrm{H}$。しかし、これは$r = 0$、つまり$y \in a\mathbf{Z}$の場合にのみ可能です。 整数 $a$ は一意です。$\mathrm{H} = \{0\}$ の場合は必然的に $a = 0$ となり、$\mathrm{H} \neq \{0\}$ の場合、整数 $a$ は $\mathbf{Z}/\mathrm{H}$ の位数です。

#### 定義 15 {#alg-i-s4-def-15 .statement tag=059Z}

*群が単一の元の生成元からなるの系を認める場合、群は単生と呼ばれます。有限の一次群は循環と呼ばれます。*

すべての単次群は可換です (no. 3、系 2 から命題 2)。単次群のすべての剰余群は単次です (no. 3、系 3 ～ 命題 2)。

加法群 $\mathbf{Z}$ は単生です: $\{1\}$ によって生成されます。すべての正の整数 $a$ に対して、群 $\mathbf{Z}/a\mathbf{Z}$ は、$\mathbf{Z}$ の商であるため、単次です。

#### 命題 18 {#alg-i-s4-prop-18 .statement tag=05A0}

*位数 a の有限単次群は $\mathbf{Z}/a\mathbf{Z}$ と同型です。無限単次群は $\mathbf{Z}$ と同型です。*

G を、G の単次群 (乗法で書かれた) と x 生成元とします。恒等式 $x^m x^n = x^{m+n}$ (§ 1, no. 3, 公式 (1)) は、写像 $n \mapsto x^n$ が G の $\mathbf{Z}$ の準同型であることを示します。 像は G 含む x の部分群であるため、G です。 no. 5、定理 3、群により、G は部分群により $\mathbf{Z}$ の商と同型であり、必然的に形 $a\mathbf{Z}$ (命題 17)。 $a > 0$ の場合、群 G は位数 a の有限であり、$a = 0$ の場合、群 G は $\mathbf{Z}$ と同型です。

#### 命題 19 {#alg-i-s4-prop-19 .statement tag=05A1}

*a を整数 > 0 とします。H を $\mathbf{Z}/a\mathbf{Z}$ の部分群、b を H の位数、c を $\mathbf{Z}/a\mathbf{Z}$ の添字とします。次に、$a = bc$、$H = c\mathbf{Z}/a\mathbf{Z}$、H は $\mathbf{Z}/b\mathbf{Z}$ と同型です。

逆に、b と c を 2 整数 > 0 とし、$a = bc$ とします。すると、$a\mathbf{Z} \subset c\mathbf{Z}$ と $c\mathbf{Z}/a\mathbf{Z}$ は、$\mathbf{Z}/a\mathbf{Z}$ の部分群、位数 b と添字 c です。

$a = bc$ no. 4、系から命題 4. no. 7、定理 4 により、H は形 $H'/a\mathbf{Z}$ であり、$H'$ は $\mathbf{Z}$ の部分群であり、 $\mathbf{Z}/H'$ は $(\mathbf{Z}/a\mathbf{Z})/H$ と同型であるため、位数 c. 命題 17 および系から命題 16 まで、$H' = c\mathbf{Z}$ であるため、H は一次です。最後に、H は命題 18 によって $\mathbf{Z}/b\mathbf{Z}$ と同型です。逆に、$a = bc$ の場合、$a \in c\mathbf{Z}$ に対して $a\mathbf{Z} \subset c\mathbf{Z}$ は次のようになります。 剰余群 $(\mathbf{Z}/a\mathbf{Z})/(c\mathbf{Z}/a\mathbf{Z})$ は $\mathbf{Z}/c\mathbf{Z}$ (no. 7, 定理 4) と同型であり、したがって、位数 c (no. 4、系 ～ 命題 4) および添字 b (no. 4、系 ～ 命題 4) になります。

#### 系 {#alg-i-s4-n10-cor-2 .statement tag=05A2}

*単一種群のすべての部分群は単一種です。*

a と b を 2 整数 $\neq 0$ とします。 関係 $b \in a\mathbf{Z}$ は、*b は a* の倍数であり、*割る b* または *は b* の因子とも書かれます。

#### 定義 16 {#alg-i-s4-def-16 .statement tag=05A3}

*整数 $p > 0$ は、$p \neq 1$ の場合に素数と呼ばれ、p 以外の因子 > 1 は認められません。*

#### 命題 20 {#alg-i-s4-prop-20 .statement tag=05A4}

*整数 $p > 0$ は、群 $\mathbf{Z}/p\mathbf{Z}$ が単純な群である場合にのみ素数になります。*

命題 19からの続きです。

#### 系 {#alg-i-s4-n10-cor-3 .statement tag=05A5}

*すべての可換単純群は素数位数の巡回です。*

G をそのような群とします。それから$G \neq \{e\}$; $a \neq e$ を G の元とします。 G が可換であるため、a によって生成された部分群は正規であり、$\{e\}$ に還元されず、したがって G に等しいです。 したがって、G は単次であり、したがって形 $\mathbf{Z}/p\mathbf{Z}$ の群と同型です。 $\mathbf{Z}$ は単純ではなく、$p$ は必ず素数であるため、$p > 0$ です。

#### 注意 {#alg-i-s4-n10-rem-1 .statement tag=05A6}

素数位数の有限群 G は必ず巡回です。 G は G と $\{e\}$ 以外の部分群を認めないため、元 $\neq e$ ごとに生成されます。

#### 補題 2 {#alg-i-s4-lem-2 .statement tag=05A7}

$a$ を整数 $> 0$ とします。 群 $\mathbf{Z}/a\mathbf{Z}$ 数列 $(s_i)_{1 \leq i \leq n}$ のすべての組成列 $(\mathbf{H}_i)_{0 \leq i \leq n}$ と関連付けることにより、$s_i$ は $\mathbf{H}_{i-1}/\mathbf{H}_i$ の位数であり、以下の間で 1 対 1 の対応が得られます。 $\mathbf{Z}/a\mathbf{Z}$ の組成列と整数 $> 0$ の有限列 $(s_i)$ は、$a = s_1 \ldots s_n$ になります。 組成列 $(\mathbf{H}_i)_{0 \leq i \leq n}$ は、$s_i$ が素数である場合に限り、ジョーダン ヘルダー 系列です。

$(\mathbf{H}_i)_{0 \leq i \leq n}$ が $\mathbf{Z}/a\mathbf{Z}$ の組成列である場合、no. 4、命題 4 から $n$ の帰納法により、$a = \prod_{i=1}^n (\mathbf{H}_{i-1} : \mathbf{H}_i)$ になります。

逆に、$(s_i)_{1 \leq i \leq n}$ を整数 $> 0$ の数列として、$a = s_1 \ldots s_n$ とします。 $(\mathbf{H}_i)_{0 \leq i \leq n}$ が $\mathbf{Z}/a\mathbf{Z}$ の組成列で、$1 \leq i \leq n$ が $(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$ である場合、$i$、よって $\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$ の帰納法に見られるように、必然的に $((\mathbf{Z}/a\mathbf{Z}) : \mathbf{H}_i) = \prod_{1 \leq j \leq i} s_j$ になります。 (命題 19)、これは問題の写像の単射性を示しています。ここでその主観性を示します。 $0 \leq i \leq n$に$\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$を書くと、$\mathbf{Z}/a\mathbf{Z}$の組成列は$(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$(命題19)となります。 2 番目の主張は、命題 20 と no. 7、命題 9 に続きます。

$\mathfrak{P}$ を素数数の集合とします。

#### 定理 7 (分解を素数因子) {#alg-i-s4-thm-7 .statement tag=05A8}

*$a$ を厳密には正の整数とします。 $p \in \mathfrak{P}$ と $v_p(a) \neq 0$ の集合が有限であるような、整数 $> 0$ の家族 $(v_p(a))_{p \in \mathfrak{P}}$ が 1 つだけ存在し、*

$$
a = \prod_{p \in \mathfrak{P}} p^{v_p(a)}.
$$

群 $\mathbf{Z}/a\mathbf{Z}$ は有限なので、ヨルダン・ヘルダー 系列が認められます。 補題 2 は、$a$ が素数整数の積、よって族 $(v_p(a))$ の存在を意味します。さらに、すべての家族について、定理 7 の $(v_p(a))_{p \in \mathfrak{P}}$ 満たす条件、整数 $v_p(a)$ は、すべての $p \in \mathfrak{P}$ に対して、ヨルダン・ヘルダーの因子の数系列に等しくなります。 $\mathbf{Z}/a\mathbf{Z}$ は $\mathbf{Z}/p\mathbf{Z}$ (補題 2) と同型です。したがって、家族 $(v_p(a))$ の一意性は、ヨルダン・ヘルダー 定理 (no. 7, 定理 6) から続きます。

#### 系 {#alg-i-s4-n10-cor-4 .statement tag=05A9}

※$a$と$b$を2つの整数$> 0$とします。それから$v_p(ab) = v_p(a) + v_p(b)$。 $a$ から割る $b$ については、すべての素数数 $p$ に対して $v_p(a) \leq v_p(b)$ であることが必要かつ十分です。*

任意の群 $G$ において、元 $x \in G$ によって生成された (単次) 部分群が有限位数 $d$ である場合、$x$ は *位数* の元と呼ばれます。 $d$;したがって、数 $d$ は、$x^d = e$ となる最小の整数 $> 0$ です。 $x$ によって生成された部分群が無限である場合、$x$ は *無限位数* であると言われます。これらの定義は、命題 4 (no. 4) とともに、特に有限群 G では、G のすべての元の位数が G の位数の因子であることを意味します。

#### 命題 21 {#alg-i-s4-prop-21 .statement tag=05AA}

位数 n の有限群 G では、すべての $x \in G$ に対して $x^n = e$ です。

$p$ が $x$ の位数である場合、$n = pq$、$q$ 整数であるため、$x^n = (x^p)^q = e$ となります。

### 練習問題 {#alg-i-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
