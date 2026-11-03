---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Representations of real, complex or quaternionic type
appendix: true
lang: zh
source: lie-vii-ix
book_pages: 385-388
pdf_pages: 0392-0395
extraction: native
subsections:
    - "no": 1
      title: REPRESENTATIONS OF REAL ALGEBRAS
      page: 385
      pdf_page: 392
    - "no": 2
      title: REPRESENTATIONS OF COMPACT GROUPS
      page: 387
      pdf_page: 394
statements: 6
exercises: 0
content_sha256: e40896c41aaf533c0934a60db9c421f09e9e0da02ec19115464eb02ead978a96
translated_from: content/en/lie/IX/A2_a2_representations_of_real_complex_or.md
translation_method: google
source_content_sha256: 166c8e4a3ff2601758b90e2cbc28e90c5ad2ac9dc57f18a2eb1d30f70fa6ca87
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 9548fcbf4728d606d98468e12b0652e84d52140156171a6ddae5a6c978ec4c7d
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 附录 II

# 表示实数、复数或四元数型

### 1. 表示 / 实代数

用$\mathbf{C}$的$\sigma$自同构$\alpha  \rightarrow \overline{\alpha}$表示；如果 W 是复数向量空间，则用 W 表示 $\mathbf{C}$ 向量空间 $\sigma_*(W)$（即群 W，其中律为运算 $(\alpha , w) \rightarrow \overline{\alpha w}$，对于 $\alpha \in \mathbf{C}, w\in W$）。

#### 命题 1 {#lie-ix-a2-prop-1 .statement tag=01IS}

设 A 是一个 $\mathbf{R}$ 代数（结合和单位）和 V $\mathbf{R}$ 上的有限维单A-模。那么，我们一定处于以下三种情况之一：

V（代数，第VIII, § 5, no. 1章）的$\alpha )$交换子与$\mathbf{R}$同构的，并且$A_{(\mathbf{C})}$-模$V_{(\mathbf{C})}$很简单；

V的$\beta )$交换子与$\mathbf{C}$同构的； $A_{(\mathbf{C})}$-模块$V_{(\mathbf{C})}$是由$\sigma \otimes 1_V$互换的两个非同构简单$A_{(\mathbf{C})}$-子模块的直和；

V的$\gamma )$交换子与$\mathbf{H}$同构的； $A_{(\mathbf{C})}$-模块$V_{(\mathbf{C})}$是由$\sigma \otimes 1_V$互换的两个同构简单$A_{(\mathbf{C})}$-子模块的直和。

V的交换子E是域，$\mathbf{R}($代数的有限扩张，第1章。 VIII, §3, no. 2，命题 2)，因此同构于 $\mathbf{R},\mathbf{C}$ 或 $\mathbf{H}($代数，第 1 章。 VIII, §15）。 $A_{(\mathbf{C})}$-模块$V_{(\mathbf{C})}$是半单（代数，第VIII, §11, no. 4章），其交换子可以用$\mathbf{C}\otimes_{\mathbf{R}}E ($代数来识别，第7章。 VIII, §11, no. 2、引理 1)。

如果E同构于$\mathbf{R}$，$V_{(\mathbf{C})}$的交换子同构于$\mathbf{C}$，并且$V_{(\mathbf{C})}$是一个简单的$A_{(\mathbf{C})}$模（代数，第VIII, §11, no. 4章）。

若E不与$\mathbf{R}$同构的，则包含域同构于$\mathbf{C}$；由此可见，V有一个$A_{(\mathbf{C})}$模块结构，用$V^c$表示。那么$V^c$是一个简单的$A_{(\mathbf{C})}$模块，而$\mathbf{C}$线性映射$\psi : V_{(\mathbf{C})}\rightarrow V^c\oplus \overline{V}^c$使得$\psi (\alpha \otimes v) =$$(\alpha v,\overline{\alpha v})$对于$\alpha \in \mathbf{C},v\in V$来说是同构（代数，第1章）。 V, §10, no. 4，提案 8）。此外，在这个同构下的$\sigma \otimes 1_V$对应到$V^c\oplus \overline{V}^c$的$\mathbf{R}$自同构$(v, v') \rightarrow (v', v)$，因此互换了两个$A_{(\mathbf{C})}$子模块$\psi^{-1}(V^c)$和$\psi^{-1}(V^c)$。

$V_{(\mathbf{C})}$的交换子$E_{(\mathbf{C})}$因此包含$\mathbf{C}\times \mathbf{C}$，通过$V^c\oplus \overline{V}^c$上的同位运算。当且仅当 $E_{(\mathbf{C})}$ 约化到 $\mathbf{C}\times \mathbf{C}$ 时，不存在从 $V^c$ 到 $\overline{V}^c$ 的 $A_{(\mathbf{C})}$ 模块中的同构，即，如果 E 与 $\mathbf{C}$ 同构。这样就完成了证明。

#### 命题 2 {#lie-ix-a2-prop-2 .statement tag=01IT}

设 A 为 $\mathbf{R}$ 代数（结合和单位），W 为 $\mathbf{C}$ 上的有限维简单 $A_{(\mathbf{C})}$ 模。那么，我们一定处于以下三种情况之一：

a) 存在从W到$\overline{W}$与$\theta \circ \theta = 1_W$的$A_{(\mathbf{C})}$同构$\theta$。那么$\theta$的固定点的集合V是W上的$\mathbf{R}$结构，单A-模与交换子$\mathbf{R}.1_V$。而且，$W_{[\mathbf{R}]}$是两个同构单A-模的直和。

