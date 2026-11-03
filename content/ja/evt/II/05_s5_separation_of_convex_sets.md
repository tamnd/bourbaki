---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 5
section_title: Separation of convex sets
lang: ja
source: evt-i-v
book_pages: TVS II.36-TVS II.40, TVS II.76-TVS II.81
pdf_pages: 0073-0077, 0113-0118
extraction: ocr
subsections:
    - "no": 1
      title: The Hahn-Banach theorem (geometric form)
      page: 36
      pdf_page: 73
    - "no": 2
      title: Separation of convex sets in a topological vector space
      page: 37
      pdf_page: 74
    - "no": 3
      title: Separation of convex sets in a locally convex space
      page: 38
      pdf_page: 75
    - "no": 4
      title: Approximation to convex functions
      page: 39
      pdf_page: 76
statements: 24
exercises: 30
content_sha256: dde3f427ce05b9278b23afe9454eca7bd21b252f162eaf2ddf12b5b7916df08e
translated_from: content/en/evt/II/05_s5_separation_of_convex_sets.md
translation_method: google
source_content_sha256: 497d18fc81f060c697d16f5bff7ad7d5e4bacb2a2d64dfc57ebdfcc324868bea
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e9af9b36c150c5eb128d5a7dc5a753886d7343c311480e703386f6ce6eb46811
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。凸部の分離集合

### 1. ハーン・バナッハ定理 (幾何学模様形)

#### 定理 1 (ハーン・バナッハ) {#evt-ii-s5-thm-1 .statement tag=07FI}

— *A をトポロジー ベクトル空間 E の空でない開いた凸集合とし、M を A を満たさない空でない線形多様体とする。すると、含む M で A を満たさない閉じた超平面 H が存在します。

つまり、問題は $0 \in A$ の場合に還元できるため、$A$ は吸収性になります。 $p$ を $A$ (II, p. 20) の *ゲージ* とし、$A$ は点 $x \in E$ の集合となり、$p(x) < 1$ となります。一方、$V$ を、$M$ によって生成された $E$ のベクトル部分空間とします。したがって、$M$ は $V$ では超平面ですが、含む $0$ ではないため、$V$ には$M$ が集合となるような固有の線型形式 $f$ が存在します。 点 $y \in V$ の$f(y) = 1$。したがって、仮定 $M \cap A = \varnothing$ は、$f(y) = 1$ を含むすべての $y \in V$ に対して、$p(y) \geqslant 1$ があることを意味します。 $f$ と $p$ は正に同次なので、$f(y) > 0$ となるすべての $y \in V$ に対して $f(y) \leqslant p(y)$ が得られます。最後に、すべての $y \in V$ に対して $p(y) \geqslant 0$ が表示されるため、*すべて* $y \in V$ に対して $f(y) \leqslant p(y)$ が表示されます。ハーン・バナッハ定理 (II, p. 22, th. 1) の分析形によれば、$E$ には拡大する $f$ である線型形式 $h$ が存在し、すべての人にとって、 $x \in E$、$h(x) \leqslant p(x)$。方程式$h(x) = 1$を使用して、$H$を$E$の超平面とします。明らかに$H \cap V = M$と$H \cap A = \varnothing$です。一方、$E$ 含むの$H$ の補数は開いた空でない集合 $A$ であるため、$H$ は $E$ (I, p. 11, 系) で*閉じられています*。

Q.E.D.

#### 注意 1 {#evt-ii-s5-n1-rem-1 .statement tag=07FJ}

$0 \in M$ のとき。 1 は次のように述べることができます。E* には *連続線型形式が存在します。*そのような* $g(x) = 0$ *in* $M$ *および* $g(x) > 0$ *in* $A$ (II, p. 8, prop. 4)。

#### 注意 2 {#evt-ii-s5-n1-rem-2 .statement tag=07FK}

$E$ が局所的に最も細かい凸位相 (II、p. 25、*例* 2) を運ぶ場合に定理を適用する 1 を適用し、簡単にするために $0 \in A$ と仮定すると、次の結果が得られます (表面的には関係ありません) 位相) : $A$ が実数ベクトル空間 $E$ の *吸収* 凸集合で、$M$ が $A$ を満たさない空ではない線形多様体である場合、超平面 $H$ が存在します。 含む $M$ など、$A$ は $H$ の片側にあります。この結果は、すべての凸集合 $A$ (II、p. 65、演習 5) に対して有効ではありません。

