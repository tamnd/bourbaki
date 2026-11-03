---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 3
section_title: Local rings. Passage from the local to the global
lang: zh
source: ac-i-vii
book_pages: 80-94, 136-139
pdf_pages: 0100-0114, 0156-0159
extraction: ocr
subsections:
    - "no": 1
      title: LOCAL RINGS
      page: 80
      pdf_page: 100
    - "no": 2
      title: MODULES OVER A LOCAL RING
      page: 82
      pdf_page: 102
    - "no": 3
      title: PASSAGE FROM THE LOCAL TO THE GLOBAL
      page: 87
      pdf_page: 107
    - "no": 4
      title: LOCALIZATION OF FLATNESS
      page: 91
      pdf_page: 111
    - "no": 5
      title: SEMI-LOCAL RINGS
      page: 92
      pdf_page: 112
statements: 39
exercises: 14
content_sha256: 8673016c74aee5220976145cfc0b042594d7b25616b1c870636a50a85a2a0f65
translated_from: content/en/ac/II/03_s3_local_rings_passage_from_the_local_to.md
translation_method: google
source_content_sha256: 5f8c454a02fa9609498046c6e41e498f87f8eae9c6d223e684879450c3339532
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 2abe3844bdc7e4624bd11affa77a1b252d98479c97be589329f2ef681d2b96cf
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 局部环。从本土走向全球

### 1. 局部环

#### 命题 1 {#ac-ii-s3-prop-1 .statement tag=047R}

令$\mathbf{A}$为$\mathbf{A}$的不可逆元素的环和$I$集合。 集合$I$是$\mathbf{A}$理想中的并，与$\mathbf{A}$不同。此外，以下条件是等价的：
(a) $I$ 是一个理想。
(b) 与$\mathbf{A}$不同的$\mathbf{A}$理想中的集合有最大元素。
(c) $\mathbf{A}$ 有一个独特的最大理想。

关系 $x \in I$ is equivalent to $1 \notin xA$ and hence $xA \neq \mathbf{A}$. If $a$ is an ideal of $\mathbf{A}$ distinct from $\mathbf{A}$ and $x \in a$, then $xA \subset a$, hence $xA \neq \mathbf{A}$ and $x \in I$.因此，与$\mathbf{A}$不同的$\mathbf{A}$的每个理想都包含在$I$中，并且每个元素$x \in I$属于都包含在主理想$xA \neq \mathbf{A}$中。 This proves the first 断言, which immediately implies 等价 of (a), (b) and (c).

注 (1)。请注意，如果 (c) 成立，$I$ 是环 $\mathbf{A}$ (代数, 章 VIII, §6, no. 3, 定义 3) 的 Jacobson 根基。

#### 定义 1 {#ac-ii-s3-def-1 .statement tag=047S}

如果环$\mathbf{A}$满足命题1的等价条件(a)、(b)和(c)，则称为局部环。$\mathbf{A}$的雅各布森根基的商（这是$\mathbf{A}$的唯一极大理想）被称为剩余类域共 $\mathbf{A}$。

#### 定义 2 {#ac-ii-s3-def-2 .statement tag=047T}

令$\mathbf{A}, \mathbf{B}$为两个局部环和$m, n$各自的最大理想。如果 $u(m) \subset n$ 则同态 $u : \mathbf{A} \to \mathbf{B}$ 称为本地。

这等于 $\bar{u}^{-1}(n) = m$ 的说，因为 $\bar{u}^{-1}(n)$ 是理想的包含 $m$，而不是包含 1，因此等于 $m$。取商，然后我们从$\mathbf{A}$的剩余类域到$\mathbf{B}$的$u$单同态$\mathbf{A}/m \to \mathbf{B}/n$规范地推导。

例
(1) 域为局部环。 环减为0就不是局部环。
(2) 设$\mathbf{A}$为局部环，$k$为剩余类域。形式幂级数$B = \mathbf{A}[[X_1, \ldots, X_n]]$的环是局部环，因为$B$的不可逆元素是形式幂级数，其常数项在$\mathbf{A}$中不可逆（代数，章IV, §5, no. 6，命题4）。 $\mathbf{A}$到$B$的典范嵌入是本地同态，剩余类域的相应的单射是同构。
(3) 令$b$为环$\mathbf{A}$的理想，且仅包含在单个最大理想$m$中；那么$A/b$是一个*局部环*，极大理想$m/b$和剩余类域与$A/m$自然同构。这尤其适用于$b = m^k$、$m$是$A$（$§ 1$、no. 1、推论至命题 1）的任何最大理想的情况。如果$A$本身是局部环且最大理想$m$，则对于$A$的每个理想$b \neq A$，$A/b$是局部环，典范同态$A \to A/b$一个局部同态并且相应的同态剩余类域和 *同构*。

(4) 设$X$为$X$的拓扑空间、$x_0$点和$A$环，实值函数连续于邻域的点$x_0$处的细菌$x_0$（*一般拓扑*、章I, § 6, no. 10）。显然，对于连续的函数$f$中$x_0$处的胚芽在$A$中可逆，$f(x_0) \neq 0$是必要且充分的，因为这意味着$x_0$的邻域中的$f(x) \neq 0$。因此，环$A$是局部环，其最大理想$m$是函数细菌的集合，即零*at*$x_0$；将 $A$ 的商、映射 $g \mapsto g(x_0)$ 取到$\mathbf{R}$，可得到 $\mathbf{R}$ 的 *同构* 剩余类域 $A/m$。

#### 命题 2 {#ac-ii-s3-prop-2 .statement tag=047U}

*设$A$为环，且$p$为$A$的素理想。 环 $A$，是本地的；其最大理想是$A$中$p$的典范像生成的理想$pA_p = p_v$；它的剩余类域与 $A/p$ 的分数的域是标准同构的。*

