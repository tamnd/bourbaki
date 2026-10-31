---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 7
section_title: Free monoids, free groups
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 81-96, 159-171
pdf_pages: 0105-0120, 0183-0195
extraction: ocr
subsections:
    - "no": 1
      title: FREE MAGMAS
      page: 81
      pdf_page: 105
    - "no": 2
      title: FREE MONOIDS
      page: 82
      pdf_page: 106
    - "no": 3
      title: AMALGAMATED SUM OF MONOIDS
      page: 84
      pdf_page: 108
    - "no": 4
      title: APPLICATION TO FREE MONOIDS
      page: 88
      pdf_page: 112
    - "no": 5
      title: FREE GROUPS
      page: 89
      pdf_page: 113
    - "no": 6
      title: PRESENTATIONS OF A GROUP
      page: 90
      pdf_page: 114
    - "no": 7
      title: FREE COMMUTATIVE GROUPS AND MONOIDS
      page: 92
      pdf_page: 116
    - "no": 8
      title: EXPONENTIAL NOTATION
      page: 94
      pdf_page: 118
    - "no": 9
      title: RELATIONS BETWEEN THE VARIOUS FREE OBJECTS
      page: 95
      pdf_page: 119
statements: 17
exercises: 40
content_sha256: 14efdf630fd5e8ae1c1644fc07bc6ea776e066f11094bd522384e69265777bab
translated_from: content/en/alg/I/07_s7_free_monoids_free_groups.md
translation_method: google
source_content_sha256: 97dfa3c35501eb8d7f97ddf5171fd22adaac2703346a99cfb362c9406ce8d816
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a73e50d8eb9efb5abfb41c6d9ec05c6673db61411dd6988dffabe88cea87e917
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 7。免费幺半群，免费群

在本段中，X将表示集合。另外，除非，幺半群的单位元素将用e表示。

### 1. 免费岩浆

集合 $M_n(X)$的序列由整数$n \geqslant 1$上的归纳定义如下：写成$M_1(X) = X$，对于$n \geqslant 2$，$M_n(X)$就是集合的集合和 $M_p(X) \times M_{n-p}(X)$ 换$1 \leqslant p \leqslant n-1$。 $(M_n(X))_{n \geqslant 1}$家族的集合和用$M(X)$表示；每个集合$M_n(X)$都用$M(X)$中的典范像来标识。对于$M(X)$的每个元素$w$，都存在一个唯一的整数$n$，使得$w \in M_n(X)$；它被称为$w$的长度，并用$l(w)$表示。 集合 X 由长度 1 的 $M(X)$ 中的元素组成。

设$w$和$w'$在$M(X)$内；写出$p = l(w)$和$q = l(w')$。 $M_p(X) \times M_q(X)$的典范嵌入下的$(w, w')$的像变成和集合$M_{p+q}(X)$称为$w$和$w'$的合成并记为$ww'$或$w.w'$。那么$l(w.w') = l(w) + l(w')$和长度$\geqslant 2$的$M(X)$的每个元素可以唯一地写在形式$w'w''$和$w', w''$在$M(X)$中。

集合$M(X)$与律为合成$(w, w') \mapsto w.w'$称为X（§ 1, no. 1，定义1）上构造的自由岩浆。

#### 命题 1 {#alg-i-s7-prop-1 .statement tag=05FH}

设M为岩浆。 X 的每个映射 f 都可以以独特的方式扩展到 M 中的 $M(X)$ 态射。

由$n \geqslant$上的归纳，映射$f_n : M_n(X) \to M$定义如下：对于 n \geq 2，映射 f_n 由 $p = 1, 2, \ldots, n-1$ 的 $f_n(w.w') = f_p(w).f_{n-p}(w')$ 和 $M_p(X) \times M_{n-p}(X)$ 中的 $(w, w')$ 定义。让$g$是$M(X)$的映射进入$M$，其中对于每个整数$n \geq 1$，诱导$f_n$在$M_n(X)$上。显然，$g$ 是$M(X)$ 的唯一态射到$M$，其中扩展 $f$。

设$u$为$X$的映射到集合$Y$。到命题 1，$M(X)$ 到$M(Y)$ 中存在且仅有一个同态，其中重合和$X$ 上的$u$。它将用$M(u)$表示。如果$v$是$Y$的映射变成集合$Z$，$M(X)$的同态$M(v) \circ M(u)$变成$M(Z)$重合，$v \circ u$在$X$， 从而

$$
M(v) \circ M(u) = M(v \circ u).
$$

#### 命题 2 {#alg-i-s7-prop-2 .statement tag=05FI}

*令$u : X \to Y$为映射。如果 $u$ 是单射（分别是满射、双射），则 $M(u)$ 也是。*

假设 $u$ 是单射的。当 $X$ 为空时，$M(X)$ 为空，因此 $M(u)$ 是单射的。如果$X$非空，$X$中存在$Y$的映射$v$，使得$v \circ u$是$X$的恒等映射（*集合理论*，II, § 3, no. 8， 命题8); 映射 $M(v) \circ M(u) = M(v \circ u)$ 是 $M(X)$ 的恒等映射，因此 $M(u)$ 是单射的。

当$u$是满射时，$X$中存在$Y$的映射$w$，使得$u \circ w$是$Y$的恒等映射（*集合理论*，II, § 3, no. 8， 命题8)。那么 $M(u) \circ M(w) = M(u \circ w)$ 是 $M(Y)$ 的恒等映射，因此 $M(u)$ 是满射。

最后，如果 $u$ 是双射的，那么它是单射和满射的，因此 $M(u)$ 具有相同的性质。

令 $S$ 为 $X$ 中的子集。通过 $S$ 的命题 2 单射进入$X$，可以扩展到$M(S)$ 的同构到$M(X)$ 的子岩浆$M'(S)$。岩浆$M(S)$和$M'(S)$是通过这个同构来识别的。那么$M(S)$就是$S$生成的$M(X)$的次岩浆。

设$X$为集合，$(u_\alpha, v_\alpha)_{\alpha \in I}$为$M(X)$的元素的有序对的族。令$R$为$M(X)$上的等价关系，与$M(X)$的律兼容，并由$(u_\alpha, v_\alpha)$（§ 1, no. 6）生成。岩浆$M(X)/R$称为*由$X$和相关子*$(u_\alpha, v_\alpha)_{\alpha \in I}$定义的岩浆。令$h$为$M(X)$到$M(X)/R$的规范态射。然后$M(X)/R$由$h(X)$生成。

令$N$为岩浆，$(n_x)_{x \in X}$为元素和$N$的族。令 $k$ 为从 $M(X)$ 到 $N$ 的态射，使得 $k(x) = n_x$ 对于所有 $x \in X$ (命题 1)。如果$k(u_\alpha) = k(v_\alpha)$对于所有$\alpha \in I$，则存在且仅一个态射$f : M(X)/R \to N$，使得$f(h(x)) = n_x$对于所有$x \in X$（§ 1, no. 6，命题9）。

### 2.免费幺半群

由 $\mathbf{N}$ 的区间 $[1, n]$（可能为空）索引的 $X$ 的元素的任何有限序列 $w = (x_i)_{1 \leq i \leq n}$ 称为在 $X$ 上构造的 *字*。 整数$n$称为字$w$的*长度*，记为$l(w)$。 长度 0 存在一个唯一的字，即空的序列$e$。 $\mathbf{X}$ 将被识别为集合 of 字 of 长度 1。

令$w = (x_i)_{1 \leq i \leq m}$和$w' = (x'_j)_{1 \leq j \leq n}$为两个字。 $w$ 和 $w'$ 的合成是字 $u = (y_k)_{1 \leq k \leq m+n}$ 定义为

