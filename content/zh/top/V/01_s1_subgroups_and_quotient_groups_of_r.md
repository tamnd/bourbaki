---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 1
section_title: Subgroups and quotient groups of R
lang: zh
source: top-v-x
pdf_pages: 0013-0017, 0030-0031
extraction: ocr
subsections:
    - "no": 1
      title: CLOSED SUBGROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 2
      title: QUOTIENT GROUPS OF $\mathbf{R}$
      page: 0
      pdf_page: 13
    - "no": 3
      title: CONTINUOUS HOMOMORPHISMS OF $\mathbf{R}$ INTO ITSELF
      page: 0
      pdf_page: 15
    - "no": 4
      title: LOCAL DEFINITION OF A CONTINUOUS HOMOMORPHISM OF $\mathbf{R}$ INTO A TOPOLOGICAL GROUP
      page: 0
      pdf_page: 15
statements: 13
exercises: 3
content_sha256: d476b573cc8025cff2a7d9221d49dbfcadb09cd3e1c966b2d57b2fdea4634b33
translated_from: content/en/top/V/01_s1_subgroups_and_quotient_groups_of_r.md
translation_method: google
source_content_sha256: 1e96322726cdb481cae00351a70dc8c5c1282af2de71cdb8ab479eeee32a02d2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 9efd3f8cd5b9c7697aff22e70964127bbce6d588e208b31fbb62ce7e89cf3afa
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 子群和商群 $\mathbf{R}$

### 1. 子群 $\mathbf{R}$ 关闭

#### 命题 1 {#top-v-s1-prop-1 .statement tag=0BV0}

*加法群 $\mathbf{R}$的每个闭子群，除了$\mathbf{R}$和$\{0\}$之外，都是形式$a.\mathbf{Z}$的离散群，其中$a > 0$*（在其他字中，它由整数组成） 倍数共 $a$）。

我们首先证明$\mathbf{R}$的每个非离散子群在$\mathbf{R}$中都是稠密的。如果$\mathbf{R}$的子群$G$不是离散的，那么对于每个$\varepsilon > 0$，$G$中有点$x \neq 0$，其中属于到区间$[-\varepsilon, +\varepsilon]$；由于 $x$ 属于到 $G$ 的所有整数倍数，长度 $> \varepsilon$ 包含元素 $G$ 的每区间，因此$G$ 在 $\mathbf{R}$ 中是稠密的。

因此，除 $\mathbf{R}$ 本身之外，$\mathbf{R}$ 的每个闭子群都是离散的。还需要证明，除了$\{0\}$之外，$\mathbf{R}$的每个离散子群$G$都是形式$a.\mathbf{Z}$，其中$a > 0$。现在关系$-G = G$表明$G$中元素$> 0$的集合$H$不为空；如果$b \in H$、区间、$[0, b]$和$G$的交是*紧凑且离散的*，因此是*有限的*。令$a$为$[0, b]$中包含的$H$的最小的元素，并且对于每个$x \in G$放入$m = [x/a]$、$x/a$的整数部分；那么我们就有 $x - ma \in G$ 和 $0 \leq x - ma < a$。根据$a$的定义，可以得出$x - ma = 0$，因此也有$G = a.\mathbf{Z}$。

### 2. 商群共 $\mathbf{R}$

$\mathbf{R}$ 的每个 *Hausdorff* 商群都是形式 $\mathbf{R}/H$，其中 $H$ 是 $\mathbf{R}$ 的*封闭* 子群 (章 III, § 2, no. 6，命题 18)；因此，通过命题 1 of no. 1：

#### 命题 2 {#top-v-s1-prop-2 .statement tag=0BV1}

** $\mathbf{R}$ 的 *Hausdorff 商群，*除了* $\{0\}$，*为群* $\mathbf{R}/a\mathbf{Z}$ ($a \geqslant 0$)。
*如果* $a$ *和* $b$ *是* $> 0$、*自同构* $x \to b/a\,x$ *的* $\mathbf{R}$ *变换* $a\mathbf{Z}$ *进入* $b\mathbf{Z}$，*因此* (章 III, § 2, no. 8, 注 3) *商群* $\mathbf{R}/a\mathbf{Z}$ *和* $\mathbf{R}/b\mathbf{Z}$ *同构的；其他字*：

