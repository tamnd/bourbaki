---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 2
section_title: Zeros of polynomials
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.14-A IV.19, A IV.87-A IV.88
pdf_pages: 0023-0028, 0096-0097
extraction: ocr
subsections:
    - "no": 1
      title: Roots of a polynomial in one indeterminate. Multiplicity
      page: 14
      pdf_page: 23
    - "no": 2
      title: Differential criterion for the multiplicity of a root
      page: 17
      pdf_page: 26
    - "no": 3
      title: Polynomial functions on an infinite integral domain
      page: 17
      pdf_page: 26
statements: 20
exercises: 13
content_sha256: 7b51ba95706df481df3da241acc9a00367de7e02f1e6a5d59ecd9aa5f82a917f
translated_from: content/en/alg/IV/02_s2_zeros_of_polynomials.md
translation_method: google
source_content_sha256: 581af5e1e6500b23403ced41ae2a03e6692f4156d4da25e5f960df6e8a7c1371
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0060e0ac2b9c483ea1d381f443facc4c61e8fb63aa73b7eae37b604d14bce85f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。多项式的零

### 1. 一个不定多项式的根。 重数

令 $g \in A[(X_i)_{i \in I}]$ 和$E$ 为单位结合律$A$-代数。设$x = (x_i)_{i \in I}$是$E$的成对可置换元素族。如果$g(x) = 0$，我们可以说$x$是$E^l$中$g$的零。如果$f$是单不定多项式，则$E$中$f$的零也称为$E$中$f$的根。

#### 命题 1 {#alg-iv-s2-prop-1 .statement tag=06AO}

— 设 $f \in A[X]$ 和 $\alpha \in A$。 $f$除以$X - \alpha$的余数为$f(\alpha)$。为了使$\alpha$成为$f$的根，$X - \alpha$应该是$A[X]$中的$f$的除子是充分必要的。

因为如果 $u,\ v \in \mathbf{A}[X]$ 满足 $f = (X - \alpha)\ u + v,\ \deg v < 1$，则 $v$ 是标量，$f(a) = (a - a)\ u(\alpha) + v = v$。这证明了第一个断言，并由此得出第二个断言。

#### 命题 2 {#alg-iv-s2-prop-2 .statement tag=06AP}

— *令$f \in \mathbf{A}[X]$、$a \in \mathbf{A}$，并令$h$为整数$\geq 0$。以下条件是等效的*：
(i) $f$ 能被 $(X - \alpha)^h$整除，但不能被 $(X - \alpha)^{h-1}$整除；
(ii) *存在$g \in \mathbf{A}[X]$使得$f = (X - \alpha)^h g$和$g(a) \neq 0$。
(i) $\Rightarrow$ (ii) 立即由提案 1 得出。
(ii) $\Rightarrow$ (i) ：假设$f = (X - \alpha)^h g$，其中$g$不承认$a$为根。那么$f$可以被$(X - \alpha)^h$整除；如果$g_1 \in \mathbf{A}[X]$存在使得$f = (X - \alpha)^{h+1} g_1$，那么由于$(X - \alpha)^n$不是$\mathbf{A}[X]$中零的除子（IV，p. 9，命题7），我们有$g = (X - a)\ g_1$，所以$g(\alpha) = 0$，即荒谬的。

#### 命题 3 {#alg-iv-s2-prop-3 .statement tag=06AQ}

— *令$f$为$\mathbf{A}[X]$和$a \in \mathbf{A}$的非零元素。提案 2 中仅存在一个整数 $h \geq 0$ 满足条件 (i) 和 (ii)。*
对于条件 (i) 来说这是很清楚的，记住 iff 可被 $(X - \alpha)^h$整除，然后被$\deg f \geq h$整除（IV，p. 9，命题 7）。

#### 定义 1 {#alg-iv-s2-def-1 .statement tag=06AR}

