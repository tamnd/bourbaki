---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 1
section_title: Premeasures and measures on a topological space
lang: zh
source: int-vii-ix
pdf_pages: 0183-0204, 0288-0289
extraction: ocr
subsections:
    - "no": 1
      title: Encumbrances
      page: 0
      pdf_page: 183
    - "no": 2
      title: Premeasures and measures
      page: 3
      pdf_page: 185
    - "no": 3
      title: Examples of measures
      page: 6
      pdf_page: 188
    - "no": 4
      title: Locally negligible sets and functions
      page: 8
      pdf_page: 190
    - "no": 5
      title: Measurable sets and functions
      page: 9
      pdf_page: 191
    - "no": 6
      title: Directed families; support of a measure
      page: 11
      pdf_page: 193
    - "no": 7
      title: Upper envelopes and sums of measures
      page: 12
      pdf_page: 194
    - "no": 8
      title: Crushings
      page: 13
      pdf_page: 195
    - "no": 9
      title: Upper integral
      page: 17
      pdf_page: 199
    - "no": 10
      title: Integration theory
      page: 20
      pdf_page: 202
statements: 52
exercises: 10
content_sha256: 0b05dd5e731e014f35835162505cb940efaaa3503f15d99bf771c57d417b3b68
translated_from: content/en/int/IX/01_s1_premeasures_and_measures_on_a.md
translation_method: google
source_content_sha256: 317fc43050baeab2bc8c0cb022963528cc65340ba4a1f70e587dec5228ab5967
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 97d2eb44f13e36f64f1a0b5ae4d7ed88584e47d4eb75b9033d9f52bcb568a913
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。拓扑空间上的预测量和测量

### 1. 负担

#### 定义 1 {#int-ix-s1-def-1 .statement tag=09MO}

— 令 T 为集合。我们将 T 上 $\mathscr{F}_+(T)$ 的任何映射 p 称为 $\overline{\mathbf{R}}_+$ ，其具有以下属性：
a) 如果 f 和 g 是 $\mathscr{F}_+$ 的两个元素，使得 $f \leq g$，则$p(f) \leq p(g)$。
b) 如果 f 是 $\mathscr{F}_+$ 的元素，并且 t 是数 $\geq 0$，则$p(tf) = tp(f)$。

c) *如果f和g是$\mathscr{F}_+$中的两个元素，则$p(f + g) \leq p(f) + p(g)$。*
d) *如果$(f_n)$是$\mathscr{F}_+$的元素递增序列，并且如果$f = \lim_{n \to \infty} f_n$，则$p(f) = \lim_{n \to \infty} p(f_n)$。*
*如果 A 是 T 的子集，我们写 $p(A)$ 而不是 $p(\varphi_A)$。*

条件 b) 意味着$p(0) = 0$。另一方面，设$(f_n)$为$\mathscr{F}_+$元素序列； 条件 c) 和 d) 意味着不等式

$$
p\left( \sum_n f_n \right) \leq \sum_n p(f_n)
$$

（可数凸性*不等式*）。

对于例，令T为局部紧致空间，$\mu$为T的正测度；那么 $\mu^*$ 和 $\mu^\bullet$ 是 T 上的负担。这是从 Props 得出的。 10、11、12 和 Th。第 3 章。 IV, §1, No. 3 对应 $\mu^*$，来自第 1 章第 1 章的提案 1。 V, §1, No. 1 $\mu^\bullet$。

#### 命题 1 {#int-ix-s1-prop-1 .statement tag=09MP}

*令 $(p_\alpha)_{\alpha \in A}$ 为 T 上的产权负担族。和和家庭 $(p_\alpha)$ 的上封套（在 $\mathscr{F}_+(\mathscr{F}_+(T))$ 中）则为产权负担。*

有限族负担中的和显然是一种负担，处理上封套的情况就足够了。 定义 1 的性质 a)、b)、c) 显然满足，仍有待建立 d)。 集合$p = \sup_\alpha p_\alpha$；然后，当记号为定义 1 d) 时，

$$
p(f) = \sup_\alpha p_\alpha(f) = \sup_\alpha \sup_n p_\alpha(f_n) = \sup_n \sup_\alpha p_\alpha(f_n) = \sup_n p(f_n).
$$

#### 定义 2 {#int-ix-s1-def-2 .statement tag=09MQ}

*设 p 为集合 T 上的负担。有人说，如果 $p(T) < +\infty$，则 p 是有界的。如果 T 是拓扑空间，则 p 被认为是局部有界的，前提是每个 $x \in T$ 都承认有一个邻域 V，使得 $p(V) < +\infty$。*

然后根据 Def 的属性 a) 和 c) 得出。 1 对于 T 的每个紧凑子集 K，$p(K) < +\infty$。特别是，如果 T 是紧凑的，则 T 上的每个局部有界负担都是有界的。

设 p 为集合 T 上的负担，A 子集为 T 的负担。对于每个函数 $f \in \mathscr{F}_+(A)$，令 $f^0$ 为扩张，f 到 T 的差为 0； $\mathscr{F}_+(A)$ 上的映射 $f \mapsto p(f^0)$ 是一种负担，称为由 A 上的 p* 引起的*负担，并表示为 $p|A$ 或 $p_A$。

设 T 和 U 是 T 到 U 的两个集合、$\pi$ 映射，并且 p 是 T 上的负担。 U 上的负担 $\pi(p)$，其 $f \in \mathscr{F}_+(U)$ 的值由下式给出

$$
(\pi(p))(f) = p(f \circ \pi),
$$

称为$\pi$下$p$的*像负担*。

让$p$成为集合$T$的负担；如果$p(T - A) = 0$，则据说$p$“集中”在子集$A$或$T$。

#### 引理 1 {#int-ix-s1-lem-1 .statement tag=09MR}

— *如果产权负担$p$集中在$A \subset T$，则每$f \in \mathscr{F}_+(T)$就有$p(f) = p(f \varphi_A)$。*

对于，集合$T - A = B$，使得$p(\varphi_B) = 0$；那么

$$
f \varphi_B \leq (+\infty) \cdot \varphi_B = \sup_{n \in \mathbf{N}} n \varphi_B,
$$

因此 $p(f \varphi_B) = 0$ 由 Def 的属性 $a), b), d)$ 得到。 1. 从c)得出$p(f) \leq p(f \varphi_A) + p(f \varphi_B) = p(f \varphi_A)$，最后由a)得出$p(f) = p(f \varphi_A)$。

### 2. 预防措施和措施

令$T$为拓扑空间，并令$\mathfrak{K}$为$T$的紧凑子集的集合，按包含排序。对于每个$K \in \mathfrak{K}$，令$\mathscr{M}(K; \mathbf{C})$为$K$上的复杂测度的集合。对于$\mathfrak{K}$的元素的每个对$(K, L)$使得$K \subset L$，令$\iota_{KL}$为$\mathscr{M}(L; \mathbf{C})$的映射到$\mathscr{M}(K; \mathbf{C})$，与$L$上的每个测度$\mu$相关联$\mu_K$ 由 $K$ 上的 $\mu$ 诱发（第 IV, §5, No. 7 章，定义 4）。那么$\iota_{KM} = \iota_{KL} \circ \iota_{LM}$，当$K, L$和$M$是$T$的紧子集，使得$K \subset L \subset M$；这是从诱导措施传递性得出的（第V, §7, No. 2章，第4条命题）。族$(\mathscr{M}(K; \mathbf{C}))_{K \in \mathfrak{K}}$的*逆极限*的元素针对映射$\iota_{KL}$的元素将在$T$被称为*预防措施*。其他字：

#### 定义 3 {#int-ix-s1-def-3 .statement tag=09MS}

*One calls premeasure on a topological space $T$ every mapping $w$ that associates, to every compact subset $K$ of $T$, a measure $w_K$ on $K$, and that has the following property:

*如果$K$和$L$是$T$的紧子集使得$K \subset L$，$w_L$在$K$上引起的测度$(w_L)_K$等于$w_K$。

如果所有度量 $w_K$ 都是真实的（分别为正），则预测量 $w$ 被称为真实（分别为正）。*

