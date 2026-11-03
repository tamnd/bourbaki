---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 1
section_title: Diagrams and exact sequences
lang: ja
source: ac-i-vii
book_pages: 1-9, 39-40
pdf_pages: 0021-0029, 0059-0060
extraction: ocr
subsections:
    - "no": 1
      title: DIAGRAMS
      page: 1
      pdf_page: 21
    - "no": 2
      title: COMMUTATIVE DIAGRAMS
      page: 2
      pdf_page: 22
    - "no": 3
      title: EXACT SEQUENCES
      page: 3
      pdf_page: 23
    - "no": 4
      title: THE SNAKE DIAGRAM
      page: 4
      pdf_page: 24
statements: 7
exercises: 7
content_sha256: 63afb31444f68046b01f01a4b8c31191312834cdfb8ac5aef328b293c522de33
translated_from: content/en/ac/I/01_s1_diagrams_and_exact_sequences.md
translation_method: google
source_content_sha256: e122c6b77c1c3a3f195f1e5d14b8ed8bb246e933209f2cbcd2975f972a3111ae
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0ae75a034c8b839b5ed052024989376393545ddb8b9d4c645c82f9ef990e3655
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 図式と完全系列

### 1. 図式

たとえば、$A, B, C, D, E$ を 5 の集合とし、$f$ を $A$ から $B$ までの写像、$B$ から $C$ の$g$ 写像、$h$ 写像とします。 $D$から$E$まで、$u$写像は$B$から$D$まで、$v$写像は$C$から$E$までです。このような状況を要約するために、私たちはよく図式を利用します。たとえば、上記の状況は次のように要約されます。

(*) この章の結果は、§ 4を除き、書籍I～VIのみに依存します。

図式 (集合理論、章 II, § 3, no. 4)

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
& & \downarrow u \\
& & D \\
& & \downarrow v \\
& & E \\
& & \xrightarrow{h}
\end{array}
$$

(1)

このような記号$A \xrightarrow{f} B$の図式群は、$f$が$A$から$B$までの写像であることを模式的に表しています。 $f$ について曖昧さがない場合は、文字 $f$ を省略して、単純に $A \to B$ と書きます。

$A, B, C, D, E$ が群 (可換群) と $f, g, h, u, v$ 群準同型のとき、図式 (1) は、略称として、群 (可換群) の図式と呼ばれます。

原則として、図式は数学的なオブジェクトではなく、議論を読みやすくするために設計された図にすぎません。実際には、図式は、検討中のすべての集合と写像に名前を付けることを避けるための略語記号としてよく使用されます。したがって、というの代わりに「図式 (1)を考えてください」と言います。「A、B、C、D、Eを5つの集合...そしてCからEまでの$v$写像とする」。たとえば、no. 4 の命題 2 の主張を参照してください。

### 2. 可換図式

たとえば、次の図式について考えてみましょう。

$$
\begin{array}{ccccccc}
A & \xrightarrow{f} & B & \xrightarrow{g} & C & \xrightarrow{h} & D \\
a \downarrow & & b \downarrow & & c \downarrow & & d \downarrow \\
A' & \xrightarrow{f'} & B' & \xrightarrow{g'} & C' & \xrightarrow{h'} & D'
\end{array}
$$

(2)

矢印によって示される方向に横断されるダイアグラムの特定の数のセグメントで構成されるすべてのパスには、最初のセグメントの先頭によって表されるセットから最後のセグメントの終端によって表されるセットへのマッピング、つまり、横断されるさまざまなセグメントによって表されるマッピングの構成が対応します。 図式の各頂点、たとえば B に対して、慣例により B に縮小されるパスがあり、そこに対応する恒等写像 1、

(2) には、たとえば、$A$ で始まり $C'$ で終わる 3 つのパスがあります。 対応する写像は $c \circ g \circ f, g' \circ b \circ f$ と $g' \circ f' \circ a$ です。 図式は、同じ始まりと終わりを持つ図式のすべての対について、2 つの対応する写像が等しい場合、可換であると言われます。特にパス一致する対応する写像の先頭と末尾が ID である必要がある場合。

