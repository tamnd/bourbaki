---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 1
section_title: Bornology in a topological vector space
lang: ja
source: evt-i-v
pdf_pages: 0133-0143, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Bornologies
      page: 0
      pdf_page: 133
    - "no": 2
      title: Bounded subsets of a topological vector space
      page: 2
      pdf_page: 134
    - "no": 3
      title: Image under a continuous mapping
      page: 4
      pdf_page: 136
    - "no": 4
      title: Bounded subsets in certain inductive limits
      page: 5
      pdf_page: 137
    - "no": 5
      title: The spaces $E_A$ (A bounded)
      page: 7
      pdf_page: 139
    - "no": 6
      title: Complete bounded sets and quasi-complete spaces
      page: 8
      pdf_page: 140
    - "no": 7
      title: Examples
      page: 9
      pdf_page: 141
statements: 30
exercises: 18
content_sha256: 1a7149d72b5ea7e3c47b9fef6f1893cfe97c5d83d82e3f957aecb9b2da56239b
translated_from: content/en/evt/III/01_s1_bornology_in_a_topological_vector_space.md
translation_method: google
source_content_sha256: 4e7875bd1f38c0a02c517e1a85849c5df0ef1b2158b71d579dbe784bbc3c6f54
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 902abf301c6e3e613d1ae25760a9294f7639564d5ec05fd863d4f8e8ae76fbd8
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。トポロジーにおけるボーンロジー ベクトル空間

### 1. 系統学

#### 定義 1 {#evt-iii-s1-def-1 .statement tag=07KW}

— *集合* $E$ の生まれつき学は、部分集合* $\mathscr{B}$ *すべての集合のうち部分集合 $E$ *満たす次の条件* (cf. GT、X, § 1.2、 注意 2）。
(B1) *$\mathscr{B}$ *属するから * $\mathscr{B}$ の集合の部分集合ごと。
(B2) *$\mathscr{B}$ *属するから* $\mathscr{B}$ の集合のすべての有限和集合。

*We say that* $\mathscr{B}$ *is covering if every element of* $E$ *is contained in a set which belongs to* $\mathscr{B}$, *or, which is the same, if* $\mathscr{B}$ *is a cover of* $E$.

#### 例 {#evt-iii-s1-n1-exa-1 .statement tag=07KX}

— Let E be a metric space; the set of all bounded subsets of E (GT, IX, § 2, No. 2) is a covering bornology on E. Let G be the group of isometries of E; the set of all subsets M of G such that for every $x \in E$, the set $M.x$ is a bounded subset of E, is a covering bornology on G.

If $\mathscr{B}$ is a bornology on a set E, a subset $\mathscr{B}_1$ of $\mathscr{B}$ is said to be a *base* of $\mathscr{B}$ if every set of $\mathscr{B}$ is contained in a set of $\mathscr{B}_1$.

E の系統学ファミリーの共通部分は系統学です。従って、$\mathfrak{P}(E)$ の部分集合 $\mathfrak{S}$ ごとに、最小のの生まれ方含む $\mathfrak{S}$ が存在します。この生まれつき学は $\mathfrak{S}$ によって*生成される* と言われており、$\mathfrak{S}$ の集合の有限和集合の基底集合であると認められます。 E と E' が 2 つの集合と $\mathscr{B}$ (それぞれ $\mathscr{B}'$) が E (それぞれ E') 上の骨学である場合、積の骨学は集合 $M \times M'$ を基底として認める $E \times E'$ 上の骨学であり、ここで $M \in \mathscr{B}$ と$M' \in \mathscr{B}'$。

#### 定義 2 {#evt-iii-s1-def-2 .statement tag=07KY}

※$E$をベクトル空間とします。 $E$ 上のボーンロジー $\mathscr{B}$ は、すべての $X \in \mathscr{B}$ と $t \in K$ について、相補的集合 $tX$ と、$X$ の凸状の平衡包絡線 $\Gamma(X)$ (II, p. 10) が一致する場合、凸であると言われます。 属する ～ $\mathscr{B}$.*

$X$ と $Y$ が $E$ の 2 つの部分集合である場合、次のようになります。
$$
X + Y \subset 2\Gamma(X \cup Y)
$$
$$
\lambda X \subset t\Gamma(X) \quad \text{for} \quad |\lambda| \leq t .
$$

従って、$\mathscr{B}$ が $E$ 上の凸ボーンロジーである場合、$A$ が $K$ の有界部分集合である場合、$X, Y$ 属するから $\mathscr{B}$ である場合、$X + Y \in \mathscr{B}$ と $A.X \in \mathscr{B}$ になります。

### 2. トポロジカルベクトル空間の有界部分集合

#### 定義 3 {#evt-iii-s1-def-3 .statement tag=07KZ}

*$E$をトポロジカルベクトル空間とします。 $E$ の部分集合 $A$ は、$E$ (I、p. 7、定義 4) の $0$ のすべての近傍によって吸収される場合、有界であると言われます。

$A$ が制限される位数では、$A$ が $0$ の近傍の基本的な系のすべての近傍によって吸収されるだけで十分です。 Since there exists a fundamental system of balanced neighbourhoods of $0$ (I, p. 7, prop. 4), this is the same as saying that, for every neighbourhood $V$ of $0$ in $E$, there exists $\lambda \in K$ such that $A \subset \lambda V$.

$E$ の位相が準規範 (II、p. 3) の基本系 $\Gamma$ によって定義されているとします。その場合、すべての準ノルム $p \in \Gamma$ が $A$ で制限される場合に限り、$E$ の部分集合 $A$ は制限されます。

特に、$E$ が半正規化された空間である場合、$E$ の部分集合 $A$ は、ボールに含まれる場合に限り、有界となります。他の語では、$E$ がノルムである場合、これは $A$ が $E$ (GT、IX, § 2, No. 2) の計量空間構造で制限されることを意味します。

#### 注意 {#evt-iii-s1-n2-rem-1 .statement tag=07L0}

— 1) $E$ が半正規化空間である場合、ボール形は、$E$ の$0$ の有界近傍の基本系です。逆に、$E$ が局所凸トポロジベクトル空間で、$E$ に $0$ の有界近傍が存在する場合、この近傍含むは凸平衡近傍 $W$ であり、ゲージは$W$ は、$E$ の位相を定義する準ノルムになります。

