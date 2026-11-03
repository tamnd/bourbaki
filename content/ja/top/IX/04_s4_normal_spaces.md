---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 4
section_title: Normal spaces
lang: ja
source: top-v-x
pdf_pages: 0185-0196, 0245-0255
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NORMAL SPACES
      page: 0
      pdf_page: 185
    - "no": 2
      title: EXTENSION OF A CONTINUOUS REAL-VALUED FUNCTION
      page: 0
      pdf_page: 188
    - "no": 3
      title: LOCALLY FINITE OPEN COVERINGS OF A CLOSED SET IN A NORMAL SPACE
      page: 0
      pdf_page: 191
    - "no": 4
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 193
    - "no": 5
      title: PARACOMPACTNESS OF METRIZABLE SPACES
      page: 0
      pdf_page: 194
statements: 25
exercises: 30
content_sha256: 173c8e59af13ef88178ee1a7216f21d9216dddd4dacd5dbe97234a63d064e035
translated_from: content/en/top/IX/04_s4_normal_spaces.md
translation_method: google
source_content_sha256: 9659cfc8beeaee4a3f7b73b432335f6ffd60e7f82a5d2d879d79d7ffdfda75df
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 87e9369fdcb59d62869af52e0c3569733ea14127de5dff40a94c5f4c1ea31bd3
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 通常空間

### 1. 定義の通常の空間

統一可能な空間 ($§ 1$, no. 5) の公理 ($O_{IV}$) は、次の形で記述できます: *任意の閉集合* $A$ * および任意の点* $x \in \mathbf{C}A$、*連続写像があるとしますof* $X$ *into* $[0, 1]$ *これは 0 *at* $x$ *に等しく、 $A$ の点ごとに * 1 * に等しい。この性質は再びというで表すことができ、均一化可能な空間では、点と閉じた集合 (含む点ではない) を連続実数値写像で分離できます。

ここで、同じ方法で、連続実数値写像によって閉じられた 2 つの互いに素集合を分離することができる空間を研究します。

#### 定義 1 {#top-ix-s4-def-1 .statement tag=0C5F}

*トポロジカル空間 $X$ は、ハウスドルフであり、次の公理を満たす場合に正規であると言われます:*

$(O_v)$ *$A$ と $B$ が $X$ の部分集合で閉じた 2 つの互いに素である場合、 点ごとに $0$ に等しい $X$ から $[0, 1]$ までの連続する写像が存在します。 $A$ から $B$ の点ごとに $1$ まで。*

明らかに、すべての正規空間は完全に正規です。しかし、正常ではない完全に規則的な空間もあります (練習問題 9、10、13、26 と § 5、練習問題 15、16 を参照)。

公理$(O_v)$の主張は、$(O_{IV})$と同様に、実直線$\mathbf{R}$が補助集合として含まれています。しかし、補助集合を含まない $(O_v)$ と同等の条件があります。

#### 定理 1 (ユリソーン) {#top-ix-s4-thm-1 .statement tag=0C5G}

*公理 $(O_v)$ は次と同等です:*

