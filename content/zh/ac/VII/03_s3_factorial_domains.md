---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 3
section_title: Factorial domains
lang: zh
source: ac-i-vii
book_pages: 502-512, 563-571
pdf_pages: 0520-0530, 0581-0589
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 2
      title: CHARACTERIZATIONS OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 3
      title: DECOMPOSITION INTO EXTREMAL ELEMENTS
      page: 504
      pdf_page: 522
    - "no": 4
      title: RINGS OF FRACTIONS OF A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 5
      title: POLYNOMIAL RINGS OVER A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 6
      title: FACTORIAL DOMAINS AND ZARISKI RINGS
      page: 506
      pdf_page: 524
    - "no": 7
      title: PRELIMINARIES ON AUTOMORPHISMS OF RINGS OF FORMAL POWER SERIES
      page: 506
      pdf_page: 524
    - "no": 8
      title: THE PREPARATION THEOREM
      page: 507
      pdf_page: 525
    - "no": 9
      title: FACTORIALITY OF RINGS OF FORMAL POWER SERIES
      page: 511
      pdf_page: 529
statements: 19
exercises: 27
content_sha256: 64cddddec3f1420f9a2c5d81d2b6605ab367a7a1a78523473dececede731ae17
translated_from: content/en/ac/VII/03_s3_factorial_domains.md
translation_method: google
source_content_sha256: 7c78792af87db965faba28fa907fb71b383afe818bec0650262706d6b261062c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0943a3d468ed7c6584f2afd3719d6dc31ec621127542bbf1f512c09d23170d19
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 3. 阶乘域

### 1. 阶乘域的定义

#### 定义 1 {#ac-vii-s3-def-1 .statement tag=051N}

所有除数理想均为主要的 Krull 域称为阶乘（或唯一因式分解）域。

在其他字中，除子类（§ 1, no. 2）的群减少为0。

例
(1) 每个主理想整环都是阶乘（并且回想一下，是 Dedekind 域）。相反，每个阶乘 Dedekind 域都是主理想整环 × § 2, no. 2、定理 1 (c)。
(2) 特别地，如果 K 为域，则环 K[X] 和 K[[X]] 是阶乘域（关于推广，请参见下面的定理 2 和命题 8）。
(3) 代数簇的简单点的 \* 局部环是阶乘域。在$\mathbf{C}^n$原点解析的函数细菌的环是阶乘域。 \*

### 2. 刻画阶乘域

给定环$A$，我们需要考虑以下条件：

(M) $A$ 的每个非空积分主理想族都有极大元素。

#### 定理 1 {#ac-vii-s3-thm-1 .statement tag=051O}

令$A$为整环。以下条件是等效的：
(a) $A$ 是阶乘；
(b) $A$的非零分数主理想的有序群是群同构于$\mathbf{Z}$的直和（按乘积阶排序）；
(c) 满足条件(M)​​，且$A$的两个主理想中的交为主理想；
(d) 满足条件 (M)，并且对于$A$的每个极值元素$p$，理想的$Ap$是素数；
(e) $A$ 是一个克鲁尔域，并且每个高度为 1 的素理想都是主理想。

我们将用 A 的分数的 K 域和$\mathscr{P}^*$（或 $\mathscr{P}^*(A)$）表示 A 的非零分数主理想的有序群。证明将由证明执行以下含义：

(a) ⇔ (b) ⇔ (c) ⇔ (d) ⇔ (e)

我们证明 (a) 蕴涵 (b)；如果 A 是阶乘，$\mathscr{P}^*$ 同构于 A 的除子的群，因此同构于群 $\mathbf{Z}$ 的直和 ($§ 1$, no. 3, 定理 2)。

注既然关系“A 的两个积分主理想的交是主理想”，则意味着 A 的元素中的每一个有序对都承认一个 $lcm$，即 $\mathscr{P}^*$ 是格序的群 （代数、章、VI、$§ 1$、no. 9、命题 8）。因此，(b) 蕴含 (c)（甚至与其等价）的事实是从代数、章 VI、$§ 1$、no. 13、定理 2. (c) 蕴涵 (d) 的事实是从代数得出， 章 VI、$§ 1$、no. 13、命题 14（DIV）。

