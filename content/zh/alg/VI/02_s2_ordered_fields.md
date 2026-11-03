---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 2
section_title: Ordered fields
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VI.37-A VI.47
pdf_pages: 0330-0341, 0348-0358
extraction: ocr
subsections:
    - "no": 1
      title: Ordered rings
      page: 19
      pdf_page: 330
    - "no": 2
      title: Ordered fields
      page: 20
      pdf_page: 331
    - "no": 3
      title: Extensions of ordered fields
      page: 21
      pdf_page: 332
    - "no": 4
      title: Algebraic extensions of ordered fields
      page: 23
      pdf_page: 334
    - "no": 5
      title: Maximal ordered fields
      page: 25
      pdf_page: 336
    - "no": 6
      title: Characterisation of maximal ordered fields. Euler-Lagrange Theorem
      page: 26
      pdf_page: 337
    - "no": 7
      title: Vector spaces over an ordered field
      page: 28
      pdf_page: 339
statements: 33
exercises: 41
content_sha256: 7618e2f68f7eb79a33c8bb2c4cca43bcba07317978a4d9f7fb3fdf55aaf9d7fe
translated_from: content/en/alg/VI/02_s2_ordered_fields.md
translation_method: google
source_content_sha256: 10e2ee3ef0d0866e43d0f80ca2949c9e257a5a5b6c77401f65001eb032b1d94c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: e16f9d17258dfdae3b4a8d9a463eb7bb8df9632795c9669310b7a32019f0dcce
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。 有序域

### 1. 已订购环

#### 定义 1 {#alg-vi-s2-def-1 .statement tag=06YV}

— 给定交换环$\mathbf{A}$，我们说$\mathbf{A}$上的排序与$\mathbf{A}$的环结构兼容，如果它与$\mathbf{A}$的加法群结构兼容，并且满足以下公理：
（或）关系$x \geqslant 0$和$y \geqslant 0$意味着$xy \geqslant 0$。
环 $\mathbf{A}$ 与这样的排序一起称为有序环。

#### 例 1 {#alg-vi-s2-n1-exa-1 .statement tag=06YW}

环 $\mathbf{Q}$和$\mathbf{Z}$，按照通常的订购方式，订购的是环。

#### 例 2 {#alg-vi-s2-n1-exa-2 .statement tag=06YX}

已订购的环中的乘积，配备乘积订购，是已订购的环。特别是，映射从集合$E$到有序环$\mathbf{A}$的环$\mathbf{A}^E$是有序环。

#### 例 3 {#alg-vi-s2-n1-exa-3 .statement tag=06YY}

有序环的子环通过诱导排序，是有序环。

在有序的环中，关系 $x \geqslant y$ 和 $z \geqslant 0$ 意味着 $xz \geqslant yz$。事实上，这些不等式分别相当于 $x - y \geqslant 0$、$z \geqslant 0$ 和 $(x - y)z \geqslant 0$。
类似地，我们可以证明关系$x \leqslant 0$和$y \geqslant 0$（分别为$y \leqslant 0$）意味着$xy \leqslant 0$（分别为$xy \geqslant 0$）。这些结果通常以符号规则的名义调用（如果两个元素都是 $\geqslant 0$ 或都是 $\leqslant 0$，则称它们具有相同的符号）。它们意味着，如果 $\mathbf{A}$ 是全序环，则每个平方都是正数，特别是每个幂等（例如单位元）都是正数。

#### 例{#alg-vi-s2-n1-exa-4 .statement tag=06YZ}

$\mathbf{Z}$上只有一个完全订购的环结构：实际上，归纳每自然数$n \neq 0$对应$1 > 0$、从而$n > 0$。相反，在 $\mathbf{Z}$ 上存在有序的环结构，它们不是完全有序的（见下文）。

令 $P$ 为有序环 $\mathbf{A}$ 的正元素的集合。已知（VI、p. 3、命题 3）$P$ 确定 $\mathbf{A}$ 上的排序。说 $\mathbf{A}$ 是有序的环等价于说 $P$ 满足以下属性：

$$
\begin{align*}
(\mathrm{AP}_I) &\quad P + P \subset P \\
(\mathrm{AP}_{II}) &\quad PP \subset P \\
(\mathrm{AP}_{III}) &\quad P \cap (-P) = \{0\}
\end{align*}
$$

