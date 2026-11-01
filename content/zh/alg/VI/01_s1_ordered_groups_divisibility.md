---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 1
section_title: Ordered groups. Divisibility
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0312-0330, 0341-0348
extraction: ocr
subsections:
    - "no": 1
      title: Definition of ordered monoids and groups
      page: 0
      pdf_page: 312
    - "no": 2
      title: Pre-ordered monoids and groups
      page: 3
      pdf_page: 314
    - "no": 3
      title: Positive elements
      page: 3
      pdf_page: 314
    - "no": 4
      title: Filtered groups
      page: 4
      pdf_page: 315
    - "no": 5
      title: Divisibility relations in a field
      page: 5
      pdf_page: 316
    - "no": 6
      title: Elementary operations on ordered groups
      page: 7
      pdf_page: 318
    - "no": 7
      title: Increasing homomorphisms of ordered groups
      page: 7
      pdf_page: 318
    - "no": 8
      title: Suprema and infima in an ordered group
      page: 8
      pdf_page: 319
    - "no": 9
      title: Lattice ordered groups
      page: 10
      pdf_page: 321
    - "no": 10
      title: The decomposition theorem
      page: 11
      pdf_page: 322
    - "no": 11
      title: Positive and negative parts
      page: 12
      pdf_page: 323
    - "no": 12
      title: Coprime elements
      page: 13
      pdf_page: 324
    - "no": 13
      title: Irreducible elements
      page: 17
      pdf_page: 328
statements: 53
exercises: 36
content_sha256: 7e9d41562b097d12327dcba95606d158c6af2dcba32b4633b37829600d0d5cb7
translated_from: content/en/alg/VI/01_s1_ordered_groups_divisibility.md
translation_method: google
source_content_sha256: 1339023eced66ef1b9e52222dbf004f549e42eec4f38ebac19c97f31df6e572b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7adcf5f66e8062143e4007b11a34816e0c97caa94ea7e02e42b0de0dcec3b04d
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。订购群。分割性

概念和截面中提出的结果涉及序关系在交换幺半群中的研究（I，p. 12，Def.2），最重要的情况是阿贝尔的群。 除非另有明确说明，我们将在所有群和正在研究的幺半群中对合成律使用加法记号。另一方面，随着我们的进展，我们将介绍有序群和幺半群理论的某些重要代数应用，并且我们将相应地将某些结果转换为适合这些应用的乘法记号。

### 1.有序幺半群的定义和群

#### 定义 1 {#alg-vi-s1-def-1 .statement tag=06WE}

— 一个可交换幺半群结构（写成加法）和集合$M$上的排序（写成$\leq$）被认为是兼容的，如果它们满足满足以下公理：

(OM) 对于每个$z \in M$，关系$x \leq y$意味着$x + z \leq y + z$。

集合$M$配备可交换幺半群结构和兼容的排序称为有序幺半群；如果它的交换幺半群结构是群结构，那么它被称为有序群。

以类似的方式，我们可以定义概念一个非交换有序幺半群（VI，p. 30，例 1）。

如果一个排序与给定的幺半群结构兼容，那么相反的排序也是如此。

#### 例 1 {#alg-vi-s1-n1-exa-1 .statement tag=06WF}

有理数整数的加法群和有理数数的群按照I，第21页和117页中定义的顺序排序。 *对于实数的加法群也是如此（Gen.Top.， IV，第 3 页）。 \*

#### 例 2 {#alg-vi-s1-n1-exa-2 .statement tag=06WG}

*在集合$E$上定义的有限数值函数的加法群是一个有序的群，其排序为“$f(x) \leq g(x)$对于所有$x \in E$”，写作$f \leq g$。这个关系表示函数$f$的图形位于函数$g$的图形下方。读者偶尔思考一下项这个图形解释可能会很方便。 \*

根据一般定义（集合理论，IV，p. 264），从有序幺半群M到有序幺半群M'的双射映射$f$称为M到M'的*同构*，如果M'的结构是通过沿 $f$ 传输 M 获得。这相当于说 $f$ 是映射 *onto* M'，这样

$$
f(x + y) = f(x) + f(y)
$$

（也就是说，幺半群M的同态到幺半群M'上），并且关系$x \leq y$和$f(x) \leq f(y)$是等价的（从而特别是$f(x) = f(y)$意味着$x = y$，即$f$是单射的）。

#### 命题 1（« 加法不等式 »）{#alg-vi-s1-prop-1 .statement tag=06WH}

— *在有序幺半群 M* 中，令 $(x_i)$ 和 $(y_i)$ ($1 \leq i \leq n$) 为 n 元素中的两个序列，使得 $x_i \leq y_i$ 对于所有 $i$；那么一个人有

$$
x_1 + \cdots + x_n \leq y_1 + \cdots + y_n
$$

*此外，如果所有元素 $x_i, y_i$ 均可取消（I、p. 15、默认 5）（特别是如果 M 为群），并且如果 $x_i < y_i$ 对于某些 $i$，则*

$$
x_1 + \cdots + x_n < y_1 + \cdots + y_n .
$$

一般情况约化乘归纳到情况$n = 2$，利用可取消的元素的和对于第二个断言可取消的事实（I，p. 15，提案2）。第一个断言源自关系

$$
x_1 + x_2 \leq x_1 + y_2 \quad \text{and} \quad x_1 + y_2 \leq y_1 + y_2 ,
$$

这是假设的推论和 (OM)。既然如此，关系

$$
x_1 + x_2 = y_1 + y_2
$$

会暗示

$$
x_1 + x_2 = x_1 + y_2 = y_1 + y_2 ,
$$

如果$x$和$y_2$可以取消，则从而$x_2 = y_2$和$x_1 = y_1$，这就证明了第二个断言。

#### 命题 2 {#alg-vi-s1-prop-2 .statement tag=06WI}

*在有序的群 G* 关系 $x \leq y$ *和* $x + z \leq y + z$ *等价*。

事实上，可以通过向两边添加 $z$ 或 $(-z)$ 来从对方获得每一个。

这个事实可以用说来表达，在有序的群 G 中，排序是*平移不变*。在其他字中，翻译是有序群的*排序*的*自同构*。

#### 推出 {#alg-vi-s1-n1-cor-1 .statement tag=06WJ}

— 在有序的群 $G$、关系 $x \leq y$、$0 \leq y - x$、$x - y \leq 0$ 和 $-y \leq -x$ 等价。

事实上，我们应用命题2，依次取$z = -x$、$z = -y$和$z = -(x + y)$。

特别是，我们从这个推论中推断出，如果$G$是有序的群，则从$G$到自身的映射$x \mapsto -x$将$G$的顺序改为相反的顺序。

### 2. 预购幺半群和群

回想一下，如果集合$E$的元素之间的关系$x \leq y$是自反且传递的，则称为先序关系（集合理论，III，p. 133）。 关系 « $x \leq y$ 和 $y \leq x$ » 是 $E$ 上的等价关系 $S$，与关系 $x \leq y$ 相容的；在经过上求商，在 $E/S$ 上关系 $\leq$ 诱导序关系，称为与 $\leq$ 关联的序关系。

#### 定义 2 {#alg-vi-s1-def-2 .statement tag=06WK}

— 集合 $M$ 上的前序关系（写为 $\leq$）和可交换幺半群结构（写为加法）如果满足满足以下公理，则称它们是兼容的：