— *对于上面的记号，我们说$a$是阶$h$，或者重数$h$相对于$f$。*
如果$h > 0$我们也说$a$是阶$h$或重数$h$的根。 阶 1 的根称为简单的根，阶 2 的根双根，... 阶$> 1$的根据说是倍数。

#### 注 1 {#alg-iv-s2-n1-rem-1 .statement tag=06AS}

如果$f = 0$我们同意说$a$相对于$f$有阶$\geq h$，无论$a \in \mathbf{A}$和整数$h \geq 0$。对于任何$f \in \mathbf{A}[X]$和$a \in \mathbf{A}$，说$a$相对于$f$有阶$\geq h$意味着$(X - \alpha)^h$除$f$。

#### 注 2 {#alg-iv-s2-n1-rem-2 .statement tag=06AT}

令$B$为交换环包含$\mathbf{A}$为子环。令$f \in \mathbf{A}[X]$非零且$a \in \mathbf{A}$。无论我们将$f$视为$B[X]$的元素还是$\mathbf{A}[X]$的元素，$a$的阶相对于$f$都是相同的。这从命题 2 的条件(ii)中可以清楚地看出。

#### 命题 4 {#alg-iv-s2-prop-4 .statement tag=06AU}

— *令 $f$ 和 $g$ 为 $\mathbf{A}[X]$ 的非零元素。令$a \in \mathbf{A}$，并令$a$相对于$f$和$g$的阶分别为$p$和$q$。*
(i) *$a$相对于$f + g$的阶为$\geq \inf(p, q)$。如果$p \neq q$*，则等于$\inf(p, q)$。
(ii) *$a$相对于$fg$的阶为$\geq p + q$。如果 $\mathbf{A}$ 是整环*，则它等于 $p + q$。

因为我们有 $f(X) = (X - \alpha)^p f_1(X)$、$g(X) = (X - \alpha)^q g_1(X)$ 和 $f_1(\alpha) \neq 0$、$g_1(a) \neq 0$。假设例 $p \leq q$；那么我们有
$$
f(X) + g(X) = (X - \alpha)^p (f_1(X) + (X - \alpha)^{q-p} g_1(X)) .
$$

如果$p < q$，$a$不是$f_1(X) + (X - \alpha)^{q-p} g_1(X)$的根；这就证明了(i)。另一方面，如果$A$是整环，我们就有$f(X)g(X) = (X - \alpha)^{p+q} f_1(X)g_1(X)$和$f_1(\alpha)g_1(\alpha) \neq 0$；这就证明了(ii)。

#### 命题 5 {#alg-iv-s2-prop-5 .statement tag=06AV}

*假设$A$是整环。令$f$为$A[X]$的非零元素，且$\alpha_1, \ldots, \alpha_p$为$A$、阶$k_1, \ldots, k_r$中$f$的成对不同根。我们有*

$$
f(X) = (X - \alpha_1)^{k_1}(X - \alpha_2)^{k_2} \ldots (X - \alpha_p)^{k_p} g(X)
$$

*其中 $g \in A[X]$ 和 $\alpha_1, \ldots, \alpha_p$ 不是 $g$ 的根。*

我们通过 $p$ 上的归纳继续进行，命题对于 $p = 1$ 来说是明显的，根据 Def。 1. 假设 $f(X) = g_1(X)g_2(X)$，其中

$$
g_1(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_{p-1})^{k_{p-1}}, \quad g_2(X) \in A[X].
$$

由于$A$是整环并且$\alpha_p$与$\alpha_1, \ldots, \alpha_{p-1}$不同，因此$\alpha_p$不是$g_1(X)$的根，因此$\alpha_p$是阶$k_p$或$g_2(X)$的根 （提案 4，(ii)）。由此可见 $g_2(X)$ 可以被 $(X - \alpha_p)^{k_p}$整除，所以

$$
f(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_p)^{k_p} g(X)
$$

其中$g(X) \in A[X]$。显然 $\alpha_1, \ldots, \alpha_p$ 不是 $g$ 的根。

