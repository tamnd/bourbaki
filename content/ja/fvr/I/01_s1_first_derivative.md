---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 1
section_title: FIRST DERIVATIVE
lang: ja
source: fvr-i-vii
book_pages: 3-12, 35-37
pdf_pages: 0018-0027, 0050-0052
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVE OF A VECTOR FUNCTION
      page: 3
      pdf_page: 18
    - "no": 2
      title: LINEARITY OF DIFFERENTIATION
      page: 5
      pdf_page: 20
    - "no": 3
      title: DERIVATIVE OF A PRODUCT
      page: 6
      pdf_page: 21
    - "no": 4
      title: DERIVATIVE OF THE INVERSE OF A FUNCTION
      page: 8
      pdf_page: 23
    - "no": 5
      title: DERIVATIVE OF A COMPOSITE FUNCTION
      page: 9
      pdf_page: 24
    - "no": 6
      title: DERIVATIVE OF AN INVERSE FUNCTION
      page: 9
      pdf_page: 24
    - "no": 7
      title: DERIVATIVES OF REAL-VALUED FUNCTIONS
      page: 10
      pdf_page: 25
statements: 36
exercises: 9
content_sha256: 2ab7d75e739ef6373251bce04e8578d335d656597c67903c491159c26ca6a54f
translated_from: content/en/fvr/I/01_s1_first_derivative.md
translation_method: google
source_content_sha256: 5dea356d12e98a054923f53371a9f84b313b2a5f5dd6646107d466573ef4a73f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 6ffc092b7c9fcf8c664ef94e0e852d9a7cb1bc8299d603ef3cd932375b785d9b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。一次導関数

はじめに述べたように、今回の章と次回では、実数体 $\mathbf{R}$ の部分集合で定義される写像の微小な性質を研究し、それらの値を *ハウスドルフ トポロジカルベクトル空間* E 上の体で取り上げます。 $\mathbf{R}$;簡潔にするために、そのような写像は実数変数 * の *ベクトル写像であると言いましょう。最も重要なケースは、$E = \mathbf{R}$ (実数変数の実数値写像) の場合です。 $E = \mathbf{R}^n$のとき、E簡約するの値とベクトル写像を$n$有限実数写像を同時に考慮します。

定義と、章 I 拡大するから写像に記載されているプロパティの多くは、体の部分集合 $\mathbf{C}$ 複素数で定義され、それらの値をトポロジカルベクトル空間で引き継ぎます。 $\mathbf{C}$ (複素変数のベクトル写像)。 これらの定義とプロパティ拡大するから写像までは、任意の可換 *位相体* K の部分集合で定義され、それらの値を K 上の位相位相ベクトル空間に取ります。

これらの一般化を移行で示します (特に I、p. 10、*注意 2* を参照)。特に複素変数の写像の場合を強調します。これらは実数変数の写像とともに最も重要であり、後の本でさらに詳しく検討します。

### 1. ベクトル写像の導関数

#### 定義 1 {#fvr-i-s1-def-1 .statement tag=082P}

*$f$ を、単一の点に対して簡約するではない区間 $I \subset \mathbf{R}$ で定義されたベクトル写像とします。 * の場合、$f$ は点 $x_0 \in I$ で微分可能であると言います。
$$
\lim_{x \to x_0, x \in I, x \neq x_0} \frac{f(x) - f(x_0)}{x - x_0}
$$
* 存在します ($f$ が値になるベクトル空間);この極限の値は、点$x_0$における$f$の一次導関数（または単に導関数）と呼ばれ、$f'(x_0)$または$Df(x_0)$で表されます*。

$f$ が点 $x_0$ で微分可能である場合、$f$ の *制限* は、簡約するが単一の点にならない、$x_0 \in J$ などの任意の区間 $J \subset I$ に微分可能です。そして、この制限の導関数は $f'(x_0)$ に等しくなります。逆に、$J$を$I$に対する$x_0$の$I$と含む近傍に含まれる区間とします。 $f$ から $J$ の制限が点 $x_0$ で導関数を認める場合、$f$ も同様です。

これらの性質をという導関数の概念は局所的な概念であると要約します。

#### 注意 1 {#fvr-i-s1-n1-rem-1 .statement tag=082Q}

運動学では、点 $\mathbf{f}(t)$ が$t$ 空間 $\mathbf{R}^3$ で移動する点の位置である場合、$\frac{\mathbf{f}(t) - \mathbf{f}(t_0)}{t - t_0}$ は瞬間 $t_0$ と $t$ の間の平均速度、およびその極限と呼ばれます。 $\mathbf{f}'(t_0)$ は、$t_0$ (この極限が存在する場合) の瞬間速度 (または単に速度) です。*

#### 注意 2 {#fvr-i-s1-n1-rem-2 .statement tag=082R}

$I$ で定義された写像 $\mathbf{f}$ が点 $x_0 \in I$ で微分可能である場合、この点で$I$ に対して必然的に連続です。

#### 定義 2 {#fvr-i-s1-def-2 .statement tag=082S}

