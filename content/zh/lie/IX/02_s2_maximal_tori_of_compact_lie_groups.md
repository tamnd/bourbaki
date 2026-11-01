---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Maximal tori of compact Lie groups
lang: zh
source: lie-vii-ix
book_pages: 287-295, 391-394
pdf_pages: 0294-0302, 0398-0401
extraction: native+ocr
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS OF COMPACT ALGEBRAS
      page: 287
      pdf_page: 294
    - "no": 2
      title: MAXIMAL TORI
      page: 288
      pdf_page: 295
    - "no": 3
      title: MAXIMAL TORI OF SUBGROUPS AND QUOTIENT GROUPS
      page: 291
      pdf_page: 298
    - "no": 4
      title: SUBGROUPS OF MAXIMAL RANK
      page: 292
      pdf_page: 299
    - "no": 5
      title: WEYL GROUP
      page: 293
      pdf_page: 300
    - "no": 6
      title: MAXIMAL TORI AND COVERING OF HOMOMORPHISMS
      page: 295
      pdf_page: 302
statements: 32
exercises: 11
content_sha256: b7a156fdf5905e06c93c7efc93bc4afdc105033f7066698ca59f5ba76f5c785a
translated_from: content/en/lie/IX/02_s2_maximal_tori_of_compact_lie_groups.md
translation_method: google
source_content_sha256: 09376883a430ceee6e2f9d7416163648064cb06680a75c0f4d800750884c66c2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 49964c0e6a5b1f3fb2fbcbef5dda640157216c3e0d7cdc27f5ffaad9499a7b7e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。最大环面紧李群

### 1. 嘉当子代数的紧代数

#### 引理 1 {#lie-ix-s2-lem-1 .statement tag=019Z}

令 G 为李群，K 为 G 的紧致子群，且 F 不变双线性形式在 L(G) 上。让$x, y\in L(G)$。存在 K 的元素 $k$，使得对于所有 $u\in L(K)$ 都有 $F(u$，[(Ad $k$)$(x), y]) = 0$。

从 K 到 $\mathbf{R}$ 的函数 $v \rightarrow$ F((Ad $v$)$(x), y$) 是连续的，因此在点 $k\in K$ 处有最小值。令 $u\in L(K)$ 并放入

$h(t) =$ F((广告费用($tu$)$.k$)$(x), y$)$,t\in \mathbf{R}$。

我们为所有 $t$ 准备了 $h(t)\geq h(0)$；此外，由章。 III, §3, no. 12，第 44 号提案，

$\frac{dh}{dt}(0) = F([u$,(广告$k$)$(x)], y) = F(u$,[(广告$k$)$(x), y])$,

因此引理（实变量的函数，第I, §1, no. 7章，第7条命题）。

#### 定理 1 {#lie-ix-s2-thm-1 .statement tag=01A0}

设$\mathfrak{g}$为紧李代数。 $\mathfrak{g}$（第VII, §2, no. 1，定义1）中的嘉当子代数是其最大交换子代数；特别是，$\mathfrak{g}$是其嘉当子代数的并。 群 Int($\mathfrak{g}$) 在 $\mathfrak{g}$ 的嘉当子代数的集合上进行传递运算。

由于 $\mathfrak{g}$ 是还原性的，因此它的嘉当子代数是可交换的（第 VII, §2, no. 4 章，第 2 章第 3 章）。相反，令 $\mathfrak{t}$ 为 $\mathfrak{g}$ 中的交换子代数。根据 §1, no. 3，第 1 号提案，广告 $x$ 对于所有 $x\in \mathfrak{t}$ 来说是半单；由章。 VII, §2, no. 3，命题10，存在$\mathfrak{g}$包含$\mathfrak{t}$中的嘉当子代数。这就证明了定理的第一个断言。