(d) 蕴含 (b) 的事实源自代数、章 VI、$§ 1$、no. 13、定理 2 应用于群 $\mathscr{S}^*$。

我们证明 (b) 蕴涵 (e)。如果 (b) 成立，则 $\mathscr{P}^*$ 中有同构到 $\mathbf{Z}^{(l)}$；让$(v_i(x))_{i \in I}$表示$\mathbf{Z}^{(l)}$相应的到理想$Ax$（$x \in K^*$）的元素。立即可以看出，每个$v_i$都是对K的离散评估，A是$v_i$的环的交，并且对于$x \in K^*$，$v_i(x) = 0$，除了指标$i$的有限数；因此 A 是克鲁尔域。另一方面，令 q 为高度为 1 的 A 的素理想；它包含一个非零元素 a，它必然是不可逆的，因此也是（通过素理想的定义）A的极值元素之一；因为$Ap$是素数且非零、$q = Ap$，这就证明q是主数。

最后我们证明（e）蕴涵（a）。设a是A的除理想。存在高度为1的A的素理想$p_i$使得$\operatorname{div} a = \sum_i n_i \operatorname{div} p_i$其中$n_i \in \mathbf{Z}$。如果 (e) 成立，则 $p_i$ 为形式 $Ap_i$、从而 $\operatorname{div} a = \operatorname{div} \left( \prod_i Ap_i^{n_i} \right)$，因此为 $a = \prod_i Ap_i^{n_i}$，因为 a 是除数。

#### 命题 1 {#ac-vii-s3-prop-1 .statement tag=051P}

*设 A 为克鲁尔域。如果 A 的每个除数理想都是可逆的，那么对于 A 的每个最大理想 m，$A_m$ 都是阶乘。如果还假设 A 的每个除数理想都是有限生成的（特别是如果 A 为诺特），则逆命题为真。*

假设 $A$ 的每个除理想都是可逆的；由于$A_{,,}$是一个克鲁尔域（$§ 1$，no. 4，命题6），$A_{,,}$的每个除数理想$a$是两个主分数理想（$§ 1$，no. 5）的交，推论2到命题9);因此$a = bA_m$，其中$b$是$A$的除数理想（章II，$§ 2$，no. 4）；由于 $b$ 可通过假设可逆，我们从章 II、$§ 5$、no. 6、定理 4 推论出 $a$ 是主数，因此 $A_{,,}$ 是阶乘域（no. 1，定义1）。相反，如果所有$A_{,,}$都是阶乘，并且$c$是$A$的有限生成除数理想，则$cA_m$是$A_{,,}$的除数理想，如下从$§ 1$，no. 5，推论2到命题9， 章II、$§ 2$、no. 4；由假设 $cA_m$ 为主，因此从章 11, $§ 5$, no. 6, 定理 4 可以得出 $c$ 是可逆的。

### 3.分解进入极端元素

设$A$为整环，$K$为分数的域以及$A$的可逆元$U$乘法群。回想一下 (代数, 章 VI, $§ 1$, no. 5)，$K^*/U$ 中的典范同构存在于群 $\mathscr{P}^*$ $A$ 的非零分数主理想上。 定理 1 的条件 (b) 可以翻译如下：

#### 命题 2 {#ac-vii-s3-prop-2 .statement tag=051Q}

*令$A$为整环。对于$A$是阶乘，$A$存在子集$P$是充分必要的，使得每个$a \in A - \{0\}$可以唯一地写在形式$a = u \prod_{p \in P} p^{n(p)}$中，其中$u \in U$和$n(p)$是正整数除了其中有限的数之外，还有零。*

如果$P$满足这个条件，显然它的所有元素都是*极值*，并且$A$的每个极值元素都与$P$的唯一元素相关联。回想一下，$P$被称为$A$的极值元素*的*代表系统（代数，章VII，$§ 1$，no. 3，定义） 2）。

