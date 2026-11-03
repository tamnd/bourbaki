---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 5
section_title: Real-valued functions
lang: ja
source: top-i-iv
book_pages: 347-359, 389-393
pdf_pages: 0353-0365, 0395-0399
extraction: ocr
subsections:
    - "no": 1
      title: REAL-VALUED FUNCTIONS
      page: 347
      pdf_page: 353
    - "no": 2
      title: REAL-VALUED FUNCTIONS DEFINED ON A FILTERED SET
      page: 348
      pdf_page: 354
    - "no": 3
      title: LIMITS ON THE RIGHT AND ON THE LEFT OF A FUNCTION OF A REAL VARIABLE
      page: 349
      pdf_page: 355
    - "no": 4
      title: BOUNDS OF A REAL-VALUED FUNCTION
      page: 350
      pdf_page: 356
    - "no": 5
      title: ENVELOPES OF A FAMILY OF REAL-VALUED FUNCTIONS
      page: 352
      pdf_page: 358
    - "no": 6
      title: UPPER LIMIT AND LOWER LIMIT OF A REAL-VALUED FUNCTION WITH RESPECT TO A FILTER
      page: 353
      pdf_page: 359
    - "no": 7
      title: ALGEBRAIC OPERATIONS ON REAL-VALUED FUNCTIONS
      page: 356
      pdf_page: 362
statements: 31
exercises: 18
content_sha256: 174207789294c848d850bd2dc164a86c8def0645f186351104f4079b4e809d28
translated_from: content/en/top/IV/05_s5_real_valued_functions.md
translation_method: google
source_content_sha256: 621e60dc8288e6ddcbaf7c1e586598f735828021aa542b362efd2af2f9c86a93
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 9d17c1f0733944c8f4beadb25f1814b1f59efcd95a5560295e832e36cf912d94
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 5. 実数値写像

### 1. 実数値写像

#### 定義 1 {#top-iv-s5-def-1 .statement tag=0BR2}

集合 $X$ から実直線への写像は、$X$ で定義された実数値写像 (または実数値写像) と呼ばれます。

§ 4, no. 2 で述べたのと同様の言葉の乱用により、$X$ から $\overline{\mathbf{R}}$ への写像も、この文と次の切断の $X$ で定義される実数値写像と呼ばれます。 $X$ の $\mathbf{R}$ への写像を有限の実数値写像と呼びます。

$f$ と $g$ が $X$ で定義された 2 つの実数値写像である場合、関係 $f \leq g$ は定義だけ「すべての $x \in X$ に対して $f(x) \leq g(x)$」と等価です。この関係は、$X$ のすべての実数値写像の集合 $\overline{\mathbf{R}}^X$ での順序です。この関係によって注文された集合 $\overline{\mathbf{R}},^X$ は格子です。 $f$ と $g$ が 2 つの実数値写像、写像 $h$ である場合、すべての $x \in X$ は、両方である $X$ の実数値写像の最小のに対して、$h(x) = \sup (f(x), g(x))$ によって定義されます。 $\geq f$ と $\geq g$;一般的な記法に従って、この写像（$f$と$\overline{\mathbf{R}}^X$の$g$の最小の上界）を$\sup (f, g)$で表します。同様に、各$x \in X$の値が$\inf (f(x), g(x))$である写像は$\inf (f, g)$で表されます。

$\sup (f, g)$ は写像の合成であることに注意してください。
$$
(u, v) \to \sup (u, v)
$$
$\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ を $\overline{\mathbf{R}}$ に、写像 $x \to (f(x), g(x))$ を $X$ から $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ に。 $\inf (f, g)$も同様です。

集合 $X$ で定義された実数値関数 $f$ は、$f(X)$ が $A'' = [-\infty, +\infty]$ の部分集合で上に制限されている場合 (または $f(X)$ が $A' = ]-\infty, +\infty]$ の部分集合で下に制限されている場合)、$X$ で *上に制限* (または *下に制限*) であると言われます。 $f$ は、上下の両方で有界である場合、つまり $f(X)$ が $\mathbf{R}$ の有界サブセットである場合、$X$ で *有界* であると言われます。

したがって、すべての有界な写像は *有限* です。 $\mathbf{R}_+^* = ]0, +\infty[$ の写像 $1/x$ が示すように、逆は false です。

### 2. フィルタリングされた集合上で定義された実数値写像

#### 命題 1 {#top-iv-s5-prop-1 .statement tag=0BR3}

*$f$ と $g$ を、フィルター $\mathfrak{F}$ でフィルターされた集合 $X$ で定義された 2 つの実数値写像とします。 $\lim_{\mathfrak{F}} f$ と $\lim_{\mathfrak{F}} g$ が存在し、各部分集合 $A \in \mathfrak{F}$ に対して $f(x) \leq g(x)$ となる $x \in A$ が存在する場合、$\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$ が存在します。*

この結果を証明するには、次の同等の主張を証明します。

#### 命題 2 {#top-iv-s5-prop-2 .statement tag=0BR4}

*$f$ と $g$ を、フィルター $\mathfrak{F}$ でフィルターされた集合 $X$ で定義された 2 つの実数値写像とします。 $\lim_{\mathfrak{F}} f$ と $\lim_{\mathfrak{F}} g$ が存在し、$\lim_{\mathfrak{F}} f > \lim_{\mathfrak{F}} g$ の場合、集合 $A \in \mathfrak{F}$ があり、すべての $x \in A$ に対して $f(x) > g(x)$ になります。*

$a = \lim_{\mathfrak{F}} f$、$b = \lim_{\mathfrak{F}} g$、$c$ を $b < c < a$ となるようにします。 $\overline{\mathbf{R}}$ (それぞれ $]-\infty, c[$) の区間 $]c, +\infty]$ は、$a$ (それぞれ $b$) の近傍です。したがって、すべての $x \in M$ [それぞれに対して $f(x) > c$ となるような集合 $M \in \mathfrak{F}$ (それぞれ集合 $N \in \mathfrak{F}$) が存在します。 $g(x) < c$ 全員に $x \in N$]。 集合 $A = M \cap N$ 属するから $\mathfrak{F}$ まで、すべての $x \in A$ に対して $f(x) > c > g(x)$ があります。

