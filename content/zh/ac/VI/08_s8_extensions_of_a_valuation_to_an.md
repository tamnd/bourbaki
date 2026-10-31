---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 8
section_title: Extensions of a valuation to an algebraic extension
lang: zh
source: ac-i-vii
book_pages: 416-431, 461-469
pdf_pages: 0434-0449, 0479-0487
extraction: ocr
subsections:
    - "no": 1
      title: RAMIFICATION INDEX. RESIDUE CLASS DEGREE
      page: 416
      pdf_page: 434
    - "no": 2
      title: EXTENSION OF A VALUATION AND COMPLETION
      page: 418
      pdf_page: 436
    - "no": 3
      title: THE RELATION $\sum_i e_i f_i \leq n$
      page: 420
      pdf_page: 438
    - "no": 4
      title: INITIAL RAMIFICATION INDEX
      page: 422
      pdf_page: 440
    - "no": 5
      title: THE RELATION $\sum_i e_i f_i = n$
      page: 423
      pdf_page: 441
    - "no": 6
      title: VALUATION RINGS IN AN ALGEBRAIC EXTENSION
      page: 427
      pdf_page: 445
    - "no": 7
      title: THE EXTENSION OF ABSOLUTE VALUES
      page: 428
      pdf_page: 446
statements: 36
exercises: 21
content_sha256: de0a56780994fe3e45bcc423dde7030da4219fba24df1f43b2597df8b11f0d86
translated_from: content/en/ac/VI/08_s8_extensions_of_a_valuation_to_an.md
translation_method: google
source_content_sha256: cdeab4f8e3ec406096d5a84060f974fac6c1348ec20e61d5f464c6c18df5b822
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4155c6ee236a5de7f4ead620f10c6ec80f5c6ff974781dfd1abe50fa8b5907ab
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 8. 扩张对代数的评估扩张

### 1. 衍生指标。 剩余类类次数