令$S = A - p$和$j : A \to A_v$为典范同态； 假设 $p$ 是素数意味着 $p$ 相对于 $S$ 是饱和的，因此 $j^{-1}(pA_p) = p$ ($§ 2$, no. 4, 命题 10) 并且，由于 $A$ 不满足 $S$ 的理想是包含在$p$，前两个断言是$§ 2$、no. 5、命题 11 (ii)的特例。此外，当且仅当是典范同态$A \to A/p$，$f(S)$是元素$\neq 0$或整环$A/p$的集合，因此最后一个断言是$§ 2$，no. 5的特例， 命题 11（一）。

#### 定义 3 {#ac-ii-s3-def-3 .statement tag=047V}

*设$A$为环，且$p$为$A$的素理想。 环 $A$，在没有歧义的情况下，在$p$处称为$A$的局部环，或$p$的局部环。*

*注 (2).* 如果$A$是局部环且$m$是其最大理想，则$A - m$的元素是可逆的(命题 1)，因此$A_{m'}$规范地等同于$A$ ($§ 2$， no. 1、注5)。

例
(5) 设$p$为素数数。 局部环 $\mathbf{Z}_{(p)}$ 是有理数数 $a/b$ 的集合，其中 $a, b$ 是有理数整数且$b$素数顶； $\mathbf{Z}_{(p)}$的剩余类域与素数域$\mathbf{F}_p = \mathbf{Z}/(p)$同构的。

(6) 令$V$为仿射代数簇，$V$上正则函数的$A$环，$W$为$V$的不可约子簇，$p$为$A$的理想（必然是素数） 函数中的由……组成，每$W$中的点为零。 环$A$，在$V$上称为$W$的局部环。 \*

#### 命题 3 {#ac-ii-s3-prop-3 .statement tag=047W}

设$A$为环，$p$为$A$和$S = A - p$的素理想。对于与$A_p$不同的$A_p$的每个理想$b'$，令$b$为$A$的理想$(i_A^S)^{-1}(b')$，以便$b' = bA_p$。

(i) 设$f$为典范同态$A \to A/b$。从 $A$ 到 $(A/b)_{p/b}$ 与 $f$ ($§ 2$, no. 1, 命题 2) 规范相关的同态是满射的，它的核是 $b'$，其中定义，通过取商、典范同构（共 $A_p/b'$）到$(A/b)_{p/b}$。

(ii) 映射$b' \to b = (i_A^S)^{-1}(b')$，仅限于$A_p$素理想的集合，是同构（关于包含）这个集合到$p$中包含的$A$素理想的集合。如果$b'$在$A_p$中是素数，则环$A_b$存在同构到环$(A_p)_{b'}$，其中映射$a/s$到$(a/1)/(s/1)$对于所有$a \in A, s \in A - b$。

这只是$§ 2$、no. 5、命题 11 的特例。

注
(3) 如果$a$是不包含在$p$中的$A$的理想，则$aA_p = A$和$(A/a)_p = 0$（$§ 2$，no. 5，注）。
(4) 令$A, B$为两个环、$\rho : A \to B$同态、$q$$B$的素理想和$p$$A$的素理想$\rho^{-1}(q)$。由于$\rho(A - p) \subset B - q$、典范同态$\rho_q : A \to B_q$源自$\rho$（$§ 2$、no. 1、命题2），$\rho_q(pA_p) \subset qB_q$是直接的，因此$\rho$是本地同态。

### 2. 模超过局部环

#### 命题 4 {#ac-ii-s3-prop-4 .statement tag=047X}

令$A$为环，它不一定是可交换的，$m$包含在$A$的雅各布森根基中的$A$的右理想，以及$M$左$A$模。假设以下条件之一成立：
(i) $M$ 是有限生成的；
(ii) $m$ 幂零的。
那么关系$(A_d/m) \otimes_A M = 0$就意味着$M = 0$。

断言相对于假设(i)恰好是代数、章VIII、$§ 6$、no. 3中的推论3至命题6。另一方面，关系$(A_d/m) \otimes_A M = 0$等价于$M = mM$，因此对于每个整数$n > 0$意味着$M = m^nM$； 从而断言相对于假设(ii)。

#### 推论 1 {#ac-ii-s3-prop-4-cor-1 .statement tag=047Y}

设$A$是一个不一定可交换的环，$m$包含在$A$、$M$和$N$的雅各布森根中的$A$的右理想，两个左$A$模和$u : M \to N$一个$A$线性映射。 如果 $N$ 是有限生成的或 $m$ 幂零且
$$
1 \otimes u : (A_d/m) \otimes_A M \to (A_d/m) \otimes_A N
$$
是满射，则 $u$ 是满射。

$(A_d/m) \otimes_A (N/u(M))$ 典型地同构于
$$
((A_d/m) \otimes_A N)/\operatorname{Im}(1 \otimes u)
$$

（代数、章II、、no. 6、推论 1 至命题 6）；那么假设意味着$(A_d/m) \otimes_A (N/u(M)) = 0$，因此$N/u(M) = 0$乘以命题 4

#### 推论 2 {#ac-ii-s3-prop-4-cor-2 .statement tag=047Z}

*设$A$为环，它不一定是可交换的，$m$包含在$A$的雅各布森根基中的$A$的双面理想，$M$左$A$模和$(x_i)_{i \in I}$元素的族$M$。如果 $M$ 是有限生成的或 $m$ 幂零且元素 $1 \otimes x_i$ ($i \in I$) 生成左$(A/m)$-模 $(A/m) \otimes_A M$，则 $x_i$ 生成 $M$。*

