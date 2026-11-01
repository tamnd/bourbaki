---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 4
section_title: Regular elements of a Lie group
lang: zh
source: lie-vii-ix
book_pages: 27-34, 63
pdf_pages: 0037-0044, 0072-0072
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS FOR A LINEAR REPRESENTATION
      page: 27
      pdf_page: 37
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE GROUP
      page: 29
      pdf_page: 39
    - "no": 3
      title: RELATIONS WITH REGULAR ELEMENTS OF THE LIE ALGEBRA
      page: 31
      pdf_page: 41
    - "no": 4
      title: APPLICATION TO ELEMENTARY AUTOMORPHISMS
      page: 34
      pdf_page: 44
statements: 18
exercises: 4
content_sha256: 9185bec37435fe5710567361a06fa270a3c89a11c4041cef7d21186244bf5e78
translated_from: content/en/lie/VII/04_s4_regular_elements_of_a_lie_group.md
translation_method: google
source_content_sha256: 1839a11c4384fe28967cd541901f8ab98cc088922894403c4f8106b9bf54bee7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 5bc48eda83d31966cfbf0a5e8351b81bdd40b2e75bb0fd8e6706a9da1bfec15c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 正则元素 / 李群

在没有。根据本段的1、2和3，我们假设$k$是$\mathbf{R},\mathbf{C}$或特征为0的非离散完全超度量域。我们用G表示$k$上的有限维李群，用$\mathfrak{g}$表示其李代数，并用$e$表示其单位元素。如果$a\in G$，我们用$\mathfrak{g}^1(a)$表示Ad$(a)-1$的零空间，在其他字空间$\mathfrak{g}^1$(Ad($a$))(cf.§1, no. 1)。

### 1.正则元素对于线性表示

#### 引理 1 {#lie-vii-s4-lem-1 .statement tag=00VU}

设 M 为 $k$ 上的解析流形以及 M 上函数的解析 $a= (a_0, . . . , a_{n-1}, a_n= 1)$ 序列。对于所有 $x\in M$，令 $r_a(x)$ 为 $i\in 0, n$ 的上界，使得 $a_j(x) = 0$对于$j < i$，令$r_a^0(x)$为那些$i\in 0, n$中的上界，使得对于$j < i$，$a_j$是$x$的邻域上的零。

(i) 函数 $r_a$ 是上半连续。

(ii) 对于所有$x\in M,r_a^0(x) =$ lim inf$_{y\rightarrow x}r_a(y)$。

(iii) 函数 $r_a^0$ 是局部常数。

(iv) 点 $x\in M$的集合使得$r^0_a(x) =r_a(x)$是邻域上M的点的集合，其中$r_a$是常数。这是 M 的密集开子集。如果 $k=\mathbf{C}$ 且 M 是有限维且连通的，则它是开且连通的。

(i) 如果$r_a(x) =i$，则$a_i(x)\not= 0$，并且对于$x$的邻域中的所有$y$，我们有$a_i(y)\not= 0$，因而$r_a(y)\leq i$。

(ii) 如果 $r^0_a(x) =i$、函数 $a_0, . . . , a_{i-1}$ 是 $x$ 的邻域上的零，并且对于此邻域中的任何 $y$，$r_a(y)\geq i$。因而，lim inf$_{y\rightarrow x}r_a(y)\geq i$。 $x$ 包含点 $y$ 的每个邻域使得$a_i(y)\not= 0$ 因而$r_a(y)\leq i$。因而 lim inf$_{y\rightarrow x}r_a(y) =i$。