### 2. トポロジカルベクトル空間における凸集合の分離

#### 定義 1 {#evt-ii-s5-def-1 .statement tag=07FL}

— *実際のトポロジー ベクトル空間* $E$ の 2 つの空ではない集合* $A, B$ *は、閉じた超平面* $H$ *if* $A$ * が * $H$ によって決定される閉じた半空間の 1 つに含まれるといいます。 *そして* $B$ *はもう一方の閉じた半空間*に含まれています。

#### 定義 2 {#evt-ii-s5-def-2 .statement tag=07FM}

— *実際のトポロジー ベクトル空間の 2 つの空ではない集合* $A, B$ * は、閉じた超平面* $H$ *if* $A$ * が * $H$、*and* によって決定される開いた半空間の 1 つに含まれることによって厳密に分離されていると言われます。 $B$ *もう一方の開いたハーフスペース*に含まれます。

#### 命題 1 {#evt-ii-s5-prop-1 .statement tag=07FN}

— *$A$ * を空でない凸型集合とし、* $B$ * を実際のトポロジカルベクトル空間* $E$ における空でない凸型集合とします。 *もし* $A$ *が満たさない* $B$ *その場合、$A$ *から* $B$を隔てる閉じた超平面が存在します。

集合の場合、$C = A - B$ は開いており、凸型 (II、p. 9、prop. 7) で空ではなく、$0 \notin C$ も同様です。 II, p. 36 の定理 1 までに、$E$ に連続する線型形式 $f \neq 0$ が存在し、$C$ に $f(z) > 0$ が入ります。次に、すべての $x \in A$ と $y \in B$ に対して、$f(x) > f(y)$ が得られます。 $\alpha = \inf_{x \in A} f(x)$と書きます。 $\alpha$ は有限であり、すべての $x \in A$ に対して $f(x) \geq \alpha$ があり、すべての $y \in B$ に対して $f(y) \leq \alpha$ が得られます。方程式 $f(z) = \alpha$ で閉じた超平面 $H$ は、$A$ と $B$ を分離します。

#### 注意 {#evt-ii-s5-n2-rem-1 .statement tag=07FO}

— 1) 超平面 $H$ は $A$ を満たしません (II、p. 15、提案 1; $A$ と $B$ が 2 つの凸の空でない *開* 集合で満たさない場合、閉じたものが存在します。 超平面は、$A$ を *厳密に * $B$ から分離します。
2) ただし、$B$ が開いていない場合、たとえ$E$ が有限次元であっても、$\overline{A}$ が$\overline{B}$ を満たさなかったとしても、$A$ を$B$ から厳密に分離する閉じた超平面が存在するとは限りません。 (II、p. 78、練習問題 12)。

#### 定義 3 {#evt-ii-s5-def-3 .statement tag=07FP}

— *部分集合* $A$ *のベクトル空間* $E$、*超平面* $H$ *は、* $A$ のサポート超平面と呼ばれます、*場合* $H$ *含むの少なくとも 1 つの点 $A$ *そして* $A$ のすべての点は * $H$ の同じ側にあります。

$f$ を $E$ の線型形式とします。これは同じ零ではありません。方程式$f(x) = \alpha$の超平面が$A$のサポート超平面であるということは、$\alpha$が集合$f(A) \subset \mathbf{R}$の最小のまたは最大ののいずれかであることを意味します。他の語では、集合 $f(A)$ の範囲の 1 つが有限であり、$f(A)$ まで属するである場合に限り、方程式 $f(x) = 0$ の超平面と平行する $A$ のサポート超平面が存在します。

#### 命題 2 {#evt-ii-s5-prop-2 .statement tag=07FQ}

— *$A$ *を位相幾何学ベクトル空間* $E$ の空ではないコンパクト部分集合とします。 *$E$で*閉じた超平面* $H$ごとに、*$A$のサポート超平面が*$H$と*平行して存在します。

なぜなら、$f(x) = \gamma$が$H$の方程式で、$f$が$E$の連続線型形式である場合、$f$から$A$の制限は連続であるため、有界であり、$A$でその境界に達します（GT、 IV, § 6.1、第1)。

これは、$H$と平行して$A$の1つまたは2つのサポート超平面が存在することを示しています。最初のケースは、$A$ が $H$ と平行して超平面に完全に含まれている場合にのみ発生します。