令$(e_i)_{i \in I}$为左侧$A$-模块$A_s^{(I)}$的典范基：应用推论1到$A$线性映射$u : A_s^{(I)} \to M$就足够了，使得$u(e_i) = x_i$对于所有$i \in I$。

#### 命题 5 {#ac-ii-s3-prop-5 .statement tag=0480}

*令$A$为环，它不一定是可交换的，$m$包含在$A$的雅各布森根基中的$A$的两侧理想，以及$M$左$A$模。 Suppose that one of the following 条件 holds:
(i) $M$ 是有限呈现的；
(ii) $m$ 幂零。
那么，如果$(A/m) \otimes_A M = M/mM$是自由左$(A/m)$模，并且从$m \otimes_A M$到$M$的典范同态是单射的，则$M$是自由$A$模。准确地说，如果$(x_i)_{i \in I}$是$M$的元素族，使得$(1 \otimes x_i)$是$(A/m)$模块$M/mM$的基，则$(x_i)$是$M$的基。*

If $a \in A$, $x \in M$ and $\bar{a}$ is 类 of $a$ in $A/m$, then $\bar{a} \otimes x = 1 \otimes (ax)$ and hence 假设 implies that there exists a family $(x_i)_{i \in I}$ of 元素 of $M$这样$(1 \otimes x_i)$是$(A/m)$-模块$(A/m) \otimes_A M$的基。我们已经知道 $x_i$ 生成 $M$（推出 2 到命题 4）； we shall see that they are linearly independent over $A$. To this end, let us consider the free $A$-module $L = A_s^{(I)}$;令$(e_i)$为其典范基，$u : A_s^{(I)} \to M$为$A$线性映射，使得$u(e_i) = x_i$对于所有$i \in I$； if $R$ is 核 of $u$, we shall prove that $R = 0$.在假设 (i) 下，$(A/m) \otimes_A M$ 是有限生成的 $(A/m)$ 模，因而 $I$ 必然是有限的，$R$ 是由章 I, § 2, no. 8、引理 9 有限生成的 $A$ 模。然后由命题 4 it will be sufficient to prove (under either 假设) that $R = mR$.

设$j$为典范嵌入$R \to L$；那么有一个交换律图表

$$
\begin{array}{ccccc}
m \otimes R & \xrightarrow{1 \otimes j} & m \otimes L & \xrightarrow{1 \otimes u} & m \otimes M \\
\downarrow^a & & \downarrow^c & & \downarrow^c \\
R & \xrightarrow{j} & L & \xrightarrow{u} & M
\end{array}
$$

