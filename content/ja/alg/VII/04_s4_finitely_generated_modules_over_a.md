---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 4
section_title: Finitely generated modules over a principal ideal domain
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.15-A VII.28, A VII.62-A VII.70
pdf_pages: 0374-0387, 0421-0429
extraction: ocr
subsections:
    - "no": 1
      title: Direct sums of cyclic modules
      page: 15
      pdf_page: 374
    - "no": 2
      title: Content of an element of a free module
      page: 16
      pdf_page: 375
    - "no": 3
      title: Invariant factors of a submodule
      page: 18
      pdf_page: 377
    - "no": 4
      title: Structure of finitely generated modules
      page: 19
      pdf_page: 378
    - "no": 5
      title: Calculation of invariant factors
      page: 20
      pdf_page: 379
    - "no": 6
      title: Linear mappings of free modules, and matrices over a principal ideal domain
      page: 21
      pdf_page: 380
    - "no": 7
      title: Finitely generated abelian groups
      page: 22
      pdf_page: 381
    - "no": 8
      title: Indecomposable modules. Elementary divisors
      page: 23
      pdf_page: 382
    - "no": 9
      title: Duality in modules of finite length over a principal ideal domain
      page: 25
      pdf_page: 384
statements: 40
exercises: 25
content_sha256: 149c79cac33be8f4ce47dec32691d5f4ecf0232ea6043d89565d005f9838a416
translated_from: content/en/alg/VII/04_s4_finitely_generated_modules_over_a.md
translation_method: google
source_content_sha256: e417e7dc96e464c48ed19a91e2e8d38e2c97d4afc92adb2cc15edbd954a62d34
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 87f6b08cf9d5ac2efeaf7b18e474902605e1cbf886a526fb0d2edd6fe50c6c67
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 有限生成加群主イデアル整域以上

### 1. サイクリック加群の直和

Aを可換環とします。 (II、p. 220、提案 22) を思い出してください。循環 A-加群は *商加群* $A/a$ と同型です。ここで、a は A のイデアルです。 主イデアル整域上のすべての有限生成加群は次のとおりであることが後でわかります (セクション 4)。有限多循環加群の直和。

#### 命題 1 {#alg-vii-s4-prop-1 .statement tag=073N}

— *E を可換環 A よりも加群とします。 E が n 巡回加群 $\Lambda/\mathfrak{a}_k$ ($1 \leq k \leq n$) の直和であると仮定します。ここで、$\mathfrak{a}_k$ は A のイデアルです。*

すると、各整数 $p > 0$ について、$A$ 加群 $\bigwedge^p E$ は加群 $A / a_H$ の直和と同型であり、各 $p$ 要素部分集合 $H = \{ k_1, \ldots, k_p \}$ $[1, n]$ については、理想的な$a_H$は$\sum_{j=1}^p a_{k_j}$です。

$x_k$ を $A / a_k$ の正規の生成元、つまり $A$ の単位元の像とすると、$E$ は $Ax_i$ ($1 \leq i \leq n$) の直和になります。次に、外部代数 $\bigwedge^n E$ がテンソル積 $\bigotimes_{i=1}^n (\bigwedge (Ax_i))$ の $A$ 加群として同型であることがわかります (III, p. 515、提案 10)。ここで、$\bigwedge (Ax_i)$ は単に直和 $A \oplus Ax_i$ です。$Ax_i$ の任意の 2 つの元の外側積が零であるため、$\bigwedge^p E$ は加群 $M_H = (Ax_{k_1}) \otimes \ldots \otimes (Ax_{k_p})$ の直和になります。 $H = \{ k_1, \ldots, k_p \}$ は、$p$ の集合、$[1, n]$ の要素部分集合 ($k_1 < \ldots < k_p$ と) を超えます。現在、$M_H$ は $A / a_{11}$ (II、p. 257、Cor. 4) と同型であることが知られており、証明が完成します。

提案 1 の記法で、理想が $a_k$ 形増加する数列である場合、それらは加群 $E$ によって完全に決定されることがわかります。より正確には:

#### 命題 2 {#alg-vii-s4-prop-2 .statement tag=073O}

— *$A$ を可換環とし、$E$ を $n$ 循環加群 $A / a_k$ の直和とします。ここで、$a_k$ 満たす $a_1 \subset a_2 \subset \ldots \subset a_n$。次に、$1 \leq p \leq n$ の場合、理想的な $a_p$ は $\bigwedge^p E$ の消滅子です。 $a_n \neq A$ の場合、$1 \leq p \leq n$ の場合は $\bigwedge^p E \neq 0$、$m > n$ の場合は $\bigwedge^m E = 0$。

実際、提案 1 の記法では、$a_p = a_{s(H)}$ があり、$s(H)$ は部分集合 $H$ の最大の元を表します。すべての $p$ 要素部分集合 $H$ については $s(H) \geq p$ であるため、$H = \{ 1, \ldots, p \}$ については $s(H) = p$ であるため、$H$ が集合にわたって変化するため、$a_p$ は $a_r$ の共通部分であることがわかります。 $p$ - $(1, n)$ の要素部分集合;したがって、提案 1 によれば、イデアル $a_p$ は確かに $\bigwedge^p E$ の消滅子になります。

#### 系 {#alg-vii-s4-n1-cor-1 .statement tag=073P}

— *提案 2 の記法で、$a_n \neq A$ の場合、および $E$ が $m$ の循環加群 $A / a'_j$ と $a'_1 \subset a'_2 \subset \ldots \subset a'_m \neq A$ の直和にも同型である場合、$m = n$ および$1 \leq k \leq n$ の $a_k = a'_k$ (*$a_k *$ の一意性)。

### 2. 自由加群の元の内容

$A$ を主イデアル整域、$L$ を自由な $A$ モジュール、$x$ を $L$ の元とします。 $f$ が $L$ 上の線形形式の集合 $L^*$ を通過すると、要素 $f(x)$ は、$L$ の $x$ の *内容* と呼ばれる、$A$ の理想的な $c_L(x)$ を形成します。 $A$ の要素 $c$ は、理想的な $c_{L}(x)$ を生成する場合、$L$ の $x$ の *内容* と呼ばれます。これは、$L$ 上に $f(x) = c$ となる線形形式 $f$ が存在し、$L$ 上のすべての線形形式 $g$ に対して $c$ が $g(x)$ を除算することを意味します。 $(e_i)_{i \in I}$ を $L$ の基底とします。 $x = \sum a_i e_i, a_i \in A$を入れます。その場合、理想的な $c_L(x)$ は和 $\sum a_i b_i$ で構成され、$(b_i)$ は集合 $A'$ を通過します。 $A$ の元 $c$ は、$x$ の座標の$(a_i)$ ファミリの gcd である場合に限り、$L$ の $x$ の内容であることがすぐにわかります。

