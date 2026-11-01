---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 5
section_title: Hypocontinuous bilinear mappings
lang: zh
source: evt-i-v
book_pages: TVS III.28-TVS III.33, TVS III.46-TVS III.49
pdf_pages: 0160-0165, 0178-0181
extraction: ocr
subsections:
    - "no": 1
      title: Separately continuous bilinear mappings
      page: 28
      pdf_page: 160
    - "no": 2
      title: Separately continuous bilinear mappings on a product of Fréchet spaces
      page: 29
      pdf_page: 161
    - "no": 3
      title: Hypocontinuous bilinear mappings
      page: 30
      pdf_page: 162
    - "no": 4
      title: Extension of a hypocontinuous bilinear mapping
      page: 32
      pdf_page: 164
    - "no": 5
      title: Hypocontinuity of the mapping $(u, v) \mapsto v \circ u$
      page: 32
      pdf_page: 164
statements: 16
exercises: 15
content_sha256: 467b239b06088655fc36961333af8bbbc9f8586c4cef2a3352cc4545b5889209
translated_from: content/en/evt/III/05_s5_hypocontinuous_bilinear_mappings.md
translation_method: google
source_content_sha256: eefe4b53c6330aa7a5e81cb0b9c60f3b12b31b2df9f7ff14d5388452b92097de
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 87055b941e0f681b92a33d82b9cae35bcc8817fb7db63b6774b9de3b528ed394
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。次连续双线性映射

### 1. 单独连续的双线性映射

令 $E, F, G$ 为三个局部凸空间。对于从$E \times F$到$G$的每个双线性映射$u$，以及每个$x \in E$（分别$y \in F$），我们用$u(x, .)$（分别$u(., y)$）映射$y \mapsto u(x, y)$（分别$x \mapsto u(x, y)$）表示$F$ 变为 $G$（分别从 $E$ 变为 $G$）。

#### 定义 1 {#evt-iii-s5-def-1 .statement tag=07P9}

*如果对于所有 $x \in E$、线性映射 $u(x, .)$ 从 $F$ 到 $G$ 是连续的，并且对于所有 $y \in F$、线性映射，则称从 $E \times F$ 到 $G$ 的双线性映射 $u$ 是单独连续的$u(., y)$从$E$到$G$是连续的。*

接下来的命题紧接在定义之后。

#### 命题 1 {#evt-iii-s5-prop-1 .statement tag=07PA}

*对于从$E \times F$到$G$的双线性映射$u$是单独连续的，对于所有$y \in F$，线性映射$u(., y)$从$E$到$G$是连续的并且线性映射是必要和充分的$y \mapsto u(., y)$从$F$到$\mathscr{L}_s(E; G)$是连续的。*

我们还可以说，每个线性映射$v \in \mathscr{L}(F; \mathscr{L}_s(E; G))$都与双线性映射$(x, y) \mapsto v(y)(x)$相关联，那么我们定义从$\mathscr{L}(F; \mathscr{L}_s(E; G))$到向量空间的线性*双射*从$E \times F$到$G$的单独连续双线性映射。

从$E \times F$到$G$的单独连续双线性映射不一定在$E \times F$上连续（III，p. 47，练习2；cf.，但是III，p. 30和IV， p. 26，第 2)。

The notion of a separately continuous bilinear *form* on a product $E_1 \times E_2$ of two locally convex spaces is directly related to that of a continuous linear mapping when $E_1$ and $E_2$ are assigned the *weak* topologies (II, p. 42), Suppose that $(E_1, F_1)$ and $(E_2, F_2)$ are two pairs of real (resp. complex) vector spaces in separating duality (*loc. cit.*); we assign to $E_i$ (resp. $F_i$) the weak topology $\sigma(E_i, F_i)$ (resp. $\sigma(F_i, E_i)$) for $i = 1, 2$, and denote by $B(E_1, E_2)$ the vector space of separately *continuous* bilinear forms on $E_1 \times E_2$. 应用道具。 1 对于$G = K$的情况，我们看到，对于每个双线性形式$\Phi \in B(E_1, E_2)$和每个$x_2 \in E_2$，映射$x_1 \mapsto \Phi(x_1, x_2)$是$E_1$上的连续线性形式，因此（II，p. 43，道具3）存在一个元素，并且只有一个$^d\Phi(x_2) \in F_1$使得

