---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 10
section_title: Proper mappings
lang: ja
source: top-i-iv
book_pages: 97-107, 150-155
pdf_pages: 0103-0113, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: PROPER MAPPINGS
      page: 97
      pdf_page: 103
    - "no": 2
      title: CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES
      page: 101
      pdf_page: 107
    - "no": 3
      title: PROPER MAPPINGS INTO LOCALLY COMPACT SPACES
      page: 104
      pdf_page: 110
    - "no": 4
      title: QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES
      page: 105
      pdf_page: 111
statements: 30
exercises: 21
content_sha256: 8bbe35b0a201f78ee6398bc39d5a529c5f280c27d9a0c1351474d9f7024053a4
translated_from: content/en/top/I/10_s10_proper_mappings.md
translation_method: google
source_content_sha256: 5a1cc21b1eb39135e8b2b41344fcaf3ba40ecd043ec0192b77c8b672b5efb1a1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 195de15db0ee0a838c923aa3f68310306e9d526329bda7c7dd5a305644fa6013
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 10. 適切な写像

*この切断では、集合 $X$ の $\iota_X$ 恒等写像をそれ自体に表します。

### 1. 適切な写像

$f : X \to Y$ と $f' : X' \to Y'$ が 2 つの *連続閉* 写像である場合、$f$ が形 $\iota_X$ であっても、積 $f \times f' : X \times X' \to Y \times Y'$ は必ずしも閉写像であるとは限りません。

#### 例 {#top-i-s10-n1-exa-1 .statement tag=0BA1}

ハウスドルフ空間への定数写像はすべて閉じられます。しかし、$f$ は定数写像 $Q \to 0$ なので、$f \times \iota_Q$ は $Q^2$ の写像 $(x, y) \to (0, y)$ を $Q^2$ に変換するため、2 番目の射影であり、閉じていません (§ 4, no. 2、注意) 1)。

#### 定義 1 {#top-i-s10-def-1 .statement tag=0BA2}

*$f$ をトポロジカル空間 $X$ の写像をトポロジカル空間 $Y$ にします。 $f$ は、すべてのトポロジー 空間 $Z$ について、$f$ が連続で、写像 $f \times \iota_Z : X \times Z \to Y \times Z$ が閉じている場合、適切であると言われます。

no. 2と3で適切な写像の他の特徴付けを与えます。

定義 1 で空間 $Z$ が 1 つの点で構成されるとすると、次のようになります。

#### 命題 1 {#top-i-s10-prop-1 .statement tag=0BA3}

*適切な写像はすべて閉まっています。*

#### 命題 2 {#top-i-s10-prop-2 .statement tag=0BA4}

※$f : X \to Y$を連続した単射とします。したがって、次の 3 つの主張は同等です:*
a) $f$ が適切です。
b) $f$はお休みです。
c) $f$ は、$Y$ の閉じた部分集合に対する $X$ の同相写像です。

a) が b) を暗示していることを見てきました。 同値関係 $f(x) = f(x')$ は等式関係であるため、この関係に対する $X$ の商空間は $X$ と識別できます。したがって、b) は、§ 5, no. 2、命題という理由で c) を意味します。 3. 最後に、c) が満たされる場合、$f \times \iota_Z$ は、$Y \times Z$ の閉部分空間に対する $X \times Z$ の同相写像であり、したがって閉写像です。したがって、c) は a) を意味します。

#### 命題 3 {#top-i-s10-prop-3 .statement tag=0BA5}

※$f : X \to Y$を連続した写像とします。 $T$ が $Y$ のいずれかの部分集合である場合、$f_T$ は $\overline{f}^{-1}(T)$ の $f$ と一致する写像 $\overline{f}^{-1}(T) \to T$ を表します。
a) *$f$ が適切であれば、$f_T$ も適切です。*
b) *$(T(i))_{i \in I}$を$Y$の部分集合の族とし、その内部は$Y$をカバーするか、$Y$の局所的に有限の閉じたカバーであるとします。 写像 $f_{T(i)}$ がそれぞれ適切であれば、$f$ も適切です。*

