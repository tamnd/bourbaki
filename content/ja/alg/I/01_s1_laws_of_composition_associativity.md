---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 1
section_title: Laws of composition; associativity; commutativity
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 1-12, 124-126
pdf_pages: 0025-0036, 0148-0150
extraction: ocr
subsections:
    - "no": 1
      title: LAWS OF COMPOSITION
      page: 1
      pdf_page: 25
    - "no": 2
      title: COMPOSITION OF AN ORDERED SEQUENCE OF ELEMENTS
      page: 3
      pdf_page: 27
    - "no": 3
      title: ASSOCIATIVE LAWS
      page: 4
      pdf_page: 28
    - "no": 4
      title: STABLE SUBSETS. INDUCED LAWS
      page: 6
      pdf_page: 30
    - "no": 5
      title: PERMUTABLE ELEMENTS. COMMUTATIVE LAWS
      page: 7
      pdf_page: 31
    - "no": 6
      title: QUOTIENT LAWS
      page: 11
      pdf_page: 35
statements: 31
exercises: 16
content_sha256: e7e79e4c43db5b1f2c31aac07a6a2e64d078020df41f05e94cf98c416ea3ffbb
translated_from: content/en/alg/I/01_s1_laws_of_composition_associativity.md
translation_method: google
source_content_sha256: 5e673d0115ec27e87cd42d00b10d88a67c6691b3b1a9b1ee5776c4a964875bff
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: b249d5024b5b8a7294cdfcaccc05154ca39ed8b178f1a756578462520e69bd25
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。 合成中法則;結合性。 可換性

### 1. 合成中法則

#### 定義 1 {#alg-i-s1-def-1 .statement tag=055B}

Eを集合とします。 E × E の写像 f を E に入れると、E 上の合成の法則と呼ばれます。 順序付けられた対 (x, y) ∈ E × E に対する f の値 f(x, y) は、この法則の下で x と y の合成と呼ばれます。 合成の法則を持つ集合をマグマと呼びます。

x と y の合成は、通常、x と y を明確な位数で書き、問題の法則の特徴的な記号 (省略することが合意される記号) で区切ることによって表されます。最もよく使用される記号は + と . ですが、通常は必要に応じて後者を省略します。これらの記号を使用すると、x と y の合成は、それぞれ x + y、x.y または xy と書きます。記号 + で示される法則は通常加法 (合成 x + y は x と y の和と呼ばれます) と呼ばれ、加算的に書かれると言います。 法則は の記号で示されます。は通常乗法 (合成 x.y = xy は x と y の積と呼ばれます) と呼ばれ、乗算的に書かれると言います。この章のパラグラフ 1 から 3 の一般論拠では、合成の任意の法則を示すために、一般に記号 ⊔ と ⊓ を使用します。

By an abuse of language, a mapping of a subset of E × E into E is sometimes called a law of composition not everywhere defined on E.

#### 例 {#alg-i-s1-n1-exa-1 .statement tag=055C}

(1) 写像 (X, Y) ↦ X ∪ Y と (X, Y) ↦ X ∩ Y は合成の集合の部分集合の集合 E の法則です。

(2) 自然数、加法、乗法の集合 N およびべき乗は、合成の法則 (これら法則の下で x ∈ N および y ∈ N の合成は、それぞれ x + y、xy または x.y で表され、 x^y) (集合理論, III, § 3, no. 4)。

(3) E を集合とします。 写像 (X, Y) ↦ X ⋅ Y は、E × E (集合理論, II, § 3, no. 3, 定義 6) の部分集合の集合上の合成の法則です。 写像 (f, g) ↦ f ⋅ g は、E の写像の集合上の合成の法則を E に変換します (集合理論, II, § 5, no. 2)。

(4) E を格子 (集合理論, III, § 1, no. 11) とする。 sup(x, y) が集合 {x, y} の最小の上界を表す場合、写像 (x, y) ↦ sup(x, y) は E 上の合成の法則です。 最大の下界 inf(x, y) についても同様です。上記の例 1 は、$\mathfrak{P}(E)$ を含めて順序付けした、この特別なケースです。

(5) $(E_t)_{t \in I}$ をマグマの族とする。 $\tau_t$ が $E_t$ の合成の法則を表すとします。 写像
$$
((x_i), (y_i)) \mapsto ((x_i \tau_t y_i))
$$
積 $E = \prod_{t \in I} E_t$ の合成の法則は、法則 $\tau_t$ の *積* と呼ばれます。この法則が付いた集合Eをマグマ$E_t$の*積マグマ*といいます。特に、すべてのマグマ$E_t$が同じマグマMに等しい場合、M*からIの写像の*マグマが得られます。

$(x, y) \mapsto x \tau y$ を集合 E の合成の法則とします。任意の 2 つの部分集合 X、E の Y、$X \tau Y$ (この記法が混乱を招かない限り†) は、元の集合を表します。 Eの$x \tau y$、$x \in X, y \in Y$（写像$(x, y) \mapsto x \tau y$の下の$X \times Y$の他の語、像）。