始终假设 $A$ 是阶乘。可知(no. 2,定理1)群$\mathscr{P}^*$是一个格子。因此，我们可以应用代数、章、VI、$§ 1$、第 3 条的结果。 9和13。特别是，$K^*$的每个元素都可以以本质上唯一的方式写成*不可约分数*的形式。 $K^*$ 中的任意两个元素 $a, b$ 都有 g.c.d。和一个 L.C.M.；如果$a = u \prod_{p \in P} p^{n(p)}$并且
$$
b = u' \prod_{p \in P} p^{m(p)}
$$
是$a$的分解和$b$作为极值元素的乘积，则：
$$
\text{(1)} \quad \text{g.c.d.}(a, b) = w \prod_{p \in P} p^{\inf(m(p), n(p))}
$$
$$
\text{(2)} \quad \text{l.c.m.}(a, b) = w' \prod_{p \in P} p^{\sup(m(p), n(p))}
$$

其中$w, w'$在U中。我们特别恢复了代数、章VIII, § 1, no. 3的结果。

对于所有$p \in P$，映射$a \mapsto n(p)$是K上的离散估值$v_p$，其环显然是$A_{A_p}$。从定理 1(e) 可以得出，$v_p$ 只是 A 的基本估值，而理想 $Ap$ ($p \in P$) 只是高度为 1 的 A 的素理想。

### 4. 阶乘域的分数的环

#### 命题 3 {#ac-vii-s3-prop-3 .statement tag=051R}

*设 A 为克鲁尔域，S 为 A 的乘法子集而不是包含 0。*

(i) *如果 A 是阶乘，则 $S^{-1}A$ 是阶乘。*
(ii) *如果 S 由元素 $p_i$ 族生成，且主理想 $Ap_i$ 为素数且 $S^{-1}A$ 为阶乘，则 A 为阶乘。*

这紧接着 no. 1 和 § 1, no. 10、命题 17 中的定义 1。

### 5. 多项式环在阶乘域上

设 A 为阶乘域，K 为分数的域，$f$ 为 $K[X]$ 的非零元素；如果是 g.c.d，则 $K^*$ 的元素 c 将被称为 $f$ 的*内容*。的系数关闭。令 $\nu$ 为对 A 至关重要的 K 的估值，$\bar{\nu}$ 其规范的扩张至 $K[X]$（由 $\bar{\nu}\left(\sum a_i X^i\right) = \inf \nu(a_i)$、cf. 章 VI, § 10, no. 1、命题 2 定义）；然后$\bar{\nu}(f) = \nu(c)$。

#### 引理 1（高斯）{#ac-vii-s3-lem-1 .statement tag=051S}

*令$f, f'$为$K[X]$和c的非零元素，$c'$内容关闭，$f', f'$。那么$cc'$就是$ff'$的内容。*

令d为$ff'$的内容。对于对 A 来说必不可少的 K 的每一个评估$\nu$，让$\bar{\nu}$表示其规范的扩张到$K[X]$。然后
$$
\nu(d) = \bar{\nu}(ff') = \bar{\nu}(f) + \bar{\nu}(f') = \nu(c) + \nu(c') = \nu(cc').
$$
因此$cc'd^{-1}$是A的可逆元。

#### 定理 2 {#ac-vii-s3-thm-2 .statement tag=051T}

*设A为阶乘域，K为分数的域，$(p_\lambda)$代表A的极值元素的系统，$(P_\lambda)$代表元$K[X]$的不可约多项式系统，每个$P_\lambda$以1为内容。然后：*
(i) *A[X] 是阶乘域；*
(ii) *$p_\lambda$和$P_\lambda$的集合是A[X]的极值元素的代表系统。*

令 $f$ 为 $A[X]$ 的非零元素。在环 $K[X]$ $f$ 中可以在形式中唯一分解：
$$
f = a \prod_\lambda P_\lambda^{n(\lambda)} \quad (a \in K^*, n(\lambda) \geq 0).
$$

引理 1 证明$a$ 是一个内容关闭。因此$a \in A$。由于$A$是阶乘，$a$可以在形式中唯一分解：

$$
a = u \prod p_i^{m(i)} \quad (u \text{ invertible in } A,\ m(i) \geqslant 0).
$$

从而分解的存在性和唯一性：

