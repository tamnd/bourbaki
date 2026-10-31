---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 1
section_title: Valuation rings
lang: zh
source: ac-i-vii
book_pages: 375-381, 441-444
pdf_pages: 0393-0399, 0459-0462
extraction: ocr
subsections:
    - "no": 1
      title: THE RELATION OF DOMINATION BETWEEN LOCAL RINGS
      page: 375
      pdf_page: 393
    - "no": 2
      title: VALUATION RINGS
      page: 376
      pdf_page: 394
    - "no": 3
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS
      page: 378
      pdf_page: 396
    - "no": 4
      title: EXAMPLES OF VALUATION RINGS
      page: 379
      pdf_page: 397
statements: 15
exercises: 9
content_sha256: 2da6ca54d49d1bd27ff36d5d745dbf3614f86e50699de1a56c5d3f70770b0833
translated_from: content/en/ac/VI/01_s1_valuation_rings.md
translation_method: google
source_content_sha256: 4be9d8f7039b4d494391e430e87dbd619d54a3c9a43b0816d5138e002b649b77
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: ab027268670076c9bc12605639fbdcc18ba582b920731bf2e79bec3c176b4109
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 1. 估值环

### 1. 关系之间的统治局部环

#### 定义 1 {#ac-vi-s1-def-1 .statement tag=04RZ}

令$A$和$B$为两个局部环。如果$A$是$B$和$m(A) = A \cap m(B)$中的子环，则称$B$支配$A$。

#### 命题 1 {#ac-vi-s1-prop-1 .statement tag=04S0}

令$A$和$B$为局部环，使得$A$为$B$的子环。以下条件是等效的：
(a) $m(A) \subset m(B)$；
(b) $B$ 支配 $A$；
(c) $B$ 中$m(A)$ 生成的理想$Bm(A)$ 不等于包含 1。

如果$m(A) \subset m(B)$，$m(B) \cap A$是$A$的理想，它不等于包含1，并且包含是最大理想$m(A)$；因此它等于它并且 (a) 蕴涵 (b)。如果$B$支配$A$，则理想的$Bm(A)$包含在$m(B)$中，因此包含不为1；因此(b)意味着(c)。如果(c)成立，则$Bm(A)$包含在$B$、从而(a)的唯一最大理想$m(B)$中。

注，如果$K$是环，关系“B支配A”是序关系在$K$的本地子环的集合上。

令$A$和$B$为两个局部环，使得$B$支配$A$。 典范嵌入$A \to B$定义，将域$\kappa(A)$的商同构代入$\kappa(B)$的子域；这个同构允许我们认同$\kappa(A)$和子域为$\kappa(B)$。

例
(1) 设$A$为诺特局部环且$\hat{A}$其补全； 局部环 $\hat{A}$ 然后支配 $A$ (章 111, § 3, no. 5, 命题 9)。
(2) 令$B$为整环，$B$的$A$子环，$p'$为$B$和$p = A \cap p'$的素理想。然后$pA_p \subset p'B_{p'}$，这样$B_{p'}$支配$A_p$。

### 2. 估值环

#### 定理 1 {#ac-vi-s1-thm-1 .statement tag=04S1}

*设 K 为 K 的域，V 子环。以下条件是等效的*：
(a) *V 是 K 的局部子环的集合极大元素，这个集合在 A 和 B 之间按关系“B 支配 A”排序。*
(b) *从 V 到 L 存在代数闭域 L 和同态 h，其在 K 到 L 的子环同态集合中最大，按 f 和 g 之间的关系“g 扩张 off”排序。*
(c) *如果$x \in K - V$，则$x^{-1} \in V$。*
(d) *V 的分数的域是 K，V 的主理想集合由包含的关系全序。*
(e) *V 的分数的域是 K，V 的理想集合由包含的关系全序。*

我们将通过证明来展示定理以下含义

$$(a) \Rightarrow (b) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (a).$$

假设(a)成立。那么$V$就是局部环。令$L$为从$V$到$L$的剩余类域$\kappa(V)$和$h$典范同态中的代数闭包。令$V'$为$K$包含$V$和$h'$同态的子环，从$V'$延伸到$L$延伸$h$。如果$p'$是$h'$的核，则$p' \cap V = m(V)$；因此(no. 1,例2)$V'_{p'}$支配$V$，这意味着$V'_{p'} = V$和$V' = V$。因此(b)成立。