#### 命题 3 {#top-v-s1-prop-3 .statement tag=0BV2}

** $\mathbf{R}$ 的每个 Hausdorff 商群，*除了* $\mathbf{R}$ *和* $\{0\}$，*同构于群* $\mathbf{R}/\mathbf{Z}$。

#### 定义 1 {#top-v-s1-def-1 .statement tag=0BV3}

*拓扑群* $\mathbf{R}/a\mathbf{Z}$ ($a > 0$) *称为实数模* $a$的加法群。 *拓扑群* $\mathbf{R}/\mathbf{Z}$ *表示为* $\mathbf{T}$。 *作为拓扑空间，* $\mathbf{T}$ *被称为一维环面*（滥用语言，拓扑群$\mathbf{T}$也被称为一维环面）。

#### 注 1 {#top-v-s1-n2-rem-1 .statement tag=0BV4}

*关系* $x \equiv y \pmod{a\mathbf{Z}}$ *is usually written* $x \equiv y \pmod{a}$, *or simply* $x \equiv y (a)$, *and is read* "x and y are congruent modulo a"; *it means that* $x - y$ *is 整数倍数 of* $a$. *When* $a$ *is 整数, 关系 induced on* $\mathbf{Z}$ *by this 关系 is precisely congruence modulo* $a$; *这证明了记号*。

#### 注 2 {#top-v-s1-n2-rem-2 .statement tag=0BV5}

\* *正如我们将在章 VI, § 2, no. 4 中看到的，拓扑空间* $\mathbf{T}$ *同胚于圆* $x^2 + y^2 = 1$ *在实数平面* $\mathbf{R}^2$； *乘积空间* $\mathbf{T}^2$ *同胚于 * $\mathbf{R}^3$ *(章 VII, § 1, 习题 15)* 的旋转* 环面。 *这就是名字的由来*“一维环面”*对于*$\mathbf{T}$*（在章VII, § 1，我们称之为*$\mathbf{T}^n$*n维环面）* *。

#### 命题 4 {#top-v-s1-prop-4 .statement tag=0BV6}

*环面* $\mathbf{T}$ *同构于* $\mathbf{R}$ *形式* $[a, a+1]$ *的任何闭区间的商空间，通过识别该区间的端点获得；它结构紧凑、互联且本地连接*。

每个$x \in \mathbf{R}$*与区间*$[a, a+1]$中的某些数全等*$(\bmod\,1)$*，*即与*$x - [x-a]$； *因此* $\mathbf{T}$ *是区间的像在典范映射* $\varphi$ *的* $\mathbf{R}$ *到* $\mathbf{R}/\mathbf{Z}$，*因此是紧凑且相连的* (章 I, § 9, no. 4，定理 2，并且§ 11, no. 2、命题 4)。 *另一方面，区间* $[a, a+1]$ *的两个不同的元素 *全等* $(\bmod\,1)$ *仅当它们是区间的端点时；根据* $\mathbf{T}$ *因此得出* $\mathbf{T}$ *同胚于* $[a, a+1]$ *的商空间 *通过识别端点获得* (章 I, § 9, no. 4, 定理 2, 推论 4、§ 10, no. 4、命题 8)。 *最后，*$\mathbf{Z}$*作为*$\mathbf{R}$、$\mathbf{T} = \mathbf{R}/\mathbf{Z}$*的离散子群*与*$\mathbf{R}$*（章III, § 2, no. 6、命题19）*局部同构*并且特别是局部连接的（最后一个事实也是推论章 I, § 11, no. 6、命题 12)。

#### 注 {#top-v-s1-n2-rem-3 .statement tag=0BV7}