(POM) 对于每个 $z \in M$，关系 $x \leq y$ 意味着 $x + z \leq y + z$。

集合$M$配备了可交换幺半群结构和兼容的先序关系称为先序幺半群。

令 $M$ 为预定幺半群，$S$ 等价关系 « $x \leq y$ 和 $y \leq x$ »。根据(POM) 关系 $x \equiv x' \pmod{S}$，对于所有$y \in M$，意味着$x + y \leq x' + y$和$x' + y \leq x + y$，即$x + y \equiv x' + y \pmod{S}$。在其他字等价关系$S$与$M$（I，p. 11）中的加法兼容。因此，加法律在 $M$ 上除以 $S$ 的商，以及与 $\leq$ 相关的排序，给出有序幺半群的 $M/S$ 结构。在 $M$ 是预购的群的情况下，群 $M/S$ 是所有元素 $x$ $M$ 除以子群由……组成的商，使得 $x \leq 0$ 和$0 \leq x$。

### 3.积极元素

令$G$为已预订的群，具有前序关系$\leq$；如果$0 \leq x$和$0 \leq y$，那么我们通过（POM）推导出$y \leq x + y$，因此通过传递性推导出$0 \leq x + y$；这表示元素$x \in G$的集合$G_+$使得$0 \leq x$在加法下闭合；而且，关系$x \leq y$相当于$0 \leq y - x$，即$y - x \in G_+$。反之：

#### 命题 3 {#alg-vi-s1-prop-3 .statement tag=06WL}

— 如果$P$是阿贝尔的群$G$、包含$0$的子集且$P + P \subset P$，则关系$y - x \in P$是兼容的前序关系群结构共 $G$。为了使关系使$G$成为有序的群，有$P \cap (-P) = \{0\}$是必要且充分的；在此排序下，要使$G$成为全序群，加法$P \cup (-P) = G$是必要且充分的。

关系 $y - x \in P$是自反且及物的，并且（如果写成$x \leq y$）满足公理*POM*，这是直接的。 为了证明第二个断言，注足以证明$P \cap (-P)$是子群$G'$由……组成元素$x$，使得$0 \leq x$和$x \leq 0$。 最后，说$G$是完全有序的意味着，对于$G$的元素$x, y$中的每个对，至少有元素$x - y, y - x$属于到$P$之一，从而完成证明。

#### 定义 3 {#alg-vi-s1-def-3 .statement tag=06WM}

*在有序群 $G$ 中，任何元素 $x$ 使得 $0 \leq x$（或$x \leq 0$）称为正（或负）元素。*

注 $0$ 是唯一的元素 *既是正数又是负数* ；任何元素$x$使得$0 < x$（或$x < 0$）被称为*严格正数*（或*严格负数*）。

#### 例 {#alg-vi-s1-n3-exa-1 .statement tag=06WN}

— 在加法群 $\mathbf{Z} \times \mathbf{Z}$ 中，令 $P$ 为元素 $(x, y)$ 满足两个不等式 $ax + by \geq 0$ 和 $cx + dy \geq 0$ 的集合，其中 $a, b, c, d$ 为整数（* 或实数 *) 使得 $ad - bc \neq 0$; «锥体»$P$满足命题3的前两个条件，这样就可以定义与$\mathbf{Z} \times \mathbf{Z}$的群结构兼容的各种排序； 群在任何这些排序下都不是完全排序的。

#### 注 {#alg-vi-s1-n3-rem-1 .statement tag=06WO}

— 凭借条件 $P + P \subset P$，有序群中的关系 $x \geq 0$ 意味着对于每个自然数 $n$ 都有 $nx \geq 0$。若加法中$G$的正值元素$x$有有限阶$n$，则$-x = (n-1)x$为正；自从

$$
P \cap (-P) = \{0\},
$$

这意味着$x = 0$。特别是，如果$G$的每个元素都有有限的阶，则$P = \{0\}$； 关系 $x \leq y$ 等价于$x = y$（*离散*排序）。

### 4. 过滤群

回想一下（*集合理论*，III，p. 145），如果对于$G$的元素的每个对$(x, y)$，有序的集合$G$是*右*（分别是*左*）*过滤*\脚注{1}存在$z \in G$使得$x \leq z$和$y \leq z$（分别为$z \leq x$和$z \leq y$）。每个右过滤有序群 $G$ 也被左过滤，反之亦然：事实上，由于存在 $z \in G$ 使得 $-x \leq z$ 和 $-y \leq z$，我们有 $-z \leq x$ 和 $-z \leq y$（VI，p. 3，Cor.）。因此，我们将简单地讨论过滤后的群。

#### 命题 4 {#alg-vi-s1-prop-4 .statement tag=06WP}

*对于要过滤的有序群$G$，它由其正元素生成是必要且充分的，即每个元素都是两个正元素的差。*

事实上，如果$G$被过滤，那么对于每个$x \in G$，都存在一个正的元素$z$，使得$x \leq z$，而$x$是两个正的元素$z$和$z - x$的差。相反，如果$x = u - v$和$y = w - t$且$u, v, w, t$为正，则元素$u + w$大于$x$且大于$y$。

1 术语用于*loc。 cit.* 是*定向*。

#### 命题 5 {#alg-vi-s1-prop-5 .statement tag=06WQ}

— *如果* $(x_i)$ *是过滤后的群 G 的元素的有限族，则存在* $z \in G$ *使得* $x_i + z$ *对于每个 i 都是正数。*

*如果* $x_i = u_i - v_i$，*与* $u_i$ *和* $v_i$ *为正，则足以将* $z$ *成为家庭的和* $(v_i)$。

### 5. 关系能被域整除

这里我们将定义某些有序的群，它在代数中起着重要的部分的作用。 记号通常用于这些群是乘法；因此，将之前在加法记号中获得的结果应用到这些群中，就以翻译为乘法记号为前提——这对读者来说不会有任何困难。 *在整个截面中，字母A代表整环，K代表分数*的域（*l*，p. 116）。

在$\mathbf{K}$的非零元素的乘法群$\mathbf{K}^*$中，A的非零元素的集合P在乘法下闭合，因为A是环。因此，定义是$\mathbf{K}^*$上$x^{-1}y \in P$的先序关系，即“存在$z \in P$使得$y = zx$”，这使得$\mathbf{K}^*$*预先排序群*（乘法写）（*VI*， p. 3，提案 3）。将与 A (I, p. 97) 的元素相关的术语扩展到$\mathbf{K}^*$、关系$x^{-1}y \in P$也可以表示为： *x 除 y*，或 x 是 y* 的 *除子，或y 是 x* 的 *倍数（相对于环 A）；我们将关系 $x^{-1}y \in P$ 称为 $\mathbf{K}^*$ 相对于环 A 的 *整除性关系*。 关系 « x '除 y » 表示为 $x \mid y$，其否定$x \nmid y$。 P 的元素正是 1* 的 *倍数。

#### 注 1 {#alg-vi-s1-n5-rem-1 .statement tag=06WR}

$\mathbf{K}^*$中的关系在本质上取决于特定的环A。如果$A = K$我们得到“平凡”关系，其中$x \mid y$对于元素的每个对$(x, y)$ $\mathbf{K}^*$。设 p 和 q 为素数数；有理数数 r/s，其分母不是 $p$（或 q）形式子环 $\mathbf{Z}_{(p)}$（或 $\mathbf{Z}_{(q)}$）或 $\mathbf{Q}$ 的倍数；如果 $p \neq q$、数 $p/q$ 在一个关系下倍数为 1 而在另一个关系下不为 1，则 $\mathbf{Q}^*$ 中的关系相对于这两个环的整除性是不同的。

