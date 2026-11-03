---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 1
section_title: Finitely generated graded algebras
lang: ja
source: ac-i-vii
book_pages: 155-162, 232-233
pdf_pages: 0175-0182, 0252-0253
extraction: ocr
subsections:
    - "no": 1
      title: SYSTEMS OF GENERATORS OF A COMMUTATIVE ALGEBRA
      page: 155
      pdf_page: 175
    - "no": 2
      title: Criteria of Finiteness for Graded Rings
      page: 156
      pdf_page: 176
    - "no": 3
      title: PROPERTIES OF THE RING $A^{(d)}$
      page: 157
      pdf_page: 177
    - "no": 4
      title: GRADED PRIME IDEALS
      page: 160
      pdf_page: 180
statements: 13
exercises: 3
content_sha256: e5cc428171c5c7c1e56db82a31e595bcb38acfa23ca452012ad4424155d1ba61
translated_from: content/en/ac/III/01_s1_finitely_generated_graded_algebras.md
translation_method: google
source_content_sha256: 4ef8d10c43b0b3fc4352b08bd49dd75b1412e18ba3d610df64784225920b10c7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2b58afaf8e46f4dbb7430f42617654d9c54dc07b96dcd92386c243005a59bf1b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 有限生成されたグレーディング代数

### 1. 系/生成元/可換代数

$\mathbf{A}$ を可換環 、$\mathbf{B}$ を可換$\mathbf{A}$-代数とする。 (代数, 章 IV, § 2, no. 1) $x = (x_i)_{i \in I}$ が $\mathbf{B}$ の元の族である場合、多項式代数 $\mathbf{A}[X_i]_{i \in I}$ から $\mathbf{B}$ の写像 $f \mapsto f(x)$ は次のようになります。 $\mathbf{A}[X_i]_{i \in I}$ の準同型を $\mathbf{B}$ の部分代数に、$x_i$ によって生成されます。その核 $a$ は、$f(x) = 0$ となるような多項式 $f$ であり、代数の *イデアルと呼ばれます。 $x_i$* の間には関係 ($\mathbf{A}$ には係数が入ります)。

#### 定義 1 {#ac-iii-s1-def-1 .statement tag=04D1}

* 可換環 $\mathbf{A}$ 上の可換代数 $\mathbf{B}$ において、$\mathbf{B}$ の元の族 $(x_i)_{i \in I}$ は、$\mathbf{A}$ 上で代数的に自由と呼ばれます (または、$x_i$ は $\mathbf{A}$ 上で代数的に独立と呼ばれます)。 $\mathbf{A}$ に係数がある、$x_i$ 間の代数関係は 0 に減らされます。 $\mathbf{A}$ 上で代数的に自由でない族 $(x_i)$ は、代数的に関連しているとも呼ばれます (またはその元は、代数的に依存しているとも呼ばれます) $\mathbf{A}$).*

この定義は、可換体の元の家族に対して代数、章 V, § 5, no. 1、定義 1 で与えられたものを一般化します。

(*) 章 I, § 4 の結果を使用し、したがって相同的である代数を使用する § 5 を除き、この本の I ～ VI と章 I および II 以外の本のこの章では使用されません。

族 $(x_i)_{i \in I}$ が $A$ 上で代数的に自由であると言うのは、$x$ の単項式 $\prod_i x_i^{n_i}$ が $A$ 上で *一次独立* であるというというと同じになります。特に、$x_i$ は $A$ に対して線形独立です。

#### 定義 2 {#ac-iii-s1-def-2 .statement tag=04D2}

*可換代数* $B$ *over 可換環* $A$ *それが元の有限族によって生成される場合、有限生成と呼ばれます。*

$B$ が形 $A[X_1, \ldots, X_n]/a$ の $A$-代数と同型であると言うのは同じことになります (ここで、$X_i$ は不定であり、$a$ は多項式環 $A[X_1, \ldots, X_n]$ のイデアルです)。

$A$-代数 $B$ が *有限生成された $A$-加群* である場合、それは明らかに有限生成された $A$-代数です。多項式代数の例が示すように、逆は偽です(cf.章V)。

