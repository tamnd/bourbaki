---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 4
section_title: Classification of root systems
lang: zh
source: lie-iv-vi
pdf_pages: 0214-0246, 0255-0261
extraction: ocr
subsections:
    - "no": 1
      title: FINITE COXETER GROUPS
      page: 0
      pdf_page: 214
    - "no": 2
      title: DYNKIN GRAPHS
      page: 0
      pdf_page: 220
    - "no": 3
      title: AFFINE WEYL GROUP AND COMPLETED DYNKIN GRAPH
      page: 0
      pdf_page: 223
    - "no": 4
      title: PRELIMINARIES TO THE CONSTRUCTION OF ROOT SYSTEMS
      page: 0
      pdf_page: 225
    - "no": 5
      title: SYSTEMS OF TYPE $B_l$ ($l \geq 2$)
      page: 0
      pdf_page: 227
    - "no": 6
      title: SYSTEMS OF TYPE $C_l$ ($l \geq 2$)
      page: 0
      pdf_page: 229
    - "no": 7
      title: SYSTEMS OF TYPE $A_l$ ($l \geq 1$)
      page: 0
      pdf_page: 230
    - "no": 8
      title: SYSTEMS OF TYPE $D_l$ ($l \geq 3$)
      page: 0
      pdf_page: 233
    - "no": 9
      title: SYSTEM OF TYPE $F_4$
      page: 0
      pdf_page: 236
    - "no": 10
      title: SYSTEM OF TYPE E_8
      page: 0
      pdf_page: 238
    - "no": 11
      title: SYSTEM OF TYPE E_7
      page: 0
      pdf_page: 240
    - "no": 12
      title: SYSTEM OF TYPE E_6
      page: 0
      pdf_page: 242
    - "no": 13
      title: SYSTEM OF TYPE G_2
      page: 0
      pdf_page: 244
    - "no": 14
      title: IRREDUCIBLE NON-REDUCED ROOT SYSTEMS
      page: 0
      pdf_page: 246
statements: 19
exercises: 16
content_sha256: e8193024456062db74dc4ac501e14cf4658bccbc19e83034682ae13d48ef798b
translated_from: content/en/lie/VI/04_s4_classification_of_root_systems.md
translation_method: google
source_content_sha256: 45e10d913c1a6d6fc187b08ddce9c5ebb593714b0771388b35b7618ac35e06d7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 87ca053881d925dad55d0adf1993ce476241734709b303fd82e19dfa3a03df75
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。 根系的分类

### 1. 有限 coxeter 群

在这个截面中，我们将要确定，直到同构，所有根系，因此所有晶体群（§ 2, no. 5）。更一般地，我们首先确定有限维实数向量空间中的反射生成的所有有限群：这相当于（第 V, § 4, no. 8 章）确定所有有限 Coxeter 群，或（第 V, § 4, no. 8，第 2 章）确定有限维的所有 Coxeter 矩阵阶使得相关的双线性形式是正的且非简并的。

令 $M = (m_{ij})_{i,j \in I}$ 为有限阶 $l$ 的 Coxeter 矩阵。放

$$
q_{ij} = -\cos(\pi / m_{ij}).
$$

回想一下，$q_{ii} = 1$ 和$q_{ij} = q_{ji}$ 是零或$\leq -1/2$ $i \neq j$。放入$E = \mathbf{R}^l$，并令$(e_i)_{i \in I}$为$E$的典范基。用与$M$（第V, § 4, no. 1章）相关的$E$上的$(x|y)$双线性形式和$q$在$E$上的二次形式$x \mapsto (x|x)$表示。对于$x = \sum_{i \in I} \xi_i x_i$，

$$
\| x \| ^2 = q(x) = \sum_{i,j \in I} q_{ij} \xi_i \xi_j.
$$

用 $(X, f)$ 表示 $M$ 的 Coxeter 图（第 IV, § 1, no. 9）。如果$a$是$X$的边，则$f(a)$称为$a$的阶。

在这个数的其余部分中，由$M$（第V, § 4, no. 3章）定义的Coxeter群$W(M)$被假设是有限的，因而$q$是正的且非退化的，$X$是一个森林（第V, § 4, no. 8章，提案 8）。我们还假设$X$是连通的（在其他字中，Coxeter群$W(M)$是不可约的），因而$X$是一棵树。

从$q$为正且非退化的条件，我们将在$m_{ij}$上获得条件，这将使我们能够列出相应的 Coxeter图的所有可能性；剩下的只是证明这些可能性实际上已经实现，而在其他字中，相应的群$W(M)$是有限的。

#### 引理 1 {#lie-vi-s4-lem-1 .statement tag=0AY2}

对于所有 $i$、$\sum_{j \neq i} q_{ij}^2 < 1$。

令$J$为$j \in I$的集合，使得$q_{ij} \neq 0$，在其他字中使得$\{i, j\}$是$X$的边。如果$j, j' \in J$和$j \neq j'$，$\{j, j'\}$不是边（否则$i, j, j'$将是形式一条电路），所以$(e_j|e_{j'}) = 0$。让$F = \sum_{j \in J} \mathbf{R} e_j$。那么 $(e_j)_{j \in J}$ 是 $F$ 的正交基。从 $e_i$ 到 $F$ 的距离 $d$ 由 $d^2 = 1 - \sum_{j \in J} (e_i|e_j)^2 = 1 - \sum_{j \in J} q_{ij}^2 = 1 - \sum_{j \neq i} q_{ij}^2$ 给出，因此为引理。

#### 引理 2 {#lie-vi-s4-lem-2 .statement tag=0AY3}

$X$ 属于的任意顶点至多 3 条边。

事实上，如果$i$链接到$h$其他顶点，则这些其他顶点的关系$q_{ij}^2 \geq \frac{1}{4}$意味着$\frac{h}{4} < 1$乘以引理1，因而$h \leq 3$。

#### 引理 3 {#lie-vi-s4-lem-3 .statement tag=0AY4}

*如果 $i$ 属于为 3 个边，则这些边为阶 3。*

如果没有，鉴于关系 $\cos \frac{\pi}{4} = \frac{\sqrt{2}}{2}$，

$$
\sum_{j \neq i} q_{ij}^2 \geq \frac{1}{4} + \frac{1}{4} + (\frac{\sqrt{2}}{2})^2 = 1
$$

这是不可能的（引理1）。

#### 引理 4 {#lie-vi-s4-lem-4 .statement tag=0AY5}

*如果存在阶$\geq 6$的边，则$l = 2$。*

事实上，让 $\{i, j\}$ 成为这样的一条边。如果$l > 2$，边$i, j$（例如$i$）之一将链接到第三个顶点$j'$，因为$X$连通。鉴于关系 $\cos \frac{\pi}{6} = \frac{\sqrt{3}}{2}$ 我们将有

$$
\sum_{k \neq i} q_{ik}^2 \geq \frac{1}{4} + (\frac{\sqrt{3}}{2})^2 = 1
$$

这是不可能的（引理1）。

#### 引理 5 {#lie-vi-s4-lem-5 .statement tag=0AY6}

*顶点不能属于到阶$\geq 4$的两条不同边。*

令$i$为这样一个顶点。我们会有 $\sum_{j \neq i} q_{ij}^2 \geq (\frac{\sqrt{2}}{2})^2 + (\frac{\sqrt{2}}{2})^2 = 1$，这是不可能的 (引理 1)。

令$\{i, j\}$为$X$的一条边。我们将得到定义一个新的 Coxeter 图，它将从 $M$ *通过识别* $i$ *和* $j$ 的图获得。其顶点的集合$I'$是通过识别$i$和$j$得到的$I$中的商。将$p = \{i, j\}$（即$I'$的元素）和$I$的认同元素与$i$和$j$及其典范像放入$I'$不同。令$k, k'$是$I'$的两个不同的元素。那么，在以下情况下，$\{k, k'\}$就是新图的一条边：

1) $k$和$k'$与$p$不同，$\{k, k'\}$是$X$的一条边：在这种情况下，该边的阶定义为$m_{kk'}$：

2）$k = p$，集合$\{i, k'\}, \{j, k'\}$之一是$X$的一条边；如果$\{i, k'\}$是$X$的边，$\{p, k'\}$的阶被定义为$m_{ik'}$，如果$\{j, k'\}$是$X$的边，则定义为$m_{jk'}$（这两种可能性是互斥的，因为$X$是一棵树）。

令 $M' = (m'_{ij})_{i,j \in I'}$ 为如此定义的新 Coxeter 矩阵，并放入 $q'_{ij} = -\cos \frac{\pi}{m'_{ij}}$。然后，对于$k \neq p$，$t'_{pk} = q_{ik} + q_{jk}$。因此，如果$(\xi_i) \in \mathbf{R}^{I'}$，

$$
\sum_{k, k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} + \xi_p^2 - \xi_i^2 - \xi_j^2 - 2q_{ij} \xi_i \xi_j \tag{1}
$$
$$
= \sum_{k, k' \in I} q_{kk'} \xi_k \xi_{k'} - (1 + 2q_{ij}) \xi_p^2.
$$

#### 引理 6 {#lie-vi-s4-lem-6 .statement tag=0AY7}

*如果 $\{i, j\}$ 为阶 3，则 $W(M')$ 是有限 Coxeter 群。*

事实上，$q_{ij} = -\frac{1}{2}$，所以 (1) 变成

$$
\sum_{k,k' \in I'} q'_{kk'} \xi_k \xi_{k'} = \sum_{k,k' \in I} q_{kk'} \xi_k \xi_{k'}
$$

$(\xi_k)_{k \in I'} \mapsto \sum_{k,k' \in I'} q'_{kk'} \xi_k \xi_{k'}$ 是正非简并二次形式。
现在应用 Th 就足够了。第 2 章V。 § 4, no. 8。

#### 引理 7 {#lie-vi-s4-lem-7 .statement tag=0AY8}

我们有以下其中一项：

a) X 具有独特的分支点（第 IV、附录、no. 1 章）。并且 X 的所有边都是阶 3。
b) X 是一条链，最多有阶 $\geq 4$ 的一条边。

我们在l上通过归纳争论。

a) 假设 X 具有分支点 i。然后我属于到阶3的3条边。$\{i, k_1\}, \{i, k_2\}, \{i, k_3\}$（引理2和3）。若$l = 4$引理得证。如果不是，则将 $k_1$（例如属于）连接到与刚才提到的边不同的边，因为 X 连通。 M 的 Coxeter 图中的认同 i 和 $k_1$。鉴于引理 6，这给出了可以应用归纳假设的新图。现在 i 的像 $p$ 是新图 $X'$ 的分支点。因此$X'$没有其他分支点，并且它的所有边都是阶3。因此X的所有边都是阶3，而i和$k_1$是它唯一可能的分支点。但是，如果 $k_1$ 是X 的点，则$p$ 将属于扩展到$X'$ 中的至少 4 个边，这与引理 2 相反。

b) 假设X没有影响点。那么X是一条链（第IV，附录，no. 3，第3条命题）。令$\{i, j\}$为阶$\geq 4$的边。如果 $l = 2$，引理是微不足道的。如果不是，那么我说，属于到带有$k \neq j$的边$\{i, k\}$（因为X已连接）。这条边的长度为阶 3 (引理 5)。 M的Coxeter图中的认同i和k。通过引理6，可以应用归纳假设。令 $p$ 为新图 $X'$ 中 i 的像。在$X'$中，$\{p, j\}$是阶$\geq 4$的一条边，因此$X'$没有阶$\geq 4$的其他边，因此$\{i, j\}$是阶$\geq 4$的唯一边X。

#### 引理 8 {#lie-vi-s4-lem-8 .statement tag=0AY9}

令$i_1, i_2, \ldots, i_p$为X的顶点，使得$\{i_1, i_2\}, \{i_2, i_3\}, \ldots, \{i_{p-1}, i_p\}$为阶3的边。然后为$q(\sum_{r=1}^p r e_{i_r}) = \frac{1}{2} p(p+1)$。

如果$s > r + 1$，我们有$(e_{i_r}|e_{i_r}) = 1, (e_{i_r}|e_{i_{r+1}}) = -\frac{1}{2}, (e_{i_r}|e_{i_s}) = 0$。因此

$$
q(\sum_{r=1}^p r e_{i_r}) = \sum_{r=1}^p r^2 - 2 \sum_{r=1}^{p-1} \frac{1}{2} r(r+1) = p^2 - \sum_{r=1}^{p-1} r.
$$

集合论，第 1 章III。 § 5, no. 8。科。根据提案 14，这等于

$$
p^2 - \frac{1}{2} p(p-1) = \frac{1}{2} p(p+1).
$$

#### 引理 9 {#lie-vi-s4-lem-9 .statement tag=0AYA}

假设 X 是一条具有顶点 1, 2, ..., l 和边 {1, 2}, {2, 3}, ..., {l - 1, l} 的链。

(i) 如果边 {2, 3}, {3, 4}, ..., {l - 2, l - 1} 之一的大小为阶 $\geq 4$，则该边的大小为阶 4，并且图形如下：

![具有 4 个节点连接成链的图](../images/chain_4.png)

(ii) 如果边 {1, 2} 的大小为阶 5，则该图为以下之一：

![具有 5 个节点以链连接的图](../images/chains_5.png)

我们可以假设 $l > 2$ (引理 4)。假设$\{i, i + 1\}$是阶$\geq 4$，还有$1 \leq i \leq l - 1$。放

$$
x = e_1 + 2e_2 + \cdots + ie_i,\ y = e_i + 2e_{l-1} + \cdots + (l - i)e_{i+1}, \text{ and } j = l - i.
$$

引理 8、$\| x \| ^2 = \frac{1}{2} i(i + 1)$、$\| y \| ^2 = \frac{1}{2} j(j + 1)$。另一方面，$(x|y) = ij(e_i|e_{i+1}) = -ij \cos \frac{\pi}{m}$ 与 $m = 4$ 或 5 (引理 4)。现在

$$
(x|y)^2 < \| x \| ^2 \| y \| ^2.
$$

这给出了

$$
\frac{1}{4} ij(i + 1)(j + 1) > i^2 j^2 \cos^2 \frac{\pi}{m}
$$

所以

$$
(i + 1)(j + 1) > 4ij \cos^2 \frac{\pi}{m} \geq 2ij.
$$

首先，给出$ij - i - j - 1 < 0$，或$(i - 1)(j - 1) < 2$。如果

$$
1 < i < l - 1,
$$

然后$1 < j < l - 1$，所以$i = j = 2$，所以$^1$

$$
9 > 16 \cos^2 \frac{\pi}{m}, \text{ thus } \cos^2 \frac{\pi}{m} < \cos^2 \frac{\pi}{5}
$$

因此$m = 4$。这就证明了(i)。如果$i = 1$和$m = 5$，则$2j + 2 > 4j \frac{3+\sqrt{5}}{8}$，或$j \frac{\sqrt{5}-1}{2} < 2, j < \sqrt{5} + 1 < 4$，等等$l = j + 1 \leq 4$。这就证明了(ii)。

$^1$ 1 中与 1 不同的第 5 个根是 $z^4 + z^3 + z^2 + z + 1 = 0$ 中的解。代入$x = \frac{1}{2}(z + \frac{1}{z})$，这个方程就变成了$(2x)^2 - 2 + 2x + 1 = 0$，或者$4x^2 + 2x - 1 = 0$，所以$x = \frac{-1 \pm \sqrt{5}}{4}$。因此，

$$
2 \cos^2 \frac{\pi}{5} - 1 = \cos \frac{2\pi}{5} = \frac{\sqrt{5} - 1}{4}, \quad \cos^4 \frac{\pi}{5} = \frac{3 + \sqrt{5}}{8} > \frac{5}{8} > \frac{9}{16}, \quad \cos \frac{\pi}{5} = \frac{1 + \sqrt{5}}{4}.
$$

#### 引理 10 {#lie-vi-s4-lem-10 .statement tag=0AYB}

如果X有分支点i，则完整子图X - {i}是三个链的并，并且如果p - 1，q - 1，r - 1是这些链的长度，则三元组{p，q，r}等于三元组之一，直到置换 {1, 2, 2}，{1, 2, 3}，{1, 2, 4}，{1, 1, m}（对于某些 m $\geq 1$）。

顶点 i 属于到 3 条边 (引理 2)，并且没有其他分支点 (引理 7)，因此完整子图 X - {i} 是 3 个链 X_1、X_2、X_3 的和，每个链都有一个链接到 i 的终端顶点X。令 {i_1, i_2}, {i_2, i_3}, ..., {i_{p-1}, i_p} 为 X_1 的边，{j_1, j_2}, {j_2, j_3}, ..., {j_{q-1}, j_q} 为 X_2 的边，{k_1, k_2}, {k_2, k_3}, ..., {k_{r-1}， k_r} X_3 的那些，其中 i_1、j_1、k_1 链接到 X 中的 i。我们可以假设$p \geq q \geq r \geq 1$。放

$$
x = e_{i_p} + 2e_{i_{p-1}} + \cdots + pe_{i_1}
$$
$$
y = e_{j_q} + 2e_{j_{q-1}} + \cdots + qe_{j_1}
$$
$$
z = e_{k_r} + 2e_{k_{r-1}} + \cdots + re_{k_1}.
$$

由于 X 的所有边都是阶 3 (引理 7)，引理 8 给出 $\| x \| ^2 = \frac{1}{2} p(p+1)$、$\| y \| ^2 = \frac{1}{2} q(q+1)$、$\| z \| ^2 = \frac{1}{2} r(r+1)$。另一方面，$e_i$与$e_{i_2}, e_{i_3}, \ldots, e_{i_p}$正交，因此$(e_i | x) = p(e_i | e_{i_1}) = -\frac{1}{2} p$；同样$(e_i | y) = -\frac{1}{2} q$，$(e_i | z) = -\frac{1}{2} r$。 单位向量 $\| x \|^{-1} x, \| y \|^{-1} y, \| z \|^{-1} z$ 相互正交，$e_i$ 不属于到子空间 F 生成；从$e_i$到F的距离平方为

$$
1 - (e_i | \frac{x}{\| x \|})^2 - (e_i | \frac{y}{\| y \|})^2 - (e_i | \frac{z}{\| z \|})^2
$$
$$
= 1 - \frac{1}{2} \frac{p}{p+1} - \frac{1}{2} \frac{q}{q+1} - \frac{1}{2} \frac{r}{r+1}
$$
$$
= 1 - \frac{1}{2} + \frac{1}{2} \frac{1}{p+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{q+1} - \frac{1}{2} + \frac{1}{2} \frac{1}{r+1}.
$$

由于这个数量 > 0，我们有

$$
(p+1)^{-1} + (q+1)^{-1} + (r+1)^{-1} > 1.
$$ (4)

因此$3(r+1)^{-1} > 1$，所以$r < 2$，最后$r = 1$。然后 (4) 给出

$$
(p+1)^{-1} + (q+1)^{-1} > \frac{1}{2}
$$ (5)

因此$2(q+1)^{-1} > \frac{1}{2}$，所以$q \leq 2$。最后，如果 $q = 2$，(5) 给出

$$
(p+1)^{-1} > \frac{1}{6}. \quad \text{hence } p \leq 4.
$$

#### 定理 1 {#lie-vi-s4-thm-1 .statement tag=0AYC}

任何不可约有限 Coxeter 系统 (W, S) 的图同构于以下之一：

A_l (l \geq 1\ 顶点)
B_l (l \geq 2\ 顶点)
D_l (l \geq 4\ 顶点)
E_6
E_7
E_8
F_4 4
G_2 6
H_3 5
H_4 5
I_2(p) p (p = 5\ 或\ p \geq 7)。

这些图中没有两个是同构的。

事实上，令 W = (m_{ij}) 为 (W, S) 的 Coxeter 矩阵，并令 l = Card(S)。如果其中一个 m_{ij} 为 \geq 6，则 l = 2 (引理 4)，并且 (W, S) 的 Coxeter 图为型 G_2 或 I_2(p)，p \geq 7。现在假设所有 m_{ij} \leq 5。

a) 如果 m_{ij} 不全部等于 3，则 (W, S) 的图 X 是一个链，并且 m_{ij} 中恰好有一个等于 4 或 5 (引理 7)。如果 m_{ij} 之一等于 5，则引理 9 表明我们有型 H_3、H_4 或 I_2(5) 之一。如果 m_{ij} 之一等于 4，则引理 9 表明我们有型 B_1 或 F_4 之一。

b) 现在假设所有 m_{ij} 都等于 3。如果 X 是一条链，则 Coxeter 图为型 A_l。如果不是，则引理10表明它是型E_6、E_7、E_8或D_1。

显然，列出的 Coxeter 图中没有两个是同构的。

反之：

#### 定理 2 {#lie-vi-s4-thm-2 .statement tag=0AYD}

由 Th 的 Coxeter 图 A_1、B_1、...、I_2(p) 定义的 Coxeter 群。 1 是有限的。

这对于 I_2(p) 来说是清楚的，相应的群是阶 2p 的二面角群（第 IV, § 1, no. 9 章）。对于 H_4 相应的二次形式是

$$
\xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - 2(\cos \frac{\pi}{5}) \xi_3 \xi_4
$$
$$
= \xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 - \xi_1 \xi_2 - \xi_2 \xi_3 - \frac{1 + \sqrt{5}}{2} \xi_3 \xi_4
$$
$$
= (\xi_2 - \frac{\xi_1 + \xi_3}{2})^2 + (\xi_4 - \frac{1 + \sqrt{5}}{4} \xi_3)^2 + \frac{3}{4} (\xi_1 - \frac{1}{3} \xi_3)^2 + \frac{7 - 3 \sqrt{5}}{24} \xi_3^2.
$$

由于$7 - 3 \sqrt{5}$是$> 0$，所以这个形式是正非简并的，而相应的Coxeter群是有限的。这同样适用于相应的到 $H_3$，因为它与前面（第 IV, § 1, no. 8 章）的子群同构。

对于型$A_l, B_l, \ldots, G_2$，我们将构造，在第5至13号中，根系具有相应的群作为Weyl群。我们将看到这些群不仅是有限的，而且是*晶体*（§ 2, no. 5）。

### 2. 德金图

通过滥用语言，我们将调用具有以下属性的*规范图* 对 $(\Gamma, f)$：

1) $\Gamma$ 是一个图（称为 $(\Gamma, f)$ 的*底层*图）。

