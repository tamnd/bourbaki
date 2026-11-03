---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 2
section_title: Fundamental topological properties of the real line
lang: zh
source: top-i-iv
book_pages: 334-339
pdf_pages: 0340-0345, 0387-0393
extraction: ocr
subsections:
    - "no": 1
      title: ARCHIMEDES' AXIOM
      page: 334
      pdf_page: 340
    - "no": 2
      title: COMPACT SUBSETS OF $\mathbf{R}$
      page: 335
      pdf_page: 341
    - "no": 3
      title: LEAST UPPER BOUND OF A SUBSET OF $\mathbf{R}$
      page: 335
      pdf_page: 341
    - "no": 4
      title: CHARACTERIZATION OF INTERVALS
      page: 336
      pdf_page: 342
    - "no": 5
      title: CONNECTED SUBSETS OF $\mathbf{R}$
      page: 336
      pdf_page: 342
    - "no": 6
      title: HOMEOMORPHISMS OF AN INTERVAL ONTO AN INTERVAL
      page: 338
      pdf_page: 344
statements: 15
exercises: 21
content_sha256: 644063119e826640ca3e7c93a74d294084f80a3396e7d4c73681faf03bd7f83a
translated_from: content/en/top/IV/02_s2_fundamental_topological_properties_of.md
translation_method: google
source_content_sha256: 755e0a5ffdc8a22322a526f93559f059538fb20d8e64ae8fd4eec35f00c1c939
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: aef33cb129802bf6b2a13d71c2504a820e2959156e77a8ad2b2d07118777eb99
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 2. 实直线的基本拓扑性质

### 1. 阿基米德公理

作为该截面主题的实直线的拓扑性质是以下定理的所有推论：

#### 定理 1 {#top-iv-s2-thm-1 .statement tag=0BPF}

*如果 $x$ 和 $y$ 是任意两个实数 > 0，则存在整数 $n > 0$ 使得 $y < nx$。*

存在两个有理数数、$p/q$和$r/s$，使得$0 < p/q < x$和$y < r/s$，因为开区间]$0, x$和]$y, \to$不为空（$\S$I，no. 4， 命题 4);取$n$使得$nps > qr$，我们有$y < nx$。

#### 注 {#top-iv-s2-n1-rem-1 .statement tag=0BPG}

实数的理论的公理构造将在章V、$\S$2中找到，其中定理1作为公理出现；有关该公理的更多详细信息，请参阅历史注记至章 IV。

### 2. 紧凑型子集 / $\mathbf{R}$

#### 定理 2（波雷尔-勒贝格）{#top-iv-s2-thm-2 .statement tag=0BPH}

为了使实直线 $\mathbf{R}$ 的子集变得紧致，它是闭集且有界的必要且充分。

1) 条件是必要的。令$A$为$\mathbf{R}$的紧致子集，令$a$为实数$> 0$。 集合 $A$ 是闭集 (章 I, $\S$ 9, no. 3, 命题 4) 并且存在有限数点 $x_i$ $\mathbf{R}$的($1 \leq i \leq n$)使得$A$包含在邻域$[x_i - a, x_i + a]$的并中(章I、$\S$9、no. 3)。令$b$为数$|x_i|$中的最大值；那么我们就有$A \subset [-b - a, b + a]$。

2) 条件就足够了。足以证明每个区间$[ -a, +a ]$（$a > 0$）都是紧的，并且由于这个区间是完全均匀空间的封闭子集，因此足以证明，对于每个$b > 0$，我们可以用有限的覆盖$[ -a, +a ]$ 形式$[x - b, x + b]$区间数(章II、$\S$4、no. 2、推论至定理3)。现在，令$n$为整数$> 0$，使得$a < nb$；如果$x \in [ -a, +a ]$并且$m$是最大的整数（正或负）使得$mb \leq x$，那么我们有$-n \leq m \leq n$和$mb \leq x \leq (m + 1)b$。因此，$2n + 1$区间$[ (k - 1)b, (k + 1)b ]$（$-n \leq k \leq n$）形式覆盖了所需的型。

#### 推论 1 {#top-iv-s2-thm-2-cor-1 .statement tag=0BPI}

实直线 $\mathbf{R}$ 的子集是相对紧的当且仅当它是有界的。

#### 推论 2 {#top-iv-s2-thm-2-cor-2 .statement tag=0BPJ}

实直线是局部紧致的空间并且不是紧致的。

#### 注 {#top-iv-s2-n2-rem-1 .statement tag=0BPK}

定理 2 通常被称为“Heine-Borel 定理”；请参阅历史注记至章、II和IV。

### 3. 至少上界 / 子集 / $\mathbf{R}$

#### 定理 3 {#top-iv-s2-thm-3 .statement tag=0BPL}

实直线的每个非空子集其上界（或下界）都至少有上界（或下确界）。

