---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 6
section_title: Semi-simple Lie algebras
lang: zh
source: lie-i-iii
book_pages: 50-68, 102-109
pdf_pages: 0068-0086, 0120-0127
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SEMI-SIMPLE LIE ALGEBRAS
      page: 50
      pdf_page: 68
    - "no": 2
      title: SEMI-SIMPLICITY OF REPRESENTATIONS
      page: 51
      pdf_page: 69
    - "no": 3
      title: SEMI-SIMPLE ELEMENTS AND NILPOTENT ELEMENTS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 54
      pdf_page: 72
    - "no": 4
      title: REDUCTIVE LIE ALGEBRAS
      page: 56
      pdf_page: 74
    - "no": 5
      title: 'APPLICATION: A CRITERION FOR SEMI-SIMPLICITY OF REPRESENTATIONS'
      page: 58
      pdf_page: 76
    - "no": 6
      title: SUBALGEBRAS REDUCTIVE IN A LIE ALGEBRA
      page: 59
      pdf_page: 77
    - "no": 7
      title: EXAMPLES OF SEMI-SIMPLE LIE ALGEBRAS
      page: 60
      pdf_page: 78
    - "no": 8
      title: THE LEVI-MALCEV THEOREM
      page: 62
      pdf_page: 80
    - "no": 9
      title: THE INVARIANTS THEOREM
      page: 66
      pdf_page: 84
    - "no": 10
      title: CHANGE OF BASE FIELD
      page: 68
      pdf_page: 86
statements: 50
exercises: 27
content_sha256: beaf3b0fe5f79e8330cfd267d3ac6544df2df4af04894a9397dae924ef3f1257
translated_from: content/en/lie/I/06_s6_semi_simple_lie_algebras.md
translation_method: google
source_content_sha256: a9c8167085c5b67b76f2c398b6f6632816160cebdc605e7610218d0eb473ffb7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5941c1b93db7d7a7e97bd0fdb55b0ae3ec704129908710fc42342eda726ce0f3
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 6。 半单李代数

*回想一下，K 表示特征 0 的域，并且所有李代数都被假定为 K 上的有限维。*

### 1. 定义 / 半单李代数

#### 定义 1 {#lie-i-s6-def-1 .statement tag=09ZA}

*设g为李代数。 g 称为半单当且仅当 g 的唯一交换理想是 {0}。*

#### 注 {#lie-i-s6-n1-rem-1 .statement tag=09ZB}

(1) 代数 {0} is 半单. 维数 1 或 2 中的代数不是半单（cf. § 5, no. 1，例 1）。存在维数 3 个（cf. no. 7）中的半单代数。

(2) 半单代数有零中心，因此它的伴随物表示是忠实的。

(3) 如果$g_1, \ldots, g_n$是半单，$g = g_1 \times \cdots \times g_n$是半单：因为如果a是g的交换理想，则a的投影到$g_1, \ldots, g_n$约化到{0}。

#### 定理 1 {#lie-i-s6-thm-1 .statement tag=09ZC}

*设g为李代数。 The following 条件 are equivalent:*

(a) *g 为半单。*
(b) *根基 r of g is 零.*
(c) *杀死 g 的形式 $\beta$ 是非退化的。*

*此外，半单李代数等于其导出的理想值。*

(a) $\Rightarrow$ (b)：对于如果$r \neq \{0\}$，r 的最后一个非零导出代数是 g 的交换理想。

(b)$\Rightarrow$(c)：这是从§ 5, no. 5的命题5(b)得出的（同时证明了定理的最后一个断言）。

(c) $\Rightarrow$ (a)：这是从 § 4, no. 4 的命题 6 (b) 得出的。

#### 推论 {#lie-i-s6-n1-cor-1 .statement tag=09ZD}

*设g为有限维向量空间V上g的半单李代数和$\rho$表示。然后$\rho(g) \subset \mathfrak{sl}(V)$.*

当 x 为形式 $[y, z]$ ($y \in g, z \in g$) 时，线性形式 $x \mapsto \operatorname{Tr} \rho(x)$ ($x \in g$) 为零，因此在 $\mathscr{D}g = g$ 上。

#### 命题 1 {#lie-i-s6-prop-1 .statement tag=09ZE}

令$g$为半单李代数且$\varphi$为$g$的有限维忠实表示。那么与$\varphi$相关的$g$上的双线性形式是非简并的。

$g$ 相对于形式的正交是一个可解的理想（$§ 5$，no. 4，定理 2），因此是零。

#### 推论 1 {#lie-i-s6-prop-1-cor-1 .statement tag=09ZF}

令$g$为李代数，$\beta$其杀戮形式和$a$半单$g$的子代数。 $a$相对于$\beta$的正交$h$是$g$和$[a, h] \subset h$中$a$的补充子空间。如果$a$是$g$的理想，那么$h$也是$a$在$g$的中心化子。

令$\beta'$为$\beta$至$a$的限制：双线性形式与空间$g$上$a$的表示$x \mapsto \operatorname{ad}_g x$相关联。这个表示是忠实的，因此$\beta'$是非退化的（命题1）。因此$h$是$g$中$a$的补充。另一方面，如果 $x, y$ 在 $a$ 和 $z \in h$ 中，则

$$
\beta(x, [y, z]) = \beta([x, y], z) = 0,
$$

因为$[x, y] \in a$，所以$[y, z] \in h$，这证明了$[a, h] \subset h$。如果$a$是$g$的理想，我们知道$h$是$g$的理想（$§ 3$，命题7），并且$g$与$a \times h$一致。由于$a$的中心是零，所以$g$中$a$的扶正器是$h$。

#### 推论 2 {#lie-i-s6-prop-1-cor-2 .statement tag=09ZG}

半单李代数到半单李代数的每个扩张都是半单并且微不足道。

这紧随推论 1 而来。

#### 推论 3 {#lie-i-s6-prop-1-cor-3 .statement tag=09ZH}

如果$g$是半单，则$g$的每一个推导都是内部。

$\operatorname{ad} g$与$g$同构的，因此与半单同构，并且是$g$的推导的李代数$\delta$的理想（$§ 1$，命题1）。如果 $D \in \delta$ 与 $\operatorname{ad} g$ 的元素通勤，则对于所有 $x \in g$、$\operatorname{ad} D(x) = [D, \operatorname{ad} x] = 0$、从而 $D(x) = 0$；因此$D = 0$。然后从推论 1 得出推论 3。

### 2. 表示的半简单

#### 引理 1 {#lie-i-s6-lem-1 .statement tag=09ZI}

令 $g$ 为半单李代数。 $g$ 的伴随表示是半单。每个理想和$g$的每个商代数都是半单。

令$a$为$g$的理想。 $g$中$a$的正交$b$关于杀戮形式是$g$的一个理想，$a \cap b$是一个交换理想（$§ 3$，no. 6，命题7），因此零。因此$b$是$g$中$a$的补充。此外，由于$g$的杀戮形式是非退化的，所以它的限制到$a$和$b$（*代数*，章IX，$§ 4$， no. 1、推论至命题 1)，因此 $a$ 和 $b$ 为半单（no. 1、定理 1 和 $§ 3$、no. 6， 命题9)。

#### 引理 2 {#lie-i-s6-lem-2 .statement tag=09ZJ}

令$g$为李代数。那么下面两个条件是等价的：
(a) $g$ 的所有有限维线性表示都是半单。
(b) 给定余维 1 上 $g$ 的线性表示 $\varphi$ 和有限维向量空间 $V$ 和向量子空间 W，使得 $\rho(x)(V) \subset W$ 对于所有 $x \in g$，存在一条 W 的补线，该线在$\rho(g)$（因此被$\rho(g)$消灭）。