*$\mathbf{f}$ を区間 $I \subset \mathbf{R}$ で定義されたベクトル写像とし、$x_0$ を区間 $I \cap [x_0, +\infty[$ (それぞれ $I \cap ]-\infty, x_0]$) が成立しないように $I$ の点とします。 簡約するから単一の点まで。 $\mathbf{f}$ の制限から区間 $I \cap [x_0, +\infty[$ (それぞれ $I \cap ]-\infty, x_0]$) が点で微分可能である場合、$\mathbf{f}$ は右側 (それぞれ左側) 点 $x_0$ で微分可能であると言います。 $x_0$;この制限の点 $x_0$ での導関数の値は、点 $x_0$ での $\mathbf{f}$ の右 (または左) 導関数と呼ばれ、$\mathbf{f}'_d(x_0)$ (それぞれ $\mathbf{f}'_g(x_0)$) で表されます*。

$\mathbf{f}$ を $I$ で定義されたベクトル写像とし、$x_0$ を $I$ の内部点として、$\mathbf{f}$ がこの点で連続するとします。それはdefsから続きます。 1 と 2 から、$\mathbf{f}$ が $x_0$ で微分可能であるためには、$\mathbf{f}$ がこの点で右導関数と左導関数の両方を認め、これらの導関数が等しいことが必要かつ十分であることがわかります。そしてそれから

$$
\mathbf{f}'(x_0) = \mathbf{f}'_d(x_0) = \mathbf{f}'_g(x_0).
$$

#### 例 1 {#fvr-i-s1-n1-exa-1 .statement tag=082T}

定数写像は点ごとに零の導関数を持ちます。

#### 例 2 {#fvr-i-s1-n1-exa-2 .statement tag=082U}

アフィン線形写像 $x \mapsto ax + b$ は、点ごとに $a$ に等しい導関数を持ちます。

#### 例 3 {#fvr-i-s1-n1-exa-3 .statement tag=082V}

実数写像 $1/x$ ($x \neq 0$ で定義) は、$\left( \frac{1}{x} - \frac{1}{x_0} \right) / (x - x_0) = -\frac{1}{x x_0}$ があるため、各点 $x_0 \neq 0$ で微分可能であり、$1/x$ は $x_0$ で連続であるため、前の式の極限は次のようになります。 $-1/x_0^2$。

#### 例 4 {#fvr-i-s1-n1-exa-4 .statement tag=082W}

$\mathbf{R}$ で定義されたスカラー 写像 $|x|$ は、$x = 0$ で右導関数 $+1$ と左導関数 $-1$ を持ちます。この点では微分できません。

#### 例 5 {#fvr-i-s1-n1-exa-5 .statement tag=082X}

$x = 0$ では 0、$x \neq 0$ では $x \sin 1/x$ に等しい実数写像は、$\mathbf{R}$ では定義され連続ですが、点 $x \neq 0$ では右導関数も左導関数もありません。* 写像では連続である写像の例を与えることができます。 区間であり、区間の各点で導関数がありません (I、p. 35、演習 2 および 3)。

#### 定義 3 {#fvr-i-s1-def-3 .statement tag=082Y}

*区間 $I \subset \mathbf{R}$ で定義されたベクトル写像 $\mathbf{f}$ が、各点で微分可能 (それぞれ右微分可能、左微分可能) であれば、$I$ で微分可能 (それぞれ右微分可能、左微分可能) であると言います。 $I$; $I$ で定義された写像 $x \mapsto \mathbf{f}'(x)$ (それぞれ $x \mapsto \mathbf{f}'_d(x)$、$x \mapsto \mathbf{f}'_g(x)$) は、派生写像、または (言葉の乱用により) $\mathbf{f}$ の導関数 (それぞれ右導関数、左導関数) と呼ばれ、$\mathbf{f}'$ または$\mathrm{Df}$ または $d\mathbf{f}/dx$ (それぞれ $\mathbf{f}'_d, \mathbf{f}'_g$)*

#### 注意 {#fvr-i-s1-n1-rem-3 .statement tag=082Z}

写像は、微分が区間の点ごとに連続でなくても、区間で微分可能である可能性があります (*cf.* I、p. 36、演習 5)。 *これは、写像の例が、$x = 0$ では 0、$x \neq 0$ では $x^2 \sin 1/x$ に等しいことで示されます。どこにでも導関数がありますが、この導関数は点 $x = 0$ で不連続です。

### 2. 微分の直線性

#### 命題 1 {#fvr-i-s1-prop-1 .statement tag=0830}

* 区間 $I \subset \mathbf{R}$ で定義されたベクトル写像の集合は、与えられたトポロジー ベクトル空間 $E$ で値を取り、点 $x_0$ で微分可能です。 ベクトル空間は $\mathbf{R}$ を超え、写像 $f \mapsto Df(x_0)$ は、この空間の線形写像が $E$ になります。*

他の語では、$f$ と $g$ が $I$ で定義され、点 $x_0$ で微分可能である場合、$f + g$ と $fa$ ($a$ は任意のスカラー) は $x_0$ とその導関数で微分可能です。それぞれ$f'(x_0) + g'(x_0)$と$f'(x_0)a$があります。これは、それぞれ$E \times E$と$E$における$x + y$と$xa$の連続性の直後に続きます。

#### 系 {#fvr-i-s1-n2-cor-1 .statement tag=0831}