设$w$和$w'$为$T$、$t$复数的两个预测值；对于$T$的每个紧凑子集$K$，预防措施$w + w'$和$tw$由公式$(w + w')_K = w_K + w'_K$、$(tw)_K = tw_K$定义。对$T$的预制显然是形式向量空间，记为$\mathscr{P}(T; \mathbf{C})$；实际预测值的空间将表示为$\mathscr{P}(T; \mathbf{R})$，或更常见的是$\mathscr{P}(T)$，正预测值的凸锥将表示为$\mathscr{P}_+(T)$。令 $w$ 为预测值； 映射 $K \mapsto |w_K|$ 是 $T$（第 IV, §5, No. 7、引理 3）的预测值，将表示为 $|w|$。若 $w$ 为实数，则集合 w^+ = \frac{1}{2}(|w| + w),\ w^- = \frac{1}{2}(|w| - w);这两个预测值是正的，我们可以看到每一个真正的预测值都是两个正预测值的差值。显然，对于 T 的每个紧凑子集 K，$(w^+)_K = (w_K)^+$、$(w^-)_K = (w_K)^-$。

向量空间 $P(T)$ 按圆锥$P_+(T)$ 排序。显然$w^+ = \sup(w, 0),\ w^- = \sup(-w, 0)$；因而，$P(T)$ 是晶格有序的，$\sup(w, w') = w + (w' - w)^+,\ \inf(w, w') = w - (w' - w)^-$ 是晶格有序的。而且，明确

$$
(\sup(w, w'))_K = \sup(w_K, w'_K),\quad (\inf(w, w'))_K = \inf(w_K, w'_K)
$$

对于 T 的每个紧凑子集 K。

#### 定义 4 {#int-ix-s1-def-4 .statement tag=09MT}

*令 w 为 T 的正预测值。对于每个函数 $f \in \mathscr{F}_+(T)$，我们应集合，*

$$(1)$$
$$
w^\bullet(f) = \sup_K (w_K)^\bullet(f_K),
$$

*其中 K 运行于 T 的紧凑子集的集合。*

对于每个紧集 K，令$p^K$为K的典范嵌入下的负担$(w_K)^\bullet$的像负担进入T； $w^\bullet$ 是产权负担 $p^K$ 的上封套，因此是产权负担（No. 1，命题 1）。有人说 $w^\bullet$ 是与正预测值 w 相关的“基本上积分”。人们经常写$\int^\bullet f\, dw$或$\int^\bullet f(t)\, dw(t)$而不是$w^\bullet(f)$。

*注 1).* — 如果 v 和 w 是两个正预测值，则 $(v + w)^\bullet = v^\bullet + w^\bullet$（第 V, §1, No. 1 章，命题 3）。如果 v 和 w 是两个复数预测值，则 $|v + w|^\bullet \leq |v|^\bullet + |w|^\bullet$。

#### 命题 2 {#int-ix-s1-prop-2 .statement tag=09MU}

*a) 令 w 为正预测值。对于 T 的每个紧凑子集 K，$w^\bullet$ 在 K 上引起的负担 $(w^\bullet)_K$ 等于 $(w_K)^\bullet$。对于每一个函数 $f \in \mathscr{F}_+(T)$，一个人有关系 $(w_K)^\bullet(f_K) = w^\bullet(f_{\varphi_K})$ 并且*

$$(2)$$
$$
w^\bullet(f) = \sup_K w^\bullet(f_{\varphi_K}).
$$

*b) 相反，令 p 为 T 满足以下条件的负担：
1) 对于 T 的每个紧致子集 K，K 上存在一个正测度 $w_K$，使得 $p_K = (w_K)^\bullet$。
2) 对于每个函数$f \in \mathscr{F}_+(T)$，$p(f) = \sup_K p(f_{\varphi_K})$。
映射 $w : K \mapsto w_K$ 是 T 的正预测值，$p = w^\bullet$。

让我们证明$a$：令$g \in \mathscr{F}_+(K)$和$g^0$乘以$g$到$T$的零为扩张；那么，通过定义的诱发产权负担，

$$
(w^\bullet)_K(g) = w^\bullet(g^0) = \sup_L (w_L)^\bullet(g^0|L),
$$

其中$L$运行超过$T$的紧凑子集的集合，或者仅仅运行包含$K$的集合。但如果$L$包含$K$，则$(w_L)^\bullet(g^0|L) = (w_K)^\bullet(g)$来自$g^0|L$是零在$K$之外（第V, §7, No. 1，命题1），这证明了第一个断言。因此

$$
(w_K)^\bullet(f_K) = (w^\bullet)_K(f_K) = w^\bullet((f_K)^0) = w^\bullet(f_{\varphi_K})
$$

对于所有$f \in \mathscr{F}_+(T)$，并且（2）仅翻译公式（1）。

让我们转到 $b$：1) 中考虑的度量 $w_K$ 是唯一的（第 V, §1, No. 1 章）。让我们证明映射$K \mapsto w_K$是一个预测量：让$K$和$L$是两个紧凑的子集使得$K \subset L$，并让$\lambda$是$w_L$在$K$上引起的测度；一切都归结为展示$\lambda^\bullet = (w_K)^\bullet$。现在，$\lambda^\bullet = ((w_L)^\bullet)_K$（第 V, §7, No. 1 章，提案 1）；从$(w_L)^\bullet = p_L$开始，我们有$\lambda^\bullet = (p_L)_K = p_K = (w_K)^\bullet$。

让我们用$w$表示预测值$K \mapsto w_K$；从$p_K = (w_K)^\bullet = (w^\bullet)_K$开始，我们有$p(f_{\varphi_K}) = p_K(f_K) = (w^\bullet)_K(f_K) = w^\bullet(f_{\varphi_K})$。因此，由于$p$上的公式 (2) 和假设 2)，两个产权负担$p$和$w^\bullet$相等。

Q.E.D.

由于诱发的负担$(w^\bullet)_K$等于$(w_K)^\bullet$，因此简单地写成$w_K^\bullet$不会产生歧义。从现在开始我们就使用这个记号。

#### 推论{#int-ix-s1-n2-cor-1 .statement tag=09MV}

— *令$v$和$w$为$T$的两个正预测值，使得$v^\bullet(L) = w^\bullet(L)$对于$T$的每个紧凑子集$L$；然后$v = w$。特别是，关系$v^\bullet = w^\bullet$意味着$v = w$*。

例如，令$T$中的$K$为紧集；每有紧集 $L \subset K$，就有关系

$$
w_K(L) = w_K^\bullet(L) = w^\bullet(L) = v^\bullet(L) = v_K^\bullet(L) = v_K(L)
$$

根据提案 2；因此 $w_K = v_K$（第 IV, §4, No. 10 章，第 19 号提案第 3 条），最后由定义预防措施$w = v$。

#### 定义 5 {#int-ix-s1-def-5 .statement tag=09MW}

— *令 $w$ 为拓扑空间 $T$ 的预测值。如果负担 $|w|^\bullet$ 是局部有界（或有界）的，则可以说 $w$ 是一种测度（或有界测度）（cf. No. 1，定义 2）*。

$T$上的复杂测度的集合显然是向量空间（*注* 1），将其表示为$\mathscr{M}(T; \mathbf{C})$。实际措施的空间将表示为$\mathscr{M}(T; \mathbf{R})$或更常见的是$\mathscr{M}(T)$，积极措施的锥体将表示为$\mathscr{M}_+(T)$。

如果 $w$ 是复测度，则其实数部分和虚数部分均为实测度。如果$w$是实测度，则$w^+$和$w^-$是正测度。因此，每个复杂（或实际）测量都是线性组合（或差异）的正测量。

#### 注 2 {#int-ix-s1-n2-rem-2 .statement tag=09MX}

如果 $T$ 是*局部紧凑*，则 $T$ 上的每个预测值 $w$ 都是一个测度。因为，每个$x \in T$都承认一个紧凑邻域$K$和$|w|^*(K) = \|w_K\| < +\infty$，因此负担$|w|^*$是局部有界的。

#### 注 3 {#int-ix-s1-n2-rem-3 .statement tag=09MY}

对于 $T$ 的每个 Borel 子集 $A$（特别是 $A = T$）和$T$ 上的每个正措施$\mu$，数 $\mu^*(A)$ 是契约措施$\mu^*(K)$ 的至高子集共 $A$。事实上，对于 $A$ 的每一个紧凑子集 $K$，都有 $\mu^*(K) \leq \mu^*(A)$；另一方面，如果$\mathfrak{K}$是$T$的紧凑子集的集合，那么

$$
\mu^*(A) = \sup_{K \in \mathfrak{K}} \mu_K^*(A \cap K) = \sup_{K \in \mathfrak{K}} \sup_{L \in \mathfrak{K}, L \subset A \cap K} \mu_K^*(L) \leq \sup_{L \in \mathfrak{K}, L \subset A} \mu^*(L)
$$

由科. 1 Th。第 4 章。 IV, §4, No. 6。

### 3. 例措施

#### 例 1 {#int-ix-s1-n3-exa-1 .statement tag=09MZ}

— *局部紧凑空间的措施。*

下面的命题表明了这个章包含的理论。 IV。在叙述中，字“测量”和记号 $\mathscr{M}(T; \mathbf{C})$ 的含义与之前的章相同。

#### 命题 3 {#int-ix-s1-prop-3 .statement tag=09N0}

*令$T$为局部紧致空间，令$\mu$为$T$的测度。用 $W(\mu)$ 映射表示，它与 $T$ 的每个紧凑子集 $K$ 相关联，导出测度 $\mu_K$。那么$W(\mu)$是$T$上的一项预测，一个有$W(|\mu|) = |W(\mu)|$，线性映射$W : \mu \mapsto W(\mu)$是空间$\mathscr{M}(T; \mathbf{C})$的双射到空间$\mathscr{P}(T; \mathbf{C})$上的预测$T$。此外，如果$\mu$为正，则$\mu^* = (W(\mu))^*$。

