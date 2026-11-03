---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 1
section_title: Premeasures and measures on a topological space
lang: ja
source: int-vii-ix
pdf_pages: 0183-0204, 0288-0289
extraction: ocr
subsections:
    - "no": 1
      title: Encumbrances
      page: 0
      pdf_page: 183
    - "no": 2
      title: Premeasures and measures
      page: 3
      pdf_page: 185
    - "no": 3
      title: Examples of measures
      page: 6
      pdf_page: 188
    - "no": 4
      title: Locally negligible sets and functions
      page: 8
      pdf_page: 190
    - "no": 5
      title: Measurable sets and functions
      page: 9
      pdf_page: 191
    - "no": 6
      title: Directed families; support of a measure
      page: 11
      pdf_page: 193
    - "no": 7
      title: Upper envelopes and sums of measures
      page: 12
      pdf_page: 194
    - "no": 8
      title: Crushings
      page: 13
      pdf_page: 195
    - "no": 9
      title: Upper integral
      page: 17
      pdf_page: 199
    - "no": 10
      title: Integration theory
      page: 20
      pdf_page: 202
statements: 52
exercises: 10
content_sha256: f0561ebcaf0901151f846ddff4e29cc4fc998c54bfc28ad1d709a6e25a57216c
translated_from: content/en/int/IX/01_s1_premeasures_and_measures_on_a.md
translation_method: google
source_content_sha256: 317fc43050baeab2bc8c0cb022963528cc65340ba4a1f70e587dec5228ab5967
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 3737c0ed16a6357d929a7af8ed0ba073be2b34f5b7253840586b1857b3a39ae6
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。トポロジー上の事前対策と対策空間

### 1. 障害

#### 定義 1 {#int-ix-s1-def-1 .statement tag=09MO}

— T を集合とします。 T 上の負担を $\mathscr{F}_+(T)$ の写像 p から $\overline{\mathbf{R}}_+$ に呼び出します。これは次の特性を持ちます。
a) f と g が $f \leq g$ となるような $\mathscr{F}_+$ の 2 つの元である場合、$p(f) \leq p(g)$ になります。
b) f が $\mathscr{F}_+$ の元で、t が数 $\geq 0$ の場合、$p(tf) = tp(f)$ です。

c) *f と g が $\mathscr{F}_+$ の 2 つの元である場合、$p(f + g) \leq p(f) + p(g)$。*
d) *$(f_n)$ が増加する数列の元または $\mathscr{F}_+$ の場合、$f = \lim_{n \to \infty} f_n$ の場合、$p(f) = \lim_{n \to \infty} p(f_n)$。*
*A が T の部分集合の場合、$p(\varphi_A)$ の代わりに $p(A)$ と書きます。

条件 b) は $p(0) = 0$ を意味します。一方、$(f_n)$ を $\mathscr{F}_+$ の元の数列とします。 条件 c) と d) は不等式を暗示します

$$
p\left( \sum_n f_n \right) \leq \sum_n p(f_n)
$$

(可算凸*の*不等式)。

たとえば、T を局所的にコンパクトな空間、$\mu$ を T の正の測度であるとします。次に、$\mu^*$ と $\mu^\bullet$ は T に対する制約です。これは Props から続きます。 １０、１１、１２およびＴｈ．第3章IV, §1, No. 3 は $\mu^*$ 、および第 3 章の提案 1 より。 $\mu^\bullet$の場合はV, §1, No. 1。

#### 命題 1 {#int-ix-s1-prop-1 .statement tag=09MP}

*$(p_\alpha)_{\alpha \in A}$ を T 上の債務のファミリーとします。和とファミリー $(p_\alpha)$ ($\mathscr{F}_+(\mathscr{F}_+(T))$ 内) の上部エンベロープが債務になります。*

明らかに負担である有限族の和は、上部のエンベロープの場合を扱うだけで十分です。 定義 1 の特性 a)、b)、c) が明らかに満たされているため、d) を確立することが残っています。 集合 $p = \sup_\alpha p_\alpha$;次に、定義 1 d) の記法で、

$$
p(f) = \sup_\alpha p_\alpha(f) = \sup_\alpha \sup_n p_\alpha(f_n) = \sup_n \sup_\alpha p_\alpha(f_n) = \sup_n p(f_n).
$$

#### 定義 2 {#int-ix-s1-def-2 .statement tag=09MQ}

*p を集合 T の制約とする。$p(T) < +\infty$ の場合、p は有界であると言われます。 T が位相幾何学的空間である場合、すべての $x \in T$ が $p(V) < +\infty$ となるような近傍 V を許容するという条件で、p は局所的に有界であると言われます。

次に、Def のプロパティ a) と c) から導き出されます。 1 は、T のすべてのコンパクト部分集合 K に対して $p(K) < +\infty$ です。特に、T がコンパクトな場合、T 上のローカルに制限されたすべての制約が制限されます。

p を集合 T の制約、および T の A 部分集合とする。すべての写像 $f \in \mathscr{F}_+(A)$ について、f から T までの 0 によって $f^0$ を拡大とする。 $\mathscr{F}_+(A)$ の写像 $f \mapsto p(f^0)$ は、A の p* によって引き起こされる * 障害と呼ばれる障害であり、 $p|A$ または $p_A$ で示されます。

T と U を、T を U に変換した 2 つの集合、$\pi$ 写像、および T 上の制約とします。U 上の制約 $\pi(p)$ は、$f \in \mathscr{F}_+(U)$ に対する値は次の式で与えられます。

$$
(\pi(p))(f) = p(f \circ \pi),
$$

は、$\pi$ の下の $p$ の *像負担* と呼ばれます。

$p$ を集合 $T$ の負担とします。 $p$は、$p(T - A) = 0$の場合、$T$の部分集合$A$に*集中*されると言われています。

#### 補題 1 {#int-ix-s1-lem-1 .statement tag=09MR}

— *負担$p$が$A \subset T$に集中している場合、$f \in \mathscr{F}_+(T)$ごとに$p(f) = p(f \varphi_A)$が発生します。*

集合 $T - A = B$ なので、$p(\varphi_B) = 0$;それから

$$
f \varphi_B \leq (+\infty) \cdot \varphi_B = \sup_{n \in \mathbf{N}} n \varphi_B,
$$

したがって、Def のプロパティ $a), b), d)$ により $p(f \varphi_B) = 0$ となります。 1. c) から $p(f) \leq p(f \varphi_A) + p(f \varphi_B) = p(f \varphi_A)$ が得られ、最後に a) によって $p(f) = p(f \varphi_A)$ が得られます。

### 2. 事前対策と対策

$T$ をトポロジー 空間とし、$\mathfrak{K}$ を包含順に並べた $T$ のコンパクトな部分集合の集合とします。 すべての $K \in \mathfrak{K}$ について、$\mathscr{M}(K; \mathbf{C})$ を $K$ の複素測度の集合とします。 For every pair $(K, L)$ of elements of $\mathfrak{K}$ such that $K \subset L$, let $\iota_{KL}$ be the mapping of $\mathscr{M}(L; \mathbf{C})$ into $\mathscr{M}(K; \mathbf{C})$ that associates to each measure $\mu$ on $L$ the measure $\mu_K$ induced by $\mu$ on $K$ (Ch. IV, §5, No. 7、デフォルト。 4)。 次に、$K, L$ と $M$ が $T$ の部分集合で、$K \subset L \subset M$ となるとき、$\iota_{KM} = \iota_{KL} \circ \iota_{LM}$。これは、誘導措置の推移性から続きます（Ch. V, §7, No. 2、提案 4)。 写像 $\iota_{KL}$ の族 $(\mathscr{M}(K; \mathbf{C}))_{K \in \mathfrak{K}}$ の *逆数極限* の元は、$T$ で *premeasures* と呼ばれます。 その他語:

#### 定義 3 {#int-ix-s1-def-3 .statement tag=09MS}

*$T$ のすべてのコンパクト部分集合 $K$、$K$ 上のメジャー $w_K$ に関連付けられる写像 $w$ ごとにトポロジカル空間 $T$ の事前メジャーを呼び出します。これには次の性質が含まれます。

*$K$ と $L$ が $K \subset L$ となるように $T$ のコンパクト部分集合である場合、 $K$ で $w_L$ によって引き起こされる測度 $(w_L)_K$ は $w_K$ に等しくなります。

すべての測定値 $w_K$ が実数 (それぞれ正) である場合、事前測定値 $w$ は実数 (それぞれ正) であると言われます。*