$$
\Phi(x_1, x_2) = \langle x_1, ^d\Phi(x_2) \rangle
$$

对于每个 $x_1 \in E_1$ 和 $x_2 \in E_2$；此外，对于 $E_2$ 和 $F_1$ 的（弱）拓扑，映射 $^d\Phi : E_2 \to F_1$ 是线性且“连续”的。

相反，对于每个连续的线性映射$u : E_2 \to F_1$映射$(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$都是$E_1 \times E_2$上的单独连续双线性形式，并且我们有$u = {}^d \Phi$。因此，我们定义了从$B(E_1, E_2)$到$\mathscr{L}(E_2; F_1)$的同构$d : \Phi \mapsto {}^d \Phi$，据说是*典范的*。同样公式

$$
\Phi(x_1, x_2) = \langle {}^s \Phi(x_1), x_2 \rangle
$$

定义一个*规范*同构$s : \Phi \to {}^s \Phi$从$B(E_1, E_2)$到$\mathscr{L}(E_1, F_2)$；显然我们有交换律图表

$$
\begin{array}{ccc}
& B(E_1, E_2) & \\
s & / & d \\
\downarrow & & \downarrow \\
\mathscr{L}(E_1; F_2) & \leftrightarrow & \mathscr{L}(E_2; F_1)
\end{array}
$$

其中 $t$ 是转置的同构（II、p. 46、命题 5 和推论）。鉴于$F_1$和$F_2$上的弱拓扑定义，当$B(E_1, E_2)$、$\mathscr{L}(E_1; E_2)$、$\mathscr{L}(E_2; F_1)$被赋值为简单收敛*拓扑时，直接的为直接的，图表(3)的同构为拓扑向量空间同构*。

### 2. Fréchet 空间乘积上的单独连续双线性映射

#### 命题 2 {#evt-iii-s5-prop-2 .statement tag=07PB}

*设E、F和G为三个局部凸空间。假设 E 和 F 是可度量的并且 E 是桶形的。令 H 为从 E × F 到 G 的单独连续双线性映射的集合。假设对于从 F 到 G 的映射 $u(x, .)$ 的每个$x \in E$、集合，其中 u 穿过 H，是等连续的。那么 H 是等连续的。*

令$U_n$（或$V_n$）为E（或F）中0的邻域的基本序列。如果 H 不等连续，则 G 中存在闭、凸、平衡 0 的邻域 W，使得对于所有 $n$，$H(U_n \times V_n)$ 不包含在 W 中。则存在对 $(x_n, y_n) \in U_n \times V_n$ 的序列和元素的序列 $(u_n)$ H，使得 $u_n(x_n, y_n) \notin W$。令$p$为W的规范。对于每个$y \in F$和每个$u \in H$，从E到G的映射$u(., y)$是连续的，因此$p \circ u(., y)$是E上的连续半范数。另一方面，对于映射的每个$x \in E$，集合 $u(x, .)$ 对于 $u \in H$ 是等连续的；由于序列 $(y_n)$ 趋于 0，因此它是有界的，并且对于 $n \geq 0$ 和 $u \in H$，所有 $u(x, y_n)$ 的集合是有界的（III，p. 22，道具 9）。由此可见，函数$p'(x) = \sup_{\substack{u \in H \\ n \geq 0}} p(u(x, y_n))$是E上的下半连续半范数（有限）。由于E是桶状的，所以$p'$是连续的（III，p. 24，推论）。由于E中$(x_n)$趋于0，$p'(x_n)$趋于0，因此如果$n$足够大，我们就有$p'(x_n) \leq 1$；但然后$p(u_n(x_n, y_n)) \leq p'(x_n) \leq 1$，因此$u_n(x_n, y_n) \in W$，与……矛盾假设在$u_n, x_n, y_n$上。

#### 推论 1 {#evt-iii-s5-prop-2-cor-1 .statement tag=07PC}

— 令 E 和 F 为两个 Fréchet 空间，G 为局部凸空间。从 $E \times F$ 到 G 的每个单独连续双线性映射都是连续的。

事实上，每颗 Fréchet 空间都是桶装的（III、p. 25，推论）。

令 E 和 F 为两个局部凸空间。我们用$\mathscr{B}(E, F)$表示$E \times F$上连续双线性形式的空间，拓扑在形式$A \times B$的集合上一致收敛，其中A（或B）有界于E（或F）。 公式
$$
u(x, y) = \langle y, \phi(u)(x) \rangle
$$
（对于$x \in E, y \in F$和$u \in \mathscr{B}(E, F)$）定义从$\mathscr{B}(E, F)$到$\mathscr{L}_b(E; F'_b)$的连续线性单射映射$\phi$。

#### 推论 2 {#evt-iii-s5-prop-2-cor-2 .statement tag=07PD}

— 假设 E 和 F 是可度量的并且 E 是桶状的。那么$\phi$是从$\mathscr{B}(E, F)$到$\mathscr{L}_b(E; F'_b)$的拓扑向量空间同构。

让$f \in \mathscr{L}_b(E; F'_b)$。将 $u(x, y) = \langle y, f(x) \rangle$ 替换为 $x \in E$ 和 $y \in F$。 双线性形式 $u$在$E \times F$上分别连续；通过道具。 2、从属于到$\mathscr{B}(E, F)$，我们有$f = \phi(u)$。因此$\phi$是从$\mathscr{B}(E, F)$到$\mathscr{L}_b(E; F'_b)$的线性双射。 $\phi$ 是双连续的，因此是直接的。 2如下。

### 3. 次连续双线性映射

接下来，我们将定义概念介于连续双线性映射和单独连续双线性映射之间。

#### 命题 3 {#evt-iii-s5-prop-3 .statement tag=07PE}

— 令 E、F、G 为三个局部凸空间、$\mathfrak{S}$ E 的有界子集族。令 u 为从 $E \times F$ 到 G 的单独连续双线性映射。以下属性是等效的：

a) 对于 G 中每个 0 的邻域 W 和每个集合 $M \in \mathfrak{S}$，F 中存在 0 的邻域 V，使得 $u(M \times V) \subset W$。

b) 对于每个集合$M \in \mathfrak{S}$，映射$x \mapsto u(x, .)$下的M的像是$\mathscr{L}(F; G)$的等连续子集。

c) 从 F 到 $\mathscr{L}_{\mathfrak{S}}(E; G)$ 映射 $y \mapsto u(., y)$ 是连续的。

