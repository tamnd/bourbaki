---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 3
section_title: Products of sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 357-362
pdf_pages: 0362-0367
extraction: ocr
statements: 0
exercises: 0
content_sha256: f0b928ce8c0c3c2cddc92c8069acb0189ffcbe537a90f598f1b65423d3514a7d
translated_from: content/en/ens/ER/03_s3_products_of_sets.md
translation_method: google
source_content_sha256: 911c36b076fa6fa142fe625cbd3bb6de17b251c6493dfaffdaf76058fad82252
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c9b6203c2cebc2b210021ee42e17717a29eea307d948ca4a1118c55c6f2337da
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 集合中積

1. E、F を 2 つの集合とします。これは区別できる場合と区別できない場合があります。 The *ordered 対* $(x,y)$, whose first 元 $x$ is any 元 of E and whose second 元 $y$ is any 元 of F, are 元 of a new 集合, called the *積 of EはF*で表され、$E\times F$で表されます。 E と F は、$E\times F$ の *因子* と呼ばれます。 2 つの順序付けられた対は、最初の元と 2 番目の元が同じである場合にのみ同一とみなされます。その他の語、関係「$(x,y)=(x',y')$」は、関係「$x=x'$および$y=y'$」と同等です。 $z$ が $E\times F$ のいずれかの元である場合、関係 「$x$ は順序付けられた対 $z$ の最初の元」は $x$ の関数関係です。 $E\times F$ の決定する写像を E 上に配置します。これは *最初の座標写像* または *最初の射影* と呼ばれ、$\operatorname{pr}_1$ で示されます。 という「$x$ は注文された対 $z$ の最初の元です」の代わりに、「$x$ は $z$ または「$x = \mathrm{pr}_1 z$」の最初の座標 (または射影) です」とも言います。 同様に、*第 2 座標関数*、または *第 2 投影*を定義します。これは、$\mathrm{pr}_2$ で示される、$\mathrm{E} \times \mathrm{F}$ の *上* $\mathrm{F}$ へのマッピングです。

関係「$x = \mathrm{pr}_1 z$と$y = \mathrm{pr}_2 z$」は「$z = (x, y)$」と同等です。

関数 $\mathrm{pr}_1$ の部分集合の集合への拡張は、一般的な規則に従って同じ記号で示され、再び *第一射影* と呼ばれます (ここでは「座標」という用語は使用しません)。 2 番目の投影の延長についても同様です。

2. E の一般的な元 $x$ と F の一般的な元 $y$ の間の関係 R は、対 $(x, y)$ の性質であり、結果として、の定義する部分集合積 $\mathrm{E} \times \mathrm{F}$ は、R の *グラフ* と呼ばれます。逆に、$\mathrm{E} \times \mathrm{F}$ のすべての部分集合 A は、$x$ と $y$ の間の関係 $(x, y) \in \mathrm{A}$ のグラフです。

AをEの部分集合、BをFの部分集合とします。$x$と$y$の間の関係「$x \in \mathrm{A}$と$y \in \mathrm{B}$」で定義される$\mathrm{E} \times \mathrm{F}$の$\mathrm{A} \times \mathrm{B}$部分集合で表します。

3. 次の命題では、X と X$'$ は E の任意の部分集合、Y と Y $'$ は F の任意の部分集合、Z は $\mathrm{E} \times \mathrm{F}$ の任意の部分集合を表します。

(a) 関係 「$\mathrm{X} \times \mathrm{Y} = \emptyset$」は「$\mathrm{X} = \emptyset$ または $\mathrm{Y} = \emptyset$」と*同等*です。

(b) $\mathrm{X} \times \mathrm{Y} \neq \emptyset$ の場合、関係 「$\mathrm{X} \times \mathrm{Y} \subset \mathrm{X}' \times \mathrm{Y}'$」は「$\mathrm{X} \subset \mathrm{X}'$ および $\mathrm{Y} \subset \mathrm{Y}'$」と * 同等* です。

(c) すべての X、X$'$、Y について、

$$(\mathrm{X} \times \mathrm{Y}) \cup (\mathrm{X}' \times \mathrm{Y}) = (\mathrm{X} \cup \mathrm{X}') \times \mathrm{Y}. \tag{22}$$

