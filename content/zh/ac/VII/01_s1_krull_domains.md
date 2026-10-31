---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 1
section_title: Krull domains
lang: zh
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
content_sha256: 73ffebc4cc1947821198d879a2413694d910f3f95dfdcb006c0521fdbea0efce
translated_from: content/en/ac/VII/01_s1_krull_domains.md
translation_method: google
source_content_sha256: c7f552328385d94715aa4fc98b5c4522cc8ad73080a081dd41bebfb79b236ea5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 088572f3e8a86758a513bddfcb6432543910d0addc917e1ae9e9f73731b7ec57
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 1. 克鲁尔域

### 1. 整环的 DMSORIAL 理想

#### 定义 1 {#ac-vii-s1-def-1 .statement tag=04YL}

令$A$为整环，$K$为分数的域。 $K$的每个子A模块$a$，使得$A$中存在元素$d \neq 0$，其中$da \subset A$被称为$A$的分数理想$\mathfrak{d}$（或$K$，滥用语言）。

$K$的每个有限生成的子A模块$a$都是分数理想：因为如果$(a_i)_{1 \leq i \leq n}$是$a$的生成元的系统，我们可以写成$a_i = b_i/d_i$，其中$b_i \in A$，$d_i \in A$和$d, \neq 0$；如果$d = d_1 \ldots d_n$，显然是$da \subset A$。特别是 $K$ 的单生子 A 模是分数理想（回想一下，它们在代数、章 VI, § 1, no. 5 中被称为分数主理想）。如果 $A$ 是诺特，则每个分数理想都会无限生成 A-模。 $A$ 分数理想的每个子 A 模都是分数理想。 $A$ 的每个理想都是分数理想；为了避免混淆，这些也被称为$A$的积分理想。

我们用$I(A)$集合表示$A$的非零分数理想。给定$I(A)$的两个元素$a, b$，我们将为关系写$a \prec b$（或$b \succ a$）“每个分数主理想包含$a$也包含$b$”；显然这个关系是在$I(A)$上预购的。让$R$表示关联的等价关系“$a \prec b$和$b \prec a$”（集合理论，章III, § 1, no. 2）和$D(A)$商集$I(A)/R$；我们可以说，$D(A)$的元素是$A$的除子，并且对于每个分数理想$a \in I(A)$，我们将用$D(A)$中的$a$的$\operatorname{div} a$（或$\operatorname{div}, a$）典范像表示，并且我们应该说$\operatorname{div} a$是$a$的除子$\mathfrak{d}$；如果$a = Ax$是分数主理想，我们写div(x)而不是div(Ax)，div(x)被称为x的除子； 形式 div(x) 的 D(A) 的元素称为主除子。通过取商，I(A) 上的预排序$\prec$ D(A) 上的定义，我们将用$\leqslant$ 表示。

对于所有$a \in I(A)$，A 中存在假设一些$d \neq 0$，使得$a \subset Ad - 1$；因此，分数主理想包含 a 的交 $\tilde{a}$ 是 I(A) 的元素。显然关系$a \prec b$等价于关系$\tilde{a} \supset 6$；因此关系$a \supset b$意味着$a \prec b$。为了使 I(A) 的两个元素 $a, b$ 等效于模 R，$\tilde{a} = 6$ 是充分必要的。

#### 定义 2 {#ac-vii-s1-def-2 .statement tag=04YM}

*I(A) 的每个元素 a 使得 $a = \tilde{a}$ 称为 A 的除数分数理想。*

在其他字中，除数理想只是一个非空分数主理想族的非零交。每个非零交的除数理想都是除数理想。如果 a 是除数，则 ax 对于所有 $x \in K^*$，映射 $b \mapsto bx$ 是分数主理想的集合的双射到自身，对于所有 $a \in I(A)$，6 是最小除数理想包含 a 并且相当于模 R。此外，如果$b$ 是除数理想，相当于模 R，然后是 $\tilde{a} = 6 = b$。因此 5 是唯一的除数理想 $b$，使得 div $a =$ div $b$ （在除数理想的其他字中，映射 $a \mapsto$ div $a$ 到集合的限制是单射的）。

令 a 和 b 为 K 的两个分数理想。回想一下 (章 I, § 2, no. 10)，$b : a$ 表示 $x \in K$ 的集合，使得 $xa \subset b$；这显然是A-模；如果 $b \in I(A)$ 和 $a \in I(A)$，则 $b : a \in I(A)$；因为如果$d$是A的非零元素，使得$db \subset A$和$da \subset A$以及$a$是$A \cap a$的非零元素，则$da(b : a) \subset A$；另一方面，如果$b \neq 0$属于到$b$，则$bda \subset b$，因此$bd \in b : a$和$b : a \neq 0$。

$b : a$的定义也可以写成：

$$
(1) \quad b : a = \bigcap_{x \in a, x \neq 0} b x^{-1}.
$$

#### 命题 1 {#ac-vii-s1-prop-1 .statement tag=04YN}

(a) *如果 b 是除数理想且 $a \in I(A)$，则 $b : a$ 是除数。*

(b) *设a、b在I(A)中。在阶那个div$a =$div$b$中，$A : a = A : b$是必要且充分的。*

(c) *对于所有 $a \in I(A)$、$6 = A : (A : a)$。*

断言 (a) 直接从等式 (1) 得出，因为如果 $b$ 是除数，则对于所有 $x \neq 0$，$b x^{-1}$ 也是除数。

为了显示 (b)，令 $P(a)$ 表示分数主理想包含 a 的集合； 关系 $Ax \in P(a)$ 相当于$x^{-1} a \subset A$，因此也相当于$x^{-1} \in A : a$。由于关系 div $a =$ div $b$ 通过定义等价于 $P(a) = P(b)$，因此也等价于 $A : a = A : b$。

最后为$a(A : a) \subset A, a \subset A : (A : a)$。在这个公式中，替换$a$乘以$A : a$，可见$A : a \subset A : (A : (A : a))$；另一方面，关系$a \subset A : (A : a)$意味着
$$
A : a \supset A : (A : (A : a)).
$$
因此 $A : a = A : (A : (A : a))$ 并且从 (b) 可以得出 $\operatorname{div} a = \operatorname{div}(A : (A : a))$
由于$A : (A : a)$能被(a)整除，当然也有$6 = A : (A : a)$，这就证明了(c)。

#### 注 {#ac-vii-s1-n1-rem-1 .statement tag=04YO}

在上述证明的过程中，已经证明了$A : a = A : (A : (A : a))$对于每一个理想$a \in I(A)$，这是*集合理论*、章111、§ 1, no. 5、命题2的特例。

#### 命题 2 {#ac-vii-s1-prop-2 .statement tag=04YP}

(i) *在 $D(A)$ 中，上面有界的每个非空集合至少承认上界。更准确地说，如果 $(a_i)$ 是 $I(A)$ 的元素的非空族，并且在上面有界，那么*
$$
\sup(\operatorname{div} a_i) = \operatorname{div}\left( \bigcap_i 5_i \right).
$$
(ii) *在$D(A)$中，每个有界的非空集合都承认下确界。更准确地说，如果 $(a_i)$ 是 $I(A)$ 的元素的非空族，其下界如下，那么*
$$
\inf(\operatorname{div} a_i) = \operatorname{div}\left( \sum_i a_i \right).
$$
(iii) *集合 $D(A)$ 是一个格子。*

令 $(a_i)$ 为 $I(A)$ 的元素的非空族，其上界。如果说一个除数理想$b$将这个族限制在上面，那么等于说它包含在所有$a_i$中，也就是说$b$包含在$\bigcap_i 6_i$中。因此 $\bigcap_i a_i \neq (0)$ 和 $\bigcap_i 6_i$ 是一个除理想，它显示 (i)。

现在让 $(6_i)$ 成为 $I(A)$ 的元素的非空族，其边界如下。说除数理想 $b$ 限制了下面这个族，意味着它包含所有$a_i$，也就是说（因为$b$是除数）它包含所有$a_i$，或者也$b \supset \sum_i a_i$。这就证明了(ii)。

