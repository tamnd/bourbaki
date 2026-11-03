---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 1
section_title: COMPARISON OF FUNCTIONS ON A FILTERED SET
lang: zh
source: fvr-i-vii
book_pages: 211-220
pdf_pages: 0226-0235, 0274-0274
extraction: ocr
subsections:
    - "no": 1
      title: 'COMPARISON RELATIONS: I. WEAK RELATIONS'
      page: 211
      pdf_page: 226
    - "no": 2
      title: 'COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 214
      pdf_page: 229
    - "no": 3
      title: CHANGE OF VARIABLE
      page: 217
      pdf_page: 232
    - "no": 4
      title: COMPARISON RELATIONS BETWEEN STRICTLY POSITIVE FUNCTIONS
      page: 217
      pdf_page: 232
    - "no": 5
      title: NOTATION
      page: 219
      pdf_page: 234
statements: 38
exercises: 3
content_sha256: 78db92e3f85210fada336024f82bc9ca43aa480b1965071048c316d80aed1031
translated_from: content/en/fvr/V/01_s1_comparison_of_functions_on_a_filtered.md
translation_method: google
source_content_sha256: 8313e76e55f08fcd7dd783b09028bd3331bcb51b6229df45213a85cc59097f4a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 8d4ec27d79d01305d2cd5d7254bd556fb3751d42f8f96ffcdd7273e0cf457cb1
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。 函数与过滤后的集合的比较

令 E 被基 $\mathfrak{F}$ 的过滤器过滤为集合 (*Gen.Top.*, I, p. 58);在这个章中，我们将考虑函数，其定义的域是E属于的子集到过滤器基$\mathfrak{F}$（子集取决于函数），并且其值要么域或实数 $\mathbf{R}$，或者更一般地，在标准化的向量空间中，超过有价值的域（*Gen. Top.*、IX、p. 170）。

在应用中，E 通常是实空间 $\mathbf{R}^n$ 的子空间，或者延长线 $\overline{\mathbf{R}}$，$\mathfrak{F}$ 是 E 的闭包点的邻域过滤器在 E 上的迹，或者是 E 的相对紧凑的子集的补集过滤器（“无穷远处点的邻域”）。

一般来说，仅仅知道这样的函数趋向于沿着$\mathfrak{F}$的给定极限能够处理由此函数形成的表达式的“沿着$\mathfrak{F}$到极限的通道”的所有问题是不够的。

例如，当实数变量 x 趋于 $+\infty$ 时，三个函数 $x$、$x^2$ 和 $\sqrt{x}$ 都趋于 $+\infty$，但是，表达式

$$
(x+1)^2 - x^2, \quad (x+1) - x, \quad \sqrt{x+1} - \sqrt{x},
$$

第一个趋向于$+\infty$，第二个趋于1，第三个趋于0。

因此，不仅要了解函数沿$\mathfrak{F}$的极限值（当极限存在时），还要了解函数接近其极限的“方式”；在其他字中，导致对函数中的集合进行分类，其趋向于相同的极限。

### 1. 比较关系：I。弱关系

