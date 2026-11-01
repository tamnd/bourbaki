---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: Cartan subalgebras and regular elements of a Lie algebra
lang: zh
source: lie-vii-ix
book_pages: 12-20, 55-57
pdf_pages: 0022-0030, 0064-0066
extraction: native
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS
      page: 13
      pdf_page: 23
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE ALGEBRA
      page: 16
      pdf_page: 26
    - "no": 3
      title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
      page: 18
      pdf_page: 28
    - "no": 4
      title: CARTAN SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS
      page: 19
      pdf_page: 29
statements: 40
exercises: 16
content_sha256: 233c07b14713105a91722f5eb2891bf2d9a2ad86c5879ab7569ff14a1d47c7c6
translated_from: content/en/lie/VII/02_s2_cartan_subalgebras_and_regular_elements.md
translation_method: google
source_content_sha256: 05b31ef931fa1971af6f075dc663eed9dae014f8584d9c3690519a9cceb1ce2d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 381766fb1e7ac1292b3ae304917d2d03a7633091bc7fac0383be7126a3d63180
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。 嘉当子代数和正则元素李代数

从 no. 2 开始，域 $k$ 被假定为无限。

### 1.嘉当子代数

#### 定义 1 {#lie-vii-s2-def-1 .statement tag=00TJ}

设$\mathfrak{g}$为李代数。 $\mathfrak{g}$的嘉当子代数是$\mathfrak{g}$的幂零子代数，等于其自身的归一化器。

稍后我们将得到如下结果：

1) 如果 $k$ 是无限的，$\mathfrak{g}$ 有嘉当子代数（no. 3，Th.1 的 Cor.1）；

2) 如果$k$是特征零，则$\mathfrak{g}$的所有嘉当子代数都具有相同的维数（§3, no. 3，Th.2）；

