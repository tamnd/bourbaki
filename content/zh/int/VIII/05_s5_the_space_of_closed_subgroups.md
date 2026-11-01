---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 5
section_title: The space of closed subgroups
lang: zh
source: int-vii-ix
book_pages: INT VIII.73-INT VIII.74
pdf_pages: 0146-0159, 0173-0174
extraction: ocr
subsections:
    - "no": 1
      title: The space of Haar measures on the closed subgroups of G
      page: 46
      pdf_page: 146
    - "no": 2
      title: Semi-continuity of the volume of the homogeneous space
      page: 48
      pdf_page: 148
    - "no": 3
      title: The space of closed subgroups of G
      page: 51
      pdf_page: 151
    - "no": 4
      title: The case of groups without arbitrarily small finite subgroups
      page: 53
      pdf_page: 153
    - "no": 5
      title: The case of abelian groups
      page: 55
      pdf_page: 155
    - "no": 6
      title: Another interpretation of the topology of the space of closed subgroups
      page: 56
      pdf_page: 156
statements: 20
exercises: 6
content_sha256: 54ff7caaa9a6594da6f459d592fa134125a35ca13bc03163d7c174c5214a8561
translated_from: content/en/int/VIII/05_s5_the_space_of_closed_subgroups.md
translation_method: google
source_content_sha256: 0d59b39eb609eb19a1cde4e7e71ffe935476923daecf7a76ec5c3f620241a549
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 9d18f016cc93278ca325b53ae22c5874dcd0b35c274b1fd9318aabdfeffe57b7
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 空间关闭子群

在整个截面中，G 表示局部紧致群和 $\mu$ G 上的右 Haar 测度。

### 1. G 关闭子群的 Haar 措施空间

#### 引理 1 {#int-viii-s5-lem-1 .statement tag=09LY}

令$\alpha$为$\neq 0$对G、S其支持度的正测度；以下两个条件是等价的：
a) S 是 G 的闭子群，并且 $\alpha$ 在 S 上引起的测度是 S 上的右 Haar 测度。
b) 每 $s \in S$ $\delta(s)\alpha = \alpha$。
此外，当满足这些条件时，$t \in G$的集合使得$\delta(t)\alpha = \alpha$等于S。
显然，a) 蕴涵 b)；相反，关系 b) 意味着对于每个 $x \in S$ 都有 $Sx = S$；在其他字，关系$x \in S$和$y \in S$意味着$y \in Sx$，或者再次意味着$yx^{-1} \in S$，并且由于S是非空，所以S是G的闭子群。$t \in G$的集合使得$St = S$则等于S本身，从而最后一个断言。

对于截面的其余部分，我们用$\Gamma$集合表示$\neq 0$对引理1的G满足条件的积极措施，并且对于每个$\alpha \in \Gamma$，我们用$H_\alpha$表示封闭的子群 G 的值就是 $\alpha$ 的支持度。

#### 命题 1 {#int-viii-s5-prop-1 .statement tag=09LZ}

集合$\Gamma$在空间$\mathscr{M}_+(G) - \{0\}$关闭，配备模糊拓扑。
我们首先证明以下引理：

#### 引理 2 {#int-viii-s5-lem-2 .statement tag=09M0}

令X为局部紧致空间，对于每个测度$\alpha \in \mathscr{M}_+(X) - \{0\}$，令$S_\alpha$为$\alpha$的支持。令 $\Phi$ 为 $\mathscr{M}_+(X) - \{0\}$ 上的过滤器，模糊地收敛到度量 $\alpha_0 \neq 0$。那么，对于$\alpha_0$支持的点s的每个邻域V，都存在集合$M \in \Phi$，这样，对于每一个$\alpha \in M$，都有$V \cap S_\alpha \neq \varnothing$。
因为，如果$\varphi \in \mathscr{K}_+(X)$是函数，并且V包含支持，并且$\int \varphi(x) d\alpha_0(x) > 0$，则到定义，存在集合$M \in \Phi$，使得$\int \varphi(x) d\alpha(x) > 0$对于所有$\alpha \in M$，这意味着$V \cap S_\alpha \neq \varnothing$。

#### 引理 3 {#int-viii-s5-lem-3 .statement tag=09M1}

令 E 为 $\Phi$ 过滤后的集合，并令 $\xi \mapsto \alpha(\xi)$ 为 E 的映射进入$\Gamma$，相对于 $\Phi$ 模糊地收敛到度量 $\alpha_0 \neq 0$。另一方面，让$\xi \mapsto t_\xi$是$E$到$G$的映射，这样每个$\xi \in E$都有$t_\xi \in H_{\alpha(\xi)}$。如果$s$是映射$\xi \mapsto t_\xi$相对于$\Phi$的簇点，则$\delta(s)\alpha_0 = \alpha_0$。

替换如果需要$\Phi$通过更细过滤，我们可以假设$s$相对于$\Phi$是$\xi \mapsto t_\xi$的极限；每$\xi \in E$乘以引理 1，$\delta(t_\xi)\alpha(\xi) = \alpha(\xi)$，结论来自映射$(u, \lambda) \mapsto \delta(u)\lambda$对$G \times \mathscr{M}_+(G)$的连续性（§ 3, No. 3，命题13）。

