---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 8
section_title: Hausdorff spaces and regular spaces
lang: ja
source: top-i-iv
book_pages: 75-83, 134-141
pdf_pages: 0081-0089, 0140-0147
extraction: ocr
subsections:
    - "no": 1
      title: HAUSDORFF SPACES
      page: 75
      pdf_page: 81
    - "no": 2
      title: SUBSPACES AND PRODUCTS OF HAUSDORFF SPACES
      page: 77
      pdf_page: 83
    - "no": 3
      title: HAUSDORFF QUOTIENT SPACES
      page: 78
      pdf_page: 84
    - "no": 4
      title: REGULAR SPACES
      page: 80
      pdf_page: 86
    - "no": 5
      title: EXTENSION BY CONTINUITY; DOUBLE LIMIT
      page: 81
      pdf_page: 87
    - "no": 6
      title: EQUIVALENCE RELATIONS ON A REGULAR SPACE
      page: 82
      pdf_page: 88
statements: 30
exercises: 29
content_sha256: 292c25e8966fd252b0e78c5e4db7ebe8297fda046b0c29ea938530523aab1e28
translated_from: content/en/top/I/08_s8_hausdorff_spaces_and_regular_spaces.md
translation_method: google
source_content_sha256: daafa83709f77ca8c5f24c854acb749ef62cc4f8fd95a86660a5a0aa731a2fec
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d2327e80fe0b782c1343e6a1294f258818948edc7e1037a37371309ad43a2399
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 8. ハウスドルフ空間とレギュラー 空間

### 1. ハウスドルフ空間

#### 命題 1 {#top-i-s8-prop-1 .statement tag=0B65}

$X$ をトポロジー 空間とします。したがって、次の主張は同等です。

(H) $X$ の 2 つの異なる点は、互いに素近傍を持ちます。
(こんにちは) $X$ のいずれかの点の閉じた近傍の共通部分は、その点だけで構成されます。
(ひぃ) 積空間 $X \times X$ の対角線は閉じた集合です。
(ひぃ) 集合 $I$ ごとに、積空間 $Y = X^I$ の対角線が $Y$ で閉じられます。
(Hiv) $X$ に複数の極限点があるフィルターはありません。
(Hv) $X$ のフィルター $\mathfrak{F}$ が $x$ に収束すると、$x$ は $\mathfrak{F}$ の唯一のクラスター 点になります。

その意味を証明してみます

$$
\begin{array}{cccccc}
(H) & \Longrightarrow & (Hi) & \Longrightarrow & (Hv) & \Longrightarrow (Hiv) \Longrightarrow (H)
\\
(H) & \Longrightarrow & (Hiii) & \Longrightarrow & (Hii) & \Longrightarrow (H).
\end{array}
$$

そして

(H) $\Longrightarrow$ (Hi): $x \neq y$ の場合、$x$ のオープン近傍 $U$ と $y$ のオープン近傍 $V$ があり、$U \cap V = \varnothing$ になります。したがって$y \notin \overline{U}$です。

(こんにちは) $\Longrightarrow$ (Hv): $y \neq x$ にしましょう。次に、$y \notin V$ のような $x$ の閉じた近傍 $V$ があり、仮定までに $M \subset V$ のような $M \in \mathfrak{F}$ が存在します。したがって$M \cap C_V = \varnothing$。しかし、$C_V$は$y$の近傍です。したがって、$y$ は $\mathfrak{F}$ のクラスター 点ではありません。

(Hv) $\Longrightarrow$ (Hiv): フィルターのすべての極限点もクラスター 点であるため、クリアです。

(Hiv) $\Longrightarrow$ (H): $x \neq y$ と、$x$ のすべての近傍 $V$ が $y$ のすべての近傍 $W$ と一致すると仮定します。次に、極限点として、$x$ と $y$ の両方を持つフィルターの集合 $V \cap W$ 形基底は、仮定とは逆です。

