---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 5
section_title: Measures on completely regular spaces
lang: zh
source: int-vii-ix
book_pages: INT IX.56-INT IX.72, INT IX.113-INT IX.117
pdf_pages: 0238-0254, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: Measures and bounded continuous functions
      page: 56
      pdf_page: 238
    - "no": 2
      title: Bounded measures and linear forms on $\mathscr{C}^b(T)$
      page: 59
      pdf_page: 241
    - "no": 3
      title: Tight convergence of bounded measures
      page: 60
      pdf_page: 242
    - "no": 4
      title: 'Application: topological properties of the space $\mathscr{M}_+^b(T)$'
      page: 63
      pdf_page: 245
    - "no": 5
      title: Compactness criterion for tight convergence
      page: 64
      pdf_page: 246
    - "no": 6
      title: Tight convergence of measures and compact convergence of functions
      page: 67
      pdf_page: 249
    - "no": 7
      title: 'Application: the Laplace transformation'
      page: 68
      pdf_page: 250
statements: 33
exercises: 13
content_sha256: 77601149dec8d7e2c22af1babfcdfa071a1ae86257adbb249a5b8ee839431706
translated_from: content/en/int/IX/05_s5_measures_on_completely_regular_spaces.md
translation_method: google
source_content_sha256: 0a375a056c9792c3ccd44cccce1d823b83bccfdd6973e87e8cb9fdf911d4ef53
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 864b80947d1ee203e8e5457ada2123306fa945356d757f6636e9566d0685101c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。完全正常的措施空间

如果T是拓扑空间，F是Banach空间，则记号$C^b(T; F)$表示T上有界连续函数的空间，F中值，配备一致收敛的范数。如果$F = \mathbf{R}$，则此记号缩写为$C^b(T)$，如果没有歧义则缩写为$C^b$，并且用$C^b_+(T)$或$C^b_+$表示$C^b(T)$中正函数的圆锥体。 T 上有界复测度的空间将表示为 $M^b(T; \mathbf{C})$，有界实测度的空间将表示为 $M^b(T)$ 或 $M^b$，有界正测度的锥体将表示为 $M^b_+(T)$ 或 $M^b_+$。

### 1. 测度和有界连续函数

回想一下 (GT, IX, §1, No. 5, Def. 4)，如果拓扑空间 T 是可均匀化且 Hausdorff 的，则称其是完全正则的。这相当于说（参见第 3 条命题），即 T 同胚于紧致空间的子空间。如果T是完全正则的，则T上的每个正下半连续函数$f$是$C^b_+(T)$的元素递增有向集合的上包络，即$\leq f$，并且每个正有界上半连续函数 $g$ 是 $C^b_+(T)$ 的元素的递减有向集合的下包络线，即$\geq g$（前述，§1, No. 6，第 5 条）。我们需要以下引理：

#### 引理 {#int-ix-s5-n1-lem-1 .statement tag=09QV}

设T是完全正则空间，K是T的紧子集，U是T包含K的开子集。
a) 存在 T 的开子集 U'，使得 $K \subset U' \subset \overline{U'} \subset U$。
b) 令 f 为在 K 上定义的连续函数，其中值位于I $\mathbf{R}$ 区间（分别在 $\mathbf{C}$ 中）。 T 上存在有界连续函数 $f'$，I 中有值（$\mathbf{C}$），扩展 f 且 $T - U$ 上有零。

处理T是紧致空间X的子空间的情况就足够了。令V为X的开子集，使得$V \cap T = U$；用$V'$表示X包含K中的开集合，使得$\overline{V'} \subset V$，用g表示X上的连续函数，以及I中的值（分别在$\mathbf{C}$中）在$X - V$上扩展f和零（GT，IX, §4, No. 1，提案1）。 条件 a) 通过取 $U' = V' \cap T$ 来满足，b) 通过将 $f'$ 取为 g 到 T 的限制来满足。

#### 命题 1 {#int-ix-s5-prop-1 .statement tag=09QW}

— 设 T 是完全正则的空间。
a) 令 $\mu$ 为 T 上的正测度，f 为 T 上定义的数值函数 $\geq 0$ 和下半连续（分别为上半连续，有限，具有紧支撑）。然后

(1) $\mu^\bullet(f) = \sup_{g \in I_f} \mu^\bullet(g)$（分别为$\mu^\bullet(f) = \inf_{g \in S_f} \mu(g)$），

其中$I_f$（或$S_f$）表示有界连续函数$g$的集合，使得$0 \leq g \leq f$（或$g \geq f$）。

b) 令 $\theta$ 为 $T$ 上的复测度，$f$ 为$T$ 及下半连续上定义的数值函数 $\geq 0$。然后

(2) $|\theta|^\bullet(f) = \sup_g |\theta(g)|$,

其中 $g$ 超过有界且 $|\theta|$ 可积连续复形函数的集合，使得 $|g| \leq f$。

公式(1)的第一个是显而易见的，因为$I_f$是连续函数的递增有向集合，其上包络线是$f$，并且可以应用§1, No. 6的第5条命。同样的命题将意味着第二个公式，如果我们证明$S_f$包含是$\mu$可积有界连续函数。因而，令$K$为$f$的支持，$M$为$f$的上确界；由于 $K$ 是紧致的，$M$ 是有限的（GT、IV, §6, No. 2、Th. 3）。令 $U$ 为开集合包含 $K$ 且$\mu^\bullet(U) < +\infty$；存在(引理)一个连续的函数$g$，$[0, M]$内有值，等于$K$上的$M$，$U$外有零；然后是$g \in S_f$和$\mu^\bullet(g) \leq M \mu^\bullet(U) < +\infty$。

让我们转到b)。显然足以证明$|\theta|^\bullet(f) \leq \sup_g |\theta(g)|$。

令$a$和$b$是两个实数，使得$a < b < |\theta|^\bullet(f)$。由(1)，存在函数$h \in \mathscr{C}_+^b(T)$使得$h \leq f$和$|\theta|^\bullet(h) > b$；用$M$表示$h$的上界。通过$|\theta|^\bullet$的定义（§1, No. 2，定义4），存在$T$的紧子集$K$，使得$|\theta|_K^\bullet(h_K) > b$。那么在$K$上存在一个连续复形函数$j$，使得$|j| \leq h_K$和$|\theta_K(j)| > b$（第III, §1, No. 6）。让我们选择一个开集合$U$包含$K$，这样$|\theta|^\bullet(U - K) \leq \frac{b - a}{M}$（§1, No. 9，提案13和14）； 扩展 $j$ 到 $T$ 上的连续复合体函数 $k$，$U$ 外部零 (引理)；每$t \in T$、集合

(3)
$$
g(t) = \begin{cases}
k(t) & \text{if } |k(t)| \leq h(t) \\
\frac{k(t)}{|k(t)|} h(t) & \text{if } |k(t)| > h(t)
\end{cases}
$$

显然$|g| \leq h \leq f$，$g = j$在$K$上，因而$||\theta_K(j)| - |\theta(g)|| = ||\theta(j^0)| - |\theta(g)|| \leq |\theta|^\bullet(|j^0 - g|) \leq M \cdot |\theta|^\bullet(U - K) \leq b - a$，因而$|\theta(g)| > a$。另一方面，让我们证明 $g$ 是连续的函数：