* 区間 $I$ で定義されたベクトル写像の集合は、与えられたトポロジベクトル空間 $E$ で値を取り、$I$ で微分可能であり、$\mathbf{R}$ よりもベクトル空間です、そして写像 $f \mapsto Df$ は、$I$ から $E$ への写像のベクトル空間へのこの空間の線形写像です。*

#### 注意 {#fvr-i-s1-n2-rem-1 .statement tag=0832}

$I$ から $E$ への写像のベクトル空間と、微分可能な写像の部分空間 (*cf. Gen. Top.*、X、p. 277)、単純収束の位相 (または一様収束の位相)、線形写像 $f \mapsto Df$ *連続ではありません* (一般に) *たとえば、写像* の数列 $f_n(x) = \sin n^2 x / n$ *収束します*$\mathbf{R}$ では一様に 0 になりますが、*ただし導関数* $f'_n(x) = n \cos n^2 x$ の数列は *単純に * 0 にも収束しません。

#### 命題 2 {#fvr-i-s1-prop-2 .statement tag=0833}

*$E$ と $F$ を $\mathbf{R}$ にわたる 2 つのトポロジカルベクトル空間とし、$u$ を $E$ から $F$ までの連続線形写像とします。 $f$ が区間 $I \subset \mathbf{R}$ で定義されたベクトル写像で、$E$ で値を取り、点 $x_0 \in I$ で微分可能である場合、合成写像 $u \circ f$ の導関数は次のようになります。 $u(f'(x_0))$ 時刻 $x_0$.*

確かに、$\frac{u(f(x)) - u(f(x_0))}{x - x_0} = u \left( \frac{f(x) - f(x_0)}{x - x_0} \right)$ 以降、これは $u$ の連続性から生じます。

#### 系 {#fvr-i-s1-n2-cor-2 .statement tag=0834}

*$\varphi$ が $E$ で連続する線型形式である場合、実数写像 $\varphi \circ f$ は点 $x_0$ で $\varphi(f'(x_0))$ に等しい導関数を持ちます。

#### 例 1 {#fvr-i-s1-n2-exa-1 .statement tag=0835}

$f = (f_i)_{1 \leq i \leq n}$ を $\mathbf{R}^n$ の値を含む写像とし、区間 $I \subset \mathbf{R}$ で定義します。それぞれの実数写像 $f_i$ は合成写像 $\mathrm{pr}_i \circ f$ に他ならないので、$f$ があれば点 $x_0$ で微分可能であり、そうであれば $f'(x_0) = (f'_i(x_0))_{1 \leq i \leq n}$ で微分可能です。

#### 例 2 {#fvr-i-s1-n2-exa-2 .statement tag=0836}

運動学では、$f(t)$ が時間 $t$ における移動点 $M$ の位置である場合、$g(t)$ がカーネルを使用して$M$ を平面$P$ (または線$D$) に投影した$M'$ の同じ瞬間の位置である場合、線 (または平面) ではありません。 $P$ (それぞれ$D$) に平行な場合、$g$ は、$\mathbf{R}^3$ を$P$ (それぞれ$D$) と$f$ に投影した$u$ の合成です。 $u$ は (連続) 線形マッピングであるため、移動点の平面 (それぞれの線) への投影の速度は、移動点の平面 (それぞれの線) への投影の速度に等しいことがわかります。*

#### 例 3 {#fvr-i-s1-n2-exa-3 .statement tag=0837}

$f$ を区間 $I \subset \mathbf{R}$ で定義された複素数値写像とし、$a$ を任意の複素数とします。小道具。 2 は、$f$ が点 $x_0$ で微分可能である場合、$af$ も微分可能であり、この写像の $x_0$ での導関数は $af'(x_0)$ に等しいことを示しています。

### 3. 積の導関数

ここで、$\mathbf{R}$ 上の $p$ トポロジカルベクトル空間 $E_i$ ($1 \leq i \leq p$) と連続多重線形 $^1$ 写像 (これを次のように表します) を考えてみましょう。

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p])
$$

$E_1 \times E_2 \times \cdots \times E_p$ を $\mathbf{R}$ 上のトポロジカルベクトル空間 F に変換します。

#### 命題 3 {#fvr-i-s1-prop-3 .statement tag=0838}

*それぞれの添字 $i$ ($1 \leq i \leq p$) について、$f_i$ を区間 $I \subset \mathbf{R}$ で定義された写像とし、$E_i$ で値を取り、点 $x_0 \in I$ で微分可能とします。それから写像

$$
x \mapsto [f_1(x).f_2(x) \ldots f_p(x)]
$$

$F$ の値を使用して $I$ に定義された導関数は次のとおりです

$$
\sum_{i=1}^p [f_1(x_0) \ldots f_{i-1}(x_0).f'_i(x_0).f_{i+1}(x_0) \ldots f_p(x_0)]
$$

$x_0$で。

$h(x) = [f_1(x).f_2(x) \ldots f_p(x)]$ を入れてみましょう。次に、アイデンティティによって

$$
[b_1.b_2 \ldots b_p] - [a_1.a_2 \ldots a_p] = \sum_{i=1}^p [b_1 \ldots b_{i-1}.(b_i - a_i).a_{i+1} \ldots a_p],
$$

私たちは書くことができます

$$
h(x) - h(x_0) = \sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x).(f_i(x) - f_i(x_0)).f_{i+1}(x_0) \ldots f_p(x_0)].
$$

