---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 1
section_title: Krull domains
lang: ja
source: ac-i-vii
book_pages: 475-493, 545-555
pdf_pages: 0493-0511, 0563-0573
extraction: ocr
subsections:
    - "no": 1
      title: DMSORIAL IDEALS OF AN INTEGRAL DOMAIN
      page: 475
      pdf_page: 493
    - "no": 2
      title: THE MONOID STRUCTURE ON D(A)
      page: 478
      pdf_page: 496
    - "no": 3
      title: KRULL DOMAINS
      page: 480
      pdf_page: 498
    - "no": 4
      title: ESSENTIAL VALUATIONS OF A KRULL DOMAIN
      page: 482
      pdf_page: 500
    - "no": 5
      title: APPROXIMATION FOR ESSENTIAL VALUATIONS
      page: 484
      pdf_page: 502
    - "no": 6
      title: PRIME IDEALS OF HEIGHT 1 IN A KRULL DOMAIN
      page: 485
      pdf_page: 503
    - "no": 7
      title: 'APPLICATION: NEW CHARACTERIZATIONS OF DISCRETE VALUATION RINGS'
      page: 487
      pdf_page: 505
    - "no": 8
      title: THE INTEGRAL CLOSURE OF A KRULL DOMAIN IN A FINITE EXTENSION OF ITS FIELD OF FRACTIONS
      page: 487
      pdf_page: 505
    - "no": 9
      title: POLYNOMIAL RINGS OVER A KRULL DOMAIN
      page: 488
      pdf_page: 506
    - "no": 10
      title: DIVISOR CLASSES IN KRULL DOMAINS
      page: 489
      pdf_page: 507
statements: 41
exercises: 32
content_sha256: dd80eff78813566bc237f0f3720b707dffc1c214ae81a89ad2900582f3e0b028
translated_from: content/en/ac/VII/01_s1_krull_domains.md
translation_method: google
source_content_sha256: c7f552328385d94715aa4fc98b5c4522cc8ad73080a081dd41bebfb79b236ea5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: d25d7769c4ca50462d1374bdb1197f90a9bfdd73069fcfd9a5b5399e257939ac
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. クルールドメイン

### 1. 整域の Dmsorial の理想

#### 定義 1 {#ac-vii-s1-def-1 .statement tag=04YL}

$A$ を整域とし、$K$ を分数の体とします。 $A$ に元 $d \neq 0$ が存在するような $K$ のすべてのサブ A モジュール $a$ は、$da \subset A$ が $A$ (または言葉の乱用により $K$) の分数イデアル $\mathfrak{d}$ と呼ばれます。

有限生成されたすべてのサブ A モジュール $K$ の $a$ は分数イデアルです。つまり、$(a_i)_{1 \leq i \leq n}$ が $a$ の生成元の系である場合、$a_i = b_i/d_i$ と書くことができます。ここで、$b_i \in A$、$d_i \in A$、 $d, \neq 0$; $d = d_1 \ldots d_n$なら、明らかに$da \subset A$。特に、$K$ の単次サブ A 加群は分数イデアルです (代数、章 VI, § 1, no. 5 では分数主イデアルと呼ばれたことを思い出してください)。 $A$ がネーター である場合、すべての分数イデアルは無限に生成されます A-加群。 $A$ の分数イデアルのすべてのサブ A モジュールは分数イデアルです。 $A$ のすべての理想は分数の理想です。混乱を避けるために、これらは $A$ の積分理想とも呼ばれます。

$A$ の非ゼロ分数イデアルを $I(A)$ 集合で表します。 $I(A)$ の 2 つの元 $a, b$ が与えられると、関係 「すべての分数主イデアル含む $a$ も含む $b$」に対して $a \prec b$ (または $b \succ a$) と書くことになります。明らかに、この関係は$I(A)$の予約注文です。 $R$ は、関連する同値関係 「$a \prec b$ および $b \prec a$」 (集合理論、章 III, § 1, no. 2) および $D(A)$ 商集合を表すものとします。 $I(A)/R$; $D(A)$の元は$A$の因子であり、すべての分数イデアル$a \in I(A)$について、$D(A)$の$a$の標準像を$\operatorname{div} a$（または$\operatorname{div}, a$）で表すものとします。 $\operatorname{div} a$ は $a$ の因子 $\mathfrak{d}$ であると言うでしょう。 $a = Ax$ が分数主イデアルの場合、div(Ax) の代わりに div(x) と書き、div(x) は x の因子と呼ばれます。 形 div(x) の D(A) の元をプリンシパル因子と呼びます。 商を取ると、I(A) 定義するの事前順序付け $\prec$ が D(A) で$\leqslant$ で示される順序になります。

すべての $a \in I(A)$ に対して、仮定までに、$a \subset Ad - 1$ となるような A のいくつかの $d \neq 0$ が存在します。したがって、分数主イデアル含む a の共通部分 $\tilde{a}$ は、I(A) の元です。明らかに、関係 $a \prec b$ は関係 $\tilde{a} \supset 6$ と同等です。したがって、関係 $a \supset b$ は $a \prec b$ を意味します。 I(A) の 2 つの元 $a, b$ が等価な法 R であるためには、$\tilde{a} = 6$ であることが必要かつ十分です。

#### 定義 2 {#ac-vii-s1-def-2 .statement tag=04YM}

*$a = \tilde{a}$ となるようなI(A) の各元 a を A の約分数イデアルと呼びます。*

他の語では、除数イデアルは、分数主イデアルの空ではない族の単なる非ゼロ共通部分です。ゼロ以外のすべての除数イデアル共通部分は除数イデアルです。 a が除数である場合、すべての $x \in K^*$、写像 $b \mapsto bx$ は、それ自体に対する分数主イデアルの集合の全単射であり、すべての $a \in I(A)$ について、6 は最小除数イデアル含む a であり、法 R と等価です。 $b$ はモジュロ R に相当する除数イデアルであり、その後 $\tilde{a} = 6 = b$ になります。したがって、5 は div $a =$ div $b$ となるような固有の除数イデアル $b$ です (他の語、制限の写像 $a \mapsto$ div $a$ から集合は単射法です)。

a と b を K の 2 つの分数イデアルとします。(章 I, § 2, no. 10) を思い出してください。$b : a$ は $xa \subset b$ となる $x \in K$ の集合を示します。これは明らかに A-加群です。 $b \in I(A)$ と $a \in I(A)$ の場合、$b : a \in I(A)$;たとえば、$d$ が A の非ゼロ元で、$db \subset A$ と $da \subset A$ であり、$a$ が $A \cap a$ の非ゼロ元である場合、$da(b : a) \subset A$ です。一方、$b \neq 0$ 属するから $b$ の場合、$bda \subset b$、したがって $bd \in b : a$ と $b : a \neq 0$ になります。

$b : a$ の定義は次のように書くこともできます。

$$
(1) \quad b : a = \bigcap_{x \in a, x \neq 0} b x^{-1}.
$$

#### 命題 1 {#ac-vii-s1-prop-1 .statement tag=04YN}

(a) *b が約数イデアルで、$a \in I(A)$ が約数である場合、$b : a$ は約数です。*

(b) ※I(A)にa,bを入れます。 位数の div $a =$ div $b$ では、$A : a = A : b$ であることが必要十分です。*

(c) *$a \in I(A)$、$6 = A : (A : a)$ のすべてに適用されます。*

主張 (a) は、$b$ が除数である場合、すべての $x \neq 0$ に対して $b x^{-1}$ となるため、式 (1) から直接得られます。

(b) を示すために、$P(a)$ が分数主イデアル含む a の集合を表すものとします。 関係 $Ax \in P(a)$ は $x^{-1} a \subset A$ と同等なので、$x^{-1} \in A : a$ と同等です。 関係 div $a =$ div $b$ は定義だけ$P(a) = P(b)$ に相当するので、$A : a = A : b$ にも相当します。

最後に$a(A : a) \subset A, a \subset A : (A : a)$として。この公式では、置き換えること $a$ が $A : a$ によって、$A : a \subset A : (A : (A : a))$ であることがわかります。一方、関係 $a \subset A : (A : a)$ は、次のことを意味します。
$$
A : a \supset A : (A : (A : a)).
$$
したがって $A : a = A : (A : (A : a))$ となり、(b) から $\operatorname{div} a = \operatorname{div}(A : (A : a))$ となります。
$A : (A : a)$ は (a) で約数なので、確かに $6 = A : (A : a)$ となり、(c) が証明されます。

#### 注意 {#ac-vii-s1-n1-rem-1 .statement tag=04YO}

上記の証明の過程で、すべての理想 $a \in I(A)$ に対して $A : a = A : (A : (A : a))$ であることが証明されました。これは *集合理論*、章 111、§ 1, no. 5、命題 2 の特殊なケースです。

#### 命題 2 {#ac-vii-s1-prop-2 .statement tag=04YP}

