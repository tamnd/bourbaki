---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Complements on Hilbert spaces
appendix: true
lang: zh
source: int-vii-ix
book_pages: INT IX.118-INT IX.119
pdf_pages: 0284-0288, 0300-0301
extraction: ocr
subsections:
    - "no": 1
      title: Trace of a quadratic form with respect to another$^{(1)}$
      page: 0
      pdf_page: 284
    - "no": 2
      title: Hilbert–Schmidt mappings$^{(2)}$
      page: 104
      pdf_page: 286
statements: 5
exercises: 9
content_sha256: 2be2f501c38b9877a7ca7d1e61c4ab0c5946963844b745f3a7c9d2c06798d604
translated_from: content/en/int/IX/A_a_complements_on_hilbert_spaces.md
translation_method: google
source_content_sha256: 345b39c6aa42db2dbb13f3b4da3d834dda0b94e5c0750c5ee630d5f4b9b588d5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 2f062710836ab464c662faf796196abd9958b8093bedb260d952aa926055c4b1
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附件

# 希尔伯特空间的补充

### 1. 二次方形式相对于另一个$^{(1)}$ 的迹

在这个数中，我们用$E$表示实数向量空间，用$Q, H$表示$E$上的两个正二次形式。存在两个对称的双线性形式、$(x, y) \mapsto (x|y)_Q$和$(x, y) \mapsto (x|y)_H$，其特征为
$$
Q(x) = (x|x)_Q , \quad H(x) = (x|x)_H
$$
对于所有$x \in E$。

一称为 Q 相对于 H* 的迹，一用 $\operatorname{Tr}(Q/H)$ 表示正实数，无论是否有限，定义如下：

a) 如果存在$x \in E$使得$H(x) = 0$和$Q(x) \neq 0$，则有一个集合$\operatorname{Tr}(Q/H) = +\infty$。

b) In the contrary case, $\operatorname{Tr}(Q/H)$ is the supremum of the set of numbers of the form $\sum_{i=1}^p Q(e_i)$, where $(e_1, \ldots, e_p)$ runs over the set of finite sequences of elements of $E$ orthonormal for $H$.

令$E$为实希尔伯特空间，$Q$为$E$上的正二次方形式。 集合 $H(x) = \|x\|^2$ 对于所有 $x \in E$；那么$H$是$E$上的正二次方形式。如果 $\operatorname{Tr}(Q/H)$ 是有限的，则可以说 $Q$ 是*核*。对于范数 1 中的每一个 $x \in E$，有 $Q(x) \leq \operatorname{Tr}(Q/H)$、从而 $Q \leq \operatorname{Tr}(Q/H) \cdot H$；特别是，每个核形式$Q$都是连续的。

#### 注 {#int-ix-a0-n1-rem-1 .statement tag=09T5}

— 1) 对于$E$的每个子空间$F$，用$Q$至$F$的$Q_F$限制表示，并用$H_F$表示$H$。那么$\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$和$\operatorname{Tr}(Q/H)$就是$F \subset E$有限维的数$\operatorname{Tr}(Q_F/H_F)$的上界。

2) 令$E_1$为实向量空间、$Q_1$和$H_1$在$E_1$上的两个正二次形式，以及$\pi : E \to E_1$为满射线性映射。如果$Q = Q_1 \circ \pi$和$H = H_1 \circ \pi$，则$\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$。

(1) 参见。 TVS，V, §4, No. 9。

#### 命题 1 {#int-ix-a0-prop-1 .statement tag=09T6}

— *假设 E 是有限维的，H 是非简并的。*

a) *E 中存在自同态 u，其特征在于* $(x|y)_Q = (u(x)|y)_H$ *对于 E* 中的 x、y。

b) $\operatorname{Tr}(Q/H) = \operatorname{Tr}(u)$。

c) $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$ *对于 H* 的 E 正交的每个基* $(e_1, \ldots, e_m)$ *。

