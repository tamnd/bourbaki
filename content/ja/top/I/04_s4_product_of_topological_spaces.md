---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 4
section_title: Product of topological spaces
lang: ja
source: top-i-iv
book_pages: 43-50, 125-127
pdf_pages: 0049-0056, 0131-0133
extraction: ocr
subsections:
    - "no": 1
      title: PRODUCT SPACES
      page: 43
      pdf_page: 49
    - "no": 2
      title: SECTION OF AN OPEN SET; SECTION OF A CLOSED SET; PROJECTION OF AN OPEN SET. PARTIAL CONTINUITY
      page: 46
      pdf_page: 52
    - "no": 3
      title: CLOSURE IN A PRODUCT
      page: 47
      pdf_page: 53
    - "no": 4
      title: INVERSE LIMITS OF TOPOLOGICAL SPACES
      page: 48
      pdf_page: 54
statements: 21
exercises: 10
content_sha256: 5d7057a178c565aeb1bc6b323d6600405f5e9c26dbb0d307cd009229705cb569
translated_from: content/en/top/I/04_s4_product_of_topological_spaces.md
translation_method: google
source_content_sha256: ca28b3bed17cb5f1025ef827c13e6c41b2a4a8dcca42f1668734a8ba2d7c3fa4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 372373278a014d79e3a935c2018f905e6123bb3fa423ee1156a4a1da4ea62861
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. トポロジカル空間の積

### 1. 積空間

#### 定義 1 {#top-i-s4-def-1 .statement tag=0B27}

*位相空間の族 $(X_i)_{i \in I}$ が与えられると、この族の積空間は、$X_i$ のトポロジーの積であるトポロジーを持つ積集合 $X = \prod_{i \in I} X_i$ になります (§ 2, no. 3、例 3)。 空間 $X_i (i \in I)$ は、X の因子と呼ばれます。*

§ 2, no. 3、命題 4 により、$X$ の積トポロジーは、$\overline{\mathrm{pr}}_i^{-1}(U_i)$ の形式の集合の有限交差の集合 $\mathfrak{B}$ をベースとし、$U_i$ は $X_i$ で開いています。これらのセットは積 $\prod_{i \in I} A_i$ で、有限数を除くすべてのインデックスに対して $i \in I$ と $A_i = X_i$ のそれぞれに対して $A_i$ が $X_i$ でオープンになります。 これらの集合を初級集合と呼びます。

$\mathfrak{B}_i$ が $X_i$ の位相の基底 (各 $i \in I$ について) である場合、基本集合 $\prod_{i \in I} A_i$ は、添字 $i$ ごとに $A_i \neq X_i$ となる $A_i \in \mathfrak{B}_i$ であることは明らかです。 形他の基底の積位相。 したがって、与えられた点 $x \in X$ を含むこのタイプの基本集合は、$x$ ($§ 1$、no. 3、命題 3) の近傍の基本システムを形成します。

$I$ が有限集合である場合、因子 $X_i$ のトポロジーからの積位相の構成はより単純です。基本的な集合は単なる積 $\prod_{i \in I} A_i$ であり、$A_i$ は任意です。 $i \in I$ (cf. 練習問題 9) ごとに、$X_i$ の部分集合を開きます。

#### 例 {#top-i-s4-n1-exa-1 .statement tag=0B28}

\* $n$ 空間の積 $\mathbf{R}^n$ は、実直線 $\mathbf{R}$ と同一で、$n$ 次元の実数空間と呼ばれます。 $\mathbf{R}^2$ は実平面 (cf. 章 VI, § 1) とも呼ばれます。同様に、有理線 $\mathbf{Q}$ から始めて、$n$ 次元 $\mathbf{Q}^n$ の有理線数空間 ($n = 2$ の有理平面) を定義するとします。

空間 $\mathbf{R}^n$ の位相は、$n$ のすべての積の基底集合が $\mathbf{R}$ で区間をオープンしており、これを $n$ 次元のオープンボックスと呼びます。 含む点 $x \in \mathbf{R}^n$ 形この点の近傍の基本となる系のオープンボックス。同様に、$\mathbf{R}$の区間が閉じた$n$の積を、$n$次元の閉じたボックスと呼びます。 $x$ が内部である閉じた箱は、$x$ の近傍の基本的な系形も内部です。 $\mathbf{Q}^n$ についても同様の結果があります。 \*

#### 命題 1 {#top-i-s4-prop-1 .statement tag=0B29}

