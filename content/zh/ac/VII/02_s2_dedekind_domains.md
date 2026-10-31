---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 2
section_title: Dedekind domains
lang: zh
source: ac-i-vii
book_pages: 493-502, 556-563
pdf_pages: 0511-0520, 0574-0581
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF DEDEKIND DOMAINS
      page: 493
      pdf_page: 511
    - "no": 2
      title: CHARACTERIZATIONS OF DEDEKIND DOMAINS
      page: 494
      pdf_page: 512
    - "no": 3
      title: DECOMPOSITION OF IDEALS INTO PRODUCTS OF PRIME IDEALS
      page: 496
      pdf_page: 514
    - "no": 4
      title: THE APPROXIMATION THEOREM FOR DEDEKIND DOMAINS
      page: 497
      pdf_page: 515
    - "no": 5
      title: THE KRULL-AKIZUKI THEOREM
      page: 499
      pdf_page: 517
statements: 15
exercises: 22
content_sha256: e0fb89218ed683d4147f100a5d08c56dd890cc4b41337aca00050a1d3abbb5b0
translated_from: content/en/ac/VII/02_s2_dedekind_domains.md
translation_method: google
source_content_sha256: 608c7dd934256b19a42a5a2679369ddf6b2698e699e08b46c35914c9e02a03b8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: cdbe1cbf9c72ef61a22e4f40ec7a0eb470853a49919aeb15c5c663076657e592
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 2. DEDEKIND 域

### 1. DEDEKIND 域的定义

设$A$为整环。显然以下条件是等价的：
(a) $A$ 的非零素数理想中没有两个在包含方面具有可比性；
(b) $A$ 的非零素理想是最大的；
(c) $A$ 的非零素理想高度为 1。

#### 定义 1 {#ac-vii-s2-def-1 .statement tag=050M}

所有非零素理想都最大的 Krull 域称为 Dedekind 域。

Dedekind 域的例
(1) 每个主理想整环都是一个戴德金域。
(2) 令K为$\mathbf{Q}$的有限扩张，A为K中$\mathbf{Z}$的积分闭包。环A是Krull域(§ 1, no. 8，命题12)。令 $\mathfrak{p}$ 为 A 的非零素理想。则 $\mathfrak{p} \cap \mathbf{Z}$ 为非零（章 V, § 2, no. 1，命题 1 的推论），因此是 $\mathbf{Z}$ 的极大理想；因此 $\mathfrak{p}$ 是 A 的最大理想 (*loc.cit.*, 命题 1)。因此，A 是 Dedekind 域。一般来说，A 不是主理想整环 (*代数*, 章 VII, § 1, 习题 12)。
(3) \* 设 V 为仿射代数簇，函数的 A 环在 V 上是正则。假设 A 不是域（即 V 未约化为点）。对于 A 是戴德金域，V 是一条没有奇异点的不可约曲线是充分必要的：因为说 A 是整环等于说，V 是不可约的；说 A 的每个非零素理想最大等于说，A 是一条曲线；最后，由于A是诺特，所以说它是一个Krull域相当于说，它是积分闭的，即V是一条正规曲线，或者说它没有奇异的点。 \*
(4) 如果$0 \notin S$，则戴德金域A的分数$S^{-1}A$的环是戴德金域。因为 $S^{-1}A$ 是一个 Krull 域（§ 1, no. 4，命题 6），$S^{-1}A$ 的每个非零素理想最大为章 II, § 2, no. 5，命题 11。

### 2. DEDEKIND 域的刻画

#### 定理 1 {#ac-vii-s2-thm-1 .statement tag=050N}