$w$ と $w'$ を $T$、$t$ 複素数の 2 つの事前測定とします。事前対策 $w + w'$ と $tw$ は、$T$ の各コンパクト部分集合 $K$ について、公式 $(w + w')_K = w_K + w'_K$、$(tw)_K = tw_K$ によって定義されます。 $T$ の事前措置は明らかに形ベクトル空間であり、$\mathscr{P}(T; \mathbf{C})$ で示されます。実際の事前測定値の空間は $\mathscr{P}(T; \mathbf{R})$、またはより多くの場合 $\mathscr{P}(T)$ で示され、正の事前測定値の凸円錐は $\mathscr{P}_+(T)$ で示されます。 $w$ を事前措置としましょう。 写像 $K \mapsto |w_K|$ は、$T$ (Ch. IV, §5, No. 7、補題 3) の事前措置であり、$|w|$ と示されます。 $w$ が実数の場合、1 つの集合 w^+ = \frac{1}{2}(|w| + w),\ w^- = \frac{1}{2}(|w| - w);これら 2 つの事前測定値が正である場合、すべての実際の事前測定値は 2 つの正の事前測定値の差であることがわかります。 T のすべてのコンパクト部分集合 K に対して、明らかに $(w^+)_K = (w_K)^+$、$(w^-)_K = (w_K)^-$ です。

ベクトル空間 $P(T)$ は、コーン $P_+(T)$ によって順序付けされます。 $w^+ = \sup(w, 0),\ w^- = \sup(-w, 0)$であることは明らかです。従って、$P(T)$ は格子順序であり、$\sup(w, w') = w + (w' - w)^+,\ \inf(w, w') = w - (w' - w)^-$ です。しかも、明らかに

$$
(\sup(w, w'))_K = \sup(w_K, w'_K),\quad (\inf(w, w'))_K = \inf(w_K, w'_K)
$$

T のすべてのコンパクト部分集合 K に対して。

#### 定義 4 {#int-ix-s1-def-4 .statement tag=09MT}

*w を T の正の事前測定とします。写像 $f \in \mathscr{F}_+(T)$ ごとに、集合とします*

$$(1)$$
$$
w^\bullet(f) = \sup_K (w_K)^\bullet(f_K),
$$

*ここで、K は T のコンパクト部分集合の集合を超えます。*

それぞれの圧縮集合 K について、$p^K$ を、K の標準単射の下での債務 $(w_K)^\bullet$ の T への債務像とします。 $w^\bullet$ は債務 $p^K$ の上部エンベロープであり、したがって債務です (No. 1、提案 1)。 $w^\bullet$ は、正の事前測度 w に関連付けられた*必須の上積分*であると言われています。 $w^\bullet(f)$ の代わりに $\int^\bullet f\, dw$ または $\int^\bullet f(t)\, dw(t)$ と書くことがよくあります。

*注意 1).* — v と w が 2 つの正の事前測定値である場合、$(v + w)^\bullet = v^\bullet + w^\bullet$ (Ch. V, §1, No. 1、提案 3)。 v と w が 2 つの複素前測度の場合、$|v + w|^\bullet \leq |v|^\bullet + |w|^\bullet$。

#### 命題 2 {#int-ix-s1-prop-2 .statement tag=09MU}

*a) w を正の事前尺度とします。 T のすべてのコンパクト部分集合 K について、K 上の $w^\bullet$ によって引き起こされる制約 $(w^\bullet)_K$ は $(w_K)^\bullet$ に等しくなります。 写像 $f \in \mathscr{F}_+(T)$ ごとに、1 つは関係 $(w_K)^\bullet(f_K) = w^\bullet(f_{\varphi_K})$ となり、*

$$(2)$$
$$
w^\bullet(f) = \sup_K w^\bullet(f_{\varphi_K}).
$$

*b) 逆に、p を T 満たす次の条件に対する負担とする。
1) T のすべてのコンパクト部分集合 K に対して、$p_K = (w_K)^\bullet$ となるような K 上の正の測度 $w_K$ が存在します。
2) 写像 $f \in \mathscr{F}_+(T)$、$p(f) = \sup_K p(f_{\varphi_K})$ ごとに。
写像 $w : K \mapsto w_K$ は T の正の事前測定値であり、$p = w^\bullet$ です。

$a$ を証明しましょう: $g \in \mathscr{F}_+(K)$ と $g^0$ は、$g$ から $T$ の零によって拡大になります。その後、誘発された障害の定義により、

$$
(w^\bullet)_K(g) = w^\bullet(g^0) = \sup_L (w_L)^\bullet(g^0|L),
$$

ここで、$L$ は、$T$ のコンパクトな部分集合の集合、または含む $K$ のうちの集合を上回ります。 しかし、$L$ 含む $K$ の場合、$g^0|L$ は $K$ の外にある零であるという事実から、$(w_L)^\bullet(g^0|L) = (w_K)^\bullet(g)$ になります。 V, §7, No. 1、提案 1)、これは最初の主張を証明します。 したがって

$$
(w_K)^\bullet(f_K) = (w^\bullet)_K(f_K) = w^\bullet((f_K)^0) = w^\bullet(f_{\varphi_K})
$$

すべての $f \in \mathscr{F}_+(T)$ に対して、(2) は単に公式 (1) を変換するだけです。

$b$ に進みましょう: 1) で考慮されたメジャー $w_K$ は一意です (Ch. V, §1, No. 1)。 写像 $K \mapsto w_K$ が事前測度であることを示しましょう。$K$ と $L$ を、$K \subset L$ となる 2 つのコンパクト部分集合とし、$\lambda$ を $K$ で $w_L$ によって誘導される測度としましょう。すべては、$\lambda^\bullet = (w_K)^\bullet$ を示すことに尽きるのです。 さて、$\lambda^\bullet = ((w_L)^\bullet)_K$ (Ch. V, §7, No. 1、提案 1); $(w_L)^\bullet = p_L$ から、$\lambda^\bullet = (p_L)_K = p_K = (w_K)^\bullet$ になります。

事前測定 $K \mapsto w_K$ を $w$ で表しましょう。 $p_K = (w_K)^\bullet = (w^\bullet)_K$ から、$p(f_{\varphi_K}) = p_K(f_K) = (w^\bullet)_K(f_K) = w^\bullet(f_{\varphi_K})$ になります。したがって、2 つの負担 $p$ と $w^\bullet$ は、$p$ の公式 (2) と仮定 2) により等しくなります。

Q.E.D.

誘発された障害 $(w^\bullet)_K$ は $(w_K)^\bullet$ に等しいため、単純に $w_K^\bullet$ と書くことに曖昧さはありません。今後はこれ記法を採用します。

#### 系 {#int-ix-s1-n2-cor-1 .statement tag=09MV}

— *$v$ と $w$ を $T$ の 2 つの正の事前測定とし、$T$ のすべてのコンパクト部分集合 $L$ に対して $v^\bullet(L) = w^\bullet(L)$ とする。次に$v = w$。特に、関係 $v^\bullet = w^\bullet$ は $v = w$* を意味します。

なぜなら、$K$ を $T$ のコンパクトな集合とします。コンパクト集合 $L \subset K$ ごとに、1 つは関係を持ちます

$$
w_K(L) = w_K^\bullet(L) = w^\bullet(L) = v^\bullet(L) = v_K^\bullet(L) = v_K(L)
$$

提案2による。したがって $w_K = v_K$ (Ch. IV, §4, No. 10、コル。提案 19 の 3)、最終的には事前措置の定義によって $w = v$ となります。

#### 定義 5 {#int-ix-s1-def-5 .statement tag=09MW}

— *$w$ をトポロジカル空間 $T$ の事前測定とします。制約事項 $|w|^\bullet$ が局所的に限定されている (それぞれ有界) (cf. No. 1、定義 2)* 場合、$w$ は尺度 (それぞれ有界の尺度) であると言われます。

$T$ の複雑な測度の集合は明らかにベクトル空間 (*注意* 1) であり、$\mathscr{M}(T; \mathbf{C})$ と表されます。実際の対策の空間は$\mathscr{M}(T; \mathbf{R})$、または多くの場合$\mathscr{M}(T)$で示され、前向きの対策のコーンは$\mathscr{M}_+(T)$で示されます。

$w$ が複素測度の場合、その実数部分と虚数部分が実数測度です。 $w$ が実際の指標である場合、$w^+$ と $w^-$ は積極的な指標です。したがって、すべての複雑な (それぞれ実際の) 測定は、正の測定の線形結合 (それぞれの差) です。

#### 注意 2 {#int-ix-s1-n2-rem-2 .statement tag=09MX}

$T$ が *局所的にコンパクト* である場合、$T$ 上のすべての事前メジャー $w$ がメジャーになります。なぜなら、すべての $x \in T$ はコンパクトな近傍 $K$ と $|w|^*(K) = \|w_K\| < +\infty$ を許容するため、制約事項 $|w|^*$ は局所的に制限されるからです。

#### 注意 3 {#int-ix-s1-n2-rem-3 .statement tag=09MY}

$T$ のすべてのボレル部分集合 $A$ (特に $A = T$) および $T$ のすべてのポジティブな尺度 $\mu$ について、数 $\mu^*(A)$ は、コンパクトな部分集合の尺度 $\mu^*(K)$ の最高値です。 $A$。実際、$A$ の各コンパクト部分集合 $K$ には、$\mu^*(K) \leq \mu^*(A)$ があります。一方、$\mathfrak{K}$ が $T$ のコンパクト部分集合の集合である場合、

$$
\mu^*(A) = \sup_{K \in \mathfrak{K}} \mu_K^*(A \cap K) = \sup_{K \in \mathfrak{K}} \sup_{L \in \mathfrak{K}, L \subset A \cap K} \mu_K^*(L) \leq \sup_{L \in \mathfrak{K}, L \subset A} \mu^*(L)
$$

コル著Thの1第4章IV, §4, No. 6。

### 3. 例の対策

#### 例 1 {#int-ix-s1-n3-exa-1 .statement tag=09MZ}

— *ローカルコンパクト空間で測定。*

次の命題は、この章含むの理論が Ch の理論であることを示しています。 IV。 主張、語の「測定」、記法 $\mathscr{M}(T; \mathbf{C})$は、先ほどの章の意味で解釈されます。

#### 命題 3 {#int-ix-s1-prop-3 .statement tag=09N0}

*$T$ を局所コンパクト空間とし、$\mu$ を $T$ のメジャーとします。 $T$ の各コンパクト部分集合 $K$ に誘導メジャー $\mu_K$ を関連付ける $W(\mu)$ 写像で示します。次に、$W(\mu)$は$T$の事前措置であり、$W(|\mu|) = |W(\mu)|$があり、線形写像$W : \mu \mapsto W(\mu)$は空間$\mathscr{M}(T; \mathbf{C})$の全単射を空間$\mathscr{P}(T; \mathbf{C})$に事前措置します。 $T$。さらに、$\mu$が正なら$\mu^* = (W(\mu))^*$です。