最后，为了证明(iii)，由(i)和(ii)足以证明，如果$a, b$在$I(A)$中，则集合$\{a, b\}$在$I(A)$中上下界；现在它的边界是$a \cap b$（与$(0)$不同）。对于$a + b \in I(A)$，它的边界是$a + b$：如果$d$和$d'$是$A$的非零元素，使得$da \subset A$和$d'b \subset A$，则$dd'(a + b) \subset A$。

#### 推论{#ac-vii-s1-n1-cor-1 .statement tag=04YQ}

*如果$x, y$和$x + y$在$K^*$中，则$\operatorname{div}(x + y) \geq \inf(\operatorname{div}(x), \operatorname{div}(y))$。*

$A(x + y) \subset Ax + Ay$，因此$\operatorname{div}(x + y) \geq \operatorname{div}(Ax + Ay)$。

### 2. D(A) 上的幺半群结构

#### 命题 3 {#ac-vii-s1-prop-3 .statement tag=04YR}

设$a, a', b, b'$为$I(A)$的元素。 关系 $a > a'$ 和$b > b'$ 意味着$ab > a'b'$。

我们可以将注意力限制在$b = b'$的情况。则设$Ax$为分数主理想包含$a'b$；对于$b$、$Ax \supset a'y$的每个非零元素$y$，以及$Axy^{-1} \supset a'$、从而$Axy^{-1} \supset a$和$Ax \supset ay$。变化$y$，可以看出$Ax \supset ab$，从而$ab > a'b$。

从命题 3 可以得出$I(A)$ 定义上的乘法，通过经过得到合成在$D(A)$ 上的商律，显然是结合律和交换律。它是附加的，这样我们就可以写：

$$
\text{div}(ab) = \text{div } a + \text{div } b,
$$

$I(A)$ 中的 $a, b$。显然，对于这个加法，$\text{div}(1)$ 是单位元素；这个元素用0表示。命题3进一步证明$D(A)$上的阶结构与这个加法*相容的*（*代数*，章VI, § 1, no. 1），更准确地说（no. 1、命题 2 (ii)）：

$$
\inf(\text{div } a + \text{div } b, \text{div } a + \text{div } c) = \inf(\text{div}(ab), \text{div}(ac)) = \text{div}(ab + ac)
= \text{div}(a(b + c)) = \text{div} a + \text{div}(b + c) = \text{div} a + \inf(\text{div } b, \text{div } c).
$$

对于分数理想$a \neq 0$，在$D(A)$中，$\text{div } a \geq 0$是这样的，$a \subset A$是必要且充分的（在其他字中，$a$是$A$的*整的*理想）。

对于$K^*$中的两个元素$x, y$，关系$\text{div}(x) = \text{div}(y)$相当于$Ax = Ay$； $A$的主除子与序关系以及由$D(A)$上的主律诱导的幺半群集合是一个*有序的群*规范同构于由相反的序关系排序的分数主理想的乘法群包含（*代数*，章VI, § 1, no. 5）。 关系 $S$ 两个元素 $P, Q$ 与 $D(A)$ 之间：

“存在$x \in K^*$使得$P = Q + \text{div}(x)$”

因此是等价关系，因为关系$P = Q + \text{div}(x)$等价于$Q = P + \text{div}(x^{-1})$；如果$P$和$Q$模$S$全等，则它们被称为*等价于$A$的除子*。显然，关系$S$与幺半群$D(A)$的律兼容，因此后者定义，通过取商，在$D(A)/S$上得到幺半群结构；这个幺半群被称为 A* 的 *除子类幺半群。

#### 命题 4 {#ac-vii-s1-prop-4 .statement tag=04YS}

令 $a, b$ 为 $A$ 的两个除数分数理想。以下属性是等效的：
(a) $\text{div } a$和$\text{div } b$等价于除子；
(b) 存在$x \in K^*$使得$b = xa$。

如果$\operatorname{div} b = \operatorname{div} a + \operatorname{div}(x)$对于某些$x \in K^*$，则$\operatorname{div} b = \operatorname{div}(xa)$，并且由于$b$和$xa$是除数，$b = xa$，这证明了命题。

令 $a$ 为可逆分数理想 (章 II, § 5, no. 6)；那么 $a = A : (A : a)$ (*loc.cit.*, 命题 10) 因此 $a$ 是 *除数* (no. 1, 命题 1)。因此，可逆分数理想的群$J(A)$可与幺半群$D(A)$的子群和$D(A)/S$中$J(A)$的典范像以及*射影*的类的群识别$A$-*秩* 1 的模块（章 II, § 5, no. 7，推论 2 至命题 12 和 *注* 1）。

#### 定理 1 {#ac-vii-s1-thm-1 .statement tag=04YT}

*令$A$为整环。对于$A$的除子的幺半群$D(A)$为群，$A$完全积分闭是充分必要的。*

假设$D(A)$是群。让$x \in K$；假设$A[x]$包含在$K$的有限生成的子$A$模块中。然后我们看到(no. 1)$a = A[x]$是$I(A)$的元素。然后$xa \subset a$，因此$\operatorname{div}(x) + \operatorname{div} a \geq \operatorname{div} a$。由于$D(A)$是有序的群，我们将结论表示$\operatorname{div}(x) \geq 0$、从而$x \in A$。因此$A$是完全整体封闭的（章V, § 1，编号**4**，定义5）。

相反，假设$A$是完全积分闭的。令 $a$ 为除数理想。我们将证明$\operatorname{div} a + \operatorname{div}(A : a) = 0$，这将证明$D(A)$是群。作为 $a(A : a) \subset A$，足以 (no. 1) 验证每个分数主理想 $Ax^{-1}$ 其中包含 $a(A : a)$ 也包含 $A$。现在，对于$y \in K^*$，关系$Ay \supset a$意味着$y^{-1} \in A : a$，从而$y^{-1}a \subset a(A : a) \subset Ax^{-1}$，因此$xa \subset Ay$。由于 $a$ 是除数，因此我们对所有 $n \in \mathbf{N}$ 推出 $xa \subset a$、从而 $x^n a \subset a$。存在$K^*$的元素$x_0, x_1$使得$Ax_0 \subset a \subset Ax_1$；因此$x^n x_0 \in Ax_1$，从而$x^n \in Ax_1 x_0^{-1}$。由于$A$是全积分闭的，$x \in A$，即$Ax^{-1} \supset A$，完成证明。

注，如果$A$完全积分闭（甚至诺特），则$A$的除数理想不一定是可逆的，在其他字中，一般来说$J(A) \neq D(A)$（习题2和§ 3, no. 2， 命题 1)。

#### 推论 {#ac-vii-s1-n2-cor-1 .statement tag=04YU}

*令$A$为完全积分闭域，$a$为$A$的除数分数理想。然后，对于 $A$ 的每个分数理想 $b \neq 0$，$\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b$*

凭借no. 1的公式(1)：

$$
\operatorname{div}(a : b) = \operatorname{div}\left( \bigcap_{y \in b, y \neq 0} y^{-1}a \right) = \sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a)
$$

考虑到命题 2 以及分数理想 $y^{-1}a$ 是除数的事实。但由于 $D(A)$ 是有序的群 (*代数*, 章 VI, § 1, no. 8)：

$$
\sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a) = \sup_{y \in b, y \neq 0} (\operatorname{div} a - \operatorname{div}(y)) \\
= \operatorname{div} a - \inf_{y \in b, y \neq 0} \operatorname{div}(y) = \operatorname{div} a - \operatorname{div} b.
$$

### 3.克鲁尔领域

#### 定义 3 {#ac-vii-s1-def-3 .statement tag=04YV}

如果存在对域的分数 $K$ 的 $A$ 进行估值的$(v_i)_{i \in I}$族，且具有以下属性，则 n 整环 $A$ 称为克鲁尔域：
(AK$_I$) 估值$v_i$是离散的；
(AK$_{II}$)$v_i$环交为$A$；
(AK$_{III}$) 对于所有 $x \in K^*$、集合或指标 $t \in I$，使得 $v_t(x) \neq 0$ 是有限的。

显然，验证 $A - (0)$ 的元素 $x$ 的条件 (AK$_{III}$) 就足够了。

