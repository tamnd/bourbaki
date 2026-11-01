---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 8
section_title: Lie groups over R or Qp
lang: zh
source: lie-i-iii
book_pages: 337-342, 395-397
pdf_pages: 0355-0360, 0413-0415
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS MORPHISMS
      page: 337
      pdf_page: 355
    - "no": 2
      title: CLOSED SUBGROUPS
      page: 340
      pdf_page: 358
statements: 9
exercises: 7
content_sha256: e9077b682af728800b4926c315bb814fee40066142fe8a16669e5c6d04acc113
translated_from: content/en/lie/III/08_s8_lie_groups_over_r_or_qp.md
translation_method: google
source_content_sha256: 9a8748db60c9fd84976b7413bf30ec32e2a4b17c04a06e968ec301e544a51660
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 81134980d048290ddc1fea55d884df996c0f05c978503a4eab485539667997bb
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 8。 李群超过$\mathbf{R}$且$\mathbf{Q}_p$

### 1. 连续态射

#### 定理 1 {#lie-iii-s8-thm-1 .statement tag=0AI2}

*令 G 和 H 为超过 $\mathbf{R}$ 或 $\mathbf{Q}_p$ 的两个李群细菌。设 f 是 G 到 H 的连续态射。那么 f 是解析的。*

我们给出 $L(G)$ 和 $L(H)$ 范数以及定义它们的拓扑，并且对于所有 $x, y$ 都有 $\| [x, y] \| \leq \|x\| \|y\|$。在 $L(G)$ 中存在中心 0 的开球V，并且在 V 上定义 G 的指数映射 $\phi$，使得： (1) $\phi(V)$ 是 G 中$e$ 的开球邻域； (2) $\phi$是解析式流形V到解析式流形$\phi(V)$的同构； (3) $\phi(nx) = \phi(x)^n$对于所有$x \in V$和所有$n \in \mathbf{Z}$使得$nx \in V$。我们类似地对 W 定义和 H $\psi$。如有必要，通过缩小 V，可以假设 $f(\phi(V)) \subset \psi(W)$。那么$g = \psi^{-1} \circ f \circ \phi$就是V到W的连续映射。