$(O'_v)$ *$A$ と $B$ が $X$ の 2 つの互いに素が閉じている部分集合である場合、$A \subset U$ と $B \subset V$ のように 2 つの互いに素が開いている集合 $U, V$ が存在します。

$(O_v)$ は $(O'_v)$ を暗示します。つまり、$f$ が $X$ の $[0, 1]$ への連続写像で、$A$ では $0$ に、$B$ では $1$ に等しい場合、開いた集合が続きます。 $\overline{f}^{-1}([0, 1/2[)$ と $\overline{f}^{-1}(]1/2, 1])$ 含む $A$ と $B$ は交差しません。

逆を証明するには、まず $(O'_v)$ が次の公理と同等であることに注意してください。

$(O''_v)$ *クローズド集合 $A$ と $A$ のオープン近傍 $V$ が与えられると、$\overline{W} \subset V$ となるような $A$ のオープン近傍 $W$ が存在します。

$A$ の $-1$ と $B$ の $+1$ に等しい連続写像 $f : X \to [-1, +1]$ があり、それぞれの $t \in [0, 1]$ に $U(t) = \overline{f}^{-1}([-1, t[)$ を置くと、$X$ にオープン集合のファミリーが定義され、次のようにインデックス付けされます。 $[0, 1]$、(i) $A \subset U(0)$、(ii) $B \subset \mathbf{C}U(1)$、(iii) 実数 $t, t'$ のそれぞれの対に対して、$0 \leq t < t' \leq 1$ が得られます。

$$(1)$$
$$
\overline{U}(t) \subset U(t');
$$

$U(t)$ は閉じた集合 $\overline{f}^{-1}([-1, t])$ に含まれます。 逆に、これら 3 つのプロパティ (i)、(ii)、および (iii) を使用して、オープン集合 $(0 \leq t \leq 1)$ のファミリー $(U(t))$ を定義したとします。 それぞれの $x \in X$ について、$x \in \mathbf{C}U(1)$ の場合は $g(x) = 1$ を置き、$x \in U(1)$ の場合は $g(x)$ を $x \in U(t)$ となるような $t$ の値の最大下限とします。 明らかに、$A$ では $x \in X$、$g(x) = 0$、$B$ では $g(x) = 1$ ごとに $0 \leq g(x) \leq 1$ です。また、$g$ は $X$ で連続です。なぜなら、$g(x) = a$ を置くと、すべての $y \in U(a + \varepsilon) \cap \overline{\mathbf{C}U}(a - \varepsilon)$ に対して $|g(y) - g(x)| \leq \varepsilon$ が得られます。これは、(i) による $x$ の近傍です [$a + \varepsilon > 1$ の場合は $U(a + \varepsilon) = X$、$U(a - \varepsilon) = \varnothing$ という規則に従います) $a - \varepsilon < 0$の場合]。

したがって、上記の条件 (i)、(ii)、(iii) を満たす開集合の族 $(U(t))$ を定義できれば、定理 1 が証明されます。これを行うには、公理 $(\mathrm{O}'_V)$ を使用します。 $U(1) = \mathbf{C}B$ を取ります。 $A \subset U(1)$ 以降、$(\mathrm{O}'_V)$ までに $A \subset U(o)$ と $U(o) \subset U(1)$ となるようなオープン集合 $U(o)$ が存在します。 次に、各二項数 $k/2^n$ ($k = 0, 1, \ldots, 2^n$) に対して、オープン集合 $U(k/2^n)$ を定義し、これらの集合が $0 \leq k \leq 2^n - 1$ に対して $\overline{U}(k/2^n) \subset U((k+1)/2^n)$ になると仮定します。 For each dyadic number
$$
(2k + 1)/2^{n+1} \quad (0 \leq k \leq 2^n - 1)
$$
there exists by $(\mathrm{O}'_V)$ an open set $U((2k + 1)/2^{n+1})$ such that
$$
\overline{U}(k/2^n) \subset U((2k + 1)/2^{n+1})
$$
and
$$
\overline{U}((2k + 1)/2^{n+1}) \subset U((k + 1)/2^n).
$$
Hence for each dyadic number $r$ such that $0 \leq r \leq 1$ we can define an open set $U(r)$, such that $A \subset U(o)$, $B \subset \mathbf{C}U(1)$, and
$$(2)$$
$$
\overline{U}(r) \subset U(r')
$$
for each pair of dyadic numbers $r, r'$ such that $0 \leq r < r' \leq 1$.

さて、定義する、実数 $t \in [0, 1]$ ごとに、
$$
U(t) = \bigcup_{r \leq t} U(r) \quad (r \text{ dyadic});
$$
(2) により、この定義は、前の $t$ 二進数と一致します。また、$0 \leq t < t' \leq 1$ の場合、$t \leq r < r' \leq t'$ となる 2 つの二項数 $r, r'$ が存在します。 (2) により $U(t) \subset U(r)$ となるので、
$$
\overline{U}(t) \subset \overline{U}(r) \subset U(r') \subset U(t');
$$
これで (1) が証明され、証明が完了します。

定理 1 を使用すると、トポロジカル空間の 2 つの重要なカテゴリが正規であることを示すことができます。まず第一に:

#### 命題 1 {#top-ix-s4-prop-1 .statement tag=0C5H}

*コンパクト空間は正常です。*

コンパクト空間は、章 I, § 9, no. 2 の命題 2 により、公理 $(\mathrm{O}'_V)$ を満たします。

*局所的にコンパクト* 空間に関しては、そのような空間のすべての点には、通常の部分空間であるコンパクト近傍があります。しかし、ローカルにコンパクトな空間のうち例は *正常ではありません* (cf. 練習問題 9 と 26、および § 5、練習問題 15)。

#### 命題 2 {#top-ix-s4-prop-2 .statement tag=0C5I}

*metrizable 空間は正常です。*

$X$ をメトリック化可能な空間とし、$d$ を $X$ の位相と互換性のあるメトリックとします。 Let $A, B$ be two disjoint closed subsets of $X$; since the functions $d(x, A)$ and $d(x, B)$ are continuous, the set $U$ (resp. $V$) of points $x$ such that $d(x, A) < d(x, B)$ [resp. $d(x, B) < d(x, A)$] is open; clearly $A \subset U$ and $B \subset V$ and $U \cap V = \varnothing$, hence Axiom $(O'_V)$ is satisfied.

#### 注意 1 {#top-ix-s4-n1-rem-1 .statement tag=0C5J}

命題 2 は、metrizability に他の *必須* 条件を与えます。しかし、この条件は、§ 2 で与えられたすべての必要な条件と組み合わせても、metrizability (cf. 練習問題 6 および § 5、練習問題 10) に十分な条件の集合を与えません。

#### 注意 2 {#top-ix-s4-n1-rem-2 .statement tag=0C5K}

メトリズ可能でも局所的にコンパクトでもない、通常の空間の例があります (§ 5、練習問題 16 を参照)。

$(O'_V)$ までに、通常の空間のすべての *閉じられた* 部分集合は *通常の部分空間* になります。しかし、これは通常の空間の *任意の* 部分集合には必ずしも当てはまりません。

たとえば、正規ではない完全に正規の空間は、コンパクト空間 (§ 1, no. 5, 命題 3) の部分空間と同相であり、後者は正規です。

最後に、2 つの正規空間の *積* は必ずしも正規ではないことを記録します (練習問題 9 と § 5、練習問題 16 を参照)。

### 2. 連続実数値写像の拡大

$X$ と $Y$ を 2 つのトポロジー 空間とし、$A \neq X$ を $X$ の *閉じた* 部分集合とします。 $f$が$A$から$Y$に連続する写像である場合、*拡大する*$f$から$X$全体の$Y$に連続する写像になるとは限りません。 $Y = \overline{\mathbf{R}}$ の場合、そのような拡大の可能性は次の定理によって決まります。

#### 定理 2 (ユリソーン) {#top-ix-s4-thm-2 .statement tag=0C5L}

*公理* $(O_V)$ * は次の性質* と同等です: $(O''_V)$ * 任意の閉部分集合* $A$ *of* $X$ * および任意の連続実数値写像* $f$ *(有限かどうか)* *定義済み* $A$、*拡大* $g$ *の* $f$ *全体に空間* $X$、 *これは * $X$ * $\overline{\mathbf{R}}$ の連続写像です。

$(O''_V)$ が $(O_V)$ を意味することは簡単にわかります。たとえば、$B$と$C$が$X$の部分集合に閉じた2つの互いに素である場合、$B$では0に等しく、$C$では$i$に等しい写像が定義され、閉じた集合で連続します。 $B \cup C$ なので、$(O''_{V})$ までには拡大 $f$ から $X$ が連続します。 $g = \inf (f^{+}, 1)$ の場合、$g$ は $X$ で連続し、その値を $[0, 1]$ で取得し、$B$ の $o$ と$C$ の $i$ に等しくなります。

逆に、$(O_{V})$ が $(O''_{V})$ を意味することを示してみましょう。 $\overline{\mathbf{R}}$ と区間 $[ -i, +i ]$ は同型であるため、連続する写像 $f : A \to \overline{\mathbf{R}}$ が $[ -i, +i ]$ でその値を取る場合のみを考慮する必要があります。 $X$ に連続する写像の数列 $(g_{n})$ を形成して、$f$ から $X$ までの構成する拡大 $g$ を作成し、数列 $(g_{n}(x))$ がすべて収束するようにします。 区間 $[ -i, +i ]$ の $x \in X$ から点まで。この極限は、定義までに、$x$には$g$の値になり、$g_{n}$の選択から写像$g$が必要な条件を満たすことになります。

$g_{n}$ の定義は次の補題に基づいています。

#### 補題 1 {#top-ix-s4-lem-1 .statement tag=0C5M}

*$u$を$A$から$[ -i, +i ]$への連続した写像とします。次に、$X$ から $[ -i/3, +i/3 ]$ への連続した写像 $v$ があり、すべての $x \in A$ に対して $|u(x) - v(x)| \leq 2/3$ になります。*

$H$ を、$-i \leq u(x) \leq -i/3$ となるすべての $x \in A$ の集合とし、$K$ を、$i/3 \leq u(x) \leq i$ となるすべての $x \in A$ の集合とします。 $H$ と $K$ は $A$ で閉じており、したがって $X$ で閉じており、交差しません。したがって、$(O_{V})$までに$X$の$[ -i/3, +i/3 ]$への連続写像$v$があり、これは$H$の$-i/3$、$K$の$+i/3$に等しい。 写像 $v$ は補題の条件を満たします。

現在、定義する写像 $g_{n}$ 帰納法です。 適用補題と $u = f$ を組み合わせると、定義する $g_{0}$ は、$X$ の $[ -i/3, +i/3 ]$ への連続写像となり、すべての $x \in A$ に対して $|f(x) - g_{0}(x)| \leq 2/3$ になります。ここで、$X$ から区間に写像 $g_{n}$ が連続すると仮定します。

$$
[-i + (\frac{2}{3})^{n+1}, i - (\frac{2}{3})^{n+1}]
$$

すべての $x \in A$ に対して $|f(x) - g_{n}(x)| \leq (\frac{2}{3})^{n+1}$ となるように定義されています。 適用補題から写像 $u(x) = (\frac{2}{3})^{n+1} (f(x) - g_{n}(x))$ まで、$X$ から区間までの連続した写像 $h_{n+1}$ が存在することがわかります。

$$
\left[ -\frac{2^{n+1}}{3^{n+2}}, \frac{2^{n+1}}{3^{n+2}} \right]
$$

そのような

$$
|f(x) - g_{n}(x) - h_{n+1}(x)| \leq (2/3)^{n+2}
$$

すべての$x \in A$; 帰納法は、$h_{n+1}$ の定義により、この写像がすべての $x \in X$ に対して不等式 $|g_{n+1}(x)| \leq 1 - (2/3)^{n+2}$ を満たすので、$g_{n+1} = g_{n} + h_{n+1}$ を取ることで完成します。

この定義から、$m \geq p$ と $n \geq p$ については、次のようになります。

$$
|g_{m}(x) - g_{n}(x)| \leq \frac{2^{p+1}}{3^{p+2}} \sum_{k=0}^{\infty} (2/3)^{k} = (2/3)^{p+1}
$$

それぞれ点 $x \in X$;したがって、数列 $(g_n(x))$ は、各 $x \in X$ に対するコーシー 数列であるため、区間 $[ -1, +1 ]$ の点 $g(x)$ に収束します。そして、$f(x) - g_n(x)$は$n \to \infty$と同様にすべての$x \in A$に対して0になる傾向があるため、$g$は$f$から$X$の拡大になります。したがって、$g$ が $X$ で連続していることを示すだけが残ります。

ここで、$x$ を $X$ のいずれかの点とします。次に、任意の $\varepsilon > 0$ が与えられると、すべての $y \in X$、すべての $m \geq n_0$、およびすべての $n \geq n_0$ に対して $|g_m(y) - g_n(y)| \leq \varepsilon$ となる整数 $n_0$ が存在します。したがって、$m$ を $+\infty$ にする傾向を持たせると、

$$
|g(y) - g_n(y)| \leq \varepsilon.
$$

$V$ を $x$ の近傍として、すべての $y \in V$ に対して $|g_n(y) - g_n(x)| \leq \varepsilon$ となるようにします。次に、それぞれの $y \in V$ について、

$$
|g(y) - g(x)| \leq |g(y) - g_n(y)| + |g_n(y) - g_n(x)| + |g(x) - g_n(x)| \leq 3\varepsilon,
$$

これは、$g$ が $x$ で連続し、定理 2 の証明を完了することを示しています。 (証明の最後の部分は、特定の場合に一様収束のアイデアを使用します。これについては、章 X で一般的に学習します。 no. 1.)

#### 系 {#top-ix-s4-n2-cor-1 .statement tag=0C5N}

*$f$ が $A$ で定義された有限連続実数値写像である場合、$X$ で定義された有限連続実数値写像 $g$ が存在します。これは拡大する $f$ です。

まず、すべての $x \in A$ に対して $f(x) \geq 0$ である場合を考えてみましょう。次に、$f$ から $X$ までの連続する拡大 $g_1$ があり、その値が $[0, +\infty]$ に入ります。 $B = \overline{g_1}(+\infty)$ を置くと、$B$ は閉じられ、仮定までに $A$ と一致しなくなります。したがって、$A$ では $f$ に等しく、$B$ では 0 に等しい写像 $h$ は、閉じた集合 $A \cup B$ では連続した写像になります。 $g_2$ を $h$ から $X$ までの連続した拡大とし、再び $[0, +\infty]$ でその値を取ります。 写像 $g = \inf(g_1, g_2)$ は、$f$ から $X$ までの連続拡大であり、その値は $\geq 0$ であり、$X$ の点ごとに *有限* になります。

一般的なケースに移ると、$f$ が $A$ 上で有限かつ連続である場合、$f^+$ と $f^-$ も有限で連続であることに注意するだけで十分です。 $f^+$ と $f^-$ をそれぞれ有限連続写像 $g_1$ と $g_2$ で $X$ に拡張すると、写像 $g_1 - g_2$ が $X$ と拡大する $f$ で有限連続であることがわかります。

#### 注意 {#top-ix-s4-n2-rem-1 .statement tag=0C5O}

$X$ が通常空間で、$A$ が $X$ の閉じた部分集合である場合、$A$ のすべての連続マッピング $f$ を *立方体* $K^1$ (§ 1, no. 5) にマッピングする$X$ への連続拡張も存在します。なぜなら、$f = (f_i)_{i \in I}, f_i$ は $\mathbf{R}$ のコンパクトな区間 $K$ への $A$ の連続マッピングであるからです。 $f_i$ を拡張する連続マッピング $g_i : X \to K$ が存在するため、マッピング $g = (g_i)$ は $f$ から $X$ への連続拡張です。

### 3. 通常の空間における閉じた集合の局所的に有限な開いたカバー

#### 定理 3 {#top-ix-s4-thm-3 .statement tag=0C5P}

$(A_i)_{i \in I}$ を、通常の空間 $X$ における閉じた集合 $Y$ の局所的に有限な開いたカバーとします。次に、$i \in I$ ごとに $\overline{B}_i \subset A_i$ となるように、$Y$ のオープンカバー$(B_i)_{i \in I}$ があります。

順当添字集合 $I$ (集合理論, 章 III, § 2, no. 3, 定理 1)。 $X$ でオープン集合の家族 $(B_i)_{i \in I}$ を、超限帰納法によって、次のように定義するします。 (i) 各 $i \in I$ に対して $\overline{B}_i \subset A_i$; (ii) それぞれの $i \in I$ について、$\lambda \leq i$ となるように $B_\lambda$ によって形成され、$\lambda > i$ が $Y$ の開いたカバーとなるように $A_\lambda$ によって形成されるファミリー。 (i) と (ii) がすべての $i < \gamma$ で満たされるように $i < \gamma$ の $B_i$ を定義したとします。そして、(i) と (ii) が $i = \gamma$ でも満たされるように定義する $B_\gamma$ ができることを示しましょう。まず、$i < \gamma$ に対する $B_i$ と $i \geq \gamma$ 形に対する $A_i$ が $Y$ をカバーしていることを示しましょう。 仮定までに、各 $x \in Y$ には、添字 $\lambda \in I$ の有限の数のみが存在し、$x \in A_\lambda$、たとえば $\lambda_1 < \lambda_2 < \cdots < \lambda_n$ になります。 $\lambda_h$ を $\lambda_i$ の最大のとして、$\lambda_i < \gamma$ とします。 $h < n$ の場合、$x \in A_{\lambda_n}$ と $\lambda_n \geq \gamma$ があり、$h = n$ の場合、帰納法仮定は、$x$ 属するから$B_\lambda$ への$\lambda \leq \lambda_n < \gamma$ が続き、主張が続きます。

ここで $C = (\complement Y) \cup \left( \bigcup_{i < \gamma} B_i \right) \cup \left( \bigcup_{i > \gamma} A_i \right)$ を入力します。 $C$ は開いており、これまでの話によると、$\complement A_\gamma \subset C$ が開いています。通常の空間に対する公理 $(O''_V)$ により、$\complement A_\gamma \subset \overline{V} \subset V \subset C$ となるようなオープン集合 $V$ が存在します。 $B_\gamma = \complement \overline{V}$ とすると、$\overline{B}_\gamma \subset \complement V \subset A_\gamma$ と $B_\gamma \cup C = X$ があり、$i \leq \gamma$ となるような $B_i$ と、$i > \gamma$ が $Y$ をカバーするような $A_i$ になります。

#### 注意 {#top-ix-s4-n3-rem-1 .statement tag=0C5Q}

カバー$(A_i)$ が点有限であるという事実、つまり、$X$ 属するのすべての点から集合 $A_i$ の有限の数のみを使用していることに注意してください。

#### 定義 2 {#top-ix-s4-def-2 .statement tag=0C5R}

$X$ をトポロジー 空間とし、$f$ を $X$ で定義された実数値写像とします。 $\operatorname{Supp}(f)$ で示される $f$ のサポートは、$X$ で最小のが閉じられ、集合 $S$ となり、すべての $x \notin S$ に対して $f(x) = 0$ になります。

他の語では、$\operatorname{Supp}(f)$ は、$f(x) \neq 0$ となるすべての $x \in X$ の集合の $X$ における閉包です。または、すべての $x \in X$ のうち集合であり、$x$ 含む点 $y$ のすべての近傍が $f(y) \neq 0$ になります。

$(f_i)_{i \in I}$ を、局所的に有限な族である形をサポートする $X$ 上の有限の実数値写像の族とする。次に、和 $\sum_{i \in I} f_i(x)$ が各 $x \in X$ に対して定義されます (含むは非ゼロ項の有限の数のみであるため)。 有限の実数値写像 $x \to \sum_{i \in I} f_i(x)$ は、族 $(f_i)$ の和と呼ばれ、$\sum_{i \in I} f_i$ で表されます。 それぞれの $f_i$ が連続している場合、$f = \sum_{i \in I} f_i$ も連続しています。なぜなら、$x$が$X$のいずれかの点である場合、$f_i$の有限のサポート数のみを満たす$x$の近傍$V$があり、したがって、有限部分集合$H$が存在します。 $I$ は、すべての $y \in V$ に対して $f(y) = \sum_{i \in H} f_i(y)$ となります。

#### 定義 3 {#top-ix-s4-def-3 .statement tag=0C5S}

*ファミリー* $(A_i)_{i \in I}$ *位相空間のサブセット* $X$、*ファミリー* $(f_i)_{i \in I}$ *上に定義された実数値関数* $X$ *はファミリーに従属すると言われます* $(A_i)_{i \in I}$ *ある場合* $\operatorname{Supp}(f_i) \subset A_i$ *各インデックスについて* $i \in I$。

*連続単位元の連続分割 on* $X$ *任意のファミリー* $(f_i)_{i \in I}$ *実数値連続写像* の $\geq 0$ *オン* $X$ *ローカル有限ファミリー 形をサポートし、次のようなもの* $\sum_{i \in I} f_i(x) = 1$ *すべて* $x \in X$。

#### 命題 3 {#top-ix-s4-prop-3 .statement tag=0C5T}

*局所的に有限の開いた被覆* $(A_i)_{i \in I}$ *通常の空間* $X$ が与えられると、*統一の連続分割が存在します* $(f_i)_{i \in I}$ *上* $X$、 *被覆に従属する* $(A_i)_{i \in I}$。

定理 3 までに、$i \in I$ ごとに $\overline{B}_i \subset A_i$ となるように、$X$ の開いた被覆 $(B_i)_{i \in I}$ が存在し、被覆 $(B_i)$ が局所的に有限であることは明らかです。公理$(O''_V)$によれば、各$i \in I$に対して、$\overline{B}_i \subset C_i \subset \overline{C}_i \subset A_i$となるような開いた集合$C_i$が存在します。公理$(O_V)$により、$i \in I$ごとに、$X$から$[0,1]$への連続した写像$g_i$が存在し、$\overline{B}_i$には$g_i(x) = 1$となり、$\overline{g}_i$のサポートは$\overline{C}_i$に含まれるようになります。したがって、$A_i$ に含まれます。 $(B_i)$ は $X$ をカバーしているため、$x \in X$ ごとに $\sum_{i \in I} g_i(x) > 0$ が得られます。置いたら
$$
f_i(x) = \frac{g_i(x)}{\sum_{i \in I} g_i(x)}
$$
すべての $i \in I$ とすべての $x \in X$ に対して、$f_i$ 形は、カバー$(A_i)$ に従属する単位元の連続する分割になります。

#### 系 {#top-ix-s4-n3-cor-1 .statement tag=0C5U}

*局所的に有限の開いたカバー* $(A_i)$ *閉じた集合* $F$ *通常の空間* $X$ に、 *族が存在します* $(f_i)$ *連続実数値写像* $\geq 0$ *on* $X$、 *カバーに従属する* $(A_i)_{i \in I}$ *およびそのようなもの* $\sum_{i \in I} f_i(x) = 1$ *すべてに* $x \in F$ *および* $\sum_{i \in I} f_i(x) \leq 1$ *すべてに* $x \in X$。

$CF$ の集合からなると $A_i$ の族は、$X$ の局所的に有限な開いたカバーです。したがって、このカバーに従属する単位元の連続した分割、各$i \in I$に対して$\operatorname{Supp}(f_i) \subset A_i$となるような家族$(f_i)_{i \in I}$のからなる、および$F$の補体にサポートが含まれる写像$g$が存在します。ファミリ $(f_i)$ は、要求される条件を明らかに満たしています。

### 4. パラコンパクト空間

We recall (Chapter I, § 9, no. 10) that a topological space $X$ is said to be *paracompact* if it is Hausdorff and if every open covering of $X$ has a locally finite open refinement.

#### 命題 4 {#top-ix-s4-prop-4 .statement tag=0C5V}

*すべてのパラコンパクト空間は正常です。*

これは次の補題の帰結です:

#### 補題 2 {#top-ix-s4-lem-2 .statement tag=0C5W}

*$A, B$ を、パラコンパクト空間 $X$ の 2 つの互いに素が閉じた部分集合とします。それぞれの $x \in A$ に、$x$ のオープン近傍 $V_x$ と、交差しない $B$ のオープン近傍 $W_x$ が存在する場合、$A$ のオープン近傍 $T$ とオープンが存在します。 近傍 $U$/$B$ は交差しません。*

現時点では、この補題が真実であると仮定すると、$X$ はハウスドルフであるため、$B$ が単一の点で構成されている場合に適用することができ、$X$ が *正規* であることがわかります。次に、$X$ の任意の 2 つの互いに素が閉じた部分集合に再度補題 2 を適用することができ、これは公理 $(O'_V)$ が満たされていることを示しています。

補題を証明するには、$CA$ の $X$ からなると $x \in A$ である $V_x$ のオープンカバーを考えてください。 $(T_i)_{i \in I}$ をこのカバーの局所的に有限なオープンリファインメントとします。次に、定義までに、$A \cap T_i \neq \emptyset$であれば、$T_i \subset V_{x_i}$となるような$x_i \in A$が存在します。 $T$ を、$A$ と一致する $T_i$ の和集合であるオープン集合とし、$T$ と一致しない $B$ のオープン近傍 $U$ があることを示します。それぞれの $y \in B$ には、集合 $T_i$ の有限の数のみを満たす $y$ の開いた近傍 $S_y$ があります。 $J$ を、添字 $i$ のうちの $I$ からなるの有限部分集合とし、$T_i$ が $S_y$ と $A$ の両方を満たすようにします。 $U_y = S_y \cap \bigcap_{i \in J} W_{x_i}$ とすると、$U_y$ は $A$ を満たす $T_i$ のどれにも満たない $y$ のオープン近傍となり、したがって $U_y \cap T = \emptyset$ となります。 $U = \bigcup_{y \in B} U_y$ しましょう。この場合、$U'$ は $T$ を満たさない $B$ の開いた近傍であり、補題が証明されます。

パラコンパクト(練習問題19)ではない通常の空間も存在します。

#### 系 1 {#top-ix-s4-lem-2-cor-1 .statement tag=0C5X}

*パラコンパクト空間 $X$ の開いたカバー $(A_i)_{i \in I}$ が与えられると、$x$ にはカバー $(A_i)$ に従属する単位元 $(f_i)_{i \in I}$ の連続する分割が存在します。

$(U_\lambda)_{\lambda \in L}$ を、カバー $(A_i)_{i \in I}$ を洗練する $X$ の局所的に有限な開いたカバーとします。次に、$\lambda \in L$ ごとに $U_\lambda \subset A_{\varphi(\lambda)}$ となるように写像 $\varphi : L \to I$ があります。 命題 3 と 4 までに、$(U_\lambda)$ に従属する単位元 $(g_\lambda)_{\lambda \in L}$ の連続する分割が存在します。 $i \in I$ ごとに、

$$
f_i = \sum_{\varphi(\lambda) = i} g_\lambda;
$$

この和は、局所的に有限のカバーである $g_\lambda$ 形のサポートにより定義され、連続的です。さらに、$g_\lambda$ のサポートの和集合 $B_i$ は、$\varphi(\lambda) = i$ が章 I, § 1, no. 6 の命題 4 によって閉じられ、$A_i$ に含まれるようになります。 $x \in \mathbf{C}B_i$ のときはいつでも $f_i(x) = 0$ があるため、$f_i$ のサポートは $B_i$ に含まれ、したがって $A_i$ に含まれます。一方、族 $B_i$ は局所的に有限です。なぜなら、各 $x \in X$ には、$x$ の近傍 $V$ と $I$ の有限部分集合 $H$ があり、すべての $\lambda \notin H$ に対して $V \cap U_\lambda = \emptyset$ が成り立ちます。したがって、すべての $i \notin \varphi(H)$ に対して $V \cap B_i = \emptyset$ ということになります。最後に、各 $x \in X$ について、

$$
1 = \sum_{\lambda \in L} g_\lambda(x) = \sum_{i \in I} \left( \sum_{\varphi(\lambda) = i} g_\lambda(x) \right) = \sum_{i \in I} f_i(x),
$$

そして証明が完成しました。

#### 系 2 {#top-ix-s4-lem-2-cor-2 .statement tag=0C5Y}

*F がパラコンパクト空間 X の閉じた部分集合である場合、X 含むの F のすべての近傍は F の閉じた (したがってパラコンパクト) 近傍になります。

章 I, § 9, no. 10 の命題 16 までに、X の閉じた部分空間はパラコンパクトになります。したがって、系は命題 4 と公理 $(O_v')$ から続きます。

### 5. metrizable 空間の準コンパクト性

次の定理は、no. 1 の命題 2 の結果をシャープにします。

#### 定理 4 {#top-ix-s4-thm-4 .statement tag=0C5Z}

*すべての metrizable 空間はパラコンパクトです。*

定理は、次の4つの補題のうちの帰結です。

#### 補題 3 {#top-ix-s4-lem-3 .statement tag=0C60}

*$\mathscr{R} = (U_\alpha)_{\alpha \in A}$ をメトリズ可能な空間 X のオープンカバーとします。次に、X の開いた部分集合の局所有限族の数列 $(\mathscr{G}_n)$ があり、$\mathscr{S} = \bigcup_n \mathscr{S}_n$ は $\mathscr{R}$ を洗練する X の開いたカバーになります。

$d$ を、位相と互換性のある X のメトリクスとします。それぞれの $\alpha \in A$ とそれぞれの整数 $n$ について、$F_{n\alpha}$ が $d(x, X - U_\alpha) \geq 2^{-n}$ となるように、すべての $x \in U_\alpha$ の集合を表すものとします。 $X - U_\alpha$が休みのため、$U_\alpha = \bigcup_n F_{n\alpha}$がございます。

順調です集合 $A$;それぞれの $\alpha \in A$ とそれぞれの整数 $n$ について、$G_{n\alpha}$ をすべての $x \in F_{n\alpha}$ の集合とし、すべての $\beta < \alpha$ について $x \notin F_{n+1,\beta}$ とし、$V_{n\alpha}$ をすべての $y \in X$ の集合とします。 $d(y, G_{n\alpha}) > 2^{-n-3}$。 $V_{n\alpha}$ は明らかにオープン集合です。一方、$V_{n\alpha} \subset U_\alpha$ は、$y \in V_{n\alpha}$ ごとに $d(x, y) \leq 2^{-n-1}$ のような $x \in G_{n\alpha}$ が存在し、$x \in F_{n\alpha}$ 以降、

$$
d(y, X - U_\alpha) \geq d(x, X - U_\alpha) - d(x, y) \geq 2^{-n-1},
$$

だから$y \in U_\alpha$。さらに、各 $x \in X$ について、$A$ で $\alpha$ を最小の添字とし、$x \in U_\alpha$ とします。次に、$x \in F_{n\alpha}$ となるような整数 $n$ があり、$\alpha$ の定義は $x \in G_{n\alpha}$ を暗示し、したがって $x \in V_{n\alpha}$ になります。これは、$\mathfrak{S}_n = (V_{n\alpha})_{\alpha \in A}$ を置くと、$\mathfrak{S} = \bigcup_n \mathfrak{S}_n$ は $\mathscr{R}$ を洗練する $X$ のオープンカバーであることを示しています。したがって、各族 $\mathfrak{S}_n$ が *局所的に有限*であることはまだ示されていません。この目的のために、まず、$\alpha \neq \beta$ の場合、$d(G_{n\alpha}, G_{n\beta}) \geq 2^{-n-1}$ であることを示します。 $\beta < \alpha$; と仮定します。 $x \in G_{n\alpha}$ と $y \in F_{n\beta}$ の場合、定義によって $x \notin F_{n+1,\beta}$ が得られるため、$d(x, X - U_\beta) < 2^{-n-1}$ と $d(y, X - U_\beta) \geq 2^{-n}$、したがって $d(x, y) \geq 2^{-n-1}$ になります。 $G_{n\beta} \subset F_{n\beta}$ 以降、主張が続きます。これから、$V_{n\alpha}$ と $V_{n\beta}$ の定義を使用して、$d(V_{n\alpha}, V_{n\beta}) \geq 2^{-n-2}$ がすぐに続きます。この最後の不等式から、各 $z \in X$ について、中心 $z$ と半径 $2^{-n-3}$ のオープンボールは、ファミリー $\mathfrak{S}_n$ の最大 1 つの集合と一致すると推測します。したがって、$\mathfrak{S}_n$ は局所有限族であり、証明は完全です。

#### 補題 4 {#top-ix-s4-lem-4 .statement tag=0C61}

*$(\mathfrak{S}_n)$ * をトポロジカル空間* $X$ の開いた集合の局所有限族の数列とする、*次のような*
$$
\mathfrak{S} = \bigcup_n \mathfrak{S}_n
$$
*は* $X$のカバーです。 *その後、局所的に有限な (ただし必ずしも開いているわけではない) カバー* $\mathscr{B}$ *of* $X$ *これが *$\mathfrak{S}$ を洗練する* ことが存在します。

$E_n$ を、$\mathfrak{S}_n$ のすべての集合の和集合である $X$ のオープン集合とします。 $U_n$ は $\bigcup_{k=1}^n E_k$ を表し、$A_n$ は $U_n - U_{n-1}$ ($U_0 = \varnothing$ を含む) を表します。 部分集合 $V \cap A_n$ の集合 $\mathscr{B}$ を考えてみましょう。ここで、$V \in \mathfrak{S}_n$ と $n$ は任意の整数です。 $\mathscr{B}$ が補題の条件を満たすことを示します。 それぞれの $x \in X$ には、$X$ の $A_n$ 形分割から、$x \in A_n$ となる整数 $n$ があります。したがって、$x \in E_n$ となり、$x \in V$ となるような $V \in \mathfrak{S}_n$ が存在します。したがって、$x \in V \cap A_n$、そして$\mathscr{B}$が$X$のカバーであることが証明されました。 明らかに、このカバーは $\mathfrak{S}$ を洗練します。 一方、各 $x \in X$ には、$x \in U_n$ となる整数 $n$ が存在します。 $U_n$ はオープンで、$\mathfrak{S}_m$ はローカル有限ファミリーであるため、$U_n$ に含まれる各 $m$ に対して、$\mathfrak{S}_m$ の集合の有限数のみを満たす $x$ の近傍 $W_m$ が存在します。したがって、$p > n$ に対する $W \cap A_p = \varnothing$ のため、$x$ の近傍 $W = \bigcap_{m=1}^n W_m$ は、$\mathscr{B}$ の集合の有限数のみと一致します。 したがって、$\mathscr{B}$ は局所有限であり、補題 4 が証明されます。

#### 補題 5 {#top-ix-s4-lem-5 .statement tag=0C62}

*$X$ *を正規の空間とし、各開いたカバー* $\mathscr{R}$ *of* $X$ に対して、*(必ずしも開いているとは限らない) 局所的に有限なカバー* $\mathscr{U}$ *of* $X$ *これをリファインする* $\mathscr{R}$ が存在するようにします。 *その後、各開いたカバー* $\mathscr{R}$ *of* $X$ *局所的に有限の閉じたカバー* $\mathfrak{F}$ *of* $X$ *これを洗練* $\mathscr{R}$ します。

$\mathfrak{R}$ を $X$ のオープンカバーとします。それぞれの $x \in X$ には、含む $x$ のオープン集合 $U \in \mathfrak{R}$ があり、したがって ($X$ が規則的であるため) $x$ のオープン近傍 $V_x$ は、$\overline{V}_x \subset U$ のようになります。 $V_x$ によって形成される族 $\mathscr{B}$ は、$X$ の開いたカバーであるため、仮定までに、$\mathscr{B}$ よりもより細かいである局所有限カバー $\mathscr{B}'$ が存在します。 $\mathscr{F}$ を $\mathscr{B}$ の集合の閉包ファミリーとします。 $\overline{V}_x$によって形成される覆い$\mathscr{B}'$は$\mathfrak{R}$よりより細かいであり、$\mathscr{F}$は$\mathscr{B}'$よりより細かいであるため、$\mathscr{F}$は$\mathfrak{R}$を洗練する$X$の閉じた覆いであることがわかります。しかし、$\mathscr{F}$ も局所的に有限です。なぜなら、開いた集合が集合 $B \in \mathscr{B}$ を満たさない場合、その閉じ $\overline{B}$ も満たさないからです。

#### 補題 6 {#top-ix-s4-lem-6 .statement tag=0C63}

*$X$ をハウスドルフ空間とし、$X$ の開いたカバー $\mathfrak{R}$ が与えられると、$\mathfrak{R}$ を洗練する $X$ の局所的に有限な閉じたカバー $\mathscr{F}$ が存在します。次に、$X$ はパラコンパクトです。*

$\mathfrak{R}$ を $X$ のオープンカバーとします。 $\mathfrak{R}$ を洗練する $X$ の局所的に有限な開いたカバーが存在することを示さなければなりません。 $\mathscr{A}$ を、$\mathfrak{R}$ を洗練する $X$ の局所的に有限なカバー (閉じているかどうか) とします。それぞれの $x \in X$ について、$W_x$ を $\mathscr{A}$ の集合の有限数のみを満たす $x$ の開いた近傍とします。 集合 $W_x$ のファミリー $\mathscr{W}$ は、$X$ のオープンカバーです。 $\mathscr{F}$ を、$\mathscr{W}$ を洗練する $X$ の局所的に有限な *閉じた * カバーとする。それぞれの $A \in \mathscr{A}$ について、$U_A$ を含む $A$ である $\mathfrak{R}$ の集合とし、$C_A$ を $A \cap F = \varnothing$ となる集合 $F \in \mathscr{F}$ の和集合とします。 $\mathscr{F}$ は局所的に有限であるため、$C_A$ は $X$ (章 I, § 1, no. 6, 命題 4) で閉じられており、したがって $A' = U_A \cap (X - C_A)$ は開いています。 $A \cap C_A = \varnothing$ と $A \subset U_A$ があるので、$A \subset A'$ が成り立ち、集合 $A'$ のファミリー $\mathscr{A}'$ は、$A$ が $\mathscr{A}$ を通るので、$X$ のオープンカバーになります。さらに、$A' \subset U_A \in \mathfrak{R}$ なので、$\mathscr{A}'$ は $\mathfrak{R}$ を洗練します。 $\mathscr{A}'$ が *局所的に有限*であることを示すことはまだ残っています。それぞれの $x \in X$ には、$x$ の近傍 $T$ があり、これは $\mathscr{F}$ の集合の有限の数、たとえば $F_1, \ldots, F_n$ とのみ一致します。それぞれの $F_i$ は形 $W_{y_i}$ の集合に含まれるため、定義 $F_i$ は $\mathscr{A}$ の集合の有限の数とのみ一致します。 $A_{ij}$ ($1 \leq j \leq s_i$) をこれらの集合とします。 $A$ が $A_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq s_i$) の 1 つ以外の $\mathscr{A}$ の集合である場合、定義から、$A'$ は $F_i$ のいずれにも満たされず、したがって $T \subset \bigcup_{i=1}^n F_i$ も満たされないことがわかります。これで、補題 6 の証明と定理 4 が完了します。

### 練習問題 {#top-ix-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