很明显，$W(\mu)$ 是预测值（第 V, §7, No. 2，命题 4），映射 $W$ 是线性的。 关系 $W(\mu) = 0$ 表示 $\mu$ 诱导 $T$ 中每个紧集的测度 0；那么$\mu(f) = 0$对应$f \in \mathscr{H}(T; \mathbf{C})$，因此$\mu = 0$，这证明$W$是单射的。仍有待证明 $W$ 是满射。由于每个预测值都是线性组合的正预测值，因此对于每个“正”预测值 $w$，一个正值 $\mu$ 就足以构造，从而使得 $w = W(\mu)$。令$f \in \mathscr{H}(T)$为给定的函数，令$L$为紧集包含$f$的支持度； 数 $w_L(f_L)$ 独立于$L$ 的选择，通过定义的诱导措施，因此可以集合 $\mu(f) = w_L(f_L)$；那么$\mu$是$\mathscr{H}(T)$上的正线性形式，即正测度。让我们验证一下$w = W(\mu)$；首先，关系$\mu^\bullet(f) = w_L^\bullet(f_L)$扩展到$f$是有限上半连续函数，且零在$L$之外。例如，令$M$是$L$的紧邻域，$\mathscr{H}$是$T$上连续函数的（递减有向）集合，$M$包含支持，即$\geq f$。然后（第 IV, §4, No. 4 章，第 5 号提案第 2 条）

$$
\mu^\bullet(f) = \inf_{h \in \mathscr{H}} \mu(h) = \inf_{h \in \mathscr{H}} w_M(h_M) = w_M^\bullet(f_M),
$$

另一方面，$w_M^\bullet(f_M) = w_L^\bullet(f_L)$，因为$f_M$在$M - L$上是零（第V, §7, No. 1章，提案1）。特别是，如果通过$\mathscr{H}_+(L)$的元素的0取$f$为扩张，那么这个公式表明$\mu_L = w_L$通过定义的诱导措施，因此确实是$W(\mu) = w$。

如果 $\mu$ 为正，则

$$
\mu^\bullet(f) = \sup_K \mu^\bullet(f \varphi_K) = \sup_K \mu_K^\bullet(f_K) = (W(\mu))^\bullet(f)
$$

对于每个$f \in \mathscr{F}_+(T)$（第V, §1，定义1和§7，提案1）。 关系 $|W(\mu)| = W(|\mu|)$ 是显而易见的（第 IV, §5, No. 7、引理 3）。

Q.E.D.

当$T$是*局部紧凑*时，我们从现在开始将通过双射$W$*认同*空间$\mathscr{M}(T; \mathbf{C})$和$\mathscr{P}(T; \mathbf{C})$。

#### 例 2 {#int-ix-s1-n3-exa-2 .statement tag=09N1}

— *在拓扑空间上提供紧凑支持的措施。*

#### 引理 2 {#int-ix-s1-lem-2 .statement tag=09N2}

— *令$T$为拓扑空间，$L$为$T$的紧子集，$\lambda$为$L$的正测度。 $T$ 上存在唯一的正测度 $\mu$，这样，对于每一个函数 $f \in \mathscr{F}_+(T)$，*

(2)
$$
\mu^\bullet(f) = \lambda^\bullet(f_L).
$$

让我们对每个 $f \in \mathscr{F}_+(T)$ 集合 $p(f) = \lambda^\bullet(f_L)$，并证明命题 2 *b*) 的条件 1) 和 2) 得到满足。第二个显然是满足的：确实，如果$K$包含$L$，则$p(f) = p(f \varphi_K)$。如果 $K \subset T$ 是紧的，并且如果 $h \in \mathscr{F}_+(K)$，那么

$$
p_K(h) = p(h^0) = \lambda^\bullet(h^0|L).
$$

但$h^0|L$是扩张除$h_{K \cap L}$到$L$的0：因此最后一个表达式等于$(\mu_K)^\bullet(h)$，其中$\mu_K$是$K \cap L$的单射下的$\lambda|K \cap L$的像进入$K$（第1章） V, §6, No. 2，提案 2 和 §7, No. 1，提案 1)，以及 $p_K = (\mu_K)^\bullet$。因此，命题 2 *b*) 的条件 1) 也成立，$\mu$ 的存在性随之而来。

Q.E.D.

我们可以说 $\mu$ 是由 $\lambda$ *定义*的 T 测度。特别是，对于 T 的每点 $x$，可以定义测量$\varepsilon_x$；它的特征是$(\varepsilon_x)^*(f) = f(x)$为$f \in \mathscr{F}_+(T)$。

#### 注 {#int-ix-s1-n3-rem-1 .statement tag=09N3}

— 1) 当 T 是局部紧致时，$\mu$ 是 $\lambda$ 的像在 L 的单射下进入 T。我们将在 §2, No. 3，*例* 中看到，当像度量被处理时，这种解释对于任意空间仍然有效。
2) 我们还将看到，*例* 2 中定义的测度是具有紧凑支持的 T 上的正测度（No. 6，*注* 2））。

*今后我们将只考虑积极措施，除非明确提及相反的措施。对于截面的其余部分，T 将表示拓扑空间，而 $\mu$ 则表示 T 上的正测度。*

以下小节中的许多结果可以扩展到积极的预防措施。这个扩张就留给读者了。

### 4. 局部可忽略不计集合和函数

#### 定义 6 {#int-ix-s1-def-6 .statement tag=09N4}

*函数* $f \in \mathscr{F}_+$（分别为*子集* A *of* T）*据说对于测量来说局部可忽略不计* $\mu$ *if* $\mu^*(f) = 0$（分别为$\mu^*(A) = 0$）。 *有人说* $\mu$ *集中在子集* A *of* T *如果* T − A *是局部* $\mu$*-可忽略*。

#### 注 {#int-ix-s1-n4-rem-1 .statement tag=09N5}

— 1) 当 T 是局部紧的时，如此定义的概念重合具有通常的概念。
2）之后我们已经定义了*可忽略*集合，我们将看到局部可忽略的集合确实是那些其胚芽，在T的每点处，是可忽略的集合的胚芽（No. 9，第14号提案的Cor.2）。
3）如第 1 章所示。 IV和V，表达“局部几乎无处不在”将与“除了局部可忽略不计的集合”同义。
4）如果$\theta$是一个复杂的测度，我们可以说函数（T的子集）对于$\theta$来说是局部可忽略的，如果对于正测度$|\theta|$也是如此。

#### 例 {#int-ix-s1-n4-exa-1 .statement tag=09N6}

— 令 L 为 T 的紧凑子集，$\lambda$ L 上的测度，$\mu$ $\lambda$ (No. 3, *例* 2) 定义的 T 上的测度。 公式 (3) 立即意味着函数 $f \in \mathscr{F}_+(T)$ 局部 $\mu$ 可以忽略不计，当且仅当 $f_L$ 是 $\lambda$ 可以忽略不计。

紧接着从公式 (1) 可以得出，函数 $f \in \mathscr{F}_+(T)$ 是局部 $\mu$ 可以忽略的，当且仅当 $f_K$ 对于 T 的每个紧致子集 K 来说，$\mu_K$ 是可以忽略的。因此，局部可忽略的集合约化的性质立即变为那些紧凑空间中可忽略不计的集合，在第 1 章中处理。 IV。以下是一些今后将使用的结果，不再进一步参考。

— 为了使函数 $f \geqslant 0$ 局部可忽略不计，$f(t) = 0$ 局部几乎处处都是必要且充分的（Ch. IV, §2, No. 3，Th. 1）。如果 $f$ 是函数，而 Banach 空间中的值，则相当于说 $f = 0$ 几乎在任何地方都存在，或者$\mu^*(|f|) = 0$；在这种情况下，我们将再次说 $f$ 局部可以忽略不计。

— 局部可忽略的函数 $\geqslant 0$ 的和和序列的上包络线局部可忽略不计（*loc.cit.*，No. 1，提案 2）。

— 如果 $f$ 和 $g$ 是两个函数 $\geqslant 0$，并且几乎在任何地方都局部相等，则 $\mu^\bullet(f) = \mu^\bullet(g)$（*loc.cit.*，No. 3，第 6 条）。

### 5. 可测量集合和函数

#### 定义 7 {#int-ix-s1-def-7 .statement tag=09N7}

*函数* $f$ *定义于* $T$，*与值在拓扑空间* $F$（*豪斯多夫或非豪斯多夫*）*据说对于测量* $\mu$ *（或为* $\mu$*-可测量）*如果，*对于每个紧凑子集*$K$*的*$T$，*函数*$f_K$*是*$\mu_K$*-可测量*。

这相当于存在说，对于每个紧集$K$，将$K$的划分转化为$\mu_K$可忽略不计的集合$N$和序列$(K_n)$ 紧集，使得$f$到每个$K_n$的限制是连续的。因为它相当于说 $N$ 是 $\mu_K$-可忽略的，或者它是局部 $\mu$-可忽略的 (No. 4)，所以可以看出 $f$ 是 $\mu$-可测的，当且仅当，对于每个紧集 $K$，存在将$K$的划分转换为局部$\mu$可忽略的集合$N$和紧集的序列$(K_n)$，使得$f_{K_n}$对于所有$n$都是连续的。这个定义与Def相同。第 1 章。 IV, §5, No. 1，因此当$T$局部紧致时，我们恢复了可测量函数的通常概念。

