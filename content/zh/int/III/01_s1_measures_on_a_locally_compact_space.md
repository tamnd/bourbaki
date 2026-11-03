---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 1
section_title: Measures on a locally compact space
lang: zh
source: int-i-vi
pdf_pages: 0046-0068, 0100-0104
extraction: ocr
subsections:
    - "no": 1
      title: Continuous functions with compact support
      page: 0
      pdf_page: 46
    - "no": 2
      title: Approximation properties
      page: 4
      pdf_page: 49
    - "no": 3
      title: Definition of a measure
      page: 7
      pdf_page: 52
    - "no": 4
      title: Product of a measure by a continuous function
      page: 10
      pdf_page: 55
    - "no": 5
      title: Real measures. Positive measures
      page: 11
      pdf_page: 56
    - "no": 6
      title: Absolute value of a complex measure
      page: 13
      pdf_page: 58
    - "no": 7
      title: Definition of a measure by extension
      page: 15
      pdf_page: 60
    - "no": 8
      title: Bounded measures
      page: 16
      pdf_page: 61
    - "no": 9
      title: Vague topology on the space of measures
      page: 18
      pdf_page: 63
    - "no": 10
      title: Compact convergence in $\mathscr{M}(X; \mathbf{C})$
      page: 21
      pdf_page: 66
statements: 41
exercises: 18
content_sha256: de2686a0d66f63a87cdd58e4f3c577343668240caccccedc1b39443420bde957
translated_from: content/en/int/III/01_s1_measures_on_a_locally_compact_space.md
translation_method: google
source_content_sha256: a5649ad91c991534fecdc842feb81de5c325d32e755f63251c2a1e0724811493
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: df89c55a2777785ad9b9bd9837a1afea5c7b7a5cca3c7baf1e4ee4c973fe55d4
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 1。局部紧凑的措施空间

### 1. 连续函数带紧凑支撑

#### 定义 1 {#int-iii-s1-def-1 .statement tag=08L4}

— 令X为拓扑空间，令E为$\mathbf{R}$上的$\overline{\mathbf{R}}$或向量空间，并令f为E中X的映射。最小的在X中闭合集合S，使得$X - S$上的$f(x) = 0$（在其他字中，所有$x \in X$的集合在X中的闭包，使得$f(x) \neq 0$）称为f的支持度，记为Supp(f)。

令 X 为局部紧致空间，E 为$\mathbf{R}$ 或 $\mathbf{C}$ 上的拓扑向量空间；回想一下，$\mathscr{C}(X;E)$表示X的连续映射到E中的向量空间；当$E = \mathbf{R}$或$E = \mathbf{C}$时，如果不造成混淆，我们将在记号中省略E的提及。我们用紧支撑连续映射形成的$\mathscr{C}(X;E)$中的$\mathscr{K}(X;E)$子空间来表示；对于 X 的每个子集 A，我们用映射 f 形成的$\mathscr{C}(X;E)$（或$\mathscr{K}(X;E)$）的$\mathscr{C}(X,A;E)$（或$\mathscr{K}(X,A;E)$）子空间表示，这样$\operatorname{Supp}(f) \subset A$。如果$E = \mathbf{R}$或$E = \mathbf{C}$，我们写为$\mathscr{K}(X)$（分别为$\mathscr{K}(X,A)$），而不是$\mathscr{K}(X;\mathbf{R})$或$\mathscr{K}(X;\mathbf{C})$（分别为$\mathscr{K}(X,A;\mathbf{R})$或$\mathscr{K}(X,A;\mathbf{C})$），前提是不会导致混淆；我们用$\mathscr{K}_+(X)$表示由函数$\geq 0$和$\mathscr{K}(X;\mathbf{R})$形成的尖凸圆锥体。

对于X的每个紧凑子集 K，空间$\mathscr{K}(X,K;E)$可以用连续函数$\mathscr{C}(K;E)$的空间子空间（即，K的连续映射子空间到E中来识别） 零在 K 的边界$^1$）。当$\mathscr{C}(K;E)$配备K中一致收敛的拓扑时，$\mathscr{K}(X,K;E)$是$\mathscr{C}(K;E)$的闭子空间。特别是，如果 E 是 Fréchet 空间（分别是 Banach 空间），那么 $\mathscr{K}(X,K;E)$ 也是，因为如果 E 的拓扑由半范数 $p_n$（分别是范数 $x \mapsto \|x\|$）定义，则定义了$\mathscr{K}(X,K;E)$的拓扑

（1）原文为frontière，又译为“边疆”（GT，I, §1, No. 6，Def.11）。

由半范数$f \mapsto \sup_{x \in K} p_n(f(x))$（分别为范数$f \mapsto \sup_{x \in K} \|f(x)\|$，表示为$\|f\|$）。

空间$\mathscr{K}(X; E)$是子空间$\mathscr{K}(X, K; E)$的递增有向族并，其中$K$运行于$X$的紧致子集的集合；此外，如果$K_1 \subset K_2$是$X$的两个紧凑子集，则典范嵌入$\mathscr{K}(X, K_1; E) \to \mathscr{K}(X, K_2; E)$对于上面定义的拓扑是连续的。如果$E$是*局部凸*，则可以在$\mathscr{K}(X, K; E)$（TVS，II, §4, No. 4）的局部凸拓扑的*直极限*² $\mathscr{K}(X; E)$上定义；与除非相反，当我们将$\mathscr{K}(X; E)$视为拓扑向量空间时，这将始终是拓扑的问题。

#### 命题 1 {#int-iii-s1-prop-1 .statement tag=08L5}

*令$X$为局部紧致空间，$E$为Hausdorff局部凸空间。*

(i) *局部凸空间 $\mathscr{K}(X; E)$ 是 Hausdorff。对于$X$的每个紧致子集$K$，由$\mathscr{K}(X; E)$的紧致在$\mathscr{K}(X, K; E)$上诱导的拓扑是在$K$中一致收敛的拓扑，并且每个子空间$\mathscr{K}(X, K; E)$在$\mathscr{K}(X; E)$中都是封闭的。*

(ii) *如果$E$是局部凸空间$E_i$($1 \leq i \leq n$)的有限数的乘积，则映射$f \mapsto (\mathrm{pr}_i \circ f)$是空间$\mathscr{K}(X; E)$的同构到乘积空间$\prod_{1 \leq i \leq n} \mathscr{K}(X; E_i)$.*

(iii) *如果$X$是局部紧凑空间的族$(X_\lambda)_{\lambda \in L}$的和，则映射$f \mapsto (f|X_\lambda)_{\lambda \in L}$是拓扑直和上空间$\mathscr{K}(X; E)$的同构家庭空间$(\mathscr{K}(X_\lambda; E))_{\lambda \in L}$.*

