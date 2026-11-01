---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 4
section_title: Passage from Lie algebras to Lie groups
lang: zh
source: lie-i-iii
book_pages: 279-297, 376-382
pdf_pages: 0297-0315, 0394-0400
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 279
      pdf_page: 297
    - "no": 2
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 281
      pdf_page: 299
    - "no": 3
      title: EXPONENTIAL MAPPINGS
      page: 284
      pdf_page: 302
    - "no": 4
      title: FUNCTORIZATION OF EXPONENTIAL MAPPINGS
      page: 288
      pdf_page: 306
    - "no": 5
      title: STRUCTURE INDUCED ON A SUBGROUP
      page: 289
      pdf_page: 307
    - "no": 6
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 291
      pdf_page: 309
    - "no": 7
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 294
      pdf_page: 312
statements: 40
exercises: 13
content_sha256: 3508f09abc0d5c58893e87c3f1b1017c87f03935ca08a5d6911da55d667aa055
translated_from: content/en/lie/III/04_s4_passage_from_lie_algebras_to_lie_groups.md
translation_method: google
source_content_sha256: ac80217cc327976168394892cdf7db00cf39b8b242f761fd1c03f5a44ca03e51
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: bf39d96d52655814b5574cecc987d25b979d0ea71c122a1454747d4509906515
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。从李代数到李群的通道

回想一下，直到章结束，K 都被假设为特征 0。

### 1. 从李代数态射到李群态射

#### 引理 1 {#lie-iii-s4-lem-1 .statement tag=0ACK}

*设 G 为李群胚芽，$\mathfrak{h}$是$L(G)$的谎言子代数，承认拓扑补充。 $g \in G$ 的 $g\mathfrak{h}$（或 $\mathfrak{h}g$）的并是 $T(G)$ 的可积向量子束。*

通过考虑 $T(G)$ (§ 2, no. 3) 的左平凡化，立即可见$g \in G$的$g\mathfrak{h}$是$T(G)$的向量子束E的纤维。让$g \in G$。 $(L_a)_g$的集合，其中$a \in \mathfrak{h}$等于$g\mathfrak{h}$。现在，如果$a$和$b$属于到$\mathfrak{h}$，那么$[L_a, L_b] = L_{[a, b]}$和$[a, b] \in \mathfrak{h}$。因此 E 是可积的（*可微且解析流形*, R, 9.3.3 (iv)）。 $\mathfrak{h}g$ 的论证类似。

$g\mathfrak{h}$（或$\mathfrak{h}g$）的并的积分叶化（*可微分和解析流形*，R，9.3.2）被称为与$\mathfrak{h}$相关的G的*左*（或*右*）*叶化*。

#### 定理 1 {#lie-iii-s4-thm-1 .statement tag=0ACL}

*设G和H为李群细菌，f为$L(G)$到$L(H)$的连续态射。
(i) 存在 G 的开李子群胚$G'$和$G'$的态射$\phi$进入H，使得$f = L(\phi)$。
(ii) 设$G_1, G_2$开，将G的子群胚芽和$G_i$的$\phi_i$态射放入H中，使得$f = L(\phi_i)$为$i = 1, 2$。然后是 e 的邻域上的 $\phi_1$ 和 $\phi_2$ 重合。
让 $p_1 : G \times H \to G, p_2 : G \times H \to H$ 成为规范的投影。对于所有$(g, h) \in G \times H$，令$f_{g, h}$为$T_g(G) = gL(G)$的映射$ga \mapsto hf(a)$到$T_h(H) = hL(H)$。通过考虑$T(G)$和$T(H)$的左平凡化，可以立即看出$p_1^*T(G)$的$f_{g, h}$定义态射变成*$p_2^*T(H)$。令$a$为$f$的图；它是 $L(G) \times L(H)$ 的闭合谎言子代数，承认 $\{0\} \times L(H)$ 是拓扑补充。对于所有$(g, h) \in G \times H$，$f_{g,h}$的图是$(g, h) \cdot a$。这些图中的并是$T(G \times H)$（引理1）的可积向量子丛。那么存在（可微且解析流形，R，9.3.7）$G$中$e_G$的开邻域$U$和$U$的解析映射$\phi$进入$H$这样$\phi(e_G) = e_H$ 和 $T_g(\phi) = f_{g, \phi(g)}$ 对于所有 $g \in U$。特别是$T_{e_G}(\phi) = f$。

令$V$为$G$中$e_G$的开邻域，使得对于$(s, t) \in V \times V$，定义乘积、$st$和$\phi(s)\phi(t)$且$st \in U$。将 $V \times V$ 的映射 $\alpha_1, \alpha_2$ 考虑为 $H$ 定义为

$$
\alpha_1(s, t) = \phi(ts), \quad \alpha_2(s, t) = \phi(t)\phi(s).
$$

然后$\alpha_1(t, e) = \phi(t) = \alpha_2(t, e)$。另一方面，将$t$固定在$V$中，将$\beta_i$固定在$V$的映射$s \mapsto \alpha_i(s, t)$到$H$中。然后，对于所有$s \in V$和所有$a \in L(G)$，

$$
\begin{align*}
T_s(\beta_1)(sa) &= T_{ts}(\phi)(tsa) = f_{ts, \phi(ts)}(tsa) \\
&= \phi(ts)f(a) = f_{s, \beta_1(s)}(sa) \\
T_s(\beta_2)(sa) &= \phi(t)T_s(\phi)(sa) = \phi(t)f_{s, \phi(s)}(sa) \\
&= \phi(t)\phi(s)f(a) = f_{s, \beta_2(s)}(sa).
\end{align*}
$$

因此（可微分和解析流形，R，9.3.7）$\alpha_1$和$\alpha_2$重合在$(e_G, e_G)$的邻域上。因此，$\phi$的限制到$e_G$的足够小的对称开邻域，因此是李群细菌的态射，从而（i）。

让$G_1, G_2, \phi_1, \phi_2$如(ii)中那样，让我们​​在$e_G$的邻域上证明$\phi_1, \phi_2$重合。存在$e_G$的开邻域$W$，使得$\phi_1(ts) = \phi_1(t)\phi_1(s)$、$\phi_2(ts) = \phi_2(t)\phi_2(s)$对于$W$中的所有$s, t$。那么，如果$s \in W$和$a \in L(G)$，

$$
T_s(\phi_i)(sa) = \phi_i(s)T_e(\phi_i)(a) = \phi_i(s)f(a) = f_{s, \phi_i(s)}(sa)
$$

$i = 1, 2$。作为$\phi_1(e_G) = e_H = \phi_2(e_G)$，从可微分和解析流形，R，9.3.7可以得出$\phi_1$和$\phi_2$重合在$e_G$的邻域上。

#### 推论 1 {#lie-iii-s4-thm-1-cor-1 .statement tag=0ACM}

令$G$和$H$为两个李群细菌。如果 $L(G)$ 和 $L(H)$ 同构的，则 $G$ 和 $H$ 局部同构。

这是从定理 1 和 § 1, no. 10、命题 21 得出的。

#### 推论 2 {#lie-iii-s4-thm-1-cor-2 .statement tag=0ACN}

设$G$为李群胚芽。如果 $L(G)$ 是可交换的，则 $G$ 与加法李群 $L(G)$ 局部同构。

加法群 $L(G)$ 的李代数与 $L(G)$ 同构的。因此，应用推论 1 就足够了。

#### 推论 3 {#lie-iii-s4-thm-1-cor-3 .statement tag=0ACO}

令 $G$ 为李群。如果$L(G)$是可交换的，则$G$包含是可交换的开子群。

G 存在一个可交换的开李子群胚芽 U（推论 2）。令 V 为 e 的邻域，使得 V^2 ⊂ U。则对于 V 中的所有 x, y，xy = yx。因此V生成的G的子群是可交换的；显然是开放的。

