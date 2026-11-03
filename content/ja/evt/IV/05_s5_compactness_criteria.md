---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 5
section_title: Compactness criteria
lang: ja
source: evt-i-v
book_pages: TVS IV.32-TVS IV.38, TVS IV.67-TVS IV.71
pdf_pages: 0214-0220, 0249-0253
extraction: ocr
subsections:
    - "no": 1
      title: General remarks
      page: 32
      pdf_page: 214
    - "no": 2
      title: Simple compactness of sets of continuous functions
      page: 33
      pdf_page: 215
    - "no": 3
      title: The Eberlein and Šmulian theorems
      page: 35
      pdf_page: 217
    - "no": 4
      title: The case of spaces of bounded continuous functions*
      page: 36
      pdf_page: 218
    - "no": 5
      title: Convex envelope of a weakly compact set
      page: 37
      pdf_page: 219
statements: 8
exercises: 18
content_sha256: e6b0a172d3b73d1a09b8a0ebbf8595937df0cb9f366f28cadfacf36a53ad01a3
translated_from: content/en/evt/IV/05_s5_compactness_criteria.md
translation_method: google
source_content_sha256: 109a4d05718fd73c2e0104fdb772994f028706b89a9a4001b0f091a0d03c8b4b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 35f2c981694686a63c3dc7b838af692c658b957957037f71f96ad7f02a2efe6b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。コンパクトさの基準

### 1. 一般注意

A をトポロジカル空間 E の部分集合とします。A の点の数列 $(x_n)_{n \in \mathbf{N}}$ が E の点 x を極限点とするためには、次の条件が満たされることが必要かつ十分です (GT, I, § 7, No. 3) :

(A) x のすべての整数 $m \geq 0$ とすべての近傍 U に対して、$x_n \in U$ となるような整数 $n \geq m$ が存在します。

A sequence of the form $(y_k)_{k \in \mathbf{N}}$ with $y_k = x_{n_k}$ for a strictly increasing sequence $(n_k)_{k \in \mathbf{N}}$ of positive integers is called an extracted sequence of the sequence $(x_n)_{n \in \mathbf{N}}$. x に収束する数列 $(x_n)_{n \in \mathbf{N}}$ の抽出された数列が存在する場合、x は $(x_n)$ の極限点です。逆に、x が近傍の可算基本系を持ち、x が数列 $(x_n)$ の極限点である場合、x に収束する $(x_n)$ の抽出された数列が存在します。

GT、IX, § 2, No. 9、系を考慮して、E が計量可能である場合、次の条件は同等であることが結論するわかります。
a) 集合 A は E の中で比較的コンパクトです。
b) A の点のすべての無限数列は E に極限点を持ちます。
c) A の点のすべての無限数列から、E の点に収束する数列を抽出できます。

この切断では、この基準を特定の非計量化不可能なトポロジカルベクトル空間に拡大する適用します。次の命題により、数のケースにおけるコンパクト集合から弱コンパクト集合の検討を簡約する行うことができます。

#### 命題 1 {#evt-iv-s5-prop-1 .statement tag=07VR}

— E を局所的に凸なハウスドルフ空間とし、A を E の部分集合とします。$E_\sigma$ は、位相を弱めた空間 E を表します。
a) A の点のすべての無限数列が E に極限点を持っている場合、A は E でプリコンパクトです。
b) 位数において、A が E において相対的にコンパクトであることは、E においてプレコンパクトであり、$E_\sigma$ において比較的コンパクトであることが必要かつ十分である。

a) を不合理な還元によって証明します。 A がプリコンパクトでない場合は、th によって計算されます。 GT の 3、II, § 3, No. 7 の場合、E には 0 の対称凸型近傍 V が存在し、できないは V の平行移動の有限数でカバーされることになります。