#### 注 2 {#alg-vi-s1-n5-rem-2 .statement tag=06WS}

我们将关系$x \mid y$有时扩展定义到$\mathbf{K}$元素对（而不仅仅是$\mathbf{K}^*$），这个关系被认为是“那里”存在 $z \in A$ 使得 $y = zx$ »;因此，我们将为所有 $x \in K$ 提供 $x \mid 0$。这允许我们在没有限制的情况下陈述以下结果：如果 $x \mid y$ 和 $x \mid z$ 那么 $x \mid (y - z)$；如果$x \mid y$和$x \nmid z$则$x \nmid (y - z)$。以同样的方式，我们可以扩展所有相应的术语。

为了从关系整除性中获得 *序关系* (No. 2)，我们必须将元素 $x \in \mathbf{K}^*$ 的子群 $\mathbf{A}^*$ 传递到 $\mathbf{K}^*$ 的商群，使得 $x \mid 1$ 和 $1 \mid x$；这些是 P 的元素，它们是 1* 的 *除子，也就是说 $A$ 的*可逆* 元素；由于滥用语言，它们通常被称为单位或环 A。 商群 $\mathbf{K}^*/\mathbf{A}^*$ 则为有序的群。 $\mathbf{K}^*$的两个元素$x$和$y$，其中属于与$\mathbf{A}^*$的同一个陪集被称为*关联*；这意味着$x \mid y$和$y \mid x$。另一方面，如果 x 除 y 没有 y 除 x，我们说 x 严格除 y，或者 x 是 y 的严格除子，或者 y 是 x 的严格倍数。

注 $K^*/A^*$ 是一个*过滤* 群，因为 K 是 A 的分数的域（VI，p. 4，命题 4）。

说 $K^*$ 的两个元素 x 和 y 是关联相当于说，它们在 K 中具有*相同*相同的倍数，凭借关系的整除性传递性。对于所有$x \in K$，我们将用$z \in A$的所有元素zx中的$Ax$集合来表示； 集合$Ax$是K的子模视为A-模。扩展术语与$x \in A$的情况相关，我们将其称为域 K相对于环 A的主分数理想。相反，环 A的理想被认为是积分的。

注如果$A \neq K$，则主分数理想$\neq \{0\}$ 不是被视为环的 K 理想。

主分数理想 $Ax$ 也表示为 (x)。我们将$x \in Ay$写为$x \equiv 0$（mody），为$x - x' \in Ay$写为$x \equiv x'$（mody）；如果 $x \equiv x'$ (mody) 那么 $zx \equiv zx'$ (mod $zy$) 对于任何$z \in K$。

注 $x \equiv x'$ (mod y) 并不意味着 $zx \equiv zx'$ (mod y) 除非 $z \in A$。因此，在$\mathbf{Q}$中，相对于$\mathbf{Z}$，我们有$4 \equiv 2$（mod 2），但没有$2 \equiv 1$（mod 2）。

关系 $x | y$ 显然等价于$(x) \supset (y)$。 映射$x \mapsto (x)$从$K^*$到K的主分数理想$\neq (0)$的集合$\mathscr{P}^*$，因此定义，在经过到商，双射映射从$K^*/A^*$ 到$\mathscr{P}^*$；通过这个映射将$K^*/A^*$的群结构翻译成$\mathscr{P}^*$，我们得到两个主分数理想(x)和(y)的定义乘积是理想(xy)，它仅取决于(x)和(y)。有了这个律和序关系$(x) \supset (y)$，集合$\mathscr{P}^*$就是一个有序的群，与$K^*/A^*$同构的。按照惯例，我们将通过上面的映射来认同 $\mathscr{P}^*$ 与 $K^*/A^*$。

注关系 « x 除 y »，在正整数的情况下，意味着 x 小于 y，对应包含 $(x) \supset (y)$，其中理想 (x) “大于”理想 (y)。我们可以通过注意到例 7 比 91 具有更多的倍数 »来记住这个“阶反转”。

如果我们对 K 的所有元素扩展关系 $x | y$，这个关系仍然等价于 K 的所有主分式理想的集合 $\mathscr{P}$ 中的$(x) \supset (y)$（其中 $(0)$ 是包含关系下的最小的元素）。

与之前的截面一样，我们通常会在续集中使用加法记号。然而，与整除性相关的术语将在相应的加法术语之后引入，在符号（DIV）之前的段落中（其中所使用的记号是现在的截面）。在阶中，为了使读者的任务更容易，某些结果将被翻译成整除性的语言，即第7号提案的翻译，对于例，被表示为“命题7（DIV）”。

### 6. 订购群时的基本运算

令 H 为有序群 G 的子群；显然，G 的排序限制与 H 的群结构是兼容的；我们总是以这种方式订购H，否则除非。如果 P 是 G 的正元素的集合，则 H 的正元素的集合是 H ∩ P。

设$(G_\alpha)$是群的有序族；根据有序集乘积定义（集合理论，III，p. 137）乘积群G=$\prod G_\alpha$配备排序，关系《$(x_\alpha) \leq (y_\alpha)$》之间的两个G 的元素通过定义与 « $x_\alpha \leq y_\alpha$ 对于所有 α » 相同。该排序与G的群结构兼容为直接的；这种排序使 G 成为有序群，我们将其称为有序群 $G_\alpha$ 的乘积。 G 的正元素是那些元素所有分量都为正的。在所有因子 $G_\alpha$ 与相同有序群 H 相同的情况下，则 G 是映射的群 H'，从指标集合 I 转换为 H，关系 « f ≤ g » 介于两个之间从 I 到 H 的映射与所有 α ε I 的 « f(α) ≤ g(α) 相同 »；正映射是那些只取正值的值。有序群的族$(G_\alpha)$的直和被定义为其乘积（II，p. 202）的有序子群。

令 $(G_i)_{i \in I}$ 为有序群的族，其中指标集合 I 是良序的：回想一下（集合理论，III，p. 157）序关系，称为词典顺序，是在乘积上定义的集合 G = $\prod G_i$, 关系 « $(x_i) < (y_i)$ » 在 G 的两个元素之间通过定义与 « 如果 β 是指标 i 的最小的使得 x_i ≠ y_i，则 x_β < y_β » 相同。回想一下，全序集的良序族中的乘积是按照字典顺序完全有序的。一般情况下，G 上的字典顺序与其群结构兼容，这一点立即得到验证；配备此排序，群 G 因此是有序的群，称为有序群 $(G_i)$ 良序族的词典乘积。

#### 注 1 {#alg-vi-s1-n6-rem-1 .statement tag=06WT}

在最常见的情况下，良序指标集合 I 将是 N 中的有限区间 (1, n)。

#### 注 2 {#alg-vi-s1-n6-rem-2 .statement tag=06WU}

词典乘积 G 的正元素的集合由0和那些至少指标的非零的分量为正的非零元素组成。

### 7. 已订购群的递增同态

