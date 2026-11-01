---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 4
section_title: Exponentials and logarithms
lang: zh
source: top-v-x
pdf_pages: 0025-0029, 0034-0034
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 25
    - "no": 2
      title: BEHAVIOUR OF THE FUNCTIONS $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 27
    - "no": 3
      title: MULTIPLIABLE FAMILIES OF NUMBERS $> 0$
      page: 0
      pdf_page: 28
statements: 1
exercises: 2
content_sha256: 4b2c71871bc5a5915d7ce8bf98cd02a0814a96c4f3fb9ff128548e730e542664
translated_from: content/en/top/V/04_s4_exponentials_and_logarithms.md
translation_method: google
source_content_sha256: 55a9b7eecb6aa809fbac52ae103f840e9203fcdc0fe64340d7af904b5c851e60
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 6ca82175c22f23a0f3dc2bcc0ca21bd93de5060ae2d3d0430cff97bcecc01140
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4. 指数和对数

### 1. $a^x$ 和 $\log_a x$ 的定义

#### 定理 1 {#top-v-s4-thm-1 .statement tag=0BW0}

*乘法群* $\mathbf{R}_+^*$ *of 实数* $> 0$ *是群同构于加法群* $\mathbf{R}$ *of 实数*。

因为$\mathbf{R}_+^* = ]0, +\infty[$是$\mathbf{R}$的开区间，因此与$\mathbf{R}$*同胚*（章IV, § 4, no. 1，命题1）。因此，通过 § 3 的定理 2，它是群 *同构的*到 $\mathbf{R}$。

从推论到§ 1, no. 3的命题5，对于每个数$a > 0$，都有一个唯一的连续同态$f_a$，从$\mathbf{R}$到$\mathbf{R}_+^*$，使得$f_a(1) = a$。因此，对于所有 $x \in \mathbf{R}$ 和所有 $y \in \mathbf{R}$，我们有

$$
f_a(x + y) = f_a(x) f_a(y), \qquad f_a(-x) = \frac{1}{f_a(x)},
$$

因此，特别是对于所有 $n \in \mathbf{Z}$，

$$
f_a(n) = a^n.
$$

因此，对于所有 $x \in \mathbf{R}$，我们用 $a^x$ 表示 $f_a(x)$； 函数 $a^x$（对于 $a > 0$ 的所有值）称为*指数函数*。我们为所有 $x \in \mathbf{R}$ 提供了 $1^x = 1$；如果$a \neq 1$，$x \to a^x$是群$\mathbf{R}$到群$\mathbf{R}_+^*$的*同构的*。

如果$a \neq 1$，$\mathbf{R}_+^*$到$\mathbf{R}$（$x \to a^x$的倒数）的同构称为基* $a$的*对数，并且其在$x \in \mathbf{R}_+^*$的值表示为$\log_a x$。因此，有了这个记号，我们就有了

(1) $$
a^{x+y} = a^x a^y \qquad (x \in \mathbf{R}, y \in \mathbf{R}, a > 0);
$$
(2) $$
a^{-x} = \frac{1}{a^x} \qquad (x \in \mathbf{R}, a > 0);
$$
(3) $$
\log_a 1 = 0, \quad \log_a a = 1 \qquad (a > 0, a \neq 1);
$$
(4) $$
\log_a (xy) = \log_a x + \log_a y \qquad (x > 0, y > 0);
$$
(5) $$
\log_a \left( \frac{1}{x} \right) = -\log_a x \qquad (x > 0);
$$
(6) $$
a^{\log_a x} = x \qquad (x > 0);
$$
(7) $$
\log_a a^x = x \qquad (x \in \mathbf{R}).
$$

到§ 1, no. 3的命题 5，$\mathbf{R}$到$\mathbf{R}_+^*$的每一个连续的同态都是形式$y \to a^{xy}$，其中$x \in \mathbf{R}$；因为当$y = 1$是$a^x$时它是值，所以我们有相同的

(8) $$
(a^x)^y = a^{xy} \qquad (x \in \mathbf{R}, \ y \in \mathbf{R}, \ a > 0),
$$
或者，更改记号，

(9) $$
x^y = a^{y \cdot \log_a x} \qquad (x > 0, y \in \mathbf{R}, a > 0, a \neq 1).
$$

公式 (8) 表明，对于每个整数 $n > 0$，我们都有 $(a^{1/n})^n = a$，这证明了为第 n 个根* $\sqrt[n]{a}$ 引入记号 $a^{1/n}$（在章 IV, § 3, no. 3 中定义）是合理的。

公式 (7) 和 (9) 表明

(10) $$
\log_a (x^y) = y \log_a x \qquad (x > 0, y \in \mathbf{R}),
$$
或者，改变记号，

(11) $$
\log_a x = \log_a b \cdot \log_b x \qquad (x > 0, a > 0, b > 0, a \neq 1, b \neq 1),
$$
这是“基的变换”的公式。

最后，让我们获得拓扑群$\mathbf{R}^*$的所有*连续同态*；如果$g$是这样一个连续的同态，

$$
\log_a (g(a^x))
$$

是$\mathbf{R}$到$\mathbf{R}$的连续同态，因此（§ 1, no. 3，命题 5）存在$\alpha \in \mathbf{R}$，使得$\log_a (g(a^x)) = \alpha x$对于所有$x \in \mathbf{R}$；因此，通过 (8)，$g(x) = x^\alpha$ 对于所有$x > 0$。因此我们有相同的

(12) $$
(xy)^\alpha = x^\alpha y^\alpha \text{ for all } x > 0, y > 0 \text{ and } \alpha \in \mathbf{R}.
$$

由于公式 (4)，其中约化每乘法到加法（唯一与习惯的系统很好地适应的运算），对数长期以来一直是数值计算中不可或缺的工具（参见历史注记到章）。

用于此目的时，基选择为$a = 10$；并且有表给予值函数 $\log_{10} x$（达到一定的近似值）。在数学分析中，一个人被引导到选择一个不同的基（用$e$表示），即$\lim_{x \to 1, x \neq 1} \frac{\log_e x}{(x - 1)} = 1$（cf.习题1）。

### 2. 函数 $a^x$ 和 $\log_a x$ 的行为

通过章IV, § 2, no. 6的定理5，如果$a \neq 1, x \to a^x$是$\mathbf{R}$的严格单调映射到区间$\mathbf{R}_+^* = ]0, + \infty[$。如果$a > 1$，我们有$a^1 = a \geq 1 = a^0$，因此$a^x$是严格递增的；此外，由于$\mathbf{R}_+^*$没有上界，$a^x$在$\mathbf{R}$中也没有上界，因此

$$
\lim_{x \to +\infty} a^x = +\infty \quad (a > 1)
$$

并且，通过(2)，

$$
\lim_{x \to -\infty} a^x = 0 \quad (a > 1).
$$

另一方面，如果$a < 1$、函数、$a^x$为严格递减，当$x$趋于$+\infty$时趋向于0，当$x$趋于$-\infty$时趋于$+\infty$（图1）。

![图表显示 y = a^x (a > 1) 和 y = a^x (a < 1)](https://i.imgur.com/1.png)

图 1.

![图表显示 y = log_a x (a > 1) 和 y = log_a x (a < 1)](https://i.imgur.com/2.png)

图 2.

从这些属性和 (12) 中，我们推断出，如果 $0 < a < b$，则对于 $x > 0$，我们有 $a^x < b^x$，对于 $x < 0$，我们有 $a^x > b^x$；如果$x > 0$则为$\left(\frac{b}{a}\right)^x > 1$，如果$x < 0$则为$\left(\frac{b}{a}\right)^x < 1$。

$\mathbf{R}_+^*$中$\log_a x$的行为是从$\mathbf{R}$中$a^x$的行为推导出来的；如果$a > 1$、函数$\log_a x$为严格递增的，当$x$趋向于$0$时趋向于$-\infty$，并且当$x$趋向于$+\infty$时趋向于$+\infty$；如果$a < 1$、函数$\log_a x$为严格递减，当$x$趋向$0$时趋向于$+\infty$，当$x$趋于$+\infty$时趋于$-\infty$（图2）。

函数 $a^x$（分别为$\log_a x$），视为在延长线$\overline{\mathbf{R}}$的子集上定义，并在$\overline{\mathbf{R}}$中取其值，可以*通过连续性*扩展到$\overline{\mathbf{R}}$（分别为$[0, +\infty]$的区间） $\overline{\mathbf{R}}$）通过将其限制值分配给点$+\infty$和$-\infty$（分别为$0$和$+\infty$）。

More generally, formula (9) shows that the function $x^y$ is continuous on the subspace $\mathbf{R}_+^* \times \mathbf{R}$ of $\overline{\mathbf{R}}^2$ and tends to a limit when $(x, y)$ tends to any point $(a, b)$ of $\overline{\mathbf{R}}^2$ which lies in the closure of $\mathbf{R}_+^* \times \mathbf{R}$, with the exception of the points $(0, 0)$, $(+\infty, 0)$, $(1, +\infty)$, $(1, -\infty)$. 因此，我们可以通过连续到$\overline{\mathbf{R}}^2$的点（其中极限存在）来得到扩展$x^y$；通过扩张的原理恒等式（章 I, § 8, no. 1、命题 2，推论 1），公式 (1)、(4) 和 (8) 只要双方都有意义，就仍然有效。

注扩张通过$x^y$的连续性不允许我们获得公式$0^0 = 1$。

注另外，指数的定义允许我们对所有 $a > 0$ 定义在 $\mathbf{Z}$ 上的扩展到 $\mathbf{R}$ 函数 $n \to a^n$；但是当 $a < 0$ 时，我们并没有通过这种方式获得这个函数的任何扩张；这个函数的“自然”扩张只能在解析函数理论的项中定义。

### 3. 数 $> 0$ 的可乘族

拓扑群$\mathbf{R}$和$\mathbf{R}_+^*$的同构立即表明，对于有限实数$> 0$的族$(x_i)$来说，要*可乘*（章IV, § 7, no. 4），族$(\log_a x_i)$应该是*可求和*（$a$是任何数$> 0$和$\neq 1$）；我们有

$$
\prod_i x_i = a^{\sum \log_a x_i}.
$$

同样，由有限数 $> 0$ 的序列 $(1 + u_n)$ 定义的无限乘积 *收敛* (章 IV, § 7, no. 6) 当且仅当级数收敛，其一般项为 $\log_a (1 + u_n)$ 收敛，然后我们有

$$
\prod_{n=0}^{\infty} (1 + u_n) = a^{S_{n=0}^{\infty} \log_a (1 + u_n)}.
$$

因此，对实数$> 0$的无穷乘积的研究就简化为对实数的无穷级数的研究，其项出现在对数的形式中；稍后我们将看到如何通过对数的微分性质来轻松研究这种性质的和。

### 习题 {#top-v-s4-exercises}

请参阅 § 4](exercises/s4/) 的 [习题。