図式 (2) が可換であるためには、関係が必要かつ十分です。
$$
f' \circ a = b \circ f, \quad g' \circ b = c \circ g, \quad h' \circ f = d \circ h;
$$
ホールド;他の語では、(2) に含まれる 3 つの平方図式が可換であることが必要十分です。 関係 (3) の場合、$c \circ g = g' \circ b$ からは $c \circ g \circ f = g' \circ b \circ f$、$b \circ f = f' \circ a$ からは $g' \circ b \circ f = g' \circ f' \circ a$ を意味します。したがって、$A$ で始まり $C'$ で終わる 3 つのパスは同じ写像を与えます。 $A$ で始まり $D'$ で終わる 4 つのパス (それぞれ、$B$ で始まり $D'$ で終わる 3 つのパス) が同じ写像を与えることも同様に検証できます。 関係 (3) は、$A$ (それぞれ B、C) で始まり、$B'$ (それぞれ C'、D') で終わる 2 つのパスが同じ写像を与えることを意味します。 (2) の他の頂点対はいずれも複数のパスで結合できず、したがって図式 (2) は可換です。

以下では、図式の他の型についての同様の結果の検証は読者に委ねます。

### 3. 完全系列

次の定義 (代数、章 II, § 1, no. 4) を思い出してください。

#### 定義 1 {#ac-i-s1-def-1 .statement tag=0421}

$A$ を環、$F, G, H$ 3 つの右 (それぞれ左) $A$ モジュール、$f$ 準同型の $F$ から $G$ および $g$ 準同型の $G$ を$H$。 $\overline{g}^{-1}(0) = f(F)$ の場合、つまり、$g$ の核が $f$ の像に等しい場合、順序付けられた対 $(f, g)$ は完全系列と呼ばれます。

図式
$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$
完全系列とも呼ばれます。

同様に、4 つの加群と 3 つの準同型のうち図式からなるを考えてみましょう。
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$
この図式は、図式 $E \xrightarrow{f} F \xrightarrow{g} G$ が完全系列の場合、$F$ で正確であると言われます。 $F \xrightarrow{g} G \xrightarrow{h} H$ が完全系列の場合、正確に $G$ になると言われています。 (5) が $F$ と $G$ で正確である場合、それは正確である、または完全系列であると言われます。 完全系列と項の任意の数も同様に定義されます。

次の結果を思い出してください (引用箇所)。ここで、$E, F, G$ は右 (それぞれ左) を示します。

A-加群、矢印は準同型を表し、$0$ は加群が単位元に縮小されたことを示します。

(a) $0 \to E \xrightarrow{f} F$ が完全系列であると言うのは、$f$ が単射であるというと同等です。

(b) $E \xrightarrow{f} F \to 0$ が完全系列であると言うのは、$f$ が全射であるというと同等です。

(c) $0 \to E \xrightarrow{f} F \to 0$ が完全系列であると言うのは、$f$ が全単射であるというと等価です。つまり、$f$ は $F$ 上の $E$ の同型です。

(d) $F$が$E$の部分加群で、$i$が$F$の標準単射を$E$と$E$の$p$標準全射を$E/F$、図式に表す場合
$$
\begin{array}{ccccccc}
0 & \longrightarrow & F & \xrightarrow{i} & E & \xrightarrow{p} & E/F \longrightarrow 0
\end{array}
$$
完全系列です。

(e) $E \to F$ が準同型である場合、図は
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & f^{-1}(0) & \xrightarrow{i} & E & \xrightarrow{f} & F & \xrightarrow{p} & F/f(E) \longrightarrow 0
\end{array}
$$
(ここで、$i$ は $(0)$ から $E$ への正準注入であり、$p$ は $F/f(E)$ の正準射影です) は正確なシーケンスです。

(f) 図式の場合
$$
\begin{array}{ccccc}
E & \xrightarrow{f} & F & \xrightarrow{g} & G
\end{array}
$$
完全系列であるためには、加群 $S$、$T$、準同型 $a : E \to S$、$b : S \to F$、$c : F \to T$、$d : T \to G$ が存在し、$f = b \circ a$、$g = d \circ c$ とその 3 つが存在することが必要かつ十分です。 数列
$$
\begin{array}{ccccccccc}
E & \xrightarrow{a} & S & \longrightarrow & 0 \\
0 & \longrightarrow & S & \xrightarrow{b} & F & \xrightarrow{c} & T & \longrightarrow & 0 \\
0 & \longrightarrow & T & \xrightarrow{d} & G
\end{array}
$$
正確に言ってください。

最後に、$E \to F$ が A-加群準同型であれば、集合 $\operatorname{Ker}(f) = f^{-1}(0)$、$\operatorname{Im}(f) = f(E)$、$\operatorname{Coim}(f) = E/f^{-1}(0)$、$\operatorname{Coker}(f) = F/f(E)$ であることを思い出してください。この記法を使用すると、(9) で、$S = \operatorname{Im}(f) = \operatorname{Ker}(g)$ および $T = \operatorname{Im}(g)$ (標準的には $\operatorname{Coker}(f)$ と同型) を取ることができます。

### 4. ヘビ図式

#### 命題 1 {#ac-i-s1-prop-1 .statement tag=0422}

可換群の可換図式を考えてみましょう。
$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

(10) の 2 つの行が正確であると仮定します。それから：

(i) c が単射の場合、次のようになります。

(11) $\operatorname{Im}(b) \cap \operatorname{Im}(u') = \operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u).$

(ii) a が全射である場合、次のようになります。

(12) $\operatorname{Ker}(b) + \operatorname{Im}(u) = \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).$

(i) を証明しましょう。明らかに

$$
\operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u) \subset \operatorname{Im}(b) \cap \operatorname{Im}(u').
$$

逆に$x \in \operatorname{Im}(b) \cap \operatorname{Im}(u')$とします。 $x = b(y)$ となるような $y \in B$ が存在します。 c は単射なので、$v' \circ u' = 0$ として、$0 = v'(x) = v'(b(y)) = c(v(y))$、よって $v(y) = 0$ が得られます。 $(u, v)$が完全系列であるため、$y = u(z)$、よって、$x = b(u(z))$となるような$z \in A$が存在します。

(ii)を証明しましょう。 $v \circ u = 0$ と $v' \circ u' = 0$ として、次のことが明らかです。

$$
\operatorname{Ker}(b) + \operatorname{Im}(u) \subset \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).
$$

逆に$x \in \operatorname{Ker}(v' \circ b)$とします。次に、$b(x) \in \operatorname{Ker}(v')$ と、数列 $(u', v')$ が正確であるため、$u'(y') = b(x)$ となるような $y' \in A'$ が存在します。 a は全射なので、$a(y) = y'$, よって $b(x) = u'(a(y)) = b(u(y))$ となる $y \in A$ が存在します。続いて$x - u(y) \in \operatorname{Ker}(b)$が続き、証明が完成します。

