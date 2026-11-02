---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 1
section_title: PRIMITIVES AND INTEGRALS
lang: ja
source: fvr-i-vii
book_pages: 51-62, 79-84
pdf_pages: 0066-0077, 0094-0099
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIMITIVES
      page: 51
      pdf_page: 66
    - "no": 2
      title: EXISTENCE OF PRIMITIVES
      page: 52
      pdf_page: 67
    - "no": 3
      title: REGULATED FUNCTIONS
      page: 53
      pdf_page: 68
    - "no": 4
      title: INTEGRALS
      page: 56
      pdf_page: 71
    - "no": 5
      title: PROPERTIES OF INTEGRALS
      page: 59
      pdf_page: 74
    - "no": 6
      title: INTEGRAL FORMULA FOR THE REMAINDER IN TAYLOR'S FORMULA; PRIMITIVES OF HIGHER ORDER
      page: 62
      pdf_page: 77
statements: 28
exercises: 23
content_sha256: 54867ce470cebb33cf9a2d8986acede0f316c6b08b4916d5b647938a63900b0b
translated_from: content/en/fvr/II/01_s1_primitives_and_integrals.md
translation_method: google
source_content_sha256: 966025e49c722d33da4fca08c6c4f13c4514b7e1ed5ae715959b710f37572bbe
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: eae5f1f33b8ec3df4dd729a4d265ea6d1d273df749154f81525cce13182b31db
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。原始関数と積分

〜でない限りは反対のことを明示的に述べていますが、この章では、$\mathbf{R}$ に対する完全な正規化空間で値を取る実数変数のベクトル写像のみを考慮します。特に実数値写像を扱う場合、これらの写像は反対に述べられた有限 〜でない限りであることが常に理解されます。

### 1. プリミティブの定義