$c_L(x) = A$ の場合、つまり $L$ の基底に関する $x$ の座標が集合的に互いに素である場合、$x$ は *不可分* であると言います。

#### 補題 1 {#alg-vii-s4-lem-1 .statement tag=073Q}

*$L$ を主イデアル整域 $A$ の自由加群とし、$x$ を $L$ の元とします。したがって、次の条件は同等です*:

(i) $x$ は分割できません。
(ii) * $L$ には $f(x) = 1$ となる線型形式 $f$ が存在します。
(iii) $x$ は非零であり、部分加群 $Ax$ は $L$ の直因子です。
(iv) $x$ は、$L$ の一部の基底の元です。

(i) $\Rightarrow$ (ii) : これは定義から続きます。
(ii) $\Rightarrow$ (iii) : $f$ を $L$ 上で線型形式とし、 $f(x) = 1$ とする。次に、$x \neq 0$ と写像 $y \mapsto f(y)x$ は、$L$ の射影子で、像 $Ax$ です。
(iii) $\Rightarrow$ (iv) : $L'$ を $L$ の $Ax$ の補数とし、$B'$ を $L'$ の基底とする (*VII*, p. 15, Cor. 2)。すると、$B' \cup \{x\}$は$L$の基底になります。
(iv) $\Rightarrow$ (i) : 些細なこと。

#### 注意 {#alg-vii-s4-n2-rem-1 .statement tag=073R}

— 1) $x$ が $L$ の非零元で、$c$ が $x$ の内容である場合、 $x = cy$ となる $L$ の一意元 $y$ が存在します。これを元 $x/c$ と示します。その場合、$x/c$ は $L$ の分割できない元です。
2) 内容$c_L(x)$は捩れの消滅子、$L/Ax$の加群です。

$L$ を主イデアル整域 $A$ の自由加群とし、$M$ を $L$ の部分加群とします。 by *VII*、p. 4、補題 1、家族 $c_L(x), x \in M$ には極大元があります。 $M \neq \{0\}$ の場合、その極大元は非零です。

#### 命題 3 {#alg-vii-s4-prop-3 .statement tag=073S}

*$L$ を主イデアル整域 $A$ の自由加群とし、$M$ を $L$ の非零部分加群とします。 $M$の元の内容の中で$c_L(x)$が最大となるような$M$の元を$x$とし、$c$を$L$の$x$の内容とし、$f$を$L$ の線型形式は $f(x) = c$ になります。

a) $L$ は、$A(x/c)$ と $f$ のカーネル $K$ の直接和です。
b) $M$ は、$Ax$ と $K \cap M$ の直接和です。
c) $L$ 上のすべての線形形式 $g$ に対して $g(M) \subset Ac$。

$y = x/c$ を入れてください。 $f(y) = 1$ 以来、明らかに $Ay \cap K = \{0\}$ です。さらに、それぞれの $u \in L$ について、
$$
u = f(u)\,y + (u - f(u)\,y),
$$
$f(u)y \in Ay$ と $u - f(u)y \in K$ ;これは *a)* を証明します。ここで、$u \in M$ に対して $f(u) \in Ac$ があることに注意してください。実際、$u \in M$ と $d$ を $f(u)$ と $c$ の gcd とします。その場合、 $d = Xf(u) + \mu c = f(Xu + \mu x)$ となるような $\lambda, \mu \in A$ が存在します。したがって、 $M$ 割る $d$ の元 $\lambda u + \mu x$ の内容になります。 $c$ の最大値により、これは $d$ が $c$ の関連物であることを意味し、つまり $f(u) \in Ac$ になります。したがって、$M$ のすべての $u$ について、次のように書くことができます。
$$
u = (f(u)/c)\,x + (u - (f(u)/c)\,x) \in Ax + (K \cap M),
$$
これは *b)* を示しています。最後に、$g$ を $L$ の線型形式とします。 *a)* により、 $K$ には $g(u) = \alpha f(u) + h(u - f(u)\,y)$ となるようなスカラー $\alpha \in A$ と線型形式 $h$ が存在します。したがって、

b) $g(M) \subset Ac + h(K \cap M)$ があります。したがって、c) を証明するには、$K$ 上のすべての線型形式 $h$ に対して $h(K \cap M) \subset Ac$、または同等に $L$ 上のすべての線型形式 $h$ について、$h(x) = 0$ が成り立つことを証明すれば十分です。ここで、$u \in K \cap M$ と $d$ が $h(u)$ と $c$ の gcd である場合、$d = \lambda h(u) + \mu c$ を持つ $A, \mu \in A$ が存在します。次に $(f + h)(Au + \mu x) = d$ が続き、これは上記のように $h(u) \in Ac$ を意味し、c) が続きます。

### 3. 不変式因子/部分加群

#### 定理 1 {#alg-vii-s4-thm-1 .statement tag=073T}

— $L$ を主イデアル整域 $A$ の自由加群とし、$M$ を有限階数 $n$ の $L$ の部分加群とします。次に、$L$ の基底 $B$、$n$ 元 $e_i$ の $B$、および $A$ ($1 \leq i \leq n$) の $n$ 非零元 $\alpha_i$ が存在します。
a) $M$ の $\alpha_i e_i$ 形基底;
b) $a_i$ 割る $\alpha_{i-1}$、$1 \leq i \leq n-1$ の場合。

さらに、$(e_i)$ によって生成される加群 $M'$ と主要なイデアル $A\alpha_i$ は、上記の条件によって一意に決定されます。 加群 $M'/M$ は $L/M$ の捩れ部分加群であり、$A$ 加群 $A/A\alpha_i$ の直和と同型です。最後に、$L/M$ は $M'/M$ の直和であり、自由加群は $L/M'$ と同型です。

1) $e_i$ と $\alpha_i$ の存在。

$M = \{0\}$ の場合、定理は自明です。 $M \neq \{0\}$ の場合、提案 3 から、$L$ の元 $e_1$、$A$ の非零元 $a$、および $L$ の部分加群 $L_1$ が存在することがわかり、$L$ は次のようになります。 $Ae_1$と$L_1$の直和、$M$は$A\alpha_1 e_1$の直和、$L$の部分加群$M_1 = M \cap L_1$、そして線型形式ごとに$g(M) \subset A\alpha_1$となる$L$の$g$。