in Which the two rows are exact, $j$ is injective and $1 \otimes u$ is surjective (章

$$
0 \xrightarrow{d} \mathrm{Coker}(a) \longrightarrow \mathrm{Coker}(b) \xrightarrow{v} \mathrm{Coker}(c)
$$

（章I, § 1, no. 4，命题2）；验证 v 是双射就足够了，因为然后我们推断 Coker(a) = 0，在其他字中 a 是满射，因而 R = mR。现在，Coker(b) = (A/m) \otimes_A L 并且

$$
\mathrm{Coker}(c) = (A/m) \otimes_A M
$$

and by 定义 v(1 \otimes e_i) = 1 \otimes x_i;因为 (1 \otimes e_i) 是 (A/m) \otimes_A L 的基，x_i 的定义表明 v 是双射的。

#### 推出 1 {#ac-ii-s3-prop-5-cor-1 .statement tag=0481}

Let A be a not necessarily 交换环, m the Jacobson 根基 of A and M 左A-模.假设A/m为域，从m \otimes_A M 到M的典范同态是单射的，并且满足命题 5的条件(i)、(ii)之一。对于 M 的元素的族 (y_\lambda) 为 M 的直因子的基，该族 (1 \otimes y_\lambda) 在 M/mM 中自由是充分必要的。

如果条件成立，则可以假设(y_\lambda)是M的元素族(x_i)的子族，使得(1\otimes x_i)是M/mM的基(代数，章II, § 7, no. 1， 定理 2) and 命题 5 then proves that (x_i) is 基 of M.

#### 推出 2 {#ac-ii-s3-prop-5-cor-2 .statement tag=0482}

Let A be a not necessarily 交换环, m the Jacobson 根基 of A and M 左A-模. Suppose that A/m is 域 and that one of the following 条件 holds:
(i) M 是有限呈现的；
(ii) m 是幂零的。
那么下面的属性是等价的：
(a) M 是自由的；
(b) M 是投影；
(c) M 是平的；
(d) 典范同态 m \otimes_A M \to M 是单射的；
(e) Tor_1^A(A/m, M) = 0。

The implications (a) \Rightarrow (b) \Rightarrow (c) \Rightarrow (d) are 直接的. As A/m is 域, (A/m) \otimes_A M is a free (A/m)-module and 命题 5 shows that (d) implies (a).

Finally, we know that Tor_1^A(A, M) = 0 and from 正合序列 0 \to m \to A \to A/m \to 0 we therefore derive 正合序列

$$
0 \to \mathrm{Tor}_1^A(A/m, M) \to m \otimes_A M \to M;
$$

这证明Tor$_1^A(A/m, M)$同构于典范同态$m \otimes_A M \to M$的核； (d)和(e)的从而等价。 \*

可以证明，对于每个环 $A$ 和 Jacobson 根基 $m$，使得 $A/m$ 为域，*每个*射影 $A$ 模都是自由的 (习题 3)。

#### 命题 6 {#ac-ii-s3-prop-6 .statement tag=0483}

*设$A$为环，它不一定是可交换的，$m$为雅各布森根基；假设$A/m$是域。令$M$和$N$是两个有限生成的免费$A$模块和$u: M \to N$同态。以下属性是等效的*：

(a) $u$是$M$的同构到$N$的直因子；
(b) $1 \otimes u: (A/m) \otimes_A M \to (A/m) \otimes_A N$ 是单射的；
(c) $u$ 是单射的，$\operatorname{Coker}(u)$ 是一个自由的 $A$ 模块；
(d) 转置同态 ${}^t u: N^* \to M^*$ 是满射。

我们知道(*代数*, 章 II, § 1, no. 11, 命题 21)，如果$N/u(M)$是自由的，$u(M)$是$N$的直因子，因此(c)蕴涵(a)；相反，(a) 意味着$\operatorname{Coker}(u)$，与$N$中$u(M)$的补集同构，是有限生成的射影$A$模和*更不必说*有限呈现（章I, § 2, no. 8，引理8）；因此，这个模是自由的推论 2 到命题 5 并且 (a) 蕴涵 (c)。另一方面，(a)显然意味着(b)。为了简单起见，我们写为$M' = (A/m) \otimes_A M$，$N' = (A/m) \otimes_A N$；由于$M$和$N$是有限生成的，$(A/m)$模块$M'$和$N'$的对偶${M'}^*$和${N'}^*$被规范地标识为$M^* \otimes_A (A/m)$和$N^* \otimes_A (A/m)$和${}^t(1 \otimes u)$ $({}^t u) \otimes 1$ (*代数*, 章 II, § 5, no. 4, 命题 8);由于 $M'$ 和 $N'$ 是向量空间超过域 $A/m$，假设 $1 \otimes u$ 是单射意味着 ${}^t(1 \otimes u)$ 是满射 (*代数*, 章 11, § 7, no. 5、命题10)； 推论 1 到命题 4 那么表明 ${}^t u$ 是满射的，因此我们证明了 (b) 蕴涵 (d)。最后我们证明（d）蕴涵（a）。假设 ${}^t u$ 是满射；因为$M^*$是免费的，所以从$M^*$到$N^*$存在同态$f$使得$1_{M^*} = {}^t u \circ f$(*代数*,章II, § 1, no. 11,命题21);由于$M$和$N$是自由且有限生成的，因此从$N$到$M$存在同态$g$，使得$f = {}^t g$；因此${}^t 1_M = 1_{M^*} = {}^t u \circ {}^t g = {}^t(g \circ u)$、从而$1_M = g \circ u$；这证明$u$是$M$的同构到子模，也就是$N$的直因子 (*代数*, 章 11, § 1, no. 9, 推论 2 到命题15)。

#### 推论 {#ac-ii-s3-n2-cor-1 .statement tag=0484}

*在命题 6 的假设下，以下属性是等效的*：

(a) $u$ 是 $M$ 中的同构到$N$；
(b) $M$ 和 $N$ 具有相同的秩 (*代数*, 章 II, § 7, no. 2) 并且 $u$ 是满射；
(c) $1 \otimes u: M/mM \to N/mN$ 是双射的。

显然（a）意味着（b）； (b) 暗示 $1 \otimes u$ 是满射的；此外，假设 M 和 N 具有相同的秩意味着向量空间 $(A/m) \otimes_A M$ 和 $(A/m) \otimes_A N$ 超过 $A/m$，因此 $1 \otimes u$ 是双射 (*代数*, 章 II, , no. 4、推论至命题 9) 和 (b) 意味着 (c)。最后，条件(c)通过命题6意味着N是$u(M)$的直和和自由的子模P，$u$是M到$u(M)$的同构；如果$P \neq 0$，则$(A/m) \otimes_A P \# 0$和$1 \otimes u$将不是满射；因此 (c) 意味着 (a)

命题 proved above in this no.通常当 $A$ 是 *局部环* 并且 $m$ 是它的*极大理想*时应用。 推论 2 到命题 5 然后由

#### 命题 7 {#ac-ii-s3-prop-7 .statement tag=0485}

*设$A$为约化局部环，$m$其最大理想，$(p_i)_{i \in I}$$A/p_i$和$M$的分数的$A$、$K_i$域的最小素理想族生成$A$-模块。要使 $M$ 自由，满足以下条件是必要且充分的*

$$(1)\qquad [(A/m) \otimes_A M : (A/m)] = [K, \otimes_A M : K]\qquad \text{for all } i \in I.$$

如果 M 是自由的，显然对于所有 $i \in I$，(1) 的两侧都等于 M 的秩。现在假设满足条件，用(1)两侧的$n$公共的值表示；由推论 2 到命题 4 M 有系统 $n$ 生成元 $x_j$ ($1 \leq j \leq n$)。首先假设 $A$ 是 *整环*，在这种情况下，$p_i = 0$ 对于所有 $i \in I$。 元素 $1 \otimes x_j$ ($1 \leq j \leq n$) 生成向量空间 $K \otimes M$ $A$ 分数 K 的域以上；但到假设时，空间是 K 上的维数 $n$，元素 $1 \otimes x_j$ 与 K 线性无关。因此 (*代数*, 章 II, § 1, no. 13, *注* 1) $x_j$ 与 $A$ 线性无关，因此 M 的形式基。

经过对于一般情况，存在从 $L = A''$ 到 M 的满同态 $v$。考虑交换律图表

$$
\begin{array}{ccc}
L & \xrightarrow{v} & M \\
|u| \downarrow & & \downarrow u' \\
\prod_i ((A/p_i) \otimes L) & \xrightarrow{v'} & \prod_i ((A/p_i) \otimes M)
\end{array}
$$

其中 $u$（分别为 $u'$）为映射 $x \mapsto (\phi_i(x))$（分别为 $y \mapsto (\psi_i(y))$），

$$
\phi_i : L \to (A/p_i) \otimes L
$$

（分别为$\psi_i : M \to (A/p_i) \otimes M$）为典范映射，$v'$为$1_{A/p_i} @ v_e$的乘积。然后$(A/p)/(m/p_i) \otimes_{A/p_i} ((A/p_i) \otimes_A M) = (A/m) \otimes_A M$，并且由于$A/p_i$是本地整环，因此从参数的第一个部分可以得出每个$1_{A/p_i} \otimes v$都是同构；那么$v'$也是如此。另一方面，随着$A$减少，$\bigcap_i p_i = (0)$（$§ 2$，no. 6，命题13），从而$\bigcap_i (p_i L) = 0$，因为$L$是免费的（*代数*，章 II、$§ 3$、no. 7、*注*)；由于$p_i L$是$\phi_i$的核，这表明$u$是单射的。由此可见 $v' \circ u = u' \circ v$ 是单射的，因此 $v$ 是单射的，并且由于 $v$ 是定义的满射，这表明 $M$ 是自由的。

### 3. 从本土走向全球

#### 命题 8 {#ac-ii-s3-prop-8 .statement tag=0486}

*令$A$为环，$m$为$A$的最大理想，$M$为$A$模。如果存在 $A$ 的理想 $a$，使得 $m$ 是 $A$ 包含 $a$ 和 $aM = 0$ 的唯一最大理想，则典范同态 $M \to M$ 是双射的。*

$A/a$则为局部环，最大理想为$m/a$； $M$可以被视为$(A/a)$模块；对于$A/a$中$s$的所有$s \in A - m$典范像是可逆的，因此$M$的位似$x \mapsto sx$是$M$的定义的双射，作为泛函的解问题（$§ 2$，no. 2）； 从而命题。

特别是，如果存在$k \geqslant 0$使得$m^k M = 0$，同态$M \to M_m$是双射（$§ 1$，no. 1，推论到命题1）。

#### 命题 9 {#ac-ii-s3-prop-9 .statement tag=0487}

*令$A$为环，$m$为$A$的最大理想，$M$为$A$模，$k$整数$\geqslant 0$。 典范同态 $M \to M_m/m^k M_m$ 是满射，$M/m^k M$ 的核 $m^k M$ 和定义同构到 $M_m/m^k M_m$。*

由于情况$k = 0$很简单，假设$k \geqslant 1$。从命题 8 可知典范同态 $M/m^k M \to (M/m^k M)_m$ 是双射的。另一方面，$(M/m^k M)_m$在规范上与$M_m/(m^k M)_m$（§ 2, no. 4，定理1）等同，因而$(m^k M)_m = m^k M_m$（§ 2, no. 7，推论到命题18），从而有同构 $M/m^k M$到$M_m/m^k M_m$，其中元素$x \in M$到映射类到$x/1$的类。

#### 推论 {#ac-ii-s3-n3-cor-1 .statement tag=0488}

*令$A$为环、$m_1, m_2, \ldots, m_n$不同的$A$、$M$、$A$模和$k_1, k_2, \ldots, k_n$整数$\geqslant 0$。从$M$到$\prod^n M_m/m_{i_1}^{k_1} M_m$的典范同态是满射，它的核是$\left( \bigcap^n m_{i_1}^{k_1} \right) M$。*

这很容易从命题 9 和 $§ 1$、no. 2、命题 6 得出，$m_{i_1}^{k_1}$ 在对中互质（$§ 1$、no. 2、命题 3）。

*在本编号的其余部分中。 $A$将表示$A$最大理想的环和$\Omega(A)$（或$\Omega$）集合。*

#### 命题 10 {#ac-ii-s3-prop-10 .statement tag=0489}

*A-模* $\bigoplus_{m \in \Omega} \mathbf{A}_m$，*$\mathbf{A}_m$的*直和*其中*$m \in \Omega$，*忠实地平坦*。

每个$\mathbf{A}_m$都是平坦的A-模（§ 2, no. 4，定理1），因而$E = \bigoplus_{m \in \Omega} \mathbf{A}_m$是平坦的（章I, § 2, no. 3，命题2）。此外，对于$A$的每个最大理想$m$，$mA_m$是$\mathbf{A}_m$的唯一最大理想，因而$mA_m \neq A_m$，从而，$mE \neq E$因而$E$忠实平坦（章） I, § 3, no. 1、命题 1 (d))。