$$
y_k = \begin{cases}
x_k & \text{for } 1 \leq k \leq m \\
x'_{k-m} & \text{for } m+1 \leq k \leq m+n.
\end{cases}
$$

在其他字中，序列$w''$是通过先写序列$w$的元素，然后写$w'$的元素得到。 $w$和$w'$中的合成一般用$ww'$或$w.w'$表示； 有时说是由$w$和$w'$并列得到。然后构造$l(w.w') = l(w) + l(w')$。

对于每个字$w$立即建立关系$we = ew = w$。令$w = (x_i)_{1 \leq i \leq m}$、$w' = (x'_j)_{1 \leq j \leq n}$和$w'' = (x''_k)_{1 \leq k \leq p}$为三个字；显然字 $w(w'w'')$ 和 $(ww')w''$ 都等于字 $(y_l)_{1 \leq l \leq m+n+p}$ 定义为

$$
y_l = \begin{cases}
x_l & \text{if } 1 \leq l \leq m \\
x_{l-m} & \text{if } m+1 \leq l \leq m+n \\
x''_{l-m-n} & \text{if } m+n+1 \leq l \leq m+n+p.
\end{cases}
$$

上式表明，在 $\mathbf{X}$ 和合成 $(w, w') \mapsto w.w'$ 的律上构造的字集合是一个具有单位元素 $e$ 的幺半群。它用$\mathrm{Mo}(\mathbf{X})$表示，并称为*在*$\mathbf{X}$上构建的自由幺半群。紧接着从定义、乘积、字得出，每个字$w = (x_i)_{1 \leq i \leq n}$等于乘积$\prod_{i=1}^n x_i$。因此字可以写成形式$x_1 \ldots x_n$。

#### 命题 3 {#alg-i-s7-prop-3 .statement tag=05FJ}

*设 M 为幺半群。 X 的每个映射 f 转换为 M 扩展唯一到 Mo(X) 的同态转换为 M。*

设$g$是$\mathrm{Mo}(\mathbf{X})$的同态延伸到$M$延伸$f$。如果$w = (x_i)_{1 \leq i \leq n}$是字，那么$w = \prod_{i=1}^n x_i$在幺半群$\mathrm{Mo}(\mathbf{X})$、从而中

$$
g(w) = \prod_{i=1}^n g(x_i) = \prod_{i=1}^n f(x_i)
$$

在幺半群 $M$ (§ 1, no. 2, 公式 (2)) 中。这就证明了$g$的唯一性。

让$h(w) = \prod_{i=1}^n f(x_i)$对应于每个字$w = (x_i)_{1 \leq i \leq n}$。 $\mathrm{Mo}(\mathbf{X})$中乘积的结合性定理（§ 1, no. 3，定理1）和定义意味着$h(ww') = h(w)h(w')$。按照惯例，空的乘积$h(e)$是$M$的单位元素，$h(x) = f(x)$是$x \in \mathbf{X}$。因此，$h$是$\mathrm{Mo}(x)$的同态延伸到$M$延伸$f$。

令$u : \mathbf{X} \to \mathbf{Y}$为映射。到命题 3 时，Mo(Y) 中存在且仅有一个同态的 Mo(X)，其中重合且 u 在X；用Mo(u)表示。它映射字$(x_i)_{1 \leq i \leq n}$到字$(u(x_i))_{1 \leq i \leq n}$。与岩浆 (no. 1) 的情况一样，对于每个映射 $v : Y \to Z$，方程 Mo(v \circ u) = Mo(v) \circ Mo(u) 成立，并且可以证明，如果 u 是，则 Mo(u) 是单射的（分别是满射、双射的）。对于X的每个子集 S，Mo(S) 可以用 S 生成的 Mo(X) 的子幺半群来标识。

设X为集合，$(u_\alpha, v_\alpha)_{\alpha \in I}$为Mo(X)的元素的有序对族。令 R 为 Mo(X) 上的等价关系，与 Mo(X) 上的律兼容，并由 $(u_\alpha, v_\alpha)$ (§ 1, no. 6) 生成。幺半群 Mo(X)/R 称为*由 X 和关系子* $(u_\alpha, v_\alpha)_{\alpha \in I}$ 定义的幺半群。令 h 为 Mo(X) 在 Mo(X)/R 上的规范态射。然后Mo(X)由h(X)生成。

令 N 为幺半群，$(n_x)_{x \in X}$ N 的元素族。令 k 为 N 中 Mo(X) 的态射，使得 $k(x) = n_x$ 对于所有 $x \in X$ (命题 3)。如果$k(u_\alpha) = k(v_\alpha)$对于所有$\alpha \in I$，则存在且仅存在一种岩浆态射$f : Mo(X)/R \to N$，使得$f(h(x)) = n_x$对于所有$x \in X$（§ 1, no. 6，命题9）；因为 k 是单位的，所以 f 是幺半群态射。

### 3. 粘合和幺半群

*令$(M_i)_{i \in I}$表示幺半群族，$e_i$单位元素表示$M_i$。我们得到一个幺半群 A 和一个同态$h_i : A \to M_i$（对于$i \in I$）。*

$(M_i)_{i \in I}$家族的集合S和有元素有序对$(i, x)$以及$i \in I$和$x \in M_i$。对于$M_i$中的每个三元组$\alpha = (i, x, x')$和$i \in I$、$x, x'$，写出$u_\alpha = (i, xx')$和$v_\alpha = (i, x).(i, x')$；对于$I \times I \times A$中的每个三元组$\lambda = (i, j, a)$，写出$p_\lambda = (i, h_i(a))$和$q_\lambda = (j, h_j(a))$；对于所有$i \in I$，写下$\varepsilon_i = (i, e_i)$。由 S 和关系子 $(u_\alpha, v_\alpha)$、$(p_\lambda, q_\lambda)$ 和 $(\varepsilon_i, e)$ 定义的幺半群 M 称为族* $(M_i)_{i \in I}$ *由* A 合并的 *和。令 $\phi$ 表示 Mo(S) 的典范同态到 M 上，并将 $\phi_i(x) = \phi(i, x)$ 写为$(i, x) \in S$。据说$\phi_i$是$M_i$到M的*典范映射*。对于所有$a \in A$，元素$\phi(i, h_i(a))$与i无关，记为$h(a)$。\footnote{当I为空时，$M = \{e\}$和$h(a) = e$ 所有人$a \in A$。}

由生成元和相关子 (no. 2) 定义的幺半群的泛性质意味着以下结果：

#### 命题 4 {#alg-i-s7-prop-4 .statement tag=05FK}

(a) *对于所有 $i \in I$，映射 $\phi_i$ 是 $M_i$ 的同态进入 M，对于所有 $i \in I$，$\phi_i \circ h_i = h$。进一步地，M由$\bigcup_{i \in I} \phi_i(M_i)$生成。*

(b) *令$M'$为幺半群，$f' : M_i \to M'$（对于$i \in I$）同态，使得$f_i \circ h_i$独立于$i \in I$。存在且仅有一个同态 $f : M \to M'$，使得 $f_i = f \circ \phi_i$ 对于所有 $i \in I$。*

接下来我们将进行以下假设：

(A) *对于所有$i \in I$，存在$M_i$包含$e_i$的子集$P_i$，使得$A \times P_i$到$M_i$的映射$(a, p) \mapsto h_i(a).p$是双射的。*

这意味着同态 $h_i$ 是单射的。让$x \in M$；每有限序列 $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$，其中 $a \in A, i_\alpha \in I$ 和 $p_\alpha \in P_{i_\alpha}$ 为 $1 \leq \alpha \leq n$、满足

$$
x = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha)
$$

称为 $x$ 的分解。 整数$n \geq 0$称为分解$\sigma$的长度，记为$l(\sigma)$； 序列$(e)$是$M$单位元素长度分解0。如果$i_\alpha \neq i_{\alpha+1}$代表$1 \leq \alpha < n$，$p_\alpha \neq e_{i_\alpha}$代表$1 \leq \alpha \leq n$，则分解$\sigma$被称为缩减。

#### 命题 5 {#alg-i-s7-prop-5 .statement tag=05FL}

在假设 (A) 下，$M$ 的每一个元素 $x$ 都承认一个唯一的缩减分解 $\sigma$。 $x$中的每分解$\sigma' \neq \sigma$满足$l(\sigma') > l(\sigma)$。