为了证明命题 1，通过引理 1 就足以表明，如果 $\Gamma$ 上的过滤器 $\Psi$ 模糊地收敛到测度 $\alpha_0 \neq 0$，并且如果 $s$ 属于支持$\alpha_0$，则$\delta(s)\alpha_0 = \alpha_0$。现在，对于$G$中$s$的每个邻域$V$，都存在一个$M \in \Psi$，这样，对于每个$\alpha \in M$，一个人有$V \cap H_\alpha \neq \varnothing$，通过引理2。对于$s$的每个邻域$V$和每个$\alpha \in \Gamma$，如果$V \cap H_\alpha \neq \varnothing$，则令$t_{V,\alpha}$为$V \cap H_\alpha$的点，反之则为$H_\alpha$的任意点；如果$\Theta$是$s$邻域过滤器的截面过滤器，并且$\Phi$是乘积过滤器$\Theta \times \Psi$，则根据前述，$s$是关于$(V, \alpha) \mapsto t_{V,\alpha}$的集群点 $\Phi$。另一方面，由于映射$(V, \alpha) \mapsto \alpha$的$\alpha_0$与$\Phi$的极限相同，因此从引理3可以得出命题。

#### 命题 2 {#int-viii-s5-prop-2 .statement tag=09M2}

— 令$\varphi$为$\mathscr{K}_+(G)$中的函数，使得$\varphi(e) > 0$。然后测量$\alpha \in \Gamma$的集合$\Gamma_\varphi$使得$\int \varphi(x)\,d\alpha(x) = 1$对于模糊拓扑来说是紧凑的。

集合$\Gamma_\varphi$是由$\alpha$形成的$\Gamma$的交和$\mathscr{M}(G)$的超平面，使得$\int \varphi(x)\,d\alpha(x) = 1$；由于这个超平面在$\mathscr{M}(G)$中模糊闭，并且包含不为0，因此从命题1可以得出$\Gamma_\varphi$在$\mathscr{M}(G)$中模糊闭。因此，只要证明对于$G$的每一个紧凑子集$K$，就有$\sup_{\alpha \in \Gamma_\varphi} \alpha(K) < +\infty$（第III, §1, No. 9章，第15条命题）。现在，令$U$为不等式$\varphi(x) > \varphi(e)/2$定义的$G$中$e$的开邻域；从 $1 = \int \varphi(x)\,d\alpha(x) \geq \int_U \varphi(x)\,d\alpha(x)$ 对应 $\alpha \in \Gamma_\varphi$ 开始，可以看到，在设定 $c = 2/\varphi(e)$，每 $\alpha \in \Gamma_\varphi$ 就有 $\alpha(U) \leq c$。设$V$是$e$在$G$中的对称开邻域，使得$V^2 \subset U$；让我们证明对于每个$x \in G$和每个$\alpha \in \Gamma_\varphi$都有$\alpha(Vx) \leq c$。事实上，如果$Vx$不与$\alpha$的支撑$H_\alpha$相交，那么这个关系是微不足道的；相反，如果存在 $h \in Vx \cap H_\alpha$，则对于某些 $v \in V$、从而存在 $h = vx$
$$
Vx = Vv^{-1}h \subset V^2h \subset Uh,
$$
从$\delta(h)\alpha = \alpha$开始，得出$\alpha(Vx) \leq \alpha(Uh) = \alpha(U) \leq c$。现在令$(x_i)_{1 \leq i \leq n}$为$K$的点的序列，使得$Vx_i$形式覆盖$K$；由前述可知，每$\alpha \in \Gamma_\varphi$对应$\alpha(K) \leq \sum_{i=1}^n \alpha(Vx_i) \leq nc$； Q.E.D.

#### 命题 3 {#int-viii-s5-prop-3 .statement tag=09M3}

— *根据第 2 条假设，映射* $\alpha \mapsto \left( \langle \varphi, \alpha \rangle, \frac{\alpha}{\langle \varphi, \alpha \rangle} \right)$ *是* $\Gamma$ *到乘积空间* $\mathbf{R}_+^* \times \Gamma_\varphi$ 的同胚。

由于映射 $\alpha \mapsto \langle \varphi, \alpha \rangle$ 是模糊连续的，因此只要观察到 $\langle \varphi, \alpha \rangle \neq 0$ 对于每个测度 $\alpha \in \Gamma$，从 $e$ 属于到 $\alpha$ 和 $\varphi(e) > 0$ 的支撑$H_\alpha$ 即可。

### 2. 齐次空间体积的半连续

在这个数字中，对于每一个措施$\alpha \in \Gamma$我们集合

$$
Q_\alpha = G / H_\alpha ,
$$

我们用$\pi_\alpha$典范映射$G \to Q_\alpha$表示。

令 $\Gamma^0$ 为由 $\alpha$ 测度形成的 $\Gamma$ 的子集，使得 $G$ 的子群 $H_\alpha$ 是*单模*； $\Gamma^0$的元素的特点是$\alpha(f) = \alpha(\dot{f})$对应于每个函数$f \in \mathscr{K}(G)$（$\mathscr{K}(H_\alpha)$的每个函数可以通过Urysohn的定理扩展到$\mathscr{K}(G)$的函数）；由此可见，$\Gamma^0$是$\Gamma$的*封闭*子集。回想一下，对于每个 $\alpha \in \Gamma^0$，$Q_\alpha$ 上的商度量 $\mu_\alpha = \mu / \alpha$ 已定义，并且在 $G$ 下相对不变（第 VII, §2, No. 6，第 3 章）；还记得对于每个函数 $f \in \mathscr{K}(G)$，