在下文中，我们用V表示在值域K上的规范化向量空间，并用函数的$\mathscr{H}(\mathfrak{F}, V)$集合和V中的值表示，每个都在E的子集上定义属于至过滤器基 $\mathfrak{F}$。 关系，我们将在函数之间的定义相对于带有基$\mathfrak{F}$的过滤器有一个*本地*特征标：让我们澄清一下这是什么意思。如果 f 和 g 是 $\mathscr{H}(\mathfrak{F}, V)$ 中的两个函数，请回想一下关系“存在集合 $Z \in \mathfrak{F}$，使得 f 和 g 在 Z 上定义且相等”是 $\mathscr{H}(\mathfrak{F}, V)$ 上的 *等价关系 $R_\infty$ (*Gen.Top.*, I, p. 66）。既然如此，我们可以说涉及$\mathscr{H}(\mathfrak{F}, V)$的函数$f$的关系S相对于$f$是*本地*特征标（沿着$\mathfrak{F}$），如果它与等价关系*相容的*（在$f$中） $R_\infty$ (*集合理论*, II, p. 117);我们知道，如果$\tilde{f}$是$f$沿$\mathfrak{F}$的*胚芽*，$f$模$R_\infty$的等价类（商集$\mathscr{H}_\infty(\mathfrak{F}, V) = \mathscr{H}(\mathfrak{F}, V)/R_\infty$的元素），那么可以从S导出，通过商、关系在$\tilde{f}$和S的其他参数之间，并且相反，相对于$f$，局部特征标的这种性质的每个关系定义关系。

#### 例 {#fvr-v-s1-n1-exa-5 .statement tag=08DN}

如果$f$和$g$是$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的两个函数，则关系“存在一个$X \in \mathfrak{F}$，使得对于每个$t \in X$，在$X$和$f(t) \leq g(t)$上定义了$f$和$g$”是局部的特征标相对于 $f$ 和 $g$。我们用经过到商获得的$\tilde{f} \leq \tilde{g}$关系表示（对于$f$和$g$）；我们注意到，如果$\tilde{f} \leq \tilde{g}$，则存在函数$f_1 \in \tilde{f}$和函数$g_1 \in \tilde{g}$，定义在*所有*E上，使得$f_1(t) \leq g_1(t)$适用于所有$t \in E$。

#### 注 {#fvr-v-s1-n1-rem-3 .statement tag=0E5L}

1) 令$V_i$ ($1 \leq i \leq n$) 为$n$在K上范数为向量空间，并且$\varphi$函数定义在$V_1 \times V_2 \times \cdots \times V_n$上，值在V中；由经过至商沿 $R_\infty$ 函数 $\varphi$ 定义映射从
$$
\mathscr{H}_\infty(\mathfrak{F}, V_1) \times \cdots \times \mathscr{H}_\infty(\mathfrak{F}, V_n)
$$
到 $\mathscr{H}_\infty(\mathfrak{F}, V)$，最常用 $\varphi(\tilde{f}_1, \ldots, \tilde{f}_n)$ 表示（*Gen.Top.*、I、p. 67）。例如，对于 $\mathscr{H}_\infty(\mathfrak{F}, V)$、元素 $\tilde{f} + \tilde{g}$ 中的任意两种细菌$\tilde{f}, \tilde{g}$，将$\varphi$ 取为映射 $(x, y) \mapsto x + y$ 和$x \mapsto x\lambda$ ($\lambda \in K$)，因此定义和$\tilde{f}\lambda$，并且立即验证合成$(\tilde{f}, \tilde{g}) \mapsto \tilde{f} + \tilde{g}$和$(\lambda, \tilde{f}) \mapsto \tilde{f}\lambda$定义在$\mathscr{H}_\infty(\mathfrak{F}, V)$a *向量空间*结构超过域K的规则；其中空间$\tilde{O}$是$\mathfrak{F}$中集合上函数等于0所形成的类，而$-\tilde{f}$是函数等于$-f$上所形成的类集合 $\mathfrak{F}$。同样，如果V是K上的*代数*，则$\mathscr{H}_\infty(\mathfrak{F}, V)$上的一个定义通过取$\varphi(x, y) = xy$得到合成$(\tilde{f}, \tilde{g}) \mapsto \tilde{f}\tilde{g}$的第二个内部规则；与前面的两条规则一起，在 $\mathscr{H}_\infty(\mathfrak{F}, V)$ 上，定义和 *代数* 结构超过 K；如果V有单位元 e，则$\mathscr{H}_\infty(\mathfrak{F}, V)$有由函数形成的单位元类$\tilde{e}$等于$\mathfrak{F}$中某些集合上的e；对于$\tilde{f}$在$\mathscr{H}_\infty(\mathfrak{F}, V)$中“可逆”，对于某些$f \in \tilde{f}$，存在一个$Z \in \mathfrak{F}$，使得对于每个$t \in Z$，$f(t)$在V中可逆（在这种情况下，每个条件满足每个函数在类$\tilde{f}$）。

2）同样的记号，令$\psi$为$\prod_{i=1}^n V_i$的子集的映射变为V；我们用$\psi(f_1, f_2, \ldots, f_n)$函数表示在每个点$t \in E$处等于$\psi(f_1(t), f_2(t), \ldots, f_n(t))$，其中$f_i(t)$被定义并且其中点$(f_i(t))$属于到集合其中$\psi$ 定义为 $^1$。例如，在每个点 $t \in E$ 处，$f + g$ 函数等于 $f(t) + g(t)$，其中$f$ 和 $g$ 均已定义。观察映射$(f, g) \mapsto f + g$*在$\mathscr{H}(\mathfrak{F}, V)$上不是群运算*，因为如果$f$未在所有E上定义，则不存在函数$g \in \mathscr{H}(\mathfrak{F}, V)$使得$f + g = 0$。

#### 定义 1 {#fvr-v-s1-def-1 .statement tag=08DO}

*给定两个真实的函数* $f, g$ *属于到* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$，*它们是* $\geq 0$ *在* $\mathfrak{F}$中的集合，*我们说* $f$ *由* $g$主导，*或者* $g$ *支配*$f$*（沿着*$\mathfrak{F}$*），并写*$f \preceq g$*或*$g \succeq f$，*如果有集合*$X \in \mathfrak{F}$*和数*$k > 0$*这样*$f(t) \leq k\ g(t)$*对于每个* $t \in X$ *（在其他字中，如果存在* $k > 0$ *使得* $\tilde{f} \leq k\ \tilde{g}$）

$^1$ 特别是，在接下来的所有内容中，给定$\mathscr{H}(\mathfrak{F}, V)$中的函数$f$，我们将用$\|f\|$函数$t \mapsto \|f(t)\|$表示，其中属于到$\mathscr{H}(\mathfrak{F}, \mathbf{R})$并且在相同的集合上定义为$f$：我们明确提请注意，在此章$\|f\|$是*函数*而不是*数*。

给定两个规范化的向量空间$V_1, V_2$和两个函数$f_1, f_2$属于分别对应于$\mathscr{H}(\mathfrak{F}, V_1)$和$\mathscr{H}(\mathfrak{F}, V_2)$，可以说$f_1$受$f_2$支配（沿着$\mathfrak{F}$），并写$f_1 \preccurlyeq f_2$ 或 $f_2 \succeq f_1$，如果 $\|f_1\| \preccurlyeq \|f_2\|$。