$B$ が有限生成された $A$-代数であり、$A'$ が任意の可換 $A$-代数である場合、$(x_i)_{i \in I}$ が $A$-代数の生成系である場合、$B_{(A')} = B \otimes_A A'$ は有限生成された $A'$-代数です。 $B$ は明らかに、$x, \otimes 1$ が $A$-代数 $B_{(A')}$ の生成系を形成しています。

$B$ が有限生成された $A$-代数、$C$ が有限生成された $B$-代数である場合、$C$ は有限生成された $A$-代数です。なぜなら、$(b_\lambda)_{\lambda \in L}$ が $A$-代数 $B$ の生成元の系であり、$(c_\mu)_{\mu \in M}$ が $B$-代数 の生成元の系である場合、定義からすぐに導かれるからです。 $C$、$C$ のすべての元は多項式に等しく、$A$、$b_\lambda$、$c_\mu$ では係数となります。

### 2. 等級付けの有限性の基準環

※このNo.以下では、考慮されるすべての卒業 (代数、章 II, § 11) は型* $\mathbf{Z}$ であると仮定されます。 *場合* $A$ *(それぞれM)* *が等級環* (それぞれ *等級加群*)、$A_i$ (それぞれ$M_i$) *次数の元の集合を表します* $i$ *in* $A$ *(それぞれM)*。

*もし* $A_i = \{0\}$ *(それぞれ$M_i = \{0\}$) for* $i < 0$, $A$ *(それぞれM)* *略して、グレード付き環* (それぞれ*加群*) *プラスの次数*と呼ばれます。

#### 命題 1 {#ac-iii-s1-prop-1 .statement tag=04D3}

*$A = \bigoplus_{i \in \mathbf{Z}} A_i$ *を正の次数を持つ段階的可換環とし、mを段階的理想* $\bigoplus_{i \geq 1} A_i$ *および* $(x_\lambda)_{\lambda \in L}$ *同種元の* $A$ *次数* $\geq 1$とする。 *以下の条件は同等です*:

(a) *理想* $A$ *家族によって生成* $(x_\lambda)$ *は$m$と等しい*。

(b) *家族* $(x_\lambda)$ * は* $A$*-代数* $A$ の生成元の系です。

(c) *すべて* $i \geq 0$ について、* $A$* モジュール* $A_i$ *は、次数* $i$ *in* $A$ の形* $\prod_\lambda x_\lambda^{n_\lambda}$ の元によって生成されます。

明らかに、条件 (b) と (c) は同等です。それらが成り立つ場合、m のすべての元は形 $f((x_i))$ になります。ここで、$f$ は定数項を持たない $A_0[X_\lambda]_{\lambda \in L}$ の多項式です。次に $m = \sum_{\lambda \in L} A x_\lambda$ ですが、これは (c) が (a) を意味していることを証明します。逆に、条件 (a) が成り立つとします。 $A' = A_0[x_\lambda]_{\lambda \in L}$ を族 $(x_\lambda)$ によって生成された A の部分 A,-代数とし、それを $A' = A$ で示しましょう。このためには、すべての $i \geq 0$ に対して $A_i \subset A$ を示すだけで十分です。 $i$ では帰納法まで進み、$i = 0$ では性質が明らかです。次に、$y \in A$を$i \geq 1$とします。 $y \in m$ 以降、$y = \sum_\lambda a_\lambda x_\lambda$ となるような有限台の A の元の族 $(a_\lambda)_{\lambda \in L}$ が存在し、$a_\lambda$ のそれぞれは次数 $i - \deg(x_\lambda)$ と同次であると仮定できます (必要に応じて置き換えることによって)均質な成分のうち次数)。 $\deg(x_\lambda) > 0$、帰納法の仮定は、すべての $\lambda \in L$、よって $y \in A'$、$A_i \subset A'$ に対して $a_\lambda \in A'$ であることを示しており、これは (a) が (b) を意味していることを証明します。

#### 系 {#ac-iii-s1-n2-cor-1 .statement tag=04D4}

*$A = \bigoplus_{i \in \mathbf{Z}} A_i$ を、ポジティブな次数* と $m$ *段階的な理想*、$\bigoplus_{i \geq 1} A_i$ を持つ段階的な可換環とします。

(i) *以下の条件は同等です*:
(a) *理想* $m$ *は有限生成A-加群* です。
(b) *環* $A$ *は有限生成された A,-module* です。

(ii) *(i) の条件が成立すると仮定し、* $M = \bigoplus_{i \in \mathbf{Z}} M_i$ * を有限生成された等級付けされた A-加群とします。次に、すべて* $i \in \mathbf{Z}$ に対して、$M_i$ *は有限 A,-加群であり、*$i < i_0$ に対して* $M_i = \{0\}$ * となる* $i_0$ が存在します。

(i) A の元の族 $(y_\mu)$ が A-加群 m (それぞれ A、モジュール A) の生成元の系である場合、$y_\mu$ の同種成分の族からなるも同様です。 条件 (a) および (b) の同値は、命題 1 から続きます。

(ii) A は次数 $> 1$ の同次元 $a_i$ ($1 < i < r$) によって (A,-代数として) 生成され、M は同次元 $x_j$ によって (A-加群として) 生成されると仮定できます。 ($1 < j < s$); $h_i = \deg(a_i), k_j = \deg(x_j)$ にしましょう。明らかに M は、元 $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_r^{\alpha_r} x_j$ の $A_0$ に係数を含む線形結合で構成され、$\alpha_i$ は整数 $\geq 0$ 満たす関係 $k_j + \sum_{i=1}^r \alpha_i h_i = n$ になります。すべての $i$ については $h_i \geq 1$ なので、それぞれの $n$ に対して、家族 $(\alpha_i)_{1 \leq i \leq r}$ 満たすこれらの条件は有限の数だけです。 結論するは、$M_n$ が有限生成された A,-加群であること、さらに、$n < \inf(k_j)$ のときは明らかに $M_n = \{0\}$ であることがわかります。

### 3. 環 $A^{(d)}$ の特性

$A = \bigoplus_{i \in \mathbf{Z}} A_i$ をグレード環とし、$M = \bigoplus_{i \in \mathbf{Z}} M_i$ をグレード A-加群とします。 整数 $(d, k)$ のうち、$d \geqslant 1$ と $0 \leqslant k \leqslant d - 1$、集合のすべての注文対について

$$
A^{(d)} = \bigoplus_{i \in \mathbf{Z}} A_{id}, \quad M^{(d, k)} = \bigoplus_{i \in \mathbf{Z}} M_{id + k}.
$$

明らかに、$A^{(d)}$ は $A$ のグレード付けされた部分環であり、$M^{(d, k)}$ はグレード付けされた $A^{(d)}$ モジュールです。さらに、$N$ が $M$ の等級付けされた部分加群である場合、$N^{(d, k)}$ は $M^{(d, k)}$ の等級付けされたサブ$A^{(d)}$ モジュールです。 $M^{(d, 0)}$ の代わりに $M^{(d)}$ と書きます。各 $d \geqslant 1$、$M$ は、$A^{(d)}$ モジュール $M^{(d, k)}$ $(0 \leqslant k \leqslant d - 1)$ の直和です。

#### 命題 2 {#ac-iii-s1-prop-2 .statement tag=04D5}

*$A = \bigoplus_{i \in \mathbf{Z}} A_i$ をポジティブな次数を持つグレード付き可換環とし、$M = \bigoplus_{i \in \mathbf{Z}} M_i$ をグレード付き $A$ モジュールとします。 $A$ が有限生成された $A_0$-代数であり、$M$ が有限生成された $A$-加群であると仮定します。次に、整数の注文されたすべての対 $(d, k)$ について、$d \geqslant 1, 0 \leqslant k \leqslant d - 1$ は次のようになります:*

(i) $A^{(d)}$ は有限生成された $A$ モジュールです。
(ii) $M^{(d, k)}$ は有限生成された $A^{(d)}$ モジュールです。

$A$ が *有限生成された $A^{(d)}$*-*加群* であることを示しましょう。 $(a_i)_{1 \leqslant i \leqslant s}$ を同次元の $A$-代数 $A$ からなるの生成元の系とします。 $1 \leqslant i \leqslant s$ の $0 \leqslant \alpha_i \leqslant d$ が $A^{(d)}$ モジュール $A$ の生成元の系を構成するように、形 $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_s^{\alpha_s}$ の $A$ の元 (数で有限)。 整数 $n_i \geqslant 0$ $(1 \leqslant i \leqslant s)$ のすべての系には、$r_i < d$ $(1 \leqslant i \leqslant s)$ である $n_i = q_i d + r_i$ などの正の整数 $q_i, r_i$ があります。それから

$$
a_1^{n_1} a_2^{n_2} \ldots a_s^{n_s} = (a_1 \ldots a_s^{q_s})^d (a_1^{r_1} \ldots a_s^{r_s})
$$

これは、すべての同種の元 $x \in A$ が $x^d \in A^{(d)}$ を満たすため、私たちの主張を証明します。次に、$M$ が有限生成された $A$ モジュールである場合、それは有限生成された $A^{(d)}$ モジュールでもあります。 $M$ は $M^{(d, k)}$ $(0 < k < d - 1)$ の *直接* 和であるため、各 $M^{(d, k)}$ は有限生成された $A^{(d)}$ モジュールであり、これは (ii) を証明します。

上記を、no. 2 の系から命題 1 によって有限生成される段階的$A$ モジュール $m = \bigoplus_{i \geqslant 1} A_i$ に適用してみましょう。 $m^{(d)}$ は有限生成された $A^{(d)}$ モジュールであることがわかります。したがって (no. 2, 系から命題 1) $A^{(d)}$ は有限生成された $A$-代数です。

#### 補題 1 {#ac-iii-s1-lem-1 .statement tag=04D6}

*$A$ を、$A = A_0[A_1]$、$M$ が段階的な $A$ モジュール、$(y_\lambda)_{\lambda \in L}$ がすべての $\lambda \in L$ に対して $\deg(y_\lambda) \leqslant n_0$ となるような $M$ の同種生成器の系であるとする。 次に、すべての $n \geqslant n_0$ とすべての $k \geqslant 0$、$M_{n+k} = A_k \cdot M_n$ について*

$n \geqslant n_0$ と $x \in M_n$ としましょう。 $y_\lambda$ 生成する $M$ から、$x = \sum_\lambda a_\lambda y_\lambda$ のような元の $A$ 有限台の家族 $(a_\lambda)_{\lambda \in L}$ が存在します。さらに、それぞれの $a_\lambda$ は同種であり、 次数 $n + 1 - \deg(y_\lambda)$ の同種であると仮定することもできます (置き換えることは、必要に応じて、その次数の同種の成分によって決まります)。として

$A = A_0[A_1]$ と $\deg(a_\lambda) > 0$、それぞれの $a_\lambda$ は、$b \in A_0, b' \in A$、よって $x \in A_1 M_n$ の元の形 $bb'$ の和です。その後、$k$の帰納法までに$M_{n+1} = A_1 M_n$、よって、$M_{n+k} = A_k M_n$となります。

#### 補題 2 {#ac-iii-s1-lem-2 .statement tag=04D7}

*$A$ を、$A = A_0[A_1]$ のような段階的可換環とし、$S = \bigoplus_{i \geq 0} S_i$ を、有限生成された $A$ 加群である正の次数を持つ段階的可換 $A$ 代数とする。次に、次のような整数 $n_0 \geq 0$ が存在します:*

(i) *$n \geq n_0$、$k \geq 0$、$S_{n+k} = S_k \cdot S_n$の場合。*
(ii) *$d \geq n_0$、$S^{(d)} = S_0[S_d]$の場合。*

補題 1 までに整数 $n_0 \geq 0$ が存在し、$n \geq n_0$ と $k \geq 0$、$S_{n+k} = A_k S_n$、よって *なおさら* $S_{n+k} = S_k S_n$ が成立し、(i) が成立します。次に、$d \geq n_0$と$m > 0$については、$m$適用(i)の帰納法により以下のように$S_{m d} = (S_d)^m$となります。これにより (ii) が確立されます。

#### 命題 3 {#ac-iii-s1-prop-3 .statement tag=04D8}

*$R = \bigoplus_{i \geq 0} R_i$ を、有限生成された $R_0$-代数である正の次数を持つ等級付けされた可換環とします。すべての $m \geq 1$ に対して $R^{(me)} = R_0[R_{me}]$ となるような整数 $e \geq 1$ が存在します。*

$(x_j)_{1 \leq j \leq s}$ を $R_0$-代数 $R$ の同次生成元の系とし、その次数は $\geq 1$ です。 $h_j = \deg(x_j)$、$q$を$h_j$の共通の倍数とし、$1 \leq j \leq s$を$q_j = q/h_j$と書きます。 元 $x_j^{q_j}$ は、次数 $q$ のすべてになります。 $B$ を、$x_j^{q_j}$ によって生成された $R$ の部分$R_0$ 代数とします。 $i$が$q$の倍数でない場合は、$R$の部分代数、および$B_i = 0$となります。 $A$ (それぞれ $S$) を等級付けされた環とし、その基礎となる環は $B$ (それぞれ $R^{(q)}$) であり、その卒業は $A_i = B_{iq}$ (それぞれ $S_i = R_{iq}$) で構成されます。次に、$B$の定義による$A = A_0[A_1]$。 形 $x_1^{\alpha_1} x_2^{\alpha_2} \ldots x_s^{\alpha_s}$ の $R$ (数で有限) の元を考えてみましょう。ここで、$0 \leq \alpha_j \leq q_j$ と $\alpha_1 h_1 + \ldots + \alpha_s h_s \equiv 0$ (修正 $q$) です。それらが生成する $B$ モジュール $R^{(q)}$ であることを示しましょう。 形 $x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s}$ の $R^{(q)}$ のすべての元が上記の元の $B$ 線形結合であることを証明すれば十分です。さて、$r_j < q_j$ ($1 \leq j \leq s$) である $n_j = k_j q_j + r_j$ のような正の整数 $k_j, r_j$ が存在します。それから

