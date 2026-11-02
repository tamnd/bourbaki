---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 6
section_title: Etale algebras
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.26-A V.36, A V.151
pdf_pages: 0140-0150, 0265-0265
extraction: ocr
subsections:
    - "no": 1
      title: Linear independence of homomorphisms
      page: 26
      pdf_page: 140
    - "no": 2
      title: Algebraic independence of homomorphisms
      page: 28
      pdf_page: 142
    - "no": 3
      title: Diagonalizable algebras and etale algebras
      page: 28
      pdf_page: 142
    - "no": 4
      title: Subalgebras of an etale algebra
      page: 30
      pdf_page: 144
    - "no": 5
      title: Separable degree of a commutative algebra
      page: 31
      pdf_page: 145
    - "no": 6
      title: Differential characterization of etale algebras
      page: 33
      pdf_page: 147
    - "no": 7
      title: Reduced algebras and etale algebras
      page: 34
      pdf_page: 148
statements: 22
exercises: 2
content_sha256: 03189d2a48c88c6d1468be5be1c20fc7296bd8980bbda2f0131847bc85b5d052
translated_from: content/en/alg/V/06_s6_etale_algebras.md
translation_method: google
source_content_sha256: 3c20d3c3070caf43cf4bd713b7f6047a4fcb2604b1f551ae1ea6b1868b0306eb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 4db91e778aaf3730cf7657962eb897ba2114cf5e6fedfdedc58e1b03393778f0
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。エタール代数

この段落全体を通じて、K は体を表します。

### 1. 準同型の線形独立性

LをKの拡大、K上のVベクトル空間とします。この段落では、VのすべてのK-線型写像をLにベクトル空間構造を備えた$\operatorname{Hom}_K(V, L)$集合で表します。 L 次のようになります:

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

$\mathrm{Hom}_K(V, L)$の$x \in V,\ a \in L$と$f,\ g$用。 $V_{(L)} = L \otimes_K V$ を V からスカラーの拡大で導出し、L 上のベクトル空間とし、その双対を $(V_{(L)})^*$ とします。 II、p. 277 までに、ベクトル L のうち $(V_{(L)})^*$ から $\mathrm{Hom}_K(V, L)$ までのスペースが標準同型 $u \mapsto 3$ になり、$x \in V$ と $u$ には $\tilde{u}(x) = u(1 \otimes x)$ が入ります。 $(V_{(L)})^*$。 V が *有限* である場合、$K$ 上の次元 $n$、$L$ 上のベクトル空間 $(V_{(L)})$ は、次元 $n$ およびその双対 $(V_{(L)})^* = V_{(\bar{L})}^*$ です。 よって公式

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### 定理 1 {#alg-v-s6-thm-1 .statement tag=06JB}

— *L を体 K の拡大および K 上の A 代数とします。 $\mathscr{H}$ を A のすべての K-代数準同型の集合を L にします。その場合、$\mathscr{H}$ は、L 上のベクトル空間 $\mathrm{Hom}_K(A, L)$ の無料の部分集合です。*

整数 $n \geq 0$ の帰納法によって、$\mathscr{H}$ の個別の元のすべての数列 $(u_1, \ldots, u_n)$ が無料であることを示しましょう。 $n = 0$ の場合は自明なので、今後は $n \geq 1$ と仮定します。 $a_1, \ldots, a_n$ を L の元として、A の $x,\ y$ に対して $$\sum_{i=1}^n \alpha_i u_i = 0.$$ が成り立つようにします。
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
よって $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ 帰納法の仮定までに、$\mathscr{H}$ の元 $u_1, \ldots, u_{n-1}$ は線形独立であり、$1 \leq i \leq n-1$ と A のすべての $x$ に対してよって $\alpha_i [u_i(x) - u_n(x)] = 0$ が線形独立です。 $u_i$ は別個であるため、これは、$i \neq n$ に対して $\alpha_i = 0$、したがって $\alpha_n u_n = 0$、したがって $\alpha_n = \alpha_n u_n(1) = 0$ (A の 1 単位元で表すと) を意味します。 したがって、$a_1, \ldots, a_{n-1}, \alpha_n$ は零であることが示され、これにより定理が証明されます。

#### 系 1 {#alg-v-s6-thm-1-cor-1 .statement tag=06JC}

— *$\Gamma$ をモノイド、$\Gamma$ の準同型の L 体と X 集合を L の乗法モノイドとします。次に、X は、ベクトルのL の空き部分集合と、$\Gamma$ の写像の $L^\Gamma$ が L に追加されます。

