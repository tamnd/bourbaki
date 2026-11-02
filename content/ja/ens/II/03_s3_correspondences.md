---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 3
section_title: Correspondences
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 75-90, 124-125
pdf_pages: 0082-0097, 0131-0132
extraction: ocr
subsections:
    - "no": 1
      title: GRAPHS AND CORRESPONDENCES
      page: 75
      pdf_page: 82
    - "no": 2
      title: INVERSE OF A CORRESPONDENCE
      page: 78
      pdf_page: 85
    - "no": 3
      title: COMPOSITION OF TWO CORRESPONDENCES
      page: 78
      pdf_page: 85
    - "no": 4
      title: FUNCTIONS
      page: 81
      pdf_page: 88
    - "no": 5
      title: RESTRICTIONS AND EXTENSIONS OF FUNCTIONS
      page: 82
      pdf_page: 89
    - "no": 6
      title: DEFINITION OF A FUNCTION BY MEANS OF A TERM
      page: 83
      pdf_page: 90
    - "no": 7
      title: COMPOSITION OF TWO FUNCTIONS. INVERSE FUNCTION
      page: 84
      pdf_page: 91
    - "no": 8
      title: RETRACTIONS AND SECTIONS
      page: 86
      pdf_page: 93
    - "no": 9
      title: FUNCTIONS OF TWO ARGUMENTS
      page: 89
      pdf_page: 96
statements: 37
exercises: 11
content_sha256: 1e052fa9ade423055cbc1af221710685d4a2655a4db5445e3f7c7f5a20ca71e6
translated_from: content/en/ens/II/03_s3_correspondences.md
translation_method: google
source_content_sha256: 09657f186f72956f32a3834e46ca25f5e52a2f152080a83c21123877583d9007
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 7ee14bfde4bb4853bc5ced07f4cc2c1215a0037ee0487373c10aab25b3f94843
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 3. 対応

### 1. グラフと対応

#### 定義 1 {#ens-ii-s3-def-1 .statement tag=03PG}

G * のすべての元が順序付き対である場合、つまり関係* の場合、G * はグラフであると言われます。

$$(\forall z)(z \in G \Rightarrow (z \text{ is an ordered pair}))$$

*本当です。*

G をグラフとすると、関係 $(x, y) \in G$ は「G の下で$y$ 対応するから $x$ まで」というというで表されます。

$\boldsymbol{R}\{x, y\}$ を関係とします。ここで、$x$ と $y$ は別個の文字です。 $\boldsymbol{G}$ を、$\boldsymbol{R}$ には現れない $x$ や $y$ とは異なる文字とします。 関係の場合

$$(\exists \boldsymbol{G})(\boldsymbol{G} \text{ is a graph and } (\forall x)(\forall y)(\boldsymbol{R} \Leftrightarrow ((x, y) \in \boldsymbol{G})))$$

は真であり、関係 $\boldsymbol{R}$ は *グラフがある*と言われています (文字 $x$ と $y$ に関して)。グラフ $\boldsymbol{G}$ は範囲の公理により一意であり、$x$ と $y$ に関する $\boldsymbol{R}$ の *グラフ* と呼ばれます。

¶ $Z$ を、$R$ には現れない$x$ や $y$ とは異なる文字とします。 関係の場合

$$(\exists Z)(\forall x)(\forall y)(R \Rightarrow ((x, y) \in Z))$$

が true の場合、$R$ にはグラフが表示されます。このグラフは、$z \in Z$ と $R \{ \mathrm{pr}_1 z,\ \mathrm{pr}_2 z \}$ のように順序付けられた対 $z$ の集合であると考えることができます ($z$ は、$R$ には現れない $x$、$y$、$Z$ とは異なる文字です)。この条件は、項 $T$ がわかっていれば満たされますが、$x$ も $y$ も含むではなく、$R \Rightarrow ((x,\ y) \in T)$ が真となります。

#### 命題 1 {#ens-ii-s3-prop-1 .statement tag=03HI}

*G * をグラフとしましょう。 *次のプロパティ*を持つ集合* A * と 1 つだけ集合* B が存在します。

(1) *関係* $(\exists y)((x,\ y) \in \mathrm{G})$ *は $x \in \mathrm{A}$ と同等です。

(2) *関係* $(\exists x)((x,\ y) \in \mathrm{G})$ *は$y \in \mathrm{B}$と同等です。

なぜなら、A (それぞれ B) を、形 $\mathrm{pr}_1 z$ (それぞれ $\mathrm{pr}_2 z$) のすべてのオブジェクトの集合とするだけで十分だからです。ここで、$z \in \mathrm{G}$ (§ 1, no. 6) です。正確には、

$$\mathrm{A} = \mathscr{E}_x((\exists y)((x, y) \in \mathrm{G}))) \qquad \text{and} \qquad \mathrm{B} = \mathscr{E}_y((\exists x)((x,\ y) \in \mathrm{G}));$$

これらの集合は、それぞれグラフ G の *最初と 2 番目の射影*、または G の *ドメイン* と *範囲* と呼ばれます。それらは、$\mathrm{pr}_1 \langle \mathrm{G} \rangle$ と $\mathrm{pr}_2 \langle \mathrm{G} \rangle$ (または、混乱の危険がない場合は、$\mathrm{pr}_1 \mathrm{G}$ と $\mathrm{pr}_2 \mathrm{G}$) で示されます。 $\mathrm{G} \subset (\mathrm{pr}_1 \mathrm{G}) \times (\mathrm{pr}_2 \mathrm{G})$; であることがすぐに確認されます。したがって、注文された対のすべての集合は、積の部分集合となり、その逆も可能です。 2 つの集合 $\mathrm{pr}_1 \mathrm{G}$、$\mathrm{pr}_2 \mathrm{G}$ の 1 つが空の場合、$\mathrm{G} = \emptyset$ (§ 2、命題 2) になります。

#### 注意 {#ens-ii-s3-n1-rem-3 .statement tag=03S1}

関係 $x = y$ にはグラフがありません。グラフの最初の射影が存在する場合、すべてのオブジェクト (cf. § 1, no. 7、注意) の集合になります。

#### 定義 2 {#ens-ii-s3-def-2 .statement tag=03HJ}

*集合* A * と集合* B の間の *対応はトリプル*

$$\Gamma = (\mathrm{G},\ \mathrm{A},\ \mathrm{B}),$$

*ここで* G *は、* $\mathrm{pr}_1 \mathrm{G} \subset \mathrm{A}$ *および* $\mathrm{pr}_2 \mathrm{G} \subset \mathrm{B}$ のようなグラフです。 G *は $\Gamma$ のグラフであると言われており、A は *ソース、* B は * $\Gamma$ の *ターゲット* です。

