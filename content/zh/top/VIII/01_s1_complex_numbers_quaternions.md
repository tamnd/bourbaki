---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 1
section_title: Complex numbers, quaternions
lang: zh
source: top-v-x
pdf_pages: 0106-0111, 0129-0131
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF COMPLEX NUMBERS
      page: 0
      pdf_page: 106
    - "no": 2
      title: THE TOPOLOGY OF $\mathbf{C}$
      page: 0
      pdf_page: 108
    - "no": 3
      title: THE MULTIPLICATIVE GROUP $\mathbf{C}^*$
      page: 0
      pdf_page: 109
    - "no": 4
      title: THE DIVISION RING OF QUATERNIONS
      page: 0
      pdf_page: 110
statements: 9
exercises: 5
content_sha256: ec5faa873b1e3569cc6fbd7d5d2a9e92a26336e2f2709416ab831c4c77fb6b6b
translated_from: content/en/top/VIII/01_s1_complex_numbers_quaternions.md
translation_method: google
source_content_sha256: e5059e22ac4891308f9c35de29452c98d7b526ede462c73990757938a2903d64
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 83cfc305c1ef8400bd679bc507972f5b46526bf26f3c92dd5d42c8402125daa8
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 复数，四元数

### 1. 定义复数

多项式 $X^2 + 1$ 在 $\mathbf{R}$ 中没有根，因为 $x^2 + 1 \geq 1$ 对于所有 $x \in \mathbf{R}$；因此它在 $\mathbf{R}$ 上是不可约的。 [这是适用于任何有序域的类似结果的特殊情况。]

#### 定义 1 {#top-viii-s1-def-1 .statement tag=0BZV}

*域* $\mathbf{R}[X]/(X^2 + 1)$ *称为复数的域，记为*$\mathbf{C}$。 * $X$ *中* $\mathbf{C}$ *的典范像 * 表示为* $i$，*因此* $\mathbf{C}$ * 由域* $\mathbf{R}$ * 通过根* $i$ * 的代数伴随获得多项式* $X^2 + 1$。 * $\mathbf{C}$ *的*元素称为复数*。

从代数点的角度来看，域$\mathbf{C}$的重要性归因于以下基本定理：

#### 定理 1 {#top-viii-s1-thm-1 .statement tag=0BZW}

（达朗贝尔-高斯）。 *域* $\mathbf{C}$ *复数是代数闭*。

对于证明，足以确定 (i) $\mathbf{R}$ 中的每个元素 $\geq 0$ 都有一个 *平方根*，并且 (ii) 系数在 $\mathbf{R}$ 中的 *奇数* 次数的每个多项式有 *至少一个根*在$\mathbf{R}$。其中第一个断言已在章IV, § 3, no. 3中得到证明。对于第二个，如果 $f(X) = a_0 X^n + a_1 X^{n-1} + \cdots + a_n$ 是具有实数系数的奇数次数 $n$ ($a_0 \neq 0$) 的多项式，我们可以将 $x \neq 0$ 写为 $f(x) = a_0 x^n g(x)$，其中

$$
g(x) = 1 + \frac{a_1}{a_0 x} + \cdots + \frac{a_n}{a_0 x^n}
$$

趋于 $+1$，因为 $x$ 趋于 $+\infty$ 或 $-\infty$。因此，存在数$a > 0$，使得$f(a)$具有$a_0$的符号，并且$f(-a)$具有$-a_0$的符号；

因此根据 Bolzano 的定理 (章 IV, § 6, no. 1, 定理 2)，$f$ 在 $[—a, a]$ 中至少有一个根。

#### 注 1 {#top-viii-s1-n1-rem-1 .statement tag=0BZX}

利用域$\mathbf{C}$的拓扑性质，可以在不援引有序域理论的情况下证明定理1，其定义如下（no. 2）；请参阅§ 2、习题 2 以及级数的部分，专门用于代数拓扑，其中达朗贝尔-高斯的定理将显示为映射的次数结果的推论。

#### 注 2 {#top-viii-s1-n1-rem-2 .statement tag=0BZY}