A を、L の係数と、L (III, p. 446) 上の A の $(e_\gamma)_{\gamma \in \Gamma}$ 標準基底を含むモノイド $\Gamma$ の代数とします。 For every L-linear mapping $u$ of A into L let us write $\tilde{u}(\gamma) = u(e_\gamma)$ (for $\gamma \in \Gamma$); then the mapping $u \mapsto 3$ is an isomorphism of vector L-spaces of $\mathrm{Hom}_L(A, L)$ onto $L^\Gamma$ which maps onto X the set of L-algebra homomorphisms of A into L. ここで、Th を適用するだけで十分です。 1 に $K = L$ が付きます。

#### 系 2 (デデキントの定理) {#alg-v-s6-thm-1-cor-2 .statement tag=06JD}

*E と L を K の 2 つの拡大とする。E の L への K 準同型の集合は L 上で自由である。 E が K 上で有限次数である場合、E の L への K 準同型射の数は、最大でも $[E : K]$ に等しくなります。*

公式 (2) を考慮して、最初から最後の主張が続きます。

### 2. 準同型の代数的独立性

#### 定理 2 {#alg-v-s6-thm-2 .statement tag=06JE}

— K を無限体、K の L 拡大と K 上の A 代数とします。$u_1, \ldots, u_n$ を A から L への別個の K-代数準同型とし、f を $L[X_1, \ldots, X_j]$ の多項式とします。すべての $x \in A$ に対して $f(u_1(x), \ldots, u_n(x)) = 0$ がある場合、$f = 0$ になります。

Let B be the set of elements of $L^n$ of the form $(u_1(x), \ldots, u_n(x))$ with $x \in A$. Thさんより1、すべての $x \in A$ に対して $\sum_{i=1}^n \alpha_i u_i(x) = 0$ となるような、L のすべての零ではなく、元の数列 $(\alpha_1, \ldots, \alpha_n)$ はありません。したがって (II, p. 301, Th. 7) B 生成するベクトル空間 $L^n$ L より。 したがって、行列 $(u_i(a_j))_{1 \leq i,j \leq n}$ が可逆であるような $A$ の元 $a_1, \ldots, a_n$ が存在します。

多項式 $g \in L[Y_1, \ldots, Y_n]$ を定義するとしましょう
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
$y_1, \ldots, y,$ を $K$ に入れます。 $x = \sum_{i=1}^n y_i a_i$ を書いています。
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
よって $g(y_1, \ldots, y_n) = 0$
$f$の仮定までに。 体 $K$ は無限であるため、$g = 0$ (IV, p. 18、Cor. 2) が得られます。今行列 $(u_i(a_j))$ には逆数 $(b_{ij})$ があり、
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
よって $f = 0$。

Th. 2 には、有限体に相当するものはありません。したがって、q 元、$A = L = K$、$f(X) = X^q - X$ を使用して、$K$ を有限体とします。すべての $x \in K$ に対して $x^q = x$ があります (V、p. 93、提案 2)。したがって、$u$ が $K$ の同一性自己同型である場合、すべての $x \in K$ に対して $f(u(x)) = 0$ があり、けれども $f$ は零ではありません。

### 3. 対角可能代数および etale 代数

#### 定義 1 {#alg-v-s6-def-1 .statement tag=06JF}

— A を K より代数とします。このとき、A が積代数 $K^n$ と同型であるような整数 $n \geq 0$ が存在する場合、A は対角化可能であると言われます。スカラーの拡大によって A から導出された L 上の代数 $A_{(L)}$ が対角化可能である場合、A は K の拡大 L によって対角化されると言います。 A を対角化する K の拡大が存在する場合、A はエタールであると言います。

積代数 $K''$ は、次のように定義された積を備えたベクトル空間 $K''$ であることを思い出してください。

$$
(x_1, \ldots, x_n) \cdot (y_1, \ldots, y_n) = (x_1 y_1, \ldots, x_n y_n)
$$

$\varepsilon_1, \ldots, \varepsilon_n$ が $K^n$ の標準基底である場合、次のようになります。

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{if} \quad i \neq j
$$

そして$1 = \varepsilon_1 + \ldots + \varepsilon_n$。

$\mathbf{K}$ 上のすべてのエタール代数は *可換* であり、 $K$ 上の *有限次数* です。

#### 命題 1 {#alg-v-s6-prop-1 .statement tag=06JG}

*A を体 K 以上の有限次数の代数とします。その場合、次の条件は同等です :*
  *a)* *代数 A は対角化可能です。*
  *b)* *$i \neq j$に対して$e_i^2 = e_i$と$e_i e_j = 0$となるようなAの基底$(e_1, \ldots, e_n)$があります。*
  *c)* * A のK-代数準同型を $\mathbf{K}$ 生成するベクトル K 空間 A の双対に変換します。*
  *d)* *すべての A-加群は、部分加群の直和であり、K を 1 上回る次元です。*