显然（a）意味着（b）。假设(b)成立。设$\sigma$为$g$在向量空间M和N向量子空间上的有限维表示，在$\sigma(g)$下是稳定的。令$\mu$为$\mathscr{L}(M)$上$g$的表示，规范地源自$\sigma$（§ 3, no. 3）：回想一下$\mu(x) = \mathrm{ad}_{\mathscr{L}(M)} \rho(x)$。设V（分别为W）为M的线性映射的$\mathscr{L}(M)$由……组成到N的子空间，其中限制到N为位似（分别为零）；那么对于所有 $x \in g$，W 在 V 和 $\mu(x)(V) \subset W$ 中具有余维 1。通过条件 (b)，存在$u \in V$，对于所有$x \in g$，它被$\mu(x)$ 湮灭，并且其限制到N 是非零位似。通过将$u$乘以合适的标量，可以假设$u$是M在N上的投影算子。说$\mu(x) \cdot u = 0$意味着$u$可以用$\sigma(x)$置换。因此，$u$的核是M中N的补充，对于所有$x \in g$，它在$\sigma(x)$下是稳定的。因此$\sigma$是半单。

#### 引理 3 {#lie-i-s6-lem-3 .statement tag=09ZK}

*令 g 为余维 1 的有限维向量空间 V 上 g 的半单李代数、$\rho$ 线性表示和 V 的 W 子空间，使得所有 $x \in g$ 都有 $\rho(x)(V) \subset W$。则存在W的补充线，其在$\rho(g)$下稳定。*

对于所有$x \in g$，令$\sigma(x)$为$\rho(x)$到W的限制。首先假设$\sigma$是简单的。如果$\sigma = 0$，那么$\rho(x)\rho(y) = 0$对于$g$中的所有$x, y$，因此$\rho(g) = \rho(\mathscr{D}g) = \{0\}$和我们的断言是显而易见的。如果$\sigma \neq 0$，则令n为$\sigma$的核，并令m为$g$中n的补理想（引理1）；则$\sigma$对m的$m \neq \{0\}$和限制是忠实的；与$\sigma$相关的双线性形式的限制到m是非简并的（命题1），因此可以形成与m和$\sigma$相关的卡西米尔元素c。通过§ 3, no. 7的命题12，$\sigma(c)$是W的自同构。另一方面，$\rho(c)(V) \subset W$。因此$\rho(c)$的核Z是W的补线；由于$g$的包络代数的c属于到中心，对于所有$x \in g$，$\rho(c)$可以与$\rho(x)$置换，因此Z在$\rho(g)$下是稳定的。

一般情况下，我们通过归纳对V的维数进行争论。令 T 为 W 的最小非零稳定子空间。令$\rho'$ 为$V' = V/T$ 上的商表示。然后，对于所有$x \in g$、$\rho'(x)(V') \subset W'$，其中$W' = W/T$是$V'$中的余维1。到归纳假设时，存在$Z'$线，它是$W'$的补充，并稳定在$\rho'(g)$之下。它在 V 中的逆像 Z 在 $\rho(g)$、包含于 T 下稳定，作为余维 1 的子空间、$Z \cap W = T$，因此对于所有 $x \in g$ 来说，$\rho(x)(Z) \subset T$ 是稳定的。由上证明，Z中存在T的补系，在$\rho(g)$下稳定；该行是V中W的补充，完成了证明。

#### 定理 2（H.韦尔）{#lie-i-s6-thm-2 .statement tag=09ZL}

*半单李代数的每个有限维线性表示都是完全可约的。*

这是从引理 2 和 3 得出的。

#### 定义 2 {#lie-i-s6-def-2 .statement tag=09ZM}

*李代数 g 被称为简单的，如果 g 的唯一理想是 {0} 和 g 并且如果进一步的 g 是不可交换的。*

一个简单的李代数就是半单。 代数{0}并不简单。

#### 命题 2 {#lie-i-s6-prop-2 .statement tag=09ZN}

*为了使李代数g成为半单，它是单代数中的乘积是必要且充分的。*

条件就足够了（no. 1、注 3）。相反，假设 g 为半单。由于 g 的伴随表示是半单，因此 g 是最小非零理想 $a_1, \ldots, a_m$ 的直和。然后g被识别为$a_i$（§ 1, no. 1）的乘积代数。 $a_i$ 的每个理想都是 g 的理想，因此零或等于 $a_i$。另一方面 $a_i$ 是不可交换的。因此$a_i$是简单的李代数。

#### 推论 1 {#lie-i-s6-prop-2-cor-1 .statement tag=09ZO}

*半单李代数是其简单理想$g_i$的乘积。 g 的每个理想都是 $g_i$ 中某些的乘积。*

$g = a_1 \times \cdots \times a_m$，其中$a_i$很简单。由于$a_i$的中心是零，所以g中$a_i$的扶正器是$j \neq i$的$a_j$的乘积。则设a为g的理想。如果它不是包含$a_i$，那么$a \cap a_i = \{0\}$，因此$[a, a_i] = \{0\}$，并且a包含在$j \neq i$的$a_j$的乘积中。由此可见，a 是 $a_i$ 中某些乘积。因此 g 的简单理想正是 $a_i$。

半单李代数的简单理想称为 g 的 *简单分量*。

#### 推论 2 {#lie-i-s6-prop-2-cor-2 .statement tag=09ZP}

*设g、$g'$是两个李代数、r和$r'$，它们的根基和f同态到$g'$。然后$r' = f(r)$.*

由于 $f(r)$ 可解，$f(r) \subset r'$。另一方面，$g/r$是半单（§ 5, no. 2，命题3），因此与$g/r$的商同构的$g'/f(r)$是半单（引理1），因此$f(r) \supset r'$（§ 5, no. 2，命题3）。

#### 注 {#lie-i-s6-n2-rem-1 .statement tag=09ZQ}

(1) 定理 2 承认逆命题：如果g的每个有限维表示都是半单，则g是半单。因为伴随表示是半单，g的每个理想都承认一个补充理想，因此可以被认为是g的商。如果 g 不是半单，则 g 承认非零交换律商，因此维数 1 的商。例如，现在维数 1 的李代数 K 承认非半单表示

$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

(2) 令 g 为 K 上的李代数，且 g 的 $\sigma$ 表示在向量空间 M 上。另一方面，令 $f$ 为 M 中 $g$ 的 K-线性映射，使得：

$$
f([x, y]) = \sigma(x) \cdot f(y) - \sigma(y) \cdot f(x)
$$

对于$g$中的所有$x, y$。 通过示例2的§ 1, no. 8，给出$\sigma$和$f$相当于给出$g$到$\mathfrak{af}(M)$的同态$x \mapsto (f(x), \sigma(x))$。 另一方面，我们已经看到（loc.cit.）$\mathfrak{af}(M)$的元素$(f(x), \sigma(x))$被规范地等同于$\mathfrak{gl}(N)$的元素$\rho(x)$（其中$N = M \times K$），其中M上的诱导$\sigma(x)$和映射 N 至 $f(x)$ 中的元素 $(0, 1)$。 那么$\rho$就是N上$g$的表示，这样对于所有$x \in g$来说$\rho(x)(N) \subset M$。

那么，如果$g$是半单，则存在（引理3）一条与N中M互补并被$\rho(g)$湮灭的线Z。在其他字中，*存在元素* $m_0 \in M$使得$(-m_0, 1) \in N$被$\rho(x)$湮灭，即*这样*

$$
f(x) = \sigma(x) \cdot m_0
$$

*对于所有人*$x \in g$。

*假设$K = \mathbf{R}$。设 G 是与李代数 g 连接的李群。考虑将 G 的同态 $\phi$ 解析为 M 相应的的仿射群 A 到 g 的同态 $x \mapsto (f(x), \sigma(x))$ 到 $\mathfrak{af}(M)$。上述结果可以用说解释，如果g为半单$\phi(G)$，则M的点固定。令H为$\mathbf{GL}(N)$的元素的集合，使得N的所有线性簇平行于M保持稳定。存在A到H的(§ 1, no. 8，例2)典范同构$\psi$。设Z是N中M的补线。可以说$\rho(g)$消灭Z等于说，$(\psi \circ \phi)(G)$使Z的点固定，因此（考虑$\psi$的定义）$\phi(G)$使投影固定到Z的交的点的M上，并且$M \times \{1\}$.*

