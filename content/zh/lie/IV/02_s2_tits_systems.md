---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 2
section_title: Tits Systems
lang: zh
source: lie-iv-vi
pdf_pages: 0028-0039, 0057-0072
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS AND FIRST PROPERTIES
      page: 0
      pdf_page: 28
    - "no": 2
      title: AN EXAMPLE
      page: 0
      pdf_page: 30
    - "no": 3
      title: DECOMPOSITION OF G INTO DOUBLE COSETS
      page: 0
      pdf_page: 31
    - "no": 4
      title: RELATIONS WITH COXETER SYSTEMS
      page: 0
      pdf_page: 32
    - "no": 5
      title: SUBGROUPS OF G CONTAINING B
      page: 0
      pdf_page: 34
    - "no": 6
      title: PARABOLIC SUBGROUPS
      page: 0
      pdf_page: 35
    - "no": 7
      title: SIMPLICITY THEOREMS
      page: 0
      pdf_page: 36
statements: 30
exercises: 29
content_sha256: 245354b9720ef5f7eea32f58c6def3d30a085856b760ae1e23e5913ac82ced09
translated_from: content/en/lie/IV/02_s2_tits_systems.md
translation_method: google
source_content_sha256: d7aeccab1a27d0a0619f437c65961e9feffe9a183de0171b993a7c7681af0384
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: ef345c0a68298bb22cf70e53958a36b3cadbb9b157cb7dc199704cb4cbba542b
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。奶系统

本段中字母 G、B、N、S、T、W 的含义见下文no. 1。

### 1. 定义和第一批房产

令 G 为 G 的群，B 子群。群 $B \times B$ 通过 $(b, b').g = bg{b'}^{-1}$ 对 $b, b' \in B$ 和 $g \in G$ 作用于 G。 G 上$B \times B$的轨道对于$g \in G$来说是集合$BgB$，并且被称为G关于B的双陪集。它们是G的形式划分； 相应的商由$B \backslash G / B$表示。如果C和$C'$是双陪集，则$CC'$是双陪集中的并。

#### 定义 1 {#lie-iv-s2-def-1 .statement tag=0AN8}

A Tits 系统是四元数$(G, B, N, S)$，其中G是群，B和N是G的两个子群，S是$N/(B \cap N)$的子集，满足以下公理：

(T1) 集合 $B \cup N$ 生成 G 和 $B \cap N$ 是 N 的正规子群。
(T2) 集合 S 生成群 $W = N/(B \cap N)$ 并由元素阶 2 组成。
(T3) $sBw \subset BwB \cup BswB$ 代表 $s \in S$ 和 $w \in W$。
(T4) 对于所有$s \in S$、$sBs \notin B$。

群$W = N/(B \cap N)$被有时称为山雀系统$(G, B, N, S)$的韦尔群。

5 W 的每个元素都是模$B \cap N$ 的陪集，因此是 G 的子集；因此乘积例如 $BwB$ 是有意义的。更一般地，对于 W 的任意子集 A，我们用 BAB 子集 $\bigcup_{w \in A} BwB$ 表示。

#### 注 1 {#lie-iv-s2-n1-rem-1 .statement tag=0AN9}

我们将在no. 5（Th.3的Cor.）中看到，如果给定$(G, B, N)$，则$N/(B \cap N)$中最多存在一个子集$S$，使得$(G, B, N, S)$是山雀系统。

#### 注 2 {#lie-iv-s2-n1-rem-2 .statement tag=0ANA}

令$(G, B, N, S)$为山雀系统，并令$Z$为包含在$B$中的$G$的正常子群。令$G' = G/Z, B' = B/Z, N' = N/(Z \cap N)$，并令$S'$为$N'/(B' \cap N')$中$S$的像。然后人们立即看到$(G', B', N', S')$是一只山雀系统。

在本段中，$(G, B, N, S)$表示山雀系统，我们集合$T = B \cap N$和$W = N/T$。 双陪集意味着$G$相对于$B$的双陪集。对于任何$w \in W$，我们集合$C(w) = BwB$；这是双陪集。

我们将推导出公理 (T1) 到 (T4) 的几个初等推论。我们用$W$的$w, w', \ldots$元素和$s, s', \ldots$元素表示$S$。以下关系是明确的：