The equivalence of *a)* and *b)* follows from Formula (6); on the other hand the n projections $K^n \to K$ are algebra homomorphisms, hence *a)* implies *c)*. *c)* が成り立つ場合、A の代数準同型が A の双対 (*V*, p. 27, Th. 1) の $\mathbf{K}$ 形基底に変換され、それらを $u_1, \ldots, u_n$ で表します。その場合、$a \mapsto (u_i(a))$ は A の同型から代数 $K''$、よって *a)* になります。 したがって、条件 *a)*、*b)*、および *c)* の同値が確立されました。

*b)* が成立し、M を A-加群とします。この場合、比 $e_i$ の相似関係 $(e_i)_M$ は $M$ の射影子であり、$M$ は $e_i M$ の直和であり、これらはサブ A 加群です。したがって、$j \neq i$ に対して $(e_j)_M = 0$ となるような添字 $i$ が存在すると仮定できます。したがって、$M$ のすべてのベクトル部分空間はサブ A モジュール、よって *d)* です。

逆に *d)* が成り立つと仮定して、A-加群 A, を考えます。したがって、$i = 1, \ldots, n$ に対して $Af_i = Kf_i$ となるようなベクトル K 空間 A の基底 $(f_i)$ が存在します。 後で置き換えることそれぞれ $f_i$ を適切なスカラー 倍数で計算し、必要に応じて $1 = f_i + \ldots + f_n$ と仮定することもできます。 $i \neq j$ の場合、$f_i f_j$ 属するから $Af_i \cap Af_j = Kf_i \cap Kf_j$ なので、零になります。現在、$f_i = f_i f_1 + \ldots + f_i f_n = f_i^2$、よって *b)*。

#### 系 {#alg-v-s6-n3-cor-1 .statement tag=06JH}

※LをKの拡大、Aの代数準同型の$\mathscr{H}$集合をLとします。 A が L で対角化されている場合にのみ、等式を持つカード $\mathscr{H} \leq [A : K]$ があります。 A を L で対角化すると、$\mathscr{H}$ はベクトル L-スペース $\mathrm{Hom}_K(A, L)$ の基底になります。*

ベクトル空間 $\mathrm{Hom}_K(A, L)$ over L has 次元 $[A : K]$, by 公式 (2), and $\mathscr{H}$ is a free 部分集合 of $\mathrm{Hom}_K(A, L)$ by Th. 1 (*V*、p. 27)。 We thus have Card $\mathscr{H} \leq [A : K]$ with 等式 if and only if $\mathscr{H}$ is 基底 of $\mathrm{Hom}_K(A, L)$. ベクトル L スペースの同型が存在します。たとえば $\pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^*$ で、$x \in A$ の $u(x) = (\pi u)(1 \otimes x)$ と、集合 $\mathscr{H}_L$ への $\pi$ 写像 $\mathscr{H}$ が特徴です。 L-algebra homomorphisms of $A(\cdot)$ into L.最後に、提案 1 の a) と c) の同値は、L に対して $\mathscr{H}_L$ 生成するベクトル空間 $A_{(L)}^*$ がL に対して代数 $A_{(L)}$ が対角化可能であることを示しています。これで系の証明が完了しました。

#### 命題 2 {#alg-v-s6-prop-2 .statement tag=06JI}

— *A を K 上の代数および K の $\Omega$ 代数閉拡大とします。次の主張は同等です*:

a) *代数 A はエターレ*です。
b) *A*を対角化する有限次数の拡大が存在します。
c) K の *拡大 $\Omega$ は A* を対角化します。

A がエターレであるとします。 $n$ を K 上の A の次数とし、L を A を対角化する K の拡大とし、$\mathscr{H}$ を A の代数準同型の L の集合とします。コルによって。提案 1 に対して、カード $\mathscr{H} = n$ があります。一方、$u \in \mathscr{H}$ ごとに、$[u(A):K] \leq n$ があります。 V、p. 18、木曜日までに。 2、$\mathscr{H}$の元の像によって生成されたLの部分拡張L’は、K上の有限次数です。L’、拡大にはAの$n$の異なる準同型が存在するため、拡大 L' は、Cor によって A を対角化します。これは、a) が b) を意味することを示しています。

K の有限次数のすべての拡大は $\Omega$ (V, p. 20, Th. 1) の部分拡張と同型であるため、b) は c) を意味します。最後に、c) は明らかに a) を意味します。

### 4. エタールの部分代数代数

#### 命題 3 {#alg-v-s6-prop-3 .statement tag=06JJ}