假设(b)成立。令$L$为代数闭域且从$V$到$L$为$h$同态；假设从$K$的子环到$L$，$h$在同态的集合中最大；设$p$为$h$中的核。 $h(V - p)$的元素在$L$可逆，$h$可以从$V_p$到$L$扩展到同态（章II, § 2, no. 1，命题1）；因此$V = V_p$，这表明$V$是局部环，并且$p$是它的最大理想。令$x$为$K$的非零元素；我们必须证明元素$x, x^{-1}$属于到$V$中至少有一个，也就是说，凭借$h$的最大特征标，$h$可以扩展到$V[x]$或$V[x^{-1}]$。如果 $x$ 对 $V$ 是整数，则从章 V, § 2, no. 1，推论 4 到定理 1。如果$x$ 不是对 $V$ 的整数，我们将使用以下引理：

#### 引理 1 {#ac-vi-s1-lem-1 .statement tag=04S2}

设$A$为环$B$的子环且$x$元素为$B$不整$A$；则分数$B$的环，(章II, § 5, no. 1)*不归约到O*且存在于$B$的子环$A[1/x]$，最大理想包含$1/x$；此外，如果$\mathfrak{M}$是这些最大理想中的任何一个，则$A$中$\mathfrak{M}$的逆像*是*一个最大理想。

由于 $x$ 不是 $A$ 的积分，因此它不是幂零的，因此$B, \neq 0$；而且$x/1 \notin A[1/x]$，否则就有形式的关系

$$
x/1 = a_0/1 + a_1/x + \cdots + a_n/x^n
$$

对于某些$n \geq 0$（其中$a_i \in A$代表$0 \leq i \leq n$），这相当于

$$
x^{n+h} - a\ x^{n+h-1} - a_1 x^{n+h-2} - \cdots - a_n x^{h-1} = 0
$$

为了一些方便$h \geq 1$；但这样的关系意味着$x$是$A$的积分，与假设相反。因此，最大理想 $A[1/x]$ 包含 $1/x$ 的存在源于$1/x$ 在 $A[1/x]$ 中不可逆 (*代数*, 章 I, § 8, no. 7, 定理 2)。

则令$\mathfrak{M}$为$A[1/x]$包含$1/x$的极大理想；令$\phi : A \to A[1/x]$、$p : A[1/x] \to A[1/x]/\mathfrak{M}$为典范同态；那么

$$
p(A[1/x]) = p(\phi(A))[p(1/x)] = p(\phi(A))
$$

从 $p(1/x) = 0$ 开始；这证明$p(\phi(A))$是域，因此逆像$\phi^{-1}(\mathfrak{M})$是$A$的极大理想。

我们将这个引理与$A = V$和$B = K$一起应用；那么存在$V[x^{-1}]$包含$x^{-1}$的最大理想$\mathfrak{m}$，并且$\mathfrak{m} \cap V$是$V$的最大理想，那么$\mathfrak{m} \cap V = p$，因为$V$是局部的；用$V[x^{-1}]$的$f$典范同态表示到$V[x^{-1}]/\mathfrak{m}$、$f(x^{-1}) = 0$、从而$V/p = f(V) = f(V[x^{-1}])$；作为$h$定义，通过从$V/p$到$L$取商单同态$\bar{h}$，$\bar{h}$*of*是从$V[x^{-1}]$到$L$延伸$h$的同态。因此(c)成立。