*a)* 从以下事实得出：双线性形式 $(x, y) \mapsto (x|y)_H$ 是非简并的。 H 的 E 正交中的每个序列都可以补全为 H 的 E 正交的基。因而，$\operatorname{Tr}(Q/H)$ 是形式 $\sum_{i=1}^m Q(e_i)$ 的数的集合在所有 E 正交的基 $(e_1, \ldots, e_m)$ 上的上界H. 为了证明 *b)* 和 *c)*，只需证明对于此类的每个基都有 $\sum_{i=1}^m Q(e_i) = \operatorname{Tr}(u)$。 集合 $a_{ij} = (u(e_i)|e_j)_H = (e_i|e_j)_Q$ $1 \leq i, j \leq m$；然后$u(e_i) = \sum_{j=1}^m a_{ij} e_j$换$1 \leq i \leq m$，从而

$$
\operatorname{Tr}(u) = \sum_{i=1}^m a_{ii} = \sum_{i=1}^m (e_i|e_i)_Q = \sum_{i=1}^m Q(e_i).
$$

Q.E.D.

#### 命题 2 {#int-ix-a0-prop-2 .statement tag=09T7}

— *假设 E 是有限维的。存在基* $(e_1, \ldots, e_n)$ *E 和整数 m 且* $0 \leq m \leq n$ *这样*

$$
\operatorname{H}\left( \sum_{i=1}^n t_i e_i \right) = \sum_{i=1}^m t_i^2
$$

*对于*$t_1, \ldots, t_n$*真实。此外，如果关系* $\operatorname{H}(x) = 0$ *意味着* $Q(x) = 0$ *对于* $x \in E$，*则* $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$。

存在与 H 正交的 E 的基 $(e'_1, \ldots, e'_n)$。可以假设基的索引方式为 $1 \leq i \leq m$ 为 $\operatorname{H}(e'_i) > 0$，$\operatorname{H}(e'_i) = 0$ 为 $m < i \leq n$。然后集合$e_i = e'_i / \operatorname{H}(e'_i)^{1/2}$代表$1 \leq i \leq m$，$e_i = e'_i$代表$m < i \leq n$； 关系 (1) 满足。

令F为$e'_{m+1}, \ldots, e'_n$生成的E的子空间；它是$x \in E$的集合使得$\operatorname{H}(x) = 0$。用E的$\pi$典范映射到$E_1 = E/F$表示。由于Q和H在F上零，因此在$E_1$上存在两个正二次形式、$Q_1$和$H_1$，使得$Q = Q_1 \circ \pi$和$H = H_1 \circ \pi$。此外，$(\pi(e_1), \ldots, \pi(e_m))$ 是$H_1$ 的$E_1$ 正交的基，因而$H_1$ 是非简并的。

根据提案 1 和 *注 2*，

$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1) = \sum_{i=1}^m Q_1(\pi(e_i)) = \sum_{i=1}^m Q(e_i).
$$

Q.E.D.

#### 注 3 {#int-ix-a0-n1-rem-3 .statement tag=09T8}

— 假设 E 有限维且 H 非简并。令$(e_1, \ldots, e_n)$为E的基。集合$q = ((e_i|e_j)_Q)_{1 \leq i,j \leq n}$和$h = ((e_i|e_j)_H)_{1 \leq i,j \leq n}$。根据命题1中的记号，E的基$(e_1, \ldots, e_n)$的$u$的矩阵等于$h^{-1}q$、从而

(2)
$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(h^{-1}q) = \operatorname{Tr}(qh^{-1}).
$$

### 2. 希尔伯特-施密特映射$^{(2)}$

令 E 为实希尔伯特空间，其中标量乘积表示为 $(x|y)$。 E 在其对偶上存在等距 $j_E$，其特征为公式

(3)
$$
(x|y) = \langle x, j_E(y) \rangle \quad \text{for } x, y \text{ in E}
$$
（TVS，V, §1, No. 7，Th.3）。

令$E_1$和$E_2$是两个实希尔伯特空间和$u$，$E_1$到$E_2$的连续线性映射。我们将$E_2$的连续线性映射$u^* = j_{E_1}^{-1} \circ {}^t u \circ j_{E_2}$称为$E_1$的*伴随。 映射 $u^*$ 的特点是关系

