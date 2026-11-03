---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 3
section_title: Subalgebras of split semi-simple Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 86-95, 229-231
pdf_pages: 0094-0103, 0237-0239
extraction: native
subsections:
    - "no": 1
      title: SUBALGEBRAS STABLE UNDER ad $\mathfrak{h}$
      page: 86
      pdf_page: 94
    - "no": 2
      title: IDEALS
      page: 89
      pdf_page: 97
    - "no": 3
      title: BOREL SUBALGEBRAS
      page: 90
      pdf_page: 98
    - "no": 4
      title: PARABOLIC SUBALGEBRAS
      page: 92
      pdf_page: 100
    - "no": 5
      title: NON-SPLIT CASE
      page: 94
      pdf_page: 102
statements: 28
exercises: 14
content_sha256: b4460313acd45fb1f2aef4857f7a0a2b3a05eb3696c8033241d9af21ad200b5f
translated_from: content/en/lie/VIII/03_s3_subalgebras_of_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 043e172960e451fa011db5fc5b2cdd69d22334e7720054bdacde767c930f9a50
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 90b06bfe7db1c3607794304649ca02c1bafd592a892a7b8e1be547fb1f9f4755
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。 子代数共分裂的半单李代数

在本段中，我们用 $(\mathfrak{g},\mathfrak{h})$ 分裂的半单李代数表示，用 R 表示根系。

### 1. 子代数广告下稳定$\mathfrak{h}$

#### 引理 1 {#lie-viii-s3-lem-1 .statement tag=00ZO}

令V为$\mathfrak{g}$的向量子空间且R(V)集合为$\alpha \in R$，使得$\mathfrak{g}^{\alpha}\subset V$。那么，$(V\cap \mathfrak{h}) +\sum_{\alpha\in R(V)}\mathfrak{g}^{\alpha}$在广告$\mathfrak{h}$下是稳定的V的最大的向量子空间。

向量子空间 V 的 W 在 ad $\mathfrak{h}$ 下稳定当且仅当

$$
W = (W\cap \mathfrak{h}) +\sum_{\alpha\in R}(W\cap \mathfrak{g}^{\alpha})
$$

（代数，第 VII, §2, no. 2 章，第 1 章第 1 章）。因此，在广告 $\mathfrak{h}$ 下，V 的最大的向量子空间稳定，因此为 $(V\cap \mathfrak{h}) +\sum_{\alpha\in R}(V\cap \mathfrak{g}^{\alpha})$。但是$V\cap \mathfrak{g}^{\alpha}=\mathfrak{g}^{\alpha}$对应$\alpha \in R(V)$，$V\cap \mathfrak{g}^{\alpha}= 0$对应$\alpha  \notin R(V)$，因为暗淡$\mathfrak{g}^{\alpha}= 1$。 Q.E.D.

对于 R 的任意子集 P，将

$$
\mathfrak{g}^P=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}\mathfrak{h}_P=\sum_{\alpha\in P}\mathfrak{h}_{\alpha}
$$

如果$P\subset R$和$Q\subset R$，我们显然有

$$
[\mathfrak{h},\mathfrak{g}^P]\subset \mathfrak{g}^P \tag{1}
$$

$$
[\mathfrak{g}^P,\mathfrak{g}^Q] =\mathfrak{g}^{(P+Q)\cap R}+\mathfrak{h}_{P\cap(-Q)} \tag{2}
$$

回想一下（第VI, §1, no. 7，定义4），如果条件$\alpha \in P, \beta \in P, \alpha +\beta \in R$暗示$\alpha +\beta \in P$，则R的子集P被认为是封闭的，在其他字，如果$(P + P)\cap R\subset P$。

#### 引理 2 {#lie-viii-s3-lem-2 .statement tag=00ZP}

令$\mathfrak{h}'$为$\mathfrak{h}$的向量子空间，P为R的子集。则$\mathfrak{h}'+\mathfrak{g}^P$为$\mathfrak{g}$的子代数当且仅当P为R的闭子集且

$$
\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)}
$$

确实，

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}'+\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] =\mathfrak{h}_{P\cap(-P)}+ [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}
$$

因此 $\mathfrak{h}'+\mathfrak{g}^P$ 是 $\mathfrak{g}$ 的子代数当且仅当

$\mathfrak{h}_{P\cap(-P)}\subset \mathfrak{h}'$ 和 $\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P$

这就证明了引理。

#### 命题 1 {#lie-viii-s3-prop-1 .statement tag=00ZQ}

(i) 在ad$\mathfrak{h}$下稳定的$\mathfrak{g}$子代数是形式$\mathfrak{h}'+\mathfrak{g}^P$的向量子空间，其中P是R的闭子集，$\mathfrak{h}'$是向量子空间 $\mathfrak{h}$ 包含 $\mathfrak{h}_{P\cap(-P)}$。

(ii) 设$\mathfrak{h}',\mathfrak{h}''$为$\mathfrak{h}$和$P,Q$的向量子空间，并且用$\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)},\mathfrak{h}''\subset \mathfrak{h}'$和$Q\subset P$封闭R的子集。那么$\mathfrak{h}''+\mathfrak{g}^Q$是$\mathfrak{h}'+\mathfrak{g}^P$的理想当且仅当

$(P + Q)\cap R\subset Q$ 和$\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}''\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$ 克尔$\alpha$。

