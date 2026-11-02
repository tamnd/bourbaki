---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: The Structure of Modules of Finite Length
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.25-A VIII.43
pdf_pages: 0042-0060
extraction: native
subsections:
    - "no": 1
      title: Local Rings
      page: 25
      pdf_page: 42
    - "no": 2
      title: Weyr–Fitting Decomposition
      page: 27
      pdf_page: 44
    - "no": 3
      title: Indecomposable Modules and Primordial Modules
      page: 30
      pdf_page: 47
    - "no": 4
      title: Semiprimordial Modules
      page: 32
      pdf_page: 49
    - "no": 5
      title: The Structure of Modules of Finite Length
      page: 37
      pdf_page: 54
statements: 37
exercises: 20
content_sha256: f047d54445eb44a9239a24b452dbbda75a3ec42de1c180411506ddde7dc42d75
translated_from: content/en/alg/VIII/02_s2_the_structure_of_modules_of_finite.md
translation_method: google
source_content_sha256: 937d6660bbf18635e63c4c1addfaf3e44ee88a5456fdc47cb5c2eacabc9099b5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: aebedd7b7ce9aa87b7f9633f6bad724af197326a5b2acab2d5fe934687c19378
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。 構造/加群/有限長

### 1. 局所環

#### 命題 1 {#alg-viii-s2-prop-1 .statement tag=001P}

A を非零環とし、$\mathfrak{r}$ を A の非可逆元の集合とします。以下のプロパティは同等です。

(i) 集合 $\mathfrak{r}$ は A の両面の理想です。

(ii) 集合 $\mathfrak{r}$ は加法以下で安定しています。

(iii) 環 A は独自の最大左イデアルを持ちます。

(iv) $a\in A$ ごとに、元 $a$ および $1-a$ の 1 つが反転可能です。

(v) $a\in A$ ごとに、元 $a$ および $1-a$ の 1 つが反転可能なままになります。

(i) $\Rightarrow$ (ii) の含意は、理想の定義から導き出されます。 1 は属するから $\mathfrak{r}$ にならないので、(ii) $\Rightarrow$ (iv) になります。

A に等しくない A のすべての左イデアルには、$\mathfrak{r}\not= A$ と集合 $\mathfrak{r}$ 含むがあります。 $\mathfrak{r}$ が A の左イデアルである場合、それは、A の一意の最大左イデアルです。これは、(i) が (iii) を意味することを証明します。

A が独自の最大左イデアル $\mathfrak{m}$ を持っていると仮定します。 $b\in A-\mathfrak{m}$に乗ります。左イデアル $Ab$ は A の最大左イデアルに含まれていないため、A (I, §8, No. 6, p. 104, 定理 1) に等しく、$b$ は反転可能です。すべての $a\in A$ に対して、元 $a$ と $1-a$ 属するの 1 つが A $-\mathfrak{m}$ になります。なぜなら、$\mathfrak{m}$ は含む 1 にならない理想だからです。したがって、(iii) は (v) を意味します。

性質 (v) が成り立つとします。 $b$ を A の左可逆元とします。 $c\in A$ を $cb= 1$ となるようにします。 $(1-bc)b= 0$ と $b\not= 0$ があります。したがって、$1-bc$ は可逆のままではありません。 性質 (v) までに、$bc$ は反転可能なままになり、なおさら、$c$ は反転可能なままになります。しかし、$c$ は反転可能です。 $b$ はその逆なので、$b$ は可逆です。したがって、(v) は (iv) を意味します。

(iv) が (i) を意味することを証明することはまだ残っています。 (iv) が成り立つと仮定します。この場合、$\mathfrak{r}$ は、次の主張 a) ～ d) による A の両側イデアルです。

a) 環 A は非零であるため、$0\in \mathfrak{r}$ となります。

b) A の 2 つの元のうち積、1 つは所属から $\mathfrak{r}$ まで、もう 1 つは A $-\mathfrak{r}$、属するから $\mathfrak{r}$ へ。

c) 集合 $\mathfrak{r}$ は加法で安定しています。

実際、$a$ と $b$ を $\mathfrak{r}$ の元として、$s=a+b$ が可逆であるとします。 b)により、属するから$\mathfrak{r}$の元$s^{-1}a$と$s^{-1}b$。 $s^{-1}b= 1-s^{-1}a$ 以降、この矛盾する仮定は (iv) が成り立ちます。

d) 集合 $\mathfrak{r}$ は乗法で安定しています。

実際、$a$ と $b$ を $\mathfrak{r}$ の 2 つの元とします。 b) により元 $a'=-a(1-b)$ 属するから $\mathfrak{r}$ となり、元 $ab$ は $a+a'$、c) により属するから $\mathfrak{r}$ に等しい。 主張 d) が続きます。

#### 定義 1 {#alg-viii-s2-def-1 .statement tag=001Q}

局所環は、命題 1 と同等の特性を持つ非零環です。

環 A は、反対環 $A^o$ がローカルである場合にのみローカルです。

A が局所環の場合、A の非可逆元の集合 $\mathfrak{r}$ は A の両面イデアルです。それは、含む A の左右すべてのイデアルが A に等しくないことです。環 $A/\mathfrak{r}$ は、従って、体であり、これを A の剰余体と呼びます。集合 $\mathfrak{r}$ は、A の一意の最大左 (それぞれ右、両側) イデアルです。 $\mathfrak{r}$ が A の最大の理想であると言うだけです。

#### 例 1 {#alg-viii-s2-n1-exa-1 .statement tag=001R}