(i) 请注意，在 $\mathscr{K}(X; E)$ 上，$X$ 一致收敛的拓扑与 $\mathscr{K}(X; E)$ 的向量空间结构兼容，因为对于每个$f \in \mathscr{K}(X; E)$，具有（紧凑）支持$S$、集合 $f(X) = f(S) \cup \{0\}$ 是紧致的，因此有界于 $E$（TVS，III, §3, No. 1，命题 1）。由于这个拓扑$\mathscr{T}_0$是局部凸的，诱导在$K$均匀收敛的每个$\mathscr{K}(X, K; E)$拓扑上，直极限拓扑$\mathscr{T}$在$\mathscr{K}(X; E)$上也是如此（TVS， II, §4, No. 4,*注*);此外，$\mathscr{T}$比$\mathscr{T}_0$是更细，并且$\mathscr{T}_0$是Hausdorff，因此$\mathscr{T}$是Hausdorff。最后，假设函数$f \in \mathscr{K}(X; E)$属于到$\mathscr{K}(X, K; E)$的闭包；到定义，存在$X$的紧子集$K' \supset K$，使得$f \in \mathscr{K}(X, K'; E)$。综上所述，$f$属于到空间$\mathscr{K}(X, K'; E)$中的$\mathscr{K}(X, K; E)$关闭，因此属于到$\mathscr{K}(X, K; E)$。

(ii) 直极限（TVS，II, §4, No. 4，命题 5）中的连续性准则立即表明映射 $f \mapsto (\mathrm{pr}_i \circ f)$ 是连续的，并且逆矩阵映射也是如此（对于后者，只需注意，如果对于每个函数 $f_i \in \mathscr{K}(X; E_i)$， 1 表示 $f'_i$ 映射

² *极限感性*，在S、A、GT中翻译为“直极限”。

将X转化为E，使得$\mathrm{pr}_i \circ f'_i = f_i$和$\mathrm{pr}_j \circ f'_i = 0$对应于$j \neq i$，则映射$f_i \mapsto f'_i$中的每一个都是连续的）。

(iii) X 的每个紧致子集 K 仅与 $(X_\lambda)_{\lambda \in L}$ 的有限子族 $(X_\lambda)_{\lambda \in H}$ 的 $X_\lambda$ 相交，如果集合 $K_\lambda = K \cap X_\lambda$ 与 $\lambda \in H$、映射相交，则为直接的 $f \mapsto (f|X_\lambda)_{\lambda \in H}$ 是 $\mathscr{K}(X, K; E)$ 的同构到$\prod_{\lambda \in H} \mathscr{K}(X_\lambda, K_\lambda; E)$。相反，对于每个函数$f_\lambda \in \mathscr{K}(X_\lambda; E)$，令$f''_\lambda$为X的映射进入E，使得$f''_\lambda|X_\lambda = f_\lambda$和$f''_\lambda|X_\mu = 0$对于$\mu \neq \lambda$； $\mathscr{K}(X_\lambda; E)$到$\mathscr{K}(X; E)$的映射$f_\lambda \mapsto f''_\lambda$连续就是直接的。 断言 (iii) 由注和直极限中的连续性标准得出（TVS，II, §4, No. 4，第 5 条）。

#### 命题 2 {#int-iii-s1-prop-2 .statement tag=08L6}

— *令 X 为局部紧致空间，E 为 Hausdorff 局部凸空间。*

(i) *如果 E 是 Fréchet 空间，则空间 $\mathscr{K}(X; E)$ 被桶装。*

(ii) *如果 X 是仿紧的，那么对于 $\mathscr{K}(X; E)$ 中的每个有界集合 B，都存在 X 的紧子集 K，使得 $B \subset \mathscr{K}(X, K; E)$。*

假设 E 是 Fréchet 空间。然后，对于 X 的每个紧凑子集 K，$\mathscr{K}(X, K; E)$ 是 Fréchet 空间，因此是桶装的，并且我们知道桶装空间的直极限是桶装的（TVS，III, §4, No. 1，第 3 条的 Cor.3），从而 (i)。

如果 X 是仿紧的，则知道（GT，I, §9, No. 10，Th.5）X 是和的$(X_\lambda)_{\lambda \in L}$ 局部紧致空间，可在无穷大处计数；因此（命题1，(iii)），$\mathscr{K}(X; E)$是子空间$\mathscr{K}(X_\lambda; E)$（$\lambda \in L$）族的*拓扑直和*。凭借拓扑直和中有界集合的刻画（TVS，III, §1, No. 4，命题 5），$\mathscr{K}(X; E)$ 中的每个有界集合都包含在子空间的*有限* 数的和中$\mathscr{K}(X_\lambda; E)$，并且足以证明$\mathscr{K}(X_\lambda; E)$中的每个有界集合都包含在子空间$\mathscr{K}(X_\lambda, K_\lambda; E)$中，并且$K_\lambda$紧凑在$X_\lambda$中。因此，我们被简化为X在无穷大处可数的情况，在其他字是相对紧开的集合$U_n$的序列的并，使得$\overline{U}_n \subset U_{n+1}$（GT，I, §9, No. 9，命题15）。但$\mathscr{K}(X; E)$是空间$\mathscr{K}(X, \overline{U}_n; E)$、从而断言（ii）的序列的*严格*直极限（TVS，III, §1, No. 4，第6条）。

We shall say that a subset H of $\mathscr{K}(X; E)$ is *strictly compact* if it is compact and if there exists a compact subset K of X such that $H \subset \mathscr{K}(X, K; E)$. 从命题 2 可以立即得出，如果 X 是一个 *paracompact* 局部紧致空间并且如果 E 是 Hausdorff，那么 *$\mathscr{K}(X; E)$ 中的每个紧集* 都是 *严格紧致*。 可以给出局部紧致的例

3 *Dénombrable à l'infini*，也翻译为“σ-紧凑”（GT，I, §9, No. 9，Def.5）。

空间 $X$（不是仿紧致），使得 $\mathscr{K}(X; \mathbf{R})$ 中存在集合，它们是*紧致但不是严格紧致*（习题 3 和 4）。

我们记得，根据阿斯科利的定理（GT，X, §2, No. 5，Th.2的Cor.3），$\mathscr{K}(X, K; E)$中包含的$\mathscr{K}(X; E)$的严格紧致子集$H$具有以下条件特征：$1^\circ$是封闭的； $2^\circ$ 等连续；对于每个$x \in K$，$3^\circ$，集合$H(x)$在$E$中相对紧凑。

#### 推论 {#int-iii-s1-n1-cor-1 .statement tag=08L7}

*令 $X$ 为拟紧致、局部紧致空间；如果 $E$ 是准完备局部凸空间，则空间 $\mathscr{K}(X; E)$ 是准完备的。*

凭借命题 2，(ii)，注意到对于$X$的每个紧致子集$K$，$\mathscr{K}(X, K; E)$是$C(K; E)$的封闭子空间，这是准完备的，因为$C(K; E)$的每个有界子集包含函数在 $E$ 的同一有界子集中取值。

### 2. 近似性质

#### 引理 1 {#int-iii-s1-lem-1 .statement tag=08L8}

*令$X$为局部紧致空间，$K$为$X$的紧致子集，$(V_k)_{1 \leq k \leq n}$为$X$的开集合对$K$的有限覆盖。那么，$X$存在$n$连续的映射$f_k$进入$[0, 1]$，使得$f_k$的支持度包含在$V_k$中，对于$1 \leq k \leq n$，$\sum_{k=1}^n f_k(x) \leq 1$对于所有$x \in X$， $\sum_{k=1}^n f_k(x) = 1$ 对于所有$x \in K$。

例如，令 $X'$ 为在无穷大 $\omega$ 处邻接 $X$ 点所获得的紧空间（GT，I, §9, No. 8，Th. 4）； 集合 $V_0 = X' - K$ 和 $V_k$ ($1 \leq k \leq n$) 形式 $X'$ 的开放覆盖物。令$(f_k)_{0 \leq k \leq n}$是单位元的连续划分，从属于$X'$的覆盖（GT，IX, §4, No. 3，命题3）； 函数$f_k$与指标$k \geq 1$满足条件共引理。

#### 引理 2 {#int-iii-s1-lem-2 .statement tag=08L9}

*令$X$为局部紧致空间，$K$为$X$的紧致子集，$E$为局部凸空间，$q$为$E$上的连续半范数，$\Phi$为$X$的映射等连续集合进入$E$，其支撑包含在$K$中。那么，对于每个 $\varepsilon > 0$，在 $X$ 上都存在一个连续的划分单位元 $(\varphi_j)_{0 \leq j \leq n}$，具有以下属性：
(i) $\operatorname{Supp}(\varphi_j) \subset K$ 为 $1 \leq j \leq n$。
(ii) *如果，对于 $1 \leq j \leq n$，$x_j$ 是 $\operatorname{Supp}(\varphi_j)$ 中的任意点，那么，对于每个函数 $f \in \Phi$ 和每个 $x \in X$，
$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x) f(x_j)\right) \leq \varepsilon.
$$*

对于$K$边界的每一个$y$属于，对于所有$f \in \Phi$，都有$f(y) = 0$，因此$X$中存在$y$的开邻域$V_y$，这样，对于每个$z \in V_y$和每个$f \in \Phi$，都有一个$q(f(z)) \leq \varepsilon/2$。令$K'$为$K$的点的集合，而不是属于到任何$V_y$，因为$y$越过$K$的边界； $K'$结构紧凑，包含在$K$的内部。 集合 $\Phi$ 在 $K$ 中一致等连续；因此，在$K$包含的$X$中，存在$K'$由……组成的开集合的有限开覆盖$(U_j)_{1 \leq j \leq n}$，使得对于同一$U_j$的点$x, y$的每个对，有一个每 $f \in \Phi$ $q(f(x) - f(y)) \leq \varepsilon/2$。到引理 1，存在 $X$ 的 $n$ 连续映射 $\varphi_j$ 到 $[0, 1]$ ($1 \leq j \leq n$) 使得 $\operatorname{Supp}(\varphi_j) \subset U_j$ 并且使得
$$
\sum_{j=1}^n \varphi_j(x) \leq 1 \text{ on } X \text{ and } \sum_{j=1}^n \varphi_j(x) = 1 \text{ on } K'.
$$
对于 $x_j \in \operatorname{Supp}(\varphi_j)$ ($1 \leq j \leq n$) 和 $f \in \Phi$，因此对于所有 $x \in U_j$，我们有，
$$
q(f(x)\varphi_j(x) - f(x_j)\varphi_j(x)) = \varphi_j(x)q(f(x) - f(x_j)) \leq \frac{\varepsilon}{2}\varphi_j(x),
$$
如果 $x \notin U_j$ 从那时起 $\varphi_j(x) = 0$，则此关系仍然为真。根据加法，我们推断对于每个$x \in X$，
$$
q\left(f(x)(1 - \varphi_0(x)) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \frac{\varepsilon}{2}(1 - \varphi_0(x)),
$$
其中$\varphi_0 = 1 - \sum_{j=1}^n \varphi_j$； 从而 (1) 为$x \in K'$，从那时起$\varphi_0(x) = 0$；
(1) 也适用于$x \notin K$，那么第一个成员就是零。最后，对于$x \in K - K'$，我们有$q(f(x)\varphi_0(x)) \leq \varepsilon/2$乘定义等于$K'$，因此在这种情况下，关系和(2)再次暗示(1)。

设$X$为局部紧致空间；对于每个 Banach 空间 $E$（实数或复数），我们用 $\mathscr{C}^b(X; E)$ 向量空间表示$X$ 的连续且有界映射到 $E$；我们知道$X$中一致收敛的拓扑与$\mathscr{C}^b(X; E)$的向量空间结构（实数，复数）相容的，并且它由范数定义
$$
||f|| = \sup_{x \in X} ||f(x)||.
$$
此外，如此定义的范数空间是Banach空间（GT、X, §3, No. 2和No. 1，Prop.2的Cor.2）；由这个$\mathscr{K}(X; E)$上的范数定义的拓扑（在$X$中一致收敛的其他字、拓扑）比No. 1中定义的$\mathscr{K}(X; E)$上的直极限拓扑更粗糙。

#### 命题 3 {#int-iii-s1-prop-3 .statement tag=08LA}

— 令 $X$ 为局部紧致空间，$X'$ 通过在无穷远 $\omega$ 邻接 $X$ 点获得紧致空间 (GT, I, §9, No. 8,

Th。 4)，E a Banach 空间。范数空间$C^b(X;E)$中$\mathscr{K}(X;E)$的闭包是X上连续函数的向量空间，其中值在E中并在点$\omega$趋于0。