$$
x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s} = (x_1^{q_1})^{k_1} \ldots (x_s^{q_s})^{k_s} \cdot (x_1^{r_1} \ldots x_s^{r_s})
$$

そして仮定 $\sum_{j=1}^s n_j h_j \equiv 0$ (修正 $q$) により、したがって $\sum_{j=1}^s r_j h_j \equiv 0$ (修正 $q$)。 定義による$x_j^{q_j}$ 属するから $B$ のように、これは私たちの主張を証明します。 $S$ は有限生成された $A$ モジュールであるため、補題 2 が適用できます。$d > n_0$ に対しては $S^{(d)} = S_0[S_d]$、したがって $d \geq n_0$ に対しては $R^{(qd)} = R_0[R_{qd}]$ となるような $n_0$ が存在します。 命題に $e = q n_0$ が続きます。

### 4. 段階的なプライム理想

$A = \bigoplus_{i \geq 0} A_i$ を *正* 次数で等級付けされた可換環とし、$m$ を等級付けされた理想 $\bigoplus_{i \geq 1} A_i$ とします。 $n \geq n_0$ に対して $a_n = b_n$ となるような整数 $n_0$ が存在する場合、$A$ の 2 つの段階的な理想 $a = \bigoplus_{i \geq 0} a_i, b = \bigoplus_{i \geq 0} b_i$ を *同等* と呼びます (明らかに同値関係です)。段階的な理想は、$m$ に相当しない場合、*必須* と呼ばれます。