$$
\int_G f(x) d\mu(x) = \int_{Q_\alpha} d\mu_\alpha(\dot{x}) \int_{H_\alpha} f(xs) d\alpha(s) ,
$$

其中$\dot{x} = \pi_\alpha(x)$是$Q_\alpha$中$x \in G$的典范像。

#### 命题 4 {#int-viii-s5-prop-4 .statement tag=09M4}

— *让* $\Gamma^0$ *成为集合的测度* $\alpha \in \Gamma$ *使得* $H_\alpha$ *是幺模的，并且对于每个* $\alpha \in \Gamma^0$ *集合* $\mu_\alpha = \mu / \alpha$； *然后映射*$\alpha \mapsto \| \mu_\alpha \|$*of*$\Gamma^0$*进入*$\overline{\mathbf{R}}$*对于模糊拓扑*来说是下半连续。

对于每个 $\alpha \in \Gamma^0$ 和每个函数 $f \in \mathscr{K}(G)$、集合

$$
f_\alpha(\dot{x}) = \int_{H_\alpha} f(xs) d\alpha(s) = (f * \alpha)(x) ,
$$

其中卷积乘积是相对于正确的 Haar 测量 $\mu$ 进行的，并且利用了 $\dot{\alpha} = \alpha$ (§ 4, No. 4, 公式 (11)) 这一事实。我们知道（第VII, §2, No. 1，命题2）$\mathscr{K}_+(G)$到$\mathscr{K}_+(Q_\alpha)$的映射$f \mapsto f_\alpha$是*满射*；因而，通过(2)，

$$
\| \mu_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu_\alpha(f_\alpha) / \| f_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu(f) / \| f_\alpha \|,
$$

其中一个人有集合

$$
\|f_\alpha\| = \sup_{\dot{x} \in Q_\alpha} |f_\alpha(\dot{x})| = \sup_{x \in G} |(f * \alpha)(x)| .
$$

为了建立命题，只要证明给定$f \in \mathscr{H}_+(G)$，映射$\alpha \mapsto \|f_\alpha\|$是模糊连续的。现在，设 K 为 $f$ 的支持度； 函数$f * \alpha$的支持包含在$KH_\alpha$中，并且在$H_\alpha$下的右侧不变；因而

$$
\|f_\alpha\| = \sup_{x \in K} |(f * \alpha)(x)| .
$$

因而，结论是，配备模糊拓扑的$\mathscr{M}_+(G)$的映射$\alpha \mapsto f * \alpha$，到配备紧致收敛的拓扑的$\mathscr{C}(G)$，是连续的（§ 4, No. 2，注1）。

回想一下，如果对于测度 $\alpha \in \Gamma^0$，$\|\mu_\alpha\|$ 是有限的，则 G 必然是幺模的（Ch. VII, §2, No. 6，Th. 3 的 Cor. 3）。

#### 命题 5 {#int-viii-s5-prop-5 .statement tag=09M5}

*令g为$\mu$可积正数值函数，并令$\Gamma^0(g)$为$\alpha \in \Gamma^0$测度的集合，使得$\int^* g(xs)\, d\alpha(s) \geq 1$对于所有$x \in G$。那么$\Gamma^0(g)$到$\overline{\mathbf{R}}$的映射$\alpha \mapsto \|\mu_\alpha\|$是模糊连续的。*

对于每一个测量$\alpha \in \Gamma^0(G)$，请回忆（第VII, §2, No. 3，第 5 条命题）函数

$$
g_\alpha(\dot{x}) = \int_{H_\alpha} g(xs)\, d\alpha(s)
$$

定义为 $\mu_\alpha$ - $Q_\alpha$ 上几乎所有位置，$\mu_\alpha$ - 可积，并且

$$
\int_G g(x)\, d\mu(x) = \int_{Q_\alpha} g_\alpha(\dot{x})\, d\mu_\alpha(\dot{x}) .
$$

根据命题4，只需证明，在$\Gamma^0(g)$中，$\alpha \mapsto \|\mu_\alpha\|$是*上*半连续的。固定测度$\alpha \in \Gamma^0(g)$，令K为G的紧子集。$Q_\alpha$上存在紧支撑的连续函数，取其在$[0, 1]$中的值，在紧集$\pi_\alpha(K)$上等于1；由于 $\mathscr{H}_+(G)$ 到 $\mathscr{H}_+(Q_\alpha)$ 的映射 $f \mapsto f_\alpha$ 是满射（第 VII, §2, No. 1，命题 2），因此可以看出存在函数 $f \in \mathscr{H}_+(G)$，使得

