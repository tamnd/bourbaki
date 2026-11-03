---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 4
section_title: The extended real line
lang: ja
source: top-i-iv
book_pages: 342-347, 388-389
pdf_pages: 0348-0353, 0394-0395
extraction: ocr
subsections:
    - "no": 1
      title: HOMEOMORPHISMS OF OPEN INTERVALS OF $\mathbf{R}$
      page: 342
      pdf_page: 348
    - "no": 2
      title: THE EXTENDED LINE
      page: 343
      pdf_page: 349
    - "no": 3
      title: ADDITION AND MULTIPLICATION IN $\overline{\mathbf{R}}$
      page: 345
      pdf_page: 351
statements: 11
exercises: 7
content_sha256: 2de3ddf2a22c9e67f3cd9a2c939a73080deb4e752150ef3bd11f8aded545408d
translated_from: content/en/top/IV/04_s4_the_extended_real_line.md
translation_method: google
source_content_sha256: 91dd5beb94c7b102f68de8b003d98eed8682578549dc7b95cc038872a79f0294
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 8e8a2dadc65fe6620194d9447ea09aa15147db0fb2f5d25180281de358bc2b00
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 拡張された実直線

### 1. オープン区間 OF $\mathbf{R}$ の準射影

#### 命題 1 {#top-iv-s4-prop-1 .statement tag=0BQK}

$\mathbf{R}$ の空でないオープン区間はすべて $\mathbf{R}$ と同相です。