现在假设 (c) 成立。显然$K$是$V$的分数的域。令$a$和$b$为$V$的元素，使得$Va \notin Vb$；我们证明$Vb \subset Va$。如果 $b = 0$ 则为真；否则关系$a \notin Vb$通过(c)$a^{-1}b \in V$暗示$b^{-1}a \notin V$、从而，因此$Vb \subset Va$。因此(d)成立。

假设(d)成立。令$a$和$b$为$V$的理想，使得$a \notin b$。存在$a \in a$使得$a \notin b$。对于所有 $b \in b$、$a \notin Vb$、从而 $Va \notin Vb$，因此$Vb \subset Va \subset a$（通过 (c)）和 $b \in a$。然后$b \subset a$，这表明条件(e)*是*满足的。

最后假设(e)成立。由于$V$有一个最大理想，它只有一个，因此是局部环。令$V'$为$K$支配$V$的局部子环，并令$x$为$V'$的非零元素，我们将$x = ab^{-1}$写为$a \in V, b \in V$。其中一个理想$Va, Vb$包含在另一个理想中。 *如果 Va \子集 Vb*，则$x \in V$。 *若 Vb \子集 Va*，则$x^{-1} \in V$；因为理想的$V' m(V)$不会再次$x \in V$包含1（no. 1，命题1），$x^{-1} \notin m(V)$，从而，因为$V$是本地的。 $V'$的每元素因此属于至$V$；我们结论 (a) 成立。

#### 定义 2 {#ac-vi-s1-def-2 .statement tag=04S3}

*在定理 1 的记号中，如果等值条件 (a)、(b)、(c)、(d)、(e) 成立，则$V$ 称为对域 $K$ 的估值环。如果整环是环，则称为环估价，并且域是分数的估价环。*

#### 定理 2 {#ac-vi-s1-thm-2 .statement tag=04S4}

*令$K$为域且从$K$的子环$A$到代数闭域$L$为$h$同态。那么对于$K$和同态$h'$，存在从$V$到$L$的估值环$V$，使得$V$包含于$A$，$h'$ 扩展$h$和${h'}^{-1}(O) = m(V)$。*

设$\mathfrak{S}$为$K$子环同态集合到$L$，按扩张关系排序。这个集合是感性的；因为如果$(h_\alpha)_{\alpha \in I}$是$\mathfrak{S}$和$B$的元素的非空全序族，则定义$h_\alpha$的环，$B_\alpha$形式是$K$的子环的全序族及其因此，并$B$是$K$的子环；因此，从$B$到$L$存在唯一映射$\bar{h}$，其中扩展$h_\alpha$（*集合理论*，章II, § 4, no. 6，命题7），并且立即可见从$B$到$L$，$\bar{h}$是同态。 Zorn 的引理然后表明存在 $\mathfrak{S}$ 中的极大元素 $h'$，其中扩展 $h$。 $h'$的定义环$V$是$K$的环估值（定理1）；如果$p$是$h'$的核，$h'$可以从$V_p$延伸到同态到$L$（章II, § 2, no. 1，命题1），从而 $V_p = V$ 和 $p = m(V)$。

#### 推论{#ac-vi-s1-n2-cor-1 .statement tag=04S5}

*域$K$的每一个局部子环$A$至少由$K$的一个估价环主导。*

从$A$到代数闭包$L$$A/m(A)$，应用定理2到典范同态$h$。

### 3. 元素的积分刻画

#### 定理 3 {#ac-vi-s1-thm-3 .statement tag=04S6}

*设$A$为域$K$中的子环。 The integral closure $A'$ of $A$ in $K$ is the intersection of the valuation rings of $K$ which contain $A$; if $A$ is local, $A'$ is the intersection of the valuation rings of $K$ which dominate $A$.*

设$x$为$A'$的元素，$V$为$K$包含$A$的估值环；由于$x$是$V$的积分，因此存在$V[x]$的素理想$p'$，使得$p' \cap V = m(V)$ (章 V, § 2, no. 1, 定理 1)；显然，局部环$(V[x])_{p'}$支配$V$，因此等于它； 从而 $x \in V$.反之，令 $y$ 为 $K$ 的元素，它不是 $A$ 的整数；则存在 $A[y^{-1}]$ 的最大理想 2.2，其中包含 $y^{-1}$ (no. 2, 引理 1)；还存在环$V$为$K$，它主导$(A[y^{-1}])_m$（no. 2，定理2的推论）； as $y^{-1} \in m(V)$, $y \notin V$.进一步$2.2 \cap A$是$A$的最大理想（no. 2，引理1）；因此，如果$A$是局部的，$2.2 \cap A = m(A)$和$V$支配$A$。

