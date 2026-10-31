---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 8
section_title: Rings
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 96-114, 171-174
pdf_pages: 0120-0138, 0195-0198
extraction: ocr
subsections:
    - "no": 1
      title: RINGS
      page: 96
      pdf_page: 120
    - "no": 2
      title: CONSEQUENCES OF DISTRIBUTIVITY
      page: 98
      pdf_page: 122
    - "no": 3
      title: EXAMPLES OF RINGS
      page: 101
      pdf_page: 125
    - "no": 4
      title: RING HOMOMORPHISMS
      page: 102
      pdf_page: 126
    - "no": 5
      title: SUBRINGS
      page: 103
      pdf_page: 127
    - "no": 6
      title: IDEALS
      page: 103
      pdf_page: 127
    - "no": 7
      title: QUOTIENT RINGS
      page: 105
      pdf_page: 129
    - "no": 8
      title: SUBRINGS AND IDEALS IN A QUOTIENT RING
      page: 106
      pdf_page: 130
    - "no": 9
      title: MULTIPLICATION OF IDEALS
      page: 107
      pdf_page: 131
    - "no": 10
      title: PRODUCT OF RINGS
      page: 108
      pdf_page: 132
    - "no": 11
      title: DIRECT DECOMPOSITION OF A RING
      page: 110
      pdf_page: 134
    - "no": 12
      title: RINGS OF FRACTIONS
      page: 112
      pdf_page: 136
statements: 32
exercises: 16
content_sha256: 1f094337b610cf8ee4592ae6dfca5c67b1e2c5a4bd510acf8e164b0bf76895cb
translated_from: content/en/alg/I/08_s8_rings.md
translation_method: google
source_content_sha256: 9e2e678718b8b04bcfb806c30df7ec34dec70b897c7a14a41eee1a9ca40499a1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 75e2174d60d6adf608583b457bd44cb153490ce77a18cfefbd61c9a5b09d7b2b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 8。 环

### 1.环

#### 定义 1 {#alg-i-s8-def-1 .statement tag=05H2}

*环是集合* $\mathbf{A}$ *与合成的两个律分别称为加法和乘法、满足以下公理*：

(AN I) *在加法* $\mathbf{A}$ *下是可交换的群*。
(AN II) *乘法具有结合律并拥有单位元素*。
(AN III) *乘法对于加法* 是可分配的。
*环* $\mathbf{A}$ *如果其乘法是可交换的，则称其是可交换的*。

其中，$(x, y) \mapsto x + y$表示加法，$(x, y) \mapsto xy$乘法； $0$ 表示加法的单位元素，$1$ 乘法。最后，$-x$表示加法下$x$的负数。因此，环的公理由以下恒等式表示：

$$
\begin{array}{ll}
(1) & x + (y + z) = (x + y) + z \quad \text{(associativity of addition)} \\
(2) & x + y = y + x \quad \text{(commutativity of addition)} \\
(3) & 0 + x = x + 0 = x \quad \text{(zero)} \\
(4) & x + (-x) = (-x) + x = 0 \quad \text{(negative)} \\
(5) & x(yz) = (xy)z \quad \text{(associativity of multiplication)} \\
(6) & x.1 = 1.x = x \quad \text{(unit element)} \\
(7) & (x + y).z = xz + yz \\
(8) & x.(y + z) = xy + xz \quad \text{(distributivity)}
\end{array}
$$

最后，如果$xy = yx$对于$\mathbf{A}$中的$x, y$来说，环$\mathbf{A}$是可交换的。

单独使用加法 $\mathbf{A}$ 是一个可交换的群，称为 $\mathbf{A}$ 的 *加法群*。对于所有$x \in \mathbf{A}$，我们将定义左侧位似$\gamma_x$和右侧位似$\delta_x$乘以$\gamma_x(y) = xy$，$\delta_x(y) = yx$。通过公式（7）和（8），$\gamma_x$和$\delta_x$是$\mathbf{A}$的加法群的自同态，因此映射零到零并且负对负。所以

$$
\begin{align*}
(9) & \quad x.0 = 0.x = 0 \\
(10) & \quad x.(-y) = (-x).y = -xy;
\end{align*}
$$
由此可知 $(-x)(-y) = -((-x).y) = -(-xy)$, 从而
$$(11) \quad (-x)(-y) = xy.$$
公式 (10) 和 (11) 构成*符号规则*。由此可见
$$-x = (-1)x = x(-1)$$
和$(-1)(-1) = 1$。

从 (11) 可以得出 $n$ 上的归纳
$$(12) \quad (-x)^n = \begin{cases} x^n & \text{if } n \text{ is even} \\ -x^n & \text{if } n \text{ is odd.} \end{cases}$$

当我们说到环$\mathbf{A}$的*可取消*元素、*可逆*元素、*可改变*元素、*中心的*元素、*集中器*或*中心*时，所有这些概念都会指代乘法 $\mathbf{A}$。如果$x, y \in \mathbf{A}$和$y$可逆，则当$\mathbf{A}$可交换时，$\mathbf{A}$的元素$xy^{-1}$也表示为$x/y$。 $\mathbf{A}$可逆元集合稳定在乘法以下。在乘法诱导的律下，群称为$\mathbf{A}$的*乘法群*，有时用$\mathbf{A}^*$表示。

设$x, y$在$\mathbf{A}$中。如果存在$y' \in \mathbf{A}$使得$x = y'y$（或$x = yy'$），则$x$被称为$y$的*左*（或*右*）*倍数*；也有人说 $y$ 是一个*右*（分别是。

左）x 的除子。当A是可交换的时，不需要区分“左”和“右”。

与上述术语一致，每一个元素$y \in \mathbf{A}$都会被视为左右除子为0；但是，由于语言滥用，一般来说，项“0的右（或左）除子”被保留给元素$y$，使得在满足关系$xy = 0$（或$yx = 0$）中存在$x \neq 0$。在其他字中，零的右（或左）除子是右（或左）不可取消的元素。

让$x \in \mathbf{A}$。如果存在整数 $n > 0$ 和 $x^n = 0$，则$x$ 称为幂零。 元素 $1 - x$ 是可逆的，其逆等于
$$
1 + x + x^2 + \cdots + x^{n-1}.
$$

由于 A 是加法下的交换律群，因此定义了 $n \in \mathbf{Z}$ 和 $x \in \mathbf{A}$ 的元素 $nx$ (§ 2, no. 8)。由于$\gamma_x$和$\delta_x$是加法群A、$\gamma_x(ny) = n\gamma_x(y)$和$\delta_y(nx) = n\delta_y(x)$的自同态，从而
$$
x.(ny) = (nx).y = n.(xy).
$$
特别是$nx = (n.1)x$。

集合加法和乘法满足公理为环，但保证乘法下存在单位元素，则称为伪环。

### 2.推论 / 分配律

乘法的分配律相对于加法允许我们应用命题 1 of § 3, no. 4，这给出
$$
\prod_{i=1}^n \left( \sum_{\lambda \in L_i} x_{i,\lambda} \right) = \sum_{\alpha_1, \ldots, \alpha_n} \prod_{i=1}^n x_{i, \alpha_i}
$$
其中和扩展在序列$(\alpha_1, \ldots, \alpha_n)$属于到$L_1 \times \cdots \times L_n$，对于$i = 1, \ldots, n$，环A的元素的$(x_{i,\lambda})_{\lambda \in L_i}$家庭是有限支撑。