令$\mathbf{K}$为域，$\mathbf{L}$扩张为$\mathbf{K}$，$\mathbf{A}'$为$\mathbf{L}$的估值环。正如在§ 1, no. 4中所见，环$\mathbf{A} = \mathbf{K} \cap \mathbf{A}'$是环对$\mathbf{K}$的估值，并且
$$
m(\mathbf{A}) = m(\mathbf{A}') \cap \mathbf{K}.
$$
如果$v'$是与$\mathbf{A}'$相关的估值，则$v'$至$\mathbf{K}$的限制$v$是与$\mathbf{A}$相关的$\mathbf{K}$的估值； $v$阶群$\Gamma_v$是$v'$阶群$\Gamma_{v'}$子群。

#### 定义 1 {#ac-vi-s8-def-1 .statement tag=04W4}

*指标* $[\mathfrak{p}_v : \Gamma_{v'}]$ *被称为* $v'$ *超过* $v$ *（或超过* $\mathbf{K}$*）的分支指标，并表示为* $e(v'/v)$ *（或* $e(A'/A)$，*或有时* $e(L/K)$*）。

这个指标是自然数或$+\infty$。如果$v'_0$是$v'$*等价*的估值，$e(v'/v)$也称为$v'_0$*超过*$v$的分支指标。如果 $e(v'/v) = 1$，$v'$ 被称为在 $v$ 上“无分支”。

另一方面，$v$的剩余类域$\kappa(\mathbf{A})$被识别为$v'$的剩余类域$\kappa(\mathbf{A}')$的子域。

#### 定义 2 {#ac-vi-s8-def-2 .statement tag=04W5}

*次数* $[\kappa(\mathbf{A}') : \kappa(\mathbf{A})]$ *称为* $v'$ *超过* $v$ *（或超过* $\mathbf{K}$*）的剩余类类次数，并表示为* $f(v'/v)$ *（或* $f(A'/A)$， *或有时*$f(L/K)$*）。

这个次数是自然数或$+\infty$。

#### 引理 1 {#ac-vi-s8-lem-1 .statement tag=04W6}

*设*$\mathbf{K}, \mathbf{K}', \mathbf{K}''$*为三个域，使得*$K \subset K' \subset K''$、$v''$*对*$K''$*和*$v$*和*$v'$*其限制到*$\mathbf{K}$*和*进行评估$\mathbf{K}'$。 *然后还有关系:*
$$(1)\quad e(v''/v) = e(v''/v') e(v'/v), \qquad f(v''/v) = f(v''/v') f(v'/v).$$

这是显而易见的。

#### 引理 2 {#ac-vi-s8-lem-2 .statement tag=04W7}

令$K$为域，$L$为次数$n$的$K$的有限扩张，$v'$对$L$和$v$的估值为限制至$K$。然后不等式

$$
e(v'/v) f(v'/v) \leq n
$$

持有；特别是$e(v'/v)$和$f(v'/v)$是有限的。

让我们分别取自然数、$r$和$s$不大于$e(v'/v)$和$f(v'/v)$。足以证明$rs \leq n$。鉴于$r$的定义，存在$L$（$1 \leq i \leq r$）的元素$x_i$，使得$i \neq j$有$v'(x_i) \not\equiv v'(x_j)$（模$\Gamma_v$）。鉴于$s$的定义，存在$v'$的环$A'$元素$y_k$（$1 \leq k \leq s$），其中$\kappa(A')$中的典范像$\bar{y}_k$线性无关$\kappa(A)$；显然 $v'(y_k) = 0$ 对于所有$k$。我们将证明$rs$元素$x_i y_k$在$K$上是线性独立的，这肯定会建立不等式$rs \leq n$。

假设存在形式的非平凡线性关系

$$
\sum_{i,k} a_{ik} x_i y_k = 0 \quad (a_{ik} \in K).
$$

让我们选择指标$j, m$这样

$$
v'(a_{jm} x_j y_m) \leq v'(a_{ik} x_i y_k)
$$

每有序对 $(i, k)$；然后$a_{jm} \neq 0$。如果 $i \neq j$，那么 $v'(a_{ik} x_i y_k) = v'(a_{jm} x_j y_m)$ 是不可能的，因为这意味着

$$
v'(x_i) - v'(x_j) = v'(a_{jm}) - v'(a_{ik}) \in \Gamma_v,
$$

与$x_i$的选择相反。将 (3) 乘以 $(a_{jm} x_j)^{-1}$，我们得到关系 / 形式

$$
\sum_k b_k y_k + z = 0, \text{ where } b_k = \frac{a_{jk} x_j}{a_{jm} x_j} \in A', \quad z \in A'
$$

和$v'(b_k) \geq 0, v'(z) > 0$。 从而，$\kappa(A')$，关系，共形式$\sum_k \bar{b}_k \bar{y}_k = 0$。与$b_m = 1$一样，这个与……矛盾假设是在$y_k$制作的。

#### 命题 1 {#ac-vi-s8-prop-1 .statement tag=04W8}

令$K$为域，$L$为$K$的代数扩张，$v'$为$L$的估值，$v$其限制至$K$以及$A$和$A'$ $v$ 和 $v'$ 中的环。那么$\Gamma_{v'}/\Gamma_v$是挠元群，$\kappa(A')$是$\kappa(A)$的代数扩张。

令$(L_\alpha)$为$L$的有限子扩张族；让我们写$\Gamma_\alpha = v'(L_\alpha^*)$。 群$\Gamma_{v'}$是$\Gamma_\alpha$的右有向族由……组成的并；由于群 $\Gamma_\alpha/\Gamma_v$ 是有限的 (引理 2)，$\Gamma_{v'}/\Gamma_v$ 是挠元群。该论证类似于证明$\kappa(A')$是$\kappa(A)$的代数扩张。

#### 推论 1 {#ac-vi-s8-prop-1-cor-1 .statement tag=04W9}

*$v'$的高度等于$v$的高度。*

这是从命题 1 和下面的引理得出的：

#### 引理 3 {#ac-vi-s8-lem-3 .statement tag=04WA}

*令$G'$为$G$和$\mathscr{G}'$（或$\mathscr{G}$）的全序群、$G$子群和$G'$（或$G$）的孤立子群的集合。 映射$H' \mapsto H' \cap G$映射$\mathscr{G}'$到$\mathscr{G}$。如果 $G'/G$ 是挠元群，则映射是双射的。*

显然$H' \in \mathscr{G}'$蕴含$H' \cap G \in \mathscr{G}$。 现在令 $H \in \mathscr{G}$；令$H'$表示$x' \in G'$的集合，使得存在$h \in H$满足$-h \leq x' \leq h$；立即验证$H'$是$G'$的孤立子群；那么$H' \cap G = H$，因为$H$是孤立的；因此映射 $H' \mapsto H' \cap G$ 是满射。 Suppose finally that $G'/G$ is a torsion group; let $H'_1$ and $H'_2$ be two isolated subgroups of $G'$ such that $H'_1 \cap G = H'_2 \cap G$; then, for example, $H'_1 \supset H'_2$ (cf. § 4, no. 4); then $H'_1/H'_2$ is a totally ordered group and is isomorphic to a quotient group of $H'_1/(H'_1 \cap G)$ which itself is identified with a subgroup of $G'/G$; hence $H'_1/H'_2$ is a torsion group and therefore reduces to 0.

#### 推论 2 {#ac-vi-s8-lem-3-cor-2 .statement tag=04WB}

*要使 $v'$ 不合适（对应高度 1），$v$ 不合适（对应高度 1）是充分必要的。*

#### 推论 3 {#ac-vi-s8-lem-3-cor-3 .statement tag=04WC}

*假设$L$是$K$的有限扩张。为了使 $v'$ 离散，$v$ 离散是充分必要的。*
如果 $v'$ 是离散的，$\Gamma_{v'}$ 同构于 $\mathbf{Z}$ 的非零子群（推论 2），因此也同构于 $\mathbf{Z}$。相反，如果$v$是离散的，则$\Gamma_v$与$\mathbf{Z}$同构的，$\Gamma_{v'}/\Gamma_v$是有限群（引理2）；因而 $\Gamma_{v'}$ 是秩 1 的有限生成交换律群并且无扭转；因此它与 $\mathbf{Z}$ 同构的。

### 2. 扩张评估和完成

#### 定义 3 {#ac-vi-s8-def-3 .statement tag=04WD}

*假设$K$在场，$v$对$K$和$L$扩张的估值为$K$。 $L$上的估价族$(v'_i)_{i \in I}$其中扩展$v$，并且使得$L$延伸$v$的每个估价相当于唯一的$v'_i$被称为$v$的扩张的完整系统到$L$.*

#### 命题 2 {#ac-vi-s8-prop-2 .statement tag=04WE}

*令$K$在场，$v$对$K$进行估值，$\hat{K}$完备的$K$相对于$v$，$\hat{v}$$v$至$\hat{K}$的连续扩张，以及$L$ 扩张 $K$ 次数 $n$。
(a) 设$v'$为$L$延伸$v$的估值；令$\hat{L}_{v'}$表示$L$相对于$v'$和$8'$的完成，$v'$到$\hat{L}_{v'}$的连续扩张；识别$\hat{K}$与$\hat{L}_{v'}$中$K$的闭包，
$$
e(\hat{v}'|\hat{v}) = e(v'|v), \quad f(\hat{v}'|\hat{v}) = f(v'|v),
$$
$$
[\hat{L}_{v'} : \hat{K}] \leq n,
$$
$$
e(v'|v)f(v'|v) \preceq [\hat{L}_{v'} : \hat{K}].
$$
(b) *对$L$扩展非不当估值$v$的每一个集合都是有限的。让$v'_1, \ldots, v'_s$表示对$L$扩展* v的成对独立评估，使得对L扩展v的每个评估都依赖于v_i'之一；设 L_i 为域 L，其中拓扑由 v_i' 定义，$\hat{L}_i$ 其完成；我们写$n_i = [\hat{L}_i : \hat{K}]$。然后典范映射

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

（通过连续性延伸对角线映射 $L \to \prod_{i=1}^s L_i$）是满射，其核是 $\hat{K} \otimes_K L$ 的雅各布森根式，并且

$$
\sum_{i=1}^s n_i \leq n.
$$

我们首先证明(a)。假设 v 不是不恰当的。由于 v 和 $\hat{v}$（分别为 $v'$ 和 $\hat{v}'$）具有相同的阶群和相同的剩余类域（§ 5, no. 3、命题 5 (b) 和 (f)），因而 (4) 成立。我们通过引理 2 从中推导出 (6)。最后，L 生成的 $\hat{L}_{v'}$ 的向量子$\hat{K}$空间是闭的（§ 5, no. 2，命题 4 的推论）并且处处稠密，因此等于 $\hat{L}_{v'}$；这表明 (5)。

我们现在转到(b)。我们仍然可以假设 v 不是不恰当的。令 $(v_1', \ldots, v_r')$ 为 L 上的任何有限族成对独立估值，在 $\prod_{i=1}^r L_i$ 中延伸 L 的 v. 像，在对角线下映射处处稠密 (§ 7, no. 2, 定理 1) 且 $\prod_{i=1}^r L_i$ 稠密于$\prod_{i=1}^r \hat{L}_i$。因而，$\prod_{i=1}^r \hat{L}_i$中$\hat{K} \otimes_K L$的典范像到处都是稠密的。另一方面，这个像是$\prod_{i=1}^r \hat{L}_i$的向量子$\hat{K}$空间；由于通过 (5) $\prod_{i=1}^r \hat{L}_i$ 的有限维超过$\hat{K}$，$\hat{K} \otimes_K L$ 的像是闭集（§ 5, no. 2，命题 4 的推论），因此等于 $\prod_{i=1}^r \hat{L}_i$。由于 K 上的 $\hat{K} \otimes_K L$ 的维数是 n，因而$\sum_{i=1}^r n_i \leq n$。这特别表明整数 r 在上面以 n 为界，并显示 (b) 的第一个断言。

我们现在采用$(v_1', \ldots, v_s')$，如叙述。事实是

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

是满射且关系 (7) 已被证明。仍有待验证$\phi$的核n是$\hat{K} \otimes_K L$的雅各布森根式$t$。因为$\prod_{i=1}^s \hat{L}_i$是半单，$t \subset n$。另一方面，对于$\hat{K} \otimes_K L$的每个最大理想m，商域$L(m) = (\hat{K} \otimes_K L)/m$是$\hat{K}$和L在K上的复合扩张（代数，

章VIII, § 8、命题1)。存在对 L(m) 延伸 $\vartheta$ (§ 3, no. 3, 命题 5) 的估值 w； w 的限制 $v'$ 至 L 扩展 $v$。由于 $[L(m): \hat{K}]$ 是有限的，$L(m)$ 对于 w ($§ 5$, no. 2, 命题 4) 是完备的。现在$L(m)$中L的闭包是域包含$\mathbf{K}$和L，因此等于$L(m)$。因而，$L(m)$ 等同于完成$\hat{L}_{v'}$，并且 m 是$\hat{K} \otimes_K L$ 的典范映射到$\hat{L}_{v'}$ 的核。现在，到假设，存在指标$i$，使得$v'$和$v'_i$是相关的； 从而$L_{v'} = L_i$（$§ 7$、no. 2、命题 3）。因而$n \subset m$，证明$n \subset r$并完成证明。

#### 推出 1 {#ac-vi-s8-prop-2-cor-1 .statement tag=04WF}

*如果 K 相对于 v 是完整的并且 v 不是不恰当的，则扩展 v 的 L 的两个估值是相关的。*

这是从$\hat{K} \otimes_K L = L$开始的。

#### 推出 2 {#ac-vi-s8-prop-2-cor-2 .statement tag=04WG}

*如果$\hat{K}$或L可在K上分离，则典范映射*

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*是同构*。

$\hat{K} \otimes_K L$ 的雅各布森根式则为零 (*代数*, 章 VIII, § 7, no. 3, 定理 1)。

#### 注 {#ac-vi-s8-n2-rem-1 .statement tag=04WH}

命题 2 (b) 表明 $\hat{K}$ 和 L 在 K 上的每个复合扩张 (*代数*, 章 VIII, § 8) 与其中一个完成$\hat{L}_i$ 同构，并且它们是复合的扩张其中没有两个是同构的。

### 3.关系$\sum_i e_i f_i \leq n$

令 K 为域，$v$ K 的估值，L K 的次数 $n$ 的有限扩张。令$(v'_1, \ldots, v'_r)$为L延伸$v$的估值*其中没有两个是等价的；如果*它们是*独立的*（如果$v$的高度为1，情况总是如此），那么

$$
\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n
$$

命题 2 (公式 (6) 和 (7))。我们将看到这个结果在一般情况下是正确的。准确地说：

#### 定理 1 {#ac-vi-s8-thm-1 .statement tag=04WI}

*设 K 为域，v 为 K 的估值，L 为次数 n 的 K 的有限扩张。然后：*

(a) *v 到 L 的扩张的每个完整系统 $(v'_i)_{i \in I}$ 都是有限的。*

(b) $\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n$ 和更不必说 $\operatorname{Card}(I) \leq n$

(c) *环和$v'_i$ 中没有两个在包含方面具有可比性。*

由于如果$v$不合适，定理是微不足道的，因此我们假设$v$不是不合适的。令 $(v'_1, \ldots, v'_s)$ 为 L 延伸 $v$ 的任何有限估值族，不

关系$\sum_i e_i f_i \leq n$

其中两个是等价的。我们首先要证明$\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$。这就证明了(a)和(b)。

我们通过归纳对 s 进行论证，因此假设不等式已针对 0, 1, ..., s - 1 估值的情况成立。我们区分两种情况。

(1) 假设至少存在两个独立的估值$v'_i$。则存在 $[1, s]$ 的 (§ 7, no. 2, 注 1) 划分 $[1, s] = I_1 \cup \ldots \cup I_t$ 使得：
(i) 要使$v'_i$和$v'_j$相关，$i$和$j$属于与相同的$I_k$是必要且充分的；
(ii) 所有 $k$ 的卡$(I_k) < s$。

我们每个$I_k$指标$i(k)$都有选择。让$\hat{L}_{i(k)}$表示$L$相对于$v'_{i(k)}$和$n(k) = [\hat{L}_{i(k)} : \hat{K}]$的完成。对于$L$上的所有$i \in I_k$、$v'_i$定义，拓扑与$v'_{i(k)}$（§ 7, no. 2、命题3）相同，因此可以扩展到$\hat{L}_{i(k)}$上的估价$\bar{v}'_i$，其限制到$\hat{K}$为0。由于$i \in I$的$v'_i$没有两个是等价的，$\bar{v}'_i$也是如此。 归纳假设应用于有序对$(\hat{K}, \hat{L}_{i(k)})$表明，凭借命题2（a），公式（4），$\sum_{i \in I_k} e(v'_i/v)f(v'_i/v) \leq n(k)$。作为 $\sum_{k=1}^t n(k) \leq n$ (命题 2 (b), 公式 (7))，当然是 $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$。

(2) 现在我们讨论任意两个 $v'_i$ 是相关的情况。设$A'_i$为$v'_i$($1 \leq i \leq s$)的环；为$v$的环写$A$，为所有$i$写$A'_i \cap K = A$。设$B'$为$A'_1, \ldots, A'_s$生成的$L$的子环；我们写$B = B' \cap K$；然后$B \supseteq A$。那么$B$是$K$的估价$w$的环，$B'$环是$w'$的估价，这是不恰当的，扩展$w$（§ 7, no. 2，命题） 4); 域$\kappa(B')$是次数$f(w'/w)$$\kappa(B)$扩张。考虑$\kappa(B')$中$A'_i$和$A$的典范像$\bar{A}'_i, \bar{A}$；那么$\bar{A}$是$\kappa(B)$上的评估$\bar{v}$的环，$\bar{A}'_i$是$\kappa(B')$上的评估$\bar{v}'_i$延伸$\bar{v}$的环。由于 $A'_i$ 生成 $B'$、$\bar{A}'_i$ 生成 $\kappa(B')$ 以及$\bar{v}'_i$ 并非全部相关（§ 7, no. 2、命题 4）。从证明的第一个部分开始，

$$
\sum_{i=1}^s e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq [\kappa(B') : \kappa(B)] = f(w'/w)
$$

因此

$$
\sum_{i=1}^s e(w'/w)e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq e(w'/w)f(w'/w) \leq n \quad \text{(no. 1, Lemma 1).}
$$

因此，如果我们证明，（a）和（b）的证明将完成

$$
f(\bar{v}'_i/\bar{v}) = f(\bar{v}'_i/v), \quad e(w'/w)e(\bar{v}'_i/\bar{v}) = e(v'_i/v).
$$

为此，我们注$v$和$\bar{v}$（分别是$v'_i$和$\bar{v}'_i$）具有相同的剩余类域（§ 4, no. 1，命题2的推论）；这就证明了第一个方程。对于第二个，由于§4, no. 3中的注，有以下交换律图表，其中行是正合序列，垂直箭头代表典范嵌入：

$$
\begin{array}{ccccccccc}
0 & \to & \Gamma_{\bar{v}} & \to & \Gamma_v & \to & \Gamma_w & \to & 0 \\
& & \downarrow & & \downarrow & & \downarrow & & \\
0 & \to & \Gamma_{\bar{v}_i'} & \to & \Gamma_{v_i'} & \to & \Gamma_{w'} & \to & 0
\end{array}
$$

我们推断有正合序列

$$
0 \to \Gamma_{\bar{v}_i'}/\Gamma_{\bar{v}} \to \Gamma_{v_i'}/\Gamma_v \to \Gamma_{w'}/\Gamma_w \to 0
$$

由章I, § 1, no. 4，命题2，证明第二个公式(8)。

要完成定理 1 的证明，还需要证明(c)。如果$v_i'$包含的环$v_j'$、$\Gamma_{v_i'}$与商群$\Gamma_{v_j'}/H$相同，$H$是孤立的子群（§ 4, no. 3）。作为复合典范映射

$$
\Gamma_v \to \Gamma_{v_j} \to \Gamma_{v_j'}/H = \Gamma_{v_i'}
$$

是单射，$H \cap \Gamma_v = \{0\}$, 从而 $H = \{0\}$ (引理 3, no. 1)。那么$v_i'$和$v_j'$是等价的，从而$i = j$。

#### 注 {#ac-vi-s8-n3-rem-1 .statement tag=04WJ}

估值$v_i'$($i \in I$)的环$A_i'$的交C是L中$A$的积分闭包(§ 1, no. 3，推论3到定理3)；此外，根据 (c) 和§ 7, no. 1、命题 1 和 2，C 是半局部环，对于所有 $i \in I$，其最大理想是交 $m_i = C \cap m(A_i')$ 和$A_i' = C$。

### 4. 初始分支指标

#### 定义 4 {#ac-vi-s8-def-4 .statement tag=04WK}

设 G 是有限指标的 G 的全序交换群和 H 子群。 The number of major subsets of G consisting of strictly positive elements and containing all the elements > O of H is called the initial index of H in G and denoted by $\varepsilon(G, H)$.

由于以下命题，这个初始指标是自然数：

#### 命题 3 {#ac-vi-s8-prop-3 .statement tag=04WL}

在定义 4的假设下，如果G的严格正元素的集合不存在最小元素，则对于所有H来说$\varepsilon(G, H) = 1$。如果存在G的至少元素 > O且$G'$表示子群它生成，则

$$
\varepsilon(G, H) = (G : (G \cap H)).
$$

在第一种情况下，令 x 在 G 中为元素 > 0。 $y \in G$ 的集合使得 $0 < y < x$ 是无限的，因此存在这个集合的两个元素，它们对模 H 不同且全等；它们的差是 H 的元素 z，使得 $0 < z < x$。因此，每个主要子集其中包含都是H包含x的严格正元素，因此G的所有元素> 0。

在第二种情况下，令 $x$ 为 G 的最小元素 >0，并令 $n$ 为满足 $nx \in H$ 的最小整数 >0。显然$n = (G : (G \cap H))$。另一方面，将$z \in G$的集合写为$M(y)$，使得$y \leq z \ (y \in G)$，立即可以看出定义4的主集合只是$M(x), M(2x), \ldots, M(nx)$。

#### 推论{#ac-vi-s8-n4-cor-1 .statement tag=04WM}

*初始指标 $\varepsilon(G, H)$ 除指标* $(G : H)$ *并且等于它，如果* $G$ *同构于* $\mathbf{Z}$。

特别是$\varepsilon(G, H) \leq (G : H)$。

#### 定义 5 {#ac-vi-s8-def-5 .statement tag=04WN}

*设* $K$ *为域、L* $K$、$w$ *对* $L$、$v$ *其限制到* $K$ *和* $\Gamma_w$的有限扩张 *和*$\Gamma_v$ *他们的阶群。 * $\Gamma_v$ *在* $\Gamma_w$ *中的初始指标称为* $w$ *相对于* $v$ *（或相对于* $K$*）的初始分支指标，并表示为* $\varepsilon(w/v)$。

从上述推论，在离散估值的情况下，$\varepsilon(w/v)$除$e(w/v)$和等式。

#### 命题 4 {#ac-vi-s8-prop-4 .statement tag=04WO}

*在定义 5的假设下，令* $A$ *和* $m$ *（分别* $A'$ *和* $m'$）*为环和估值理想* $v$ *（分别* $w$*）。 *然后*

$$
[A'/mA': A/m] = \varepsilon(w/v) f(w/v).
$$

$A'$ 包含 $mA'$ 的理想，不同于 $A'$ 对应到 $\Gamma_w$ 由……组成的主要子集元素 >0 和包含元素 >0 $\Gamma_v$（§ 3, no. 5，命题7 的推论）。因此，它们的数与 $\varepsilon(w/v)$ 相等，并且由于它们包含形式全序集，因此该数等于商环 $A'/mA'$ 的长度。现在$A'$上的长度1的模是$A'/m'$上的一维向量空间，因此$A$上的长度$f(w/v)$的模；因此，由于$A'/mA'$是长度$\varepsilon(w/v)$超过$A'$，它是长度$\varepsilon(w/v) f(w/v)$超过$A$，即超过$A/m$。

### 5.关系$\sum_i e_i f_i = n$

#### 命题 5 {#ac-vi-s8-prop-5 .statement tag=04WP}

*设* $K$ *为域，v 对* $K$，$A$ *其环，m 为理想值，L 为* $K$ *次数* 的有限扩张* $n$、$B$**$A$*在*$L$*和*$(v'_i)_{1 \leq i \leq s}$*完整闭包*$v$*到*$L$的扩张系统。 *然后*

$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v).
$$

设$A_i$为$v'_i$中的环；然后$A_i = B_{m_i}$，其中$m_i$贯穿$B$（no. 3，注）的极大理想族。令$q_i$为$mB$相对于$m_i$的饱和度（章II, § 2, no. 4）。由章V，推论3至命题1，no. 1，§ 2，典范同态$B/mB \to \prod_{i=1}^s B/q_i$为同构且$m_i$是B包含的唯一极大理想$q_i$。因此 $B/q_i$ 与 $(B/q_i)_{m_i}$ (章 II, § 3, no. 3, 命题 8) 典型同构，即
$$
B_{m_i}/mB_{m_i} = A_i/mA_i.
$$
因此，凭借 no. 4 的命题 4 得到典范同构 $B/mB \to \prod_{i=1}^s A_i/mA_i$、从而。

#### 推论{#ac-vi-s8-n5-cor-1 .statement tag=04WQ}

*使用相同的假设和记号，
$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n.
$$
我们知道$\varepsilon(v'_i/v) \leq \varepsilon(v'_i/v)$（no. 4，命题3的推论）和$\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n$（no. 3，定理1）。

#### 定理 2 {#ac-vi-s8-thm-2 .statement tag=04WR}

*使用命题 5 的假设和记号，以下条件是等价的：
(a) B 为有限生成A-模；
(b) B 为自由A-模；
（三）$[B/mB : A/m] = n;$
(d) 对于所有 i，$\sum_{i=1}^n \varepsilon(v'_i/v) f(v'_i/v) = n$ 和 $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$。

(a)和(b)的等价由引理1、§ 3, no. 6得出。显然 (b) 意味着 (c) (*代数*, 章 11, § 1, no. 5, 公式 (19))。 (c) 和 (d) 的等价由命题 5 的推论得出。 仍有待证明 (c) 蕴涵 (b)。

一般来说，如果M是A-模，我们将在$A/m$上用V(M)​​向量空间$M/mM$来表示。 假设(c)意味着$\dim(V(B)) = n$。 设$x_1, \ldots, x_n$为B的元素，其典范像位于V(B)形式基中V(B)，并令L$\subset B$为它们生成的子A模块。 由于 L 是无扭且有限生成的，因此它是自由的 (§ 3, no. 6, 引理 1)。 我们将会看到$B = L$。 设 $y \in B$；我们写$M = L + Ay$；这也是自由A-模。 典范嵌入$L \to M \to B$给典范同态$V(L) \to V(M) \to V(B)$。 As the ranks of L and M are $\leq n$, so are the dimensions of V(L) and V(M). 现在，通过假设，$V(L) \to V(B)$是满射，$V(B)$是n维，因此$V(L)$和$V(M)$是n维，$V(L) \to V(M)$是满射。 由于 M 是有限生成的，$L \to M$ 是满射（章 II, § 3, no. 2，推论 1 到命题 4）、从而 $L = M, y \in L$ 和 $B = L$。 因此B是自由的。

#### 注 (1) {#ac-vi-s8-n5-rem-1 .statement tag=04WS}

如果 v 是*离散*，则 $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ (no. 4) 和条件 (d) 约化到 $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) = n.$

#### 推论 1 {#ac-vi-s8-thm-2-cor-1 .statement tag=04WT}

*与记号相同的假设，进一步假设v是离散的并且L可分离。然后*

$$
\sum_{i=1}^{s} e(v_i'/v) f(v_i'/v) = n.
$$

那么 A 的积分闭包 B 就是秩 $n$ 的自由A-模，因为 A 是主理想整环（章 V, § 1, no. 6，推论 2 到命题 18）。

#### 推论 2 {#ac-vi-s8-thm-2-cor-2 .statement tag=04WU}

*令 K 为域，v 是 K 的离散估值，K 是完整的，L 是次数 n 的 K 的有限扩张。然后v承认一个唯一的（最多等价）扩张$v'$到L，$v'$的环A'是v和$e(v'/v) f(v'/v) = n$的环A上有限生成的自由模。*

adic 拓扑（其中 $m = m(A)$）； 环 A 是完备的，因为它在 K 中是封闭的。我们结论认为，由于 $A'/mA'$ 是有限维向量 ($A/m$)-空间 (no. 4, 命题 4)，A' 是有限生成A-模 (章 III, § 2, no. 9，推论 3 至命题 12)。因此它是免费的并且 $e(v'/v) f(v'/v) = n$

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

（no. 2，命题2）。 *是双射的。对于所有$x \in L$，特征多项式$P_{C_{L/K}}(x; X)$等于特征多项式$P_{C_{\hat{L}_i/\bar{K}}}(x; X)$（$1 \leq i \leq s$）的乘积；尤其，

$$
\begin{cases}
\operatorname{Tr}_{L/K}(x) = \sum_{i=1}^s \operatorname{Tr}_{\hat{L}_i/\bar{K}}(x) \\
N_{L/K}(x) = \prod_{i=1}^s N_{\hat{L}_i/\bar{K}}(x) \\
v(N_{L/K}(x)) = \sum_{i=1}^s n_i v_i'(x).
\end{cases}
$$

（（9）中的最后一个关系是有意义的，因为我们显然可以假设$v_i'$（根据推论2到no. 1的命题1的高度为1），就像v一样，在$\mathbf{R}$的子群中取它们的值。）

由于没有两个$v'_i$是等价的，并且它们的高度为1，因此它们是独立的，并且no. 2的命题2因此表明$e(v'_i/v) f(v'_i/v) \leq n_i$对于所有$i$和$\sum_{i=1}^s n_i \leq n$。因此，第一个断言是由这些不等式和关系$\sum_{i=1}^s e(v'_i/v) f(v'_i/v) = n$得出的。在$\hat{K} \otimes_K L$的同构$\phi$自同态$z \mapsto z(1 \otimes x)$（对于$x \in L$）转换为$\prod_{i=1}^s \hat{L}_i$的自同态，使每个因子保持不变，并在每个因子到乘法上减少$x$（$L$ 规范地嵌入其完成$\hat{L}_i$）； 从而断言与$x$的特征多项式和(9)的前两个公式有关。最后，令E为$\hat{K}$、包含$\hat{L}_i$的有限准伽罗瓦扩张；由于 $\hat{K}$ 是完整的且 $\hat{\nu}$ 的高度为 1，因此在延伸 $\hat{\nu}$ 的 E 上仅存在一个估价（最多等价）$w$（no. 2，推论 1 至命题 2）；那么，对于 E 的每个$\hat{K}$自同构$\sigma$，$w(\sigma(x)) = v'_i(x)$。因此
$$
\vartheta(N_{\hat{L}_i/\hat{K}}(x)) = n_i v'_i(x)
$$
(代数, 章 VIII, § 12, no. 2, 公式 (15))，证明了(9)的公式。

#### 推论 4 {#ac-vi-s8-thm-2-cor-4 .statement tag=04WV}

*在推论3的假设下，如果L是K的可分扩张，则每个$\hat{L}_i$都是$\hat{K}$的可分扩张。如果进一步L是K的伽罗瓦扩张，伽罗瓦群$\mathscr{G}$且$\mathscr{G}_i$表示B中$v'_i$理想的分解群（章V, § 2, no. 2，定义） 2), 那么$\hat{L}_i$是$\hat{K}$的伽罗瓦扩张，其伽罗瓦群同构于$\mathscr{G}_i$。*

显然$\hat{L}_i = \hat{K}(L)$；因此，如果 L 在 K 上可分，则 $\hat{L}_i$ 在 $\hat{K}$ 上可分（代数、章 V, § 7, no. 6、命题 10）。现在假设 L 是伽罗瓦。每个自同构$\sigma \in \mathscr{G}_i$在L上连续，拓扑由$v'_i$定义，事实上，$v'_i$的两个理想在包含方面没有可比性（§ 7, no. 2，推论1到定理1）必然意味着： $v'_i = v'_i \circ \sigma$乘定义共$\mathscr{G}_i$；因此$\sigma$可以通过连续性扩展到$\hat{L}_i$的$\hat{K}$自同构$\hat{\sigma}$。这证明$\hat{K}$的数-$\hat{L}_i$的自同构至少等于$\mathrm{Card}(\mathscr{G}_i)$。但由于估值$v'_i$是成对共轭低于$\mathscr{G}$（章V, § 2, no. 3，命题6），$s = (\mathscr{G}_i)$，从而
$$
\mathrm{Card}(\mathscr{G}_i) = n/s \leq n.
$$
另一方面，$n = sn$，由推论 3 得出；这证明$\hat{L}_i$是$\hat{K}$的伽罗瓦扩张，并且扩张通过自同构$\sigma \in \mathscr{G}_i$的连续性是$\hat{L}_i$唯一的$\hat{K}$自同构。

*注 (2)*.上述结果中的部分扩展适用于对*不一定可交换*域K（cf.§ 3, no. 1）进行估值的情况。令L为K的扩张域，令$v'$为L的估值，$v$为K和A'的限制，A分别为$v'$和$v$的估值环；然后定义了一个分支指标$e(v'/v)$，如no. 1；另一方面，$\kappa(A)$与$\kappa(A')$的子域等同，$v'$的（左）剩余类秩相对于$v$被定义为数$f(v'/v)$等于左侧的维数向量 $\kappa(A)$-空间$\kappa(A')$，如果维数是有限的，而$+\infty$则相反。然后，如果L是有限维$n$的左向量K空间，则no. 1的引理2及其证明保持不变。此外，如果K对于$v$完备，no. 5的推论2到定理2的断言（$u'$的存在除外）也有效（$n$将L的维数表示为左） 向量 K 空间），具有以下证明：

首先，L上的$v'$定义的拓扑是Hausdorff，并且与其左向量K空间结构兼容，因此$v$到L的两个扩张给出相同的拓扑 L ($§ 5$, no. 2, 命题 4)，证明这些扩张直到等价 ($§ 6$, no. 2)都是相同的。接下来我们证明，如果$m = m(A)$，$A'/mA'$是维数$e(v'/v) f(v'/v)$的左向量$(A/m)$空间。写出$e = e(v'/v)$，我们可以假设$v(K^*) = Z$和$v'(L^*) = e^{-1}Z$；令$u'$为L的元素，使得$v'(u') = e^{-1}$和K的$u$元素，使得$v(u) = 1$；因此$u = z{u'}^e$，其中$z \in L$使得$v'(z) = 0$。由于 m 由 $u$（作为 A 的左理想或右理想）、$mA' = {u'}^eA' = A'{u'}^e$ 生成，并且足以证明，对于 $0 \leq k \leq e - 1$，$A'{u'}^k/A'{u'}^{k+1}$ 是维数 $f(v'/v)$ 的左向量 $(A/m)$ 空间。但是 $t \mapsto t{u'}^k$ 是左A-模 A 的同构到左A-模 $A'{u'}^k$ 映射 $A'u'$ 到 $A'{u'}^{k+1}$，因此通过取商可以得到 $A'/A'u'$ 的 $(A/m)$ 同构$A'{u'}^k/A'{u'}^{k+1}$、从而我们的断言除以$f(v'/v)$、$u'$生成的的定义$A'$的最大理想。当 K 和 L 可交换时，证明是完备的（有限生成的无扭转 A 模是自由的，这一事实如$§ 3$、no. 6、引理 1 中所证明）。

### 6. 代数中的估值环扩张

#### 命题 6 {#ac-vi-s8-prop-6 .statement tag=04WW}

令 K 为域，$v$ K 的估值，A 为环，L K 的代数扩张，$A'$ A 在L 中的积分闭包。令 23 为 L 上环的集合，其中 $A'$ 的最大理想为扩展 $v$ 和 $\mathfrak{M}'$ 集合。那么映射$V \mapsto m(V) \cap A'$就是23的双射到$\mathfrak{M}'$，$m' \mapsto A'_{m'}$就是逆双射。

$A'$的每个最大理想$m'$使得$m' \cap A$是A的最大理想（章V, § 2, no. 1，命题1）并且$A'_{m'}$由L的评估环V主导（因此是L的估值延伸$v$）的环（$§ 1$，no. 2，推论到定理2）。 域L是L的有向子扩展族K的并，其在K上是有限的，并且在阶中看到$V = A'_{m'}$就足以证明$V \cap K = A'_{m'} \cap K$，对于所有$\alpha$。现在，如果我们写 $A'_\alpha = A' \cap K_\alpha$，$A'_\alpha$ 是 A 在 K 中的积分闭包，因此是 K 估值的环的交，其中扩展 $v$ 和这些环 $V_\alpha$ 在数中是有限的，并且是$A'_\alpha$ ($1 \leq i \leq n$) 的局部环 $(A'_\alpha)_{i|m_\alpha}$，其中$m'_{i\alpha}$ 是$A'_\alpha$ (no. 3, 注) 的不同最大理想；但$m' \cap A'_\alpha$是$m'_{i\alpha}$之一，因此$V \cap K_\alpha$等于相应的局部环$(A'_\alpha)_{m'_{i\alpha}} \subset A'_{m'}$，从而完成证明和$V = A'_{m'}$。相反，如果$V \in \mathfrak{V}$，则$A' \subset V$（§ 3, no. 3，命题 6），如果$m' = m(V) \cap A'$，则$m' \cap A = m$，因此$m'$是$A'$（章V, § 2, no. 1， 命题 1) 并且上述论证表明$V = A'_{m'}$。

#### 命题 7 {#ac-vi-s8-prop-7 .statement tag=04WX}

*设 K 为域、L K 和 f 的拟伽罗瓦扩展以及 L 的 $f'$ 位置，其中值位于相同的域 F 中。假设限制关闭且 $f'$ 为 K 重合。那么存在 L 的 K-自同构 s 使得 $f' = f \circ s$.*

令 A 为 K 公共的限制位置的环和 $f'$。 环关闭和$f'$包含A在L中的积分闭包$A'$（§ 1, no. 3，推论3到定理3），因此（章V, § 2, no. 3，推论1到命题 6) 存在L的K-自同构s，使得限制off和$f \circ s$到$A'$相等；如果$m'$是这些限制中的公共的核，则$m' \cap A$是A的最大理想，因此$m'$是$A'$以及$f'$和$f \circ s$的最大理想重合环 $A'_{m'}$；但到了命题 6，L支配$A'_{m'}$的唯一估值环是环$A'_{m'}$本身，因此$f'$和$f \circ s$位置的环是相同的。

#### 推论 1 {#ac-vi-s8-prop-7-cor-1 .statement tag=04WY}

*令 K 为域，v 对 K 的估值，L K 的准伽罗瓦扩展，以及 $v'$ 和 $v''$ v 到 L 的两个扩张。那么存在L的K-自同构s，使得$v''$等价于$v' \circ s$。*

设$f'$和$f''$为与$v'$和$v''$相关的K的位置；如果需要将替换放在等价位置，则可以假设它们都在v的剩余类域的代数闭包中取值（no. 1，命题1）。那么存在L的K-自同构s使得$f'' = f' \circ s$(命题7)；因此，凭借地点和估价之间的对应 (§ 3, no. 3)，$v''$ 相当于 $v' \circ s$。

#### 推论 2 {#ac-vi-s8-prop-7-cor-2 .statement tag=04WZ}

*设 K 为域，f 为 K 的位（分别为 v 对 K 的估价），L 为 K 的根数扩张。那么 f（分别为 v）到 L 的所有扩张都是等价的。*

L是准伽罗瓦扩展，其唯一的自同构是恒等式。因此，推论 2 由命题 7 得出（分别推论 1）。

#### 命题 8 {#ac-vi-s8-prop-8 .statement tag=04X0}

*令 K 为域，v 为 K 的估值，L K 的次数 n 的有限拟伽罗瓦扩展，$(v'_i)_{1 \leq i \leq g}$ v 的扩张到 L 的完整系统。那么$e(v'_i/v)$和$f(v'_i/v)$有值e和$\mathfrak{f}$独立于i。然后$ef g \leq n$。如果v的环A在L的积分闭包是有限生成A-模，那么$ef g = n$.*

这紧接着定理 1 (no. 3) 和 2 (no. 5)。

### 7.绝对值的扩张

#### 命题 9 {#ac-vi-s8-prop-9 .statement tag=04X1}

*设 K 为域，L K 的代数扩张，$\mathfrak{f}$ 为 K 上的绝对值值。那么 $\mathfrak{f}$ 可以扩展到 L 上的绝对值值。*

首先假设存在对 $K$ 的估值 $v$ 且实际值值使得 $f(x) = e^{-v(x)}$。 $L$ 存在估值$v'$，其限制到$K$ 相当于$v$（$§ 3$、no. 3、命题 5）。那么 $v'$ 的高度为 0 或 1（no. 1，推论 2 到命题 1），因此可以假设具有实数值。 映射 $x \mapsto e^{-v'(x)}$ 到 $K$ 的限制是绝对值等于 $f$，因此形式 $f^s$ 与 $s > 0$（*一般拓扑*、章 IX、$§ 3$、no. 2、命题 5)。我们结论

$$
x \mapsto e^{-v'(x)/s}
$$

是$L$上的绝对值延伸$f$。

现在假设 $f$ 不是超度量。然后将 $K$ 与 $\mathbf{C}$ 的子域进行识别，使得 $f(x) = |x|^s$ 其中 $0 \leq s \leq 1$ ($§ 6$, no. 4, 定理 2)。由于 $\mathbf{C}$ 是代数闭集，$L$ 等同于 $\mathbf{C}$ 的子域以及绝对值 $x \mapsto |x|^s$ 扩展 $f$。

#### 命题 10 {#ac-vi-s8-prop-10 .statement tag=04X2}

*令 $K$ 为域，$f$ $K$ 上的绝对值值，使得 $K$ 相对于 $f$ 而言是完整的且非离散的，而 $L$ 的代数扩张 $K$。那么$f$可以在$L$上唯一地扩展到绝对值$f'$，并且，如果$L$是有限次数$n$，那么*

$$
f'(x) = (f(N_{L/K}(x)))^{1/n}
$$

*对于所有人*$x \in L$。

$f'$ 的存在源自命题 9 及其唯一性（在$L$ 的每个有限子扩展上，因此在整个$L$ 上）源自$§ 6$、no. 4 的引理 2。令$f'$是$K$到代数闭包的唯一扩张，并假设$L$是有限次数$n$。我们知道$N_{L/K}(x) = \prod_{i=1}^n x_i$，其中每个$x_i$是$x$的共轭超过$K$（*代数*，章VIII，$§ 12$，no. 2，命题4）。鉴于$f'$的唯一性，所有$i$的$f'(x_i) = f'(x)$，从而规定的公式。

#### 命题 11 {#ac-vi-s8-prop-11 .statement tag=04X3}

*令 $K$ 为域，$f$ $K$，$\hat{K}$ 上的非超量绝对值，$K$ 相对于 $f$，$\hat{f}$ 的连续扩张的完成$\hat{K}$ 和 $L$ 扩张 $K$ 次数 $n$。

(a) *令$f'$为$L$上的绝对值延伸$f$；令$\hat{L}_{f'}$表示$L$相对于$f'$的完成，并令$\hat{K}$等同于$\hat{L}_{f'}$中$K$的闭包；然后*$[\hat{L}_{f'} : K] \leq n$。

(b) *在$L$上延伸$f$的绝对值在数中是有限的。如果它们由* $f'_1, \ldots, f'_s$ *表示，并且相对于* $f'_i$ *由* $\hat{L}_i$、*典范映射*完成$L$

$$
\hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*是同构并且*

$$
\sum_{i=1}^s [\hat{L}_i : \hat{K}] = n.
$$

(10)

证明与命题 2 (no. 2) 中的类似断言相同。参考文献

§ 7, no. 2、定理1； § 5, no. 2，命题 4 的推论应替换为以下内容

§ 7, no. 3、定理2；拓扑向量空间、章 I,
§ 2, no. 3，推论 1 至定理 2。

观察两个扩张到L，其中定义相同的拓扑是相等的（一般拓扑，章IX, § 3, no. 2，命题5）。最后，由于 $f$ 不是超度量，K 的特征为 0，因此 $\hat{K} \otimes_K L$ 的雅各布森根式为零。

注
(1) 命题 11 (b) 表明，K 上$\hat{K}$ 和 L 的每个复合扩张都同构于完成$\hat{L}_i$ 之一，并且它们是复合扩张，其中没有两个是同构的。
（2）我们知道补全$\hat{K}$和$\hat{L}_i$同构于$\mathbf{R}$或$\mathbf{C}$（$§ 6$，no. 4，定理2）。如果 $\hat{K}$ 与 $\mathbf{C}$ 同构，则对于所有 $i$，$\hat{L}_i$ 也同构，并且 (10) 表明扩张 $f_i'$ 的数 *等于 n*。如果$\hat{K}$同构于$\mathbf{R}$（对于$K = \mathbf{Q}$则为例），令$r_1$（或$r_2$）表示指标$i$的数，使得$\hat{L}_i$为同构于$\mathbf{R}$（分别为$\mathbf{C}$）；那么(10)可以写成：

$$
r_1 + 2r_2 = n.
$$

#### 命题 12 {#ac-vi-s8-prop-12 .statement tag=04X4}

*设 K 为域，f 是 K 上的绝对值，L K 的准伽罗瓦扩展，以及 $f'$ 和 $f''$ 两个扩张到 L。那么存在 L 的 K-自同构 s 使得 $f'' = f' \circ s$.*

如果$f$是超度量的，推论1到命题7（no. 6）表明存在L的K-自同构s，使得$f''$和$f' \circ s$等价绝对值；那么存在实数 $a > 0$，使得 $f''(x) = (f'(s(x)))^a$ 对于所有 $x \in L$。若$f$不妥，取$x \in K^*$使得$f(x) \neq 1$，则可知$a = 1$。如果$f$不合适，$f'$和$f''$也不合适（推论2到命题1，no. 1），并且s可以被视为恒等式自同构。

如果$f$不是超度量，则存在L的Q同构$u', u''$到$\mathbf{C}$的子域和实数指数$a' > 0, a'' > 0$，使得$f'(x) = |u'(x)|^{a'}$和

$$
f''(x) = |u''(x)|^{a''}
$$

对于所有 $x \in L$（$§ 6$、no. 4、定理 2）。取$x = 2$，可知$a' = a''$。 $u'$和$u''$的限制到K 扩展，通过连续到同构$u_1$和$\hat{K}$的$u_2$到$\mathbf{R}$（分别为$\mathbf{C}$）。那么$u_2 \circ \bar{u}_1^{-1}$是*值*域$\mathbf{R}$（或$\mathbf{C}$）的自同构，因此是恒等式（或自同构$c : \zeta \to \bar{\zeta}$）。 替换如果需要$u'$乘以$c \circ u'$，则可以看出，$u'$和$u''$对K的限制可以假设为重合。通过公共的限制将K与$\mathbf{C}$的子域识别，$u'$和$u''$是L到$\mathbf{C}$的子域的K同构。由于L是K的拟伽罗瓦扩展，因此存在L的K-自同构s，使得$u'' = u' \circ s$；从$a' = a''$开始，我们立即推断出$f'' = f' \circ s$。

注 (3)。如果$\hat{K}$同构于$\mathbf{R}$，命题12表明$L$的所有补全$\hat{L}_t$（在命题11的记号中）同构于一个另一个。因此，对于上面的记号或注 2，要么是 $r_1 = n$ 和 $r_2 = 0$，要么是 $r_1 = 0$ 和 $2r_2 = n$。

### 习题 {#ac-vi-s8-exercises}

§ 8](exercises/s8/)参见[习题。