关系 $f_1 \preccurlyeq f_2$ 在$f_1$和$f_2$中显然是本地特征标；因此，它相当于由经过到商导出的关系 $\tilde{f}_1 \preccurlyeq \tilde{f}_2$。当$f$和$g$是真实的函数时，必须小心不要混淆关系、$\tilde{f} \preccurlyeq \tilde{g}$和$\tilde{f} \leq \tilde{g}$。

请注意，对于每个标量 $\lambda \neq 0$ 关系 $f_1 \preccurlyeq f_2 \lambda$ *等于* $f_1 \preccurlyeq f_2$。如果$f_1 \preccurlyeq f_2$存在集合$X \in \mathfrak{F}$，使得每个点$x \in X$都有$f_1(x) = 0$，其中$f_2(x) = 0$。

#### 例 {#fvr-v-s1-n1-exa-6 .statement tag=0E5I}

1) 关系 $f \preccurlyeq 1$ 表示 $f$ *有界*在 $\mathfrak{F}$ 的集合上。

2) 对于$\mathscr{H}(\mathfrak{F}, V)$的每一个函数$f$，以及每个标量$\lambda \neq 0$，都有$f \preccurlyeq f \lambda$。
3) 当$x$趋于$+\infty$时，就有$\sin^2 x \preccurlyeq \sin x$。
4) 当 $\mathbf{R}^2$ 中 $(x, y)$ 趋于 $(0, 0)$ 时，有
$$
xy \preccurlyeq x^2 + y^2.
$$

以下命题是def的直接的推论。 1：

#### 命题 1 {#fvr-v-s1-prop-1 .statement tag=08DP}

*如果* $f, g, h$ *是* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 中的三个函数 *则关系* $f \preccurlyeq g$ *和* $g \preccurlyeq h$ *意味着* $f \preccurlyeq h$。

#### 命题 2 {#fvr-v-s1-prop-2 .statement tag=08DQ}

*令*$f_1, f_2$*为*$\mathscr{H}(\mathfrak{F}, V)$*中的两个函数*和*$g$*函数在*$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中。 *关系* $f_1 \preccurlyeq g$ *和* $f_2 \preccurlyeq g$ *暗示* $f_1 + f_2 \preccurlyeq g$。

进一步：

#### 命题 3 {#fvr-v-s1-prop-3 .statement tag=08DR}

*令*$V_1, V_2, V$*为相同值域*上的三个范数空间，并且$(x, y) \mapsto [x.y]$*双线性映射从*$V_1 \times V_2$*到*$V$。 *如果* $f_1$ *和* $f_2$ *分别是函数在* $\mathscr{H}(\mathfrak{F}, V_1)$ *和* $\mathscr{H}(\mathfrak{F}, V_2)$ *，并且* $g_1, g_2$ *是两个函数在* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ *这样* $f_1 \preccurlyeq g_1$ *和* $f_2 \preccurlyeq g_2$*然后*$[f_1.f_2] \preccurlyeq g_1 g_2$。

确实 (*Gen.Top.*, IX, p. 173, th.1) 存在数 $a > 0$ 使得
$$
|[f_1.f_2]| \leq a \|f_1\| \|f_2\|.
$$

#### 推论 {#fvr-v-s1-n1-cor-1 .statement tag=08DS}

*如果* $V$ *是标准化的代数*，*如果* $f_1, f_2$ *是* $\mathscr{H}(\mathfrak{F}, V)$中的两个函数，*和* $g_1, g_2$ *是* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的两个函数，*则关系* $f_1 \preccurlyeq g_1, f_2 \preccurlyeq g_2$ *暗示* $f_1 f_2 \preccurlyeq g_1 g_2$。

$\mathscr{H}(\mathfrak{F}, V)$ 中的函数之间的关系 $f \preccurlyeq g$ 是通过属性“传递”的。 1;因为它是 *​​自反* 关系 "*f \preccurlyeq g 和 g \preccurlyeq f*" 是 $\mathscr{H}(\mathfrak{F}, V)$ (*集合理论*, II, p. 113) 上的 *等价关系*。

#### 定义 2 {#fvr-v-s1-def-2 .statement tag=08DT}

*给定两个函数* $f, g$ *of* $\mathscr{H}(\mathfrak{F}, V)$ *我们说* $f$ *和* $g$ *相似（沿着* $\mathfrak{F}$），*并写* $f \simeq g$，*如果* $f \preccurlyeq g$ *和* $g \preccurlyeq f$。

对于每个标量 $\lambda \neq 0$ 关系 $f \simeq g$ 等价于 $f \simeq g \lambda$。这意味着集合$X \in \mathfrak{F}$的存在，使得点的$X$的子集（其中$f(x) = 0$）与点的$X$的子集（其中$g(x) = 0$）相同。

#### 例 1 {#fvr-v-s1-n1-exa-1 .statement tag=08DU}

对于实数函数 $f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$ 关系 $f \simeq 1$ 意味着有两个数 $a > 0,\ b > 0$，使得 $a \leq |f(x)| \leq b$ 位于 $\mathfrak{F}$ 中的集合上，或者函数 $\log |f|$ 的边界为$\mathfrak{F}$ 中的集合：然后可以说 $f$ 是 $\mathfrak{F}$ 中的集合的“对数有界”。

#### 例 2 {#fvr-v-s1-n1-exa-2 .statement tag=08DV}

令 $V$ 为非离散值域 $K$ 上的标准化空间，并令 $f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ 为变量 $x \in K$ 中的多项式，系数位于 $V$ 中，使得$a_0 \neq 0$。对于每一个向量$b \neq 0$，都有一个$f(x) \simeq b x^n$，因为$|x|$趋向于$+\infty$。