现在让$\mathfrak{t}$和$\mathfrak{t}'$是$\mathfrak{g}$的两个嘉当子代数。我们证明存在$u\in$ Int($\mathfrak{g}$)使得$u(\mathfrak{t}) =\mathfrak{t}'$。根据§1, no. 3的命题1，我们可以假设$\mathfrak{g}$是形式L(G)，其中G是连通的紧李群，并且可以选择是$\mathfrak{g}$上的分离不变对称双线性形式F。令$x$（或$x'$）为$\mathfrak{g}$的正则元素，使得$\mathfrak{t}=\mathfrak{g}^0(x)$（或$\mathfrak{t}'=\mathfrak{g}^0(x')$）（第VII, §3, no. 3，第2章）。 应用引理 1，其中 K = G，我们看到存在 $k\in G$，使得 [(Ad $k$)$(x), x']$ 与 $\mathfrak{g}$ 关于 F 正交，因此是零；那么 (Ad $k$)$(x)\in \mathfrak{g}^0(x') =\mathfrak{t}'$，所以 $\mathfrak{g}^0$((Ad $k$)$(x)$) $=\mathfrak{t}'$，因为 (Ad $k$)$(x)$ 是常规的。我们结论（广告$k$）$(\mathfrak{t}) =\mathfrak{t}'$，因此定理。

#### 推论{#lie-ix-s2-n1-cor-1 .statement tag=01A1}

令$\mathfrak{t}$和$\mathfrak{t}'$为$\mathfrak{t}$的$\mathfrak{g},\mathfrak{a}$子集的嘉当子代数，以及将$\mathfrak{a}$带入$\mathfrak{t}'$的$\mathfrak{g}$的$u$自同构。 Int($\mathfrak{g}$) 存在元素$v$，使得$u\circ v$将$\mathfrak{t}$带到$\mathfrak{t}'$，并且重合与$u$在$\mathfrak{a}$上。

设G = Int($\mathfrak{g}$)，并考虑G中$\mathfrak{a}$的固定器$Z_G(\mathfrak{a})$；这是G的谎言子群，其李代数$\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$由$\mathfrak{g}$的元素组成，与$\mathfrak{a}$的每个元素可交换（第III, §9, no. 3，第7章）。那么$\mathfrak{t}$和$u^{-1}(\mathfrak{t}')$就是紧李代数$\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$中的两个嘉当子代数。由 Th. 1、存在$Z_G(\mathfrak{a})$的元素$v$使得$v(\mathfrak{t}) =u^{-1}(\mathfrak{t}')$；任何这样的元素都具有所需的属性。

### 2. 最大托里

令 G 为李群。 G 的环面是闭子群，即环面 (§1, no. 2)，在其他字中任何可交换连通紧致子群。 G的环面的集合中的极大元素，按包含排序，称为G的最大环面。

#### 定理 2 {#lie-ix-s2-thm-2 .statement tag=01A2}

令 G 为连通的紧李群。

a) G 的最大环面的李代数是L(G)的嘉当子代数。

b) 设$T_1$和$T_2$为G的两个最大环面。存在$g\in G$使得$T_2=gT_1g^{-1}$。

c) G 是其最大环面的并。

设$\mathfrak{t}$为L(G)中的嘉当子代数； 李代数为 $\mathfrak{t}$ 的 G 的积分子群是闭集（第 VII, §2, no. 1 章，命题 4 的 Cor. 4）且可交换（Th.1），因此是 G 的环面。如果 T 是 G 的极大值环面，则其李代数是可交换，因此包含在 L(G) (Th. 1) 的嘉当子代数中。由此可见，G 的最大环面恰好是与 L(G) 的嘉当子代数相关的 G 的积分子群，因此 a)。 断言 b) 由 Th 推出。 1，因为典范同态 $G\rightarrow$ Int(L(G)) 是满射的（第 10 条第 III, §6, no. 4 章，Cor. 4）。

用G的最大环面X并表示，并令T为G的最大环面。从$G\times T$到G的连续映射$(g, t) \rightarrow gtg^{-1}$有像X，因此在G中是封闭的；因此，要证明c)，只需证明X在G中是开集即可；由于X在内自同构下是不变的，因此足以证明，对于所有$a\in T, X$来说，邻域等于$a$。我们通过归纳对G的维数进行论证，并区分两种情况：

$1)a$ 在 G 中不是中心。设 H 为 G 中$a$ 的中心子的恒等分量；这是 G 的连通紧致子群，与 G 不同，包含于 T，因此$a$。由于 Ad $a$ 是半单 (§1, no. 1)，因此 H 的李代数就是 Ad $a-1$ 的零空间；现在是从第 1 章开始的。 VII, §4, no. 2，命题4，H 的共轭的并 Y 是$a$ 的邻域。 归纳假设、$H\subset X$，因此$Y\subset X$；因此，X 是 $a$ 的邻域。