令 G 和 G' 为二阶群；在从 G 的底层加法群到 G' 的同态 f 中，考虑递增映射是有意义的，即 x ≤ y 意味着 f(x) ≤ f(y)。由于关系 $f(y - x) = f(y) - f(x)$，因此从 G 到 G' 的递增同态的特征在于，在这样的同态下，G 的正元素的像是 G' 的正元素；如果 P（分别为 P'）表示 G（分别为 G'）的正元素的集合，则可以写为 $f(P) \subset P'$。很明显，将子群 G 的典范嵌入放入有序的群 G'，以及将群的乘积的投影有序放入其因子之一，是递增同态。

同构 (VI, p. 2) $f$ 从有序群 G 到有序群 G' 是从 G 到 G' 的双射同态，使得 $f$ 和逆同态都是递增，在其他情况下字$f(P) = P'$。

可能发生的是，从 G 的底层群到 G' 的底层群的同构可以是递增，而逆同构也不是递增。情况就是这样，对于例，如果$G = G'$，如果$f$是G上的恒等式映射，并且如果$P \subset P'$但是$P \neq P'$。因此，在$\mathbf{Z}$中，我们可以将$P'$视为（普通）正整数的集合，并将P视为偶数正整数的集合。

(DIV) 令 K 为有理数函数 $F_2(X)$ 的域超过阶的域 $F_2$ 2. 关系相对于环 $F_2[X] = A'$ 和 $F_2[X^2, X^3] = A$ 定义两个不同有序群结构在$K^*$上，这样$A \subset A'$（它们被排序为群结构，因为1是A中唯一的单位，也是A'中唯一的单位）。

### 8. 有序群中的 Suprema 和 infima

回想一下（集合理论，III，p. 141），如果有序集合E的子集F的上界集合（也就是说$z \in E$的集合使得$x \leq z$对于所有$x \in F$) 至少有元素 a，那么这个唯一的元素称为 F 的上界。如果 F 是 E 的元素的$(x_i)_i$族中元素的集合，则其上界（如果存在）表示为$\sup x_i$（或$\sup x_i$或简单地$\sup(x_i)$）；如果它是有限族$(x_i)$ ($1 \leq i \leq n$)，则该上界也表示为$\sup_{\text{LEI}} (x_1, \ldots, x_n)$。下确界以类似的方式定义并表示为 inf。 运算sup 和 inf 是结合律和交换律。

回想一下（集合理论，前述），如果F是有序集合E的子集，并且$(x_i)$F的元素族，那么E中$\sup(x_i)$的存在（可以表示为$\sup_E(x_i)$）并不意味着存在F 中的$x_i$（当存在时可以表示为$\sup_F(x_i)$）；如果两者都存在，我们只知道 $\sup_E(x_i) \leq \sup_F(x_i)$；然而，如果 $\sup_E(x_i)$ 存在且属于为 F，则 $\sup_F(x_i)$ 存在且等于 $\sup_E(x_i)$。对于例，在多项式环 $A = K[X, Y]$ (K 域) 中，主理想 AX 和 AY 在 A 的理想有序集合中以理想 $AX + AY$ 作为上界（在关系 $\subset$ 之下），但以理想 A 作为上界在 A 的所有主要理想的集合中。

(DIV) $K^*$ 的元素 d 称为最大的公共的除子，简称 gcd，对于 $K^*$ 的元素族$(x_i)$，如果主分数理想 (d) 是 $\mathscr{P}^*$ 中的上界（在理想族$((x_i))$的关系$\subset$），或者在其他字中，如果$z \in K^*$的关系$z \mid d$相当于“所有$i$的$z \mid x_i$”。 In the same way we will say that $m \in K^*$ is a least common multiple or an lcm of the family $(x_i)$ if $(m)$ is the infimum in $\mathscr{P}^*$ of the family of ideals $((x_i))$, that is if m | z is equivalent to « x_i | z for all i ». 说 $(m) = \cap_{i} (x_i)$ 相当于同样的事情；事实上，条件$x_i | z$对于所有$i$相当于$z \in A x$，对于所有$i$，即$z \in \cap_{i} (x_i)$，条件$m | z$相当于$z \in (m)^1$。

注如果主分数理想 (d) 满足$(d) = \sum (x_i)$，则 d 是$(x_i)$族的 gcd；但相反，$(x_i)$的gcd不一定是满足上面的条件（cf.VI，p. 33，例24）。

gcd 和 lcm（如果存在）是明确定义的模子群 U 的单位的 $K^*$，即给定族的两个 gcd（或两个 lcm）是关联的；通过滥用语言，我们经常会为 $(x_i)$ 家族的任何 gcd 或 lcm 编写 gcd$(x_i)$ 和 lcm$(x_i)$，只要存在这样的元素 。

(DIV) 通过滥用语言，我们将gcd的有时扩展概念给一个家庭$(x_i)$元素K，其中一些可能是零；该 gcd 再次定义为元素 d，使得关系 $z | d$ 相当于所有 $i$ 的“$z | x_i$”；显然，如果所有 $x_i$ 都是零 ，则 d 为 0；否则 d 是非零的 $x_i$ 的 gcd。同样，一个族的 lcm（其中一些元素是零）为 0。

在有序群 G 中，在排序转换下不变性的直接的推论（VI，p. 2，命题 2）是：

(1)
$$
\sup(z + x_i) = z + \sup(x_i)
$$
从某种意义上说，每当一侧被定义时，另一侧也被定义，并且两者是相等的。类似地，从映射$x \mapsto -x$将G的顺序取为相反的顺序（VI，p. 3，Cor.）这一事实得出结论

(2)
$$
\inf(-x_i) = -(\sup(x_i)),
$$
这个关系与前一个的含义相同。

#### 命题 6 {#alg-vi-s1-prop-6 .statement tag=06WV}

— 令 $(x_i)_{i \in A}, (y_\beta)_{\beta \in B}$ 为有序群 G 的元素的两个族，每个族都有一个上界。那么家族$(x_\alpha + y_\beta)_{(\alpha, \beta) \in A \times B}$有一个至高点，并且
$$
\sup_{(\alpha, \beta) \in A \times B} (x_\alpha + y_\beta) = \sup_{\alpha \in A} x_\alpha + \sup_{\beta \in B} y_\beta.
$$
事实上，从所有$\alpha$和$\beta$的$x_\alpha + y_\beta \leq z$，我们推导出所有$\beta$的$\sup(x_i) + \sup(y_\beta) \leq z$，从而推导出$\sup(x_i) + \sup(y_\beta) \leq z$。

1 当 A 是整数的环（分别是多项式环，系数在域中）时，这些定义重合与 I、p. 112（分别是 IV、p. 12、Def.） 1）。

### 9. 格子有序群

回想一下，有序集合，其中每个非空有限子集都有上界和下确界，称为格 (E, III, p. 13)。显然，群晶格有序的乘积，特别是全序群的乘积，是群晶格有序。相反，晶格有序群的子群不一定是晶格有序的。