$Z$ をトポロジー 空間とします。 $T$ が $Y$ のいずれかの部分集合である場合、次のようになります。
$$
f_T \times \iota_Z = (f \times \iota_Z)_{T \times Z};
$$
$f$ が適切であれば、$f \times \iota_Z$ は閉じており、したがって $(f \times \iota_Z)_{T \times Z}$ [§ 5, no. 1, 命題 2 a)] も同様であり、よって a) が証明されます。ここで、$(T(i))_{i \in I}$ が b) で述べた 2 つの条件のいずれかを満たしている場合、$Y \times Z$ のカバー $(T(i) \times Z)_{i \in I}$ は同じ性質を持ちます。 $f_{T(i)}$ が適切であれば、写像
$$
(f \times \iota_Z)_{T(i) \times Z}
$$
よって $f \times \iota_Z$ は休業です [§ 5, no. 1、命題 2 b)]。これで証明は完了です。

#### 命題 4 {#top-i-s10-prop-4 .statement tag=0BA6}

*$I$ を有限の集合とし、各 $i \in I$ に対して $f_i : X_i \to Y_i$ を連続の写像とします。 $X = \prod_{i \in I} X_i, \ Y = \prod_{i \in I} Y_i,$ と $f : X \to Y$* を積写像 $(x_i) \to (f_i(x_i))$ とします。次に:
a) *$f_i$ がそれぞれ適切であれば、$f$ も適切です。*
b) *$f$ が適切で、$X_i$ が空でない場合、それぞれの $f_i$ は適切です。*

(no. 2、定理 1、系 3 で、この命題拡大するが無限積になることがわかります。)

帰納法までに、$I = \{1, 2\}$の場合を考慮すれば十分です。
a) $f_1, f_2$ が適切であると仮定し、$Z$ を位相幾何学的な空間とします。 $f_1 \times f_2 \times \iota_Z$ は $\iota_{Y_1} \times f_2 \times \iota_Z$ の合成であり、
$$
f_1 \times \iota_{X_2} \times \iota_Z;
$$
これら 2 つの写像は仮定によって閉じられているため、$f_1 \times f_2 \times \iota_Z$ [§ 5, no. 1, 命題 1 a)] も同様であり、よって $f_1 \times f_2$ が適切です。

b) ここで、$f$ が適切であると仮定します。 $F$ を $X_2 \times Z$ の閉じた部分集合とし、$G$ を写像 $f_2 \times \iota_Z$ の下の $Y_2 \times Z$ の $F$ の像とします。すると、$f_1 \times f_2 \times \iota_Z$の下の$Y_1 \times Y_2 \times Z$の$X_1 \times F$の像は$f_1(X_1) \times G$になります。 仮定までに、ここは$Y_1 \times Y_2 \times Z$に閉鎖されます。 $X_1 \neq \emptyset$ の場合、$f_1(X_1)$ は空ではありません。これは、$G$ が $Y_2 \times Z$ (§ 4, no. 3、系 ～ 命題 7) で閉じられていることを意味します。したがって、$f_2$ が適切です。同様に、$X_2 \neq \emptyset$ の場合は $f_1$ が適切です。

#### 命題 5 {#top-i-s10-prop-5 .statement tag=0BA7}

*$f : X \to X'$と$g : X' \to X''$を2つの連続する写像とします。*
a) *$f$と$g$が適切であれば、$g \circ f$が適切です。*
b) *$g \circ f$ が適切で、$f$ が全射であれば、$g$ が適切です。*
c) *$g \circ f$ が適切で、$g$ が単射であれば、$f$ が適切です。*
d) *$g \circ f$ が適切で、$X'$ がハウスドルフである場合、$f$ が適切です。*

$Z$ をトポロジー 空間とします。私たちは持っています
$$
(g \circ f) \times \iota_Z = (g \times \iota_Z) \circ (f \times \iota_Z);
$$
$f$ と $g$ が適切な場合、$f \times \iota_Z$ と $g \times \iota_Z$ は閉じられます。したがって、[§ 5, no. 1, 命題 1 a)] $(g \circ f) \times \iota_Z$ は閉まっています。これは a) を証明します。 b) の証明 [それぞれc)] は、部分 b) [それぞれを使用して、同じ線に沿って実行されます。 c)] の命題 1 の § 5, no. 1 を計算し、$f$ が全射である場合 (または $g$ が単射である場合)、$f \times \iota_Z$ は全射である (または $g \times \iota_Z$ が単射である) ことに注意してください。最後に、d) を証明するために、可換図式を考えます。

