---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 2
section_title: INTEGRALS OVER NON-COMPACT INTERVALS
lang: ja
source: fvr-i-vii
book_pages: 62-68, 84-86
pdf_pages: 0077-0083, 0099-0101
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 62
      pdf_page: 77
    - "no": 2
      title: INTEGRALS OF POSITIVE FUNCTIONS OVER A NON-COMPACT INTERVAL
      page: 66
      pdf_page: 81
    - "no": 3
      title: ABSOLUTELY CONVERGENT INTEGRALS
      page: 67
      pdf_page: 82
statements: 9
exercises: 9
content_sha256: 8c05c743efb885574baa24ac932fb9be329f848062899046c9f2c6c86bc6096d
translated_from: content/en/fvr/II/02_s2_integrals_over_non_compact_intervals.md
translation_method: google
source_content_sha256: c9b52ed8d14396c752cf882b9999823a887d9dfcc853a8cd546dc7a96f2d2721
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2a21547a9877923661874b621d50b67d4129ca522e56d6d34f06c9f534ceaa15
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。非コンパクト上の積分区間

### 1. 非コンパクト上の積分の定義区間

I を *拡張線* $\overline{\mathbf{R}}$ のコンパクトな区間 $[a,\ b]$ とします ($a$ と $b$ は無限になる可能性があります)。 $f$ を $[a,\ b[$ で定義された写像とし、その値を $\mathbf{R}$ 上の完全ノルム空間 E に取ります。 Generalizing def. 1 of II, p. 51, we shall say that a function $g$, defined on $[a,\ b]$ with values in E, is a *primitive* of $f$ if it is continuous on $[a,\ b]$ (and in particular at the endpoints $a$ and $b$) and admits a derivative equal to $f(x)$ at all the points of the complement with respect to $[a,\ b[$ of a countable subset of this interval.

次の場合に限定します: $I = [a,\ b]$ の点の有限真に増加する数列 $(c_i)_{0 \leq i \leq n}$ が存在し、$c_0 = a,\ c_n = b$ が存在し、$f$ が開いた区間 $[c_i,\ c_{i+1}[$ のそれぞれで *規制* されます。 けれども区間含む点 $c_i$ $I$ の内部を少なくとも 1 つ開くすべてのけれどもが規制されるわけではありません。このような写像は、$[a,\ b[$ に *区分的に規制* されます。 $[a,\ b[$ の規制された写像は区分的に規制されていることに注目します (前の定義で $n = 1$ を取る)。

$f$ が原始値 $g$ (上で正確に説明した意味で) を認め、$c$ が区間 $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$ の点である場合、仮定までに、この区間の各 $x$ に対して、その $g(x) - g(c) = \int_c^x f(t)\,dt$ が得られます。 $g$は$I$で仮定まで連続しているため、$x$が右から$c_i$になる傾向があり、$x$が左から$c_{i+1}$になる傾向があるとき、$\int_c^x f(t)\,dt$は$E$で極限になる傾向があることがわかります。逆に、これらの条件がすべての $t$ に対して満たされると仮定し、$g_i$ を区間 $[c_i,\ c_{i+1}[\ (0 \leq i \leq n - 1)$ 上の $f$ のプリミティブとします。直ちに、$c_i$の集合の$I$の補数で条件によって定義された写像$g$は、$0 \leq i \leq n - 1$の$[c_i,\ c_{i+1}[$の$g_i(x) + \sum_{k=1}^i (g_{k-1}(c_k-) - g_k(c_k+))$に等しいことが、どの時点でも連続であることに注意します。 $I$ の点は $c_i$ とは異なり、これらの点のそれぞれに極限が認められます。したがって、これらの点のそれぞれへの連続性によって拡張でき、拡張された写像は明らかに $I$ 上の $f$ のプリミティブです。さらに、$f$ の他のすべてのプリミティブは形 $g + a$ ($E$ の $a$ 元) であることは明らかです。

#### 定義 1 {#fvr-ii-s2-def-1 .statement tag=088F}

*ある人は、ベクトル写像* $f$、*区間* $[a,\ b[$ *of* $\overline{\mathbf{R}}$ で*区分的に規制され、*この区間について積分を認める* $f$ *$[a,\ b[$* について原始演算を認める。 if* $g$ * が * $f$ *on* $[a,\ b[$* のプリミティブのいずれか 1 つであり、* $x_0$ * および* $x$ * が * $[a,\ b[$* の任意の 2 つの点である場合、 *1 つは元* $g(x) - g(x_0)$ * の積分* $f$ *から* $x_0$ *から* $x$、*そして1はそれを* $\int_{x_0}^x f(t)\,dt$で表します。

この概念は、区間 $[x_0,\ x]$ 含む点 $c_i$ のいずれでもない場合に定義された概念と明らかに一致します。

defの前にある注意。 1 は、$f$ が $[a,\ b[$ で積分を持つためには、その制限から区間 $[c_i,\ c_{i+1}[$ がこの区間にわたる積分を許容する必要があり、十分であることを示しています。他の語では、$f$ が *非コンパクト* 区間 $I \subset \mathbf{R}$ で規制されており、エンドポイント $a,\ b$ ($a < b$) の場合に 1 つの簡約するが適用されます。 1 数 $a,\ b$ (時点)最小）は無限です。 2 または $f$ は、コンパクト区間含む点 $a,\ b$ の少なくとも 1 つでは規制されていません (これら 2 つの仮説は相互に排他的ではありません)。 $f$が$I$の積分を持つためには、点$(x,\ y)$が$I \times I$のままで$(a,\ b) \in \overline{\mathbf{R}}^2$に近づくとき、整$\int_a^x f(t)\,dt$が極限に近づくことが必要かつ十分です。そして、この極限は$\int_a^b f(t)\,dt$に他なりません。デフによると。 1. 言葉の乱用により、$f$ が $I$ に対して積分を持つというというの代わりに、整 $\int_a^b f(t)\,dt$ は *収束* (または *収束*) であると言います。

#### 例 {#fvr-ii-s2-n1-exa-1 .statement tag=088G}

i) 整$\int_1^{+\infty} dt/t^2$ は収束し、1 に等しくなります。
$$
\int_1^x \frac{dt}{t^2} = 1 - \frac{1}{x}.
$$

2) 整$\int_0^1 dt / \sqrt{t}$ は収束し、2 に等しくなります。
$$
\int_1^x \frac{dt}{\sqrt{t}} = 2(1 - \sqrt{x}) \quad \text{for} \quad x > 0.
$$

3) $(\mathbf{u}_n)_{n \geq 1}$ を E の点の無限大数列とし、$\mathbf{f}$ を区間 $[1, +\infty[$ 上で条件によって定義されたステップ写像とします: $n \leq x < n+1$ に対する $\mathbf{f}(x) = \mathbf{u}_n$。次に、整 $\int_1^{+\infty} \mathbf{f}(t)\,dt$ が収束するには、系列と一般項 $\mathbf{u}_n$ が E で *収束* することが必要かつ十分です。確かに、人は持っています
$$
\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p,
$$
したがって、条件が必要です。逆に、系列と一般的な項 $\mathbf{u}_n$ が E に収束すると、$\lim_{n \to \infty} \mathbf{u}_n = 0$ になります。今、$n \leq x \leq n+1$ の場合、$\int_1^n \mathbf{f}(t)\,dt = \sum_{p=1}^{n-1} \mathbf{u}_p + \mathbf{u}_n(x-n)$ があります。したがって、$x$ が $+\infty$ になる傾向があるとき、この積分は極限 $\sum_{n=1}^{\infty} \mathbf{u}_n$ になります。

明らかは、区分的に調整された写像 $\mathbf{f}$ が I にわたる積分を許容する場合、II、p. 59 の式 (4) ～ (9) が有効なままであるということです。同様に、II、p. 59 拡大するの公式 (10) は、次のようになります: $\mathbf{f}$ と $\mathbf{g}$ は、$]a,\ b[$ 上の規制された写像 $\mathbf{f}'$ と $\mathbf{g}'$ のプリミティブであると想定されます。 $(x,\ y)$ は ($a < x \leq y < b$ とともに) $(a,\ b)$ になる傾向があるため、$[\mathbf{f}.\mathbf{g}]|_x^y$ の $[\mathbf{f}.\mathbf{g}]|_a^b$ 極限 (存在する場合) を表します。この場合、$[\mathbf{f}.\mathbf{g}]|_a^b$、$\int_a^b [\mathbf{f}(t).\mathbf{g}'(t)]\,dt$、$\int_a^b [\mathbf{f}'(t).\mathbf{g}(t)]\,dt$ の 3 つの式のうち 2 つが意味を持つ場合、3 つ目も意味があり、II、p. 59 の公式 (10) が有効になります。

最後に、$f$ を、$I = ]a,\ b[$ で定義され連続する実数の写像とし、$]a,\ b[$ で規制された写像 $f'$ のプリミティブとします。一方、$g$ を、開いた区間 J 含む $f(I)$ 上で連続するベクトル写像とします。 写像 $g(f(x))f'(x)$ が I に関する積分を許容し、$f$ が点 $a$ および $b$ で極限 (有限であるかどうかにかかわらず) になる傾向がある場合、$g$ は $f(a+)$ からの積分を許容します。 $f(b-)$ まで、そして 1 つは公式です
$$
\int_a^b g(f(t))f'(t)\,dt = \int_{f(a+)}^{f(b-)} g(u)\,du.
$$
実際、$(x,\ y)$ が $(a,\ b)$ になる傾向がある場合、$(f(x),\ f(y))$ は仮定までに $(f(a+),\ f(b-))$ になる傾向があります。 $x$と$y$の間にII、p. 60の公式(12)を適用し、極限に渡して(1)を得るだけで十分です。

非コンパクト区間 $I \subset \mathbf{R}$ で規制された写像 $\mathbf{f}$ が与えられ、エンドポイント $a$ および $b$ ($a < b$) を使用すると、I を超える積分を持つ $\mathbf{f}$ に対する条件を提示できます。以下の方法で。 $[ \alpha , \beta ]$ と $[ \gamma , \delta ]$ が $I$ に含まれる 2 つのコンパクト区間である場合、関係 $\subset ^1$ に対するコンパクト区間 $J \subset I$ 形は *有向集合* $\mathscr{K}(I)$ となります。 $\lambda = \min(\alpha, \gamma)$、$\mu = \max(\beta, \delta)$とすると、区間 $[ \lambda , \mu ]$は、考慮された2つの区間のうち、$I$と含むに含まれます。 $I$ に含まれる各コンパクト区間 $J = [ \alpha , \beta ]$ について、

$$
\int_J f(t) \, dt = \int_\alpha^\beta f(t) \, dt;
$$

$f$ が $I$ の積分を認めるには、写像 $J \mapsto \int_J f(t) \, dt$ が有向集合 $\mathfrak{K}(I)$ に関して極限を持つことが必要かつ十分です。この極限は積分 $\int_a^b f(t) \, dt$ であり、これを再び $\int_I f(t) \, dt$ で表します。

#### 命題 1 (積分に対するコーシーの基準) {#fvr-ii-s2-prop-1 .statement tag=088H}

*$f$ を、エンドポイント $a$ および $b$ ($a < b$) を持つ区間 $I \subset \mathbf{R}$ の規制された写像とします。整 $\int_a^b f(t) \, dt$ が存在するには、すべての $\varepsilon > 0$ に対して、$I$ に含まれるコンパクト区間 $J_0 = [\alpha, \beta]$ が存在することが必要かつ十分です。つまり、どのコンパクト区間 $K = [x, y]$ も $I$ に含まれ、共通のには内部点が存在しません。 $J_0$ の場合、1 つは $\| \int_K f(t) \, dt \| \leq \varepsilon$ になります。*

実際、$E$ が完全であるため、コーシー基準は、整 $\int_I f(t) \, dt$ が収束するには、任意の $\varepsilon > 0$ に対して、$J_0 \subset J \subset I$ が $\| \int_J f(t) \, dt - \int_{J_0} f(t) \, dt \| \leq \varepsilon$ を持つような、すべてのコンパクト区間 $J$ を伴うコンパクト区間 $J_0 = [\alpha, \beta]$ が存在することが必要かつ十分であることを示しています。 命題は次の補題から続きます:

#### 補題 {#fvr-ii-s2-n1-lem-1 .statement tag=088I}

※$J_0 = [\alpha, \beta]$を$I$に含まれる圧縮区間とする。 位数では、$I$ と含む $J'$ に含まれるコンパクト区間 $J, J'$ の対ごとに $\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \| \leq \varepsilon$ が$\| \int_K f(t) \, dt \| \leq \varepsilon$ である必要があり、すべてのコンパクトに対して $\| \int_K f(t) \, dt \| \leq \varepsilon / 2$ があれば十分です。 区間 $K$ は $I$ に含まれており、共通のには$J_0$ の内部点がありません。*

確かに、$J_0 \subset J \subset I$ と $J_0 \subset J' \subset I$ の場合、次のようになります。

$$
\left\| \int_J f(t) \, dt - \int_{J'} f(t) \, dt \right\| \leq \varepsilon
$$

特に、$x \leq y \leq \alpha$ または $\beta \leq x \leq y$ ($I$ の $x$ と $y$) については、$\| \int_x^y f(t) \, dt \| \leq \varepsilon$ があることがわかります。逆に、$K \cap J_0 = \emptyset$ のようなすべてのコンパクト区間 $K \subset I$ に対して $\| \int_K f(t) \, dt \| \leq \varepsilon / 2$ があり、$J = [x, y]$、$J' = [z, t]$ が $I$ と含む $J_0$ に含まれる 2 つのコンパクト区間である場合、1 つは次のようになります。

1 思い出してください (*集合理論*, III, p. 144) $I$ の部分集合の集合 $\mathfrak{F}$ は、関係* $\subset$ に関して * 指示されています。 $X \in \mathfrak{F}$、$Y \in \mathfrak{F}$、$X \subset Z$、$Y \subset Z$のような$Z \in \mathfrak{F}$が存在します。 $S(X)$ が、$U \supset X$ となるように $U \in \mathfrak{F}$ によって形成された $\mathfrak{F}$ の部分集合を表す場合、$\mathfrak{F}$ のフィルターの $S(X)$ 形基底は、切断の *フィルターと呼ばれます$\mathfrak{F}$; $\mathfrak{F}$の切断のフィルタに関して、$\mathfrak{F}$の$f$の写像の極限（存在する場合）をトポロジカルな空間に変換することは、有向集合*に関するfの*極限と呼ばれます$\mathfrak{F}$ (*cf. Gen. Top.*、I、p. 70 および *Gen. Top.*、IV、p. 348)。

$$
\left\| \int_J f(t)\,dt - \int_{J'} f(t)\,dt \right\| = \left\| \int_x^z f(t)\,dt + \int_t^y f(t)\,dt \right\| \leq \varepsilon,
$$
それ以来
$$
x \leq \alpha \leq \beta \leq y \quad \text{and} \quad z \leq \alpha \leq \beta \leq t.
$$

#### 例 {#fvr-ii-s2-n1-exa-2 .statement tag=088J}

区間 I が *有界* で、$f$ が I で *有界* である場合、整 $\int_I f(t)\,dt$ は常に存在します。なぜなら、平均値定理では、$y \leq \alpha \leq \beta \leq z$ に対して、
$$
\left\| \int_y^\alpha f(t)\,dt \right\| \leq (\alpha - a) \sup_{t \in I} \|f(v)\| , \quad \left\| \int_\beta^z f(t)\,dt \right\| \leq (b - \beta) \sup_{t \in I} \|f(x)\|
$$
そして、コーシー基準を満たすのに十分小さい $\alpha - a$ と $b - \beta$ を取るだけで十分です。

この場合、Iがコンパクトで$f$が制御されている場合とは対照的に、I上の$f$のプリミティブは、Iの左側の端点（または右側の端点）（この数が有限の場合）で必ずしも右側（または左側）導関数を持たないことに注意するかもしれません。 I (*cf.* II、p. 33、練習問題 1)。

### 2. 非コンパクト区間に対する正の写像の積分

#### 命題 2 {#fvr-ii-s2-prop-2 .statement tag=088K}

*$f$ を、エンドポイント $a$ および $b$ ($a < b$) で区間 $I \subset \mathbf{R}$ に規制されている実際の写像 $\geq 0$ とします。整 $\int_a^b f(t)\,dt$ が存在するには、J が I に含まれるコンパクト区間の集合を通過するとき、数 $\int_J f(t)\,dt$ の集合が上に境界されることが必要かつ十分です。整 $\int_a^b f(t)\,dt$ は、$\int_J f(t)\,dt$ の集合の最小値上界になります。

確かに、$f \geq 0$ 以降、関係 $J \subset J'$ は次のことを意味します。
$$
\int_J f\,dt \leq \int_{J'} f\,dt;
$$
したがって、写像 $J \mapsto \int_J f\,dt$ は増加するとなり、単調な極限定理 (*Gen. Top.*、IV、p. 349、th. 2) から命題が続きます。

写像 $J \mapsto \int_J f(t)\,dt$ が制限されていない場合、有向集合 $\mathscr{K}(I)$ に関して極限 $+\infty$ があります。そして、言葉を乱用して、整$\int_a^b f(t)\,dt$は$+\infty$に等しいと言います。 n 1 拡大する (写像 $\geq 0$ を扱う場合) で確立される積分の性質は、関係する積分の一部が無限である場合まで、その特徴が意味をなす関係の場合に適用されます。

**命題 3 (比較原理)。** *$f$ と $g$ を、区間 $I \subset \mathbf{R}$ で規制される 2 つの実数写像とし、$f$ と $g$ が連続する各点で $0 \leq f(x) \leq g(x)$ となるようにします。 (*cf.* II、p. 61、提案 6)。 $I$ に対する $g$ の積分が収束する場合、$f$ の積分も収束し、$\int_I f(t)\,dt \leq \int_I g(t)\,dt$ が得られます。さらに、2 つの積分できないは、$f$ と $g$ が連続している場合、$I$ の点ごとに〜でない限り $f(x) = g(x)$ に等しくなります。*

現在、すべてのコンパクト区間 $J \subset I$ には、

$$
\int_J f(t)\,dt \leq \int_J g(t)\,dt;
$$

$\int_J g(t)\,dt \leq \int_I g(t)\,dt$ 以降、整 $\int_J f\,dt$ は上に境界があるため、整 $\int_I f(t)\,dt$ は収束します。さらに、移行から極限には、$\int_I f(t)\,dt \leq \int_I g(t)\,dt$ があります。さらに、$f$と$g$が連続している点$x \in I$で$f(x) < g(x)$とします。 $I$ に含まれるコンパクトな区間 $[c,\ d]$ が存在し、(単一の) 点には還元されず、$x \in [c,\ d]$ になります。一方には $\int_c^d f(t)\,dt < \int_c^d g(t)\,dt$ (II, p. 61, cor. 1) があり、他方では上記から $\int_a^c f(t)\,dt \leq \int_a^c g(t)\,dt$ と $\int_d^b f(t)\,dt \leq \int_d^b g(t)\,dt$ があるため、項ごとに追加すると $\int_a^b f(t)\,dt < \int_a^b g(t)\,dt$ であることがわかります。

この命題は、写像 $f \geq 0$ の積分が収束しているかどうかを判断するために最も頻繁に使用される手段を提供します。つまり、$f$ を、収束しているか収束していないことがすでにわかっている積分であるより単純な写像 $g \geq 0$ と比較します。この章で見ていきます。 V コンパレーター 写像を検索する方法 (最も一般的な場合)。そして、積分と系列の収束のための日常的な基準を推定します。

### 3. 絶対収束積分

#### 定義 2 {#fvr-ii-s2-def-2 .statement tag=088L}

*正の写像 $\| \mathbf{f}(x) \|$ の積分が収束する場合、規制された写像 $\mathbf{f}$ の区間 $I \subset \mathbf{R}$ の積分は絶対に収束すると言われています。

#### 命題 4 {#fvr-ii-s2-prop-4 .statement tag=088M}

*$I$ に対する $\mathbf{f}$ の積分が絶対に収束する場合、それは収束しており、*

$$
\left| \int_I \mathbf{f}(t)\,dt \right| \leq \int_I \| \mathbf{f}(t) \| \,dt.\tag{2}
$$

実際、すべてのコンパクト区間 $J \subset I$ には (II, p. 61, 公式 (16)) があります。

$$
\left| \int_J \mathbf{f}(t)\,dt \right| \leq \int_J \| \mathbf{f}(t) \| \,dt.\tag{3}
$$

正の写像 $\| \mathbf{f}(x) \|$ の積分が収束する場合、すべての $\varepsilon > 0$ に対して、$I$ に含まれるコンパクト区間 $[\alpha,\ \beta]$ が存在します。つまり、すべてのコンパクト区間 $[\lambda,\ \gamma]$ は $I$ に含まれ、内部を持たないことになります。 点の共通のと $[\alpha,\ \beta]$ は、$\int_{\lambda}^{\gamma} \| \mathbf{f}(t) \, dt \| \leq \varepsilon$ になります (II、p. 65、提案 1)。 $\left| \int_{\lambda}^{\gamma} \mathbf{f}(t)\,dt \right| \leq \varepsilon$ は、$I$ にわたる積分の収束を示します (II, p. 16、提案 1)。 (3) の移行から極限から、不等式 (2) が推測されます。

#### 系 {#fvr-ii-s2-n3-cor-1 .statement tag=088N}

*$E, F, G$ を $\mathbf{R}$ 上の 3 つの完全ノルム空間とし、$(x, y) \mapsto x.y$ を $E \times F$ から $G$ までの連続双線形写像とします。 $\mathbf{f}, \mathbf{g}$を$I$の2つの規制写像とし、それぞれ$E$と$F$に値を追加します。 $\mathbf{f}$ が $I$ で境界があり、g の * 積分が I で絶対収束する場合、[f, g] の積分は絶対収束します。

実際、$\| [x.y] \| \leq h \| x \| . \| y \|$ が同じになるような数 h > 0 が存在します (Gen. Top., IX, p. 173, th. 1)。 $k = \sup_{x \in I} \| f(x) \|$ を置くと、I には $\| [f(x).g(x)] \| \leq h k \| g(x) \|$ が入ります。比較原理は、[f.g] の積分が絶対に収束することを示し、(2) より、

$$
\left\| \int_I [f(t).g(t)] \, dt \right\| \leq h k \int_I \| g(t) \| \, dt.
$$

#### 注意 {#fvr-ii-s2-n3-rem-1 .statement tag=088O}

積分は完全に収束しなくても収束する可能性があります。これは、II、p. 64 の例 3 によって示されるものです。ここで、系列と一般的な項 $u_n$ は、絶対に収束するわけではなく収束します。

### 練習問題 {#fvr-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