事实上，$(\mathrm{AP}_I)$和$(\mathrm{AP}_{III})$表明，$\mathbf{A}$的加法群是有序的群（VI，p. 3，命题3），而$(\mathrm{AP}_{,,})$是（OR）的翻译。

回想一下，以下条件对于 $\mathbf{A}$ 上的序关系来说是必要且充分的：

$$
(\mathrm{AP}_{IV}) \quad P \cup (-P) = \mathbf{A}.
$$

#### 例 {#alg-vi-s2-n1-exa-5 .statement tag=06Z0}

在$\mathbf{Z}$中，如果我们将$P$视为正数（通常意义上的）集合，甚至整数，我们会得到环，它不是完全有序的。

还记得，在全序阿贝尔的群、关系 $n \cdot x = 0$（对于自然数 $n \neq 0$）意味着$x = 0$（VI、p. 4）；这给了我们以下结果。

#### 命题 1 {#alg-vi-s2-prop-1 .statement tag=06Z1}

— *完全排序的环是挠元作为 $\mathbf{Z}$ 模块*（II，p. 313）自由的。

### 2. 有序域

#### 定义 2 {#alg-vi-s2-def-2 .statement tag=06Z2}

— 如果 *其排序与其环结构兼容*，则配备全排序的交换 *域称为有序域*。

我们将自己限制在域上*总计* 序关系，因为其他的都非常“病态”（VI、p. 38、示例 6）。

#### 例 {#alg-vi-s2-n2-exa-2 .statement tag=0DID}

*1) 有理数数的域$\mathbf{Q}$为有序域。
2) 有序域的子域，经过诱导排序后，为有序域。
3) \* 实数的域是有序域。 \*

设$K$为有序域。对于所有$x \in K$，我们把

$$
\begin{align*}
\operatorname{sgn}(x) &= 1 & \text{if } x > 0, \\
\operatorname{sgn}(x) &= -1 & \text{if } x < 0, \\
\operatorname{sgn}(x) &= 0 & \text{if } x = 0.
\end{align*}
$$

那么我们就有$\operatorname{sgn}(xy) = \operatorname{sgn}(x) \operatorname{sgn}(y)$；我们称$\operatorname{sgn}(x)$为$x$的*符号*。从$K^*$到乘法群$\{-1, +1\}$的映射$x \mapsto \operatorname{sgn}(x)$是满同态，其中$K$的严格正元素的核、集合，是$K^*$的子群指标2.

相反，如果 $K$ 是交换域并且 $s : K^* \to \{-1, +1\}$ 是满同态，且核在加法下闭合，则 $s$ 是唯一有序域结构的符号映射，其中严格正数元素的集合是$s$的核。

对于$K$中的所有$x$和$y$，我们有$x = \operatorname{sgn}(x)|x|$和$|xy| = |x||y|$。

另一方面，每个有序域都是特征零（命题 1）。

#### 命题 2 {#alg-vi-s2-prop-2 .statement tag=06Z3}

— *令$A$为全序整环，令$K$为分数的域。那么 $K$ 上存在且仅有一个排序，其中限制与 $A$ 上的给定排序相比较，使得 $K$ 有序域。*

每个$x \in K$都可以用形式$x = ab^{-1}$来表示，$a$和$b$可以用$A$和$b \neq 0$来表示。如果$x$为正，则$a$和$b$具有相同的符号，反之亦然。由此可见，如果$K$ 满足上存在规定的条件的排序，那么它是唯一的，并且正元素的集合$P$与$ab^{-1}$的集合相同，其中$a$和$b$是相同符号的$A$中的元素，以及$b \neq 0$。仍有待证明$P$满足条件（AP$_I$）、（AP$_{II}$）、（AP$_{III}$）和（AP$_{IV}$）。这对于 (AP$_{II}$) 和 (AP$_{IV}$) 来说是显而易见的。对于(AP$_I$)，考虑$ab^{-1} + cd^{-1}$，其中我们可以假设$a$、$b$、$c$和$d$为正；这个和就是$(ad + bc)(bd)^{-1}$，$ad + bc$和$bd$都是正数。

To show $(\mathrm{AP}_{III})$, consider an identity of 形式 $ab^{-1} = -cd^{-1}$, so that $ad + bc = 0$.如果我们假设$a$和$b$具有相同的符号，并且$c$和$d$具有相同的符号，则符号规则表明$ad$和$bc$具有相同的符号； 从而$ad = bc = 0$，所以$a = c = 0$；因此$P$确实是满足$(\mathrm{AP}_{III})$。