#### 推论 1 {#ac-vi-s1-thm-3-cor-1 .statement tag=04S7}

每个估值环均已整体关闭。

#### 推论 2 {#ac-vi-s1-thm-3-cor-2 .statement tag=04S8}

为了使整环整体封闭，它是分数的域的评估族环的交是必要且充分的。

在诺特环的情况下，推论2可以变得更精确（章VII, § 1, no. 3，推论到定理1）。

#### 推论 3 {#ac-vi-s1-thm-3-cor-3 .statement tag=04S9}

令 K 为域，K 的 K' 扩张，A 为 K 的估值环。K' 中 A 的积分闭包是 K 的估值环 V' 的交，使得 V' $\cap K = A$。

定理 1 (c) 表明，如果 V' 是 K' 的估值环，则 V' $\cap K$ 是 K 的估值环，并且 V' 支配 V' $\cap K$。对于 V' 支配 A，V' $\cap K$ 支配 A 因此等于它是充分必要的。

### 4. 例估值环

(1) 每域是一个估价环。

(2) 如果 V' 是域 K' 的估价环，K 是 K' 的子域，则 V' $\cap K$ 通过 no. 2，定理 1 (c)，是 K 的估价环。

(3) 以下命题提供了众多例的估价环：

#### 命题 2 {#ac-vi-s1-prop-2 .statement tag=04SA}

设A为局部环，其最大理想是主理想Ap。如果$\bigcap_{n=1}^{\infty} Ap^n = (0)$（对于例，如果A是诺特，cf.章III, § 3, no. 2，推论命题5），A的唯一理想是（0）和Ap^n；那么要么 p 是幂零的，要么 A 是估值环。

令 A 通过 Ap^n 进行过滤，并令 v 表示相应的阶函数 (章 III, § 2, no. 2)。作为

$$
\bigcap_{n=1}^{w} Ap^n = (0),
$$