命題 1 の特別なケースとして、次の定理があります。

#### 定理 1 (不等式の拡大の原理) {#top-iv-s5-thm-1 .statement tag=0BR5}

*$f$ と $g$ を、フィルター $\mathfrak{F}$ でフィルターされた集合 $X$ で定義された 2 つの実数値写像とします。 $\lim_{\mathfrak{F}} f$ と $\lim_{\mathfrak{F}} g$ が存在する場合、および $f \leq g$ の場合は、$\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$。*

#### 注意 {#top-iv-s5-n2-rem-1 .statement tag=0BR6}

特に、すべての $x \in X$ (またはフィルター $\overline{\mathbf{R}}$ の集合のすべての点のみ) に対して $f(x) < g(x)$ がある場合、定理 1 によって $\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$ と推論できます。 *しかし、私たちはできないが強い不等式* $\lim_{\mathfrak{F}} f < \lim_{\mathfrak{F}} g$ と推測します。 たとえば、$X$ をフレシェ フィルターでフィルター処理した自然数の集合 $\mathbf{N}$ とし、$f(n) = 0$ と $g(n) = 1/n$ の場合、$\lim_{n \to \infty} f(n) = \lim_{n \to \infty} f(n) = 0$ を除くすべての $n$ に対して $f(n) < g(n)$ となります。 したがって、*厳密* 不等式で極限に渡すと、*厳密性が失われます*。

#### 定理 2 (モノトーン極限の定理) {#top-iv-s5-thm-2 .statement tag=0BR7}

$X$ を順序付き集合とし、$A$ を $X$ の有向部分集合とします (*)。 $A$ で定義されたすべての単調実数値写像 $f$ は、$A$ に関して極限 (章 I, , no. 3) になります。 $f$ が増加する (それぞれ減少する) の場合、この極限は集合 $f(A) \subset \overline{\mathbf{R}}$ の最小の上界 (それぞれ最大の下界) に等しくなります。

たとえば、$f$ が増加するであると仮定し、$a = \sup f(A)$ とします。 $a = -\infty$ の場合、定理は自明です。 $a > -\infty$ の場合、$b < a$ ごとに $b < f(x) \leq a$ となる $x \in A$ が存在します。したがって、$S_x$ が $x$ に対して $A$ の切断である場合 (つまり、すべての $y \geq x$ の集合、cf. 章 I, § 6, no. 3)、$f(S_x)$ は$a$の近傍 $]b, +\infty]$、そして定理が続きます。 $f$ が減少するである場合、証明は類似しています。

#### 系 {#top-iv-s5-n2-cor-1 .statement tag=0BR8}

順序付けられた集合 $X$ の有向部分集合 $A$ 上で定義される増加する (それぞれ減少する) 実数値写像は、上で制限されている場合に限り、 $A$ に関して有限の極限を持ちます。 (それぞれ以下の境界) $A$。

$A = X = \mathbf{N}$ (関係 $\leq$ によって順序付けされる) の場合に定理を適用する 2 を加えると、次の命題が得られます。

#### 命題 3 {#top-iv-s5-prop-3 .statement tag=0BR9}

実数のすべての単調数列には $\overline{\mathbf{R}}$ に極限があります。
特に、有限数のすべての増加する (それぞれ減少する) 数列は、上に限定されている (または下に限定されている) 場合は有限実数に収束し、そうでない場合は $+\infty$ (それぞれ $-\infty$) に収束します。たとえば、正の整数の数列は $+\infty$ に収束します。

この事実は、数列 (章 I, § 7, no. 3) の極限を表す記法 $\lim_{n \to \infty} u_n$ の起源です。

同様に、整数 $(p_n)$ のすべての真に増加する数列は $+\infty$ に収束します。なぜなら、帰納法によって、すべての$n$が$p_n \geq p_0 + n$であることがわかります。

### 3. 実数変数の写像の右側と左側にある極限