### 2.从李代数到李群的通道

我们用 H(X, Y) (章 II, § 6, no. 4, 定义 1) 表示 Hausdorff 级数。

#### 引理 2 {#lie-iii-s4-lem-2 .statement tag=0ACP}

令L是$\mathbf{R}$或$\mathbf{C}$的完全规范李代数。令 G 为 $x \in L$ 的集合，使得 $\|x\| < \frac{1}{3} \log \frac{3}{2}$。令$\theta$为G到G的映射$x \mapsto -x$。令H为L(章II, § 7, no. 2)的Hausdorff函数的限制至$G \times G$。
(i) $(G, 0, \theta, H)$ 是李群胚芽。
(ii) 设$\phi$为G到L的恒等映射。 $\phi$ 在 0 处的微分是可规范李代数 $L(G)$ 到 L 的同构。
(i) 从章 II, § 7, no. 2 得出。
由于$\phi$是G上的图表，$\phi$在0处的微分$\psi$是可规范空间的同构。另一方面，展开作为映射H的级数$H = \sum_{i,j \geq 0} H_{ij}$的积分使得$H_{11}(x, y) = \frac{1}{2}[x, y]$。截至 § 3、命题 24，对于 $L(G)$ 中的所有 $a, b$，
$$
\psi([a, b]) = H_{11}(\psi(a), \psi(b)) - H_{11}(\psi(b), \psi(a)) = [\psi(a), \psi(b)]
$$
这就证明了(ii)。

G被称为由L*定义的*李群胚芽。

假设 K 是超度量的。令$p$为K的剩余类域的特征。如果$p \neq 0$，则令$\lambda = |p|^{1/(p-1)}$；如果$p = 0$，则令$\lambda = 1$。

#### 引理 3 {#lie-iii-s4-lem-3 .statement tag=0ACQ}

令 L 为 K 上的完全范数李代数。令 G 为 $x \in L$ 的集合，使得 $\|x\| < \lambda$。令 $H : G \times G \to G$ 为 L (章 II, § 8, no. 3) 的 Hausdorff 函数。
(i) 当律为合成H时，G为李群，其中0为单位元素，$-x$为所有$x \in G$的x的倒数。
(ii) 设$\phi$为G到L的恒等映射。 $\phi$ 在 0 处的微分是可规范李代数 $L(G)$ 到 L 的同构。
(iii) 对于所有$\mu \in \mathbf{R}_+^*$，令$G_\mu$为$x \in L$的集合，使得$\|x\| < \mu$。那么$G_\mu$，对于$\mu < \lambda$，形式是0的开闭邻域的基本系统，并且是G的子群。
断言 (i) 和 (iii) 由章 II, § 8, no. 3 推出，命题 3 和 (ii) 可以如引理 2 那样证明。

G称为由L*定义的*李群。

#### 定理 2 {#lie-iii-s4-thm-2 .statement tag=0ACR}

令 L 为完全范数李代数。存在李群胚芽G，使得L(G)与L同构。两个这样的李群细菌是局部同构的。

第一个断言由引理2和3得出。第二个断言由推论1到no. 1的定理1得出。

#### 推论 1 {#lie-iii-s4-thm-2-cor-1 .statement tag=0ACS}

令 G 为李群。 e 存在邻域，其中包含没有与 {e} 不同的有限子群。如果 K = R 或 C，则存在 e 的开邻域，其中包含没有与 {e} 不同的子群。

我们写 L(G) = L。在L上定义选择范数，在L上定义拓扑，这样$\| [x, y] \| \leq \| x \| \| y \|$对于L中的所有x，y。

假设 K = R 或 C。令 G' 为由 L 定义的李群胚芽。 G' 中存在中心 0 的开球 U' 和李群胚芽 U' 的同构 $\phi$ 位于 G 中 e 的开邻域 U 上。设 V' = $\frac{1}{2} U'$, $V = \phi(V')$, H V和$h \in H$中包含G的子群。让$x = \phi^{-1}(h) \in V'$。如果$x \neq 0$，则存在整数 $n > 0$，使得$x, 2x, \ldots, nx$位于V'、$(n+1)x \in U'$、$(n+1)x \notin V'$中。那么$h, h^2, \ldots, h^n$在V，

$$
h^{n+1} \in U, \qquad h^{n+1} \notin V,
$$

这是荒谬的。因此 H = {e}。

假设 K 是超度量的。当G是李群与L相关时，足以证明推论。如果G中计算的g的$g \in G$、幂是L中计算的$\mathbf{Z}g$的元素。如果$g \neq e$，它们是不同的。因此 G 包含没有与 {e} 不同的有限子群。

#### 推论 2 {#lie-iii-s4-thm-2-cor-2 .statement tag=0ACT}

令 k 为 K 的非离散闭子域，k 上的 G 李群且 L = L(G)。假设L有一个可范李K-代数结构L'，与可范李K-代数结构兼容，且在G的伴随表示下不变量。则G上存在唯一一个与该李兼容的李K群结构k 群结构，其中李代数为 L'。

在 K 上存在李群胚芽$G_1$使得$L(G_1) = L'$(定理2)。根据no. 1的推论1至定理1，G和$G_1$被视为李k群细菌，是局部同构的。因此，G 中存在 e 的开邻域 G'，G' 上存在李 K 群胚芽结构，其中李代数L，与 k 上的李群胚芽结构兼容。令 V 为 G 中 e 的对称开邻域，使得 $V^2 \subset G'$。让$g \in G$。那么 $\phi = \operatorname{Int} g$ 是 G' 的足够小的开李子群胚芽到 G' 的开李子群胚芽的 k 同构；并且 $T_e(\phi)$ 是 K 线性的，因此当 x 足够接近 e 时，$T_x(\phi)$ 是 K 线性的；因此，Int g 的限制到 V 中 e 的足够小的开邻域是 K-解析的（可微且解析流形，R，5.14.6）。到 § 1, no. 9，命题 18，G 上存在一个解析 K 流形结构，其中 G 是一个谎言

K-群和V是G的开子K-流形。通过翻译，可以看出G的底层k流形结构是给定的结构。李 K 群 G 的李代数与开李 K 子群胚芽 V 相同，因此是 L'。最后，推论中所述的唯一性是从§ 3, no. 8、命题32得出的。

#### 定理 3 {#lie-iii-s4-thm-3 .statement tag=0ACU}

令 G 为李群胚芽和$\mathfrak{h}$一个$L(G)$的谎言子代数，承认拓扑补充。 G 存在一个李子群胚芽 H，使得 $L(H) = \mathfrak{h}$。如果 $H_1$ 和 $H_2$ 是 G 的谎言子群细菌，使得

$$
L(H_1) = L(H_2) = \mathfrak{h},
$$

那么$H_1 \cap H_2$在$H_1$和$H_2$开放。

存在李群胚芽$H'$，其中李代数同构于$\mathfrak{h}$（定理2）。如果必要的话，收缩$H'$，可以假设$H'$存在态射$\phi$到G中，使得$L(\phi)$是$L(H')$的同构到$\mathfrak{h}$（no. 1，定理） 1）。由于 $\mathfrak{h}$ 承认拓扑补充，$\phi$ 是 e 处的浸没。因此，进一步缩小$H'$，可以假设$\phi$是流形$H'$的同构到G的子流形上。这证明了H的存在。第二个断言由以下命题推出：

#### 命题 1 {#lie-iii-s4-prop-1 .statement tag=0ACV}

设G为李群胚芽，H和$H'$两个李子群胚芽。在阶、$L(H) \supset L(H')$中，$H \cap H'$在$H'$开放是必要且充分的。