#### 例 {#alg-vi-s2-n2-exa-1 .statement tag=06Z4}

— 由于 $Z$ 只承认一个全序环结构 (*VI*, p. 19, *例*)，域 $\mathbf{Q}$ 只承认一个全序有序域：这是通常的排序。

### 3. 扩张 / 有序域

#### 定义 3 {#alg-vi-s2-def-3 .statement tag=06Z5}

*设$K$为有序域。 $K$ 的有序扩张为对 $(E, u)$，其中 $E$ 为有序域，$u$ 为递增同态，从 $K$ 到 $E$。*

令$K$为域，令$E$为有序域，令$u : K \to E$为同态。 关系
$$
x \leq y \quad \text{if} \quad u(x) \leq u(y)
$$
是$K$上的总计序关系，它给出了有序域结构，据说是由$E$*诱导*的。如果$K$和$E$是有序域，则同态$u : K \to E$是递增当且仅当$K$的有序域结构是由$E$的有序域结构诱发的。我们通常将认同$K$及其像放在$E$下$u$。

#### 例 {#alg-vi-s2-n3-exa-1 .statement tag=06Z6}

— 1) 每个有序域$K$都是$\mathbf{Q}$的有序扩张。事实上，$K$是$\mathbf{Q}$的扩张，因为它是特征零，而另一方面$\mathbf{Q}$只能以一种方式排序，正如我们刚才所看到的。

2) 令$K$为有序域，并令$K(X)$为函数的有理函数在$K$上的一个不定数中的域。让我们对多项式环 $K[X]$ 进行定义的排序，将正元素取为 $0$ 以及那些前导系数为正的多项式。这样我们就得到了一个全序的环，它的顺序是扩展，而$K$的顺序是扩展。根据应用命题2，我们给出了$K$的有序扩张的$K(X)$结构。 *对于$K = \mathbf{R}$，可以证明以这种方式定义在$K(X)$上的序关系是$+\infty$附近的增长（cf. *VI*，p. 24，命题4）。*

#### 定理 1 {#alg-vi-s2-thm-1 .statement tag=06Z7}

*对于$K$的扩展$E$承认$K$的有序扩展的结构，以下条件是必要且充分的：*
*(OE)* *关系$p_1 x_1^2 + \ldots + p_n x_n^2 = 0$意味着*
$$
p_1 x_1 = \ldots = p_n x_n = 0
$$
*对于任意有限序列$(x_i, p_i)$，由$x$、$E$的元素对和$K$的正元素$p_i$组成。*

