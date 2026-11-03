---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 1
section_title: Uniform spaces
lang: ja
source: top-i-iv
book_pages: 169-174, 206-207
pdf_pages: 0175-0180, 0212-0213
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A UNIFORM STRUCTURE
      page: 169
      pdf_page: 175
    - "no": 2
      title: TOPOLOGY OF A UNIFORM SPACE
      page: 171
      pdf_page: 177
statements: 14
exercises: 5
content_sha256: af4cca2a1c77a3757a62b61ed71ea51cd1efc89f19f18197f836132d3e1e1499
translated_from: content/en/top/II/01_s1_uniform_spaces.md
translation_method: google
source_content_sha256: 0fd087b92f4bcb3cb8327201790fedf19f1e8b4d6d6fa498400dbc46a4cbcd83
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1e5bc32fb82f81febab89f2e604aa70a18f90a195905a11212eb165516098a33
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 制服空間

### 1. 定義ユニフォーム構造

#### 定義 1 {#top-ii-s1-def-1 .statement tag=0BCY}

*均一な構造* (または *均一性*) *集合上* $X$ *集合* $\mathfrak{U}$ *の部分集合の* $X \times X$ *公理* $(\mathrm{F}_1)$ *および* $(\mathrm{F}_{\mathrm{II}})$ *I, § 6, no. 1章の公理を満たし、次の公理*も満たします。

(U₁) *集合所属から* $\mathfrak{U}$ *含む対角線* $\Delta$ まで。

(U₂) *もし* $V \in \mathfrak{U}$ *その後* $\overline{V}^{-1} \in \mathfrak{U}$。

(U₃) *それぞれ* $V \in \mathfrak{U}$ *存在します* $W \in \mathfrak{U}$ *そのような* $W \circ W \subset V$。

![図2](../images/chapter_ii_uniform_structures.png)

$\mathfrak{U}$ の集合は、$X$ によって $\mathfrak{U}$ で定義された均一性の取り巻きと呼ばれます。均一性を持たせた集合を制服空間と呼びます。