$$
\begin{array}{ccc}
X & \overset{\varphi}{\to} & X \times X' \\
f \downarrow & & \downarrow (g \circ f) \times \iota_{X'} \\
X' & \underset{\psi}{\to} & X'' \times X'
\end{array}
$$

ここで、$\varphi(x) = (x, f(x))$ と $\psi(x') = (g(x'), x')$ です。 写像 $\varphi$ (それぞれ $\psi$) は、$f$ のグラフ (それぞれ $g$ のグラフの反映) への $X$ (それぞれ $X'$) の同相写像です (§ 4, no. 1, 命題 1, 系 2）。さらに、$X'$はハウスドルフなので、$f$のグラフ$\varphi(X)$は$X \times X'$(§ 8, no. 1, 命題 2, 系 2)で閉じられます。したがって、(命題 2) $\varphi$ が適切です。一方、命題 4 は、$(g \circ f) \times i_{X'}$ が適切であることを示しています。上記a)と図式(1)の可換性より、$\psi \circ f$が妥当です。しかし、$\psi$ は単射なので、上記の c) により $f$ が適切です。

#### 注意 {#top-i-s10-n1-rem-1 .statement tag=0BA8}

$X'$ がハウスドルフでない場合、$g \circ f$ が適切で、$f$ が適切ではないということが起こります。たとえば、$X$ と $X''$ は 1 つの点で構成され、$X'$ は 2 つの点で構成され、最も粗いのは位相です。

#### 系 1 {#top-i-s10-prop-5-cor-1 .statement tag=0BA9}

*$f : X \to Y$ がプロパー 写像の場合、$f$ の制限からクローズド部分集合 $X$ の $F$ は、$F$ のプロパー 写像から $Y$ になります。

この場合、制限は合成 $f \circ j$ で、$j : F \to X$ は標準単射であり、命題 2 によって適切になります。

#### 系 2 {#top-i-s10-prop-5-cor-2 .statement tag=0BAA}

*$f : X \to Y$ を適切な写像とし、$X$ はハウスドルフです。次に、$Y$ の部分空間 $f(X)$ はハウスドルフです。*

命題 5 c) の理由により、$f(X) = Y$ の場合のみを考慮する必要があります。 このとき、$Y \times Y$ の対角線は、$X$ の対角線の$f \times f$ の下にある像であり、閉じられています (§ 8, no. 1、命題 1)。 $f \times f$ は適切です (提案 4)。したがって、$Y \times Y$ の対角線は閉じており (命題 1)、したがって $Y$ はハウスドルフです (§ 8, no. 1、命題 1)。

#### 系 3 {#top-i-s10-prop-5-cor-3 .statement tag=0BAB}

*$I$ を有限の集合とし、各 $i \in I$ に対して、$f_i : X \to Y_i$ を適切な写像とします。 $X$ がハウスドルフである場合、$X$ の $\prod_{i \in I} Y_i$ へのマッピング $x \mapsto (f_i(x))$ は適切です。*

This mapping is the composition of the product mapping $(x_i) \mapsto (f_i(x_i))$ of $X^I$ into $\prod_i Y_i$ and the diagonal mapping of $X$ into $X^I$; since the latter is proper (by Proposition 2 and § 8, no. 1, Proposition 1) the conclusion follows from Proposition 4 and Proposition 5 a).

#### 系 4 {#top-i-s10-prop-5-cor-4 .statement tag=0BAC}

*$X$ と $Y$ を 2 つのトポロジー 空間、 $f : X \to Y$ を連続写像、 $R$ 同値関係 $f(x) = f(y)$ を $X$ にするとします、そして*
$$
X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y
$$
*$f$ の正準分解.* *したがって、$f$ が適切であるためには、$p$ が適切であり、$h$ が同型写像であり、$f(X)$ が $Y$ の閉じた部分集合であることが必要かつ十分です。

命題 5 a) と命題 2 により、条件は十分です。逆に、$f$ が適切であれば、$f$ は閉じられます。したがって、$f(X)$ は $Y$ で閉じられ、$h$ は同相写像 ($§ 5$, no. 2, 命題 3) です。また、$h \circ p$ は命題 5 c) によって適切です。したがって、命題 5 a) によれば、$p = h^{-1} \circ (h \circ p)$ は適切です。

### 2. コンパクト性の特性による適切な写像の特徴付け

この小節では、単一の点とその固有の位相の $P$ 空間からなるで表します。

#### 補題 1 {#top-i-s10-lem-1 .statement tag=0BAD}

*定数写像 $X \to P$ が適切となるように、$X$ をトポロジー 空間とします。そうすると、$X$ は準コンパクトになります。*

(この性質が準コンパクト空間を特徴付けることは、少し後で (定理 1, 系 1) わかります。)

