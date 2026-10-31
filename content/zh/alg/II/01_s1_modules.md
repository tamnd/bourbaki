---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 1
section_title: Modules
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 191-227, 380-386
pdf_pages: 0215-0251, 0404-0410
extraction: ocr
subsections:
    - "no": 1
      title: MODULES; VECTOR SPACES; LINEAR COMBINATIONS
      page: 191
      pdf_page: 215
    - "no": 2
      title: LINEAR MAPPINGS
      page: 194
      pdf_page: 218
    - "no": 3
      title: SUBMODULES; QUOTIENT MODULES
      page: 196
      pdf_page: 220
    - "no": 4
      title: EXACT SEQUENCES
      page: 197
      pdf_page: 221
    - "no": 5
      title: PRODUCTS OF MODULES
      page: 200
      pdf_page: 224
    - "no": 6
      title: DIRECT SUM OF MODULES
      page: 202
      pdf_page: 226
    - "no": 7
      title: INTERSECTION AND SUM OF SUBMODULES
      page: 205
      pdf_page: 229
    - "no": 8
      title: DIRECT SUMS OF SUBMODULES
      page: 208
      pdf_page: 232
    - "no": 9
      title: SUPPLEMENTARY SUBMODULES
      page: 210
      pdf_page: 234
    - "no": 10
      title: MODULES OF FINITE LENGTH
      page: 212
      pdf_page: 236
    - "no": 11
      title: FREE FAMILIES. BASES
      page: 214
      pdf_page: 238
    - "no": 12
      title: ANNIHILATORS. FAITHFUL MODULES. MONOGENOUS MODULES
      page: 219
      pdf_page: 243
    - "no": 13
      title: CHANGE OF RING OF SCALARS
      page: 221
      pdf_page: 245
    - "no": 14
      title: MULTIMODULES
      page: 224
      pdf_page: 248
statements: 88
exercises: 27
content_sha256: 812f55bffecb52ab08673db72d978ba4a379ae4cf23828c05ccfbffaa991f567
translated_from: content/en/alg/II/01_s1_modules.md
translation_method: google
source_content_sha256: 7b2cea857b009f809085412ca64248b0f317359a2bcbd7a3a189e12a6f0b01fe
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: bc7f2af2bf3dd67c19b4532baa1af3a3f193a7ac366fe57a89e144aae57bfd75
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 1。 模

### 1.模； 向量空间； 线性组合

#### 定义 1 {#alg-ii-s1-def-1 .statement tag=05JO}

*给定环* $\mathbf{A}$，*左模超过* $\mathbf{A}$（*或左* $\mathbf{A}$-*模*）*是集合* $\mathbf{E}$ *通过给定定义代数结构*：

(1) *在* $\mathbf{E}$ 上可交换群运算 （*在下面附加地写出*）；

(2) *作用* $(\alpha, x) \mapsto \alpha \top x$的律，*其算子域为环* $\mathbf{A}$ *且满足以下公理*：

$$
\begin{align*}
(\mathbf{M_I})\quad & \alpha \top (x + y) = (\alpha \top x) + (\alpha \top y) \text{ for all } \alpha \in \mathbf{A}, x \in \mathbf{E}, y \in \mathbf{E}; \\
(\mathbf{M_{II}})\quad & (\alpha + \beta) \top x = (\alpha \top x) + (\beta \top x) \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{III}})\quad & \alpha \top (\beta \top x) = (\alpha \beta) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{IV}})\quad & 1 \top x = x \text{ for all } x \in \mathbf{E}.
\end{align*}
$$

公理$(\mathbf{M_I})$意味着左$\mathbf{A}$-模块$\mathbf{E}$的外法则相对于$\mathbf{E}$上的加法是“可分配的”；因此，模是与运算符可交换的群。

如果在定义 1 中，公理 $(\mathbf{M_{III}})$ 被替换为

