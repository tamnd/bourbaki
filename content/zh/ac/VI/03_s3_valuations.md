---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 3
section_title: Valuations
lang: zh
source: ac-i-vii
book_pages: 385-393, 446-449
pdf_pages: 0403-0411, 0464-0467
extraction: ocr
subsections:
    - "no": 1
      title: VALUATIONS ON A RING
      page: 385
      pdf_page: 403
    - "no": 2
      title: VALUATIONS ON A FIELD
      page: 387
      pdf_page: 405
    - "no": 3
      title: TRANSLATIONS
      page: 389
      pdf_page: 407
    - "no": 4
      title: EXAMPLES OF VALUATIONS
      page: 389
      pdf_page: 407
    - "no": 5
      title: IDEALS OF A VALUATION RING
      page: 391
      pdf_page: 409
    - "no": 6
      title: DISCRETE VALUATIONS
      page: 392
      pdf_page: 410
statements: 15
exercises: 8
content_sha256: 9ceb901e555d6c46e9295329b88cdc1ed22f035ee353222a2e5ee44394edf96e
translated_from: content/en/ac/VI/03_s3_valuations.md
translation_method: google
source_content_sha256: 53da8eeb6a8932911f9fa4e5bb93b698a2373f5f22e0893d102d4323fd2301f1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 5dafe43918716927a51f7fd0de06365908b0630a98034305142b27ed7633a77c
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 3. 估值

### 1. 环的估值

令 $\Gamma$ 为加法写成的全序交换律群。在这个章的其余部分，我们必须考虑，对于这样的群，通过邻接由$+\infty;$表示的$\Gamma$元素获得的集合，我们将用$\Gamma_\infty$表示这个集合，并且我们将给出它：（1）总排序$+\infty$ 是最大元素，在其他字中，使得 $a < +\infty$ 对于所有 $a \in \Gamma;$ (2) 一个可交换幺半群结构，其律诱导在 $\Gamma$ 给定的群运算上并且由方程定义

$$
(+\infty) + (+\infty) = +\infty, \quad a + (+\infty) = +\infty
$$

对于所有$\alpha \in \Gamma$；立即验证该律是结合律和交换律，并且$\Gamma_\infty$中的关系$\alpha_1 \leq \beta$对于所有$\gamma \in \Gamma_a$意味着$\alpha_1 + \gamma \leq \beta + \gamma$。

#### 定义 1 {#ac-vi-s3-def-1 .statement tag=04T2}

*令 $C$ 为（不一定可交换的）环和 $\Gamma$ 一个全序可交换的群加法书写。 $\Gamma$ 中值的$C$ 的估值是满足以下条件的任何映射 $v : C \to \Gamma_\infty$：*

(VL_I) $v(xy) = v(x) + v(y)$ $x \in C, y \in C$。
(VL_{II}) $v(x + y) \geq \inf(v(x), v(y))$ 为 $x \in C, y \in C$。
(VL_{III})$v(1) = 0$和$v(0) = +\infty$。

如果$C$除0之外没有零的除子，则$C$至$\Gamma_\infty$的唯一映射$v_0$，使得$x \neq 0$和$v_0(0) = +\infty$的$v_0(x) = 0$是一个估值，称为*不当估值* $C$。如果$z \in C$对于某些整数$n \geq 1$来说$z^n = 1$，那么，通过(VL_I)，$nv(z) = v(z^n) = 0$，因此$v(z) = 0$对于$C$上的*每个*评估$v$，因为$\Gamma$是全序的群。特别是 $v(-1) = 0$、从而 $v(-x) = v(x)$ 对于所有 $x \in C$。此外，从(VL_I)可以得出，对于$C$中的所有$x, y$，$v(xy) = v(yx)$。如果 $x$ 在 $C$ 中可逆，则 $v(x^{-1}) = -v(x)$。

#### 命题 1 {#ac-vi-s3-prop-1 .statement tag=04T3}

*令 $v$ 为（不一定可交换）环 $C$ 的估值。对于任意元素 $x_i \in C$ ($1 \leq i \leq n$)，*

