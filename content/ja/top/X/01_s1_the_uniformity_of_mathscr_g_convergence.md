---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 1
section_title: The uniformity of $\mathscr{G}$-convergence
lang: ja
source: top-v-x
pdf_pages: 0280-0289, 0324-0327
extraction: ocr
subsections:
    - "no": 1
      title: THE UNIFORMITY OF UNIFORM CONVERGENCE
      page: 0
      pdf_page: 280
    - "no": 2
      title: $\mathfrak{S}$-convergence
      page: 0
      pdf_page: 281
    - "no": 3
      title: EXAMPLES OF $\mathscr{E}$-CONVERGENCE
      page: 0
      pdf_page: 283
    - "no": 4
      title: PROPERTIES OF THE SPACES $\mathscr{F}_\mathscr{S}(X; Y)$
      page: 0
      pdf_page: 284
    - "no": 5
      title: COMPLETE SUBSETS OF $\mathscr{F}_\mathscr{S}(X; Y)$
      page: 0
      pdf_page: 285
    - "no": 6
      title: $\mathscr{E}$-CONVERGENCE IN SPACES OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 286
statements: 33
exercises: 12
content_sha256: af3dfdd4f39729e3250a1f3b8bf52f85ab15793f769a6fbdd57d4197ecefc64c
translated_from: content/en/top/X/01_s1_the_uniformity_of_mathscr_g_convergence.md
translation_method: google
source_content_sha256: 745807f99ebf8ccad98600e79411f1137bc903046fec07540ab638fc2319dece
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 48d120507e35aae5cb343bf15c4b7d5b91eb016fffe44aea8733219e3f3221e3
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. $\mathscr{G}$-収束の均一性

記法。 $X$ と $Y$ が任意の 2 つの集合である場合、$X$ のすべての写像のうち $Y$ の集合は $\mathscr{F}(X; Y)$ で示され、積集合 $Y^X$ と識別できることを思い出します。 (集合理論、章 II, § 5, no. 2)。 $\mathscr{F}(X; Y)$ の各部分集合 $H$ と各 $x \in X$ について、$u$ から $H$ までを実行するので、元 $u(x) \in Y$ の $H(x)$ 集合で表します。 $\Phi$ が $\mathscr{F}(X; Y)$ のフィルター 基底である場合、$H$ が $\Phi$ を通過するため、集合 $H(x)$ によって形成される $Y$ のフィルター 基底を $\Phi(x)$ で表します。 最後に、$X$ の各 $u \in \mathscr{F}(X; Y)$ と部分集合 $A$ について、$u|A$ は $u$ から $A$ の制限を表し、これは $A$ の写像から $Y$ を表します。 $H$が$\mathscr{F}(X; Y)$の部分集合である場合、$H|A$は制限の集合、写像の$u|A$、$u \in H$を表します。

### 1. 一様収束の均一性

$X$ を集合とし、$Y$ を制服空間とします。 $Y$の各取り巻き$V$について、$W(V)$は、すべての対の集合、$X$の写像の$(u, v)$を$Y$に、すべての$x \in X$に対して$(u(x), v(x)) \in V$を表すものとします。 $V$が$Y$の側近の集合を貫くように、集合$W(V)$形は$\mathscr{F}(X; Y)$の統一性のある側近の基本系です。なぜなら、彼らは明らかに満たす公理 $(U'_1)$ (章 II, § 1, no. 1) であるからです。 $V, V'$ が $V \subset V'$ となるような $Y$ の 2 つの取り巻きである場合、$W(V) \subset W(V')$ があり、したがって集合 $W(V)$ 満たす

