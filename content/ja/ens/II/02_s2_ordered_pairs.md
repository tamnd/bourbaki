---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 2
section_title: Ordered pairs
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 72-75, 123-124
pdf_pages: 0079-0082, 0130-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE ORDERED PAIR
      page: 72
      pdf_page: 79
    - "no": 2
      title: PRODUCT OF TWO SETS
      page: 74
      pdf_page: 81
statements: 4
exercises: 2
content_sha256: d2427291a3ce4945da2dc7b2e66341a3ba26c4d5657730bae9d07223b9ecba4c
translated_from: content/en/ens/II/02_s2_ordered_pairs.md
translation_method: google
source_content_sha256: 30cc0208eaab54246e96f854154d361c7bc5ca97861fad03285d7ff5c5137aa4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 143cfacec09c3b8b0615b38e3fe0bf4f3112caedcb29e99e0c449d11fcbd91ee
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 注文数対

### 1. 順序付けられた公理対

§1, no. 1で述べたように、記号$\supset$は、集合の理論における重み2の実体記号です。 T、U が項の場合、$\supset$TU は項となり、実際には (T, U) で表されます。この記法では、順序付けされた対* の *公理は次のとおりです。

A3. $(\forall x)(\forall x')(\forall y)(\forall y')(((x, y) = (x', y')) \Rightarrow (x = x' \quad \text{and} \quad y = y'))$。

関係 "$x = x'$ と $y = y'$" は C44 (章 I, § 5, no. 2) によって $(x, y) = (x', y')$ を意味するため、関係 $(x, y) = (x', y')$ は "$x = x'$ と $y = y'$" と *同等* です。

¶ 関係 $(\exists x)(\exists y)(z=(x,y))$ は「$z$ は *注文された対*」と書かれています。 $z$が注文した対、関係の場合

$$
(\exists y)(z=(x,y)),\qquad(\exists x)(z=(x,y))
$$

それぞれ $x$ と $y$ に関して機能します。 A3の明らか帰結です。 項

$$
\tau_x((\exists y)(z=(x,y)))\qquad\text{and}\qquad\tau_y((\exists x)(z=(x,y)))
$$

はそれぞれ$\operatorname{pr}_1z$と$\operatorname{pr}_2z$で表され、$z$の*最初の座標* (または *最初の射影*) と *2 番目の座標* (または *2 番目の射影*) と呼ばれます。 $z$ が注文された対である場合、関係 $(\exists y)(z=(x,y))$ は $x=\operatorname{pr}_1z$ に相当し、関係 $(\exists x)(z=(x,y))$ は $y=\operatorname{pr}_2z$ (章 I, §5, no. 3) に相当します。

¶ 関係 $z=(x,y)$ は、「$z$ は順序付けられた対、および $x=\operatorname{pr}_1z$ および $y=\operatorname{pr}_2z$」と同等です。後者の場合、関係は次と同等です。

$$
(\exists x')(\exists y')(\exists x'')(\exists y'')(z=(x',y')\text{ and }z=(x,y'')\text{ and }z=(x'',y));
$$

A3 によれば、「$z=(x',y')$ と $z=(x,y'')$ と $z=(x'',y)$」は、「$z=(x,y)$ と $x=x'$ と $x=x''$ と $y=y'$ と $y=y''$」に相当します。したがって、C33 (章 I, §4, no. 3) により、「$z$ は順序付けられた対、$x=\operatorname{pr}_1z$ と $y=\operatorname{pr}_2z$」は次と同等です。

$$
z=(x,y)\text{ and }(\exists x')(\exists y')(\exists x'')(\exists y'')(x=x'\text{ and }x=x''\text{ and }y=y'\text{ and }y=y''),
$$

これは私たちの主張を証明します。明らかに私たちは持っています

$$
\operatorname{pr}_1(x,y)=x,\qquad \operatorname{pr}_2(x,y)=y,
$$

関係 $z=(\operatorname{pr}_1(z),\operatorname{pr}_2(z))$ は、「$z$ は注文された対」と同等です。

¶ $R\{x,y\}$ を関係とします。ここで、文字 $x$ と $y$ は別個のものであり、$R$ に現れます。 $z$ を、$R$ には現れない $x$ や $y$ とは異なる文字とします。 $S\{z\}$ を関係とします

$$
(\exists x)(\exists y)(z=(x,y)\text{ and }R\{x,y\});
$$

これは、含むが$R$より1文字少ない関係で、「$z$は順序付けされた対と$R\{\operatorname{pr}_1z,\operatorname{pr}_2z\}$」と*同等*です。これは、$z=(x,y)$が「$z$は順序付けられた対で、 $x=\operatorname{pr}_1z$ および $y=\operatorname{pr}_2z$」、基準 C33 (章 I, §4, no. 3) および C47 (章 I, §5, no. 3) から。 $R\{x, y\}$ は $S\{(x, y)\}$ と同等であることがすぐにわかります。

