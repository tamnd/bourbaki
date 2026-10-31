---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 2
section_title: Flat modules
lang: zh
source: ac-i-vii
book_pages: 9-27, 41-49
pdf_pages: 0029-0047, 0061-0069
extraction: ocr
subsections:
    - "no": 1
      title: REVISION OF TENSOR PRODUCTS
      page: 9
      pdf_page: 29
    - "no": 2
      title: M-FLAT MODULES
      page: 10
      pdf_page: 30
    - "no": 3
      title: FLAT MODULES
      page: 12
      pdf_page: 32
    - "no": 4
      title: EXAMPLES OF FLAT MODULES
      page: 14
      pdf_page: 34
    - "no": 5
      title: FLATNESS OF QUOTIENT MODULES
      page: 15
      pdf_page: 35
    - "no": 6
      title: INTERSECTION PROPERTIES
      page: 17
      pdf_page: 37
    - "no": 7
      title: TENSOR PRODUCTS OF FLAT MODULES
      page: 19
      pdf_page: 39
    - "no": 8
      title: FINITELY PRESENTED MODULES
      page: 20
      pdf_page: 40
    - "no": 9
      title: EXTENSION OF SCALARS IN HOMOMORPHISM MODULES
      page: 22
      pdf_page: 42
    - "no": 10
      title: 'EXTENSION OF SCALARS: CASE OF COMMUTATIVE RINGS'
      page: 22
      pdf_page: 42
    - "no": 11
      title: INTERPRETATION OF FLATNESS IN TERMS OF RELATIONS (*)
      page: 25
      pdf_page: 45
statements: 37
exercises: 24
content_sha256: f7707a1a1b62be6e2544ea8c4a3219c012295e198a0590e243370ebb5bd83cc2
translated_from: content/en/ac/I/02_s2_flat_modules.md
translation_method: google
source_content_sha256: 28d69ca6e99e7466a70edf5b1c736029d397199a01db0537698a81ada5d7fea8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f369edee2b57f650edea98a2f93f2889828d9484d3f7b7f68178ab3a2cdcc46f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2. 扁平模(*)

### 1. 张量积的修订

设 A 为环，E 右A-模，M 左A-模。在代数，章II, §3, no. 1中，我们定义了张量积$E \otimes_A M$，它是一个$\mathbf{Z}$模。如果 E'（分别为 M'）是右（分别为左）A-模和 $u : E \to E'$（分别为 $v : M \to M'$）同态，我们还定义了（loc.cit，no. 2）一个 $\mathbf{Z}$ 同态

$$
u \otimes v : E \otimes_A M \to E' \otimes_A M'.
$$

#### 引理 1 {#ac-i-s2-lem-1 .statement tag=042F}

*令*$M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$*为左A-模和E右A-模中的正合序列。然后序列*

$$
E \otimes_A M' \xrightarrow{\text{1}\otimes v} E \otimes_A M \xrightarrow{u \otimes w} E \otimes_A M'' \longrightarrow 0
$$

*是交换律群的正合序列。*

这是命题 5 of 代数、章 II, § 3, no. 6 的推论。

由此可见，对于任意左A-模同态 $u : M \to N$，

$$
E \otimes_A (\operatorname{Coker} u)
$$

规范地标识为 $\operatorname{Coker}(1_E \otimes u)$，如引理 1 应用于正合序列时所示

$$
M \xrightarrow{u} N \longrightarrow \operatorname{Coker} u \longrightarrow 0.
$$

在引理 1 的记号中，我们知道（前述）如果 v 是*单射*，也就是说，如果序列 $0 \to M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$ 是精确的，则并不一定意味着 $1_E \otimes v$ 是单射的，因此 $E \otimes_A M'$ 不能通常可以用 a

(*) 我们通知已经熟悉同调代数的读者，他们会在§ 4中找到平模的其他刻画。

$E \otimes_A M$ 的子群。然而，回想一下（代数，章II, § 3, no. 7，推论5到命题7）以下结果：

#### 引理 2 {#ac-i-s2-lem-2 .statement tag=042G}

*如果$v : M' \to M$是单射且$v(M')$是$M$的直因子，则同态$1, \otimes v$是单射并且其像是$E \otimes_A M$的直因子。*

### 2. M 平底模

#### 定义 1 {#ac-i-s2-def-1 .statement tag=042H}

令$A$为环，$E$为右$A$模块，$M$为左$A$模块。如果对于每个左 $A$-模 $M'$ 和每个单同态 $v : M' \to M$，同态 $l_E \otimes v : E \otimes_A M' \to E \otimes_A M$ 是单射的，则称 $E$ 对于$M$（或$M$-平坦）是平坦的。

对于任何右$A$-模块$N$，$N$-平面左模的概念的定义类似。说右$A$-模块$E$对于左$A$-模块$M$来说是平坦的，相当于说，$E$，被视为左$A^0$-模块（回想一下，$A^0$表示逆环到$A$)，对于右侧$A^0$模块$M$来说是平坦的。

#### 引理 3 {#ac-i-s2-lem-3 .statement tag=042I}

*对于紧密的$A$模$E$为$M$平坦，对于$M$典范同态的每个有限生成的子模$M'$是必要且充分的*

$$
l_E \otimes j : E \otimes_A M' \to E \otimes_A M
$$

（*j 为典范嵌入 $M' \to M$）*是单射*。

假设条件成立，并令$N$为$M$中的任意子模。假设元素的$E \otimes_A M$中有典范像

$$
z = \sum x_i \otimes y_i \in E \otimes_A N \quad (x_i \in E, y_i \in N)
$$

是零，令$M'$是它们生成的$N$的有限生成的子模；由于假设，复合映射$E \otimes_A M' \to E \otimes_A N \to E \otimes_A M$是单射的，和$z' = \sum x_i \otimes y_i$，被视为$E \otimes_A M'$的元素，是零。 *由于*$z$是$z'$的像，我们还有$z = 0$，从而引理。

#### 引理 4 {#ac-i-s2-lem-4 .statement tag=042J}

*令$E$为右$A$模，$M$为左$A$模，使得$E$为$M$平。如果$N$是子模或商模或$M$，则$E$是$N$平坦。*

$N$ 是子模的情况很简单，因为如果 $N'$ 是 $N$ 的子模，则复合同态

$$
E \otimes_A N' \to E \otimes_A N \to E \otimes_A M
$$

是单射的，因此 $E \otimes_A N' \to E \otimes_A N$ 也是。假设$N$是$M$的商模，即存在正合序列$0 \to R \xrightarrow{i} M \xrightarrow{p} N \to 0$。