$f = (f_i)$ をトポロジー 空間 $Y$ の写像から積空間 $X = \prod_{i \in I} X_i$ とします。次に、$f_i$ が各 $i \in I$ の $a$ で連続している場合に限り、$f$ は点 $a \in Y$ で連続します。

$f_i = \mathrm{pr}_i \circ f$ 以降、これは § 2, no. 3 の命題 4 の特殊なケースにすぎません。

#### 系 1 {#top-i-s4-prop-1-cor-1 .statement tag=0B2A}

$(X_i)_{i \in I}, (Y_i)_{i \in I}$ を、添字の同じ集合を持つトポロジカル空間の 2 つの族とする。それぞれの $i \in I$ について、$f_i$ を $X_i$ の写像から $Y_i$ にします。 位数では、その積写像 $f : (x_i) \to (f_i(x_i))$
$$
\prod_{i \in I} X_i \text{ into } \prod_{i \in I} Y_i
$$
点 $a = (a_i)$ で連続している必要があります。 $f_i$ が各 $i \in I$ で $a_i$ で連続していることが必要かつ十分です。

f は $x \to (f_i(\mathrm{pr}_i(x)))$ と書けるので、命題 1 条件で十分です。逆に、各 $x \in I$ について、$g_x$ を $X_x$ の写像を $\prod_{i \in I} X_i$ にすると、$i \neq x$ のときは常に $\mathrm{pr}_x(g_x(x_x)) = x_x$ と $\mathrm{pr}_i(g_x(x_x)) = a_i$ になります。 $g_x$ は命題 1 により、点 $a_x$ で連続です。 $f_x = \mathrm{pr}_x \circ f \circ g_x$ なので、$f$ が $a$ で連続であれば、$f_x$ は $a_x$ で連続であることがわかります。

#### 系 2 {#top-i-s4-prop-1-cor-2 .statement tag=0B2B}

*$X, Y$を2つのトポロジー空間とします。 写像 $f : X \to Y$ が連続であるべきである位数では、写像 $g : x \to (x, f(x))$ が $f$ のグラフ $G$ (の部分空間とみなされる) に対する $X$ の同相写像であることが必要かつ十分です。 積空間 $X \times Y$).*

$f = \mathrm{pr}_2 \circ g$なので条件で十分です。また、$f$ が連続の場合、$g$ は全単射連続 (命題 1) であり、$g$ の逆数は $\mathrm{pr}_1$ から $G$ の制限であり、連続です (cf. *集合) ためです。 理論*、章 IV, § 2, no. 4、基準 CST 17)。

#### 命題 2 (トポロジーの結合性積) {#top-i-s4-prop-2 .statement tag=0B2C}

*$(X_i)_{i \in I}$ をトポロジカル空間、集合 $I$ の $(J_x)_{x \in K}$ 分割とし、それぞれの $x \in K$ について、$X'_x = \prod_{i \in J_x} X_i$ を空間 $X_i$ の積とします。 $i \in J_K$。次に、積の標準写像空間*
$$
\prod_{i \in I} X_i \text{ onto the product space } \prod_{x \in K} X'_x
$$
*は準同型写像です。*

これは、初期トポロジの推移性の特別なケースです ($\S$ 2、no. 3、命題 5; cf. *集合理論*、章 IV, § 2, no. 4、基準 CST 13)。

一般に、*同一視する* 積空間 $\prod_{i \in I} X_i$ および $\prod_{x \in K} X'_x$ を標準写像によって実行します。

#### 系 {#top-i-s4-n1-cor-1 .statement tag=0B2D}

※$\sigma$を集合$I$の置換とします。すると、写像 $(x_i) \to (x_{\sigma(i)})$ は*の準同型写像です。
$$
\prod_{i \in I} X_i \text{ onto } \prod_{i \in I} X_{\sigma(i)}.
$$

命題 2 の $i \in I$ に対して、$K = I$ と $J_i = \{ \sigma(i) \}$ を取り出します。

#### 命題 3 {#top-i-s4-prop-3 .statement tag=0B2E}

*$X$を集合、$(Y_i)_{i \in I}$をトポロジカル空間の族とし、それぞれの$i \in I$について、$f_i$を$X$の写像を$Y_i$にします。 $f$を$X$の写像$x \to (f_i(x))$を$Y = \prod_{i \in I} Y_i$に、$\mathfrak{T}$を$X$上の最も粗い位相とし、写像$f_i$が連続します。この場合、$\mathfrak{T}$ は、$Y$ の積位相によって$f(X)$ に誘発された位相の $f$ の下で逆像になります。