すべての体は局所環です。

#### 例 2 {#alg-viii-s2-n1-exa-2 .statement tag=001S}

A を非零環とし、すべての元が可逆または零能であるとします。するとAは局所環になります。確かに、$a\in A$ が可逆でない場合、仮定までに、$a^{n+1}= 0$ となるような整数 $n\geqslant 0$ が存在し、$1-a$ は逆$1 +a+\cdots +a^n$ になります。

#### 例 3 {#alg-viii-s2-n1-exa-3 .statement tag=001T}

X を $C^r$ 多様体 (VAR、R、5.1.5) および X の $x$ 点とします。 $\mathscr{O}_x$ を、スカラー K の体の値で、$C^r$ 写像の $x$ における細菌の環とします。すると、$\mathscr{O}_x$ は可換局所環で、その最大理想は次のようになります。

$x.*$で零である写像の細菌

#### 例 4 {#alg-viii-s2-n1-exa-4 .statement tag=001U}

A を、A (III, §2, No. 11、p. 456) に係数が入った形式冪系列の可換局所環と $B = A[[X_i]]_{i\in I}$ 代数とします。 IV, §4, No. 4、p. 30、環の命題 6 により、B は局所的であり、その最大イデアルは、A の最大イデアルに定数項を伴う形式的な冪系列で構成されます。特に、A が体の場合、 $A[[X_i]]_{i\in I}$ は、正式な冪系列と定数項零で構成されます。

#### 例 5 {#alg-viii-s2-n1-exa-5 .statement tag=001V}

$p$ を素数数とします。 We denote by $\mathbf{Z}_{(p)}$ the subring of the field $\mathbf{Q}$ of rational numbers consisting of the fractions $a/b$ with $a\in \mathbf{Z},b\in \mathbf{Z}$, and $b$ not divisible by $p*$(cf. Comm. アルゴリズム、II, §2, No. 1、p. 60) 。 すると$\mathbf{Z}$は

$*(_{p)}$

可換局所環、最大理想$p\mathbf{Z}_{(p)}$。 $p$ 進数整数 (V, §12, No. 3、p. 96) の環 $\mathbf{Z}_p$ は可換局所環で、最大理想値 $p\mathbf{Z}_p$ (VIII、p. 40、練習問題 9) です。

#### 例 6 {#alg-viii-s2-n1-exa-6 .statement tag=001W}

K を特性 $p >0$ の可換体とし、G を $p$ グループ (I, §6, No. 5、p. 76、定義 9) とします。 K (III, §2, No. 6、p. 446) 上の群 G の代数 K[G] は局所環です。その最大の理想は、$\sum_{g\in G}a_g= 0$ (VIII, p. 41, 練習問題 10) となる K[G] の元 $(a_g)_{g\in G}$ の集合です。

### 2. ウェアーフィッティング分解

A を M の環、M A-加群、および $u$ 自己準同型とします。任意の整数 $p\geqslant 0$ について、$u^p$ の核を $N_p$ で表します。 部分加群 $(N_p)$ の数列は増加するで、その和集合は $u$ で安定している M の部分加群 $N_{\infty}$ です。 整数 $p\geqslant 0$ ごとに $N_{p+1}=\overset{-1}{u}(N_p)$ があり、関係 $N_p= N_{p+1}$ は $N_{p+1}= N_{p+2}$ を意味します。従って、数列 $(N_p)$ は真に増加するであるか、$N_0, . . . ,N_p$ と $N_p= N_{\infty}$ が異なるような整数 $p\geqslant 0$ が存在します。

任意の整数 $q\geqslant 0$ について、$u^q$ の像を $I_q$ で表します。 部分加群 $(I_q)$ の数列は減少するで、その共通部分は $u$ で安定している M の部分加群 $I_{\infty}$ です。 整数 $q\geqslant 0$ ごとに $u(I_q) = I_{q+1}$ があり、関係 $I_q= I_{q+1}$ は $I_{q+1}= I_{q+2}$ を意味します。その結果、数列 $(I_q)$ は真に減少するであるか、$I_0, . . . ,I_q$ と $I_q= I_{\infty}$ が異なるような整数 $q\geqslant 0$ が存在します。

#### 命題 2 {#alg-viii-s2-prop-2 .statement tag=001X}

a) 数列 $(N_p)$ が静止していると仮定します。次に、$N_{\infty}\cap I_{\infty}= 0$、$u$ から $I_{\infty}$ の制限は単射法、$N_{\infty}$ の $u$ 誘導する冪零自己準同型です。

b) 数列 $(I_p)$ が静止していると仮定します。すると、M = $N_{\infty}+ I_{\infty}$ と $u(I_{\infty}) = I_{\infty}$ が得られます。

c) (「Weyr–フィッティング分解」—ときどきを「フィッティング分解」と呼ぶ) 数列 $(N_p)$ と $(I_p)$ が静止していると仮定します。 この場合、M は $u$ の下で安定している部分加群 $N_{\infty}$ と $I_{\infty}$ の直和 、および $N_{\infty}$ の $u$ 誘導する冪零自己準同型と $I_{\infty}$ の自己同型です。

$p$ を $N_p= N_{\infty}$ となるように自然数とし、$v=u^p$ とします。 構成までに、$v$と$v^2$は同じ核$N_{\infty}$を持ち、$I_p$は$v$の像になります。 $N_{\infty}\cap I_p$ の $x$ には、$x=v(y)$ となるような $y\in M$ が存在し、従って $v^2(y) =v(x) = 0$ になります。従って、$y\in N_{\infty}$ があり、その結果、$x= 0$ になります。 特に$N_{\infty}\cap I_{\infty}= 0$があります。 Since the kernel $N_1$ of $u$ is contained in $N_{\infty}$, the restriction of $u$ to $I_{\infty}$ is injective; on the other hand, we have $u^p(N_{\infty}) = 0$. これは a) を証明します。