したがって、$E$ が局所的に凸で計量可能であり、その位相できないが単一のノルムによって定義される場合、位相を定義する$E$ 上には距離が存在せず、$d$ の有界部分集合は存在しません (GT, IX, § 2, No. 2) は、$E$ の有界な部分集合です。より正確には、平行移動不変で、$E$の定義する位相の$E$上のすべての距離$d$について、$E$の有界部分集合は$d$に有界されます（III、p. 38、実行）。 3) ですが、逆は誤りです。

2) $M$ を、誘導された位相を備えた $E$ のベクトル部分空間とします。 位数において、$M$の部分集合が$M$で拘束されることは、$E$で拘束されることが必要十分です。

3) $N$ を $E$ の $0$ のすべての近傍の共通部分とすると、$\tilde{E} = E/N$ は $E$ に関連付けられたハウスドルフベクトル空間になります。次に、$N$ は有界です。 $\pi : E \to \tilde{E}$ が標準準同型の場合、$\pi(B)$ が有界である場合に限り、$E$ の部分集合 $B$ は有界となります。

4) $E$ を局所凸ハウスドルフ空間とします。その場合、$E$ のすべての $x \neq 0$ に対して、$p(x) \neq 0$ となるような連続的な半ノルム $p$ が存在します。この準ノルムは、$x$ によって生成される実際の半直線 $\mathbf{R}_+ . x$ で制限されません。したがって、$E$ の非 null 部分空間は制限されません。特に、境界のある部分集合はどの線も含むではありません。

#### 定義 4 {#evt-iii-s1-def-4 .statement tag=07L1}

*$E$を局所凸空間とする。 $E$ 上のボーンロジー $\mathscr{B}$ は、凸型の場合、$E$ の有界な部分集合で構成され、$\mathscr{B}$ 属するから $\mathscr{B}$ までのすべての集合の閉包があれば、$E$ に適応されると言われます。

#### 命題 1 {#evt-iii-s1-prop-1 .statement tag=07L2}

*$E$を局所的に凸な空間とする。 $E$ の境界のある部分集合の集合は、適応されたボーンロジーです。*

次のプロパティを確立する必要があります。
a) $B$ が $E$ の有界部分集合である場合、$B$ のすべての部分集合は有界です。
b) 2 つの有界部分集合のうち和集合は有界です。
c) 有界の集合と相似であるすべての集合は有界です。
d) 有界部分集合の閉じた凸平衡エンベロープ (II、p. 13) は有界です。
$p$が$E$の連続半ノルムである場合、$p$の玉は凸でバランスが取れており、閉じており、集合は玉と相似で玉です。したがって、$p$ が $E$ の 2 つの部分集合 $X$ と $Y$ に境界がある場合、$X \cup Y$ の閉じた凸平衡包絡線にも境界があり、これらと相似な集合にも境界があります。これにより、特性 $b), c)$ と d) が確立され、a) は明らかです。

#### 定義 5 {#evt-iii-s1-def-5 .statement tag=07L3}

*$E$を局所凸空間とする。 $E$ の境界のあるすべての部分集合のうち集合は、$E$ の標準ボーンロジーと呼ばれます。

$\mathscr{B}$ が $E$ の有界部分集合の集合である場合、$E$ と含む $\mathscr{B}$ に適応した最小の生まれ変わり $\tilde{\mathscr{B}}$ が存在します。 $\tilde{\mathscr{B}}$の集合は、$\mathscr{B}$の集合の有限和集合の閉じた凸平衡包絡線に相似な集合に含まれるものです。

適応されたすべてのボーンロジーは、標準的なボーンロジーに含まれています。

#### 命題 2 {#evt-iii-s1-prop-2 .statement tag=07L4}

*局所凸型空間 $E$ では、すべてのプリコンパクト集合は有界です。
$A$ を $E$ の事前圧縮部分集合とし、$V$ を $0$ の凸平衡近傍とします。次のような有限列 $(a_i)_{1 \leq i \leq n}$ 点 $A$ が存在します。
$$
A \subset \bigcup_{1 \leq i \leq n} (a_i + V).
$$
$B = \{a_1, ..., a_n\}$ は有界であるため、$0 < \lambda < 1$ と $\lambda B \subset V$ のようなスカラー $\lambda$ が存在します。 $\lambda A \subset \lambda B + \lambda V \subset V + V$ があり、そこから命題が続きます。