これは、初期トポロジ (\S\ 2、no. 3、命題 5、cf. 集合理論、章 IV、\S\ 2、no. 4、基準 CST) の推移性の他のの特定のケースです。 15）。

#### 系 {#top-i-s4-n1-cor-2 .statement tag=0B2F}

*それぞれの $i \in I$ について、$A_i$ を $Y_i$ の部分空間とします。次に、$\prod_{i \in I} Y_i$の積位相によって$A = \prod_{i \in I} A_i$に誘導された位相は、部分空間$A_i$のトポロジの積になります。

$j_i$ を標準単射 $A_i \to Y_i$、命題を適用する 3 から写像 $f_i = j_i \circ \mathrm{pr}_i$ (cf. 集合理論, 章 IV, \S\ 2, no. 4,基準 CST 14)。

### 2. オープン集合の切断;閉じた集合の切断。オープン集合の射影。部分的な連続性

#### 命題 4 {#top-i-s4-prop-4 .statement tag=0B2G}

*$X_1, X_2$ を 2 つのトポロジー 空間とします。それぞれの $a_1 \in X_1$、写像 $x_2 \to (a_1, x_2)$ は、$X_1 \times X_2$ の部分空間 $\{a_1\} \times X_2$ に対する $X_2$ の同型写像です。

これは、定数写像 $x_2 \to a_1$ に適用される系 1 of 命題 1 of no. 1 の特殊なケースです。

写像 $x_2 \to (a_1, x_2)$ は、$X_1 \times X_2$ の同値関係 $\mathrm{pr}_2 z = \mathrm{pr}_2 z'$ に関して *連続切断* (\S\ 3, no. 5) です。したがって、この同値関係による商空間 $X_1 \times X_2$ は $X_2$ と同相です。

#### 系 {#top-i-s4-n2-cor-1 .statement tag=0B2H}

*切断 $A(x_1)$ のオープン (またはクローズ) 集合 $A$ の積 $X_1 \times X_2$ は、任意の点 $x_1 \in X_1 (*)$ が $X_2$ でオープン (またはクローズ) になります。

#### 命題 5 {#top-i-s4-prop-5 .statement tag=0B2I}

*積 $X_1 \times X_2$ の開集合 $U$ をいずれかの因子に投影したものが開集合です。*

たとえば、$\mathrm{pr}_2 U = \bigcup_{x_1 \in X_1} U(x_1)$ があり、系から命題 4 と公理 (O_1) に続き、命題が続きます。

#### 注意 1 {#top-i-s4-n2-rem-1 .statement tag=0B2J}

射影の *クローズド* 部分集合の $X_1 \times X_2$ から因子へ *クローズする必要はありません*。たとえば、有理平面 $\mathbf{Q}^2$ では、方程式が $x_1 x_2 = 1$ である双曲線は閉じた集合ですが、その射影は両方とも $\mathbf{Q}$ の点 0 の補数に等しく、これは閉じた集合ではありません。

(*) $x_1$ における $A$ の *切断* $A(x_1)$ は、$(x_1, x_2) \in A$ (cf. 集合理論 R, \S\ 3, no. 7) など、すべての $x_2 \in X_2$ の集合を意味します。

#### 命題 6 {#top-i-s4-prop-6 .statement tag=0B2K}

$X_1, X_2, Y$ を、積空間 $X_1 \times X_2$ の 3 つのトポロジー 空間、$f$ 写像を $Y$ にするとします。 $f$ が点 $(a_1, a_2)$ で連続である場合、$X_2$ から $Y$ への部分写像 $x_2 \to f(a_1, x_2)$ は点 $a_2$ で連続です。

この場合、写像は $f$ と写像 $x_2 \to (a_1, x_2)$ の合成です。したがって、結果は命題 4 から得られます。

命題 6 は、2 つの変数の連続写像がそれぞれについて個別に連続であることをというで表すことがよくあります。

#### 注意 2 {#top-i-s4-n2-rem-2 .statement tag=0B2L}