$(x,\ y) \in \mathrm{G}$の場合、「対応 $\Gamma$の$y$ 対応するから$x$」と言います。それぞれの $x \in \mathrm{pr}_1 \mathrm{G}$ 対応 $\Gamma$ は $x$ で *定義されていると言われ、 $\mathrm{pr}_1 \mathrm{G}$ は $\Gamma$ の *ドメイン* と呼ばれます。それぞれの $y \in \mathrm{pr}_2 \mathrm{G}$ は、* $\Gamma$ が取得した *値であると言われ、$\mathrm{pr}_2 \mathrm{G}$ は、$\Gamma$ の *範囲* と呼ばれます。

$R \{ x, y \}$ が $G$ のグラフ (文字 $x$、$y$ に関して) を持つ関係で、$A$、$B$ が $\mathrm{pr}_1 G \subset A$ と $\mathrm{pr}_2 G \subset B$ のような 2 つの集合である場合、$R$ であると言います。 $A$の元と$B$*の元の間の*関係です(文字$x$、$y$に関して)。 対応 $\Gamma = (G, A, B)$ は、$A$ と $B$ の間の対応であると言われています。*定義* 関係 $R$ ($x$ と $y$ に関して)。

G をグラフとし、X を集合とします。 関係

$$x \in X \text{ and } (x, y) \in G$$

は $(x, y) \in G$ を意味するため、グラフは $G'$ になります。 $G'$ の 2 番目の射影は、G の下にある対応するから X のオブジェクトまでのすべてのオブジェクトで構成されます。

#### 定義 3 {#ens-ii-s3-def-3 .statement tag=03PI}

*G *をグラフとし、* X *集合とします。 * G * の下で対応するから * X の元までにあるすべてのオブジェクトの集合は、* X * G * の下で像と呼ばれ、* $G\langle X \rangle$ *または* $G(X)$ で表されます。

¶ *$\Gamma = (G, A, B)$ *を対応とし、* X *を* Aの部分集合とします。 *集合* $G\langle X \rangle$ *は* $\Gamma\langle X \rangle$ *または* $\Gamma(X)$ *で表され、* Xの像と呼ばれます*下* $\Gamma$。

*注意*

#### 注意 1 {#ens-ii-s3-n1-rem-1 .statement tag=03PH}

正確には、$G\langle X \rangle$ は集合 $\mathscr{E}_y((\exists x)(x \in X \text{ and } (x,y) \in G))$ を表します。これからは、通常、定義を正式な言語に翻訳することはありません。

#### 注意 2 {#ens-ii-s3-n1-rem-2 .statement tag=03S2}

記法 $G(X)$ と $\Gamma(X)$ は、後で導入される記法と混同されることがあります (定義 9 に続く cf. no. 4、注意)。

Gをグラフとする。 関係 $(x, y) \in G$ は $y \in \mathrm{pr}_2 G$ を意味するため、集合 X ごとに $G\langle X \rangle \subset \mathrm{pr}_2 G$ が得られます。 $(x, y) \in G$ は $x \in \mathrm{pr}_1 G$ を意味するので、$G\langle \mathrm{pr}_1 G \rangle = \mathrm{pr}_2 G$ になります。 $x \notin \emptyset$は定理なので、$G\langle \emptyset \rangle = \emptyset$になります。 $X \subset \mathrm{pr}_1 G$ と $X \neq \emptyset$ の場合、$G\langle X \rangle \neq \emptyset$ になります。

#### 命題 2 {#ens-ii-s3-prop-2 .statement tag=03PJ}

*G * をグラフとし、* X、Y * を 2 集合とします。次に、関係* $X \subset Y$ *暗黙* $G\langle X \rangle \subset G\langle Y \rangle$。

これは、定義と C50 (§ 1, no. 4) の明らか帰結です。

#### 系 {#ens-ii-s3-n1-cor-1 .statement tag=03PK}

*もし* $A \supset \mathrm{pr}_1 G$なら、*私たちは* $G\langle A \rangle = \mathrm{pr}_2 G$を持っています。

#### 定義 4 {#ens-ii-s3-def-4 .statement tag=03PL}

*G *をグラフとし* $x$ *オブジェクトとする。 集合* $G\langle \{x\} \rangle$ (言葉の乱用により、$G(x)$ によって示されるときどき) *G *at* $x$ の切断と呼ばれます。

C43 (章 I, § 5, no. 1) からすぐに、関係 $y \in G\langle \{x\} \rangle$ が $(x, y) \in G$ と同等であることがわかります。 G と $G'$ が 2 つのグラフである場合、関係 $G \subset G'$ は次と同等です。