a) 表示$y \mapsto u(., y)$在点 0处连续，因为$\mathscr{L}_{\mathfrak{S}}(E; G)$中邻域的定义为0（III，p. 13）；同样a)表示M在映射$x \mapsto u(x, .)$下的像在点0（III，p. 16）处等连续。

#### 定义 2 {#evt-iii-s5-def-2 .statement tag=07PF}

— 设 u 是从 $E \times F$ 到 G 的双线性映射。如果 u 单独连续并且它验证了 prop 的等价条件 a)、b)、c) 之一，则我们说 u 是 $\mathfrak{S}$ 次连续的。 3.

条件 c) 的支柱。图3表明，$\mathfrak{S}$-次连续双线性映射的概念仅通过$\mathscr{L}(E, G)$上的$\mathfrak{S}$拓扑依赖于$\mathfrak{S}$。

For every set $\mathfrak{T}$ of bounded subsets of F, we define similarly the notion of $\mathfrak{T}$-hypocontinuous mapping, by interchanging the roles of E and F in prop. 3. 如果单独连续的双线性映射 u 既是 $\mathfrak{S}$ 次连续又是 $\mathfrak{T}$ 次连续，则称其为 $(\mathfrak{S}, \mathfrak{T})$ 次连续。

从$E \times F$到$G$的每个*连续*双线性映射对于有界子集的集合的每个对$(\mathscr{S}, \mathscr{T})$来说都是$(\mathscr{S}, \mathscr{T})$-次连续的：对于0中的每个邻域$W$ $G$，$E$中存在0的邻域$U$，$F$中存在0的邻域$V$，使得$u(U \times V) \subset W$；因为每个集合$M \in \mathscr{S}$都是有界的，所以存在$\lambda > 0$使得$\lambda M \subset V$，所以