$$
(\mathbf{M'_{III}})\quad \alpha \top (\beta \top x) = (\beta \alpha) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E},
$$

由此定义的代数结构的 E 是 A 或右A-模上的右模。

当谈到 A-模（左或右）时，环 A 的元素通常称为标量。

通常外法则或合成或左A-模（或右A-模）写成乘法，运算符写在左边（或右边）；然后条件 (M_{III}) 写成$\alpha(\beta x) = (\alpha\beta)x$，条件 (M'_{III}) 写成$(x\beta)\alpha = x(\beta\alpha)$。

如果 $A^0$ 表示逆环到 A (I, § 8, no. 3)，则模 E 在环 A 上的每个右权都是左模在环 $A^0$ 上。由此可见，可以对模的属性进行阐述，同时系统地将注意力限制在左模或右模；在§§ 1和2中，我们通常会对左模进行这种解释，当我们谈到模时（不指定哪个型），我们指的是左模，其外法则将被写成乘法。当环 A 是可交换的时，右模和左模对于 A 的概念是相同的。

对于所有 $\alpha \in A$，A-模 E 的映射 $x \mapsto \alpha x$ 自身被称为位似与 E 的$\alpha$ 之比 (I, § 4, no. 2)；通过 (M_I) 位似是 E 上可交换的群结构（无运算符）的自同态，但一般不是 E 上的模结构（I, § 4, no. 2；cf. II, § 1, no. 2 和 no. 13）。因此$\alpha 0 = 0$和$\alpha(-x) = -(\alpha x)$；如果 $\alpha$ 是 A 的可逆元，位似 $x \mapsto \alpha x$ 是 E 上交换律群结构（无运算符）的自同构，因为关系 $y = \alpha x$ 凭借 (M_IV) 意味着$x = \alpha^{-1}(\alpha x) = \alpha^{-1}y$。

类似地，根据(M_{II})，对于所有$x \in E$，映射$\alpha \mapsto \alpha x$是加法群A的同态到可交换的群（无运算符）E；因此$0x = 0$和$(-\alpha)x = -(\alpha x)$；此外，通过(M_IV)，对于每整数$n \in \mathbf{Z}$，$n.x = (n.1)x$。

当环 A 仅由元素 0 组成时，每个 A-模 E 仅由元素 0 组成，则 A 中的 $1 = 0$，从而，对于所有 $x \in E$，
$x = 1.x = 0.x = 0$。

#### 例 {#alg-ii-s1-n1-exa-1 .statement tag=05JP}

(1) 设$\phi$为环A的同态入环B； 映射 $(a, x) \mapsto \phi(a)x$（或$(a, x) \mapsto x\phi(a)$）的$A \times B$进入B 定义，在B左侧（或右侧）A-模结构。特别是，如果 A 上的 $\phi$ 被取为恒等映射，则在 A 上获得规范的左（右）A-模结构；为了避免混淆，集合 A 与结构表示为$A_s$（分别为$A_d$）。

(2) 在由外法则 $(n, x) \mapsto n.x$ (I, § 3, no. 1) 定义的运算符结构的交换群 G（加法写）群上，模结构超过环 $\mathbf{Z}$ 有理数整数。

(3) 令 E 为可加写的交换律群，E 的 $\mathscr{E}$ 自同态环 (I, § 8, no. 3：回想一下，两个自同态的乘积 $fg$ 是由定义合成的自同态$f \circ g$）。 E 上运算符 $f \in \mathscr{E}$ 和元素 $x \in E$ 定义之间的外法则 $(f, x) \mapsto f(x)$ 是规范的左 $\mathscr{E}$ 模块结构。

现在考虑环 A 并假设 E 上有左（右）A-模结构；对于所有 $\alpha \in A$、位似 $h_\alpha : x \mapsto \alpha x$（分别为 $x \mapsto x\alpha$）属于至 $\mathscr{E}$； 映射 $\phi : \alpha \mapsto h_\alpha$ 是环 A（分别为逆环 $A^0$）到环 $\mathscr{E}$ 的同态和定义 $\alpha x = (\phi(\alpha))(x)$（分别为 $x\alpha = (\phi(\alpha))(x)$）。 相反，通过上面的公式在 E 上给环同态 $\phi : A \to \mathscr{E}$（分别为 $\phi : A^0 \to \mathscr{E}$）定义一个左（分别为右）A-模结构。 在其他字中，在加法群 E 上给予左（或右）A-模结构以及添加剂律给定的群运算相当于给予环同态 $A \to \mathscr{E}$（或 $A^0 \to \mathscr{E}$）。

#### 定义 2 {#alg-ii-s1-def-2 .statement tag=05JQ}

*左（右）向量空间超过域 K 是左（右）K-模。*

向量空间中的元素是有时称为*向量*。

#### 例 {#alg-ii-s1-n1-exa-2 .statement tag=05JR}

(4) 域相对于任意子域来说既是左又是右向量空间。

*(5)* 三个维数$\mathbf{R}^3$的实数空间相对于实数$\mathbf{R}$域、实数乘积$tx$为向量空间 $t$和点$x$，坐标$x_1, x_2, x_3$是点，坐标$tx_1, tx_2, tx_3$。类似地，在任意集合 F 上定义的实值函数的集合是向量空间，而$\mathbf{R}$、乘积 $tf$ 实数 $t$ 和函数 $f$ 是实值函数 $x \mapsto tf(x)$.*

对于两个族 $(x_i)_{i \in I}, (y_i)_{i \in I}$ of 元素 of A-模 E of 有限支撑 (I, § 2, no. 1)，以下等式成立：

(1)
$$
\sum_{i \in I} (x_i + y_i) = \sum_{i \in I} x_i + \sum_{i \in I} y_i
$$

(2)
$$
\alpha \cdot \sum_{i \in I} x_i = \sum_{i \in I} (\alpha x_i) \quad \text{for all } \alpha \in A;
$$
通过考虑 I 包含的有限子集 H 以及 $(x_i)$ 和 $(y_i)$ 的支持，方程立即简化为有限和的类似方程。

#### 定义 3 {#alg-ii-s1-def-3 .statement tag=05JS}

*如果存在有限支撑的A的元素的族$(\lambda_i)_{i \in I}$，则A-模E的元素x被称为线性组合，且E的$(a_i)_{i \in I}$族的A中的系数为元素，使得$x = \sum_{i \in I} \lambda_i a_i$。*

一般来说，有几个不同的家族$(\lambda_i)$满足这个条件（cf.no. 11）。

注 0 是 E 的元素空族中唯一的线性组合（按照 I, § 2, no. 1 的约定）。

### 2.线性映射

#### 定义 4 {#alg-ii-s1-def-4 .statement tag=05JT}

设 E 和 F 是关于同一个环 A 的两个（左）模。E 到 F 的线性映射（或A-线性映射、或同态、或 A 同态）是任意映射 u : E → F，使得：

(3) $u(x + y) = u(x) + u(y)$ 为 $x \in E, y \in E;$

(4G) $u(\lambda . x) = \lambda . u(x)$ $\lambda \in A, x \in E.$

如果E和F是两个右A-模，则线性映射$u : E \to F$是映射满足 (3)

(4D) $u(x . \lambda) = u(x) . \lambda$ 为 $\lambda \in A, x \in E.$

#### 注 {#alg-ii-s1-n2-rem-1 .statement tag=05JU}

当E和F是两个可交换的群视为环$\mathbf{Z}$（no. 1）上的模时，群E（无运算符）的每个同态$u$进入群F（无运算符）也等于E的线性映射进入F，因为对于 n 整数 > 0，关系 $u(n . x) = n . u(x)$ 从 $u(x + y) = u(x) + u(y)$ 到 n 上的归纳，对于$n = -m < 0$，
$$
u(n . x) = u(-(m . x)) = -u(m . x) = -(m . u(x)) = n . u(x).
$$

#### 例 {#alg-ii-s1-n2-exa-1 .statement tag=05JV}

(1) 令E为A-模且E的元素； A-模 $A_s$ 到 E 中的映射 $\lambda \mapsto \lambda a$ 为线性映射 $\theta_a$，使得 $\theta_a(1) = a.$
*(2) 令 I 为 I 上可微实值函数的实直线 $\mathbf{R}$、E 向量空间和 I 上定义的所有实值函数的 F 向量空间的开区间。映射 $x \mapsto x'$ 与每个可微分相关联函数 x 从 E 到 F 的导数是线性映射。*

注，A-模E上的位似$x \mapsto \alpha x$不一定是线性映射：在其他字，关系$\alpha(\lambda x) = \lambda(\alpha x)$不一定对所有$\lambda \in A$和$x \in E$成立。然而，当 A 的 $\alpha$ 属于到中心时，关系成立； $x \mapsto \alpha x$ 则称为中心位似 (cf. no. 13)。

如果$u : E \to F$是线性映射，那么，对于E的元素的每个家庭$(x_i)_{i \in I}$和A的元素的每个家庭$(\lambda_i)_{i \in I}$，使得家庭$(\lambda_i x_i)_{i \in I}$的支持是有限的，

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i)
$$

如下紧接着（3）和（4G）由归纳以家庭支持$(\lambda_i x_i)$为基数。

#### 命题 1 {#alg-ii-s1-prop-1 .statement tag=05JW}

设E、F、G为三个A-模，E的u线性映射为F，F的v线性映射为G。则复合映射$v \circ u$是线性的。

(1) *如果 u:E → F 和 v:F → E 是两个线性映射，使得 v ∘ u 是 E 上的恒等映射，u ∘ v 是 F 上的恒等映射，u 是 E 到 F 上的同构，v 是逆同构。*

(2) *每个双射线性映射 u:E → F 都是 E 到 F 上的同构。*

这些命题紧随定义 4 之后。

命题 1 和 2 表明，线性映射可以看作A-模结构的类的*态射*（*集合理论*，IV, § 2, no. 1）；从此以后，我们将始终假设态射中的选择已经完成。

给定两个左（右）A-模 E 和 F，令 Hom(E, F) 或 Hom_A(E, F) 表示 E 的线性映射到 F 的集合。

集合 Hom(E, F) 是乘积的 *交换环*、子群可交换群 F^E，将 E 的所有映射转换为 F (I, § 4, no. 8)；回想一下，对于 F^E 的两个元素 u, v 以及所有 x ∈ E，

$$(u + v)(x) = u(x) + v(x), \quad (-u)(x) = -u(x)$$

从而紧接着，如果 u 和 v 是线性的，那么 u + v 和 −u 也是线性的。如果 G 是 Hom(E, F) 的左第三个（右）A-模, f, f_1, f_2 元素和 Hom(F, G) 的 g, g_1, g_2 元素，则立即验证以下关系：

(6) $$g \circ (f_1 + f_2) = g \circ f_1 + g \circ f_2$$
(7) $$(g_1 + g_2) \circ f = g_1 \circ f + g_2 \circ f$$
(8) $$g \circ (-f) = (-g) \circ f = -(g \circ f).$$

特别是，Hom(E, E) 定义上的合成 (f, g) ↦ f ∘ g 的律以及 Hom(E, E) 上的上述加法群结构 a *环* 结构，其中单位元，用 1_E 表示或Id_E，在E上是恒等映射； E 的线性映射自身也称为 A-模 E 的 *自同态*，环 Hom(E, E) 也表示为 End(E) 或 End_A(E)。 A-模 E 的 *自同构* 只是 End(E) (命题 2) 的*可逆* 元素；它们形式乘法*群*，用Aut(E)或GL(E)表示，也称为相对于E的*线性群*。

从 (6) 和 (7) 可以得出，对于两个 A-模 E, F, Hom(E, F)，在环 Hom(F, F) 上具有 *左模* 的规范结构，在 Hom(E, E) 上有 *右模* 的规范结构。

令 E、F、E'、F' 为四（左）A-模，u:E' → E 和 v:F → F' A-线性映射。如果每个元素 f ∈ Hom(E, F) 都与元素 v ∘ f ∘ u ∈ Hom(E', F') 关联，则映射

$$\operatorname{Hom}(E, F) \to \operatorname{Hom}(E', F')$$

定义为$\mathbf{Z}$-线性，用$\mathrm{Hom}(u, v)$或$\mathrm{Hom}_A(u, v)$表示。如果$u, u_1, u_2$属于到$\mathrm{Hom}(E', E)$且$v, v_1, v_2$到$\mathrm{Hom}(F, F')$，则

$$
\begin{cases}
\mathrm{Hom}(u_1 + u_2, v) = \mathrm{Hom}(u_1, v) + \mathrm{Hom}(u_2, v) \\
\mathrm{Hom}(u, v_1 + v_2) = \mathrm{Hom}(u, v_1) + \mathrm{Hom}(u, v_2)
\end{cases}
$$

令$E'', F''$为两个$A$模块，$u': E'' \to E'$和$v': F' \to F''$线性映射。然后

$$
\mathrm{Hom}(u \circ u', v' \circ v) = \mathrm{Hom}(u', v') \circ \mathrm{Hom}(u, v).
$$

如果$u$是$E'$的同构到$E$，并且$F$的$v$同构到$F'$，则$\mathrm{Hom}(u, v)$是$\mathrm{Hom}(E, F)$的同构到$\mathrm{Hom}(E', F')$，其逆同构通过 (10) 等于 $\mathrm{Hom}(u^{-1}, v^{-1})$。

如果$h$（或$k$）是$E$（或$F$）的自同态，则$\mathrm{Hom}(h, 1_F)$（或$\mathrm{Hom}(1_E, k)$）只是位似，其比率为$h$（或$k$）。左）模结构位于上面定义的环 $\mathrm{End}(E)$（或$\mathrm{End}(F)$）上。

### 3.子模; 商模

设$E$为$A$模，$M$子集为$E$；对于$E$到诱导上的$A$模块结构以及$M$上的$A$模块结构，$M$是$E$（I, § 4, no. 3）的稳定子群是必要且充分的，因为如果是这样，则结构为群与$M$ 上引出的算子显然满足公理 ($M_{II}$)、($M_{III}$) 和 ($M_{IV}$)；那么 $M$ 和这个结构 （或者，滥用语言，集合 $M$ 本身）被称为 $E$ 的子模； 典范嵌入$M \to E$是线性映射。当$E$为向量空间时，其子模称为向量子空间（或者在不引起混淆的情况下简称为子空间）。

#### 例 {#alg-ii-s1-n3-exa-1 .statement tag=05JX}

(1) 在任何 0 的模 $E$ 集合由……组成中，子模 （零子模，通常用 0 表示，滥用记号）。
(2) 设$A$为环。 $A_s$（或$A_d$）的子模只是环$A$的左理想（或右理想）。
(3) 设$E$为$A$模，$x$元素为$E$的$a$为$A$的左理想。 元素 $\alpha x$的集合，其中$\alpha$贯穿$a$，是$E$的子模，用$ax$表示。
(4) 在被视为$\mathbf{Z}$模(no. 1)的交换群$G$中，$G$的每个子群也是子模。

*(5) 设$I$为实直线$\mathbf{R}$的开区间；在$I$上定义且连续的实值函数的集合$C$是在$I$上定义的所有实值函数的向量空间$\mathbf{R}^I$的向量子空间。类似地，$I$上可微的函数的集合$D$是$C_*$的向量子空间*

令 $E$ 为 $A$ 模块。每个$E$上与模结构兼容的等价关系（I, § 1, no. 6）都是形式$x - y \in M$，其中$M$是E（I, § 4, no. 4）的稳定子群，即E的子模。立即验证商群 E/M (I, § 4, no. 4) 上有运算符的群的结构为A-模结构，其中典范映射 $E \to E/M$ 是线性的；有了这个结构，E/M 被称为 E 与子模 M 的 *商模*。 向量空间 E 的商模被称为 E 的*商向量空间*（或简称为*商空间*）。

*例* (6)。 左A-模 $A_s$ 环定义商模 $A_s/a$ 中各左理想$a$；由于滥用记号，这个商模通常被表示为$A/a$。

设E、F为两个A-模。从群与运算符（I, § 4, no. 5）（或直接从定义）的一般性质可以得出，如果$u : E \to F$是线性映射，则E的任何子模的$u$下的像是F的子模和逆像 F 的任意子模的 $u$ 是 E 的子模。 特别是，*核* $N = \overline{u}^{-1}(0)$ 是 E 的子模，$u$ 下的 E 的像 $u(E)$ 是 F 的子模 （I, § 4, no. 6，命题7）；通过滥用语言，$u(E)$ 被称为 u* 的 *像。 商模$E/N$也称为$u$的*共像*和商模$F/u(E)$$u$的*余核*。在 $u$ (I, § 4, no. 5) 的*规范分解* 中

$$
u : E \xrightarrow{p} E/N \xrightarrow{v} u(E) \xrightarrow{i} F
$$

$v$ 是 $u$ 到 $u$ 的像的余像 *同构*（no. 2，命题 2）。对于$u$是*内射*，其核是零是充分必要的；对于$u$是*满射*，其余核是零是充分必要的。

$u$的核、像、coimage和余核分别用Ker$u$、Im$u$、Coim$u$、Coker$u$表示。

#### 注{#alg-ii-s1-n3-rem-1 .statement tag=05JY}

令 M 为 A-模 E 和 $\phi : E \to E/M$ 典范同态的子模。对于A-线性映射$u : E \to F$为形式$v \circ \phi$，其中$v$是E/M到F中的线性映射，$M \subset \mathrm{Ker}(u)$是充分必要的；因为，如果这个条件成立，关系$x - y \in M$意味着$u(x) = u(y)$，因此$u$与这个等价关系兼容，并且显然从$u$取商得出的映射$v : E/M \to F$是线性的。

### 4.正合序列

#### 定义 5 {#alg-ii-s1-def-5 .statement tag=05JZ}

*设F、G、H为三个A-模；设 f 是 F 到 G 的同态，g 是 G 到 H 的同态。 有序对 (f, g) 称为正合序列 if*

$$
g^{-1}(0) = f(F)
$$

*在其他字中，如果g的核等于f的像。*

图表

(12)
$$
F \xrightarrow{f} G \xrightarrow{g} H
$$
也称为 *正合序列*。

我们类似地考虑四个A-模和三个同态中的图表由……组成：

(13)
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

如果图表 $E \xrightarrow{f} F \xrightarrow{g} G$ 精确，则该图表被称为 *精确于* F；如果 $F \xrightarrow{g} G \xrightarrow{h} H$ 是精确的，则它被称为*精确于* G。如果图表 (13) *精确于* F *和* G，则简单地称为*精确*，或*正合序列*。 正合序列与任意数项的定义类似。

#### 注 {#alg-ii-s1-n4-rem-1 .statement tag=05K0}

(1) 若有序对$(f, g)$为正合序列，则$g \circ f = 0$；但当然，这个性质并不表征正合序列，因为它只意味着$f$的像“包含于”在$g$的核中。

下面叙述中，E、F、G表示A-模，0 A-模缩减为单位元素；箭头代表A-模同态。由于从模 0 到模 E（分别是 E 到 0）只有一个同态，因此在正合序列中为这些同态命名时没有点它们出现的地方。

#### 命题 3 {#alg-ii-s1-prop-3 .statement tag=05K1}

(a) *对于*
$$
0 \longrightarrow E \xrightarrow{f} F
$$
*要成为正合序列，* $f$ *是单射的*是必要且充分的。

(b) *对于*
$$
E \xrightarrow{f} F \longrightarrow 0
$$
*要成为正合序列，* $f$ *是满射的*是必要且充分的。

(c) *对于*
$$
0 \longrightarrow E \xrightarrow{f} F \longrightarrow 0
$$
*要成为正合序列，* $f$ *是双射*（在其他字（no. 2，命题 2）中，$f$是E到F的*同构*）是必要且充分的。

(d) *如果* F * 是 * E * 的子模且* $i : F \to E$ * 是典范嵌入，* $p : E \to E/F$ *典范同态，图表*
(14)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0
$$
*是正合序列。*

(e) *如果$f : E \to F$是同态，图表*

$$
0 \longrightarrow f^{-1}(0) \overset{i}{\longrightarrow} E \overset{f}{\longrightarrow} F \overset{p}{\longrightarrow} F/f(E) \to 0
$$

*（其中$i$是典范嵌入，$p$典范满射）是正合序列。*

命题紧接在no. 2的定义和命题2之后。

#### 注 {#alg-ii-s1-n4-rem-2 .statement tag=05K2}

(2) 说有正合序列

$$
0 \longrightarrow E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \longrightarrow 0
$$

意味着$f$是单射的，$g$是满射的，并且与$g$相关的规范双射是$F/f(E)$到$G$的*同构*。也有人说，三元组$(F, f, g)$是模G乘模E*（I, § 6, no. 7）的*扩张。

(3) 如果有正合序列和 4 项

$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \overset{h}{\longrightarrow} H
$$

$f$的余核是$F/f(E) = F/g^{-1}(0)$，$h$的核是$g(F)$；因此，与 $g$ 关联的规范双射是 *同构*

$$
\operatorname{Coker} f \to \operatorname{Ker} h.
$$

(4) 考虑A-模同态中的有序对

$$(15)$$
$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G.
$$

对于图表 (15) 为正合序列，存在两个A-模 S、T 和同态 $a : E \to S,\ b : S \to F,\ c : F \to T,\ d : T \to G$ 是充分必要的，使得三个序列

$$(16)$$
$$
\begin{cases}
E \overset{a}{\longrightarrow} S \longrightarrow 0 \\
0 \longrightarrow S \overset{b}{\longrightarrow} F \overset{c}{\longrightarrow} T \longrightarrow 0 \\
0 \longrightarrow T \overset{d}{\longrightarrow} G
\end{cases}
$$

是*精确*和$f = b \circ a$和$g = d \circ c$。

If (15) is an exact sequence, then take $S = f(E) = g^{-1}(0)$ and $T = g(F)$, $b$ and $d$ being the canonical injections and $a$ (resp. $c$) the homomorphism with the same graph as $f$ (resp. $g$). 反之，如果S、T、a、b、c、d满足上述条件，则$f(E) = b(a(E)) = b(S)$和$g^{-1}(0) = c(d(0)) = c(0)$，因此(16)的正确性表明$f(E) = g^{-1}(0)$。

当参数不需要时，通常会省略使用显式字母来表示正合序列中的同态。

#### 注 {#alg-ii-s1-n4-rem-3 .statement tag=05K3}

(5) 正合序列扩展的定义立即到群，它们不一定可交换；在这种情况下，当然使用乘法记号，并将公式中的0替换为1（如果不产生混淆）。 命题 3 的部分 (a)、(b)、(c) 仍然有效，并且 (d) 当 F 是 E 的正规子群时。 注 2 和命题 3(e) 在条件上，$f(E)$ 是 F 的正规子群； 注 3 和 4 无需修改即可有效。

### 5. 乘积的模

设$(E_i)_{i \in I}$是环A上的模的族。立即验证$E_i$上模结构的乘积（$I, § 4,$no. 8）是A-模结构在乘积上集合$E = \prod_{i \in I} E_i$。这样结构集合E就称为模$E_i$的乘积模；如果$x = (x_i), y = (y_i)$是E的两个元素，那么

$$
\begin{cases}
x + y = (x_i + y_i) \\
\lambda \cdot x = (\lambda x_i)
\end{cases}
$$
对于所有$\lambda \in A$。

公式 (17) 表示投影 $pr_i : E \to E_i$ 是线性映射；这些映射显然是满射的。

回想一下，如果索引集合 I 为空，则乘积集合 $\prod_{i \in I} E_i$ 则由单个元素组成； 乘积模结构在这个集合上，那么唯一元素是0。

#### 命题 4 {#alg-ii-s1-prop-4 .statement tag=05K4}

*设*$E = \prod_{i \in I} E_i$*为A-模*$(E_i)_{i \in I}$家庭的乘积。 *对于每一个A-模* F *和每个线性映射* $f_i : F \to E_i$ *都存在一个且仅有一个映射* f *的* F *进入* E *使得* $pr_i \circ f = f_i$ *对于所有* $i \in I$ *并且这个映射是线性的*。

这直接从定义得出。

模的乘积是“结合的”：如果 $(J_\lambda)_{\lambda \in L}$ 是 I 的划分，则典范映射
$$
\prod_{i \in I} E_i \to \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} E_i \right)
$$
是同构。

#### 命题 5 {#alg-ii-s1-prop-5 .statement tag=05K5}

(i) *令* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *为具有相同索引集合* I 的两个A-模族； *对于线性映射* $f_i : E_i \to F_i$ ($i \in I$) 的每个族，*映射* $f : (x_i) \to (f_i(x_i))$ ** $\prod_i E_i$ *进入* $\prod_i F_i$ *（有时表示为* $\prod_i f_i$）*是线性的*。

(ii) *令* $(G_i)_{i \in I}$ *成为A-模的第三个族，其中* I *作为索引集合，并且对于所有*$i \in I,$，让$g_i : F_i \to G_i$为线性映射；让$g = \prod_i g_i$。准确地说，对于序列 $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ 中的每一个，序列是充分必要的

$$
\prod_i E_i \xrightarrow{f} \prod_i F_i \xrightarrow{g} \prod_i G_i
$$

准确地说。

断言 (i) 紧接着定义。另一方面，说$y = (y_i)$属于到$\operatorname{Ker}(g)$意味着$g_i(y_i) = 0$对于所有$i \in I$，因此$y_i \in \operatorname{Ker}(g_i)$对于所有$i \in I$；类似地，说$y$属于到$\operatorname{Im}(f)$意味着存在$x = (x_i) \in \prod_i E_i$使得$y = f(x)$，这相当于说，对于所有$i \in I$来说$y_i = f_i(x_i)$，或者对于所有$i \in I$来说也相当于$y_i \in \operatorname{Im}(f_i)$； 从而（二）。

#### 推论 {#alg-ii-s1-n5-cor-1 .statement tag=05K6}

在命题 5 的条件下，(i)，

$$
\operatorname{Ker}(f) = \prod_{i \in I} \operatorname{Ker}(f_i), \qquad \operatorname{Im}(f) = \prod_{i \in I} \operatorname{Im}(f_i)
$$

还有典范同构

$$
\operatorname{Coim}(f) \to \prod_{i \in I} \operatorname{Coim}(f_i), \qquad \operatorname{Coker}(f) = \prod_{i \in I} \operatorname{Coker}(f_i)
$$

通过分别与$\prod_i E_i$、模$\operatorname{Ker}(f)$的元素$x = (x_i)$类（分别与$\prod_i F_i$、模$\operatorname{Im}(f)$的元素$y = (y_i)$的类）相关联而获得$x_i$ 模组的类。 $\operatorname{Ker}(f_i)$（分别是$y_i$ mod. $\operatorname{Im}(f)$ 的类系列）。

特别是，对于 $f$ 是单射的（分别是满射、双射的、零），对于所有 $i \in I$、$f_i$ 是单射（分别是满射、双射的、零）是必要且充分的。

如果对于所有$i \in I$，我们认为$E_i$的子模$F_i$，模$\prod_{i \in I} F_i$是$\prod_{i \in I} E_i$的子模，并且根据命题5的推论，有典范同构

$$
\prod_{i \in I} (E_i/F_i) \to \left( \prod_{i \in I} E_i \right) / \left( \prod_{i \in I} F_i \right).
$$

乘积或模的一个重要的例是，所有因子模都等于相同的模$F$；那么他们的乘积$F^I$就是$I$的映射中的集合到$F$。 $I$ 上等于 $x$ 的常数函数的对角线映射 $F \to F^I$ 映射 $x \in F$ 是线性的。如果 $(E_i)_{i \in I}$ 是一系列 $A$ 模块，并且对于所有 $i \in I$，$f_i : F \to E_i$ 是线性映射，则 $F$ 的线性映射 $x \mapsto (f_i(x))$ 到 $\prod_{i \in I} E_i$ 的合成将$F^I$的映射$(x_i) \mapsto (f_i(x_i))$分解为$\prod_{i \in I} E_i$和对角线映射$F \to F^I$。

### 6.直和模

让$(E_i)_{i \in I}$是A-模的一个家庭，$F = \prod_{i \in I} E_i$是他们的乘积。 $x \in F$的集合$E$，使得除了指标的有限数之外，$\mathrm{pr}_i x = 0$显然是$F$的子模，称为族的外部直和（或简称为直和） 模 $(E_i)$ 并表示为 $\bigoplus_{i \in I} E_i$ (I, § 4, no. 9)。当 I 有限时，则 $\bigoplus_{i \in I} E_i = \prod_{i \in I} E_i$；如果$I = \{p, q\}$（$\mathbf{Z}$的间隔），我们也写

$$
\bigoplus_{i \in I} E_i = E_p \oplus E_{p+1} \oplus \cdots \oplus E_q.
$$

对于所有$\kappa \in I$，令$j_\kappa$为映射$E_\kappa \to F$，它与$F$的每个$x_\kappa \in E_\kappa$元素相关联，使得$\mathrm{pr}_i(j_\kappa(x_\kappa)) = 0$对应于$i \neq \kappa$和$\mathrm{pr}_\kappa(j_\kappa(x_\kappa)) = x_\kappa$； 直接的是$j_\kappa$是$E_\kappa$的单射线性映射到$E_i$的直和$E$，我们称之为典范嵌入； $E$的子模$j_\kappa(E_\kappa)$，与$E_\kappa$同构的，称为指标$\kappa$的$E$的分量子模。通常通过 $j_\kappa$ 来识别$E_\kappa$。

对于所有$x \in E = \bigoplus_{i \in I} E_i$，因此我们有

$$
x = \sum_{i \in I} j_i(\mathrm{pr}_i x).
$$

(20)

#### 命题 6 {#alg-ii-s1-prop-6 .statement tag=05K7}

*让*$(E_i)_{i \in I}$*成为A-模*、$M$*A-模的一个家庭，并且对于所有*$i \in I$，*让*$f_i : E_i \to M$*成为线性映射*。 *那么存在且仅有一个线性映射* $g : \bigoplus_{i \in I} E_i \to M$ *这样，对于所有* $i \in I$：

$$
g \circ j_i = f_i.
$$

(21)

根据 (20)，如果 $g$ 存在，那么必然对于所有 $x \in \bigoplus_{i \in I} E_i$，

$$
g(x) = \sum_i g(j_i(\mathrm{pr}_i(x))) = \sum_i f_i(\mathrm{pr}_i(x)),
$$

从而唯一性共$g$。相反，对于所有$x \in \bigoplus_{i \in I} E_i$，设定$g(x) = \sum_i f_i(\mathrm{pr}_i(x))$，立即验证线性映射已经定义为叙述的满足条件。

当不会引起混淆时，我们写$g = \sum_{i \in I} f_i$（这与I, § 2, no. 1的约定相反，当$(f_i)$家族不属于有限支撑时）。

特别是，如果 J 是 I 的任意子集，$i \in J$ 定义的典范嵌入 $j_i$ 是一个规范的线性映射 $j_J : \bigoplus_{i \in J} E_i \to \bigoplus_{i \in I} E_i$，它与每个 $(x_i)_{i \in I}$ 元素 $(x'_i)_{i \in I}$ 关联，使得 $x'_i = x_i$ 为$i \in J$，$x'_i = 0$为$i \notin J$；这个映射显然是内射的。此外，如果$(J_\lambda)_{\lambda \in L}$是I的划分，则映射$i : \bigoplus_{\lambda \in L} \left( \bigoplus_{i \in J_\lambda} E_i \right) \to \bigoplus_{i \in I} E_i$相应的到命题6的$(j_{J_\lambda})$家庭是一个称为规范的*同构的*（直和的“结合性”）。

#### 推论 1 {#alg-ii-s1-prop-6-cor-1 .statement tag=05K8}

*令$(E_i)_{i \in I}, (F_\lambda)_{\lambda \in L}$为A-模的两个族。 映射*
$$
\text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) \to \prod_{(i, \lambda) \in I \times L} \text{Hom}_A(E_i, F_\lambda)
$$
*与每个$g \in \text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right)$家族$(\operatorname{pr}_\lambda \circ g \circ j_i)$相关联的是一个$\mathbf{Z}$-模块同构（称为规范）。*