On multiplying both sides by $\frac{1}{x - x_0}$ and letting $x$ approach $x_0$ in $I$, we obtain the expression (1), since both the map

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p]
$$

F の加法は連続です。

$^1$ F への $E_1 \times E_2 \times \cdots \times E_p$ の写像 $f$ は、各部分写像の場合 *多重線形* と言われることを思い出してください (Alg.、II、p. 265)。

$$
x_i \mapsto f(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_p)
$$

$E_i$ から F ($1 \leq i \leq p$) への変換は *線型* 写像であり、添字 $j \neq i$ の $a_j$ は $E_j$ では任意です。 $E_i$ が $\mathbf{R}$ 上で *有限* 次元である場合、F への $E_1 \times E_2 \times \cdots \times E_p$ のすべての多重線形写像は必然的に *連続* であることに注意してください。これら空間のいくつかが無限次元のトポロジカルベクトル空間である場合、この必要はありません。

写像 $f_i$ の一部が定数である場合、式 (1) の項含むの導関数 $f'_i(x_0)$ は零になります。

アプリケーションで最も重要な特定のケース $p = 2$ を詳しく考えてみましょう。 $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}.\mathbf{y}]$ が $E \times F$ から $G$ への連続双線形写像であり (E、F、G は $\mathbf{R}$ 上のトポロジカルベクトル空間です)、$\mathbf{f}$ と $\mathbf{g}$ は 2 です。 ベクトル写像は、$x_0$ で微分可能で、それぞれ E と F に値があると、ベクトル写像 $x \mapsto [\mathbf{f}(x).\mathbf{g}(x)]$ ($[\mathbf{f}.\mathbf{g}]$ で表します) は、$x_0$ で$[\mathbf{f}'(x_0).\mathbf{g}(x_0)] + [\mathbf{f}(x_0).\mathbf{g}'(x_0)]$ に等しい導関数を持ちます。特に、$\mathbf{a}$ が定数ベクトルである場合、$[\mathbf{a}.\mathbf{f}]$ (それぞれ $[\mathbf{f}.\mathbf{a}]$) は、$x_0$ で $[\mathbf{a}.\mathbf{f}'(x_0)]$ (それぞれ $[\mathbf{f}'(x_0).\mathbf{a}]$) に等しい導関数を持ちます。

$\mathbf{f}$ と $\mathbf{g}$ が両方とも I で微分可能である場合、$[\mathbf{f}.\mathbf{g}]$ も微分可能であり、次のようになります。