— *A を K 上のエタール代数とする。部分代数の有限数と A のイデアルのみが存在する。さらに、A を対角化する K のすべての拡大は、A のすべての部分代数とすべての商代数も対角化する。特にこれらの代数は etale* です。

代数 $K^n$ は部分代数の有限数とイデアルのみを持ち、$K^n$ の部分代数と商代数は対角化可能であることを示すだけで十分です。 $K^n$ の $(\varepsilon_1, \ldots, \varepsilon_n)$ 標準基底で表します。

A を $K^n$ の部分代数とし、$v_1, \ldots, v_n$ を n 射影 $K^n \to K$ の A に対する制限とします。 $v_i$ の核の共通部分は明らかに 0 であるため、$v_i$ 生成するベクトル K 空間は A (II、p. 302、Cor. 1) に対して二重になります。したがって、K-代数 A は対角化可能です (V, p. 29、提案 1)。

$\{1, 2, \ldots, n\}$ の部分集合 I ごとに $\varepsilon_I = \sum_{i \in I} \varepsilon_i$ を置きます。 元 $\varepsilon_I$ が $K^n$ の冪等であることは明らかです。 I が空の場合に限り、$\varepsilon_I = 0$ があり、$\varepsilon_I \varepsilon_J = \varepsilon_{I \cap J}$ があります。これまで述べてきたように、$K^n$ のすべての部分代数 A は対角化可能です。 条件による提案 1 の b) $K^n$ の部分代数 A ごとに基底 $(\varepsilon_{I_1}, \ldots, \varepsilon_{I_p})$ が認められますが、$(I_1, \ldots, I_p)$ は $\{1, 2, \ldots, n\}$ の分割であり、そのようなものは有限の数だけです部分代数。

$(1, 2, \ldots, n)$ のすべての部分集合 I に対して、$a_i$ を $K^n$ のベクトル部分空間とし、$i \in I$ の冪等$\varepsilon_i$ を基底とします。その場合、$a_i$ が $K^n$ の理想であることは明らかです。さらに、$J = (1, 2, \ldots, n) - I$ の場合、$K^n / a_i$ の $j \in J$ 形基底に対して、$\varepsilon_j$ の $a_i$ を修正する剰余類 $\overline{\varepsilon}_j$ になります。 $j \neq k$ の場合、$\overline{\varepsilon}_j^2 = \overline{\varepsilon}_j$ と $\overline{\varepsilon}_j \overline{\varepsilon}_k = 0$ があるため、V, p. 29 の提案 1 により、代数 $K^n / a_I$ は対角化可能です。

$K^n$ のすべての理想は形 $a_I$ であることを示す必要があります。 I を整数 $i$ の集合として、$1 \leq i \leq n$ と $\varepsilon_i \in a$、その後 $a_i \subset a$ とします。 $x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n$ を $a$ の元 ($K$ に $x_1, \ldots, x_n$ が含まれる) とし、$i$ を $(1, 2, \ldots, n) - I$ に含めます。 $x_i \varepsilon_i = x \varepsilon_i \in a_i$、$\varepsilon_i \notin a$、よって $x_i = 0$があります。したがって、$x = \sum_{i \in I} x_i \varepsilon_i$、そしてこれは$x \in a_i$を示しています。これで$a \subset a_I$、よって、最後に$a = a_i$が表示されました。

#### 系 {#alg-v-s6-n4-cor-1 .statement tag=06JK}

— *$A_1, \ldots, A_r$を$K$と$A = A_1 \times \cdots \times A_r$の上で代数とします。 $A$ がエターレであるためには、$A_1, \ldots, A_r$ がエターレであることが必要かつ十分です。*

$A$ がエターレであると仮定します。それぞれの代数 $A_1, \ldots, A_r$ は $A$ の商と同型であるため、提案 3 によりエタールです。 逆に、 $A_1, \ldots, A_r$ を対角化する $K$ のすべての拡大は明らかに $A$ を対角化します。

### 5. 分離可能な次数/可換代数

$A$ を $K$ 上の有限次数 $n$ の可換代数とします。 $K$ の拡大 $L$ について、$A$ の代数準同型の数 $h(L)$ の $L$ は有限であり、その上は $n$ (V, p. 29, Cor.) によって制限されます。

#### 補題 1 {#alg-v-s6-lem-1 .statement tag=06JL}

— *$\Omega$を$K$の代数閉包とします。その場合、$K$ のすべての拡大 $L$ に対して $h(L) \leq h(\Omega)$ が得られ、$L$ が代数的に閉じているときは等式になります。