这是从命题 6 和 no. 5、命题 4 得出的。

#### 推论 2 {#alg-ii-s1-prop-6-cor-2 .statement tag=05K9}

*令$(E_i)_{i \in I}$为A-模、F A-模的族，对于每个$i \in I$，令$f_i : E_i \to F$为线性映射。为了使 $f = \sum_{i \in I} f_i$ 成为 $E = \bigoplus_{i \in I} E_i$ 的同构在 F 上，每个$i \in I$ 线性映射 $g_i : F \to E_i$ 存在以下属性是充分必要的：*
(1) $g_i \circ f_i = 1_{E_i}$ 对于所有 $i \in I$。
(2) $g_i \circ f_\kappa = 0$ 为 $i \neq \kappa$。
(3) *对于所有$y \in F$，家庭$(g_i(y))$有有限支撑并且*
$$
y = \sum_{i \in I} f_i(g_i(y)).
$$
注如果 I 是有限的，则最后的条件也可以写为
$$
\sum_{i \in I} f_i \circ g_i = 1_F.
$$
显然条件是必要的，因为他们已经满足了$g_i = \operatorname{pr}_i \circ f_i^{-1}$。相反，如果它们成立，则对于所有 $y \in F$，定义了$g(y) = \sum_i j_i(g_i(y))$，并且 $g$ 是 F 到 E 的线性映射是直接的。对于所有 $y \in F$，$f(g(y)) = \sum_i f_i(g_i(y)) = y$ 假设。另一方面，对于所有$x \in E$，$g_\kappa(f(x)) = g_\kappa \left( \sum_i f_i(\operatorname{pr}_i(x)) \right) = g_\kappa(f_\kappa(\operatorname{pr}_\kappa(x))) = \operatorname{pr}_\kappa(x)$乘以假设；

因此$g(f(x)) = \sum_i j_i(g_i(f(x))) = \sum_i j_i(\mathrm{pr}_i(x)) = x$，证明了推论。

#### 命题 7 {#alg-ii-s1-prop-7 .statement tag=05KA}

(i) *设* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *为两个系列的* $A$*-具有相同索引集合* $I$的模块； *对于线性映射* $f_i : E_i \to F_i$ ($i \in I$) 的每个家庭，*限制到* $\bigoplus_{i \in I} E_i$ *线性映射* $(x_i) \mapsto (f_i(x_i))$ *是线性映射* $f : \bigoplus_{i \in I} E_i \to \bigoplus_{i \in I} F_i$ *表示为* $\bigoplus_{i \in I} f_i$ *或* $\bigoplus_i f_i$ *（其中* $f = f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ *如果* $I = [p, q]$ *是* $\mathbf{Z}$* 中的一个区间）。*

(ii) *让*$(G_i)_{i \in I}$*成为*$A$*模块的第三个系列，其中*$I$*作为索引集合，并且对于所有*$i \in I$，*让*$g_i : F_i \to G_i$*成为线性映射；我们写* $g = \bigoplus_i g_i$。 *对于序列* $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ *准确地说，序列* 是充分必要的
$$
\bigoplus_i E_i \xrightarrow{f} \bigoplus_i F_i \xrightarrow{g} \bigoplus_i G_i
$$
*准确地说*。

显然，对于所有$(x_i) \in \bigoplus_i E_i$，族$(f_i(x_i))$有有限支撑、从而(i)。另一方面，说$\bigoplus_i F_i$属于到$\mathrm{Ker}(g)$的元素$y = (y_i)$意味着$y_i \in \mathrm{Ker}(g_i)$对于所有$i \in I$（no. 5，命题5）；类似地，如果$y_i \in \mathrm{Im}(f_i)$对于所有$i \in I$，则每个$i \in I$都存在$x_i \in E_i$，使得$y_i = f_i(x_i)$，并且当$y_i = 0$时，可以假设$x_i = 0$；因此$y \in \mathrm{Im}(f)$和逆命题是明显的。

#### 推论 1 {#alg-ii-s1-prop-7-cor-1 .statement tag=05KB}

*在条件下，命题 7 下，(i)，*
$$
\mathrm{Ker}(f) = \bigoplus_{i \in I} \mathrm{Ker}(f_i), \qquad \mathrm{Im}(f) = \bigoplus_{i \in I} \mathrm{Im}(f_i)
$$
*还有典范同构*
$$
\mathrm{Coim}(f) \to \bigoplus_{i \in I} \mathrm{Coim}(f_i), \qquad \mathrm{Coker}(f) \to \bigoplus_{i \in I} \mathrm{Coker}(f_i)
$$
*定义如no. 5，推论命题 5。特别是，对于* $f$ *是单射（分别是满射、双射的、零），每个* $f_i$ *都是单射（分别是满射、双射的、 零)*。

如果对于所有$i \in I$，我们认为$E_i$的子模$F_i$，模$\bigoplus_{i \in I} F_i$是$\bigoplus_{i \in I} E_i$的子模，并且根据推论1到命题7，有典范同构
$$
\bigoplus_{i \in I} (E_i/F_i) \to \left( \bigoplus_{i \in I} E_i \right) / \left( \bigoplus_{i \in I} F_i \right).
$$

#### 推论 2 {#alg-ii-s1-prop-7-cor-2 .statement tag=05KC}

令$(E_i)_{i \in I}, (E'_i)_{i \in I}, (F_\lambda)_{\lambda \in L}, (F'_\lambda)_{\lambda \in L}$为$A$模块的四个系列，并且对于每个$i \in I$（分别为每个$\lambda \in L$），$u_i : E'_i \to E_i$（分别为$v_\lambda : F_\lambda \to F'_\lambda$）线性映射。然后图表

$$
\begin{array}{ccc}
\operatorname{Hom}\left( \bigoplus_{i \in I} E'_i, \prod_{\lambda \in L} F'_\lambda \right) & \xrightarrow{\phi'} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E'_i, F'_\lambda) \\
\uparrow & & \uparrow \\
\operatorname{Hom}\left( \bigoplus_i u_i, \prod_\lambda v_\lambda \right) & & \prod \operatorname{Hom}(u_i, v_\lambda) \\
\operatorname{Hom}\left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) & \xrightarrow{\phi} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E_i, F_\lambda)
\end{array}
$$

（其中$\phi$和$\phi'$是推论1到命题6中定义的典范同构）是可交换的。

验证立即从定义开始。

当所有$E_i$等于同一个$A$模$E$时，直和$\bigoplus_{i \in I} E_i$也用$E^{(I)}$表示：其元素是$I$的映射转化为$E$ 有限支撑。如果对于所有$i$，$f_i$被取为恒等映射$E \to E$，通过命题6，得到线性映射$E^{(I)} \to E$，称为*对角线*，它与元素的每个家庭$(x_i)_{i \in I}$相关联$E$，有限支撑，它的*和* $\sum_{i \in I} x_i$。

#### 注 {#alg-ii-s1-n6-rem-1 .statement tag=05KD}

回想一下，直和扩展的定义立即到*群*的$(E_i)_{i \in I}$族，它们不一定是可交换的，乘法记号当然替换加法记号；然后我们说“*restricted 乘积*”或“*restricted 和*”而不是“*直和*”(I, § 4, no. 9)。