断言 (i) 紧随引理 1 和 2。令 $\mathfrak{h}',\mathfrak{h}'',P,Q$ 如 (ii) 中所示。然后

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}''+\mathfrak{g}^Q] =\mathfrak{h}_{P\cap(-Q)}+ [\mathfrak{h}',\mathfrak{g}^Q] + [\mathfrak{h}'',\mathfrak{g}^P] +\mathfrak{g}^{(P+Q)\cap R}
$$

因此，$\mathfrak{h}''+\mathfrak{g}^Q$是$\mathfrak{h}'+\mathfrak{g}^P$的理想当且仅当

$$
\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}'',[\mathfrak{h}'',\mathfrak{g}^P]\subset \mathfrak{g}^Q,\mathfrak{g}^{(P+Q)\cap R}\subset \mathfrak{g}^Q
$$

这意味着(ii)。

#### 命题 2 {#lie-viii-s3-prop-2 .statement tag=00ZR}

令$\mathfrak{a}$为在ad$\mathfrak{h}$下稳定的$\mathfrak{g}$的子代数，并令$\mathfrak{h}'\subset \mathfrak{h}$、$P\subset R$为$\mathfrak{a}=\mathfrak{h}'+\mathfrak{g}^P$。

(i) 设$\mathfrak{k}$为$x\in \mathfrak{h}'$的集合，使得$\alpha (x) = 0$对于所有$\alpha \in P\cap (-P)$。 $\mathfrak{a}$的根基是$\mathfrak{k}+\mathfrak{g}^Q$，其中Q是$\alpha \in P$的集合，使得$-\alpha  \notin P$。此外，$\mathfrak{g}^Q$是$\mathfrak{a}$的幂零理想。

(ii) $\mathfrak{a}$ 是半单当且仅当 $P =-P$ 和 $\mathfrak{h}'=\mathfrak{h}_P$。

(iii) $\mathfrak{a}$ 可解当且仅当$P\cap (-P) =\emptyset$。在这种情况下$[\mathfrak{a},\mathfrak{a}] =\mathfrak{g}^S$，其中