$q$ を $I_q= I_{\infty}$ となるように自然数とし、$w=u^q$ とします。すると、$w$と$w^2$は同じ像$I_{\infty}$を持ち、$N_q$は$w$の核になります。 $x\in M$ にしましょう。 $w(x)\in I_{\infty}$ があるので、$w(x) =w^2(y)$ のような $y\in M$ が存在します。次に、$x-w(y)\in N_q$、よって $M = N_q+ I_{\infty}$、なおさら $M = N_{\infty}+ I_{\infty}$ となります。 $u(I_{\infty}) =u(I_q) = I_{q+1}= I_{\infty}$があります。これは b) を証明します。

主張 c) は a) と b) の直後に続きます。

#### 注意 1 {#alg-viii-s2-n2-rem-1 .statement tag=001Y}

$p$ を整数として、$N_p= N_{p+1}$ とします。上の証明は、$u$から$I_p$の$N_{\infty}\cap I_p= 0$と制限が単射であることを示しています。同様に、$q$ を整数として、$I_q= I_{q+1}$ とします。次に、$N_q+ I_{\infty}= M$ があり、$u$ から移行によって商を推定した $M/N_q$ の自己準同型は全射です。

#### 注意 2 {#alg-viii-s2-n2-rem-2 .statement tag=001Z}

M が 2 つの部分加群 N と I の直和で、$u$ で安定しており、N の $u$ 誘導する冪零自己準同型 $u_N$ と I の自己同型であるとします。次に、$N_{\infty}= N$ と $I_{\infty}= I$ があり、数列 $(N_p)$ と $(I_p)$ は静止しています。さらに、次の整数は等しいです。

$\alpha )$ 整数 $p\geqslant 0$ $N_p= N_{\infty}$、

$\beta )$ 整数 $q\geqslant 0$ $I_q= I_{\infty}$、

$\gamma )$ 整数 $r\geqslant 0$ は $(u_N)^r= 0$ になります。

#### 注意 3 {#alg-viii-s2-n2-rem-3 .statement tag=0020}

The assumption of assertion a) is satisfied if the A-module M is Noetherian; the assumption of assertion b) is satisfied if M is Artinian; by Proposition 1 of VIII, p. 2, the assumption of assertion c) is satisfied if M has finite length.

#### 系 1 {#alg-viii-s2-prop-2-cor-1 .statement tag=0021}

Aを環、MをA-加群とします。

a) 加群 M がネーター の場合、M のすべての全射自己準同型は全単射です。

b) 加群 M がアルティンの場合、M のすべての単射詞自己準同型は全単射です。

c) 加群 M に有限長がある場合、M のすべての単射詞または全射自己準同型は全単射です。

d) 環 A が可換で、A-加群 M が有限生成される場合、M のすべての全射自己準同型は全単射です。

$u$ を A-加群 M の自己準同型とします。この小節の冒頭で紹介した記法を使用します。 自己準同型 $u$ が全射であれば、$I_{\infty}= M$ になります。 主張 a) は、命題 2、a) および注意 3 から続きます。同様に、自己準同型 $u$ が単射であれば、$N_{\infty}= 0$ が得られます。したがって、主張 b) は、命題 2、b) および注意 3 から続きます。 主張 c) は、a) および b) からすぐに続きます。

ここで、環 A が可換、A-加群 M が有限生成、自己準同型 $u$ が全射であるとします。 $u$ が単射であることを証明しましょう。 $x$ を $u(x) = 0$ となるような M の元とします。 A-加群 M の選ぶ有限生成家族 $(x_i)_{i\in I}$ と、M のすべての $i\in I$、元 $y_i$ について、$u(y_i) =x_i$ になります。 A には次のような家族 $(a_i)_{i\in I}, (b_{ij})_{(i,j)\in I\times I}$ と元の $(c_{ij})_{(i,j)\in I\times I}$ が存在します。

$$
x=\sum_{i\in I}a_ix_i,y_j=\sum_{i\in I}b_{ij}x_i,u(x_j) =\sum_{i\in I}c_{ij}x_i
$$

$j\in I$ごとに。 $A'$ を含む元 $a_i,b_{ij}$ および $c_{ij}$ (VIII, p. 12, 系 3) のネーター 部分環とします。 $M'$ を、ファミリー $(x_i)_{i\in I}$ によって生成された M の $A'$ サブモジュールとします。 $j\in I$ ごとに $u(x_j)\in M',y_j\in M'$ と $u(y_j) =x_j$ があります。したがって、$A'$ モジュール $M'$ の制限、全射自己準同型 $u'$ による $u$ 定義する。 環 $A'$ はネーター であるため、有限生成された $A'$ モジュール $M'$ はネーター (VIII, p. 7, 命題 4 a)) です。 a) により、$M'$ の自己準同型 $u'$ は全単射です。 構成、$x$ 属するから$M'$、そして$u'(x) =u(x) = 0$になります。したがって、$x= 0$ が得られ、これは d) を証明します。

#### 系 2 {#alg-viii-s2-prop-2-cor-2 .statement tag=0022}

左ネーター環では、左または右のすべての可逆元が反転可能です。