#### 命題 3 {#evt-ii-s5-prop-3 .statement tag=07FR}

— *トポロジー ベクトル空間* $E$ では、*$A$ を空ではない内部を持つ*閉じた凸型集合にします。その後、$A$ のすべてのサポート超平面が閉じられ、$A$ 属するのすべてのフロンティア点が $A$ の少なくとも 1 つのサポート超平面になります。

$A$ のすべてのサポート超平面は、$A$ のすべての点が超平面の同じ側にあるため (II、p. 15、提案 17) です。また、$x_0$ が $A$ のフロンティア点である場合、$x_0$ は開いた空でない凸面集合 $\overset{\circ}{A}$ に属するしません。 後で番目。 II, p. 36 の 1 には、含む $x_0$ が存在し、$\overset{\circ}{A}$ を満たさない超平面 $H$ が存在します。 $A$ は $\overset{\circ}{A}$ (II、p. 14、cor. 1 から prop. 16) の閉包であるため、prop から続きます。 II、p. 15の17、その$H$は$A$のサポート超平面です。

### 3. 局所凸型空間における凸型集合の分離

#### 命題 4 {#evt-ii-s5-prop-4 .statement tag=07FS}

— $A$ を局所凸空間 $E$ の閉じた空でない凸集合とし、$K$ を $A$ を満たさない $E$ のコンパクトで空でない凸集合とします。次に、$A$ と $K$ を厳密に分離する閉じた超平面 $H$ が存在します。

というのは、$E$ には 0 の開いた凸近傍 $V$ が存在し、$A + V$ と $K + V$ が一致しないからです (GT、II, § 4.3、提案 4)。 $A + V$と$K + V$は凸で$E$に開いているので、プロップします。 II、p. 37 の 1 は、$A + V$ と $K + V$、および $a$ なおさら $A$ と $K$ を厳密に分離する、閉じた超平面 $H$ が存在することを示しています。

#### 注意 {#evt-ii-s5-n3-rem-1 .statement tag=07FT}

ハウスドルフの局所凸型空間 $E$ では、$A$ と $B$ を 2 つの閉じた空でない凸型集合、つまり互いに素とします。$E$ が有限次元の場合、分離する閉じた超平面が存在します。 $A$ (II、p. 78、練習問題 13);しかし、$E$ が無限大次元 (II、p. 78、例題 10 と 11) である場合、この結論は必ずしも真ではありません。

#### 系 1 {#evt-ii-s5-prop-4-cor-1 .statement tag=07FU}

— 局所凸型空間では、すべての閉じた凸型集合 $A$ は、含むである閉じた半空間の共通部分です。

実際、点 $x \notin A$ ごとに、$x$ を $A$ から厳密に分離する閉じた超平面が存在します (提案 4 を使用)。

#### 系 2 {#evt-ii-s5-prop-4-cor-2 .statement tag=07FV}

— ハウスドルフ局所凸空間では、すべてのコンパクト凸集合 $A$ は、閉じた半空間含むの共通部分であり、$A$ のサポート超平面によって決定されます。

というのは、$x_0 \notin A$ としましょう。 $\{ x_0 \}$ は閉じているため、$x_0$ を $A$ から厳密に分離する閉じた超平面 $H$ が存在します (提案 4)。 $f(x) = \alpha$ を $H$ ($f$ 連続線型形式) の方程式とし、すべての $x \in A$ に対して $f(x) > \alpha$ と仮定します。 $\gamma = \inf_{x \in A} f(x)$ とすると、$f(x) \geq \gamma$ 含む $A$ で定義される半空間は、方程式 $f(x) = \gamma$ のサポート超平面によって決まり、含む $x_0$ ではありません。 よって系。

コンパクトではなく、内部点を持たない閉じた凸型集合、局所凸型空間では、閉じたサポート超平面 (II、p. 86、実行 18 : cf. も) を持たない可能性があります。 V、p. 71、11) を実行します。

#### 系 3 {#evt-ii-s5-prop-4-cor-3 .statement tag=07FW}

— 局所的に凸な空間では、各線形多様体 $M$ の閉包は、含む $M$ の閉閉超平面の共通部分です。

すべての $x \notin \overline{M}$ について、$H$ を閉じた超平面とし、$x$ を $\overline{M}$ から厳密に分離します。

したがって、$\overline{M}$ は $H$ と平行です。閉じた超平面 $H_1$、含む $\overline{M}$ と$H$ に平行な含む $x$ はありません。 系が続きます。