我们表明
$$
(x \in V, \lambda \in \mathbf{Q} \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
可以假设$\lambda \neq 0$。让$\lambda = \frac{r}{q}$和$r, q$进入$\mathbf{Z} - \{0\}$。让$y = \frac{r}{q} x$。

如果$K = \mathbf{R}$，我们写$z = \frac{x}{q} = \frac{y}{r} \in V$。然后$x = qz, y = rz$，从而
$$
g(x) = \psi^{-1}(f(\phi(qz))) = \psi^{-1}(f(\phi(z)^q)) = \psi^{-1}(f(\phi(z))^q).
$$
我们证明$\psi^{-1}(f(\phi(z))^q) = q \psi^{-1}(f(\phi(z))) = qg(z)$。只要验证一下，如果$u \in \psi(W)$使得$u^q \in \psi(W)$，则$\psi^{-1}(u^q) = q \psi^{-1}(u)$；但如果$u = \psi(v)$，$u^q = \psi(v^q)$，则$v^1/q \in W$和$(\psi(v^1/q))^q = u^q$，因此$\psi(v^1/q) = u = \psi(v)$，因此$v^1 = qv$。

同样，$g(y) = rg(z)$，从而 (1)。

如果$K = \mathbf{Q}_p$，我们再次写$z = rx = qy \in V$、从而、$g(z) = rg(x) = qg(y)$、从而（1）。

由于 $\mathbf{Q}$ 在 $K$ 中是稠密的，(1) 意味着
$$
(x \in V, \lambda \in K \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
令$x \in L(G)$和$\lambda, \lambda'$为$K^*$的元素，使得$\lambda x \in V, \lambda' x \in V$。然后
$$
g(\lambda' x) = g\left( \frac{\lambda'}{\lambda} \lambda x \right) = \frac{\lambda'}{\lambda} g(\lambda x)
$$
由 (2) 得出 $\frac{1}{\lambda} g(\lambda x) = \frac{1}{\lambda'} g(\lambda' x)$。因此，$g$到$L(G)$的扩张$h$是通过对所有$\lambda$写出$h(x) = \frac{1}{\lambda} g(\lambda x)$来定义的，这样$\lambda x \in V$。显然 $h$ 是连续的。我们表明
$$
(x \in L(G) \text{ and } \lambda \in K) \Rightarrow h(\lambda x) = \lambda h(x).
$$
令 $\lambda' \in K^*$ 满足 $\lambda' x \in V$ 和 $\lambda' \lambda x \in V$。然后
$$
h(\lambda x) = \frac{1}{\lambda'} g(\lambda' \lambda x) = \frac{1}{\lambda'} \lambda g(\lambda' x) = \lambda \frac{1}{\lambda'} g(\lambda' x) = \lambda h(x).
$$
令$x, y$位于$L(G)$中。然后，到 § 4, no. 3 的命题 4，
$$
\begin{align*}
h(x) + h(y) &= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(\lambda h(x)) \psi(\lambda h(y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(h(\lambda x)) \psi(h(\lambda y))).
\end{align*}
$$
对于 $|\lambda|$ 足够小，$\lambda x \in V$ 和 $\lambda y \in V$，因此上述表达式等于
$$
\begin{align*}
&\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(f(\phi(\lambda x)) f(\phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} (\psi^{-1} \circ f)(\phi(\lambda x) \phi(\lambda y)) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} g(\phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} h(\lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(x + y).
\end{align*}
$$
因此 $h$ 是连续且线性的，因此 $g = h|V$ 是解析的，因此 $f$ 是 $\phi(V)$ 的解析，因此 $f$ 是解析的 (§ 1, no. 10)。

#### 推论 1 {#lie-iii-s8-thm-1-cor-1 .statement tag=0AI3}

设$G$为拓扑群。 $G$ 上最多存在一个解析流形结构超过$\mathbf{R}$（或$\mathbf{Q}_p$）与$G$ 上的拓扑群结构兼容。

这紧随定理 1 而来。

#### 定义 1 {#lie-iii-s8-def-1 .statement tag=0AI4}

*拓扑群 G 称为实数（分别为 p-adic）李群，如果 G 上存在实数（分别为 p-adic）李群结构与其拓扑兼容。*

那么结构是唯一的，我们可以说这样的群的*维数*。如果 G 和 H 是两个这样的群，则 G 到 H 中的每个连续态射都是解析的。

#### 推论 2 {#lie-iii-s8-def-1-cor-2 .statement tag=0AI5}

*设 G 是 e 的拓扑群和 V 开邻域。假设 V 具有解析流形结构，使其成为实数（或 p-adic）李群胚芽。那么 G 是实数（分别为 p-adic）李群.*

让$g \in G$。 G 中存在 $e$ 的开邻域 $V'$，使得 $V' \cup gV'g^{-1} \subset V$。 $V'$到$V$的映射$v \mapsto gv g^{-1}$是连续的，因此是李群胚芽$V'$到李群胚芽$V$的解析态射。那么就足以满足 § 1, no. 9 中的应用命题 18 了。

#### 注{#lie-iii-s8-n1-rem-1 .statement tag=0AI6}

(1) 如果 $\mathbf{R}$（或 $\mathbf{Q}_p$）被 $\mathbf{C}$ (习题 1) 取代，定理 1 及其推论不再成立。

(2) 设G是拓扑群。可以证明†以下条件是等价的： (a) G是有限维实李群； (b) G 是局部紧的，并且存在 $e$ 包含中的邻域，不存在与 $\{e\}$ 不同的子群； (c) 存在 $e$ 的开邻域同胚于空间 $\mathbf{R}^n$ 的开球。 （对于不太困难的结果，cf.习题6。）

#### 命题 1 {#lie-iii-s8-prop-1 .statement tag=0AI7}

*设 G、G' 为拓扑群，且 f 为 G 到 G' 的连续态射。假设以下三种情况之一成立：
(a) G 是实李群并且 G' 是 p 进数李群；
(b) G 是 p-adic 李群并且 G' 是实李群；
(c) G 是 p-adic 李群，G' 是 $p'$-adic 李群，且有 $p \neq p'$。
那么 f 是局部常数。*

案例（一）。设$G_0$为G的恒等分量。则$f(G_0)$是$G'$的连通子群，因此$f(G_0) = \{e\}$和$G_0$在G中开。

情况（b）。令$V'$为$G'$中$e$的邻域，使得$G'$的每个子群包含在$V'$约化到$\{e\}$中（§ 4, no. 2，推论1到定理2）。 G 中存在$e$ 的邻域 V，使得$f(V) \subset V'$。则存在 G 的开子群 $G_1$，使得 $G_1 \subset V$ (§ 7, no. 1, 命题 1)。然后$f(G_1) = \{e\}$。

情况（c）。根据§ 7、定理 4 以及命题 8 的推论，$G'$ 中存在 $e$ 的邻域 $V'$，因此，对于所有 $x' \in V' - \{e\}$，${x'}^{p^n}$ 不倾向于

† 请参阅例 D. Montgomery 和L。 Zippin，*拓扑变换群*，Interscience 纯数学和应用数学小册子，no. 1，Interscience 出版社，纽约 1955 年（特别是第 169 和 184 页）。

到$e$，因为$n$趋于$+\infty$。 $G$中存在$e$的邻域$V$，使得$f(V) \subset V'$。在 § 7、定理 4 和命题 9 时，存在 $G$ 的开子群 $G_1$，使得 $G_1 \subset V$ 并且对于所有 $x \in G_1$，$x^{p^n}$ 趋向于 $e$ $n$趋于$+\infty$。然后$f(G_1) = \{e\}$。

### 2. 关闭子群

#### 定理 2 {#lie-iii-s8-thm-2 .statement tag=0AI8}

*令$G$为$\mathbf{R}$或$\mathbf{Q}_p$的有限维李群。 $G$ 的每个闭合子群都是 $G$ 的谎言子群。更一般地，令$U$是$G$中$e$的对称开邻域，而$H$是$U$的非空闭子空间，使得条件$x \in H$、$y \in H$和$xy^{-1} \in U$ 意味着$xy^{-1} \in H$。那么 $H$ 就是 $G$ 的谎言子群萌芽。*

设 $\mathfrak{h}$ 为在 $e$ 处与 $H$ 相切的谎言子代数（§ 4, no. 5，定义 2）。存在$G$的谎言子群胚芽$H_0$与李代数$\mathfrak{h}$并包含在$H$中。我们证明$H_0$在$H$开路，并由$G$诱导拓扑开路。这将证明$H$是$G$的解析子流形，并将建立定理。

$L(G)$中存在对$\mathfrak{h}$的补充向量子空间$\mathfrak{k}$，$\mathfrak{h}$和$\mathfrak{k}$中分别存在零的对称开邻域$V_1, V_2$以及指数映射 $G$的$\phi$定义在$V_1 + V_2$上，并拥有以下属性：

(a) 映射 $(a_1, a_2) \mapsto \phi(a_1)\phi(a_2)$ 是 $V_1 \times V_2$ 的解析同构到 $G$ 的开子集 $V$；
(b) $\phi(V_1) \subset H_0$；
(c) $V^2 \subset U$。

我们将证明（并且这将实现证明）在$V_2$中存在0的开邻域$V'_2$使得$H \cap (\phi(V_1)\phi(V'_2)) = \phi(V_1)$。

假设断言为假。然后我们可以发现$V_1$中的序列$(x_n)$和$V_2 - \{0\}$中的序列$(y_n)$趋于0，这样对于所有$n$来说$\phi(x_n)\phi(y_n) \in H$。然后通过(c) $\phi(y_n) \in H$。

如果$K = \mathbf{Q}_p$，可以假设$V_2$是$\mathfrak{k}$的加法子群，并且对于所有$a \in V_2$和所有$p \in \mathbf{Z}$来说$\phi(pa) = \phi(a)^p$。然后对所有$\lambda \in \mathbf{Z}$有$\phi(\lambda y_1) \in H$，因此对所有$\lambda \in \mathbf{Z}_p$具有连续性。 $\mathbf{Z}_p$到$G$的映射$f : \lambda \mapsto \phi(\lambda y_1)$是解析的，并在$H$和$(T_0f)(1) = y_1$中取其值。因此$y_1 \in \mathfrak{h}$，这是荒谬的。因此，在$\mathbf{Q}_p$的情况下，定理成立。

如果$K = \mathbf{R}$，则可以假设$V_2$连通，且$y_n$属于至$\frac{1}{2}V_2 - \{0\}$。如果需要的话，通过取$(y_n)$的子序列，我们可以找到非零标量的序列$(\lambda_n)$，使得$\lambda_n^{-1}y_n$趋向于$V_2 - \{0\}$的元素$y$。 序列 $(\lambda_n)$趋于0。令$\lambda \in \mathbf{R}$使得$\lambda y \in \frac{1}{2}V_2$；我们证明$\exp(\lambda y) \in H$。可以假设 $\lambda \lambda_n^{-1}y_n \in \frac{1}{2}V_2$ 对于所有$n$。令 $k_n \in \mathbf{Z}$ 使得 $|\lambda - k_n \lambda_n|$ 趋于 0。对于 $n$ 足够大，$(\lambda - k_n \lambda_n)\lambda_n^{-1}y_n \in \frac{1}{2}V_2$，因此$k_n y_n \in \frac{1}{2}V_2$。因此，$\exp(h y_n) \in H$代表$h$、整数和$0 \leq |h| \leq |k_n|$（如$|h|$上的归纳所示）。然后
$$
\exp(\lambda y) = \lim_{n \to \infty} \exp(\lambda \lambda_n^{-1}y_n) = \lim_{n \to \infty} (\exp((\lambda - k_n \lambda_n)\lambda_n^{-1}y_n) \exp(k_n y_n))
= \lim_{n \to \infty} \exp k_n y_n \in H.
$$

因此，映射$f : \lambda \mapsto \exp \lambda y$，其中$\lambda y \in \frac{1}{4}V_2$，在$H$和$(T_0f)(1) = y$中取其值。因此$y \in \mathfrak{h}$，这是荒谬的。因此，在$\mathbf{R}$的情况下，定理成立。

如果 $G$ 不被假定为有限维 (习题 12)，则定理 2 不再成立。

#### 推论 1 {#lie-iii-s8-thm-2-cor-1 .statement tag=0AI9}

*令$G'$为局部紧致群，$G$为$\mathbf{R}$（或$\mathbf{Q}_p$）上的有限维李群，以及$f$为$G'$到$G$的连续态射。如果 $f$ 的核是离散的，则 $G'$ 是有限维实数（分别为 $p$-adic）李群。*

$G'$中存在$e$的紧邻域$V$，使得$f|V$是$V$到$G$的紧子空间的同胚。如果$U$是$G$中$e$的足够小的开邻域，定理2的假设满足$H = f(V) \cap U$。因此$H$是$G$的谎言子群萌芽。令$W$为$f|V$下$H$的逆像。那么$W$就是$G'$中$e$的邻域。让 $W$ 得到从 $H$ 到 $(f|W)^{-1}$ 传输的解析流形结构。对于所有$z \in G'$，$G$到$G$的映射$x \mapsto f(z)x f(z)^{-1}$是解析的；因此，$W$中存在$e$的开邻域$W'$，使得$W'$到$W$的映射$x' \mapsto zx'z^{-1}$是解析的。到§ 1, no. 9的命题 18，$G'$李群结构上存在诱导，其中诱导位于$e$的足够小的开邻域上，与$W$相同的解析结构，因此相同拓扑作为$G'$ 上的初始拓扑。

#### 推论 2 {#lie-iii-s8-thm-2-cor-2 .statement tag=0AIA}

*设$G$是$K$上的有限维李群，$G$的$H$子群，$V$在$G$和$(M_i)_{i \in I}$中的$e$的开邻域分析流形超过$K$的家庭；对于所有$i \in I$，让$f_i$是$V$到$M_i$的$K$解析映射，这样*

$$
H \cap V = \{ x \in V \mid f_i(x) = f_i(e) \text{ for all } i \in I \}.
$$

(i) *如果 $K = \mathbf{C}$，$H$ 是子群的$G$。*
(ii) *如果$K$是$\mathbf{Q}_p$的有限扩张且$I$是有限的，则$H$是$G$的谎言子群。*

(i) 假设$K = \mathbf{C}$。我们将$G$视为实李群。那么 $H$ 是 $G$ (定理 2) 的真谎言子群。让$a \in L(H)$。 $\mathbf{C}$ 中存在$0$ 的连通开邻域 $W$，使得$\exp \lambda a \in V$ 对于所有$\lambda \in W$。让$i \in I$。那么$f_i(\exp \lambda a) = f_i(e)$如果$\lambda \in \mathbf{R} \cap W$。因此 $f_i(\exp \lambda a) = f_i(e)$ if $\lambda \in W$ 通过解析延拓。因此，$\exp \lambda a \in H$适用于$\lambda \in W$，因此$\mu a \in L(H)$适用于所有$\mu \in \mathbf{C}$。因此 $H$ 是复数李群 $G$ (§ 4, no. 2, 命题 2) 的谎言子群。

(ii) 假设$K$是$\mathbf{Q}_p$的有限扩张。我们将$G$视为李群超过$\mathbf{Q}_p$。它是有限维的，并且定理 2 意味着 $H$ 是 $G$ 的 $p$ 进数谎言子群。由于$I$是有限的，$\prod_{i \in I} M_i$是流形，并且可以假设族$(f_i)$约化到单个映射$f$。让$a \in L(G)$。令$\phi$为$G$的指数映射。那么$f(\phi(\lambda a)) = f(e)$对于$\lambda \in \mathbf{Q}_p$和$|\lambda|$足够小。由于$f$是K解析的，因此$f(\phi(\lambda a)) = f(e)$对于$\lambda \in K$和$|\lambda|$足够小。因此，$\phi(\lambda a) \in H$对于$\lambda \in K$和$|\lambda|$足够小，因此$\mu a \in L(H)$对于所有$\mu \in K$。 证明如 (i) 所示完成。

如果我们忽略假设 I 是有限的，则推论 2 (ii) 不再成立。

### 习题 {#lie-iii-s8-exercises}

参见[习题为 § 8](exercises/s8/)。
