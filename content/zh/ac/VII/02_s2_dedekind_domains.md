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
content_sha256: 60624f4b7f0ae376cae4609338575ca4630cfc522410b33d912f2f7541e5494c
translated_from: content/en/ac/VII/02_s2_dedekind_domains.md
translation_method: google
source_content_sha256: 608c7dd934256b19a42a5a2679369ddf6b2698e699e08b46c35914c9e02a03b8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: cdbe1cbf9c72ef61a22e4f40ec7a0eb470853a49919aeb15c5c663076657e592
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 2. 戴德金域

### 1. dedekind 域的定义

设$A$为整环。显然以下条件是等价的：
(a) $A$ 的非零素数理想中没有两个在包含方面具有可比性；
(b) $A$ 的非零素理想是最大的；
(c) $A$ 的非零素理想高度为 1。

#### 定义 1 {#ac-vii-s2-def-1 .statement tag=050M}

所有非零素理想都最大的 Krull 域称为 Dedekind 域。

Dedekind 域的例
(1) 每个主理想整环都是一个戴德金域。
(2) 令K为$\mathbf{Q}$的有限扩张，A为K中$\mathbf{Z}$的积分闭包。环A是Krull域(§ 1, no. 8，命题12)。令 $\mathfrak{p}$ 为 A 的非零素理想。则 $\mathfrak{p} \cap \mathbf{Z}$ 为非零（章 V, § 2, no. 1、推论至命题 1），因此是 $\mathbf{Z}$ 的极大理想；因此$\mathfrak{p}$是A的最大理想（*loc.cit.*，命题1）。因此，A 是 Dedekind 域。一般来说，A 不是主理想整环 (*代数*, 章 VII, § 1, 习题 12)。
(3) \* 令 V 为仿射代数簇，函数的 A 环正则于V。假设 A 不是域（即 V 没有减少到点）。对于 A 是戴德金域，V 是一条没有奇异点的不可约曲线是充分必要的：因为说 A 是整环相当于说，V 是不可约的；说 A 的每个非零素理想最大等于说，A 是一条曲线；最后，由于A是诺特，所以说它是一个Krull域，说就是它是全闭的，即V是一条正规曲线，或者说它没有奇异的点。 \*
(4) 如果$0 \notin S$，戴德金域A的分数$S^{-1}A$的环是戴德金德域。因为$S^{-1}A$是一个克鲁尔域（§ 1, no. 4，命题6），$S^{-1}A$的每个非零素理想最大为章II, § 2, no. 5，命题11。

### 2. dedekind 域的刻画

#### 定理 1 {#ac-vii-s2-thm-1 .statement tag=050N}

设 A 为整环，K 为分数的域。以下条件是等效的：
(a) A 是 Dedekind 域；
(b) A 是一个 Krull 域，并且对 K 的每一个对 A 为正的非不当估值相当于对 A 的基本估值；
(c) A 是克鲁尔域，A 的每个分数理想 $\mathfrak{J} \neq (0)$ 都是除数；
(d) A 的每个分数理想 $3 \neq (0)$ 都是可逆的；
(e) A 是诺特积分闭域，并且 A 的每个非零素理想都最大；
(f) A 是诺特，并且对于 A 的每个最大理想 m，$A_m$ 要么是域，要么是离散估值环；
(g) A 为诺特，并且对于 A 的每个最大理想 m，$A_m$ 为主理想整环。

我们首先展示（a）和（b）的等价。 推论 2 到定理 3，§ 1, no. 6，立即表明 (a) 蕴涵 (b)。相反，(b) 意味着 (a)，因为对于 $A$ 的每个素理想 $p$，都存在 $K$ 的估价环，它支配$A_p$（章 VI, § 1, no. 2、推论到定理） 2）。

证明的其余部分由证明执行以下含义：

$$
(a) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (f) \Rightarrow (g) \Rightarrow (a).
$$

如果 $A$ 是戴德金域且 $b$ 是非零分数理想，则对于每个最大理想 $p$ ($§ 1$, no. 4, 命题 7) 都有$bA_p = bA_p$，因此$b = 6$ (章) II、$§ 3$、no. 3、推论 3 至定理 1)；因此（a）意味着（c）。