由于$a$受制于唯一的条件$a < |\theta|^*(f)$，这意味着(2)的第二个成员是$\geqslant$第一个，从而命题。现在，令 F（分别为 $F'$）为 $t \in T$ 的集合，使得 $|k(t)| \leq h(t)$（分别为 $|k(t)| \geq h(t)$）。这些集合是封闭的，并且它们的并是T，足以证明$g_F$和$g_{F'}$是连续的：现在，这个性质对于$g_F = k_F$来说是明显的，对于$g_{F'}$在点处也是如此，其中$k(t) \neq 0$；另一方面，如果$t \in F'$满足$k(t) = 0$，则$h(t) = 0$和不等式$|g| \leq h$意味着$g$在点$t$连续。

#### 注 1 {#int-ix-s5-n1-rem-1 .statement tag=09QX}

令$f$为正下半连续函数，并令$J_f$为$\mu$可积开集合外部且以$f$为界的正有界连续函数零的集合。 可以证明$f$是$J_f$和$\mu^*(f) = \sup_{g \in J_f} \mu(g)$的上包络线。

#### 注 2 {#int-ix-s5-n1-rem-2 .statement tag=09QY}

如果测度 $\mu$ 有界，则公式 $\mu^*(f) = \inf_{g \in S_f} \mu(g)$ 显然对每个上半连续、正且有界的函数 $f$ 有效。

#### 命题 2 {#int-ix-s5-prop-2 .statement tag=09QZ}

— *令 $\eta$ 和 $\eta'$ 为完全正则空间 $T$ 上的两个复杂测度，使得 $\eta(f) = \eta'(f)$ 对于每个函数 $f \in \mathscr{C}^b(T)$ 可积为 $|\eta|$ 和 $|\eta'|$。然后$\eta = \eta'$.*

让我们在设定 $\theta = \eta - \eta'$ 上再次讨论命题 1 的第二个部分的证明。 我们可以要求开集合 U 对于$|\eta|$ 和$|\eta'|$ 可积。 The function $g$ is then integrable for these two measures, and the relation $\theta(g) = 0$ implies $a < 0$; therefore $|\theta|^*(f) = 0$ for every positive lower semi-continuous function $f$, whence finally $|\theta| = 0$, on taking $f = +\infty$.

#### 命题 3 {#int-ix-s5-prop-3 .statement tag=09R0}

— *令 $\mu$ 为完全正则空间 $T$ 的正测度，并令 $p \in [1, +\infty[$。 函数$f \in \mathscr{C}^b(T)$的空间$\mathscr{H}$，其支撑包含在$\mu$可积开集合中，在$\mathscr{L}^p(\mu)$中密集。*

根据§1, No. 10的第15条命题，足以证明，如果K在T中是紧的，并且如果$g$是扩张到T，$\mathscr{C}_+(K)$中函数的0在0和1之间，则存在函数$f \in \mathscr{C}_+^b(T)$，其支持包含在$\mu$-可积开集合，使得$\|f - g\|_p$任意小。现在，令 $\varepsilon$ 为数 $> 0$，U 为 K 的开邻域，使得 $\mu^*(U - K) < \varepsilon$，V 为 K 的开邻域，使得 $\overline{V} \subset U$，以及 $f$ 函数，其中值在 $[0, 1]$ 中，连续，等于K 上的 $g$ 以及 V (引理) 之外的 0。 函数 $|f - g|^p$ 则以 $\varphi_{U-K}$ 为界；因此$\|f - g\|_p \leq \varepsilon^{1/p}$，从而建立命题。

*注 3).* — 在 Banach 空间 F 中，函数与值存在类似的叙述：子空间 $\mathscr{H} \otimes F$ $\mathscr{C}^b(T; F)$ 在 $\mathscr{L}_F^p(\mu)$ 中稠密。

#### 命题 4 {#int-ix-s5-prop-4 .statement tag=09R1}

— *在阶中，完全正则空间$T$上的有界复数测度$\theta$为正，对于每个函数$f \in \mathscr{C}_+^b(T)$，$\theta(f) \geq 0$是必要且充分的。*

必要性是显而易见的。为了确定充分性，让我们在取 $p = 1$ 和 $\mu = |\theta|$ 的基础上，再次取前面命题的证明； 记号相同，关系$\mu^*(|f - g|) \leq \varepsilon$和不等式$\theta(f) \geq 0$意味着$\theta_K(g_K) = \theta(g) \geq -\varepsilon$；由于$g_K$是$\mathscr{C}(K)$在0和1之间的任意元素，因此测度$\theta_K$为正； 紧集 K 是任意的，这意味着 $\theta$ 是正数。

### 2. 有界度量和 $\mathscr{C}^b(T)$ 上的线性形式

#### 命题 5 {#int-ix-s5-prop-5 .statement tag=09R2}

— *令 T 为完全正则空间，且 I 为范数空间 $\mathscr{C}^b(T; \mathbf{C})$ 上的连续复形线性形式。在阶中，T上存在有界复测度$\theta$，使得$\theta(f) = I(f)$对于所有$f \in \mathscr{C}^b(T; \mathbf{C})$，满足以下条件是必要且充分的：

(M) *对于每个数 $\varepsilon > 0$，都存在 T 的紧凑子集 K，使得关系 $g \in \mathscr{C}^b(T; \mathbf{C}), |g| \leq 1, g_K = 0$ 隐含 $|I(g)| \leq \varepsilon$。

那么度量 $\theta$ 是唯一的。*

唯一性源自No. 1的第2条命题。让我们证明条件 (M) 是必要的。令 $\theta$ 为有界复数测度；令 K 为紧集，使得 $|\theta|^*(T - K) \leq \varepsilon$ (§ 1, No. 2, *注 3*)。假设$|g| \leq 1, g_K = 0$意味着$|g| \leq \varphi_{\mathbf{C}_K}$，因此$|\theta(g)| \leq |\theta|^*(\varphi_{\mathbf{C}_K}) \leq \varepsilon$。

让我们讨论充分性的证明。令 X 为 T 的 Stone–Čech 紧致化（GT，IX, § 1，Exer.7；或 TG，IX, § 1, No. 6）。对于每个函数 $f \in \mathscr{C}(X; \mathbf{C})$，集合 $\nu(f) = I(f_T)$；我们以这种方式定义在$\mathscr{C}(X; \mathbf{C})$上连续线性形式，即紧凑空间X上的复杂测度。设$\varepsilon$为数$> 0$，K紧集满足（M）； 函数$\varphi_{\mathbf{C}_K}$在X、公式(2)上是下半连续且正的，给出以下关系，其中$\mathscr{G}$表示函数$g \in \mathscr{C}(X; \mathbf{C})$的集合，使得$|g| \leq \varphi_{\mathbf{C}_K}$：

$$
|\nu|^*(X - K) = \sup_{g \in \mathscr{G}} |\nu(g)| = \sup_{g \in \mathscr{G}} |I(g_T)| \leq \varepsilon.
$$

令$(K_n)_{n \geq 1}$为T的紧凑子集的序列，使得每个$K_n$对于$\varepsilon = 1/n$满足(M)，并令$S = \bigcup K_n$； S 是 X 中的 Borel 集合，包含在 T 中，并且对于所有 n 而言为 $|\nu|^*(X - T) \leq |\nu|^*(X - S) \leq |\nu|^*(X - K_n) \leq 1/n$，因此 T 是 $\nu$ 可测的，$\nu$ 集中在 T 上。令 $f$ 为 T 上的有界连续函数；由于 X 是 T 的 Stone-Čech 紧化，因此 $f$ 可以通过连续性扩展到函数 $g \in \mathscr{C}(X; \mathbf{C})$。现在令$\mu$为$\nu$在$T$上引起的测度；一个有 $\mu(f) = \nu(f^0)$。 (1) 由于$\nu$集中于$T$，函数、$f^0$和$g$几乎处处都相等$\nu$，因此$\mu(f) = \nu(g) = I(g_T) = I(f)$，它完成了证明。

#### 推论{#int-ix-s5-n2-cor-1 .statement tag=09R3}

— *使用第 5 条中的记号，假设 $T$ 上存在有界正测度 $\mu$，使得 $|I(f)| \leq \mu(|f|)$ 对于所有 $f \in \mathscr{C}^b(T; \mathbf{C})$；那么$T$上存在一个复杂测度$\theta$，使得$\theta(f) = I(f)$适用于所有$f \in \mathscr{C}^b(T; \mathbf{C})$。

### 3. 有界测度的紧密收敛

设$T$是完全正则的空间； 双线性形式
$$
(f, \mu) \mapsto \int f(t) \, d\mu(t)
$$
在$\mathscr{C}^b(T) \times \mathscr{M}^b(T)$上将这两个空间置于分离的二元性中。因为，很明显，$\mathscr{C}^b(T)$中的二元性与$\varepsilon_x \ (x \in T)$属于到$\mathscr{M}^b(T)$的测量事实相分离；它在 $\mathscr{M}^b(T)$ 中由 No. 1 的命题 2 分离。

#### 定义 1 {#int-ix-s5-def-1 .statement tag=09R4}

*与前面的$\mathscr{C}^b(T)$和$\mathscr{M}^b(T)$之间的对偶性相关的$\mathscr{M}^b(T)$上的弱拓扑被称为$\mathscr{M}^b(T)$上紧收敛的拓扑（或紧拓扑）。*

紧的拓扑是Hausdorff，由注先于定义。我们经常使用副词“tightly”来表示“在紧密拓扑的意义上”。如果没有相反的情况，$\mathscr{M}^b(T)$将在截面的剩余时间内配备紧身的拓扑。

$\mathscr{C}^b(T)$的每个元素是$\mathscr{C}_+^b(T)$的元素的线性组合。对于$\mathscr{M}^b(T)$上的过滤器$\mathfrak{F}$紧密收敛到有界测度$\lambda$，有必要且充分：
$$
\lim_{\mu} \mu(f) = \lambda(f) \quad \text{with respect to } \mathfrak{F} \text{ for every } f \in \mathscr{C}_+^b(T).
$$

#### 注 1 {#int-ix-s5-n3-rem-1 .statement tag=09R5}

如果$T$是局部紧致的，则紧的拓扑比模糊拓扑在$\mathscr{M}^b(T)$上引起的拓扑要强于更细，并且这两种拓扑重合仅当$T$是紧致的时。因为，如果 $T$ 不是紧致的，则映射 $t \mapsto \varepsilon_t$ 相对于 $T$ 的相对紧致子集的补集过滤器模糊地收敛到 0，但不会紧密收敛到 0，因为函数 1 属于到 $\mathscr{C}^b(T)$ （对于模糊收敛和紧收敛之间的关系，参见命题9）。

(1) 这个关系仅在上面（§ 2, No. 1，命题1）$f$和$\nu$为正的情况下成立。 扩张目前的情况，其中$f$和$\nu$是复杂且有界的，通过线性度是直接的。

#### 注 2 {#int-ix-s5-n3-rem-2 .statement tag=09R6}

从命题 4 可以立即看出，$\mathscr{M}_+^b(T)$ 在$\mathscr{M}^b(T)$ 中是封闭的。

#### 注 3 {#int-ix-s5-n3-rem-3 .statement tag=09R7}

如果 T 是完全正则的，则 T 到 $\mathscr{M}^b(T)$ 的映射 $t \mapsto \varepsilon_t$ 是同胚（GT，IX, §1, No. 5）。

#### 命题 6 {#int-ix-s5-prop-6 .statement tag=09R8}

— 设 T 是完全正则的空间。

a) 设f为T上定义的下半连续数值函数$\geqslant 0$；那么函数$\mu \mapsto |\mu|^*(f)$在$\mathscr{M}^b(T)$上是下半连续的。

b) 设 f 为 T 上定义的上半连续有界函数；那么函数$\mu \mapsto \mu(f)$是$\mathscr{M}_+^b(T)$上的上半连续。

