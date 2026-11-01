---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 1
section_title: Lie groups
lang: zh
source: lie-i-iii
book_pages: 209-233, 370-372
pdf_pages: 0227-0251, 0388-0390
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A LIE GROUP
      page: 209
      pdf_page: 227
    - "no": 2
      title: MORPHISMS OF LIE GROUPS
      page: 213
      pdf_page: 231
    - "no": 3
      title: LIE SUBGROUPS
      page: 214
      pdf_page: 232
    - "no": 4
      title: SEMI-DIRECT PRODUCTS OF LIE GROUPS
      page: 215
      pdf_page: 233
    - "no": 5
      title: QUOTIENT OF A MANIFOLD BY A LIE GROUP
      page: 217
      pdf_page: 235
    - "no": 6
      title: HOMOGENEOUS SPACES AND QUOTIENT GROUPS
      page: 219
      pdf_page: 237
    - "no": 7
      title: ORBITS
      page: 222
      pdf_page: 240
    - "no": 8
      title: VECTOR BUNDLES WITH OPERATORS
      page: 223
      pdf_page: 241
    - "no": 9
      title: LOCAL DEFINITION OF A LIE GROUP
      page: 226
      pdf_page: 244
    - "no": 10
      title: GROUP GERMS
      page: 228
      pdf_page: 246
    - "no": 11
      title: LAW CHUNKS OF OPERATION
      page: 231
      pdf_page: 249
statements: 54
exercises: 10
content_sha256: 0cecf36d2acec4061eaebeb670f764476d17d4d4f06054c16cb39a13cb14dfa3
translated_from: content/en/lie/III/01_s1_lie_groups.md
translation_method: google
source_content_sha256: c28e00b85f74025ecd9db6adb574f2c95ce70e7ad72db45eba1ee38c85b62c4a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 1e3b6726374a57c1ff8e9e45fe9092c2febe2afc713435bca327b855daaa332c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。 李群

### 1. 定义 / 李群

令 G 为集合。如果以下条件成立，则群结构和 G 上的解析 K 流形结构称为兼容：
(GL) $G \times G$ 映射 $(g, h) \mapsto gh^{-1}$ 入 G 解析。

#### 定义 1 {#lie-iii-s1-def-1 .statement tag=0A76}

*K 上的李群是集合 G 与群结构和解析 K 流形结构，使得这两个结构兼容。*

李群超过$\mathbf{R}$（分别为$\mathbf{C}$、$\mathbf{Q}_p$）称为实数（分别为复数、$p$-adic）李群。

设 G 为群，解析式为流形结构。对于 G 中的 $g, h, g_0, h_0$，
$$
gh^{-1} = (g_0 h_0^{-1}) h_0 ((g_0^{-1} g)(h_0^{-1} h)^{-1}) h_0^{-1}.
$$
由此可见，G 是李群当且仅当以下三个条件成立：

(GL$_1$) 对于所有 $g_0 \in G$, 映射 $g \mapsto g_0 g$ G 到 G 是解析的；
(GL$_2$) 对于所有$g_0 \in G$，G 的映射 $g \mapsto g_0 g g_0^{-1}$ 到 G 中是在 $e$ 的开邻域中解析；
(GL$_3$) $G \times G$ 的映射 $(g, h) \mapsto gh^{-1}$ 到 G 中，在 $(e, e)$ 的开邻域上解析。

令 G 为李群。对于所有$g \in G$，$\gamma(g)$和$\delta(g)$是G的基础流形的自同构。因此，这个流形是纯的（*可微分和解析流形*，R，5.1.7）。特别是，对于所有 $g \in G$，G 在 $g$ 处的维数等于 $\dim G$（回想一下，$\dim G$ 是整数 $\geqslant 0$ 或 $+\infty$）。

由于解析映射是连续的，李群是一个拓扑群，其底层拓扑为流形结构。令 G 为集合。如果群结构和流形结构兼容并且 G 上的拓扑是拓扑底层流形，则 G 上的拓扑群结构和解析 K 流形结构称为*相容的* 结构。

#### 引理 1 {#lie-iii-s1-lem-1 .statement tag=0A77}

*设 G 为李群，U 是 e 的开邻域，E 是完全规范的空间，$\phi : U \to E$ 流形 G 的图表。存在包含在 U 中的 e 的邻域 W，使得 $\phi | W$ 是 W 的同构（其中右均匀结构）到$\phi(W)$（由E上的均匀结构引起）。*