$2)a$是G中的中心。对于L(G)中的所有$x$，只需证明$a$exp$x$属于到X即可。现在，G 的L(G) 属于至嘉当子代数的每元素 $x$（第 1 期）； 相应的积分子群$T'$包含指数$x$；因为它是共轭到 T，所以它是包含 $a$，因此 $a$ exp $x$，根据需要。

#### 推论 1 {#lie-ix-s2-thm-2-cor-1 .statement tag=01A3}

a) G 的指数映射是满射的。

b) 对于所有 $n\geq 1$，从 G 到自身的映射 $g \rightarrow g^n$ 是满射。

事实上，exp(L(G)) 包含于 G 的所有最大环面，因此 a)。 断言 b) 从公式 (exp $x$)$^n=$ exp $nx$ 得出L(G) 中的 $x$。

#### 注 1 {#lie-ix-s2-n2-rem-1 .statement tag=01A4}

存在 L(G) 的紧子集 K，使得 exp$_G(K) = G$。事实上，如果 T 是 G 的最大环面，则存在紧致子集 $C\subset L(T)$，使得 exp$_T(C) = T$；取$K =\bigcup_{g\in G}$（广告$g$）$(C)$就足够了。

#### 推论 2 {#lie-ix-s2-thm-2-cor-2 .statement tag=01A5}

G 的最大环面交是 G 的中心。

设$x$为G的中心元素；通过 Th。 $2c)$，G 包含于 $x$ 存在最大环面 T；那么$x$属于到T的所有共轭，因此到G的所有最大环面。相反，如果$x$属于到G的所有最大环面，它与G的每个元素交换Th。 $2c)$。

#### 推论 3 {#lie-ix-s2-thm-2-cor-3 .statement tag=01A6}

令$g\in G$，并令C为其扶正器。然后$g$属于到$C_0$； 群 $C_0$ 是 G 包含于 $g$ 的最大环面的并。

G 包含于 $g$ (Th. $2c$)$)$ 存在最大环面 T，因此包含在 $C_0$ 中。此外，群$C_0$是一个连通的紧李群，因此其最大环面的并 (Th. $2c$)$)$；这些都是包含$g$（Cor.2），因此正是G包含$g$的最大环面。

#### 推论 4 {#lie-ix-s2-thm-2-cor-4 .statement tag=01A7}

让$g\in G$。如果 $g$ 是正则的（第 VII, §4, no. 2，定义 2），则它属于为唯一的最大值环面，这是其集中器的恒等分量。否则，它属于到无限多个最大环面。

由于 Ad $g$ 是半单，因此 Ad $g-1$ 的零空间的维数也是 $g$ 的中心化器 C 的零空间。按地点。引文、第 8 号提案和 Th。 $1,g$ 是正则的当且仅当 $C_0$ 是 G 的最大环面。现在的结论来自 Cor. 3.

#### 推论 5 {#lie-ix-s2-thm-2-cor-5 .statement tag=01A8}

a) 令S为G的环面。S的扶正器是连通的；它是 G 包含 S 的最大环面的并。

b) 设$\mathfrak{s}$为L(G)的交换子代数。 G中$\mathfrak{s}$的固定器已连接；它是 G 的最大环面的并，其中李代数包含 $\mathfrak{s}$。

为了证明a)，只要证明如果G的元素$g$集中S，则存在G包含S和$g$的最大环面。现在，如果C是$g$的中心化子，我们就有$g\in C_0$（Cor.3）和$S\subset C_0$；如果 T 是连接的紧李群 $C_0$ 包含 S 的最大环面，则我们有 $g\in T$（Cor. 2），因此 a)。 断言 b) 由适用于子群与李代数 $\mathfrak{s}$ 的积分的 a) 得出，鉴于第 1 章。 III, §9, no. 3，提案 9。

#### 注 2 {#lie-ix-s2-n2-rem-2 .statement tag=01A9}