$$
C(1) = B, \quad C(ww') \subset C(w).C(w'), \quad C(w^{-1}) = C(w)^{-1}.
$$

公理 (T3) 也可以写成形式

$$
C(s).C(w) \subset C(w) \cup C(sw).
$$

此外，由于 $C(sw) \subset C(s).C(w)$ 通过 (1) 且$C(s).C(w)$ 是双陪集的并，因此只有两种可能性：

$$
C(s).C(w) = \begin{cases}
C(sw) & \text{if } C(w) \not\subset C(s).C(w) \\
C(w) \cup C(sw) & \text{if } C(w) \subset C(s).C(w).
\end{cases}
$$

(T4) 出发，$B \neq C(s).C(s)$；将$w = s$代入(3)并使用关系$s^2 = 1$，我们得到

$$
C(s).C(s) = B \cup C(s).
$$

这个公式表明$B \cup C(s)$是$G$的子群。将右边的(4)两边乘以$C(w)$，并使用公式(3)和关系

$$
B.C(w) = C(w),
$$

我们得到

$$
C(s).C(s).C(w) = C(w) \cup C(sw).
$$

将集合取逆代入公式(2)、(3)、(5)，再乘以$w^{-1}$替换$w$，可得公式

$$
C(w).C(s) \subset C(w) \cup C(ws)
$$
$$
C(w).C(s) = \begin{cases}
C(ws) & \text{if } C(w) \not\subset C(w).C(s) \\
C(w) \cup C(ws) & \text{if } C(w) \subset C(w).C(s)
\end{cases}
$$
$$
C(w).C(s).C(s) = C(w) \cup C(ws).
$$

#### 引理 1 {#lie-iv-s2-lem-1 .statement tag=0ANB}

设 $s_1, \ldots, s_q \in S$ 并设 $w \in W$。我们有
$$
C(s_1 \ldots s_q).C(w) \subset \bigcup_{(i_1, \ldots, i_p)} C(s_{i_1} \ldots s_{i_p} w),
$$
其中 $(i_1, \ldots, i_p)$ 表示区间 $[1, q]$ 中严格递增的序列的集合整数。

我们通过归纳对$q$进行争论，$q = 0$的情况是微不足道的。如果$q \geqslant 1$，我们有$C(s_1 \ldots s_q).C(w) \subset C(s_1).C(s_2 \ldots s_q).C(w)$。到归纳假设，$C(s_2 \ldots s_q).C(w)$包含在$C(s_{j_1} \ldots s_{j_p} w)$的并中，其中
$$
2 \leq j_1 < \cdots < j_p \leq q.
$$
通过(T3)，集合$C(s_1).C(s_{j_1} \ldots s_{j_p} w)$包含在集合$C(s_1 s_{j_1} \ldots s_{j_p} w)$和$C(s_{j_1} \ldots s_{j_p} w)$的并中。这就证明了引理。

### 2. AN 例

令$k$为域，$n$整数$\geq 0$，$(e_i)$典范基为$k^n$。令$G = \mathbf{GL}(n, k)$，令$B$为$G$的上三角子群，令$N$为矩阵的$G$由……组成的子群，每一行中恰好有一个非零元素， 列。 $N$ 的元素排列$ke_i$ 行；这就产生了满同态$N \to \mathscr{S}_n$，其核是对角线矩阵的子群$T = B \cap N$，并且允许我们用$\mathscr{S}_n$来计算认同$W = N/T$。我们用$W$相应的的$s_j$($1 \leq j \leq n-1$)元素表示$j$和$j+1$的转置；设$S$为$s_j$的集合。 *四倍* $(G, B, N, S)$ *是奶系统*。确实：

Axiom (T1) 源自 Cor。 *代数* 第 14 号提案第 2 条II, § 10, no. 13。