$L'$ を $L$ の $K$ の代数閉包とします。 For every homomorphism $u$ of $A$ into $L$ we have $[u(A) : K] \leq n$, hence $u(A) \subset L'$ by V, p. 18, Prop. 2; we thus have $h(L') = h(L)$. $K$ の拡大 $L'$ は $\Omega$ (V, p. 20, Th. 1) の部分拡張と同型であるため、$h(L') \leq h(\Omega)$ が得られます。 $L$ が代数的に閉じている場合、$L'$ は $K$ の代数閉包です。 $K$ の拡大 $L'$ と $\Omega$ は同型 (V、p. 23、Th. 2) なので、$h(L') = h(\Omega)$; 補題はここから直接続きます。

補題 1 までに、数 $h(L)$ は、$K$ のすべての代数閉拡大 $L$ に対して同じ値を持ちます。この数は$[A : K]$で示され、$A$の*分離可能な次数*と呼ばれます。

$A$ と $B$ を $K$ 上の有限次数の 2 つの可換代数とします。 公式を確立します

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

Let $L$ be an algebraically closed extension of $K$ and denote by $\mathscr{H}(A)$ the set of algebra homomorphisms of $A$ into $L$, and similarly define $\mathscr{H}(B)$ and $\mathscr{H}(A \otimes_K B)$. 定義により、カード $\mathscr{H}(A) = [A : K]$ と [B : K] および [A \otimes_K B : K] の対応する式が得られます。 さらに (III, p. 465, 公式 (6))、公式 $(u * v)(a \otimes b) = u(a)v(b)$ 定義する全単射 $\mathscr{H}(A) \times \mathscr{H}(B)$ の $(u, v) \mapsto u * v$ を$\mathscr{H}(A \otimes_K B)$、よって公式 (7) と続きます。

$K'$ を $K$ の拡大とします。 公式を証明しましょう
$$
[A_{(K')}: K'], = [A: K], .
$$
$L$ は $K'$ の代数閉包になります。 公式 $\tilde{u}(x) = u(1 \otimes x)$ ($x \in A$ の場合) 定義する全単射 $u \mapsto \tilde{u}$ $K'$ の集合 - $A_{(K')}$ の $L$ と集合への準同型写像$K$-$A$ の $L$、よってへの準同型写像 (8)。

最後に、$K'$ が $K$ の有限次数の拡大であると仮定します。 $A'$ が有限次数の可換 $K'$-代数である場合、それは有限次数の可換 $K$-代数でもあり、$[A': K] = [A': K'] \cdot [K': K]$ (V. p. 10, Th. 1) が得られます。 We shall prove the formula
$$
[A': K], = [A': K']_s \cdot [K': K], .
$$
For let $S$ (resp. $T$) be the set of $K$-homomorphisms of $K'$ (resp. $A'$) into an algebraic closure $L$ of $K$; for every $\sigma \in S$ we denote by $T_\sigma$ the set of elements $f$ of $T$ such that $f(a \cdot 1) = \sigma(a)$ for all $a \in K'$. 次に、家族 $(T_\sigma)_\sigma$ は $T$ の分割であり、カード $S = [K': K]$ があります。さて、それぞれの $\sigma \in S$ 集合 $T_\sigma$ は、$A'$ の $K'$ の代数閉拡大 $(L, \sigma)$ への $K'$ 準同型写像で構成されているため、カード $T_\sigma = [A': K']_s$ が証明され、(9) が証明されました。

#### 命題 4 {#alg-v-s6-prop-4 .statement tag=06JM}

— $A$ を $K$ 上の有限次数の可換代数とします。 $A$ がエターレの場合に限り、$[A: K], \leq [A: K]$ と等式が結合します。

Let $\Omega$ be an algebraic closure of $K$ and $A?$ the set of algebra homomorphisms of $A$ into $\mathbf{R}$. カード $A? = [A: K]$ があり、$A$ が $K$ の拡大 $\Omega$ によって対角化された場合に限り、$A$ はエタールになります (V、p. 30、提案 2)。 したがって、提案 4 は Cor. V、p. 29の。

#### 系 1 {#alg-v-s6-prop-4-cor-1 .statement tag=06JN}

— $A, B$ を、有限非ゼロ次数の $K$ 上の 2 つの可換代数とします。次に、代数 $C = A \otimes_K B$ がエターレであるためには、$A$ と $B$ がエターレであることが必要かつ十分です。

分離可能な次数には $[C: K] = [A: K] \cdot [B: K]$ と対応する公式 (7) があります。さらに、$B$ と $C$ に対する$[A: K], \leq [A: K]$ と対応するの式があります。したがって、$[A: K] = [A: K]$ と $[B: K] = [B: K]$ の両方がある場合に限り、$[C: K] = [C: K]$ になります。ここで、提案 4 を適用するだけで十分です。

#### 系 2 {#alg-v-s6-prop-4-cor-2 .statement tag=06JO}

— $K'$ を $K$ の拡大とします。

a) $K$-代数 $A$ がエタールであるためには、$K'$-代数 $A_{(K')}$ がエタールであることが必要かつ十分である。

