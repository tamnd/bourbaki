---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 4
section_title: Product of topological spaces
lang: zh
source: top-i-iv
book_pages: 43-50, 125-127
pdf_pages: 0049-0056, 0131-0133
extraction: ocr
subsections:
    - "no": 1
      title: PRODUCT SPACES
      page: 43
      pdf_page: 49
    - "no": 2
      title: SECTION OF AN OPEN SET; SECTION OF A CLOSED SET; PROJECTION OF AN OPEN SET. PARTIAL CONTINUITY
      page: 46
      pdf_page: 52
    - "no": 3
      title: CLOSURE IN A PRODUCT
      page: 47
      pdf_page: 53
    - "no": 4
      title: INVERSE LIMITS OF TOPOLOGICAL SPACES
      page: 48
      pdf_page: 54
statements: 21
exercises: 10
content_sha256: 4df9ddbab76214c842b4d62667bce6e96ed2a57aa392ff5d305b65eb5385ea27
translated_from: content/en/top/I/04_s4_product_of_topological_spaces.md
translation_method: google
source_content_sha256: ca28b3bed17cb5f1025ef827c13e6c41b2a4a8dcca42f1668734a8ba2d7c3fa4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: ea80a5a12475ef9d5c2637313692e0d4b1b3128c62928bf3cc94a55803f0a55e
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 拓扑空间的乘积

### 1. 乘积空间

#### 定义 1 {#top-i-s4-def-1 .statement tag=0B27}

*给定拓扑空间的族$(X_i)_{i \in I}$，该族的乘积空间是乘积集合$X = \prod_{i \in I} X_i$，拓扑是$X_i$拓扑的乘积（§ 2, no. 3， 例3）。 空间 $X_i (i \in I)$ 称为 X 的因子。*

根据命题 4 § 2, no. 3，$X$ 上的乘积拓扑以$\overline{\mathrm{pr}}_i^{-1}(U_i)$ 形式的集合的有限交集$\mathfrak{B}$ 作为基，其中$U_i$ 在$X_i$ 中开；这些集合是乘积 $\prod_{i \in I} A_i$，其中 $A_i$ 对于每个 $i \in I$ 和 $A_i = X_i$ 对于除了有限数量的索引之外的所有索引，在 $X_i$ 中是开放的。 这些集合将被称为基本集合。

如果$\mathfrak{B}_i$是$X_i$的拓扑的基（对于每个$i \in I$），很明显，对于每个指标$i$，初等集合$\prod_{i \in I} A_i$使得$A_i \in \mathfrak{B}_i$使得$A_i \neq X_i$ 形式另一个基共乘积拓扑。这个型的基本集合，其中包含给定点$x \in X$，因此形式是$x$的邻域的基本系统（$§ 1$，no. 3， 命题3)。

如果$I$是有限集合，则因子$X_i$拓扑中乘积拓扑的构造更简单：初等集合只是乘积$\prod_{i \in I} A_i$，其中$A_i$是任何开路$X_i$ 中的子集，每个 $i \in I$ (cf. 习题 9)。

#### 例 {#top-i-s4-n1-exa-1 .statement tag=0B28}

\* $n$ 空间乘积 $\mathbf{R}^n$ 与实直线 $\mathbf{R}$ 相同，称为 $n$ 维数实数空间； $\mathbf{R}^2$也称为实平面（cf.章VI, § 1）。同样，从有理线$\mathbf{Q}$开始，我们定义$n$维数$\mathbf{Q}^n$的有理数空间（$n = 2$的有理平面）。

空间 $\mathbf{R}^n$的拓扑在$\mathbf{R}$有$n$的所有乘积中的基集合打开区间，称为$n$维数的开箱。打开的盒子是包含点$x \in \mathbf{R}^n$形式这个邻域的基本系统这个点。同样，$n$的乘积在$\mathbf{R}$中封闭了区间，称为$n$维数的封闭盒子。 $x$ 内部的封闭盒子也是形式 $x$ 邻域的基本系统。 $\mathbf{Q}^n$ 也有类似的结果。 \*

