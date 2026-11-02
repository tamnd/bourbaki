---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 1
section_title: Prime ideals
lang: ja
source: ac-i-vii
book_pages: 51-55, 121-123
pdf_pages: 0071-0075, 0141-0143
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIME IDEALS
      page: 51
      pdf_page: 71
    - "no": 2
      title: RELATIVELY PRIME IDEALS
      page: 53
      pdf_page: 73
statements: 9
exercises: 11
content_sha256: d33b2bc8a8634cb2652aee59a3cad893c88d3a5eb817fdd834baf597e2cdf033
translated_from: content/en/ac/II/01_s1_prime_ideals.md
translation_method: google
source_content_sha256: 556d7efab2e0c3d357dfbbd27923b000a4c0af8dc523529bed393394168a1056
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 9c7b4387ad9276ba97724ebf6e5ad10a751b6779e76f81c0c0dc069f37059fdf
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. 最高の理想

### 1. 定義の主要な理想

#### 定義 1 {#ac-ii-s1-def-1 .statement tag=0450}

環 $A/p$ が整域の場合、環 $A$ の理想$p$ を素数と呼びます。

この定義により、次の 2 つの条件が成り立つ場合、環 $A$ の理想的な $p$ は素数になります。
(1) $p \neq A$;
(2) $x, y$ が $x \notin p$ と $y \notin p$ のように $A$ の 2 つの元である場合、$xy \notin p$ です。

これらの条件は、$\mathfrak{g}p$ 属するから $\mathfrak{g}p$ までの元の任意の有限族の積をというで表すこともできます。これは、適用この条件を空の集合にすると次のようになります。 $1 \notin p$。

$A/m$ は体であるため、$A$ の最大理想$m$ は素数です。次に、クルルの定理 (代数, 章 I, § 8, no. 7, 定理 2) から、

(*) 2 つのアスタリスク \* ... * の間に置かれた主張を除き、この章の結果は、この本の I ～ VI および章 I, §§ 1–3 にのみ依存します。

*以外* $\mathbf{A}$ が少なくとも 1 つの素イデアルに含まれています。特に、環 $\mathbf{A}$ に素イデアルが存在するには、$\mathbf{A}$ が 0 にならないことが必要十分です。

$f : \mathbf{A} \to \mathbf{B}$ を環準同型とし、$q$ を $\mathbf{B}$ の理想とします。 集合 $p = f^{-1}(q)$; 商を取って $f$ から導出された準同型 $\overline{f} : \mathbf{A}/p \to \mathbf{B}/q$ は単射法です。 $q$ が素数であると仮定します。 環 $\mathbf{B}/q$ は整域であるため、$\mathbf{A}/p$ も$\mathbf{B}/q$ の部分環と同型です。従って、理想的な $p = f^{-1}(q)$ は素数です。特に、$\mathbf{A}$ を $\mathbf{B}$ の部分環とします。 $\mathbf{B}$ のすべての理想 $q$ に対して、$q \cap \mathbf{A}$ は主要な理想 $\mathbf{A}$ です。 $f$ が全射法の場合、$\overline{f}$ は同型です。 条件「p は素数」と「$q$ は素数」は等価です。従って、$p$と$a$が$a \subset p$となるような$\mathbf{A}$の理想である場合、$p$が素数になるために必要かつ十分な条件は、$\mathbf{A}/a$において$p/a$が素数であることです。

#### 命題 1 {#ac-ii-s1-prop-1 .statement tag=0451}

*$\mathbf{A}$を環、$a_1, a_2, \ldots, a_n$を$\mathbf{A}$、$p$を$\mathbf{A}$の主な理想とします。 $p$ 含む積 $a_1 a_2 \ldots a_n$ の場合、含む $a_i$ の少なくとも 1 つです。*

実際、$p$ 含むが $a_i$ のどれもなかったと仮定します。 $1 \leq i \leq n$ の場合、元 $s_i \in a_i \cap p$ が存在します。すると、$s = s_1 s_2 \ldots s_n$ は $a_1 a_2 \ldots a_n$ に含まれ、$p$ には含まれません。これは不合理です。

#### 系 {#ac-ii-s1-n1-cor-1 .statement tag=0452}

*$m$を$\mathbf{A}$の最大の理想とする。すべての整数 $n > 0$ に対して、唯一の素のイデアル含む $m^n$ は $m$ です。*

このような理想 $p$ は、$1 \leq i \leq n$ に対して $a_i = m$ に 1 を適用して含む $m$ 命題を加算する必要があります。 $m$ が最大なので、$p = m$ です。

#### 命題 2 {#ac-ii-s1-prop-2 .statement tag=0453}

*$\mathbf{A}$を環、$a$を加法と乗法で閉じられる$\mathbf{A}$の空でない集合、そして$(p_i)_{i \in I}$を$\mathbf{A}$の空でない有限の理想族とする。 $a$ が $p_i$ の和集合に含まれており、$p_i$ のうち最大 2 つが素数ではないとします。すると、$a$ は $p_i$ の 1 つに含まれます。*