公理 (T2) 在*代数*，第 1 章中得到证明。 I，更正p. 97。
公理 (T4) 是直接的。
仍有待验证公理（T3），即
$$
s_j B w \subset B w B \cup B s_j w B \quad \text{for } 1 \leq j \leq n-1, w \in W,
$$
或同等地，
$$
s_j B \subset B B' \cup B s_j B', \quad \text{with } B' = w B w^{-1}.
$$
设$G_j$为$G$由……组成或元素的子群，将$e_i$固定为$i \neq j, j+1$，并稳定$e_j$和$e_{j+1}$所跨越的平面；这个群与$\mathbf{GL}(2, k)$同构的。一个人检查$G_j B = B G_j$。从$s_j \in G_j$开始，我们有$s_j B \subset B G_j$，这足以证明
$$
G_j \subset (B \cap G_j)(B' \cap G_j) \cup (\cap G_j) s_j (B' \cap G_j).
$$
认同 $G_j$ 与 $\mathbf{GL}(2, k)$；然后，群 $B \cap G_j$ 与$\mathbf{GL}(2, k)$ 的上三角子群 $B_2$ 进行识别，而群 $B' \cap G_j$ 在$w(j) < w(j+1)$ 时与$B_2$ 以及下三角子群进行识别$B_2^-$ 否则。第一种情况，需要证明的公式可以写成

$$
\mathbf{GL}(2, k) = B_2 \cup B_2 s B_2 \quad \text{where } s = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix};
$$

对于例，这是因为在射影线$\mathbf{P}_1(k)$上，对于$\mathbf{GL}(2, k)$的作用，$B_2$是点的稳定子，并且传递地作用于该点的补集。在第二种情况下，需要证明的公式可以写成

$$
\mathbf{GL}(2, k) = B_2 B_2^- \cup B_2 s B_2^-;
$$

从$B_2^- = s B_2 s$开始，这是前面的公式通过在右侧乘以$s$得出的。

### 3. G 的分解变成双陪集

#### 定理 1 {#lie-iv-s2-thm-1 .statement tag=0ANC}

*我们有$G = \mathrm{BWB}$。 映射$w \mapsto C(w)$是$W$到集合$B \backslash G / B$的$G$相对于$B$的双陪集的双射。*

显然，$\mathrm{BWB}$在$x \mapsto x^{-1}$下是稳定的，引理1表明在乘积下是稳定的。由于它包含$B$和$N$，所以它等于$G$。

仍有待证明 $C(w) \neq C(w')$ if $w \neq w'$。为此，我们将通过归纳对整数$q$证明以下断言：

(A_q) 如果$w$和$w'$不同于$W$的元素，使得$l_S(w) \geq l_S(w') = q$，则$C(w) \neq C(w')$。

（对于$l_S(w)$中的定义，请参阅§ 1, no. 1。）

这个断言对于$q = 0$来说是明确的，从那时起$w' = 1$和$w \neq 1$，因此$C(w') = B$和$C(w) \neq B$。

假设 $q \geq 1$ 和 $w, w'$ 满足 (A_q) 的假设。存在$s \in S$使得$sw'$是长度$q - 1$。我们有