b) $A'$ を 0 に減らさずに、$K'$ を超える代数とする。 $A'$ が $K$ を超えるためには、 $A'$ が $K'$ を超え、$K'$ が $K$ を超えることが必要かつ十分である。

私たちはコルについて議論します。 1、適用今回は、a) の場合は (8)、b) の場合は (9) です。

### 6. エターレ代数の差動特徴付け

#### 定理 3 {#alg-v-s6-thm-3 .statement tag=06JP}

— $A$ を $K$ 上の有限次数の可換代数とします。 $A$ がエターレであるためには、$A$ の $K$ 差分のうち加群 $\Omega_K(A)$ が $0$ に減少することが必要かつ十分です。

A) $L$ を $K$ の代数閉包とします ($V$、p. 23、Th. 2)。 $A$ がエターレであるためには、$L$ 上の代数 $A_{(L)}$ が対角化可能であることが必要かつ十分です ($V$, p. 30、提案 2)。さらに、$A$加群$\Omega_L(A_{(L)})$は$\Omega_K(A) \otimes_A A_{(L)}$ (III、p. 572、提案20)と同型であるため、テンソル積の結合性により$\Omega_K(A) \otimes_K L$となります。したがって、$\Omega_K(A) = 0$ は $\Omega_L(A_{(L)}) = 0$ と同等です。 Thを証明するには。したがって、$K$ が代数的に閉じている場合を考慮し、$\Omega_K(A) = 0$ の場合に限り、代数 $A$ が対角化可能であることを示すだけで十分です。

B) $A$ が対角化可能であると仮定します。 ($V$, p. 29, 提案 1)、ベクトル空間 $A$ は $A$ の冪等によって生成されます。したがって、主張 $\Omega_K(A) = 0$ は、次の補題の帰結です。

#### 補題 2 {#alg-v-s6-lem-2 .statement tag=06JQ}

$A$ を $K$ 上の可換代数とし、$e$ を $A$ の冪等とします。そうすると、$\Omega_K(A)$には$de = 0$が入ります。

関係 $e = e^2$ から $de = 2e \cdot de$ を導き出します。 $e$を掛けると$e \cdot de = 2e \cdot de$、したがって$e \cdot de = 0$、そして最終的には$de = 2e \cdot de = 0$になります。

C) まず 2 つの補題を証明します。

#### 補題 3 {#alg-v-s6-lem-3 .statement tag=06JR}

$A$ を有限次数の代数閉体 $K$ の可換代数として、$\Omega_K(A) = 0$ とします。すると、$A$ の最大理想値 $m$ ごとに $m = m^2$ が得られます。

代数 $A/m$ は、代数閉体 $K$、よって $[A/m : K] = 1$ の有限次数の拡大です。したがって、各 $a \in A$ には、$a - \lambda \cdot 1 \in m$ のような固有のスカラー $\lambda$ が存在します。 $a - \lambda \cdot 1$ mod $m^2$ の剰余類に $D(a)$ と書きます。 $D$ が $A$ の $A$ モジュール $m/m^2$ への $K$ 導出であることは明らかです。 $\Omega_K(A)$ (III、p. 569) および仮定 $\Omega_K(A) = 0$ の普遍性は、$D = 0$、よって $m/m^2 = 0$、そして $m = m^2$ を意味します。

#### 補題 4 {#alg-v-s6-lem-4 .statement tag=06JS}

$A$ を可換環とし、$a$ を $a = a^2$ となるような $A$ の有限生成理想とする。次に、$a = Ae$ のような冪等な $e$ が $A$ に存在します。

$(a_1, ..., a_r)$ を理想 $a$ の生成する系とします。 $a = a^2$ 以降、$a$ には $1 \leq i \leq r$ に対して $a_i = \sum_{j=1}^r x_{ij} a_j$ が存在するように、元 $x_{ij}$ が存在します。 元が$\delta_{ij} - x_{ij}$である位数$r$の平方行列を$M$と書き、$D$をその行列式とします。 $A$ に元が入った位数 $r$ の (III, p. 532, 公式 (26)) 平方行列 $N$ が存在し、$N \cdot M = D \cdot I$、 よってすぐに $Da_j = 0$ が $1 \leq j \leq r$ になり、最終的に $Da = 0$ になります。ここで、行列 $M$ は $I$、mod $a$ と合同なので、$D \equiv I$ mod $a$ となります。 $e = 1 - D$を入れてください。次に、すべての $x \in a$ に対して $e \in a$ と $ex = x$ が続きます。したがって、$e$ は冪等であり、$a$ は $Ae$ に等しいことがわかります。