#### 命題 4 {#ac-iii-s1-prop-4 .statement tag=04D9}

*$p = \bigoplus_{i \geq 0} p_i$を$A$の段階的な理想とします。 $p$ が素数であるためには、$x \in A, \ y \in A,$ 満たす $x \notin p$ および $y \notin p,$ の場合、$xy \notin p$ であることが必要かつ十分です。*

条件は明らかに必要です。逆に、それが満たされる場合、2 つの同種元 $\neq 0$ の等級付けされた環 $A/p = \bigoplus_{i \geq 0} A_i/p_i$ 積は $\neq 0$ であるため、$A/p$ は整域 (*代数*, 章) II, § 11, no. 4、命題 7)。

#### 命題 5 {#ac-iii-s1-prop-5 .statement tag=04DA}

*$a = \bigoplus_{i \geq 0} a_i$を$A$と$n_0$整数$> 0$の段階的な理想とします。 $n \geq n_0,$ に対して $p_{n_0} = a,$ となるような段階素数理想 $p = \bigoplus_{i \geq 0} p_i$ が存在するには、同次の対に対して元 $x, y$ 次数 $\geq n_0,$ 関係 $xy \in a$ が必要かつ十分です。 「$x \in a$ または $y \in a$」を意味します。 $a_n \neq A_n,$ が素イデアル満たすとなるような $n \geq n_0$ が存在する場合、上記の条件は一意です。*