因为，根据No. 1的命题1 b)可以看出，$\mu \mapsto |\mu|^*(f)$是形式$\mu \mapsto |\mu(g)|$和$g \in \mathscr{C}^b(T)$的函数族的上层信封，因此对于紧的拓扑是连续的。这就建立了a)。为了证明b)，只要选择为f的常数上界C，并写成$\mu(f) = \mu(C) - \mu(C - f)$即可；由上可知，函数$\mu \mapsto \mu(C)$是连续的，函数$\mu \mapsto \mu(C - f)$是$\mathscr{M}_+^b(T)$上的下半连续。

#### 命题 7 {#int-ix-s5-prop-7 .statement tag=09R9}

— 设 T 是完全正则的空间。令 $\mu$ 为 T 上的有界正测度，并令 f 为 T 上的有界正函数，这样，当 f 不连续时，T 的点的集合局部$\mu$ 可忽略不计。那么$\mathscr{M}_+^b(T)$到$\mathbf{R}$的映射$\lambda \mapsto \lambda^*(f)$在点$\mu$处连续。

对于每个 $t \in T$、集合 $f'(t) = \liminf_{s \to t} f(s)$、$f''(t) = \limsup_{s \to t} f(s)$。显然 $f' \leqslant f \leqslant f''$，在 T 的每点处有等式，其中 f 是连续的（因而 $\mu$ - 几乎无处不在）。另一方面，$f'$是下半连续，$f''$是上半连续且有界（GT，IV, §6, No. 2，命题4）。因而，根据第 6 条命题，我们得到以下关系，

$$
\mu^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f) \leqslant \mu^*(f) \leqslant \limsup_{\lambda \to \mu} \lambda^*(f)
$$
$$
\leqslant \limsup_{\lambda \to \mu} \lambda^*(f'') \leqslant \mu^*(f'').
$$

