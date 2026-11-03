---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 1
section_title: Order relations. Ordered sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 131-148, 212-221
pdf_pages: 0137-0154, 0218-0227
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ORDER RELATION
      page: 131
      pdf_page: 137
    - "no": 2
      title: PREORDER RELATIONS
      page: 133
      pdf_page: 139
    - "no": 3
      title: NOTATION AND TERMINOLOGY
      page: 135
      pdf_page: 141
    - "no": 4
      title: ORDERED SUBSETS. PRODUCT OF ORDERED SETS
      page: 136
      pdf_page: 142
    - "no": 5
      title: INCREASING MAPPINGS
      page: 138
      pdf_page: 144
    - "no": 6
      title: MAXIMAL AND MINIMAL ELEMENTS
      page: 139
      pdf_page: 145
    - "no": 7
      title: GREATEST ELEMENT AND LEAST ELEMENT
      page: 140
      pdf_page: 146
    - "no": 8
      title: UPPER AND LOWER BOUNDS
      page: 141
      pdf_page: 147
    - "no": 9
      title: LEAST UPPER BOUND AND GREATEST LOWER BOUND
      page: 141
      pdf_page: 147
    - "no": 10
      title: DIRECTED SETS
      page: 145
      pdf_page: 151
    - "no": 11
      title: LATTICES
      page: 145
      pdf_page: 151
    - "no": 12
      title: TOTALLY ORDERED SETS
      page: 146
      pdf_page: 152
    - "no": 13
      title: INTERVALS
      page: 147
      pdf_page: 153
statements: 52
exercises: 24
content_sha256: 49b6fdb508f8ae24a5983c4ccd01da2694911bba401f03e840aa7580da336986
translated_from: content/en/ens/III/01_s1_order_relations_ordered_sets.md
translation_method: google
source_content_sha256: 14e9fa04ef3714dde5ebc1c24c59c34cba4c8b4444c04468c4103f599e7d160e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0d1130263411c453e56fcd1b28d96ce6c885213198c531351455c0f8214fa6c6
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 順序関係。 順序集合

### 1. 定義/順序関係

$R\{x, y\}$ を関係、$x$ と $y$ を別個の文字とする。 R は、文字 x と y* (または *x と y* の間) に関して *順序関係であると言われます。

$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, z\}) \Rightarrow R\{x,\, z\},$$
$$(R\{x,\, y\} \ \text{ and } \ R\{\, y,\, x\}) \Rightarrow (x = y),$$
$$R\{x, y\} \Rightarrow (R\{x,\, x\} \ \text{ and } \ R\{\, y,\, y\}).$$

上記の最初の関係は、R が文字 $x$ と $y$ (章 II, § 6, no. 1) に関して *推移的* であることを示しています。

*例*

(1) 等式*、$x = y$ の *関係は、順序関係です。

(2) 関係 $X \subset Y$ は、X と Y (章 II, § 1, no. 2、命題 1 と 2 および公理 A1) の間の順序関係であり、これはしばしば *包含関係* と呼ばれます。

(3) $R\{x, y\}$を$x$と$y$の間の順序関係とします。 関係 $R\{\, y,\, x\}$ は、順序関係 *x と y* の間であり、順序関係 $R\{x,\, y\}$ の *反対* と呼ばれます。

集合* E 上の *順序関係は、2 つの異なる文字 $x$、$y$ に関して順序関係 $R\{x,\, y\}$ であるため、関係 $R\{x,\, x\}$ は * と等価です* $x \in E$ (他の語では、$R\{x,\, y\}$ が E (章 II, § 6, no. 1) に対して *再帰的* であるようなものです)。次に、関係 $R\{x,\, y\}$ は「$x \in E$ と $y \in E$」を意味し、関係 $(R\{x,\, y\}$ と $R\{\, y,\, x\})$ は「$x \in E$ と $y \in E$ と $x = y$」に相当します。

*例*

#### 例 1 {#ens-iii-s1-n1-exa-1 .statement tag=03SH}

等式の関係と包含は、集合の順序関係ではありません。関係 $x = x$ と $\mathrm{X} \subset \mathrm{X}$ は集合化されていません (章 II, § 1, no. 7)。

#### 例 2 {#ens-iii-s1-n1-exa-2 .statement tag=03SI}