(d) すべての X、X$'$、Y、Y$'$ について、

$$(\mathrm{X} \times \mathrm{Y}) \cap (\mathrm{X}' \times \mathrm{Y}') = (\mathrm{X} \cap \mathrm{X}') \times (\mathrm{Y} \cap \mathrm{Y}'). \tag{23}$$

(e) すべての X について、Y は次のとおりです。

$$\overset{-1}{\mathrm{pr}_1}(\mathrm{X}) = \mathrm{X} \times \mathrm{F}, \qquad \overset{-1}{\mathrm{pr}_2}(\mathrm{Y}) = \mathrm{E} \times \mathrm{Y}. \tag{24}$$

(f) $\mathrm{Y} \neq \emptyset$ の場合、すべての X について、

$$\mathrm{pr}_1(\mathrm{X} \times \mathrm{Y}) = \mathrm{X}. \tag{25}$$

(g) すべての Z に対して、

$$\mathrm{Z} \subset \mathrm{pr}_1(\mathrm{Z}) \times \mathrm{pr}_2(\mathrm{Z}). \tag{26}$$

(h) $a$ を E の元とします。そのとき、集合 $\{a\} \times \mathrm{F}$ *onto* F の写像 $(a, y) \rightarrow y$ (つまり、$\mathrm{pr}_2$ から部分集合 $\{a\} \times \mathrm{F}$ の制限) は *1 対 1* です。

4. 写像

(27) $$(x, y) \to (y, x)$$

は、$\mathrm{E} \times \mathrm{F}$ *onto* $\mathrm{F} \times \mathrm{E}$ の *1 対 1* 写像であり、*正規* と呼ばれます。 E と F が同じ集合, 写像 (27) は *正準対称* と呼ばれます。その場合、それは*強制的*になります。この対称性の下で固定される $\mathrm{E} \times \mathrm{E}$ の元 $(x, y)$ は、性質 $x = y$ を持つものです。この元のうち集合 $\Delta$ を $\mathrm{E} \times \mathrm{E}$ の *対角* と呼びます。 写像 $x \to (x, x)$ は、$\Delta$ への E の *全単射* であり、E の $\mathrm{E} \times \mathrm{E}$ への *対角線写像* と呼ばれます。

Z が $\mathrm{E} \times \mathrm{F}$ の任意のサブセットである場合、$\mathrm{E} \times \mathrm{F}$ の $\mathrm{F} \times \mathrm{E}$ への正規マッピングに基づく Z のイメージは $\overset{-1}{\mathrm{Z}}$ で示されます。 X が E のいずれかの部分集合であり、Y が F のいずれかの部分集合である場合、