$$
(f * \alpha)(x) = \int_G f(xs)\, d\alpha(s) \left\{ \begin{array}{ll}
\leq 1 & \text{for all } x \in G \\
= 1 & \text{for all } x \in K .
\end{array} \right.
$$

由于$\beta \mapsto f * \beta$是$\mathscr{M}_+(G)$的连续映射，配备了模糊的拓扑，进入$\mathscr{C}(G)$配备了紧致收敛的拓扑（§ 4, No. 2，注1），可以看到对于每一个$\varepsilon > 0$， 集合 $U_\varepsilon$ / $\beta \in \Gamma^0(G)$ 使得
$$
f_\beta(\dot{x}) = \int_G f(xs)\, d\beta(s) > 1 - \varepsilon \quad \text{for all } x \in K
$$
是$\Gamma^0(g)$中$\alpha$的开放邻域；对于每一个 $\beta \in U_\varepsilon$，我们凭借公式 (2)，
$$
(5) \quad \| \mu_\alpha \| \geq \int_G f(x)\, d\mu(x) = \int_{Q_\beta} f_\beta(\dot{x})\, d\mu_\beta(\dot{x}) \geq (1 - \varepsilon) \mu_\beta(\pi_\beta(K)).
$$
给定数$\varepsilon > 0$，让我们选择函数$h \in \mathscr{K}_+(G)$这样$\int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon$，并让我们在前面的$K = \mathrm{Supp}(h)$中取。对于每个 $\beta \in \Gamma^0(g)$，假设 $g_\beta(\dot{x}) \geq 1$ $Q_\beta$ 中几乎所有地方（对于 $\mu_\beta$），因此
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{Q_\beta - \pi_\beta(K)} g_\beta(\dot{x})\, d\mu_\beta(\dot{x}) = \int_{G - KH_\beta} g(x)\, d\mu(x)
$$
凭借（4）；由于$h$在$K$之外是零，并且$a fortiori$在$KH_\beta$之外，因此
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{G - KH_\beta} |g(x) - h(x)|\, d\mu(x) \\
\leq \int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon;
$$
将此结果与 (5) 结合起来，可以看出
$$
\| \mu_\beta \| \leq \varepsilon + \| \mu_\alpha \|/(1 - \varepsilon)
$$
当$\beta \in U_\varepsilon$时，完成证明。

#### 推论 1 {#int-viii-s5-prop-5-cor-1 .statement tag=09M6}

— 令 $K$ 为 $G$ 的紧致子集，$V$ $G$、$c$ 实数 $> 0$ 中 $e$ 的对称紧邻邻域。 映射$\alpha \mapsto \| \mu_\alpha \|$的限制到$\alpha \in \Gamma^0$的集合，使得$G = KH_\alpha$和$\alpha(V) \geq c$是模糊连续的。

例如，令$g \in \mathscr{K}_+(G)$为函数，使得$g(x) \geq 1/c$对应$x \in KV$。每$x \in K$，
$$
\int g(xs)\, d\alpha(s) \geq \int_V g(xs)\, d\alpha(s) \geq 1
$$

对于叙述的 $\alpha$ 满足条件；此外，由于$\pi_\alpha(K) = Q_\alpha$，有$\alpha \in \Gamma^0(g)$、从而的推论。

#### 推论 2 {#int-viii-s5-prop-5-cor-2 .statement tag=09M7}

*设 A 是 G 的 $\mu$ 可积子集。 G 的离散子群 H 的归一化 Haar 测量的映射 $\alpha \mapsto \| \mu_\alpha \|$ 到集合 $N_A$ 的限制，使得 $G = AH$ 是模糊连续的。*

对于 $a \in A$ 和 $\alpha \in N_A$，

$$
\int \varphi_A(as)\ d\alpha(s) \geq \varphi_A(a) = 1,
$$

并且从 $\pi_\alpha(A) = Q_\alpha$ 开始，就有 $N_A \subset \Gamma^0(\varphi_A)$，因此由命题 5 得出推论。

### 3. G 的空间闭合子群

让我们用G的*闭子群*的$\Sigma$集合来表示；如果将 $\alpha \in \Gamma$ 子群 $H_\alpha$ 的每个测度关联起来，即$\alpha$ 的支持，则可以将 $\Gamma$ 的映射（称为规范）转化为 $\Sigma$，这显然是满射的，并且允许规范地识别 $\Sigma$ 与集合 $\Gamma$ 中同位的群的轨道与比率 $> 0$。 集合$\Sigma$，配备模糊拓扑在$\Gamma$上的商拓扑，称为G的闭子群*的*空间。

#### 定理 1 {#int-viii-s5-thm-1 .statement tag=09M8}

*设 G 为局部紧致群。 G 的闭子群的空间$\Sigma$是紧的。此外，它还具有以下特性：*

(i) *G 的单模闭子群的集合$\Sigma^0$在$\Sigma$中闭（因此是紧的）。*

(ii) *如果 G 由 e 的紧邻域生成，则 G 的单模闭子群 H 的集合 $\Sigma_c^0$ 使得商空间 $G/H$ 是紧的，在 $\Sigma^0$ 中开（因此是局部紧的）。*

(iii) *对于 G 中 e 的每个相对紧开邻域 U，G 的离散子群 H 的集合 $D_U$，使得 $H \cap U = \{e\}$ 在 $\Sigma^0$ 中闭合（因此是紧致的）。*

由No. 1的命题3可知，$\Sigma$同胚于$\Gamma_\varphi$，因此由No. 1的命题2紧致。此外，在No. 2的开头注意到，$\alpha \in \Gamma$的测度集合$\Gamma^0$使得$H_\alpha$是幺模，在$\Gamma$中是封闭的；由于$\Gamma^0$在与$> 0$的同位比下是稳定的，$\Sigma$中$\Gamma^0$的像$\Sigma^0$是$\Sigma$的闭子集，从而证明(i)。

性质 (ii) 将是以下命题中的推论：

#### 命题 6 {#int-viii-s5-prop-6 .statement tag=09M9}

*假设局部紧致群 G 由 e 的紧邻域生成。那么使得$G/H_\alpha$紧的测度$\alpha \in \Gamma^0$*的集合$\Gamma_c^0$在$\Gamma^0$中开，并且映射$\alpha \mapsto \| \mu_\alpha \|$的限制到$\Gamma_c^0$是模糊连续的。

根据No. 2的第5条命题记号，对于$g \in \mathscr{K}_+(G)$，我们有，

$$
\Gamma^0(g) \subset \Gamma_c^0.
$$

因为，如果K是$g$的支持，关系$\int g(xs)\, d\alpha(s) \geq 1$对于所有$x \in G$意味着$KH_\alpha = G$，积分显然是$KH_\alpha$的补集零，因此$G/H_\alpha = \pi_\alpha(K)$是紧的。给定测度$\alpha \in \Gamma_c^0$，因此足以满足定义函数$g \in \mathscr{K}_+(G)$，使得$\Gamma^0(g)$是$\Gamma^0$中$\alpha$的邻域。由于 $G/H_\alpha$ 是紧致的，并且 $\mathscr{K}_+(G)$ 到 $\mathscr{K}_+(G/H_\alpha)$ 的典范映射 $f \mapsto f_\alpha$ 是满射（第 VII, §2, No. 2 章），因此存在函数 $g \in \mathscr{K}_+(G)$，使得 $\int g(xs)\, d\alpha(s) = 2$ 对于*每个* $x \in G$。令 K 为$g$、L e 在 G 中的对称紧邻域，生成 G； $\mathscr{M}_+(G)$的映射$\beta \mapsto g * \beta$进入$\mathscr{C}(G)$是模糊连续的（§ 4, No. 2，*注*1），$\Gamma^0$中存在$\alpha$的邻域W，使得

$$
(g * \beta)(x) = \int g(xs)\, d\beta(s) \geq 1
$$

对于所有 $\beta \in W$ 和 $x \in LK$。 (7) 的第一个成员等于 $KH_\beta$ 之外的零，关系 $\beta \in W$ 意味着

$$
LK \subset KH_\beta,
$$

由此可以推断，通过$n$上的归纳，每整数$n > 0$对应$L^n K \subset KH_\beta$；由于 L 生成 G，因此对于每个度量$\beta \in W$，我们都有 $G = KH_\beta$，这证明了 $W \subset \Gamma_c^0$。另一方面，(7)的第一个成员在$H_\beta$右端不变，不等式(7)对于$x \in LKH_\beta = G$也有效；因此$W \subset \Gamma^0(g)$，证明命题。

最后，(iii) 将是以下命题中的推论：

#### 命题 7 {#int-viii-s5-prop-7 .statement tag=09MA}

*令$N \subset \Gamma^0$为G的离散子群上的归一化哈尔测度的子空间，并且对于G中e的每个相对紧开邻域U，令$N_U$为由$\alpha$形成的N的子集，使得$H_\alpha \cap U = \{e\}$。然后：
a) $N_U$ 是紧凑的。
b) N 形式中集合 $N_U$ 的内部是 N 的覆盖，因为 U 运行在 G 中 e 的相对紧凑的开放邻域的集合上。
c) 为了使 N 的子集 M 在 N 中相对紧，必要且充分的是，G 中存在 e 的相对紧开邻域 U，使得 $M \subset N_U$。*