#### 命题 1 {#alg-i-s8-prop-1 .statement tag=05H3}

设 A 为交换环和 $(x_\lambda)_{\lambda \in L}$ A 的元素的有限族。对于正整数 $\beta = (\beta_\lambda)_{\lambda \in L}$ 的每个族，令 $|\beta| = \sum_{\lambda \in L} \beta_\lambda$。然后
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}.
$$
我们将公式 (13) 与$L_i = L$ 相结合，将$x_{i,\lambda} = x_\lambda$ 应用于$1 \leq i \leq n$。然后
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{\alpha_1, \ldots, \alpha_n} x_{\alpha_1} \cdots x_{\alpha_n},
$$
和延伸至所有序列$\alpha = (\alpha_1, \ldots, \alpha_n) \in L^n$。

设$\alpha$在$L^n$内；对于所有$\lambda \in L$，让$U_\lambda^\alpha$表示整数$i$的集合，这样$1 \leq i \leq n$和$\alpha_i = \lambda$，并让$\Phi(\alpha) = (U_\lambda^\alpha)_{\lambda \in L}$。 $\Phi$是$L^n$双射到由$L$索引的$\{1, 2, \ldots, n\}$划分集合上，是直接的。对于所有$\beta \in \mathbf{N}^L$使得$|\beta| = n$，让$L_\beta^n$表示$\alpha \in L^n$的集合，使得$\mathrm{Card}\ U_\beta^\alpha = \beta_\lambda$对于所有$\lambda \in L$。由此可见，家庭$(L_\beta^n)_{|\beta|=n}$是$L^n$的划分，并且

$$
\mathrm{Card}\ L_\beta^n = \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!}
$$

（§ 5, no. 5）。

最后，对于$\alpha \in L_\beta^n$，

$$
x_{\alpha_1} \cdots x_{\alpha_n} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_{\alpha_i} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_\lambda = \prod_{\lambda \in L} x_\lambda,
$$

从而

$$
\sum_{(\alpha_1, \ldots, \alpha_n)} x_{\alpha_1} \cdots x_{\alpha_n} = \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} x_{\alpha_1} \cdots x_{\alpha_n}
= \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}
= \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} x_\lambda^{\beta_\lambda}
$$

公式 (14) 因此从 (15) 得出。

#### 推论 1（二项式公式）{#alg-i-s8-prop-1-cor-1 .statement tag=05H4}

*设 x 和 y 为交换环 A 中的两个元素。那么*：

$$
(x + y)^n = \sum_{p=0}^n \binom{n}{p} x^p y^{n-p}.
$$

将公式 (14) 应用于 $L = \{1, 2\}$、$x_1 = x$ 和 $x_2 = y$ 给出

$$
(x + y)^n = \sum_{p+q=n} \frac{n!}{p! q!} x^p y^q,
$$

和延伸超过正整数 $p, q$ 的有序对和 $p + q = n$。由此立即得出二项式公式（*集合理论*，III, § 5, no. 8）。

#### 推论 2 {#alg-i-s8-prop-1-cor-2 .statement tag=05H5}

*设A为A的交换环、X集合、$\mathbf{u} = (u_x)_{x \in X}$和$\mathbf{v} = (v_x)_{x \in X}$两个族元素。令$\mathbf{u} + \mathbf{v}$表示族$(u_x + v_x)_{x \in X}$。对于所有$\lambda \in \mathbf{N}^{(X)}$，我们写为$\lambda! = \prod_{x \in X} \lambda(x)!$。那么对于所有$\alpha \in \mathbf{N}^{(X)}$，在§ 7, no. 8的记号中，

$$
(\mathbf{u} + \mathbf{v})^\alpha = \sum_{\beta + \gamma = \alpha} \frac{\alpha!}{\beta! \gamma!} \mathbf{u}^\beta \mathbf{v}^\gamma.
$$

对于$x \in X$，

$$
(u_x + v_x)^{\alpha(x)} = \sum_{m+n=\alpha(x)} \frac{\alpha(x)!}{m! n!} u_x^m v_x^n
$$

由推论 1。将这些方程中的乘积代入 $x \in X$ 并使用 (13)，我们得到推论。

#### 命题 2 {#alg-i-s8-prop-2 .statement tag=05H6}

*设$A$为环、$x_1, \ldots, x_n$元素、$A$和$I = \{1, 2, \ldots, n\}$。对于$H \subset I$，我们写为$x_H = \sum_{i \in H} x_i$。然后*

$$
(-1)^n \sum_{\sigma \in S_n} x_{\sigma(1)} \cdots x_{\sigma(n)} = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

*特别是，如果 $A$ 是可交换的，

$$
(-1)^n n! x_1 x_2 \cdots x_n = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

设$C$为$I$的映射到$\{0, 1\}$的集合。如果将每个$H \subset I$映射到其特征函数，则将$\mathscr{P}(I)$映射到$C$，即可获得双射。因此，(16) 的右侧等于：

$$
\sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \left( \sum_{i \in I} a(i) x_i \right)^n
$$
$$
= \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \sum_{(i_1, \ldots, i_n) \in I^n} a(i_1) \ldots a(i_n) x_{i_1} \ldots x_{i_n}
$$
$$
= \sum_{(i_1, \ldots, i_n) \in I^n} c_{i_1 \ldots i_n} x_{i_1} \ldots x_{i_n}
$$

哪里

$$
c_{i_1 \ldots i_n} = \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n).
$$

(1) 假设$(i_1, \ldots, i_n)$不是$I$的置换。存在与$i_1, \ldots, i_n$不同的$j \in I$。令 $C'$ 为 $a \in C$ 的集合，使得 $a(j) = 0$。对于所有$a \in C'$，令$a^*$为$a$的和以及$\{j\}$的特征函数。然后 $a^*(1) + \cdots + a^*(n) = a(1) + \cdots + a(n) + 1$ 因此