$$(\exists z)(z = (x, y) \text{ and } S\{z\})$$

C47による。

これは、オブジェクト $x$ と $y$ の間の関係を、これらのオブジェクトによって形成される順序付けられた対の性質として解釈できることを意味します。

### 2. 積/2 集合

#### 定理 1 {#ens-ii-s2-thm-1 .statement tag=03PC}

*関係*

$$(\forall X)(\forall Y)(\exists Z)(\forall z)((z \in Z) \Leftrightarrow (\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y)$$

*は本当です。他の語では、すべて* X *およびすべて* Y *関係* 「$z$ * は順序付けられた対および* $\mathrm{pr}_1 z \in X$ * および* $\mathrm{pr}_2 z \in Y$」 * $z$ で集合化されています。

$A_y$ が、$x \in X$ に対する形 $(x, y)$ のすべてのオブジェクトの集合を表すものとします (cf. §1, no. 6、基準 C53)。 R を関係 $z \in A_y$ とします。これは、$(\exists x)(z = (x, y)$ および $x \in X)$ と同等です。 関係であることは明らかです

$$(\forall y)(\exists A)(\forall z)(R \Rightarrow (z \in A))$$

S5 (章 I, §4, no. 2) のおかげで、これは真実です。次に、S8 から、関係 $(\exists y)(y \in Y$ と R$)$ が $z$ で集団化していることがわかります。しかし、この関係は$(\exists x)(\exists y)(y \in Y$、$x \in X$、$z = (x, y))$と同等です。したがって結果です。

#### 定義 1 {#ens-ii-s2-def-1 .statement tag=03PD}

*2 つの集合* X * と * Y、*集合* を与えます

$$\mathscr{E}_z((\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y))$$

*は X *および* Y の積と呼ばれ、 * X $\times$ Y で表されます。

したがって、関係 $z \in X \times Y$ は、「$z$ は、対と $\mathrm{pr}_1 z \in X$ および $\mathrm{pr}_2 z \in Y$ の順序である」と等価です。 集合 X と Y は、X $\times$ Y の *最初* と *2 番目の因子* と呼ばれます。

#### 命題 1 {#ens-ii-s2-prop-1 .statement tag=03PE}

*A$'$、B$'$ *が空ではない集合、関係* A$' \times$ B$' \subset$ A $\times$ B *は*「A$' \subset$ A *および* B$' \subset$ B」と同等です。

そもそも、関係 $z \in A' \times B'$ は、「$z$ は対と $\mathrm{pr}_1 z \in A'$ と $\mathrm{pr}_2 z \in B'$ の順序である」と等価です。したがって、A$'$ と B$'$ に制限がなければ、関係 「A$' \subset$ A と B$' \subset$ B」は意味します。

$$A' \times B' \subset A \times B.$$

逆に、$B' \neq \emptyset$ ($A'$ に制限がない) の場合、関係 $A' \times B' \subset A \times B$ は $A' \subset A$ を意味することを最初に示します。 $x$ を $A'$ の元とします。 $B' \neq \emptyset$ 以降、$B'$ の元であるオブジェクト $y$ が存在します。 $(x, y) \in A' \times B'$ があるため、$(x, y) \in A \times B$、従って $x \in A$ になります。従って$A' \subset A$。同様に、$A' \neq \emptyset$ の場合、関係 $A' \times B' \subset A \times B$ は $B' \subset B$ を意味します。従って、結果は次のとおりです。

#### 命題 2 {#ens-ii-s2-prop-2 .statement tag=03PF}

*A *と* B *を 2 集合とします。 関係* $A \times B = \emptyset$ *は「$A = \emptyset$ *または* $B = \emptyset$」と同等*。

関係 $z \in A \times B$ は $\mathrm{pr}_1 z \in A$ と $\mathrm{pr}_2 z \in B$ を意味します。従って、$A \neq \emptyset$ と $B \neq \emptyset$ です。逆に、関係「$x \in A$と$y \in B$」は$(x, y) \in A \times B$、つまり$A \times B \neq \emptyset$を意味します。他の語、関係、$A \times B \neq \emptyset$は「$A \neq \emptyset$、$B \neq \emptyset$」に相当します。したがって結果です。

A、B、C が集合の場合、次のように書きます。

$$(A \times B) \times C = A \times B \times C;$$

$A \times B \times C$の元$((x, y), z)$は$(x, y, z)$と書かれ、*トリプル*と呼ばれます。もう一度、A、B、C、D が集合の場合、次のように書きます。

$$(A \times B \times C) \times D = A \times B \times C \times D;$$

など。

### 練習問題 {#ens-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
