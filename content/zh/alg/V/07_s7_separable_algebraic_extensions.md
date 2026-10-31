---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 7
section_title: Separable algebraic extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.36-A V.47, A V.151-A V.153
pdf_pages: 0150-0161, 0265-0267
extraction: ocr
subsections:
    - "no": 1
      title: Separable algebraic extensions
      page: 36
      pdf_page: 150
    - "no": 2
      title: Separable polynomials
      page: 37
      pdf_page: 151
    - "no": 3
      title: Separable algebraic elements
      page: 39
      pdf_page: 153
    - "no": 4
      title: The theorem of the primitive element
      page: 40
      pdf_page: 154
    - "no": 5
      title: Stability properties of separable algebraic extensions
      page: 41
      pdf_page: 155
    - "no": 6
      title: A separability criterion
      page: 42
      pdf_page: 156
    - "no": 7
      title: The relative separable algebraic closure
      page: 43
      pdf_page: 157
    - "no": 8
      title: The separable closure of a field
      page: 45
      pdf_page: 159
    - "no": 9
      title: Separable and inseparable degrees of an extension of finite degree
      page: 46
      pdf_page: 160
statements: 39
exercises: 5
content_sha256: 725c15629c6c31d8f541842e58e27f1b00f4659abc8dc15252f7a99d3bf535b4
translated_from: content/en/alg/V/07_s7_separable_algebraic_extensions.md
translation_method: google
source_content_sha256: 6efc8ea4adffb96079107da26548dc480864f6a35c138ba6f08fe110dc1e0941
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 18ddc9d7d7ccb17ab461ee7b4493b1732cd93693654885da1edffa103b93a0e4
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 7。可分离代数扩张

在本段中，$K$ 表示域。

### 1.可分代数扩张

#### 定义 1 {#alg-v-s7-def-1 .statement tag=06K0}

— *令 E 为 K 的代数扩张；则称 E 是可分的（在 K 上），如果 K 上有限次数的 E 的每个子外延 F 都是 K* 上的 etale 代数 ($V$, p. 28, Def. 1)。

设 E 为 K 的有限次数的扩张。由于 etale 代数的每个子代数都是 etale（$V$，p. 30，命题 3），因此假设 E 是 $K$ 的可分扩张，或者 E 是 etale 代数 $K$。

#### 命题 1 {#alg-v-s7-prop-1 .statement tag=06K1}

— *令 E 为 K 的代数扩张。如果 E 是可分的，则 E 的每个子外延 $E'$ 都是可分的。相反，如果 E 的有限次数的每个子扩展都是可分的，则 E 是可分的。*

这立即从定义 1 开始。

#### 命题 2 {#alg-v-s7-prop-2 .statement tag=06K2}

— *为了使域 K 完美，K 的每个代数扩张应该是可分的是必要且充分的。*

首先假设 K 是完美的。由于域是减少的环，因此从引理 5（$V$，p. 35）得出，$K$的有限次数的每个扩张都是$K$上的一个etale代数；因此 $K$ 的每个代数扩张都是可分的。

现在假设$K$是特征$p \neq 0$的不完美域。令$\Omega$为$K$的代数闭包。由于$K$不完美，因此存在$b \in K$而不是属于到$K^p$；把$a = b^{1/p}$。那么$K$的扩张$K(a)$就是有限次数的p根式。根据$V$，p. 26，命题3，存在$K(a)$到$\Omega$的单个K同态，并且由于$[K(a):K] > 1$，代数$K(a)$在$K$上不完整（$V$， p. 32，提案 4）。其他字、$K$有限次数扩张$K(a)$是不可分离的。

#### 推论{#alg-v-s7-n1-cor-1 .statement tag=06K3}

— *特征 0 的域或有限域的每个代数扩张都是可分的。*
    这是从 *V*、p. 7、提案 5 得出的。

### 2.可分离多项式

#### 命题 3 {#alg-v-s7-prop-3 .statement tag=06K4}

— *令 f 为 K[X] 中的非零多项式，并令 Ω 为 K 的代数闭扩张。以下条件是等效的：*
    *a) 多项式 f 与其在 K[X] 中的导数 f' 互质。*
    *b) deg(f) = 0，或 deg(f) > 0 且 dis(f) ≠ 0 (IV, p. 83)。*
    *c) 存在 K 的扩张 L，使得 L[X] 中的 f 分裂的进入次数 ≤ 1 的不同多项式的乘积。*
    *d) 根关 Ω 很简单。*
    *e) K-代数 K[X]/(f) 是 etale (V, p. 28, Def. 1).*

*a) ⇒ d)*: 在假设 *a*) 下，K[X] 中存在两个多项式 g 和 h，使得 fg + f'h = 1 (IV, p. 12)。设a为fin Ω的根；我们有
$$
f'(a)\ h(a) = f(a)\ g(a) + f'(a)\ h(a) = 1,
$$
从而$f'(a) \neq 0$；因此 $a$ 是 fin Ω 的简单根 (*IV*, p. 17, 命题 7)。