$X$ が空でない場合に限定することもできます。 $\mathfrak{F}$ を $X$ のフィルターとし、$X' = X \cup \{ \omega \}$ を $\mathfrak{F}$ ($§ 6$、no. 5、例) に関連付けられたトポロジカル空間とします。 $\Delta$ を、$x \in X$ のすべての $(x, x)$ からなる $X \times X'$ の部分集合とし、$F = \overline{\Delta}$ を $X \times X'$ の $\Delta$ の閉包とします。 $X$ の仮説を考慮すると、射影 $X \times X' \to X'$ の下での $F$ の画像は $X'$ で閉じられます。この画像には $X$ が含まれているため、$X$ の終端にある $\omega$ が含まれています。言い換えれば、$(x, \omega) \in F$ となるような点 $x \in X$ が存在します。 $X \times X'$の位相の定義により、これは、$X$の$x$の各近傍$V$と各$M \in \mathfrak{F}$に対して、$(V \times M) \cap \Delta \neq \emptyset$、つまり$V \cap M \neq \emptyset$があるため、$x$は次のようになります。フィルター $\mathfrak{F}$ のクラスター 点なので、$X$ は準コンパクトです。

Q.E.D.

#### 定理 1 {#top-i-s10-thm-1 .statement tag=0BAE}

※$f : X \to Y$を連続した写像とします。したがって、次の 4 つの主張は同等です。

a) $f$ が適切です。
b) $f$ は閉じており、$\overline{f}^{-1}(y)$ は各 $y \in Y$ に対して準コンパクトです。
c) *$\mathfrak{F}$が$X$のフィルターであり、$y \in Y$が$f(\mathfrak{F})$のクラスター点である場合、$f(x) = y$のような$\mathfrak{F}$のクラスター点$x$が存在します。
d) *$\mathfrak{U}$ が $X$ の限外濾過器であり、$y \in Y$ が限外濾過器の極限点基底 $f(\mathfrak{U})$ である場合、極限点 $x$ が存在します。 $\mathfrak{U}$ は $f(x) = y$ となります。*

a) $\Longrightarrow$ b): $f$ が適切な場合、$f$ は閉じられ (no. 1、命題 1)、それぞれの $y \in Y$ 写像 $f_{|y|} : \overline{f}^{-1}(y) \to \{ y \}$ は適切です [no. 1、命題 3a)]。 補題 1 により、これは $\overline{f}^{-1}(y)$ が準コンパクトであることを意味します。

b) $\Longrightarrow$ c): c) の仮説 $\mathfrak{F}$ と $y$ 満たすを仮定します。 $\mathfrak{B}$ を、$\mathfrak{F}$ の集合のクロージャーによって形成される $X$ 上のフィルター 基底とします。 $f$が定休日のため、$M \in \mathfrak{F}$(§ 5, no. 4、命題9)ごとに$f(\overline{M}) = f(M)$がございます。これは、集合 $\overline{M} \cap \overline{f}^{-1}(y)$ がすべての $M \in \mathfrak{F}$ に対して空ではないことを示しており、したがって形 $\overline{f}^{-1}(y)$ のフィルター 基底の元は $\overline{f}^{-1}(y)$ の部分集合で閉じられています。 $\overline{f}^{-1}(y)$ は準コンパクトなので、$M$ が $\mathfrak{F}$ を通るので、すべての集合 $M$ に属するを加えた点 $x \in \overline{f}^{-1}(y)$ があります。したがって、$f(x) = y$ と $x$ は、$\mathfrak{F}$ のクラスター 点です。

c) $\Longrightarrow$ d): 些細なこと。

d) $\Longrightarrow$ a): まず、d) が満たされる場合、$f$ は閉じた写像であることを示します。 $A$ を $X$ の空ではない閉じた部分集合とし、$\mathfrak{F}$ を $X$ の部分集合 (含む $A$) のフィルターとします。 すると、$A$ は$\mathfrak{F}$ のクラスター点の集合になります。 $B$ を、$Y$ 上のフィルター 基底 $f(\mathfrak{F})$ のクラスター 点の集合とします。 $B$ は閉じており、明らかに含む $f(A)$; $B = f(A)$ を示します。 $y \in B$ と $\mathfrak{B}$ を $Y$ の $y$ の近傍フィルターとします。次に仮説により、$\mathfrak{W} = \overline{f}^{-1}(\mathfrak{B})$ のすべてのセットは $\mathfrak{F}$ のすべてのセットと一致します。したがって、$\mathfrak{W}$ は$X$ のフィルターベースであり、$X$ には限外フィルター $U$ があり、これは $\mathfrak{F}$ およびベースが $\mathfrak{W}$ であるフィルターよりも細かいです (§ 6, no. 2、命題 1、系 1 および no. 4、定理 1)。 基底が $f(U)$ である限外濾過器は、$\mathfrak{B}$ よりもより細かいであるため、$y$ に収束します。 d) により、$f(x) = y$ と $U$ が $x$ に収束するような点 $x \in X$ が存在します。 $U$ は $\mathfrak{F}$ よりもより細かいであるため、$x$ は $\mathfrak{F}$ のクラスター 点です。したがって$x \in A$です。 これは、$B = f(A)$、つまり $f$ が閉じていることを示しています。