$a \in E$ の場合、通常は $\{a\} \tau Y$ の代わりに $a \tau Y$ 、$X \tau \{a\}$ の代わりに $X \tau a$ と書きます。 写像 $(X, Y) \mapsto X \tau Y$ は、E の部分集合の集合にある合成の法則です。

#### 定義 2 {#alg-i-s1-def-2 .statement tag=055D}

*E をマグマとし、$\tau$ はその合成の法則を表します。 Eの合成$(x, y) \mapsto y \tau x$の法則は上記の逆と呼ばれます。 集合 E とこの法則を E の反対のマグマと呼びます*。

E と E' を 2 つのマグマとします。それらの法則を同じ記号 $\tau$ で表します。一般的な定義 (*集合理論*, IV, § 1, no. 5) に準拠し、E に対する E の全単射写像 f は次のようになります。
$$
f(x \tau y) = f(x) \tau f(y)
$$
注文されたすべての対 $(x, y) \in E \times E$ は、E から E'* への *同型と呼ばれます。 E' 上に E の同型が存在する場合、E と E' は *同型* であると言われます。

より一般的には:

#### 定義 3 {#alg-i-s1-def-3 .statement tag=055E}

* 関係 (1) が順序付けされたすべての対 $(x, y) \in E \times E$ に対して成り立つような、E の E から E' への写像 f は、E から E' への準同型または射と呼ばれます。 $E = E'$ の場合、f は E の自己準同型と呼ばれます。*

マグマEの恒等写像は準同型、2つの準同型の合成は準同型です。

† 次の例では、この原則は混乱を招くため、使用すべきではありません。 問題の合成の法則が集合 E の部分集合の間の法則 $(A, B) \mapsto A \cup B$ であるとします。 法則/合成
$$
(\mathscr{A}, \mathscr{B}) \mapsto F(\mathscr{A}, \mathscr{B})
$$
$\mathfrak{P}(E)$の部分集合、$F(\mathscr{A}, \mathscr{B})$は$A \cup B$の集合と$A \in \mathscr{A}, B \in \mathscr{B}$の間で導出されます。ただし、$F(\mathscr{A}, \mathscr{B})$ は $\mathscr{A} \cup \mathscr{B}$ で表されるべきではありません。この記法にはすでに別の意味があります ($\mathscr{A}$ の和集合と $\mathscr{B}$ は $\mathfrak{P}(E)$ の部分集合と見なされます)。

E から E' への写像 $f$ が同型であるためには、それが全単射準同型であり、そのとき $f^{-1}$ が E' から E への同型であることが必要十分です。

### 2. 注文済みの合成のうち数列の元

集合 E の元のファミリーは、E への集合 I の写像 $i \mapsto x_i$ (インデックス付け集合と呼ばれます) であることを思い出してください。インデックス付け集合が有限である場合、ファミリー $(x_i)_{i \in I}$ は有限と呼ばれます。

インデックス付け集合 I が完全に順序付けされている E の元の有限族 $(x_i)_{i \in I}$ は、E の元の順序付き数列と呼ばれます。

In particular, every finite sequence $(x_i)_{i \in H}$, where H is a finite subset of the set $\mathbf{N}$ of natural numbers, can be considered as an ordered sequence if H is given the order relation induced by the relation $m \leq n$ between natural numbers.

すべての $i \in I$ に対して $y_{\phi(i)} = x_i$ となるような、K 上に I の順序付き集合同型 $\phi$ が存在する場合、2 つの順序付き数列 $(x_i)_{i \in I}$ と $(y_k)_{k \in K}$ は類似していると呼ばれます。

注文されたすべての数列 $(x_\alpha)_{\alpha \in A}$ は、適切な有限列と同様です。なぜなら、$\mathbf{N}$の区間$[0, n]$の上にAの増加する全単射が存在するからです。

#### 定義 4 {#alg-i-s1-def-4 .statement tag=055F}

*$(x_\alpha)_{\alpha \in A}$ * を、インデックス集合 A が空ではないマグマ E 内の元の順序付けられた数列とします。注文された数列* $(x_\alpha)_{\alpha \in A}$ の合成 (法則 T の下)、*で示される* $\prod_{\alpha \in A} x_\alpha$、* は、次のように A の元の数に帰納法によって定義される E の元です。

(1) *if* $A = \{\beta\}$ *then* $\prod_{\alpha \in A} x_\alpha = x_\beta$;

(2) A が * $p > 1$ *元である *場合、* A * および* $A' = A - \{\beta\}$ のうち、$\beta$ が最小の元である場合、*その後* $\prod_{\alpha \in A} x_\alpha = x_\beta \ T \left( \prod_{\alpha \in A'} x_\alpha \right)$ となります。