例
(1) 每个离散估值环都是一个Krull域。
(2) 更一般地，每个主理想整环$A$都是一个Krull域。令$(p_i)_{i \in I}$为$A$的极值元素的代表系统，令$v_i$为由$p_i$定义的$A$的分数域的估值（章VI, § 3, no. 3， 例4)。立即可见族$(v_i)_{i \in I}$满足性质(AK$_I$)、(AK$_II$)和(AK$_{III}$)。
(3) 设$F$为域，$(R_i)_{1 \leq i \leq n}$为$F$的子环的有限族，它们是Krull域。那么他们的交$S = \bigcap_{j=1}^n R_j$，就是一个Krull域。对于 $1 \leq j \leq n$ 令 $(v_{j,t})_{t \in I_j}$ 为 $R_j$、满足 (AK$_I$)、(AK$_{II}$)、(AK$_{III}$) 的分数域的评估族（其中 $A$ 替换为$R_j$）。让$w_{j,t}$表示$S$分数中$v_{j,t}$到域的限制。那么族$(v_{j,t})_{1 \leq j \leq n, t \in I_j}$显然满足(AK$_{II}$)(其中$A$被$S$替代)并且也满足(AK$_{III}$)，因为指标$j$的集合是有限的。估值$w_{j,t}$要么是离散的，要么是不正确的。通过仅保留那些离散的，可以获得明显满足（AK$_I$）、（AK$_{II}$）和（AK$_{,,}$）的族（其中$A$被$S$替代）。因此 $S$ 肯定是一个 Krull 域。
(4) 特别地，如果$A$是Krull域，并且分数的域、$A$的$K$、$K'$、子域，则$K' \cap A$是Krull域。

#### 定理 2 {#ac-vii-s1-thm-2 .statement tag=04YW}

令$A$为整环。要使$A$成为克鲁尔域，满足以下两个条件是必要且充分的：
(a)$A$完全整体封闭；
(b) $A$ 的每个非空除积分理想族都承认极大元素（相对于关系$\subset$）。
此外，如果$P(A)$是$D(A)$的极值元素的集合，则$P(A)$是$\mathbf{Z}$模$D(A)$的基，$D(A)$的正元素是线性组合 / 元素 / $P(A)$，系数为$\geq 0$。

令 $A$ 为克鲁尔域。它是完全整体封闭的（章VI, § 4, no. 5，推论命题9）。令$(v_i)_{i \in I}$为$A$满足（AK$_I$）、（AK$_{II}$）和（AK$_{III}$）的分数$K$的域的估值族。 $v_i$ 可以假设是标准化的 (章 VI, § 3, no. 6, 定义 3)。对于所有$a \in I(A)$，我们应该写：

$$
v_t(a) = \sup_{a \subset Ax} (v_t(x));
$$

那么$v_t(a) \in \mathbf{Z}$，对于，如果$a$是$a$的非零元素，关系$Ax \supset Aa$意味着$v_t(x) \leq v_t(a)$（通过（AK$_{III}$）），这表明$v_t(x)$（$a \subset Ax$）的族上面有界。我们建立以下属性：

(1) *令$a$为除数分数理想；在阶和 $y \in a$ 中，$v_t(y) \geq v_t(a)$ 对于所有 $t \in I$ 是必要且充分的。*

由于$a$是除数，关系$y \in a$等价于关系““$a \subset Ax$意味着$y \in Ax$”。现在，通过（AK$_{II}$），关系$y \in Ax$等价于“$v_t(y) \geq v_t(x)$” $t \in I$”。从而 (1)。

(2) *设$a$和$b$为$A$的两个除数分数理想；在阶和 $a \subset b$ 中，$v_t(a) \geq v_t(b)$ 对于所有 $t \in I$ 是必要且充分的。*

这紧随性质 (1) 而来。

(3) *如果$x \in K^*$，则$v_t(Ax) = v_t(x)$。*

如果$Ay \supset Ax$，则$v_t(y) \leq v_t(x)$除以(AK$_{II}$)，并且在$y = x$处取$v_t(y)$的最小值。

(4) *对于所有 $a \in I(A)$、指标 $t \in I$，使得 $v_t(a) \neq 0$ 在数中是有限的。*

$K^*$中存在$x, y$使得$Ax \subset a \subset Ay$。根据性质 (2) 和 (3)，对于所有 $t \in I$，$v_t(x) \geq v_t(a) \geq v_t(y)$。然后就可以申请（AK$_{III}$）。

因此，我们展示了以下引理：

#### 引理 1 {#ac-vii-s1-lem-1 .statement tag=04YX}

*If $A$ is a Krull domain and $(v_t)_t$, is a family of normed valuations on $K$ satisfying (AK$_I$), (AK$_{II}$) and (AK$_{III}$), the mapping $a \mapsto (v_t(a))_{t \in I}$ is a decreasing injective mapping of the set of divisorial integer ideals of $A$ (ordered by $\subset$) to the set of positive elements & the ordered group the direct sum $\mathbf{Z}^{(I)}$.*

既然如此，$\mathbf{Z}^{(I)}$的每个非空正集元素都有一个最小的元素（*代数*，章VI, § 1, no. 13，定理2）。因此$A$当然满足叙述的性质(b)。

相反，令$A$为叙述的整环满足性质(a)和(b)。由于 $A$ 是完全积分闭的，$D(A)$ 是有序的群 (no. 2, 定理 1)。这个群是一个格子（no. 1，命题2）。到叙述的条件 (b) 时，$D(A)$ 的正元素的每个非空族都具有最小元素。令$P(A)$为$D(A)$的极值元素的集合。那么 (*代数*, 章 VI, § 1, no. 13, 定理 2) $P(A)$ 是 $\mathbf{Z}$ 模 $D(A)$ 的基，$D(A)$ 的正元素是线性组合， 正整数元素的系数$P(A)$。

因此，对于$x \in K^*$，有理数整数$v_P(x)$（对于$P \in P(A)$）定义如下：

$$
\text{div}(x) = \sum_{P \in P(A)} v_P(x) \cdot P.
$$

我们还写$v_P(0) = +\infty$。

从关系

$$
\text{div}(xy) = \text{div}(x) + \text{div}(y)
$$

和

$$
\text{div}(x + y) \geq \inf(\text{div}(x), \text{div}(y)),
$$

对于$K^*$中的$x, y$和$x + y$，我们推断$v_P$是$K$的*离散估值*。在阶那个$x \in A$中，$\text{div}(x) \geq 0$是必要且充分的，即对于所有$P \in P(A)$来说$v_P(x) \geq 0$。因此 $v_P$ 满足条件 (AK$_1$) 和 (AK$_{11}$) 显然还有 (AK$_{III}$)。

#### 推出{#ac-vii-s1-n3-cor-1 .statement tag=04YY}

*要使诺特环成为 Krull 域，它是全闭域是充分必要的。*

积分闭域诺特域是完全积分闭域 (章 V, § 1, no. 4)。

存在非诺特克鲁尔域，对于例多项式环 $K[X_n]_{n \in \mathbf{N}}$ 超过域 $K$ 的无限个不定数 (cf. 习题 8)。

### 4. 克鲁尔领域的基本评估

令$A$为克鲁尔域，$K$为分数的域。由no. 3（对于$x \in K^*$）的公式（4）定义的估值称为$K$（*或*$A$）的*基本估值*。

我们在定理 2 的证明过程中注意到，$v_P$ 满足属性 (AK$_1$)、(AK$_2$) 和 (AK$_{III}$) 定义 3 的估值。此外，这些离散估值 $v_P$ 是*标准化的*：对于每个极值除子、$P \in P(A)$、$P < 2P$，因此，如果$a$和$b$是除数理想相应的到$P$和$2P$，则$a \supseteq b$和$a \neq b$；对于$x \in a - b$，$\text{div}(x) \geq P$和$\text{div}(x) \not\geq 2P$，从而$v_P(x) = 1$，这证明了我们的断言。

#### 命题 5 {#ac-vii-s1-prop-5 .statement tag=04YZ}