証明を完了するには、すべてのトポロジカル空間 $Z$ に対して $f \times \iota_Z$ が閉じていることを示す必要があります。証明されたことから、$f$ が条件 d) を満たす場合、$f \times \iota_Z$ も満たすことを示すだけで十分です。これは、次の一般的な補題の帰結です。

#### 補題 2 {#top-i-s10-lem-2 .statement tag=0BAF}

** $(f_i)_{i \in I}$ * が連続する写像* $f_i : X_i \to Y_i$ の族で、 *それぞれが定理 1 の条件 d)* を満たす場合、 *その後積写像*
$$
f : (x_i) \to (f_i(x_i))
$$
*d) も満たします。

$U$ を $X = \prod_i X_i$ の限外フィルターとし、$y = (y_i)$ を $f(U)$ が $y$ に収束するような $Y = \prod_i Y_i$ の点とします。これは、各限外フィルター 基底 $\operatorname{pr}_i(f(U)) = f_i(\operatorname{pr}_i(U))$ が $y_i$ (§ 7, no. 6、命題 10、系 1) に収束することを意味します。 条件 d) により、$i \in I$ ごとに $f_i(x_i) = y_i$ と $\operatorname{pr}_i(U)$ が $x_i$ に収束するような $x_i \in X_i$ が存在します。しかしその後、$U$ は $x = (x_i)$ (*上記引用*) に収束し、$f(x) = y$ になります。これで、補題 2 の証明が完了し、したがって定理 1 が完了します。

#### 系 1 {#top-i-s10-lem-2-cor-1 .statement tag=0BAG}

*トポロジカル空間* $X$ *は、写像* $X \to P$ *が適切*である場合に限り、準コンパクトです。

a) $\iff$ b) を$X \to P$ に適用します。

#### 系 2 {#top-i-s10-lem-2-cor-2 .statement tag=0BAH}

*準コンパクト空間* $X$ *ハウスドルフ空間* $Y$ * の連続写像* $f$ *は適切です*。

合成 $X \xrightarrow{f} Y \to P$ は系 1 によって適切です。したがって、no. 1, 命題 5 d) により、$f$ は適切です。あるいは、§ 9, no. 4、定理 2、系 2 を使用して、定理 1 の基準 b) を適用することもできます。

#### 系 3 {#top-i-s10-lem-2-cor-3 .statement tag=0BAI}

*もし* $(f_i)$ *が適切な写像のファミリーである場合、積写像* $(x_i) \to (f_i(x_i))$ *は適切*です。

定理 1 から見ると、これはちょうど上の補題 2 です。

この系を写像 $X_i \to P$ の族に適用し、系 1 を使用すると、ティコノフの定理 (§ 9、no 5、定理 3) が得られます。

#### 系 4 {#top-i-s10-lem-2-cor-4 .statement tag=0BAJ}

* $X$ * をハウスドルフ空間とし、* $f_i : X \to Y_i$ * を適切な写像の家族とします。次に、写像* $f : x \to (f_i(x))$ *of* $X$ *into* $\prod_i Y_i$ *が適切です*。

証明 is the same as in the case of a finite family (no. 1, 命題 5, 系 3), using 系 3 above and the fact that the diagonal of $X^1$ is closed (§ 8, no. 1, 命題 1).

#### 系 5 {#top-i-s10-lem-2-cor-5 .statement tag=0BAK}

** $X$ * が任意の準コンパクト空間であり、* $Y$ * が任意のトポロジカル空間である場合、射影* $\mathrm{pr}_2 : X \times Y \to Y$ *は適切*です。

なぜなら、$X \to P$と$\iota_Y$の積を使って、$P \times Y$と$\mathrm{pr}_2$を組み合わせて同一視する$Y$をすることができ、どちらも正しい写像だからです。