$$
[\mathbf{f}.\mathbf{g}]' = [\mathbf{f}'.\mathbf{g}] + [\mathbf{f}.\mathbf{g}'].
$$

(2)

#### 例 1 {#fvr-i-s1-n3-exa-1 .statement tag=0839}

$f$ を実数写像、$\mathbf{g}$ ベクトル写像とし、両方とも点 $x_0$ で微分可能です。 写像 $\mathbf{g}f$ は、$x_0$ で $\mathbf{g}'(x_0)f(x_0) + \mathbf{g}(x_0)f'(x_0)$ に等しい導関数を持ちます。特に、$\mathbf{a}$ が定数の場合、$\mathbf{a}f$ は微分値 $\mathbf{a}f'(x_0)$ を持ちます。この最後の注意は、I、p. 5の例 1と組み合わせて、$\mathbf{f} = (f_i)_{1 \leq i \leq n}$がベクトル写像で、$\mathbf{R}^n$に値がある場合、$\mathbf{f}$は次で微分可能であることを証明します。 点 $x_0$ 実数写像 $f_i$ ($1 \leq i \leq n$) がそこで微分可能であることが必要かつ十分です。なぜなら、$(\mathbf{e}_i)_{1 \leq i \leq n}$ が $\mathbf{R}^n$ の標準基底である場合、$\mathbf{f} = \sum_{i=1}^n \mathbf{e}_i f_i$ と書くことができるからです。

#### 例 2 {#fvr-i-s1-n3-exa-2 .statement tag=083A}

実数写像 $x^n$ は多重線形写像から生じます

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$

$x_i$ のそれぞれを $x$ に置き換えることにより、$\mathbf{R}^n$ で定義されます。それで小道具。 3 は、$x^n$ が $\mathbf{R}$ で微分可能であり、導関数 $nx^{n-1}$ があることを示しています。その結果、多項式関数 $\mathbf{a}_0 x^n + \mathbf{a}_1 x^{n-1} + \cdots + \mathbf{a}_{n-1} x + \mathbf{a}_n$ ($\mathbf{a}_i$ は定数ベクトル) は導関数を持ちます。

$$
n \mathbf{a}_0 x^{n-1} + (n-1) \mathbf{a}_1 x^{n-2} + \cdots + \mathbf{a}_{n-1};
$$

$\mathbf{a}_i$ が実数の場合、この写像一致するは、代数 (A, IV) で定義されている多項式関数の導関数を使用します。

#### 例 3 {#fvr-i-s1-n3-exa-3 .statement tag=083B}

ユークリッドスカラー 積 $(\mathbf{x}| \mathbf{y})$ (Gen. Top 、VI、p. 40) は、$\mathbf{R}^n \times \mathbf{R}^n$ から $\mathbf{R}$ への双線形写像 (必ず連続) です。 $\mathbf{f}$ と $\mathbf{g}$ が 2 つのベクトル写像で、$\mathbf{R}^n$ に値が含まれ、点 $x_0$ で微分可能である場合、実数写像 $x \mapsto (\mathbf{f}(x)|\mathbf{g}(x))$ は、$(\mathbf{f}'(x_0)|\mathbf{g}(x_0)) + (\mathbf{f}(x_0)|\mathbf{g}'(x_0))$ に等しい導関数を持ちます。 点 $x_0$。 $\mathbf{C}^n$ のエルミートスカラー 積にも同様の結果があり、この空間は $\mathbf{R}$ に対するベクトル空間と見なされます。

特に、ユークリッドノルム $\| \mathbf{f}(x) \|$ が定数であるため、$(\mathbf{f}(x)|\mathbf{f}(x)) = \| \mathbf{f}(x) \|^2$ も定数である場合を考えてみましょう。 $(\mathbf{f}(x)|\mathbf{f}(x))$ の導関数が $x_0$ で消えると書くと、$(\mathbf{f}(x_0)|\mathbf{f}'(x_0)) = 0$ が得られます。他の語では、$\mathbf{f}'(x_0)$は$\mathbf{f}(x_0)$と直交します。

#### 例 4 {#fvr-i-s1-n3-exa-4 .statement tag=083C}

$E$ が $\mathbf{R}$ 上のトポロジー 代数 (cf. 導入) である場合、$E$ の 2 つの元のうち積 $xy$ は、$(x, y)$ の連続双線形写像です。 $\mathbf{f}$ と $\mathbf{g}$ が $E$ に値を持ち、 点 $x_0$ で微分可能である場合、 写像 $x \mapsto \mathbf{f}(x)\mathbf{g}(x)$ は $x_0$ で $\mathbf{f}'(x_0)\mathbf{g}(x_0) + \mathbf{f}(x_0)\mathbf{g}'(x_0)$ に等しい導関数を持ちます。特に、$U(x) = (\alpha_{ij}(x))$ と $V(x) = (\beta_{ij}(x))$ が $x_0$ で微分可能な位数 $n$ の 2 つの正方行列である場合、それらの積 $UV$ は $x_0$ で $U'(x_0)V(x_0) + U(x_0)V'(x_0)$ に等しい導関数を持ちます (ここで、 $U'(x) = (\alpha'_{ij}(x))$ と $V'(x) = (\beta'_{ij}(x))$)。

#### 例 5 {#fvr-i-s1-n3-exa-5 .statement tag=083D}

$n$ ベクトル $\mathbf{x}_i = (x_{ij})_{1 \leq i \leq n}$ の行列式 $\det(\mathbf{x}_1, \mathbf{x}_2, \ldots, \mathbf{x}_n)$ は空間 $\mathbf{R}^n$ (Alg., III, p. 522) から$\mathbf{x}_i$ の (連続) 多線形関数であり、$n^2$ 実数関数 $f_{ij}$ が$x_0$ で微分可能である場合、その行列式 $g(x) = \det(f_{ij}(x))$ は次と等しい導関数を持ちます。
$$
\sum_{i=1}^n \left[ \mathbf{f}_1(x_0), \ldots, \mathbf{f}_{i-1}(x_0), \mathbf{f}_i'(x_0), \mathbf{f}_{i+1}(x_0), \ldots, \mathbf{f}_n(x_0) \right]
$$
$x_0$、どこで$\mathbf{f}_i(x) = (f_{ij}(x))_{1 \leq j \leq n}$;言い換えれば、各 $i$ について、$i^{th}$ 列の項を導関数で置き換えることによって形成された $n$ 行列式の和を取ることによって、次数 $n$ の行列式の導関数を取得します。

#### 注意 {#fvr-i-s1-n3-rem-1 .statement tag=083E}

$U(x)$ が点 $x_0$ で微分可能かつ可逆的な平方行列である場合、その行列式 $\Delta(x) = \det(U(x))$ の導関数は、$U(x)$ による公式の導関数を通じて表現できます。
$$
\Delta'(x_0) = \Delta(x_0) \cdot \operatorname{Tr}(U'(x_0) U^{-1}(x_0)).
$$
確かに、$U(x_0 + h) = U(x_0) + h V$ と入れてみましょう。その後、定義までに、$h$ が 0 になる傾向があるとき、$V$ は $U'(x_0)$ になる傾向があります。
$$
\Delta(x_0 + h) = \Delta(x_0) \cdot \det(I + h V U^{-1}(x_0)).
$$
さて、$\det(I + h X) = 1 + h \operatorname{Tr}(X) + \sum_{k=2}^n \lambda_k h^k$、$\lambda_k$ ($k \geq 2$) は、行列 $X$ の元の多項式です。 $h$ が 0 になる傾向があるとき、$V U^{-1}(x_0)$ の元には極限があるため、確かに公式が得られます (3)。

### 4. 写像の逆関数の導関数

#### 命題 4 {#fvr-i-s1-prop-4 .statement tag=083F}