2) 如果$E$表示对$(i, j)$的集合，使得$\{i, j\}$是$\Gamma$的边，则$f$是从$E$到$\mathbf{R}$的映射，使得$f(i, j) f(j, i) = 1$ 对于所有$(i, j) \in E$。

规范图存在明显的概念和同构。

令 $R$ 为实向量空间 $V$ 中的约化根系。 我们将与它关联一个规范图 $(X, f)$，称为 $R$ 的 *Dynkin 图*。 $X$的顶点将是集合$\{B\} \times B$的并中集合的元素、$W(R)$的轨道$I$（其中$B$是基的集合） $R$）。 如果$N = (n_{ij})_{i,j \in I}$（或$M = (m_{ij})_{i,j \in I}$）是$R$（§ 1, no. 5，*注 7*）的规范嘉当矩阵（或Coxeter矩阵），则两个顶点$i$和$j$ $X$ 是链接的当且仅当 $n_{ij} \neq 0$ 然后我们把
$$
f(i, j) = \frac{n_{ij}}{n_{ji}}.
$$
由于$n_{ij} = 0$蕴含$n_{ji} = 0$，因此定义是一个规范图$(X, f)$。

令$(x|y)$为$V$上的标量乘积，在$W(R)$下不变，并令$B = (\alpha_i)_{i \in I}$为$R$的基，规范索引。 § 1, no. 1的公式(7)和(9)表明，图$X$的顶点$i$和$j$是链接的当且仅当
$$
(\alpha_i|\alpha_j) \neq 0
$$
还有那个
$$
f(i, j) = \frac{(\alpha_i|\alpha_i)}{(\alpha_j|\alpha_j)}.
$$

鉴于§ 1、第3和第5个结果，唯一的可能性如下，直到交换$i$和$j$：

1) $i$和$j$不相连； $n_{ij} = n_{ji} = 0; m_{ij} = 2;$
2) $f(i, j) = f(j, i) = 1; n_{ij} = n_{ji} = -1; m_{ij} = 3;$
3) $f(i, j) = 2, f(j, i) = 1/2; n_{ij} = -2, n_{ji} = -1; m_{ij} = 4;$
4) $f(i, j) = 3, f(j, i) = 1/3; n_{ij} = -3, n_{ji} = -1; m_{ij} = 6.$

由此我们可以看出，Dynkin 图 $R$ 确定 $R$ 的嘉当矩阵和 Coxeter 矩阵，因此确定 $R$ 直至同构。更准确地说，Cor。 § 1, no. 5的第15条命题意味着以下结果：

#### 命题 1 {#lie-vi-s4-prop-1 .statement tag=0AYE}

*令$R_1$和$R_2$为向量空间$V_1$和$V_2$中的两个约化根系。令$B_1 = (\alpha_i)_{i \in I_1}$和$B_2 = (\alpha_i)_{i \in I_2}$为$R_1$和$R_2$的基，按规范索引。设$\lambda$为同构，从$R_1$的Dynkin图到$R_2$的Dynkin图。那么，对于所有$i \in I_1$，存在从$V_1$到$V_2$的唯一同构，将$R_1$转换为$R_2$，将$\alpha_i$转换为$\alpha_{\lambda(i)}$。*

很明显，$R$ 的 Dynkin 图的 $R$ 定义自同构的自同构，因此同态 $\varphi$ 从群 $A(R)$ 到自同构的 Dynkin 图的群 $R$。

#### 推论 {#lie-vi-s4-n2-cor-1 .statement tag=0AYF}

*同态 $\varphi$ 通过商的传递定义了从群 $A(R)/W(R)$ 到 Dynkin 图 $R$ 的自同构群的同构。*

显然，$\varphi(g) = \mathrm{Id}$ 对于所有$g \in W(R)$。另一方面，命题1表明，在给定的基不变的情况下，从$R$的Dynkin图的同构群到$A(R)$的元素子群$E$，存在同构$\psi$。 $R$的$B$，使得$\varphi \circ \psi = \mathrm{Id}$。由于$A(R)$是$E$和$W(R)$的半直接乘积（§ 1, no. 5，命题16），因此推论紧随其后。

在实践中，Dynkin图$(X, f)$由节点和键组成的图表表示，如下所示。节点对应到$X$的顶点；在上述情况 1)、2)、3) 和 4) 中，两个节点相应的到两个不同顶点 $i$ 和 $j$ 通过 0、1、2 或 3 个键连接（最多交换 $i$ 和 $j$）。此外，在情况3)和4)中，即当$f(i, j) > 1$，或当根、$\alpha_i$和$\alpha_j$不正交并且不属于相同的长度、不等式符号$>$放置在双或连接节点的三键上时相应的到$i$和$j$面向节点相应的到$j$（即最短的根）：

$$
\begin{array}{cc}
\circ \Longrightarrow \circ & \text{(for } f(i, j) = 2 \text{).} \\
\circ \Rrightarrow \circ & \text{(for } f(i, j) = 3 \text{).}
\end{array}
$$

很明显，可以从此图表恢复Dynkin图$(X, f)$。

我们注意到，与 $W(R)$ 的 Coxeter 图相关联的图表可以通过与 $R$ 的 Dynkin 图相关联，通过保留节点和单键以及替换双（或三重）键并由数 4（或 6）超越的键来获得。相反，给定 W(R) 的 Coxeter 图，与 R 的 Dynkin 图相关的图表可以使用此过程的逆过程来恢复，除了双或三键上的不等式符号。 Th。因此，图 1 立即给出了可能的 Dynkin 图的列表。更准确地说：

#### 定理 3 {#lie-vi-s4-thm-3 .statement tag=0AYG}