(i) *$D(A)$ では、上に境界のある空でないすべての集合には、少なくとも上界が許可されます。より正確には、$(a_i)$ が上に境界のある $I(A)$ の元の空ではない族である場合、*
$$
\sup(\operatorname{div} a_i) = \operatorname{div}\left( \bigcap_i 5_i \right).
$$
(ii) *$D(A)$ では、下に境界のある空でないすべての集合が最大の下界を許可します。より正確には、$(a_i)$ が下に境界のある $I(A)$ の元の空ではない族である場合、*
$$
\inf(\operatorname{div} a_i) = \operatorname{div}\left( \sum_i a_i \right).
$$
(iii) *集合 $D(A)$ は格子です。*

$(a_i)$ を、上で境界のある $I(A)$ の元の空でない族とする。分割理想 $b$ が上記のこの家族を制限していると言うのは、というがすべての $a_i$ に含まれている、つまり $b$ が $\bigcap_i 6_i$ に含まれているということになります。したがって、$\bigcap_i a_i \neq (0)$ と $\bigcap_i 6_i$ は、(i) を示す除算イデアルです。

ここで、$(6_i)$ を、下に境界がある $I(A)$ の元の空ではない族とします。除数的理想 $b$ が以下のこの族を制限すると言うことは、それが含むすべての $a_i$ であること、つまり ($b$ は除数的であるため) 含むすべての $a_i$ であるか、あるいは $b \supset \sum_i a_i$ であることを意味します。これは(ii)を証明します。

最後に、(iii) を証明するには、(i) と (ii) によって、$a, b$ が $I(A)$ にある場合、集合 $\{a, b\}$ は $I(A)$ の上下両方で有界であることを証明できれば十分です。現在は、その上が $a \cap b$ で囲まれています (これは $(0)$ とは異なります)。 $a + b \in I(A)$ については、$a + b$ によって下に制限されます。$d$ と $d'$ が、$da \subset A$ と $d'b \subset A$ のように、$A$ の非ゼロ元である場合、$dd'(a + b) \subset A$ になります。

#### 系 {#ac-vii-s1-n1-cor-1 .statement tag=04YQ}

*$x, y$と$x + y$が$K^*$にある場合、$\operatorname{div}(x + y) \geq \inf(\operatorname{div}(x), \operatorname{div}(y))$。

$A(x + y) \subset Ax + Ay$ したがって、$\operatorname{div}(x + y) \geq \operatorname{div}(Ax + Ay)$。

### 2. D(a) 上のモノイド構造

#### 命題 3 {#ac-vii-s1-prop-3 .statement tag=04YR}

$a, a', b, b'$を$I(A)$の元とします。 関係 $a > a'$ と $b > b'$ は $ab > a'b'$ を暗示します。

私たちは$b = b'$の場合に注意を限定するかもしれません。次に、$Ax$ を分数主イデアル含む $a'b$ とします。 $b$、$Ax \supset a'y$ のゼロ以外のすべての元 $y$、したがって $Axy^{-1} \supset a'$、よって $Axy^{-1} \supset a$、$Ax \supset ay$ です。 $y$ を変化させると、$Ax \supset ab$、よって $ab > a'b$ となることがわかります。

命題 3 から、$I(A)$ 定義するの乗法、移行から商、$D(A)$ の合成の法則が続きますが、これは明らかに結合的で可換です。これは加法的に書かれているので、次のように書けます。

$$
\text{div}(ab) = \text{div } a + \text{div } b,
$$

$I(A)$の$a, b$に。明らかに、$\text{div}(1)$ は、この加法に対して単位元です。この元は 0 で示されます。 命題 3 は、$D(A)$ の位数構造がこの加法 (*代数*、章 VI, § 1, no. 1) と *互換性* であることをさらに証明します。 (no. 1、命題 2 (ii)):

$$
\inf(\text{div } a + \text{div } b, \text{div } a + \text{div } c) = \inf(\text{div}(ab), \text{div}(ac)) = \text{div}(ab + ac)
= \text{div}(a(b + c)) = \text{div} a + \text{div}(b + c) = \text{div} a + \inf(\text{div } b, \text{div } c).
$$

分数イデアル $a \neq 0$ が $D(A)$ で $\text{div } a \geq 0$ となるためには、 $a \subset A$ であることが必要かつ十分です (他の語では、$a$ が $A$ の *整* イデアルであること)。

$K^*$ の 2 つの元 $x, y$ では、関係 $\text{div}(x) = \text{div}(y)$ は $Ax = Ay$ に相当します。 位数関係を伴う $A$ の主因子の集合と、$D(A)$ 上のそれによって誘起されるモノイド法則は、反対の順序で順序付けされた分数主イデアルの乗法群と正準的に同型の *順序付き群* です。 位数関係を含めます (*代数*、章 VI, § 1, no. 5)。 $D(A)$ の 2 つの元 $P, Q$ の間の関係 $S$:

「$P = Q + \text{div}(x)$のような$x \in K^*$が存在します」

したがって、関係 $P = Q + \text{div}(x)$ は $Q = P + \text{div}(x^{-1})$ と同等であるため、同値関係となります。 $P$ と $Q$ が $S$ を法として合同である場合、それらは $A$ の *同等の因子* と呼ばれます。さらに明らかに、関係 $S$ はモノイド $D(A)$ の法則と互換性があり、後者は$D(A)/S$ 上のモノイド構造である商を取ることにより定義するとなります。このモノイドは A* の *因子類モノイドと呼ばれます。

#### 命題 4 {#ac-vii-s1-prop-4 .statement tag=04YS}

$a, b$ を $A$ の 2 つの約分数イデアルとします。次のプロパティは同等です。
(a) $\text{div } a$ と $\text{div } b$ は因子と同等です。
(b) $b = xa$ となるような $x \in K^*$ が存在します。

ある$x \in K^*$に対して$\operatorname{div} b = \operatorname{div} a + \operatorname{div}(x)$であれば、$\operatorname{div} b = \operatorname{div}(xa)$、$b$と$xa$が約数であるため、$b = xa$となり、命題が証明されます。

$a$ を可逆分数イデアル (章 II, § 5, no. 6) とします。次に $a = A : (A : a)$ (*loc. cit.*, 命題 10)、したがって $a$ は *除数* (no. 1, 命題 1) です。したがって、可逆分数イデアルの群 $J(A)$ は、モノイド $D(A)$ の部分群および $D(A)/S$ の $J(A)$ の標準像と *射影* の類の群と同一視されます。 $A$-*階数* 1 のモジュール (章 II, § 5, no. 7、系 2 ～ 命題 12 および *注意* 1)。

#### 定理 1 {#ac-vii-s1-thm-1 .statement tag=04YT}

※$A$を整域とします。 $A$の因子のモノイド$D(A)$が群となるためには、$A$が完全に積分的に閉じていることが必要十分です*。

$D(A)$ が群であるとします。 $x \in K$ しましょう。 $A[x]$ が、$K$ の有限生成されたサブ$A$ モジュールに含まれているとします。次に、$a = A[x]$ が $I(A)$ の元であること (no. 1) を確認しました。次に$xa \subset a$、したがって$\operatorname{div}(x) + \operatorname{div} a \geq \operatorname{div} a$となります。 $D(A)$ は注文された群なので、$\operatorname{div}(x) \geq 0$、よって $x \in A$ を結論するとします。したがって、$A$ は完全に一体的に閉じられています (章 V, § 1、no. **4**、定義 5)。

逆に、$A$ が完全に積分的に閉じているとします。 $a$ を二分的な理想とします。 $\operatorname{div} a + \operatorname{div}(A : a) = 0$ を示して、$D(A)$ が群であることを証明します。 $a(A : a) \subset A$ として、含む $a(A : a)$ も含む $A$ であるすべての分数主イデアル $Ax^{-1}$ を検証するだけで十分です (no. 1)。さて、$y \in K^*$、関係 $Ay \supset a$ は $y^{-1} \in A : a$、よって $y^{-1}a \subset a(A : a) \subset Ax^{-1}$、したがって $xa \subset Ay$ を意味します。 $a$ は約数であるため、すべての $n \in \mathbf{N}$ に対して $xa \subset a$、よって $x^n a \subset a$ が推定されます。 $Ax_0 \subset a \subset Ax_1$ となるような $K^*$ のうち元 $x_0, x_1$ が存在します。したがって、$x^n x_0 \in Ax_1$、よって $x^n \in Ax_1 x_0^{-1}$。 $A$が完全に一体的に閉じているので、$x \in A$、つまり$Ax^{-1} \supset A$で証明が完成します。

$A$ が完全に積分的に閉じている場合 (さらにはネーター)、他の語、一般に $J(A) \neq D(A)$ (練習問題 2 および § 3, no. 2、命題 1) では、$A$ の約数イデアルは必ずしも反転可能ではないことに注意してください。

#### 系 {#ac-vii-s1-n2-cor-1 .statement tag=04YU}

*$A$ を完全な積分閉領域、$a$ を $A$ の除分数イデアルとする。次に、$A$ の各分数イデアル $b \neq 0$、$\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b$* について

no. 1 の公式 (1) により:

$$
\operatorname{div}(a : b) = \operatorname{div}\left( \bigcap_{y \in b, y \neq 0} y^{-1}a \right) = \sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a)
$$