$$
v \left( \sum_{i=1}^n x_i \right) \geq \inf_{1 \leq i \leq n} v(x_i)
$$

此外，如果存在单个指标$k$使得$v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$，则(1)的两侧相等。特别是，如果$v(x) \neq v(y)$，则$v(x + y) = \inf(v(x), v(y))$。

关系 (1) 由公理 (VL_{II}) 通过 $n$ 上的归纳得出。如果存在单个指标$k$使得$v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$，则通过(1)写出$y = \sum_{i \neq k} x_i$和$z = \sum_{i=1}^n x_i$、$v(y) > v(x_k)$和$v(z) \geq v(x_k)$；如果$v(z) > v(x_k)$，关系$x_k = z - y$会给出$v(x_k) \geq \inf(v(z), v(y)) > v(x_k)$，这是荒谬的； 从而$v(z) = v(x_k)$，证明第二个断言。

#### 推论{#ac-vi-s3-n1-cor-1 .statement tag=04T4}

*If a finite sequence of elements $(x_i)_{1 \leq i \leq n}$ of $C$ (for $n \geq 2$) is such that $\sum_{i=1}^n x_i = 0$, there exist at least two distinct indices $j, k$ such that*

$$
v(x_j) = v(x_k) = \inf_{1 \leq i \leq n} v(x_i).
$$

如果只有一个指标$k$，$v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$，命题1将显示$v(x_k) = v(0) = +\infty$，从而$v(x_i) = +\infty$对于所有$i$，与关系$n \geq 2$和假设相反$k$。

注
(1) 如果$v : C \to \Gamma_\infty$是环$B$到$C$对$C$和$u : B \to C$同态的估价，则直接的是映射$B \xrightarrow{u} C \xrightarrow{v} \Gamma_\infty$对$B$的估价$\Gamma$ 中的值。

(2) Conditions (VL$_I$) and (VL$_II$) show immediately that the set $\bar{v}^{-1}(+\infty)$ is a two-sided ideal $\mathfrak{p}$ in $C$ distinct from $C$ by virtue of (VL$_III$); moreover, if $x, y$ are two elements of $C$ such that $v(xy) = +\infty$, it follows from (VL,) that necessarily $v(x) = +\infty$ or $v(y) = +\infty$; in other words, the quotient ring $C/\mathfrak{p}$ has no divisor of 0 other than 0; it is immediately verified that the mapping $\bar{v} : C/\mathfrak{p} \to \Gamma_\infty$ derived from $v$ by passing to the quotient is a valuation on $C/\mathfrak{p}$, the inverse image of $+\infty$ under this valuation reducing to 0.

### 2. 域的估值

#### 命题 2 {#ac-vi-s3-prop-2 .statement tag=04T5}

令$K$为（不一定可交换）域，$v$为$K$的估值，值为$\Gamma$。然后：
(i) 对于$x \neq 0$、$v(x) \neq +\infty$。
(ii) $x \in K$的集合$A$使得$v(x) \geq O$是$K$的子环。
(iii) 对于$\Gamma$、集合$V$、（或$V'_a$）$x \in A$中的所有$a \geq O$，使得$v(x) > a$（或$v(x) \geq a$）是$A$的双面理想以及每个（左或右）理想$A$ 包含 $m$ $V'_a$ $\neq (O)$。
(iv) $x \in A$的集合$m(A)$使得$v(x) > O$是最大的理想的$\#A$在$A$中； $U(A) = A - m(A)$是$A$的可逆元的集合，并且$\kappa(A) := A/m(A)$是（不一定可交换的）域。
(v) 对于所有$x \in K - A$、$x^{-1} \in m(A)$。