(iii) 令$i=r_a^0(x)$且令V为$x$的邻域，使得$a_j(y) = 0$对于所有$y\in V$和所有$j < i$。那么$x\in M$**--** Z，其中Z表示邻域中M的点的集合，其中函数$a_i$是零。由于 Z 在 M 中是封闭的（可微分和解析流形，结果$, 5.3.5$）$, V\cap (M$ **--** Z）是 $x$ 的邻域。对于这个邻域中的每个点$y$，$r_a^0(y) =i$。

(iv) 函数$r_a-r_a^0$是上半连续，其值在任意点处为$\geq 0$。若$r_a(x) =r^0_a(x),r_a-r^0_a$在$x$的邻域上为零，则由(iii)可知$r_a$在$x$的邻域上恒定。相反，如果$r_a$在$x$的邻域上恒定，则$r_a^0(x) =r_a(x)$满足(ii)。 点 $x\in M$的集合，使得$r_a^0(x) =r_a(x)$是M的开子集$\Omega$。如果$x\in M$和$r^0_a(x)< r_a(x)$，$x$包含的每个邻域点$y$使得$r_a(y)< r_a(x)$和$r^0_a(y) =r_a^0(x)$。 $x$的每邻域因此包含点$y$这样

$$
r_a(y)-r^0_a(y)< r_a(x)-r^0_a(x)
$$

由此可知 $\Omega$ 在 M 中是稠密的。

如果 M 已连通，且 $p$ 是 M 上 $r_a^0$ 的值，则 $\Omega$ 的点是点 $x\in M$，使得 $a_p(x)\not= 0$。如果$k=\mathbf{C}$，这意味着$\Omega$由附录II中的引理 3 连接。

令 $\rho$ 为 G 在 $k$ 上有限维 $n$ 的向量空间 V 上的解析线性表示。放

检测（T$-\rho (g) + 1$）$=a_0(g) +a_1(g)T +\cdots +a_{n-1}(g)T^{n-1}+ T^n$。

与序列$(a_0, a_1, . . . , a_{n-1},1)$关联的函数$r_a$和$r_a^0$将分别由$r_{\rho}$和$r^0_{\rho}$表示。然后，对于所有$g\in G$，

$r_{\rho}(g) =$ 昏暗 $V^1(\rho (g))$

$r_{\rho}^0(g) =$lim inf$_{g'\rightarrow g}$暗淡$V^1(\rho (g'))$。

#### 引理 2 {#lie-vii-s4-lem-2 .statement tag=00VV}

令 $0\rightarrow V'\rightarrow V\rightarrow V''\rightarrow 0$ 分别为由 G 的解析线性表示 $\rho ', \rho , \rho ''$ 定义的 G 模的正合序列。然后：

$r_{\rho}=r_{\rho'}+r_{\rho''}$和$r^0_{\rho}=r^0_{\rho'}+r^0_{\rho''}$。

事实上，对于所有 $g\in G$，有 (§1, no. 1，Th.1 的 Cor. 3) 正合序列

$$
0\rightarrow (V')^1(\rho '(g))\rightarrow V^1(\rho (g))\rightarrow (V'')^1(\rho ''(g))\rightarrow 0
$$

这就证明了第一个断言。第二个是从它开始的，通过 G 的密集开子集上的引理 1 (iv)、$r^0_{\rho}=r_{\rho}, r^0_{\rho'}=r_{\rho'}$ 和 $r_{\rho''}^0=r_{\rho''}$。

#### 定义 1 {#lie-vii-s4-def-1 .statement tag=00VW}

如果 $r_{\rho}(g) =r^0_{\rho}(g)$，则元素 $g\in G$ 被称为线性表示 $\rho$ 的常规。

#### 命题 1 {#lie-vii-s4-prop-1 .statement tag=00VX}

G 的解析线性表示 $\rho$ 的正则点是邻域中 G 的点，其中 $r_{\rho}$ 是常数。它们构成了G的密集开子集。如果$k=\mathbf{C}$和G连通，则$\rho$的正则点的集合连通。

这是从引理 1 (iv) 得出的。

#### 注 {#lie-vii-s4-n1-rem-1 .statement tag=00VY}

设$G^*$是G的开子群。对于G的线性表示$\rho$，元素$a\in G^*$是G的正则元素当且仅当它是线性表示$\rho |G^*$的$G^*$的正则元素。

### 2. 正则元素李群

#### 定义 2 {#lie-vii-s4-def-2 .statement tag=00VZ}

如果 G 的伴随表示是正则的，则称 G 的元素是正则的。