実際、$xy= 1$ となるような左ネーター環 A の元 $x,y$ を考えてみましょう。 A-加群 $A_s$ の自己準同型 $a\mapsto ax$ と $a\mapsto ay$ をそれぞれ $\boldsymbol{\delta }(x)$ と $\boldsymbol{\delta }(y)$ で表します。 $\boldsymbol{\delta }(y)\circ \boldsymbol{\delta }(x) = 1_{A_s}$ があります。したがって、$\boldsymbol{\delta }(y)$ は全射法です。 系 1 により、a)、$\boldsymbol{\delta }(y)$ は全単射です。 自己準同型 $\boldsymbol{\delta }(x)$ は、$\boldsymbol{\delta }(y)$ の逆全単射で、$yx= (\boldsymbol{\delta }(x)\circ \boldsymbol{\delta }(y))(1) = 1$ になります。 系が続きます。

### 3. 不分解加群と原始加群

A を環とします。次の定義 (VII, §4, No. 8、p. 23、定義 3) を思い出してください。

#### 定義 2 {#alg-viii-s2-def-2 .statement tag=0023}

A-加群 M は、0 および M と異なる部分加群族の直和ではない場合、非分解可能と呼ばれます。

By the corollary of Proposition 12 of II, §1, No. 8, p. 209, the following properties are equivalent:

a) A-加群 M は不分解です。

b) A-加群 M は非零であり、M のすべての直和因子部分加群は 0 または M に等しい。

c) A-加群 M は非零であり、環 End$_A(M)$ 含む 0 と $1_M$ から区別されるべき等はありません。

特に、A-加群 $A_s$ の自己準同型環は A の反対環と同型であるため、環 A が非零であり、べき等が 0 と 1 である場合に限り、A-加群 $A_s$ は分解不可能であることがわかります。

#### 例 {#alg-viii-s2-n3-exa-1 .statement tag=0024}

環 A が主イデアル整域であるとします。分解不可能な有限生成A-加群は、A または $A/p^nA$ のいずれかと同型の A-加群です。ここで、$p$ は A の既約元および $n$ 整数 $>0$ (VII, §4, No. 8、p. 24、命題 8) です。

#### 命題 3 {#alg-viii-s2-prop-3 .statement tag=0025}

ネーター またはアルティン A-加群 M は、分解不可能な部分加群の有限族の直和です。

まず、M のすべての非零部分加群 P には分解不可能な直因子があることを証明しましょう。 If this were not the case, then every direct factor submodule of P would be decomposable; proceeding by induction, we could then construct, for every $n\in \mathbf{N}$, nonzero submodules $N'_n$ and $N''_n$ of P such that $P = N'_0\oplus N''_0$ and $N'_{n-1}= N'_n\oplus N''_n$ for $n\geqslant 1$. しかし、その場合、部分加群 $N''_0+\cdots + N''_n$ の数列は真に増加するになり、部分加群 $N'_n$ の真に減少するになります。 加群 M は、仮定とは反対に、ネーター でもアルティンでもありません。

さて、M が分解不可能な部分加群の有限族の直和ではないと仮定します。 By induction, we construct indecomposable submodules $P''_n$ of M and nonzero submodules $P'_n$ of M for every $n\in \mathbf{N}$ such that $M = P'_0\oplus P''_0$ and $P'_{n-1}= P'_n\oplus P''_n$ for $n\geqslant 1$. 確かに、M は非零で、証明の最初の部分を P = M に適用すると、$P'_0$ と $P''_0$ が得られます。 加群 $P'_k$ と $P''_k$ が $k < n$ に対して定義されているため、証明の最初の部分によって、 $P'_{n-1}= P'_n\oplus P''_n$ と $P''_n$ が分解不可能となるような部分加群 $P'_n$ と $P''_n$ が存在します。 関係 $M = P'_n\oplus P''_0\oplus  \cdots  \oplus P''_n$ は、M が分解不可能な加群の有限族の直和ではないため、$P'_n\not= 0$ を意味します。

部分加群 $P''_0\oplus  \cdots  \oplus P''_n$ の数列は真に増加する、部分加群 $P'_n$ の数列は真に減少するです。この矛盾する仮定の M はネーター またはアルティンです。

加群の分解の一意性を分解不可能な部分加群の直和として扱う問題は、次の小節で学習します。

#### 定義 3 {#alg-viii-s2-def-3 .statement tag=0026}

自己準同型環がローカルである場合、加群は原始[^1] と呼ばれます。

定義によって、局所環は 0 に減りません。従って、原初の加群は非零になります。さらに、A-加群 $A_s$ は、環 A がローカルである場合に限り、原始的です。

#### 命題 4 {#alg-viii-s2-prop-4 .statement tag=0027}

a) 根源的な加群は分解不可能です。

b) 有限長の不分解な加群は根源的である。

M をA-加群とします。 M が原始的であると仮定します。 $e$ を局所環 End$_A(M)$ の冪等とします。 $e^2=e$ なので、$e$ が可逆で $e= 1$ になるか、$1-e$ が可逆で $e= 0$ になります。これは、M が分解不可能であることを証明します (VIII, p. 30)。

さて、M が分解不可能で、有限長であると仮定します。 命題 2、c) VIII、p. 27 により、M のすべての自己準同型は可逆または零能です。従って、環 End$_A(M)$ は、VIII、p. 26 の例 2 によってローカルです。

$\mathbf{Z}$ モジュール $\mathbf{Z}$ は分解不可能ですが、ネーター は分解できませんが、アルティンは分解できません。その自己準同型環は $\mathbf{Z}$ と同型であるため、ローカルではありません。従って、$\mathbf{Z}$ は原始的な $\mathbf{Z}$ モジュールではありません。