$$
f = u \prod p_i^{m(i)} \bigcap_{\lambda} p_{\lambda}^{n(\lambda)}.
$$

注，这个定理证明$A$的每个元素都承认*相同*分解进入$A$和$A[X]$的极值元素。 g.c.d.因此，元素和$A$ 的家庭在$A$ 和$A[X]$ 中是相同的。

我们还可以用 § 1, no. 10 的应用命题 18 来证明 $A[X]$ *是*阶乘域当且仅当 $A$ 是阶乘域。

#### 推论{#ac-vii-s3-n5-cor-1 .statement tag=051U}

*如果 $A$ 是阶乘域，则域 $A[X_1, \ldots, X_n]$ 也是阶乘。*

在$n$上以归纳争论。

这个推论可以扩展到无限族不定数的情况 (cf. 习题 2)。

### 6.阶乘域和 ZARISKI 环

#### 命题 4 {#ac-vii-s3-prop-4 .statement tag=051V}

*令 $A$ 为 Zariski 环，$\hat{A}$ 为其补全。如果 $\hat{A}$ 是阶乘域，则 $A$ 是阶乘域。*

这是从no. 1、定义 1 和§ 1, no. 10、命题 16 得出的。

#### 推论{#ac-vii-s3-n6-cor-1 .statement tag=051W}

*如果诺特局部环 $A$的补全是阶乘域，则$A$是阶乘域。*

### 7. 正式幂级数自同构环的预备知识

#### 引理 2 {#ac-vii-s3-lem-2 .statement tag=051X}

*令$f(X_1, X_2, \ldots, X_n)$为形式幂级数$\neq 0$，系数为环$E$。存在整数 $u(i) \geqslant 1$ ($1 \leqslant i \leqslant n - 1$) 这样*

$$
f(T^{u(1)}, \ldots, T^{u(n-1)}, T) \neq 0.
$$

假设确定整数$u(i) \geqslant 1$($1 \leqslant i \leqslant k - 1$)使得$f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X_n) \neq 0$。我们将确定整数 $u(k) \geqslant 1$ 这样

$$
f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_n^{u(k)}, X_{k+1}, \ldots, X_n) \neq 0.
$$

然后引理将由归纳证明。

观察级数 $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X)$ 可以被视为$X_k$ 和$X_n$ 中的级数，系数在$E[[X_{k+1}, \ldots, X_{n-1}]]$ 中。因此我们看到，为$n = 2$建立引理就足够了。

因此让
$$
f = \sum_{i,j} e_{ij} X^i Y^j \in E[[X, Y]]
$$
其中$f \neq 0$。令$G \subset \mathbf{N} \times \mathbf{N}$为有序对$(i, j)$的非空集合，使得$e_{ij} \neq 0$。让 $\mathbf{N} \times \mathbf{N}$ 得到字典顺序。令$(c, d)$是$G$中最小的元素。 选择整数$p > d$。在展开中
$$
f(T^p, T) = \sum_{(i, j) \in G} e_{ij} T^{ip + j}
$$
我们寻找次数 $cp + d$ 中的项。如果 $ip + j = cp + d, i \geq c + 1$ 是不可能的，因为这将给出
$$
ip + j \geq (c + 1)p + j \geq (c + 1)p > cp + d;
$$
$i < c$也不可能，因为$(c, d)$是$G$中最小的元素；因此$i = c$，然后$j = d$。因此，$f(T^p, T)$中次数$cp + d$的项是$e_{cd} T^{cp + d}$。从$e_{cd} \neq 0, f(T^p, T) \neq 0$开始。 从而引理。

在环 $E[[X_1, \ldots, X_n]]$ 中，令 $a$ 为没有常数项的形式幂级数的理想。如果$w_1, \ldots, w_n$是$a$的元素，请记住映射$f(X_1, \ldots, X_n) \mapsto f(w_1, \ldots, w_n)$是环$E[[X_1, \ldots, X_n]]$的唯一内同态$s$，这样$s(X_i) = w_i$对于$1 \leq i \leq n$ （章III, § 4, no. 5，命题6）。