*如果 R 是不可约约化根系，则其 Dynkin 图同构于以下图表表示的图之一：*

$$
\begin{array}{ll}
A_l & \circ-\cdots-\circ \quad (l \geq 1 \text{ vertices }) \\
B_l & \circ-\cdots-\circ-\circ \quad (l \geq 2 \text{ vertices }) \\
C_l & \circ-\cdots-\circ-\circ \quad (l \geq 3 \text{ vertices }) \\
D_l & \circ-\cdots-\circ-\circ-\circ \quad (l \geq 4 \text{ vertices }) \\
E_6 & \circ-\cdots-\circ \\
E_7 & \circ-\cdots-\circ-\circ-\circ \\
E_8 & \circ-\cdots-\circ-\circ-\circ-\circ \\
F_4 & \circ-\circ-\circ-\circ \\
G_2 & \circ-\circ-\circ
\end{array}
$$

*这些图中没有两个是同构的，并且存在不可约的约化根系将它们中的每一个作为其 Dynkin 图（最多同构）。*

第一个断言紧随 Th 之后。 1、鉴于前面的注，图 H_3、H_4 和 I_2(p)（对于 p = 5 和 p \geq 7）的 Coxeter 群不是晶体学的事实，以及与 Coxeter 图 F_4 相关的 Dynkin 图的双（或三重）键的两个可能的不等式(resp. G_2) 给出同构 Dynkin 图。第二个断言是明确的，第三个将根据第5至13号中执行的每个型、构造的不可约约化根系的显式构造得出。

#### 注 1 {#lie-vi-s4-n2-rem-1 .statement tag=0AYH}

图 A_1 约化为单个节点；我们也用 B_1 或 C_1 表示它。图 B_2 \circ-\circ-\circ-\circ 也用 C_2 表示。图 A_3 \circ-\cdots-\circ 也用 D_3 表示。最后，D_2 表示两个不连接节点的图由……组成。 （这些约定源自相应的根系、cf.第5至8个属性。）

#### 注 2 {#lie-vi-s4-n2-rem-2 .statement tag=0AYI}

如果(X,f)是约化根系R的Dynkin图，则逆系的Dynkin图可以用(X,f^{-1})来标识。在其他字中，与R^-的Dynkin图相关联的图表可以通过与R的Dynkin图相关联的不等式符号反转来获得。如果 R 是不可约的，我们看到 R 与 R^- 除非同构，R 属于型 B_l 或 C_l，在这种情况下，R^- 属于型 C_l 或 B_l。

### 3. Affine Weyl 群和完整的 dynkin 图

令 R 为不可约约化根系，令 (X, f) 为其 Dynkin 图。我们将得到定义另一个范数图 (\tilde{X}, \tilde{f})，我们将其称为 R 的完整 Dynkin 图。 \tilde{X} 顶点的集合 \tilde{I} 由集合 I 组成X 的顶点和用 0 表示的顶点，而不是属于到 I。到 R 的定义 \tilde{f}、选择基 B = (\alpha_i)_{i \in I} 和标量乘积 \langle x | W(R) 下 y \rangle 不变。设 \alpha_0 为 B 定义的阶的最高根的负数。 \in \tilde{I} 中的两个不同顶点 i, j 相连当且仅当 \langle \alpha_i | \alpha_j \rangle \neq 0 然后我们把

$$
\tilde{f}(i, j) = \frac{\langle \alpha_i | \alpha_i \rangle}{\langle \alpha_j | \alpha_j \rangle}.
$$

正是直接的这样定义的图\tilde{X}和映射\tilde{f}不依赖于B的选择或标量乘积。

若R的秩l等于1，则I=\{i\}且\alpha_0=-\alpha_1；因此 \tilde{f}(0, i) = 1。如果 l \geq 2，\alpha_0 不与 \alpha_i 和 \langle \alpha_0 | 中的任何一个成比例。 \alpha_i \rangle 为 \leq 0 （§ 1, no. 8，命题 25）。对于 \tilde{I} 的不同元素的任何对 (i, j)，唯一的可能性是前面数中由 1), 2), 3), 4) 表示的那些（例如，n_{0i} = n(\alpha_0, \alpha_i) 和 m_{0i} = 阶 s_{\alpha_0} s_{\alpha_i} 对于所有 i \in I)。

在 l \geq 2 的情况下，完整的 Dynkin 图由图表表示，其约定与前面的数、有时相同，用虚线表示连接顶点 0 和其他顶点的键。我们注意到，这样的键上的不等式符号>，如果存在的话，总是指向不同于0的顶点，因为\alpha_0是最长的根（§ 1, no. 8，命题25）。图 (X, f) 是 (\tilde{X}, \tilde{f}) 删除顶点 0 得到的子图。

A(R) 的作用在 (X, f) 扩展到作用在 (\tilde{X}, \tilde{f}) 上，保持 0 固定，而 W(R) 在 (\tilde{X}, \tilde{f}) 上作用很简单。

我们保留§ 2的记号、§ 2, no. 2的第5号提案以及Th。第 1 章V, § 3, no. 2，表明仿射 Weyl 群 W_a(R) 的 Coxeter 图 \Sigma 可以通过与从 (X, f) 获得 W(R) 的 Coxeter 图相同的规则从 (\tilde{X}, \tilde{f}) 获得。 另一方面，令 G 为 W_a(R) (§ 2, no. 3) 的归一化器。 对于 \Sigma 的任何 g \in G 对应自同构 \varphi(g) 且 \varphi(g) = \mathrm{Id} 如果 g \in W_a(R)。 相反，根据第 11 章的 Prop. 11，给定自同构 \lambda of \Sigma，则有。 V, § 4, no. 9, 唯一元素 g = \psi(\lambda) 保留给定的凹室C，并且使得 \varphi(g) = \lambda。 由于G是元素的子群G_C的半直接乘积，保留C和W_a(R)(§ 2, no. 3)，我们通过从G/W_a（或从G_C）到商同构推导出\varphi定义到自动（\西格玛）。 直接的同构与从 A(R)/W(R) 到 G/W_a 的规范映射重合与同态从 A(R)/W(R) 到 Aut(\Sigma) 由同态从 A(R)/W(R) 诱导到Aut(\tilde{X}, \tilde{f}) 定义如上。 由 § 2, no. 3，群 Aut(\Sigma) 同构于 的半直接乘积

A(R)/W(R) 通过 P(R^*)/Q(R^*)。 P(R^*)/Q(R^*) 与群 $I_C = G_C \cap W'_a$ 同构（§ 2, no. 3 的记号）：Aut($\Sigma$) 的元素相应的到 $I_C$ 的元素 $\gamma_i$ 变换顶点0到$\Sigma$的顶点$i$。

#### 注 {#lie-vi-s4-n3-rem-1 .statement tag=0AYJ}

可以证明规范的映射
$$
\operatorname{Aut}(\tilde{X}, \tilde{f}) \to \operatorname{Aut}(\Sigma)
$$
是同构。

#### 定理 4 {#lie-vi-s4-thm-4 .statement tag=0AYK}

令 (W, S) 为不可约 Coxeter 系统，且 S 有限。当且仅当 (W, S) 的 Coxeter 图与以下之一同构时，相关的二次形式（第 V, § 4, no. 1 章）为正且简并：

$$
\begin{array}{ll}
\tilde{A}_1 & \circ \longrightarrow \infty \\
\tilde{A}_l \quad (l \geq 2) & \circ \longrightarrow \cdots \longrightarrow \circ \quad \text{(circuit with } l + 1 \text{ vertices)} \\
\tilde{B}_2 & \circ \longrightarrow 4 \longrightarrow \circ \\
\tilde{B}_l \quad (l \geq 3) & \circ \longrightarrow \cdots \longrightarrow \circ \longrightarrow 4 \quad \text{(l + 1 vertices)} \\
\tilde{C}_l \quad (l \geq 3) & \circ \longrightarrow 4 \longrightarrow \cdots \longrightarrow 4 \quad \text{(l + 1 vertices)} \\
\tilde{D}_l \quad (l \geq 4) & \circ \longrightarrow \cdots \longrightarrow \circ \quad \text{(l + 1 vertices)} \\
\tilde{E}_6 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{E}_7 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{E}_8 & \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \longrightarrow \circ \\
\tilde{F}_4 & \circ \longrightarrow \circ \longrightarrow 4 \longrightarrow \circ \\
\tilde{G}_2 & \circ \longrightarrow 6 \longrightarrow \circ
\end{array}
$$

这些 Coxeter 图中没有两个是同构的。

由章。 V, § 4, no. 9 和 § 2, no. 5 的第 8 条，二次形式为正且退化的 Coxeter 系统是对应到不可约约化根系的仿射 Weyl 群的那些。因此，定理是根据第 7 号中完成的 Dynkin 图的确定得出的。下面5至13。

### 4. 根系构造的预赛

令V为维数$l \geq 1$的实向量空间，配备标量乘积$(x|y)$，L为V的离散子群，$\Lambda$为集合的有限集合数 > 0，且 $\alpha \in L$ 的 R 集合使得 $(\alpha|\alpha) \in \Lambda$。假设 R 生成 V，并且对于 R 的点中的任意对 $(\alpha, \beta)$，数 $2 \frac{(\alpha|\beta)}{(\alpha|\alpha)}$ 为整数。那么，R*是根系*V。事实上，R 显然满足 (RS_I)。设 $\alpha \in R$；设$s_{\alpha}$为正交反射$x \mapsto x - 2 \frac{(x|\alpha)}{(\alpha|\alpha)} \alpha$：那么，如果$\beta \in R$，我们有$2 \frac{(\beta|\alpha)}{(\alpha|\alpha)} \in \mathbf{Z}$，所以$s_{\alpha}(\beta) \in L$，还有$\| s_{\alpha}(\beta) \| = \| \beta \|$，所以$s_{\alpha}(\beta) \in R$；因此，R满足(RS_{II})和(RS_{III})，并且如果$\Lambda$不包含形式$\lambda$和$4\lambda$中的两个数，则R被减小。

现在令 V 为 $E = \mathbf{R}^n$ 的子空间。令$(\varepsilon_1, \ldots, \varepsilon_n)$为E的典范基；我们通过标量乘积为 E 配备标量乘积，其中基是正交的，并为 E 配备认同 $E^*$（分别为 $V^*$ 和 V）。我们对 E 定义子群 $L_0, L_1, L_2, L_3$ 如下：

1) $L_0$ 是带有基 $(\varepsilon_i)$ 的 $\mathbf{Z}$ 模块。我们为所有 $\alpha, \beta \in L_0$ 提供了 $(\alpha|\beta) \in \mathbf{Z}$。 向量 $\alpha \in L_0$，其中 $(\alpha|\alpha) = 1$ 是 $\pm \varepsilon_i$ ($1 \leq i \leq n$)；那些$(\alpha|\alpha) = 2$是$i < j$的$\pm \varepsilon_i \pm \varepsilon_j$（$\pm \varepsilon_i \pm \varepsilon_j$中的两个符号$\pm$是彼此独立选择的；我们在截面的其余部分采用类似的约定）。

2) $L_1$是$x = \sum_{i=1}^n \xi_i \varepsilon_i \in L_0$的$L_0$由……组成的$\mathbf{Z}$子模，使得$\sum_{i=1}^n \xi_i$是偶数；由于$\xi_i$和$\xi_i^2$具有相同的奇偶性，这相当于要求$(x|x)$是偶数。设$L_1'$为$\varepsilon_i \pm \varepsilon_j$生成的$L_1$中的子模；我们有$\sum_{i=1}^n \xi_i \varepsilon_i \equiv (\sum_{i=1}^n \xi_i) \varepsilon_n \pmod{L_1'}$，从$2\varepsilon_n = (\varepsilon_1 + \varepsilon_n) - (\varepsilon_1 - \varepsilon_n) \in L_1'$开始，就有$L_1' = L_1$。由于$L_0$是由$L_1$和$\varepsilon_1$生成的，$L_0/L_1$与$\mathbf{Z}/2\mathbf{Z}$同构的。

3）$L_2 = L_0 + \mathbf{Z}(\frac{1}{2} \sum_{i=1}^n \varepsilon_i)$。显然，V的元素$x = \sum_{i=1}^n \xi_i \varepsilon_i$在$L_2$中当且仅当
$$
2\xi_i \in \mathbf{Z}, \quad \xi_i - \xi_j \in \mathbf{Z} \text{ for all } i \text{ and } j.
$$
从$(\varepsilon_k | \frac{1}{2} \sum_{i=1}^n \varepsilon_i ) = \frac{1}{2}$开始，对于所有$k$，从$\| \frac{1}{2} \sum_{i=1}^n \varepsilon_i \| ^2 = \frac{n}{4}$开始，如果$n$是偶数，我们对$\alpha, \beta \in L_2$有$(\alpha|\beta) \in \frac{1}{2}\mathbf{Z}$。 群 $L_2/L_0$ 与 $\mathbf{Z}/2\mathbf{Z}$ 同构的。

4）$L_3 = L_1 + \mathbf{Z} (\frac{1}{2} \sum_{i=1}^n \varepsilon_i )$。如果 $n$ 是 4 中的倍数，$L_3$ 是 $\sum_{i=1}^n \xi_i \varepsilon_i$ 满足 (6) 和条件 $\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$ 中的集合：在这种情况下，$(\alpha|\beta) \in \mathbf{Z}$ 对于所有 $\alpha, \beta \in L_3$。

与$L_0$（或$L_1, L_2$）关联的E 的子群是直接的，是$L_0$（或$L_2, L_1$）。与 $L_3$ 伴随的 E 的子群是集合

$$
x := \sum_{i=1}^n \xi_i \varepsilon_i \in L_2
$$