*d) ⇒ c)*：如果 *d*) 成立，则 Ω[X] 中的 f 分裂的变为次数 ≤ 1 的不同因子的乘积。

*c) ⇒ b)*：在假设 c) 下，L 中存在元素 $A \neq 0$ 以及 L 的*不同* 元素 $a_1, ..., a_n$，使得 $f(X) = \lambda (X - a_1) ... (X - a_n)$。如果 $\deg(f) > 0$，我们有 (*IV*, p. 83, 命题 11)，
$$
\operatorname{dis}(f) = \lambda^{2n-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 \neq 0.
$$

*b) ⇒ a)*：设 c 为主导系数，D 为 f 的判别式； $f'$ 和 f 的结果等于 ± cD (IV, p. 84, 公式 (54))，因此不为零；因此 (*IV*, p. 78, Cor. 2) 多项式 f 和 $f'$ 在 K[X] 中互质。

*a) ⇒ e)*：设 A 为 K-代数 K[X]/(f) 且 A 中 X 的 x 像；由III、p. 573、第22号提案、A-模$\Omega_K(A)$由元素$dx$生成，受单个关系$f'(x)\ dx = 0$的约束。由*V*，p. 33，Th。 3、K-代数 A 是 etale 当且仅当$f'(x)$ 是 A 中的可逆元，这意味着 f 和 $f'$ 在 K[X] 中互质。

#### 定义 2 {#alg-v-s7-def-2 .statement tag=06K5}

— *如果多项式 $f \in K[X]$ 非零且满足命题 3 的等价条件 a)、b)、c)、d) 和 e)，则称其为可分的。*

#### 注 {#alg-v-s7-n2-rem-1 .statement tag=06K6}

— 1) 令 L 为 K 的扩张，f 为 K[X] 中的非常数多项式。根据第 3 号提案的 *e)* 和 V、p. 32，Cor。 2 假设 f 是可分离的，无论是被视为 K[X] 的元素还是L[X] 的元素，情况都是一样的。另一方面，很可能 f 在 K[X] 中不可约，但在 L[X] 中不可约。

2）设$f \in K[X]$；我们知道（IV，p. 13，命题13）$K[X]$中存在不可约多项式$f_1, \ldots, f_m$使得$f = f_1 \ldots f_m$。设$\Omega$为$K$的代数闭包；由于不可约多项式$g \in K[X]$是$\Omega$中每个根的$K$上的最小多项式，因此$K[X]$中的两个不同的不可约多项式在$\Omega$中没有公共的根。命题 3 的条件 d) 现在表明，当且仅当多项式 $f_1, \ldots, f_m$ 可分离且两两不同时，$f$ 才是可分离的。

#### 命题 4 {#alg-v-s7-prop-4 .statement tag=06K7}

— *令 $f$ 为 $K[X]$ 中的不可约多项式。那么下面的条件是等价的*：

a) $f$ 是可分离的。
b) *存在$K$的扩张$L$，其中$f$有一个简单的根。*
c) *导数$f'$关闭不是零。*
d) *域$K$具有特征$0$，或者具有特征$p \neq 0$和$f \not\in K[X^p]$*。

我们注首先$K[X]$中的不可约多项式不是常数。很明显，a) 蕴涵 b)（取 $K$ 中的代数闭包得到 $L$）。如果$x$是$K$的扩张$L$中的一个简单根，我们有$f'(x) \neq 0$（IV，p. 17，命题7），所以b)蕴涵c)，而c)和d)的等价由V，p. 9，科。

最后假设$f \neq 0$；令$x$为$K$的代数闭扩张$\Omega$中的$f$根。由于$f$是$x$在$K$和$\deg f' < \deg f$上的最小多项式，我们有$f'(x) \neq 0$，因此$x$是$f$的简单根（IV，p. 17，命题1） 7).因此 $f$ 是可分的，我们已经证明 c) 蕴涵 a)。

#### 推论 1 {#alg-v-s7-prop-4-cor-1 .statement tag=06K8}

— *为了使域 $K$ 完美，$K[X]$ 的每个不可约多项式应该是可分的是必要且充分的*。

如果域$K$具有特征$0$，则$K$是完美的，并且$K[X]$的每个不可约多项式都是可分的，通过上面的d）。假设$K$具有特征$p \neq 0$。

首先假设 $K$ 是完美的。我们有 $K[X^p] = K[X]^p$，因此不存在 $K[X]$ 属于到 $K[X^p]$ 的不可约多项式。根据命题 4，$K[X]$ 的每个不可约多项式都是可分的。

接下来假设$K$不完美，从而$K \neq K^p$。令$a$为$K$的元素，而不是属于到$K^p$；多项式 $X^p - a$ 在 $K[X]$ (V, p. 24, 引理 1) 中不可约，并且它属于到 $K[X^p]$，因此不可分。