注，$E$是乘积$F = \prod_{i \in I} E_i$的*正常*子群，并且每个$j_k(E_k)$是$F$的*正常*子群；此外，对于两个不同的指标$\lambda, \mu$，$j_\lambda(E_\lambda)$的每一个元素与$j_\mu(E_\mu)$的每一个元素都是“可置换”的。 命题 6 扩展对于假设的一般情况，对于两个不同的指标 $\lambda, \mu$，$f_\lambda(E_\lambda)$的每一个元素在$M$中都是“可置换”的，每一个元素 $f_\mu(E_\mu)$（I, § 4, no. 9，命题12）。受限制的和的“*结合性*”的性质紧随其后。 命题 7 及其推论 1 和 2 无需修改就成立。

### 7. 交和和子模

对于$A$模块$E$的子模的每个族$(M_i)_{i \in I}$，交$\bigcap_{i \in I} E_i$是$E$的子模。如果，对于每个$i \in I$，$\phi_i$表示典范同态$E \to E/M_i$，$\bigcap_{i \in I} M_i$是$E$的同态$\phi : x \mapsto (\phi_i(x))$到$\prod_{i \in I} (E/M_i)$的*核*，在其他字中，有*正合序列*

$$
0 \longrightarrow \bigcap_{i \in I} M_i \longrightarrow E \xrightarrow{\phi} \prod_{i \in I} (E/M_i).
$$

线性映射 $\phi$ 和映射
$$
E / \left( \bigcap_{i \in I} M_i \right) \to \prod_{i \in I} (E / M_i)
$$
由经过求商得到的，称为规范的。

尤其：

#### 命题 8 {#alg-ii-s1-prop-8 .statement tag=05KE}

*如果一个家庭* $(M_i)_{i \in I}$ * of 子模 of* $E$ *将交简化为* $0$ *E 与* $\prod_{i \in I} (E / M_i)$ 的子模典型同构。

给定 $A$ 模块 $E$ 的子集 $X$，$E$ 包含 $X$ 的子模交 $F$ 被称为子模 *由 $X$ *生成*，并且$X$ 称为 $F$ (I, § 4, no. 3) 的 *生成的集合* (或 *生成的系统*)；对于$E$的元素的族$(a_i)_{i \in I}$，由$a_i$的集合生成的子模称为由$(a_i)$的族生成的子模。

如果 $A$ 模块具有*有限* 生成的集合，则称为“有限生成”。

#### 命题 9 {#alg-ii-s1-prop-9 .statement tag=05KF}

*The submodule generated by a family* $(a_i)_{i \in I}$ *of elements of an* $A$*-module* $E$ *is the set of linear combinations of the family* $(a_i)$.

$E$中的每个子模，其中包含所有$a_i$以及$a_i$中的包含线性组合。反过来，no. 1的公式（1）和（2）证明$a_i$的线性组合的集合是$E$的子模，显然包含所有$a_i$因此是最小的子模包含他们。

#### 推论 1 {#alg-ii-s1-prop-9-cor-1 .statement tag=05KG}

*设*$u : E \to F$*为*$E$*的线性映射、S子集和*$M$*子模*$E$*由*$S$生成。 *那么*$u(M)$*是*$F$*的子模*由*$u(S)$生成。

特别地，$E$的任意有限生成的子模在$u$下的像是$F$的有限生成的子模。

#### 注 {#alg-ii-s1-n7-rem-1 .statement tag=05KH}

如果$u(x) = 0$代表所有$x \in S$，那么$u(x) = 0$也代表所有$x \in M$。我们将有时将此结果称为“线性恒等式扩张的原理”*或“线性恒等式扩张的原理”*。

特别是，要验证线性映射$u : E \to F$是形式$v \circ \phi$，其中$v : E / M \to F$是线性的，$\phi : E \to E / M$是规范的投影，验证$u(S) = 0$就足够了。

#### 推论 2 {#alg-ii-s1-prop-9-cor-2 .statement tag=05KI}

*The submodule generated by the union of a family* $(M_i)_{i \in I}$ *of submodules of a module* $E$ *is identical with the set of sums* $\sum_{i \in I} x_i$, *where* $(x_i)_{i \in I}$ *runs through the set of families of elements of* $E$ *of finite support such that* $x_i \in M_i$ *for all* $i \in I$.

显然$\bigcup_{i \in I} M_i$的元素的每一个线性组合都是上面的形式； 逆命题是显而易见的。

The submodule of E generated by the union of a family $(M_i)_{i \in I}$ of submodules of E is called the *sum* of the family $(M_i)$ and is denoted by $\sum_{i \in I} M_i$.

如果对于所有$i \in I$，$h_i$是典范嵌入$M_i \to E$和$\bigoplus_{i \in I} M_i$的$h : (x_i) \mapsto \sum_i h_i(x_i)$线性映射到E相应的到家庭$(h_i)$（no. 6，命题6），$\sum_{i \in I} M_i$是$h$的*像*；在其他字中，有一个*正合序列*

$$
\bigoplus_{i \in I} M_i \xrightarrow{h} E \longrightarrow E / \left( \sum_{i \in I} M_i \right) \longrightarrow 0.
$$

#### 推论 3 {#alg-ii-s1-prop-9-cor-3 .statement tag=05KJ}

*如果* $(M_\lambda)_{\lambda \in L}$ *是A-模 E 的子模的右有向族，和* $\sum_{\lambda \in L} M_\lambda$ *与并* $\bigcup_{\lambda \in L} M_\lambda$相同。

$\bigcup_{\lambda \in L} M_\lambda \subset \sum_{\lambda \in L} M_\lambda$ *在没有假设的情况下始终为真；另一方面，对于每个有限子族* $(M_\lambda)_{\lambda \in J}$ *of* $(M_\lambda)_{\lambda \in L}$，*存在假设 a* $\mu \in L$ *使得* $M_\lambda \subset M_\mu$ *对于所有* $\lambda \in J$，*因此* $\sum_{\lambda \in L} M_\lambda \subset M_\mu$ *因此从推论2得出* $\sum_{\lambda \in L} M_\lambda \subset \bigcup_{\lambda \in L} M_\lambda$。

#### 推论 4 {#alg-ii-s1-prop-9-cor-4 .statement tag=05KK}

*设* $0 \to E \xrightarrow{f} F \xrightarrow{g} G \to 0$ *为A-模的正合序列，* E 的 S 生成的系统，* G 的 *T 生成的系统。 *如果 T' 为 F 的子集，则* $g(T') = T$，*T' \cup f(S) 为* F 的生成的系统。

由 T' \cup f(S) 包含 $f(E)$ 生成的 F 的子模 F' 以及$g(F')$ 包含 T、$g(F') = G$；因此$F' = F$。

#### 推论 5 {#alg-ii-s1-prop-9-cor-5 .statement tag=05KL}

*在正合序列* $0 \to E \to F \to G \to 0$ *A-模中，如果 E 和 G 是有限生成的，那么 F 也是有限生成的。*

#### 命题 10 {#alg-ii-s1-prop-10 .statement tag=05KM}

*设* M，N *为A-模 E 中的两个子模。则有两个正合序列*

$$
\begin{align*}
&0 \longrightarrow M \cap N \xrightarrow{u} M \oplus N \xrightarrow{i-j} M + N \longrightarrow 0 \\
&0 \longrightarrow E/(M \cap N) \xrightarrow{v} (E/M) \oplus (E/N) \xrightarrow{p-q} E/(M + N) \longrightarrow 0
\end{align*}
$$

*其中* $i : M \to M + N$, $j : N \to M + N$ *是典范嵌入,*
$$
p : E/M \to E/(M + N) \quad \text{and} \quad q : E/N \to E/(M + N)
$$

*典范满射，其中同态 u 和 v 定义如下：*

如果$f : M \cap N \to M \to M \oplus N$和$g : M \cap N \to N \to M \oplus N$是典范嵌入，$u = f + g$，并且如果$r : E/(M \cap N) \to E/M \to (E/M) \oplus (E/N)$和
$$
s : E/(M \cap N) \to E/N \to (E/M) \oplus (E/N)
$$
是典范映射，$v = r + s$。

我们证明(29)的正确性：显然$i - j$是满射的，$u$是单射的。另一方面，说$(i - j)(x, y) = 0$，其中$x \in M$和$y \in N$，意味着$i(x) - j(y) = 0$，因此$i(x) = j(y) = z \in M \cap N$，从而乘以定义$x = f(z), y = g(z)$，这证明了$\operatorname{Ker}(i - j) = \operatorname{Im} u$。

我们证明(30)的正确性：显然$p - q$是满射的。 另一方面，说 $t \in E/(M \cap N)$ 为 $v(t) = 0$ 意味着 $r(t) = s(t) = 0$，因此 $t$ 是类 mod。 元素 $z \in E$ 的 $(M \cap N)$ 其类 mod。 $M$ 和模组。 $N$是零，这意味着$z \in M \cap N$和$t = 0$。 最后说$(p - q)(x, y) = 0$，其中$x \in E/M, y \in E/N$意味着$p(x) = q(y)$，或者说$E$存在两个元素$z', z''$，其类模。 $M$ 和 mod。 $N$分别是$x$和$y$，且$z' - z'' \in M + N$。 因此有 $t' \in M, t'' \in N$ 使得 $z' - z'' = t' - t''$, 从而
$$
z' - t' = z'' - t'' = z.
$$
令 $w$ 为类 mod。 $z; r(w)$ 的$(M \cap N)$ 是类 mod。 $z$的$M$，因此还有$z'$的$x$；类似地，$s(w) = y$，它完成了证明那个$\operatorname{Ker}(p - q) = \operatorname{Im} v$。

### 8. 直和的子模

#### 定义 6 {#alg-ii-s1-def-6 .statement tag=05KN}

*A-模* $E$ *据说是一家人的直和* $(M_\iota)_{\iota \in I}$ *子模的* $E$ *如果典范映射* $\bigoplus_{\iota \in I} M_\iota \to E$ *(no. 6)* *就是同构*。

这相当于说每个$x \in E$都可以*以独特的方式*写成形式$x = \sum_{\iota \in I} x_\iota$，其中$x_\iota \in E_\iota$代表所有$\iota \in I$； 元素 $x_\iota$ 因此相应的到$x$被称为$E_\iota$中$x$的*分量*； 映射 $x \mapsto x_\iota$ 是*线性*。

#### 注 {#alg-ii-s1-n8-rem-1 .statement tag=05KO}

(1) 令$(M_\iota)_{\iota \in I}, (N_\iota)_{\iota \in I}$为模$E$的子模的两个族，具有相同的索引集合；假设$E$*同时*是$(M_\iota)$族和$(N_\iota)$族的直和，并且对于所有$\iota \in I$来说*那个*$N_\iota \subset M_\iota$。然后$N_\iota = M_\iota$*对于所有*$\iota \in I$，如下所示，立即从no. 6开始，推论1到命题7应用于典范嵌入$f_\iota : N_\iota \to M_\iota$。

#### 命题 11 {#alg-ii-s1-prop-11 .statement tag=05KP}

*让*$(M_\iota)_{\iota \in I}$*成为A-模*$E$的子模家庭。 *以下属性是等效的*：

(a) *子模* $\sum_{\iota \in I} M_\iota$ *是家庭的直和* $(M_\iota)_{\iota \in I}$。

(b) *关系* $\sum_{i \in I} x_i = 0$，*其中* $x_i \in M_i$ *对于所有* $i \in I$，*意味着* $x_i = 0$ *对于所有* $i \in I$。

(c) *For all* $\kappa \in I$, *the intersection of* $M_\kappa$ *and* $\sum_{i \neq \kappa} M_i$ *reduces to* 0.

(a) 和 (b) 等价的是直接的，因为关系 $\sum_i x_i = \sum_i y_i$ 等价于 $\sum_i (x_i - y_i) = 0$。另一方面，根据定义6，(a)通过将$\bigoplus_{i \in I} M_i$的元素的表达式唯一性隐含为元素$x_i \in M_i$的直和。最后，关系$\sum_i x_i = 0$，其中$x_i \in M_i$对于所有$i$，可以写成，对于所有$\kappa \in I$，$x_\kappa = \sum_{i \neq \kappa} (-x_i)$； 条件 (c) 那么对于所有 $\kappa \in I$ 意味着 $x_\kappa = 0$，因此 (c) 意味着 (b)。

#### 定义 7 {#alg-ii-s1-def-7 .statement tag=05KQ}

* A-模 E 的自同态 e 称为投影算子 if* $e \circ e = e$ *（在其他字中，如果 e 在环 End(E) 中是幂等的）。在* $\operatorname{End}(E)$ *family* $(e_\lambda)_{\lambda \in L}$ *of 投影算子中，如果* $e_\lambda \circ e_\mu = 0$ *对于* $\lambda \neq \mu$ 则称为正交。

#### 命题 12 {#alg-ii-s1-prop-12 .statement tag=05KR}

*设E为A-模。*

(i) *如果 E 是直和族* $(M_\lambda)_{\lambda \in L}$ *的子模，且对于所有* $x \in E$、$e_\lambda(x)$ *是 x 的分量* $M_\lambda$、$(e_\lambda)$ *是投影算子的正交族，使得* $x = \sum_{\lambda \in L} e_\lambda(x)$ *对于所有* $x \in E$。

(ii) *相反，如果* $(e_\lambda)_{\lambda \in L}$ *是$\operatorname{End}(E)$中投影算子的正交族，使得* $x = \sum_{\lambda \in L} e_\lambda(x)$ *对于所有* $x \in E$，*E是子模* $M_\lambda = e_\lambda(E)$族的直和。

性质 (i) 由定义推出，(ii) 是no. 6的特例，推论2至命题 6，适用于典范嵌入 $M_\lambda \to E$ 和映射 $e_\lambda : E \to M_\lambda$。

注当 L 有限时条件 $x = \sum_{\lambda \in L} e_\lambda(x)$ 对于所有 $x \in E$ 也可以写成$\operatorname{End}(E)$。

(31)
$$
1_E = \sum_{\lambda \in L} e_\lambda.
$$

#### 推论{#alg-ii-s1-n8-cor-1 .statement tag=05KS}

*对于E的每个投影算子 e，E是e的像*$M = e(E)$*和核*$N = e^{-1}(0)$*的直和；对于所有* $x = x_1 + x_2 \in E$ *与* $x_1 \in M$ *和* $x_2 \in N$、$x_1 = e(x)$； *1 − e 是像 N 和核 M* 的 E 的投影算子。