令$\mathscr{K}(X;E)$闭包中的$f \in C^b(X;E)$为函数；对于每个$\varepsilon > 0$，都存在函数$g \in \mathscr{K}(X;E)$，使得$\|f(x) - g(x)\| \leq \varepsilon$对于所有$x \in X$；如果K是g的支持，则对于所有$x \in \mathbf{C}K$，$\|f(x)\| \leq \varepsilon$，因此$f(x)$趋于0，而$x$趋于$\omega$。相反，如果 f 有这个性质，那么对于每个 $\varepsilon > 0$，都存在紧集 $K \subset X$，这样对于所有 $x \in \mathbf{C}K$ 都有 $\|f(x)\| \leq \varepsilon$。到引理 1 时，存在 X 到 $[0,1]$ 的连续映射 h，具有紧支撑，等于 K 上的 1；然后$\|f(x)h(x)\| \leq \varepsilon$在$\mathbf{C}K$上，$f(x) = f(x)h(x)$在K上；由于$fh$具有紧凑的支持，并且$\|f(x) - f(x)h(x)\| \leq 2\varepsilon$对于所有$x \in X$，命题被证明。

我们用$C^b(X;E)$的$C^0(X;E)$子空间来表示，函数在$\omega$无穷大点处趋向于零；因此，这是规范的空间$\mathscr{K}(X;E)$的完成。

#### 命题 4 {#int-iii-s1-prop-4 .statement tag=08LB}

— 令 X 为局部紧致空间，E 为局部凸空间；那么，对于紧凑收敛的拓扑，空间$\mathscr{K}(X;E)$在$C(X;E)$中是稠密的。

对于每一个紧集$K \subset X$，在K上都存在函数$h \in \mathscr{K}(X;\mathbf{R})$等于1，引理1；对于每个函数$f \in C(X;E)$函数$hf$，其中属于到$\mathscr{K}(X;E)$，都等于K上的f，从而我们的断言。

#### 命题 5 {#int-iii-s1-prop-5 .statement tag=08LC}

— 令 X 为局部紧致空间，E 为实数（或复数）局部凸空间。 对于X的每个紧子集K，向量空间$\mathscr{K}(X,K;\mathbf{R}) \otimes_{\mathbf{R}} E$（分别为$\mathscr{K}(X,K;\mathbf{C}) \otimes_{\mathbf{C}} E$）（用X到E，cf.A，II, §7, No. 7，Prop.15的Cor.的一组映射来标识）在$\mathscr{K}(X,K;E)$中是稠密的；向量空间 $\mathscr{K}(X;\mathbf{R}) \otimes_{\mathbf{R}} E$（或 $\mathscr{K}(X;\mathbf{C}) \otimes_{\mathbf{C}} E$）在 $\mathscr{K}(X;E)$ 中是稠密的。

由于第二个断言是第一个明显的推论，因此足以证明后者。我们应用引理 2，并将$\Phi$减少为$\mathscr{K}(X,K;E)$的单个元素$f$；那么，对于每个 $x \in X$，

$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \varepsilon,
$$

其中 $\varphi_j$ 属于至 $\mathscr{K}(X,K;\mathbf{R})$；由于映射 $x \mapsto \sum_{j=1}^n \varphi_j(x)f(x_j)$ 可以与元素 $\sum_{j=1}^n \varphi_j \otimes f(x_j)$ 进行规范地识别，这通过 $\mathscr{K}(X,K;E)$ 的拓扑定义证明了命题。

### 3. 定义度量单位

#### 定义 2 {#int-iii-s1-def-2 .statement tag=08LD}

— *在* $\mathscr{K}(X; \mathbf{C})$上连续的线性形式，*X局部紧凑的空间*，*称为在X*上的测度*（或*复杂测度*）。

如果 $\mu$ 是局部紧凑空间 $X$ 上的测度，则函数 $f \in \mathscr{K}(X; \mathbf{C})$ 测度的值称为 *f 关于* $\mu$ 的积分；除一般的记号、$\mu(f)$、$\langle f, \mu \rangle$外，还用记号、$\int f d\mu$、$\int f \mu$、$\int f(x) d\mu(x)$、$\int f(x) \mu(x)$来表示；关于字母$x$的使用，参见S，I, §1, No. 1。

根据直极限中的连续性标准（TVS，II, §4, No. 4，第 5 条），说 $\mu$ 是$X$ 上的测度意味着 $\mu$ 是 $\mathscr{K}(X; \mathbf{C})$ 满足上的线性形式以下条件：对于$X$的每个紧凑子集$K$，都存在数$M_K$，这样，对于每个函数$f \in \mathscr{K}(X; \mathbf{C})$*其支持包含在*$K$中，

$$
| \mu(f) | \leq M_K \cdot \| f \| \quad \text{(where } \| f \| = \sup_{x \in X} |f(x)| ).
$$

更一般地说：

#### 命题 6 {#int-iii-s1-prop-6 .statement tag=08LE}

— *令 X 为局部紧凑空间，($K_\alpha$) X 的紧凑子集系列，其内部$\overset{\circ}{K}_\alpha$ 形式 X 的开放覆盖物。为了使$\mathscr{K}(X; \mathbf{C})$上的线性形式$\mu$成为X上的测度，对于每个$\alpha$，存在数$M_\alpha$使得*

$$
| \mu(f) | \leq M_\alpha \cdot \| f \|
$$

*每函数* $f \in \mathscr{K}(X, K_\alpha; \mathbf{C})$。

条件显然是必要的，只要证明对于$X$的每个紧致子集$K$，(5)蕴涵(4)即可。现在，$K$被开集合$\overset{\circ}{K}_{\alpha_i}$（$1 \leq i \leq n$）的有限数覆盖； No. 2到$K$和$\overset{\circ}{K}_{\alpha_i}$中的应用引理 1，在$X$上存在连续的函数$g_i \geq 0$，使得$\operatorname{Supp}(g_i) \subset K_{\alpha_i}$，$0 \leq \sum_{i=1}^n g_i(x) \leq 1$对于所有$x \in X$ 和$\sum_{i=1}^n g_i(x) = 1$ 对应$x \in K$。因此，对于每个函数$f \in \mathscr{K}(X, K; \mathbf{C})$，我们可以写成$f = \sum_{i=1}^n f g_i$，我们有$f g_i \in \mathscr{K}(X, K_{\alpha_i}; \mathbf{C})$和$\| f g_i \| \leq \| f \|$；如果$M_K = \sum_{i=1}^n M_{\alpha_i}$，则我们有关系 (4)。

我们用 $\mathscr{M}(X; \mathbf{C})$ 表示，或者如果不会造成混淆，则简单地用 $\mathscr{M}(X)$ 表示，$X$ 上的措施向量空间，在其他字中，表示$\mathscr{K}(X; \mathbf{C})$ 的*对偶*。

人们知道，对于$\mathscr{K}(X;\mathbf{C})$的*有界*子集的每个集合$\mathscr{S}$，在$\mathscr{M}(X;\mathbf{C})$上定义了$\mathscr{S}$拓扑，该拓扑是局部凸的（TVS，III, §3, No. 1，Prop.1的Cor.）。我们用$\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$或$\mathscr{M}_{\mathscr{S}}(X)$表示通过为$\mathscr{M}(X;\mathbf{C})$配备$\mathscr{S}$拓扑而获得的拓扑向量空间。

#### 命题 7 {#int-iii-s1-prop-7 .statement tag=08LF}

*对于$\mathscr{K}(X;\mathbf{C})$的有界子集的每个集合$\mathscr{S}$（覆盖$\mathscr{K}(X;\mathbf{C})$），空间$\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$是豪斯多夫（Hausdorff）且准完备。*

这是由于 $\mathscr{K}(X;\mathbf{C})$ 是桶装的（TVS、III, §4, No. 2、Th.1 的 Cor.4）。

*例措施。* — I。 *原子措施。*令X为X的局部紧凑空间、$a$点；对于X 包含 $a$ 的每个紧凑子集 K，将$\mathscr{K}(X;\mathbf{C})$的映射$f\mapsto f(a)$转化为$\mathbf{C}$显然满足条件 (4) 和$M_K=1$，因此是X，记作$\varepsilon_a$；它被称为点$a$的*狄拉克测度*，或由放置在点$a$的*单位质量定义的测度。*

更一般地，令 $\alpha$ 为 X 的映射到 $\mathbf{C}$，这样，对于 X 的每个紧致子集 K，
$$
\sum_{x\in K}|\alpha(x)|<+\infty.
$$
然后，对于每个函数 $f\in\mathscr{K}(X,K;\mathbf{C})$，和
$$
\mu(f)=\sum_{x\in X}\alpha(x)f(x)
$$
被定义为，等于
$$
\sum_{x\in K}\alpha(x)f(x);
$$
很明显，$\mu$ 是 $\mathscr{K}(X;\mathbf{C})$ 上的线性形式，并且对于 $f\in\mathscr{K}(X,K;\mathbf{C})$，
$$
|\mu(f)|\leq\left(\sum_{x\in K}|\alpha(x)|\right)\cdot\|f\|,
$$
其他字条件 (4) 满足。