ベクトル写像 $f$ は区間 $I \subset \mathbf{R}$ できないで定義され、ベクトル写像 $g$ のこの区間の点ごとの微分になります (定義され連続です)。 $I$) 〜でない限りは非常に厳しい条件を満たします: たとえば、$f$ が点 $x_0$ で$I$ の内側に右極限と左極限を認める場合、$f$ は以下の点で連続でなければなりません。 点 $x_0$、プロップより以下の通り。 I、p. 18の6つ。したがって、$I$ に対して区間 $[ -1 , 1 ]$ を、$f$ に対して実際の写像が $[ -1 , 0[$ の $-1$ と $[0 , 1]$ の $+1$ に等しい場合、$f$ は次の導関数ではないということになります。 $I$ の連続する写像;同じように、写像 $|x|$ は、点 $\neq 0$ ごとに導関数として $f(x)$ を持ちます。したがって、人は次のようなことをするように導かれます定義:

#### 定義 1 {#fvr-ii-s1-def-1 .statement tag=0870}

*区間 $I \subset \mathbf{R}$ に定義されたベクトル写像 $f$ を考えると、$g$ が連続であれば、$I$ に定義された写像 $g$ は $f$ のプリミティブであると言います。 $I$ であり、$I$ の可算部分集合の補数 ($I$ に関して) 点 $x$ ごとに$f(x)$ に等しい導関数があります。*

また、$g$ が $I$ の点 $x$ ごとに $f(x)$ に等しい導関数を認める場合、$g$ は $f$ の厳密な原始関数であると言われます。

この定義により、上で検討した実際の写像 $f$ が $|x|$ に等しいプリミティブを許容することがわかります。

$f$ が $I$ のプリミティブを認める場合、$f$ のすべてのプリミティブは、$I$ の可算数部分集合の点を除いて、$f$ に等しいすべての写像のプリミティブでもあることは明らかです。言葉の乱用により、$I$ の可算部分集合の補数 ($I$ に関して) のみで定義された写像 $f_0$ の $I$ の原始関数について話します。これは、上で定義されたすべての写像 $f$ の原始関数になります。 $I$ であり、$f_0$ が定義されている点の $f_0$ に等しい。

#### 命題 1 {#fvr-ii-s1-prop-1 .statement tag=0871}

*$f$ を $I$ で定義されたベクトル写像とし、$E$ では値を定義します。 $f$ が $I$ 上のプリミティブ $g$ を認める場合、$I$ 上の $f$ のプリミティブの集合は、写像 $g + a$ の集合と同一になります。ここで、$a$ は定数写像 $E$の値。*

実際、$g + a$ が任意の $a \in E$ に対して $f$ のプリミティブであることは明らかです。一方、$g_1$ が $f$ のプリミティブである場合、$g_1 - g$ は、$I$ の可算数部分集合の点を除いて 0 に等しい導関数を許容し、したがって定数 (I、p. 17、系) になります。

写像 $f$ のプリミティブ (存在する場合) は「加法定数まで」定義されると言われています。 $f$ のプリミティブ定義するには、点 $x_0 \in I$ で (恣意的に) 値を明確に割り当てるだけで十分です。特に、$g(x_0) = 0$ となるような $f$ のプリミティブ $g$ が 1 つだけ存在します。 $f$ のすべてのプリミティブ $h$ に対して 1 つは $g(x) = h(x) - h(x_0)$ を持ちます。

### 2. プリミティブの存在

$f$ を任意の区間 $I \subset \mathbf{R}$ で定義された写像とします。 $I$ で定義された写像 $g$ が $f$ のプリミティブであるためには、すべてのコンパクト区間 $J \subset I$ に対する $g$ の制限が $f$ の制限のプリミティブであることが必要かつ十分です。 $J$。

#### 定理 1 {#fvr-ii-s1-thm-1 .statement tag=0872}

*$A$ をフィルター $\mathfrak{F}$ でフィルターした集合とし、$(f_\alpha)_{\alpha \in A}$ を区間で定義された$\mathbf{R}$ 上の完全ノルム空間 $E$ 内の値を含むベクトル写像のファミリーとします。 $I \subset \mathbf{R}$: それぞれの $\alpha \in A$ について、$g_\alpha$ を $f_\alpha$ のプリミティブとします。次のように仮定します。
1. フィルター $\mathfrak{F}$ 写像 $f_\alpha$ は、$I$ ～ 写像 $f$ のすべてのコンパクト部分集合に均一に収束します。
2. 点 $a \in I$ があり、フィルター $\mathfrak{F}$ に関して、ファミリー $(g_\alpha(a))$ は $E$ に極限を持ちます。
これらの仮説の下では、写像 $g_\alpha$ は、$I$ のすべてのコンパクト部分集合で$f$ のプリミティブ $g$ に（$\mathfrak{F}$ に関して）一様に収束します。

この小節の冒頭の注意によって、$I$ が *コンパクト* 区間である場合に限定できます。

まず、$g_\alpha$ が $I$ で連続的な写像 $g$ に一様に収束することを示します。 仮定までに、$\varepsilon > 0$ ごとに集合 $M \in \mathfrak{F}$ があり、添字 $\alpha, \beta$ 所属から $M$ までの 2 つについて、$x \in I$ ごとに 1 つが $\|f_\alpha(x) - f_\beta(x)\| \leq \varepsilon$ になります。 帰結には (I, p. 15, th. 2) があります。

$$
\|g_\alpha(x) - g_\beta(x) - (g_\alpha(a) - g_\beta(a))\| \leq \varepsilon |x - a| \leq \varepsilon l
$$

ここで、$l$は$I$の長さを表します。 $g_\alpha(a)$ が $\mathfrak{F}$ に対して仮定までに極限に近づくため、コーシーの基準から、$g_\alpha$ は$I$ に一様に収束します。 $g_\alpha$ の極限 $g$ が $f$ のプリミティブであることを示すことが残っています。

それぞれの整数 $n > 0$ について、$\alpha_n$ を添字として、$I$ に $\|f(x) - f_{\alpha_n}(x)\| \leq 1/n$ が来るようにします。 数列 $(f_{\alpha_n})$ が $f$ に一様に収束し、 数列 $(g_{\alpha_n})$ が $I$ で $g$ に一様に収束することは明らかです。 $H_n$を$I$の可算部分集合とし、$f_{\alpha_n}$は$g_{\alpha_n}$の導関数ではなく、$H$を$H_n$の和集合とし、したがってIの可算部分集合とします。 所属から H 写像までではなく、点 $x \in I$ ごとに、g は $f(x)$ に等しい導関数を持つことがわかります。実際、上記のように、$m \geq n$ および $y \in I$ ごとに、

$$
\| g_{\alpha_m}(y) - g_{\alpha_m}(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|.
$$

$m$ を無限に増加させると、次のようになります。

$$
\| g(y) - g(x) - (g_{\alpha_n}(y) - g_{\alpha_n}(x)) \| \leq \frac{2}{n} |y - x|
$$

$y \in I$ごとに;現在、$h > 0$ が存在し、$|y - x| \leq h$ と $y \in I$ には $\| g_\alpha(y) - g_{\alpha_n}(x) - f_{\alpha_n}(x)(y - x) \| \leq |y - x| / n$ が含まれます。一方、$\| f(x) - f_{\alpha_n}(x) \| \leq 1 / n$ があるので、最終的に次のようになります。

$$
\| g(y) - g(x) - f(x)(y - x) \| \leq \frac{4}{n} |y - x|
$$

$y \in I$ と $|y - x| \leq h$ は、証明を完了します。

#### 系 1 {#fvr-ii-s1-thm-1-cor-1 .statement tag=0873}

* I から E への写像の集合 $\mathscr{H}$ は、区間 I のプリミティブを許可します。これは、完全なベクトル空間 $\mathscr{F}_c(I; E)$ の閉じた (したがって完全な) ベクトル部分空間です。 I から E への写像は、I* (*Gen. Top.*、X、p. 277) のすべてのコンパクト部分集合に一様収束の位相が付与されています。

#### 系 2 {#fvr-ii-s1-thm-1-cor-2 .statement tag=0874}

*$x_0$ を I の点とし、それぞれの写像 $f \in \mathscr{H}$ について、$P(f)$ を点 $x_0$ で消える $f$ の原始値とします。 写像 $f \mapsto P(f)$ の $\mathscr{H}$ から $\mathscr{F}_c(I; E)$ は連続した線形写像です。*

コル。 1からthまで。 1 では、次の手順で写像の特定のカテゴリに対するプリミティブの存在を確立できます。 $\mathscr{F}_c(I; E)$ の写像所属から部分集合 $\mathscr{A}$ がプリミティブを認めることがわかっている場合、写像所属は、$\mathscr{F}_c(I; E)$ の *閉包* になります。 ベクトル部分空間は $\mathscr{A}$ によって生成されました。この方法を次の小節に適用します。

### 3. 規制対象写像

#### 定義 2 {#fvr-ii-s1-def-2 .statement tag=0875}

*One says that a map $f$ of an interval $I \subset \mathbf{R}$ into a set E is a step function if there is a partition of I into a finite number of intervals $J_k$ such that $f$ is constant on each of the $J_k$.*

$(a_i)_{0 \leq i \leq n}$ を、$J_k$ の個別の端点によって形成される真に増加する数列とします。 $J_k$ はペアの互いに素であるため、それぞれがシングルトン $a_i$ に対する簡約するか、エンドポイントとして 2 つの連続する点 $a_i, a_{i+1}$ を持つ区間です。さらに、I は $J_k$ の和集合であるため、点 $a_0$ は左側の端点、$a_n$ は I の右側の端点です。したがって、I のすべてのステップ写像は、オープン区間 ]$a_i,\ a_{i+1}[\ (0 \leq i \leq n - 1)$ のそれぞれで一定である写像として特徴付けることができます。ここで、$(a_i)_{0 \leq i \leq n}$ は、$I$ の点の真に増加する数列です。 $a_0$ は $I$ の左側のエンドポイント、$a_n$ は右側のエンドポイントです。

#### 命題 2 {#fvr-ii-s1-prop-2 .statement tag=0876}

*The set of step functions defined on $I$, with values in a vector space $E$ over $\mathbf{R}$, is a vector subspace $\mathscr{E}$ of the vector space $\mathscr{F}(I; E)$ of all maps of $I$ into $E$.*

実際、$f$ と $g$ を 2 つのステップ写像とし、$(A_i)$ と $(B_j)$ を $I$ の 2 つの分割から区間の有限数にすると、$f$ (それぞれ$g$) になります。それぞれの $A_i$ (それぞれ $B_j$) で一定です。 実数 $\lambda, \mu$ が何であれ、空でない区間 $A_i \cap B_j$ のそれぞれで $\lambda f + \mu g$ が一定であること、および $I$ の区間形分割が一定であることは明らかです。

#### 系 {#fvr-ii-s1-n3-cor-1 .statement tag=0877}

*ベクトル部分空間 $\mathscr{E}$ は、区間の特性写像によって生成されます。

Now let us consider the case where $E$ is a normed space over $\mathbf{R}$; it is then immediate that the characteristic function of an interval $J$ with endpoints $a, b$ ($a < b$) admits a primitive, namely the function equal to $a$ for $x \leq a$, to $x$ for $a \leq x \leq b$, and to $b$ for $x \geq b$. コル。支柱に。したがって、2 は、*$E$ の値を含むすべてのステップ写像がプリミティブ* を受け入れることを示しています。

これで、n' 2 で方法集合を適用できるようになりました。

#### 定義 3 {#fvr-ii-s1-def-3 .statement tag=0878}

*ある人は、区間 $I$ で定義され、$\mathbf{R}$ 上の空間 $E$ で値が定義されているベクトル写像は、ステップの均一極限であれば、規制された写像であると言われています。 $I$ のすべてのコンパクト部分集合に写像。*

他の語では、規制されている写像は、ステップ写像の部分空間$\mathscr{E}$の$\mathscr{F}_c(I; E)$における閉鎖の元です。 $\overline{\mathscr{E}}$ は $\mathscr{F}_c(I; E)$ のベクトル部分空間であり、$\mathscr{F}_c(I; E)$ が完了しているため、$\overline{\mathscr{E}}$ も完了しています。他の語では、写像が$I$の各コンパクト部分集合で規制されている写像の均一極限である場合、$I$で規制されます。 区間 $I$ に$f$ が規制されるためには、その制限から $I$ に含まれるすべてのコンパクト区間が規制されることが必要かつ十分です。

コル。 I ～ II、p. 53 は次を示します。

#### 定理 2 {#fvr-ii-s1-thm-2 .statement tag=0879}

*区間 $I$ で規制されているすべての写像は、$I$ でのプリミティブを許可します。*

我々は変換絶対に勝ちます。 II、p. 4 ～ 他ののうちの 3 つが同等のもの:

#### 定理 3 {#fvr-ii-s1-thm-3 .statement tag=087A}

*区間 $I$ で定義されたベクトル写像 $f$ について、$\mathbf{R}$ を超えた空間 $E$ が完全に基準化された値を備えている場合、規制されるには、右極限と左極限があれば十分であり、これらの点属するから $I$ のとき、$I$ のすべての内部点に極限、$I$ の左側の端点に右側極限が、$I$ の右側の端点に左側極限が配置されます。したがって、$I$ における $f$ の不連続の点の集合は可算です。*

すべての区間はコンパクトな区間の可算和集合であるため、証明番目までに制限できます。 3 I がコンパクトな場合、I = [a, b] とします。

1条件が必要です。 f が規制されており、x が b とは異なる I の点であると仮定します。 仮定までに、すべての ε > 0 に対して \|f(z) - g(z)\| となるようなステップ写像 g が存在します。 I のすべての z に対して \leq \varepsilon; g は点 x で権利極限を持っているため、x < y \leq b となる y が存在し、点 z, z' の区間 ]x, y] のすべての対に対して \|g(z) - g(z')\| が成立します。 \leq \varepsilon、および帰結 \|f(z) - f(z')\| \leq 3\バレプシロン;これは (コーシーの基準によって) f が点 x で権利極限を持っていることを証明します。同様に、f には a とは異なる I の点ごとに左極限があることが証明されます。

2° 条件で十分です。それが満たされていると仮定します。 I の x \in ごとにオープン区間 V_x = ]c_x, d_x[ 含む x があり、I の共通部分にはオープン区間 ]c_x, x[, ]x, d_x[ (共通部分が空でない場合) が存在します。 f の振動は \leq \varepsilon です。 I はコンパクトなので、I には点 x_i の有限の数があり、V_{x_i} 形は I のカバーになります。 (a_k)_{0 \leq k \leq n} を点 a, b とそれら点 x_i, c_{x_i} と d_{x_i} で構成される有限集合を増加する位数点に並べて数列とします。 属するから I まで。それぞれの区間 ]a_k, a_{k+1}[ (0 \leq k \leq n - 1) は区間 ]c_{x_i}, x_i[ または ]x_i, d_{x_i}[ に含まれており、f の振動は \leq \varepsilon です。 c_k を ]a_k, a_{k+1}[ の f の値の 1 つとします。 0 \leq k \leq n に対して g(a_k) = f(a_k)、すべての x \in に対して g(x) = c_k を代入すると、]a_k, a_{k+1}[ (0 \leq k \leq n - 1)、\|f(z) - g(z)\| となる 1 つの定義する a ステップ写像 g \leq \varepsilon I;したがって、f はI に規制されます。

最後に、f が I で規定されている場合、不連続性の点の集合が可算であることを示します。すべての n > 0 に対して、\|f(x) - g_n(x)\| となるステップ写像 g_n が存在します。 \leq 1/n I; 数列 (g_n) は I で f に一様に収束するため、g_n がすべて連続である場合、f は点ごとに連続であることがわかります (Gen. Top.、X、p. 281、cor. 1)。しかし、g_n は有限集合 H_n の点を除いて連続であるため、f は集合 H = \bigcup_{n} H_n の補数の点で連続であり、これは可算であることになります。

#### 系 1 {#fvr-ii-s1-thm-3-cor-1 .statement tag=087B}

f を I の規制された写像とします。 I のすべての点で、I の右側の端点 (左側の端点) を除いて、f のすべてのプリミティブは f(x+) に等しい右導関数 (または f(x-) に等しい左導関数) を持ちます。特に、f が連続である点 x ごとに、f(x) はそのプリミティブの 1 つの微分になります。

これは明らか帰結です。 II、p. 54、およびプロップの 3 つ。 I、p. 18の6。

#### 系 2 {#fvr-ii-s1-thm-3-cor-2 .statement tag=087C}

f_i (1 \leq i \leq n) が区間 I で写像に制御され、各 f_i が \mathbf{R} (1 \leq i \leq n) 上の完全ノルム空間 E_i でその値を持つものとします。 g が \prod_{i=1}^{n} E_i の部分空間 \prod_{i=1}^{n} \overline{f_i(I)} の連続写像であり、 \mathbf{R} 上の完全ノルム空間 F である場合、合成写像 x \mapsto g(f_1(x), f_2(x), \ldots, f_n(x)) はI で規制されています。

確かに、条件を明らかに満たしています。 II、p. 54 の 3 つ。

したがって、f が I 上で規定されたベクトル写像である場合、実数写像 x \mapsto \|f(x)\| であることが分かります。も規制されています。さらに、実質は I 形環に写像が規制されました。

さらに、$f$ と $g$ が 2 つの実際の規制対象写像である場合、$\sup(f, g)$ と $\inf(f, g)$ が規制されます。

#### 注意 1 {#fvr-ii-s1-n3-rem-1 .statement tag=087D}

$f$ が $I$ で実際に規制されている写像であり、$g$ が区間含む $f(I)$ で規制されているベクトル写像である場合、複合写像 $g \circ f$ は必ずしも規制されているわけではありません($cf.$ II、p. 79、練習問題 4)。

特定の 2 つのケース。 II、p. 54 の 3 つは特に重要です。

#### 命題 3 {#fvr-ii-s1-prop-3 .statement tag=087E}

*区間 $I \subset \mathbf{R}$ 上のすべての連続ベクトル写像は、$\mathbf{R}$ 上の完全ノルム空間 $E$ の値が規制されており、$I$ での原始関数が認められ、その原始関数はすべて点での微分になります。

#### 注意 2 {#fvr-ii-s1-n3-rem-2 .statement tag=087F}

連続写像がプリミティブを受け入れることを示すには、実数変数 ($E$ の係数を含む) のすべての *多項式関数* がプリミティブを受け入れるという事実を使用できます。 Weierstrass の定理 (*Gen. Top.*、X、p. 313、提案 3) から、すべての連続写像は、すべてのコンパクト区間上の多項式の一様極限です。 II、p. 52 の 1 は、すべての連続する写像がプリミティブを受け入れることを示しています。

#### 注意 3 {#fvr-ii-s1-n3-rem-3 .statement tag=087G}

前述の注意拡大するの原則を、$\mathbf{C}$ で完全に正規化された空間で値を取る *複雑* 変数のベクトル写像に大幅な変更を加えません。 $U$ が $\mathbf{C}$ の開いた集合で、$\mathbf{C}$ と同同型である場合、$U$ で定義されたそのようなベクトル写像 $f$ の *プリミティブ* は、定義による連続写像です。 $U$、$U$ の点ごとに $f$ に等しい導関数を持ちます。 With this definition, th. 1 of II, p. 52 extends without modification (one proves, using the connectedness of $U$, that $(g_\alpha)$ is uniformly convergent with respect to $\mathscr{F}$ on a neighbourhood of each point of $U$, from which it follows that $(g_\alpha)$ is uniformly convergent with respect to $\mathscr{F}$ on every compact subset of $U$; the proof is completed using prop. 4 of I, p. 18). その結果、$U$ のすべてのコンパクト部分集合上の多項式の *一様な極限* であるすべての写像は、$U$ 上の原始関数を受け入れます。これらの写像は、$U$ の *正則* と呼ばれる写像に他なりません。これについては、後の本でさらに詳しく学びます。

#### 命題 4 {#fvr-ii-s1-prop-4 .statement tag=087H}

*区間 $I \subset \mathbf{R}$ 上のすべての単調実数写像 $f$ は規制されており、$f$ のすべてのプリミティブは $I$ に凸です。

確かに、$f$ は th の基準を満たします。 *Gen の 3トップ。*、IV、p. 350、プロップ。 4; 命題の 2 番目の部分は cor から続きます。 1、II、p. 55、プロップから。 I、p. 27 の 5。

#### 注意 4 {#fvr-ii-s1-n3-rem-4 .statement tag=087I}

区間 $I$ で規制されている写像が、$I$ ($cf.$ II、p. 80、練習問題 7 および 8) にプリミティブを持つ唯一の写像であると考えてはなりません。

### 4. 整

ステップ写像のプリミティブの統一極限として、区間 $I$ で規制された写像のプリミティブ (II, p. 54, th. 2) を取得しました。この手順は、少し異なる方法で表現できます。$x_0, x$ を、$x_0 < x$ となるような $I$ の任意の 2 つの点とします。 区間 $[x_0, x]$ 区間 $[x_i, x_{i+1}]$ の任意の数列を和集合 $[x_0, x]$ で * サブディビジョン* と呼びます。ここで、$(x_i)_{0 \leq i \leq n}$ は真に増加する数列の点です。 $[x_0, x]$ は $x_n = x$ になります。 I で定義されたベクトル写像 $f$ と、$[x_i,\ x_{i+1}]$ によって形成される下位区分、形の任意の式に対して * リーマン和* と呼ぶことにします。
$$
\sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i)
$$
ここで、$t_i$ 属するから $[x_i,\ x_{i+1}]$ は $0 \leq i \leq n-1$ です。すると、次の命題になります。

#### 命題 5 {#fvr-ii-s1-prop-5 .statement tag=087J}

*$f$を区間Iの規制された写像、$g$をIの$f$のプリミティブ、$[x_0,\ x]$をIに含まれるコンパクトな区間とする。 $\varepsilon > 0$ ごとに数 $\rho > 0$ が存在し、$[x_0,\ x]$ を長さ $\leq \rho$ の区間に分割するたびに、*
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon
$$
*(1)*
*この区画を基準としたすべてのリーマン和に対して。*

実際、$f_1$ を、$y \in [x_0,\ x]$ ごとに $\|f(y) - f_1(y)\| \leq \varepsilon$ となるようなステップ写像とします。 1 つは、$g_1$ による I 上の $f_1$ のプリミティブを示し、
$$
\|g(x) - g(x_0) - (g_1(x) - g_1(x_0))\| \leq \varepsilon(x - x_0)
$$
ちなみに値定理、そしてその一方で
$$
\left| \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) - \sum_{i=0}^{n-1} f_1(t_i)(x_{i+1} - x_i) \right| \leq \varepsilon(x - x_0).
$$

したがって、$f$ が *ステップ写像* であるとき、命題を証明するだけで十分です。 $(y_k)_{1 \leq k \leq m}$ を $[x_0,\ x]$ における $f$ の不連続点の点の真に増加する有限列とします。 $[x_0,\ x]$ を長さ $\leq \rho$ の区間に分割するたびに、点 $y_k$ 属するを最大 2 つ区間に分割します。したがって、$f$ が一定ではない$2m$ 区間を超えることはできません。しかし、そのような区間 $[x_i,\ x_{i+1}]$ では、
$$
\|g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i)\| \leq 2M (x_{i+1} - x_i)
$$
$[x_0,\ x]$ の $\|f\|$ の最小値上界を $M$ で表す場合。一方、$f$ が $[x_i,\ x_{i+1}]$ で一定の場合、次のようになります。
$$
g(x_{i+1}) - g(x_i) - f(t_i)(x_{i+1} - x_i) = 0.
$$
したがって、違いがわかります
$$
\left| g(x) - g(x_0) - \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i) \right|
$$
できないは $4Mm\rho$ を超えます。したがって、(1) を得るには $\rho \leq \varepsilon / 4Mm$ かかるだけで十分です。

