---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 2
section_title: Linear forms on a Riesz space
lang: zh
source: int-i-vi
book_pages: INT II.19-INT II.21
pdf_pages: 0033-0039, 0043-0045
extraction: ocr
subsections:
    - "no": 1
      title: Positive linear forms on a Riesz space
      page: 9
      pdf_page: 33
    - "no": 2
      title: Relatively bounded linear forms
      page: 10
      pdf_page: 34
statements: 13
exercises: 9
content_sha256: 17098cae15c5c0f3b09644d8068e05a762967592780dc2cf0efb5d28419bfd50
translated_from: content/en/int/II/02_s2_linear_forms_on_a_riesz_space.md
translation_method: google
source_content_sha256: 417cef2f31fafd157b7a2cbea53f12a17f40a56765605873734c2f538ed5f1ad
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: b88439bae75a5e6f4e094ca25e1aeec572e498d522121a1867f105a1e41737a7
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。 线性形式在 RIESZ 空间

### 1. Riesz 空间呈阳性线性形式

我们回忆一下以下定义（TVS，II, §2, No. 5）：

#### 定义 1 {#int-ii-s2-def-1 .statement tag=08KI}

给定一个有序的向量空间 E，如果对于 E 中的每个 $x \geq 0$ 都有$L(x) \geq 0$，则 E 上的线性形式 L 被认为是正数。

由于$L(y) - L(x) = L(y - x)$，关系$x \leq y$意味着$L(x) \leq L(y)$，或者$L$在E上是递增函数，这也是一样的。

#### 例 1 {#int-ii-s2-n1-exa-1 .statement tag=08KJ}

设 A 为任意集合，E 是 A 上定义的所有实值函数的空间 $\mathbf{R}^A$ 的线性子空间。对于每个元素 $a \in A$，映射 $x \mapsto x(a)$ 是 E 上的正线性形式。

#### 例 2 {#int-ii-s2-n1-exa-2 .statement tag=08KK}

令$I = [a, b]$为$\mathbf{R}$的紧区间，E由I上的规范实值函数形成的Riesz空间（FRV，II, §1, No. 3）； 映射 $x \mapsto \int_a^b x(t) \, dt$ 是 E 上的正线性形式。

#### 例 3 {#int-ii-s2-n1-exa-3 .statement tag=08KL}

设 F 为 F 上的任意集合、$\mathscr{U}$ 超滤器（GT、I, §6, No. 4），E 为 F 上有界实值函数的 Riesz 空间 $\mathscr{B}(F)$。对于每个 $x \in E$，$\lim_{\mathscr{U}} x(t)$ 都存在，因为$x(\mathscr{U})$是超滤器相对于紧集$x(F)$的基，因此是收敛的。此外，如果$x \geq 0$则$\lim_{\mathscr{U}} x(t) \geq 0$乘以不等式扩张的原理；因此映射$x \mapsto \lim_{\mathscr{U}} x$是E上的正线性形式。如果将$\mathscr{U}$视为由集合包含元素$a \in F$形成的超滤器，则恢复正线性形式 $x \mapsto x(a)$（例1）。

#### 命题 1 {#int-ii-s2-prop-1 .statement tag=08KM}

令E为E到$\mathbf{R}$的有序向量空间、L映射，使得$L(x + y) = L(x) + L(y)$并且关系$x \geq 0$蕴含$L(x) \geq 0$；然后对于每个标量 $\lambda$ 和每个 $x \geq 0$ $L(\lambda x) = \lambda L(x)$。

由于$L(-x) = -L(x)$（$L$是$\mathbf{R}$中加法群E的表示），我们可以将自己限制在$\lambda \geq 0$的情况。对于每个整数$n \geq 0$，我们有$L(nx) = nL(x)$，从而$L((1/n)x) = (1/n)L(x)$，因此对于每个有理数$r \geq 0$，我们有$L(rx) = rL(x)$。另一方面，E 中的$L$ 是递增；如果$r$和$r'$是有理数数使得$r \leq \lambda \leq r'$，则有$rL(x) \leq L(\lambda x) \leq r'L(x)$；由于 $rL(x)$ 和 $r'L(x)$ 与 $\lambda L(x)$ 的差异尽可能小，因此我们有 $L(\lambda x) = \lambda L(x)$。

#### 命题 2 {#int-ii-s2-prop-2 .statement tag=08KN}

令 E 为实数向量空间，C 一个在 E 中顶点为 0 的凸锥体，使得 $E = C - C$，并且将 C 的 $x \mapsto M(x)$ 映射放入$\mathbf{R}$，使得$M(\lambda x + \mu y) = \lambda M(x) + \mu M(y)$ 对于所有 $x \in C$， $y \in C$、$\lambda \geq 0$、$\mu \geq 0$。那么，存在且仅有一个线性形式L即扩展M到E。

