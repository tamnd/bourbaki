---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 6
section_title: Filters
lang: ja
source: top-i-iv
book_pages: 57-68
pdf_pages: 0063-0074, 0135-0138
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A FILTER
      page: 57
      pdf_page: 63
    - "no": 2
      title: COMPARISON OF FILTERS
      page: 58
      pdf_page: 64
    - "no": 3
      title: BASES OF A FILTER
      page: 59
      pdf_page: 65
    - "no": 4
      title: ULTRAFILTERS
      page: 60
      pdf_page: 66
    - "no": 5
      title: INDUCED FILTER
      page: 61
      pdf_page: 67
    - "no": 6
      title: DIRECT IMAGE AND INVERSE IMAGE OF A FILTER BASE
      page: 62
      pdf_page: 68
    - "no": 7
      title: PRODUCT OF FILTERS
      page: 63
      pdf_page: 69
    - "no": 8
      title: ELEMENTARY FILTERS
      page: 64
      pdf_page: 70
    - "no": 9
      title: GERMS WITH RESPECT TO A FILTER
      page: 65
      pdf_page: 71
    - "no": 10
      title: GERMS AT A POINT
      page: 68
      pdf_page: 74
statements: 30
exercises: 20
content_sha256: 606f18e070a6ddb077779e7e5a87379df4840823017ddcd6c77a3246eb392fa8
translated_from: content/en/top/I/06_s6_filters.md
translation_method: google
source_content_sha256: a165a0f76eeee4bd4e5a4290b8617a33d4316a02017e4b95b814435276231fc9
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1a49e7951f363118e65075c00401fae020972a8d8a206f33c854a195ecded2f5
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 6. フィルター

### 1. フィルターの定義

#### 定義 1 {#top-i-s6-def-1 .statement tag=0B3X}

*集合 $X$ のフィルターは、$X$ の部分集合の集合 $\mathfrak{F}$ であり、次のプロパティがあります:*

$(\mathrm{F}_1)$ *$X$の部分集合、$\mathfrak{F}$属するの含む集合から$\mathfrak{F}$まで*。
$(\mathrm{F}_\mathrm{II})$ *有限の共通部分、集合、$\mathfrak{F}$、属するから$\mathfrak{F}$まで*。
$(\mathrm{F}_\mathrm{III})$ *空の集合は $\mathfrak{F}$ にはありません。*

$(\mathrm{F}_\mathrm{II})$ と $(\mathrm{F}_\mathrm{III})$ から、$\mathfrak{F}$ の集合のすべての有限共通部分は *空ではない* ことがわかります。

$X$ 定義する構造 $X$ のフィルター $\mathfrak{F}$、その公理は $(\mathrm{F}_1)$、$(\mathrm{F}_\mathrm{II})$、$(\mathrm{F}_\mathrm{III})$ です。この構造はフィルターされた集合* の *構造と呼ばれ、この構造を備えた集合 $X$ は * $\mathfrak{F}$ でフィルターされた *集合と呼ばれます。

公理 $(\mathrm{F}_\mathrm{II})$ は、次の 2 つの公理の結合と同等です。
$(\mathrm{F}_{\mathrm{II}\,\mathrm{a}})$ *共通部分の 2 集合 $\mathfrak{F}$ 属するから $\mathfrak{F}$。*
$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ *$X$ 属するから $\mathfrak{F}$.*

公理 $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ と $(\mathrm{F}_\mathrm{III})$ は、*空の集合* にはフィルターがないことを示しています。

$(\mathrm{F}_1)$ を満たし、満たす $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ を満たす部分集合の集合に対する位数では、それが*空ではない*ことが必要十分です。 $(\mathrm{F}_1)$を満たす部分集合の集合は、$\mathfrak{P}(X)$と異なる場合に限り、$(\mathrm{F}_\mathrm{III})$も満たします。

*フィルタの例* 1) $X \neq \varnothing$ の場合、$X$ のみからなるサブセットのセットが $X$ のフィルタになります。 より一般的には、$X$ の指定された空でないサブセット $A$ を含む $X$ のすべてのサブセットのセットは、$X$ のフィルターになります。

2) トポロジー 空間 $X$ では、任意の空でない部分集合 $A$ の $X$ のすべての近傍* の *集合 (特に、すべての近傍の点の集合) $X$) は、$A$ の *近傍フィルター* と呼ばれるフィルターです。

3) $X$ が *無限* 集合の場合、$X$ の有限部分集合* の *補数はフィルターの元です。 有限部分集合 of 集合 $\mathbf{N}$ of 整数 $\geqslant 0$ の補数のフィルタを *Fréchet フィルタ * と呼びます。

### 2. フィルターの比較

#### 定義 2 {#top-i-s6-def-2 .statement tag=0B3Y}

同じ集合 $X$ に 2 つのフィルター $\mathfrak{F}, \mathfrak{F}'$ があるとすると、$\mathfrak{F}'$ は $\mathfrak{F}$ よりもより細かいであるか、$\mathfrak{F} \subset \mathfrak{F}'$ の場合、$\mathfrak{F}$ は$\mathfrak{F}'$ より粗いと言えます。 $\mathfrak{F} \neq \mathfrak{F}'$ もある場合、$\mathfrak{F}'$ は$\mathfrak{F}$ より厳密により細かい、または$\mathfrak{F}'$ より厳密に$\mathfrak{F}$ 粗いといわれます。

2 つのフィルターは、一方が他方よりより細かいであれば同等であると言われます。 $X$ のすべてのフィルターの集合は、関係によって順序付けされます。「$\mathfrak{F}$ は $\mathfrak{F}'$ より粗い」。この関係は、$\mathfrak{P}(\mathfrak{P}(X))$ に関係が含まれることによって引き起こされます。

$(\mathfrak{F}_i)_{i \in I}$ を、集合 $X$ 上の空でないフィルタのファミリとします (したがって、空ではない必要があります)。それから集合

$$
\mathfrak{F} = \bigcap_{i \in I} \mathfrak{F}_i
$$