设 A 为整环，K 为分数的域。以下条件是等效的：
(a) A 是 Dedekind 域；
(b) A 是一个 Krull 域，并且对 K 的每一个对 A 为正的非不当估值相当于对 A 的基本估值；
(c) A 是克鲁尔域，A 的每个分数理想 $\mathfrak{J} \neq (0)$ 都是除数；
(d) A 的每个分数理想 $3 \neq (0)$ 都是可逆的；
(e) A 是诺特积分闭域，并且 A 的每个非零素理想都极大；
(f) A 是诺特，并且对于 A 的每个最大理想 m，$A_m$ 要么是域，要么是离散估值环；
(g) A 是诺特，并且对于 A 的每个最大理想 m，$A_m$ 是主理想整环。

我们首先展示（a）和（b）的等价。推论 2 到定理 3、§ 1, no. 6，立即表明 (a) 蕴涵 (b)。相反，(b) 意味着 (a)，因为对于 $A$ 的每个素理想 $p$，都存在$K$ 的估价环，它支配$A_p$（章 VI, § 1, no. 2，定理 2 的推论）。

证明的其余部分由证明执行以下含义：

$$
(a) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (f) \Rightarrow (g) \Rightarrow (a).
$$

如果 $A$ 是戴德金域且 $b$ 是非零分数理想，则对于每个最大理想 $p$ ($§ 1$, no. 4, 命题 7) 都有$bA_p = bA_p$，因此$b = 6$ (章 II, $§ 3$、no. 3、推论 3 至定理 1)；因此（a）意味着（c）。

现在我们证明 (c) 蕴涵 (d)。如果(c)成立，映射$a \mapsto \operatorname{div} a$是$I(A)$的双射到$D(A)$（cf.$§ 1$，no. 1）；因为它是同态（$§ 1$，no. 2）并且$D(A)$是群，所以$I(A)$的每个元素都是可逆的。

我们证明 (d) 蕴涵 (e)。如果(d)成立，$A$的每个积分理想$\neq (0)$都是有限生成的（章11，$§ 5$，no. 6，定理4），因此$A$是诺特；因为$I(A)$是群，$D(A)$是群，因此$A$是完全整体封闭的（$§ 1$，no. 2，定理1）。最后，如果$p$是$A$的非零素理想，$m$是$A$包含$p$的极大理想，环$A_{m}$是主理想整环（章II， $§ 5$、no. 6、定理 4)；因为 $pA_m$ 是素数且非零，必然 $pA_m = mA_m$ （主理想整环是戴德金域） 从而 $p = m$ (章 11, $§ 2$, no. 5, 命题 11) 并且$p$ 是最大的。

现在我们证明 (e) 蕴涵 (f)。如果$m$是$A$的最大理想且(e)成立，则$A_{m}$是全闭域诺特，其最大理想$mA_m$是(0)，或者是$A_{m}$的唯一非零素理想；因此$A_{m}$是域或$§ 1$、no. 7的命题 11的离散估值环。

(f) 暗示 (g) 的事实是显而易见的。

最后我们证明（g）蕴涵（a）。由于$A$是$A_{m}$的交，其中$m$贯穿最大理想的集合（章II，$§ 3$，no. 3，推论4到定理1），（g）意味着$A$是积分闭且诺特，因此$A$是克鲁尔域（$§ 1$，no. 3，定理2的推论）。另一方面，可以证明 $A$ 的每个非零素理想都是最大的，如证明中的 (d) $\Rightarrow$ (e)。

#### 命题 1 {#ac-vii-s2-prop-1 .statement tag=050O}

*半本地 Dedekind 域为主理想整环。*

令$A$为半局部戴德金域，$K$为分数的域，$p_1, \ldots, p_n$其最大理想以及$v_1, \ldots, v$、相应的基本估值；这些是$A$唯一的基本估值。令$a$为$A$的非零积分理想。由于它是除数，因此存在 ($§ 1$, no. 4, 命题 5) 整数 $q_1, \ldots, q_n$，使得$a$是$x \in K$的集合，使得$v_i(x) \geq q_i$对于$1 \leq i \leq n$。令 $x_0$ 为 $K$ 的元素，使得 $1 \leq i \leq n$ 为 $v_i(x_0) = q_i$（章 VI，$§ 7$，no. 2，推论 1 至定理 1）。那么$a$是$x \in K$的集合，这样$v_i(xx_0^{-1}) \geq 0$就代表$1 \leq i \leq n$。因此$a = Ax_0$。