$$
u(M \times \lambda V) = u(\lambda M \times V) \subset u(U \times V) \subset W .
$$

逆命题一般为假（III、p. 47、练习 3）。

#### 命题 4 {#evt-iii-s5-prop-4 .statement tag=07PG}

*设$u$是从$E \times F$到$G$的$\mathscr{S}$-次连续双线性映射。对于每个集合 $M \in \mathscr{S}$，$u$ 到 $M \times F$ 的限制是连续的，并且对于 $F$ 的每个有界子集 $Q$，$u(M \times Q)$ 都以 $G$为界。*

第一个断言来自cor。 GT 3，X, § 2, No. 1。令$W$为$G$中0的邻域；通过假设、邻域$V$在$F$中存在0使得$u(M \times V) \subset W$。由于存在$\lambda \neq 0$使得$\lambda Q \subset V$，我们有$\lambda u(M \times Q) = u(M \times \lambda Q) \subset W$，这证明了命题的第二个部分。

#### 命题 5 {#evt-iii-s5-prop-5 .statement tag=07PH}

*设$u$是从$E \times F$到$G$的$(\mathscr{S}, \mathscr{T})$-次连续双线性映射。对于集合$M \in \mathscr{S}$、$N \in \mathscr{T}$、$u$的每个对在$M \times N$上均匀连续。*

命题紧随 prop. GT、X, § 2, No. 1 和 prop 的 2 个。 GT 5，X, § 2, No. 2。

#### 命题 6 {#evt-iii-s5-prop-6 .statement tag=07PI}

*如果$F$是桶状空间，则对于有界子集的每个集合$\mathscr{S}$，从$E \times F$到局部凸空间$G$的每个单独连续双线性映射$u$都是$\mathscr{S}$低连续的$E$.*

在其他字中，从$F$到$\mathscr{L}_b(E; G)$的*线性映射*$y \mapsto u(., y)$*是连续的*。

足以证明$E$在$x \mapsto u(x, .)$下的每个有界子集$M$的像在$\mathscr{L}(F; G)$中等连续（III，p. 30，命题3）。但是，凭借道具。 1 (III, p. 28) 这个像是$\mathscr{L}(F; G)$的简单有界子集，并且由于$F$是桶状的，$\mathscr{L}(F; G)$的每个简单有界子集是等连续的（III， p. 25，第 1)。

#### 注 {#evt-iii-s5-n3-rem-1 .statement tag=07PJ}

— 假设 $F$ 的拓扑是 $F$ 上最精细的局部凸拓扑，其中线性映射 $h_\alpha : F_\alpha \to F$ 是连续的（II，p. 27）。然后是 prop 的条件 *c)*。 3 (III,p. 30)表明，如果$E$和$G$是局部凸的，则双线性映射$u : E \times F \to G$是$\mathscr{S}$-次连续当且仅当每个双线性映射

$$
(x, y_\alpha) \mapsto u(x, h_\alpha(y_\alpha))
$$

从$E \times F_\alpha$到$G$是$\mathscr{S}$-低连续的。

现在假设$E$是局部凸空间，它是$E$的闭向量子空间的递增序列$(E_n)$的*严格*归纳极限（II， p. 33);那么每个集合 $M \in \mathscr{S}$ 都包含在 $E_n$ 之一中，并且受此子空间限制（III，p. 5，道具 6）。我们用$\mathscr{S}_n$表示$E_n$中包含的所有子集属于到$\mathscr{S}$的家族。

条件 a) 道具。图3（III，p. 30）表明，对于$u : E \times F \to G$为$\mathfrak{S}$次连续的双线性映射，$u$的每个限制$u_n : E_n \times F \to G$为$\mathfrak{S}_n$次连续是充分必要的。

### 4. 次连续双线性映射的扩张

#### 命题 7 {#evt-iii-s5-prop-7 .statement tag=07PK}