#### 推论 2 {#alg-v-s7-prop-4-cor-2 .statement tag=06K9}

— *令 $f \in K[X]$ 为非零多项式。为了使$f$是可分离的，$K$应该存在扩张$L$，即完美域，并且$f$在$L[X]$*中没有重复的因子，这是充分必要的。

设$\Omega$为$K$的代数闭包； iff 是可分离的，$f$ 在 $\Omega[X]$ 中没有重复的因子（命题 3，d））。相反，如果$L$是$K$的完美扩张，使得$f$在$L[X]$中没有重复的因子，则$f$在$L[X]$中可分离（Cor.1和注2），因此$K[X]$（注1）。

### 3.可分离代数元素

#### 定义 3 {#alg-v-s7-def-3 .statement tag=06KA}

— 令 E 为 K 的扩张。如果 K 的代数扩张 K(x) 可分，则 E 的元素 x 在 K 上是可分的，则称其在 K 上可分。

#### 命题 5 {#alg-v-s7-prop-5 .statement tag=06KB}

— 令 E 为 K 的扩张，E 的 x 元素在 K 上的代数，f 为 x 在 K 上的最小多项式。则以下条件是等效的：
a) x 在 K 上可分；
b) 首一多项式 f 是可分离的；
c) x 是 f 的简单根。
a) 和 b) 的等价由命题 3 得出，b) 和 c) 的等价由命题 3 和 4 得出（cf. V、p. 37 和 38）。

#### 推论 1 {#alg-v-s7-prop-5-cor-1 .statement tag=06KC}

— 如果 E 的元素 x 是 K[X] 的多项式 g 的简单根，则它在 K 上可分。
对于 K[X] 中 K 除 g 上 x 的最小多项式 f (V, p. 16, Th. 1)，因此 x 是 f 的简单根。

#### 推论 2 {#alg-v-s7-prop-5-cor-2 .statement tag=06KD}

— 如果 E 的元素 x 在 K 上是代数且可分的，则它在 E 中包含的 K 的每个扩张 K' 上也是代数且可分的。
设f是x在K上的最小多项式。那么x是根据Prop.5的f的简单根，并且由于f属于到K'[X]，E的元素x可以在K'上通过Cor分离。 1.

#### 推论 3 {#alg-v-s7-prop-5-cor-3 .statement tag=06KE}

— 假设 K 具有特征 $p \neq 0$。对于 E 到属于到 K 的元素 x，它是 K 上的可分代数和 p 根式是必要且充分的。
所规定的条件显然是必要的。相反，假设 x 在 K 上是可分的代数，并且在 K 上是高度 e 的 p 根式。由于 x 在 K 上是可分的，因此 x 在 K 上的最小多项式 f 不会属于到 K[X^p]（命题 4 和 5）；因为 x 是 K 上高度为 e 的 p 根，所以我们有 $f(X) = X^{p^e} - x^{p^e}$ (V, p. 24, 命题 1)；我们结论$e = 0$，所以$x \in K$。

#### 命题 6 {#alg-v-s7-prop-6 .statement tag=06KF}

— 令 E 为 K 的扩张。
a) 如果 E 是代数且在 K 上可分，则 E 的每个元素是代数且在 K 上可分。
b) 相反，令 A 为 E 的元素的集合，在 K 上代数且可分离，且满足 $E = K(A)$；则 E 是代数且可在 K 上分离。
如果 E 是代数且可在 K 上分离，则对于每个 $x \in E$、从而 a)，K 的扩张 K(x) 也是如此。
在假设 b) 下，扩张 E 是 K 上的代数 (V, p. 18, Cor. 1)。

设F是有限次数的E在K上的子扩展。根据V，p. 11，Cor.，存在A的元素$x_1, \ldots, x_m$，使得$F \subset K(x_1, \ldots, x_r)$，我们有

$$
K(x_1, \ldots, x_m) = K[x_1, \ldots, x_m] \quad (\text{V, p. 18, Cor. 1}).
$$

到 A 上的假设时，代数 $K[x_1], \ldots, K[x_m]$ 已在 K 上完成；因此$K[x_1] \otimes \cdots \otimes K[x_m]$（V，p. 32，Cor.1）也是如此。现在 F 同构于代数与 $K[x_1] \otimes \cdots \otimes K[x_m]$ 的商子代数，etale 也同构（V，p. 30，命题 3）。

#### 推论{#alg-v-s7-n3-cor-1 .statement tag=06KG}

— *为了使代数扩张 E 在 K 上可分，E 的每个元素应该是其在 K 上的最小多项式的简单根是必要且充分的。应用命题 5 和 6 就足够了。*

### 4. 原始元素的定理

设$E$为$K$中的扩张；如果 $E = K[x]$，则 $E$ 的元素 $x$ 被称为“原始”。为了使扩张 $E$ 拥有原语元素，$[E : K]$ 必须是有限的。