公理 $(F_I), (F_{II})$ および $(F_{III})$ を満たすため、フィルターになります。 $\mathfrak{F}$ は、フィルター ファミリー $(\mathfrak{F}_i)_{i \in I}$ の共通部分と呼ばれ、$X$ のすべてのフィルターの順序付けられた集合の $\mathfrak{F}_i$ の集合の最大の下界であることは明らかです。

単一の集合 $X$ によって形成されるフィルターは、$X$ のすべてのフィルターの順序付けられた集合の最小の元です。 no. 4 で、$X$ に複数の元がある場合、$X$ のすべてのフィルターの集合には最大の元がないことがわかります。

集合 $X$ の部分集合の集合 $\mathfrak{G}$ が与えられた場合、含む $\mathfrak{G}$ である $X$ にフィルタがあるかどうかを考えてみましょう。そのようなフィルターが存在する場合、$(F_{II})$ により、含むは、$\mathfrak{G}$ の集合の有限共通部分の集合 $\mathfrak{G}'$ (空の部分集合の共通部分である$X$ を含む) $\mathfrak{G}$);したがって、そのようなフィルターが存在するために必要な条件は、$X$ の空の部分集合が $\mathfrak{G}'$ に存在しないことです。この条件は、含む $\mathfrak{G}'$ も含む集合 $\mathfrak{G}''$ of 部分集合 of $X$ 含む集合の$(F_I)$ までに十分です。 $\mathfrak{G}'$。ここで、$\mathfrak{G}''$ は明らかに $(F_I)$ を満たします。 $\mathfrak{G}'$ の定義により、$(F_{II})$ を満たします。そして、$X$ の空の部分集合が属するから $\mathfrak{G}'$ にならないため、最終的に $(F_{III})$ が満たされます。したがって、$\mathfrak{G}''$ は含む $\mathfrak{G}$ よりも粗いフィルタであり、次のことが証明されました。

#### 命題 1 {#top-i-s6-prop-1 .statement tag=0B3Z}

$X$ の部分集合の $X$ 含む集合 $\mathfrak{G}$ にフィルタが存在するために必要かつ十分な条件は、$\mathfrak{G}$ の有限部分集合に空の共通部分がないことです。

上記で定義されたフィルター $\mathfrak{G}''$ は $\mathfrak{G}$ によって生成されると言われ、 $\mathfrak{G}$ は $\mathfrak{G}''$ のサブベースであると言われます。

#### 例 {#top-i-s6-n2-exa-1 .statement tag=0B40}

$\mathscr{S}$ を集合 $X$ の部分集合のいずれかの集合とし、$\mathfrak{T}$ を $\mathscr{S}$ ($\S$ 2、no. 3、例) によって生成された $X$ の位相とします。 II）。 $\mathscr{S}$の集合の有限共通部分の集合は$\mathfrak{T}$の基底であるため、上記の命題1の証明と$\S$1の命題3から、 no. 3、$\mathfrak{T}$ の $x$ 近傍の各$x \in X$ 近傍フィルターは、$\mathscr{S}$ の集合の集合 $\mathfrak{G}(x)$ と含む $x$ によって生成されます。

#### 系 1 {#top-i-s6-prop-1-cor-1 .statement tag=0B41}

$\mathfrak{F}$ を $X$ の集合 $X$ と $A$ 部分集合のフィルターとします。次に、$\mathfrak{F}$ よりもより細かいであるフィルター $\mathfrak{F}'$ があり、$A$ が $\mathfrak{F}$ のすべての集合を満たす場合に限り、$A \in \mathfrak{F}'$ になります。

#### 系 2 {#top-i-s6-prop-1-cor-2 .statement tag=0B42}

空ではない集合 $X$ のフィルターの集合 $\Phi$ は、元のすべての有限列 $(\mathfrak{F}_i)_{1 \leq i \leq n}$ について、$X$ のすべてのフィルターの集合に少なくとも上界が含まれています。 $\Phi$ とすべての $A_i \in \mathfrak{F}_i$ ($1 \leq i \leq n$)、共通部分 $A_1 \cap \cdots \cap A_n$ は空ではありません。

このため、条件は、フィルター $\mathfrak{F} \in \Phi$ の和集合 $\mathfrak{G}$ が命題 1 の条件を満たすことを表します。

#### 系 3 {#top-i-s6-prop-1-cor-3 .statement tag=0B43}

空ではない集合 $X$ 上のすべてのフィルターの順序付けられた集合は帰納的です。

$X$ の線形に順序付けされたフィルターのすべての集合 $\Phi$ は、集合 $A_i$ すべての属するが仮定までに同じ$\mathfrak{F}_j$ になるため、系 2 of 命題 1 の条件を満たします。 $(\mathrm{F}_{\mathrm{II}})$ を適用できます。

### 3. フィルターの基底

$\mathfrak{G}$ が $X$ (no. 2) のフィルター $\mathfrak{F}$ のサブベースである場合、$\mathfrak{F}$ は一般に、$X$ の部分集合の集合や $\mathfrak{G}$ の含む集合ではありません。 $\mathfrak{G}$ がこの性質を持つためには、$\mathfrak{G}$ の集合のすべての有限共通部分が $\mathfrak{G}$ の含む集合となることが必要かつ十分です。したがって、次の命題:

#### 命題 2 {#top-i-s6-prop-2 .statement tag=0B44}

$\mathfrak{B}$ を部分集合の集合 $X$ の集合とします。次に、$\mathfrak{B}$ が次の 2 つのプロパティを持つ場合に限り、$X$ の部分集合の集合と $\mathfrak{B}$ の含む集合がフィルターになります。
(B_I) 共通部分/2 集合/$\mathfrak{B}$ 含む集合/$\mathfrak{B}$。
(B_{II}) $\mathfrak{B}$ は空ではなく、$X$ の空の部分集合は $\mathfrak{B}$ にはありません。

#### 定義 3 {#top-i-s6-def-3 .statement tag=0B45}

公理 (B_I) および (B_{II}) を満たす集合 $X$ の部分集合の集合 $\mathfrak{B}$ は、生成されるフィルターのベースであると言われます。 2 つのフィルター 基底が同じフィルター 生成するである場合、それらは同等であると言われます。

$\mathfrak{G}$ がフィルター $\mathfrak{F}$ の部分基底である場合、$\mathfrak{G}$ の集合の有限共通部分の集合 $\mathfrak{G}'$ は、$\mathfrak{F}$ (no. 2) の基底です。