#### 定理 1 {#alg-iv-s2-thm-1 .statement tag=06AW}

*设$A$为整环。给定 $A[X]$、次数 $n$ 的非零元素 $f$，则 $A$ 中所有根中的阶的和为 $\leq n$。*

这紧随第 5 号提案而来。

#### 推论{#alg-iv-s2-n1-cor-1 .statement tag=06AX}

*假设$A$是整环，并让$f, g \in A[X]$为次数$\leq n$。如果$A$存在$n + 1$成对不同的元素$x_1, \ldots, x_{n+1}$，使得$f(x_i) = g(x_i)$对应于$1 \leq i \leq n + 1$，则$f = g$。*

应用Th就足够了。 1 到$f - g$。

#### 命题 6（拉格朗日插值公式）{#alg-iv-s2-prop-6 .statement tag=06AY}

— *令$K$为交换域，$\alpha_1, \alpha_2, \ldots, a,$不同于$K$的元素，以及$\beta_1, \beta_2, \ldots, \beta_n$$K$的任何元素。对于$i = 1, 2, \ldots, n$，我们输入*

$$
f_i(X) = \prod_{j \in U(i)} (X - \alpha_j)/(\alpha_i - \alpha_j),
$$

*其中$U(i)$是整数$j$的集合，使得$j \neq i$和$1 \leq j \leq n$。那么 $\beta_1 f_1 + \ldots + \beta_n f_n$ 是 $K[X]$ 的唯一元素 $f$，使得 $\deg f < n$ 和 $f(\alpha_i) = \beta_i$ 对应 $1 \leq i \leq n$。*

唯一性关闭来自Cor。至 Th。 1.设$f = \beta_1 f_1 + \ldots + \beta_n f_n$，那么由于$f_i$有次数$n - 1$，所以我们有$\deg f < n$。另一方面，$f_i(\alpha_j) = 0$代表$j \neq i$和$f_i(\alpha_i) = 1$，因此$f(\alpha_i) = \beta_i$代表$1 \leq i \leq n$。

#### 推论{#alg-iv-s2-n1-cor-2 .statement tag=06AZ}

— 假设 $\mathbf{A}$ 是整环。令次数$< n$中的$f \in \mathbf{A}[X]$，并令$K$为$\mathbf{A}$中的子环，即域。如果$\mathbf{A}$存在$n$不同的元素$\alpha_1, \ldots, a_n$，使得$\alpha_i \in K$和$f(\alpha_i) \in K$对于$i = 1, \ldots, n$，则$f \in K[X]$。

### 2. 重数与根的微分准则

#### 命题 7 {#alg-iv-s2-prop-7 .statement tag=06B0}

— 令 $f \in \mathbf{A}[X]$ 且令 $a \in \mathbf{A}$ 为根关：为了使 $a$ 成为简单的根关，$a$ 不应是 $f$ 的导数 $Df$ 的根是必要且充分的。

到假设，我们有$f = (X - a)\ g$，其中$g \in \mathbf{A}[X]$。要使$a$成为$f$的简单根，$g(\alpha) \neq 0$是必要且充分的。现在我们有$Df = g + (X - \alpha)\ Dg$，从而$(Df)(\alpha) = g(\alpha)$。

更一般地说：

#### 命题 8 {#alg-iv-s2-prop-8 .statement tag=06B1}

— 设$f \in \mathbf{A}[X]$和$a \in \mathbf{A}$，并假设$a$相对于$f$有阶$k \geq 1$：则$a$相对于$Df$有阶$\geq k - 1$。如果$k . 1$在$\mathbf{A}$中可取消，则$a$相对于$Df$有阶$k - 1$。