#### 補題 1 {#ac-i-s1-lem-1 .statement tag=0423}

可換群の可換図式を考えてみましょう。

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
a \downarrow & & b \downarrow \\
A' & \xrightarrow{u'} & B'
\end{array}
$$

次に、図式となるような 1 つだけの準同型 $u_1 : \operatorname{Ker}(a) \to \operatorname{Ker}(b)$ と 1 つだけの準同型 $u_2 : \operatorname{Coker}(a) \to \operatorname{Coker}(b)$ が存在します。

$$
\begin{array}{ccc}
\operatorname{Ker}(a) & \xrightarrow{u_1} & \operatorname{Ker}(b) \\
i \downarrow & & j \downarrow \\
A & & B
\end{array}
$$

そして

$$
\begin{array}{ccc}
A' & \xrightarrow{u'} & B' \\
p \downarrow & & q \downarrow \\
\operatorname{Coker}(a) & \xrightarrow{u_2} & \operatorname{Coker}(b)
\end{array}
$$

は可換であり、i と j は標準単射、p と q は標準全射を表します。

$x \in \mathrm{Ker}(a)$なら、$a(x) = 0$と$b(u(x)) = u'(a(x)) = 0$、よって$u(x) \in \mathrm{Ker}(b)$となり、$u_1$の存在と一意性は明らかとなります。同様に、$u'(a(A)) = b(u(A)) \subset b(B)$ があり、商 $u'$ を取ると準同型 $u_2 : \mathrm{Coker}(a) + \mathrm{Coker}(b)$ が得られます。これは、(15) が可換である唯一の準同型です。

それでは、可換群の *可換* 図式 (10) から始めましょう。 補題 1 図式までに対応する

$$
\begin{array}{ccccccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) \\
i \downarrow & & j \downarrow & & k \downarrow \\
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \longrightarrow & B' & \longrightarrow & C' \\
\vdots & & \vdots & & \vdots \\
\cdots \to \mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

ここで、$i, j, k$ は、標準単射、$p, q, r$ 標準全射、および $u_1, u_2$ (それぞれ $v_1, v_2$) 準同型は、補題によって $u, u'$ (それぞれ $v, u'$) と正規に関連付けられています。 1. すぐに検証されます。この図式は可換であるということ。

#### 命題 2 {#ac-i-s1-prop-2 .statement tag=0424}

*可換式図式 (10) 数列 $(u, v)$ と $(u', u')$ が正確であると仮定します。次に:*