$(1 - e)^2 = 1 - 2e + e^2 = 1 - e$ *在* $\operatorname{End}(E)$ *因此* $1 - e$ *是投影算子；同样* $e(1 - e) = (1 - e)e = e - e^2 = 0$，*E 是像* $M$ *的直和和* $N$ *e 和* $1 - e$ *通过命题 12。最后，对于所有* $x \in E$，*关系* $x \in M$ * 是等价的至* $x = e(x)$； *对于* $x = e(x)$ *意味着定义* $x \in M$ *并且相反，如果* $x = e(x')$ *与* $x' \in E$，*则* $e(x) = e^2(x') = e(x') = x;$

因此，这表明M是$1 - e$的核，并且交换$e$和$1 - e$的角色，类似地可以看出N是$e$的核。

#### 注 {#alg-ii-s1-n8-rem-2 .statement tag=05KT}

(2) 令E、F为两个A-模，使得E是子模的有限族$(M_i)_{1 \leq i \leq m}$的直和，并且F直和属于子模的有限族$(N_j)_{1 \leq j \leq n}$。然后可知（no. 6，推论 1 到命题 6）$\mathrm{Hom}_A(E, F)$ 与乘积 $\prod_{i,j} \mathrm{Hom}_A(M_i, N_j)$ 被规范地识别；准确地说，对于一个家庭$(u_{ji})$，其中$u_{ji} \in \mathrm{Hom}_A(M_i, N_j)$还有对应线性映射$u : E \to F$定义如下。 $u$中的定义限制足以满足每个$M_i$和每个$x_i \in M_i$，
$$
u(x_i) = \sum_{j=1}^n u_{ji}(x_i).
$$
现在让 G 为子模的有限族 $(P_k)_{1 \leq k \leq p}$ 的第三个A-模、直和；令$v$为F到G的线性映射，并让$(v_{kj}) \in \prod_{j,k} \mathrm{Hom}_A(N_j, P_k)$规范地为它的相应的族。对于所有$x_i \in M_i$，
$$
v(u(x_i)) = \sum_{j=1}^n v(u_{ji}(x_i)) = \sum_{k=1}^p \sum_{j=1}^n v_{kj}(u_{ji}(x_i)).
$$
由此可见，如果我们写
$$
w_{ki} = \sum_{j=1}^n v_{kj} \circ u_{ji} \in \mathrm{Hom}_A(M_i, P_k)
$$
族$(w_{ki})$对应规范地从E到G（cf.§ 10, no. 5）合成线性映射$w = v \circ u$。

### 9.补子模

#### 定义 8 {#alg-ii-s1-def-8 .statement tag=05KU}

在A-模E中，如果E是$M_1$和$M_2$的直和，则两个子模$M_1, M_2$被称为补充。

no. 8的命题11表明，$M_1$和$M_2$互补，$M_1 + M_2 = E$和$M_1 \cap M_2 = \{0\}$（cf.I, § 4, no. 9，命题15）是充分必要的。

#### 命题 13 {#alg-ii-s1-prop-13 .statement tag=05KV}

令$M_1, M_2$为A-模E中的两个补子模。典范映射$E \to E/M_2$的限制到$M_1$是$M_1$到$E/M_2$的同构。

这个线性映射从$M_1 + M_2 = E$开始就是满射，并且它是单射的，因为它的核是$M_1$的交和$E \to E/M_2$的核$M_2$，因此约化到$\{0\}$。

#### 推论{#alg-ii-s1-n9-cor-1 .statement tag=05KW}

如果$M_2$和$M_2'$是E的相同子模$M_1$、有序对$(x, x') \in M_2 \times M_2'$的集合的两个补充，则$x - x' \in M_1$是$M_2$的同构的图$M_2'$。

它是同构$M_2 \to E/M_1 \to M'_2$的合成图，即直接的。

#### 定义 9 {#alg-ii-s1-def-9 .statement tag=05KX}

*如果$E$中有补子模，则$A$模块$E$的子模$M$称为$E$的直因子。*

当这样时，$E/M$同构于$M$（命题13）的补充。

子模不一定承认补充（习题11）。当子模为直因子时，一般有几个不同的补充；然而，这些补充在规范上与另一个同构（命题13的推论）。

#### 命题 14 {#alg-ii-s1-prop-14 .statement tag=05KY}

*为了使模$E$的子模$M$成为直因子，只要存在$E$的投影算子且像为$M$或投影算子即可。 $E$，其核为 $M$。*

这紧随no. 8、命题 12 和推论。

#### 命题 15 {#alg-ii-s1-prop-15 .statement tag=05KZ}

*给定 $A$ 模块中的正合序列*
$$
(33)\quad 0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$
*以下命题等效：*
(a) *$F$中的子模$f(E)$为直因子。*
(b) *存在与$f$相关的线性回缩$r : F \to E$（集合理论，II, § 3, no. 8，定义11）。*
(c) *存在与$g$相关的线性截面$s : G \to F$（集合理论，II, § 3, no. 8，定义11）。*
*这样的话，$f + s : E \oplus G \to F$就是同构。*

如果$\mathrm{End}(F)$中存在投影算子$e$，使得$e(F) = f(E)$、同态$f^{-1} \circ e : F \to E$是与$f$相关的线性回缩；反之，如果存在这样的收缩$r$，则$f \circ r$在$F$中投影算子是直接的，而像是$f(E)$，因此(a)和(b)是等价的(命题14)。如果$f(E)$在$F$中承认补充$E'$且$j : E' \to F$是典范嵌入，则$g \circ j$是$E'$的同构到$G$和逆同构，视为$G$到$F$的映射，是与$g$相关的线性截面。相反，如果存在这样的截面$s$，则$F$中$s \circ g$是投影算子，而核是$f(E)$，因此(a)和(c)是等价的(命题14)。此外，$s$是$G$到$s(G)$的双射，并且由于$s(G)$是$f(E)$的补充，所以$f + s$是同构。

注，被给予$r$（或$s$）相当于在$F$中被给予$f(E)$的补充，即$r$的核（或$s$的像）。

当正合序列(33)满足命题15的条件时，可以说*分裂的*或$(F, f, g)$被认为是$G$的*平凡*扩张乘以$E$(I, § 6, no. 1)。

#### 推论 1 {#alg-ii-s1-prop-15-cor-1 .statement tag=05L0}

设$u : E \to F$为线性映射。对于存在线性映射$v : F \to E$使得$u \circ v = 1_F$（$u$被称为右可逆且$v$被称为$u$的右逆），$u$是满射且其核是充分必要的直因子 $E$。 $E$的子模$\operatorname{Im}(v)$则为$\operatorname{Ker}(u)$的补充。

显然 $u$ 是满射的；由于 $v$ 是截面与 $u$ 相关联，因此结论是从命题 15 得出的。

#### 推论 2 {#alg-ii-s1-prop-15-cor-2 .statement tag=05L1}

设$u : E \to F$为线性映射。对于存在线性映射$v : F \to E$使得$v \circ u = 1_E$（$u$被称为左可逆且$v$被称为$u$的左逆的情况），$u$是内射的并且其像是必要且充分的$F$ 中的直因子。 $F$的子模$\operatorname{Ker}(v)$则为$\operatorname{Im}(u)$的补充。

显然$u$是单射的；由于$v$是与$u$相关的撤回，因此结论也可以从命题15得出。

#### 注 {#alg-ii-s1-n9-rem-1 .statement tag=05L2}

(1) Let $M, N$ be two supplementary submodules in an $A$-module $E$, $p, q$ the projectors of $E$ onto $M$ and $N$ respectively, corresponding to the decomposition of $E$ as a direct sum of $M$ and $N$. 已知（no. 6，推论 1 到命题 6），对于每个 $A$-模块 $F$，映射 $(u, v) \mapsto u \circ p + v \circ q$ 是同构
$$
\operatorname{Hom}_A(M, F) \oplus \operatorname{Hom}_A(N, F)
$$
到$\operatorname{Hom}_A(E, F)$。 在这个同构下，$\operatorname{Hom}_A(M, F)$的像是线性映射$w : E \to F$的集合，这样对于所有$x \in N$来说$w(x) = 0$。

(2) If $M, N$ are two submodules of $E$ such that $M \cap N$ is a direct factor of $M$ and $N$, then $M \cap N$ is also a direct factor of $M + N$: if $P$ (resp. $Q$) is a supplement of $M \cap N$ in $M$ (resp. $N$), $M + N$ is the direct sum of $M \cap N, P$ and $Q$, as is immediately verified.

### 10. 模的有限长度

回想一下（I, § 4, no. 4，定义 7），如果$A$-模块$M$没有减少到0，并且包含没有子模与$M$和$\{0\}$不同，则称其为简单模块。如果一个$A$-模$M$有一个Jordan-Hölder级数$(M_i)_{0 \leq i \leq n}$和数$n$这个级数的商（不依赖于Jordan-Hölder级数），则称其为有限长度。考虑$M$）则称为$M$（I, § 4, no. 7，定义 11）的长度；我们用$\operatorname{long}(M)$或$\operatorname{long}_A(M)$来表示。 $A$-模减少到 0 是长度 0；如果$M$是有限长度的非零$A$模，则$\operatorname{long}(M) > 0$。

#### 命题 16 {#alg-ii-s1-prop-16 .statement tag=05L3}

Let $M$ be an $A$-module and $N$ a submodule of $M$; for $M$ to be of finite length, it is necessary and sufficient that $N$ and $M/N$ be so, and then
$$
\operatorname{long}(N) + \operatorname{long}(M/N) = \operatorname{long}(M).
$$
The proof has been given in I, § 4, no. 7, Proposition 10.

#### 推论 1 {#alg-ii-s1-prop-16-cor-1 .statement tag=05L4}

令$M$为有限长度的$A$模；为了使$M$的子模$N$等于$M$，$\operatorname{long}(N) = \operatorname{long}(M)$是充分必要的。

#### 推论 2 {#alg-ii-s1-prop-16-cor-2 .statement tag=05L5}

令$u : M \to N$为$A$模块同态。如果$M$或$N$是有限长度，那么$\operatorname{Im}(u)$也是。如果 $M$ 为有限长度，则 $\operatorname{Ker}(u)$ 也为有限长度，并且
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Ker}(u)) = \operatorname{long}(M).
$$
如果 $N$ 为有限长度，则 $\operatorname{Coker}(u)$ 也为有限长度，并且
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Coker}(u)) = \operatorname{long}(N).
$$

#### 推论 3 {#alg-ii-s1-prop-16-cor-3 .statement tag=05L6}

