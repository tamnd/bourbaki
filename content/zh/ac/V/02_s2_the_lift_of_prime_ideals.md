---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 2
section_title: The lift of prime ideals
lang: zh
source: ac-i-vii
book_pages: 325-344, 362-369
pdf_pages: 0344-0363, 0381-0388
extraction: ocr
subsections:
    - "no": 1
      title: THE FIRST EXISTENCE THEOREM
      page: 325
      pdf_page: 344
    - "no": 2
      title: DECOMPOSITION GROUP AND INERTIA GROUP
      page: 330
      pdf_page: 349
    - "no": 3
      title: DECOMPOSITION AND INERTIA FOR INTEGRALLY CLOSED DOMAINS
      page: 337
      pdf_page: 356
    - "no": 4
      title: THE SECOND EXISTENCE THEOREM
      page: 343
      pdf_page: 362
statements: 36
exercises: 22
content_sha256: 2c05da9012494b735aa387b0fcae1e086b48546e65e424d4f900da8c006db376
translated_from: content/en/ac/V/02_s2_the_lift_of_prime_ideals.md
translation_method: google
source_content_sha256: 89a50149d078678d4ea98a688a9a6bd071b42b62e0d62c0a7d340a9d004553ca
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 9274221945b8b984a9c8d33027aa6ac65899ce1a5a5e6739678e4c3198fa39ad
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 2. 素理想的提升

### 1. 第一个存在定理

#### 定义 1 {#ac-v-s2-def-1 .statement tag=04PJ}