条件 (OE) 显然等价于：
(OE') *元素 – 1 不是形式* $px^2$ ($x \in E, p \in K, p \geq 0$) 元素和。

条件 (OE) 是必要的：如果 E 是 K 的有序扩张，则元素 $p_i x_i^2$ 在 E 中为正，因此零如果它们的和是零。另一方面，$p_i x_i^2 = 0$相当于$p_i x_i = 0$。

相反，假设满足条件 (OE)，那么我们将通过构造 E 的子集 P 来对 E 进行定义排序，该 P 满足条件 (AP_I)、(AP_{II})、(AP_{III}) 和 (AP_{IV})，并且K 的正元素的包含集合 $K_+$。 这样的子集 P 肯定会使 E 成为 K 的有序扩张，因为我们将有 $K \cap P = K_+$；事实上，如果 P 为 K 的包含元素 $-a < 0$，则 a 将为属于到 $P \cap (-P)$，与 (APIIII) 相矛盾。

对于定义 P，让我们考虑 E 的子集的集合 $\mathscr{M}$，其中满足 (AP_I)、(AP_{II}) 和 (AP_{III})，以及 $K_+$ 的包含并和E 元素平方集合 C。 这个集合$\mathscr{M}$是非空，为其形式$\sum p_i x_i^2$元素包含集合$P_0$($P_0$满足(AP_{III})紧随从(OE)而来)。

此外，$\mathscr{M}$是归纳的（*集合理论*，III，p. 154，Def.3）。因此，Th 存在。 $\mathscr{M}$中的*集合理论*、III、p. 154、极大元素中的2个，还有待我们证明是否满足（AP_{IV}）；现在这可以从以下引理得出：

#### 引理 {#alg-vi-s2-n3-lem-1 .statement tag=06Z8}

— *让* $P \in \mathscr{M}$ *和* $x \notin P$； *那么存在*$P' \in \mathscr{M}$*使得*$P \subset P'$*和*$-x \in P'$。

取$P' = P - xP$，并检查$P'$是否具有所需的属性。从$0 \in C \subset P$开始，我们有$P \subset P'$。 从而$C \subset P'$和$K_+ \subset P'$。从 $1 \in C \subset P$ 开始，我们就有了 $-x \in P'$。我们有
$$
P' + P' = P - xP + P - xP = P + P - x(P + P) \subset P - xP = P',
$$
从而 (AP_I)。我们有
$$
P'P' = (P - xP)(P - xP) \subset \\
\quad \subset PP + x^2PP - x(PP + PP) \subset P + CP - xP \subset P - xP = P',
$$
从而 (AP_{II})。最后，让我们检查 (AP_{III})：假设给定一个恒等式形式 $p - xq = -(r - xs)$，其中 $p, q, r, s$ 属于为 P；我们由此推导出关系 $x(s + q) = p + r$；如果 $s + q \neq 0$ 我们有
$$
x = (s + q)^{-2}(s + q)(p + r) \in CPP \subset P,
$$
与假设相反；因此$s + q = 0$、从而$p + r = 0$；由于 P 满足 (AP_{III})，我们推断出 $s = q = r = p = 0$，从而完成证明。

#### 推出 1 (*« 阿廷-施赖尔定理 »*) {#alg-vi-s2-thm-1-cor-1 .statement tag=06Z9}

— *必要且充分的条件才能在交换域* E 上存在排序，从而使其成为有序域，即关系* $x_1^2 + \ldots + x_n^2 = 0$ *暗示* $x_1 = \ldots = x_n = 0$。

其必要性是显而易见的。相反，所述条件意味着E属于特征零，因此扩张属于Q；则满足条件 $(OE)$，且 Th.图 1 表明，E 结构上存在 Q 的有序扩张，即有序域结构。

在域 E 上*不*存在任何有序域结构，其中$-1$ 是平方，特别是在代数闭域上。

#### 推出 2 {#alg-vi-s2-thm-1-cor-2 .statement tag=06ZA}

*设 E 为 K 的扩张，承认 K 的有序扩张的结构。对于 E 上的每个这样的结构下元素 $x \in E$ 为正，x 为形式 $\sum_i p_i x_i^2$ 是必要且充分的，其中 $x_i \in E$ 和$p_i$ 是 K 的正元素。*

条件显然就足够了；对于（在Th.1的证明的记号中），如果$x \notin P_0$存在$\mathscr{M}$的极大元素P使得$x \notin P$也是必要的；那么 $-x \in P$ 引理，并且 x 在 P 定义的排序下不是正数，因为 $x \neq 0$。

### 4. 有序域的代数扩张

设 K 为有序域，f 为 K[X] 中的多项式。如果 K 中存在两个元素 a 和 b 使得 $f(a) f(b) < 0$，我们会说 *f 变换在 K* 中签名；那么我们说 *f 变换位于 a 和 b* 之间。

#### 命题 3 {#alg-vi-s2-prop-3 .statement tag=06ZB}

*设 K 为有序域，f 为 K 上的不可约多项式，其中变换在 K 中的 a 和 b 之间签名。则 K 的扩张 $E = K[X]/(f)$ 承认有序扩张的结构。*

我们将在归纳上次数n下争论。对于 $n = 1$ 证明来说是微不足道的。假设结果对于次数$\leq n - 1$成立，我们用反证法证明次数n；通过 Th。 1 因此我们假设关系为形式

$$
1 + \sum_i p_i f_i^2(X) \equiv 0 \pmod{f(X)}, \quad \text{where } f_i \in K[X], \quad p_i \in K \quad \text{and} \quad p_i \geq 0
$$

不失一般性，我们可以假设 $f_i$ 有次数 $\leq n - 1$ (*IV*, p. 11, Cor)。然后

$$
1 + \sum_i p_i f_i^2(X) = h(X) f(X)
$$

其中$h \neq 0$最多有次数$n - 2$。 替换 X 通过上面不等式中的a和b，我们看到$h(a) f(a) > 0$和$h(b) f(b) > 0$。由于 f 变换在 a 和 b 之间按假设签名，因此我们结论 $h(a) h(b) < 0$。那么对于$h(X)$的不可约因子$g(X)$之一，我们有一个类似的不等式：即$g(a)\ g(b) < 0$。但是$1 + \sum_i P_i f_i^2(X) \equiv 0 \pmod{g(X)}$，这表明域$K[X]/(g)$不能是$K$（Th.1）的有序扩张，与归纳假设相反。

#### 注 {#alg-vi-s2-n4-rem-1 .statement tag=06ZC}

存在不可约多项式 $f$ 在有序域 $K$ 上，变换不签入 $K$，但$K[X]/(f)$ 承认 $K$ 的有序扩张的结构 （cf.VI、p. 43、例 26、c））。

在阶中应用之前的命题我们将需要以下结果：

#### 命题 4 {#alg-vi-s2-prop-4 .statement tag=06ZD}

— *令$K$为有序域并令$f \in K[X]$。 $K$中存在区间，其补码$f$与其最高次数项同号。*

我们可以立即将约化转化为一元多项式的情况；那么可以将$x \neq 0$写成$f(x) = x^n(1 + a_1 x^{-1} + \ldots + a_n x^{-n})$。让

$$
M = \sup (1, |a_1| + \cdots + |a_n|).
$$

对于$|x| > M$，我们有$1 + a_1 x^{-1} + \ldots + a_n x^{-n} > 0$，它完成了命题的证明。

#### 推论 1 {#alg-vi-s2-prop-4-cor-1 .statement tag=06ZE}

— *奇数有限次数的有序域的每个扩张承认有序扩张的结构。*

这样的扩张是单调的（V，p. 40，Th.1），与$K[X]/(f)$同构的，其中$f$是奇数次数的不可约多项式。那么只要证明$f$变换签入$K$（命题3），它紧接着命题4。

#### 推论 2 {#alg-vi-s2-prop-4-cor-2 .statement tag=06ZF}

— *如果 $a$ 是有序域 $K$ 的正元素，则多项式 $X^2 - a$ 的每个分裂域 $E$ 都承认有序扩张的结构 $K$.*

如果 $a$ 是 $K$ 中的平方，则结果是微不足道的。否则，首一多项式 $f(X) = X^2 - a$ 是不可约的且有变换符号，因为 $f(0) < 0$ 和 $f(x)$ 与 $x^2$ 具有相同的符号，因此为正，对于 $x$ 是 $K$ 的某个区间的补集。我们现在可以通过应用命题 3 来完成证明。

#### 注 {#alg-vi-s2-n4-rem-2 .statement tag=06ZG}

当有序域 $K$ 包含 $K$ 的正元素 $a$（多项式 $X^2 - a$ 的根）的 « 平方根 » 时，则记号 $\sqrt{a}$ 通常保留为*正* 平方根。如果 $K$ *不* 包含平方根 $b$ 和域 $E$ 中$a$ 的$-b$，则后者可以在*两个* 中成为 $K$ 的有序扩张方式，每一种都从对方*通过* $K$-自同构导出$b$到$-b$；这些顺序之一的选择确定$\sqrt{a}$：它是元素$b$和$-b$中的正数。

如果$a$和$a'$是$K$的两个正元素，其平方根在$K$中，则$\sqrt{aa'} = \sqrt{a} \sqrt{a'}$，由$\sqrt{a}$的定义和符号规则得出。

### 5. 极大有序域

#### 定义 4 {#alg-vi-s2-def-4 .statement tag=06ZH}

— *如果 K 的每个有序代数扩展都是平凡的，则有序域 K 是最大的。*

#### 例 {#alg-vi-s2-n5-exa-1 .statement tag=06ZI}

*我们稍后会看到（Gen.Top.，VIII，p. 1）实数的域 R 是极大有序域。*

极大有序域的存在性是以下定理中的推论：

#### 定理 2 {#alg-vi-s2-thm-2 .statement tag=06ZJ}

— *每个有序域 K 都承认一个有序代数扩张，即极大有序域。*

可以证明这个有序扩张在 K 同构方面是唯一的（VI，p. 40，例 15）。

令$\Omega$为K的代数闭包，并令$\mathfrak{N}$为对$(A, w)$的集合，其中$A$是$\Omega$的子K扩展，$w$是$A$的排序$A$ $K$ 的有序扩张。 阶 $\mathfrak{N}$ by 关系 « L 是 M 的有序扩张 » 在 M 和 $L$ 之间。配备此排序后，$\mathfrak{N}$是一个*归纳*有序的集合：实际上，如果$(L_i)$是$\mathfrak{N}$的元素的全序族，那么域$L = \bigcup L_i$，通过取$L_1 = \bigcup (L_i)_1$排序，是上界 $L_i$。那么$\mathfrak{N}$有极大元素，由*集合理论*，III，p. 154，Th。 2，完成证明。

#### 命题 5 {#alg-vi-s2-prop-5 .statement tag=06ZK}

— *令 K 为极大有序域，并令 f 为 K[X] 中的多项式，其中变换在 K 的两个元素 a 和 b 之间签名（与 $a < b$）。那么 f 在 K 中具有根 x，使得 $a < x < b$.*

至少有一个不可约因子关闭，例如 $a$ 和 $b$ 之间的 $h$、变换符号。那么域$K[X]/(h)$承认$K$的有序扩张（VI，p. 23，命题3）的结构，并且$h$有次数1（定义4）。从$h(a) h(b) < 0$开始，$h$唯一的根$x$使得$a < x < b$，因为次数1的多项式函数是单调的。

#### 命题 6 {#alg-vi-s2-prop-6 .statement tag=06ZL}

— *极大有序域 K 的每个正数元素在 K 中都有平方根。K[X] 中的每个奇数次数多项式在 K 中至少有一个根。*

这立即来自Cor。 2 和 1 到VI、p. 24 的命题 4。

#### 推论 {#alg-vi-s2-n5-cor-1 .statement tag=06ZM}

— *在极大有序域 K 上，仅存在一种与域结构兼容的排序。*

事实上，K 的正元素由其代数结构决定：它们是平方。

### 6. 极大有序域的表征。欧拉-拉格朗日定理

性质由VI的第6条命题表达，p. 25表征极大有序域。更准确地说：

#### 定理 3（欧拉-拉格朗日）{#alg-vi-s2-thm-3 .statement tag=06ZN}

— 令 K 为有序域。那么下面三个属性是等价的：
a) 域 $K(i)$ 是代数封闭的（其中 i 表示 -1 的平方根）。
b) 有序域 K 最大。
c) K 的每个正元素都是平方，$K[X]$ 中的每个奇数次数多项式在 K 中都有根。

