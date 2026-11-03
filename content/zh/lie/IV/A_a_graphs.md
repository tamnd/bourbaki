---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 0
section_title: Graphs
appendix: true
lang: zh
source: lie-iv-vi
pdf_pages: 0040-0043
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS
      page: 0
      pdf_page: 40
    - "no": 2
      title: CONNECTED COMPONENTS OF A GRAPH
      page: 0
      pdf_page: 40
    - "no": 3
      title: FORESTS AND TREES
      page: 0
      pdf_page: 42
statements: 6
exercises: 0
content_sha256: 3b613c23d447e697e8e84b18b5db691b571ddd8269a6702e6b074abbd3ef7e75
translated_from: content/en/lie/IV/A_a_graphs.md
translation_method: google
source_content_sha256: 7fa7ab5ecf248630c43ab97ab1126594432fdccc1695b2f5d4ac5a3b570217ea
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: a61207713c0a47045ebb90603d4b7d46da8b9898e6ae0fe25bc20f420fda92cd
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 附录
# 图表

### 1. 定义

#### 定义 1 {#lie-iv-a0-def-1 .statement tag=0AOV}

*组合图（或简单的图，如果没有混淆的风险）是对* $(\mathbf{A}, S)$，*其中S是集合，A是$\mathfrak{P}(S)$的子集，集合的由……组成和两个元素。*

设 $\Gamma = (\mathbf{A}, S)$ 为图。 $\mathbf{A}$的元素称为*边*，S的$\Gamma$的*顶点*；如果 $\{x, y\}$ 是一条边，则两个顶点被称为“连接”。如果一个顶点最多连接到一个顶点，则该顶点称为*终端*；如果它连接到至少三个顶点，则称为*分支点*。

根据一般的定义（*集合R*，§8），从图$\Gamma$到图$\Gamma' = (\mathbf{A}', S')$的*同构*是从S到S'的双射，需要$\mathbf{A}$到$\mathbf{A}'$。如果 $S' \subset S$ 和 $\mathbf{A}' \subset \mathbf{A}$，则图 $\Gamma' = (\mathbf{A}', S')$ 被称为 $\Gamma$ 的*子图*；如果$S' \subset S$和$\mathbf{A}' = \mathbf{A} \cap \mathfrak{P}(S)$，$\Gamma$被称为$\Gamma$的*完整子图*。很明显，S 的每个子集恰好是 $\Gamma$ 的一个完整子图的顶点集合。

为了使论证更容易理解，我们用图表表示一个图，其中顶点有点相应的，当且仅当它们表示的顶点在图中连接时，两个点通过一条线连接起来。例如，图表