到假设，存在$g \in \mathbf{A}[X]$，使得$f = (X - a)^k g$和$g(a) \neq 0$。因此$Df = k(X - \alpha)^{k-1}g + (X - \alpha)^k Dg = (X - \alpha)^{k-1}(kg + (X - \alpha)\ Dg)$，它建立了命题的第一个部分。 $X = \alpha$的$kg + (X - \alpha)\ Dg$的值是$kg(a)$，如果$k . 1$在$\mathbf{A}$中可取消，则该值非零；这就证明了命题的第二个部分。

令$k$为整数$> 0$，使得$k . 1 = 0$包含在$\mathbf{A}$中。如果$f(X) = X^k$，则$0$是$f$的阶$k$根，以及$Df$的任意高阶的根。

#### 推论{#alg-iv-s2-n2-cor-1 .statement tag=06B2}

— 设$f \in \mathbf{A}[X]$、$a \in \mathbf{A}$和$p$整数$\geq 0$，进一步假设$p! . 1$在$\mathbf{A}$中可取消。那么，为了使$a$成为阶的根、$f$的$p$，$a$应该是$f, Df, ..., D^{p-1}f$的根而不是$D^pf$的根是充分必要的。

这是根据归纳于 $p$ 提出的第 8 号提案得出的。

### 3. 多项式函数无限整环

#### 命题 9 {#alg-iv-s2-prop-9 .statement tag=06B3}

— 假设 $A$ 是整环。令$I$为集合，$(\mathbf{H}_i)_{i \in I}$由$\mathbf{A}$和$H = \prod_{i \in I} \mathbf{H}_i \subset A'$组成的无限子集族。 Iff 是 $\mathbf{A}[(X_i)_{i \in I}]$ 的非零元素，并且是所有 $x \in H$ 的 $H_f$ 集合，使得 $f(x) \neq 0$，则 $H$ 和 $H_f$ 等价。

a) 首先假设$I$是有限的，并放入$n = \mathrm{Card}\ I$。 命题对于$n = 0$来说是清晰的；我们将通过$n$上的归纳来证明它。 $I$的选择元素$i_0$并放入$J = I - \{i_0\}$，$B = \mathbf{A}[(X_i)_{i \in J}]$。从$f \neq 0$开始，我们可以写成$f = \sum_{k=0}^m g_k X_{i_0}^k$，其中$g_0, \ldots, g_m \in B$和$g_m \neq 0$。通过所有$x \in \prod_{i \in s} H_i$的归纳假设集合K，使得$g_m(x) \neq 0$与$\prod_{i \in J} H_i$等价。对于 $x \in K$ 多项式
$$
h(X_{i_0}) = \sum_{k=0}^m g_k(x) X_{i_0}^k \in A[X_{i_0}]
$$
是非零的。由 Th. 1 (IV, p. 16) 集合 of $a \in H_{i_0}$，使得 $h(\alpha) \neq 0$ 与 $H_{i_0}$ 从而等价
$$
\operatorname{Card} H \geq \operatorname{Card} H_f \geq (\operatorname{Card} K) \cdot (\operatorname{Card} H_{i_0}) = \operatorname{Card} H,
$$
所以$\operatorname{Card} H = \operatorname{Card} H_f$。

b) 在一般情况下，存在有限子集 $I'$ 或 I，使得 $f \in A[(X_i)_{i \in I'}]$。令$H'_f$为所有$x \in \prod_{i \in I'} H_i$中的集合，使得$f(x) \neq 0$。然后
$$
H_f = H'_f \times \left( \prod_{i \in I - I'} H_i \right),
$$
只需应用证明中的第一个部分到$H'_f$即可。

#### 推论 1 {#alg-iv-s2-prop-9-cor-1 .statement tag=06B4}

— *我们保留命题 9 的假设和记号。如果 l 非空，则 $H_f$ 是无限的。*

#### 推论 2 {#alg-iv-s2-prop-9-cor-2 .statement tag=06B5}