### 3. 半单李代数中的半单元素和幂零元

#### 命题 3 {#lie-i-s6-prop-3 .statement tag=09ZR}

*设 M 大于 K 的有限维向量空间且$g$ 半单子代数 $\mathfrak{gl}(M)$。然后$g$包含半单及其元素的幂零分量。*

如果$K_1$是K的扩张，$g_{(K_1)}$的杀戮形式是$g$（§ 3, no. 8）的扩张到$g_{(K_1)}$，因此是非退化的；因此$g_{(K_1)}$是半单。因此，当基域是代数封闭时，证明命题 3 就足够了，我们今后将假设情况如此。

对于M的每一个子空间N，令$g_N$为$\mathfrak{gl}(M)$由……组成或元素的子代数，这使得N保持稳定，并且其限制到N有迹线零。如果 N 在 $g$ 下稳定，则$g = \mathscr{D}g$、$g \subset g_N$。然后令$g^*$为$\mathfrak{gl}(M)$和代数$g_N$中$g$标准化器的交，其中N穿过M的子空间的集合，在g下稳定。因为$x \in gl(M)$的半单（或幂零）分量 s（或n）是x中的多项式，没有常数项，并且ad s（或ad n）是ad x（$§ 5$）的半单（或幂幂）部分， no. 4, 引理 2), 显然$x \in g^*$隐含$s \in g^*$和$n \in g^*$;因此只要证明 $g^* = g$ 就足够了。由于 g 是 $g^*$、$g^* = a \times g$ 的半单理想值（no. 1、推论 1 到命题 1）。令 $a \in a$ 并使 N 为子空间，它是 M 的非零子空间中最小的，在 g 下是稳定的。 a 到 N 的限制是 Burnside 的定理恒等式的标量倍数，通过构造有迹零，因此是零，因为 K 的特征为 0。由于 M 是子空间的直和，例如 N，因此得出$a = 0$，因此$g^* = g$。

#### 推论 {#lie-i-s6-n3-cor-1 .statement tag=09ZS}

g 的元素 x 是 M 的半单（幂零的）自同态当且仅当 $ad_g x$ 是 g 的半单（幂零的）自同态。

令 s（或 n）为 $x \in g$ 的半单（或幂零）分量。然后是$s \in g$和$n \in g$（命题3）。那么$ad_g s$（或$ad_g n$）是$ad_g x$的半单（或幂幂）分量，乘以$§ 5$、no. 4的引理 2。如果 x 为半单（或幂零），则为 $ad_g x$。如果现在 $ad_g x$ 是半单（或幂零），则它等于 $ad_g s$（或 $ad_g n$），因此等于 $x = s$（或 $x = n$），因为 g 的伴随表示是忠实的。

#### 定义 3 {#lie-i-s6-def-3 .statement tag=09ZT}

设g为半单李代数。 g 的元素 x 称为半单（幂零的），如果对于 K 上有限维的每个 g 模 M，$x_M$ 是 M 的半单（幂幂）自同态。

#### 命题 4 {#lie-i-s6-prop-4 .statement tag=09ZU}

令 g、g' 为半单李代数，并将 g 的 f 同态代入 g'。如果 $x \in g$ 是半单（或幂零），那么 $f(x)$ 也是。如果 f 是满射，则 g' 的每个半单（幂零的）元素在 g 的半单（幂幂）元素的 f 下都是像。

如果$\rho$是g'的表示，$\rho \circ f$是g的表示，从而是第一个断言。如果 f 是满射，则存在 g' 的同态 g 到 g 中，使得 $f \circ g$ 是 g' 的恒等式同态（no. 1、推论 2 到命题 1），然后从第一个断言得出第二个断言。

#### 定理 3 {#lie-i-s6-thm-3 .statement tag=09ZV}

设g为半单李代数。

(a) 设 $x \in g$。如果存在 g 的忠实表示 $\rho$，使得 $\rho(x)$ 为半单（或幂零）自同态，则 x 为半单（或幂幂）。

(b) g 的每个元素都可以唯一地写为半单元素和幂零元的和，它们与一个另一个可交换。

假设 (a) 的假设成立。设$\sigma$为g的表示，b​​为$\sigma$的核和g的$\alpha$投影在b上的补理想。那么 $ad_g x$ 是半单（幂幂）乘推论到命题 3，因此 $ad_b \alpha(x)$ 是半单（幂幂）。作为$\sigma(x) = \sigma(\alpha(x))$，第一个断言从推论到命题3。然后第二个结果从命题3应用到忠实的表示。

### 4. 还原李代数

#### 定义 4 {#lie-i-s6-def-4 .statement tag=09ZW}

*如果它的伴随物表示是半单，则李代数被称为约简。*

#### 命题 5 {#lie-i-s6-prop-5 .statement tag=09ZX}

*令$g$为李代数，$r$为根基。以下条件是等效的：*
(a) $g$ 是还原的。
(b) $\mathscr{D}g$ 是半单。
(c) $g$是半单代数和交换代数中的乘积。
(d) $g$ 具有有限维表示，因此相关的双线性形式是非简并的。
(e) $g$ 有忠实的半单有限维表示。
(f) *$g$的幂零根基是零。*
(g) $r$ 是 $g$ 中的中心。

(a) $\Rightarrow$ (b): 如果$g$的伴随表示是半单，$g$是最小非零理想$a_i$的直和，因此$g$同构于乘积 $a_i$；并且$a_i$除了$\{0\}$和$a_i$之外没有理想，因此是简单的或可交换维数 1。因此，$\mathscr{D}g$等于那些简单的$a_i$中的乘积，因此是半单。

(b) $\Rightarrow$ (c): 如果 $\mathscr{D}g$ 是半单，$g$ 与 $\mathscr{D}g$ 的乘积同构李代数 $h$ (no. 1, 推论 1 到命题1); $h$ 与 $g/\mathscr{D}g$ 同构的，因此是可交换的。

(c) $\Rightarrow$ (d)：令$g_1$和$g_2$为与$\rho_i$相关的$g_i$上的$g_i$和$\beta_i$双线性形式的两个李代数、$\rho_i$有限维表示 ($i = 1, 2$); $\rho_1$和$\rho_2$可以认为是$g = g_1 \times g_2$的表示；让$\rho$成为他们的直和。显然，与$\rho$相关的$g$上的双线性形式是$\beta_1$和$\beta_2$的直和，因此如果$\beta_1$和$\beta_2$是非简并的，则它是非简并的。那么，为了证明蕴涵 (c) $\Rightarrow$ (d)，只需考虑以下 2 种情况即可： (1) $g$ 是半单；那么伴随表示承认与形式相关的杀戮形式，这是非退化的； （2）$g = K$；那么$g$在$K$上的恒等式表示有一个关联的双线性形式，它是非简并的。

(d) $\Rightarrow$ (e)：令$\rho$为$g$和$\beta$关联的双线性形式中的有限维表示；通过§ 4, no. 3的命题 4，存在$g$的有限维半单表示$\sigma$，使得$\sigma$的核$n$与$g$正交$\beta$。如果$\beta$是非退化的，那么$n = \{0\}$以及$\sigma$是忠实的。

(e) $\Rightarrow$ (f)：这是显而易见的。

(f) $\Rightarrow$ (g)：若$g$的幂零根基为零，则$\mathscr{D}g \cap r$为零（$§ 5$，no. 3，定理 1）；因为$[g, r] \subset \mathscr{D}g \cap r$，$r$是$g$的中心。

(g) ⇒ (a): 如果 r 是 g 的中心，则 g 的伴随表示与 g/r 的表示相同，即半单李代数 (§ 5, no. 2, 命题 3)；因此，这个表示是半单 (定理 2)。

#### 注 {#lie-i-s6-n4-rem-1 .statement tag=09ZY}

如果李代数 g 可以分解为可交换的李代数 a 和半单李代数 b 的乘积 a × b，则这个分解是唯一的。更准确地说，g 的中心等于 a 和 b 的中心的乘积，因此等于 a。还有$\mathscr{D}g = \mathscr{D}a \times \mathscr{D}b = b$。