令$A$为$\mathbf{R}$的非空子集，有界于上，并令$b$为$A$的上界，因此$A \subset ]\leftarrow, b]$。对于每个$x \in A$，考虑数$\geqslant x$中的集合$A_x$，其中属于到$A$； 集合 $A_x$ 形式基 $\mathfrak{B}$ 在 $\mathbf{R}$ 上，从 $A_y \subset A_x$ 如果 $y \geqslant x$ 开始。设$a$为$A$中的点。对于每个$x \geqslant a$属于到$A$，$A_x$包含在紧凑区间$[a, b]$中，因此过滤器基$\mathfrak{B}$有一个集群点$c$。由于区间 $[x, \rightarrow[$ 是闭合的，$c$ 属于到它们的交，因此 $c$ 是 $A$ 的上界。但是，另一方面，$A$的每个上界$z$都是$\geqslant c$，否则$c$的邻域$]z, \rightarrow[$不会包含$A$的任何点。因此$c$是$A$中最小的上界。

我们可以类似地论证一个下界的非空集合$B$，或者简单地指出$-B$非空且上界，并且如果$c$是$-B$的最小上界，那么$-c$是$B$的下确界。

$A$中最小的上界$c$可以用以下两个性质来表征：
(i) 对于每个 $x \in A, x \leqslant c_*$。
(ii) 对于每个$a < c$，存在$x \in A$使得$a < x \leqslant c$。

闭集合（非空且上界）属于到集合的最小上界是它的最大元素；并且上面有界的$\mathbf{R}$的任何非空子集$A$中的最小上界可以定义为$A$闭包中的最大的实数。

### 4. 刻画 / 区间

#### 命题 1 {#top-iv-s2-prop-1 .statement tag=0BPM}

*$\mathbf{R}$的非空子集$A$是区间当且仅当$a$和$b$是$A$的任意两个点，使得$a < b$为闭区间 $[a, b]$包含在$A$*中。

条件显然是必要的。反之，假设它是满意的。如果$A$既不上界也不下界，它一定是$\mathbf{R}$的整体，因为如果$x$是$\mathbf{R}$的任意点，则$A$有两个点$a, b$，使得$a < x < b$。如果$A$有界于上方而不是下方，则令$k$为其最小上界；那么对于任何$x < k$，$A$中存在$a$和$b$，使得$a < x < b \leqslant k$，因此$x \in A$，因此$A$只能是两个区间$]\leftarrow, k], ]\leftarrow, k[$之一。其他情况下的论证也类似。

### 5. 已连接子集 / $\mathbf{R}$

#### 定理 4 {#top-iv-s2-thm-4 .statement tag=0BPN}

*当且仅当$A$为区间时，$\mathbf{R}$的子集$A$相连。*

i) 条件是必要的。假设$A$是连通的：如果$A$由单个点组成，则它是区间。如果$A$有多个点，则令$a$和$b$为$A$中的两个点，使得$a < b$；通过 no. 4 的命题 1 足以证明每个 $x$ 使得 $a < x < b$ 属于到 $A$。现在，如果$x \notin A$我们应该有$A \subset C\{x\}$；但$C\{x\}$是两个不相交的开集合]$\leftarrow, x[$和$]x, \rightarrow[$的并，它们都满足$A$，因此$A$不会连接，与假设相反。

2) 条件 *足够*。首先让我们证明每个 *compact* 区间 $[a, b]$ 都是连通的。对于每个整数$n > 0$，让$V_{1/n}$是所有对$(x, y)$的随从由……组成，使得$|x - y| \leq 1/n$；通过命题 6 of 章 II, § 4, no. 4，足以证明点 $x, y$ 的$[a, b]$的每一个对都可以由$V_{1/n}$链连接起来。令 $p$ 为最大的整数，使得 $p/n \leq x$，令 $q$ 为最大的整数，使得 $q/n \leq y$（$p$ 和 $q$ 存在，因为定理 1 no. 1);然后$p \leq q$。如果$p = q$则$y - x < 1/n$和点$x$和$y$形式一条$V_{1/n}$链。如果$q > p$，则放入$x_i = (p + i)/n$（$i = 1, 2, \ldots, q - p$）；我们有$x_1 - x \leq 1/n$，$y - x_{q-p} \leq 1/n$和$x_{i+1} - x_i = 1/n$，因此点$x, x_1, x_2, \ldots, x_{q-p}, y$形式连接$x$和$y$的$V_{1/n}$链。

如果现在$I$是单个点的任何区间而不是由……组成，并且如果$a$和$b$是$I$的任何两个点使得$a < b$，则区间 $[a, b]$包含在$I$中并且是连通的，因此$I$是连通的。

#### 推论 1 {#top-iv-s2-thm-4-cor-1 .statement tag=0BPO}

*实直线是已连接且本地连接的空间.*

#### 推论 2 {#top-iv-s2-thm-4-cor-2 .statement tag=0BPP}

*只有$\mathbf{R}$的紧连通子集才是有界闭区间。*

到定理 4 时，$\mathbf{R}$ 中的子集不会包含超过 1 个点中的任何区间由……组成 *完全断开连接*；例如，对于有理数数的集合$\mathbf{Q}$来说，这是正确的，因为无理数数的集合$C\mathbf{Q}$在$\mathbf{R}$中是稠密的。

#### 命题 2 {#top-iv-s2-prop-2 .statement tag=0BPQ}