(A) 减少的分解的唯一性：

让$\Sigma$表示序列$\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$的集合，其中$n \geq 0$、$a \in A, i_\alpha \in I$和$p_\alpha \in P_{i_\alpha} - \{e_{i_\alpha}\}$代表$1 \leq \alpha \leq n$，这样$i_\alpha \neq i_{\alpha+1}$代表$1 \leq \alpha < n$。让 $\Phi$ 表示 $\Sigma$ 的映射到 $M$ 定义为

$$
\Phi(a; i_1, \ldots, i_n; p_1, \ldots, p_n) = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha).
$$

$x \in M$的减少分解是$\Sigma$的元素$\sigma$，这样$\Phi(\sigma) = x$。

对于所有$i \in I$，令$\Sigma_i$为序列$(e; i_1, \ldots, i_n; p_1, \ldots, p_n)$的$\Sigma$由……组成的子集，当$n > 0$时为$i \neq i_1$。让

$$
\sigma = (e; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$

位于$\Sigma_i$且$\xi$位于$M_i$；让 $\xi = h_i(a) \cdot p$ 与 $a \in A$ 和 $p \in P_i$，以及

$$
\Psi_i(\xi, \sigma) = \begin{cases}
(a; i_1, \ldots, i_n; p_1, \ldots, p_n) & \text{if } p = e_i \\
(a; i, i_1, \ldots, i_n; p, p_1, \ldots, p_n) & \text{if } p \neq e_i.
\end{cases}
$$

$\Psi_i$是$M_i \times \Sigma_i$的双射到$\Sigma$，就是直接的。

设$i \in I$和$x \in M_i$；由于 $\Psi_i$ 是双射，$\Sigma$ 的映射 $f_{i,x}$ 自身定义为

$$
f_{i,x}(\Psi_i(\xi, \sigma)) = \Psi_i(x\xi, \sigma) \quad (\xi \in M_i, \sigma \in \Sigma_i).
$$

此外，对于 $a \in A, f_a$ 表示 $\Sigma$ 的映射自身定义为

$$
f_a(a'; i_1, \ldots, i_n; p_1, \ldots, p_n) = (aa'; i_1, \ldots, i_n; p_1, \ldots, p_n).
$$

显然，$f_{i,e_i}$ 是$\Sigma$ 的恒等映射，$M_i$ 中$x, x'$ 是$f_{i,xx'} = f_{i,x} \circ f_{i,x'}$，$a \in A$ 和$i \in I$ 中$f_{i,h_i(a)} = f_a$。

那么命题 4 可以应用于以下情况：$M'$是$\Sigma$的映射的幺半群，律是合成$(f,f') \mapsto f \circ f'$，并且f_i是$M_i$的同态$x \mapsto f_{i,x}$ $M'$；那么$M$到$M'$存在同态$f$，使得$f_{i,x} = f(\phi_i(x))$对应于$i \in I$和$x \in M_i$。让
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
处于$\Sigma$。 公式 (5) 至 (7) 由 $n$ 关系上的归纳暗示
$$
\begin{align*}
\sigma &= (f_a \circ f_{i_1, p_1} \circ \cdots \circ f_{i_n, p_n})(e) \\
&= f(h(a)\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n))(e),
\end{align*}
$$
即$\sigma = f(\Phi(\sigma))(e)$。这证明$\Phi$是单射的。

(B) *分解*的存在：

令$D$为承认分解的$M$元素集合。然后$e \in D$和$M$由$\bigcup_{i \in I} \phi_i(M_i)$生成，因此由$h(A) \cup \bigcup_{i \in I} \phi_i(P_i)$生成。那么$D.\phi_i(P_i) \subset D$对于所有$i \in I$；要证明$D = M$，只需证明关系$D.h(A) \subset D$即可。这是从以下更精确的引理得出的：

#### 引理 1 {#alg-i-s7-lem-1 .statement tag=05FM}

*让$i_1, \ldots, i_n$在$I$中，而$p_\alpha$在$P_{i_\alpha}$中，则$1 \leq \alpha \leq n$。对于所有 $a \in A$ 都存在 $a' \in A$ 和序列 $(p'_\alpha)_{1 \leq \alpha \leq n}$ 以及 $p'_\alpha \in P_{i_\alpha}$ 这样*
$$
\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n)h(a) = h(a')\phi_{i_1}(p'_1) \ldots \phi_{i_n}(p'_n).
$$
$h(a) = \phi_{i_n}(h_{i_n}(a))$ 且存在 $a_n \in A$ 和 $p'_n \in P_{i_n}$ 且
$$
p_n \cdot h_{i_n}(a) = h_{i_n}(a_n) \cdot p'_n.
$$
由此可知 $\phi_{i_n}(p_n)h(a) = h(a_n)\phi_{i_n}(p'_n)$, 从而
$$
\phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})\phi_{i_n}(p_n)h(a) = \phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})h(a_n)\phi_{i_n}(p'_n);
$$
引理在此之后是$n$ 上的归纳。

(C) *证明结束*:

令$x \in M$且令$n$为$x$的分解中的长度中的最小值。我们将证明长度$n$的$x$中的每一个分解$\sigma$都会减少。这将确定分解减少为 $x$ 的存在；减少的分解的唯一性则意味着对于$x$的每个分解$\sigma' \neq \sigma$有$l(\sigma') > l(\sigma)$。

案例$n = 0$很简单，假设$n > 0$。让
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
为长度$n$$x$分解。如果存在整数$\alpha$与$1 \leq \alpha \leq n$和$p_\alpha = e_{i_\alpha}$，序列
$$
(a; i_1, \ldots, i_{\alpha-1}, i_{\alpha+1}, \ldots, i_n; p_1, \ldots, p_{\alpha-1}, p_{\alpha+1}, \ldots, p_n)
$$