如果 $A$ 是 Dedekind 域，则在定理 1 的证明中，可以看出 A 的除子的群 D(A) 与分数理想 $a \neq (0)$ 的群 I(A) 相同（因为 A 是诺特，每个非零分数理想是有限生成的）。然后将 A ($§ 1$, no. 2) 的除子类群 C(A) 与 A 的理想 $\neq 0$ 的类群等同（在章 II、$§ 5$ 中定义， no. 7）。

### 3. 分解理想转化为乘积素理想

设 A 为 Dedekind 域，I(A) A 的非零分数理想的有序乘法群和 A 的除子的 D(A) 群。 I(A) 的同构 $a \mapsto \operatorname{div} a$ 到 D(A) 映射到 A 的非零素理想的极值除子 ($§ 1$, no. 6, 定理 3) 因此乘法群 I(A) 承认 A 的非零素理想 ($§ 1$, no. 3, 定理 2) 的基集合。在其他字中，*A 的每个非零分数理想 a 都承认形式的唯一分解*：

$$
a = \prod_p p^{n(p)}
$$

其中乘积扩展为 A 的非零素理想，指数 $n(p)$ 为零，除了有限的数 。此外，当且仅当 $n(p)$ 均为正数时，a 才是积分。 关系 (1) 称为 a 到素数因子* 的 *分解。特别是，如果a是主要理想$Ax$，那么，对于所有$p$，$n(p) = v_p(x)$，其中$v_p$表示基本估值相应的至$p$；这是从 $§ 1$、no. 3 的公式 (4) 得出的。让

$$
a = \prod_p p^{m(p)}, \quad b = \prod_p p^{n(p)}
$$

是 A 的两个非零分数理想。那么

$$
ab = \prod_p p^{m(p) + n(p)} \tag{2}
$$
$$
a : b = ab^{-1} = \prod_p p^{m(p) - n(p)} \tag{3}
$$
$$
a + b = \prod_p p^{\inf(m(p), n(p))} \tag{4}
$$
$$
a \cap b = \prod_p p^{\sup(m(p), n(p))} \tag{5}
$$

关系 (2) 显而易见；由其得出关系 (3)，由方程得出方程$a : b = ab^{-1}$

$$
\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b
$$

（$§ 1$，no. 2，定理 1 的推论）； 公式 (4) 和 (5) 遵循命题 2、$§ 1$、no. 1。

这些结果特别适用于 $\mathbf{Q}$ 的有限扩张中$\mathbf{Z}$ 的积分闭包。

如果$A$是主理想整环，上面的结果又给出了代数、章VII, § 1, no. 3的结果。

### 4. DEDEKIND 域的近似值定理

在戴德金域中，有一个“近似定理”，它加强了章VI, § 7, no. 2的定理1和§ 1, no. 5的命题9：

#### 命题 2 {#ac-vii-s2-prop-2 .statement tag=050P}

设$A$为戴德金域，$K$为分数的域和$A$的非零素理想$P$集合；对于$p \in P$，让$v_p$表示相应的对$A$的基本估值。令$p_1, \ldots, p_q$不同于$P$的元素和$n_1, \ldots, n_q$有理整数以及$x_1, \ldots, x_q$元素$K$。那么存在$x \in K$，使得$1 \leq i \leq q$有$v_{p_i}(x - x_i) \geq n_i$，所有与$p_i$不同的$p \in P$有$v_p(x) \geq 0$。

替换如果需要是$n_i$大于整数，则可以假设它们全部为正。我们首先检查$x_i$在$A$中的情况；显然这相当于找到 $x \in A$ 满足同余