命題 2 と分数イデアル $y^{-1}a$ が除数であるという事実を考慮します。しかし、$D(A)$ は順序付き群 (*代数*, 章 VI, § 1, no. 8) であるため、次のようになります。

$$
\sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a) = \sup_{y \in b, y \neq 0} (\operatorname{div} a - \operatorname{div}(y)) \\
= \operatorname{div} a - \inf_{y \in b, y \neq 0} \operatorname{div}(y) = \operatorname{div} a - \operatorname{div} b.
$$

### 3. クルールドメイン

#### 定義 3 {#ac-vii-s1-def-3 .statement tag=04YV}

整域 $A$ は、以下の特性を持つ分数 $K$ $A$ の体に評価のファミリー $(v_i)_{i \in I}$ が存在する場合、クルールドメインと呼ばれます。
(AK$_I$) 評価$v_i$ は離散的です。
(AK$_{II}$) $v_i$ の環の共通部分は $A$ です。
(AK$_{III}$) $v_t(x) \neq 0$ が有限であるような、添字 $t \in I$ のすべての $x \in K^*$、集合。

$A - (0)$ の元 $x$ に対して条件 (AK$_{III}$) を検証するだけで明らかに十分です。

例
(1) すべての離散評価環は Krull ドメインです。
(2) より一般的には、すべての主イデアル整域 $A$ が Krull ドメインです。 $(p_i)_{i \in I}$ を $A$ の極値元の代表系とし、$v_i$ を $p_i$ (章によって定義される $A$ の分数の体の評価) とします。 VI, § 3, no. 3、例 4)。ファミリ $(v_i)_{i \in I}$ が特性 (AK$_I$)、(AK$_II$)、および (AK$_{III}$) を満たすことがすぐにわかります。
(3) $F$を体、$(R_i)_{1 \leq i \leq n}$をクルル領域である$F$の部分環の有限族とする。次に、彼らの共通部分 $S = \bigcap_{j=1}^n R_j$ は Krull ドメインです。 $1 \leq j \leq n$ の場合、$(v_{j,t})_{t \in I_j}$ を $R_j$ の分数、満たす (AK$_I$)、(AK$_{II}$)、(AK$_{III}$) の体の評価ファミリーとします ($A$ は次のように置き換えられます)。 $R_j$）。 $w_{j,t}$ は、$S$ の分数の $v_{j,t}$ から体の制限を表すものとします。この場合、族 $(v_{j,t})_{1 \leq j \leq n, t \in I_j}$ は明らかに (AK$_{II}$) ($A$ は $S$ に置き換えられます) を満たし、添字$j$ の集合は有限であるため、(AK$_{III}$) も満たします。評価 $w_{j,t}$ は離散的であるか、不適切です。離散的なもののみを保持することにより、(AK$_I$)、(AK$_{II}$)、(AK$_{,,}$) ($A$ は $S$ に置き換えられます) を明らかに満たすファミリが得られます。したがって、$S$ は確かにクルルのドメインです。
(4) 特に、$A$ が Krull ドメインであり、分数の体 $K$ の $A$ の $K'$ 部分体の場合、$K' \cap A$ は Krull ドメインです。

#### 定理 2 {#ac-vii-s1-thm-2 .statement tag=04YW}

$A$を整域とします。 $A$ が Krull ドメインであるためには、条件に続く 2 つが満たされることが必要かつ十分です。
(a) $A$ は完全に一体的に閉じられています。
(b) $A$ の除数積分イデアルの空でないすべての族は、極大元 (関係 $\subset$ に関して) を認めます。
さらに、$P(A)$ が $D(A)$ の極値元の集合である場合、$P(A)$ は $\mathbf{Z}$ モジュール $D(A)$ の基底であり、$D(A)$ の正の元は次のようになります。 係数 $\geq 0$ と $P(A)$ の元の線形結合。

$A$ を Krull ドメインとします。完全一体クローズ（章VI, § 4, no. 5、系～命題9）です。 $(v_i)_{i \in I}$ を、分数 $K$ の $A$ 満たす (AK$_I$)、(AK$_{II}$)、および (AK$_{III}$) の体の評価ファミリーとします。 $v_i$ は正規化されていると仮定できます (章 VI, § 3, no. 6, 定義 3)。すべての $a \in I(A)$ について、次のように書きます。

$$
v_t(a) = \sup_{a \subset Ax} (v_t(x));
$$

次に、$v_t(a) \in \mathbf{Z}$、つまり、$a$が$a$のゼロ以外の元である場合、関係 $Ax \supset Aa$は$v_t(x) \leq v_t(a)$（by (AK$_{III}$)）を意味し、$v_t(x)$の家族であることがわかります。 ($a \subset Ax$) は上に有界です。次のプロパティを確立します。

(1) *$a$ を除数分数イデアルとします。 位数では $y \in a$ であるため、すべての $t \in I$ に対して $v_t(y) \geq v_t(a)$ であることが必要かつ十分です。*

$a$ は除数であるため、関係 $y \in a$ は関係と等価です。「「$a \subset Ax$ は $y \in Ax$」を意味します。ここで、(AK$_{II}$) により、関係 $y \in Ax$ はすべての「$v_t(y) \geq v_t(x)$」と等価です$t \in I$”。よって (1)。

(2) *$a$ と $b$ を $A$ の 2 つの分数イデアルとする。 位数では $a \subset b$ であるため、すべての $t \in I$ に対して $v_t(a) \geq v_t(b)$ であることが必要かつ十分です。*

これは、性質 (1) の直後に続きます。

(3) *$x \in K^*$の場合は、$v_t(Ax) = v_t(x)$。*

$Ay \supset Ax$ の場合、(AK$_{II}$) によって $v_t(y) \leq v_t(x)$ が計算され、$v_t(y)$ の最小値値が $y = x$ で取得されます。

(4) *すべての $a \in I(A)$、添字 $t \in I$ について、$v_t(a) \neq 0$ は数で有限になります。*

$Ax \subset a \subset Ay$ のような $K^*$ には $x, y$ が存在します。特性 (2) と (3) により、すべての $t \in I$ に対して $v_t(x) \geq v_t(a) \geq v_t(y)$ になります。その後、(AK$_{III}$) を適用するだけで十分です。

したがって、次の補題を示しました。

#### 補題 1 {#ac-vii-s1-lem-1 .statement tag=04YX}

*If $A$ is a Krull domain and $(v_t)_t$, is a family of normed valuations on $K$ satisfying (AK$_I$), (AK$_{II}$) and (AK$_{III}$), the mapping $a \mapsto (v_t(a))_{t \in I}$ is a decreasing injective mapping of the set of divisorial integer ideals of $A$ (ordered by $\subset$) to the set of positive elements & the ordered group the direct sum $\mathbf{Z}^{(I)}$.*

そうなると、$\mathbf{Z}^{(I)}$ の正の元の空でないすべての集合には、最小の元 (*代数*、章 VI, § 1, no. 13、定理 2) が含まれます。したがって、$A$ は主張の性質 (b) を確実に満たします。

逆に、$A$を整域満たすの主張の性質(a)と(b)とする。 $A$ は完全に積分的に閉じているため、$D(A)$ は順序付けられた群 (no. 2, 定理 1) です。この群は格子（no. 1、命題2）です。 主張の条件 (b) までに、$D(A)$ の正の元の空でないすべての家族は最小の元を持ちます。 $P(A)$ を $D(A)$ の極値元の集合とします。次に (*代数*, 章 VI, § 1, no. 13, 定理 2) $P(A)$ は $\mathbf{Z}$ モジュール $D(A)$ の基底であり、$D(A)$ の正の元は、次の式で線形結合になります。 正の整数係数/元/$P(A)$。

したがって、$x \in K^*$ について、有理数整数 $v_P(x)$ は次のように定義されます ($P \in P(A)$ について):

$$
\text{div}(x) = \sum_{P \in P(A)} v_P(x) \cdot P.
$$

$v_P(0) = +\infty$とも書きます。

関係から

$$
\text{div}(xy) = \text{div}(x) + \text{div}(y)
$$

そして

$$
\text{div}(x + y) \geq \inf(\text{div}(x), \text{div}(y)),
$$

$K^*$ の $x, y$ と $x + y$ について、$v_P$ は $K$ の *離散評価* であると推測します。 $x \in A$の位数では、$P \in P(A)$すべてに対して$\text{div}(x) \geq 0$、つまり$v_P(x) \geq 0$があれば必要十分です。したがって、$v_P$ 満たす条件 (AK$_1$) と (AK$_{11}$)、そして明らかに (AK$_{III}$) も同様です。

#### 系 {#ac-vii-s1-n3-cor-1 .statement tag=04YY}

*ネーター 環がクルルドメインであるためには、それが完全に閉じられたドメインであることが必要十分です。*

積分的に閉じられたネーター ドメインは完全に積分的に閉じられています (章 V, § 1, no. 4)。

非ネーター クルール ドメインが存在します。たとえば、無限の不定値 (cf. 練習問題 8) では、体 $K$ の上に多項式環 $K[X_n]_{n \in \mathbf{N}}$ があります。

### 4. クルールドメインの重要な評価