现在我们证明 (c) 蕴涵 (d)。如果(c)成立，映射$a \mapsto \operatorname{div} a$是$I(A)$的双射到$D(A)$（cf.$§ 1$，no. 1）；因为它是同态（$§ 1$，no. 2）并且$D(A)$是群，所以$I(A)$的每个元素都是可逆的。

我们证明 (d) 蕴涵 (e)。如果(d)成立，$A$的每个积分理想$\neq (0)$都是有限生成的（章11，$§ 5$，no. 6，定理4），因此$A$是诺特；因为$I(A)$是群，$D(A)$是群，因此$A$是完全整体封闭的（$§ 1$，no. 2，定理1）。最后，如果$p$是$A$的非零素理想，$m$是$A$包含$p$的极大理想，则环$A_{m}$是主理想整环（章） II、$§ 5$、no. 6、定理 4)；因为 $pA_m$ 是素数且非零，必然 $pA_m = mA_m$ （主理想整环是 Dedekind 域） 从而 $p = m$ (章 11, $§ 2$, no. 5, 命题 11) 并且$p$ 是最大的。

现在我们证明 (e) 蕴涵 (f)。如果$m$是$A$的最大理想且(e)成立，则$A_{m}$是全闭域诺特，其最大理想$mA_m$是(0)，或者是$A_{m}$的唯一非零素理想；因此$A_{m}$是域或$§ 1$、no. 7的命题 11的离散估值环。

(f) 暗示 (g) 的事实是显而易见的。

最后我们证明（g）蕴涵（a）。 As $A$ is 交 of the $A_{m}$, where $m$ runs through 集合 of maximal ideals (章 II, $§ 3$, no. 3, 推论 4 to 定理 1), (g) implies that $A$ is integrally closed and 诺特 and hence that $A$ is a Krull domain ($§ 1$, no. 3, 推论 to 定理 2).另一方面，可以证明 $A$ 的每个非零素理想都是最大的，如证明中的 (d) $\Rightarrow$ (e)。

#### 命题 1 {#ac-vii-s2-prop-1 .statement tag=050O}

*半本地 Dedekind 域为主理想整环。*

令$A$为半局部戴德金域，$K$为分数的域，$p_1, \ldots, p_n$其最大理想以及$v_1, \ldots, v$、相应的基本估值；这些是$A$唯一的基本估值。令$a$为$A$的非零积分理想。由于它是除数，因此存在 ($§ 1$, no. 4, 命题 5) 整数 $q_1, \ldots, q_n$，使得$a$是$x \in K$的集合，使得$v_i(x) \geq q_i$对于$1 \leq i \leq n$。令$x_0$为$K$的元素，使得$v_i(x_0) = q_i$对应于$1 \leq i \leq n$（章VI、$§ 7$、no. 2、推论1至定理1）。那么$a$是$x \in K$的集合，这样$v_i(xx_0^{-1}) \geq 0$就代表$1 \leq i \leq n$。因此$a = Ax_0$。

如果 $A$ 是戴德金域，则可以看出，在定理 1 的证明中，A 的除子的群 D(A) 等同于分数理想 $a \neq (0)$ 的群 I(A)（因为 A 是诺特，每个非零分数理想都是有限生成的）。然后将 A ($§ 1$, no. 2) 的除子类群 C(A) 与 A 的理想 $\neq 0$ 的类的群进行识别（在章 II 中定义， $§ 5$、no. 7）。

### 3. 分解理想化为乘积素理想

设A为戴德金域，I(A) A的非零分数理想的有序乘法群和A的除子的D(A) 群。 将 I(A) 的同构 $a \mapsto \operatorname{div} a$ 推到 D(A) 映射极值除子到 A 的非零素理想 ($§ 1$, no. 6, 定理 3)，因此乘法群 I(A)承认 A 的非零素理想为基集合 ($§ 1$, no. 3, 定理 2)。 在其他字中，*A 的每个非零分数理想 a 都承认形式的唯一分解*：

$$
a = \prod_p p^{n(p)}
$$

其中乘积扩展为 A 的非零素理想，指数 $n(p)$ 为零，除了有限的数之外。此外，当且仅当 $n(p)$ 均为正数时，a 才是积分。 关系 (1) 称为 a 到素数因子* 的 *分解。特别是，如果a是主理想$Ax$，那么，对于所有$p$，$n(p) = v_p(x)$，其中$v_p$表示基本估值相应的至$p$；这是从 $§ 1$、no. 3 的公式 (4) 得出的。让

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