$$
c_{i_1 \ldots i_n} = \sum_{a \in C'} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n) + (-1)^{a^*(1)+\cdots+a^*(n)} a^*(i_1) \ldots a^*(i_n)
$$
$$
= \sum_{a \in C'} ((-1)^{a(1)+\cdots+(n)} + (-1)^{a(1)+\cdots+a(n)+1}) a(i_1) \ldots a(i_n) = 0.
$$

(2) 假设存在$\sigma \in S_n$使得$i_1 = \sigma(1), \ldots, i_n = \sigma(n)$。那么$a(i_1) \ldots a(i_n) = 0$除非$a$只需要值1。因此$c_{i_1 \ldots i_n} = (-1)^n$。

### 3. 例环

I.零环。设 A 为环。对于A中的$0 = 1$，A由单个元素组成是充分必要的。 条件显然已经足够了。另一方面，如果$0 = 1$，那么对于所有$x \in A$，$x = x.1 = x.0 = 0$。这样的环称为零环。

有理整数的II.环。由于加法在§ 2, no. 5中定义，乘法在§ 2, no. 6中定义，$\mathbf{Z}$是交换环。 记号 0, 1, $-x$ 与之前介绍的记号一致。

*三。实值函数的环。令 I 为实数的集合 $\mathbf{R}$ 中的一个区间，并令 A 为在 I 上用实数值定义的连续函数的集合。两个函数 $f$ 和 $g$ 中的和 $f + g$ 和乘积 $f.g$ 定义为
$$(f + g)(t) = f(t) + g(t), \quad (fg)(t) = f(t)g(t) \quad (t \in I).$$
得到交换环，其中单位元是常数1.*

*四。卷积伪环。令 E 为 $\mathbf{R}$ 上的实值连续函数的集合，其中零在有界区间之外。两个函数的和定义如 III 中，但乘积现在定义为
$$(fg)(t) = \int_{-\infty}^{\infty} f(s)g(t-s)\ ds$$
（“卷积乘积”）。这样就得到了一个可交换的伪环，它不是环（cf.积分，VIII, §4）。*

环 A 的 V. 逆环。设 A 为环。与 A 相同的加法和乘法 $(x, y) \mapsto yx$ 的集合 A 通常用$A^0$ 表示。它是环（称为A的逆环），与A具有相同的零和相同的单位，并且当且仅当A是可交换的时，它与A有重合。

交换律群的 VI. 自同态环。设 G 是可加写的交换律群。令E表示G的自同态的集合。给定E中的$f$和$g$，G到G的映射$f + g$和$fg$定义为
$$(f + g)(x) = f(x) + g(x), \quad (fg)(x) = f(g(x)) \quad (x \in G).$$
通过 § 1, no. 5、命题 5，$f + g$ 是 G 的自同态，因此显然也是 $fg = f \circ g$。到§ 4, no. 8，E 是加法下的（可交换的）群。 乘法显然是结合律并且有单位元素 $\mathrm{Id}_G$。同样对于E中的$f, g$和$h$，我们写成$\phi = f.(g + h)$；对于所有$x \in G$，
$$\phi(x) = f((g + h)(x)) = f(g(x) + h(x)) = f(g(x)) + f(h(x))$$
对于 $f$ 是 G 的自同态；因此 $\phi = fg + fh$ 显然
$$(g + h)f = gf + hf.$$

因此 E 是一个（一般而言不可交换的）环，称为 G* 的 *自同态环。

VII. *零平方的伪环。* 如果 $xy = 0$ 对于所有 $x, y \in A$，则称伪环 A 为零平方。设 G 是可交换的群。如果给集合 G 赋予群 G 的加法和乘法 $(x, y) \mapsto 0$，则获得零平方的伪环。如果 $G = \{0\}$，则仅为环，在这种情况下，它为零环。

### 4.环同态

#### 定义 2 {#alg-i-s8-def-2 .statement tag=05H7}

*设A和B为两个环。 A 到 B 的态射或同态是 A 到 B 的任意映射 f 满足关系：*

$$
f(x + y) = f(x) + f(y), \quad f(xy) = f(x) \cdot f(y), \quad f(1) = 1,
$$

*对于所有*$x, y$*在A*中。

两个环同态中的合成是环同态。设A和B是A到B的两个环和$f$映射；对于$f$是同构，它是双射同态是充分必要的；在这种情况下，$f^{-1}$是B到A的同态。环A到自身的同态称为A的*自同态*。

设$f : A \to B$为环同态。 映射$f$是A的加法群的同态到B的加法群；特别是，对于所有$x \in A$，$f(0) = 0$和$f(-x) = -f(x)$。 A的可逆元的$f$下的像是B的可逆元，并且将A的乘法群的$f$诱导同态转化为B的乘法群。

#### 例 {#alg-i-s8-n4-exa-1 .statement tag=05H8}

(1) 设A为环。立即可见，$\mathbf{Z}$到A的映射$n \mapsto n \cdot 1$是$\mathbf{Z}$到A的唯一同态。特别是，$\mathbf{Z}$的恒等映射是环$\mathbf{Z}$的唯一内同态。

特别地，取A为加法群$\mathbf{Z}$（no. 3，例VI）中的自同态环。 $\mathbf{Z}$的映射$n \mapsto n \cdot 1$进入A是$\mathbf{Z}$（§ 2, no. 6）中乘法的构造到A的$\mathbf{Z}$同构到A。

(2) 设$a$为环A的可逆元。映射$x \mapsto axa^{-1}$为A的自同态

$$
a(x + y)a^{-1} = axa^{-1} + aya^{-1},
$$
$$
a(xy)a^{-1} = (axa^{-1})(aya^{-1}).
$$

它是双射的，因为关系$x' = axa^{-1}$等价于$x = a^{-1}x'a$。因此，它是环 A 的自同构，称为与 $a$ 伴随的 *内自同构*。

### 5.子环

#### 定义 3 {#alg-i-s8-def-3 .statement tag=05H9}

设$A$为环。 $A$的子环是$A$的任意子集$B$，即加法下$A$的子群，在乘法下稳定，并且$A$的包含单位。

上面的条件可以写成如下

$$
0 \in B, \quad B + B \subset B, \quad -B \subset B, \quad B.B \subset B, \quad 1 \in B.
$$

如果$B$是$A$的子环，则由$A$上的那些诱导出加法和乘法，从而使其变成环。 $B$到$A$的典范嵌入是环同态。

#### 例 {#alg-i-s8-n5-exa-1 .statement tag=05HA}

(1) 加法群 $\mathbf{Z}$ 中的每个子群，其中包含 1 等于$\mathbf{Z}$。因此$\mathbf{Z}$是$\mathbf{Z}$中唯一的子环。

(2) 设$A$为环且$(A_t)_{t \in I}$为$A$的子环族； $\bigcap_{t \in I} A_t$是$A$的子环是直接的。 In particular, the intersection of the subrings of $A$ containing a subset $X$ of $A$ is a subring called the subring of $A$ generated by $X$.

(3) 设$X$为环$A$中的子集。 $A$中$X$的集中器是$A$的子环。特别地，$A$中的中心是$A$中的子环。

(4) 设$G$是带有运算符的可交换群；让$\Omega$表示运算符的集合，并在$G$上表示$\Omega$的$\alpha \mapsto f_\alpha$作用。令$E$为不带运算符$G$的群的自同态环，以及带运算符$G$的群的自同态的$F$集合。通过定义，$F$ 由自同态 $\phi$ 和 $G$ 组成，使得 $\phi \cdot f_\alpha = f_\alpha \cdot \phi$ 代表所有 $\alpha \in \Omega$。因此$F$是环$E$中的子环。 $F$ 被称为群的自同态环，运算符为 $G$ (cf. II, § 1, no. 2)。令$F_1$为由$f_\alpha$生成的$E$的子环。那么$F$就是$F_1$在$E$的中心化子。

### 6.理想

#### 定义 4 {#alg-i-s8-def-4 .statement tag=05HB}

设$A$为环。如果$A$的加法群的子群且关系$a \in A, x \in a$隐含$ax \in a$（或$xa \in a$），则$A$的子集$a$被称为左（或右）理想。如果$a$既是$A$的左理想又是右理想，则称$A$的双边理想。

左理想的定义可以表示为关系

$$
0 \in a, \quad a + a \subset a, \quad A.a \subset a
$$

关系 $-a \subset a$ 继公式 $(-1).x = -x$ 和 $A.a \subset a$ 之后。对于所有$x \in A$，令$\gamma_x$为$A$的映射$a \mapsto xa$到$A$； 作用 $x \mapsto \gamma_x$ 给出群的$A$ 结构的加法群 $A^+$，其中$A$ 的运算符作为集合的运算符。 $A$的左理想正好是$A^+$的子群，在作用下是稳定的。

环$A$中的左理想正是逆环$A^0$的右理想。在交换环中，三个类的理想是相同的；它们被简单地称为理想。

#### 例 {#alg-i-s8-n6-exa-1 .statement tag=05HC}

(1) 设$A$为环。 集合 $A$是$A$的双面理想； 集合由……组成为 0，称为零理想值，有时用 0 或 $(0)$ 表示，而不是 $\{0\}$。

(2) 对于$A$的每一个元素$a$，$a$的左倍数的集合$A.a$都是左理想；同样，集合$a.A$是一个正确的理想。当$a$在$A$的中心时，$A.a = a.A$；这个理想称为$a$生成的主理想，用$(a)$表示。 $(a) = A$当且仅当$a$可逆。

(3) 设$M$为$A$中的子集。 元素 $x \in A$的集合，使得$xy = 0$对于所有$y \in M$来说是$A$的左理想，称为$M$的左湮没子。 $M$的右湮灭子的定义类似。

(4) $A$ 的左（或右，两侧）的每交都是一个左（或右，两侧）理想。给定子集 $X$ 和 $A$，因此存在最小的左（右，两侧）理想包含 $X$；它被称为由 $X$ 生成的左（或右、两侧）理想。

令$a$为$A$的左理想。 条件 $1 \notin a, a \neq A$ 显然是等价的。

#### 定义 5 {#alg-i-s8-def-5 .statement tag=05HD}

*令$A$为环。通过滥用语言，如果左理想 $a$ 是与 $A$ 不同的左理想中的集合中的极大元素，则称其为最大。*

在其他字中，如果$a \neq A$且$A$包含$a$的唯一左理想是$a$和$A$，则$a$最大。

#### 定理 1（克鲁尔）{#alg-i-s8-thm-1 .statement tag=05HE}

*令$A$为环，且$a$与$A$不同的$A$左理想。存在最大理想 $m$ $A$ 包含 $a$。*

将 $A$ 视为在 $A$ 左侧乘法的加法群 $A^+$ 上进行操作。那么$A$的左理想就是$A^+$的稳定子群。因此，定理由§ 4, no. 3得出，命题3适用于$A^+$的子集$P = \{1\}$。

#### 命题 3 {#alg-i-s8-prop-3 .statement tag=05HF}

*令$A$为环，$(x_\lambda)_{\lambda \in L}$为$A$的元素和$a$（分别为$b$）和$\sum_{\lambda \in L} a_\lambda x_\lambda$的集合，其中$(a_\lambda)_{\lambda \in L}$为有限支撑元素 $A$ 的家庭（分别为$\sum_{\lambda \in L} a_\lambda x_\lambda b_\lambda$，其中$(a_\lambda)_{\lambda \in L}, (b_\lambda)_{\lambda \in L}$ 是有限支撑元素 $A$ 的家庭）。那么$a$（或$b$）是元素$x_\lambda$生成的$A$的左（或两侧）理想。

公式

$$
0 = \sum_{\lambda \in L} 0.x_\lambda
$$
$$
\sum_{\lambda \in L} a_\lambda x_\lambda + \sum_{\lambda \in L} a'_\lambda x_\lambda = \sum_{\lambda \in L} (a_\lambda + a'_\lambda)x_\lambda
$$
$$
a.\sum_{\lambda \in L} a_\lambda x_\lambda = \sum_{\lambda \in L} (aa_\lambda)x_\lambda
$$

证明$a$是左理想。令$a'$为左理想，使得$x_\lambda \in a'$适用于所有$\lambda \in L$，并令$(a_\lambda)_{\lambda \in L}$为$A$中的有限支撑的家庭。那么$a_\lambda x_\lambda \in a'$对于所有$\lambda \in L$，从而$\sum_{\lambda \in L} a_\lambda x_\lambda \in a'$；因此$a \subset a'$。因此$a$是由$x_\lambda$生成的$A$的左理想。 $b$ 的论证是类似的。

#### 命题 4 {#alg-i-s8-prop-4 .statement tag=05HG}

*设$A$为环，$(a_\lambda)_{\lambda \in L}$为$A$的左理想族。 $\bigcup_{\lambda \in L} a_\lambda$ 生成的左理想由和 $\sum_{\lambda \in L} y_\lambda$ 组成，其中 $(y_\lambda)_{\lambda \in L}$ 是一个具有有限支撑的族，使得 $y_\lambda \in a_\lambda$ 对于所有 $\lambda \in L$。*

对于所有 $\lambda \in L$，令 $a$ 为和 $\sum_{\lambda \in L} y_\lambda$ 的集合，其中$y_\lambda \in a_\lambda$。 公式 $\sum_{\lambda \in L} x_\lambda + \sum_{\lambda \in L} y_\lambda = \sum_{\lambda \in L} (x_\lambda + y_\lambda)$和$a \cdot \sum_{\lambda \in L} x_\lambda = \sum_{\lambda \in L} a x_\lambda$表明$a$是$A$的左理想。设$\lambda \in L$和$x \in a_\lambda$；将 $\mu \neq \lambda$ 写为 $y_\lambda = x$ 和 $y_\mu = 0$；然后$x = \sum_{\lambda \in L} y_\lambda$，从而$x \in a$，最后$a_\lambda \subset a$。如果对于所有 $\lambda \in L$ 都有一个左理想 $a'$ 包含 $a_\lambda$，则显然包含 $a$，因此 $a$ 由 $\bigcup_{\lambda \in L} a_\lambda$ 生成。

由$\bigcup_{\lambda \in L} a_\lambda$生成的理想$a$称为左理想*$a_\lambda$的*和，记为$\sum_{\lambda \in L} a_\lambda$（cf.II, § 1, no. 7）。特别地，两个左理想的和$a_1 + a_2$由和$a_1 + a_2$组成，其中$a_1 \in a_1$和$a_2 \in a_2$。

### 7.商环

设$A$为环。如果$a$是$A$的双面理想，$A$的两个元素$x$和$y$被认为是*全等模*$a$，写作$x \equiv y$（模$a$）或$x \equiv y(a)$，如果$x - y \in a$。这是$A$的等价关系。 关系$x \equiv y(a)$和$x' \equiv y'(a)$意味着$x + x' \equiv y + y'(a)$，$a$的$xx' \equiv xy'(a)$是左理想，$xy' \equiv yy'(a)$对于$a$是右理想，从而$xx' \equiv yy'(a)$。相反，如果$R$在$A$上是等价关系，与加法和乘法兼容，则$x \equiv 0$ mod的集合$a$。 $R$ 是双面理想，$x \equiv y$ mod。 $R$ 相当于 $x \equiv y$ mod。 $a$。

令$A$为环，且$a$为$A$的双面理想。 $A/a$ 表示 $A$ 除以等价关系 $x \equiv y(a)$ 的商集，加法和乘法为$A$ 的商（$§ 1$、no. 6、定义） 11）。我们证明 $A/a$ 是环：

(a) 在加法下，$A/a$是加法群与$A$的商交换群除以子群$a$。

(b) 在乘法下，$A/a$是幺半群（$§ 2$，no. 1）。

(c) 令$\xi, \eta, \zeta$在$A/a$中，并令$\pi : A \to A/a$为典范映射；我们选择元素 $x, y, z$ 在 $A$ 中，这样 $\pi(x) = \xi, \pi(y) = \eta$ 和 $\pi(z) = \zeta$。然后
$$
\xi(\eta + \zeta) = \pi(x)\pi(y + z) = \pi(x(y + z)) = \pi(xy + xz)
= \pi(x)\pi(y) + \pi(x)\pi(z) = \xi\eta + \xi\zeta
$$
关系$(\xi + \eta)\zeta = \xi\zeta + \eta\zeta$同样成立。

#### 定义 6 {#alg-i-s8-def-6 .statement tag=05HH}

设$A$为环，$a$为$A$的双面理想。 $A$除以$a$的商环，用$A/a$表示，是$A$除以等价关系$x \equiv y(a)$的商集，其中加法和乘法是$A$上的商。

环$A/\{0\}$与$A$同构的，$A/A$是零环。

#### 定理 2 {#alg-i-s8-thm-2 .statement tag=05HI}

令$A$为环，且$a$为$A$的双面理想。
(a) $A$ 到$A/a$ 的典范映射 $\pi$ 是环同态。
(b) 设$B$为环，并将$A$的$f$同态代入$B$。如果$f(a) = \{0\}$，则$A/a$到$B$中存在且仅有一个同态$\bar{f}$使得$f = \bar{f} \circ \pi$。

由构造、$\pi(x + y) = \pi(x) + \pi(y)$ 和 $\pi(xy) = \pi(x)\pi(y)$ 乘坐 $A$ 内的 $x, y$；并且$\pi(1)$是$A/a$、从而的单位$\varepsilon$(a)。

设$A^+$为$A$的加法群，$B^+$为$B$的加法群；因为$f$是$A^+$的同态到$B^+$，零在$A^+$的子群$a$，所以存在（§ 4, no. 4，命题 5）一个且仅有一个同态将$A^+/a$的$\bar{f}$转化为$B^+$，使得$f = \bar{f} \circ \pi$。设$\xi, \eta$在$A/a$中； 选择$x, y$在$A$与$\pi(x) = \xi$和$\pi(y) = \eta$；然后$\xi \eta = \pi(xy)$，从而

$$
\bar{f}(\xi \eta) = \bar{f}(\pi(xy)) = f(xy) = f(x)f(y) = \bar{f}(\xi)\bar{f}(\eta)
$$

和$\bar{f}(\varepsilon) = f(\pi(1)) = f(1)$，因此$\bar{f}$是环同态。

#### 定理 3 {#alg-i-s8-thm-3 .statement tag=05HJ}

设$A$和$B$为$A$的环和$f$同态到$B$。
(a) $f$ 的核 $a$ 是$B$ 的双面理想。
(b) $f$ 的像 $B' = f(B)$ 是$B$ 的子环。
(c) 令 $\pi : A \to A/a$ 和 $i : B' \to B$ 为规范的态射。 $A/a$到$B'$中存在且仅有一个态射$\bar{f}$，使得$f = i \circ \bar{f} \circ \pi$和$\bar{f}$是同构。

因为$f$是$A$的加法群到$B$的态射，所以$a$是$A$的子群。如果$x \in a$和$a \in A$，则$f(ax) = f(a)f(x) = 0$，因此$ax \in a$，类似地$xa \in a$；因此$a$是$A$的双面理想。 断言 (b) 是显而易见的。由于$f$是$a$上的零，因此$A/a$中存在态射$\bar{f}$进入$B'$，使得$f = i \circ \bar{f} \circ \pi$（定理2）。 $\bar{f}$的唯一性以及$\bar{f}$是同构的事实源自集合理论，II, § 6, no. 4。

### 8.子环和商环的理想

#### 命题 5 {#alg-i-s8-prop-5 .statement tag=05HK}

令$A$和$A'$为$A$的两个环、$f$同态分解为$A'$和$f$的$a$核。
(a) 设$B'$为$A'$中的子环。那么$B = f^{-1}(B')$就是$A$包含$a$中的子环。如果 $f$ 是满射，则当经过到 $B/a$ 的商同构到 $B'$ 时，$f(B) = B'$ 和 $f|_B$ 定义。
(b) 令 $b'$ 为 $A'$ 的左（或右、两侧）理想。那么$b = f^{-1}(b')$是$A$包含$a$的左（或右，两侧）理想。

(c) *如果$b'$是$A'$的双面理想，则规范态射$A' \to A'/b'$和$f : A \to A'$定义的复合映射，当经过为商时，单射态射$\bar{f}$ $A/b$ 变为 $A'/b'$。如果 $f$ 是满射，$\bar{f}$ 是 $A/b$ 的同构到 $A'/b'$。

(d) *假设 $f$ 是满射。令 $\Phi$ 为 $A$ 包含 $a$ 的子环（分别为左理想、右理想、双边理想）中的集合。令 $\Phi'$ 为 $A'$ 的子环（分别为左理想、右理想、两侧理想）的集合。 映射 $B \to f(B)$ 和 $B' \mapsto \bar{f}(B')^{-1}$ 是 $\Phi$ 到 $\Phi'$ 的逆双射和 $\Phi'$ 到 $\Phi$。

(a) 和 (b) 是显而易见的，除了 (a) 的最后一个断言是从 no. 7、定理 3 得出的。

(c) 中考虑的复合态射 $g : A \to A' \to A'/b'$ 具有核 $b$，因此 $\bar{f}$ 是 $A/b$ 到 $A'/b'$ 的单射态射 (§ 8, no. 7, 定理 3)。如果 $f$ 是满射，则 $g$ 是满射，因此 $\bar{f}$ 是满射。

假设 $f$ 是满射。综上所述，映射$\theta : B' \mapsto \bar{f}(B')^{-1}$等于$\Phi'$的映射变成$\Phi$。显然，映射 $\eta : B \mapsto f(B)$ 是 $\Phi$ 的映射到 $\Phi'$。然后$\theta \circ \eta = \mathrm{Id}_{\Phi}, \eta \circ \theta = \mathrm{Id}_{\Phi'},$从而（d）。

#### 注 {#alg-i-s8-n8-rem-1 .statement tag=05HL}

上面的记号、$\theta$和$\eta$按集合同构排序（$\Phi$和$\Phi'$按包含排序）。

#### 推论{#alg-i-s8-n8-cor-1 .statement tag=05HM}

*令$A$为环，且$a$为$A$的双面理想。
(a) $A/a$ 的每个左（或右、两侧）理想都可以唯一地写成形式 $b/a$，其中 $b$ 是 $A$ 包含 $a$ 的左（或右、两侧）理想。
(b) 如果$b$是双面的，当经过与$A/b$的商同构到$(A/a)/(b/a)$时，合成同态$A \to A/a \to (A/a)/(b/a)$定义。*

它足以将应用命题 5 转换为$A$ 到$A/a$ 的规范态射。

### 9. 乘法理想

设$A$为环以及$a$和$b$$A$的两侧理想。 形式$x_1 y_1 + \cdots + x_n y_n$的元素的集合与$n \geq 0, x_i \in a$和$y_i \in b$对于$1 \leq i \leq n$，显然是$A$的双面理想，用$ab$表示，称为双面理想的*乘积* $a$ 和 $b$。在这个乘法下，$A$的双面理想的集合是一个幺半群，而单位元是双面理想$A$。如果$a, b, c$是$A$的两侧理想，则$a(b+c) = ab + ac, (b+c)a = ba + ca$。如果 $A$ 是可交换的，则乘法的理想也是可交换的。

$ab \subset aA \subset a$ 和 $ab \subset Ab \subset b$，因此

$$
ab \subset a \cap b.
$$

(21)

#### 命题 6 {#alg-i-s8-prop-6 .statement tag=05HN}

*设$a, b_1, \ldots, b_n$为$A$的两侧理想。如果 $A = a + b_i$ 对于所有 $i$，则 $A = a + b_1 b_2 \ldots b_n = a + (b_1 \cap b_2 \cap \cdots \cap b_n)$。*

由(21)足以证明$A = a + b_1 b_2 \ldots b_n$。到归纳，就足以考虑$n = 2$的情况。到假设，存在$a, a' \in a, b_1 \in b_1, b_2 \in b_2$使得$1 = a + b_1 = a' + b_2$。然后
$$
1 = a' + (a + b_1) b_2 = (a' + a b_2) + b_1 b_2 \in a + b_1 b_2,
$$
从而$A = a + b_1 b_2$。

#### 命题 7 {#alg-i-s8-prop-7 .statement tag=05HO}

*令$b_1, \ldots, b_n$为$A$的两侧理想，使得$b_i + b_j = A$对应于$i \neq j$。然后$b_1 \cap b_2 \cap \cdots \cap b_n = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$。特别是，如果 $A$ 是可交换的，则 $b_1 \cap b_2 \cap \cdots \cap b_n = b_1 b_2 \ldots b_n$ (cf. 习题 2).*

假设首先$n = 2$。存在$a_1 \in b_1, a_2 \in b_2$使得$a_1 + a_2 = 1$。如果$x \in b_1 \cap b_2$，则$x = x(a_1 + a_2) = x a_1 + x a_2 \in b_2 b_1 + b_1 b_2$。因此$b_1 \cap b_2 = b_1 b_2 + b_2 b_1$。

假设现在对于所有整数 $< n$ 都成立了命题的方程。 命题 6，$b_n + (b_1 b_2 \ldots b_{n-1}) = A$，因此
$$
b_1 \cap b_2 \cap \cdots \cap b_n = (b_1 \cap b_2 \cap \cdots \cap b_{n-1}) b_n + b_n (b_1 \cap b_2 \cap \cdots \cap b_{n-1})
$$
$$
= \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right) b_n
$$
$$
+ b_n \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right)
$$
$$
\subset \sum_{\tau \in S_n} b_{\tau(1)} b_{\tau(2)} \cdots b_{\tau(n)} \subset b_1 \cap b_2 \cap \cdots \cap b_n.
$$