在其他字（命题1）中，元素$g\in G$是正则的，如果对于G中$g$的邻域中的所有元素$g'$，Ad($g'$)$-1$的零空间的维数等于Ad($g$)$-1$ 的零空间的维数。

#### 命题 2 {#lie-vii-s4-prop-2 .statement tag=00W0}

设$G'$是$k$上的有限维李群，而$f$是从G到$G'$的开态射。 G的正则元素$f$下的像是$G'$的正则元素。如果$f$的核包含在G的中心中，则元素$g\in G$是规则的当且仅当$f(g)$是规则的。

事实上，让$\mathfrak{g}'$是$G'$的李代数，而$\mathfrak{h}$是由$Tf|\mathfrak{g}$的核给出的$\mathfrak{g}$中的理想值。对于所有$g\in G$，令$\rho$为$\mathfrak{h}$上G的线性表示，由$\rho (g) =$Ad$g|\mathfrak{h}$定义，并令Ad$\circ f$为$\mathfrak{g}'$上G的线性表示，由$f$与$G'$ 的伴随表示。这些线性表示定义正合序列 G 模块：

$$
0\rightarrow \mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}'\rightarrow 0
$$

引理$2,r_{Ad}=r_{\rho}+r_{Ad\circ f}$。由于$r_{Ad\circ f}=r_{Ad}\circ f$和$f$是开放的映射，$r_{Ad\circ f}^0=r_{Ad}^0\circ f$。因而：

$$
r_{Ad}-r^0_{Ad}=r_{\rho}-r_{\rho}^0+ (r_{Ad}-r_{Ad}^0)\circ f
$$

因而，如果$g$是正则，则$(r_{Ad}-r^0_{Ad})(f(g)) = 0$，这意味着$f(g)$是正则。如果$f$的核包含在G的中心中，

$r_{\rho}(g) =r_{\rho}^0(g) =$ 暗淡$\mathfrak{h}$ 对于所有 $g\in G$。因而，如果$f(g)$是正则，则$r_{Ad}(g) =r_{Ad}^0(g)$，在其他字中，$g$是正则。

#### 命题 3 {#lie-vii-s4-prop-3 .statement tag=00W1}

令$G_1$和$G_2$是$k$上的两个有限维李群。 $G_1\times G_2$的元素$(g_1, g_2)$是正则当且仅当$g_1$和$g_2$分别是$G_1$和$G_2$的正则元素。

根据命题 2，条件是必要的。我们证明它是充分的。对于所有$g= (g_1, g_2)\in G_1\times G_2,r_{Ad}(g) =r_{Ad}(g_1) +r_{Ad}(g_2)$。鉴于引理 1 (ii)，得出$r^0_{Ad}(g) =r^0_{Ad}(g_1) +r_{Ad}^0(g_2)$。如果$g_1$和$g_2$是正则，$r^0_{Ad}(g_1) =$$r_{Ad}(g_1)$和$r^0_{Ad}(g_2) =r_{Ad}(g_2)$，那么$r^0_{Ad}(g) =r_{Ad}(g)$，这意味着$g$是正则。

#### 引理 3 {#lie-vii-s4-lem-3 .statement tag=00W2}

令$a\in G$和$\mathfrak{m}$为$\mathfrak{g}$中$\mathfrak{g}^1(a)$的补集。令 U 为 $\mathfrak{g}$ 中 0 的邻域，并用指数映射从 U 到 G。 映射

$f: (x, y) \rightarrow$（经验$y$）$a$（经验$x$）（经验$y$）$^{-1}$

从 $(\mathfrak{g}^1(a)\times \mathfrak{m})\cap U$ 到 G 的时间为 $(0,0)$。