#### 命題 3 {#top-i-s6-prop-3 .statement tag=0B46}

$X$ 上のフィルター $\mathfrak{F}$ のサブセット $\mathfrak{B}$ は、$\mathfrak{F}$ のすべてのセットに $\mathfrak{B}$ のセットが含まれる場合に限り、$\mathfrak{F}$ のベースになります。

$\mathfrak{B}$ が $\mathfrak{F}$ の基底である場合、明らかに $\mathfrak{F}$ 含む集合の $\mathfrak{B}$ のすべての集合です。逆に、$\mathfrak{F}$ 含む集合 $\mathfrak{B}$ の集合ごとの場合、$X$ 含む集合 $\mathfrak{B}$ 一致するの部分集合のうち集合 $(\mathrm{F}_1)$の理由で$\mathfrak{F}$と。

#### 命題 4 {#top-i-s6-prop-4 .statement tag=0B47}

集合 $X$ では、$\mathfrak{B}$ 含むの集合ごとに限り、基底 $\mathfrak{B}'$ を含むフィルター $\mathfrak{F}'$ は、基底 $\mathfrak{B}$ を含むフィルター $\mathfrak{F}$ よりもより細かいになります。 $\mathfrak{B}'$中集合。

これは、定義 2 と 3 の明らか帰結です。

#### 系 {#top-i-s6-n3-cor-1 .statement tag=0B48}

集合 $X$ の 2 つのフィルター 基底 $\mathfrak{B}, \mathfrak{B}'$ は、$\mathfrak{B}$ 含む集合の $\mathfrak{B}'$ のすべての集合と、$\mathfrak{B}'$ 含むのすべての集合が一致する場合にのみ同等です。 $\mathfrak{B}$中集合。

フィルター基底の例。 1) $X$ をトポロジー 空間とします。 命題 3 は、点 $x \in X$ の近傍フィルターの基底が、正確に $x$ (§ 1, no. 3、定義 5) の近傍の基本系であることを示しています。

2) $X$ を、関係 $(\sigma)$ (集合理論, 章 III, § 1, no. 10) に関して空でない有向集合とします。すべての $x \in X$ のそれぞれの $a \in X$、集合 $S(a)$ について、$a(\sigma)x$ は、元 $a$ に対して$X$ の切断と呼ばれます。次に、$X$の切断の集合$\mathscr{S}$はフィルター基底です。これは明らかに$(\mathrm{B}_{\mathrm{II}})$を満たし、$a, b$が$X$のいずれか2つの元である場合、仮定によるものです。 元 $c \in X$ は $a(\sigma)c$ と $b(\sigma)c$ であるため、
$$
S(c) \subset S(a) \cap S(b),
$$
$(\mathrm{B}_1)$が満足できるように。 $\mathscr{S}$ によって生成されるフィルターは、有向集合 $X$ の切断フィルターと呼ばれます。

たとえば、Fréchet フィルター (no. 1) は、関係 $\leqslant$ によって指示されたものとみなされ、順序付けされた集合 $\mathbf{N}$ の切断フィルターです。
$\mathfrak{F}$ を集合 $Z$ のフィルターとします。 $\mathfrak{F}$ は関係 $\supset$ に関して指示されているため、[公理 $(\mathrm{F}_{\mathrm{II}})$ により] 定義する切断は $\mathfrak{F}$ でフィルタリングできます。ここで、集合 $A \in \mathfrak{F}$ に対する $\mathfrak{F}$ の切断は、$M \subset A$ のように、すべての $M \in \mathfrak{F}$ の集合 $S(A)$ です。このフィルターはフィルター$\mathfrak{F}$の切断フィルターと呼ばれます。

### 4. ウルトラフィルター

#### 定義 4 {#top-i-s6-def-4 .statement tag=0B49}

集合 $X$ の限外フィルターはフィルター $\mathfrak{F}$ であるため、$X$ にはフィルターが存在せず、$\mathfrak{F}$ よりも厳密により細かい (他の語、極大元では、すべてのフィルターの順序付けられた集合) $X$）。

$X$ のすべてのフィルターの順序付けられた集合は帰納的 (no. 2、命題 1、系 3) であるため、Zorn の補題 (集合理論、R、§ 6, no. 10) は次のことを示します。

#### 定理 1 {#top-i-s6-thm-1 .statement tag=0B4A}

$\mathfrak{F}$ が集合 $X$ のフィルターである場合、$\mathfrak{F}$ よりも限外フィルター より細かいがあります。

#### 命題 5 {#top-i-s6-prop-5 .statement tag=0B4B}

$\mathfrak{F}$ を集合 $X$ の限外フィルターとします。 $A$ と $B$ が $A \cup B \in \mathfrak{F}$ となるような $X$ の 2 つの部分集合である場合、$A \in \mathfrak{F}$ または $B \in \mathfrak{F}$ のいずれかになります。

命題が偽の場合、$X$ の部分集合 $A$ と $B$ が存在し、$A \notin \mathfrak{F}$ と $B \notin \mathfrak{F}$ と $A \cup B \in \mathfrak{F}$ が存在します。 $\mathfrak{G}$ を部分集合の集合 $X$ の $M$ として、$A \cup M \in \mathfrak{F}$ とします。 $\mathfrak{G}$ が $X$ のフィルターであり、$B \in \mathfrak{G}$ 以降、$\mathfrak{G}$ が厳密に $\mathfrak{F}$ よりもより細かいであることを確認するのは簡単です。しかし、この矛盾する仮定の $\mathfrak{F}$ は限外濾過器です。

#### 系 {#top-i-s6-n4-cor-1 .statement tag=0B4C}

*有限列* の和集合 $(A_i)_{1 \leq i \leq n}$ * $X$ の部分集合 * 属するを限外濾過装置* $\mathfrak{F}$ にすると、*その後* $A_i$ *属するから* $\mathfrak{F}$ の少なくとも 1 つになります。

証明は$n$の帰納法までです。
特に、$(A_i)_{1 \leq i \leq n}$ が $X$ の *カバー* である場合、$A_i$ 属する ～ $\mathfrak{F}$ の少なくとも 1 つです。
命題 5 限外フィルターの *特徴*。より一般的には、次のようになります。