$$
l_S(w) > l_S(sw')
$$

因此$w \neq sw'$。此外，$sw \neq sw'$；通过 § 1, no. 1 的公式 (3)，我们有

$$
l_S(sw) \geq l_S(w) - 1 \geq l_S(sw') = q - 1.
$$

通过归纳假设，$C(sw')$不同于$C(w)$和$C(sw)$；由公式 (2) 可知

$$
C(sw') \cap C(s).C(w) = \varnothing.
$$

从$C(sw') \subset C(s).C(w')$开始，我们终于有了$C(w) \neq C(w')$。

#### 注 {#lie-iv-s2-n3-rem-1 .statement tag=0AND}

前面的证明中没有使用Axiom（T4）。

### 4. 关系与考克塞特系统

#### 定理 2 {#lie-iv-s2-thm-2 .statement tag=0ANE}

对 $(W, S)$ 是 Coxeter 系统。此外，对于$s \in S$和$w \in W$，关系$C(sw) = C(s).C(w)$和$l_S(sw) > l_S(w)$是等价的。

对于任何$s \in S$，令$P_s$为元素$w \in W$中的集合，使得
$$
C(s).C(w) = C(sw).
$$
我们要验证§ 1, no. 7的$P_s$满足条件（A'），（B'）和（C）； 定理的两个断言将遵循§ 1, no. 7的第6条命题。

条件 (A') 清晰。

我们验证（B'）。如果$P_s$和$sP_s$在公共的中有元素$w$，我们就会有$w \in P_s$和$sw \in P_s$，因此
$$
C(s).C(w) = C(sw), \qquad C(s).C(sw) = C(w).
$$
由此得出$C(s).C(s).C(w) = C(w)$，并且通过公式 (5)，这将意味着$C(w) = C(sw)$，这将与 Th 相矛盾。 1.

我们验证（C）。让$s, s' \in S$和$w, w' \in W$与$w' = ws'$。 假设 $w \in P_s$ 和 $w' \notin P_s$ 意味着
$$
C(sw) = C(s).C(w) \tag{9}
$$
$$
C(w') \subset C(s).C(w') \tag{10}
$$
由（3）。

由 (9) 和关系 $w = w's'$ 可知
$$
C(s)w's'B = C(sw). \tag{11}
$$
通过公式 (2'), $C(w').C(s') \subset C(w') \cup C(w's')$，这立即意味着
$$
C(w')s'B \subset C(ws') \cup C(w). \tag{12}
$$
因为 $C(w')$ 是左陪集 $gB$ 的并并且因为
$$
C(s).C(w') = C(s)w'B,
$$
公式 (10) 表明$C(s)w'$ 满足$C(w')$ 并且*更不必说* $C(s)w's'B$ 满足$C(w')s'B$。从公式 (11) 和 (12) 可以得出，双陪集 $C(sw)$ 等于双陪集 $C(ws')$ 和 $C(w)$ 之一；从 $sw \neq w$ 开始1 允许我们结论 $sw = ws'$。

#### 推论 1 {#lie-iv-s2-thm-2-cor-1 .statement tag=0ANF}

*让*$w_1, \ldots, w_q \in W$*并让*$w = w_1 \ldots w_q$。 *如果*
$$
l_S(w) = l_S(w_1) + \cdots + l_S(w_q),
$$
*然后*
$$
C(w) = C(w_1) \ldots C(w_q).
$$

在取 $w_i$ 的减少的分解时，减少到减少的分解的情况

$$
w = s_1 \ldots s_q, \quad \text{with } s_i \in S.
$$

如果$u = s_2 \ldots s_q$，则$w = s_1 u$和$l_S(s_1 u) > l_S(u)$，因此$C(w) = C(s_1).C(u)$乘以定理。所需的公式由 $q$ 上的归纳得出。

#### 推论 2 {#lie-iv-s2-thm-2-cor-2 .statement tag=0ANG}

*令$w \in W$和$T_w$为通过§ 1, no. 4的引理2的过程与$w$相关联的$W$的子集。如果$t \in T_w$，那么*

$$
C(t) \subset C(w).C(w^{-1}).
$$

如果 $t \in T_w$，则存在定义元素 $w', w'' \in W$ 和 $s \in S$ 使得

$$
w = w' s w'', \quad l_S(w) = l_S(w') + l_S(w'') + 1 \quad \text{and} \quad t = w' s {w'}^{-1}.
$$

由科. 1、

$$
C(w).C(w^{-1}) = C(w').C(s).C(w'').C({w''}^{-1}).C(s).C({w'}^{-1}).
$$

因此，

$$
C(w).C(w^{-1}) \supset C(w').C(s).C(s).C({w'}^{-1}).
$$

由 (4)，$C(s) \subset C(s).C(s)$。因此，

$$
C(w).C(w^{-1}) \supset C(w').C(s).C({w'}^{-1}) \supset C(t).
$$

#### 推论 3 {#lie-iv-s2-thm-2-cor-3 .statement tag=0ANH}

*令$w \in W$且$H_w$为由$C(w).C(w^{-1})$生成的$G$的子群。然后：*

a) *对于任何减少的分解 $(s_1, \ldots, s_q)$ 或 $w$，*

$$
C(s_j) \subset H_w \quad \text{for } 1 \leq j \leq q.
$$

b) *群 $H_w$ 包含于 $C(w)$ 由$C(w)$生成。*

我们通过归纳在$j$上证明a)。假设对于$k < j$，$C(s_k)$包含在$H_w$中。让

$$
t = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1}.
$$

$W$的元素$t$属于至子集$T_w$在§ 1, no. 4的引理2中定义。由科. 2、$C(t) \subset H_w$，因此$C(s_j) \subset H_w$。

从 $C(w) = C(s_1) \ldots C(s_q)$ 开始，cf. Cor. 1，我们有$C(w) \subset H_w$，b)如下。

#### 例 {#lie-iv-s2-n4-exa-1 .statement tag=0ANI}

Th。 2，应用于no. 2中描述的山雀系统，表明*对称群*$\mathfrak{S}_n$，其中集合是连续元素的转置，*是Coxeter群*。

### 5. 子群 G 包含于 B

对于 S 的任何子集 X，我们用 X (cf. §1, no. 8) 生成的 W 的 W_X 子群和双陪集 C(w) 的 G_X 并 BW_XB 表示，w ε W_X。我们有 G_∅ = B 且 G_S = G。

#### 定理 3 {#lie-iv-s2-thm-3 .statement tag=0ANJ}

a) 对于 S 的任意子集 X，集合 G_X 是由 $\bigcup_{s \in X} C(s)$ 生成的 G 的子群。