映射 $x \rightarrow a$(exp $x$) 和 $y \rightarrow$ (exp $y$)$a$(exp $y$)$^{-1}$ 在 0 处的切线映射为映射 $x \rightarrow ax$ 且$y \rightarrow ya-ay=a(a^{-1}ya-y)$从$\mathfrak{g}$到$T_aG =a\mathfrak{g}$（第III, §3, no. 12章，第46条提案）。因而，$f$在$(0,0)$处的切线映射是从$\mathfrak{g}^1(a)\times \mathfrak{m}$到$a\mathfrak{g}$的映射$(x, y) \rightarrow ax+a(a^{-1}ya-y) =a(x+a^{-1}ya-y)$。这个映射是单射的。事实上，如果 $x\in \mathfrak{g}^1(a), y\in \mathfrak{m}$ 且 $x+a^{-1}ya-y$ = 0，则 (Ad($a$)$-1$)$y$ = Ad($a$)$x\in \mathfrak{g}^1(a)$，因为 Ad($a$)$\mathfrak{g}^1(a)\subset \mathfrak{g}^1(a)$。这意味着$y\in \mathfrak{g}^1(a)$，因而$y$ = 0。由于Ad($a$)在$\mathfrak{g}^1(a)$上单射，因而$x$ = 0。由于dim $\mathfrak{g}=$ dim$\mathfrak{g}^1(a) +$ dim $\mathfrak{m}$，这表明$f$是étale $(0,0)$。

#### 命题 4 {#lie-vii-s4-prop-4 .statement tag=00W3}

令 $a\in G$ 和 H 为 G 与李代数 $\mathfrak{g}^1(a)$ 的李子子群胚芽。从$H\times G$到G的映射$(b, c) \rightarrow cabc^{-1}$是$(e, e)$的淹没。

事实上，让$\mathfrak{m}$是$\mathfrak{g}$中$\mathfrak{g}^1(a)$的补集，并计算在$\mathfrak{g}$中0的开邻域U上定义的G的指数映射。我们可以选择 U 使得 exp(U $\cap \mathfrak{g}^1(a)$)$\subset H$。 映射 $f: (x, y) \rightarrow$ (exp $x$, exp $y$) 是$\mathfrak{g}^1(a)\times \mathfrak{m}$ 中$(0,0)$ 的邻域上的解析映射和$H\times G$ 中的值。到引理 3 时，$f$ 与映射 $\varphi : (b, c) \rightarrow cabc^{-1}$ 的复合结果为 $(0,0)$。由此可见，$\varphi$ 是$f(0,0) = (e, e)$ 处的淹没。

#### 命题 5 {#lie-vii-s4-prop-5 .statement tag=00W4}

设 $a\in G$ 并令 W 为 G 中 $e$ 的邻域。存在 $a$ 的邻域 V 以及以下性质：对于所有 $a'\in V$，存在元素 $g\in W$ 使得$\mathfrak{g}^1(a')\subset$ 广告($g$)$\mathfrak{g}^1(a)$。

放入$\mathfrak{g}^1=\mathfrak{g}^1(a)$并令$\mathfrak{g}=\mathfrak{g}^1+\mathfrak{g}^+$为Ad($a$)$-1 ($§1, no. 1)的Fitting 分解。设 H 是 G 的谎言子群胚芽，具有李代数 $\mathfrak{g}^1$。对于所有 $h\in H$，Ad($h$)$\mathfrak{g}^1\subset \mathfrak{g}^1$。从$[\mathfrak{g}^1,\mathfrak{g}^+]\subset \mathfrak{g}^+$开始，H中存在$e$的邻域U，使得对于所有$h\in H$来说Ad($h$)$\mathfrak{g}^+\subset \mathfrak{g}^+$。由于Ad($a$)$-1$到$\mathfrak{g}^+$的限制是双射的，因此可以选择U使得Ad($ah$)$-1$到$\mathfrak{g}^+$的限制对于所有$h\in U$都是双射的。然后 $\mathfrak{g}^1(ah)\subset \mathfrak{g}^1(a) =\mathfrak{g}^1$ 代表所有 $h\in U$。通过命题 4，Int(W)($aU$) 是 G 中 $a$ 的邻域。如果 $a'\in$ Int(W)($aU$)，则 $a'=g(ah)g^{-1}$ 与 $g\in W$ 和 $h\in U$；由此可知 $\mathfrak{g}^1(a') =$ Ad($g$)$\mathfrak{g}^1(ah)\subset$ Ad($g$)$\mathfrak{g}^1(a)$。

#### 推论{#lie-vii-s4-n2-cor-1 .statement tag=00W5}

令$G^*$为G的开子群。如果$a\in G$是正则，则存在$a$的邻域V，使得对于所有$a'\in V,\mathfrak{g}^1(a')$来说，在Ad($G^*$)下，共轭到$\mathfrak{g}^1(a)$。