如果函数的特征是可测量的，则$T$的子集$A$被认为是可测量的。当$A$是$\mu$可测量并且$\mu^\bullet(A) < +\infty$时，这个数简单地表示为$\mu(A)$并且被称为$A$的*测量*。当$f$是$\geqslant 0$、$\mu$可测量和$\mu^\bullet(f) < +\infty$时，类似地可以将$\mu^\bullet(f)$写为$\mu(f)$。

如果$\theta$是$T$上的复杂测度，则函数$f$（分别是$T$的子集）如果对于正测度$|\theta|$是可测的，则称其为$\theta$可测。下面的结果可以扩展到复杂的测量。

#### 例 {#int-ix-s1-n5-exa-1 .statement tag=09N8}

— Let $L$ be a compact subset of $T$, $\lambda$ a measure on $L$, and $\mu$ the measure on $T$ defined by $\lambda$ (No. 3, *Example 2*). 当且仅当$f_L$是$\lambda$可测时，在$T$上定义的函数$f$是$\mu$可测的。 因为，这个条件显然是必要的。 相反，如果满足，则存在$L$的划分到$\lambda$可忽略的集合$N$和紧集的序列$(L_n)$，使得$f_{L_n}$对于所有$n$都是连续的。 如果$K$是$T$的紧凑子集，集合$K - \bigcup^n (K \cap L_n)$有交和$L$，$\lambda$可忽略不计，因此集合是$\mu$可忽略不计No. 3的公式(3)，以及$f$到$K \cap L_n$的限制对于所有$n$都是连续的。

定义。 7 允许在没有新的证明的情况下，将可测量函数上的结果数扩展到空间非局部紧凑的情况。以下是其中的一些，我们将在以后使用而无需进一步参考：$T$的开集合和闭集合是$\mu$可测量的； $\mu$-可测量的集合形式一个部落（第IV, §5, No. 4，第2章的Cor.2），包含T的Borel集合（前述，第3章），以及Souslin集合（第2章） IV, §5, No. 1，第 3)(1) 条第 2 条。数值函数上的通常代数运算保持可测量性（第 IV, §5, No. 3 章），可数通道到极限的运算也保持可测量性（前述，No. 4，Th.2 和 Cor.1）。下面的性质值得更明确地提及：

#### 命题 4 {#int-ix-s1-prop-4 .statement tag=09N9}

— 令 $f$ 为 T 上 $\mu$ 的正函数和 $(g_n)_{n \geq 1}$ 序列 - 可测量正函数。设定 $g = \sum_{n \geq 1} g_n$，有

$$
\mu^\bullet(fg) = \sum_{n \geq 1} \mu^\bullet(fg_n).
$$

集合 $h_n = \sum_{i=1}^n g_i$ 对于所有 $n \geq 1$。对于 T 的每个紧凑子集 K，

$$
\mu_K^\bullet((fh_n)_K) = \sum_{i=1}^n \mu_K^\bullet((f g_i)_K)
$$

由第 2 章的提案 2将V, §1, No. 1应用于紧凑空间K。对于T的紧凑子集的递增有向集合，经过到极限，可得

$$
\mu^\bullet(fh_n) = \sum_{i=1}^n \mu^\bullet(f g_i).
$$

现在，$fg$是递增序列$(fh_n)_{n \geq 1}$、从而$\mu^\bullet(fg) = \lim_{n \to \infty} \mu^\bullet(fh_n)$的极限；前面的公式则立即暗示(4)。

#### 推论{#int-ix-s1-n5-cor-1 .statement tag=09NA}

— 令 $(A_n)$ 为成对不相交的可测量子集的序列，其中并 A。对于 T 的每个子集 B，

$$
\mu^\bullet(A \cap B) = \sum_n \mu^\bullet(A_n \cap B)
$$

特别是

$$
\mu^\bullet(A) = \sum_n \mu^\bullet(A_n).
$$

在可测量函数或集合以及扩展的性质中，如上文 Hausdorff 空间所示，我们还引用了第 1 章的第 12 章提案。 IV, §5, No. 8（$\mu$-紧集的密集族）。因此，函数 $f$ 和值在拓扑中

(1) 该推论的证明对于不可度量局部紧致空间 (GT, IX, §6, No. 9, Th. 5) 中的 Souslin 集合无需修改即可有效。

空间（Hausdorff 与否）是 $\mu$ 可测的，当且仅当 T 的紧凑子集 K 的集合，使得 $f_K$ 是连续的，是$\mu$-稠密的（*loc.cit.*，No. 10，命题 15）。

### 6. 定向家庭；对某项措施的支持

#### 命题 5 {#int-ix-s1-prop-5 .statement tag=09NB}

**a)** *设 H 为函数 $\geqslant 0$ 的递增有向集合，它们在 T 的每个紧凑子集上都是下半连续的。然后*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

*b)* *设H为函数$\geqslant 0$的递减有向集合，它们在T的每个紧致子集上是上半连续的。如果H中存在函数$h_0$使得$\mu^\bullet(h_0) < +\infty$，则*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

对于每个紧集 $K \subset T$，我们都有情况 *a)*

$$
\mu^\bullet \left( \sup_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \sup_{h \in H} h_K \right) = \sup_{h \in H} \mu_K^\bullet(h_K) = \sup_{h \in H} \mu^\bullet(h \varphi_K),
$$

如果是 *b)*

$$
\mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \mu_K^\bullet \left( \inf_{h \in H} h_K \right) = \inf_{h \in H} \mu_K^\bullet(h_K) = \inf_{h \in H} \mu^\bullet(h \varphi_K),
$$

根据 No. 2 的第 2 条提案和第 8 章的第 8 条提案V, §1, No. 2。情况 *a*) 紧随其后，通过关于 K 的上界（No. 2，命题 2）。为了处理情况 *b*)，用 $\varepsilon$ 数 $> 0$ 和选择紧集 K 表示，使得 $\mu^\bullet(h_0 \varphi_K) \geqslant \mu^\bullet(h_0) - \varepsilon$。然后我们有 (No. 5，命题 4) $\mu^\bullet(h_0 \varphi_{C_K}) \leqslant \varepsilon$；对于每个函数 $h \in H$ 即 $\leqslant h_0$，我们因此有 $\mu^\bullet(h \varphi_{C_K}) \leqslant \varepsilon$，最后根据 No. 5 的第 4 条命题得到 $\mu^\bullet(h \varphi_K) \geqslant \mu^\bullet(h) - \varepsilon$。因而

$$
\mu^\bullet \left( \inf_{h \in H} h \right) \geqslant \mu^\bullet \left( \inf_{h \in H} h \varphi_K \right) = \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h \varphi_K) \geqslant \inf_{h \in H, h \leqslant h_0} \mu^\bullet(h) - \varepsilon.
$$

因而(6)的左边是右边$\geqslant$；反之不等式显而易见，命题成立。

#### 推论{#int-ix-s1-n6-cor-1 .statement tag=09NC}

— a) 令$(U_\alpha)_{\alpha \in I}$为递增有向$T$的开子集族，其中并$U$。然后$\mu^\bullet(U) = \sup_{\alpha \in I} \mu^\bullet(U_\alpha)$。

b) 令 $(F_\alpha)_{\alpha \in I}$ 为递减 $T$ 的封闭子集有向族，其中交 $F$。如果存在 $\alpha \in I$ 使得 $\mu^\bullet(F_\alpha)$ 是有限的，则$\mu^\bullet(F) = \inf_{\alpha \in I} \mu^\bullet(F_\alpha)$。

由前面的推论，存在最大的局部可忽略的开集合；这证明了以下定义的合理性：

#### 定义 8 {#int-ix-s1-def-8 .statement tag=09ND}

— *对$T$的措施$\mu$的支持被定义为本地最大的的补充$\mu$-可忽略$T$中的开放集合*。

$\mu$的支持度表示为$\operatorname{Supp}(\mu)$。

#### 注 1 {#int-ix-s1-n6-rem-1 .statement tag=09NE}

如果$\mu$是一个复杂测度，$\mu$的支持度定义为正测度$|\mu|$的支持度；它又是本地$\mu$的最大的的补充-可以忽略不计的开放集合。

#### 注 2 {#int-ix-s1-n6-rem-2 .statement tag=09NF}

让我们证明No. 3的*例2*中引入的措施是$T$中具有紧凑支持的措施。令$\mu$为$T$的正测度，其支持度为紧集$K$，并令$\nu$为$\mu_K$定义的测度（在No. 3的意义上）。让$f \in \mathscr{F}_+(T)$；那么

$$
\nu^\bullet(f) = \mu_K^\bullet(f_K) \quad \text{(No. 3, formula (3))}.
$$

负担$\mu^\bullet$集中在$K$，我们也有

$$
\mu^\bullet(f) = \mu^\bullet(f \varphi_K) = \mu^\bullet((f_K)^0) = \mu_K^\bullet(f_K),
$$

