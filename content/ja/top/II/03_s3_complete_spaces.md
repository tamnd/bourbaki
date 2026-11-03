---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 3
section_title: Complete spaces
lang: ja
source: top-i-iv
book_pages: 181-198, 208-209
pdf_pages: 0187-0204, 0214-0215
extraction: ocr
subsections:
    - "no": 1
      title: CAUCHY FILTERS
      page: 181
      pdf_page: 187
    - "no": 2
      title: MINIMAL CAUCHY FILTERS
      page: 183
      pdf_page: 189
    - "no": 3
      title: COMPLETE SPACES
      page: 184
      pdf_page: 190
    - "no": 4
      title: SUBSPACES OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 5
      title: PRODUCTS AND INVERSE LIMITS OF COMPLETE SPACES
      page: 186
      pdf_page: 192
    - "no": 6
      title: EXTENSION OF UNIFORMLY CONTINUOUS FUNCTIONS
      page: 190
      pdf_page: 196
    - "no": 7
      title: THE COMPLETION OF A UNIFORM SPACE
      page: 191
      pdf_page: 197
    - "no": 8
      title: THE HAUSDORFF UNIFORM SPACE ASSOCIATED WITH A UNIFORM SPACE
      page: 196
      pdf_page: 202
    - "no": 9
      title: COMPLETION OF SUBSPACES AND PRODUCT SPACES
      page: 197
      pdf_page: 203
statements: 48
exercises: 7
content_sha256: cce40f3c1f6274c9ec1ff32e0ad5ac561d0a04753662a8683425cf3fb34ae260
translated_from: content/en/top/II/03_s3_complete_spaces.md
translation_method: google
source_content_sha256: 4fff5edd8ba62b0c67040f4aad9934e1ca08a8f7749a27d75004f56f99335c47
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 21ff4460caddac8190018c5678b9e38a64eedbd25dcfe99b5527dfa354a191fe
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 空間を完了する

### 1. コーシーフィルター

集合 $X$ に制服構造が与えられると、$X$ の「小さい」部分集合 (この構造と比較して) が何を意味するのかを定義する知ることができます。$X$ の「小さい」部分集合は、すべての点が揃うものです。お互いに「非常に近い」です。正確に：

#### 定義 1 {#top-ii-s3-def-1 .statement tag=0BEE}

$X$ が均一空間で、$V$ が $X$ の側近である場合、$A$ の点のすべてのペアが $V$ に近い場合 (つまり、$A \times A \subset V$ の場合)、$X$ の部分集合 $A$ は $V$-小さい と言われます。

#### 命題 1 {#top-ii-s3-prop-1 .statement tag=0BEF}

一様空間 $X$ では、2 つの集合 $A$ と $B$ が $V$-小で交差する場合、それらの和集合 $A \cup B$ は $\vec{V}$-小 です。

$x$ と $y$ を $A \cup B$ の任意の 2 つの点とし、$Z \in A \cap B$ とします。次に、$(x, z) \in V$ と $(z, y) \in V$ なので、$(x, y) \in \overline{V}$ になります。

#### 定義 2 {#top-ii-s3-def-2 .statement tag=0BEG}

*ユニフォーム空間 $X$ のフィルター $\mathfrak{F}$ は、$X$ の各取り巻き $V$ に、$V$ が小さく、属する ～ $\mathfrak{F}$ である $X$ の部分集合がある場合、コーシーフィルターです。

ここでも、「十分に小さい集合」と「必要なだけ小さい集合」という表現を使用して、言語をより表現力豊かにすることができます。したがって、定義 2 は、というによってコーシーフィルターが 1 つ含む *任意に小さい集合* であると言い換えることができます。

数列に関連付けられた基本フィルターがコーシー フィルターである場合、一様空間 $X$ の点の無限数列 $(u_n)$ は、*コーシー 数列* であると言われます。 $X$ の各取り巻き $V$ には整数 $n_0$ があり、すべての整数 $m \geq n_0$ と $n \geq n_0$ には $(u_m, u_n) \in V$ があると言うのも同じことになります。

#### 命題 2 {#top-ii-s3-prop-2 .statement tag=0BEH}

*均一空間 $X$ では、すべての収束フィルターはコーシー フィルターになります。*

$x$ が $X$ の任意の点で、$V$ が $X$ の対称な取り巻きである場合、$x$ の近傍 $V(x)$ は $\overline{V}$-small です。 $\mathfrak{F}$が$x$に収束するフィルタである場合、$V(x)$には$\mathfrak{F}$の集合が含まれるため、$V$は小さいです。

明らかに、コーシー フィルターより *より細かい* であるすべてのフィルターはコーシー フィルターです。

#### 命題 3 {#top-ii-s3-prop-3 .statement tag=0BEI}

※$f : X \to X'$を一様連続の写像とします。次に、$X$ のコーシー フィルター 基底の $f$ の下の像は、$X'$ のコーシー フィルター 基底です。

$g = f \times f$ にしましょう。 $V'$ が $X'$ の側近である場合、$\overline{g^{-1}(V')}$ は $X$ の側近であり、$\overline{g^{-1}(V')}$-小さい集合の $f$ の下の像は $V'$-小さいです。したがって結果です。

特に、均一空間 $X$ の均一性が *粗い* 均一性で置き換えられた場合、元の均一性に関するすべてのコーシー フィルターは、新しい均一性に関してはコーシー フィルターのままになります。

この事実は、次の形で簡単に思い出すことができます: *より細かい均一性が高いほど、コーシー フィルターの数は少なくなります*。

#### 命題 4 {#top-ii-s3-prop-4 .statement tag=0BEJ}

*$X$を集合、$(Y_i)_{i \in I}$を均一空間の家族とし、それぞれの$i \in I$について、$f_i$を$X$の写像を$Y_i$にします。 $X$ に、$f_i$ が均一に連続する最も粗い均一性 $U$ を持たせます。次に、位数では、$X$ のフィルター 基底 $\mathfrak{B}$ はコーシーフィルター 基底である必要があり、各 $i \in I$ について、$f_i(\mathfrak{B})$ は$Y_i$ のコーシーフィルター基底であることが必要かつ十分です。