由于在 Th 的规范连续映射 $\Gamma \to \Sigma$、断言 (iii) 下，$D_U$ 是 $N_U$ 的像。 1 将立即由提案 7 a) 得出。

为了证明第 7 条，我们观察到 $N_U$ 可以定义为由 $\alpha$ 形成的 $\Gamma^0$ 的子集，这样，

$$
\alpha(\{e\}) \geq 1 \quad \text{and} \quad \alpha(U) \leq 1.
$$

现在，如果 $G$ 中的 $A$ 是紧致的（或开放且相对紧致的），则 $\mathscr{M}_+(G)$ 到 $\mathbf{R}$ 的映射 $\alpha \mapsto \alpha(A)$ 对于模糊拓扑是上（或下）半连续（第 IV, §4, No. 4 章，第 5 条的 Cor. 3 和前述，§1, No. 1，提案 4）；因此我们看到$N_U$是$\Gamma^0$的闭子集。此外，令$\varphi \in \mathscr{K}_+(G)$为函数，使得$\varphi(e) = 1$和$\varphi(x) = 0$在$G - U$上；很明显，$\int \varphi(x) d\alpha(x) = 1$对于所有$\alpha \in N_U$；因此No. 1的命题2表明$N_U$是紧集，这就证明了a)。另一方面，让$V$是$G$中$e$的相对紧凑的开放邻域，使得$\overline{V} \subset U$，并让$\varphi \in \mathscr{K}_+(G)$，支持包含在$U$中，使得$\varphi(x) = 1$在$V$上。那么$\alpha(\varphi) = 1$对应$\alpha \in N_U$，因此在$N$中存在$\alpha$的邻域$W$，使得$\beta(\varphi) < 2$对应$\beta \in W$；显然$W \subset N_V$，因此$N_V$是$N_U$的邻域。由于$N_U$覆盖了$N$，这就证明了b)。最后，$N$的每个紧凑子集$M$都包含在集合$N_{U_i}$（$1 \leq i \leq n$）的有限并中，并且从$\bigcup_i N_{U_i} \subset N_U$开始，其中$U = \bigcap_i U_i$，这证明了c）。