(4)
$$
(u(x_1)|x_2) = (x_1|u^*(x_2)) \quad \text{for } x_1 \in E_1,\ x_2 \in E_2.
$$

如果 $v$ 是 $E_2$ 的连续线性映射到希尔伯特空间 $E_3$，则有 $(v \circ u)^* = u^* \circ v^*$。

令$E_1$和$E_2$是$E_1$到$E_2$的两个实希尔伯特空间和$u$线性映射。一个定义两个正二次形式 H 和 Q 在 $E_1$ 乘公式

$$
H(x) = \|x\|^2,\quad Q(x) = \|u(x)\|^2 \quad (x \in E_1).
$$

#### 命题 3 {#int-ix-a0-prop-3 .statement tag=09T9}

*假设u是连续的。令 $(e_i)_{i \in I}$ 为 $E_1$ 的正交基，并且 $(f_j)_{j \in J}$ 为 $E_2$ 的正交基。然后*

$$
\operatorname{Tr}(Q|H) = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2.
$$

(2) 参见。 TVS，V, §4, No. 7。

对于每个$x \in E_1$，我们有$\|x\|^2 = \sum_{i \in I} (x|e_i)^2$，同样，对于每个$y \in E_2$，我们有$\|y\|^2 = \sum_{j \in J} (y|f_j)^2$。因而，

$$
\sum_{i \in I} \|u(e_i)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2 \\
= \sum_{j \in J} \sum_{i \in I} (e_i|u^*(f_j))^2 \\
= \sum_{j \in J} \|u^*(f_j)\|^2 .
$$

特别是，数$\sum_{i \in I} \|u(e_i)\|^2$独立于$E_1$的正交基$(e_i)_{i \in I}$。

集合$t = \operatorname{Tr}(Q|H)$。对于 $I$ 中的每有限子集 $I'$，按定义

$$
\sum_{i \in I'} \|u(e_i)\|^2 = \sum_{i \in I'} Q(e_i) \leq t ,
$$

从而$\sum_{i \in I} \|u(e_i)\|^2 \leq t$。令 $(e'_1, \ldots, e'_p)$ 为 $E$ 中的有限正交序列。这个序列可以完成为$E_1$的正交基$(e'_\alpha)_{\alpha \in A}$。然后

$$
\sum_{\alpha=1}^p \|u(e'_\alpha)\|^2 \leq \sum_{\alpha \in A} \|u(e'_\alpha)\|^2 = \sum_{i \in I} \|u(e_i)\|^2
$$

并且，经过对所有$(e'_1, \ldots, e'_p)$的最高，得到不等式$t \leq \sum_{i \in I} \|u(e_i)\|^2$。我们就这样建立了等式$t = \sum_{i \in I} \|u(e_i)\|^2$。

Q.E.D.

有人说，如果$E_1$上的正二次方形式$Q : x \mapsto \|u(x)\|^2$是核的话，$u$是$E_1$到$E_2$的*希尔伯特-施密特映射*。当这种情况发生时，就有 $Q \leq \operatorname{Tr}(Q/H) \cdot H$，因而 $u$ 是连续的并且

$$
\|u\| \leq \operatorname{Tr}(Q/H)^{1/2} .
$$

设$u : E_1 \to E_2$为连续的线性映射。根据命题 3，当且仅当存在 $E_1$ 的正交基 $(e_i)_{i \in I}$ 使得 $\sum_{i \in I} \|u(e_i)\|^2 < +\infty$ 时，$u$ 是希尔伯特-施密特映射。在这种情况下，$E_1$ 的每个正交基都具有相同的性质。此外，如果$u$是希尔伯特-施密特映射，那么根据公式$\sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2$（命题3），它的伴随$u^*$也是希尔伯特-施密特映射。

习题

### 习题 {#int-ix-a0-exercises}

参见[习题附录 0](exercises/a0/)。