#### 注意 1 {#fvr-ii-s1-n4-rem-1 .statement tag=087K}

$f$ が *連続* プロパティの場合。 5はより簡単に証明できます。$f$は$[x_0,\ x]$上で一様連続であるため、$[x_0,\ x]$に含まれる長さ$\leq \rho$の区間ごとに$f$の振動が$\leq \frac{\varepsilon}{x - x_0}$となるような$\rho > 0$が存在します。 $[x_0,\ x]$ の長さ $\leq \rho$ の区間 $[x_i,\ x_{i+1}]$ と、$[x_i,\ x_{i+1}]$ の $t_i$ のすべての選択について、$0 \leq i \leq n-1$ のステップ写像 $f_1$ は次と等しくなります。 $[x_i,\ x_{i+1}]$ ($0 \leq i \leq n-1$) の $f(t_i)$ と点の $f(x)$ x は、$[x_0, x]$ の $\| f(y) - f_1(y) \| \leq \frac{\varepsilon}{x - x_0}$ になります。 $g_1$ が $f_1$ のプリミティブである場合、次のようになります。
$$
g_1(x) - g_1(x_0) = \sum_{i=0}^{n-1} f(t_i)(x_{i+1} - x_i),
$$
したがって、関係 (1) は平均値値定理からすぐに続きます。