*令$A$为克鲁尔域，$K$为分数的域，以及$(v_P)_{P \in P(A)}$其基本估值系列。令 $(n_P)_{P \in P(A)}$ 为有理数整数族，除了指标的有限数外，其余为零。然后$x \in K$的集合使得$v_P(x) \geq n_P$对于所有$P \in P(A)$来说是$A$的除数理想$a$使得$\text{div } a = \sum_{P \in P(A)} n_P \cdot P$。*

让$x \in K^*$。在阶 $x \in a$ 中，$Ax \subset a$ 是必要且充分的，因此 $\text{div}(x) \geq \text{div } a$ ，因此，根据 (4)，对于所有 $P \in P(A)$ ，$v_P(x) \geq n_P$ 是必要且充分的。

#### 命题 6 {#ac-vii-s1-prop-6 .statement tag=04Z0}

令$A$是一个Krull域，$K$其分数的域，$(v_t)_{t \in I}$对$K$的一系列评估，具有定义3和$A$，环的$v_t$属性。令$S$是$A$的乘法子集，而不是包含$0$和$J$集合与指标$t \in I$，使得$v_t$是零 $S$。然后$S^{-1}A = \bigcap_{t \in J} A_t$；特别是$S^{-1}A$是一个Krull域。

我们写$B = \bigcap_{t \in J} A_t$。然后是$S^{-1} \subset B$和$A \subset B$，然后是$S^{-1}A \subset B$。相反，设$x \in B$。让$J'$表示指标$t$的有限集合，使得$v_t(x) < 0$。如果$t \in J'$，则$x \notin A_t$，因此$t \notin J$，因此存在$s_t \in S$使得$v_t(s_t) > 0$。令$n(t)$为整数$> 0$，使得$v_t(s_t^{n(t)}x) \geq 0$；我们写$s = \prod_{t \in J'} s_t^{n(t)}$。然后 $v_t(sx) \geq 0$ 对于所有 $t \in I$，因此$sx \in A$ 和 $x \in S^{-1}A$。因此$B = S^{-1}A$。

#### 推论 1 {#ac-vii-s1-prop-6-cor-1 .statement tag=04Z1}

令$P$为$A$和$p$相应的除理想的极值除子。则$p$是质数，$v_P$的环是$A$，$v_P$的剩余类域与$A/p$的分数的域进行识别。

让$S = A - p$。到命题 5 时，$v_P$ 是 $S$ 上的零，以及 $p$ 上的 $> 0$。因此$p$是$A$的交，也是$v_P$的理想，因此是素数。另一方面，对于每个极值除子 $Q \neq P$、$Q \not\subset P$，因此除数理想 $q$ 相应的到 $Q$ 不包含在 $p$ 中；因此$q \cap S \neq \varnothing$，因此，到命题 5，$v_Q$ 不再是$S$ 上的零。既然如此，则由命题 6 和章 II, § 3, no. 1、命题 3 得出推论。

#### 推论 2 {#ac-vii-s1-prop-6-cor-2 .statement tag=04Z2}

令$A$是一个克鲁尔域，$K$是分数和$(v_t)_{t \in I}$的域，具有定义3属性的评估族。那么$A$的每个基本评估都相当于$v_t$之一。

令$P$为$A$和$p$相应的除理想的极值除子。根据推论1、命题 5、引理 1 和断言 (1)，在定理 2、no. 3 的证明中，存在$t \in I$，使得$v_t$ 的环 $A_t$ 包含环$A$，共$v_P$。由于$v_t$和$v_P$的高度为1，因此它们是等价的（章VI, § 4, no. 5，命题6）。

#### 命题 7 {#ac-vii-s1-prop-7 .statement tag=04Z3}

令 $A$ 为克鲁尔域，$(v_P)_{P \in P(A)}$ 为其基本估值系列，$a \in I(A)$。那么$\operatorname{div} a$中$P$的系数就是$\inf_{y \in a} (v_P(y))$。如果$p$是极值除子$P$的除素理想相应的，则$aA_p = \tilde{a}A_p$。

由于 $a = \sum_{y \in a} Ax$, 命题 2 (b) (no. 1) 表明 $\operatorname{div}(a) = \inf_{x \in a} (\operatorname{div}(Ax))$, 从而我们的第一个断言。第二个紧随其后，因为$\operatorname{div} \tilde{a} = \operatorname{div} a$和$A_p$是离散估值$v_P$的环。

#### 命题 8 {#ac-vii-s1-prop-8 .statement tag=04Z4}

设$A$为积分闭域诺特。
(a) 设$P$为$A$和$p$相应的除数素理想的极值除子；

对于$n \in \mathbf{N}$，设$p^{(n)} = p^n A_p \cap A$；那么$p^{(n)}$是$x \in A$的集合，使得$v_p(x) \geq n$是$p$-初等理想。

(b) 设 $a$ 为除数理想积分，$n_1 P_1 + \ldots + n_r P_r$ 除子为 $a$（$P_i$ 为不同极值除子），$p_i$ 为除数素理想相应的至 $P_i$。那么$a = \bigcap_{i=1}^r p_i^{(n_i)}$是$a$的唯一减少的初等分解并且$p_i$没有被浸入。

由推论1到命题6，关系$x \in p^n A_p = (pA_p)^n$等价于$v_p(x) \geq n$；另一方面，由于$A$是离散估值环，$(pA_p)^n$是$(pA_p)$-主要（章IV, § 2, no. 1，例4），因此$p^{(n)}$是$p$-主要（章） IV, § 2, no. 1、命题 3)；这显示了（a）。 命题 5 当然表明$a = \bigcap_{i=1}^r p_i^{(n_i)}$。由于$p_i \not\subset p_j$对于$i \neq j$来说，初等分解被减少：因为如果$p_i^{(n_i)} \supset \bigcap_{j \neq i} p_j^{(n_j)} \supset \prod_{j \neq i} p_j^{(n_j)}$，$p_{ji}$将是包含对于$j \neq i$的$p_j$之一（章II, § 1, no. 1， 命题 1)。 唯一性源自章 IV, § 2, no. 3、命题 5。

### 5. 基本估值的近似值

由于克鲁尔域的基本估值是离散且规范的，因此没有两个是等价的，因此它们是独立的（章VI, § 7, no. 2）。因此，近似定理的推论 2（前述，定理 1）可以应用于它们：给定一些 $n_i \in \mathbf{Z}$ 和一些基本估值 $v_i$ 在数中有限且不同，存​​在 $x \in K$，使得对于所有 $i$ 都有 $v_i(x) = n_i$。但这里有一个更精确的结果：

#### 命题 9 {#ac-vii-s1-prop-9 .statement tag=04Z5}

令$v_1, \ldots, v_r$为克鲁尔域$A$和$n_1, \ldots, n_r$有理整数的不同基本估值。 There exists an element $x$ of the field of fractions $K$ of $A$ such $v_i(x) = n_i$ for $1 \leq i \leq r$ and $v(x) \geq 0$ for every essential valuation $v$ of $A$ distinct from $v_1, \ldots, v_r$.

令$p_1, \ldots, p_r$为$A$相应的与估值$v_1, \ldots, v_r$的除理想。 存在$y \in K$使得$v_i(y) = n_i$对应$1 \leq i \leq r$（章VI, § 7, no. 2，推论1到定理1）。 $A$的基本估值$w_1, \ldots, w_s$与$v_i$不同，其中整数$w_j(y) = -m_j$为$< 0$，在数中是有限的；设$q_1, \ldots, q_s$为相应的理想。 $p_1, \ldots, p_r, q_1, \ldots, q_s$之间不存在关系，因为这些理想对应到极值除子并且这些理想是素数（推论1到命题6）。 因此，积分理想$a = q_1^{m_1} \ldots q_s^{m_s}$不包含在任何$p_i$（章11，§ 1, no. 1，命题1）中，因此也不包含在它们的并（前述，命题2）中。 因此存在$z \in a$使得$z \notin p_i$对于$1 \leq i \leq r$；然后 $v_1(z) = \cdots = v_r(z) = 0$ 和 $w_j(z) \geq m_j$ $1 \leq j \leq s$；因此元素$x = yz$解决了问题。