#### 定理 1 {#alg-v-s7-thm-1 .statement tag=06KH}

— *令 E 为 K 的扩张。则以下条件是等价的：
a) E 拥有原语元素；
b) E 只存在有限数个子扩展。
当E为有限次数中的可分扩张时，满足这些条件。*
首先假设$E$拥有原语元素$x$，并让$f$为$x$在K上的最小多项式。对于每个一元多项式$g \in E[X]$除以$E[X]$中的$f$，用$E_g$表示子扩张$E$ 由 g 的系数生成。由于可能的多项式 g 在数中是有限的（如果 $E[X]$ 中的 $f$ 分裂的进入 r 莫式不可约多项式的乘积，数以 $2^r$ 为界），子扩展 $E_g$ 是有限的数。因此，为了证明 b)，只需证明 $E$ 的每个子扩展 L 都是 $E_g$ 之一。现在如果$L$是E的子扩展，那么我们有$L[x] = E$；如果 g 是 $x$ 在 L 上的最小多项式，我们有 $[E : L] = \deg(g)$。此外，g 在 $L[X]$ 中偏离除子，因此在 $E[X]$ 中；所以我们有$E_g \subset L$和$E = E_g[x]$。从$g(x) = 0$开始，我们有$[E : E_g] \leq \deg(g)$，因此有$[E : E_g] \leq [E : L]$，还有$L = E_g$，正如我们希望展示的那样。

接下来我们观察条件 b) 意味着扩张 E 是有限次数：通过注 2 of V，p. 18 足以证明它是代数；现在，如果 z 是 $E$ 超越 $K$ 的元素，则子外延 $K(z^n), n \in \mathbf{N}$ 是两两不同的。

为了证明 b) $\Rightarrow$ a) 我们现在区分两种情况：
A) 如果域 $K$ 是*有限*，域 $E$ 是 K 上有限维的向量空间，因此是有限的集合。因此$^1$(V,p. 78,引理1)存在$E$的$E$生成的乘法群的元素$x$，我们有$E = K[x]$。

B) 现在假设域 $K$ 是无限的。如果b)成立，则扩张$E$为有限次数，因此b)也可以用说来表示，$E$仅拥有子代数的有限数。既然如此，$b) \Rightarrow a)$就是下面更一般的命题的推论（其中假设，域$K$是无穷大是不可缺少的，cf.V，p. 153，Ex.5） § 7):

#### 命题 7 {#alg-v-s7-prop-7 .statement tag=06KI}

— *假设$K$无穷大；设 $A$ 为交换性 $K$-代数，仅拥有有限数子代数（对于例一个 etale $K$-代数，$V$，p. 30，命题 3）并令 $V$ 为向量子空间共$A$生成的$A$。那么存在 $x \in V$ 使得 $A = K[x]$.*

令 $A_1, \ldots, A_n$ 为与 $A$ 不同的 $A$ 的子代数。如果 $x \notin A_1 \cup \ldots \cup A_n$，则子代数 $K[x]$ 不能等于任何 $A_i$，因此必须重合与 $A$。另外，由于$V$生成$A$，所以不包含在子空间$A_i$中。因此，第 7 号提案是以下引理中的推论：

#### 引理 1 {#alg-v-s7-lem-1 .statement tag=06KJ}

*令$A$为向量$K$-空间，$V, A_1, \ldots, A_n$子空间等于$A$。如果 $\mathrm{Card}(K) \geq n$ 且 $V$ 不包含在任何 $A_i$ 中，则 $V$ 不包含在 $A_1 \cup \ldots \cup A_n$ 中。*

由归纳对$n$论证，我们只需证明如果$V \subset A$，且$V \subset A_1 \cup \ldots \cup A_n$，则$V \subset A_1 \cup \ldots \cup A_{n-1}$。 令$x \in V, x \notin A_n$，并令$y$在$V$中任意。 如果$y \in Kx$，我们有$y \in A_1 \cup \ldots \cup A_{n-1}$；如果不是，则元素$x$和$y + \lambda x, \lambda \in K$严格大于数和属于到$A_1 \cup \ldots \cup A_n$中的$n$，因此其中两个属于到同一个$A_i$。 因此，存在$i, 1 \leq i \leq n$，对于某些$\lambda \in K$，存在$x \in A_i$和$y + \lambda x \in A_i$，或者对于两个不同的标量$\lambda, \mu \in K$，存在$y + \mu x \in A_i$和$y + \mu x \in A_i$。 在这两种情况下，我们结论即$x \in A_i$和$y \in A_i$；但这意味着$i \neq n$，因此$y \in A_1 \cup \ldots \cup A_{n-1}$，正如我们希望展示的那样。

这样就完成了Th中a)和b)的等价的证明。 1. 最后，如果扩张 $E$ 可分，且有限次数、条件 b) 成立，则由 V、p. 30，命题 3。

### 5.可分离代数扩张的稳定性性质