#### 推论{#int-viii-s5-n3-cor-1 .statement tag=09MB}

— *子空间* $N$ *of* $\Gamma^0$ *局部紧凑*。

### 4. 群无任意小有限子群的情况

#### 定理 2 {#int-viii-s5-thm-2 .statement tag=09MC}

— *让* $G$ *成为以下群满足的局部紧致条件*：
（L）*在*$G$*中存在*$e$*的邻域，即包含没有有限的子群*$G$*不减少到*$e$。
*以下属性保持*：
(i) *集合* $D$ *离散子群的* $G$ *局部闭于* $\Sigma$ *（相当于说局部紧致）*。
(ii) *对于一个封闭的子集* $A$ *of* $D$ *为了紧凑，存在一个邻域* $U$ *of* $e$ *在* $G$ *使得* $H \cap U = \{e\}$ *对于每个子群* $H \in A$。
(iii) *如果在加法* $G$ *由 * $e$ 的紧邻邻域生成，*则集合* $D_c$ *为离散子群* $H$ *为* $G$ *使得* $G/H$ *是紧致的局部封闭于* $\Sigma$ *（因此是局部紧凑的）*。

我们有 $D_c = D \cap \Sigma_c^0$，因此 (iii) 是 (i) 的推论，并且 Th。 1 (ii) No. 3。

对于No. 3的记号，第7条命题，对于证明 (i) 和 (ii) 来说，足以证明：

#### 命题 8 {#int-viii-s5-prop-8 .statement tag=09MD}

*N 到 D 的规范双射是同胚。*

现在，如果$\Gamma_d$是$G$的离散子群上的Haar测度的集合，则$D$与$\Gamma_d$中同调的群轨道空间与比率标准同胚$> 0$（GT，I, §5, No. 2，提案 4）。因此，只要证明$\Gamma_d$到$\mathbf{R}_+^* \times \mathbf{N}$的典范映射$\alpha \mapsto (\alpha(\{e\}), \alpha/\alpha(\{e\}))$是*同胚*，这将由以下引理得出：

#### 引理 4 {#int-viii-s5-lem-4 .statement tag=09ME}

*如果群G满足条件(L)，则$\Gamma_d$到$\mathbf{R}_+^*$的映射$\alpha \mapsto \alpha(\{e\})$是模糊连续的。*

让我们考虑一个度量$\alpha \in \Gamma_d$；令$V_0$是$G$中$e$的相对紧邻开邻域，使得$H_\alpha \cap V_0 = \{e\}$并且不存在$V_0$中包含的$G$的有限子群并且不减少到$e$。令 $V$ 为 $e$ 的对称紧邻域，使得 $V^3 \subset V_0$，令 $U$ 为 $e$ 的对称邻域，使得 $U^2 \subset V$。设$\varphi$（分别为$\psi$）在$\mathscr{H}_+(G)$中为函数，$[0, 1]$中的值等于$V^3$（分别在点$e$）上的1，并且支持包含在$V_0$（分别在$U$）。 集合测量$\beta \in \Gamma_d$，使得$|\beta(\varphi) - \alpha(\varphi)| \leq \varepsilon$和$|\beta(\psi) - \alpha(\psi)| \leq \varepsilon$是$\alpha$的邻域$W$。我们建议证明，只要 $\varepsilon$ 足够小，$H_\beta \cap V = \{e\}$ *对于每个* $\beta \in W$；然后它会遵循$\beta(\psi) = \beta(\{e\})$，因此$|\beta(\{e\}) - \alpha(\{e\})| \leq \varepsilon$，这将证明引理。

足以证明，对于 $\beta \in W$，

$$
(V^2 - V) \cap H_\beta = \varnothing.
$$

对于，假设这个点成立：那么，对于$V \cap H_\beta$中的$x$和$y$，有$xy^{-1} \in V^2 \cap H_\beta$；但是，根据 (8)，这意味着 $xy^{-1} \in V \cap H_\beta$；在其他字中，$V \cap H_\beta$是$G$的*子群*，显然是离散且紧致的，因此是有限的；但是，通过$V_0$的选择，这意味着确实是$V \cap H_\beta = \{e\}$。

让我们用反证法来论证，假设存在$V^2 - V$中的点$z$即属于到$H_\beta$；通过$U$和$V$的选择，我们在$G$中有$\psi(sz^{-1}) + \psi(s) \leq \varphi(s)$，关系$z \notin U^2$意味着$Uz \cap U = \varnothing$。自从

$$
\int \psi(sz^{-1})\, d\beta(s) = \int \psi(s)\, d\beta(s),
$$

由此可见 $2\beta(\psi) \leq \beta(\varphi) \leq \alpha(\varphi) + \varepsilon$；但我们也有
$$
\beta(\psi) \geq \alpha(\psi) - \varepsilon,
$$
以及构造$\alpha(\varphi) = \alpha(\psi) = \alpha(\{e\})$。因此，我们通过取 $\varepsilon < \alpha(\{e\})/3$ 来得出矛盾。 Q.E.D.