We take $w_1 = X_1 + X_n^{u(1)}, \ldots, w_{n-1} = X_{n-1} + X_n^{u(n-1)}, w_n = X_n$, where the $u(i)$ are 整数 $\geq 1$. Let $s'$ be 自同态 of $E[[X_1, \ldots, X_n]]$ which 映射 $X_1$ to $X_1 - X_n^{u(1)}, \ldots, X_{n-1}$ to $X_{n-1} - X_n^{u(n-1)}$ and $X_n$ to $X_n$.那么$s'(s(X_i)) = X_i$对应$1 \leq i \leq n$，因此$s' \circ s$是恒等式自同构； $s \circ s'$ 类似。因此 $s$ 是 *自同构*。

#### 引理 3 {#ac-vii-s3-lem-3 .statement tag=051Y}

*Let $f$ be a non-zero 元素 of $E[[X_1, \ldots, X_n]]$.存在整数$u(i) \geq 1 (1 \leq i \leq n-1)$使得$E$的自同构$s$由*定义
$$
s(X_i) = X_i + X_n^{u(i)} \quad (1 \leq i \leq n-1)
$$
*and $s(X_n) = X_n$, 映射 $f$ to 元素 $g$ such that $g(0, \ldots, 0, X_n) \neq 0$.*

$g(0, \ldots, 0, X_n) = f(X_n^{u(1)}, \ldots, X_n^{u(n-1)}, X_n)$。因此，引理 3 是引理 2 的推论。

### 8.准备定理

在这个没有。 A 将表示*局部* 环，$m$ 其最大理想，$k = A/m$ 其剩余类域。 Suppose that A is *Hausdorff and complete* with the $m$-adic 拓扑.让$B = A[[X]]$； it is 局部环 whose maximal ideal $\mathfrak{n}$ is generated by $m$ and $X$;与 $\mathfrak{A}$-adic 拓扑一起，B 是 Hausdorff 且完整 (章 III, § 2, no. 6，命题 6)。

对于每一个正式幂级数
$$
f = \sum_{i=0}^{\infty} a_i X^i \in B,
$$
我们写
$$
\tilde{f} = \sum_{i=0}^{\infty} \bar{a}_i X^i \in k[[X]],
$$
其中$\bar{a}_i$表示$k$中$a_i$的典范像。 级数 $\tilde{f}$ will be called the *reduced 级数* off; if $\tilde{f} \neq 0$, 阶 of $\tilde{f}$ (that is the least 整数 $s$ such that $a_s \notin m$) will be called the *reduced 阶* off.

#### 命题 5 {#ac-vii-s3-prop-5 .statement tag=051Z}

*令$f \in B$为级数，其减少的级数非零。 Let $s$ denote its reduced 阶 and $M$ the sub-A-module of $B$ with 基 $\{1, X, \ldots, X^{s-1}\}$. Then $B$ is 直和 of $M$ and $f$ is not 除子 of 零 in $B$.*

(a) 我们证明$f \mid B \cap M = (0)$。假设有关系：
$$
\left( \sum_{i=0}^{\infty} b_i X^i \right) f = r_0 + r_1 X + \cdots + r_{s-1} X^{s-1} \qquad (b_i \in A, r_j \in A).
$$
We show that the $b_i$ (and hence the $r_j$) are all 零, which will prove in particular that $f$ is not 除子 of 零 in $B$.由于 $A$ 是 Hausdorff，因此足以证明 $b_i \in m^n$ 对于所有 $i \geq 0$ 和所有 $n \geq 0$。对于$n = 0$来说这是显而易见的。 We shall argue by 双归纳: we shall assume that $b_i \in m^{n-1}$ for all $i$ and $b_i \in m^n$ for $i < k$ and show that this implies that $b_k \in m^n$.为此，我们写出$f = \sum_{i=1}^{\infty} a_i X^i$并比较(3)中$X^{s+k}$的系数；那么：
$$
(b_0 a_{s+k} + \cdots + b_{k-1} a_{s+1}) + b_k a_s + (b_{k+1} a_{s-1} + \cdots + b_{k+s} a_0) = 0.
$$
第一个括号中的项从属于到$m^n$，因为$b_i \in m^n$代表$i < k$；对于第二个中的情况也是如此，因为 $b_i \in m^{n-1}$ 代表所有 $i$，$a_i \in m$ 代表$i \leq s-1$。因此$b_k a_s \in m^n$，并且由于$a_s$是$A$的可逆元，所以$b_k \in m^n$。