#### 命題 6 {#top-i-s6-prop-6 .statement tag=0B4D}

*$\mathfrak{G}$ * を集合* $X$ のフィルターのサブベースとします。 *それぞれの部分集合* $Y$ *of* $X$ * $Y \in \mathfrak{G}$ * または* $\complement Y \in \mathfrak{G}$ のいずれかがある場合、 *そのとき* $\mathfrak{G}$ * $X$ は限外フィルターがオンです*。

$\mathfrak{F}$ をフィルター 含む $\mathfrak{G}$ とします (仮定までに 1 つあります)。次に $\mathfrak{F}$ 一致すると $\mathfrak{G}$; $Y \in \mathfrak{F}$ なら $\complement Y \notin \mathfrak{F}$;したがって $\complement Y \notin \mathfrak{G}$、したがって $Y \in \mathfrak{G}$ です。

* 限外フィルターの例。* 空ではない集合 $X$ のすべての部分集合の集合のうち、指定された元 $a \in X$ の含むが限外フィルターです。これはフィルターであり、$Y$ が $X$ のいずれかの部分集合である場合、$a \in Y$ または $a \in \complement Y$ のいずれかになります。このような限外濾過装置は *トリビアル* と呼ばれます。

この例とは別に、定理 1 (したがって選択の公理) を使用する場合を除き、限外フィルターの存在を (可算無限の集合上であっても) 証明することはできません。

#### 注意 {#top-i-s6-n4-rem-1 .statement tag=0B4E}

$X$ 含む少なくとも 2 つの元の場合、$X$ には少なくとも 2 つの異なる限外フィルターがあり、したがって、$X$ のフィルターの順序付けられた集合には最大の元がありません。

#### 命題 7 {#top-i-s6-prop-7 .statement tag=0B4F}

*すべてのフィルター* $\mathfrak{F}$ *集合* $X$ * は、* $\mathfrak{F}$ よりも限外フィルターのより細かいの共通部分です。

明らかに、これは共通部分含む $\mathfrak{F}$ です。逆に、$A$ を属するから $\mathfrak{F}$ にならない$X$ の部分集合とし、$A'$ を $\complement A$ とします。 $A$ 含むいいえ集合の $\mathfrak{F}$;したがって、すべての $M \in \mathfrak{F}$ は $A'$ と一致するため、(no. 2、命題 1、系 1) $\mathfrak{F}$ および含む $A'$ よりもより細かいであるフィルター $\mathfrak{F}'$ が存在します。 $\mathfrak{U}$ が $\mathfrak{F}'$ (定理 1) よりも限外濾過器より細かいである場合、$A \notin \mathfrak{U}$ になります。これで証明は完了です。

### 5. 誘導フィルター

#### 命題 8 {#top-i-s6-prop-8 .statement tag=0B4G}

*$\mathfrak{F}$ *を集合* $X$ *および* $A$ *部分集合の* $X$ のフィルターにします。 *その後、トレース* $\mathfrak{F}_A$ *of* $\mathfrak{F}$ *on* $A$ *は、* $\mathfrak{F}$ の各集合 *が $A$ *を満たす場合にのみフィルターになります。

$(M \cap N) \cap A = (M \cap A) \cap (N \cap A)$ なので、$\mathfrak{F}_A$ が $(\mathrm{F}_{\mathrm{II}})$ を満たすことがわかります。もう一度、$M \cap A \subset P \subset A$ の場合、$P = (M \cup P) \cap A$、よって $\mathfrak{F}_A$ は $(\mathrm{F}_1)$ を満たします。したがって、$\mathfrak{F}_A$ は、$(\mathrm{F}_{\mathrm{III}})$ を満たす場合に限り、つまり、$\mathfrak{F}$ の各集合が $A$ を満たす場合に限り、フィルターになります。

特に、$A \in \mathfrak{F}$ の場合、$\mathfrak{F}_A$ は、$(\mathrm{F}_{\mathrm{II}})$ と $(\mathrm{F}_{\mathrm{III}})$ による $A$ のフィルターになります。

#### 定義 5 {#top-i-s6-def-5 .statement tag=0B4H}

*$A$ を集合 $X$ の部分集合とし、$\mathfrak{F}$ を $X$ のフィルターとします。 $A$ 上の $\mathfrak{F}$ のトレースが $A$ 上のフィルターである場合、このフィルターは $A$ 上の $\mathfrak{F}$ によって誘発されると言われます。

$X$ 誘導するのフィルター $\mathfrak{F}$ が $A \subset X$ のフィルターである場合、$\mathfrak{F}$ の基底の $A$ のトレースは、命題 3 により、$\mathfrak{F}_A$ の基底になります。 no. 3。

#### 例 {#top-i-s6-n5-exa-1 .statement tag=0B4I}

$X$ を、$X$ のトポロジー 空間、$A$ 部分集合、$X$ の $x$ 点とします。 *近傍フィルター* $x$ の $\mathfrak{B}$ の $A$ のトレースが $A$ のフィルターである必要があるという位数では、$x$ のすべての近傍が $A$ を満たすこと、つまり $x$ が存在することが必要かつ十分です。 $A$ (§ 1, no. 6、定義 10) の*クロージング*で。

誘導フィルターのこの例は 2 つの理由で興味深いものです。1 つは、極限 (§ 7, no. 5) の理論で重要な役割を果たすため、もう 1 つは *すべてのフィルターをこの方法で定義できるためです*。実際、$\mathfrak{F}$ を集合 $X$ のフィルターとし、$X'$ を $X$ に新しい元 $\omega$ を *隣接* させることで得られる集合とします。$X$ は次の補数で識別されます。 $X'$の$\{ \omega \}$ (*集合理論*、R、§ 4, no. 5); $\mathfrak{F}'$ を集合 $M \cup \{ \omega \}$ の $X'$ からなるのフィルターとし、$M$ は $\mathfrak{F}$ を通過します。 $X'$ の各点 $x \neq \omega$ について、$\mathfrak{B}(x)$ を $X'$ のすべての部分集合のうち含む $x$ の集合とし、$\mathfrak{B}(\omega)$ を $\mathfrak{F}'$ とします。次に、$x \in X'$ に対する $\mathfrak{B}(x)$ は明らかに満たす公理 $(\mathrm{V}_1), (\mathrm{V}_{\mathrm{II}}), (\mathrm{V}_{\mathrm{III}})$ と $(\mathrm{V}_{\mathrm{IV}})$ なので、$X'$ 上の定義する位相は、点の近傍フィルターになります。最後に$\omega$はこの位相の$X$の*クロージャ*にあり、$\mathfrak{F}$は$X$の$\mathfrak{F}' = \mathfrak{B}(\omega)$によって誘発されます。このように $X'$ で定義された位相 (この位相を含む集合 $X'$) は、$\mathfrak{F}$ に *関連付けられた *位相* (*トポロジカル空間*) と呼ばれます。