$W(\mu)$ が事前措置であることは明らかです (Ch. V, §7, No. 2、提案 4) そして、写像 $W$ は線形です。 関係 $W(\mu) = 0$ は、$\mu$ 誘導する $T$ のすべてのコンパクト集合の小節 0 を意味します。次に、$f \in \mathscr{H}(T; \mathbf{C})$ に対して $\mu(f) = 0$、つまり $\mu = 0$ となり、$W$ が単射であることが証明されます。 $W$ が全射であることを証明することはまだ残っています。 すべての事前測定は、正の事前測定の線形結合であるため、すべての *正の* 事前測定 $w$ に対して、$w = W(\mu)$ となるような正の測定 $\mu$ を構成するすれば十分です。 $f \in \mathscr{H}(T)$ を与えられた写像とし、$L$ を $f$ のサポートをコンパクトにした集合含むとします。 数 $w_L(f_L)$ は、$L$ の選択から、誘導措置の定義によって独立しているため、集合 $\mu(f) = w_L(f_L)$ が可能です。この場合、$\mu$ は $\mathscr{H}(T)$ に対するプラスの線型形式、つまりプラスの尺度です。 $w = W(\mu)$; であることを確認してみましょう。まず、関係 $\mu^\bullet(f) = w_L^\bullet(f_L)$ 拡大するを、$f$ が正で$L$ の外側の零である有限の上半連続写像である場合に当てはめます。 なぜなら、$M$ を $L$ のコンパクトな近傍とし、$\mathscr{H}$ を $T$ 上の連続写像の (減少するで指示された) 集合とし、$M$ に含まれるサポート、つまり $\geq f$ とする。 それから (Ch. IV, §4, No. 4、コル。提案 5 の 2)

$$
\mu^\bullet(f) = \inf_{h \in \mathscr{H}} \mu(h) = \inf_{h \in \mathscr{H}} w_M(h_M) = w_M^\bullet(f_M),
$$

一方、$f_M$ は $M - L$ で零であるため、$w_M^\bullet(f_M) = w_L^\bullet(f_L)$ (Ch. V, §7, No. 1、提案 1)。特に、$f$が$\mathscr{H}_+(L)$の元の0によって拡大とされる場合、この公式は、誘導措置の定義によって$\mu_L = w_L$、したがって実際には$W(\mu) = w$であることを示しています。

$\mu$ が正の場合、

$$
\mu^\bullet(f) = \sup_K \mu^\bullet(f \varphi_K) = \sup_K \mu_K^\bullet(f_K) = (W(\mu))^\bullet(f)
$$

$f \in \mathscr{F}_+(T)$ ごとに (Ch. V, §1、デフォルト。 1 および §7、提案 1)。 関係 $|W(\mu)| = W(|\mu|)$ は明らかです (Ch. IV, §5, No. 7、補題 3)。

Q.E.D.

$T$ が *局所的にコンパクト* である場合、これから全単射 $W$ を使用して *同一視する* 空間 $\mathscr{M}(T; \mathbf{C})$ と $\mathscr{P}(T; \mathbf{C})$ を実行します。

#### 例 2 {#int-ix-s1-n3-exa-2 .statement tag=09N1}

— *トポロジー 空間でのコンパクトなサポートによる測定。*

#### 補題 2 {#int-ix-s1-lem-2 .statement tag=09N2}

— *$T$ をトポロジー 空間、$L$ を $T$ の圧縮部分集合、$\lambda$ を $L$ の正の測度とする。 $T$ には、写像 $f \in \mathscr{F}_+(T)$ ごとに、* となるような独自のポジティブな尺度 $\mu$ が存在します。

(2)
$$
\mu^\bullet(f) = \lambda^\bullet(f_L).
$$

すべての $f \in \mathscr{F}_+(T)$ について集合 $p(f) = \lambda^\bullet(f_L)$ とし、条件提案 2 *b*) の 1) と 2) が満たされることを示しましょう。 2 番目は明らかに満たされています。実際、$K$ 含む $L$ であれば、$p(f) = p(f \varphi_K)$ です。 $K \subset T$ がコンパクトであれば、$h \in \mathscr{F}_+(K)$ であれば、

$$
p_K(h) = p(h^0) = \lambda^\bullet(h^0|L).
$$

しかし、$h^0|L$ は $h_{K \cap L}$ から $L$ の 0 による拡大です。したがって、最後の式は $(\mu_K)^\bullet(h)$ と等しくなります。ここで、$\mu_K$ は、$K \cap L$ の単射の下にある $\lambda|K \cap L$ の像です。 $K$ (Ch. V, §6, No. 2、提案 2 および §7, No. 1、提案 1)、および $p_K = (\mu_K)^\bullet$。したがって、提案 2 *b*) の条件 1) も満たされ、直ちに $\mu$ の存在が続きます。

Q.E.D.

$\mu$ は、$\lambda$ によって *定義*された T 上のメジャーであると言いましょう。特に、T の点 $x$ ごとに、メジャー $\varepsilon_x$ を定義する求めることができます。 $f \in \mathscr{F}_+(T)$に対する$(\varepsilon_x)^*(f) = f(x)$が特徴です。

#### 注意 {#int-ix-s1-n3-rem-1 .statement tag=09N3}

— 1) T が局所的にコンパクトな場合、$\mu$ は T のL の単射の下で$\lambda$ の像になります。像測度が処理されるとき、§2, No. 3、*例* で、この解釈が任意の場合に有効であることがわかります。 空間。
2) *例* 2 で定義された措置は、コンパクトなサポート (No. 6, *注意* 2)) を備えた T 上の積極的な措置であることもわかります。

*今後は、反対の明示的な言及を除き、前向きな措置のみを検討します。この切断の残りについては、T はトポロジカル空間を表し、$\mu$ は T の正の測度を表します。

以下の小節の多くの結果は、肯定的な事前測定に拡張される可能性があります。この拡大は読者に委ねられています。

### 4. 局所的に無視できる集合および写像

#### 定義 6 {#int-ix-s1-def-6 .statement tag=09N4}

*写像* $f \in \mathscr{F}_+$ (対応 *部分集合* A *of* T) *測度に対して局所的に無視できると言われています* $\mu$ *if* $\mu^*(f) = 0$ (対応 $\mu^*(A) = 0$)。 *ある人は、* $\mu$ * は部分集合* A *of* T *if* T − A *が局所的に* $\mu$ *-無視できる* に集中していると言います。

#### 注意 {#int-ix-s1-n4-rem-1 .statement tag=09N5}

— 1) T が局所的にコンパクトなとき、通常の概念を使用して定義された概念一致する。
2) *無視できる* 集合を定義した後でから、局所的に無視できる集合は実際に、T のすべての点におけるその芽が無視できる集合の芽であることがわかります (No. 9、提案 14 の Cor. 2)。
3) 第 3 章と同様。 IV と V では、「局所的にほぼどこでも」という表現は、「局所的に無視できる集合を除いて」と同義になります。
4) $\theta$ が複素測度である場合、正の測度 $|\theta|$ がそうであれば、写像 (T の部分集合) は $\theta$ に対して局所的に無視できると言えます。

#### 例 {#int-ix-s1-n4-exa-1 .statement tag=09N6}

— L を T の圧縮部分集合、$\lambda$ を L のメジャー、$\mu$ を $\lambda$ (No. 3, *例* 2) で定義される T のメジャーとします。 公式 (3) は、$f_L$ が $\lambda$ 無視できる場合に限り、写像 $f \in \mathscr{F}_+(T)$ が局所的に $\mu$ 無視できることをすぐに暗示します。

公式 (1) から、写像 $f \in \mathscr{F}_+(T)$ は、T のすべてのコンパクト部分集合 K について $f_K$ が $\mu_K$ 無視できる場合に限り、局所的に $\mu$ 無視できることがわかります。 したがって、局所的に無視できる集合の性質は次のようになります。 簡約するを一度に、無視できる程度の集合をコンパクトな空間にまとめます。 IV。以下は、さらなる参照なしで今後使用されるいくつかの結果です。

— 写像 $f \geqslant 0$ が局所的に無視できるためには、ほぼどこでも $f(t) = 0$ が局所的に存在することが必要かつ十分です (Ch. IV, §2, No. 3、Th. 1)。したがって、$f$ がバナッハ空間の値とともに写像である場合、それはほぼどこでも局所的に $f = 0$ であるか、あるいは $\mu^*(|f|) = 0$ であると言うのと同じです。この場合、$f$ は局所的に無視できるともう一度言います。

— 和と、局所的に無視できる写像 $\geqslant 0$ の数列の上部エンベロープは、局所的に無視できます (*上記引用*、No. 1、提案 2)。

— $f$ と $g$ が、ほぼどこでも局所的に等しい 2 つの写像 $\geqslant 0$ である場合、$\mu^\bullet(f) = \mu^\bullet(g)$ (*loc. cit.*、No. 3、提案 6)。

### 5. 測定可能集合および写像

#### 定義 7 {#int-ix-s1-def-7 .statement tag=09N7}

*写像* $f$ *上に定義* $T$、*トポロジカル空間で値を使用* $F$ (*ハウスドルフか否か*) *測度が可測であると言われている* $\mu$ *(または* $\mu$*可測である)* *すべてのコンパクト部分集合* $K$ *of* $T$、*写像* $f_K$ *は* $\mu_K$*測定可能*。

これは、$K$ のすべてのコンパクト集合 $K$、分割が、コンパクト集合の $\mu_K$ 無視できる集合 $N$ および数列 $(K_n)$ に存在するというというになります。 $f$から各$K_n$までの制限は連続です。 Since it is equivalent to say that $N$ is $\mu_K$-negligible or that it is locally $\mu$-negligible (No. 4), one sees that $f$ is $\mu$-measurable if and only if, for every compact set $K$, there exists a partition of $K$ into a locally $\mu$-negligible set $N$ and a sequence $(K_n)$ of compact sets such that $f_{K_n}$ is continuous for all $n$. この定義はDefのものと同一です。 1章 IV, §5, No. 1, and one thus recovers the usual concept of measurable function when $T$ is locally compact.