#### 定理 1 {#ac-ii-s3-thm-1 .statement tag=048A}

*设* $M, N$ *为两个A-模，$u : M \to N$一个A同态，并且对于所有* $m \in \Omega$，*让* $u_m : M, \to N_m$ *为相应的* $A_m$-*同态* (§ 2, no. 2， 注5)。 *对于* $u$ *是单射（分别是满射、双射、零），对于所有* $m \in \Omega$、$u_m$ *是单射（分别是满射、双射、零）*是必要且充分的。

也就是说，对于所有 $m \in \Omega$，$u_m$ 都是单射（分别是满射、双射、零），相当于说同态 $\bigoplus_m u_m : \bigoplus M, \to \bigoplus N$，具有相同的性质。但是$\bigoplus_m M_m = M \otimes_A E, \bigoplus_m N_m = N \otimes_A E$和$\bigoplus_m u_m = u \otimes 1$，其中$E = \bigoplus_m \mathbf{A}_m$；因为 $E$ 是忠实平坦的 (命题 10)，定理源自章 I, § 3, no. 1、命题 1 (c) 和命题 2。

#### 推论 1 {#ac-ii-s3-thm-1-cor-1 .statement tag=048B}

*令*$M$*为A-模，*$M$*的N个子模*和*$x$*元素*$M$。 *对于*$x \in N$，*对于所有*$m \in R$，*$x$*在*$M$中的*规范图像，*属于*$N$是必要且充分的。