他の語では、$x_0, x_1, ..., x_{n-1}$がAの点であれば、$A \notin \bigcup_{0 \leq i < n} (x_i + V)$となり、$0 \leq i < n$に対して$x_n - x_i \notin V$となるようなAの点$x_n$が存在します。次に、整数 $n$ の帰納法までに、$n > m$ になるたびに $x_n - x_m \notin V$ となるような A の点の構成するを無限に数列 $(x_n)_{n \in \mathbf{N}}$ にすることができます。 V は対称なので、$m \neq n$ には $x_m - x_n \notin V$ もあり、集合 $x_n + \frac{1}{2} V$ は互いに素です。 E のすべての点 $x$ に対して、$x_n \in x + \frac{1}{2} V$ となる整数 $n \geq 0$ が最大 1 つ存在するため、数列 $(x_n)_{n \in \mathbf{N}}$ には極限点が存在しません。これは *a)* を証明します。

ここで、A が E で事前コンパクトであり、$E_\sigma$ のコンパクト部分集合 B に含まれているとします。次に、B は $E_\sigma$ で完了するため、E (IV、p. 5、*注意 2*) でも完了します。 $\overline{A} \subset B$ があるため、A は E 内で比較的コンパクトです。逆は明らかであり、*b)* が続きます。

### 2. 連続写像の集合のシンプルなコンパクトさ

この切断では、XはXの連続写像の*コンパクト*空間と$\mathscr{C}_s(X)$空間を表し、体K（$\mathbf{R}$または$\mathbf{C}$に等しい）の値を含みます。 空間 $\mathscr{C}_s(X)$ には、X への単純収束の位相が割り当てられます。

#### 命題 2 {#evt-iv-s5-prop-2 .statement tag=07VS}

*D を X の密な部分集合と、A 空間 $\mathscr{C}_s(X)$ の密な部分集合とします。 次の条件は同等です:*
(i) *$\mathscr{C}_s(X)$ では比較的コンパクトです。*
(ii) *A のすべての要素の無限シーケンスから、$\mathscr{C}_s(X)$ に収束するシーケンスを抽出できます。
(iii) *A の要素の無限シーケンスにはすべて、$\mathscr{C}_s(X)$ に極限点があります。*
(iv) *$(f_n)_{n \in \mathbf{N}}$ を A に属する関数の列、$(x_m)_{m \in \mathbf{N}}$ を D の点の列とする。 極限* が反復された場合

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

* が存在する場合、それらは等しいです。 加法では、すべての $x \in X$ に対して $\sup_{f \in A} |f(x)| < + \infty$ があります。*

(i) $\Rightarrow$ (ii) : $\overline{A}$ を $\mathscr{C}_s(X)$ の A の閉包とします。 A がコンパクトであると仮定し、写像 $f_n \in A$ ($n \in \mathbf{N}$ の場合) の数列を考えます。 $\phi$ を、X から計量可能空間 $K^\mathbf{N}$ への連続写像 $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ とします。 $\phi$ の下の X の像 $X'$ は、X がコンパクトなので、コンパクトなメトリズ可能空間です。 E を、X の点 $x, y$ のすべてのペアに対して関係 $\phi(x) = \phi(y)$ が $f(x) = f(y)$ を意味するように、X 上の連続関数 $f$ から構成される$\mathscr{C}_s(X)$ の閉部分空間とする。 コルによって。 GTの2、I, § 9, No. 4、プロップ。 GT の 3、I, § 5, No. 2、写像 $f' \mapsto f' \circ \phi$ は、$\mathscr{C}_s(X')$ から E への$\phi^*$ の同型写像です。 従って、集合 $A' = (\phi^*)^{-1}(\overline{A})$ は $\mathscr{C}_s(X')$ でコンパクトであり、$A'$ には $\phi^*(f'_n) = f'_n \circ \phi$ が $f_n$ に等しい元 $f'_n$ が存在することは明らかです。

$X'$ はコンパクト計素可能空間であるため、$X'$ には可算密な部分集合 D' が存在します (GT、IX, § 2, No. 8、提案 12 および § 2, No. 9、提案 16)。 $\mathscr{T}_1$ (それぞれ $\mathscr{T}_2$) を、D' (それぞれ $X'$) に対する単純な収束の位相によって引き起こされる $A'$ 上の位相とします。 この場合、$\mathscr{T}_1$ は計量化可能で、$\mathscr{T}_2$ はコンパクトで、$\mathscr{T}_1$ よりもより細かいなので、$\mathscr{T}_1$ と $\mathscr{T}_2$ 一致するになります。他の語、$A'$は、$\mathscr{C}_s(X')$のコンパクトな *metrizable* 部分空間です。 従って、$(f'_n)$から抽出され、$\mathscr{C}_s(X')$の元$f'$に収束する数列$(f'_{n_k})$が存在します。 従って、数列 $(f_{n_k})$ は $\mathscr{C}_s(X)$ で $f = f' \circ \phi$ に収束します。