断言 (i) 源自$\bar{v}^{-1}(+\infty)$ 是$K$ 的理想，不等于$K$。 The verification of the fact that $A$ is 环 and the $V$, and $V'_a$ two-sided ideals is trivial by virtue of axioms (VL$_I$), (VL$_II$) and (VL$_III$). If $a$ is a (left, for 例) ideal of $A$ and $x \neq 0$ 属于 to $A$, every $y \in A$ such that $v(y) \geq v(x)$ can be written $y = zx$ where $z = yx^{-1}$, hence $v(z) = v(y) - v(x) \geq O$，因此$z \in A$；在其他字左理想$Ax$包含$V'_a$为$a > v(x)$。 集合$U(A) = A - m(A)$是$x \in K$的集合使得$v(x) = 0$；如果$x \in U(A)$，那么
$$
v(x^{-1}) = -v(x) = 0,
$$
从而$x^{-1} \in U(A)$；相反，如果$y \in A$在$A$中可逆，则$v(y) \geq 0$、$v(y^{-1}) \geq 0$和$v(y) + v(y^{-1}) = 0$、从而、$v(y) = 0$和$y \in U(A)$；这证明了 (iv) 和 (v) 紧随定义而来。

$A$（分别为$m(A)$、$\kappa(A)$）被称为$K$上的估值$v$的环（分别为理想、剩余类域）。

显然U(A)是同态$v : K^* \to \Gamma$核和乘法群$K^*$$v$下的像$v(K^*)$是加法群$\Gamma$子群，称为$v$的阶群或值群，因此与$K^*/U(A)$同构的；对于$x \in K$，$\Gamma_\infty$的元素$v(x)$称为估价有时，或$v$称为$x$的阶。如果环相同，则 $K$ 的两个估值 $v, v'$ 被称为等值。

#### 命题 3 {#ac-vi-s3-prop-3 .statement tag=04T6}

*For two valuations $v, v'$ over a (not necessarily commutative) 域 $K$ to be equivalent, it is necessary and sufficient that there exist 同构的 $\lambda$ of the ordered 群 $v(K^*)$ onto the ordered 群 $v'(K^*)$ such that $v' = A \circ v$.*

假设$v$和$v'$等价；将$v$估价的假设、环$A$与$v'$、$v$和$v'$相同（仅限于$K^*$）因子转换为同态$K^* \to K^*/U(A) \xrightarrow{\mu} v(K^*)$， $K^* \to K^*/U(A) \xrightarrow{\nu} v'(K^*)$，其中$\mu$和$\nu$是同构；此外，$v(K^*)$（或$v'(K^*)$）正元素的集合是类模集合的$\mu$（或$\nu$）下的像。 元素 $U(A)$ $\neq 0$ $m(A)$；我们结论$A = v \circ \mu^{-1}$解决了问题，逆命题是显而易见的。

现在假设$K$是交换域；那么，对于$K$的所有评估$v$，评估$v$的环$A$是$K$的评估环，在§ 1, no. 2，定义2的意义上（这证明术语是合理的）；这紧随命题 2 (c) 和§ 1 no. 2、定理 1 (c)。 *相反*，回想一下，对于每个整环$B$，其分数的域是$K$关系的整除性$x|y$（相当于$y \in Bx$）使得$K^*$成为预定的群，其*相关有序群* $\Gamma_B$是$K^*$的$K^*/U(B)$除以$B$的可逆元的群$U(B)$的商，这个群的正值元素是$B^*/U(B)$（其中$B^* = B - \{0\}$）； 映射 $x \mapsto Bx$ 定义，通过经过与有序群 $K^*/U(B)$ 到群（按关系 $\supset$ 有序）的商同构的非零主分数理想$K$（*代数*、章VI, § 1, no. 5）。 环$A$，域为分数$K$，并且群$\Gamma_A = K^*/U(A)$是*全序*，正是K*的*评估环（§ 1, no. 2，定理1） (d))。如果$v_A$表示$K^*$的典范同态到$\Gamma_A$，则直接的$v_A$（由$v_A(0) = +\infty$扩展）是$K$的评估（称为*规范*），其环是$A$；每个等于 $v_A$ 的估价都可以写成 $v = \sigma \circ v_A$，其中 $\sigma$ 是$\Gamma_A$ 的同构到群的子群，其中 $v$ 取其值 (命题 3)； $\sigma \circ v_A$ 称为 $v$ 的*规范分解*。