#### 例 {#top-i-s10-n2-exa-1 .statement tag=0BAL}

$X$ を集合とし、$f : X \to X'$ をトポロジー 空間 $X'$ 上の $X$ の写像とします。 $X'$ の位相の $f$ の下で $X$ を逆像とトポロジします。 Then $f$ is *proper*, for $f$ is closed (§ 5, no. 1, 例 3) and 逆像 of 点 of $X'$ is 部分空間 of $X$ whose 位相 is the最も粗い位相なので、準コンパクトです。

#### 注意 {#top-i-s10-n2-rem-1 .statement tag=0BAM}

$Y$ が *Hausdorff* の場合、定理 1 の条件 d) は次と同等です。

d') *もし* $\mathfrak{U}$ *がオンの限外フィルター* $X$ *そのような* $f(\mathfrak{U})$ *が収束フィルター基底である場合、* $\mathfrak{U}$ *は収束*です。

なぜなら、$\mathfrak{U}$ が $x$ に収束し、$f(\mathfrak{U})$ が $y$ に収束する場合、$Y$ の極限の一意性と $f$ の連続性は、$y = f(x)$ がなければならないことを示しています。同様に、Y がハウスドルフである場合、定理 1 の条件 c) は次と同等です。

c') *$\mathfrak{F}$ が $f(\mathfrak{F})$ にクラスター 点があるような、X のフィルターである場合、$\mathfrak{F}$ にはクラスター 点があります。*

c) $\Longrightarrow$ c') $\Longrightarrow$ d') $\Longrightarrow$ d) $\Longrightarrow$ c) の場合。

一方、Y がハウスドルフでない場合、d') はもはや d) を意味しません。たとえば、X を 1 つの点で構成し、Y を 2 つの点で構成し、最も粗い位相とします。

#### 命題 6 {#top-i-s10-prop-6 .statement tag=0BAN}

*$f : X \to Y$ を適切な写像とし、K を Y の準コンパクト部分集合とします。その場合、$\overline{f}^{-1}(K)$ は準コンパクトです。*

no. 1 の命題 3 までに、写像 $f_K : \overline{f}^{-1}(K) \to K$ が適切です。 $K \to P$ は正規の写像 (定理 1, 系 1) であるため、no. 1, 命題 5 a) から、合成 $\overline{f}^{-1}(K) \xrightarrow{f_K} K \to P$ は正規であり、よって $\overline{f}^{-1}(K)$ は準コンパクトであることがわかります。 定理 1、系 1。

### 3. 適切な写像を局所的にコンパクトな空間に変換

#### 命題 7 {#top-i-s10-prop-7 .statement tag=0BAO}

* f を局所コンパクト空間 Y へのハウスドルフ空間 X の連続写像とします。すると、Y のすべてのコンパクト部分集合の f の下の逆像がコンパクトである場合にのみ、f が適切になります。さらに、f が適切であれば、X は局所的にコンパクトになります。*

f が適切で、K が Y のコンパクトな部分集合である場合、$\overline{f}^{-1}(K)$ は no. 2 の命題 6 によってコンパクトになります。逆に、この条件が満たされる場合、$(\mathbf{U}_\alpha)$は比較的コンパクトに開いた集合でYを覆うものとします。次に、集合 $\overline{f}^{-1}(\overline{\mathbf{U}}_\alpha)$ は X でコンパクトになり、その内部は X をカバーします。 X はハウスドルフであるため、これは X が局所的にコンパクトであることを示しています。さらに、写像 $f_{\overline{\mathbf{U}}_\alpha} : \overline{f}^{-1}(\alpha \overline{\mathbf{U}}) \to \overline{\mathbf{U}}_\alpha$ はそれぞれ固有 (no. 2, 定理 1, 系 2) であるため、f は no. 1 の命題 3 b) によって固有です。

#### 系 {#top-i-s10-n3-cor-1 .statement tag=0BAP}