如果$H \cap H'$在$H'$开放，则$L(H') = L(H \cap H') \subset L(H)$。假设$L(H) \supset L(H')$。令i，$i'$为H的典范嵌入，$H'$为G。如有必要，通过收缩$H'$，可以假设存在$H'$的态射$\psi$到H中，使得$L(\psi)$为典范嵌入 $L(H')$ 变为 $L(H)$（no. 1、定理 1）。那么$L(i \circ \psi) = L(i')$，因此$H'$中存在$e_{H'}$的邻域V，使得$i \circ \psi$和$i'$重合在V（定理1）上。因此 $V \subset H$、$V \subset H \cap H'$ 和 $H \cap H'$ 在 $H'$ (§ 1, no. 10) 中开放。

#### 命题 2 {#lie-iii-s4-prop-2 .statement tag=0ACW}

令 G 为 K 上的李群，k 为 K 的非离散闭子域，H 为李 k 群 G 的李子群。假设 $L(H)$ 是 $L(G)$ 的向量子 K 空间，其中承认拓扑补充。那么 H 是李 K 群 G 的李子群。

存在李 K 群 G 的李子群胚$H'$，使得 $L(H') = L(H)$ (定理 3)。考虑G、H、$H'$为李k群细菌； 定理 3 然后证明$H \cap H'$ 在H 和$H'$ 中开。因此，G 中存在 e 的开邻域 U，使得 $U \cap H$ 是 G 在 K 上的子流形。因此，H 是李 K 群 G 的李子群 (§ 1, no. 3，命题 6)。

### 3.指数映射

#### 定理 4 {#lie-iii-s4-thm-4 .statement tag=0ACX}

令G为李群胚芽，L其李代数，VL中0的开邻域，φ为V的解析映射进入G，使得φ(0) = 0且T_0(φ) = Id_L。以下条件是等效的：
(i) 对于所有 b ∈ L，对于 |λ| ， φ((λ + λ')b) = φ(λb)φ(λ'b)和|λ'|足够小。
(ii) 对于所有 b ∈ L 且每个整数 n > 0，φ_*(b^n) 是 U(G) 中次数 n 的齐次（T_0^{(∞)}(L) 用 TS(L) 标识，b^n 在 TS(L) 中评估）。
(iii) TS(L)到U(G)的映射 φ_*与TS(L)和U(G)的分度兼容。
(iv) TS(L)到U(G)的映射 φ_*是TS(L)到L的包络代数的典范映射。
(v) L上存在范数，定义L的拓扑，并且使得
$$
\|[x, y]\| \leq \|x\|\|y\|
$$
对于 L 中的所有 x、y 和由 L (no. 2) 定义的李群胚芽的开子群胚芽 W ⊂ V，使得 φ|W 是 W 的同构到 G 的开李子群胚芽上。

(v) ⇒ (i)：显然，对于 (λb).(λ'b) = (λ + λ')b 在 W 中 |λ|和|λ'|足够小。
(i)⇒(ii)：假设满足条件(i)。设 b ∈ L。令 ψ 为 φ 到 V ∩ Kb 的限制。通过假设，加法李群 Kb 中存在对称邻域 T 为 0，使得 ψ|T 为李群胚芽 T 到 G 的态射。因此
$$
\varphi_*(b^n) = (\psi|T)_*(b^n) = ((\psi|T)_*(b))^n = (\varphi_*(b))^n,
$$
使得 φ_*(b^n) 是 U(G) 中次数 n 的齐次。
(ii) ⇒ (iii): 这是因为 TS^n(L) 是由 L 的元素的第 n 个幂生成的 TS(L) 的向量子空间 (代数, 章) IV, § 5、命题5)。
(iii) ⇒ (iv): TS(L)的典范映射进入L的包络线代数，是分级余代数映射1到1的唯一态射，并延伸Id_L(章II, § 1, no. 5， 注3)。现在 φ_* 为余代数态射并且 φ_*|L = Id_L by 假设。如果条件(iii)成立，则可知条件(iv)也成立。
(iv)⇒(v)：假设满足条件(iv)。 选择范数在 L 上定义 L 的拓扑且满足 \|[x, y]\| \leq \|x\|\|y\|对于 L 中的所有 x, y。令 H 为由范数李代数 L 定义的李群胚芽。通过定理 1，存在 H 的开子群胚芽 S ⊂ V 和 S 的同构 φ' 到 G 的开子群胚芽。我们已经知道 (v) ⇒ (iv)，TS(L) 的映射 φ_* 变为U(G) 是 TS(L) 的典范映射到 L 的包络线代数中。因此，对于所有 t ∈ T_0^{(∞)}(L)，φ_*(t) = φ'_*(t)。由于 φ 和 φ' 是解析的，因此 φ 和 φ' 重合在 0 的邻域上。

#### 定义 1 {#lie-iii-s4-def-1 .statement tag=0ACY}

令 G 为李群胚芽，L 为李代数。 G 的指数映射是定义在 L 中 0 的开邻域、G 中的值和定理 4 的满足条件上定义的任何解析式映射 $\phi$。

定理 4 立即意味着，对于每个李群细菌 G，存在 G 的指数映射以及 G 重合在 0 的邻域上的两个指数映射。

#### 例 {#lie-iii-s4-n3-exa-1 .statement tag=0ACZ}

(1) 令 G 为完全可范空间 E 的加法群。L(G) 到 E 上的典范同构满足定理 4 的条件 (i)，因此是 G 的指数映射。

(2) 设 A 为完全范数酉结合词代数。令 A* 为 A 的可逆元的李群由……组成。我们认同 L(A*) 与 A (§ 3, no. 9，命题 33 的推论)。如果 K = \mathbf{R} 或 \mathbf{C}，我们知道章 II, § 7, no. 3 中定义的 A 到 A* 的映射 exp 满足定理 4 的条件 (i)，因此是指数映射。现在让 K 为超度量。令$p$为K的剩余类域的特征。如果$p \neq 0$，则令$\lambda = |p|^{1/(p-1)}$；如果$p = 0$，则令$\lambda = 1$。令 U 为 $x \in A$ 的集合，使得 $\|x\| < \lambda$。我们知道 (章 II, § 8, no. 4) U 到 A* 的映射 exp 满足定理 4 的条件 (i)，因此是指数映射。 注 U 是 A 的加法子群。

这例解释了定义1中采用的术语。

设G为李群胚芽，$\phi$G的指数映射。则$\phi$在0处为étale，因此L(G)中存在0的开邻域U，使得$\phi(U)$在G中开，$\phi|U$是同构解析流形 U 到解析流形 $\phi(U)$。

G 上的规范图（第一个类）是解析流形 G 上的图 $\psi$，其逆映射是指数映射。如果进一步 G 是有限维的，并且选择 L(G) 的基，则由 $\psi$ 定义的坐标系统和$\psi$ 域中的基称为规范坐标系统（第一个类的）。

#### 命题 3 {#lie-iii-s4-prop-3 .statement tag=0AD0}

令 G 为李群胚芽，L其李代数和$\phi$G的指数映射。令$L_1, \ldots, L_n$为L的向量子空间，使得L是拓扑直和 $L_1, \ldots, L_n$。 映射

$$
(b_1, b_2, \ldots, b_n) \mapsto \theta(b_1, b_2, \ldots, b_n) = \phi(b_1)\phi(b_2)\cdots\phi(b_n),
$$

定义在$L_1 \times L_2 \times \cdots \times L_n$的开子集上，是解析的。 $(0, 0, \ldots, 0)$ 到 $\theta$ 的切线映射是 $L_1 \times \cdots \times L_n$ 到 L 的典范映射。

设$k_i$为$L_i$的典范嵌入到$L_1 \times L_2 \times \cdots \times L_n$。然后，对于所有 $b \in L_i$、$(T_{(0, \ldots, 0)}\theta)(T_0k_i)(b) = (T_0\phi)(b) = b$，因此 $(T_{(0, \ldots, 0)}\theta)|L_i$ 是 $L_i$ 的典范嵌入到 L。

特别是，$\theta$ 是 $(0, 0, \ldots, 0)$ 的 étale。它的限制足够小

LIE GROUPS

$(0, 0, \ldots, 0)$的开邻域U在G中有一个开像，并且是流形U的同构到流形$\theta(U)$。 U 上 $\theta(U)$ 的逆映射 $\eta$ 称为 G 的第二个类* 的*规范图，与给定的 L 的分解关联为直和。如果进一步的 G 是有限维的，并且每个 $L_i$ 由非零向量 $e_i$ 生成，则由 $\eta$ 定义的 $\theta(U)$ 上的坐标系统和 $e_i$ 称为第二个类* 的*规范坐标系统。

#### 命题 4 {#lie-iii-s4-prop-4 .statement tag=0AD1}

*设 G 为李群胚芽，$\phi$ G 的单射指数映射。对于 $L(G)$ 中的所有 x、y，*

(1)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))
$$
(2)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2} \phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))
$$
（注，$\phi^{-1}(\phi(\lambda x) \phi(\lambda y))$和$\phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))$被定义为$|\lambda|$足够小）。