令 $(M_i)_{0 \leq i \leq n}$ 为 $A$ 有限长度模的有限族。如果存在线性映射中的正合序列
$$
0 \longrightarrow M_0 \xrightarrow{u_0} M_1 \xrightarrow{u_1} M_2 \longrightarrow \cdots \longrightarrow M_{n-1} \xrightarrow{u_{n-1}} M_n \longrightarrow 0
$$
然后
$$
\sum_{k=0}^n (-1)^k \operatorname{long}(M_k) = 0.
$$
对于$n = 1$，推论是显而易见的，对于$n = 2$，推论只是命题 16；我们在归纳关于$n$争论。如果$M'_{n-1} = \operatorname{Im}(u_{n-2})$，则乘以归纳假设，
$$
\sum_{k=0}^{n-2} (-1)^k \operatorname{long}(M_k) + (-1)^{n-1} \operatorname{long}(M'_{n-1}) = 0.
$$
另一方面，正合序列$0 \to M'_{n-1} \to M_{n-1} \to M_n \to 0$给出
$$
\operatorname{long}(M'_{n-1}) + \operatorname{long}(M_n) = \operatorname{long}(M_{n-1}),
$$
从而关系 (38)。

#### 推论 4 {#alg-ii-s1-prop-16-cor-4 .statement tag=05L7}

令$M$和$N$为$A$模块$E$的有限长度中的两个子模；那么 $M + N$ 是有限长度并且
$$
\operatorname{long}(M + N) + \operatorname{long}(M \cap N) = \operatorname{long}(M) + \operatorname{long}(N).
$$
将推论3应用到正合序列(29)(no. 7)就足够了。
$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$
利用 $\operatorname{long}(M \oplus N) = \operatorname{long}(M) + \operatorname{long}(N)$ 乘以 (34) 的事实。

#### 推论 5 {#alg-ii-s1-prop-16-cor-5 .statement tag=05L8}

令$M$为有限长度的子模族$(N_i)$的$A$模块和。那么 $M$ 是有限长度并且
$$
\operatorname{long}(M) \leq \sum_i \operatorname{long}(N_i).
$$

此外，为了使(40)的两侧相等，M是$N_i$的直和是必要且充分的。

已经看出(no. 7,公式(28))存在一个规范满射线性映射$h : \bigoplus_i N_i \to M$；因此，推论由（35）得出。

#### 推论 6 {#alg-ii-s1-prop-16-cor-6 .statement tag=05L9}

*设M和N是A-模E中的两个子模，使得E/M和E/N是有限长度中的模；那么 E/(M \cap N) 是有限长度并且*

$$
\text{(41)} \quad \text{long}(E/(M \cap N)) + \text{long}(E/(M + N)) = \text{long}(E/M) + \text{long}(E/N).
$$

只需将推论 3 应用到正合序列 (30)

$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$

利用这一事实

$$
\text{long}((E/M) \oplus (E/N)) = \text{long}(E/M) + \text{long}(E/N).
$$

#### 推论 7 {#alg-ii-s1-prop-16-cor-7 .statement tag=05LA}

*令$(M_i)$为A-模E的子模的有限族，使得$E/M_i$为有限长度的模。那么 $E/(\bigcap_i M_i)$ 是有限长度并且*

$$
\text{(42)} \quad \text{long}\left(E/(\bigcap_i M_i)\right) \leq \sum_i \text{long}(E/M_i).
$$

已经看出(公式(27))存在一个规范单射线性映射$E/(\bigcap_i M_i) \to \bigoplus_i (E/M_i)$。

#### 注 {#alg-ii-s1-n10-rem-1 .statement tag=05LB}

除了 no. 7、命题 9 之外，*所有* 的结果。 2 到 10 对于任意 *可交换群与运算符*、子模（分别为商模）在叙述中被稳定的子群（分别为商群被稳定的子群）替换是有效的；我们还约定用运算符“线性映射”调用群的同态。 no. 7、命题 9 的推论对于带有运算符的交换群也有效：这对于推论 4 和 5 以及推论 2 来说都是显而易见的，因为对于每个运算符 $\alpha$ 都有 $\alpha \left( \sum_{i \in I} x_i \right) = \sum_{i \in I} \alpha x_i$，并且推论 3 由此推出。对于推论 1，只要注如果 N 是 F 包含 $u(S)$ 的稳定子群，$u^{-1}(N)$ 是 E 包含 S 的稳定子群，因此$u^{-1}(N)$ 包含 M，因此$u(M) \subset N$。

### 11.免费的家庭。 基

令 A 为环，T 集合并考虑 A-模 $A_s^{(T)}$。通过定义，它是A-模的家庭$(M_t)_{t \in T}$的外部直和，全部等于$A_s$，并且对于所有$t \in T$，有典范嵌入$j_t : A_s \to A_s^{(T)}$（no. 6）。我们写j_t(1) = e_t，这样$e_t = (\delta_{tt'})_{t' \in T}$，其中如果$t' \neq t$则$\delta_{tt'}$等于0，如果$t' = t$则等于1（“克罗内克符号”；$(t, t') \mapsto \delta_{tt'}$只是$T \times T$对角线的特征函数）；每个 $x = (\xi_t)_{t \in T} \in A_s^{(T)}$ 都可以被唯一地写成：
$$
x = \sum_{t \in T} \xi_t e_t.
$$
$T$到$A_s^{(T)}$的映射$\phi : t \mapsto e_t$称为规范；如果 $A$ 非零，则它是单射的。我们将看到有序对$(A_s^{(T)}, \phi)$是普遍映射问题的解（集合理论，IV, § 3, no. 1）。

#### 命题 17 {#alg-ii-s1-prop-17 .statement tag=05LC}

*对于每个 A-模 E 和每个映射 $f : T \to E$，存在且仅有一个 A-线性映射 $g : A_s^{(T)} \to E$ 使得 $f = g \circ \phi$。*

条件 $f = g \circ \phi$ 意味着$g(e_t) = f(t)$ 对于所有$t \in T$，相当于对于所有$\xi \in A$ 和所有$t \in T$ 的$g(\xi e_t) = \xi f(t)$，也意味着$g \circ j_t$ 是线性映射 $\xi \mapsto \xi f(t)$将所有 $t \in T$ 的 $A_s$ 转换为 $E$；因此，命题是no. 6、命题 6 的特例。

线性映射$g$据说是由$E$的元素的$(f(t))_{t \in T}$家族“决定”；通过定义
$$
g\left( \sum_{t \in T} \xi_t e_t \right) = \sum_{t \in T} \xi_t f(t).
$$

The kernel $R$ of $g$ is the set of $(\xi_t) \in A_s^{(T)}$ such that $\sum_t \xi_t f(t) = 0$; it is sometimes said that the module $R$ is *the module of linear relations between the elements of the family* $(f(t))_{t \in T}$. 正合序列
$$
0 \longrightarrow R \longrightarrow A_s^{(T)} \overset{g}{\longrightarrow} E
$$
据说是由家庭$(f(t))_{t \in T}$“决定”。

#### 推论 1 {#alg-ii-s1-prop-17-cor-1 .statement tag=05LD}

*令$T, T'$为两个集合、$g : T \to T'$映射。那么存在且仅有一个 A-线性映射 $f : A^{(T)} \to A^{(T')}$ 呈现可交换的图表*
$$
\begin{array}{ccc}
T & \overset{g}{\longrightarrow} & T' \\
\downarrow \phi & & \downarrow \phi' \\
A^{(T)} & \overset{f}{\longrightarrow} & A^{(T')}
\end{array}
$$
*其中$\phi$和$\phi'$是典范映射。*

应用命题 17 足以合成映射 $T \overset{g}{\to} T' \overset{\phi'}{\to} A^{(T')}$。

#### 推论 2 {#alg-ii-s1-prop-17-cor-2 .statement tag=05LE}

*对于A-模 E 的元素的族$(a_t)_{t \in T}$成为E的生成的系统，由该族确定的线性映射$A_s^{(T)} \to E$是满射的充分必要*。

这只是另一个表达no. 7的命题9的方式。

#### 定义 10 {#alg-ii-s1-def-10 .statement tag=05LF}

* $\mathbf{A}$*-模块* $E$ *的$(a_t)_{t \in T}$ * 元素 *被称为自由族*（分别是。 *基 of* $E$) *如果线性映射* $A_s^{(T)} \to E$ *由该族确定是单射*（分别是 *双射的*）。 *如果有基*，则称模为自由。

特别是，如果 $G$（相加地写）是一个 *自由* $\mathbf{Z}$*-模块* (cf. I, § 7, no. 7)，则可交换的群 $G$ 被称为 *自由*。

定义 10 与推论 2 到命题 17 一起表明，$\mathbf{A}$-模块$E$ 的基是$E$ 的*自由生成的系列*。因此，$E$的元素的每个自由族都是子模和生成的基。

到定义时，$\mathbf{A}$ 模块 $A_s^{(T)}$ 是免费的，$(e_t)_{t \in T}$ 系列是该 $\mathbf{A}$ 模块的基（称为*规范*）。当$\mathbf{A} \neq \{0\}$、$T$经常被规范的双射$t \mapsto e_t$等同于$e_t$的集合；这相当于将 $A_s^{(T)}$ 的元素写为 $\sum_{t \in T} \xi_t \cdot t$ 而不是 $\sum_{t \in T} \xi_t a_t$。当采用这个约定时，$A_s^{(T)}$的元素被称为*正式的线性组合*（系数在$\mathbf{A}$）*元素的*$T$。

定义 10 和命题 17 立即给出以下结果：

#### 推论 3 {#alg-ii-s1-def-10-cor-3 .statement tag=05LG}

*让*$E$*成为*$E$、$F$*一个*$\mathbf{A}$*-模块的自由*$\mathbf{A}$*-模块*、$(a_t)_{t \in T}$*基和*$(b_t)_{t \in T}$*$F$的元素家族。 *存在且仅有一个线性映射* $f : E \to F$ *这样*
$$
f(a_t) = b_t \quad \text{for all } t \in T.
$$
*对于* $f$ *成为单射*（或*满射*），*必要且充分的是* $(b_t)$ *成为* $F$（或* $F$的*生成的系统）中的自由家庭。

当一个家庭$(a_t)_{t \in T}$不自由时，它被称为*相关*。 定义 10 也可以表达如下：说$(a_t)_{t \in T}$是*自由的*意味着关系$\sum_{t \in T} \lambda_t a_t = 0$（其中$(\lambda_t)$属于有限支撑）意味着$\lambda_t = 0$对于所有$t \in T$；说$(a_t)_{t \in T}$是$E$的*基*，意味着每个$x \in E$在形式$x = \sum_{t \in T} \xi_t a_t$中都可以用一种且只有一种方式写出来；对于所有 $t \in T$，$\xi_t$ 被称为指标* $t$ *相对于基* $(a_t)$ 的*$x$ *的*分量*（或*坐标*）； 映射 $x \to \xi_t$ 从 $E$ 到 $A_s$ 是*线性*。

假设$\mathbf{A} \neq \{0\}$；那么，在一个$\mathbf{A}$-模块$E$中，一个自由族$(a_t)_{t \in T}$的两个元素其指标是不同的，它们本身是*不同的*：因为如果$a_{t'} = a_{t''}$对于$t' \neq t''$，则$\sum_{t \in T} \lambda_t a_t = 0$与$\lambda_{t'} = 1$，$\lambda_{t''} = -1$和$T$ 的元素的$\lambda_t = 0$ 与$t'$ 和$t''$ 不同。 如果 $S$ 的恒等映射定义的族本身是自由的（分别是 $E$ 的基），则 $E$ 的子集 $S$ 将被称为 *自由子集* （分别是 $E$ 的 *基*）；然后，由索引集合到$S$ 的双射映射定义的每个族都是自由的（分别是基）。 $E$ 的自由子集的元素也称为“线性无关”。

如果 E 的子集不是自由的，则称为相关或相关的系统及其元素称为线性相关。

免费的子集的每一个子集都是免费的；特别地，空的子集是自由的，并且是E的子模{0}的基。

#### 命题 18 {#alg-ii-s1-prop-18 .statement tag=05LH}

*要使模 E 的族 $(a_t)_{t \in T}$ 自由，$(a_t)_{t \in T}$ 的每个有限子族都是自由的。*

这立即从定义开始。

命题 18 表明 E 的自由子集按包含排序，集合是归纳的（*集合理论*，III, § 2, no. 4）；因为它是非空的（因为$\varnothing$属于），所以它有极大元素$(a_l)_{l \in I}$（Zorn的引理）。由此得出（如果$A \neq \{0\}$）对于所有$x \in E$，存在A的元素$\mu \neq 0$和元素A的族$(\xi_l)$，使得$\mu x = \sum_l \xi_l a_l$（cf.§ 7, no. 1）。

#### 命题 19 {#alg-ii-s1-prop-19 .statement tag=05LI}

*设E为子模的$(M_\lambda)_{\lambda \in L}$族的A-模、直和。如果对于每个 $\lambda \in L$，$S_\lambda$ 是 $M_\lambda$ 的自由子集（分别是生成的集合、基），则 $S = \bigcup_{\lambda \in L} S_\lambda$ 是自由子集（分别是生成的） E.* 的集合、基)

命题源自定义和关系 $A_s^{(S)} = \bigoplus_{\lambda \in L} A_s^{(S_\lambda)}$（直和、cf. no. 6 的结合性）。

#### 注 {#alg-ii-s1-n11-rem-1 .statement tag=05LJ}

(1) 到定义 10，如果$A \neq \{0\}$和$(a_l)_{l \in I}$是自由族，元素$a_\kappa$不能等于指标$l \neq \kappa$的$a_l$中的线性组合。但反过来说，一个家庭$(a_l)$满足这个条件不一定是一个自由的家庭。对于例，令A为整环和$a, b$两个不同的非零元素；在 A 中，自 $(-b)a + ab = 0$ 起，被视为 A-模、$a$ 和 $b$ 形式相关的系统。但一般来说，不存在元素$x \in A$使得$b = xa$的$a = xb$（cf.然而§ 7, no. 1，*注*）。

如果$\{x\}$是一个自由的子集，模E的元素$x$被称为*自由*，也就是说，如果关系$\alpha x = 0$蕴涵$\alpha = 0$。免费子集中的每个元素都是免费的，特别是 0 不能属于到 $A \neq \{0\}$ 时的任何免费子集。

#### 注 {#alg-ii-s1-n11-rem-2 .statement tag=05LK}

(2) 自由模可以有元素$\neq 0$，但例、A-模$A_s$是免费的，但A中零的右除子不是免费的$A_s$的元素。

(3) 在加法群 $\mathbf{Z}/(n)$ ($n$ 整数 $\geq 2$) 被视为 $\mathbf{Z}$ 模块时，没有元素是空闲的，并且 *更不必说* $\mathbf{Z}/(n)$ 不是自由模。

(4) 可能会出现 A-模中的每一个元素 $\neq 0$ 都是空闲的，而模都是空闲的。对于例，有理数的域 $\mathbf{Q}$ 是一个$\mathbf{Z}$ 模块，与此性质，对于 $\mathbf{Q}$ 的两个元素 $\neq 0$ 总是形式相关因此，$\mathbf{Q}$的系统和基只能是包含单个元素$a$；但$\mathbf{Q}$的元素不是形式$na$和$n \in \mathbf{Z}$的全部（cf.VII, § 3）。

#### 命题 20 {#alg-ii-s1-prop-20 .statement tag=05LL}

*每个 A-模 E 都同构于自由A-模的商模。*

如果T是E的生成的集合，则存在满射线性映射$A_s^{(T)} \to E$（推论2到命题17），并且如果R是这个映射的核，则E同构于$A_s^{(T)}/R$。

特别是我们可以取$T = E$；然后有一个满射线性映射$A_s^{(E)} \to E$，称为*规范*。

特别是，说 A-模 E 是*有限生成* (no. 7) 意味着它同构于自由A-模与*有限基* 的商，或者还存在形式的正合序列

$$
A_s^n \to E \to 0 \quad (n \text{ an integer } > 0).
$$

注，如果$A \neq \{0\}$*有限生成*自由模E的每个基必然是*有限*，因为如果S是有限生成系统并且B基是E，则S的每个元素是B 的元素的有限数的线性组合，如果 B' 是 B 的所有元素的集合，因此在 S 的元素的表达式中，B' 是有限的，并且每个 $x \in E$ 是 的线性组合 B' 的元素，因此$B' = B$。

#### 命题 21 {#alg-ii-s1-prop-21 .statement tag=05LM}

*每正合序列共A-模*

$$
0 \longrightarrow G \xrightarrow{g} E \xrightarrow{f} F \longrightarrow 0
$$

*其中F为自由A-模、分裂的* (no. 9)。 *准确地说，如果*$(b_\lambda)_{\lambda \in L}$*是F的基，并且对于每个*$\lambda \in L$、$a_\lambda$*是E的元素，使得*$f(a_\lambda) = b_\lambda$、*家庭*$(a_\lambda)_{\lambda \in L}$*是免费的并且生成补子模至 g(G)*。

存在且仅有一个线性映射 $h : F \to E$，使得 $h(b_\lambda) = a_\lambda$ 对于所有 $\lambda \in L$（推论 3 到命题 17）。由于 h 是与 f 相关的线性截面，因此从 I, § 4, no. 9、命题 15 得出命题。

#### 注 {#alg-ii-s1-n11-rem-3 .statement tag=05LN}

(5) 令$(a_i)_{1 \leq i \leq n}$为A-模E的*基*，并令$(b_i)_{1 \leq i \leq n}$为由关系给出的E的元素族

$$
b_i = \lambda_{1i} a_1 + \cdots + \lambda_{ii} a_i \quad (1 \leq i \leq n)
$$

其中 $\lambda_{ii}$ 在 A 中是“可逆的”；那么$(b_i)_{1 \leq i \leq n}$是E的*基*。用归纳论证$n$就足够了，命题对于$n = 1$来说是显而易见的。如果E'是$(a_i)_{1 \leq i \leq n-1}$族生成的E的子模，则从归纳假设可以得出$(b_i)_{1 \leq i \leq n-1}$是E'的基；另一方面，从 (46) 可以得出，如果 $\mu b_n \in E'$ 与 $\mu \in A$，则还有 $\mu \lambda_{nn} a_n \in E'$、从而 $\mu = 0$，因为 $\lambda_{nn}$ 是可逆的。因此，$(b_i)_{1 \leq i \leq n}$家庭是自由的，并且，
$$
a_n = -\lambda_{nn}^{-1}\lambda_{1n}a_1 - \cdots - \lambda_{nn}^{-1}\lambda_{n-1,n}a_{n-1} + \lambda_{nn}^{-1}b_n
$$
可以看出，$(b_i)_{1 \leq i \leq n}$是E的生成的系统，从而完成证明。这个结果很容易推广到索引集合 I 有序的族$(a_i)_{i \in I}$。

### 12.湮没子。忠实的模。单源模

#### 定义 11 {#alg-ii-s1-def-11 .statement tag=05LO}

*A-模 E 的子集 S 的湮没子是元素 $\alpha \in A$ 的集合，使得$\alpha x = 0$ 对于所有$x \in S$。*

S的湮没子通常记为Ann(S)；对于单个元素 x 的子集 S 由……组成，我们写 Ann(x) 而不是 Ann(\{x\}) 并调用 x* 的 Ann(x) *湮没子。

关系$\alpha x = 0$也可以用说来表示*x被$\alpha$*消灭。

E 的任意子集 S 的湮没子是 A 的*左理想*，即直接的；要使其等于 A，$S = \{0\}$ 是必要且充分的（凭借 (M_IV)）。如果E的两个子集S，T使得T的$S \subset T$，湮没子包含在S的湮没子中。如果$(S_i)_{i \in I}$是E的子集的任意族，则并$\bigcup_i S_i$的湮没子是交 $S_i$ 的湮没子。特别地，E的子集S湮没子是S的元素湮没子交。说E的元素是*自由*相当于其湮没子是$\{0\}$的说。对于所有$x \in E$和所有$\alpha \in A$，$\alpha x$的湮没子是$\beta \in A$的集合，使得$\beta \alpha \in \mathrm{Ann}(x)$。

E 的 *子模* M 的湮没子是 A 的*双边理想*；因为，如果$\alpha x = 0$对于所有$x \in M$，那么$\alpha (\beta x) = 0$对于所有$x \in M$和所有$\beta \in A$，因此对于所有$\beta \in A$，M的$\alpha \beta$属于到湮没子。特别是，E 的湮没子是 A 的双面理想。

对于所有$\alpha \in A$，令$h_\alpha$为位似$x \mapsto \alpha x$；已知将 A 的映射 $\alpha \mapsto h_\alpha$ 转换为可交换的群（无运算符）E 的自同态环 $\mathscr{E} = \mathrm{Hom}_\mathbf{Z}(E, E)$，是 *环同态* (§ 2, no. 5)。这个同态下0的逆像就是E的*湮没子*$a$；因此，A 在同态 $\alpha \mapsto h_\alpha$ 下的像与商环 $A/a$ 同构的。如果湮没子 $a$ 约化为 0，则模 E 被称为“忠实”。

令E为任意A-模，$a$包含在Ann(E)中的A的双面理想，并令$\dot{\alpha}$为商环$A/a$的元素；对于所有$x \in E$，元素$\alpha x$对于所有$\alpha \in A$属于到类$\dot{\alpha}$模组都是相同的。 $a$;如果这个元素用$\dot{\alpha} x$表示，那么立即可以看出映射（α，x）↦αx定义（E上有加法）E上的（A/α）-模结构。当α = Ann（E）时，如此定义的（A/α）-模E是*忠实的*；我们可以说，它是与 A-模 E *关联的忠实模。请观察，A-模 E 的每个子模也是关联忠实模的子模，反之亦然。

#### 定义 12 {#alg-ii-s1-def-12 .statement tag=05LP}

*如果模是由单个元素生成的，则称为单生的。*

no. 7的命题 9表明，如果E是单生A-模并且a是元素生成的E，则E与ψa的集合A.a相同，其中ψ贯穿A。

#### 例 {#alg-ii-s1-n12-exa-1 .statement tag=05LQ}

(1) 每个单生群，可交换 (I, § 4, no. 10, 命题 18)，都是单生 $\mathbf{Z}$ 模。
(2) 如果A是交换环，A-模A的单生子模就是环A的*主理想*(I, § 8, no. 6)。
(3) 每个*简单* A-模 E 都是单生的，因为由 E 的元素 ≠ 0 生成的 E 的子模必然等于 E。

#### 命题 22 {#alg-ii-s1-prop-22 .statement tag=05LR}

*设A为环。 $A_s$ 的每个商模都是单生的。相反，令 E 为单生 A-模，E 的 c 生成元且 a 为它的湮没子； 线性映射 $\xi \mapsto \xi c$ 定义，当经过为商时，$A_s/a$ 的同构到 E.*

由于$A_s$本身是单生的，由1生成，第一个断言从no. 7（推论1）到命题9。第二个是明显的，因为$\xi \mapsto \xi c$是由假设满射并且有核a。

注，如果 A 不可交换，则单生 A-模 E 的两个不同生成元 c、c' 的湮没子通常是*不同的*，并且也不同于模 E 的湮没子。 另一方面，如果 A 是*可交换的*，则湮没子 E 的生成元 c 包含在 E 的每个元素的湮没子中，因此是整个 E 的湮没子。

#### 推论{#alg-ii-s1-n12-cor-1 .statement tag=05LS}

*单生 A-模 E 的每个子模都同构于商模 b/a，其中 a 和 b 是 A 的两个左理想，使得 a ⊂ b。单源 A-模的每个商模都是单源的。*

第二个断言是直接的，第一个命题22和I, § 4, no. 6、定理4。

注另一方面，单生的模的子模不一定是单生的。对于例，如果A是交换环，其中存在非主理想（VII, § 1, no. 1），这些理想是单生A-模 A的非单生子模。

由定义得出，由E的元素族$(a_i)$生成的A-模E的子模是单源子模的*和*

E的Aa_i；对于 (a_i) 是 E 的基，每个 a_i 是 E 的自由元素并且 Aa_i 的和是直接的，这是充分必要的。

#### 命题 23 {#alg-ii-s1-prop-23 .statement tag=05LT}

令 E 为非零子模的无限族 (M_i)_{i \in I} 的 A-模、直和。对于 E 的每个生成的系统 S，Card(S) \geq Card(I)。

对于所有 x \in S，令 C_x 为指标 i \in I 的有限集合，使得 M_i 中 x 的分量为 \neq 0，并令 C = \bigcup_{x \in S} C_x。对于 i \in C 和假设，每个 x \in S 属于通过 M_i 的 E 直和定义到子模，因此 S 生成 E 意味着 C = I；因为 I 是假设无限的，所以 S 也是无限的（集合理论，III, § 5, no. 1，推论 1 到命题 1）；因此 Card(I) = Card(C) \leq Card(S) （集合理论，III, § 6, no. 3，推论 3 到定理 2）。

#### 推论 1 {#alg-ii-s1-prop-23-cor-1 .statement tag=05LU}

在命题 23 的假设下，假设每个 M_i 是单源的，并且 E 是非零单源子模的第二个族 (N_\lambda)_{\lambda \in L} 的直和。那么卡(L) = 卡(I)。

如果 b_\lambda 是 N_\lambda 的生成元，则 b_\lambda 的集合是 E 的生成的系统，因此 Card(L) \geq Card(I)。特别是 L 是无限的，并且交换 (M_i) 和 (N_\lambda) 的角色，类似的 Card(I) \geq Card(L)，从而推论。

#### 推论 2 {#alg-ii-s1-prop-23-cor-2 .statement tag=05LV}

如果模 E 承认无限基 B，则 E 的每个生成的系统都有基数 \geq Card(B) 并且 E 的每个基等价于 B。

### 13. 标量的变换 OF 环

设 A, B 为环 B 到环 A 中的两个环和 \rho 同态。对于每个 A-模 E， 外法则 (\beta, x) \mapsto \rho(\beta)x 定义 (与加法) B-模据说结构与E上的\rho和A-模结构相关；这个 B-模用 \rho_*(E) 或 E_{[B]} 表示（如果不会引起混淆，甚至可以简单地用 E 表示）。特别地，如果 B 是 A 的子环并且 \rho : B \to A 是典范嵌入，则 E_{[B]} 称为通过将标量 A 到 B 的环限制而获得的 B-模；由于滥用语言，当同态 \rho 是任意的时，也会使用此表达式。

如果 F 是 A-模 E 的子模，则 \rho_*(F) 是 \rho_*(E) 的子模，且 \rho_*(E/F) 等于 \rho_*(E)/\rho_*(F)。

设E、F为两个A-模；每个 A-线性映射 u : E \to F 也是 B-线性映射 E_{[B]} \to F_{[B]} ，用 \rho_*(u) 表示；在其他字中，有典范嵌入个 \mathbf{Z}-modules

(47)
$$
\operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{[B]}, F_{[B]}).
$$

这个映射不一定是双射的；在其他字 B-线性映射 E_{[B]} \to F_{[B]} 不一定是 A 线性的。对于例，E_{[B]} 的子 B 模不一定是 E 的子 A 模：如果 A 为域且 B 子域为 $A$，则向量子空间 $B_s$ 为向量 $B$-空间如果$B \neq A$，则$(A_s)_{[B]}$不是向量子$A$空间。

直接的，对于$A$模块的每个$(E_i)_{i \in I}$族，$B$模块$\rho_*\left(\prod_{i \in I} E_i\right)$（或$\rho_*\left(\bigoplus_{i \in I} E_i\right)$）等于$\prod_{i \in I} \rho_*(E_i)$（或$\bigoplus_{i \in I} \rho_*(E_i)$）。

$\rho_*(E)$的每个生成的系统都是$E$的生成的系统，但逆命题不一定为真。

#### 命题 24 {#alg-ii-s1-prop-24 .statement tag=05LW}

*令$A, B$为两个环和$\rho : B \to A$环同态。*

(i) *如果 $\rho$ 是满射，则典范映射 (47) 是双射。对于每个$A$模块$E$，$\rho_*(E)$的每个子$B$模块都是$E$的子$A$模块； $E$ 中的每生成的系统是 $\rho_*(E)$ 中的生成的系统。*

(ii) *如果$\rho$是单射的，$A$-模块$E$中的每个自由族都是$B$-模块$\rho_*(E)$中的自由族。*

命题紧随定义之后。

注即使$\rho$是单射的，$\rho_*(E)$中的自由族在$E$中也不一定是自由的。

*对于例，1和$\sqrt{2}$不将$\mathbf{R}$中的形式空闲系统视为向量$\mathbf{R}$空间，尽管它们将$\mathbf{R}$中的形式空闲系统视为向量 $\mathbf{Q}$-空间 (cf. 注 1).*

#### 命题 25 {#alg-ii-s1-prop-25 .statement tag=05LX}

*令$A, B$为两个环、$\rho : B \to A$、环、同态和$E$一个$A$模块。令$(\alpha_\lambda)_{\lambda \in L}$为生成的系统（分别为元素、基的自由族），将$A$视为左$B$模块。令$(a_\mu)_{\mu \in M}$为$A$模块$E$的生成的系统（分别为元素、基的自由族）。那么$(\alpha_\lambda a_\mu)_{(\lambda, \mu) \in L \times M}$是$B$-模块$\rho_*(E)$的生成的系统（分别是（当$\rho$是单射时）元素、基的自由族）。*

如果$x = \sum_{\mu \in M} \gamma_\mu a_\mu$，其中$\gamma_\mu \in A$和$(\alpha_\lambda)$是$A$的生成的系统，对于所有$\mu \in M$，从而$x = \sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu$，我们可以写成$\gamma_\mu = \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda$和$\beta_{\lambda \mu} \in B$。另一方面，如果$(\alpha_\lambda)$和$(a_\mu)$是自由族，关系$\sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu = 0$，加上$\beta_{\lambda \mu} \in B$，可以写成$\sum_{\mu \in M} \left( \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda \right) a_\mu = 0$；因此，如果 $\rho$ 是单射的，那么它对于所有 $\mu \in M$ 意味着 $\sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda = 0$，并且因此对于所有 $\lambda, \mu$ 意味着 $\beta_{\lambda \mu} = 0$。

#### 推论 {#alg-ii-s1-n13-cor-1 .statement tag=05LY}

*如果$A$是有限生成的左$B$-模块并且$E$是有限生成的左$A$-模块，则$\rho_*(E)$是有限生成的左$A$-模块。*

令$C$为第三个环，$\rho' : C \to B$环同态以及$\rho'' = \rho \circ \rho'$复合同态。对于每个$A$-模块$E$，紧随定义而来的是$\rho''_*(E) = \rho'_*(\rho_*(E))$。特别是，如果$\rho$是$B$到$A$的*同构*，则$E = \rho'_*(\rho_*(E))$，其中$\rho'$表示$\rho$的逆同构。

#### 注 {#alg-ii-s1-n13-rem-1 .statement tag=05LZ}

(1) 设$K$为域和$K$的$A$子环，并有以下性质：对于$K$的元素的每个有限族$(\xi_i)_{1 \leq i \leq n}$，存在一个非零的$\gamma \in A$，并且使得$\gamma \xi_i \in A$对于$1 \leq i \leq n$（当$A$是*可交换的*并且$K$是$A$的分数的域时，总是满足假设）。令$E$为$K$之上的向量空间，而$E_{[A]}$为通过将标量的环限制为$A$而获得的$A$模。那么，如果一个家庭$(x_\lambda)_{\lambda \in L}$在*$E_{[A]}$*自由的，那么它在*$E$也*自由的。注意可能仅限于$L = \{1, n\}$的情况；如果有关系$\sum_{i=1}^n \xi_i x_i = 0$和$\xi_i \in K$，$\xi_i$不是所有零，那么对于所有$\beta \in A$，$\sum_{i=1}^n (\beta \xi_i) x_i = 0$来说都是如此。通过假设，我们可以假设$A$中有$\beta \neq 0$，这样对于所有$i$，$\beta \xi_i = \alpha_i$属于到$A$；但关系$\sum_{i=1}^n \alpha_i x_i = 0$与假设相反，$\alpha_i$不全是零。

(2) 如果环同态 $\rho : B \to A$ 是满射且 $b$ 是它的核（因此 $A$ 与 $B/b$ 被规范地等同），那么，对于每个 $A$-模 $E$， $b$包含在$\rho_*(E)$的湮没子中，$E$是通过no. 12中定义的过程从$\rho_*(E)$派生的$A$模块。

令$A, B$为两个环和$\rho : B \to A$同态。设$E$为$A$模块，$F$为$B$模块； *B-线性* 映射 $u : F \to \rho_*(E)$（如果不引起混淆，也称为 *$F$ *到* $E$ 的 *B-线性映射）也称为 $B$ 模块 $F$ 的 *半线性映射*（相对于 $\rho$） $A$-模块$E$；也有人说，有序对$(u, \rho)$是$F$到$E$的*二态性*；因此，这意味着，对于 $x \in F, y \in F$ 和 $\beta \in B$，

$$
\begin{cases}
u(x + y) = u(x) + u(y) \\
u(\beta x) = \rho(\beta) u(x).
\end{cases}
$$

如果不会引起混淆，$B$的集合$\mathrm{Hom}_B(F, \rho_*(E))$-$F$到$E$的线性映射也可写为$\mathrm{Hom}_B(F, E)$。

当$\rho$是$B$到$A$的*同构*时，所有$\beta \in B$的关系$u(\beta x) = \rho(\beta) u(x)$也可以写成所有$\alpha \in A$的$u(\rho'(\alpha)x) = \alpha x$，其中$\rho'$表示逆同构共 $\rho$；说 $u$ 对于 $\rho$ 来说是半线性的，则相当于说，$u$ 是* $\rho'_*(F)$ *到* $E$ 的 *A-线性映射。

#### 例 {#alg-ii-s1-n13-exa-1 .statement tag=05M0}

已经看出（no. 1）位似$h_\alpha : x \mapsto \alpha x$在$A$模块$E$上不一定是线性映射。但如果$\alpha$是*可逆的*，$h_\alpha$是相对于$A$的内自同构$\xi \mapsto \alpha \xi \alpha^{-1}$的*半线性*映射（而且是双射），对于$\alpha(\lambda x) = (\alpha \lambda \alpha^{-1})(\alpha x)$。

设 C 为第三个环，$\rho': C \to B$ 同态，G C-模。如果$v: G \to F$是相对于$\rho'$的半线性映射，则合成$w = u \circ v$是G到E相对于同态$\rho'' = \rho \circ \rho'$的半线性映射。如果$\rho$是*同构*并且$u: F \to E$是相对于$\rho$的*双射的*半线性映射，则逆映射$u': E \to F$是*相对于$\rho$的逆同构*$\rho': A \to B$的半线性映射。

由此可见，对于通过对A上的集合环结构和E上的左A-模结构的有序对(A，E)定义的结构的类来说，*二态性*$(u, \phi)$可取为*态射* （*集合理论*，IV, § 2, no. 1）；接下来我们将始终假设态射中的选择已经制作完成。

*注(3)*。令$A_1, A_2$为两个环，$A = A_1 \times A_2$为它们的乘积，并让$e_1 = (1, 0),\ e_2 = (0, 1)$在A中，这样$A_1$和$A_2$规范地等同于A的双面理想$Ae_1$和$Ae_2$。对于每个A-模E， $e_1E$和$e_2E$是E的子A模块$E_1,\ E_2$，分别被$e_2$和$e_1$湮灭，因此，将$A/Ae_2$与$A_1$和$A/Ae_1$与$A_2$、$E_1$规范地识别（或$E_2$）被赋予一个$A_1$-模块（或$A_2$-模块）结构。而且，E是$E_1$和$E_2$的*直和*，因为每个$x \in E$都可以写成$x = e_1x + e_2x$和关系，$e_1x = e_2y$意味着$e_1x = e_1^2x = e_1e_2y = 0$。相反，对于$A_1$-模块$F_1$和$A_2$-模块$F_2$的每个有序对由……组成，令$E_1$为A-模$(p_1) * (F_1)$、$E_2$A-模 $(p_2) * (F_2)$、$p_1$和$p_2$分别是A到$A_1$和$A_2$的投影；然后在A-模$E = E_1 \oplus E_2,\ E_1 = e_1E,\ E_2 = e_2E$。因此，A-模的研究被简化为$A_1$-模块和$A_2$-模块的研究。特别是，E 的每个子模 M 都是形式 $M_1 \oplus M_2$，其中 $M_1 = e_1M$ 和 $M_2 = e_2M$。

### 14. 多模块

设A、B为两个环，并在集合E上考虑两个左模结构，具有*相同*加法律，且其环运算符分别为A和B；令 $\mathscr{E}$ 为加法群 E 的自同态环，并且对于所有 $\alpha \in A$（分别为 $\beta \in B$），令 $h_\alpha$（分别为 $h'_\beta$）表示元素 $x \mapsto \alpha x$（分别为 $x \mapsto \beta x$） $\mathscr{E}$。显然，以下三个属性是等效的： (a) $h_\alpha \circ h'_\beta = h'_\beta \circ h_\alpha$ 对于所有 $\alpha$ 和 $\beta$； (b) 同态 $a \mapsto h_\alpha$下的A的像*包含在*$\mathrm{Hom}_B(E, E)$中； (c) 同态 $\beta \mapsto h'_\beta$ 下的 B 的像 *包含在* $\mathrm{Hom}_A(E, E)$ 中。当A-模（或B-模）结构是右模结构时，环 A（或B）必须在（b）（或（c））中用$A^0$（或$B^0$）替换。上述性质可以用说来表示，E上定义的两个（左或右）模结构是*相容的*的。

#### 定义 13 {#alg-ii-s1-def-13 .statement tag=05M1}

*设*$(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$ *为环的两个家庭；一个* $((A_\lambda),\ (B_\mu))$*-多模块*（或*环* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$系列上的多模块）*是集合* E *对于每个* $\lambda \in L$，*左* $A_\lambda$*-模块结构，并且对于每个* $\mu \in M$，*右* $B_\mu$*-模块结构，所有这些模结构都兼容一个另一个.*

当族$(B_\mu)$（或$(A_\lambda)$）为空时，E 称为*左*（或*右*）*多模块*。当 Card(L) + Card(M) = 2 时，我们说“*双模*”而不是“*multimodule*”；然后，通常可以方便地将双模视为相对于环 A 和*右模* 具有*左模* 结构（正如操作符的替换环总是可以通过其对立面cf.no. 1来完成） 结构相对于环 B，律的可置换性则用关系表示

$$
\alpha(x\beta) = (\alpha x)\beta \quad \text{for } x \in E, \alpha \in A, \beta \in B.
$$

那么也可以说 E 是 *(A, B)*-*双模*。

如果 E 上的所有模结构其中定义这些多模块结构中的一个或另一个与一个另一个兼容，则集合 E 上的两个 *多模块* 结构被称为“相容的”。

#### 例 {#alg-ii-s1-n14-exa-1 .statement tag=05M2}

(1) 在环上，$A_s$ 和 $A_d$ 的 A 模结构是兼容的，因此 A 可以被规范地视为 (A, A)-双模。

(2) 左A-模 E 在环 $\operatorname{End}_A(E)$ 上具有规范的左模结构，并且 E 上的 A-模和 $\operatorname{End}_A(E)$ 模块结构是*兼容的*。

显然，当 E 是环的两个族 $(A_\lambda)_{\lambda \in L}, (B_\mu)_{\mu \in M}$ 上的多模块时，E 也是任意两个子族 $(A_\lambda)_{\lambda \in L'}, (B_\mu)_{\mu \in M'}$ 上的多模块，其中 $\lambda \in L'$ 和 $\mu \in M'$ 的 $A_\lambda$ 模块和 $B_\mu$ 模块结构是最初给出的结构。

由于多模块是特定的例与运算符的可交换群，因此 nos 的结果。 2到10（cf.no. 10，*注*）可以应用于它们；特别是，如果 E、F 是两个 $((A_\lambda), (B_\mu))$ 多模，则 *同态* $u : E \to F$ 是映射，这是所有 $\lambda \in L$ 的 $A_\lambda$ 同态，以及所有 $\mu \in M$ 的 $B_\mu$ 同态。 $((A_\lambda), (B_\mu))$-多模的稳定子群是 $((A_\lambda), (B_\mu))$-多模（称为*子多模*），以及此类子群的商（称为*商多模*）； 乘积和直和类似。

设 E 为 $((A_\lambda), (B_\mu))$ 多模块，对于每个 $\lambda \in L$（分别为 $\mu \in M$），令 $\phi_\lambda : A'_\lambda \to A_\lambda$（分别为 $\psi_\mu : B'_\mu \to B_\mu$）为环同态；显然，与E上给出的$\phi_\lambda$和$A_\lambda$模块结构相关联的$A'_\lambda$模块结构以及与E上给出的$\psi_\mu$和$B_\lambda$模块结构相关联的$B'_\mu$模块结构与另一个兼容，因此E上的定义兼容$((A'_\lambda), (B'_\mu))$-多模块结构，据说与给定的$((A_\lambda), (B_\mu))$-多模块结构以及$\phi_\lambda$和$\psi_\mu$“关联”。

如果E、F是两个$((A_\lambda), (B_\mu))$多模块，则E到F中的同态的加法群表示为$\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$（或简称为$\operatorname{Hom}(E, F)$）。 no. 2的公式(6)到(8)显然对于$((A_\lambda), (B_\mu))$-多模块同态有效，特别是$\operatorname{Hom}(E, E) = \operatorname{End}(E)$有一个*环*结构；

此外，Hom(E, F) 具有规范的 *left* End(F) 模块结构和 *right* End(E) 模块结构，这两个结构是兼容的；在其他字中，Hom(E, F) 有一个规范的 (End(F), End(E))-**双模** 结构。

现在假设 E 有一个多模块结构，其左（右）运算符的环一方面是 $\lambda \in L$ 的 $A_\lambda$（分别是 $\mu \in M$ 的 $B_\mu$），另一方面是另一个系列 $(A'_{\lambda'})_{\lambda' \in L'}$ 的环（分别是 $(B'_{\mu'})_{\mu' \in M'}$）。 Suppose similarly that F has a multimodule structure whose rings of left (resp. right) operators are on the one hand the $A_\lambda$ for $\lambda \in L$ (resp. the $B_\mu$ for $\mu \in M$) and on the other the rings of another family $(A''_{\lambda''})_{\lambda'' \in L''}$ (resp. $(B''_{\mu''})_{\mu'' \in M''}$); to abbreviate we shall say that E is an (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$))-multimodule and F an (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$))-multimodule. 将 E 和 F 视为 (($A_\lambda$), ($B_\mu$))-多模块，从而“限制”运算符到子族 ($A_\lambda$) 和 ($B_\mu$)。 根据本文开头所述，在 E 和 F 定义上给出的多模块结构规范地环同态

$$
A'_{\lambda'} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E), \qquad {B'_{\mu'}}^0 \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E),
$$
$$
A''_{\lambda''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F), \qquad B''_{\mu''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F);
$$