### 3. 关系与正则元素的李代数

#### 命题 6 {#lie-vii-s4-prop-6 .statement tag=00W6}

令V为$\mathfrak{g}$的开子群，并令exp$: V\rightarrow G$为在V上定义的指数映射。

(i) V 中存在 0 的邻域 W，使得对于所有 $x\in W$ 都有 $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$。

(ii) 如果 $k=\mathbf{R}$ 或 $\mathbf{C},\mathfrak{g}^1$(exp $x$)$\supset \mathfrak{g}^0(x)$ 对于所有 $x\in \mathfrak{g}$。

由科.第 8 章提案 3 III, §4, no. 4，V中存在 0 的邻域 $V'$，因此，对于所有 $x\in V'$，定义了 exp(ad($x$)) $=\sum_{n=0}^{\infty}\frac{1}{n!}$ ad($x$)$^n$ 并且 Ad(exp $x$) $=$ exp(ad($x$)).如果$P\in k[X]$和$\alpha \in$结束($\mathfrak{g}$)，很容易检查$\mathfrak{g}^{\lambda}(\alpha )\subset \mathfrak{g}^{P(\lambda)}(P(\alpha ))$对于所有$\lambda \in k$。因此，

$\mathfrak{g}^0$(广告($x$))$\subset \mathfrak{g}^1$(exp(广告($x$)))$=\mathfrak{g}^1$(广告(exp $x$))$=\mathfrak{g}^1$(exp $x$)

对于所有$x\in V'$。如果$k=\mathbf{R}$或$\mathbf{C}, V =\mathfrak{g}$，我们可以取$V'$ = V，这就证明了(ii)。我们证明（i）。令 U 为 End($\mathfrak{g}$) 中的 0 的邻域，这样为所有 $\alpha \in U$ 定义了 Log(1 $+\alpha$ ) $=\sum_{n>0}(-1)^{n+1 1}_{\overline{n}}\alpha^n$。然后 Log $\circ$ exp = 1 on 邻域 of 0 和 $\mathfrak{g}^1(1 +\alpha )\subset \mathfrak{g}^0$(Log(1 $+\alpha$ )) 对于所有$\alpha \in U$。令 W 为那些 $x\in V'$ 的 $\mathfrak{g}$ 由……组成中的 0 的邻域，使得 exp ad $x\in 1 + U$ 并且

Log(exp(广告($x$))) $=$广告($x$)。

然后，对于所有 $x\in W$，

$\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^1$(广告(exp $x$)) $=\mathfrak{g}^1$(exp(ad($x$)))

$\subset \mathfrak{g}^0$（日志（exp（广告（$x$））））$=\mathfrak{g}^0$（广告（$x$））$=\mathfrak{g}^0(x)$。

这表明对于所有 $x\in W$，$\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$。

#### 引理 4 {#lie-vii-s4-lem-4 .statement tag=00W7}

令 U 为 $\mathfrak{g}$ 中 0 的邻域，并用从 U 到 G 的指数映射，在 U 的每点处进行 étale，并且对于所有 $x\in U$，$\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$。

(i) 函数 $r^0_{Ad}$ 是常数，并且等于 exp(U) 上 $\mathfrak{g}$ 的秩。

(ii) 如果$x\in U$，exp $x$是正则当且仅当$x$是$\mathfrak{g}$的正则元素。

(iii) 元素 $a\in$ exp(U) 是正则当且仅当 $\mathfrak{g}^1(a)$ 是 $\mathfrak{g}$ 的嘉当子代数。

设 $l=$ rk($\mathfrak{g}$)。如果$x\in U$是$\mathfrak{g}$中的正则元素，