(b) 我们证明$f \mid B + M = B$。我们写
$$
g = a_s + a_{s+1} X + a_{s+2} X^2 + \cdots;
$$
它是$B$中的可逆元。然后
$$
f - X^s g = a_0 + a_1 X + \cdots + a_{s-1} X^{s-1};
$$
因此，如果我们写成$fg^{-1} - X^s = (f - X^s g) g^{-1} = -h$，则$h$属于到$m$的系数。然后令$r$为$B$的元素。在$n$上归纳我们B的元素定义序列$(q^{(n)})$：我们取$q^{(0)}$为唯一的级数满足：
$$
r \equiv X^s q^{(0)} \pmod{M};
$$
写 $h = \sum_{i=0}^m h_i X^i$ 和 $q^{(n)} = \sum_{i=0}^\infty q_i^{(n)} X^i$，$q_i^{(n)}$ 定义为：
$$
q_i^{(n)} = \sum_{j=0}^{i+s} h_j q_{i+s-j}^{(n-1)}
$$
从 (6) 可以立即得出：
$$
X^s q^{(n)} \equiv h q^{(n-1)} \pmod{M}.
$$
作为所有$j$的$h_j \in m$，它还可以从（6）通过$n$上的归纳得出，对于所有$i$和所有$n$，$q_i^{(n)} \in m^n$。由于 A 是完整的，因此级数
$$
q^{(0)} + q^{(1)} + \ldots + q^{(n)} + \ldots
$$
收敛于B的元素$q$。由(5)和(7)，
$$
X^s(q^{(0)} + q^{(1)} + \ldots + q^{(n)}) \equiv r + h(q^{(0)} + \ldots + q^{(n-1)}) \pmod{M}.
$$
由于 M 是闭集，在极限 (8) 处给出 $r \equiv (X^s - h)q \pmod{M}$，即
$$
r \in fg^{-1}q + M \subset fB + M.
$$
我们还可以使用章III, § 2的结果来显示关系$B = fB + M$（cf.习题12）。这里遵循的方法的优点是适用于收敛的级数。

#### 推论 {#ac-vii-s3-n8-cor-1 .statement tag=0520}

*根据命题 5 的假设和记号，假设$s \geq 1$，从而$f \in Bm + BX$。然后$B' = A[[T]]$到$B = A[[X]]$的A-同态$h$使得$h(T) = f$(章III, § 2, no. 9,命题11(a))定义在B上一个自由的$B'$-模块结构承认$\{1, X, \ldots, X^{s-1}\}$为基。特别是 $h$ 是单射的。*

让 $B'$-模块 B 被给予 (T)-adic 过滤，它由 $n \geq 0$ 的 $f^n B$ (章 111, § 2, no. 1) 组成。 那么$B/fB$是A-模形式基（命题5）中$X^i$（$0 \leq i \leq s-1$）的环$A = B'/TB'$和像的自由模；而且$f$不是B中零的除子（命题5），$Bf^n/Bf^{n+1}$也是秩s的自由$(B'/TB')$模，因此章111的条件（GR），满足§ 2, no. 8（替换 A by B' 且 M by B）。 另一方面，由于 B' 是 Hausdorff 并且相对于 (T)-adic 过滤是完备的，并且 gr(B) 是由上述有限生成的 gr(B')-模，因此首先可以看出（章 III, § 2, no. 9，推论 1 到命题 12）B 是有限生成的 B' 模。 推论的第一个断言是从章 III, § 2, no. 9、命题 13 得出的。 第二个紧随其后。

#### 定义 2 {#ac-vii-s3-def-2 .statement tag=0521}

*多项式* $F \in \mathbf{A}[X]$ *如果它是形式*则称为可区分多项式*
$$
F = X^s + a_{s-1} X^{s-1} + \cdots + a_0,
$$
*其中*$a_i \in \mathfrak{m}$*对于*$0 \leq i \leq s - 1$。