$A$ を $\overline{\mathbf{R}}$ の空ではない部分集合とし、$a \neq -\infty$ を集合 $B = A \cap [-\infty, a[$ の閉包内にある $\overline{\mathbf{R}}$ の点とします。 集合 $B$ は関係 $\leq$ に関して方向付けられており、その切断フィルター $\mathfrak{F}$ は、$\overline{\mathbf{R}}$ の $a$ の近傍フィルターの $B$ 上のトレースと同じです。

(*) この主張は、$X$ の順序が $x \leq y$ で書かれていることを暗黙的に前提としています。この関係が$x(\sigma) y$と書かれ、$(\sigma)$が特定の記号、または関係に特徴的な予期される記号の群である場合、主張の語の「指示された」は「$(\sigma)$に関して指示された」に置き換えられなければなりません。

#### 定義 2 {#top-iv-s5-def-2 .statement tag=0BRA}

* f を $\overline{\mathbf{R}}$ の空ではない部分集合 A 上で定義された写像とし、トポロジカル空間 X の値とします。フィルタ $\mathfrak{F}$ に関する f の極限は、存在する場合、A を基準にして点 a の左側にある f の極限と呼ばれ、* で表されます。
$$
\lim_{x \to a,\ x < a,\ x \in A} f(x),
$$
*または X がハウスドルフの場合は $f(a-)$。*

同様に、$a$ が集合 $A \cap ]a, + \infty]$ の閉包内にある場合、定義する点 $a$ で $f$ の右側* (存在する場合) に *極限を追加し、次のように表します。
$$
\lim_{x \to a,\ x > a,\ x \in A} f(x),
$$
*または X がハウスドルフの場合は $f(a+)$。*

次の命題は、定理 2 の明らか帰結です。

#### 命題 4 {#top-iv-s5-prop-4 .statement tag=0BRB}