b) 映射X↦G_X是G包含B的子群的$\mathscr{P}(S)$到集合双射。

c) 令 (X_i)_{i \in I} 为子集和 X 的族。如果$X = \bigcap_{i \in I} X_i$，则$G_X = \bigcap_{i \in I} G_{X_i}$。

d) 令X和Y为S的两个子集。则$G_X \subset G_Y$（或$G_X = G_Y$）当且仅当$X \subset Y$（或$X = Y$）。

显然$G_X = (G_X)^{-1}$； 引理 1 of no. 1 表明$G_X . G_X \subset G_X$；因此a)如下，考虑到Cor。 1 Th。 2.

X ↦ G_X 的单射性源自 X ↦ W_X (§1, no. 8, Th. 2)。相反，令 H 为 G 包含 B 的子群。令 U 为 $w \in W$ 的集合，使得 $C(w) \subset H$。我们有$H = BUB$，因为H是双陪集的并。设 $X = U \cap S$；我们证明$H = G_X$。显然，$G_X \subset H$。另一方面，令 $u \in U$ 和$(s_1, \ldots, s_q)$ 为 u 的约化分解。科。 3 Th。 2 意味着 $C(s_j) \subset H$，因此 $s_j \in X$ 代表 $1 \leq j \leq q$。因此，$u \in W_X$，并且由于 $u \in U$ 的 H 是 $C(u)$ 的并，所以我们有 $H \subset G_X$，这证明了 b)。

断言 c) 和 d) 源自 W_X (§ 1, no. 8, Th. 2) 的类似属性。

#### 推论{#lie-iv-s2-n5-cor-1 .statement tag=0ANK}

集合 S 由元素 $w \in W$ 组成，使得 $w \neq 1$ 和 $B \cup C(w)$ 是 G 的子群。

元素$w \in W$使得$B \cup C(w)$是G的子群是那些存在$X \subset S$和$W_X = \{1, w\}$的。此外，如果$w \neq 1$，我们必然有 Card(X) = 1 ，即$w \in S$。

#### 注 1 {#lie-iv-s2-n5-rem-1 .statement tag=0ANL}

上述推论表明，S由(G,B,N)决定；因此，我们有时允许自己说（G，B，N）是G中的山雀系统，或者（B，N）是G中的山雀系统。

#### 命题 1 {#lie-iv-s2-prop-1 .statement tag=0ANM}

令 X 为 S 的子集，N' 子群为 N，其中 W 中的像等于 W_X。那么，(G_X, B, N', X) 就是一个 Tits 系统。

我们有$G_X = BW_XB = BN'B$，这表明$G_X$是由$B \cup N'$生成的。 公理（T1）到（T4）的验证现在是直接的。

#### 命题 2 {#lie-iv-s2-prop-2 .statement tag=0ANN}

设 X，Y ⊂ S 和 $w \in W$。我们有

$$
G_X w G_Y = BW_X w W_Y B.
$$

设$s_1, \ldots, s_q \in X$和$t_1, \ldots, t_q \in Y$。 引理 1 表明
$$
C(s_1 \ldots s_q).C(w).C(t_1 \ldots t_q) \subset BW_X w W_Y B,
$$
因此
$$
G_X w G_Y \subset BW_X w W_Y B.
$$
相反的包容性是显而易见的。

#### 注 2 {#lie-iv-s2-n5-rem-2 .statement tag=0ANO}

用形式$G_X g G_Y$$G$子集$G_X \backslash G / G_Y$集合、$g \in G$表示；和定义 $W_X \backslash W / W_Y$ 类似。前面的命题显示了从 $W$ 到 $B \backslash G / B$ 定义通过商 a *双射* $W_X \backslash W / W_Y \to G_X \backslash G / G_Y$ 的规范双射 $w \mapsto C(w)$。