$*$$p$を素数数とします。 $\mathbf{Z}$ モジュール $\mathbf{Q}_p/\mathbf{Z}_p$ の自己準同型環は、局所環 $\mathbf{Z}_p$ (cf. VII, §4, p. 65, 練習問題 13) と同型です。従って、これは原始的な $\mathbf{Z}$ モジュールです。

単射詞加群は、それが原始的 (X, §1、n$^o9$、p. 21、命題 $14$)$.*$ である場合に限り、分解不可能です。

### 4. 半原始加群

#### 定義 4 {#alg-viii-s2-def-4 .statement tag=0028}

加群が原始部分加群の族の直和である場合、加群は半原始と呼ばれます。

#### 例 1 {#alg-viii-s2-n4-exa-1 .statement tag=00SE}

$*$すべての単純加群は原始 (VIII、p. 45) です。従って、すべての半単純加群は半原始的です (VIII、p. 55、定義 1)。

#### 例 2 {#alg-viii-s2-n4-exa-2 .statement tag=01L7}

A が左ネーター環の場合、すべての単射詞 A-加群は半原始的です (X, §1、n$^o9$、p. 21、命題 14 および X, §1、n$^o10$、p. 22、定理 3、 b)).$*$

#### 定理 1 (東谷) {#alg-viii-s2-thm-1 .statement tag=00RX}

Aを環、Lを原始A-加群、Mを半原始A-加群とする。 [M : L] で示される固有の基数が存在し、次の性質が含まれます。

原始加群の直和としての M のすべての分解 $M =\bigoplus_{i\in I}M_i$ に対して、$M_i$ が L と同型であるような添字 $i\in I$ の集合は基数 [M : L] になります。

証明は以下の4つの補題をもとにしています。

#### 補題 1 {#alg-viii-s2-lem-1 .statement tag=0029}

M を M の A-加群、$M'$ 原始部分加群、$M'$ を補足する M の $M''$ 部分加群とする。 $u$ を M の自己準同型とします。次に、$M''$ を補足する M の $M'$ から部分加群までの $u$ または $1_M-u$ 誘導する同型です。

$p$をMから核と$M''$を伴う$M'$への射影とし、$v$を$p\circ u$から$M'$の制限とします。まず、$v$が$M'$の自己同型であるとします。 $v$は単射なので、$u$から$M'$の制限は単射で、$u(M')\cap M''= 0$が得られます。 $v$は全射なので、$u(M')\oplus M''= M$になります。その結果、M の $M''$ を補う $M'$ から部分加群までの $u$ 誘導する同型が、$v$ が $M'$ の自己同型ではないとします。すると、$M'$が原始なので、$1_{M'}-v$は$M'$の自己同型になります。さて、$1_{M'}-v$は$p\circ (1_M-u)$から$M'$の制限です。前の推論は、$M''$を補うMの$M'$から部分加群まで$1_M-u$誘導する同型であることを証明しています。

#### 補題 2 {#alg-viii-s2-lem-2 .statement tag=002A}

Mを原始部分加群の家族$(M_i)_{i\in I}$の直和であるA-加群とし、$u$をMの自己準同型とする。Iの部分集合Jごとに集合$v= 1_M-u$と$M_J=\bigoplus_{i\in J}M_i$とする。次に、次の 2 つのうちの 1 つ性質が成り立つ:

a) M の $M_i$ から直和因子部分加群まで $u$ 誘導する同型となる添字 $i\in I$ が存在します。

b) $M_J$ から部分加群までの I$,v$ 誘導する同型の有限部分集合 J ごとに、$M_{I-J}$ を補足します。

性質 b) が成り立つ場合、$v$ は単射法です。