令$\bar{x}$为$M/N$中$x$的类；说$x \in N$意味着A-线性映射$u : a \mapsto a\bar{x}$从$A$到$M/N$是零。现在，$(M/N)_m$ 被标识为 $M_m/N_m$（§ 2, no. 4、定理 1），$u_m : A_m \to M_m/N_m$ 被标识为映射 $A \mapsto \lambda \bar{x}_m$，其中 $\bar{x}_m$ 是类 mod。 $N$、$M$ 中的典范像、$x$。由于关系 $u = 0$ 等价于所有 $m$ 除定理 1 的 $u_m = 0$，因此证明了推论。

#### 推论 2 {#ac-ii-s3-thm-1-cor-2 .statement tag=048C}

*设* $M$ *为A-模，并且对于所有* $m \in \Omega$，*让* $f_m$ *为典范映射* $M \to M_m$。 *同态* $x \mapsto (f_m(x))$ *的* $M$ *到* $\prod_{m \in \Omega} M_m$ *是单射*。

在$N = 0$的情况下应用推论1，可以看出对于所有$m \in \Omega$，关系$x = 0$等价于$f_m(x) = 0$。

#### 推论 3 {#ac-ii-s3-thm-1-cor-3 .statement tag=048D}

(i) *设* $b$ *为* $A$ *和* $a$ *元素的理想* $A$。 *对于*$a \in b$，*对于所有*$m \in \Omega$，*$a$*中*$A_m$*属于到*$bA_m$的*典范像是必要且充分的。

(ii) 特别地，令b和c是A的两个元素。为了使c成为b的倍数，对于A中c的所有$m \in \Omega$、典范像，是b的倍数是充分必要的。

由于 $bA_m = b_m$ (§ 2, no. 7, 推论到命题 18)，(i) 是推论 1 的特例； (ii) 由适用于理想 $Ab$ 的 (i) 得出。

#### 推论 4 {#ac-ii-s3-thm-1-cor-4 .statement tag=048E}

设 A 为整环，K 为分数的域，M 为无扭 A 模，使得 M 被规范地识别为 $K \otimes_A M$ 的子 A 模。然后，对于所有$m \in \Omega$，$M_m$被规范地标识为$K \otimes_A M$和$M = \bigcap_{m \in \Omega} M_m$的子A模块。

由于M用$K \otimes_A M$的子模来标识，所以M用$(K \otimes_A M)_m = K_m \otimes_A M$的子模块来标识（§ 2, no. 4，定理1）；作为 $K_m = K$，我们可以立即看出 $M_m$ 是无扭转的；此外，图表中的交换律

$$
\begin{array}{ccc}
M & \longrightarrow & K \otimes_A M \\
\downarrow & & \uparrow \\
M_m & \longrightarrow & (K \otimes_A M)_m
\end{array}
$$

证明典范映射 $M \to M_m$ 是单射的。 推论然后从推论 1 应用于A-模 $K \otimes_A M$ 及其子模 M。

特别是，对于每个整环 A，

(2)
$$
A = \bigcap_{m \in \Omega} A_m.
$$

#### 推论 5 {#ac-ii-s3-thm-1-cor-5 .statement tag=048F}

设 A 为环。 A-模$A^n$生成元的每个系统和n元素是$A^n$的基。

令$(e_i)_{1 \leq i \leq n}$为$A''$的典范基，$A^n$的生成元$(x_i)_{1 \leq i \leq n}$系统，其中n为元素和$u : A^n \to A''$A-线性映射，使得$u(e_i) = x_i$为$1 \leq i \leq n$。由假设$u$是满射，需要证明$u$是单射。凭借定理 1，这可以立即简化为 A 为局部环的情况；如果$m$是A的最大理想，则$(A/m)^n$中的元素$1 \otimes x_i$($1 \leq i \leq n$)则自由$(A/m)$模$(A/m)^n$的生成元的形式系统； as $A/m$ is 域, this 系统 is 基 of $(A/m)^n$;由于$A^n$是自由A-模，我们从命题5推出$(x_i)$是$A^n$的基。

#### 命题 11 {#ac-ii-s3-prop-11 .statement tag=048G}

设 M 为 A-模，N 有限生成A-模和 $u : M \to N$ 同态。为了使 u 成为满射，对于所有 $m \in S_2$，通过取商为满射，从 $u$ 导出同态 $M/mM \to N/mN$ 是充分必要的。

It follows from 定理 1 that, for $u$ to be surjective, it is necessary and sufficient that $u_m : M_m \to N_m$ be surjective for all $m \in \Omega$.由于$A$是局部环，而$N_m$是有限生成的$A_m$模，因此这相当于说，通过取商获得的同态$u'_m : M_m/mM_m \to N_m/mN_m$是满射的（no. 2，推论） 1 至命题 4)；但$M_m/mM_m$（分别$N_m/mN_m$）与$M/mM$（分别$N/mN$）（命题9）、从而命题相同。

#### 命题 12 {#ac-ii-s3-prop-12 .statement tag=048H}

*设E、F、G为三个A-模和$v : G \to F$、$u : E \to F$同态。假设 E 是有限呈现的。为了存在同态$w : E \to G$，使得$u$因子进入$E \xrightarrow{w} G \xrightarrow{v} F$，对于所有$m \in S_2$，存在同态$w^m : E_m \to G$，使得$u_m : E_m \to F$，是充分必要的， 因子变为 $E \xrightarrow{w^m} G_m \xrightarrow{v_m} F$,*

$w$ 满足的存在性上述叙述等价于以下性质：$u$属于到像映射的P

$$
r = \operatorname{Hom}(1_E, v) : \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F).
$$