### 10.乘积环

设$(A_i)_{i \in I}$是环的一个家庭。设$A$为乘积集合$\prod_{i \in I} A_i$。在 $A$ 加法和乘法上由公式定义
$$
(x_i) + (y_i) = (x_i + y_i), \quad (x_i)(y_i) = (x_i y_i).
$$
立即验证$A$是环称为环$A_i$的*乘积*，与零元素$0 = (0_i)_{i \in I}$，其中$0_i$是$A_i$的零，并且单位 $1 = (1_i)_{i \in I}$，其中 $1_i$ 是 $A_i$ 的单位。如果$A_i$是可交换的，那么$A$也是可交换的。如果$C_i$是$A_i$的中心，则$A$的中心就是$\prod_{i \in I} C_i$。

对于所有$i \in I$，$A$到$A_i$的投影$\mathrm{pr}_i$是环同态。如果$B$是环并且$f_i : B \to A_i$是同态的族，则存在唯一同态$f : B \to A$，使得$f_i = \mathrm{pr}_i \circ f$对于所有$i \in I$；它由$f(b) = (f_i(b))_{i \in I}$给出。

对于所有$i \in I$，令$a_i$为$A_i$的左理想。那么$a = \prod_{i \in I} a_i$是$A$的左理想。对于正理想、双面理想和子环也有类似的结果。