#### 命题 3 {#lie-iv-s2-prop-3 .statement tag=0ANP}

*设$X \subset S$和$g \in G$。 关系 $g B g^{-1} \subset G_X$ 意味着 $g \in G_X$.*

设$w \in W$使得$g \in C(w)$。 Since $B$ is a subgroup of $G_X$, the hypothesis $g B g^{-1} \subset G_X$ implies that $C(w).C(w^{-1}) \subset G_X$, and hence that $C(w) \subset G_X$ by Cor. 3 of Th. 2, so $g$ belongs to $G_X$.

### 6. 抛物线子群

#### 定义 2 {#lie-iv-s2-def-2 .statement tag=0ANQ}

*如果$B$的包含共轭，则称$G$的子群为抛物线。*

显然，每个子群包含都是抛物线子群都是抛物线。

#### 命题 4 {#lie-iv-s2-prop-4 .statement tag=0ANR}

*令$P$为$G$的子群。*

a) *$P$ 是抛物线当且仅当存在 $S$ 的子集 $X$ 且 $P$ 为共轭到 $G_X$（对于 $G_X$ 的定义，cf. no. 5）。*

b) *设$X, X' \subset S$和$g, g' \in G$使得$P = g G_X g^{-1} = g' G_{X'} {g'}^{-1}$。然后，$X = X'$和$g' g^{-1} \in P$。*

断言 a) 由 Th 得出。 3、b）。
在 b) 的假设下，我们有
$$
g^{-1} g' B {g'}^{-1} g \subset g^{-1} g' G_{X'} {g'}^{-1} = G_X,
$$
命题 3 表明$g^{-1} g' \in G_X$。因此，Th 为 $G_{X'} = G_X$ 和 $X' = X$。 3、b）。最后，
$$
g' g^{-1} = g . g^{-1} g' . g^{-1} \in g G_X g^{-1},
$$
这就证明了b)。

如果抛物线子群 $P$ 为共轭到 $G_X$，其中 $X \subset S$，则 $P$ 被称为 *型 X*。

#### 定理 4 {#lie-iv-s2-thm-4 .statement tag=0ANS}

(i) 令$P_1$和$P_2$是$G$的两个抛物线子群，其中交是抛物线，并令$g \in G$使得$gP_1g^{-1} \subset P_2$。然后是$g \in P_2$和$P_1 \subset P_2$。

(ii) 两个抛物线子群且交是抛物线，则不是共轭。

(iii) 设$Q_1$和$Q_2$为包含在$G$的子群$Q$中的$G$的两个抛物线子群。然后任意$g \in G$使得$gQ_1g^{-1} = Q_2$属于到$Q$。

(iv) 每个抛物线子群都是其自己的归一化器$^6$。

断言 (i) 来自 Props。 3和4，并暗示(ii)。在(iii)的假设下，我们有$gQ_1g^{-1} \subset Q$，这意味着$g \in Q$乘以(i)。最后，(iv) 由 (iii) 得出 $Q_1 = Q_2 = Q$。

#### 命题 5 {#lie-iv-s2-prop-5 .statement tag=0ANT}

令$P_1$和$P_2$为$G$的两个抛物线子群。然后$P_1 \cap P_2$包含共轭共$T$。

首先将$P_1$和$P_2$变换为$G$的内自同构，我们可以假设$B \subset P_1$。令$g \in G$ 使得$gB_2g^{-1} \subset P_2$。由 Th. 1、存在$n \in N$和$b, b' \in B$使得$g = bn b'$。由于$T$在$N$中是正常的，

$$
P_2 \supset gB_2g^{-1} = bnBn^{-1}b^{-1} \supset bnTn^{-1}b^{-1} = bTb^{-1}
$$

和

$$
P_1 \supset B \supset bTb^{-1},
$$

这就证明了命题。

### 7. 简单定理

#### 引理 2 {#lie-iv-s2-lem-2 .statement tag=0ANU}

令$H$为$G$的正常子群。存在$S$的子集$X$使得$BH = G_X$并且使得$X$的每个元素与$S - X$的每个元素交换。