结论乘注意到即$\mu^*(f') = \mu^*(f'')$，因为$f'$和$f''$在局部$\mu$几乎处处相等。

#### 命题 8 {#int-ix-s5-prop-8 .statement tag=09RA}

— 令 X 为完全正则空间，X 的 T 子空间，以及 T 的 i 典范嵌入为 X。用 W 集合表示 X 上集中于 T 的有界正测度，配备由 $\mathscr{M}^b(X)$ 诱导的拓扑。那么$\mathscr{M}_+^b(T)$到$\mathscr{M}^b(X)$的映射$\mu \mapsto i(\mu)$是$\mathscr{M}_+^b(T)$到W的同胚。

我们再次将$\mathscr{M}_+^b(T)$的i映射$\mu \mapsto i(\mu)$表示为$\mathscr{M}_+^b(X)$； i 是单射（§2, No. 4，命题 8）和映射 $\mathscr{M}_+^b(T)$ 到 W（§2, No. 3，命题 7）。如果$\lambda \in W$，则$\lambda = i(\lambda_T)$（§2, No. 3，提案 7 b））。因而，i 是 W 上 $\mathscr{M}_+^b(T)$ 的双射，i 的逆双射是 $W$ 上的映射 $r : \lambda \mapsto \lambda_T$。另一方面，$i$是连续的：对于，如果$f \in \mathscr{C}^b(X)$，则$\langle i(\mu), f \rangle = \langle \mu, f \circ i \rangle$，$f \circ i$属于到$\mathscr{C}^b(T)$。因而，一切都归结为，对于每一个度量 $\mu \in W$ 和每一个函数 $f \in \mathscr{C}^b_+(T)$，一个人有

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda_T(f) = \mu_T(f),
$$

或再次

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda(f^0) = \mu(f^0).
$$

Let $f^\infty$ be the function on $X$ that coincides with $f$ on $T$ and with $+\infty$ on $X - T$, and let $f'$ and $f''$ be, respectively, the upper semi-continuous regularization of $f^0$ and the lower semi-continuous regularization of $f^\infty$ (GT, IV, §6, No. 2). The relations

$$
f'(x) = \limsup_{y \to x} f^0(y), \quad f''(x) = \liminf_{y \to x} f^\infty(y)
$$

立即暗示$f'$和$f''$都是重合，$f$和$f^0$在$T$上。命题 6 则得出

$$
\mu^\bullet(f') \geq \limsup_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'), \quad \mu^\bullet(f'') \leq \liminf_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'').
$$

但是在这两个公式中可以通过$f^0$来替换$f'$和$f''$，因为$\lambda$和$\mu$是由$T$承载的；这样我们就得到了想要的关系。

命题 8 的叙述仅对正测度有效：$\mathscr{M}^b(T)$到$\mathscr{M}^b(X)$的映射$\mu \mapsto i(\mu)$是单射且连续的，但通常不是$\mathscr{M}^b(T)$与其像的同胚。对于例，取$X = \mathbf{R}$、$T = \mathbf{R} - \{0\}$； $\lambda_t = \varepsilon_t - \varepsilon_{-t}$ ($t > 0$) 在 $X$ 中紧密收敛于 0，因为 $t$ 趋向于 0，但在 $T$ 中并不紧密收敛于 0（$]0, +\infty[$ 属于到 $\mathscr{C}^b(T)$ 的特征函数）（但是cf. No. 5 的 Cor。

#### 命题 9 {#int-ix-s5-prop-9 .statement tag=09RB}

— *令 T 为局部紧凑空间，并令 $\mathfrak{F}$ 为 $\mathscr{M}^b_+(T)$ 上的过滤器，模糊地收敛到有界测度 $\mu$。为了使$\mathfrak{F}$紧密收敛于$\mu$，$\lim_{\lambda} \lambda(1) = \mu(1)$相对于$\mathfrak{F}$是必要且充分的。*

条件显然是必要的。为了证明它是充分的，让我们用$X$表示$T$（GT，I, §9, No. 8）的Alexandroff紧缩，并用$i$典范嵌入将$T$表示为$X$。根据第 8 条命题，一切都可以归结为，在 $\mathscr{M}^b(X)$ 中，$\lambda \mapsto i(\lambda)$ 相对于 $\mathfrak{F}$ 紧密收敛于 $i(\mu)$。从$\mu(1) < +\infty$开始，存在集合$A \in \mathfrak{F}$，使得$A$中的测度总质量以数$M$为界；因此只需验证

$$
\lim_{\lambda, \mathfrak{F}} \int_X g \, d(i(\lambda)) = \int_X g \, d(i(\mu))
$$

函数 $g \in \mathscr{C}^b(X)$ 在 $\mathscr{C}^b(X)$ 中形成总计集合。现在，当$g$在$T$中具有紧凑支持时，由于$\mathfrak{F}$到$\mu$的模糊收敛，并且当$g$是$X$上的常量函数时，由于$\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$这一事实，等式就得到满足。由于前两个型形式中的函数在$\mathscr{C}^b(X)$中总计集合（第III, §1, No. 2，第3条），这完成了证明。

### 4. 应用：空间 $\mathscr{M}_+^b(T)$的拓扑性质

我们首先观察到，如果$T$是完全正则的，那么$\mathscr{M}^b(T)$是豪斯多夫拓扑向量空间，因此是完全正则的。因而，$\mathscr{M}_+^b(T)$是完全正则的。

#### 命题 10 {#int-ix-s5-prop-10 .statement tag=09RC}

*令$T$为波兰人空间； 空间 $\mathscr{M}_+^b(T)$ 则为紧身拓扑。*

我们首先处理 $T$ 是波兰语且*紧凑*的情况。具有质量 $\leq 1$ 的正测度的集合 $U$ 是紧致的（第 III, §1, No. 9 章，第 15 条命题第 2 条），并且拓扑在 $U$ 上由紧的拓扑 （这里是重合和模糊的拓扑）诱发，是也由 $\mathscr{C}(T)$ 的总子集上的拓扑逐点收敛引起（*loc.cit.*，No. 10，提案 17）。现在，$\mathscr{C}(T)$中存在可数总数集合（GT，X, §3, No. 3，Th.1）；因而，$U$是可度量的紧致空间。质量$< 1$的正测量的集合$V$在$U$中开放，因此是波兰局部紧凑空间。现在，$\mathscr{M}_+^b(T)$到$V$的映射$\mu \mapsto \frac{1}{1 + \mu(1)} \mu$是同胚，映射$\lambda \mapsto \frac{1}{1 - \lambda(1)} \lambda$是逆同胚。

让我们讨论 $T$ 是波兰语的情况；我们可以假设$T$是可度量紧凑空间$X$中开集合的递减序列$(G_n)$的交（GT，IX, §6, No. 1，Th.1的Cor.1）；那么，空间$\mathscr{M}_+^b(T)$同构于$\mathscr{M}_+^b(X)$由……组成的$T$措施中的子空间$W$（No. 3，第8条），并且足以证明$W$是交波兰语空间 $\mathscr{M}_+^b(X)$ 的开放集合的序列（GT，*loc.cit.*，Th.1）。 现在，令 $W_n$ 为集合，集中在$G_n$的措施$\mu \in \mathscr{M}_+^b(X)$； $\mathscr{M}_+^b(X)$上的映射$h_n : \mu \mapsto \mu^*(X - G_n)$是上半连续（No. 3，命题6），并且测度$\mu \in \mathscr{M}_+^b(X)$的集合$A_k^n$使得$h_n(\mu) < 1/k$因此对每个$k \geq 1$和每个$n \in \mathbf{N}$开放。 证明由注意到完成$W = \bigcap_n W_n = \bigcap_{n,k} A_k^n$。

#### 推论 1 {#int-ix-s5-prop-10-cor-1 .statement tag=09RD}

*如果 T 是可数型的可度量空间，则对于紧拓扑，$\mathscr{M}_+^b(T)$ 是可数型的可度量。*

对于定义 T 的拓扑的度量，令 $\hat{T}$ 为 T 的完成； 空间 $\hat{T}$ 是波兰语，$\mathscr{M}_+^b(T)$ 与波兰语空间 $\mathscr{M}_+^b(\hat{T})$ 由……组成的子空间同构，集中于 T 的措施（No. 3，第 8 条）。 但是波兰语空间的每个子空间都可度量可数型 (GT, IX, §2, No. 8)。

#### 推论 2 {#int-ix-s5-prop-10-cor-2 .statement tag=09RE}

*如果 T 是完全正则的 Souslin (resp. Lusin) 空间，则空间 $\mathscr{M}_+^b(T)$ 是 Souslin (resp. Lusin)。*

例如，考虑波兰空间 P 和 P 到 T 上的连续映射 $f$（GT，IX, §6, No. 2，Def. 2）。设$\tilde{f}$为$\mathscr{M}_+^b(P)$到$\mathscr{M}_+^b(T)$的连续映射$\mu \mapsto f(\mu)$； 空间 $\mathscr{M}_+^b(P)$ 是根据第 10 条命题的波兰式，$\tilde{f}$ 是满射（§2, No. 4，第 9 条命题）；因此，空间 $\mathscr{M}_+^b(T)$ 是苏斯林。类似地，如果 T 是 Lusin，则 $f$ 可以假定为单射（GT，*loc.cit.*，No. 4，Prop. 12）；那么 $\tilde{f}$ 是单射（§2, No. 4，第 8 条命题），因此 $\mathscr{M}_+^b(T)$ 是 Lusin（GT，*loc.cit.*，No. 4，第 12 条命题）。

令 T 为完全正则 Souslin 空间（回想一下，T 为 Souslin 且*正则*（TG，App. 1，Cor. of Prop. 2）就足够了），并令 H 为 $\mathscr{M}_+^b(T)$ 的紧致子集；那么 H 是紧致的且是 Souslin 的，因此 *可度量化*，对于紧拓扑 (*loc. cit.*, App. 1, Cor. 2 of Prop. 3)。

### 5. 紧收敛的紧致准则

#### 定义 2 {#int-ix-s5-def-2 .statement tag=09RF}

*设T为拓扑空间，设H为$\mathscr{M}^b(T)$的子集；有人说 H 满足 Prokhorov 的条件 if*
    a）$\sup_{\mu \in H} |\mu|(1) < +\infty$；
    b) *对于每个数 $\varepsilon > 0$，都存在一个 T 的紧凑子集 $K_\varepsilon$，使得*
    $$
    |\mu|(T - K_\varepsilon) \leq \varepsilon \quad \text{for every measure } \mu \in H.
    $$