#### 命题 4 {#ac-vi-s3-prop-4 .statement tag=04T7}

*令$C$为整环，$K$为分数、$C^* = C - \{0\}$和$v : C \to \Gamma_\infty$的域对$C$的估值。那么$K$上存在唯一的估值$w$，其中扩展$v$和$w(K^*)$是$v(C^*)$生成的$\Gamma$的子群。*

通过*代数*的定理 2，章I, § 2, no. 7，从$K^*$到$\Gamma$存在唯一同态$w$，扩展$v|C^*$和$w(K^*)$由下式生成$v(C^*)$。仍有待证明$w$满足公理（VL$_{\text{II}}$）。然后令$x' \in K^*, y \in K^*$使得$x + y \in K^*$；存在$a \in \mathbf{C}^*$使得$ax \in \mathbf{C}^*$和$ay \in \mathbf{C}^*$，从而$a(x + y) \in \mathbf{C}^*$。由于$w$到$\mathbf{C}^*$的限制满足(VL$_{\text{II}}$)，

$$
w(a(x + y)) \geq \inf(w(ax), w(ay)).
$$

两边消去$w(a)$，我们得到

$$
w(x + y) \geq \inf(w(x), w(y)).
$$

### 3. 翻译

令$K$为（交换的）域，$f$为$K$的位置，$v$为$K$的估值，$A$为$K$的环估值。如果$A$是$f$的环和$v$的环，我们可以说$A, f$和$v$是*伴随的。凭借no. 1和§ 2, no. 3，三个对象、$A$、$f$和$v$中的每一个，然后确定另外两个（就地点和估价而言，最高为等价）。特别是以下等价：

$$
\begin{array}{lllll}
x \in A & \Leftrightarrow & f(x) \neq \infty \\
x \in m(A) & \Leftrightarrow & f(x) = 0 \\
x \in A - m(A) = U(A) & \Leftrightarrow & f(x) \neq 0 \quad \text{and} \quad f(x) \neq \infty \Leftrightarrow v(x) = 0 \\
x \in K - A & \Leftrightarrow & f(x) = \infty & \Leftrightarrow & v(x) < 0
\end{array}
$$

每个与估价环、地点或估价相关的结果都可以转换为与其他两个概念相关的结果。因此命题 4 of § 2, no. 4 给出：

#### 命题 5 {#ac-vi-s3-prop-5 .statement tag=04T8}

*令$K$为域，$v$对$K$和$K'$扩张的估值为$K$。 $K'$ 存在估价 $v'$，其限制至 $K$ 相当于 $v$。*

设$\Gamma_v$和$\Gamma_{v'}$为$v$和$v'$的阶群。由于$v'$到$K$的限制等价于$v$，因此$\Gamma_v$的同构$A$存在于$\Gamma_{v'}$的子群上，使得$v' = A \circ v$在$K$上。如果通过$\lambda$将$\Gamma_v$与$\lambda(\Gamma_v)$进行识别，则可知$v'$扩展$v$。