注两个可区分多项式中的乘积是可区分多项式。

#### 命题 6（准备定理）{#ac-vii-s3-prop-6 .statement tag=0522}

*设*$f \in B$*为级数，其减少的级数不是零，并且*$s$*其减少的阶。 Then there exists a unique ordered pair* $(u, F)$ *such that* $u$ *is an invertible element of* $B$, $F$ *a distinguished polynomial of degree* $s$ *and* $f = uF$.

我们写 $F = X^s + G$，其中 $G = g_0 + \cdots g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$)。 关系$f = uF$相当于$F = u^{-1}f$，即$X^s = u^{-1}f - G$。因此，命题 5 显示$G$ 和$u^{-1}$ 的唯一性，因此也显示$F$ 和$u$。它还表明存在 $v \in B$ 和多项式 $G = g_0 + \cdots + g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$) 使得 $X^s = v - G$；仍然需要证明$v$在$B$中是可逆的，并且$g_i \in \mathfrak{m}$对于所有$i$是可逆的。现在，将$k$中的$g_i$的典范像写成$\bar{g}_i$，将$f, g$的减少的级数写成$\bar{f}, \bar{v}$，
$$
X^s + \bar{g}_0 + \bar{g}_1 X + \cdots + \bar{g}_{s-1} X^{s-1} = \bar{f} \bar{v};
$$
因为$\bar{f}$是阶$s$，$\bar{g}_i = 0$对于所有$i$和$\bar{v}$是阶0，因此$v$是可逆的。

#### 命题 7 {#ac-vii-s3-prop-7 .statement tag=0523}

*让*$F$*成为一个杰出的多项式，并且*$g, h$**$B$*的两个形式幂级数*使得*$F = gh$。 *则存在* $B$ *的可逆元* $u$ *使得* $ug$ *和* $u^{-1}h$ *是可区分的多项式和* $F = (ug)(u^{-1}h)$。

事实上，$g$和$h$减少的级数是$\neq 0$；因此，到命题 6，存在$B$的可逆元$u, v$，使得$ug$和$vh$是可区分的多项式。那么 $uvF = (ug)(vh)$ 是可区分多项式，$uv$ 是可逆的。 经过到缩小的级数，立即可以看出$F$和$uvF$具有相同的缩小的阶，即相同的次数。因此，命题 6 中的唯一性断言显示$F = uvF$、从而 $uv = 1$。

#### 推论{#ac-vii-s3-n8-cor-2 .statement tag=0524}

*进一步假设*$\mathbf{A}$*是整环并且*$F$*次数*$s$的可分辨多项式。 *对于* $F$ *在* $\mathbf{A}[X]$ 中为极值，*它在* $B = \mathbf{A}[[X]]$ 中为极值是必要且充分的。

假设$F$在$\mathbf{A}[X]$中不是极值，则$F = f_1 f_2$，其中$f_1$和$f_2$是$\mathbf{A}[X]$的不可逆元素； $f_1$和$f_2$的主系数乘积等于1，这些系数在$\mathbf{A}$和假设中可逆，意味着$f_1$和$f_2$分别为次数、$> 0$和$< s$；由于约化多项式 $\bar{f}_1, \bar{f}_2$ 满足 $\bar{f}_1 \bar{f}_2 = X^s$，$\bar{f}_1$ 和 $\bar{f}_2$ 都不能在 $k[[X]]$ 中可逆，因为，如果 $\bar{f}_1$ 可逆，$\bar{f}_2$ 将是阶 $s$，这是荒谬的。 *更不必说*，$f_1$和$f_2$在$B$中都不可逆，并且$F$在$B$中不是极值。

相反，如果 F 在 $A[[X]]$ 中不是极值，则 $F = gh$，其中 g 及其在 B 中的可逆都不是；因此，他们减少的阶为 $\geq 1$；则命题 7 的可区分多项式$ug$和$u^{-1}h$不是常数，这表明F在$A[X]$中不是极值。

### 9. 形式幂级数环的阶乘