使得$(x| \frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in \mathbf{Z}$，即$\sum_{i=1}^n \xi_i \in 2\mathbf{Z}$：如果$n \equiv 0 \pmod{4}$，则该关联的子群因此是$L_3$。

阿贝尔的群 $L_2/L_1$ 是阶 4，因此与 $\mathbf{Z}/4\mathbf{Z}$ 或 $\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$ 同构的（代数，第 VII, § 4, no. 6，第 3 章）。如果$n$是奇数，

$$
p(\frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in L_1 \Leftrightarrow p \equiv 0 \pmod{4}
$$

所以$L_2/L_1$是阶 4的循环。如果$n$是偶数，

$$
p(\frac{1}{2} \sum_{i=1}^n \varepsilon_i ) \in L_1 \Leftrightarrow p \equiv 0 \pmod{2}
$$

所以$L_2/L_1$，其中包含阶 2 中两个不同的元素，与$\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$同构的。

我们将在接下来的九个项目中使用这个记号。和在盘子里。对于 Th 中 Dynkin 图的每个型。 3、我们要明确描述：

(I) 根系 R 和根的数。
R 的 (II) 基 B，且相应的正根。 基 B 将由整数 1, ..., l 索引。
（III）考克斯特数小时（§ 1, no. 11）。
(IV) 最高根 $\tilde{\alpha}$（对于 B 定义的阶）和完整的 Dynkin 图 (no. 3)。我们将在 B 的每个顶点相应的根旁边注明。
(V) 逆系 $R^-$，规范双线性形式和常数$\gamma(R)$ (§ 1, no. 12)。
(VI) 相对于 B (§ 1, no. 10) 的基本权。
正根的 (VII) 和。
(VIII) 群 P(R)、Q(R)、P(R)/Q(R) 以及连接指标 (§ 1, no. 9)。
W(R) 的 (IX) 指数（第V, § 6, no. 2章，定义 2）。在情况 A_l、B_l、C_l 和 D_l 中，我们确定对称不变量。
W(R) 的 (X) 阶（在某些情况下为结构）。

(XI) 群 $A(R)/W(R)$，其在 Dynkin 图上的作用，以及 $W(R)$ 的元素 $w_0$ 即变换 $B$ 至 $-B$。

已完成的 Dynkin 图上的 $P(R^-)/Q(R^-)$ 的 (XII) 作用，以及 $P(R^-)/Q(R^-)$ 上的 $A(R)/W(R)$ 作用。

对于 Th 中的每个 Dynkin 图。 3、这些数据将被收集在板块I至IX中，并按照上述统一方式排序。我们还给予：

(XIII) 嘉当矩阵，从中导出 Dynkin 图，如no. 2 中所述。

### 5. 系统型 $B_l$ ($l \geq 2$)

(I) 我们在$V = \mathbf{R}^l$ (no. 4) 中考虑群 $L_0$。令$R$为$\alpha \in L_0$的集合，使得$(\alpha|\alpha) = 1$或$(\alpha|\alpha) = 2$，在向量$\pm \varepsilon_i$（$1 \leq i \leq l$）和$\pm \varepsilon_i \pm \varepsilon_j$的其他字集合中（$1 \leq i < j \leq l$）。很明显，对于所有 $\alpha, \beta \in R$，$R$ 生成 $V$ 和 $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$。因此，$R$ 是$V$ (no. 4) 中的约化根系。 根中的数是$n = 2l + 4^{l(l-1)/2} = 2l^2$。

(II) 放

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3,\ldots,\alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_1,\ \alpha_l = \varepsilon_l.
$$

然后

$$
\varepsilon_i = \alpha_i + \alpha_{i+1} + \cdots + \alpha_l \quad (1 \leq i \leq l)
$$
$$
\varepsilon_i + \varepsilon_j = (\alpha_i + \alpha_{i+1} + \cdots + \alpha_l) + (\alpha_j + \alpha_{j+1} + \cdots + \alpha_l) \quad (1 \leq i < j \leq l)
$$
$$
\varepsilon_i - \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} \quad (1 \leq i < j \leq l).
$$

因此$(\alpha_1, \alpha_2, \ldots, \alpha_l)$是$R$的基（§ 1, no. 7，第20号提案的Cor.3）。此外，$i < l$为$\| \alpha_i \|^2 = 2$，$\| \alpha_l \|^2 = 1$，$(\alpha_i|\alpha_{i+1}) = -1$为$1 \leq i \leq l-1$，$(\alpha_i|\alpha_j) = 0$为$j > i + 1$：$R$的Dynkin图因此为型$B_l$，这表明$R$是不可约的。正的根是$\varepsilon_i$和$\varepsilon_i \pm \varepsilon_j$（$i < j$）。

(III) 作者：Th.第 1 章第 1(ii) 节V, § 6, no. 2,

$$
h = n/l = 2l.
$$

(IV)设$\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + 2\alpha_3 + \cdots + 2\alpha_l$，即根。其坐标和相对于基$(\alpha_i)$的坐标为$2l - 1 = h - 1$。鉴于§ 1, no. 11第31号提案，$\tilde{\alpha}$是$R$的最高根。我们有 $(\tilde{\alpha}|\alpha_i) = 0$ 对应 $i \neq 2$ 和 $(\tilde{\alpha}|\alpha_2) = 1$。由于当$l = 2$（或$l \geq 3$）时，$\alpha_2$为长度 1（或$\sqrt{2}$），$R$的完整Dynkin图如下：

$l = 2$

$$
\begin{array}{c}
\alpha_2 \\
\alpha_1
\end{array}
$$

$l \geq 3$

$$
\begin{array}{cccccc}
\alpha_1 & & & & & \\
& \alpha_2 & \alpha_3 & \cdots & \alpha_{l-1} & \alpha_l
\end{array}
$$

(V)公式$\alpha^- = \frac{2\alpha}{(\alpha|\alpha)}$给出向量$\pm 2\varepsilon_i$($1 \leq i \leq l$)、$\pm \varepsilon_i \pm \varepsilon_j$($1 \leq i < j \leq l$)的$R^-$集合。 $R^-$ 的 Dynkin 图是通过no. 2 中解释的过程从$R$ 的 Dynkin 图获得的，我们看到 $R^-$ 是型 $C_l$。

与$\beta = \varepsilon_1$不正交的有$4l - 2$根，即$\pm \varepsilon_1$和$\pm \varepsilon_1 \pm \varepsilon_j$对应$2 \leq j \leq l$；对于每个这样的根$\alpha$，$n(\alpha, \beta) = \pm 2$。 § 1, no. 12的公式(17)表明，对于$\Phi_R$，$\beta$的长度的平方是$(4l - 2)^{-1}$：因此$\Phi_R(x, y) = (x|y)/(4l - 2)$。将§ 1, no. 12 中的公式 (18) 与$x = y = \beta$ 一起应用。这给出了
$$
2 + \frac{1}{4}(4l - 4) = \gamma(R) \frac{1}{4l - 2}
$$
所以$\gamma(R) = (l + 1)(4l - 2)$。

(VI) 权 $\omega_i$ ($1 \leq i \leq l$) 使得$(\omega_i|\alpha_j) = \delta_{ij}$很容易计算，我们发现
$$
\begin{align*}
\omega_i &= \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
&= \alpha_1 + 2\alpha_2 + \cdots + (i - 1)\alpha_{i-1} + i(\alpha_1 + \alpha_{i+1} + \cdots + \alpha_l) \quad (i < l) \\
\omega_l &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l) = \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + l\alpha_l).
\end{align*}
$$

(VII) 和的正根是
$$
\begin{align*}
2\rho &= (2l - 1)\varepsilon_1 + (2l - 3)\varepsilon_2 + \cdots + 3\varepsilon_{l-1} + \varepsilon_l \\
&= (2l - 1)\alpha_1 + 2(2l - 2)\alpha_2 + \cdots + i(2l - i)\alpha_i + \cdots + l^2\alpha_l.
\end{align*}
$$

(VIII) 我们有$Q(R) = L_0$ (no. 4)，$P(R)$由$Q(R)$和$\omega_l$生成，因此等于$L_2$ (no. 4)。因而，$P(R)/Q(R)$与$\mathbf{Z}/2\mathbf{Z}$同构的，并且连接指标等于2。

(IX) 和 (X) 在 $\mathbf{R}^l$ 中，正交反射 $s_{\varepsilon_i, -\varepsilon_j}$ ($i \neq j$) 互换 $\varepsilon_i$ 和 $\varepsilon_j$，并且当指标 $k$ 不同于时，使 $\varepsilon_k$ 不变$i$ 和 $j$。 $s_{\varepsilon_i, -\varepsilon_i}$ 生成群 $G_1$ 同构于对称的群 $S_l$。当指标 $k$ 与 $i$ 不同时，正交反射 $s_{\varepsilon_i}$ 变换 $\varepsilon_i$ 到 $-\varepsilon_i$ 并使 $\varepsilon_k$ 保持不变。 $s_{\varepsilon_i}$ 生成群 $G_2$ 同构于 $(\mathbf{Z}/2\mathbf{Z})^l$。 Weyl 群 $W(R)$ 由$G_1$ 和$G_2$ 生成，$G_2$ 在$W(R)$ 中是正规的，因而$W(R)$ 与$G_l$ 的半直接乘积与$(\mathbf{Z}/2\mathbf{Z})^l$ 同构的。因此它的阶是$2^l.l!$。

对称的代数$S(\mathbf{R}^l)$可以与$\mathbf{R}^l$上的多项式函数$P(\xi_1, \ldots, \xi_l)$的代数进行规范地识别。为了使这样的多项式在 $W(R)$ 下保持不变，首先需要满足以下条件：
$$
P(\xi_1, \xi_2, \ldots, \xi_l) = P(\pm \xi_1, \pm \xi_2, \ldots, \pm \xi_l)
$$
对于右侧所有选择的符号，因而
$$
P(\xi_1, \ldots, \xi_l) = Q(\xi_1^2, \ldots, \xi_l^2)
$$

其中Q是多项式，并且Q是对称多项式；这些条件就足够了。因而（代数。章节V，附录I），$S(\mathbf{R}^l)^{W(R)}$是由l多项式函数生成的代数

$$
t_i = \sum_{\tau \in S_l} \xi_{\tau(1)}^2 \xi_{\tau(2)}^2 \cdots \xi_{\tau(l)}^2 \quad (1 \leq i \leq l).
$$

而且，$S(\mathbf{R}^l)^{W(R)}$的分数对域对$\mathbf{R}$的超越次数为l，因而$t_i$在代数上是独立的。由于$t_i$有次数 2, 4, ..., 2l，我们结论 W(R) 的指数（第V。§ 6, no. 3，命题3）是：

$$ 1, 3, 5, \ldots, 2l - 1. $$

(XI) Dynkin 图中唯一的自同构是单位元素。因而，$A(R) = W(R)$和$-1 \in W(R)$。从$-1$变换B到$-B$，我们结论即$w_0 = -1$。

(XII) 群 $P(R^-)/Q(R^-)$ 与 $P(R)/Q(R)$ 对偶，因此与 $\mathbf{Z}/2\mathbf{Z}$ 同构的。它的非平凡元素将顶点相应的排列为 $\alpha_0$ 和 $\alpha_1$ 并保持其他不变。

### 6. 系统型 $C_l$ ($l \geq 2$)

(I)型$C_l$的根系的存在性已在no. 5中得到证明，因为我们已经看到型$B_l$的系统的逆系是型$C_l$。因此，通过取入$\mathbf{R}'$向量$\pm 2\varepsilon_i$($1 \leq i \leq l$)和$\pm \varepsilon_i \pm \varepsilon_j$($1 \leq i < j \leq l$)来获得型$C_l$中的根系。 根中的数是$2l^2$。

R的(II)基可以通过在no. 5中考虑系统的基的映射$\alpha \mapsto \frac{2\alpha}{(\alpha|\alpha)}$取像来获得。我们得到：

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2, \quad \alpha_2 = \varepsilon_2 - \varepsilon_3, \ldots, \quad \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l, \quad \alpha_l = 2\varepsilon_l.
$$

正根是 $2\varepsilon_i$ 和 $\varepsilon_i \pm \varepsilon_j$ ($i < j$)。

(III) Coxeter 数与逆系相同：$h = 2l$。

(IV)设$\tilde{\alpha} = 2\varepsilon_1 = 2\alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-1} + \alpha_l$，即根。其坐标和相对于$(\alpha_i)$的坐标为$2l - 1 = h - 1$。因此，$\tilde{\alpha}$是最高根。我们有 $(\tilde{\alpha}|\alpha_i) = 0$ 对应 $i \neq l$、$(\tilde{\alpha}|\alpha_l) = 2$。因此，完整的 Dynkin 图为

![C_l 的 Dynkin 图](https://i.imgur.com/3Q5z5QG.png)

(V) 我们已经确定了$R^-$，即型$B_l$。通过§ 1, no. 12的公式(19)和no. 5(V)，$\Phi_R$的$2\varepsilon_i$长度平方是

$$
((l+1)(4l-2))^{-1} ((4l-2)^{-1})^{-1} = (l+1)^{-1};
$$

因此，$\Phi_R(x, y) = (x|y)/4(l+1)$。

我们有$\gamma(R) = \gamma(R^-) = (l+1)(4l-2)$。

(VI) 基本权很容易找到：

$$
\omega_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i
$$
$$
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \frac{1}{2}\alpha_l) \quad (i \leq l).
$$

(VII) 和的正根为
$$
2\rho = 2l\varepsilon_1 + (2l-2)\varepsilon_2 + \cdots + 4\varepsilon_{l-1} + 2\varepsilon_l
$$
$$
= 2l\alpha_1 + 2(2l-1)\alpha_3 + \cdots + i(2l-i+1)\alpha_i + \cdots
$$
$$
\cdots + (l-1)(l+2)\alpha_{l-1} + \frac{1}{2}l(l+1)\alpha_l.
$$

(VIII) 通过no. 4和no. 5 (VIII)，$Q(R) = L_1, P(R) = L_0; P(R)/Q(R)$与$\mathbf{Z}/2\mathbf{Z}$同构的，且连接指标为2。

(IX) 和 (X) 这些数据仅取决于$W(R)$，因此与型 $B_l$ 相同。

(XI) 与no. 5相同的论证表明$A(R) = W(R)$和$w_0 = -1$。