これで、$M$の階数$n$を帰納法まで進めることができます。 $L_1$ は自由加群 (VII、p. 15、Cor. 2) であり、$M_1$ は階数 $n-1$ であるため、$L_1$、$(n-1)$ の基底 $B_1$ が存在します。 $B_1$の元 $e_2, \ldots, e_n$、および$A$の非零元 $\alpha_2, \ldots, a$、$(\alpha_2 e_2, \ldots, \alpha_n e_n)$は$M_1$の基底、および$\alpha_i$ 割る $\alpha_{i+1}$ $2 \leq i \leq n-1$。 $L'$ が $e_1, \ldots, e_n$ とは異なる $B_1$ の元によって生成された $L$ の部分加群である場合、$L$ は $e_1, \ldots, e_n$ によって生成された $L'$ および加群 $M'$ の直和です。現在、$(e_1, \ldots, e_n)$は$M'$の基底、$(\alpha_1 e_1, \ldots, \alpha_n e_n)$は$M$の基底です。 今残っているのは、$a_i$ 割る $a_i$ であることを示すことだけです。しかし、$A\alpha_2$ には形 $g(M_1)$ があり、$g$ は $i \neq 2$ と $g(L') = (0)$ の $g(e_2) = 1, g(e_i) = 0$ によって定義された $L$ の線型形式です。そしてその上にある$g(M_1) \subset A\alpha_1$を見てきました。

2) 一意性プロパティ。

$a_i$ は非零なので、加群 $M'$ は $x \in L$ の集合であり、$A$ の一部の $\beta \neq 0$ については $\beta x \in M$ になります。他の語 $M'/M$ は、$L/M$ の捩れ部分加群です。これはユニークな決定する $M'$ です。

$M'/M$ が $n$ 循環加群 $A/A\alpha_i$ (II, p. 204, 公式 (26)) の直和と同型であることは明らかです。 $r$ を、$A$ とは異なる理想 $A\alpha$ の数とします。つまり、最初の $n-r$ 理想 $A\alpha_i$ は $A$ に等しく、最後のレアは $A$ とは異なります。次に、$M'/M$ は、加群 $A/A\alpha_n, \ldots, A/A\alpha_{n-r+1}$ の直和とも同型です ($A\alpha_n \subset A\alpha_{n-1} \subset \ldots \subset A\alpha_{n-r+1} \neq A$)。

したがって、コルの条件。提案 2 (VII、p. 16) は満たされます: したがって、理想 $Aa_i$ ($1 \leq i \leq n$) は加群 $M'/M$ によって一意に決定されます。