$\mathrm{R}\}x,\ y\{$ を $x$ と $y$ の間の順序関係とし、$x \in \mathrm{E}$ が $\mathrm{R}\}x,\ x\{$ を意味するように E を集合とします (空の集合がこれを満たすことに注意してください) 条件）。 関係 「$\mathrm{R}\}x,\ y\{$ と $x \in \mathrm{E}$ と $y \in \mathrm{E}$」は、すぐに検証されるように、E では順序関係になります。それは、E (cf. no. 4) の $\mathrm{R}\}x,y\{$ によって *誘導* された順序関係と呼ばれます。言葉の乱用により、「E の元の間の関係 $\mathrm{S}\}x,\ y\{$ は順序関係です」という表現が、「関係 ($\mathrm{S}\}x,\ y\{$ と $x \in \mathrm{E}$ と $y \in \mathrm{E}$) は、 順序関係 on E」。たとえば、Aが集合の場合、Aの部分集合の間の関係「$\mathrm{X} \subset \mathrm{Y}$と$\mathrm{X} \subset \mathrm{A}$と$\mathrm{Y} \subset \mathrm{A}$」は順序関係になります。

#### 例 3 {#ens-iii-s1-n1-exa-3 .statement tag=03SJ}

E、Fを集合とします。 関係 "*g 拡大する f*" は、E を F にすると、写像の部分集合の集合の順序関係 ($f$ と $g$ の間) になります。

#### 例 4 {#ens-iii-s1-n1-exa-4 .statement tag=03V3}

In the set $\mathfrak{P}(\mathfrak{P}(\mathrm{E}))$ of sets of subsets of a set E, let $\mathscr{P}$ be the set of *partitions* of E (Chapter II, § 4, no. 7). 分割 $\varpi$ は分割 $\varpi'$ よりも *粗い* と言われていることを思い出します。 $\mathrm{Y} \in \varpi'$ が与えられた場合、 $\mathrm{Y} \subset \mathrm{X}$ (章 II, § 4, no. 6) のような $\mathrm{X} \in \varpi$ が存在します。 E の各分割 $\varpi$ について、$\tilde{\varpi}$ を、E (章 II, § 6, no. 2) 上の $\varpi$ によって定義される同値関係のグラフ、つまり、(相互に互いに素) 集合の和集合とします。 Aが$\varpi$を通る$\mathrm{A} \times \mathrm{A}$。 関係「$\varpi$は$\varpi'$より粗い」は$\tilde{\varpi} \supset \tilde{\varpi}'$と同等であることがすぐにわかり、したがって$\varpi$と$\varpi'$の間の集合$\mathscr{P}$では順序関係になります。

集合 E の *順序付け* は、E をソースおよびターゲットとして持つ対応 $\Gamma = (\mathrm{G},\ \mathrm{E},\ \mathrm{E})$ であり、関係 $(x,\ y) \in \mathrm{G}$ は E 上で順序関係になります。 言葉の乱用により、ときどきは、E の順序付けとして $\Gamma$ のグラフ G を参照します。 $\mathrm{R}\}x,\ y\{$ は E 上の順序関係であり、E 上の順序であるグラフがあります。

#### 命題 1 {#ens-iii-s1-prop-1 .statement tag=03JA}

*対応* $\Gamma$ *間* E *と* E *は、E *そのグラフ* が次の条件を満たす場合に限り* E * 上の順序付けです* G * 以下の条件 :*

(a) $\mathrm{G} \circ \mathrm{G} = \mathrm{G}$。

(b) *集合* $\mathrm{G} \cap \overset{-1}{\mathrm{G}}$ *は $\mathrm{E} \times \mathrm{E}$ の対角線* $\Delta$ です。

関係 $((x,\ y) \in \mathrm{G}$ と $(y,\ z) \in \mathrm{G}) \Rightarrow ((x,\ z) \in \mathrm{G})$ は、$\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$ と関係として書くことができます

$$((x,\ y) \in \mathrm{G} \text{ and } (y,\ x) \in \mathrm{G}) \Leftrightarrow (x = y \text{ and } x \in \mathrm{E} \text{ and } y \in \mathrm{E})$$

$\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$ と書くことができます。 $\mathrm{G} \cap \overset{-1}{\mathrm{G}} = \Delta$ から、$\Delta \subset \mathrm{G}$、よって $\mathrm{G} = \Delta \circ \mathrm{G} \subset \mathrm{G} \circ \mathrm{G}$ を推定します。 $\mathrm{G} \circ \mathrm{G} \subset \mathrm{G}$ 以来、

$$\mathrm{G} \circ \mathrm{G} = \mathrm{G}.$$

### 2. 予約注文関係

$R\{x, y\}$ を関係、$x$ および $y$ を別個の文字とする。 $R$ が推移的で、$R\{x, y\} \Rightarrow (R\{x, x\}$ と $R\{y, y\})$ がある場合、関係であるため、$R$ が順序関係であるとは必ずしも言えません。

$$(R\{x, y\} \text{ and } R\{y, x\})$$

必ずしも$x = y$を意味するものではありません。 $R\{x, y\}$ は、$x$ と $y$ の間の *予約注文関係* であると言われています。 $R\{y, x\}$ は、$x$ と $y$ の間の予約注文関係でもあり、関係 $R\{x, y\}$ の *反対* と呼ばれます。

たとえば、$\mathfrak{R}$ を E (章 II, § 4, no. 6) のカバーである $\mathfrak{P}(E)$ の部分集合の集合とします。 関係 $\mathfrak{R}$ (章 II, § 4, no. 6) の元 $\mathfrak{R}$, $\mathfrak{R}'$ 間の「$\mathfrak{R}$ は $\mathfrak{R}'$ より粗い」は推移的かつ再帰的です。しかし、2 つの異なる被覆は、それぞれが他方よりも粗い場合があります。たとえば、これは、$\mathfrak{R}'$ が $\mathfrak{R}$ の和集合 ($\mathfrak{P}(E)$ 内) と、$\mathfrak{R}$ の集合に含まれる E の部分集合であるが、所属から $\mathfrak{R}$ には含まれない場合に当てはまります。

しかしいずれにしても、関係 $(R\{x, y\}$ と $R\{y, x\})$ は、$x$ と $y$ に関して *同値関係* $S\{x, y\}$ です。 $x'$、$y'$ を、R に現れない$x$、$y$ とは異なる文字とします。すると、$R\{x, y\}$ は ($x$ および $y$ に関して) 同値関係 $S\{x, x'\}$ と *互換性* があり、 $S\{y, y'\}$;その他語 (章 II, § 6, no. 8)、関係

$$(R\{x, y\} \text{ and } S\{x, x'\} \text{ and } S\{y, y'\})$$

$R\{x', y'\}$ を意味します。

¶ 集合* E の *preorder 関係は、関係 $R\{x, x\}$ が $x \in E$ と同等となるような、関係 $R\{x, y\}$ の事前注文です。 関係 $R\{x, y\}$ は「$x \in E$ と $y \in E$」を意味します。

¶ $R\{x, y\}$ が集合 E の予約注文関係である場合、上記で定義された関係 $S\{x, y\}$ は E の同値関係です。 $R'\{X, Y\}$ が関係を表すものとします。

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\exists x)(\exists y)(x \in X \text{ and } y \in Y \text{ and } R\{x, y\}),$$

つまり、移行から商にかけて R によって関係が誘発されます ($x$ と $y$ に関して)。 章 II, § 6, no. 3 で、それが関係と同等であることがわかりました。

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow R\{x, y\}).$$

¶ $R'\{X, Y\}$ が E/S の元の間の *順序関係* であることを示しましょう。 関係 $(R'\{X, Y\}$ および $R'\{Y, Z\})$ は以下と同等です

$$X \in E/S \text{ and } Y \in E/S \text{ and } Z \in E/S \text{ and }$$
$$(\forall x)(\forall y)(\forall z)((x \in X \text{ and } y \in Y \text{ and } z \in Z) \Rightarrow (R\{x, y\} \text{ and } R\{y, z\}))$$

(章 I, § 4、基準 C40、C41)。 $R\{x, y\}$ は推移的であり、$Y \in E/S \Rightarrow Y \neq \emptyset$ (章 II, § 6, no. 2) であるため、$R'\{X, Y\}$ は推移的であることがすぐにわかります。次に$(R'\{X, Y\}$と$R'\{Y, X\})$は以下と同等です。

$$X \in E/S \text{ and } Y \in E/S \text{ and }$$
$$(\forall x)(\forall y) \ ((x \in X \text{ and } y \in Y) \Rightarrow (R\{x, y\} \text{ and } R\{y, x\})),$$

したがって、次と同等です

$$X \in E/S \text{ and } Y \in E/S \text{ and } (\forall x)(\forall y)((x \in X \text{ and } y \in Y) \Rightarrow S\{x, y\}),$$

したがって、暗黙的に

$$X \in E/S \quad \text{and} \quad Y \in E/S \quad \text{and} \quad X = Y.$$

さらに、$R\{x, y\}$ は $R\{x, x\}$ と $R\{y, y\}$ を意味し、したがって $R'\{X, Y\}$ はそれぞれの関係を意味します。

$$X \in E/S \text{ and } (\forall x)((x \in X) \Rightarrow R\{x, x\}),$$
$$Y \in E/S \text{ and } (\forall y)((y \in Y) \Rightarrow R\{y, y\}),$$

よって $R'\{X, Y\}$ は $(R'\{X, X\}$ と $R'\{Y, Y\})$ を意味します。最後に、$x \in E$ は $R\{x, x\}$ を暗示し、$X \in E/S$ は $R'\{X, X\}$ を暗示し、主張の証明が完成します。 $R'\{X, Y\}$ は順序関係が $R\{x, y\}$ に *関連付けられている * と言われています。

¶ 集合 E の *事前順序付け* は、ソースとターゲットとして E を持つ対応 $\Gamma = (G, E, E)$ であり、$(x, y) \in G$ は E に対する事前順序付け関係です。言葉の乱用により、ときどきを E に対する事前順序付けとして $\Gamma$ のグラフ G に参照します。 $\Delta \subset G$ と $G \circ G \subset G$ (これは $G \circ G = G$ を意味します) であることが必要かつ十分です。 同値関係 S 対応するから予約注文関係 $(x, y) \in G$ はグラフとして $G \cap \overset{-1}{G}$ を持ちます。 $(x, y) \in G$ に関連付けられた順序関係は、$E \times E$ の標準写像の下で、対応する (章 II, § 6, no. 8) から G の像まで$(E/S) \times (E/S)$ のグラフ部分集合 G' を持ちます。

$$(E \times E)/(S \times S).$$

#### 例 {#ens-iii-s1-n2-exa-1 .statement tag=03JB}

\* A を単位元で環とします。 2 つの元 $x$ の間の関係 $(\exists z)(z \in \mathrm{A}$ と $y = zx)$、A の $y$ は A の予約注文関係です。 「$x$は$y$の右因子」または「$y$は$x$の左倍数」と読みます。 \*