— *假设 A 是无限整环或 A 是无限域上的代数。对于每个 $f \in A[(X_i)_{i \in I}]$，令 $\tilde{f}: A^I \to A$ 为由 f (IV, p. 4) 定义的多项式函数。那么映射 $f \mapsto \tilde{f}$ 是单射的。*

当 A 是无穷大整环时，命题 9 立即推出推论。假设 A 在无穷大域 k 上是代数。令$f = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu$为$A[(X_i)_{i \in I}]$的非零元素；则存在 $\nu_0 \in \mathbf{N}^{(I)}$ 使得 $\alpha_{\nu_0} \neq 0$，以及 A 上的 k 线性形式 $\varphi$ 使得 $\varphi(\alpha_{\nu_0}) \neq 0$。让$g = \sum_{\nu \in \mathbf{N}^{(I)}} \varphi(a_\nu) X^\nu \in k[(X_i)_{i \in I}]$；我们有$g \neq 0$，因此存在$x \in k^I$使得$g(x) \neq 0$。然后$\varphi(f(x)) = g(x) \neq 0$，等等$f(x) \neq 0$。

当A是无限整环或当A是代数超过无限域时，我们通常将认同f与$\tilde{f}$。

假设 A 是有限的，并且令 $f(X) = \prod_{a \in A} (X - a)$，然后$f \neq 0$，但是$\tilde{f} = 0$。对于其他例，请参阅IV、p. 88、习题 7 和 8。

#### 定理 2（代数恒等式扩张原理）{#alg-iv-s2-thm-2 .statement tag=06B6}

— *假设 A 是无穷大整环。令 $g_1, \ldots, g_m, f$ 为元素 / $A[(X_i)_{i \in I}]$ 并假设以下假设：*

a）$g_1 \neq 0, \ldots, g_m \neq 0$；
b) *对于所有* $x \in \mathbf{A}^1$ *这样* $g_1(x) \neq 0, \ldots, g_m(x) \neq 0$，*我们有* $f(x) = 0$。 *然后*$f = 0$。

对于如果$f \neq 0$，我们有$fg_1 \ldots g_m \neq 0$（IV，p. 9，命题8），因此存在$x \in \mathbf{A}^1$使得$f(x)g_1(x) \ldots g_m(x) \neq 0$（IV，p. 18，Cor.2），其中与……矛盾假设。

#### 学院{#alg-iv-s2-n3-sch-1 .statement tag=06B7}

— 令 A 为整环和 $f \in A[(X_i)_{i \in I}]$。 Th。 2 提供了证明到 $f = 0$ 的便捷方式。将无限整环 E 包含 A 视为子环就足够了；如果我们可以证明对于所有$(x_i) \in E^I$（或者甚至对于那些给定非零多项式的有限数不会消失的$(x_i) \in E^I$），$f((x_i)) = 0$，那么可以得出$f = 0$。如果A本身不是无限的，我们可以对例取E为环$A[X]$或其分数的域。

一旦我们证明了关系 $f = 0$，我们就可以清楚地推论出对于所有 $(y_i) \in F^I$ $f((y_i)) = 0$，其中 F 是任何单位结合律和交换律 A-代数；特别是 F 可以是有限的或非整数。

在其他$f((x_i)) = 0$的字、证明中，当$x_i$运行于无限整环包含A作为子环时（对于$1 \leq k \leq m$，可能有限制即$g_k((x_i)) \neq 0$，其中$g_k$ 是非零多项式）意味着当 $x_i$ 运行在任何单位结合律和交换律 A-代数上时具有相同的恒等式。

特别是让$f \in Z[(X_i)_{i \in I}]$。如果当$x_i$超过$\mathbf{Z}$时$f((x_i)) = 0$（对于$1 \leq k \leq m$可能有$g_k((x_i)) \neq 0$的限制，其中$g_k$是$\mathbf{Z}[(X_i)]$的非零元素），那么当$x_i$ 运行任意交换环。

### 习题 {#alg-iv-s2-exercises}

§ 2](exercises/s2/)参见[习题。