3) 如果$k$是代数闭的且特征为0，则$\mathfrak{g}$的所有嘉当子代数在$\mathfrak{g}($§3, no. 2的初等自同构的群下都是共轭，Th。 1）。

#### 例 1 {#lie-vii-s2-n1-exa-1 .statement tag=00TK}

如果$\mathfrak{g}$幂零，$\mathfrak{g}$中唯一的嘉当子代数就是$\mathfrak{g}$本身（第I, §4, no. 1章，命题3）。

#### 例 2 {#lie-vii-s2-n1-exa-2 .statement tag=00TL}

设$\mathfrak{g}=\mathfrak{g}\mathfrak{l}(n, k)$，并设$\mathfrak{h}$为矩阵属于到$\mathfrak{g}$的对角线集合。我们证明$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数。首先，$\mathfrak{h}$是可交换的，因此是幂零的。令$(E_{ij})$为$\mathfrak{g}\mathfrak{l}(n, k)$的典范基，并令$x=\sum\mu_{ij}E_{ij}$为$\mathfrak{g}$中$\mathfrak{h}$标准化器的元素。如果$i\not=j$，公式（5）章。 I, §1, no. 2表明$E_{ij}$在$[E_{ii}, x]$中的系数为$\mu_{ij}$。由于$E_{ii}\in \mathfrak{h}$、$[E_{ii}, x]\in \mathfrak{h}$，所讨论的系数是零。因此$\mu_{ij}= 0$对应$i\not=j$，所以$x\in \mathfrak{h}$，这表明$\mathfrak{h}$确实是$\mathfrak{g}$的嘉当子代数。

#### 例 3 {#lie-vii-s2-n1-exa-3 .statement tag=00TM}

令$\mathfrak{h}$为$\mathfrak{g}$的嘉当子代数，并令$\mathfrak{g}_1$为$\mathfrak{g}$包含$\mathfrak{h}$的子代数。那么$\mathfrak{h}$就是$\mathfrak{g}_1$的嘉当子代数；这立即来自 Def。 1.

#### 命题 1 {#lie-vii-s2-prop-1 .statement tag=00TN}

令$\mathfrak{g}$为李代数，令$\mathfrak{h}$为$\mathfrak{g}$的嘉当子代数。那么$\mathfrak{h}$是$\mathfrak{g}$的最大幂零子代数。

令 $\mathfrak{h}'$ 为 $\mathfrak{g}$ 包含 $\mathfrak{h}$ 的幂零子代数。那么$\mathfrak{h}$是$\mathfrak{h}'$(例3)的嘉当子代数，所以$\mathfrak{h}=\mathfrak{h}'$(例1)。

存在不是嘉当子代数的最大幂零子代数（练习 2）。

#### 命题 2 {#lie-vii-s2-prop-2 .statement tag=00TO}

令$(\mathfrak{g}_i)_{i\in I}$为李代数和$\mathfrak{g}=\prod_{i\in I}\mathfrak{g}_i$的有限族。

嘉当子代数 / $\mathfrak{g}$ 是子代数 / 形式 $\prod_{i\in I}\mathfrak{h}_i$，其中 $\mathfrak{h}_i$

是嘉当子代数 / $\mathfrak{g}_i$。

如果使用标准化器$\mathfrak{n}_i$，$\mathfrak{h}_i$是$\mathfrak{g}_i$的子代数，则使用标准化器$\prod\mathfrak{n}_i$，$\prod\mathfrak{h}_i$是$\mathfrak{g}$的子代数；如果 $\mathfrak{h}_i$ 幂零，则 $\prod\mathfrak{h}_i$ 幂零；因此，如果$\mathfrak{h}_i$是$\mathfrak{g}_i$的嘉当子代数，则所有$i,\prod\mathfrak{h}_i$是$\mathfrak{g}$的嘉当子代数。相反，令$\mathfrak{h}$为$\mathfrak{g}$的嘉当子代数； $\mathfrak{h}$的投影$\mathfrak{h}_i$到$\mathfrak{g}_i$是$\mathfrak{g}_i$的幂零子代数，$\prod\mathfrak{h}_i$是$\mathfrak{g}$包含$\mathfrak{h}$的幂零子代数；因此$\mathfrak{h}=\prod\mathfrak{h}_i$（命题1）；因此，对于所有 $i,\mathfrak{h}_i$ 来说，它是 $\mathfrak{g}_i$ 中自己的标准化器，$\mathfrak{g}_i$ 的嘉当子代数也是如此。

#### 例 4 {#lie-vii-s2-n1-exa-4 .statement tag=00TP}

如果$k$具有特征，$0,\mathfrak{g}\mathfrak{l}(n, k)$是理想$\mathfrak{s}\mathfrak{l}(n, k)$和$k.1$的乘积。由例2和命题2可知，$\mathfrak{s}\mathfrak{l}(n, k)$中迹线0的对角线矩阵的集合是$\mathfrak{s}\mathfrak{l}(n, k)$的嘉当子代数。

#### 命题 3 {#lie-vii-s2-prop-3 .statement tag=00TQ}

设$\mathfrak{g}$为李代数，$\mathfrak{g}$为$\mathfrak{h}$子代数，$k'$扩张为$k$。那么$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数当且仅当$\mathfrak{h}\otimes_kk'$是$\mathfrak{g}\otimes_kk'$的嘉当子代数。

事实上，$\mathfrak{h}$ 是幂零的当且仅当 $\mathfrak{h}\otimes_kk'$ 是（第 I, §4, no. 5）。另一方面，如果$\mathfrak{n}$是$\mathfrak{g}$中$\mathfrak{h}$的归一化器，则$\mathfrak{g}\otimes_kk'$中$\mathfrak{h}\otimes_kk'$的归一化器是$\mathfrak{n}\otimes_kk'$（第I, §3, no. 8章）。

#### 命题 4 {#lie-vii-s2-prop-4 .statement tag=00TR}

令$\mathfrak{g}$为李代数，$\mathfrak{h}$是$\mathfrak{g}$的幂零子代数。那么$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数当且仅当$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$。

如果$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h},\mathfrak{h}$是它自己的标准化子（§1，命题10（i）），那么$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数。假设$\mathfrak{g}^0(\mathfrak{h})\not=\mathfrak{h}$。考虑通过商从伴随表示获得 $\mathfrak{g}^0(\mathfrak{h})/\mathfrak{h}$ 上 $\mathfrak{h}$ 的表示。通过应用恩格尔的定理（第I, §4, no. 2，第1章），我们看到存在$x\in \mathfrak{g}^0(\mathfrak{h})$使得$x \notin \mathfrak{h}$和$[\mathfrak{h}, x]\subset \mathfrak{h}$；然后$x$属于到$\mathfrak{g}$中$\mathfrak{h}$的归一化器，所以$\mathfrak{h}$不是$\mathfrak{g}$的嘉当子代数。

#### 推论 1 {#lie-vii-s2-prop-4-cor-1 .statement tag=00TS}

令$\mathfrak{g}$为李代数，$\mathfrak{h}$嘉当子代数/$\mathfrak{g}$。如果$k$是无限的，则存在$x\in \mathfrak{h}$使得$\mathfrak{h}=\mathfrak{g}^0(x)$。

事实上，$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$，我们可以应用§1的第9（ii）号提案。

#### 推论 2 {#lie-vii-s2-prop-4-cor-2 .statement tag=00TT}