b) $A_{(\mathbf{C})}$模W和$\overline{W}$不是同构的；那么 $W_{[\mathbf{R}]}$ 是单A-模和交换子 $\mathbf{C}.1_W$。

c) 存在从W到$\overline{W}$与$\theta \circ \theta =-1_W$的$A_{(\mathbf{C})}$同构$\theta$。那么A-模$W_{[\mathbf{R}]}$就简单了，它的交换子就是域$\mathbf{C}.1_W\oplus \mathbf{C}.\theta$，与$\mathbf{H}$同构。

复杂的向量空间Hom$_{A_{(\mathbf{C})}}(W,W)$是维数$\leq 1 ($代数，第1章。 VIII, §3, no. 2);如果$\theta \in$Hom$_{A_{(\mathbf{C})}}(W,W)$，则W的自同态$\theta \circ \theta$为位似，比率为$\alpha \in \mathbf{C}$。对于所有$w\in W$，我们有$\alpha \theta (w) =\theta \circ \theta \circ \theta (w) =$$\theta (\alpha w) = \overline{\alpha \theta}(w)$，所以$\alpha$是真实的。如果$\theta '=\lambda \theta$，与$\lambda \in \mathbf{C}$，则$\theta '\circ \theta '=|\lambda |^2\theta \circ \theta$；因此，恰好实现了以下三种可能性之一：

a) 存在$\theta \in$Hom$_{A_{(\mathbf{C})}}(W,W)$和$\theta \circ \theta = 1_W$；

b) 坎$_{A_{(\mathbf{C})}}(W,W) =\{0\}$；

c) 存在$\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ 和$\theta \circ \theta =-1_W$。

在情况a)中，$\theta$的固定点的集合V是W上的$\mathbf{R}$结构（代数，第V，p. 61，第7条）；由于 $V_{(\mathbf{C})}$ 与 W 同构，A-模 V 与交换子 $\mathbf{R}.1_V$ 是简单的（命题 1），而 $W_{[\mathbf{R}]}$ 则不简单。

反之，如果$W_{[\mathbf{R}]}$不简单，则令V为$W_{[\mathbf{R}]}$的简单A-子模；因为$A_{(\mathbf{C})}$-模W很简单，$V +iV = W$和$V\cap iV =\{0\}$，即$W = V\oplus iV$。因而，V是W上的$\mathbf{R}$结构，并且同构$\theta$从W到$\overline{W}$，使得$v$的$\theta (v+iv') =v-iv'$和V中的$v'$满足$\theta \circ \theta = 1_W$。

因而，在情况 b) 和 c) 中，A-模 $W_{[\mathbf{R}]}$ 很简单；根据命题 1，其交换子 E 同构于情况 b) 中的 $\mathbf{C}$，以及情况 c) 中的$\mathbf{H}$。此外，很明显，在情况 c) 中，E 包含 $\mathbf{C}.1_W$ 和$\mathbf{C}.\theta$，因此命题。

对于命题中的假设，在$a),b)$或c）情况下，$A_{(\mathbf{C})}$模W分别被称为实模、复模或四元数型（相对于A）。

对于$K =\mathbf{R}$或$\mathbf{C}$，用K上的有限维简单$A_{(K)}$模的类的$\mathfrak{S}_K(A)$集合表示。群$\Gamma =$Gal($\mathbf{C}/\mathbf{R}$)在$\mathfrak{S}_{\mathbf{C}}(A)$上运算；前两个命题在$\mathfrak{S}_{\mathbf{R}}(A)$和商集$\mathfrak{S}_{\mathbf{C}}(A)/\Gamma$之间建立双射对应。

### 2. 紧凑型表示群

令 G 为紧拓扑群，并令 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(W)$ 为 G 在有限维复数向量空间上的连续表示。如果$\mathbf{C}^{(G)}$-模W（相对于代数$A =\mathbf{R}^{(G)}$）就是这种情况，我们可以说$\rho$是实数、复数或四元数型的不可约。令 H 为 W 上的分离正数厄米特形式，在 G 下不变。

#### 命题 3 {#lie-ix-a2-prop-3 .statement tag=01IU}

假设 $\rho$ 是不可约的。

a) 表示 $\rho$ 是实型当且仅当 W 上存在非零对称双线性形式 B，且在 G 下不变。在这种情况下形式 B 是分离的； $w\in W$的集合V使得$H(w, x) = B(w, x)$对于所有$x\in W$来说是G下W不变量上的$\mathbf{R}$结构。