由于$BH$是$G$包含于$B$的子群，因此存在$S$的唯一子集$X$，使得$BH = G_X$（Th.3）。

设$s_1 \in X$和$s_2 \in S - X$；设$n_1$和$n_2$分别为$s_1$和$s_2$中$N$的代表。那么$n_1 \in G_X = BH$并且存在$b \in B$使得$bn_1 \in H$。由于$H$在$G$中是正常的，所以$G$属于到$H$中的元素$h = n_2 b n_1 n_2^{-1}$。这意味着

$$
h \in C(s_2).C(s_1).C(s_2).
$$

如果 $s_2 s_1 s_2$ 的长度等于 3，Cor. 1 Th。 2 意味着

$$
C(s_2).C(s_1).C(s_2) = C(s_2 s_1 s_2),
$$

(6) 如果$H$是群$G$的子群，则$G$中$H$的归一化器是元素$g$的子群$\mathfrak{N}(H)$由……组成 $G$使得$gHg^{-1} = H$。如果 $H' \subset \mathfrak{N}(H)$，子群 $H'$ 据说可以标准化 $H$，在这种情况下，$HH' = H'H$ 是 $G$ 的子群，其中 $H$ 是正常的。

因此$h \in H \cap C(s_2 s_1 s_2)$。由于$H \cap C(s_2 s_1 s_2)$非空，因此$s_2 s_1 s_2 \in W_X$。由于$(s_2, s_1, s_2)$是缩小的分解，因此得出$s_2 \in X$，与我们的假设相反。

因此$l_S(s_2 s_1 s_2) \leq 2$；如果$l_S(s_2 s_1 s_2) = 1$，则$s_1 s_2 \in S$，如此$(s_1 s_2)^2 = 1$，或$s_1 s_2 = s_2 s_1$。如果$l_S(s_2 s_1 s_2) = 2$，§1, no. 5的性质（E）意味着$s_2 s_1 = s_1 s_2$，因为$s_1 \neq s_2$。 Q.E.D.

群 U 的以下性质进入Th。 5 如下：

(R) *对于任何不同于 U 的正常子群 V，换位子子群*（cf. *代数*，第 I, §6, no. 8）*U/V 与 U/V* 不同。

每个可溶群满足(R)；特别地，每个阿贝尔的群满足(R)。可以证明对称群$\mathfrak{S}_n$满足(R)(cf.Exerc.29)。

#### 定理 5 {#lie-iv-s2-thm-5 .statement tag=0ANV}

*设Z为B的共轭的交，设U为B的子群，设G_1为G中U的共轭生成的子群。我们得到以下假设：*

(1) *U 在 B 中是正规的且 B = UT*。
(2) *U 有性质 (R)*。
(3) *G_1 等于其换位子子群*。
(4) *Coxeter 系统 (W, S) 不可约* (cf. §1, no. 9)。

*那么G_1归一化的G的每个子群H要么包含在Z中，要么包含在包含G_1*中。

*首先我们证明 G = G_1 T*。 群 $G_1 T$ 包含于 B，因此是它自己的标准化器（Th. 4）；但当 N 标准化 $G_1$ 和 T 时，它也标准化 $G_1 T$，因此$N \subset G_1 T$。由于G是由B和N生成的，因此有$G = G_1 T$。

*下一个，集合*

$$
G' = G_1 H, \quad B' = B \cap G', \quad N' = N \cap G',
T' = T \cap G' = B' \cap N' \quad \text{and} \quad W' = N'/T'.
$$

从 $G'$ 包含于 $G_1$ 开始，我们有 $G = G'T$，因此有 $N = N'T$。将$N'$包含在N中，因此定义，在经过上商，同构$\alpha : W' \to W$。让$S' = \alpha^{-1}(S)$。

*我们现在证明 (G', B', N', S') 是山雀系统*。从$G = BNB$和$B = TU = UT$开始，我们有$G = UNU$。由于U是$G'$的子群，因此有$G' = UN'U$；从$U \subset B'$开始，这证明了(T1)。公理 (T2) 满足，因为 $\alpha$ 是同构。令 $w \in W$ 且令 $w' = \alpha^{-1}(w)$ 为 $W'$ 的相应的元素。我们有

$$
BwB = BwB' = Bw'B', \quad \text{since } B = B'T.
$$