令$\mathbf{A}, \mathbf{A}'$为两个环和$h : \mathbf{A} \to \mathbf{A}'$环同态。如果$a = \overline{h}^1(a')$，则据说理想的$a' \in A'$高于$\mathbf{A}$的理想$a$。

说$A'$的素理想$p'$位于$\mathbf{A}$的理想$p$之上，因此意味着$p$是与$h$相关的连续映射“$h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$”下的$p'$的像 （章11，§ 4, no. 3）。

注对于存在高于$\mathbf{A}$理想$(0)$的理想$A'$，$h : \mathbf{A} \to \mathbf{A}'$是单射的是必要且充分的。

令$a$为$\mathbf{A}$的理想；通过商同态 $h$ 给出同态 $h_1 : \mathbf{A}/a \to \mathbf{A}'/a'$；说$a'$是位于$a$之上的$A'$的理想，相当于说即$aA' \subset a'$，而$a'/aA'$是位于$(0)$之上的$\mathbf{A}'/aA'$的理想。

#### 引理 1 {#ac-v-s2-lem-1 .statement tag=04PK}

设 $h : \mathbf{A} \to \mathbf{A}'$ 为环同态，$S$ $\mathbf{A}$，$i = i_A^S : \mathbf{A} \to S^{-1}\mathbf{A}$，$i' = i_{A'}^{h(S)} : \mathbf{A}' \to S^{-1}\mathbf{A}' = (h(S))^{-1}\mathbf{A}'$ 典范同态和 $h_1 = S^{-1}h : S^{-1}\mathbf{A} \to S^{-1}\mathbf{A}'$ 的乘法子集，因此存在交换律图表

$$
\begin{array}{ccc}
\mathbf{A} & \xrightarrow{h} & \mathbf{A}' \\
i \downarrow & & i' \downarrow \\
S^{-1}\mathbf{A} & \xrightarrow{h_1} & S^{-1}\mathbf{A}'
\end{array}
$$

令$p$为$\mathbf{A}$的素理想，使得$p \cap S = \varnothing$。那么$a' \mapsto S^{-1}a'$是位于$p$之上的$\mathbf{A}'$理想的集合$\mathscr{F}$的满射映射到位于$S^{-1}p$之上的$S^{-1}\mathbf{A}'$理想的集合$\mathscr{F}_1$并且映射$a'_1 \mapsto i'(a'_1)$是$\mathscr{F}_1$的双射到理想属于到$\mathscr{F}$的集合并且相对于$h(S)$饱和；特别地，$p' \mapsto S^{-1}p'$是位于$p$上方的$\mathbf{A}'$素理想的集合的双射到位于$S^{-1}p$上方的$S^{-1}\mathbf{A}'$素理想的集合。

我们知道$S^{-1}p$是$S^{-1}\mathbf{A}$的素理想，$i_1(S^{-1}p) = p$（章11，§ 2, no. 5，命题11）；如果存在$S^{-1}\mathbf{A}'$的理想$b'$位于$S^{-1}p$之上，则$h(i_1(b')) = i(h_1(b')) = p$；如$S^{-1}i'(b') = b'$（前述），这已经表明$\mathscr{F}$的像位于映射$a' \mapsto S^{-1}a'$包含$\mathscr{F}_1$之下。另一方面，如果$a' \in \mathscr{F}$、$a \in A$和$s \in S$，则有以下等价

$$
h_1(a/s) \in S^{-1}a' \iff h(a)/h(s) \in S^{-1}a'
$$
$\iff$ 存在$t \in S$使得$h(t)h(a) \in a'$
$\iff$ 存在$t \in S$使得$ta \in \mathfrak{p}$
$\iff a/z \in S^{-1}\mathfrak{p}$。

因此$h_1^{-1}(S^{-1}a') = S^{-1}\mathfrak{p}$，完成证明，映射$a' \mapsto S^{-1}a'$下$\mathscr{F}$的像等于$\mathscr{F}_1$；其他断言是从章 11、§ 2, no. 5、命题 11 开始的。

#### 命题 1 {#ac-v-s2-prop-1 .statement tag=04PL}

*令$h : A \to A'$为环同态，使得$A'$是$A$的积分，$\mathfrak{p}'$是$A'$和$\mathfrak{p} = h^{-1}(\mathfrak{p}')$的素理想。为了使$\mathfrak{p}$极大，$\mathfrak{p}'$为最大是必要且充分的。*

让我们写出$B = A/\mathfrak{p}$，$B' = A'/\mathfrak{p}'$，并让$h_1 : B \to B'$是由$h$通过商得出的同态； $B$ 和 $B'$ 是整环，$B'$ 是$B$ 的积分（$§ 1$、no. 1、命题 2）。说 $\mathfrak{p}$（或 $\mathfrak{p}'$）是最大意味着 $B$（或 $B'$）是域。 命题由以下引理得出：

#### 引理 2 {#ac-v-s2-lem-2 .statement tag=04PM}

*令$B$为整环且$B$为$A$子环，使得$B$是$A$的积分。为了使$B$成为域，$A$成为域是充分必要的。*

如果$A$是域，那么，对于$B$中的盟友$\neq 0$，$A[y]$是由假设（$§ 1$，定理1）有限生成的$A$-模块；因为$A[y]$是整环，所以它是域（*代数*，章V, § 2, no. 1，命题1）并且*更不必说*$y$在$B$中可逆，因此$B$是域。相反，假设$B$是域，并让$z \neq 0$进入$A$；由于$z^{-1} \in B$、$z^{-1}$是$A$的积分，其他字存在积分依赖方程

$$
z^{-n} + a_1 z^{-(n-1)} + \ldots + a_n = 0
$$

其中$a_i \in A$；现在这个关系表明

$$
-z^{-1} = a_1 + a_2 z + \ldots + a_n z^{n-1} \in A,
$$

因此$A$肯定是域。

#### 推论 1 {#ac-v-s2-lem-2-cor-1 .statement tag=04PN}

*让$h : A \to A'$环同态使得$A'$是$A$的积分，$\mathfrak{p}$是$A$和$\mathfrak{p}'$的素理想，$a'$位于上面的$A'$的两个理想$\mathfrak{p}$使得$\mathfrak{p}' \subset a'$。如果 $\mathfrak{p}'$ 是素数，则 $a' = \mathfrak{p}'$.*

让我们写$S = A - \mathfrak{p}$；那么 $S^{-1}A'$ 是 $S^{-1}A$ 的积分 ($§ 1$, no. 5, 命题

16)，$S^{-1}p$是$S^{-1}A$的最大理想（章11，§ 2, no. 5，命题11），$S^{-1}a'$和$S^{-1}p'$是位于$S^{-1}p$之上的$S^{-1}A'$的理想(引理1) 和$S^{-1}a' \supseteq S^{-1}p'$。由于 $S^{-1}p'$ 是质数，因此它最大为命题 1，因此为 $S^{-1}p' = S^{-1}a'$；因此$a'$包含在$p'$相对于$h(S)$的饱和度中，等于$p'$（章II, § 2, no. 5，命题11）。

#### 推论 2 {#ac-v-s2-lem-2-cor-2 .statement tag=04PO}

令$A'$为整环、$A$子环或$A'$，使得$A'$是$A$和$f$同态从$A'$到环的积分$B$。如果限制到$A$是单射的，那么$f$是单射的。

如果$a'$关闭核，则假设表示$a' \cap A = (0)$；由于$A'$是整环，可以应用推论1，将$p$和$p'$分别作为$A$的理想（0）和$A'$的理想（0），从而$a' = (0)$。

#### 推论 3 {#ac-v-s2-lem-2-cor-3 .statement tag=04PP}

令$h : A \to A'$为环同态，使得$A'$是$A$和$m$的积分，$A$的最大理想，并假设$A'$中只有有限的数不同的最大理想$m'_j$ ($1 \leq j \leq n$) 位于$m$之上。令$q'_j$为$mA'$相对于$m'_j$的饱和度（章II, § 2, no. 4）。然后：
(i) 在零的环 $A'/q'_j$ 除子中，元素 $m'_j/q'_j$ 并且它们是幂零的 ($1 \leq j \leq n$)。
(ii) $mA' = \bigcap_j q'_j = \prod_j q'_j$。
(iii) 典范同态 $A'/mA' \to \prod_j (A'/q'_j)$ 是双射的。

对于$A'$到包含$mA'$的素理想，其逆像低于$h$包含$m$是必要且充分的，因此它位于$m$之上，因为$m$在$A$；因此，$m'_j$是$A'$包含$mA'$（命题1）的唯一素理想，因此$c' = \bigcap_j m'_j$是$mA'$的根式（章II, § 2, no. 6，推论1到命题） 13）。由$q'_j$、类 mod 的定义。 $A' - m'_j$元素$q'_j$不是$A'/q'_j$中0除子；另一方面，由于$m'_j$是不同的最大理想，对于每个指标$j$，都存在元素$a'_j$属于到$\bigcap_j m'_j$而不是$m'_j$（章II, § 1, no. 1， 命题 4)：那么，对于所有 $x \notin m'_j, a'_j x \in r'$，因此类 mod。 $a'_j x$的$q'_j$是幂零的，并且由于$a'_j$的除子不是0，所以我们结论认为$x$的类是幂零的；另外字$m'_j$是$q'_j$的部首，证明(i)。由此可见，$q'_j$在对中互质（章II, § 1, no. 1，命题3）； (iii) 因此将是 (ii) 的推论，考虑到章 II, § 1, no. 2、命题 5. 为了建立 (ii)，我们注在环 $A'/mA'$ 中，$m'_j/mA'$ 是唯一的最大理想，并且$q'_j/mA'$是(0)相对于$m'_j/mA'$(章11,§ 2, no. 4)的饱和度；因此，我们可能会将注意力集中在案例$mA' = (0)$； (ii) 的断言则从章II, § 3, no. 3，推论2到定理1。

#### 注 (1) {#ac-v-s2-n1-rem-1 .statement tag=04PQ}

如果 $A'$ 是诺特，则从 (i) 和 (ii) 可以得出，$(q'_j)_{1 \leq j \leq n}$ 是 $mA'$ 的唯一初等分解 (章 IV, § 2, no. 3)。

#### 定理 1 {#ac-v-s2-thm-1 .statement tag=04PR}

令$h : A \to A'$为单射环同态，使得$A$是$A$的积分，并且$p$是$A$的素理想。存在$A'$的素理想$p'$位于$p$之上。

首先假设$A$是局部环，$p$是$A$的最大理想；那么，对于$A'$的每个最大理想$m'$，$h^{-1}(m')$是$A$（命题1）的最大理想，因此等于$p$，在这种情况下证明了定理（因为$A'$包含 $A$ 乘以假设，因此不会减少到 0)。一般情况下，我们写 $S = A - p$；那么 $S^{-1}A$ 是局部环，其最大理想是 $S^{-1}p$ (章 11, § 2, no. 5, 命题 11), $S^{-1}h : S^{-1}A \to S^{-1}A$，是单射 (章 II, § 2, no. 4, 定理 1) 并且$S^{-1}A'$ 是 $S^{-1}A$ 的积分 ($§ 1$, no. 5, 命题 16)；那么存在$S^{-1}p$上方的$S^{-1}A'$的素理想$q'$，并且我们知道$q' = S^{-1}p'$，其中$p'$是位于$p$（引理1）上方的$A'$的素理想。

如果 $h : A \to A'$ 不是单射，定理 1 不再必然为真，如同态 $Z \to \mathbf{Z}/n\mathbf{Z} \ (n > 1)$ 的例所示。然而定理 1 可以应用于典范嵌入 $h(A) \to A'$；在其他字中，定理 1 的叙述对于素理想 $p$ 包含 $\mathrm{Ker}(h)$ 成立。

#### 推论 1 {#ac-v-s2-thm-1-cor-1 .statement tag=04PS}

假设定理 1、$\bar{h}^{-1}(pA') = p$ 和记号。

$pA' \subset p'$ 和 $\bar{h}(p') = p$。

#### 推论 2 {#ac-v-s2-thm-1-cor-2 .statement tag=04PT}

令$h : A \to A'$为环同态，使得$A'$是$A$、$a$和$p$的积分，$A$的两个理想，使得$a \subset p$和$a'$的理想$A'$位于$a$之上。假设 $p$ 是素数。那么存在$A'$的素理想$p'$位于$p$和包含$a'$之上。

如果 $h_1 : A/a \to A'/a'$ 是 $h$ 取商所得的同态，$h_1$ 是假设的单射，$A'/a'$ 是 $A/a$ 的积分（$§ 1$、no. 1、命题 2）；则存在$A'/a'$（$A$中的p'素的）的素理想$p'/a'$位于$p/a$（定理 1）之上，并且$p'$是所需的理想。

#### 推论 3 {#ac-v-s2-thm-1-cor-3 .statement tag=04PU}

令$A$为环且$A'$环包含$A$并对$A$整的。如果$\mathscr{R}'$是$A'$的雅各布森根式，那么$\mathscr{R}' \cap A$就是$A$的雅各布森根式。

令 $32$ 为 $A$ 的雅各布森根式。对于$A'$的每个最大理想$m'$，$m' \cap A$是$A$（命题1）的最大理想，因此$\mathscr{R} \subset m' \cap A$，因此$\mathscr{R} \subset \mathscr{R}' \cap A$（代数，章VIII, § 5, no. 3， 定义3）。相反地​​，令 $x \in 32' \cap A$；对于$A$的每个最大理想$m$，都存在一个位于$m$之上的素理想$A'$（定理1），并且这个理想$m'$必然是最大的（命题1），因此$x \in m' \cap A = m$和$x \in 32$。

#### 推论 4 {#ac-v-s2-thm-1-cor-4 .statement tag=04PV}

令 $A$ 为环、$A'$ 环包含 $A$，并从 $A$ 到代数闭域对 $A$ 和 $f$ 同态进行积分$L$。那么$f$可以从$A'$扩展到$L$延伸到同态。

令$\mathfrak{p}$为$f$的核，这是一个素理想，因为$f(A) \subset L$是整环；令 $\mathfrak{p}'$ 为$A'$ 的素理想，位于 $\mathfrak{p}$ (定理 1) 之上。那么 $A/\mathfrak{p}$ 与 $A'/\mathfrak{p}'$ 的子环被规范地等同，并且 $A'/\mathfrak{p}'$ 是 $A/\mathfrak{p}$ 上的积分（$§ 1$、no. 1、命题 2）。 同态 $f$ 定义，将$A/\mathfrak{p}$的同构除以$L$的子环$f(A)$，可推广至域的同构$g$ 分数 $K$ $A/\mathfrak{p}$ 到子域 $L$。由于分数 $K'$ $A'/\mathfrak{p}'$ 的域是$K$ 上的代数，$g$ 可以扩展到$K'$ 的同构 $g'$ 到$L$ 的子域 （代数、章 V、$§ 4$、no. 2，定理 1 的推论）；如果$\pi': A' \to A'/\mathfrak{p}'$是典范同态，则$g' \circ \pi'$是同态，从$A'$到$L$延伸$f$。

#### 注 (2) {#ac-v-s2-n1-rem-2 .statement tag=04PW}

令$h : A \to A'$为环同态，使得$A'$是$A$的积分；那么关联的连续映射 $^a h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ 是闭合的。对于$A'$的每个理想$a'$，$A'/a'$是$A'$上的积分，因此也超过$A$（$§ 1$，no. 1，命题6），并且$\mathrm{Spec}(A'/a')$用闭子空间标识$V(a')$ 共 $\mathrm{Spec}(A')$；为了证明 $^a h$ 是闭的，我们看到（替换 $A'$ by $A'/a'$）足以证明$^a h$下$\mathrm{Spec}(A)'$的像是$\mathrm{Spec}(A)$的闭子集；现在从定理 1 可以得出，这个像只是 $A$ 包含理想$\mathrm{Ker}(h)$ 的素理想的集合，而这个集合被$\mathrm{Spec}(A)$ 上拓扑的定义封闭。

#### 命题 2 {#ac-v-s2-prop-2 .statement tag=04PX}

令$h : A \to A'$为环同态，使得$A'$是$A$的积分，$\mathfrak{p}$是$A$、$S = A - \mathfrak{p}$、$(p'_i)_{i \in I}$的素理想，$A'$的所有素理想$\mathfrak{p}$位于上面$\mathfrak{p}$和$S' = \bigcap_{i \in I} (A' - p_i)$；然后$S^{-1}A' = {S'}^{-1}A'$。

事实上，通过定义 $h(S) \subset S'$ 并且，

$$
h(S)^{-1}A' = S^{-1}A',
$$

凭借章 II、$§ 2$、no. 3、命题 8，足以证明，如果$A'$的素理想$q'$不满足$h(S)$，那么它也不满足$S'$。现在，假设 $q' \cap h(S) = \varnothing$ 并令 $q = h^{-1}(q')$；然后$q \cap S = \varnothing$，其他字$q \subset \mathfrak{p}$。由于$q'$位于$q$上方定义，因此从推论2到命题1，存在指标$c$，使得$q' \subset p'_c$进而$q' \cap S' = \varnothing$，从而完成证明。

#### 命题 3 {#ac-v-s2-prop-3 .statement tag=04PY}

令$h : A \to A'$为环同态，使得$A'$是有限生成的$A$模；那么，对于$A$的每个素理想$\mathfrak{p}$，位于$\mathfrak{p}$之上的$A'$的素理想集合是有限的。

让$S = A - p$；通过引理 1，我们可以通过$S^{-1}A$实现替换$A$，通过$S^{-1}A'$实现$A'$（这是一个有限生成的$S^{-1}A$模块），通过$S^{-1}p$实现$p$；在其他字中，我们可以假设$A$是局部环，$p$是它的最大理想。然后（通过本号开头的注），$A$可以用$A/p$替代，$A'$可以用$A'/pA'$替代，$p$可以用$(0)$替代，因为$A'/pA' = (A/p) \otimes_A A'$是有限生成的$(A/p)$模块。这样，当$A$为域和$p = (0)$时，我们最终将问题减少为证明命题；那么$A'$是有限秩的$A$代数，因此是阿廷的，我们知道在这样的代数中只有有限的数素理想（章IV, § 2, no. 5，命题9）。

### 2. 分解群和惯性群

#### 定义 2 {#ac-v-s2-def-2 .statement tag=04PZ}

令$A'$为环，并且$G$群在$A'$（$§ 1$，no. 9）上运行。给定元素 $\sigma \in G$ 的素理想 $p' \subset A'$ 子群，使得 $\sigma.p' = p'$ 被称为 $p'$ 的分解群（相对于 $G$），并用 $G^z(p')$ 表示。 $G^z(p')$下不变的$A'$元素环称为$p'$的分解环（相对于$G$）并用$A^z(p')$(*)表示。

在没有歧义的情况下，我们经常分别写为$G^z$和$A^z$来代替$G^z(p')$和$A^z(p')$。

对于所有$\sigma \in G^z(p')$，我们还用环$A'/p'$的$z \mapsto \sigma.z$自同态表示，通过取商从$A'$的自同态$x \mapsto \sigma.x$得出；显然群$G^z(p')$在环$A'/p'$上是这样运作的。

#### 定义 3 {#ac-v-s2-def-3 .statement tag=04Q0}

以定义 2 的记号、$\sigma$ 的$G^z(p')$ 由……组成子群使得$A'/p'$ 的自同态 $z \mapsto \sigma.z$ 为恒等式，称为惯性群 $p'$（相对于$G$）并用$G^T(p')$（或$G^T$）表示。 $A'$在$G^T(p')$下不变的元素的环称为$p'$的惯性环（相对于$G$），并用$A^T(p')$（或$A^T$）（†）表示。

如果$A$是$G$的不变量的$A'$由……组成中的子环，显然

$$
A \subset A^z(p') \subset A^T(p') \subset A'.
$$

从定义 2 和 3 可以得出，对于所有 $p \in G$，

$$
G^z(\rho.p') = \rho G^z(p') \rho^{-1}, \quad G^T(\rho.p') = \rho G^T(p') \rho^{-1}.
$$

如果对于所有$\sigma \in G^z(p')$，$\bar{\sigma}$是$A'/p'$的自同构$z \mapsto \sigma.z$，$\sigma \mapsto \bar{\sigma}$是$G^z$到群$\Gamma_0$的同态（称为规范），自同构的

(*) 字母$Z$是德语字“Zerlegung”的首字母，意思是“分解”。
(†) 字母 T 是德语字“Tragheit”的首字母，意思是“惯性”。

A'/p' 留下 $A^{\mathbf{Z}}/(p' \cap A^{\mathbf{Z}})$ 的不变式元素（规范地用 $A'/p'$ 的子环来识别）并且通过定义 $\mathscr{G}^{\Gamma}(p')$ 是这个典范同态的核；因此，$\mathscr{G}^{\Gamma}$ 是 $\mathscr{G}^{\mathbf{Z}}$ 的正常子群。如果$k'$是$A'/p'$的分数的域，$A'/p'$的每一个自同构都可以唯一地扩展到$k'$的自同构，这样$\sigma \mapsto \bar{\sigma}$可以被认为是从$\mathscr{G}^{\mathbf{Z}}(p')$到同态 $k'$ 自同构群。 注最后，由于$\mathscr{G}^{\Gamma}$在$\mathscr{G}^{\mathbf{Z}}$正常，$A^{\Gamma}$在$\mathscr{G}^{\mathbf{Z}}$下稳定。

#### 引理 3 {#ac-v-s2-lem-3 .statement tag=04Q1}

*设$A'$为环、$\mathscr{G}$群，对$\mathscr{G}$、$p'$的不变量$A'$、$A$环进行操作，$A'$的素理想和$S$ $A$ 的乘法子集不满足$p'$。然后 $\mathscr{G}^{\mathbf{Z}}(S^{-1}p') = \mathscr{G}^{\mathbf{Z}}(p')$、$\mathscr{G}^{\Gamma}(S^{-1}p') = \mathscr{G}^{\Gamma}(p')$，如果 $\mathscr{G}$ 局部有限，则$S^{-1}A^{\mathbf{Z}}(p') = A^{\mathbf{Z}}(S^{-1}p')$ 和 $S^{-1}A^{\Gamma}(p') = A^{\Gamma}(S^{-1}p')$。*

由于$S$的元素在$\mathscr{G}$下是不变的，显然，如果$\sigma.p' = p'$，也有$\sigma.(S^{-1}p') = S^{-1}p'$。相反，假设$\sigma \in \mathscr{G}$使得$\sigma.(S^{-1}p') = S^{-1}p'$；那么，如果$x \in p'$，$(\sigma.x)/1 \in S^{-1}p'$，因此存在$s \in S$使得$s(\sigma.x) \in p'$，从而$\sigma.x \in p'$，因为$p'$是素数且$s \notin p'$；这证明了$\sigma.p' \subset p'$，并且可以类似地证明$\sigma^{-1}.p' \subset p'$，因此$\sigma.p' = p'$和$\sigma \in \mathscr{G}^{\mathbf{Z}}(p')$。如果$\sigma \in \mathscr{G}^{\Gamma}(p')$，则$\sigma.x - x \in p'$对于所有$x \in A'$，因此，对于所有$s \in S$，

$$
\sigma.(x/s) - (x/s) = (O.x - x)/s \in S^{-1}p'
$$

因此$\sigma \in \mathscr{G}^{\Gamma}(S^{-1}p')$。相反，假设$\sigma \in \mathscr{G}^{\Gamma}(S^{-1}p')$；那么，对于所有$x \in A'$，$\sigma.(x/1) - (x/1) \in S^{-1}p'$，因此存在$s \in S$，使得$s(\sigma.x - x) \in p'$，从而如上$\sigma.x - x \in p'$，这证明了$\sigma \in \mathscr{G}^{\Gamma}(p')$。最后两个断言是从§ 1, no. 9、命题23开始的。

#### 定理 2 {#ac-v-s2-thm-2 .statement tag=04Q2}

*令$A'$为环，$\mathscr{G}$有限群对$\mathscr{G}$的不变量$A'$和$A$环进行运算，使得$A'$在$A$上积分（§ 1, no. 9， 命题22).*

(i) *给定$A'$的两个素理想$p', q'$位于$A$的同一素理想$p$之上，存在$\sigma \in \mathscr{G}$使得$q' = \sigma.p'$；在其他字中，$\mathscr{G}$可传递地作用于$p$之上的$A'$素理想的集合。*

(ii) *设$p'$为$A'$、$p = p' \cap A$和$k$（分别为$k'$）、域或$A/p$（分别为$A'/p'$）的分数。那么$k'$是$k$和典范同态$\sigma \mapsto \bar{\sigma}$从$\mathscr{G}^{\mathbf{Z}}(p')$到群$\Gamma$的$k$自同构（$k'$定义），通过取$\mathscr{G}^{\mathbf{Z}}(p')/\mathscr{G}^{\Gamma}(p')$ 的同构到 $\Gamma$ 的商。*

(*) 在阶中，为了避免与字“正常”的其他含义混淆，我们今后使用项“准伽罗瓦扩展”作为代数、章、V, § 6, no. 2、定义2中定义的项“正常扩张”的同义词。

(i) 如果$x \in \mathfrak{q}$则$\prod_{\sigma \in \mathscr{G}} \sigma.x \in q' \cap A = p \subset p'$；那么存在$\sigma \in \mathscr{G}$使得$\sigma.x \in p'$，即$x \in \sigma^{-1}.q'$。我们结论即$q' \subset \bigcup_{\sigma \in \mathscr{G}} \mathfrak{s}.\mathfrak{p}'$，因此（因为$\mathscr{G}$是有限的且$\mathfrak{s}.\mathfrak{p}'$素的）存在$\sigma \in \mathscr{G}$使得$\mathfrak{q}' \subset \mathfrak{s}.\mathfrak{p}'$（章II, § 1, no. 1，命题2）；因为$q'$和$\sigma.\mathfrak{p}'$都位于$p$、$q' = \sigma.\mathfrak{p}'$之上（no. 1，推论1到命题1）。

(ii) 要看出$k'$是$k$的拟伽罗瓦扩展，只需证明元素$\bar{x} \in A'/p'$是$k[X]$中的多项式$P$的根，其所有根都在$A'/p'$中（代数、章 V, § 6, no. 3、推论 3 至命题 9）。现在，让$x \in A'$代表类$\bar{x}$；多项式 $Q(X) = \prod_{\sigma \in \mathscr{G}} (X - \sigma.x)$ 的所有系数都在 $A$ 中；令$P(X)$为$(A/p)[X]$中的多项式，其系数为$Q$在典范同态$\pi : A \to A/p$下的像。由于$\pi$可以被认为是典范同态$\pi' : A' \to A'/p'$的限制到$A$，因此可以看出，$P$是线性因子$X - \pi'(\sigma.x)$的$(A'/p')[X]$中的乘积，因此求解自$\bar{x} = \pi'(x)$起问题。

显然，对于所有$\sigma \in \mathscr{G}^z$，$\hat{\sigma}$是$k'$的$k$自同构；仍然需要验证 $\sigma \mapsto \hat{\sigma}$ 映射 $\mathscr{G}^z$ 到 $k'$ 的所有 $k$ 自同构的群上。让我们写$S = A - p$；由于§ 1, no. 9、命题 23 和关系 $S^{-1}p' \cap S^{-1}A = S^{-1}(A \cap p') = S^{-1}p$，$k$ 和$k'$ 分别不会被替换 $A'$ 和$p'$ $S^{-1}A'$ 和$S^{-1}p'$ 改变（章11，§ 2, no. 4）；从引理 3 可以看出，$\mathscr{G}^z$ 及其在 $k'$ 上的运算都没有改变；因此，我们可以将注意力限制在$p$最大的情况，在这种情况下，我们知道$p'$也是最大（no. 1，命题1），因此对于某些$x \in A'$，$k'$的每个元素都是形式$\pi'(x)$；从上面可以看出，这样的元素是次数$\leq \mathrm{Card}(\mathscr{G})$的$k[X]$多项式的根。由于$k$的每个有限可分扩张都承认一个原语元素（代数，章V, § 7, no. 7，命题12和§ 11, no. 4，命题4），因此可以看出，每个有限可分扩张 $k'$中包含的$k$是次数$\leq \mathrm{Card}(\mathscr{G})$、从而，因此$k'$中包含的$k$中的最大的可分扩张$k'_s$(代数， 章 V, § 7, no. 6、命题 11) 为次数 $\leq \mathrm{Card}(\mathscr{G})$ (代数、章 V, § 3, no. 2、注 2)。令$y \in A'$为元素，使得$\pi'(y)$是$k'_s$的原语元素。 $\sigma \in \mathscr{G} - \mathscr{G}^z$ 的理想$\sigma.p'$ 是最大的，并且与 $p'$ 相差定义；因此，存在$x \in A'$，使得$x \equiv y \pmod{p'}$和$x \in \sigma^{-1}p'$对应$\sigma \in \mathscr{G} - \mathscr{G}^z$（章11，§ 1, no. 2，命题5）。既然如此，设$u$是$k'$的$k$自同构，并设$P(X) = \prod_{\sigma \in \mathscr{G}} (X - \pi'(\sigma.x))$；由于$\pi'(x)$是$P$和$P \in k[X]$的根，$u(\pi'(x))$也是$k'$中$P$的根，因此存在$\tau \in \mathscr{G}$使得

$$
u(\pi'(x)) = \pi'(\tau.x);
$$

但是$u(\pi'(x)) \neq 0$，对于$\sigma \in \mathscr{G} - \mathscr{G}^z$，$\sigma.x \in p'$，因此$\pi'(\sigma.x) = 0$；我们结论必然$\tau \in \mathscr{G}^z$。但由于$u$和$\tilde{\tau}$对于$k'_s$的原语元素$\pi'(y) = \pi'(x)$具有相同的值，因此它们在$k'_s$上有重合，并且由于$k'$是$k'_s$的根式扩张，他们在$k'$上重合。

#### 推论{#ac-v-s2-n2-cor-1 .statement tag=04Q3}

*根据假设和定理2中的记号，令$f_1, f_2$为$A$至域$L$中的两个同态，且限制至$A$相同。那么存在 $\sigma \in \mathscr{G}$ 这样*

$$
f_2(x) = f_1(\sigma.x)
$$

*对于所有人*$x \in A'$。

设$p'_i$为$f_i$($i = 1, 2$)的核，这是$A'$的素理想； 假设 $p'_1 \cap A = p'_2 \cap A$，而这个交是$A$的素理想$p$；因此存在 $\tau \in \mathscr{G}$ 使得 $\tau.p'_2 = p'_1$ (定理 2 (i))； 替换$f_1$乘以同态$x \mapsto f_1(\tau.x)$，我们可以假设$p'_2 = p'_1$（我们用$p'$表示的理想）。通过求商，我们可以从$f_1$和$f_2$从$A'/p'$到$L$得出两个单同态$f'_1, f'_2$，因此从域得出扩展到两个单同态$f''_1, f''_2$ 分数$k'$共$A'/p'$至$L$。由于 $k'$ 是 $k$ 的准伽罗瓦扩展，$k''_1 = f''_1(k')$ 和 $k''_2 = f''_2(k')$ 也是如此（k 与 $L$ 的子域相同），而且，$k''_1$ 在 $k''_2, k''_1 = k''_2$ 上存在 k 同构（*代数*、章V, § 6、命题6）。因此$f''_1 \circ {f''_2}^{-1}$是$k'$的k-自同构； 定理 2 (ii) 因此，它是形式 6，其中$\sigma \in \mathscr{G}^z(p')$。特别是，对于所有 $x \in A'$ 元素 $f_2(x)$ 和 $f_1(\sigma.x)$ 都是相等的。

**注**

(1) 注在定理 2 的假设下，如果$k'$ 在$k$ (习题 9) 上不可分，则$k'$ 可能在$k$ 上“无限”。

(2) 显然，如果域 $k$ 是*完美*，则 $k$ 是 $k$ 的 *伽罗瓦* 扩张。那么它在 $k$ 上是有限的。

#### 命题 4 {#ac-v-s2-prop-4 .statement tag=04Q4}

*设$A'$为环、$\mathscr{G}$有限群，对$\mathscr{G}$的不变量的$A'$、$\mathscr{H}$子群进行操作，$\mathscr{G}$、$A$和$B$环分别为 $\mathscr{H}$ 和 $p'$ $A$ 的素理想；让我们写 $p = A \cap p'$ 和 $p(B) = B \cap p'$。

(i) 要使$\mathscr{H}$包含在分解群$\mathscr{G}^z(p')$中，$p'$是$A$位于$p(B)$之上的唯一素理想，是充分必要的。

(ii) *如果$\mathscr{H}$包含于$\mathscr{G}^z(p')$，则满足以下条件*：
(a) *环$A/p$和$B/p(B)$具有相同的域和分数*。
(b) *局部环$B_{p(B)}$的最大理想等于$pB_{p(B)}$*。

(iii) *进一步假设$A'$为整环且$\bigcap_{n \geq 0} p^nA'_p = 0$；那么条件 (a) 和 (b) & (ii) 意味着 $\mathscr{G}^z(p')$ 使 $B$* 保持不变元素。

(i) 由定理 2 (i) 可知，位于$p(B)$之上的$A$的素理想是形式 $\sigma.p'$的理想，其中$\sigma \in \mathscr{H}$； 从而立即 (i)。

(ii) 我们写$S = A - p$；我们知道$S^{-1}A'$中$\mathscr{G}$和$\mathscr{H}$的不变量环分别为$S^{-1}A$和$S^{-1}B$（§ 1, no. 9，命题23）和$\mathscr{G}^{\mathbf{Z}}(S^{-1}p) = \mathscr{G}^{\mathbf{Z}}(p')$（引理3）；最后$S^{-1}p(B) = S^{-1}p' \cap S^{-1}B$(章II, § 2, no. 4)，环$S^{-1}B$的素理想$S^{-1}p(B)$的局部环与$B_{p(B)}$自然同构，其剩余类域与域同构分数 / $B/p(B)$（章 II, § 2, no. 5、命题 11）。因此，我们可以证明 (ii) 将我们的注意力限制在 $p$ 最大的情况。为建立(a)，只需证明

$$
B = A + p(B)
$$

因为这将表明域 $A/p$ 和 $B/p(B)$ 是*自然同构*。到定理 2 时，只有有限数的 $A'$ 素理想位于 $p$ 之上，到 no. 1 的定理 1 时，至少有一个 $A'$ 素理想位于 $B$ 的每个素理想之上；这意味着$B$的素理想只有*有限*数位于$p$之上；让$n_j$ ($1 \leq j \leq r$) 表示这些理想中的$\neq p(B)$。设$x$为$B$的元素；由于理想 $p(B)$ 和 $n_j$ 是最大的 (no. 1, 命题 1)，因此存在 $y \in B$，使得 $y \equiv x$ (mod. $p(B)$) 和 $y \in n_j$ 对于 $1 \leq j \leq r$ (章 11， § 1, no. 2、命题5)。令$y_1 = y, y_2, \ldots, y_q$不同于$\mathscr{G}$下的$y$轨道元素；显然地

$$
z = y_1 + y_2 + \cdots + y_q \in A,
$$

并建立（3），只要证明 $y_i \in p'$ 对于 $i \geq 2$ 就足够了，因为那时我们将从 $x \equiv y$（模 $p(B)$）推论出 $z - y \in p' \cap B = p(B)$、从而 $x \in A + p(B)$。然后令$i \geq 2$和$\sigma \in \mathscr{G}$使得$\sigma.y = y_i$；我们证明$\sigma^{-1}.p'$不高于$p(B)$。否则，将存在$\tau \in \mathscr{H}$使得$\sigma^{-1}.p' = \tau.p'$（定理2（i）），从而$(\tau^{-1}\sigma^{-1}).p' = p'$，在其他字$\tau^{-1}\sigma^{-1} \in \mathscr{G}^{\mathbf{Z}} \subset \mathscr{H}$由假设，从而$\sigma \in \mathscr{H}$;但对于$y \in B$和$\sigma.y \neq y$来说，这是荒谬的。我们结论认为$\sigma^{-1}.p'$高于理想之一$n_j$，并且，正如$y \in n_j$与构造一样，当然是$y \in \sigma^{-1}.p'$或$y_i = \sigma.y \in p'$。

证明 (b) 足以证明$p(B)$包含在理想$pB$相对于$p(B)$的*饱和度*$q$中（章II, § 2, no. 4，命题10）；由于 $p(B)$ 不包含在 $n_j$ ($1 \leq j \leq r$) 中，因此只需证明

$$
p(B) \subset q \cup n_1 \cup \cdots \cup n_r
$$

通过章 II, § 1, no. 1、命题 2。为此，我们考虑元素 $u \in p(B)$ 属于到 $n_j$ ($1 \leq j \leq r$) (章 11、§ 1, no. 1、命题) 2）；令$u_1 = u, u_2, \ldots, u_m$为$\mathscr{G}$下$u$的轨道的不同元素；我们写$w = u_1u_2 \ldots u_m, v = u_2 \ldots u_m$；显然$w \in A$；另一方面，如果$\tau \in \mathscr{H}$，$\tau.u = u$，因此对于$i \geq 2$必然是$\tau.u_i \neq u$，这表明$\tau.v = v$，因此$v \in B$。可以如(a)的证明所示，如果$\sigma \in \mathscr{G}$是这样的$\sigma.u = u_i$，其中$i \geq 2$、$\sigma^{-1}.p'$位于$n_j$之一之上，并且如$u \notin n_j$，也位于字中的$u \notin \sigma^{-1}.p'$ $u_i \notin p'$。我们结论$v \notin p'$，因此$v \notin p(B)$。另一方面，显然$w \in p' \cap A = p$和关系$w = uv$表明$u$相对于$p(B)$处于$pB$的饱和状态，因此成立（4）。

(iii) 假设$A'$为整环，则(ii)的$\bigcap_{n \geq 0} p^n A'_p = 0$和条件成立。与(ii)中的记号相同，显然$S^{-1}A'$是整环和$S^{-1}A'_p = A'_p$；因此，可以通过$S^{-1}A'$和$S^{-1}p'$来替换、$A'$和$p'$，在其他字中，还假设理想的$p$是最大的。假设 (a) 和 (b) 意味着

$$
\mathbf{B}_{p(B)} = A + p \mathbf{B}_{p(B)}
$$

到 $n$ 上的归纳，我们推导出所有 $n > 0$ 都有 $\mathbf{B}_{p(B)} = A + p^n \mathbf{B}_{p(B)}$。然后令$\sigma$为$\mathscr{G}^\mathbf{Z}$的元素，并且$x$为$B$的元素。对于所有$n > 0$，存在$a_n \in A$使得$x - a_n \in p^n \mathbf{B}_{p(B)} \subset p^n A'_p$；作为$\sigma.a_n = a$和$\sigma.p' = p'$，我们推导出$\sigma.x - x \in p^n A'_p$。由于这个关系对所有$n$都成立，所以我们从假设得到结论到$\sigma.x = x$。

哈克斯

(3) 如果$A'$是整环且诺特，则条件$\bigcap_{n \geq 1} p^n A'_p = 0$始终成立（章III, § 3, no. 2，命题5的推论）。可以证明，如果假设$A'$为整环且$A$为诺特，则也满足此条件。

(4) 如果$p$不是$A$的最大理想，则关系(3)在(ii)的假设下不一定成立，因此即使我们取$\mathscr{H} = \mathscr{G}^\mathbf{Z}$、从而$B = A''$ (习题)，$A/p$和$B/p(B)$也不一定是同构的10）。

#### 推论 1 {#ac-v-s2-prop-4-cor-1 .statement tag=04Q5}

假设定理 2 环 $A/p$ 和 $A^\mathbf{Z}/(p' \cap A^\mathbf{Z})$ 具有相同的域分数且局部环 $(A^\mathbf{Z})'_{p' \cap A^\mathbf{Z}}$ 的最大理想由 $p$ 生成。

#### 推论 2 {#ac-v-s2-prop-4-cor-2 .statement tag=04Q6}

令$A'$为整环、$\mathscr{G}$有限群，对$\mathscr{G}$和$p'$的不变量$A'$、$A'$环进行运算，$A'$的素理想；令$K, K^\mathbf{Z}$和$K$分别为$A, A^\mathbf{Z}$和$A'$的分数域。那么$K'$是$K$的伽罗瓦扩张和$K$包含于$K$的子域$L$，这样$p'$是$A'$位于理想$p' \cap L$之上的唯一素理想的 $A' \cap L$ 正是那些包含 $K^\mathbf{Z}$。

$\mathscr{G}$ operates on $K'$ and $K$ is the field of invariants of $\mathscr{G}$ in $K'$ (§ 1, no. 9, Proposition 23 applied to $S = A - \{0\}$) and similarly $K^\mathbf{Z}$ is the field of invariants of $\mathscr{G}^\mathbf{Z}$; by definition $K'$ is therefore a Galois extension of $K$. 如果那些$\sigma \in \mathscr{G}$的$\mathscr{G}$由……组成子群留下L的不变元素，则说L包含$K^{\mathbf{Z}}$意味着$\mathscr{H}$包含在$\mathscr{G}^{\mathbf{Z}}$（代数，章）中V, § 10, no. 5, 定理 3) 并且，由于 L 是 $K'$ 中$\mathscr{H}$ 不变量的域，$A' \cap L$ 是 $A'$ 中 $\mathscr{H}$ 不变量的环；第二个断言是从命题4(i)开始的。

#### 定义 4 {#ac-v-s2-def-4 .statement tag=04Q7}

*根据推论 2 至命题 4 的假设和记号，如果位于$\mathfrak{p}$之上的$A'$素理想数等于$[K':K]$，则称$A$的素理想$\mathfrak{p}$在$K'$中完全分解。*

It amounts to the same to say that, for a prime ideal $\mathfrak{p}'$ of $A'$ lying over $\mathfrak{p}$, the subgroup $\mathscr{G}^{\mathbf{Z}}(\mathfrak{p}')$ is equal to the subgroup $\mathscr{M}$ leaving invariant all the elements of $A'$, or that $A^{\mathbf{Z}}(\mathfrak{p}') = A'$, or that $\mathscr{G}/\mathscr{M}$ operates faithfully on the set of prime ideals of $A'$ lying above $\mathfrak{p}$.

#### 推论 3 {#ac-v-s2-def-4-cor-3 .statement tag=04Q8}

*设$A'$为整环，$\mathscr{G}$是对$A'$，$A$环进行运算的有限交换群，$\mathscr{G}$的不变量，$\mathfrak{p}$是$A$和$K$的素理想，并且分别为$A$和$A'$分数$K'$域。 那么$\mathfrak{p}$之上的$A'$的素理想都有相同的分解环$A^{\mathbf{Z}}$，分数$K^{\mathbf{Z}}$的域和$A^{\mathbf{Z}}$的最大的中间域 $K$和$K'$，其中$\mathfrak{p}$完全分解。*

如果$\mathfrak{p}'$是位于$\mathfrak{p}$之上的$A'$的素理想，则$\mathscr{G}^{\mathbf{Z}}(\sigma.\mathfrak{p}') = \mathscr{G}^{\mathbf{Z}}(\mathfrak{p}')$，因为$\mathscr{G}$是可交换的(公式 (2))，因此(定理 2 (i))位于$\mathfrak{p}$之上的$A'$的所有素理想具有相同的性质分解群 $\mathscr{G}^{\mathbf{Z}}$，因此相同的分解环 $A^{\mathbf{Z}}$；他们的数是$(\mathscr{G}:\mathscr{G}^{\mathbf{Z}})$。令L为K和$K'$之间的中间域，并令$\mathscr{H}$为$\mathscr{G}$的子群，留下L的不变式元素； $\mathfrak{p}'$相对于$\mathscr{H}$的分解群为$\mathscr{G}^{\mathbf{Z}} \cap \mathscr{H}$；由于$A' \cap L$是$A'$中$\mathscr{H}$不变量的环，位于$\mathfrak{p}' \cap L$之上的$A'$素理想的数是$(\mathscr{H}:(\mathscr{G}^{\mathbf{Z}} \cap \mathscr{H})) = (\mathscr{H}\mathscr{G}^{\mathbf{Z}}:\mathscr{G}^{\mathbf{Z}})$（因为$\mathscr{G}$是可交换的）。因此，位于$\mathfrak{p}$之上的$A' \cap L$素理想的数是$(\mathscr{G}:\mathscr{H}\mathscr{G}^{\mathbf{Z}})$。为了使$\mathfrak{p}$在L中完全分解，$(\mathscr{G}:\mathscr{H}\mathscr{G}^{\mathbf{Z}}) = [L:K] = (\mathscr{G}:\mathscr{H})$是必要且充分的，并且，作为$\mathscr{H} \subset \mathscr{H}\mathscr{G}^{\mathbf{Z}}$，这相当于$\mathscr{H}\mathscr{G}^{\mathbf{Z}} = \mathscr{H}$，或者还相当于$\mathscr{G}^{\mathbf{Z}} \subset \mathscr{H}$，最后相当于$L \subset K^{\mathbf{Z}}$。

#### 命题 5 {#ac-v-s2-prop-5 .statement tag=04Q9}

*假设定理 2 的记号，$A^T/(\mathfrak{p}' \cap A^T)$ 的分数 $k^T$ 域等于$k'$ 中包含的$k$ 最大的可分扩张 $k'_s$。*

如在命题 4 中，这可以简化为$\mathfrak{p}$ 是$A$ 的最大理想，这意味着$\mathfrak{p}'$、$\mathfrak{p}' \cap A^{\mathbf{Z}}$ 和$\mathfrak{p}' \cap A^T$ 分别在$A'$、$A^{\mathbf{Z}}$ 和$A^T$ 中最大（no. 1， 命题1)。

对于所有$x \in A'$，多项式$P(X) = \prod_{\sigma \in \mathscr{G}^T} (X - \sigma.x)$的惯性系数为环$A^T$，并且通过$\mathscr{G}^T$的定义，$A'$中的所有根都是同余模。 $\mathfrak{p}'$； $A^T/(\mathfrak{p}' \cap A^T)$上的多项式$\pi'(P)$其系数是P在同态$\pi':A' \to A'/\mathfrak{p}'$下的系数的典范像，因此$A'/\mathfrak{p}'$中的所有根等于$x$的像，这表明$k'$是根式扩张 / $k^T$； 从而$k'_s \subset k^T$，因为$k'_s$的每个元素都可以在k上分离，而更不必说在$k^T$上可分离。

我们知道$k'_s$是k的伽罗瓦扩张（代数，章V, § 10, no. 9，命题14），并且从定理2可以得出它的伽罗瓦群与$\mathscr{G}' = \mathscr{G}^z / \mathscr{G}^T$同构的。由于$k^T$是$k'_s$的根扩张，$k^T$是k的拟伽罗瓦扩展，并且$k^T$的次数在k上的可分因子是$q = (\mathscr{G}^z : \mathscr{G}^T )$。仍有待观察$k^T$是k的可分扩张。我们在上面看到，$\mathscr{G}'$与$A^T$的自同构群等同，而$A^z$是$\mathscr{G}'$的不变量的环。如果$x \in A^T$，则多项式$Q(X) = \prod_{\sigma' \in \mathscr{G}'} (X - \sigma'(x))$的系数在$A^z$中； $A^z / (p' \cap A^z)$ 上 Q 在 $\pi'$ 下的系数为像的多项式为次数 $q$，并且有根 $\pi'(x) \in A^T / (p' \cap A^T )$。由于$A^z / (p' \cap A^z) = k$乘以命题 4 (ii)，我们看到$k^T$的每个元素都是超过k的次数$\leq q$。

既然如此，令k为$k$的拟伽罗瓦扩展$k^T$的k-自同构群的不变量域；然后$[k^T : k_1] = q$（代数，章V, § 10, no. 9，命题14）。设$u$是$k^T$在$k_1$上的原语元素；由于它在 k 上具有次数 $q$，并且在 k 上具有次数 $\leq q$，因此它在 k 上具有次数 $q$ 及其在 k 上的最小多项式，其系数为 $k$；这表明 $u$ 在 k 上是可分的。另一方面，对于所有$v \in k_1$，存在特征指数p的幂$p'$使得$v^{p'} \in k$。我们结论$k(u - v)$，其中包含
$$
(u - v)^{p'} = u^{p'} - v^{p'},
$$
包含 $u^{p'}$，因而$k(u^{p'})$。但由于 $u$ 可以在 $k$、$k(u) = k(u^{p'})$ (代数、章 V, § 8, no. 3、命题 4)、从而 $k(u) \subset k(u - v)$ 上分离。由于$u$在k上是次数$q$并且$u - v$是次数$\leq q$，因而$k(u) = k(u - v)$，从而$v \in k(u)$。这表明 $v$ 在 k 上可分离，因而 $k_1 = k$ 和 $k^T$ 在 $k$ 上可分离。

#### 推出 {#ac-v-s2-n2-cor-2 .statement tag=04QA}

*如果惯性群$\mathscr{G}^T(p')$的阶与k的特征指数p互质，则域$k'$就是k的伽罗瓦扩张。*

当记号为证明为命题5时，多项式$\pi'(P)$在$k^T = k'_s$中有系数，并且其所有根等于$\pi'(x)$；我们立即推断出 $\pi'(P)$ 是 $\pi'(x)$ 与 $k'_s$ 的最小多项式的幂；但后者的次数等于p的幂，因而，由于$\pi'(P)$的次数等于$\mathscr{G}^T$的阶，假设意味着$\pi'(x) \in k'_s$，而其他字$k'_s = k'$。

### 3. 分解和整体闭域的惯性

#### 引理 4 {#ac-v-s2-lem-4 .statement tag=04QB}

*设 A 为积分闭域，K 为分数的域，p 为 K 的特征指数，K' 为 K 的基数扩张，A' 子环为 K' 包含 A 并在 A 上积分。对于 A 的每个素理想 p，都存在一个唯一的素理想* p' $A'$位于$p$和$p'$之上的是$x \in A'$的集合，因此存在整数$m \geq 0$，其中$x^{p^m} \in p$。

$p'$ 的存在源自no. 1、定理 1。如​​果$x \in p'$，则存在$m \geq 0$，使得$x^{p^m} \in K$、从而 $x^{p^m} \in A$，因为$A$ 是积分闭集，因此$x^{p^m} \in p' \cap A = p$。相反，如果 $x \in A'$ 满足 $x^{p^m} \in p \subset p'$，则 $x \in p$，因为 $p'$ 是素数。

#### 注 (1) {#ac-v-s2-n3-rem-1 .statement tag=04QC}

从§ 1, no. 3，推论到命题 11，$K'$中$A$的积分闭包是$x \in K'$的集合，因此存在$m \geq 0$，其中$x^{p^m} \in A$ (代数, 章 V, § 8, no. 1， 命题1)。

#### 命题 6 {#ac-v-s2-prop-6 .statement tag=04QD}

令$A$是一个整闭域，$K$是分数的域，$K'$是$K$的准伽罗瓦扩展，$A'$是$A$在$K'$的整闭域。然后：

(i) 对于$A$的每个素理想$p$，$K$的群$\mathscr{G}$，$K'$的自同构可传递地作用于位于$p$之上的$A'$素理想的集合。

(ii) For every prime ideal $p'$ of $A'$, the field of fractions $k'$ of $A'/p'$ is a quasi-Galois extension of the field of fractions $k$ of $A/(A \cap p')$ and the canonical homomorphism $\sigma \mapsto \tilde{\sigma}$ from $\mathscr{G}^Z(p')$ to the group $\Gamma$ of $k$-automorphisms of $k'$ defines, by taking the quotient, a bijection of $\mathscr{G}^Z(p')/\mathscr{G}^T(p')$ onto $\Gamma$.

(A) 首先假设$K'$是$K$的ajinite伽罗瓦扩张。那么$A = A \cap K$，因为$A$是积分闭的，因此$A$是$\mathscr{G}$在$A'$中的不变量的环。由于 $\mathscr{G}$ 是有限的，在这种情况下，命题由 no. 2、定理 2 得出。

(B) 其次假设$K'$是$K$中的任意伽罗瓦扩张。 那么$K'$就是$K$的有限伽罗瓦扩张的右有向族$(K_\alpha)_{\alpha \in I}$的并。 为了证明 (i)，请考虑位于 $p$ 之上的 $A'$ 的两个素理想 $p', q'$。 对于所有$\alpha \in I$，$p' \cap K_\alpha$和$q' \cap K_\alpha$是$A \cap K_\alpha$的两个素理想，位于$p$之上。 由于$A' \cap K_\alpha$是$K_\alpha$中$A$的整体闭包，以及$\mathscr{G}$形式群的元素的限制到$K_\alpha$-$K$的$K$自同构，因此从case可以得出(A) 存在$\sigma \in \mathscr{G}$使得$(\sigma.(p' \cap K_\alpha)) = q' \cap K_\alpha$。 令$\mathscr{E}_\alpha$为具有上述性质的$\sigma \in \mathscr{G}$的集合。 设 $\sigma \in \mathscr{G} - 8$；那么，对于所有$\tau \in \mathscr{G}$，留下$K_\alpha$的不变元素，(QT) $(\sigma.(p' \cap K_\alpha)) = \varrho.(p' \cap K_\alpha) \neq q' \cap K_\alpha$，因此$\sigma \tau \in \mathscr{G} - b$。 由此可见，$\mathscr{E}_\alpha$ 在拓扑伽罗瓦群 $\mathscr{G}$（代数、章 V、附录 11、no. 1）中是闭的，并且显然族 $(\mathscr{E}_\alpha)_{\alpha \in I}$ 是左有向的。 由于 $\mathscr{G}$ 是紧致的（如前所述，no. 2、命题 3）且 $\mathscr{E}_\alpha$ 非空，因此 $(8,)$ 族的交 $\mathscr{E}$ 非空，$\sigma.p' = q'$ 对于所有 $\sigma \in \mathscr{E}$、从而 (一).

为了证明(ii)，注$k'$是右有向族$(k_\alpha)_{\alpha \in I}$的并，其中$k_\alpha$是$(A' \cap K_\alpha)/(p' \cap K_\alpha)$的分数的域。由于每个 $k_\alpha$ 都是 $k$ 通过 (A) 的准伽罗瓦扩展，因此 $k'$ (代数, 章 V, § 6, no. 3, 命题 8)。另一方面，令$u$为$k'$的$k$自同构，并令$\pi': A' \to A'/p'$为典范同态。由于no. 2、定理 2 应用于$A' \cap K_\alpha$，对于所有$\alpha$，存在元素$\sigma \in \mathscr{G}$的非空集合$F_\alpha$，使得对于所有$x \in A' \cap K_\alpha$，$\sigma.(p' \cap K_\alpha) = p' \cap K_\alpha$和$u(\pi'(x)) = \pi'(\sigma.x)$。从上面可以看出，$\mathscr{F}_\alpha$在$\mathscr{G}$是闭的，并且由于$(\mathscr{F}_\alpha)$是左有向集合，所以它的交$\mathscr{F}$非空。显然，对于 $\alpha \in \mathscr{F}$、$\alpha \in \mathscr{G}^\mathbf{Z}(p')$ 和 $\tilde{\sigma} = u$，在本例中完成了 (ii) 的证明。

(C) *一般护理*。 $\mathscr{G}$的不变量$K_1$的域是$K$的根式扩张 (*代数*, 章 V, § 10, no. 9, 命题 14);因此，存在一个位于$p$（引理 4）之上的$A_1 = A' \cap K_1$的单一素理想$p_1$。如果$p'$和$q'$是$A'$位于$p$之上的两个素理想，那么它们位于$p_1$之上；由于$K'$是$K$的伽罗瓦扩张，并且$A' \cap K$是积分闭的（§ 1, no. 2、命题7和命题8的推论），从(B)可以得出，存在$\sigma \in \mathscr{G}$使得$(1.p' = q'$； 从而（一）。另一方面，显然分数$k$、$A_1/p_1$的域是$k$的根扩张（A是全闭的）；因为$k'$是$k$的拟伽罗瓦扩展，由(B)可知，$k'$是$k$的拟伽罗瓦扩展，$k'$的$k'$到代数闭扩张的每个$k$同构是$k_1$-同构。最后的注还表明，考虑到(B)，$k'$的每个$k$自同构都是形式$\tilde{\sigma}$，其中$\alpha \in \mathscr{G}^\mathbf{Z}(p')$，这完成了(ii)的证明。

*注*

(2) Suppose that $K$ is a *Galois* extension of $K$ and let us keep the notation of the proof of Proposition 6; for all $a$ let $\mathscr{G}_a^\mathbf{Z}$ (resp. $\mathscr{G}_a^\mathbf{T}$) be the subgroup of $\mathscr{G}$ consisting of the $\sigma$ whose restriction to $A' \cap K$, belongs to $\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $\mathscr{G}^\mathbf{T}(p' \cap K_\alpha)$). 命题 6 的证明表明这些子群在 $\mathscr{G}$ 中*封闭*，并且
$$
\mathscr{G}^\mathbf{Z}(p') = \bigcap_a \mathscr{G}_a^\mathbf{Z} \quad \text{and} \quad \mathscr{G}^\mathbf{T}(p') = \bigcap_a \mathscr{G}_a^\mathbf{T}.
$$
此外，限制到$A' \cap K$的集合，$\mathscr{G}$（或$\mathscr{G}_a^\mathbf{T}$）的元素是群$\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$（或$\mathscr{G}^\mathbf{T}(p' \cap K_\alpha)$）的整体，每个$K$自同构$K$，延伸至$\mathscr{G}$的元素。

With the same hypotheses, the ring $A^\mathbf{Z}(p')$ (resp. $A^\mathbf{T}(p')$) is the *union* of the directed family of the $A^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $A^\mathbf{T}(p' \cap K_\alpha)$); in fact, every $x \in A^\mathbf{Z}(p')$ (resp. every $x \in A^\mathbf{T}(p')$) belongs to one of the $K$, and by the above there exists a $\beta$ such that $K_\alpha \subset K_\beta$ and the restrictions to $A' \cap K$, of the elements of $\mathscr{G}^\mathbf{Z}(p')$ (resp. $\mathscr{G}^\mathbf{T}(p')$) are the same as the restrictions to $A' \cap K$, of the elements of $\mathscr{G}^\mathbf{Z}(p' \cap K_\beta)$ (resp. $\mathscr{G}^\mathbf{T}(p' \cap K_\beta)$), the groups $\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$ and $\mathscr{G}^\mathbf{T}(p' \cap K_\beta)$ being finite; hence $x$ belongs to $A^\mathbf{Z}(p' \cap K_\beta)$ (resp. $A^\mathbf{T}(p' \cap K_\beta)$).

#### 推论 1 {#ac-v-s2-prop-6-cor-1 .statement tag=04QE}

*在命题6的假设下，令f为从A到域L的同态，而g_1、g_2为从A'到L的两个同态，其中扩展f。那么存在一个 K-自同构 $\sigma \in K'$ 使得 $g_1 = g_2 \circ \sigma$.*

从命题 6 开始的证明与从后者开始到定理 2 的推论相同。

#### 推论 2 {#ac-v-s2-prop-6-cor-2 .statement tag=04QF}

*设 A 为积分闭域，K 为分数的域，K' 为 K 的有限代数扩张，A' 为 K' 包含 A 的子环以及 A 上的积分。*

(i) 对于位于$\mathfrak{p}$之上的$A'$素理想的$A$集合的每个素理想$\mathfrak{p}$都是有限的。
(ii) 如果$\mathfrak{p}'$是位于$\mathfrak{p}$之上的$A'$的素理想，$A'/\mathfrak{p}'$的每个元素都是次数$\leq [\mathbf{K}':\mathbf{K}]$超过$A/\mathfrak{p}$的分数的域。

(i) 设$K''$为$K'$的代数闭包中$K'$生成的$K$的拟伽罗瓦扩展，$A''$为$K''$中$A$的积分闭包。 域$K''$是$K$的有限扩张（代数，章V, § 6, no. 3，推论1到命题9），因此其$K$自同构的群是有限的；由此可见，位于$\mathfrak{p}$之上的$A''$素理想的集合是有限的（命题 6 (i)）。 另一方面，由于$A''$是$A$的积分，因此位于$\mathfrak{p}$上方的$A''$素理想的集合的映射$\mathfrak{p}'' \mapsto \mathfrak{p}'' \cap A'$位于$x$上方的$A'$素理想到集合是满射（no. 1，定理1）。

(ii) 任意元素 $x' \in A'$ 属于到 $A$ 的最小多项式（超过 $K$）的系数（$§ 1$、no. 3，命题 10 的推论）；将应用典范同态$\pi': A' \to A'/\mathfrak{p}'$代入该多项式的系数，对于类模，可得到$A/\mathfrak{p}$和次数$\leq [\mathbf{K}':\mathbf{K}]$系数的积分相关方程。 $\mathfrak{p}'$ / $x$； 从而结论。

#### 推论 3 {#ac-v-s2-prop-6-cor-3 .statement tag=04QG}

根据推论2的假设和记号，如果$A$是半局部的，$A'$也是半局部的。

对于$A'$的每个最大理想$m'$，$m' \cap A$是$A$的最大理想（no. 1，命题1）；然后从推论 2 得出推论，因为 $A$ 的最大理想的假设集合是有限的。

#### 推论 4 {#ac-v-s2-prop-6-cor-4 .statement tag=04QH}

Let $A$ be an integrally closed domain, $K$ its field of fractions, $K$ a Galois extension of $K$, $A'$ the integral closure of $A$ in $K'$, $\mathfrak{p}'$ a prime ideal of $A$, $\mathfrak{p} = A \cap \mathfrak{p}'$ and $k$ and $k'$ the fields of fractions of $A/\mathfrak{p}$ and $A'/\mathfrak{p}'$ respectively. 然后：

(i) $A^{\mathbf{Z}}/(\mathfrak{p}' \cap A^{\mathbf{Z}})$的分数的域等于$k$，$A^{\mathbf{Z}}$的局部环相对于$\mathfrak{p}' \cap A^{\mathbf{Z}}$的最大理想由$\mathfrak{p}$生成。

(ii) $A^T/(\mathfrak{p}' \cap A^T)$的分数$k^T$中的域是$k'$中包含的$k$中的最大的可分扩张。

环$A$是$K'$伽罗瓦群$A'$超过$K$的不变量环；如果 $K'$ 的有限次数大于 $K$，则从命题 4 和 5 of no. 2 得出推论。现在考虑一般情况，$K'$因此是$K$的有限伽罗瓦扩张的右有向集合$(K_i)$的并。然后：

(i) 如果$x, y$是$A^{\mathbf{Z}}$的两个元素，其中$y \notin \mathfrak{p}'$，则存在指标$\alpha$使得$x$和$y$属于到$A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha})$（注） 2）；通过no. 2的命题 4，$A$中有$x_0, y_0$和$y_0 \notin \mathfrak{p}'$，使得$xy_0 - x_0y \in \mathfrak{p}'$，这证明了(i)的第一个断言；如果进一步$x \in \mathfrak{p}'$，我们可以假设$y_0$满足
$$
xy_0 \in \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha}) \subset \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}'),
$$
这就证明了(i)的第二个断言。

(ii) 现在假设$x \in A^T$；存在$\alpha$使得no. 2的$x \in A^T(p' \cap K_\alpha)$(注2)和命题5表明$x \mod.(p' \cap K_\alpha \cap A^T)$的类$\bar{x}$是代数且在$k$上可分； *更不必说* 类 $\mod.(p' \cap A^T)$ 或 $x$ 在 $k$ 上可分；要完成推论的证明，只需证明$k'$是$k^T$的*根式*扩张即可。现在，$k'$是环$(A' \cap K_\alpha)/(p' \cap K_\alpha)$分数$k_\alpha$域的右有向族的并。因此，从命题 5 可以得出，如果 $k'$ 属于的元素到 $k$，则它是分数的域的根

$$
A^T(p' \cap K_\alpha)/(p' \cap A^T(p' \cap K_\alpha))
$$

和*更不必说*超过$k^T$（凭借注2）。

#### 定义 5 {#ac-v-s2-def-5 .statement tag=04QI}

*根据命题 6 的假设和记号，域 $K'$ 中群 $G^Z(p')$（$G^T(p')$）的不变量$K^Z(p')$（$K^T(p')$）域被称为 $p'$ 相对于 $K$* 的分解域*（或 *惯性域*）*。

我们还写 $K^Z$（或 $K^T$）来代替 $K^Z(p')$（或 $K^T(p')$）。从 § 1, no. 9、命题 23 可以得出，$K^Z$（分别为 $K^T$）是环 $A^Z$（分别为 $A^T$）的分数* 的域 *； $A^Z$（或$A^T$）是$A$在$K^Z$（或$K^T$）中的积分闭包。

*注*

(3) 根据命题 6 的推论 4 的条件，并假设$[K':K]$是*有限*，位于$p$之上的不同素理想的数是$[K^Z:K]$，这个次数等于指标 ('3:*G*Z*) 通过伽罗瓦理论；此外，根据伽罗瓦理论可以得出：

$$(6)$$
$$
[K^T:K^Z] = (G^Z:G^T) = [k^T:k].
$$

(4) 令$A$为积分闭域，$K$为分数的域，$K'$为$K$的有限代数扩张，$A'$为$A$在$K'$的积分闭集。 然后，对于$A$的每个素理想$p$，*数*$\&$*素理想*$\&$*的*$A'$*位于上面*$p$*最多*$[K':K]_s$（次数的可分离因子 $K$超过$K$）。 我们可以首先将注意力限制在$K$是$K$的可分扩张的情况，因为一般来说，$K$是$K'$中包含的$K$的扩张、最大的可分扩张$K_0$， $[K':K]_s = [K_0:K]$乘定义，如果$A$是$A$在$K_0$的积分闭包，$A$和$A'$的素理想是一一对应的对应（引理4）。 因此，假设$K$在$K$上可分，并令$N$为$K$的代数闭包中$K$生成的$K$的伽罗瓦扩张，$G$其伽罗瓦群，$B$的积分闭包$N$和$\mathfrak{P}$中的$A$是$B$的素理想，位于$p$之上。 令$\mathscr{H}$为$N$的伽罗瓦群超过$K$且$G^Z$为$\mathfrak{P}$的分解群； $p$之上的$B$的主要理想是$s.\mathfrak{P}$，其中$s \in G$（no. 2，定理2）和关系$s.\mathfrak{P} = s'.\mathfrak{P}$意味着$s' = sg$，其中$g \in G^Z$。 另一方面，在阶和$s.\mathfrak{P} \cap K' = s'.\mathfrak{P} \cap K'$中，$s'.\mathfrak{P} = ts.\mathfrak{P}$是充分必要的，其中$t \in \mathscr{H}$（no. 2，定理2），从而最后是$s' = tsg$，其中$t \in \mathscr{H}$和$g \in G^Z$。 因此，位于$p$之上的$A'$素理想的数等于等价关系*下$G$的类的*数*“存在$t \in \mathscr{H}$和$g \in G^{\mathbf{Z}}$使得$s' = tsg$”在$s$和$s'$;显然，根据伽罗瓦理论，数最多等于指标$(G : \mathscr{H})$、$\mathscr{H}$在$G$中的右陪集数，以及$(G : \mathscr{H}) = [K' : K]$。

#### 命题 7 {#ac-v-s2-prop-7 .statement tag=04QJ}

*设$A$为全闭域，$K$为分数的域，$K$的$K'$伽罗瓦扩张，$\mathscr{G}$为伽罗瓦群，$A'$$A$的全闭域$K'$、$p'$是$A'$和$p = A \cap p'$的素理想。最后，令$L$为$K'$包含于$K$中的子域，并令$p(L) = p' \cap L$。

(i) *分解域*（分别为*惯性域*）*$p'$相对于$L$为$L(K^{\mathbf{Z}})$（分别为$L(K^T)$）； *如果进一步$L$是$K$的伽罗瓦扩张，则$p(L)$相对于$K$的分解域是$L \cap K^{\mathbf{Z}}$。

(ii) *如果$L$包含在$K^{\mathbf{Z}}$中，$A/p$和$(A' \cap L)/p(L)$具有与分数相同的域，并且在局部环$A' \cap L$相应的中到素理想$p(L)$，则生成极大理想$p$。反之，如果这两个条件成立，再加上$\bigcap_{n > 0} p^n A'_p = 0$，则$L$包含在$K^{\mathbf{Z}}$中。

(i) 如果$\mathscr{H}$是$\mathscr{G}$的子群，而$L$的元素保持不变，则$p'$相对于$L$的分解群（分别为惯性群）为$G^{\mathbf{Z}} \cap \mathscr{H}$（分别$G^T \cap \mathscr{H}$）和第一个断言根据伽罗瓦理论得出，如果$K'$是$K$的*有限*伽罗瓦扩张（*代数*，章V, § 10, no. 6，推论1到定理3);在一般情况下，它是根据以下事实得出的：*注 2* 的记号中$A^{\mathbf{Z}}$（或$A^T$）是$A^{\mathbf{Z}}(p' \cap K_\alpha)$（或$A^T(p' \cap K_\beta)$）的并：每个元素$x \in K'$ 属于到某些$K$，如果它在$G^{\mathbf{Z}}(p') \cap \mathscr{H}$（或$G^T(p') \cap \mathscr{H}$）下不变，那么对于某些合适的$\beta'$，它在$G^{\mathbf{Z}}(p' \cap K_{\beta'}) \cap \mathscr{H}$（或$G^T(p' \cap K_{\beta'}) \cap \mathscr{H}$）下也不变；因此，在论证开始时它是属于

$$
L(K^{\mathbf{Z}}(p' \cap K_{\alpha})) \subset L(K^{\mathbf{Z}}) \quad (\text{resp. } L(K^T(p' \cap K_{\beta})) \subset L(K^T)).
$$

现在假设$L$是$K$的伽罗瓦扩张；每个$\sigma \in G^{\mathbf{Z}}$的限制到$L$然后留下不变的$p(L) = p' \cap L$，因此相对于$K$，$p(L)$的属于到分解群。相反，令$\tau$是$L$属于的自同构到这个群，并让$\sigma$是$\tau$的扩张到$K'$的$K$自同构；我们写$q' = \sigma.p'$。由于$p'$和$q'$都位于$p(L)$之上，因此存在自同构$\rho \in \mathscr{H}$使得$q' = \rho.p'$，从而$\rho^{-1}\sigma \in G^{\mathbf{Z}}$和$\tau$是$\rho^{-1}\sigma$的限制到$L$；在其他字中，$p(L)$的分解群相对于$K$与限制的群到自同构$\sigma \in G^{\mathbf{Z}}$的$L$相同，这证明了第二个断言。

(ii) 说$L \subset K^{\mathbf{Z}}$意味着当$[K':K]$有限时，(ii)的$\mathscr{H} \supset G^{\mathbf{Z}}$和断言是no. 2、命题 4 (ii)和(iii)的特例。在一般情况下，参数如命题 6 中的证明所示。

### 4.第二个存在定理

#### 定理 3 {#ac-v-s2-thm-3 .statement tag=04QK}

令 $A$ 为积分闭域，且 $A'$ 环包含 $A$ 且在 $A$ 上积分。假设$0$是$A$中唯一的元素，即$A'$中$0$的除子。令$p, q$为$A$的两个素理想，使得$q \supset p$和$q'$为位于$q$之上的$A$的素理想。那么存在$A$的素理想$p'$位于$p$之上，因此$q' \supset p'$。

首先假设$A'$是整环。设$K, K'$分别为$A$和$A'$的分数域；设$K''$为$K$和$A$的代数闭包，$A$在$K''$的积分闭包；然后$A \subset A' \subset A''$。令 $p''$ 为位于$p$之上的$A''$的素理想（no. 1，定理 1），$q''$位于$q$之上的$A''$的素理想，并且使得$p'' \subset q''$（no. 1，推论） 2 到定理 1)，最后是 $q_1''$ $A''$ 的素理想，位于 $q'$ (no. 1，定理 1) 之上。通过no. 3，命题 6 (i)，存在$K''$的$K$自同构$\sigma$，使得$Q.q'' = q_1''$。那么$Q.p''$是位于$p$上方的$A''$的素理想，使得$Q.p'' = q_1''$，因此$p' = A' \cap \sigma.p''$是位于$p$上方并包含在$A' \cap q_1'' = q'$中的$A'$的素理想。

我们转向一般情况。由于$A$是整环且$q'$是素数，所以子集$A - \{0\}$和$A' - q'$是$A'$的乘法；那么它们的乘积$S = (A - \{0\})(A' - q')$是$A'$的乘法子集，它不是包含0，因为$A$的非零元素不是$A'$中0的除子。那么存在（章II, §2, no. 5，推论2至命题11）从$S$出发的$A'$不相交的的素理想$m'$，在其他字中，使得$m' \subset q'$和$m' \cap A = 0$。设$h$为典范同态$A' \to A'/m'$。 $h$到$A$的限制是单射的，因此$h(A)$是积分闭的。由于$m' \subset q'$，$h(q')$是位于$h(q)$之上的$A'/m'$的素理想；由于$A'/m'$是整环，证明的第一个部分证明存在$A'/m'$的素理想$n'$，使得$n' \cap h(A) = h(p)$和$h(q') \supset n'$。理想 $p' = h^{-1}(n')$ 是 $A'$ 和 $q' \supset p'$ 的素理想，因为 $h$ 的 $q'$ 包含核。如$n' \supset h(p)$、$p' \supset p$。最后，对于$x \in p' \cap A$，$h(x) \in n' \cap h(A) = h(p)$，因此$x \in p$，因为$h$到$A$的限制是单射的；因此$p' \cap A = p$。

#### 推论 {#ac-v-s2-n4-cor-1 .statement tag=04QL}

在定理 3 的$A$和$A'$的假设下，令$p$为$A$的素理想。 $p$之上的$A'$素理想是$A'$包含$pA'$素理想中集合$\mathscr{E}$的最小值元素。

位于$p$之上的$A'$的素理想在$\mathscr{E}$中是最小的，因为no. 1，推论1到命题1。相反，让$q'$是$\mathscr{E}$的最小元素。如$q' \cap A \supset p$、定理 3 所示，存在$A'$ 的素理想$p'$ 位于$p$ 之上，使得$q' \supset p'$。由于$p'$包含于$pA'$，假设在$q'$上生成意味着$q' = p'$，因此$q'$位于$p$之上。

\* 令$V, V'$为两个仿射代数簇，且$V'$至$V$的$f$态射，使得$f(V')$在$V$中稠密。令$A$（或$A'$）为$V$（或$V'$）上常规函数的环；被赋予$f$后，我们可以确定$A$，子环为$A'$；假设$A'$是$A$的积分。 no. 1 的定理 1 表明，对于 V 的每个不可约子簇 W，都存在 V' 的不可约子簇 W'，使得 f(W') 是 W 的稠密子集；特别是，V 的每个点都是 V' 的不可约子簇的像，这表明 f 是满射的。类似地，f 的限制到 V' 的每个不可约子品种 W' 映射 W' 到 V 的不可约子品种。推论 2 到定理 1，no. 1 表明，如果 W 和 X 是 V 的两个不可约子品种，使得 W ⊃ X 并且如果 W' 是 V 的不可约子品种V' 使得 f(W') = W，则存在包含在 W' 中的 V' 的不可约子簇 X'，并且使得 f(X') = X。

如果 A 是整闭的，则 V 称为正规的。 定理 3 表明，如果 V 是正规的，如果 W 和 X 是 V 的不可约子变体，使得 W ⊃ X 并且如果 X' 是 V' 的不可约子变体，使得 f(X') = X，则存在 V' 包含于 X' 的子变体 W'，并且使得 f(W') = W。最后，推论定理 3 表明，如果 V 是正规的并且 W 是 V 的不可约子簇，则 V' 的不可约子簇 W' 使得 f(W') = W 只是 $\overline{f}(W)$ 的不可约分量。

### 习题{#ac-v-s2-exercises}

§ 2](exercises/s2/)参见[习题。