从而$\mu^\bullet = \nu^\bullet$，最后$\mu = \nu$。相反，如果$K$是$T$中的紧集，并且$\lambda$是$K$上的测度，并且如果$\mu$是由$\lambda$定义的$T$上的测度，则$\mu^\bullet(\mathbf{C}K) = 0$ (No. 3， 公式 (3));因而，$\mu$的支撑包含在$K$中，因此是紧的。

### 7. 上部信封和和措施

#### 命题 6 {#int-ix-s1-prop-6 .statement tag=09NG}

— *令 $(\lambda_\alpha)_{\alpha \in A}$ 为递增 $T$ 上的有向测度系列，并令 $p = \sup_\alpha \lambda_\alpha^\bullet$。对于家庭$(\lambda_\alpha)$在$\mathscr{M}(T)$中的上述界限，产权负担$p$在当地有界限是必要且充分的。然后，族$(\lambda_\alpha)$在$\mathscr{M}(T)$和$\lambda^\bullet = p$中承认至高$\lambda$。对于每个紧集 $K$，测度 $\lambda_K$ 是 $\mathscr{M}(K)$* 中测度 $(\lambda_\alpha)_K$ 的上乘。

如果族 $(\lambda_\alpha)$ 在 $\mathscr{M}(T)$ 中有界，那么 $p$ 显然是局部有界的。相反，让我们假设 $p$ 是局部有界的，并证明它满足 No. 2 的命题 2 b) 的条件 1) 和 2)。对于 2)，这是由以下等式得出的：

$$
p(f) = \sup_\alpha \lambda_\alpha^\bullet(f) = \sup_\alpha \sup_K \lambda_\alpha^\bullet(f \varphi_K) = \sup_K \sup_\alpha \lambda_\alpha^\bullet(f \varphi_K) = \sup_K p(f \varphi_K).
$$

另一方面，令K为紧集；负担$p_K$等于负担$(\lambda_\alpha^\bullet)_K$的上包络线，并且它是有界的，因为$p$是局部有界的。因此，措施$(\lambda_\alpha)_K$在$\mathscr{M}(K)$和$\lambda_K^\bullet = p_K$中承认最高值$\lambda_K$（第V, §1, No. 4章，第11条命题）。从而满足No. 2的命题2 b)的条件1)，因此在T上存在测度$\lambda$使得$\lambda^\bullet = p$；显然，$\lambda$是措施$\lambda_\alpha$的至高无上。

#### 定义 9 {#int-ix-s1-def-9 .statement tag=09NH}

*设$(\mu_i)_{i \in I}$为T上的一系列测度。设A为I的有限子集的集合；对于每个$\alpha \in A$让$\lambda_\alpha = \sum_{i \in \alpha} \mu_i$。如果族$(\lambda_\alpha)$在$\mathscr{M}(T)$中承认一个至上$\mu$，则称族$(\mu_i)$是可和的，$\mu$称为族$(\mu_i)$的和，并且写为$\mu = \sum_{i \in I} \mu_i$。*

第 1 章的这个定义扩展定义 V, §2, No. 1。

#### 命题 7 {#int-ix-s1-prop-7 .statement tag=09NI}

*对于家庭 $(\mu_i)_{i \in I}$ 来说，和 $\mu$ 是可求和的，产权负担 $p = \sum_{i \in I} \mu_i^\bullet$ 是局部有界的，在这种情况下是 $p = \mu^\bullet$ 是必要且充分的。对于 T 的每个紧凑子集 K，族 $((\mu_i)_K)_{i \in I}$ 可以在 $\mathscr{M}(K)$ 和 $\mu_K = \sum_{i \in I} (\mu_i)_K$ 中求和。*

与 Def 中的记号相同。 9、I中每有限子集$\alpha$对应$\lambda_\alpha^\bullet = \sum_{i \in \alpha} \mu_i^\bullet$（No. 2，*注* 1）。 叙述则为第 6 条命题的直接的推论。

关系 $\mu_K = \sum_{i \in I} (\mu_i)_K$ 和第 2 章的提案 2。 V, §2, No. 2 产生以下结果：

#### 命题 8 {#int-ix-s1-prop-8 .statement tag=09NJ}

*设 $\mu$ 为 T 上可求和族 $(\mu_i)_{i \in I}$ 的和。在阶中，T 的映射 f 进入拓扑空间 F（无论是否豪斯多夫）为 $\mu$ 可测，f 是可测的$\mu_i$-可测量每个$i \in I$。*

### 8. 压碎物

#### 定义 10 {#int-ix-s1-def-10 .statement tag=09NK}

*我们称T为$\mu$或$\mu$压榨，T的成对不相交的紧凑子集的任何局部可数族$(K_\alpha)_{\alpha \in A}$，使得集合$N = T - \bigcup_{\alpha \in A} K_\alpha$局部$\mu$可忽略不计。*

#### 命题 9 {#int-ix-s1-prop-9 .statement tag=09NL}

*a) 对于 $\mu$，存在 T 的压榨 $(K_\alpha)_{\alpha \in A}$。
b) 令 $(K_\alpha)_{\alpha \in A}$ 为 T 右 $\mu$ 的压榨。如果 $\mu_\alpha$ 是由 $\mu_{K_\alpha}$ (No. 3, 例 2) 定义的 T 测度，则族 $(\mu_\alpha)_{\alpha \in A}$ 是可求和的，*其和等于 $\mu$，并且，对于每个函数 $f \in \mathscr{F}_+(T)$，

$$
\mu^\bullet(f) = \sum_{\alpha \in A} \mu_\alpha^\bullet(f) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_{K_\alpha}) . \tag{1}
$$

为了将 $T$ 的映射 $g$ 转换为拓扑空间 $G$（无论是否为 Hausdorff），并且$\mu$ 可测，$g_{K_\alpha}$ 对于每个$\mu_{K_\alpha}$ 可测是充分必要的$\alpha \in A$。

A) *存在挤压*：

证明是第 14 章命题的重复。 IV, §5, No. 9，略有修改。令$\mathscr{K}$为$T$的紧凑子集$K$的集合，使得$\mathrm{Supp}(\mu_K) = K$，并让$\mathscr{H}$为子集$\mathscr{L}$的集合（按包含排序） $\mathscr{K}$由……组成成对的不相交的集合。让我们首先证明$\mathscr{H}$的每个元素$\mathscr{L}$都是*局部可数的*。令$x$为$T$的点，且$V$为$x$的开邻域，使得$\mu^\bullet(V) < +\infty$；令 $\mathscr{L}_V$ 为与 $V$ 相交的 $K \in \mathscr{L}$ 的集合。如果$(K_i)_{1 \leq i \leq n}$是$\mathscr{L}_V$的不同元素的有限序列，我们有，根据Cor.提案 4，

$$
\sum_{i=1}^n \mu^\bullet(K_i \cap V) = \mu^\bullet\left(V \cap \left( \bigcup_{i=1}^n K_i \right) \right) \leq \mu^\bullet(V),
$$

因为$K_i$是成对的不相交的。因此，

$$
\sum_{K \in \mathscr{L}_V} \mu^\bullet(K \cap V) < +\infty.
$$

现在，对于每个$K \in \mathscr{L}_V$，$\mu^\bullet(K \cap V) = \mu_K^\bullet(K \cap V) > 0$，因为$K \cap V$是非空，在$K$开放，而$\mu_K$的支持度是$K$的全部；因此$\mathscr{L}_V$是可数的，并且$\mathscr{L}$确实是局部可数的。 $\mathscr{H}$ 是归纳性的，直接的，以及非空（有 $\varnothing \in \mathscr{H}$）。因此，令 $\mathfrak{H}$ 为 $\mathscr{H}$ 的极大元素。我们将证明集合 $N = T - \bigcup_{K \in \mathfrak{H}} K$ 局部可以忽略不计。根据命题 2，足以验证对于每个紧集 $L$ 都有 $\mu^\bullet(N \cap L) = 0$，或者再次证明 $\mu_L^\bullet(N \cap L) = 0$。我们将通过矛盾来论证。因此，假设$\mu_L^\bullet(N \cap L) > 0$。由于与$L$相交的$K \in \mathfrak{H}$的集合是可数的，因此$N \cap L$是$\mu_L$可测的；因此存在紧集$J$包含在$N \cap L$中，使得$\mu_L^\bullet(J) > 0$。设$S$为非零的措施$(\mu_L)_J = \mu_J$的支撑；它包含在$N$中，度量$\mu_S$是非零的和$\mathrm{Supp}(\mu_S) = S$（第IV, §5, No. 7，引理2章）。 集合$\mathfrak{H} \cup \{S\}$因此属于到$\mathscr{H}$，与$\mathfrak{H}$的最大特征标矛盾。这就证明了碾压的存在。

(1) 我们稍后会看到 (§2, No. 2) $\mu_\alpha$ 是$\varphi_{K_\alpha} \cdot \mu$。