$f$ が $X_1 \times X_2$ で連続的でなくても、写像 $f : X_1 \times X_2 \to Y$ によって決定されるすべての部分写像が連続である可能性があります (cf. 章 IX, § 5、練習問題 23)。 \* たとえば、$f$ が実平面 $\mathbf{R}^2$ の写像である場合、次のように定義されます $\mathbf{R}$
$$
f(x, y) = xy/(x^2 + y^2) \quad \text{if} \quad (x, y) \neq (0, 0)
$$
と $f(0, 0) = 0$ の場合、すべての部分写像は連続です。しかし、$x \neq 0$なら$f(x, x) = 1/2$なので、$f$は$(0, 0)$では連続ではありません。

$g$ が $X_1$ から $Y$ への写像であり、点 $a_1$ で連続である場合、$X_1 \times X_1 \to Y$ の写像 $(x_1, x_2) \to g(x_1)$ はすべての点 $(a_1, x_2)$ で連続です。これは、$g$ の合成と $X_1$ への射影であるためです。

この小節の結果は、この積が $I$ の任意の分割 $(J, K)$ に対して積 $\left( \prod_{i \in J} X_i \right) \times \left( \prod_{i \in K} X_i \right)$ と同相であることに注意することで、トポロジカル空間の任意の積 $\prod_{i \in I} X_i$ に簡単に拡張できます。 (no. 1、命題 2)。

### 3. 積で閉店

#### 命題 7 {#top-i-s4-prop-7 .statement tag=0B2M}

積空間 $\prod_{i \in I} X_i$ では、集合 $\prod_{i \in I} A_i$ の積のクロージャは、それらのクロージャの積 $\prod_{i \in I} \overline{A}_i$ と同じです。

$a = (a_i)$ が $\prod_{i \in I} A_i$ の閉包にあると仮定します。次に、各 $x \in I$ について、$a_x = \operatorname{pr}_x a$ は $\operatorname{pr}_x$ (§ 2, no. 1、定理 1) の連続性により $A_x$ の閉包内にあり、したがって $a \in \prod_{i \in I} \overline{A}_i$ になります。逆に、$b = (b_i) \in \prod_{i \in I} \overline{A}_i$ と $\prod_{i \in I} V_i$ を任意の初歩的な集合含む $b$ とします。それぞれ $i \in I$、$V_i$ 含む点 $x_i \in A_i$;したがって $\prod_{i \in I} V_i$ 含む点 $(x_i) \in \prod_{i \in I} A_i$ したがって、$b$ は $\prod_{i \in I} A_i$ の終点にあります。

#### 系 {#top-i-s4-n3-cor-1 .statement tag=0B2N}

*積* $\prod_{i \in I} A_i$ *空ではない集合が積空間* $\prod_{i \in I} X_i$ **の場合に限り* $A_i$ * $X_i$ *それぞれ* $i \in I$ で閉じられます。

$I$ が *有限* の場合、各 $i \in I$ の $X_i$ で $A_i$ が開いている限り、積 $\prod_{i \in I} A_i$ は開いています。しかし、$I$ が無限の場合はそうではありません。

#### 命題 8 {#top-i-s4-prop-8 .statement tag=0B2O}

*$a = (a_i)$ *積空間* $X = \prod_{i \in I} X_i$ のいずれかの点とします。 *その後、 集合* $D$ *点* $x \in X$ *そのような* $\mathrm{pr}_i x = a_i$ *添字* $i$ の有限数を除いて * $X$ に密集します。

それぞれの $x \in X$ と、含む $x$ の各初級集合 $V = \prod_{i \in I} U_i$ には、$I$ の添字 $i$ 所属から有限部分集合 $J$ を除く $U_i = X_i$ があります。 $y_i = x_i$ を $i \in J$ に、$y_i = a_i$ を $i \notin J$ にすると、次のことが明らかです。
$$
y = (y_i) \in D \quad \text{and} \quad y \in V;
$$
したがって結果です。

### 4. トポロジカル空間の逆極限