到假设，每个$z \in E$都可以写成$z = y - x$，其中$x, y$属于到C；此外，如果还有$z = y' - x'$和$x' \in C$，$y' \in C$，那么

$M(y) - M(x) = M(y') - M(x')$；因为，从关系$y - x = y' - x'$我们推断出$y + x' = x + y'$，因而$M(y) + M(x') = M(x) + M(y')$。让我们用$M(y) - M(x)$的$L(z)$公共的值来表示$z$的所有表达式作为$C$的两个元素的差$y - x$；立即验证$L$是线性形式在$E$上延伸$M$； $L$的唯一性是由$C$生成空间$E$产生的。

#### 命题 3 {#int-ii-s2-prop-3 .statement tag=08KO}

*令$E$为$E$的元素$\geqslant 0$的有向有序向量空间、$P$集合以及$P$的$x \mapsto M(x)$映射到$\mathbf{R}$，其中值 $\geqslant 0$，这样$M(x + y) = M(x) + M(y)$适用于$P$中的所有$x, y$。那么，存在且仅有一个正线性形式$L$即扩展$M$到$E$。*

从$E = P - P$开始，与命题2中相同的推理首先证明$E$的*加法*映射$L$到$\mathbf{R}$的存在和唯一性到扩展$M$。 命题 1 然后显示对于所有 $\lambda \geqslant 0$ 和所有 $x \in P$，$L(\lambda x) = \lambda L(x)$，从直接的 $L$ 是线性形式。

### 2. 相对有界线性形式

令 $E$ 为有向有序向量空间。令$Q$为$E$上*正*线性形式的集合；它是$E$的代数对偶$E^*$的子集（$E$上所有线性形式的空间）。对于每个标量$\lambda > 0$，$Q + Q \subset Q$和$\lambda Q \subset Q$是直接的（在其他字中，$Q$是$E^*$中的*凸锥体*）。此外，$Q \cap (-Q) = \{0\}$，因为如果$L$和$-L$都是正线性形式，那么$L(x) \geqslant 0$和$L(x) \leqslant 0$对于所有$x \geqslant 0$，从而$L(x) = 0$对于所有$x \geqslant 0$，因此$L = 0$（No. 1，提案 3）。 集合 $Q$ 因此 $E^*$ 上的定义和 *序关系* $L \leqslant M$，相当于 « $M - L$ 是 $E$ » 上的正线性形式，或者再次为 « 对于每个 $x \geqslant 0$， $L(x) \leqslant M(x)$ »;对于这个阶结构，$E^*$的元素$\geqslant 0$是正的线性形式（这证明了引入术语的合理性）。令$\Omega$为$Q$生成的$E^*$的线性子空间，即$E$上线性形式的集合，是*两个正数线性形式的差*；当$E$是Riesz空间时，我们将给出$\Omega$的元素的另一个刻画。

#### 定义 2 {#int-ii-s2-def-2 .statement tag=08KP}

*给定 Riesz 空间 $E$，$E$ 上的线性形式 $L$ 被认为是相对有界的，如果对于 $E$ 中的每个 $x \geqslant 0$，$L$ 在集合上有界$y \in E$使得$|y| \leqslant x$.*

#### 定理 1 {#int-ii-s2-thm-1 .statement tag=08KQ}

1° *在阶中，Riesz 空间 $E$ 上的线性形式 $L$ 相对有界，它是两个正线性形式之差是充要的。*

2° *在 $E$ 上相对有界线性形式有序向量空间 $\Omega$ 是完全格序的 Riesz 空间。*

如果$L = U - V$，其中$U$和$V$在$E$上为正线性形式，关系$-x \leq y \leq x$意味着

$$
-U(x) \leq U(y) \leq U(x) \quad \text{and} \quad -V(x) \leq V(y) \leq V(x),
$$

从而$|L(y)| \leq U(x) + V(x)$就是直接的；因此，$L$是相对有界的。相反，假设 $L$ 是相对有界的；这一切都归结为证明，存在一个正的线性形式$N$，使得$N(x) \geq L(x)$对于所有$x \geq 0$，因为$N - L$将是一个正的线性形式。

现在，如果正数线性形式$N$有性质，那么对于每个$x \geq 0$和$0 \leq y \leq x$，我们有$N(x) \geq N(y) \geq L(y)$，因此$N(x) \geq \sup_{0 \leq y \leq x} L(y)$；如果我们证明实值函数