#### 命题 8 {#alg-v-s7-prop-8 .statement tag=06KK}

— *令$E$是$K$和$(E_i)_{i \in I}$的扩张，是$E$的子扩展族，使得$E = K \left( \bigcup_{i \in I} E_i \right)$。如果每个扩张 $E_i$ 都是代数且在 $K$ 上可分，则 $E$ 也是如此。*

这立即来自第 6 号提案 (V, p. 39)。

$^1$ 读者可能会说服自己Th。 V、p. 78 引理 1 之前证明任何地方都没有使用 1。

#### 命题 9 {#alg-v-s7-prop-9 .statement tag=06KL}

— *设 F 是 K 的代数扩张，E 是 F 的子扩展。为了使 F 在 K 上可分，F 在 E 上可分且 E 在 K 上可分是充分必要的。*

首先假设 F 在 K 上可分；那么 E 可以通过命题 1 (V, p. 36) 在 K 上分离。此外，F 的每个元素在 K（V，p. 39，命题 6）上可分，因此在 E（V，p. 39，Cor.2）上可分，因此 F 在 E（V，p. 39，命题 6）上可分。

相反，假设 F 在 E 上可分，E 在 K 上可分。用 F 的 x 元素和 $f \in E[X]$ 表示 x 在 E 上的最小多项式。由于 E 在 K、Th 上是代数。 2 (V,p. 18)表明在K上存在有限次数的E的子扩展E'，使得$f \in E'[X]$；那么 f 同时是 x 在 E 和 E' 上的最小多项式，并且由于 x 在 E (V, p. 39, 命题 6) 上可分，因此在 E' (V, p. 39, 命题 5) 上也是可分的。写$F' = E'(x)$；则 F 可分且在 E' 上有有限次数，并且由于 E 在 K 上可分，因此 E' 在 K 上可分且有有限次数（V，p. 36，命题 1）。因此，F 是可分的，并且有限次数在 K 上，通过 V，p. 32，Cor。 2. 因此 (V, p. 39, 命题 6) x 在 K 上可分。我们现在已经证明 F 的每个元素在 K 上可分，因此 F 在 K 上可分 (V, p. 39, 命题 6)。

#### 命题 10 {#alg-v-s7-prop-10 .statement tag=06KM}

— *设 E 和 K' 是 K 的同一扩张的两个子扩展，并设 $E' = K'(E)$。假设 E 是 K 上的代数，因此 E' 是 K' 上的代数 (V, p. 18, Cor. 2)。

a) *如果 E 在 K 上可分离，则 E' 在 K' 上可分离._

b) *相反，如果 E' 在 K' 上可分离，并且 E 和 K' 在 K 上线性不相交的，则 E 在 K 上可分离._

断言 *a)* 直接源自第 6 条命题 (V, p. 39)。

在假设 *b)* 下，设 F 是有限次数的 E 在 K 上的子扩展。则 F 和 K' 在 K 上线性不相交的，因此 K'-代数 $F_{(K')} = K' \otimes_K F$ 同构于 $K'(F)$。由于 $K'(F)$ 是有限次数 E' 在 K' 上的子扩展，并且 E' 是代数且在 K' 上可分，因此 K'-代数 $K'(F)$ 是 etale。在其他字中，K'-代数 $F_{(K')}$ 是 etale，现在 Cor.命题 4 的 2 (V, p. 32) 表明 F 在 K 上是 etale 的。因此我们证明 E 在 K 上是可分的。

### 6. 可分离性标准

#### 命题 11 {#alg-v-s7-prop-11 .statement tag=06KN}

— *假设 K 的特征指数为 p，并令 E 为 K 的代数扩张，由集合 S 生成。如果 E 在 K 上可分，则对于所有整数 $n \geq 0$，$E = K(S^{p^n})$；相反，如果 E 在 K 和 $E = K(S^p)$ 上具有有限次数，则 E 在 K 上可分离。_

对于 Cor 来说，案例 $p = 1$ 是微不足道的。 V、p. 37。假设从现在开始$p \neq 1$。

假设 E 是 K 的代数，我们有 $E = K(S)$，因此

$$
K(S^p) = K(E^p) = K[E^p] \quad \text{by V, p.18, Cor. 1.}
$$

如果 E 是 K 上的有限次数，则当且仅当它是 K 上的 etale 代数时，它才是 K 的可分扩张；科。 V、p. 35 表明当且仅当 $E = K[E^p]$ 时才会发生这种情况。