#### 命题 1 {#top-i-s4-prop-1 .statement tag=0B29}

令$f = (f_i)$为拓扑空间$Y$到乘积空间$X = \prod_{i \in I} X_i$的映射。 那么$f$在点$a \in Y$连续当且仅当$f_i$对于每个$i \in I$在$a$连续。

从 $f_i = \mathrm{pr}_i \circ f$ 开始，这只是 § 2, no. 3 的命题 4 的特例。

#### 推论 1 {#top-i-s4-prop-1-cor-1 .statement tag=0B2A}

令$(X_i)_{i \in I}, (Y_i)_{i \in I}$为拓扑空间的两个族，且集合与指标相同。对于每个$i \in I$，令$f_i$为$X_i$到$Y_i$的映射。在阶中乘积映射 $f : (x_i) \to (f_i(x_i))$
$$
\prod_{i \in I} X_i \text{ into } \prod_{i \in I} Y_i
$$
应在点 $a = (a_i)$ 连续 对于每个 $i \in I$，$f_i$ 在 $a_i$ 连续是必要且充分的。

f 可以写成 $x \to (f_i(\mathrm{pr}_i(x)))$，因此命题 1 条件就足够了。相反，对于每个$x \in I$，令$g_x$为$X_x$到$\prod_{i \in I} X_i$的映射，使得每当$i \neq x$时，$\mathrm{pr}_x(g_x(x_x)) = x_x$和$\mathrm{pr}_i(g_x(x_x)) = a_i$；那么$g_x$在点$a_x$连续命题1。从$f_x = \mathrm{pr}_x \circ f \circ g_x$开始，如果$f$在$a$连续，那么$f_x$在$a_x$连续。

#### 推论 2 {#top-i-s4-prop-1-cor-2 .statement tag=0B2B}

*令$X, Y$为两个拓扑空间。在阶中，映射$f : X \to Y$应该是连续的，映射$g : x \to (x, f(x))$是$X$同胚到$f$的图$G$（视为子空间）是充分必要的乘积空间$X \times Y$）。*

由于$f = \mathrm{pr}_2 \circ g$，条件就足够了。这也是必要的，因为如果 $f$ 是连续的，则 $g$ 是双射且连续的 (命题 1)，并且 $g$ 的逆是 $\mathrm{pr}_1$ 到 $G$ 的限制，它是连续的 (cf. *集合) 理论*、章 IV, § 2, no. 4，标准 CST 17)。

#### 命题 2（拓扑乘积的结合性）{#top-i-s4-prop-2 .statement tag=0B2C}

*令$(X_i)_{i \in I}$为集合$I$的拓扑空间、$(J_x)_{x \in K}$划分族，对于每个$x \in K$令$X'_x = \prod_{i \in J_x} X_i$为空间的乘积 $X_i$ 换$i \in J_K$。然后典范映射乘积空间*
$$
\prod_{i \in I} X_i \text{ onto the product space } \prod_{x \in K} X'_x
$$
*是同胚。*

这是初始拓扑传递性的特例（$\S$ 2、no. 3、命题 5；cf. *集合理论*、章 IV, § 2, no. 4，标准 CST 13）。

一般地，我们通过典范映射*认同*乘积空间$\prod_{i \in I} X_i$和$\prod_{x \in K} X'_x$。

#### 推论 {#top-i-s4-n1-cor-1 .statement tag=0B2D}

*令$\sigma$为集合$I$中的置换。那么映射 $(x_i) \to (x_{\sigma(i)})$ 是*的同胚
$$
\prod_{i \in I} X_i \text{ onto } \prod_{i \in I} X_{\sigma(i)}.
$$

对命题 2 中的每个$i \in I$取$K = I$和$J_i = \{ \sigma(i) \}$。

#### 命题 3 {#top-i-s4-prop-3 .statement tag=0B2E}

*令$X$为集合，$(Y_i)_{i \in I}$为空间的拓扑族，对于每个$i \in I$，令$f_i$为$X$到$Y_i$的映射。令$f$为$X$到$Y = \prod_{i \in I} Y_i$的映射$x \to (f_i(x))$，并令$\mathfrak{T}$为$X$上最粗糙的拓扑，其中映射$f_i$是连续的。那么$\mathfrak{T}$是逆像在$f$下，拓扑在$f(X)$上由乘积拓扑在$Y$上诱导。*