$T$ の部分集合 $A$ は、その特性写像が測定可能であれば測定可能であると言われます。 $A$が$\mu$可測かつ$\mu^\bullet(A) < +\infty$のとき、この数は単に$\mu(A)$と表され、$A$の*測度*と呼ばれます。同様に、$f$が$\geqslant 0$、$\mu$可測、$\mu^\bullet(f) < +\infty$の場合、$\mu^\bullet(f)$に対して$\mu(f)$と書きます。

$\theta$ が $T$ の複素測度である場合、写像 $f$ (それぞれ $T$ の部分集合) は、正の測度 $|\theta|$ で測定可能であれば、$\theta$ 測定可能であると言われます。以下の結果は、複雑な尺度に拡張できる可能性があります。

#### 例 {#int-ix-s1-n5-exa-1 .statement tag=09N8}

— $L$ を $T$ の圧縮部分集合、$\lambda$ を $L$ のメジャー、$\mu$ を $\lambda$ (No. 3, *例 2*) で定義される $T$ のメジャーとします。 $T$ で定義された写像 $f$ は、$f_L$ が $\lambda$ 測定可能である場合に限り、$\mu$ 測定可能です。 なぜなら、この条件は明らかに必要だからです。 逆に、それが満たされる場合、$\lambda$-無視できる集合 $N$ とコンパクト集合の数列 $(L_n)$ に$L$ の分割が存在し、$f_{L_n}$ がすべての$n$ に対して連続になります。 $K$ が $T$ のコンパクト部分集合である場合、集合 $K - \bigcup^n (K \cap L_n)$ は $\lambda$ が無視できる $L$ を持つ共通部分を持ちます。したがって、この集合は、次の式によって $\mu$ が無視できますNo. 3の公式(3)、$f$～$K \cap L_n$の制限は$n$全て連続です。

デフ。 7 では、新しい証明、数を使用せずに、測定可能な写像の結果を局所的にコンパクトではない空間の場合に拡張することができます。 以下にそれらのいくつかを示しますが、これ以降は参照せずに使用します。 $T$ のオープン集合とクローズ集合は $\mu$ で測定可能です。 $\mu$ 測定可能な集合形部族 (Ch. IV, §5, No. 4、コル。 Thの2。 2)、T の含むボレル集合 (上記引用、コリント 3)、およびスースリン集合 (Ch. IV, §5, No. 1、コル。議案3)(1)の2． 数値写像に対する通常の代数演算は可測性を維持します (Ch. IV, §5, No. 3)、極限への可算通路の演算 (上記引用、No. 4、Th. 2 および Cor. 1) も同様です。 次の性質については、より明確に言及する価値があります。

#### 命題 4 {#int-ix-s1-prop-4 .statement tag=09N9}

— $f$ を T 上の $\mu$ 測定可能な陽性写像の陽性写像と $(g_n)_{n \geq 1}$ 数列とします。設定 $g = \sum_{n \geq 1} g_n$ は、

$$
\mu^\bullet(fg) = \sum_{n \geq 1} \mu^\bullet(fg_n).
$$

$n \geq 1$ 全員に対して集合 $h_n = \sum_{i=1}^n g_i$。 T のすべてのコンパクト部分集合 K に対して、

$$
\mu_K^\bullet((fh_n)_K) = \sum_{i=1}^n \mu_K^\bullet((f g_i)_K)
$$

第 2 章の提案による。 V, §1, No. 1 をコンパクト空間 K に適用します。T のコンパクト部分集合の増加する有向集合に関して移行から極限を取得します。

$$
\mu^\bullet(fh_n) = \sum_{i=1}^n \mu^\bullet(f g_i).
$$

さて、$fg$ は、増加する数列 $(fh_n)_{n \geq 1}$、よって $\mu^\bullet(fg) = \lim_{n \to \infty} \mu^\bullet(fh_n)$ の極限です。前述の公式はすぐに (4) を意味します。

#### 系 {#int-ix-s1-n5-cor-1 .statement tag=09NA}

— $(A_n)$ を、和集合 A を持つ測定可能なペアワイズ互いに素部分集合の数列とします。T のすべての部分集合 B について、

$$
\mu^\bullet(A \cap B) = \sum_n \mu^\bullet(A_n \cap B)
$$

そして特に

$$
\mu^\bullet(A) = \sum_n \mu^\bullet(A_n).
$$

上記の拡大するからハウスドルフ空間までの測定可能な写像または集合の特性のうち、第2章の提案12も引用します。 IV, §5, No. 8 ($\mu$ - コンパクトな集合の高密度ファミリー)。したがって、トポロジカルでは写像 $f$ と値

(1) この系の証明は、計量不可能な局所コンパクト空間 (GT, IX, §6, No. 9, Th. 5) の Souslin 集合に対して修正なしで有効です。

空間 (ハウスドルフかどうか) は、$f_K$ が連続であるようなコンパクトな集合部分集合 K の T が $\mu$ 密である場合に限り、$\mu$ 可測です (*loc. cit.*、No. 10、提案 15)。

### 6. 指示された家族。対策のサポート

#### 命題 5 {#int-ix-s1-prop-5 .statement tag=09NB}

**a)** *H を、T の各コンパクト部分集合の下位半連続である写像 $\geqslant 0$ の増加する有向集合とします。すると*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

*b)* *H を、T のすべてのコンパクト部分集合で上部半連続である写像 $\geqslant 0$ の減少する有向集合とします。$\mu^\bullet(h_0) < +\infty$ のような H 写像 $h_0$ が存在する場合、*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

すべてのコンパクト集合 $K \subset T$ について、ケース *a)* があります。

$$
\mu^\bullet \left( \sup_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \sup_{h \in H} h_K \right) = \sup_{h \in H} \mu_K^\bullet(h_K) = \sup_{h \in H} \mu^\bullet(h \varphi_K),
$$

そして *b)* の場合

$$
\mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \inf_{h \in H} h_K \right) = \inf_{h \in H} \mu_K^\bullet(h_K) = \inf_{h \in H} \mu^\bullet(h \varphi_K),
$$

No. 2 の提案 2、および第 58 章の提案 8 による。 V, §1, No. 2。ケース *a*) は、K に関する最高値への移行によってすぐに続きます (No. 2、提案 2)。ケース *b*) を扱うには、$\varepsilon$ 数 $> 0$、および $\mu^\bullet(h_0 \varphi_K) \geqslant \mu^\bullet(h_0) - \varepsilon$ となるようなコンパクトな集合 K を選ぶで表します。すると (No. 5、提案 4) $\mu^\bullet(h_0 \varphi_{C_K}) \leqslant \varepsilon$; 写像 $h \in H$ ごとに、つまり $\leqslant h_0$ であるため、$\mu^\bullet(h \varphi_{C_K}) \leqslant \varepsilon$ が得られ、No. 5 の提案 4 により最終的に $\mu^\bullet(h \varphi_K) \geqslant \mu^\bullet(h) - \varepsilon$ が得られます。従って、

$$
\mu^\bullet \left( \inf_{h \in H} h \right) \geqslant \mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h \varphi_K) \geqslant \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h) - \varepsilon.
$$

従って、(6) の左辺は $\geqslant$ 右辺になります。逆の不等式は明らかですが、命題が成立します。

#### 系 {#int-ix-s1-n6-cor-1 .statement tag=09NC}

— a) $(U_\alpha)_{\alpha \in I}$ を、和集合 $U$ を持つ、$T$ のオープン部分集合の増加する有向族とします。それから$\mu^\bullet(U) = \sup_{\alpha \in I} \mu^\bullet(U_\alpha)$。

b) $(F_\alpha)_{\alpha \in I}$ を、共通部分 $F$ を伴う、$T$ の閉じた部分集合の減少する指向家族とします。 $\mu^\bullet(F_\alpha)$ が有限であるような $\alpha \in I$ が存在する場合、$\mu^\bullet(F) = \inf_{\alpha \in I} \mu^\bullet(F_\alpha)$ になります。

前の系までに、局所的に無視できるオープン集合が最大の存在します。これは次のことを正当化します定義:

#### 定義 8 {#int-ix-s1-def-8 .statement tag=09ND}

— *$T$のメジャー$\mu$のサポートは、$T$*の$\mu$-無視できるオープン集合のローカルで最大のの補数であると定義されます。

$\mu$ のサポートは $\operatorname{Supp}(\mu)$ で示されます。

#### 注意 1 {#int-ix-s1-n6-rem-1 .statement tag=09NE}

$\mu$ が複雑な指標である場合、$\mu$ のサポートはポジティブ指標 $|\mu|$ のサポートとして定義されます。これもまた、局所的には最大のの補数です $\mu$ - 無視できるオープン集合です。

#### 注意 2 {#int-ix-s1-n6-rem-2 .statement tag=09NF}

No. 3の*例2*で紹介した対策が、$T$でコンパクトにサポートされた対策であることを示しましょう。 $\mu$ を、サポートがコンパクト集合 $K$ である $T$ に対するポジティブなメジャーであるとします。また、$\nu$ を、(No. 3 の意味で) $\mu_K$ によって定義されるメジャーとします。 $f \in \mathscr{F}_+(T)$ にしましょう。それから

$$
\nu^\bullet(f) = \mu_K^\bullet(f_K) \quad \text{(No. 3, formula (3))}.
$$

負担$\mu^\bullet$が$K$に集中しているため、

$$
\mu^\bullet(f) = \mu^\bullet(f \varphi_K) = \mu^\bullet((f_K)^0) = \mu_K^\bullet(f_K),
$$

よって $\mu^\bullet = \nu^\bullet$、そして最後に $\mu = \nu$ です。逆に、$K$ が $T$ のコンパクト集合であり、$\lambda$ が $K$ 上のメジャーであり、$\mu$ が $\lambda$ によって定義される $T$ 上のメジャーである場合、$\mu^\bullet(\mathbf{C}K) = 0$ (No. 3, 公式 (3));従って、$\mu$ のサポートは $K$ に含まれるため、コンパクトになります。