#### 命題 9 {#top-i-s6-prop-9 .statement tag=0B4J}

*集合 $X$ 誘導するのウルトラフィルター $U$ $A \in U$ の場合に限り、$X$ の部分集合 $A$ にフィルター。そして、この条件が満たされる場合、 $U_A$ は $A$ のウルトラフィルターになります。*

これは、命題の5とno. 4の6の明らか帰結です。

### 6. フィルター基底の直像と逆像

$\mathfrak{B}$ を集合 $X$ のフィルター 基底とし、$f$ を $X$ の写像から集合 $X'$ にするとします。この場合、$f(\mathfrak{B})$ は $X'$ の *フィルター 基底* であり、関係 $M \neq \emptyset$ は $f(M) \neq \emptyset$ を意味し、$f(M \cap N) \subset f(M) \cap f(N)$ が得られます。 $\mathfrak{B}_1$ が、基底 $\mathfrak{B}$ のフィルターより *より細かい* であるフィルターの基底である場合、$f(\mathfrak{B}_1)$ は、基底 $f(\mathfrak{B})$ のフィルターより *より細かい* のフィルターの基底です。 (no. 3、命題 4)。

#### 命題 10 {#top-i-s6-prop-10 .statement tag=0B4K}

*$\mathfrak{B}$ が集合 $X$ の限外フィルター 基底であり、$f$ が $X$ の写像から集合 $X'$ である場合、$f(\mathfrak{B})$ は限外フィルターです$X'$の基底*

$M'$を$X'$の部分集合とします。 $\mathfrak{B}$ の $\overline{f}^{-1}(M')$ 含む集合 $M$ の場合、$M'$ 含む $f(M)$;そうでない場合は、$\mathfrak{B}$ の $\mathscr{C}_{\overline{f}}^{-1}(M') = \overline{f}^{-1}\mathscr{C}(M')$ 含む集合 $N$ (no. 4、命題 5)、したがって $\mathscr{C}M'$ 含む $f(N)$ となります。したがって、結果は no. 4 の命題 6 になります。

特に、$f$ が標準単射 $A \to X$ の部分集合 $A$ の集合 $X$ である場合を考えてみましょう。 $\mathfrak{B}$ が $A$ のフィルター 基底である場合、$f(\mathfrak{B})$ は $X$ のフィルター 基底です。 $f(\mathfrak{B})$ によって生成された $X$ 上のフィルター $\mathfrak{F}$ は、$\mathfrak{B}$ が $X$ 上のフィルター 基底とみなされる場合、$\mathfrak{B}$ によって生成された *フィルター と呼ばれます。 $\mathfrak{B}$ が $A$ の *ウルトラフィルター 基底* である場合、命題 10 の理由により、$X$ の *ウルトラフィルター 基底* でもあります。

次に、フィルター 基底の *逆像* がフィルター 基底であるかどうかを調べてみましょう。 $\mathfrak{B}'$ を集合 $X'$ のフィルター 基底とし、$f$ を集合 $X$ の写像を$X'$ にします。この場合、$\overline{f}^{-1}(\mathfrak{B}')$ は、$X$ *その場合にのみ* $\overline{f}^{-1}(M') \neq \varnothing$ *それぞれ* $M' \in \mathfrak{B}'$ に対するフィルター 基底です。これは、関係 $\overline{f}^{-1}(M' \cap N') = \overline{f}^{-1}(M') \cap \overline{f}^{-1}(N')$ の明らか帰結と、no. 3 の定義 3 です。この条件は、*$\mathfrak{B}'$ のすべての集合が $f(X)$* を満たすというというによって表現することもできます [または $f(X)$ 上の $\mathfrak{B}'$ のトレースがフィルター 基底である]。この条件が満たされる場合、$f(\overline{f}^{-1}(\mathfrak{B}'))$ は基底 $\mathfrak{B}$ のフィルター *より細かい* の基底になります。

$\mathfrak{B}$ が $X$ のフィルター 基底である場合、上記の条件が $\mathfrak{B}' = f(\mathfrak{B}); \; \overline{f}^{-1}(f(\mathfrak{B}))$ によって満たされることは明らかであり、その場合、基底 $\mathfrak{B}$ のフィルターより *粗い* フィルターの基底になります。

$A$ を集合 $X$, $\varphi$ 標準単射 $A \to X$ の部分集合とします。 $\mathfrak{B}$ が $X$ のフィルター 基底である場合、$\overline{\varphi}^{-1}(\mathfrak{B})$ は $\mathfrak{B}_A$ と同じになります。これを上記の条件を用いて$A$のフィルター基底として表現すると、命題の8、no. 5の部分が得られます。

### 7. 積のフィルター

$(X_i)_{i \in I}$ を集合の族とし、各 $i \in I$ に対して $\mathfrak{B}_i$ を $X_i$ の *フィルター 基底* とします。 $\mathfrak{B}$ を積集合 $X = \prod_{i \in I} X_i$ の部分集合のうち形 $\prod_{i \in I} M_i$ の集合とします。ただし、$M_i = X_i$ は添字の *有限* 数を除き、 $M_i \neq X_i$ となるように、$i$ ごとに $M_i \in \mathfrak{B}_i$。 公式 $\left( \prod_{i \in I} M_i \right) \cap \left( \prod_{i \in I} N_i \right) = \prod_{i \in I} (M_i \cap N_i)$ は、$\mathfrak{B}$ が $X$ の *フィルター 基底* であることを示します。 基底 $\mathfrak{B}$ のフィルターも、