这是初始拓扑的传递性另一个特例（\S\ 2、no. 3、命题 5；cf. 集合理论、章 IV、\S\ 2、no. 4，标准 CST 15）。

#### 推论 {#top-i-s4-n1-cor-2 .statement tag=0B2F}

*对于每个$i \in I$，令$A_i$为$Y_i$的子空间。那么乘积拓扑在$\prod_{i \in I} Y_i$上在$A = \prod_{i \in I} A_i$上诱导拓扑是子空间$A_i$拓扑的乘积。*

令 $j_i$ 为典范嵌入 $A_i \to Y_i$，应用命题 3 至映射 $f_i = j_i \circ \mathrm{pr}_i$ (cf. 集合理论, 章 IV, \S\ 2, no. 4，标准 CST 14）。

### 2. 开集合的截面；闭合集合的截面；开放的集合的投影。部分连续性

#### 命题 4 {#top-i-s4-prop-4 .statement tag=0B2G}

*设$X_1, X_2$为两个拓扑空间；那么对于每个$a_1 \in X_1$，映射$x_2 \to (a_1, x_2)$是$X_2$到$X_1 \times X_2$的子空间$\{a_1\} \times X_2$的同胚。*

这是推论 1 of 命题 1 of no. 1 应用于常数函数 $x_2 \to a_1$ 的特殊情况。

映射$x_2 \to (a_1, x_2)$相对于$X_1 \times X_2$中的等价关系$\mathrm{pr}_2 z = \mathrm{pr}_2 z'$来说是一个*连续段*（\S\3, no. 5）；因此，由该等价关系得出的商空间 $X_1 \times X_2$ 同胚于 $X_2$。

#### 推论 {#top-i-s4-n2-cor-1 .statement tag=0B2H}

* 乘积 $X_1 \times X_2$ 的截面 $A(x_1)$ 开（或闭）集合 $A$ 在任意点 $x_1 \in X_1 (*)$ 在 $X_2$ 开（或闭）。*

#### 命题 5 {#top-i-s4-prop-5 .statement tag=0B2I}

* 乘积 $X_1 \times X_2$ 的开集合 $U$ 的投影到任一因子上是开集合。*

例如，我们有$\mathrm{pr}_2 U = \bigcup_{x_1 \in X_1} U(x_1)$，命题从推论到命题4以及公理（O_1）。

#### 注 1 {#top-i-s4-n2-rem-1 .statement tag=0B2J}

*关闭* 的投影 $X_1 \times X_2$ 的子集到因子 *不需要关闭*。例如，在有理平面$\mathbf{Q}^2$中，方程为$x_1 x_2 = 1$的双曲线是闭的集合，但它的投影都等于$\mathbf{Q}$中点 0的补，这不是闭的集合。

(*) $x_1$ 处$A$的*截面* $A(x_1)$表示所有$x_2 \in X_2$中的集合，使得$(x_1, x_2) \in A$ (cf. 集合理论 R, \S\ 3, no. 7)。

#### 命题 6 {#top-i-s4-prop-6 .statement tag=0B2K}

设$X_1, X_2, Y$为乘积空间$X_1 \times X_2$到$Y$的三个拓扑空间、$f$映射。如果$f$在点$(a_1, a_2)$连续，则$X_2$到$Y$的部分映射$x_2 \to f(a_1, x_2)$在点$a_2$连续。

对于这个映射是$f$和映射$x_2 \to (a_1, x_2)$的合成；因此结果是从命题 4 得出的。

命题 6 通常用说来表示，两个变量的连续函数对于它们中的每一个来说都是连续的。

#### 注 2 {#top-i-s4-n2-rem-2 .statement tag=0B2L}

由映射 $f : X_1 \times X_2 \to Y$ 确定的所有部分映射可能是连续的，而不是 $f$ 在 $X_1 \times X_2$ 上连续（cf. 章 IX, § 5、习题 23）。 \* 例如，如果$f$是实平面$\mathbf{R}^2$到$\mathbf{R}$的映射，定义为
$$
f(x, y) = xy/(x^2 + y^2) \quad \text{if} \quad (x, y) \neq (0, 0)
$$
和$f(0, 0) = 0$，则所有部分映射都是连续的；但$f$在$(0, 0)$处不连续，因为如果$x \neq 0$则$f(x, x) = 1/2$。

如果$g$是$X_1$的映射到$Y$，在点$a_1$连续，那么$X_1 \times X_1 \to Y$的映射$(x_1, x_2) \to g(x_1)$完全连续点$(a_1, x_2)$，因为它是$g$和投影到$X_1$的合成。

这个小节的结果很容易扩展到拓扑空间的任意乘积$\prod_{i \in I} X_i$，通过指出对于任何划分$(J, K)$来说，这个乘积同胚于乘积$\left( \prod_{i \in J} X_i \right) \times \left( \prod_{i \in K} X_i \right)$ $I$（no. 1，命题2）。

### 3. 乘积关闭

#### 命题 7 {#top-i-s4-prop-7 .statement tag=0B2M}

在乘积空间$\prod_{i \in I} X_i$中，集合$\prod_{i \in I} A_i$的乘积的关闭与乘积$\prod_{i \in I} \overline{A}_i$的关闭相同。

假设$a = (a_i)$位于$\prod_{i \in I} A_i$的闭包内；那么对于每个$x \in I$，由于$\operatorname{pr}_x$（§ 2, no. 1，定理 1）的连续性，$a_x = \operatorname{pr}_x a$位于$A_x$的闭包中，因此$a \in \prod_{i \in I} \overline{A}_i$。相反，令$b = (b_i) \in \prod_{i \in I} \overline{A}_i$，并令$\prod_{i \in I} V_i$为任意初等集合包含$b$；对于每个 $i \in I$、$V_i$ 包含点 $x_i \in A_i$；因此$\prod_{i \in I} V_i$包含点$(x_i) \in \prod_{i \in I} A_i$，因此$b$位于$\prod_{i \in I} A_i$的闭包中。

#### 推论 {#top-i-s4-n3-cor-1 .statement tag=0B2N}

*乘积* $\prod_{i \in I} A_i$ *非空集合在乘积空间* $\prod_{i \in I} X_i$ *当且仅当* $A_i$ *在* $X_i$ *对于每个* $i \in I$ 时封闭。

如果 $I$ 是*有限*，则乘积 $\prod_{i \in I} A_i$ 开，前提是对于每个 $i \in I$，$A_i$ 在 $X_i$ 中开；但如果 $I$ 是无限的，情况就不再如此。

#### 命题 8 {#top-i-s4-prop-8 .statement tag=0B2O}

*令*$a = (a_i)$*为乘积空间*$X = \prod_{i \in I} X_i$中的任意点； *然后点* $x \in X$ *的集合* $D$ *这样* $\mathrm{pr}_i x = a_i$ *除了指标* $i$ *的有限数是稠密的* $X$。

对于每个$x \in X$和每个基本集合$V = \prod_{i \in I} U_i$其中包含$x$，我们有$U_i = X_i$，除了指标$i$属于到有限子集$J$ $I$；如果我们用$y_i = x_i$代表$i \in J$，用$y_i = a_i$代表$i \notin J$，很明显
$$
y = (y_i) \in D \quad \text{and} \quad y \in V;
$$
因此结果。

### 4. 拓扑逆极限空间

令$I$为偏序（但不一定有向）集合(*)，其中序关系写为$\alpha \leq \beta$。对于每个$\alpha \in I$，令$X_\alpha$为拓扑空间，对于每个对$(\alpha, \beta)$，使得$\alpha \leq \beta$令$f_{\alpha \beta}$为$X_\beta$到$X_\alpha$的映射。我们说$(X_\alpha, f_{\alpha \beta})$是拓扑空间*的*逆系，如果： 1) $(X_\alpha, f_{\alpha \beta})$是集合*的*逆系； 2) 每当 $\alpha \leq \beta$ 时，$f_{\alpha \beta}$ 都是*连续* 映射。令$X$表示集合$\varprojlim X_\alpha$，对于每个$\alpha \in I$，令$f_\alpha$为典范映射$X \to X_\alpha$；那么$X$上的*粗略*拓扑（其中$f_\alpha$是连续的）被认为是$X_\alpha$拓扑的*逆极限*（相对于$f_{\alpha \beta}$），并且集合$X$与此拓扑称为拓扑空间*$(X_\alpha, f_{\alpha \beta})$的逆系*逆极限。每当我们将$\varprojlim X_\alpha$称为拓扑空间时，总是可以理解，这个空间的拓扑是$X_\alpha$拓扑的逆极限，除非明确指出相反。