由于 $\mathbf{C}$ 的次数 2 大于 $\mathbf{R}$，因此$\mathbf{C}$ 是同构以内的 $\mathbf{R}$ 除了 $\mathbf{R}$ 本身以外的唯一代数扩张，并且 $\mathbf{C}$ 中不包含域，其中包含 $\mathbf{R}$，$\mathbf{R}$ 和 $\mathbf{C}$ 除外。

我们知道$\mathbf{R}$可以与$\mathbf{C}$的子域等同，并且每个$z \in \mathbf{C}$都可以唯一地写成形式$x + iy$，其中$x$和$y$是实数； $x$称为$z$的实部分，记为$\Re(z)$； $y$ $z$ 的虚数部分，记为$\Im(z)$。 形式 $iy$（$y$实数）中的复数称为纯虚数。 关系 $x + iy = 0$（$x, y$实数）相当于$x = 0$和$y = 0$。

从 $i^2 = -1$、元素到 $\mathbf{C}$（由实部和虚部部分给出）满足计算规则如下：

$$
(x + iy) + (x' + iy') = (x + x') + i(y + y')
$$
$$
(x + iy)(x' + iy') = (xx' - yy') + i(xy' + x'y').
$$

特别是$(x + iy)(x - iy) = x^2 + y^2 \in \mathbf{R}$，因而，如果$x + iy \neq 0$，

$$
\frac{1}{x + iy} = \frac{x}{x^2 + y^2} - i \frac{y}{x^2 + y^2}.
$$

$\mathbf{C}$中多项式$X^2 + 1$的第二个根是$-i$；因而，除了恒等映射之外，$\mathbf{C}$中唯一使所有实数保持不变的自同构是映射$z = x + iy$到$x - iy$；后者用$\overline{z}$表示，（与一般的定义一致）称为复数共轭至$z$。我们有

$$
\Re(z) = \frac{1}{2}(z + \overline{z}) \quad \text{and} \quad \Im(z) = \frac{1}{2i}(z - \overline{z}).
$$

由于自同构，如果$f(z)$是具有实数系数的多项式，则对于所有$z \in \mathbf{C}$，我们都有$f(\overline{z}) = \overline{f(z)}$。

实数 $z \overline{z} = x^2 + y^2$ 被称为 $z$ 的代数范数，或者在不存在混淆风险的情况下简称为范数；它是实数$\geq 0$，只有$z = 0$才会消失。当$z$为实数时，实数$\sqrt{z \overline{z}} = \sqrt{x^2 + y^2} \geq 0$约化到$z$的绝对值，当$z$为任意时，我们仍然称其为$z$的绝对值，并用$|z|$表示复数。 关系 $|z| = 0$ 相当于 $z = 0$。如果$z$和$z'$是两个复数，则$zz'$的共轭是$\overline{zz'}$，因而$|zz'|^2 = zz'\overline{zz'} = |z|^2|z'|^2$，因而$|zz'| = |z|\cdot|z'|$：*乘积的绝对值是乘积因子的绝对值。*特别是，如果$z \neq 0$和$z' = 1/z$，我们有$|1/z| = |1/z|$。

最后，对于所有复数$z, z'$，我们有*三角形不等式*
$$
|z + z'| \leq |z| + |z'|.
$$

### 2. $\mathbf{C}$ 的拓扑

实平面 $\mathbf{R}^2$ 到 $\mathbf{C}$ 的映射 $(x, y) \to x + iy$ 是*双射的*；通过这个双射，我们可以*迁移*到$\mathbf{R}^2$的$\mathbf{C}$拓扑（cf.章VI, § 1, no. 5）。因此在$\mathbf{C}$上定义的拓扑与$\mathbf{C}$（章III, § 6, no. 7）的域结构*相容的*，因为它与$\mathbf{C}$（章VI, § 1, no. 5）的环结构兼容，并且， (3)、$1/z$在$\mathbf{C}$中0的补$\mathbf{C}^*$上连续。

如果我们赋予集合$\mathbf{C}$这个拓扑和之前定义的域结构（no. 1，定义1），我们就在$\mathbf{C}$结构上定义了一个*拓扑域* （章III, § 6, no. 7）；每当我们谈到拓扑或$\mathbf{C}$时，它的意思总是上面的拓扑。

以后我们一般将*认同* 集合 $\mathbf{C}$和$\mathbf{R}^2$视为拓扑空间；然后，$\mathbf{C}$的子域$\mathbf{R}$与$\mathbf{R}^2$的横坐标一致，因此称为*实轴*；同样，纵坐标称为*虚轴*（注，这*不是*$\mathbf{C}$的子域）。原点为 0、方向比为 $(1, 0)$（用 $\mathbf{R}_+$ 标识）的射线称为*正实半轴*；具有相同原点和方向比 $(-1, 0)$ 的相反射线称为*负实半轴*。

为了便于图示，我们使用 $\mathbf{R}^2$ 的表示（在初等解析几何中众所周知）和点的平面，其中绘制了两个垂直的坐标轴，分别代表 $\mathbf{C}$ 的实轴和虚轴（图 7）。

与每个拓扑域一样，具有复数系数的$n$复变量的每个*有理函数*在$\mathbf{C}^n$的每个点处都是*连续的，此时分母不会消失。

![图表显示复平面，轴标记为 x 和 y，点标记为 z = x + iy](https://i.imgur.com/3Q5z5QG.png)

图 7.

$\mathbf{C}$的置换$z \to \overline{z}$是连续的，因此是拓扑域$\mathbf{C}$的自同构。

事实上，它是拓扑域 $\mathbf{C}$ 中除恒等式自同构之外的唯一自同构（参见习题 4）。

函数 $\Re(z), \Im(z)$ 只是 $\mathbf{R}^2$ 的投影到它的因子上，因此是连续的；绝对值值$|z|$也是如此，因为它是$\mathbf{R}^2$中点$(x, y)$的欧氏范数（章VI, § 2, no. 1）。

绝对值的属性导致另一个证明，$\mathbf{C}$的拓扑与其域结构兼容（cf.章IX, § 3, no. 2）； $z + z'$ 的连续性源自三角形不等式 $|z + z'| \leq |z| + |z'|$； $zz'$ 是从关系得出的
$$
|zz' - z_0z'_0| = |z_0(z' - z'_0) + (z - z_0)z'_0 + (z - z_0)(z' - z'_0)| \\
\leq |z_0| \cdot |z' - z'_0| + |z'_0| \cdot |z - z_0| + |z - z_0| \cdot |z' - z'_0|;
$$
最后，$z^{-1}$的连续性来自关系
$$
|z_0^{-1} - z^{-1}| = |z|^{-1} \cdot |z - z_0| \cdot |z_0|^{-1}.
$$

### 3. 乘法群$\mathbf{C}^*$

从章III, § 6, no. 7可知，非零复数在乘法群$\mathbf{C}^*$上诱导的拓扑与$\mathbf{C}^*$的群结构兼容。由于$\mathbf{C}^*$在$\mathbf{C}$中开路，因此$\mathbf{C}^*$是局部紧拓扑群（章I, § 9, no. 7，命题13），因此是完备的（相对于乘法均匀性；cf. 章III, § 6, no. 8、命题8)。 实数$> 0$的乘法群$\mathbf{R}_+^*$是$\mathbf{C}^*$的闭子群。 另一个子群是值 1 的复数的集合 $\mathbf{U}$，它与$\mathbf{R}^2$ 的单位圆$S_1$ 一致，因此是紧凑的群。此外：

#### 命题 1 {#top-viii-s1-prop-1 .statement tag=0BZZ}

*拓扑群$\mathbf{C}^*$同构于拓扑群$\mathbf{R}^*$和$\mathbf{U}$的乘积。*

对于映射 $z \to \left( |z|, \frac{z}{|z|} \right)$ 是 $\mathbf{C}^*$ 到 $\mathbf{R}_+^* \times \mathbf{U}$ 的同胚 (章 VI, § 2, no. 3, 命题 3)；紧接着它就是群结构中的同构。

拓扑群 $\mathbf{R}_+^*$ 已知与加法群 $\mathbf{R}$ (章 V, § 4, 定理 1) 同构的；因此，拓扑群$\mathbf{C}^*$的研究被简化为$\mathbf{U}$的研究，我们将在§ 2中考虑。

### 4. 四元数的除法环

从定理 1 可以得出，域 $\mathbf{R}$ 是极大有序域，因此有限秩在 $\mathbf{R}$ 上的唯一非交换除法环是（直到同构）四元数除法环 $\mathbf{R}$；它用$\mathbf{H}$表示，称为实四元数的除法环（或者简称为四元数的除法环，不用担心混淆）。由于$\mathbf{H}$是秩 4超过域$\mathbf{R}$，我们可以在$\mathbf{H}$上的定义拓扑同胚于$\mathbf{R}^4$（章VI, § 1, no. 5）。准确地说，我们通常将认同$\mathbf{H}$和$\mathbf{H}$的典范基的$\mathbf{R}^4$、元素$i, i, j, k$分别与$\mathbf{R}^4$的典范基的向量、$e_0, e_1, e_2, e_3$进行识别。

我们记得$\mathbf{H}$的典范基的乘法表由公式给出

$$
i^2 = j^2 = k^2 = -1, \quad ij = -ji = k,
jk = -kj = i, \quad ki = -ik = j.
$$

$\mathbf{H}$的拓扑不仅与$\mathbf{H}$的环结构（章VI, § 1, no. 5）相容的，而且还与其除法环结构兼容；因为如果 $x$ 是非零四元数，则 $x^{-1}$ 的坐标是 $x$ 坐标的有理数函数，其分母不会消失。因此，赋予了拓扑的除法环$\mathbf{H}$是一个非交换拓扑除法环。 $\mathbf{H}$的四元数$a + bi$（$a, b$实数）形式a（拓扑）子域，与经常被识别的域$\mathbf{C}$同构的。

We have thus a third example of a locally compact, connected topological division ring, the others being $\mathbf{R}$ and $\mathbf{C}$. 事实上，这是唯一具有这两个属性的拓扑划分环。

我们从代数知道四元数$x = x_0 + x_1 i + x_2 j + x_3 k$的约化范数是

$$
N(x) = x_0^2 + x_1^2 + x_2^2 + x_3^2 = ||x||^2
$$

（因此它是欧氏范数 $x$ 的平方）。自从

$$
N(xy) = N(x)N(y),
$$

由此可见，范数 1 的所有四元数中的集合，与球体$S_3$相同，形式是非零四元数乘法群$\mathbf{H}^*$的紧凑子群。

#### 命题 2 {#top-viii-s1-prop-2 .statement tag=0C00}

The multiplicative group $\mathbf{H}^*$ of non-zero quaternions is a topological group isomorphic to the product of its subgroups $\mathbf{R}_+^*$ and $S_3$.

每个四元数$x / o$都可以写成$x \cdot z$，其中$z$是范数为1的四元数；由于$H^*$的$\|xx'\| = \|x\|\cdot\|x'\|$、映射$x \to (\|x\|, x_1, x_2)$到$\mathbf{R}_+^* \times S_2$是群结构的同构，而从章VI, § 2, no. 2、命题2，则是同态 $H^*$ 到$\mathbf{R}_+^* \times S_2$。

#### 注 1 {#top-viii-s1-n4-rem-1 .statement tag=0C01}

利用关系$\|x + y\| = \|x\| + \|y\|$和$\|xy\| = \|x\|\cdot\|y\|$，可以直接证明，就像no. 2中复数的域一样，$\mathbf{R}^4$的拓扑与$H$的环结构相容（cf.） 章IX, § 3, no. 2）。

#### 注 2 {#top-viii-s1-n4-rem-2 .statement tag=0C02}

经证明，球体$S_1$和$S_n$可以携带与其拓扑兼容的群结构。稍后我们将看到，对于除了1和3之外的每个整数$n$，$S_n$上不存在与$S_n$的拓扑兼容的群结构。

#### 注 3 {#top-viii-s1-n4-rem-3 .statement tag=0C03}

群 $S_2$ 中的每个点都有邻域同构于 $\mathbf{R}^3$ (章 VI, § 2, no. 4, 命题 5)，但 $S_4$ 不局部同构于 $\mathbf{R}^3$；因为如果是的话，它会是阿贝尔的，因为它是连接的（章VII, § 2, no. 2，定理1），但事实并非如此，因为$i$和$j$属于到$S_3$和$ij \neq ji$（cf.） 章V, § 3）。

### 习题 {#top-viii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