$$(\forall x)(G\langle \{x\} \rangle \subset G'\langle \{x\} \rangle).$$

$\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ が A と B の間の対応である場合、$x$ における G のすべての $x \in \mathrm{A}$ 切断は、* $x$ における* $\Gamma$ の *切断とも呼ばれ、$\Gamma\langle\{x\}\rangle$ (または$\Gamma(x)$）。

### 2. 対応の逆数

G をグラフとし、$\mathrm{A} = \mathrm{pr}_1\mathrm{G}$、$\mathrm{B} = \mathrm{pr}_2\mathrm{G}$ をその射影とします。 関係 $(y, x) \in \mathrm{G}$ は $(x, y) \in \mathrm{B} \times \mathrm{A}$ を意味します。したがって、この関係には、$(y, x) \in \mathrm{G}$ のような順序付けられたすべての対 $(x, y)$ で構成されるグラフが含まれます。

#### 定義 5 {#ens-ii-s3-def-5 .statement tag=03PM}

※Gをグラフとする。 元が $(y, x) \in \mathrm{G}$ となるように順序付けられた対 $(x, y)$ であるグラフは、G の逆関数と呼ばれ、* $\overset{-1}{\mathrm{G}}$ で表されます。

すべての集合 X に対して、$\overset{-1}{\mathrm{G}}\langle\mathrm{X}\rangle$ は * X *G の下の *逆像と呼ばれます。

¶ $\overset{-1}{\mathrm{G}}$ の逆数が G であることは明らかです。

$$\mathrm{pr}_1\overset{-1}{\mathrm{G}} = \mathrm{pr}_2\mathrm{G}, \qquad \mathrm{pr}_2\overset{-1}{\mathrm{G}} = \mathrm{pr}_1\mathrm{G}.$$

特に、X、Y が 2 集合の場合、次のようになります。

$$\overset{-1}{\overbrace{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

グラフ G は、$\overset{-1}{\mathrm{G}} = \mathrm{G}$ の場合 *対称* であると言われます。

¶ $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ を A と B の間の対応とします。 $\mathrm{pr}_1\overset{-1}{\mathrm{G}} \subset \mathrm{B}$ と $\mathrm{pr}_2\overset{-1}{\mathrm{G}} \subset \mathrm{A}$ なので、トリプル $(\overset{-1}{\mathrm{G}}, \mathrm{B}, \mathrm{A})$ は B と A の間の *対応であり、対応 $\Gamma$ の *逆* と呼ばれ、次のように表されます。 $\overset{-1}{\Gamma}$。 B のすべての部分集合 Y に対して、$\overset{-1}{\Gamma}$ の下にある Y の像 $\overset{-1}{\Gamma}\langle\mathrm{Y}\rangle$ は、$\Gamma$ の下にある Y の *逆像* とも呼ばれます。明らかに、$\overset{-1}{\Gamma}$ の逆数は $\Gamma$ です。

### 3. 合成/2 対応

G、G'を2つのグラフとする。 A が集合 $\mathrm{pr}_1\mathrm{G}$ を表し、C が集合 $\mathrm{pr}_2\mathrm{G}'$ を表すものとします。 関係 $(\exists y)((x, y) \in \mathrm{G}$ と $(y, z) \in \mathrm{G}')$ は $(x, z) \in \mathrm{A} \times \mathrm{C}$ を意味するため、$x$ と $z$ に関するグラフが存在します。

#### 定義 6 {#ens-ii-s3-def-6 .statement tag=03PN}

※G、G'を2つのグラフとする。 関係 $(\exists y)((x, y) \in \mathrm{G}$ と $(y, z) \in \mathrm{G}')$ のグラフ ($x$ と $z$ に関して) を G' と G の合成と呼び、* $\mathrm{G}' \circ \mathrm{G}$ (またはときどきを $\mathrm{G}'\mathrm{G}$ で表す) で表します。

#### 命題 3 {#ens-ii-s3-prop-3 .statement tag=03HK}

*G、G' *を 2 つのグラフとしましょう。 * G' ∘ G * の逆数は* $\overset{-1}{G} \circ \overset{-1}{G'}$ となります。

関係の場合、「$(x, y) \in G$ および $(y, z) \in G'$」は以下と同等です

$$(z, y) \in \overset{-1}{G'} \text{ and } (y, x) \in \overset{-1}{G}.$$

#### 命題 4 {#ens-ii-s3-prop-4 .statement tag=03HL}

*$G_1$、$G_2$、$G_3$ * をグラフとしましょう。それから*

$$(G_3 \circ G_2) \circ G_1 = G_3 \circ (G_2 \circ G_1).$$

関係 $(x, t) \in (G_3 \circ G_2) \circ G_1$ は関係と同等です

$$(\exists y)((x, y) \in G_1 \text{ and } \exists z((y, z) \in G_2 \text{ and } (z, t) \in G_3))$$

したがって (C33 (章 I, § 4, no. 3) による) から関係

(1) $$(\exists y)(\exists z)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

同様に、関係 $(x, t) \in G_3 \circ (G_2 \circ G_1)$ は次と同等です。

(2) $$(\exists z)(\exists y)((x, y) \in G_1 \text{ and } (y, z) \in G_2 \text{ and } (z, t) \in G_3).$$

しかし、関係 (1) と (2) は同等です。したがって結果です。

¶ グラフ$G_3 \circ (G_2 \circ G_1)$を$G_3 \circ G_2 \circ G_1$で表します。同様に、$G_1$、$G_2$、$G_3$、$G_4$ がグラフの場合、次のようにします。

$$G_4 \circ (G_3 \circ G_2 \circ G_1) = G_4 \circ G_3 \circ G_2 \circ G_1;$$

など。

#### 命題 5 {#ens-ii-s3-prop-5 .statement tag=03HM}

*G、G' *をグラフとし、* A *を集合とします。それから*

$$(G' \circ G)\langle A \rangle = G'\langle G\langle A \rangle\rangle.$$

なぜなら、C33 (章 I, § 4, no. 3) 関係 $z \in (G' \circ G)\langle A \rangle$ は次と同等だからです。

$$(\exists y)((\exists x)(x \in A \text{ and } (x, y) \in G) \text{ and } (y, z) \in G')$$

したがって、$(\exists y)(y \in G\langle A \rangle$ および $(y, z) \in G')$ と同等です。したがって結果です。

¶ G と G' が 2 つのグラフである場合、$\mathrm{pr}_1(G' \circ G) = \overset{-1}{G}\langle \mathrm{pr}_1 G'\rangle$ と $\mathrm{pr}_2(G' \circ G) = G'\langle \mathrm{pr}_2 G\rangle$ が得られます。たとえば、これらの 2 番目の関係を証明するには、関係 $z \in \mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G})$ が $(\exists x)((x, z) \in \mathrm{G}' \circ \mathrm{G})$ と同等であることに注意するだけで十分です。

$$(\exists y)((\exists x)((x, y) \in \mathrm{G}) \quad \text{and} \quad (y, z) \in \mathrm{G}');$$

しかし、これは $z \in \mathrm{G}'\langle \mathrm{pr}_2\mathrm{G}\rangle$ に相当します。

¶ G がグラフで、X 集合が $\mathrm{X} \subset \mathrm{pr}_1\mathrm{G}$ となる場合、次のようになります。

$$\mathrm{X} \subset \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle.$$

関係 $x \in \mathrm{X}$ は、仮定によって $(\exists y)((x, y) \in \mathrm{G})$ を意味します。しかし、$(x, y) \in \mathrm{G}$ は $(y, x) \in \overset{-1}{\mathrm{G}}$ と同等であり、一方、$(x, y) \in \mathrm{G}$ は $(\exists z)(z \in \mathrm{X}$ と $(z, y) \in \mathrm{G})$ を暗示します。したがって、$x \in \mathrm{X}$ は意味します

$$(\exists y)((\exists z)(z \in \mathrm{X} \quad \text{and} \quad (z, y) \in \mathrm{G}) \quad \text{and} \quad (y, x) \in \overset{-1}{\mathrm{G}}),$$

つまり、$x \in \overset{-1}{\mathrm{G}}\langle \mathrm{G}\langle \mathrm{X}\rangle\rangle$です。

¶ $\mathrm{G}_1$、$\mathrm{G}_2$、$\mathrm{G}'_1$、$\mathrm{G}'_2$ がグラフである場合、関係 $\mathrm{G}_1 \subset \mathrm{G}_2$ および $\mathrm{G}'_1 \subset \mathrm{G}'_2$ が $\mathrm{G}'_1 \circ \mathrm{G}_1 \subset \mathrm{G}'_2 \circ \mathrm{G}_2$ を意味することは明らかです。

¶ $\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ と $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ を 2 つの対応とし、$\Gamma$ のターゲットが $\Gamma'$ のソースと同じになるようにします。上記の議論から、$\mathrm{pr}_1(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_1\mathrm{G} \subset \mathrm{A}$ と $\mathrm{pr}_2(\mathrm{G}' \circ \mathrm{G}) \subset \mathrm{pr}_2\mathrm{G}' \subset \mathrm{C}$ が得られます。したがって、次のように言えます定義 :

#### 定義 7 {#ens-ii-s3-def-7 .statement tag=03PO}

*$\Gamma = (\mathrm{G}, \mathrm{A}, \mathrm{B})$ *と* $\Gamma' = (\mathrm{G}', \mathrm{B}, \mathrm{C})$ *を2 対応とし、* $\Gamma$ *のソース* $\Gamma'$ とします。 *その後、対応* $(\mathrm{G}' \circ \mathrm{G}, \mathrm{A}, \mathrm{C})$ * $\Gamma'$ * と* $\Gamma$ の合成と呼ばれ、 * $\Gamma' \circ \Gamma$ (またはときどき $\Gamma'\Gamma$) で表されます。

命題 5 からすぐに、X が A の部分集合である場合、$(\Gamma' \circ \Gamma)\langle \mathrm{X}\rangle = \Gamma'\langle \Gamma\langle \mathrm{X}\rangle\rangle$ が得られます。さらに、$\overset{-1}{\Gamma'}$のターゲットは$\overset{-1}{\Gamma}$のソースと同じであるため、$\Gamma' \circ \Gamma$の逆数は命題3により$\overset{-1}{\Gamma} \circ \overset{-1}{\Gamma'}$となります。

#### 定義 8 {#ens-ii-s3-def-8 .statement tag=03PP}

*A が集合、集合* $\Delta_\mathrm{A}$ *形* $(x, x)$ のすべてのオブジェクトの *場合* $x \in \mathrm{A}$、 * は $\mathrm{A} \times \mathrm{A}$ の対角と呼ばれます。

明らかに $\mathrm{pr}_1\Delta_\mathrm{A} = \mathrm{pr}_2\Delta_\mathrm{A} = \mathrm{A}$ があります。 対応

$$\mathrm{I}_\mathrm{A} = (\Delta_\mathrm{A}, \mathrm{A}, \mathrm{A})$$

は A の *恒等性対応* と呼ばれます。それ自体の逆です。

¶ $\Gamma$ が A と B の間の対応で、$\mathrm{I}_\mathrm{A}$、$\mathrm{I}_\mathrm{B}$ がそれぞれ A、B の同一性対応である場合、$\Gamma \circ \mathrm{I}_\mathrm{A} = \mathrm{I}_\mathrm{B} \circ \Gamma = \Gamma$ です。

### 4. 写像

#### 定義 9 {#ens-ii-s3-def-9 .statement tag=03HN}

*グラフ* F * 各 x に対して、* F (章 I, § 5, no. 3) の下に対応するから x に至るオブジェクトが最大 1 つある場合、関数グラフであると言われます。 *対応* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *そのグラフ* F *が関数グラフであり、そのソース* A *がそのドメイン* $\mathrm{pr}_1\mathrm{F}$ に等しい場合、*は写像であると言われます。 *他の語、対応* $f = (\mathrm{F}, \mathrm{A}, \mathrm{B})$ *すべての x 所属に対してソース* A *f 関係* $(x, y) \in \mathrm{F}$ *は y* (章 I, § 5, no. 3) で機能する場合、写像です。 *the unique object which corresponds to x under f is called the value of f at the element x of* A, *and is denoted by* $f(x)$ (*or* $f_x$, *or* $\mathrm{F}(x)$, *or* $\mathrm{F}_x$).

$f$ が写像、F のグラフ、および $f$ の定義域の $x$ 元である場合、関係 $y = f(x)$ は $(x, y) \in \mathrm{F}$ と等価になります (章 I, § 5, no. 3、基準 C46)。

#### 注意 {#ens-ii-s3-n4-rem-1 .statement tag=03HO}

読者は、定義 3 (cf. 練習問題 11) で導入された記法 $f(x)$ と $f(\mathrm{X})$ ($f\langle \mathrm{X} \rangle$ と同義) を同時に使用することで生じる可能性のある混乱に注意する必要があります。

A と B を 2 集合とします。 * A *into* B の *写像は写像 $f$ であり、そのソース (ドメインに等しい) は A に等しく、そのターゲットは B に等しい。このような写像は A で *定義され*、その値を B に *取り込む* とも言われます。

「$f$ を A から B の写像にしましょう」というフレーズの代わりに、「$f : \mathrm{A} \to \mathrm{B}$ を写像にしましょう」または「$f : \mathrm{A} \to \mathrm{B}$ にしましょう」というフレーズがよく使用されます。いくつかの写像が関与する議論の表現を簡略化するために、次のような *図式* を使用します。

$$\begin{array}{ccccccccc} & f & & & g & \mathrm{C} & & i & \\ \mathrm{A} & \to & \mathrm{B} & \nearrow & & & \searrow & & \mathrm{E} \\ & & & \searrow & & \mathrm{D} & \nearrow & & \\ & & & h & & & j & & \end{array}$$

ここで、$\mathrm{A} \overset{f}{\to} \mathrm{B}$ などの記号の群は、$f$ が A の写像を B に変換することを意味すると解釈されます。

A で定義された写像 $f$ は、*変換 x $f(x)$ (すべての $x \in \mathrm{A}$ に対して) になると言われます。 $f(x)$ は、f* によって x の *変換と呼ばれたり、(言葉の乱用によって) $f$ の下の $x$ の *像* と呼ばれたりします。

¶ 特定の状況下では、関数グラフは *ファミリー* と呼ばれます。この場合、ドメインは *添字集合* と呼ばれ、その範囲は (言葉の乱用により) ファミリの *集合または元* と呼ばれます。 記法 $f_x$ という記号が元 $x$ で $f$ の値を表すために使用されるのは、主にこの関連です。 添字集合が 2 つの集合のうち積であるとき、私たちはよく*二重家族*について話します。

¶ 同様に、ターゲットが E である写像は、E の *ファミリー 元* と呼ばれるときどきです。 E のすべての元が集合 F の部分集合である場合、F の *ファミリー 部分集合* について話します。

この系列では、「関数グラフ」の代わりに語 「写像」 をよく使用します。

*例/写像*

#### 例 1 {#ens-ii-s3-n4-exa-1 .statement tag=03V1}

空の集合は関数グラフです。グラフが空であるすべての写像は、空の集合と等しい領域と範囲を持ちます。このような写像のうち、ターゲットが空のもの（つまり写像$(\varnothing,\varnothing,\varnothing)$）を*空の写像*と呼びます。

#### 例 2 {#ens-ii-s3-n4-exa-2 .statement tag=03V2}

A を集合とします。 A (no. 3) の同一性対応は写像であり、A の *恒等写像* と呼ばれます。

したがって、すべての集合 A には、A の恒等写像によって定義される家族が関連付けられ、その添字集合が A であり、元の集合が A です。言葉の乱用により、集合はときどきと呼ばれ、この場合、それはこのように関連付けられた家族です。問題の集合。

$f$ の領域内のすべての $x$ と $x'$ に対して $f(x)=f(x')$ がある場合、写像 $f$ は *定数* であると言われます。

¶ $f$ を E の集合 E の写像とします。E の元 $x$ は、$f(x)=x$ の場合、$f$ の下で *固定* されます。

### 5. 写像の制限と拡大

2 つの写像 $f$ と $g$ は、E が $f$ と $g$ の領域に含まれ、すべての $x\in E$ について $f(x)=g(x)$ が含まれる場合、集合 E に *同意* (または *一致する*) と言われます。同じグラフを持つ 2 つの写像は、その領域に一致します。 $f=g$ が言うことは、$f$ と $g$ が同じドメイン A と同じターゲット B を持ち、A について同意することを意味します。

¶ $f=(F,A,B)$ と $g=(G,C,D)$ を 2 つの写像とします。 $F\subset G$ ということは、$f$ のドメイン A が $g$ のドメイン C に含まれており、$g$ が A の $f$ と一致することを意味します。$B\subset D$ もある場合、$g$ は *拡大* であると言われます。 $f$ (正確には$f$からCの拡大)、$g$は*拡大する* $f$ (Cまで)と言われています。 $g$がDの元*の*ファミリーと呼ばれるとき、$f$は$g$の*サブファミリー*と言われます。

¶ $f$ を写像とし、A を $f$ の領域の部分集合とします。 関係「$x\in A$と$y=f(x)$」が$x$と$y$に関してグラフGを持ち、このグラフが機能し、Aがその領域であることは、明らかです。 $f$と同じターゲットを持つグラフがGである写像は、$f$～$A$の*制限*と呼ばれ、ときどきは$f|A$で表されます。 写像は、その制限の拡大です。 2 つの写像 $f$、$g$ が同じターゲットを持ち、集合 $E$ に同意する場合、それらの制限 ～ $E$ は等しいです。

### 6. 項による写像の定義

C54。 *$T$、$A$ を 2 つの項とし、$x$、$y$ を個別の文字とします。 $x$ が $A$ に現れず、$y$ が $T$ にも $A$ にも現れないとします。 $R$を関係「$x \in A$と$y = T$」とします。 関係 $R$ には、$x$ と $y$ の文字に関してグラフ $F$ があります。 このグラフは機能します。最初の射影は $A$ で、2 番目の射影は $x \in A$ (§ 1, no. 6) の形 $T$ のオブジェクトの集合です。 $x \in A$ ごとに $F(x) = T$ があります。*

$x \in A$ に対する形 $T$ のオブジェクトの集合を $B$ とします。それから

$$
R \Longrightarrow ((x,y) \in A \times B);
$$

$A \times B$ 含むで示されるアセンブリには $x$ も $y$ もないので、$R$ は文字 $x$ と $y$ (no. 1) に関してグラフ $F$ を持ちます。 関係であることは明らかです

$$
(x,y) \in F \quad\text{and}\quad (x,y') \in F
$$

は $y = y'$ を意味するため、$F$ は関数グラフです。残りの主張は明らかです。

¶ If $C$ is a set which contains the set $B$ of objects of the form $T$ for $x \in A$ (where $y$ does not appear in $C$), then the function $(F,A,C)$ is also denoted by the notation $x \to T$ ($x \in A$, $T \in C$); the corresponding assembly in formal mathematics contains neither $x$ nor $y$ and does not depend on the choice of the letter $y$ satisfying the above conditions. 文脈が十分に明示的であれば、記法 $x \to T(x \in A)$、$(T)_{x \in A}$、または $x \to T$、およびときどきは単純に $T$ または $(T)$ を許可します。 *したがって、文脈が明らかに写像 $x \to x^3$ の集合の複素数をそれ自体の中に意味していることが明らかであれば、「写像 $x^3$」について話すことができます。 \*

*例*

#### 例 1 {#ens-ii-s3-n6-exa-1 .statement tag=03S3}

$f$ が $A$ の写像を $B$ にすると、写像 $f$ は写像 $x \to f(x)$ ($x \in A$, $f(x) \in B$) に等しく、単に $x \to f(x)$ または $(f_x)_{x \in A}$ とも書きます。 (後者の記法は、「写像」ではなく「元の家族」というフレーズに特に関連付けられています)。

#### 例 2 {#ens-ii-s3-n6-exa-2 .statement tag=03S4}

G を注文した対の集合とします。 写像

$$z \to \mathrm{pr}_1 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_1 z \in \mathrm{pr}_1 \mathrm{G})$$

そして

$$z \to \mathrm{pr}_2 z \quad (z \in \mathrm{G}, \ \mathrm{pr}_2 z \in \mathrm{pr}_2 \mathrm{G})$$

それぞれ、G 上の *最初と 2 番目の座標写像と呼ばれます。混同の恐れがない場合は、$\mathrm{pr}_1$ および $\mathrm{pr}_2$ で表されます。

### 7. 2 つの写像のうち合成。インバース写像

#### 命題 6 {#ens-ii-s3-prop-6 .statement tag=03HP}

*f が * A *into* B の写像であり、 * そして g が * B *into* C の写像である場合、 * $g \circ f$ * は * A *into* C の写像です。

F、G をそれぞれ$f$、$g$ のグラフとし、$\mathrm{G} \circ \mathrm{F}$ が関数グラフであることを示します。 $x$、$z$、$z'$ を、$(x, z) \in \mathrm{G} \circ \mathrm{F}$、$(x, z') \in \mathrm{G} \circ \mathrm{F}$ のようなオブジェクトとしましょう。次のようなオブジェクト $y$、$y'$ が存在します。

$$(x, y) \in \mathrm{F}, \qquad (x, y') \in \mathrm{F}, \qquad (y, z) \in \mathrm{G}, \qquad (y', z') \in \mathrm{G}.$$

F は関数グラフなので、$y = y'$、したがって $(y, z') \in \mathrm{G}$ になります。 G は関数グラフであるため、$z = z'$ となり、主張が証明されます。さらに、$g \circ f$の領域は明らかにAであり、証明は完全です。

¶ 写像 $g \circ f$ は、混乱の恐れがない場合、$x \to g(f(x))$ または $gf$ と書くこともできます。

#### 定義 10 {#ens-ii-s3-def-10 .statement tag=03HQ}

*f を* A *B の写像とします。* 写像 f は単射的である、または * A の 2 つの異なる元が f の下で異なる像を持っている場合、単射であると言われます。 写像 f は、* $f(\mathrm{A}) = \mathrm{B}$ の場合、全射法、または全射法であると言われます。 * f が単射と全射の両方である場合、それは全単射、つまり全単射と言われます。

$f$が全射であるというというの代わりに、ときどきは、$f$がB*上の*Aの写像であるか、またはAによるBの*パラメトリックな表現*であると言います(この場合、Aはパラメータ*の*集合と呼ばれます)。 A の表現と元を *パラメータ* と呼びます。 $f$ が全単射である場合、ときどきは *f が A * と * B を *1 対 1 対応* に置くと言います。 A の A への全単射を A の *置換* と呼びます。

*例*

#### 例 1 {#ens-ii-s3-n7-exa-1 .statement tag=03S5}

$\mathrm{A} \subset \mathrm{B}$ の場合、グラフが A の対角である B への A の写像は単射であり、A から B への *標準写像* または *標準単射* (または単に *単射*) と呼ばれます。

#### 例 2 {#ens-ii-s3-n7-exa-2 .statement tag=03S6}

Aを集合とします。 A の写像 $x \to (x, x)$ を $\mathrm{A} \times \mathrm{A}$ の対角線 $\Delta_\mathbf{A}$ に入れると、全単射写像となり、A の *対角線写像* と呼ばれます。

#### 例 3 {#ens-ii-s3-n7-exa-3 .statement tag=03S7}

G を注文した対の集合とします。 G の写像 $\mathrm{pr}_1$ (それぞれ $\mathrm{pr}_2$) から $\mathrm{pr}_1\mathrm{G}$ (それぞれ $\mathrm{pr}_2\mathrm{G}$) は全射法です。 $\mathrm{pr}_1$ は、G が関数グラフである場合にのみ単射的です。

#### 例 4 {#ens-ii-s3-n7-exa-4 .statement tag=03S8}

G を注文した対の集合とします。 写像

$$z \to (\mathrm{pr}_2 z,\ \mathrm{pr}_1 z)$$

G の $\overset{-1}{\mathrm{G}}$ への変換は全単射 (*標準* 全単射と呼ばれます) です。

#### 例 5 {#ens-ii-s3-n7-exa-5 .statement tag=03S9}

A を集合および $b$ をオブジェクトとします。 A の写像 $x \to (x,\ b)$ を $\mathrm{A} \times \{b\}$ にすると全単射になります。

#### 命題 7 {#ens-ii-s3-prop-7 .statement tag=03PQ}

*$f$を* Aの*から* Bへの* 写像とします。 *すると* $\overset{-1}{f}$ *は、$f$が全単射である場合に限り、写像になります。*

$\overset{-1}{f}$ が写像の場合、そのソース B はそのドメイン、つまり $f(\mathrm{A})$ と等しくなります。従って、$f$ は全射法です。 $f$ が単射であることを示すために、$x$ と $y$ を $f(x) = f(y)$ となるような A の 2 つの元とします。 F が $f$ のグラフを表す場合、次のようになります。

$$(f(x),\ x) \in \overset{-1}{\mathrm{F}} \qquad \text{and} \qquad (f(y),\ y) \in \overset{-1}{\mathrm{F}},$$

従って

$$(f(x),\ y) \in \overset{-1}{\mathrm{F}},$$

従って $x = y$ となり、これは主張を証明します。

¶ 逆に、$f$ が全単射である場合、$\overset{-1}{\mathrm{F}}$ が関数的であり、$\overset{-1}{f}$ の定義域が B に等しいことは明らかです。

$f$ が全単射の場合、$\overset{-1}{f}$ は $f$ の *逆写像* と呼ばれます。 $\overset{-1}{f}$は全単射、$\overset{-1}{f} \circ f$はAの恒等写像、$f \circ \overset{-1}{f}$はBの恒等写像です。

¶ 置換がその逆数と同じである場合、それは *involutory* であると言われます。

#### 注意 {#ens-ii-s3-n7-rem-1 .statement tag=03HR}

$f$ を A の写像から B にするとします。A の各部分集合 X に対して、(no. 3) $\mathrm{X} \subset \overset{-1}{f}\langle f\langle \mathrm{X}\rangle\rangle$ が得られます。さらに、B の各部分集合 Y に対して $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle \subset \mathrm{Y}$ があり、関係 $y \in f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle$ は次と同等です。

$$(\exists x)((\exists z)(z \in \mathrm{Y} \text{ and } z = f(x)) \text{ and } y = f(x))$$

従って、関係 $(\exists z)(z \in \mathrm{Y} \text{ and } y = z)$ を意味し、その結果、関係 $y \in \mathrm{Y}$ も意味します。

$f$ が *全射* の場合、B のすべての部分集合 Y に対して $f\langle \overset{-1}{f}\langle \mathrm{Y}\rangle\rangle = \mathrm{Y}$ があり、関係 $y \in \mathrm{Y} \subset \mathrm{B}$ は仮定関係 $(\exists x)(y = f(x))$ によって暗示され、従って $(\exists x)(y \in \mathrm{Y} \text{ and } y = f(x))$ も暗黙的に表されます。しかし、「$y \in \mathrm{Y}$ と $y = f(x)$」は $(\exists z)(z \in \mathrm{Y} \text{ and } z = f(x))$ を暗示し、その後に主張が続きます。

$f$ が *単射* の場合、A の部分集合 X ごとに $\overset{-1}{f}\langle f\langle X\rangle\rangle = X$ が得られます。 関係の場合、$x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ は $f(x) \in f\langle X\rangle$ と同等であるため、

$$(\exists z)(z \in X \text{ and } f(z) = f(x));$$

しかし、仮定は $f(z) = f(x)$ が $z = x$ を意味することを意味し、従って $x \in \overset{-1}{f}\langle f\langle X\rangle\rangle$ は $x \in X$ を意味します。

### 8. 撤回と切断

#### 命題 8 {#ens-ii-s3-prop-8 .statement tag=03HS}

*$f$ を * A の *B への写像とします。 *存在する写像 $r$* (それぞれ $s$) *B の *A への *そのような $r \circ f$* (それぞれ $f \circ s$) *が * A (それぞれ B) の恒等写像である場合、 *そのとき $f$ は単射* (*全射*) です。 *逆に、$f$ が全射であれば、$f \circ s$ が * B の恒等写像となるように、* B *に* A の写像 $s$ が存在します。 *If $f$ is injective and if* A $\neq \emptyset$, *there exists a mapping $r$ of* B *into* A *such that $r \circ f$ is the identity mapping of* A.

$r \circ f$ が A の恒等写像であるような B の写像 $r$ が A に存在する場合、等式 $f(x) = f(y)$ ($x \in A$ と $y \in A$ は $x = r(f(x)) = r(f(y)) = y$ を意味するため、$f$ は単射法) になります。 $f \circ s$ が B の恒等写像となるような B の写像 $s$ が A に存在する場合、$B = f(s(B)) \subset f(A) \subset B$ があり、$f$ は全射になります。 $f$ が全射である場合、T は項 $\tau_y(y \in A \text{ and } f(y) = x)$ を表すものとします。 $x \in B$には$f(T) = x$があります。 $s$ が写像 $x \to T$ $(x \in B, T \in A)$ を表す場合、$f \circ s$ は B の恒等写像です。最後に、$f$ が単射で A が $\neq \emptyset$ であると仮定し、$a$ を B の元とします。 A. 関係

$$\text{“}(y \in A \text{ and } x = f(y)) \text{ or } (y = a \text{ and } x \in B - f(A))\text{''}$$

は $(x, y) \in B \times A$ を意味するため、文字 $x$、$y$ に関してグラフ R があります。このグラフは $f$ の仮定の理由により機能し、ドメインとして B を持ちます。そして、$x \in B - f(A)$の場合は$R(x) = a$、$x \in f(A)$の場合は$f(R(x)) = x$になります。したがって、写像 $r = (R, B, A)$ は、$r \circ f$ が A の恒等写像となるようなものです。

#### 系 {#ens-ii-s3-n8-cor-1 .statement tag=03HT}

*A、Bを*集合とし、$f$を* A *into* Bの写像とし、*$g$を* B *into* Aの写像とします。 *$g \circ f$ が * A の恒等写像で、$f \circ g$ が * B の恒等写像である場合、*そのとき、$f$ と $g$ は全単射で、$g = \overset{-1}{f}$ です。

#### 定義 11 {#ens-ii-s3-def-11 .statement tag=03HU}

*$f$ を単射語* (それぞれ *全射語*) としましょう* A の *写像を B に *します。 *任意の写像 $r$* (それぞれ $s$) *の B *が A に * $r \circ f$* (それぞれ $f \circ s$) * が * A (それぞれ B) の恒等写像であることを *撤回* (それぞれ *切断*) *の$f$.*

撤回 (それぞれ切断) の代わりに、*left-inverse* (それぞれ *right-inverse*) というフレーズがときどき使用されます。

¶ $f$ が単射法 (または全射法) で、$r$ (または $s$) が $f$ の撤回 (それぞれ切断) である場合、$f$ は $r$ (それぞれ切断) の切断 (それぞれ撤回) です。 $s$）。したがって、撤回は全射的であり、切断は単射的です。

¶ $f$ が全射で、$s$、$s'$ が $f$ の 2 つの切断で、$s(\mathrm{B}) = s'(\mathrm{B})$ となる場合、$s = s'$ になります。なぜなら、$x \in \mathrm{B}$の場合、$s(x) = s'(y)$となるような$y \in \mathrm{B}$が存在し、$x = f(s(x)) = f(s'(y)) = y$があるので、$s(x) = s'(x)$、その結果$s = s'$となるからです。従って、切断 $s$ は集合 $s(\mathrm{B})$ によって一意に決定されます。言葉の乱用により、集合 $s(\mathrm{B})$ はときどきを $f$* の *切断と呼びます。

#### 定理 1 {#ens-ii-s3-thm-1 .statement tag=03PR}

*$f$を* A *into* Bの写像とし、*$f'$を* B *into* Cの写像とし、*そして$f'' = f' \circ f$とします。それから:*

(a) ※$f$と$f'$が単射の場合、$f''$は単射となります。 $r$、$r'$ がそれぞれ $f$、$f'$ の撤回である場合、$r \circ r'$ は $f''$ の撤回です。*

(b) *$f$と$f'$が全射である場合、$f''$は全射です。 $s$、$s'$ がそれぞれ $f$ の切断、$f'$ である場合、$s \circ s'$ は $f''$ の切断です。*

(c) ※$f''$が単射の場合、$f$は単射となります。 $r''$ が $f''$ の撤回である場合、$r'' \circ f'$ は $f$ の撤回です。*

(d) *$f''$ が全射である場合、$f'$ は全射です。 $s''$ が $f''$ の切断である場合、$f \circ s''$ は $f'$ の切断です。*

(e) *$f''$ が全射で、$f'$ 単射の場合、$f$ は全射です。 $s''$ が $f''$ の切断である場合、$s'' \circ f'$ は $f$ の切断です。*

(f) *$f''$ が単射で、$f$ が全射である場合、$f'$ は単射です。 $r''$ が $f''$ の撤回である場合、$f \circ r''$ は $f'$ の撤回です。*

すべての集合 E について、$\mathrm{I_E}$ は E の恒等写像を表します。

(a) $r \circ f = \mathrm{I_A}$ と $r' \circ f' = \mathrm{I_B}$ があるため、

$$(r \circ r') \circ (f' \circ f) = r \circ \mathrm{I_B} \circ f = r \circ f = \mathrm{I_A}.$$

If $f$ and $f'$ are injections, then $f''$ is an injection, by Proposition 8 if $\mathrm{A} \neq \emptyset$, and trivially if $\mathrm{A} = \emptyset$.

(b) $f \circ s = \mathrm{I_B}$ と $f' \circ s' = \mathrm{I_C}$ があるため、

$$(f' \circ f)(s \circ s') = f' \circ \mathrm{I_B} \circ s' = f' \circ s' = \mathrm{I_C}.$$

$f$ と $f'$ が全射である場合、$f''$ は命題 8 による全射です。

(c) $r'' \circ f'' = \mathrm{I_A}$ があるため、$(r'' \circ f') \circ f = r'' \circ f'' = \mathrm{I_A}$ となります。 $f''$ が単射の場合、$f$ は単射、$\mathrm{A} \neq \emptyset$ の場合は 8命題倍、$\mathrm{A} = \emptyset$ の場合は自明です。

(d) $f'' \circ s'' = \mathrm{I_C}$ があるため、$f' \circ (f \circ s'') = f'' \circ s'' = \mathrm{I_C}$ となります。 $f''$ が全射である場合、$f'$ は命題 8 による全射です。

(e) $f'' \circ s'' = \mathrm{I_C}$ があり、$f'$ は (d) により全単射になります。したがって、

$$f \circ (s'' \circ f') \;=\; (\overset{-1}{f}{}' \circ f') \circ f \circ (s'' \circ f') \;=\; \overset{-1}{f}{}' \circ (f'' \circ s'') \circ f'$$
$$= \overset{-1}{f}{}' \circ \mathrm{I_C} \circ f' = \overset{-1}{f}{}' \circ f' = \mathrm{I_B}.$$

$f''$ が全射で、$f'$ 単射の場合、$f$ は命題 8 による全射です。

(f) $r'' \circ f'' = \mathrm{I_A}$ があり、$f$ は (c) により全単射になります。したがって、

$$(f \circ r'') \circ f' = (f \circ r'') \circ f' \circ (f \circ \overset{-1}{f}) = f \circ (r'' \circ f'') \circ \overset{-1}{f} = f \circ \mathrm{I_A} \circ \overset{-1}{f}$$
$$= f \circ \overset{-1}{f} = \mathrm{I_B}.$$

$f''$ が単射で、$f$ が全射である場合、$f'$ は単射となり、$\mathrm{A} \neq \emptyset$ の場合は 8命題 8 倍され、$\mathrm{A} = \emptyset$ の場合は自明です (その場合、$\mathrm{B} = f\langle \mathrm{A}\rangle = \emptyset$ になります)。

#### 命題 9 {#ens-ii-s3-prop-9 .statement tag=03PS}

(a) *E, F, G *を集合とし、* $g$ * 写像 of* E *onto* F *and* $f$ *写像 of* E *into* G とする。 *すると、写像* $h$ *of* F *into* G *そのような* $f = h \circ g$ *関係* $g(x) = g(y)$ *(ここで* $x \in \mathrm{E}$, $y \in \mathrm{E}$*) は関係* $f(x) = f(y)$ を意味します。 *写像* $h$ *その後* $f$ によって一意に決定されます。 *もし* $s$ *が* $g$の切断であれば、*$h = f \circ s$があります。

$$\begin{array}{ccc}
\mathrm{E} & \overset{f}{\searrow} & \\
{\scriptstyle g}\big\downarrow\big\uparrow{\scriptstyle s} & & \\
\mathrm{F} & \underset{h}{\longrightarrow} & \mathrm{G}
\end{array}
\qquad\qquad
\begin{array}{ccc}
 & \overset{f}{\nearrow} & \mathrm{E} \\
 & & {\scriptstyle r}\big\downarrow\big\uparrow{\scriptstyle g} \\
\mathrm{G} & \underset{h}{\longrightarrow} & \mathrm{F}
\end{array}$$
$$\text{(a)} \qquad\qquad\qquad \text{(b)}$$

(b) *E, F, G *を集合とし、* $g$ * 単射 of* F *into* E とし、*そして $f$ *be 写像 of* G *into* E とします。 *すると、 写像* $h$ *of* G が存在します。 *に* F *そのような* $f = g \circ h$ *もし、そしてその場合に限り* $f(\mathrm{G}) \subset f(\mathrm{F})$。 *写像* $h$ *は* $f$ によって一意に決定されます。 *もし* $r$ *が $g$ の撤回*であれば、 *$h = r \circ f$ があります*。

(a) $f = h \circ g$、関係 $g(x) = g(y)$ ($x \in \mathrm{E}$、$y \in \mathrm{E}$) は明らかに $f(x) = f(y)$ を意味します。そして、$g$ の切断 $s$ ごとに、

$$h = h \circ (g \circ s) = f \circ s,$$

これは、$h$ が $f$ によって一意に決定されることを示しています。逆に、関係 $g(x) = g(y)$ が $f(x) = f(y)$ を意味するとします。 $s$ を $g$ の切断とし、$h = f \circ s$ とします。 $x \in E$ごとに$g(s(g(x))) = g(x)$、したがって$f(s(g(x))) = f(x)$、つまり$h(g(x)) = f(x)$、したがって$f = h \circ g$になります。

(b) $f = g \circ h$ の場合、明らかに $f(G) \subset f(F)$ であり、$g$ のすべての撤回 $r$ に対して、$h = (r \circ g) \circ h = r \circ f$ が得られます。これは、$h$ が $f$ によって一意に決定されることを示しています。逆に、$f(G) \subset f(F)$; と仮定します。 $r$を$g$の撤回とし、$h = r \circ f$を置きます。すべての $x \in G$ に対して、$f(x) = g(y)$ となるような $y \in F$ が存在します。

$$g(h(x)) = g(r(f(x))) = g(r(g(y))) = g(y) = f(x)$$

したがって $f = g \circ h$ です。

### 9. 2 つの引数の写像

2 つの引数の *写像* は写像で、その定義域は順序付けられた対の集合 (または同等に、積の部分集合) です。 $f$ をそのような写像とします。 $(x, y)$ が $f$ の領域の元である場合、元 $(x, y)$ における $f$ の値 $f((x, y))$ は一般に $f(x, y)$ で表されます。

¶ $f$ を 2 つの引数の写像とし、D をそのドメイン、C をターゲットとします。それぞれの $y$ について、$A_y$ をすべての $x$ の集合とし、$(x, y) \in D$ (つまり、$y$ (no. 1) での $\overset{-1}{D}$ の切断) とします。 写像

$$x \to f(x, y) \quad (x \in A_y, f(x, y) \in C)$$

は、第 2 引数 * の値 $y$ に関して、$f$ によって定義された *部分写像と呼ばれ、$f(\bullet, y)$ または $f(\ , y)$ (またはときどき $f_y$) で表されます。 $(x, y) \in D$ 全員に対して $f(\bullet, y)(x) = f(x, y)$ があります。同様に、各 $x$ について、$B_x$ をすべての $y$ の集合とし、$(x, y) \in D$ とします。 写像

$$y \to f(x, y) \quad (y \in B_x, f(x, y) \in C)$$

最初の引数*の値$x$に関して$f$で定義された*部分写像と呼ばれ、$f(x, \bullet)$または$f(x, \ )$(またはときどき$f_x$)で表されます。 $(x, y) \in D$ 全員に対して $f(x, \bullet)(y) = f(x, y)$ があります。

¶ すべての $y$ (それぞれ $x$) について、部分写像 $f(\bullet, y)$ (それぞれ $f(x, \bullet)$) が定数写像である場合、 $f$ はその最初 (または 2 番目) の引数に *依存しない* と言います。したがって、これは、D に対して $(x, y)$ および $(x', y)$ 属するの場合は常に $f(x, y) = f(x', y)$ (それぞれ、D に対して $(x, y)$ および $(x, y')$ 属するの場合は常に $f(x, y) = f(x, y')$) であることを意味します。 D の各 $y$ 所属から 2 番目の射影について、$g(y)$ は $x \in A_y$ の $f(x, y)$ の共通の値を表します。 写像 $y \to g(y)$ は、$\mathrm{pr}_2 D$ の写像が C になります。

$$g(y) = f(x, y) \qquad \text{for all } (x, y) \in D.$$

¶ 逆に、$g$ を集合 B の写像を集合 C とし、A を任意の集合とします。 この場合、$A \times B$ の C への写像 $(x, y) \to g(y)$ は最初の引数に依存しません。

¶ $u$ を、A の写像を C に、B の $v$ 写像を D にするとします。 写像 $A \times B$ の $z \to (u(\mathrm{pr}_1 z), v(\mathrm{pr}_2 z))$ を $C \times D$ にすると、 (*標準*) *拡大と呼ばれます。 $u$ と $v$ から積集合*、または単純に $u$ と $v$* の *積 (混乱の危険がない場合)。その範囲は$u\langle A\rangle \times v\langle B\rangle$です。 $u \times v$で表されます。 $u$ と $v$ が単射 (それぞれ全単射) の場合、 $u \times v$ は単射 (それぞれ全単射) です。 $u$ と $v$ が全単射である場合、$u \times v$ は全単射であり、その逆数写像は $\overset{-1}{u} \times \overset{-1}{v}$ です。 $u'$ が C の集合 E への写像であり、$v'$ が D の写像から集合 F である場合、次のようになります。

$$(u' \times v') \circ (u \times v) = (u' \circ u) \times (v' \circ v).$$

U、V がそれぞれ $u$、$v$ のグラフである場合、$u \times v$ のグラフ W は、$(x, z) \in U$ と $(y, t) \in V$ のように、$(A \times B) \times (C \times D)$ の対 $((x,y), (z, t))$ の集合です。 写像 $((x, y), (z, t)) \to ((x, z), (y, t))$ は、W を対応と積 $U \times V$ ($(A \times C) \times (B \times D)$ の部分集合) (cf. §5, no. 5) と 1 対 1 にします。

### 練習問題 {#ens-ii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