设$N'$为$N$和$M' = \overline{p}(N')$的子模。令$i'$表示$R$至$M'$的映射，与$i$相同的图，$p'$表示满射$M \to N'$，与$p$至$M'$的限制相同的图， $\mathbf{R}$至$\mathbf{R}$、$m$典范嵌入$M' \to M$和$n$典范嵌入$N' \to N$的$r$恒等映射。 图表

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i'} & M' & \xrightarrow{p'} & N' & \longrightarrow & 0 \\
& & \downarrow r & & \downarrow m & & \downarrow n & & \\
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i} & M & \xrightarrow{p} & N & \longrightarrow & 0
\end{array}
$$

是可交换的并且它的行是精确的。

为了简化书写，我们对每个左$A$-模块$Q$使用集合$T(Q) = E \otimes_A Q$，对每个左$A$-模块同态$v$使用$T(v) = 1_E \otimes v$。 图表

$$
\begin{array}{ccccccccc}
T(\mathbf{R}) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(N') & \longrightarrow & 0 \\
\downarrow T(r) & & \downarrow T(m) & & \downarrow T(n) & & \\
T(\mathbf{R}) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(N) & \longrightarrow & 0
\end{array}
$$

是可交换的，并且它的行精确到 no. 1 的引理 1。此外，由于 $E$ 是 $M$ 平坦的，因此同态 $T(m)$ 是单射的。由于$T(r)$和$T(p')$是满射，因此从推论2 § 1, no. 4到命题 2，$T(n)$是单射，从而证明了引理。

#### 引理 5 {#ac-i-s2-lem-5 .statement tag=042K}

令$(M_i)_{i \in I}$是左$A$模块、$M = \bigoplus_{i \in I} M_i$、它们的直和和$E$右$A$模块的族。如果对于所有 $i \in I$，$E$ 对于 $M_i$ 是平坦的，那么 $E$ 对于 $M$ 是平坦的。

(a) 首先假设$I = \{1, 2\}$，并令$M'$为$M = M_1 \oplus M_2$、$M$和$M$中的子模，与$M$中的子模进行规范地识别。 用 $M'_1$ 交 $M' \cap M_1$ 表示，并在 $M_2$ 上$M$ 的规范投影 $p$ 下，用$M_2$ 中$M'$ 的$M'_2$ 像表示。 我们有图表

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M'_1 & \xrightarrow{i'} & M' & \xrightarrow{p'} & M'_2 & \longrightarrow & 0 \\
& & \downarrow v_1 & & \downarrow v & & \downarrow v_2 & & \\
0 & \longrightarrow & M_1 & \xrightarrow{i} & M & \xrightarrow{p} & M_2 & \longrightarrow & 0
\end{array}
$$

其中$v_1, v, v_2, i, i'$是典范嵌入，$p'$是映射，与$p$到$M'$的限制相同，这是满射的。立即验证了这个图表是可交换的并且它的行是精确的。 $T(Q)$和$T(v)$的使用与引理4的证明相同，我们有一个可交换的图表

$$
\begin{array}{ccccccccc}
T(M'_1) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(M'_2) \\
\downarrow T(v_1) & & \downarrow T(v) & & \downarrow T(v_2) \\
T(M_1) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(M_2)
\end{array}
$$

通过引理 1 of no. 1，这个图表的两行是精确的；因为 E 对于 $M_1$ 和 $M_n$ 是平的，$T(v_1)$ 和 $T(v_2)$ 是单射的；此外，通过 no. 1 的引理 2，$T(i)$ 是单射的。 § 1, no. 4 的推论 2 到命题 2 则表明 $T(v)$ 是单射的，因而 E 是 M 平的。

(b) 如果 I 是一个有限集合，其中 n 元素，则使用 (a)，引理在 n 上跟随归纳。

(c) 在一般情况下，令$M'$为M的有限生成的子模。则存在索引集合I的有限子集J，使得$M'$包含在直和$M_J = \bigoplus_{i \in J} M_i$中。由 (b) E 对于 $M_J$ 是平坦的； 典范同态 $E \otimes_A M' \to E \otimes_A M$，因此是单射的。另一方面，由于$M_J$是M的直因子，典范同态$E \otimes_A M_J \to E \otimes_A M$是单射的（no. 1，引理2）。取合成，可得出$E \otimes_A M, \to E \otimes_A M$ 是单射且 E 对 M 平展引理 3。

### 3.平模

#### 命题 1 {#ac-i-s2-prop-1 .statement tag=042L}

设E为右A-模。以下三个属性是等效的：

(a) E 对于 A 是平坦的，（在其他字中，对于 A 的每个左理想 $a$，典范同态 $E \otimes_A a \to E \otimes_A A, = E$ 是单射的）。
(b) 对于每左A-模 M，E 是 M 降调。
(c) 对于左A-模和同态中的每正合序列

$$
M' \xrightarrow{v} M \xrightarrow{w} M''
$$

the sequence

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

是准确的。

(b) 蕴涵(a) 是直接的。相反，假设 (a) 成立；通过 no. 2 的引理 5，E 对于每个免费左A-模都是平的；由于每个左A-模都同构于自由模的商（代数、章 11、§ 1, no. 11、命题 20），因此从 no. 2 的引理 4 可以得出，E 对于 M 是平坦的。

我们证明（c）蕴涵（b）。如果$v : M' \to M$是单同态，则序列$0 \to M' \xrightarrow{v} M$是精确的；通过 (c) 序列

$$
0 \to E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M
$$

是准确的；这意味着$1 \otimes v$是单射的，在其他字中，E是M平的。

最后，蕴涵 (b) $\Rightarrow$ (c) 是以下更精确的引理的推论：

#### 引理 6 {#ac-i-s2-lem-6 .statement tag=042M}

*如果$M' \xrightarrow{v} M \xrightarrow{w} M''$是左A-模的正合序列并且如果E是$M''$平右A-模、序列*

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

*准确。*

我们使用记号$T(Q)$和$T(v)$的意义与no. 2的引理4的证明相同。我们写出$M_1'' = w(M)$，并令$i : M_1'' \to M''$为M到$M_1''$的典范嵌入和$p$映射，与w具有相同的图。 序列 $M' \xrightarrow{v} M \xrightarrow{p} M_1'' \to 0$ 是精确的，并且从引理 1 of no. 1 得出序列

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(p)} T(M_1'') \longrightarrow 0
$$

是准确的。此外，由于 E 是 $M''$-平，映射 $T(i) : T(M_1'') \to T(M'')$ 是单射，并且由于 $T(i) \circ T(p) = T(w)$，序列

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(w)} T(M'')
$$

*准确。* (§ 1, no. 3.)

#### 定义 2 {#ac-i-s2-def-2 .statement tag=042N}

*右A-模 E 被称为平坦的，如果*它具有与命题 1 等效的属性。

平面左A-模的定义类似。要说右A-模 E 是平坦的，则相当于说，即 E（被视为左 $A^0$ 模）是平坦的。

Remarks

(1) 通过 no. 2 的引理 3，对于右A-模 E 是平坦的，对于每个“有限”生成 A 的左理想 $a$，典范映射 $E \otimes_A a \to E$ (命题 1) 且像 Ea 是内射的，这是充分必要的。

(2) 设 E 为平右A-模。如果$M'$是左A-模M的子模，典范嵌入$E \otimes_A M' \to E \otimes_A M$允许我们认同$E \otimes_A M'$和子群$E \otimes_A M$。既然如此，令N为左A-模、$u : M \to N$同态、$K = \mathrm{Ker}\, u$和$I = \mathrm{Im}\, u$。考虑正合序列