$L$ は $M'$ と $L'$ の直和であるため、$L/M$ は $M'/M$ と $(L' + M)/M$ の和であり、この和は $(L' + M) \cap M' = M$ から直接です。一方、$(L' + M)/M$ は $L'/(M \cap L')$ (I, p. 41, Th. 4, c))、つまり $L'$ と同型であり、これは $(L' + M)/M$ が自由加群と $L/M'$ と同型であることを示しています。

#### 系 {#alg-vii-s4-n3-cor-1 .statement tag=073U}

— $L/M$ が捩れ空いている場合に限り、主イデアル整域 $A$ 上の自由加群 $L$ の有限階数の部分加群 $M$ は、$L$ に補数があります。

木曜日記法に。 1、$L/M$ が捩れ空いている場合、$M = M'$、$M'$ には $L$ に補数 $L'$ があります。逆に、$M$ が $L$ に補数 $L'$ を持っている場合、$L/M$ は$L'$ と同型であり、これは自由 (VII、p. 15、Cor. 2)、およびなおさら捩れは自由です。

#### 注意 {#alg-vii-s4-n3-rem-1 .statement tag=073V}

自由加群 $L$ の無限ランクの部分加群 $M$ は、$L/M$ が捩れ自由であるが、$L$ では$M$ が補数を持たないということが起こります (VII、p. 60、例 6、b))。

#### 定義 1 {#alg-vii-s4-def-1 .statement tag=073W}

— 記法と Th の仮説において。 1 では、$A$ のイデア $A\alpha_i$ は、加群 $L$ に関して部分加群 $M$ の不変量因子と呼ばれます。

$A$ が有理数整数の環 $\mathbf{Z}$ または体 $K$ 上の 1 つの不定数における多項式環 $K[X]$ の場合、$A$ の各イデアルに対して生成元を選択する標準的な方法があります。 $\mathbf{Z}$ の場合は正の整数、$K[X]$ の場合はモニック多項式 (VII、p. 5)。これらのそれぞれの場合において、不変式因子 $Aa_i$ の標準生成元は、言葉の乱用により、$L$ に関する $M$ の不変式因子とも呼ばれます。

### 4. 構造/有限生成加群

#### 定理 2 {#alg-vii-s4-thm-2 .statement tag=073X}

— 主イデアル整域 $A$ 上のすべての有限生成加群 $E$ は、循環加群 $A/a_k$ の有限数 $m$ の直和と同型であり、$a_k$ は次のイデアルです。 $a_1 \subset a_2 \subset \ldots \subset a_m \neq A$ などの$A$ (一部は零) であり、これらの条件によって一意に決定されます。

$E$ が $q$ 元によって生成できる場合、商加群 $L/M$ と同型になります。ここで、$L = A^q$ (II. p. 218) です。 $M$ には有限階数 $n \leq q$ (VII、p. 15、提案 1) があるため、Th の条件 1 (VII、p. 18) は満足しています。その後、Th の記法に。 1 $L/M$ は、$L$ および捩れ加群 $M'/M$ の $M'$ の補数 $L'$ の直和と同型です。 加群 $L'$ は有限階数 $p = q - n$ を含まないため、$A^p$ と同型です。 $r$ が $A\alpha_r \neq A$ となるような最小の添字である場合、$M'/M$ は $r \leq i \leq n$ について加群 $A/A\alpha_i$ の直和と同型です。次に、$1 \leq k \leq p$ に対して $m = p + (n - r + 1)$、$a_k = (0)$、$1 \leq j \leq n - r + 1$ に対して $a_j = A\alpha_n , - ,$ を取ると、前述の条件が満たされます。 一意性はコルから続きます。 VII、p. 16の。

#### 系 1 {#alg-vii-s4-thm-2-cor-1 .statement tag=073Y}

— *主イデアル整域を超えるすべての有限生成加群 E は、捩れの直和、E の部分加群、および自由加群です。*

E の捩れ部分加群には、一般にいくつかの異なる補数があります。たとえば、$E = \mathbf{Z} \times (\mathbf{Z}/(2))$ の場合、E の捩れ部分加群は $\{0\} \times (\mathbf{Z}/(2))$ です。補数として部分加群 $\mathbf{Z} \times (0)$ と、すべての元 $(n, \overline{n})$ の部分加群からなるがあり、$n$ は $\mathbf{Z}$ を通過し、$\overline{n}$ は剰余です。 $n$ mod 2 の類。

#### 系 2 {#alg-vii-s4-thm-2-cor-2 .statement tag=073Z}

— *主イデアル整域を超えるすべての捩れが無料有限生成加群は、有限階数が無料になります。*
これはコルからすぐに続きます。 1.

条件加群が有限に生成されることが不可欠です。たとえば、A の分数の体の加法群は、A の捩れが A-加群として自由になります。ただし、$A \neq K$ の場合は自由加群ではなく、一方で K の任意の 2 つの元は共通の因子を持ち、他方では K は循環 A-加群ではなく、そうでない場合は $K = ab^{-1}A$ ($a, b \in A$)、 よって $b^{-2} = acb^{-1}$ ($c \in A$) なので、$b^{-1} = ac \in A$、そして $K = A$ です。

#### 定義 2 {#alg-vii-s4-def-2 .statement tag=0740}

— *記法と Th の仮説。 2、理想 $a_k$ は、加群 E* の不変量因子と呼ばれます。
Defのように。 1 (VII, p. 19)、$A = \mathbf{Z}$ または $A = K[X]$ の場合、理想 $a_k$ (正の整数またはモニック多項式) の標準生成元は、言葉の乱用により、次の *不変式因子* とも呼ばれます。 有限生成加群 E.

加群 E の不変式因子と、自由加群 L の不変式部分加群 M の不変式と、加群 L (定義 I) に関して混同しないように注意しなければなりません。

### 5. 不変式の計算因子

#### 命題 4 {#alg-vii-s4-prop-4 .statement tag=0741}

— *A を主イデアル整域とし、L を自由A-加群とし、有限基底 $(u_j)$ ($1 \leq j \leq k$) とし、M を L の部分加群とし、$(x_i)$ を生成元の系とするM の $A \alpha_i$ ($1 \leq i \leq n$) を L に関する M の不変量因子とします。次に、$1 \leq m \leq n$ 積 $\delta_m = \alpha_1 \ldots \alpha_m$ は、行列の m 番目の位数マイナーの gcd であり、その列は、基底 $(u_j)$ に対する $x_i$ の座標ベクトルです。

Thさんより1 $M \subset \alpha_1 L$ であることは明らかです。したがって、M の任意の元の座標は、$a_1$ の倍数になります。一方、Lには$a_1$が内容となるMの元$x$が存在します。 $x$を$x_i$の線形結合として表現すると、$a_1$は$x_i$の座標によって生成される理想の元となる。これらはすべて $a_1$ の倍数であるため、$a_1$ が確かにそれらの gcd であり、私たちの主張は $m = 1$ の場合に証明されます。

一般的な $m$ については、M (III, p. 507) の m 番目の *外部冪* $\bigwedge^m M$ を考慮します。 Thの表記では。 1 $a_i = \alpha_i e_i$ ($1 \leq i \leq n$) である M には基底 $(a_i)$ が存在します。したがって、$(i_1, \ldots, i_m)$ は$(1, n)$ の$m$ 要素の厳密に増加するシーケンスのセットを実行するため、$\bigwedge^m M$ は要素 $a_{i_1} \wedge \ldots \wedge a_{i_m}$ で構成される基底を持ちます。 現在、元 $e_{i_1} \wedge \ldots \wedge e_{i_m}$ 属するから基底 $B_m$ の $\bigwedge^m L$ です。 したがって、$\bigwedge^m M$ から $\bigwedge^m L$ への正規の写像は、$\bigwedge^m M$ から $\bigwedge^m L$ の部分加群への同型で、基底元 $(\alpha_{i_1} \ldots \alpha_{i_m})\, e_{i_1} \wedge \ldots \wedge e_{i_m}$ となり、この部分加群を同一視するとします。 $\bigwedge^m M$。 $\alpha_j$ は $j \geq k$ の $\alpha_k$ の倍数であるため、要素 $\alpha_{i_1} \ldots \alpha_{i_m}$ はすべて $\delta_m = \alpha_1 \ldots \alpha_m$ の倍数であり、そのうちの 1 つは $\delta_m$ に等しくなります。したがって、$\delta_m$ は、$\bigwedge^m M$ の生成器系の要素の $B_m$ に関する座標の gcd です。 引数の最初の部分は、$\delta_m$ が、$\bigwedge^m L$ の任意の基底に関して、$\bigwedge^m M$ の生成元の任意の系の座標の集合の gcd であることを示しています。 $L$の$(u_j)$の基底から導き出される$\bigwedge^m L$を基底とし、$(x_i)$の外面積の$\bigwedge^m M$からなるを生成元の系とすれば、これらの座標を表す式となります。 行列式の項の積 (III、p. 528、提案 9) は、記載された結果を与えます。

### 6. 自由加群の線形写像、および主イデアル整域の上の行列

$A$を主イデアル整域とします。 線形写像 $f$ を、階数 $m$ の空き $A$ モジュール $L$ から階数 $n$ の空き $A$ モジュール $L'$ に変換することを考えてください。前述の結果により、$L$ と $L'$ に適切な基底を選択することで、行列の *標準形* と呼ばれる、特に単純な形の $f$ に行列を入れることができます。

#### 命題 5 {#alg-vii-s4-prop-5 .statement tag=0742}

*$A$を主イデアル整域、$f$を階数$r$の$A$モジュール$L$の階数$m$を自由な$A$モジュールに変換する線形写像とする階数 $n$の$L'$。次に、$L$ の基底 $(e_i)$ ($1 \leq i \leq m$) と $L'$ の $(e'_j)$ ($1 \leq j \leq n$) が存在し、$1 \leq i \leq r$ の場合は $f(e_i) = \alpha_i e'_i$、$i > r$ の場合は $f(e_i) = 0$ になります。 $\alpha_i$ は $A$ の非零元であり、それぞれ次の割るです。理想 $A \alpha_i$ は $L'$ における $f(L)$ の不変条件因子であるため、一意に決定されます。

$L_0 = f^{-1}(0)$ を $f$ の核とします。 商 $L/L_0$ は、$L'$ の部分加群である加群 $f(L)$ と同型であり、自由です (*VII*、p. 15、Cor. 2)。したがって、$L_0$ には $L$ に補数 $L_1$ があり (*II*、p. 218、提案 21)、$f$ から $L_1$ の制限は $L_1$ から同型になります。 $f(L) = M'$。 理想 $A \alpha_i$ ($1 \leq i \leq r$) が $L'$ における $M'$ の不変式因子である場合、Th. *VII* の 1、p. 18 は、$(\alpha_i e'_i)$ ($1 \leq i \leq r$) が $M'$ の基底となるように、$L'$ の基底 $(e'_j)$ ($1 \leq j \leq n$) が存在することを示します。 $f$から$L_1$の制限は、$L_1$から$M'$までの同型なので、$f(e_i) = \alpha_i e'_i$となるような$L_1$の基底$(e_i)$($1 \leq i \leq r$)が存在します。 この基底拡大するは、$(e_s)$ ($r+1 \leq s \leq m$) を核 $L_0$ の基底として、$L$ の基底 $(e_s)$ ($1 \leq k \leq m$) になります。

#### 系 1 {#alg-vii-s4-prop-5-cor-1 .statement tag=0743}

— X を階数 r の行列とし、n 行と m 列、主イデアル整域 A 上にします。すると、形のX (II, p. 354) に相当する行列 $X_0$ が存在します。

$$
\begin{pmatrix}
\alpha_1 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & \alpha_2 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & \alpha_r & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0
\end{pmatrix}
$$

ここで、$\alpha_i$ は A の非零元であり、それぞれ次の割るです。これら条件の下で$\alpha_i$は可逆元によって乗法まで一意に決まります。

位数 n と m の可逆な正方行列 P と Q が A 上に存在する場合、2 つの行列 X と $X'$ が等価であるとすると、$X' = PXQ$ のように、Cor. 1は、行列の項で表現された提案5にすぎません。

提案 5 の記法および Cor. 1、(非零) イデアル $Au$ は、線形写像 f または行列 X の不変量因子と呼ばれます。その後、コルからすぐに続きます。 I:

#### 系 2 {#alg-vii-s4-prop-5-cor-2 .statement tag=0744}

— 主イデアル整域 A 上の n 行と m 列を持つ 2 つの行列 X と $X'$ は、同じ不変式因子を持つ場合にのみ等価です。

A が体の場合、$\alpha_i$ を 1 に等しいとみなすことができ、その後、II、p. 360 の提案 13 が得られることに注意してください。

X が L の任意の基底および L' の任意の基底に関する線形写像 f の行列である場合、X の列は、L' の基底に関する、生成器系を形成する L' の要素の座標ベクトルです。 $f(L)$。 したがって、次の結果は、提案 4 の明らか帰結となります。

#### 命題 6 {#alg-vii-s4-prop-6 .statement tag=0745}

— X を主イデアル整域 A 上の階数の行列とし、$A \alpha_i$ ($1 \leq i \leq r$) を不変式因子の数列とします。すると、$\alpha_1$ は X の元の gcd です。そして、積 $\alpha_1 \ldots \alpha_q$ は、$q \leq r$ に対する X の q 番目の位数マイナーの gcd です。

### 7. 有限生成アーベル群

$A = \mathbf{Z}$の場合、切断4の結果を表現できます

#### 定理 3 {#alg-vii-s4-thm-3 .statement tag=0746}

— 有限に生成されたすべてのアーベル群 G は、その捩れ部分群 F の直和 (G の有限位数の元の部分群) と自由なアーベル群です。 有限階数 p ($\mathbf{Z}^p$ と同型)。 群 F は、位数 $n_1, n_2, \ldots, n_q$ の循環群の有限数の直和で、$n_i$ は整数 $> 1$ で、それぞれ前の割るです。また、整数 $p, q$ と $n_i$ ($1 \leq i \leq q$) は $G$ によって一意に決まります。

#### 注意 {#alg-vii-s4-n7-rem-1 .statement tag=0747}

一方、F が直接和である巡回群の次数 $n_1, \ldots, n_q$ は、Th の可分性条件によってよく定義されます。たとえば、$\mathbf{Z}/(p)$ とそれ自体 (p 素数の場合) の積 G では、サブグループは正確に $\mathbf{F}_p$ ベクトル部分空間であり、G は $p(p+1)$ 異なる方法での 2 つの 1 次元部分空間の直接和です。

#### 系 1 {#alg-vii-s4-thm-3-cor-1 .statement tag=0748}

— *有限アーベル群 G には、位数が G の元のすべての位数の lcm である元が存在します。この位数 n は G の最初の不変式因子です。*

#### 系 2 {#alg-vii-s4-thm-3-cor-2 .statement tag=0749}

— *任意の整数 $> 1$ の位数が平方で割り切れない有限アーベル群 G は循環です。*
Th の記法まで続けましょう。 3. 次に、G が有限であるため $p = 0$、そうでない場合は G の位数が $n_q^2$ で割り切れるため、$q \leq 1$ となります。したがって、G は巡回です。

#### 系 3 {#alg-vii-s4-thm-3-cor-3 .statement tag=074A}

— *LとMを階数nの2つの空き$\mathbf{Z}$モジュールとし、$(e_i)$をLの場合は基底、M ($1 \leq i \leq n$)の場合は$(f_i)$基底、uを準同型としますL を M に変換し、基底 $(e_i)$ および $(f_i)$ に対するその行列を U とします。 この場合、$\mathrm{Coker}\,u = M/u(L)$ は、$\det(U) \neq 0$ の場合にのみ有限であり、その後 $\mathrm{Card}(\mathrm{Coker}(u)) = |\det(U)|$ になります。
必要に応じて L と M の基底を変更することで、U が VII、p. 22、Cor. で説明されている形を持つと仮定できます。 1 から提案 5 (この場合、$a_i$ は整数); $\mathbf{Z}$ モジュール $\mathbf{Z}/\alpha_i \mathbf{Z}$ ($1 \leq i \leq n$) の直和の位数は、$a_i$ の 1 つが零であれば無限で、そうでない場合は $|\alpha_1 \alpha_2 \ldots a_n|$ に等しいため、系は明らかになります。

### 8. 不分解加群。初級因子

#### 定義 3 {#alg-vii-s4-def-3 .statement tag=074B}

— *左加群環を超える A は、適切な非零部分加群の家族の直和である場合、分解可能であると言われます。それ以外の場合は、不分解であると言われます。*
したがって、零加群は *分解可能* であり、部分加群の空の族の直和です。
$\mathfrak{a}$ を環 A の左イデアルとします。 $A/\mathfrak{a}$ の部分加群はちょうど商 $b/\mathfrak{a}$ であり、$b$ は含む $\mathfrak{a}$ (I、p. 41、Th. 4) の理想です。 $b$ と $c$ が含む $\mathfrak{a}$ の 2 つの理想である場合、加群 $A/\mathfrak{a}$ は、$A = b + c$ とその場合に限り、部分加群 $b/\mathfrak{a}$ および $c/\mathfrak{a}$ の直和になります。 $b \cap c = \mathfrak{a}$。結果として：

#### 補題 2 {#alg-vii-s4-lem-2 .statement tag=074C}

— *加群 $A/\mathfrak{a}$ は、$\mathfrak{a} \neq A$ であり、A と $\mathfrak{a}$ とは異なる、A の理想の対 $(b, c)$ ($A = b + c$ や $b \cap c = \mathfrak{a}$ など) が存在しない場合に限り、分解不可能です。

#### 命題 7 {#alg-vii-s4-prop-7 .statement tag=074D}

— $A$ を可換環とし、$\mathfrak{p}$ を $A$ (I、p. 117、定義 3) の主イデアルとし、$q$ を $\mathfrak{p}$ に含まれる $A$ のイデアルとする。 $x \in \mathfrak{p}$ ごとに整数 $n > 0$ が存在し、$x^n \in q$ が存在すると仮定します。その場合、$A$ モジュール $A/q$ は分解不可能です。

Let $b$ and $c$ be two ideals of $A$, such that $A = b + c$ and $b \cap c = q$. Then $bc \subset b \cap c = q \subset \mathfrak{p}$; if $x \notin \mathfrak{p}$ and $x \in c$, then $xb \subset p$, so $b \subset \mathfrak{p}$ (I, p. 316, Prop. 4);したがって、$b \subset \mathfrak{p}$ または $c \subset p$ のいずれかになります。たとえば、$c \subset \mathfrak{p}$ なので $b + p = A$ とします。 then there exist $x \in b$ and $y \in \mathfrak{p}$ such that $1 = x + y$; $n \in \mathbf{N}$ を $y^n \in q$ となるようにします。それから$1 = (x + y)^n$。だから$1 \in xA + y^nA \subset b + q \subset b$、だから$b = A$。 補題 2 now shows that $A/q$ is indecomposable.

ここで、$A$ が主イデアル整域であると仮定します。 VII、p. 2、提案 2 によると、$A$ の主な理想は $(p)$ であり、$p$ は $A$ の既約元であり、理想 $0$ です。 by the previous 命題, 加群 $A$ and $A/(p^n)$, for $p$ irreducible and $n > 0$, are indecomposable.すべての循環加群はこの型の加群の直和であるため (VII、p. 3、提案 4)、すべての有限生成された $A$ 加群は循環加群の直和であるため、 (VII, p. 19, Th. 2)、次のように推測します。

#### 命題 8 {#alg-vii-s4-prop-8 .statement tag=074E}

— Let $A$ be 主イデアル整域 and let $M$ be a finitely generated $A$-module.

a) $M$ は、$A$ または形 $A/(p^n)$ の加群と同型である場合に限り、分解不可能です。ここで、$p$ は $A$ の既約元であり、$n > 0$ は整数.

b) $M$ is 直和 of a finite family of indecomposable 部分加群.

部分 b) of the above 命題 can be made more precise as follows:

#### 命題 9 {#alg-vii-s4-prop-9 .statement tag=074F}

— $A$ を主イデアル整域とし、$P$ を $A$ の既約元の代表の系とし、$M$ を有限生成された $A$ 加群とする。次に、正の整数 $m(0)$ と $m(p^n)$ ($p \in P, n > 0$) が存在します。これらは、$M$ が $A^{m(0)}$ の直和と同型であるなど、有限の多くを除いて、$M$ と零によって一意に決定されます。 $(A/(p^n))^{m(p^n)}$ ($p \in P, n > 0$).

整数 $m(0)$ と $m(p^n)$ ($p \in P, n > 0$) の存在は、提案 8 から導き出されます。 整数 $m(0)$ は一意に決定されます。捩れ部分加群により、$M$ の商である自由加群の階数です。 最後に、$M$ の $p$ 主要成分は、$(A/(p^n))^{m(p^n)}$ の直和と同型です。理想群 $(p^n)$ ($n \geq 1$) は包含によって完全に順序付けられているため、$m(p^n)$ の一意性はコルから続きます。 VII、p. 16の提案2に。

#### 定義 4 {#alg-vii-s4-def-4 .statement tag=074G}

— 提案 9 の記法では、$m(p^n) > 0$ が加群 $M$ および整数 $m(p^n)$ の初等因子と呼ばれるようなイデア $(p^n)$ ($p \in P, n \geq 1$ 整数) は多重度と呼ばれます。 整数 $m(0)$ が $> 0$ の場合、それは初級因子 0 の重複度と呼ばれます。

不変式因子 (VII、p. 19、定義 1) に関しては、$A = \mathbf{Z}$ または $A = K[X]$ (K 可換体) の場合、理想$(p^n)$ (正の整数またはモニック多項式) の標準生成元も、次の乱用によって呼び出されます。言語、有限生成加群 $M$ の初級因子。

#### 注意 1 {#alg-vii-s4-n8-rem-1 .statement tag=074H}

$M$ が有限のアーベル群である場合、その構造はその基本因子を書き留めることによって記述でき、それぞれが重複度と同じ頻度で繰り返されます。 We will say, for example, that $M$ is « of type $(2, 2, 4, 27, 27, 25)$ » (or that it is « a group $(2, 2, 4, 27, 27, 25)$ ») if it is isomorphic to the product of two groups $\mathbf{Z}/(2)$, one group $\mathbf{Z}/(2^2)$, two groups $\mathbf{Z}/(3^3)$ and one group $\mathbf{Z}/(5^2)$.

#### 注意 2 {#alg-vii-s4-n8-rem-2 .statement tag=074I}

主イデアル整域 $A$ 上で有限生成された捩れ加群 $M$ が $A/(a_i)$ と同型の巡回加群の直和として与えられる場合 (特に $M$ の不変式因子が既知)、その後、$M$ の初等因子とその多重度は、$A/(a)$ が $A/(p^{n(p)})$ の積と同型であることに注目することで決定できます。ここで、$a = e \prod_{p \in P} p^{n(p)}$ は $a$ の分解で既約因子になります。 ($VII$、p. 3)。たとえば、乗法群 $G(464\ 600)$ を見てみましょう。ここで、$G(n)$ は乗法群 $(\mathbf{Z}/n\mathbf{Z})^*$ ($VII$, p. 12) を表します。 $464\ 600 = 2^3 \cdot 5 \cdot 23 \cdot 101$ 以降、この群は、群 $G(2^3)$、$G(5^2)$、$G(23)$、$G(101)$ ($VII$、p. 13、Th. 3) の積と同型です。ここで、最後の 3 つの群は位数 20、22、および 100 の循環であり、$G(2^3)$ は位数 2 の 2 つの循環群の積 (\emph{loc. cit.})。 $20 = 2^2 \cdot 5$、$22 = 2 \cdot 11$、$100 = 2' \cdot 5^2$ なので、群 $G(464\ 600)$ は型 $(2, 2, 2, 2^2, 2^2, 2^2, 5, 5^2, 11)$ になります。

#### 注意 3 {#alg-vii-s4-n8-rem-3 .statement tag=074J}

基本約数が既知であるねじり加群の不変因子を計算するには、$a_i$ が $A$ のペアごとの互いに素な要素である場合、積 $\prod A/(a_i)$ は $A/(a_1 a_2 ... a_n)$ と同型の巡回加群であるという事実に再び頼ります ($VII$, p. 3、提案 4)。 群 $G(464\ 600) = M$ の例を見て方法を説明しましょう。同じ既約 $p$ の冪である $M$ の基本因子 $p^n$ を、最大ののものから始めて、同じ行に書きます。 指数; 拡大する必要に応じて 1 を入れて、これらの行を同じ長さの行に変換します。

$$
\begin{array}{cccccc}
2^2 & 2^2 & 2 & 2 & 2 \\
5^2 & 5 & 1 & 1 & 1 \\
11 & 1 & 1 & 1 & 1 .
\end{array}
$$

すると、不変式因子は、同じ列の元の積です: $1100, 20, 2, 2, 2$。実際、$M$ は、$VII$, p. 3 の提案 4 により、位数 1100, 20, 2, 2, 2 の巡回群の積と同型です。これらのそれぞれの位数は次の倍数であるため、これらは $M$ ($VII$、p. 22、Th. 3) の不変式因子です。

#### 注意 4 {#alg-vii-s4-n8-rem-4 .statement tag=074K}

$A$ モジュールが非ゼロであり、それ自体と $0$ 以外にサブモジュールがない場合、そのモジュールは単純 ($I$、p. 37) と呼ばれます。したがって、それは必然的に循環的であり、有限に生成され、分解不可能です。モジュール $A/(p^n)$ は $n \neq 1$ に対して単純ではありませんが、モジュール $A/(p)$ は単純であり、リング $A$ がフィールドである場合にのみ $A$ は単純であるため、単純な $A$ モジュールは次のように推定されます。
a) $A$ がフィールドの場合、ランク 1 のモジュールを解放します。
b) 商 $A/(p)$ と同型のモジュール。$p$ は、$A$ が体でない場合、$A$ の既約要素です。