可以证明，如果T是完全正则的，条件*a)*和*b)*的集合等价于下面的条件：T上存在实数函数$f \geq 1$，使得T满足的点t的集合 $f(t) \leq c$ 对于每个 $c \in \mathbf{R}_+$ 都是紧致的（这特别意味着 $f$ 是下半连续的），因此$\sup_{\mu \in H} |\mu|(f) < +\infty$。此外，当 T 是局部紧致时，通过要求 f 连续可以得到等价的叙述 (cf. Exer. 10)。

#### 命题 11 {#int-ix-s5-prop-11 .statement tag=09RG}

*设T为完全正则空间，设H为满足普罗霍罗夫条件的$\mathscr{M}^b(T)$的子集；那么它在 $\mathscr{M}^b(T)$ 中的闭包 $\overline{H}$ 满足 Prokhorov 的条件。*

因为，根据No. 3的第6条命题，函数、$\mu \mapsto |\mu|^*(1)$、$\mu \mapsto |\mu|^*(T - K_\varepsilon)$在$\mathscr{M}^b(T)$上是下半连续的。

普罗霍罗夫的条件的兴趣来自于下面的定理，其逆命题将在稍后（Th.2）进行研究。

#### 定理 1（普罗霍罗夫）{#int-ix-s5-thm-1 .statement tag=09RH}

— *令T为完全正则空间，令H为满足普罗霍罗夫条件的$\mathscr{M}^b(T)$的子集；那么对于紧拓扑，H 在 $\mathscr{M}^b(T)$ 中相对紧凑。*

我们可以假设 T 是紧致空间 X 的子空间；令 i 为 T 的典范嵌入变为 X。另一方面，根据命题 11，我们可以假设 H 在 $\mathscr{M}^b(T)$ 中*闭合*。那么就足以证明 H 上的每个超滤器 $\mathfrak{U}$ 都收敛于 $\mathscr{M}^b(T)$。

我们将从$H \subset \mathscr{M}_+^b(T)$的情况开始。以假设、$i(\mu)$为界的测度$\mu \in H$的总质量相对于$\mathfrak{U}$模糊地收敛于$\mathscr{M}_+(X)$，测度$\nu \in \mathscr{M}_+(X)$（第III, §1, No. 9章，第15条命题第2条）；根据No. 3的第8条，一切都归结为证明，$\nu$集中在T上。现在，令$\varepsilon$为数$> 0$，并让$K_\varepsilon$为T满足的紧凑子集公式 (6)。由于$X - K_\varepsilon$在X中开放，根据No. 3的第6条命题应用于X，我们有不等式

$$
\nu^*(X - T) \leq \nu^*(X - K_\varepsilon) \leq \liminf_{\mu, \mathfrak{U}} i(\mu)^*(X - K_\varepsilon)
= \liminf_{\mu, \mathfrak{U}} \mu^*(T - K_\varepsilon) \leq \varepsilon;
$$

由于$\varepsilon > 0$是任意的，因此在这种特殊情况下定理成立。

让我们转向一般情况；对于 T 上的每个测量$\mu$，集合

$$
a_1(\mu) = \Re(\mu)^+, \quad a_2(\mu) = \Re(\mu)^-, \quad a_3(\mu) = \Im(\mu)^+, \quad a_4(\mu) = \Im(\mu)^-;
$$

从 $\mu = a_1(\mu) - a_2(\mu) + ia_3(\mu) - ia_4(\mu)$ 开始，只需证明映射 $a_j$ ($j = 1, 2, 3, 4$) 相对于 $\mathfrak{U}$ 紧密收敛。但措施$a_j(\mu)$的集合$H_j$，其中$\mu$超过H，凭借关系$|a_j(\mu)| \leq |\mu|$满足普罗霍罗夫的条件，并且包含在$\mathscr{M}_+^b(T)$中；因此，在特殊情况下，$\mathscr{M}_+^b(T)$相对紧凑，然后定理紧随其后。

#### 推论{#int-ix-s5-n5-cor-1 .statement tag=09RI}

— 令 T 为完全正则空间 X 的子空间，并令 H 为满足 Prokhorov 条件的 $\mathscr{M}^b(T)$ 的子集。如果i表示T到X的典范嵌入，那么限制到$\mathscr{M}^b(T)$到$\mathscr{M}^b(X)$的映射$\mu \mapsto i(\mu)$的H是H到像的同胚。

处理 H 是闭合的情况（命题 11）就足够了，因此是紧凑的；结论是根据 $\mu \mapsto i(\mu)$ 是连续且单射的这一事实得出的。

回想一下，这个结果对于 $\mathscr{M}_+^b(T)$ 的任意子集也有效（No. 3，命题 8）。

#### 定理 2 {#int-ix-s5-thm-2 .statement tag=09RJ}

— 令 T 为局部紧致空间，或波兰式空间，并令 H 为 $\mathscr{M}_+^b(T)$ 的相对紧致子集；那么 H 满足 Prokhorov 的条件。

我们可以将自己限制在 H 是封闭的、因此是紧凑的情况。措施$\mu \in H$的总质量显然是有界的，因为映射$\mu \mapsto \mu(1)$是连续的，一切都归结为Def的证明断言b)。 2.