*A を $\overline{\mathbf{R}}$ の部分集合とし、共通部分 $A \cap [-\infty, a[$ の閉包で $a \neq -\infty$ を点とします。 f が A 上で定義された単調実数値写像である場合、f は A を基準にして a の左側に極限 $f(a-)$ を持ちます。

### 4. 実数値写像の境界

#### 定義 3 {#top-iv-s5-def-3 .statement tag=0BRC}

*f を集合 X で定義された実数値写像とし、A を X の空でない部分集合とします。次に、$\overline{\mathbf{R}}$ の集合 $f(A)$ の最小上界 (それぞれ最大の下界) は、A の f の最小上界 (それぞれ最大の下界) と呼ばれ、* で表されます。
$$
\sup_{x \in A} f(x) \quad \text{[resp. } \inf_{x \in A} f(x) \text{]}.
$$

特に、A が空ではない $\overline{\mathbf{R}}$ の部分集合である場合、
$$(1)$$
$$
\sup A = \sup_{x \in A} x.
$$
多くの場合、A の最小の上界を表すには、右辺の記法を使用する方が便利です。

数 $a = \sup_{x \in A} f(x)$ は、次の 2 つのプロパティによって特徴付けられます。
(i) $x \in A, f(x) \leq a$ 全員に対して。
(ii) $b < a$ ごとに、$b < f(x) \leq a$ となるような $x \in A$ が存在します。

数 $\sup_{x \in A} f(x)$ と $\inf_{x \in A} f(x)$ 属するから $\overline{\mathbf{R}}$ の $f(A)$ の *クロージング* まで。 $\inf_{x \in A} f(x) \leq \sup_{x \in A} f(x)$ があります。そして、これら 2 つの数は、$f$ が A 上で *定数* である場合に限り、*等しい* になります。

集合 X で定義された実数値写像は、$\sup_{x \in A} f(x) < + \infty$ [それぞれ 1 つの場合に限り、X の空ではない部分集合 A で *上に境界* (それぞれ *下に境界*) になります。 $\inf_{x \in A} f(x) > -\infty$]。 $f$ は、A 内で $|f|$ が上に境界がある場合に限り、A 内で *境界あり* になります。したがって、$\sup_{x \in A} |f(x)| < + \infty$ の場合にのみです。

我々は持っています

$$
\inf_{x \in A} f(x) = -\sup_{x \in A} (-f(x)).
$$

これは、関係簡約する最大の下界のすべてのプロパティから最小の上界のプロパティまでです。したがって、一般的には後者についてのみ説明します。

#### 命題 5 {#top-iv-s5-prop-5 .statement tag=0BRD}

*$f$ を、集合 $X$ で定義された実数値写像とします。 $X$ のすべての有限部分集合の集合 $\mathfrak{F}(X)$ では、関係 $\subset$ に関して方向づけられており、実数値関数 $H \to \sup_{x \in H} f(x)$ は増加し、実数値関数 $H \to \inf_{x \in H} f(x)$ は減少しており、次のようになります*

$$
\begin{cases}
\sup_{x \in A} f(x) = \lim_{H \in \mathfrak{F}(X)} (\sup_{x \in H} f(x)), \\
\inf_{x \in A} f(x) = \lim_{H \in \mathfrak{F}(X)} (\inf_{x \in H} f(x)).
\end{cases}
$$

$\varphi(H) = \sup_{x \in H} f(x)$ にしましょう。明らかに、$\varphi$ は増加するであるため、極限 $a$ (no. 2, 定理 2) になります。そしてすべての $H$ に対して $\varphi(H) \leq \sup_{x \in A} f(x)$ なので、$a \leq \sup_{x \in A} f(x)$ (no. 2, 定理 1) になります。 $a < \sup_{x \in A} f(x)$ がある場合、$a < f(x_0)$ のような $x_0 \in X$ が存在します。しかし、これは $\varphi(H) \geq f(x_0)$ から $x_0 \in H$ まで常に矛盾しています。

特に、(1) により、$A$ が $\overline{\mathbf{R}}$ の空でない部分集合である場合、次のようになります。

$$
\sup A = \lim_{H \in \mathfrak{F}(A)} (\sup_{x \in H} x).
$$

#### 命題 6 {#top-iv-s5-prop-6 .statement tag=0BRE}

*$f$ と $g$ を、$X$ で定義された 2 つの実数値写像とします。空ではない部分集合 $A$ の $X$ の点 $x$ ごとに $f(x) \leq g(x)$ がある場合、*

$$
\begin{cases}
\sup_{x \in A} f(x) \leq \sup_{x \in A} g(x), \\
\inf_{x \in A} f(x) \leq \inf_{x \in A} g(x).
\end{cases}
$$

#### 命題 7 {#top-iv-s5-prop-7 .statement tag=0BRF}

*$f$を、$X$で定義された実数値写像とします。 $A$ と $B$ が $A \subset B$ のように $X$ の 2 つの空でない部分集合である場合、*

$$
\sup_{x \in A} f(x) \leq \sup_{x \in B} f(x).
$$

#### 命題 8 {#top-iv-s5-prop-8 .statement tag=0BRG}

*$f$ を $X$ で定義された実数値写像とし、$(A_i)_{i \in I}$ を $X$ の空でない部分集合の空でない家族とする。それから*

$$
\sup_{x \in \bigcup_{i \in I} A_i} f(x) = \sup_{i \in I} (\sup_{x \in A_i} f(x)).
$$

$f$ を、積集合 $X_1 \times X_2$ で定義された実数値写像とします。 $A_2$ が $X_2$ の空ではない部分集合である場合、$X_2$ で定義された実数値写像 $x_2 \to f(x_1, x_2)$ の$A_2$ の最小上界を $\sup_{x_1 \in A_2} f(x_1, x_2)$ で表します。 命題 8 から特に次のように推測します。

#### 命題 9 {#top-iv-s5-prop-9 .statement tag=0BRH}

*$f$ を、積集合 $X_1 \times X_2$ で定義された実数値写像とします。 $A_1, A_2$ がそれぞれ $X_1, X_2$ の空ではない部分集合である場合、*

$$
\sup_{(x_1, x_2) \in A_1 \times A_2} f(x_1, x_2) = \sup_{x_1 \in A_1} (\sup_{x_2 \in A_2} f(x_1, x_2)) = \sup_{x_2 \in A_2} (\sup_{x_1 \in A_1} f(x_1, x_2)).
$$

### 5. 本物の価値のある写像の家族の封筒

#### 定義 4 {#top-iv-s5-def-4 .statement tag=0BRI}

*$(f_i)_{i \in I}$ を、集合 $X$ で定義された実数値写像の族とします。 $X$ の実数値写像の各点 $x \in X$ の値は $\sup_{i \in I} (f_i(x))$ [それぞれ$\inf_{i \in I} (f_i(x))$] は、ファミリー $(f_i)$ の上部 (または下部) エンベロープと呼ばれ、$\sup_{i \in I} f_i$ または $\sup_i f_i$ (それぞれ $\inf_{i \in I} f_i$ または $\inf_i f_i$) で示されます。

したがって、族 $(f_i)$ の上部包絡線は、$X$ で定義された実数値写像の格子 $\overline{\mathbf{R}}$ 内でこの族の最小の上界となり、これにより記法 $\sup_{i \in I} f_i$ が正当化されます。

さらに、$\overline{\mathbf{R}}^X$ にその因子のトポロジーの積であるトポロジー (すべて $\overline{\mathbf{R}}$ と同一) を与えると、次の命題が得られます。

#### 命題 10 {#top-iv-s5-prop-10 .statement tag=0BRJ}

*積空間 $\overline{\mathbf{R}}^X$ では、実数値写像 $(f_i)_{i \in I}$ の族の上部エンベロープ $\sup_{i \in I} f_i$ は、有限部分集合の $I$ の有向集合 $\mathfrak{F}(I)$ に対して、極限です。 写像 $H \to \sup_{i \in H} f_i$ [それぞれ写像有限部分集合 $H$ の $I$ を有限部分族 $(f_i)_{i \in H}$ の上部包絡線にします]。

これは、no. 4 の命題 5 と、章 I, § 7, no. 6、系 1 から命題 10 の直後に続きます。

したがって、次のように書くこともできます

$$
\sup_{i \in I} f_i = \lim_{H \in \mathfrak{F}(I)} (\sup_{i \in H} f_i).
$$

#### 定義 5 {#top-iv-s5-def-5 .statement tag=0BRK}

集合 $X$ で定義された実数値写像の * ファミリー $(f_i)_{i \in I}$ は、$f_i(x) \leq a$ [それぞれ 13] のような有限数 $a$ が存在する場合、$X$ で上に一様に境界がある (それぞれ下に一様に境界がある) と言われます。 $f_i(x) \geq a$] すべての $x \in X$ とすべての $i \in I$ に適用されます。家族 $(f_i)$ は、$X$ で上下が一様有界である場合、$X$ で一様有界であると言われます。

したがって、$(f_i)$ は、この族の上部エンベロープが $X$ の上で境界がある場合にのみ、$X$ で上に一様に境界されます。 $(f_i)$ は、ファミリー $(|f_i|)$ の上部エンベロープが $X$ で上に制限されている場合にのみ、$X$ で一様に制限されます。すべての $x \in X$ とすべての $i \in I$ に対して $|f_i(x)| \leq a$ となるような有限の実数 $a \geq 0$ が存在する場合に限ります。

### 6. フィルタの実数値写像の上位極限と下位極限

$f$ を、フィルター $\mathfrak{G}$ でフィルターされた集合 $X$ で定義された実数値写像とします。 $\mathfrak{G}$ は、関係 $\supseteq$ (章 I, § 6) に対して有向集合です。それぞれの $M \in \mathfrak{G}$ について、実数 $\sup_{x \in M} f(x)$ を検討します。$\mathfrak{G}$ の写像 $M \to \sup_{x \in M} f(x)$ を $\overline{\mathbf{R}}$ に変換します。これは、$\mathfrak{G}$ の減少する写像を、命題 7 で計算します。 no. 4。したがって、no. 2の定理 2までに、有向集合 $\mathfrak{G}$に対して極限が得られます。

#### 定義 6 {#top-iv-s5-def-6 .statement tag=0BRL}

*実数値関数の限界* $M \to \sup_{x \in M} f(x)$ *有向集合に関して* $\mathfrak{G}$ *は、* $f$ *フィルタに関して* $\mathfrak{G}$、* によって表され* $\lim \sup_{\mathfrak{G}} f$、*または* $\lim \sup_{x, \mathfrak{G}} f(x)$ で表されます。

フィルタ$\mathfrak{G}$に対する$f$の*下位極限*も同様に定義され、$\lim \inf_{\mathfrak{G}} f$または$\lim \inf_{x, \mathfrak{G}} f(x)$で表されます。したがって、私たちは

$$
\begin{cases}
\lim \sup_{\mathfrak{G}} f = \lim_{M \in \mathfrak{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathfrak{G}} f = \lim_{M \in \mathfrak{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(10)

多くの場合、フィルター $\mathfrak{G}$ は記法から抑制され、混乱の危険がない場合は単純に $\lim \sup f$ または $\lim \sup_{x} f(x)$ または $\lim \sup f(x)$ と書きます。

式 (10) と定理 1 から、次のようになります。

$$
\inf_{x \in X} f(x) \leq \lim \inf_{\mathfrak{G}} f \leq \lim \sup_{\mathfrak{G}} f \leq \sup_{x \in X} f(x).
$$

(11)

no. 2 の定理 2 までに、次のように書くこともできます

$$
\begin{cases}
\lim \sup_{\mathfrak{G}} f = \inf_{M \in \mathfrak{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathfrak{G}} f = \sup_{M \in \mathfrak{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(12)

また、$\mathfrak{G}$ の任意の *基底* $\mathfrak{B}$ によって、式 (10) と (12) の右辺にフィルター $\mathfrak{G}$ を置き換える適用することもできます。

(2)と(10)より、

$$
\lim \inf_{\mathfrak{G}} f = -\lim \sup_{\mathfrak{G}} (-f)
$$

したがって、上位の極限のみを考慮する必要があります。

#### 定理 3 {#top-iv-s5-thm-3 .statement tag=0BRM}

*フィルター $\mathfrak{G}$ に関する実数値写像 $f$ の上位極限は、$\mathfrak{G}$ に関する $f$ の値クラスタ最大のに等しい。

$b$を$\mathfrak{G}$に対する$f$のクラスター点とする。それぞれの $M \in \mathfrak{G}$、$b$ は $f(M)$ の閉包内にあるため、$b \leq \sup_{x \in M} f(x)$ となり、(12) により、
$b \leq \lim \sup_{\mathfrak{G}} f = a.$

一方、$V$ を $\overline{\mathbf{R}}$ の $a$ の任意のオープン近傍とします。次に、$\mathfrak{G}$ には集合 $M_0$ が存在し、$M_0$ に含まれる$M \in \mathfrak{G}$ ごとに $\sup_{x \in M} f(x) \in V$ が存在します。 $V$ が開いているので、$f(M)$ が $V$ と一致することになり、したがって、$a$ は $\mathfrak{G}$ に関して$f$ の *クラスター 点* となり、証明が完了します。

#### 系 1 {#top-iv-s5-thm-3-cor-1 .statement tag=0BRN}

*In order that $\lim \sup_{\mathfrak{G}} f = \lim \inf_{\mathfrak{G}} f$, it is necessary and sufficient that $f$ has a limit with respect to the filter $\mathfrak{G}$, and then*
$$
\lim_{\mathfrak{G}} f = \lim \sup_{\mathfrak{G}} f = \lim \inf_{\mathfrak{G}} f.
$$
For since $\overline{\mathbf{R}}$ is compact, the filter base $f(\mathfrak{G})$ has a limit point if and only if it has only one cluster point (Chapter I, § 9, no. 1, Corollary to Theorem 1).

#### 系 2 {#top-iv-s5-thm-3-cor-2 .statement tag=0BRO}

*$\mathfrak{H}$ が $\mathfrak{G}$ ではなくより細かいのフィルターである場合、*
$$
\lim \inf_{\mathfrak{G}} f \leq \lim \inf_{\mathfrak{H}} f \leq \lim \sup_{\mathfrak{H}} f \leq \lim \sup_{\mathfrak{G}} f.
$$
すべてのクラスターについて、$\mathfrak{H}$ に対する $f$ のクラスター 点は、$\mathfrak{G}$ (章 I, § 7, no. 3) に対する$f$ のクラスター 点でもあります。
特に、$\lim_{\mathfrak{G}} f$ が存在する場合、
$$
\lim \inf_{\mathfrak{G}} f \leq \lim_{\mathfrak{G}} f \leq \lim \sup_{\mathfrak{G}} f.
$$

#### 系 3 {#top-iv-s5-thm-3-cor-3 .statement tag=0BRP}

*$A$をフィルター$\mathfrak{G}$の集合、$\mathfrak{G}_A$を$\mathfrak{G}$によって$A$に誘導されたフィルター、$f_A$を$f$から$A$の制限とします。それから*
$$
\lim \sup_{\mathfrak{G}_A} f_A = \lim \sup_{\mathfrak{G}} f.
$$
フィルター 基底 $f(\mathfrak{G})$ のクラスター 点はフィルター 基底 $f_A(\mathfrak{G}_A)$ のクラスター 点であり、その逆も同様です。

このため、$X$ 所属 ～ $\mathfrak{G}$ の部分集合 $A$ のみに $f$ が定義されている場合、言葉の乱用により、$\limsup_{\mathfrak{G}_A} f_A$ の代わりに $\limsup_{\mathfrak{G}} f$ と書くことになります。

#### 命題 11 {#top-iv-s5-prop-11 .statement tag=0BRQ}

$f$ と $g$ を、フィルタリングされた集合 $X$ で定義された 2 つの実数値写像とします。その場合、関係 $f \leq g$ は意味します

$$
\begin{cases}
\limsup f \leq \limsup g, \\
\liminf f \leq \liminf g.
\end{cases}
$$

これは、関係 (12) の明らか帰結です。

$X$ がトポロジー 空間で、$\mathfrak{G}$ が点 $a$ の $X$ の近傍フィルターである場合、$\limsup_{x \to a} f(x)$ [それぞれ$\limsup_{\mathfrak{G}} f$ [それぞれ $\liminf_{x \to a} f(x)$] の代わりに$\liminf_{\mathfrak{G}} f$];明らかに私たちは持っています

$$
\liminf_{x \to a} f(x) \leq f(a) \leq \limsup_{x \to a} f(x).
$$

より一般的には、$X$ がトポロジカル空間 $Y$ の部分空間であり、$\mathfrak{G}$ が点 $a \in \overline{X}$ の近傍フィルターの $X$ 上のトレースである場合、$\limsup_{x \to a, x \in X} f(x)$ [それぞれ$\limsup_{\mathfrak{G}} f$ の代わりに $\liminf_{x \to a, x \in X} f(x)$ [それぞれ$\liminf_{\mathfrak{G}} f$] ; $x$は$X$に留まりながら$a$になる傾向があるため、$\limsup$は$f(x)$の上位極限と呼ばれます。 $X$ が $\{a\}$ の補数である場合、これらの記法の「x \in X」の代わりに「x \neq a」と書きます。

$A$ が $a \in \overline{A}$ となるような $X$ の部分集合である場合、(系 2 から定理 3)

$$
\liminf_{x \to a, x \in X} f(x) \leq \liminf_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in X} f(x).
$$

$V$ が $Y$ の $a$ の近傍である場合、(系 3 から定理 3) になります。

$$
\limsup_{x \to a, x \in V \cap X} f(x) = \limsup_{x \to a, x \in X} f(x).
$$

したがって、トポロジー 空間の点にある上部および下部極限の概念は、極限の概念と同様に、ローカル指標の概念です。

最後に、$\mathfrak{G}$が$\mathbf{N}$のフレシェフィルタである場合、$\mathbf{N}$の$\overline{\mathbf{R}}$に入る写像$n \to u_n$のうち、$\mathfrak{G}$を基準とした上（または下）極限は$\limsup_{n \to \infty} u_n$（それぞれ下）で表されます。 $\liminf_{n \to \infty} u_n$) で、実数 $u_n$ の数列の上部 (それぞれ下部) 極限と呼ばれます。

したがって、関係 $\limsup_{n \to \infty} u_n = a \in \mathbf{R}$ は次と同等です。任意の $\varepsilon > 0$ が与えられると、整数 $n_0$ が存在し、それぞれの $n \geq n_0$ については $u_n \leq a + \varepsilon$ があり、$n$ の無限大の値については $u_n \geq a - \varepsilon$ が存在します。 数列の上の極限の定義は、その値が $+\infty$ または $-\infty$ の場合も同様に翻訳できます。

集合 $X$ で定義された実数値写像の数列 $(f_n)$ を考えると、任意の点における値の実数値写像を $\limsup_{n \to \infty} f_n$ (それぞれ $\liminf_{n \to \infty} f_n$) で表します。 $x \in X$ は $\limsup_{n \to \infty} f_n(x)$ [それぞれ$\liminf_{n \to \infty} f_n(x)$]。 (10) と (12) から推測します。
$$
\begin{cases}
\limsup_{n \to \infty} f_n = \inf_{n \in \mathbf{N}} (\sup_{m \geq n} f_m) = \lim_{n \to \infty} (\sup_{m \geq n} f_m), \\
\liminf_{n \to \infty} f_n = \sup_{n \in \mathbf{N}} (\inf_{m \geq n} f_m) = \lim_{n \to \infty} (\inf_{m \geq n} f_m),
\end{cases}
$$
極限は*積空間*$\overline{\mathbf{R}}^X$に撮影されています。 数列 $(f_n)$ は、$\limsup_{n \to \infty} f_n = \liminf_{n \to \infty} f_n$ (系 1 ～ 定理 3、および章 I, § 7, no. 6、系 1 ～ 命題) の場合に限り、$\overline{\mathbf{R}}^X$ に *極限* を持ちます。 10)。

### 7. 実数値写像に対する代数演算

$f$ と $g$ を集合 $X$ で定義された 2 つの実数値写像とします。 和 $f(x) + g(x)$ の場合 [それぞれ積 $f(x)g(x)$] がすべての $x \in X$ に対して定義されている場合、実数値写像を $f + g$ (それぞれ $fg$) で表します。
$$
x \mapsto f(x) + g(x) \quad \text{[resp. } x \mapsto f(x)g(x)].
$$
再度、$1/f(x)$ がすべての $x \in X$ に対して定義されている場合、$1/f$ は写像 $x \mapsto 1/f(x)$ を表します。

したがって、この最後の写像は、$f$ が値 0 をとらないという条件で定義されます。 $f$ が区間 $[0, +\infty]$ (それぞれ $[-\infty, 0]$) $1/f(x)$ の値を、$1/0 = +\infty$ (それぞれ $1/0 = -\infty$) を入れることで定義される場合。この場合、写像 $1/f$ が定義されます。

$X$ がフィルター $\mathfrak{F}$ でフィルターされ、$\lim_{\mathfrak{F}} f$ と $\lim_{\mathfrak{F}} g$ が存在するとします。 If on the one hand the function $f + g$ (resp. $fg$, $1/g$) is defined, and if on the other hand the expression $\lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g$ (resp. $\lim_{\mathfrak{F}} f \cdot \lim_{\mathfrak{F}} g$, $1/\lim_{\mathfrak{F}} f$) has a sense, then $\lim_{\mathfrak{F}} (f + g)$ [resp. $\lim_{\mathfrak{F}} fg$, $\lim_{\mathfrak{F}} (1/f)$] exists and is equal to this expression by reason of the continuity of the function $x + y$ (resp. $xy$, $1/x$) at points where it is defined.

#### 命題 12 {#top-iv-s5-prop-12 .statement tag=0BRR}

*$f$ と $g$ を集合 $X$ で定義された 2 つの実数値写像とし、$A$ を $X$ の空でない部分集合とします。

(i) *私たちは持っています*
$$
\begin{align*}
&\sup_{x \in A} (f(x) + g(x)) \leq \sup_{x \in A} f(x) + \sup_{x \in A} g(x), \\
&\sup_{x \in A} f(x) + \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x) + g(x)),
\end{align*}
$$
*これらの不等式の両辺が定義されるときはいつでも。*

(ii) *$f(x)$ と $g(x)$ がそれぞれ $x \in A$ に対して $\geq 0$ である場合、*

(19)
$$
\sup_{x \in A} (f(x)g(x)) \leq \sup_{x \in A} f(x) \sup_{x \in A} g(x),
$$
(20)
$$
\sup_{x \in A} f(x) \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x)g(x))
$$
*これらの不等式の両辺が定義されるときはいつでも。*

(iii) *すべての $x \in A$ に対して $f(x) \geq 0$ の場合、*
(21)
$$
\sup_{x \in A} (1/f(x)) = 1/\inf_{x \in A} f(x)
$$
*($1/0 = +\infty$を入れる).*

$H$ を $A$ の *有限* 部分集合とします。 $x_0$ が $H$ の点の 1 つである場合、$f + g$ はその最大の値をとります。
$$
f(x_0) + g(x_0) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x);
$$
一方、$x_1$ が $H$ の点の 1 つである場合、$f$ はその最大の値をとります。
$$
f(x_1) + g(x_1) \geq \sup_{x \in H} f(x) + \inf_{x \in H} g(x);
$$
したがって
$$
\sup_{x \in H} f(x) + \inf_{x \in H} g(x) \leq \sup_{x \in H} (f(x) + g(x)) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x).
$$
ここから、不等式 (17) と (18) は、no. 4 の適用命題 5 と no. 2 の定理 1 によって続きます。他の不等式の証明も同様です。