*$\mathbf{R}$中的每个非空开集合都是互为不相交的开区间的可数族的并。*

令$A$为$\mathbf{R}$中的非空开集合。由于$\mathbf{R}$是本地连接的，$A$的每个*分量*都是一个连接的开集合（章I, § 11, no. 6，命题11），因此一个*开区间*由定理4。这些开放区间是不相交的；另一方面，它们每个包含都是有理数数；因此，这些区间中的集合有幂小于或等于$\mathbf{Q}$，即是*可数*。

由此可见，$\mathbf{R}$中的每个闭集合都是互开不相交的开区间（有限或无限）序列$(I_n)$的并的补集。据说这些区间与正在考虑的封闭集合“连续”。相反，给定区间的序列，它们的并的补集是一个闭集合，这些区间与它相邻。

#### 例 {#top-iv-s2-n5-exa-1 .statement tag=0BPR}

让我们将定义由归纳互为不相交的的可数族$(I_{n,p})$开区间如下：
整数$n$取所有值$\geqslant 0$，对于$n$中的每个值，$p$取值$1, 2, 3, \ldots, 2^n$。所有区间 $I_{n,p}$ 都包含在
$$
A = [0, 1],
$$
我们取$I_{0,1} = ]1/3, 2/3[$（$]0, 1[$的“中间三分之一”）。现在假设$2^{m+1} - 1$区间$I_{n,p}$已经为$0 \leq n \leq m$定义，如果$J_m$是它们的并，则集合$A \cap \complement J_m$互为$2^{m+1}$的并不相交的区间 $K_{m,p}$ ($1 \leq p \leq 2^{m+1}$) 长度 $\frac{1}{3^{m+1}}$ 各关闭。如果$K_{m,p} = [a, b]$，那么我们将$I_{m+1,p}$作为开盘区间$\left[ a + \frac{b-a}{3}, \frac{b-a}{3} \right]$（区间$]a, b[$的“中间三分之一”），并且立即验证归纳可以这样继续下去（图3）。

![图表显示区间 I_{2,1}、I_{1,1}、I_{2,2}、I_{0,1}、I_{2,3}、I_{1,2}、I_{2,4} 和相应的区间 K_{2,1}、K_{2,2}、K_{2,3}、 K_{2,4}、K_{1,1}、K_{1,2}、K_{1,3}、K_{1,4}、K_{0,1}、K_{0,2}](https://i.imgur.com/3Q5z5QG.png)

图 3.

如果$K'$是$I_{n,p}$的并的补集，则闭集集合$K = A \cap K'$称为康托三元集合。显然 $K$ 是紧致的 (no. 2, 定理 2)； $K$ 也完全断开。因为如果$K$包含长度$> 0$中的区间$I$，那么$I$将包含在一些区间$K_{m,p}$中；因此，对于每个$m$，它的长度将是$\leq 1/3^{m+1}$，这是荒谬的。

### 6. 区间到区间的同态

#### 定理 5 {#top-iv-s2-thm-5 .statement tag=0BPS}

*令I为R中的区间。则I的映射f到R中是I到f(I)的同胚当且仅当f在I上严格单调且连续；那么 f(I) 就是 R 中的区间。*

1) 条件是必要的。令$a$和$b$为I的两个点，使得$a < b$，并假设例如$f(a) < f(b)$。让我们证明$f$在I上是严格递增的。首先，如果$a < c < b$，那么我们必须有$f(a) < f(c) < f(b)$；例如，如果我们有$f(a) < f(b) < f(c)$，那么$f$下的区间$[a, c]$的像将是一个连接的集合（章I，，no. 2，命题4）并且将因此包含区间 $[f(a), f(c)]$；因此存在$x \in [a, c]$使得$f(x) = f(b)$，与假设相反，$f$是单射的

由此可见，如果$x$和$y$是I中的任意两个点，使得$x < y$，则$f(x) < f(y)$；因为如果$a < x < b$，我们有$f(a) < f(x) < f(b)$，如果$b < x$，我们有$f(a) < f(b) < f(x)$，如果$x < a$，我们有$f(x) < f(a) < f(b)$；分别用$a, x, y$代替$a, b, x$重复论证，我们看到$f(x) < f(y)$。

2) 条件 *足够*。假设 $f$ 在 I（比如严格递增的）上是连续且严格单调的：$f(I)$ 是连通的，因此是区间，并且由于 $f$ 是严格递增的，$f$ 是一个双射映射 I 到$f(I)$。此外，开区间 *in* I 的 $f$ 下的像是开区间 *in* $f(I)$，因此 (§ 1, no, 4, 命题 5) $f$ 是I 到$f(I)$。

#### 注 {#top-iv-s2-n6-rem-1 .statement tag=0BPT}

前面的证明的第一个部分实际上表明I到$\mathbf{R}$的*连续单射*映射是严格单调的；因此，从证明的第二个部分开始，*区间* I *到* $\mathbf{R}$ *的每个连续单射映射* $f$ *都是* I *到* $f(I)$ 的同胚。

### 习题 {#top-iv-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