性質 a) が成り立たないと仮定して、J の基数上の帰納法によって性質 b) を確立しましょう。$J =\emptyset$ であれば証明するものは何もありません。従って、J は J の空でない、選ぶ元 $i$、集合 $J'= J-\{i\}$ であるとします。 帰納法の仮定、$v$ 誘導する同型 $M_{J'}$ から部分加群まで、$M_{I-J'}= M_{I-J}\oplus M_i$ を補足します。従って、部分加群 $M''=v(M_{J'})\oplus M_{I-J}$ は $M_i$ を補足します。 $u$の補題1と仮定までに、$M''$を補足するMの$M_i$から部分加群までの自己準同型$v$誘導する同型。従って、$v$ 誘導する同型 $M_J= M_i\oplus M_{J'}$ から部分加群は、$M_{I-J}$ を補足します。

最後の主張は、M が部分加群 $M_J$ の和集合であるという事実から導き出され、J は I の有限部分集合を通過します。

#### 補題 3 {#alg-viii-s2-lem-3 .statement tag=002B}

M を A-加群、つまり原始部分加群の家族 $(M_i)_{i\in I}$ の直和とし、$p$ を M の非零射影子とします。 $p$ 誘導するとなるような添字 $i\in I$ が存在します。 $p(M)$の$M_i$から直和因子部分加群までの同型。

$p$ は非零であるため、$1_M-p$ は単射ではありません。 補題 2 までに、M の $M_i$ から直和因子部分加群まで $p$ 誘導する同型となる添字 $i\in I$ が存在します。M のすべての射影子には像 $p(M_i)$ が付きます定義する、制限により、$p(M)$ の射影子と像 $p(M_i)$ により、$p(M_i)$ は $p(M)$ の直和因子部分加群になります。

#### 補題 4 {#alg-viii-s2-lem-4 .statement tag=002C}

MをA-加群、つまり原始部分加群の家族$(M_i)_{i\in I}$の直和、Lを原始A-加群、NをMの直和因子部分加群とします。Nが家族$(N_j)_{j\in J}$の直和であると仮定します。 部分加群は L と同型であり、添字 $i\in I$ の $I_L$ 集合で表され、$M_i$ は L と同型です。次に、

(1) カード(J) $\leqslant$ カード(I$_L$)。

$N_0$ を N を補足する M の部分加群とします。 加群 M は、$N_0$ と族 $(N_j)_{j\in J}$ の直和です。すべての $j\in J$ について、M の像 $N_j$ をこの分解 (II, §1, No. 8、p. 209、命題 12) に関連付けて、M の $p_j$ 射影子で表します。すべての $i\in I$ について、$M_i$ から $N_j$ までの$p_j$ 誘導する同型のように、添字 $j\in J$ の $J(i)$ 集合で表します。この集合は有限です。実際、$x$ が $M_i$ の非零元で、K が J の有限部分集合で、$x$ 属するから $N_0+\sum_{k\in K}N_k$ となる場合、次の式は $p_j(x) = 0$ になります。 $j\in J$- K なので、K には $J(i)$ が含まれます。

$j\in J$ にしましょう。 補題 3 までに、$N_j$ の $M_i$ から直和因子部分加群まで $p_j$ 誘導する同型となる添字 $i\in I$ が存在します。 $M_i$ は非零で、$N_j$ は原始的であるため分解不可能 (VIII、p. 31、命題 4) なので、$p_j(M_i) = N_j$、$j$ 属するが得られます。 $J(i)$。 加群 $M_i$ は $N_j$ 、つまり L と同型であるため、添字 $i$ 属するは $I_L$ となります。これは、J が有限族集合 $(J(i))_{i\in I_L}$ の和集合であることを証明します。 集合 J が無限大の場合、集合 $I_L$ は無限大となり、(集合理論, III, §6, No. 3, p. 188, 系 3) となります。

カード(J)$\leqslant \sum_{i\in I_L}$カード(J($i$))$\leqslant$カード(I$_L$)。

さて、集合 J が有限であると仮定し、J の基数上の帰納法によって補題を証明しましょう。 J が空の場合、証明できるものは何もありません。 したがって、J を空でないとし、J の選ぶ元 $j$ とします。 以上により、$M_i$から$N_j$まで$p_j$誘導する同型となる添字$i\in I_L$が存在します。 集合 $I'= I-\{i\}$ と $J'= J-\{j\}$。 加群 M は、$M_i$ の直和と $p_j$ の核です。 $M_i$ と部分加群 $M'=\oplus_{i'\in I'}M_{i'}$ の直和でもあります。 したがって、Ker $p_j= N_0\oplus_{j'\in J'}N_{j'}$ から $M'$ まで (命題 13 の II, §1, No. 9、p. 210、系) 同型 $\varphi$ が存在します。 集合 $N'=\varphi (\sum_{j'\in J'}N_{j'})$。 $M'$ の部分加群 $N'$ は直因子であり、原始部分加群のファミリー $(\varphi (N_{j'}))_{j'\in J'}$ の直和は L と同型です。 帰納法の仮定を $M'$ と $N':$ に適用すると、Card(J$'$)$\leqslant$ Card(I$_L-\{i\}$) があるため、不等式 (1) となります。

定理 1 を証明してみましょう。 $(M_i)_{i\in I}$ と $(N_j)_{j\in J}$ を直和 M を持つ 2 つの原始部分加群族とします。 $I_L$ (それぞれ $J_L$) を $i\in I$ (それぞれ $j\in J$) の集合とします。 $M_i$ (それぞれ $N_j$) は L と同型です。 補題 4 による Card(J$_L$)$\leqslant$ Card(I$_L$) があります。 I と J の役割交換することにより、逆数不等式が得られ、したがって定理が得られます。

定理 1 で定義された基数 [M : L] は、M では L の原始多重度と呼ばれます。

#### 系 1 {#alg-viii-s2-lem-4-cor-1 .statement tag=002D}

M と N を半原始加群とします。したがって、すべての原始加群 L に対して [M : L] = [N : L] である場合に限り、M と N は同型です。

#### 系 2 {#alg-viii-s2-lem-4-cor-2 .statement tag=00QY}

M を半原始加群とします。 $(M_i)_{i\in I}$ と $(M'_j)_{j\in J}$ を次のような M の原始部分加群の家族とする

$$
M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j
$$

次に、M の自己同型 $u$ と I から J までの全単射 $\varphi$ が存在し、$i\in I$ ごとに $u(M_i) = M'_{\varphi(i)}$ が存在します。

任意の原始加群 L について、$I_L$ (それぞれ $J_L$) を添字 $i\in I$ (それぞれ $j\in J$) の集合とし、$M_i$ (それぞれ $M'_j$) がL。 空でない集合の形 $I_L$ (それぞれ $J_L$) 形分割の I (それぞれ J)、そしてすべての L について、

カード(I$_L$) $=$ カード(J$_L$) $= [M : L]$;

系が続きます。

#### 系 3 {#alg-viii-s2-lem-4-cor-3 .statement tag=002E}

M、N、P を半原始加群とします。 $M\oplus P$ が $N\oplus P$ と同型であり、[P : L] がすべての原始加群 L に対して有限であると仮定します。この場合、M と N は同型です。

仮定までに、

[M : L] + [P : L] = [N : L] + [P : L]

すべての原初の加群 L に対して。 [P : L] は有限であるため、(集合理論, III, §3, No. 4, p. 162, 命題 8) から帰納法が続き、すべての原始関数に対して [M : L] = [N : L] が得られます。 加群 L。したがって、加群 M と N は系 1 と同型です。

#### 系 4 {#alg-viii-s2-lem-4-cor-4 .statement tag=002F}

M と N を半原始加群とします。 $M^d$ が $N^d$ と同型となる整数 $d >0$ が存在するとします。この場合、加群 M と N は同型です。

Lを原始加群とします。 仮定までに、

$$
d[M : L] =d[N : L]
$$

したがって、等式 [M : L] = [N : L] となります。実際、無限の基数 $\mathfrak{a}($集合理論, III, §6, No. 3, p. 188 に対して、$d\mathfrak{a}=\mathfrak{a}$ が得られます。 系 4）。 加群 M と N は系 1 によって同型になります。

#### 系 5 {#alg-viii-s2-lem-4-cor-5 .statement tag=002G}

M を原始部分加群の有限族 $(M_i)_{i\in I}$ の直和である半原始加群とします。 I の部分集合 J には、$M_J=\bigoplus_{i\in J}M_i$ と書き込みます。 N を M の直和因子部分加群とします。

a) $M_J$ が N を補足する部分加群となるような I の部分集合 J が存在します。

b) J を I の部分集合とします。 $M_J$ が N の補足である場合、加群 N は $M_{I-J}$ と同型であり、半原始的です。

$N\cap M_i= 0$ となるような添字 $i\in I$ を K 集合で表します。 K の基数に帰納法を用いるを当てはめてみましょう。M = N であれば、系は明らかです。$M\not= N$ と仮定します。 $p$ を核 N を持つ M の射影子とします。その像を P で表します。それは非零であり、補題 3 により、$p$ 誘導するとなる$j\in I$ が存在します。 Pの$M_j$から直和因子部分加群まで同型です。$N\cap M_j= 0$がございます。 集合 $N'= N\oplus M_j$。 $N'= N\oplus p(M_j)$ あります。 P の $p(M_j)$ を補足する部分加群は M の $N'$ も補足するので、$N'$ は M の直和因子部分加群になります。 添字の $i\in I$ の集合は、$N'\cap M_i= 0$ が K に含まれるようになります。 $-\{j\}$。 帰納法の仮定までに、$M_{J'}$ が M の $N'$ を補う部分加群となるように、I の部分集合 $J'$ が存在します。集合 $J = J'\cup  \{j\}$。すると、$M_J$ は M の N を補う部分加群になります。

J を I の部分集合とし、$M_J$ が N の M を補足する部分加群であるとします。$M_J$ も $M_{I-J}$ を補足するため、加群 N と $M_{I-J}$ は同型であり、N は半原始的です。

#### 系 6 {#alg-viii-s2-lem-4-cor-6 .statement tag=002H}

局所環を超えるすべての有限生成射影加群は無料です。[^2]

Aを局所環とします。 A-加群 $A_s$ は原始的 (VIII、p. 31) です。 M が有限生成射影 A-加群である場合、A-加群 N と自然数 $n$ が存在し、$M\oplus N$ は $A^n_s$ (II, §2, No. 2, p. 232, 系 1) と同型になります。 系 5 から、加群 M 自体は、整数 $m$ に対して $A^m_s$ と同型であるため、$0\leqslant m\leqslant n$ は自由であることがわかります。

#### 注意 {#alg-viii-s2-n4-rem-1 .statement tag=002I}

M と $M'$ を半原始的な A-加群とします。 VIII, p. 33 の補題 4 から、すべての原始 A-加群 L に対して $[M': L]\leqslant [M : L]$ がある場合に限り、$M'$ は M の直和因子部分加群と同型であることがすぐにわかります。特に、L が原始 A-加群である場合、[M : L] は基数 $\mathfrak{a}$ の最大のであり、これに対して $L^{(\mathfrak{a})}$ と同型の M の直和因子部分加群が存在します。

したがって、関係 [M : L] = 0 は、L と同型の M の直和因子部分加群が存在しないことを意味します。これは、L と同型の M の部分加群の存在を除外するものではありません。 例ここで、$A =\mathbf{Z}, L =\mathbf{Z}/2\mathbf{Z}$ と $M =\mathbf{Z}/4\mathbf{Z}:$ 、$\mathbf{Z}$ 加群 L および M は原始的で同型ではないため、[M : L] = 0 および L は以下と同型であることを考慮するだけで十分です。 M の部分加群 $2\mathbf{Z}/4\mathbf{Z}$

### 5. 構造/加群/有限長

#### 定理 2 (クルル–レマック–シュミット) {#alg-viii-s2-thm-2 .statement tag=00RY}

Aを環、Mを有限長のA-加群とします。

a) $M =\bigoplus_{i\in I}M_i$ となるような M の分解不可能な部分加群の有限族 $(M_i)_{i\in I}$ が存在し、加群 M は半原始的です。