$r_{Ad}$（经验$x$）$=$暗淡$\mathfrak{g}^1$（经验$x$）$=$暗淡$\mathfrak{g}^0(x) =l$。

由于$\mathfrak{g}$属于的正则元素到U构成了$x$的邻域，并且exp在$x$处是étale，这表明exp$x$是正则的并且$r^0_{Ad}$(exp$x$)$=l$。 $\mathfrak{g}$ 属于的正则元素到 U 在 U 中是稠密的，对于所有 $a\in$ exp(U)，我们有 $r^0_{Ad}(a) =$ $l$。令 $a\in$ exp(U) 为 G 的正则元素，并令 $x\in U$ 使得 $a=$ exp $x$。从$\mathfrak{g}^0(x) =\mathfrak{g}^1(a)$开始，昏暗$\mathfrak{g}^0(x) =r^0_{Ad}(a) =l$。因而，$x$是$\mathfrak{g}$的正则元素，$\mathfrak{g}^1(a)$是$\mathfrak{g}$的嘉当子代数。最后，如果 $a\in$ exp(U) 和 $\mathfrak{g}^1(a)$ 是嘉当子代数 of $\mathfrak{g}$，

$r_{Ad}(a) =$ 暗淡$\mathfrak{g}^1(a) =l=r_{Ad}^0(a)$，

所以 $a$ 是常规的。

#### 命题 7 {#lie-vii-s4-prop-7 .statement tag=00W8}

令V为G中$e$的邻域。$\mathfrak{g}$的每个嘉当子代数都是形式$\mathfrak{g}^1(a)$，其中$a$是G属于到V的正则元素。