(ii) $\Rightarrow$ (iii) : これは明らかです。

(iii) $\Rightarrow$ (iv) : A の元のすべての無限数列が $\mathscr{C}_s(X)$ に極限点を持つと仮定します。 $x \in X$ にしましょう。 写像 $\phi_x : f \mapsto f(x)$ A から K までは連続です。従って、$\phi_x(A)$ のすべての無限の数列には極限点が含まれます。 体 K ($\mathbf{R}$ または $\mathbf{C}$ に等しい) は計量可能であるため、集合 $\phi_x(A)$ は K において比較的コンパクトであり、したがって有界です。その他語には$\sup_{f \in A} |f(x)| < \infty$がございます。

$f_n, x_m, \gamma$ と $\delta$ を (iv) のようにします。 $f$ を $\mathscr{C}_s(X)$ の数列 $(f_n)$ の極限点とし、$x$ をコンパクト空間の数列 $(x_m)$ の極限点とします。 X。 $m$ ごとに、$\mathscr{C}_s(X)$ から K までの写像 $h \mapsto h(x_m)$ は連続です。仮説を考慮すると、$f(x_m) = \lim_{n \to \infty} f_n(x_m)$、したがって $\gamma = \lim_{m \to \infty} f(x_m)$ になります。 $f : X \to K$ は連続であり、$x$ は数列 $(x_m)$ の極限点であるため、$\gamma = f(x)$ が得られます。同様の方法で、等式 $\delta = f(x)$、よって $\gamma = \delta$ を証明します。

(iv) $\Rightarrow$ (i) : 数 $f(x)$ の集合は、$f$ の範囲が A であるため、すべての $x \in X$ について K で制限されるとします。これは、積空間 $K^X$ の A の閉包 $\overline{A}$ がコンパクト (GT, I, § 9, No. 5) であると仮定するのと同じです。 A が *$\mathscr{C}_s(X)$ において比較的コンパクトではないと仮定します。これは、$u$が$a$で連続しないような写像$u \in \overline{A}$と点$a \in X$が存在することを意味します。したがって、$a$ のすべての近傍 U に、$|u(x) - u(a)| \geq \varepsilon$ を伴う点 $x$ が存在するように、実数 $\varepsilon > 0$ が存在します。

D の点の帰納法数列 $(x_n)_{n \in \mathbf{N}}$ と、A の元の数列 $(f_n)_{n \in \mathbf{N}}$、次の満たす関係によって構成するを実行します。

(1)$_m$ $$ |u(x_m) - u(a)| \geq \varepsilon \quad \text{for} \quad m \geq 1 ; $$

(2)$_m$ $$ |u(x_i) - f_m(x_i)| \leq \frac{1}{m + 1} \quad \text{for} \quad 0 \leq i \leq m - 1 ; $$

(3)$_{m,i}$ $$ |f_m(x_i) - f_m(a)| \leq \frac{1}{i + 1} \quad \text{for} \quad 0 \leq m \leq i . $$

A で任意の $f_0$ を使用して $x_0 = a$ を取得します (集合 A は空ではありません。そうでない場合は、$\mathscr{C}_s(X)$ で比較的コンパクトになります)。 $n \geq 1$ と $x_0, x_1, ..., x_{n-1}, f_0, f_1, ..., f_{n-1}$ 満たす関係を (1)$_m$、(2)$_m$ を $1 \leq m < n$ に、(3)$_{m,i}$ を $0 \leq m \leq i < n$ とします。 $u$ 属するから $\overline{A}$ までなので、$f_n \in A$ 満たす (2)$_n$ が存在します。 $V_n$ をすべての $x \in X$ の集合とし、$0 \leq m \leq n$ に対して $|f_m(x) - f_m(a)| \leq \frac{1}{n + 1}$ を計算します。 $f_n$ は連続なので、$V_n$ は $a$ の近傍です。 $D \cap V_n$ の選ぶ点 $x_n$ は、$|u(x_n) - u(a)| \geq \varepsilon$ となるため、(1)$_n$ と (3)$_{m,n}$ が満たされます。従って、構成は継続可能です。