この章の残りでは、区間 I の *規制* 写像のプリミティブの研究に限定します。 For such a function $f$, with values in E, a primitive $g$ of $f$, and for two arbitrary points $x_0, x$ of I, the element $g(x) - g(x_0)$ of E (which is clearly the same, no matter which primitive $g$ of $f$ one considers) is called the *integral of the function* $f$ *from* $x_0$ *to* $x$ (or *over the compact interval* $[x_0, x]$) and is denoted by $\int_{x_0}^x f(t) dt$ or $\int_{x_0}^x f$. この名前と記法の由来はプロップにあります。 II、p. 57 の 5。これは、積分がリーマン和によって任意に近似できることを示します。より具体的には、$[x_0, x]$ の細分を区間に等しくすると、次のように書くことができます。

$$
\frac{1}{x - x_0} \int_{x_0}^x f(t) dt = \lim_{n \to \infty} \frac{1}{n} \sum_{k=0}^{n-1} f \left( x_0 + k \frac{x - x_0}{n} \right).
$$

他の語では、元 $\frac{1}{x - x_0} \int_{x_0}^x f(t) dt$ は、$[x_0, x]$ を区間に等しく分割する区間の左側の端点における$f$ の値の *算術平均* の極限です。 区間 $[x_0, x]$ の写像 $f$ の *平均値* (または *平均値*) とも呼ばれます。