$$
S = ((P + P)\cap R)\cup  \{\alpha \in P|\alpha (\mathfrak{h}')\not= 0\}
$$

(iv) 当且仅当$P =-P$时，$\mathfrak{a}$在$\mathfrak{g}$中可还原。

(v) $\mathfrak{a}$ 包含幂零元当且仅当 $\mathfrak{h}'= 0$。那么$P\cap (-P) =$$\emptyset$，$\mathfrak{a}$是幂零的。

我们证明(v)。如果$\mathfrak{a}$由幂零元组成，$\mathfrak{a}$显然是幂零的，并且$\mathfrak{h}'= 0$自$\mathfrak{h}$的元素是半单。假设$\mathfrak{h}'= 0$。根据提案 1 (i)，$P\cap (-P) =\emptyset$。由章。 VI, §1, no. 7，命题22，存在R的室C使得$P\subset R_+(C)$。因此，存在整数 $n >0$，具有以下性质：如果 $\alpha_1, . . . , \alpha_n\in P$ 和 $\beta \in R\cup  \{0\}$，则

$$
\alpha_1+\cdots +\alpha_n+\beta  \notin R\cup  \{0\}
$$

这意味着 $\mathfrak{g}^P$ 的每个元素都是幂零的，因此 (v)。

我们证明(iii)。如果 $P\cap (-P) =\emptyset ,\mathfrak{g}^P$ 是 $\mathfrak{g}$ 的子代数（命题 1 (i)），并且由 (v) 幂零。现在

$$
[\mathfrak{a},\mathfrak{a}] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P
$$

所以$\mathfrak{a}$是可解的，$[\mathfrak{a},\mathfrak{a}]$由公式在命题中给出。如果$P\cap (-P)\not=\emptyset$，则令$\alpha \in P$使得$-\alpha \in P$。那么$\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$是$\mathfrak{a}$的单子代数，所以$\mathfrak{a}$是不可解的。

我们证明（i）。由于 P 是闭集，$(P + Q)\cap R\subset P$。如果$\alpha \in P, \beta \in Q$和$\alpha +\beta \in R$，我们不能有$\alpha +\beta \in  -P$，因为P是封闭的，这意味着$-\beta =-(\alpha +\beta ) +\alpha \in P$而$\beta \in Q$；因而，$(P + Q)\cap R\subset Q$。这证明了 $\mathfrak{g}^Q$ 是 $\mathfrak{a}$ 的理想，由 (v) 幂零的。我们有$P\cap (-Q) =\emptyset$和$P\cap (-P) = P\cap \complement Q$，所以$\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{k}\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$Ker$\alpha$。根据提案 1 (ii)，

$\mathfrak{k}+\mathfrak{g}^Q$是$\mathfrak{a}$的理想。从 $Q\cap (-Q) =\emptyset$ 开始，这个理想可以通过 (iii) 求解。因此它包含在$\mathfrak{a}$的根基$\mathfrak{r}$中。因为$\mathfrak{r}$在每个推导下是稳定的，$\mathfrak{a},\mathfrak{r}$在广告$\mathfrak{h}$下是稳定的。因而，存在 P 的子集 S，使得 $\mathfrak{r}= (\mathfrak{r}\cap \mathfrak{h}) +\mathfrak{g}^S$。假设 $\alpha \in S$ 和 $-\alpha \in P$。那么$\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}$，所以$\mathfrak{g}^{-\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}= 0$，所以$-\alpha \in S$；通过 (iii)，与……矛盾 $\mathfrak{r}$ 是可解的。因而，$S\subset Q$。最后，如果$x\in \mathfrak{r}\cap \mathfrak{h}$并且如果$\alpha \in P\cap (-P)$，那么$[x,\mathfrak{g}^{\alpha}]\subset \mathfrak{g}^{\alpha}\cap \mathfrak{r}= 0$，所以$\alpha (x) = 0$；这表明$x\in \mathfrak{k}$。因而(i)的$\mathfrak{r}\subset \mathfrak{k}+\mathfrak{g}^Q$和证明是完整的。

我们证明(iv)。通过(i)，$\mathfrak{g}$上$\mathfrak{a}$的伴随表示是半单当且仅当对于所有$x\in \mathfrak{k}+\mathfrak{g}^Q$而言ad$_{\mathfrak{g}}x$是半单（第I, §6, no. 5，第4章）；由(v)可知，当且仅当$Q =\emptyset$，在其他字$P =-P$。

我们证明(ii)。如果$\mathfrak{a}$是半单，$P =-P$乘以(i)，那么$\mathfrak{h}_P\subset \mathfrak{h}'$；此外，$\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}_P+\mathfrak{g}^P$，因而$\mathfrak{h}'=\mathfrak{h}_P$。如果$P =-P$和$\mathfrak{h}'=\mathfrak{h}_P,\mathfrak{a}$通过(iv)约简，并且$\mathfrak{a}=\sum_{\alpha\in P}\mathfrak{s}_{\alpha}$，那么$\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]$和$\mathfrak{a}$是半单。

#### 命题 3 {#lie-viii-s3-prop-3 .statement tag=00ZS}

令$\mathfrak{a}$为在ad($\mathfrak{h}$)下稳定的$\mathfrak{g}$的半单子代数，并令P为R的子集，使得$\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P$。

(i) $\mathfrak{h}_P$ 是 $\mathfrak{a}$ 中的分裂嘉当子代数。

(ii) $(\mathfrak{a},\mathfrak{h}_P)$的根系是P的限制的集合到元素的$\mathfrak{h}_P$。

由于$\mathfrak{h}_P$在广告$\mathfrak{h}$下是稳定的，$\mathfrak{a}$中的标准化器在广告$\mathfrak{h}$下是稳定的，因此是形式$\mathfrak{h}_P+\mathfrak{g}^Q$，其中$Q\subset P$（引理1）。如果$\alpha \in Q$，

$$
\mathfrak{g}^{\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{\alpha}]\subset [\mathfrak{h}_P,\mathfrak{g}^{\alpha}]\subset \mathfrak{h}_P
$$

这是荒谬的。因此，$Q =\emptyset$和$\mathfrak{h}_P$是$\mathfrak{a}$中自己的标准化器。这就证明了$\mathfrak{h}_P$是$\mathfrak{a}$的嘉当子代数。如果 $x\in \mathfrak{h}_P$、ad$_{\mathfrak{g}}x$ 和更不必说 ad$_{\mathfrak{a}}x$ 可三角化。至此(i)得证，(ii)清楚。

根据命题1(i)，$\mathfrak{g}$包含$\mathfrak{h}$的子代数是集合$\mathfrak{h}+\mathfrak{g}^P$，其中P是R的闭子集。 VII, §3，命题3，$\mathfrak{h}+\mathfrak{g}^P$的每嘉当子代数等于$\mathfrak{g}$的嘉当子代数。

#### 命题 4 {#lie-viii-s3-prop-4 .statement tag=00ZT}

令$\mathfrak{a}$为$\mathfrak{a},s$的$\mathfrak{g}$包含$\mathfrak{h},x$元素的子代数，并且$n$其半单和幂零分量。然后是$s\in \mathfrak{a}$和$n\in \mathfrak{a}$。

我们有（广告$x$）$\mathfrak{a}\subset \mathfrak{a}$，所以（广告$s$）$\mathfrak{a}\subset \mathfrak{a}$和（广告$n$）$\mathfrak{a}\subset \mathfrak{a}$。由于$\mathfrak{a}$在$\mathfrak{g}$中是它自己的标准化器（VII, §2, no. 1章，$4$提案的Cor.4）$,s\in \mathfrak{a}$和$n\in \mathfrak{a}$。

#### 命题 5 {#lie-viii-s3-prop-5 .statement tag=00ZU}

令 P 为 R 的闭子集。

(i) $\mathfrak{h}+\mathfrak{g}^P$ 可解当且仅当$P\cap (-P) =\emptyset$。在这种情况下，$[\mathfrak{h}+\mathfrak{g}^P,\mathfrak{h}+\mathfrak{g}^P] =\mathfrak{g}^P$。

(ii) $\mathfrak{h}+\mathfrak{g}^P$ 是可还原的当且仅当 $P =-P$。

断言 (i) 源自提案 2 (iii)。如果 $P =-P,\mathfrak{h}+\mathfrak{g}^P$ 是还原性的（命题 2 (iv)）。假设 $\mathfrak{a}=\mathfrak{h}+\mathfrak{g}^P$ 是可还原的。然后

$$
\mathfrak{g}^P= [\mathfrak{h},\mathfrak{g}^P]\subset [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}+\mathfrak{g}^P
$$

所以 $[\mathfrak{a},\mathfrak{a}]$ 是形式 $\mathfrak{h}'+\mathfrak{g}^P$ 和 $\mathfrak{h}'\subset \mathfrak{h}$；因为 $[\mathfrak{a},\mathfrak{a}]$ 是半单，$P =-P$（命题 2 (ii)）。

### 2. 理想

#### 命题 6 {#lie-viii-s3-prop-6 .statement tag=00ZV}

令$R_1, . . . ,R_p$为R的不可约分量。对于$i= 1, . . . , p$，输入$\mathfrak{g}_i=\mathfrak{h}_{R_i}+\mathfrak{g}^{R_i}$。那么$\mathfrak{g}_1, . . . ,\mathfrak{g}_p$就是$\mathfrak{g}$的简单分量。

$\mathfrak{g}_i$ 是$\mathfrak{g}$ 的理想（命题 1 (ii)）。很明显，$\mathfrak{g}$是$\mathfrak{g}_i$的直和，因此乘积是$\mathfrak{g}_i$。令$\mathfrak{a}$和$\mathfrak{b}$是$\mathfrak{g}$的互补理想。那么$\mathfrak{a}$和$\mathfrak{b}$是半单并且在ad$\mathfrak{h}$下稳定，所以存在R的子集$P,Q$使得$\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P,\mathfrak{b}=\mathfrak{h}_Q+\mathfrak{g}^Q$。那么对于杀戮形式来说，$\mathfrak{h}_P,\mathfrak{h}_Q$是$\mathfrak{h}$中彼此的正交补，因此P和Q是R的不可约分量的并。这证明了$\mathfrak{g}_i$是$\mathfrak{g}$的最小理想。

#### 推论 1 {#lie-viii-s3-prop-6-cor-1 .statement tag=01IZ}

当且仅当 R 不可约时，$\mathfrak{g}$ 是简单的（在其他字中，其 Dynkin 图是连通的）。

这是根据第 6 条命题得出的。

如果对于 $k$ 的每个扩张 $k'$，$k'$-李代数 $\mathfrak{a}_{(k')}$ 是简单的，则称李代数 $\mathfrak{a}$ 是绝对简单的。

#### 推论 2 {#lie-viii-s3-prop-6-cor-2 .statement tag=00ZW}

可拆分的简单李代数绝对简单。

这是从 Cor 得出的。 1.

如果$\mathfrak{g}$是型$A_l(l\geq 1)$或$B_l(l\geq 1)$或$C_l(l\geq 1)$或$D_l(l\geq 3),\mathfrak{g}$，则称为经典的可分割简单李代数。如果$\mathfrak{g}$是型$E_6, E_7, E_8, F_4$，或者$G_2,\mathfrak{g}$，则据说是一个特殊的可分割简单李代数。

### 3. 博雷尔子代数

#### 命题 7 {#lie-viii-s3-prop-7 .statement tag=00ZX}

设$\mathfrak{b}=\mathfrak{h}+\mathfrak{g}^P$为$\mathfrak{g}$包含$\mathfrak{h}$中的子代数。以下条件是等效的：

(i) $\mathfrak{b}$ 是 $\mathfrak{g}$ 的最大可解子代数；

(ii) 存在 R 的室C，使得 $P = R_+(C)$；

(iii)$P\cap (-P) =\emptyset$和$P\cup (-P) = R$。

(i) $=\Rightarrow$ (ii)：如果 $\mathfrak{b}$ 可解，则$P\cap (-P) =\emptyset$。那么存在 R 的室 C 使得 $P\subset R_+(C)$ （第 VI, §1, no. 7 章，第 22 条命题）。那么$\mathfrak{h}+\mathfrak{g}^{R_+(C)}$是$\mathfrak{g}$包含$\mathfrak{b}$的可解子代数，因此如果$\mathfrak{b}$极大，则等于$\mathfrak{b}$。

(ii) $=\Rightarrow$ (iii)：这很清楚。

(iii) $=\Rightarrow$ (i)：假设 $P\cap (-P) =\emptyset$ 和 $P\cup (-P) = R$。那么$\mathfrak{b}$是可解的。令 $\mathfrak{b}'$ 为 $\mathfrak{g}$ 包含 $\mathfrak{b}$ 的可解子代数。 R 存在子集 Q，使得$\mathfrak{b}'=\mathfrak{h}+\mathfrak{g}^Q$。然后$Q\cap (-Q) =\emptyset$和$Q\supset P$，所以Q = P和$\mathfrak{b}'=\mathfrak{b}$。

#### 定义 1 {#lie-viii-s3-def-1 .statement tag=00ZY}

$\mathfrak{g}$ 包含 $\mathfrak{h}$ 的子代数和满足等价于第 7 条提案中的条件称为 $(\mathfrak{g},\mathfrak{h})$ 的博雷尔子代数。

如果存在 $\mathfrak{g}$ 的分裂嘉当子代数 $\mathfrak{h}'$，使得 $\mathfrak{b}$ 是博雷尔子代数，则可拆分代数 $\mathfrak{g}$ 的子代数 $\mathfrak{b}$ 称为 $\mathfrak{g}$ 的博雷尔子代数 $(\mathfrak{g},\mathfrak{h}')$。

设$(\mathfrak{g},\mathfrak{h})$为分裂约化李代数。令 $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ 与 $\mathfrak{c}$ 可交换且 $\mathfrak{s}$ 半单。 形式$\mathfrak{c}\times \mathfrak{b}$$\mathfrak{g}$子代数，其中$\mathfrak{b}$是$(\mathfrak{s},\mathfrak{h}\cap \mathfrak{s})$的博雷尔子代数，称为$(\mathfrak{g},\mathfrak{h})$博雷尔子代数。

对于第7条命题的记号，我们还说$\mathfrak{b}$是$\mathfrak{g}$的博雷尔子代数，由$\mathfrak{h}$和C定义（或由与C相关的R的$\mathfrak{h}$和基定义）。

#### 注 {#lie-viii-s3-n3-rem-1 .statement tag=00ZZ}

将 $R_+(C)$ 关联到 R 的室 C 的映射是单射的（第 VI, §1, no. 7 章，第 20 条命题第 1 条）。因而，从R室的集合到$(\mathfrak{g},\mathfrak{h})$的博雷尔子代数的集合，$C \rightarrow \mathfrak{h}+\mathfrak{g}^{R_+(C)}$为双射。因而，$(\mathfrak{g},\mathfrak{h})$的博雷尔子代数的数等于R的Weyl 群的阶（第VI, §1, no. 5，第2章）。

#### 命题 8 {#lie-viii-s3-prop-8 .statement tag=0100}

令 $\mathfrak{b}$ 为 $\mathfrak{g},k'$ 扩张 $k$ 中的子代数。那么$\mathfrak{b}\otimes_kk'$是$(\mathfrak{g}\otimes_kk',\mathfrak{h}\otimes_kk')$的博雷尔子代数当且仅当$\mathfrak{b}$是$(\mathfrak{g},\mathfrak{h})$的博雷尔子代数。

这从第 7 条提案条件(iii)中可以清楚地看出。

#### 命题 9 {#lie-viii-s3-prop-9 .statement tag=0101}

设 $\mathfrak{b}$ 为由 R 的室 C 定义的 $(\mathfrak{g},\mathfrak{h})$ 的博雷尔子代数。设 $\mathfrak{n}=\mathfrak{g}^{R_+(C)}=\sum_{\alpha\in R,\alpha >0}\mathfrak{g}^{\alpha}$。让$l=$变暗$\mathfrak{h}$。

(i) 如果$h\in \mathfrak{h}$和$x\in \mathfrak{n}$，则ad$_{\mathfrak{g}}(h+x)$的特征多项式为$T^l\prod_{\alpha\in R}(T-\alpha (h))$。

(ii) $\mathfrak{b}$ 的幂零理想最大的等于$\mathfrak{n}$ 和$[\mathfrak{b},\mathfrak{b}]$。这也是$\mathfrak{g}$中$\mathfrak{b}$元素幂零的集合。

(iii) 令 B 为与 C 相关的 R 的基。对于所有 $\alpha \in B$，令 $X_{\alpha}$ 为 $\mathfrak{g}^{\alpha}$ 的非零元素。然后$(X_{\alpha})_{\alpha\in B}$生成李代数$\mathfrak{n}$。我们有$[\mathfrak{n},\mathfrak{n}] =\sum_{\alpha\in R,\alpha >0,\alpha  \notin B}\mathfrak{g}^{\alpha}$。

$\mathfrak{h}^*_{\mathbf{Q}}$上存在总共阶与其向量空间结构兼容，因此$R_+(C)$的元素是$>0$（第VI, §1, no. 7章）。令$h, x$如(i)和$y\in \mathfrak{g}^{\alpha}$所示。然后$[h+x, y] =\alpha (h)y+z$，其中$z\in \sum_{\beta >\alpha}\mathfrak{g}^{\beta}$。然后，

相对于$\mathfrak{g}$的合适基，ad$_{\mathfrak{g}}(h+x)$的矩阵具有以下属性：

1) 是下三角形；

2）矩阵的对角线条目是数$0 (l$倍），$\alpha (h)$是$\alpha \in R$。

这就证明了(i)。还表明ad$_{\mathfrak{b}}(h+x)$的特征多项式为$T\prod_{\alpha\in R_+(C)}^l(T-\alpha (h))$。由前文可知

$\mathfrak{g}$中$\mathfrak{b}$幂零元素的集合，以及$\mathfrak{b}$的最大幂零理想，等于$\mathfrak{n}$。 根据提案 5 (i)，我们有 $\mathfrak{n}= [\mathfrak{b},\mathfrak{b}]$。 最后，断言 (iii) 源自§2、第 4 (ii) 条命题和第 4 章。 VI, §1, no. 6，提案 19。

#### 推论 {#lie-viii-s3-n3-cor-1 .statement tag=0102}

设$\mathfrak{b}$为$\mathfrak{g}$的博雷尔子代数。

(i) $\mathfrak{b}$ 的每个嘉当子代数都是 $\mathfrak{g}$ 的分裂嘉当子代数。

(ii) 如果$\mathfrak{h}_1,\mathfrak{h}_2$是$\mathfrak{b}$的嘉当子代数，则存在$x\in [\mathfrak{b},\mathfrak{b}]$使得$e^{ad_{\mathfrak{g}}x}\mathfrak{h}_1=\mathfrak{h}_2$。

断言 (i) 源自第 9 (i) 号提案和第 9 章。 VII, §3, no. 3，提案 3。断言 (ii) 源自提案 9 (ii) 和第 1 章。 VII, §3, no. 4，Th。 3.

#### 命题 10 {#lie-viii-s3-prop-10 .statement tag=0103}

设$\mathfrak{b},\mathfrak{b}'$为$\mathfrak{g}$的博雷尔子代数。 $\mathfrak{b}\cap \mathfrak{b}'$中包含$\mathfrak{g}$，存在分裂嘉当子代数。

令$\mathfrak{h}$为$\mathfrak{b},\mathfrak{n}= [\mathfrak{b},\mathfrak{b}],\mathfrak{n}'= [\mathfrak{b}',\mathfrak{b}'],\mathfrak{p}=\mathfrak{b}\cap \mathfrak{b}'$的嘉当子代数，且$\mathfrak{g}$的$\mathfrak{s}$向量子空间与$\mathfrak{b}+\mathfrak{b}'$互补。用$\mathfrak{s}^{\bot},\mathfrak{b}^{\bot},\mathfrak{b}^{'\bot}$表示$\mathfrak{s},\mathfrak{b},\mathfrak{b}'$相对于$\mathfrak{g}$的杀戮形式的正交补集。把$l=$暗淡$\mathfrak{h}, n=$暗淡$\mathfrak{n}, p=$暗淡$\mathfrak{p}$。然后调暗$\mathfrak{b}=$ 调暗$\mathfrak{b}'=l+n$，

昏暗$\mathfrak{s}^{\bot}=$ 昏暗($\mathfrak{b}+\mathfrak{b}'$) $= 2(l+n)-p$,

所以

暗淡($\mathfrak{s}^{\bot}\cap \mathfrak{p}$)$\geq$暗淡$\mathfrak{s}^{\bot}+$暗淡$\mathfrak{p}-$暗淡$\mathfrak{g}$ (3)

$$
= 2(l+n)-p+p-(l+ 2n) =l
$$

根据§2第1号提案，没有。 $2,\mathfrak{n}\subset \mathfrak{b}^{\bot},\mathfrak{n}'\subset \mathfrak{b}^{'\bot}$。 $\mathfrak{p}\cap \mathfrak{n}$的元素在$\mathfrak{g}$（命题9（ii））中是幂零的，并且属于到$\mathfrak{b}'$，因此到$\mathfrak{n}'$（命题9（ii））。因而，$\mathfrak{p}\cap \mathfrak{n}\subset \mathfrak{n}\cap \mathfrak{n}'\subset \mathfrak{b}^{\bot}\cap \mathfrak{b}^{'\bot}$，所以$\mathfrak{s}^{\bot}\cap \mathfrak{p}\cap \mathfrak{n}= 0$。鉴于(3)，我们看到$\mathfrak{s}^{\bot}\cap \mathfrak{p}$是$\mathfrak{b}$中$\mathfrak{n}$的补集。令$z$为$\mathfrak{g}$中$\mathfrak{h}$正则的元素；存在$y\in \mathfrak{n}$使得$y+z\in \mathfrak{s}^{\bot}\cap \mathfrak{p}$；根据命题 9 (i)，ad$_{\mathfrak{g}}(y+z)$ 与 ad$_{\mathfrak{g}}z$ 具有相同的特征多项式，因而 $x=y+z$ 在 $\mathfrak{g}$ 中是正则，在 $\mathfrak{b}$ 和 $\mathfrak{b}'$ 中是更不必说（第 VII, §2, no. 2 章，命题 9）。由于$\mathfrak{g},\mathfrak{b},\mathfrak{b}'$具有相同的秩，$\mathfrak{b}^0(x) =\mathfrak{g}^0(x) ={\mathfrak{b}'}^0(x)$同时是$\mathfrak{b}$、$\mathfrak{g}$和$\mathfrak{b}'$的嘉当子代数（第VII, §3, no. 3第2章）。最后，$\mathfrak{g}$的嘉当子代数是Cor的分裂。提案 9。

#### 推论 {#lie-viii-s3-n3-cor-2 .statement tag=0104}

群 Aut$_e(\mathfrak{g})$ 在对 $(\mathfrak{t},\mathfrak{b})$ 的集合上传递操作，其中 $\mathfrak{t}$ 是 $\mathfrak{g}$ 的分裂嘉当子代数，$\mathfrak{b}$ 是博雷尔子代数 $(\mathfrak{g},\mathfrak{t})$。

令$(\mathfrak{t}_1,\mathfrak{b}_1)$和$(\mathfrak{t}_2,\mathfrak{b}_2)$是两个这样的对。 $\mathfrak{b}_1\cap \mathfrak{b}_2$ 中包含$\mathfrak{g}$，存在分裂嘉当子代数 $\mathfrak{t}$（命题10）。由科。根据第 9 条命题，我们被简化为 $\mathfrak{t}_1=\mathfrak{t}_2=\mathfrak{t}$ 的情况。令 S 为 $(\mathfrak{g},\mathfrak{t})$ 的根系。 S 存在基 $B_1,B_2$，使得$\mathfrak{b}_i$ 与$B_i(i= 1,2)$ 相关联，并且存在$s\in W(S)$，其中变换 $B_1$ 与$B_2$ 相关联。最后，存在$a\in$Aut$_e(\mathfrak{g})$使得$a|\mathfrak{t}=s($§2, no. 2，Cor。的 Th。 2）。然后是$a(\mathfrak{t}) =\mathfrak{t}$和$a(\mathfrak{b}_1) =\mathfrak{b}_2$。

### 4. 抛物线子代数

#### 命题 11 {#lie-viii-s3-prop-11 .statement tag=0105}

设$\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$为$\mathfrak{g}$包含于$\mathfrak{h}$中的子代数。以下条件是等效的：

(i) $\mathfrak{p}$ 包含博雷尔子代数共 $(\mathfrak{g},\mathfrak{h})$；

(ii) 存在 R 的室C，使得 $P\supset R_+(C)$；

(iii) P 是抛物线形，在其他字（第 VI, §1, no. 7 章，定义 4）、$P\cup (-P) =$ R 中。

条件 (i) 和 (ii) 与第 7 条提案等效。 条件 (ii) 和 (iii) 与第 7 章等效。 VI, §1, no. 7，提案 20。

#### 定义 2 {#lie-viii-s3-def-2 .statement tag=0106}

$\mathfrak{g}$ 包含 $\mathfrak{h}$ 的子代数和满足等价于第 11 条的条件称为 $(\mathfrak{g},\mathfrak{h})$ 的抛物线子代数。 $\mathfrak{g}$ 的抛物线子代数是 $(\mathfrak{g},\mathfrak{h}')$ 的抛物线子代数，其中 $\mathfrak{h}'$ 是 $\mathfrak{g}$ 的分裂嘉当子代数。

这个定义扩展立即对应于$(\mathfrak{g},\mathfrak{h})$是分裂约化李代数的情况。

#### 注 {#lie-viii-s3-n4-rem-1 .statement tag=0107}

设B为R的基，且$\mathfrak{b}$相应的博雷尔子代数。若$\Sigma \subset B$，则用根$Q_{\Sigma}$集合表示，即$\Sigma$元素线性组合和系数$\leq 0$；把$\mathfrak{p}(\Sigma ) = R_+(B)\cup Q_{\Sigma}$和$\mathfrak{p}_{\Sigma}=\mathfrak{h}\oplus \mathfrak{g}^{P(\Sigma)}$。由章。 VI, §1, no. 7、引理 3 和命题$20,\mathfrak{p}_{\Sigma}$ 是抛物线子代数包含 $\mathfrak{b}$，$\mathfrak{g}$ 包含 $\mathfrak{b}$ 的每个抛物线子代数都是这样得到的。

#### 引理 3 {#lie-viii-s3-lem-3 .statement tag=0108}

设V为S的抛物线子集的$V^*,\mathscr{P}$集合中的有限维实数向量空间、S根系；令$\mathscr{H}$为$\alpha \in S$的Ker $\alpha$的集合，以及V相对于$\mathscr{H}$的面的$\mathscr{F}$集合（第V, §1, no. 2章，定义1）。

如果 $P\in \mathscr{P}$，则令 F(P) 为 $v\in V$ 的集合，使得对于所有 $\alpha \in P$ 都有 $\alpha (v)\geq 0$。如果$F\in \mathscr{F}$，令P(F)为$\alpha \in R$的集合，使得$\alpha (v)\geq 0$对于所有$v\in F$。

那么从$\mathscr{F}$到$\mathscr{P}$，$F \rightarrow P(F)$就是双射；对于所有 $F\in \mathscr{F}$，F(P(F)) 是 F 的闭包。

a) 设 $P\in \mathscr{P}$。存在 S 的室 C 和基 B(C) 的子集 $\Sigma$，使得$P = S_+(C)\cup Q$，其中 Q 为 $\Sigma$ 的元素线性组合的集合，且非正整数系数 （第 VI, §1, no. 7 章，第 20 条提案）。放

$$
B(C) =\{\alpha_1, . . . , \alpha_l\}, \Sigma =\{\alpha_1, . . . , \alpha_m\}
$$

如果$v\in V$，我们有以下等价：

$\alpha (v)\geq 0$ 所有人 $\alpha \in P$

$$
\Leftarrow \Rightarrow \alpha_1(v)\geq 0, . . . \alpha_l(v)\geq 0, \alpha_1(v)\leq 0, . . . , \alpha_m(v)\leq 0
$$

$$
\Leftarrow \Rightarrow \alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)\geq 0, . . . , \alpha_l(v)\geq 0
$$

所以 F(P) 是集合的闭包

$$
\{v\in V|\alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)>0, . . . , \alpha_l(v)>0\}
$$