*X、X' を 2 つの局所コンパクト空間とし、Y (それぞれ Y') を無限遠で隣接する点 $\omega$ (それぞれ $\omega'$) から X (それぞれ X') で得られるコンパクト空間とします。 (§ 9, no. 8)。 したがって、連続写像 $f : X \to X'$ は、その拡大 $\overline{f} : Y \to Y'$ ($\overline{f}(\omega) = \omega'$ など) が連続である場合にのみ適切です。*

命題 7 によれば、X' の各コンパクトサブセット K' について、$\overline{f}^{-1}(X' - K') = X - \overline{f}^{-1}(K')$ が X のコンパクトサブセットの補数である場合に限り、f は適切です。 Y (または Y') の $\omega$ (または $\omega'$) の近傍の定義によれば、これは、$\overline{f}$ が $\omega$ で連続している場合にのみ当てはまります。

### 4. コンパクト空間とローカル コンパクト空間の商空間

#### 命題 8 {#top-i-s10-prop-8 .statement tag=0BAQ}

$X$ を、$X \times X$, $f$ 標準写像 $X \to X/R$ の $X$, $C$ の $R$ のグラフをコンパクト空間, $R$ 同値関係とします。したがって、次の条件は同等です。

a) $C$ は $X \times X$ でクローズされます。

b) $R$ は閉まっています。

c) $f$ が適切です。

d) $X/R$ はハウスドルフです。

さらに、これら条件が満たされれば、$X/R$はコンパクトになります。

$R$ は、$f$ が閉じている場合にのみ閉じられます。したがって、b) は、定理 1b) の no. 2 の理由により c) を意味します。 c) は、d) が no. 1、命題 5、系 2 の特定のケースであることを意味します。 d) は、a) が任意のトポロジカル空間 $X$ ($\S$ 8, no. 3, 命題 8) について意味します。 a) が b) を意味することを示すことはまだ残っています。 $F$ が $X$ の閉じた部分集合である場合、その彩度 ($R$ に関して) は $\mathrm{pr}_2(C \cap (F \times X))$ です。 仮定により、$C \cap (F \times X)$ はコンパクトな空間 $X \times X$ の閉じた部分集合であるため、コンパクトです ($\S$ 9、no. 3、命題 3)。結果は、$\mathrm{pr}_2$ ($\S$ 9、no. 4、定理 2、系 2) の連続性から得られます。

最後に、$X/R$ がハウスドルフである場合、コンパクトであることが明らかです ($\S$ 9、no. 4、定理 2)。

#### 命題 9 {#top-i-s10-prop-9 .statement tag=0BAR}

$X$ を、$X \times X$, $f$ 標準写像 $X \to X/R$ の $R$ のグラフを、$X$, $C$ で局所的に圧縮した空間, $R$ 同値関係とします。 点を無限遠$\omega$から$X$に隣接させて得られるコンパクト空間を$X'$とし、グラフが$C' = C \cup \{(\omega, \omega)\}$である$X'$上の同値関係を$R'$とします。したがって、次の条件は同等です。

a) $f$ が適切です。

b) $R$ に対する$X$ の各コンパクト部分集合の彩度はコンパクトです。

c) $R'$ は閉まっています。

d) $\mathrm{pr}_2$ ～ $C$ の制限が適切です。

e) $R$ は閉じており、$R$ に対して同値類はコンパクトです。

さらに、これら条件が満たされれば、$X/R$は局所的にコンパクトになります。

a) $\Longrightarrow$ b): $X/R = f(X)$ と $f$ が適切であるため、$X/R$ はハウスドルフ (no. 1, 命題 5, 系 2);したがって、すべてのコンパクトの $f$ の下の像 、$X$ の部分集合 $K$ はコンパクトです ($\S$ 9、no. 4、定理 2、系 1)。

$R$ に対する $K$ の彩度は $\overline{f}^{-1}(f(K))$ であるため、no. 2、命題 6 だけコンパクトになります。

b) $\Longrightarrow$ c) : $F'$ が $X'$ で閉じられ、含む $\omega$ ではない場合、$F'$ は $X$ の圧縮部分集合です。したがって、$R'$ に関するその彩度は、$R$ に関する彩度と同じですが、コンパクトであり、*なおさら* は $X'$ で閉じられます。 $\omega \in F'$ で、$F = F' \cap X = F' - \{ \omega \}$ の場合、$R'$ に対する $F'$ の彩度は、$\{ \omega \}$ の和集合であり、$R$ に対する$F$ の彩度 $H$ です。したがって、$H$ が $X$ で *closed* であることを示すだけで十分です (つまり、 $R$ が *closed* 関係である)。このためには、$K$ が $X$ の任意のコンパクト部分集合である場合、$H \cap K$ はコンパクト ($§ 9$、no. 7、命題 11) であることを示すだけで十分です。ここで、$R$に対する$K$の彩度$L$は仮定だけコンパクトになり、$H \cap L$は$F \cap L$の彩度であり、これもコンパクトです。 *なおさら* $H \cap K = (H \cap L) \cap K$はコンパクトです。

