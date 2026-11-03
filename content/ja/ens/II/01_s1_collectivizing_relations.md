---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 1
section_title: Collectivizing relations
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 65-72, 123
pdf_pages: 0072-0079, 0130-0130
extraction: ocr
subsections:
    - "no": 1
      title: THE THEORY OF SETS
      page: 65
      pdf_page: 72
    - "no": 2
      title: INCLUSION
      page: 66
      pdf_page: 73
    - "no": 3
      title: THE AXIOM OF EXTENT
      page: 67
      pdf_page: 74
    - "no": 4
      title: COLLECTIVIZING RELATIONS
      page: 67
      pdf_page: 74
    - "no": 5
      title: THE AXIOM OF THE SET OF TWO ELEMENTS
      page: 69
      pdf_page: 76
    - "no": 6
      title: THE SCHEME OF SELECTION AND UNION
      page: 69
      pdf_page: 76
    - "no": 7
      title: COMPLEMENT OF A SET. THE EMPTY SET
      page: 71
      pdf_page: 78
statements: 10
exercises: 6
content_sha256: ff2b8097f195f3e306c4535ff5ace7e8cb5f19b3c43e3f65ba0060e0fde931c0
translated_from: content/en/ens/II/01_s1_collectivizing_relations.md
translation_method: google
source_content_sha256: 15e4c05cbeaa37f947e4dd88b319dfea58ef5aed00b479f31e5cbe9ae7b53342
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 4b1bebe92f0850cbf9760e043f72f56769af64ae40cba68a223beb7f54f4ce08
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 集団化関係

### 1. 集合中理論

集合* の *理論は理論であり、含む関係記号 $=$、$\in$ と実体記号 $\supset$ (これらの記号はすべて重み 2 です)。 加法では、章 I で与えられたスキーム S1 から S7 に、含む no. 6 で導入されるスキーム S8 と、明示的な公理 A1 (no. 3.) A2 (no. 5)、A3 (§ 2, no. 1)、A4 が適用されます。 (§ 5, no. 1)、および A5 (章 III, § 6, no. 1)、これらの明示的な公理含む文字は含まれません。他の語、集合の理論は、*定数なし* の理論です。

集合の理論は平等主義理論なので、章Iの結果が当てはまります。

¶ 今後、〜でない限り反対のことが明確に述べられていますが、私たちは常に集合の理論よりも強い (章 I, § 2, no. 4) 理論で議論することになります。 理論が言及されていない場合は、集合の理論が暗示されていると想定されます。多くの場合、この仮定が不必要であることは明らかであり、読者は、集合の理論よりも弱い理論のどれが記載されている結果が有効であるかを判断するのに困難はありません。

$T$ と $U$ が項の場合、アセンブリ $\in TU$ は関係 (メンバーシップ* の *関係と呼ばれます) で、実際には次のいずれかの方法で記述します: $T \in U$、$(T) \in (U)$、「$T$ 属する to $U$」、「$T$は$U$の元です」。 関係「$(T \in U)$ではない」は$T \notin U$と書かれています。

「素朴な」点視点からは、多くの数学的実体はオブジェクトのコレクションまたは「集合」と考えることができます。私たちはこの概念を形式化するつもりはありません。また、以下の形式的な解釈では、語「集合」は厳密には「項」と同義であると見なされます。特に、「X を集合にしましょう」などのフレーズは、すべての文字が項であるため、原則として非常に不要です。このような語句は、テキストの直感的な解釈を支援するためにのみ紹介されています。

### 2. インクルージョン

#### 定義 1 {#ens-ii-s1-def-1 .statement tag=03H5}

*関係* $(\forall z)((z \in x) \Rightarrow (z \in y))$ は、*$x$ と $y$ のみが表示され、次のいずれかの方法で記述されます:* $x \subset y$、$y \supset x$、 *「$x$ は $y$」、「$y$ 含む」に含まれます$x$」、「$x$は$y$の部分集合です」。 関係* 「$(x \subset y)$ ではありません」 *$x \not\subset y$ *または* $y \not\supset x$ と書かれています*。