(i) $v_1 \circ u_1 = 0$; $u'$ が単射であれば、数列 $(u_1, v_1)$ は正確です。
(ii) $v_2 \circ u_2 = 0$; $v$ が全射であれば、数列 $(u_2, v_2)$ は正確です。
(iii) *$u'$が単射、$v$が全射であるとします。次に、次の性質を伴う準同型 $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ が 1 つだけ存在します。$x \in \mathrm{Ker}(c)$、$y \in B$、$t' \in A'$ 満たす関係 $v(y) = k(x)$ と $u'(t') = b(y)$ の場合、$d(x) = p(t')$ です。しかも数列*

(*) $$
\begin{array}{cccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) & \xrightarrow{d} \\
& & & & & \\
& & & & & \\
& & & & & \\
\mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

正確です。

(i) を証明しましょう。 $u_1$と$v_1$は、それぞれ$u$と$v$から$\mathrm{Ker}(a)$と$\mathrm{Ker}(b)$の制限と同じグラフを持っているので、$v_1 \circ u_1 = 0$になります。それから
$$
\mathrm{Ker}(v_1) = \mathrm{Ker}(b) \cap \mathrm{Ker}(v) = \mathrm{Ker}(b) \cap \mathrm{Im}(u) = \mathrm{Im}(j) \cap \mathrm{Im}(u).
$$
ただし、命題 1, (i) により、$u'$ が単射法であれば、$\mathrm{Ker}(v_1) = \mathrm{Im}(j \circ u_1) = \mathrm{Im}(u_1)$ になります。