#### 命题 8 {#ac-vii-s3-prop-8 .statement tag=0525}

令C为环，即域或离散估值环。那么形式幂级数 $C[[X_1, \ldots, X_n]]$ 的定义域是阶乘。

令$p$为C和$p$的$x$生成元（如果C是域，则$\pi = 0$）。让 C 被赋予 $p$-adic 拓扑，即 Hausdorff。由于C是诺特局部环，$B = C[[X_1, \ldots, X_n]]$是诺特局部环，其完成度是$\hat{C}[[X_1, \ldots, X_n]]$（章III, §2, no. 6，命题6）。由命题 4 (no. 6)的推论，足以证明$\hat{C}[[X_1, \ldots, X_n]]$是阶乘。现在，如果C是域，那么$\hat{C} = C$；如果C是离散估值环，则$\hat{C}$也是如此（章VI, §5, no. 3，命题5）。因此，我们假设在证明的剩余部分中 C 是完整的。

从平凡的情况$n = 0$开始，通过归纳进行论证，我们假设已经证明了$A = C[[X_1, \ldots, X_{n-1}]]$是阶乘。我们将认同 B 与$A[[X_n]]$ 并用m 表示A 的最大理想（由$\pi, X_1, \ldots, X_{n-1}$ 生成）。我们将证明 B 的每个非零元素 g 以本质上唯一的方式是极值元素的乘积。

设K为域$C/C\pi$；由于$B/B\pi$与$K[[X_1, \ldots, X_n]]$相同，理想的$Bx$是素数，$x$是极值。如果$x \neq 0$，$B_{B\pi}$因此是规范离散估值w的环（章VI, §3, no. 6，命题9）；因此，B 的每个非零元素 g 可以写为 $g = \pi^{w(g)} f$，其中 $f \in B$ 且 f 不是 $\pi$ 的倍数。因此，只要证明 $f$ 是极值元素本质上唯一的乘积就足够了。现在$K[[X_1, \ldots, X_n]]$中$f$的典范像不是零； 引理 3 (no. 7)因此表明B存在自同构，其中映射$f$到元素$f'$，使得$f'(0, \ldots, 0, X_n)$的系数不全部在$Cx$中；这意味着级数$f'$的系数（被视为$X_n$中的正式幂级数）并不全部以m为单位。足以证明我们的断言适合$f'$。

接下来，B 的所有元素将被视为 $X_n$ 中的形式幂级数，其系数在 A 中。通过 no. 8 的命题 6 （从 C 开始适用，因此 A 是可分离且完整的，并且减少的级数 off' 为$\neq 0$），$f'$在B中与一个唯一的可区分多项式F相关联。通过no. 8的命题7，每个级数其中除$f'$（或者，相当于相同的除F）与一个可区分多项式相关联， 除 F 和每个分解 off' 是在可逆因子内，形式 $f' = u F_1 \cdots F_q$，其中 $u$ 是可逆的，$F_i$ 是极值可区分多项式（在 B 中），使得 $F = F_1 \cdots F_q$。根据 no. 8 命题 7 的推论，$F_i$ 在 $\mathbf{A}[X_n]$ 中也是极值。现在，由于 $\mathbf{A}$ 是归纳假设的阶乘，$\mathbf{A}[X_n]$ 也是如此（定理 2, no. 5）；因此，由于它们是单调的，$F_i$由$F$唯一确定（最多置换）。这显示了分解 $f' = u F_1 \ldots F_r$ 的唯一性；它的存在源于 $B$ 是诺特，从而完成证明。

注
(1) 存在阶乘环 $\mathbf{A}$，使得环 $\mathbf{A}[[X]]$ 不是阶乘 (习题 8)。但是，如果 $\mathbf{A}$ 是主理想整环，则 $\mathbf{A}[[X_1, \ldots, X_n]]$ 是阶乘 (习题 9)。
(2) \* 稍后我们将看到，通过同源方法，每个正则局部环都是阶乘（cf.§ 4, no. 7，推论3到命题16）。这将给出另一个证明，概念上更简单，命题 8。 \*

### 习题{#ac-vii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