$$
0 \longrightarrow K \longrightarrow M \xrightarrow{u} N
$$

很容易看出（命题 1）$E \otimes_A (\mathrm{Ker}\, u)$*与$\mathrm{Ker}(1_E \otimes u)$*一致*。另一方面，将满同态 $M \to I$ 写成 $u'$ ，其图形与 $u$ 相同，将典范嵌入 $I \to N$ 写成 $i$，$1_E \otimes u'$ 是满射（no. 1，引理 1）和 $1_E \otimes i$是单射的，因为 E 是平的。作为

$$
1_E \otimes u = (1_E \otimes i) \circ (1_E \otimes u'),
$$

$E \otimes_A (\mathrm{Im}\, u)$ *被识别*为$\mathrm{Im}(1_E \otimes u)$。

#### 命题 2 {#ac-i-s2-prop-2 .statement tag=042O}

(i) 设$(E_t)_{t \in I}$是右$A$模块族。为了使$E = \bigoplus_{t \in I} E_t$平坦，每个$E_t$平坦是必要且充分的。

(ii) 令$I$为右$A$模块(代数、章II, § 6, no. 2)的有序集合和$(E_\alpha, f_{\beta \alpha})$直接系统。如果每个$E_\alpha$都是平坦的，那么$E = \lim_{\longrightarrow} E_\alpha$也是平坦的。

设$M' \to M$为左单射$A$-模同态。

(i) 对于直和同态
$$
\bigoplus_{t \in I} (E_t \otimes_A M') \to \bigoplus_{t \in I} (E_t \otimes_A M)
$$
准确地说，同态 $E_t \otimes_A M' \to E_t \otimes_A M$ 中的每一个都如此（代数，章 II, § 1, no. 6，命题 7 的推论 1）是充分必要的，这证明了 (i) 因为 $\bigoplus_{t \in I} (E_t \otimes_A M)$ 与 $E \otimes_A M$ (代数， 章II, § 3, no. 7、命题7)。

(ii) 假设各序列
$$
0 \to E_\alpha \otimes_A M' \to E_\alpha \otimes_A M
$$
是准确的；那么序列
$$
0 \to E \otimes_A M' \to E \otimes_A M
$$
因为采用直极限与张量积 (代数, 章 II, § 6, no. 3, 命题 7) 进行通勤并保持精确性 (同上, § 6, no. 2, 命题 3)。

### 4. 例平坦模

(1) 对于任何环 $A$、$A$，显然是一个平面 $A$ 模（代数、章 II, § 3, no. 4、命题 4）。然后从命题 2, (i) of no. 3 得出，每个自由权$A$-模，更一般地每个射影权$A$-模（代数，章 11，§ 2, no. 2），都是一个平面$A$-模。

（2）如果$A$是半单环（代数，章VIII, § 5, no. 1，定义1）每个右$A$模$E$是半单，因此直和等于单模；由于后者均同构于 $A$ 的直因子（同上，§ 5, no. 1，命题 6），$E$ 是射影，因此平坦于 (1) (cf. 习题 16)。

*(3) 在章II和III中，我们将详细研究扁平$A$模块中两个重要的例：分数$S^{-1}A$的环和$A$的Hausdorff完成$\hat{A}$ $S$-adic 拓扑。*

#### 命题 3 {#ac-i-s2-prop-3 .statement tag=042P}

令$A$为环，且$E$为右$A$模。

(i) 假设 $E$ 是平坦的。对于每个元素$a \in A$（不是$0(*)$的右除子），关系$x \in E,\ xa = 0$意味着$x = 0$。

(*) 回想一下，环 $A$ 中 0 的右（或左）除子是元素 $b \in A$，使得映射 $x \mapsto xb$（或 $x \mapsto bx$）不是单射的。

(ii) 假设 $A$ 是整环，其中每个有限生成的理想都是主要的（对于例主理想整环 (代数, 章 VII, , no. 1)）。那么，要使 $E$ 平坦，$E$ 无扭转是必要且充分的

我们证明（i）。设$v : A, \to A$为左$A$-模同态$t \mapsto ta$； 假设意味着 $v$ 是单射的。由于 $E$ 是平的，同态 $1_E \otimes v : E \otimes_A A, \to E \otimes_A A$ 也是单射的。当 $E \otimes_A A$ 与 $E$ 进行规范标识时，$1, \otimes v$ 变为 $E$ 的自同态 $x \mapsto xa$。因此关系$xa = 0$意味着$x = 0$。

我们证明(ii)。根据 (i)，如果 $E$ 是平坦的，则 $E$ 是无扭转的。相反，令$E$为无扭$A$模；我们验证，对于$A$的每个有限生成的理想$a$，典范同态$E \otimes_A a \to E$是单射的（no. 3，注1）。如果$a = (0)$，这个断言是显而易见的；否则，对于某些$a \in A, a \neq 0$，通过假设$a = Aa$，然后$t \mapsto ta$是$A$的同构$v$到$a$；使用 $i$ 表示典范嵌入 $a \to A$，$i \circ v$ 是位似，$a$ 与 $E$ 之比，并且是单射的，因为 $E$ 被假定为无扭转。然后$1, \otimes (i \circ v) = (1, \otimes i) \circ (1_E \otimes v)$；由于 $1_E \otimes v$ 是同构，$1, \otimes i$ 是单射的，它完成证明。

#### 例 {#ac-i-s2-n4-exa-1 .statement tag=042Q}

应用命题3到环$\mathbf{Z}$，可以看出$\mathbf{Q}$是一个扁平的$\mathbf{Z}$模，但是$\mathbf{Z}/n\mathbf{Z}$（对于$n \geq 2$）不是一个扁平的$\mathbf{Z}$模。

### 5. 商模的平坦度

#### 命题 4 {#ac-i-s2-prop-4 .statement tag=042R}

令$E$为右$A$模。以下三个属性是等效的：

(a) $E$ 是平坦的。
(b) 对于右$A$的每个正合序列-形式的模块

(1)
$$
0 \longrightarrow G \xrightarrow{v} H \xrightarrow{w} E \longrightarrow 0
$$
以及剩下的每个$A$-模块$F$，序列

(2)
$$
0 \longrightarrow G \otimes_A F \xrightarrow{v \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
是准确的。

(c) 存在正合序列 (1)，其中 $H$ 是平坦的，使得序列 (2) 对于形式 $A_s/a$ 的每个左$A$-模 $F$ 是精确的，其中 $a$ 是 $A$ 的有限生成的左理想。

我们首先证明（a）蕴涵（b）。左侧$A$模$F$同构于商自由模 (代数, 章 II, § 1, no. 11, 命题 20)；在其他字，我们有正合序列

$$
0 \longrightarrow R \xrightarrow{i} L \xrightarrow{p} F \longrightarrow 0
$$

其中 L 是免费的。考虑图表

$$
\begin{array}{ccccccccc}
G \otimes R & \xrightarrow{v \otimes 1_R} & H \otimes R & \xrightarrow{w \otimes 1_R} & E \otimes R \\
\downarrow l_G \otimes i & & \downarrow l_H \otimes i & & \downarrow l_E \otimes i \\
G \otimes L & \xrightarrow{v \otimes 1_L} & H \otimes L & \xrightarrow{w \otimes 1_L} & E \otimes L \\
\downarrow l_G \otimes p & & \downarrow l_H \otimes p & & \\
G \otimes F & \xrightarrow{v \otimes 1_F} & H \otimes F
\end{array}
$$

(3)

紧接着，这个图表是可交换的，并且它的行和列精确到no. 1的引理 1；此外，由于$l_G \otimes p$和$l_H \otimes p$是满射（no. 1，引理1），我们有$G \otimes F = \operatorname{Coker}(l_G \otimes i)$，

$$
H \otimes F = \operatorname{Coker}(l_H \otimes i);
$$

$w \otimes 1_1$ 是满射 (no. 1, 引理 1)；最后，由于 L 是自由的，因此是平坦的，$v \otimes 1_L$ 是单射的。因此蛇图表(§ 1, no. 4,命题2,(iii))可以用来证明正合序列的存在

(4) $$ \operatorname{Ker}(l_H \otimes i) \longrightarrow \operatorname{Ker}(l_E \otimes i) \xrightarrow{d} G \otimes F \xrightarrow{v \otimes 1_F} H \otimes F. $$

既然如此，如果 E 是平的，则 $l_E \otimes i$ 是单射的，在其他字 $\operatorname{Ker}(l_E \otimes i) = 0$ 和正合序列 (4) 中，$v \otimes 1_F$ 是单射的，因此序列 (2) 是精确的（考虑到 no. 1 的引理 1）。

由于(b)显然蕴涵(c)，所以还需要证明(c)蕴涵(a)。 在$\mathbf{R} = \mathbf{a}, \mathbf{L} = \mathbf{A}_s, \mathbf{F} = \mathbf{A}_s/\mathbf{a}$情况下考虑图表(3)并应用正合序列(4)。 By hypothesis $v \otimes 1_F$ is injective, hence $\operatorname{Im}(d) = 0$; moreover, as H is flat, we have $\operatorname{Ker}(1, @i) = 0$; the exactness of the sequence (4) then implies $\operatorname{Ker}(l_E \otimes i) = 0$, in other words, $1, \otimes i$ is injective and this proves that E is flat (no. 3, Remark 1).

#### 命题 5 {#ac-i-s2-prop-5 .statement tag=042S}

*令*$0 \to E' \xrightarrow{v} E \xrightarrow{w} E'' \to 0$*为右*$\mathbf{A}$*-模块的正合序列。假设* $E''$ *是平坦的。那么，* *对于* $E$ *要平坦，* $E'$ *平坦是必要且充分的。*

令 $u : F' \to F$ 为左侧 $\mathbf{A}$ 模块的单同态。考虑图表

$$
\begin{array}{ccccccccc}
E' \otimes F' & \xrightarrow{v \otimes 1_{F'}} & E \otimes F' & \xrightarrow{w \otimes 1_{F'}} & E'' \otimes F' \\
\downarrow l_{E'} \otimes u & & \downarrow l_E \otimes u & & \downarrow l_{E''} \otimes u \\
E' \otimes F & \xrightarrow{v \otimes 1_F} & E \otimes F & \xrightarrow{w \otimes 1_F} & E'' \otimes F
\end{array}
$$

它是可交换的，并且它的行是精确的 (no. 1, 引理 1)。由于 $E''$ 是平坦的，所以 l_{E''} \otime u 是单射的；此外，命题 4 证明 v \otimes 1_{F'} 和 v \otimes 1 是单射的。既然如此，如果 E 是平坦的，则 l_E \otime u 是单射的，因此也

$$(l_E \otimes u) \circ (v \otimes 1_{F'}) = (v \otimes 1_F) \circ (l_{E'} \otimes u);$$

由此可知 l_{E'} \otime u 是单射的，因而 E' 是平坦的。相反，如果 E' 是平坦的，则 l_{E'} \otime u 是单射的；那么从 § 1, no. 4，推论 1 到命题 2，l_E \otimes u 是单射的，因而 E 是平坦的。

注
(1) E 和 E' 也可能平坦，而 E'' 则不平坦，如 \mathbf{Z} 模块 E = \mathbf{Z}、E' = n\mathbf{Z}、E'' = \mathbf{Z}/n\mathbf{Z} (n \geq 2) 的例所示。
(2) 平坦模的子模不一定是平坦模（习题3）。

### 6. 交属性

#### 引理 7 {#ac-i-s2-lem-7 .statement tag=042T}

令 E 为右A-模、F 左A-模和 F'、F'' F 的两个子模，使得 F = F' + F''。那么 E \otimes F' 和 E \otimes F'' 中的典范像的交就等于 E \otimes (F' \cap F'') 的典范像。

考虑图表

$$
\begin{array}{ccccccc}
0 & \longrightarrow & F' \cap F'' & \longrightarrow & F' & \longrightarrow & F'/(F' \cap F'') \longrightarrow 0 \\
& & \downarrow & & \downarrow & & \downarrow \\
0 & \longrightarrow & F'' & \longrightarrow & F' + F'' & \longrightarrow & (F' + F'')/F'' \longrightarrow 0
\end{array}
$$

where the unspecified arrows are 典范嵌入 and surjections and j 典范同构 defined in 代数, 章 I, § 6, no. 13, 定理 6. This 图表 is commutative and its rows are exact.我们导出（因为 F = F' + F''）一个可交换的图表

$$
\begin{array}{ccc}
E \otimes (F' \cap F'') & \longrightarrow & E \otimes F' \longrightarrow E \otimes (F'/(F' \cap F'')) \\
\downarrow & & \downarrow \\
E \otimes F'' & \longrightarrow & E \otimes F \longrightarrow E \otimes (F/F'')
\end{array}
$$

这个图表的行是精确的（no. 1，引理1）并且1\otimes j是同构。那么我们的断言就是 § 1, no. 4, 命题 1, (i) (cf. 习题 5) 的特例。

#### 命题 6 {#ac-i-s2-prop-6 .statement tag=042U}

令 E 为右A-模且 F 左A-模 ，使得 E 是 F 平的。对于 F 的每个子模 F'，我们用 E \otimes F' 的 \phi(F') 像表示，在 E \otimes F' 到 E \otimes F 的典范映射下（它是 no. 2 的定义 1 的内射）。那么，如果 F', F'' 是 F 的两个子模，我们有

$$\phi(F' \cap F'') = \phi(F') \cap \phi(F'').$$

由于E是降F调，$\phi(F' + F'')$与$E \otimes (F' + F'')$识别，子模、$\phi(F')$、$\phi(F'')$、$\phi(F' \cap F'')$分别与$E \otimes (F' + F'')$中的$E \otimes F'$、$E \otimes F''$、$E \otimes (F' \cap F'')$的典范像识别。然后从引理 7 得出命题 6。

#### 注 1 {#ac-i-s2-n6-rem-1 .statement tag=042V}

对于命题 6 的假设，对于 $F$ 的每一个子模 $F'$，$E \otimes_A F'$ 通常等同于 $\phi(F')$，从而得到公式
$$
E \otimes_A (F' \cap F'') = (E \otimes_A F') \cap (E \otimes_A F'').
$$

#### 命题 7 {#ac-i-s2-prop-7 .statement tag=042W}

*设E为E的右A-模、E的E'子模、F的左A-模和F'子模。假设E/E'或F/F'是平坦的。那么$E \otimes F$中$E' \otimes F'$的典范像就是$E \otimes F$中$E' \otimes F$和$E \otimes F'$的典范像交。*

假设例 $E/E'$ 是平坦的，并考虑图表
$$
\begin{array}{ccc}
E' \otimes F' & \longrightarrow & E \otimes F' \\
\downarrow & & \downarrow \\
E' \otimes F & \longrightarrow & E \otimes F
\end{array}
$$
$$
\begin{array}{ccc}
& & (E/E') \otimes F' \\
E \otimes F' & \longrightarrow & (E/E') \otimes F
\end{array}
$$
其中箭头是典范同态。这个图表是可交换的，并且它的行是精确的（no. 1，引理1）。由于 $E/E'$ 是平的，$u$ 是单射的。那么我们的断言就是 § 1, no. 4, 命题 1, (i) 的特例。

#### 推论{#ac-i-s2-n6-cor-1 .statement tag=042X}

令 E 为 E 的右A-模且 E' 子模。

(i) *假设 E/E' 是平坦的。然后，对于 A 的每个左理想 a，
$$
E'a = E' \cap Ea.
$$
(ii) *相反，假设 E 是平坦的，并且对于 A 的每个有限生成的左理想 a，关系 (5) 成立。那么 E/E' 是平坦的。*

(i) 对于$F = A$、$F' = a$的情况，应用命题就足够了。
(ii) 为了证明$E/E'$是平坦的，应用no. 5的命题 4的标准(c)；那么有必要确定序列
$$
0 \to E'/E'a \to E/Ea \to E/(E' + Ea) \to 0
$$
对于 A 的每个有限生成的左理想 a，精确于 $E'/E'a$。现在这正是关系 (5) 所表达的。

#### 注 2 {#ac-i-s2-n6-rem-2 .statement tag=042Y}

如果我们仅假设 $E/E'$ 是 F 降调或 $F/F'$ 是 E 降调，则命题 7 的结论仍然成立。

### 7. 张量积扁平模

令$A, B$为两个环，$E$为右$A$模，$F$为$(A,B)$双模（*代数*，章II, § 1, no. 14）。回想一下 (*代数*, 章 II, § 3, no. 4)，$E \otimes_A F$ 有一个规范的右$B$-模块结构，其中

$$
(x \otimes y)b = x \otimes (yb) \quad \text{for} \quad x \in E,\ y \in F,\ b \in B.
$$

#### 命题 8 {#ac-i-s2-prop-8 .statement tag=042Z}

*令$A, B$为两个环，$E$为右$A$模，$F$为$(A,B)$双模。假设 $E$ 是平坦的，并且 $F$ 作为 $B$ 模也是平坦的。那么$B$-模块$E \otimes_A F$是平的。*

设$G$为$B$模，$G'$子模为$G$。由于 $F$ 是平直的 $B$ 模，因此典范同态 $F \otimes_B G' \to F \otimes_B G$ 是单射的。由于 $E$ 是平坦的，典范同态

$$
E \otimes_A (F \otimes_B G') \to E \otimes_A (F \otimes_B G)
$$

是单射的。由于 $E \otimes_A (F \otimes_B G')$ 和 $E \otimes_A (F \otimes_B G)$ 分别被规范地标识为 $(E \otimes_A F) \otimes_B G'$ 和 $(E \otimes_A F) \otimes_B G$ (*代数*, 章 II, § 3, no. 8, 命题 8), 典范同态

$$
(E \otimes_A F) \otimes_B G' \to (E \otimes_A F) \otimes_B G
$$

是单射的，证明$E \otimes_A F$是平的$B$模。

#### 推论 1 {#ac-i-s2-prop-8-cor-1 .statement tag=0430}

令$C$为交换环、$E, F$两个扁平的$C$模块。那么$E \otimes_C F$是一个扁平的$C$模块。

$F$是一个$(C, C)$双模，用$B = A = C$满足应用命题 8即可。

#### 推论 2 {#ac-i-s2-prop-8-cor-2 .statement tag=0431}

*令$\rho$为环$A$到环$B$中的同态。如果$E$是平右$A$-模，则将标量的环扩展到$B$（*代数*，章II, § 5, no. 1）获得的右$B$-模$\rho^*(E) = E_{(B)}$是平的。*

通过定义$E_{(B)} = E \otimes_A B$，其中$B$通过$\rho$被视为$(A,B)$双模。由于右边的$B$-模$B_d$是平的，所以应用命题8就足够了。

#### 推论 3 {#ac-i-s2-prop-8-cor-3 .statement tag=0432}

*令$R, S$为两个环和$\phi : R \to S$环同态。如果$M$是平右$S$模，$\phi_*(S_d)$是平右$R$模，则$\phi_*(M)$是平右$R$模。*

回想一下，$\phi_*(M)$是$x.r = x.\phi(r)$为所有$x \in M$和所有$r \in R$定义的正确$R$模块（*代数*，章II, § 1, no. 13）。然后应用命题 8 与$A = S, B = R, E = M$ 和$F = S, S$ 具有由$\phi$ 定义的$(S, R)$双模的结构；那么正确的$R$-模块$M \otimes_S S$恰好是$\phi_*(M)$。

#### 命题 9 {#ac-i-s2-prop-9 .statement tag=0433}

*令$(A_\alpha, f_{\beta\alpha})$为环的直接系统，$A = \lim A_\alpha$为其直极限，$(E_\alpha, f_{\beta\alpha})$直接系统为右$A_\alpha$的模块，具有相同索引集合和$E = \lim E_\alpha$其直极限，这是一个右$A$模块（代数，章II, § 6, no. 2）。如果每个 $\alpha$ $E_\alpha$ 都是平面 \& 模块，则 $E$ 是平面 $A$ 模块。*

设$E'_\alpha = E_\alpha \otimes_{A_\alpha} A$，其中$A$通过典范同态$A_\alpha \to A$被视为左$A_\alpha$模；我们知道正确的$A$-模块$E$在规范上与$\lim E'_\alpha$同构的（*loc.cit.*，推论2到命题7）。从推论2到命题8，$E'_\alpha$是所有$\alpha$的平右$A$模，因此$E$是no. 3的命题2的平$A$模。

### 8. 有限呈现模

设$A$为环。 正合序列
$$
L_1 \to L_0 \to E \to 0
$$
左（或右）$A$-模块，其中$L_0$和$L_1$是自由的，被称为左（或右）$A$-模块$E$的*呈现*（或*长度* 1的呈现）。

每个 $A$-模块 $E$ 都承认一个演示文稿。事实上我们知道（*代数*，章II, § 1, no. 11，命题20）存在满同态$u : L_0 \to E$，其中$L_0$是免费的；如果$R$是$u$的核，则类似地存在满同态$v : L_1 \to R$，其中$L_1$是空闲的。如果将$v$视为$L_1$到$L_0$的同态，则序列$L_1 \xrightarrow{v} L_0 \xrightarrow{u} 0$正好等于定义，从而我们的断言。

如果 $\rho : A \to B$ 是环同态，$E$ 诱导的每个呈现 (6) 都会呈现 $E_{(B)} = E \otimes_A B$：
$$
L_1 \otimes_A B \to L_0 \otimes_A B \to E \otimes_A B \to 0
$$
通过 no. 1 的引理 1，并且如果 $L$ 是免费的，则 $L \otimes_A B$ 是免费的 $B$ 模块。

如果自由模 $L_0$ 和 $L_1$ 具有有限的基，则模 $E$ 的表示 (6) 被称为*有限*。显然，如果表示（6）是有限的，那么表示（7）也是有限的。如果$E$允许有限表示，则称为*有限表示$A$模块*。

#### 引理 8 {#ac-i-s2-lem-8 .statement tag=0434}

(i) *每个模承认有限的表示都是有限生成的。*
(ii) *如果 $A$ 是左诺特环，则每个有限生成的左 $A$ 模块都承认有限表示。*
(iii) *每个有限生成射影模都承认有限的表示。*

断言 (i) 是从定义简单得出的。如果$A$是左诺特的并且存在满同态$u : L_0 \to E$，其中$L_0$是具有有限基的自由左$A$模，则$u$的核$R$是有限生成的(*代数*, 章 VIII, , no. 1, 命题 1 和 no. 3, 命题 7)，因此有满同态 $u : L_1 \to R$，其中 $L_1$ 是自由的并且有一个有限的基，正合序列$L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$是$E$的有限表示； 从而 (二)

最后，假设$E$是有限生成射影模；那么它是有限生成的自由模$L_0$的直因子（*代数*，章II, §2, no. 2，命题4的推论）； 满同态$L_0 \to E$的核$R$同构于$L_0$的商，因此是有限生成的并且证明如(ii)那样完成。

#### 引理 9 {#ac-i-s2-lem-9 .statement tag=0435}

*令$A$为环且$E$为有限呈现的$A$模块。每正合序列*

$$
0 \longrightarrow F \xrightarrow{j} G \xrightarrow{p} E \longrightarrow 0
$$

*其中 $G$ 是有限生成的，模 $F$ 是有限生成的。*

令 $L, \xrightarrow{r} L_0 \xrightarrow{s} E \to 0$ 为有限表示；如果$(e_i)$是$L_0$的基，则对于每个$i$元素$g_i \in G$都存在$p(g_i) = s(e_i)$； 同态 $u : L_0 \to G$，使得所有$i$的$u(e_i) = g_i$满足$s = p \circ u$。由于$s \circ r = 0$，我们有$u(r(L_1)) \subset \mathrm{Ker}\, p$，并且由于$\mathrm{Ker}\, p$与$F$同构的，因此可以看出，存在同态$v : L, \to F$使得图表

$$
\begin{array}{ccccccccc}
L, & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \longrightarrow & 0 \\
\downarrow v & & \downarrow u & & \downarrow 1_E & & \\
F & \xrightarrow{i} & G & \xrightarrow{p} & E & \longrightarrow & 0
\end{array}
$$

是可交换的。由于$j$是单射，$s$满射，我们可以应用蛇图表（$\S$1，no. 4，命题4），在其他字有正合序列

$$
0 = \mathrm{Ker}\, 1, \xrightarrow{d} \mathrm{Coker}\, v \longrightarrow \mathrm{Coker}\, u \longrightarrow \mathrm{Coker}\, 1, = 0.
$$

This shows that $\mathrm{Coker}\, v$ is isomorphic to $G / u(L_0)$, which is finitely generated by hypothesis. 此外，我们还有正合序列

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\, v \to 0
$$

由于$v(L_1)$和$\mathrm{Coker}\, v$是有限生成的，$F$也是有限生成的（*代数*，章II, § 1, no. 7，推论5到命题9）。

### 9. 同态模中的标量扩张

令$A$和$B$为两个环，$E$为右$A$模，$F$为右$B$模，$G$为$(B, A)$双模。回想一下，我们已经定义了 $\mathbf{Z}$ 模块的 (代数, 章 II, § 4, no. 2) 典范同态

$$
\nu : F \otimes_B \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F \otimes_B G)
$$

这样，对于$\in F$和$u \in \operatorname{Hom}_A(E, G)$，$\nu(y \otimes u)$是$A$线性映射$x \mapsto y \otimes u(x)$。

#### 命题 10 {#ac-i-s2-prop-10 .statement tag=0436}

*令$A, B$为两个环，$E$为右$A$模，$F$为右$B$模，$G$为$(B, A)$双模。假设 $F$ 是平坦的。那么，如果 $E$ 是有限生成的（或有限呈现的），则典范同态 (8) 是单射的（或双射的）。*

将 $A, B, F, G$ 视为固定的，并且对于每个右$A$-模块 $E$ 集合

$$
T(E) = F \otimes_B \operatorname{Hom}_A(E, G), \quad T'(E) = \operatorname{Hom}_A(E, F \otimes_B G)
$$

并用 $\nu_E$ 表示同态 (8)；对于每个右$A$-模块同态$v : E \to E'$、集合$T(v) = 1, \otimes \operatorname{Hom}(v, 1_G)$和$T'(v) = \operatorname{Hom}(v, 1, \otimes 1_G)$。设$L, \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$是$E$的表示；我们假设自由模 $L_0$（分别是自由模 $L_0$ 和 $L_1$）是*有限生成的*。 图表

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & \downarrow{\nu_E} & & \downarrow{\nu_{L_0}} & & \downarrow{\nu_{L_1}} \\
0 & \longrightarrow & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

是可交换的，并且第二行是精确的 (代数, 章 II, § 2, no. 1, 定理 1)；此外，序列

$$
0 \to \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(L_0, G) \to \operatorname{Hom}_A(L_1, G)
$$

是精确的（*loc.cit.*），并且由于$F$*是平坦的*，（9）的第一行也是正合序列（no. 3，命题1）。然后我们知道$\nu_{L_0}$（分别是$\nu_{L_0}$和$\nu_{L_1}$）是*双射*（分别是*双射*）（代数，章II, § 4, no. 2，命题2）。如果我们仅假设 $\nu_{L_0}$ 是双射的，则从 (9) 可以得出：

$$
\nu_{L_0} \circ T(w) = T'(w) \circ \nu_E
$$

是单射的，因此 $\nu_E$ 也是单射的。如果我们假设$\nu_{L_0}$和$\nu_{L_1}$都是双射的，那么从§ 1, no. 4，推论2，(ii)到命题2，$\nu_E$是满射的，正如我们刚刚看到的，$\nu_E$是单射的，它是双射的。

### 10.标量的扩张：交换环的情况

Now let $A$ be a *commutative* 环, $B$ 环 and $\rho : A \to B$ 环同态 such that $\rho(A)$ is contained in the *中心* of $B$;其他字、$\rho$ 定义 $B$ 上

A-代数结构。 For every A-模 E, 右B-模 $E_{(B)} = E \otimes_A B$ is then identified with $B \otimes_A E$, A-模结构 of $\rho_*(B_s)$ and $\rho_*(B_d)$ being identical by 假设. Recall that for every 有序对 (E, F) of A-模, we have defined a canonical B-homomorphism

$$
\omega : (\operatorname{Hom}_A(E, F))_{(B)} \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

这样对于所有$u \in \operatorname{Hom}_A(E, F)$，$\omega(u \otimes 1) = u \otimes 1_B$（代数，章II, § 5, no. 3）。

#### 命题 11 {#ac-i-s2-prop-11 .statement tag=0437}

设A为A的交换环，B环，A的$\varphi$同态到B的中心，E和F为A-模。假设 B 是平面 A-模并且 E 是有限生成的（或有限呈现的）。那么典范同态 (10) 是单射（或双射）。

因为$\omega$由典范同构组成

$$
\operatorname{Hom}_A(E, B \otimes_A F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

和典范同态 (8)

$$
\nu : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, B \otimes_A F)
$$

（前述），命题是命题 10 no. 9 的推论。

现在假设 A 和 B 是可交换的，并考虑三个 A-模 $E_1, E_2, E$ 和一个 A 双线性映射 $f : E_1 \times E \to E_3$。那么存在且仅有一个 B-双线性映射 $f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}$ 使得

$$
f_B(1 \otimes x_1, 1 \otimes x_2) = 1 \otimes f(x_1, x_2)
$$

对于所有 $x_1 \in E_1, x_2 \in E$、(代数、章 IX, § 1, no. 4、命题 1)。

在接下来的叙述中，我们假设B是平的A-模，并且对于$E_i$（$i = 1, 2, 3$）的每个子模E'，我们将规范地认同$E'_{(B)}$及其在$E_{i(B)}$（no. 3）中的像， 注2)。

#### 命题 12 {#ac-i-s2-prop-12 .statement tag=0438}

设 A, B 为 A 到 B 的交换环、$\varphi$ 同态、$E_1, E_2, E_3$ 三个A-模、$f : E_1 \times E \to E_3$ 一个 A 双线性映射以及

$$
f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}
$$

它扩张。考虑$E_2$的子模$F_2$，$E_3$的子模$F_3$，并用$x_1 \in E_1$的$E_1$由……组成的T子模表示，使得$f(x_1, x_2) \in F$，对于所有$x_2 \in F$。假设 B 是平坦的 A-模并且 $F_2$ 是有限生成的。那么 $T_{(B)}$ 是那些 $x'_1 \in E_{1(B)}$ 中的集合，使得 $f_B(x'_1, x'_2) \in F_{3(B)}$ 对于所有 $x'_2 \in F_{2(B)}$。

设$p$为典范满射$E_3 \to E_3/F_3$；对于每个$x_1 \in E_1$，我们将$F_2$的A-线性映射$x_2 \mapsto p(f(x_1, x_2))$与$E_3/F_3$相关联，我们用$g(x_1)$表示；那么$g$是$E_1$到$\mathrm{Hom}_A(F_2, E_3/F_3)$的A同态，而$g$的核恰好是T。由于B是平的A-模，所以我们有正合序列

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{1 \otimes g} (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)}
$$

（no. 3，命题1）。截至命题 11 典范同态

$$
\omega : (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)} \to \mathrm{Hom}_B(F_{2(B)}, (E_3/F_3)_{(B)})
$$

是*内射*。另一方面，由于 B 是降调 A-模，因此 $(E_3/F_3)_{(B)}$ 被规范地等同于 $E_{3(B)}/F_{3(B)}$；将$\omega$中的合成与$1 \otimes g$相乘，我们得到同态$u$，其中序列！

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{u} \mathrm{Hom}_B(F_{2(B)}, E_{3(B)}/F_{3(B)})
$$

是准确的。从定义紧接着$u(x'_1)$，其中

$$
x'_1 = 1 \otimes x_1 \in E_{1(B)},
$$

是线性映射其中映射每个 $x'_2 \in F_{2(B)}$ 到类 mod。 $F_{3(B)}$ 共 $f_B(x'_1, x'_2)$；根据线性度，这对于所有 $x'_1 \in E_{1(B)}$ 也成立；由于$u$的核是$T_{(B)}$，所以命题得证。

#### 推论 1 {#ac-i-s2-prop-12-cor-1 .statement tag=0439}

*令 A、B 为两个交换环、$p : A \to B$ 同态，使得 B 为平坦 A-模，E 为有限呈现的 A-模。对于E的每个有限生成的子模F，与$F_{(B)}$正交的$E_{(B)}$对偶的子模等于$(F')_{(B)}$，其中$F'$是与F正交的E的对偶$E^*$的子模。*

命题 11 $(E^*)_{(B)}$ 与 $E_{(B)}$ 的对偶 $(E_{(B)})^*$ 典型同构。那么它就足以满足应用命题 12 以及 $E_1 = E^*$、$E_2 = E$、$E_3 = A$、$F_2 = F$、$F_3 = \{0\}$ 和 $f$ $E^* \times E$ 上的规范双线性形式。

#### 推论 2 {#ac-i-s2-prop-12-cor-2 .statement tag=043A}

*设A、B为两个交换环、$p : A \to B$同态，则B为平音A-模，E为A-模。然后，对于 E 的每个有限生成的子模 F，$F_{(B)}$ 的湮没子是 B 的理想 $aB$，其中 a 是 A 中 F 的湮没子。*

加上 $E_1 = A$、$E_2 = E_3 = E$、$F_2 = F$、$F_3 = \{0\}$ 就足以满足应用命题 12。

#### 注 {#ac-i-s2-n10-rem-1 .statement tag=043B}

如果模 E 上没有歧义，双线性映射 $f$ 也没有歧义，则$F_3 : F_2$ 是有时用于表示命题 12 中由T 表示的模，并且它被称为F 到F 的*传送器*。 命题 12 的结论如下：

$$
F_{3(B)} : F_{2(B)} = (F_3 : F_2)_{(B)}.
$$

在特定情况下，当$E_i$等于环，$A, f$等于乘法且$F_i$理想$a_i$时，我们获得*转运公式*

$$
B(a_3 : a_2) = Ba_3 : Ba_2
$$

当 $B$ 是平面 $A$ 模并且 $a_2$ 是有限生成的理想时有效。

### 11. 项 OF 关系中平坦度的解释 (*)

在整个过程中没有。 $A$表示环，$E$表示右$A$模块，$F$表示左$A$模块。

$E \otimes_A F$中的每个元素都可以用至少一种方式写成形式
$$
z = \sum_{i=1}^n e_i \otimes f_i \text{ where } e_i \in E \text{ and } f_i \in F.
$$
下面的引理给出条件，其中和是零：

#### 引理 10 {#ac-i-s2-lem-10 .statement tag=043C}

*让*$(f_\lambda)_{\lambda \in L}$*成为*$F$*的生成元的家庭和*$(e_\lambda)_{\lambda \in L}$*元素的*$E$*有限支撑的家庭。对于*$\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$，*存在一个有限的集合*$J$，*$(x_j)_{j \in J}$*的元素*$E$*和一个元素的*族*$(a_{j,\lambda})$*($j \in J, \lambda \in L$)*是充分必要的$A$ *具有以下属性：*

(1) *族* $(a_{j,\lambda})$ *有有限支撑;*

(2) $\sum_{\lambda \in L} a_{j,\lambda} f_\lambda = 0$ *对于所有人* $j \in J;$

(3) $e_\lambda = \sum_{j \in J} x_j a_{j,\lambda}$ *对于所有人* $\lambda \in L.$

宽松地说，$e_\lambda$的系统必须是线性组合，其中系统、元素、$A$的$E$的系数是“$f_\lambda$之间的关系”。

考虑免费的$A$-模块$A_s^{(L)}$，其典范基$(u_\lambda)$和同态$g : A_s^{(L)} \to F$，使得$g(u_\lambda) = f_\lambda$适用于所有$\lambda \in L$；用$g$的$R$核表示，我们有（从$f_\lambda$生成$F$）正合序列

$$
R \xrightarrow{i} A_s^{(L)} \xrightarrow{g} F \longrightarrow 0
$$

其中$i$表示典范嵌入。通过 no. 1 的引理 1，我们得出正合序列

$$
E \otimes_A R \xrightarrow{1 \otimes i} E \otimes_A A_s^{(L)} \xrightarrow{1 \otimes g} E \otimes_A F \longrightarrow 0.
$$

(*) 此编号的结果。除了§ 3, no. 7之外，将不会在章的其余部分中使用。

现在，$E \otimes_A A_s^{(L)}$ 被规范地标识为 $E^{(L)}$，$e = (e_\lambda) \in E^{(L)}$ 家族被标识为 $\sum_{\lambda \in L} e_\lambda \otimes u_\lambda$（*代数*、章 II、、no. 7、推论 1 到命题 7）。对于$1_E @ g$属于到核这样的家庭来说，$E \otimes_A F$中的$\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$是充分必要的；考虑到正合序列（13），这相当于$1, \otimes i$的$e$属于到像的说，其他字还有形式的关系

$$
\sum_{\lambda \in L} e_\lambda \otimes u_\lambda = \sum_{j \in J} x_j \otimes i(r_j)
$$

其中 $x_j \in E, r_j \in R$ 和 $J$ 是有限的。写 $i(r_j) = \sum_{\lambda \in L} a_{j\lambda} u_\lambda$、假设 $r_j \in R$ 意味着所有 $j \in J$ 都有关系 $\sum_{\lambda \in L} a_{j\lambda} f_\lambda = 0$；另一方面，关系 (14) 对所有$\lambda \in L$意味着$e_\lambda = \sum_{j \in J} x_j a_{j\lambda}$（*代数*，章II, § 3, no. 7，推论1到命题7），从而完成证明。

#### 命题 13 {#ac-i-s2-prop-13 .statement tag=043D}

*为了使E成为F降调*（no. 2，*定义1*），*满足以下条件是必要且充分的*：

*(R)* *如果* $(e_i)_{i \in I}$ *和* $(f_i)_{i \in I}$ *分别是E和F的元素的两个有限族，使得* $\sum_{i \in I} e_i \otimes f_i = 0$ *在* $E \otimes_A F$中，*存在有限集合 J，E的元素族* $(x_j)_{j \in J}$ *和A 的元素的族* $(a_{ji})$ *($j \in J, i \in I$)，具有以下属性*：

(1) $\sum_{i \in I} a_{ji} f_i = 0$ *对于所有人* $j \in J$；
(2) $e_i = \sum_{j \in J} x_j a_{ji}$ *对于所有人* $i \in I$。

假设E 是降F 的。令$(e_i)$和$(f_i)$为元素的有限族，使得$\sum_{i \in I} e_i \otimes f_i = 0$位于$E \otimes_A F$中，并令$F'$为由*$f_i$生成的F *的子模。由于典范映射 $E \otimes_A F' \to E \otimes_A F$ 是单射的，因此我们还有 $\sum_{i \in I} e_i \otimes f_i = 0$ *in* $E \otimes_A F'$ *，并且引理 10 可以应用于 E 和 F'；从而获得(R)*的家庭*$(x_j)$*和*$(a_{ji})$*满足条件。

相反，假设条件 (R) 成立。令$F'$为F的子模，令$y = \sum_{i \in I} e_i \otimes f_i$为典范映射$E \otimes_A F' \to E \otimes_A F$的核元素。由于(R)成立，存在族$(x_j)$和$(a_{ji})$满足条件(1)和(2)。我们结论，在$E \otimes_A F'$，

$$
y = \sum_{i,j} x_j a_{ji} \otimes f_i = \sum_{j \in J} (x_j \otimes \sum_{i \in I} a_{ji} f_i) = 0.
$$

因此 $E \otimes_A F' \to E \otimes_A F$ 是单射的。

#### 推论 1 {#ac-i-s2-prop-13-cor-1 .statement tag=043E}

对于右$A$模$E$是平坦的，满足以下条件成立是必要且充分的：

(RP) *如果* $(e_i)_{i \in I}$和$(b_i)_{i \in I}$分别是$E$和$A$的元素的两个有限族，使得$\sum e_i b_i = 0$，存在有限集合$J$，元素的$(x_j)_{j \in J}$族$E$ 和元素 $A$ 的$(a_{ji})$ ($j \in J, i \in I$) 家庭，使得$\sum a_{ji} b_i = 0$ 适合所有$j \in J$，$e_i = \sum_{j \in J} x_j a_{ji}$ 适合所有$i \in I$。

条件 (RP) 只是命题 13 的条件 (R) 应用于模 $F = A_s$。

宽松地说，（RP）指出：系数在$E$中的$b_i$之间的每个“关系”，是系数在$A$中的$b_i$之间的“关系”的线性组合（系数在$E$中）。

让我们特别考虑$A$到环$B$的同态，这使得$B$成为右$A$模块。我们知道（no. 3，命题 1），这相当于说，这个$A$-模块是平坦的，或者它对于每个左边的$A$-模块$A_s^m$（$m \geqslant 1$）都是平坦的。 命题 13 与 $E = B$ 和 $F = A_s^m$ 的应用条件 (R) 我们得到以下条件：

#### 推论 2 {#ac-i-s2-prop-13-cor-2 .statement tag=043F}

为了使环$B$成为平右$A$模，满足以下条件是充分必要的：
(RP') *齐次线性方程组解* $(y_k)_{1 \leq k \leq n}$、$B$、系统元素、由……组成

$$
\sum_{k=1}^n y_k c_{ki} = 0 \quad (1 \leq i \leq m)
$$
$A$ 中的*系数* $c_{ki}$，*为线性组合*
$$
y_k = \sum_{j=1}^q b_j z_{jk} \quad (1 \leq k \leq n)
$$
其中*系数* $b_j \in B$，解 $(z_{jk})_{1 \leq k \leq n}$，系统 (15)，由……组成，元素 $z_{jk}$，$A$。

### 习题{#ac-i-s2-exercises}

§ 2](exercises/s2/)参见[习题。