#### 系 1 {#top-iv-s5-prop-12-cor-1 .statement tag=0BRS}

*$f$を$X$で定義された実数値写像とし、$k$を実数とします。それから*
(22)
$$
\sup_{x \in A} (f(x) + k) = k + \sup_{x \in A} f(x)
$$
*両側が定義されている場合、および $k \geq 0,$* の場合
(23)
$$
\sup_{x \in A} (kf(x)) = k \cdot \sup_{x \in A} f(x)
$$
*両側が定義されている場合は常に*

#### 系 2 {#top-iv-s5-prop-12-cor-2 .statement tag=0BRT}

*$f_1$ と $f_2$ を、それぞれ集合 $X_1, X_2$ で定義された 2 つの実数値写像とします。次に、$A_1, A_2$ がそれぞれ $X_1, X_2$ の空ではない部分集合である場合、*
(24)
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) + f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) + \sup_{x_2 \in A_2} f_2(x_2)
$$

両側が定義されている場合は常に。そして、$f_1, f_2$ がそれぞれ $A_1, A_2$ の $\geq 0$ である場合、次のようになります。

$$
(25) \quad \sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1)f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) \sup_{x_2 \in A_2} f_2(x_2),
$$

両側が定義されている場合は常に。

これは、前の系の明らか帰結と、no. 4 の命題 9 です。