(XII) $P(R^-)/Q(R^-)$ 定义的单个非恒等元素是完整 Dynkin 图的唯一非平凡自同构：它将顶点相应的交换为 $\alpha_j$，将$\alpha_{l-j}$ 交换为 $0 \leq j \leq l$。

### 7. 系统型 $A_l$ ($l \geq 1$)

(I) 和 (II) 令$E = \mathbf{R}^{l+1}$中的$V$为超平面，并使用等式$\sum_{i=1}^{l+1} \xi_i = 0$。由no. 5中的$l+1$替换$l$，我们得到$E$中型$B_{l+1}$的系统$R'$和基
$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3, \ldots, \alpha_l = \varepsilon_l - \varepsilon_{l+1},\ \alpha_{l+1} = \varepsilon_{l+1}.
$$
由于$\alpha_1, \ldots, \alpha_l$生成$V$，$R = R' \cap V$在$V$和基$(\alpha_1, \ldots, \alpha_l)$中是根系（§ 1, no. 7，第20号提案的Cor.4）。通过no. 5中的标量乘积计算，$R$是型$A_l$的直接的。 $R$中的元素是$\varepsilon_i - \varepsilon_j$（$i \neq j, 1 \leq i \leq l+1, 1 \leq j \leq l+1$）。有$n = l(l+1)$根。正根是 $\varepsilon_i - \varepsilon_j$，其中 $i < j$。

(III) 我们有$h = n/l = l+1$。

(IV)设$\tilde{\alpha} = \varepsilon_1 - \varepsilon_{l+1} = \alpha_1 + \alpha_2 + \cdots + \alpha_l$，即根。其坐标和相对于$(\alpha_i)$的坐标为$l = h-1$。因此$\tilde{\alpha}$是最高根。
对于$l = 1$，$\tilde{\alpha} = \alpha_1$，所以$(\tilde{\alpha}|\alpha_1) = 2$； 群 $W_a(R)$ 的 Coxeter 图为

$$
\begin{array}{c}
\infty \\
\alpha_1
\end{array}
$$

$l \geq 2$。 $(\tilde{\alpha}|\alpha_i) = 0$适用于$0 < i < l$和$(\tilde{\alpha}|\alpha_1) = (\tilde{\alpha}|\alpha_l) = 1$。因此完整的 Dynkin 图为：

![丁金图](https://i.imgur.com/3Q5z5QG.png)

(V) 使用标量乘积识别V及其对偶，我们对所有$\alpha \in \mathbf{R}$有$\tilde{\alpha} = \frac{2\alpha}{(\alpha|\alpha)} = \alpha$，因此$R^* = R$。

对于形式$\Phi_R$，根的长度是$h^{-1/2} = (l+1)^{-1/2}$（§ 1, no. 12）；所以$\Phi_r(x, y) = (x|y)/2(l+1)$。

我们有 $\gamma(R) = (l+1)^2$ (§ 1, no. 12, 公式 (20))。

(VI) 设$(\omega_i)_{1 \leq i \leq l}$为基数权的族。放

$$
\omega_i = \sum_{j=1}^{l+1} \xi_{ij} \varepsilon_j. \quad \text{with } \xi_{ij} \in \mathbf{R}.
$$

条件 $(\omega_i|\alpha_j) = \delta_{ij}$ 和 $\omega_i \in V$ 给出

$$
\xi_{ii} - \xi_{i,i+1} = 1, \quad \xi_{ij} - \xi_{i,j+1} = 0 \text{ for } j \neq i. \quad \sum_{j=1}^{l+1} \xi_{ij} = 0,
$$

从而容易导致

$$
\begin{align*}
\omega_i &= \varepsilon_1 + \cdots + \varepsilon_i - \frac{i}{l+1}(\varepsilon_1 + \cdots + \varepsilon_{l+1}) \\
&= \frac{1}{l+1}((l-i+1)(\alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1}) \\
&\qquad + i((l-i+1)\alpha_i + (l-i)\alpha_{i+1} + \cdots + \alpha_l)).
\end{align*}
$$

(VII) 和的正根是

$$
\begin{align*}
2\rho &= l\varepsilon_1 + (l-2)\varepsilon_2 + (l-4)\varepsilon_3 + \cdots - (l-2)\varepsilon_l - l\varepsilon_{l+1} \\
&= l\alpha_1 + 2(l-1)\alpha_2 + \cdots + i(l-i+1)\alpha_i + \cdots + l\alpha_l.
\end{align*}
$$

(VIII) 引入no. 4的$E = \mathbf{R}^{l+1}$子群$L_0$。令$p$ 为$E$ 到$V$ 的正交投影。根据第 28 条提案§ 1, no. 10，我们有

$$
Q(R) = Q(R') \cap V \not\subset L_0 \cap V, \quad \text{and} \quad P(R) = p(P(R'));
$$

鉴于$R'$的最后一个基本权与$V$正交，我们有$P(R) = p(Q(R')) = p(L_0)$。因而，$P(R)$是由$\varepsilon_i - \varepsilon_j$和$p(\varepsilon_1) = \varepsilon_1 - (l+1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i$生成的群，所以

$$
P(R) = Q(R) + \mathbf{Z}(\varepsilon_1 - (l+1)^{-1} \sum_{i=1}^{l+1} \varepsilon_i).
$$

现在$l + 1$是最小的整数$m > 0$这样$mp(\varepsilon_1) \in Q(R)$。因而$P(R)/Q(R)$与$\mathbf{Z}/(l+1)\mathbf{Z}$同构的，并且连接指标是$l + 1$。

(IX) 和 (X) 对于$V$的任何自同构$g$，令$\varphi(g)$为$E$的自同构，扩展$g$且使$\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_l$不变。如果$g$是正交反射$s_{\varepsilon_i - \varepsilon_j}|V$，则$\varphi(g)$等于$s_{\varepsilon_i - \varepsilon_j}$，它互换了$\varepsilon_i$和$\varepsilon_j$，并且使$\varepsilon_k$固定，$k$不同于$i$和$j$。让

$$
X = \{\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_{l+1}\}.
$$

那么从$W(R)$到$X$的对称群，$g \mapsto \varphi(g)|X$就是同构。因而，$W(R)$ 与对称的群 $S_{l+1}$ 同构的，阶 $(l+1)!$ 也同构。

对称的代数$S(E)$可以与$E$上的多项式函数$P(\xi_1, \xi_2, \ldots, \xi_{l+1})$的代数进行规范地识别。让$G = \varphi(W(R))$。由上段可知，$G$下$S(E)$不变量的元素的集合$S(E)^G$是对称多项式的集合（代数，V章，附录I），因而(\emph{同上。}) 是由函数生成的代数

$$
s'_i = \sum_{\tau \in S_{l+1}} \xi_{\tau(1)} \xi_{\tau(2)} \cdots \xi_{\tau(i)} \quad (1 \leq i \leq l+1).
$$

代数$S(V)$可以与$E$上多项式函数的限制到$V$进行识别。如果$P \in S(E)^G$，$P$到$V$的限制在$W(R)$下显然是不变的。反之，若$Q \in S(V)^{W(R)}$，则存在$P \in S(E)$延伸$Q$； 替换$P$乘$((l+1)!)^{-1} \sum_{g \in G} g(P)$，其限制与$P$至$V$相同，我们可以假设$P \in S(E)^G$。因此，$S(V)^{W(R)}$是由$s_i = s'_i|V$生成的。现在$s_1 = 0$。此外，$S(V)^{W(R)}$的分数对域的超越次数对$\mathbf{R}$的超越是$l$，因此$s_i$（$2 \leq i \leq l+1$）在代数上是独立的。由于$s_i$是次数$2, 3, \ldots, l+1$，$W(R)$的指数是

$$
1, 2, 3, \ldots, l.
$$

(XI) 适用于 $l = 1$、$A(R) = W(R) = \mathbf{Z}/2\mathbf{Z}$ 和 $w_0 = -1$。

对于$l \geq 2$，令$\varepsilon \in A(R)$为自同构，即变换$\alpha_i$到$\alpha_{l+1-i}$。很明显，由 $\varepsilon$ 导出的自同构是 Dynkin 图的唯一非平凡自同构。 群 $A(R)/W(R)$ 与 $\mathbf{Z}/2\mathbf{Z}$ 同构的。由于$-1$是$A(R)$的元素，而属于不通过(IX)和(X)从属于到$W(R)$，我们看到$A(R)$与$W(R) \times \mathbf{Z}/2\mathbf{Z}$同构的。我们有$w_0 = -\varepsilon$。

(XII)群$P(R^-)/Q(R^-)$是阶$l+1$的循环，并通过循环置换作用于完整的Dynkin图。如果$l \geq 2$，则$A(R)/W(R)$的唯一非恒等元素通过自同构$x \mapsto -x$作用于$P(R^-)/Q(R^-)$。

### 8. 系统型 $D_l$ ($l \geq 3$)

（I）考虑$V = \mathbf{R}'$群$L_0$（no. 4）。 $\alpha \in L_0$的集合$R$，使得$(\alpha|\alpha) = 2$由向量$\pm \varepsilon_i \pm \varepsilon_j$($1 \leq i < j \leq l$)组成。很明显，对于所有 $\alpha, \beta \in R$，$R$ 生成 $V$ 和 $2(\alpha|\beta)/(\alpha|\alpha) \in \mathbf{Z}$。因此，$R$ 是$V$ (no. 4) 中的约化根系。 根中的数是$n = 2l(l-1)$。

(II) 放

$$
\alpha_1 = \varepsilon_1 - \varepsilon_2,\ \alpha_2 = \varepsilon_2 - \varepsilon_3 \ldots \ldots \alpha_{l-1} = \varepsilon_{l-1} - \varepsilon_l,\ \alpha_l = \varepsilon_{l-1} + \varepsilon_l.
$$

以下公式为直接的：

$$
\varepsilon_i - \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1}\quad (i < j)
$$
$$
\varepsilon_i + \varepsilon_j = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{j-1} + 2\alpha_j + 2\alpha_{j+1} + \cdots
$$
$$
\cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l\quad (i < j \leq l-2)
$$
$$
\varepsilon_i + \varepsilon_{l-1} = \alpha_i + \alpha_{i+1} + \cdots + \alpha_l\quad (i < l-1)
$$
$$
\varepsilon_i + \varepsilon_l = \alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2} + \alpha_l\quad (i < l-1)
$$
$$
\varepsilon_{l-1} + \varepsilon_l = \alpha_l.
$$

所以如果 $R$，$(\alpha_1, \ldots, \alpha_l)$ 就是基（§ 1, no. 2，第 20 条命题第 3 条）。此外，$\| \alpha_i \| ^2 = 2$适用于所有$i$。 $(\alpha_i|\alpha_j) = 0$ 对应 $i + 1 < j$，$i = l-2, j = l$ 除外，在这种情况下$(\alpha_{l-2}|\alpha_l) = -1$，$(\alpha_i|\alpha_{i+1}) = -1$ 对应$i \leq l-2$，最后$(\alpha_{l-1}|\alpha_l) = -1$；因此，$R$ 的 Dynkin 图为型 $D_l$。正根是 $i < j$ 的 $\varepsilon_i \pm \varepsilon_j$。

(III) 我们有$h = n/l = 2(l-1)$。

(IV)设$\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = \alpha_1 + 2\alpha_2 + \cdots + 2\alpha_{l-2} + \alpha_{l-1} + \alpha_l$，即根。其相对于$(\alpha_i)$的坐标和为

$$
2l-3 = h-1.
$$

因此$\tilde{\alpha}$是最高根。

如果$l = 3$，我们有

$$
(\tilde{\alpha}|\alpha_1) = 0,\quad (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = 1.
$$

如果$l \geq 4$，我们有$(\tilde{\alpha}|\alpha_i) = 0$对应$i \neq 2$和$(\tilde{\alpha}|\alpha_2) = 1$。因此完整的 Dynkin 图为：

![D_l 的 Dynkin 图](https://i.imgur.com/3Q5z5QG.png)

(V) 从$(\alpha|\alpha) = 2$开始，对于所有$\alpha \notin R$，我们有$R^- = R$。
$\Phi_{L'}$ 的根的长度是$h^{-1/2} = (2l-2)^{-1/2}$。因此

$$
\Phi_R(x, y) = (x|y)/(4l-4)\quad \text{and}\quad \gamma(R) = 4(l-1)^2.
$$

(VI) 类似于 no. 7 中的计算给出基本权：

$$
\omega_i = \varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_i \\
= \alpha_1 + 2\alpha_2 + \cdots + (i-1)\alpha_{i-1} + i(\alpha_i + \alpha_{i+1} + \cdots + \alpha_{l-2}) \\
\quad + \frac{1}{2}i(\alpha_{l-1} + \alpha_l)
$$

对于$i < l - 1$，

$$
\omega_{l-1} = \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} - \varepsilon_l) \\
= \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2}l\alpha_{l-1} + \frac{1}{2}(l-2)\alpha_l),
$$
$$
\omega_l = \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \cdots + \varepsilon_{l-2} + \varepsilon_{l-1} + \varepsilon_l) \\
= \frac{1}{2}(\alpha_1 + 2\alpha_2 + \cdots + (l-2)\alpha_{l-2} + \frac{1}{2}(l-2)\alpha_{l-1} + \frac{1}{2}l\alpha_l).
$$

(VII) 和的正根是

$$
2\rho = 2(l-1)\varepsilon_1 + 2(l-2)\varepsilon_2 + \cdots + 2\varepsilon_{l-1} \\
= \sum_{i=1}^{l-2} 2(i(l-\frac{i(i+1)}{2}))\alpha_i + \frac{l(l-1)}{2}(\alpha_{l-1} + \alpha_l).
$$

(VIII) $\pm \varepsilon_i \pm \varepsilon_j$ 生成 $L_1$ (no. 4)，所以$Q(R) = L_1$。因而$Q(R^*) = L_1$，进而$P(R) = L_2$ (no. 4)。通过no. 4，对于$l$奇数，$P(R)/Q(R)$与$\mathbf{Z}/4\mathbf{Z}$同构的，对于$l$偶数，$\mathbf{Z}/2\mathbf{Z} \times \mathbf{Z}/2\mathbf{Z}$同构的。在第一种情况下，$P(R)/Q(R)$由$\omega_l$的典范像生成（也由$\omega_{l-1}$的典范像生成）。在第二种情况下，$P(R)/Q(R)$是由$\omega_{l-1}$和$\omega_l$的典范像生成的。在这两种情况下，连接指标均为 4。