现在，$(\operatorname{Hom}_A(E, F))_m$（或$(\operatorname{Hom}_A(E, G))_m$）被规范地标识为$\operatorname{Hom}_{A_m}(E_m, F_m)$（或$\operatorname{Hom}_{A_m}(E_m, G_m)$）（§ 2, no. 7、命题 19 (i)），$(\operatorname{Hom}_A(E, F))_m$中$u$的典范像被标识为$u_m$， $r_m$ 与$\operatorname{Hom}_{A_m}(1_{E_m}, v)$ 和$P_m$ 与像或$r_m$ 进行识别。 命题然后从推论 1 到定理 1 应用于$\operatorname{Hom}_A(E, F)$ 及其子模 P。

#### 推论 1 {#ac-ii-s3-prop-12-cor-1 .statement tag=048I}

*令 M 为 M 的 A-模且 N 子模，使得 M/N 是有限呈现的。为了使 N 成为 M 的直因子，对于所有 $m \in S_2$，N 成为 M 的直因子是必要且充分的。*

说 N 是 M 的直因子意味着 M/N 因子上的恒等式同态进入 $M/N \xrightarrow{w} M \xrightarrow{\phi} M/N$，其中 $\phi$ 是典范同态和 $w$ 同态 (*代数*, 章 II, § 1, no. 9、命题 14)；因为 $(M/N)_m = M_m/N_m$ 和 $\phi_m$ 是典范同态 $M_m \to M_m/N_m$，推论很容易从命题 12 得出。

#### 推论 2 {#ac-ii-s3-prop-12-cor-2 .statement tag=048J}

*设 M 为有限生成的自由A-模，M 的 N 子模为有限生成的自由A-模。为了使 N 成为 M 的直因子，对于所有 $m \in \Omega$，$mN = N \cap (mM)$ 是必要且充分的。*

到定义 M/N 是有限的；另一方面，N 和 M 是有限生成的自由 $A_n$ 模块。为了使 $N$ 成为 $M$ 的直因子，典范映射 $N_m / mN_m \to M_m / mM_m$ 是单射的 (no. 2, 命题 6) 是充分必要的；这与说相同，典范映射$N / mN \to M / mM$必须是单射的（命题9），并且由于其核是$(N \cap mM) / mN$，这证明了推论。

命题 12（或推论 1）将特别适用于当$A$为诺特且$E$（或$M/N$）*有限生成* $A$-模块（章） I, § 2, no. 8、引理 8)。

### 4. 平整度定位

#### 命题 13 {#ac-ii-s3-prop-13 .statement tag=048K}

*令$S$为环$A$的乘法子集和$M$一个$A$模。如果 $M$ 是 jflat（或忠实平坦），则 $S^{-1}M$ 是 ajflat（或忠实平坦）$S^{-1}A$-模块和平坦 $A$-模块。*

作为$S^{-1}M = M \otimes_A S^{-1}A$，第一个断言从章I, § 2, no. 7、推论2到命题8（分别为章I, § 3, no. 3、命题5）；此外，$S^{-1}A$是一个扁平的$A$模（$§ 2$，no. 4，定理1）；因而，如果 $M$ 是一个平面 $A$ 模，那么 $S^{-1}M$ 也是一个平面章 I, § 2, no. 7、推论 3 到命题 8。

#### 注 {#ac-ii-s3-n4-rem-1 .statement tag=048L}

如果 $N$ 是一个 $S^{-1}A$ 模块，则 $S^{-1}N$ 被标识为 $N$，因此这与说等价，即 $N$ 是平面 $S^{-1}A$ 模块或平面 $A$ 模块。

#### 命题 14 {#ac-ii-s3-prop-14 .statement tag=048M}

*令$A$为环，$B$为可交换的$A$代数，$T$为$B$的乘法子集。如果 $N$ 是一个 $B$-模块，并且与 $A$-模块一样平坦，则 $T^{-1}N$ 是一个平坦的 $A$-模块。*

$T^{-1}N = T^{-1}B \otimes_B N$；然后从章I, § 2, no. 7、命题8开始，命题应用$A$替换为$B$，$B$替换为$A$，$E$替换为$T^{-1}B$，$F$替换为$N$。

#### 命题 15 {#ac-ii-s3-prop-15 .statement tag=048N}

*令$A, B$为两个环、$\phi : A \to B$同态和$N$一个$B$模块。以下属性是等效的：
(a) $N$ 是扁平 $A$ 模块。
(b) *对于$B$的每个最大理想$n$，$N_n$是一个平坦的$A$模。*
(c) *对于$B$的每个最大理想$n$，如果我们写成$m = \phi(n)$，$N_n$是一个平坦的$A_m$模。*

对于所有$a \notin m$，$a$诱导的$N_n$的位似是双射的，因此$N_n$规范地等同于（b）和（c）的$(N_n)_m$和等价，由