$I$ を部分的に順序付けされた (ただし、必ずしも指示されているわけではない) 集合 (*) とし、その中に位数関係が $\alpha \leq \beta$ として書き込まれます。 各 $\alpha \in I$ について、$X_\alpha$ をトポロジー 空間とし、各対 $(\alpha, \beta)$ について、$\alpha \leq \beta$ $f_{\alpha \beta}$ を $X_\beta$ の写像から $X_\alpha$ とする。 以下の場合、$(X_\alpha, f_{\alpha \beta})$ はトポロジカル空間* の *逆系であると言います: 1) $(X_\alpha, f_{\alpha \beta})$ が集合* の *逆系である。 2) $f_{\alpha \beta}$ は、$\alpha \leq \beta$ のときは常に *連続* 写像です。 $X$ は集合 $\varprojlim X_\alpha$ を表し、各 $\alpha \in I$ について $f_\alpha$ は標準写像 $X \to X_\alpha$ とします。その場合、$f_\alpha$が連続している$X$上の*最も粗い*位相は、$X_\alpha$のトポロジーの*逆極限*（$f_{\alpha \beta}$に関して）であると言われ、この位相を含む集合$X$が呼ばれます。トポロジカル空間* $(X_\alpha, f_{\alpha \beta})$ の逆数系の * 逆数極限。 $\varprojlim X_\alpha$ を位相空間として語るときは常に、反対のことが明示的に述べられていない限り、この空間のトポロジーは $X_\alpha$ のトポロジーの逆極限であることを常に理解する必要があります。

集合 $X$ は、点 $x$ のうちの積 $\prod_{\alpha \in I} X_\alpha$ からなるの部分集合です。
$$(1)$$
$$
\mathrm{pr}_\alpha(x) = f_{\alpha \beta}(\mathrm{pr}_\beta(x))
$$
いつでも$\alpha \leq \beta$。 no. 1の命題 3から、$X_\alpha$のトポロジーの逆極限は、積空間 $\prod_{\alpha \in I} X_\alpha$の位相によって$X$に*誘導*された位相と同じであることがわかります。それぞれの $\alpha \in I$、$Y_\alpha$ が

(*) つまり、集合には再帰的かつ他動的な関係 (*集合理論* R, § 6, no. 1) が与えられます。

$X_\alpha$の部分空間、$Y_\alpha$ 形が$X_\alpha$の部分集合*の*逆系 (*集合理論* 章 III, , n° 2) である場合、次のようになります。トポロジー 空間 $\varprojlim Y_\alpha$ が $\varprojlim X_\alpha$ の *部分空間* であることは明らかです

$(X'_\alpha, f'_{\alpha\beta})$ を、同じ集合 $I$ によってインデックス付けされたトポロジカル空間の他の逆数系とし、各 $\alpha \in I$ について、$u_\alpha : X_\alpha \to X'_\alpha$ を *連続* 写像とし、$(u_\alpha)$ が *逆数になるようにします。 写像*中系;その場合、$u = \varprojlim u_\alpha$ は $X = \varprojlim X_\alpha$ から $X' = \varprojlim X'_\alpha$ への連続した写像です。なぜなら、$f'_\alpha$ が標準写像 $X' \to X'_\alpha$ である場合、$f'_\alpha \circ u = u_\alpha \circ f_\alpha$ があるため、$f'_\alpha \circ u$ は各$\alpha \in I$ に対して連続であり、主張は § 2, no. 3 の 4 つである命題から続きます。

最後に、$I$ が *有向* 集合であり、$J$ が $I$ の *共同最終* 部分集合であるとします。 $Z$ をトポロジカル空間 $(X_\alpha, f_{\alpha\beta})_{\alpha \in J, \beta \in J}$ の逆数系の逆数極限とします。したがって、標準全単射 $g : X \to Z$ (*集合理論*, 章 III, § 7, no. 2, 命題 3) は *同相同型* です。というのは、$\lambda \in J$ ごとに $\mathrm{pr}_\lambda(g(x)) = \mathrm{pr}_\lambda(x)$ があるからです。したがって、$g$ は連続です (no. 1, 命題 1)。そして、$h$ が $g$ の逆数である場合、$\alpha \in I$ ごとに $\alpha \leq \lambda$ となるような $\lambda \in J$ が存在し、したがって $\mathrm{pr}_\alpha(h(z)) = f_{\alpha\lambda}(\mathrm{pr}_\lambda(z))$ が存在します。これは、$h$ が連続であることを示します (no. 1, 命題 1)。 $f_{\alpha\lambda}$は連続です。

#### 命題 9 {#top-i-s4-prop-9 .statement tag=0B2P}

*$I$を有向集合、$J$を$I$の最終部分集合とします。 $(X_\alpha, f_{\alpha\beta})$ を、$I$ でインデックス付けされたトポロジカル空間の逆数系とします。 $X = \varprojlim X_\alpha$ とし、$f_\alpha : X \to X_\alpha$ を標準写像とします。 次に、$\alpha$ が $J$ を通過し、$U_\alpha$ がそれぞれ $\alpha \in J$ の $X_\alpha$ のトポロジーのベース $\mathfrak{B}_\alpha$ を通過する集合 $f^{-1}_\alpha(U_\alpha)$ のファミリーが、$X$ のトポロジーのベースになります。