#### 推论 {#lie-i-s6-n4-cor-1 .statement tag=09ZZ}

(a) 约化代数的每个有限乘积都是约约代数。
(b) 如果 g 是中心 c 的还原李代数，则 g 的每个理想都是其交与 c 和 $\mathscr{D}g$ 的直因子、乘积，并且是还原李代数。
(c) 约化李代数的每个商都是约化李代数。

例如，断言 (a) 由命题 5 的条件 (c) 得出。

假设 g 是可还原的。 设a为g的理想。 由于g的伴随表示是半单，a有一个补理想b，g可以用a×b来表示。 对于所有$x \in g$，令$\rho(x)$为$\mathrm{ad}_g x$到a的限制。 那么 $\rho$ 是 g 的半简单表示，它在 b 上为零，并在将 a 上的伴随表示传递给商时定义。 因此 a 是可还原的。 类似地，同构的 g/a 和 b 是还原的。 最后，令d、d'为a和b的中心；那么$a = d \times \mathscr{D}a, b = d' \times \mathscr{D}b, d \times d' = c, \mathscr{D}a \times \mathscr{D}b = \mathscr{D}g$；因此$a = (a \cap c) + (a \cap \mathscr{D}g)$。

#### 命题 6 {#lie-i-s6-prop-6 .statement tag=0A00}

设g为李代数，r为根基，s为幂零根基。
（一）$s = [g, r] = \mathscr{D}g \cap r$。
(b) s 是 g 相对于与 g 的有限维表示相关的双线性形式的正交线的交。

显然$[g, r] \subset \mathscr{D}g \cap r$。现在 $\mathscr{D}g \cap r = s$ 已由定理 1 个§ 5, no. 3 组成。设$g' = g/[g, r]$和f是g到$g'$的典范同态；那么$f(r)$是$g'$的根基$r'$（推论3到命题2，no. 2），因此$[g', r'] = \{0\}$和$r'$是$g'$的中心；因此 (命题 5) $g'$ 具有有限维忠实的半单表示、从而 $s \subset [g, r]$。这就证明了(a)。

令 t 为 g 相对于与 g 的有限维表示相关的双线性形式的正交线的交。然后 $s \subset t$ (§ 4, no. 3, 命题 4 (d))。另一方面，$g/s$ 具有有限维忠实的半单表示，因此 (命题 5) 有限维表示 $\rho$ 使得相关的双线性形式是非简并的；视为 g 的表示，$\rho$ 在 g 上有关联的双线性形式 $\beta$，g 相对于 $\beta$ 的正交为 s、从而 $t \subset s$。因此$t = s$。

即使$s \neq \{0\}$，g 上也可能存在非简并对称双线性形式 (习题 18 (c))。当然，这样的形式与g的任何表示无关。

#### 推论 {#lie-i-s6-n4-cor-2 .statement tag=0A01}

令$g, g'$为李代数，$s$（或$s'$）$g$（或$g'$）的幂零根基以及$g$的$f$同态到$g'$。
(a) 然后$s' = f(s)$。
(b) $g'$ 是可还原的当且仅当核 of $f$ 包含 $s$。

如果$r, r'$是$g, g'$的根基，则$s' = [g', r'] = [f(g), f(r)] = f([g, r]) = f(s)$。 断言(b)是(a)的直接的推论。

### 5. 应用：表示的半简单准则

#### 定理 4 {#lie-i-s6-thm-4 .statement tag=0A02}

令$g$为李代数，$r$为$g$、$g' = \rho(g)$和$r' = \rho(r)$的根基、$\rho$有限维表示。那么下面的条件是等价的：
(a) $\rho$ 为半单；
(b) $g'$ 是还原性的，其中心由半单自同态组成；
(c) $r'$ 由半单自同态组成；
(d) $\rho$至$r$中的限制为半单。

(a) $\Rightarrow$ (b)：如果 $\rho$ 是半单，则 $g'$ 可还原 (命题 5)； 1 和 $g'$ 生成的结合律代数是半单 (\emph{代数}, 章 VIII, § 5, no. 1, 命题 3)，因此它的中心是半单 (\emph{loc. cit.}, § 5, no. 4, 命题 12)，因此中心的元素是半单 (\emph{loc. cit.}, § 9, no. 1, 命题 2)。

(b) $\Rightarrow$ (c)：如果$g'$是还原性的，则其中心等于其根基，即$r'$、从而蕴涵(b)$\Rightarrow$(c)。

(c) $\Rightarrow$ (d)：假设$r'$ 由半单自同态组成。因为 $[g', r']$ 由幂零自同态 (no. 4, 命题 6), $[g', r'] = \{0\}$ 组成。那么蕴涵 (c) $\Rightarrow$ (d) 由 \emph{代数}, 章 VIII, § 9, no. 2, 定理 1 得出。

(d) $\Rightarrow$ (a)：令$s$为$g$的幂零根基以及$\rho$到$r$的$\rho'$限制。 $\rho(s)$的元素是幂零的，因此$s$包含在$\rho'$的最大的幂零理想中。由于$\rho'$是半单，$\rho'(s) = \{0\}$和$g'$是还原的（推论到命题6），因此$g' = a' \times r'$与$a'$半单（命题5）。设 $A'$（或 $R'$）为 1 和 $a'$（或 $r'$）生成的结合律代数。它是半单 (\emph{代数}, 章 VIII, § 5, no. 1, 命题 3)，因此 $A' \otimes_K R'$ 是半单 (\emph{loc.cit.}, § 7, no. 6, 推论 4到定理 3)，因此1和$g'$生成的结合律代数，即$A' \otimes_K R'$的商，是半单，这证明$\rho$是半单。

#### 推论 1 {#lie-i-s6-thm-4-cor-1 .statement tag=0A03}

令$g$为李代数，并且$\rho$和$\rho'$为$g$的两个有限维半单表示。那么$\rho$和$\rho'$的张量积就是半单。

设$r$为$g$中的根基。对于 $x \in r$、$\rho(x)$ 和 $\rho'(x)$ 为半单 (定理 4)，因此 $\rho(x) \otimes 1 + 1 \otimes \rho'(x)$ 为半单 (\emph{代数}, 章 VIII, § 9， 推论到定理 1)，因此 $\rho$ 和 $\rho'$ 的张量积是半单 (定理 4)。

#### 推论 2 {#lie-i-s6-thm-4-cor-2 .statement tag=0A04}

令$g$为$g$的李代数、$\rho$半单表示在有限维向量空间$V$、$T$和$S$张量以及对称的代数 $T$ 和$S$ 上的$g$ 的$V$ 和$\sigma_T$、$\sigma_S$ 表示规范地源自$\rho$。那么$\sigma_T$和$\sigma_S$就是半单，更准确地说，是有限维简单表示的直和。

令$T^n$为阶$n$的齐次张量的$T$由……组成子空间。这个子空间在$\sigma_T$下是稳定的，$\sigma_T$在$T^n$上定义的表示是半单（推论1）。因此，对于$\sigma_T$来说是推论，对于$\sigma_S$来说，它是商表示除以$\sigma_T$。

#### 推论 3 {#lie-i-s6-thm-4-cor-3 .statement tag=0A05}