如果 X 的映射 $\alpha$ 存在于 $\mathbf{C}$ 中，则 X 上的$\mu$ 被称为“原子”，使得
$$
\sum_{x\in K}|\alpha(x)|<+\infty
$$
对于X的每个紧凑子集 K，并且$\mu$等于上面定义的度量。如果 N 是 $x\in X$ 的集合，则$\alpha(x)\neq0$、条件强加于 $\alpha$ 意味着对于X 的每个紧凑子集 K，$K\cap N$ 是*可数的*。还有人说 $\mu$ 是由位于点* $x\in N$ 的*质量* $\alpha(x)$ *定义的。如果假设对于每个紧集 $K\subset X$，$N\cap K$ 是*有限的*，那么显然
$$
\sum_{x\in K}|\alpha(x)|<+\infty;
$$
说N是X的*封闭*和*离散*子空间是一样的，因为X的每个点都有一个紧邻域包含，只有N的点的有限数，反之，如果是这种情况，那么每个X的紧凑子集可以被有限的数这样的邻域覆盖。当 N 是封闭且离散的时，由函数 $\alpha$ 定义的每个原子测度，使得 $\mathbf C N$ 上的 $\alpha(x)=0$ 称为 X 上的离散测度（cf. §2, No. 5）。

### II。 *勒贝格测度。*对于每个函数$f\in\mathscr K(\mathbf R;\mathbf C)$，都存在一个$\mathbf R$的紧凑区间$[a,b]$，其中$f$是零。整的

$$
\mathrm I(f)=\int_{-\infty}^{+\infty}f(x)\,dx=\int_a^b f(x)\,dx
$$

因此被定义；此外，通过平均值的定理（FRV，II, §1, No. 5，命题6），我们有$|\mathrm I(f)|\leq(b-a)\|f\|$；这表明$f\mapsto\mathrm I(f)$是$\mathbf R$的测度，称为*勒贝格测度*。

对于 $\mathbf R$ 的每一个区间 J（有界或无界），类似地，我们将 J* 上的*勒贝格测度称为$f\mapsto\int_Jf(x)\,dx$、线性形式在 $\mathscr K(J;\mathbf C)$ 上的测度（该积分有意义，因为存在包含在 J 中的紧凑区间 $[a,b]$，其中 $f$ 是零）。

### III。设$g$是紧致区间$I\subset\mathbf R$到$\mathbf C$的连续映射，在I有连续导数。设$\Gamma=g(I)$，它是$\mathbf C$的紧致子空间； 映射

$$
f\mapsto\int_I f(g(t))g'(t)\,dt
$$

凭借平均值定理，将 $\mathscr C(\Gamma;\mathbf C)$ 转换为 $\mathbf C$ 是连续的线性形式，因此是 *对 $\Gamma$* 的复杂测度；相对于该度量的积分也写为$\int_\Gamma f(z)\,dz$，甚至虽然，它不仅取决于$\Gamma$，还取决于$g$。

#### 注 {#int-iii-s1-n3-rem-1 .statement tag=08LG}

在局部紧凑空间X定义上对X采取措施$\mu$（以及X的拓扑）结构$\mathscr S$。设$X_1$是第二个集合，$\varphi$是X到$X_1$的双射映射；与一般的定义（S、R、§8）一致，通过$\varphi$*运输*到X的$X_1$结构$\mathscr S$而获得结构$\mathscr S_1$，定义如下。 X的拓扑由$\varphi$运输到$X_1$； $\mathscr K(X_1;\mathbf C)$ 的函数则为函数 $f$，使得$f\circ\varphi$ 属于到$\mathscr K(X;\mathbf C)$，并且$X_1$ 上的测度$\mu_1$ 由$\mu_1(f)=\mu(f\circ\varphi)$ 定义。

特别是，结构$\mathscr S$的*自同构*是X的同胚$\sigma$自身，使得

$$
\mu(f)=\mu(f\circ\sigma)
$$

每函数 $f\in\mathscr K(X;\mathbf C)$；测度 $\mu$ 也被称为*在同胚*$\sigma$ 下不变。

#### 例 {#int-iii-s1-n3-exa-1 .statement tag=08LH}

$\mathbf{R}$ 的勒贝格测度在加法群 $\mathbf{R}$ 的每种翻译下都是不变的。事实上，对于每个函数$f \in \mathscr{K}(\mathbf{R}; \mathbf{C})$和每个实数$a$，我们有

$$
\int_{-\infty}^{+\infty} f(x + a)\, dx = \int_{-\infty}^{+\infty} f(t)\, dt
$$

通过变量变化公式 (FRV, II, §2, No. 1, 公式 (1))。对于推广，请参见第 1 章。 VII, §1, No. 2，周四。 1.

### 4. 连续函数的测量乘积

令$X$是局部紧凑的空间，$g$是$X$到$\mathbf{C}$的连续映射。显然，$f \mapsto gf$ 是 $\mathscr{K}(X; \mathbf{C})$ 的线性映射自身；让我们证明这个映射是连续的。事实上，对于$X$的每个紧凑子集$K$，以及每个函数$f \in \mathscr{K}(X, K; \mathbf{C})$，我们有$gf \in \mathscr{K}(X, K; \mathbf{C})$；此外，如果$b_K = \sup_{x \in K} |g(x)|$则$\|gf\| \leq b_K \|f\|$，从而我们的断言（TVS，II, §4, No. 4，提案5）。因此，该连续线性映射（TVS，II, §6, No. 4）的转置等于 $\mathscr{M}(X; \mathbf{C})$ 的线性映射自身，表示为 $\mu \mapsto g \cdot \mu$（或 $\mu \mapsto g\mu$，如果不会导致混淆）。如果 $\nu = g \cdot \mu$ 因此，对于每一个函数 $f \in \mathscr{K}(X; \mathbf{C})$，

$$
\langle f, \nu \rangle = \langle gf, \mu \rangle
$$

或再次

$$
\int f(x)\, d\nu(x) = \int f(x)g(x)\, d\mu(x)
$$

（缩写为形式$d\nu(x) = g(x)\, d\mu(x)$）。有人说，$g \cdot \mu$是函数$g$测量$\mu$的乘积，或者也是密度$g$相对于$\mu$的测量（cf.Ch.V, §5, No. 2，定义2）。如果$g_1, g_2$是$X$到$\mathbf{C}$的两个连续的映射，$\mu_1, \mu_2$是$X$上的两个小节，那么

$$
(g_1 + g_2) \cdot \mu = g_1 \cdot \mu + g_2 \cdot \mu, \quad g \cdot (\mu_1 + \mu_2) = g \cdot \mu_1 + g \cdot \mu_2,
$$
$$
(g_1 g_2) \cdot \mu = g_1 \cdot (g_2 \cdot \mu).
$$

此外，$1 \cdot \mu = \mu$（这里1表示常数函数在$X$上等于1）； 集合$\mathscr{M}(X; \mathbf{C})$，配备合成$(g, \mu) \mapsto g \cdot \mu$的外法则及其添加剂结构，因此模超过环$\mathscr{C}(X; \mathbf{C})$。

### 5. 切实措施。积极措施

设 X 为局部紧致空间。实数向量空间$\mathscr{K}(X; \mathbf{R})$是复数向量空间$\mathscr{K}(X; \mathbf{C})$底层实数向量空间的子空间；此外，映射$(f_1, f_2) \mapsto f_1 + i f_2$是乘积拓扑向量空间$\mathscr{K}(X; \mathbf{R}) \times \mathscr{K}(X; \mathbf{R})$到真实拓扑向量空间$\mathscr{K}(X; \mathbf{C})$的*同构*（No. 1，命题1）。

对于$\mu$到$\mathscr{K}(X; \mathbf{R})$的每个（复数）测度$\mu \in \mathscr{M}(X; \mathbf{C})$、限制$\mu_0$，是$\mathscr{K}(X; \mathbf{R})$到$\mathbf{C}$的连续$\mathbf{R}$线性映射；此外，这个限制确定$\mu$，因为如果$f = f_1 + i f_2$和$f_1, f_2$在$\mathscr{K}(X; \mathbf{R})$中，那么$\mu(f) = \mu_0(f_1) + i \mu_0(f_2)$。相反，令$\mu_0$是$\mathscr{K}(X; \mathbf{R})$到$\mathbf{C}$的连续$\mathbf{R}$线性映射；很明显映射

$$
f_1 + i f_2 \mapsto \mu_0(f_1) + i \mu_0(f_2)
$$

是 X 的（复杂）测度。因此，X上的每个测度都可以用其限制到$\mathscr{K}(X; \mathbf{R})$来标识。

令 $\mu$ 为X 的度量。对于每个函数$f \in \mathscr{K}(X; \mathbf{C})$，我们可以调用$\mu$的*共轭测度*由$\overline{\mu}(f) = \overline{\mu(\overline{f})}$定义的测度$\overline{\mu}$；因为，很明显$\overline{\mu}$是C线性形式，并且它在$\mathscr{K}(X; \mathbf{C})$上连续；显然 $\overline{\mu} = \mu$，并且对于 $\mathbf{C}$ 中的两个度量 $\mu, \nu$ 和两个标量 $\alpha, \beta$，

$$
(\alpha \mu + \beta \nu) = \overline{\alpha} \cdot \overline{\mu} + \overline{\beta} \cdot \overline{\nu}.
$$

更一般地，对于函数$g \in \mathscr{C}(X; \mathbf{C})$和X上的每个$\mu$小节，

