---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 1
section_title: Notion of an integral element
lang: zh
source: ac-i-vii
book_pages: 303-324, 355-362
pdf_pages: 0322-0343, 0374-0381
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL ELEMENTS OVER A RING
      page: 303
      pdf_page: 322
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A RING. INTEGRALLY CLOSED DOMAINS
      page: 308
      pdf_page: 327
    - "no": 3
      title: EXAMPLES OF INTEGRALLY CLOSED DOMAINS
      page: 309
      pdf_page: 328
    - "no": 4
      title: COMPLETELY INTEGRALLY CLOSED DOMAINS
      page: 312
      pdf_page: 331
    - "no": 5
      title: THE INTEGRAL CLOSURE OF A RING OF FRACTIONS
      page: 314
      pdf_page: 333
    - "no": 6
      title: NORMS AND TRACES OF INTEGERS
      page: 316
      pdf_page: 335
    - "no": 7
      title: EXTENSION OF SCALARS IN AN INTEGRALLY CLOSED ALGEBRA
      page: 318
      pdf_page: 337
    - "no": 8
      title: INTEGERS OVER A GRADED RING
      page: 320
      pdf_page: 339
    - "no": 9
      title: 'APPLICATION: INVARIANTS OF A GROUP OF AUTOMORPHISMS OF AN ALGEBRA'
      page: 323
      pdf_page: 342
statements: 69
exercises: 29
content_sha256: 0c1b6076b0486626b753c306a2a863e915dcf9b8697345801a335c923b5d7831
translated_from: content/en/ac/V/01_s1_notion_of_an_integral_element.md
translation_method: google
source_content_sha256: 7deb20eda4181c66deed788db2dd8c9dfd03ddc75e31d67d9679866d4b1220a1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 96e443a8a4ad6c6def24d5c7cb84cb370d56adbe3fdb1709ae0fdf20415ecdef
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 积分元素的概念

### 1.积分元素超过环

#### 定理 1 {#ac-v-s1-thm-1 .statement tag=04MS}

设$\mathbf{A}$是环（可交换），$\mathbf{R}$代数超过$\mathbf{A}$（不一定可交换）和$\mathbf{R}$的$x$元素。以下属性是等效的：

(E₁) $x$ 是多项式环 $\mathbf{A}[X]$ 中的一元多项式的根。
(E2) $\mathbf{R}$ 的子代数 $\mathbf{A}[x]$ 是有限生成的$\mathbf{A}$ 模。
(E₃) 在环$\mathbf{A}[x]$上存在忠实的模，它是有限生成的$\mathbf{A}$模块。

让我们首先证明 (E₁) 蕴涵 (E2)。让
$$
X^n + a_1 X^{n-1} + \ldots + a_n
$$
是$\mathbf{A}[X]$中的一元多项式，其中$x$为根；对于每个整数$q \geq 0$，让$M_q$是由$1, x, \ldots, x^n + q$生成的$\mathbf{R}$的子$\mathbf{A}$模块。然后
$$
x^{n+q} = -a_{n+q-1} x^{n+q-1} - \ldots - a_n x^q \in M_{-1}
$$
对于所有$q \geq 1$、从而、归纳、$q$，
$$
M_q = M_{q-1} = \cdots = M_0.
$$

(*) 这章和下一本章的结果除了I到VI之外，不依赖于任何书，也不依赖于章I, § 4，也不依赖于章111，§ 5。

我们结论认为$A[x]$等于$M_0$，因此是有限生成的$A$模块。

由于交换环 $A[x]$ 是对自身的忠实模，因此 ($E_{II}$) 意味着 ($E_{III}$)。

最后，($E_{III}$) 蕴含 ($E_1$) 的事实可以从以下更精确的引理得出：

#### 引理 1 {#ac-v-s1-lem-1 .statement tag=04MT}

*设$A$为环，$R$代数（不一定可交换）超过$A$和$x$元素或$R$。 Let $M$ be a faithful module over $A[x]$ which is a finitely generated $A$-module. 如果$q$是$A$的理想，使得$xM \subset qM$，则$x$是一元多项式的根，其中$A$中的系数全部为$\notin$，其系数除了主系数属于到$q$之外。*

令$(u_i)_{1 \leq i \leq n}$是$M$的元素的有限族，使得$M = \sum_{i=1}^n Au_i$。对于所有$i$，假设存在$q$的元素的有限族$(q_{ij})_{1 \leq j \leq n}$，使得

$$
xu_i = \sum_{j=1}^n q_{ij}u_j \quad \text{for} \quad 1 \leq i \leq n.
$$

因此 (*代数*, 章 III, § 8) 如果 $d$ 是矩阵 $(q_{ij} - \delta_{ij}x)$ 的行列式，其中元素在 $A[x]$ 中（$\delta_{ij}$ 表示克罗内克指标），则$du_i = 0$ 对于所有$i$，因此$dM = 0$；因为$M$被假定为忠实的$A[x]$模块，必然是$d = 0$。这意味着 $x$ 是 $A[X]$ 中的多项式 $\det(q_{ij} - \delta_{ij}X)$ 的根，该多项式在符号范围内是一个一元多项式，其系数除了主系数属于到 $q$ 之外。

#### 定义 1 {#ac-v-s1-def-1 .statement tag=04MU}

*设$A$为环且$R$为$A$代数（不一定可交换）。如果元素$x \in R$满足定理1的等价性质($E_1$)、($E_{II}$)、($E_{III}$)，则称为$A$上的积分。*

形式 $P(x) = 0$ 的关系，其中 $P$ 是 $A[X]$ 中的*单调*首一多项式，也称为系数在 $A$ 中的*积分相关方程*。

*例*

#### 例 1 {#ac-v-s1-n1-exa-1 .statement tag=04MV}

设 $K$ 为（可交换的）域，$R$ 为 $K$ 代数；说元素 $x \in R$ 是 $K$ 的积分，相当于说，$x$ 是环 $K[X]$ 中*非常数*多项式的根；当$R$是$K$的*扩张*时引入的泛化术语（*代数*，章V, § 3, no. 3），元素$x \in R$在$K$上积分也称为*代数* $R$ 中的元素超过 $K$。