令$g$为李代数、$\rho$和$\rho'$在空间、$M$和$M'$上$g$的两个有限维半单表示。那么$\mathscr{L}_K(M, M')$上的$g$的表示规范地源自$\rho$和$\rho'$是半单。

$g$-模块 $\mathscr{L}_K(M, M')$ 与 $g$-模块 $M^* \otimes_K M'$ (§ 3, no. 3, 命题 4) 被规范地标识，因此推论 3 源自推论 1。

#### 推论 4 {#lie-i-s6-thm-4-cor-4 .statement tag=0A06}

令$g$为李代数，$a$为$g$的理想，$\rho$半单表示为$g$。
(a) $\rho$ 至$a$ 中的限制 $\rho'$ 为半单。
(b) 如果$\rho$是简单的，$\rho'$是简单的表示的和同构于1另一个。

经过到商乘以$\rho$的核，$\rho$可以被认为是忠实的。那么 $g$ 是可还原的。设$g = g_1 \times g_2$，其中$g_1$是$g$的中心，$g_2$是半单。然后$a = a_1 \times a_2$，其中$a_1 \subset g_1$、$a_2 \subset g_2$和$a_1$是$a$的中心。 $\rho(g_1)$的元素，特别是$\rho(a_1)$的半单（定理4），因此$\rho'$是半单（定理4）。因此(a)。 断言 (b) 由 (a) 得出，使用 § 3, no. 1、推论到命题 1。

### 6. 子代数还原为李代数

#### 定义 5 {#lie-i-s6-def-5 .statement tag=0A07}

令$g$为李代数，且$h$是$g$的谎言子代数。如果$h$的表示$x \mapsto \operatorname{ad}_g x$是半单，$h$在$g$中被称为约简。

这个表示承认子表示是$h$的伴随表示。因此，如果 $h$ 在 $g$ 中可还原，则 $h$ 也可还原。另一方面，说李代数本身是还原性的，就相当于说是还原性的。

#### 命题 7 {#lie-i-s6-prop-7 .statement tag=0A08}

令$g$在向量空间$V$和$W$上约化$g$的$g$、$\rho$表示、李代数、$h$子代数 $V$ 的有限维子空间的和是简单的$h$ 模块。那么$W$稳定在$\rho(g)$以下。

令$W_0$为$V$的有限维简单子$h$模。我们需要证明 $\rho(x)(W_0) \subset W$ 对于所有$x \in g$。令 $M$ 表示向量空间 $g$ 通过 $g$ 上 $h$ 的表示 $x \mapsto \operatorname{ad}_g x$ 被视为 $h$ 模块。那么 $M \otimes_K W_0$ 就是半单 $h$-模（推论 1 到定理 4）。令$\theta$为$M \otimes_K W_0$的K-线性映射进入由$\theta(x \otimes w) = \rho(x)w$定义的V。这是一个 $\mathfrak{h}$ 模块同态，如果 $y \in \mathfrak{h}$ 那么：

$$
\begin{align*}
\theta([y, x] \otimes w + x \otimes \rho(y)w) &= \rho([y, x])w + \rho(x)\rho(y)w \\
&= \rho(y)\rho(x)w = \rho(y)\theta(x \otimes w).
\end{align*}
$$

因此 $\theta(M \otimes_K W_0)$ 是有限维半单 $\mathfrak{h}$ 模。因此$\theta(M \otimes_K W_0) \subset W$，即所有$x \in g$的$\rho(x)(W_0) \subset W$。

#### 推论 1 {#lie-i-s6-prop-7-cor-1 .statement tag=0A09}

*令$g$为李代数，$\mathfrak{h}$子代数在$g$和$\rho$中约简为$g$的有限维半单表示。那么$\rho$到$\mathfrak{h}$的限制就是半单。*

考虑$\rho$很简单的情况就足够了。我们采用记号V，命题的W。 4.令$W_1$为V中子空间在$\rho(\mathfrak{h})$下稳定的非零子空间中最小。然后$W_1 \subset W$，因此$W \neq \{0\}$，因此$W = V$。

#### 推论 2 {#lie-i-s6-prop-7-cor-2 .statement tag=0A0A}

*令$g$在$g$中还原为李代数，$\mathfrak{h}$子代数还原，在$\mathfrak{h}$中还原$\mathfrak{h}$的$\mathfrak{k}$子代数。那么 $\mathfrak{k}$ 就可以还原为 $g$。*

$g$上的$\mathfrak{h}$的表示$x \mapsto \mathrm{ad}_g x$是半单，因此它的限制到$\mathfrak{k}$是半单（推论1）。

### 7. 例 / 半单李代数

#### 命题 8 {#lie-i-s6-prop-8 .statement tag=0A0B}

*令$V$为有限维向量空间。那么 $\mathrm{gl}(V)$ 是还原的。它的中心是$V$同位的集合，它的派生代数是$\mathrm{sl}(V)$，后者是半单。*

$\mathrm{gl}(V)$的恒等式表示很简单，因此$\mathrm{gl}(V)$是还原性的，因此$\mathrm{gl}(V)$是其中心$c$及其派生代数$\mathscr{D}(\mathrm{gl}(V))$的直和。 中心 $c$ 是集合同位（*代数*、章 II, § 2, no. 5、推论 1 到命题 5）。显然$\mathscr{D}(\mathrm{gl}(V)) \subset \mathrm{sl}(V)$。如$\mathrm{sl}(V) \cap c = \{0\}$、$\mathscr{D}(\mathrm{gl}(V)) = \mathrm{sl}(V)$。因此$\mathrm{sl}(V)$是半单。

#### 例 {#lie-i-s6-n7-exa-1 .statement tag=0A0C}

我们将认同$\mathrm{sl}(K^2)$与阶2的矩阵李代数并追踪零。我们写

$$
X = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} \quad Y = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} \quad H = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

然后 $\mathrm{sl}(K^2)$ 的 $X, Y, H$ 形式基和

$$
[H, X] = 2X \qquad [H, Y] = -2Y \qquad [X, Y] = H.
$$

由于维数 1或2的代数不是半单（no. 1，*注 1*），$\mathrm{sl}(K^2)$很简单。事实上，$\mathrm{sl}(V)$对于$\dim V \geq 2$来说很简单，我们稍后会看到（cf.还有习题21和24）。

#### 命题 9 {#lie-i-s6-prop-9 .statement tag=0A0D}

令 V 为 K 上有限维 n 的向量空间，且 β 为 V 上的非简并对称（分别为交错的）双线性形式。令 g 为 x ∈ gl(V) 的李代数由……组成，使得 β(xm, m') + β(m, xm') = 0 对于 V 中的所有 m、m'。那么 g 是还原的； g 是偶数半单，除非 β 是对称且 n = 2 的情况。

对于所有 u ∈ gl(V) 令 u* 表示其相对于 β 的伴随；那么 Tr(u) = Tr(u*) by 命题 7 of 代数, 章 IX, § 1, no. 8。 条件

$$
\beta(um, m') + \beta(m, um') = 0
$$

对于所有 m，V 中的 m' 意味着$u + u^* = 0$。特别是，如果$v \in \mathrm{gl}(V)$，则$(v - v^*)^* = v^* - v$，因此$v - v^* \in g$。然后令 u 为 g 的元素，关于与 g 的恒等式表示相关的双线性形式 φ，与 g 正交。对于所有$v \in \mathrm{gl}(V)$，$\mathrm{Tr}\,u(v - v^*) = 0$，因此

$$
\mathrm{Tr}(uv) = \mathrm{Tr}(uv^*) = \mathrm{Tr}(uv^*)^* = \mathrm{Tr}(vu^*) = -\mathrm{Tr}(vu) = -\mathrm{Tr}(uw)
$$

因此$\mathrm{Tr}(uw) = 0$。由此可见 $u = 0$，因此 φ 是非简并的。因此 g 是可还原的 (命题 5)。仍有待证明 g 的中心是零（除非 β 对称且$n = 2$）。通过扩展基域，我们可以假设 K 是代数封闭的。

(a) 当β对称时，可以用$K^n$上的双线性形式和矩阵$I_n$相对于典范基（代数、章IX, § 6、推论1至定理1）进行识别。在这些下，条件 g 被识别为斜对称矩阵（$§ 3$，no. 4，例 1）的李代数。设 $U = (u_{ij}) \in g$；我们利用 U 与矩阵 $(v_{ij}) \in g$ 通勤的事实，除了 $v_{i_0j_0}$ 和 $v_{j_0i_0}$ ($i_0 \neq j_0$) 分别等于 1 和 -1 之外，所有元素都是零。我们发现$u_{i_0j} = u_{j_0i} = u_{i_0} = u_{j_0} = 0$对应于$i \neq i_0, j_0$和$j \neq i_0, j_0$。如果$n > 2$，对于所有不同的指标$i_0$和$j$，存在不同的指标i和$j_0$使得$i \neq i_0, j_0 \neq j, j_0 \neq i_0$；因此$u_{i_0j} = 0$。这就证明了g的中心的元素是零。