#### 推论 1 {#ac-vii-s1-prop-9-cor-1 .statement tag=04Z6}

令$\mathbf{A}$为克鲁尔域，$\mathbf{K}$是分数和$\mathbf{a}, \mathbf{b}$的域和$c$$\mathbf{A}$的三个除数分数理想，使得$\mathbf{a} \subset \mathbf{b}$。存在$x \in \mathbf{K}$使得$\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$。

Let $(v_t)_{t \in I}$ be the family of essential valuations of $\mathbf{A}$ and let $(m_t)$ (resp. $(n_t), (p_t)$) be the family of rational integers (zero except for a finite number of indices) such that $\mathbf{a}$ (resp. $\mathbf{b}, c$) is the set of $x \in \mathbf{K}$ for which $v_t(x) \geq m_t$ (resp. $n_t, p_t$) for all $t \in I$ (Proposition 5, no. 4). $t \in I$ 的集合 $\mathbf{J}$ 使得 $m_t > n_t$ 是有限的。 由于$p_t = m_t = 0$除了指标的有限数之外，命题9表明存在$x \in \mathbf{K}^*$使得$v_t(x^{-1}) + m_t = p_t$对于$t \in \mathbf{J}$并且
$$
v_t(x^{-1}) + m_t \geq p_t
$$
$t \in I - \mathbf{J}$。 然后，对于所有$t \in I$，$m_t = \sup(n_t, v_t(x) + p_t)$。 从而$\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$。

#### 推论 2 {#ac-vii-s1-prop-9-cor-2 .statement tag=04Z7}

令 $\mathbf{A}$ 为克鲁尔域。对于 $\mathbf{A}$ 的分数理想 $\mathbf{a}$ 而言，它是两个分数主理想的交是必要且充分的。

充分性是显而易见的（no. 1，定义2）。必然性来自推论1：以$b$和$c$为主，且$b \supseteq a$。

### 6. 克鲁尔域中高度 1 的素理想

#### 定义 4 {#ac-vii-s1-def-4 .statement tag=04Z8}

设$\mathbf{A}$为整环。如果 $\mathbf{A}$ 的素理想 $\mathfrak{p}$ 在 $\mathbf{A}$ 的非零素理想中最小，则称其高度为 1。

我们还可以说理想的 $(0)$ 的高度为 0；因此，高度 $\leq 1$ 的首要理想是定义等于 $(0)$ 或高度 1。

一般而言，我们将定义低于素理想的高度。

#### 定理 3 {#ac-vii-s1-thm-3 .statement tag=04Z9}

令$\mathbf{A}$为克鲁尔域，$\mathfrak{p}$为$\mathbf{A}$的积分理想。为了使$\mathfrak{p}$成为极值除子的除数理想相应的，$\mathfrak{p}$是高度为1的素理想是充分必要的。

如果$\mathfrak{p}$是极值除子的除数理想相应的，我们知道（no. 4，推论1到命题6）$\mathfrak{p}$是素数，$\mathbf{A}_\mathfrak{p}$是离散估值环；由于$\mathbf{A}_\mathfrak{p}$除了$(0)$和$\mathfrak{p}\mathbf{A}_\mathfrak{p}$之外没有素理想，$(0)$和$\mathfrak{p}$是$\mathfrak{p}$中包含的$\mathbf{A}$唯一的素理想（章II, § 3, no. 1，命题3）；因此$\mathfrak{p}$的高度为1。相反，我们首先要证明$\mathbf{A}$包含的每个素理想$\mathfrak{p} \neq (0)$都是除数素理想$\mathfrak{q}$相应的到极值除子：因为，如$\mathbf{A}_\mathfrak{p} \neq K$， $\mathbf{A}_\mathfrak{p}$是非空家庭的交基本估价环的$(\mathbf{A}_t)$（no. 4，命题6）；每个$\mathbf{A}_t$都是形式$\mathbf{A}_{\mathfrak{q}_t}$（no. 4，推论1到命题6），并且从$\mathbf{A}_\mathfrak{p} \subset \mathbf{A}_{\mathfrak{q}_t}$我们推导出$\mathfrak{q}_t \subset \mathfrak{p}$。因此，如果$\mathfrak{p}$的高度为1，则$\mathfrak{p} = \mathfrak{q}$，这表明$\mathfrak{p}$是极值除子的除理想相应的。

#### 推出 1 {#ac-vii-s1-thm-3-cor-1 .statement tag=04ZA}

在克鲁尔域中，每个非零素理想 m 包含都是高度为 1 的素理想。如果 m 的高度不是 1，则 div m = 0 且 A : m = A。

第一个断言已经在定理3的证明过程中看到过。如果m不是高度1，并且p是m中包含的高度1的素理想，则p ⊂ m̃且p ≠ m̃；由于 div p 是极值，因此必然 div m = div m̃ = 0；因此 div(A : m) = 0 并且，由于 A : m 是除数 (no. 1, 命题 1)，A : m = A。

#### 推出 2 {#ac-vii-s1-thm-3-cor-2 .statement tag=04ZB}

令 A 为克鲁尔域，K 为分数的域，v 为 K 的估值，对 A 为正，x ∈ A 的 p 集合使得 v(x) > 0。如果素理想 p 的高度为 1，则 v 相当于 A 的基本估值。

设 B 为 v 的环，m 为理想值。那么 m ∩ A = p，因此 A_p ⊂ B。现在 A_p 是离散估值环（定理 3 和推论 1 到命题 6）。由于 p ≠ (0)，B ≠ K，因此 B = A，(章 VI, § 4, no. 5，命题 6)。

#### 定理 4 {#ac-vii-s1-thm-4 .statement tag=04ZC}

设 A 为高度为 1 的素理想的整环且 M 集合。对于 A 为克鲁尔域，满足以下性质是必要且充分的：
(i) 对于所有 p ∈ M, A，是一个离散估值环。
(ii) 对于 p ∈ M，A 是 A_p 的交。
(iii) 对于 A 中所有 x ≠ 0，仅存在有限数理想 p ∈ M 使得 x ∈ p。
此外，对于 p ∈ M 的 A_p 的估值相应的是 A 的基本估值。

条件就足够了。它们的必要性紧随no. 4的定理3，推论I到命题6，以及no. 3的定义3的满足条件的基本评估这一事实。

#### 命题 10 {#ac-vii-s1-prop-10 .statement tag=04ZD}

设 A 是一个积分闭域诺特 ，并且是 A 的积分理想。以下条件是等价的：
(a) a 是除数；
(b) 与 A/a 相关的素理想的高度为 1。

回想一下，如果 a = $\bigcap^n q_i$ 是 a 的约化初等分解，并且 p_i 表示 q_i 的素理想相应的，则与 A/a 相关的素理想就是 p_i (章 IV, § 2, no. 3，命题 4)。 (a) 蕴含 (b) 的事实是从 no. 4 的命题 8 得出的。相反，如果在上面的记号中，p_i的高度为1，则A_{p_i}是离散估值环(定理4)；现在，q_i = q_i A_{p_i} ∩ A (章 IV, § 2, no. 1, 命题 3)；用 v_i 表示对 p_i 的基本评估相应的，因此存在整数 n_i，使得 q_i 是 x ∈ A 的集合，使得 v_i(x) ≥ n_i；这表明 q_i 是除数 (no. 4, 命题 5)，因此也是 a。

### 7. 应用：离散估值新刻画环

#### 命题 11 {#ac-vii-s1-prop-11 .statement tag=04ZE}

令 $\mathbf{A}$ 为局部 Krull 域（特别是整体闭局部诺特域），$m$ 为其最大理想。以下条件是等效的：
(a) $\mathbf{A}$是离散估值环；
(b) $m$是可逆的；
(c) $\mathbf{A}:m \neq \mathbf{A}$；
(d) $m$ 是除数；
(e) $m$ 是 $\mathbf{A}$ 唯一的非零素理想。