$$
x \equiv x_i \pmod{p_i^{n_i}}
$$

$x$ 的存在则由章 II, § 1, no. 2、命题 5 推出。

我们现在讨论一般情况。我们可以写$x_i = s^{-1} y_i$，其中$s, y_i$在$A$中；写$x = s^{-1} y$，就等于找到一个$y \in A$，这样，对于所有与$p_i$不同的$p \in P$，一方面是$v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s)$，另一方面是$v_p(y) \geq v_p(s)$；作为 $v_p(s) = 0$，除了指标 $p$ 的有限数之外，它因此被简化为上述情况； 从而命题。

命题 2 可以解释为稠密性定理。 准确地说，对于所有$p \in P$，令$\hat{K}_p$（或$\hat{A}_p$）为$K$（或$A$）对于离散估值$v_p$的完成，并考虑乘积$\prod_{p \in P} \hat{K}_p$；如果$x_p \in \hat{A}_p$对于所有$p \in P$（其中有限的数除外），则此乘积的元素$x = (x_p)$被称为$A$的受限adèle。 显然，受限广告的集合$A$是$\prod_{p \in P} \hat{K}_p$的子环，其中包含乘积环$A, = \prod_{p \in P} \hat{A}_p$。 考虑$A$，乘积拓扑，$A,$是完整的； $A$上有一个独特的拓扑$\mathscr{T}$，与其加法群结构兼容，其中$A$中的邻域为0，形式为邻域的基本系统$\mathscr{G}$ 0。 拓扑 $\mathscr{T}$ 与$A$ 上的环结构兼容；对于一般拓扑、章 111、§ 6, no. 3的明确公理（AVII）成立，由$A,$上的$\mathscr{T}$引发的拓扑与$A,$上的环结构兼容。 另一方面，对于所有$x \in A$，存在$P$的有限子集$J$，这样，如果我们写$J' = P - J, \ K_J \leq \prod_{p \in J} \hat{K}_p, \ A_{J'} = \prod_{p \in J'} \hat{A}_p,$，那么x \in K_J \times A_{J'} 并且，由于对于所有p，$\hat{A}_p$在$\hat{K}_p$中开，$\mathscr{G}$是基本系统 $K_J \times A_{J'}$ 上乘积拓扑的邻域为 0；因为后者与乘积上的环结构兼容，*General 拓扑*、章 III、*loc 的公理 (AV_1)。 cit.* 也被认为成立，这证明了我们的断言。 显然，A 是 A 的*开* 子环，因此 A 也是一个*完整*环（*一般拓扑*、章 III, § 3, no. 3、命题 4）。

对于所有$x \in K$，令$\Delta(x)$为元素$(x_p) \in \prod_{p \in P} \hat{K}_p$，使得$x_p = x$对于所有$p \in P$；作为 $x_p \in \hat{A}_p$，除了 p 的值的有限数，$\Delta(x) \in A$；因此，我们定义了同态 $A : K \to A$，如果 $P \neq \varnothing$ 则它是*内射*（即如果 A 不是域）； $\Delta(K)$ 中的元素被称为*主要受限adèles*，并且显然是$\Delta(A) \subset A$。

#### 命题 3 {#ac-vii-s2-prop-3 .statement tag=050Q}

*环 A（分别 A ）被确定为 A（分别 K）关于环拓扑的完成，其中邻域的基本系统和 0 以及 A 的所有积分理想 $\neq (0)$ 组成。*

在A（或K）上考虑拓扑是Hausdorff，直接的。考虑到 A 的 no. 3、断言，可从章 111、§ 2, no. 13、命题 17 得出。因此，这表明 $\Delta(A)$ 在 A 中是稠密的；类似地，$\Delta(K)$在A中是稠密的，注对于所有$x = (x_i) \in A$来说，只有$p \in P$的有限数使得$v_p(x_p) < 0$；通过§ 1, no. 5，命题 9，因此存在$s \in K$，使得$sx_p \in \hat{A}_p$对于所有$p \in P$，在其他字$\Delta(s)x \in A$，并且，由于乘法通过$\Delta(s)$是同态，从A到自身，它就足够了应用 $\Delta(A)$ 在 A 中稠密的事实，推导出 $\Delta(K)$ 在 A 中稠密。

当然，我们也可以使用命题 2 来证明 $\Delta(K)$ 在 A 中是稠密的。

现在考虑矩阵$U \in \mathbf{M}_n(A)$的乘法群$\mathbf{SL}(n, A)$由……组成使得$\det(U) = 1$；如果给定$\mathbf{M}_n(A) = A^{n^2}$乘积拓扑，则$\mathbf{SL}(n, A)$拓扑上的诱导*与$\mathbf{SL}(n, A)$上的群结构*相容的。只要验证映射$U \mapsto U^{-1}$在$\mathbf{SL}(n, A)$上连续即可；但由于 U 是幺模的，所以已知 (*代数*, 章 III, § 6, no. 5, 公式 (17))，$U^{-1}$ 的元素是 U 的 *次数*，因此是 U 的元素中的多项式，这证明了我们的断言。如果通过A将K与A的子环等同，则群$\mathbf{SL}(n, K)$是$\mathbf{SL}(n, A)$的子群。

#### 命题 4 {#ac-vii-s2-prop-4 .statement tag=050R}

*群$\mathbf{SL}(n, K)$在$\mathbf{SL}(n, A)$中稠密。*

令G为$\mathbf{SL}(n, A)$中$\mathbf{SL}(n, K)$的闭包；因为 K 在 A (命题 3)、G 包含中是稠密的，对于 $i \neq j$ 和 $a \in A$，形式 $I + a . E_{ij}$ 的所有矩阵。对于所有$p \in P$和所有$\lambda \in \hat{K}_p$，令$\lambda(p)$为受限制的adèle$x = (x_q)_{q \in P}$，使得对于$q \neq p$有$x_p = \lambda$和$x_q = 0$；上式表明，对于 $i \neq j$，G 包含矩阵 $I + \lambda(p)E_{ij}$。但我们知道形式 $I + \lambda E_{ij}$ 的矩阵对应 $\lambda \in \hat{K}_p$ 生成群 $\mathbf{SL}(n, \hat{K}_p)$ (*代数*, 章 111)。对于每个矩阵$U \in \mathbf{SL}(n, A)$，令$U_p$表示$\mathbf{SL}(n, \hat{\mathbf{K}}_p)$中$U$的典范像；因此可以看出，对于所有$p \in P$，$G$包含矩阵$U \in \mathbf{SL}(n, A)$，使得$U_q = I$对于所有$q \# p$。由于$G$是群，它也包含所有矩阵$U \in \mathbf{SL}(n, A)$，这样$U_p = I$除了$p \in P$的*有限*数；现在，$A$上的拓扑的定义立即表明这些矩阵中的集合在$\mathbf{SL}(n, A)$中是密集的。

### 5.克鲁尔秋月定理

#### 引理 1 {#ac-vii-s2-lem-1 .statement tag=050S}

*令 $A$ 为诺特域，其中每个非零素数理想都最大，且 $M$ 有限生成挠元 $A$ 模。那么 $M$ 的长度 $\operatorname{long}_A(M)$ 是无限的。*

由于 $M$ 是挠元模，因此与 $M$ 相关的每个素理想都是 $\neq (0)$，因此是最大的。然后从章 IV, § 2, no. 5、命题 7 得出引理。

#### 引理 2 {#ac-vii-s2-lem-2 .statement tag=050T}

*设$A$为环，$T$为$A$模，$(T_i)$为$T$的子模与并$T$的右有向族。然后$\operatorname{long}_A(T) = \sup_i (\operatorname{long}_A(T_i))$.*

$\operatorname{long}_A(T_i) \leq \operatorname{long}_A(T)$ 对于所有$i$。如果没有整数超过$\operatorname{long}_A(T_i)$，引理是明显的，那么两边都是无限的。否则，令$i_0$为指标，其中$\operatorname{long}_A(T_{i_0})$取其最大的值；那么$T_{i_0} = T$，因为家庭$(T_i)$是有方向的；在这种情况下，从而我们的断言。

#### 注 {#ac-vii-s2-n5-rem-1 .statement tag=050U}

这个证明不假设$A$是可交换的。

#### 引理 3 {#ac-vii-s2-lem-3 .statement tag=050V}

*令$A$为诺特域，使得每个非零素数理想$\& A$极大，$M$为有限秩$r$的无扭$A$模，以及$A$的非零元素。那么$A/Aa$是有限长度的$A$模，并且：*
$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$
引理 1 表明 $\operatorname{long}_A(A/Aa)$ 是有限的。我们首先在 $M$ 是“有限生成”的情况下展示（6）。由于 $M$ 是无扭的且具有秩 $r$，因此存在 $M$ 的子模 $L$，它与 $A'$ 同构的，因此 $Q = M/L$ 是有限生成的挠元 $A$-模，因此为有限长度 (引理 1)。对于每个整数$n \geq 1$，典范满射$M/a^nM \to Q/a^nQ$的核等于$(L + a^nM)/a^nM$并且同构于$L/(a^nM \cap L)$；作为
$$
a^nL \subset a^nM \cap L,
$$
因此
$$
\operatorname{long}_A(M/a^nM) \leq \\
\operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$
现在，由于 $M$ 无扭转，乘法乘以 $a$ 定义同构

M/aM 到 aA/a^2M； L 也类似； 从而，由归纳于n，公式：

$$
\text{long}_A(M/a^nM) = n \cdot \text{long}_A(M/aM).
$$
$$
\text{long}_A(L/a^nL) = n \cdot \text{long}_A(L/aL).
$$

考虑到(7)，我们推论：

$$
\text{long}_A(M/aM) \leq \text{long}_A(L/aL) + n^{-1}\text{long}_A(Q)
$$

对于所有$n > 0$；由于 L 与 A' 同构的，$\text{long}_A(L/aL) = r \text{long}_A(A/Aa)$； 从而 (6) 通过让 $n$ 在 (9) 中趋于无穷大。

我们现在讨论一般情况。令$(M_i)$为M的有限生成的子模族。模$T = M/aM$是子模$T_i = (M_i + aM)/aM = M_i/(M_i \cap aM)$的并。现在，T 同构于 $M_i/aM_i$ 的商，因此

$$
\text{long}_A(T_i) \leq r \text{long}_A(A/Aa)
$$

由我们刚才证明的。 从而

$$
\text{long}_A(T) \leq r \text{long}_A(A/Aa)
$$

引理2。

#### 命题 5（克鲁尔-秋月）{#ac-vii-s2-prop-5 .statement tag=050W}

*设 A 为诺特域，每个域的非零素理想都最大，K 为分数的域，L 为 K 的有限扩张，B 为 L 包含 A 的子环。则 B 为诺特，B 的每个非零素理想为最大。此外，对于 B 的每个理想 $b \neq (0)$，B/b 为有限生成A-模。*

设b是B的非零理想。我们将证明B/b是有限长度的A-模（因此，*更不必说*，有限长度的B-模），并且b是有限生成的B-模。

b 的非零元素 y 满足形式的方程：

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_1 = 0 \quad (a_i \in A, a_1 \neq 0).
$$

这个方程表明$a_1 \in By \subset b$。 应用引理3到$M = B$，可见$B/a_0B$是有限长度的A-模； B/b 也是如此，它是商模。进一步B-模 b 包含，如子模、$a_0B$是有限生成的；由于$b/a_0B$是有限长度（如子模是$B/a_0B$），因此是有限生成的，b当然是有限生成的B-模。

上式首先表明B是诺特。另一方面，如果 $p$ 是 B 的非零素理想，环 $B/p$ 是整环和有限长度，因此是域 (*代数*, 章 VIII, § 6, no. 4， 命题 9)，因此 $p$ 极大。

#### 推出 1 {#ac-vii-s2-prop-5-cor-1 .statement tag=050X}

*对于 A 的每个素理想 p，位于 p 之上的 B 素理想的集合是有限的。*

首先假设$p = (0)$；那么$B$的唯一素理想$q$使得$q \cap A = (0)$是$(0)$；否则，写$S = A - \{0\}, S^{-1}q$将是$S^{-1}B$的非零素理想（章11，§ 2, no. 5，命题11），$S^{-1}B$只是$B$的分数的域，因为它是子环 $L$ 包含 $K$ (\emph{代数}, 章 V, § 3, no. 2, 命题 3); 从而一个荒谬的结论。如果现在 $p \neq (0)$，则从命题 5 可以得出，$B/pB$ 是有限维向量空间超过域 $A/p$，因此有 \emph{阿廷的} 环，因此只有有限的数素理想(章IV, § 2, no. 5,命题9)，证明素理想的$B$包含$p$只有有限个数。

#### 推论 2 {#ac-vii-s2-prop-5-cor-2 .statement tag=050Y}

*$L$中$A$的积分闭包是一个Dedekind域。*

这个积分闭包是一个积分闭的诺特域，其所有非零素理想都是极大的；因此，满足no. 2中的应用定理 1即可。

特别是：

#### 推论 3 {#ac-vii-s2-prop-5-cor-3 .statement tag=050Z}

*Dedekind 域在域的分数的有限扩张内的积分闭包是 Dedekind 域。*

#### 命题 6 {#ac-vii-s2-prop-6 .statement tag=0510}

*令$A$为戴德金域，$K$为分数的域，$L$为$K$的有限扩张，$B$为$A$在$L$的积分闭包。令 $p$ 为 $A$ 的非零素理想，$v$ 相应的 $K$ 的基本估值和*

$$
Bp = \prod_i p_i^{e(i)}
$$

*理想$Bp$的分解与素理想的乘积一样。然后：*
(a) *位于$p$之上的$B$的素理想是$p_i$，使得$e(i) > 0$；*
(b) *对这些理想$p_i$的$L$相应的的估值$v_i$，直到等价，是对$L$延伸$v$的估值；*
（三）$[B/p_i : A/p] = f(v_i/v);$
(d)$e_i = e(v_i/v)$（cf.章VI, § 8, no. 1、定义1和2）。

(a) 说$B$的素理想$q$位于$p$之上相当于说即$q \supseteq p$，因此$q \supseteq Bp$和$q$包含是$p_i$之一，使得$e(i) > 0$ （章 11、§ 1, no. 1、命题 1）。
(b) 考虑到(a)，从§ 1, no. 8，推论到命题 12。
(c) $v$的剩余类域与$A/p$相同，$v_i$的$B/p_i$相同（§ 1, no. 4，推论1至命题6）。

(d) 设$a$（分别$a_i$）为$v$（分别$v_i$）的均匀化器。然后
$$
a B_{p_i} = a A_p B_{p_i} = p A_p B_{p_i} = p B . B_{p_i} = \left( \prod_j p_j^{e(j)} \right) B_{p_i} = \prod_j (p_j B_{p_i})^{e(j)} \\
= (p_i B_{p_i})^{e(i)} = a_i^{e(i)} B_{p_i}
$$
从$p_j B_{p_i} = B_j$开始$j \neq i$； 从而 (d)，自 $e(v_i/v) = v_i(a)$ 起。

### 习题{#ac-vii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