集合 $X$ 是点 $x$ 中乘积 $\prod_{\alpha \in I} X_\alpha$ 由……组成的子集，使得
$$(1)$$
$$
\mathrm{pr}_\alpha(x) = f_{\alpha \beta}(\mathrm{pr}_\beta(x))
$$
每当$\alpha \leq \beta$时。 从no. 1的命题3得出，$X_\alpha$拓扑的逆极限与乘积空间$\prod_{\alpha \in I} X_\alpha$的拓扑在$X$上“诱导”的拓扑相同。 如果对于每个 $\alpha \in I$，$Y_\alpha$ 是

(*) 即，集合赋予自反和及物关系 (*集合理论* R, § 6, no. 1)。

$X_\alpha$的子空间使得$Y_\alpha$形式和$X_\alpha$的子集*的*逆系 (*集合理论* 章III, , n° 2)，则显然拓扑空间 $\varprojlim Y_\alpha$ 是 $\varprojlim X_\alpha$ 的 *子空间*

令$(X'_\alpha, f'_{\alpha\beta})$为拓扑空间的另一个逆系，由相同的集合$I$索引，并且对于每个$\alpha \in I$令$u_\alpha : X_\alpha \to X'_\alpha$为*连续*映射，使得$(u_\alpha)$为*逆系共映射*；那么$u = \varprojlim u_\alpha$是$X = \varprojlim X_\alpha$到$X' = \varprojlim X'_\alpha$的连续映射。因为如果$f'_\alpha$是典范映射$X' \to X'_\alpha$，我们有$f'_\alpha \circ u = u_\alpha \circ f_\alpha$，因此$f'_\alpha \circ u$对于每个$\alpha \in I$都是连续的，并且断言从§ 2, no. 3的命题4开始。