#### 例 3 {#fvr-v-s1-n1-exa-3 .statement tag=08DW}

我们已经看到，$\sin^2 x \preccurlyeq \sin x$随着$x$趋向于$+\infty$，但是*我们没有*$\sin^2 x \simeq \sin x$，甚至虽然，这些函数也会同时消失于点。

#### 例 4 {#fvr-v-s1-n1-exa-4 .statement tag=08DX}

当$(x,\ y)$在$\mathbf{R}^2$中趋于$(0,\ 0)$时，一个人有$x^2 + xy + y^2 \simeq x^2 + y^2$，但*不是*$xy \simeq x^2 + y^2$。

它立即来自 prop。 V、p. 213中的 3 个，如果 $f_1,\ f_2,\ g_1,\ g_2$ 是 $\mathscr{H}(\mathfrak{F}, K)$ 中的函数（$K$ 是任何值域）关系 $f_1 \simeq g_1$ 和 $f_2 \simeq g_2$ 则意味着$f_1 f_2 \simeq g_1 g_2$。

我们注意到，相比之下，关系$f_1 \simeq g_1$和$f_2 \simeq g_2$*并不意味着*$f_1 + f_2 \simeq g_1 + g_2$，如例$f_1(x) = g_1(x) = x^2,\ f_2(x) = -(x^2 + x),\ g_2(x) = -(x^2 - 1)$所示，因为实数变量$x$趋向于$+\infty$。

比较关系$f \preccurlyeq g,\ f \simeq g$据说是*弱*。我们说，$\mathscr{H}(\mathfrak{F}, V)$中的两个函数$f,\ g$是“弱可比性”，如果它们满足（至少）是关系$f \preccurlyeq g,\ g \preccurlyeq f$中的一个。

#### 注 1 {#fvr-v-s1-n1-rem-1 .statement tag=08DY}

$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的两个函数不需要弱可比，如函数1的例和$x \sin x$所示，因为$x$趋向于$+\infty$。

#### 注 2 {#fvr-v-s1-n1-rem-2 .statement tag=08DZ}

在$\mathscr{H}(\mathfrak{F}, V)$上用$R_0$关系$f \simeq g$表示，并用$\mathscr{H}_0(\mathfrak{F}, V)$商集$\mathscr{H}(\mathfrak{F}, V)/R_0$表示；请注意，关系$R$*意味着*$R_0$。 经过到商关系 $f \preccurlyeq g$ 通过道具给出。 1 个V、p. 213、$\mathscr{H}_0(\mathfrak{F}, V)$ 上的 *序关系*（*集合理论*、III、p. 134）；前面的例表明$\mathscr{H}_0(\mathfrak{F}, V)$*没有被这个关系完全排序*。

### 2. 比较关系：II。强关系

#### 定义 3 {#fvr-v-s1-def-3 .statement tag=08E0}

*给定两个实数函数* $f,\ g$ *属于到* $\mathscr{H}(\mathfrak{F}, \mathbf{R})$，*它们是* $\geq 0$ *在* $\mathfrak{F}$中的集合，*一个说* $f$ *相对于* $g$可以忽略不计，*或者* $g$ *优于* $f$ *（沿着* $\mathfrak{F}$），*有人写* $f \ll g$ *或* $g \gg f$ *如果，对于每个* $\varepsilon > 0$，*存在集合* $X \in \mathfrak{F}$ *这样* $f(t) \leq \varepsilon g(t)$ *对于每个* $t \in X$。

*给定两个范数空间* $V_1,\ V_2$ *和两个函数* $f_1,\ f_2$ *属于分别到* $\mathscr{H}(\mathfrak{F}, V_1)$ *和* $\mathscr{H}(\mathfrak{F}, V_2)$ *，有人说* $f_1$ *相对于* $f_2$ 可以忽略不计*（沿着* $\mathfrak{F}$），*一个人写* $f_1 \ll f_2$ *或* $f_2 \gg f_1$，*如果* $\|f_1\| \ll \|f_2\|$。

对于每个标量 $\lambda \neq 0$ 关系 $f_1 \ll f_2 \lambda$ *等于* $f_1 \ll f_2$。 关系 $f_1 \ll f_2$ 暗示 $f_1 \preccurlyeq f_2$ 但不等同于它。

请注意，关系$f_1 \preccurlyeq f_2$绝不意味着关系“$f_1 \ll f_2$或$f_1 \asymp f_2$”：一个人有$\sin x \preccurlyeq 1$，因为$x$倾向于$+\infty$，但关系$\sin x \ll 1$或$\sin x \asymp 1$ 是真的。

#### 例 {#fvr-v-s1-n2-exa-8 .statement tag=0E5N}

1) 关系 $f \ll 1$ 意味着$f$ *沿$\mathfrak{F}$*趋于0。

2) 当$\alpha$和$\beta$是两个实数时，$\alpha < \beta$一个有$x^\alpha \ll x^\beta$，而$x$趋于$+\infty$。类似地，当$m$和$n$是两个有理整数时，$m < n$其中一个有$z^m \ll z^n$，因为复数$z$趋于$\infty$。

3) 由于$x$趋向于$+\infty$，每有整数$n$就有$x^n \ll e^x$（III，p. 105）。