因此，在乘积有序群$Z \times Z$中，“反对角”（对$(n, n')$的集合，使得$n + n' = 0$）以离散排序进行排序，因此不是网格有序群。 *一个实数变量中多项式的加法群（VI、p. 1、例 2）是经过过滤的群（因为$p(x)$和$q(x)$都小于$(p(x))^2 + (q(x))^2 + 1$），可以证明它不是格序的。 \*

#### 命题 7 {#alg-vi-s1-prop-7 .statement tag=06WW}

— *如果 x 和 y 是有序群 G 的两个元素，并且如果元素 $\inf(x, y)$、$\sup(x, y)$ 之一存在，则另一个也存在，$x + y = \inf(x, y) - \sup(x, y)$ 也存在。

事实上，根据关系 (1) 和 (2) (VI, p. 9) 我们有

$$
\sup(a - x, a - y) = a + \sup(-x, -y) = a - \inf(x, y),
$$

取$a = x + y$就足够了。

#### 命题 7 {#alg-vi-s1-div-prop-7 .statement tag=06WX}

— *如果$a, b \in K^*$，并且如果 d 是 a 和 b 的 gcd，并且 m 是 a 和 b 的 lcm，则乘积 dm 是 ab 的关联。

#### 命题 8 {#alg-vi-s1-prop-8 .statement tag=06WY}

— *令 P 为有序群 G 的正元素的集合。 对于 G 是晶格有序的，$G = P - P$ 以及加法 P 中的加法 P（配备诱导排序）满足以下条件中的一个或其他是必要且充分的：

a) P 的元素的每个对在P中都有一个上界。
b) P 的元素中的每个对在 P 中都有一个下确界。

这些条件的必要性是显而易见的：确实关系$G = P - P$说G被过滤了（VI，p. 4，命题4）；另一方面，P 的两个元素的上界和下确界 *in* G 是正的，它们在 P 中的上界和下确界也是正的。

相反，注首先，在假设 a) (resp. b)) 下，P 的元素 x, y 的每个对都有一个上界 (resp. infimum) *in* G 等于其上界 a (resp. infimum b) *in* P。这对于 a 来说是显而易见的，因为任何上界 x 和 y 为正；对于 b，令 x 和 y 的 $z \in G$ 为下界；那么存在$u \in P$使得$z + u \in P$，因为$G = P - P$；现在 $\inf_P(x + u, y + u)$ 大于 $b + u$，形式 $b + c + u$ ($c \geq 0$)；因为 $b + c$ 小于 x 且小于 y，所以我们有 $c = 0$；因此$\inf_P(x + u, y + u) = b + u$，这意味着$z + u \leq b + u$，因此$z \leq b$和b肯定是G中x和y的下确界。现在，如果x和y是G的任意元素，我们将它们转换为P：令$v \in P$使得$x + v$和$y + v$为正（VI，p. 5，提案 5）；在假设 a) (resp. b)) 下，$P$ 中存在 $x + v$ 和 $y + v$ 的上确界（resp. 下确界），因此根据我们刚才所见，在 $G$ 中也存在；通过翻译，$x$和$y$在$G$有一个上确界（分别为下确界）；根据命题 7，其中一个的存在意味着另一个，这表明条件是充分的。

### 10.分解定理

#### 定理 1 (分解定理) {#alg-vi-s1-thm-1 .statement tag=06WZ}

— *设* $(x_i)_{1 \leq i \leq p}$ *和* $(y_j)_{1 \leq j \leq q}$ *为群* $G$ *的正元素的两个有限序列 *这样* $$
\sum_{i=1}^p x_i = \sum_{j=1}^q y_j ;
$$ *则存在双序列* $(z_{ij})_{1 \leq i \leq p, 1 \leq j \leq q}$ *正元素*$G$*使得*$x_i = \sum_{j=1}^q z_{ij}$*对于所有*$i$，*和*$y_j = \sum_{i=1}^p z_{ij}$*对于所有*$j$。

1) 让我们首先针对$p = q = 2$的情况证明定理。令$x, x', y, y'$为$G$的正元素，使得$x + x' = y + y'$，并放入$a = \sup(0, x - y')$。自从
$$
x - y' = y - x'
$$
小于$x$且小于$y$，则$b = x - a$和$c = y - a$为正，$d = a - (x - y')$亦然。我们还有
$$
x = a + b, \quad x' = c + d, \quad y = a + c \quad \text{and} \quad y' = b + d .
$$

2) 现在让我们证明，如果 $p < m$ 和 $q = n$ ($m > 2,\ n \geq 2$) 定理为真，那么$p = m$ 和 $q = n$ 也为真。到假设，我们就有了$x, + \sum_{i=1}^{m-1} x_i = \sum_{j=1}^n y_j$。 定理对于$p = 2$和$q = n$成立，$n$正项存在两个有限序列$(z_j'), (z_j'')$，使得对于$1 \leq j \leq n$有$\sum_{i=1}^{m-1} x_i = \sum_{j=1}^n z_j'$、$x_m = \sum_{j=1}^n z_j''$和$y_j = z_j' + z_j''$。另一方面，由于定理对于$p = m - 1$和$q = n$成立，因此存在双序列$(u_{ij})_{1 \leq i \leq m-1, 1 \leq j \leq n}$，使得$x_i = \sum_{j=1}^n u_{ij}$对于$1 \leq i \leq m - 1$，以及$z_j' = \sum_{i=1}^{m-1} u_{ij}$对于$1 \leq j \leq n$。推杆
$$
z_{ij} = u_{ij} \quad \text{for} \quad 1 \leq i \leq m - 1 , \quad \text{and} \quad z_{mj} = z_j'' \quad (1 \leq j \leq n) ,
$$
我们当然得到定理的双序列满足条件。

3）通过交换、$x_i$和$y_j$，我们以同样的方式看到，如果定理对于$p = m$和$q < n$（$m \geq 2,\ n > 2$）为真，那么对于$p = m$和$q = n$也为真。因此，定理由双归纳从情况$p = q = 2$开始证明，因为每当$p \leq 1$或$q \leq 1$时它都是平凡的真。

#### 推论 {#alg-vi-s1-n10-cor-1 .statement tag=06X0}

— 令 $y, x_1, x_2, \ldots, x_n$ 为 $n + 1$ $G$ 的正元素，使得 $y \leq \sum_{i=1}^n x_i$；则存在$n$正元素$y_i$($1 \leq i \leq n$)使得$y_i \leq x_i$和$y = \sum_{i=1}^n y_i$。

元素$y$和$z = \left( \sum_{i=1}^n x_i \right) - y$两个中的应用定理1至序列$(x_i)$和序列由……组成就足够了。

### 11.正负部分

#### 定义 4 {#alg-vi-s1-def-4 .statement tag=06X1}

— 在群$G$有序的格子中，元素$x \in G$的正部分（或负部分，绝对值）为元素$\sup(x, 0)$（或$\sup(-x, 0)$， $\sup(x, -x)$），表示为$x^+$（分别为$x^-$、$|x|$）。

尽管有它的名字，负数部分 $x^-$ 是正数元素。

显然是$x^- = (-x)^+$和$|-x| = |x|$。让我们也注下面的公式，其中第一个是定义的直接的推论以及翻译下的顺序不变性，第二个是从第一个VI、p. 10的第7条命题得出的：

$$
\begin{cases}
\sup(x, y) = x + (y - x)^+ \\
\inf(x, y) = y - (y - x)^+
\end{cases}
$$

#### 命题 9 {#alg-vi-s1-prop-9 .statement tag=06X2}

— a) 对于有序群 $G$ 的每个元素 $x$，我们有 $x = x^+ - x^-$ 和 $\inf(x^+, x^-) = 0$。

b) 对于作为两个正数元素之差的$x$的每个表达式，例如$x = u - v$，我们有$u = x^+ + w$和$v = x^- + w$以及$w = \inf(u, v)$。特别是如果$\inf(u, v) = 0$则$u = x^+$和$v = x^-$。