*设* $E, F, G$ *为三个局部凸空间*，$G$ *假设为Hausdorff*； *令* $E_0$ *（或$F_0$）为* $E$ *（或$F$）的稠密向量子空间。令*$u$*为从*$E \times F$*到*$G$的单独连续双线性映射。

1) *如果*$u(E_0 \times F_0) = \{0\}$，*则*$u = 0$。

2) *设* $\mathfrak{S}_0$ *是* $E_0$的有界子集族； *如果*$u$*到*$E_0 \times F_0$*的限制*是*$\mathfrak{S}_0$*-低连续，那么*$u$也是。

1) By hypothesis, for all $x \in E_0$, the continuous linear mapping $u(x, .)$ is null on $F_0$, hence on $F$: therefore for all $y \in F$, the continuous linear mapping $u(., y)$ is null on $E_0$, hence on $E$. 这就证明了$u = 0$。

2) 对于$G$中每个0的闭邻域$W$和每个集合$M \in \mathfrak{S}_0$，通过假设，$F_0$中存在0的邻域$V$使得$u(M \times V) \subset W$。但$\overline{V}$是$F$中0的邻域；对于每个$x \in M$，关系$u(\{x\} \times V) \subset W$意味着$u(\{x\} \times \overline{V}) \subset W$，因为$u(x, .)$是连续的并且$W$是闭集的；因此$u(M \times \overline{V}) \subset W$，证明$u$是$\mathfrak{S}_0$*-低连续的。

#### 命题 8 {#evt-iii-s5-prop-8 .statement tag=07PL}

*设* $E, F, G$ *为三个局部凸空间*； *假设* $G$ *是豪斯多夫且准完备*。 *Let* $E_0$ *(resp. $F_0$) be a dense vector subspace of* $E$ *(resp. $F$), $\mathfrak{S}_0$ *(resp. $\mathfrak{T}_0$) a family of bounded subsets of* $E_0$ *(resp. $F_0$) such that every point of* $E$ *(resp. $F$) is in the closure of an element of* $\mathfrak{S}_0$ *(resp. $\mathfrak{T}_0$). 那么每个* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-次连续双线性映射* $u$ *from* $E_0 \times F_0$ *into* $G$ *扩展唯一地到单独的连续双线性映射* $\overline{u}$ *from* $E \times F$ *into* $G$ *和* $\overline{u}$ *是* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-低连续*。

唯一性和 $\overline{u}$ 的次连续性由命题得出。 7；剩下的就是证明$\overline{u}$的存在。对于每个$y' \in F_0$，从$E_0$到$G$扩展的连续线性映射$x' \mapsto u(x', y')$唯一地到从$E$到$G$的连续线性映射$x \mapsto u_1(x, y')$（III，p. 8，道具 10）。紧接着，对于每个$x \in E$，从$F_0$到$G$的映射$y' \mapsto u_1(x, y')$是线性的；我们将证明它是连续的。到假设时，存在$M \in \mathfrak{S}_0$，因此$x \in \overline{M}$。对于$G$中每一个0的闭邻域$W$，通过假设，$F_0$中存在0的邻域$V$使得$u(M \times V) \subset W$；由于$x \mapsto u_1(x, y')$是连续的，我们推断出$u_1(\overline{M} \times V) \subset W$，特别是对于所有$y' \in V$，$u_1(x, y') \in W$。这就建立了我们的断言。凭借道具。 7、从$E \times F_0$到$G$的双线性映射$u_1$是$(\mathfrak{S}_0, \mathfrak{T}_0)$*-低连续的。我们以交换结束证明，证明的第一个部分中$E$和$F$的角色应用于$u_1$。

### 5. 映射 $(u, v) \mapsto v \circ u$ 的次连续性

#### 命题 9 {#evt-iii-s5-prop-9 .statement tag=07PM}