(インデックス作成集合の元の数の帰納法によって) 2 つの類似した順序数列の合成が等しいことがすぐに続きます。特に、注文された数列の合成は、有限列の合成と等しくなります。 $A = \{\lambda, \mu, \nu\}$ に元 ($\lambda < \mu < \nu$) が 3 つある場合、合成 $\prod_{\alpha \in A} x_\alpha$ は $x_\lambda \ T \ (x_\mu \ T \ x_\nu)$ です。

#### 注意 {#alg-i-s1-n2-rem-1 .statement tag=055G}

順序付けられた数列の合成の定義については、ある程度の恣意性があることに注意してください。 帰納法収益を「右から左へ」導入しました。 「左から右」に進むと、上記の数列 $(x_\lambda, x_\mu, x_\nu)$ のうち合成は $(x_\lambda \ T \ x_\mu) \ T \ x_\nu$ になります。

記法の問題として、注文された数列 $(x_\alpha)_{\alpha \in A}$ の合成は、$\perp$ で示される法則に対して $\prod_{\alpha \in A}$ と書き込まれます。加法的に書かれた法則の場合、通常は$\sum_{\alpha \in A} x_\alpha$で表され、数列$(x_\alpha)_{\alpha \in A}$の順序の和と呼ばれます（$x_\alpha$は和の項と呼ばれます）。乗算的に書かれた法則は通常 $\prod_{\alpha \in A} x_\alpha$ で表され、順序付けられた数列 $(x_\alpha)$ の *積* と呼ばれます ($x_\alpha$ は積の *因子* と呼ばれます)。

インデックス付け集合 (またはその順序付け) に混乱の可能性がない場合、順序付けされた数列の合成の記法では省略されることが多く、たとえば法則については加法的に次のように記述します。
$\sum_{\alpha \in A} x_\alpha$ の代わりに $\sum_\alpha x_\alpha$;もう一方の記法についても同様です。

集合のインデックスを持つ *数列* $(x_i)$ の $\top$ 合成で表される法則の場合、$\mathbf{N}$ の空でない区間 $[p, q]$ は $\prod_{p \leq i \leq q} x_i$ または $\prod_{i=p}^q x_i$ で表されます。他の記号で示される法則についても同様です。

E と F を 2 つのマグマとし、その合成の法則が E の $\top$ と $f$ 準同型で F に表されるものとします。 E の数列 $(x_\alpha)_{\alpha \in A}$ の元を注文するたびに
$$
f\left( \prod_{\alpha \in A} \right) = \prod_{\alpha \in A} f(x_\alpha).
$$

### 3. 連想法則

#### 定義 5 {#alg-i-s1-def-5 .statement tag=055H}

*A law of composition* $(x, y) \mapsto x \top y$ *on a set* E *is called associative if, for all elements* $x, y, z$ *in* E,
$$
(x \top y) \top z = x \top (y \top z).
$$
*A magma whose law is associative is called an associative magma*.

結合法則の反対の法則は結合です。

#### 例 {#alg-i-s1-n3-exa-1 .statement tag=055I}

(1) 自然数の加法と乗法は、$\mathbf{N}$ 上の合成の法則と結合します (*集合理論*、III, § 3, no. 3、系 ～ 命題 5)
(2) 例のno. 1の(1)、(3)、(4)で引用されている法則は連想的です。

#### 定理 1 (結合性定理) {#alg-i-s1-thm-1 .statement tag=055J}

*E *を、その法則が * $\top$ で表される結合マグマとしましょう。 *A * を完全に順序付けされた空でない有限集合とし、これは空でない部分集合* $(B_i)_{i \in I}$ * 関係* $\alpha \in B_i, \beta \in B_j, i < j$ *暗黙* $\alpha < \beta$ の順序付けられた数列の和集合です。 * $(x_\alpha)_{\alpha \in A}$ * を、* E * の元の順序付けられた数列とし、* A を * インデックス付け集合* として使用します。 *それでは*
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right)
$$

† この用語と記法 $\prod_{\alpha \in A} x_\alpha$ の使用は、集合の理論 (*集合理論*、II, § 5, no. 3) で定義される集合 $x_\alpha$ の積と混同される危険がある場合には避けなければなりません。ただし、$x_\alpha$ が基数で、加法 (それぞれ乗法) が基数和 (それぞれ基数積) である場合、基数は $\sum_{\alpha \in A} x_\alpha$ (それぞれ乗法) で表されます。上の記法の$\prod_{\alpha \in A} x_\alpha$)は、家族$(x_\alpha)_{\alpha \in A}$(*集合理論*、III, § 3, no. 3)の基数和(それぞれ基数積)です。

§ 1.3

$A$ の基数 $n$ で定理を帰納法で証明します。 $p$ を $I$ の基数と、$h$ の最小値元とします。 $J = I - \{h\}$ にしましょう。 $B_i$ が空ではないので、$n = 1$ の場合、必然的に $p = 1$ と定理は明らかです。それ以外の場合、定理が最大 $n - 1$ 元のインデックス付け集合に当てはまると仮定すると、次の 2 つのケースが区別されます。