$V$が$X$の一様性の取り巻きである場合、関係$(x, x') \in V$をというで「$x$と$x'$が$V$に近い」と表現できます。

#### 注意 1 {#top-ii-s1-n1-rem-1 .statement tag=0BCZ}

言語をより表現力豊かにするために、一部の主張では「$x$ は $y$ に十分近い」や「$x$ と $y$ は好きなだけ近い」という表現を使用することがあります。たとえば、関係とします。

R $\{ x, y \}$ は、関係 $(x, y) \in V$ が $R \{ x, y \}$ を暗示するような取り巻き $V$ が存在する場合、$x$ と $y$ が十分に近いときはいつでも true です。

#### 注意 2 {#top-ii-s1-n1-rem-2 .statement tag=0BD0}

公理 (U_{II}) と (U_{III}) の論理積は、(他の公理が一様構造であると仮定して) 次の公理と等価です。

(U_a) それぞれの $V \in \mathfrak{U}$ に対して、$W \circ \overline{W} \subset V$ となるような $W \in \mathfrak{U}$ が存在します (*)。

明らかに (U_{II}) と (U_{III}) は (U_a) を暗示しています。逆に、(U_a) が満たされる場合、(U_I) によって $\overline{W} = \Delta \circ W \subset V$ が得られます。したがって $W \subset \overline{V}$、したがって [by (F_1)] $\overline{V} \in \mathfrak{U}$。 $W' = W \cap \overline{W}$ にしましょう。次に、今証明されたことと公理 (F_{II}) により $W' \in \mathfrak{U}$ となり、$W' \circ W' \subset W \circ \overline{W} \subset V$ が得られます。

この章を通して、$V \circ V$ の代わりに $\overline{V}^2$ と書き、一般的には整数 $n > 1$ と $X \times X$ の各部分集合 $V$ に対して $\overline{V}^{n-1} = \overline{V} \circ V = V \circ \overline{V}^{n-1}$ と書きます。

#### 注意 3 {#top-ii-s1-n1-rem-3 .statement tag=0BD1}

$X$ が空でない場合、公理 (U_I) は、$\mathfrak{U}$ の集合が空ではないことを意味するため、$\mathfrak{U}$ は $X \times X$ のフィルターになります。空の集合には均一性が 1 つだけあり、つまり $\mathfrak{U} = \{ \emptyset \}$ です。

#### 定義 2 {#top-ii-s1-def-2 .statement tag=0BD2}

均一性の側近の基本的な系は、すべての側近含む集合所属から $\mathfrak{B}$ となるような側近の任意の集合 $\mathfrak{B}$ です。

公理 (U_{III}) は、$n$ が任意の整数 $> 0$ であり、$V$ が側近の基本系を通る場合、集合 $\overline{V}^n$ が再び形側近の基本系になることを示しています。

$V = \overline{V}^1$ のような取り巻き $V$ は対称と呼ばれます。 $V$ が取り巻きである場合、$V \cap \overline{V}^1$ と $V \cup \overline{V}^1$ は対称取り巻きであり、公理 (F_{II}) と (U_{II}) は、対称取り巻き形が取り巻きの基本系であることを示しています。

$X \times X$ の部分集合の集合 $\mathfrak{B}$ は、$\mathfrak{B}$ が章 I, § 6, no. 3 の公理 (B_I) を満たし、かつ以下も満たす場合に限り、$X$ における一様性の取り巻きの基本系です。公理:

(U'_I) $\mathfrak{B}$含むの集合ごとに対角$\Delta$。

(U'_II) それぞれの $V \in \mathfrak{B}$ に対して、$V' \subset \overline{V}^1$ となるような $V' \in \mathfrak{B}$ が存在します。

(U'_III) それぞれの $V \in \mathfrak{B}$ に対して、$\overline{W}^2 \subset V$ となるような $W \in \mathfrak{B}$ が存在します。

$X$ が空でない場合、$X$ の制服構造の側近の基本系は、この構造の側近によって形成されるフィルターの基底 (章 I, § 6, no. 3, 命題 3) です。

(*) (集合理論、R、§ 3、番号 4 と 10) を思い出してください。$V$ と $W$ が $X \times X$ の 2 つの部分集合である場合、対 $(x, y) \in X \times X$ の集合は次のようになります。一部の$z \in X$の$(x, z) \in W$と$(z, y) \in V$は$V \circ W$または$VW$で表され、対$(x, y) \in X \times X$の集合は$(y, x) \in V$が$\overline{V}^1$で表されます。

例の均一性。 \* 1) 実数の集合 $\mathbf{R}$ では、*加法均一性* と呼ばれる均一性定義するを次のようにすることができます。各 $\alpha > 0$ について、$V_\alpha$ をすべての $\mathbf{R} \times \mathbf{R}$ からなるの部分集合とします。 対 $(x, y)$ は $|x - y| < \alpha$ になります。 $\alpha$ はすべての実数 $> 0$ の集合を通過するため、$V_\alpha$ 形は$\mathbf{R}$ での加法的均一性のための基本的な取り巻きの系です。同様に、有理数数の集合 $\mathbf{Q}$ で均一性 (これも *加法均一性 * と呼ばれます) を定義する求めることができます。これらの構造と、*群*、章 III および IV の類似の制服構造を学習します。 \*
2) $X$ を集合とし、$R$ を $X$ の *同値関係* とします。 $C$を$X \times X$の$R$のグラフとします。次に$\Delta \subset C$と$\overset{2}{C} = \overset{-1}{C} = C$。 (*集合理論、R、§ 5, no. 1*);したがって、集合 $C$ のみで構成される $X \times X$ の部分集合の集合は、$X$ における統一性の側近の基本的な系です。特に、$R$ を等式の関係とすると、$C = \Delta$ と対応するの取り巻きは *すべて $X \times X$ の部分集合* であり、含む $\Delta$ です。この均一性は $X$ の *離散* 均一性と呼ばれ、この均一性を備えた集合 $X$ は *離散均一空間* と呼ばれます。
3) 有理数整数の集合 $\mathbf{Z}$ では、数の理論で重要な均一性定義するができます。素数数 $p$ が与えられた場合、$W_n$ をすべての集合とします対 $(x, y) \in \mathbf{Z} \times \mathbf{Z}$ は、整数 $n > 0$ ごとに $x \equiv y \pmod{p^n}$ になります。 集合 $W_n$ (固定 $p$ の場合) 形が、*$p$ 進数* の均一性 (cf. 章) と呼ばれる、$\mathbf{Z}$ 上の均一性の取り巻きの基本系であることは簡単に検証されます。 III, § 6、練習問題 23以降、および章 IX, § 3, no. 2）。

一般的な定義 (*集合理論、R、§ 8, no. 5*) に従って、$X$ と $X'$ がそれぞれ均一性を備えた 2 つの集合であり、側近の集合が $U$ と $U'$ であるとします。それぞれ、$X$ の $X'$ に対する全単射 $f$ は、$g(U) = U'$ の場合、$X'$ の均一性に対する $X$ の均一性の *同型* です。ここで、$g = f \times f$ です。

たとえば、$X$ と $X'$ が 2 つの等電位集合である場合、$X'$ 上の$X$ のすべての全単射は、$X'$ の離散均一性に対する $X$ の離散均一性の同型になります。

### 2. 位相ユニフォーム空間

#### 命題 1 {#top-ii-s1-prop-1 .statement tag=0BD3}

*Let $X$ be 集合 endowed with a uniform 構造 $U$, and for each $x \in X$ let $\mathfrak{B}(x)$ be 集合 of 部分集合 $V(x)$ of $X (*)$, where $V$ runs through $U$の取り巻きの集合。次に、$X$ には一意の位相があり、それぞれの $x \in X$、$\mathfrak{B}(x)$ は、この位相の $x$ の近傍フィルターになります。

章 I, § 1, no. 2 の $\mathfrak{B}(x)$ 満たす条件 (V_I)、(V_{II})、(V_{III})、および (V_{IV}) であることを示さなければなりません。最初の 3 つがそうだということは、

(*) We recall (*集合理論, R, § 3, no. 7*) that if $V$ is any 部分集合 of $X \times X$ and $x$ is any 元 of $X$, then $V(x)$ denotes $y \in X$ のうち集合は $(x, y) \in V$ になります。

これらの条件は、$\mathfrak{U}$ 満たす $(\mathbf{F}_I),\ (\mathbf{F}_{II})$ および $(\mathbf{U}_I)$ の側近であるという事実からすぐに続きます。 $(\mathbf{V}_{IV})$ に関しては、$V$ を $\mathfrak{U}$ の取り巻き、$W$ を $\mathfrak{U}$ の取り巻きとし、$\dot{W} \subset V$ とします。次に、$(x, y) \in W$ と $(y, z) \in W$ の場合、$(x, z) \in V$ があり、すべての $y \in W(x)$ に対して $W(y) \subset V(x)$、したがってすべての $y \in W(x)$ に対して $V(x) \in \mathfrak{B}(y)$ となります。これで証明は完了です。

#### 定義 3 {#top-ii-s1-def-3 .statement tag=0BD4}

* 命題 1 で定義された位相は、制服構造 $\mathfrak{U}$ により位相と呼ばれます。

#### 例 1 {#top-ii-s1-n2-exa-1 .statement tag=0BD5}

実数の集合の加法均一性によって引き起こされる位相は、実直線の位相(章I, § 1, no. 2)です。同様に、有理線数の集合上の加法的一様性によって引き起こされる位相は、有理直線の位相です。

#### 例 2 {#top-ii-s1-n2-exa-2 .statement tag=0BD6}

離散均一性 (no. 1、例 2) によって引き起こされる任意の集合 $X$、位相では、離散位相になります。

In the future, when we speak of 位相 of a uniform 空間 $X$, we shall always mean 位相 induced by the uniform 構造 of 空間, 〜でない限り the contrary is expressly stated. The topological 空間 obtained by putting this 位相 on 集合 $X$ is ときどき called the topological 空間 *underlying* the uniform 空間 in question. For example, when we say that a uniform 空間 is *Hausdorff*, or *compact*, or *locally compact*, etc., we mean that the underlying topological 空間 has this 性質.

If $X$ and $X'$ are two uniform 空間, any 同型 $f$ of the uniform 構造 of $X$ onto that of $X'$ is also a *homeomorphism* of $X$ onto $X'$; $X$ は、ユニフォーム空間 $X$ をユニフォーム空間 $X'$ に *同型* したものであると言います。 It should be noted that a homeomorphism of $X$ onto $X'$ is not necessarily 同型 of the uniform 構造 of $X$ onto that of $X'$.

他の語では、同じ集合 $X$ 上の *明確な * 均一性が誘導する同じ位相になる可能性があります。 *For example, on ]0, +∞[, the *additive* and the *multiplicative* uniformities (which are distinct : 章 III, § 6, 練習問題 17) 誘導する the same 位相.*
他の例については、§ 2, no. 2、注意 1 を参照してください。

#### 命題 2 {#top-ii-s1-prop-2 .statement tag=0BD7}

※$X$を制服空間とします。 $X$ のすべての対称取り巻き $V$ と $X \times X$ のすべての部分集合 $M$ について、$VMV$ は積空間 $X \times X$ の $M$ の近傍であり、この空間の $M$ は公式* によって与えられます

$$
\overline{M} = \bigcap_{V \in \mathscr{S}} VMV
$$

*ここで、$\mathscr{S}$は$X$の対称的な取り巻きの集合を表します。*

$V$ を $X$ の対称な取り巻きとする。 関係 $(x, y) \in VMV$ は、$(x, p) \in V$ と $(q, y) \in V$ のような $M$ の元 $(p, q)$ が存在することを意味します。他の語 ($V$ は対称です) $x \in V(p)$ と $y \in V(q)$ には、 $(x, y) \in V(p) \times V(q)$です。 $V(p) \times X(q)$は$X \times X$の$(p, q)$の近傍なので、命題の最初の部分が証明されます。 関係 $(x, p) \in V, (y, q) \in V$ は、$p \in V(x), q \in V(y)$ または $(p, q) \in V(x) \times V(y)$ と書くこともできます。 $V$ が $\mathscr{S}$ を通過するため、集合 $V(x) \times V(y)$ 形は $X \times X$ の $(x, y)$ の近傍の基本的な系です。なぜなら、$U, U'$ が任意の 2 つの取り巻きである場合、常に対称的な取り巻き $V \subset U \cap U'$ が存在するため、$V(x) \times V(y) \subset U(x) \times U'(y)$ となるからです。したがって、$(x, y) \in \overline{M}$ が続き、公式 (1) が続く場合に限り、$V(x) \times V(y)$ は各 $V \in \mathscr{S}$ に対して $M$ と一致します。

#### 系 1 {#top-ii-s1-prop-2-cor-1 .statement tag=0BD8}

*$A$ が $X$ のいずれかの部分集合で、$V$ が $X$ の対称的な取り巻きである場合、$V(A)$ は $X$ の $A$ の近傍であり、*

$$
\overline{A} = \bigcap_{V \in \mathscr{S}} V(A) = \bigcap_{U \in \mathfrak{U}} V(A)
$$

*ここで、$\mathfrak{U}$は$X$のすべての取り巻きのうち集合を表します。*

$M = A \times A$ の場合、$V \in \mathscr{S}$ に対しては $VMV = V(A) \times V(A)$。 関係について、「$(x, p) \in V$ となるような$p \in A$ が存在する」は、定義により$x \in V(A)$ と等価です。 系は、章 I, § 4, no. 2、命題 5、no. 3、命題 7 に続きます。

$V(A)$ は、* $A$ の*V 近所であると言われています。

$V$ が $X \times X$ で *オープン* な側近である場合、$V(x)$ は $x \in X$ (章 I, § 4, no. 2、系から命題 4) に対して $X$ でオープンであるため、$V(A)$ となります。 $x$ が $A$ を通過するため、$V(x)$ の和集合は、$X$ に *オープン* します。一方、$V$ が $X \times X$ で閉じられた側近である場合、$X$ (練習問題 3) のすべての部分集合 $A$ について、$V(A)$ が $X$ で閉じられる必要はありません。

また、$V$ が$X$ の側近の集合を通過するため、集合 $V(A)$ が$X$ の$A$ の基本的な近傍システムを形成するとは限らないことにも注意する必要があります (練習問題 2)。

#### 系 2 {#top-ii-s1-prop-2-cor-2 .statement tag=0BD9}

*$X \times X$ 形の $X$ の側近の内部 (それぞれクロージャ) $X$ の側近の基本的な系。

$V$ が $X$ の取り巻きである場合、$W \subset V$ のような対称的な取り巻き $W$ が存在します。 $W$ は $W$ (命題 2) の近傍であるため、$X \times X$ 含む $W$ の $V$ の内部であり、従って取り巻きです。さらに、命題 2 までに $W \subset W \subset W \subset V$ があるため、$V$ 含むで側近が終了します。

#### 系 3 {#top-ii-s1-prop-2-cor-3 .statement tag=0BDA}

*すべてのユニフォーム空間は公理* $(O_{III})$ を満たします。

$x$ が $X$ のいずれかの点であり、$V$ が $X \times X$ で閉じられた$X$ の取り巻きを通過する場合、集合 $V(x)$ 形は、近傍の基本系になります。 $X$の$x$は系2まで、$X$には閉店します（章I、no. 2、系から命題4）

#### 命題 3 {#top-ii-s1-prop-3 .statement tag=0BDB}

*制服空間 $X$ は、その制服構造のすべての取り巻きのうち共通部分が $X \times X$ の対角線 $\Delta$ である場合に限り、ハウスドルフです。ハウスドルフのユニフォーム空間はすべてレギュラーです。*

後者の主張は、系 3から命題 2のすぐ後に続きます。閉じた取り巻き形が取り巻きの基本的な系（命題2、系2）であることがわかりました。それらの共通部分が $\Delta$ の場合、$\Delta$ は $X \times X$ で閉じられ、その結果、$X$ はハウスドルフ (章 I, § 8, no. 1, 命題 1) になります。逆に、$X$ がハウスドルフの場合、点 $(x, y) \notin \Delta$ ごとに、$y \notin V(x)$ または同等の $(x, y) \notin V$ となるような $X$ の側近 $V$ が存在します。したがって、$\Delta$ は側近全員の共通部分になります。

制服空間 $X$ がハウスドルフである場合、$X$ の制服構造は *ハウスドルフ* と言います。 $\mathfrak{B}$ がこの構造の側近の基本系である場合。この場合、$\mathfrak{B}$ のすべての集合のうち共通部分が $\Delta$ である場合に限り、$X$ はハウスドルフになります。

### 練習問題 {#top-ii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