(ii)を証明しましょう。 $u$と$v$から商を取ることで$u_2$と$v_2$が得られるので、$v_2 \circ u_2 = 0$であることは明らかです。 $v$ が全射であると仮定します。 $q$ と $p$ は全射であるため、仮説と命題 1、(ii) から次のようになります。
$$
\begin{align*}
\mathrm{Ker}(v_2) &= q(\mathrm{Ker}(v_2 \circ q)) = q(\mathrm{Ker}(v') + \mathrm{Im}(b)) = q(\mathrm{Ker}(v')) = q(\mathrm{Im}(u')) \\
&= \mathrm{Im}(q \circ u') = \mathrm{Im}(u_2 \circ p) = \mathrm{Im}(u_2).
\end{align*}
$$

最後に(iii)を証明しましょう。 $x \in \mathrm{Ker}(c)$ の場合、$v$ は全射であるため、$v(y) = k(x)$ となるような $y \in B$ が存在します。さらに $v'(b(y)) = c(k(x)) = 0$ があり、その結果、$u'$ は単射なので、$u'(t') = b(y)$ のような *固有の* $t' \in A'$ が存在します。ここで、元 $p(t') \in \mathrm{Coker}(a)$ が $v(y) = k(x)$ のように元 $y \in B$ から*独立している*ことを示します。たとえば、$y' \in B$ が他の元で、$v(y') = k(x)$ である場合、$y' = y + u(z)$、ここで $z \in A$ です。 $t'' \in A'$ が $u'(t'') = b(y')$ となる場合、$t'' = t' + a(z)$ となることがわかります。のために
$$
u'(t' + a(z)) = u'(t') + u'(a(z)) = b(y) + b(u(z)) = b(y + u(z)) = b(y').
$$
最後に$p(t'') = p(t') + p(a(z)) = p(t')$となります。すると、集合 $d(x) = p(t')$ が可能となり、写像 $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ が定義されました。

ここで、$x_1, x_2$ が $\mathrm{Ker}(c)$ と $x = x_1 + x_2$ の元である場合、$B$ の元 $y_1, y_2$ を採用し、$v(y_1) = k(x_1)$ と $v(y_2) = k(x_2)$ および選ぶが $y \in B$ になります。 元 $y_1 + y_2$; $d(x) = d(x_1) + d(x_2)$ は明らかなので、$d$ は *準同型* になります。

いくつかの $x' \in \mathrm{Ker}(b)$ に対して $x = v_1(x')$ があるとします。次に、$y \in B$ を元 $j(x')$ とします。 $b(j(x')) = 0$ であるため、$d(x) = 0$ となり、従って $d \circ v_1 = 0$ となります。逆に$d(x) = 0$とします。上記の記法では、$t' = a(s)$ があり、ここで $s \in A$ です。この場合、$b(y) = u'(t') = u'(a(s)) = b(u(s))$ または $b(y - u(s)) = 0$ になります。従って、元 $y - u(s)$ は形 $j(n)$ で、$n \in \mathrm{Ker}(b)$ となり、$k(x) = v(y) = v(u(s) + j(n)) = v(j(n)) = k(v_1(n))$ になります。 $k$ は単射法であるため、$x = v_1(n)$ となり、数列 (*) が $\mathrm{Ker}(c)$ で正確であることが証明されます。

最後に、(常に同じ記法)
$$
u_2(d(x)) = u_2(p(t')) = q(u'(t')) = q(b(y)) = 0
$$
従って $u_2 \circ d = 0$ です。 逆に、$\mathrm{Coker}(a)$ の元 $w = p(t')$ が $u_2(w) = u_2(p(t')) = 0$ (ただし、$t' \in A$) となるとします。 次に、$q(u'(t')) = 0$、その結果、$y \in B$ については $u'(t') = b(y)$ になります。 $v'(u'(t')) = 0$ として、$v'(b(y)) = 0$ があるため、$c(v(y)) = 0$、他の語 $v(y) = k(x)$ には$x \in \mathrm{Ker}(c)$ があり、定義 $w = d(x)$ により、数列 (*) が正確であることがわかります。

コーカー(a)。 (i) では Ker(b) で正確であり、(ii) では Coker(b) で正確であることがわかり、(iii) の証明が完了します。

#### 注意 {#ac-i-s1-n4-rem-1 .statement tag=0425}

図式 (10) の群がすべて (たとえば右) 環 $A$ 加群であり、準同型が A-加群準同型である場合、命題 2 で定義された準同型 d がすぐに検証されます。 (iii) も A-加群準同型: $x \in \mathrm{Ker}(c)$ と $a \in A$、および $y \in B$ が $v(y) = k(x)$ である場合、$v(ya) = k(xa)$ に注意するだけで十分です。

#### 系 1 {#ac-i-s1-prop-2-cor-1 .statement tag=0426}

図式 (10) が可換であり、2 つの行が正確であると仮定します。それから：

(i) $u'$ の場合、a と c は単射であり、b は単射です。
(ii) v、a、c が全射である場合、b は全射です。

主張 (i) は命題 2 の主張 (i) の帰結: $\mathrm{Ker}(a) = 0$ と $\mathrm{Ker}(c) = 0$ の場合、従って $\mathrm{Ker}(b) = 0$ です。

主張 (ii) は、命題 2 の主張 (ii) の帰結です: $\mathrm{Coker}(a) = 0$ と $\mathrm{Coker}(c) = 0$ の場合、従って $\mathrm{Coker}(b) = 0$ です。

#### 系 2 {#ac-i-s1-prop-2-cor-2 .statement tag=0427}

図式 (10) が可換であり、2 つの行が正確であると仮定します。これら条件の下:

(i) b が単射であり、a と v が全射である場合、c は単射です。
(ii) b が全射的で、c と $u'$ が単射的であれば、a は全射的です。

証明するには (i) 図式を考えます

$$
\begin{array}{ccccc}
u(A) & \xrightarrow{w} & B & \xrightarrow{v} & C \\
a' \downarrow & & b \downarrow & & c \downarrow \\
u'(A') & \xrightarrow{w'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

ここで、$a'$は写像で、bから$u(A)$までの制限と同じグラフで、wと$w'$は標準単射です。明らかに、この図式は可換であり、その行は正確です。さらに、$w'$ は単射的であり、仮定 v によって全射的になります。その後、命題 2 までに、(iii) 完全系列になります

$$
0 = \mathrm{Ker}(b) \longrightarrow \mathrm{Ker}(c) \xrightarrow{d} \mathrm{Coker}(a') = 0
$$

b は単射であり、$a'$ は全射であるため、 よって $\mathrm{Ker}(c) = 0$。

(ii) を証明するには、図式を検討します。

$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{w} & v(B) \\
a' \downarrow & & b \downarrow & & c' \downarrow \\
A' & \xrightarrow{w'} & B' & \xrightarrow{\sigma'} & v'(B')
\end{array}
$$

ここで、今回の$c'$はv(B)に対するcの制限と同じグラフを持つ写像であり、wとw'はそれぞれvとv'と同じグラフを持ちます。この図式は可換であり、その行は正確です。さらに、w は全射法であり、仮定 u' によって単射法です。その後、命題 2 までに、(iii) 完全系列になります。

$$
0 = \operatorname{Ker}(c') \xrightarrow{d} \operatorname{Coker}(a) \longrightarrow \operatorname{Coker}(b) = 0
$$

b は全射的であり、c' は単射的であるため。 よってコーカー (a) = 0。

### 練習問題 {#ac-i-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