$$
x \mapsto M(x) = \sup_{0 \leq y \leq x} L(y),
$$

定义在元素 $\geq 0$ 的集合 $P$ $E$ 上，可以扩展到 $E$ 上的正线性形式（也表示为 $M$），我们将演示定理的第一个部分，并且将此外，还证明了$M$是$0$和$L$在$\Omega$中的上乘。从$M(x) \geq 0$到$P$，一切都归结为证明

$$
M(x + x') = M(x) + M(x')
$$

对于元素 $x \geq 0,\ x' \geq 0$ $E$ 中的每对（No. 1，提案 3）。 定义，

$$
M(x) + M(x') = \sup_{0 \leq y \leq x} L(y) + \sup_{0 \leq y' \leq x'} L(y')
= \sup_{0 \leq y \leq x,\ 0 \leq y' \leq x'} L(y + y') \leq M(x + x').
$$

另一方面，对于每个$z$使得$0 \leq z \leq x + x'$，我们有$x + x' = z + u$和$u \geq 0$；由分解引理 (§ 1, No. 1)，存在两个元素 $y,\ y'$，使得 $0 \leq y \leq x,\ 0 \leq y' \leq x'$ 且使得 $z = y + y',\ u = (x - y) + (x' - y')$；然后

$$
L(z) = L(y) + L(y') \leq M(x) + M(x'),
$$

因此$M(x + x') = \sup_{0 \leq z \leq x + x'} L(z) \leq M(x) + M(x')$，它完成了定理的第一个部分的证明。此外，我们已经证明 $\Omega$ 是一个 *Riesz 空间* 并且，对于 $E$ 上的每个相对有界的线性形式 $L$ 以及对于每个 $x \geq 0$，

(1)
$$
L^+(x) = \sup_{0 \leq y \leq x} L(y).
$$

仍有待观察 $\Omega$ 是完全晶格有序的；为此，只需证明*正* 线性形式的任何集合 $H$，在上面有界并指向关系 $\leqslant$，在 $\Omega$ 中具有上界。

更一般地说，我们有以下引理：

#### 引理 {#int-ii-s2-n2-lem-1 .statement tag=08KR}

— *令 E 为有向有序向量空间，$E^*$ 其对偶，以正线性形式为正元素进行排序。设$(u_\alpha)$是$E^*$的元素的递增定向族。如果，对于 E 中的每个 $x \geqslant 0$，$\sup u_\alpha(x) < +\infty$，则族 $(u_\alpha)$ 在 $E^*$ 中有一个至高点 $u$，并且，对于 E 中的所有 $x \geqslant 0$，

$$
u(x) = \sup_{\alpha} u_\alpha(x).
$$

在 E 中所有 $x \geqslant 0$ 的集合 P 中，定义映射 $u$ 乘以公式 (2)；对于所有$\lambda \geqslant 0$和$x \in P$来说，直接的等于$u(\lambda x) = \lambda u(x)$；为了证明引理因此，根据 No. 1 的命题 2 就足够了

$$
u(x + y) = u(x) + u(y)
$$

对于P中的$x, y$。但这就是注意到上的直接的，$u(x) = \lim u_\alpha(x)$相对于指标的有向集合（单调极限定理）。

从公式 (1) 可以立即推断出，如果 $L$ 和 $M$ 是 E 上两个相对有界的线性形式，则对于每个 $x \geqslant 0$，

$$
\begin{cases}
\sup(L, M)(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)) \\
\inf(L, M)(x) = \inf_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)).
\end{cases}
$$

特别是，如果在第一个公式中，$M$被$-L$替换，我们得到

$$
|L|(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} L(y - z).
$$

现在，如果$x = y + z$、$y \geqslant 0$和$z \geqslant 0$，则$-x \leqslant y - z \leqslant x$；相反，关系$|u| \leqslant x$意味着$L(u) \leqslant |L|(|u|) \leqslant |L|(x)$。由此我们推导出公式

$$
|L|(x) = \sup_{|y| \leqslant x} L(y) \quad \text{for } x \geqslant 0,
$$

从而，特别是，

$$
|L(x)| \leqslant |L|(|x|)
$$

对于所有$x \in E$。

#### 命题 4 {#int-ii-s2-prop-4 .statement tag=08KS}

— 在阶中，Riesz 空间 $E$ 上的两个正线性形式 $L, M$ 在空间 $\Omega$ 中彼此互不相容，对于每个数 $\varepsilon > 0$ 和每个 $x \geq 0$ 来说，这是充分必要的$E$，$E$存在两个元素$y \geq 0, z \geq 0$，使得$x = y + z$和$L(y) + M(z) \leq \varepsilon$。