很明显，a) 蕴涵 b)：实际上 K 只有两个代数扩张到同构、域 K 本身和 $K(i)$，其中不能是有序的，因为 -1 是平方。

b) 隐含 c) 的事实正是VI、p. 25 的第 6 条命题。

我们仍然需要证明 c) 蕴涵 a)。这将从接下来的两个命题开始。

#### 命题 7 {#alg-vi-s2-prop-7 .statement tag=06ZO}

— 令 K 为有序域，其中每个正数元素为平方。那么$K(i)$的每个元素都是平方，次数2在$K(i)$上的每个多项式在$K(i)$都有根。

让我们首先证明第二个断言约化与第一个断言约化。我们可以将第二个次数多项式 $aX^2 + bX + c$ ($a \neq 0$) 代入下面的形式，通常称为规范三项式形式：

$$
a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)
$$

如果 d 是 $(b^2 - 4ac)/4a^2$ 的平方根，则 $d - (b/2a)$ 是所考虑的二次多项式的根。

现在我们证明每个元素 $a + bi$ ($a \in K, b \in K$) 都是平方；我们正在寻找元素 $x + yi$ 这样

$$
(x + yi)^2 = a + bi;
$$

这转化为 $x^2 - y^2 = a$ 和 $2xy = b$。由此我们推断