章 I, § 1, no. 1 で述べた規則に従って、この定義には次のメタ数学的規則が伴います。 $T$ と $U$ をアセンブリとします。アセンブリ $x \subset y$ の $x$ を $T$ に、$y$ を $U$ に置き換えると、$T \subset U$ で示されるアセンブリが得られます。 $x$、$y$ とは異なり、互いに異なり、$T$ にも $U$ にも現れない文字を $\mathbf{x}$、$\mathbf{y}$ で表すと、アセンブリ $T \subset U$ は $(T|\mathbf{x})(U|\mathbf{y})(\mathbf{x}|x)(\mathbf{y}|y)(x \subset y)$ と同一となり、したがって CS8、CS9 となります。 (章 I, § 4, no. 1)、CS5 (章 I, § 1, no. 2) は$(\forall z)((z \in T) \Rightarrow (z \in U))$ となります。ただし、$z$ は$T$ にも$U$ にも現れない文字です。

今後、私たちが数学的な定義を述べるときは常に、それが伴うメタ数学的な約束事については言及しないことにします。

CS12。 *$T$、$U$、$V$ をアセンブリ、$x$ を文字とします。この場合、アセンブリ $(V|x)(T \subset U)$ は $(V|x)T \subset (V|x)U$ と同一になります。*

これは、CS9 (章 I, § 4, no. 1) および CS5 (章 I, § 1, no. 2) の直後に続きます。

CF13。 *$T$と$U$が項の場合、$T \subset U$は関係となります。

これは CF8 (章 I, § 1, no. 4) の直後に続きます。

¶ 形 $T \subset U$ ($T$ と $U$ は項) のすべての関係を *包含関係* と呼びます。

今後、定義に従うべき置換の基準と形成基準を明示的に記述することはなくなります。ただし、これらの基準は証明で暗黙的に使用されることが多いことに注意してください。

理論 $\mathscr{T}$ の関係 $x \subset y$ を証明するには、C27 (章 I, § 4, no. 1) により、$z \in x$ を $\mathscr{T}$ の公理に隣接させることで得られる理論の $z \in y$ を証明すれば十分です。ここで、$z$ は、$x$、$y$、および理論の定数とは異なる文字です。実際には、「$z$を$x$の元とする」と言い、$z \in y$を証明しようとします。

#### 命題 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x \subset x$。

明らか。

#### 命題 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x \subset y$と$y \subset z) \Rightarrow (x \subset z)$。

仮説 $x \subset y$、$y \subset z$、および $u \in x$ を隣接させます。それから関係

$$(u \in x) \Rightarrow (u \in y), \qquad (u \in y) \Rightarrow (u \in z),$$

は true であるため、 関係 $u \in z$ は true です。

### 3. 範囲の公理

*範囲の公理* は次の公理です。

A1. $\qquad (\forall x)(\forall y)((x \subset y \text{ and } y \subset x) \Rightarrow (x = y))$。

直観的には、この公理は、同じ元を持つ 2 つの集合が等しいという事実を表します。

したがって、$x = y$ を証明するには、仮定 $z \in x$ を隣接させて得られる理論の $z \in y$ と、仮定 $z \in y$ を隣接させて得られる理論の $z \in x$ を証明すれば十分です。ただし、$z$は、$x$、$y$、および定数とは異なる文字です。

C48。 *$\mathbf{R}$を関係、$x$を文字、$y$を$\mathbf{R}$には現れない$x$とは異なる文字とします。次に、関係 $(\forall x)((x \in y) \Leftrightarrow \mathbf{R})$ は $y$ で単一値になります。*

$z$ を、$\mathbf{R}$ には現れない $x$ とは異なる文字とする。仮説を隣接させる

$$(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\forall x)((x \in z) \Leftrightarrow \mathbf{R}).$$

続いて、定理が続きます。

$$(\forall x)(((x \in y) \Leftrightarrow \mathbf{R}) \text{ and } ((x \in z) \Leftrightarrow \mathbf{R})),$$
$$(\forall x)((x \in y) \Leftrightarrow (x \in z)),$$
$$y \subset z, \qquad z \subset y.$$

A1 までに、$y = z$ になります。これでC48が証明されました。

### 4. 集団化関係

$\mathbf{R}$を関係、$x$を文字としましょう。 $y$ と $y'$ が $x$ *$\mathbf{R}$* には現れない文字を表す場合、関係

$$(\exists y)(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\exists y')(\forall x)((x \in y') \Leftrightarrow \mathbf{R})$$

CS8 (章 I, §4, no. 1) と同一です。このように定義された関係 (含む $x$ ではない) は $\operatorname{Coll}_xR$ で表されます。