条件は命題 3 には必要である。逆にそれが満たされると仮定し、$U(V_{i_1}, \ldots, V_{i_n})$ を均一性 $\mathfrak{U}$ [§ 2, no. 3, 公式 (1)] の取り巻きとする。 仮定までに、添字 $k$ ごとに集合 $M_k \in \mathfrak{B}$ があり、$f_{i_k}(M_k)$ は$V_{i_k}$ が小さい ($1 \leq k \leq n$) になります。 $M$を、$1 \leq k \leq n$の$M_k$に含まれる$\mathfrak{B}$の集合とします。次に、点 $x, x'$ $M$ のそれぞれの対に対して、$1 \leq k \leq n$ に対して $[f_{i_k}(x), f_{i_k}(x')] \in V_{i_k}$ が得られます。
$$
(x, x') \in U(V_{i_1}, \ldots, V_{i_n}).
$$
これで証明は完了です。

#### 系 1 {#top-ii-s3-prop-4-cor-1 .statement tag=0BEK}

*ユニフォーム空間 $X$ 誘導するのコーシー フィルターが $X$ の部分集合 $A$ のフィルターである場合、このフィルターはユニフォーム部分空間 $A$ のコーシー フィルターです。

#### 系 2 {#top-ii-s3-prop-4-cor-2 .statement tag=0BEL}

*制服空間の積 $\prod_{i \in I} X_i$ のフィルター 基底 $\mathfrak{B}$ は、各 $i \in I$、$\operatorname{pr}_i(\mathfrak{B})$ が $X_i$ のコーシーフィルター 基底である場合に限り、コーシーフィルター 基底です。

### 2. 最小限のコーシーフィルター

一様空間 $X$ 上のコーシー フィルターの集合の最小元 (包含に関して) は、$X$ 上の *最小コーシー フィルター* と呼ばれます。

#### 命題 5 {#top-ii-s3-prop-5 .statement tag=0BEM}

※$X$を制服空間とします。 $X$ 上の各コーシー フィルター $\mathfrak{F}$ には、$\mathfrak{F}$ よりも粗い固有の最小コーシー フィルター $\mathfrak{F}_0$ があります。 $\mathfrak{B}$ が $\mathfrak{F}$ の基底で、$\mathfrak{G}$ が $X$ の対称取り巻きの基本系である場合、集合 $V(M)$ ($M \in \mathfrak{B}, V \in \mathfrak{G}$) 形基底 $\mathfrak{F}_0$。

$M, M'$ が $\mathfrak{B}$ にあり、$V, V'$ が $\mathfrak{G}$ にある場合、集合 $M'' \in \mathfrak{B}$ (それぞれ $V'' \in \mathfrak{G}$) があり、$M'' \subset M \cap M'$ (それぞれ $V'' \subset V \cap V'$) になります。したがって $V''(M'') \subset V(M) \cap V'(M')$ なので、$X$ のフィルター $\mathfrak{F}_0$ の集合 $V(M)$ ($M \in \mathfrak{B}, V \in \mathfrak{G}$) は確かに形基底になります。さらに、$M$ が $V$ 小さい場合、$V(M)$ は $V$ 小さいです。したがって、$\mathfrak{F}_0$ はコーシー フィルターであり、$\mathfrak{F}$ よりも明らかに粗くなっています。 証明を完了するには、$\mathfrak{G}$ が $\mathfrak{F}$ よりも粗いコーシーフィルターである場合、$\mathfrak{G}$ は $\mathfrak{F}_0$ よりもより細かいであることを示すだけで十分です。それぞれの $M \in \mathfrak{B}$ とそれぞれの $V \in \mathfrak{G}$ には集合 $N \in \mathfrak{G}$ があり、これは $V$ の小さいものです。 $N \in \mathfrak{F}$ 以降、$N$ は $M$ と一致します。したがって$N \subset V(M)$、したがって$V(M) \in \mathfrak{G}$です。

#### 系 1 {#top-ii-s3-prop-5-cor-1 .statement tag=0BEN}

*それぞれの $x \in X$、近傍では、$X$ の $x$ の $\mathfrak{B}(x)$ が最小のコーシー フィルターです。

命題 5 の $\mathfrak{F}$ を、含む $x$ である $X$ のすべての部分集合のフィルターとし、$\mathfrak{B}$ を単一の元 $\{x\}$ で構成します。

#### 系 2 {#top-ii-s3-prop-5-cor-2 .statement tag=0BEO}

*すべてのクラスター 点* $x$ *コーシー フィルター* $\mathfrak{F}$ * は * $\mathfrak{F}$ の極限点です。

$\mathfrak{F}$ と $\mathfrak{B}(x)$ の両方よりもより細かいであるフィルター $\mathfrak{G}$ があります (章 I, § 7, no. 2、命題 4)。 $\mathfrak{F}$ は Cauchy フィルターなので、$\mathfrak{G}$ も同様です。 $\mathfrak{F}_0$ が $\mathfrak{F}$ より粗い固有の最小コーシー フィルターである場合、$\mathfrak{F}_0$ と $\mathfrak{B}(x)$ は両方とも $\mathfrak{G}$ より粗い最小コーシー フィルターです。したがって、$\mathfrak{F}_0 = \mathfrak{B}(x)$ は、$\mathfrak{F}$ が $x$ に収束することを示しています。

#### 系 3 {#top-ii-s3-prop-5-cor-3 .statement tag=0BEP}

*各コーシー フィルターは、点* $x$ に収束するフィルターよりも粗く、*$x$ にも収束します。

系 2の帰結です。

#### 系 4 {#top-ii-s3-prop-5-cor-4 .statement tag=0BEQ}

*もし* $\mathfrak{F}$ * が最小コーシーフィルターであれば、* $\mathfrak{F}$ * のすべての集合は空ではない内部を持ち、また属するから* $\mathfrak{F}$ * (他の語、$\mathfrak{F}$ には基底からなるが含まれます) 集合)* を開きます。

$V$ を $X$ の取り巻きとする。次に、オープンな側近$U \subset V$ ($\S$ 1、no. 2、系 2 ～ 命題 2) がいます。 $X$ の各部分集合 $M$ では、$U(M)$ が開いており、$V(M)$ に含まれています。したがって、命題 5 を考慮した結果です。

### 3. 完了空間

ユニフォーム空間 $X$ では、*コーシーフィルターには極限点* は必要ありません。

#### 例 1 {#top-ii-s3-n3-exa-1 .statement tag=0BER}

$u_n = \sum_{p=0}^n 2^{-p(p+1)/2}$ で定義される有理直線 $\mathbf{Q}$ 上の数列 $(u_n)$ を考えます。 $m > n$ がある場合
$$
|u_m - u_n| \leq 2^{-n(n+3)/2}
$$
したがって、$(u_n)$ は *Cauchy 数列* です。しかし、この数列には$\mathbf{Q}$には極限がありません。なぜなら、有理数数 $a/b$ が $(u_n)$ の極限である場合、(1) によってすべての $n$ が得られるはずです。
$$
|a/b - h_n/2^{n(n+1)/2}| \leq 1/2^{n(n+3)/2}
$$
ここで、$h_n$ は整数 ($n$ に応じて) です。つまり、
$$
|a \cdot 2^{n(n+1)/2} - b h_n| \leq b \cdot 2^{-n}
$$
$n$ 全員のために。さて、この不等式の左辺は、すべての $n$ に対して整数であるため、$b < 2^{n_0}$ のように $n$ が整数 $n_0$ より大きい場合は常に零となる必要があります。したがって、すべての $n > n_0$ に対して $a/b = u_n$ が必要ですが、これは不合理です。

#### 例 2 {#top-ii-s3-n3-exa-2 .statement tag=0BES}

$X$ を無限大集合とし、$X$ ($\S$ 2, no. 2, 注意 1) 上の有限分割の一様性を考えます。 $X$ 上のすべての *ウルトラフィルター* $\mathfrak{F}$ は、

この均一性に関する Cauchy フィルター。 $(A_i)$ が $X$ の有限分割であり、
$$
V = \bigcup_i (A_i \times A_i)
$$
対応する側近、その後、$A_i$ 属する ～ $\mathfrak{F}$ (章 I, § 6, no. 4、系 ～ 命題 5) の少なくとも 1 つ、および $A_i$ は V 小さい。一方、$X$ は無限離散空間であるためコンパクトではなく、その結果、$X$ には収束しない限外フィルターが存在します。

#### 定義 3 {#top-ii-s3-def-3 .statement tag=0BET}

*完全な空間は、すべてのコーシー フィルターが収束する一様な空間です。*

従って、完全な空間では、すべての *Cauchy 数列* (no. 1) は収束します。

#### 例 {#top-ii-s3-n3-exa-3 .statement tag=0BEU}

*離散* 均一空間 $X$ では、コーシー フィルターは自明な限外フィルター (章 I, § 6, no. 4) であるため、収束します。その結果、$X$が完成しました。

no. 1 の定義 2 と 3 および no. 1 の命題 2 から、*コーシーの基準* として知られる次の命題を導き出します。

#### 命題 6 {#top-ii-s3-prop-6 .statement tag=0BEV}

*$\mathfrak{F}$を集合$X$のフィルターとし、$f$を$X$の写像として完全なユニフォーム空間$X'$とします。この場合、$f$ の下の $\mathfrak{F}$ の像がコーシー フィルター 基底である場合に限り、$f$ は $\mathfrak{F}$ に関して極限になります。