注继命题 13； (a) 蕴涵 (b) 是命题 14 的特例。 还需要证明 (b) 蕴涵 (a)，也就是说，如果 (b) 成立，对于每个单射 A-模同态 $u : M \to M'$，同态 $v = 1 @ u : N \otimes_A M \to N @^* M'$ 都是单射的。现在，$v$ 也是B-模同态，并且，为了使其成为单射，对于 $B$ (no. 3，定理 1) 的每个最大理想 $n$，$v_n : (N \otimes_A M)_n \to (N \otimes_A M')_n$ 是充分必要的。作为
$$
(N \otimes_A M)_n = B_n \otimes_B (N @_A M) = N_n \otimes_A M,
$$
$v_n$ 只是同态 $1 \otimes u : N_n \otimes_A M \to N_n \otimes_A M'$，它是单射的，因为 $N_n$ 是 A-模与假设的平展。

#### 推论 {#ac-ii-s3-n4-cor-1 .statement tag=048O}

*为了使 A-模 M 平坦（或忠实平坦），对于 A、M 的每个最大理想 m，是平坦（或忠实平坦）A_m 模是必要且充分的。*

条件的必要性由命题 13 得出。相反，如果$M,$ 是$A$ 的每个最大理想$m$ 的平坦$A_m$ 模，则$M$ 是平坦的A-模，因为命题 15 应用于以下情况： $\phi$ 是恒等式。最后，如果$M,$对于所有$m$来说是一个忠实平坦的$A_m$模，那么对于所有$m$（no. 3，命题9）来说，$mM_m = mA_mM_m \neq M,$因此是$mM \neq M$，这证明了$M$是一个忠实平坦的A-模 （章I, § 3, no. 1，命题1（d））。

### 5. 半局部环

#### 命题 16 {#ac-ii-s3-prop-16 .statement tag=048P}

*设A为环。以下属性是等效的：
(a) A 的最大理想集合是有限的；
(b) A 的 Jacobson 根基的商是域的有限数的直接合成。*

假设 A 的根基 $\mathfrak{R}$ 的商是域的有限数的直接合成。那么$A/\mathfrak{R}$仅拥有有限的数理想，而*更不必说*仅拥有有限的数最大理想。由于每个最大理想包含$\mathfrak{R}$（*代数*，章VIII, § 6, no. 2，定义2），A的最大理想是典范同态$A \to A/\mathfrak{R}$下$A/\mathfrak{R}$的最大理想中的逆像；因此它们在数内是有限的。

相反，假设 A 只有有限的数不同的最大理想 $m_1, \ldots, m_n$。 $A/m_i$ 是域，从 § 1, no. 2、命题 5 可以得出典范映射 $A \to \prod_{i=1}^n A/m_i$ 是满射；因为它的核 $\bigcap_{i=1}^n m_i$ 是 Jacobson 根基 $\mathfrak{R}$ (*代数*, 章 VIII, § 6, no. 2, 定义 2)，$A/\mathfrak{R}$ 与 $\prod_{i=1}^n A/m_i$ 同构。

#### 定义 4 {#ac-ii-s3-def-4 .statement tag=048Q}

如果环满足命题 16的等价条件 (a), (b)，则称为半局部。

#### 例 {#ac-ii-s3-n5-exa-1 .statement tag=048R}

每个局部环都是半局部的。半局部环的每个商都是半局部环。每个有限乘积半局部环都是半局部的。

如果A是诺特半局部环，B是A-代数即有限生成A-模，则B是半局部环（章IV, § 2, no. 5，推论3到命题9）。

另一个例，推广局部环$A_{\mathfrak{p}}$的构造，由以下命题提供：

#### 命题 17 {#ac-ii-s3-prop-17 .statement tag=048S}

设 A 为 A 的环和 $\mathfrak{p}_1, \ldots, \mathfrak{p}_n$ 素理想。我们写
$$ S = \bigcap_1^n (A - \mathfrak{p}_i) = A - \bigcup_1^n \mathfrak{p}_i. $$

(a) 环 $S^{-1}A$ 是半局部的；如果$q_1, \ldots, q_r$是$\mathfrak{p}_i$的集合的不同极大元素（关于包含），则$S^{-1}A$的最大理想是$S^{-1}q_j$（$1 \leq j \leq r$），并且这些理想是不同的。

(b) 对于 $1 \leq i \leq n$，环 $A_{\mathfrak{p}_i}$ 与 $(S^{-1}A)_{S^{-1}\mathfrak{p}_i}$ 是典型同构的。

(c) 如果A是整环，则$S^{-1}A = \bigcap_1^n A_{\mathfrak{p}_i}$在A的分数的域中。

(a) 不满足S的A的理想是包含在$\mathfrak{p}_i$的并中的理想，因此包含在$\mathfrak{p}_i$（§ 1, no. 1，命题2）中的至少一个中；因而，$q_j$是不满足S的理想的极大元素或集合；因而，$S^{-1}q_j$是$S^{-1}A$乘§ 2, no. 5、命题11 (ii)的最大理想。

(b) 是§ 2, no. 5、命题 11 (iii) 的特例。

(c) 假设 A 是整环。若$\mathfrak{p}_i \subset \mathfrak{p}_k$，则$A_{\mathfrak{p}_i} \supset A_{\mathfrak{p}_k}$；为了证明（c），我们可以假设没有两个 $\mathfrak{p}_i$ 具有可比性。那么从(a)和no. 3、推论 4 到定理 1 得出$S^{-1}A = \bigcap_1^n (S^{-1}A)_{S^{-1}\mathfrak{p}_i}$； 从而 (c) 凭借 (b)。

如果 A 是整环，$S^{-1}A$ 也是命题 17，则提供半局部环的例，该半局部环不是局部环的直接合成 (cf. 章 III, § 2, no. 13)。

#### 推论 {#ac-ii-s3-n5-cor-1 .statement tag=048T}

设 A 为 A 的整环和 $\mathfrak{p}_1, \ldots, \mathfrak{p}_n$ 素理想，其中没有两个在包含方面具有可比性。若A的分数的域中有$A = \bigcap_1^n A_{\mathfrak{p}_i}$，则A的最大理想为$\mathfrak{p}_1, \ldots, \mathfrak{p}_n$。

设定 $S = \bigcap_{i=1}^n (\mathbf{A} - p_i)$、$S^{-1}\mathbf{A} = \mathbf{A}$ 至命题 17 (c)；因而，对于所有$i$，$S$的元素在$\mathbf{A}$和$S^{-1}p_i = p_i$中是可逆的。然后我们的断言凭借命题17(a)得出。

### 习题{#ac-ii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