私たちは$n = \mathrm{Card}(I)$について帰納法までに議論します。 $n = 1$ であれば、命題は自明です。 $n \geq 2$; と仮定します。 添字 $j$ が存在する場合、$a \cap p_j \subset \bigcup_{i \neq j} p_i$、集合 $a$、つまり$i \in I$ が$a \cap p_i$ の和集合が$\bigcup_{i \neq j} p_i$ に含まれ、したがって帰納法の仮定による$p_i$ の 1 つに含まれる場合です。 次に、そのような添字が存在しないと仮定します。すべての $j \in I$ について、$y_j$ を $i \neq j$ の$p_i$ に対する所属ではなく、$a \cap p_j$ の元にします。 $n > 2$の場合は$p_k$が素数となり、$n = 2$の場合は任意に選択されるように、$k$を$I$の元とします。 $z = y_k + \prod_{i \neq k} y_i$ にしましょう。 次に、$a$ は加法と乗法で閉じられるため、$z \in a$ になります。 $j \neq k$、$\prod_{i \neq k} y_i$ 属するから $p_j$ の場合、$y_k \notin p_j$、よって $z \notin p_j$。 On the other hand, $\prod_{i \neq k} y_i$ does not belong to $p_k$, as none of the factors $y_i \ (i \neq k)$ belongs to it and $p_k$ is prime if $n - 1 > 1$; as $y_k \in p_k$, $z$ does not belong to $p_k$ and the proposition is established.

### 2. 比較的プライムな理想

$A$ を環とします。 $A$ の 2 つのイデアル $a, b$ が $a + b = A$ の場合、*相対素* と呼ばれます。これが真実であるためには、$a + b$ が素イデアル (*代数*、章 I, § 8, no. 7、定理 2) に含まれていないこと、他の語に含まれていないこと、$a$ と $b$ の両方に素イデアル含むが含まれていないことが必要かつ十分です。 2 つの異なる最大理想は比較的素です。

$A$ が *主イデアル整域* (*代数*, 章 VII, § 1) である場合、$A$ の 2 つの元 $a, b$ が相対的に素であることは、ベズーの恒等式 (*loc. cit.*, no. 2, 定理 1)、理想 $Aa$ と $Ab$ が互いに素であること。

#### 命題 3 {#ac-ii-s1-prop-3 .statement tag=0454}

*$a$ と $b$ を環 $A$ の 2 つの比較的素な理想とする。 $a'$ と $b'$ を、$a$ (それぞれ $b$) のすべての元が $a'$ (それぞれ $b'$) に冪を含むように、$A$ の 2 つの理想とする。この場合、$a'$ と $b'$ は相対的に素です。*

与えられた仮定の下で、すべての素イデアル含む $a'$ 含む $a$ とすべての素イデアル含む $b'$ 含む $b$。素の理想が含む $a'$ と $b'$ である場合、含む $a$ と $b$ になりますが、$a$ と $b$ は相対的に素であるため、これは不合理です。したがって、$a'$ と $b'$ は相対的に素です。

#### 命題 4 {#ac-ii-s1-prop-4 .statement tag=0455}

※$a, b_1, \ldots, b_n$を環$A$の理想とします。 $a$ がそれぞれの $b_i$ ($1 \leq i \leq n$) に対して互いに素である場合、$b_1 b_2 \ldots b_n$ に対して相対的に素です。

$p$を$A$の第一の理想とする。 $p$ 含む $a$ と $b_1 b_2 \ldots b_n$ の場合、含むは $b_i$ (no. 1, 命題 1) の 1 つになります。$a$ と $b_i$ は互いに素であるため、これは不合理です。

#### 命題 5 {#ac-ii-s1-prop-5 .statement tag=0456}

*$(a_i)_{i \in I}$を環$A$の空でない有限族とする。次のプロパティは同等です =
(a) $i \neq j$ の場合、$a_i$ と $a_j$ は互いに素です。
(b) *標準準同型* $\phi : A \to \prod_{i \neq I} (A/a_i)$ (*代数*, 章 11, § 1, no. 7) は全射です。
*これらが成り立つ場合、$a_i$ の共通部分 $a$ はそれらの積に等しく、標準準同型* $\phi : A/a \to \prod_{i \in I} (A/a_i)$ (*代数*, 章 II, § 1, no. 7) は全単射です。*

$I$の元の$n$数について帰納法によって議論しますが、$n = 1$の場合は自明です。まず、$n = 2$ の場合を考えてみましょう。すると、数列の正確さから (a) と (b) の同値が求まります。

$$
0 \longrightarrow A/(a_1 \cap a_2) \xrightarrow{\psi} (A/a_1) \oplus (A/a_2) \longrightarrow A/(a_1 + a_2) \longrightarrow 0
$$