### 3. 記法と用語

この切断の残りで与えられる定義は、$x$と$y$の間の任意の順序（または予約注文）関係$\mathrm{R}\{x, y\}$に適用されますが、主に$\mathrm{R}\{x, y\}$$x \leqslant y$が書かれている場合に使用されます。 \*(整数または実数間の通常の順序関係との類推による)\* (または $x \subset y$、または類似の符号による);したがって、記法 $x \leqslant y$ についてのみ記載し、他の記法に転記する作業は読者に委ねます。 $\mathrm{R}\{x, y\}$ が $x \leqslant y$ と書かれている場合、$y \geqslant x$ は $x \leqslant y$ と同義であり、これらの関係は、「$x$ は $y$ より *小さい*」、または「$x$ は $y$ より *小さい*」、または「$y$ は $x$ より *大きい*」または「$y$ は $x$ より *大きい*」。 関係 $x \geqslant y$ は予約注文関係 (*間* $x$ *と* $y$) $x \leqslant y$の*反対側*です。

言葉の乱用により、私たちはしばしば「関係 $x \leqslant y$」の代わりに「関係 $\leqslant$」について話すことになります。この場合、「関係 $\geqslant$」は「関係 $\leqslant$」の反対です。また、同じ証明において、混同の危険がない場合には、複数の異なる順序関係を表すために同じ記号 $\leqslant$ を使用する場合があることにも注意します。

集合 E に順序関係が$x \leqslant y$ と書かれた関係に対する条件は次のとおりです。

(RO$_{\mathrm{I}}$) *関係 「$x \leqslant y$ と $y \leqslant z$」は $x \leqslant z$ を意味します。*
(RO$_{\mathrm{II}}$) *関係「$x \leqslant y$と$y \leqslant x$」は$x = y$を意味します。*
(RO$_{\mathrm{III}}$) *関係 $x \leqslant y$ は「$x \leqslant x$ と $y \leqslant y$」を意味します。*
(RO$_{\mathrm{IV}}$) *関係 $x \leqslant x$ は $x \in \mathrm{E}$ に相当します。*

条件 (RO$_{\mathrm{II}}$) を省略すると、$x \leqslant y$ が E で先順位関係になる条件が得られます。
¶ 順序関係が $x \leqslant y$ と書かれている場合、「$x \leqslant y$ と $x \neq y$」の関係については $x < y$ (または $y > x$) と書きます。これらの関係は、「$x$ は $y$ より *厳密に小さい*」、または「$x$ は $y$ より *厳密に小さい*」、または「$y$ は $x$ より *厳密に大きい*」、または「$y$ は $x$ より *厳密に大きい*」と読み取られます。

包含関係の例は、$x \leqslant y$ ($x \nleqslant y$ で示されるときどき) の否定が $y < x$ (cf. no. 12) と *必ずしも等価ではない* ことを示しています。

C58。 *$\leqslant$ を順序関係とし、$x$、$y$ を 2 つの異なる文字とします。 関係 $x \leqslant y$ は「$x < y$ または $x = y$」に相当します。 関係「$x \leqslant y$と$y < z$」、「$x < y$と$y \leqslant z$」はそれぞれ$x < z$を意味します。*

最初の主張は、基準 $A \Rightarrow ((A$ および ($B$)) または $B$) (章 I, § 3、基準 C24) から続きます。 2 番目の主張を証明するには、各仮説が推移性までに $x \leqslant z$ を暗示していることに注意します。そして、関係 ($x = z$ と $x \leqslant y$ と $y \leqslant z$) は、仮定とは反対に、$x = y = z$ を暗示します。

¶ 順序では、物事を簡単にし、数学的定理によるメタ数学的基準を置き換える考慮するために、通常は理論 $\mathscr{T}$ 含む集合の理論の公理と公理スキーム、加法では 2 つの定数 E と$\Gamma$ 満たす公理

「$\Gamma$は集合E」(no. 1)の注文です。

$x \leqslant y$ 関係 $y \in \Gamma\langle x \rangle$ で表し、集合 E は *順序付け* $\Gamma$ (または順序関係 $y \in \Gamma\langle x \rangle$) (cf. 章 IV, § 1) であると言います。

¶ $\mathscr{T}$ において、$\Gamma$ が E に対する事前順序付けであるとき、同様に、E は *事前順序付け* $\Gamma$ によって *事前順序付けされていると言います。

状況によっては (たとえば、次の定義)、これから検討する理論はもう少し複雑になります。このような理論の定数と公理を明確にするのは読者に任せます。

E、E$'$を、順序$\Gamma$、$\Gamma'$によって順序付けられた2つの集合とします。 * E *onto* E$'$ の *同型 (順序 $\Gamma$ と $\Gamma'$ の場合) は、E の全単射 $f$ から E$'$ となり、関係 $x \leqslant y$ と $f(x) \leqslant f(y)$ は等価です (cf.) 章 IV, § 1）。

### 4. 部分集合を注文しました。 順序集合中積

グラフ G を使用して、E を順序付け $\Gamma$ で順序付けする集合とします。E の各部分集合 A について、$G \cap (A \times A)$ は A の順序付けです。 対応する順序関係は「$x \leqslant y$ と $x \in A$ と $y \in A$」に相当し、単純に $x \leqslant y$ で表します（言葉の乱用により）。このように A で定義された順序と順序関係は、E で与えられた順序と順序関係によって *誘発される*と言われます。そして、E 上の順序と順序関係は、順序の *拡大* と順序関係で、A では誘導するであると言われます。 A を順序付き集合と考えるときはいつでも、E 上の順序によって A に誘発される順序、〜でない限りを念頭に置いています。と明記されています。

*例*。 部分集合のさまざまな集合に関係 $X \subset Y$ を含めることによって引き起こされる関係は、非常に重要です。 例の一部をご紹介します。

#### 例 1 {#ens-iii-s1-n4-exa-1 .statement tag=03WB}

E、Fを2つの集合とし、$\Phi(E, F)$をEの部分集合のすべての写像の集合とします。それぞれの$f \in \Phi(E, F)$について、$G_f$を$f$、つまり$E \times F$の部分集合のグラフとします。 $\Phi(E, F)$ に $f$ と $g$ (no. 1, 例 3) の間の順序関係 "*g 拡大する f*" を与えると、$f \to G_f$ は順序の同型になります。 集合 $\Phi(E, F)$ を $\mathfrak{P}(E \times F)$ の部分集合に含めて順序付けします。

#### 例 2 {#ens-iii-s1-n4-exa-2 .statement tag=03WC}

集合 E の各分割 $\varpi$ について、$\tilde{\varpi}$ を E 上の $\varpi$ によって定義される同値関係のグラフとします。 写像 $\varpi \to \tilde{\varpi}$ は、集合 $\mathfrak{L}$ の同型です。 E の分割、関係によって順序付けられ、$\varpi$ と $\varpi'$ (no. 1、例 4) の間の「$\varpi$ は $\varpi'$ よりより細かいである」を、$\mathfrak{P}(E \times E)$ の部分集合に含めて順序付けします。

#### 例 3 {#ens-iii-s1-n4-exa-3 .statement tag=03WD}

E を集合とし、$\Omega \subset \mathfrak{P}(E \times E)$ を E (no. 2) 上の *事前注文* のグラフの集合とします (または、言葉の乱用により、E 上のすべての事前注文の集合) とします。 $s$ と $t$ の間の順序関係 $s \subset t$ は、$\mathfrak{P}(E \times E)$ に関係を含めることによって$\Omega$ に誘導され、というによって「事前順序付け$s$ は *より細かい* である」と表現されます。 $t$」（または「$t$は$s$より*粗い*」）。 $x(s)y$ と $x(t)y$ がそれぞれ E の予約注文関係 $(x, y) \in s$ と $(x, y) \in t$ を表すものとします。次に、$s$ がより細かいであるということは、$t$ がというであるということは、関係 $x(s)y$ が *暗黙的に $x(t)y$ であることを意味します。