主張の条件は明らかに必要です。すべての $n \geq n_0,$ に対して $a_n = A_n$ である場合、明らかにすべての素数理想含む $m$ は解 ～ 問題です。したがって、問題を解決するいくつかの主要なイデアルが存在する可能性があります。ただし、これらの理想のうち 2 つは明らかに同等です。次に、所属 ～ $a_d$ ではなく、同種の元 $a \in A_d$ ($d \geq n_0$ を伴う) が存在すると仮定します。 $p$ を $x \in A$ の集合として、$ax \in a$ とします。明らかに、$p$ は $A$ の理想です。 $ax$ の同次成分は、$x$ の$a$ による積であり、$a$ は段階的理想であり、$p$ は段階的理想です。さらに、$1 \notin p$ なので $p \neq A$ となります。 $p$ が素数であることを証明するには、$x \in A, \ y \in A,$ 満たす $x \notin p$ および $y \notin p,$ である場合、$xy \notin p$ (命題 4) であることを示すだけで十分です。次に、$ax \notin a_{m+d}, ay \notin a_{n+d},$ よって by 仮定

$$
a^2xy \notin a_{m+n+2d};
$$

私たちは$xy \notin p$以来$axy \notin a_{m+n+d}$を結論するとしています。 最後に、$n \geq n_0$ と $x \in A_n,$ 条件 $x \in a,$ と $ax \in a_{n+d}$ が仮定によって等価である場合、したがって $p \cap A_n = a_n$ が完成し、問題を解く段階的素数イデアル $p$ の存在の証明が完成します。 また、$p'$ が、$n \geq n_0,$ に対して $p' \cap A_n = a_n$ となるような、$A$ の別の段階素数イデアルである場合、すべての $x \in p,$ に対して $a \notin p'$ と $ax \in p'$ が成り立ち、$p'$ が素数であるため、$p \subset p'$ となります。 一方、$x$ が $p',$ の次数 $n \geq 0$ の同次要素である場合、$ax$ は次数 $n + d \geq n_0$ の同次要素であるため、$p' \cap A_{n+d} = a_{n+d}$ に属します。したがって、定義により $x \in p$ となり、$p' \subset p$、最後に $p' = p$ であることがわかります。