可以假设$\phi(e) = 0$。让$U' = \phi(U)$。令$\psi : U' \to U$为$\phi$的逆映射。令V是e的对称开邻域，使得$V^2 \subset U$并令$V' = \phi(V)$。我们将$V' \times V'$中的定义映射$\theta_1, \theta_2$转换为$V' \times U'$如下：
$$
\begin{align*}
\theta_1(x, y) &= (x, \phi(\psi(x)\psi(y)^{-1})) \\
\theta_2(x, y) &= (x, \phi(\psi(y)^{-1}\psi(x))).
\end{align*}
$$
立即验证$\theta_2(\theta_1(x, y)) = \theta_1(\theta_2(x, y)) = (x, y)$对于$x, y$足够接近0。另一方面，$\theta_1$和$\theta_2$是解析的，因此在$(0, 0)$处严格可微。因此（*可微分和解析流形*，R，1.2.2）$V'$中存在0的邻域$W'$和常数$a > 0, b > 0$使得
$$
a(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
\leq \|x_1 - x_2\| + \|y_1 - y_2\|
\leq b(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
$$

对于$W'$中的所有$x_1, x_2, y_1, y_2$。写$x_1 = x_2 = y_2$，我们得到

$$
(2) \quad a \| \phi(\psi(x_1)\psi(y_1)^{-1}) \| \leq \| x_1 - y_1 \| \leq b \| \phi(\psi(x_1)\psi(y_1)^{-1}) \|.
$$

对于$\delta > 0$，令$N_\delta$为有序对$(x, y) \in W' \times W'$的集合，使得$\| x - y \| \leq \delta$。 $N_\delta$形式是$W'$中随行人员的基本系统。我们写$W = \psi(W')$。令$M_\delta$为有序对$(u, v) \in W \times W$的集合，使得$\| \phi(uv^{-1}) \| \leq \delta$。 $M_\delta$形式是$W$中随行人员的基本系统，配有正确的制服结构。但关系(2)证明了

$$
N_\delta \subset (\phi \times \phi)(M_{a^{-1}\delta}), \qquad (\phi \times \phi)(M_\delta) \subset N_{b\delta}
$$

因此 $W$ 的性质为引理。

#### 命题 1 {#lie-iii-s1-prop-1 .statement tag=0A78}

*李群是一个完整的可度量拓扑群。*

由于 $e$ 承认一个开邻域同胚于一个范数空间的开球，$e$ 承认邻域的一个可数基本系统，其交是 $\{e\}$。因此 $G$ 是可度量的（*一般拓扑*、章 III, § 1，命题 2 和章 IX, § 3、命题 1 的推论）。到引理 1，存在$e$的邻域，它在正确的制服结构下是完整的，因此$G$是完整的（*一般拓扑*，章III, § 3，命题4）。

#### 命题 2 {#lie-iii-s1-prop-2 .statement tag=0A79}

*令$G$为李群。*
(i) *如果$K = \mathbf{R}$或$\mathbf{C}$，$G$是本地连接的。*
(ii) *如果 $K$ 不同于 $\mathbf{R}$ 和 $\mathbf{C}$，则 $G$ 为零维*（*一般拓扑*、章 IX, § 6、定义 5）。
(iii) *假设 $K$ 是局部紧致的。为了使 $G$ 局部紧致，$G$ 是有限维的是必要且充分的。*
(iv) *如果$G$由子空间生成，而拓扑承认可数基，则$G$上的拓扑承认可数基。*

设$U$为$e$的邻域。存在包含在$U$中的$e$的开邻域$U_1$，并且同胚于$K$上的范数空间$E$的开球。若$K = \mathbf{R}$或$\mathbf{C}$，$U_1$连通，则证明(i)。假设 $K$ 是超度量的。存在 $e$ 的邻域 $U_2$，其在$G$ 中闭合，因此$U_2 \subset U_1$。那么$e$存在邻域$U_3$，使得$U_3 \subset U_2$和$U_3$相对于$U_1$开闭。那么$U_3$相对于$U_2$闭合，因此$G$相对于$U_1$开，因此$G$。这就证明了(ii)。为了使$G$局部紧致，$E$局部紧致是充分必要的；如果 $K$ 是局部紧致的，则相当于说，$E$ 是有限维的（*拓扑向量空间*、章 I, § 2、定理 3）、从而 (iii)。假设$G$是由子集$V$生成的，令$W = V \cup V^{-1}$；然后

$$
G = W \cup W^2 \cup W^3 \cup \ldots;
$$

如果$V$中存在序列稠密，我们看到G中存在序列稠密，并且由于G是可度量的（命题1），G上的拓扑承认可数基。

#### 推论{#lie-iii-s1-n1-cor-1 .statement tag=0A7A}

如果 K = R 或 C 并且 G 是连通且有限维的，则 G 是局部连通且局部紧的，并且其拓扑承认可数基。

#### 引理 2 {#lie-iii-s1-lem-2 .statement tag=0A7B}

设X为类C^r流形，X、U e 点和V开e的邻域和U×U的类C^r m映射转化为X满足以下条件：
(a) m(e, x) = m(x, e) = x 对于所有 x ∈ U；
(b) V ⊂ U, m(V × V) ⊂ U 且 m(m(x, y), z) = m(x, m(y, z)) 对于 V 中的所有 x, y, z。

那么在 V 和流形 W 中存在 e 的开邻域 W 和自同构 θ，使得 θ(e) = e, θ(θ(x)) = x 且 m(x, θ(x)) = m(θ(x), x) = e 对于所有 x ∈ W。

m(e, y) = y 对于所有 y ∈ U，因此，通过隐式函数定理，在 V 中存在 e 的开邻域 W_1 和 W_1 的类 C^r 到 V 的映射 θ_1，使得对于所有 x ∈ W_1，θ_1(e) = e, m(x, θ_1(x)) = e。类似地，存在V中e的开邻域W_2和W_2的类C^r到V的映射θ_2，使得θ_2(e) = e, m(θ_2(x), x) = e，对于所有x ∈ W_2。对于 x ∈ W_1 ∩ W_2，

$$
\begin{align*}
\theta_2(x) &= m(\theta_2(x), e) = m(\theta_2(x), m(x, \theta_1(x))) \\
&= m(m(\theta_2(x), x), \theta_1(x)) = m(e, \theta_1(x)) = \theta_1(x).
\end{align*}
$$

令 θ(x) 为 θ_1(x) 和 θ_2(x) 的公共的值，其中 x ∈ W_1 ∩ W_2。令 W 为 x ∈ W_1 ∩ W_2 的集合，使得 θ(x) ∈ W_1 ∩ W_2。 集合W 已打开。对于 x ∈ W，

$$
\theta(\theta(x)) = m(m(x, \theta(x)), \theta(\theta(x))) = m(x, m(\theta(x), \theta(\theta(x)))) = m(x, e) = x
$$

因此 θ(x) ∈ W。我们看到 θ | W 定义自同构流形 W。

#### 命题 3 {#lie-iii-s1-prop-3 .statement tag=0A7C}

设 X 为解析流形，m 为合成在 X 上承认单位元素的解析结合律律。 X 可逆元集合 G 在 X 开且 G 与 m 为李群 | (G × G) 和 X 引起的流形结构。

到引理 2，G 是单位元素的邻域。对于所有 g ∈ G，映射 x ↦ m(g, x) 是流形 X 的自同构。因此在映射下G的像是g的邻域，显然包含在G中。因此G在X中开。显然条件 (GL_1) 和 (GL_2) 成立。 条件 (GL_3) 满足引理 2。

例 / 李群

(1) 令 E 为 K 上的完全可范空间。 E × E 的映射 (x, y) ↦ x − y 到 E 中是连续且线性的，因此是解析的。

因此，E 及其加法群和解析流形结构，为李群。

特别地，K是李群。

(2) 设 A 是 K 上的完全规范单位结合律代数。 $A \times A$ 的乘法 $(x, y) \mapsto xy$ 到 A 是双线性且连续的，因此是解析的。 命题 3 表明 A 的可逆元的群 $A^*$ 在 A 中是开集（这也是从 *General 拓扑*、章 IX, § 3、命题 13 得出），并且 $A^*$ 是李群。

对于例，令 E 为 K 上的完全可范化空间，并令 $A = \mathscr{L}(E)$（*一般拓扑*、章 IX, § 3、命题 5）。那么 $A^*$ 就是 E 的自同构群 $\mathbf{GL}(E)$。 *因此，这个群在 K* 上具有规范的李群结构。更具体地，$\mathbf{GL}(n, K)$与由$\mathbf{M}_n(K)$上的流形结构诱发的李群。对于 $n = 1$，我们看到乘法群 $K^*$ 是李群以及由 K 上的流形结构引起的。

(3) 令G在K上李群。令$K' = \mathbf{R}$或$\mathbf{C}$或值域$K'$的非离散完全超度量域和$\sigma$同构到K的值子域上。则群 G，以及通过标量限制获得的 $K'$ 流形结构，在 $K'$ 上是李群，据说是*通过标量限制从李群 G 导出的*（从 K 到 $K'$ 通过$\sigma$）。对于例，每个复数李群都具有规范的实李群结构。同样，每个复数李群 G 都与一个复数李群相关联，称为 G 的 *共轭*，它是通过 $\mathbf{C}$ 的自同构 $z \mapsto \overline{z}$ 衍生自 G。

### 2. 态射李群

#### 定义 2 {#lie-iii-s1-def-2 .statement tag=0A7D}

*设G和H为李群。 G 到 H 的李群态射（或者简单地，如果不会引起混淆，G 到 H 的态射）是 G 到 H 的映射，它是群同态并且是解析的。 G 的自同构群表示为$\operatorname{Aut}(G)$.*。

G 的恒等映射是态射。两个态射的合成是态射。如果$f : G \to H$和$f' : H \to G$是两个逆态射，则$f$和$f'$是李群同构。

#### 例 {#lie-iii-s1-n2-exa-1 .statement tag=0A7E}

(1) 设G为李群。对于所有 $x \in G$，$\operatorname{Int}(x)$ 是李群 G 的自同构。

(2) 设G为李群。令$G^\vee$表示G的对数群，与G相同的流形结构。$G^\vee$是李群（称为G的*对数*李群），映射$g \mapsto g^{-1}$是直接的李群 G 的同构到李群 $G^\vee$。

(3) 设G为李群，E为完全可范空间。 G 在 E 上的*解析线性表示*（或者在不会产生混淆的情况下，简单地在 E 上解析 G 的线性表示）是李群 G 到李群 $\mathbf{GL}(E)$ 的态射，在其他字中，G 到映射 $\pi$ 的解析$\mathbf{GL}(E)$使得G中的$g, g'$有$\pi(gg') = \pi(g)\pi(g')$。假设E在K上承认有限的基$(e_1, e_2, \ldots, e_n)$；设$(e_1^*, e_2^*, \ldots, e_n^*)$为对偶基；令$\rho$为群G的同态变为群$\mathbf{GL}(E)$；那么下面的条件是等价的：
(i) $\rho$ 是解析线性表示；
(ii) 对于所有 $x \in E$ 和 $x' \in E'$，G 上的函数 $g \mapsto \langle \rho(g)x, x' \rangle$ 是解析的；
(iii) 对于所有 i 和 j，G 上的函数 $g \mapsto \langle \rho(g)e_i, e_j^* \rangle$ 是解析的。
对于 (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) 的含义是明确的。另一方面，函数$u \mapsto \langle ue_i, e_j^* \rangle$形式是$\mathscr{L}(E)$上的坐标系统；因此，它们的限制到$\mathbf{GL}(E)$形式是$\mathbf{GL}(E)$上的坐标系统，从而蕴涵(iii)$\Rightarrow$(i)。

设 G 为实李群，E 为群 G 的实数完全可规范空间和 $\rho$ 同态到群 $\mathbf{GL}(E)$。我们将在§ 8，定理 1 中看到，如果$\rho$是连续的（当$\mathbf{GL}(E)$具有从$\mathbf{L}(E)$上的范数导出的拓扑时），那么$\rho$是解析的。但注这个概念的连续性与积分中考虑的连续性不同，章VIII, § 2、定义1(iii)(习题1)。

(4) 设G为实李群，E为复数完全范数空间。 G 在 E 上的解析线性表示是 G 的态射到 $\mathbf{GL}(E)$ 的底层实李群。

#### 命题 4 {#lie-iii-s1-prop-4 .statement tag=0A7F}

设 G 和 H 为李群，群 G 的 f 同态为群 H。要使 f 解析，存在 G 的非空开子集 U 使得 $f|_U$ 解析是必要且充分的。

条件显然是必要的。假设它成立。对于所有$x_0 \in G$，$f(x_0x) = f(x_0)f(x)$对于所有$x \in U$，因此$f|_{x_0U}$是解析的。但是集合$x_0U$，其中$x_0 \in G$，形式是G的开覆盖。

#### 注 {#lie-iii-s1-n2-rem-1 .statement tag=0A7G}

如果 f 是 e 处的浸没（或 e 处的浸没），则显然 f 是浸没（或 e 处的浸没）。

### 3. 谎言子群

设G为G的李群和H子群，G同时是G的子流形。则$H \times H$到G的映射$(x, y) \mapsto xy^{-1}$是解析的，因此$H \times H$到H的映射$(x, y) \mapsto xy^{-1}$是解析的。 （可微分和解析流形，R，5.8.5）。因此，H 加上由 G 上的那些引起的群和流形结构，是李群。

#### 定义 3 {#lie-iii-s1-def-3 .statement tag=0A7H}

设G为李群。如果 H 是子群并且是 G 的子流形，则 G 的子集 H 称为李子群。

G 的开子群是 G 的谎言子群。特别是，如果 G 是实数或复数李群，则其恒等分量是 G 的谎言子群。

#### 命题 5 {#lie-iii-s1-prop-5 .statement tag=0A7I}

设 G 为李群，H 为 G 的谎言子群。
(i) H 在 G 中是闭的。
(ii) H 到 G 的典范嵌入是李群态射。
(iii) 设L为李群，L的f映射进入G，使得f(L)⊂H。对于f为L的态射进入H，f为L的态射进入G是充分必要的。

由可微分和解析流形，R，5.8.3，H 是局部闭的。因此 H 是闭的（通则拓扑、章 III, § 2、命题 4）。 断言 (ii) 是显而易见的。 断言 (iii) 由可微分和解析流形, R, 5.8.5 得出。

#### 命题 6 {#lie-iii-s1-prop-6 .statement tag=0A7J}

设G是G的李群和H子群。要使H成为G的谎言子群，充分必要条件是存在点h ∈ H和G中h的开邻域U，使得H∩U是G的子流形。

条件显然是必要的。假设它成立。对于所有 h' ∈ H，平移 γ(h'h^{-1}) 是流形 G 的自同构和映射 U 的子流形 H ∩ U 到 h'h^{-1}U 的子流形 (h'h^{-1}H) ∩ (h'h^{-1}U)。由于 h'h^{-1}H = H 且 h'h^{-1}U 是 G 中 h' 的开邻域，我们看到 H 的每个点都有一个开邻域 V，使得 V ∩ H 是 G 的子流形。因此 H 是 G 的子流形。

设 G 是李群，H 是 G 的谎言子群。如果 L 是 H 的谎言子群，则通过可微分和解析流形，R，5.8.6，L 是 G 的谎言子群。设M是G的谎言子群，使得M⊂H。那么M是H的谎言子群，因为M到H的典范嵌入显然是浸没。

令 k 为 K 的非离散闭子域。G 的李 k 子群是 G 的底层李 k 群的李子群。

#### 注 {#lie-iii-s1-n3-rem-1 .statement tag=0A7K}

如果将定义 3 中的“子流形”替换为“拟子流形”，我们就得到 G 的李拟子群定义。（对于有限维 G，李拟子群就是李子群。）假设 K 的特征为 0。命题 5 仍然有效。 证明为李拟子群。 命题 6 对于相同的证明、替换仍然有效，“李准子群”的“李子群”和“拟子流形”的“子流形”。

### 4. 半直接乘积 OF 李群

令 I 为有限集合且 (L_i)_{i \in I} 为李群族。 L = \prod_{i \in I} L_i 上的群和流形结构是兼容的，因此 L 具有李群结构。 L 称为李群 (L_i)_{i \in I} 家族的乘积李群。

令L和M为L的李群和σ同态进入群M的自同构群。令S为M相对于σ的L的外部半直接乘积（代数，章） I, § 6, no. 1、定义 2)。