この基準は、極限の概念を含むすべての質問において完全な空間が重要であることを示しています。写像がその値を完全な空間で取得した場合、証明できるは極限の*存在*を、事前に知る必要はありません。 極限* の値; 極限のうち定義が自由に使える唯一の収束基準である場合、これは不可能です。

完全な空間の均一性より *より細かい* である均一性は、完全な空間 (練習問題 2) の均一性である必要はありません。ただし、次の命題があります。

#### 命題 7 {#top-ii-s3-prop-7 .statement tag=0BEW}

*$\mathfrak{U}_1, \mathfrak{U}_2$ を集合 $X$ 上の 2 つの均一性とし、$\mathfrak{T}_1, \mathfrak{T}_2$ をこれらの均一性によって引き起こされるトポロジーとします。 $\mathfrak{U}_1$ が $\mathfrak{U}_2$ よりもより細かいであり、位相 $\mathfrak{T}_2 \times \mathfrak{T}_2$ の $X \times X$ で閉じられる $\mathfrak{U}_1$ の側近の基本系があるとします。次に、$X$ のフィルター $\mathfrak{F}$ は、均一性 $\mathfrak{U}_1$ のコーシーフィルターである場合に限り、位相 $\mathfrak{T}_1$ に収束し、位相 $\mathfrak{T}_2$ に収束します。

$\mathfrak{T}_2$ は $\mathfrak{T}_1$ よりも粗いため、条件は明らかに必要です。逆に、条件が満たされていると仮定し、$x$を$\mathfrak{T}_2$に対して$\mathfrak{F}$の極限点とする。 $x$ は $\mathfrak{T}_1$ に関して $\mathfrak{F}$ の極限であることを示します。 $V$ を、位相 $\mathfrak{T}_2 \times \mathfrak{T}_2$ で閉じられる $\mathfrak{U}_1$ の対称な取り巻きとします。 仮定, $\mathfrak{F}$ 含む集合 $M$ では、V が小さいです。従って、$x' \in M$ の場合、$M \subset V(x')$ になります。ただし、$V(x')$ は位相 $\mathfrak{T}_2$ に閉まります。従って、$\mathfrak{T}_2$ に対する$M$ の閉包にある $x$ は、属するから $V(x')$ でなければなりません。従って、$M \subset \hat{V}(x)$、命題が証明されます。

#### 系 {#top-ii-s3-n3-cor-1 .statement tag=0BEX}

命題 7 の条件で、$U_2$ が完全な空間の均一性である場合、$U_1$ も同様です。

$U_1$ に関するすべてのコーシー フィルターは、$U_2$ に関するコーシー フィルターとなるため、位相 $\mathfrak{T}_2$ に収束します。

系 ～ 命題 7 の仮説は、$\mathfrak{T}_1 = \mathfrak{T}_2$ (§ 1, no. 2、系 2 ～ 命題 2) のときに満たされることに注意してください。

### 4. 部分空間 / 完了空間

#### 命題 8 {#top-ii-s3-prop-8 .statement tag=0BEY}

完全な空間のすべての閉じられた部分空間が完了します。ハウスドルフのユニフォーム空間のすべての完全な部分空間 (完全であるかどうかに関係なく) は閉じられています。

$X$ を完全な空間とし、$A$ を $X$ の閉じた部分空間とします。 $\mathfrak{F}$ が $A$ のコーシー フィルターである場合、それは $X$ (no. 1、命題 3) のコーシー フィルター 基底であるため、点 $x \in X$ に収束します。しかし、$A$ が閉じているため、$x \in A$ があり、したがって、$\mathfrak{F}$ は部分空間 $A$ に収束します。

ここで、$\overline{A}$ をハウスドルフユニフォーム空間 $X$ の閉じていない部分集合とし、$b \in \overline{A} - A$ とします。 $X$ の $b$ の $\mathfrak{B}$ フィルターの近傍の $A$ 上のトレース $\mathfrak{B}_A$ は、$A$ のコーシーフィルターです。しかし、できないは点 $c \in A$ に収束します。そうでない場合、$c$ は $\mathfrak{B}$ (no. 2, 命題 5, 系 3) の極限点になります。これは不合理です。 $b \neq c$と$X$はハウスドルフです。

#### 命題 9 {#top-ii-s3-prop-9 .statement tag=0BEZ}

$X$ を均一空間とし、$A$ を $X$ の密な部分集合とし、$A$ 上のすべてのコーシー フィルター 基底が $X$ に収束するようにします。これで$X$は完了です。

$X$ 上のすべての最小コーシー フィルター $\mathfrak{F}$ が収束することを示すだけで十分です。 $A$ は密であり、$\mathfrak{F}$ のすべての集合には空ではない内部 (no. 2、系 4 ～ 命題 5) があるため、$A$ 上の$\mathfrak{F}$ のトレース $\mathfrak{F}_A$ は、 $A$、したがって、点 $x_0 \in X$ に収束します。 $\mathfrak{F}$ は、$\mathfrak{F}_A$ によって生成された $X$ のフィルターより粗いため、$\mathfrak{F}$ は $x_0$ (no. 2、系 3 ～ 命題 5) に収束します。

### 5. 積と完全な空間の逆数極限

#### 命題 10 {#top-ii-s3-prop-10 .statement tag=0BF0}

完全ユニフォーム空間のすべての積が完成しました。逆に、空でないユニフォーム空間の積が完全であれば、因子はそれぞれ完全なユニフォーム空間になります。

最初の主張は、コーシー フィルターの特徴付けと、積空間 (no. 1、系 2 ～ 命題 4 および章) の収束フィルターの帰結です。 I, § 7, no. 6、系 1 ～ 命題 10)。逆に仮定すると、

$$
X = \prod_{i \in I} X_i
$$

は完了しており ($X_i$ は空ではない)、$\mathfrak{F}_x$ を $X_x$ の Cauchy フィルターにします。それぞれの $i \neq x$ について、$\mathfrak{F}_i$ を $X_i$ のコーシー フィルターとし、積フィルター (章 I, § 6, no. 7) を考慮します。

$$
\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i \text{ on } X;
$$

$\mathfrak{F}$ はコーシー フィルター (no. 1、系 2 ～ 命題 4) であるため収束します。したがって、各 $\operatorname{pr}_x \mathfrak{F} = \mathfrak{F}_x$ (章 I, § 7, no. 6、系 1 ～ 命題) も同様です。 10)。

#### 系 {#top-ii-s3-n5-cor-1 .statement tag=0BF1}

*$(X_\alpha, f_{\alpha\beta})$ *を均一空間の逆数系とします。* *$X_\alpha$ *がハウスドルフで完全であれば、* $X = \varprojlim X_\alpha$ も同様です。

$X$ はハウスドルフであり、$\prod_{i \in I} X_\alpha$ (章 I, § 8, no. 2、系 2 ～ 命題 7) の *クローズ* 部分空間で識別できます。したがって、系は、命題 10 と命題 8 (no. 4) から続きます。

An inverse limit of complete Hausdorff uniform spaces $X_\alpha$ can be *empty*, even if all the $X_\alpha$ are non-empty and all the $f_{\alpha\beta}$ are surjective, as is shown by the case of discrete spaces (*Set Theory*, Chapter III, § 1, Exercise 32). ただし、次の定理があります。

#### 定理 1 (ミタグ・レフラー) {#top-ii-s3-thm-1 .statement tag=0BF2}

*$(X_\alpha, f_{\alpha\beta})$ * を完全なハウスドルフ均一空間の逆数系とし、有向集合* $I$ * 可算末尾部分集合を持つものとします。また、それぞれ* $\alpha \in I$、$X_\alpha$ * には数えられる基本的な系の取り巻きがある* (*) と仮定します。 *最後に、それぞれ* $\alpha \in I$ * 添字* $\beta \geq \alpha$ *満たすに次の条件* があると仮定します。