b) 表示 $\rho$ 是复数型当且仅当在 G 下的 W 不变量上不存在非零双线性形式。

c) 表示 $\rho$ 为四元数型当且仅当 W 上存在非零交错的双线性形式，在 G 下不变；这样形式必然是分离的。

对于 $\theta \in$ Hom$_{\mathbf{C}^{(G)}}(W,W)$ 和 $x, y\in W$，输入 $B_{\theta}(x, y) = H(\theta x, y)$。那么$B_{\theta}$在W上是双线性形式，在G下不变，并且如果$\theta$非零则分离。用G下W不变量上的双线性形式的$\mathscr{B}(W)^G$空间表示；从Hom$_{\mathbf{C}^{(G)}}(W,W)$到$\mathscr{B}(W)^G$的映射$\theta  \rightarrow B_{\theta}$是$\mathbf{C}$向量空间的同构。这尤其意味着断言 b)。

令$\theta$是从W到$\overline{W}$的$\mathbf{C}^{(G)}$同构的，使得$\theta \circ \theta =\alpha_W$，与$\alpha \in  \{-1,+1\}$（命题2）；由于 $\mathscr{B}(W)^G$ 的值为维数 1，因此存在 $\varepsilon \in \mathbf{C}$ 使得

$B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y)$ 对于 $W$ 中的所有 $x, y$。

迭代，我们得到$B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y) =\varepsilon^2B_{\theta}(y, x)$，因此$\varepsilon^2$ = 1 和$\varepsilon \in  \{-1,+1\}$。此外，对于 W 中的 $x$，

$$
H(\theta x, \theta x) = B_{\theta}(x, \theta x) =\varepsilon B_{\theta}(\theta x, x) =\varepsilon H(\theta \circ \theta (x), x) =\varepsilon \alpha H(x, x)
$$

所以$\varepsilon \alpha  >0$，因为H是正数，即$\varepsilon =\alpha$。 断言 a) 和 c) 现在遵循命题 2。

用 $dg$ 表示 G 上总质量 1 的哈尔测度。

#### 引理 1 {#lie-ix-a2-lem-1 .statement tag=01IV}

设$W^G$为W的子空间，元素的由……组成在G下不变。W的自同态$\int_G\rho (g)dg$为投影和像$W^G$，与G的运算兼容。特别是，dim$W^G=\int_G$Tr $\rho (g)dg$。

把$p=\int_G\rho (g)dg$；对于$h\in G$，

$$
\rho (h)\circ p=\int_G\rho (hg)dg=\int_G\rho (g)dg=p
$$

类似地$p\circ \rho (h) =p$。因此，$p$与G的运算兼容，其像包含在$W^G$中。如果$w\in W^G$，我们就有$p(w) =\int_G\rho (g)w dg=w$，因此有引理。

#### 引理 2 {#lie-ix-a2-lem-2 .statement tag=01IW}

令 $u$ 为域 K 上有限维向量空间 E 的自同态。则

Tr $u^2=$ Tr $\mathbf{S}^2(u)-$ Tr $\wedge \wedge^2(u)$。

设$\chi_u(X) =\prod_{i=1}^n(X-\alpha_i)$为$u$的特征多项式的分解，在合适的K扩张中将因子转化为线性因子。我们有Tr$u^2=\sum_i\alpha^2_i$，Tr$\wedge \wedge^2(u) =\sum_{i<j}\alpha_i\alpha_j$，Tr$\mathbf{S}^2(u) =\sum_{i\leq j}\alpha_i\alpha_j$（cf.代数，第1章） VII, §5, no. 5，Cor.3)，因此是结果。

#### 命题 4 {#lie-ix-a2-prop-4 .statement tag=01IX}

假设 $\rho$ 是不可约的。那么，$\rho$ 是实数（复数，四元数）型当且仅当积分 $\int_G$ Tr$\rho (g^2)dg$ 等于 1（分别为 0，分别为 $-1$）。

用$\check{\rho}$表示$\rho$在$W^*$上的同余表示（由$\check{\rho}(g) =^t\rho (g^{-1})$定义）。 应用引理 2 到 $\check{\rho}(g)$ 并在 G 上积分得到

$\int_G$ Tr$\rho (g^2)dg=\int_G$ Tr $^t\rho (g^{-2})dg=\int_G$ Tr $\mathbf{S}^2( \check{\rho}(g))dg-\int_G$ Tr $\wedge \wedge^2( \check{\rho}(g))dg$

因此，通过引理 1，

$\int_G$Tr$\rho (g^2)dg=$暗淡($\mathbf{S}^2W^*$)$^G-$暗淡($\wedge \wedge^2W^*$)$^G$。

但$\mathbf{S}^2W^*$（或$\wedge \wedge^2W^*$）可以与W 上对称（或交错的）双线性形式的空间等同。因此，命题立即由命题3 得出。