#### 命題 6 {#ac-iii-s1-prop-6 .statement tag=04DB}

*d を整数 $\geq 1$ とします。*

(i) *A のすべての必須段階的イデアル p について、$p \cap A^{(d)}$ は $A^{(d)}$ の必須段階的素数イデアルです。*

(ii) *逆に、$A^{(d)}$ のすべての必須の段階的素数イデアル $p'$ に対して、$p \cap A^{(d)} = p'$ となるような A の固有の (必然的に必須の) 段階的素数イデアル $p$ が存在します。

(i) $a \in A_k$ が属するから $p_k$ にならない場合、$a^{kd}$ は属するから $p_{kd}$ にならないため、$p \cap A^{(d)}$ が必須です。

(ii) すべての $n \geq 0$、集合 $p \cap A$ は、$x^d \in p'$ となるように、$x \in A$ の集合 $a_n$ に等しくなければなりません。 $a = \bigoplus_{n \geq 0} a_n$ が段階的素数イデアルであることを示しましょう。 $a_n = p'_n$のように、$n$が$d$の倍数であるとき、$p'$は素数なので、$p$の一意性が証明されます。ここで、$x \in a_n$、$y \in a_m$、$(x - y)^{2d}$ が項の和である場合、それぞれは次数の同次元により、$x^d$ または $y^d$ の積になります。 $nd$ したがって $(x - y)^{2d} \in p'$、そして $p'$ が素数であるため、$(x - y)^d \in p'$ したがって $a_n$ は $A$ の部分群です。 $p'$ は $A^{(d)}$ の理想であるため、$a$ は $A$ の段階的な理想です。最後に、関係 $(xy)^d \in p'$ は $x^d \in p'$ または $y^d \in p'$ を暗示し、命題 4 によって証明が完成します。