(IX) 和 (X) 在 $\mathbf{R}^l$ 中，正交反射 $s_{\varepsilon_i, -\varepsilon_j}$ ($i \neq j$) 互换 $\varepsilon_i$ 和 $\varepsilon_j$，并且使 $\varepsilon_k$ 不变，$k$ 不同于 $i$ 和$j$。 $s_{\varepsilon_i, -\varepsilon_j}$ 生成群 $G_1$ 同构于对称的群 $S_l$。另一方面，$s_{ij} = s_{\varepsilon_i, -\varepsilon_j} s_{\varepsilon_i, +\varepsilon_j}$变换$\varepsilon_i$到$-\varepsilon_i$，$\varepsilon_j$到$-\varepsilon_j$，并且使$\varepsilon_k$保持不变，而$k$不同于$i$和$j$。 向量空间$\mathbf{R}^l$的自同构$u$的$s_{ij}$生成群$G_2$、集合使得$u(\varepsilon_i) = (-1)^{\nu_i} \varepsilon_i$和$\prod_{i=1}^l (-1)^{\nu_i} = 1$。 群$G_2$与$(\mathbf{Z}/2\mathbf{Z})^{l-1}$同构的，$G_2$在$W(R)$中是正规的，因而$W(R)$与$S_l$的半直接乘积同构于$(\mathbf{Z}/2\mathbf{Z})^{l-1}$。因而，它的阶是$2^{l-1} l!$。

no. 5的多项式函数$t_i$在$W(R)$下是不变的，$t = \xi_1 \xi_2 \ldots \xi_l$也是不变的；此外，$t_l = t^2$。令$P(\xi_1, \ldots, \xi_l)$为$W(R)$下的多项式不变量。设$\xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$是$P$的单项式，使得$\nu_i$是奇数；那么$\nu_j$对于所有$j$来说都是奇数，因为单项式$(-1)^{\nu_i + \nu_j} \xi_1^{\nu_1} \xi_2^{\nu_2} \ldots \xi_l^{\nu_l}$在$s_{ij}(P)$中具有特征，所以$\nu_i + \nu_j \equiv 0 \pmod{2}$和$\nu_j \equiv 1 \pmod{2}$。因此

P = P_1 + tP_2，其中 P_1 和 P_2 中的所有单项式都只有偶数指数。由于 P 在 $\xi_i$ 的置换下是不变的，因此 P_1 和 P_2 具有相同的性质，因此可以写成 $t_1, t_2, \ldots, t_l$ 中的多项式。这就证明代数$S(\mathbf{R}^l)^{W(R)}$是由$t_1, t_2, \ldots, t_{l-1}, t$生成的。而且，$S(\mathbf{R}^l)^{W(R)}$的分数对域的超越次数是l，所以$t_1, t_2, \ldots, t_{l-1}, t$在代数上是独立的。我们将结论指数中的序列适当排序后，为：

$$
1, 3, 5, \ldots, 2l - 5, 2l - 3, l - 1.
$$

Note that $l - 1$ appears twice if $l$ is even, and once if $l$ is odd.

Dynkin 图的 (XI) 自同构是底层图的那些。因此：
1) 若$l = 3$，则$A(R)/W(R)$同构于$\mathbf{Z}/2\mathbf{Z}$。
2) 如果$l = 4$，则图的终止顶点定义自同构的每个置换，所以$A(R)/W(R)$与$\mathfrak{S}_3$同构。
3) 如果$l \geq 5$，则从分支点开始的链有长度1、1和$l - 3 \geq 2$。图中唯一与恒等不同的自同构，因此从对应到自同构$\varepsilon \in A(R)$，它们交换了$\alpha_{l-1}$和$\alpha_l$，并且将$\alpha_i$固定为$1 \leq i \leq l - 2$。因此$A(R)/W(R)$与$\mathbf{Z}/2\mathbf{Z}$同构；此外，$A(R)$是$\mathbf{R}^l$的自同构$u$的群$G_3$由……组成在(IX)中定义的群$G_1 \cong \mathfrak{S}_l$的半直接乘积，使得$u(\varepsilon_i) = \pm \varepsilon_i$ 对于所有$i$。

如果$l$是偶数，则$-1 \in W(R)$，所以$w_0 = -1$。如果$l$是奇数，则$-1 \notin W(R)$，所以$A(R) = W(R) \times \{1, -1\}$和$w_0 = -\varepsilon$。

(XII) 对于$l$偶数，$P(R^-)/Q(R^-)$有阶2中的三个元素，即$\omega_1, \omega_{l-1}$和$\omega_l$。由于$\omega_l$（或$\omega_{l-1}$）将顶点相应的互换至$\alpha_0$和$\alpha_l$（或$\alpha_{l-1}$），因此它将相应的互换至$\alpha_1$和$\alpha_{l-1}$（或$\alpha_l$），还有那些相应的到 $\alpha_j$ 和 $\alpha_{l-j}$

$$
2 \leq j \leq l - 2.
$$

我们有$\omega_1 = \omega_l \omega_{l-1}$。

对于$l$奇数，$P(R^-)/Q(R^-)$有阶 4中的两个元素，即$\omega_{l-1}$和$\omega_l$，以及阶 2中的一个元素，等于$\omega_1$。事实上，$\omega_1$将顶点相应的互换到$\alpha_0$和$\alpha_1$，因此对于$2 \leq j \leq l - 2$来说，它保留了固定的顶点相应的到$\alpha_j$，并且必然是阶2。因而$\omega_l$是阶 4 和变换顶点相应的到 $\alpha_0$（分别为 $\alpha_l$，分别为 $\alpha_1$，分别为 $\alpha_{l-1}$）到相应的到 $\alpha_l$（分别为 $\alpha_1$，分别为 $\alpha_{l-1}$、$\alpha_0$），并将顶点相应的替换为 $\alpha_j$，将 $\alpha_{l-j}$ 替换为 $2 \leq j \leq l - 2$。我们有$\omega_1 = \omega_l^2$和$\omega_{l-1} = \omega_l^3$。

对于$l \neq 4$，$A(R)/W(R)$的非恒等元素将顶点相应的互换到$\alpha_{l-1}$和$\alpha_l$，从而互换$P(R^-)/Q(R^-)$的元素、$\omega_{l-1}$和$\omega_l$。对于$l$奇数，这样得到的$P(R^-)/Q(R^-)$中的自同构为映射$x \mapsto -x$。

对于$l = 4$，$A(R)/W(R)$可以与$\{1, 3, 4\}$的置换的群识别，并通过指标的置换作用于$\{\omega_1, \omega_3, \omega_4\}$。

### 9. 系统型 $F_4$

(I) 考虑$\mathbf{R}^4$中的群$L_2$(no. 4)。令$R$为$\alpha \in L_2$的集合，使得$(\alpha|\alpha) = 1$或$(\alpha|\alpha) = 2$； 包含向量
$$
\pm \varepsilon_i,\quad \pm \varepsilon_i \pm \varepsilon_j\ (i < j),\quad \frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
反之，如果$\alpha \in R$，则$\alpha$的坐标只能取值$0, \pm \frac{1}{2}, \pm 1$（从$(\frac{3}{2})^2 > 2$开始）；或者这些坐标都是整数，给出向量$\pm \varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j$，或者它们都等于$\pm \frac{1}{2}$，给出向量$\frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$。

我们证明，对于 $\alpha, \beta \in R$，我们有 $2(\alpha|\beta)/(|\alpha|\alpha) \in \mathbf{Z}$。如果$\alpha = \pm \varepsilon_i$或$\alpha = \frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$，则$(\alpha|\alpha) = 1$，并且我们在no. 4中看到自$\alpha, \beta \in L_2$以来的$(\alpha|\beta) \in \frac{1}{2}\mathbf{Z}$。如果$\alpha = \pm \varepsilon_i \pm \varepsilon_j$，则$(\alpha|\alpha) = 2$，并且自$\alpha \in L_1$和$\beta \in L_2$以来，我们在no. 4中看到了$(\alpha|\beta) \in \mathbf{Z}$。因此，$R$ 是$\mathbf{R}^4$ (no. 4) 中的约化根系。 根中的数是$n = 8 + \binom{4}{2} 4 + 2^4 = 48$。

(II) 给出$\mathbf{R}^4$由基$(\varepsilon_1, \varepsilon_2, \varepsilon_3, \varepsilon_4)$(§ 1, no. 7)定义的词典阶。特别是，我们有$\varepsilon_1 > \varepsilon_2 > \varepsilon_3 > \varepsilon_4$。正值根是
$$
\varepsilon_i,\quad \varepsilon_i \pm \varepsilon_j\ (i < j),\quad \frac{1}{2}(\varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4).
$$
最小的根为$\alpha_3 = \varepsilon_4$。在根属于到$\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$但不到$\mathbf{R}\varepsilon_4$中，最小的是$\alpha_2 = \varepsilon_3 - \varepsilon_4$。在根属于到$\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$但不到$\mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$的正数中，最小的是$\alpha_1 = \varepsilon_2 - \varepsilon_3$。在正根不是属于到$\mathbf{R}\varepsilon_2 + \mathbf{R}\varepsilon_3 + \mathbf{R}\varepsilon_4$中，最小的是$\alpha_4 = \frac{1}{2}(\varepsilon_1 - \varepsilon_2 - \varepsilon_3 - \varepsilon_4)$。 $\alpha_i$ 都不是 2 个正根中的和。因此，$(\alpha_1, \alpha_2, \alpha_3, \alpha_4)$ 是$R$ 的基（§ 1, no. 6，Cor. 1 到 Prop. 19）。我们有$\| \alpha_1 \| = \| \alpha_2 \| = 2, \| \alpha_3 \| = \| \alpha_4 \| = 1, (\alpha_1|\alpha_2) = (\alpha_2|\alpha_3) = -1, (\alpha_3|\alpha_4) = -\frac{1}{2}, (\alpha_1|\alpha_3) = (\alpha_1|\alpha_4) = (\alpha_2|\alpha_4) = 0$。我们看到$R$的Dynkin图是型$F_4$，因此是不可约的。

(III) 我们有$h = \frac{n}{l} = 12$。

(IV) 让$\tilde{\alpha} = \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4$。 $\tilde{\alpha}$相对于$(\alpha_i)$的坐标和是$11 = h - 1$，所以$\tilde{\alpha}$是最高根。我们有$(\tilde{\alpha}|\alpha_1) = 1, (\tilde{\alpha}|\alpha_2) = (\tilde{\alpha}|\alpha_3) = (\tilde{\alpha}|\alpha_4) = 0$。

完整的 Dynkin 图为

![F_4 的 Dynkin 图](https://i.imgur.com/3Q5z5QG.png)

(V)公式$\alpha^* = \frac{2\alpha}{(\alpha|\alpha)}$给出$R^-$集合/向量$\pm 2\varepsilon_i, \pm \varepsilon_i \pm \varepsilon_j, \pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4$。 $R^-$的Dynkin图是通过no. 2中解释的过程从$R$的Dynkin图获得的，我们看到$R^-$是型$F_4$。

The roots not orthogonal to $\beta = \varepsilon_1$ are $\pm \varepsilon_1, \pm \varepsilon_1 \pm \varepsilon_j \ (j \geq 2)$, and $\frac{1}{2}(\pm \varepsilon_1 \pm \varepsilon_2 \pm \varepsilon_3 \pm \varepsilon_4)$: the number $n(\alpha|\beta) = 2(\alpha|\beta)$ is equal to $\pm 2$ for the first 14 of these roots and to $\pm 1$ for the last 16; thus, for $\Phi_R$, the square of the length of $\beta$ is $4(14.4 + 16.1)^{-1} = \frac{1}{18}$; hence

$$
\Phi_R(x, y) = \frac{(x|y)}{18}.
$$

我们现在应用§ 1, no. 12的公式(18)，以及$x = y = \beta$；这给出了

$$
2 + 12.\frac{1}{4} + 16.\frac{1/4}{1} = \gamma(R).\frac{1}{18}
$$

所以

$$
\gamma(R) = 2.3^4.
$$

(VI) 计算基本权给出

$$
\begin{align*}
\omega_1 &= \varepsilon_1 + \varepsilon_2 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 2\alpha_4 = \tilde{\alpha} \\
\omega_2 &= 2\varepsilon_1 + \varepsilon_2 + \varepsilon_3 = 3\alpha_1 + 6\alpha_2 + 8\alpha_3 + 4\alpha_4 \\
\omega_3 &= \frac{1}{2}(3\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4) = 2\alpha_1 + 4\alpha_2 + 6\alpha_3 + 3\alpha_4 \\
\omega_4 &= \varepsilon_1 = \alpha_1 + 2\alpha_2 + 3\alpha_3 + 2\alpha_4.
\end{align*}
$$

正根的 (VII) 和为

$$
2\rho = 11\varepsilon_1 + 5\varepsilon_2 + 3\varepsilon_3 + \varepsilon_4 = 16\alpha_1 + 30\alpha_2 + 42\alpha_3 + 22\alpha_4.
$$

(VIII) 我们有 $Q(R) = L_2$ (no. 4)，还有$P(R) = Q(R)$ (VI)。因而，连接指标为1。

(IX)指数族有4个项，从$h = 12$开始，它必须包含整数1,5,7,11，与12互质（§ 1, no. 11，命题30）；因而，这些都是 $W(R)$ 的指数。

(X) 和 (XI) Dynkin 图中唯一的自同构是恒等式，因而$A(R) = W(R)$ 和 $w_0 = -1$。设$R'$为$R$中最长的元素中的集合，即$\pm \varepsilon_i \pm \varepsilon_j$； $R'$是no. 8建造的型$D_4$中的根系。显然，$A(R)$的每个元素都是$A(R')$的元素。相反，$A(R')$的元素使$L_1$保持稳定（因为它是由$R'$生成的），因此它的相关$L_2$也是如此，因而$R$也是如此。所以$W(R) = A(R) = A(R')$。通过no. 8，$W(R)$是$S_3$通过$W(R')$的半直接乘积，$W(R')$本身是$S_4$通过$(\mathbf{Z}/2\mathbf{Z})^3$的半直接乘积。 $W(R)$中的阶是$3!4!2^3 = 2^7.3^2$。