### 7. 上部エンベロープと小節の和

#### 命題 6 {#int-ix-s1-prop-6 .statement tag=09NG}

— *$(\lambda_\alpha)_{\alpha \in A}$ を増加する $T$ に指示されたメジャー群とし、$p = \sup_\alpha \lambda_\alpha^\bullet$ とします。ファミリ $(\lambda_\alpha)$ が上で $\mathscr{M}(T)$ で制限されるためには、制約 $p$ が局所的に制限されることが必要かつ十分です。その後、家族$(\lambda_\alpha)$は$\mathscr{M}(T)$と$\lambda^\bullet = p$に$\lambda$の最高位を認めます。すべてのコンパクト集合 $K$ について、メジャー $\lambda_K$ は、$\mathscr{M}(K)$* のメジャー $(\lambda_\alpha)_K$ の上限です。

ファミリ $(\lambda_\alpha)$ が $\mathscr{M}(T)$ で上に境界がある場合、$p$ は明らかに局所的に境界があります。逆に、$p$ が局所的に有界であると仮定し、No. 2 の提案 2 b) の条件 1) と 2) を満たすことを示しましょう。 2) の場合、これは次の等式から得られます。

$$
p(f) = \sup_\alpha \lambda_\alpha^\bullet(f) = \sup_\alpha \sup_K \lambda_\alpha^\bullet(f \varphi_K) = \sup_K \sup_\alpha \lambda_\alpha^\bullet(f \varphi_K) = \sup_K p(f \varphi_K).
$$

一方、K をコンパクト集合とします。負担 $p_K$ は負担 $(\lambda_\alpha^\bullet)_K$ の上部エンベロープに等しく、$p$ が局所的に有界であるため、有界です。したがって、措置 $(\lambda_\alpha)_K$ は、$\mathscr{M}(K)$ および $\lambda_K^\bullet = p_K$ における最高$\lambda_K$ を認めます (Ch. V, §1, No. 4、提案 11)。 条件 No. 2 の提案 2 b) の 1) が満たされるため、T には $\lambda^\bullet = p$ となるような尺度 $\lambda$ が存在します。 $\lambda$ が措置 $\lambda_\alpha$ の最高値であることは明らかです。

#### 定義 9 {#int-ix-s1-def-9 .statement tag=09NH}

* $(\mu_i)_{i \in I}$ を T 上のメジャーの族とします。A を I の有限部分集合の集合とします。 $\alpha \in A$ごとに$\lambda_\alpha = \sum_{i \in \alpha} \mu_i$にしましょう。家族 $(\lambda_\alpha)$ が $\mathscr{M}(T)$ の最高値 $\mu$ を認める場合、家族 $(\mu_i)$ は合計可能であると言われ、$\mu$ は家族 $(\mu_i)$ の和と呼ばれ、$\mu = \sum_{i \in I} \mu_i$ と書きます。

これは、Ch. の定義拡大する定義です。 V, §2, No. 1。

#### 命題 7 {#int-ix-s1-prop-7 .statement tag=09NI}

*家族 $(\mu_i)_{i \in I}$ が和 $\mu$ と合計可能であるためには、負担 $p = \sum_{i \in I} \mu_i^\bullet$ が局所的に限定されていることが必要かつ十分であり、その場合は $p = \mu^\bullet$ になります。 T のすべてのコンパクト部分集合 K について、ファミリー $((\mu_i)_K)_{i \in I}$ は $\mathscr{M}(K)$ および $\mu_K = \sum_{i \in I} (\mu_i)_K$ で合計可能です。*

Defのように記法とします。 9、I の有限部分集合 $\alpha$ ごとに $\lambda_\alpha^\bullet = \sum_{i \in \alpha} \mu_i^\bullet$ (No. 2、*注意* 1)。 主張は提案 6 の明らか帰結となります。

関係 $\mu_K = \sum_{i \in I} (\mu_i)_K$ および第 2 章の提案 2 V, §2, No. 2 は次の結果を生成します。

#### 命題 8 {#int-ix-s1-prop-8 .statement tag=09NJ}

*$\mu$ を、T 上の測度の加算可能な族 $(\mu_i)_{i \in I}$ の和とします。T の写像 f をトポロジカル空間 F (ハウスドルフかどうか) に変換する位数では、f が $\mu$ 可測であることが必要かつ十分です。 $\mu_i$-$i \in I$ごとに測定可能*。

### 8. 破砕物

#### 定義 10 {#int-ix-s1-def-10 .statement tag=09NK}

*集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$ が局所的に $\mu$-無視できるような、T のペアごとの互いに素コンパクト部分集合のローカルで可算可能な族 $(K_\alpha)_{\alpha \in A}$ を、$\mu$ に対する T のクラッシュ、または $\mu$ クラッシュと呼びます。

#### 命題 9 {#int-ix-s1-prop-9 .statement tag=09NL}

*a) $\mu$に対するTの粉砕$(K_\alpha)_{\alpha \in A}$が存在します。
b) $(K_\alpha)_{\alpha \in A}$ を $\mu$ に対する T の粉砕とします。 $\mu_\alpha$ が $\mu_{K_\alpha}$ (No. 3, 例 2) によって定義される T 上のメジャーである場合、族 $(\mu_\alpha)_{\alpha \in A}$ は合計可能* であり、その和は $\mu$ に等しく、すべての写像 $f \in \mathscr{F}_+(T)$ について、

$$
\mu^\bullet(f) = \sum_{\alpha \in A} \mu_\alpha^\bullet(f) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_{K_\alpha}) . \tag{1}
$$

$T$ の写像 $g$ をトポロジカル空間 $G$ (ハウスドルフであろうとなかろうと) が $\mu$ 可測となるためには、すべての$g_{K_\alpha}$ が $\mu_{K_\alpha}$ 可測であることが必要かつ十分です。 $\alpha \in A$。

A) *潰れの存在*:

証明は、第 4 章の提案 14 の繰り返しです。 IV, §5, No. 9、少し変更あり。 $\mathscr{K}$ を、$\mathrm{Supp}(\mu_K) = K$ となるようなコンパクトな部分集合 $K$ の $T$ の集合とし、$\mathscr{H}$ を、部分集合 $\mathscr{L}$ の集合とします。ペアワイズ互いに素集合の $\mathscr{K}$ からなる。まず、$\mathscr{H}$ のすべての元 $\mathscr{L}$ が *局所的に数えられる* ことを示しましょう。 $x$ を $T$ の点とし、$V$ を $\mu^\bullet(V) < +\infty$ となるような $x$ の開いた近傍とします。 $\mathscr{L}_V$を、$V$と交差する$K \in \mathscr{L}$の集合とします。 $(K_i)_{1 \leq i \leq n}$ が $\mathscr{L}_V$ の別個の元の有限列である場合、コルによれば、提案 4 の、

$$
\sum_{i=1}^n \mu^\bullet(K_i \cap V) = \mu^\bullet\left(V \cap \left( \bigcup_{i=1}^n K_i \right) \right) \leq \mu^\bullet(V),
$$

$K_i$ はペアの互いに素であるためです。したがって、

$$
\sum_{K \in \mathscr{L}_V} \mu^\bullet(K \cap V) < +\infty.
$$

さて、$K \in \mathscr{L}_V$ ごとに $\mu^\bullet(K \cap V) = \mu_K^\bullet(K \cap V) > 0$ です。$K \cap V$ は空でないなので、$K$ でオープンし、$\mu_K$ のサポートはすべて $K$ です。したがって、$\mathscr{L}_V$ は可算であり、$\mathscr{L}$ は実際に局所的に可算です。 $\mathscr{H}$ が帰納的であるのは明らかであり、空でない (1 つは $\varnothing \in \mathscr{H}$ を持つ) です。したがって、$\mathfrak{H}$を$\mathscr{H}$の極大元とします。 集合 $N = T - \bigcup_{K \in \mathfrak{H}} K$ が局所的に無視できることを示します。提案 2 により、すべてのコンパクト集合 $L$ について $\mu^\bullet(N \cap L) = 0$ であること、または再度 $\mu_L^\bullet(N \cap L) = 0$ であることを検証するだけで十分です。私たちは矛盾によって議論しよう。したがって、$\mu_L^\bullet(N \cap L) > 0$ と仮定します。 $L$と交差する$K \in \mathfrak{H}$の集合は可算であるため、$N \cap L$は$\mu_L$可測です。したがって、$\mu_L^\bullet(J) > 0$ となるような、$N \cap L$ に含まれるコンパクト集合 $J$ が存在します。 $S$ を非零メジャー $(\mu_L)_J = \mu_J$ のサポートとします。それは$N$に含まれており、$\mu_S$の小節は非零、$\mathrm{Supp}(\mu_S) = S$ (Ch. IV, §5, No. 7、補題 2) です。 集合 $\mathfrak{H} \cup \{S\}$ したがって、属するから $\mathscr{H}$ となり、$\mathfrak{H}$ の最大指標と矛盾します。これはクラッシュの存在を証明します。

(1) $\mu_\alpha$ が $\varphi_{K_\alpha} \cdot \mu$ の尺度であることは後で (§2, No. 2) わかります。