#### 系 {#evt-iii-s1-n2-cor-1 .statement tag=07L5}

*局所凸型の空間、コーシー 数列の点の集合は有界です。
実はこの集合はプリコンパクト（GT、II, § 4, No. 2）です。

#### 注意 5 {#evt-iii-s1-n2-rem-5 .statement tag=07L6}

— 一般に、局所凸型空間 $E$ の有界部分集合は、すべてが事前コンパクトではありません (たとえば、$E$ が無限次元ノルム空間である場合、その単位元ボールはコンパクトではありません (I, p. 15, th. 3))。ただし、これは、$E$ が弱い空間 (II, p. 42) の場合に当てはまります。E に関連付けられたハウスドルフ位相幾何学ベクトル空間は、有界部分集合がプリコンパクトである積 K^l の部分空間と同型です。 (*cf.* III、p. 4、cor. 2)。
その他の例についてはIV、p. 18をご覧ください。

#### 命題 3 {#evt-iii-s1-prop-3 .statement tag=07L7}

— *A を局所的に凸な空間 E の部分集合とします。 A が有界であると仮定します。次に、A の点のすべての数列 (x_n) と、0 になる傾向のあるスカラーのすべての数列 (\lambda_n) について、数列 (\lambda_n x_n) は 0 になる傾向があります。 逆に、A の点のすべての数列 (x_n) に対して、数列 (\lambda_n x_n) が制限されるようなゼロ以外のスカラーの数列 (\lambda_n) が存在する場合、A は制限されます。*

A が有界であると仮定します。 (\lambda_n) が 0 に向かうスカラーの数列であり、 V が 0 の近傍である場合、n が十分に大きいときは常に \lambda_n A \部分集合 V が得られ、最初の主張が続きます。

逆に、A が有界でなく、(\lambda_n) がスカラー \neq 0 の数列である場合、$p(x_n) \geq \frac{n}{|\lambda_n|}$ となるような、A の点の連続半ノルム p と数列 (x_n) が存在します。すると、$p(\lambda_n x_n) \geq n$ と数列 (\lambda_n x_n) は有界ではないことがわかります。

#### 系 {#evt-iii-s1-n2-cor-2 .statement tag=07L8}

— *部分集合 E の A は、A のすべての可算部分集合が有界である場合に限り、有界となります。*

### 3. 像連続写像の下

#### 命題 4 {#evt-iii-s1-prop-4 .statement tag=07L9}

— *E と F を 2 つの局所凸空間とし、f : E \to F を連続写像とします。 f(0) = 0 であり、すべての \lambda > 0 に対して f(\lambda x) = \lambda^m f(x) となるような実数 m \geq 0 が存在すると仮定します。そして、A が E の有界部分集合である場合、f(A) は F で有界になります。

実際、F で V が 0 の近傍である場合、E では $f^{-1}(V)$ は 0 の近傍です。A が E で有界である場合、A \部分集合 \lambda f^{-1}(V) となる \lambda > 0 が存在し、これは $f(A) \subset \lambda^m V$ を意味します。

#### 系 1 {#evt-iii-s1-prop-4-cor-1 .statement tag=07LA}

— *E と F を 2 つの局所凸空間とし、u : E \to F を連続線形写像とします。 A が E の有界部分集合である場合、u(A) は F で有界になります。

#### 系 2 {#evt-iii-s1-prop-4-cor-2 .statement tag=07LB}

— *E = \prod_{i \in I} E_i を局所凸型空間の族の積とします。次に、E の部分集合は、そのすべての射影が有界である場合に限り、有界となります。*

より一般的には:

#### 系 3 {#evt-iii-s1-prop-4-cor-3 .statement tag=07LC}

— *E をベクトル空間、(F_i)_{i \in I} を E から F_i への局所凸空間と f_i 線形写像の族とします (i \in I の場合)。 E に、すべての f_i が連続 (II、p. 26) である最も粗い位相 (局所的に凸) が割り当てられているとします。次に、E の部分集合 A が有界であるためには、I のすべての i \ に対して f_i(A) が F_i で有界であることが必要かつ十分です。

実際、A が有界であれば、f_i(A) (cor. 1) も有界です。逆に、f_i(A) が有界で、p が E 上の連続半ノルムである場合、I の有限部分集合 J と族 $(q_j)_{j \in J}$ が存在します。ここで、$q_j$ は $F_j$ 上の連続半ノルムであり、その結果、$p \leq \sup_{j \in J} (q_j \circ f_j)$ は $p$ で有界されます。 $A$。

#### 系 4 {#evt-iii-s1-prop-4-cor-4 .statement tag=07LD}

*$E_i$ ($1 \leq i \leq n$) と $F$ を局所凸空間とし、$f$ を $\prod_{i=1}^n E_i$ から $F$ までの連続多重線形写像とします。 $B_i$ が $1 \leq i \leq n$ の $E_i$ の有界部分集合である場合、$f(\prod_{i=1}^n B_i)$ は $F$ に有界されます。*

#### 系 5 {#evt-iii-s1-prop-4-cor-5 .statement tag=07LE}