*Eを$\mathbf{R}$以上の単位元を持つ完全ノルム代数とし、$\mathbf{f}$を区間$I \subset \mathbf{R}$で定義された写像とし、Eで値を取り、点$x_0 \in I$で微分可能とします。 E で $y_0 = \mathbf{f}(x_0)$ が可逆 $^2$ である場合、写像 $x \mapsto (\mathbf{f}(x))^{-1}$ は (I を基準として) $x_0$ の近傍で定義され、$x_0$ で $-(\mathbf{f}(x_0))^{-1} \mathbf{f}'(x_0) (\mathbf{f}(x_0))^{-1}$ に等しい導関数を持ちます。

確かに、E の可逆元の集合は、写像 $y \mapsto y^{-1}$ が連続するオープン集合です (*Gen. Top.*、IX、p. 178)。 $\mathbf{f}$ は $x_0$ で連続 (I に対して) なので、$(\mathbf{f}(x))^{-1}$ は $x_0$ の近傍で定義され、次のようになります。
$$
(\mathbf{f}(x))^{-1} - (\mathbf{f}(x_0))^{-1} = (\mathbf{f}(x))^{-1} \left( \mathbf{f}(x_0) - \mathbf{f}(x) \right) (\mathbf{f}(x_0))^{-1}.
$$
したがって、命題は、$y_0$の近傍における$y^{-1}$の連続性と、$E \times E$における$xy$の連続性から生じます。

$^2$ (*Alg.*, I, p. 15) から、$z^{-1}$ で示される $E$ の要素が存在し、$zz^{-1} = z^{-1}z = e$ (e は $E$ の単位要素である) になる場合、要素 $z \in E$ は *反転可能*であると言われることを思い出してください。

#### 例 1 {#fvr-i-s1-n4-exa-1 .statement tag=083G}

最も重要な特別なケースは、E がフィールド $\mathbf{R}$ または $\mathbf{C}$ の 1 つである場合です。$f$ が実数値または複素数値を持つ関数で、点 $x_0$ で微分可能であり、$f(x_0) \neq 0$ である場合、$1/f$ は$x_0$ で$-f'(x_0)/(f(x_0))^2$ に等しい導関数を持ちます。

#### 例 2 {#fvr-i-s1-n4-exa-2 .statement tag=083H}

$U = (\alpha_{ij}(x))$ が位数 $n$ の平方行列で、$x_0$ で微分可能で、この点で可逆である場合、$U^{-1}$ は$x_0$ で$-U^{-1} U' U^{-1}$ に等しい導関数を持ちます。

### 5. 複合体の導関数写像

#### 命題 5 {#fvr-i-s1-prop-5 .statement tag=083I}

*$f$ を、区間 $I \subset \mathbf{R}$ で定義された実際の写像と、$\mathbf{R}$ 含む $f(I)$ の区間で定義された$g$ ベクトル写像とします。 $f$ が点 $x_0$ で微分可能であり、$g$ が点 $f(x_0)$ で微分可能である場合、合成写像 $g \circ f$ は $x_0$ で $g'(f(x_0)) f'(x_0)$ に等しい導関数を持ちます。

$h = g \circ f$ を入れましょう。 $x \neq x_0$ については次のように書くことができます
$$
\frac{h(x) - h(x_0)}{x - x_0} = u(x) \frac{f(x) - f(x_0)}{x - x_0}
$$
ここで、$f(x) \neq f(x_0)$ の場合は集合 $u(x) = \frac{g(f(x)) - g(f(x_0))}{f(x) - f(x_0)}$、それ以外の場合は $u(x) = g'(f(x_0))$ となります。現在、$f(x)$ は極限 $f(x_0)$ ですが、$x$ が $x_0$ になる傾向があるため、$u(x)$ は極限 $g'(f(x_0))$ となり、写像の連続性を考慮して命題が続きます。 $E \times \mathbf{R}$の$yx$。

### 6. 逆関数の導関数写像

#### 命題 6 {#fvr-i-s1-prop-6 .statement tag=083J}

*$f$を区間$I \subset \mathbf{R}$の区間$J = f(I) \subset \mathbf{R}$への同型写像とし、$g$を逆同型$^3$とする。 $f$ が点 $x_0 \in I$ で微分可能で、$f'(x_0) \neq 0$ の場合、$g$ は $y_0 = f(x_0)$ で $1/f'(x_0)$ に等しい導関数を持ちます。

それぞれの $y \in J$ には、$g(y) \in I$ と $u = f(g(y))$ があります。したがって、次のように書くことができます
$$
\frac{g(y) - g(y_0)}{y - y_0} = \frac{g(y) - x_0}{f(g(y)) - f(x_0)}
$$
$y \neq y_0$の場合。 $y$ が $J$ と $\neq y_0$ に留まりながら $y_0$ になる傾向がある場合、$g(y)$ は $I$ と $\neq x_0$ に残る $x_0$ になる傾向があり、前の公式の右側はこうなります。 極限 $1/f'(x_0)$、仮定 $f'(x_0) \neq 0$ 以降。

#### 系 {#fvr-i-s1-n6-cor-1 .statement tag=083K}