$$\overset{-1}{\overgroup{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

$x$ と $y$ の間の関係 R が、$\mathrm{E} \times \mathrm{F}$ の対 $(x, y)$、定義する部分集合 A の性質とみなされ、*同じ* 関係と見なされます。 対 $(y, x)$ の性質、 定義する部分集合 $\mathrm{F} \times \mathrm{E}$ の $\overset{-1}{\mathrm{A}}$。 R は、関係、$(x, y) \in \mathrm{A}$、$(y, x) \in \overset{-1}{\mathrm{A}}$ のそれぞれに相当します。 E と F が同じ集合、関係 R および対応する部分集合 A は、$\mathrm{A} = \overset{-1}{\mathrm{A}}$ のときに *対称* であると言われます。対角線 $\Delta$ (等式の関係によって定義される) は対称です。 Z が $\mathrm{E} \times \mathrm{E}$ のいずれかの部分集合である場合、$\mathrm{Z} \cup \overset{-1}{\mathrm{Z}}$ と $\mathrm{Z} \cap \overset{-1}{\mathrm{Z}}$ は対称です。

5. A を集合 E の部分集合とし、$f$ を A の写像から集合 F にします。 E のジェネリック元 $x$ とジェネリックの間の関係 「$x \in \mathrm{A}$ と $y = f(x)$」 F の元 $y$ 定義する部分集合の $\mathrm{E} \times \mathrm{F}$ は、写像 $f$ の *グラフ* と呼ばれます。 Bが含むAであるEの部分集合で、$g$がBに対する$f$の*拡大*(§ 2, no. 13)である場合、$f$のグラフは$g$のグラフに*含まれます*。

逆に、C を $\mathrm{E} \times \mathrm{F}$ の部分集合として、$x \in \mathrm{E}$ ごとに、$(x, y) \in \mathrm{C}$ となるような $y \in \mathrm{F}$ が *最大 1 つ* 存在するようにします。次に、一般的な元 $x$ *of 集合* $\mathrm{pr}_1(\mathrm{C})$ と一般的な元 $y$ の間の関係 $(x, y) \in \mathrm{C}$ は、$y$ と決定するの関数型関係になります。 $\mathrm{pr}_1(\mathrm{C})$の写像をグラフがCであるFに変換します。

したがって、「すべての $x \in \mathrm{E}$ に対して、$(x, y) \in \mathrm{C}$ となるような $y \in \mathrm{F}$ が 1 つだけ存在する」という特性を持つ $\mathrm{E} \times \mathrm{F}$ の部分集合 C ($\mathfrak{P}(\mathrm{E} \times \mathrm{F})$ の部分集合である集合) は、E の部分集合の *F へのマッピングの *集合 と 1 対 1 に対応させることができます。

$f$ を F への E の単射詞写像とし、$g$ を $f(\mathrm{E})$ への E の全単射とみなされる $f$ の逆数とします。 Cが$f$のグラフだとすると、$g$のグラフは$\overset{-1}{\mathrm{C}}$になります。

6. $f$ が E から F への写像であり、C が E $\times$ F におけるそのグラフである場合、関係 "$y = f(x)$" は "$(x, y) \in \mathrm{C}$" と等価です。 関係「$y \in f(\mathrm{X})$」は、「$x \in \mathrm{X}$と$(x,\ y) \in \mathrm{C}$のような$x$が存在する」と同等です。

ここで、K を E $\times$ F の *任意の* 部分集合とし、X を E の任意の部分集合とします。 K(X) が、「$x \in \mathrm{X}$ と $(x, y) \in \mathrm{K}$ となるような $x$ が存在する」という関係を満たすすべての要素 $y$ からなる F の部分集合を表すものとします。したがって、この関係は「$y \in \mathrm{K}(\mathrm{X})$」と等価です。 $\mathfrak{P}(\mathrm{E})$ の $\mathfrak{P}(\mathrm{F})$ へのマッピング $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ は、E $\times$ F の *サブセット* K によって定義されると言われます。 K(X) は集合 $\mathrm{K} \cap (\mathrm{X} \times \mathrm{F})$ の 2 番目の射影であることに注意してください。 K が E の写像 $f$ を F に変換したグラフである場合、写像 $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ は $f$ から部分集合の集合までの正規の拡大です。

7. $x$ が E の一般的な元である場合、$x \rightarrow \mathrm{K}(\{x\})$ は E の写像から $\mathfrak{P}(\mathrm{F})$ であり、その値 $\mathrm{K}(\{x\})$ (言葉の乱用により $\mathrm{K}(x)$ によっても示される) は、* K *at* の *切断と呼ばれます。 $x$。 関係 $(x,\ y) \in \mathrm{K}$ は $y \in \mathrm{K}(x)$ と同等です。

逆に、E の *すべての* 写像 $x \rightarrow \Phi(x)$ を $\mathfrak{P}(\mathrm{F})$ に入れると、この方法で取得できます。 関係 $y \in \Phi(x)$ 定義する部分集合 E $\times$ F の K、そして $\Phi(x)$ は正確に $x$ における K の切断です。したがって、$\mathfrak{P}(\mathrm{F})$ への E の写像の集合 $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$ と集合は 1 対 1 の対応になります。

8. E $\times$ F の部分集合 K によって定義されるすべての写像 $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ には次の特性があり、E の写像の標準拡大の特性を F に一般化します (§2、番号 4 および 5)。
(a) $\mathrm{K}(\emptyset) = \emptyset$。
(b) 「$\mathrm{X} \subset \mathrm{Y}$」は「$\mathrm{K}(\mathrm{X}) \subset \mathrm{K}(\mathrm{Y})$」を意味します。
(c) すべての X について、Y は次のとおりです。

(28) $$\mathrm{K}(\mathrm{X} \cup \mathrm{Y}) = \mathrm{K}(\mathrm{X}) \cup \mathrm{K}(\mathrm{Y}),$$
(29) $$\mathrm{K}(\mathrm{X} \cap \mathrm{Y}) \subset \mathrm{K}(\mathrm{X}) \cap \mathrm{K}(\mathrm{Y}).$$

K と K$'$ が $\mathrm{K} \subset \mathrm{K}'$ となるような E $\times$ F の 2 つの部分集合である場合、すべての $\mathrm{X} \subset \mathrm{E}$ に対して $\mathrm{K}(\mathrm{X}) \subset \mathrm{K}'(\mathrm{X})$ が得られます。特に、すべての $x \in \mathrm{E}$ に対して $\mathrm{K}(x) \subset \mathrm{K}'(x)$ です。逆に、$x \in \mathrm{E}$がすべて$\mathrm{K}(x) \subset \mathrm{K}'(x)$であれば、$\mathrm{K} \subset \mathrm{K}'$になります。

9. E の一般的な元と F の一般的な元の間の関係定義する部分集合 E の K $\times$ F と F $\times$ E の部分集合 $\overset{-1}{\mathrm{K}}$、したがって写像 $\mathfrak{P}(\mathrm{E})$の$\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$が$\mathfrak{P}(\mathrm{F})$に、写像の$\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$が$\mathfrak{P}(\mathrm{F})$から$\mathfrak{P}(\mathrm{E})$に。

K が E の写像 $f$ を F に変換したグラフである場合、写像 $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$ は $f$ の逆数拡大です。

$K$ が $E \times F$ の任意の部分集合である場合、関係 (18) と (19) は写像 $X \to K(X)$ と $Y \to \overset{-1}{K}(Y)$ に一般化されないことに注意する必要があります。

10. E、F、G を 3 つの集合とし、区別できる場合と区別できない場合があります。A を $E \times F$ の部分集合とし、B を $F \times G$ の部分集合とします。次に、性質を持つ $E \times G$ の元 $(x, z)$ は、「$(x, y) \in A$ と $(y, z) \in B$ となるような $y \in F$ が存在します」、$E \times G$ の形部分集合、* B * と* A の *合成と呼ばれます、そして$B \circ A$、または混乱の危険がない場合は単に BA で示されます。ここでも、合成の順序が重要です。

¶ $\mathfrak{P}(E)$ の $\mathfrak{P}(G)$ へのマッピング $X \to BA(X)$ は、$Y \to B(Y)$ と $X \to A(X)$ の合成です。言い換えれば、すべての $X \subset E$ について、

$$(30) \qquad BA(X) = B(A(X)).$$

H を他の集合とし、必ずしも E、F、G と区別する必要はありません。また、C を $G \times H$ の部分集合とします。次に、$C \circ (B \circ A) = (C \circ B) \circ A$ があります。この集合は $C \circ B \circ A$ (または単に CBA) とも表され、この順序に含まれる C、B、A の *合成* と呼ばれます。

$f$ を E から F への写像とし、$g$ を F から G への写像とします。A (または B) が $f$ (または $g$) のグラフである場合、合成 BA は合成写像 $g \circ f$ のグラフです。

11. 私たちは、

$$(31) \qquad \overset{-1}{\overbrace{B \circ A}} = \overset{-1}{A} \circ \overset{-1}{B}.$$

A、A′を$E \times F$の2つの部分集合とし、B、B′を$F \times G$の2つの部分集合とする。それから関係

$$\text{“}A \subset A' \text{ and } B \subset B'\text{”} \qquad \text{implies} \qquad \text{“}B \circ A \subset B' \circ A'\text{”}.$$

A を $E \times F$ の部分集合、$E \times E$ の対角線 $\Delta$、および $F \times F$ の対角線 $\Delta'$ とします。それでは、

$$(32) \qquad A \circ \Delta = \Delta' \circ A = A.$$

12. E、F、G を 3 つの集合とします。これらは区別できる場合と区別できない場合があります。 それらの *積* $E \times F \times G$ は、順序付けされた *トリプル* $(x, y, z)$ の集合です。ここで、$x \in E$、$y \in F$、$z \in G$、関係 "$(x, y, z) = (x', y', z')$" は "$x = x'$ および $y = y'$ と同等です。 $z = z'$」。 $E \times F \times G$ の E、F、G への 3 つのマッピング $(x, y, z) \to x$、$(x, y, z) \to y$、$(x, y, z) \to z$ は、それぞれ *第一、第二、*、および *第三の座標関数* (または *射影*) と呼ばれます。同様に、たとえば、*インデックス* 1、2 の射影はマッピングです。

$$
(x, y, z) \mapsto (x, y)
$$

$E \times F \times G$ を $E \times F$ に移し、$\mathrm{pr}_{1,2}$ で表します。

番号の定義と命題 2、3、および 4 は、3 つの集合のうち積に簡単に一般化できます。

さらに、3 つの集合の積 $E \times F \times G$ を考慮する代わりに、2 つの集合から積を形成する演算を 2 回適用して得られる積 $(E \times F) \times G$ を同等に考慮することもできます。実際、$(x, y, z) \mapsto ((x, y), z)$ は、*canonical* と呼ばれる、$E \times F \times G$ の $(E \times F) \times G$ に対する 1 対 1 の写像です。同様に、$E \times F \times G$ の写像を集合 $E \times (F \times G)$ に定義する 1 対 1 で変換し、E、F、G の 3 つの文字を並べ替えることによって $E \times F \times G$、$(E \times F) \times G$、$E \times (F \times G)$ から得られたすべての集合に変換します。

類似した定義と、3 つ以上の集合の積のプロパティがあります。

13. 任意の集合 $E'$ の値をとった写像 $f$ が、3 つの集合 $E$、$F$、$G$ の積で定義される場合、次のように言われます。 写像の *3 つの変数*。それぞれは、集合、$E$、$F$、$G$ のいずれかを通過します。 $E \times F \times G$の元$(x, y, z)$における$f$の値は$f(x, y, z)$で表されます。

$a$ を $E$ のいずれかの元とします。次に、$(y, z) \mapsto f(a, y, z)$ は、$F \times G$ の写像から $E'$ になり、$x$ の $f$ 対応するから値 $a$ によって決定される *部分写像 (または写像) と呼ばれます。また、$F \times G$ の $f$ と写像 $(y, z) \mapsto (a, y, z)$ を $E \times F \times G$ に合成したものでもあります。

同様に、$b$ が $F$ の元である場合、$z \mapsto f(a, b, z)$ は $G$ の $E'$ の写像であり、$f$ 対応するから値によって決定される部分写像と呼ばれます。 $x$、$y$の$a$、$b$。

逆に、$g$を$E$の写像を$E'$とします。 次に、$(x, y, z) \mapsto g(x)$ は、$E \times F \times G$ から $E'$ へのマッピング $h$ であり、$h$ によって決定される $E$ から $E'$ へのすべての部分マッピングは、$y$ と $z$ の値に対応し、$g$ と同一になります。 この事実は、多くの場合、議論 $x$ の写像は、その時点で考慮する必要があり、もちろん $x$ を含むすべての議論の写像として想定できるというというによって表現されます。

14. $f$、$g$、$h$を、それぞれ$E$の3つの写像を$E'$に、$F$を$F'$に、$G$を$G'$にします。 $E \times F \times G$の$E' \times F' \times G'$への写像$(x, y, z) \mapsto (f(x), g(y), h(z))$は$f \times g \times h$で表され、$f$、$g$、$h$から積*の*拡大と呼ばれます。 $f$、$g$、$h$ の 3 つすべてが単射（それぞれ全単射、全単射）である場合、$f \times g \times h$ は単射（それぞれ全単射、全単射）です。

今回と前回の小節では、単にアイデアを修正するために *3* 集合の場合のみを検討しました。同様の考慮事項が、集合の有限の数にも当てはまります。