(H) $\Longrightarrow$ (Hiii): $(x) = (x_i)$ を、対角線 $\Delta$ に対して属するではない $X^I$ の点とします。次に、$x_\lambda \neq x_\mu$ となるような添字 $\lambda, \mu$ が少なくとも 2 つあります。 $V_\lambda$ (それぞれ $V_\mu$) を $X$ の $x_\lambda$ (それぞれ $x_\mu$) の近傍として、$V_\lambda \cap V_\mu = \varnothing$ とします。その場合、集合 $W = V_\lambda \times V_\mu \times \prod_{i \neq \lambda, \mu} X_i$ ($i \neq \lambda, \mu$ の場合、$X_i = X$) は、$X^I$ (§ 4, no. 1) の $x$ の近傍であり、$\Delta$ を満たしません。したがって、$\Delta$は$X^I$に閉まります。

(ひぃ) $\Longrightarrow$ (ひぃ): 当たり前だよ。

(Hii) $\Longrightarrow$ (H): $x \neq y$ の場合、$(x, y) \in X \times X$ は対角線 $\Delta$ にないので、(§ 4, no. 1) $x$ の近傍 $V$ と $X$ の $y$ の近傍 $W$ が存在します。 $(V \times W) \cap \Delta = \varnothing$、つまり、
$$
V \cap W = \varnothing.
$$

#### 定義 1 {#top-i-s8-def-1 .statement tag=0B66}

*トポロジカル空間満たす条件の命題 1 は、ハウスドルフまたは分離された空間と呼ばれます。そんな空間のうち位相はハウスドルフ位相と言われています*。

公理 (H) は *ハウスドルフの公理* です。

#### 例 {#top-i-s8-n1-exa-1 .statement tag=0B67}