(a) $B_h$ には 1 つの元 $\beta$ があります。 $C = \bigcup_{i \in J} B_i$ にしましょう。 (3) の左辺は、定義だけ$x_\beta \top \left( \prod_{\alpha \in C} x_\alpha \right)$ に等しくなります。右辺は定義だけ等しいので、
$$
x_\beta \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right);
$$
この結果は、定理が $C$ と $(B_i)_{i \in J}$ に対して真であると想定されるという事実から得られます。

(b) それ以外の場合、$\beta$ を $A$ (したがって $B_h$) の最小値元とします。 $A' = A - \{\beta\}$ を$i \in I$ として$B'_i = A' \cap B_i$ にします。次に、$i \in J$の場合は$B'_i = B_i$です。 集合 $A'$ には $n - 1$ 元と定理の条件は $A'$ とその部分集合 $B'_i$ に当てはまります。したがって、仮定までに:
$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{\alpha \in B'_h} x_\alpha \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right).
$$
各辺で $x_\beta$ の合成を形成すると、左側には定義、$\prod_{\alpha \in A} x_\alpha$ が、右側には結合性を使用して、
$$
\left( x_\beta \top \left( \prod_{\alpha \in B'_h} x_\alpha \right) \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right)
$$
これは、公式 (3) の右辺に定義 3 を加えたものと等しくなります。

$\top$ 合成 $\prod_{p \leq i \leq q} x_i$ の数列 $(x_i)_{i \in [p, q]}$ で表される結合法則は、(混乱が生じないため) とも表されます。
$$
x_p \top \cdots \top x_q.
$$
定理 1 の特定のケースは公式
$$
x_0 \top x_1 \top \cdots \top x_n = (x_0 \top x_1 \top \cdots \top x_{n-1}) \top x_n.
$$
項がすべて同じ元 $x \in E$ に等しい、$n$ 項の順序付き数列を考えてみましょう。この数列の合成は$\top$で示される法則に対して$\prod^n x$で示され、$\perp$で示される法則は$\prod^n x$となります。 法則を乗算的に書くと、合成は $x^n$ で表され、$x$ の $n$ 番目 *冪* と呼ばれます。加法的に書かれた法則の場合、合成は通常$nx$で表されます。 項がすべて等しい順序付けられた数列に結合性定理を適用すると、次の方程式が得られます。

$$
\frac{n_1 + n_2 + \cdots + n_p}{T} x = \left( \frac{n_1}{T} x \right) T \left( \frac{n_2}{T} x \right) T \cdots T \left( \frac{n_p}{T} x \right).
$$

特に $p = 2$ の場合、

$$
\frac{m+n}{T} x = \left( \frac{m}{T} x \right) T \left( \frac{n}{T} x \right)
$$
$n_1 = n_2 = \cdots = n_p = m$ の場合、
$$
\frac{pm}{T} x = \frac{p}{T} \left( \frac{m}{T} x \right).
$$

$X$ が $E$ の部分集合である場合、上記の記法に従って、ときどきは $\frac{p}{T} X$ 集合 $X_1 T X_2 T \cdots T X_p$ で表されます。
$$
X_1 = X_2 = \cdots = X_p = X;
$$
したがって、合成 $x_1 T x_2 T \cdots T x_p$ と $x_1 \in X, x_2 \in X, \ldots, x_p \in X$ のすべての集合になります。

この集合を $\frac{p}{T} x$ の集合 ($x$ から $X$ まで) と混同しないことが重要です。

### 4. 安定の部分集合。誘導法則

#### 定義 6 {#alg-i-s1-def-6 .statement tag=055K}

* 集合 $E$ の部分集合 $A$ は、$A$ 属するの 2 つの元のうち合成が $E$ の合成 $T$ の法則の下で安定と呼ばれます。 $A$。 $A \times A$ の $A$ への写像 $(x, y) \mapsto x T y$ は、法則 $T$ によって $A$ に誘導された法則と呼ばれます。 $T$によって誘発された法則を伴う集合$A$を$E$のサブマグマと呼びます*。

他の語では、$A$ が法則 $T$ で安定するには、$A T A \subset A$ であることが必要かつ十分です。 $E$ および対応するのサブマグマの安定した部分集合がよく確認されます。

安定した家族の共通部分 $E$ の部分集合は安定しています。特に、特定の部分集合 $X$ には、$E$ 含むの最小の安定した部分集合 $A$ が存在します。それは$X$によって*生成*され、$X$は$A$の*生成する系*、または$A$の*生成する集合*と呼ばれます。 対応するサブマグマは $X$ によって*生成*されるとも言われています。

#### 命題 1 {#alg-i-s1-prop-1 .statement tag=055L}

※$E$と$F$を2つのマグマとし、$E$の$f$準同型を$F$とします。
(i) $E$ の安定した部分集合の $f$ の下の像は、$F$ の安定した部分集合です。
(ii) 部分集合 $F$ の$f$ の下にある逆像は、$E$ の安定した部分集合です。
(iii) $X$ を $E$ の部分集合とします。 The image under $f$ of the stable subset of $E$ generated by $X$ is the stable subset of $F$ generated by $f(X)$.
(iv) If $g$ is a second homomorphism of $E$ from $F$ the set of elements $x$ of $E$ such that $f(x) = g(x)$ is a stable subset of $E$.*

主張 (i)、(ii)、(iv) は明らかです。 (iii) を証明します。 $\overline{X}$ を X によって生成された E の安定した部分集合とし、$\overline{f(X)}$ を $f(X)$ によって生成された F の安定した部分集合とします。 (i) $\overline{f(X)} \subset f(\overline{X})$ および (ii) $\overline{X} \subset f^{-1}(\overline{f(X)})$、よって $f(\overline{X}) \subset \overline{f(X)}$ により。

#### 命題 2 {#alg-i-s1-prop-2 .statement tag=055M}

*E を連想マグマ、E の X 部分集合とします。X' を $x_1 \top x_2 \top \cdots \top x_n$ の集合とします。$n \geq 1$ と $x_i \in X$ は $1 \leq i \leq n$ です。 X によって生成される安定した部分集合は X' に等しいです。

n 上の帰納法の直後に、n 項所属から X 属するの順序付けられた数列の合成が、X によって生成された安定した部分集合に続きます。したがって、X' が安定していることを確認するだけで十分です。ここで、u と v が X の元である場合、それらは形 $u = x_0 \top x_1 \top \cdots \top x_{n-1}$、$v = x_n \top x_{n+1} \top \cdots \top x_{n+p}$ であり、$0 \leq i \leq n + p$ の場合は $x_i \in X$ です。次に (定理 1) $u \top v = x_0 \top x_1 \top \cdots \top x_{n+p}$ 属するから X'。

#### 例 {#alg-i-s1-n4-exa-1 .statement tag=055N}

(1) 自然数の集合 $\mathbf{N}$ では、{1} によって生成された加法の安定した部分集合は整数 $\geq 1$ の集合です。 乗法集合 {1} 未満は安定しています。

(2) 集合 E で法則 $\top$ が与えられた場合、単一の元の部分集合 {h} からなるが法則 $\top$ で安定するには、$h \top h = h$ であることが必要かつ十分です。その場合、 h は *冪等元*であると言われます。たとえば、格子のすべての元は、 法則 sup と inf のそれぞれに対して冪等です。

(3) 集合 E 上の結合法則 $\top$ の場合、単一元の集合 {a} からなるによって生成される安定部分集合は、元の集合です。 $\overline{\top}^n a$、n は整数 $> 0$ の集合を通過します。

### 5. 変更可能元。可換法則

#### 定義 7 {#alg-i-s1-def-7 .statement tag=055O}

*E を法則が $\top$ で表されるマグマとする。 E の 2 つの元 x と y は、$y \top x = x \top y$ の場合に可換 (または置換可能) と言われます。*

#### 定義 8 {#alg-i-s1-def-8 .statement tag=055P}

* 集合 E 上の合成の法則は、E の任意の 2 つの元がこの法則の下で可換である場合、可換と呼ばれます。 合成の法則が可換であるマグマを可換マグマといいます。

可換法則はその反対のものと等しい。

#### 例 {#alg-i-s1-n5-exa-1 .statement tag=055Q}

(1) 自然数の加法と乗法は、$\mathbf{N}$ で可換法則 (*集合理論*、III, § 3, no. 3、系 ～ 命題) 5)。

(2) 格子法則では sup と inf は可換です。したがって、特に、集合 E の部分集合の間にある法則 $\cup$ と $\cap$ です。

(3) E を基数 $> 1$ の集合とします。 E から E への写像の間の法則 $(f, g) \mapsto f \circ g$ は、f と g を別個の定数写像とすることからわかるように可換ではありませんが、恒等写像はすべての写像と置換可能です。

(4) $(x, y) \mapsto x \top y$ を $E$ 上の可換法則とする。 法則
$$
(X, Y) \mapsto X \top Y
$$
部分集合と $E$ の間は可換です。

#### 定義 9 {#alg-i-s1-def-9 .statement tag=055R}

※$E$をマグマ、$E$の$X$部分集合とします。 $X$の元のそれぞれと交換する$E$の元の集合は、$X$のセントラライザーと呼ばれます。

$X$ と $Y$ を、$E$ と $X'$ および $Y'$ の 2 つの部分集合とします。 $X \subset Y$の場合は、$Y' \subset X'$。

$(X_i)_{i \in I}$ を $E$ の部分集合の家族とし、すべての $i \in I$ について、$X'_i$ を $X_i$ の中心者とします。 $\bigcup_{i \in I} X_i$ のセントラライザーは $\bigcap_{i \in I} X'_i$ です。

$X$ を $E$ の部分集合と $X'$ を $X$ のセントラライザーとします。 $X'$ のセントラライザー $X''$ は、$X$ の *bicentralizer* と呼ばれます。次に$X \subset X''$。 $X''$ のセントラライザー $X'''$ は $X'$ に等しい。というのは、$X'$ はそのバイセントラライザー $X'''$ に含まれており、関係 $X \subset X''$ は $X'''' \subset X'$ を暗示します。

#### 命題 3 {#alg-i-s1-prop-3 .statement tag=055S}

*$E$を法則が$\top$で表される結合マグマとする。 $E$ の元 $x$ が、$E$ の元 $y$ および $z$ のそれぞれと交換する場合、$y \top z$ と交換します。*

のために
$$
x \top (y \top z) = (x \top y) \top z = (y \top x) \top z \\
= y \top (x \top z) = y \top (z \top x) = (y \top z) \top x.
$$

#### 系 {#alg-i-s1-n5-cor-1 .statement tag=055T}

*$E$を連想マグマとします。 $E$ の任意の部分集合のセントラライザーは、$E$ の安定した部分集合です。*

#### 定義 10 {#alg-i-s1-def-10 .statement tag=055U}

※マグマ$E$の求心器は$E$の中心と呼ばれます。 $E$の中心の元は、$E$の中心元と呼ばれます*。

$E$ が結合マグマである場合、その中心は系から命題 3 による安定な部分集合であり、その中心で誘導される法則は可換です。

#### 命題 4 {#alg-i-s1-prop-4 .statement tag=055V}

*$E$を連想マグマ、$X$と$Y$を$E$の2つの部分集合とする。 $X$ のすべての元が $Y$ のすべての元と交換する場合、$X$ によって生成された安定した部分集合のすべての元が、$Y$ によって生成された安定した部分集合のすべての元と交換します。

$X'$ と $X''$ を $X$ の集中化者と双集中化者とする。 $E$の部分集合が安定しています。現在、$X \subset X''$ と $Y \subset X'$、したがって $X''$ (それぞれ $X'$) 含むは、$X$ (それぞれ $Y$) によって生成された $E$ の安定した部分集合です。 $X''$ のすべての元が $X'$ のすべての元と交換するため、命題が続きます。

#### 系 1 {#alg-i-s1-prop-4-cor-1 .statement tag=055W}

*$x$ と $y$ が結合法則 $\top$ で置換可能な場合、整数 $m > 0$ と $n > 0$ のすべてに対して $\top^m x$ と $\top^n y$ も同様です。特に、$\top^m x$ と $\top^n x$ は、すべての $x$ とすべての整数 $m > 0$ および $n > 0$ に対して置換可能です。*

#### 系 2 {#alg-i-s1-prop-4-cor-2 .statement tag=055X}

*部分集合 X の元のすべての対が結合法則 T の下で置換可能である場合、X によって生成された安定な部分集合上で T によって誘導された法則は結合かつ可換です。

#### 定理 2 (可換性定理) {#alg-i-s1-thm-2 .statement tag=055Y}

*T を E 上の合成の結合法則とします。 $(x_\alpha)_{\alpha \in A}$ をペアごとに置換可能な E の元の空でない有限族とする。 B と C を合計 2 つの順序集合とし、A を基礎となる集合とします。それから*
$$
\prod_{\alpha \in B} x_\alpha = \prod_{\alpha \in C} x_\alpha.
$$

A に 1 つの元がある場合、定理が真であるため、A の元の数 $p$ について帰納法によって議論します。$p$ を整数 > 1 とし、カード A < のときに定理が真であると仮定します。 $p$。カード A = $p$ について証明します。 A は $\mathbf{N}$ の区間 $[0, p - 1]$ であると仮定できます。 A 上の自然な位数関係によって定義される順序付けられた数列 $(x_\alpha)_{\alpha \in A}$ の合成は $\prod_{i=0}^{p-1} x_i$ です。

A に他のの合計順序付けが与えられ、h をこの順序付けに基づく A の最小の元と、A の他の元の A' 集合 (誘導順序付けによって合計順序付け) とします。最初に $0 < h < p - 1$ と仮定し、P = $\{0, 1, \ldots, h - 1\}$ および Q = $\{h + 1, \ldots, p - 1\}$ とします。 定理が A' に対して真であると仮定すると、適用結合性定理が得られます ($A' = P \cup Q$ 以降)

$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right)
$$

よって、両側で$x_h$を構成し、適用可換性とTの結合性を繰り返す:

$$
\begin{align*}
\prod_{\alpha \in A} x_\alpha &= x_h \circ \left( \prod_{\alpha \in A'} x_\alpha \right) = x_h \circ \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right) \\
&= \left( \prod_{i=0}^{h-1} x_i \right) \circ x_h \circ \left( \prod_{i=h+1}^{p-1} x_i \right) = \prod_{i=0}^{p-1} x_i,
\end{align*}
$$

この場合、これは定理を証明します。 $h = 0$ または $h = p - 1$ の場合も同じ結果が続きますが、より単純には、P から生じる項または Q から生じる項が式に現れません。

集合 E 上の可換結合法則の下では、*有限族* の *合成* 元の $(x_\alpha)_{\alpha \in A}$ は、すべての定義共通の値合成によって決まります。 A をすべての可能な方法で完全に順序付けることによって得られる *順序付けられた数列*。この合成は、引き続き T で示される法則の下で $\prod_{\alpha \in A} x_\alpha$ で示されます。他の記法についても同様です。

#### 定理 3 {#alg-i-s1-thm-3 .statement tag=055Z}

*T を E 上の結合法則と、ペアごとに置換可能な E の元の空でない有限族 $(x_\alpha)_{\alpha \in A}$ とします。 A が空ではない部分集合 $(B_i)_{i \in I}$ のペア互いに素の和集合である場合、*

$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

これは、$A$ と $I$ が完全に順序付けされている場合、定理 1 の $B_i$ 満たす条件が成り立つ場合、定理 2 から続きます。

この定理の 2 つの重要な特殊ケースを取り上げます。

1. $(x_{\alpha \beta})_{(\alpha, \beta) \in A \times B}$ が、インデックス付け集合が 2 つの空ではない有限集合 $A, B$ の積である連想マグマの置換可能な元の有限族である場合 (「二重族」)、

$$
\prod_{(\alpha, \beta) \in A \times B} x_{\alpha \beta} = \prod_{\alpha \in A} \left( \prod_{\beta \in B} x_{\alpha \beta} \right) = \prod_{\beta \in B} \left( \prod_{\alpha \in A} x_{\alpha \beta} \right)
$$

定理 3 から、$A \times B$ を、一方では集合 $\{\alpha\} \times B$ の和集合として、もう一方では集合 $A \times \{\beta\}$ の和集合として考えると、次のようになります。

たとえば、$B$ に $n$ 元があり、各 $\alpha \in A$ に対してすべての $x_{\alpha \beta}$ が同じ値 $x_\alpha$ を持っている場合、

$$
\prod_{\alpha \in A} \left( \prod^n_{\beta=1} x_\alpha \right) = \prod^n_{\alpha=1} \left( \prod_{\alpha \in A} x_\alpha \right).
$$

$B$ に 2 つの元がある場合、次の結果が得られます: $(x_\alpha)_{\alpha \in A}, (y_\alpha)_{\alpha \in A}$ を $E$ の元の 2 つの空ではないファミリーとします。 $x_\alpha$ と $y_\beta$ がペアごとに変更可能である場合、

$$
\prod_{\alpha \in A} x_\alpha \prod_{\alpha \in A} y_\alpha = \left( \prod_{\alpha \in A} x_\alpha \right) \prod_{\alpha \in A} y_\alpha.
$$

double 数列 $(x_{ij})$ の公式 (7) 合成のインデックス付け集合は、$\mathbf{N}$ の 2 つの区間 $\{p, q\}$ と $\{r, s\}$ の積であり、可換結合として表されることが多いためです。 法則によって追加的に書かれました

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij} \quad \text{or} \quad \sum_{j=r}^s \sum_{i=p}^q x_{ij}
$$

他の記号で示される法則についても同様です。

2. $n$ を整数 $> 0$ とし、$A$ を整数 $(i, j)$ の順序付けられた対の集合とし、$0 \leq i \leq n, 0 \leq j \leq n$ と $i < j$ とします。家族 $(x_{ij})_{(i, j) \in A}$ (可換結合法則の下) の合成は、$\prod_{0 \leq i < j \leq n} x_{ij}$ (または、混乱が生じない場合は単に $\prod_{i < j} x_{ij}$) によっても表されます。 定理 3 は式を示します

$$
\prod_{0 \leq i < j \leq n} x_{ij} = \prod_{i=0}^{n-1} \left( \prod_{j=i+1}^n x_{ij} \right) = \prod_{j=1}^n \left( \prod_{i=0}^{j-1} x_{ij} \right).
$$

There are analogous formulae to (7) for a family whose indexing set is the product of more than two sets and analogous formulae to (10) for a family whose indexing set is the set $S_p$ of *strictly increasing sequences* $(i_k)_{1 \leq k \leq p}$ of $p$ integers such that $0 \leq i_k \leq n$ ($p \leq n + 1$): in the latter case the composition of the family $(x_{i_1 i_2 \ldots i_p})_{(i_1, \ldots, i_p) \in S_p}$ is denoted by

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p < n} x_{i_1 i_2 \ldots i_p} \quad \text{or simply} \quad \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \ldots i_p}.
$$

#### 命題 5 {#alg-i-s1-prop-5 .statement tag=0560}

E と F をマグマとし、法則を T で表し、f と g を E から F への準同型とします。f T g を E から F への写像 x ↦ f(x) T g(x) とします。F が結合的かつ可換である場合、f T g は準同型です。

E のすべての元 x と y について:

$$(f T g)(x T y) = f(x T y) T g(x T y) = f(x) T f(y) T g(x) T g(y)$$
$$= f(x) T g(x) T f(y) T g(y) = ((f T g)(x)) T ((f T g)(y)).$$

### 6. 商法則

#### 定義 11 {#alg-i-s1-def-11 .statement tag=0561}

Eを集合とします。 A law of composition T and an equivalence relation R on E are said to be compatible if the relations x ≡ x' (mod R) and y ≡ y' (mod R) (for x, x', y, y' ∈ E) imply x T y ≡ x' T y' (mod R); the law of composition on the quotient set E/R which maps the equivalence classes of x and y to the equivalence class of x T y is called the quotient law of the law T with respect to R. 商法則を持つ集合 E/R を R に対して E の商マグマと呼びます。

E 上の同値関係 R が合成 f: E × E → E の内部法則と互換性があると言うことは、写像 f が (集合理論、II, § 6, no. 5 の意味で) 積同値関係 R × R on E × E と互換性があることを意味します。 同値関係 R on E. (集合理論、II, § 6, no. 8)。これは、R のグラフが E × E のサブマグマであることも意味します。

法則 T が結合性 (可換性) であれば、商法則も同様です (より簡単に言うと、移行から商までのときに結合性、つまり可換性が維持されると言います)。

マグマEからマグマE/Rまでの標準写像は準同型です。

マグマ F への E/R 写像 g が準同型であるためには、E/R への E/R の標準写像を伴う g の合成が準同型であることが必要かつ十分です。

命題に続く 2 つは、定義の明らかです。

#### 命題 6 {#alg-i-s1-prop-6 .statement tag=0562}

E と F を 2 つのマグマとし、E の f 準同型を F にするとします。R[x, y] は、E の元 x, y の間の関係 f(x) = f(y) を表します。すると、R は、E の法則および次の式で f から導出される f(E) 上の E/R の写像と互換性のある E 上の同値関係になります。 移行から商は、Fのサブマグマf(E)上にある商マグマE/Rの同型です。

#### 命題 7 {#alg-i-s1-prop-7 .statement tag=0563}

E をマグマとし、E 上の R 同値関係が E 上の法則と互換性があるとします。E/R 上の同値関係 S が商法則と互換性があるためには、S が形 T/R であることが必要かつ十分であり、ここで T は R によって暗示される E 上の同値関係であり、E 上の法則と互換性があります。 E. (E/R)/(T/R) 上の E/T の標準写像 (集合理論, II, § 6, no. 7) はマグマ同型です。

#### 命題 8 {#alg-i-s1-prop-8 .statement tag=0564}

E をマグマ、A を E の安定した部分集合とし、E 上の R 同値関係は E 上の法則と互換性があります。R に対する A の飽和 B (集合)

理論、II、、、no. 5）は安定の部分集合です。 $A$と$B$でそれぞれ$R$によって誘導された同値関係$R_A$と$R_B$は、$A$の標準単射から$B$に誘導された法則と写像と互換性があります。 移行から商は、$A / R_A$の$B / R_B$上のマグマ同型です

$\top$ が $E$ の法則を表すとします。 $x$と$y$が$B$の2つの元である場合、$x \equiv x' \pmod{R}$と$y \equiv y' \pmod{R}$のように、$A$の2つの元$x'$と$y'$が存在します。次に$x \top y \equiv x' \top y' \pmod{R}$と$x' \top y' \in A$、よって$x \top y \in B$。したがって、$B$ は $E$ の安定した部分集合であり、他の主張は明らかです。

$M$ をマグマ、$((u_\alpha, v_\alpha))_{\alpha \in I}$ を $M \times M$ の元の族とします。 $M$ のすべての同値関係 $S$ は、$M$ の法則と互換性があり、すべての $\alpha \in I$ については $u_\alpha \equiv v_\alpha \pmod{S}$ であることを考慮してください。これら関係のグラフのうち共通部分は、$M$の法則や$u_\alpha \equiv v_\alpha \pmod{R}$と互換性のある同値関係$R$のグラフです。したがって、$R$ は、これら 2 つの特性を持つ最高級 (集合理論、III, § 1、番号 3 および 7) 同値関係です。これは、$(u_\alpha, v_\alpha)$ によって生成された $M$ の法則と互換性のある同値関係と呼ばれます。

#### 命題 9 {#alg-i-s1-prop-9 .statement tag=0565}

上記の記法を保存して、$f$を$M$の準同型として、すべての$\alpha \in I$に対して$f(u_\alpha) = f(v_\alpha)$となるようなマグマにします。次に、$f$ は $R$ と互換性があります。

$T$ を $f$ に関連付けられた同値関係とします。次に、すべての $\alpha \in I$ と $T$ に対する $u_\alpha \equiv v_\alpha \pmod{T}$ は、$M$ の法則と互換性があるため、$T$ は $R$ より粗くなります。これは命題を証明します。

### 練習問題 {#alg-i-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