*$E$ と $F$ を 2 つの局所凸空間とし、$u : E \to F$ を連続多項式写像とします。 $A$ が $E$ の有界部分集合である場合、$u(A)$ は有界です。*

### 4. 特定の帰納法極限における有界部分集合

#### 命題 5 {#evt-iii-s1-prop-5 .statement tag=07LF}

*$(E_i)_{i \in I}$ を局所凸ハウスドルフ族空間とし、$E$ をこの族の位相幾何学直和 (II, p. 29) とします。 $E$ の部分集合 $B$ が制限される位数では、$\operatorname{pr}_i(B)$ が $i \in J$ と $\operatorname{pr}_i(B) \subset \{0\}$ ですべての$E_i$ に制限されるように、$I$ の有限部分集合 $J$ が存在することが必要かつ十分です。 $i \notin J$。

$J$を$I$の有限部分集合とします。 $\prod_{j \in J} E_j$ の $E$ 誘導する積位相の位相 (II、p. 30、提案 7 および p. 31、提案 8) から、III、p. 4、コル。 2 条件で十分です。

逆に、$B$ を $E$ の有界な部分集合とします。 次に、$\operatorname{pr}_i(B)$ はすべての $i$ (III、p. 4、cor. 1) に対して有界です。 従って、すべての $i \notin J$ に対して $\operatorname{pr}_i(B) \subset \{0\}$ となるような $I$ の有限部分集合 $J$ が存在することを証明すれば十分です。 If not, then there exists an infinite sequence $(i_n)$ of distinct elements of $I$ and an infinite sequence $(x_n)$ of elements of $B$ such that $\operatorname{pr}_{i_n}(x_n) \neq 0$. $E_{i_n}$ はハウスドルフであるため、$E_{i_n}$ 上に $p_n(\operatorname{pr}_{i_n}(x_n)) \geq n$ のような連続半ノルム $p_n$ が存在します。 従って、$p = \sum_{n \geq 1} p_n \circ \operatorname{pr}_{i_n}$ は $E$ 上の連続半ノルムであり、$p$ は $B$ に制限されておらず、これは矛盾です。*

#### 命題 6 {#evt-iii-s1-prop-6 .statement tag=07LG}

*$E$ を、$E$ (II、p. 33) の閉ベクトル部分空間の増加する数列 $(E_n)$ の厳密な帰納極限である局所凸空間とします。 $E$ の部分集合 $B$ は、部分空間 $E_n$ のいずれかに含まれる場合にのみ制限され、この部分空間に制限されます。

$E$ の$E_n$ によって誘導される位相は、正確に $E_n$ の所与の位相であるため、条件で十分です (II、p. 32、提案 9)。 条件が必要であることを確認するには、$E$ の点の数列 $(x_m)$ が部分空間 $E_n$ のいずれにも含まれていない場合、できないは 0 になる傾向があることを証明するだけで十分です (III、p. 4、提案 3)。 数列 $(x_m)$ の部分列を抽出すると、添字 $k$ ごとに $x_k \notin E_{n_k}$ と $x_k \in E_{n_{k+1}}$ が存在するように、整数の真に増加する数列 $(n_k)$ が存在すると仮定できます。 次に、$E_{n_k}$、$V_{k+1} \cap E_{n_k} = V_k$ で $V_k$ が 0 の近傍となるような凸集合の (II、p. 33、補題 2) 増加する数列 $(V_k)$ が存在します。 添字 $k$ ごとに $x_k \notin V_{k+1}$。 $V_k$ の和集合 $V$ は、$E$ の 0 の近傍となり、すべての $k$ に対して $x_k \notin V$ が得られます。 これは、数列 $(x_k)$ が 0 になる傾向がないことを証明しています。*

プロップの結論。 6 は、E の閉部分空間の非計数不可能有向集合の帰納極限である空間 E には必ずしも真ではありません (cf. III, p. 38、演習 7)。

#### 命題 7 {#evt-iii-s1-prop-7 .statement tag=07LH}

— $(E_n)_{n \geq 0}$ をハウスドルフの局所凸型空間の数列とし、すべての $n$ について、$u_n : E_n \to E_{n+1}$ をコンパクトな単射法線形写像とする（すなわち、$E_n$ に 0 の近傍が存在するようにする） $u_n$ の下の像は比較的コンパクトです。これは、$u_n$ が連続であることを意味します)。 $E$ を系 $(E_n, u_n)$ (II、p. 29) の帰納極限とし、$v_n$ を $E_n$ から $E$ までの標準写像とします。次に、局所的に凸の空間$E$がハウスドルフです。さらに、$E$ の各部分集合 $A$ について、次の条件は同等です。
(i) $A$ は有界です。
(ii) $E_n$ の有界部分集合の $v_n$ の下に $A$ が像となるような整数 $n$ が存在します。
(iii) $A$ は比較的コンパクトです。
私たちは $E$ のベクトル部分空間で同一視する $E_n$ になります (誘導された位相よりも位相より細かいが与えられています)。

#### 補題 1 {#evt-iii-s1-lem-1 .statement tag=07LI}

プロップの仮定の下。 7、$E$の位相は、すべての写像$v_n : E_n \to E$が連続する最高級の位相です。