集合是相对于$\mathscr{H}$的一个面F，因为S的每个元素都是$\alpha_1, . . . , \alpha_l$的线性组合，其中系数要么都是$\geq 0$，要么都是$\leq 0$。此外，如果$\beta =u_1\alpha_1+\cdots +u_l\alpha_l\in S$，

$$
\beta \in P(F)\Leftarrow \Rightarrow u_{m+1}\geq 0, . . . , u_l\geq 0
$$

$\Leftarrow \Rightarrow \beta \in S_+(C)$ 或 $(-\beta \in S_+(C)$ 和 $u_{m+1}=. . .=u_l= 0)$

$$
\Leftarrow \Rightarrow \beta \in S_+(C)\cup Q = P
$$

所以 P(F) = P。

b) 设 $F\in \mathscr{F}$。显然$P(F)\in \mathscr{P}$。另一方面，F 包含在相对于 $\mathscr{H}$ 的腔室封闭中（第 V, §1, no. 3 章，公式 (6)），相对于该腔室壁的集合的小面也是如此（第 V, §1, no. 4 章，第 9 条）。因而，对于所有 $\alpha \in T\}$，$\overline{F}$ 是形式 $\{v\in V|\alpha (v)\geq 0$，其中 T 是 S 的子集，我们可以清楚地认为它等于 P(F)。因而，$\overline{F}= F(P(F))$。 Q.E.D.

如果 $P\in \mathscr{P}$，则认为满足 P = P(F) 的面 F 与 P 相关联；我们用 F(P) 表示。我们将扩展这些约定应用于$(\mathfrak{g},\mathfrak{h})$是分裂的还原的情况。

#### 命题 12 {#lie-viii-s3-prop-12 .statement tag=0109}

令R中的$\mathscr{H}$为$\mathfrak{h}_{\mathbf{R}}$超平面由……组成集合根核集合。 令$\mathscr{F}$为$\mathfrak{h}_{\mathbf{R}}$相对于$\mathscr{H}$的面的集合。 令$\mathscr{S}$为$(\mathfrak{g},\mathfrak{h})$的抛物线子代数的集合。 对于每个$\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P\in \mathscr{S}$，令$F(\mathfrak{p})$为与P相关的面。那么$\mathfrak{p} \rightarrow F(\mathfrak{p})$是从$\mathscr{S}$到$\mathscr{F}$的双射。 如果$\mathfrak{p}_1,\mathfrak{p}_2\in \mathscr{P}$，

$$
\mathfrak{p}_1\supset \mathfrak{p}_2\Leftarrow \Rightarrow F(\mathfrak{p}_1)\subset \overline{F(\mathfrak{p}_2)}
$$

这紧随引理 3 而来。

#### 例 {#lie-viii-s3-n4-exa-1 .statement tag=010A}

$(\mathfrak{g},\mathfrak{h})$ 包含于 Borel 代数 $\mathfrak{b}$ 的抛物线子代数的小面相应的是包含在与 $\mathfrak{b}$（上面的cf. 注）相关的腔室封闭中的小面。

#### 命题 13 {#lie-viii-s3-prop-13 .statement tag=010B}

令$\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$为$(\mathfrak{g},\mathfrak{h})$的抛物线子代数、$\alpha \in P$的Q集合，使得$-\alpha  \notin P$和$\mathfrak{s}=\mathfrak{h}+\mathfrak{g}^{P\cap(-P)}$。 那么$\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{g}^Q,\mathfrak{s}$在$\mathfrak{g}$中还原，$\mathfrak{g}^Q$是$\mathfrak{p}$的最大幂零理想和$\mathfrak{p}$的幂零根。 $\mathfrak{p}$的中心是零。

根据命题，$2,\mathfrak{s}$ 是$\mathfrak{g}$ 的约简，$\mathfrak{g}^Q$ 是$\mathfrak{p}$ 的幂零理想。如果 $\mathfrak{n}$ 是 $\mathfrak{p},\mathfrak{g}^Q\subset \mathfrak{n}\subset \mathfrak{h}+\mathfrak{g}^Q$ 的最大的幂零理想（命题 2 (i)）；如果$x\in \mathfrak{n}\cap \mathfrak{h}$，ad$_{\mathfrak{p}}x$是幂零的，所以$\alpha (x) = 0$对于所有$\alpha \in P$，因而$x= 0$；这就证明了$\mathfrak{n}=\mathfrak{g}^Q$。从$[\mathfrak{h},\mathfrak{g}^Q] =\mathfrak{g}^Q$开始，$\mathfrak{p}$包含于$\mathfrak{g}^Q$的幂零根基因此等于$\mathfrak{g}^Q$。让$z=h+\sum_{\alpha\in P}u_{\alpha}$（其中$h\in \mathfrak{h}, u_{\alpha}\in \mathfrak{g}^{\alpha}$）为

$\mathfrak{p}$ 中心元素。对于所有$h'\in \mathfrak{h}, 0 = [h', z] =\sum\alpha (h')u_{\alpha}$，因而$u_{\alpha}= 0$对于所有$\alpha \in P$；由此可见，$[h,\mathfrak{g}^{\beta}] = 0$适用于所有$\beta \in P$，因而$h= 0$。

### 5. 非分裂情形

#### 命题 14 {#lie-viii-s3-prop-14 .statement tag=010C}

设$k'$为$k$和$\mathfrak{g}'=\mathfrak{g}\otimes_kk'$的扩张。设$\mathfrak{m}$为$\mathfrak{g}$和$\mathfrak{m}'=\mathfrak{m}\otimes_kk'$的子代数。如果 $\mathfrak{m}'$ 是抛物线（分别为 Borel ），则 $\mathfrak{g}',\mathfrak{m}$ 的子代数是 $\mathfrak{g}$ 的抛物线（分别为 Borel ）子代数。

根据命题8和命题11，足以证明$\mathfrak{g}$的$\mathfrak{m}$包含分裂嘉当子代数。令$\mathfrak{b}$为$\mathfrak{g}$的博雷尔子代数。那么 $\mathfrak{b}'=\mathfrak{b}\otimes_kk'$ 是 $\mathfrak{g}'$ 的博雷尔子代数，所以 $\mathfrak{m}'\cap \mathfrak{b}'$ 包含嘉当子代数 $\mathfrak{g}'$（命题 10）。设$\mathfrak{t}$为$\mathfrak{m}\cap \mathfrak{b}$的嘉当子代数。那么$\mathfrak{t}\otimes_kk'$是$\mathfrak{m}'\cap \mathfrak{b}'$的嘉当子代数，因此是$\mathfrak{g}'$（第VII, §3, no. 3章，第3条）。因而，$\mathfrak{t}$是$\mathfrak{g}$的嘉当子代数，并且由于它包含在$\mathfrak{b}$中，所以它是分裂。

#### 定义 3 {#lie-viii-s3-def-3 .statement tag=010D}

令 $\mathfrak{a}$ 为半单（或更一般地还原）李代数，且$\overline{k}$ 代数闭包为 $k$。如果 $\mathfrak{m}\otimes_k\overline{k}$ 是 $\mathfrak{a}\otimes_k\overline{k}$ 的抛物线（分别 Borel ）子代数，则 $\mathfrak{a}$ 的子代数 $\mathfrak{m}$ 被称为抛物线（分别 Borel ）。

如果 $\mathfrak{a}$ 是可分割的，则第 14 条命题表明，这个定义相当于定义 2（分别相当于定义 1）。

#### 命题 15 {#lie-viii-s3-prop-15 .statement tag=010E}

令$\mathfrak{a}$为李代数的约简，$k'$扩张为$k$的约简，$\mathfrak{m}$子代数为$\mathfrak{a}$的约简。那么$\mathfrak{m}$是$\mathfrak{a}$的抛物线（分别是Borel）子代数当且仅当$\mathfrak{m}\otimes_kk'$是$\mathfrak{a}\otimes_kk'$的抛物线（分别是Borel）子代数。

这紧随第 14 号提案而来。

### 习题{#lie-viii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