4) 在 $\mathbf{R}^2$ 中，随着 $(x, y)$ 趋于 $(0, 0)$，
$$
x^2 + y^2 \ll |x| + |y|.
$$

从 def 可以立即推导出以下命题。 3：

#### 命题 4 {#fvr-v-s1-prop-4 .statement tag=08E1}

*如果$f, g, h$是$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的三个函数，则关系$f \preccurlyeq g$和$g \ll h$（分别是$f \ll g$和$g \preccurlyeq h$）意味着$f \ll h$。*

#### 命题 5 {#fvr-v-s1-prop-5 .statement tag=08E2}

*令$f_1, f_2$为$\mathscr{H}(\mathfrak{F}, V)$中的两个函数，以及$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的$g$函数。那么关系$f_1 \ll g$和$f_2 \ll g$意味着$f_1 + f_2 \ll g$。*

此外，与 prop 中的论点相同。 V、p. 213中的3表明：

#### 命题 6 {#fvr-v-s1-prop-6 .statement tag=08E3}

*带有记号的支柱。 3、关系$f_1 \ll g_1$和$f_2 \preccurlyeq g_2$（分别为$f_1 \preccurlyeq g_1$和$f_2 \ll g_2$）意味着$[f_1.f_2] \ll g_1g_2$。*

命题4表明，$\mathscr{H}(\mathfrak{F}, V)$中函数之间的关系$f \ll g$是*及物*；但*它不是自反的*：准确地说，关系$f \ll f$意味着$f$*在$\mathfrak{F}$*中消失在集合上（在其他字中，$f$相当于0模$R_\infty$）；事实上，对于$\varepsilon$使得$0 < \varepsilon < 1$存在一个$X \in \mathfrak{F}$使得对于每个$x \in X$有$\|f(x)\| \leq \varepsilon \|f(x)\|$，只有当$f(x) = 0$对于每个$x \in X$才有可能。由此可见，关系“f \ll g 和 g \ll f”是传递且对称的，但不是自反：因此它不是等价关系（这意味着存在集合$X \in \mathfrak{F}$，使得每个$x \in X$都有$f(x) = g(x) = 0$）。

#### 命题 7 {#fvr-v-s1-prop-7 .statement tag=08E4}

*如果$f$和$g$是$\mathscr{H}(\mathfrak{F}, V)$中的两个函数，则关系$f - g \ll f$相当于$f - g \ll g$。*

事实上，$f - g \ll f$意味着对于每个$\varepsilon > 0$都存在一个$X \in \mathfrak{F}$，这样对于每个$x \in X$都存在$\|f(x) - g(x)\| \leq \varepsilon \|f(x)\|$。但然后是 $(1 - \varepsilon) \|f(x)\| \leq \|g(x)\|$，进而是 $f \preccurlyeq g$、从而（V、p. 215，道具 4）$f - g \ll g$。

#### 推论 {#fvr-v-s1-n2-cor-1 .statement tag=08E5}

*关系$f - g \ll f$是$\mathscr{H}(\mathfrak{F}, V)$上的等价关系。*

事实上，如果$f - g \ll f$和$g - h \ll g$，那么$f - g \ll g$，从而（V，p. 215，道具5）$f - h \ll g$，因而，从$g \preceq f$开始，我们有$f - h \ll f$，这表明这个关系是及物;它是由道具对称的。 7，并且显然是反身的，从而推论。

#### 定义 4 {#fvr-v-s1-def-4 .statement tag=08E6}

*给定* $\mathscr{H}(\mathfrak{F}, V)$ *的两个函数* $f, g$ *一个说* $f$ *和* $g$ *是等价的（沿着* $\mathfrak{F}$），*并写* $f \sim g$，*如果* $f - g \ll f$。

关系 $f \sim g$ 暗示 $f \asymp g$ 但不等同于它。

#### 例 1 {#fvr-v-s1-n2-exa-1 .statement tag=08E7}

如果$a$是常数函数，$\neq 0$在$E$上，关系$f \sim a$意味着$f$*趋于*$a$*沿着*$\mathfrak{F}$。

#### 例 2 {#fvr-v-s1-n2-exa-2 .statement tag=08E8}

令 $V$ 为非离散值域 $K$ 上的范数空间，并令 $f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ 为变量 $x \in K$ 中的多项式，系数位于 $V$ 中，使得 $a_0 \neq 0$。然后 $f(x) \sim a_0 x^n$ 因为 $|x|$ 趋向于 $+\infty$。

#### 例 3 {#fvr-v-s1-n2-exa-3 .statement tag=08E9}

当实数$x$趋于$+\infty$时，一个人就有$\left( 1 + \frac{1}{x} \right) \sin x \sim \sin x$。

#### 例 4 {#fvr-v-s1-n2-exa-4 .statement tag=08EA}

由于复数变量 $z$ 趋于 0，因此有 $e^z - 1 \sim z$。更一般地，如果 $V$ 是在值域 $K$ 上的标准化空间，并且 $f$ 是在 $x_0 \in K$ 的邻域上定义的函数，值在 $V$ 中，并且允许导数$f'(x_0) \neq 0$在点$x_0$，然后，当$x$接近$x_0$时，我们有$f(x) - f(x_0) \sim f'(x_0)(x - x_0)$（I，p. 3，定义1）。