*$f$が$I$で微分可能であり、$f'(x) \neq 0$が$I$で微分可能である場合、$g$は$J$で微分可能であり、各点$y \in J$での導関数は$1/f'(g(y))$です。

たとえば、各整数 $n > 0$、写像 $x^{1/n}$ は、それ自体に対する $\mathbf{R}_+$ の同相写像であり、$x^n$ の逆であり、各 $x > 0$ で導関数 $\frac{1}{n} x^{\frac{1}{n} - 1}$ があります。

根拠から簡単に推測できます。 5、すべての有理数数 $r = p/q > 0$ 写像 $x^r = (x^{1/q})^p$ は、$x > 0$ ごとに導関数 $r{x'}^{-1}$ を持ちます。

$^3$ $f$ が $\mathbf{R}$ の部分集合への $I$ の同型であるためには、 $f$ が $I$ 上で連続的かつ厳密に単調であることが必要かつ十分であることがわかっています (*Gen. Top.*, IV, p. 338、第5)。

#### 注意 1 {#fvr-i-s1-n6-rem-1 .statement tag=083L}

点 $x_0$ で微分可能な写像について述べた前述のすべての命題は、写像自体の代わりに、$x_0$ で微分可能な右 (または左) である写像に対する命題を直ちに生成します。 定義の区間の制限から共通部分と区間 $[x_0, +\infty[$ (それぞれ ]$-\infty, x_0$])。それらを述べるのは読者に任せます。

#### 注意 2 {#fvr-i-s1-n6-rem-2 .statement tag=083M}

前述の定義と命題 (右導関数と左導関数に関するものを除く) 拡大するは、任意の *可換非離散位相幾何学体* $K$ と位相幾何学ベクトル空間により置き換える $\mathbf{R}$ が成り立つ場合に容易に当てはめることができます。 (それぞれトポロジカル代数) $\mathbf{R}$ によるトポロジカルベクトル空間 (それぞれトポロジカル代数) $K$ 。間違いなく。 1と小道具。 1、2、3 では、$K$ の $x_0$ の *近傍* によって置き換える I になるだけで十分です。プロップで。 4 さらに、写像 $y \mapsto y'$ が E の $f(x_0)$ の近傍上で連続していると仮定する必要があります。提案 5 は次のように一般化します: $K'$ をトポロジカル体 $K$ の非離散部分体とし、E をトポロジー ベクトル空間 *オーバー* $K$; $f$ を $x_0 \in K'$ の近傍 $V \subset K'$ で定義された写像とし、値は $K$ ($K'$ 上のトポロジカルベクトル空間とみなされる) で微分可能とします。 $x_0$、g を $f(x_0) \in K$ の近傍で定義された写像とし、E に値があり、点 $f(x_0)$ で微分可能とします。この場合、写像 $g \circ f$ は $x_0$ で微分可能であり、導関数 $g'(f(x_0))f'(x_0)$ が存在します (E はトポロジカルベクトル空間 *over* $K'$ と見なされます)。

同じ記法で、$f$ を $a \in K$ の近傍 V で定義された写像とし、値を E に置き、点 $a$ で微分可能とします。 $a \in K'$の場合、$f$から$V \cap K'$の*制限*は$a$で微分可能であり、そこに導関数$f'(a)$があります。これらの考慮事項は、実際には、特に $K = \mathbf{C}$ と $K' = \mathbf{R}$ の場合に当てはまります。

最後にプロップ。 6 拡大するは、$x_0 \in K$ の近傍による置き換える I と、$y_0 = f(x_0)$ の近傍 $J = f(I)$ への I の準同型写像による $f$ の場合です。 $K$。

### 7. 実数値写像の導関数

実数変数の *実数値* 写像を扱う場合、前述の定義と命題はいくつかの点で拡張される可能性があります。

そもそも、$f$ が区間 $I \subset \mathbf{R}$ で定義され、I に対して点 $x_0 \in I$ で連続する写像である場合、$x$ が I に留まりながら$x_0$ になる傾向があり、 $\neq x_0$、$\frac{f(x) - f(x_0)}{x - x_0}$ は $+\infty$ または $-\infty$ に等しい極限を持ちます。次に、$f$ は $x_0$ で微分可能であり、そこに導関数 $+\infty$ (それぞれ $-\infty$) があると言います。 写像 $f$ が I の点 $x$ ごとに導関数 $f'(x)$ (有限または無限) を持つ場合、 写像 $f'$ ($\overline{\mathbf{R}}$ に値が含まれる) が再び導関数と呼ばれます。 $f$ の写像 (または単に派生)。右導関数と左導関数の定義を同様に一般化します。

#### 例 {#fvr-i-s1-n7-exa-1 .statement tag=083N}

点 $x = 0$ 写像 $x^{1/3}$ ($x^3$ の逆写像、$\mathbf{R}$ のそれ自身への同型写像) には、$+\infty$ に等しい導関数があります。 $x = 0$ 写像 $|x|^{1/3}$ には右導関数 $+\infty$ と左導関数 $-\infty$ があります。

微分可能実数写像の和、積の導関数、および微分可能実数写像の逆導関数 (提案 1、3、および 4)、および写像の (実数値) 合成の導関数 (提案 5) の公式は、次の場合にも有効です。これらの式で発生するすべての式が意味をなす限り、発生する導関数は無限です (*Gen Top.*、IV、p. 345–346)。実際、プロップの場合。 6 $f$ は真に増加する (それぞれ真に減少する) で、I で連続すると仮定します。そして、$f'(x_0) = 0$ の場合、逆数写像 $g$ は、次の時点で $+\infty$ (それぞれ $-\infty$) に等しい導関数を持ちます。 点 $y_0 = f(x_0)$; $f'(x_0) = +\infty$ (それぞれ $-\infty$) の場合、$g$ の導関数は 0 になります。右導関数と左導関数についても同様の結果が得られますが、これについては読者の判断に任せます。

C を、点 $(x, f(x))$ によって形成される平面 $\mathbf{R}^2$ の有限実数写像 $f$、部分集合のグラフまたは表現曲線とします。ここで、$x$ は集合を通過し、$f$ が定義されます。 写像 $f$ が点 $x_0 \in I$ に有限の右導関数を持つ場合、C の点 $M_{x_0} = (x_0, f(x_0))$ を原点とし、方向数 $(1, f'_d(x_0))$ をもつ半線を右半接線と呼びます。 点 $M_{x_0}$ の曲線 C; $f'_d(x_0) = +\infty$ (それぞれ $f'_d(x_0) = -\infty$) の場合、原点 $M_{x_0}$ と方向数 $(0, 1)$ (それぞれ $(0, -1)$) の半直線に同じ用語を使用します。同様に、$f'_g(x_0)$ が存在する場合、$M_{x_0}$ での左半接線定義するを 1 つ作成します。これらの定義を使用すると、右（左）半接線が横軸となす角度が、Cの$M_{x_0}$と移行から点$M_1 = (x, f(x))$を通る半線とこの軸がなす角度の極限であることがすぐに確認できます。 $x$ は $> x_0$ (それぞれ $< x_0$) のままですが、$x_0$ になる傾向があります。

また、右 (それぞれ左) 半接線は、$M_{x_0}$ 移行から $M_1$ までの半線の極限であり、同じ原点を持つ半線の集合に商空間位相 $C^*/\mathbf{R}_+^*$ を与えたものであるとも言えます。 (将軍トップ、VIII、p. 107)。

2 つの半接線が C の点 $M_{x_0}$ に存在する場合、$f$ が点 $x_0$ (I の内部と仮定) に導関数 (有限であるかどうか) がある場合にのみ、それらは反対方向になります。 $f'_d(x_0)$ と $f'_g(x_0)$ が無限で符号が反対の場合にのみ同一になります。これら 2 つの場合、これら 2 つの半接線含むは点 $M_{x_0}$ における C への接線であると言います。

$M_{x_0}$ に接線が存在する場合、それは、$M_{x_0}$ と $M_1$ を通る線移行の極限です。$x$ は、指定された固定を通過する線の集合上で $x_0$ $\neq x_0$、位相に残る傾向があるためです。 点は商空間 $C^*/\mathbf{R}^*$ のものです (Gen. トップ。、VIII、p. 114）。

グラフの接線と半接線の概念は、微分可能な多様体に特化したこの系列の部分で定義される一般概念の特殊なケースです。

#### 定義 4 {#fvr-i-s1-def-4 .statement tag=083O}

We say that a real function $f$, defined on a subset A of a topological space E, has a relative maximum (resp. strict relative maximum, relative minimum, strict relative minimum) at a point $x_0 \in A$, relative to A, if there is a neighbourhood $V$ of $x_0$ in E such that at every point $x \in V \cap A$ distinct from $x_0$ one has $f(x) \leq f(x_0)$ (resp. $f(x) < f(x_0)$, $f(x) \geq f(x_0)$, $f(x) > f(x_0)$).

$f$ が A の点で A の最小値上界 (それぞれ最大の下界) に達すると、この点で A に対する相対最大値 (それぞれ相対最小値) を持つことは明らかです。 逆はもちろん間違いです。

$B \subset A$ で、$f$ が (たとえば) B に対する点 $x_0 \in B$ での相対最大値を認める場合、$f$ は必ずしもこの点で A に対する相対最大値を持たないことに注意してください。

#### 命題 7 {#fvr-i-s1-prop-7 .statement tag=083P}

$f$ を、区間 $I \subset \mathbf{R}$ で定義された有限実数写像とします。 $f$ が I の内側点 $x_0$ で相対最大値 (相対最小値) を認め、この点で右導関数と左導関数の両方を持つ場合、$f'_d(x_0) \leq 0$ と $f'_g(x_0) \geq 0$ (それぞれ $f'_d(x_0) \geq 0$ と $f'_g(x_0) \leq 0$) が得られます。特に、$f$ が点 $x_0$ で微分可能である場合、$f'(x_0) = 0$ です。

命題は定義から自明に続きます。

さらに、点 $x_0$ で I 写像 $f$ の内部が微分可能であり、相対最大値または最小値が認められる場合、そのグラフの接線は横軸に平行であると言えます。 逆は正しくありません。写像 $x^3$ の例で示されているように、点 $x = 0$ に零導関数がありますが、この点には相対最大値も最小値もありません。

### 練習問題 {#fvr-i-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