这是从 Cor 得出的。 5 G 的最大环面是最大交换律子群。 逆命题不成立：对于例，在群 $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ 中，最大环面为维数 1，因此对角线矩阵的不能包含子群，与 $(\mathbf{Z}/2\mathbf{Z})^2$ 同构的。此外，如果$g\in \mathbf{S}\mathbf{O}(3,\mathbf{R})$是非标量对角矩阵，则$g$是未连接扶正器的$\mathbf{S}\mathbf{O}(3,\mathbf{R})$的正则元素（cf.Cor.4）。

#### 推论 6 {#lie-ix-s2-thm-2-cor-6 .statement tag=01AA}

G 的最大环面是它们自己的中心化器，并且是它们的李代数的固定器。

令 T 为 G 的最大值环面和其扶正器 C；由于L(T) 是L(G) 的嘉当子代数，我们有L(T) = L(C)，因此C = T，因为C 是连通的（Cor. 5）。

#### 推论 7 {#lie-ix-s2-thm-2-cor-7 .statement tag=01AB}

设T和$T'$是G的两个最大环面，T的A子集和G的$s$自同构，将A带入$T'$。存在 $g\in G$ 使得 $s\circ$ (Int $g$) 将 T 带到 $T'$ 和重合，并在 A 上使用 $s$。

设C为A的中心化子，则T和$s^{-1}(T')$为$C_0$的两个最大环面； $C_0$ 的每个元素 $g$ 使得 (Int $g$)$(T) =s^{-1}(T')$ 具有所需的属性。

#### 推论 8 {#lie-ix-s2-thm-2-cor-8 .statement tag=01AC}

设H为紧李群，T为H的最大环面。然后将$N_H(T)$的$H = N_H(T).H_0$和单射转化为H诱导同构，从$N_H(T)/N_{H_0}(T)$到$H/H_0$。

让$h\in H$。那么$h^{-1}Th$是$H_0$的最大值环面，因此(Th.2)存在$g\in H_0$使得$hg\in N_H(T)$；因此$h$属于到$N_H(T).H_0$，因此第一个断言。第二个紧随其后。

#### 注 3 {#lie-ix-s2-n2-rem-3 .statement tag=01AD}

令 G 为连通的李群，其李代数是紧致的。 G 的嘉当子群是积分子群，其李代数是 L(G) 的嘉当子代数（连通紧凑群的嘉当子群因此是其最大环面）。 定理 2 及其推论对于 G 仍然有效，如果我们替换处处都是“Cartan 子群”的表达式“最大环面”。根据§1, no. 4的命题5，G是向量群V的直接乘积和连通紧凑群K，并且G的嘉当子群是V的乘积，其中K 的最大环面。此外，它从 Cor 得出注。由上式6可知，G的嘉当子群也可以定义为L(G)的嘉当子代数的固定剂。

定理2的$^*4)$部分c)也可以用以下方式证明。给 G 一个不变的黎曼度量（§1, no. 3，命题 3）。那么，对于G的任意元素$g$，都存在G的最大测地线经过到$g$和单位元素（Hopf-Rinow定理），并且可以验证这样的测地线的闭包是$G$的子圆环。\*

### 3. 子群和商群的最大环面

#### 命题 1 {#lie-ix-s2-prop-1 .statement tag=01AE}

设 G 和 $G'$ 是两个相连的紧李群。

a) 令$f: G\rightarrow G'$为李群的满射态射。 $G'$ 的最大环面是 G 的最大环面的 $f$ 之下的像。如果 $f$ 的核是 G 的中心（对于例离散），则 G 的最大环面是 G 的最大环面的 $f$ 之下的逆像 $G'$。

b) 令 H 为 G 的连通闭子群。H 的每个最大值环面为交，其中 H 为 G 的最大值环面。

c) 令 H 为 G 的连通闭法线子群。H 的最大环面为交，其中 H 为 G 的最大环面。

a) 令 T 为 G 的最大值环面；那么 L(T) 是 L(G) 的嘉当子代数 (no. 2, Th. $2a$)$)$，所以 $L(f(T))$ 是 $L(G')$ 的嘉当子代数（第 VII, §2, no. 1 章，第 2 条） 4);由此可见，$f(T)$ 是 $G'$ (no. 2，Th. $2a$)$)$ 的最大环面。如果 Ker $f$ 是 G 的中心，则它包含在 T（Th.2 的 Cor.2）中，因此$T =f^{-1}(f(T))$。