根据命题6，$\mathfrak{g}$中存在0的开邻域U和引理4的指数映射exp$: U\rightarrow G$满足条件。如果$\mathfrak{h}$是$\mathfrak{g}$的嘉当子代数，则存在正则元素$x\in \mathfrak{h}$使得$\mathfrak{h}=\mathfrak{g}^0(x) ($§3，Th。 2）。另一方面，存在元素$t\in k^*$使得$tx\in U$和exp($tx$)$\in V$。那么 $\mathfrak{h}=\mathfrak{g}^0(x) =\mathfrak{g}^0(tx) =\mathfrak{g}^1$(exp($tx$))，到引理 4 (ii)，exp($tx$) 就是 G 的正则元素。

#### 命题 8 {#lie-vii-s4-prop-8 .statement tag=00W9}

令 $l$ 为 $\mathfrak{g}$ 的秩。存在 G 的开子群 $G^*$ 使得：

(i) 函数 $r^0_{Ad}$ 在 $G^*$ 上恒定，其值为 $l$；

(ii) 元素 $a\in G^*$ 是正则当且仅当 $\mathfrak{g}^1(a)$ 是 $\mathfrak{g}$ 的嘉当子代数；

(iii) 如果$a\in G^*$，则$\mathfrak{g}^1(a)$的每个嘉当子代数是$\mathfrak{g}$的嘉当子代数。

(i) 根据命题 6，$\mathfrak{g}$ 中存在 0 的开邻域 U，以及从 U 到 G 满足条件引理 4 的指数映射 exp。在下文中，$G^*$ 将表示 G 的恒等分量，如果 $k=\mathbf{R}$ 或如果$k$是超度量的，则$\mathbf{C}$和包含在exp(U)中的G的开子群。由于 $r_{Ad}^0$ 是局部常数，并且其在 exp(U) 的任意点处的值为 $l$ (引理 4 (i))，因此 $r_{Ad}^0$ 是常数并且等于 $G^*$ 上的 $l$。

(ii) 令$R^*$（或$S^*$）为$G^*$的正则元素的集合（或元素$a\in G^*$的集合，使得$\mathfrak{g}^1(a)$为$\mathfrak{g}$的嘉当子代数）。然后$S^*\subset R^*$。事实上，如果$a\in S^*$，则$r_{Ad}(a) =l=r^0_{Ad}(a)$。我们证明$R^*\subset S^*$。如果 $k$ 是超量度的，则由包含 $G^*\subset$ exp(U) 和引理 4 (iii) 得出。假设$k=\mathbf{C}$。由科。根据第5条，如果$a\in R^*$，那么对于$a,\mathfrak{g}^1(a')$的每一个$a'$、属于到邻域，就是共轭到$\mathfrak{g}^1(a)$乘以$\mathfrak{g}$的自同构。这就证明$S^*$和$R^*$ **--** $S^*$对$G^*$开子集。我们已经看到，$e$的邻域中的$S^*$包含全部正则元素（引理4（iii））；因而，$S^*$非空。由于 $G^*$ 是连通的，因而 $R^*$（命题 1）也是连通的，因而 $S^*= R^*$ 也是连通的。

案例$k=\mathbf{R}$还有待研究。首先假设$G^*$是$\mathbf{G}\mathbf{L}(E)$的积分子群，其中E表示有限维实数向量空间。令$G^*_c$为$\mathbf{G}\mathbf{L}(E\otimes_{\mathbf{R}}\mathbf{C})$与李代数$\mathfrak{g}_c=\mathfrak{g}\otimes \mathbf{C}$的积分子群。 $G^*_c$上存在解析函数，其零的集合是$G^*_c$的正则元素的开集合的补集。通过可微分和解析流形，结果，3.2.5，这个函数不能在$G^*$的每点消失。因而，$G^*$包含正则元素$G^*_c$。设 Ad$_c$ 为$G^*_c$ 的伴随表示。对于任何 $a\in G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$，因而 $r_{Ad_c}(a) =r_{Ad}(a)$。如果$a\in G^*$是$G^*_c$中的正则元素，则这是$G^*$和$r_{Ad}^0(a) =r_{Ad}^0(a)$中的正则元素。 函数$r^0_{Ad}$和$r_{Ad}^0$分别在$G^*_c$和$G^{^c*}$上恒定，因而$G^*$的正则元素$^{^c}$是$G^*_c$属于的正则元素到$G^*$。由上式可知，若$a$为$G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$的正则元素则为$\mathfrak{g}_c$的嘉当子代数；这意味着$\mathfrak{g}^1(a)$是$\mathfrak{g}($§2的嘉当子代数，命题3）。

现在假设 G 是单连通的。存在一个有限维实数向量空间 E 和一个从 G 到 $\mathbf{G}\mathbf{L}(E)$ 的积分子群 $G'$ 的 étale 态射 $f$（第 III, §6, no. 1 章，Cor. of Th. 1）。根据命题 2，如果 $a\in G$ 是正则，则 $f(a)$ 也是正则。由上可知，${\mathfrak{g}'}^1(f(a))$是$G'$的李代数$\mathfrak{g}'$之嘉当子代数。由于${\mathfrak{g}'}^1(f(a)) = (Tf)\mathfrak{g}^1(a)$和$Tf$从$\mathfrak{g}$到$\mathfrak{g}'$是同构，因此证明$\mathfrak{g}^1(a)$是$\mathfrak{g}$的嘉当子代数。

我们最后转向一般情况$(k=\mathbf{R})$。令$\widetilde{G}$是$G^*, \widetilde{\mathfrak{g}}= L( \widetilde{G})$的通用覆盖，$q$是从$\widetilde{G}$到$G^*$的规范映射。由于$q$的核包含在$\widetilde{G}$的中心中，因此如果$a\in G^*$是正则且$a'\in q^{-1}(a)$，则$a'$是正则（命题2）。由上可知，$\widetilde{\mathfrak{g}}^1(a')$是$\widetilde{\mathfrak{g}}$中的嘉当子代数。由于$\mathfrak{g}^1(a) = (Tq)\widetilde{\mathfrak{g}}^1(a')$并且由于从$\widetilde{\mathfrak{g}}$到$\mathfrak{g}$$Tq$是同构，这证明$\mathfrak{g}^1(a)$是$\mathfrak{g}$的嘉当子代数。

(iii) 根据命题 5，存在 $a$ 的邻域 V，使得对于所有 $a'\in V,\mathfrak{g}^1(a')$ 来说，$\mathfrak{g}^1(a)$ 的共轭到子代数乘$\mathfrak{g}$ 的自同构。由于$a$包含正则元素$G^*$的每个邻域，从(ii)可以得出$\mathfrak{g}$的$\mathfrak{g}^1(a)$包含嘉当子代数。因此，根据§3的第3条，$\mathfrak{g}^1(a)$的每嘉当子代数就是$\mathfrak{g}$的嘉当子代数。

#### 注 {#lie-vii-s4-n3-rem-1 .statement tag=00WA}

如果$k=\mathbf{C}$、子代数$\mathfrak{g}^1(a)$，对于$a$正则和属于到G的连通分量M，在Int($\mathfrak{g}$)下是共轭。事实上，令 R 为 G 的正则元素的集合。对于所有 $a\in R\cap M$，令 $M_a$ 为那些 $b\in R\cap M$ 的集合，使得 $\mathfrak{g}^1(a)$ 为 Int($\mathfrak{g}$) 下的共轭至 $\mathfrak{g}^1(a)$。我们有 Int($\mathfrak{g}$) $=$ Ad(G$^0$)，其中 $G^0$ 是 G 的恒等分量。根据命题的推论，$5, M_a$ 在 R 中是开的。因此，$M_a$ 在 R 中是开和闭的。因为 $k=\mathbf{C}, R\cap M$ 是连通的 (引理) 1)，因此$M_a= R\cap M$。

### 4. 小学应用自同构

#### 命题 9 {#lie-vii-s4-prop-9 .statement tag=00WB}

令$k$为特征0的域，并且$\mathfrak{g}$李代数超过$k$。如果$a\in$Aut$_e(\mathfrak{g})$，则$a-1$的零空间的维数大于或等于$\mathfrak{g}$的秩。

根据“Lefschetz 原理”（代数，V, §14, no. 6，第$5$的Cor.2）$,k$是子域$(k_i)_{i\in I}$的升序有向并，承认$\mathbf{C}$为扩张域。令$(e_{\alpha})$为$\mathfrak{g}$的基超过$k$和$x_1, . . . , x_m$元素为$\mathfrak{g}$，这样ad($x_1$)$, . . .$、ad($x_m$)是幂零的且$a=e^{ad(x_1)}. . . e^{ad(x_m)}$。令$c^{\gamma}_{\alpha \beta}$为$\mathfrak{g}$相对于基$(e_{\alpha})$的结构常数，$(x^{\alpha}_r)$相对于基$(1\leq r\leq m)$的$x_r$的分量。存在指标$j\in I$，使得$c^{\gamma}_{\alpha \beta}$和$x^{\alpha}_r$都是属于到$k_j$。让$\mathfrak{g}_j=\sum_{\alpha}k_je_{\alpha}$；

这是李代数超过$k_j$包含$x_1, . . . , x_m$，$a$到$\mathfrak{g}_j$的限制$a_j$是$\mathfrak{g}_j$的初等自同构。 $a_j$到$\mathfrak{g}_j\otimes_{k_j}\mathbf{C}$的扩张是$\mathfrak{g}_j\otimes \mathbf{C}$的初等自同构$a_j\otimes 1$。因此，让$G_j$是李群与李代数$\mathfrak{g}_j\otimes \mathbf{C}$和$G_j$的$s$元素，使得Ad($s$)$=a_j\otimes 1$。命题 8，应用于对 $(G_j, s)$，表明 $a_j\otimes 1-1$ 的零空间为维数 $n$，所以

$n\geq$ rk($\mathfrak{g}_j\otimes \mathbf{C}$) $=$ rk($\mathfrak{g}_j$) $=$ rk($\mathfrak{g}$)。

但是这个零空间与$a_j-1$和$a-1$具有相同的维数。因此命题。

### 习题 {#lie-vii-s4-exercises}

记号和假设是第 1 号。 §4 的 1、2、3。

§ 4](exercises/s4/)参见[习题。