注 $\Gamma_{v'}$ 通常*不同于* $\lambda(\Gamma_v)$，并且 $v'$ 的等价类不一定是唯一的。我们将在§ 8返回*到*这个。

翻译 § 1, no. 3 的定理 3（或 § 2, no. 5 的命题 6），我们得到：

#### 命题 6 {#ac-vi-s3-prop-6 .statement tag=04T9}

*令$K$为域，$K$中的$A$子环以及$K$中的$x$元素。为了使 $x$ 对 $A$ 整的，$K$ 上的每一个在 $A$ 上为正值的估值在 $x$ 上也是正值是必要且充分的。*

从现在开始，我们一般将把进行与上述类似的翻译的麻烦留给读者。

### 4. 例估值

§ 1, no. 4中给出的估价环的例为我们提供了*例1到4*如下：

#### 例 (1) {#ac-vi-s3-n4-exa-1 .statement tag=04TA}

对有限域 F 的每个估值都是不恰当的，因为 F* 的每个元素都是根单位元。

#### 例 (2) {#ac-vi-s3-n4-exa-2 .statement tag=04TB}

如果 K 是域 K' 的子域，则对 K' 的评估的限制对 K 是对 K 的评估。

#### 例 (3) {#ac-vi-s3-n4-exa-3 .statement tag=04TC}

令 k 为域且 K = k((T))。 映射 v 其中映射每个非零形式幂级数到其阶 (代数, 章 IV, § 5, no. 7) 是对 K 的评估，其阶群是 Z 并且其环是 k[[T]]。相关位置是典范同态 f: k[[T]] → k 通过设定 f(u) = ∞ 扩展为 k((T))，如果 u ∉ k[[T]]。

#### 例 (4) {#ac-vi-s3-n4-exa-4 .statement tag=04TD}

设 A 为主理想整环，K 为分数的域，p 为 A 的极值元素。对于 x ∈ K* 令 v_p(x) 表示 x 的分解中 p 到极值元素的指数 (代数， 章VII, § 1, no. 3、定理2)；立即可以看出，v_p 是一个估值，其阶群为 Z，环为 A_{A_p}。通过§ 1, no. 4的命题3，我们获得了直到等价的对K的所有不不当且对A为正的估值。取A=Z，我们恢复了对Q的p进估值（一般拓扑，章IX, § 3, no. 2）；这些估值是在等价以内对 Q 唯一不不当的估值（§ 1, no. 4，推论 1 至命题 3）。取 A = k[X]，其中 k 为域，限制到 k 不恰当的 k(X) 的非不当估值为（最多等价）：一方面是估值 v_P，其中 P 贯穿 k[X] 的不可约单调多项式的集合，另一方面是由下式定义的估值 v

$$
v(P/Q) = \deg(Q) - \deg(P)
$$

对于 P ε k[X] 且 Q ε k[X]（§ 1, no. 4，推论 2 至命题 3）；所有这些估值显然都有Z作为阶群，并且它们的剩余类域是k的单生代数扩张（代数，章V, § 3, no. 1）。

#### 例 (5) {#ac-vi-s3-n4-exa-5 .statement tag=04TE}

C[X, Y] 到 C((T)) 的映射 P(X, Y) ↦ P(T, e^T) 是单射的（实变量的函数，章 IV, §2，命题 9），因此可以扩展到 C(X, Y) 的同构 C((T)) 的子域。 限制例 3 定义中定义的 C((T)) 评估的子域，对 C(X, Y) 的评估对 C 是不正确的，其阶群为 Z，其剩余类域为 C。

no. 2中的命题 4 允许我们对构造进行评估，其阶群和剩余类域给出：

#### 例 (6) {#ac-vi-s3-n4-exa-6 .statement tag=04TF}

令 Γ 为全序群且 k 域。令 Г_+ 为 Г 的正元素和 Г_+ 的 C 代数在 k 上的幺半群。到定义，C 在 k 上有基 (x_\alpha)_{\alpha \in \Gamma_-}，其乘法表为 x_\alpha x_\beta = x_{\alpha + \beta}。如果$x = \sum a_\alpha x_\alpha$是C的非零元素，我们写成$v(x) = \inf_{a_\alpha \neq 0} (a)$和$v(0) = +\infty$；立即验证$C$至$\Gamma_\infty$的映射$v$满足no. 1的条件(VL_I)和(VL_{II})，且$C$为整环。令$K$为$C$和$w$分数域其中扩展$v$(命题4，no. 2)对$K$的估值。由于$\Gamma$的每个元素都是两个正数元素之差，$w$承认$\Gamma$为阶群。令$A$为$w$和$m$的环其最大理想；我们将证明$A$是$m$和$k$的直和（与$k \cdot 1$相同），这将证明$w$的剩余类域与$k$同构的。显然$m \cap k = (0)$。另一方面，用$p$表示由$x_a$生成的$C$的理想，其中$a > 0$，$K$中估值为0的每个元素$x$可以写成形式$(a + y)/(b + z)$，其中$a \in k^*, b \in k^*, y \in p$和$z \in p$；那么

$$
x = ab^{-1} + (by - az)b^{-1}(b + z)^{-1}
$$

从而$w(x - ab^{-1}) > 0$和$x \equiv ab^{-1} \pmod{m}$；这显示了我们的断言。

如果$\Gamma = \mathbf{Z} \times \mathbf{Z}$，那么$K = k(X, Y)$和上面的构造则提供对$k(X, Y)$的估值，这对$k$来说是不合适的，其阶群是$\mathbf{Z} \times \mathbf{Z}$，其剩余类域是$k$。这些估值取决于在 $\mathbf{Z} \times \mathbf{Z}$ 上选择的阶结构。对于例，$\mathbf{Z} \times \mathbf{Z}$可以给出字典顺序。或者事实上，对于无理数数$a$，$\mathbf{Z} \times \mathbf{Z}$可以在同态$(m, n) \mapsto m + n\alpha$下被识别为$\mathbf{R}$的子群（同态是单射的，因为$a$是无理数），并给出由此引起的排序$\mathbf{R}$。

使用no. 2中的命题 4进行评估的其他构造将在§ 10中描述。

### 5. 估值理想环

#### 定义 2 {#ac-vi-s3-def-2 .statement tag=04TG}

*令 G 为有序集合。如果关系 $x \in M$ 且 $y \geq x$ 暗示 $y \in M$，G 的子集称为大调。*

令$K$为域，$v$为$K$、$A$环为$v$以及$G$阶群为$v$。对于每个主要子集$M \subset G$，令$a(M)$为$x \in K$的集合，使得$v(x) \in M \cup \{+\infty\}$。显然$a(M)$是$K$的子A模块。

#### 命题 7 {#ac-vi-s3-prop-7 .statement tag=04TH}

*映射$M \mapsto a(M)$是$G$主修子集的集合递增双射到$K$子A模块的集合。*

令$b$为$K$的子A模块。 $x \in b - (0)$的$v(x)$中的集合是$G$的主要子集$M(b)$。若证明下列方程，则可得命题 7：

(2) $M(a(N)) = N$ 子集 $N$ $G$；
(3) $a(M(b)) = b$ 对于 $K$ 的每个子 A 模块 $b$。

公式 (2) 很容易，因为对于所有$m \in N$，存在$x \in K$使得$v(x) = m$。那么显然$b \subset a(M(b))$；相反，令 $x \in a(M(b))$ 并假设 $x \neq 0$；

那么$v(x) \in M(b)$，因此存在$y \in b$使得$v(x) = v(y)$； 从而 $x = uy$ 其中$v(u) = 0$，证明$x \in A$ $y \subset b$ 并完成证明。

#### 推论{#ac-vi-s3-n5-cor-1 .statement tag=04TI}

令$G_+$为$G$中正元素的集合。 映射$M \mapsto a(M)$是$G_+$专业子集集合双射，到$A$理想集合。

由于$A = a(G_+)$，$a(M) \subset A$相当于$M \subset G_+$。

对于例，极大理想$m(A)$等于$a(S)$，其中$S$表示$G$严格正的元素的集合。

### 6. 离散估值

#### 定义 3 {#ac-vi-s3-def-3 .statement tag=04TJ}

令$K$为（不一定可交换）域，$v$对$K$和$\Gamma$阶群的$v$的估值。如果在 $\mathbf{Z}$ 上存在有序的群 $\Gamma$ 的（必须是唯一的）同构，$v$ 称为离散的。设该同构下$\gamma$为$\Gamma$相应的至$1$的元素； $K$的每个元素$u$使得$v(u) = \gamma$被称为$v$的均匀化器。如果离散估值的阶群为 $\mathbf{Z}$，则称为标准化。

对于例，由主理想*或阶乘的极值元素$p$定义的估值$v_p$，域是一个规范的离散估值，它承认$p$作为均匀化器。特别是，如果$k$是域，则$k[[T]]$是$k((T))$离散估值的环，它承认$T$作为均匀化器。令$S$为维数1、$S$上亚纯函数的$K$域和$S$的$z_0$点的连通复解析簇； $\in K$的集合在$z_0$是全纯的，是离散估值$v$的环；为了让函数$f \in K$对于$v$来说是一致的，它是全纯的且零在$z_0$处是充分必要的，并且在$S$中存在$z_0$的邻域$V$使得限制出发到$V$是$V$的同态到达$\mathbf{C}$原点的邻域。正是这个例和其他类似物是字“均质器”的起源。*

#### 命题 8 {#ac-vi-s3-prop-8 .statement tag=04TK}

令 $K$ 为（不一定可交换）域，$v$ $K$、$A$ 环的离散估值，$v$ 以及$u$ $v$ 的均匀化器。 $A$ 的非零理想是双面的，形式 $Au^n$ ($n \geq 0$) 的非零理想。

可以假设$v$是标准化的，因此$v(u) = 1$。对于所有$x \in K^*$，有整数$n \in \mathbf{Z}$使得$(v(x) = n = v(u^n)$，因此我们可以写

$$
x = zu^n = u^n z',
$$

其中$z, z'$是环$A$中的两个可逆元； 从而命题。

#### 命题 9 {#ac-vi-s3-prop-9 .statement tag=04TL}

令 $A$ 为局部整环，与分数的域不同。以下条件是等效的：
(a) $A$ 是离散估值的环。
(b) $A$ 是主理想整环。
(c) 理想的$m(A)$为主，$\bigcap_{n=1}^{\infty} m(A)^n = (0)$。

(d) $A$ 是 *诺特环*，$m(A)$ 是*本金*。
(e) $A$ 是 *诺特估值环*。

命题 8 表明(a) 蕴涵(b)、(d) 和(e)。如果 $A$ 为主理想整环，则 $m(A) = Au$ 且 $A$ 的每个非零理想为形式 $Au^n$，因为 $A$ 是本地的 (*代数*, 章 VII, § 1, no. 3, 定理 2）；因此$\bigcap_{n=1}^\infty m(A)^n = 0$；这表明(b)蕴涵(c)。另一方面，(d) 意味着 (c)（章 III, § 3, no. 2，命题 5 的推论）；通过命题 2 of § 1, no. 4，(c) 隐含 (a)。因此条件 (a), (b), (c), (d) 是等价的并且隐含(e)。最后假设 (e) 成立，让我们证明 (b) 成立；足以证明以下引理：

#### 引理 1 {#ac-vi-s3-lem-1 .statement tag=04TM}

*令$A$为估值环。每个有限生成的无扭转 $A$ 模块都是自由的。每个有限生成的理想$\mathfrak{a}$ $A$ 都是主要的。每个无扭转 $A$ 模块都是平坦的。*

令$E$为有限生成的无扭转$A$模，并令$x_1, \ldots, x_n$为$E$的生成元，其在数中最小；我们证明它们是线性独立的。如果 $\sum_{i=1}^n a_i x_i = 0$ ($a_i \in A$) 是 $x_i$ 之间的非平凡关系，则 $a_i$ 之一，例如 $a_1$，除所有其他，因为 $A$ 的主要理想的集合完全按包含排序（§ 1, no. 2，定理1）；那么 $a_1 \neq 0$ 因为关系是不平凡的。由于$E$是无扭转的，我们可以通过$a_1$来除，这相当于假设$a_1 = 1$。但$x_1$是$x_2, \ldots, x_n$的线性组合，与$n$的最小特征标相反。因此$E$是免费的。

特别是，$A$的每个有限生成的理想$\mathfrak{a}$是主要的，$\mathfrak{a}$的生成元的系统的所有元素是其中之一的倍数。 命题 3 of 章 I, § 2, no. 4 则表明每个无扭转 $A$ 模块都是平坦的。

### 习题{#ac-vi-s3-exercises}

§ 3](exercises/s3/)参见[习题。