相反，令$T'$为$G'$的最大值环面；我们证明存在 G 的最大环面 T，使得 $f(T) = T'$。令$T_1$为G的最大环面；那么$f(T_1)$是$G'$的最大环面，并且存在$g'\in G'$使得$T'=g'f(T_1)g^{'-1}$(Th.$2b$)$)$；如果$g\in G$使得$f(g) =g'$，我们有$T'=f(T)$和$T =gT_1g^{-1}$。

b) 令 S 为 H 的最大值环面；这是 G 的环面，因此存在 G 包含 S 的最大环面 T。那么 $T\cap H$ 是 H 包含 S 的交换性子群，因此等于 S (no. 2, 注 2)。

c) 根据§1, no. 3，命题$2c), L(G)$是带有理想的L(H)的直乘积；因此，L(H)的嘉当子代数是交，其中L(H)是L(G)的嘉当子代数。因此，对于 $G, T\cap H$ 包含的任何最大环面 T，H 和 $S = T\cap H$ (no. 2，注 2) 的最大环面 S。

#### 注 1 {#lie-ix-s2-n3-rem-1 .statement tag=01AF}

命题 1 立即概括为与紧李代数连接的群。特别是，如果 G 是一个连通的李群，且李代数是紧的，则 G 的嘉当子群 (cf. 注 3, no. 2) 恰好是连通的紧李群 Ad(G) 的最大环面的逆像（在典范同态下，从 G 到广告（G））。

#### 注 2 {#lie-ix-s2-n3-rem-2 .statement tag=01AG}

设 G 是连通的紧李群，$\widetilde{D}(G)$ 群 D(G) 和 $f: \widetilde{D}(G)\rightarrow G$ 从 $\widetilde{D}(G)$ 到 D(G) 以及从 D(G) 到 G 的规范态射的组合。那么映射 $T\rightarrow f^{-1}(T)$ 是双射 G 最大环面的集合到 $\widetilde{D}(G)$ 最大环面的集合； 逆双射与 $\widetilde{D}(G)$ 的最大值环面 $\widetilde{T}$ 和 G 的最大值环面 $C(G)_0.f( \widetilde{T})$ 相关联。

### 4. 最大秩的子群

我们将称其李代数的连接的李群 G 秩为秩，并用 rk G 表示。 2 a)，连接的紧李群的秩是其最大环面的公共的维数。

设 G 是 G 的连通紧李群，H 是 G 的闭子群。如果 H 是连通的，则 rk $H\leq$ rk G （因为 H 的最大环面是 G 中的环面）。由 Th. 2 c) ，说 H 是连通的并且最大秩 （即秩 rk G）意味着 H 是 G 的最大环面的并。我们立即从命题 1 推出：

#### 命题 2 {#lie-ix-s2-prop-2 .statement tag=01AH}

令 $f$ : G $\rightarrow G'$ 为连通紧李群的满射态射，其中核为中心。 映射$H \rightarrow f(H)$和$H' \rightarrow f^{-1}(H')$是最大秩的G连接闭合子群的集合和$G'$的类似集合之间的逆双射。

#### 命题 3 {#lie-ix-s2-prop-3 .statement tag=01AI}

设 G 为连通的紧李群，H 为最大秩的连通的闭子群。

a) 紧流形 $G/H$ 是单连通的。

b) 同态 $\pi_1(H)\rightarrow \pi_1(G)$，由 H 的典范嵌入归纳为 G，是满射。

由于 H 是连通的，所以我们有正合序列（一般拓扑，第 XI 章，正在准备中）

$$
\pi_1(H)\rightarrow \pi_1(G)\rightarrow \pi_1(G/H,\overline{e})\rightarrow 0
$$

其中$\overline{e}$是G的单位元素的$G/H$中的像。由于$G/H$是连通的，这立即意味着断言a)和b)的等价。此外，如果$f: G'\rightarrow G$是连通的紧李群的满射态射，其中核是中心，则G的证明命题（在形式$a$中）$)$与G的证明相同$G'$（提案 2）。因此，我们可以首先通过 Ad(G) 得到替换 G，然后假设 G 是半单，然后通过通用覆盖 (§1, no. 4，Cor. 2) 得到替换 G，假设 G 是单连通的。但断言 b) 就微不足道了。