让$L = L(G)$被给定范数，定义L的拓扑，并且$\| [x, y] \| \leq \| x \| \| y \|$适用于L中的所有$x, y$。使用定理 2和4，可以假设G是由L和$\phi = \mathrm{Id}_G$定义的李群胚芽。设$(x, y) \mapsto x \cdot y$表示群G中的乘积，则待证明的公式可写成
(3)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1}((\lambda x) \cdot (\lambda y))
$$
(4)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2}((\lambda x) \cdot (\lambda y) \cdot (-\lambda x) \cdot (-\lambda y)).
$$

K 中存在 0 的开邻域 V，使得函数
$$
\lambda \mapsto f(\lambda) = (\lambda x) \cdot (\lambda y)
$$
在 V 上定义并解析。将$f$的章II, § 6, no. 4、*注2*、展开作为关于原点的级数积分为
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] + \cdots
$$
这证明了(3)。另一方面，对于G中的$u, v$和$\|u\|, \|v\|$足够小，$u \cdot v$是$(u, v)$的解析函数和次数1和2在展开中的项作为这个函数的积分关于原点的级数是$u + v + \frac{1}{2}[u, v]$。通过*可微解析流形*，R，3.2.7和4.2.3，次数1和2的项在函数$f(\lambda) \cdot f(-\lambda)$的展开作为关于原点的积分级数是项次数 1 和 2 英寸
$$
f(\lambda) + f(-\lambda) + \frac{1}{2}[f(\lambda), f(-\lambda)]
$$
或也在
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] - \lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] \\
+ \frac{1}{2} [\lambda(x + y), -\lambda(x + y)] = \lambda^2 [x, y]
$$
这就证明了(4)。

指数映射

§ 4.3

#### 命题 5 {#lie-iii-s4-prop-5 .statement tag=0AD2}

令 G 为李群，k 为 K 的非离散闭子域，G' 群 G 被视为 k 上的李群，$\phi$（或 $\phi'$）为 G（或 G'）的指数映射。然后 $\phi$ 和 $\phi'$ 重合在 0 的邻域上。

相对于G'，$\phi$满足定理4的假设(i)，因此是G'的指数映射。

#### 命题 6 {#lie-iii-s4-prop-6 .statement tag=0AD3}

设G是李群胚芽，L是李代数，$\phi : V \to G$是G的指数映射。对于所有$x \in V$，让$T_x(L)$等同于L，这样$\phi$在x处的右微分$\varpi(x)$是将L的线性映射转化为L。对于 x 足够接近 0，

$$
\varpi(x) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\operatorname{ad} x)^n.
$$

让L被赋予与其拓扑兼容的范数，并且使得$\| [x, y] \| \leq \| x \| \| y \|$对于所有$x, y \in L$。考虑 G 是由 L 和 $\phi = \operatorname{Id}_G$ 定义的李群胚芽的情况就足够了。通过定义，$\varpi(x)$ 是 G 在 x 处到映射 $y \mapsto y . x^{-1}$ 到 G 的切线映射。如果 $H(X, Y)$ 表示 Hausdorff 级数，则 $\varpi(x)$ 是，对于 $\| x \|$ 足够小，切线映射在G的0到映射$y \mapsto H(x, +y, -x)$进入G。在$H(X + Y, -X)$中，Y中第一个次数的项的和是

$$
\sum_{m \geq 0} \frac{1}{(m+1)!} (\operatorname{ad} X)^m Y
$$

（章II, § 6, no. 5，命题5）。 命题由可微分和解析流形、R、3.2.4 和 4.2.3 得出。

令 G 为李群胚芽和$t \in K$。 G* 的 *t-th 幂映射是任意映射，在 e 的开邻域上定义和解析，其中值在 G 中并且在 e 的邻域上与映射重合

$$
g \mapsto \phi(t \phi^{-1}(g))
$$

其中 $\phi$ 是 G 的单射指数映射。

#### 命题 7 {#lie-iii-s4-prop-7 .statement tag=0AD4}

(i) *如果 $t \in \mathbf{Z}$，则 e 的邻域上第 t 个幂映射重合与映射 $g \mapsto g^t$。*

(ii) *在 e 处与第 t 个幂映射的切线映射是比率 t 的位似。*

(iii) *如果 h 是 G 的第 t 个幂映射并且 h' 是 G 的第 t' 个幂映射，则 $h \circ h'$ 是第 (tt') 个幂映射并且 $g \mapsto h(g)h'(g)$ 是 (t + t')-第幂映射.*

(iv) *如果 h 是第 t 个幂映射和 $u \in U^n(G)$，则 $h_*(u) = t^n u$。*

当 G 是由完整范数李代数定义的李群胚芽时，并且当考虑的第t个幂映射是使用指数映射$\phi = \operatorname{Id}_G$构造时，足以证明命题。但在这种情况下，一切都是显而易见的。

### 4.指数映射的函数化

#### 命题 8 {#lie-iii-s4-prop-8 .statement tag=0AD5}

设G和H为李群细菌，G的h态射转化为H以及G和H的$\phi_G$和$\phi_H$指数映射。在$L(G)$中存在0的邻域V使得$h \circ \phi_G$和$\phi_H \circ L(h)$重合于V。

让 $L(G)$ 和 $L(H)$ 被给定范数定义它们的拓扑，并且使得 $\| [x, y] \| \leq \| x \| \| y \|$ 对于所有 x 和 y。可以假设 G（分别为 H）是由 $L(G)$（分别为 $L(H)$）定义的李群胚芽，因此 $\phi_G$（分别为 $\phi_H$）重合和 $\mathrm{Id}_G$（分别为 $\mathrm{Id}_H$） 邻域为 0。另一方面，$L(G)$ 中存在 0 的对称开邻域 W，使得 $L(h)$ 为李群胚芽 W 到 H 的态射。由定理 1，$L(h)$ 重合，邻域上的 h 为 0，从而命题。

宽松地说，如果 G 和 H 在单位元素的邻域中与 $L(G)$ 和 $L(H)$ 通过指数映射进行辨识，则 G 到 H 的每个态射在 0 的邻域中都是“线性”。

#### 推论 1 {#lie-iii-s4-prop-8-cor-1 .statement tag=0AD6}

设 G 为李群胚芽，G' 为 G 的谎言子群胚芽，$\phi$ 为 G 的指数映射。