### 9. 主イデアル整域に対する有限長の加群の二重性

このセクションでは、$A$ は体ではない (したがって少なくとも 1 つの既約要素を持つ) 主イデアル領域を表し、$K$ は $A$ の分数体を表します。 すべての $A$ モジュール $M$ に対して、

$$
D(M) = \operatorname{Hom}_A(M, K/A);
$$

$D(M)$ には自然な方法で A-加群の構造が備わっていることがわかります。つまり、すべての準同型 $u : M \to K/A$ とすべての $\alpha \in A$、準同型 $\alpha u$ 写像 $x$ から $\alpha u(x) = u(\alpha x)$ です。 A-加群のすべての準同型 $f : M \to N$ には、準同型 $D(f) : D(N) \to D(M)$ が関連付けられます。ここで、$D(f)(v) = v \circ f$ (II、p. 196) です。 $x \in M$ と $x' \in D(M)$ には $\langle x, x' \rangle = x'(x) \in K/A$ を入れます。この場合、$(x, x') \mapsto \langle x, x' \rangle$ は、$M \times D(M)$ から $K/A$ への *A 双線形* 写像であり、*正準* と呼ばれます。

M と $N$ が 2 つの A-加群である場合、すべての A 双線形写像 $\varphi : M \times N \to K/A$ には、A 線形写像 $d_\varphi : N \to D(M)$ と $s_\varphi : M \to D(N)$ が関連付けられます。ここで、$d_\varphi(y)(x) = \varphi(x, y) = s_\varphi(x)(y)$ (II、p. 268、Cor. から Prop. *1*)。特に、正準 A-bilinear 写像 $M \times D(M) \to K/A$ 定義する A-linear 写像 (*正準* とも呼ばれます)