B) (7) の証明:
すべての $\alpha \in A$、$\mu_\alpha^\bullet(f) = \mu_{K_\alpha}^\bullet(f_{K_\alpha}) = \mu^\bullet(f \varphi_{K_\alpha})$ について、No. 3 の公式 (3) およびNo. 2 の提案 2 a) による。これらの公式は、負担 $\sum_{\alpha \in A} \mu_\alpha^\bullet$ が $\leq \mu^\bullet$ であることを示しており、したがって家族 $(\mu_\alpha)_{\alpha \in A}$ は合計可能です (No. 7、提案 7)。したがって、$\mu = \sum_{\alpha \in A} \mu_\alpha$、つまり公式を確立することを示すだけで十分です。
$$
\mu_K^\bullet = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet
$$
T のすべてのコンパクト部分集合 K に対して、K は固定されており、$K_\alpha$ が K と交差するような $\alpha \in A$ の集合 $A'$ は可算です。 $g \in \mathscr{F}_+(K)$ しましょう。次に $g^0 = g^0 \varphi_N + \sum_{\alpha \in A} g^0 \varphi_{K_\alpha}$、$g^0 \varphi_{K_\alpha} = 0$ が $\alpha \in A - A'$ になります。 No. 5 の提案 4 により、$\mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha})$, よってとなります。
$$
\mu_K^\bullet(g) = \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g^0) = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet(g);
$$
したがって、(8) が成立します。

C) 測定可能性:
T 上で定義された写像 $g$ が $\mu$ 可測であるためには、すべての $\alpha \in A$ について $\mu_\alpha$ が可測であることが必要かつ十分です (No. 7、提案 8)。しかし、これは、$g_{K_\alpha}$ がすべての $\alpha \in A$ (No. 5、例) に対して $\mu_{K_\alpha}$ 測定可能であることを意味するというになります。 Q.E.D.

第 14 章の提案 14 にあるように。 IV, §5, No. 9 では、事前に与えられた T のコンパクト部分集合の $\mu$ 密集合に対して、コンパクト集合 $K_\alpha$ から属するを要求できます。必要なのは次の結果のみであり、これを直接確立します。

#### 命題 10 {#int-ix-s1-prop-10 .statement tag=09NM}

— * g がトポロジカル空間 G (ハウスドルフかどうか) の値を伴う $\mu$ 可測写像である場合、制限 $g_{L_\beta}$ がすべての $\beta \in B$ に対して連続であるような T の $\mu$ 破砕 $(L_\beta)_{\beta \in B}$ が存在します。

$\mu$ に対する T の粉砕 $(K_\alpha)_{\alpha \in A}$ を考えてみましょう。 写像 $g$ は可測であるため、コンパクトな集合の数列 $(K_{\alpha n})$ と局所的に無視できる集合 $N_\alpha$ への $K_\alpha$ の各 $\alpha \in A$ 分割が存在します。 $g$の制限から集合$K_{\alpha n}$までは連続しています。その場合、家族$(K_{\alpha n})_{(\alpha, n) \in A \times \mathbf{N}}$が求められているのです。なぜなら、コンパクトな集合は最大でも可算無限大集合 $N_\alpha$ と交差するため、局所的に可算であり、集合 $N' = N \cup (\bigcup_\alpha N_\alpha)$ は局所的に無視できるからです。

#### スクリウム {#int-ix-s1-n8-sch-1 .statement tag=09NN}

— $(K_\alpha)_{\alpha \in A}$ を T のクラッシュとし、$N = T - \bigcup_\alpha K_\alpha$ とします。 We denote by $T'$ the locally compact space obtained by equipping $T'$ with the sum topology of the topologies of the subspaces $K_\alpha$ and any locally compact topology on $N$ (unless expressly mentioned to the contrary, $N$ will always be equipped with the discrete topology). それぞれの $\alpha \in A$ について、$i_\alpha$ を $K_\alpha$ から $T'$ への標準単射とし、$\mu'_\alpha$ を $T'$ における$i_\alpha$ の下の $\mu_{K_\alpha}$ の像とする。 ファミリ $(\mu'_\alpha)$ は加算可能です。つまり、$f$ がコンパクト サポートを備えた $T'$ 上の連続写像である場合、$\operatorname{Supp}(f)$ は添字 $\alpha$ の有限数のみで $K_\alpha$ と交差します。 私たちは集合 $\mu' = \sum_{\alpha \in A} \mu'_\alpha$です。 集合 $N$ は、$\mu'$ に対して局所的に無視できます。各 $\mu'_\alpha$ についても同様であるため (提案 9)、族 $(K_\alpha)_{\alpha \in A}$ は $T'$ の $\mu'$ 粉砕です。さて、$K_\alpha$ で $\mu'$ によって引き起こされる尺度は明らかに $\mu_{K_\alpha}$ と公式 (7) であり、$\mu$ と $\mu'$ に適用すると、$\mu^\bullet = {\mu'}^\bullet$ であることがわかります。 Similarly, the last assertion of the statement of Prop. 9, applied to $\mu$ and to $\mu'$, shows that *the measurable mappings are the same for the two measures $\mu$ and $\mu'$*.

これら 2 つの特性により、局所的にコンパクトな空間のために作成された$\mu$ から理論に関する積分理論のほぼすべてを削減できます。これらの考慮事項は、No. 10 で開発されます。

粉砕の概念を他の応用したものは次のとおりです。

#### 命題 11 {#int-ix-s1-prop-11 .statement tag=09NO}

*$X$ を $T$ の $\mu$ で測定可能な部分集合とします。 $X - \bigcup_{\alpha \in A} L_\alpha$ が局所的に $\mu$ 無視できるような、$X$ のコンパクト部分集合のペアごとの互いに素の局所的に可算な族 $(L_\alpha)_{\alpha \in A}$ が存在します。 If, in addition, $X$ is the union of a sequence $(X_n)$ of measurable sets such that $\mu^\bullet(X_n) < +\infty$, then the set $B$ of $\alpha \in A$ such that $\mu^\bullet(L_\alpha) \neq 0$ is countable, and $X - \bigcup_{\beta \in B} L_\beta$ is locally $\mu$-negligible.*

$f$ を $X$ の特徴写像とし、$(K_\alpha)_{\alpha \in A}$ を $f$ の $K_\alpha$ のそれぞれに対する制限が連続となるような $T$ の破砕とする (提案 10)。 集合 $L_\alpha = K_\alpha \cap X$ は、$\alpha \in A$ ごとにコンパクトになり、$(L_\alpha)_{\alpha \in A}$ が目的のファミリになります。 2 番目の主張に進みましょう。測定可能な集合 $X_n$ は明らかに互いに素であると仮定でき、それぞれに対して主張を確立するだけで十分です。他の語では、必要に応じて記法を変更して、$\mu^\bullet(X) < +\infty$とすることができます。 $\alpha \in A$ の集合 $B$ により、$\mu^\bullet(L_\alpha) > 0$ は可算となり、集合 $N = \bigcup_{\alpha \in A - B} L_\alpha$ が局所的に無視できることを証明するだけです。しかし、$K$ はコンパクトな集合です。家族 $(L_\alpha)_{\alpha \in A}$ は局所的に可算であり、集合 $K \cap N$ は家族 $(K \cap L_\alpha)_{\alpha \in A - B}$ の *可算* サブファミリーの和集合であり、したがってこの集合は局所的に無視できます。 $N$ (No. 2、提案 2) についても同様であり、命題が成立します。

### 9. 上部積分

#### 定義 11 {#int-ix-s1-def-11 .statement tag=09NP}

*すべての写像 $f \in \mathscr{F}_+(T)$ に対して、1 つの定義する $f$ の上積分 (メジャー $\mu$ に関して) が有限または無限の正の数*

$$
\mu^*(f) = \inf_g \mu^\bullet(g),
$$

*ここで、$g$ は、$\geqslant f$ である下位の半連続写像の集合を上回ります。*

記法 $\int^* f(t) d\mu(t)$ および $\int^* f d\mu$ も使用されます。 $T$ が局所的にコンパクトな場合、この定義一致するは通常の定義となります (Ch. V, §1, No. 1、提案 4)。明らかに$\mu^\bullet(f) \leqslant \mu^*(f)$、$f$が下位半連続の場合は等式です。 $A$が$T$の部分集合である場合、$\mu^*(\varphi_A)$の代わりに$\mu^*(A)$と書き、この数を$A$の*外側メジャー*と呼びます。有限の外測度を持つ可測集合は、局所的にコンパクトな空間の場合と同様、 *可積分集合* と呼ばれます。

写像 $f$ とバナッハ空間または $\overline{\mathbf{R}}$ の値で、$\mu^*(|f|) = 0$ は *無視できる* と言われます。 $\varphi_A$ が無視できる場合、つまり $\mu^*(A) = 0$ の場合、集合 $A \subset T$ は無視できると言われます。 「ほぼどこでも」という表現は、第 3 章のように導入されています。 IV, §2, No. 3。

#### 命題 12 {#int-ix-s1-prop-12 .statement tag=09NQ}

*写像 $\mu^*$ は $T$ の負担です。*

Def のプロパティ $a), b), c)$ No. 1 のうち 1 つは明らかです。 性質の証明 d)はThのものと同一です。第3章IV, §1, No. 3、小道具を考慮する場合。 4 と 5 *a)*。

#### 系 {#int-ix-s1-n9-cor-1 .statement tag=09NR}

*写像 $f$ は、バナッハ空間または $\overline{\mathbf{R}}$ に値が含まれており、ほぼどこでも $f(t) = 0$ である場合にのみ無視できます。*

簡約するが 1 つあれば、すぐに写像が陽性となります。 証明は Th のそれと同一になります。 1章IV, §2, No. 3。

#### 命題 13 {#int-ix-s1-prop-13 .statement tag=09NS}

* $T$ の各部分集合 $A$ について、$\mu^*(A)$ は、オープン集合含む $A$ の外側の寸法の下限です。

証明は、第 2 章の提案 19 と同じです。 IV, §1, No. 4。

#### 定義 12 {#int-ix-s1-def-12 .statement tag=09NT}