$$
g \cdot \overline{\mu} = \overline{g} \cdot \overline{\mu},
$$

与定义 (No. 4) 中的直接的一样。

如果 $\overline{\mu} = \mu$，则 X 上的$\mu$ 被称为“真实”；由上可知，对于每个函数 $f \in \mathscr{K}(X; \mathbf{R})$，$\mu(f)$ 都是一个*实数* 数。如果用限制到 $\mathscr{K}(X; \mathbf{R})$ 来识别实测度，则可以说 X 上实测度的集合是实数局部凸空间 $\mathscr{K}(X; \mathbf{R})$ 的*对偶*；它是一个真正的向量空间，表示为$\mathscr{M}(X; \mathbf{R})$（或有时$\mathscr{M}(X)$，如果这不会引起任何混淆）。 $\mathbf{R}$ 上的勒贝格测度是一个“真实”测度，对于每个点 $a \in X$ 的狄拉克测度 $\varepsilon_a$ 也是如此。如果 $g \in \mathscr{C}(X; \mathbf{R})$ 且 $\mu$ 是实测度，则根据 (7) $g \cdot \mu$ 也是实测度。

令 $\mu$ 为 X 的（复数）测度。从前面的定义可以看出，措施$\mu_1 = (\mu + \overline{\mu})/2$和$\mu_2 = (\mu - \overline{\mu})/2i$是*真实的*；它们分别称为$\mu$的*实数部分*和*虚数部分*，分别用$\mathscr{R}\mu$和$\mathscr{I}\mu$表示；这些措施的另一个特点是，对于每函数 $f \in \mathscr{K}(X; \mathbf{R})$，

$$
\mu_1(f) = \mathscr{R}(\mu(f)) , \quad \mu_2(f) = \mathscr{I}(\mu(f)).
$$

显然
$$
\mu = \mu_1 + i \mu_2,\quad \overline{\mu} = \mu_1 - i \mu_2.
$$

具有紧凑支持的 $X$ 上的连续实值函数的空间 $\mathscr{K}(X; \mathbf{R})$ 显然是序关系 $f \leq g$ 的 *Riesz 空间*。我们可以说，如果$\mu(f) \geq 0$对于每个函数$f \geq 0$属于到$\mathscr{K}(X; \mathbf{R})$，则$X$上的实际测度$\mu$是“正”；因此，它是 Riesz 空间 $\mathscr{K}(X; \mathbf{R})$ 上的正线性形式（第 II, §2, No. 1，定义 1）。反之：

#### 定理 1 {#int-iii-s1-thm-1 .statement tag=08LI}

*Riesz 空间 $\mathscr{K}(X; \mathbf{R})$ 上的每个正值线性形式都是 $X$ 上的（正）实际度量。*

例如，令$\mu$为$\mathscr{K}(X; \mathbf{R})$上的正线性形式，并令$K$为$X$的紧凑子集。存在$X$到$[0, 1]$的连续映射$f_0$，具有紧支撑，使得$f_0(x) = 1$位于$K$上（No. 2，引理1）。对于每一个函数$g \in \mathscr{K}(X, K; \mathbf{R})$，我们就有$-\|g\|f_0 \leq g \leq \|g\|f_0$，因而$|\mu(g)| \leq \|g\| \cdot \mu(f_0)$，这证明了定理。

我们用 $\mathscr{M}_+(X)$ 表示 $X$ 上的正测量的尖凸锥体（或者，相当于相同的东西，Riesz 空间 $\mathscr{K}(X; \mathbf{R})$ 上的正线性形式锥体）。

#### 定理 2 {#int-iii-s1-thm-2 .statement tag=08LJ}

*局部紧凑空间 $X$ 上的每个实际测度都是两个正测度的差。*

鉴于定理 1 和 Ch. II, §2, No. 2，周四。 1，这一切都归结为证明，$X$ 上的实际测度 $\mu$ 是 Riesz 空间 $\mathscr{K}(X; \mathbf{R})$ 上的*相对有界* 线性形式。设$f$是$X$上的连续函数$\geq 0$，有紧支撑$K$； $\mathscr{K}(X; \mathbf{R})$中的关系$0 \leq g \leq f$意味着$\|g\| \leq \|f\|$并且$g$的支持包含在$K$中。到假设，存在数$M_K \geq 0$，使得每个函数$h \in \mathscr{K}(X, K; \mathbf{R})$都有$|\mu(h)| \leq M_K \cdot \|h\|$；因而$|\mu(g)| \leq M_K \cdot \|g\| \leq M_K \cdot \|f\|$，证明定理。

因而，$X$ 上的实际测度的空间 $\mathscr{M}(X; \mathbf{R})$ 与 Riesz 空间 $\mathscr{K}(X; \mathbf{R})$ 上相对有界的线性形式的空间相同；我们记得在$\mathscr{M}(X; \mathbf{R})$中，序关系$\mu \leq \nu$表示$\nu - \mu$是一个积极的措施，或者对于每个函数$f \in \mathscr{K}_+(X)$表示$\mu(f) \leq \nu(f)$。

#### 定理 3 {#int-iii-s1-thm-3 .statement tag=08LK}

*局部紧凑空间 $X$ 上的实际测量的空间 $\mathscr{M}(X; \mathbf{R})$ 是完全格序的。*

这是从第 1 章得出的。 II, §2, No. 2，Th。 1.

符合第 1 章记号。 II, §1，我们定义，对于$X$上的每一个*实际*测量$\mu$，

$$
\mu^+ = \sup(\mu, 0),\quad \mu^- = \sup(-\mu, 0),\quad |\mu| = \sup(\mu, -\mu);
$$

然后是$\mu = \mu^+ - \mu^-,\ |\mu| = \mu^+ + \mu^-$和$\inf(\mu^+, \mu^-) = 0$。此外，对于每个函数 $f \in \mathscr{K}_+(\mathrm{X})$，

$$
\int f\, d\mu^+ = \sup_{0 \leq g \leq f,\ g \in \mathscr{K}(\mathrm{X})} \int g\, d\mu
$$

和

$$
\int f\, d|\mu| = \sup_{|g| \leq f,\ g \in \mathscr{K}(\mathrm{X})} \int g\, d\mu,
$$

从而，特别是，

$$
\left| \int f\, d\mu \right| \leq \int |f|\, d|\mu|
$$

对于每个函数 $f \in \mathscr{K}(\mathrm{X}; \mathbf{R})$。

如果 $f \in \mathscr{K}(\mathrm{X}; \mathbf{C})$，则该不等式也成立；因为，将$f$乘以绝对值1的复数（这不会改变不等式的任一侧），可以假设$\int f\, d\mu \geq 0$。 然后

$$
\left| \int f\, d\mu \right| = \int f\, d\mu = \int (\Re f)\, d\mu \leq \int |\Re f|\, d|\mu| \leq \int |f|\, d|\mu|.
$$

### 6. 复测度的绝对值值

令 $\mu$ 为局部紧凑空间 $\mathrm{X}$ 上的复测度；对于每个函数 $f \in \mathscr{K}_+(\mathrm{X})$，正实数

$$
L(f) = \sup_{|g| \leq f,\ g \in \mathscr{K}(\mathrm{X}; \mathbf{C})} \left| \int g\, d\mu \right|
$$

是有限的，因为关系$|g| \leq f$意味着$\operatorname{Supp}(g) \subset \operatorname{Supp}(f)$和$\|g\| \leq \|f\|$，因此我们的断言是从No. 3的公式(4)得出的。让我们证明$L$只能以一种方式扩展到$\mathrm{X}$的正测度；鉴于No. 5，Th。 1 和 Ch. II, §2, No. 1，命题3，只要证明如果$f_1,\ f_2$是$\mathscr{K}_+(\mathrm{X})$中的两个函数，则$L(f_1 + f_2) = L(f_1) + L(f_2)$。现在，如果$|g_1| \leq f_1$和$|g_2| \leq f_2$，其中$g_1$和$g_2$是$\mathscr{K}(\mathrm{X}; \mathbf{C})$中的函数，对于绝对值1的任何复数$\zeta$，我们有$|g_1 + \zeta g_2| \leq f_1 + f_2$，因而

$$
|\mu(g_1 + \zeta g_2)| = |\mu(g_1) + \zeta \mu(g_2)| \leq L(f_1 + f_2).
$$

此外，我们可以假设$\zeta$这样选择
$$
|\mu(g_1) + \zeta \mu(g_2)| = |\mu(g_1)| + |\mu(g_2)|;
$$
由于$|\mu(g_i)|$任意接近$L(f_i)$（$i = 1, 2$），这证明了$L(f_1) + L(f_2) \leq L(f_1 + f_2)$。另一方面，考虑函数$g \in \mathscr{K}(X; \mathbf{C})$使得$|g| \leq f_1 + f_2$。 函数$g_i$在点处等于$g f_i/(f_1 + f_2)$，其中$f_1(x) + f_2(x) \neq 0$，并且在其他地方等于0（$i = 1, 2$），在X上连续，因为$f_i/(f_1 + f_2)$（$i = 1, 2$）在每个点处连续，其中$f_1(x) + f_2(x) \neq 0$，对于每个$x \in X$，我们有$|g_i(x)| \leq |g(x)|$，这证明了$g_i$在点的连续性，其中$f_1(x) + f_2(x) = 0$（$i = 1, 2$），因为在这些点我们也有$g(x) = 0$。显然 $|g_i| \leq f_i$ ($i = 1, 2$) 和 $g = g_1 + g_2$，因而
$$
|\mu(g)| \leq |\mu(g_1)| + |\mu(g_2)| \leq L(f_1) + L(f_2);
$$
由于 $|\mu(g)|$ 任意接近 $L(f_1 + f_2)$，我们有
$$
L(f_1 + f_2) \leq L(f_1) + L(f_2),
$$
这就完成了我们的断言中的证明。