b) $(M_i)_{i\in I}$ と $(M'_j)_{j\in J}$ を、$M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j$ となるような M の分解不可能な部分加群の 2 つの有限族とする。 I から J までの全単射 $\sigma$ と M の自己同型 $u$ が存在し、$i\in I$ ごとに $u(M_i) = M'_{\sigma(i)}$ が存在します。

c) N を M の直和因子部分加群とし、$(M_i)_{i\in I}$ を直和 M をもつ M の分解不可能な部分加群の有限族とする。 $\bigoplus_{i\in I-J}M_i$ が N を補うような I の部分集合 J が存在する。 加群 N は以下と同型である。 $\bigoplus_{j\in J}M_j$。

d) N をA-加群とします。 加群 $M^d$ と $N^d$ が同型であるような整数 $d >0$ が存在する場合、加群 M と N は同型です。

e) N と P を有限長の A-加群とする。 加群 $M\oplus P$ と $N\oplus P$ が同型である場合、M と N は同型です。

有限長の加群は、アルティンとネーター の両方です (VIII、p. 2、命題 1)。さらに、有限長の加群については、分解不可能または原始的であることは同じ意味になります (VIII、p. 31、命題 4)。 主張 a) は、命題 VIII、p. 30 の 3 から続きます。 主張 b)、c)、および e) は、それぞれ、定理 1、VIII、p. 32 の系譜 2、5、および 3 から導き出されます。最後に、主張 d) は、VIII の系 4、p. 35 から続きます。これは、d) の仮定の下で、加群 N は有限長を持ち、したがって a) によって半原始的であるためです。