首先假设 T 是局部紧的。令$\varepsilon$为数 > 0。让我们将T中的每个测度$\mu \in H$紧集$K_\mu$关联起来，使得$\mu^\bullet(T - K_\varepsilon) < \varepsilon$，然后是$K_\mu$的相对紧凑的开放邻域$U_\mu$。 函数$\lambda \mapsto \lambda^\bullet(T - U_\mu)$在$\mathscr{M}_+^b(T)$（No. 3，命题6）、集合$V^\mu$上是$\lambda \in H$测度的上半连续，使得$\lambda^\bullet(T - U_\mu) < \varepsilon$是H中$\mu$的邻域。因此存在有限子集 H 的 $H'$ 使得集合 $V^\mu$ ($\mu \in H'$) 覆盖 H。用 K 紧集 $\bigcup_{\mu \in H'} \overline{U}_\mu$ 表示，对于所有 $\lambda \in H$，我们有 $\lambda^\bullet(T - K) < \varepsilon$。

接下来假设 T 是波兰语。我们不通过假设T是紧致空间X的开子集的递减序列$(T_p)_{p \geq 1}$的交来限制一般性（GT，IX, §6, No. 1，Th.1的Cor.1）。令$i_p$为$T_p$中T的单射，并令$H_p$为$\lambda \in H$的形式$i_p(\lambda)$度量的集合；由于 $H_p$ 在 $\mathscr{M}_+^b(T_p)$ 中是紧致的，因此存在紧集 $K_p \subset T_p$，使得对于每个测度 $\nu \in H_p$ 都有 $\nu^\bullet(T_p - K_p) \leq \varepsilon 2^{-p}$，通过将前面的结果应用于局部紧致空间 $T_p$。因此对于每一个小节$\lambda \in H$也是$\nu^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$，最后是$\lambda^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$。现在集合$K = \bigcap_p K_p$； 集合 K 是紧致的并且包含在 T 中，并且对于每个度量 $\lambda \in H$，我们有 $\lambda^\bullet(T - K) \leq \sum_p \lambda^\bullet(T - (T \cap K_p)) \leq \sum_p \varepsilon 2^{-p} = \varepsilon$。普罗霍罗夫的条件由此得到验证。

### 6. 措施的紧密收敛和函数的紧凑收敛

#### 命题 12 {#int-ix-s5-prop-12 .statement tag=09RK}

— 令 T 为完全正则空间，令 B 为规范空间 $\mathscr{C}^b(T; \mathbf{C})$ 的单位球。令I为$\mathscr{C}^b(T; \mathbf{C})$上的线性形式。在阶中，T上存在有界复测度$\theta$，使得$I(f) = \theta(f)$对于所有$f \in \mathscr{C}^b(T; \mathbf{C})$，I到B的限制对于紧致收敛的拓扑是连续的充要充分。那么测度 $\theta$ 是唯一的。

让我们证明叙述中的条件是必要的。令 $\theta$ 为 T 上的有界复测度，$\varepsilon$ 数 $> 0$，K 为 T 的紧凑子集，使得 $|\theta|^*(T - K) < \varepsilon$。设 $f \in B$；我们用U表示紧收敛的拓扑在B中$f$的邻域，由函数$g \in B$形成，使得$\sup_{x \in K} |g(x) - f(x)| \leq \varepsilon$。然后，对于每个 $g \in U$，

$$
|\theta(g) - \theta(f)| \leq \int_T |g - f| d|\theta| \leq \varepsilon |\theta|^*(K) + 2|\theta|^*(T - K) \leq (||\theta|| + 2)\varepsilon ,
$$

因为 $|g - f|$ 在 K 上以 $\varepsilon$ 为界，在 $T - K$ 上以 2 为界。

相反，考虑$\mathscr{C}^b(T; \mathbf{C})$上的线性形式I，其限制到B对于紧致收敛的拓扑是连续的。那么，对于每个数$\varepsilon > 0$，都存在数$a > 0$和T的紧凑子集K，使得关系$f \in B, \sup_{x \in K} |f(x)| \leq a$隐含$|I(f)| \leq \varepsilon$。 No. 2 的命题 5 意味着存在一个唯一的有界复数测度$\theta$，使得$I(f) = \theta(f)$ 对于所有$f \in \mathscr{C}^b(T; \mathbf{C})$。

#### 命题 13 {#int-ix-s5-prop-13 .statement tag=09RL}

— 设 T 为局部紧致空间，H 为范数空间 $\mathscr{C}^b(T; \mathbf{C})$ 的有界子集。 $\mathscr{M}_+^b(T) \times H$到$\mathbf{C}$的映射$(\mu, f) \mapsto \mu(f)$则连续，当$\mathscr{M}_+^b(T)$配备紧拓扑，且H与拓扑紧收敛。

令$\mu \in \mathscr{M}_+^b(T), f \in H$，并令M为实数，使得$||\mu|| < M$，以及对于所有$g \in H$为$|g| \leq M$。令 $\varepsilon$ 为数 $> 0$ 和选择 T 的紧致子集 K，使得 $\mu^*(T - K) < \varepsilon$，则为 K 的相对紧致开邻域 S。 集合 U 的测量 $\lambda \in \mathscr{M}_+^b(T)$ 满足不等式

$$
\lambda^*(T) < M , \quad \lambda^*(T - S) < \varepsilon , \quad |\lambda(f) - \mu(f)| < \varepsilon
$$

那么是 $\mathscr{M}_+^b(T)$ 中 $\mu$ 的邻域（No. 3，命题 6）。在加法中，令 V 为函数 $g \in H$ 的 H 由……组成中$f$ 的邻域，使得

$$
\sup_{x \in S} |g(x) - f(x)| < \varepsilon .
$$

设$\lambda \in U$和$g \in V$；因为函数 $|g - f|$ 在 $S$ 中以 $\varepsilon$ 为界，在 $T - S$ 中以 $2M$ 为界，所以我们有
$$
|\lambda(g) - \lambda(f)| \leq \int_T |g - f| d\lambda \leq \varepsilon \lambda^*(S) + 2M \lambda^*(T - S) \leq 3M \varepsilon,
$$
由此推论
$$
|\lambda(g) - \mu(f)| \leq |\lambda(g) - \lambda(f)| + |\lambda(f) - \mu(f)| \leq (3M + 1)\varepsilon.
$$
这就证明了映射$(\lambda, g) \mapsto \lambda(g)$在$\mathscr{M}_+^b(T) \times H$的点$(\mu, f)$的连续性。

#### 注 {#int-ix-s5-n6-rem-1 .statement tag=09RM}

设$T$是$\mathscr{M}^b(T)$的完全正则空间、$M$子集，满足普罗霍罗夫的条件、$H$和$C^b(T)$的有界子集。与刚才的论证非常接近的一个论证可以用来证明，当$M$配备了紧收敛的拓扑和$H$配备了紧收敛的拓扑时，$M \times H$到$\mathbf{C}$的映射$(\lambda, g) \mapsto \lambda(g)$是连续的。

#### 推出{#int-ix-s5-n6-cor-1 .statement tag=09RN}

*设$T$是一个完全正则的空间，$X$是一个拓扑空间，$f$是一个在$T \times X$上定义的复值函数，连续且有界。对于$T$上的每个有界测度$\mu$，令$F_\mu$为$X$上的函数，由$F_\mu(x) = \int_T f(t, x) d\mu(t)$对所有$x \in X$定义。

a) 函数 $F_\mu$ 是连续的，并且对于每个有界测度 $\mu$ 都是有界的。