### 10. 系统 / 型 E_8

(I) 考虑$\mathbf{R}^8$中的群 L_3 (no. 4)。令 R 为 $\alpha \in L_3$ 的集合，使得 $(\alpha|\alpha) = 2$； 包含向量

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (i < j), \quad \frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i \quad (\sum_{i=1}^8 \nu(i) \text{ even}).
$$

相反，如果元素 $\alpha \in L_3$ 满足 $(\alpha|\alpha) = 2$，则其坐标必须在值 $0, \pm \frac{1}{2}, \pm 1$ 之间：到 no. 4，这些坐标要么都是整数，给出向量 $\pm \varepsilon_i \pm \varepsilon_j$，要么它们都等于 $\pm \frac{1}{2}$，其中整数和，给予向量

$$
\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i
$$

与 $\sum_{i=1}^8 \nu(i)$ 偶数。

我们已经看到（no. 4）对于所有$\alpha, \beta \in L_3$来说$(\alpha|\beta) \in \mathbf{Z}$。因而，R 为约化根系。 根中的数是$n = \binom{8}{2} . 4 + 2^7 = 240$。

(II) 设$\rho$为向量$(0, 1, 2, 3, 4, 5, 6, 23)$除$L_3$。 R 中没有元素与 $\rho$ 正交（这对于 $\pm \varepsilon_i \pm \varepsilon_j$ 来说是清楚的；如果 $\frac{1}{2} \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i$ 与 $\rho$ 正交，我们将有 $\sum_{i=1}^6 i(-1)^{\nu(i+1)} + 23(-1)^{\nu(8)} = 0$，这从 $\sum_{i=1}^6 i < 23$ 开始是不可能的）。因而（§ 1, no. 7，第 20 条命题第 2 条）$\alpha \in R$，使得 $(\alpha|\rho) > 0$ 是相对于某个房间的正根。这些根是 $\pm \varepsilon_i + \varepsilon_j \ (i < j)$，以及

$$
\frac{1}{2} (\varepsilon_8 + \sum_{i=1}^7 (-1)^{\nu(i)} \varepsilon_i)
$$

与 $\sum_{i=1}^7 \nu(i)$ 偶数。对于所有 $\alpha \in R$ (no. 4)，我们有 $(\alpha|\rho) \in \mathbf{Z}$，对于以下根，$(\alpha|\rho)$ 等于 1：

$$
\begin{align*}
\alpha_1 &= \frac{1}{2} (\varepsilon_1 + \varepsilon_8) - \frac{1}{2} (\varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7), \\
\alpha_2 &= \varepsilon_1 + \varepsilon_2, \ \alpha_3 = \varepsilon_2 - \varepsilon_1, \ \alpha_4 = \varepsilon_3 - \varepsilon_2, \ \alpha_5 = \varepsilon_4 - \varepsilon_3, \\
\alpha_6 &= \varepsilon_5 - \varepsilon_4, \ \alpha_7 = \varepsilon_6 - \varepsilon_5, \ \alpha_8 = \varepsilon_7 - \varepsilon_6.
\end{align*}
$$

还有$\mathbf{R}^8$这八个向量形式基。 § 1, no. 6，科罗纳。根据第 19 条命题 1，$(\alpha_1, \alpha_2, \ldots, \alpha_8)$ 是 R 的基，其中正根是上面定义的那些。我们有

$$
(\alpha_4|\alpha_5) = (\alpha_5|\alpha_6) = (\alpha_6|\alpha_7) = (\alpha_7|\alpha_8) = (\alpha_4|\alpha_2) = (\alpha_4|\alpha_3) = (\alpha_3|\alpha_1) = -1,
$$

$(\alpha_i|\alpha_j) = 0$ 适用于指标中的所有其他对。因而，R 的 Dynkin 图为型 E_8，并且 R 是不可约的。

(III) 我们有$h = \frac{n}{8} = 30$。

(IV)让
$$
\tilde{\alpha} = \varepsilon_7 + \varepsilon_8 = 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7 + 2\alpha_8,
$$
即根。它相对于$(\alpha_i)$的坐标和是$29 = h - 1$，所以$\tilde{\alpha}$是最高根。它与除 $\alpha_8$ 和 $(\tilde{\alpha}|\alpha_8) = 1$ 之外的所有 $\alpha_i$ 正交。因而，完整的 Dynkin 图为：

![E_8 的 Dynkin 图](../images/dynkin_e8.png)

(V) 从$(\alpha|\alpha) = 2$开始，对于所有$\alpha \in R$，我们有$R^- = R$。

对于 $\Phi_R$，根的长度平方为 $\frac{1}{30}$ (§ 1, no. 12)。因而，$\Phi_R(x, y) = (x|y)/60$和$\gamma(R) = 900$（§ 1。no. 12，公式（20））。

(VI) 计算基本权给出
$$
\begin{align*}
\omega_1 &= 2\varepsilon_8 = 4\alpha_1 + 5\alpha_2 + 7\alpha_3 + 10\alpha_4 + 8\alpha_5 + 6\alpha_6 + 4\alpha_7 + 2\alpha_8 \\
\omega_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8) \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\omega_3 &= \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 7\varepsilon_8) \\
&= 7\alpha_1 + 10\alpha_2 + 14\alpha_3 + 20\alpha_4 + 16\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\omega_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 5\varepsilon_8 \\
&= 10\alpha_1 + 15\alpha_2 + 20\alpha_3 + 30\alpha_4 + 24\alpha_5 + 18\alpha_6 + 12\alpha_7 + 6\alpha_8 \\
\omega_5 &= \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 4\varepsilon_8 \\
&= 8\alpha_1 + 12\alpha_2 + 16\alpha_3 + 24\alpha_4 + 20\alpha_5 + 15\alpha_6 + 10\alpha_7 + 5\alpha_8 \\
\omega_6 &= \varepsilon_5 + \varepsilon_6 + \varepsilon_7 + 3\varepsilon_8 \\
&= 6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 12\alpha_6 + 8\alpha_7 + 4\alpha_8 \\
\omega_7 &= \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8 \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 2\alpha_4 + 10\alpha_5 + 8\alpha_6 + 6\alpha_7 + 3\alpha_8 \\
\omega_8 &= \varepsilon_7 + \varepsilon_8 \\
&= 5\alpha_1 + 8\alpha_2 + 10\alpha_3 + 15\alpha_4 + 12\alpha_5 + 9\alpha_6 + 6\alpha_7 + 3\alpha_8 = \tilde{\alpha}.
\end{align*}
$$

(VII) 正根的一半和是基本权的和（§ 1, no. 10，命题29）；这给出了
$$
\begin{align*}
\rho &= \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 5\varepsilon_6 + 6\varepsilon_7 + 23\varepsilon_8 \\
&= 46\alpha_1 + 68\alpha_2 + 91\alpha_3 + 135\alpha_4 + 110\alpha_5 + 84\alpha_6 + 57\alpha_7 + 29\alpha_8.
\end{align*}
$$

(VIII)群Q(R)由$\varepsilon_i \pm \varepsilon_j$和$\frac{1}{2} \sum_{i=1}^8 \varepsilon_i$生成，等于L_3(no. 4)。因而，与 Q(R̄) = Q(R) = L_3 相关的 P(R) 是 L_3 (no. 4)。连接指标为 1。

(IX) 指数家族有8个项，从$h = 30$开始，整数 1, 7, 11, 13, 17, 19, 23, 29，互质到30，必须出现在这个家族中；因而，这些是 W(R) 的指数。

(X) 来自 (IX) 和章节。 V。 § 6, no. 2，科。由命题 3 的 1 可知，W(R) 的阶为

$$
2.8.12.14.18.20.24.30 = 2^{14}.3^5.5^2.7.
$$

(XI) Dynkin 图的唯一自同构是恒等式，因为从分支点发出的三个链具有不同的长度。因而，$A(R) = W(R)$和$w_0 = -1$。

### 11. 系统 / 型 E_7

(I)和(II)令$E = \mathbf{R}^8$，并令在no. 10构造的E中R_8为根系。令R_8的根$\alpha_1, \ldots, \alpha_7$生成的E中的V为超平面；它与 R_8 的第八基本权$\omega = \varepsilon_7 + \varepsilon_8$正交。

让$R = R_8 \cap V$。那么 R 是约化根系和基 $(\alpha_1, \ldots, \alpha_7)$，cf. § 1, no. 7，Cor。第 20 号提案第 4 条；因此，这个系统是型E_7。其元素为：

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i \leq j \leq 6), \quad \pm (\varepsilon_7 - \varepsilon_8),
$$
$$
\pm \frac{1}{2} (\varepsilon_7 - \varepsilon_8 + \sum_{i=1}^8 (-1)^{\nu(i)} \varepsilon_i) \quad \text{with } \sum_{i=1}^8 \nu(i) \text{ odd}.
$$

根中的数是$n = 2 + \binom{6}{2}.4 + 2^6 = 126$。正根是

$$
\pm \varepsilon_i + \varepsilon_j \quad (1 \leq i < j \leq 6), \quad -\varepsilon_7 + \varepsilon_8,
$$
$$
\frac{1}{2} (-\varepsilon_7 + \varepsilon_8 + \sum_{i=1}^6 (-1)^{\nu(i)} \varepsilon_i) \quad \text{with } \sum_{i=1}^6 \nu(i) \text{ odd}.
$$

(III) 我们有$h = \frac{n}{l} = 18$。

(IV)设$\tilde{\alpha} = \varepsilon_8 - \varepsilon_7 = 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7$，即根。其相对于$(\alpha_i)$的坐标和为17 = $h - 1$。因此是最高根。对于 $2 \leq i \leq 7$ 和 $(\tilde{\alpha}|\alpha_1) = 1$，它与 $\alpha_i$ 正交。完整的 Dynkin 图为

![E_7 的 Dynkin 图](https://i.imgur.com/3Q5z5QG.png)

(V) 从$(\alpha|\alpha) = 2$开始，对于所有$\alpha \in R$，我们有$R^- = R$。
对于$\Phi_R$，根的平方长度是$\frac{1}{18}$，所以
$$
\Phi_R(x, y) = (x|y)/36, \quad \text{and} \quad \gamma(R) = 2^2 \cdot 3^4
$$
（§ 1。no. 12，公式（20））。

(VI) 计算基本权给出
$$
\begin{align*}
\omega_1 &= \varepsilon_8 - \varepsilon_7 = 2\alpha_1 + 2\alpha_2 + 3\alpha_3 + 4\alpha_4 + 3\alpha_5 + 2\alpha_6 + \alpha_7 \\
\omega_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 2\varepsilon_7 + 2\varepsilon_8) \\
&= \frac{1}{2}(4\alpha_1 + 7\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 8\alpha_6 + 3\alpha_7) \\
\omega_3 &= \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 - 3\varepsilon_7 + 3\varepsilon_8) \\
&= 3\alpha_1 + 4\alpha_2 + 6\alpha_3 + 8\alpha_4 + 6\alpha_5 + 4\alpha_6 + 2\alpha_7 \\
\omega_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + 2(\varepsilon_8 - \varepsilon_7) \\
&= 4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 9\alpha_5 + 6\alpha_6 + 3\alpha_7 \\
\omega_5 &= \varepsilon_4 + \varepsilon_5 + \varepsilon_6 + \frac{3}{2}(\varepsilon_8 - \varepsilon_7) \\
&= \frac{1}{2}(6\alpha_1 + 9\alpha_2 + 12\alpha_3 + 18\alpha_4 + 15\alpha_5 + 10\alpha_6 + 5\alpha_7) \\
\omega_6 &= \varepsilon_5 + \varepsilon_6 - \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 2\alpha_7 \\
\omega_7 &= \varepsilon_6 + \frac{1}{2}(\varepsilon_8 - \varepsilon_7) \\
&= \frac{1}{2}(2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6 + 3\alpha_7).
\end{align*}
$$

正根的 (VII) 和 $2\rho$ 是 $2 \sum_{i=1}^7 \omega_i$ (§ 1. no. 10. 命题 29)，所以
$$
\begin{align*}
2\rho &= 2\varepsilon_2 + 4\varepsilon_3 + 6\varepsilon_4 + 8\varepsilon_5 + 10\varepsilon_6 - 17\varepsilon_7 + 17\varepsilon_8 \\
&= 34\alpha_1 + 49\alpha_2 + 66\alpha_3 + 96\alpha_4 + 75\alpha_5 + 52\alpha_6 + 27\alpha_7.
\end{align*}
$$

(VIII) 由no. 10 (VIII) 和§ 1, no. 10。提案 28，我们有
$$
Q(R) = Q(R_8) \cap V = L_3 \cap V \quad \text{and} \quad P(R) = p(P(R_8)) = p(L_3),
$$
其中 $p$ 表示 $E$ 到 $V$ 的正交投影。 群$Q(R)$有基$(\alpha_1, \ldots, \alpha_7)$； 群 $P(R)$ 由 $Q(R)$ 生成，并且
$$
p(\alpha_8) = \alpha_8 - \frac{1}{2}\omega.
$$

我们有$\omega \in P(R_8)$，$\frac{1}{2}\omega \notin P(R_8)$。所以$2p(\alpha_8) \in Q(R)$和$p(\alpha_8) \notin Q(R)$。因此，$P(R)/Q(R)$与$\mathbf{Z}/2\mathbf{Z}$同构的，并且由例如$\omega_7$的像生成。

连接指标为 2。