事实上，通过(3)的第二个公式，这个条件表达了$\inf(L, M) = 0$。

#### 命题 5 {#int-ii-s2-prop-5 .statement tag=08KT}

— 令 $L$ 为 Riesz 空间 $E$ 上的正线性形式。 In order that a positive linear form $M$ on $E$ belong to the band generated by $L$ in $\Omega$, it is necessary and sufficient that, for every $x \geq 0$ in $E$ and every number $\varepsilon > 0$, there exist a number $\delta > 0$ such that the relations $0 \leq y \leq x$ and $L(y) \leq \delta$ imply $M(y) \leq \varepsilon$.

让我们首先证明条件是必要的。如果 $M \geq 0$ 属于到 $\Omega$ 中$L$ 生成的能带，则（§ 1, No. 5，第 6 条命题的修正）

$$
M = \sup_n \left( \inf(nL, M) \right).
$$

如果有一个集合

$$
U_n = M - \inf(nL, M),
$$

因而，$U_n$ 是$E$ 上的正线性形式，$\Omega$ 中的$\inf_n U_n = 0$；因而，(引理)$U_n(x)$趋于0，而$n$趋于无穷大，并且存在$n$使得$U_n(x) \leq \varepsilon/2$。固定这样的$n$，我们对所有$y$有$U_n(y) \leq \varepsilon/2$，这样$0 \leq y \leq x$，因此关系$0 \leq y \leq x$意味着

$$
M(y) \leq \frac{\varepsilon}{2} + \inf(nL, M)(y) \leq \frac{\varepsilon}{2} + nL(y);
$$

如果$y$满足$L(y) \leq \varepsilon/2n$，则$M(y) \leq \varepsilon$成立，从而建立了我们的断言。

现在让我们证明条件就足够了。对于$E$上的每个正线性形式$M$，可以写出$M = U + V$，其中$U$属于属于$\Omega$中$L$生成的带，其中$V$与$L$、$U$不相容， $V$ 为正（§ 1, No. 5，Th.1）。如果$M$满足条件或叙述，那么$V = M - U$也满足，因为$0 \leq V \leq M$。由此我们将推导出$V = 0$。对于$E$中的每个$x \geq 0$和每个数$\eta > 0$，存在$E$的两个元素$y \geq 0, z \geq 0$，使得$x = y + z$和$L(y) + V(z) \leq \eta$（命题4）；给定任意数 $\varepsilon > 0$、选择 $\eta \leq \varepsilon$，使得关系 $0 \leq u \leq x$ 和 $L(u) \leq \eta$ 隐含 $V(u) \leq \varepsilon$；然后按照上面的方法确定 $y$ 和 $z$，我们有 $L(y) \leq \eta$，因此 $V(y) \leq \varepsilon$ 等等

$$
V(x) = V(y) + V(z) \leq \varepsilon + \eta \leq 2\varepsilon;
$$

由于$\varepsilon$是任意的，因此对于每个$x \geq 0$，我们都有$V(x) = 0$，即$V = 0$。

#### 例 {#int-ii-s2-n2-exa-1 .statement tag=08KU}

令 E 为 Riesz 空间，配备与其有序向量空间结构（TVS，II, §2, No. 7）兼容的局部凸拓扑。令E'为E的拓扑对偶，并假设在加法中，E的元素$\geqslant 0$的锥体P对于弱化的拓扑*$\sigma(E, E')$来说是*完全的。那么每个连续的线性形式$x' \in E'$都是*相对有界的*，因为我们知道（TVS，II, §6, No. 8，第11号命题的Cor.2），在这些条件下，对于$y \in E$的E集合中的每个$x \geqslant 0$，使得$|y| \leqslant x$是*紧凑* $\sigma(E, E')$。由此我们推断 E 是“完全晶格有序的”；对于（$§ 1$，No. 3，命题 2），足以证明对于上面有界并指向$\leqslant$、截面滤波器$\mathscr{F}$ 的每个集合$H \subset E$，H 的拓扑*在 E 中*收敛$\sigma(E, E')$（后者与E的有序向量空间结构兼容）。通过翻译，我们可以假设$H \subset P$，然后就足以证明$\mathscr{F}$是$\sigma(E, E')$的*柯西滤波器*，或者再次证明每个连续的线性形式$x' \in E'$相对于$\mathscr{F}$都有极限。但是，当$x'$是*正*线性形式时，这立即从单调极限定理得出，并且由于每个线性形式$x' \in E'$都是两个正线性形式（Th.1）的差，因此我们的断言得到了证明。

习题

### 习题 {#int-ii-s2-exercises}

请参阅[习题为 § 2](exercises/s2/)。