#### 命题 4 {#lie-ix-s2-prop-4 .statement tag=01AJ}

设G为紧李群，H是G的最大秩的连通闭子群，N是G中H的归一化器。则H是N中的有限指标，并且是N的单位分量。

事实上，H 包含嘉当子代数 L(G) 的李代数。因此，由章。 VII, §2, no. 1，科。命题 4 的 4 中，H 是 N 的恒等分量。由于 N 是紧的，因此 H 在 N 中具有有限指标。

#### 注 1 {#lie-ix-s2-n4-rem-1 .statement tag=01AK}

G 的每个积分子群 H 使得 rk H = rk G 都是闭的：事实上，前面的证明表明 H 是其归一化器的恒等分量，它是 G 的闭子群。

#### 注 2 {#lie-ix-s2-n4-rem-2 .statement tag=01AL}

对于命题 4 的记号，G 包含于 H 的每个闭子群 $H'$ 且$(H': H)$ 是有限的，对 H 进行归一化，因此包含在 N 中；类似地，$H'$的归一化项包含在N中。特别地，N是它自己的归一化项。

### 5.韦尔群

令 G 为连通的紧李群，T 为 G 的最大值环面。用 $N_G(T)$ 表示 G 中 T 的归一化器；根据命题 4 (no. 4)，商群 $N_G(T)/T$ 是有限的。我们用 $W_G$(T) 或 W(T) 表示它，并称其为 G 的最大环面 T 的 Weyl 群，或 G 相对于 T 的 Weyl 群。由于 T 是可交换的，因此 T 上 $N_G(T)$ 的运算乘以 G 的内自同构诱导通过李群 T 上群 $W_G(T)$ 的商运算，称为规范运算。 6 Th. no. 2 的 2 个，这个运算是忠实的：关联的同态 $W_G(T)\rightarrow$ Aut T 是单射的。

如果 $T'$ 是 G 的另一个最大环面，并且如果 $g\in G$ 使得 Int $g$ 映射 T 到 $T'$ (no. 2, Th. $2b$)$)$，则 Int $g$诱导同构$a_g$从$W_G(T)$到$W_G(T')$和$a_g(s)(gtg^{-1}) =gs(t)g^{-1}$适用于所有$s\in W_G(T)$和所有$t\in T$。

#### 命题 5 {#lie-ix-s2-prop-5 .statement tag=01J9}

G 的每$a)$ 共轭类都会遇到 T。

b) 交，G 的共轭类 T 是 Weyl 群的轨道。

设 $g\in G$；通过 Th。 no. 2中的2，存在$h\in G$使得$g\in hTh^{-1}$，因此a)。根据Weyl 群的定义，T上$W_G(T)$的同一个轨道中的任意两个元素在G中都是共轭；反之，令$a, b$为G下T共轭的两个元素。存在$h\in G$使得$b=hah^{-1}$； 应用科。 7 Th。 2 (no. 2) 与 $A =\{a\},s=$ Int $h, T'= T$，我们看到存在 $g\in G$，使得 Int $hg$ 映射 T 到 T 以及 $a$ 到 $b$。 $W_G(T)$中的$hg$的类，然后映射$a$到$b$，因此命题。

#### 推论 1 {#lie-ix-s2-prop-5-cor-1 .statement tag=01JA}

将 T 的典范嵌入转化为 G 定义，通过求 G 的共轭类的从 $T/W_G(T)$ 到空间 $G/$Int(G) 的同胚。

事实上，这是两个紧凑空间之间的双射连续映射（cf. General 拓扑，第 III，p. 29，Cor. 1）。

#### 推论 2 {#lie-ix-s2-prop-5-cor-2 .statement tag=01JB}

设 E 为 G 在内自同构下稳定的子集。那么 E 在 G 中是开（或闭、或密）当且仅当 $E\cap T$ 在 T 中是开（或闭、或密）。