#### 例 5 {#fvr-v-s1-n2-exa-5 .statement tag=08EB}

当$(x, y)$在$\mathbf{R}^2$接近$(0, 0)$时，有
$$
\sqrt{\sin^2 x + \sin^2 y} \sim \sqrt{x^2 + y^2}.
$$

#### 例 6 {#fvr-v-s1-n2-exa-6 .statement tag=08EC}

设 $f(x, y)$ 是一个多项式，其中实数系数位于两个实数变量 $x, y$ 中，没有常数项。如果当 $x$ 接近 0 而剩余 $> 0$ 时，存在函数 $\varphi(x)$，在区间 $[0, a]$ 上连续，并且使得 $\varphi(0) = 0$ 和 $f(x, \varphi(x)) = 0$ 对于 $0 \leq x \leq a$，可以证明存在有理数数$r$和实数$\lambda \neq 0$使得$\varphi(x) \sim \lambda x^r$（V，p. 259，练习3）。

#### 例 7 {#fvr-v-s1-n2-exa-7 .statement tag=08ED}

对于每个$x > 0$，让$\pi(x)$表示素数数的数，即$\leq x$；已经证明，$\pi(x) \sim x / \log x$$^2$和$x$趋向于$+\infty$。

#### 注 {#fvr-v-s1-n2-rem-3 .statement tag=08EE}

请注意，关系$f \sim g$绝不意味着差值$f - g$沿$\mathfrak{F}$趋于0；这种差异甚至可以是“无界”的，如例$x^2 + x \sim x^2$所示，因为$x$趋于$+\infty$。

#### 命题 8 {#fvr-v-s1-prop-8 .statement tag=08EF}

*设*$K$*是一个有价值的域和*$f_1, f_2, g_1, g_2$*四个函数在*$\mathscr{H}(\mathfrak{F}, K)$; *然后关系* $f_1 \sim g_1$ *和* $f_2 \sim g_2$ *意味着* $f_1 f_2 \sim g_1 g_2$。

事实上，我们有 $f_1 f_2 - g_1 g_2 = f_1 (f_2 - g_2) + (f_1 - g_1) g_2$；从$f_1 \preceq g_1$、$f_1 - g_1 \ll g_1$和$f_2 - g_2 \ll g_2$开始，我们有$f_1 f_2 - g_1 g_2 \ll g_1 g_2$（V、p. 215，第5条和第6条）。

相比之下，我们在 V、p. 214 中给出了例，其中有 $f_1 = g_1$、$f_2 \sim g_2$，但关系 $f_1 + f_2 \asymp g_1 + g_2$ 不成立（因此 *更不必说* 也不成立）
$$
f_1 + f_2 \sim g_1 + g_2).
$$
2 例如，参见 A. E. INGHAM，*素数数* 的分布（剑桥小册子，n 30），剑桥大学出版社，1932 年。

比较关系$f \ll g, f \sim g$称为强关系。 $\mathscr{H}(\mathfrak{F}, V)$ 中的两个函数 $f, g$ 被称为可比较（或当人们想避免任何可能的混淆时强可比），如果它们满足是三个关系：$f \ll g, f \gg g$之一，或者“存在一个$\lambda \neq 0$使得$f \sim g\lambda$”。

#### 注 1 {#fvr-v-s1-n2-rem-1 .statement tag=08EG}

两个函数可以弱可比，虽然则不能强可比，例如函数1和$\sin x$，因为$x$倾向于$+\infty$。

#### 注 2 {#fvr-v-s1-n2-rem-2 .statement tag=08EH}

在空间$V_1, V_2$比较关系$f_1 \preccurlyeq f_2$和$f_1 \ll f_2$范数的定义中，其中$f_1$和$f_2$分别取它们的值，仅明显涉及；实际上，仅涉及$V_1$和$V_2$上的拓扑，因为当$V_1$或$V_2$上的替换、范数被等效的关系替换时，关系、$f_1 \preccurlyeq f_2$和$f_1 \ll f_2$被等效的关系替代范数（\emph{Gen.Top.}，IX，p. 170，def.7）。

### 3. 变量的变换

让$\varphi$是从集合$E'$到$E$的映射，这样$\varphi^{-1}(\mathfrak{F})$是$E'$上的过滤器基。很明显，如果$\mathscr{H}(\mathfrak{F}, V_1)$和$\mathscr{H}(\mathfrak{F}, V_2)$中的$f_1, f_2$分别为函数，则$f_1 \circ \varphi, f_2 \circ \varphi$属于分别为$\mathscr{H}(\varphi^{-1}(\mathfrak{F}), V_1)$和$\mathscr{H}(\varphi^{-1}(\mathfrak{F}), V_2)$，并且关系$f_1 \preccurlyeq f_2$（分别为$f_1 \ll f_2$）为相当于$f_1 \circ \varphi \preccurlyeq f_2 \circ \varphi$（分别为$f_1 \circ \varphi \ll f_2 \circ \varphi$）。

### 4. 严格正函数之间的比较关系