$U$ が $E$ の部分集合で、$U \cap E_n$ が $n$ ごとに $E_n$ でオープンになり、$U$ が $E$ でオープンになることを証明する必要があります。他の語では、証明しなければならないでは、すべての $x \in U$ に対して、$x + V \subset U$ および$V \cap E_n$ が十分に大きいすべての $E_n$ で 0 の近傍となる *凸平衡* 集合 $V$ が存在します。 $n$ (II、p. 27、提案 5)。すべての $n$ について、$E_{n+1}$ の $W_n$ の閉包 $H_n$ がコンパクトになるように、$E_n$ の 0 の凸バランスの近傍を$W_n$ とします。 $x \in U$ と $n_0$ を $x \in E_{n_0}$ となるように整数とします。 $x + \sum_{n_0 \leq i \leq n} \varepsilon_i H_i$ が $n \geq n_0$ の $U$ に含まれるように、スカラー $> 0$ の帰納法、数列 $(\varepsilon_n)_{n \geq 0}$ によって構成するを計算します。 $i < n$ の $\varepsilon_i$ が構築されたとします。 $n = n_0$、集合 $V_{n-1} = \{0\}$の場合。そうでない場合は、集合
$$
V_{n-1} = \sum_{n_0 \leq i \leq n-1} \varepsilon_i H_i.
$$
すると、$V_{n-1}$は$E_n$でコンパクトになり、*なおさら*は$E_{n+1}$でコンパクトになります。 $U \cap E_{n+1}$ は $E_{n+1}$ で開いているため、$x + V_n = x + V_{n-1} + \varepsilon_n H_n$ が $U$ に含まれるようなスカラー $\varepsilon_n > 0$ が存在します (GT, II, § 4, No. 3, cor.)。 $V = \bigcup_{n \geq n_0} V_n$ にしましょう。次に、$V$ は凸でバランスが取れています。 $n \geq n_0$ の場合、$V \cap E_n \supset \varepsilon_n H_n \cap E_n \supset \varepsilon_n W_n$ があるため、$V \cap E_n$ は $E_n$ の 0 の近傍になります。これで補題の証明が完了しました。

集合 $U = E - \{0\}$ は、集合 $U \cap E_n = E_n - \{0\}$ が $n$ ごとに $E_n$ で開いているため、$U$ が $E$ で開いており、$E$ がハウスドルフ (GT、III, § 1, No. 3、prop. 2)。 性質 (ii) が (iii) を意味し、(iii) が (i) を意味することは明らかです。最後に、(i) が (ii) を意味することを示します。このためには、$E$ の部分集合 $A$ が集合 $\sum_{0 \leq i \leq n} H_i$ のいずれにも吸収されない場合、$A$ は有界ではないことを示すだけで十分です。しかし、その後、$A$の点のうち数列$(x_n)_{n \geq 1}$が存在し、$n$ごとに$x_n \notin n^2 \sum_{0 \leq i \leq n} H_i$が存在します。

次に、$x_n / n$ の集合は、$E_m$ を持つ共通部分が整数 $m$ ごとに離散するため、補題 1 によって閉じられます。 $x_n / n$ の集合の補数は 0 のオープン近傍であり、数列 $(x_n)$ を吸収しないため、$A$ は有界ではありません。

#### 注意 1 {#evt-iii-s1-n4-rem-1 .statement tag=07LJ}

上記の記法で、$F_n$を$H_n$によって生成されるベクトル空間とし、ノルムは$H_n$のゲージに等しいとします。 (III, p. 8, cor.) $F_n$ がバナッハ空間であることが分かります。 $F_n$ から $E_{n+1}$ への単射はコンパクトなので、*なおさら* も $F_n$ から $F_{n+1}$ への単射 $w_n$ です。さらに、$E$ は、バナッハ空間* の帰納的系* $(F_n, w_n)$ * の * 帰納的極限です。なぜなら、$E$ の 0 の凸平衡近傍 $V$ は、$V \cap E_n$ がすべての $n \geq 1$ に対して $H_{n-1}$ を吸収するようなものであり、逆に、$E$ の凸平衡集合 $W$ が次のようなものである場合、 $W \cap E_n$ は $H_{n-1}$ を吸収し、次に $W \cap E_{n-1}$ 含む集合はすべての $n \geq 1$ について $W_{n-1}$ と相似となり、したがって $W$ は $E$ の 0 の近傍になります。

#### 注意 2 {#evt-iii-s1-n4-rem-2 .statement tag=07LK}

$F$ を局所凸空間、$k$ 整数 $\geq 0$、および $f : E^k \to F$ を多重線形マッピングとします。 $f$が連続であるためには、$f$から$E_n^k$の制限が$n$ごとに連続していることが必要十分です。 $E^k$ が線形写像 $v_n \times \cdots \times v_n : E_n \times \cdots \times E_n \to E \times \cdots \times E$ (II, p. 28, cor. 2 および p. 30, prop. 7) の最終局所凸位相を持ち、$u_n \times \cdots \times u_n$ がコンパクト単射であることをすぐに検証します。 $(E_n)^k$から$(E_{n+1})^k$への線形写像。 補題 1 を適用するだけで十分です。

### 5. 空間 $E_A$ (有界)