¶ $\operatorname{Coll}_xR$ が理論 $\mathscr{T}$ の定理である場合、$R$ は $\mathscr{T}$ の $x$* に * 集合していると言われます。その場合、$x$ や $\mathscr{T}$ の定数とは異なり、$R$ には現れない補助定数 $a$ を、導入公理 $(\forall x)((x \in a) \Longleftrightarrow R)$ または同等の ($x$ が $\mathscr{T}$ の定数ではない場合) $(x \in a) \Longleftrightarrow R$ とともに導入することができます。

直観的には、$R$が$x$で集団化していると言うのは、性質$R$を所有するオブジェクト$x$が正確に$a$の元となるような集合$a$が存在すると言うことです。

*例*

#### 例 1 {#ens-ii-s1-n4-exa-1 .statement tag=03RZ}

関係 $x \in y$ は$x$ において明らかに集団化しています。

#### 例 2 {#ens-ii-s1-n4-exa-2 .statement tag=03S0}

関係 $x \neq x$ *$x$* では集団化していません。他の語では、($\operatorname{Coll}_x(x \neq x)$ではなく)は定理です。矛盾によって議論し、$x \neq x$ が集団化していると仮定してみましょう。導入公理を使用して、$a$ を補助定数とし、$x$ および理論の定数とは区別します。

$$
(\forall x)((x \neq x) \Longleftrightarrow (x \in a)).
$$

それでは関係

$$
(a \neq a) \Longleftrightarrow (a \in a)
$$

C30 (章 I, §4, no. 3) までは true です。場合の選別 (章 I, §3, no. 3) の方法は、最初に関係 $a \neq a$ が真であることを示し、次に関係 $a \in a$ が真であることを示しますが、これは不合理です。

**C49.** *$R$を関係、$x$を文字とします。 $R$ が $x$ で集団化している場合、関係 $(\forall x)((x \in y) \Longleftrightarrow R)$ ($y$ は $R$ には現れない $x$ とは異なる文字です) は、$y$ で機能します。

これは C48 の直後に続きます。

非常に多くの場合、以下では形 $\operatorname{Coll}_xR$ の定理が自由に使えるようになります。 項を表す

$$
\tau_y(\forall x)((x \in y) \Longleftrightarrow R),
$$

これは文字$y$の選択に依存しない($x$とは異なり、$R$には現れない)ので、機能記号$\mathscr{E}_x(R)$を導入します。 対応する項は含む $x$ ではありません。この項は、「$R$ となるすべての $x$ の集合」で示されます。 定義 (章 I, §4, no. 1) 関係によって

$$
(\forall x)((x \in \mathscr{E}_x(R)) \Longleftrightarrow R)
$$

$\mathrm{Coll}_x R$と*同一*です。従って、関係 $R$ は次と *同等* になります

$$x \in \mathscr{E}_x(R).$$

C50。 ※$R$、$S$を2つの関係、$x$を文字とします。 $R$ と $S$ が $x$ で集合化している場合、関係 $(\forall x)(R \Rightarrow S)$ は * に相当します

$$\mathscr{E}_x(R) \subset \mathscr{E}_x(S),$$

*および関係 $(\forall x)(R \Leftrightarrow S)$ は $\mathscr{E}_x(R) = \mathscr{E}_x(S)$ と同等です。*

これは、前の注意と定義 1 および公理 A1 の直後に続きます。

### 5. 2 元の集合の公理

A2. $\qquad\qquad (\forall x)(\forall y)\ \mathrm{Coll}_z(z = x \text{ or } z = y).$

この公理は、$x$ と $y$ がオブジェクトである場合、集合があり、その元は $x$ と $y$ だけであると述べています。

#### 定義 2 {#ens-ii-s1-def-2 .statement tag=03H6}

*集合 $\mathscr{E}_z (z = x \text{ or } z = y)$ (元は $x$ と $y$ のみ) は $\{x, y\}$ で表されます。

従って、関係 $z \in \{x, y\}$ は「$z = x$ または $z = y$」と同等です。 C50 からは $\{y, x\} = \{x, y\}$ となります。

$R\{z\}$ を関係とし、$x, y$ を $z$ とは異なる文字とします。 C32、C33 (章 I, §4, no. 3)、および C43 (章 I, §5, no. 1) から、関係 $(\exists z)((z \in \{x, y\})$ および $R\{z\})$ は「$R\{x\}$ または $R\{y\}$」と同等であることが簡単にわかります。従って、関係 $(\forall z)((z \in \{x, y\}) \Rightarrow R\{z\})$ は「$R\{x\}$ および $R\{y\}$」と同等です。