$(E_\iota)_{\iota \in I}$ を集合の族とし、各添字 $\iota \in I$ に対して $\Gamma_\iota$ を $E_\iota$ の順序とします。 $G_\iota \subset E_\iota \times E_\iota$ をそのグラフとし、$x_\iota \leqslant y_\iota$ が $E_\iota$ 上の順序関係 $(x_\iota, y_\iota) \in G_\iota$ を表すものとします。 積集合 $F = \prod_{\iota \in I} E_\iota$、関係

$$(\forall \iota) \, ((\iota \in I) \Rightarrow (x_\iota \leqslant y_\iota))$$

すぐに確認できるように、$x = (x_\iota)$ と $y = (y_\iota)$ の間の順序関係です。 F で定義された順序と順序関係は、順序* $\Gamma_\iota$ の *積と順序関係* $x_\iota \leqslant y_\iota$ の *積と呼ばれます。この関係は $x \leqslant y$ と書かれ、順序 $\Gamma_\iota$ の積によって順序付けられた集合 F は、順序集合* $E_\iota$ の *積と呼ばれます。

F での積順序のグラフは、$\prod_{\iota \in I} (E_\iota \times E_\iota)$ の標準写像から $F \times F$ (章 II, § 5, no. 5) の下で、積集合 $\prod_{\iota \in I} G_\iota$ の像であることがすぐに検証されます。

順序集合の積の重要な例は、集合Eの写像を順序付けられた集合Fに変換したグラフの集合$F^E$です。$F^E$の正規の全単射があります。 E の写像の集合 $\mathfrak{F}(E, F)$ を F に変換し、この写像は、順序付けられた集合 $F^E$ の同型を $\mathfrak{F}(E, F)$ に移すものであり、すべての関係によって定義された順序付けが施されています。 E の 2 つの写像 $f$、$g$ を F にすると、$x \in E$、$f(x) \leqslant g(x)$」になります。この関係は、$f \leqslant g$ と書かれます。

☡

集合 $\mathfrak{F}(E, F)$ の順序では、関係 $f < g$ が意味することに注意してください。
$$\text{"for all } x \in E, f(x) \leqslant g(x), \text{ and there exists } y \in E \text{ such that } f(y) < g(y)\text{"}$$
*そうではない*
$$\text{"for all } x \in E, f(x) < g(x)\text{"}.$$

順序では、混乱を避けるために、この状況では記法 $f < g$ を使用しない方がよいでしょう。

この小節の定義は、「注文」が全体を通して「予約注文」に置き換えられる場合、予約注文されたセットに変更を適用せずに適用されます。

### 5. 増加する写像

#### 定義 1 {#ens-iii-s1-def-1 .statement tag=03JC}

* E * と * F * を事前注文セット* とします (* 事前注文関係をそれぞれ * $\leqslant$ で示します)。 *写像 f of* E *into* F *は増加する* (または *順序保持*) *関係* $x \leqslant y$ *暗示* $f(x) \leqslant f(y)$; *それは減少する* (または *順序反転*) *関係* $x \leqslant y$ の場合 *$f(x) \geqslant f(y)$ を *暗示します。 * E *into* F *の*写像が増加するか減少するの場合は単調と言われます。

E から F への増加する写像は、反対の事前順序付けによって E または F 上の事前順序付けの *1* を置き換えるにすると、減少する (逆も同様) になります。  すべての *定数* 写像は、増加すると減少するの両方です。この主張の逆は通常は真実ではありません。

たとえば、集合 E が等式関係で順序付けされている場合、それ自体に対する E の恒等写像は増加すると減少するの両方になりますが、E に複数の元 (cf. 練習問題) がある場合は定数ではありません。 7)。

#### 定義 2 {#ens-iii-s1-def-2 .statement tag=03JD}

*E * と * F * を 2 順序集合とします。 写像 f of* E *into* F *は真に増加する* (または *厳密に順序保持*) *関係* $x < y$ *暗黙* $f(x) < f(y)$; であると言われています。 *f は真に減少する* (または *厳密に順序反転*) であると言われています。 *関係* $x < y$ の場合 *$f(x) > f(y)$ を *暗示します。 * E *into* F *の*写像は、真に増加するまたは真に減少するの場合、厳密に単調であると言われます。

*例*

#### 例 1 {#ens-iii-s1-n5-exa-1 .statement tag=03SK}

E を集合とします。  $\mathfrak{P}(E)$ の写像 $X \rightarrow E - X$ (包含順) をそれ自体に適用すると、真に減少するになります。

#### 例 2 {#ens-iii-s1-n5-exa-2 .statement tag=03SL}

E を順序付き集合とします。それぞれの $x \in E$ について、$U_x$ をすべての $y \in E$ の集合とし、$y \geqslant x$ とします。 写像 $x \to U_x$ は、E の真に減少する写像を $\mathfrak{P}(E)$ に変換します (包含順)。実際、関係 $x \leqslant y$ は $U_x \supset U_y$ と同等です。

順序付き集合 E から順序付き集合 F への単調単調写像は *厳密に単調 * です。 逆は通常は true ではありません。関係 $x \leqslant y$、$x \geqslant y$ のどちらも true でない場合に $f(x) = f(y)$ が発生する可能性があるためです (cf. no. 12、命題 11)。

¶ 順序付き集合 E から順序付き集合 E' への全単射写像 $f$ は、$f$ とその逆写像の両方が次の場合に限り、E から E' への同型 (no. 3) です。 増加する。

¶ I が *順序* 添字集合である場合、$\iota \to X_\iota$ が増加する写像である場合、部分集合* $(X_\iota)_{\iota \in I}$ の集合 E は *増加する* であると言われます。 I を $\mathfrak{P}(E)$ に含めて順序付けします (他の語、$\iota \leqslant \varkappa$ が $X_\iota \subset X_\varkappa$ を意味する場合)。同様に、私たちは定義する部分集合 $(X_\iota)_{\iota \in I}$ の *減少する、真に増加する、*、または *真に減少する* 家族です。

#### 命題 2 {#ens-iii-s1-prop-2 .statement tag=03JE}

*E、E'を*2の順序集合とし、* $u : E \to E'$ *と* $v : E' \to E$ *2の減少する写像とし、すべて* $x \in E$ *とすべて* $x' \in E'$ *ある* $v(u(x)) \geqslant x$ *と* $u(v(x')) \geqslant x'$。 *それから*

$$u \circ v \circ u = u \quad \textit{and} \quad v \circ u \circ v = v.$$