c) 关系 « $x \leq y$ » 相当于 « $x^+ \leq y^+$ 和 $x^- \geq y^-$ »。

d) 我们有$|x| = x^+ + x^- \geq 0$。

e) For any $x$ and $y$ in $G$, we have the inequality $|x + y| \leq |x| + |y|$, and more generally $\left| \sum_{i=1}^n x_i \right| \leq \sum_{i=1}^n |x_i|$ for any finite family $(x_i)$ of elements of $G$.

f) 对于$G$中的任何$x$和$y$，我们有$||x| - |y|| \leq |x - y|$。

我们将同时证明a）和b）。如果 $x = u - v$ 且 $u$ 和 $v$ 为正，则 $u$ $x$，因此 $u \geq \sup(x, 0) = x^+$ 和 $w = u - x^+$ 为正。另一方面我们有

$$
x^+ - x = \sup(x, 0) - x = \sup(x - x, -x) = x
$$

由此得出$x = x^+ - x^-$和$v - x^- = w$。如果$z \leq x^-$则$z \leq x^+ - x$，依此类推$x \leq x^+ - z$；如果也$z \leq x^+$，则$x^z - z$为正，因此$x^i \leq x^+ - z$乘以$x^i$的定义。因此我们有$z \leq 0$，这意味着$\inf(x^+, x^-) = 0$，通过翻译$\inf(u, v) = w$意味着从而。

c) 关系$x \leq y$意味着$\sup(y, 0) \geq x$和$\sup(y, 0) \geq 0$，因此$x^i \leq y^i$；类似地，如果$-y \leq -x$我们推导出$x^- \geq y^-$。 逆命题含义紧接着$x = x^+ - x$ 和$y = y^+ - y$。

d) 由于$x \leq x^+$和$-x \leq x^-$，显然
$$
|x| = \sup(x, -x) \leq x^+ + x
$$
相反，如果$a \geq x$和$a \geq -x$，那么我们从c)推导出$a^+ \geq x^+$、$a^+ \geq x^-$、$a^- \leq x^-$和$a^- \leq x^+$；由于$a^-$为正且$\inf(x^i, x^-) = 0$，最后两个不等式意味着$a^- = 0$和$a = a^+$；前两个不等式给出 $a \geq \sup(x^+, x^-)$，并且根据 a) 和VI、p. 10 的第 7 条命题，$\sup(x^+, x^-)$ 等于 $x^+ + x^-$。

e) 从$x$和$y$到$|x|$和$y$，我们有$x + y \leq |x| + |y|$；从$-x \leq |x|$和$-y \leq |y|$开始，我们有$-x - y \leq |x| + |y|$； 从而第一个不等式。第二个跟随在 n 上的归纳。

f) 替换 x 和 y 通过 e) 中的 y 和 x - y，我们得到
$$
|x| - |y| \leq |x - y|
$$
同样，我们有 $|y| - |x| \leq |y - x| = |x - y|$； 从而所规定的结果。

#### 注 {#alg-vi-s1-n11-rem-1 .statement tag=06X3}

我们从 d) 推论出 $|x| = 0$ 蕴涵$x = 0$（因为 $x^+$ 和 $x^-$ 是正数）；因此$x \neq 0$意味着$|x| > 0$。

#### 命题 9 {#alg-vi-s1-div-prop-9 .statement tag=06X4}

— 如果 K 的主分数理想群 $\mathscr{P}^*$ 是格序的，则 $K^*$ 的每个元素 x 都可以写成形式 $x = uv^{-1}$，其中 u 和 v 是 A 的元素，使得 $1 = \gcd(u, v)$；对于 x 的任何其他表达式 $x = u'{v'}^{-1}$ 作为 A 的两个元素的商，我们有 $u' = uw$ 和 $v' = vw$，其中 w 是 $u', v'$ 的 gcd；特别是如果 $1 = \gcd(u', v')$ 那么 u' 和 v' 分别是 u 和 v 的关联。

$K^*$ 的元素 x 的这种表达式$uv^{-1}$ 通常称为约化分数。

### 12.Coprime 元素

#### 定义 5 {#alg-vi-s1-def-5 .statement tag=06X5}

— 在有序群中，如果 $\inf(x, y) = 0$，则两个元素 x 和 y 称为互质。

在某些情况下，如果$\inf(|x|, |y|) = 0$（cf. INT，II, § 1），定义两个元素互质，或者在整除理论中引入相应的术语，这是很自然的。我们不会在这里这样做。

两个互质元素必然是正数。 x 的正负部分 $x^+$ 和 $x^-$ 互质（VI，p. 12，命题 9，a））。一个家庭 $(x_i)_{i \in I}$ 的元素 $x_i$ 被认为是 *setwise coprime* if $\inf_{i \in I} x_i = 0$;如果$x_i$都是$\geq 0$，那么存在I的有限子集J就足够了，使得相应的元素是集合互质的。如果$\inf(x_i, x_j) = 0$对于不同指标的每个对$(\ell, \kappa)$，则称家庭$(x_i)$的元素是“成对互质”。

$x_i$ 可以是集合互质而不是成对互质。

如果 x 和 y 互质，我们也说 x 与 y 互质，或者 y 与 X 互质

(DIV) 如果主理想 (x) 和 (y) 为非零的并且在 $\mathscr{P}^*$ 中互质，则称 K 的两个元素 x 和 y 为*互质*；这等于说，1 是 x 和 y 的 gcd，并且意味着 x 和 y *属于* 到 A。对于例，约简分数的分子和分母是互质的。成对和集合互质元素的概念定义类似。

(DIV) 当 x 和 y 互质时，它们通常被称为“与 1 互质另一个”；避免这个术语很方便，这可能会导致与素数数的概念混淆（I，p. 50，Def. 16）。

#### 命题 10 {#alg-vi-s1-prop-10 .statement tag=06X6}

*设 x、y 和 z 为有序群的三个元素；对于 x – z 和 y – z 互质，z = inf (x, y).* 是充分必要的

事实上关系 $z = \inf(x, y)$ 和 $0 = \inf(x - z, y - z)$ 是等价的。

**命题 10 (DIV).** — *令 a、b 和 c 为 K 的三个元素，其中 c $\neq 0$；为了使商 $ac^{-1}$ 和 $bc^{-1}$ 互质，c 是 a 和 b 的 gcd 是充分必要的。*

#### 命题 11 {#alg-vi-s1-prop-11 .statement tag=06X7}

*如果$(x_i), (y_j)$是群有序晶格的正元素的两个有限族，那么*

$$
\inf \left( \sum_i x_i, \sum_j y_j \right) \leq \sum_{i,j} \inf(x_i, y_j)
$$

在$(x_i)$和$(y_j)$族中，通过归纳对元素的数进行论证，足以证明，如果x、y和z为正元素，则

$$
\inf(x, y + z) \leq \inf(x, y) + \inf(x, z).
$$

确实，放入$t = \inf(x, y + z)$；由VI，p. 12，Cor.，我们可以用$0 \leq t_1 \leq y$和$0 \leq t_2 \leq z$写出$t = t_1 + t_2$；由于$t_1$和$t_2$是正数，我们还有$t_1 \leq x$和$t_2 \leq x$，从而$t_1 \leq \inf(x, y)$和$t_2 \leq \inf(x, z)$。