令 $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ 为满同态 / 李代数。如果$\mathfrak{h}$是$\mathfrak{g},f(\mathfrak{h})$的嘉当子代数，那么$\mathfrak{g}'$的嘉当子代数。

事实上，$f(\mathfrak{h})$是$\mathfrak{g}'$的幂零子代数。另一方面，考虑 $\mathfrak{g}'$ 上的表示 $x \rightarrow$ 和 $f(x)$ 的 $\mathfrak{h}$。根据§1, no. 3、$f(\mathfrak{g}^0(\mathfrak{h})) ={\mathfrak{g}'}^0(\mathfrak{h})$第 9 (iv) 号提案。现在$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$，另一方面很明显${\mathfrak{g}'}^0(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$。因此，$f(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$ 就足以应用第 4 条命题。

#### 推论 3 {#lie-vii-s2-prop-4-cor-3 .statement tag=00TU}

令$\mathfrak{h}$为李代数$\mathfrak{g}$的嘉当子代数，并令$\mathscr{C}^n\mathfrak{g}(n\geq 1)$为$\mathfrak{g}$的下降中央级数的项（第I, §1, no. 5章）。然后$\mathfrak{g}=\mathfrak{h}+\mathscr{C}^n\mathfrak{g}$。

事实上，推论2表明，$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$中$\mathfrak{h}$的像是$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$的嘉当子代数，因此等于$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$，因为$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$是幂零的（例1）。

#### 推论 4 {#lie-vii-s2-prop-4-cor-4 .statement tag=00TV}

令$\mathfrak{g}$为李代数，$\mathfrak{g}$中的$\mathfrak{h}$嘉当子代数，以及$\mathfrak{g}$包含$\mathfrak{h}$中的$\mathfrak{a}$子代数。

(i) $\mathfrak{a}$ 等于$\mathfrak{g}$ 中它自己的标准化器。

(ii) 假设$k=\mathbf{R}$或$\mathbf{C}$；令 G 为李群和李代数 $\mathfrak{g}$，A 是 G 和李代数 $\mathfrak{a}$ 的积分子群。则 A 是 G 的 Lie 子群，并且它是 G 中 A 的归一化子的恒等分量。

令$\mathfrak{n}$为$\mathfrak{g}$中$\mathfrak{a}$的归一化器。由于$\mathfrak{h}$是$\mathfrak{n}$的嘉当子代数（例$3$）$,\{0\}$是$\mathfrak{n}/\mathfrak{a}$的嘉当子代数（Cor.2），因此等于$\mathfrak{n}/\mathfrak{a}$中的归一化器； in other 字, $\mathfrak{n}=\mathfrak{a}$. 断言 (ii) follows from (i) and Chap. III, §9, no. 4, Cor. of Prop. 11.

#### 推论 5 {#lie-vii-s2-prop-4-cor-5 .statement tag=00TW}

设$\mathfrak{g}$为李代数，E为$\mathfrak{g}$的子集。让 E 通过伴随表示对 $\mathfrak{g}$ 进行运算。那么E是$\mathfrak{g}$的嘉当子代数当且仅当$E =\mathfrak{g}^0(E)$。

条件 is necessary (Prop. 4). Assume now that $E =\mathfrak{g}^0(E)$.根据§1, no. 1的命题2(ii)，E则为$\mathfrak{g}$的子代数。如果$x\in E$，则从$E\subset \mathfrak{g}^0(E)$开始，ad$_Ex$是幂零的； hence 代数 E is nilpotent. But then E is 嘉当子代数 by Prop. 4.

#### 推论 6 {#lie-vii-s2-prop-4-cor-6 .statement tag=00TX}

Let $\mathfrak{g}$ be 李代数, let $k_0$ be 子域 of $k$ such that $[k:k_0]<+\infty$, and let $\mathfrak{g}_0$ be 李代数 obtained from $\mathfrak{g}$ by restricting 域 of scalars to $k_0$。 Let $\mathfrak{h}$ be 子集 of $\mathfrak{g}$.那么$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数当且仅当$\mathfrak{h}$是$\mathfrak{g}_0$的嘉当子代数。

这是从 Cor 得出的。 5、由于条件$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$不涉及基域。

#### 命题 5 {#lie-vii-s2-prop-5 .statement tag=00TY}

令$\mathfrak{g}$为李代数，$\mathfrak{c}$为中心，$\mathfrak{h}$向量子空间为$\mathfrak{g}$。那么$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数当且仅当$\mathfrak{h}$包含$\mathfrak{c}$并且$\mathfrak{h}/\mathfrak{c}$是$\mathfrak{g}/\mathfrak{c}$的嘉当子代数。

Assume that $\mathfrak{h}$ is 嘉当子代数 of $\mathfrak{g}$.从$[\mathfrak{c},\mathfrak{g}]\subset \mathfrak{h}$开始，我们有$\mathfrak{c}\subset \mathfrak{h}$。另一方面，Cor. 的$\mathfrak{h}/\mathfrak{c}$ 是$\mathfrak{g}/\mathfrak{c}$ 的嘉当子代数。 2 of Prop. 4.

假设$\mathfrak{h}\supset \mathfrak{c}$且$\mathfrak{h}/\mathfrak{c}$是$\mathfrak{g}/\mathfrak{c}$的嘉当子代数。令$f$为从$\mathfrak{g}$到$\mathfrak{g}/\mathfrak{c}$的规范态射。 代数 $\mathfrak{h}$，它是$\mathfrak{h}/\mathfrak{c}$的中心扩张，是幂零的。令$\mathfrak{n}$为$\mathfrak{g}$中$\mathfrak{h}$的标准化。如果$x\in \mathfrak{n}$，$[f(x),\mathfrak{h}/\mathfrak{c}]\subset \mathfrak{h}/\mathfrak{c}$，则$f(x)\in \mathfrak{h}/\mathfrak{c}$，等等$x\in \mathfrak{h}$。这就证明了$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数。

#### 推论{#lie-vii-s2-n1-cor-1 .statement tag=00TZ}

令$\mathscr{C}_{\infty}\mathfrak{g}$为李代数$\mathfrak{g}$的升中中央级数的并（第I, §1, no. 6章）。 $\mathfrak{g}$嘉当子代数是$\mathfrak{g}/\mathscr{C}_{\infty}\mathfrak{g}$嘉当子代数逆像。

事实上，$\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$的中心是$\mathscr{C}_{i+1}\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$，并且推论直接从第5条命题归纳得出。

#### 注 {#lie-vii-s2-n1-rem-1 .statement tag=00U0}

$\mathscr{C}_{\infty}\mathfrak{g}$ is the smallest ideal $\mathfrak{n}$ of $\mathfrak{g}$ such that the centre of $\mathfrak{g}/\mathfrak{n}$ is zero; it is a characteristic and nilpotent ideal of $\mathfrak{g}$.

### 2. 正则元素的李代数

[回想一下，从现在开始，$k$ 被假定为无限。]

设$\mathfrak{g}$为维数$n$中的李代数。如果$x\in \mathfrak{g}$，则将ad$x$的特征多项式写在形式中

det(T $-$ ad $x$) $=\sum_{i=0}^na_i(x)T^i$，与 $a_i(x)\in k$。

我们有 $a_i(x) = (-1)^{n-i}$Tr $(\bigwedge^{n-i}$ ad x)、cf. 代数，第 1 章。 III, §8, no. 11。这表明$x \rightarrow a_i(x)$是从$\mathfrak{g}$到$k($代数的次数$n-i$的齐次多项式映射，第1章。 IV, §5, no. 9）。

#### 注 1 {#lie-vii-s2-n2-rem-1 .statement tag=00U1}

如果 $\mathfrak{g}\not=\{0\},a_0= 0$ 自 (ad $x$)$(x) = 0$ 对于所有 $x\in \mathfrak{g}$。

#### 注 2 {#lie-vii-s2-n2-rem-2 .statement tag=00U2}

设$k'$为$k$的扩张。为 $x'\in \mathfrak{g}\otimes_kk'$ 编写 det(T $-$ ad $x'$) $=\sum_{i=0}^na'_i(x')T^i$。然后 $a'_i|\mathfrak{g}=a_i$ 代表所有 $i$。

#### 定义 2 {#lie-vii-s2-def-2 .statement tag=00U3}

$\mathfrak{g}$的秩，用rk($\mathfrak{g}$)表示，是最小的整数$l$，使得$a_l\not= 0$。如果$a_l(x)\not= 0$，则$\mathfrak{g}$的元素$x$称为正则。

对于所有 $x\in \mathfrak{g}$，rk($\mathfrak{g}$)$\leq$ dim$\mathfrak{g}^0(x)$ 和等式当且仅当 $x$ 是正则时成立。

正则元素的集合密集，而对于 Zariski 拓扑（App. I），$\mathfrak{g}$ 则开放。

#### 例 1 {#lie-vii-s2-n2-exa-1 .statement tag=00U4}

如果$\mathfrak{g}$是幂零的，那么rk($\mathfrak{g}$)$=$dim$\mathfrak{g}$和$\mathfrak{g}$的所有元素都是正则的。

#### 例 2 {#lie-vii-s2-n2-exa-2 .statement tag=00U5}

让$\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$。如果$x=(\gamma -\alpha )\in \mathfrak{g}$，一个简单的计算可以得出

$$
\beta \gamma
$$

det(T $-$广告$x$)$= T^3-4(\alpha \beta +\gamma^2)T$。

如果$k$的特征是$\not= 2$，那么rk($\mathfrak{g}$)$= 1$和正则元素就是那些$x$使得$\alpha \beta +\gamma^2\not= 0$。

#### 例 3 {#lie-vii-s2-n2-exa-3 .statement tag=00U6}

令V为有限维$n$和$\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$中的向量空间。令$\overline{k}$为$k$的代数闭包。令$x\in \mathfrak{g}$，并令$\lambda_1, . . . , \lambda_n$为$x$的特征多项式的$\overline{k}$中的根（每个根被写入等于其重数的次数数）。 典范同构从$V^*\otimes V$到$\mathfrak{g}$与这两个空间的$\mathfrak{g}$模块结构兼容，在其他字中需要$1\otimes x-^tx\otimes 1$到$x$（第I, §3, no. 3章，第4条）。根据命题4(i)§1，可以得出ad$x$的特征多项式的根是$1\leq i\leq n,1\leq j\leq n$的$\lambda_i-\lambda_j$（每个根被写数的次数等于其重数）。因此，$\mathfrak{g}$的秩是$n$，并且$x$是正则的当且仅当每个$\lambda_i$是$x$的特征多项式的简单根。

#### 命题 6 {#lie-vii-s2-prop-6 .statement tag=00U7}

设$\mathfrak{g}$为李代数，$k$的$k'$扩张，以及$\mathfrak{g}'=$$\mathfrak{g}\otimes_kk'$。

(i) $\mathfrak{g}$的元素$x$在$\mathfrak{g}$中是正则当且仅当$x\otimes 1$在$\mathfrak{g}'$中是正则。

(ii) rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)。