b) 假设 $T$ 是局部紧致的。如果$\mathscr{M}_+^b(T)$配备了紧收敛的拓扑，并且$C^b(X; \mathbf{C})$配备了紧收敛的拓扑，则$\mathscr{M}_+^b(T)$到$C^b(X; \mathbf{C})$的映射$\mu \mapsto F_\mu$是连续的。

对于每个$x \in X$，用$f_x$表示$T$上连续且有界的函数$t \mapsto f(t, x)$； $X$到$C^b(T; \mathbf{C})$的映射$x \mapsto f_x$有界像，如果$C^b(T; \mathbf{C})$具备紧收敛的拓扑，则它是连续的（GT，X, §3, No. 4，Th.3）。由于 $F_\mu(x) = \mu(f_x)$，函数 $F_\mu$ 由命题 12 连续。假设 $T$ 是局部紧的；命题13表明，$\mathscr{M}_+^b(T) \times X$到$\mathbf{C}$的映射$(\mu, x) \mapsto F_\mu(x)$是连续的； 断言 b) 由此得出 (*loc.cit.*)。

### 7. 应用：拉普拉斯变换

在这个数中，我们用 $M$ 表示一个可交换幺半群，其合成的律是可加写的，配备有*局部紧凑* 空间的拓扑，其中 $M \times M$ 的映射 $(m, m') \mapsto m + m'$ 为$M$是连续的。 $M$的中性线元素用$0$表示。一个人在$M$满足关系上调用$M$的*特征标*每个有界连续复形函数$\chi$
$$
\chi(m + m') = \chi(m) \cdot \chi(m'), \quad \chi(0) = 1, \quad |\chi(m)| \leq 1
$$

$M$ 中的 $m, m'$。如果$\chi$和$\chi'$是特征标，那么$\chi \chi'$也是。 $M$的特征标的集合是幺半群，记为$X$；为其配备紧收敛的拓扑，其中$X \times X$到$X$的映射$(\chi, \chi') \mapsto \chi \chi'$是连续的。 $X$ 的中性线元素是常数函数 1。

对于 $M$ 上的每个有界复数测度 $\mu$，可在 $X$ 上调用 $\mu$ 函数 $\mathscr{L}\mu$ 的 *Laplace 变换*，定义为

$$
(\mathscr{L}\mu)(\chi) = \int_M \chi(m)\, d\mu(m).
$$

由 Th. GT中的3，$M \times X$到$\mathbf{C}$的X, §3, No. 4、映射$(m, \chi) \mapsto \chi(m)$是连续且有界的。 No. 6第13条命题的推论意味着以下结果：

#### 命题 14 {#int-ix-s5-prop-14 .statement tag=09RO}

*对于$M$上的每个有界复测度$\mu$，函数$\mathscr{L}\mu$在$X$上是连续且有界的。如果$\mathscr{M}_+^b(M)$配备紧拓扑和$\mathscr{C}^b(X; \mathbf{C})$与紧收敛的拓扑，$\mathscr{M}_+^b(M)$到$\mathscr{C}^b(X; \mathbf{C})$的映射$\mu \mapsto \mathscr{L}\mu$是连续的。*

$M$的特征标、集合在无穷大趋于0的情况记为$X_0$；这个集合在乘法下是稳定的。 我们可以说 $X$ 的子幺半群$^{(1)}$ S 是*满的*，如果 S 对于映射 $\chi \mapsto \overline{\chi}$ 稳定，$S \cap X_0$ 分离 $M$ 的点（GT，X, §4, No. 1，Def. 1），并且如果给定任何$m \in M$，存在$S \cap X_0$的元素$\chi$使得$\chi(m) \neq 0$。

假设在加法中，$M$ 是非紧阿贝尔的 *群*。令$f$为函数，在$M$上无穷远趋于0； $M$上的函数$x \mapsto f(x)f(-x)$也是如此，而$M$的每一个特征标$\chi$都满足$\chi(x)\chi(-x) = \chi(0) = 1$。由此可见，$X_0$是空的，并且$X$没有包含任何满的子幺半群。因此，下面的定理3不适用于局部紧凑的群，因为群不是紧致的。

#### 定理 3 {#int-ix-s5-thm-3 .statement tag=09RP}

*令 S 为 X 的完整子幺半群。*
a) *如果$\mu$和$\mu'$是$M$上的两个有界复数测度，使得$\mathscr{L}\mu$和$\mathscr{L}\mu'$具有相同的限制到$S \cap X_0$，则$\mu = \mu'$。*
b) *令$\mathfrak{F}$为$\mathscr{M}_+^b(M)$的过滤器，使得对于每个$s \in S$，$\mathscr{L}\lambda(s)$相对于$\mathfrak{F}$有极限$\Phi(s) \in \mathbf{C}$。然后，过滤器$\mathfrak{F}$模糊地收敛到有界正测度$\mu$，以及所有$s \in S \cap X_0$的$\Phi(s) = \mathscr{L}\mu(s)$。*
c) *在b)的假设下，假设在加法中，$S \cap X_0$包含1闭包，$S$上的函数$\Phi$在点1处连续。则$\mathfrak{F}$紧密收敛于$\mu$，以及所有$s \in S$的$\Phi(s) = \mathscr{L}\mu(s)$。*

我们用E 代数表示连续复数函数在$M$上趋向于无穷大的0，用$\mathfrak{A}$表示E生成的线性子空间

(1) 回想一下幺半群包含的子幺半群通过定义 A 的中性元素 (A, I, §2, No. 1)。

$S \cap X_0$；则$\mathfrak{A}$是$E$的子代数稳定在映射$f \mapsto \overline{f}$下；因为 $S$ 是 $X$ 的完整子幺半群，Cor。 GT 的第 7 条命题 2，X, §4, No. 4 意味着$\mathfrak{A}$ 在$E$ 中是稠密的。

让我们证明a)：对于每个$f \in \mathfrak{A}$，通过假设，$\mu(f) = \mu'(f)$；由于$\mu$和$\mu'$在$E$上是连续的线性形式，这意味着$\mu(f) = \mu'(f)$对于$f \in E$，特别是对于具有紧凑支持的每个连续函数$f$，从而$\mu = \mu'$。

让我们将自己置于 b) 的假设之下。 数$\Phi(1) = \lim_{\lambda, \mathfrak{F}} \lambda(1)$真实、积极；给定实数 $a > \Phi(1)$；由于$\| \lambda \| = \mathscr{L} \lambda(1)$对于$\lambda \in \mathscr{M}_+^b(M)$，关系$\lim_{\lambda, \mathfrak{F}} \mathscr{L} \lambda(1) = \Phi(1)$意味着集合$H$测量$\lambda \in \mathscr{M}_+^b(M)$，使得$\| \lambda \| \leq a$属于到$\mathfrak{F}$。由于 $\mathscr{M}^b(M; \mathbf{C})$ 可以与规范的空间 $E$ 等同（第 III, §1, No. 8 和 §1, No. 2，命题 3），空间 $H$ 对于拓扑 $\sigma(\mathscr{M}^b(M; \mathbf{C}), E)$ 是紧致的。另一方面（TVS，III, §3, No. 4，命题 5），$H$ 上的拓扑重合与拓扑的点向收敛在$E$ 的任何总子集中。特别是，由于$\mathfrak{A}$在$E$中是稠密的，并且对于具有紧支撑的连续函数的空间也是如此（第III, §1, No. 2，命题3），$S \cap X_0$重合中$H$的逐点收敛拓扑与模糊的拓扑，和$H$对于这个拓扑来说是紧凑的。由此可见，$\mathfrak{F}$ 模糊地收敛于$\mu \in H$，并且对于所有$s \in S \cap X_0$，$\mathscr{L} \mu(s) = \lim_{\lambda, \mathfrak{F}} \mathscr{L} \lambda(s)$。