c) $\Longrightarrow$ d) : $X'$ は通常 ($§ 9$、no. 2、系 ～ 命題 1) であるため、$C'$ は $X' \times X'$ ($§ 8$、no. 6、 命題 14) なのでコンパクトです。したがって、$C'$ は $C$ ($§ 9$、no. 8、定理 4) を 1 点圧縮したものになります。 $pr_2 : X' \times X' \to X'$の制限～$C'$は$\omega$で連続なので、結果はno. 3、系～命題と続きます。

d) $\Longrightarrow$ e) : $F$ が $X$ の閉じた部分集合である場合、$C \cap (F \times X)$ は $C$、よってで閉じられ、$R$ に対する$F$ の彩度は以下に等しい。 $pr_2(C \cap (F \times X))$、$X$ (no. 1、命題 1) で閉店します。また、$x \in X$ mod $R$ の同値類は、$pr_2$ から $C$ の制限の下で $\{ x \}$ の逆像と同型であるため、コンパクトです [no. 2, 定理 1 b)]。

e) $\Longrightarrow$ a) : $R$ が閉じている場合、定義までに $f$ が閉じられ、各 $z \in X/R$ に対して、$f^{-1}(z)$ は同値類 mod $R$ であるため、コンパクトになります。したがって、no. 2 の定理 1 b) により、$f$ は適切です。

最後に、$X/R$ が局所的にコンパクトであることを証明する必要があります。 $X'/R'$ は c) と命題 8 によってコンパクトになります。 関係 $R$ は、$X$ に $R'$ によって誘発されたものです。 $X$は$X'$でオープンし、$R'$に関して飽和しています。したがって、$X/R$ は、標準写像 $f' : X' \to X'/R'$ ($§ 3$, no. 6, 命題 10, 系 1) の下で、$X$ の像 $f'(X)$ と同相です。現在、$f'(X)$ は $X'/R'$ にオープンしているため、ローカルでは $X'/R'$ の部分空間がコンパクトになります。

Q.E.D.

#### 系 {#top-i-s10-n4-cor-1 .statement tag=0BAS}

*$X$ をハウスドルフ空間、$Y$ をトポロジカル空間、$f : X \to Y$ を固有の写像とします。次に、$X$ がコンパクト (局所的にコンパクト) であるためには、$f(X)$ がコンパクト (局所的にコンパクト) であることが必要かつ十分であり、$Y$ がコンパクト (局所的にコンパクト) であるだけで十分です。*

f_z : X \to f(X) は適切です [no. 1, 命題 3 a)] no. 2 の命題 6 と no. 3 の命題 7 の理由により、X はコンパクト (それぞれ局所的にコンパクト) であることがわかります。最後に、Y がコンパクト (つまり局所的にコンパクト) であれば、Y で閉じられた f(X) も同様です (no. 1, 命題 1 および , no. 7, 命題 13)

#### 注意 {#top-i-s10-n4-rem-1 .statement tag=0BAT}

X が局所的にコンパクトであるがコンパクトではない場合、X 上の閉じた同値関係 R はハウスドルフ (章 IX, § 4, 練習問題 14) である必要はありません。そして、たとえ R がハウスドルフであっても、X/R は局所的にコンパクトである必要はありません (練習問題 17)。ただし、次の基準があります。

#### 命題 10 {#top-i-s10-prop-10 .statement tag=0BAU}

X を局所コンパクト空間、R を X 上の開いたハウスドルフ同値関係とし、 f​​ : X \to X/R を標準写像とします。この場合、X/R は局所的にコンパクトであり、K' が X/R のコンパクト部分集合である場合、f(K) = K' となるような X のコンパクト部分集合 K が存在します。

最初の主張は、X の各 x \ がコンパクト近傍 V を持ち、f(V) が f(x) (§ 5, no. 3、命題 5 および § 9, no. 4) のコンパクト近傍であるという事実の帰結です。 定理 2、系 1)。 K' の各 y \について、V(y) を X の f^{-1}(y) の一部の点の圧縮近傍とするため、f(V(y)) は y の圧縮近傍になります。 f(V(y_i)) が K' をカバーするような、K' の点 y_i \in の有限数があります。 K_1 を X のコンパクト集合 $\bigcup_i V(y_i)$ とします。 K' \部分集合 f(K_1);したがって、 K = K_1 \cap f^{-1}(K') はコンパクト (K_1 で閉じているため) であり、 f(K) = K' です。

### 練習問題 {#top-i-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