$A$ を Krull ドメイン、$K$ をその分数の体とします。 no. 3 ($x \in K^*$) の公式 (4) によって定義される評価は、$K$ (*または* $A$) の *必須評価* と呼ばれます。

定理 2 の証明の過程で、定義 3 の評価 $v_P$ 満たすプロパティ (AK$_1$)、(AK$_2$)、および (AK$_{III}$) が、定義 3 の評価$v_P$ であることに注意しました。 *正規化*: すべての極値因子 $P \in P(A)$、$P < 2P$ に対して、$a$ と $b$ が対応するから $P$ と $2P$ までの除数イデアルである場合、$a \supseteq b$ と $a \neq b$ になります。 $x \in a - b$、$\text{div}(x) \geq P$、$\text{div}(x) \not\geq 2P$、よって $v_P(x) = 1$ は、主張を証明します。

#### 命題 5 {#ac-vii-s1-prop-5 .statement tag=04YZ}

*$A$ を Krull ドメイン、$K$ をその分数の体、そして $(v_P)_{P \in P(A)}$ をその本質的な評価のファミリーとします。 $(n_P)_{P \in P(A)}$ を、添字の有限数を除いて零である有理数整数の族とします。次に、$x \in K$ の集合は、すべての $P \in P(A)$ に対して $v_P(x) \geq n_P$ が、$\text{div } a = \sum_{P \in P(A)} n_P \cdot P$ となるような $A$ の除数イデアル $a$ になります。

$x \in K^*$ にしましょう。 位数の $x \in a$ では、$Ax \subset a$、したがって $\text{div}(x) \geq \text{div } a$、したがって (4) により、すべての $P \in P(A)$ に対して $v_P(x) \geq n_P$ となることが必要かつ十分です。

#### 命題 6 {#ac-vii-s1-prop-6 .statement tag=04Z0}

$A$ を Krull ドメイン、$K$ を分数の体、$(v_t)_{t \in I}$ を定義 3 と $A$、環のプロパティを持つ $K$ の評価ファミリーとします。 $v_t$。 $S$ を、含む $0$ と添字 $t \in I$ の $J$ 集合ではなく、$A$ の乗算部分集合とし、$v_t$ が零となるようにします。 $S$。次に$S^{-1}A = \bigcap_{t \in J} A_t$;特に $S^{-1}A$ は Krull ドメインです。