$$
(x^2 + y^2)^2 = a^2 + b^2
$$

令c表示$a^2 + b^2$的正平方根；然后是$c \geq |a|, c \geq |b|$和$x^2 + y^2 = c$。 从而$x^2 = (c + a)/2$和$y^2 = (c - a)/2$。由于$c \geq |a|$这些方程可溶于K，并且如果$x_0$和$y_0$是两个解，则$x_0^2 - y_0^2 = a$和$2x_0y_0 = \pm b$。我们通过取$x = x_0$和$y = b/2x_0$得到所需的平方根。

#### 命题 8 {#alg-vi-s2-prop-8 .statement tag=06ZP}

— 对于多项式 $X^2 + 1 \in K[X]$ (V, p. 21)，令 K 为交换域（任意特征），并令$K'$ 为分裂域。假设：
a) 奇数次数的$K[X]$中的每个多项式在$K'$中都有根；

b) 次数 2 的 $K'[X]$ 中的每个多项式在 $K'$ 中都有根。
那么 $K'$ 是代数闭的。

注首先足以证明$K[X]$中的每个非常数多项式在$K'$中都有根：这确实很清楚如果$K' = K$；如果$K' \neq K$则$[K':K] = 2$；让$a \mapsto a$表示$K'$的唯一$K$自同构，与恒等式映射不同；如果$f \in K'[X]$且$\bar{f}$表示由$f$的应用$a \mapsto \bar{a}$到系数得到的多项式，则$f \bar{f} \in K[X]$；如果$a \in K'$是$f \bar{f}$的根，则$a$是$f$的根或$\bar{f}$；因此$a$或$a$是根或$f$。