请注意，$\mathbf{R}$到$T = \mathbf{R}/\mathbf{Z}$的典范映射$\varphi$，仅限于半开区间$[a, a+1[$，是这个区间到$T$的连续双射映射；逆映射在$T$的每个点处连续，除了$\varphi(a)$之外，但在$\varphi(a)$处不连续。我们将有时认同空间$T$与区间$[a, a+1[$，赋予拓扑，即$T$拓扑$\varphi$下的逆像 （章I, § 1, no. 3）；这个拓扑当然和$\mathbf{R}$的拓扑在$[a, a+1[$上诱发的不一样。

### 3. 连续同态 OF $\mathbf{R}$ 自身

#### 命题 5 {#top-v-s1-prop-5 .statement tag=0BV8}

拓扑群 $\mathbf{R}$ 自身的每个连续同态 $f$ 都是形式 $x \to ax$，其中 $a \in \mathbf{R}$；如果$a \neq 0$的话，就是$\mathbf{R}$的自同构。

对于每个$x \in \mathbf{R}$和每个整数$p \in \mathbf{Z}$，我们有$f(px) = pf(x)$； 替换 $x$乘$(1/p)x$，因此

$$
f\left(\frac{1}{p}x\right) = \frac{1}{p} f(x) \quad \text{if } p \neq 0;
$$

因此，对于所有整数 $p$ 和 $q \neq 0$，我们有

$$
f\left(\frac{p}{q}x\right) = \frac{p}{q} f(x).
$$

在其他字，$f(rx) = rf(x)$对于所有有理数数$r$。如果现在$t$是任何实数，由于$f$的连续性，我们有

$$
f(tx) = \lim_{r \to t, r \in \mathbf{Q}} f(rx) = \lim_{r \to t, r \in \mathbf{Q}} rf(x) = \left( \lim_{r \to t, r \in \mathbf{Q}} r \right) f(x) = tf(x).
$$

特别是，如果$a = f(1)$我们有$f(t) = at$，并且命题被证明。

因此，拓扑群$\mathbf{R}$的自同构的群同构于非零实数的乘法群$\mathbf{R}^*$。

#### 推论 {#top-v-s1-n3-cor-1 .statement tag=0BV9}

设$G$是群同构于$\mathbf{R}$。对于每个$a \in G$，$\mathbf{R}$中恰好有一个连续的同态$f_a$进入$G$，使得$f_a(1) = a$，并且如果$a$，则该同态是$\mathbf{R}$的同构到$G$不是 $G$ 的零元素。

### 4. 将$\mathbf{R}$的连续同态的局部定义转换为拓扑群

如果我们给出$G$的群$G$和子集$A$，其中生成$G$，很明显，$G$的两个同态$f, g$会变成群$G'$ 重合，如果他们在$A$的每点取相同的值。但$G$同态$f$$A$上值成$G'$不能一般是任意取的；如果 $G$ 和 $G'$ 被写成乘法，则对于每个对 $(x, y)$，这些值必须是满足条件 $f(xy) = f(x)f(y)$，使得 $x \in A, y \in A$ 和 $xy \in A$。此外，这个必要的条件一般来说是不够的。

特别是，拓扑群$G$的*局部同构*和拓扑群$G'$不能总是扩展到$G$的同态（连续或不连续）到$G'$。例如，将$T$的局部同构$f$和$\mathbf{R}$不能扩展到$T$的同态延伸到$\mathbf{R}$；因为如果$f$定义在$o$的邻域$V$上，则存在整数$p > 0$使得$\frac{1}{p}$属于到$V$的类$x \pmod{\mathbf{Z}}$；由于$x$在$T$中有阶$p$，因此在$T$的每个同态下进入$\mathbf{R}$的像必然是$o$，因此与$f(x)$相差假设。

在这方面，拓扑群$\mathbf{R}$享有以下性质：

#### 命题 6 {#top-v-s1-prop-6 .statement tag=0BVA}

*令$I$为$\mathbf{R}$中的区间，其中包含$o$以及至少一个其他点；设 $f$ 为 $I$ 的连续映射到拓扑群 $G$（乘法书写），使得 $f(x+y) = f(x)f(y)$ 对于点 $(x, y)$ 的每个对使得 $x \in I, y \in I$ 和$x + y \in I$。然后存在$\mathbf{R}$到$G$的唯一连续同态，其中扩展$f$.*。

扩张（如果存在）的唯一性源自前面的注，因为$I$生成群$\mathbf{R}$。我们必须确定这样的扩张的存在。

如果$n$是整数$> 0$并且如果$x \in I$和$nx \in I$，我们有$f(nx) = (f(x))^n$，通过归纳在$n$上（从$mx \in I$对于所有整数$m$这样$1 \leq m \leq n$）。把$J = \bigcup_{n \in \mathbf{N}} nI$； $J$要么是整条线$\mathbf{R}$，要么是区间、$[0, +\infty[$或$[-\infty, 0]$之一，根据$o$是否是$I$的内部点。如果$x \in J$，只要$n$是足够大整数$> 0$，我们就有$x/n \in I$。令$x \in J$，并令$m, n$是两个整数$> 0$，使得$x/n \in I$和$x/m \in I$；那么$x/mn \in I$，因此

$$
f\left( \frac{x}{m} \right) = \left( f\left( \frac{x}{mn} \right) \right)^n \quad \text{and} \quad f\left( \frac{x}{n} \right) = \left( f\left( \frac{x}{mn} \right) \right)^m;
$$

在其他字中，$G$的元素$(f(x/n))^n$对于所有整数$n > 0$都是相同的，因此$x/n \in I$。让我们用$f_1(x)$来表示这个元素； $f_1$是$J$到$G$的映射，它与$I$上的$f$一致，因此在点$o$连续（相对于$J$）。令$x, y$为J的两个元素，并令n为足够大整数 > 0，使得$\frac{x}{n} \in I, \frac{y}{n} \in I$和$\frac{x+y}{n} \in I$；然后

$$
f\left( \frac{x+y}{n} \right) = f\left( \frac{x}{n} \right) f\left( \frac{y}{n} \right) = f\left( \frac{y}{n} \right) f\left( \frac{x}{n} \right),
$$

这表明 $f\left( \frac{x}{n} \right)$ 和 $f\left( \frac{y}{n} \right)$ 通勤；通过$f_1$的定义，我们有$f_1(x+y) = f_1(x) f_1(y)$。如果$J = \mathbf{R}$，则证明完整；如果不是，则为 $J = [0, +\infty[$，并且每个 $x < 0$ 定义 $f_1(x)$ 为 $(f_1(-x))^{-1}$。那么关系$f_1(x+y) = f_1(x) f_1(y)$对于所有$x \in \mathbf{R}$和所有$y \in \mathbf{R}$仍然有效。如果$x < 0$和$y < 0$，这很清楚；如果$x \geqslant 0$、$y < 0$和$x + y \geqslant 0$，则从$f_1(x) = f_1(x+y) f_1(-y)$得出；类似地，如果$x \geqslant 0, y < 0$和$x + y < 0$，那么我们有

$$
f_1(-y) = f_1(-x-y) f_1(x);
$$

类似 $x < 0$ 和 $y \geqslant 0$ 的证明。因此我们看到$f_1$是$\mathbf{R}$的同态进入G，因此G的$f_1(0) = e$，单位元素；由于$f_1$相对于J连续，因此在0处右边有极限，等于$e$；由于$f_1(-x) = (f_1(x))^{-1}$，$f_1$在左侧0处也有极限，等于$e$；因此$f_1$在0处连续，证明是完整的。

#### 推论 {#top-v-s1-n4-cor-1 .statement tag=0BVB}

*设 f 是 $\mathbf{R}$ 的局部同构，具有拓扑群 G。那么，$\mathbf{R}$ 的唯一严格态射到 G 的开子群，其中重合与 0 的某些邻域的 f 完全点。*

设$\overline{f}$为$\mathbf{R}$到G的连续同态，它在开区间I的所有点上与$f$重合，其中包含0并且包含在定义$f$的集合中；假设$\overline{f}(\mathbf{R})$包含G的单位元的邻域，因此（第III, § 2, no. 1章，命题4的推论）是G的开子群；并且$\overline{f}$是$\mathbf{R}$到$\overline{f}(\mathbf{R})$的严格态射，根据第III, § 2, no. 8章，命题24。

#### 命题 7 {#top-v-s1-prop-7 .statement tag=0BVC}

*每个与 $\mathbf{R}$ 局部同构的连通群 G 也与 $\mathbf{R}$ 或 $\mathbf{T}$ 同构。*

对于$\mathbf{R}$的局部同构和G扩展到$\mathbf{R}$的严格态射到G的开放子群（推论到命题6），因此到G本身，因为G是连通的。因此 G 同构于 $\mathbf{R}$ 的商群；由于 G 是 Hausdorff 并且不单独由单位元素组成（因为它与 $\mathbf{R}$ 局部同构），因此它与 $\mathbf{R}$ 或 $\mathbf{T}$ 同构于 no. 2 的命题 3。

### 习题{#top-v-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