![具有顶点 a, b, c, d, e 和边 {a, b}, {b, c}, {c, d}, {c, e} 的图的图表](https://i.imgur.com/3Q5z5QG.png)

表示一个图，其顶点为 $a, b, c, d, e$，边为 $\{a, b\}, \{b, c\}, \{c, d\}$ 和 $\{c, e\}$。

### 2. 图的连通分量

设 $\Gamma = (\mathbf{A}, S)$ 为图。如果$a$和$b$是两个顶点，则连接$a$和$b$的*路径*是$\Gamma$和$x_0 = a, x_n = b$的顶点的序列$(x_0, \ldots, x_n)$，顶点$x_i$和$x_{i+1}$被连接为$0 \leq i < n$； 整数 $n \geq 0$ 是路径的 *长度*。如果 $x_i \neq x_j$ if $i \neq j$，则称路径 $(x_0, \ldots, x_n)$ 是单射的。如果连接$a$和$b$的路径$(x_0, \ldots, x_n)$在这些路径中具有最小的长度，则它必然是单射的；因为如果没有，就会存在$i$和$j$以及$0 \leq i < j \leq n$和$x_i = x_j$，然后是序列

$$
(x_0, \ldots, x_i, x_{j+1}, \ldots, x_n)
$$

将是连接$a$和$b$的长度$< n$路径。

关系“在$\Gamma$的两个顶点$a$和$b$之间存在连接$a$和$b$的路径”，在集合$S$上有等价关系$R$。 $R$的等价类称为$\Gamma$的*相连的分量*；如果$S$至多有一个连接的分量，即$\Gamma$的任意两个顶点可以通过至少一条路径连接，则$\Gamma$被称为*连接*。

#### 命题 1 {#lie-iv-a0-prop-1 .statement tag=0AOW}

*令 $\Gamma = (A, S)$ 为图，$(S_\alpha)_{\alpha \in L}$ 为其连通的分量族。用 $\Gamma_\alpha$ 表示 $\Gamma$ 的完整子图，其中 $S_\alpha$ 作为其集合顶点。*

(i) *对于$L$中的任何$\alpha$，图$\Gamma_\alpha$是连通的。*
(ii) *如果$\Gamma' = (A', S')$是$\Gamma$的连通子图，则$L$中存在$\alpha$，使得$\Gamma' \subset \Gamma_\alpha$。*
(iii) *如果$\alpha \neq \beta$，则$S_\alpha$中的任何元素都不会在$\Gamma$中与$S_\beta$中的任何元素相连接（等效地，$\Gamma$的每条边都是$\Gamma_\alpha$之一的边）。*
(iv) *令$(S'_\lambda)_{\lambda \in M}$为$S$的划分，这样，如果$\lambda \neq \mu$，$S'_\lambda$中没有元素加入到$\Gamma$与$S'_\mu$中的任何元素；那么每个集合$S'_\lambda$都是$\Gamma$相连的分量的并。*

(i) 设$\alpha$在$L$中，并且$a$和$b$在$S_\alpha$中。那么$\Gamma$中存在一条连接$a$和$b$的路径$c = (x_0, \ldots, x_n)$。对于任何带有$0 \leq i \leq n$的$i$，路径$(x_0, \ldots, x_i)$在$\Gamma$中将$a$连接到$x_i$，因此$x_i \in S_\alpha$。因此，$c$是$\Gamma_\alpha$*中*连接$a$和$b$的路径。由此可知$\Gamma_\alpha$是连通的。

(ii) 令$\Gamma' = (A', S')$为$\Gamma$的非空连通子图，令$a$为$S'$的元素，令$S_\alpha$为$S$包含$a$的连通分量。对于$S'$中的任何$b$，存在连接$\Gamma'$中的$a$和$b$的路径$c$，以及$\Gamma$中的*更不必说*。由此可知$S' \subset S_\alpha$。

(iii) 给定$L$的不同元素、$\alpha$和$\beta$，以及顶点$a \in S_\alpha$和$b \in S_\beta$，没有连接$a$和$b$的路径，特别是没有连接$a$和$b$的边。

(iv) 设$a$在$S'_\lambda$中，并令$S_\alpha$为$\Gamma$包含$a$的连通分量。那么，对于$S_\alpha$中的任何$b$，都存在一条连接$\Gamma$中的$a$和$b$的路径$(x_0, \ldots, x_n)$。如果$i$是整数，使得$0 \leq i < n$并且如果$x_i \in S'_\lambda$，则从$x_i$开始将$x_{i+1} \in S'_\lambda$连接到$x_{i+1}$。接下来是归纳，$x_i \in S'_\lambda$代表$0 \leq i \leq n$，特别是$b = x_n$在$S'_\lambda$中。因此，$S_\alpha \subset S'_\lambda$。

#### 推论 1 {#lie-iv-a0-prop-1-cor-1 .statement tag=0AOX}

*图$\Gamma = (A, S)$连接当且仅当不存在$S$的划分$(S', S'')$连接成两个非空子集，使得$S'$的元素不会在$\Gamma$中连接到$S''$的任何元素。*

假设$\Gamma$未连接，并令$S'$为其连接的分量之一。根据命题 1 (i)，集合 $S'' = S - S'$ 是非空的，并且根据命题 1 (iii)，$S'$ 中的任何元素都不会与 $S''$ 中的任何元素连接。

现在假设 $\Gamma$ 连通，并令 $(S', S'')$ 为划分与指定的性质。根据命题1（iv），集合$S'$包含至少有一个分量相连，因此$S' = S$和$S'' = \varnothing$矛盾。

#### 推论 2 {#lie-iv-a0-prop-1-cor-2 .statement tag=0AOY}

*当且仅当没有顶点属于到$S'$连接到任何顶点属于到$S - S'$时，$S$的子集$S'$是连接的分量的并。*

根据命题 1 (iv)，条件是充分的。根据提案 1 (iii)，这是必要的。

### 3. 森林和树木

让 $\Gamma = (A, S)$ 成为一个图。 $\Gamma$的*电路*是序列

$$
(x_1, \ldots, x_n)
$$

$\Gamma$ 的不同顶点，使得 $n \geq 3$、$x_i$ 连接到 $x_{i+1}$ 以获得 $1 \leq i < n$，并且 $x_n$ 连接到 $x_1$。如果$\Gamma$没有电路，则$\Gamma$称为*森林*；那么$\Gamma$的每个子图也是一片森林。连接的森林称为“树”；因此，森林的相连分量就是树木。

#### 命题 2 {#lie-iv-a0-prop-2 .statement tag=0AOZ}

*令 $\Gamma = (A, S)$ 为仅具有有限数顶点的森林。*

(i) *如果 $\Gamma$ 至少有一个顶点，则它有一个终端顶点。*
(ii) *如果$\Gamma$至少有两个顶点，则其集合顶点中有划分$(S', S'')$分成两个非空子集，使得两个不同的顶点属于都$S'$或属于都属于 $S''$ 从未加入。*

假设$\Gamma$至少有一个顶点，并令$(x_0, \ldots, x_n)$为$\Gamma$中最大长度的单射路径。顶点$x_0$不能连接到与$x_0, x_1, \ldots, x_n$不同的顶点$y$，否则$\Gamma$中将存在长度$n + 1$的单射路径，即$(y, x_0, \ldots, x_n)$。顶点 $x_0$ 不与任何带有 $2 \leq i \leq n$ 的顶点 $x_i$ 连接，否则 $(x_0, x_1, \ldots, x_i)$ 将成为森林 $\Gamma$ 中的环路。因此，$x_0$是终结符。

我们将通过$\Gamma$顶点的数$m$的归纳来证明（ii），情况$m = 2$是平凡的。假设对于具有 $m - 1$ 顶点的图证明了 $m \geq 3$ 和断言 (ii)。令 $a$ 为$\Gamma$ (cf. (i)) 的终端顶点。我们将归纳假设应用于$\Gamma$的完整子图，其顶点是$\Gamma$的顶点$x \neq a$。因此，$S$与$S'_1 \cup S''_1 = S - \{a\}$存在两个非空不相交的子集$S'_1$和$S''_1$，并且$S'_1$（或$S''_1$）中的两个不同顶点永远不会连接。由于$a$最多连接到$\Gamma$的一个顶点，因此我们可以假设它没有连接到$S'_1$中的任何顶点。 划分 $(S'_1, S''_1 \cup \{a\})$ 则具有所需的性质。 Q.E.D.

对于任意整数 $n \geq 1$，用 $A_n$ 表示顶点为整数 $1, 2, \ldots, n$、边为对 $\{i, j\}$ 和 $i - j = \pm 1$ 的图：

$$
\begin{array}{cccccc}
1 & 2 & 3 & n-1 & n \\
\circ & \circ & \circ & \cdots & \circ
\end{array}
$$

如果图$\Gamma$与$A_{m+1}$同构的，则称其为长度$m \geq 0$的链。这相当于$\Gamma$中存在单射路径$(x_0, \ldots, x_m)$包含所有顶点，如果$|i - j| > 1$则顶点$x_i$和$x_j$不被连接。

#### 命题 3 {#lie-iv-a0-prop-3 .statement tag=0AP0}

*图是一个链当且仅当它的顶点数是有限且非零的并且它是一个没有分支点的树。*

假设图$\Gamma$是一个链$(x_0, \ldots, x_m)$，具有命题3中列出的属性之前叙述。显然，$\Gamma$的任何顶点最多连接到两个顶点。如果从路径$(x_0, \ldots, x_m)$提取的$i < j$路径$(x_i, \ldots, x_j)$将$x_i$连接到$x_j$；因此，$\Gamma$是相连的。最后，令$(x_{p_1}, \ldots, x_{p_n})$为$\Gamma$中的电路，并令$p_k$为不同整数$p_1, \ldots, p_n$的最小的。存在不同的指标、$i$和$j$，使得$x_{p_k}$连接到$x_{p_i}$和$x_{p_j}$：这是从电路的定义得出的。由于$p_k < p_i$和$p_k < p_j$，我们必然有$p_i = p_j = p_k + 1$，这是一个矛盾，因为$p_1, \ldots, p_n$是不同的。因此，$\Gamma$中没有电路。

相反，令$\Gamma$为一棵没有分支点且具有有限非零数顶点的树，并令$(x_0, \ldots, x_m)$为$\Gamma$中最大长度的单射路径。 $x_0, \ldots, x_m$以外的顶点用$T$集合表示。顶点 $b \in T$ 不能连接到任何顶点 $x_i$，因为我们可以有

a) $i = 0$，但是$(b, x_0, \ldots, x_m)$将是$\Gamma$中长度$m + 1$的单射路径，或者
b) $i = m$，但是$(x_0, \ldots, x_m, b)$将是$\Gamma$中长度$m + 1$的单射路径，或者
c) $0 < i < m$，但是$x_i$将连接到三个不同的顶点$x_{i-1}$、$x_{i+1}$和$b$。

由于 $\Gamma$ 已连通，因此 $T$ 被 Cor 为空。命题1的1.此外，如果有$i, j$与$j - i > 1$和$x_i, x_j$连接，则$\Gamma$中将存在$(x_i, x_{i+1}, \ldots, x_j)$电路。因此，$\Gamma$是一条链。 Q.E.D.