$u(X)$ は K の圧縮部分集合なので、$(x_m)$ から抽出された数列 $(y_k)$ が存在し、極限 $\gamma = \lim_{k \to \infty} u(y_k)$ が存在します。 (2)$_m$ により、すべての $i \in \mathbf{N}$ に対して $u(x_i) = \lim_{n \to \infty} f_n(x_i)$ が得られます。

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k) .
$$

一方、(3)$_{m,i}$ により $f_n(a) = \lim_{i \to \infty} f_n(x_i)$ が得られるため、$f_n(a) = \lim_{k \to \infty} f_n(y_k)$ となります。 $x_0 = a$なので、(2)$_m$から$\lim_{n \to \infty} f_n(a) = u(a)$と導きます。その結果、

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k) .
$$

最後に、(1)$_m$ から、$|\gamma - u(a)| \geq \varepsilon$ が得られるので、$\gamma \neq u(a)$ になります。これ矛盾する主張 (iv);従って、(iv) が (i) を意味することを証明しました。

### 3. エベラインとシュムリアン定理

#### 定理 1 (エバーライン) {#evt-iv-s5-thm-1 .statement tag=07VT}

— *E をハウスドルフとし、E 上の準完全局所凸空間、$\mathscr{T}$ 位相とします。これは、E と E' および E の A 部分集合の間の双対性と互換性があります。A が $\mathscr{T}$ に対して比較的コンパクトであるためには、A の点のすべての無限数列が極限点の E は $\mathscr{T}$ です*。

条件に記載されているものは明らかに必要です。

ここで、A の点のすべての無限数列が $\mathscr{T}$ に対して極限点を持ち、したがってより粗い位相 $\sigma(E, E')$ にも極限点があるとします。この場合、A は $\mathscr{T}$ (IV, p. 32、提案 1) に対して事前圧縮されます。 位数で、A が $\mathscr{T}$ に対して比較的コンパクトであることは、$\sigma(E, E')$ に対しても同様であることが必要かつ十分です (*loc. cit.*)。従って、$\mathscr{T}$が弱体化された位相$\sigma(E, E')$であるときに、定理を証明するだけで十分です。

$\hat{E}$ が E の完成を表すものとし、通常どおり、E' の代数双対 ${E'}^*$ の部分空間と同一視するします (III, p. 21, th. 2)。 $E_\sigma$、$\hat{E}_\sigma$、${E_\sigma'}^*$ が、それぞれトポロジー $\sigma(E, E')$、$\sigma(\hat{E}, E')$、$\sigma({E'}^*, E')$ を備えた空間 E、$\hat{E}$、${E'}^*$ を表すものとします。