(b) 当β为交错的和$n = 2m$时，β可以用$K^{2m}$上的双线性形式和矩阵$\begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix}$相对于典范基（代数，章IX, § 5， 推论 1 至定理 1)。在这些条件 g 被识别为形式 $U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$ 矩阵李代数，其中$D = -{}^tA$，B 和C 是对称的（$\mathbf{M}_m(K)$ 中的$A, B, C, D$）（$§ 3$， no. 4、例 1)。我们首先使用 U 与矩阵 $\begin{pmatrix} X & 0 \\ 0 & -{}^tX \end{pmatrix}$ 通勤的事实，其中 $X \in \mathbf{M}_m(K)$。然后$AX = XA, CX = -{}^tXC, XB = -B\cdot{}^tX$；由于这些等式对于所有 X 都成立，因此 A 是标量矩阵 $\lambda I_m$。我们现在使用 U 与矩阵 $\begin{pmatrix} 0 & Y \\ 0 & 0 \end{pmatrix}$ 通勤的事实，其中

Y 是 $\mathbf{M}_m(\mathbf{K})$ 的对称矩阵。然后$\lambda Y = YC = CY = 0$。这首先证明$\lambda = 0$。此外，对于所有 $X \in \mathbf{M}_m(\mathbf{K})$，$X + {}^tX$ 是对称的，因此$XC = -{}^tXC$。使用上面获得的方程$CX = -{}^tXC$，我们看到$C$与$\mathbf{M}_m(\mathbf{K})$的每元素进行交换，因此$C$是标量矩阵，从$YC = 0$开始必然是零。类似地证明$B = 0$。

对于 $\beta$ 对称和 $n = 2$，$g$ 为维数 1，因此可交换。对于其他情况cf.习题25和26。

### 8. 列维-马尔切夫定理

令 E 为 $\mathbf{R}$ 上的完全范数向量空间，$u$ E 的连续自同态。我们已经看到（实数变量的函数，章 IV, § 2, no. 6）序列 $\frac{u^n}{n!}$ 可求和$\mathscr{L}(E)$ 我们写了

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

现在令 E 为域 K 上的向量空间以及 E 的 $u$ 幂零自同态。 级数 $\sum_{n=0}^\infty \frac{u^n}{n!}$ 只有非零项的有限数，因此我们可以写

$$
e^u = \exp u = \sum_{n=0}^\infty \frac{u^n}{n!}.
$$

如果 $K = \mathbf{R}$ 并且 E 是完备且规范的，则该定义与上述一致。如果 $v$ 是与 $u$ 交换的 E 的另一个幂零自同态，则：

$$
e^{u+v} = \left( \sum_{n=0}^\infty \frac{u^n}{n!} \right) \left( \sum_{p=0}^\infty \frac{v^p}{p!} \right) = \sum_{n,p=0}^\infty \frac{u^n v^p}{n! p!}
$$
$$
= \sum_{q=0}^\infty \frac{1}{q!} \left( \sum_{n+p=q} \binom{q}{n} u^n v^p \right) = \sum_{q=0}^\infty \frac{1}{q!} (u+v)^q = e^{u+v}.
$$

特别是，$e^u e^{-u} = e^{-u} e^u = e^0 = 1$ 因而$e^u$ 始终是 E 的自同构。

如果进一步 E 是（不一定结合）代数并且 $u$ 是 E 的（幂零）推导，则 $e^u$ 是代数 E 的自同构。 对于 if $x, y \in E$ 那么

$$
u^p(xy) = \sum_{r+s=p} \binom{p}{r} u^r(x) u^s(y)
$$

对于每个整数$p \geqslant 0$（莱布尼茨的公式）。由此可见

$$
e^{u}(xy) = \sum_{p \geqslant 0} \frac{1}{p!} u^p(xy) = \sum_{p \geqslant 0} \sum_{r+s=p} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!}
$$

$$
= \sum_{r,s=0}^{\infty} \frac{u^r(x)}{r!} \frac{u^s(y)}{s!} = e^{u}(x)e^{u}(y)
$$

从而我们的断言。

现在让 $g$ 为李代数。如果$x$属于对$g$的幂零根基来说，$g$的推导$\mathrm{ad}_g x$是幂零的。因此我们可以做出以下定义：

#### 定义 6 {#lie-i-s6-def-6 .statement tag=0A0E}

*特殊的$g$自同构是形式$e^{\mathrm{ad}\, x}$$g$自同构，其中$x$处于$g$的幂零根基。*

显然，特殊的自同构使$g$的每一个理想都保持稳定。

#### 定义 7 {#lie-i-s6-def-7 .statement tag=0A0F}

*设$g$为李代数，$r$为根基。 $g$ 的列维子代数是 $g$ 的任意子代数对 $r$ 的补充。*

Levi 子代数与 $g/r$ 同构的，因此是半单。由于半单子代数在公共的和$r$中只有0，因此每个半单子代数$h$使得$g = r + h$是Levi子代数；因而，Levi 子代数在满同态下的像是 Levi 子代数。

#### 定理 5（列维-马尔切夫）{#lie-i-s6-thm-5 .statement tag=0A0G}

*李代数$g$总是有李维斯子代数$s$。每个 Levi 子代数 $g$ 是像 $s$ 在特殊的自同构下。*

让$r$表示$g$的根基。我们首先处理两种特殊情况。

（一）$[g, r] = \{0\}$。

到命题 5 时，$g$ 就是其中心 $r$ 的乘积 $\mathscr{D}g$，即半单。因而 $\mathscr{D}g$ 是 Levi 子代数。此外，如果$s'$是半单子代数，则$s' = \mathscr{D}s'$（定理1），因而$s' \subset \mathscr{D}g$和$\mathscr{D}g$是$g$的唯一列维子代数。

(b) $[g, r] \neq \{0\}$ 以及$r$ 中包含的$g$ 的唯一理想是$\{0\}$ 和$r$。

那么$g$的$[g, r] = r,\ [r, r] = \{0\}$和中心就是零。 令$M$（或$N$）为$\mathscr{L}(g)$的子空间，由$g$到$r$的线性映射组成，其对$r$的限制是相似性（或零）；因此，$N$ 是 $M$ 中的余维 1。 对于$m \in M$，令$\lambda(m)$表示由$m$定义的位似与$r$的比率。 令$\sigma$为$g$在$\mathscr{L}(g)$上的表示，从伴随表示规范导出；回想一下，$\sigma(x).u = [\mathrm{ad}_g x, u]$适用于所有$x \in g$和所有$u \in \mathscr{L}(g)$。

显然 $\sigma(x)(M) \subset N$ 对于所有$x \in g$。此外，如果 $x \in r, y \in g$ 和 $u \in M$，则
$$
(\sigma(x).u)(y) = [x, u(y)] - u([x, y]) = -\lambda(u)[x, y]
$$
从 $[r, r] = \{0\}$ 开始； (4) 可以写成：
$$
(x).u = -\mathrm{ad}(\lambda(u).x).
$$

由于$g$的中心是零，$r$的映射$x \mapsto \mathrm{ad}_g x$定义双射$\phi$到$\mathscr{L}(g)$的子空间$P$。 这个子空间在$\sigma(g)$下是稳定的，并且包含在$N$中，因为$r$是交换理想，并且（5）表明$\sigma(x)(M) \subset P$对于$x \in r$。 因而，$M/P = V$上的$g$的表示源自$\sigma$，因此是$r$上的零和半单代数$g/r$上的定义表示$\sigma'$ $V$。 For all $y \in g/r$, the space $\sigma'(y)(V)$ is contained in $N/P$, which is of codimension 1 in $V$. 因而，(no. 2，引理 3) 存在$u_0 \in M$，使得对于所有$x \in g$ 都有$\lambda(u_0) = -1$ 和$\sigma(x).u_0 \in P$。 映射 $x \mapsto \phi^{-1}(\sigma(x).u_0)$ 是$g$ 的线性映射到$r$。 由(5)可知，限制到$r$是$r$的恒等映射。 因此它的核是$g$的子空间$s$对$g$中$r$的补充。 由于$s$是$x \in g$的集合，因而$\sigma(x).u_0 = 0$，$s$是$g$的子代数，因此Levi 子代数为$g$。