*(2)* 元素 *of* $\mathbf{Q}(i)$ 在 $\mathbf{Z}$ 上积分，是形式 $a + ib$ 的元素，其中 $a \in \mathbf{Z}$ 和 $b \in \mathbf{Z}$ ("*高斯整数*"')； $\mathbf{Q}(\sqrt{5})$的元素在$\mathbf{Z}$上积分是元素*形式$(a + b\sqrt{5})/2$，其中$a$和$b$属于到$\mathbf{Z}$并且都是偶数或都是奇数（对于这两个例参见习题1)。

(3) $\mathbf{Z}$ 上的复数积分也称为代数整数。

注
(1) 令$A'$为$R$的子环（包含在$R$的中心）环同态$A \to R$下的$A$像，其中定义 $A$-代数结构关于$R$。显然，这相当于说$R$的元素在$A$上积分或者在$A'$上积分。

#### 例 2 {#ac-v-s1-n1-exa-2 .statement tag=04MW}

令$R'$为$R$的子A代数； $R'$的元素在$A$上积分，只是$R$的元素在$A$和属于到$R'$上积分；这通常允许我们在不引起混淆的情况下，不必指定代数是 $A$ 属于上的积分元素。

#### 命题 1 {#ac-v-s1-prop-1 .statement tag=04MX}

*设$A$为环，$R$代数超过$A$（不一定可交换），$x$元素为$R$。 For $x$ to be integral over $A$, it is necessary and sufficient that $A[x]$ be contained in a subalgebra $R'$ of $R$ which is a finitely generated $A$-module.*

由于性质(E_{II})，条件显然是必要的；凭借(E_{III})，它也是足够的，因为$R'$是一个忠实的$A[x]$模块（因为它是$R$的包含单位元）。

#### 推论{#ac-v-s1-n1-cor-1 .statement tag=04MY}

*令 $A$ 为诺特环，$R$ $A$ 代数（不一定可交换）以及 $R$ 的 $x$ 元素。为了使 $x$ 对 $A$ 整的，存在一个由 $R$ 包含于 $A[x]$ 有限生成的子模是充分必要的。*

由于 (E_{II})，条件是必要的；如果$A[x]$是有限生成A-模的子A模块，它本身就是有限生成A-模（*代数*，章VIII, § 2, no. 3，命题7）就足够了。

假设 $A$ 是诺特不能从叙述 (习题 2) 中省略。

#### 定义 2 {#ac-v-s1-def-2 .statement tag=04MZ}

*设$A$为环。如果 $R$ 的每个元素都在 $A$ 上积分，则 $A$ 代数 $R$（不一定可交换）被称为在 $A$ 上积分。如果 $R$ 是有限生成的 $A$ 模，$R$ 被称为在 $A$ 上有限。*

从命题 1 可以得出，每个有限 $A$-代数都是积分的；如果$R$是可交换的并且是有限的$A$-代数，则$R$显然是有限生成的$A$-代数； 逆命题是假的。

*例 (4)* 如果$M$是有限生成的$A$模，$M$的自同态的代数$\mathrm{End}_A(M)$凭借(E_{III})在$A$上积分；特别是，对于每个整数 $n$，矩阵代数 $M_n(A) = \mathrm{End}_A(A^n)$ 是 $A$ 上的整数（甚至是有限的）。

#### 命题 2 {#ac-v-s1-prop-2 .statement tag=04N0}

*令$A, A'$为两个环、$R$一个$A$代数、$R$一个$A'$代数（不一定可交换）以及$f : A \to A'$和$g : R \to R'$两个环同态，使得图表

$$
\begin{array}{ccc}
A & \xrightarrow{f} & A' \\
| & & | \\
\mathbf{R} & \xrightarrow{g} & \mathbf{R}'
\end{array}
$$

是可交换的。如果元素 $x \in R$ 对 $A$ 整的，则 $g(x)$ 对 $A'$ 整的。

如果 $x^n + a_1 x^{n-1} + \cdots + a_n = 0$ 其中 $a_i \in A$ 为 $1 \leq i \leq n$，我们推断

$$
(g(x))^n + f(a_1)(g(x))^{n-1} + \cdots + f(a_n) = 0.
$$

#### 推出 1 {#ac-v-s1-prop-2-cor-1 .statement tag=04N1}

*令$A$为环，$B$（可交换）$A$-代数和$C$（不一定可交换）$B$-代数。那么每个在 $A$ 上积分的元素 $x \in C$ 也在 $B$ 上积分。*

#### 推出 2 {#ac-v-s1-prop-2-cor-2 .statement tag=04N2}

*令$K$为$K$中的域、$L$扩张和$x, x'$$L$中的两个元素，其中共轭超过$K$（代数， 章V, § 6, no. 2）。如果$A$是$K$的子环并且$x$是$A$的积分，$x'$也是$A$的积分。*

$K(x)$存在$K$同构$f$到$K(x')$，使得$A$的$f(x) = x'$和元素在$f$下不变。

#### 推出 3 {#ac-v-s1-prop-2-cor-3 .statement tag=04N3}

*设$A$为环，$B$（可交换）$A$-代数和$C$（不一定可交换）$B$-代数。如果 $C$ 对 $A$ 整的，则 $C$ 对 $B$ 整的。*

#### 命题 3 {#ac-v-s1-prop-3 .statement tag=04N4}

*设 $(R_i)_{1 \leq i \leq n}$ 为（不一定可交换的）$A$-代数的有限族，并设 $R = \prod_{i=1}^n R_i$ 为它们的乘积。为了使$R$的元素$x = (x_i)_{1 \leq i \leq n}$在$A$上积分，$x_i$中的每一个在$A$上积分是充分必要的。为了使$R$在$A$上积分，每个$R_i$在$A$上积分是必要且充分的。*

显然证明第一个断言就足够了。 命题 2 需要条件。 相反，如果每个$x_i$都是$A$的积分，则$R_i$的子代数$A[x_i]$是有限生成的$A$模，因此$R$的子代数$\prod_{i=1}^n A[x_i]$也是如此；由于$A[x]$包含在子代数中，$x$是$A$除命题 1的积分。

#### 命题 4 {#ac-v-s1-prop-4 .statement tag=04N5}

*令$A$为环，$R$为$A$代数（不一定可交换），$(x_i)_{1 \leq i \leq n}$为$R$的元素的有限族，它们是成对可置换的。如果对于所有 $i$，$x_i$ 是 $A[x_1, \ldots, x_{i-1}]$ 的积分（特别是如果所有 $x_i$ 是 $A$ 的积分），则 $R$ 的子代数 $A[x_1, \ldots, x_n]$ 是有限生成的 $A$ 模。*

我们通过归纳对$n$进行论证，命题只是(E_{II})对于$n = 1$。 归纳假设意味着$B = A[x_1, \ldots, x_{n-1}]$是有限生成A-模；由于$x_n$是$B$的积分，$B[x_n] = A[x_1, \ldots, x_n]$是有限生成的B-模，因此也是有限生成A-模（代数、章II, § 1, no. 13、命题25）。

#### 推论 1 {#ac-v-s1-prop-4-cor-1 .statement tag=04N6}

令 $A$ 为环且 $R$ a（可交换）A-代数。 The set of elements $\& R$ integral over $A$ is a subalgebra of $R$.

事实上，如果$x, y$是$R$对$A$积分的两个元素，则从命题4可以得出$A[x, y]$是有限生成A-模；因为包含$x + y$和$xy$，推论来自命题1。

在非交换代数中，两个元素在$A$上的积分和和乘积不一定是$A$（习题4）上的积分。

#### 推论 2 {#ac-v-s1-prop-4-cor-2 .statement tag=04N7}

设 $A$ 为环、$R$ A-代数（不一定可交换）和 $E$ 集合 $\&$ 元素 $\& R$，它们在 $A$ 上可成对置换和积分。那么$E$生成的子A代数$B \& R$在$A$上积分。

$B$ 属于的每个元素到由 $E$ 的有限子集生成的 $B$ 子 A 代数。

注 (3) 从命题 4 可以得出，$A$ 上的每个可交换 A-代数积分都是 $A$ 上有限子代数的右有向族的并。

#### 命题 5 {#ac-v-s1-prop-5 .statement tag=04N8}

令 $A$ 为环且 $A$ 和 $R$ 两个（可交换）A-代数。如果$R$是$A$的积分，则$R \otimes_A A'$是$A'$的积分。

考虑$R \otimes_A A'$的任何元素$x' = \sum_{i=1}^n x_i \otimes a'_i$，其中$x_i$属于到$R$以及$a'_i$到$A'$；由于 $x_i \otimes a'_i = (x_i \otimes 1)a'_i$ 和 $x_i \otimes 1$ 是 $A'$ (命题 2) 的积分，$x$ 也是如此。

#### 推论{#ac-v-s1-n1-cor-2 .statement tag=04N9}

令$R$为环且$A, B, C$子环$\& R$，使得$A \subset B$。如果$B$是$A$的积分，则$C[B]$是$C[A]$的积分。

$B \otimes_A C[A]$ 是 $C[A]$ 命题 5 的积分，因此 $R$ 中 $B \otimes_A C[A]$ 的典范像 $C[B]$ 也是如此（被视为A-代数）乘命题 2。

#### 命题 6 {#ac-v-s1-prop-6 .statement tag=04NA}

令 $A$ 为环，$B$ 一个（可交换的）A-代数和 $C$ 一个（不一定可交换的）B 代数。如果 $B$ 在 $A$ 上积分，且 $C$ 在 $B$ 上积分，则 $C$ 在 $A$ 上积分。

只要验证每个 $x \in C$ 都是 $A$ 的整数就足够了。到假设，存在一元多项式$X^n + b_1 X^{n-1} + \cdots + b$，$B$和$x$的系数为根；那么$x$是$B' = A[b_1, \ldots, b_n]$的积分，因此$B'[x]$是有限生成的B-模。但由于$B$是$A$的积分，$B'$是有限生成A-模（命题4）；我们结论 B'[x] 也是有限生成A-模 (代数, 章 11, § 1, no. 13, 命题 25)，因此 x 是 A 的整数。

#### 推论{#ac-v-s1-n1-cor-3 .statement tag=04NB}

*设 A 环且 R、R' 是 A 上的两（可交换）A-代数积分。则 R $\otimes_A$ R' 是 A 上的积分。*

$R \otimes_A R$ 是 R (命题 5) 的积分，因此结论由命题 6 得出。

### 2. 环的整体闭合。整体封闭域

#### 定义 3 {#ac-v-s1-def-3 .statement tag=04NC}

*设 A 为环，R a（可交换）A-代数。 R 在 A 上积分的元素的 R 由……组成的子 A 代数 A'（no. 1，推论 1 到命题 4）称为 A 在 R 中的积分闭包。如果 A' 等于 A 在 R 中的典范像，则称 A 在 R 中积分闭。*

注

(1) 如果$h : A \to R$是环同态，在R上定义A-代数结构，则A在R中的积分闭包也是$h(A)$在R中的积分闭包。另一方面，如果R'是R的子代数，则A在R'中的积分闭包是$A' \cap R'$。

(2) 如果A是域，则A在R中的积分闭包$A'$由R的元素组成，它们是A上的代数(no. 1，例1)；推广术语用于域扩张 (代数, 章 V, § 3, no. 3)，则 A' 也称为代数 R 中域 A 的代数闭包，并且 A 在 R 中被称为代数封闭，如果$A' = A$。

#### 定义 4 {#ac-v-s1-def-4 .statement tag=04ND}

*若A为整环，则A在其分数的域的积分闭包称为A的积分闭包。整环若等于其积分闭包，则称为A的积分闭包。*

注积分闭域不一定在任何环包含中也是闭域，如域的例所示，它不是代数闭域。

#### 命题 7 {#ac-v-s1-prop-7 .statement tag=04NE}

*设A为环，R为A-代数。 A 在 R 中的积分闭包 A' 是子环在 R 中积分闭。*

R 中 A' 的积分闭包在 A 上积分no. 1、命题 6；因此它等于A'。

#### 推论{#ac-v-s1-n2-cor-1 .statement tag=04NF}

*整环 A 的积分闭域是一个积分闭域。*

设K为A的分数的域，B为A的积分闭包。 显然

K是B的分数的域并且应用命题7到$R = K$就足够了。

#### 命题 8 {#ac-v-s1-prop-8 .statement tag=04NG}

*令$R$为环，$(B_\lambda)_{\lambda \in L}$为$R$的子环的族，对于每个$\lambda \in L$，令$A_\lambda$为$B_\lambda$的子环。如果每个$A_\lambda$在$B_\lambda$内积分闭，则$A = \bigcap_{\lambda \in L} A_\lambda$在$B = \bigcap_{\lambda \in L} B_\lambda$内积分闭。*

这紧随定义 3 和no. 1，推论 1 到命题 2。

#### 推论{#ac-v-s1-n2-cor-2 .statement tag=04NH}

*整环$A$的非空全闭子域族中的每个交都是一个全闭域。*

应用命题 8 取$R$且$B_\lambda$等于$A$的分数$K$的域，并注意到$K$的子环在$K$内积分闭，则*更不必说* 是一个积分闭域，因为分数的域包含在$K$ 中。

#### 命题 9 {#ac-v-s1-prop-9 .statement tag=04NI}

*设$A$为环，$(R_i)_{1 \leq i \leq n}$$A$代数的有限族，$A'_i$为$A$在$R_i$，$(1 \leq i \leq n)$的积分闭包。那么$A$在$R = \prod_{i=1}^n R_i$的积分闭包，等于$\prod_{i=1}^n A'_i$。*

这是no. 1、命题 3 中的直接的推论。

#### 推论 1 {#ac-v-s1-prop-9-cor-1 .statement tag=04NJ}

*设$A$是诺特环、$p_i$$(1 \leq i \leq n)$其独特的最小素理想、整环$A/p_i$的分数的$K$、域（规范同构于局部环$A_{p_i}$（章IV, § 2, no. 5，命题10））和$A'_i$$A$在$K$，$(1 \leq i \leq n)$的积分闭包。 Then the canonical isomorphism of the total ring of fractions $B$ of $A$ onto $\prod_{i=1}^n K_i$ (loc. cit.) maps the integral closure of $A$ in $B$ onto the product ring $\prod_{i=1}^n A'_i$.*

#### 推论 2 {#ac-v-s1-prop-9-cor-2 .statement tag=04NK}

*对于要在分数的环内积分闭合的约化诺特环，它是积分闭合 (诺特) 域的直接合成是必要且充分的。*

### 3. 例整体封闭域

#### 命题 10 {#ac-v-s1-prop-10 .statement tag=04NL}

*每个主理想整环都是整体封闭的。*

令$A$为主理想整环，$K$为分数的域，以及$K$的$x$元素。 $A$存在两个互质元素 $a, b$，使得 $x = ab^{-1}$ (*代数*, 章 VII, § 1, no. 2, 命题 1 和章 VI, § 1, no. 11, 命题 9 （DIV））。如果 $x$ 对 $A$ 整的，则它是多项式的根

X^n + c_1 X^{n-1} + \ldots + c_n \text{ } A[X]。然后$a^n = b(-c_1 a^{n-1} - \ldots - c_n b^{n-1})$，证明$b$除$a''$。由于$a$和$b$互质，这意味着$b$在$A$中可逆（代数，章VI, § 1, no. 12，推论1到命题11（DIV））；因此$x \in A$。

#### 引理 2 {#ac-v-s1-lem-2 .statement tag=04NM}

*设 R 为环，P 为 R[X] 中的多项式。存在环 R' 包含 R，使得在多项式环 R'[X] 中，首一多项式 P 是次数 1 的一元多项式的乘积。*

我们在 P 的次数 $n$ 上沿归纳前进，引理对于$n = 0$ 和 $n = 1$ 是显而易见的。因此假设$n > 1$。令$a$为P生成的$R[X]$的理想，令$f$为$R[X]$到$B = R[X]/a$的典范同态。由于 P 是单调的，对于每个多项式 $Q \in R[X]$、$\deg(PQ) = \deg(P) + \deg(Q)$、从而 $a \cap R = 0$；因此限制到 R 是单射的。通过$f$将R与B的子环$f(R)$等同，并写成$b = f(X)$，我们看到$b$是B中P的根，P被视为$B[X]$中的多项式。那么$B[X]$中存在次数$n - 1$的一元多项式Q使得$P(X) = (X - b)Q(X)$(代数,章IV, § 1, no. 4,命题5)。到归纳假设，存在环$R' \supseteq B$，使得在$R'[X]$中，多项式Q是次数1的一元多项式的乘积；显然，在$R'[X]$中，P是次数1的单调多项式的乘积。

#### 命题 11 {#ac-v-s1-prop-11 .statement tag=04NN}

*设 A 为环，R A-代数，R[X] 中的 P 和 Q 首一多项式。如果 PQ 的系数在 A 上积分，则 P 和 Q 的系数在 A 上积分。*

通过双应用引理2，我们发现存在环R'包含R和R'的元素$(a_i)_{1 \leq i \leq m}, (b_j)_{1 \leq j \leq n}$族，使得在$R'[X]$
$$
P(X) = \prod_{i=1}^\infty (X - a_i), \quad Q(X) = \prod_{j=1}^n (X - b_j);
$$
P Q 属于的系数到 R' 中 A 的积分闭包 $A'$，因此 (no. 2, 命题 7) 元素 $a, (1 \leq i \leq m)$ 和 $b, (1 \leq j \leq n)$ 属于到 A。因此，P 和 Q 的系数是 A 上的积分（no. 1，推论 1 至命题 4）。

设 A 为整环，K 为分数的域，K' K-代数（不一定可交换）。给定 K 上的代数元素 $x \in K'$，首一多项式 $P \in K[X]$ 满足 $P(x) = 0$ 形式 $K[X]$ 的理想$a \neq 0$，必然是主项 (代数, 章 IV, § 1, no. 5， 命题7)。存在唯一的一元多项式生成 a；推广代数、章、V, § 3, no. 1、定义 3 中引入的术语，这个一元多项式将被称为 x 在 K 上的最小多项式。

#### 推论 {#ac-v-s1-n3-cor-1 .statement tag=04NO}

*设 A 为整环，K 为分数的域，以及 K-代数 K* 的 x 元素（不一定可交换）。 *如果 x 在 A 上积分，则 $x$ 在 $K$ 上的最小多项式 $P$ 在 $A$ 上积分（因此，如果 $A$ 是积分闭集，则它们从属于到 $A$）。

假设 (no. 1, 定理 1) 存在一个单调多项式$Q \in A[X]$，使得$Q(x) = 0$。如$K[X]$中的$P$除$Q$，从命题11可以得出$P$的系数在$A$上积分。

令 $A$ 为环且 $R$ 为（可交换的）$A$-代数；定义$R$上的$A$-代数结构的同态$\phi : A \to R$可以在$A$和$R$上唯一地扩展到多项式环的同态$A[X] \to R[X]$，留下$X$ 不变，因此 $R[X]$ 被赋予规范的 $A[X]$-代数结构。

#### 命题 12 {#ac-v-s1-prop-12 .statement tag=04NP}

令$A$为环，$R$为$A$代数，$P$为$R[X_1, \ldots, X_n]$的多项式。为了使$P$对$A[X_1, \ldots, X_n]$整的，$P$的系数对$A$积分是必要且充分的。

通过将 $R[X_1, \ldots, X_n]$ 的多项式视为 $X$ 中的多项式，系数在 $R[X_1, \ldots, X_{n-1}]$ 中，我们立即看到，对于 $n = 1$，它被简化为证明命题。然后令$P$为$R[X]$的多项式；由no. 1、命题 5 立即得出，若$P$的系数在$R$、元素、$P$中$A$的积分闭包$B$内，则属于为$B[X] = B \otimes_A A[X]$，是$A[X]$的积分。相反，假设 $P$ 是 $A[X]$ 的积分，并令

$$
Q(Y) = Y^m + F_1 Y^{m-1} + \cdots + F,
$$

是系数为$F_i \in A[X]$且$P$为根的一元多项式。令 $r$ 整数严格大于多项式 $P$ 和 $F_i$ ($1 \leq i \leq m$) 的所有次数，并让我们写

$$
P_1(X) = P(X) - X^r.
$$

那么$P_1$就是多项式的根

$$
Q_1(Y) = Q(Y + X') = Y^m + G_1 Y^{m-1} + \cdots + G,
$$

系数在$A[X]$；因此我们可以写

$$
-P_1(P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}) = G_r
$$

现在$r$的选择意味着$-P_1$是$R[X]$的一元多项式，$G_m(X) = Q(X^r)$也是如此，首一多项式$F_k(X) X^{r(m-k)}$的次数对于$k \geq 1$来说都是$< rm$。我们结论首先多项式

$$
P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}
$$

$R[X]$ 也是单数；而且，由于$G_i$属于到$A$的系数，命题11表明$P_1$在$A$上有系数积分，因此$P$的系数肯定在$A$上积分。

#### 命题 13 {#ac-v-s1-prop-13 .statement tag=04NQ}

令$A$为环，$\mathbf{R}$为$A$代数，$A'$为$A$在$\mathbf{R}$的积分闭包。那么$A[X_1, \ldots, X_n]$在$\mathbf{R}[X_1, \ldots, X_n]$的积分闭包等于$A'[X_1, \ldots, X_n]$。

这是从 no. 2 的命题 12 和定义 3 得出的。

#### 推论 1 {#ac-v-s1-prop-13-cor-1 .statement tag=04NR}

设$A$为整环，$A'$为其积分闭包。那么多项式环$A[X_1, \ldots, X_n]$的积分闭包就是$A'[X_1, \ldots, X_n]$。

由归纳对$n$进行争论，问题立即还原为$n = 1$。令$K$为$A$的分数的域，这也是$A'$的域；如果$A[X]$的分数$K(X)$域元素$P$在$A[X]$上积分，则属于到多项式环$K[X]$，因为后者是主理想整环 (代数、章IV, § 1, no. 5、命题7)，因此整体封闭(命题10)；然后将命题 13 应用于 $\mathbf{R} = K$ 得出推论。

#### 推论 2 {#ac-v-s1-prop-13-cor-2 .statement tag=04NS}

设$A$为整环。为了使多项式环$A[X_1, \ldots, X_n]$整体封闭，$A$整体封闭是必要且充分的。

#### 推论 3 {#ac-v-s1-prop-13-cor-3 .statement tag=04NT}

如果$K$是域，则每个多项式代数$K[X_1, \ldots, X_n]$都是一个积分闭域。

### 4. 完全封闭的域

#### 定义 5 {#ac-v-s1-def-5 .statement tag=04NU}

如果满足以下条件，整环$A$称为完全积分闭：域、分数、$K$、$A$的每一个元素$x$，使得所有幂$x^n$ ($n \geqslant 0$) 包含在$K$、属于到$A$ 的有限生成子A 模块中。

Note that the hypothesis that the $x^n$ are contained in a finitely generated sub-A-module of $K$ can also be expressed by saying that there exists a non-zero element $d \in A$ such that $dx^n \in A$ for all $n \geqslant 0$; for the latter condition means that $x^n \in Ad^{-1}$; and conversely, if $(b_i)_{1 \leqslant i \leqslant m}$ is a finite sequence of elements of $K$, there exists $d \in A$ such that $db_i \in A$ for $1 \leqslant i \leqslant m$, whence $dM \subset A$ for the sub-A-module $M$ of $K$ generated by the $b_i$.

显然，完全积分闭域是积分封闭的；反之，no. 1 命题 1 的推论表明，整闭的诺特域是完全整闭的。 \* 另一方面，高度$\geqslant 2$ (章 VI, § 4, no. 4) 的估值环是积分封闭的，但不是完全积分封闭的。 \* 如果$(A_i)$是一个完全积分闭域族，且域与分数$K$相同，则$A = \bigcap_i A_i$是完全积分闭域。因为如果$x \in K$是这样的，对于$A$，$dx^n$属于到$A$中的某些非零$d$，对于所有$n > 0$，假设意味着$x \in A$，对于所有$i$，因此$x \in A$。

#### 命题 14 {#ac-v-s1-prop-14 .statement tag=04NV}

*设$A$为完全积分闭域。那么每个多项式环$A[X_1, \ldots, X_n]$（分别是正式幂级数$A[[X_1, \ldots, X_n]]$的每个环）都是完全积分封闭的。*

通过$n$上的归纳，足以证明$A[X]$（或$A[[X]]$）是完全积分闭的。 Then let $P$ be an element of the field of fractions of $A[X]$ (resp. $A[[X]]$) and suppose that there exists a non-zero element $Q \in A[X]$ (resp. $Q \in A[[X]]$) such that $Q P^m \in A[X]$ (resp. $Q P'' \in A[[X]]$) for every integer $m \geq 0$. 如果$K$是$A$分数域，$A[X]$（分别$A[[X]]$）是$K[X]$（分别$K[[X]]$）和$K[X]$（分别$K[[X]]$）子环主理想整环 (*代数*, 章 VII, § 1, no. 1) 因此整体封闭 (no. 4, 命题 10) 和诺特 (*代数*, 章 VIII, § 2, no. 3) 因此完全整体封闭；那么我们已经看到了

$P \in K[X]$（分别为$P \in K[[X]]$）。设$P = \sum_{k=0}^{\infty} a_k X^k$ ($a_k \in K$) 和$Q = \sum_{k=0}^{\infty} b_k X^k$ ($b_k \in A$)，我们通过假设$a_i$ 并不都是属于到$A$ 来论证；那么至少有指标$i$使得$a_i \notin A$；如果我们写

$$
P_1 = \sum_{k=0}^{i-1} a_k X^k \in A[X],
$$

对于所有$m \geq 0$，紧接着假设还有$Q(P - P_1)^m \in A[X]$（或$Q(P - P_1)^m \in A[[X]]$）。令$j$是最小的整数，使得$b_j \neq 0$；显然，在至少次数的 $Q(P - P_1)^m$ 项中，系数 $\neq 0$ 是 $b_j a_i^m X^{j + mi}$，因此对于所有 $m \geq 0$ 来说，$b_j a_i^m \in A$；但由于$A$是完全积分闭的，这意味着$a_i \in A$，与假设相反。

#### 命题 15 {#ac-v-s1-prop-15 .statement tag=04NW}

*令$A$为经过过滤的环，其过滤是详尽的，并且$A$的每个主理想都在过滤定义的拓扑下封闭。如果关联的分级环$\mathrm{gr}(A)$（章III, § 2, no. 3）是一个完全积分闭域，则$A$是一个完全积分闭域。*

令$(A_n)_{n \in \mathbf{Z}}$为$A$上定义的过滤；因为 $\bigcap_{n \in \mathbf{Z}} A_n$ 是理想 (0) 的闭包 (章 III, § 2, no. 5)，假设首先意味着过滤 $(A_n)$ 被分离，并且由于 $\mathrm{gr}(A)$ 是整环，所以$A$ (章 III, § 2, no. 3，推论命题1)。 Let $x = b/a$ be an element of the field of fractions $K$ of $A$ ($a \in A, b \in A$) for which there exists an element $d \neq 0$ of $A$ such that $dx^n \in A$ for all $n \geq 0$. 我们必须证明 $b \in A a$ 并且，到假设时，理想的 $A a$ 已关闭，足以证明，对于所有 $n \in \mathbf{Z}, b \in A a + A$。 由于$A$的过滤是穷举的，因此存在整数$q \in \mathbf{Z}$使得$b \in A a + A_q$。 因此，只要证明关系$b \in A a + A_q$蕴含$b \in A a + A_{q+1}$即可。

假设 $b = a y + z$ 其中 $y \in A, z \in A_{q+1}$。然后通过假设$dx^n \in A$对于所有$n \geq 0$，从而我们立即获得对于所有$n \geq 0$的$d(x - y)^n \in A$；在其他字、$dz^n = a^n t_n$ 中，$t_n \in A$ 代表所有 $n \geq 0$。显然，我们可以将极限的注意力集中到$z \neq 0$的情况。让$v$表示$A$（章III, § 1, no. 2）上的阶函数，并让我们写成$v(d) = n_1,\ v(z) = n_2 \geq m,\ v(a) = n_3$；设$d', z', a'$为$A_{n_1}/A_{n_1+1},\ A_{n_2}/A_{n_2+1},\ A_{n_3}/A_{n_3+1}$中$d, z, a$各自的像。对于所有$n \geq 0,\ v(dz^n) = n_1 + nn_2$（章III, § 2, no. 3，命题1），因此$dz^n$的$\mathrm{gr}(A)$中的典范像是$d'{z'}^n$；类似地，可以看出，$a^n t_n$的$\mathrm{gr}(A)$中的典范像是形式${d'}^n t'_n$，其中$t'_n \in \mathrm{gr}(A)$，并且，对于所有$n \geq 0,\ d'(z'/a')^n \in \mathrm{gr}(A)$，我们推断出$a' \neq 0$。 假设 $\mathrm{gr}(A)$ 是完全积分闭的，因此意味着存在$s' \in \mathrm{gr}(A)$使得$z' = a's'$；将$s'$分解为齐次元素的和，进一步看出（因为$z'$和$a'$是齐次的）$s'$可以被假设为齐次的，即元素$s \in A$的像；然后$v(as) = v(z) = n_2$和$z \equiv as \pmod{A_{n_2+1}}$；作为$n_2 \geq m, a fortiori$$z \equiv as \pmod{A_{m+1}}$，因此$b \equiv a(y+s) \pmod{A_{m+1}}$。

### 5. 环分数的整体闭合

令$A$为环，$R$为$A$代数，$S$为$A$的乘法子集。回想一下 (章 II, § 2, no. 8)，$S^{-1}R$ 有一个规范的 $S^{-1}A$-代数结构。

#### 命题 16 {#ac-v-s1-prop-16 .statement tag=04NX}

*令$A$为环，$R$为$A$代数，$A'$为$R$中$A$的积分闭包，以及$S$为$A$的乘法子集。那么$S^{-1}A$在$S^{-1}R$的积分闭包就是$S^{-1}A'$。*

设$b/s$为$S^{-1}A'$($s \in S,\ b \in A'$)中的元素。从图表开始

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
\downarrow h & & \downarrow S^{-1}h \\
R & \xrightarrow{i_R^S} & S^{-1}R
\end{array}
$$

是可交换的，$b/1$ 对 $S^{-1}A$ (no. 1, 命题 2) 是积分。由于$1/s \in S^{-1}A$，$b/s = (b/1)(1/s)$是$S^{-1}A$的积分。

Conversely, let $r/t \ (r \in R,\ t \in S)$ be an element of $S^{-1}R$ which is integral over $S^{-1}A$; then $r/1 = (t/1)(r/t)$ is integral over $S^{-1}A$. 那么形式就有关系

$$
(r/1)^n + (a_1/s)(r/1)^{n-1} + \cdots + (a_n/s) = 0,
$$

其中$a_i \in A \ (1 \leq i \leq n)$和$s \in S$。这个关系也可以写成

$$
(sr^n + a_1 r^{n-1} + \ldots + a_n)/s = 0
$$

因此存在$s' \in S$使得${s'}^n(sr^n + a_1 r^{n-1} + \ldots + a_n) = 0$；我们推断出$(s'sr)^n + s'a_1(s'sr)^{n-1} + \ldots + {s'}^ns^{n-1}a_n = 0$。通过定义，因此$s'sr \in A'$、从而 $r/1 \in S^{-1}A'$ 和 $r/t \in S^{-1}A'$。

#### 推出 1 {#ac-v-s1-prop-16-cor-1 .statement tag=04NY}

令$A$为整环，$A'$为其积分闭包，$S$为$A$的乘法子集，使得$0 \notin S$。那么$S^{-1}A$的积分闭包就是$S^{-1}A'$。

$A$分数$R$域也是从$0 \notin S$起$S^{-1}A$分数域(章II, § 1, no. 1、注7)；然后将命题 16 应用于$R$。

#### 推出 2 {#ac-v-s1-prop-16-cor-2 .statement tag=04NZ}

令$A$为整环，$K$为分数的域，$R$代数在$K$上，以及$B$$A$在$R$上的积分闭包。 $R$的元素是$K$（no. 1，例 1）的代数，是形式$a^{-1} b$的元素，其中$b \in B$和$a \in A, a \neq 0$；如果$R$中$L$是$K$的代数闭包，则$B$中存在$L$的基超过$K$。

第一个断言源自应用于案例 $S = A - \{0\}$ 的命题 16。如果$(x_i)_{i \in I}$是$L$的基超过$K$，则对于$A$的所有$i \in I$元素$a_i \neq 0$，存在$a_i x_i \in B$；那么 $(a_i x_i)_{i \in I}$ 也是 $L$ 的基超过 $K$。

#### 推论 3 {#ac-v-s1-prop-16-cor-3 .statement tag=04O0}

令$A$为$A$的最大理想的整环和$\Omega$集合。为了使$A$整体闭合，对于所有$m \in \Omega$、$A_m$整体闭合是必要且充分的。

由推论1可知条件是必要的。对于 $A = \bigcap_{m \in \Omega} A_m$ (章 II, § 3, no. 3, 公式 (2))，条件是足够的，并且将推论应用于 no. 2 的命题 8 就足够了。

#### 推论 4 {#ac-v-s1-prop-16-cor-4 .statement tag=04O1}

令$A$为整环，$K$为分数的域，$S$为$A$的乘法子集，使得$0 \notin S$。

(i) 令$B$为$K$的子环，它是$A$的积分，并令$\mathfrak{f}$为$A$模$B/A$的湮没子。 Then $S^{-1}\mathfrak{f}$ is contained in the annihilator of the $(S^{-1}A)$-module $S^{-1}B/S^{-1}A$ and is equal to this annihilator if $B$ is a finitely generated $A$-module.

(ii) 设$A'$为$A$的积分闭包。为了使$S^{-1}A$整体闭合，$A$模$A'/A$的湮没子$\mathfrak{f}$满足$S$就足够了。如果$A'$是有限生成的$A$模块，那么这个条件也是必要的。

(i) 由于$\mathfrak{f}B \subset A$、$(S^{-1}\mathfrak{f})(S^{-1}B) \subset S^{-1}A$，因此$S^{-1}\mathfrak{f}$包含在$\operatorname{Ann}(S^{-1}B/S^{-1}A)$中。如果$B$是有限生成的$A$模，则方程$S^{-1}\mathfrak{f} = \operatorname{Ann}(S^{-1}B/S^{-1}A)$是章II, § 2, no. 4的公式(9)的特例，$S^{-1}B/S^{-1}A$被规范地标识为$S^{-1}(B/A)$。

(ii) 由推论 1 $S^{-1}A'$ 是$S^{-1}A$ 的积分闭包。由于关系 $\mathfrak{f} \cap S \neq \varnothing$ 和 $S^{-1}\mathfrak{f} = S^{-1}A$ 等价 (章 II, § 2, no. 5, 注) (ii) 是 (i) 的直接的推论。

如果$B$是$K$的子环（对$A$整的），$B/A$的湮没子$f$（等于定义到运输机$A : B$（章I, § 2, no. 10））是有时称为$A$ 中$B$ 的*导体*。

#### 推论 5 {#ac-v-s1-prop-16-cor-5 .statement tag=04O2}

*令$A$为整环，$A'$其整体闭包以及$A$模块$A'/A$的$f$湮没子。假设$A'$是有限生成的$A$模块。使 $A_p$ 不全闭的素理想 $p \in A$ 是包含 $f$。*

这直接源自适用于 $S = A - p$ 的推论 **4 (ii)**。

注在推论 5 $f \neq 0$ 的假设下，因为 $A'$ 是有限生成的 $A$ 模，并且 $K/A$ 的每个元素（$A$ 分数的$K$ 域）有湮没子$\neq 0$。

*在代数几何中，推论5和上面的注表明点，其中仿射簇$V$不是正规的形式闭集合，与$V$不同。* \*

### 6. 范数和整数的痕迹

#### 命题 17 {#ac-v-s1-prop-17 .statement tag=04O3}

*令$A$为环，$B$一个（可交换的）$A$代数，以及阶$n$在$B$上的$X$平方矩阵；以下属性是等效的：

(a) $X$ 是$A$ 的积分。

(b) 存在$B^n$的有限生成子$A$模块$M$，使得所有$x \in M$和$M$的$X.x \in M$是$B$模块$B^n$的生成元的系统。

(c) $X$的特征多项式的系数在$A$上积分。*

如果 $\chi(T) = \det(T.1 - X)$ 是 $X$ 的特征多项式，则 Cayley-Hamilton 定理显示 $\chi(X) = 0$ (*代数*, 章 VII, § 5, no. 4, *注* 1) 并且，因为 $\chi$ 是一个单调函数多项式，(c) 通过 no. 1、命题 6 隐含 (a)。

第二位假设 (a) 成立。如果$(e_i)_{1 \leq i \leq n}$是$B^n$的典范基，则$X^k.e_i$（$1 \leq i \leq n, k \geq 0$）生成的$B$的子$A$模$M$是有限生成的$A$模，因为$A$代数$A[X]$是有限生成的 $A$-模块 (no. 1, 定理 1)；由$M$包含和$e_i$可知，(a)蕴涵(b)； 逆命题是 no. 1、定理 1、条件 (E_{III}) 中的推论。

最后让我们证明(a)蕴涵(c)；因为$X$是$A$的积分，并且*更不必说*是多项式环$A[T]$的积分，$T.1 - X$也是$A[T]$的积分，并且到no. 3，命题12问题可以看出约化（由替换 $X$ $T.1 - X$ 和 $A$ $A[T]$）到证明，如果 $X$ 是 $A$ 的整数，$d = \det(X)$ 是元素 $B$是$A$的积分。现在，我们在上面看到，由$X$定义的$B^n$的自同态$u$留下了稳定的有限生成的子$A$模块$M$包含于$e_i$； $n$-向量$x_1 \wedge x_2 \wedge \ldots \wedge x_n$，其中$x_i \in M$代表$1 \leq i \leq n$，因此$\bigwedge^n(B^n)$中的生成是有限生成的子$A$-模块包含$e_1 \wedge e_2 \wedge \ldots \wedge e$，并且在$\bigwedge^n u$下稳定，在其他情况下比率$d$的字低于位似； 湮没子的

$$
e_1 \wedge e_2 \wedge \ldots \wedge e,
$$

在 B 约化到 0、no. 1、定理 1 的条件 (E_{III}) 中证明 d 在 A 上是积分。

#### 推论 1 {#ac-v-s1-prop-17-cor-1 .statement tag=04O4}

设 A 为整环，K 为分数的域，K' 为有限维 K-代数（不一定可交换）。如果 x \in K' 在 A 上积分，则特征多项式 Pc_{K'/K}(x; X) (代数, 章 VIII, § 12, no. 2) 在 A 上积分。

如果 z \mapsto M(z) 是代数 K' 的正则表示 (视为矩阵表示; cf. 代数, 章 VIII, § 13) Pc_{K'/K}(x; X) 由定义矩阵 M(x) 的特征多项式；如果 x 右 A 整的，矩阵 M(x) 右 A (no. 1, 命题 2) 整的，并且足以应用命题 17。

#### 推论 2 {#ac-v-s1-prop-17-cor-2 .statement tag=04O5}

利用与推论 1 中相同的假设和记号，Tr_{K'/K}(x) 和 N_{K'/K}(x) 右 A 是积分。

Tr_{K'/K}(x) 和 N_{K'/K}(x) 在符号范围内是 Pc_{K'/K}(x; X) (代数, 章 VIII, § 12, no. 1, 方程 (4)) 的系数，因此是积分。

#### 注 (1) {#ac-v-s1-n6-rem-1 .statement tag=04O6}

如果 K' 是 K 上的简单中心代数，且 K' 中的 x 是 A 上的积分，则 x 的约简特征多项式 (代数, 章 VIII, § 12, no. 3) 的系数在 A 上积分。因为该多项式的幂等于 Pc_{K'/K}(x; X）（前述，命题8）并且足以满足应用命题17和no. 3，命题11。

#### 命题 18 {#ac-v-s1-prop-18 .statement tag=04O7}

设A是一个积分闭域，K是分数的域，K'是有限维可分K-代数（代数，章VIII, § 7, no. 5），A'是A在K'中的积分闭包。那么A'包含在有限生成的A-模中。

命题由以下更精确的引理得出：

#### 引理 3 {#ac-v-s1-lem-3 .statement tag=04O8}

在命题 18 的假设下，令 (w_1, ..., w_n) 为 K' 相对于 A' 中包含的 K 的基（no. 5，推论 2 至命题 16）；那么 K' 在 K 上有唯一的基 (w_1^*, ..., w_n^*) ，其中 Tr_{K'/K}(w_i w_j^*) = \delta_{ij} (Kronecker 指标)；如果 d = D_{K'/K}(w_1, ..., w_n) 是基 (w_1, ..., w_n) (代数, 章 IX, § 2) 的判别式，则 d \neq 0 且

$$
\sum_{i=1}^n Aw_i \subset A' \subset \sum_{i=1}^n Aw_i^* < d^{-1} \left( \sum_{i=1}^n Aw_i \right).
$$

特别是，如果 d 是 A 的可逆元，则 A' 是自由A-模且基 (w_1, ..., w_n)。

由于 K' 是可分离的 K-代数，因此 d \neq 0 (代数, 章 IX, § 2, 命题 5) 和 K 双线性形式

$$(x, y) \mapsto \operatorname{Tr}_{K'/K}(xy)$$

因此 K' 上是非简并的（*loc. cit.*, 命题 4）；这表明基$(w_i^*)_{1 \leq i \leq n}$的存在和唯一性（*代数*，章IX, § 1, no. 6，命题6的推论）。既然如此，（2）的第一个包含是显而易见的。设$x$为$A'$的元素；让我们在 $\xi_i \in K$ 处写出 $x = \sum_{i=1}^n \xi_i w_i^*$；对于所有$i$、$\xi_i = \mathrm{Tr}_{K'/K}(xw_i)$，因此$\xi_i$是$A$的积分（推论2到命题17），并且由于$A$是积分闭集，$\xi_i \in A$对于$1 \leq i \leq n$；这显示了第二个包含项 (2)。最后，让我们在 $\alpha_{ji} \in K$ 处写出 $w_j^* = \sum_{i=1}^n \alpha_{ji} w_i$；那么 $$\sum_{i=1}^n \alpha_{ji} \mathrm{Tr}_{K'/K}(w_i w_k) = \delta_{jk}$$ 对于所有 $j$ 和 $k$； Cramer 的公式显示 $\alpha_{ji}$ 属于至 $d^{-1}A$、从而第三个包含体 (2)。 最后一个断言紧接着 (2)，在本例中给出$A' = \sum_{i=1}^n Aw_i$。

在遵循假设和记号的两个推论中，是命题18的推论。

#### 推论 1 {#ac-v-s1-lem-3-cor-1 .statement tag=04O9}

*如果$A$是诺特环，则$A$-模块$A'$是有限生成的，特别是环$A'$是诺特。*

$A'$ 是有限生成的 $A$ 模块的子模。

#### 推论 2 {#ac-v-s1-lem-3-cor-2 .statement tag=04OA}

*如果 $A$ 是主理想整环，$A'$ 是秩 $n$ 的免费 $A$ 模块。* 每一个子模的免费 $A$ 模块都是免费的（*代数*、章 VII, § 3， 定理1)。

#### 推论 3 {#ac-v-s1-lem-3-cor-3 .statement tag=04OB}

*令$E$为有理数数的域$Q$次数$n$扩张。 有理整数的环$Z$的$E$积分闭包的加法群是秩$n$的自由交换群。*

$Z$ 是整体闭集（no. 3，命题 10），$E$ 是可分的，因为 $Q$ 的特征为 0。因此，推论 2 可以应用于$A = Z$、$K = Q$ 和 $K' = E$ 的情况。

*注(2)*。 如果不假设 $K'$ 与 $K$ 是分离的，即使$K'$ 是 $K$ (习题 20) 的扩张域，推论 1 的结论也不一定成立。 On the other hand, if $A$ is a *finitely generated integral $K_0$-algebra*, where $K_0$ is a *field*, the integral closure of $A$ in *any* extension of finite degree of the field of fractions of $A$ is a finitely generated $A$-module and a Noetherian ring, as we shall see in § 3, no. 2, Theorem 2.

### 7. 整闭代数中标量的扩张

#### 命题 19 {#ac-v-s1-prop-19 .statement tag=04OC}

*令$k$为域、$L$可分扩张的$k$和$R$积分闭$k$代数。如果环 $L \otimes_k R$ 是整环，则它是积分闭的。*

令K为R的分数的域；因为 k 为域，L $\otimes_k$ R 被规范地识别为 L $\otimes_k$ K 和 L 的子 k 代数，而 R 则被 L $\otimes_k$ R 的子 k 代数识别。 此外，由于 R 的元素 s $\# 0$ 不是 R 中 0 的除子，因此 1 $\otimes s$ 不是 L $\otimes_k$ R 中零的除子，因为 L 在 k 上是平坦的 (章) I, § 2, no. 3);将 s 标识为 1 $\otimes s$，因此可知，如果 S = R - {0}，则 L $\otimes_k$ K 标识为 S$^{-1}$(L $\otimes_k$ K)；由于 L $\otimes_k$ R 被假定为整环，L $\otimes_k$ K 因此被识别为分数 $\Omega$ 的 L $\otimes_k$ R 的域的子环。

(1) Suppose that L is a finite extension of k; then L $\otimes_k$ K is an algebra of finite rank over K and by hypothesis has no divisor of 0; hence it is a field (Algebra, Chapter V, § 2, no. 1, Proposition 1) and therefore it is in this case the field of fractions $\Omega$ of L $\otimes_k$ R. 令($w_1, \ldots, w_r$)为L除以k的基，因此它也是L$\otimes_k$K除以K的基。 存在L的基($w_1^*, \ldots, w_n^*$)使得$\mathrm{Tr}_{L/k}(w_i w_j^*) = \delta_{ij}$(no. 6,引理3)；每个$z \in L \otimes_k K$都可以唯一地写成$z = \sum_{i=1}^u a_i w_i$，其中$a_i \in K$；然后

$$
\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = \sum_{i=1}^n a_i \mathrm{Tr}_{(L \otimes K)/K}(w_i w_j^*)
$$

如L中的痕迹$\mathrm{Tr}_{(L \otimes K)/K}$和$\mathrm{Tr}_{L/K}$重合（代数，章VIII, § 12, no. 2，公式（13））最后$\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = a_j$，对于$1 \leq j \leq n$。 注另一方面，L 的元素是 k 上的积分，因此也是 R 上的积分（no. 1，推论 1 到命题 2）；因此 (no. 1, 命题 5) L $\otimes_k$ R 是 R 上的积分。 既然如此，假设 $z \in L \otimes_k K$ 是 L $\otimes_k$ R 上的积分；那么 z 也是 R 上的整数 (no. 1, 命题 6)，因此 $z w_j^*$ 也是如此，因此对于 $1 \leq j \leq n$ 也是 $a_j = \mathrm{Tr}_{(L \otimes K)/K}(z w_j^*)$（no. 6，推论 2 到命题 17）。由于 R 是积分闭集，因此对于所有 $j$ 都有 $a_j \in R$，因此也有 $z \in L \otimes_k R$，在这种情况下证明了命题。

(2) 现在假设L是K的有限生成的可分扩张；则存在 L 对 k (代数, 章 V, § 9, no. 3, 定理 2) 的分离超越基 ($x_1, \ldots, x_d$);由于 L 和 K 在域 $\Omega$ (代数, 章 V, § 5, no. 4) 中在代数上不相交的于 k，因此 $x_i$ 在 K 上代数独立；因此 $R[x_1, \ldots, x_d]$ 是积分闭的（no. 3，推论 2 到命题 13）。令T为环$A = k[x_1, \ldots, x_d] \subset L$的元素$\neq 0$中的集合，使得域$k_1 = k(x_1, \ldots, x_d) \subset L$等于$T^{-1}k[x_1, \ldots, x_d]$；然后

$$
k_1 \otimes_k R = (T^{-1}A) \otimes_k R = T^{-1}A \otimes_A (A \otimes_k R) = T^{-1}(A \otimes_k R)
= T^{-1}R[x_1, \ldots, x_d]
$$

通过张量积的结合性，因此该域是整体封闭的（no. 5，推论 1 到命题 16）。但 $L \otimes_k R$ 等同于

L \otimes_{k_1} (k, \otimes_k R) 和定义 L 是 $k_1$ 的有限可分扩张；因此，从 (1) 可以得出 $L \otimes_k R$ 是整闭的。

(3) *一般情况。*如果$z$是$\Omega$对$L \otimes_k R$积分的元素，则满足形式$z^m + b_1 z^{m-1} + \ldots + b_m = 0$的关系，其中$b_i$属于到$L \otimes_k R$；则存在$k$上L的有限生成子扩展$L'$，使得$1 \leq i \leq m$的$b_i$属于到$L' \otimes_k R$和$z$到$L' \otimes_k K$。那么从 (2) 可以得出 $z \in L' \otimes_k R$ 以及$L \otimes_k R$ 是积分闭的。

\* 令V为仿射不可约代数簇，$k$定义V的域和函数正则的$R$环在$k$上定义的V；如果 R 是积分闭集，则 V 称为 *正规于 $k$*； 命题 19 表明，如果 V 在 $k$ 上正常，则在 $k$ 的每个可分扩张 L 上保持正常。 \*

#### 推论{#ac-v-s1-n7-cor-1 .statement tag=04OD}

*设k为域，R和S为两个整体封闭的K-代数。假设环$R \otimes_k S$是整环，并且分数K的域和R和S的L分别在k上可分离。那么环 $R \otimes_k S$ 是一个全闭域。*

As R and S are identified with subalgebras of $R \otimes_k S$, K and L are identified with subfields of the field of fractions $\Omega$ of $R \otimes_k S$ which are linearly disjoint over $k$ (*Algebra*, Chapter V, § 2, no. 3, Proposition 5). 由命题 19 可知$R \otimes_k L$ 和$K \otimes_k S$ 是整闭域；由于它们的交是$R \otimes_k S$（章I, § 2, no. 6，命题7），$R \otimes_k S$是一个全闭域（no. 2，命题8的推论）。

\* 给定两个不可约仿射簇V，W在$k$上定义，它们的乘积$V \times W$是仿射簇，$V \times W$上正则的函数的环与环的$k$上的张量积进行识别V 上的函数正则和 W 上的函数正则环。 命题 19 的推论表明，如果 V 和 W 在 $k$ 上正常，则 $V \times W$ 在 $k$ 上正常。 \*

### 8. 整数超过评分环

*All the graduations considered in this no. are of type $\mathbf{Z}$; if A is a graded ring and $i \in \mathbf{Z}$, $A_i$ denotes the set of homogeneous elements of degree $i$ of the ring A.*

设 A 为环等级，B 为 A-代数等级。设 x 是 B 的 *齐次* 元素，它是 A 的积分；那么就有关系

$$
x^n + a_1 x^{n-1} + \ldots + a_n = 0 \quad \text{where } a_i \in A \quad \text{for } 1 \leq i \leq n.
$$

令$m = \deg(x)$和$a'_i$为$a_i$($1 \leq i \leq n$)的次数$mi$的齐次分量；那么显然

$$
x^n + a'_1 x^{n-1} + \ldots + a'_n = 0
$$

在其他情况下，字 x 满足具有*齐次*系数的积分相关方程。

令$\mathbf{A}[X, X^{-1}]$表示一个不定式中分数$S^{-1}\mathbf{A}[X]$、多项式环$\mathbf{A}[X]$的环，$S$是$\mathbf{A}[X]$由……组成与幂的乘法子集 $X$ ($n \geq 0$) 中的$X^n$；因为$X$不是$\mathbf{A}[X]$中0的除子，所以$X^i$（$i \in \mathbf{Z}$）形式基超过$\mathbf{A}$-模块$\mathbf{A}[X, X^{-1}]$的$\mathbf{A}$是直接的。 对于每个具有同质分量 $a_i$ ($i \in \mathbf{Z}$) 的元素 $a \in \mathbf{A}$，我们写

$$
j_{\mathbf{A}}(a) = \sum_{i \in \mathbf{Z}} a_i X^i \in \mathbf{A}[X, X^{-1}]
$$

直接的 $j_{\mathbf{A}} : \mathbf{A} \to \mathbf{A}[X, X^{-1}]$ 是单射环同态。

#### 命题 20 {#ac-v-s1-prop-20 .statement tag=04OE}

*令 $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} A_i$ 为分级环，$\mathbf{B}$ 为（交换）分级 $\mathbf{A}$ 代数。 $\mathbf{B}$积分的集合$\mathbf{A}'$对$\mathbf{A}$的元素积分是$\mathbf{B}$的分级子代数。

如果 $i < 0$ 的 $A_i = 0$ 和 $\mathbf{B}$ 是环的约化环，则 $i < 0$ 的 $A'_i = 0$。*

The diagram

$$
\begin{array}{ccc}
\mathbf{B} & & \mathbf{A} \\
& \rho & \\
& & \\
& & \\
\mathbf{A}[X, X^{-1}] \xrightarrow{\phi'} \mathbf{B}[X, X^{-1}] \\
\end{array}
$$

（其中$\rho$是定义$\mathbf{B}$上的$\mathbf{A}$代数结构的同态，并且$\rho'$同态规范地从中导出）是可交换的，正如从定义（5）中立即验证的那样。设$x$为$\mathbf{B}$对$\mathbf{A}$积分的元素；那么 $j_{\mathbf{B}}(x)$ 是 $\mathbf{A}[X, X^{-1}]$ (no. 1, 命题 2) 的积分，因此从 no. 5, 命题 16 可以得出，存在整数 $m > 0$，使得 $X^m j_{\mathbf{B}}(x)$ 是元素 $\mathbf{B}[X]$ 对 $\mathbf{A}[X]$ 整的。然后我们从no. 3、命题 12 推导出多项式$X^m j_{\mathbf{B}}(x)$的系数在$\mathbf{A}$上积分；由于这些系数是$x$的齐次分量定义，因此可以看出它们在$\mathbf{A}$上积分，这证明$\mathbf{A}'$是$\mathbf{B}$的分级子代数。

现在假设 $x \in A'_i$ 其中 $i < 0$; 注在此编号的开头。表明 $x$ 满足方程形式 (4)，其中 $a_k' \in A_{kt}$ 满足 $1 \leq k \leq n$。如果$A_j = 0$代表$j < 0$，则$x^n = 0$，如果$\mathbf{B}$是减少的环，我们结论即$x = 0$，因此在这种情况下，对于所有$i < 0$，$A'_i = 0$。

回想一下 (章 II, § 2, no. 9)，如果 $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ 是分级环并且 $S$ 是 *同质* 元素的 $\mathbf{A}$ 由……组成的乘法子集，则分级环结构是在$S^{-1}\mathbf{A}$上定义，将次数$i$的齐次元素的集合$(S^{-1}\mathbf{A})_i$取形式$a/s$的元素集合，其中$a \in \mathbf{A}$和$s \in S$ 是齐次的并且使得 $\deg(a) - \deg(s) = i$

#### 引理 4 {#ac-v-s1-lem-4 .statement tag=04OF}

令$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$为$\mathbf{A}$的同质元素$\neq 0$的分级整环和$S$集合。

(i) $S^{-1}\mathbf{A}$ 的每个齐次元素 $\neq 0$ 都是可逆的，环 $K_0 = (S^{-1}\mathbf{A})_0$ 是域和 $i \in \mathbf{Z}$ 的集合，使得 $(S^{-1}\mathbf{A})_i \neq 0$ 是子群 $q\mathbf{Z}$ $\mathbf{Z}$（其中$q \geqslant 0$）。

(ii) 假设 $q \geqslant 1$ 并令 $t$ 为 $(S^{-1}\mathbf{A})_q$ 的非零元素。然后将多项式环$K_0[X]$到$S^{-1}\mathbf{A}$的$K_0$同态$f$到映射$X$到$t$扩展到$K_0[X, X^{-1}]$的同构到$S^{-1}\mathbf{A}$和$S^{-1}\mathbf{A}$是整体封闭的。

(i)中的断言紧接着从定义和假设得出$\mathbf{A}$是整环，因为如果$a/s$和$a'/s'$是次数$S^{-1}\mathbf{A}$的两个齐次元素$\neq 0$ $i$和$i'$、$aa'/ss'$是齐次元素$\neq 0$和次数$i + i'$。为了证明(ii)，我们注，因为$t$在$S^{-1}\mathbf{A}$同态$f$扩展中以一种独特的方式可逆到同态$\tilde{f}: K_0[X, X^{-1}] \to S^{-1}\mathbf{A}$并且必然$\tilde{f}(X^{-1}) = t^{-1}$。另一方面，通过$q$的定义，$S^{-1}\mathbf{A}$的每个齐次元素$\neq 0$都是次数$qn \ (n \in \mathbf{Z})$，因此可以唯一地写成形式$\lambda t^n$，其中$\lambda \in K_0$（因为$S^{-1}\mathbf{A}$ 为整环)；因此 $\tilde{f}$ 是双射的。最后，我们知道$K_0[X]$是整体闭的（no. 3，命题10），因此$K_0[X, X^{-1}]$也是整体闭的（no. 5，推论1到命题16），从而完成了引理的证明。

#### 命题 21 {#ac-v-s1-prop-21 .statement tag=04OG}

令$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$为$\mathbf{A}$的齐次元素$\neq 0$的分级整环和$S$集合。 $\mathbf{A}$的积分闭包$\mathbf{A}'$则为$S^{-1}\mathbf{A}$的分级子环。如果进一步将$\mathbf{A}_i = 0$换成$i < 0$，则将$\mathbf{A}'_i = 0$换成$i < 0$。

如果$\mathbf{A} = \mathbf{A}_0$，命题是微不足道的。否则我们可以申请引理4； 环 $S^{-1}\mathbf{A}$ 是一个积分闭域，因此$\mathbf{A} \subset S^{-1}\mathbf{A}$；由于 $S^{-1}\mathbf{A}$ 已分级，$\mathbf{A}'$ 也按命题 20 分级；后者断言也是从命题20得出的。

#### 推论 1 {#ac-v-s1-prop-21-cor-1 .statement tag=04OH}

假设命题 21 和记号，如果$S^{-1}\mathbf{A}$ 的每个齐次元素在$\mathbf{A}$ 属于到$\mathbf{A}$ 上积分，则$\mathbf{A}$ 是积分闭的。

然后$\mathbf{A}'_i \subset \mathbf{A}$对于所有$i \in \mathbf{Z}$，因此$\mathbf{A}' = \mathbf{A}$。

#### 推论 2 {#ac-v-s1-prop-21-cor-2 .statement tag=04OI}

若$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$是积分闭分级域，则域$\mathbf{A}_0$也是积分闭。

The field of fractions $K_0$ of $\mathbf{A}$, is identified (in the notation of Proposition 21) with a subring of the ring of homogeneous elements of degree 0 of $S^{-1}A$; every element of $K_0$ integral over $A$, (and *a fortiori* over $A$) belongs therefore by hypothesis to $A$.

#### 推论 3 {#ac-v-s1-prop-21-cor-3 .statement tag=04OJ}

*令$A = \bigoplus_{i \in \mathbf{Z}} A_i$为积分闭分级域。那么，对于每个整数 $d > 0$，环 $A^{(d)}$ (章 III, § 1, no. 3) 都是一个积分闭域。*

令$U$为$A^{(d)}$的齐次元素$\neq 0$的集合，并让$x$为$U^{-1}A^{(d)}$在$A^{(d)}$上的齐次元素积分，从而在$A$上；如 $x \in S^{-1}A$、$x$ 属于至 $A$ 假设；因为它的次数可以被$d$整除，所以它属于到$A^{(d)}$，然后从推论1可以得出$A^{(d)}$是整闭的。

### 9. 应用：群 OF 自同构 OF AN 代数的不变量

给定环 $K$、$K$-代数 $A$ 和群 $G$，我们可以说 $G$ 对 $A$ 进行运算，如果： (1) 集合 $A$ 有群 $G$ (*代数*, 章 I, § 7, no. 2); (2) 对于所有 $\sigma \in G$，映射 $x \mapsto \sigma.x$ 是 $K$-代数 $A$ 的 *自同态*（因此是 *自同构*，因为它是双射的 (*loc.cit.*)）。我们用$A^G$、集合、元素、$A$表示，它们在$G$下*不变*；显然它是$A$的*亚K代数*。

我们可以说，$G$是$A$上的*局部有限*群运算符，如果$A$中$G$的每个*轨道*（*代数*，章I，对*分册*的更正） IV) 是*有限*。

#### 命题 22 {#ac-v-s1-prop-22 .statement tag=04OK}

*令$A$为（可交换的）$K$代数，而$G$为$A$上的本地有限群运算符。那么$A$是子代数$A^G$的积分。*

对于所有$x \in A$，令$x_i$（$1 \leq i \leq n$）为$G$下$x$的轨道的不同元素；对于所有$\sigma \in G$，存在集合$\{1, 2, \ldots, n\}$的置换$\pi_\sigma$，使得$\sigma.x_i = x_{\pi_\sigma(i)}$对应于$1 \leq i \leq n$；因此，$x_i$的基本对称函数是$A$的元素，它们在$G$下不变，在$A^G$的其他字元素中不变。由于$x$是一元多项式$\prod_{i=1}^n (X - x_i)$的根，并且该多项式属于到$A^G$的系数，$x$是$A^G$的积分。

#### 定理 2 {#ac-v-s1-thm-2 .statement tag=04OL}

*令$A$是有限生成的$K$代数，$G$是$A$上的局部有限群运算符。那么$A$是有限生成的$A$-模；如果进一步$K$是诺特，则$A^G$亲和生成$K$-代数。*

令$(a_j)_{1 \leq j \leq m}$为$K$-代数$A$的生成元的系统；由于 *更不必说* $A = A^G[a_1, \ldots, a_l]$ 和 $a_j$ 在 $A^G$ 上除以命题 22 整的，第一个断言由 no. 1、命题 4 得出。第二个是以下引理的推论：

#### 引理 5 {#ac-v-s1-lem-5 .statement tag=04OM}

*令 $K$ 为诺特环，$B$ 为有限生成的 $K$ 代数，$C$ B 的子 K 代数，使得 B 在 C 上积分。那么C就是有限生成的A-代数。

令$(x_i)_{1 \leq i \leq n}$为K-代数B的生成元的有限系统。对于所有i，假设存在一个单调多项式$P_i \in C[X]$使得$P_i(x_i) = 0$。令C'为由$P_i$($1 \leq i \leq n$)的系数生成的C的子K代数；显然，$x_i$是C'和$B = C'[x_1, \ldots, x_n]$的积分；因此 B 是有限生成的 C'-模块 (no. 1, 命题 4)。另一方面，$C'$是诺特环（章III, § 2, no. 10，推论3到定理2）；因此C是有限生成的$C'$模，这证明C是有限生成的K-代数。

#### 注 {#ac-v-s1-n9-rem-1 .statement tag=04ON}

$\sigma \in G$的集合，使得$1 \leq j \leq m$的$\sigma a_j = a_j$显然在A的每元素保持不变。因此，$G$的正常子群$\mathscr{H}$在A的每元素保持不变，因此是有限的$G$中的指标，A可被认为具有有限群个运算符$G/\mathscr{H}$；显然$A^{G/\mathscr{H}} = A^G$。

设 S 是环 A 和 $G$ 群在 A 上运行的乘法子集，且 S 是稳定的；那么，对于所有$\sigma \in G$，存在环$S^{-1}A$的唯一内同态$z \mapsto q_z$，使得对于所有$a \in A$有$q_z(a/1) = (a.a)/1$；对于 $a \in A$ 和 $s \in S$，它由公式 $\sigma.(a/s) = (\sigma.a)/(\sigma.s)$ 给出（章 II, § 2, no. 1，命题 2）；如果$\tau$是$G$的另一个元素，显然对于所有$z \in S^{-1}A$来说$q_z(\tau.z) = (\sigma\tau).z$，因此群$G$在环$S^{-1}A$上运行。

#### 命题 23 {#ac-v-s1-prop-23 .statement tag=04OO}

令A为K-代数，$G$A上算子的局部有限群，S为A在$G$和$S^G$集合$S \cap A''$下稳定的乘法子集。那么$(S^G)^{-1}A$到$S^{-1}A$的典范映射（章II, § 2, no. 1，推论2到命题2）是同构，其中映射$(S^G)^{-1}A^G$到$(S^{-1}A)^G$。

对于所有$s \in S$，令$s, s_1, \ldots, s_q$为$G$下s的轨道的不同元素；如$ss_1 \ldots s_q \in S^G$，第一个断言源自章11、§ 2, no. 3、命题8。将$(S^G)^{-1}A$与$S^{-1}A$进行规范识别，显然$(S^G)^{-1}A^G$的每个元素在$G$下都是不变的。相反，令$a/t$为$(S^G)^{-1}A$的元素，在$G$（$a \in A, t \in S^G$）下不变；如果$a, (1 \leq j \leq m)$是$G$下$a$的轨道的不同元素，则$a_j/t = a/t$对应$1 \leq j \leq m$，因此存在$s \in S^G$使得$s(a_j - a) = 0$对应$1 \leq j \leq m$；在其他字中，sa在$G$下是不变的，并且，作为$a/t = (sa)/(st)$，当然在$a/t \in (S^G)^{-1}A^G$下也是不变的。

#### 推论 {#ac-v-s1-n9-cor-1 .statement tag=04OP}

设A是整环，K是分数的域，$G$是A上的局部有限群运算符。那么$G$对K进行操作，$K^G$是$A^G$的分数的域。

$- \{0\}$ 在 $G$ 下是稳定的。

### 习题 {#ac-v-s1-exercises}

§ 1](exercises/s1/)参见[习题。