现在假设$E$是可分的并且在$K$上具有无限度。那么$K[E^p]$是子环$K[{E'}^p]$的并，其中$E'$范围超过集合，是有限次数的$E$在$K$的子扩展；但是这样的扩张$E'$可以通过$K$（$V$，p. 36，命题1），从而$E' = K[{E'}^p] \subset K[E^p]$来分离；最后我们有了$E = K[E^p]$。通过$n \geq 0$上的归纳，关系$E = K[E^p]$意味着$E = K[E^{p^n}]$。

#### 推论 1 {#alg-v-s7-prop-11-cor-1 .statement tag=06KO}

— *完美域的每个代数扩张都是完美域。*

令$K$为特征指数$p$的完美域，并令$E$为$K$的代数扩张。那么 $E$ 可以通过 $K$ ($V$, p. 36, 命题 2) 从而 $E = K(E^p)$ 通过命题 11 分离；但我们有$K = K^p \subset E^p$，因此$E = K(E^p) = E^p$，所以$E$是完美的。

#### 推论 2（Mac Lane）{#alg-v-s7-prop-11-cor-2 .statement tag=06KP}

— *令$K$为$K$和$K^{p^{-\infty}}$的代数闭包，$\overline{K}$中$K$的完美闭合。对于 $\overline{K}$ 的子扩展 $E$ 在 $K$ 上可分离，它应该是从 $K^{p^{-\infty}}$ 到 $K$ 线性不相交的的必要且充分的。*

我们可以立即将约化转化为$[E : K]$有限的情况。设$(x_i)_i$为$E$除$K$的基。对于$E$从$K^{p^{-\infty}}$线性地不相交的来说，对于所有$n \geq 0$来说，从$K^{p^n}$开始也是线性的不相交的是必要且充分的，这仅仅意味着关系$\sum_{i \in I} x_i a_i^{p^{-n}} = 0$对于所有$i \in I$、对于任何家庭$(a_i)_i$意味着$a_i = 0$， 元素 $K$。这反过来意味着家庭$(x_i^{p^n})_{i \in I}$在$K$上是免费的，或者也意味着它是向量空间$E$在$K$上的基。换句话说，当且仅当$E = K(E^{p^n})$时，$E$与$K^{p^{-n}}$呈线性不相交的。现在应用第 11 条提案就足够了。

#### 注 {#alg-v-s7-n6-rem-1 .statement tag=06KQ}

— 1) 当$E$是代数并且在$K$上具有无限次时，条件$E = K(E^p)$并不总是确保$E$在$K$上可分。对于例，如果$K$是不完美的，并且$E$是$K$的完美闭包，那么我们有$E = K(E^p)$，但$E$不是$K$的可分扩张（$V$，p. 39，Cor.3）。
2) 设$E$特征指数$p$的域$K$的可分离代数扩张。那么我们有$E^p \cap K = K^p$（Cor.2）；因此，如果$E$是完美的，$K$也是如此。

### 7. 相对可分代数闭包

#### 命题 12 {#alg-v-s7-prop-12 .statement tag=06KR}

— *令$E$为$K$和$E_s$的扩张，$E$的元素为集合，它们是代数且可在$K$上分离。那么 $E_s$ 是 $E$ 的最大的子扩展，它是代数且在 $K$ 上可分。*

根据命题 6，*a*) ($V$, p. 39) $E$ 的每个子外延在 $K$ 上是代数且可分的，都包含在 $E_s$ 中。根据命题 6，*b*) (*loc.cit.*) $K$ 的扩张 $K(E_s)$ 是代数且可分离的，从而 $K(E_s) \subset E$，所以 $K(E_s) = E_s$。

与前面的命题的记号，E，称为E中K的相对可分（代数）闭包。当K完美时，E，是E中K的相对代数闭包（V，p. 36，命题2）。

#### 命题 13 {#alg-v-s7-prop-13 .statement tag=06KS}

— 令 E 为 K 的代数扩张，并令 E_s 为 E 中 K 的相对可分代数闭包。
a) E 是 E, 的 p 根扩展。
b) 如果 F 是 E 的子扩展，使得 E 是 F 上的 p 根式，则 F ⊃ E,。
c) E，是 E 的唯一子外延，它可在 K 上分离，且 E 是 p 根式。
当 K 具有特征 $p \neq 0$ 时，只要证明 a) 就足够了。设 x 为 E 的元素，f 为 K 上的最小多项式。存在整数 $m \geq 0$，使得 f 属于到 $K[X^{p^m}]$ 但不到 $K[X^{p^{m+1}}]$；在其他字中，我们有$f(X) = g(X^{p^m})$和$g \in K[X]$，$g \notin K[X^p]$。由于f是不可约的，g也是如此，因此g是$x^{p^m}$在K上的最小多项式。根据V，p. 38，命题4和p. 39，命题5，我们因此有$x^{p^m} \in E_s$，所以E是E上的p根式。

现在假设假设 b) 并令 $x \in E,$。由于 x 在 K 上可分，因此在 F (V, p. 39, Cor. 2) 上也是可分的，但由于 E 在 F 上是 p 根，所以 x 也在 F 上是 p 根，因此 $x \in F$ (V, p. 39, Cor. 3)。

最后，c) 由 a) 和 b) 以及命题 12 得出。

#### 推论 1 {#alg-v-s7-prop-13-cor-1 .statement tag=06KT}