$W(R)$指数(IX)序列有7个项。 数 1, 5, 7, 11, 13, 17，与$h = 18$互质，在此序列中出现。最后一个指数$m$必须是$m + m = 18$（第V, § 6, no. 2，公式（2））。因此，指数的序列是

$$ 1, 5, 7, 9, 11, 13, 17. $$

(X) 来自 (IX) 和章节。 V, § 6, no. 2，科。根据命题 3 的 1，$W(R)$ 的阶为

$$ 2.6.8.10.12.14.18 = 2^{10}.3^4.5.7. $$

(XI) Dynkin 图中唯一的自同构是恒等式，因此$A(R) = W(R)$ 和 $w_0 = -1$。

(XII) $P(R^-)/Q(R^-)$ 只有一个非单位元素。它将顶点相应的与$\alpha_0$和$\alpha_7$、$\alpha_1$和$\alpha_6$、$\alpha_3$和$\alpha_5$互换，并且使$\alpha_2$和$\alpha_4$固定。

### 12. 系统 / 型 E_6

(I)和(II)令$E = \mathbf{R}^8$，并令$R_8$在no. 10构造的$E$中为根系。令$V$为由$R_8$的根$\alpha_1, \ldots, \alpha_6$生成的$E$的向量子空间；这是由 $R_8$ 的最后两个基本权$\omega = \varepsilon_7 + \varepsilon_8$和$\pi = \varepsilon_6 + \varepsilon_7 + 2\varepsilon_8$生成的平面的正交补。

让$R = R_8 \cap V$。这是约化根系与基 $(\alpha_1, \ldots, \alpha_6)$，因此是型 $E_6$。它的元素是：

$$
\pm \varepsilon_i \pm \varepsilon_j \quad (1 \leq i < j \leq 5),
$$
$$
\pm \frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \text{ with } \sum_{i=1}^5 \nu(i) \text{ even}.
$$

根中的数是$n = \binom{5}{2}.4 + 2^5 = 72$。正根是

$$
\pm \varepsilon_i + \varepsilon_j \quad (1 \leq i < j \leq 5),
$$
$$
\frac{1}{2} (\varepsilon_8 - \varepsilon_7 - \varepsilon_6 + \sum_{i=1}^5 (-1)^{\nu(i)} \varepsilon_i) \text{ with } \sum_{i=1}^5 \nu(i) \text{ even}.
$$

(III) 我们有$h = \frac{n}{6} = 12$。

(IV)让

$$
\tilde{\alpha} = \frac{1}{2} (\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8)
$$
$$
= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6,
$$

即根。它相对于$(\alpha_i)$的坐标和是$11 = h - 1$，所以$\tilde{\alpha}$是最高根。它与 $\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6$ 和 $(\tilde{\alpha}|\alpha_2) = 1$ 正交。完整的 Dynkin 图为

![丁金图](../images/dynkin_graph.png)

(V) 从$(\alpha|\alpha) = 2$开始，对于所有$\alpha \in R$，我们有$R' = R$。对于$\Phi_R$，根的平方长度是$\frac{1}{12}$，所以
$$
\Phi_R(x, y) = (x|y)/24, \quad \text{and} \quad \gamma(R) = 144.
$$

(VI) 计算基本权得出：
$$
\begin{align*}
\omega_1 &= \frac{2}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) = \frac{1}{3}(4\alpha_1 + 3\alpha_2 + 5\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6) \\
\omega_2 &= \frac{1}{2}(\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8) \\
&= \alpha_1 + 2\alpha_2 + 2\alpha_3 + 3\alpha_4 + 2\alpha_5 + \alpha_6 = \tilde{\alpha} \\
\omega_3 &= \frac{5}{6}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \frac{1}{2}(-\varepsilon_1 + \varepsilon_2 + \varepsilon_3 + \varepsilon_4 + \varepsilon_5) \\
&= \frac{1}{3}(5\alpha_1 + 6\alpha_2 + 10\alpha_3 + 12\alpha_4 + 8\alpha_5 + 4\alpha_6) \\
\omega_4 &= \varepsilon_3 + \varepsilon_4 + \varepsilon_5 - \varepsilon_6 - \varepsilon_7 + \varepsilon_8 \\
&= 2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 4\alpha_5 + 2\alpha_6 \\
\omega_5 &= \frac{2}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_4 + \varepsilon_5 \\
&= \frac{1}{3}(4\alpha_1 + 6\alpha_2 + 8\alpha_3 + 12\alpha_4 + 10\alpha_5 + 5\alpha_6) \\
\omega_6 &= \frac{1}{3}(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) + \varepsilon_5 \\
&= \frac{1}{3}(2\alpha_1 + 3\alpha_2 + 4\alpha_3 + 6\alpha_4 + 5\alpha_5 + 4\alpha_6).
\end{align*}
$$

(VII) 正根的一半和是$\sum_{i=1}^6 \omega_i$，所以
$$
\begin{align*}
\rho &= \varepsilon_2 + 2\varepsilon_3 + 3\varepsilon_4 + 4\varepsilon_5 + 4(\varepsilon_8 - \varepsilon_7 - \varepsilon_6) \\
&= 8\alpha_1 + 11\alpha_2 + 15\alpha_3 + 21\alpha_4 + 15\alpha_5 + 8\alpha_6.
\end{align*}
$$

(VIII) 根据no. 10 (VIII) 和§ 4, no. 10，第 28 号提案，
$$
Q(R) = Q(R_8) \cap V = L_3 \cap V \quad \text{and} \quad P(R) = p(P(R_8)) = p(L_3),
$$

其中 $p$ 表示 $E$ 与 $V$ 的正交投影。我们有
$$
p(\alpha_7) = \alpha_7 - \frac{2}{3}\pi + \omega, \quad p(\alpha_8) = \alpha_8 + \pi - 2\omega.
$$
群$Q(R)$有基$(\alpha_1, \ldots, \alpha_6)$。从$p(\alpha_8) \in P(R_8) \cap V = Q(R_8) \cap V = Q(R)$开始，群$P(R)$由$Q(R)$和$p(\alpha_7)$生成。我们有$3p(\alpha_7) \in Q(R)$和$p(\alpha_7) \notin Q(R)$。因此，群$P(R)/Q(R)$同构于$\mathbf{Z}/3\mathbf{Z}$；例如，它是由像或 $\omega_6$ 生成的。

连接指标为 3。

(IX) 和 (X) 根据§ 2, no. 4，第 7 号提案，Weyl 群的阶是 $6!1.2.2.3.2.1.3 = 2^7.3^4.5$。 指数的序列有6个项在1到11之间，以及包含整数1,5,7,11与12互质。其他指数$m, m'$是整数这样
$$
m + m' = 12,
$$
$$
(m + 1)(m' + 1)(1 + 1)(5 + 1)(7 + 1)(11 + 1) = 2^7.3^4.5,
$$
鉴于章。 V, § 6, no. 2、公式 (2) 和 Cor。命题 3 的 1. 第二个关系给出$(m + 1)(m' + 1) = 45$，从$m + m' + 2 = 14$开始，我们得到$m = 4, m' = 8$。因此，指数的序列是
$$
1, 4, 5, 7, 8, 11.
$$

(XI) 和 (XII) 由于根都具有相同的长度，因此 Dynkin 图的自同构是基础图的自同构。除了身份之外，只有自同构$\varepsilon$，其中变换$\alpha_1, \alpha_3, \alpha_4, \alpha_5, \alpha_6, \alpha_2$分别变成$\alpha_6, \alpha_5, \alpha_4, \alpha_3, \alpha_1, \alpha_2$。因此，$A(R)/W(R)$与$\mathbf{Z}/2\mathbf{Z}$同构的；由于$-1 \in W(R)$（第V, § 6, no. 2章，第3条命题第3条），$A(R)$与$W(R) \times \{1, -1\}$同构的，$w_0$可以与$-\varepsilon$识别。由此可见$A(R)/W(R)$定义自同构$x \mapsto -x$$P(R^-)/Q(R^-)$的非恒等元素。

此外，$P(R^-)/Q(R^-)$有两个非恒等元素阶 3。它们是完成的Dynkin图的阶 3的两个自同构定义。

### 13. 系统 / 型 G_2

(I) 令 $\mathbf{R}^3$ 中的 $E$ 为超平面，方程如下
$$
\xi_1 + \xi_2 + \xi_3 = 0.
$$
令$R$为$\alpha \in L_0 \cap V$的集合，使得$(\alpha|\alpha) = 2$或$(\alpha|\alpha) = 6$。 $R$中的元素是
$$
\pm (\varepsilon_1 - \varepsilon_2), \quad \pm (\varepsilon_1 - \varepsilon_3), \quad \pm (\varepsilon_2 - \varepsilon_3), \quad \pm (2\varepsilon_1 - \varepsilon_2 - \varepsilon_3),
$$
$$
\pm (2\varepsilon_2 - \varepsilon_1 - \varepsilon_3), \quad \pm (2\varepsilon_3 - \varepsilon_1 - \varepsilon_2).
$$

然后，R 生成 V，以及所有$\alpha, \beta \in R$的$\frac{2(\alpha|\beta)}{(\beta|\beta)} \in \mathbf{Z}$：如果$\beta = \pm (\varepsilon_i - \varepsilon_j)$和$i \neq j$，这很清楚；例如，如果$\beta = 2\varepsilon_1 - \varepsilon_2 - \varepsilon_3$，我们有$(\alpha|\beta) \in 3\mathbf{Z}$，并且我们的断言再次成立。因此，R 是V 中的约化根系。 根中的数是$n = 12$。

（II）放入$\alpha_1 = \varepsilon_1 - \varepsilon_2, \alpha_2 = -2\varepsilon_1 + \varepsilon_2 + \varepsilon_3$。那么根是

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \alpha_2,
$$
$$
\pm (3\alpha_1 + \alpha_2), \quad \pm (3\alpha_1 + 2\alpha_2).
$$

因此，$(\alpha_1, \alpha_2)$是R的基。我们有$\| \alpha_1 \| ^2 = 2, \| \alpha_2 \| ^2 = 6, (\alpha_1|\alpha_2) = -3$，所以R是型G_2的系统。正的根是$\alpha_1, \alpha_1 + \alpha_2, 2\alpha_1 + \alpha_2, 3\alpha_1 + \alpha_2, 3\alpha_1 + 2\alpha_2$。

(III) 我们有$h = \frac{n}{2} = 6$。

(IV)最高根为$\tilde{\alpha} = 3\alpha_1 + 2\alpha_2 = -\varepsilon_1 - \varepsilon_2 + 2\varepsilon_3$。我们有$(\tilde{\alpha}|\alpha_1) = 0, (\tilde{\alpha}|\alpha_2) = 3$。完整的 Dynkin 图为

![丁金图](https://i.imgur.com/3Q5z5QG.png)

(V) 逆系是向量的以下集合：

$$
\pm \alpha_1, \quad \pm (\alpha_1 + \alpha_2), \quad \pm (2\alpha_1 + \alpha_2), \quad \pm \frac{1}{3}\alpha_2,
$$
$$
\pm \frac{1}{3}(3\alpha_1 + \alpha_2), \quad \pm \frac{1}{3}(3\alpha_1 + 2\alpha_2).
$$

有10个根不与$\alpha_1$正交；我们有 $n(\beta, \alpha_1) = \pm 1$ 适合其中 4 个根，$n(\beta, \alpha_1) = \pm 3$ 适合另外 4 个，$n(\beta, \alpha_1) = \pm 2$ 适合 $\beta = \pm \alpha_1$。因此，$\Phi_R$ 的$\alpha_1$ 的平方长度为$4(4.1 + 4.9 + 2.4)^{-1} = \frac{1}{12}$。因此，$\Phi_R(x, y) = (x|y)/24$。我们现在应用§ 1, no. 12的公式(18)，与$x = y = \alpha_1$；这给出了

$$
2 + 4.\frac{1}{4} + 4.\frac{1}{4} = \gamma(R).\frac{1}{12}
$$

所以$\gamma(R) = 48$。

(VI) 和 (VII) 正根的一半和为

$$
\rho = 5\alpha_1 + 3\alpha_2.
$$

基本权$\omega_1$和$\omega_2$与$\alpha_2$和$\alpha_1$正交，因此与$2\alpha_1 + \alpha_2$和$3\alpha_1 + 2\alpha_2$成比例。我们有

$$
\omega_1 + \omega_2 = \rho = 5\alpha_1 + 3\alpha_2 = (2\alpha_1 + \alpha_2) + (3\alpha_1 + 2\alpha_2).
$$

因此，

$$
\omega_1 = 2\alpha_1 + \alpha_2, \quad \omega_2 = 3\alpha_1 + 2\alpha_2 = \tilde{\alpha}.
$$

例如，(VIII) Q(R) 由$\varepsilon_1 - \varepsilon_2$和$\varepsilon_1 - \varepsilon_3$生成。由(VI)和(VII)，P(R) = Q(R)。连接指标为 1。

(IX)指数家里有2个项；因为 1 和 $h - 1 = 5$ 是指数，所以它们是唯一的。

(X) 我们有 $(\overline{\alpha_1, \alpha_2}) = \frac{5\pi}{6}$，所以 W(R) 同构于阶 12 的二面角群。

(XI) Dynkin 图表唯一的自同构是恒等式，因此$\Lambda(R) = W(R)$和$w_0 = -1$。

### 14. 不可还原的非还原根系

不可约的、非约化的根系统可以通过使用 Props 从不可约的、约化的系统中获得。 § 1 的 13 和 14。 no. 4。对于每个整数$l \geq 1$，存在直到同构，唯一的秩$l$的不可约、非约根系统：令R为型B_l的根系，A集合为R的最短根；取 R 和 2A 的并。利用 no. 5 的记号，我们得到 $2l(l+1)$ 向量

$$
\pm \varepsilon_i,\ \pm 2\varepsilon_i,\ \varepsilon_i \pm \varepsilon_j\ (i < j).
$$

### 习题{#lie-vi-s4-exercises}

若R为根系，则用行列式1$W(R)$元素$W^+(R)$集合表示。

参见[习题为 § 4](exercises/s4/)。