关系$v(x) = +\infty$意味着$x = 0$。设a是A的理想$\neq (0)$和a的元素，此时v取最小值；让我们写 $v(a) = s$ ($s \neq +\infty$)。 Then $a \subset Ap^s$.特别地，存在$u \in A$使得$a = up^s$； as $a \notin Ap^{s+1}$, $u \notin Ap$;因此 u 是可逆的且 $p^s \in A$ $a \subset a$。接下来是$a = Ap^s$，从而我们的第一个断言。还可以看出，A 的每个元素 $a \neq 0$ 都可以写成形式 $a = up^{v(a)}$，其中 u 是可逆的。如果$a' = u'p^{v(a')}$（$u'$可逆）是A的另一个非零元素，则$aa' = uu'p^{v(a)+v(a')}$；因此，如果 p 不是幂零的，则 $aa' \neq 0$ 并且 A 为整环。那么，由于 A 的理想集合是通过包含完全排序的，我们结论认为A是一个估值环（定理I（e））。

对于例，如果$p$是质数数，则局部环$\mathbf{Z}_{(p)}$是估价环。设$B = K[X_1, \ldots, X_n]$为多项式环，且$n$在域$K$上不定；理想的 $BX_1$ 是素数，因为 $B/BX_1$ 同构于 $K[X_2, \ldots, X_n]$；因此$B_{BX_1}$是估值环；它由有理数函数$PQ^{-1}$组成，其中$P$和$Q$是多项式，$Q(0, X_2, \ldots, X_n) \neq 0$。

更一般地，我们将看到，如果 $F$ 是元素的极值

$$
B = K[X_1, \ldots, X_n],
$$

$B_{BF}$ 是估价环 (cf. 章 VII, § 3, no. 5)。 \*

正式幂级数$K[[T]]$的环在域$K$上的一个不确定中是诺特局部整环，其最大理想是主要的；因此，其估值为环。另一方面，两个不定式中形式幂级数的环$K[[T_1, T_2]]$，即诺特局部整环不是估价环，因为元素$T_1, T_2$都不是倍数其他。

#### 命题 3 {#ac-vi-s1-prop-3 .statement tag=04SB}

*设$A$为主理想整环，$K$为分数的域。 $K$ 包含 $A$ 的估值环与 $K$ 不同，是形式 $A_{Ap}$ 的环，其中$p$ 是$A$ 的极值元素。

显然，$A_{Ap}$（$p$极值）是环包含$A$的估值，与$K$（命题2）不同。相反，令$V$为不同于$K$和包含$A$的估值环。如$V \neq K$、$m(V)$包含元素$x \neq 0$；将$x = a/b$写入$a \in A$和$b \in A$，可以看出$A \cap m(V)$包含非零元素$a$。由于 $A \cap m(V)$ 是素数，因此它是形式 $Ap$，其中 $p$ 是 $A$ 中的极值。然后$A_{Ap} \subset V, pA_{Ap} \subset m(V)$，这样$V$支配$A_{Ap}$；因为 $A_{Ap}$ 是环的估值 $K$ (命题 2), $V = A_{Ap}$。

#### 推论 1 {#ac-vi-s1-prop-3-cor-1 .statement tag=04SC}

*域$\mathbf{Q}$且不同于$\mathbf{Q}$的每个估值环都是形式$\mathbf{Z}_{(p)}$，其中$p$是质数数。

每子环$\mathbf{Q}$包含$\mathbf{Z}$。

#### 推论 2 {#ac-vi-s1-prop-3-cor-2 .statement tag=04SD}

*令$K$为域，有理函数的$K(X)$域在$K$和$V$的一个不确定中，$K(X)$包含$K$的估值环并且不同于$K(X)$。若$X \in V$，则存在不可约多项式$P \in K[X]$使得$V = (K[X])_{(P)}$；否则$V$是素理想$X^{-1}K[X^{-1}]$处$K[X^{-1}]$的局部环（在其他字$V$由分数$A/B$组成，其中$A \in K[X]$和$B \in K[X]$，使得$\deg(A) \leq \deg(B)$）。

如果$X \in V$，则从命题得到$K[X] \subset V$和断言 3。如果$X \notin V$，则$X^{-1} \in V$，从而$K[X^{-1}] \subset V$；那么 $V$ 是 $K[X^{-1}]$ 的局部环在素理想 $p$ (命题 3) 处，并且这个理想包含 $X^{-1}$ 因为 $X^{-1}$ 在 V 中不可逆；那么 $p = X^{-1}K[X^{-1}]$ 因为后一个理想是最大的。最后让我们考虑一个有理数函数$A(X)/B(X)$，其中A和B分别是次数$a$和$b$的多项式；然后$A(X) = X^a A'(X^{-1})$和$B(X) = X^b B'(X^{-1})$，其中$A'$和$B'$是多项式，使得$A'(0) \neq 0$和$B'(0) \neq 0$；因此，对于$X^{-1}K[X^{-1}]$处的$K[X^{-1}]$的$A(X)/B(X)$到属于到局部环，$a \leq b$是充分必要的。

### 习题 {#ac-vi-s1-exercises}

请参阅[习题了解§ 1](exercises/s1/)。