B) (7) 的证明：
对于每个$\alpha \in A$，$\mu_\alpha^\bullet(f) = \mu_{K_\alpha}^\bullet(f_{K_\alpha}) = \mu^\bullet(f \varphi_{K_\alpha})$乘以No. 3的公式(3)和No. 2的提案2a)；这些公式表明负担$\sum_{\alpha \in A} \mu_\alpha^\bullet$是$\leq \mu^\bullet$，因此家庭$(\mu_\alpha)_{\alpha \in A}$是可求和的（No. 7，命题7）。因此只要证明$\mu = \sum_{\alpha \in A} \mu_\alpha$，即成立公式
$$
\mu_K^\bullet = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet
$$
对于T的每个紧凑子集K。现在，K是固定的，$\alpha \in A$的集合$A'$使得$K_\alpha$与K相交是可数的。让$g \in \mathscr{F}_+(K)$；然后 $g^0 = g^0 \varphi_N + \sum_{\alpha \in A} g^0 \varphi_{K_\alpha}$，然后 $g^0 \varphi_{K_\alpha} = 0$ $\alpha \in A - A'$；根据No. 5的第4条命题，可以得出$\mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha})$、从而
$$
\mu_K^\bullet(g) = \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g^0) = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet(g);
$$
从而式(8)成立。

C) 可测量性：
为了使 T 上定义的函数 $g$ $\mu$ 可测，对于每个 $\alpha \in A$ $\mu_\alpha$ 可测是充分必要的（No. 7，第 8 条）；但这相当于说，$g_{K_\alpha}$对于所有$\alpha \in A$（No. 5，例）来说是$\mu_{K_\alpha}$可测量的。 Q.E.D.

正如第 14 章第 14 章的提案一样。 IV, §5, No. 9，可以要求紧集$K_\alpha$到属于到T的紧凑子集的$\mu$密集集合，提前给出。我们只需要以下结果，我们将直接建立该结果：

#### 命题 10 {#int-ix-s1-prop-10 .statement tag=09NM}

— *如果 g 是拓扑空间 G 中的 $\mu$ 可测映射，其中值（豪斯多夫或非豪斯多夫），则存在 T 的 $\mu$ 压缩 $(L_\beta)_{\beta \in B}$，使得限制 $g_{L_\beta}$ 对于所有情况都是连续的$\beta \in B$.*

考虑将 T 的 $(K_\alpha)_{\alpha \in A}$ 压碎为 $\mu$。由于映射 $g$ 是可测的，因此对于 $K_\alpha$ 的每个 $\alpha \in A$ 划分都存在到紧集的序列 $(K_{\alpha n})$ 以及局部可忽略的集合 $N_\alpha$，使得$g$的限制到集合$K_{\alpha n}$都是连续的。那么，家庭$(K_{\alpha n})_{(\alpha, n) \in A \times \mathbf{N}}$就是人们所寻求的压垮者。因为，它是局部可数的，并且集合$N' = N \cup (\bigcup_\alpha N_\alpha)$局部可忽略不计，因为紧集最多与集合$N_\alpha$的可数无穷大相交。

#### 学院{#int-ix-s1-n8-sch-1 .statement tag=09NN}

— 令 $(K_\alpha)_{\alpha \in A}$ 为 T 的压榨，并令 $N = T - \bigcup_\alpha K_\alpha$。我们用$T'$表示通过将$T'$配备子空间$K_\alpha$拓扑的和拓扑和$N$上的任何局部紧凑拓扑（明确提到的除非）获得的局部紧凑空间。相反，$N$将始终配备离散的拓扑）。对于每个$\alpha \in A$，令$i_\alpha$为$K_\alpha$到$T'$的典范嵌入，并令$\mu'_\alpha$为$T'$上的度量，即$i_\alpha$下$\mu_{K_\alpha}$的像。族 $(\mu'_\alpha)$ 是可求和的：因为，如果 $f$ 是 $T'$ 上的连续函数，且具有紧支撑，则 $\operatorname{Supp}(f)$ 与 $K_\alpha$ 相交，仅获得指标 $\alpha$ 的有限数。我们集合$\mu' = \sum_{\alpha \in A} \mu'_\alpha$。 集合$N$对于$\mu'$来说在局部可以忽略不计，因为对于每个$\mu'_\alpha$都是如此（命题9），$(K_\alpha)_{\alpha \in A}$族是$\mu'$压榨$T'$；现在，$\mu'$对$K_\alpha$引起的测度显然是$\mu_{K_\alpha}$和公式 (7)，应用于$\mu$和$\mu'$，表明$\mu^\bullet = {\mu'}^\bullet$。类似地，第 9 号提案的叙述的最后一个断言，应用于$\mu$ 和$\mu'$，表明*可测量的映射对于两个测量$\mu$ 和$\mu'$* 是相同的。

这两个属性允许将几乎所有关于$\mu$的积分理论简化为针对局部紧致空间阐述的理论。这些考虑因素将在No. 10中展开。

这是另一个破碎概念的应用：

#### 命题 11 {#int-ix-s1-prop-11 .statement tag=09NO}

*令 $X$ 为 $T$ 的 $\mu$ 可测量子集。存在$X$的紧凑子集的局部可数族$(L_\alpha)_{\alpha \in A}$，成对不相交的，使得$X - \bigcup_{\alpha \in A} L_\alpha$在局部$\mu$可以忽略不计。如果，在加法中，$X$是可测量的集合的序列$(X_n)$的并使得$\mu^\bullet(X_n) < +\infty$，那么$\alpha \in A$的集合$B$使得$\mu^\bullet(L_\alpha) \neq 0$是可数，并且$X - \bigcup_{\beta \in B} L_\beta$在本地$\mu$可以忽略不计。*

令$f$为$X$的特征函数，并让$(K_\alpha)_{\alpha \in A}$为$T$的压榨，使得$f$的限制对于每个$K_\alpha$都是连续的（命题10）。然后，集合$L_\alpha = K_\alpha \cap X$对于每个$\alpha \in A$来说都是紧凑的，而$(L_\alpha)_{\alpha \in A}$就是所需的族。让我们进入第二个断言；可测量的集合$X_n$可以清楚地假设为不相交的，并且足以为它们中的每一个建立断言。在其他字中，如果必要的话改变记号，我们可以假设$\mu^\bullet(X) < +\infty$。 $\alpha \in A$的集合$B$使得$\mu^\bullet(L_\alpha) > 0$是可数的，只需要证明集合$N = \bigcup_{\alpha \in A - B} L_\alpha$是局部可忽略的。但$K$是紧集；家庭$(L_\alpha)_{\alpha \in A}$在当地可数，集合$K \cap N$是家庭$(K \cap L_\alpha)_{\alpha \in A - B}$的*可数*亚科的并，因此这个集合在当地可以忽略不计。 $N$也是如此（No. 2，命题2），命题成立。

### 9. 上积分

#### 定义 11 {#int-ix-s1-def-11 .statement tag=09NP}

*对于每个函数$f \in \mathscr{F}_+(T)$，一个定义$f$的上积分（相对于测量$\mu$）是有限或无限正数*

$$
\mu^*(f) = \inf_g \mu^\bullet(g),
$$

*其中$g$超过下半连续函数的集合，即$\geqslant f$。*

还使用记号$\int^* f(t) d\mu(t)$和$\int^* f d\mu$。当$T$局部紧致时，定义重合与通常的定义（第V, §1, No. 1，第4条）。显然$\mu^\bullet(f) \leqslant \mu^*(f)$，当$f$是下半连续时，等式。如果$A$是$T$的子集，则写为$\mu^*(A)$而不是$\mu^*(\varphi_A)$，这个数称为$A$的*外测度*。具有有限外部测量的可测集合称为*可积集合*，就像局部紧致空间的情况一样。

函数 $f$ 与值位于 Banach 空间或$\overline{\mathbf{R}}$ 中，使得$\mu^*(|f|) = 0$ 被称为“可忽略不计”；如果 $\varphi_A$ 可以忽略不计，即 $\mu^*(A) = 0$，则称集合 $A \subset T$ 可以忽略不计。表述“几乎无处不在”是在第 1 章中引入的。 IV, §2, No. 3。

#### 命题 12 {#int-ix-s1-prop-12 .statement tag=09NQ}

*函数$\mu^*$是$T$的负担。*

Def 的属性$a), b), c)$。 No. 1 中的 1 个是明显的。 性质d)的证明与Th相同。第 3 章。 IV, §1, No. 3，考虑到道具。 4 和 5 *a)*。

#### 推论{#int-ix-s1-n9-cor-1 .statement tag=09NR}

*函数$f$，与值在Banach空间或$\overline{\mathbf{R}}$中，当且仅当$f(t) = 0$几乎无处不在时，可以忽略不计。*

如果函数呈阳性，则立即使用 1 个约化。 证明与 Th 相同。第 1 章。 IV, §2, No. 3。

#### 命题 13 {#int-ix-s1-prop-13 .statement tag=09NS}

*对于$T$的每个子集$A$，$\mu^*(A)$是开集合包含$A$的外部度量的下确界。*

证明与第19章的命题相同。 IV, §1, No. 4。

#### 定义 12 {#int-ix-s1-def-12 .statement tag=09NT}

*令 $f$ 为 $T$ 上定义的函数，其中值在 Banach 空间或$\overline{\mathbf{R}}$ 中。有人说，如果$f$是零对可积开集合的可数并的补集，则$f$针对测度$\mu$进行调节，或$\mu$调节。如果函数 $\varphi_A$ 被审核，则 $T$ 的子集 $A$ 被认为被审核。如果函数 $1$ 为 $\mu$ 缓和，则称措施 $\mu$ 已缓和。*