関係 $v(u(x)) \geqslant x$ は、$u$ が減少するであるため、$(u(v(u(x))) \leqslant u(x)$ を意味します。一方、不等式 $u(v(x')) \geqslant x'$ では、置き換えることによって $u(v(u(x))) \geqslant u(x)$ $u(x)$ によって $x'$ が得られます。従って、最初の等式です。 2番目の証明も同様です。

### 6. 最大値と最小値元

#### 定義 3 {#ens-iii-s1-def-3 .statement tag=03JF}

*E *を順序付けられた集合とします。 元* $a \in E$ *は最小* (または *最大*) *元 of* E *if 関係* $x \leqslant a$ (または $x \geqslant a$) *暗黙* $x = a$と言われています。

E のすべての最小元は、逆の順序に関しては極大元であり、その逆も同様です。

*例*

#### 例 1 {#ens-iii-s1-n6-exa-1 .statement tag=03SM}

A を集合とします。 A の空ではない部分集合の $\mathfrak{P}(A)$ の部分集合 (包含順) からなるでは、最小の元は単一の元の部分集合からなるです。

#### 例 2 {#ens-iii-s1-n6-exa-2 .statement tag=03SN}

E の部分集合の写像の集合 $\Phi(E, F)$ を F (F は空ではない) に変換し、$u$ と $v$ の間で関係 "$v$ 拡大する $u$" で順序付けすると、極大元は次のようになります。 E全体の写像をFに。

#### 例 3 {#ens-iii-s1-n6-exa-3 .statement tag=03SO}

\* $m$ と $n$ の間で関係 "$m$ 割る $n$" で順序付けされた自然な整数 $> 1$ の集合では、最小の元は素数数です。 \*

#### 例 4 {#ens-iii-s1-n6-exa-4 .statement tag=03SP}

\* 実数の集合には極大元も最小の元もありません。 \*

### 7. 最大の元以上元

すべての $x \in E$ に対して $a \leqslant x$ となるような順序付けられた集合 E に元 $a$ が存在する場合、$a$ は、この性質を持つ E の*唯一* の元になります。 for if also $b \leqslant x$ for all $x \in E$, then we should have $a \leqslant b$ and $b \leqslant a$, and consequently $a = b$.

#### 定義 4 {#ens-iii-s1-def-4 .statement tag=03JG}

*E *を順序付けられた集合とします。 元* $a \in E$ *is said to be the* least (resp. *最大の*) *元 of* E *if for all* $x \in E$ *we have* $a \leqslant x$ (resp. $x \leqslant a$).

注文された集合には最大の元も、少なくとも元も必要ありません。 E が少なくとも元 $a$ を持つ場合、反対の順序に関して $a$ は最大の元になります。

¶ E に最小の元 $a$ がある場合、$a$ は E の *一意の最小値元* です。なぜなら、$x \in E$ が $a$ と異なる場合、$a < x$ があるからです。

*例*

#### 例 1 {#ens-iii-s1-n7-exa-1 .statement tag=03SQ}

$\mathfrak{S}$ を空ではない部分集合 of 集合 $\mathfrak{P}(E)$ of 部分集合 of 集合 E とします。$\mathfrak{S}$ が包含関係に関して最小 (それぞれ最大の) 元 A を持つ場合、A は次のようになります。 $\mathfrak{S}$の集合の共通部分（それぞれ和集合）。逆に、$\mathfrak{S}$ 属するの集合の共通部分 (それぞれ和集合) から $\mathfrak{S}$ の場合、$\mathfrak{S}$ の最小 (それぞれ最大の) 元になります。

#### 例 2 {#ens-iii-s1-n7-exa-2 .statement tag=03SR}

特に、$\emptyset$ は $\mathfrak{P}(E)$ の最小の元と E 最大の元です。 E のサブセットから F へのマッピングの集合 $\Phi(E, F)$ をマッピングの拡張順に並べたもの (no. 1、例 3) では、空のマッピングが最小要素であり、F が単一の要素で構成されない限り最大の要素はありません。 $E \times E$ の対角線 $\Delta$ は、E 上の同値関係 (または E 上の事前順序付けの集合) のグラフの集合の最小の元です。

#### 命題 3 {#ens-iii-s1-prop-3 .statement tag=03JH}

* E * を順序付けられた集合とし、* E$'$ * E * の互いに素和集合と、単一の元の集合* $\{a\}$ *からなるとします。次に、* E$'$ * 上に一意の順序付けが存在します。* E 上で指定された順序付けは誘導するであり、* $a$ * は * E$'$ の最大の元です。

G が E の順序付けのグラフである場合、命題の条件を満たす E$'$ の順序付けのグラフは、G の和集合 G$'$ およびすべての対 $(x, a)$ の集合でなければなりません。ここで、$x \in E'$;逆に、G$'$ は、与えられた条件を満たす E$'$ の順序付けのグラフであることは明らかです。

¶ 順序付けられた集合 E$'$ は、最大の元* $a$ *を * E (cf. 練習問題 3) に *隣接させることによって得られると言われます。

¶ 予約注文された集合 $E$ の部分集合 $A$ は、$x\in E$ ごとに $x\leq y$ (それぞれ $y\leq x$) となる $y\in A$ が存在する場合、$E$ の *cofinal* (それぞれ *coinitial*) であると言われます。したがって、順序付けられた集合 $E$ に最大の (それぞれ最小) 元があると言うことは、$E$ が単一の元の共終点 (それぞれコインイニシャル) 部分集合からなるを持つことを意味します。

### 8. 上と下界

#### 定義 5 {#ens-iii-s1-def-5 .statement tag=03JI}

*$E$を予約済みの集合、$X$を$E$の部分集合とします。すべての $y\in X$ に対して $x\leq y$ (または $x\geq y$) となるような任意の元 $x\in E$ は、$E$ の $X$ の下限 (または上限) と呼ばれます。

逆の順序では、$X$ のすべての上界は $X$ の下界であり、その逆も同様です。

¶ $x$ が $X$ の下界である場合、すべての元 $z\leq x$ は $X$ の下界でもあります。 $X$の下界は、$X$の各部分集合の下界でもあります。 属するから $X$ までの $X$ の下界が存在する場合に限り、注文された集合 $X$ は最小の元を持ちます。

¶ 事前順序付けされた集合 $E$ の部分集合 $X$ の下限の集合は空である可能性があります。これは、$X=E$ と $E$ が最小要素を持たない順序付き集合である場合に当てはまります。

¶ $E$ の部分集合 $X$ のうち、下限 (または上限) の集合が空ではないものは、*下に境界がある* (または *上に境界がある*) と言われます。上下両方に有界のある部分集合は *有界* と言われます。 $X$ が下に境界がある場合 (それぞれ、上に境界があり、境界がある場合)、同じことが $X$ のすべての部分集合にも当てはまります。

単一の元のすべての部分集合からなるは有界です。ただし、2 つの元のうち部分集合からなるは、上下 (no. 10) のいずれかに制限される必要はありません。

$E$ を事前注文された集合とし、$f$ を任意の集合 $A$ から $E$ への写像とします。 集合 $f(A)$ が $E$ で下に制限されている場合 (言葉の乱用により)、マッピング $f$ は *下に制限* (それぞれ *上に制限、制限*) されると言われます。

### 9. 少なくとも上界と最大の下界

#### 定義 6 {#ens-iii-s1-def-6 .statement tag=03JJ}

*$E$ を順序付けられた集合とし、$X$ を $E$ の部分集合とします。 $E$ の要素は、$E$ の $X$ の下限 (または上限) セットの最大 (または最小) 要素である場合、$E$ の $X$ の最大の下限または下限 (それぞれ最小上限または最高値) であると言われます。

順序付けられた集合 $E$ の部分集合 $X$ が与えられた場合、$E$ の $X$ の最小上界 (それぞれ最大の下界) が存在する場合、それは次のように表されます。

$$
\sup_E X\quad\text{(resp. }\inf_E X\text{)}
$$

または、あいまいさの危険がない場合は、sup X (resp. inf X) によって。 2 つの元のうち、集合 $\{x, y\}$ の最小の上界 (それぞれ最大の下界) が存在する場合、sup $(x, y)$ (それぞれ inf $(x, y)$) で表されます。同様に、3 つの元のうち、集合の最小の上界と最大の下界なども同様です。

¶ E の部分集合 X に最大の元 $a$ がある場合、$a$ は E の X の最小の上界です。

¶ X が E に最大の下界 $a$ をもつ場合、E の反対の順序に関して、$a$ は X の最小の上界です。 このため、以下では、最小の上界の特性を考慮するために、ほとんどの部分を制限することができます。

*例*

(1) 順序付けられた集合 E 内の空の集合 $\emptyset$ の上界の集合は、明らかに E そのものです。したがって、E に *最小* 元がある場合に限り、$\emptyset$ は E に最高値を持ちます。その場合、それは $\emptyset$ の *最小* 上界* になります。

(2) 包含順に並べた、集合 E の部分集合の集合 $\mathfrak{P}(E)$ では、$\mathfrak{P}(E)$ のすべての部分集合 $\mathfrak{S}$ には少なくとも上界があり、つまり、$\mathfrak{S}$ の集合の *和集合* があり、 最大の下界、つまり$\mathfrak{S}$の集合の*共通部分*です。

(3) E, F を 2 つの集合とし、$\Theta$ を E の写像の部分集合の $\Phi(E, F)$ の部分集合とし、写像の拡大で順序付けします (no. 1, 例 3)。それぞれの $u \in \Phi(E, F)$ について、$D(u)$ を $u$ のドメインとします。 写像所属から $\Phi(E, F)$ (章 II, § 4, no. 6, 命題 7) の家族の共通の拡大の存在に対する条件は、$\Theta$ が最小の上界を持っていることを示しています。 $\Phi(E, F)$ 対 $(u, v)$、元、$\Theta$ のそれぞれについて、$x \in D(u) \cap D(v)$ のときはいつでも $u(x) = v(x)$ があります。

集合 A の順序集合 E への写像 $f$ は、画像 $f(A)$ が E に最小上限を持つ場合、最小上限を持つと言われます。この境界は *f* の最小上限と呼ばれ、$\sup_{x \in A} f(x)$ と書かれます。 最大の下界についても同様です。

特に、E の部分集合 A が E に最小の上界を持っている場合、この境界は A の E への標準単射の最小の上界であるため、$\sup_{x \in A} x$ と書くことができます。

#### 命題 4 {#ens-iii-s1-prop-4 .statement tag=03JK}

*E *を順序付けられた集合とし、* A を * E に最大の下界と少なくとも上界の両方を持つ * E の部分集合とする。 *その後* $\inf A \leqslant \sup A$ *場合* $A \neq \emptyset$; *if* $A = \emptyset$, $\sup A$ *が最小かつ* $\inf A$ *最大の元の* E.

これは定義の直後に続きます。

#### 命題 5 {#ens-iii-s1-prop-5 .statement tag=03JL}

*E を順序付けられた集合とし、* A、B を * E の 2 つの部分集合とし、*それぞれが少なくとも上界* (それぞれ *最大の下界*) を *E に含めます。 *If* $A \subset B$、*then* $\sup A \leqslant \sup B$ (それぞれ$\inf A \geqslant \inf B$）。

#### 系 {#ens-iii-s1-n9-cor-1 .statement tag=03JM}

*$(x_\iota)_{\iota \in I}$ を、*$\mathrm{E}$ に少なくとも上界がある、注文された集合* $\mathrm{E}$ の元のファミリーとします。 *もし* $\mathrm{J}$ *が* $\mathrm{I}$の部分集合で、*家族* $(x_\iota)_{\iota \in J}$ *$\mathrm{E}$に*少なくとも上界がある場合、*$\sup\limits_{\iota \in J} x_\iota \leqslant \sup\limits_{\iota \in I} x_\iota$があります。

#### 命題 6 {#ens-iii-s1-prop-6 .statement tag=03JN}

*$(x_\iota)_{\iota \in I}$、$(y_\iota)_{\iota \in I}$ * を、順序付けられた集合* $\mathrm{E}$ の元の 2 つのファミリーとし、 *同じ集合* $\mathrm{I}$ によってインデックス付けされ、 * そしてそのような* $x_\iota \leqslant y_\iota$ *すべて* $\iota \in \mathrm{I}$ となります。 *両方の家族が $\mathrm{E}$ に少なくとも上界を持っている場合、*その後* $\sup\limits_{\iota \in I} x_\iota \leqslant \sup\limits_{\iota \in I} y_\iota$ になります。

$a = \sup\limits_{\iota \in I} y_\iota$ は $y_\iota$ の集合の上界であるため、すべての $\iota \in \mathrm{I}$ に対して $x_\iota \leqslant y_\iota \leqslant a$ となり、したがって $\sup\limits_{\iota \in I} x_\iota \leqslant a$ となります。

#### 命題 7 {#ens-iii-s1-prop-7 .statement tag=03JO}

*$(x_\iota)_{\iota \in I}$ * を注文された集合* $\mathrm{E}$ の元のファミリーとし、*そして * $(\mathrm{J}_\lambda)_{\lambda \in L}$ * を添字集合* $\mathrm{I}$ のカバーとします。 *各サブファミリー* $(x_\iota)_{\iota \in J_\lambda}$ * $\mathrm{E}$ に少なくとも上界があるとします。 *家族* $(x_\iota)_{\iota \in I}$ *少なくとも上界インチ* $\mathrm{E}$ であれば、*家族* $\left( \sup\limits_{\iota \in J_\lambda} x_\iota \right)_{\lambda \in L}$ * 少なくとも上界インチ* $\mathrm{E}$ があれば十分であり、*そして私たちは*

$$(1) \qquad \sup_{\iota \in I} x_\iota = \sup_{\lambda \in L} \left( \sup_{\iota \in J_\lambda} x_\iota \right).$$

$b_\lambda = \sup\limits_{\iota \in J_\lambda} x_\iota$ にしましょう。 $(x_\iota)_{\iota \in I}$ に最小の上界 $a$ があるとします。次に、$\lambda \in \mathrm{L}$ ごとに $a \geqslant b_\lambda$ (系 ～ 命題 5)。一方、$\lambda \in \mathrm{L}$ ごとに $c \geqslant b_\lambda$ がある場合、$(\mathrm{J}_\lambda)_{\lambda \in L}$ は $\mathrm{I}$ をカバーするため、$\iota \in \mathrm{I}$ ごとに $c \geqslant x_\iota$ になります。したがって $c \geqslant a$ は次のことを証明します。

$$a = \sup_{\lambda \in L} b_\lambda.$$

逆に、家族 $(b_\lambda)_{\lambda \in L}$ が最小の上界 $a'$ を持っているとします。次に、すべての $\iota \in \mathrm{I}$ に対して $a' \geqslant x_\iota$ です。一方、すべての $\iota \in \mathrm{I}$ に対して $c' \geqslant x_\iota$ である場合、特に

$$c' \geqslant \sup_{\iota \in J_\lambda} x_\iota = b_\lambda$$

それぞれの $\lambda \in \mathrm{L}$ に対して、$c' \geqslant a'$ となるので、

$$a' = \sup_{\iota \in I} x_\iota.$$

#### 系 {#ens-iii-s1-n9-cor-2 .statement tag=03JP}

*$(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *を、順序付けられた集合* $\mathrm{E}$ の元の「ダブル」ファミリーとし、*それぞれ* $\mu \in \mathrm{M}$ *ファミリー* $(x_{\lambda\mu})_{\lambda \in L}$ * $\mathrm{E}$ に少なくとも上界が含まれるようにします。 *家族* $(x_{\lambda\mu})_{(\lambda,\ \mu) \in L \times M}$ *少なくとも上界 in* $\mathrm{E}$ であれば、*家族* $\left( \sup\limits_{\lambda \in L} x_{\lambda\mu} \right)_{\mu \in M}$ *少なくとも* *上界 in* E があれば十分であり、*そして私たちは*

$$(2) \qquad \sup_{(\lambda,\,\mu)\in L\times M} x_{\lambda\mu} = \sup_{\mu\in M}\left(\sup_{\lambda\in L} x_{\lambda\mu}\right).$$

#### 命題 8 {#ens-iii-s1-prop-8 .statement tag=03QI}

*$(E_\iota)_{\iota\in I}$ *順序集合の家族にしましょう。 * A *を積の部分集合として集合* $E = \prod_{\iota\in I} E_\iota$ を注文し、*そして * $A_\iota = \mathrm{pr}_\iota A$ *それぞれに* $\iota \in I$ を与えます。 *A が * 上界を * E に持つには、 * それぞれ * $\iota \in I$、$A_\iota$ * $E_\iota$ に * 少なくとも上界が必要であり、 * そして、次のようになります*

$$\sup A = (\sup A_\iota)_{\iota\in I} = \left(\sup_{x\in A} \mathrm{pr}_\iota x\right)_{\iota\in I}.$$

それぞれの $\iota \in I$ について、$A_\iota$ の $E_\iota$ には少なくとも上界 $b_\iota$ があるとします。 $c = (c_\iota)$ が A の上界であると言うことは、各 $\iota \in I$ に対して $c_\iota \geqslant b_\iota$ であることを意味します。従って、$(b_\iota)_{\iota\in I}$ は A の上界です。 逆に、A が最小の上界 $a = (a_\iota)_{\iota\in I}$ を持っていると仮定します。それぞれの $\varkappa \in I$、$a_\varkappa$ は、$A_\varkappa$ の上界です。なぜなら、$x_\varkappa \in A_\varkappa$ の場合、$A_\varkappa$ の定義までに $\mathrm{pr}_\varkappa x = x_\varkappa$ となるような $x \in A$ が存在するからです。一方、$a'_\varkappa$ が $E_\varkappa$ の $A_\varkappa$ の上界である場合、元 $c' = (c'_\iota)_{\iota\in I}$ は、

$$c'_\iota = a_\iota \quad \text{for} \quad \iota \neq \varkappa \qquad \text{and} \qquad c'_\varkappa = a'_\varkappa$$

Aの上界です。従って、$c' \geqslant a$、従って$a'_\varkappa \geqslant a_\varkappa$;従って、$a_\varkappa$ は、$E_\varkappa$ の $A_\varkappa$ の最小の上界です。

☡

¶ F を順序付き集合 E の部分集合とし、A を F の部分集合とします。 2 つの元 $\sup_E A$、$\sup_F A$ のうちの 1 つが存在するが、もう 1 つが存在しない、または両方が存在するが等しくないことが起こります。

*例*

#### 例 1 {#ens-iii-s1-n9-exa-1 .statement tag=03SS}

\* 実数の順序付き集合 $E = \mathbf{R}$ で、有理数数の部分集合 $F = \mathbf{Q}$ と有理数数 $< \sqrt{2}$ の集合 $A \subset F$ を考慮します。 $\sup_E A$ は存在しますが、$\sup_F A$ は存在しません。

#### 例 2 {#ens-iii-s1-n9-exa-2 .statement tag=03ST}

例 1 の記法では、G を A の和集合および集合 $\{2\}$ とします。この場合、$G \subset F$ と $\sup_G A$ は存在しますが、$\sup_F A$ は存在しません。

#### 例 3 {#ens-iii-s1-n9-exa-3 .statement tag=03SU}

同じ記法、$\sup_E A = \sqrt{2}$、$\sup_G A = 2$。 \*

ただし、次の結果が得られます。

#### 命題 9 {#ens-iii-s1-prop-9 .statement tag=03QJ}

*E *を順序付けられた集合、* F *部分集合 of* E、A *部分集合 of* F とする。 *両方* $\sup_E A$ * と* $\sup_F A$ *が存在する場合、* $\sup_E A \leqslant \sup_F A$ が得られる。 *もし* $\sup_E A$ *が存在し、 属するが* Fであれば、*そのとき* $\sup_F A$ *が存在し、$\sup_E A$と等しい*。

最初の主張は、FのAの上界の集合$\mathrm{M}$が、EのAの上界の集合Nに含まれるという事実と、命題5から続きます。一方、Nの最小の元がFにある場合、それはMに属するになります。そして明らかに M の中で最も小さい元です。これは 2 番目の主張を証明します。

### 10. 有向集合

#### 定義 7 {#ens-iii-s1-def-7 .statement tag=03QK}

*事前順序付けされた集合* E *は右向きであると言われます* (それぞれ *左向き*) *2 つの元のすべての部分集合が * 上に境界がある* (または *下に境界がある*) 場合。

「正しく指示された」の代わりに、「関係 $\leqslant$ に関して指示された」という表現や、予約注文関係が他の記号で示される場合の類似の表現をよく使用します。たとえば、$\mathfrak{S}$ が集合 A の部分集合の集合である場合、各部分集合 $\{\mathrm{X}, \mathrm{Y}\}$ について、$\mathfrak{S}$ は *関係* $\subset$ (それぞれ $\supset$) に関して指示されていると言います。 $\mathfrak{S}$ の 2 つの元のうちからなるには、$\mathrm{X} \subset \mathrm{Z}$ と $\mathrm{Y} \subset \mathrm{Z}$ (それぞれ $\mathrm{X} \supset \mathrm{Z}$ と $\mathrm{Y} \supset \mathrm{Z}$) のような $\mathrm{Z} \in \mathfrak{S}$ が存在します。

*例*
(1) 最大の元を持つ順序付けられた集合は右方向です。
\* (2) トポロジー 空間では、点の近傍の基本的な系が関係 $\supset$ に関して方向付けられています。
(3) 任意の加群の有限型の部分加群の集合は、関係$\subset$に関して方向付けられます。 \*

#### 命題 10 {#ens-iii-s1-prop-10 .statement tag=03QL}

*右向きの順序集合* E では、*極大元 a は * E の最大の元です。

$x \in \mathrm{E}$ ごとに、$x \leqslant y$ と $a \leqslant y$ のように仮定 $y \in \mathrm{E}$ が存在します。 $a$ が最大なので、$y = a$ です。

¶ 右方向の事前順序付け集合は、反対の順序付けに関しては左方向です。右有向集合の積は右向きです。一方、右有向集合の部分集合は、必ずしも右向きであるとは限りません。ただし、右有向集合 E の *コファイナル* 部分集合 F は常に右方向です。与えられた $x$、$y \in \mathrm{F}$ に対して、$x \leqslant z$ および $y \leqslant z$ のような $z \in \mathrm{E}$ が存在し、次に $z \leqslant t$ のような $t \in \mathrm{F}$ が存在します。

### 11. 格子

#### 定義 8 {#ens-iii-s1-def-8 .statement tag=03QM}

*順序付けられた集合* E * 2 つの元の部分集合からなるごとに * E に少なくとも上界と最大の下界がある場合、格子であると言われます。

格子のすべての積は格子です。これは、順序集合 (no. 9、命題 8) の積に少なくとも上界が存在するという条件の結果になります。 A の 2 つの部分集合のうち和集合と共通部分が再び A の部分集合であるため、包含順に並べた集合 A の部分集合の集合は格子です。

*例*

#### 例 1 {#ens-iii-s1-n11-exa-1 .statement tag=03SV}

\* $m$ と $n$ の間の関係 「$m$ 割る $n$」で順序付けされた整数 $\geqslant 1$ の集合は格子です。 $\{m,n\}$ のうち最小の上界が l.c.m です。 $m$ と $n$ 、および最大の下界は彼らの h.c.f. です。

#### 例 2 {#ens-iii-s1-n11-exa-2 .statement tag=03TT}

群 G の部分群の集合は、包含順に並べると格子です。

#### 例 3 {#ens-iii-s1-n11-exa-3 .statement tag=03TU}

集合 A 上のトポロジーの集合は、$\mathscr{T}$ と $\mathscr{T}'$ の間の関係 「$\mathscr{T}$ は$\mathscr{T}'$ より粗い」で順序付けされており、格子です。 (*一般位相*、章 I, § 2)。

#### 例 4 {#ens-iii-s1-n11-exa-4 .statement tag=03TV}

$\mathbf{R}$ の区間 I で定義されたすべての実数値写像の集合 $\mathfrak{F}(I,\mathbf{R})$ は、順序関係 $f\leqslant g$ (no. 4) に関する格子であり、それ自体と同型です。 積 $\mathbf{R}^{I}$。 \*

#### 注意 {#ens-iii-s1-n11-rem-1 .statement tag=03JQ}

格子は明らかに左右両方の方向を向いています。しかし、左と右の両方に向けられた順序付けられた集合は、必ずしも格子であるとは限りません。 \* 後者の例は、写像 $x\mapsto p(x)$ の $\mathbf{R}$ の集合です。ここで、$p$ は $\mathbf{R}[X]$ の多項式であり、この集合は関係 $p\leqslant q$ (no. 4) によって順序付けされます。 \*

### 12. 合計順序集合

#### 定義 9 {#ens-iii-s1-def-9 .statement tag=03JR}

*予約注文された集合 E の 2 つの元 $x$、$y$ は、関係 「$x\leqslant y$ または $y\leqslant x$」が真の場合、同等であると言われます。 集合 E は、順序付けされており、E の 2 つの元が比較可能な場合、完全に順序付けされていると言われます。 E の順序は合計順序、対応する順序関係は合計順序関係であると言われます。

$x$ と $y$ が完全に順序付けられた集合の元である場合、$x=y$ または $x<y$ または $x>y$ になります。したがって、$x\leqslant y$ の否定は $x>y$ になります。

E の順序付けは、そのグラフ G が関係 $G\cup\overset{-1}{G}=E\times E$ および関係 $G\circ G=G$ および $G\cap\overset{-1}{G}=\Delta$ を満たす場合に限り、全順序付けとなります。

*例*

#### 例 1 {#ens-iii-s1-n12-exa-1 .statement tag=03SW}

完全に順序付けされた集合のすべての部分集合は、誘導順序付けによって完全に順序付けされます。

#### 例 2 {#ens-iii-s1-n12-exa-2 .statement tag=03TW}

E を任意の順序の集合とします。 E の空の部分集合は完全に順序付けされており、E のすべての部分集合からなるの単一の元も同様です。

#### 例 3 {#ens-iii-s1-n12-exa-3 .statement tag=03TX}

\* 集合 $\mathbf{R}$ の実数は完全にオーダーされています。 \*

#### 例 4 {#ens-iii-s1-n12-exa-4 .statement tag=03TY}

A が少なくとも 2 つの異なる元を持つ集合である場合、$x\neq y$、部分集合 $\{x\}$ および $\{y\}$ は比較できないため、集合 $\mathfrak{P}(A)$ (包含によって順序付けされている) は完全に順序付けされていません。

完全に順序付けされた集合は、反対の順序付けに関しても完全に順序付けされます。それは格子であり、 *なおさら* 左右両方の方向を向いています。

#### 命題 11 {#ens-iii-s1-prop-11 .statement tag=03JS}

*完全に順序付けられた集合* E * から順序付けられた集合* F * へのすべての厳密に単調な写像 $f$ は単射法です。 $f$ が真に増加するの場合、$f$ は * E * の $f(\mathrm{E})$* の同型です。

$x \neq y$ は、$x < y$ または $x > y$ のいずれかを意味します。したがって

$$f(x) < f(y) \qquad \text{or} \qquad f(x) > f(y),$$

どちらの場合も $f(x) \neq f(y)$ となります。 $f$ が真に増加するである場合、$f(x) \leqslant f(y)$ は $x \leqslant y$ を意味することはまだわかりません。そうでない場合は、$x > y$、つまり $f(x) > f(y)$ が必要です。

#### 命題 12 {#ens-iii-s1-prop-12 .statement tag=03JT}

*E を完全に順序付けられた集合とし、* X *E の部分集合とする。 * E の元 $b$ が * X の最小の上界であることについて、* E において、* (1) *$b$ であることが必要かつ十分である* * X の上界、(2) * $c < b$ となる $c \in \mathrm{E}$ ごとに、$c < x \leqslant b$ となる $x \in \mathrm{X}$ が存在します。*

2番目の条件は、元 $c < b$はXの上界ではない、つまり、$b$はXの上界の集合Mの最小元であることを示しています。しかし、これは、M が完全に順序付けされている (no. 10、命題 10) ため、$b$ が M の最小の元であるというというと同じです。

### 13. 区間

E を順序付き集合とし、$a$、$b$ を $a \leqslant b$ となるような E の 2 つの元とします。 E の部分集合元 $x$ のからなるは、$a \leqslant x \leqslant b$ が左側の端点 a と右側の端点 b* を持つ * 閉じた区間と呼ばれ、$[a, b]$ で表されます。 $a \leqslant x < b$ (それぞれ $a < x \leqslant b$) のようなすべての $x \in \mathrm{E}$ の集合は、端点 $a$ と $b$ を持つ *右側の半開* (それぞれ *左側*) の区間と呼ばれ、 $[a, b[$ (それぞれ $]a, b]$) で表されます。 $a < x < b$ がエンドポイント $a$ と $b$ を持つ *オープン区間* と呼ばれる、すべての $x \in \mathrm{E}$ の集合は、$]a, b[$ で示されます。

閉じた区間は決して空ではないことに注意してください。 区間 $[a, a]$ は集合 $\{a\}$ です。一方、区間 $[a, a[$、$]a, a]$、$]a, a[$ はすべて空です。そして、開いている区間 $]a, b[$ は、$a < b$ のときでも空である可能性があります。

$a$ を E の元とします。すべての $x \in \mathrm{E}$ の集合を、$x \leqslant a$ (それぞれ $x < a$) を *closed* (それぞれ *open*) *区間と呼び、左側に境界がなく、右側の端点が a* で、次のように表されます。 $]{\leftarrow}, a]$ (それぞれ $]{\leftarrow}, a[$);同様に、$x \geqslant a$ (それぞれ $x > a$) であるすべての $x \in \mathrm{E}$ の集合は、左側の端点 a、右側に境界がない * を持つ *closed* (それぞれ *open*) *区間と呼ばれ、$[a, {\rightarrow}[$ (それぞれ $]a, {\rightarrow}[$) で示されます。最後に、E 自体は、$]\leftarrow, \rightarrow[$ で示される *左右に境界のない開いた区間* と見なすことができます。

#### 命題 13 {#ens-iii-s1-prop-13 .statement tag=03JU}

*格子では、2 つの区間のうち共通部分は区間です。* たとえば、閉じた 2 つの区間 $[a, b]$ と $[c, d]$ のうち共通部分を考えて、$\alpha = \sup (a, c)$、$\beta = \inf (b, d)$ とします。 $a \leqslant x \leqslant b$ と $c \leqslant x \leqslant d$ の両方があれば、$\alpha \leqslant x \leqslant \beta$ があり、その逆も可能です。 $[a, b]$ および $[c, d]$ の $\alpha \not\leqslant \beta$、共通部分が空の場合。 $\alpha \leqslant \beta$ の場合、この共通部分は $[\alpha, \beta]$ です。他のケースについては、証明を実行するかどうかは読者に任せます。

### 練習問題 {#ens-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