#### 定理 3 {#alg-viii-s2-thm-3 .statement tag=002J}

Kを可換体、AをK-代数、MとNを有限長の加群とする。 $A_{(K')}$ 加群 $M_{(K')}$ と $N_{(K')}$ が同型となるように、$K'$ を非零可換K-代数とします。この場合、A-加群 M と N は同型です。

a) まず、代数 $K'$ が K 上で有限次数 $d$ を持つとします。そのとき、A-加群 $M_{(K')}$ は $M^d$ と同型で、A-加群 $N_{(K')}$ は $N^d$ と同型です。 A-加群 $M^d$ と $N^d$ は同型です。 定理 2 より、d)、A-加群 M と N は同型です。

b) さて、有限個の元から K-代数 $K'$ が生成されるとします。 選ぶ $K'$ の最大理想$\mathfrak{m}$、および集合 $K''= K'/\mathfrak{m}$。ヒルベルトのヌルステレンザッツ (VIII, p. 462, 系 1 of 定理 1)$, K''$ は、K の有限次数拡大により、$K'$ からのスカラーの拡大により、 $K''$ まで、$A_{(K')}$-線形同型 $M_{(K')}\rightarrow N_{(K')}$ から $A_{(K'')}$-線形同型 $M_{(K'')}\rightarrow N_{(K'')}$ を推定します。 証明の部分 a) により、A-加群 M と N は同型です。

c) 最後に、一般的なケースを扱いましょう。 $u: M_{(K')}\rightarrow N_{(K')}$ を $A_{(K')}$ モジュールの同型と $v: N_{(K')}\rightarrow M_{(K')}$ 逆同型とします。有限多数の元によって生成される K-部分代数の $K'$ の $\mathscr{E}$ 集合で表します。 E がそのような部分代数である場合、$A_{(E)}$ は $A_{(K')}$ の部分環と識別され、$M_{(E)}$ と $N_{(E)}$ はそれぞれ $M_{(K')}$ と $N_{(K')}$ の $A_{(E)}$ サブモジュールと識別されます (II, §7, No. 7, p. 306);さらに、$M_{(K')}$ と $N_{(K')}$ は、それぞれ、右方向の家族 $(M_{(E)})_{E\in\mathscr{E}}$ と $(N_{(E)})_{E\in\mathscr{E}}$ の和集合です。 A-加群 M と N は有限長であるため、有限に生成されます。 S を A-加群 M の有限生成部分集合とし、T 有限生成部分集合 A-加群 N とする。$s\in S$ ごとに $u(1\otimes s)\in N_{(E)}$ が得られるように、K-代数 $E\in \mathscr{E}$ が存在する。 $t\in T$ごとに$v(1\otimes t)\in M_{(E)}$。線形性により、$u(M_{(E)})\subset N_{(E)}$ と $v(N_{(E)})\subset M_{(E)}$ が得られます。 写像 $u$ と $v$ その後、$M_{(E)}$ から $N_{(E)}$ まで、$N_{(E)}$ から $M_{(E)}$ まで誘導する逆全単射となります。これらの全単射は明らかに $A_{(E)}$ 線形です。したがって、$A_{(E)}$ モジュール $M_{(E)}$ と $N_{(E)}$ は同型です。 部分 b) の証明, A-加群により、M と N は同型です。

#### 注意 {#alg-viii-s2-n5-rem-1 .statement tag=002K}

E と F を可換体 K 上の 2 つの有限次元ベクトル空間とし、$K'$ を K の拡大とします。 $u$ を E の自己準同型と F の $v$ 自己準同型とし、$u_{(K')}$ と $v_{(K')}$ をスカラーの拡大で得られた $E_{(K')}$ と $F_{(K')}$ の自己準同型とします。 VII, §5, No. 3、p. 32 の系 1 と 2 から、自己準同型 $u$ と $v$ は、自己準同型 $u_{(K')}$ と $v_{(K')}$ が類似する場合に限り、類似することがわかります。 これは、上記の定理 3 を代数 A = K[X] と A-加群 $M = E_u$ および $N = F_v$ (VII, §5, No. 1, p. 29) に適用した結果にもなります。

### 練習問題 {#alg-viii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。

[^1]: Note added in translation: some authors use the terminology “module with local endomorphism ring” for “primordial module.”
[^2]: It can be shown that every projective module over a local ring is free (VIII, p. 42, Exercise 18).