(i) $L(G')$ 中存在 0 的开邻域 V，使得 $\phi|V$ 是流形 V 的同构到 G' 中 e 的开邻域。

(ii) 设 $x \in L(G)$。以下条件是等效的： (a) $x \in L(G')$； (b) $\phi(\lambda x) \in G'$ 对于 $|\lambda|$ 足够小。

(i) 是通过将 G' 的应用命题 8 到典范嵌入代入 G 获得的，并且 (ii) 由 (i) 得出。

#### 推论 2 {#lie-iii-s4-prop-8-cor-2 .statement tag=0AD7}

设 G 为李群，$\rho$ G 的解析线性表示，$\phi$ G 的指数映射。在 $L(G)$ 中存在 0 的邻域 V，使得
$$
\rho(\phi(x)) = \exp(L(\rho)x)
$$
对于所有$x \in V$。

这是从 no. 3 的命题 8 和例 2 得出的。

#### 推论 3 {#lie-iii-s4-prop-8-cor-3 .statement tag=0AD8}

令 G 为李群和 $\phi$ G 的指数映射。

(i) $L(G)$ 中存在 0 的邻域 V 使得
$$
\mathrm{Ad}(\phi(x)) = \exp \mathrm{ad}\ x.
$$
对于所有$x \in V$。

(ii) 如果 $g \in G$，$L(G)$ 中存在 0 的邻域 W，使得
$$
g \phi(x) g^{-1} = (\mathrm{Ad}\ g.x)
$$
对于所有$x \in W$。

(i) 由推论 2 和 § 3, no. 12、命题 44 得出。
(ii) 从适用于 Int g 的命题 8 得出。

### 5. 结构由子群引发

#### 引理 4 {#lie-iii-s4-lem-4 .statement tag=0AD9}

设G是有限维李群，$\Omega$G中e的对称开邻域和$\Omega$包含e的H子集，使得条件$x \in H, y \in H, xy^{-1} \in \Omega$隐含$xy^{-1} \in H$。让$r \in N_K$。对于所有$x \in H$，令$h_x$为$a \in T_x(G)$的集合，其中性质：K中存在0的开邻域I和类$C^r$的映射f I 代入 G 使得$f(0) = x, f(I) \subset H, (T_0f)(1) = a$。

(i) 设 $h_e = h$。那么h是$L(G)$的谎言子代数，在$\mathrm{Ad}_{L(G)}(H)$下不变。

(ii) $h_x = xh = hx$ 对于所有 $x \in H$（其中 $xh$ 和 $hx$ 在 $T(G)$ 中评估）。

(iii) 令V为类$C^r$的流形、V的$v_0$点以及V的类$C^r$的f映射代入G，使得$f(v_0) = e$ 和 $f(V) \subset H$。对于具有李代数 h 的 G 的每个谎言子群胚$H'$，$f(v) \in H'$ 对于足够接近 $v_0$ 的 v。

(iv) 对于具有李代数 h 的 G 的每个谎言子群胚$H'$，$H' \cap H$ 是$H'$ 中 e 的邻域。

(v) 对于所有$x \in H$和所有$a \in h_x$，K中存在0的开邻域I和G中I的类$C^a$的映射f，使得$f(0) = x, f(I) \subset H, (T_0f)(1) = a$。显然，对于 H 中的 $x, y, xy, xyz$，$Kh = h$ 和 $xh_yz = h_{xyz}$。这意味着 (ii) 以及 h 在 $\mathrm{Ad}_{L(G)}(H)$ 下不变的事实。

设 $a_1, a_2$ 位于 h 中。令I是K中0的开邻域，并将I的类$C^r$的$f_1, f_2$映射放入G中，使得$f_j(0) = e, f_j(I) \subset H, (T_0f_j)(1) = a_j$（$j = 1, 2$）。我们定义$f : I \to G$到$f(\lambda) = f_1(\lambda)f_2(\lambda)$。那么 f 就是类 $C^r$ 和 $f(0) = e$。如有必要，通过缩小 I，我们得到 $f(I) \subset H$。另一方面，$T_e(G) \times T_e(G)$到$T_e(G)$的映射与映射$(g, g') \to gg'$的切线是加法；因此$(T_0f) = a_1 + a_2$。因此 $a_1 + a_2 \in h$ 且 h 为 $L(G)$ 的向量子空间。由于$xhx^{-1} = h$适用于所有$x \in H$，$(\mathrm{Ad}_{f_1(\lambda)}) . a_2 \in h$适用于所有$\lambda \in I$。 0 到映射 $\lambda \mapsto \mathrm{Ad}f_1(\lambda)$ 处的切线映射为 § 3, no. 12 的命题 44，映射 $\lambda \mapsto \mathrm{ad}(a_1\lambda)$；因此

$$
[a_1, a_2] = (\mathrm{ad}\, a_1) . a_2 \in h
$$

因为 h 在 $L(G)$ 内闭合。由此我们证明了(i)。在证明的其余部分中，我们用李代数 h 修复了 G 的谎言子群胚芽 $H'$。

令V、$v_0, f$如(iii)中所示。令 Y 为与 h (no. 1) 相关的 G 的左叶化。对于所有$y \in H'$，$T_y(H') = yh$。另一方面，对于所有$v \in V$，$T_v(f)$下的$T_v(V)$的像包含在$h_{f(v)} = f(v)h$中（$h_{f(v)}$的定义）。通过 *可微分和解析流形*, R, 9.3.2，f 是 V 的态射进入 Y。由于 $H'$ 是 Y 的叶子（*可微分和解析流形*, R, 9.2.8），$f(v) \in H'$ 对于 v 足够接近$v_0$。

设 $(a_1, \ldots, a_s)$ 为 h 的基。 K 中存在 0 的开邻域 I，G 中存在 I 的类 $C^r$ 映射 $f_1, \ldots, f_s$，使得对于所有 j 都有 $f_j(0) = e, f_j(I) \subset H, (Tf_j)1 = a_j$。到(iii)，$f_j(\lambda) \in H'$对于$|\lambda|$足够小。因此，对于$|\lambda_1|, |\lambda_2|, \ldots, |\lambda_s|$足够小，$f_1(\lambda_1)f_2(\lambda_2)\ldots f_s(\lambda_s)$构成$H'$中$e$的邻域；而这个邻域包含在$H$中。因此(iv)。

如果$a \in \mathfrak{h}$，则$K$中存在$0$的开邻域$I$和$I$的映射$f$到$G$的类$C^\omega$，使得$f(0) = e, f(I) \subset H', (T_0 f)1 = a$。这与 (iv) 一起意味着 (v)。

#### 定义 2 {#lie-iii-s4-def-2 .statement tag=0ADA}

$\mathfrak{h}$ 称为子代数在 $e$ 处与 $H$ 相切。

#### 命题 9 {#lie-iii-s4-prop-9 .statement tag=0ADB}

令 $G$ 为 $G$ 的有限维李群和 $H$ 子群。

(i) 在 $H$ 上存在且仅有一个解析流形结构与以下性质：对于 1 到 $\omega$ 之间的所有 $r$，对于类的每个流形 $V$ $C^r$ 且对于 $V$ 的每个映射 $f$ 到 $H$，$f$ 的类 $C^r$ 与 $V$ 的映射到 $H$ 当且仅当$f$ 是类 $C^r$，就像映射是 $V$ 的$G$。

(ii) 有了这个结构，$H$是李群，$H$到$G$的典范嵌入$i$是沉浸，$L(i)(L(H))$是$e$到$H$的谎言子代数切线。

在(i)中唯一性是显而易见的。我们证明存在。令 $\mathfrak{h}$ 为李代数在 $e$ 到 $H$ 的切线。设$H'$是$G$与李代数$\mathfrak{h}$的谎言子群胚芽。通过替换$H'$通过$H'$的开放子群胚芽，可以假设$H' \subset H$（引理4（iv））。对于所有$x \in H$，$xH'x^{-1}$是$G$与李代数$x\mathfrak{h}x^{-1} = \mathfrak{h}$的谎言子群胚芽。因此，$H' \cap (xH'x^{-1})$ 在 $H'$（no. 2、定理 3）中开放，映射 $y \mapsto xyx^{-1}$ 是 $H' \cap x^{-1}H'x$ 的同构到 $xH'x^{-1} \cap H'$。利用§ 1, no. 9的命题 18，$H'$和李群结构存在一个开谎言子群胚芽$W$，并且在$H$上具有以下性质： $W$在$H$开并且$H$ 上的流形结构和$H'$ 诱导 $W$ 上的结构相同。由此可见，$H$到$G$的典范嵌入$i$是沉浸，$L(i)(L(H)) = L(H') = \mathfrak{h}$。此外，令$V$和$f$如(i)中那样。如果 $f : V \to H$ 为类 $C^r$，则 $i \circ f : V \to G$ 为类 $C^r$。假设$i \circ f : V \to G$是类$C^r$；那么我们证明$f : V \to H$是类$C^r$。通过翻译，考虑存在$v_0 \in V$使得$f(v_0) = e$的情况并证明$f : V \to H$在$v_0$的开邻域中是类$C^r$就足够了。现在，到引理 4 (iii)，$f(v) \in H'$对于$v$足够接近$v_0$，从而我们的断言。这样我们就证明了(i)和(ii)已经得到了。

#### 定义 3 {#lie-iii-s4-def-3 .statement tag=0ADC}

命题 9 中定义的$H$上的李群结构称为$G$上的李群结构在$H$上诱导的结构。

如果$H$是$G$的谎言子群，则其李群结构由$G$上的谎言子群诱导（可微分和解析流形，R，5.8.5）。

如果 $G = \mathbf{R}$ 和 $H = \mathbf{Q}$，则 $\mathfrak{h} = \{0\}$ 以及因此在 $H$ 上导出的结构是离散的李群结构。类似地，如果$G = \mathbf{C}$（被视为复数李群）和$H = \mathbf{R}$。

### 6. 形式与值李代数的微分原语

#### 引理 5 {#lie-iii-s4-lem-5 .statement tag=0ADD}

令$X$为类$C^r$、$F$的流形和类$C^r$的$F'$向量丛和基空间$X$以及将$F$中的$\phi$态射转换为$F'$。对于所有 $x \in X$，令 $S_x$ 为集合
$$
(a, \phi(a)) \in F_x \oplus F'_x
$$
$a \in F_x$。那么$S_x$的并$S$是$F \oplus F'$的向量子束。

设$\theta$和$\theta'$为$F \oplus F'$的映射，定义如下：如果$(u, v) \in F_x \oplus F'_x$，则
$$
\theta(u, v) = (u, v + \phi(u)), \qquad \theta'(u, v) = (u, v - \phi(u)).
$$
通过*可微分和解析流形*，R、7.7.1、$\theta$和$\theta'$本身就是$F \oplus F'$的态射。显然$\theta \circ \theta' = \theta' \circ \theta = \mathrm{Id}_{F \oplus F'}$。因此$\theta$和$\theta'$是$F \oplus F'$的自同构。因此，$S = \theta(F \oplus \{0\})$是$F \oplus F'$的向量子丛。

#### 引理 6 {#lie-iii-s4-lem-6 .statement tag=0ADE}

令$G$为李群胚芽，$\omega$$G$（§ 3, no. 18.9）的规范左微分形式，类$C^r$（$r \geq 2$）的$M$流形以及$\alpha$ $M$ 上的类 $C^{r-1}$ 和次数 1 的差形式与$L(G)$ 中的值。

(i) $T(M \times G)$ 的元素，其中差值形式
$$
\theta = \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega
$$
零构成类 $C^{r-1}$ $T(M \times G)$ 的向量子束$S$。

(ii) 对于所有 $(x, g) \in M \times G$，$T(\mathrm{pr}_1)|S_{(x, g)}$ 是 $S_{(x, g)}$ 的同构到 $T_x(M)$。

(iii) *如果* $d\alpha + [\alpha]^2 = 0$ (cf. § 3, no. 14) *向量子束* $S$ *可积*。

若$(x, g) \in M \times G$且$(u, v) \in T_x(M) \times T_g(G)$，则
$$
\theta_{(x, g)}(u, v) = \alpha(u) - g^{-1}v.
$$
因此，对于$u \in T_x(M)$、从而 (ii)，$\theta_{(x, g)}$ 的核是$(u, g\alpha(u))$ 的集合 $S_{(x, g)}$。我们将$T(M \times G)$视为两个向量丛、$F$和$F'$以及$F_{(x, g)} = T_x(M) \times \{0\}$和$F'_{(x, g)} = \{0\} \times T_g(G)$的直和。
$$
(x, g) \in M \times G.
$$
对于$u \in T_x(M) \times \{0\}$，我们写为$\phi(u) = (0, g\alpha(u))$。使用$T(G)$的左平凡化，可以看出$\phi$是$F$的态射变成$F'$，从而（i）（引理5）。最后，如果$d\alpha + [\alpha]^2 = 0$，那么
$$
\begin{align*}
d\theta &= \mathrm{pr}_1^*(d\alpha) - \mathrm{pr}_2^*(d\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha \wedge \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega \wedge \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega) \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}\theta \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega)
\end{align*}
$$
因此 $S$ 是可积的（*可微且解析流形*, R, 9.3.6）。

#### 定理 5 {#lie-iii-s4-thm-5 .statement tag=0ADF}

设G为李群胚芽，M流形为类$C^r$($r \geq 2$)和$\alpha$微分形式为类$C^{r-1}$和次数1在M上与值在$L(G)$，使得$d\alpha + [\alpha]^2 = 0$。对于所有$x \in M$和所有$g \in G$，存在映射$f$，定义为类$C^{r-1}$在$x$的开邻域上，值在$G$中，这样$f(x) = g$ 和 $f^{-1}.df = \alpha$。 $x$的邻域上有两个映射，其中满足这些条件重合。

设$x \in M$和$g \in G$。由引理 6（我们采用其记号）和可微分解析流形，R，9.3.7，M中存在$x$的开邻域U和类的映射$m \mapsto \phi(m) = (m, f(m))$将 U 的 $C^{r-1}$ 化为 $M \times G$，使得 $f(x) = g$ 和 $\phi^*(0) = 0$。然后

$$
f^{-1}.df = f^*(\omega) \quad (§ 3, \text{no. 18.9}) \\
= (\mathrm{pr}_2 \circ \phi)^*(\omega) \quad (\text{for } f = \mathrm{pr}_2 \circ \phi) \\
= \phi^*(\mathrm{pr}_1^*\alpha - \theta) \quad (\text{Lemma 6}) \\
= \phi^*(\mathrm{pr}_1^*\alpha) \quad (\text{for } \phi^*(\theta) = 0) \\
= \alpha \quad (\text{for } \mathrm{pr}_1 \circ \phi = \mathrm{Id}_U).
$$

令$f'$为U的类$C^{r-1}$到G中的映射，使得$f'(x) = g$和${f'}^{-1}df' = \alpha$。到§ 3，18.9，${f'}^{-1}$是局部常数，因此$f' = f$位于$x$的邻域中。

#### 命题 10 {#lie-iii-s4-prop-10 .statement tag=0ADG}

设 M 为 M 上的解析流形、$\mathfrak{g}$ 完全可范李代数和 $\alpha$ M 上次数 1 的解析微分形式，其中值在 $\mathfrak{g}$ 中，具有以下属性：
(a) 对于所有$m \in M$，$\alpha_m$是$T_m(M)$的同构到$\mathfrak{g}$；
(b) $d\alpha + [\alpha]^2 = 0$。

那么，对于所有$m_0 \in M$，M中存在$m_0$的开邻域$M'$和$M'$上的李群胚芽结构，与$M'$上的流形结构兼容，有单位元素 $m_0$ 并具有以下属性：
(i) $\alpha_{m_0}$ 是$L(M')$ 的同构到$\mathfrak{g}$；
(ii) 微分形式 $m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$ 是 $M'$ 的左规范微分形式。
如果$M'_1$和$M'_2$是两个这样的群胚芽，$M'_1$和$M'_2$有公共的开放子群胚芽。

存在李群细菌G使得$L(G) = \mathfrak{g}$。让$m_0 \in M$。到定理 5，M 中存在$m_0$ 的开邻域 $M'$，G 中存在$M'$ 的解析映射 $f$，使得$f(m_0) = e$ 和$f^{-1}.df = \alpha$。那么$T_{m_0}(f) = \alpha_{m_0}$就是$T_{m_0}(M)$的同构到$\mathfrak{g}$上；因此，收缩$M'$和G，可以假设$f$是流形$M'$的同构到流形G上。我们通过以下方式将迁移到$M'$李群胚芽结构 $f^{-1}$。然后$T_{m_0}(f)$ 变成$L(M')$ 的同构到$L(G) = \mathfrak{g}$、从而 (i)。另一方面，如果 $\omega$ 表示 $G$ 的左规范微分形式，则
$$
\alpha_{m_0}^{-1} \circ \alpha_m = (\mathrm{T}_{m_0} f)^{-1} \circ (f^{-1}.df)(m)
= (\mathrm{T}_m f)^{-1} \circ \omega(f(m)) \circ \mathrm{T}_m f
$$
因此$m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$是$M'$的左规范微分形式。

设$M''$是$m_0$的开邻域，具有李群胚芽结构，具有单位元素$m_0$，并且具有与性质(i)和(ii)类似的性质。那么$\alpha_{m_0}$是$L(M')$到$g$的同构，也是$L(M'')$到$g$的同构，因此是$L(M') = L(M'')$。因此，缩小$M'$和$M''$，可以假设群胚芽$M'$存在同构$\phi$到群胚芽$M''$（no. 1，推论1到定理1）。那么$\phi^{-1}.d\phi$就是$M'$的规范左微分。另一方面，令$\psi$为流形$M' \cap M''$的典范嵌入转化为李群胚芽$M''$；显然$\psi^{-1}.d\psi$是$M''$的规范左微分的限制。因此，对于所有$m \in M' \cap M''$，$(\psi^{-1}.d\psi)(m) = \alpha_{m_0}^{-1} \circ \alpha_m = (\phi^{-1}.d\phi)(m)$。因此$\phi$和$\psi$重合在$m_0$的邻域上（§ 3，18.9）。这就证明了命题的最后一个断言。

#### 推论{#lie-iii-s4-n6-cor-1 .statement tag=0ADH}

令 $M$ 为有限维 $n$ 的解析流形。令$\omega_1, \ldots, \omega_n$为$M$上次数1的解析微分形式，标量为值，其在$M$的每个点处线性独立，因此，对于所有$k = 1, \ldots, n$，$d\omega_k$为线性组合具有$\omega_i \wedge \omega_j$ 的常数系数。那么，对于所有$m_0 \in M$，$M$中存在$m_0$的开放邻域$M'$，以及$M'$上的李群胚芽结构与$M'$上的流形结构兼容，与单位元素 $m_0$ 且使得次数 1 的 $M'$ 上的左不变微分形式空间的 $\omega_1|_{M'}, \ldots, \omega_n|_{M'}$ 形式基与标量值。

如果$M'_1$和$M'_2$是两个这样的群胚芽，$M'_1$和$M'_2$有公共的开放子群胚芽。

令$X_1, \ldots, X_n$为$M$上的向量域，使得在$M$的每个点$m$处，$(X_t)_m$构成$T_m(M)$右$((\omega_1)_m, \ldots, (\omega_n)_m)$的基。这些域是分析性的。到假设，存在$c_{ijk} \in \mathbf{K}$ ($1 \leq i, j, k \leq n$)，使得$c_{ijk} = -c_{jik}$和$d\omega_k = \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j$。通过 *可微分和解析流形*, R, 8.5.7, 公式 (11),
$$
\langle [X_i, X_j], \omega_k \rangle = -(d\omega_k)(X_i, X_j) = -\left( \sum_{r < s} c_{rsk} \omega_r \wedge \omega_s \right)(X_i, X_j) = -c_{ijk}
$$
因此$[X_i, X_j] = -\sum_k c_{ijk} X_k$。由此可见，$-c_{ijk}$是李代数$g$相对于基$(e_1, \ldots, e_n)$的结构的常数。对于所有$m \in M$，令$\alpha_m$为$T_m(M)$到$g$的线性映射，其中映射$(X_1)_m$到$e_1, \ldots, (X_n)_m$到$e_n$。那么$\alpha$是次数1的$M$上的解析微分形式与$g$中的值，$\alpha_m$是$T_m(M)$到$g$的同构。另一方面，$\alpha = \sum_{k=1}^n \omega_k e_k$，因此
$$
d\alpha = \sum_{k=1}^n (d\omega_k)e_k = \sum_{k=1}^n \left( \sum_{i<j} c_{ijk}\omega_i \wedge \omega_j \right)e_k
$$
和
$$
\begin{align*}
[\alpha]^2 &= \sum_{k=1}^n [\omega_k e_k]^2 + \sum_{i<j} (\omega_i e_i) \wedge (\omega_j e_j) \quad (§ 3, \text{formula (30)}) \\
&= \sum_{i<j} (\omega_i \wedge \omega_j)[e_i, e_j] \\
&= -\sum_{k=1}^n \sum_{i<j} (c_{ijk}\omega_i \wedge \omega_j)e_k \\
&= -d\alpha.
\end{align*}
$$
那么就足以应用命题 10。

### 7. 从无穷小运算的律到运算的律

#### 命题 11 {#lie-iii-s4-prop-11 .statement tag=0ADI}

设$G_1$和$G_2$为李群细菌，$X_1$和$X_2$流形为类$C^r$（$r \geq 2$）。对于$i = 1, 2$，令$\psi_i$为$X_i$上$G_i$的类$C^r$的左运算的律块，以及$D_i$无穷小运算的关联律。令$\mu : G_1 \to G_2$为态射且$\phi : X_1 \to X_2$映射等于类$C^r$。假设对于所有 $a \in L(G)$，向量域 $(D_1)_a$ 和 $(D_2)_{L(\mu)a}$ 与 $\phi$ 相关（可微分和解析流形，R，8.2.6）。那么$G_1 \times X_1$中存在$\{e\} \times X_1$的邻域$\Omega$，使得$\phi(\psi_1(g, x)) = \psi_2(\mu(g), \phi(x))$对于所有$(g, x) \in \Omega$。

令 $p_1 : G_1 \times X_2 \to G_1, p_2 : G_1 \times X_2 \to X_2$ 为规范的投影。对于所有$(g_1, x_2) \in G_1 \times X_2$，令$f_{g_1, x_2}$为$T_{g_1}(G_1) = g_1 L(G_1)$的映射$g_1 a \mapsto (D_2)_{L(\mu)a}(x_2)$到$T_{x_2}(X_2)$。将$p_1^*T(G_1)$的$f_{g_1, x_2}$定义态射转化为$p_2^*T(X_2)$。

让$x_0 \in X_1$。在$G_1$中存在$e$的开邻域$G$，在$X_1$中存在$x_0$的开邻域$X$，使得为$(g, x) \in G \times X$定义了$\psi_1(g, x)$和$\psi_2(\mu(g), \phi(x))$。我们为$(g, x) \in G \times X$写道，
$$
\alpha(g, x) = \phi(\psi_1(g, x)) \in X_2, \qquad \beta(g, x) = \psi_2(\mu(g), \phi(x)) \in X_2.
$$
如果 $G$ 和 $X$ 足够小，那么对于所有 $(a, g, x) \in L(G_1) \times G \times X$，
$$
\begin{align*}
(T\alpha)(ag, 0_x) &= (T\phi)((D_1)_a(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}(\phi(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}\alpha(g, x), \\
(T\beta)(ag, 0_x) &= (T\psi_2)(L(\mu)a.\mu(g), \phi(x)) \\
&= (D_2)_{L(\mu)a}(\psi_2(\mu(g), \phi(x))) \\
&= (D_2)_{L(\mu)a}\beta(g, x).
\end{align*}
$$

因此对于$x \in X$，态射、$g \mapsto \alpha(g, x)$和$g \mapsto \beta(g, x)$是$f$的积分；作为
$$
\beta(e, x) = \phi(x) = \alpha(e, x)
$$
对于所有$x \in X$，可从*可微分和解析流形*，R，9.3.7得出，$\alpha$和$\beta$重合在$(e, x_0)$的邻域上。因此命题。

#### 推论{#lie-iii-s4-n7-cor-1 .statement tag=0ADJ}

*令 G 为李群胚芽和类$C^r$中的X流形。考虑X上G的类$C^r$的左侧运算的两个律块。假设对于所有$a \in L(G)$，X上的相应的向量域$D_a$对于两个律块来说是相同的。然后这两个律块重合位于$\{e\} \times X$的邻域上。*

#### 定理 6 {#lie-iii-s4-thm-6 .statement tag=0ADK}

*设G为李群胚芽、类$C^r$($r \geq 2$)的X流形和X的$x_0$点。令$a \mapsto D_a$为X上$L(G)$的类$C^{r-1}$的左无穷小运算的律。*

(i) *在X中存在$x_0$的开邻域$X'$，并且在$X'$上存在G的类$C^{r-1}$的左侧运算的律块，使得关联的无穷小律运算是$a \mapsto D_a|X'$。*

(ii) *让G的类$C^{r-1}$的左运算有两个律块位于$x_0$的开邻域$X''$上；如果他们承认$a \mapsto D_a|X''$与无穷小运算相关的律，那么他们重合就在$(e, x_0)$的邻域上。*

断言 (ii) 由命题 11 的推论得出。我们证明 (i)。对于所有$(g, x) \in G \times X$和所有$a \in L(G)$，我们写
$$
Q_a(g, x) = (ag, D_a(x)) \in T_g(G) \times T_x(X).
$$
对于$a \in L(G)$，令$S_{(g, x)}$为$Q_a(g, x)$的集合。通过no. 6的引理5，$S_{(g, x)}$是$T(G) \times T(X)$的向量子束S的纤维。设$a, b$在$L(G)$中；然后
$$
\begin{align*}
[Q_a, Q_b](g, x) &= ([R_a, R_b](g), [D_a, D_b](x)) \\
&= (-R_{[a, b]}(g), -D_{[a, b]}(x)) \quad (§ 3, 18.6) \\
&= Q_{-[a, b]}(g, x)
\end{align*}
$$
因此 S 是可积的（*可微且解析流形*, R, 9.3.3, (iv)）。

由*可微分和解析流形*，R，9.3.7，G中存在e的开邻域$G_1$，X中存在$x_0$的开邻域$X_1$和映射$(g, x) \mapsto gx$将$G_1 \times X_1$的类$C^{r-1}$转化为X，使得$ex = x$对于所有$x \in X_1$并且
$$
(ag)x = D_a(gx) \quad \text{for } a \in L(G), g \in G_1, x \in X_1.
$$
特别是
$$
ax = D_a(x).
$$
令$G_2$为$G_1$中e的开邻域，以及$X_2$为$X_1$中$x_0$的开邻域，这样$gg'$被定义，并且属于到$G_1$为定义了$G_2$和$gx$中的$g, g'$，并且对于$(g, x) \in G_2 \times X_2$定义了属于至$X_1$。将 $G_2 \times (G_2 \times X_2)$ 的映射 $\alpha_1, \alpha_2$ 考虑为 $X$ 定义为
$$
\alpha_1(g, (h, x)) = g(hx), \quad \alpha_2(g, (h, x)) = (gh)x.
$$
它们的尺寸为类 $C^{r-1}$。然后
$$
\alpha_1(e, (h, x)) = hx = \alpha_2(e, (h, x)).
$$
另一方面
$$
\begin{align*}
T(\alpha_1)(ag, 0_{(h, x)}) &= (ag)(hx) \\
&= D_a(g(hx)) \qquad \text{by (6)} \\
&= D_a(\alpha_1(g, (h, x))), \\
T(\alpha_2)(ag, 0_{(h, x)}) &= (agh)x \\
&= D_a((gh)x) \qquad \text{by (6)} \\
&= D_a(\alpha_2(g, (h, x))).
\end{align*}
$$
通过 *可微分和解析流形*、R、9.3.7、$\alpha_1$ 和 $\alpha_2$ 重合在 $(e, (e, x_0))$ 的邻域上。然后 (i) 由 (7) 和 § 1, no. 11 的命题 23 得出。

#### 推论 1 {#lie-iii-s4-thm-6-cor-1 .statement tag=0ADL}

*令$G$为李群胚芽，$X$为类$C^r$（$r \geq 2$）的副紧致流形。 令$a \mapsto D_a$为$X$上$L(G)$的类$C^{r-1}$的左无穷小运算的律。

(i) $X$ 上$G$ 的类 $C^{r-1}$ 的左运算存在律块，使得无穷小运算的关联律为$a \mapsto D_a$。

(ii) Two laws of left operation of class $C^{r-1}$ of $G$ on $X$ which admit $a \mapsto D_a$ as associated law of infinitesimal operation coincide on a neighbourhood of $\{e\} \times X$.

断言 (ii) 从推论到命题 11。到定理 6 (i)，存在$X$的开放覆盖$(X_i)_{i \in I}$，并且对于所有$i \in I$，左运算$\psi_i$的律块$X_i$ 上$G$的类$C^{r-1}$，使得无穷小运算的关联律为$a \mapsto D_a|_{X_i}$。由于 $X$ 是仿紧的，因此可以假设覆盖$(X_i)_{i \in I}$ 是局部有限的。对于 $(e, x)$ 的邻域上的所有 $(i, j) \in I \times I$ 以及所有 $x \in X_i \cap X_j$、$\psi_i$ 和 $\psi_j$ 重合（命题 11 的推论）。由于$X$是正规的，我们可以得到§ 1, no. 11的应用命题24，从而证明(i)。

#### 推论 2 {#lie-iii-s4-thm-6-cor-2 .statement tag=0ADM}

*令 $X$ 为类 $C^r$ ($r \geq 2$) 的仿紧凑流形和 $X$ 上类 $C^{r-1}$ 的$\xi$ 向量域。 $X$ 上存在运算 $\psi$ 类 $C^{r-1}$ $K$ 的律块，使得对于所有$x \in X$，$\xi(x)$ 是切线$t \mapsto (t, x)$ 下的像向量 1 到 $K$ 位于 0。运算的两个律块以及上述性质重合位于 $\{0\} \times X$ 的邻域。

这是推论 1 的一个特例。*

§ 5.1

#### 注 {#lie-iii-s4-n7-rem-1 .statement tag=0ADN}

左运算的律当然可以在整个编号中被右运算的律替换。

### 习题 {#lie-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