まず、有界オープン区間 $I = ]a, b[$ ($a < b$) を考えてみましょう。それぞれの $x \in I$ に $f(x) = -\left( \frac{1}{x-a} + \frac{1}{x-b} \right)$ を入れます。この写像は連続しており、$I$ では真に増加するです。これは、$\frac{1}{x-b}$ が $]-, b[$ では真に減少するであり、$]a, \to[$ では $\frac{1}{x-a}$ 真に減少するであることがわかっているためです。したがって、$f$ は、$\mathbf{R}$ (§ 2, no. 6, 定理 5) の区間 $f(I)$ に対する $I$ の同型写像です。 $f(I)$ は上下に境界がありません。たとえば、すべての $x \in I$ に対して $f(x) \leq c$ があった場合、$b-x > 0$ 以降は $1 - \frac{b-x}{x-a} \leq c(b-x)$ になります。そして、$x$ が$b$ に十分に近い場合、これは矛盾につながります (点 $b$ で有理写像である不等式の両辺の連続性により)。したがって、$f(I) = \mathbf{R}$、したがって、すべての有界オープン区間は $\mathbf{R}$ と同相です。 $g$ を $f$ の逆数とします。つまり、写像は、$\mathbf{R}$ の区間を、$I$ に含まれる区間 $J$ に無制限に開き、$I$ で開きます。 $I$は$\mathbf{R}$にオープンしているため、$J$も$\mathbf{R}$にオープンしています。有界であるため、$\mathbf{R}$ と同型です。したがって、すべての無制限のオープン区間が $\mathbf{R}$ と同相であることを証明しました。

#### 注意 {#top-iv-s4-n1-rem-1 .statement tag=0BQL}

すべての *有界な* 開いた区間が互いに同相であることを示すには、 $a \neq b$ と $a' \neq b'$ の場合、写像である形 $x \to ax + \beta$ (そして 1 つだけ) の、それ自体に対する $\mathbf{R}$ の同型性が存在することを指摘するだけで十分です。 $a$ から $a'$ および $b$ から $b'$ 、したがって写像オープン (それぞれハーフオープン、クローズ) 区間とエンドポイント $a, b$ がオープン (それぞれハーフオープン、クローズ) 区間とエンドポイント$a', b'$;読者は、$\alpha$ と $\beta$ を計算することでこれを簡単に検証できます。

### 2. 延長線

ここで、2 つの新しい元から $\mathbf{R}$ を*隣接*することにより、$\mathbf{R}$ の有界開いた区間 $I$ に対する $\mathbf{R}$ のすべての同型写像が次のように拡張できるように、トポロジカル空間 $\overline{\mathbf{R}}$ を定義するとします。 $I$ と同じ終点を持つ閉じた区間に対する $\overline{\mathbf{R}}$ の同型写像。

$\overline{\mathbf{R}}$ を、$\mathbf{R}$ に 2 つの新しい元を隣接 (*集合理論*, R, § 4, no. 5) して得られる集合とし、$-\infty$ と $+\infty$ で表します。 すべての $a \in \mathbf{R}$ と $-\infty < +\infty$ に $-\infty < a$ と $a < +\infty$ を入れることで、$\mathbf{R}$ から $\overline{\mathbf{R}}$ までの順序を拡大する決定します。したがって、線形順序付けされた集合が得られ、その順序付け誘導するは $\mathbf{R}$ の実直線の順序付けであることは明らかです。 次に、$\overline{\mathbf{R}}$のオープン区間の集合によって生成された$\overline{\mathbf{R}}$の位相を考えます。 $\overline{\mathbf{R}}$のオープン区間の$\mathbf{R}$のトレースは$\mathbf{R}$のオープン区間であるため、この位相誘導するは実直線の$\mathbf{R}$位相にあります。

#### 定義 1 {#top-iv-s4-def-1 .statement tag=0BQM}

*集合* $\overline{\mathbf{R}}$ *上記で定義された位数構造および位相を拡張実直線と呼びます。

延長線 $\overline{\mathbf{R}}$ を使用する場合、言葉を乱用して、その点を *実数* と呼ぶと便利なことがよくあります。 $\mathbf{R}$ の点は *有限実数* と呼ばれます。私たちはこの規約を *この切断とこの章* の次の 3 つの切断で採用します。将来この規則を採用するときは、本文のどの部分が拡大するであるかを明示的に示すことになります。

$a$ が有限の実数である場合、$\overline{\mathbf{R}}$ の区間 $[a, +\infty[$ と ]—$\infty, a]$ (それぞれ ]$a, +\infty[$ と ]—$\infty, a[$) は、区間とともに $\mathbf{R}$ と一致するに含まれます。 $\mathbf{R}$ はこれまで、$[a, \rightarrow[$ と ]$\leftarrow, a]$ (それぞれ ]$a, \rightarrow[$ と ]$\leftarrow, a[$ で表されていました。この新しい記法の方がはるかに頻繁に使用されます。もう一度、$\mathbf{R}$ 一致すると区間 ]—$\infty, +\infty[$ の $\overline{\mathbf{R}}$ は、ときどきと表されます。

#### 命題 2 {#top-iv-s4-prop-2 .statement tag=0BQN}

*すべての同型写像* $f$ *of* $\mathbf{R}$ *onto 区間* ]$a, b[$ *同型写像* $\overline{f}$ *of* $\overline{\mathbf{R}}$ *onto* $[a, b]$ に拡張できます。 *もし* $f$ *が増加する写像であれば、* $\overline{f}$ *は* $\overline{\mathbf{R}}$ *上* $[a, b]$の位数同型です。

$f$ を増加するの同型写像とします。 $\overline{f}(-\infty) = a$ と $\overline{f}(+\infty) = b$ を代入して拡大する $f$ を $\mathbf{R}$ にすると、$\overline{f}$ が $\overline{\mathbf{R}}$ の真に増加する写像 (したがって全単射) が $[a, b]$ になることは明らかです。したがって、$\overline{f}$ 写像は、$\overline{\mathbf{R}}$ のすべての区間を区間にオープンします。これは、$[a, b]$ に関してオープンであり、したがって、定義 1 と命題の理由により、$\mathbf{R}$ の$[a, b]$ への同型写像となります。 § 1, no. 4 の 5。

$f$ が減少するの場合、$\mathbf{R}$ の増加する同型写像 $x \to -f(x)$ で証明されたものを ]$-b, -a[$ に適用します。

したがって、区間の位数構造と位相のみを含む、§ 2 で取得された区間 $[a, b]$ のすべてのプロパティを $\overline{\mathbf{R}}$ に移すことができます。したがって、次の命題:

#### 命題 3 {#top-iv-s4-prop-3 .statement tag=0BQO}

*拡張された実直線はコンパクトです。*

したがって (章 II, § 4, no. 1, 定理 1) $\overline{\mathbf{R}}$ には、その位相と互換性のある独自の均一性があります。この均一性は、$\mathbf{R}$ の加法均一性によって $[a, b]$ に誘発される均一性と同形です。しかし、$\overline{\mathbf{R}}$の均一性によって$\mathbf{R}$に*誘発される*均一性は、$\mathbf{R}$の加法的な均一性ではないことに留意する必要があります(ただし、実直線の位相とは互換性があります)。 for $\mathbf{R}$ は、加法均一性に関して*完全な* 空間ですが、$\overline{\mathbf{R}}$ で閉じられていないため、$\overline{\mathbf{R}}$ の完全な部分空間ではありません。

#### 命題 4 {#top-iv-s4-prop-4 .statement tag=0BQP}

** $\overline{\mathbf{R}}$ の空でないすべての部分集合 * には少なくとも上界と最大の下界があります。*

$\mathbf{R}$ の空でない部分集合 $A$ の最小の上界 (それぞれ最大の下界) は、$\sup A$ (それぞれ $\inf A$) で表されます。明らかに

(1)
$$
\inf A \leq \sup A.
$$

$A \subset B$ の場合、$\sup A \leq \sup B$ と $\inf A \geq \inf B$ (*集合理論*、章 III, § 1, no. 9、命題 4)。

#### 命題 5 {#top-iv-s4-prop-5 .statement tag=0BQQ}

* $\overline{\mathbf{R}}$ の部分集合 $A$ は、$A$ が区間である場合にのみ接続されます。*

#### 系 {#top-iv-s4-n2-cor-1 .statement tag=0BQR}

*拡張実直線は、ローカル接続された空間です。*

#### 命題 6 {#top-iv-s4-prop-6 .statement tag=0BQS}

*$\overline{\mathbf{R}}$の区間$I$の$\overline{\mathbf{R}}$へのマッピング$f$は、$f$が厳密に単調で$I$上で連続である場合に限り、$I$の$f(I)$への同型写像となります。 $f(I)$ は $\overline{\mathbf{R}}$ の間隔になります。

最後に、写像 $\sup(x, y)$ と $\inf(x, y)$ は $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ で *連続* します。

### 3. $\overline{\mathbf{R}}$ の加法と乗法

注意まず、式 $-(-\infty) = +\infty$ と $-(+\infty) = -\infty$ に従って、写像 $-x$ を連続性によって $\overline{\mathbf{R}}$ まで拡張できます。このように拡張された写像は、それ自体に対する $\overline{\mathbf{R}}$ の同型写像です。

次に、$\mathbf{R} \times \mathbf{R}$ で定義され、$\mathbf{R}$ に値が定義された写像 $x + y$ と $xy$ を考えてみましょう。それらが値 *トポロジー 空間* $\overline{\mathbf{R}}$ を取ることを考慮すると、それらも $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ の特定の点での連続性によって拡張できることがわかります。

$x + y$ に関する限り、$A' = ]-\infty, +\infty]$ と $A'' = [-\infty, +\infty[$ とします。次に、次の命題があります。

#### 命題 7 {#top-iv-s4-prop-7 .statement tag=0BQT}

*写像 $x + y$ は、式に従って、連続性によって集合 $A' \times A'$ および $A'' \times A''$ に拡張できます*

$$
(2)
\begin{cases}
x + (+\infty) = (+\infty) + x = +\infty & (x \neq -\infty), \\
x + (-\infty) = (-\infty) + x = -\infty & (x \neq +\infty).
\end{cases}
$$

たとえば、$(x, y)$ は $\mathbf{R} \times \mathbf{R}$ に留まりながら点 $(a, +\infty)$ ($a \neq -\infty$) になる傾向があるため、$x + y$ は $+\infty$ になる傾向があることを示します。有限の数 $b < a$ が存在し、区間 $]b, +\infty[$ は $\mathbf{R}$ の $a$ の近傍です。有限の $c$、関係、$x > b$、$y > c - b$ は $x + y > c$ を暗示し、これは、$(x, y)$ が $(a, +\infty)$ に十分に近いときは常に、$x + y$ が$+\infty$ に限りなく近いことを示しています。他の場合でも議論は同様です。

逆に、$x + y$ * には $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ の点 $(-\infty, +\infty)$ と $(+\infty, -\infty)$ に極限* がありません。というのは、$x + y$ が極限 $k$ (有限または無限) であった場合、$(x, y)$ は $\mathbf{R} \times \mathbf{R}$ に留まりながら $(+\infty, -\infty)$ になる傾向があるため、有限の$a$ ごとに、写像 $(x + a) - x$ は次の傾向になるでしょう。 $x$は$\mathbf{R}$のままで$+\infty$になる傾向があるため、$k$。 $(x + a) - x = a$ と $a$ は任意であるため、これは不合理です。

写像 $x + y$ 写像 $A' \times A'$ (それぞれ $A'' \times A''$) を $A'$ (それぞれ $A''$) に変換します。したがって、$A'$ の合成の法則 (それぞれ $A''$) は、$\mathbf{R}$ の加法の拡大する法則です。恒等式 (章 I, , no. 1, 系 1 から命題 2) の拡大の原理により、この法則は可換かつ結合的です。 o は、この法則に対して単位元です。式 (2) より、$A'$ の唯一の非正規要素 (代数、章 I, § 2, no. 2) は $+ \infty$ です。

$x, y, z, t$ が $x \leq y$ と $z \leq t$ のように $\overline{\mathbf{R}}$ の点である場合、この不等式の両側が定義されている場合は常に $x + z \leq y + t$ になります。

$\overline{\mathbf{R}}$ 関係 $x < y$ は、式 (2) により、$z$ が有限である場合にのみ $x + z < y + z$ を意味することに注意してください。この不等式の両側が定義されている場合、関係 $x < y$ と $z < t$ が $x + z < y + t$ を意味することは簡単に検証できます。

$\overline{\mathbf{R}}$ には $x^+ = \sup (x, 0), x^- = \sup (-x, 0), |x| = \sup (x, -x)$ を入れます。したがって、$(+\infty)^+ = (-\infty)^- = +\infty$、$(+\infty)^- = (-\infty)^+ = 0$、および$|+\infty| = |- \infty| = +\infty$となります。 和 $x^+ - x^-$ と $x^+ + x^-$ はすべての $x \in \overline{\mathbf{R}}$ に対して定義されているため、恒等式の拡大の原理により、それぞれ $x$ と $|x|$ に等しくなります。また、和 $x + y$ が定義されるときは常に、$|x + y| \leq |x| + |y|$ になります。

注意逆に、§ 1, no. 1 の式 (6) と (7) は、$\overline{\mathbf{R}}$ の $x$ と $y$ の特定の値にとってもはや意味をなさない可能性があります。たとえば、$x = -\infty$ と $y = 0$ の場合、$\sup (x, y) = 0$ がありますが、$(y - x)^+ = +\infty$ であるため、和 $x + (y - x)^+$ は定義されません。

$\overline{\mathbf{R}}^*$ が $\overline{\mathbf{R}}$ の o の補数を表すものとします。次に、乗法に対する命題 7 の類似物は次のように実行されます。

#### 命題 8 {#top-iv-s4-prop-8 .statement tag=0BQU}

*写像 xy は、式に従って連続性により集合 $\overline{\mathbf{R}}^* \times \overline{\mathbf{R}}^*$ まで拡張できます*

$$
\begin{cases}
x.(+\infty) = (+\infty).x = \begin{cases} +\infty & \text{if } x > 0 \\ -\infty & \text{if } x < 0 \end{cases} \\
x.(-\infty) = (-\infty).x = \begin{cases} -\infty & \text{if } x > 0 \\ +\infty & \text{if } x < 0. \end{cases}
\end{cases}
$$

(3)

証明は読者に任せます。これは、命題 7 の証明に類似しています。

同様に、$xy$ には $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ の点 $(0, +\infty), (+\infty, 0), (0, -\infty), (-\infty, 0)$ に極限がないことがわかります。

写像 $xy$ は、$\overline{\mathbf{R}}^*$ の合成の法則であり、$\mathbf{R}$ の乗法の拡大する法則です。この法則は結合的かつ可換的です (恒等性の拡大の原理)。 単位元として 1 があります。 $\overline{\mathbf{R}}^*$ の非正規要素は $+\infty$ と $-\infty$ です。

$x \leq y$ と $z > 0$ の場合、この不等式の両側が定義されると常に $xz \leq yz$ になります。 積 $xy$ が定義されている場合、$|x| \cdot |y|$ も定義され、$|xy| = |x| \cdot |y|$ が得られます。

最後に、分配性公式

$$
x(y + z) = xy + xz
$$

拡大の恒等式の原理により、いずれかの側のすべての演算が定義されている場合には常に有効です。

(4) の左側は定義されているが、右側は定義されていない場合があることに注意してください。たとえば、$x = +\infty$、$y = 2$、$z = -1$ の場合を考えてみましょう。したがって、分配性公式は $\overline{\mathbf{R}}$ で注意して使用する必要があります。

### 練習問題 {#top-iv-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