$(B_1)$ (章 I, § 6, no. 3); $\widehat{W(V)} = W(\overline{V})$ があるので、$(U''_{II})$ は満たされます。最後に、関係 "$(u(x), v(x)) \in V$ for all $x \in X$" と "$(v(x), w(x)) \in V$ for all $x \in X$" は、関係 "$(u(x), w(x)) \in \overline{V}^2$ for all $x \in X$" を意味します。他の語には $\widehat{W(V)} \subset W(\overline{V}^2)$ があり、これは $(U'''_{III})$ を証明します。

#### 定義 1 {#top-x-s1-def-1 .statement tag=0CAR}

*The uniformity on the set $\mathscr{F}(X; Y)$ which has as a fundamental system of entourages the set of subsets $W(V)$, where $V$ runs through the set of entourages of $Y$, is called the uniformity of uniform convergence. 位相それ誘導するを一様収束の位相といいます。 この位相に関して$\mathscr{F}(X; Y)$のフィルター$\Phi$が元$u_0$に収束すると、$\Phi$は$u_0$に一様に収束するといいます。

$\mathscr{F}(X; Y)$ の一様収束の *位相* は、$Y$ (練習問題 4) の位相だけではなく、$Y$ の一様構造に依存することに注意してください。

$\mathscr{F}(X; Y)$に一様収束の一様性を持たせた一様空間を$\mathscr{F}_u(X; Y)$とする。

### 2. $\mathfrak{S}$-収束

#### 定義 2 {#top-x-s1-def-2 .statement tag=0CAS}

※$X$を集合、$Y$を空間、$\mathfrak{S}$を部分集合の$X$の集合とします。 $\mathfrak{S}$の集合の一様収束の均一性、または単に$\mathfrak{S}$収束の均一性は、$\mathscr{F}(X; Y)$で最も粗い均一性であり、$\mathscr{F}(X, Y)$の制限写像$u \to u|A$を均一に連続させます。 空間 $\mathscr{F}_u(A; Y)$、$A$ は $\mathfrak{S}$ を通過します。 $\mathscr{F}(X; Y)$ に $\mathfrak{S}$ 収束の一様性を与えることによって得られる一様空間は、$\mathscr{F}_{\mathfrak{S}}(X; Y)$ で表されます*。

$\mathfrak{S}$-収束の均一性によって引き起こされる位相は、$\mathfrak{S}$-収束*の*位相と呼ばれます。これは、$\mathscr{F}(X; Y)$ から $\mathscr{F}_u(A; Y)$ ($A \in \mathfrak{S}$) までのすべての写像 $u \to u|A$ が連続しているものです (章 II, § 2, no. 3、命題 4、系)。

$\mathscr{F}(X; Y)$ のフィルター $\Phi$ は、すべての $A \in \mathfrak{S}$ (章) について $u|A$ が $\Phi$ に関して一様に $u_0|A$ に収束する場合に限り、$\mathfrak{S}$ 収束の位相に関して $u_0$ に収束します。したがって、I, § 7, no. 6、命題 10)、および $\Phi$ は、*$\mathfrak{S}$ の集合で $u_0$ に一様に収束すると言えます*。

$\mathscr{F}_{\mathfrak{S}}(X; Y)$ のフィルター 基底 $\Phi$ は、写像 $u \to u|A$ の下の $\Phi$ の各 $A \in \mathfrak{S}$、像が $\mathscr{F}_u(A; Y)$ のコーシーフィルター 基底である場合に限り、コーシーフィルター 基底です。 (章 II, § 3, no. 1、命題 4)。

$f$ をトポロジカル (それぞれ一様) 空間 $Z$ から $\mathscr{F}_{\mathfrak{S}}(X; Y)$ への写像とします。この場合、$Z$ から $\mathscr{F}_u(A; Y)$ への各 $A \in \mathfrak{S}$、写像 $z \to f(z)|A$ が連続 (それぞれ一様連続) である場合に限り、$f$ は連続 (それぞれ一様連続) になります (章 I, § 2, no. 3, 命題 4; 章 II, § 2, no. 3、命題 4）。

最後に、$M$ を $\mathscr{F}_{\mathfrak{S}}(X; Y)$ の部分集合とします。この場合、$M$ は、制限 $u|A$ の各 $A \in \mathfrak{S}$、集合について、$u \in M$ の$\mathscr{F}_u(A; Y)$ (章 II, § 4, no. 2、命題) のプリコンパクト部分集合である場合に限り、プリコンパクトです。 3)。

#### 注意 1 {#top-x-s1-n2-rem-1 .statement tag=0CAT}

The general definition of the entourages of an initial uniformity (Chapter II, § 2, no. 3, Proposition 4) shows that a fundamental system of entourages of $\mathscr{F}_\mathscr{S}(X; Y)$ may be obtained as follows: for each $A \in \mathscr{S}$ and each entourage $V$ of a fundamental system of entourages $\mathscr{B}$ of $Y$, let $W(A, V)$ be the set of all pairs of mappings $(u, v)$ of $X$ into $Y$ such that $(u(x), v(x)) \in V$ for each $x \in A$; as $A$ runs through $\mathscr{S}$ and $V$ runs through $\mathscr{B}$, the *finite intersections of the sets* $W(A, V)$ form a fundamental system of entourages of $\mathscr{F}_\mathscr{S}(X; Y)$.

この記述は、$\mathscr{S}, \mathscr{S}'$が$\mathscr{S} \subset \mathscr{S}'$となるような$X$の部分集合の2つの集合である場合、$\mathscr{S}'$-収束の均一性は$\mathscr{S}$-収束の均一性よりも*より細かい*であることを示しています。

#### 注意 2 {#top-x-s1-n2-rem-2 .statement tag=0CAU}

ただし、$\mathscr{S}$-収束の一様性は、$\mathscr{S}$の集合の有限和集合に含まれる$X$のすべての部分集合の集合$\mathscr{S}'$によって置き換えること$\mathscr{S}$によって変更されません。したがって、$\mathscr{S}$ 収束の研究では、常に集合 $\mathscr{S}$ が次の 2 つの条件を満たす場合に限定することができます。

(F'$_1$) *$\mathscr{S}$ *属するから * $\mathscr{S}$ の集合の部分集合ごと。

(F'$_2$) ** $\mathscr{S}$ *属するから* $\mathscr{S}$ の集合のすべての有限和集合。

(F'$_2$) が満たされる場合、集合 $W(A, V)$ をすべて取得することで、$\mathscr{F}_\mathscr{S}(X; Y)$ の側近の基本系が得られます。ここで、$A$ は $\mathscr{S}$ を通過し、$V$ は $Y$ の側近の基本系を通過します。

#### 注意 3 {#top-x-s1-n2-rem-3 .statement tag=0CAV}

$\mathscr{S}$-収束の均一性は、$\mathscr{F}(X; Y)$ から $\prod_{A \in \mathscr{S}} \mathscr{F}_u(A; Y)$ へのマッピング $u \to (u|A)_{A \in \mathscr{S}}$ の下で、この積空間の均一性の逆像です (II, § 2, no. 6 章、命題 8)。 $\mathscr{S}$ が $X$ の *カバー* である場合、この写像は *単射* であり、したがって $\mathscr{F}_\mathscr{S}(X; Y)$ は、この写像の像である $\prod_{A \in \mathscr{S}} \mathscr{F}_u(A; Y)$ の均一部分空間と同型です。

#### 命題 1 {#top-x-s1-prop-1 .statement tag=0CAW}

*もし* $Y$ *がハウスドルフで、* $\mathscr{S}$ *が* $X$のカバーである場合、*その場合、空間* $\mathscr{F}_\mathscr{S}(X; Y)$ *はハウスドルフ*です。

$u, v$ を $\mathscr{F}_\mathscr{S}(X; Y)$ の 2 つの元とし、$Y$ のすべての取り巻き $V$ とすべての $A \in \mathscr{S}$ に対して $(u, v) \in W(A, V)$ を与えます。 $Y$ はハウスドルフなので、集合 $A \in \mathscr{S}$ ごとに $u$ と $v$ 一致するが成り立ち、$\mathscr{S}$ が $X$ をカバーするので、$u = v$ がなければなりません。

#### 注意 4 {#top-x-s1-n2-rem-4 .statement tag=0CAX}

$H$を$\mathscr{F}(X; Y)$の部分集合とします。言葉の乱用により、$\mathscr{F}(X; Y)$への$\mathscr{S}$収束の均一性（それぞれ位相）によって$H$に誘発される均一性（それぞれ位相）を、$\mathscr{S}$-集合への収束の均一性（それぞれ位相）と呼びます。 $H$。

#### 注意 5 {#top-x-s1-n2-rem-5 .statement tag=0CAY}

$L$ をフィルター $\mathfrak{S}$ でフィルターした集合とし、$\lambda \to u_\lambda$ を $L$ の写像として、$\mathfrak{S}$ に関して極限 $v$ を持つ$\mathscr{F}_\mathscr{S}(X; Y)$ とします。そのとき、*フィルターに関して* $\mathfrak{S}$、*写像* $u_\lambda$ *of* $X$ *into* $Y$ *一様に* $v$ *[または家族* $(u_\lambda)$ *が一様に収束する* $v$] *in * $\mathscr{S}$ の集合ごと。 *$L = \mathbf{N}$ *かつ* $\mathfrak{S}$ *がフレシェフィルター*の場合、*この主張*では$\mathfrak{S}$の言及を省略します。

より具体的には、$Y$ で定義された合成の可換かつ結合的な法則 (加法的に書かれた) があると仮定します。 $(u_n)$ が $X$ の写像のいずれかの数列を $Y$ に変換した場合、$v_n$ を次のように定義される写像とします。

$$
v_n(x) = \sum_{k=0}^n u_k(x) \quad (n \in \mathbf{N});
$$

一般的な項が* $u_n$ * である *系列は、* $\mathscr{G}$ のすべての集合で一様収束します。 * 数列* $(v_n)$ * は、* $\mathscr{G}$ のすべての集合で一様収束します。同様に、すべての有限部分集合 $J$ $L$ について写像 $x \to \sum_{\lambda \in J} n_\lambda(x)$ を考慮することで、定義する *一様に加算可能な族* $(u_\lambda)_{\lambda \in L}$ of 写像 of $X$ を $Y$ にします。 $L$ の有限部分集合の有向集合に対して、$\mathscr{F}_\mathscr{G}(X; Y)$ の写像のうち極限 (章 III, § 5, no. 1)。

#### 注意 6 {#top-x-s1-n2-rem-6 .statement tag=0CAZ}

定義 1 と 2 からすぐに、$x \in \bigcup_{A \in \mathscr{G}} A$ ごとに、$\mathscr{F}_\mathscr{G}(X; Y)$ から $Y$ への写像 $u \to u(x)$ が *一様連続* であることがわかります。したがって、特に、$\overline{H}$ が $\mathscr{F}_\mathscr{G}(X; Y)$ の部分集合 $H$ の終結を示す場合、すべての $x \in \bigcup_{A \in \mathscr{G}} A$ (章 I, § 2, no. 1, 定理 1) に対して $\overline{H}(x) \subset \overline{H(x)}$ が得られます。

### 3. $\mathscr{E}$-収束の例

I。 ** $X$ の部分集合で一様収束。 $A$を$X$の部分集合とし、$\mathscr{G} = \{ A \}$とします。 $\mathscr{G}$ 収束の均一性 (それぞれ位相) は、$A$ における一様収束の *均一性* (それぞれ *位相*) と呼ばれます。 $\mathscr{F}_\mathscr{G}(X; Y)$ のフィルター $\Phi$ が $u_0$ に収束する場合、それは $A$ で *一様に * $u_0$ に収束するといいます。 $A = X$ のとき、no. 1 で定義された一様収束の構造を回復します。

II。 ** $X$ の部分集合における点ごとの収束。 $A$ を $X$ の部分集合とし、$\mathscr{G}$ を 1 つの点所属から $A$ で構成される $X$ のすべての部分集合の集合とします（ no. 2 の注意 2 を、$\mathscr{G}$ をすべての有限部分集合の $A$ の集合とみなしても同じことになります。 $\mathscr{G}$ 収束の均一性 (それぞれ位相) は、$A$ における *点ごとの収束の *均一性* (それぞれ *位相*) と呼ばれます。 $\mathscr{F}_\mathscr{G}(X; Y)$ のフィルター $\Phi$ が $u_0$ に収束する場合、それは $A$ *点ごとに * $u_0$ に収束するといいます。これは、各 $x \in A$、$u_0(x)$ がフィルター $\Phi$ に関して $u(x)$ の極限である場合にのみ当てはまります。

特に、$A = X$ の場合、$X$ での点収束の均一性 (それぞれ位相) は、単に点ごとの収束 * の *均一性 * (それぞれ *位相*) と呼ばれます。この構造を$\mathscr{F}(X; Y)$に付与して得られるユニフォーム空間を$\mathscr{F}_s(X; Y)$と表記します。点収束の位相は、$Y^X$ 上の *積* 位相であるため、$Y$ の位相にのみ依存し、その一様な構造には依存しないことに注意してください。

III。コンパクトな収束。 $X$ がトポロジー 空間であると仮定し、$\mathscr{S}$ を $X$ のすべてのコンパクト部分集合の集合とします。 $\mathscr{S}$ 収束の均一性 (それぞれ位相) をコンパクト収束の均一性 (それぞれ位相) と呼び、$\mathscr{F}(X; Y)$ にこの均一性を与えることで得られる均一性空間を $\mathscr{F}_c(X; Y)$ で表します。コンパクトな収束の構造は一様収束のそれより粗く、$X$ がコンパクトな場合は 2 つの一致するが粗くなります。また、点収束の構造よりもより細かいであり、$X$ が離散であれば、これら 2 つの一致するです。

$X$ が均一空間である場合、$\mathscr{S}$ を $X$ のすべてのプレコンパクト部分集合の集合とすることで、$\mathscr{F}(X; Y)$ でプレコンパクト収束の一様性を定義する求めることができます。繰り返しますが、$X$ がメトリクス空間である場合、$\mathscr{S}$ は、$X$ のすべての境界付き部分集合のうちの集合であると考えられます。 $\mathscr{S}$-収束の均一性は、有界収束の均一性と呼ばれます。

### 4. 空間 $\mathscr{F}_\mathscr{S}(X; Y)$ の特性

#### 命題 2 {#top-x-s1-prop-2 .statement tag=0CB0}

$X_1, X_2$ を 2 つの集合とし、$Y$ を制服空間とし、$\mathscr{S}_i$ を $X_i$ ($i = 1, 2$) の部分集合と$\mathscr{S}_1 \times \mathscr{S}_2$ 集合の集合とします。 部分集合の $X_1 \times X_2$ の形 $A_1 \times A_2$、ここで $A_i \in \mathscr{S}_i, i = 1, 2$。次に、正規の全単射
$$
\mathscr{F}(X_1 \times X_2; Y) \to \mathscr{F}(X_1; \mathscr{F}(X_2; Y))
$$
(集合理論、R、§ 4, no. 14) はユニフォーム空間の同型です
$$
\mathscr{F}_{\mathscr{S}_1 \times \mathscr{S}_2}(X_1 \times X_2; Y)
$$
$\mathscr{F}_{\mathscr{S}_1}(X_1; \mathscr{F}_{\mathscr{S}_2}(X_2; Y))$へ。

$V$ を $Y$ の取り巻きとし、$A_i \in \mathscr{S}_i (i = 1, 2)$ とします。次に、定義の直後に、$W(A_1 \times A_2, V)$ が正規の全単射によって $W(A_1, W(A_2, V))$ と識別され、結果は明らかになります。

#### 命題 3 {#top-x-s1-prop-3 .statement tag=0CB1}

a) $X$ を集合とします。 $\mathscr{S}$ を $X$ の部分集合の集合とします。 $Y, Y'$ を 2 つの均一な空間とします。そして、$f : Y \to Y'$を一様連続写像とします。すると、$\mathscr{F}_\mathscr{S}(X; Y)$ から $\mathscr{F}_\mathscr{S}(X; Y')$ への写像 $u \to f \circ u$ は一様連続です。

b) $X, X'$ を 2 集合とします。 $\mathscr{S}$ (それぞれ $\mathscr{S}'$) を部分集合の集合または $X$ (それぞれ $X'$) とします。 $Y$ を制服空間とします。そして、$g : X' \to X$ を写像として、それぞれの $A' \in \mathscr{S}'$ について、$g(A')$ が $\mathscr{S}$ の集合の有限の和集合に含まれるようにします。すると、$\mathscr{F}_\mathscr{S}(X, Y)$ から $\mathscr{F}_{\mathscr{S}'}(X'; Y)$ への写像 $u \to u \circ g$ は一様連続になります。

#### 命題 4 {#top-x-s1-prop-4 .statement tag=0CB2}

$X, Y$ を 2 つの集合とし、$(X_\lambda)_{\lambda \in L}$ を集合の家族とし、$(Y_\mu)_{\mu \in M}$ を均一空間の家族とする。 それぞれの $\lambda \in L$ について、$\mathscr{S}_\lambda$ を $X_\lambda$ の部分集合の集合とし、$g_\lambda$ を $X_\lambda$ の写像を $X$ に、$\mathscr{S}$ を部分集合の集合とします。 $X$ の集合 $g_\lambda(\mathscr{S}_\lambda)$ の和集合です。 それぞれの $\mu \in M$ について、$f_\mu$ を $Y$ の写像から $Y_\mu$ とし、$Y$ に$f_\mu$ が均一に連続する最も粗い均一性を与えます。 このとき、$\mathscr{F}(X; Y)$ での$\mathscr{S}$ 収束の均一性は、$\mathscr{F}(X; Y)$ の写像 $u \to f_\mu \circ u \circ g_\lambda$ を$\mathscr{F}_{\mathscr{S}_\lambda}(X_\lambda, Y_\mu)$ に均一に連続させる最も粗い均一性です。

これらの命題は、no. 2、注意 1 で与えられる$\mathscr{S}$ 収束の均一性のための基本的な取り巻きの系の記述の明らか帰結です。 証明の詳細は読者に任せます。 命題 4 は、特に次のことを意味します。

#### 系 {#top-x-s1-n4-cor-1 .statement tag=0CB3}

$X$ を集合、$(Y_i)_{i \in I}$ を制服空間のファミリー、$\mathscr{S}$ を $X$ の部分集合の集合とします。 $\prod_{i \in I} Y_i$ に積の均一性を与えると、積の均一空間 $\prod_{i \in I} \mathscr{F}_\mathscr{S}(X; Y_i)$ (集合理論, R, § 4, no. 13) に対する均一空間 $\mathscr{F}_\mathscr{S}(X, \prod_{i \in I} Y_i)$ の標準全単射は次のようになります。 同型。

### 5. $\mathscr{F}_\mathscr{S}(X; Y)$中部分集合を完了

#### 命題 5 {#top-x-s1-prop-5 .statement tag=0CB4}

$\Phi$を集合、$Y$を空間、$\mathscr{S}$を部分集合の$X$の集合とします。次に、$\mathscr{F}_\mathscr{S}(X; Y)$ のフィルター $\Phi$ は、$\Phi$ が $\mathscr{S}$ 収束の均一性に関してコーシーフィルターである場合に限り、$u_0$ に収束し、$B = \bigcup_{A \in \mathscr{S}} A$ で点的に $u_0$ に収束します。

$B$ の点ごとの収束の構造は $\mathscr{S}$ 収束のそれより粗いため、各 $A \in \mathscr{S}$ と $Y$ の各閉じた取り巻き $V$ について、$W(A, V)$ が $B$ に関して閉じていることを示すだけで十分です。点ごとの収束の位相 (章 II, § 3, no. 3、命題 7)。 $x$ が $A$ を通過するため、$W(A, V)$ は写像 $(u, v) \to (u(x), v(x))$ の下で $V$ の逆像の共通部分になります。これらの写像は、点単位収束 (no. 2、注意 6) の位相に関して連続であり、結果は次のようになります。

#### 系 1 {#top-x-s1-prop-5-cor-1 .statement tag=0CB5}

$\mathscr{F}_\mathscr{S}(X; Y)$ の部分空間 $H$ は、$H$ の各コーシー フィルター $\Phi$ について、$\Phi$ が $B = \bigcup_{A \in \mathscr{S}} A$ の $u_0$ に点的に収束するような $u_0 \in H$ が存在する場合にのみ完了します。

これは命題 5 の直後に続きます。

#### 系 2 {#top-x-s1-prop-5-cor-2 .statement tag=0CB6}

$\mathscr{S}_1, \mathscr{S}_2$ を、$X$ の部分集合の 2 つの集合とし、その和集合は同じで、$\mathscr{S}_1 \subset \mathscr{S}_2$ となるものとし、$H$ を $\mathscr{F}(X; Y)$ の部分集合とします。そして、$H$が$\mathscr{S}_1$-収束に関して完了すれば、$\mathscr{S}_2$-収束に関しても完了します。

$\mathscr{G}_2$-収束に関するすべてのコーシー フィルターは、$\mathscr{G}_1$-収束に関するコーシー フィルターでもあり、系を適用する 1 となります。

#### 系 3 {#top-x-s1-prop-5-cor-3 .statement tag=0CB7}

*$H$ を $\mathscr{F}(X; Y)$ の部分集合として、それぞれ*
$$
x \notin B = \bigcup_{A \in \mathscr{G}} A,
$$
*$Y$の$H(x)$のクローズは、$Y$の部分空間の完了です。そして、$\mathscr{F}_{\mathscr{G}}(X; Y)$の$H$の$\overline{H}$は完全な部分空間になります。*

以下のように、$\Phi$ を $\overline{H}$ および定義する写像 $v : X \to Y$ に対するコーシーフィルターとします。 $x \in B$、$\Phi(x)$ が $\overline{H(x)}$ (no. 2、注意 6) のコーシーフィルターである場合、仮定までに少なくとも 1 つの極限点を持ちます。 $v(x)$ をこれらの極限の 1 つとします。 $x \notin B$ の場合、$v(x)$ は $Y$ のいずれかの点となります。この$v$の定義により、$\Phi$は$B$の$v$に点的に収束し、したがって$v$は$\mathscr{F}_{\mathscr{G}}(X; Y)$の$\Phi$の命題5による極限であることが明らかです。

特に、$Y$ が完全であれば、命題 5 の系 3 の仮説はすべての $H \subset \mathscr{F}(X; Y)$ について満たされます。したがって:

#### 定理 1 {#top-x-s1-thm-1 .statement tag=0CB8}

*$X$を集合、$\mathscr{G}$を$X$の部分集合の集合、$Y$を完全な均一空間とします。これでユニフォーム空間$\mathscr{F}_{\mathscr{G}}(X; Y)$が完成しました*。

### 6. $\mathscr{E}$-連続写像の空間での収束

$X, Y$ を 2 つのトポロジー 空間とし、$\mathscr{C}(X; Y)$ は、$X$ から $Y$* に *連続するすべての写像の集合を表すものとします。 $\mathscr{G}$ が $X$ の部分集合の集合であり、$Y$ が均一空間である場合、$\mathscr{G}$ 収束の一様性を備えた $\mathscr{C}_{\mathscr{G}}(X; Y)$ 集合 $\mathscr{C}(X; Y)$ で表します。特に、$\mathscr{C}_s(X; Y), \mathscr{C}_c(X; Y)$ と $\mathscr{C}_u(X; Y)$ は、それぞれ点収束、コンパクト収束、一様収束の均一性を備えた集合 $\mathscr{C}(X; Y)$ を示します。

#### 命題 6 {#top-x-s1-prop-6 .statement tag=0CB9}

*$X$ をトポロジー 空間、$Y$ を均一空間、$\mathscr{G}$ 集合を $X$ の部分集合とします。それぞれの $A \in \mathscr{G}$ と $Y$ の各クローズド取り巻き $V$ について、$W(A, V)$ と $W(\overline{A}, V)$ の $\mathscr{C}(X; Y) \times \mathscr{C}(X; Y)$ のトレースは同じです。*

なぜなら、$u, v$が$X$の$Y$への写像、$X$の$x \mapsto (u(x), v(x))$の$Y \times Y$への写像は連続であり、仮定がすべての$x \in A$に対して$(u(x), v(x)) \in V$であることは、次のことを意味します。 $x \in \overline{A}$ (章 I, § 2, no. 1、定理 1) はすべて $(u(x), v(x)) \in \overline{V} = V$ です。

$\bar{\mathscr{G}}$ が $\mathscr{G}$ の集合の$X$ の閉包の集合を表す場合、命題 6 は、*上* $\mathscr{C}(X; Y)$、$\mathscr{G}$-収束と $\bar{\mathscr{G}}$-収束の構造が同一であることを示します。

**連続写像** の空間での G 収束

#### 系 {#top-x-s1-n6-cor-1 .statement tag=0CBA}

*B を X の密な部分集合とします。 $C(X; Y)$ では、一様収束の構造は B の一様収束の構造と同一です。*

#### 命題 7 {#top-x-s1-prop-7 .statement tag=0CBB}

*Xを位相幾何学的空間、$\mathfrak{S}$をXの部分集合の集合、Yを均一空間とする。 Y がハウスドルフで、$\mathfrak{S}$ の集合の和集合 B が X に密集している場合、$C_{\mathfrak{S}}(X; Y)$ はハウスドルフです。*

なぜなら、$(u, v)$ 属するをすべての集合 $W(A, V)$ に対して、$A \in \mathfrak{S}$ と V が Y の側近である場合、仮定 Y がハウスドルフであるということは、すべての $x \in B$ に対して $u(x) = v(x)$ であることを示します。 $u$ と $v$ が連続の場合、恒等式の拡大の原理 (章 I, § 8, no. 1、命題 2、系 1) により、$u = v$ になります。

特に、X の *密* 部分集合における点収束の $C(X; Y)$、位相はハウスドルフです。

#### 命題 8 {#top-x-s1-prop-8 .statement tag=0CBC}

*Xを集合、$\mathfrak{T}$をXのフィルター、Yを均一空間とする。次に、$u(\mathfrak{T})$ が Y 上のコーシー フィルター 基底となるような写像 $u : X \to Y$ の集合 H は、$F_u(X; Y)$ で閉じられます。*

$u_0 : X \to Y$ を $F_u(X; Y)$ の H の閉包内に置きます。 Y の各対称取り巻き V には、写像 $u \in H$ があり、すべての $x \in X$ に対して $(u_0(x), u(x)) \in V$ になります。一方、仮定によって、$x$ と $x'$ が M にあるときは常に $(u(x), u(x')) \in V$ となるような集合 $M \in \mathfrak{T}$ が存在します。 $(u_0(x), u(x)) \in V$ と $(u_0(x'), u(x')) \in V$ なので、$x$ のときは常に $(u_0(x), u_0(x')) \in V$ ということになります。 $x'$ は M にあるため、$u_0(\mathfrak{T})$ は Y 上のコーシー フィルター 基底です。

#### 系 1 {#top-x-s1-prop-8-cor-1 .statement tag=0CBD}

*Xをトポロジカルな空間、Yを均一な空間とする。 点 $x_0 \in X$ で連続する Y への X の写像の集合は、$F_u(X; U)$ で閉じられます。*

V が X の $x_0$ の近傍フィルターである場合、$u(x_0)$ は $u(V)$ のクラスター 点です。したがって、$u$ は、$u(V)$ が Y 上のコーシー フィルター 基底 (章 II, § 3, no. 2、命題 5、系 2) である場合に限り、$x_0$ で連続です。

#### 系 2 {#top-x-s1-prop-8-cor-2 .statement tag=0CBE}

*X、Lをそれぞれフィルター$\mathfrak{T}, \mathfrak{G}$でフィルターされた2つの集合とし、Yを完全な一様空間とする。各 $\lambda \in L$ について、$u_\lambda$ を Y の X の写像とします。(i) ファミリ $(u_\lambda)_{\lambda \in L}$ が X (フィルター $\mathfrak{G}$ に関して) で写像 $v : X \to Y$ に一様に収束するとします。 (ii) 各 $\lambda \in L$、$u_\lambda$ は、フィルター $\mathfrak{T}$ に関して極限 $y_\lambda$ を持ちます。これらの条件の下で、v は $\mathfrak{T}$ に関して極限を持ち、$\mathfrak{T}$ に関する v のすべての極限は、$\mathfrak{G}$ に関して家族 $(y_\lambda)_{\lambda \in L}$ の極限になります。

v は、$F_u(X; Y)$ の $u_\lambda$ の集合の閉包にあるため、$v(\mathfrak{T})$ は、命題 8 により Y 上のコーシー フィルター 基底になります。これは、Y が完全であるため、v が $\mathfrak{T}$ に関して極限 y を持つことを示しています。させて

X' = X \cup \{ \omega \} be the topological space associated with the filter $\mathscr{F}$ (Chapter I, § 6, no. 5), and extend $u_\lambda$ (resp. $v$) to a mapping $\bar{u}_\lambda$ (resp. $\bar{v}$) of $X'$ into $Y$ by putting $\bar{u}_\lambda(\omega) = y_\lambda$ [resp. $\bar{v}(\omega) = y$]. すると、写像 $\bar{u}_\lambda, \bar{v}$ は$X'$ で連続し、$\bar{u}_\lambda$ は$\mathscr{G}$ に関して$X$ ～ $\bar{v}$ で一様に収束します。 $X$ は $X'$ で密であるため、系から命題 6 は、$\bar{u}_\lambda$ が $X'$ から $\bar{v}$、特に $y = \lim_{\mathscr{G}} y_\lambda$ で一様に収束することを示しています。

#### 定理 2 {#top-x-s1-thm-2 .statement tag=0CBF}

*$X$を位相ベクトル空間、$Y$を均一空間とする。そして、$X$の連続写像の$Y$への集合$C(X; Y)$は、一様収束の位相を備えた空間$F(X; Y)$の閉じた部分集合です。

それぞれの $x \in X$ について、$x$ で連続する $X$ から $Y$ への写像の集合は、$F_u(X; Y)$ で閉じられます (命題 8、系 1)。したがって、これらのセットの交差点 $C(X; Y)$ も閉鎖されます。

この結果は、連続写像の*一様極限が連続*であるという形で表現できるかもしれません。

#### 系 1 {#top-x-s1-thm-2-cor-1 .statement tag=0CBG}

*$Y$が完全なユニフォーム空間であれば、$C_u(X; Y)$が完成します。

なぜなら、定理 2 によって、$C_u(X; Y)$ は制服空間 $F_u(X; Y)$ の閉じた制服部分空間となり、no. 5 の定理 1 によって完成するからです。

#### 系 2 {#top-x-s1-thm-2-cor-2 .statement tag=0CBH}

*$X$ をトポロジー 空間、$\mathscr{S}$ 集合の $X$ の部分集合、$Y$ を均一空間とします。 $\tilde{C}_\mathscr{S}(X; Y)$ は、$X$ のすべての写像から $Y$ への集合を表し、その制限から $\mathscr{S}$ のそれぞれの集合までが連続しているものとします。次に、$\tilde{C}_\mathscr{S}(X; Y)$ はユニフォーム空間 $F_\mathscr{S}(X; Y)$ のクローズド部分空間であり、$Y$ が完了すると完了します*。

$u$ が $F_\mathscr{S}(X; Y)$ の $\tilde{C}_\mathscr{S}(X; Y)$ の閉包にあるとします。次に (no. 2)、各 $A \in \mathscr{S}$、$u|A$ は $F_u(A; Y)$ の $C(A; Y)$ の閉包内にあるため、定理 2 まで連続します。

#### 系 3 {#top-x-s1-thm-2-cor-3 .statement tag=0CBI}

*$X$ を metrizable または局所的にコンパクトなトポロジー 空間とし、$Y$ を均一空間とします。次に、$C(X; Y)$ はユニフォーム空間 $F_c(X; Y)$ で閉じられます。 加法 $Y$ が完了すると、ユニフォーム空間 $C_c(X; Y)$ が完成します。*

系 2 により、$\mathscr{S}$ を $X$ のコンパクトな部分集合の集合とすると、検討中の両方のケースで $\tilde{C}_\mathscr{S}(X; Y) = C(X; Y)$ が得られることを示すのに十分です。 $X$ が局所的にコンパクトであれば、これは明らかです。 $X$ が計量可能で、$u : X \to Y$ が写像で、その $X$ のすべてのコンパクト部分集合への制限が連続である場合、各 $x \in X$ と $X$ の点の各数列 $(z_n)$ について、 $x$ に収束すると、$u(x) = \lim_{n \to \infty} u(z_n)$ があり、したがって、$u$ は $x$ (章 IX, § 2, no. 6, 命題 10) で連続します。

上記の議論は、$x$ のすべての点に近傍の *可算* 基底値系がある場合に常に適用されることに注意してください。

#### 注意 1 {#top-x-s1-n6-rem-1 .statement tag=0CBJ}

一般に、集合 $\mathscr{C}(X; Y)$ は *点単位* 収束の位相に関して $\mathscr{F}(X; Y)$ では閉じていません。他の語では、連続写像の点単位極限は必ずしも連続ではありません [練習問題 5 a)]。

#### 注意 2 {#top-x-s1-n6-rem-2 .statement tag=0CBK}

$\mathscr{C}(X; Y)$ のフィルターは、この写像に均一に収束することなく、*連続* 写像に *点ごとに*収束する可能性があります。

たとえば、区間 $I = [0, 1]$ では、$u_n$ を実数値の写像とします。これは、$x = 0$ と $2/n \leq x \leq 1$ では 0 に等しく、$x = 1/n$ では 1 に等しく、区間 $[0, 1/n]$ と $[1/n, 2/n]$ では線形です。 数列 $(u_n)$ は点的に 0 に収束しますが、$I$ (cf. 練習問題 6) では一様に 0 に収束しません。

#### 注意 3 {#top-x-s1-n6-rem-3 .statement tag=0CBL}

$X$ が均一空間である場合、命題 8 と類似した証明は、$X$ から $Y$ への *一様連続* 写像の集合が $\mathscr{F}_u(X; Y)$ で *閉じている* ことを示します。

#### 注意 4 {#top-x-s1-n6-rem-4 .statement tag=0CBM}

ユニフォーム空間 $Y$ が、写像 $(y, y') \to y + y'$ が $Y \times Y$ で連続するように加法的に書かれた合成の可換かつ結合的な法則を運ぶとします。 次に、$(u_n)$ が $X$ の写像から $Y$ に連続する数列であり、その一般項が $u_n$ である系列が $X$ で *一様収束* する場合、系列の和は連続です$X$に。

連続写像の *一様に合計可能な* ファミリー (no. 1、注意 5) の対応するの結果を述べるのは読者に任せます。

#### 命題 9 {#top-x-s1-prop-9 .statement tag=0CBN}

*$X$ を位相ベクトル空間、$Y$ を均一空間とします。次に、$\mathscr{C}_u(X; Y) \times X$ から $Y$ への写像 $(f, x) \to f(x)$ は連続です。*

$f_0 : X \to Y$ を連続する写像とし、$x_0$ を $X$ の点とし、$V$ を $Y$ の取り巻きとする。 連続する写像 $f : X \to Y$ の集合 $T$ は、すべての $x \in X$ の $(f(x), f(x_0)) \in V$ が $\mathscr{C}_u(X; Y)$ の $f_0$ の近傍になります。 一方、$f_0$は連続なので、すべての$x \in U$に対して$(f_0(x), f_0(x_0)) \in V$となるような$X$の$x_0$の近傍$U$が存在します。 したがって、$(f, x) \in T \times U$ の場合には常に $(f(x), f(x_0)) \in V$ が得られ、結果が証明されます。

### 練習問題 {#top-x-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