最后，让我们转到c)。由于函数$\Phi$和$\mathscr{L} \mu$在点$1 \in S$连续，并且在$S \cap X_0$上相等，并且由于$1$在$S \cap X_0$的闭包中，所以我们有$\Phi(1) = \mathscr{L} \mu(1)$。其他字，$\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$。 No. 3 的第 9 条命题表明 $\mu$ 是过滤器 $\mathfrak{F}$ 的紧极限。 $S$的每个元素都是$M$上的有界连续函数，这意味着$\Phi(s) = \lim_{\lambda, \mathfrak{F}} \lambda(s) = \mu(s) = \mathscr{L} \mu(s)$对于所有$s \in S$。

#### 推论{#int-ix-s5-n7-cor-1 .statement tag=09RQ}

— *令$S$为$X$的完整子幺半群，使得$S \cap X_0$包含1的闭包。令$L$为限制的$\mathscr{C}^b(S; \mathbf{C})$由……组成到$S$的子集措施$\lambda \in \mathscr{M}_+^b(M)$的拉普拉斯变换。*

a) *集合$L$在配备拓扑逐点收敛的空间$\mathscr{C}^b(S; \mathbf{C})$中闭合。*

b) *映射 $\lambda \mapsto (\mathscr{L} \lambda)_S$ 是 $\mathscr{M}_+^b(M)$ 到 $L$ 的同胚，如果 $\mathscr{M}_+^b(M)$ 配备紧拓扑和$L$ 拓扑逐点收敛。*

c) *在$L$上点式收敛的拓扑和紧凑收敛重合的拓扑。*

断言 a) 和 b) 是 Th 的直接的推论。 3； 断言 c) 由 b) 和命题 14 得出，因为紧凑收敛的拓扑比逐点收敛的更细 。

必须警惕的是，L 在 S 上所有有界复形函数的集合中不是封闭的，配备了逐点收敛的拓扑。假设下面的例 2 的例记号（M = \mathbf{R}_+，S 用 \mathbf{R}_+ 标识）。措施$\varepsilon_n$（$n \in \mathbf{N}$）的拉普拉斯变换为$\mathbf{R}_+$上的函数$t \mapsto e^{-nt}$；由于$n$趋向于$+\infty$，这些函数逐点收敛到函数，对于$t = 0$等于1，对于$t \neq 0$等于0，而属于不会收敛到L。

*例 1).* — 取正整数的M集合N，配备加法的律和离散拓扑。设 D 为 \mathbf{C} 的单位圆盘（绝对值 $\leq 1$ 复数集合），配备由 \mathbf{C} 诱导的拓扑和由律诱导的乘法。对于每个$z \in D$，让我们用N的$f(z)$特征标$n \mapsto z^n$表示。对于N的每个特征标$\chi$，用$g(\chi)$复数$\chi(1) \in D$表示。我们立即验证$f$和$g$是D和X之间的互逆同胚，这将允许我们从现在开始到*认同*X和D。特征标在无穷远趋于0的集合可以被识别为绝对值<1的复数的集合$D_0$。最后，\mathbf{R}的区间]0, 1]是D的完整子幺半群，1在$]0, 1[ \cap D_0 = ]0, 1[$的闭包中。

N 上的每个测度 $\mu$ 都可以以唯一的方式写成形式 $\mu = \sum_{n \in \mathbf{N}} u_n \cdot \varepsilon^n$，并且 $\mu$ 是有界的当且仅当 $\sum_n |u_n| < +\infty$；那么就有 $\mathscr{L}\mu(z) = \sum_{n \in \mathbf{N}} u_n z^n$ 换 $z \in D$。这个函数在D上连续；习惯上称其为可和序列 $(u_n)_{n \in \mathbf{N}}$ 的 *生成的函数*。转录成这种语言，Th。 3 产生以下结果（考虑No. 3的第 9 条命题）：

#### 命题 15 {#int-ix-s5-prop-15 .statement tag=09RR}

*让 A 集合配备过滤器 $\mathfrak{F}$。对于每个$\alpha \in A$，令$(u_{\alpha,n})_{n \in \mathbf{N}}$为正数的可和序列，并令$\Phi_\alpha$为由$\Phi_\alpha(x) = \sum_{n \in \mathbf{N}} u_{\alpha,n} x^n$在\mathbf{R}的区间]0, 1]上定义的函数。在阶中，存在正数的可和序列$(u_n)_{n \in \mathbf{N}}$使得*

$$
\lim_{\alpha, \mathfrak{F}} u_{\alpha,n} = u_n \quad \text{for all } n , \quad \lim_{\alpha, \mathfrak{F}} \sum_{n \in \mathbf{N}} u_{\alpha,n} = \sum_{n \in \mathbf{N}} u_n ,
$$

*$\Phi_\alpha$在]0, 1[上逐点收敛，相对于$\mathfrak{F}$，到函数$\Phi$在点1连续。在这种情况下，$\Phi(x) = \sum_{n \in \mathbf{N}} u_n x^n$对于所有$x \in ]0, 1[$。*

取M为幺半群$\mathbf{N}^n$，可以得到类似的结果，其中$n$表示整数 > 1；然后，空间X可以被识别为$D^n$，并且可以将选择$]0, 1[^n$视为完整的子幺半群。我们把抄写 Th 的任务留给读者。在这种情况下为3。

例2)。 — 让我们以M 集合 $\mathbf{R}_+$为例，配备律或加法以及通常的拓扑。令 P 为复数 z 的集合，具有正实数部分，配备由 C 诱发的拓扑，并在 C 中配备由加法诱发的律。对于每个$p \in P$，用$\mathbf{R}_+$的$f(p)$特征标$x \mapsto e^{-px}$表示；容易验证，$f$是P的拓扑幺半群结构到X的同构；我们通过$f$将认同X与P。很明显，$\mathbf{R}_+$是P和Th的完整子幺半群。 3 产生以下结果：

#### 命题 16 {#int-ix-s5-prop-16 .statement tag=09RS}

*令A为集合，配备过滤器$\mathscr{F}$。对于每个$\alpha \in A$，令$\mu_\alpha$为$\mathbf{R}_+$上的有界正测度，并令$\Phi_\alpha$为由$\Phi_\alpha(p) = \int_0^{+\infty} e^{-px} d\mu_\alpha(x)$在$\mathbf{R}_+$上定义的函数。在阶中，映射$\alpha \mapsto \mu_\alpha$相对于$\mathscr{F}$紧密收敛到有界正测度$\mu$，$\Phi_\alpha$相对于$\mathscr{F}$在$\mathbf{R}_+$逐点收敛到函数$\Phi$是充分必要的在点 0 处连续。在这种情况下，$\Phi(p) = \int_0^{+\infty} e^{-px} d\mu(x)$ 对于所有 $p \in \mathbf{R}_+$。*

对于加法幺半群 $\mathbf{R}_+^n$ ($n$ 整数 $> 1$) 也有类似的结果；我们将 Th 的转录留给读者。在这种情况下为3。

### 习题{#int-ix-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