这是从 Cor 得出的。 1 以及规范的映射 $\mathrm{T}\to \mathrm{T}/\mathrm{W}_{G}(\mathrm{T})$ 和 $\mathrm{G}\to \mathrm{G}/\mathrm{Int}(\mathrm{G})$ 已开放的事实（*常规拓扑*，第 III、p. 10、引理 2）。

将$\mathrm{G}$的李代数表示为$\mathfrak{g}$，将$\mathrm{T}$的$\mathfrak{t}$表示。 $\mathrm{T}$ 诱导表示上$\mathrm{W}_{G}(\mathrm{T})$的运算，称为$\mathbf{R}$向量空间$\mathfrak{t}$上群$\mathrm{W}_{G}(\mathrm{T})$的*规范表示*。

#### 命题 6 {#lie-ix-s2-prop-6 .statement tag=01JC}

a) *$\mathfrak{g}$上$\mathrm{G}$的每个轨道（对于伴随表示）满足$\mathfrak{t}$。*

b) *交和$\mathrm{G}$轨道$\mathfrak{t}$是$\mathfrak{t}$上$\mathrm{W}_{G}(\mathrm{T})$轨道。*

断言 a) 由 Th 得出。 1（no. 1）。令$x,y$为$\mathrm{Ad}(\mathrm{G})$下$\mathfrak{t}$共轭的两个元素，并令$h\in\mathrm{G}$为$(\mathrm{Ad}\,h)(x)=y$。 应用 Th 的推论。 1（no. 1）与$\mathfrak{a}=\{x\}$，$u=\mathrm{Ad}\,h$，$\mathfrak{t}'=\mathfrak{t}$，我们看到存在$g\in\mathrm{G}$使得$\mathrm{Ad}\,hg$映射$\mathfrak{t}$到$\mathfrak{t}$和$x$到$y$。然后$hg\in\mathrm{N}_{G}(\mathrm{T})$（第III, §9, no. 4章，第11条命题），以及$\mathrm{W}_{G}(\mathrm{T})$映射$x$到$y$中$hg$的类，因此命题。

#### 推论 {#lie-ix-s2-n5-cor-1 .statement tag=01JD}

*通过从$\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T})$到$\mathfrak{g}/\mathrm{Ad}(\mathrm{G})$商同态，将$\mathfrak{t}$的典范嵌入转化为$\mathfrak{g}$定义。*

将这个映射表示为$j$；它是双射且连续的（命题 6）。我们有一个可交换的图表

$$
\begin{array}{ccc}
\mathfrak{t} & \xrightarrow{\ i\ } & \mathfrak{g} \\
{\scriptstyle p}\downarrow\phantom{{\scriptstyle p}} & & \phantom{{\scriptstyle q}}\downarrow{\scriptstyle q} \\
\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T}) & \xrightarrow{\ j\ } & \mathfrak{g}/\mathrm{Ad}(\mathrm{G})
\end{array}
$$

其中$p$和$q$是映射的商，$i$是典范嵌入。由于 $i$ 和 $q$ 是正确的（*一般拓扑*，第 I, §10, no. 1 章，命题 2 和 *一般拓扑*，第 III, §4, no. 1，命题 2 c)），并且由于 $p$ 是满射的，因此得出$j$ 是正确的（*一般拓扑*，第 I, §10, no. 1 章，命题 5），因此是同胚。

#### 命题 7 {#lie-ix-s2-prop-7 .statement tag=01JE}

*令$H$为$\mathrm{G}$包含$\mathrm{T}$的闭子群。*

a) *用$\mathrm{W}_{G}(\mathrm{T})$中的$\mathrm{W}_{H}(\mathrm{T})$子群$\mathrm{N}_{H}(\mathrm{T})/\mathrm{T}$表示； 群 $H/H_{0}$ 同构于商群 $\mathrm{W}_{H}(\mathrm{T})/\mathrm{W}_{H_{0}}(\mathrm{T})$。*

b) *$H$是连通的当且仅当$\mathrm{W}_{G}(\mathrm{T})$的每个元素在$H$属于到$\mathrm{W}_{H_{0}}(\mathrm{T})$都有代表。*

断言 a) 源自 Cor. 8 Th。 2 (no. 2)，而断言 b) 是 a) 的特例。

### 6. 最大环面和覆盖范围同态