$B = \bigcap_{t \in J} A_t$と書きます。次に、$S^{-1} \subset B$、$A \subset B$、そして$S^{-1}A \subset B$となります。逆に$x \in B$とします。 $J'$ は、$v_t(x) < 0$ となるような添字 $t$ の有限集合を表すものとします。 $t \in J'$ の場合、$x \notin A_t$、したがって $t \notin J$ となり、$v_t(s_t) > 0$ となるような $s_t \in S$ が存在します。 $n(t)$ を整数 $> 0$ として、$v_t(s_t^{n(t)}x) \geq 0$ とします。 $s = \prod_{t \in J'} s_t^{n(t)}$と書きます。次に、すべての $t \in I$ に対して $v_t(sx) \geq 0$、したがって $sx \in A$ と $x \in S^{-1}A$ になります。したがって、$B = S^{-1}A$。

#### 系 1 {#ac-vii-s1-prop-6-cor-1 .statement tag=04Z1}

$P$ を $A$ と $p$ 対応するの極値因子とする。この場合、$p$ は素数であり、$v_P$ の環は $A$ であり、$v_P$ の剰余体は $A/p$ の分数の体と同一視されます。

$S = A - p$ にしましょう。 命題 5 までに、$v_P$ は $S$ では零になり、$p$ では $> 0$ になります。したがって、$p$ は $A$ の共通部分であり、$v_P$ のイデアルであり、したがって素数です。一方、すべての極値因子 $Q \neq P$、$Q \not\subset P$、したがって除算イデアル $q$ 対応するから $Q$ は $p$ に含まれません。したがって、$q \cap S \neq \varnothing$ となり、命題 5 までに、$v_Q$ は $S$ の零ではなくなります。そうなると、命題 6 と章 II, § 3, no. 1、命題 3 から系が続きます。

#### 系 2 {#ac-vii-s1-prop-6-cor-2 .statement tag=04Z2}

$A$ を Krull ドメイン、$K$ を分数の体、および $(v_t)_{t \in I}$ を定義 3 の特性を持つ評価ファミリーとします。すると、$A$ のすべての必須評価は、$v_t$ の 1 つに相当します。

$P$ を $A$ と $p$ 対応するの極値因子とする。 系 1、命題 5、補題 1、主張 (1) により、定理 2、no. 3 の証明には、環 $A_t$ となるような$t \in I$ が存在します。 $v_t$ 含む環 $A$、$v_P$中。 $v_t$ と $v_P$ は高さ 1 なので、同等です (章 VI, § 4, no. 5、命題 6)。

#### 命題 7 {#ac-vii-s1-prop-7 .statement tag=04Z3}

$A$ を Krull ドメイン、$(v_P)_{P \in P(A)}$ をその本質的な評価のファミリー、$a \in I(A)$ とします。すると、$\operatorname{div} a$の$P$の係数は$\inf_{y \in a} (v_P(y))$になります。 $p$ が極値因子 $P$ に対する約数素イデアル対応するである場合、$aA_p = \tilde{a}A_p$ です。

$a = \sum_{y \in a} Ax$、命題 2 (b) (no. 1) は、$\operatorname{div}(a) = \inf_{x \in a} (\operatorname{div}(Ax))$、よってが最初の主張であることを示しています。 $\operatorname{div} \tilde{a} = \operatorname{div} a$ と $A_p$ は離散評価 $v_P$ の環であるため、2 番目がすぐに続きます。

#### 命題 8 {#ac-vii-s1-prop-8 .statement tag=04Z4}

$A$ を完全に閉じたネーター ドメインとします。
(a) $P$ を $A$ と $p$ 対応するの極値因子とする。

$n \in \mathbf{N}$ の場合は $p^{(n)} = p^n A_p \cap A$ とします。この場合、$p^{(n)}$ は $v_p(x) \geq n$ となる $x \in A$ の集合であり、$p$ の主イデアルです。

(b) Let $a$ be a divisorial integral ideal, $n_1 P_1 + \ldots + n_r P_r$ 因子 of $a$ (the $P_i$ being distinct extremal 因子) and $p_i$ the divisorial prime ideal 対応する to $P_i$.次に、$a = \bigcap_{i=1}^r p_i^{(n_i)}$ は $a$ の固有の還元原色分解であり、$p_i$ は浸されていません。

系 1 から命題 6 まで、関係 $x \in p^n A_p = (pA_p)^n$ は $v_p(x) \geq n$ と同等です。一方、$A$ は離散評価環であるため、$(pA_p)^n$ は $(pA_p)$ - 主要 (章 IV, § 2, no. 1、例 4) であるため、$p^{(n)}$ は $p$ - 主要です(章 IV, § 2, no. 1、命題 3);これは (a) を示しています。 命題 5 は確かに $a = \bigcap_{i=1}^r p_i^{(n_i)}$ を示しています。 As $p_i \not\subset p_j$ for $i \neq j$ this primary decomposition is reduced: For if $p_i^{(n_i)} \supset \bigcap_{j \neq i} p_j^{(n_j)} \supset \prod_{j \neq i} p_j^{(n_j)}$, $p_{ji}$ would contain one of the $p_j$ for $j \neq i$ (Chapter II, § 1, no. 1, Proposition 1). 一意性は、章 IV, § 2, no. 3、命題 5 から続きます。

### 5. 重要な評価額の概算

Krull ドメインの本質的な評価は離散的かつ標準化されているため、同等のものは 2 つなく、したがって独立しています (章 VI, § 7, no. 2)。したがって、近似値定理 (引用文献、定理 1) に系 2 を適用することができます。いくつかの $n_i \in \mathbf{Z}$ といくつかの本質的な評価 $v_i$ が数で有限で個別であるとすると、すべてに対して $v_i(x) = n_i$ となるような $x \in K$ が存在します。 $i$。しかし、ここではより正確な結果が得られます。

#### 命題 9 {#ac-vii-s1-prop-9 .statement tag=04Z5}

$v_1, \ldots, v_r$ を、クルール領域 $A$ と $n_1, \ldots, n_r$ 有理数整数の個別の本質的評価とします。 元 $x$ の体の分数 $K$ の $A$ などの $1 \leq i \leq r$ の $v_i(x) = n_i$ と $A$ の $v$ のすべての重要な評価に対して $v(x) \geq 0$ が存在します。 $v_1, \ldots, v_r$。

$p_1, \ldots, p_r$ を、評価 $v_1, \ldots, v_r$ に対する $A$ 対応するの除数イデアルとします。 $1 \leq i \leq r$ に対して $v_i(y) = n_i$ となるような $y \in K$ が存在します (章 VI, § 7, no. 2, 系 1 ～ 定理 1)。 $A$ の本質的な評価 $w_1, \ldots, w_s$ は、整数 $w_j(y) = -m_j$ が $< 0$ である $v_i$ とは異なり、数で有限です。 $q_1, \ldots, q_s$を対応するの理想としましょう。これらの理想値対応するから極値因子までがあり、これらの理想値は素数 (系 1 から命題 6) であるため、$p_1, \ldots, p_r, q_1, \ldots, q_s$ の間に包含関係は存在しません。したがって、積分イデアル $a = q_1^{m_1} \ldots q_s^{m_s}$ は、$p_i$ (章 11、§ 1, no. 1、命題 1) のいずれにも含まれず、したがってそれらの和集合 (上記、命題 2) にも含まれません。したがって、$1 \leq i \leq r$ に対して $z \notin p_i$ となるような $z \in a$ が存在します。次に、$v_1(z) = \cdots = v_r(z) = 0$ と $w_j(z) \geq m_j$ が $1 \leq j \leq s$ になります。したがって、元 $x = yz$ は問題を解決します。

#### 系 1 {#ac-vii-s1-prop-9-cor-1 .statement tag=04Z6}

$\mathbf{A}$ をクルール領域、$\mathbf{K}$ を分数の体と $\mathbf{a}, \mathbf{b}$ および $c$ の 3 つの約数分数イデアルである $\mathbf{a} \subset \mathbf{b}$ とする $\mathbf{A}$ とします。 $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$ となるような $x \in \mathbf{K}$ が存在します。

Let $(v_t)_{t \in I}$ be the family of essential valuations of $\mathbf{A}$ and let $(m_t)$ (resp. $(n_t), (p_t)$) be the family of rational integers (zero except for a finite number of indices) such that $\mathbf{a}$ (resp. $\mathbf{b}, c$) is the set of $x \in \mathbf{K}$ for which $v_t(x) \geq m_t$ (resp. $n_t, p_t$) for all $t \in I$ (Proposition 5, no. 4). $m_t > n_t$ が有限となるような $t \in I$ の集合 $\mathbf{J}$。 $p_t = m_t = 0$ として、添字の有限数を除いて、命題 9 は、$t \in \mathbf{J}$ に対して $v_t(x^{-1}) + m_t = p_t$ となるような$x \in \mathbf{K}^*$ が存在することを示します。
$$
v_t(x^{-1}) + m_t \geq p_t
$$
$t \in I - \mathbf{J}$の場合。 次に、すべての $t \in I$、$m_t = \sup(n_t, v_t(x) + p_t)$ についてです。 よって $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$。

#### 系 2 {#ac-vii-s1-prop-9-cor-2 .statement tag=04Z7}

$\mathbf{A}$ を Krull ドメインとします。 $\mathbf{A}$ の分数イデアル $\mathbf{a}$ が除数であるためには、それが 2 つの分数主イデアルの共通部分であることが必要かつ十分です。

十分性は明らかです (no. 1、定義 2)。必然性は系 1 から続きます。$b$ と $c$ を主とし、$b \supseteq a$ となります。

### 6. クルール領域の高さ 1 の主な理想

#### 定義 4 {#ac-vii-s1-def-4 .statement tag=04Z8}

$\mathbf{A}$ を整域とします。 $\mathbf{A}$ の素イデアル $\mathfrak{p}$ は、$\mathbf{A}$ の非ゼロの素イデアルの中で最小である場合、高さ 1 であると言われます。

また、理想的な $(0)$ は高さ 0 であるとも言えます。したがって、高さ $\leq 1$ の主イデアルは、定義により $(0)$ または高さ 1 に等しくなります。

私たちは、一般的な方法で、主要な理想の高さを定義する下回ります。

#### 定理 3 {#ac-vii-s1-thm-3 .statement tag=04Z9}

$\mathbf{A}$ を Krull 領域、$\mathfrak{p}$ を $\mathbf{A}$ の整数イデアルとします。 $\mathfrak{p}$ が極値因子に対する除数イデアル対応するであるためには、$\mathfrak{p}$ が高さ 1 の素イデアルであることが必要かつ十分です。

$\mathfrak{p}$ が極値因子に対する除数理想対応するである場合、$\mathfrak{p}$ が素数であり、$\mathbf{A}_\mathfrak{p}$ が離散評価環であることがわかります (no. 4、系 1 から命題 6)。 $\mathbf{A}_\mathfrak{p}$ には $(0)$ と $\mathfrak{p}\mathbf{A}_\mathfrak{p}$ 以外に素イデアルがないため、$\mathfrak{p}$ (章 II, § 3, no. 1, 命題 3) に含まれる $\mathbf{A}$ の素イデアルは $(0)$ と $\mathfrak{p}$ だけです。したがって、$\mathfrak{p}$ は高さ 1 です。 逆に、$\mathbf{A}$ 含むの約数素イデアル $\mathfrak{q}$ 対応するから極値因子までのすべての素イデアル $\mathfrak{p} \neq (0)$ が、$\mathbf{A}_\mathfrak{p} \neq K$ と同様に、$\mathbf{A}_\mathfrak{p}$ は空でない族の共通部分であることを最初に示します。必須評価の$(\mathbf{A}_t)$ 環 (no. 4、命題 6);それぞれの $\mathbf{A}_t$ は形 $\mathbf{A}_{\mathfrak{q}_t}$ (no. 4、系 1 から命題 6) であり、$\mathbf{A}_\mathfrak{p} \subset \mathbf{A}_{\mathfrak{q}_t}$ から $\mathfrak{q}_t \subset \mathfrak{p}$ と推定されます。 したがって、$\mathfrak{p}$ の高さが 1 の場合、$\mathfrak{p} = \mathfrak{q}$ となり、$\mathfrak{p}$ が極値因子に対する除数イデアル対応するであることを示します。

#### 系 1 {#ac-vii-s1-thm-3-cor-1 .statement tag=04ZA}

クルール領域では、すべての非ゼロ素イデアル m 含むは高さ 1 の素イデアルです。 m が高さ 1 でない場合、 div m = 0 および A : m = A です。

最初の主張は、定理 3 の証明の過程ですでに見られています。m が高さ 1 ではなく、p が m に含まれる高さ 1 の素イデアルである場合、p ⊂ m̃ および p ≠ m̃ です。 div p が極値であるため、必然的に div m = div m̃ = 0;したがって、 div(A : m) = 0 となり、A : m は除数 (no. 1, 命題 1) であるため、A : m = A となります。

#### 系 2 {#ac-vii-s1-thm-3-cor-2 .statement tag=04ZB}

A をクルール領域、K を分数の体、v を A および x ∈ A の p 集合で正となる K の評価とし、v(x) > 0 とする。素イデアル p の高さが 1 の場合、v は A の本質評価と等価です。

B を v と m の環として理想的とします。この場合、m ∩ A = p となり、A_p ⊂ B となります。ここで、A_p は離散評価環 (定理 3 および系 1 ～ 命題 6) になります。 p ≠ (0)、B ≠ K であるため、B = A、(章 VI, § 4, no. 5, 命題 6)。

#### 定理 4 {#ac-vii-s1-thm-4 .statement tag=04ZC}

A を高さ 1 の主イデアルの整域および M 集合とします。A が Krull ドメインであるためには、次のプロパティが満たされることが必要かつ十分です。
(i) すべての p ∈ M に対して、A は離散評価環です。
(ii) A は、p ∈ M に対する A_p の共通部分です。
(iii) A のすべての x ≠ 0 に対して、x ∈ p となるイデアル p ∈ M は有限数だけ存在します。
さらに、p ∈ M に対する A_p の評価対応するが A の本質的な評価です。

条件で十分です。 それらの必要性は、no. 4の定理 3、系 Iから命題 6、そして満たす条件の定義 3のno. 3の本質的な評価がすぐに続きます。

#### 命題 10 {#ac-vii-s1-prop-10 .statement tag=04ZD}

A を積分的に閉じたネーター 領域および A の積分イデアルとします。次の条件は等価です。
(a) a は除数です。
(b) A/a に関連付けられた主イデアルの高さは 1 です。

a = $\bigcap^n q_i$ が a の縮小主分解であり、p_i が q_i に対する素イデアル対応するを表す場合、A/a に関連付けられた素イデアルは単なる p_i (章 IV, § 2, no. 3, 命題 4) であることを思い出してください。 (a) が (b) を意味するという事実は、no. 4 の命題 8 から導かれます。逆に、上記の記法で、p_i の高さが 1 である場合、A_{p_i} は離散評価環 (定理 4) です。ここで、q_i = q_i A_{p_i} ∩ A (章 IV, § 2, no. 1, 命題 3); p_i に対する本質的な評価対応するを v_i で表すと、q_i が x ∈ A の集合となり、v_i(x) ≥ n_i となるような整数 n_i が存在します。これは、q_i が除数 (no. 4, 命題 5) であることを示しており、したがって a でもあります。

### 7. アプリケーション: 離散評価環の新しい特徴付け

#### 命題 11 {#ac-vii-s1-prop-11 .statement tag=04ZE}

$\mathbf{A}$ をローカル Krull ドメイン (特に、積分的に閉じたローカルネーター ドメイン) とし、$m$ をその最大理想とする。次の条件は同等です。
(a) $\mathbf{A}$ は離散評価環です。
(b) $m$ は反転可能です。
(c) $\mathbf{A}:m \neq \mathbf{A}$;
(d) $m$ は除数的です。
(e) $m$ は、$\mathbf{A}$ の唯一の非ゼロの素イデアルです。

離散評価環のゼロ以外の理想はすべて主 (章 VI, § 3, no. 6、命題 9) であるため、可逆であり、したがって (a) は (b) を意味します。 $m$ が反転可能な場合、その逆数は $\mathbf{A}:m$ (章 II, § 5, no. 6, 命題 10) となり、したがって $\mathbf{A}:m \neq \mathbf{A}$ になります。したがって、(b) は (c) を意味します。 $\mathbf{A}:m \neq \mathbf{A}$ の場合は、$\mathbf{A}:(\mathbf{A}:m) \neq \mathbf{A}$。現在$m \subset \mathbf{A}:(\mathbf{A}:m)$;したがって、$m = \mathbf{A}:(\mathbf{A}:m)$ $m$ が最大であるため、$m$ は約数になります (no. 1, 命題 1 (c))。したがって、(c) は (d) を意味します。 (d) が (e) を意味するという事実は、no. 6 の定理 3 から導き出されます。最後に、$m$ が $\mathbf{A}$ の唯一の非ゼロ素数イデアルである場合、その高さは 1 であるため、$\mathbf{A}_m$ は離散評価環 (no. 6, 定理 4); $\mathbf{A}$ はローカルであるため、$\mathbf{A}_m = \mathbf{A}$ は、(e) が (a) を意味することを示しています。

### 8. 分数の体の有限拡大におけるクルール領域の積分閉包

#### 命題 12 {#ac-vii-s1-prop-12 .statement tag=04ZF}

$\mathbf{A}$ をクルール領域、$K$ を分数の体、$K'$ を $K$ の有限拡大、$\mathbf{A}'$ を $K'$ の $\mathbf{A}$ の積分閉包とします。次に$\mathbf{A}'$はクルルドメインです。 $\mathbf{A}'$ の本質的評価は、$K'$ の標準化された離散評価であり、$\mathbf{A}$ の本質的評価の拡大に相当します。

$(v_i)_{i \in I}$ を $\mathbf{A}$ の本質的評価の拡大から $K'$ の族とする。 次数 $n = [K':K]$ は有限であるため、$v_i$ は $K'$ の離散評価 (章 VI, § 8, no. 1、系 3 ～ 命題 1) です。 $B_i$ を $v_i$ の環とします。次に、$\mathbf{A}' \subset \bigcap_{L \in I} B_i$ (章 VI, § 1, no. 3、定理 3)。 逆に、$\bigcap_{i \in I} B_i$ のすべての元 $x$ は、$\mathbf{A}$ の各必須評価環 (章 VI, § 1, no. 3、系 3 ～ 定理 3) に対して積分されます。したがって、$K$ 属する ～ $\mathbf{A}$ (章 V, § 1, no. 3、系 ～ 命題 11) にわたる $x$ の最小多項式の係数なので、 $x \in \mathbf{A}'$ となります。したがって$\mathbf{A}' = \bigcap_{i \in I} B_i$。 ここで、$x$ を $\mathbf{A}'$ の非ゼロ元とします。 形 $x^s + a_{s-1}x^{s-1} + \ldots + a_0 = 0$ の方程式を満たす