假设$a_i$是所有$i \in I$的双面理想，并让$f_i$表示$A_i$到$A_i / a_i$的典范映射。那么$\prod_{i \in I} A_i$的映射$f : (x_i)_{i \in I} \mapsto (f_i(x_i))_{i \in I}$到$\prod_{i \in I} (A_i / a_i)$的环同态等于核$\prod_{i \in I} a_i$，因此定义当经过与同构的商$\left( \prod_{i \in I} A_i \right) / \left( \prod_{i \in I} a_i \right)$ 到$\prod_{i \in I} (A_i / a_i)$。

令$(I_\lambda)_{\lambda \in L}$为$I$中的划分。 $\prod_{i \in I} A_i$到$\prod_{\lambda \in L} \left( \prod_{i \in I_\lambda} A_i \right)$的规范双射是环同构，根据它可以识别这两个环。

让$J \subset I$。让$e_J$表示$A$的元素$(x_i)_{i \in I}$，对于$i \in J$由$x_i = 1_i$定义，对于$i \in I - J$由$x_i = 0_i$定义。那么$e_J$是$A$的中心幂等（$§ 1$，no. 4）。紧接着是以下公式：

$$
\begin{align*}
e_I &= 1; \\
e_\varnothing &= 0; \\
e_{J \cap K} &= e_J e_K & \text{for } J \subset I, K \subset I; \\
e_{J \cup K} &= e_J + e_K & \text{for } J \subset I, K \subset I, J \cap K = \varnothing; \\
\sum_\lambda e_{J_\lambda} &= 1 & \text{if } (J_\lambda) \text{ is a finite partition of } I.
\end{align*}
$$