令$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的$g$为函数，这对$\mathfrak{F}$中的集合严格为正。具有$g$的比较关系可以用另一个方式表示：关系$f \preccurlyeq g$等价于说，$\|f\|/g$（在$\mathfrak{F}$中的集合上定义）以集合为界$\mathfrak{F}$； 关系$f \ll g$相当于说，$\|f\|/g$沿$\mathfrak{F}$趋于0。如果 $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 关系 $f \asymp g$ 中 $f$ 为函数，则表示 $f/g$ 以对数方式有界于 $\mathfrak{F}$ 中的集合，并且关系 $f \sim g$ $f/g$沿$\mathfrak{F}$趋于1。如果$f$在$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中为函数，并且$\mathfrak{F}$中的集合为正，则说$f$和$g$具有可比性意味着$f/g$趋向于极限（有限或等于$+\infty$） $\mathfrak{F}$。

#### 命题 9 {#fvr-v-s1-prop-9 .statement tag=08EI}

令$f$和$g$为$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的两个函数，对$\mathfrak{F}$中的集合严格为正。为了使$f$和$g$具有可比性，对于每个数$t \geqslant 0$（最多有一个例外），函数$f - tg$在$\mathfrak{F}$中的集合上具有常数符号$^3$是必要且充分的。

条件是必要的。事实上，如果$f \ll g$除了$t = 0$之外还有$f - tg \sim -tg$，那么$f - tg$在$\mathfrak{F}$中的集合上严格为负，除了$t = 0$；如果$f \gg g$，则对于所有$t$，$f - tg$在$\mathfrak{F}$中的集合上严格为正；最后，如果$f \sim kg$（$k$常数$> 0$），则$f - t g \sim (k - t)g$除了$t = k$之外，因此，除了$t = k$之外，$f - t g$在$\mathfrak{F}$中的集合上具有$k - t$的符号。

条件就足够了。事实上，假设比率 $f/g$ 沿着 $\mathfrak{F}$ 有两个不同的簇点 $\alpha < \beta$。对于*每个* 数 $t$，使得$\alpha < t < \beta$存在于*每个* 集合 $X \in \mathfrak{F}$ 两个点 $x_1, x_2$，使得$f(x_1)/g(x_1) < t$和$f(x_2)/g(x_2) > t$；因而$f(x) - t g(x)$在$X$上没有常数符号；我们得出了与假设不相容的结论。由此可见，$f/g$ 沿着带有基 $\mathfrak{F}$ 的过滤器只能*有一个*簇值（有限或无限），因而，(*Gen.Top.*, I, p. 85, 推论) 将此值作为其*极限* 沿$\mathfrak{F}$。

#### 命题 10 {#fvr-v-s1-prop-10 .statement tag=08EJ}

*设$f$和$g$为$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的两个函数，它们对$\mathfrak{F}$中的集合严格为正；对于每个$\alpha$实数和$\neq 0$关系$f \asymp g$（分别$f \sim g$）等价于$f^\alpha \asymp g^\alpha$（分别$f^\alpha \sim g^\alpha$）；如果 $\alpha > 0$ 关系 $f \preccurlyeq g$（分别为 $f \ll g$）相当于 $f^\alpha \preccurlyeq g^\alpha$（分别为 $f^\alpha \ll g^\alpha$）；如果 $\alpha < 0$ 则相当于 $f^\alpha \succcurlyeq g^\alpha$（分别为 $f^\alpha \succ g^\alpha$）。*

证明是直接的。

有人注意到，在函数的 $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 集合 $I'$ 中，$\mathfrak{F}$ 中的集合严格为正，使得 $\Gamma/\mathbf{R}_\infty$ 是 $\mathscr{H}_\infty(\mathfrak{F}, \mathbf{R})$ 中的 *乘法群* $\Gamma_\infty$； $\Gamma/\mathbf{R}_0$ 与 $\Gamma$ 中对数有界函数的类（模 $\mathbf{R}_\infty$）的子群与 $\Gamma_\infty$ 的商群相同；在$\Gamma/\mathbf{R}_0$序关系上，从关系$f \preccurlyeq g$通过商推导出来，与$\Gamma/\mathbf{R}_0$的群结构“兼容”，从而使其成为有序的群。

#### 命题 11 {#fvr-v-s1-prop-11 .statement tag=08EK}

*令$g$为$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的函数，使得$\lim_{\mathfrak{F}} g = +\infty$； 关系 $f \ll g$ 意味着 $e^f \ll e^g$； 关系 $f \sim g$ 意味着$\log f \sim \log g$。*

事实上，如果$f \ll g$，那么$f - g = g \left( \frac{f}{g} - 1 \right)$趋于沿着$\mathfrak{F}$趋向于$-\infty$。类似地，如果$f \sim g$有一个$\log f = \log g + \log \frac{f}{g}$，那么$\log f - \log g$趋于0，$\frac{\log f}{\log g} - 1 = \frac{\log f - \log g}{\log g}$也是如此。

另一方面，请注意，关系$f \sim g$*并不意味着*$e^f \sim e^g$，甚至也不意味着$e^f \asymp e^g$，如例所示，其中$f(x) = x^2, \ g(x) = x^3 + x$与$x$趋向于$+\infty$；同样，关系$f \ll g$*并不意味着*$\log f \ll \log g$，如例$f(x) = x, \ g(x) = x^2$所示，因为$x$趋于$+\infty$。

#### 定义 5 {#fvr-v-s1-def-5 .statement tag=08EL}

*令$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的$g$为函数，$\mathfrak{F}$中的集合严格为正，并且使得$\lim_{\mathfrak{F}} g = 0$或$\lim_{\mathfrak{F}} g = +\infty$。有人说，如果$\lim_{\mathfrak{F}} \log(|f|)/\log g = \rho$，函数$f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$相对于$g$而言是阶$\rho$（有限或无限）。*