#### 系 4 {#evt-ii-s5-prop-4-cor-4 .statement tag=07FX}

*$C$を局所凸空間$E$の閉じた凸集合とする。 A subset $A$ of $E$ is contained in $C$, if, and only if, for every real valued continuous affine function $u$ in $E$ such that $u(x) \geqslant 0$ for all $x$ in $C$, we have $u(y) \geqslant 0$ for all $y$ in $A$.*

条件は明らかに必要です。逆に、それで十分であることを示します。 点 $x \in A$ が $C$ に含まれていない場合、$x$ を $C$ から厳密に分離する方程式 $f(z) = \alpha$ の閉じた超平面が存在します。たとえば、$f(x) < \alpha$ と仮定すると、連続アフィン写像 $u = f - \alpha$ 矛盾するが仮説となります。

#### 系 5 {#evt-ii-s5-prop-4-cor-5 .statement tag=07FY}

*局所凸空間 $E$ では、頂点 $0$ の各凸円錐 $C$ の閉包は、 $0$ を通過する閉超平面によって決定される $C$ を含む閉半空間の交点です。

$\overline{C}$ は頂点 $0$ の凸円錐です (II, p. 13, 提案 14)。 $x \notin \overline{C}$ については、$x$ を $\overline{C}$ から厳密に分離する閉じた超平面 $H$ が存在します (提案 4)。ここで必要なのは、次の補題を適用することだけです。

#### 補題 1 {#evt-ii-s5-lem-1 .statement tag=07FZ}

— *頂点 $0$ を持つ円錐 $A$ が、超平面 $H$ によって決定される開いた半空間に含まれる場合、その円錐は、$H$ に平行で、$0$ を通過する、超平面 $H_0$ によって決定される閉じた半空間に含まれます。

$f(z) = \alpha$と$\alpha < 0$を$H$の方程式とすると、$f(z) = 0$は$H_0$の方程式になります。 $f(z) < 0$ のような $z \in A$ が存在する場合、$f(\lambda z) = \alpha$ のような $\lambda > 0$ が存在し、$\lambda z \in A$ として、これは仮定と矛盾します。

### 4. 凸型への近似写像

#### 命題 5 {#evt-ii-s5-prop-5 .statement tag=07G0}

*$X$を局所凸空間$E$の閉じた凸集合とする。次に、$X$ で定義されたすべての下側の半連続凸写像 $f$ は、$E$ の連続アフィン線形写像の制限から $X$ である写像の族の上部エンベロープになります。

点 $(x, t)$ の集合 $A \subset E \times \mathbf{R}$ では、写像 $(x, t) \mapsto f(x) - t$ が下位半連続であるため、$x \in X$ と $t \geqslant f(x)$ が凸 (II、p. 17、提案 19) で閉じています。次に、$x$ を $X$ のいずれかの点とし、$a \in \mathbf{R}$ を $a < f(x)$ となるようにします。コルによって。 II、p. 38の1、$E \times \mathbf{R}$には閉じた超平面$H$が存在し、含む$(x, a)$が$A$と一致しません。 $E \times \mathbf{R}$ のすべての直線連続形は形になります

$$
(z, t) \to u(z) + \lambda t ,
$$

ここで、$\lambda \in \mathbf{R}$ と $u$ は $E$ 上で連続する線型形式であるため、$H$ には形 $u(z) + \lambda t = \alpha$ という方程式があり、$H$ 含む $(x, a)$ として、 $\alpha = u(x) + \lambda a$。ここで、点 $(x, f(x)) \in A$ は属するから $H$ にならないため、$\lambda \neq 0$ になります。必要に応じて、$-\lambda$ で割ると、$H$ の方程式を $t - a = u(z - x)$ として書くことができます。したがって、$f(x) - a > 0$ として、すべての $z \in X$ に対して $f(z) > u(z - x) + a$ が得られ、これにより命題が証明されます。

#### 注意 1 {#evt-ii-s5-n4-rem-1 .statement tag=07G1}

プロップから続きます。図5より、$f$は、写像の制限から$X$まで連続し、$E$に凸である写像の有向*増加する*族の上包絡線であることがわかります。

#### 注意 2 {#evt-ii-s5-n4-rem-2 .statement tag=07G2}