让$A_J = \prod_{i \in J} A_i$。令$\eta_J$为$A$到$A_J$的规范投影。对于$x = (x_i)_{i \in J} \in A_J$，令$\varepsilon_J(x)$为$A$的元素$(y_i)_{i \in I}$，对于$i \in J$由$y_i = x_i$定义，对于$i \in I - J$由$y_i = 0_i$定义。那么$\eta_J$在$A_J$上就是$A$环同态，$\varepsilon_J$在$A$上和图表上就是$A_J$加法群单同态

$$
A_J \xrightarrow{\varepsilon_J} A \xrightarrow{\eta_{I-J}} A_{I-J}
$$

$\eta_{I-J}$的核$a_J$等于$\varepsilon_J$的像。那么$\varepsilon_J(xx') = \varepsilon_J(x)\varepsilon_J(x')$对于所有$x, x' \in A_J$；但$\varepsilon_J$不是一般的环同态对于$\varepsilon_J(1) = e_J$。显然$a_J = e_J A = A e_J$。

让$e_{(i)} = e_i$和$a_i = a_{(i)} = e_i A = A e_i$代表所有$i \in I$。然后$e_i^2 = e_i$，

$$
e_i e_j = e_j e_i = 0
$$

$i \neq j$。如果$I$是有限的，则$\sum_{i \in I} e_i = 1$、加法群、$A$是双面理想$a_i$的直和，如果$x \in A$其在$a_i$中的分量是$x e_i$。立即推导出以下命题。