moreover, two elements of $\operatorname{End}_{(A_\lambda), (B_\mu)}(E)$ (resp. $\operatorname{End}_{(A_\lambda), (B_\mu)}(F)$) respective images of elements of two distinct rings among the $A'_{\lambda'}$, or the ${B'_{\mu'}}^0$ (resp. the $A''_{\lambda''}$ or the $B''_{\mu''}$) are permutable; it follows that the above homomorphisms define on $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ a *multimodule* structure whose rings of *left* operators are the $A''_{\lambda''}$ ($\lambda'' \in L''$) and the $B'_{\mu'}$ ($\mu' \in M'$) and whose rings of *right* operators are the $A'_{\lambda'}$ ($\lambda' \in L'$) and the $B''_{\mu''}$ ($\mu'' \in M''$).

如果现在 $E'$ 是 (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$))-多模块，$F'$ 是 (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$))-多模块， $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')$ 是

$$
((A''_{\lambda''}), (B'_{\mu'}); (A'_{\lambda'}), (B''_{\mu''}))\text{-multimodule};
$$

如果 $u : E' \to E, v : F \to F'$ 是多模块同态，

$$
\operatorname{Hom}(u, v) : \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F) \to \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')
$$

定义如no. 2，并且是一个*多模块*同态。

#### 注 {#alg-ii-s1-n14-rem-1 .statement tag=05M3}