これらの補題が確立されたので、$K$ が代数的に閉じていて $\Omega_K(A) = 0$ である場合、$A$ の次数上の帰納法によって、$A$ が対角化可能であることを示しましょう。 $m$ を $A$ (I, p. 104) の最大理想とする。 補題 3 と 4 により、$m = Ae$ となる冪等 $e$ が存在します。 $A/m$ は $K$ に対して次数 1 であることがわかりました。したがって、$A$ は理想$a = (1 - e)A$ と $m$ の直和であり、$[a : K] = 1$ があるため、$A$ は$K \times A/a$ と同型です。 $\Omega_K(A/a)$ は $\Omega_K(A)$ の商と同型であるため (III、p. 573、提案 22)、零であり、帰納法の仮定は $A/a$ が対角化可能であることを示しています。これにより、$A$ が対角化可能であることがわかります。

### 7. 削減代数とエターレ代数

#### 定義 2 {#alg-v-s6-def-2 .statement tag=06JT}

— *$A$を可換環とします。このとき、$A$ のすべての冪零元 (I, p. 98) が零である場合、$A$ は減らされると言われます。*

$A$ が減算された環の体、または整域、または積の場合、減算された環です。 可換環 $A$ を減らすには、$A$ のすべての $a \neq 0$ に対して $a^2 \neq 0$ が必要かつ十分です。これにより、$n$、$a^{2^n} \neq 0$ の帰納法によって得られるため、$a \neq 0$ のすべての$a^n \neq 0$ が得られます。 $A$。

代数は、その基礎となる環が削減される場合、*削減される*と言われます。

#### 命題 5 {#alg-v-s6-prop-5 .statement tag=06JU}

— *$A$ を $K$ 上の有限次数の可換代数とします。 For $A$ to be reduced it is necessary and sufficient that there exist extensions $L_1, \ldots, L_s$ of finite degree over $K$ such that $A$ is $K$-isomorphic to $L_1 \times \cdots \times L_s$.*

記載されている条件で十分であることは明らかです。

逆に、$A$ が減少すると仮定します。 $A$の次数に対する帰納法による議論により、$A$が体ではない場合、2つの非ゼロ代数$A_1$と$A_2$が存在し、$A$が$A_1 \times A_2$、または $A$ には 0 と 1 とは異なる冪等が存在します。

これから$A$が減って体ではなくなったとします。 0 と $A$ とは異なる $A$ の理想のうち、$a$ をベクトル $K$ として次元の空間が最小である理想とする。 $a$ の任意の $x \neq 0$ については、$A$ が減らされ、よって $a' \neq \{0\}$ になるため、$x^2 \neq 0$ になります。 $a^2 \subset a$ があり、$a$ の最小性によって $a' = a$ がわかります。 補題 4 までに、$a = Ae$ のような冪等な $e$ が存在し、$a$ は 0 および $A$ とは異なるため、$e \neq 0, e \neq 1$ が得られます。

#### 定理 4 {#alg-v-s6-thm-4 .statement tag=06JV}

— *$A$ を $K$ 上の有限次数の可換代数とします。したがって、次の主張は同等です。
a) 代数 $A$ はエターレです。
b) $K$ の拡大 $L$ ごとに、環 $L \otimes_K A$ が減らされます。
c) 環 $P \otimes_K A$ が減算されるような、$K$ の完全な拡大体 $P$ が存在します。
d) $A$ が $L_1 \times \cdots \times L_s$ と同型となるような可分代数拡大 $L_1, \ldots, L_s$ の $K$ が存在します。
特にエターレ代数が全て減額されます。

A) まず、$a$、$b$、$c$ の同値を証明しましょう。

$A$ がエターレで、$L$ が $K$ の拡大であるとします。 $\Omega$ を $L$ の代数閉拡大体とします (V、p. 23、Th. 2)。この場合、$L \otimes_K A$ は$\Omega \otimes_K A$ の部分環と同型であり、後者は提案 2 (V, p. 30) により環 $\Omega^n$ と同型です。したがって、環 $L \otimes_K A$ は減少します。

したがって、a) は b) を意味し、c) は b) の特殊なケースであることを示しました。ここで、c) が成り立つと仮定します。 K-代数 $A$ がエタールであるためには、P 代数 $A_{(P)}$ がエタールであることが必要かつ十分です (V, p. 32, Cor. 2)。したがって、代数 $A$ は、次の補題によってエターレとなります。