最后，假设$I$是一个*有向*集合，并令$J$是$I$的*共最终*子集；设$Z$为拓扑空间$(X_\alpha, f_{\alpha\beta})_{\alpha \in J, \beta \in J}$逆系逆极限。那么规范的双射 $g : X \to Z$ (*集合理论*, 章 III, § 7, no. 2, 命题 3) 是一个*同胚*。因为每个 $\lambda \in J$ 都有 $\mathrm{pr}_\lambda(g(x)) = \mathrm{pr}_\lambda(x)$；因此 $g$ 是连续的 (no. 1, 命题 1)；如果$h$是$g$的逆，那么对于每个$\alpha \in I$，存在$\lambda \in J$使得$\alpha \leq \lambda$，因此存在$\mathrm{pr}_\alpha(h(z)) = f_{\alpha\lambda}(\mathrm{pr}_\lambda(z))$，这表明$h$是连续的（no. 1，命题1），因为$f_{\alpha\lambda}$ 是连续的。

#### 命题 9 {#top-i-s4-prop-9 .statement tag=0B2P}

*令$I$为有向集合，并且$J$是$I$的并列子集。令$(X_\alpha, f_{\alpha\beta})$为由$I$索引的拓扑空间的逆系；设 $X = \varprojlim X_\alpha$ 并设 $f_\alpha : X \to X_\alpha$ 为典范映射。那么集合$f^{-1}_\alpha(U_\alpha)$的族，其中$\alpha$贯穿$J$，$U_\alpha$贯穿$X_\alpha$的拓扑的基$\mathfrak{B}_\alpha$，对于每个$\alpha \in J$，是基拓扑共 $X$。*