特に、$A$ と $B$ が和 $x + y \ (x \in A, y \in B)$ の集合 $A + B$ が定義されるように、$\overline{\mathbf{R}}$ の 2 つの部分集合である場合、次のようになります。

$$
(26) \quad \sup (A + B) = \sup A + \sup B
$$

右辺が定義されている場合。もう一度、$A$ と $B$ が $[0, + \infty]$ の 2 つの部分集合である場合、次のようになります。

$$
(27) \quad \sup AB = \sup A \cdot \sup B
$$

両側が定義されている場合は常に。

#### 命題 13 {#top-iv-s5-prop-13 .statement tag=0BRU}

*$f$ と $g$ を、フィルタリングされた集合 $X$ で定義された 2 つの実数値写像とします。*

(i) *私たちは持っています*

$$
(28) \quad \lim \sup (f + g) \leq \lim \sup f + \lim \sup g,
$$
$$
(29) \quad \lim \sup f + \lim \inf g \leq \lim \sup (f + g)
$$

*これらの不等式の両辺が定義されるときはいつでも。*

(ii) *$f$ と $g$ が $X$ の $\geq 0$ である場合、*

$$
(30) \quad \lim \sup fg \leq (\lim \sup f) (\lim \sup g),
$$
$$
(31) \quad (\lim \sup f) (\lim \inf g) \leq \lim \sup fg
$$