因此，令$f$为次数$2^n p$、$p$奇数的$K$多项式。 *我们*将在$n$在归纳出发，性质在$n = 0$在假设*a)*成立。令 E 为 $K$ 的扩张，其中 $f$ 分裂的变为线性因子：

$$
f(X) = \prod_i (X - a_i)
$$

设 $b \in K$；把 $y_{ij} = a_i + a_j + ba_i a_j \in E$ 和

$$
h(X) = \prod_{i < j} (X - y_{ij}) \in E[X].
$$

该多项式的系数在$a_i$中对称函数，在$K$中系数对称；因此属于至$K[X]$（IV、p. 62、Th.1）；因为它有次数$2^n p (2^n p - 1)/2 = 2^{n-1} p'$（$p'$奇数），所以它有根$y_{}$，在$K'$中归纳假设。如果我们注意到这对所有$b \in K$都成立，并且$K$是一个无限域（实际上是有限域，它具有任意大奇数次数的单生扩张（V，p. 94，命题3），不能满足 *a)*)，那么我们可以推导出至少一个对 $(i, j)$ 的存在：

$$
a_i + a_j + ba_i a_j \in K' \quad \text{and} \quad a_i + a_j + b'a_i a_j \in K',
$$

$b \neq b'$。那么$a_i + a_j$和$a_i a_j$是$K'$的元素，因此$a_i$和$a_j$也是，因为它们是二次方程的根

$$
x^2 - (a_i + a_j)x + a_i a_j = 0.
$$

Q.E.D.

对于基于 Galois 理论的第 8 号命题的概括和替代证明，请参阅 VI、p. 46、Ex。 33.

令$K$为有序域，并令$K' = K(i)$；对于$K'$的每个元素$z = a + bi$，$z$的范数$z \overline{z} = a^2 + b'$相对于$K$（III，p. 544，例1）是正元素 $K$，仅在$z = 0$时消失。如果$K$中的每个正元素都是平方（特别是如果$K$是极大有序域），那么范数$z \overline{z}$的正平方根被称为绝对值 $z$，写为$|z|$。从 $|zz'|^2 = |z|^2 |z'|^2$ 开始，我们就有了 $|zz'| = |z| \cdot |z'|$。

而且，三角形不等式

$$
|z + z'| \leq |z| + |z'|
$$

对于元素 $z, z'$ $K'$ 中的每一个对都成立。事实上，如果$z = a + bi$和$z' = a' + b'i$，那么这个不等式相当于

$$
(a + a')^2 + (b + b')^2 \leq a^2 + b^2 + {a'}^2 + {b'}^2 + 2 \sqrt{(a^2 + b^2)({a'}^2 + {b'}^2)}
$$

因此也

$$
(aa' + bb')^2 \leq (a^2 + b^2)({a'}^2 + {b'}^2)
$$

可以写成$(ab' - ba')^2 \geq 0$。

Th。 3 使我们能够确定极大有序域上的所有不可约多项式：

#### 命题 9 {#alg-vi-s2-prop-9 .statement tag=06ZQ}

— *如果 K 为极大有序域，则 K[X] 中唯一不可约多项式是第一个次数多项式，以及第二个次数多项式 $aX^2 + bX + c$，使得 $b^2 - 4ac < 0$。*

由于 $K(i)$ 是代数闭集，K 的每个代数扩张，以及 K 上的每个不可约多项式，都有次数 1 或 2。 要查看第二个次数多项式是不可约的，只需考虑规范形式 $a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)$ （cf. *VI*，p. 26，提案 7）。

#### 注{#alg-vi-s2-n6-rem-1 .statement tag=06ZR}

— 转换为正则三项式形式会产生更强的结果：对于给定有序域 K 上的多项式 $aX^2 + bX + c$ ，在 K 中具有恒定符号的必要且充分的条件是 $b^2 - 4ac < 0$，然后多项式的符号是 $a$。

### 7. 向量空间超过有序域