请注意，如果 $f$ 相对于 $g$ 为阶 $\rho$，则 $f$ 相对于 $1/g$ 为阶 $-\rho$；因此，只需处理$g(x)$沿$\mathfrak{F}$趋向于$+\infty$的情况。

#### 命题 12 {#fvr-v-s1-prop-12 .statement tag=08EM}

令g为$\mathscr{H}(\mathfrak{F}, \mathbf{R})$中的函数，使得$\lim_{\mathfrak{F}} g = +\infty$；令 f 为 $\mathscr{H}(\mathfrak{F}, \mathbf{R})$ 中的函数。

a) 要使 f 相对于 g 为阶 $+\infty$，对于每个 $\alpha \geq 0$ $f \gg g^\alpha$ 是充分必要的。

b) 要使 f 相对于 g 为阶 $-\infty$，对于每个 $\alpha > 0$ $f \ll g^{-\alpha}$ 是充分必要的。

c) 要使 f 相对于 g 的有限阶等于 $\rho$，对于每一个 $\varepsilon > 0$，有 $g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$ 是充分必要的。

例如，让我们证明c)。如果 f 相对于 g 的阶为 $\rho$，则对于每个 $\varepsilon > 0$，存在集合 $M \in \mathfrak{F}$，这样，对于每个 $x \in M$，我们有

$$
\left( \rho - \frac{\varepsilon}{2} \right) \log g(x) \leq \log |f(x)| \leq \left( \rho + \frac{\varepsilon}{2} \right) \log g(x),
$$

或 $(g(x))^{\rho - \frac{\varepsilon}{2}} \leq |f(x)| \leq (g(x))^{\rho + \frac{\varepsilon}{2}}$；因为$\lim_{\mathfrak{F}} g = +\infty$因此每$\varepsilon > 0$就有$g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$； 逆命题是直接的。 a) 和 b) 的证明相似。

请注意，如果 f 相对于 g 为有限阶 $\rho$，则 $fg^{-\rho}$ 相对于 g 为阶 0，反之亦然；如果$f_1$（或$f_2$）相对于g 具有阶 $\rho_1$（或$\rho_2$），并且如果定义了$\rho_1 + \rho_2$，则$f_1 f_2$ 相对于g 具有阶 $\rho_1 + \rho_2$。

#### 注 1 {#fvr-v-s1-n4-rem-1 .statement tag=08EN}

观察到虽然 f 相对于 g 可能是有限的阶 $\rho$，但比率 $f/g^\rho$ 不必趋向于极限；例如，每个对数有界函数相对于 g 都是阶 0，但不需要沿着 $\mathfrak{F}$ 具有极限。

#### 注 2 {#fvr-v-s1-n4-rem-2 .statement tag=08EO}

在$\mathfrak{F}$中的集合上定义的函数不需要具有相对于g的确定的阶（有限或非有限），因为具有相对于g的确定的阶的函数与g的所有幂相当，最多有一个例外。现在 f 不需要有这个性质，正如从例 $g(x) = x,\ f(x) = 1 + x^2 \sin^2 x$ 看到的那样（因为 x 趋于 $+\infty$）。在此，例 f 与 $\alpha < 0$ 和 $\alpha > 2$ 的 $g^\alpha$ 相当；如果取 $f(x) = e^x \sin^2 x + e^{-x} \cos^2 x$，则 f 无法与 g 的任何幂（正或负）进行比较。

### 5. 记号

给定一个实数函数$f \in \mathscr{H}(\mathfrak{F}, \mathbf{R})$，在公式中，对于由f主导的函数，通常可以方便地写出$O(f)$，对于相对于f可忽略不计的函数，写出$o(f)$。当在证明中，存在多个受相同函数 f（分别相对于 f 可以忽略不计）支配的函数时，我们用 $O_1(f),\ O_2(f)$ 等（分别 $o_1(f),\ o_2(f)$ 等）表示它们。

许多作者不加区别地将证明中的所有函数写为 $O(f)$（或 $o(f)$），而这些证明中由 f 主导（或相对于 f 可以忽略不计），这是一种语言滥用，可能会带来混淆的风险。

有了这个记号我们就可以表达道具了。 1, 2, 3 (V, p. 213)如下：如果$g = O_1(f)$且$h = O(g)$则$h = O_2(f)$；一个人可以写

$$
\sum_{i=1}^{n} \lambda_i O_i(f) = O_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{1}
$$
$$
O(f) \, O(g) = O(fg). \tag{2}
$$

同样，道具。 4（V，p. 215）表明，如果$g = O_1(f)$和$h = o(g)$（分别为$g = o_1(f)$和$h = O(g)$），则$h = o_2(f)$，以及道具。 5和6（V，p. 5）可以用形式表示
$$
\sum_{i=1}^{n} \lambda_i o_i(f) = o_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{3}
$$
$$
o(f) \, O(g) = o(fg). \tag{4}
$$

关系 $f \sim g$ 相当于$f = g + o(g)$。 记号 $O(1)$（或$o(1)$）表示函数以$\mathfrak{F}$中的集合为界（或函数沿$\mathfrak{F}$趋于0）。

### 习题{#fvr-v-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