ここで、$a_i \in \mathbf{A}$ と $a_s \neq 0$; $v_i(x) > 0$ の場合は $v_i(a_0) > 0$;ここで、$v(a_0) > 0$ が数で有限であるような $\mathbf{A}$ の本質的な評価 $v$ は、$K$ の与えられた評価を拡張した $K'$ の評価も数 (章 VI, § 8, no. 3, 定理 1); hence $v_i(x) = 0$ except for a finite 数 of 添字 $i \in I$. Thus it has been proved that $\mathbf{A}'$ is a Krull domain (no. 3, 定義 3).

$v_i$ が $A'$ (no. 4, 系 2 ～ 命題 6)、つまり (no. 6, 系 2 ～ 定理 3) の本質的な評価と同等であること、つまり主要な理想 $p_i$ が、 $v_i(x) > 0$ となる $x \in A'$ のからなるは高さ 1 です。 そうでない場合は、$(0)$ と $p_i$ から $(0) \subset q \subset p_i$ が区別されるような $A'$ の主要な理想 $q$ が存在することになります。その場合、$(0) \subset q \cap A \subset p_i \cap A$ と $q \cap A$ は、$(0)$ と $p_i \cap A$ (章 V, §2, no. 1、系 1 ～ 命題 1) とは異なります。したがって、主要な理想 $p_i \cap A$ は高さ 1 ではなく、矛盾するという事実は、$A$ の本質的な評価に対して対応するになります。

#### 系 {#ac-vii-s1-n8-cor-1 .statement tag=04ZG}

*$p$ (それぞれ $p'$) を高さ 1 の $A$ (それぞれ $A'$) の主要な理想とし、$v$ (それぞれ $u'$) をそれに対する $A$ (それぞれ $A'$) 対応するの本質的な評価とします。 $p'$が$p$の上にあるためには、$v'$から$K$の制限が$v$と同等であることが必要かつ十分です。

評価 $v'$ は、$A$ (命題 12) の必須評価 $w$ の拡大に相当します。高さ1の$A$の主な理想である$q = p' \cap A$を仮定します。$v'$から$K$の制限が$v$と同等であるためには、$w = v$、したがって$q = p$であることが必要かつ十分です。

### 9. クルールドメインを介した多項式環

#### 命題 13 {#ac-vii-s1-prop-13 .statement tag=04ZH}

*$A$ を Krull ドメインとし、$X_1, X_n, \ldots, X_n$ を不定とします。 環 $A[X_1, \ldots, X_n]$ は Krull ドメインです。*

$n$ について帰納法が議論すると、$X$ が不定の場合、$A[X]$ がクルル領域であることを示すだけで十分です。 $K$ を $A$ の分数の体とします。 $A[X]$の分数の体は$K(X)$です。 $I$ を、$K$ で既約である $K[X]$ のモニック多項式の集合とします。すべての $f \in I$ について、$v_f$ を $f$ (章 VI, §3, no. 3, 例 4) によって定義される $K(X)$ の評価とします。一方、$A$ のすべての必須評価 $w$ について、$w$ を、次のように定義される $w$ ～ $K(X)$ の拡大とします。

$$
\bar{w}\left( \sum_j a_j X^j \right) = \inf_j (w(a_j))
$$

$\sum_j a_j X^j \in K[X]$ (章 VI, §10, no. 1、補題 1) の場合。 Clearly the $u$, and the $\bar{w}$ are discrete and normed and, for all $u \in K[X]$, $v_f(u) = 0$ (resp. $\bar{w}(u) = 0$) except for a finite number of valuations $v_f$ (resp. $\bar{w}$).

したがって、命題を示すには、$A[X]$ が評価$v_f$ と $\bar{w}$ の環の共通部分であることを示すだけで十分です。現在、評価額 $v_f$ の環の共通部分は $K[X]$ です。一方、$\sum_j a_j X^j \in K[X]$ の場合、関係 $\bar{w}\left( \sum_j a_j X^j \right) \geq 0$ は「すべての $j$ に対して $w(a_j) \geq 0$」と同等です。したがって、関係「すべての評価$\bar{w}'$に対して$\bar{w}\left( \sum_j a_j X^j \right) \geq 0$」は、「すべての$j$と$A$のすべての重要な評価$w$に対して$w(a_j) \geq 0$」と同等です。これは私たちの主張を証明します。

#### 注意 {#ac-vii-s1-n9-rem-1 .statement tag=04ZI}