从§ 2, no. 3我们知道形式$f^{-1}_\alpha(U_\alpha)$集合*有限交*（$\alpha \in I, U_\alpha$在$X_\alpha$开）$X$拓扑形式基。如果$(\alpha_i)_{1 \leq i \leq n}$是$I$的指标的有限族，则存在$\gamma \in J$使得$\alpha_i \leq \gamma$对于$1 \leq i \leq n$；因此$f_{\alpha_i} = f_{\alpha_i\gamma} \circ f_\gamma$；如果我们把

$$
V_\gamma = \bigcap_i f^{-1}_{\alpha_i\gamma}(U_{\alpha_i}),
$$

那么我们有

$$
f^{-1}_\gamma(V_\gamma) = \bigcap_i f^{-1}_{\alpha_i}(U_{\alpha_i});
$$

但$V_\gamma$是开放的，因此是集合属于到$\mathfrak{B}_\gamma$的并。于是就有了这样的结果。

#### 推论 {#top-i-s4-n4-cor-1 .statement tag=0B2Q}

*令$A$为$X$的子集，并让$A_\alpha$代表每个$\alpha \in I$的$f_\alpha(A)$。然后：*

(i) *$A_\alpha$（分别为$\overline{A}_\alpha$）形成$X_\alpha$子集的逆系统，并且*

$$
\overline{A} = \bigcap_\alpha f^{-1}_\alpha(\overline{A}_\alpha) = \varprojlim \overline{A}_\alpha.
$$

(ii) *如果 $A$ 在 $X$、$A = \varprojlim A_\alpha = \varprojlim \overline{A}_\alpha$ 内关闭。*

(i) 的第一个断言由 $\alpha \leq \beta$ 的关系 $f_\alpha = f_{\alpha\beta} \circ f_\beta$ 以及$f_{\alpha\beta}$ (§ 2, no. 1, 定理 1) 的连续性得出。让 $A'$ 表示
$$
\bigcap_\alpha \overline{f}_\alpha(\overline{A}_\alpha);
$$
那么显然$A'$是闭集，包含$A$，所以$\overline{A} \subset A'$。相反，令$x \in A'$；我们必须证明$x$位于$A$的闭包中。凭借命题 9，足以证明$x$的每个邻域，其中形式$\overline{f}_\alpha(U_\alpha)$，其中$\alpha \in I$和$U_\alpha$在$X_\alpha$开，满足$A$。现在，到假设，$f_\alpha(x) \in U_\alpha$，从$f_\alpha(x) \in \overline{A}$开始，我们有了$U_\alpha \cap A_\alpha \neq \varnothing$，这意味着$A \cap \overline{f}_\alpha(U_\alpha)$不为空。

为了建立 (ii)，只需指出，在 $A$ 上没有任何限制，我们就有 $A \subset \lim A_\alpha \subset \lim \overline{A}_\alpha$；现在如果 $A$ 是闭合的，那么从 (i)
$$
A = \lim \overline{A}_\alpha
$$
(ii)如下。

#### 例 {#top-i-s4-n4-exa-1 .statement tag=0B2R}

令$I$为有向集合且$(X_\alpha)_{\alpha \in I}$为子集与集合$Y$的族，使得每当$\alpha \leq \beta$时$X_\alpha \supset X_\beta$。对于每个$\alpha \in I$，令$\mathfrak{T}_\alpha$为$X_\alpha$上的拓扑，使得每当$\alpha \leq \beta$时，$\mathfrak{T}_\beta$比更细大于拓扑，由$\mathfrak{T}_\alpha$在$X_\beta$上感应。如果我们将$\alpha \leq \beta$的$f_{\alpha\beta}$视为典范嵌入$X_\beta \to X_\alpha$，那么$\lim X_\alpha$可以用$X_\alpha$的*交*$X$规范地识别，而拓扑是*最小的$\mathfrak{T}_\alpha$ 在 $X$ 上引发的拓扑的上界* (§ 2, no. 3, 例 2)。

### 习题 {#top-i-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