集合 $\overline{\mathrm{pr}}_x^{-1}(M_x)$、$M_x \in \mathfrak{B}_x$ と $x$ は $I$ を通過します。
$$
\overline{\mathrm{pr}}_x^{-1}(M_x) = M_x \times \prod_{i \neq x} X_i.
$$

#### 定義 6 {#top-i-s6-def-6 .statement tag=0B4L}

*ファミリー 集合 $(X_i)_{i \in I}$、積の各集合 $X_i$ にフィルタ $\mathfrak{F}_i$ があるとすると、フィルタ $\mathfrak{F}_i$ は、基底集合を持つ $X = \prod_{i \in I} X_i$ のフィルタになります。 形の $X$ $\prod_{i \in I} M_i$ の部分集合、添字の有限の数を除くすべての $i \in I$ と $M_i = X_i$ の $M_i \in \mathfrak{F}_i$。 積フィルターは $\prod_{i \in I} \mathfrak{F}_i$ で表されます。*

読者は、フィルター $\mathfrak{F}_i$ の積が、各 $i \in I$ に対して $\mathrm{pr}_i(\mathfrak{G}) = \mathfrak{F}_i$ となるように、$X$ の *最も粗い* フィルター $\mathfrak{G}$ としても定義できることを簡単に検証できます。

前述の注意は、$\mathfrak{B}_i$ が各 $i \in I$ の $\mathfrak{F}_i$ の基底である場合、$\mathfrak{B}$ は積フィルター $\prod_{i \in I} \mathfrak{F}_i$ (no. 3、命題 3) の *基底* であることを示しています。

トポロジカル空間の積 $X = \prod_{i \in I} X_i$ では、任意の点 $x = (x_i)$ の近傍フィルターは、$x_i$ (§ 4, no. 1) の近傍フィルターの *積* です。

積フィルタ $\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i$ の構成は、添字集合 $I$ が *有限* の場合、より簡単になります。 $\mathfrak{F}$ の基底は、*すべて* 積 $\prod_{i \in I} M_i$ によって形成されます。ここで、それぞれ $M_i \in \mathfrak{F}_i$ $i \in I$。 $I = \{ 1, 2, \ldots, n \}$ と書くと
$$
\mathfrak{F}_1 \times \mathfrak{F}_2 \times \cdots \times \mathfrak{F}_n
$$
$\prod_{i \in I} \mathfrak{F}_i$の代わりに。

### 8. 基本フィルター

#### 定義 7 {#top-i-s6-def-7 .statement tag=0B4M}

*$(x_n)_{n \in \mathbf{N}}$を集合$X$の元の無限数列とします。 数列 $(x_n)$ に関連付けられた基本フィルターは、$\mathbf{N}$ の写像 $n \to x_n$ によってフレシェフィルター (no. 1) の像によって $X$ に生成されたフィルターです。

$(x_n)$ に関連付けられた基本フィルターは、$n$ の値の *有限* 数を除いて、$x_n \in M$ のような部分集合の $M$ $X$ の集合であると言うのと同じことになります。 $S_n$ が、$p \geq n$ などのすべての $x_p$ の集合を表す場合、集合 $S_n$ 形数列 $(x_n)$ に関連付けられた基本フィルターの *基底* になります。

数列 $(x_n)$ の無限 *サブシーケンス* に関連付けられた基本フィルターは、$(x_n)$ (cf. 練習問題 15) に関連付けられた基本フィルターよりも *より細かい* です。

定義までに、すべての基本フィルターは可算数の基底を持ちます。逆に:

#### 命題 11 {#top-i-s6-prop-11 .statement tag=0B4N}

*フィルター $\mathfrak{F}$ が可算基底を持つ場合、それは $\mathfrak{F}$ よりもより細かいである基本フィルターの共通部分です。

$\mathfrak{F}$ の可算基底を数列 $(A_n)_{n \in \mathbf{N}}$ として整理しましょう。置いたら

$$
B_n = \bigcap_{p=0}^n A_p,
$$

次に、$\mathfrak{F}$ (no. 3、命題 3) の $B_n$ が再び形基底になり、それぞれの $n$ に対して $B_{n+1} \subset B_n$ が得られます。 $a_n$ を、各 $n \in \mathbf{N}$ の $B_n$ のいずれかの元とします。その場合、$\mathfrak{F}$ が $(a_n)$ に関連付けられた基本フィルターよりも粗いことは明らかです。したがって、$\mathfrak{F}$ よりもより細かいであり、$\mathfrak{F}$ よりもより細かいである基本フィルターの共通部分 $\mathfrak{J}$ が存在します。 $\mathfrak{J}$ が $\mathfrak{F}$ より *厳密により細かい* である場合、$n$ ごとに $B_n \cap \complement M \neq \varnothing$ となる集合 $M \in \mathfrak{J}$ が存在します。 $b_n \in B_n \cap \complement M$ の場合、数列 $(b_n)$ に関連付けられた基本フィルターは $\mathfrak{F}$ よりもより細かいであり、含む $M$ ではありません。これは$\mathfrak{J}$の矛盾する定義です。

#### 注意 {#top-i-s6-n8-rem-1 .statement tag=0B4O}

可算基底を持つフィルターより *粗い* フィルターは、可算基底を持つ必要はありません。たとえば、$X$ が不可算無限集合である場合、$X$ の有限部分集合の補数のフィルター からなるには可算可能な基底がありません (そうでない場合、$X$ の有限部分集合の集合は可算になります。 仮定);それにもかかわらず、このフィルターは、$X$ の個別の元の無限数列に関連付けられたすべての基本フィルターよりも粗いです。

### 9. フィルターに関する雑菌

$\mathfrak{F}$ を集合 $X$ のフィルターとします。 $X$ のすべての部分集合のうち集合 $\mathfrak{P}(X)$ に、関係

「$M \cap V = N \cap V$というような$V \in \mathfrak{F}$が存在します」