当 $\mu$ 为实测度时，由公式 (9) 得出 $|\mu| \leq L$；另一方面，凭借No. 5的最后一个部分，如果$g \in \mathscr{K}(X; \mathbf{C})$和$|g| \leq f \in \mathscr{K}_+(X)$则$|\int g \, d\mu| \leq \int |g| \cdot d|\mu| \leq \int f \, d|\mu|$，因此通过定义$L \leq |\mu|$，在其他字$L = |\mu|$。

我们再次用$|\mu|$表示任何复杂测度$\mu$的正测度$L$，并且我们说$|\mu|$是$\mu$的绝对值。因而 $|\mu|$ 的定义可以写成
$$
|\mu|(f) = \sup_{|g| \leq f,\ g \in \mathscr{K}(X; \mathbf{C})} |\mu(g)|,
$$
因而，对于每函数 $g \in \mathscr{K}(X; \mathbf{C})$，
$$
\left| \int g \, d\mu \right| \leq \int |g| \, d|\mu|.
$$

很明显，对于$X$上的每个标量$\alpha \in \mathbf{C}$和每个测度$\mu$，
$$
|\alpha \mu| = |\alpha| \cdot |\mu|.
$$

另一方面，如果$\mu$和$\nu$是$X$上的两个度量，$f$是$\mathscr{K}_+(X)$中的函数，$g$是$\mathscr{K}(X; \mathbf{C})$中的函数，使得$|g| \leq f$，则
$$
\left| \int g \, d(\mu + \nu) \right| = \left| \int g \, d\mu + \int g \, d\nu \right| \leq \int f \, d|\mu| + \int f \, d|\nu|,
$$

从而

$$(15)$$
$$|\mu + \nu| \leq |\mu| + |\nu|.$$

对于相同的记号，关系 $|g| \leq f$ 和 $|\overline{g}| \leq f$ 是等价的，因此

$$(16)$$
$$|\overline{\mu}| = |\mu|.$$

由(14)、(15)、(16)可知

$$(17)$$
$$|\mathscr{R}\mu| \leq |\mu|,\quad |\mathscr{I}\mu| \leq |\mu|,\quad |\mu| \leq |\mathscr{R}\mu| + |\mathscr{I}\mu|.$$

#### 命题 8 {#int-iii-s1-prop-8 .statement tag=08LL}

*如果 $\mu$ 是 $X$ 的度量，那么对于每个函数 $h \in \mathscr{C}(X; \mathbf{C})$，*

$$(18)$$
$$|h \cdot \mu| \leq |h| \cdot |\mu|.$$

因为，如果$f \in \mathscr{K}_+(X)$且$g \in \mathscr{K}(X; \mathbf{C})$满足$|g| \leq f$，则根据(13)，$|\int gh d\mu| \leq \int |gh| d|\mu| \leq \int f|h| d|\mu|$，从而证明(18)。

### 7. 定义扩张

设$X$为局部紧致空间；如果$V$是$\mathscr{K}(X; \mathbf{C})$的*密集*线性子空间，很明显，$X$上的两个测度$\mu_1, \mu_2$和$V$上的重合是相等的，并且$V$上的每个线性形式连续由$\mathscr{K}(X; \mathbf{C})$引起的拓扑可以扩展到（仅以一种方式）到$X$上的测量。对于积极措施，一个方便的标准如下：

#### 命题 9 {#int-iii-s1-prop-9 .statement tag=08LM}

*令$V$为$\mathscr{K}(X; \mathbf{R})$的线性子空间，具有以下性质：
(P) 对于$X$的每个紧致子集$K$，存在函数$f \in V$使得$f \geq 0$并且对于所有$x \in K$存在$f(x) > 0$。
在这些条件下，$V$上由$\mathscr{K}(X; \mathbf{R})$（第II, §2, No. 1，定义1）引起的排序的每个正线性形式都可以扩展到$X$上的正测量（当$V$在$\mathscr{K}(X; \mathbf{R})$中密集时，这是唯一的）。
对于每个函数$f \in \mathscr{K}(X; \mathbf{R})$，在$K$的支持下，存在函数$g \in V$使得$f \leq g$；因为，$V$中存在函数$h \geq 0$，使得$h(x) > 0$对于所有$x \in K$； 设定$\alpha = \inf_{x \in K} h(x)$，因此我们有$\alpha > 0$和函数$g = (\alpha^{-1} \|f\|)h$满足要求。然后应用 Th 就足够了。 No. 5 的第 1 条和 TVS 的第 1 条，II, §3, No. 1。*

### 8. 有界措施

设 X 为局部紧致空间。由于由$\mathscr{C}^b(X; \mathbf{C})$的测量引起的$\mathscr{K}(X; \mathbf{C})$上的拓扑比$\mathscr{K}(X; \mathbf{C})$上的直极限拓扑更粗糙，因此X上的测量对于X中一致收敛的拓扑不一定是连续的。

#### 定义 3 {#int-iii-s1-def-3 .statement tag=08LN}

*如果局部紧凑空间 X 在 $\mathscr{K}(X; \mathbf{C})$ 上连续且一致收敛于拓扑，则称其为有界。*

同样的道理，存在一个有限的数 $M \geq 0$，对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$，

$$
|\mu(f)| \leq M \|f\|
$$

（其中 $\|f\|$ 由 No. 2 的公式 (3) 定义）。

因此，说$\mu$是有界测度意味着$\mu$属于是由$\|f\|$规范的空间$\mathscr{K}(X; \mathbf{C})$的对偶；我们将用 $\mathscr{M}^1(X; \mathbf{C})$ 来表示这个对偶（或者在不会导致混淆时简称为 $\mathscr{M}^1(X)$）。我们知道$\mathscr{M}^1(X; \mathbf{C})$配备了范数，$\|\mu\|$是数$M \geq 0$的最小的，其中不等式（19）对于每个函数$f \in \mathscr{K}(X; \mathbf{C})$都成立，或者再次，

$$
\|\mu\| = \sup_{\|f\| \leq 1,\ f \in \mathscr{K}(X; \mathbf{C})} |\mu(f)| .
$$

配备此范数，$\mathscr{M}^1(X; \mathbf{C})$ 被称为 Banach 空间（TVS，III, §3, No. 8，第 12 号提案的 Cor.2）。

公式 (20) 的$\|\mu\|$的定义可以扩展到X上的每个措施$\mu$，并且由于语言滥用，$\|\mu\|$再次被称为$\mu$的范数；对于 $\mu$ 有界，$\|\mu\|$ 是有限的是充分必要的。

如果 X 是紧致的，则 X 上的每个测度都是有界的。

#### 例 {#int-iii-s1-n8-exa-1 .statement tag=08LO}

— 1) 由单位质量在点 $a \in X$ 定义的测量$\varepsilon_a$ 有界，且$\|\varepsilon_a\| = 1$。

2) $\mathbf{R}$ 上的勒贝格测度无界；事实上，对于每个整数$n > 0$，都存在函数$f \in \mathscr{K}(\mathbf{R}; \mathbf{C})$，其中值在$[0, 1]$中并且在区间$[ -n, n ]$上等于1（No. 2，引理1）；因此 $\|f\| = 1$ 和

$$
\int_{-\infty}^{+\infty} f(x)\, dx \geq \int_{-n}^{n} f(x)\, dx = 2n ,
$$

证明不存在有限数 M 满足关系 (19).

3) 实直线$\mathbf{R}$、映射

$$
f \mapsto \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2}
$$

是一个有界测度，因为对于每个函数 $f \in \mathscr{H}(\mathbf{R}; \mathbf{C})$，

$$
\left| \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2} \right| \leq \|f\| \int_{-\infty}^{+\infty} \frac{dx}{1 + x^2} = \pi \cdot \|f\|.
$$

由于关系 $\|f\| \leq 1$ 和 $\|\overline{f}\| \leq 1$ 等价，由 (20) 得出

(21)
$$
\|\overline{\mu}\| = \|\mu\|
$$
对于 $X$ 上的每一个小节 $\mu$。

#### 命题 10 {#int-iii-s1-prop-10 .statement tag=08LP}

— *对于 $X$ 上的每个小节 $\mu$*，

(22)
$$
\|\mu\| = \sup_{0 \leq f \leq 1,\ f \in \mathscr{H}(X; \mathbf{R})} |\mu|(f).
$$

因为，考虑到公式 (12) 定义测度的绝对值，(22) 的第二个成员可以写成

$$
\sup_{0 \leq f \leq 1,\ f \in \mathscr{H}(X; \mathbf{R})} \left( \sup_{|g| \leq f,\ g \in \mathscr{H}(X; \mathbf{C})} |\mu(g)| \right) = \sup_{\|g\| \leq 1,\ g \in \mathscr{H}(X; \mathbf{C})} |\mu(g)|.
$$

#### 推论 1 {#int-iii-s1-prop-10-cor-1 .statement tag=08LQ}

— *对于$X$上的每个措施$\mu$，$\mu$和$|\mu|$的范数相等； $\mu$ 是有界的当且仅当 $|\mu|$ 是有界的。*

#### 推论 2 {#int-iii-s1-prop-10-cor-2 .statement tag=08LR}