在图形项中，群$G$满足条件（L）据说*不具有任意小的有限子群。*可以证明每个李群满足条件 (L);但这个条件不是李群的特性；对于例，$p$-adic 整数的乘法群全等于 1 mod $p$ 满足 (L)。*

### 5. 阿贝尔群的情形

令$G$为$G$的离散子群上的归一化哈尔测度的局部紧凑群、$N \subset \Gamma^0$子空间，以及$N$相应的的离散子群的$N_c$子集 $G$的$H$使得$G/H$是*紧凑*；因此No. 3的记号中的$N_c = N \cap \Gamma_c^0$，提案6；如果群 $G$ 是由 $e$ 的紧邻域生成的，则根据第 6 条命题 No. 3，$N_c$ 在 $N$ 中是“开*”（因此由第 7 条命题的 No. 3 是“局部紧致”）并且映射 $\alpha \mapsto \| \mu_\alpha \|$ 的限制到 $N_c$ *模糊连续*。

#### 命题 9 {#int-viii-s5-prop-9 .statement tag=09MF}

*令 $G$ 为局部紧致阿贝尔的群，由 $e$ 的紧致邻域生成。为了使$N_c$的子集$A$在$N_c$中相对紧凑，满足以下两个条件是充分必要的：*

(i) *在$G$中存在$e$的开放邻域$U$，使得$H_\alpha \cap U = \{e\}$对于所有$\alpha \in A$。*

(ii) *存在一个常数 $k$，使得 $\mu_\alpha(G/H_\alpha) \leq k$ 对于所有 $\alpha \in A$。*

如果$A \subset N_c$在$N_c$中相对紧凑，那么在$N$中它是*更不必说*，因此条件（i）和（ii）的必要性从No. 3得出，道具。 6 和 7（不假设 $G$ 为阿贝尔的）。相反，假设$A \subset N_c$满足这些条件；如果 $\overline{A}$ 是 $A$ *in* $N$ 的闭包，那么 $\overline{A}$ 根据第 7 条命题 No. 3 是紧的；此外，由于对于模糊的拓扑（No. 2，命题4），$\alpha \mapsto \| \mu_\alpha \|$在$\Gamma^0$上是下半连续的，条件(ii)意味着对于所有$\alpha \in \overline{A}$也有$\| \mu_\alpha \| \leq k$。现在，由于$G$是阿贝尔的，$\mu_\alpha = \mu/\alpha$是群$G/H_\alpha$的哈尔测度，因此$G/H_\alpha$对于每个$\alpha \in \overline{A}$都是紧凑的（第VII, §1, No. 2，第2条）。这意味着$\overline{A} \subset N_c$，因此$A$在$N_c$中相对紧凑。

#### 推论{#int-viii-s5-n5-cor-1 .statement tag=09MG}

*令 $G$ 为局部紧致阿贝尔的群，由 $e$ 和满足条件 (L) 的 No. 4 的紧致邻域生成。*

令 $D_c$ 为 $G$ 的离散子群 $H$ 的集合，使得 $G/H$ 是紧致的，对于每个 $H \in D_c$，令 $v(H)$ 为总质量 $\mu_\alpha(G/H)$，其中 $\mu_\alpha$ 为$\mu$ 通过标准化 Haar 测量$\alpha$ $H$。为了使空间$D_c$中的子集$A$在$D_c$中相对紧凑，满足以下两个条件是充分必要的：

(i) $G$ 中存在$e$ 的开放邻域$U$，使得$H \cap U = \{e\}$ 对于所有$H \in A$。

(ii) 存在一个常数 $k$，使得 $v(H) \leq k$ 对于所有 $H \in A$。

考虑到第 9 条命题，这可以立即得出以下事实：在 $N$ 到 $D$ 的规范双射下，$D_c$ 是 $N_c$ 的像，并且根据所做出的假设，这个双射是同胚（No. 4，提案 8）。

#### 例 {#int-viii-s5-n5-exa-1 .statement tag=09MH}

让我们采用 $G = \mathbf{R}^n$，对于$\mu$，采用勒贝格测度； Cor 的所有假设。提案 9 的满足。使得$G/H$紧致的$G$的离散子群$H$正是*秩*$n$的离散子群（GT，VII, §1, No. 1，Th.1）；这样子群$H$是由$\mathbf{R}^n$的基$(a_i)_{1 \leq i \leq n}$生成的，并且

$$
v(H) = |\det(a_1, \ldots, a_n)|
$$

（行列式是针对典范基或$\mathbf{R}^n$而取的）（第VII, §2, No. 10，第4章）。 空间$D_c$在这里可以这样解释：每个子群$H \in D_c$是子群$\mathbf{Z}^n$的变换$g \cdot \mathbf{Z}^n$除以元素$g \in \mathbf{GL}(n, \mathbf{R})$，以及子群使$\mathbf{Z}^n$稳定的$\mathbf{GL}(n, \mathbf{R})$可以用$\mathbf{GL}(n, \mathbf{Z})$来识别。因而，$D_c$可以被规范地识别为（非拓扑）齐次空间，与$\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$。另一方面，$\mathbf{GL}(n, \mathbf{R})$在$\mathbf{R}^n$中连续运行，因此对于模糊的拓扑（§3, No. 3，命题13）也在$\mathscr{M}_+(\mathbf{R}^n)$中运行，因此在$\mathscr{M}_+(\mathbf{R}^n)$的子空间$N_c$中运行；此外，$N_c$到$D_c$的规范同胚（No. 4，命题8）与$\mathbf{GL}(n, \mathbf{R})$的运算的律兼容。由于$\mathbf{GL}(n, \mathbf{R})$在无穷大处可数并且$D_c$是局部紧致的，因此上面定义的$\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$到$D_c$的双射是一个*同胚*（Ch.VII，App.I，引理2）。科。因而，第 9 条命题给出了齐次空间 $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$ 中紧致性的标准。