定義までに、写像 $x \mapsto \int_{x_0}^x f(t) dt$ は、点 $x_0 \in I$ で消滅する $f$ のプリミティブに他なりません。 $\int_{x_0}^x f(t) dt$ または $\int_{x_0}^x f$ で表すこともあります。

#### 注意 2 {#fvr-ii-s1-n4-rem-2 .statement tag=087L}

I で定義された任意の写像 $h$ の場合、E に値が含まれている場合、元 $h(x) - h(x_0)$ は $h(t)\Big|_{x_0}^x$ としても書き込まれます。この記法により、$g$ が I 上の規制された写像 $f$ のプリミティブである場合、次のことがわかります。

$$
\int_{x_0}^x f(t) dt = g(t)\Big|_{x_0}^x.
$$

#### 注意 3 {#fvr-ii-s1-n4-rem-3 .statement tag=087M}

式 $\int_{x_0}^x f(t) dt$ と $g(t)\Big|_{x_0}^x$ は、$t$ ではなく$x, x_0, f, g$ という文字が現れるアセンブリを表す省略記号です (*cf. 集合理論*、I、p. 15)。これらの記号のうち、$t$ は「*ダミー変数*」であると言う人もいます。したがって、そのようにして得られた記号の意味を変えることなく、$x, x_0, f$ と $g$ (およびこれらの記号が出現する証明に入る可能性のある変数) とは異なる他の変数によって置き換える $t$ を求めることができます (読者はこれらの記号を次のような記号と比較することができます) $\sum_{i=1}^n x_i$、または $\bigcup X_i$、$i$ も同様にダミー変数です)。