$$
c_M : M \to D(D(M))
$$

$x \in M$ と $x' \in D(M)$ に対して $\langle x', c_M(x) \rangle = \langle x, x' \rangle$ というように。

#### 命題 10 {#alg-vii-s4-prop-10 .statement tag=074L}

— *M が有限長の A-加群である場合、$D(M)$ は * (一般に非自然に) *M と同型であり、正規の写像 $c_M : M \to D(D(M))$ は同型です。
VII、p. *19*、Th を使用します。 2 および **II**、p. 203、Cor。 1、$M$が循環である場合を簡約するとします。従って、$M = A/tA$ と $t \neq 0$ を仮定することができます。 準同型 $u : A/tA \to K/A$ は、*1* mod $tA$ の類 $\varepsilon$ の $u$ の下の像 $\xi \in K/A$ によって完全に決定され、この元は満たす関係でなければならないことに注意してください。 $t\xi = 0$ ;逆に、$t\xi = 0$ となるような $\xi \in K/A$ に対して、$u(\varepsilon) = \xi$ となるような準同型 $u : A/tA \to K/A$ が存在します。従って、$D(M)$ は $t^{-1}A/A$ と同型であり、$t$ によるホモテティー は K 上で全単射であるため、$D(M)$ は $A/tA$ と同型であり、最初の主張が証明されます。これは、 $M$ と $D(D(M))$ が同型であるため、同じ長さをもつことを証明します。一方、$c_M$ は単射法です。$y \in A$ が関係 $tz \in A$ ($z \in K$ の場合) が $yz \in A$ を意味するようなものである場合、$z = t^{-1}$ を取ると $y \in tA$ が得られます。従って、像 $c_M(M)$ は必ず $D(D(M))$ に等しいということになります。