设$s'$为另一个列维子代数。对于所有$x \in s'$，令$h(x)$为$r$的唯一元素，使得$x + h(x) \in s$。由于 $s$ 是子代数并且 $r$ 是可交换的，对于 $s'$ 中的 $x, y$：
$$
[x + h(x), y + h(y)] = [x, y] + [x, h(y)] + [h(x), y] \in s
$$
因此
$$
h([x, y]) = (\mathrm{ad}\, x).h(y) - (\mathrm{ad}\, y).h(x).
$$
到no. 2的注2，存在$a \in r$，使得$h(x) = -[x, a]$对于所有$x \in s'$。然后：
$$
x + h(x) = x + [a, x] = (1 + \mathrm{ad}\, a).x.
$$
由于$r$是可交换的，$(\mathrm{ad}\, a)^2 = 0$因此$1 + \mathrm{ad}\, a = e^{\mathrm{ad}\, a}$。与$r = [g, r]$一样，$e^{\mathrm{ad}\, a}$是$g$的特殊自同构。由(6)此特别自同构映射$s'$至$s$。

(c) 一般情况：

我们以归纳对根基的维数$n$争论。没有什么可以证明$n = 0$是否成立，因此可以假设定理对于李代数成立，而根基是维数$< \dim r$。通过(a)，足以考虑$[g, r] \neq \{0\}$的情况。由于$[g, r]$是幂零的（no. 4，命题6），所以它的中心$c$是$\neq \{0\}$。令 $m$ 为 $c$ 中包含的 $g$ 的最小非零理想。如果$m = r$，我们就有情况(b)。因此，设$m \neq r$，并设$f$为$g$的典范映射到$g' = g/m$。 $g'$中的根基是$r' = r/m$。到归纳假设，$g'$有了李维斯子代数$l'$。那么 $b = f(l')$ 是 g 包含于 m 的子代数，使得 h/m = h' 是半单，因此 m 为根基。通过归纳假设 h = m + s，其中 s 为半单子代数。那么等式 g' = r' + h' 意味着 g = r + h = r + m + s = r + s，因此 s 是 g 的 Levi 子代数。

令 s' 为 g 的另一个 Levi 子代数。那么 f(s) 和 f(s') 是 g' 的两个列维子代数，并且存在归纳假设 a' ∈ [g', r'] 使得 e^{ad\alpha'}(f(s')) = f(s)。如果 a ∈ [g, r] 使得 f(a) = a'，则有：