对于例，由于负担$\mu^\bullet$是局部有界的，$T$的每个紧致子集$K$都包含在开集合$V$中，使得$\mu^\bullet(V) < +\infty$；因此，紧集之外的零函数会受到调节。调节了可忽略不计的函数。 注以下 Def。第 2 章。 V, §1, No. 2可以立即扩展到当前上下文。特别是，缓和的正函数的序列中的和被缓和。

#### 注 1 {#int-ix-s1-n9-rem-1 .statement tag=09NU}

在 Lindelöf 空间 T（TG、IX、附录 I，Def. 1）上，尤其是在 Souslin 空间（同上，Cor. of Prop. 1）上，每项措施都经过调节。因为，有限测度形式的开集合是T的覆盖，从中可以提取T的可数覆盖。

#### 注 2 {#int-ix-s1-n9-rem-2 .statement tag=09NV}

但请注意，$\mu$ 的有限测度 Borel 集合的序列的存在，以及并 T，并不一定意味着并 T 的有限测度的开集合的序列的存在（在其他情况下） 字，并不意味着$\mu$已被审核）。参见艾克瑟。 8.

#### 命题 14 {#int-ix-s1-prop-14 .statement tag=09NW}

让$f \in \mathscr{F}_+(T)$。如果$f$是$\mu$-调节的，则$\mu^*(f) = \mu^\bullet(f)$；如果 $f$ 不是 $\mu$ 调节的，则 $\mu^*(f) = +\infty$。

如果$\mu^*(f) < +\infty$，则存在下半连续函数$g \geq f$，使得$\mu^\bullet(g) < +\infty$。对于每个$n \in \mathbf{N}$，令$G_n$为$t \in T$的集合，使得$g(t) > 1/n$； 集合 $G_n$ 是开放的，其中有 $\mu^\bullet(G_n) \leq n \mu^\bullet(g) < +\infty$，$f$ 是零在 $G_n$ 的并之外：函数 $f$ 因此受到调节。

接下来，让我们证明对于调节的函数，$\mu^*$ 和 $\mu^\bullet$ 具有相同的值。由于$\mu^*$和$\mu^\bullet$是负担，当$f$是正函数时，足以建立关系$\mu^*(f) = \mu^\bullet(f)$，上面由常数M限制，并且零在有限测度的开放集合G之外，我们现在应该做。