$E$ を局所凸空間とし、$A$ を $E$ の凸平衡部分集合とします。 $E_A$ は、$A$ によって生成されたベクトル空間を示し、$p_A$ は準ノルムとして $A$ のゲージ (II、p. 26、*例 3*) であることを思い出します。 $A$ が有界である場合に限り、$E_A$ から $E$ への標準単射が連続であることを直ちに検証します。 加法で、$E$ がハウスドルフである場合、有界の集合 $A$ は含むの直線 (III, p. 2, *注意 4*) ではないため、$p_A$ は次のようになります。 ノルム (II、*上記引用*)。

$X$ のすべてのコーシー 数列が収束する場合、一様空間 $X$ は *半完全* であると言えます。完全なユニフォーム空間は半完成です。しかし、逆は常に真であるとは限りません (GT、II, § 4、演習​​ 4)。ただし、計量可能な半完成品空間は完成しています (GT、IX, § 2, No. 6、提案 9)。

#### 命題 8 {#evt-iii-s1-prop-8 .statement tag=07LL}

*$E$ を局所的に凸なハウスドルフ空間とし、$A$ を $E$ の閉じた平衡型有界凸型部分集合とします。 $(x_n)$ を $E_A$ のコーシー 数列とします。次に、この数列は、$E$ に収束する場合に限り、$E_A$ に収束します。*

$E_A$から$E$までの標準単射は連続です。したがって、$(x_n)$ が $E_A$ に収束すると、$E$ に収束します。逆に、$(x_n)$が$E$で$y$に収束するとします。 $m \geq n_k$ と $n \geq n_k$ であれば $p_A(x_m - x_n) \leq 2^{-k-1}$ となる整数 $(n_k)$ の増加する数列が存在します。したがって、数列 $(x_{n_k} + 2^{-k}A)$ は減少するです。 $A$ が $E$ で閉じているため、$y \in \bigcap_k (x_{n_k} + 2^{-k}A)$ が得られます。これは、$(x_{n_k})$、したがって $(x_n)$ が $E_A$ で $y$ に収束することを証明します。

#### 系 {#evt-iii-s1-n5-cor-1 .statement tag=07LM}

— *A が半完全 (特に完全) の場合、E_A はバナッハ空間です。*
    実際、E_A のコーシー 数列は、E の位相のコーシー 数列でもあり、A と相似の集合に含まれるため、E に収束します。

### 6. 完全有界集合および準完全空間

#### 定義 6 {#evt-iii-s1-def-6 .statement tag=07LN}

— *局所的に凸な空間 E は、E のすべての閉じた有界部分集合が完全である場合、準完全であると言われます (E のそれによって誘導される一様構造の場合)。
    完全な局所凸型空間は準完全ですが、 逆は常に真であるとは限りません。 *たとえば、E が無限次元のヒルベルト空間、またはより一般的には無限次元の再帰的バナハ空間である場合、その弱体化された位相を持つ E は準完全ですが、完全ではありません (II, p. 51, 提案 9)。
    すべてのコーシー 数列が閉じた有界の部分集合 (III、p. 3、系および提案 1) に含まれるため、準完全空間は半完全です。特に、局所的に凸の計化可能で準完全な空間が完全です。
    ハウスドルフ準完全空間では、プレコンパクト部分集合の閉包と閉じた凸平衡エンベロープはコンパクトです。実際、それらは事前に圧縮されており (II、p. 25、提案 3)、完全に閉じて有界になっています (III、p. 3、提案 2)。

#### 命題 9 {#evt-iii-s1-prop-9 .statement tag=07LO}

— (i) 準完全局所凸空間の *閉ベクトル部分空間は準完全です。*
    (ii) 準完全局所凸空間の*積は準完全である*。
    (iii) *準完全局所凸型空間のトポロジカル直和は準完全です。*
    (iv) *閉準完全部分空間の数列の厳密帰納法極限である *局所凸空間は準完全です。*
    主張 (i) *注意 2* (III、p. 2) から、(ii) III、p. 4、cor から続きます。 2、(iii) 提案から。 5 (III、p. 5) および (iv) プロップから。 6 (III、p. 5)。

    閉じたベクトル空間による準完全局所凸空間の商空間は、必ずしも準完全ではないことがわかります (IV、p. 63、練習問題 10)。

#### 命題 10 {#evt-iii-s1-prop-10 .statement tag=07LP}

— *E を局所凸空間, M ベクトル部分空間とし、E のすべての点が M の有界部分集合の閉包内にあるようにします。次に、M からのすべての連続線形写像 f をハウスドルフ準完全局所凸にします。 空間 F は一意に拡大するから E から F への連続線形写像になります*。
仮定は M が E 内で密であることを意味し、したがって f 拡大するは E から F の完成 $\hat{F}$ まで連続する線形写像 $\hat{f}$ に一意です (GT, III, § 3, No. 4, 系)。しかし、すべての $x \in F$ は、M の有界な部分集合 B の閉包の中にあります。したがって、$\hat{f}(x)$ は $\hat{F}$ の $f(B)$ の閉包内にあります。しかし、$f(B)$ は F で有界されているため、F での閉包が完了し、一致するは $\hat{F}$ での閉包で完了します。これは$\hat{f}(x) \in F$であることを証明します。

### 7. 例