s_1 = e^{ada}(s') \子集 m + s = h。

那么 s_1 和 s 是 h 的两个 Levi 子代数并且通过归纳假设存在 b ∈ m 使得 e^{adb}(s_1) = s。因此 s = e^{adb}.e^{ada}(s')。最后，由于 m 在 [g, r] 的中心中，因此 e^{adb}.e^{ada} = e^{ad(b+a)} 且 b + a ∈ [g, r]，从而完成证明。

#### 推论 1 {#lie-i-s6-thm-5-cor-1 .statement tag=0A0H}

令 s 为 g 的 Levi 子代数和 g 的 h 半单子代数。
(a) 在 s 的子代数上存在 g 映射 h 的特殊自同构。
(b) h 包含在 g 的 Levi 子代数中。

令 r 为 g 的根基，a = h + r，即 g 的子代数。那么 a/r 是半单并且 r 是可解的，因此 r 是 a 的根基并且 h 是 a 的 Levi 子代数。另一方面，a ∩ s = h' 是 a 中 r 的补充子代数，因此也是 a 的 Levi 子代数。则存在 (定理 5) a ∈ [a, r] 使得 e^{ada} 映射 h 到 h' 上。现在 a ∈ [g, r]; e^{ada} 映射 h 到 s 的子代数上，并且 e^{-ada}(s) 是 g 包含于 h 的 Levi 子代数。

#### 推论 2 {#lie-i-s6-thm-5-cor-2 .statement tag=0A0I}

为了使g的子代数h成为g的列维子代数，h是g的最大半单子代数是必要且充分的。

这紧接着推论 1。

#### 推论 3 {#lie-i-s6-thm-5-cor-3 .statement tag=0A0J}

令 g 为李代数，m 为 g 的理想值，使得 g/m 为半单。然后将 g 包含子代数补充到 g 中的 m 中。在其他字中，半单李代数中的每个扩张都是无关紧要的。

令 s 为 g (定理 5) 的列维子代数。它的典范像（g/m）是列维子代数，因此等于 g/m，因此 g = s + m。那么 s 中理想 m ∩ s 的补充的理想是 g 中 m 补充的子代数。

#### 推论 4 {#lie-i-s6-thm-5-cor-4 .statement tag=0A0K}

设g为李代数，r为根基，s为g的列维子代数，m为g的理想。那么 m 是 m ∩ r 的直和，m ∩ r 是它的根基，m ∩ s 是 m 的 Levi 子代数。

我们知道 m ∩ s 是 m 的根基（§ 5, no. 5、推论 3 到命题 5）。设 h 为 m 的 Levi 子代数，s' 为 g 包含于 h (推论 1) 的 Levi 子代数。 代数 m ∩ s' 是 s' 的理想，因此是半单，包含于 h，因此等于 h。因此 m 是 $m \cap r$ 和 $m \cap s'$ 中的直和。 $s$ 上存在特殊的自同构映射 $s'$；这个自同构留下$r$和$m$不变；因此，$m$是$m \cap r$和$m \cap s$的直和，$m \cap s$是$m$的列维子代数。

### 9. 不变量定理

令 $g$ 为李代数，且向量空间 $M$ 上 $g$ 的 $\rho$ 表示。对于$g$的简单表示的每个类$\delta$，令$M_\delta$为类$\delta$的$M$的同型分量。 $M$的不变量元素的子空间$M_0$就是$M_{\delta_0}$，其中$\delta_0$表示空间上的$g$的零表示的类维数1。

#### 引理 4 {#lie-i-s6-lem-4 .statement tag=0A0L}

*令$\rho, \sigma, \tau$为向量空间$M, N, P$上$g$的表示。假设我们在 $P$ 中得到了 $M \times N$ 的 $K$ 双线性映射 $(m, n) \mapsto m.n$，使得*

$$
(\rho(x)m).n + m.(\sigma(x)n) = \tau(x)(m.n)
$$

*对于所有$m \in M, n \in N, x \in g$。*

(a) *如果 $m_0 \in M_0$，映射 $n \mapsto m_0.n$ 是$g$-模块同态。*

(b) *如果$n \in N_\delta$，则$m_0.n \in P_\delta$。*

(c) *如果$M$是代数（不一定是结合的）代数且$\rho(x)$是$M$的推导，则$M_0$是$M$的子代数并且每个$M_\delta$都是右和左$M_0$-模块。*

对于 $m_0 \in M_0, n \in N$ 和 $x \in g$，

$$
\tau(x)(m_0.n) = m_0.(\sigma(x)n),
$$

从而（一）。 断言 (b) 由 (a) 得出 (*代数*, 章 VIII, § 3, no. 4, 命题 10)。如果$N = P = M$和$\sigma = \tau = \rho$，断言(b)给出断言(c)作为特殊情况。

#### 引理 5 {#lie-i-s6-lem-5 .statement tag=0A0M}

*进一步假设 $\sigma$ 和 $\tau$ 为半单，因此 $N$（分别为 $P$）为 $N_\delta$（分别为 $P_\delta$）的直和。对于所有$n \in N$（或$p \in P$），令$n^\natural$（或$p^\natural$）为其$N_0$（或$P_0$）中的分量。让$m_0 \in M_0$。然后对于所有$n \in N$，$(m_0.n)^\natural = m_0.n^\natural$。*

通过线性，足以考虑 $n \in N_\delta$ 的情况。如果 $\delta \neq \delta_0$、$n^\natural = 0$ 和 $m_0.n \in P_\delta$ (引理 4)，则$(m_0.n)^\natural = 0 = m_0.n^\natural$。如果 $\delta = \delta_0$、$n^\natural = n$ 和 $m_0.n \in P_0$ (引理 4)，则$(m_0.n)^\natural = m_0.n = m_0.n^\natural$。

#### 定理 6 {#lie-i-s6-thm-6 .statement tag=0A0N}

*令$g$为李代数、$V$半单$g$-有限维在$K$、$S$的模$V$和$x_S$的对称代数推导 / $S$ 其中扩展 $x_V$（因此 $x \mapsto x_S$ 是 $S$ 上的 $g$ 表示）。*

(a) *$S$的不变量代数$S_0$由元素的有限数生成。*

(b) *对于有限维$g$简单表示超过$K$的每个类$\delta$，令$S_\delta$为类$S$的同型分量 $\delta$。那么$S_\delta$是一个有限生成的$S_0$-模块。*

令 $\overline{S} \subset S$ 为 $S$ 的元素的理想，且没有常数项。令$I$为由$S_0 \cap \overline{S}$生成的$S$的理想，并令$(s_1, s_2, \ldots, s_p)$为理想I的生成元的有限系统（交换代数，章III, § 3）。可以假设 s_i 属于到 S_0 ∩ S̄ 和 是同质的（x_S 保留次数，因此每个 S_δ 都是分级的子模）。令S_1为1和s_i生成的S的子代数。那么S_1⊂S_0。我们证明 S_1 = S_0。为此，我们证明 S_0 的每个齐次元素 s 都在 S_1 中，通过归纳对 s 的次数 n 进行论证。如果 n = 0，我们的断言是显而易见的。因此，假设 n > 0，并且当 s 的次数 < n 时，我们的断言已被证明。由于 s ∈ I，s = $\sum_{i=1}^{p} s_i s'_i$，其中 s'_i 是 S 的元素，可以假设是齐次的，且 deg(s'_i) = deg(s) − deg(s_i) < n。可以应用引理 5，因为g模S为半单（no. 5、推论2至定理4）；在这个引理的记号中，

$$
s = s^{\natural} = \sum_{i=1}^{p} (s_i s'_i)^{\natural} = \sum_{i=1}^{p} s_i {s'_i}^{\natural}.
$$

{s'_i}^{\natural} 是 S_0 的元素，它们是同质的并且次数 < n（因为每个 S_δ 都是分级的子模）。因此，它们在归纳假设处位于 S_1。因此s ∈ S_1，证明(a)。

现在我们考虑有限维空间 M 上类 δ 的 g 的简单表示。令 L = $\mathscr{L}_K(M, S)$。对于所有 s ∈ S 和所有 f ∈ L，令 sf 为 L 的元素，定义为 (sf)(m) = s.f(m) (m ∈ M)；因此在L上定义了一个S模块结构；由于 M 是 K 上的有限维，显然 L 是有限生成的 S 模，因此是诺特 S 模，因为环 S 是诺特。另一方面，L具有规范的g-模结构。对于每个整数 n ≥ 0 令 S^n 为次数 n 的 S 齐次元素集合；则 g 模数 $\mathscr{L}_K(M, S^n)$ 为半单（no. 5、推论 3 至定理 4），因此 g 模数 L 为半单。此外，对于 s ε S、f ε L、x ε g 和 m ε M，

$$
(x_L(sf))(m) = x_S((sf)(m)) - (sf)(x_M m)
= x_S(s.f(m)) - s.f(x_M m)
= (x_S s).f(m) + s.(x_S f(m)) - s.f(x_M m)
= ((x_S s)f)(m) + (s(x_L f))(m)
$$

因此$x_L(sf) = (x_S s)f + s(x_L f)$。因此我们可以申请引理5。

L的不变量元素的子集 L_0只是g模M的同态到g模S的集合。因此，如果φ表示M ⊗_K L在S上的典范同态， $\phi(M \otimes_K L_0) = S_\delta$。由于 显然是一个 S 模同态，因此足以证明 L_0 是一个有限生成的 S_0 模。令J为L_0生成的L的子S模。由于L是诺特S模，因此存在L_0生成的的元素的有限序列(f_1,...,f_q) S模J。令L_1为由f_1、\ldots、f_q生成的S_0模。然后 L_1 \子集 L_0。另一方面，如果 f \in L_0，则 $f = \sum_{i=1}^q s_i f_i$ 和 $s_i \in S$ 对于所有 $i$ ，因此通过引理 5，其记号我们采用：

$$
f = f^\mathfrak{h} = \left( \sum_{i=1}^q s_i f_i \right)^\mathfrak{h} = \sum_{i=1}^q s_i^\mathfrak{h} f_i \in L_1.
$$

因此$L_0 = L_1$，因此$L_0$是有限生成的$S_0$模块。

### 10. 基域变换

设$K_1$是$K$的交换律扩张。为了使$K$之上的李代数$g$成为半单，$g_{(K_1)}$为半单是充分必要的；因为$g_{(K_1)}$的杀戮形式$\beta_1$是由$g$的杀戮形式$\beta$衍生而来，通过将基域从$K$延伸到$K_1$；因此$\beta_1$是非简并的当且仅当$\beta$是非简并的（*代数*，章IX, § 1, no. 4，推论到命题3）。

如果 $g_{(K_1)}$ 是简单的，$g$ 由上式可知是半单，不能是两个非零理想的乘积，因此 $g$ 是简单的。另一方面，如果 $g$ 很简单，$g_{(K_1)}$（即半单）可能并不简单（习题 17 和 26 (b)）。

令$g$为李代数，$r$为根基。那么$r_{(K_1)}$就是$g_{(K_1)}$(§ 5, no. 6)的根基。因此，如果$s$表示$g$的幂零根基，则$g_{(K_1)}$的幂零根基就是$[g_{(K_1)}, r_{(K_1)}] = [g, r]_{(K_1)} = s_{(K_1)}$。由此可见，当且仅当 $g_{(K_1)}$ 是还原的时，$g$ 是还原的。

令$g$为李代数且$h$子代数。回想一下，$h$的表示是半单当且仅当通过将基域延伸到$K_1$而得到的$h_{(K_1)}$的表示是半单。因此，当且仅当$h_{(K_1)}$在$g_{(K_1)}$中还原时，$h$在$g$中还原。

现在令 $K_0$ 为 $K$ 的子域，使得 $[K : K_0]$ 是有限的。令 $g$ 为李代数，$g_0$ 为（有限维的）李代数，通过将基域从 $K$ 限制为 $K_0$ 衍生自 $g$。 $g$的每个交换理想都是$g_0$的交换理想；反之，如果$a_0$是$g_0$最小的向量子空间的交换理想超过$g$的$K$，包含$a_0$是$g$的交换理想；因此$g$是半单当且仅当$g_0$是半单。如果 $g_0$ 很简单，那么显然 $g$ 很简单。相反，假设 $g$ 很简单。我们证明 $g_0$ 是简单的。设$a_0$为$g_0$中的简单分量。对于所有 $\lambda \in K^*$，$\lambda a_0$ 是 $g_0$ 的理想，并且

$$
[a_0, \lambda a_0] = \lambda [a_0, a_0] = \lambda a_0 \neq \{0\},
$$

因此$\lambda a_0 \supset a_0$，因此从$\dim_{K_0}(\lambda a_0) = \dim_{K_0} a_0$开始为$\lambda a_0 = a_0$。现在由$a_0$生成的$g$的向量子空间是$g$的非零理想，因此是$g$的整体。因此$g = a_0$，这证明了我们的断言。

### 习题 {#lie-i-s6-exercises}

§ 6 的约定仍然有效，除非另有提及。

参见[习题为 § 6](exercises/s6/)。