— *对于紧凑型空间 $X$ 上的每个尺寸 $\mu$，*

(23)
$$
\|\mu\| = |\mu|(1) = \int d|\mu|.
$$

这个公式将在第1章中得到推广。 IV, §4, No. 7。

在*紧凑* 空间 $X$ 上，对于$X$ 复数 $\mu(1)$ 上的每个（复杂）测量$\mu$ 称为$\mu$ 的*总质量*。当$\mu$为*正*时，其总质量等于其范数。当 $\mu$ 是总质量等于 1 的*紧凑* 空间 $X$ 的正度量时，也可以说连续函数 $f \in \mathscr{C}(X; \mathbf{C})$ 的值 $\mu(f)$ 是 $f$ 相对于该度量的*平均值* $\mu$。

#### 推论 3 {#int-iii-s1-prop-10-cor-3 .statement tag=08LS}

— 对于局部紧凑空间 $X$ 上的每个实际测量$\mu$，

$$
\| \mu \| = \sup_{\| f \| \leq 1,\ f \in \mathscr{K}(X; \mathbf{R})} | \mu(f) | .
$$

当$\mu$是实测度并且$f \in \mathscr{K}_+(X)$时，使用公式(22)和表达式(9)来表示$|\mu|(f)$就足够了。

因此，有界实际测度的集合是规范化空间 $\mathscr{K}(X; \mathbf{R})$ 的对偶；如果不会造成混淆，则表示为 $\mathscr{M}^1(X, \mathbf{R})$ 或 $\mathscr{M}^1(X)$。 典范嵌入 $\mathscr{M}^1(X, \mathbf{R}) \to \mathscr{M}^1(X; \mathbf{C})$ 是根据 (24) 的等距。

#### 命题 11 {#int-iii-s1-prop-11 .statement tag=08LT}

— 如果 $\mu$ 和 $\nu$ 是 $X$ 的两个正测度，则$\| \mu + \nu \| = \| \mu \| + \| \nu \|$。

对于，函数$f \in \mathscr{K}(X; \mathbf{R})$，使得$0 \leq f \leq 1$形式有向集合$S$对于关系$\leq$。对于 $X$ 上的正测度 $\mu$，因此可以从 (22) 和单调极限定理得出 $\| \mu \| = \lim_{f \in S} \mu(f)$； 命题的结论随即而来。

#### 推论 1 {#int-iii-s1-prop-11-cor-1 .statement tag=08LU}

— 如果$\mu$和$\nu$是$X$的两个正测度使得$\mu \leq \nu$，则$\| \mu \| \leq \| \nu \|$；特别是，如果 $\nu$ 有界，那么 $\mu$ 也是有界的。
确实，$\| \nu \| = \| \mu \| + \| \nu - \mu \|$。

#### 推论 2 {#int-iii-s1-prop-11-cor-2 .statement tag=08LV}

— 对于 $X$ 上的每一个实际测量 $\mu$，

$$
\| \mu \| = \| \mu^+ \| + \| \mu^- \|.
$$

对于（第 10 号提案第 1 条），$\mu$ 的范数等于$|\mu| = \mu^+ + \mu^-$。

#### 命题 12 {#int-iii-s1-prop-12 .statement tag=08LW}

— 如果 $\mu$ 是 $X$ 上的有界测度，并且 $g$ 是 $X$ 到 $\mathbf{C}$ 的有界连续映射，则测度 $g \cdot \mu$ 是有界的且 $\| g \cdot \mu \| \leq \| g \| \cdot \| \mu \|$。

对于每函数 $f \in \mathscr{K}(X; \mathbf{C})$，

$$
|\mu(fg)| \leq \| \mu \| \cdot \| fg \| \leq \| \mu \| \cdot \| g \| \cdot \| f \|.
$$

### 9. 对空间措施含糊不清拓扑

令 $X$ 为局部紧致空间。在空间$\mathscr{M}(X; \mathbf{C})$上，我们可以考虑$\mathscr{K}(X; \mathbf{C})$中的逐点收敛的拓扑，我们将其称为$\mathscr{M}(X; \mathbf{C})$上的模糊拓扑。

从$\mathscr{K}(X; \mathbf{C}) = \mathscr{K}(X; \mathbf{R}) + i \mathscr{K}(X; \mathbf{R})$开始，$\mathscr{M}(X; \mathbf{C})$上的模糊拓扑由*半范数*$\sup_{1 \leq i \leq n} |\mu(f_i)|$定义，其中$(f_i)_{1 \leq i \leq n}$是$\mathscr{K}(X; \mathbf{R})$（或$\mathscr{K}_+(X)$）中函数的任何有限序列。说$\mathscr{M}(X; \mathbf{C})$上的过滤器$\mathfrak{F}$*模糊地**到度量$\mu_0$意味着

$$
\mu_0(f) = \lim_{\mu, \mathfrak{F}} \mu(f)
$$

每函数 $f \in \mathscr{K}(X; \mathbf{R})$。对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$，映射 $\mu \mapsto \mu(f)$ 是空间 $\mathscr{M}(X; \mathbf{C})$ 上的*模糊连续* 线性形式。

#### 命题 13 {#int-iii-s1-prop-13 .statement tag=08LX}

*令X为局部紧致空间，对于每个$x \in X$，令$\varepsilon_x$为点x处的狄拉克测度。 映射$x \mapsto \varepsilon_x$是X测度的X到空间$\mathscr{M}(X; \mathbf{C})$的子空间的同胚，配备模糊拓扑。此外，如果$X'$表示在无穷远$\omega$处与X点邻接而获得的紧空间，则当x趋于$\omega$时，$\varepsilon_x$趋于0。*

对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$，$\langle f, \varepsilon_x \rangle = f(x)$；由于 $f$ 是连续的，因此证明映射 $x \mapsto \varepsilon_x$ 是连续的。如果$x, y$是X的两个不同的点，则存在函数$f \in \mathscr{K}(X; \mathbf{C})$使得$f(x) = 1, f(y) = 0$(No. 2，引理1)，从而证明$\varepsilon_x \neq \varepsilon_y$；因此映射 $x \mapsto \varepsilon_x$ 是单射的。此外，对于每个函数$f \in \mathscr{K}(X; \mathbf{C})$，$\langle f, \varepsilon_x \rangle$趋向于定义，就像$x$趋向于$\omega$一样，因此$x \mapsto \varepsilon_x$可以通过连续性扩展到$X' = X \cup \{ \omega \}$，方法是在以下位置将值0分配给它点$\omega$。这个扩展的映射也是单射的，因为$\varepsilon_x \neq 0$对于所有$x \in X$。因此，它是紧凑空间$X'$到$\mathscr{M}(X; \mathbf{C})$的子空间的同胚，因为$\mathscr{M}(X; \mathbf{C})$是模糊拓扑的Hausdorff（GT，I, §9, No. 4，Th.2的Cor.2）。

#### 命题 14 {#int-iii-s1-prop-14 .statement tag=08LY}

*在局部紧凑空间X上的测度空间$\mathscr{M}(X; \mathbf{C})$中，对于从模糊拓扑*推导出来的均匀结构，正测度圆锥$\mathscr{M}_+(X)$是完整的（因此在$\mathscr{M}(X; \mathbf{C})$中“模糊地封闭”）。

例如，考虑使用柯西滤波器 $\Phi$ 来处理 $\mathscr{M}_+(X)$ 上的模糊均匀结构；通过定义，每个函数$f \in \mathscr{K}(X; \mathbf{C})$都存在$\mu_0(f) = \lim_{\mu, \Phi} \mu(f)$，并且通过扩张不等式的原理，每个函数$f \in \mathscr{K}_+(X)$都存在$\mu_0(f) \geq 0$；由此可见，$\mu_0$ 是X 的正测度（No. 5，Th.1）。

应该注意的是，对于模糊制服结构（TVS，II, §6, No. 7）来说，空间$\mathscr{M}(X; \mathbf{C})$（或$\mathscr{M}(X; \mathbf{R})$）本身*不一定完整*。

#### 推论 {#int-iii-s1-n9-cor-1 .statement tag=08LZ}

*如果A和B是$\mathscr{M}_+(X)$的两个模糊闭子集，则$A + B$在$\mathscr{M}_+(X)$中模糊闭（因此也在$\mathscr{M}(X; \mathbf{C})$中）。*

这实际上是局部凸空间中的弱完全、真锥体的一般性质（TVS，II, §6, No. 8，第 11 条命题的 Cor.2）。

#### 命题 15 {#int-iii-s1-prop-15 .statement tag=08M0}

— 令 $H$ 为 $\mathscr{M}(X; \mathbf{C})$ 的子集。以下属性是等效的：

a) $H$ 是有模糊界限的。
b) $H$ 隐约相对紧凑。
c) $H$ 等连续。
d) 对于$X$的每个紧凑子集$K$，存在数$M_K \geq 0$，使得$|\mu(f)| \leq M_K \|f\|$对于每个度量$\mu \in H$和每个函数$f \in \mathscr{K}(X, K; \mathbf{C})$。

由于 $\mathscr{K}(X; \mathbf{C})$ 是桶状空间（No. 1，命题 2），属性 a)、b) 和 c) 的等价源自 TVS、III, §4, No. 1、Scholium。

显然，d) 暗示了 a)。最后，如果 $H$ 是等连续的，则 $\mu \in H$ 到 $\mathscr{K}(X, K; \mathbf{C})$ 的度量的限制的集合也是等连续的，从而条件 d)，因为 $\mathscr{K}(X, K; \mathbf{C})$ 是规范的空间。