#### 系 {#alg-vii-s4-n9-cor-1 .statement tag=074M}

— *M、N を有限長の 2 つの A モジュールとし、$\varphi$ を $M \times N$ から $K/A$ への A 双線形写像とする。次のとおり: 1) すべての $y \in N$ に対する関係 $\varphi(x, y) = 0$ は $x = 0$ を意味する。 2) すべての $x \in M$ に対する関係 $\varphi(x, y) = 0$ は $y = 0$ を意味します。 この場合、$\varphi$ に関連付けられた A-linear 写像 $s_\varphi : M \to D(N)$ と $d_\varphi : N \to D(M)$ は同型になります。*
確かに、$\varphi$ に関する仮説は、$s_\varphi$ と $d_\varphi$ が *単射的* であることを意味し、提案 *10* による $\mathrm{long}(D(N)) = \mathrm{long}(N)$ と $\mathrm{long}(D(M)) = \mathrm{long}(M)$ から、これは $\mathrm{long}(M) = \mathrm{long}(N)$ 、従って $s_\varphi$ と $d_\varphi$ が全単射的であることを意味します。

#### 命題 11 {#alg-vii-s4-prop-11 .statement tag=074N}

— *$M' \xrightarrow{u} M \xrightarrow{v} M''$ が有限長の A-加群の完全系列である場合、数列 $D(M'') \xrightarrow{D(v)} D(M) \xrightarrow{D(u)} D(M')$ は正確* [^1] です。