将是分解 / $x$ / 长度 $n - 1$，已排除。假设存在整数 $\alpha$ 以及 $1 \leq \alpha < n$ 和 $i_{\alpha} = i_{\alpha + 1}$ 并让
$$
p_{\alpha} p_{\alpha + 1} = h_{i_{\alpha}}(a') \cdot p'_{\alpha}
$$
$a' \in \mathbf{A}$ 和 $p'_{\alpha} \in P_{i_{\alpha}}$；到引理 1 存在元素 $a'' \in \mathbf{A}$，
$$
p'_{1} \in P_{i_{1}}, \ldots, p'_{\alpha - 1} \in P_{i_{\alpha - 1}}
$$
这样
$$
\phi_{i_{1}}(p_{1}) \cdots \phi_{i_{\alpha - 1}}(p_{\alpha - 1}) h(a') = h(a'') \phi_{i_{1}}(p'_{1}) \cdots \phi_{i_{\alpha - 1}}(p'_{\alpha - 1})
$$
和序列
$$
(aa''; i_{1}, \ldots, i_{\alpha - 1}, i_{\alpha}, i_{\alpha + 2}, \ldots, i_{n}; p'_{1}, \ldots, p'_{\alpha - 1}, p'_{\alpha}, p_{\alpha + 2}, \ldots, p_{n})
$$
是长度$n - 1$的分解$x$，这是一个矛盾。

由此我们证明了$\sigma$被减少了。

#### 推论 {#alg-i-s7-n3-cor-1 .statement tag=05FN}

*在假设 (A) 下，同态 $\phi_{i}$ 和 $h$ 是单射的。对于 $I$、$\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) = h(\mathbf{A})$ 中的 $i \neq j$。*

首先$h$是单射的：如果$h(a) = h(a')$，则$(a)$和$(a')$是$M$、从而$a = a'$的相同元素的两个约化分解。让$i \in I$；然后$h(\mathbf{A}) = \phi_{i}(h_{i}(\mathbf{A})) \subset \phi_{i}(M_{i})$；减少分解的唯一性意味着
$$
h(\mathbf{A}) \cap \phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \varnothing,
$$
从而$\phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \phi_{i}(M_{i}) - h(\mathbf{A})$。

同态 $\phi_{i}$ 和关系的单射性
$$
\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) \subset h(\mathbf{A})
$$
对于$i \neq j$，则推论属于以下事实：对于$I$中的$i, j$、$M_{i} - h_{i}(\mathbf{A})$中的$x$和$M_{j} - h_{j}(\mathbf{A})$中的$y$，关系$\phi_{i}(x) = \phi_{j}(y)$意味着$i = j$并且$x = y$。让$x = h_{i}(a) \cdot p$和$y = h_{j}(b) \cdot q$与$\mathbf{A}$中的$a, b$，$P_{i} - \{e_{i}\}$中的$p$以及$P_{j} - \{e_{j}\}$中的$y$。那么$\phi_{i}(x) = h(a)\phi_{i}(p)$和$\phi_{j}(y) = h(b)\phi_{j}(q)$，因此$(a; i; p)$和$(b; j; q)$是$M$的相同元素的两个减少的分解。由此可见$i = j, a = b$和$p = q$、从而$x = h_{i}(a)p = h_{j}(b)q = y$。

当满足假设(A)时，我们可以通过$\phi_{i}$来认同每个幺半群$M_{i}$，其中子幺半群为$M$；同样，我们将认同$\mathbf{A}$与子幺半群乘以$M$乘以$h$。然后$M$由$\bigcup_{i \in I} M_{i}$和$M_{i} \cap M_{j} = \mathbf{A}$生成$i \neq j$。

$M$的每个元素都可以唯一地写成形式$a \prod_{\alpha = 1}^{n} p_{\alpha}$，其中$a \in \mathbf{A}, p_{1} \in P_{i_{1}} - \{e\}, \ldots, p_{n} \in P_{i_{n}} - \{e\}$和$i_{\alpha} \neq i_{\alpha + 1}$代表$1 \leq \alpha < n$。最后，如果$M'$是幺半群，并且$(f_{i}: M_{i} \to M')$（对于$i \in I$）同态的族，其限制到$\mathbf{A}$与$\mathbf{A}$到$M'$的同态相同，则存在一个且仅有一个同态$f: M \to M'$在$M_{i}$上为所有$i \in I$诱导$f_{i}$。

假设 (A) 在两个重要情况下得到满足：