— 令 E 和 K' 为包含在 K 的同一个扩张中的 K 的两个扩张。假设 E 是 K 上的代数，并用 E 表示 K 在 E 中的相对可分代数闭包。则 $K'(E_s)$ 是 K' 在 $K'(E)$ 中的相对可分代数闭包。

因为 $K'(E_s)$ 是由命题 10 (V, p. 42) 得出的 K' 的可分代数扩张；因为 E 是 E_s 上的 p 根式，所以 $K'(E_s)$ 的扩张 $K'(E)$ 是 p 根式（V、p. 25，Cor.）。现在应用第 13 条提案就足够了。

#### 推论 2 {#alg-v-s7-prop-13-cor-2 .statement tag=06KU}

— 如果 E 的有限次数超过 K，则 $E_s = \bigcap_{n \geq 0} K(E^{p^n})$。

对于 F 表示的每个整数 $n \geq 0$，E 的子扩展$K(E^{p^n})$。E 的向量子空间序列 $(F_n)_{n \geq 0}$ 是下降的，并且 E 是 K 上的有限维。因此存在整数 $m \geq 0$ 这样$F_m = F_n$ 代表所有 $n \geq m$。因此我们有$K(F_m^p) = F_{m+1} = F_m$，因此$F_m$是K的可分扩张（V，p. 42，命题11）；很明显，E 是 F 上的 p 根式，因此第 13 条命题意味着 $E_s = F_m = \bigcap_{n \geq 0} F_n$。

#### 注 {#alg-v-s7-n7-rem-1 .statement tag=06KV}

令 E 为 K 和 E 的代数扩张，即 E 在 K 中的相对 p 根闭包 (V, p. 25)。那么 E 是 E 的最大的子扩展，E 是 K 上的 p 根式（V，p. 25，命题 2）。然而，E 通常与 E 不可分，(V, p. 152, 例 2)；对于拟伽罗瓦扩展的情况，请参见V，p. 76。

### 8. 可分闭包 / 域

#### 定义 4 {#alg-v-s7-def-4 .statement tag=06KW}

— *A field K is said to be separably closed if every separable algebraic extension of K is trivial.*

代数闭域是可分离闭的。相反，如果完美域 K 是可分离闭的，则它是代数闭的，因为 K 的每个代数扩张都是可分离的（*V*，p. 3 ，命题 2）。

#### 定义 5 {#alg-v-s7-def-5 .statement tag=06KX}

— *令 K 为域。通过 K 的可分代数闭包，或（滥用语言）可分闭包，我们理解 K 的任何扩张 E，它是代数且在 K 上可分的，并且域 E 是可分闭的。*

当 K 完美时，可分闭包的概念和 K 的代数闭包之间存在完全恒等式（*V*，p. 36，命题 2 和p. 43，Cor.1）。

#### 命题 14 {#alg-v-s7-prop-14 .statement tag=06KY}

— *令 Ω 为 K 的代数闭扩张。*

a) *Ω 中 K 的相对可分离代数闭包 Ω_s 是 K 的可分闭包。*

b) *如果E和E'是K的两个可分闭包，则存在E到E'的K同构。_

设 F 为 Ω_s 的可分离代数扩张 ；由于 Ω 是代数闭的，因此存在 F 到 Ω 的 0,-同态 u (*V*, p. 20, Th. 1)。根据命题 9 (V, p. 42) $u(F)$ 在 K 上可分，因此$u(F) = \Omega_s$。因此 F 是 $\Omega_s$ 的平凡扩张，因此 $\Omega_s$ 是可分离闭的，从而 *a)*。

设E为K的可分闭包。由于E是K的代数扩张，因此存在E到Ω的K同态v（*V*，p. 20，Th.1）。因此 $v(E)$ 是 K 上的可分代数，从而 $v(E) \subset \Omega_s$。根据 *V*、p. 42、第 9 条命题，$\Omega_s$ 在 $v(E)$ 上是可分的，并且由于域 $v(E)$ 是可分闭的，所以我们有 $v(E) = \Omega_s$。由此可见 v 是 E 在 $\Omega_s$ 上的 K 同构的。现在 *b)* 是直接的推论。

#### 推论{#alg-v-s7-n8-cor-1 .statement tag=06KZ}

— *令 E 为 K 的可分离闭扩张，F 为 K 的可分离代数扩张；那么存在 F 到 E 的 K-同态._

设 Ω 为 E 的代数闭包；我们有$\Omega_s \subset E$，足以处理$E = \Omega_s$的情况。由于 F 是 K 的代数扩张，因此存在 F 到 Ω 的 K 同态 u (*V*, p. 20, Th. 1)。由于域 $u(F)$ 在 K 上可分，因此我们有 $u(F) \subset \Omega_s$ 和 u 定义 F 到 $\Omega_s = E$ 的 K 同态。

#### 注 1 {#alg-v-s7-n8-rem-1 .statement tag=06L0}