$M$ と $N$ の間は *同値関係* $R$ です。$R$ は明らかに再帰的かつ対称であり、$M, N, P$ が $M \cap V = N \cap V$ と $N \cap W = P \cap W$ のように $X$ の 3 つの部分集合である場合、ここで$V$ と $W$ 属するから $\mathfrak{F}$ では、$M \cap (V \cap W) = N \cap (V \cap W) = P \cap (V \cap W)$ と $V \cap W \in \mathfrak{F}$ が続き、$R$ は推移的になります。 同値類 mod $R$ の部分集合 $M$ の $X$ は、$\mathfrak{F}$* に対する $M$ の * 胚芽と呼ばれます。 商集合 $\mathfrak{P}(X)/R$ は、$X$ の部分集合の細菌の *集合 ($\mathfrak{F}$ に対して)* と呼ばれます。 写像 $(M, N) \to M \cap N$ と $(M, N) \to M \cup N$

$$
\mathfrak{P}(X) \times \mathfrak{P}(X)
$$

$\mathfrak{P}(X)$ は、同値関係 $R \times R$ および $R$ と互換性があります

(集合理論、R、、no. 8)。 $M \equiv M' \pmod{R}$ と $N \equiv N' \pmod{R}$ の場合、$\mathfrak{F}$ には $V$ と $W$ が存在し、次のようになります。

$$
M \cap V = M' \cap V \quad \text{and} \quad N \cap W = N' \cap W,
$$
それで
$$
(M \cap N) \cap (V \cap W) = (M' \cap N') \cap (V \cap W)
$$
そして
$$
\begin{align*}
(M \cup N) \cap (V \cap W) &= (M \cap (V \cap W)) \cup (N \cap (V \cap W)) \\
&= (M' \cap (V \cap W)) \cup (N' \cap (V \cap W)) \\
&= (M' \cup N') \cap (V \cap W).
\end{align*}
$$

移行から商まで、これらの写像誘導する $(\mathfrak{P}(X)/R) \times (\mathfrak{P}(X)/R)$ の 2 つの写像を$\mathfrak{P}(X)/R$ とし、（言葉の乱用により）それぞれ$(\xi, \eta) \to \xi \cap \eta$ と$(\xi, \eta) \to \xi \cup \eta$ で表します。 合成 [$\mathfrak{P}(X)/R$ 全体で定義] のこれらの法則に関して、すべての元が冪等であり、各法則が他方に関して可換性、結合性、分配性があることを検証するのは簡単な練習問題です。さらに、関係 $\xi = \xi \cap \eta$ と $\eta = \xi \cup \eta$ は同等です。それらを (言葉の乱用によって) $\xi \subset \eta$ で表すと、この関係が $\mathfrak{P}(X)/R$ の順序であることが容易に検証されます。これに関して、$\mathfrak{P}(X)/R$ は、少なくとも元には $\varnothing$ の芽を持ち、最大のには $X$ の芽をもつ格子です。 元。 関係 $\xi \subset \eta$ は、$M \cap V \subset N \cap V$ となるような $M \in \xi$、$N \in \eta$、$V \in \mathfrak{F}$ が存在することを意味します。

ここで、$X'$ を他の集合とし、$\Phi$ を $\mathfrak{F}$ の集合のすべての写像の集合を $X'$ にします。 $\Phi$の関係

「$f$ と $g$ が定義され、$V$ に一致するような $V \in \mathfrak{F}$ が存在します。」

between $f$ and $g$ is 同値関係 $S$; $S$ が再帰的かつ対称であることは明らかであり、$f, g, h$ が 3 つの $\Phi$ の元であり、$f$ と $g$ が $V \in \mathfrak{F}$ で定義され、$g$ と $h$ が定義されて $W \in \mathfrak{F}$ に一致する場合、 $f$ と $h$ は定義されており、$V \cap W \in \mathfrak{F}$ に一致しているため、$S$ は推移的です。 集合$V \in \mathfrak{F}$の$X'$への写像$f$の同値類mod$S$を($\mathfrak{F}$に関して)$f$のジャームと呼び、商集合$\tilde{\Phi} = \Phi/S$を$X$から$X'$への写像のジャームの集合と呼ぶ。 ($\mathfrak{F}$に関して)。

#### 注意 1 {#top-i-s6-n9-rem-1 .statement tag=0B4P}

$X$ のサブセット $M$ から $X'$ へのすべてのマッピング $f$ ($M$ は $\mathfrak{F}$ に属します) は、$X$ から $X'$ へのマッピング $f_1$ の mod $S$ と等価です (上記の用語を正当化します)。 $f$ ～ $X$、例: $X - M$ に定数値を与えることによって。

#### 注意 2 {#top-i-s6-n9-rem-2 .statement tag=0B4Q}

$X$ の 2 つの部分集合 $M$ と $N$ の特性写像 $\varphi_M$ と $\varphi_N$ は、$M$ と $N$ が $\mathfrak{F}$ に関して同じ細菌を持っている場合に限り、$\mathfrak{F}$ に関して同じ細菌を持っています。

$X''$ を 3 番目の集合、$X'$ の $\varphi$ 写像を $X''$ に、$\Phi'$ 集合を $\mathfrak{F}$ の集合のすべての写像を$X''$ にします。 $f \in \Phi$、$\varphi \circ f$、属する ～ $\Phi'$ ごとに、さらに、$g \in \Phi$ が $\mathfrak{F}$ に関して $f$ と同じ胚芽を持っている場合、$\varphi \circ f$ と $\varphi \circ g$ は $\mathfrak{F}$ に関して同じ胚芽を持っていることがすぐにわかります。

したがって、このジャームは、$\mathfrak{F}$ に関して$f$ のジャーム $\tilde{f}$ にのみ依存し、$\varphi(\tilde{f})$ で示されます。したがって、我々は、$X$の写像の細菌の定義する写像（言葉の乱用により$\varphi$で示される）の細菌の集合$\tilde{\Phi}$を$X'$に、細菌の集合$\tilde{\Phi}'$にします。 $X$の写像が$X''$に。