#### 命题 7 {#lie-iii-s1-prop-7 .statement tag=0A7L}

*如果映射* $(m, l) \mapsto \sigma(l)m$ *of* $M \times L$ *进入* $M$ *是解析的，群* $S$，*与乘积流形结构 of* $M$ *和* $L$， *是李群*。

对于$L$中的$l, l'$和$M$中的$m, m'$，

$$
(m, l)(m', l')^{-1} = ml{l'}^{-1}{m'}^{-1} = m(\sigma(l{l'}^{-1}){m'}^{-1})l{l'}^{-1}
= (m(\sigma(l{l'}^{-1}){m'}^{-1}), l{l'}^{-1})
$$

从而命题。

如果命题 7 的条件成立，李群 $S$ 被称为* $L$ *通过* $M$ *相对于* $\sigma$ 的 (*外部*) *半直接乘积李群。

显然，$L$（或$M$）的典范嵌入到$S$是$L$（或$M$）的同构到$S$的谎言子群，我们用认同和$L$ （分别$M$）。 $S$到$L$的典范映射是李群态射。

相反，令$G$为李群和$L$，$M$两个谎言子群，使得群$G$（代数上）是$L$乘$M$的半直接乘积 （*代数*、章I, § 6, no. 1）。 我们将$l \in L$和$m \in M$写为$\sigma(l)m = lml^{-1}$。 那么$\sigma$满足命题7中的条件。 We can therefore form the semi-direct product Lie group $S$ of $L$ by $M$ relative to $\sigma$. $S$到$G$的映射$j: (m, l) \mapsto ml$是群同构并且是解析的。 如果$j$是李群同构，则*李群*$G$*被称为*$L$*的半直接乘积*通过*$M$*和*$S$*和*$G$*进行识别*。 对于所有$g \in G$，我们写为$g = p(g)q(g)$，其中$p(g) \in M$和$q(g) \in L$。 为了使李群$G$成为$L$乘$M$的半直接乘积，映射$p: G \to M$和$q: G \to L$之一是解析的是必要且充分的，在这种情况下两者都是解析的；或者，$T_e(G)$是$T_e(M)$和$T_e(L)$的拓扑直和是必要且充分的（因为，如果条件成立，$j$在$e_S$处是étale）。

#### 例 {#lie-iii-s1-n4-exa-1 .statement tag=0A7M}

Let $E$ be a normable space, $G = \mathbf{GL}(E)$, $T$ the translation group of $E$ and $A$ the permutation group of $E$ generated by $G$ and $T$. 群$A$在代数上是$G$乘以$T$的半直乘积。 （如果$E$是有限维的，则$A$是$E$、cf. *代数*、章II, § 9, no. 4的仿射群）。 令$\sigma$为$G$在$E$上的恒等式线性表示，$S$为$G$通过$E$相对于$\sigma$的外部半直接乘积。 对于所有$x \in E$，令$t_x$为由$x$定义的$E$的平移。 映射 $(x, u) \mapsto t_x \circ u$ 是群 $S$ 的同构 $\Phi$ 到群 $A$。 $E \times \mathscr{L}(E)$到$E$的映射$(x, u) \mapsto \sigma(u)x = u(x)$是连续且双线性的，因此是解析的；因此，它的限制到 $E \times G$ 是解析的。 因此，群$S$，加上$E$和$G$的乘积流形结构，就是李群。 我们通过$\Phi$将迁移这个结构到$A$。 那么$A$就变成李群，$G$的内部半直接乘积由$T$变为李群。

#### 命题 8 {#lie-iii-s1-prop-8 .statement tag=0A7N}

*设*$G$*和*$H$*为李群、$p: G \to H$和$s: H \to G$李群态射，使得*$p \circ s = \mathrm{id}_H$*和*$N = \mathrm{Ker}\ p$。 *那么* $N$ *是* $G$的谎言子群，*s是* $H$的同构 *到* $G$的谎言子群 *并且李群* $G$ *是内部半直接乘积的*$s(H)$*由*$N$。

$T_e(p) \circ T_e(s) = \mathrm{id}_{T_{e(H)}}$，因此$p$（或$s$）是浸没（或浸没）。通过 *可微分和解析流形*，R，5.10.5，N 是 G 的谎言子群。另一方面，$s$ 是 H 到 $s(H)$ 的同胚，因此 $s$ 是 H 的同构到 G 的谎言子群 （*可微分和解析流形*，R，5.8.3）。最后，对于所有$g \in G$，$g = (s \circ p)(g) \cdot n$对于某些$n \in N$；由于 $s \circ p$ 是解析的，李群 G 是 $s(H)$ 通过 N 的半直接乘积。

### 5. 流形除以李群的商

设G为类$C^r$的李群、X流形和左运算(*代数*、章I, § 5, no. 1)的$(g, x) \mapsto gx$律 X 上 G 的类$C^r$。对于所有$g \in G$，让$\tau(g)$表示由g定义的X的自同构$x \mapsto gx$。对于所有$x \in X$，让$\rho(x)$表示G到由x定义的X的轨道映射$g \mapsto gx$。然后

$$
\rho(x) = \rho(gx) \circ \delta(g), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \gamma(g^{-1})
$$

对于所有 $g \in G$ 和 $x \in X$。因此

$$
T_g(\rho(x)) = T_e(\rho(gx)) \circ T_g(\delta(g))
$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\gamma(g^{-1}))
$$

#### 命题 9 {#lie-iii-s1-prop-9 .statement tag=0A7O}

*让$x \in X$和$g_0 \in G$。*

(i) *如果$\rho(x)$是$g_0$的浸没（分别是浸没、浸没），那么对于所有$g \in G$，$\rho(gx)$是浸没（分别是浸没、浸没）。*

(ii) *如果 $\rho(x)$ 在 $g_0$ 处具有秩 k，则对于所有 $g \in G$，$\rho(gx)$ 的常数秩等于 k。*

由于 $T_g(\delta(g)), T_x(\tau(g))$ 和 $T_g(\gamma(g^{-1}))$ 是同构，因此这紧随公式 (4) 和 (5)。

#### 推论{#lie-iii-s1-n5-cor-1 .statement tag=0A7P}

*让$x \in X$。如果 K 的特征为 0 并且 X 是有限维的，则 $\rho(x)$ 是浸没。如果进一步 $\rho(x)$ 是单射的，$\rho(x)$ 是浸入式。*

这是从命题 9 和*可微分和解析流形*，R，5.10.6 得出的。

观察到，如果 $\eta$ 表示 $G \times X$ 的映射 $(g, x) \mapsto gx$ 到 X，那么，对于 $g \in G, x \in X, u \in T_g(G), v \in T_x(X)$，

$$
T_{(g, x)}(\eta)(u, v) = T_{(g, x)}(\eta)(u, 0) + T_{(g, x)}(\eta)(0, x)
$$

那就是

$$
T_{(g, x)}(\eta)(u, v) = T_g(\rho(x))u + T_x(\tau(g))v.
$$

#### 命题 10 {#lie-iii-s1-prop-10 .statement tag=0A7Q}

*设G为类$C^r$的李群和X流形，以及X上G的类$C^r$的左运算律。假设：*

(a) *群G在X上正常且自由地运行；*

(b) *对于所有 $x \in X$，$\rho(x)$ 是浸没（如果 K 具有特征 0 并且 X 是有限维，则为 (a) 的推论）。*

那么 G 在 X 上定义的等价关系是正则的（可微且解析流形，R，5.9.5）。 商集 X/G 上存在且仅有一个流形结构，使得典范映射 $\pi : X \to X/G$ 是淹没。这个流形结构的基础拓扑是X的商拓扑；这是豪斯多夫。最后，$(X, G, X/G, \pi)$是主左纤维束。\脚注{†可微分和解析流形，R，6.2.1中定义的主纤维束是主右纤维束。主左纤维束的定义可以由此以明显的方式推导出来。}

设$\theta$为$G \times X$的映射$(g, x) \mapsto (x, gx)$到$X \times X$。这个映射是类$C^\tau$。我们证明这是一种沉浸。对于 $u \in T_g(G)$ 和 $v \in T_x(X)$，通过 (6)，

$$
T_{(g, x)}(\theta)(u, v) = (v, T_g(\rho(x))u + T_x(\tau(g))v).
$$

但 $T_g(\rho(x))$ 是假设 (b) 的单射，因此 $T_{(g, x)}(\theta)$ 是单射的。它的像是$v \in T_x(X)$和子空间的向量$(v, T_x(\tau(g))v)$的子空间$H_{g, x}$由……组成的拓扑直和

$$
I_{g, x} = \{0\} \times T_g(\rho(x))(T_g(G)).
$$

到假设(b)，$T_g(\rho(x))(T_g(G))$在$T_{gx}(X)$中承认拓扑补充$J_{g, x}$。因此，$T_{(g, x)}(\theta)$的像承认拓扑补充$\{0\} \times J_{g, x}$。因此我们证明了$\theta$是$G \times X$在$X \times X$的浸没。

由于 G 在 X 上自由运行，$\theta$ 是单射的。令C为G在X上定义的等价关系R的图。当 G 正确运行时，$\theta$ 是$G \times X$ 到C 的同胚（一般拓扑、章 I, § 10、命题 2）。通过可微分和解析流形，R，5.8.3，它是$X \times X$的子流形，$\theta$是流形$G \times X$到流形C的同构。切线空间 $T_{(x, gx)}(C)$ 标识为

$$
T_{(g, x)}(\theta)(T_{(g, x)}(G \times X)) = H_{g, x} \oplus I_{g, x} \subset T_{(x, gx)}(X \times X).
$$

令 pr$_1$ 和 pr$_2$ 为$X \times X$到两个因子的规范投影。 $T_{(x, gx)}(\mathrm{pr}_1)$映射$H_{g, x}$到$T_x(X)$是直接的，$T_{(x, gx)}(\mathrm{pr}_1) | T_{(x, gx)}(C)$的核是$I_{g, x}$。因此，$\mathrm{pr}_1 | C$ 是C 淹没在X 上。由可微分和解析流形，R，5.9.5，R 是正则的。因此，到定义时，商集X/G上存在且仅一个流形结构，使得$\pi$是淹没。 X/G 的基础拓扑是X 的商拓扑（可微分和解析流形，R，5.9.4）。这个拓扑是Hausdorff（一般拓扑、章III, § 4、命题3）。

对于所有 $b \in X/G$，存在 b 的开邻域 W 和态射 $\sigma : W \to X$，使得 $\pi \circ \sigma = \mathrm{id}_W$（可微分和解析流形，R，5.9.1）。令$\phi$为$G \times W$的双射$(g, w) \mapsto g\sigma(w)$到$\pi^{-1}(W)$。它是类$C^\tau$。然后 $\pi(g\sigma(w)) = w$ 和

$$
\theta^{-1}(\sigma(w), g\sigma(w)) = (g, \sigma(w))
$$

因此，$\phi$的逆双射等于类$C^r$。显然 $\phi(gg', w) = g\phi(g', w)$ 对应 $w \in W,\ g \in G,\ g' \in G$。因此 $(X, G, X/G, \pi)$ 是主左纤维丛。

#### 注 {#lie-iii-s1-n5-rem-1 .statement tag=0A7R}

With the above hypotheses, further let $H$ be a manifold of class $C^r$ and $(x, h) \mapsto m(x, h)$ a mapping of class $C^r$ of $X \times H$ into $X$ such that $m(gx, h) = gm(x, h)$ for $x \in X,\ g \in G,\ h \in H$. 令 $n$ 为 $(X/G) \times H$ 的映射到由 $m$ 取商得出的$X/G$。 我们证明 $n$ * 是类* $C^r$。 考虑图表

$$
\begin{array}{ccc}
X \times H & \xrightarrow{m} & X \\
\pi \times 1 \downarrow & & \downarrow \pi \\
(X/G) \times H & \xrightarrow{n} & X/G
\end{array}
$$

它是可交换的，$\pi \circ m$是类$C^r$，$\pi \times 1$是满射淹没；那么应用*可微分和解析流形*，R，5.9.5就足够了。

设$G$为李群、类$C^r$的$X$流形和$G$的类$C^r$右运算$(g, x) \mapsto xg$律 $X$。让 $\tau(g)x = \rho(x)g = xg$ 代表 $g \in G,\ x \in X$。那么这次

$$(3')$$
$$
\rho(x) = \rho(xg) \circ \gamma(g^{-1}), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \delta(g)
$$
因此
$$(4')$$
$$
T_g(\rho(x)) = T_e(\rho(xg)) \circ T_g(\gamma(g^{-1}))
$$
$$(5')$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\delta(g)).
$$

另一方面，如果$\eta$表示$G \times X$的映射$(g, x) \mapsto xg$进入$X$，则公式（6）仍然有效。 命题 9，其推论和命题 10 仍然同样正确（最后将“主左纤维束”替换为“主右纤维束”）。

### 6. 同质空间和商群

#### 命题 11 {#lie-iii-s1-prop-11 .statement tag=0A7S}

*令$X$为李群，且$G$是$X$的谎言子群。*

(i) *在齐次集合$X/G$上存在且仅有一个解析流形结构，使得$X$到$X/G$的规范投影$\pi$是淹没。 $X/G$上$X$运算律解析。对于所有$x \in X$，$T_x(\pi)$的核是通过$T_e(\gamma(x))$从$T_e(G)$获得的。*

(ii) *如果$G$在$X$中正常，则$X/G$是李群，其群结构和流形结构在(i)中定义。 映射$\pi$是李群态射。*

通过*通用拓扑*、章III, § 4, no. 1、*例1*、$G$通过正确的翻译在$X$上正确且自由地运行。因此 (i) 的第一个断言由

命题 10 个，共 no. 5。第二个来自 no. 5 的注。由于 $\pi$ 是淹没，$T_x(\pi)$ 的核是 $x$ 处的切线空间
$$
\pi^{-1}(\pi(x)) = xG = \gamma(x)(G)
$$
因此由$T_e(G)$通过$T_e(\gamma(x))$获得。

假设$G$是正规的。设 $m$ 为 $(X/G) \times (X/G)$ 的映射 $(x, y) \mapsto xy^{-1}$ 到 $X/G$。然后$(m \circ (\pi \times \pi))(x, y) = \pi(xy^{-1})$对于$X$中的所有$x, y$。因此 $m \circ (\pi \times \pi)$ 是解析的。由于 $\pi \times \pi$ 是满射淹没，$m$ 是解析的（可微分和解析流形，R. 5.9.5），从而 (ii)。

(i) 中定义的齐次集合 $X/G$ 与流形结构称为 $X$ 与 $G$ 的商（左）李齐次空间。 （右）李齐次空间 $G \setminus X$ 的定义类似。当$G$正常时，(ii)中定义的李群$X/G$称为$X$除以$G$的商李群。

#### 命题 12 {#lie-iii-s1-prop-12 .statement tag=0A7T}

令$X$为李群，$Y$为非空解析流形，其中律为$Y$上$X$的解析左运算。对于所有$y \in Y$，令$\varphi(y)$为$X$中$y$的$y$和$X_y$稳定子的轨道映射。以下条件是等效的：
(i) 存在$y \in Y$使得$\varphi(y)$是满射淹没；
(i') 对于所有 $y \in Y$，$\varphi(y)$ 是满射淹没；
(ii) 存在$y \in Y$，使得$X_y$是$X$的谎言子群，并且$X/X_y$到$Y$的典范映射是流形同构；
(ii') 对于所有$y \in Y$，$X_y$是$X$的谎言子群，而$X/X_y$的典范映射进入$Y$是流形同构；
(iii) $X \times Y$到$Y \times Y$的映射$(x, y) \mapsto (y, xy)$是满射淹没。

由于$X$到$X/X_y$的典范映射是浸没，因此等价 (i) $\Leftrightarrow$ (ii)、(i') $\Leftrightarrow$ (ii') 是直接的。 (i) $\Leftrightarrow$ (i') by 命题 9 of no. 5。 等价 (i') $\Leftrightarrow$ (iii) 由no. 5 的公式 (7) 得出。

在命题 12 的条件下，$Y$ 称为$X$ 的（左）李齐次空间。 $X$ 的右李齐次空间类似地定义。

#### 例 {#lie-iii-s1-n6-exa-1 .statement tag=0A7U}

设$G$为李群。我们让$G \times G$对$(g_1, g_2)x = g_1xg_2^{-1}$左边的$G$进行操作。令$\rho$为$e$的轨道映射。然后从$T_{(e, e)}(\rho)$到$T_{(e, e)}(G \times \{e\}) = T_e(G) \times \{0\}$再到限制
$$
T_{(e, e)}(\{e\} \times G) = \{0\} \times T_e(G)
$$
其中空间中有同构到 $T_e(G)$ 上。因此，$T_{(e, e)}(\rho)$是满射，并且$\operatorname{Ker} T_{(e, e)}(\rho)$承认例的拓扑补充$T_e(G) \times \{0\}$在$T_{(e, e)}(G \times G)$中。因此 $\rho$ 是$(e, e)$ 的浸没。因此$G$是$G \times G$的左李齐次空间。

#### 命题 13 {#lie-iii-s1-prop-13 .statement tag=0A7V}

设$G$为李群，$H$为$G$的正常谎言子群，类$C^r$的$X$流形以及$(g, x) \mapsto gx$律的左运算 $X$ $G$ 类 $C^r$。假设命题 10 的条件(a)和(b)成立。

(i) $X$上$H$的左运算$(h, x) \mapsto hx$的律满足命题10的条件(a)和(b)（这样我们就可以考虑流形$X/G$和$X/H$的商）。

(ii) $X$定义上$G$左运算律取$X/H$上$G/H$类$C^r$左运算的商律；这个律满足命题10的条件(a)和(b)（这样我们就可以考虑商流形$(X/H)/(G/H)$）。

(iii) 将$X$的典范映射代入$X/H$定义，将$X/G$的商双射代入$(X/H)/(G/H)$。这个双射是类$C^r$流形同构。

显然$H$在$X$上自由运行；它通过*一般拓扑*，章III, § 4, no. 1，*例*正常运行。 1. $X$上$H$的轨道映射是浸没，因为$H$的典范嵌入到$G$是浸没。这就证明了(i)。

$X$上$G$左运算律显然是定义，在求商上，$X/H$上$G/H$左运算律。这个律是类$C^r$的*可微分和解析流形*，R，5.9.6。设$g \in G$和$x \in X$使得$(Hg)(Hx) = Hx$；然后$H(gx) = Hx$，因此$gx \in Hx$和$g \in H$；这证明了$G/H$可以在$X/H$上自由运行。 $G \times X$到$X \times X$的映射$\theta : (g, x) \mapsto (x, gx)$已关闭；另一方面，$\theta(Hg \times Hx) = Hx \times H(gx)$；紧接着映射

$$(Hg, Hx) \mapsto (Hx, H(gx))$$

$(G/H) \times (X/H)$ 到 $(X/H) \times (X/H)$ 是闭合的；而且$G/H$可以在$X/H$上自由运行，定理*一般拓扑*的1(c)，章I, § 10, no. 2证明$G/H$可以在$X/H$上正常运行。

设$\pi$是$X$的典范映射到$X/H$，$G$的$\sigma$典范映射到$G/H$，$X$和$y = \pi(x)$的$x$元素。

$$
\begin{array}{ccc}
G & \xrightarrow{\rho(x)} & X \\
\downarrow \sigma & & \downarrow \pi \\
G/H & \xrightarrow{\rho(y)} & X/H
\end{array}
$$

然后 $\pi \circ \rho(x) = \rho(y) \circ \sigma$ 因此

$$
T_x(\pi) \circ T_e(\rho(x)) = T_e(\rho(y)) \circ T_e(\sigma).
$$

设$u \in T_e(G/H)$使得$T_e(\rho(y))u = 0$。存在$v \in T_e(G)$使得$u = T_e(\sigma)v$。那么$T_x(\pi)(T_e(\rho(x))v) = 0$，因此$T_e(\rho(x))v$与$Hx$相切（*可微且解析流形*，R，5.10.5），因此对于某些$v' \in T_e(H)$来说，形式$T_e(\rho(x) | H)v'$。由于$T_e(\rho(x))$是单射的，因此有$v = v'$、从而$v \in T_e(H)$，因此$u = 0$。因此 $T_e(\rho(y))$ 是单射的。 $T_e(\rho(y))$的像等于$T_x(\pi) \circ T_e(\rho(x))$；现在$T_e(\rho(x))$的像在$T_x(X)$和$T_x(\pi)$的包含核承认拓扑补充。因此可见$\rho(y)$是沉浸，它完成了(ii)的证明。

断言 (iii) 由上述和可微分和解析流形, R, 5.9.7 得出。

#### 推论{#lie-iii-s1-n6-cor-1 .statement tag=0A7W}

设 G 为李群和 H 以及 L G 的正规李子子群和 L ⊂ H。则 H/L 是 G/L 的正规李子子群以及 G/H 的规范双射到(G/L)/(H/L) 为李群同构。

### 7. ORBITS

#### 命题 14 {#lie-iii-s1-prop-14 .statement tag=0A7X}

设 G 为李群、X 解析流形以及 (g, x) ↦ gx 律 G 在 X 上的解析左运算。设 x ∈ X。假设相应的轨道映射 ρ(x) 是浸没（如果 K 具有特征 0 并且 X 是有限维（命题 9 的推论），则总是这种情况）。令 G_x 为 G 中 x 的稳定子。
(i) G_x 是谎言子群并且 T_e(G_x) = Ker T_e(ρ(x))。
(ii) 齐次空间 G/G_x 到X 的典范映射 i_x 是像 Gx 的浸没。
(iii) 如果另外轨道 Gx 是局部闭的，且 G 上的拓扑承认可数基，则 Gx 是 X 的子流形，i_x 是流形 G/G_x 到流形 Gx 上的同构，且 T_x(Gx) = Im T_e(ρ(x))。

x 在 ρ(x) 下的逆像是 G_x。由于 ρ(x) 是浸没，G_x 是子流形，并且对于所有 g ∈ G，gG_x = ρ_{(x)}^{-1}(gx) 在 g 处的切线空间 J 为 Ker T_g(ρ(x)) （可微分和解析流形，R，5.10.5），从而 (一).令 π: G → G/G_x 为典范映射。那么 i_x ∘ π = ρ(x)。由于 G/G_x 是 G 的商流形，因此等式证明 i_x 是解析的。此外，T_g(ρ(x))和T_g(π)的核都等于J。因此T_{π(g)}(i_x)是单射的。 T_{π(g)}(i_x) 的像等于 T_g(ρ(x)) 的像，因此承认拓扑补充。这就证明了(ii)。

假设Gx是局部闭的。 Gx 的每个点在 Gx 中都有邻域，它同胚于完全度量空间的闭子空间，因此是 Baire 空间。因此 Gx 是 Baire 空间（一般拓扑、章 IX, § 5、命题 4）。如果 G 具有可数基，则 i_x 是 G/G_x 到 Gx 的同胚（一般拓扑、章 IX, § 5）。然后通过 (ii) 可微分和解析流形，R，5.8.3，i_x 是流形 G/G_x 的同构到流形 Gx 上并且

$$
T_x(Gx) = \operatorname{Im} T_{\pi(e)}(i_x) = \operatorname{Im} T_e(\rho(x)).
$$

#### 注 {#lie-iii-s1-n7-rem-1 .statement tag=0A7Y}

设G是类C^r的有限维李群、X流形和X上G的类C^r的左运算的(g, x)↦gx律。那么命题14仍然有效。唯一需要不同的证明的点是G_x是谎言子群这一事实。但如果 r ≠ ω，则 K = \mathbf{R}；显然 G_x 是闭集，G_x 是 § 8、定理 2 的谎言子群。

#### 推论{#lie-iii-s1-n7-cor-1 .statement tag=0A7Z}

设G为李群，其拓扑允许可数基和X一个非空有限维解析流形，其中律为G在X上的解析左运算。假设 G 在 X 上运算传递性，并且 K 的特征为 0。则 X 是 G 的李齐次空间。

设 x ∈ X。 x 的轨道等于 X，是闭集，因此我们可以应用命题 14 (iii)。

### 8. 向量丛与操作员

令G为类C^r的李群、X流形和X上G的类C^r的左运算的(g,x)↦gx律。设E为类C^r的向量丛，其中基空间X和π：E→X投影到X。对于所有 x ∈ X，令 E_x 为 E 在 x 处的纤维。令 (g, u) ↦ gu 为 E 上 G 左侧运算的律，使得 π 与 X 和 E 上 G 的运算兼容。对于所有 g ∈ G 且所有 x ∈ X、限制到映射 u ↦ 的 E_x gu 是 E_x 到 E_{gx} 的双射 ψ_{g, x}。我们假设，对于所有 g ∈ G 和所有 x ∈ X，ψ_{g, x} 是连续且线性的，因此是可规范空间 E_x 的同构到可规范空间 E_{gx} 上。

令 φ 为流形 G × X 的自同构 (g, x) ↦ (g, gx)。令 p 为 G × X 在 X 上的规范投影以及 p 下 E 的 E' 逆像。令 ψ : E' → E' 为 ψ_{g, x} : E'_{(g, x)} → E'_{(g, gx)} 的映射和。

#### 定义 4 {#lie-iii-s1-def-4 .statement tag=0A80}

如果ψ是类C^r的向量丛的φ-态射，则E称为类C^r的向量G丛。

在其他字中，E 是类 C^r 的向量 G 丛，如果对于所有 (g_0, x_0) ∈ G × X，以下条件成立：在 G × X 中存在 (g_0, x_0) 的开邻域 U，这样那，如果 E' | U（分别为 E' | φ(U)）通过向量图与纤维 M（分别为 N）的平凡向量丛进行识别，U 的映射 (g, x) ↦ ψ_{g, x} 到 L(M, N) 中的值为类 C^r。

映射 ψ 显然是双射的，根据上面的局部准则可知 ψ^{-1} 是向量丛的 φ^{-1} 同构，因此 ψ 是向量丛的 φ 同构。

基 X 的平凡向量 G 丛是向量丛 X × F（其中 F 是完全可规范空间），其中律为运算 (g, (x, f)) ↦ (gx, f) G 上X×F。

我们再次假设假设 和记号位于定义 4 之前，并进一步将 τ 视为类 C^r 对于同构的向量函子（可微且解析流形，R，7.6.6）。那么 τE 就是向量丛和基空间 X。对于所有 x ∈ X，其纤维 (τE)_x 等于 τ(E_x)。对于所有可规范空间 N_1, N_2，令 Isom(N_1, N_2) 表示 N_1 的同构到 N_2 的集合。如果 g ∈ G，则

$$
\tau(\psi_{g, x}) \in \mathrm{Isom}((\tau E)_x, (\tau E)_{gx}).
$$

G 在 τE 上的左运算 (g, u) ↦ gu 的 τ(ψ_{g, x}) 定义律以及 τE 在 X 上的规范投影与 G 在 X 和 τE 上的运算兼容。

#### 命题 15 {#lie-iii-s1-prop-15 .statement tag=0A81}

*如果E是类C^r的向量G丛，则τE是类C^r的向量G丛*。

设g_0, x_0, U, M, N如定义 4后面的段落。那么U的映射 (g, x) ↦ τ(ψ_{g,x})到$\mathscr{L}(\tau M, \tau N)$就是映射 (g, x) ↦ ψ_{g,x}到$\mathscr{L}(M, N)$的合成将 Isom(M, N) 的映射 f ↦ τ(f) 转化为 Isom(τM, τN)；这两个映射属于类C^r，因此它们的合成、从而命题也是。

#### 命题 16 {#lie-iii-s1-prop-16 .statement tag=0A82}

*设 G 为类 C^r (r ≥ 2) 的李群、X 流形 (r ≥ 2) 以及 G 的类 C^r 的左运算 (g, x) ↦ gx 律 X，从而，通过运输结构，TX 上 G 的左运算就有律。在这个律下，TX 是类 C^{r-1} 的向量 G 束。*

令 pr_1（分别为 pr_2）为 G × X 在 G（分别为 X）上的规范投影，并令 E_1（分别为 E_2）为 TG（分别为 TX）相对于 pr_1（分别为 pr_2）的逆像。那么向量丛 T(G × X) 就是E_1 和E_2 的直和。令 i: E_2 → T(G × X) 和 q: T(G × X) → E_2 为由此分解定义为直和的规范向量丛态射。设 φ 为 G × X 的映射 (g, x) ↦ (g, gx) 到 G × X。那么定义 4 中的 ψ 表示的映射（我们设 E = TX）就是 q ∘ T(φ) ∘ i。但 T(φ) 是类 C^{r-1} 的向量丛的 φ 态射（*可微且解析流形*，R，8.1.2）。

#### 推论{#lie-iii-s1-n8-cor-1 .statement tag=0A83}

*如果 τ 是类 C^r 的同构的向量函子，则 τ(TX) 是类 C^{r-1} 的向量 G 丛。*

这是从命题 15 和 16 得出的。

#### 注 1 {#lie-iii-s1-n8-rem-1 .statement tag=0A84}

如果 τ 是类 C^r 的同构 *in 有限维* 的向量函子，并且 E 是有限秩，则 τE 的定义类似，命题 15 仍然有效；如果 X 是有限维的，命题 16 的推论仍然有效。

#### 例 {#lie-iii-s1-n8-exa-1 .statement tag=0A85}

根据命题 16 的假设和记号，令F 为完全可范空间。那么$\mathscr{L}((TX)^p; F)$是类C^{r-1}的向量G丛；如果 K 为特征零或 X 为有限维（*可微且解析流形*, R, 7.7, 7.8），则 Alt^p(TX; F) 也是如此。如果X是有限维的，则$\bigotimes^p (TX) \otimes \bigotimes^q (TX)^*$是类C^{r-1}的向量G丛。

#### 命题 17 {#lie-iii-s1-prop-17 .statement tag=0A86}

*Let G be a Lie group, X a left Lie homogeneous space of G, x_0 a point of X, G_0 the stabilizer of x_0 in G, E and E' left vector G-bundles of class C^r and base space X, E_0 (resp. E'_0) the fibre of E (resp. E') at x_0 and f an element of $\mathscr{L}(E_0, E'_0)$ such that f(gu) = gf(u) for all u ∈ E_0 and g ∈ G_0. 那么存在且仅有一个 E 的态射到 E' 与 G 的运算兼容并扩展 f。*

这个态射的唯一性是显而易见的。我们证明它的存在。设 G 的 g、g' 元素和 u ∈ E_0 使得 gu = g'u。那么 g'^{-1}g ∈ G_0 且 g'^{-1}gu = u，因此 g'^{-1}gf(u) = f(u)，即 gf(u) = g'f(u)。因此，通过写 φ(gu) = gf(u) 将映射 φ 定义为 E 到 E'。显然，这个映射扩展 f 与 G 的运算兼容。我们证明 φ 是类 C^r 的向量丛态射。令x_1 ∈ X。在X中存在x_1的开邻域V和G的子流形W，使得映射g↦gx_0是类C^r的同构θ到V。通过缩小 V 和 W，可以假设：
(1) E | V（分别为 E' | V）与纤维 M（分别为 M'）的平凡向量丛相同；
(2) 如果 ψ_g (对应 ψ'_g) 将 E_0 (对应 E'_0) 的映射 u ↦ gu 表示为 E_{gx_0} (对应 E'_{gx_0})，则映射 g ↦ ψ_g 和 g ↦ ψ_g^{-1} (对应 g ↦) W 的 ψ'_g 和 g ↦ ψ'_g^{-1}) 转化为 $\mathscr{L}(E_0, M)$ 和 $\mathscr{L}(M, E_0)$（分别为 $\mathscr{L}(E'_0, M')$ 和 $\mathscr{L}(M', E'_0)$），其值为类 C^r。

对于 x ∈ V，令 φ_x : M → N 为 φ 到 E_x = M 的限制。然后通过组合以下映射获得 φ_x：
(1)将M的映射(ψ_θ^{-1,x})^{-1}代入E_0；
(2)将E_0的映射f转化为E_0；
(3) 将E_0的映射ψ'_θ^{-1,x}转化为M'。
因此我们看到，V到$\mathscr{L}(M, M')$的映射 x ↦ φ_x 是类 C^r。

#### 推论 1 {#lie-iii-s1-prop-17-cor-1 .statement tag=0A87}

令E_0^{G_0}为E_0的元素的集合，其在G_0下不变。对于所有 u ∈ E_0^{G_0}，令 σ_u 为 X 的映射，并由 σ_u(gx_0) = gu 定义，对于所有 g ∈ G。
(i) E 的 G 不变量截面† 为类 C^r。
(ii) u ↦ σ_u 是 E_0^{G_0} 的双射到 E 的 G 不变量截面的集合。

断言 (ii) 是显而易见的。为了证明 (i)，只需证明每个截面 σ_u 属于类 C^r。令 E' 为基 X 和纤维 E_0^{G_0} 的平凡 G 丛。令 f 为 E_0^{G_0} 到 E_0 的典范嵌入。到命题 17 时，存在 E' 的态射 φ 进入 E，与 G 的运算兼容并扩展 f。如果 u ∈ E_0^{G_0} 且 g ∈ G，则

$$
\sigma_u(gx_0) = gu = gf(u) = \varphi(gu) = \varphi((u, gx_0))
$$

因此对于所有 x ∈ X，有 σ_u(x) = φ((u, x))，这证明了我们的断言。

*对于例，设G是G的有限维实李群，G_0紧李子群和X齐次空间G/G_0。设 x_0 表示 X 中 e 的典范像。 G_0 下的 T_{x_0}(X) 不变量存在正定对称双线性形式（积分，章 VII, § 3，命题 1）。 应用上式到 (TX)* ⊗ (TX)*，我们看到X 上存在 G_* 下的解析黎曼度量不变量。

† 我们这里所说的 E 的截面是指 X 的映射 σ（不一定是类 C^r）到 E 中，使得 p ∘ σ = Id_X，其中 p 表示 E 的投影到 X 上。

#### 推论 2 {#lie-iii-s1-prop-17-cor-2 .statement tag=0A88}

假设 $G_0$ 对 $E_0$ 的运算很简单。令 $E'$ 为具有基空间 $X$ 和纤维 $E_0$ 的平凡 $G$ 束。在$E$到$E'$上存在且仅有一个同构与$G$的运算兼容并扩展$\mathrm{Id}_{E_0}$。

这紧接着命题 17。

#### 注 2 {#lie-iii-s1-n8-rem-2 .statement tag=0A89}

在这个数中，左运算的律可以全部替换为右运算的律。

### 9. 当地定义李群

#### 命题 18 {#lie-iii-s1-prop-18 .statement tag=0A8A}

令$G$为群、$U$和$V$$G$包含$e$中的两个子集。假设 $U$ 有一个解析式流形结构满足以下条件：
(i) $V = V^{-1}, V^2 \subset U, V$于$U$开放；
(ii) $V \times V$到$U$的映射$(x, y) \mapsto xy^{-1}$是解析的；
(iii) 对于所有$g \in G$，$V$中存在$e$的开邻域$V'$，使得$gV'g^{-1} \subset U$并且使得$V'$到$U$的映射$x \mapsto gxg^{-1}$是解析的。

那么$G$上存在且仅有一个解析流形结构，具有以下性质：
(α) $G$ 与此结构为李群；
(β)$V$于$G$开放；
(γ) $G$ 上的流形结构和$U$ 诱导与$V$ 上的结构相同。

(a) 设$A$为$V$的开子集和$V$的$v_0$元素，使得$v_0A \subset V$。那么$v_0A$是$v \in V$的集合，使得$v_0^{-1}v \in A$，因此是$V$的开子集（考虑(ii)）。此外，(ii) 意味着$A$到$v_0A$的映射$v \mapsto v_0v$和$v_0A$到$A$的$v \mapsto v_0^{-1}v$是逆解析双射，因此也是解析同构。

(b) 我们$V$中$e$的选择开邻域$W$，使得$W = W^{-1}$，$W^3 \subset V$，并且存在流形$U$的图表$(W, \phi, E)$，域为$W$。 For all $g \in G$, let $\phi_g$ be 映射 $h \mapsto \phi(g^{-1}h)$ of $gW$ into $E$.我们证明图表 $\phi_g$ 和 $G$ 是分析兼容的。令$g_1, g_2$为$G$的元素，使得$g_1W \cap g_2W \neq \emptyset$，使得$g_2^{-1}g_1$和$g_1^{-1}g_2$属于到$W^2$。根据 (a)，$W \cap g_1^{-1}g_2W$ 是 $W$ 的开子集，因此
$$
\phi_{g_1}(g_1W \cap g_2W) = \phi(W \cap g_1^{-1}g_2W)
$$
是 $E$ 的开子集 $D$。对于$d \in D$，
$$
(\phi_{g_2} \circ \phi_{g_1}^{-1})(d) = \phi(g_2^{-1}g_1\phi^{-1}(d));
$$
通过 (a) 我们看到 $\phi_{g_2} \circ \phi_{g_1}^{-1}$ 是解析的。

(c) By (b) there exists on $G$ an analytic 流形结构 such that $(\phi_g)_{g \in G}$ is an atlas on $G$.对于所有 $g_0 \in G$，映射 $g \mapsto g_0g$ ($g \in G$) 使该图集保持不变，因此是 $G$ 的自同构与此流形结构。特别是满足条件(GL₁)。

(d)设$v_0 \in V$。通过(ii)，在$W$中存在$e$的开邻域$A$使得$v_0A \subset V$。这首先证明$V$在$G$开。由(a) $A$到$v_0A$的映射$v \mapsto v_0v$是由U诱导的解析同构和结构。由(c)我们看到G和U诱导上的流形结构相同结构在 v_0A 上，因此最终在 V 上。

(e) by (d), (ii) and (iii), we see that 条件 (GL_2) and (GL_3) hold.因此G是李群。

(f) 如果 G 上的流形结构与 G 的群结构兼容，且V 是 G 的开子流形，则 (\phi_g)_{g\in G} 是 G 上的图集。因此命题的唯一性断言。

#### 命题 19 {#lie-iii-s1-prop-19 .statement tag=0A8B}

设G是群、H李群和群G的f同态到群H。假设G中存在e_G的开邻域、e_H处流形H的图(V,\phi,E)和闭图E 的向量子空间 F 承认拓扑补充，使得 f(U) \子集 V 和 \phi \circ f)|U 是 U 到 \phi(V) \cap F 的同胚。那么存在唯一的流形结构在 G 上，使得 f 是浸没； this 结构 is 逆像 under f of 流形结构 on H. With this 结构 G is 李群.

由于 G（或 H）的翻译是同态（或解析同构），f 满足可微分和解析流形，R，5.8.1 的条件 (R)。 The first two 断言 of 命题 then follow from Differentiable and Analytic 流形, R, loc.引用。考虑交换律图表

$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
f \times f \downarrow & & \downarrow f \\
H \times H & \xrightarrow{n} & H
\end{array}
$$

其中 m(x, y) = xy^{-1} （分别为 n(x, y) = xy^{-1}），对于 G 中的 x、y（分别为 H）。那么 n \circ (f \times f) 是解析的，因此 f \circ m 是解析的，因此 m 是解析的，因为 f 是浸没。因此G是李群。

李群结构 on G is called 逆像 of 李群结构 on H under f.

#### 推论 {#lie-iii-s1-n9-cor-1 .statement tag=0A8C}

Let G be a topological 群, N a discrete normal 子群 of G and \pi 典范映射 of G onto G/N. Suppose that an analytic 流形结构 is given on G/N, compatible with the topological 群结构 on G/N. Then there exists a unique 流形结构 on G such that \pi is an immersion; this 结构 is 逆像 under \pi of 流形结构 on G/N. With this 结构, \pi is étale, G is 李群 and G/N is the quotient 李群 of G by N.

#### 注 {#lie-iii-s1-n9-rem-1 .statement tag=0A8D}

设 H 为连通实数或复数李群，\tilde{H} 是其通用覆盖†，而 \pi 典范映射是 \tilde{H} 到 H 上的。当我们谈到 \tilde{H} 时

† 参见。一般拓扑、章XI； whilst awaiting the publication of this 章, see for 例 L. S. Pontrjagin, Topological 群, 2nd edition translated from Russian, Gordon and Breach, 1966; or G. Hochschild, 结构 of 李群, Holden-Day, 1965.

李群

as 李群, we shall always mean with 逆像结构 of that on H under $\pi$.

### 10. 群细菌

#### 定义 5 {#lie-iii-s1-def-5 .statement tag=0A8E}

*K* 上的李群胚芽为系统$(G, e, \theta, m)$满足以下条件：
(i) $G$ 是$K$ 上的解析流形；
(ii) $e \in G$；
(iii) $\theta$ 是 $G$ 到 $G$ 的解析映射；
(iv) $m$ 是$G \times G$ 的开子集 $\Omega$ 到$G$ 的解析映射；
(v) 对于所有$g \in G$、$(e, g) \in \Omega$、$(g, e) \in \Omega$、$m(e, g) = m(g, e) = g$；
(vi) 对于所有$g \in G$、$(g, \theta(g)) \in \Omega$、$(\theta(g), g) \in \Omega$、$m(g, \theta(g)) = m(\theta(g), g) = e$；
(vii) 如果$g, h, k$是$G$的元素使得$(g, h) \in \Omega$、$(h, k) \in \Omega$、$(m(g, h), k) \in \Omega$、$(g, m(h, k)) \in \Omega$，则$m(m(g, h), k) = m(g, m(h, k))$。

$e$称为群胚芽的单位元素。我们经常写$gh$而不是$m(g, h)$，并且（通过滥用记号）$g^{-1}$而不是$\theta(g)$。

李群$G$是李群胚芽，与$e, \theta, m$明显的选择。

设$G$为李群胚芽。那么$ee^{-1} = e$，即

$$
e^{-1} = e.
$$

对于所有$g \in G$，

$$
g = eg = ((g^{-1})^{-1}g^{-1})g = (g^{-1})^{-1}(g^{-1}g) = (g^{-1})^{-1}e,
$$

那就是

$$
(g^{-1})^{-1} = g.
$$

$G$在映射$g \mapsto g^{-1}$下不变的子集称为对称。

流形$G$，与点$e$、映射$g \mapsto g^{-1}$和映射$(g, h) \mapsto hg$是李群胚芽$G^\vee$称为$G$的相反。

李群胚芽$G$被称为可交换的，如果对于所有$(g, h) \in G \times G$使得$gh$被定义，$hg$被定义并且等于$gh$。

设$G$为李群胚芽。 $(g, h) \in G \times G$的集合使得$gh$被定义为$(e, e)$的邻域。另一方面，映射$(g, h) \mapsto gh$和$g \mapsto g^{-1}$是连续的。因此，$g, h, k$ 的$(gh)k = g(hk)$ 足够接近$e$。类似地，$(h^{-1}g^{-1})(gh) = h^{-1}(eh) = h^{-1}h = e$对于$g, h$足够接近$e$，从而在右侧乘以$(gh)^{-1}$，

$$
(gh)^{-1} = h^{-1}g^{-1} \quad \text{for } g, h \text{ sufficiently close to } e.
$$

#### 命题 20 {#lie-iii-s1-prop-20 .statement tag=0A8F}

*令$G$为李群胚芽和$g \in G$。存在 $e$ 的开邻域 $U$ 和 $g$ 的开邻域 $V$，具有以下属性：*
(a) $ug$ 是为所有$u \in U$ 定义的；
(b) $vg^{-1}$是为所有$v \in V$定义的；
(c) 映射 $u \mapsto ug,\ v \mapsto vg^{-1}$ 是$U$ 的一个另一个到$V$ 以及$V$ 到$U$ 的逆解析同构。

§ 1.10

由于乘积的定义的集合在$G \times G$开路，因此存在$e$的开路邻域$U$和$g$的开路邻域$V$，其性质为(a)和(b)。让$\eta(u) = ug$代表$u \in U$，$\eta'(v) = vg^{-1}$代表$v \in V$。通过缩小$U$和$V$，可以假设$(ug)g^{-1} = u$和$(vg^{-1})g = v$对应于$u \in U$和$v \in V$。那么$\eta$和$\eta'$就是单射。通过进一步缩小$U$，可以假设$\eta(U) \subset V$。那么$\eta'(V) \supset U$和$\eta(U)$是$\eta'$下$U$的逆像，因此是$V$中$g$的开邻域。 替换$V$到$\eta(U)$，我们最终到达$\eta$和$\eta'$解析逆双射的情况。

令$G_1, G_2$为两个李群细菌和单位元素$e_1, e_2$。如果$f$满足以下条件，则$G_1$到$G_2$的映射$f$称为*态射*：
(i) $f$ 是解析的；
(ii) $f(e_1) = e_2$；
(iii) 如果$g, h$是$G_1$的元素，使得$gh$被定义，则$f(g)f(h)$被定义并且等于$f(gh)$。

让$g \in G_1$。由于$gg^{-1}$已定义且等于$e_1$，因此$f(g)f(g^{-1})$已定义且等于$e_2$，因此
$$
f(g)^{-1} = f(g)^{-1}(f(g)f(g^{-1})) = (f(g)^{-1}f(g))f(g^{-1})
$$
那就是
$$
f(g)^{-1} = f(g^{-1}).
$$
(11)

两个态射的合成是态射。

如果$f : G_1 \to G_2$和$f' : G_2 \to G_1$是一个另一个的两个逆态射，则它们是同构（特别使用公式（11））。

设$G_1, G_2$为两个李群细菌，将$G_1$的$f$映射化为$G_2$满足条件(ii)和(iii)，这是在开放的邻域中解析$e_1$。使用命题 20，可以如命题 4 那样证明$f$ 是态射。

设$(G, e, \theta, m)$为李群胚芽，$m$的定义为$\Omega$集合。令$H$为$G$包含$e$的子流形，在$\theta$下稳定。假设$(x, y) \in \Omega \cap (H \times H)$的集合$\Omega_1$使得$m(x, y) \in H$在$H \times H$开。那么$(H, e, \theta|H, m|\Omega_1)$就是李群胚芽。这样的李群胚芽被称为G*的*谎言子群胚芽。 $H$到$G$的典范嵌入是态射。如果$f : L \to G$是李群病菌中的态射使得$f(L) \subset H$，则$f : L \to H$是李群病菌中的态射。

假设$K$的特征为0。如果我们替换假设$H$是$G$的子流形假设$H$是$G$的准子流形，则上段的结果仍然为真（cf. *可微分和解析流形*，R，5.8.5）。 $H$ 则称为 $G$ 的李准子群胚芽。

如果$G$是李群胚芽和单位元素$e$，则$G$中$e$的每个对称开邻域都是$G$的李子群胚芽。 （这尤其适用于当$G$为李群时。）令$H$为$G$的谎言子群胚芽；如果$G$中$H$是$e$的邻域，则$H$在$G$中开命题20。

有限数李群胚芽的 *乘积* 李群胚芽以明显的方式定义。

#### 命题 21 {#lie-iii-s1-prop-21 .statement tag=0A8G}

*令$G, H$为两个李群细菌，并将$G$的$\phi$态射放入$H$。以下条件是等效的：*

(i) $\phi$ 的长度为 $e$；
(ii) *存在开放谎言子群细菌*$G', H'$*的*$G, H$*使得*$\phi|G'$*是同构的*$G'$*到*$H'$。

含义 (ii) $\Rightarrow$ (i) 是显而易见的。假设 $\phi$ 的 étale 为 $e$。存在$G$的开谎言子群胚芽$G_1$，使得$\phi(G_1)$在$H$中开，并且$\phi|G_1$是流形$G_1$的同构到流形$\phi(G_1)$。则存在$G_1$的开谎言子群胚芽$G'$，使得$G'$的两个元素中的$G$中的乘积总是被定义，且属于至$G_1$。如果$g, g'$是$G'$的元素使得$gg' \in G'$，则$\phi(g)\phi(g') = \phi(gg') \in \phi(G')$；如果$g, g'$是$G'$的元素使得$gg' \in G_1 - G'$，那么

$$
\phi(g)\phi(g') = \phi(gg') \in \phi(G_1) - \phi(G').
$$

因此，$\phi|G'$是李群胚芽$G'$的同构到$H$的开谎言子群胚芽$\phi(G')$上。

如果命题 21 的条件成立，则 $G$ 和 $H$ 被称为“局部同构”。

#### 命题 22 {#lie-iii-s1-prop-22 .statement tag=0A8H}

*设$H$为李群，$U$是$H$的谎言子群胚芽，以及$g \in H$的$N$集合，使得$U$和$gUg^{-1}$在$e$处具有相同的胚芽（一般拓扑、章I, § 6, no. 10）。那么$N$就是$H$包含于$U$的子群。 $N$ 上存在且仅有一个解析流形结构，具有以下属性：*

(i) $N$ 与此结构是李群；
(ii) $U$ 是 $N$ 的开子流形；
(iii)*典范嵌入*$N$*进入*$H$*是一种沉浸*。

显然 $N$ 是 $H$ 的子群。如果$g \in U$，则$ge \in U$和$geg^{-1} \in U$，因此$u$的$gu \in U$和$gug^{-1} \in U$足够接近$U$中的$e$，因此$gUg^{-1}$在$e$的萌芽包含在$U$；交换$g$和$g^{-1}$，我们发现$gUg^{-1}$和$U$在$e$的细菌是相等的。因此$U \subset N$。

令$V$为$e$在$U$中的开邻域，使得$V = V^{-1}, V^2 \subset U$。满足no. 9中的命题18个条件(i)、(ii)、(iii)(其中$G$替换为$N$)。因此，$N$上存在解析流形结构，具有以下性质：($\alpha$)$N$，其中结构是李群； ($\beta$)$V$于$N$开放； ($\gamma$)$N$上的流形结构和$U$诱导与$V$上的结构相同。由于$V$是$H$的子流形，$N$到$H$的典范嵌入是在$e$处的浸没，因此在$N$的每个点处。让$u \in U$。在V中存在e的开邻域V'，使得映射$v \mapsto uv$是V'的解析同构到U中的开邻域（命题20），同时又到u 在 N 上开邻域。因此 U 在 N 上开，U 的恒等映射是同构，且 U 上给定流形结构且 N 上开子流形结构；在其他字中，U是N的开子流形。

最后，我们考虑 N 上的解析流形结构，其属性 (i) 和 (ii) 为命题，并令 N* 为由此获得的李群。那么 N* 的恒等映射是 e 处的 étale，因此李群同构。这就证明了命题的唯一性断言。

设H为李群，U是H的李准子群胚芽和$g \in H$的N集合，使得U和$gUg^{-1}$在e处具有相同的胚芽。如果 K 的特征为 0，则 G 上存在且仅有一个流形结构，其属性 (i) 和 (ii) 为命题 22。 证明与命题 22 相同。

#### 推论{#lie-iii-s1-n10-cor-1 .statement tag=0A8I}

保留命题 22 的记号，令G 为U 生成的H 的子群。则G 是N 的开子群。G 上存在且仅有一个李群结构，使得U 是G 的开子流形，且G 的典范嵌入到H 中是浸没。

#### 注 {#lie-iii-s1-n10-rem-1 .statement tag=0A8J}

保留命题 22 的记号及其推论，假设 K 的特征为 0，H 是有限维的，U 上的拓扑允许可数的基。即使有所有这些假设，G 也可能在 H (习题 3) 中不闭合。但是，如果 G 是闭集，G 是 H 的谎言子群。因为映射 $(g, h) \mapsto gh$ 是 G 在 H 上的解析左运算的律。e 的轨道是 G。然后我们的断言由命题 2 (iv) 和 14 (iii) 得出。

### 11. 律运算块

设$(G, e, \theta, m)$为李群胚芽，X流形为类$C^r$。

#### 定义 6 {#lie-iii-s1-def-6 .statement tag=0A8K}

A law chunk of left operation of class $C^r$ of G on X is a mapping $\psi$ defined on an open subset $\Omega$ of $G \times X$ containing $\{e\} \times X$, with values in X and with the following properties:
(i) $\psi$ is of class $C^r$;
(ii) for all $x \in X$, $\psi(e, x) = x$;
(iii) there exists a neighbourhood $\Omega_1$ of $\{e\} \times \{e\} \times X$ in $G \times G \times X$ such that, for $(g, g', x) \in \Omega_1$, the elements of $m(g, g')$, $\psi(m(g, g'), x)$, $\psi(g, \psi(g', x))$ are defined and $\psi(g, \psi(g', x)) = \psi(m(g, g'), x)$.

类$C^r$右运算的律块的定义类似。
我们经常写$gx$而不是$\psi(g, x)$。
设 G' 是 G 的李子群胚芽，X' 是 X 的子流形。假设$(g, x) \in \Omega \cap (G' \times X')$的集合$\Omega'$使得$\psi(g, x) \in X'$在$G' \times X'$中开放（如果$X'$在$X$中开放则总是满足条件）。那么$\psi|_{\Omega'}$是$X'$上$G'$的类$C^r$的左运算的律块，据说是从$\psi$通过限制衍生到$G'$并且$X'$。

#### 命题 23 {#lie-iii-s1-prop-23 .statement tag=0A8L}

*设$(G, e, \theta, m)$为李群胚芽，类$C^r$$X$流形，$X$$x_0$点，$\Omega$$(e, x_0)$开邻域将$\Omega$的$G \times X$和$\psi$映射转化为$X$，具有以下属性：
(i) $\psi$ 为类 $C^r$；
(ii) $\psi(e, x)$ 等于 $x$，因为 $x$ 足够接近 $x_0$；
(iii) $\psi(m(g, g'), x) = \psi(g, \psi(g', x))$ 对于 $(g, g', x)$ 足够接近 $(e, e, x_0)$。
那么$X$中存在$x_0$的开邻域$X'$和$\Omega \cap (G \times X')$的开子集$\Omega'$，使得$\psi|_{\Omega'}$是类的左侧运算的律块$X'$ $G$ 的$C^r$。
在$X$中存在$x_0$的开邻域$X'$，在$G$中存在$e$的开邻域$G'$，使得$\psi(e, x) = x$对于所有$x \in X$，并且
$$
\psi(g, \psi(g', x)) = \psi(m(g, g'), x)
$$
$(g, g', x) \in G' \times G' \times X'$。令$\Omega'$为$(g, x) \in \Omega \cap (G' \times X')$的集合，使得$\psi(g, x) \in X'$。那么$\Omega'$在$G \times X'$和$X'$中开，$\Omega'$具有命题的属性。*

#### 引理 3 {#lie-iii-s1-lem-3 .statement tag=0A8M}

*设 $X$ 为正常的空间，$(X_i)_{i \in I}$ 为 $X$ 的局部有限开覆盖​​。对于所有$(i, j) \in I \times I$和所有$x \in X_i \cap X_j$，令$V_{ij}(x)$为$X_i \cap X_j$中包含的$x$的邻域。然后我们可以关联$x$的每个$x \in X$邻域$V(x)$，从而满足以下条件：
(a) 关系 $x \in X_i \cap X_j$ 意味着 $V(x) \subset V_{ij}(x)$；
(b) 如果$V(x)$和$V(y)$相遇，则存在$i \in I$使得$V(x) \cup V(y) \subset X_i$。
存在$X$的开放覆盖$(X'_i)_{i \in I}$，使得$\overline{X'_i} \subset X_i$适用于所有$i \in I$（一般拓扑、章IX, § 4、定理3）。让$x \in X$。设$V_1(x)$为$V_{ij}(x)$和$X'_k$中的交，其中包含$x$；这是 $x$ 的开邻域。令$V_2(x)$为包含在$V_1(x)$中的$x$的邻域，且仅满足$X_i$的有限数。那么$V_2(x)$仅满足$\overline{X'_i}$的有限数，因此集合
$$
V(x) = V_2(x) \cap \bigcap_{i \in I, x \notin \overline{X'_i}} (X - \overline{X'_i})
$$
是 $x$ 中的邻域。如果$x \in X_i \cap X_j$，则$V_1(x) \subset X_i \cap X_j$，因此$V(x) \subset X_i \cap X_j$。令$x, y$在$X$中，并假设$V(x)$和$V(y)$相交。存在$i \in I$使得$x \in X'_i$。然后$V_1(x) \subset X'_i$，因此$V(x) \subset X'_i$，因此$V(y) \cap \overline{X'_i} \neq \emptyset$。然后是$y \in \overline{X'_i}$乘定义，共$V(y)$、从而$y \in X_i$和$V(y) \subset X_i$。因此$X_i$包含于$V(x)$和$V(y)$。*

§ 2.1

#### 命题 24 {#lie-iii-s1-prop-24 .statement tag=0A8N}

令 G 为李群胚芽、类C^r 的X流形以及 (X_i)_{i \in I} X的局部有限开覆盖。对于I中的所有i，令$\psi_i$为X_i上G的类C^r的左运算的律块。假设 X 的基础拓扑空间是正规的，并且对于所有 (i, j) \in I \times I 和所有 x \in X_i \cap X_j，$\psi_i$ 和 $\psi_j$ 重合在邻域上（e，x）。在X上存在G的类C^r的左运算的律块$\psi$，使得对于所有i \in I和所有x \in X_i，$\psi_i$和$\psi$ 重合在 (e, x) 的邻域上。

对于所有 (i, j) \in I \times I 和所有 x \in X_i \cap X_j, 选择 X_i \cap X_j 中 x 的开邻域 V_{ij}(x)，使得 $\psi_i$ 和 $\psi_j$ 在邻域上定义且相等{e} \times V_{ij}(x) in G \times X。对于X选择中的所有x \，X中x的开邻域V(x)，使得满足引理3的条件(a)和(b)。令 I_x 为 i \in I 的集合，使得 x \in X_i。这是一个有限的集合。令 U_x 为 (g, y) \in G \times V(x) 的集合，从而定义 I_x 中 i \的 $\psi_i$，并定义 (g, y) 的邻域上的重合。那么U_x 是开的并且(e, x) \in U_x。 I_x 中 i \的 $\psi_i$ 对于 U_x 都有相同的限制。设 x, y 在 X 内。如果 U_x 和 U_y 相遇，V(x) 和 V(y) 相遇，因此存在 i \in I 使得

$$
V(x) \cup V(y) \subset X_i.
$$

然后 i \in I_x, i \in I_y, $\psi_i|U_x = \psi_x, \psi_i|U_y = \psi_y$ 因此

$$
\psi_x|(U_x \cap U_y) = \psi_y|(U_x \cap U_y).
$$

因此，$U = \bigcup_{x \in X} U_x$的$\psi_x$定义映射$\psi$进入X，并且U是G\timesX中的{e}\timesX的开邻域。显然，对于 X 中的所有 x \，$\psi$ 是类 C^r 和 $\psi(e, x) = x$。对于所有 i \in I 和所有 x \in X_i，$\psi$ 重合与 $\psi_x$，因此 $\psi_i$ 在 (e, x) 的邻域中，因此 $\psi$ 满足定义的条件 (iii) 6.

### 习题 {#lie-iii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