まず、与えられた完全系列を示しましょう。

(1)
$$
0 \to M' \to M \to M'' \to 0
$$

対応する数列

$$
0 \to D(M'') \to D(M) \to D(M') \to 0
$$

正確です。確かに私たちはそれを知っています数列

$$
0 \to D(M'') \to D(M) \to D(M')
$$

は正確です (II, p. 227, Th. 1)。一方、(1) から次のことがわかります。

$$
\operatorname{long}(M) = \operatorname{long}(M') + \operatorname{long}(M'')
$$

(II、p. 212、提案 16);提案 10 により、次のようになります。

$$
\operatorname{long}(D(M)) = \operatorname{long}(D(M')) + \operatorname{long}(D(M''))
$$

その他語 $\operatorname{long}(D(M')) = \operatorname{long}(D(M)/D(M''))$ で。 $D(M)/D(M'')$ は当然 $D(M')$ の部分加群と同一視されるため、$D(M')$ と等しくなければならず、これは私たちの主張を証明します。

これは、$u : M' \to M$ が単射であれば、$D(u) : D(M) \to D(M')$ は全射であることをすぐに暗示します。結論は II、p. 199、注意 4 から導き出されます。

A-加群 M ごとに、M の部分加群の集合を $\mathfrak{S}(M)$ で表します。M の部分加群 N ごと (D(M) の部分加群 N' ごと) で、$N^0$ (それぞれ ${N'}^0$) が M の部分加群を表します。 $D(M)$ (それぞれ M) $x' \in D(M)$ (それぞれ $x \in M$) のうちからなるは、すべての $y \in N$ に対して $(y, x') = 0$ (すべての $y' \in N'$ に対してそれぞれ $(x, y') = 0$) となります。

#### 命題 12 {#alg-vii-s4-prop-12 .statement tag=074O}

*M を有限長の A-加群とします。次に、M のすべての部分加群 N を $N^0$ に送信する写像は、$\mathfrak{S}(M)$ から $\mathfrak{S}(D(M))$ に全単射であり、逆全単射は D(M) のすべての部分加群 N' を M の部分加群 ${N'}^0$ に送信します。 加群 $D(N)$ は$D(M)/N^0$ と、$D(M/N)$ は $N^0$ と自然に同一視されます。さらに、*

(2)
$$
(N_1 + N_2)^0 = N_1^0 \cap N_2^0, \quad (N_1 \cap N_2)^0 = N_1^0 + N_2^0
$$

M のすべての部分加群 $N_1, N_2$ のために。

M の各部分加群 N に対して、完全系列があります。

$$
0 \to N \to M \to M/N \to 0
$$

したがって (提案 11) 完全系列

$$
0 \to D(M/N) \to D(M) \to D(N) \to 0
$$

そして、$D(M)$ の $D(M/N)$ の像は明らかに $N^0$ であるため、(提案 10) $\operatorname{long}(N^0) = \operatorname{long}(M) - \operatorname{long}(N)$ であることがわかります。 $M$ は提案 10 によって $D(D(M))$ と同一視されるため、同様に

$$
\operatorname{long}(N^{00}) = \operatorname{long}(M) - \operatorname{long}(N^0) = \operatorname{long}(N);
$$

加法では、$N \subset N^{00}$ であることは明らかなので、$N^{00} = N$ です。さらに、(2) の最初の関係は明らかで、適用から部分加群 $N_1^0$ と $D(M)$ の $N_2^0$ までに、$(N_1^0 + N_2^0)^0 = N_1 \cap N_2$ ができるので、$N_1^0 + N_2^0 = (N_1^0 + N_2^0)^{00} = (N_1 \cap N_2)^0$ になります。これで命題の証明が完了です。

#### 例 1 {#alg-vii-s4-n9-exa-1 .statement tag=074P}

$A = \mathbf{Z}$ の場合、有限長の $\mathbf{Z}$ 加群はまさに有限のアーベル群です。次に$K = \mathbf{Q}$、つまり$K/A = \mathbf{Q}/\mathbf{Z}$。次に、定義する $D(M)$ に対して、$\mathbf{Q}/\mathbf{Z}$ の代わりに、(V, p. 79, Prop. 2) 群 $R$ of 根のような、それに同型の $\mathbf{Z}$ 加群をときどきとります。特性 0 の代数閉体の単位元 (乗法未満) ;次に$D(M) = \operatorname{Hom}_{\mathbf{Z}}(M, R)$を入れます。 対応する記法でこの特殊なケースについて前述の結果を書き直すのは読者に任せます。

#### 例 2 {#alg-vii-s4-n9-exa-2 .statement tag=074Q}

$a$ を $A$ の非零元とします。 写像 $x \mapsto x/a$ $A$ から $K$ 誘導する同型商加群 $A/(a)$ から部分加群 $(K/A)(a)$ $K/A$ からなる元は$a$によって全滅しました。 $M$ が $a$ によって消滅した $A$ モジュール、または同等の $A/(a)$ モジュールである場合、$A$ モジュール $D(M)$ は $\operatorname{Hom}_{A/(a)}(M, A/(a))$ で識別されます。 対応する記法 (cf. V, p. 86) のこの特殊なケースについて、前述の結果を書き直すのは読者に任せます。

### 練習問題 {#alg-vii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。

[^1]: 後で (A、X、p. 18) で、A-加群 K/A が単射であることがわかります。 したがって、提案 11 は任意の A-加群 M、M'、および M" に対して引き続き有効であることがわかります。