命題 13 の証明で導入された評価$v_f$ と $\bar{w}$ は、$A[X]$ の本質的な評価です。 $V$ が評価 $v_f$ ($f$ 既約) と $\bar{w}$ (必須) の集合である場合、すべての $v' \in V$ に対して、$A[X]$ には含まれない元 $g \in K(X)$ が存在することを示すだけで十分です。 $v'$ とは異なるすべての評価$v'' \in V$ に対して $v''(g) \geq 0$。これにより、$V - \{v'\}$ は満たす (AK$_{II}$) ではないことが証明され、結論は、no. 4、系 2 から命題 6 になります。 まず、$v'$ が形 $\bar{w}$ であると仮定します。 $g$ は元 $b \in K$ となり、$w$ とは異なる $A$ の本質的な評価 $w'$ に対して $w(b) < 0, w'(b) \geq 0$ が得られ、その場合、次の既約モニック多項式 $f$ に対して $v_f(b) = 0$ $K[X]$; 元 $b$ 満たす上記の条件は、no. 5、命題から導かれます。 9. 次に、$v'$ が既約モニック多項式の形 $v_f$ であると仮定します。 次数中$f \in K[X]$$m$;そうすると、$a \in A$ を $g = a/f$ とることができます。 $K[X]$ の既約モニック多項式 $h \neq f$ ごとに $v_h(g) \geq 0$ の場合。 $A$ のすべての必須評価 $w$ に対して、$w(a)$ が元 $w(c_i)$ の最大の下界に少なくとも等しいように、選ぶ $a \in A$ に留まります。ここで、$c_i$ は$f$ ($1 \leq i \leq m$) の係数;現在、そのような $a \in A$ の存在は、(AK$_{III}$) と no. 5、命題 9 から続きます。

また、(no. 6, 定理 4) 高さ 1 の $A[X]$ の主な理想は次のとおりであると言えます。
(1) 形 $pA[X]$ の主イデアル、ここで $p$ は高さ 1 の $A$ の主イデアルです。
(2) 形 $m \cap A[X]$ の素イデアル、ここで $m$ は $K[X]$ の (必然的に主な) 素イデアルです。

後者は、$A$ の共通部分が 0 に減少するという事実によって特徴付けられます。

### 10. クルールドメインの因子類

$A$ を Krull ドメインとします。 $A$ の因子の群 $D(A)$ は、その極値元 (no. 3, 定理 2) の集合 $P(A)$ によって生成される自由可換群であることを思い出してください。 $P(A)$ は、高さ 1 (no. 6) の $A$ の主要理想の集合と同一視されます。 $p \in P(A)$ については、標準的な必須評価対応するから $p$ (no. 4) を $v_p$ で表すことにします。 $v_p$ の環は $A_p$ (no. 4、系 1 ～ 命題 6) であることを思い出してください。本人因子の $D(A)$ からなるの $F(A)$ 部分群と、$A$ (no. 2) の $C(A) = D(A)/F(A)$ 因子類群で表します。

#### 命題 14 {#ac-vii-s1-prop-14 .statement tag=04ZJ}

$A$ を Krull ドメイン、$B$ を Krull ドメイン含む $A$ とします。次の条件が成り立つと仮定します。

(偏微分方程式) 高さ 1 の $B$ のすべての素イデアル $\mathfrak{P}$ について、主イデアル $\mathfrak{P} \cap A$ は零または高さ 1 です。

$p \in P(A)$ の場合、$\mathfrak{P} \cap A = p$ は数で有限となるような $\mathfrak{P} \in P(B)$。私たちは書きます

$$
i(p) = \sum_{\mathfrak{P} \in P(B), \mathfrak{P} \cap A = p} e(\mathfrak{P}/p)\mathfrak{P},
$$

ここで、$e(\mathfrak{P}/\mathfrak{p})$ は、$v_{\mathfrak{p}}$ の $v_{\mathfrak{p}}$ (章 VI, § 8, no. 1) への *分岐* 添字を表します。 *次に、* 線形性により、定義する、増加する *準同型* $i$ $D(A)$ から $D(B)$ となり、次の特性が得られます。

(a) *A* の体の分数のゼロ以外のすべての元 x について、

$$
i(\operatorname{div}_A(x)) = \operatorname{div}_B(x);
$$

(b) *D(A) 内のすべての D、D' について*、

$$
i(\sup(D, D')) = \sup(i(D), i(D'));
$$

$\mathfrak{p} \in P(A)$ にしましょう。 $\mathfrak{p}$ の非ゼロ元 $a$ を考えてみましょう。 含む $a$ が数 (no. 6, 定理 4) で有限である $\mathfrak{P} \in P(B)$。 *なおさら* $\mathfrak{P} \cap A = \mathfrak{p}$ が数で有限となるような $\mathfrak{P} \in P(B)$。

次に (a) を示します。加法性により、$x \in A^* = A - \{0\}$ と仮定できます。

定義、$\operatorname{div}_B(x) = \sum_{\mathfrak{P} \in P(B)} v_{\mathfrak{p}}(x) \cdot \mathfrak{P}$までに。 $v_{\mathfrak{p}}(x) > 0$ のようなすべての $\mathfrak{P} \in P(B)$ について、$\mathfrak{P} \cap A$ は ($x \in \mathfrak{P}$ の場合) 非ゼロであるため、(PDE) により高さ 1 になります。 設定 $\mathfrak{p} = \mathfrak{P} \cap A$、派生添字の定義により、$v_{\mathfrak{p}}(x) = e(\mathfrak{P}/\mathfrak{p}) v_{\mathfrak{p}}(x)$ ($v_{\mathfrak{p}}$ と $v_{\mathfrak{P}}$ が正規化されているため)。 形 $\mathfrak{Q} \cap A$ のうち $\mathfrak{Q} \in P(B)$ 以外のすべての $q \in P(A)$ に対する $\operatorname{div}_A(x) = \sum_{\mathfrak{p} \in P(A)} v_{\mathfrak{p}}(x) \cdot \mathfrak{p}$ と $i(q) = 0$ として、(a) を推定します。

(b) を証明するには、次のように書きます。

$$
D = \sum_{\mathfrak{p} \in P(A)} n(\mathfrak{p}) \cdot \mathfrak{p} \quad \text{and} \quad D' = \sum_{\mathfrak{p} \in P(A)} n'(\mathfrak{p}) \cdot \mathfrak{p};
$$

$\sup(D, D')$の$\mathfrak{p}$の係数は$\sup(n(\mathfrak{p}), n'(\mathfrak{p}))$です。 $\mathfrak{P}$を$P(B)$の元とします。 $\mathfrak{P} \cap A = (0)$ の場合、$i(D)$ と $i(D')$ の $\mathfrak{P}$ の係数は、$\sup(i(D), i(D'))$ も零になります。したがって、$i(\sup(D, D'))$ の $\mathfrak{P}$ の係数は零です。 $\mathfrak{P} \cap A \neq (0)$ の場合、高さ 1 の素イデアル $\mathfrak{p}$ ((PDE) による)。 $i(D)$、$i(D')$、$i(\sup(D, D'))$に$\mathfrak{P}$の$e = e(\mathfrak{P}/\mathfrak{p})$、係数を書くと、それぞれ$en(\mathfrak{p}), en'(\mathfrak{p})$、$e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p}))$になります。 $\sup(i(D), i(D'))$のそれは

$$
\sup(e \cdot n(\mathfrak{p}), e \cdot n'(\mathfrak{p})) = e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p})).
$$

これは (b) を証明します。

命題 14 の仮説の下では、(a) から、$C(A)$ から $C(B)$ までの商、準同型 $\bar{i}$ を正規と呼ぶことで、定義するとなり、これをときどき $i$ とも書くことになります。 記法の虐待によって。

条件 (PDE) は、次の 2 つの場合に満たされます。

(1) B は A に関して整数です。この場合、B の *素数イデアル $\mathfrak{P}$ が *高さ* 1 であるためには、*$\mathfrak{p} = \mathfrak{P} \cap A$ が高さ 1 であることが必要かつ十分です。 (0) は、A のイデアル (0) より上にある唯一の素イデアル (章 V, § 2, no. 1, 系 I 命題 1); $\mathfrak{P}$ の高さが 1 の場合、$\mathfrak{p} \neq 0$。 $\mathfrak{p}$ の高さが 1 でない場合、(0) および $\mathfrak{p}$ とは異なる A の素イデアル $\mathfrak{p}'$ が存在し、0 ⊂ p' ⊂ p が成り立ちます。しかし、その場合、B は整域であり、A は積分閉領域であるため、仮定とは反対に、$\mathfrak{p}' \cap A = p'$ と $\mathfrak{p}' \subset \mathfrak{p}$ (章 V, § 2, no. 4, 定理 3) のような B の主理想 $\mathfrak{p}'$ が存在します。逆に、p の高さが 1 の場合、0 および $\mathfrak{p}$ と異なる B の素イデアル $\mathfrak{p}'$ は存在できず、そのような $0 \subset \mathfrak{p}' \subset \mathfrak{p}$ は存在しません。そうでない場合、章 V, § 2, no. 1、系 1 により、$0 \subset \mathfrak{p}' \cap A \subset p$ および $\mathfrak{p}' \cap A$ は 0 および p と区別されます。 命題 1.

(2) B はフラット A-加群です。より正確には:

#### 命題 15 {#ac-vii-s1-prop-15 .statement tag=04ZK}

A と B を、B 含む A がフラット A-加群となるような Krull ドメインとします。次に:
(a) 命題 14 の条件 (PDE) が満たされる。
(b) すべての除数イデアル $a \in A$ に対して、Ba は対応するから因子 $i(\operatorname{div}_A(a))$ までの B の除数イデアルです。

(a) を示すために、$\mathfrak{p} \cap A$ が 0 でも高さ 1 でもない、高さ 1 の B の素イデアル $\mathfrak{p}$ が存在すると仮定します。 $\mathfrak{p} \cap A$ の元 $x \neq 0$ をとります。高さ 1 の A の理想 $p_i$ 含む x は数で有限であり、含む $\mathfrak{p} \cap A$ はありません。したがって、すべての $i$ に対して $y \notin p_i$ となるような $\mathfrak{p} \cap A$ の元 y が存在します (章 II, § 2, no. 1, 命題 2)。したがって、$\operatorname{div}_A(x)$ と $\operatorname{div}_A(y)$ は順序付けされた群 P(A) の相対素数元であるため、$\sup(\operatorname{div}_A(x), \operatorname{div}_A(y)) = \operatorname{div}_A(x) + \operatorname{div}_A(y) = \operatorname{div}_A(xy)$;理想 $Ax \cap Ay$ と $Axy$ は分割的であるため、$Ax \cap Ay = Axy$ であると推定されます。 B はフラットA-加群, $Bx \cap By = Bxy$ (章 I, § 2, no. 6, 命題 6) です。これは、$\sup(v_{\mathfrak{p}}(x), v_{\mathfrak{p}}(y)) = v_{\mathfrak{p}}(xy) = v_{\mathfrak{p}}(x) + v_{\mathfrak{p}}(y)$ が矛盾する不等式 $v_{\mathfrak{p}}(x) > 0, v_{\mathfrak{p}}(y) > 0$ (x と y が $\mathfrak{p}$ にあるので成立します) を意味します。したがって、(a) は不合理な還元によって証明されました。

次に (b) を示します。 $a$ が A の約数イデアルである場合、それは 2 つの分数主イデアル (no. 5、系 2 ～ 命題 9) の共通部分です。

$$
a = d^{-1}(Aa \cap Ab)
$$

ここで、$a, b,$ はあえて$A^*$ に入れます。 B が A に対してフラットであるため、$Ba = d^{-1}(Ba \cap Bb)$ (章 I, § 2, no. 6, 命題 6)、これは Ba が約数であることを示しています。これは、$\operatorname{div}_B(Ba) = \sup(\operatorname{div}_B(a), \operatorname{div}_B(b)) - \operatorname{div}_B(d)$; ということも示しています。 命題 14 (a) と (b) を使用すると、次のことがわかります。

$$
\begin{align*}
\operatorname{div}_B(Ba) &= \sup(i(\operatorname{div}_A(a)), i(\operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\sup(\operatorname{div}_A(a), \operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(Aa \cap Ab)) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(d^{-1}(Aa \cap Ab))) = i(\operatorname{div}_A(a)).
\end{align*}
$$

#### 系 {#ac-vii-s1-n10-cor-1 .statement tag=04ZL}

A をローカル Krull ドメイン、B を離散評価環とし、B が A を支配し、フラット A-加群であるとします。この場合、A は体または離散評価環になります。

$\mathfrak{m}$ を B の最大イデアルとします。(偏微分方程式) により、$\mathfrak{m} \cap A$ は零、つまり高さ 1 です。そのまま、A の最大イデアルである仮定により、主張は no. 7 の命題 11 から続きます。

#### 注意 {#ac-vii-s1-n10-rem-1 .statement tag=04ZM}

上記 2 つのケースのうち前者では、写像 $i : D(A) \to D(B)$ は単射法です。つまり、$P(B)$ の元形基底 $D(B)$ と $P(A)$ できないの 2 つの異なるイデアルは、同じイデアルの A 上の痕跡となります。 $P(B)$、それはすべての $p \in P(A)$ について $i(p) \neq 0$ であることを検証することになります。さて、これは章 V, § 2, no. 1, 定理 1 から続きます。同様に、B が忠実に平坦な A-加群である場合、$i$ は単射法であることがわかります (章 II, § 2, no. 5, 系 4 ～ 命題 11)。

以下では、Krull ドメイン A、B の特定の順序付き対について、$C(A)$ から $C(B)$ までの標準準同型 $\tilde{i}$ を研究することを提案します。

#### 命題 16 {#ac-vii-s1-prop-16 .statement tag=04ZN}

A をザリスキー 環とし、その補完 $\hat{A}$ がクルル領域であるとします。この場合、A はクルール領域であり、$C(A)$ から $C(\hat{A})$ までの標準準同型 $\tilde{i}$ (A はフラット A-加群; cf. 章 III, § 3, no. 4, 定理 3 であるため定義されます) は単射です。

Aは整域と$A \subset \hat{A}$なので、Aは整域です。 L を $\hat{A}$ の分数の体とし、A の K $\subset$ L とします。 $A = \hat{A} \cap K$ (章 III, § 3, no. 5, 系 4 ～ 命題 9) のように、A はクルールドメイン (no. 3, 例 4)。 $\tilde{i} : C(A) \to C(\hat{A})$ が単射であるという事実は、命題 15 (b) から得られ、$b \hat{A}$ が主である場合、b が主であるという事実 (章 III, § 3, no. 5, 系 3 から命題 9)。

ここで、A をクルル領域、S を含む 0 ではなく A の乗法部分集合とします。 群 $D(A)$ (それぞれ $D(S^{-1}A)$) は、$\operatorname{div}(p)$ (それぞれ 2011) の基底集合との自由可換群です。 $\operatorname{div}(S^{-1}p)$)、ここで p は、高さ 1 の A の素イデアルの集合 (それぞれ、$p \cap S = \varnothing$ となる高さ 1 の A の素イデアルの集合) (no. 4, 命題 6) を通過し、$p \cap S = \varnothing$ の場合は、$i(\operatorname{div}(p)) = \operatorname{div}(S^{-1}p)$ になります。したがって、$D(S^{-1}A)$ は、$p \cap S = \varnothing$ となるように、元 $\operatorname{div}(p)$ によって生成された$D(A)$ の直接因子と同一視され、$D(A)$ の自由可換部分群と$\operatorname{div}(p)$ の基底集合を補完するものとして認められます。 $p \cap S \neq \varnothing$;この補数を G で表すことにします。$i : D(A) \to D(S^{-1}A)$ が全射であるように、$i : C(A) \to C(S^{-1}A)$ も全射です。そして:

$$
G/(G \cap F(A)) = (G + F(A))/F(A) = \operatorname{Ker}(\tilde{i});
$$

なぜなら、$D(S^{-1}A)$ の元が $\operatorname{div}_{S^{-1}A}(x/s)$ に等しい場合、$x \in A$ と $s \in S$ は、元本因子 $\operatorname{div}_A(x)$ (命題 14) の$i$ の下で像になります。

ここで、主イデアル $Ap_i$ がすべて素数となるように、S が A の元 $(p_i)_{i \in I}$ の族によって生成されたとします。次に、$p$ が、$p_i$ の冪の $p \cap S \neq \varnothing$、$p$ 含む積、つまり $p_i$ の 1 つである、高さ 1 の A の主イデアルである場合、$p_\alpha$ とします。 $Ap_\alpha$ はゼロ以外の素数であり、$p$ は高さ 1 であるため、$p = Ap_\alpha$ になります。上の記法では、$G \subset F(A)$と(5)は、$\bar{i}$の核が零であることを示しています。したがって、次の結果を示しました。

#### 命題 17 {#ac-vii-s1-prop-17 .statement tag=04ZO}

*$A$をクルールドメイン、$S$を含む$0$ではなく、$A$の乗算部分集合とする。すると、$C(A)$ から $C(S^{-1}A)$ までの標準準同型 $\bar{i}$ は全射になります。さらに $S$ が元 $p_i$ の族によって生成され、主イデアル $Ap_i$ がすべて素数になる場合、$\bar{i}$ は全単射になります。*

公式 (5) の 2 番目の応用として、次の状況を考えてみましょう。$R$ を Krull ドメインとします。 $A$ を多項式環 $A = R[X]$ (no. 9, 命題 13) とし、$S$ を $A$ の非ゼロ定数多項式の集合 $R - (0)$ とします。 $p \cap S \neq \varnothing$ のような高さ 1 の $A$ の主イデアル $p$ は、形 $p_0A$ の主イデアルです。ここで、$p_0$ は高さ 1 の $R$ (no. 9、*注意*) の主イデアルです。したがって、上で紹介した記法では、$\mathrm{div}_A(p_0A)$を$\mathrm{div}_R(p_0)$と同一視することで、$G$が$D(R)$と同一視されます。一方、$G \cap F(A)$ は $F(R)$ と同一視されます。つまり、$R$ 生成するの理想 $a$ が $A = R[X]$ の主要理想 $a_0A = f(X)A$ である場合、$a_0A$ は環の段階的理想であるため、$f(0) \in a_0A$ になります。 $A$ (通常の多項式の次数によって等級付けされる)、したがって $f(0) \in a$;さらに、$a \in a_0A$、$a = f(X)g(X)$ については、$g(X) \in R$、よって、次数 0、$a = f(0)g(0)$ の項を比較します。したがって、$a$ は、$f(0)$ によって生成された $R$ の主な理想であるということになります。最後に、$R$の分数の$K$体で表すと、$S^{-1}A$は多項式環$K[X]$、つまり主イデアル整域と識別されます。したがって $C(S^{-1}A) = (0)$ です。したがって、(5) により、$C(A) = \mathrm{Ker}(\bar{i})$ は $C(R)$ と同一視され、次の結果が証明されました。

#### 命題 18 {#ac-vii-s1-prop-18 .statement tag=04ZP}

*$R$ を Krull ドメイン、$A$ 多項式環 $R[X]$ とします。 $C(R)$ ～ $C(R[X])$ の標準準同型は全単射です*。

### 練習問題 {#ac-vii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