由此我们结论得出$G' \cap BwB = B'w'B'$，这意味着将$G'$包含在经过上的G 定义与双射的商

B'\setminus G'/B' 到 B\setminus G/B。 Axiom (T3) 紧随其后。公理 (T4) 由 B = B'T 得出。

子群 H 在 G' 中是正规的。将引理 2 应用于 (G', B', N', S')，存在 S' 的子集 X'，使得 B'H = G'_X'，并且 S' 的每个元素 - X' 与 X' 的每个元素进行交换。鉴于假设(4)，只有两种可能：

a) X' = \varnothing，即 B'H = B'，所以 H \子集 B' \子集 B。如果 g \in G，则 g = g_1 t，g_1 \in G_1，t \in T，并且 H \子集 g_1 B g_1^{-1} 因为 G_1 标准化了 H。因此 H \子集 g B g^{-1}，并且由于 Z 是 g B g^{-1} 的交，所以我们有 H \子集 Z。

b) X' = S'，即 B'H = G'。由于 G = G'T，我们有

$$ G = B'HT = HB'T = HB. $$

当 B 对 U 进行归一化时，U 的每个共轭都是形式 hUh^{-1}，其中 h \in H。这样的子群包含在群 UH 中，因此 G_1 \子集 UH 乘以 G_1 的定义。因此，我们有同构

$$ U/(U \cap H) \cong UH/H = G_1 H/H \cong G_1/(G_1 \cap H). $$

通过假设 (3)，G_1/(G_1 \cap H) 等于其换位子子群。 假设 (2) 现在显示群 U/(U \cap H)，它同构于 G_1/(G_1 \cap H)、约化到单位元素。因此 G_1 \cap H = G_1 和 G_1 \子集 H，完成证明。

#### 推论{#lie-iv-s2-n7-cor-1 .statement tag=0ANW}

Th 假设以下。 5、 群 G_1/(G_1 \cap Z) 要么是简单非交换矩阵，要么是约化到单位元素。

Th。图 5 显示 G_1/(G_1 \cap Z) 是简单的或约化到单位元素。另一方面，假设(3)意味着它等于它的换位子子群。由此得出推论。

#### 注 1 {#lie-iv-s2-n7-rem-1 .statement tag=0ANX}

假设 (2), (3), (4) 未在证明中使用，即 (G', B', N', S') 是山雀系统。

#### 注 2 {#lie-iv-s2-n7-rem-2 .statement tag=0ANY}

假设 Z \cap U = \{1\}。由于 Z 和 U 在 B 中是正规的，因此 Z 的每个元素与 U 的每个元素交换，因此与 G_1 的每个元素交换。鉴于前面的推论，G_1 \cap Z 是 G_1 的中心。

#### 注 3 {#lie-iv-s2-n7-rem-3 .statement tag=0ANZ}

假设 (3) 由以下条件隐含：

(3') U 由换位子 b^{-1} u^{-1} b u 生成，其中 u \in U 和 b \in B \cap G_1。

#### 例 1 {#lie-iv-s2-n7-exa-1 .statement tag=0AO0}

令 k 为域，n 整数 \geqslant 0，G = \mathbf{GL}(n, k)，并令 (G, B, N, S) 为 no. 2 中描述的山雀系统。令U为G的严格上三角子群，即矩阵的B由……组成的子群，其对角线条目等于1。Th中的条件 (1)。 5 是直接的，(2) 也是如此，因为 U 是可溶的。如果$n \geq 2$则满足条件(4)。可以证明（cf. *代数*，第 II, § 10 章，练习 13），如果 $n \geq 3$ 和 Card$(k) \geq 4$，则满足 (3)。在这些条件下，我们结论认为$G_1 / (G_1 \cap Z)$是*简单的*并且$G_1 \cap Z$是$G_1$的中心（cf.*注*2）。

当 $k$ 可交换时，$G_1 = \mathbf{SL}(n, k)$ (cf. *代数*，第 III, § 8, no. 9)。

#### 例 2 {#lie-iv-s2-n7-exa-2 .statement tag=0AO1}

令$g$为$\mathbf{C}$上的简单李代数，并令$G$为$g$的内自同构的群（cf.第III, § 6, no. 2章，第2条）。通过使用 Th. 5, 可以证明 $G$ 是简单非交换矩阵。*

### 习题{#lie-iv-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