*$f$ を $T$ で定義された写像とし、バナッハ空間または $\overline{\mathbf{R}}$ で値を定義します。 $f$ が可算開集合の可算和集合の補数で零である場合、$f$ は$\mu$ の尺度に対して緩和される、または $\mu$ が緩和されると言われます。 写像 $\varphi_A$ が緩和されると、$T$ の部分集合 $A$ が緩和されると言われます。 写像 $1$ が $\mu$ で緩和される場合、$\mu$ の措置は緩和されると言われます。*

たとえば、制約 $\mu^\bullet$ は局所的に有界されているため、$T$ のすべてのコンパクト部分集合 $K$ は、$\mu^\bullet(V) < +\infty$ のように開いた集合 $V$ に含まれます。したがって、コンパクト集合の外側の零である写像は緩和されます。無視できるほどの写像が緩和されます。 注意 Defに続きます。第2章V, §1, No. 2 は、現在の文脈にすぐに拡張できます。特に、モデレートポジティブ写像の数列の和はモデレートです。

#### 注意 1 {#int-ix-s1-n9-rem-1 .statement tag=09NU}

リンデロフ空間 T (TG、IX、付録 I、定義 1)¹、特にスースリン空間 (同上、提案 1 の修正) では、すべての措置が緩和されます。なぜなら、T の範囲である有限尺度形の開いた集合から、T の可算範囲を抽出できるからです。

#### 注意 2 {#int-ix-s1-n9-rem-2 .statement tag=09NV}

ただし、和集合 T を持つ、$\mu$ に対する有限尺度の Borel 集合の数列の存在は、和集合 T を持つ有限尺度のオープン集合の数列の存在を必ずしも意味するわけではないことに注意してください。 語、$\mu$ が緩和されていることを意味するものではありません）。エクサーを参照してください。 8.

#### 命題 14 {#int-ix-s1-prop-14 .statement tag=09NW}

$f \in \mathscr{F}_+(T)$ にしましょう。 $f$ が $\mu$ で調整されている場合、$\mu^*(f) = \mu^\bullet(f)$。 $f$ が $\mu$ で管理されていない場合は、$\mu^*(f) = +\infty$ です。

$\mu^*(f) < +\infty$ の場合、$\mu^\bullet(g) < +\infty$ のような下位の半連続写像 $g \geq f$ が存在します。すべての $n \in \mathbf{N}$ について、$G_n$ を $t \in T$ の集合とし、$g(t) > 1/n$ とします。 集合 $G_n$ はオープンで、1 つは $\mu^\bullet(G_n) \leq n \mu^\bullet(g) < +\infty$ で、$f$ は $G_n$ の和集合の外側にある零です。したがって、写像 $f$ は緩和されます。

次に、$\mu^*$ と $\mu^\bullet$ が、モデレートされた写像に対して同じ値を持っていることを示します。 $\mu^*$ と $\mu^\bullet$ は制約であるため、$f$ が定数 M で囲まれた正の写像であり、有限尺度の開いた集合 G の外側に零がある場合、関係 $\mu^*(f) = \mu^\bullet(f)$ を確立するだけで十分です。それをこれからやります。