#### 命题 8 {#alg-i-s8-prop-8 .statement tag=05HP}

*假设 $I$ 是有限的。如果 $b$ 是 $A$ 的左理想或右理想，则 $b$ 是 $b \cap a_i$ 的直和。*

### 11.直接分解环

设$A$为环和$(b_i)_{i \in I}$，$A$的双面理想族。我们将拨打同态

$$
x \mapsto (\phi_i(x))_{i \in I},
$$

其中$\phi_i$是$A$的典范同态到$A/b_i$，典范同态到$A$到$\prod_{i \in I} (A/b_i)$。

#### 命题 9 {#alg-i-s8-prop-9 .statement tag=05HQ}

*令$A$为环和$(b_1, \ldots, b_n)$$A$的两侧理想，使得$b_i + b_j = A$为$i \neq j$。 $A$到$\prod_{i=1}^n (A/b_i)$的典范同态是核$\bigcap_{i=1}^n b_i = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}.$的满射*

显然核是$\bigcap_{i=1}^n b_i$。为了证明满射性，有必要证明，对于$A$的元素的每个族$(x_i)_{1 \leq i \leq n}$，都存在$x \in A$，使得对于所有$1 \leq i \leq n$都有$x \equiv x_i (b_i)$。我们通过归纳在$I$的基数$n$上证明断言，情况$n \leq 1$是微不足道的。到归纳假设，存在$y \in A$，使得$y \equiv x_i (b_i)$对应于$1 \leq i \leq n-1$。我们寻找形式 $y + z$ 和 $z \in A$ 的 $x$。 $i < n$必然需要$z \equiv 0 (b_i)$，即$z \in b = \bigcap_{i=1}^{n-1} b_i$，另一方面$z \equiv x_n - y (b_n)$。现在$b_n + b = A$由no. 9、命题6、从而存在$z$。最后，核的第二个表达式是从no. 9、命题7得出的。

#### 定义 7 {#alg-i-s8-def-7 .statement tag=05HR}

*令$A$为环。 $A$双面理想的有限族$(b_i)_{i \in I}$，使得$A$的典范同态进入$\prod_{i \in I} (A/b_i)$是同构，称为$A$的直接分解。*

#### 命题 10 {#alg-i-s8-prop-10 .statement tag=05HS}

*令$A$为环，$A'$其中心和$(b_i)_{i \in I}$为$A$的两侧理想的有限族。以下条件是等效的：

(a) 家庭$(b_i)_{i \in I}$是$A$的直接分解；
(b) 存在$A'$的幂等族$(e_i)_{i \in I}$，使得$e_i e_j = 0$对应$i \neq j$，$1 = \sum_{i \in I} e_i$，$b_i = A(1 - e_i)$对应$i \in I$；
(c) $b_i + b_j = A$ 代表 $i \neq j$ 和 $\bigcap_{i \in I} b_i = \{0\}$；
(d) $b_i + b_j = A$ 对应$i \neq j$，$\prod_{i \in I} b_i = \{0\}$对应$I$的总阶；
(e) 存在 $A'$ 的直接分解 $(b'_i)_{i \in I}$，使得 $b_i = A b'_i$ 对应 $i \in I$。*

(a) $\Rightarrow$ (b)。如果条件(a)成立，则$A$可以与环$\prod_{i \in I} (A/b_i)$等同，并且$b_i$可以与核等同于$\mathrm{pr}_i$。 $e_i$ 的存在性具有 (b) 中的属性，然后从 no. 10 得出。

(b) $\Rightarrow$ (d)。假设 $e_i$ 存在且具有 (b) 中的性质。对于 $i \neq j$、$1 - e_i \in b_i, \ e_i = e_i(1 - e_j) \in b_j$，因此为 $1 \in b_i + b_j$ 和 $A = b_i + b_j$。另一方面，如果给 I 一个全序并且 $(x_i)_{i \in I}$ 是 A 的元素族，那么，由于 $e_i$ 是中心，

$$
\prod_{i \in I} x_i (1 - e_i) = \left( \prod_{i \in I} x_i \right) \left( \prod_{i \in I} (1 - e_i) \right) = \left( \prod_{i \in I} x_i \right) \left( 1 - \prod_{i \in I} e_i \right) = 0
$$

因此$\prod_{i \in I} b_i = \{0\}$。

(d) $\Rightarrow$ (c)。这是从 no. 9、命题 7 得出的。

(c) $\Rightarrow$ (a)。这是从命题 9 得出的。

因此条件 (a), (b), (c) 和 (d) 是等价的。假设他们持有。到(b)$\Rightarrow$(a)，$b'_i = A'(1 - e_i)$的族是$A'$的直系分解。然后 $b_i = A(1 - e_i) = Ab'_i$ 对于所有 $i \in I$。因此条件(e)成立。

最后，假设条件 (e) 成立。通过(a)$\Rightarrow$(b)，存在$A'$幂等族$(e_i)_{i \in I}$，使得$e_i e_j = 0$对应$i \neq j$，$1 = \sum_{i \in I} e_i$和$b'_i = A'(1 - e_i)$对应$i \in I$。那么 $b_i = Ab'_i = A(1 - e_i)$ 对应 $i \in I$，因此条件 (b) 成立。

#### 注 {#alg-i-s8-n11-rem-1 .statement tag=05HT}

设 A 为环。令$(a_i)_{i \in I}$是A的加法群$A^+$的子群的有限族，使得$A^+$是$a_i$的直和。假设$a_i a_i \subset ai$代表$i \in I$，$a_i a_j = \{0\}$代表$i \neq j$。那么$a_i$对于所有$i \in I$来说都是A的双面理想。通过A上的那些诱导出加法和乘法，$a_i$是环，而单位元是$1 \in A$在$a_i$中的分量。如果 $b_i = \sum_{j \neq i} a_j$，显然命题 10 的 $b_i$ 满足条件 (c)，因此 $(b_i)_{i \in I}$ 是 A 的直接分解，据说它是由* $(a_i)_{i \in I}$ *定义的。

#### 例 {#alg-i-s8-n11-exa-1 .statement tag=05HU}

*理想和* $\mathbf{Z}$的商环

$\mathbf{Z}$的理想是$\mathbf{Z}$的子群的加法，因此形式$n.\mathbf{Z}$与$n \geqslant 0$的加法；相反，对于每个整数$n \geqslant 0$，集合$n.\mathbf{Z}$都是一个理想，即主理想$(n)$。因此，$\mathbf{Z}$的每个理想都是主要的，并且在形式$n\mathbf{Z}$和$n \geqslant 0$中唯一地表示。理想的$(1)$等于$\mathbf{Z}$，理想的$(0)$由0组成，与$\mathbf{Z}$和$\{0\}$不同的理想因此为形式$n\mathbf{Z}$和$n > 1$。如果$m \geqslant 1$和$n \geqslant 1$，$m\mathbf{Z} \supset n\mathbf{Z}$当且仅当$n \in m.\mathbf{Z}$，即$m$除$n$。因此，要使理想的$n\mathbf{Z}$极大，不存在不同于$n$并除以$n$的整数$m > 1$是充分必要的；在其他字中，*$\mathbf{Z}$的最大理想是形式*$p\mathbf{Z}$*其中*$p$*是素数数*（§ 4, no. 10，定义16）。