集合 $\{x, x\}$ は、単に $\{x\}$ で表され、*集合と呼ばれます。その元は $x$* のみです。 関係 $z \in \{x\}$ は $z = x$ に相当し、関係 $x \in \mathrm{X}$ は $\{x\} \subset \mathrm{X}$ に相当します。

### 6. 選択のスキームと和集合

*選択のスキームと和集合* は次のとおりです。

S8. *$R$を関係、$x$と$y$を別の文字、$X$と$Y$を$R$には現れない$x$と$y$とは別の文字とする。それでは関係*

(1) $\quad (\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R))$ *は公理です*。

まず、このルールが実際にスキームであることを示しましょう。 $S$ が関係 (1) を表し、$S$ の文字 $z$ を項 $T$ に置き換えます。 CS8 (章 I, §4, no. 1) では、$x$、$y$、$X$、$Y$ は $z$ とは異なり、$T$ には現れないと考えられます。この場合、$(T|z)S$ は以下と同一です。

$$(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ and } R')),$$

ここで、$R'$ は $(T|z)R$ です。

直観的に、関係 $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ は、すべてのオブジェクト $y$ に対して集合 $X$ ($y$ に依存する可能性があります) が存在し、指定されたオブジェクト $y$ とともに関係 $R$ にあるオブジェクト $x$ が$X$ の元 (ただし、必ずしも $X$ の全体ではありません)。選択スキームと和集合は、これが事実で、$Y$ が任意の集合である場合、集合が存在し、その元は正確に関係 $R$ にあるオブジェクト $x$ であり、少なくとも 1 つのオブジェクト $y$ が存在すると主張します。 集合 $Y$。

C51。 ※$P$を関係、$A$を集合、$x$を$A$に現れない文字とする。その後、関係「$P$と$x \in A$」が$x$に集団化されます*。

$R$ が関係「$P$ と $x = y$」を表すとします。ここで、$y$ は、$P$ にも $A$ にも現れない $x$ とは異なる文字です。 関係

$$(\forall x)(R \Rightarrow (x \in \{y\}))$$

C27 (章 I, §4, no. 1) によって true になります。 $X$ を、$P$ には現れない $x$ および $y$ とは異なる文字とします。前の関係は $(\{y\}|X)((\forall x)(R \Rightarrow (x \in X)))$ と同一です ($x$ は $y$ とは異なるため)、したがって、S5 と C27 (章 I, §4、番号 1 と 2) により、関係 $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ は真になります。 S8 と C30 (章 I, §4, no. 3) から次の場合、関係

$$(A|Y)\ \mathrm{Coll}x(\exists y)(y \in Y \text{ and } R)$$

($Y$ は $R$ には現れない文字です) は true であり、この関係は $\mathrm{Coll}_x(\exists y)(y \in A \text{ and } R)$ と同一です ($x$ も $y$ も $A$ には現れないため)。最後に、関係 "$y \in A$ および $R$" は、C43 (章 I, §5, no. 1) による "$x = y$ および $x \in A$ および $P$" と等価です。 $x$ は $P$ にも $A$ にも現れないため、関係

$$(\exists y)(x = y \text{ and } x \in A \text{ and } P)$$

は、C33 (章 I, §4, no. 3) による「$((\exists y)(x = y))$ and $x \in A$ and $P$」と同等であり、$(\exists y)(x = y)$ が true であるため、「$P$ and $x \in A$」と同等です。

¶ 集合 $\mathscr{E}_x(P$ と $x \in A)$ は、$P$* のようにすべての $x \in A$ のうち *集合と呼ばれます (\* したがって、$P_*$ のようにすべての実数のうちの集合について話すことができます)。

C52。 ※$R$を関係、$A$集合、$x$を$A$に現れない文字とする。 関係 $R \Rightarrow (x \in A)$ が定理である場合、$R$ は $x$ で集団化されます。*

$R$ の場合、「$R$ および $x \in A$」と同等になります。

#### 注意 {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

$R$ を $x$ で集団化する関係とし、$S$ を関係として、$(\forall x)(S \Rightarrow R)$ が定理となるようにします。そして$S$は$x$に集団化します。 $R$ は $x \in \mathscr{E}_x(R)$ と同等なので、

$$S \Rightarrow (x \in \mathscr{E}_x(R))$$

は定理、C52からは主張が続きます。この場合、C50 までに $\mathscr{E}_X(S) \subset \mathscr{E}_X(R)$ があることにも注目してください。