措施$\mu$是$\mathscr{M}(T)$中递增定向系列$(\mu_i)_{i \in I}$具有紧凑支持的措施的至高无上：这立即来自No. 8的第9号提案。令$g$为T上的下半连续函数，位于$f$和下半连续函数$M \varphi_G$之间。 集合$\nu_i = \mu - \mu_i$；那么 $\mu^\bullet = \mu_i^\bullet + \nu_i^\bullet$ (No. 2, 注 1)，因而
$$
\mu^\bullet(g) - \mu^\bullet(f) = (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + (\nu_i^\bullet(g) - \nu_i^\bullet(f))
$$
$$
\leq (\mu_i^\bullet(g) - \mu_i^\bullet(f)) + \nu_i^\bullet(M \varphi_G).
$$
其中一个有 $\nu_i^\bullet(M \varphi_G) = \mu^\bullet(M \varphi_G) - \mu_i^\bullet(M \varphi_G)$ 和 $\mu^\bullet(M \varphi_G) = \sup \mu_i^\bullet(M \varphi_G)$（No. 7，第 6 条）；因而，数$\nu_i^\bullet(M \varphi_G)$可以通过合适的选择或$i$任意小。因而，一切都归结为表明，对于任何数$c > 0$和任何指标$i \in I$，可以在$f$和$M \varphi_G$之间找到一个下半连续函数$g$，使得$\mu_i^\bullet(g) - \mu_i^\bullet(f) \leq c$。现在，令L为测度$\mu_i$的紧支座，并令$\lambda$为测度$(\mu_i)_L$；由于$\mu_i$集中于L，因此每有函数$h \in \mathscr{F}_+(T)$就有$\mu_i^\bullet(h) = \mu_i^\bullet(h \varphi_L) = \lambda^\bullet(h_L)$（No. 1、引理1和No. 2，命题2）；因而
$$
\mu_i^\bullet(g) - \mu_i^\bullet(f) = \lambda^\bullet(g_L) - \lambda^\bullet(f_L).
$$

1 TG 中引用的附录并未出现在 GT（翻译了早期版本的 Ch. IX）中。 Lindelöf 空间在 GT、I, §9、Exer 中定义。 14； Souslin 空间（GT、IX, §6, No. 2、Def. 2）的习题和定义涵盖了此处所需的材料。

但L是紧的；因而$\lambda^* = \lambda^*$，因此存在定义在L上的下半连续函数$h$，即$\geq f_L$且$\lambda^*(h) \leq \lambda^*(f_L) + c$。由于集合 L 在 T 上闭，函数 k 在 L 上等于 h，并在 $T - L$ 上等于 $+\infty$，因此在 T 上是下半连续，且为 $\geq f$ 和 $\lambda^*(k_L) = \lambda^*(h) \leq \lambda^*(f_L) + c$。它仅保留到集合$g = \inf(k, M \varphi_G)$：$g$是下半连续，$g \geq f$和

$$
\mu_i^*(g) \leq \mu_i^*(k) = \lambda^*(k_L) \leq \lambda^*(f_L) + c = \mu_i^*(f) + c.
$$

#### 推论 1 {#int-ix-s1-prop-14-cor-1 .statement tag=09NX}

*要使函数可以忽略不计，其局部可忽略且可调节是必要且充分的。*

#### 推论 2 {#int-ix-s1-prop-14-cor-2 .statement tag=09NY}

*为了使函数$f$局部可忽略不计，每个$x \in T$拥有一个邻域V使得$f \varphi_V$可以忽略不计是充分必要的。*

因为，如果满足性质，则对于每个紧集 K，$f \varphi_K$可以忽略不计，因而$f$局部可以忽略不计（No. 2，命题2）。相反，假设$f$局部可忽略，令$x$为T的点； $x$ 承认有限测度的开邻域 V。 函数 $f \varphi_V$ 则局部可以忽略不计并且经过调节，因此可以忽略不计。

#### 推论 3 {#int-ix-s1-prop-14-cor-3 .statement tag=09NZ}

*令$f$为T上定义的调节函数。存在成对不相交的紧集的序列$(K_n)$，以及可忽略的集合H，使得$f = f \varphi_H + \sum_n f \varphi_{K_n}$。*

对于，令G为集合，它是可积开集合的可数并，使得$f$是G之外的零；那么 G 是成对不相交的紧集的序列 $(K_n)$ 的并和局部可忽略的集合 H（No. 8，命题 11）；但 H 受到调节，因此可以忽略不计。

#### 推论 4 {#int-ix-s1-prop-14-cor-4 .statement tag=09O0}

*如果$\mu$和$\nu$是T上的两个度量，使得$\mu^* = \nu^*$，则$\mu = \nu$。*

因为，等式$\mu^* = \nu^*$意味着$\mu^*(f) = \nu^*(f)$对于每个正函数$f$，它被调节为$\mu$和$\nu$，因此对于每个具有紧凑支持的正函数；接下来是$\mu^* = \nu^*$（No. 2，第2条命题），然后是$\mu = \nu$（No. 2，第2条命题的Cor.）。

#### 推论 5 {#int-ix-s1-prop-14-cor-5 .statement tag=09O1}

*如果 $\mu$ 是 T 上的调节措施，则存在序列 $(\mu_n)_{n \in \mathbf{N}}$ 具有紧凑支持的措施，使得 $\mu = \sum_{n \in \mathbf{N}} \mu_n$。*

到假设时，常数函数 1 被 $\mu$ 调节。让我们应用 Cor. 3 至案例$f = 1$；因此，存在 T 的成对不相交的紧凑子集的序列 $(K_n)_{n \in \mathbf{N}}$，使得 $1 = \sum_{n \in \mathbf{N}} \varphi_{K_n}$ $\mu$ - 几乎无处不在。令 $\mu_n$ 为 T 上的测度，由 $K_n$ 上的测度 $\mu_{K_n}$ 定义（No. 3，例 2）。人们知道（No. 6，注 2）$\mu_n$具有紧凑的支持，并且$\mu_n^\bullet(f) = \mu^\bullet(f \varphi_{K_n})$对于$f \in \mathscr{F}_+(T)$。现在，$f$等于$\sum_{n \in \mathbf{N}} f \varphi_{K_n}$$\mu$——几乎所有地方，从而

$$
\mu^\bullet(f) = \sum_{n \in \mathbf{N}} \mu^\bullet(f \varphi_{K_n}) = \sum_{n \in \mathbf{N}} \mu_n^\bullet(f).
$$

由此得出 $\mu = \sum_{n \in \mathbf{N}} \mu_n$（No. 7，命题 7）。

### 10. 整合理论

#### 定义 13 {#int-ix-s1-def-13 .statement tag=09O2}

— *让* $p \in [1, +\infty[$； *一个表示由* $\overline{\mathscr{L}}^p(T, \mu)$ *（分别* $\overline{\mathscr{L}}_F^p(T, \mu)$ *如果 F 是 Banach 空间）集合的映射* $\mathbf{f}$ *T 到* $\overline{\mathbf{R}}$ *（分别到 F）进行 $\mu$ 可测量，并且满足*$\mu^\bullet(|\mathbf{f}|^p) < +\infty$。 *一个表示由* $\mathscr{L}^p(T, \mu)$ *(分别* $\mathscr{L}_F^p(T, \mu)$*) $\mu$ 集合-调节* $\overline{\mathscr{L}}^p(T, \mu)$ *(分别* $\overline{\mathscr{L}}_F^p(T, \mu)$*) 的元素。*

我们会写$\overline{N}_p(\mathbf{f}) = \left( \mu^\bullet(|\mathbf{f}|^p) \right)^{1/p}$，$N_p(\mathbf{f}) = \left( \mu^*(|\mathbf{f}|^p) \right)^{1/p}$。我们用$\overline{N}_\infty(\mathbf{f})$表示数$k \geq 0$的下确界，使得$|\mathbf{f}| \leq k$局部$\mu$——几乎无处不在；如果 $\overline{N}_\infty(\mathbf{f}) < +\infty$，则$\mathbf{f}$ 被称为本质上有界。 T 的可测量且基本有界的映射到 $\overline{\mathbf{R}}$（分别到 F）的集合表示为 $\overline{\mathscr{L}}^\infty(T, \mu)$（分别为 $\overline{\mathscr{L}}_F^\infty(T, \mu)$）。 $\overline{\mathscr{L}}_F^1(T, \mu)$（或$\mathscr{L}_F^1(T, \mu)$）中的元素本质上称为可积函数（或可积函数），在F中称为值。

如果 $\mu$ 是一个复杂的度量，则集合

$$
\overline{\mathscr{L}}_F^p(T, \mu) = \overline{\mathscr{L}}_F^p(T, |\mu|) \quad \text{and} \quad \mathscr{L}_F^p(T, \mu) = \mathscr{L}_F^p(T, |\mu|).
$$

在不造成任何混淆的情况下，上述记号通常缩写为$\overline{\mathscr{L}}_F^p(\mu)$、$\overline{\mathscr{L}}_F^p$或$\mathscr{L}^p(\mu)$、$\mathscr{L}^p$。

我们在No. 8（*Scholium*）中看到，我们可以构造一个局部紧凑的空间T'，与T具有相同的底层集合和拓扑更细，并且为T'配备一个测度$\mu'$，使得$\mu$可测量函数和$\mu'$可测函数相同，因此$\mu$和$\mu'$的正函数的本质上积分相等。由此可见，对于 $1 \leq p \leq +\infty$ $^{(1)}$，集合 $\overline{\mathscr{L}}_F^p(\mu)$ 和 $\overline{\mathscr{L}}_F^p(\mu')$ 是相同的。这也意味着在没有新的证明的情况下，$\overline{\mathscr{L}}_F^p$是向量空间，并且函数$\overline{N}_p$是$\overline{\mathscr{L}}_F^p(\mu)$的半范数，对此空间是完整的。

设$\mathbf{f}$为$\overline{\mathscr{L}}_F^p$($1 \leq p < +\infty$)中的元素；因为有 $\mu^\bullet(|\mathbf{f}|^p) = {\mu'}^\bullet(|\mathbf{f}|^p) < +\infty$，第 7 章的命题 7。 V, §1, No. 2 意味着 $\mathbf{f}$ 是零之外

(1) 注空间 $\mathscr{L}_F^p(\mu)$ 包含在 $\mathscr{L}_F^p(\mu')$ 中，但总体上与它不同。

T' 的紧凑子集的序列并和局部 $\mu'$-可忽略的集合；后者集合在局部$\mu$可以忽略不计，并且T'的每个紧凑子集在T中都是紧凑的，因此f在局部$\mu$几乎处处等于$\mu$调节的函数。让我们用局部 $\mu$-可忽略的$\overline{\mathscr{N}}_F$（或$\mathscr{N}_F$）空间（或$\mu$-可忽略）函数来表示；因此我们有$\overline{\mathscr{L}}_F^p = \mathscr{L}_F^p + \overline{\mathscr{N}}_F$和$\mathscr{N}_F = \mathscr{L}_F^p \cap \overline{\mathscr{N}}_F$（No. 9，第14号提案的Cor.1）。因此，空间$\overline{\mathscr{L}}_F^p / \overline{\mathscr{N}}_F$可以被规范地标识为$\mathscr{L}_F^p / \mathscr{N}_F$，并且人们立即验证该标识保留了范数；该商空间表示为$L_F^p(\mu)$。它可以解释为与每个半范数空间$\overline{\mathscr{L}}_F^p(\mu)$和$\mathscr{L}_F^p(\mu)$相关联的范数空间；由于$\overline{\mathscr{L}}_F^p$是完整的，$L_F^p$和$\mathscr{L}_F^p$也是如此。

函数 f 的集合以及 F 中的值，在 T' 上连续且具有紧凑支撑，在 $\overline{\mathscr{L}}_F^p(\mu') = \overline{\mathscr{L}}_F^p(\mu)$ 中密集（第 IV, §3, No. 4，定义 2）。让我们再次讨论No. 8学院的记号。由于 T' 的紧致子集仅与紧集 $K_\alpha$ 的有限数相交，因此具有紧致支持的 T' 上的每个连续函数 f 可写为和
$$
f = \sum_{\alpha \in A} f_\alpha + g,
$$
其中$f_\alpha$是，对于每个$\alpha$，扩张除以$K_\alpha$上的连续函数的0，其中$f_\alpha = 0$除了指标的有限数，并且其中g在局部$\mu$可以忽略不计。因此我们得到以下结果：

#### 命题 15 {#int-ix-s1-prop-15 .statement tag=09O3}

*函数 f 的集合，其中值在 F 中，使得 Supp(f) 是紧致的，并且 f 到 Supp(f) 的限制是连续的，对于 $1 \leq p < +\infty$，在 $\overline{\mathscr{L}}_F^p(\mu)$ 和 $\mathscr{L}_F^p(\mu)$ 中是稠密的。*

注这些函数 *不是*连续的函数 *在* T 上具有紧凑的支撑。

让我们转到积分的定义。

#### 命题 16 {#int-ix-s1-prop-16 .statement tag=09O4}

*F 中存在且仅有一个连续的线性映射 $f \mapsto \int f d\mu$，空间 $\overline{\mathscr{L}}_F^1(\mu)$，具有以下性质：
如果 f 为形式 $t \mapsto g(t)a$，其中 $a \in F$，且 g 为正函数、有限、$\mu$ 可测且$\mu^*(g) < +\infty$，则$\int f d\mu = \mu^*(g) \cdot a$。*

因为，半范数空间 $\overline{\mathscr{L}}_F^1(\mu)$ 和 $\overline{\mathscr{L}}_F^1(\mu')$ 是相同的。由于$\mu^* = {\mu'}^*$，映射$f \mapsto \int f d\mu'$满足条件或叙述。另一方面，叙述中考虑的形式$f = g \cdot a$的函数中的集合在$\overline{\mathscr{L}}_F^1(\mu')$（第IV, §3, No. 5，第10条）、从而唯一性中*总计*。

有人说，$\int f\, d\mu$是$f$对$\mu$的积分，而这个向量也表示为$\mu(f)$或$\int f(t)\, d\mu(t)$。

由于$\int f\, d\mu = \int f\, d\mu'$对于$F$中的每个本质可积函数$f$和值，所有本质积分扩展的理论到Hausdorff空间的测度，没有新的证明；由此，通过将自己限制在调节的函数，可以推导出相对于普通积分的结果。我们特别引用以下结果：

— Th。第 3 章。 IV, §3, No. 4，它的扩张到$\overline{\mathscr{L}}_F^p$，以及它的两个推论。
— Th。第 4 章。 IV, §3, No. 5（合成，带有连续的线性映射）及其推论；道具。 9、11、12为同一编号。
— Ch. 的所有结果IV, §3, No. 6，相对于$L^p$的有序向量空间结构。
— Ch. 的所有结果IV, §3, No. 7，尤其是勒贝格的定理。
— Ch. 的所有结果IV, §3, No. 8，关系，空间$L_F^p$之间。
— 定理 2 章。 IV, §4, No. 3（勒贝格的定理中的叙述特定于$L_F^1$）。
— Hölder 的不等式（第 IV, §6, No. 4，第 2 章）及其推论。
— 关系之间空间 $L_F^p$ 建立于第 1 章IV, §6, No. 5。
— 第 1 章中建立的空间 $L^p$ 对偶性结果V, §5, No. 8。
— Dunford–Pettis 定理（第 VI, §2, No. 5，第 1 章），其推论 1 和 2，以及第 10 章的命题 10 VI, §2, No. 6（$L_F^1$的双重）。

### 习题 {#int-ix-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