由于离散估值的每个非零理想环都是本金（章VI, § 3, no. 6，命题9），因此它是可逆的，因此（a）意味着（b）。如果 $m$ 可逆，则其逆为 $\mathbf{A}:m$ (章 II, § 5, no. 6, 命题 10)，因此为 $\mathbf{A}:m \neq \mathbf{A}$；因此(b)意味着(c)。如果$\mathbf{A}:m \neq \mathbf{A}$，则$\mathbf{A}:(\mathbf{A}:m) \neq \mathbf{A}$；现在$m \subset \mathbf{A}:(\mathbf{A}:m)$；因此 $m = \mathbf{A}:(\mathbf{A}:m)$ 因为 $m$ 是最大的，因此 $m$ 是除数 (no. 1, 命题 1 (c))；因此(c)意味着(d)。 (d) 蕴含 (e) 的事实来自于 no. 6 的定理 3，最后，如果 $m$ 是 $\mathbf{A}$ 唯一的非零素理想，它的高度为 1，因此 $\mathbf{A}_m$ 是离散估值环 (no. 6, 定理 4)；由于$\mathbf{A}$是局部的，$\mathbf{A}_m = \mathbf{A}$，这表明(e)蕴涵(a)。

### 8. KRULL 域在其域分数的有限扩张中的积分闭包

#### 命题 12 {#ac-vii-s1-prop-12 .statement tag=04ZF}

令$\mathbf{A}$是一个Krull域，$K$是分数的域，$K'$是$K$的有限扩张，$\mathbf{A}'$是$\mathbf{A}$在$K'$的积分闭包。那么$\mathbf{A}'$是一个Krull域。 $\mathbf{A}'$的基本估值是$K'$的规范离散估值，相当于$\mathbf{A}$基本估值的扩张。

令$(v_i)_{i \in I}$为$\mathbf{A}$基本估值的扩张到$K'$的家族。由于次数$n = [K':K]$是有限的，$v_i$是$K'$的离散估值（章VI, § 8, no. 1，推论3到命题1）。设$B_i$为$v_i$的环；然后$\mathbf{A}' \subset \bigcap_{L \in I} B_i$（章VI, § 1, no. 3，定理3）。相反，$\bigcap_{i \in I} B_i$的每个元素$x$都是$\mathbf{A}$的每个基本估值环的积分（章VI, § 1, no. 3，推论3到定理3）；因此，$x$在$K$属于到$\mathbf{A}$的最小多项式的系数（章V, § 1, no. 3，命题11的推论），因此$x \in \mathbf{A}'$；因此$\mathbf{A}' = \bigcap_{i \in I} B_i$。现在让$x$是$\mathbf{A}'$的非零元素；它满足方程形式 $x^s + a_{s-1}x^{s-1} + \ldots + a_0 = 0$

其中 $a_i \in \mathbf{A}$ 和 $a_s \neq 0$；如果$v_i(x) > 0$，则$v_i(a_0) > 0$；现在$\mathbf{A}$的基本估值$v$使得$v(a_0) > 0$在数中有限，并且对$K$的给定估值延伸的$K'$的估值也在数中有限（章VI, § 8, no. 3，定理1）；因此 $v_i(x) = 0$ 除了有限的数指标 $i \in I$。由此证明$\mathbf{A}'$是克鲁尔域（no. 3，定义3）。

仍有待证明$v_i$相当于$A'$的基本估值（no. 4，推论2至命题6），即（no. 6，推论2至定理3），$x \in A'$的素理想$p_i$，由……组成使得$v_i(x) > 0$，高度为 1。 如果不是这样，则将存在 $A'$ 的素理想 $q$，使得 $(0) \subset q \subset p_i$ 不同于 $(0)$ 和 $p_i$；那么$(0) \subset q \cap A \subset p_i \cap A$和$q \cap A$将不同于$(0)$和$p_i \cap A$（章V, §2, no. 1，推论1到命题1）；因此，首要理想 $p_i \cap A$ 不会是高度 1，而与……矛盾事实上，它对应的基本估值为 $A$。

#### 推论{#ac-vii-s1-n8-cor-1 .statement tag=04ZG}

*令$p$（或$p'$）为高度1的$A$（或$A'$）的素理想，并且$v$（或$u'$）是$A$（或$A'$）相应的的基本估值。为了使$p'$位于$p$之上，$v'$至$K$中的限制等于$v$是必要且充分的。*

估值$v'$相当于$A$（命题12）的基本估值$w$的扩张。设$q = p' \cap A$，它是高度为1的$A$的素理想。为了使$v'$到$K$的限制等于$v$，$w = v$以及$q = p$是充分必要的。

### 9. 多项式环克鲁尔领地

#### 命题 13 {#ac-vii-s1-prop-13 .statement tag=04ZH}

*令 $A$ 为 Krull 域，$X_1, X_n, \ldots, X_n$ 不确定。 环 $A[X_1, \ldots, X_n]$ 是 Krull 域。*

通过归纳对$n$的论证，足以证明，如果$X$是不定的，则$A[X]$是克鲁尔域。设$K$为$A$的分数中的域。 $A[X]$分数域为$K(X)$。令 $I$ 为 $K[X]$ 中的一元多项式的集合，这些多项式在 $K$ 上不可约；对于所有$f \in I$，令$v_f$为由$f$定义的$K(X)$的估值（章VI, §3, no. 3，例4）。另一方面，对于$A$的每个基本估值$w$，令$w$为$w$到$K(X)$的扩张，定义为

$$
\bar{w}\left( \sum_j a_j X^j \right) = \inf_j (w(a_j))
$$

$\sum_j a_j X^j \in K[X]$（章VI, §10, no. 1，引理1）。显然，$u$和$\bar{w}$是离散且规范的，对于所有$u \in K[X]$、$v_f(u) = 0$（分别为$\bar{w}(u) = 0$），除了有限的数估值$v_f$（分别为$\bar{w}$）。

因此，为了显示命题，只需显示$A[X]$是估值$v_f$和$\bar{w}$的环中的交即可。现在估价$v_f$中的环中的交是$K[X]$。另一方面，对于$\sum_j a_j X^j \in K[X]$，关系$\bar{w}\left( \sum_j a_j X^j \right) \geq 0$相当于“对于所有$j$都是$w(a_j) \geq 0$”；因此，关系“每个评估$\bar{w}'$的$\bar{w}\left( \sum_j a_j X^j \right) \geq 0$”相当于“所有$j$的$w(a_j) \geq 0$以及$A$的每个基本评估$w$”。这证明了我们的断言。

#### 注 {#ac-vii-s1-n9-rem-1 .statement tag=04ZI}