(代数, 章 II, § 1, no. 7, 公式 (30))。さらに、$1 = e_1 + e_2$となるような$e_1 \in a$と$e_2 \in a_2$が存在します。次に、すべての $x \in a = a_1 \cap a_2$、$x = xe_1 + xe_2$;しかし、定義 $xe_1 \in a_1 a_2$ と $xe_2 \in a_1 a_2$ までなので、$x \in a_1 a_2$ になります。 よって $a \subset a_1 a_2$ と逆が含まれていることは明らかです。

一般的なケースでは、条件 (a) が成り立ち、$k$ を $I$ と $b_k = \bigcap_{i \neq k} a_i$ の元とします。 帰納法の仮定は $b_k = \prod_{i \in I} a_i$ を意味し、命題 4 から$a$ と $b$ が相対的に素であることがわかります。それから

$$
a = \bigcap_{i \in I} a_i = a, \quad \cap b_k = a_k b_k = \prod_{i \in I} a_i,
$$

引数の最初の部分と同じ理由で標準準同型 $A/a \twoheadrightarrow (A/a_k) \times (A/b_k)$ は全単射です。 帰納法の仮定標準準同型 $A/b_k \to \prod_{i \neq k} (A/a_i)$ は全単射なので合成準同型も成り立ちます

$$
A/a \to (A/a_k) \times (A/b_k) \to (A/a_k) \times \prod_{i \neq k} (A/a_i) = \prod_{i \in I} (A/a_i)
$$

これは正確には $\psi$ です。つまり、(b) が成り立ちます。 逆に、(b) が成り立つとします。 $a_i$ は必ず対で相対的に素であることを示します。 逆の場合、$i \neq j$ に対して、イデアル $c \neq A$ 含む $a_i$ および $a_j$ が存在します。 $h$ に対して集合 $a_h' = a_h$ は、$i$ または $j$ および $a_i' = a_j' = c$ に等しくありません。 標準準同型 $\phi': A \to \prod_{i \in I} (A/a_i')$ は合成写像として書くことができます

$$
A \xrightarrow{\phi} \prod_{i \in I} (A/a_i) \xrightarrow{f} \prod_{i \in I} (A/a_i')
$$

$f$ は標準準同型 $A/a_i \to A/a_i'$ の積です。明らかに$\phi'$は全射ではなく、$+(A)$の$(A/a_i') \times (A/a_i')$上の射影は積$(A/c) \times (A/c)$の対角線であり、$c \neq A$以降のこの積とは区別されます。 $f$ は全射であるため、これは $\phi$ が全射ではないことを示しています。

#### 命題 6 {#ac-ii-s1-prop-6 .statement tag=0457}

*$(a_i)_{i \in I}$ を、対において相対的に素である環 $A$ の空でない有限族とする。 $a$を$a_i$の共通部分とします。すべての $A$ モジュール $M$ について、標準写像 $M \to \prod_{i \in I} (M/a_i M)$ は全射であり、その核は $aM$ です。*

明らかに、$M$ から $\prod_{i \in I} (M/a_i M)$ の標準写像は、$aM$ では零です。次に、商を取ると、定義する準同型 $A : M/aM \to \prod_{i \in I} (M/a_i M)$ になります。一方、命題 5、標準準同型までには
$$
\psi : A/a \to \prod_{i \in I} (A/a_i)
$$
全客観的です。それから$1_M \otimes \psi : M \otimes (A/a) \to M \otimes \prod_{i \in I} (A/a_i)$もそうです。現在、$M \otimes (A/a)$ は $M/aM$ と同一視され、$M \otimes \prod_{i \in I} (A/a_i)$ は $\prod_{i \in I} M \otimes (A/a_i)$ と同一視され、$\prod_{i \in I} (M/a_i M)$ と同一視されます。上記の識別変換 $1_M \otimes \psi$ が $\lambda$、よって命題に変換されることがすぐに検証されます。

#### 例 {#ac-ii-s1-n2-exa-1 .statement tag=0458}

Let $K$ be a field, $a, (1 \leq i \leq m)$ distinct elements of $K$ and, for each $i$, let $g_i$ be a polynomial in $K[X]$; the principal ideal $(X - a_i) = m_i$ is maximal in $K[X]$, hence, for every system $(n_i)_{1 \leq i \leq m}$ of $m$ integers $\geq 1$, the ideals $m_i^{n_i}$ are relatively prime in pairs. 次に、命題 5 から、$1 \leq i \leq m$ に対して $f(X) \equiv g_i(X) \pmod{(X - a_i)^{n_i}}$ となるような多項式 $f \in K[X]$ が存在し、そのような 2 つの多項式の差は $\omega(X) = \prod_{i=1}^m (X - a_i)^{n_i}$ で割り切れるということがわかります。 すべての $n_i$ が 1 に等しいとすると、問題はラグランジュ補間公式 (*代数*, 章 IV, § 2, no. 4) によって明示的に解決されることがわかります。

### 練習問題 {#ac-ii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