#### 推论 1 {#alg-vi-s1-prop-11-cor-1 .statement tag=06X8}

*如果 x 和 y 是两个互质元素，并且 z 是一个正元素，属于群晶格有序，则 $\inf(x, z) = \inf(x, y + z)$。*

事实上，第11号提案的$\inf(x, y + z) \leq \inf(x, z)$，以及自$y \geq 0$以来的$\inf(x, z) \leq \inf(x, y + z)$，从而的推论。

#### 推论 2 {#alg-vi-s1-prop-11-cor-2 .statement tag=06X9}

— 在群有序晶格中，如果 x 和 y 互质，并且如果 z $\geq 0$ 和 $x \leq y + z$，则 $x \leq z$。

#### 推论 3 {#alg-vi-s1-prop-11-cor-3 .statement tag=06XA}

— 在群有序晶格中，如果 x 与 y 和 z 互质，那么它也与 $y + z$ 互质。

#### 推论 4 {#alg-vi-s1-prop-11-cor-4 .statement tag=06XB}

— 如果 $(x_i)_{1 \leq i \leq n}$ 和 $(y_j)_{1 \leq j \leq m}$ 是群 G 晶格有序的元素的两个有限族，使得每个 $x_i$ 与每个 $y_j$ 互质，则 $x_1 + \ldots + x_n$ 与 $y_1 + \ldots + y_m$ 互质。
这是从 Cor 得出的。 3 通过归纳在 m 和 n 上。

#### 推论 5 {#alg-vi-s1-prop-11-cor-5 .statement tag=06XC}

— 对于任意整数 $n \geq 0$，我们有 $(nx)^+ = nx^+$ 和 $(nx)^- = nx^-$；对于所有$n \in \mathbf{Z}$，我们有$|nx| = |n| \cdot |x|$。
确实$nx = nx^+ - nx^-$；因为 $x^+$ 和 x 是互质的，所以如果 $n \geq 0$ 则 $nx^+$ 和 $nx^-$ 也是互质的（Cor. 4）；第一个断言遵循VI、p. 12的第9条b)提案。在$n \geq 0$情况下，第二个是根据第9 d)条命题从第一个推导出来的；案例$n < 0$是由关系$|-x| = |x|$得出的结果。

#### 命题 11 {#alg-vi-s1-div-prop-11 .statement tag=06XD}

— 假设集合$\mathscr{P}^*$是一个格，并令$(a_i)$、$(b_j)$为A的元素的两个有限族。则$\prod_i a_i$和$\prod_j b_j$除乘积$\prod_{i,j} \gcd(a_i, b_j)$的每个gcd。

#### 推论 1 {#alg-vi-s1-div-prop-11-cor-1 .statement tag=06XE}

— 如果 a、b、c 是 A 的三个元素，且 a 与 b 互质，则 a 和 c 的每个 gcd 也是 a 和 bc 的 gcd。

#### 推论 2（欧几里得引理）{#alg-vi-s1-div-prop-11-cor-2 .statement tag=06XF}

— 令 a、b、c 为 A 的三个元素。如果 a 与 b 和除 bc 互质，则它除 c。

#### 推论 3 {#alg-vi-s1-div-prop-11-cor-3 .statement tag=06XG}

— 如果 x 与 y 和 z 互质，则它与 yz 互质。

#### 推论 4 {#alg-vi-s1-div-prop-11-cor-4 .statement tag=06XH}

— 如果$(x_i)$和$(y_j)$是A的元素的两个有限族，使得每个$x_i$与每个$y_j$互质，则$x_i$的乘积与$y_j$的乘积互质。

#### 推论 5 {#alg-vi-s1-div-prop-11-cor-5 .statement tag=06XI}

— 如果 d 是 x 和 y 的 gcd，则对于每个正整数 n，$d^n$ 是 $x^n$ 和 $y^n$ 的 gcd。
事实上，$xd^1$和$yd^1$是互质的（命题10（DIV）），因此$x^n d^{-n}$和$y^n d^{-n}$也是互质的（Cor.4）。

#### 命题 12 {#alg-vi-s1-prop-12 .statement tag=06XJ}

— 令 $x_i$ ($1 \leq i \leq n$) 成为群晶格中的 n 两对互质元素。然后
$$
\sup(x_1, \ldots, x_n) = x_1 + \cdots + x_n .
$$

这是从公式$u + v = \sup(u, v) + \inf(u, v)$（VI，p. 10，命题7）通过$n$上的归纳得出的，使用$x_i$对于$2 \leq i \leq n$来说与$x_1 + \ldots + x_{i-1}$互质（Cor.4到命题7）。 11）。

#### 注 {#alg-vi-s1-n12-rem-1 .statement tag=06XK}

VI、p. 10的第7条命题还表明，$x$和$y$互质的充要条件是$x + y = \sup(x, y)$。

#### 命题 12 {#alg-vi-s1-div-prop-12 .statement tag=06XL}

— *令$a_i$为$\mathbf{A}$的成对互质元素的有限数$n$；那么乘积 $a_1 \ldots a_n$ 是 $a_1, \ldots, a_n$ 的 lcm。*

#### 命题 13 {#alg-vi-s1-prop-13 .statement tag=06XM}

— *在群$G$有序的格子中，令$(x_\alpha)$为具有下确界（或上确界）的族，并令$z$为$G$的任意元素；那么家族$(\sup(z, x_\alpha))$（或$(\inf(z, x_\alpha))$）有下确界（或至上）并且*

$$
\begin{align*}
\inf_{\alpha} (\sup(z, x_\alpha)) &= \sup \left( z, \inf_{\alpha} x_\alpha \right) \\
\sup_{\alpha} (\inf(z, x_\alpha)) &= \inf \left( z, \sup_{\alpha} x_\alpha \right)
\end{align*}
$$

分别。

假设族$(x_\alpha)$有一个下确界$y$。我们将证明$\sup(z, y)$是族$(\sup(z, x_\alpha))$的下确界。

事实上$\sup(z, x_\alpha) = z + (x_\alpha - z)^+$，通过翻译我们可以将约化翻译成$z = 0$，也就是说我们必须证明$(x_\alpha^+)$的下确界等于$y^+$。从$y \leq x_\alpha$开始，我们对所有$\alpha$都有$y^+ \leq x_\alpha^+$（VI，p. 12，提案9，c））。相反，如果 $a \leq x_\alpha^+$ 对于所有 $a$，则得出 $a \leq x_\alpha + x_\alpha^-$（命题 9，a））；现在 $y^- \geq x_\alpha^-$ 自 $y \leq x_\alpha$；因此 $a \leq x_\alpha + y^-$ 对于所有 $a$，即 $a \leq y + y^- = y^+$。

另一个公式随后更改为相反的序关系。

#### 推论{#alg-vi-s1-n12-cor-1 .statement tag=06XN}

— *如果群$G$有序格的元素$z$与具有下确界$y$的族中的每个元素$x_\alpha$互质，则$z$与$y$互质。*

这是第二个公式 (4) 的直接的推论。

#### 注 {#alg-vi-s1-n12-rem-2 .statement tag=06XO}

将第 13 条命题的应用公式应用于二人家庭元素 $(x, y)$，我们得到以下公式，它表达了以下事实：合成sup, inf 中的律中的每一个合成sup, inf 在有序群的格子中都是*可分配的*关于另一个：