a) X をトポロジカル空間とします。 X 上の数値 (有限) 写像の $\mathscr{R}(X)$、ベクトル空間に、コンパクト収束 (GT、X, § 1, No. 3) の位相を割り当てます。これは、制限の中で最も粗い位相です。 写像 $\mathscr{R}(X) \to \mathscr{R}(H)$ は連続です (H は X のコンパクトな部分集合の族を通過し、$\mathscr{R}(H)$ には一様収束の位相が割り当てられます)。コル。 III、p. 4 の 3 は、X の部分集合 H から制限の集合が写像の H に至る場合にのみ、$\mathscr{R}(X)$ の部分集合 A が有界であることを示しています。 所属から A までは一様有界です。

*b) (無限微分可能な写像の空間。) $n \geqslant 1$を整数とする。 $\mathbf{R}^n$ の開いた集合 U ごとに、$\mathscr{C}^\infty(U)$ が U で無限微分可能な写像のベクトル空間を表すものとします (VAR、R、2.3)。 f を $\mathscr{C}^\infty(U)$ にします。 $\mathbf{N}^n$ のすべてのマルチインデックス $\alpha = (\alpha_1, ..., \alpha_n)$ について、$\partial^\alpha f$ は偏導関数 $\partial^{|\alpha|} f / \partial x_1^{\alpha_1} ... \partial x_n^{\alpha_n}$ を表します。これは U (VAR、R、2.3 および 2.4) の連続写像です。すべての整数 $m \geqslant 0$ および U のすべてのコンパクト部分集合 H、集合

$$
p_{m,H}(f) = \sup_{\substack{|\alpha| \leqslant m \\ x \in H}} |\partial^\alpha f(x)| .
$$

すると、$p_{m,H}$ は $\mathscr{C}^\infty(U)$ の準ノルムとなります。

$\mathscr{C}^\infty(U)$ に半ノルム $p_{m,H}$ によって定義された位相を割り当てます。 これは、$\mathscr{C}^\infty(U)$ から $\mathscr{R}(U)$ までの写像 $f \to \partial^\alpha f$ が連続するトポロジの中で最も粗く、$\mathscr{R}(U)$ にはコンパクト コンバージェンスの位相が割り当てられます。 内部が U を覆うコンパクトな U の増加する数列部分集合 $(H_n)_{n \geqslant 0}$ が存在します。 $\mathscr{C}^\infty(U)$ の準ノルム $p_{m,H_n}$ 定義する位相の族であり、これは局所的に凸な metrizable 空間になります。 空間 $\mathscr{C}^\infty(U)$ が完了しました。他の語では、それは Fréchet 空間 (II、p. 24) です。実際、$(f_k)$ は $\mathscr{C}^\infty(U)$ の Cauchy 数列とします。すべての $\alpha \in \mathbf{N}^n$、数列 $(\partial^\alpha f_k)$ は、完全な空間 $\mathscr{R}(U)$ (TG、X, § 1, No. 5、th. 1) で連続する写像 $g_\alpha$ に収束します。 $|\alpha|$ の帰納法までに、 th から推測します。 FVR の 1、II、p. 2、$\alpha \in \mathbf{N}^n$ ごとに $g_\alpha = \partial^\alpha g_0$。 他の語では、数列$(f_k)$は、$\mathscr{C}^\infty(U)$では$g_0$に収束します。

A を $\mathscr{C}^\infty(U)$ の部分集合とします。 位数では、A が有界であるためには、数 $\sup_{f \in A} p_{m,H}(f)$ がすべての整数 $m \geqslant 0$ と U のすべてのコンパクト部分集合 H に対して有限であることが必要かつ十分です。この条件は、$f \in A$ の写像 $\partial^\alpha f|H$ のすべての $\alpha \in \mathbf{N}^n$、集合が、すべてのコンパクト $H \subset U$ で均一に制限されることを意味します。

$H \subset U$ をコンパクトにします。 H にサポートがある写像のうち、$\mathscr{C}^\infty(U)$ からなるの $\mathscr{C}_H^\infty(U)$ 部分空間で表します。 U のコンパクトサポートを持つ無限微分可能写像の空間 $\mathscr{C}_c^\infty(U)$ は、 の有向増加する和集合です。 部分空間 $\mathscr{C}_H^\infty(U)$ ここで、H は U のコンパクトな部分集合の族を貫いています。各空間 $\mathscr{C}_H^\infty(U)$ には、$\mathscr{C}^\infty(U)$ の誘導によって誘導された位相が割り当てられ、対応する誘導極限を伴う $\mathscr{C}_c^\infty(U)$ が割り当てられます。 位相。 集合 $H_n$ がその内部形が U のカバーである場合、空間 $\mathscr{C}_c^\infty(U)$ はフレシェ空間 $\mathscr{C}_{H_n}^\infty(U)$ の厳密帰納法極限です。したがって、これは完全であり (II、p. 32、提案 9)、$\mathscr{C}_c^\infty(U)$ のすべての境界付き部分集合は、部分空間 $\mathscr{C}_{H_n}^\infty(U)$ (III、p. 5、提案 6) の 1 つに含まれます。 \*