（$§ 1$、no. 2、推论至定理 1）； 公式 (4) 和 (5) 遵循命题 2、$§ 1$、no. 1。

这些结果特别适用于 $\mathbf{Z}$ 在 $\mathbf{Q}$ 的有限扩张中的积分闭包。

如果$A$是主理想整环，上面的结果又给出了代数、章VII, § 1, no. 3的结果。

### 4. dedekind 域的近似值定理

在 Dedekind 域中，有一个“近似定理”，它增强了章 VI, § 7, no. 2 的定理 1 和 § 1, no. 5 的命题 9：

#### 命题 2 {#ac-vii-s2-prop-2 .statement tag=050P}

令$A$为戴德金域，$K$为分数的域和$A$的非零素理想的$P$集合；对于$p \in P$，让$v_p$表示相应的对$A$的基本估值。令$p_1, \ldots, p_q$不同于$P$的元素和$n_1, \ldots, n_q$有理整数以及$x_1, \ldots, x_q$元素$K$。那么存在$x \in K$，使得$1 \leq i \leq q$有$v_{p_i}(x - x_i) \geq n_i$，所有与$p_i$不同的$p \in P$有$v_p(x) \geq 0$。

替换如果需要是$n_i$ 大于整数，则可以假设它们全部为正。我们首先检查$x_i$在$A$中的情况；显然这相当于找到 $x \in A$ 满足同余

$$
x \equiv x_i \pmod{p_i^{n_i}}
$$

$x$ 的存在则由章 II, § 1, no. 2、命题 5 推出。

我们现在讨论一般情况。我们可以写$x_i = s^{-1} y_i$，其中$s, y_i$在$A$中；写$x = s^{-1} y$，就等于找到一个$y \in A$，这样，对于所有与$p_i$不同的$p \in P$，一方面是$v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s)$，另一方面是$v_p(y) \geq v_p(s)$；作为 $v_p(s) = 0$，除了指标 $p$ 的有限数之外，它因此被简化为上述情况； 从而命题。