$A$ を正の次数を持つ段階的可換環とし、$p$ を本質的な段階的素数理想である $A$ とします。 *均質*の集合 $S$ 所属から $p$ ではない $A$ の元は乗法であり、したがって分数 $S^{-1}A$ の環は標準的に等級付けされます (章) II, § 2, no. 9) (この目盛りでは、一般に、負の次数の同種の元 $\neq 0$ が存在することに注意してください)。 次数 0 の同次元の $S^{-1}A$ からなるの $A_{(p)}$ 部分環を、分数 $x/s$ の語集合で表すことにします。 $x$ と $s$ は、$A$ と $s \notin p$ の同じ次数と同次です。同様に、すべての等級付けされた $A$ モジュール $M$ について、$S^{-1}M$ は標準的に等級付けされ (*loc. cit.*)、次数 0 の同種元の $M_{(p)}$ 部分群によって示されます。 $A_{(p)}$-モジュール。

#### 命題 7 {#ac-iii-s1-prop-7 .statement tag=04DC}

*$p$ を $A$、$d$ 整数 $\geq 1$、および $p'$ を $A^{(d)}$ の段階素数イデアル $p \cap A^{(d)}$ とします。すべての等級付けされた $A$ 加群 $M$ について、標準単射 $M^{(d)} \to M$ から導出された準同型 $(M^{(d)})_{(p')} \to M_{(p)}$ は全単射です。*

$S$ が $p$ と $S' = S \cap A^{(d)}$ に対する所属ではなく、$A$ の同次元の集合である場合、標準準同型 $\phi : {S'}^{-1}M^{(d)} \to S^{-1}M$ は次数 0 の同次準同型であり、は単射法です。なぜなら、$x \in M_{nd}$ が $s \in A_n, s \notin p$ に対して $sx = 0$ を満たす場合、$s^dx = 0$ と $s^d \in A_{md}, s^d \notin p'$ も満たすからです。 $(M^{(d)})_{(p')}$の$\phi$の下の像が$M_{(p)}$の全体であることを示すことが残っています。ただし、$x \in M_n, s \in A_n$ と $s \notin p$ の場合は、$x/s = (xs^{d-1})/s^d$ も$xs^{d-1} \in A_{nd}, s^d \in A_n$ と $s^d \notin p'$、よってが主張になります。

#### 命題 8 {#ac-iii-s1-prop-8 .statement tag=04DD}

*$m = \bigoplus_{i \geq 1} A_i$にしましょう。 $(p^{(k)})_{1 \leq k \leq s}$ を、$A$ の段階的素数* イデアルの有限族とし、すべての $k$ に対して $\mathfrak{a} \cap m \not\subset p^{(k)}$ となるような段階的イデアル $\mathfrak{a} \subset A$ とする。その場合、$p^{(k)}$ のいずれに対しても所属ではなく、同種の元 $z \in \mathfrak{a} \cap m$ が存在します。

$n$ については帰納法により、$n = 1$ にとって命題は自明であると主張します。 $\mathfrak{a} \cap m \cap p^{(j)}$ が添字 $k \neq j$ の $p^{(k)}$ の 1 つに含まれるような添字 $j$ が存在する場合、帰納法の仮定から、どの所属にも所属ではなく同次元 $z' \in \mathfrak{a} \cap m$ が存在することがわかります。 $p^{(k)}$ の $k \neq j$ は、所属から $p^{(j)}$ にもならず、この元は問題を解決します。次に、すべての添字 $j$ について、$\mathfrak{a} \cap m \cap p^{(j)}$ が添字 $k \neq j$ の $p^{(k)}$ のいずれにも含まれていないとします。したがって、帰納法の仮定は、$k \# j$ に対する $S_j$ のどれにも同種の元 $y_j \in \mathfrak{a} \cap m \cap S_j$ 所属が存在することを意味します。 $y_j$ はすべて次数 $\geq 1$ であるため、置き換えることを適切な冪 ($p^{(k)}$ は素数であるため) によって、$y_1$ と $\prod_{j=2}^n y_j$ は同じ次数であると仮定できます。この場合、$z = y_1 + \prod_{j=2}^n y_j$ は次数 $\geq 1$ と同次であり、章 II, § 1, no. 1 と同じ引数で、命題 2 は $z$ が問題を解くことを示します。

### 練習問題 {#ac-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