这是从注 2 得出的。

#### 命题 7 {#lie-vii-s2-prop-7 .statement tag=01IY}

令$(\mathfrak{g}_i)_{i\in I}$为李代数的有限族，并令$\mathfrak{g}=$$\prod_{i\in I}\mathfrak{g}_i$。

(i) $\mathfrak{g}$ 的元素 $(x_i)_{i\in I}$ 在 $\mathfrak{g}$ 中是正则当且仅当 $i\in I,x_i$ 在 $\mathfrak{g}_i$ 中是正则。

(ii) rk($\mathfrak{g}$) $=\sum_{i\in I}$ rk($\mathfrak{g}_i$)。

事实上，对于任何$x= (x_i)_{i\in I}\in \mathfrak{g}$，ad$_{\mathfrak{g}}x$的特征多项式是ad$_{\mathfrak{g}_i}x_i$的特征多项式的乘积。

#### 命题 8 {#lie-vii-s2-prop-8 .statement tag=00U8}

令 $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ 为李代数中的满同态。

(i) 如果$x$是正则元素，$\mathfrak{g},f(x)$在$\mathfrak{g}'$中是正则。如果 Ker $f$ 包含在 $\mathfrak{g}$ 的中心中，则逆命题为 true。

(ii) rk($\mathfrak{g}$)$\geq$ rk($\mathfrak{g}'$)。

将 rk($\mathfrak{g}$) $=r$，rk($\mathfrak{g}'$) $=r'$。让$x\in \mathfrak{g}$。 ad $x$、ad $f(x)$、ad $x|$Ker $f$的特征多项式为形式

$$
P(T) = T^n+a_{n-1}(x)T^{n-1}+\cdots +a_r(x)T^r
$$

$$
Q(T) = T^{n'}+b_{n'-1}(x)T^{n'-1}+\cdots +b_{r'}(x)T^{r'}
$$

$$
R(T) = T^{n''}+c_{n''-1}(x)T^{n''-1}+\cdots +c_{r''}(x)T^{r''}
$$

其中 $a_i, b_i, c_i$ 是 $\mathfrak{g}$ 上的多项式函数，还有 $a_r\not= 0, b_{r'}\not= 0, c_{r''}\not= 0$。我们有 P = QR，因此 $r=r'+r''$ 和 $a_r(x) =b_{r'}(x)c_{r''}(x)$，这证明了 (ii) 和 (i) 的第一个断言。如果 Ker $f$ 包含在 $\mathfrak{g}$、$R(T) = T^{n''}$ 的中心中，因此$a_r(x) =b_{r'}(x)$，因此是 (i) 的第二个断言。

#### 推论{#lie-vii-s2-n2-cor-1 .statement tag=00U9}

令$\mathscr{C}_n\mathfrak{g}(n\geq 0)$为$\mathfrak{g}$的上升中央级数的项（第I, §1, no. 6章）。 $\mathfrak{g}$中的正则元素是那些$\mathfrak{g}/\mathscr{C}_n\mathfrak{g}$中的像是规则的。

#### 命题 9 {#lie-vii-s2-prop-9 .statement tag=00UA}

设$\mathfrak{g}$为李代数，$\mathfrak{g}'$子代数等于$\mathfrak{g}$。 $\mathfrak{g}$中的$\mathfrak{g}'$正则中的每个元素在$\mathfrak{g}'$中都是正则。

对于$x\in \mathfrak{g}'$，ad$_{\mathfrak{g}}x$到$\mathfrak{g}'$的限制是ad$_{\mathfrak{g}'}x$，因此向量空间$\mathfrak{g}/\mathfrak{g}'$的定义自同态$u(x)$通过商。令$d_0(x)$（或$d_1(x)$）为ad$_{\mathfrak{g}'}(x)$（或$u(x)$）零空间的维数，并令$c_0$（或$c_1$）为$d_0(x)$（或$d_1(x)$）的最小值当$x$属于到$\mathfrak{g}'$时。从 $\mathfrak{g}'$ 到 $k$ 存在非零多项式映射 $p_0, p_1$ 使得

$$
d_0(x) =c_0\Leftarrow \Rightarrow p_0(x)\not= 0,d_1(x) =c_1\Leftarrow \Rightarrow p_1(x)\not= 0
$$

由于$k$是无限的，$x\in \mathfrak{g}'$的集合 S使得$d_0(x) =c_0$和$d_1(x) =c_1$非空。 S 的每个元素在 $\mathfrak{g}'$ 都是正则。另一方面，S 是 $\mathfrak{g}'$ 的元素的集合，使得 ad$_{\mathfrak{g}}x$ 的零空间具有最小维数，因此 $\mathfrak{g}$ 中 $\mathfrak{g}'$ 的每个元素都有包含。

#### 注 3 {#lie-vii-s2-n2-rem-3 .statement tag=00UB}

$\mathfrak{g}$中的$\mathfrak{g}'$正则的元素不一定存在。如果至少存在一个，则这些元素中的集合恰好是上面证明中用S表示的集合。

### 3.嘉当子代数和正则元素

#### 定理 1 {#lie-vii-s2-thm-1 .statement tag=00UC}

设$\mathfrak{g}$为李代数。

(i) 如果$x$是$\mathfrak{g},\mathfrak{g}^0(x)$中的正则元素，则嘉当子代数是$\mathfrak{g}$中的嘉当子代数。

(ii) 如果$\mathfrak{h}$是$\mathfrak{g}$的最大幂零子代数，并且如果$x\in \mathfrak{h}$在$\mathfrak{g}$中是正则，则$\mathfrak{h}=\mathfrak{g}^0(x)$。

(iii) 如果$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数，则dim($\mathfrak{h}$)$\geq$rk($\mathfrak{g}$)。

(iv) 维数rk($\mathfrak{g}$)的$\mathfrak{g}$的嘉当子代数是$\mathfrak{g}^0(x)$，其中$x$是正则元素。

令$x$为$\mathfrak{g}$的正则元素，并令$\mathfrak{h}=\mathfrak{g}^0(x)$。显然$\mathfrak{h}^0(x) =\mathfrak{h}$。由于$x$在$\mathfrak{h}$（命题9）中是正则，rk($\mathfrak{h}$)$=$暗淡($\mathfrak{h}$)，所以$\mathfrak{h}$是幂零的。另一方面，$\mathfrak{h}=\mathfrak{g}^0(x)\supset \mathfrak{g}^0(\mathfrak{h})\supset \mathfrak{h}$，所以$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$是$\mathfrak{g}$的嘉当子代数（命题4）。这就证明了(i)。

如果$\mathfrak{h}$是$\mathfrak{g}$的最大幂零子代数，并且如果$x\in \mathfrak{h}$在$\mathfrak{g}$中是正则，则$\mathfrak{h}\subset \mathfrak{g}^0(x)$和$\mathfrak{g}^0(x)$通过(i)是幂零的，所以$\mathfrak{h}=\mathfrak{g}^0(x)$，这证明了(ii)。

如果$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数，则存在$x\in \mathfrak{h}$使得$\mathfrak{h}=\mathfrak{g}^0(x)$（命题4的Cor.1），因此dim($\mathfrak{h}$)$\geq$rk($\mathfrak{g}$)，从而证明(iii)。如果加法 dim($\mathfrak{h}$) $=$ rk($\mathfrak{g}$)$,x$ 是正则。最后，如果$x'$在$\mathfrak{g},\mathfrak{g}^0(x')$中是正则，则由(i)得到嘉当子代数，并且显然是维数rk($\mathfrak{g}$)。这就证明了(iv)。

我们将在§3，Th 中看到。 2、当$k$为特征零时，$\mathfrak{g}$中的所有嘉当子代数都有维数rk($\mathfrak{g}$)。

#### 推论 1 {#lie-vii-s2-thm-1-cor-1 .statement tag=00UD}

每个李代数$\mathfrak{g}$都有嘉当子代数，$\mathfrak{g}$中的秩是嘉当子代数中最小的维数。

#### 推论 2 {#lie-vii-s2-thm-1-cor-2 .statement tag=00UE}

令 $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ 为李代数中的满同态。如果$\mathfrak{h}'$是$\mathfrak{g}'$的嘉当子代数，则存在$\mathfrak{g}$的嘉当子代数$\mathfrak{h}$使得$\mathfrak{h}'=f(\mathfrak{h})$。

让$\mathfrak{a}=f^{-1}(\mathfrak{h}')$。由科. $1,\mathfrak{a}$有嘉当子代数$\mathfrak{h}$。由科. $4,f(\mathfrak{h}) =\mathfrak{h}'$ 提案 2。我们证明$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数。令$\mathfrak{n}$为$\mathfrak{g}$中$\mathfrak{h}$的归一化器。足以证明$\mathfrak{h}=\mathfrak{n}$。如果$x\in \mathfrak{n},f(x)$属于是$\mathfrak{g}'$中$\mathfrak{h}'$的归一化器，那么$f(x)\in \mathfrak{h}'$和$x\in \mathfrak{a}$；但是 $\mathfrak{h}$ 是 $\mathfrak{a}$ 中它自己的标准化器，所以$x\in \mathfrak{h}$。

#### 推论 3 {#lie-vii-s2-thm-1-cor-3 .statement tag=00UF}

每个李代数 $\mathfrak{g}$ 都是其嘉当子代数的和。

The sum $\mathfrak{s}$ of the Cartan subalgebras of $\mathfrak{g}$ contains the set of regular elements of $\mathfrak{g}$ (Th. 1 (i)). 由于对于 Zariski 拓扑、$\mathfrak{s}=\mathfrak{g}$，集合在$\mathfrak{g}$ 中是稠密的。

#### 命题 10 {#lie-vii-s2-prop-10 .statement tag=00UG}

令$\mathfrak{g}$为$\mathfrak{g}$的李代数、$\mathfrak{a}$交换子代数以及$\mathfrak{c}$为$\mathfrak{g}$中$\mathfrak{a}$的交换子。假设所有 $x\in \mathfrak{a}$ 的 ad$_{\mathfrak{g}}x$ 为半单。那么$\mathfrak{c}$的嘉当子代数就是$\mathfrak{g}$包含于$\mathfrak{a}$的嘉当子代数。

设$\mathfrak{h}$为$\mathfrak{c}$的嘉当子代数。由于$\mathfrak{a}$包含在$\mathfrak{c},\mathfrak{a}\subset \mathfrak{z}\subset \mathfrak{h}$的中心$\mathfrak{z}$中（命题5）。令$\mathfrak{n}$为$\mathfrak{g}$中$\mathfrak{h}$的标准化。然后

$$
[\mathfrak{a},\mathfrak{n}]\subset [\mathfrak{h},\mathfrak{n}]\subset \mathfrak{h}
$$

由于 ad$_{\mathfrak{g}}x,x\in \mathfrak{a}$ 是半单并且彼此可交换，因此可以从第 1 章的代数得出。 VIII, §5, no. 1，存在$\mathfrak{n}$的向量子空间$\mathfrak{d}$在ad$_{\mathfrak{g}}\mathfrak{a}$下稳定且$\mathfrak{n}=\mathfrak{h}\oplus \mathfrak{d}$。然后$[\mathfrak{a},\mathfrak{d}]\subset \mathfrak{h}\cap \mathfrak{d}= 0$，所以$\mathfrak{d}\subset \mathfrak{c}$。因此，$\mathfrak{n}$是$\mathfrak{c}$中$\mathfrak{h}$的规范化器，因此$\mathfrak{n}=\mathfrak{h}$，因此$\mathfrak{h}$是$\mathfrak{g}$包含于$\mathfrak{a}$的嘉当子代数。

相反，令$\mathfrak{h}$为$\mathfrak{g}$包含于$\mathfrak{a}$中的嘉当子代数。然后$\mathfrak{h}=$$\mathfrak{g}^0(\mathfrak{h})\subset \mathfrak{g}^0(\mathfrak{a})$，再到假设$\mathfrak{g}_0(\mathfrak{a}) =\mathfrak{g}^0(\mathfrak{a}) =\mathfrak{c}$。因此，$\mathfrak{a}\subset \mathfrak{h}\subset \mathfrak{c}$和$\mathfrak{h}$是$\mathfrak{c}$的嘉当子代数（因为它等于$\mathfrak{g}$中它自己的归一化器，因此$\mathfrak{c}$中的更不必说）。

#### 命题 11 {#lie-vii-s2-prop-11 .statement tag=00UH}

令 $\mathfrak{n}$ 为李代数 $\mathfrak{g}$ 的幂零子代数。 $\mathfrak{g}^0(\mathfrak{n})$中包含$\mathfrak{g}$，存在嘉当子代数。

把$\mathfrak{a}=\mathfrak{g}^0(\mathfrak{n})$。那么 $\mathfrak{n}\subset \mathfrak{a}$ 因为 $\mathfrak{n}$ 是幂零的。如果$x\in \mathfrak{a}$，则令$P(x)$为广告$x$定义的$\mathfrak{g}/\mathfrak{a}$的自同态的行列式。用$x\in \mathfrak{a}$的$\mathfrak{a}'$集合表示$P(x)\not= 0$，它是Zariski拓扑中$\mathfrak{a}$的开子集； 关系 $x\in \mathfrak{a}'$ 和 $\mathfrak{g}^0(x)\subset \mathfrak{a}$ 等效。根据§1, no. 2的命题7(ii)，存在$y\in \mathfrak{n}$使得$\mathfrak{g}^0(y) =\mathfrak{a}$，并且存在$y\in \mathfrak{a}'$所以$\mathfrak{a}'$非空。由于$\mathfrak{a}'$是开放的，所以它的交和$\mathfrak{a}$的正则元素的集合都是非空的。令$x$为这个交的元素。那么$\mathfrak{g}^0(x)\subset \mathfrak{a}$和$\mathfrak{g}^0(x)$是$\mathfrak{a}$的嘉当子代数，因此是幂零的。另一方面，§1, no. 3的第10（i）条命题表明，$\mathfrak{g}^0(x)$是$\mathfrak{g}$自身的归一化器；因此，它是 $\mathfrak{g}$ 的嘉当子代数，从而完成证明。

### 4.嘉当子代数 / 半单李代数

#### 定理 2 {#lie-vii-s2-thm-2 .statement tag=00UI}

假设$k$的特征为0。令$\mathfrak{g}$为半单李代数，$\mathfrak{h}$嘉当子代数为$\mathfrak{g}$。那么$\mathfrak{h}$是可交换的，它的所有元素都是$\mathfrak{g}$中的半单（第I, §6, no. 3章，定义3）。

由于 $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h}),\mathfrak{h}$ 是可还原的（§1，命题 11），因此由于它是幂零的，因此可交换。另一方面，$\mathfrak{g}$到$\mathfrak{h}$的伴随表示的限制是半单（前述），所以$\mathfrak{h}$的元素是$\mathfrak{g}$中的半单 （代数，第VIII, §5, no. 1）。

#### 推论 1 {#lie-vii-s2-thm-2-cor-1 .statement tag=00UJ}

如果$x\in \mathfrak{h}$和$y\in \mathfrak{g}^{\lambda}(\mathfrak{h})$，我们有$[x, y] =\lambda (x)y$。

事实上，$\mathfrak{g}^{\lambda(x)}(x) =\mathfrak{g}_{\lambda(x)}(x)$，因为广告$x$是半单。

#### 推论 2 {#lie-vii-s2-thm-2-cor-2 .statement tag=00UK}

$\mathfrak{g}$的每个正则元素都是半单。

事实上，这样的元素属于到嘉当子代数（no. 3，Th.1（i））。

#### 推论 3 {#lie-vii-s2-thm-2-cor-3 .statement tag=00UL}

令 $\mathfrak{h}$ 为约李代数 $\mathfrak{g}$ 的嘉当子代数。

a$)\mathfrak{h}$ 是可交换的。

b) 如果$\rho$是$\mathfrak{g}$的有限维半单表示，则$\rho (\mathfrak{h})$的元素是半单。

令$\mathfrak{c}$为$\mathfrak{g}$的中心，并由$\mathfrak{s}$派生出代数。然后$\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$，所以$\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$，其中$\mathfrak{h}'$是$\mathfrak{s}$的嘉当子代数（命题2）。鉴于 Th. $2,\mathfrak{h}'$ 是可交换的，因此 $\mathfrak{h}$ 也是可交换的。此外，$\rho (\mathfrak{h}')$由半单元素组成，$\rho (\mathfrak{c})$也是如此（I, §6, no. 5章，第4章）； 断言 b)如下。

### 习题 {#lie-vii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