命题 2 可以解释为稠密性定理。 To be precise, for all $p \in P$, let $\hat{K}_p$ (resp. $\hat{A}_p$) be the completion of $K$ (resp. $A$) with respect to the discrete valuation $v_p$ and consider 乘积 $\prod_{p \in P} \hat{K}_p$; 元素 $x = (x_p)$ of this 乘积 is called a restricted adèle of $A$ if $x_p \in \hat{A}_p$ for all $p \in P$ with the exception of a finite 数 of them.显然，受限广告的集合$A$是子环/$\prod_{p \in P} \hat{K}_p$，即包含乘积环$A, = \prod_{p \in P} \hat{A}_p$。考虑$A$，乘积拓扑，$A,$是完整的； there is on $A$ a unique 拓扑 $\mathscr{T}$ which is compatible with its 加法群结构 and for which 邻域 of 0 in $A$, 形式 a fundamental 系统 $\mathscr{G}$ of 邻域为0。拓扑$\mathscr{T}$与$A$上的环结构兼容； for clearly axiom (AVII) of General 拓扑, 章 111, § 6, no. 3, holds, 拓扑 induced by $\mathscr{T}$ on $A,$ being compatible with 环结构 on $A,$. On the other hand, for all $x \in A$ there exists 有限子集 $J$ of $P$ such that, if we write $J' = P - J, \ K_J \leq \prod_{p \in J} \hat{K}_p, \ A_{J'} = \prod_{p \in J'} \hat{A}_p,$ then x \in K_J \times A_{J'} and, as $\hat{A}_p$ is open in $\hat{K}_p$ for all p, $\mathscr{G}$ is a fundamental $K_J \times A_{J'}$ 上的乘积拓扑为 0 的邻域系统；因为后者与乘积上的环结构兼容，*通用拓扑*、章III、*loc的公理（AV_1）。 cit.* 也被认为成立，这证明了我们的断言。显然，A 是 A 的*开* 子环，因此 A 也是一个*完全*环（*一般拓扑*、章III, § 3, no. 3、命题 4）。

对于所有$x \in K$，令$\Delta(x)$为元素$(x_p) \in \prod_{p \in P} \hat{K}_p$，这样对于所有$p \in P$，$x_p = x$；作为 $x_p \in \hat{A}_p$，除了 p 的值的有限数，$\Delta(x) \in A$；因此，我们定义了同态 $A : K \to A$，如果$P \neq \varnothing$（即如果 A 不是域），则它是*内射*； $\Delta(K)$ 中的元素被称为*主要受限adèles*，显然是$\Delta(A) \subset A$。

#### 命题 3 {#ac-vii-s2-prop-3 .statement tag=050Q}

*环 A, (resp. A ) is identified with the completion of A (resp. K) with respect to 环拓扑 for which a fundamental 系统 of 邻域 & 0 consists & all the integral ideals $\neq (0)$ of A.*

A（或 K）上的拓扑被认为是 Hausdorff，直接的。 Taking account of no. 3, 断言 concerning A, follows from 章 111, § 2, no. 13, 命题 17. This shows therefore that $\Delta(A)$ is dense in A,;类似地，要看到$\Delta(K)$在A中是稠密的，请注意，对于所有$x = (x_i) \in A$，只有$p \in P$的有限数使得$v_p(x_p) < 0$； by § 1, no. 5, 命题 9 there is therefore an $s \in K$ such that $sx_p \in \hat{A}_p$ for all $p \in P$, in other 字 $\Delta(s)x \in A$, and, as 乘法 by $\Delta(s)$ is 同态 from A对其自身来说，只要应用 $\Delta(A)$ 在 A 中是稠密的这一事实就足以推断出 $\Delta(K)$ 在 A 中是稠密的。

当然，我们也可以使用命题 2 证明 $\Delta(K)$ 在 A 中是稠密的。

现在考虑矩阵$U \in \mathbf{M}_n(A)$的乘法群$\mathbf{SL}(n, A)$由……组成使得$\det(U) = 1$；如果给定$\mathbf{M}_n(A) = A^{n^2}$乘积拓扑，则$\mathbf{SL}(n, A)$拓扑上的诱导*与$\mathbf{SL}(n, A)$上的群结构*相容的。只要验证映射$U \mapsto U^{-1}$在$\mathbf{SL}(n, A)$上连续即可；但由于 U 是幺模的，所以已知 (*代数*, 章 III, § 6, no. 5, 公式 (17))，$U^{-1}$ 的元素是 U 的 *次数*，因此是 U 的元素中的多项式，这证明了我们的断言。如果通过A将K与A的子环等同，则群$\mathbf{SL}(n, K)$是$\mathbf{SL}(n, A)$的子群。

#### 命题 4 {#ac-vii-s2-prop-4 .statement tag=050R}

*群$\mathbf{SL}(n, K)$在$\mathbf{SL}(n, A)$中稠密。*

令G为$\mathbf{SL}(n, A)$中$\mathbf{SL}(n, K)$的闭包；因为 K 在 A (命题 3)、G 包含中是稠密的，对于 $i \neq j$ 和 $a \in A$，形式 $I + a . E_{ij}$ 的所有矩阵。对于所有$p \in P$和所有$\lambda \in \hat{K}_p$，令$\lambda(p)$为受限制的adèle$x = (x_q)_{q \in P}$，使得对于$q \neq p$有$x_p = \lambda$和$x_q = 0$；上式表明，对于 $i \neq j$，G 包含矩阵 $I + \lambda(p)E_{ij}$。但我们知道形式 $I + \lambda E_{ij}$ 的矩阵对应 $\lambda \in \hat{K}_p$ 生成群 $\mathbf{SL}(n, \hat{K}_p)$ (*代数*, 章 111)。对于每个矩阵$U \in \mathbf{SL}(n, A)$，令$U_p$表示$\mathbf{SL}(n, \hat{\mathbf{K}}_p)$中$U$的典范像；因此可以看出，对于所有$p \in P$，$G$包含矩阵$U \in \mathbf{SL}(n, A)$，使得$U_q = I$对于所有$q \# p$。由于$G$是群，它也包含所有矩阵$U \in \mathbf{SL}(n, A)$，这样$U_p = I$除了$p \in P$的*有限*数；现在，$A$上的拓扑的定义立即表明这些矩阵中的集合在$\mathbf{SL}(n, A)$中是密集的。

### 5. 克鲁尔秋月定理

#### 引理 1 {#ac-vii-s2-lem-1 .statement tag=050S}

*令 $A$ 为诺特域，其中每个非零素数理想都最大，且 $M$ 有限生成挠元 $A$ 模。那么 $M$ 的长度 $\operatorname{long}_A(M)$ 是无限的。*

由于 $M$ 是挠元模，因此与 $M$ 相关的每个素理想都是 $\neq (0)$，因此是最大的。然后从章 IV, § 2, no. 5、命题 7 得出引理。

#### 引理 2 {#ac-vii-s2-lem-2 .statement tag=050T}

*设$A$为环，$T$为$A$模，$(T_i)$为$T$的子模与并$T$的右有向族。然后$\operatorname{long}_A(T) = \sup_i (\operatorname{long}_A(T_i))$.*

$\operatorname{long}_A(T_i) \leq \operatorname{long}_A(T)$ for all $i$.如果没有整数超过$\operatorname{long}_A(T_i)$，引理是明显的，那么两边都是无限的。否则，令$i_0$为指标，其中$\operatorname{long}_A(T_{i_0})$取其最大的值；那么$T_{i_0} = T$，因为家庭$(T_i)$是有方向的；在这种情况下，从而我们的断言。

#### 注 {#ac-vii-s2-n5-rem-1 .statement tag=050U}

这个证明不假设$A$是可交换的。

#### 引理 3 {#ac-vii-s2-lem-3 .statement tag=050V}

*Let $A$ be 诺特 domain such that every non-zero prime ideal $\& A$ is maximal, $M$ a torsion-free $A$-module of 有限秩 $r$ and a non-zero 元素 of $A$.那么$A/Aa$是有限长度的$A$模，并且：*
$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$
引理 1 shows that $\operatorname{long}_A(A/Aa)$ is finite.我们首先在 $M$ 是“有限生成”的情况下展示（6）。 As $M$ is torsion-free and of 秩 $r$, there exists 子模 $L$ of $M$ which is isomorphic to $A'$ and such that $Q = M/L$ is a finitely generated 挠元 $A$-模块，因此为有限长度 (引理 1)。对于每个整数$n \geq 1$，典范满射$M/a^nM \to Q/a^nQ$的核等于$(L + a^nM)/a^nM$并且同构于$L/(a^nM \cap L)$；作为
$$
a^nL \subset a^nM \cap L,
$$
因此
$$
\operatorname{long}_A(M/a^nM) \leq \\
\operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$
现在，由于 $M$ 无扭转，乘法乘以 $a$ 定义同构

M/aM onto aA/a^2M; similarly for L; 从而，由归纳于n，公式：

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

for all $n > 0$;因为 L 与 A' 同构的，$\text{long}_A(L/aL) = r \text{long}_A(A/Aa)$； 从而 (6) 通过让 $n$ 在 (9) 中趋于无穷大。

我们现在讨论一般情况。令$(M_i)$为M的有限生成的子模族。模$T = M/aM$是子模$T_i = (M_i + aM)/aM = M_i/(M_i \cap aM)$的并。现在，T 同构于 $M_i/aM_i$ 的商，因此

$$
\text{long}_A(T_i) \leq r \text{long}_A(A/Aa)
$$

由我们刚才证明的。 从而

$$
\text{long}_A(T) \leq r \text{long}_A(A/Aa)
$$

by 引理 2.

#### 命题 5（克鲁尔-秋月）{#ac-vii-s2-prop-5 .statement tag=050W}

*Let A be 诺特 domain each of whose non-zeroprime ideals is maximal, K its 域 of 分数, L a finite 扩张 of K and B 子环 of L 包含 A. Then B is 诺特并且 B 的每个非零素理想都是极大的。此外，对于 B 的每个理想 $b \neq (0)$，B/b 都是有限生成A-模。*

Let b be a non-zero ideal of B. We shall show that B/b is A-模 of 有限长度 (hence, *更不必说*, B-模 of 有限长度) and that b is a finitely generated B-模.

b 的非零元素 y 满足形式的方程：

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_1 = 0 \quad (a_i \in A, a_1 \neq 0).
$$

这个方程表明$a_1 \in By \subset b$。 应用引理3到$M = B$，可见$B/a_0B$是有限长度的A-模； so is B/b which is 商模 of it.进一步B-模 b 包含，如子模、$a_0B$是有限生成的；由于$b/a_0B$是有限长度（如子模是$B/a_0B$），因此是有限生成的，b当然是有限生成的B-模。

上式首先表明B是诺特。 On the other hand, if $p$ is a non-zero prime ideal of B, 环 $B/p$ is 整环 and of 有限长度 and hence is 域 (*代数*, 章 VIII, § 6, no. 4, 命题 9)，因此 $p$ 最大。

#### 推出 1 {#ac-vii-s2-prop-5-cor-1 .statement tag=050X}

*对于 A 的每个素理想 p，位于 p 之上的 B 素理想的集合是有限的。*

首先假设$p = (0)$；那么$B$的唯一素理想$q$使得$q \cap A = (0)$是$(0)$； otherwise, writing $S = A - \{0\}, S^{-1}q$ would be a non-zero prime ideal of $S^{-1}B$ (章 11, § 2, no. 5, 命题 11) and $S^{-1}B$ is just 域 of 分数 of $B$, for it is 子环 of $L$ 包含 $K$ (\emph{代数}, 章 V, § 3, no. 2, 命题 3); 从而一个荒谬的结论。 If now $p \neq (0)$, it follows from 命题 5 that $B/pB$ is 有限维向量空间 over 域 $A/p$, hence an \emph{阿廷的} 环 and therefore has only a finite 数 of prime ideals (章IV, § 2, no. 5,命题9)，证明素理想的$B$包含$p$只有有限个数。

#### 推论 2 {#ac-vii-s2-prop-5-cor-2 .statement tag=050Y}

*$L$中$A$的积分闭包是一个Dedekind域。*

这个积分闭包是一个积分闭的诺特域，其所有非零素理想都是极大的；因此应用定理 1 of no. 2 就足够了。

特别是：

#### 推论 3 {#ac-vii-s2-prop-5-cor-3 .statement tag=050Z}

*Dedekind 域在域和分数的有限扩张内的积分闭包是 Dedekind 域。*

#### 命题 6 {#ac-vii-s2-prop-6 .statement tag=0510}

*Let $A$ be a Dedekind domain, $K$ its 域 of 分数, $L$ a finite 扩张 of $K$ and $B$ the integral closure of $A$ in $L$.令 $p$ 为 $A$ 的非零素理想，$v$ 相应的 $K$ 的基本估值和*

$$
Bp = \prod_i p_i^{e(i)}
$$

*理想$Bp$的分解与素理想的乘积一样。然后：*
(a) *位于$p$之上的$B$的素理想是$p_i$，使得$e(i) > 0$；*
(b) *对这些理想$p_i$的$v_i$对$L$相应的的估值，直到等价，是对$L$的估值延伸$v$；*
（三）$[B/p_i : A/p] = f(v_i/v);$
(d)$e_i = e(v_i/v)$（cf.章VI, § 8, no. 1、定义1和2）。

(a) To say that a prime ideal $q$ of $B$ lies above $p$ amounts to 说 that $q \supseteq p$, hence that $q \supseteq Bp$ and that $q$ 包含 one of the $p_i$ such that $e(i) > 0$ （章 11、§ 1, no. 1、命题 1）。
(b) 考虑到 (a)，从 § 1, no. 8、推论到命题 12。
(c) $v$的剩余类域与$A/p$识别，$v_i$的$B/p_i$识别（§ 1, no. 4、推论1至命题6）。

(d) 设$a$（分别$a_i$）为$v$（分别$v_i$）的均匀化器。然后
$$
a B_{p_i} = a A_p B_{p_i} = p A_p B_{p_i} = p B . B_{p_i} = \left( \prod_j p_j^{e(j)} \right) B_{p_i} = \prod_j (p_j B_{p_i})^{e(j)} \\
= (p_i B_{p_i})^{e(i)} = a_i^{e(i)} B_{p_i}
$$
从$p_j B_{p_i} = B_j$开始$j \neq i$； 从而 (d)，自 $e(v_i/v) = v_i(a)$ 起。

### 习题{#ac-vii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