C53。 *$T$ を項、$A$ 集合、$x$、$y$ を別の文字とします。 $x$ は $A$ に現れず、$y$ は $A$ にも $T$ にも現れないとします。次に、関係 $(\exists x)(y = T$ と $x \in A)$ が $y$ で集団化しています。*

$R$ を関係 $y = T$ とします。 関係 $(\forall y)(R \Rightarrow (y \in \{T\}))$ は true であるため、$(\forall x)(\exists X)(\forall y)(R \Rightarrow (y \in X))$ も同様です。ここで、$X$ は、$R$ には現れない $y$ とは異なる文字です。 S8 により、関係 $(\exists x)(x \in A$ と R) が $y$ で集合化し、C53 が証明されます。

¶ 関係 $(\exists x)(y = T$ と $x \in A)$ は、次のように読まれることがよくあります: 「$x$ 所属から $A$ に対して、$y$ は形 $T$ に入れることができます」。 集合

$$\mathscr{E}_y((\exists x)(y = T \text{ and } x \in A))$$

一般に、形 $T$ のオブジェクトの $x \in A$* を *集合と呼びます。このように含むで示されるアセンブリは、$x$ でも $y$ でもなく、C53 の文字 $y$ 満たす条件の選択に依存しません。

### 7. 集合の補数。空の集合

関係 $(x \notin \mathrm{A}$ と $x \in \mathrm{X})$ は C51 によって $x$ に集団化されています。

#### 定義 3 {#ens-ii-s1-def-3 .statement tag=03H8}

*$\mathrm{A}$ *を集合* $\mathrm{X}$ の部分集合とします。 * $\mathrm{A}$ に属さない* $\mathrm{X}$ の要素の集合、 *つまり集合* $\mathscr{E}x$ $(x \notin \mathrm{A}$ *および* $x \in \mathrm{X})$、 * $\mathrm{A}$ * $\mathrm{X}$ の補数と呼ばれ、 * $\complement_{\mathrm{X}}\mathrm{A}$ * または* で表されます。 $\mathrm{X} - \mathrm{A}$ (または混乱の危険がない場合は $\complement\mathrm{A}$ までに)。

A を集合 X の部分集合とします。 関係 "$x \in \mathrm{X}$ と $x \notin \mathrm{A}$" および $x \in \complement_{\mathrm{X}}\mathrm{A}$ は同等になります。従って、関係「$x \in \mathrm{X}$および$x \notin \complement_{\mathrm{X}}\mathrm{A}$」は「$x \in \mathrm{X}$および$(x \notin \mathrm{X}$または$x \in \mathrm{A})$」、つまり$x \in A$と同等です。他の語では、$A = \complement_X(\complement_X A)$は真の関係です。同様に、B が X の部分集合である場合、関係 $A \subset B$ と $\complement_X B \subset \complement_X A$ は同等であることがわかります。

#### 定理 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

*関係* $(\forall x)(x \notin X)$ *X で機能します。

関係 $(\forall x)(x \notin X)$ は $(\forall Y)(X \subset Y)$ を意味します。従って、範囲の公理により、関係 $(\forall x)(x \notin X)$ は X において単一値となります。一方、関係 $(\forall x)(x \notin \complement_Y Y)$ は真であり、$(\exists X)(\forall x)(x \notin X)$ が真であることが証明されます。

¶ 項 $\tau_x((\forall x)(x \notin X))$ 対応するからこの関数関係は関数記号 $\emptyset$ で表され、*空集合* [^1] と呼ばれます。 関係 $(\forall x)(x \notin X)$ は、$X = \emptyset$ に相当し、次のように読み取られます: 「*集合* X *は空です*」。 定理 $x \notin \emptyset$、$\emptyset \subset X$、$\complement_X X = \emptyset$、$\complement_X \emptyset = X$ があります。 関係 $X \subset \emptyset$ は $X = \emptyset$ と同等です。 $R\{x\}$ が関係の場合、関係 $(\forall x)((x \in \emptyset) \Rightarrow R\{x\})$ は真です。

#### 注意 {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

すべてのオブジェクトが元である集合は存在しません。他の語では、「$(\exists X)(\forall x)(x \in X)$ではない」は定理です。というのは、そのような集合があったとしたら、C52までにすべての関係が集団化するであろうからである。しかし、関係 $x \notin x$ が集団化していないことを私たちは見てきました (no. 4)。

### 練習問題 {#ens-ii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。

[^1]: The term denoted by $\emptyset$ is therefore $\tau \neg \neg \in \tau \neg \neg \in \square\square\square$.