ここで、$X'_i$ ($1 \leq i \leq n$) を集合とします。
$$
Y = \prod_{i=1}^n X'_i
$$
彼らの積; $\Phi_i$ (それぞれ $\Phi$) は、$\mathfrak{F}$ の集合のすべての写像のうちの集合を $X'_i$ (それぞれ $Y$) に表すとします。 $1 \leq i \leq n$ に対して $f_i \in \Phi_i$ が指定され、$M_i \in \mathfrak{F}$ がドメインで $f_i$ の場合、写像 $t \to (f_1(t), \ldots, f_n(t))$ が定義されます。
$$
\bigcap_{i=1}^n M_i
$$
したがって、属するから $\Phi$ になります。これを（言葉の乱用により）写像を$(f_1, \ldots, f_n)$と表します。さらに、$f_i$ と $g_i$ 属するから $\Phi_i$ が$\mathfrak{F}$ ($1 \leq i \leq n$ の場合) に関して同じ胚芽を持っている場合、$(f_1, \ldots, f_n)$ と $(g_1, \ldots, g_n)$ が $\mathfrak{F}$ に関して同じ胚芽を持っていることがすぐにわかります。したがって、この細菌は、$f_i$ の細菌 $\tilde{f}_i$ のみに依存します。それを $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ で表すと、$\Gamma$ は明らかに積集合の全単射です。
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
集合 $\tilde{\Phi}$、ここで、$\tilde{\Phi}_i$ (それぞれ $\tilde{\Phi}$) は、$\mathfrak{F}$ に関して $X$ の写像の細菌の集合が $X'_i$ (それぞれ $Y$) になることを示します。したがって、言葉の乱用により、混乱の危険がない場合には、通常、$\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ ではなく $(\tilde{f}_1, \ldots, \tilde{f}_n)$ と書くことにします。

これまでの話からすると、$Y$ の写像 $\psi$ ごとに、集合 $X''$ 定義する写像 $(\tilde{f}_1, \ldots, \tilde{f}_n) \to \psi(\tilde{f}_1, \ldots, \tilde{f}_n)$ に
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
$X$の写像の細菌の集合$\tilde{\Phi}'$が$X''$に。

特に、$n = 2$ で、$X'_1, X'_2$ と $X''$ がすべて同じ集合 $X'$ に等しい場合 (つまり、$\psi$ は $X'$ 全体で定義された合成の法則になります)、$\psi$ 誘導する $X$ の写像から $X'$ までの集合 $\tilde{\Phi}$ を通して法則の合成が定義されます。 $X'$ で与えられた法則が結合 (可換) である場合、 $\tilde{\Phi}$ での対応する法則も結合であることは簡単に検証できます。 $X'$ 上の法則 $\psi$ が単位元 $e'$ を持つ場合、定数写像 $x \to e'$ の $\mathfrak{F}$ に関するジャームは、対応する法則に対する単位元です。 $\tilde{\Phi}$。最後に、$X'$ の法則が単位元 $e'$ を持つ場合、$f$ の領域に含まれる$V \in \mathfrak{F}$ が存在する場合に限り、$f \in \Phi$ の胚芽 $\tilde{f}$ は$\tilde{\Phi}$ で逆元を持ちます。 $f(t)$ は、$t \in V$ ごとに $X'$ で反転可能です。それぞれの $t \in V$ について、$g(t)$ が $f(t)$ の逆数を表す場合、$g$ の生殖 $\tilde{g}$ は $\tilde{\Phi}$ の $\tilde{f}$ の逆数です。特に、$X'$ が法則 $\psi$ に対して群である場合、$\tilde{\Phi}$ は対応する法則に対して群です。同様に、$X'$ が環 (環 $A$ を超える代数) である場合、対応するに関して $\tilde{\Phi}$ は環 (代数 $A$ を超える) になります。 合成の法則。

### 10. 点の細菌

定義と no. 9 の結果が適用される最も一般的な状況の 1 つは、$\mathfrak{F}$ がトポロジカル空間 $X$ の点 $a$ の近傍フィルターである場合です。 「$\mathfrak{F}$に関する細菌」の代わりに、「点 $a$の細菌」について話します。 $a$ の近傍の胚芽は 1 つだけ、つまり空間 $X$ 全体の胚芽だけであることに注意してください。閉じた集合の細菌は、点 $a$ で局所的に閉じた集合の細菌と同一です。つまり、$L$ が $a$ で局所的に閉じている場合、$a$ での $L$ と $\overline{\Gamma}$ の細菌は次のようになります。等しい (§ 3, no. 1, 命題 1)。したがって、$\xi, \eta$ が $a$ でローカルに閉じている集合の 2 つの細菌である場合、$\xi \cup \eta$ と $\xi \cap \eta$ も同様です。

$a$ は各 $V \in \mathfrak{F}$ にあるため、$f(a)$ はドメイン属するから $\mathfrak{F}$ の各写像 $f$ に対して定義されます。さらに、$f$と$g$が$a$で同じ細菌を持っている場合、$f(a) = g(a)$がなければなりません。そのため、$f(a)$は$a$で$f$の細菌$\tilde{f}$にのみ依存し、$\tilde{f}$で値と呼ばれます。 $a$ は $\tilde{f}(a)$ で示されます。 関係 $\tilde{f}(a) = \tilde{g}(a)$ は一般に $\tilde{f} = \tilde{g}$ を意味するものではないことを強調しておく必要があります。

$X', X''$ を 2 つのトポロジー 空間とします。 $b$ 点/$X''$; $g, g'$ $X'$ の 2 つの写像が、$b$ で同じ細菌を持つ $X''$ になります。 $f, f'$が、$X$の2つの写像を$X'$に入れ、$a$で連続し、$a$で同じ芽を持ち、$f(a) = b$となるような場合、$g \circ f$と$g' \circ f'$は点で同じ芽を持ちます。 $a$;なぜなら、$V'$が$X'$の$b$の近傍で、すべての$x' \in V'$に対して$g(x') = g'(x')$となる場合、$f(V) \subset V'$、$f'(V) \subset V'$、および$a$の近傍$V$が存在します。すべての $x \in V$ に対して $f(x) = f'(x')$ が続き、主張が続きます。 $a$の$g \circ f$の細​​菌は、$g$と$f$の細菌$\tilde{g}$と$\tilde{f}$の合成と呼ばれ、$\tilde{g} \circ \tilde{f}$で示されます。

### 練習問題 {#top-i-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