$\mu$ は、$\mathscr{M}(T)$ における、コンパクトなサポートを備えた増加する有向族 $(\mu_i)_{i \in I}$ の最高値です。これは、No. 8 の提案 9 からすぐに続きます。 $g$ を T 上の下位半連続写像とし、$f$ と下位半連続写像 $M \varphi_G$ の間にあります。 集合 $\nu_i = \mu - \mu_i$;次に $\mu^\bullet = \mu_i^\bullet + \nu_i^\bullet$ (No. 2, 注意 1)、結果的に
$$
\mu^\bullet(g) - \mu^\bullet(f) = (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + (\nu_i^\bullet(g) - \nu_i^\bullet(f))
$$
$$
\leq (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + \nu_i^\bullet(M \varphi_G).
$$
1 つは $\nu_i^\bullet(M \varphi_G) = \mu^\bullet(M \varphi_G) - \mu_i^\bullet(M \varphi_G)$ と $\mu^\bullet(M \varphi_G) = \sup \mu_i^\bullet(M \varphi_G)$ です (No. 7、提案 6)。従って、数 $\nu_i^\bullet(M \varphi_G)$ は、$i$ の適切な選択によって任意に小さくすることができます。従って、すべては、任意の数 $c > 0$ と任意の添字 $i \in I$ について、$f$ と $M \varphi_G$ の間の下位半連続写像 $g$、例えば $\mu_i^\bullet(g) - \mu_i^\bullet(f) \leq c$ を見つけることができることを示すことに帰着します。ここで、L をメジャー $\mu_i$ のコンパクトサポートとし、$\lambda$ をメジャー $(\mu_i)_L$ とします。 $\mu_i$ は L に集中しているため、写像 $h \in \mathscr{F}_+(T)$ ごとに $\mu_i^\bullet(h) = \mu_i^\bullet(h \varphi_L) = \lambda^\bullet(h_L)$ が存在します (No. 1、補題 1 および No. 2、提案 2)。従って
$$
\mu_i^\bullet(g) - \mu_i^\bullet(f) = \lambda^\bullet(g_L) - \lambda^\bullet(f_L).
$$

¹ TG で引用されている付録は、GT (第 3 章の初期版を翻訳したもの) には登場しません。 IX)。 リンデロフ空間は GT、I, §9、Exer で定義されています。 14; Souslin 空間 (GT、IX, §6, No. 2、Def. 2) のこの練習問題と定義が、ここで必要な素材をカバーしています。

でも、Lはコンパクトです。従って、$\lambda^* = \lambda^*$、その結果、L に定義された下位の半連続写像 $h$、つまり $\geq f_L$ が存在し、$\lambda^*(h) \leq \lambda^*(f_L) + c$ となります。 集合 L が T で閉じているため、写像 k は、L では h に等しく、$T - L$ では $+\infty$ に等しく、T では下位の半連続であり、$\geq f$ と $\lambda^*(k_L) = \lambda^*(h) \leq \lambda^*(f_L) + c$ です。 集合 $g = \inf(k, M \varphi_G)$ までのみ残ります: $g$ は下位半連続、$g \geq f$ と

$$
\mu_i^*(g) \leq \mu_i^*(k) = \lambda^*(k_L) \leq \lambda^*(f_L) + c = \mu_i^*(f) + c.
$$

#### 系 1 {#int-ix-s1-prop-14-cor-1 .statement tag=09NX}

*写像が無視できるためには、それが局所的に無視でき、緩和されることが必要かつ十分です。*

#### 系 2 {#int-ix-s1-prop-14-cor-2 .statement tag=09NY}

*写像 $f$ が局所的に無視できるためには、すべての $x \in T$ が $f \varphi_V$ が無視できるような近傍 V を所有することが必要かつ十分です。

なぜなら、この性質が満たされる場合、$f \varphi_K$ はすべてのコンパクト集合 K に対して無視でき、従って $f$ は局所的に無視できるからです (No. 2、提案 2)。逆に、$f$ が局所的に無視できると仮定し、$x$ を T の点とします。 $x$ は、有限の尺度の開かれた近隣地域 V を認めます。 写像 $f \varphi_V$ は局所的に無視でき、緩和されているため、無視できます。

#### 系 3 {#int-ix-s1-prop-14-cor-3 .statement tag=09NZ}

*$f$ を T で定義された緩和された写像とします。ペアごとの互いに素コンパクト集合の数列 $(K_n)$ と、$f = f \varphi_H + \sum_n f \varphi_{K_n}$ などの無視できる集合 H が存在します。

For, let G be a set that is a countable union of integrable open sets, such that $f$ is zero outside G; then G is the union of a sequence $(K_n)$ of pairwise disjoint compact sets and a locally negligible set H (No. 8, Prop. 11); but H is moderated, therefore negligible.

#### 系 4 {#int-ix-s1-prop-14-cor-4 .statement tag=09O0}

*$\mu$ と $\nu$ が $\mu^* = \nu^*$ となるような T 上の 2 小節である場合、$\mu = \nu$ となります。*

なぜなら、等式 $\mu^* = \nu^*$ は、すべてのポジティブな写像 $f$ に対して $\mu^*(f) = \nu^*(f)$ が、$\mu$ と $\nu$ に対して緩和され、したがってコンパクトなサポートを持つすべてのポジティブな写像に対してであることを意味します。したがって、$\mu^* = \nu^*$ (No. 2、提案 2)、次に $\mu = \nu$ (No. 2、提案 2 の修正) となります。

#### 系 5 {#int-ix-s1-prop-14-cor-5 .statement tag=09O1}

*$\mu$ が T の緩和された措置である場合、$\mu = \sum_{n \in \mathbf{N}} \mu_n$ のようなコンパクトなサポートを持つ措置の数列 $(\mu_n)_{n \in \mathbf{N}}$ が存在します。

仮定までに、定数写像 1 は $\mu$ で緩和されます。 Cor を適用してみましょう。 3 ケース$f = 1$;したがって、$1 = \sum_{n \in \mathbf{N}} \varphi_{K_n}$ $\mu$-ほぼどこにでも、T のペアワイズ互いに素コンパクト部分集合の数列 $(K_n)_{n \in \mathbf{N}}$ が存在します。 $\mu_n$ を、$K_n$ のメジャー $\mu_{K_n}$ (No. 3, 例 2) によって定義される T のメジャーとします。 (No. 6、注意 2) $\mu_n$ にはコンパクトなサポートがあり、$f \in \mathscr{F}_+(T)$ には $\mu_n^\bullet(f) = \mu^\bullet(f \varphi_{K_n})$ が含まれていることはわかります。さて、$f$ は $\sum_{n \in \mathbf{N}} f \varphi_{K_n}$ $\mu$ とほぼどこでもよってに等しくなります。

$$
\mu^\bullet(f) = \sum_{n \in \mathbf{N}} \mu^\bullet(f \varphi_{K_n}) = \sum_{n \in \mathbf{N}} \mu_n^\bullet(f).
$$

したがって、$\mu = \sum_{n \in \mathbf{N}} \mu_n$ (No. 7、提案 7) となります。

### 10. 統合理論

#### 定義 13 {#int-ix-s1-def-13 .statement tag=09O2}

— *しましょう* $p \in [1, +\infty[$; *1 は、* $\overline{\mathscr{L}}^p(T, \mu)$ *(それぞれ* $\overline{\mathscr{L}}_F^p(T, \mu)$ *F がバナッハ空間の場合) 写像* の集合 $\mathbf{f}$ *T を* $\overline{\mathbf{R}}$ *(それぞれ F に) $\mu$ 可測であり、 満たす* $\mu^\bullet(|\mathbf{f}|^p) < +\infty$。 *1 は、* $\mathscr{L}^p(T, \mu)$ *(それぞれ* $\mathscr{L}_F^p(T, \mu)$*) 集合の $\mu$ モデレート元の* $\overline{\mathscr{L}}^p(T, \mu)$ *(それぞれ* $\overline{\mathscr{L}}_F^p(T, \mu)$*)* を表します。

$\overline{N}_p(\mathbf{f}) = \left( \mu^\bullet(|\mathbf{f}|^p) \right)^{1/p}$、$N_p(\mathbf{f}) = \left( \mu^*(|\mathbf{f}|^p) \right)^{1/p}$と書きます。 $\overline{N}_\infty(\mathbf{f})$ によって、数 $k \geq 0$ が局所的に $|\mathbf{f}| \leq k$ - ほぼどこでも$\mu$ となるような下限を表します。 $\overline{N}_\infty(\mathbf{f}) < +\infty$ の場合、$\mathbf{f}$ は本質的に有界であると言われます。 The set of measurable and essentially bounded mappings of T into $\overline{\mathbf{R}}$ (resp. into F) is denoted $\overline{\mathscr{L}}^\infty(T, \mu)$ (resp. $\overline{\mathscr{L}}_F^\infty(T, \mu)$). The elements of $\overline{\mathscr{L}}_F^1(T, \mu)$ (resp. $\mathscr{L}_F^1(T, \mu)$) are called essentially integrable functions (resp. integrable functions) with values in F.

$\mu$ が複素数値の場合、1 つの集合

$$
\overline{\mathscr{L}}_F^p(T, \mu) = \overline{\mathscr{L}}_F^p(T, |\mu|) \quad \text{and} \quad \mathscr{L}_F^p(T, \mu) = \mathscr{L}_F^p(T, |\mu|).
$$

混乱を招かない限り、上記の記法は、$\overline{\mathscr{L}}_F^p(\mu)$、$\overline{\mathscr{L}}_F^p$ または $\mathscr{L}^p(\mu)$、$\mathscr{L}^p$ と省略されることがよくあります。

No. 8 (*Scholium*) で、T と同じ集合と T よりも位相より細かいを持ち、ローカルにコンパクトな空間 T' を構成するでき、T' に次のような尺度 $\mu'$ を装備できることがわかりました。 $\mu$ 可測写像と $\mu'$ 可測写像は同じであり、$\mu$ と $\mu'$ の正の写像の本質的な上積分が等しいようになります。したがって、集合 $\overline{\mathscr{L}}_F^p(\mu)$ と $\overline{\mathscr{L}}_F^p(\mu')$ は $1 \leq p \leq +\infty$ $^{(1)}$ に対して同一であることがわかります。これは、新しい証明がなければ、$\overline{\mathscr{L}}_F^p$がベクトル空間であり、写像$\overline{N}_p$が$\overline{\mathscr{L}}_F^p(\mu)$の準標準であり、この空間が完全であることも意味します。

$\mathbf{f}$ を $\overline{\mathscr{L}}_F^p$ ($1 \leq p < +\infty$) の元とします。 $\mu^\bullet(|\mathbf{f}|^p) = {\mu'}^\bullet(|\mathbf{f}|^p) < +\infty$、第 7 章の提案 7 があるため。 V, §1, No. 2 は、$\mathbf{f}$ が零の外側であることを意味します

(1) 空間 $\mathscr{L}_F^p(\mu)$ は $\mathscr{L}_F^p(\mu')$ に含まれていますが、一般にそれとは区別されることに注意してください。

コンパクトな T' の部分集合の数列の和集合と、局所的には無視できる $\mu'$ の集合。後者の集合は局所的に $\mu$ 無視でき、T' のすべてのコンパクト部分集合は T 内でコンパクトなので、f は局所的に $\mu$- ほぼどこでも $\mu$ 緩和された写像に等しいということになります。局所的に無視できる $\mu$ (無視できる $\mu$) 写像の $\overline{\mathscr{N}}_F$ (それぞれ $\mathscr{N}_F$) 空間で表しましょう。したがって、$\overline{\mathscr{L}}_F^p = \mathscr{L}_F^p + \overline{\mathscr{N}}_F$ と $\mathscr{N}_F = \mathscr{L}_F^p \cap \overline{\mathscr{N}}_F$ が得られます (No. 9、提案 14 のコリント 1)。したがって、空間 $\overline{\mathscr{L}}_F^p / \overline{\mathscr{N}}_F$ は正規的に $\mathscr{L}_F^p / \mathscr{N}_F$ と識別される可能性があり、この識別がノルムを保持していることがすぐに検証されます。この商空間は $L_F^p(\mu)$ と表されます。これは、半正規化された空間 $\overline{\mathscr{L}}_F^p(\mu)$ および $\mathscr{L}_F^p(\mu)$ のそれぞれに関連付けられた正規化された空間として解釈できます。 $\overline{\mathscr{L}}_F^p$ は完了しているため、$L_F^p$ と $\mathscr{L}_F^p$ も同様です。

写像 f の集合は F に値があり、コンパクトなサポートで T' に連続しており、$\overline{\mathscr{L}}_F^p(\mu') = \overline{\mathscr{L}}_F^p(\mu)$ では密集しています (Ch. IV, §3, No. 4、定義 2)。 No. 8のスコリウムの記法を再び取り上げてみましょう。 T' のコンパクト部分集合は、コンパクト集合 $K_\alpha$ の有限数とのみ交差するため、コンパクト サポートを使用した T' 上のすべての連続写像 f は、和として記述できます。
$$
f = \sum_{\alpha \in A} f_\alpha + g,
$$
ここで、$f_\alpha$ は、$\alpha$ ごとに、$K_\alpha$ 上の連続写像の 0 による拡大です。$f_\alpha = 0$ は、添字の有限数を除き、g はローカルです。 $\mu$-無視できます。したがって、次の結果が得られます。

#### 命題 15 {#int-ix-s1-prop-15 .statement tag=09O3}

*F に値を含む写像 f の集合は、Supp(f) がコンパクトであり、f の制限から Supp(f) までが連続であるように、$\overline{\mathscr{L}}_F^p(\mu)$ と $\mathscr{L}_F^p(\mu)$ で$1 \leq p < +\infty$ が密です。*

これらの写像は、コンパクト サポートを備えた *T 上で連続した写像 *ではない*ことに注意してください。

積分の定義に進みましょう。

#### 命題 16 {#int-ix-s1-prop-16 .statement tag=09O4}

*F には、次の性質を持つ空間 $\overline{\mathscr{L}}_F^1(\mu)$ のうち、連続する線形写像 $f \mapsto \int f d\mu$ が 1 つだけ存在します。
f が形 $t \mapsto g(t)a$ で、$a \in F$ で、g が正の写像で、有限で $\mu$ 可測で、$\mu^*(g) < +\infty$ の場合、$\int f d\mu = \mu^*(g) \cdot a$ となります。*

なぜなら、半正規化された空間 $\overline{\mathscr{L}}_F^1(\mu)$ と $\overline{\mathscr{L}}_F^1(\mu')$ は同一だからです。 $\mu^* = {\mu'}^*$ より、写像 $f \mapsto \int f d\mu'$ は主張の条件を満たします。一方、主張で検討した形$f = g \cdot a$の写像の集合は、$\overline{\mathscr{L}}_F^1(\mu')$（IV, §3, No. 5案10）、よって一意性の*合計*です。

$\int f\, d\mu$ は $\mu$ に関する $f$ の積分であると言われており、このベクトルは $\mu(f)$ または $\int f(t)\, d\mu(t)$ とも表されます。

$F$ の値を含む本質的にすべての可積分関数 $f$ について $\int f\, d\mu = \int f\, d\mu'$ であるため、新しい証明なしで、ハウスドルフ空間上の測度に対する必須積分拡大するのすべての理論が計算されます。そこから、緩和された写像に制限することで、通常の積分と比較した結果を推定します。特に次の結果を引用します。

— て。第3章 IV, §3, No. 4、その拡大から $\overline{\mathscr{L}}_F^p$、そしてその 2 つの帰結。
— て。第4章 IV, §3, No. 5 (合成と連続した線形写像) およびその結果。 小道具。同No.の9、11、12。
— Ch.の結果はすべて $L^p$ の順序付けられたベクトル空間構造に対する IV, §3, No. 6。
— Ch.の結果はすべて IV, §3, No. 7、特にルベーグの定理。
— Ch.の結果はすべて IV, §3, No. 8、空間 $L_F^p$ の間の関係に。
— 定理 2章 IV, §4, No. 3 ($L_F^1$ に固有のルベーグの定理の主張)。
— ヘルダーの不等式 (Ch. IV, §6, No. 4、木。 2) とその結果。
— 空間 $L_F^p$ の間の関係が第 3 章で確立されました。 IV, §6, No. 5。
— 第 2 章で確立された空間 $L^p$ の双対性に関する結果。 V, §5, No. 8。
— ダンフォード・ペティス定理 (Ch. VI, §2, No. 5、木。 1)、その系譜 1 と 2、および第 3 章の提案 10。 VI, §2, No. 6 ($L_F^1$ の双数)。

### 練習問題 {#int-ix-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