$(x'_i)_{i \in I}$ を体 K 上のベクトル空間 E' の基底とします。 写像 $f \mapsto (f(x'_i))_{i \in I}$ は ${E_\sigma'}^*$ から $K^I$ への同型写像 $\phi$ です。 写像 $x'_i$ の下にある A のすべての $i \in I$、像について、E から K への変換は比較的コンパクトです。 なぜなら、K は計量可能であり、$x'_i(A)$ の元の無限のすべての数列は極限点を持ちます。したがって、$K^I$ では$\phi(A)$ が比較的コンパクトであるため、${E_\sigma'}^*$ における A の閉包$\overline{A}$ はコンパクトであることがわかります。

*次に、$\overline{A}$ が $\hat{E}$ に含まれることを証明します。* H を E' の等連続部分集合とします。 X を $\sigma(E', E)$ の終点とします。 X はコンパクトです (III、p. 17、cor. 2)。 すべての $x \in {E'}^*$ について、$\phi_x$ を $x' \mapsto \langle x, x' \rangle$ ～ X の制限とします。 x の範囲が A を超える場合、$\tilde{A} \subset \mathscr{C}_s(X)$ を写像 $\phi_x$ の集合とします。 A の仮定を考慮すると、$\tilde{A}$ の元のすべての無限数列は、$\mathscr{C}_s(X)$ に極限点を持ちます。プロップによって。したがって、2 (IV、p. 33)、集合 $\tilde{A}$ は、$\mathscr{C}_s(X)$ では比較的コンパクトです。 *すべての $a \in \overline{A}$ について、X の写像 $\phi_a$ は連続であることがわかります。* その後、 th から包含 $\overline{A} \subset \hat{E}$ が続きます。 III、p. 21の2つ。

*ここで、$\overline{A}$ が E に含まれることを示します。* A は $E_\sigma$ (IV, p. 32, prop. 1) でプリコンパクトであるため、$E_\sigma$ (III, p. 3, prop. 2) に境界があり、したがって E (IV, p. 1、提案 1)。 C を E における A の閉じた凸平衡包絡線とします。 次に、A が有界であるため C は有界であり、E が準完全であるため完全です。 他の語では、C は$\hat{E}$ の凸で閉じた部分集合であるため、$\hat{E}_\sigma$ (IV、p. 1、提案 1) も同様です。 $A \subset C$ と $\hat{E}_\sigma$ のトポロジーは ${E_\sigma'}^*$ のトポロジーによって誘導されるため、$\overline{A} \subset C$ があり、したがって $\overline{A} \subset E$ になります。

$E_\sigma$ のトポロジーは ${E'_\sigma}^*$ のトポロジーによって誘導されるため、$E_\sigma$ の部分集合 $\overline{A}$ はコンパクトであり、 1が続きます。

#### 定理 2 (シュムリア語) {#evt-iv-s5-thm-2 .statement tag=07VU}

— *E をフレシェ空間とし、A 部分集合を E とします。$E_\sigma$ は、弱体化された位相を備えた空間 E を表します。次の条件は同等* です。

(i) *$E_\sigma$ では比較的コンパクトです;*
(ii) *A の点のすべての無限数列は $E_\sigma$ に極限点を持ちます。*
(iii) *A の点のすべての無限数列から、$E_\sigma$ に収束する数列を抽出できます。

(i) と (ii) の同値は Eberlein の定理から引き継がれており、(iii) は明らかに (ii) を暗示しています。

(i) が (iii) を意味することを証明します。 $E_\sigma$ の A の閉包 B がコンパクトで、$(x_n)_{n \in \mathbf{N}}$ が A の点の数列であるとします。F は、E 含むのベクトル部分空間が $x_n$ で閉ざされた最小のを表すとします。これはフレシェです。 空間満たす可算性の最初の公理。 F は $E_\sigma$ で閉じており、F 上の位相 $\sigma(F, F')$ は $\sigma(E, E')$ によって誘導されるため、集合 $B \cap F$ は $\sigma(F, F')$ に対してコンパクトです。 IV, p. 32 の注意により、$\sigma(E, E')$ (または、$\sigma(F, F')$ についても同様) に収束する $(x_n)_{n \in \mathbf{N}}$ から抽出された数列の存在は、次の補題の帰結になります。

#### 補題 1 {#evt-iv-s5-lem-1 .statement tag=07VV}

— *F を可算性の最初の公理であるフレシェ空間満たすとします。 $\sigma(F, F')$ によって誘導される位相 $\mathscr{T}$ に対してコンパクトである F のすべての部分集合 C は、この位相に対して計量可能です。*

$F'$ でのプレコンパクト収束の位相は位相 $\sigma(F', F)$ よりもより細かいであるため、$F'_s$ (III, p. 18, cor. 1) にはどこにでも密な可算可能部分集合が存在します。したがって、集合 C は、$K^D$ の部分集合と識別でき、C に$K^D$ によって誘発される位相は、計量可能 (GT、IX, § 2, No. 8) によって誘発される位相よりも粗いです。 Cがコンパクトな$\sigma(F, F')$。したがって、これら 2 つのトポロジは同一です (GT、I, § 9, No. 4、cor. 3)。

シュムリアンの定理は、E がフレシェ空間の数列の厳密帰納法極限である場合に拡張できます (IV、p. 67、演習 2)。

### \*4。有界連続写像*の空間の場合

すべての位相空間 X について、$\mathscr{C}^b(X)$ は、X から K までのすべての連続かつ *有界* 写像のバナッハ空間を表し、ノルムは次のように定義されます。

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

(GT、X, § 3, No. 2)。 X がコンパクトな場合、X 上のすべての連続写像は有界 (GT、IV, § 6, No. 1) となり、$\mathscr{C}^b(X)$ に $\mathscr{C}(X)$ を書き込みます。

この文と次の切断では、$\mathscr{C}(X)'$の元をXの対策として解釈することを考慮して、ルベーグの定理（INT、IV、第2版§ 4, No. 3、th.2）の特殊なケースである次の補題を使用します。

#### 補題 2 {#evt-iv-s5-lem-2 .statement tag=07VW}

Xをコンパクトな空間とします。 数列 $(f_n)_{n \in \mathbf{N}}$ が $C(X)$ で制限され、単純に X で連続写像 f に収束する場合、$C(X)'$ のすべての $\mu$ に対して $\mu(f) = \lim_{n \to \infty} \mu(f_n)$ が計算されます。

#### 命題 3 {#evt-iv-s5-prop-3 .statement tag=07VX}

X をコンパクトな空間とし、A を $C(X)$ の有界な部分集合とします。 A が単純収束の位相に対して比較的コンパクトであるためには、A が $\sigma(C(X), C(X)')$ に対して比較的コンパクトであることが必要かつ十分です。

単純収束の位相はハウスドルフであり、$\sigma(C(X), C(X)')$ よりも粗いため、記載されている条件で十分です (GT、I, § 9, No. 4、cor. 3)。

ここで、A が単純収束の位相に対して比較的コンパクトであると仮定します。 $(f_n)_{n \in \mathbf{N}}$ を A の元の数列とします。 2 (IV, p. 33) には、$(f_n)$ から抽出され、単純に連続する写像 f に収束する数列 $(f_{n_k})$ が存在します。 補題 2 までに、有界の数列 $(f_{n_k})$ は $\sigma(C(X), C(X)')$ に向かう傾向があります。次に、シュムリアンの定理 (IV, p. 36, th. 2) は、A が $\sigma(C(X), C(X)')$ に対して比較的コンパクトであることを示しています。

#### 系 {#evt-iv-s5-n4-cor-1 .statement tag=07VY}

S をトポロジー 空間とし、A を $C^b(S)$ の有界部分集合とします。次の条件は同等です。
(i) A は $\sigma(C^b(S), C^b(S'))$ にとって比較的コンパクトです。
(ii) $(f_n)_{n \in \mathbf{N}}$ が A の元の数列であり、$(x_m)_{m \in \mathbf{N}}$ が S の点の数列である場合、反復された極限
$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$
存在する場合、$\gamma = \delta$。

X を S (GT, IX, § 1, No. 6) と $\alpha$ 標準写像を S から X に圧縮した Stone-Čech とする。 D = $\alpha(S)$ と置きます。 写像 $\phi : f \mapsto f \circ \alpha$ は、標準の空間 $C(X)$ から標準の空間 $C^b(S)$ への同型です。 $\tilde{A} = \phi^{-1}(A)$を入れます。 Xはコンパクトで、XはDが密なので、プロップ。 2 (IV, p. 33) は、条件 (ii) が単純収束の位相に対する $\tilde{A}$ のコンパクトさと同等であることを示しています。 (i) と (ii) の同値が prop から続きます。 3. \*

### \*5。弱圧縮の凸包絡線集合

#### 定理 3 (クライン) {#evt-iv-s5-thm-3 .statement tag=07VZ}

E をハウスドルフで準完全な局所凸空間とし、$\mathscr{T}$ を E と E' の間の双対性と互換性のある E 上の位相とします。 A を $\mathscr{T}$ に対してコンパクトな E の部分集合とします。すると、A の閉じた凸平衡包絡線 C は $\mathscr{T}$ に対してコンパクトになります。

まずいくつかの削減を行います。
A) 集合 C は $\mathscr{T}$ (II、p. 25、提案 3) に対してプレコンパクトであり、A は $\sigma(E, E')$ に対してコンパクトです。プロップの都合上。 1 (IV, p. 32) は、C が $\sigma(E, E')$ に対してコンパクトであることを証明するのに十分なので、$\mathscr{T} = \sigma(E, E')$ の場合に帰着しました。
B) C はプリコンパクトで、$\sigma(E, E')$ に対して閉じられているため、E の最初の位相 (III、p. 3、prop. 2 および IV、p. 1、prop. 1) に対して有界で閉じられています。したがって、E は準完全なので完全です。他の語では、Cは$E$の完成$\hat{E}$における$A$の閉じた凸平衡包絡線です。 $E$の位相 $\sigma(\hat{E}, E')$ 誘導する $\sigma(E, E')$ 以降、*$E$が完了した場合*に縮小しました。

C) $\Gamma$ を $A$ の凸型バランス包絡線とします。 次に、$C$ は $\sigma(E, E')$ に対する $\Gamma$ の終結です。 Eberlein の定理 (IV, p. 35, th. 1) により、$\Gamma$ の点のすべての列 $(x_n)_{n \in \mathbf{N}}$ が $E$ の $\sigma(E, E')$ に対する極限点を持つことを証明するだけで十分です。 ただし、$x_n$ 属するは、$A$ の有限部分集合 $B_n$ の凸型バランスエンベロープに変換されます。 $F$ を、可算数集合 $B = \bigcup_n B_n$ によって生成された $E$ の閉じたベクトル部分空間とします。 次に、$F$ が完了し、$F$ の位相 $\sigma(F, F')$ が $\sigma(E, E')$ によって誘導され、すべての $n \in \mathbf{N}$ に対して $x_n \in F$ が得られます。 したがって、$(x_n)_{n \in \mathbf{N}}$ が $\sigma(F, F')$ に対して極限点をもつことを証明するだけで十分です。これにより、$E$* に可算密集合が存在する場合の *case への還元が得られます。

$A$ に $\sigma(E, E')$ によって誘導された位相が割り当てられ、コンパクトな空間になります。私たちは定義する線形写像 $u : E' \to \mathscr{C}(A)$ によって

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, x' \in E') .
$$

$(x'_n)_{n \in \mathbf{N}}$ を $E'$ の等連続数列とし、$\sigma(E', E)$ では 0 に収束します。次に、写像 $u(x'_n)$ の数列は $\mathscr{C}(A)$ で制限され、単純に 0 に収束します。すべての $\mu \in \mathscr{C}(A)'$ について、補題 2 (IV, p. 37) により $\lim_{n \to \infty} \mu(u(x'_n)) = 0$ が得られます。 III、p. 21、線型形式の注意で与えられた基準により、$E'$の$\mu \circ u$は$\mu \in \mathscr{C}(A)'$ごとに$\sigma(E', E)$まで連続します。したがって、線形写像 $v : \mathscr{C}(A)' \to E$ 満たす関係が存在します。

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \mu \in \mathscr{C}(A)') .
$$

$\mathscr{C}(A)'$ が位相 $\sigma(\mathscr{C}(A)', \mathscr{C}(A))$ と $E$ 位相 $\sigma(E, E')$ に割り当てられている場合、$v$ が連続であることは明らかです。

Banach 空間 $\mathscr{C}(A)$ の単位元ボール (クローズ) $B$ は、位相 $\sigma(\mathscr{C}(A)', \mathscr{C}(A))$ (III、p. 17、cor. 3) に対してコンパクトです。従って、$v(B)$ は、$\sigma(E, E')$ に対して、$E$ の凸バランスでコンパクトな部分集合になります。 $a \in A$ ごとに、$\mathscr{C}(A)$ 属するから $B$ まで線型形式 $\varepsilon_a : f \mapsto f(a)$ が続き、公式 (7) と (8) によって $v(\varepsilon_a) = a$ が得られます。従って、$A \subset v(B)$、そして$C \subset v(B)$となります。これは、$C$が$\sigma(E, E')$に対してコンパクトであることを証明しています。

Q.E.D.

### 練習問題 {#evt-iv-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