令 K 为有序域，令 E 为向量空间 $K$。 关系 « $K$ 中存在 $\lambda > 0$，使得 $y = \lambda x$ » 在集合 $E - \{0\}$ 中的两个元素 $x$ 和 $y$ 之间是一个 *等价关系*。 关系下的等价类称为*原点为0的开放半线*；开半线的并和$\{0\}$称为*闭半线*（或有时只是一个*半线*），原点为0。开（或闭）半线A中包含的每个向量$a \neq 0$称为$A$的*方向向量*，并且对于所有标量 $A > 0$（或 $A \geq 0$），$A$ 是向量 $ha$ 的集合。每行 $D$ 到 0 包含正好有两条以 0 为起点的开（或闭）半线；如果 $A$ 是其中之一，则 $-A$ 是另一个（称为 $A$ 的*对立*）。

现在，如果$F$是$K$上的*仿射空间*，并且E空间是F的平移，那么形式$A = a + A_0$的F的任何子集，其中$\Delta_0$是E的开（或闭）半线，被称为*开* （分别*闭合*）*带原点的半线*$a \in F$。半线$\Delta_0$完全由$A$决定（因为对于$A$中的任何$b \neq a$来说，它是方向为向量$b - a$的半线），称为$A$的*方向*； $A$的方向向量也称为$A$的*方向向量*。

现在假设 E 在 K 上有 *有限* 维数 $n$ ；那么已知 (III, p. 518, Cor. 1) *n 个外部幂* $\Lambda^n E$ 是 K 上维数 1 的向量空间，因此是原点 0 的两条相对封闭半线的并。这些半线称为 E 的方向； 空间 E 与这些半线 A 中的给定一条一起被认为是有向的；如果 n 向量 z 属于到 A（或 -A），则在此方向下称为正（或负）；在相反的方向下它是负的（或正的）。

根据定义，仿射空间 F 在 K 上的方向是 F 平移空间的方向；空间 F 与这样的方向一起被称为有向仿射空间。

令 E 为 K 上的有向向量空间，且为维数 $n$；如果 n 向量 $a_1 a_2 \ldots a_n$ 为正（或为负），则 E 的有序基 $(a_i)_{1 \leq i \leq n}$ 称为正或直接（或为负或逆）。如果$u$是向量空间E的自同构，那么对于所有$z \in \bigwedge^n E$来说$(\bigwedge^n u)(z) = \det(u) \cdot z$，因此$\bigwedge^n u$的必要且充分的条件使E的方向保持不变（或者，正如我们也说的，保持方向）是$\det(u) > 0$；具有该性质的自同构恰好是 E 的自同构作为定向向量空间；它们形式是线性群$\mathrm{GL}(E)$的正常子群$\mathrm{GL}^+(E)$，只要$E \neq 0$就有指标2。

当$E = 0$时，$\mathrm{GL}(E) = \mathrm{End}(E)$包含仅恒等式映射1，并通过定义$\det(1_E) = 1$。请注意，在这种情况下，$\bigwedge^n E = \bigwedge^0 E = K$乘以定义；由正标量形成的 K 的半线称为零空间的规范方向。

设M和N分别为维数n的向量空间E中维数p和$n - p$的两个互补的子空间；如果$z'$（或$z''$）在$\bigwedge^p M$（或$\bigwedge^{n-p} N$）中为非零向量，则$z' \wedge z''$在$\bigwedge^n E$中为非零向量。给定 M 上的方向和 N 上的方向，向量 $z' \wedge z''$ 对于正 $z'$ 和 $z''$ 形式 E 的方向，称为 M 方向与 N 方向的乘积方向（当 $p(n-p)$ 时，这取决于因子的阶）奇数）。相反，给定 E 和 M 上的方向，N 上存在唯一的方向，使得 E 上的给定方向是 M 上给定方向和 N 上的该方向的乘积（即阶）；据说该方向与 M 相对于 E 的方向互补。如果 $N'$ 是 M 的第二个互补的子空间，则与 M 平行的规范投影 $N \to N'$ 会将 N 的互补方向取到 $N'$ 的互补方向。因此，规范映射 $N \to E/M$ 下 N 的互补方向的像独立于补体 N 的选择； E 的取向与 M 的取向称为 E/M 上的商取向。

习题

### 习题 {#alg-vi-s2-exercises}

所考虑的所有环均假定为可交换的除非，否则明确说明。

参见[习题为 § 2](exercises/s2/)。