$$
\begin{align*}
\sup(z, \inf(x, y)) &= \inf(\sup(z, x), \sup(z, y)) \\
\inf(z, \sup(x, y)) &= \sup(\inf(z, x), \inf(z, y)) .
\end{align*}
$$

这个分配律性质是晶格有序 *群* 所特有的，而不是扩展任意晶格，甚至晶格有序幺半群（cf. VI、p. 33、Ex. 24）。

### 13.不可约元

#### 定义 6 {#alg-vi-s1-def-6 .statement tag=06XP}

— *有序群 G 的元素 x 被认为是不可约的，如果它是 G 的严格正元素的集合中的最小值元素。*

令 x 为有序群 G 的不可约元；如果 y 是 G 的正元素，则元素 inf(x, y)（如果存在）只能等于 x 或 0。因此，在有序群 G 的格子中，每个正 y 要么大于不可约元 x，要么与不可约元 x 互质；特别是，两个不同的不可约元是互质的。

(DIV) 如果理想 (p) 是有序群 $\mathscr{P}^*$ 的不可约元，则 A 的元素 p 称为“不可约”；这表示 p 既不是零也不是可逆的，并且除 p 与 p 或 1 关联的 $A$ 的任何元素要么与 p 要么与 1 关联。如果 $\mathscr{P}^*$ 是格序的，则每个 $a \in A$ 要么与 p 互质，要么与 p 的倍数互质。

#### 例（DIV）{#alg-vi-s1-n13-exa-1 .statement tag=0EEO}

1) 整数 $p > 0$ 在 $\mathbf{Z}$ 中不可约，当且仅当它是 *素数* (I, p. 50)。

2) 域 K 上的一个不定多项式是不可约的当且仅当它在通常意义上是不可约的 (IV, p. 13)。

#### 命题 14 {#alg-vi-s1-prop-14 .statement tag=06XQ}

— *对于有序群 G 的元素 $x > 0$ 是不可约的，只要满足以下性质就足够了：*

(P) *关系 $x \leq y + z,\ y \geq 0,\ z \geq 0$ 暗示 $x \leq y$ 或 $x \leq z$。*
*当 G 是晶格有序时，这个条件是必需的。*

如果 G 是晶格有序的并且 x 是不可约的，我们刚刚看到 y 要么大于 x，要么与 x 互质；在后一种情况下Cor。 VI、p. 15中的2表示z大于x。相反，假设满足条件：如果$0 \leq y \leq x$，那么通过放入$x = y + z\ (z \geq 0)$，可以得出$x \leq y$或$x \leq z$；在第一种情况下，我们有 $x = y$；第二个我们有$x \leq x - y$，所以$y \leq 0$，所以$y = 0$；这表明 x 确实是不可约的。

#### 命题 14 {#alg-vi-s1-div-prop-14 .statement tag=06XR}

— *为了使 A 的非零元素 p 不可约，只要它不是单位，并且它是 A 的两个元素的不能除乘积即可，无需除掉其中一个或另一个。如果 $\mathscr{P}^*$ 是晶格有序的，那么条件是必需的。*

#### 注 {#alg-vi-s1-n13-rem-1 .statement tag=06XS}

命题 14 (DIV) 也可以表示如下：如果 p 是 A 的非零元素，且理想 (p) 是 *素数* (I, p. 117, Def. 3)，则 p 是不可约的；相反，如果 $\mathscr{P}^*$ 是晶格有序的并且 p 是不可约的，则理想 (p) 是素数。

#### 命题 15 {#alg-vi-s1-prop-15 .statement tag=06XT}

— *在有序群 G 中，令 $(p_i)_{i \in I}$ 为 G 满足条件 (P) 的成对不同正元素族（因此不可约）。然后映射*

$$
(n_i)_{i \in I} \mapsto \sum_{i \in I} n_i p_i
$$

是有序群$\mathbf{Z}^{(I)}$的同构，有序群$Z$的直和（VI，p. 7）到$p_\iota$生成的$G$的有序子群。

足以证明对于所有$\iota$，关系$\sum_{\iota \in I} n_\iota p_\iota \geq 0$等价于$n_\iota \geq 0$，特别是关系$\sum_{\iota \in I} n_\iota p_\iota = 0$将意味着对于所有$\iota$的$n_\iota = 0$，因此这将表明族$(p_\iota)$是线性独立的。现在让$I'$（或$I''$）为那些$\iota$中$I$由……组成的有限子集，使得$n_\iota > 0$（或$n_\iota < 0$）；我们有

$$
\sum_{\iota \in I'} n_\iota p_\iota \geq \sum_{\iota \in I''} (-n_\iota)p_\iota .
$$

特别是，对于$\lambda \in I''$，这意味着$p_\lambda \leq \sum_{\iota \in I'} n_\iota p_\iota$，并且根据性质（P）的归纳，我们对于某些$\iota \in I'$必须有$p_\lambda \leq p_\iota$；由于$p_\iota$是不可约的，这意味着$p_\lambda = p_\iota$，这是荒谬的。因此$I'$为空，这就证明了命题。

#### 定理 2 {#alg-vi-s1-thm-2 .statement tag=06XU}

— 令 $G$ 为过滤后的群。那么以下属性是等效的：
a) $G$ 同构于形式 $\mathbf{Z}^{(I)}$ 的有序群。
b) $G$ 是格序的并且满足以下条件 ：
(MIN) $G$ 的正元素中的每个非空集合都有一个最小值元素。
c) $G$ 满足条件 (MIN)，并且 $G$ 中的每一个不可约元都有性质 (P)。
d) $G$由其不可约元生成，$G$的每个不可约元都有性质（P）。

让我们首先证明a) 蕴涵b)。 群 $\mathbf{Z}^{(I)}$ 是格序的，如全序群的直和。另一方面，令$E$为$\mathbf{Z}^{(I)}$的正元素的非空集合，并让$x = \sum n_\iota e_\iota$为$E$的元素（其中$(e_\iota)$表示$\mathbf{Z}^{(I)}$的自然基）； 元素 $y$ $\mathbf{Z}^{(I)}$ 的有限数 $\prod (n_\iota + 1)$ 使得 $0 \leq y \leq x$，因此 $E$ 的元素的集合 $F$ 小于或等于 $x$ 是$a$更不必说有限；因为它是非空，所以包含是元素的最小值（集合理论，III，p. 170，Cor.2），这显然是$E$的最小值元素。

根据命题 14，很明显 b) 蕴含 c)。让我们证明 c) 蕴含 d)。由于$G$已被过滤，因此足以（VI，p. 4，命题4）检查$G$的正元素的集合$F$（即不可约元的和）是否等于$G_+ - \{0\}$。如果这不是真的，则从 (MIN) 可以得出，$G_+ - \{0\}$ 中$F$ 的补集将具有最小元素 $a$；通过定义$a$不是不可约的，两个严格正数元素$x$和$y$的和也是不可约的；因为$x < a$和$y < a$，这些元素属于到$F$，和不可约元也是如此，因此$a$也是如此，这是一个矛盾。最后，d) 隐含了第 15 条命题中的 a)。

我们将应用Th。 2 主理想整环（VII，p. 4）和独特因式分解域（AC，VII, § 3）中的整除理论，以及戴德金环（AC，VII, § 2）中的理想研究。

### 习题 {#alg-vi-s1-exercises}

§ 1](exercises/s1/)参见[习题。