#### 注意 4 {#fvr-ii-s1-n4-rem-4 .statement tag=087N}

リーマンによる積分の近似和は、積分概念の歴史的起源の 1 つである面積の *尺度 * 問題と密接に関係しています。 この問題が導く積分概念の一般化に特化した「積分に関する本の」のこの点に戻りましょう。これらの一般化写像が「*統合*」されることは、必ずしも $\mathbf{R}$ の部分集合で定義されるわけではありません。さらに、(必ずしも規制されていない) 実数変数の (必ずしも規制されていない) 実数写像 $f$ を扱う場合でも、定義する積分 $\int_{x_0}^x f(t)\,dt$、写像 $x \mapsto \int_{x_0}^x f(t)\,dt$ が常に $f$ の原始値であるとは限らず、原始値を持ちながらもそうでない写像が存在します。私たちがほのめかしている意味での「統合可能」。

### 5. 積分の性質

規制された写像の積分の特性は、第 1 章で示された導関数の特性を適切な記法に単純に変換したものです。 I。

まず、公式 (3) は、I の点 $x,\ y,\ z$ が何であっても、

$$
\int_x^x f(t)\,dt = 0 \tag{4}
$$

$$
\int_x^y f(t)\,dt + \int_y^x f(t)\,dt = 0 \tag{5}
$$

$$
\int_x^y f(t)\,dt + \int_y^z f(t)\,dt + \int_z^x f(t)\,dt = 0 \tag{6}
$$