さらに、$X$ が頂点 0 の閉じた凸円錐であり、$f$ が *正に均一* であると仮定します。すると、$f$は、$E$の*連続線型形式*の制限から$X$である写像の上位エンベロープになります。なぜなら、$(u_\alpha)$ を $E$ の連続アフィン線形写像の族とし、そのうち制限から $X$ は上部エンベロープとして $f$ を持ちます。 $u_\alpha = v_\alpha + \lambda_\alpha$、$\lambda_\alpha \in \mathbf{R}$、そして$v_\alpha$は$E$の連続した線型形式です。 $\lambda_\alpha = u_\alpha(0) \leq f(0) = 0$があります。一方、$x \in X$ の場合、$\mu > 0$ ごとに、
$$
\mu^{-1} \lambda_\alpha + v_\alpha(x) = \mu^{-1} (\lambda_\alpha + v_\alpha(\mu x)) = \mu^{-1} u_\alpha(\mu x) \leq \mu^{-1} f(\mu x) = f(x)
$$
したがって、$X$ の $u_\alpha \leq v_\alpha \leq f$ は、$f$ が $v_\alpha$ の上部エンベロープになります。

#### 注意 3 {#evt-ii-s5-n4-rem-3 .statement tag=07G3}

The restriction to $X$ of a continuous affine function in $E$ is a function that is affine in $X$ (i.e. both concave and convex II, p. 17); but it may be the case that there exist continuous affine functions in a compact convex set $X \subset E$, that are not the restrictions to $X$ of continuous affine functions *in* $E$ (II, p. 78, exerc. II、c))。 しかし ：

#### 命題 6 {#evt-ii-s5-prop-6 .statement tag=07G4}

*$f$ を、ハウスドルフ局所凸空間 $E$ のコンパクト凸集合 $X$ の上半連続アフィン写像とします。 $L$ を、$E$ の連続アフィン写像の制限から $X$ の集合とします。すべての $x \in X$ に対して $h(x) > f(x)$ となるような $h \in L$ の集合 $L'$ は、減少するに向けられ、その下側エンベロープは $f$ に等しくなります。*

$X$ は空ではないと仮定できます。 $u, v$ を、すべての $x \in X$ に対して $u(x) > f(x)$ と $v(x) > f(x)$ となるように、$L$ の 2 つの元とし、$b$ を、$u$ と $v$ の上界である定数とします。 $U$ (それぞれ $V$) を点 $(x, t)$ の $X \times \mathbf{R}$ のコンパクト凸集合とし、$u(x) \leq t \leq b$ (それぞれ $v(x) \leq t \leq b$) とし、$F$ を $(x, t) \in X \times \mathbf{R}$ の集合とします。 $t \leq f(x)$; $F$は凸で$X \times \mathbf{R}$に閉じています。 $U \cup V$ の凸包絡線 $K$ は $F$ と一致しません。これは、$U \cup V$ が $(x, t) \in X \times \mathbf{R}$ の集合に含まれているため、$f(x) < t$、集合は凸であり、$F$ と一致しません。 $K$ はコンパクト (II、p. 14、提案 15) であるため、$E \times \mathbf{R}$ の閉じた超平面 $H$ によって、$F$ を $K$ から厳密に分離できます。 すべての $x \in X$、超平面 $H$ は $(x, f(x))$ を $(x, b)$ から厳密に分離しており、*したがって* 単一の点 $w(x)$ で線 $\{ x \} \times \mathbf{R}$ と一致します。したがって、$H$ は、制限 $w$ から $X$ が $L$ のメンバーである連続アフィン写像のグラフです。つまり、$u$ と $v$ の下界が不等式を満たします。 $x \in X$全員に$w(x) > f(x)$。 これは、集合 $L'$ が減少するに指示されていることを証明します。 $-f$ に適用されるII、p. 39 の提案 5 は、$f$ が $L'$ の下側エンベロープであることを示しています。

#### 系 {#evt-ii-s5-n4-cor-1 .statement tag=07G5}

*$f$を$X$の連続アフィン関数とします。その場合、$X$ の $f$ に一様に収束する $L$ の要素のシーケンス $(h_n)$ が存在します。

というのは、プロップ。 6 と Dini の定理 (GT, X, § 4.1, th. 1) は、すべての $n$ に対して、$f \leq h_n \leq f + 1/n$ となるような $h_n \in L$ が存在することを示しています。

### 練習問題 {#evt-ii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