*设*$R, S, T$*为三个局部凸Hausdorff空间*。 *假设空间* $\mathscr{L}(R; S), \mathscr{L}(S; T), \mathscr{L}(R; T)$ *各自分配了拓扑的简单*（分别为*紧凑*、*有界*）收敛。 *然后双线性映射* $(u, v) \mapsto v \circ u$ *从* $\mathscr{L}(R; S) \times \mathscr{L}(S; T)$ *到* $\mathscr{L}(R; T)$ *是* $(\mathfrak{S}, \mathfrak{T})$-*次连续*，*其中* $\mathfrak{T}$ *是* $\mathscr{L}(S; T)$、*和* $\mathfrak{S}$ *族的等连续子集族有限*（或*紧凑，有界*）*子集*$\mathscr{L}(R; S)$。

我们首先证明$(u, v) \mapsto v \circ u$是$\mathfrak{T}$-低连续的。令 H 为 $\mathscr{L}(S; T)$ 中的等连续集合，令 W 为 T 中 0 的邻域，并令 M 为 R 的有限（紧凑、有界）子集。我们必须证明 S 中存在 0 的邻域 V，使得如果 $u(M) \subset V$ 且$v \in H$，然后$v(u(M)) \subset W$。但为此，对于所有 $v \in H$ 有 $v(V) \subset W$ 就足够了，并且这样的邻域的存在性是根据 H 的等连续性得出的。

为了证明$(u, v) \mapsto v \circ u$是$\mathfrak{S}$-次连续的，我们将证明，对于T中0的每个邻域W，R的每个有限（紧凑，有界）子集M和$\mathscr{L}(R; S)$的每个有限（紧凑，有界）子集L都存在一个有限（分别是紧凑、有界）S 的子集 N，使得关系 $v(N) \subset W$ 和 $u \in L$ 意味着 $v(u(M)) \subset W$。显然，只要 L 和 M 是，就足以证明我们可以取 $N = \bigcup_{u \in L} u(M)$，*即* 集合 N 是有限的（或紧凑的，有界的）。如果 L 和 M 是有限的，或者如果 M 在 R 中有界并且 L 在 $\mathscr{L}(R; S)$ 中有界，则这是直接的（对于有界收敛的拓扑，*cf.* III，p. 22）。最后，我们证明，如果 M 在 R 中是紧的，并且 L 在 $\mathscr{L}(R; S)$ 中是紧的，对于拓扑的紧致收敛，则 N 在 S 中是紧的。但是，如果 $u_M$ 是限制到 $u \in L$ 的 M，则从 L 到映射 $u \mapsto u_M$ 到从M到S的所有连续映射中的空间$\mathscr{C}(M; S)$，与拓扑一致收敛，是连续的；因此，在这个映射下，L的像是紧致的，然后我们的断言是从映射$(w, x) \mapsto w(x)$从$\mathscr{C}(M; S) \times M$到S的连续性得出的（GT，X, § 1, No. 6，道具9）。

在接下来的两个推论中，我们假设为prop。 9、空间、$\mathscr{L}(R; S)$、$\mathscr{L}(S; T)$、$\mathscr{L}(R; T)$*全部三个*指定为简单收敛的拓扑，或者所有三个紧凑收敛的拓扑，或者所有三个有界收敛的拓扑。

#### 推论 1 {#evt-iii-s5-prop-9-cor-1 .statement tag=07PN}

*对于* $\mathscr{L}(S; T)$ *映射* $(u, v) \mapsto v \circ u$ *从* $\mathscr{L}(R; S) \times H$ *到* $\mathscr{L}(R; T)$ *的每个等连续子集 H 都是连续的*。

这立即来自于 prop。 9（III、p. 32）和 4（III、p. 31）。

#### 推论 2 {#evt-iii-s5-prop-9-cor-2 .statement tag=07PO}

*假设S是桶装的。如果序列* $(u_n)$ *倾向于 u in* $\mathscr{L}(R; S)$ *和序列* $(v_n)$ *倾向于 v in* $\mathscr{L}(S, T)$，*则序列* $(v_n \circ u_n)$ *倾向于* $v \circ u$ *in* $\mathscr{L}(R; T)$。

事实上，序列$(v_n)$，简单地以$\mathscr{L}(S; T)$为界是等连续的，因为S是桶状的（III，p. 25，第1）；那么推论就是 cor 的推论。 1.

### 习题{#evt-iii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