#### 補題 5 {#alg-v-s6-lem-5 .statement tag=06JW}

*B を完全体 P に対する有限次数の縮小代数とします。その場合、B はエターレです。*

提案 5 により、$B$ が代数 $L, x \ldots x L_n$ と同型となるような $P$ の拡大 $L_1, \ldots, L_n$ が存在します。 etale 代数の有限積は etale (V, p. 31, Cor.) なので、$B$ が $P$ の拡大である場合を調べるだけで十分です。 Thさんより3 (V、p. 33) すべての $x \in B$ について、$\Omega_P(B)$ に $dx = 0$ があることを示すだけで十分です。

$x \in B$ にしましょう。 $B$ は $K$ に対する有限次数であるため、$x$ は $K$ に対する代数的です (V, p. 18、提案 2)。 $f$ を $x$ の最小多項式とし、$f'$ を導関数とします。多項式 $f$ は非定数です。 $f' = 0$; と仮定します。 V、p. 9、Cor. 体 $P$ は $p \neq 0$ の特性を持ち、$f \in P[X^p]$ があります。 $P$ は完全なので、$P[X^p] = P[X]^p$ になりますが、既約多項式 $f$ できないは $P[X]^p$ にあります。

したがって、$f' \neq 0$ があり、$f'$ の次数は厳密にそれより小さいため、$f'(x) \neq 0$ になります。さて、示さなければならなかったように、$f(x) = 0$ から$\Omega_P(B)$、よって $dx = 0$ で $f(x) \cdot dx = 0$ を導き出します。

*B) $A$ がエターレであると仮定します。 a) と b) の同値により代数 $A$ が縮約されるため、$A$ が $L_1 \times \cdots \times L_n$ と同型となるような $K$ の拡大 $L_1, \ldots, L_n$ が存在します (提案 5)。 $A$ はエタールであるため、拡大 $L_i$ のそれぞれはエタール代数 (V, p. 31, Cor.) であり、したがって定義により $K$ の分離可能な代数拡大になります。

$d) \Rightarrow a)$ の含意は、V、p. 31、Cor から続きます。 \*

#### 系 {#alg-v-s6-n7-cor-1 .statement tag=06JX}

— *$K$が特性$p \neq 0$を持っているとします。 $A$ がエターレであるためには、$A = K[A^p]$ であることが必要かつ十分です。 $K$ を超える $A$ の基底 $(a_i)_i$ ごとに、家族 $(a_i^p)_i$ は $K$ を超える $A$ の基底になります。*

$K$ の選ぶ代数閉包 $\Omega$ としましょう。 $A$ の 2 つの $K$ 準同型 $u$ と $v$ を $\Omega$ に変換すると、$u$ と $v$ が同じ制限 ～ $K[A^p]$ を持つ場合、次のようになります。

$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p,
$$

よって $u(x) = v(x)$

$x \in A$の皆さんへ。したがって、不等式 $[A : K], \leq [K[A^p] : K]_s$ となります。 $A$ が etale である場合、次のようになります。

$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$

よって $A = K[A^p]$

逆に、$A = K[A^p]$があると仮定します。 $(a_i)_{i \in I}$ を $K$ 上の $A$ の基底とします。 $V$、p. 4、提案 2、b) により、ファミリー $(a_i^p)_{i \in I}$ 生成するベクトル $K$-空間 $K[A^p]$ と、$A = K[A^p]$ は有限次元の $I$ の基数に等しいので、家族 $(a_i^p)_{i \in I}$ は $K$ 上の $A$ の基底です。 $u$ を $\Omega \otimes_K A$ の元として、$u^2 = 0$、よって $u^p = 0$ とします。 $(a_i)_{i \in I}$ は $K$ 上の $A$ の基底であるため、$u = \sum_{i \in I} \lambda_i \otimes a_i$、よって $u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p$ のような $\Omega$ の元の家族 $(\lambda_i)_{i \in I}$ が存在します。 $(a_i^p)_{i \in I}$ は $K$ と $u^p = 0$ を超えた $A$ の基底であるため、すべての $i \in I$ に対して $\lambda_i^p = 0$、よって $\lambda_i = 0$ が必要になり、したがって $u = 0$ になります。これは、環 $\Omega \otimes_K A$ が削減されることを示しています。 $\Omega$ は完全なので、$K$ を超える代数 $A$ は Th によるエターレです。 4.

etale 代数の他の特徴付けについては、$V$、p. 48、提案 1 を参照してください。

### 練習問題 {#alg-v-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