### 6. 另一个关闭子群空间拓扑的解释

设$\mathfrak{F}$为$G$闭子集的集合； $\mathfrak{F}$ 上的一个定义 a *Hausdorff 均匀结构* 的方式如下：对于 $G$ 的每一个紧凑子集 $K$ 以及 $G$ 中 $e$ 的每个邻域 $V$，令 $P(K, V)$ 为集合对 $(X, Y)$ 元素 $\mathscr{F}$ 使得两者

$$
(9) \quad X \cap K \subset VY \quad \text{and} \quad Y \cap K \subset VX.
$$

让我们证明，$P(K, V)$ 的集合是 Hausdorff 制服结构 $\mathscr{U}$ $\mathscr{F}$ 的基本随从人员系统。 GT的公理$(U'_I)$和$(U'_{II})$，II, §1, No. 1显然很满意；此外，关系$K \subset K'$和$V' \subset V$意味着$P(K', V') \subset P(K, V)$；为了验证$(U'_{III})$，我们可以将极限自身化为$V$是$e$的对称紧邻域，从而$VK$是紧的。假设$(X, Y) \in P(VK, V)$和$(Y, Z) \in P(VK, V)$；那么$X \cap K \subset X \cap VK \subset VY$，如果$y \in Y$对于某些$v \in V$来说是这样的$vy \in K$，那么必然是$y \in VK$，因此

$$
X \cap K \subset V(Y \cap VK);
$$

另一方面，$Y \cap VK \subset VZ$，从而$X \cap K \subset V^2Z$，并且类似地显示$Z \cap K \subset V^2X$，从而证明$(U'_{III})$。最后，如果$X, Y$是$\mathscr{F}$的两个不同的元素，则存在例点$a \in X$使得$a \notin Y$，因此$e$的对称紧邻域$V$使得$Va \cap Y = \varnothing$，即， $a \notin VY$； *更不必说* $(X, Y) \notin P(Va, V)$，完成我们的断言的证明。

至此成立，让我们考虑一下刚才定义的均匀空间$\mathscr{F}$的拓扑所诱发的$G$拓扑$\mathscr{T}$的封闭子群的集合$\Sigma$。我们将看到这个拓扑*与No. 3*中定义的拓扑相同。只要证明当$\Sigma$配备拓扑$\mathscr{T}$时，$\Gamma$到$\Sigma$的映射$\alpha \mapsto H_\alpha$是*连续的*：因为，对于这个映射的限制来说，同样如此$\Gamma_\varphi$（与No. 1，命题 2 中的记号一样），它是双射的；但由于$\Gamma_\varphi$是紧的，并且拓扑$\mathscr{T}$是分离的，$\Gamma_\varphi$的映射$\alpha \mapsto H_\alpha$进入$\Sigma$将是同胚。

因此，令$\alpha_0$为$\Gamma$的点，并令$\Phi$为$\Gamma$上的过滤器，收敛于$\alpha_0$；我们要证明，对于$\Phi$，对于拓扑$\mathscr{T}$，$H_\alpha$趋向于$H_{\alpha_0}$。设$K$是$G$的紧子集，$V$是$e$在$G$的对称紧邻域；对于每一个$x \in H_{\alpha_0} \cap K$，都存在集合$M(x) \in \Phi$，这样对于每一个$\alpha \in M(x)$，就有$Vx \cap H_\alpha \neq \varnothing$（No. 1，引理2），从而$Vx \subset V^2H_\alpha$；当用集合 $Vx_i$ 的有限数覆盖 $H_{\alpha_0} \cap K$ 时，我们会发现，如果 $M = \bigcap_i M(x_i)$，则对于每个 $\alpha \in M$ 都有 $H_{\alpha_0} \cap K \subset V^2H_\alpha$。

相反，假设$G$中存在$e$的开邻域$U$，使得对于每一个集合$L \in \Phi$，至少有一个$\alpha \in L$对应$H_\alpha \cap K \not\subset UH_{\alpha_0}$；如果$\omega(L)$是$\alpha \in L$的集合且具有该性质，则$\omega(L)$将是$\Phi'$在$\Gamma$更细上的过滤器形式基比$\Phi$，并且，对于每个对于$L \in \Phi$，$\omega(L)$的$\alpha$属于到并$E$，将存在$t_\alpha \in H_\alpha \cap K$而不是属于到$UH_{\alpha_0}$；对于$\alpha \notin E$，取$H_\alpha$中的任何点作为$t_\alpha$。由于$K \cap C(UH_{\alpha_0})$是紧的，因此相对于$\Phi'$、属于到$K \cap C(UH_{\alpha_0})$，将存在$\alpha \mapsto t_\alpha$的簇点$s$；但由于$\Phi'$在$\Gamma$中收敛到$\alpha_0$，因此No. 1的与……矛盾引理 3。

习题

### 习题{#int-viii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