(ML$_{\alpha\beta}$) *それぞれ* $\gamma \geq \beta$、$f_{\alpha\gamma}(X_\gamma)$ *が密集* $f_{\alpha\beta}(X_\beta)$。

*$X = \varprojlim X_\alpha$ *そして* $f_\alpha$ *標準写像* $X \to X_\alpha$ とします。 *次に、それぞれ* $\alpha \in I$ *およびそれぞれ* $\beta \geq \alpha$ *満たす* (ML$_{\alpha\beta}$)、$f_\alpha(X)$ *は$f_{\alpha\beta}(X_\beta)$ * に密集しています*(従って* $X_\alpha$ *すべてが空でない場合、* $X$ *は空ではありません)*。

$(\lambda_n)$ を $I$ の添字コファイナルの数列とします。 添字 $\alpha_0 \in I$ と定義するから再帰的に増加する数列 $(\alpha_n)$ を開始し、$\alpha_n \geq \lambda_n$ および (ML$_{\alpha_n, \alpha_{n+1}}$) が true になるようにします。明らかに数列

(*) *この条件は、ハウスドルフのユニフォーム空間* $X_\alpha$ * がメトリズ可能であることを意味します。 cf. 章 IX, § 2, no. 4、定理 1.*

(α_n) は I の共同最終です。 m ≤ n の場合は f_{α_mα_n} の代わりに f_{mn} と書き、f_{n, n+1}(X_{α_{n+1}}) = Y_n とします。次に、m ≤ n の場合、f_{mn}(Y_n) は Y_m 内で密になります。なぜなら、定義 f_{m, n+1}(X_{α_{n+1}}) は密集しているからです。

f_{m, m+1}(X_{α_{m+1}}) = Y_m、および f_{m, n+1}(X_{α_{n+1}}) = f_{mn}[f_{n, n+1}(X_{α_{n+1}})] = f_{mn}(Y_n)。

n と k の帰納法により、各 n に対して X_{α_n} の閉じた対称包囲の基本システム (V_{kn})_{k∈\mathbf{N}} を次のように定義できます。

(2)
$\overset{2}{V}_{k+1, n} \subset V_{kn}$、

(3)
$(f_{n, n+1} \times f_{n, n+1})(V_{k, n+1}) \subset V_{kn}$。

実際には、(U_{kn})_{k∈\mathbf{N}} を X_{α_n} の取り巻きの基本系とします。 V_{kn} が与えられた n とすべての k ∈ \mathbf{N} に対して定義されていると仮定すると、f_{n, n+1} は一様連続であるため、取り巻き V_{k, n+1} を k 上で帰納法によって定義するできるため、(3) が満たされ、

$\overset{2}{V}_{k+1, n+1} \subset V_{k, n+1} \cap U_{k+1, n+1}$

主張が続きます。

ここで、x_0 ∈ Y_0 とします。各整数 k > 0 に対して、 [x_0, f_{α_0}(z)] ∈ V_{k-1, 0} となるような点 z ∈ X が存在することを示します。これで定理が証明されます。 f_{n, n+1} (Y_{n+1}) は Y_n 内で密であるため、次のように点 x_n ∈ Y_n の帰納法数列によって定義するができます。

(4)
$$ [x_n, f_{n, n+1}(x_{n+1})] \in V_{k+n, n} $$

(3) の理由により、m ≤ n の場合、

(5)
$$ [f_{mn}(x_n), f_{m, n+1}(x_{n+1})] \in V_{k+n, m} $$

これから、結論する、固定 m 数列 (f_{mn}(x_n))_{n≥m} は、X_{α_m} のコーシー 数列であるため、点 z_m に収束します。なぜなら、帰納法により、(5) から、整数 p ≥ m、q > 0 の各対について、次のようになります。

(6)
$$ [f_{mp}(x_p), f_{m, p+q}(x_{p+q})] \in V_{k+p+q-1, m} \circ V_{k+p+q-2, m} \circ ... \circ V_{k+p, m} $$

(2) により、(6) の右辺が V_{k+p-1, m} に含まれることは明らかです。 q が無限に増加するとします。特に、m = p = 0 の場合、V_{k-1, 0} が閉じているため、(x_0, z_0) ∈ V_{k-1, 0} となると推論します。一方、関係 z_m = \lim_{n→∞} f_{mn}(x_n) と f_{m, m+1} の連続性から、各 m ≥ 0 に対して f_{m, m+1}(z_{m+1}) = z_m であると推定されます。各 γ ∈ I には少なくとも 1 つあります。 整数 n は α_n ≧ γ となる。 $z_\gamma = f_{\gamma, \alpha_n}(z_n)$ を置くと、$z_\gamma$ が $\alpha_n \geq \gamma$ のように $n$ の値に依存しないこと、およびそのように定義されたファミリー $(z_\alpha)_{\alpha \in I}$ が $X = \varprojlim X_\alpha$ の点 $z$ であることをすぐに検証します。 $f_{\alpha_0}(z) = z_0$なので証明は完了です。

#### 系 1 {#top-ii-s3-thm-1-cor-1 .statement tag=0BF3}

*$(X_\alpha, f_{\alpha \beta})$ * を、有向集合* $I$ * によってインデックス付けされた集合の逆数系とし、可算余末部分集合を持ち、* $f_{\alpha \beta}$ * が全射であると仮定します。次に、* $X = \varprojlim X_\alpha$、*標準写像* $f_\alpha : X \to X_\alpha$ *それぞれ* $\alpha \in I$ について全射であるとします。

それぞれの $X_\alpha$ に離散的な均一性を持たせ、定理を適用するに 1 を持たせます。

#### 系 2 {#top-ii-s3-thm-1-cor-2 .statement tag=0BF4}

*$I$ *を可算末尾部分集合を持つ有向集合とします。 * $(X_\alpha, f_{\alpha \beta})$ *と* $(X'_\alpha, f'_{\alpha \beta})$ *を* $I$でインデックス付けされた集合の2つの逆数系とし、*それぞれ* $\alpha \in I$ *$u_\alpha : X_\alpha \to X'_\alpha$ *を写像とし、* $u_\alpha$ *形写像の逆系。しましょう* $u = \varprojlim u_\alpha$。 *$x = (x'_\alpha)$ *を元にしましょう*

$$
X' = \varprojlim X'_\alpha
$$