\* 我们将在第 1 章中看到。 IV, §4, No. 6 命题 15 的条件也等价于条件，对于 $X$ 的每个紧凑子集 $K$，存在一个常数 $M_K$，使得对于每个测度都有 $|\mu|(K) \leq M_K$ $\mu \in H$.*

#### 推论 1 {#int-iii-s1-prop-15-cor-1 .statement tag=08M1}

— 设$\nu$为$X$的正测度； 集合措施$\mu$ 使得$|\mu| \leq \nu$ 是模糊紧凑的。

#### 推论 2 {#int-iii-s1-prop-15-cor-2 .statement tag=08M2}

— $\mu$ 的集合使得$\|\mu\| \leq a$（$a$任何有限的数$> 0$）是模糊紧致的。

#### 推论 3 {#int-iii-s1-prop-15-cor-3 .statement tag=08M3}

— 如果 $X$ 是紧致的，则$X$ 上的$\mu$ 正措施集合使得 $\|\mu\| = 1$ 是模糊紧致的。

因为，它是模糊的紧集（Cor.2）测度中的交，例如$\|\mu\| \leq 1$和分别由关系、$\mu \geq 0$和$\mu(1) = 1$定义的模糊封闭的集合（No. 8，第10号提案的Cor.2）。

#### 推论 4 {#int-iii-s1-prop-15-cor-4 .statement tag=08M4}

— 在空间 $\mathscr{M}(X; \mathbf{C})$ 中，映射 $\mu \mapsto \|\mu\|$ 对于模糊的拓扑是下半连续的。

这是推论 2 中的直接的推论。

应该注意的是，对于模糊的拓扑（Exer.9），$\mathscr{M}(X; \mathbf{C})$的映射$\mu \mapsto |\mu|$本身不一定是连续的。

#### 命题 16 {#int-iii-s1-prop-16 .statement tag=08M5}

— 令$K$为$X$的紧凑子集，$H$为$\mathscr{M}(X; \mathbf{C})$的模糊边界子集；那么，当$\mathscr{K}(X, K; \mathbf{C})$配备一致收敛的拓扑且$H$配备模糊拓扑时，双线性形式$(f, \mu) \mapsto \langle f, \mu \rangle$在$\mathscr{K}(X, K; \mathbf{C}) \times H$上连续。

因为，存在数 $M \geqslant 0$ 使得
$$
|\mu(f)| \leqslant M \|f\|
$$
对于每个函数$f \in \mathscr{K}(X, K; \mathbf{C})$和每个$\mu \in H$（提案15）。如果$\mu_0$和$\mu$是属于到$H$的两个小节，$f_0$和$f$是$\mathscr{K}(X, K; \mathbf{C})$中的两个函数，则
$$
|\mu(f) - \mu_0(f_0)| = |\mu(f - f_0) + \mu(f_0) - \mu_0(f_0)| \\
\leqslant M \|f - f_0\| + |\mu(f_0) - \mu_0(f_0)|,
$$
当$\|f - f_0\|$和$|\mu(f_0) - \mu_0(f_0)|$为时，最后一个数量是任意小的，这证明了命题。

### 10. $\mathscr{M}(X; \mathbf{C})$ 的紧凑收敛

回想一下，$\mathscr{M}(X; \mathbf{C})$ 上的*紧致收敛* 的拓扑是 $\mathscr{K}(X; \mathbf{C})$ 的紧致子集中一致收敛的拓扑。我们将在$\mathscr{K}(X; \mathbf{C})$的严格紧致子集（No. 1）中的一致收敛的$\mathscr{M}(X; \mathbf{C})$拓扑上称为*拓扑严格紧致收敛*。

#### 命题 17 {#int-iii-s1-prop-17 .statement tag=08M6}

*在空间$\mathscr{M}(X; \mathbf{C})$上，考虑以下拓扑：*
$\mathscr{T}_1$：*拓扑，总共子集 T $\mathscr{K}(X; \mathbf{C})$；*
$\mathscr{T}_2$: *模糊拓扑;*
$\mathscr{T}_3$：*严格紧致收敛的拓扑；*
$\mathscr{T}_4$：*紧凑收敛的拓扑。*
*这些拓扑中的每一个都比下一个更粗糙。此外：*
*(i)* *有界集合对于 $\mathscr{T}_2$、$\mathscr{T}_3$ 和 $\mathscr{T}_4$ 是相同的。*
*(ii)* *如果 H 是 $\mathscr{M}(X; \mathbf{C})$ 的模糊边界子集，则由拓扑 $\mathscr{T}_1$、$\mathscr{T}_2$、$\mathscr{T}_3$、$\mathscr{T}_4$ 在 H 上导出的拓扑是相同的。*

$\mathscr{M}(X; \mathbf{C})$ 的模糊边界子集 $H$ 是等连续的（No. 9，命题 15），因此第一个断言来自 TVS，III, §3, No. 7，命题 9，第二个来自 GT，X, §2, No. 4，Th。 1.

回想一下，当 $X$ 为 *paracompact* 时，严格紧致收敛的拓扑与紧致收敛的拓扑一致（No. 1，命题 2）。

#### 命题 18 {#int-iii-s1-prop-18 .statement tag=08M7}

*在锥体$\mathscr{M}_+(X)$上，由以下拓扑引起的拓扑重合：*
$\mathscr{T}_1$：*$\mathscr{K}(X; \mathbf{C})$的线性子空间V中的逐点收敛拓扑，该子空间在$\mathscr{K}(X; \mathbf{C})$中稠密，并且满足性质(P)（No. 7，性质9）；*

\textit{\mathscr{T}_2：模糊的拓扑；}

\textit{\mathscr{T}_3: 严格紧致收敛的拓扑。}

由于每个滤波器都是超滤波器更细的交而不是它（GT，I, §6, No. 4，命题 7），因此足以证明，如果 $\mathfrak{U}$ 是 $\mathscr{M}_+(X)$ 上的超滤波器，对于拓扑 $\mathscr{T}_1$ 收敛到测度 $\mu_0$，那么它也对于 $\mathscr{T}_3$ 收敛于 $\mu_0$。设$K$是$X$的紧子集；到假设，存在函数$h \in V$，即$X$上的$\geqslant 0$，并在$K$上取值$> 0$；由此可见，每个函数 $f \in \mathscr{K}(X, K; \mathbf{C})$ 都可以写成 $f = gh$ 和 $g \in \mathscr{K}(X, K; \mathbf{C})$，如果是 $c = \inf_{x \in K} h(x) > 0$ 那么$\|g\| \leqslant c^{-1}\|f\|$。到假设时，存在集合 $H_0 \in \mathfrak{U}$，使得对于每个度量 $\mu \in H_0$，

$$
0 \leqslant \mu(h) \leqslant \mu_0(h) + 1 = b.
$$

因而，对于每个函数 $f \in \mathscr{K}(X; \mathbf{C})$，

$$
|\langle f, h \cdot \mu \rangle| = |\langle hf, \mu \rangle| \leqslant \|f\| \cdot \mu(h) \leqslant b \|f\|
$$

对于每一个测量$\mu \in H_0$；这证明了度量$h \cdot \mu$的集合$H$，其中$\mu$超过$H_0$，是\emph{模糊有界}。如果$\mathfrak{U}_0$是$H_0$上$\mathfrak{U}$诱导的超滤器，则映射下$\mathfrak{U}_0$的像，$\mu \mapsto h \cdot \mu$是$H$上$\mathfrak{F}$超滤器的基，并且由于$H$相对紧凑对于严格紧致收敛的拓扑（命题17和No. 9，命题15），$\mathfrak{F}$收敛于拓扑的测度$\nu_0$。在其他字中，对于任何$\varepsilon > 0$和$\mathscr{K}(X, K; \mathbf{C})$的任何紧凑子集$L$，存在$H_0$属于到$\mathfrak{U}$的子集$N$，这样，对于每个函数$g \in L$以及$\mu, \mu'$属于到$N$的每对小节，有$|\langle g, h \cdot \mu \rangle - \langle g, h \cdot \mu' \rangle| \leqslant \varepsilon$，即

$$
|\langle gh, \mu \rangle - \langle gh, \mu' \rangle| \leqslant \varepsilon.
$$

现在，我们在上面看到映射$g \mapsto gh$是Banach空间$\mathscr{K}(X, K; \mathbf{C})$的\emph{自同构}。因此，我们证明$\mathfrak{U}$是$\mathscr{M}_+(X)$上拓扑严格紧致收敛的\emph{柯西滤波器}。 \emph{A 更不必说}，它是一个用于模糊收敛的柯西滤波器，No. 9的第14条命题表明它模糊地收敛到一个测度$\mu_1$；此外，由于$V$在$\mathscr{K}(X; \mathbf{C})$中稠密，假设意味着$\mu_1 = \mu_0$；最后，由于$\mathfrak{U}$是严格紧致收敛的拓扑的柯西滤波器，因此对于拓扑它也收敛到$\mu_0$（GT，X, §1, No. 5，命题5）。

Q.E.D.

#### 推论 {#int-iii-s1-n10-cor-1 .statement tag=08M8}

— *如果 X 是仿紧致的，则由紧致收敛重合的模糊拓扑和拓扑在 $\mathscr{M}_+(X)$ 上导出的拓扑。*

然而，当X不是仿紧时，紧致收敛的拓扑和严格紧致收敛的拓扑在$\mathscr{M}_+(X)$上导出的拓扑可能会不同（例3）。

### 习题 {#int-iii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