(1) 设F为A-模，C为环A的*中心*；由于中心同位与所有同位交换，F 有一个 *双模* 结构，其环左运算符是 A 和 C。如果 E 是另一个 A-模，则 $\operatorname{Hom}_A(E, F)$ 因此具有规范的 C-*模* 结构（其中，对于$f \in \operatorname{Hom}_A(E, F)$和$\gamma \in C$，$\gamma f$为同态$x \mapsto \gamma f(x)$）；如果E'，F'是两个A-模，$u : E' \to E, v : F \to F'$两个A-同态，映射$\operatorname{Hom}(u, v)$是C-*线性*。

(2) 设E为左A-模；由于 A 具有规范的 (A, A) 双模结构，因此对于任何索引集合 T 都有直和 $A^{(T)}$；由上可知，$\mathrm{Hom}_A(A_s^{(T)}, E)$有一个规范的*左A-模* 结构，源自$A_s^{(T)}$上的*右*A-模结构：对于$f \in \mathrm{Hom}_A(A_s^{(T)}, E)$和$\alpha \in A$，$\alpha f$是线性映射 $x \mapsto f(x\alpha)$。 no. 11定义典范映射$j_{E, T}$的推论2至命题17从乘积模$E^T$到$\mathrm{Hom}_A(A_s^{(T)}, E)$，$j_{E, T}$下的像 $(x_t)_{t \in T}$为线性映射$f : A_s^{(T)} \to E$，使得$f(e_t) = x_t$对于所有$t \in T$（其中$(e_t)$是$A_s^{(T)}$的典范基）；已知（*loc.cit.*）$j_{E, T}$是*双射的*，并且从上面给出的A-模结构在$\mathrm{Hom}_A(A_s^{(T)}, E)$上得出的定义得出，$j_{E, T}$是*A-线性的*。最后，如果$u : E \to F$是A-模同态，图表

$$
\begin{array}{ccc}
E^T & \xrightarrow{j_{E, T}} & \mathrm{Hom}_A(A_s^{(T)}, E) \\
u^T \downarrow & & \downarrow \mathrm{Hom}(1, u) \\
F^T & \xrightarrow{j_{F, T}} & \mathrm{Hom}_A(A_s^{(T)}, F)
\end{array}
$$

是*可交换的*。

注，当T由单个元素组成时，$j_E : E \to \mathrm{Hom}_A(A_s, E)$就是no. 2中定义的映射$x \mapsto \theta_x$，*例* 1。

### 习题 {#alg-ii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