令$m$和$n$为两个整数$\geqslant 1$。理想$m\mathbf{Z} + n\mathbf{Z}$为主，从而有整数$d \geqslant 1$，以$d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$为特征；对于每个整数 r \geqslant 1，关系“r 除 d”相当于$r\mathbf{Z} \supset d\mathbf{Z}$，因此相当于“$r\mathbf{Z} \supset m\mathbf{Z}$和$r\mathbf{Z} \supset n\mathbf{Z}$”，即“r 除 m和n”。由此可见，m和n的公共的除子是d的除子，d对于m和n来说是除子$\geqslant 1$公共的的*最大的*； d 称为 m 和 n 的 *最大的公共的除子*（缩写为 g.c.d.）。作为$d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$，存在两个整数 x 和y，使得$d = mx + ny$。如果 m 和 n 的 g.c.d. 则被称为“互质”。等于 1。假设存在整数 x 和 y，且$mx + ny = 1$ 也同样存在。

理想$m\mathbf{Z}$和$n\mathbf{Z}$的交对于包含$mn$来说是非零的，因此是形式$r\mathbf{Z}$和$r \geqslant 1$。 Arguing as above, it is seen that the multiples of r are the common multiples of m and n and that r is *the least* of the integers $\geqslant 1$ which are common multiples of m and n; it is called *the least common multiple* (l.c.m.) of m and n.

对于$x_1, \ldots, y_r \in \mathbf{Z}$，理想$m\mathbf{Z}$和$n\mathbf{Z}$的乘积是$\sum_{i=1}^{r} mx_i ny_i = mn \left( \sum_{i=1}^{r} x_i y_i \right)$的集合，因此等于$mn\mathbf{Z}$。

对于每个整数$n \geqslant 1$，商环$\mathbf{Z}/n\mathbf{Z}$被称为整数模n*的*环；它有 n 个元素，即类对整数 0, 1, 2, ..., $n - 1$ 的模 n。对于$n = 1$，我们得到零环。

#### 命题 11 {#alg-i-s8-prop-11 .statement tag=05HV}

*设$n_1, \ldots, n_d$为整数$\geqslant 1$，它们在对和$n = n_1 \ldots n_r$互质。 $\mathbf{Z}$的典范同态进入乘积环$\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$是核$n\mathbf{Z}$和$\mathbf{Z}/n\mathbf{Z}$的定义环同构到$\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$的满射。*

让$a_i = n_i\mathbf{Z}$代表$i = 1, \ldots, r$。 假设，$a_i + a_j = \mathbf{Z}$ $i \neq j$。然后从命题 9 得出命题。

上述结果以及有关分解到素数因子的结果，将推广到致力于研究主理想整环的章 VII, § 1 和致力于研究阶乘域的 *交换代数*、章 VII, § 3 中。

### 12. 环的分数

#### 定理 4 {#alg-i-s8-thm-4 .statement tag=05HW}

*设 A 为 A 的交换环，S 子集。设 $A_S$ 为 A 的分数的幺半群（仅提供乘法），分母为 S (§ 2, no. 4)。令 $\varepsilon : A \to A_S$ 为规范的态射。在$A_S$上存在且仅有一个加法满足以下条件：
(a) $A_S$，加上加法及其乘法，就是交换环；
(b) $\varepsilon$ 为环同态。*

假设已经为 $A_S$ 满足条件 (a) 和 (b) 找到了加法。

让$x, y \in A_S$。令$S'$为$S$生成的$A$的稳定乘法子幺半群。存在$a, b \in A$和$p, q \in S'$使得$x = a/p, y = b/q$。然后

$$
x = \varepsilon(aq)\varepsilon(pq)^{-1}, \quad y = \varepsilon(bp)\varepsilon(pq)^{-1},
$$

whence

(23)
$$
\begin{align*}
x + y &= (\varepsilon(aq) + \varepsilon(bp))\varepsilon(pq)^{-1} \\
&= \varepsilon(aq + bp)\varepsilon(pq)^{-1} \\
&= (aq + bp)/pq.
\end{align*}
$$

这就证明了加法的唯一性。

我们现在 *定义* 加法在 $A_S$ 设定 $x + y = (aq + bp)/pq$。有必要证明这个定义不依赖于$a, b, p, q$的选择。现在，如果$a', b' \in A, p', q' \in S'$使得$x = a'/p', y = b'/q'$，则在$S'$中存在$s$和$t$使得$ap's = a'ps, bq't = b'qt$，从而

$$
(aq + bp)(p'q')(st) = (a'q' + b'p')(pq)(st)
$$

因此

$$
(aq + bp)/pq = (a'q' + b'p')/p'q'.
$$

It is easily verified that addition in $A_S$ is associative and commutative, that $0/1$ is identity element for addition, that $(-a)/p$ is the negative of $a/p$ and that $x(y + z) = xy + xz$ for all $x, y, z \in A_S$. 若$a, b \in A$，则

$$
\varepsilon(a + b) = (a + b)/1 = a/1 + b/1 = \varepsilon(a) + \varepsilon(b)
$$

因此$\varepsilon$是环同态。

#### 定义 8 {#alg-i-s8-def-8 .statement tag=05HX}

*在定理 4 中定义的环称为分数的环，与$S$相关，或与$S$中的分母相关，并用$A[S^{-1}]$表示。*

$A[S^{-1}]$的零是$0/1$，$A[S^{-1}]$的单位是$1/1$。

我们将回到*交换代数*、章II, § 2中$A[S^{-1}]$的属性。

若$S$为$A$可取消元素集合，环$A[S^{-1}]$称为$A$的分数总环。然后通过映射 $\varepsilon$ 将$A$ 与 $A[S^{-1}]$ 的子环进行识别，然后它是单射的 (I, § 2, no. 4, 命题 6)。

#### 定理 5 {#alg-i-s8-thm-5 .statement tag=05HY}

*设$A$为$A$的交换环、$S$子集、$B$环和$A$的$f$同态到$B$，使得每个$f(S)$ 的元素可逆。 $A[S^{-1}]$ 中存在且仅有一个 $\bar{f}$ 进入$B$，使得 $f = \bar{f} \circ \varepsilon$。*

我们知道（§ 2, no. 4，定理 1），乘法幺半群$A[S^{-1}]$到乘法幺半群$B$之间存在且仅有一个态射$\bar{f}$使得$f = \bar{f} \circ \varepsilon$。设$a, b \in A, p, q \in S'$（由$S$生成的$A$的稳定乘法子幺半群）。由于$f(A)$的元素在对通勤，
$$
\bar{f}(a/p + b/q) = \bar{f}((aq + bp)/pq) = f(aq + bp)f(pq)^{-1}
= (f(a)f(q) + f(b)f(p))f(p)^{-1}f(q)^{-1}
= f(a)f(p)^{-1} + f(b)f(q)^{-1}
= \bar{f}(a/p) + \bar{f}(b/q).
$$
因此$\bar{f}$是环同态。

### 习题{#alg-i-s8-exercises}

§ 8](exercises/s8/)参见[习题。