*次の条件を満たす: それぞれ* $\alpha \in I$ * 添字* $\beta \geq \alpha$ *すべてに対して* $\gamma \geq \beta$ * $f_{\alpha \gamma}(\overline{u}_\gamma^{-1}(x_\gamma)) = f_{\alpha \beta}(\overline{u}_\beta^{-1}(x'_\beta))$ があります。 *次に、元* $x \in X$ *そのような* $u(x) = x'$ があります。

定理を適用する 1 から集合 $\overline{u}_\alpha^{-1}(x'_\alpha)$ の逆数系であり、それぞれ離散的な均一性を持ちます。

#### 例 {#top-ii-s3-n5-exa-1 .statement tag=0BF5}

$C$ で与えられたとします: (i) 数列 $(|a_n|)$ が増加するであり、$+\infty$ になる傾向があるような、別個の点の数列 $(a_n)$。 (ii) 各 $n$ について、$C - \{a_n\}$ で定義され、$a_n$ に極を持つ有理数写像 $z \to R_n(z)$。 (iii) 0 を中心とする開いた円盤の増加する数列 $(B_n)$、その和集合は $C$ で、$a_k$ のどれも円盤 $B_n$ の境界上にありません。それぞれの $n$ について、$B'_n$ は $\overline{B}_n$ の共通部分と点 $a_n$ の集合の $C$ の補数を表します。そして、$X_n$ がすべての写像のうちの集合を表すものとします。

$$
z \to S(z) = P(z) + \sum_{a_k \in B'_n} R_k(z)
$$

$B'_n$ を $C$ に変換します。ここで、$P$ は写像の制限から $B'_n$ で、$\overline{B}_n$ では連続で、$B_n$ では正則です。 定義するを$X_n$ に入れることでメトリクスを計算します

$$
d_n(S_1, S_2) = \sup_{z \in B'_n} |S_1(z) - S_2(z)|.
$$

$X_n$ がこの指標に関して *完全* であることは簡単に検証できます。最後に、$n \leq m$ について、$S \in X_m$ の場合、$f_{nm}(S)$ が $S$ から $B'_n$ の *制限* になるように、定義する写像 $f_{nm} : X_m \to X_n$ を計算します。 $f_{nm}$ が *一様連続* であり、$(X_n, f_{nm})$ が一様空間の逆系であることは明らかです。そうなると、逆数極限 $X = \lim_{\leftarrow} X_n$ の元は、$\mathbf{C}$ の有理同型写像 $F$ と正準的に同定できます。その極は点 $a_n$ のみであり、各 $n$ について、 $F(z) - R_n(z)$ は $a_n$ で正則です。ミタグ＝レフラーの古典的な定理は、$X$ は空ではないと主張しています。 定理 1 により、すべての $n$ について条件 (ML$_{nn}$) を検証するだけで済みます。しましょう
$$
S_n = P_n + \sum_{a_k \in B_n} R_k
$$
$X_n$ の元であり、$P_n$ は $\overline{B}_n$ では連続であり、$B_n$ では正則です。任意の $m \geq n$ について、$Q_{mn}$ を制限とします
$$
\sum_{a_h \in B_m - B_n} R_h \text{ to } B'_n;
$$
この後者の和は、$\overline{B}_n$ の一部の近傍において正則な写像であるため、(テイラーの定理により) 各 $\varepsilon > 0$ に対して、$B_n$ で $|Q_{mn}(z) - P_{mn}(z)| \leq \varepsilon$ となるような多項式 $P_{mn}$ が存在します。 $S_m$が$S_n + Q_{mn} - P_{mn}$から$B'_m$の制限であれば、$B'_n$には$S_m \in X_m$と$|S_m(z) - S_n(z)| \leq \varepsilon$が入ります。これで証明は完了です。 \*

### 6. 一様連続写像の拡大

連続性 (章 I, § 8, no. 5、定理 1) による拡大の定理は、問題の写像が完全なハウスドルフのユニフォーム空間を着て値をとったとき、重要な加法を持ちます。

#### 命題 11 {#top-ii-s3-prop-11 .statement tag=0BF6}

*$A$ をトポロジカル空間 $X$ の密集部分集合とし、$f$ を $A$ の完全なハウスドルフ均一空間 $X'$ の写像とする。次に、$X$ の$x$ の近傍フィルタの$A$ のトレースの$f$ の下にある$x \in X$、像がコーシー フィルタである場合に限り、$f$ は連続性によって $X$ に拡張できます。 $X'$の基底。

これは、$X'$ が規則的 (§ 1, no. 2、命題 3) であり、$X'$ の収束フィルターがコーシー フィルターと同じであるため、連続性によって拡大の定理から続きます (引用箇所)。

$X$ も空間の場合、次の定理があります。

#### 定理 2 {#top-ii-s3-thm-2 .statement tag=0BF7}

*$f$ を、均一空間 $X$ の密な部分空間 $A$ 上で定義された写像とし、その値を完全なハウスドルフ均一空間 $X'$ とし、$f$ が均一連続であると仮定します。 $A$。この場合、$f$ は連続性によって $X$ 全体に拡張でき、拡張された写像 $\overline{f}$ は一様連続です*。

$\overline{f}$の存在は、命題3の明らか帰結とno. 1の11です。 $\overline{f}$が一様連続であることを示しましょう。 $V'$ を $X'$ の閉じた対称な取り巻きとし、$V$ を $X$ の取り巻きとし、$x$ と $y$ が $A$ にあり、$V$ に近いとき、$f(x)$ と$f(y)$は$V'$に近いです。 $V$ は、$A$ ($\S$ 2, no. 4, 命題 6) の側近 $W$ の $X \times X$ における終結であると仮定できます。 $(x, y) \in W$のときは$[ \bar{f}(x), \bar{f}(y) ] \in V'$です。 $\bar{f} \times \bar{f}$ は $X \times X$ で連続なので (章 I, $\S$ 4, no. 1, 命題 1)、$V'$ が閉じているので、$(x, y) \in V = \overline{W}$ のときも $[ \bar{f}(x), \bar{f}(y) ] \in V'$ になります。 (章 I、$\S$ 2、no. 1、定理 1)。

Q.E.D.

#### 系 {#top-ii-s3-n6-cor-1 .statement tag=0BF8}

*$X_1, X_2$ を 2 つの完全なハウスドルフ均一空間とし、$Y_1, Y_2$ を $X_1, X_2$ の密集部分空間とします。その後、$Y_1$ の同型 $f$ ごとに、$X_1$ の $Y_2$ 拡大するから同型が$X_2$ に続きます。

$f$ は $Y_1$ で一様連続であるため、(定理 2) 拡大するは一様連続写像 $\bar{f} : X_1 \to X_2$ になります。同様に、$f$ 拡大するの逆$g$ を一様連続写像 $\bar{g} : X_2 \to X_1$ にします。従って、写像 $\bar{g} \circ \bar{f}$ は、$X_1$ の連続写像であり、制限から $Y_1$ は恒等写像です。恒等式の拡大の原則 (章 I、$\S$ 8、no. 1、系 1 ～ 命題 2) により、$\bar{g} \circ \bar{f}$ は $X_1$ の恒等写像です。同様に、$\bar{f} \circ \bar{g}$ は $X_2$ の同一性写像です。その結果、(*集合理論*, R, $\S$ 2, no. 12) $\bar{f}^{-1}$ と $\bar{g}$ は全単射であり、互いに逆数です。それらも一様連続であるため、同型 ($\S$ 2、no. 1、命題 2) となります。

$f$ が $Y_2$ 上で $Y_1$ の *全単射* 一様連続写像である場合、その拡大は連続性により *単射でも全射でもない必要* (練習問題 3) であることに注意する必要があります。

### 7. ユニフォームの完成空間

#### 定理 3 {#top-ii-s3-thm-3 .statement tag=0BF9}

※$X$を制服空間とします。次に、完全なハウスドルフ均一空間 $\hat{X}$ と、以下の性質を持つ均一連続写像 $i : X \to \hat{X}$ が存在します。

(P) *$X$ の任意の一様連続写像 $f$ を完全なハウスドルフ均等空間 $Y$ にすると、$f = g \circ i$ のような一意連続写像 $g : \hat{X} \to Y$ が存在します。

*$(i_1, X_1)$ が完全なハウスドルフ均一空間 $X_1$ の他の対からなるであり、性質 (P) を持つ一様連続写像 $i_1 : X \to X_1$ である場合、一意の同型 $\varphi : \hat{X} \to X_1$ は $i_1 = \varphi \circ i$ となります。*

定理の最初の主張は、対 $(i, \hat{X})$ が普遍的な写像問題 (集合理論, 章) の解であることを意味します。 IV, , no. 1) ここで、$\Sigma$ 集合は完全なハウスドルフ均一空間、$\sigma$ 射は一様連続写像、$\alpha$ 写像は一様連続写像です。 $X$ は完全なハウスドルフのユニフォーム空間に。従って、対 $(i, \hat{X})$ から一意の同型までの一意性は、普遍的な写像問題の解の一般特性に従います (上記参照)。 対 $(i, \hat{X})$ の存在を証明することはまだ残っています

1) $\hat{X}$ の定義。 $\hat{X}$ を、$X$ 上の最小コーシー フィルター (no. 2) の集合とします。 $\hat{X}$には定義するのユニフォームを構造とさせていただきます。この目的のために、$V$ が $X$ の対称な取り巻きである場合、$\tilde{V}$ は、共通のに $V$ が小さい最小コーシー フィルターすべて対 $(\mathscr{K}, \mathfrak{Y})$ のうちの集合を表すものとします。 集合。 集合 $\tilde{V}$ 形が、$\hat{X}$ の制服構造の側近の基本系であることを示します。

(i) 各 $\mathscr{K} \in \hat{X}$ はコーシー フィルターであるため、$X$ のすべての対称な取り巻き $V$ に対して定義 $(\mathscr{K}, \mathscr{K}) \in \tilde{V}$ が得られます。従って、公理 $(U'_1)$ は満たされます。

(ii) $V$ と $V'$ が $X$ の 2 つの対称な取り巻きである場合、$W = V \cap V'$ は対称な取り巻きであり、$W$ が小さいすべての集合も $V$ が小さく、$V'$ が小さい。したがって $\tilde{W} \subset \tilde{V} \cap \tilde{V}'$ となり、これは $(B_1)$ を証明します。

(iii) 集合 $\tilde{V}$ は定義によって対称であるため、$(U''_1)$ が満たされます。

(iv) $X$ の対称的な取り巻き $V$ が与えられた場合、$W$ を $\tilde{V} \subset V$ となるような対称的な取り巻きとする。 $(\mathscr{K}, \mathfrak{Y}) \in \tilde{W}$ と $(\mathfrak{Y}, \mathfrak{B}) \in \tilde{W}$ のような 3 つの最小コーシー フィルター $\mathscr{K}, \mathfrak{Y}, \mathfrak{B}$ を考えます。次に、$M \in \mathscr{K} \cap \mathfrak{Y}$ と $N \in \mathfrak{Y} \cap \mathfrak{B}$ のような 2 つの $W$-小さい集合 $M, N$ があります。 $M$ と $N$ 属するから $\mathfrak{Y}$ なので、$M \cap N$ は空ではなく、したがって (no. 1, 命題 1) $M \cup N$ は $\tilde{W}$ が小さく、したがって $V$ が小さくなります。 $M \cup N$ 属するから $\mathscr{K}$、そして $\mathfrak{B}$ までは $\tilde{W} \subset \tilde{V}$ になります。したがって、$(U'''_1)$ は満たされます。

次に、ユニフォーム空間 $\hat{X}$ がハウスドルフであることを示します。 $\mathscr{K}, \mathfrak{Y}$ を、$X$ のすべての対称な取り囲み $V$ に対して $(\mathscr{K}, \mathfrak{Y}) \in \hat{X}$ となるような、$X$ 上の 2 つの最小コーシー フィルターとします。すぐに集合 $M \cup N$ が続きます。ここで、$M \in \mathscr{K}$ と $N \in \mathfrak{Y}$、形基底は、$\mathscr{K}$ と $\mathfrak{Y}$ よりも粗いフィルター $\mathfrak{B}$ です。 $\mathfrak{B}$ はコーシー フィルターです。$X$ のすべての対称取り巻き $V$ に対して、仮定によって $\mathscr{K}$ と $\mathfrak{Y}$ の両方に $V$-小さい集合 $P$ 所属が存在するからです。したがって、所属から $\mathfrak{B}$ になります。最小の Cauchy フィルターの定義により、$\mathscr{K} = \mathfrak{B} = \mathfrak{Y}$ が得られます。これは、$\hat{X}$ がハウスドルフであることを示しています。

2) $i$中定義; $X$のユニフォーム構造は、$\hat{X}$のユニフォームの$i$の下では逆像です。 $X$ の $x$ の各 $x \in X$ 近傍フィルター $\mathfrak{B}(x)$ が最小コーシー フィルター (no. 2、命題 5、系 1) であることがわかります。したがって、私たちは定義する $i(x) = \mathfrak{B}(x)$ となります。 $f = i \times i$ にしましょう。 $X$ の各対称取り巻き $V$ に対して $j^{-1}(\tilde{V}) \subset V \cup j^{-1}[(\tilde{V})^3]$ があることを示し、これで主張 (§ 2, no. 4) が証明されます。さて、$[i(x), i(y)] \in \tilde{V}$の場合、$x$と$y$のそれぞれ近傍である$V$-小さい集合$M$があり、したがって$(x, y) \in V$となります。逆に、$(x, y) \in V$の場合、集合 $V(x) \cup V(y)$は$V$-小さく、$x$と$y$のそれぞれの近傍であることがすぐにわかります。

3) $\hat{X}$ は完了し、$i(X)$ は$\hat{X}$ に密集します。 近傍 $\tilde{V}(\mathfrak{X})$ 点 $\mathfrak{X} \in X$ の $i(X)$ のトレースは、すべての $i(x)$ のうち集合です。

$$
(\mathfrak{X}, i(x)) \in \tilde{V}.
$$

この関係は、$X$に属するから$\mathfrak{X}$に$x$の$V$-小さい近傍が存在すること、つまり$x$が$V$-小さいものの内部点であることを意味します。 $\mathfrak{X}$中集合。 $M$ を、$\mathfrak{X}$ のすべての $V$-小さい集合の内部の和集合とします。次に、$M$ 属するから $\mathfrak{X}$ (no. 2、命題 5、系 4) となり、これまでの話から、$\tilde{V}(\mathfrak{X}) \cap i(X) = i(M)$ となります。私たちは結論する:

(i) $\tilde{V}(\mathfrak{X}) \cap i(X)$ は空ではないため、$i(X)$ は $\hat{X}$ 内で密です。
(ii) $i(X)$ 属するの $\tilde{V}(\mathfrak{X})$ から $X$ のフィルター 基底 $i(\mathfrak{X})$ へのトレース。したがって、このフィルター 基底は $\hat{X}$ から点 $\mathfrak{X}$ に収束します。

ここで、$\mathfrak{F}$ を $i(X)$ の Cauchy フィルターにします。次に、上記の 2) と no. 1 の命題 4 から、$\overline{i^1}(\mathfrak{F})$ は $X$ 上のコーシーフィルター $\mathfrak{G}$ の基底です。 $\mathfrak{X}$ を $\mathfrak{G}$ (no. 2, 命題 5) よりも粗い最小コーシーフィルターとします。この場合、$i(\mathfrak{X})$ は、$i(X)$ (no. 1、命題 3) のコーシーフィルター 基底であり、$\mathfrak{F} = i[\overline{i^1}(\mathfrak{F})]$ は、基底が $i(\mathfrak{X})$ であるフィルターよりもより細かいになります。後者は$\hat{X}$に収束するため、$\mathfrak{F}$も収束し、no. 4の命題9は$\hat{X}$が完了していることを示します。

4) 性質 (P) の検証。 $f$ を、$X$ の完全なハウスドルフ均等空間 $Y$ への一様連続写像とします。まず、$f = g_0 \circ i$ のような一様連続な写像 $g_0 : i(X) \to Y$ が存在することを示しましょう。 $f$ は連続なので、

$$
f(x) = \lim f(\mathfrak{B}(x)),
$$

したがって、$g_0(i(x)) = \lim f(\mathfrak{B}(x))$ とすると、$f = g_0 \circ i$ になります。したがって、$g_0$ が $i(X)$ で一様連続であることを示す必要があります。 $U$ を $Y$ の取り巻きとし、$V$ を $X$ の対称的な取り巻きとし、関係 $(x, x') \in V$ が $(f(x), f(x')) \in U$ を暗示するようにします。 2) で、関係 $(i(x), i(x')) \in \tilde{V}$ は $(x, x') \in V$ を暗黙的に示しているため、 も暗黙的に示されています。
$$
(g_0(i(x)), g_0(i(x'))) \in U,
$$
それは私たちの主張を証明します。

$\hat{X}$ (no. 6, 定理 2) への連続性により、$g$ を $g_0$ の拡大とします。次に$f = g \circ i$、$i(X)$が$\hat{X}$（章）に密集しているため、$g$が$\hat{X}$の$Y$満たす、この関係への一意の連続写像であることは明らかです。 I, § 8, no. 1、命題 2、系 1)。

Q.E.D.

#### 定義 4 {#top-ii-s3-def-4 .statement tag=0BFA}

*完全なハウスドルフ均一空間* $\hat{X}$ *定理 3 の証明で定義された * $X$、*および写像* $i : X \to \hat{X}$ * は * $X$ の標準写像と呼ばれます*ハウスドルフの完成に向けて。*

また、次の事実にも留意します。

#### 命題 12 {#top-ii-s3-prop-12 .statement tag=0BFB}

(i) *subspace* $i(X)$ *is dense in* $\hat{X}$.
(ii) *同値関係のグラフ* $i(x) = i(x')$ *は* $X$の側近の交点です。
(iii) *の均一構造* $X$ *は、* $i$ * の* $\hat{X}$ *[または部分空間* $i(X)$] の下の反転イメージです。
(iv) *の側近* $i(X)$ *は、* $X$の側近の* $i \times i$の下の画像であり、* $\hat{X} \times \hat{X}$ *の側近* $i(X)$ *の側近の基本的なシステムを形成します* $\hat{X}$。

(i) and (iii) have been proved in the course of 証明 of 定理 3; (iv) is 帰結 of (i) and (iii) by virtue of general results proved earlier (§ 2, no. 4, 注意 and 命題 6). 関係
$$
i(x) = i(x')
$$
means by 定義 that $x$ and $x'$ have the same 近傍 filter. But this implies, by 定義, that $(x, x') \in V$ for every entourage $V$ of $X$, and 逆 is obvious.

#### 系 {#top-ii-s3-n7-cor-1 .statement tag=0BFC}

*もし* $X$ * がハウスドルフのユニフォーム空間である場合、 標準写像* $i : X \to \hat{X}$ * は * $\hat{X}$ の密な部分空間の上に * $X$ の同型です。

$X$ がハウスドルフの場合、$\hat{X}$ は $X$ の *完成* であると言われ、一般的には $i$ によって $\hat{X}$ の密な部分集合を伴う *同一視する* $X$ になります。

#### 注意 {#top-ii-s3-n7-rem-1 .statement tag=0BFD}

この識別が行われる場合、X の最小のコーシー フィルターは、$\hat{X}$ の点の近傍フィルターの X のトレースにすぎません。これは、定理 3 の証明から続きます。

系から命題 12 は、ハウスドルフ ユニフォーム空間の完成を特徴づけます。

#### 命題 13 {#top-ii-s3-prop-13 .statement tag=0BFE}

*Y が完全なハウスドルフ一様空間であり、Y の密な部分空間 X である場合、正準注入 $X \to Y$ は Y への同型射影 $\hat{X}$ まで拡張されます。

X のすべての一様連続写像を完全なハウスドルフ一様空間 Z 拡大するに、定理 2 の no. 6 によって Y から Z への一様連続写像を一意に変換します。

#### 命題 14 {#top-ii-s3-prop-14 .statement tag=0BFF}

*X を完全なハウスドルフ均一空間、$\mathfrak{U}$ をその均一性、Z を X の密な部分空間とします。 $\mathfrak{U}'$ が $\mathfrak{U}$ よりも粗い X 上の均一性で、誘導するが Z 上の $\mathfrak{U}$ と同じ均一性である場合、$\mathfrak{U} = \mathfrak{U}'$ です。*

X' が集合 X を$\mathfrak{U}'$ の均一性で表すものとします。 標準写像 $X' \to \hat{X}'$ と恒等写像 $X \to X'$ の合成は、一様連続の写像 $\varphi : X \to \hat{X}'$ です。 Z は $\mathfrak{U}'$ によって誘導される一様構造のハウスドルフであるため、$\varphi$ の制限から Z への関係は、Z の仮定同型によって$\hat{X}'$ の密部分空間 $\varphi(Z)$ 上に生じます。 (no. 6、系から定理 2)、$\varphi$自体は$\hat{X}'$上のXの同型であるため、$X' = \hat{X}'$と$\mathfrak{U}' = \mathfrak{U}$になります。

#### 命題 15 {#top-ii-s3-prop-15 .statement tag=0BFG}

※XとX'を2つの均一空間とします。それぞれの一様連続写像 $f : X \to X'$ には、図式のような固有の一様連続写像 $\hat{f} : \hat{X} \to \hat{X}'$ があります。

$$
\begin{array}{ccc}
X & \xrightarrow{i'} & X' \\
i \downarrow & & \downarrow i' \\
\hat{X} & \xrightarrow{\hat{f}} & \hat{X}'
\end{array}
$$

は可換 (*) であり、$i : X \to \hat{X}$ と $i' : X' \to \hat{X}'$ は標準写像です。

定理を適用する 3 から写像 $i' \circ f : X \to \hat{X}'$。

#### 系 {#top-ii-s3-n7-cor-2 .statement tag=0BFH}

*$f : X \to X'$と$g : X' \to X''$が2つ一様に連続する写像と$h = g \circ f$の場合、$\hat{h} = \hat{g} \circ \hat{f}$です。

命題 15 の一意性の明らか帰結です。

(*)その他語、$i' \circ f = \hat{f} \circ i$では。

### 8. ハウスドルフのユニフォーム空間はユニフォーム空間に関連付けられています

#### 命題 16 {#top-ii-s3-prop-16 .statement tag=0BFI}

$X$ をハウスドルフ完成 $\hat{X}$ への $X$ の均一空間と $i$ 標準写像とする。 $X$ の各一様連続写像 $f$ をハウスドルフ均等空間 $Y$ に変換すると、$f = h \circ i$ のような固有の一様連続写像 $h : i(X) \to Y$ が存在します。

$\hat{Y}$ (no. 7、系 ～ 命題 12) の同一視する $Y$ を部分空間とすると、$f$ は$X$ の一様連続写像として考えることができます。 $\hat{Y}$。 定理 3 により、$f$ は形 $f = g \circ i$ になります。ここで、$g$ は $\hat{X}$ から $\hat{Y}$ への一様連続写像です。 $h$が$g$から$i(X)$の制限である場合、明らかに$f = h \circ i$、$h$写像$i(X)$が$Y$になります。 $h$ の一意性は些細なことです。

したがって、対 $(i, i(X))$ は汎用写像問題 (集合理論、章 IV, § 3, no. 1) の解であり、今回は$\Sigma$ セットをハウスドルフ統一とします。 空間、および $\sigma$ 射 (それぞれ $\alpha$ マッピング) は一様連続写像 (それぞれ $X$ のハウスドルフ均一空間への一様連続写像) です。

#### 定義 5 {#top-ii-s3-def-5 .statement tag=0BFJ}

定理 3 の証明で定義されたハウスドルフ制服空間 $i(X)$ は、$X$ に関連付けられたハウスドルフ制服空間と呼ばれます。

したがって、ハウスドルフの$X$ の完成は、$X$ に関連付けられたハウスドルフのユニフォーム空間の完成となります。

#### 系 {#top-ii-s3-n8-cor-1 .statement tag=0BFK}

$X, Y$ を 2 つの均一空間と、$X', Y'$ を関連するハウスドルフ空間とします。各均一連続写像 $f : X \to Y$ には、図式に対する一意の均一連続写像 $f' : X' \to Y'$ があります。

$$
\begin{array}{ccc}
X & \xrightarrow{f} & Y \\
i \downarrow & & \downarrow i' \\
X' & \xrightarrow{f'} & Y'
\end{array}
$$

は可換です。ここで、$i$ と $i'$ は標準写像です。

命題を適用する 16 から $i' \circ f : X \to Y'$。

ユニフォーム空間に関連付けられたハウスドルフ空間は、次の性質によっても特徴付けられる可能性があります。

#### 命題 17 {#top-ii-s3-prop-17 .statement tag=0BFL}

$X$ をユニフォーム空間、$i(X)$ に関連するハウスドルフ空間とし、$f$ をハウスドルフユニフォーム空間 $X'$ 上の $X$ の写像とします。 $X$ は、$X'$ の均一性の $f$ の下で逆像です。次に、写像 $g : i(X) \to X'$ となり、$f = g \circ i$ は同型になります。

命題 16 までに、$g$ は一様連続になります。また、$g$ は明らかに全射的であり、また単射的でもあります。なぜなら、関係 $f(x) = f(y)$ は、定義によって $X$ の側近全員に対して $(x, y)$ 属するを暗示し、したがって $i(x) = i(y)$ (no. 7, 命題) を意味するからです。 12)。 最後に、$X'$ の側近は、$X$ ($§ 2$、no. 4、注意) の側近の $f \times f$ の下にある像であるため、$i(X)$ の側近の $g \times g$ の下にも像があります。 (no. 7、命題12);したがって結果です。

#### 注意 {#top-ii-s3-n8-rem-1 .statement tag=0BFM}

$R$ を $X$ の同値関係 $i(x) = i(x')$ とします。 (no. 7、命題 12) $R$ のグラフ $C$ が $X$ のすべての取り巻きの共通部分であることがわかりました。 $X$ のすべての開集合 (したがってすべての閉集合) が $R$ に関して *飽和* していることは明らかです。トポロジーの逆像の定義を考慮すると、$i$ によって引き起こされる商空間 $X/R$ の $i(X)$ への正準全射は *同相同型* であると結論付けます。 したがって、$X$ に関連付けられたハウスドルフ空間は、$X/R$ と *qua* トポロジー 空間として識別できます。 標準写像 $i : X \to i(X)$ は開いたり閉じたり、さらには適切 (章 I、$§ 10$、no. 2、例) です。

$X'$ を、$X'$ のすべての側近の他の空間、$C'$ 共通部分、およびグラフが$C'$ である$R'$ 同値関係とします。 $f : X \to X'$ を *連続* 写像とします。 $f(x)$ の任意の近傍の $f$ の下の逆像は $x$ の近傍であるため、$C'(f(x))$ 含む $C(x)$ の $f$ の下の逆像は、 $f$ は、$R$ および $R'$ と *互換性* があり、誘導するは連続した写像 $X/R \to X'/R'$ (章 I、$§ 3$、no. 4、系と命題 6）。これにより、系から命題 16 が一般化されます。

### 9. 部分空間と積空間の完了

#### 命題 18 {#top-ii-s3-prop-18 .statement tag=0BFN}

*$X$を集合、$(Y_\lambda)_{\lambda \in L}$を均一空間のファミリーとし、各$\lambda \in L$に対して、$f_\lambda$を$X$の写像を$Y_\lambda$とします。 $X$ に最も粗い均一性 $U$ を持たせ、すべての $f_\lambda$ を均一に連続させます。この場合、$X$ のハウスドルフ完成 $\hat{X}$ の均一性は最も粗く、すべての写像 $\hat{f}_\lambda : \hat{X} \to \hat{Y}_\lambda$ ($\lambda \in L$) (no. 7, 命題 15) が均一に連続します。さらに、$j_\lambda$ が $Y_\lambda$ の $\hat{Y}_\lambda$ への標準写像である場合、および $g_\lambda = j_\lambda \circ f_\lambda$ の場合、$\hat{X}$ は、写像の下での $X$ の像の $\prod_{\lambda \in L} \hat{Y}_\lambda$ の閉包と同一視される可能性があります。 $x \to (g_\lambda(x))$.*

$X'$ (それぞれ $Y'_\lambda$) を、$X$ (それぞれ $Y_\lambda$) に関連付けられたハウスドルフユニフォーム空間とし、$f'_\lambda : X' \to Y'_\lambda$ を一様連続写像とし、図式を作成します。

$$
\begin{array}{ccc}
X & \xrightarrow{f_\lambda} & Y_\lambda \\
i \downarrow & & \downarrow j_\lambda \\
X' & \xrightarrow{f'_\lambda} & Y'_\lambda
\end{array}
$$

可換 (*i* は標準写像である)。

初期均一性 (§ 2, no. 3、命題 5) の推移性は、一方で $\mathfrak{U}$ が最も粗い均一性であり、写像 $j_\lambda \circ f_\lambda : X \to Y'_\lambda$ が一様に連続していること、他方で $\mathfrak{U}$ も以下の逆像であることを示しています。 集合 $X'$ の最も粗い均一性の $i$ $\mathfrak{U}'$ では、$f'_\lambda$ が均一に連続しています。ここで、$\mathfrak{U}'$ は *Hausdorff* です。つまり、$x_1, x_2$ が $X$ の 2 つの点で、各 $\lambda \in L$ に対して $j_\lambda(f_\lambda(x_1)) = j_\lambda(f_\lambda(x_2))$ である場合、$\mathfrak{U}$ のすべての側近には $(x_1, x_2)$ 属するが与えられるため、以下のようになります。 $i(x_1) = i(x_2)$。したがって、no. 8 の命題 17 は、$\mathfrak{U}'$ が $X$ に関連付けられたハウスドルフ空間 $X'$ の一様性であることを示しています。

そうなると、全単射 $x' \to (f'_\lambda(x'))$ は、積 $\prod_\lambda Y'_\lambda$ (§ 2, no. 6, 命題 8) の統一部分空間で $X$ を識別します。 $Y'_\lambda$ はハウスドルフであるため、各 $Y'_\lambda$ はその完成 $\hat{Y}_\lambda$ の密な部分空間で識別でき、したがって $\prod_\lambda Y'_\lambda$ は $\prod_\lambda \hat{Y}_\lambda$ (章 I, § 4, no. 3, 命題) の密な部分空間と識別できます。 7)。しかし、$\prod_\lambda \hat{Y}_\lambda$ はハウスドルフであり、完全です (no. 5、命題 10)。したがって、$\prod_\lambda \hat{Y}_\lambda$ の$X'$ の閉包 $\overline{X'}$ は、$X$ のハウスドルフ完了 $\hat{X}$ と識別できる完全なハウスドルフ部分空間 (no. 4, 命題 8) です。この識別の下では、写像 $\hat{f}_\lambda$ は因子 $\hat{Y}_\lambda$ 上で射影になり、命題が証明されます。

#### 系 1 {#top-ii-s3-prop-18-cor-1 .statement tag=0BFO}

*$X$ をユニフォーム空間とし、$i$ をハウスドルフ完成 $\hat{X}$ への $X$ の標準写像とする。 $A$ を $X$ と $j : A \to X$ 標準単射の部分空間とします。次に、$\hat{j} : \hat{A} \to \hat{X}$ は $\hat{A}$ の同型で、$\hat{X}$ の $i(A)$ の終点になります。*

#### 系 2 {#top-ii-s3-prop-18-cor-2 .statement tag=0BFP}

※$(Y_\lambda)_{\lambda \in L}$を制服空間の家族とします。したがって、積空間 $\prod_{\lambda \in L} Y_\lambda$ のハウスドルフ完全化は、積 $\prod_{\lambda \in L} \hat{Y}_\lambda$ と正準的に同型です。*

### 練習問題 {#top-ii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