離散空間はハウスドルフです。有理線 $Q$ はハウスドルフです。なぜなら、$x, y$ が $x < y$ となる 2 つの有理数数である場合、$x < z < y$ や近傍の $x$ ]$\leftarrow, z[$ などの有理数数 $z$ が存在します。 ]$y$の$z, \rightarrow[$は交差しません。

少なくとも 2 つの点を持ち、最も粗いトポロジー (§ 2, no. 2) を持つ集合 $X$ はハウスドルフ空間ではありません。

$f : X \to Y$ を集合 $X$ の写像として *Hausdorff* 空間 $Y$ にします。 命題 1 からすぐに、$X$ のフィルター $\mathfrak{F}$ に関して、$f$ は *最大 1 つの極限* を持つことができ、$f$ が $\mathfrak{F}$ に関して極限として $y$ を持つ場合、$y$ は次のようになります。 *$\mathfrak{F}$に関する$f$のクラスタ点*のみ。

#### 命題 2 {#top-i-s8-prop-2 .statement tag=0B68}

*$f, g$ をトポロジカル空間 $X$ からハウスドルフ空間 $Y$ への 2 つの連続する写像とします。次に、$f(x) = g(x)$ が $X$ で閉じられるように、すべての $x \in X$ のうち集合が計算されます。*

この場合、集合は写像 $x \mapsto (f(x), g(x))$ の下の $Y \times Y$ の対角線の逆像であり、連続です (§ 4, no. 1, 命題 1)。したがって、結果は (Hii) と § 2, no. 1、定理 1 から得られます。

#### 系 1 (アイデンティティの拡大の原則) {#top-i-s8-prop-2-cor-1 .statement tag=0B69}

*$f, g$ を、トポロジカル空間 $X$ からハウスドルフ空間 $Y$ への 2 つの連続する写像とします。 $X$ の部分集合が$f(x) = g(x)$ 点であれば、$f = g$。*

言い換えれば、$X$ から $Y$ (ハウスドルフ) への連続写像は、$X$ の密な部分集合のすべての点での値によって一意に決定されます。

#### 系 2 {#top-i-s8-prop-2-cor-2 .statement tag=0B6A}

*$f$ がトポロジカル空間 $X$ のハウスドルフ空間 $Y$ への連続写像である場合、$f$ のグラフは $X \times Y$ で閉じられます。

このグラフの場合、$f(x) = y$ などのすべての $(x, y) \in X \times Y$ のうち集合と、2 つの写像 $(x, y) \to y$ および $(x, y) \to f(x)$ が連続しています。

#### 命題 3 {#top-i-s8-prop-3 .statement tag=0B6B}

*$(x_i)_{1 \leq i \leq n}$ をハウスドルフ空間 $X$ の異なる点の有限族とする。すると、それぞれの $x_i$ は $X$ に近傍 $V_i$ を持ち、$V_i$ ($1 \leq i \leq n$) は相互に互いに素になります。*

証明は $n$ 上の帰納法によるものです: $n = 2$ の場合は単なる公理 (H) です。次に、$W_i$ が相互に互いに素となるように、$W_i$ ($1 \leq i \leq n - 1$) を $x_i$ の近傍とします。一方、$1 \leq i \leq n - 1$には$x_i$の近傍$T_i$と$x_n$の近傍$U_i$があり、これらは交差しません。 $V_i$ を $1 \leq i \leq n - 1$ の $W_i \cap T_i$ とすると、
$$
V_n = \bigcap_{i=1}^{n-1} U_i,
$$
命題中条件は満足しています。

#### 系 {#top-i-s8-n1-cor-1 .statement tag=0B6C}

*すべての有限ハウスドルフ空間は離散的です。*

#### 命題 4 {#top-i-s8-prop-4 .statement tag=0B6D}

*ハウスドルフ空間のすべての有限部分集合は閉まっています。*

単一の点のすべての部分集合からなるは、公理 (H\textsuperscript{i}) により閉じられます。

#### 命題 5 {#top-i-s8-prop-5 .statement tag=0B6E}

*$X$ をトポロジー 空間とし、個別の点 $x, y$ の $X$ の各対に対して、ハウスドルフ空間 $X'$ への$X$ の連続写像 $f$ があると仮定します。 $f(x) \neq f(y)$ のようになります。続いて$X$はハウスドルフ*です。

$V'$ と $W'$ をそれぞれ $X'$ の $f(x)$ と $f(y)$ の互いに素近傍とします。すると、$\overline{f}^{-1}(V')$と$\overline{f}^{-1}(W')$は、それぞれ$X$の$x$と$y$の互いに素近傍になります。

#### 系 {#top-i-s8-n1-cor-2 .statement tag=0B6F}

*ハウスドルフ位相よりより細かいであるすべての位相はハウスドルフです。*

### 2. ハウスドルフの部分空間と積空間

*ハウスドルフ空間 $X$ の部分空間 $A$ は、no. 1 ～ 標準単射 $A \to X$ の適用命題 5 でわかるように、ハウスドルフ* です。逆に、私たちは

#### 命題 6 {#top-i-s8-prop-6 .statement tag=0B6G}

*トポロジカル空間 $X$ のすべての点に、$X$ のハウスドルフ部分空間である閉じた近傍がある場合、$X$ はハウスドルフです。*

$x \in X$ を、部分空間 $V$ がハウスドルフとなるように、$X$ の$x$ の閉じた近傍を$V$ とします。次に、$V$ の$x$ の閉じた近傍は、共通部分として $\{x\}$ を持ちます (公理 (H\textsuperscript{'}))。しかし、これらは $X$ (§ 3, no. 1) の $x$ の近傍も閉じているため、$X$ は (H\textsuperscript{i}) を満たします。

すべての点がハウスドルフ近傍 (練習問題 7) を持つ *非ハウスドルフ* 空間が存在します。

#### 命題 7 {#top-i-s8-prop-7 .statement tag=0B6H}

※ハウスドルフ空間の積はすべてハウスドルフです。逆に、空ではない空間の積がハウスドルフである場合、それぞれの因子はハウスドルフ空間になります。*

$X = \prod_{i \in I} X_i$ をトポロジー 空間の積とします。次に、$x, y$ が $X$ の 2 つの異なる点である場合、一部の添字 $i$ に対して $\operatorname{pr}_i x \neq \operatorname{pr}_i y$ があり、no. 1 の命題 5 は、$X_i$ の場合、$X$ がハウスドルフであることを示します。です。逆に、$X$ がハウスドルフであり、$X_i$ が空でない場合、各 $X_i$ は $X$ (§ 4, no. 2, 命題 4) の部分空間と同型であるため、ハウスドルフです。

#### 系 1 {#top-i-s8-prop-7-cor-1 .statement tag=0B6I}

*$X$を集合とし、$(Y_i)_{i \in I}$をハウスドルフ位相位相空間の族とし、それぞれの$i \in I$に対して、$f_i$を$X$の写像を$Y_i$とします。 $X$ に、$f_i$ が連続する最も粗い位相 $\mathfrak{T}$ を持たせます。すると、$X$ がハウスドルフであるために必要かつ十分な条件は、$X$ の別個の点 $x, y$ のそれぞれの対について、一部の添字 $i \in I$ に対して $f_i(x) \neq f_i(y)$ が存在するということです。

no. 1 の 5 である命題という理由から、条件で十分です。逆に、$X$ がハウスドルフであると仮定します。 $Y = \prod_{i \in I} Y_i$ と $f = (f_i)_{i \in I}$ を写像 $x \to (f_i(x))$ とします。 $Y$の上の命題7により、§ 4, no. 1の命題3により、$\mathfrak{T}$は$Y$の位相の$f$の下の逆像になります。 $X$ の 2 つの異なる点 $x, y$ が $f(x) = f(y)$ である場合、すべてのオープン集合 (位相 $\mathfrak{T}$) のうち、含む $x$ も含むであることは明らかです。 $y$、仮定とは反対に、$X$はハウスドルフです。

#### 系 2 {#top-i-s8-prop-7-cor-2 .statement tag=0B6J}

*$(X_\alpha, f_{\alpha \beta})$をトポロジカル空間の逆系とします。 $X_\alpha$ がハウスドルフである場合、$X = \varprojlim X_\alpha$ はハウスドルフであり、$\prod_\alpha X_\alpha$ の閉じた部分空間です。

最初の主張は、$X$ がハウスドルフ空間 $\prod_\alpha X_\alpha$ (命題 7) の部分空間であるという事実から続きます。 $X$ が積空間で閉じていることを示すには、$F_{\alpha \beta}$ ($\alpha \leq \beta$) を $\prod_\alpha X_\alpha$ からなるの点 $x$ のうち $\operatorname{pr}_\alpha x = f_{\alpha \beta}(\operatorname{pr}_\beta x)$ の部分集合とします。 $F_{\alpha \beta}$ は $\prod_\alpha X_\alpha$ (no. 1、命題 2) で閉じられるため、共通部分 $X$ も同様です。

明らかに、ハウスドルフ空間 (§ 2, no. 4、例 3) の *和* はハウスドルフ空間です。

### 3. ハウスドルフ商空間

商空間 $X/R$ が *Hausdorff* である条件を探しましょう (この場合、同値関係 $R$ は *Hausdorff* と言われます)。まず、$X/R$ がハウスドルフである場合、単一の点の $X/R$ からなるの部分集合は *閉じられています* (no. 1、命題 4)、したがって *それぞれの同値類* mod $R$ *は閉じられています* $X$。しかし、この必要な条件だけでは十分ではありません。

$X/R$ の開いた集合の定義は、次の必要十分な条件を生じます。 $X/R$ は、$X$ のいずれか 2 つの異なる同値類が $X$ の互いに素飽和開いた部分集合に含まれる場合に限り、ハウスドルフです。他にもっと使いやすい条件をあげます。

#### 命題 8 {#top-i-s8-prop-8 .statement tag=0B6K}

*商空間 $X/R$ がハウスドルフになるために条件が必要なのは、$R$ のグラフ $C$ が $X \times X$ で閉じられることです。 同値関係 $R$ が開いている場合は、この条件でも十分です。*

$\varphi : X \to X/R$ を標準写像とします。すると、$C$は$(X/R) \times (X/R)$の対角$\Delta$の$\varphi \times \varphi : X \times X \to (X/R) \times (X/R)$の下にある逆像になります。したがって、命題の最初の部分は、$\varphi \times \varphi$ [公理 (Hii) と § 2, no. 1 の定理 1] の連続性から生じます。 $R$ が開いている場合、$(X/R) \times (X/R)$ は商空間 $(X \times X)/(R \times R)$ ($§ 5$、no. 3、系 ～ 命題 8) で識別され、$\Delta$ は標準像で識別されます。 集合 $C$ の $(X \times X)/(R \times R)$ は、$R \times R$ に関して飽和しています。したがって、$\Delta$ は $X \times X$ で閉じられ、したがって $X$ はハウスドルフになります。

$R$ が開いていない場合、$C$ は閉じているが、$R$ がハウスドルフではない例があります (演習 10 と 28)。

$X/R$ がハウスドルフであることを示すには、no. 1 の命題を適用する 5 もできます。 $M$ と $N$ は、$R$ の 2 つの異なる同値類であり、オープンの連続する写像 $f$ があれば十分です。 $X$ の部分集合 $A$、$R$ と含む $M$ と $N$ をハウスドルフ空間 $X'$ に変換し、1) $f$ がそれぞれ定数になるようにします。 $A$ に含まれる同値類 mod $R$、2) $f$ は、$M$ と $N$ で異なる値を取ります。 $A/R_A$ は、$X/R$ のオープン部分集合 ($§ 3$、no. 6、命題 10、系 1) で識別できるため、no. 1 の命題を適用する 5 から写像を識別できます。 $g$ は連続であるため、$f$ によって誘発される $g : A/R_A \to X'$ ($§ 3$、no. 4、命題 6)。

特に:

#### 命題 9 {#top-i-s8-prop-9 .statement tag=0B6L}

*$f$ がトポロジカル空間 $X$ のハウスドルフ空間 $X'$ への連続写像であり、$R$ が同値関係 $f(x) = f(y)$ である場合、商空間 $X/R$ はハウスドルフです*。

#### 命題 10 {#top-i-s8-prop-10 .statement tag=0B6M}

*$X$ がハウスドルフ空間で、$X$ が同値関係 $R$ に対して連続する切断 $s$ である場合、$X/R$ はハウスドルフであり、$s(X/R)$ は閉じられます。 $X$.*

($§ 3$, no. 5) $X/R$ は、ハウスドルフである $X$ の部分空間 $s(X/R)$ と同同型です。さらに、$s(X/R)$ はすべての $x \in X$ の集合であり、$s(\varphi(x)) = x$ になります。ここで、$\varphi : X \to X/R$ は標準写像です。したがって、2 番目の主張は、no. 1、命題 2 から続きます。

### 4. レギュラー 空間

#### 命題 11 {#top-i-s8-prop-11 .statement tag=0B6N}

トポロジ空間 $X$ の次のプロパティは同等です。

(O_{III}) $X$ の点のクローズド近傍の集合は、点の近傍の基本的な系です。

(O'_{III}) $X$ の閉じた部分集合 $F$ と点 $x \notin F$ を考えると、$x$ の近傍と $F$ の近傍が存在します。交差する。

(O_{III}) \Longrightarrow (O'_{III}): $F$ が閉じていて $x \notin F$ の場合、$x$ の近傍 $C_F$ に含まれる $x$ の閉じた近傍 $V$ が存在します。 $V$と$C_V$は、それぞれ$x$と$F$の近傍であり、共通のには点がありません。

(O'_{III}) \Longrightarrow (O_{III}): $W$ が $x \in X$ のオープン近傍である場合、$x$ の近傍 $U$ と近傍 $V$ が存在します。 $C_W$ は互いに素なので、$\overline{U} \subset W$ になります。

#### 定義 2 {#top-i-s8-def-2 .statement tag=0B6O}

位相幾何学的空間は、ハウスドルフで公理 (O_{III}) を満たす場合、正則であると言われます。その位相は規則的であると言われます。

離散空間は正規です。 \* § 9 では、すべてのローカル コンパクト空間 (特に実直線 $\mathbf{R}$) が正規であることがわかります。 \*

#### 命題 12 {#top-i-s8-prop-12 .statement tag=0B6P}

通常の空間のすべての部分空間は通常です。

$A$ を通常の空間 $X$ の部分空間とします。 $X$ はハウスドルフなので、$A$ (no. 2) も同様です。一方、$A$ に関する点 $x \in A$ のすべての近傍は形 $V \cap A$ であり、$V$ は $X$ の $x$ の近傍です。 $X$ が規則的であるため、$X$ には $x$ の近傍 $W$ があり、これは $X$ で閉じられ、$V$ に含まれます。 $W \cap A$ は、$A$ の $x$ の近隣となり、$A$ で閉鎖され、$V \cap A$ に含まれます。 したがって、結果は次のとおりです。 逆に:

#### 命題 13 {#top-i-s8-prop-13 .statement tag=0B6Q}

トポロジカル空間 $X$ のすべての点 $x$ に、$X$ の正規部分空間である閉じた近傍がある場合、$X$ は正規です。

$X$ は、no. 2 の命題 6 によるハウスドルフです。 $x$ を $X$ のいずれかの点とし、$V$ を $x$ のクローズドレギュラー 近傍とします。 $U$ が $V$ に含まれる $x$ の近傍である場合、$U$ は $V$ を基準とした $x$ の近傍です。したがって、仮説によれば、$V$には$x$の近傍$W$があり、これは$V$で閉じられ、$U$に含まれます。 しかし、$V$は$X$の$x$の近傍であるため、$W$は$X$の$x$の近傍であり、$V$は$X$で閉じられているため、$W$は$X$で閉じられます。

#### 注意 1 {#top-i-s8-n4-rem-1 .statement tag=0B6R}

非ハウスドルフ空間には例があり、すべての点には通常の近傍 (練習問題 7) があります。

#### 注意 2 {#top-i-s8-n4-rem-2 .statement tag=0B6S}

ハウスドルフではあるが正規ではない空間 (練習問題 20) があります。

#### 注意 3 {#top-i-s8-n4-rem-3 .statement tag=0B6T}

通常の位相よりもより細かいである位相は、通常 (練習問題 20) である必要はありません。

### 5. 拡大継続性により。ダブル極限

#### 定理 1 {#top-i-s8-thm-1 .statement tag=0B6U}

Xを位相幾何学的な空間、AをXの密な部分集合、f:A→Y写像のAを正規の空間Yにします。fから拡大するへの連続写像に対して必要かつ十分な条件 $\overline{f} : X \to Y$ は、各 $x \in X$ について、y が A に留まりながら x になる傾向があるときに、Y で $f(y)$ が極限になる傾向があるということです。 f から X までの連続する拡大 $\overline{f}$ は一意になります。

$\overline{f}$ の一意性は、恒等式の拡大の原則 (no. 1、命題 2、系 1) に続きます。 条件が必要であることは明らかです。なぜなら、$\overline{f}$ が X で連続している場合、それぞれの $x \in X$ について次のようになります。
$$
\overline{f}(x) = \lim_{y \to x, y \in A} \overline{f}(y) = \lim_{y \to x, y \in A} f(y)
$$
(§ 7, no. 5)。逆に、条件が満たされ、定義するが満たされたとします。
$$
\overline{f}(x) = \lim_{y \to x, y \in A} f(y)
$$
それぞれ$x \in X$; Y はハウスドルフであるため、$\overline{f}(x)$ は Y の明確に定義された元です。 $\overline{f}$ が各点 $x \in X$ で連続であることを示さなければなりません。次に、V' を Y の $\overline{f}(x)$ の閉じた近傍とします。そして、仮定までにXのxのオープン近傍Vがあり、$f(V \cap A) \subset V'$になります。 V はそれぞれの点の近傍であるため、次のようになります。
$$
\overline{f}(z) = \lim_{y \to z, y \in V \cap A} f(y)
$$
それぞれの $z \in V$ に対して、V' が閉じているので、このことから、$\overline{f}(z) \in \overline{f}(V \cap A) \subset V'$ となります。この結果は、Y の $f(x)$ 形のクローズ近傍が、$f(x)$ の近傍の基本系であるという事実から導き出されます。

写像 $\overline{f}$ は f をX まで連続的に拡張すると得られると言われています。

Y が通常のできないである定理 1 仮定の主張では、X、A または f (練習問題 19) に追加の制限を課すことなく弱められます。

#### 系 {#top-i-s8-n5-cor-1 .statement tag=0B6V}

$\mathfrak{F}_1$ を集合 $X_1$ のフィルター、$\mathfrak{F}_2$ を集合 $X_2$ のフィルターとします。 $\mathfrak{F}_1 \times \mathfrak{F}_2$ を $X = X_1 \times X_2$ の積フィルター (§ 6, no. 7) とし、f を X の写像にして通常の空間 Y にするとします。
a) $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$ が存在します。

b) $\lim_{x_2, \mathfrak{F}_2} f(x_1, x_2) = g(x_1)$ はすべての $x_1 \in X_1$ に対して存在します。

この場合、$\lim_{x_1, \mathfrak{F}_1} g(x_1)$ が存在し、$\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$ と等しくなります。

$X'_1 = X_1 \cup \{\omega_1\}$ (それぞれ $X'_2 = X_2 \cup \{\omega_2\}$) を、 *フィルターに関連付けられたトポロジカル空間としましょう* $\mathfrak{F}_1$ (それぞれ $\mathfrak{F}_2$) (§ 6, no. 5, 例)。 積空間 $X' = X'_1 \times X'_2$ では、$X''$ を部分空間 $X_1 \times X'_2$ と $\{(\omega_1, \omega_2)\}$ の和集合とします。 $X$は明らかに$X''$の濃厚な部分空間であり、仮説は、$(y_1, y_2)$が$X$に留まりながら$X''$のいずれかの点$(x_1, x_2)$になる傾向がある場合、$f(y_1, y_2)$は極限になる傾向があることを示唆しています。 $X''$ への連続性により、$f$ の拡大が存在することは、定理 1 から続きます。$(\omega_1, \omega_2)$ も、$X''$ に対する$X_1 \times \{\omega_2\}$ の閉包にあるため、結果はすぐに続きます (§ 7, no. 5)。

### 6. 通常の空間で同値関係

#### 命題 14 {#top-i-s8-prop-14 .statement tag=0B6W}

*$X$ *通常の空間*、$R$ *$X$は同値関係はお休みとさせていただきます。 *その後、グラフ* $C$ *of* $R$ *in* $X \times X$ *は閉じられます*。

$(a, b)$ を $C$ の終点の $X \times X$ の点とし、$V$ (それぞれ $W$) を $a$ の *閉ざされた* 近傍 (それぞれ近傍) とします。 $b$) $X$;次に、点 $(x, y) \in C \cap (V \times W)$ があります。 $x \in V$, $y$ 属するから、$R$ に対する$V$ の飽和$S$ まで。したがって、$b$ の各近傍 $W$ は $S$ と一致します。 仮定までに $S$ は *閉店* するため、$b \in S$ になります。ここで、$B$を$R$に対する$\{b\}$の飽和とすると、$a$のそれぞれの閉じた近傍$V$は$B$と一致します。 仮定までに$B$は*閉店*、$X$は*定期*であるため、$a \in B$、したがって$(a, b) \in C$になります。これで証明は完了です。

#### 系 {#top-i-s8-n6-cor-1 .statement tag=0B6X}

*通常の空間では、開いていても閉じているすべての同値関係がハウスドルフ* です。

これは、no. 3 の命題 14 と命題 8 から続きます。

#### 命題 15 {#top-i-s8-prop-15 .statement tag=0B6Y}

*$X$ *を通常の空間*、$F$ *閉じた部分集合 of* $X$、$R$ *同値関係 on* $X$ *すべての点 of* $F$ *[in other 語、同値関係、その同値類は* $F$ *(if* $F \neq \emptyset$*) および集合* $\{x\}$ *where* $x \in CF$*]。 *次に商空間* $X/R$ *はハウスドルフ*です。

$M$ と $N$ を $X$ の 2 つの異なる同値類とします。それぞれが $F$ の補数の 1 つの点で構成されている場合、ハウスドルフ部分空間 $CF$ には $M$ と $N$ の近傍が開いた 2 つの互いに素が存在します。これらは、$M$ の近傍と $X$ の $N$ であり、$R$ に関して飽和しています。 $M = F$ (つまり $F \neq \emptyset$) と $b \notin F$ が $N = \{ b \}$ の場合、$X$ が規則的であるため、交差しない $b$ のオープン近傍と $F$ のオープン近傍が存在します。これら近傍は$R$に関して飽和しており、命題が証明されます。

商空間 $X/R$ は必ずしも正規ではないことに注意してください (章 IX, § 4、練習問題 14)。

### 練習問題 {#top-i-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