（一）$A = \{e\}$。在这种情况下，有一个幺半群族$(M_i)_{i \in I}$，$M$称为该族的*幺半群和*。每个$M_i$由$M$的子幺半群标识，$M$由$\bigcup_{i \in I} M_i$生成；此外，$M_i \cap M_j = \{e\}$换成$i \neq j$。 $M$ 中的每个元素都可以唯一地写成形式 $x_1 \ldots x_n$
$$
x_1 \in M_{i_1} - \{e\}, \ldots, x_n \in M_{i_n} - \{e\}
$$
$i_\alpha \neq i_{\alpha+1}$ 代表 $1 \leq \alpha \leq n$。最后，对于同态$(f_i : M_i \to M')$的每个家庭，都存在唯一同态$f : M \to M'$，其限制到$M_i$对于所有$i \in I$来说都是$f_i$。

(b) 有一个群$(G_i)_{i \in I}$包含与子群相同的群$A$，$h_i$是$A$到$G_i$的单射。 $(G_i)_{i \in I}$族的和与$A$合并，则为*群*$G$：幺半群$G$由$\bigcup_{i \in I} \phi_i(G_i)$生成，$\bigcup_{i \in I} \phi_i(G_i)$的每个元素都承认有一个逆元$G$（cf.§ 2, no. 3，推论1至命题4）；当$I = \{1, 2\}$时，用$*_A G_i$或$G_1 *_A G_2$表示。当$A$由单位元素组成时，也可以说$G$是群的*家庭*乘积*$(G_i)_{i \in I}$，并用$* G_i$表示（如果$I = \{1, 2\}$则用$G_1 * G_2$）。†

### 4. 自由幺半群的应用

#### 引理 2 {#alg-i-s7-lem-2 .statement tag=05FO}

*令$M$为由$M_x = \mathbf{N}$定义的所有$x \in X$族$(M_x)_{x \in X}$的幺半群和，并令$\phi_x$表示$M_x$到$M$的典范同态。 映射 $x \mapsto \phi_x(1)$ $X$ 到 $M$ 扩展到同构 $h$ $\mathrm{Mo}(X)$ 到 $M$。*

令$h$为$\mathrm{Mo}(X)$的同态到以$h(x) = \phi_x(1)$为特征的$M$。 对于每个整数$n \geq 0$、$\phi_x(n) = \phi_x(1)^n = h(x)^n$，并且由于$M$是由$\bigcup_{x \in X} \phi_x(\mathbf{N})$生成的，因此它也是由$h(X)$生成的。 因此 $h$ 是*满射*。 此外，对于$X$中的所有$x$，映射$n \mapsto x^n$是$\mathbf{N} = M_x$的同态到$\mathrm{Mo}(X)$；因此，存在 (no. 3, 命题 4) 同态 $h'$，其中$M$进入$\mathrm{Mo}(X)$，使得$h'(\phi_x(n)) = x^n$对于$x \in X$和$n \in \mathbf{N}$；特别是，$h'(h(x)) = x$代表$x \in X$，因此$h' \circ h$是$\mathrm{Mo}(X)$的恒等式同态。 因此 $h$ 是*内射*。 由此证明$h$是双射的。

#### 命题 6 {#alg-i-s7-prop-6 .statement tag=05FP}

*设$w$为$\mathrm{Mo}(X)$的元素。
(a) 存在$X$和整数$m(\alpha) > 0$中的整数$n \geq 0$、元素$x_\alpha$（对于

† Note that $G_1 * G_2$ is not the "product" of $G_1$ and $G_2$ in the sense of *Set Theory*, IV, § 2, no. 4 (nor in the sense of the "theory of categories"; in the context of this theory, $G_1 * G_2$ is the "sum" of $G_1$ and $G_2$).

$1 \leq \alpha \leq n$使得$x_\alpha \neq x_{\alpha+1}$适用于$1 \leq \alpha < n$和$w = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$。 序列$(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$由这些条件唯一确定。

(b) 对于$1 \leq \beta \leq p$，令$p$为正整数、$X$中的$x'_\beta$以及$\mathbf{N}$中的$m'(\beta)$，使得$w = \prod_{\beta=1}^p {x'}^{m'(\beta)}$。然后$p \geq n$。如果$p = n$，则$x'_\beta = x_\beta$和$m'(\beta) = m(\beta)$为$1 \leq \beta \leq p$。

在引理 2 的记号中，$x \in X$ 和$n \in \mathbf{N}$ 为$h^{-1}(\phi_x(n)) = x^n$。然后从 no. 3、命题 5 得出命题 6。

### 5.免费群

让$G_x = \mathbf{Z}$代表所有$x \in X$。 $(G_x)_{x \in X}$族的自由乘积称为构建在*$X$上的*自由群，并用$F(X)$表示。让$\phi_x$表示$G_x = \mathbf{Z}$到$F(X)$的典范同态。由no. 3，推论命题 5，$X$到$F(X)$的映射$x \mapsto \phi_x(1)$是单射的；我们将认同$X$及其像放在$F(X)$下这个映射。然后是$X$生成$F(X)$和$e \notin X$。

应用no. 3，命题5，我们得到以下结果：

#### 命题 7 {#alg-i-s7-prop-7 .statement tag=05FQ}

*令 g 为免费群* $F(X)$ 中的元素。 *存在整数* $n \geq 0$ *和序列* $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ *由关系* $x_\alpha \in X$、$x_\alpha \neq x_{\alpha+1}$ *对于* $1 \leq \alpha < n$、$m(\alpha) \in \mathbf{Z}$、$m(\alpha) \neq 0$ *进行唯一确定$1 \leq \alpha \leq n$，*和*$g = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$。

免费群$F(X)$可享受以下泛性质：

#### 命题 8 {#alg-i-s7-prop-8 .statement tag=05FR}

*设 G 为群且 f 映射 of* $X$ *进入 G。存在且仅有一个同态* $\bar{f}$ *of* $F(X)$ *进入 G，其中扩展 f*。

唯一性或 $\bar{f}$ 是因为群 $F(X)$ 是由$X$ 生成的。对于$X$中的所有$x$，令$f_x$为$\mathbf{Z}$到$G$的同态$n \mapsto f(x)^n$。到no. 3，命题 4，$F(X)$中存在同态$\bar{f}$进入$G$，使得$\bar{f}(x^n) = f_x(n)$对应于$x \in X$和$n \in \mathbf{Z}$；特别是，$\bar{f}(x) = f_x(1) = f(x)$适用于所有$x \in X$，因此$\bar{f}$扩展$f$。

令 $u : X \to Y$ 为映射。到命题 8 时，$F(X)$ 到 $F(Y)$ 中存在且仅有一个同态，其中重合和 $X$ 上的 $u$；它用$F(u)$表示。以岩浆为例 (no. 1) 公式

$$
F(v \circ u) = F(v) \circ F(u)
$$

对于每个映射 $v : Y \to Z$ 成立，并且证明如果 $u$ 是单射，则 $F(u)$ 是单射（分别是满射、双射的）。对于$X$的每个子集$S$，$F(S)$将被$S$生成的$F(X)$的子群识别。

设I为集合。在某些情况下，值得注意的是，不要将认同 $i$ 放在 I 中，而将典范像 $\phi_i(1)$ 放在免费的群 $F(I)$ 中；后者将用 $T_i$（或 $T'_i, X_i, \ldots$，视情况而定）表示，并称为指标 $i$ 的*不确定*。自由的群$F(I)$则表示为$F((T_i)_{i \in I})$或$F(T_1, \ldots, T_n)$（如果$I = \{1, 2, \ldots, n\}$）。

令$G$为群且$t = (t_i)_{i \in I}$为元素的族$G$。到命题 8 时，$F((T_i)_{i \in I})$ 中存在同态 $f_t$ 进入$G$，其特征在于所有 $i \in I$ 的$f_t(T_i) = t_i$。 $f_t$下的元素$w$、$F((T_i)_{i \in I})$的像将用$w(t)$或$w(t_1, \ldots, t_n)$表示，如果$I = \{1, 2, \ldots, n\}$；据说$w(t)$是由$w$中的*代换* $T_i \mapsto t_i$产生的。特别是，如果我们取$G = F((T_i)_{i \in I})$，$(t_i) = (T_i) = T, f_T$是$G$的恒等式同态，则从而$w(T) = w$； $I = \{1, 2, \ldots, n\}$，然后$w(T_1, \ldots, T_n) = w$。

令$G$和$G'$为$G$的两个群、$u$同态转化为$G$中元素的$G'$和$t = (t_1, \ldots, t_n)$有限序列。 设 $t' = (u(t_1), \ldots, u(t_n))$；对于$1 \leq i \leq n$，将$F(T_1, \ldots, T_n)$的同态$u \circ f_t$转化为$G'$映射$T_i$到$u(t_i)$，因此等于$f_{t'}$；对于$F(T_1, \ldots, T_n)$中的$w$，则

$$
u(w(t_1, \ldots, t_n)) = w(u(t_1), \ldots, u(t_n)).
$$

让$w$在$F(T_1, \ldots, T_n)$中给出，而元素$v_1, \ldots, v_n$在自由的群$F(T'_1, \ldots, T'_m)$中给出。 代换$T_i \mapsto v_i$定义元素$w' = w(v_1, \ldots, v_n)$共$F(T'_1, \ldots, T'_m)$。令$G$为群、$G$的$t_1, \ldots, t_m$元素和$F(T'_1, \ldots, T'_m)$的$u$同态进入$G$，其特征为$u(T'_j) = t_j$为$1 \leq j \leq m$。然后$u(v_i) = v_i(t_1, \ldots, t_m)$和$u(w') = w(t_1, \ldots, t_m)$； 公式 (8) 因此意味着

$$
w'(t_1, \ldots, t_m) = w(v_1(t_1, \ldots, t_m), \ldots, v_n(t_1, \ldots, t_m)).
$$

这证明了“功能记号”$w(t_1, \ldots, t_n)$的合理性。读者将扩展公式（8）和（9）留给任意索引集合的情况。

### 6. 群的展示

令$G$为群且$t = (t_i)_{i \in I}$为$G$的元素族。 Let $f_t$ be the unique homomorphism of the free group $F(I)$ into $G$ which maps $i$ to $t_i$. $f_t$的像是$G$的元素$t_i$生成的子群。 元素、核、$f_t$被称为家庭$t$的*亲戚*。 $t$ 称为 *生成的*（分别称为 *生成的*） *自由*，*基本*）如果 $f_t$ 是满射（分别是单射、双射的）。

设$G$为群。 $G$的*表示*是生成的族$\mathbf{t} = (t_i)_{i \in I}$和关系器族$\mathbf{r} = (r_j)_{j \in J}$的有序对$(\mathbf{t}, \mathbf{r})$由……组成，使得$f_t$的核$N_t$由元素生成$gr_jg^{-1}$ 对应 $g \in F(I)$ 和 $j \in J$。也就是说，$N_t$是$j \in J$的$r_j$生成的$F(I)$的正常子群（在其他字，最小的$F(I)$包含的正常子群） 元素$r_j$（$j \in J$）、cf.§ 4, no. 4）。通过滥用语言，生成元$t_i$和关系$r_j(\mathbf{t}) = e$据说构成了群$G$的*演示*。

令I为集合，而$r = (r_j)_{j \in J}$为自由群$F(I)$的元素家庭。令$N(r)$为由$r_j$为$j \in J$生成的$F(I)$的正常子群。令$F(I, r) = F(I)/N(r)$和$\tau_i$表示$i$模$N(r)$的类。 有序对 $(\tau, r)$ 与 $\tau = (\tau_i)_{i \in I}$ 是群 $F(I, r)$ 的呈现；如果$G$是群并且$(t, r)$是$G$与$t = (t_i)_{i \in I}$的表示，则存在$F(I, r)$到$G$的唯一同构$u$，使得$u(\tau_i) = t_i$对于所有$i \in I$。据说群$F(I, r)$是由生成元$\tau_i$和关系词$r_j$定义的，或者滥用语言，它是*由生成元$\tau_i$和关系*$r_j(\tau) = e$定义的。当$I = \{1, n\}$和$J = \{1, m\}$时，称$F(I, r)$由表示定义

$$
\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle.
$$

如果$r_j = u_j^{-1} v_j$与$u_j$和$v_j$在$F(I)$中，则该表示同样用符号表示

$$
\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle.
$$

#### 例 {#alg-i-s7-n6-exa-1 .statement tag=05FS}

(1) 由表示法$\langle \tau; \tau^q = e \rangle$定义的群是阶$q$的循环。

(2) 由表示法$\langle x, y; xy = yx \rangle$定义的群与$\mathbf{Z} \times \mathbf{Z}$同构的。

#### 命题 9 {#alg-i-s7-prop-9 .statement tag=05FT}

*令$G$为群，$t = (t_i)_{i \in I}$生成的为$G$的家族，$r = (r_j)_{j \in J}$为$t$的关系者家族。以下条件是等效的：*

(a) *有序对* $(t, r)$ *是*$G$的呈现。

(b) *设*$G'$*为群且*$t' = (t'_i)_{i \in I}$*元素的家族*$G'$。 *如果* $r_j(t') = e$ *对于所有* $j \in J$，*存在* $G$ *到* $G'$ *的同态* $u$ *这样* $u(t_i) = t'_i$ *对于所有* $i \in I$。

(c) *令* $\overline{G}$ *为群和* $\bar{t} = (\bar{t}_i)_{i \in I}$ *生成的家族* $\overline{G}$ *使得* $r_j(\bar{t}) = e$ *对于所有* $j \in J$。 *每同态*$\overline{G}$*进入*$G$*其中映射*$\bar{t}_i$*到*$t_i$*对于所有*$i \in I$*是同构*。

让$f$表示$F(I)$的同态到$G$，其中对于$f$的所有$i \in I$和$N$核，映射$i$到$t_i$。

(a) $\Rightarrow$ (b)：假设$(t, r)$是$G$的表示，并让$t' = (t'_i)_{i \in I}$是群$G'$的元素的族，其中$r_j(t') = e$代表所有$j \in J$。令$f'$为$F(I)$的同态到$G'$，其特征为所有$i \in I$的$f'(i) = t'_i$。对于所有 $j \in J$，由假设 $f'(r_j) = e$ 生成，并且对于 $j \in J$ 和 $g \in F(I), f'(N) = \{e\}$，$N$ 由元素 $gr_jg^{-1}$ 生成。由于同态$f \colon F(I) \to G$与核$N$是满射，因此存在同态$u \colon G \to G'$使得$f' = u \circ f$。然后$u(t_i) = u(f(i)) = f'(i) = t'_i$。

(b) $\Rightarrow$ (c)：假设条件 (b) 成立。令$t = (t_i)_{i \in I}$为群$G$的生成的族，使得$r_j(t) = e$对于所有$j \in J$，并令$v$为$\overline{G}$到$G$的同态，使得$v(\bar{t}_i) = t_i$对于所有$i \in I$。由于家庭$(t_i)_{i \in I}$生成$G$，同态$v$是*满射*。到性质 (b) 时，存在同态 $u \colon G \to \overline{G}$，使得 $u(t_i) = \bar{t}_i$ 对于所有 $i \in I$。那么$u(v(\bar{t}_i)) = \bar{t}_i$对于所有$i \in I$，因此$u \circ v$是$\overline{G}$上的恒等式，这证明$v$是单射的。因此$v$是同构并且条件(c)成立。

(c) $\Rightarrow$ (a)：假设条件 (c) 成立。设$t'_i$为$F(I, r)$和$t' = (t'_i)_{i \in I}$中$i$的典范像；那么 $r_j(t') = e$ 对于所有 $j \in J$。由于$r_j(t) = e$对于所有$j \in J$来说，在$F(I, r)$到$G$中存在且仅有一个同态$v$，使得$v(t_i) = t_i$对于所有$i \in I$。通过(c)，$v$是$F(I, r)$的同构到$G$，其中变换将$F(I, r)$的呈现$(t', r)$转换成$G$的呈现$(t, r)$。

### 7.自由交换群和幺半群

$X$的所有映射到$\mathbf{Z}$的集合$\mathbf{Z}^X$是由$(\alpha + \beta)(x) = \alpha(x) + \beta(x)$($\alpha, \beta \in \mathbf{Z}^X, x \in X$)定义的律下的交换律群； $\mathbf{Z}^X$ 中的元素是有时称为多重索引。 单位元素，用0表示，是常数映射，值为0。对于$\alpha \in \mathbf{Z}^X$，$x \in X$的集合$S_\alpha$，使得$\alpha(x) \neq 0$称为$\alpha$的支撑；然后 $S_0 = \varnothing$ 和 $S_{\alpha+\beta} \subset S_\alpha \cup S_\beta$ 对应 $\mathbf{Z}^X$ 中的 $\alpha, \beta$。因此有限支撑的映射$\alpha : X \to \mathbf{Z}$的集合$\mathbf{Z}^{(X)}$是$\mathbf{Z}^X$的子群，称为在$X$上构造的自由交换群。

对于所有 $x \in X$，令 $\delta_x$ 表示 $\mathbf{Z}^{(X)}$ 的元素定义为

$$
\delta_x(y) = \begin{cases}
1 & \text{if } y = x \\
0 & \text{if } y \neq x.
\end{cases}
$$

另外，对于$\alpha \in \mathbf{Z}^{(X)}$、整数、$|\alpha|$、$\alpha$的长度由公式定义

$$
|\alpha| = \sum_{x \in X} \alpha(x).
$$

以下关系立即成立：

$$
\alpha = \sum_{x \in X} \alpha(x) \cdot \delta_x
$$
$$
|\delta_x| = 1, \quad |0| = 0
$$
$$
|\alpha + \beta| = |\alpha| + |\beta|
$$

对于$\mathbf{Z}^{(X)}$中的$\alpha, \beta$和$X$中的$x$。

对于所有 $x \in X$，序关系 $\alpha \leq \beta$ 在 $\mathbf{Z}^{(X)}$ 中由 $\alpha(x) \leq \beta(x)$ 定义。 关系$\alpha \leq \beta$和$\alpha' \leq \beta'$意味着$\alpha + \alpha' \leq \beta + \beta'$、$|\alpha| \leq |\beta|$和$-\alpha \geq -\beta$；此外，关系$\alpha \leq \beta$相当于$\beta - \alpha \geq 0$。 $\mathbf{Z}^{(X)}$中元素$\alpha \geq 0$的集合用$\mathbf{N}^{(X)}$表示；它是$X$的映射的集合到有限支撑的$\mathbf{N}$，并且它是$\mathbf{Z}^{(X)}$的子幺半群，称为在$X$上构造的自由交换幺半群。 长度 1 中的元素是$\mathbf{N}^{(X)} - \{0\}$ 中的最小元素，并构成$\delta_x$ ($x \in X$) 中的集合。

幺半群$\mathbf{N}^{(X)}$和群$\mathbf{Z}^{(X)}$享有以下泛性质。

#### 命题 10 {#alg-i-s7-prop-10 .statement tag=05FU}

*设 M 是可交换幺半群（分别为群），并且 X 的 f 映射进入 M。存在且仅有一个 $\mathbf{N}^{(X)}$（分别为 $\mathbf{Z}^{(X)}$）的同态进入 M，这样*对于所有 $x \in X$ 都有 $g(\delta_x) = f(x)$。 *如果 M 是相加的，则* $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$ 对于 $\mathbf{N}^{(X)}$ 中的所有 $\alpha$（或 $\mathbf{Z}^{(X)}$）。

令$g$为$\mathbf{N}^{(X)}$（或$\mathbf{Z}^{(X)}$）到M中的同态，使得$g(\delta_x) = f(x)$对于所有$x \in X$。对于$\mathbf{N}^{(X)}$（或$\mathbf{Z}^{(X)}$）中的所有$\alpha$，从 (12) 得出
$$
g(\alpha) = \sum_{x \in X} \alpha(x) \cdot g(\delta_x) = \sum_{x \in X} \alpha(x) \cdot f(x),
$$
从而唯一性共$g$。

对于$\mathbf{N}^{(X)}$（或$\mathbf{Z}^{(X)}$）中的所有$\alpha$，我们写为$g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$。那么显然$g(0) = 0$；对于$\mathbf{N}^{(X)}$中的$\alpha, \beta$（分别为$\mathbf{Z}^{(X)}$），
$$
\begin{align*}
g(\alpha + \beta) &= \sum_{x \in X} (\alpha(x) + \beta(x)) \cdot f(x) \\
&= \sum_{x \in X} [\alpha(x) \cdot f(x) + \beta(x) \cdot f(x)] \\
&= \sum_{x \in X} \alpha(x) \cdot f(x) + \sum_{x \in X} \beta(x) \cdot f(x) \\
&= g(\alpha) + g(\beta)
\end{align*}
$$
因此 $g$ 是 $\mathbf{N}^{(X)}$（或 $\mathbf{Z}^{(X)}$）到 M 中的同态。另外，对于 $X$ 中的 $y$，
$$
g(\delta_y) = \sum_{x \in X} \delta_y(x) \cdot f(x);
$$
现在$\delta_y(x) \cdot f(x) = 0$适用于$x \neq y$和$\delta_y(y) \cdot f(y) = f(y)$，从而$g(\delta_y) = f(y)$。

设$u : X \to Y$为映射。到命题 10 时，$\mathbf{Z}^{(X)}$ 到 $\mathbf{Z}^{(Y)}$ 中存在且仅有一个同态，其中对于所有 $x \in X$，映射 $\delta_x$ 到 $\delta_{u(x)}$。用$\mathbf{Z}^{(u)}$表示；立即可以看出，映射$\alpha \in \mathbf{Z}^{(X)}$到元素$\beta \in \mathbf{Z}^{(Y)}$定义为
$$
\beta(y) = \sum_{x \in u^{-1}(y)} \alpha(x).
$$
与岩浆 (no. 1) 的情况一样，每映射 $v : Y \to Z$ 都建立公式 $\mathbf{Z}^{(v \circ u)} = \mathbf{Z}^{(v)} \circ \mathbf{Z}^{(y)}$；还表明，如果 $u$ 是，则 $\mathbf{Z}^{(u)}$ 是单射（分别是满射、双射的）。

Let S be a subset of X; if i is the injection of S into X, the mapping $f = \mathbf{Z}^{(i)}$ is an isomorphism of $\mathbf{Z}^{(S)}$ onto the subgroup H of $\mathbf{Z}^{(X)}$ generated by the elements $\delta_s$ for $s \in S$. 由(15)，
$$
(f(\alpha))(x) = \begin{cases}
\alpha(x) & \text{if } x \in S \\
0 & \text{if } x \in X - S
\end{cases}
$$

因此$H$是$S$中包含的支持$\mathbf{Z}^{(X)}$的元素的集合。从此以后，$\mathbf{Z}^{(S)}$ 将通过$f$ 与$H$ 进行标识。

公式(15)表明$\mathbf{Z}^{(u)}$的限制到$\mathbf{N}^{(X)}$诱导同态$\mathbf{N}^{(u)}$到$\mathbf{N}^{(X)}$到$\mathbf{N}^{(Y)}$。然后每映射 $v : Y \to Z$ $\mathbf{N}^{(v \circ u)} = \mathbf{N}^{(v)} \circ \mathbf{N}^{(u)}$；此外，如果 $u$ 是，则 $\mathbf{N}^{(u)}$ 是单射（分别是满射、双射的）。如果$S$是$X$中的子集，

$$
\mathbf{N}^{(S)} = \mathbf{Z}^{(S)} \cap \mathbf{N}^{(X)}.
$$

#### 注 {#alg-i-s7-n7-rem-1 .statement tag=05FV}

令$M$严格为正整数的乘法幺半群，并令$\mathfrak{P}$为素数数的集合（§ 4, no. 10，定义15）。到命题 10 时，$\mathbf{N}^{(\mathfrak{P})}$ 中存在同态 $u$ 到$M$，其特征在于对于每个素数数 $p$ 具有$u(\delta_p) = p$。那么$\mathbf{N}^{(\mathfrak{P})}$中的$\alpha$和定理 7 of § 4, no. 10的$u(\alpha) = \prod_{p \in \mathfrak{P}} p^{\alpha(p)}$表明$u$是$\mathbf{N}^{(\mathfrak{P})}$到$H$的同构。

### 8.指数记号

令 $M$ 为幺半群，乘法书写，$u = (u_x)_{x \in X}$ 为 $M$ 的元素族，在对通勤。设$\alpha$在$\mathbf{N}^{(X)}$中； 元素 $u_x^{\alpha(x)}$ 和 $M$ 的 $u_y^{\alpha(y)}$ 在 $X$ 中通勤 $x, y$，并且存在 $X$ 的有限子集 $S$，使得 $u_x^{\alpha(x)} = 1$ 在 $x$ 中$X - S$。因此我们可以这样写：

$$
u^\alpha = \prod_{x \in X} u_x^{\alpha(x)}.
$$

设$M'$为$(u_x)_{x \in X}$族生成的$M$中的子幺半群；它是可交换的（§ 1, no. 5，推出 2 到命题 4）。因此，$\mathbf{N}^{(X)}$存在$M'$的(no. 7，命题10)唯一同态$f$，使得$f(\delta_x) = u_x$对于所有$x \in X$和$f(\alpha) = u^\alpha$对于所有$\alpha$ $\mathbf{N}^{(X)}$。我们推导出以下公式

$$
u^{\alpha + \beta} = u^\alpha . u^\beta
$$
$$
u^0 = 1
$$
$$
u^{\delta_x} = u_x
$$

对于$\mathbf{N}^{(X)}$中的$\alpha, \beta$和$X$中的$x$。

设$v = (v_x)_{x \in X}$为$M$的元素的另一个族；假设$X$中的$x, y$有$v_x v_y = v_y v_x$和$u_x v_y = v_y u_x$。那么存在（§ 1, no. 5，推论2到命题4）$M$的可交换子幺半群$L$，使得$u_x \in L$和$v_x \in L$对于所有$x \in X$。 $\mathbf{N}^{(X)}$的映射$\alpha \mapsto u^\alpha . v^\alpha$到$L$则为同态（§ 1, no. 5，命题5）映射$\delta_x$到$u_x . v_x$。因此我们有公式

$$
u^\alpha . v^\alpha = (u . v)^\alpha,
$$

其中$u . v$是家庭$(u_x . v_x)_{x \in X}$。

当M是可交换的时，可以为M的元素的每个族$u$定义$u^\alpha$，并且公式(15)到(20)成立，而无需限制。

### 9. 关系各种免费对象之间

由于自由幺半群Mo(X)是岩浆，no. 1的命题1表明同态$\lambda : M(X) \to Mo(X)$的存在，其中限制到X是恒等式。类似地，由于自由群 F(X) 是 X 扩展到同态 $\mu : Mo(X) \to F(X)$ (no. 2, 命题 3) 的幺半群恒等映射。通过no. 4、命题 6 和no. 5、命题 7，$\mu$ 是单射的。类似地，no. 7的命题10和no. 5的命题8表明对于所有$x \in X$，存在以$\nu(x) = \delta_x$和$\pi(x) = \delta_x$为特征的同态、$\nu : Mo(X) \to N^{(X)}$和$\pi : F(X) \to Z^{(X)}$。如果$i$是将$N^{(X)}$的单射转化为$Z^{(X)}$，则Mo(X)的两个同态$i \circ \nu$和$\pi \circ \mu$转化为X上的$Z^{(X)}$重合， 从而$i \circ \nu = \pi \circ \mu$。这种情况可以用下面的交换图表来概括：

$$
\begin{array}{ccc}
M(X) & \xrightarrow{\lambda} & Mo(X) \\
& & \downarrow \mu \\
& & F(X) \xrightarrow{\pi} Z^{(X)}
\end{array}
$$

同态 $\lambda, \mu, \nu$ 和 $\pi$ 将被称为规范的。

设w在M(X)中； $l(w)$上的归纳立即证明字$\lambda(w)$的长度等于w的长度。而且

$$
\nu(x_1 \ldots x_n) = \sum_{i=1}^n \delta_{x_i}
$$
对于 X 中的$x_1, \ldots, x_n$，从而 $|\nu(x_1 \ldots x_n)| = n$，由 (13) 和 (14) 得出。在其他字，

$$
|\nu(u)| = l(u) \quad (u \in Mo(X)).
$$

#### 命题 11 {#alg-i-s7-prop-11 .statement tag=05FW}

*Mo(X)的典范同态$\nu$到$N^{(X)}$是满射。*设$w = x_1 \ldots x_n$和$w' = x'_1 \ldots x'_m$是Mo(X)的两个元素；在阶、$\nu(w) = \nu(w')$中，$m = n$是充分必要的，且存在置换、$\sigma \in S_n$、$1 \leq i \leq n$存在$x'_i = x_{\sigma(i)}$。

$\nu$的像是$N^{(X)}$包含元素$\delta_x$的子幺半群I（对于$x \in X$）。 公式 (12) (no. 7) 表明$N^{(X)}$是由$(\delta_x)_{x \in X}$族生成的，其中$I = N^{(X)}$。 因此 $\nu$ 是满射的。

如果$m = n$和$x'_i = x_{\sigma(i)}$对于$1 \leq i \leq n$，那么

$$
\nu(w') = \sum_{i=1}^n \delta_{x'_i} = \sum_{i=1}^n \delta_{x_{\sigma(i)}} = \sum_{i=1}^n \delta_{x_i} = \nu(w)
$$

由公式 (21) 和交换律定理 (§ 1, no. 5, 定理 2)。

相反，假设$v(w)$和$v(w')$等于$\mathbf{N}^{(X)}$的相同元素$\alpha$；由公式 (22), $n = |\alpha| = m$。对于所有$x \in X$，令$I_x$（或$I'_x$）为整数$i$的集合，使得$1 \leq i \leq n$和$x_i = x$（或$x'_i = x$）。因此$(I_x)_{x \in X}$和$(I'_x)_{x \in X}$是$\mathbf{N}$的区间$[1, n]$的划分；此外，公式
$$
\alpha = \sum_{i=1}^n \delta_{x_i}
$$
证明$\alpha(x)$是$I_x$的基数；同样公式
$$
\alpha = \sum_{i=1}^n \delta_{x'_i}
$$
证明$\alpha(x)$是$I'_x$的基数。因此，存在$[1, n]$的置换$\sigma$，使得$\sigma(I'_x) = I_x$对于所有$x \in X$，即$x'_i = x_{\sigma(i)}$对于$i = 1, \ldots, n$。

#### 注 {#alg-i-s7-n9-rem-1 .statement tag=05FX}

令$S$为$X$的子集。回想一下，我们已经识别出$M(S)$具有$M(X)$的子岩浆，$Mo(S)$具有$Mo(X)$的子幺半群，以及$N^{(S)}$具有子幺半群的$N^{(X)}$。然后
$$
M(S) = \lambda^{-1}(Mo(S)).
$$
显然$\lambda(M(S)) \subset Mo(S)$。令 $w \in \lambda^{-1}(Mo(S))$；我们通过归纳在$l(w)$上显示$w \in M(S)$。显然如果$l(w) = 1$。如果$l(w) > 1$，我们可以将$w = w_1 w_2$写成$w_1, w_2 \in M(X)$，$l(w_1) < l(w)$，$l(w_2) < l(w)$。然后$\lambda(w_1) \lambda(w_2) \in Mo(S)$，$\lambda(w_1) \in Mo(S)$和$\lambda(w_2) \in Mo(S)$，从而$w_1 \in M(S)$和$w_2 \in M(S)$，归纳假设，最后$w \in M(S)$。

还有
$$
Mo(S) = v^{-1}(N^{(S)}).
$$
这紧随公式 (21)。

进一步地，$N^{(S)}$是$N^{(X)}$的元素的集合，其支持包含在$S$中；如果$(S_i)_{i \in I}$是交$S$的$X$的子集族，那么$N^{(S)} = \bigcap_{i \in I} N^{(S_i)}$和公式 (23)和(24)意味着
$$
M(S) = \bigcap_{i \in I} M(S_i), \quad Mo(S) = \bigcap_{i \in I} Mo(S_i).
$$

### 习题 {#alg-i-s7-exercises}

§ 7](exercises/s7/)参见[习题。