c) (ジュヴレの空間。) I を $\mathbf{R}$ のコンパクト区間とします。すべての整数 $n \geqslant 0$ について、$D^n f$ は、I で定義された数値写像 $f$ の $n$ 次導関数を表します (この導関数が存在する場合は常に)。 $s \geqslant 1$ と $M \geqslant 0$ を 2 つの実数とします。 $\mathscr{G}_{s,M}(I)$ は、I (FVR、I、p. 28) 上で無限微分可能な写像 $f$ のうち、数列 $(|D^n f|/M^n(n!)^s)_{n \geqslant 0}$ が空間で有界されるベクトル空間を表すものとします。 I 上のすべての連続写像のうち $\mathscr{C}(I)$ (一様収束の位相を含む)。 空間 $\mathscr{G}_{s,M}(I)$ は、ノルムを持つバナッハ空間です

$$
\|f\|_{s,M} = \sup_{n \geqslant 0, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

$M \leqslant M'$ には $\mathscr{G}_{s,M}(I) \subset \mathscr{G}_{s,M'}(I)$ があり、

$$
\|f\|_{s,M'} \leqslant \|f\|_{s,M}
$$

$f \in \mathscr{G}_{s,M}(I)$ごとに。 $\mathscr{G}_s(I)$ が空間 $\mathscr{G}_{s,M}(I)$ の和集合を表し、それに $\mathscr{G}_{s,M}(I)$ のトポロジーの帰納的極限位相を与えるものとします。

$M < M'$ とし、B を $\mathscr{G}_{s,M}(I)$ の単位元ボール (クローズ) とします。 B がバナハ空間 $\mathscr{G}_{s,M'}(I)$ のコンパクト部分集合であることを証明します。 B が $\mathscr{G}_{s,M'}(I)$ で閉じていることは明らかなので、B が $\mathscr{G}_{s,M'}(I)$ でプリコンパクトであることを証明すれば十分です。 $\varepsilon > 0$ とし、N を $(M/M')^N \leqslant \varepsilon/2$ となるように正の整数とします。 Let $k$ be a positive integer; the set of all functions $D^{k+1} f$, as $f$ ranges over B, is bounded in $\mathscr{C}(I)$, hence the set of all functions $D^k f$, as $f$ ranges over B, is relatively compact in $\mathscr{C}(I)$: this follows from the theorem of finite increments (FVR, I, p. 23, cor. 1) and from Ascoli’s theorem (GT, X, § 2, No. 5). 私たちは $\mathscr{G}_{s,M}(I)$ で定義するノルム

$$
q(f) = \sup_{0 \leqslant n \leqslant N, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

上記の引数は、B がノルム $q$ に関連付けられた位相に対してプリコンパクトであることを示しています。他の語では、B の有限部分集合 C が存在し、$f \in B$ ごとに $q(f - g) \leqslant \varepsilon$ となる $g \in C$ が存在します。最後に、$n > N$ ごとに、

$$
|D^n f(x) - D^n g(x)|/M^n(n!)^s \leqslant 2(M/M')^n \leqslant \varepsilon ,
$$

そこから $\|f - g\| \leqslant \varepsilon$ が得られます。これは、B が $\mathscr{G}_{s,M'}(I)$ でプリコンパクトであることを証明します。

空間 $\mathscr{G}_s(I)$ は、$k$ が $\mathbf{N}$ を超える範囲であるため、空間 $\mathscr{G}_{s,k}(I)$ の帰納的極限です。プロップによって。 7 (III、p. 6) $\mathscr{G}_s(I)$ のすべての境界付き部分集合は、空間 $\mathscr{G}_{s,k}(I)$ のいずれかに含まれており、この空間では比較的コンパクトです。

\* d) (正則写像の空間。) $n \geqslant 1$ を整数とします。 $\mathbf{C}^n$ のすべての開いた部分集合 U に対して、$\mathscr{H}(U)$ は U の正則な写像の空間を表し、U のコンパクト収束の位相が割り当てられます。 $\mathbf{C}^n$ のすべてのコンパクト部分集合 L について、 $\mathscr{H}(L)$は、Lの近傍における正則写像の細菌の空間を表します。この空間に、標準写像 $\pi_U : \mathscr{H}(U) \to \mathscr{H}(L)$ が連続する最も細かい局所凸型位相を与えます。ここで、U の範囲は、L のオープン近傍の集合に及びます。

すべての整数 $m \geq 1$ について、$U_m$ を、L から $< 1/m$ の距離にある $\mathbf{C}^n$ の点の集合とします。 $\mathscr{H}(U_m)$ から $\mathscr{H}(L)$ への標準写像 $\pi_{U_m}$ は *単射的* であり、 $\mathscr{H}(U_m)$ から $\mathscr{H}(U_p)$ への制限写像は $p \geq m$ に対して *コンパクト* であることがわかります。 次に、プロップを適用します。 7 (III、p. 6)。 A を $\mathscr{H}(L)$ の有界部分集合とします。その場合、A が L の近傍の写像 、所属から $\mathscr{H}(U_m)$ の有界の集合 B までの細菌から構成されるような整数 $m \geq 1$ が存在します。 さらに、$\mathscr{H}(L)$ からトポロジカル空間 T への写像 $\phi$ は、$\mathscr{H}(U)$ から T への写像 $\phi \circ \pi_U$ が、L の開いた近傍 U ごとに連続である場合にのみ連続です。 \*

### 練習問題 {#evt-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