プロップから。 II、p. 52 の 1 つが持っています

$$
\int_{x_0}^x (f + g) = \int_{x_0}^x f + \int_{x_0}^x g \tag{7}
$$

そしてすべてのスカラー $k$ について

$$
\int_{x_0}^x k f = k \int_{x_0}^x f. \tag{8}
$$

E、Fを$\mathbf{R}$上の2つの完全ノルム空間、uをEからFへの連続線形写像とする。 fがEの値を伴うIの規制された写像である場合、$u \circ f$はIの規制された写像であり、 F の値 (II、p. 6、cor. 2)、および 1 つは $a, b \in I$ (I、p. 13、prop. 2) です。

$$
\int_a^b u(f(t))\,dt = u \left( \int_a^b f(t)\,dt \right). \tag{9}
$$

ここで、E、F、G を 3 つの完全ノルム $\mathbf{R}$ で空間とし、$(x, y) \mapsto |x.y|$ を G への $E \times F$ の連続双線形写像とします。 f と g を 2 つのベクトル写像で定義し、I で連続し、それぞれ E と F で値を取るものとします。さらに、f と g が *規制* 写像の 2 つのプリミティブであるとします。これを言語の乱用により $f'$ と $g'$ で表します (これらの写像は、可算数集合の補数を除いて、実際にはそれぞれ f と g の導関数と等しいことが保証されていません)。 プロップにより。 I、p. 6、写像 $h(x) = [f(x).g(x)]$ の 3 は、I の可算部分集合の補数の点ごとに、$[f(x).g'(x)] + [f'(x).g(x)]$ に等しい導関数を持ちます。 さて、$[x.y]$ と cor の連続性により、 II、p. 55、写像、$[f.g']$、$[f'.g]$ のそれぞれは、I で規制されている写像です。つまり 1 つは公式です