*これらの不等式の両辺が定義されるときはいつでも。*

(iii) *$f \geq 0$ が $X$ の場合、*

$$
(32) \quad \lim \sup (1/f) = 1/(\lim \inf f)
$$

($1/0 = + \infty$を入れる)。

これらの関係は、命題 12 と関係 (10) の帰結です

#### 系 1 {#top-iv-s5-prop-13-cor-1 .statement tag=0BRV}

*$f$ と $g$ を、フィルタリングされた集合 $X$ で定義された 2 つの実数値写像とします。 $\lim g$ が存在する場合、*

$$
(33) \quad \lim \sup (f + g) = \lim \sup f + \lim g
$$

両側が定義されている場合は常に、

(34) $$
\lim \sup fg = (\lim \sup f) (\lim g)
$$

両側が定義されており、$f$ と $g$ が $\geqslant 0$ である場合。

#### 系 2 {#top-iv-s5-prop-13-cor-2 .statement tag=0BRW}

$f$ と $g$ を、フィルタリングされた集合 $X$ で定義された 2 つの実数値写像とします。 $\lim f = +\infty$、$\lim \inf g > -\infty$、$f + g$ が定義されている場合は、$\lim (f + g) = +\infty$ になります。 $\lim f = +\infty$、$\lim \inf g > 0$、$fg$ が定義されている場合は、$\lim fg = +\infty$ になります。

### 練習問題 {#top-iv-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