命题13中证明引入的估值$v_f$和$\bar{w}$是$A[X]$的基本估值。我们只要证明，如果$V$是估值$v_f$（$f$不可约）和$\bar{w}$（w本质）的集合，那么，对于所有$v' \in V$，存在元素$g \in K(X)$，它不在$A[X]$中，并且使得$v''(g) \geq 0$ 对于所有不同于 $v'$ 的评估$v'' \in V$；这将证明$V - \{v'\}$不满足（AK$_{II}$），因此结论将由no. 4得出，推论2到命题6。首先假设$v'$是形式$\bar{w}$：那么我们可以将$g$是元素 $b \in K$，使得$w(b) < 0, w'(b) \geq 0$对于$A$的基本评估$w'$不同于$w$，那么$v_f(b) = 0$对于$K[X]$中的每个不可约单调多项式$f$； 元素 $b$ 满足的存在性 上述条件由no. 5、命题 9得出。 其次假设$v'$对于不可约一元多项式$f \in K[X]$来说是形式$v_f$ 次数$m$；那么我们可以在$a \in A$处取$g = a/f$。对于$v_h(g) \geq 0$，对于$K[X]$中的每个不可约一元多项式$h \neq f$；对于选择$a \in A$，对于$A$的每个基本估值$w$，$w(a)$至少等于元素$w(c_i)$的下确界，其中$c_i$是$f$的系数($1 \leq i \leq m$);现在这样一个$a \in A$的存在是从(AK$_{III}$)和no. 5、命题9得出的。

我们也可以说（no. 6，定理 4），高度为1的$A[X]$的素理想是：
(1) 形式 $pA[X]$的素理想，其中$p$是高度为1的$A$的素理想；
(2) 形式$m \cap A[X]$的素理想，其中$m$是$K[X]$的（必然是主）素理想。

后者的特点是它们的交和$A$减少到0。

### 10.克鲁尔领地的除子类

令 $A$ 为克鲁尔域。回想一下，$A$的除子的群$D(A)$是其极值元素的集合$P(A)$生成的自由交换群（no. 3，定理2）并且$P(A)$与高度为1（no. 6）的$A$素理想的集合等同；对于$p \in P(A)$，我们将用$v_p$表示规范的基本估值相应的至$p$（no. 4）；回想一下，$v_p$的环是$A_p$（no. 4，推论1到命题6）。我们将用本金除子的$D(A)$由……组成的$F(A)$子群和$A$（no. 2）的$C(A) = D(A)/F(A)$除子类群表示。

#### 命题 14 {#ac-vii-s1-prop-14 .statement tag=04ZJ}

令 $A$ 为 Krull 域，$B$ 为 Krull 域包含 $A$。假设以下条件成立：

(PDE) 对于高度为 1 的每个素理想 $\mathfrak{P}$ 或 $B$，素理想 $\mathfrak{P} \cap A$ 为零或高度为 1。

对于$p \in P(A)$，$\mathfrak{P} \in P(B)$使得$\mathfrak{P} \cap A = p$在数中是有限的；我们写

$$
i(p) = \sum_{\mathfrak{P} \in P(B), \mathfrak{P} \cap A = p} e(\mathfrak{P}/p)\mathfrak{P},
$$

其中 $e(\mathfrak{P}/\mathfrak{p})$ 表示 $v_{\mathfrak{p}}$ 在 $v_{\mathfrak{p}}$ 上的*分支* 指标 (章 VI, § 8, no. 1)。 *则i定义，通过*线性度，$D(A)$至$D(B)$的递增*同态*$i$，其具有以下性质：

(a) *对于 A* 的分数域的每个非零元素 x，

$$
i(\operatorname{div}_A(x)) = \operatorname{div}_B(x);
$$

(b) *对于 D(A)* 中的所有 D、D'，

$$
i(\sup(D, D')) = \sup(i(D), i(D'));
$$

让$\mathfrak{p} \in P(A)$；考虑 $\mathfrak{p}$ 的非零元素 $a$； $\mathfrak{P} \in P(B)$，其中包含 $a$ 在数中是有限的（no. 6，定理 4）； *更不必说* $\mathfrak{P} \in P(B)$，使得 $\mathfrak{P} \cap A = \mathfrak{p}$ 在数中是有限的。

我们现在展示（a）。根据可加性，可以假设$x \in A^* = A - \{0\}$。

定义、$\operatorname{div}_B(x) = \sum_{\mathfrak{P} \in P(B)} v_{\mathfrak{p}}(x) \cdot \mathfrak{P}$。对于所有$\mathfrak{P} \in P(B)$，使得$v_{\mathfrak{p}}(x) > 0$、$\mathfrak{P} \cap A$非零（对于$x \in \mathfrak{P}$），因此通过 (PDE) 其高度为 1； 设定$\mathfrak{p} = \mathfrak{P} \cap A$，由指标、$v_{\mathfrak{p}}(x) = e(\mathfrak{P}/\mathfrak{p}) v_{\mathfrak{p}}(x)$的分支定义计算（因为$v_{\mathfrak{p}}$和$v_{\mathfrak{P}}$已标准化）。作为$\operatorname{div}_A(x) = \sum_{\mathfrak{p} \in P(A)} v_{\mathfrak{p}}(x) \cdot \mathfrak{p}$和$i(q) = 0$对于所有$q \in P(A)$（不是形式$\mathfrak{Q} \cap A$，其中$\mathfrak{Q} \in P(B)$），我们推导出(a)。

为了证明 (b) 我们写

$$
D = \sum_{\mathfrak{p} \in P(A)} n(\mathfrak{p}) \cdot \mathfrak{p} \quad \text{and} \quad D' = \sum_{\mathfrak{p} \in P(A)} n'(\mathfrak{p}) \cdot \mathfrak{p};
$$

$\sup(D, D')$中$\mathfrak{p}$的系数为$\sup(n(\mathfrak{p}), n'(\mathfrak{p}))$。设$\mathfrak{P}$为$P(B)$的元素。如果$\mathfrak{P} \cap A = (0)$，则$i(D)$和$i(D')$以及$\sup(i(D), i(D'))$中$\mathfrak{P}$的系数为零；因此$i(\sup(D, D'))$中$\mathfrak{P}$的系数为零。如果$\mathfrak{P} \cap A \neq (0)$，则它是高度为1的素理想$\mathfrak{p}$（通过（PDE））；写成$e = e(\mathfrak{P}/\mathfrak{p})$，$i(D)$、$i(D')$、$i(\sup(D, D'))$中$\mathfrak{P}$的系数分别为$en(\mathfrak{p}), en'(\mathfrak{p})$、$e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p}))$； $\sup(i(D), i(D'))$ 是

$$
\sup(e \cdot n(\mathfrak{p}), e \cdot n'(\mathfrak{p})) = e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p})).
$$

这就证明了(b)。

在命题 14 的假设下，从 (a) 可以得出，i 定义，通过取同态 $\bar{i}$（称为规范的 $C(A)$ 到 $C(B)$）的商，我们也将有时写为 $i$，通过滥用记号。

条件 (PDE) 在以下两种情况下满足：

(1) B 对 A 是积分；在这种情况下，*对于 B 的素理想 $\mathfrak{P}$ 的高度为 1，*$\mathfrak{p} = \mathfrak{P} \cap A$ 的高度为 1 是充分必要的。因为 (0) 是 B 的唯一素理想，位于 A 的理想 (0) 之上（章 V, § 2, no. 1，推论 I 到命题 1）；如果$\mathfrak{P}$的高度为1，则$\mathfrak{p} \neq 0$；如果 $\mathfrak{p}$ 的高度不是 1，则将存在 A 的素理想 $\mathfrak{p}'$ 与 (0) 和 $\mathfrak{p}$ 不同，并且 0 ⊂ p' ⊂ p；但是，由于 B 是整环并且 A 是一个积分闭域，因此 B 会有一个素理想 $\mathfrak{p}'$，使得 $\mathfrak{p}' \cap A = p'$ 和 $\mathfrak{p}' \subset \mathfrak{p}$ (章 V, § 2, no. 4，定理 3)，与假设相反。相反，如果 p 的高度为 1，则不存在不同于 0 和 $\mathfrak{p}$ 的 B 素理想$\mathfrak{p}'$，并且使得 $0 \subset \mathfrak{p}' \subset \mathfrak{p}$，否则 $0 \subset \mathfrak{p}' \cap A \subset p$ 和 $\mathfrak{p}' \cap A$ 将凭借章 V, § 2, no. 1 不同于 0 和 p，推论 1 命题1。

(2) B 是降平A-模。更准确地说：

#### 命题 15 {#ac-vii-s1-prop-15 .statement tag=04ZK}

令 A 和 B 为克鲁尔域，使得 B 包含 A 并且是平展A-模。然后：
(a) 满足命题 14 的条件 (PDE)；
(b) 对于每个除数理想 $a \in A$，Ba 是 B 的除数理想，其中对应到除子 $i(\operatorname{div}_A(a))$。

为了显示(a)，假设存在高度为1的B的素理想$\mathfrak{p}$，使得$\mathfrak{p} \cap A$既不为0也不为高度1。在$\mathfrak{p} \cap A$中取元素$x \neq 0$。高度为 1 的 A 的理想 $p_i$，其中包含 x 在数内有限，并且没有包含 $\mathfrak{p} \cap A$；因此，存在$\mathfrak{p} \cap A$的元素 y，使得$y \notin p_i$对于所有$i$（章II, § 2, no. 1，命题2）。因此$\operatorname{div}_A(x)$和$\operatorname{div}_A(y)$是有序群 P(A)的互质元素，因此$\sup(\operatorname{div}_A(x), \operatorname{div}_A(y)) = \operatorname{div}_A(x) + \operatorname{div}_A(y) = \operatorname{div}_A(xy)$；由于理想 $Ax \cap Ay$ 和 $Axy$ 是相除的，我们推断出 $Ax \cap Ay = Axy$。由于 B 是平的 A-模，$Bx \cap By = Bxy$ (章 I, § 2, no. 6，命题 6)。这意味着$\sup(v_{\mathfrak{p}}(x), v_{\mathfrak{p}}(y)) = v_{\mathfrak{p}}(xy) = v_{\mathfrak{p}}(x) + v_{\mathfrak{p}}(y)$，其中与……矛盾不等式$v_{\mathfrak{p}}(x) > 0, v_{\mathfrak{p}}(y) > 0$（由于x和y在$\mathfrak{p}$中所以成立）。因此(a)已经通过反证法得到了证明。

我们现在展示(b)。如果$a$是A的除数理想，它是两个分数主理想的交（no. 5，推论2到命题9），比如说

$$
a = d^{-1}(Aa \cap Ab)
$$

其中$a, b,$敢于$A^*$；因为 B 平于 A，$Ba = d^{-1}(Ba \cap Bb)$ (章 I, § 2, no. 6, 命题 6)，这表明 Ba 是除数。这也表明$\operatorname{div}_B(Ba) = \sup(\operatorname{div}_B(a), \operatorname{div}_B(b)) - \operatorname{div}_B(d)$；使用命题 14 (a) 和 (b) 可以看出

$$
\begin{align*}
\operatorname{div}_B(Ba) &= \sup(i(\operatorname{div}_A(a)), i(\operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\sup(\operatorname{div}_A(a), \operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(Aa \cap Ab)) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(d^{-1}(Aa \cap Ab))) = i(\operatorname{div}_A(a)).
\end{align*}
$$

#### 推出 {#ac-vii-s1-n10-cor-1 .statement tag=04ZL}

令 A 为本地 Krull 域，B 为离散估值环，使得 B 支配 A 并且平坦A-模。那么A就是域或者离散估值环。

令 $\mathfrak{m}$ 为 B 的最大理想。通过（偏微分方程），$\mathfrak{m} \cap A$ 为零或高度为 1。事实上，通过假设为 A 的最大理想，我们的断言由 no. 7 的命题 11 得出。

#### 注 {#ac-vii-s1-n10-rem-1 .statement tag=04ZM}

在上述两种情况的前一种中，映射$i : D(A) \to D(B)$是单射的：因为$D(B)$的$P(B)$形式基的元素和$P(A)$不能的两个不同理想是相同理想的A上的迹$P(B)$，相当于验证$i(p) \neq 0$对于所有$p \in P(A)$；现在，这是从章V, § 2, no. 1，定理1得出的。同样可以看出，如果B是忠实平坦的A-模，则$i$是单射的（章II, § 2, no. 5，推论4到命题11）。

接下来，我们建议针对克鲁尔域 A、B 的某些有序对，研究从$C(A)$到$C(B)$的典范同态$\tilde{i}$。

#### 命题 16 {#ac-vii-s1-prop-16 .statement tag=04ZN}

令 A 为 Zariski 环，使得其补全 $\hat{A}$ 为 Krull 域。那么A是一个Krull域，从$C(A)$到$C(\hat{A})$的典范同态$\tilde{i}$（这是因为A是平的A-模;cf.章III, § 3, no. 4，定理3）是单射的。

由于A是整环和$A \subset \hat{A}$，所以A是整环。令 L 为 $\hat{A}$ 的分数的域，K $\subset$ L 为 A 的 $A = \hat{A} \cap K$ (章 III, § 3, no. 5，推出 4 至命题 9)，A 是 Krull 域 (no. 3， 例4)。 $\tilde{i} : C(A) \to C(\hat{A})$ 是单射的事实是从命题 15 (b) 得出的，并且如果 $b \hat{A}$ 是本金，则 b 是本金（章 III, § 3, no. 5，推出 3 到命题 9）。

现在让 A 为克鲁尔域，S 为 A 的乘法子集，而不是包含 0。群 $D(A)$（分别为 $D(S^{-1}A)$）是群与 $\operatorname{div}(p)$（分别为集合）的自由交换律群和基集合。 $\operatorname{div}(S^{-1}p)$)，其中 p 穿过高度为 1 的 A 的素理想的集合（分别为高度为 1 的 A 的素理想的集合，使得 $p \cap S = \varnothing$）（no. 4，命题 6），并且，如果$p \cap S = \varnothing$，则$i(\operatorname{div}(p)) = \operatorname{div}(S^{-1}p)$。因此 $D(S^{-1}A)$ 与由元素 $\operatorname{div}(p)$ 生成的$D(A)$ 的直接因子等同，使得 $p \cap S = \varnothing$ 并承认 $D(A)$ 的自由交换子群与 $\operatorname{div}(p)$ 的基集合互补，使得$p \cap S \neq \varnothing$；我们用 G 来表示这个补集。由于 $i : D(A) \to D(S^{-1}A)$ 是满射，$i : C(A) \to C(S^{-1}A)$ 也是满射；以及：

$$
G/(G \cap F(A)) = (G + F(A))/F(A) = \operatorname{Ker}(\tilde{i});
$$

因为如果$D(S^{-1}A)$的元素等于$\operatorname{div}_{S^{-1}A}(x/s)$，其中$x \in A$和$s \in S$，则它是本金除子$\operatorname{div}_A(x)$（命题14）的$i$下的像。

现在假设 S 由 A 的元素$(p_i)_{i \in I}$族生成，使得主理想$Ap_i$都是素数。然后，如果$p$是高度为1的A的素理想，使得$p_i$的幂的$p \cap S \neq \varnothing$、$p$包含乘积，因此$p_i$之一，即$p_\alpha$；由于 $Ap_\alpha$ 是非零且素数，且 $p$ 的高度为 1，因此得出 $p = Ap_\alpha$。在上面的记号中，因此$G \subset F(A)$和(5)表明$\bar{i}$的核是零。因此，我们显示了以下结果：

#### 命题 17 {#ac-vii-s1-prop-17 .statement tag=04ZO}

*令$A$为克鲁尔域，$S$为$A$的乘法子集，而不是包含$0$。那么从$C(A)$到$C(S^{-1}A)$的典范同态$\bar{i}$是满射。如果进一步 $S$ 由一系列元素 $p_i$ 生成，使得主理想 $Ap_i$ 都是素数，则 $\bar{i}$ 是双射的。*

作为公式(5)的第二个应用，考虑以下情况：令$R$为Krull域；取$A$为$A$的非零常数多项式的多项式环$A = R[X]$（no. 9，命题13），$S$为集合$R - (0)$。高度 1 的 $A$ 的素理想 $p$ 使得 $p \cap S \neq \varnothing$ 是形式 $p_0A$ 的素理想，其中 $p_0$ 是高度 1 的 $R$ 的素理想 (no. 9, *注*)。因此，在上面介绍的记号中，通过将$\mathrm{div}_A(p_0A)$与$\mathrm{div}_R(p_0)$识别，将$G$与$D(R)$进行识别。另一方面，$G \cap F(A)$与$F(R)$相同：因为如果$R$生成的理想$a$是$A = R[X]$中的主理想$a_0A = f(X)A$，则$f(0) \in a_0A$，因为$a_0A$是环的分级理想$A$（按通常的多项式次数分级），因此$f(0) \in a$；进一步，对于$a \in a_0A$、$a = f(X)g(X)$，其中$g(X) \in R$、从而，比较项与次数0、$a = f(0)g(0)$；由此可见，$a$是由$f(0)$生成的$R$的主理想。最后，用$R$的分数的$K$域表示，$S^{-1}A$与多项式环$K[X]$等价，即主理想整环；因此$C(S^{-1}A) = (0)$。因此，根据(5)，$C(A) = \mathrm{Ker}(\bar{i})$与$C(R)$一致，我们证明了以下结果：

#### 命题 18 {#ac-vii-s1-prop-18 .statement tag=04ZP}

*令 $R$ 为 Krull 域，$A$ 多项式环 $R[X]$。 $C(R)$ 到 $C(R[X])$ 的典范同态是双射的。*

### 习题 {#ac-vii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