设E和E'是K的两个可分闭包。如果K不是可分离闭的，则存在E到E'的多个K同构。 \* 因为 E 是 K 的非平凡伽罗瓦扩张，因此存在与恒等式 (*V*, p. 56, Th. 1) 不同的 E 的 K 自同构。

#### 注 2 {#alg-v-s7-n8-rem-2 .statement tag=06L1}

\* 设 E 是 K 的代数和可分扩张。如果 K 的每个代数和可分扩张同构于 E 的子外延，则 E 是 K 的可分闭包。如果 E' 是 K 的可分闭包，则扩张 E 和 E' 中的每一个都同构于一个子外延另一个的；因此E和E'是K的同构扩张（V，p. 52，命题1，a））。

### 9. 可分离与不可分离扩张次数有限次数

设 E 为 K 的有限次数的扩张和 K 的 $\Omega$ 代数闭包。回想一下（V，p. 31），通过 E 与 K 的*可分离的次数*，写成$[E : K]_s$，我们理解数 E 的 K 同态变为 $\Omega$。

#### 命题 15 {#alg-v-s7-prop-15 .statement tag=06L2}

*设E为E中K的相对可分闭包；然后*$[E : K]_s = [E_s : K]$。

域 $\Omega$ 是完美的，E 是 $E_s$ 上的 p 根式，根据 V、p. 44，第 13 条；因此，第 3 条命题（V，p. 26）表明，E 的每个 K 同态都以一种独特的方式进入 $\Omega$ 扩展，而 E 的 K 同态则进入 $\Omega$；因此我们有$[E : K]_s = [E_s : K]$。由于E是K的有限次数的可分扩张，所以它是K上的etale代数；所以我们有$[E_s : K]_s = [E_s : K]$乘以V，p. 32，命题4，结果如下。

与前面的记号一起，E在$E_s$上的次数被称为E在K上的*不可分割的次数*，并用$[E : K]_i$表示。因此我们有

(1)
$$
[E : K] = [E : K]_s \cdot [E : K]_i
$$
根据第 15 号提案。

当 K 的特征为 0 时，$E = E_s$，$[E : K]_s = [E : K]$ 和 $[E : K]_i = 1$。如果 K 具有特征 $p \neq 0$，数 $[E : K]_i$ 是 p 的幂，因为 E 是 $E_s$ 上的 p 根（V、p. 44，命题 13 和 p. 26，命题 4）。需要注意的是，$[E : K]_i$不一定等于$p$除$[E : K]_s$的最高幂，也不一定等于E在K中的相对偏基闭包的次数$[E_s : K]$（V，p. 152，Ex. 3 和 2)。

#### 命题 16 {#alg-v-s7-prop-16 .statement tag=06L3}

*令$\Omega$为K和E、F的扩张，是$\Omega$、有限次数在K上的两个子扩展。*

a) *如果$E \subset F$，则*$[F : K]_s = [F : E]_s \cdot [E : K]_s$，*和*$[F : K]_i = [F : E]_i \cdot [E : K]_i$。

b) *令$K'$为$\Omega$的子扩展；那么我们有*
$$
[K'(E) : K']_s \leq [E : K]_s \quad \text{and} \quad [K'(E) : K']_i \leq [E : K]_i,
$$
*如果 $K'$ 是从 E 到 K 的线性不相交的，则等式成立。*

c) *我们有*$[K(E \cup F) : K]_s \leq [E : K]_s \cdot [F : K]_s$，*和*$[K(E \cup F) : K]_i \leq [E : K]_i \cdot [F : K]_i$，*和等式，如果E和F在K*上线性不相交的成立。

关于a)中可分离的次数，断言由(9)(V，p. 32)得出。由于$[F : K] = [F : E] \cdot [E : K]$，断言关于不可分割的次数由此和(1)得出。

由科. 13 号提案 (V, p. 44) 和 15 号提案，我们有

(2) $$ [K'(E) : K']_s = [K'(E_s) : K'] , \quad [K'(E) : K']_i = [F'(E) : K'(E_s)] ; $$

当 K' 在 K 上从 E 线性不相交的时，则 E 从 K' 在 K 上线性不相交的并且 E 从 K'(E_s) 在 E_s 上线性不相交的（V，p. 15，命题 8）。 断言 b) 现在源自第 5 号提案 (V、p. 14)。

由 a) 我们有 $$ [K(E \cup F) : K] = [F(E) : F] . [F : K]_s ; $$ b) 我们有 $$ [F(E) : F] , \leq [E : K] , \text{ with equality if } E \text{ and } F \text{ are linearly disjoint over } K. $$ 因此我们得到不等式 $$ [K(E \cup F) : K] , \leq [E : K] , . [F : K] , \text{ with equality if } E \text{ and } F \text{ are linearly disjoint over } K. $$ 断言 c) 关于不可分的次数以类似的方式证明。

### 习题{#alg-v-s7-exercises}

§ 7](exercises/s7/)参见[习题。