§ 2, no. 3 から、形 $f^{-1}_\alpha(U_\alpha)$ の集合の *有限共通部分* ($X_\alpha$ で $\alpha \in I, U_\alpha$ が開く) $X$ の位相の形基底がわかります。 $(\alpha_i)_{1 \leq i \leq n}$ が $I$ の添字の有限族である場合、$1 \leq i \leq n$ に対して $\alpha_i \leq \gamma$ となるような $\gamma \in J$ が存在します。したがって $f_{\alpha_i} = f_{\alpha_i\gamma} \circ f_\gamma$;置いたら

$$
V_\gamma = \bigcap_i f^{-1}_{\alpha_i\gamma}(U_{\alpha_i}),
$$

それなら私たちは持っています

$$
f^{-1}_\gamma(V_\gamma) = \bigcap_i f^{-1}_{\alpha_i}(U_{\alpha_i});
$$

しかし、$V_\gamma$ は開いているため、集合所属から $\mathfrak{B}_\gamma$ の和集合です。したがって、結果は次のとおりです。

#### 系 {#top-i-s4-n4-cor-1 .statement tag=0B2Q}

*$A$を$X$の部分集合とし、$A_\alpha$を各$\alpha \in I$の$f_\alpha(A)$とします。それから：*

(i) *$A_\alpha$ (それぞれ $\overline{A}_\alpha$) 形 $X_\alpha$ の部分集合の逆系、および*

$$
\overline{A} = \bigcap_\alpha f^{-1}_\alpha(\overline{A}_\alpha) = \varprojlim \overline{A}_\alpha.
$$

(ii) *$A$が$X$、$A = \varprojlim A_\alpha = \varprojlim \overline{A}_\alpha$で閉じられている場合。*

(i) の最初の主張は、$\alpha \leq \beta$ の関係 $f_\alpha = f_{\alpha\beta} \circ f_\beta$ と、$f_{\alpha\beta}$ (§ 2, no. 1、定理 1) の連続性から続きます。 $A'$ を表すとします
$$
\bigcap_\alpha \overline{f}_\alpha(\overline{A}_\alpha);
$$
その場合、$A'$ が閉じており、含む $A$ であるため、$\overline{A} \subset A'$ であることは明らかです。逆に、$x \in A'$ とします。 $x$ が $A$ の終りにあることを示さなければなりません。 命題 9 により、$X_\alpha$ で$\alpha \in I$ と $U_\alpha$ が開いた$x$ の形 $\overline{f}_\alpha(U_\alpha)$ のすべての近傍が$A$ を満たすことを証明するのに十分です。さて、仮定、$f_\alpha(x) \in U_\alpha$までに、$f_\alpha(x) \in \overline{A}$以降は$U_\alpha \cap A_\alpha \neq \varnothing$になります。つまり、$A \cap \overline{f}_\alpha(U_\alpha)$は空ではありません。

(ii) を確立するには、$A$ に制限がなければ、$A \subset \lim A_\alpha \subset \lim \overline{A}_\alpha$ があると述べれば十分です。今、$A$ が閉じている場合、(i) から
$$
A = \lim \overline{A}_\alpha
$$
(ii) が続きます。

#### 例 {#top-i-s4-n4-exa-1 .statement tag=0B2R}

$I$ を有向集合とし、$(X_\alpha)_{\alpha \in I}$ を集合 $Y$ の部分集合の家族として、$\alpha \leq \beta$ になるたびに $X_\alpha \supset X_\beta$ となるようにします。それぞれの $\alpha \in I$ について、$\mathfrak{T}_\alpha$ を $X_\alpha$ の位相とします。その結果、$\alpha \leq \beta$ のときはいつでも、$\mathfrak{T}_\alpha$ によって$X_\beta$ に誘導される位相よりも、$\mathfrak{T}_\beta$ がより細かいになります。 $f_{\alpha\beta}$ を $\alpha \leq \beta$ の標準単射 $X_\beta \to X_\alpha$ とすると、$\lim X_\alpha$ は$X_\alpha$ の *共通部分* $X$ と正規的に識別され、位相が *最小となります。 $\mathfrak{T}_\alpha$ によって $X$ に誘導されたトポロジーの上界* (§ 2, no. 3, 例 2)。

### 練習問題 {#top-i-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