$$
\int_a^b [f'(t).g(t)]\,dt = [f(t).g(t)]\Big|_a^b - \int_a^b |f(t).g'(t)|\,dt \tag{10}
$$

部分* による統合を表す *公式と呼ばれ、多くのプリミティブを評価できるようになります。

たとえば、部分による積分に対して公式を実行すると、次の公式が得られます。

$$
\int_{x_0}^{x} t f'(t) \, dt = t f(t) \Big|_{x_0}^{x} - \int_{x_0}^{x} f(t) \, dt
$$

したがって、2 つの写像 $f(x)$ と $x f'(x)$ の一方のプリミティブの評価を他方に減らします。

同様に、$f$ と $g$ が区間 $I$ で $n$ 回微分可能であり、$f^{(n)}$ と $g^{(n)}$ が $I$ で写像規制されている場合、公式 (5) I、p. 21 は次と同等です。

$$
\int_a^b [f^{(n)}(t) \cdot g(t)] \, dt
$$
$$
= \left( \sum_{p=0}^{n-1} (-1)^p [f^{(n-p-1)}(t) \cdot g^{(p)}(t)] \right) \Bigg|_a^b + (-1)^n \int_a^b [f(t) \cdot g^{(n)}(t)] \, dt
$$
(11)

これは、位数 n* の部分による積分のために *公式を呼び出します。

合成写像 (I, p. 9, 提案 5) を微分するために公式を翻訳しましょう。 $f$ を、$I$ で定義され連続する実際の写像とします。これは、$I$ で *規制されている* 写像 (言葉の乱用により、再び $f'$ と書きます) のプリミティブです。さらに、$g$ を、オープン区間 $J$ 含む $f(I)$ 上で *連続* ベクトル写像 (値が完全正規化空間である) とします。 $h$ が $J$ 上の $g$ の任意のプリミティブを表す場合、$h$ は $J$ の各点で $g$ に等しい導関数を許容します (II、p. 56、props 3)。したがって、合成写像 $h \circ f$ は、$I$ の可算部分集合の補数 ($I$ に関して) 点で$g(f(x)) f'(x)$ に等しい導関数を認めます (I, p. 9、提案 5)。 写像 $g(f(x)) f'(x)$ は規制されているため (II、p. 55、cor. 2)、公式と書くことができます。

$$
\int_a^b g(f(t)) f'(t) \, dt = \int_{f(a)}^{f(b)} g(u) \, du
$$
(12)

これは、変数 * の変更を *公式と呼び、プリミティブの評価も容易にします。

たとえば、$f(x) = x^2$ を取ると、写像 $g(x)$ と $x g(x^2)$ のプリミティブの評価が公式 (12) 簡約するになることがわかります。

実数の規制された写像のプリミティブの平均値定理 (I, p. 14, th. 1) を変換するには、まず、コンパクト区間 $I$ 上の実数の規制された写像 $f$ に注目します。 $I$ に境界があります。 $J$ を点の $I$ の集合とし、$f$ を *連続* とし、$m = \inf_{x \in J} f(x)$、$M = \sup_{x \in J} f(x)$ を置きます。人は、$I \cap \mathbf{C}J$ が可算であることを知っています (II, p. 54, th. 3)。さらに、$B$が$I$に関して、$I$の可算部分集合と$m' = \inf_{x \in B} f(x)$、$M' = \sup_{x \in B} f(x)$の補数である場合、$m' \leq m \leq M \leq M'$が得られます。実際、点$x \in J$ごとに、 B の点 $y$ は任意に $x$、よって $m' \leq f(y) \leq M'$ に近い。 $f$ は点 $x$ で連続しているため、$y$ が $x$ ($y$ は B に残る) に近づくため、$m' \leq f(x) \leq M'$ となり、主張が証明されます。したがって、平均値定理を翻訳すると、次の命題が得られます。

#### 命題 6 (平均値の定理) {#fvr-ii-s1-prop-6 .statement tag=087O}

*$f$ をコンパクト区間 $l = [a, b]$ の実際の規制された写像とします。 $J$ が I の点の集合で、$f$ が連続で、$m = \inf_{x \in J} f(x)$、$M = \sup_{x \in J} f(x)$ の場合、*

$$
m < \frac{1}{b-a} \int_a^b f(t)\,dt < M
$$

*(13)*

*$f$ が J 上で定数である場合を除きます。この場合、(13) の 3 つのメンバーは等しいです。*

他の語では、Iの規制された写像$f$の*平均*は、$f$が連続であるIの部分集合にわたる$f$の境界の間にあります。

#### 系 1 {#fvr-ii-s1-prop-6-cor-1 .statement tag=087P}

*I で実際に規制されている写像 $f$ が、$f$ が連続である点で $f(x) \geq 0$ である場合、* $\frac{1}{b-a} \int_a^b f(t)\,dt > 0$ *〜でない限り* $f(x) = 0$ *点で、$f$ * は連続です*。

#### 系 2 {#fvr-ii-s1-prop-6-cor-2 .statement tag=087Q}

*Let $f$ and $g$ be two real regulated functions on I, such that $g(x) \geq 0$ *at the points where* $g$ *is continuous; if* $m$ *and* $M$ *are the greatest lower bound and least upper bound of* $f$ *over the set of points where* $f$ *is continuous, then*

$$
\frac{m}{b-a} \int_a^b g(t)\,dt \leq \frac{1}{b-a} \int_a^b f(t)g(t)\,dt \leq \frac{M}{b-a} \int_a^b g(t)\,dt.
$$

*(14)*

*最初の 2 つ項 (それぞれ最後の 2 つ) は等しくありません 〜でない限り* $g(x)(f(x) - m) = 0$ *(それぞれ $g(x)(f(x) - M) = 0$) 点ここで* $f$ *と* $g$ *は連続です*。

ベクトル写像の平均値定理 (I、p. 15、th. 2) は次の命題を生成します。

#### 命題 7 {#fvr-ii-s1-prop-7 .statement tag=087R}

*$\mathbf{f}$ * をコンパクトな区間* $I = [a, b]$ 上の規制されたベクトル写像とし、*完全な基準の空間* $E$ にある値と *そして* $g$ *実際の規制された写像とします* $I$、*そのような* $g(x) \geq 0$ *点ここで* $g$ *は連続です。このような状況では*

$$
\left\| \int_a^b \mathbf{f}(t)g(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| g(t)\,dt.
$$

*(15)*

*特に、*

$$
\left\| \int_a^b \mathbf{f}(t)\,dt \right\| \leq \int_a^b \| \mathbf{f}(t) \| \,dt.
$$

*(16)*

### 6. テイラーの公式の残りを積分公式;上位位数のプリミティブ

The formula for integration by parts of order $n$ (II, p. 60, formula (11)) allows one to express in terms of an integral the remainder $r_n(x)$ in the Taylor expansion of order $n$ of a function which admits a regulated $(n+1)^{th}$ derivative on an interval I (I, p. 22); indeed, on replacing, in (12), $f$ by $f'$, $b$ by $x$, and $g(t)$ by the function $(t-x)^n/n!$, it follows that

$$
f(x) = f(a) + f'(a) \frac{(x-a)}{1!} + f''(a) \frac{(x-a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x-a)^n}{n!} + \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt
$$

その他語

$$
r_n(x) = \int_a^x f^{(n+1)}(t) \frac{(x-t)^n}{n!} \, dt,
$$

公式により、多くの場合、残りの単純な境界を取得できます。

区間 I に規制された写像 $f$ が与えられると、$f$ の任意のプリミティブ $g$ は、I で連続しており、その順番でプリミティブを受け入れます。 $f$ の任意のプリミティブの任意のプリミティブは、$f$ の *2 番目のプリミティブ*と呼ばれます。より一般的には、$f$ の位数 $n-1$ のプリミティブは、$f$ の位数* $n$ の * プリミティブと呼ばれます。 $n$ の帰納法までに、$f$ の位数 $n$ の 2 つの原始関数の差が、$n-1$ (E には係数を含む) に等しい * 次数の * 多項式であることがすぐにわかります。 $f$ の位数 $n$ の原始関数は、その値とその最初の $n-1$ 派生関数の点 $a \in I$ を指定すると完全に決定されます。

特に、$\int_a^{(n)} f$ は、$f$ の位数 $n$ のプリミティブを示し、その最初の $n-1$ 導関数とともに点 $a$ で消滅します。 位数 $n-1$ のテイラー 公式をこのプリミティブに適用すると、$g = \int_a^{(n)} f$ の場合、

$$
g(x) = \int_a^x f(t) \frac{(x-t)^{n-1}}{(n-1)!} \, dt
$$

したがって、位数 $n$ のプリミティブの決定が 1 つの積分に減ります。

### 練習問題 {#fvr-ii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