设G是连通的紧李群，T是G的最大环面。考虑G的导出群D(G)及其通用覆盖$\widetilde{D}(G)$；令 $p: \widetilde{D}(G)\rightarrow G$ 为规范态射 $\widetilde{D}(G)\rightarrow D(G)$ 和 $D(G)\rightarrow G$ 的复合。那么$\widetilde{D}(G)$是一个连通的紧李群（§1, no. 4，第4条命题的Cor.2）；此外，在$p$下T的逆像$\widetilde{T}$是$\widetilde{D}(G)$的最大环面（no. 3，命题1）。

#### 引理 2 {#lie-ix-s2-lem-2 .statement tag=01AO}

令 H 为李群的李群、$f_T: T\rightarrow H$ 和 $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ 态射，这样对于所有 $t\in \widetilde{T}$ 来说，$f_T(p(t)) = \widetilde{f}(t)$。存在李群$f: G\rightarrow H$的唯一态射使得$f\circ p= \widetilde{f}$并且使得$f$到T的限制是$f_T$。

把$Z = C(G)_0$；由 §1, no. 4 提供，Cor.第 4 条命题 1，李群 $g: Z\times \widetilde{D}(G)\rightarrow G$ 中的态射，使得 $g(z, x) =z^{-1}p(x)$ 是一个覆盖层；它的核由对$(z, x)$组成，使得$p(x) =z$，其中$x\in p^{-1}(Z)\subset \widetilde{T}$。由于态射$(z, x) \rightarrow f_T(z^{-1}) \widetilde{f}(x)$从$Z\times \widetilde{D}(G)$到H映射Ker$g$到$\{e\}$，存在从G到H的态射$f$，使得对于$z\in Z$有$f\circ p= \widetilde{f}$和$f(z) =f_T(z)$。但我们也有 $f(t) =f_T(t)$ 对应 $t\in p( \widetilde{T})$；因为$T = Z.p( \widetilde{T})$，$f$到T的限制确实是$f_T$。

#### 命题 8 {#lie-ix-s2-prop-8 .statement tag=01AP}

令 G 为连通的紧李群，T 为 G 的最大环面，H 李群和李代数的 $\varphi : L(G)\rightarrow L(H)$ 同态。存在李群 $f: G\rightarrow H$ 的态射使得 $L(f) =\varphi$ 当且仅当存在李群 $f_T: T\rightarrow H$ 的态射使得 $L(f_T) =\varphi |L(T)$；然后$f_T=f|T$。

如果$f: G\rightarrow H$是李群的态射，使得$L(f) =\varphi$，$f$到T的限制$f_T$是从T到H的唯一态射，使得$L(f_T) =\varphi |L(T)$。相反，令 $f_T: T\rightarrow H$ 为李群的态射，使得 $L(f_T) =\varphi |L(T)$。令$\widetilde{D}(G)$和$p$如上； 映射$L(p)$诱导同构从$L( \widetilde{D}(G))$到L(G)的派生代数$\mathfrak{b}$。存在李群$\widetilde{f}: \widetilde{D}(G)\rightarrow H$的态射使得$L( \widetilde{f}) = (\varphi |\mathfrak{b})\circ L(p)$（第III, §6, no. 1，第1章）。从$\widetilde{T}$到H诱导的态射$t \rightarrow \widetilde{f}(t)$和$t \rightarrow f_T(p(t))$与李代数相同的同态，因此重合。 应用引理 2，我们推导出态射$f: G\rightarrow H$的存在性使得$L(f)$和$\varphi$重合在L(T)和$\mathfrak{b}$上。从$L(G) =\mathfrak{b}+ L(T)$开始，我们有$L(f) =\varphi$。

#### 命题 9 {#lie-ix-s2-prop-9 .statement tag=01AQ}

令 G 为连通的紧李群，T 为 G、H 李群和 $f: G\rightarrow H$ 态射的最大值环面。那么 $f$ 是单射的当且仅当它的限制到 T 是单射的。

事实上，Th. 2 (no. 2) G 约化到单位元素的正常子群 Ker $f$ 当且仅当其交与 T 约化到单位元素。

### 习题{#lie-ix-s2-exercises}

§ 2](exercises/s2/)参见[习题。
