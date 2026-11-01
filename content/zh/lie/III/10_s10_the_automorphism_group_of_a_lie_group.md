---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 10
section_title: The automorphism group of a Lie group
lang: zh
source: lie-i-iii
book_pages: 359-368
pdf_pages: 0377-0386, 0427-0427
extraction: ocr
subsections:
    - "no": 1
      title: INFINITESIMAL AUTOMORPHISMS
      page: 359
      pdf_page: 377
    - "no": 2
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (REAL OR COMPLEX CASE)
      page: 362
      pdf_page: 380
    - "no": 3
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (ULTRAMETRIC CASE)
      page: 367
      pdf_page: 385
statements: 13
exercises: 4
content_sha256: 7b81d04590a9b6c50c12a1e5e4d9a2d2ea6d52879d03103ac064945f42ea8495
translated_from: content/en/lie/III/10_s10_the_automorphism_group_of_a_lie_group.md
translation_method: google
source_content_sha256: f9d7400def142eff7395a68ad471a8fd0e9e5f47e8dd9c61b495ed3c4a325f89
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: aaed4cde8102cea70495ae3e102877e3a199644f042d6bbf779323265617f482
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 10。 李群的自同构群

在本段中，K 假设为特征零。

### 1. 无穷小自同构

#### 引理 1 {#lie-iii-s10-lem-1 .statement tag=0AL6}

设 G 为 G 上的李群和 $\alpha$ 向量域。对于所有 $g \in G$，让
$$
\beta(g) = \alpha(g)g^{-1} \in L(G).
$$
以下条件是等效的：
(i) $\alpha$ 是群 G 中的同态变成群 T(G)；
(ii) 对于 G 中的所有 $g, g'$，$\alpha(gg') = \alpha(g)g' + g\alpha(g')$；
(iii) 对于 G 中的所有 $g, g'$，$\beta(gg_1) = \beta(g) + (\mathrm{Ad}\,g)\beta(g')$。

条件 (i) 意味着，对于 G 中的所有 $g, g'$，我们在群 T(G) 中有：
$$
\beta(g)g\beta(g')g' = \beta(gg')gg'
$$
或
$$
\beta(g)((\mathrm{Ad}\,g)\beta(g'))gg' = \beta(gg')gg'.
$$
但T(G)中$\beta(g)$和$(\mathrm{Ad}\,g)\beta(g')$的乘积只是$L(G)$中$\beta(g)$和$(\mathrm{Ad}\,g)\beta(g')$的和（§ 2, no. 1，命题2）。因此 (i) $\Leftrightarrow$ (iii)。另一方面，条件 (ii) 可以写成$\beta(gg')gg' = \beta(g)gg' + g\beta(g')g'$，或者
$$
\beta(gg') = \beta(g) + (\mathrm{Ad}\,g)\beta(g')
$$
因此 (ii) $\Leftrightarrow$ (iii)。

#### 定义 1 {#lie-iii-s10-def-1 .statement tag=0AL7}

令 G 为李群。 G 的无穷小自同构是引理 1 的 G 满足条件上的任意解析向量域。

#### 引理 2 {#lie-iii-s10-lem-2 .statement tag=0AL8}

令$K'$为K、A、$K'$流形、B和C$K$流形的非离散闭子域，以及$f$$A \times B$的$K'$解析映射为C。假设对于所有

李群

$a \in A$，*映射*$b \mapsto f(a, b)$*的*B*到*C*是*K-*解析*。 *然后，对于* TB *到* TC *的所有* $t \in TA$，*映射* $u \mapsto (Tf)(t, u)$ *是*K-*解析*。

我们固定$t \in TA$并写入$g(u) = (Tf)(t, u)$。显然 $g$ 是 K' 解析的。通过*可微解析流形*，R，5.14.6，足以证明映射到$g$的切线是K线性的。可以假设 A、B、C 在 K'、K、K 上的完全可范空间 E、F、G 中是 0 的开邻域，并且$t$ 在 0 处与 A 相切。我们认同 TA、TB、TC，其中 $A \times E, B \times F, C \times G$ 和$t$ 与 E 的元素。然后对于所有 $(x, y) \in TB = B \times F$。

$$
g(x, y) = (f(0, x), (D_1f)(0, x)(t) + (D_2f)(0, x)(y)).
$$

我们认同$T(B \times F)$与$(B \times F) \times (F \times F)$，$T(C \times G)$与$(C \times G) \times (G \times G)$。那么，对于所有

$$
((x, y), (h, k)) \in T(B \times F) = (B \times F) \times (F \times F),
$$

$(Tg)((x, y), (h, k)) = ((a, b), (c, d))$，哪里

$$
\begin{align*}
a &= f(0, x), \\
b &= (D_1f)(0, x)(t) + (D_2f)(0, x)(y), \quad c = (D_2f)(0, x)(h), \\
d &= (D_2D_1f)(0, x)(t, h) + (D_2D_2f)(0, x)(y, h) + (D_2f)(0, x)(k).
\end{align*}
$$

我们现在修复$(x, y) \in B \times F$。我们需要证明$F \times F$到$G \times G$的映射$(h, k) \mapsto (c, d)$是K线性的。由于 B 到 C 的映射 $x \mapsto f(0, x)$ 是 K 解析的，映射

$$
(h, k) \mapsto (D_2f)(0, x)(h), \quad (h, k) \mapsto (D_2D_2f)(0, x)(y, h),
$$
$$(h, k) \mapsto (D_2f)(0, x)(k)$$

是 K 线性的。另一方面

$$
(D_2D_1f)(0, x)(t, h) = \lim_{\lambda \in K', \lambda \to 0} \lambda^{-1}((D_2f)(\lambda t, x)(h) - (D_2f)(0, x)(h))
$$

并且，对于固定的$\lambda$，映射$x \mapsto f(\lambda t, x)$是K-解析的，因此映射$h \mapsto (D_2f)(\lambda t, x)(h)$是K-线性的。

#### 命题 1 {#lie-iii-s10-prop-1 .statement tag=0AL9}

*设* K' *为非离散闭子域 of* K, G *李群 over* K, V *流形 over* K' *和* $(v, g) \mapsto vg$ *a* K'-*解析映射 of* V $\times$ G *入* G. *假设，对于所有* $v \in V$，*映射* $g \mapsto vg$ *属于* G *进入* G *是* G 的自同构。*让* $\varepsilon$ *成为* V *的元素 *使得* $\varepsilon g = g$ *对于所有* $g \in G$ *和* $a \in T_\varepsilon(V)$。 *那么*G上的向量域*$g \mapsto ag$*是*G的无穷小自同构。

对于$v \in V,\ g_1 \in G,\ g_2 \in G,\ v(g_1g_2) = (vg_1)(vg_2)$。因此，对于 $u_1 \in TG,\ u_2 \in TG,\ a(u_1u_2) = (au_1)(au_2)$ (§ 2, no. 1, 命题 3)。特别地，G到TG中的映射$g \mapsto ag$是群同态。另一方面，这个映射是由引理2解析的。

#### 命题 2 {#lie-iii-s10-prop-2 .statement tag=0ALA}

*设* G *为实数或复数李群且*$\alpha$*G的无穷小自同构。G上存在K的解析运算$(\lambda, g) \mapsto \phi_\lambda(g)$的律，具有以下性质：
(1) 如果 D 是无穷小运算的关联律，则$D(1) = \alpha$；
(2) 对于所有$\lambda \in K$、$\phi_\lambda \in \mathrm{Aut}\, G$。
(a) 对于所有$\mu > 0$，令$K_\mu$为K中中心 0、半径为$\mu$的开球。对于所有$g \in G$，令$\mathscr{F}_g$为在球中定义的$\alpha$的解析积分曲线$f$的集合 $K_\mu$ 以及$f(0) = g$。通过可微分和解析流形，R，9.1.3和9.1.5，$\mathscr{F}_g$非空，并且$\mathscr{F}_g$重合中的两个元素位于定义的域的交上；令$\mu(g)$为数$\mu$中最小的上界，使得在$K_\mu$中定义存在$\mathscr{F}_g$的元素；存在$K_{\mu(g)}$中定义的$\mathscr{F}_g$的唯一元素；我们用$f_g$表示。
(b) 设$g_1, g_2$在G中，$f_1 \in \mathscr{F}_{g_1}, f_2 \in \mathscr{F}_{g_2}$且$f_1$和$f_2$定义在同一个球$K_\mu$上。那么$f_1 f_2 : K_\mu \to G$是解析的，$(f_1 f_2)(0) = g_1 g_2$。另一方面，对于所有 $\lambda \in K_\mu$，

$$
(T_\lambda(f_1 f_2))1 = (T_\lambda f_1)1 \cdot f_2(\lambda) + f_1(\lambda) \cdot (T_\lambda f_2)1 \quad (\S\ 2,\ \text{Proposition 7})
$$
$$
= \alpha(f_1(\lambda)) f_2(\lambda) + f_1(\lambda) \alpha(f_2(\lambda))
$$
$$
= \alpha((f_1 f_2)(\lambda)) \tag{\text{Lemma 1}}
$$

因此$f_1 f_2 \in \mathscr{F}_{g_1 g_2}$。这就证明了$\mu(g_1 g_2) \geq \inf_{g \in V} (\mu(g_1), \mu(g_2))$。
(c) 根据可微分和解析流形，R，9.1.4和9.1.5，G中存在e的邻域V使得$\sigma = \inf_{g \in V} \mu(g) > 0$。令 $h \in G$ 和 C 为其连通分量。对于 (b) 中的所有 $h' \in C$、$\mu(h') \geq \inf(\sigma, \mu(h)) > 0$。另一方面，函数$f_{h'}$，其中$h' \in C$，在C中取其值。通过可微分和解析流形，R，9.1.4和9.1.5，C中的$\mu = +\infty$，最后G中的$\mu = +\infty$。然后让$f_g(\lambda) = \phi_\lambda(g)$代表所有$g \in G$和所有$\lambda \in K$。由可微分解析流形，R，9.1.4和9.1.5，映射$(\lambda, g) \mapsto \phi_\lambda(g)$是G上K的解析运算的律。显然，如果D是无穷小运算的关联律， $D(1) = \alpha$。由(b)，

$$
\phi_\lambda(g_1 g_2) = \phi_\lambda(g_1) \phi_\lambda(g_2)
$$

对于所有$\lambda \in K, g_1 \in G, g_1 \in G$。

#### 命题 3 {#lie-iii-s10-prop-3 .statement tag=0ALB}

假设 K 是超度量的。 令 G 为紧李群且 $\alpha$ G 的无穷小自同构。 There exist an open subgroup I of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I on G with the following properties:
(1) if D is the associated law of infinitesimal operation, then $D(1) = \alpha$;
(2) for all $\lambda \in I, \phi_\lambda \in \mathrm{Aut}\, G$.
As G is compact, there exist an open subgroup I' of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I' on G with property (1) of the proposition (§ 4, no. 7, Corollary 2 to Theorem 6). 我们将$\lambda \in I'$和$g \in G$写为$\phi_\lambda(g) = f_g(\lambda)$。 然后，对于$G$和$\lambda \in I'$中的$g_1, g_2$，

$$
(T_\lambda(f_{g_1}f_{g_2}))1 = (T_\lambda f_{g_1})1 \cdot f_{g_2}(\lambda) + f_{g_1}(\lambda) \cdot (T_\lambda f_{g_2})1 \\
= \alpha(f_{g_1}(\lambda)) f_{g_2}(\lambda) + f_{g_1}(\lambda) \alpha(f_{g_2}(\lambda)) \\
= \alpha(f_{g_1}(\lambda) f_{g_2}(\lambda))
$$

和$(f_{g_1}f_{g_2})(0) = g_1 g_2 = f_{g_1g_2}(0)$。因此$f_{g_1'g_2'}(\lambda) = f_{g_1'}(\lambda) f_{g_2'}(\lambda)$代表$(g_1', g_2', \lambda)$

在 $(g_1, g_2, 0)$ 的邻域中（可微分和解析流形，R，9.1.8）。由于$G$是紧的，因此存在$I'$的开子群$I$，使得$f_{g_1g_2}(\lambda) = f_{g_1}(\lambda) f_{g_2}(\lambda)$对于所有$g_1 \in G, g_2 \in G, \lambda \in I$。在其他字，$\phi_\lambda \in \mathrm{Aut}\, G$为$\lambda \in I$。

#### 引理 3 {#lie-iii-s10-lem-3 .statement tag=0ALC}

令$G$和$G'$分别为$G$的李群和$\phi$同态到$\mathrm{Aut}(G')$。让 $f(g, g') = (\phi(g))(g')$ 代表 $g \in G, g' \in G'$。考虑以下条件：
(i) $f$ 是解析的；
(ii) $f$解析于$(e_G, e_{G'})$的邻域；
(iii) 对于所有 $g' \in G'$，映射 $g \mapsto f(g, g')$ 是解析的。
然后 (i) $\Leftrightarrow$ ((ii) 和 (iii))。如果 $G$ 连接，则 (i) $\Leftrightarrow$ (ii)。
显然 (i) 意味着 (ii) 和 (iii)。让$g_0 \in G, g_0' \in G'$。对于所有$g \in G, g' \in G'$，

$$
f(gg_0, g'g_0') = (\phi(g)\phi(g_0))(g'g_0') = \phi(g)(\phi(g_0)g').\phi(g)(\phi(g_0)g_0').
$$

这就证明了蕴涵((ii)和(iii))$\Rightarrow$(i)。最后，如果$G'$是连接的，则$G'$由$e_{G'}$的每个邻域生成，因此(ii)$\Rightarrow$(iii)。

### 2. 李群的自同构群（真实或复杂的情况）

在这个数中，我们假设$K = \mathbf{R}$或$\mathbf{C}$。

#### 引理 4 {#lie-iii-s10-lem-4 .statement tag=0ALD}

令 $H$ 为有限维单连通李群。
(i) 对于所有$u \in \mathrm{Aut}\, L(H)$，令$\theta(u)$ 为$H$ 中唯一的自同构，使得$L(\theta(u)) = u$。那么$(\mathrm{Aut}\, L(H)) \times H$到$H$的映射$(u, g) \mapsto \theta(u)g$解析。
(ii) 令$N$为$H$的谎言子群和$\mathrm{Aut}(H, N)$集合为$v \in \mathrm{Aut}\, H$，使得$v(N) = N$。那么$0^{-1}(\mathrm{Aut}(H, N))$是$\mathrm{Aut}\, L(H)$的谎言子群。
(iii) 假设$N$是离散且正规的，则$G = H/N$的李代数可与$L(H)$识别。对于所有$w \in \mathrm{Aut}\, G$，让$\eta(w)$是$H$的唯一自同构，这样$L(\eta(w)) = L(w)$。那么映射$\eta$就是群$\mathrm{Aut}\, G$的同构到群$\mathrm{Aut}(H, N)$。
为了证明(i)，只要通过no. 1的引理3，验证映射$(u, g) \mapsto \theta(u)g$在$(\mathrm{Id}_{L(H)}, e)$的邻域解析即可。在$L(H)$中存在0的开邻域B，使得$\psi = \exp_H|B$是B到H中e的开邻域的解析同构。在Aut$L(H)$中存在$\mathrm{Id}_{L(H)}$的开邻域U和$L(H)$ 中的邻域 $B'$ 为 0，使得 $U(B') \subset B$。那么$U \times \psi(B')$到H中的映射$(u, g) \mapsto \theta(u)g$由以下映射组成：

将$U \times \psi(B')$中的映射$(u, g) \mapsto (u, \psi^{-1}(g))$变为$U \times B'$；
将$U \times B'$中的映射$(u, x) \mapsto u(x)$转换为$B$；
将 $B$ 的映射 $y \mapsto \psi(y)$ 转换为 $G$。

因此这个映射是解析的。

令$p$为H的典范映射进入齐次空间$H/N$。那么 $\theta^{-1}(\mathrm{Aut}(H, N))$ 是 $u \in \mathrm{Aut}\ L(H)$ 的集合使得
$$
p(\theta(u)g) = p(e), \quad p(\theta(u^{-1})g) = p(e)
$$
对于所有$g \in N$。由§ 8, no. 2、定理2和推论2至定理2，证明了(ii)。

假设 N 是离散且正规的。让$w \in \mathrm{Aut}\ G$。然后
$$
L(p \circ \eta(w)) = L(\eta(w)) = L(w) = L(w \circ p)
$$
因此$p \circ \eta(w) = w \circ p$，因此$\eta(w) \in \mathrm{Aut}(H, N)$。显然，$\mathrm{Aut}\ G$到$\mathrm{Aut}(H, N)$的映射$\eta$是单同态。这个同态是满射，因为 $p : H \to G$ 是淹没。

令 G 为 G 的局部紧致群和 $\Gamma$ 自同构群。回想一下，拓扑 $\mathscr{T}_\beta$ 已在 $\Gamma$ 上定义（一般拓扑、章 X, § 3, no. 5）。它是最粗糙的拓扑，其中$\Gamma$进入$C_c(G; G)$的映射$v \mapsto v$和$v \mapsto v^{-1}$（G的连续映射进入G的空间与紧收敛拓扑）是连续的。 拓扑 $\mathscr{T}_\beta$ 与 $\Gamma$ 上的群结构兼容（前述）。对于 G 的每个紧凑子集 L 和 G 中$e_G$ 的每个邻域 U，令 $N(L, U)$ 为 $\phi \in \Gamma$ 的集合，使得对于所有 $g \in L$ 都有 $\phi(g) \in gU$ 和 $\phi^{-1}(g) \in gU$；那么$N(L, U)$形式是$e_\Gamma$的邻域的基本系统。如果 G 由紧致子集 C 生成，则拓扑 $\mathscr{T}_\beta$ 也是最粗糙的拓扑，其中映射 $v \mapsto v|C$ 和 $v \mapsto v^{-1}|C$ 的 $\Gamma$ 到 $C_u(C; G)$ 是连续的（对于每个紧致对于足够大 n)，G 的子集包含在$(C \cup C^{-1})^n$ 中。如果 K 是局部紧的并且 V 是 K 上的有限维向量空间，则 $\mathbf{GL}(V)$ 上的拓扑 $\mathscr{T}_\beta$ 只是通常的拓扑。

#### 定理 1 {#lie-iii-s10-thm-1 .statement tag=0ALE}

设 G 是有限维李群和 $G_0$ 其单位分量。假设 G 由 $G_0$ 和元素的有限数生成。

(i) 在$\mathrm{Aut}\ G$上存在且仅有一个解析流形结构满足以下条件：
(AUT) 对于每个解析流形 M 和 M 到 $\mathrm{Aut}\ G$ 的每个映射 f，当且仅当 $M \times G$ 到 G 的映射 $(m, g) \mapsto f(m)g$ 是解析的。

假设在叙述的其余部分中，Aut G 有这个结构。
(ii) Aut G 是有限维李群。
(iii) 将 Aut G 的态射 $\phi : u \mapsto L(u)$ 转化为 Aut L(G) 是解析的。
(iv) 如果 G 是连通的，$\phi$ 是李群 Aut G 的同构到 Aut L(G) 的谎言子群上；如果 G 是单连通的，则该 Lie 子群等于 Aut L(G)。
(v) 设$a$为G的无穷小自同构的集合，则$a$为向量域的李代数以及与映射相关的无穷小运算的律 (Aut G) $\times$ G 的 $(u, g) \mapsto u(g)$ 到 G 中是 L(Aut G) 到 $a$ 的同构。
(vi) 李群 Aut G 的拓扑为拓扑 $\mathscr{T}_\beta$。
(a) (i) 中考虑的解析结构的唯一性是显而易见的。
(b) 假设 G 是连通的。令 H 为 G 的通用覆盖空间，$p$ H 在 G 上的规范态射，且 N = Ker $p$。我们将引理的记号$\theta$、$\eta$和Aut(H,N)引入。我们通过$\theta$将AutL(G)的迁移李群结构转换为Aut H。然后 Aut H 变成有限维李群并且 Aut(H, N) 成为 Aut H 的谎言子群 (引理 4 (ii))。我们通过 $\eta^{-1}$ 将 Aut(H, N) 迁移李群结构转换为 Aut G。那么Aut G就变成了有限维的李群。满足定理的性质 (ii)、(iii) 和 (iv)，并且 (Aut G) $\times$ G 的映射 $(u, g) \mapsto u(g)$ 到 G 中是解析的 (引理 4 (i))。设 M 是 M 到 Aut G 的解析流形、$f$ 映射以及 M $\times$ G 到 G 的 $\phi$ 映射 $(m, g) \mapsto f(m)g$。显然，如果 $f$ 是解析的，$\phi$ 是分析的。假设 $\phi$ 是解析的。则 T$\phi$: TM $\times$ TG $\to$ TG 是解析的；因此，其限制到 M $\times$ L(G)，即 M $\times$ L(G) 到 L(G) 的映射 $(m, x) \mapsto L(f(m))x$ 是解析的；由于 L(G) 是有限维的，因此 M 到 Aut L(G) 中的映射 $m \mapsto L(f(m))$ 是解析的，因此 $f$ 是解析的。因此(i)成立。

让L(G) 被赋予范数。对于所有$\lambda > 0$，令B_\lambda为L(G)中中心0、半径为$\lambda$的开球。我们选择 $\lambda > 0$ 足够小，使得 $\psi = \exp_G|_{B_\lambda}$ 成为解析流形 B_\lambda 到 G 的开子流形 $\psi(B_\lambda)$ 的同构。令 $\Phi$ 为 Aut G 上的滤波器。对于 $\Phi$ 收敛到在Aut G中$\mathrm{Id}_G$，$L(\Phi)$收敛到Aut L(G)中的$\mathrm{Id}_{L(G)}$是充分必要的，因此$L(\Phi)|_{B_{\lambda/2}}$和$L(\Phi)^{-1}|_{B_{\lambda/2}}$一致收敛到$\mathrm{Id}_{B_{\lambda/2}}$。这个条件意味着$\Phi|\psi(B_{\lambda/2})$和$\Phi^{-1}|\psi(B_{\lambda/2})$一致收敛到$\mathrm{Id}_{\psi(B_{\lambda/2})}$。相反，假设$\Phi|\psi(B_{\lambda/2})$一致收敛于$\mathrm{Id}_{\psi(B_{\lambda/2})}$。存在 M $\in \Phi$，如果$u \in M$，则$u(\psi(B_{\lambda/2})) \subset \psi(B_{2\lambda/3})$；则L(u)(B_{\lambda/2})是L(G)的连通子集，其$\exp_G$下的像包含在$\psi(B_{2\lambda/3})$中，因此L(u)(B_{\lambda/2})不满足$B_\lambda - B_{2\lambda/3}$ 因此 L(u)(B_{\lambda/2}) $\subset$ B_\lambda;那么$\Phi|\psi(B_{\lambda/2})$均匀收敛到$\mathrm{Id}_{\psi(B_{\lambda/2})}$的假设意味着$L(\Phi)|_{B_{\lambda/2}}$均匀收敛到$\mathrm{Id}_{B_{\lambda/2}}$。由此可见：

$$
(\Phi \text{ converges to } \mathrm{Id}_G \text{ in Aut } G) \iff (\Phi \text{ converges to } \mathrm{Id}_G \text{ under } \mathscr{T}_\beta).
$$

这就证明了(vi)。

设 D 为无穷小运算的律，与 G 上 Aut(G) 的左运算的律相关联。由no. 1、$D(L(\text{Aut } G)) = a$ 的命题 1 和 2。因此，a 是向量域的李代数，D 是 a 上的 $L(\text{Aut } G)$ 的态射。令$x_1$和$x_2$为$L(\text{Aut } G)$的元素，使得$D(x_1) = D(x_2)$。那么G上的运算$(\lambda, g) \mapsto (\exp \lambda x_1)g$的律和K的$(\lambda, g) \mapsto (\exp \lambda x_2)g$有相同的关联无穷小运算的律；因此，对于足够小的$|\lambda|$，$\exp \lambda x_1$和$\exp \lambda x_2$重合在e的邻域上（$§ 4$，no. 7，定理6），从而$\exp \lambda x_1 = \exp \lambda x_2$。由此可见，$x_1 = x_2$，因此 D 是 $L(\text{Aut } G)$ 的同构到 a 上。

至此，定理对于G连通而言已被完全证明。

(c) 我们转向一般情况。到假设，G由$G_0$和元素$x_1, x_2, \ldots, x_n$的有限数生成。每$u \in \text{Aut } G$离开$G_0$稳定。令 $\text{Aut}_1 G$ 为 $u \in \text{Aut } G$ 的集合，将经过商，给出 $G/G_0$ 的恒等式自同构。这是正常的子群 $\text{Aut } G$。通过证明的部分(b)，$\text{Aut } G_0$具有规范的李群结构和$G_0^n \times \text{Aut } G_0$的映射$(g_1, g_2, \ldots, g_n, u) \mapsto (ug_1, ug_2, \ldots, ug_n)$到$G_0^n$的解析性。令P为$\text{Aut } G_0$乘$G_0^n$的相应的半直积；它是有限维李群 ($§ 1$, no. 4, 命题 7)。

如果$w \in \text{Aut}_1 G$，我们写
$$
w_0 = w|G_0 \in \text{Aut } G_0 \\
w_i = x_i^{-1}w(x_i) \in G_0 \quad (1 \leq i \leq n) \\
\zeta(w) = ((w_1, \ldots, w_n), w_0) \in P.
$$
对于 $\text{Aut}_1 G$ 中的所有 $w, w'$，
$$
\begin{align*}
\zeta(w)\zeta(w') &= ((w_1, \ldots, w_n)(w_0(w'_1), \ldots, w_0(w'_n)), w_0w'_0) \\
&= ((w_1w_0(w'_1), \ldots, w_nw_0(w'_n)), w_0w'_0) \\
&= ((x^{-1}w(x_1)w(x_1^{-1}w'(x_1)), \ldots, x_n^{-1}w(x_n)w(x_n^{-1}w'(x_n))), w_0w'_0) \\
&= (((ww')_1, \ldots, (ww')_n), (ww')_0) \\
&= \zeta(ww')
\end{align*}
$$
因此 $\zeta$ 是 $\text{Aut}_1 G$ 的同态到 P 中。这个同态显然是内射的。

我们证明$\zeta(\text{Aut}_1 G)$在P中是封闭的。设$\Phi$是$\text{Aut}_1 G$上的过滤器，使得$\zeta(\Phi)$收敛到P的点$((w_1, \ldots, w_n), w_0)$。然后$\Phi$逐点收敛到G的映射v到G中。显然v是群 G 的自同态。此外，v 使每个陪集模$G_0$ 稳定且$v|G_0 = w_0$。由此可见$v \in \text{Aut}_1 G$。作为$\zeta(v) = ((w_1, \ldots, w_n), w_0)$，我们已经证明$\zeta(\text{Aut}_1 G)$在P中是闭的。

(d) 在部分 (d) of 证明中，我们假设$K = \mathbf{R}$。通过$§ 8$，no. 2，定理 2，$\zeta(\text{Aut}_1 G)$是P的谎言子群。我们迁移实李群结构在$\zeta(\text{Aut}_1 G)$到$\text{Aut}_1 G$通过$\zeta^{-1}$。因此$\text{Aut}_1 G$变成有限维李群。

令 M 为 M 到 Aut_1G 的解析流形、f 映射以及 M × G 到 G 的 φ 映射 (m, g) ↦ f(m)g。我们有以下等价：

法分析
⇔ 映射 m: ↦ (f(m))_i，其中 0 ≤ i ≤ n，是解析的
⇔ {M 的映射 m ↦ f(m)x_i 进入 G，对于 1 ≤ i ≤ n，是解析的
和
映射 (m, g) ↦ M × G_0 到 G 的 f(m)g 是解析的
⇔ φ 是解析的。

对于 w ∈ Aut_1G，L(w) = L(w_0)，因此 Aut_1G 的态射 w ↦ L(w) 到 Aut L(G) 是解析的。我们在(b)中看到，与G上Aut_1G的运算的律相关的无穷小运算的律是a上的L(Aut_1G)的同构。

令 C 为 G_0 生成的 G_0 的紧致子集。为了使滤波器 Φ 在 Aut_1G 上收敛到 $\mathrm{Id}_G$，Φ|(C ∪ {x_1} ∪ ... ∪ {x_n}) 和 Φ^{-1}|(C ∪ {x_1} ∪ ... ∪ {x_n}) 均匀收敛到

Id_a|(C∪{x_1}∪...∪{x_n})。

因此，Aut_1G 的拓扑是拓扑 $\mathscr{T}_\beta$。

显然，Aut_1G 在 Aut G 中以拓扑 $\mathscr{T}_\beta$ 打开。在 Aut G 李群结构上存在与此拓扑兼容，并在上面构造的 Aut_1G 结构上进行归纳（§ 8, no. 1，推论 2 到定理 1）。 李群 Aut G 具有定理的属性这一事实源自 Aut_1G 的相应的属性。

(e) 在部分 (e) of 证明中，我们假设 K = C。由(c)和§ 8, no. 2的定理2，在Aut_1G上存在实李群结构，使得z是Aut_1G的同构到P的实谎言子群上。

G 上 (Aut_1G) × G 的运算 (w, g) ↦ wg 律是实解析。令 D 为无穷小运算的关联律。通过命题 1 和 2 of no. 1，D(L(Aut_1G)) = a。

对于所有 α ∈ a，令 α_0 表示 α 到 G_0 的限制；它是 G_0 的无穷小自同构，我们认同，因为证明的部分 (b)，元素为 L(Aut G_0)。对于 1 ≤ i ≤ n，我们写

$$ \alpha_i = x_i^{-1} \alpha(x_i) \in L(G) = L(G_0). $$

最后，我们写$f(\alpha) = ((\alpha_1, ..., \alpha_n), \alpha_0) \in L(P)$。那么 f 是 a 到 L(P) 的 C 线性映射。

另一方面，显然$L(\zeta) = f \circ D$。 因此$L(\zeta)(L(Aut_1G)) = f(a)$是L(P)的复数向量子空间。 By Proposition 2 of § 4, no. 2, $\zeta(Aut_1G)$ is a complex Lie subgroup of P and we can proceed exactly as in (d): we transport the complex Lie group structure on $\zeta(Aut_1G)$ to Aut_1G by means of $\zeta^{-1}$ and we see as in (d) that Aut_1G has the properties analogous to properties (i), (ii), (iii), (v) and (vi) of the theorem.

显然，Aut₁G 在 Aut G 中以拓扑 $\mathscr{T}_\beta$ 开路。让$w \in \mathrm{Aut}\ G$。令 $\sigma$ 为 Aut₁G 的自同构 $v \mapsto wvw^{-1}$。它是实解析的（$§ 8$、no. 1、定理 1），$L(\sigma)$是$L(\mathrm{Aut}_1 G)$的$\mathbf{R}$自同构，并且

$$
D \circ L(\mathrm{Aut}_1 G) \circ D^{-1}
$$

是$a$的$\mathbf{R}$自同构。这个自同构也是$a$的自同构由$w$由结构的迁移衍生而来；由于$w$是K-解析的，我们看到$L(\sigma)$是K-线性的。因此 $\sigma$ 是 K 解析 ($§ 3$, no. 8, 命题 32)。由 $§ 1$、no. 9、命题 18，Aut G 上存在且仅有一个李 K 群结构，使得 $\mathrm{Aut}_1 G$ 是 Aut G 的开李子群。事实上，这个结构具有定理的性质，由相应的的性质得出$\mathrm{Aut}_1 G$。

#### 推论 1 {#lie-iii-s10-thm-1-cor-1 .statement tag=0ALF}

*设 G 是有限维实李群和 $G_0$ 其单位分量。假设 G 由 $G_0$ 和元素的有限数生成。那么 Aut G 有拓扑 $\mathscr{T}_\beta$ 并且是有限维实李群。*

#### 推论 2 {#lie-iii-s10-thm-1-cor-2 .statement tag=0ALG}

*令 G 为半单连接实数或复数李群。 群 Int G 是 Aut G 的恒等分量。*

映射 $u \mapsto L(u)$ 是 Aut G 的同构到 Aut $L(G)$ (定理 1) 的谎言子群上。这个同构下的Int G的像是Ad G。但是Ad G是Aut$L(G)$的恒等分量（$§ 9$，no. 8，命题30（ii））。

### 3. 李群的自同构群（超距案例）

#### 定理 2 {#lie-iii-s10-thm-2 .statement tag=0ALH}

*当 K 是超度量且局部紧致且 G 为紧李群时，定理 1 的断言 (i)、(ii)、(iii)、(v) 和 (vi) 为真。*
(a) (i) 中考虑的解析结构的唯一性是显而易见的。
(b) 假设 G 是由可范数李代数 L 定义的李群。 那么G是L中的开球和闭球。 让$w \in \mathrm{Aut}\ G$。 然后$L(w)$重合，$w$在邻域为0。 让$x \in G$。 设$p$为剩余类域的特征。 那么当$n$趋向于$+\infty$时，$p^n x$趋于0。 因此存在$n$使得$w(p^n x) = L(w)(p^n x)$。 所以

$$
p^n w(x) = w(x)^{p^n} = w(x^{p^n}) = w(p^n x)
= L(w)(p^n x) = p^n L(w)(x)
$$

从而$w(x) = L(w)(x)$。因此，$w = L(w)|G$。

令$\Gamma$为$\gamma \in \mathrm{Aut}\ L(G)$的集合，使得$\gamma(G) = G$。由于 G 在 $L(G)$ 中是开紧的，因此 $\Gamma$ 是 $\mathrm{Aut}\ L(G)$ 的开子群。由上式可知，Aut G 可以用$\Gamma$、从而来识别，Aut G 上存在李群结构，由此定理 1 的性质（i）、（ii）、（iii）、（vi）是显而易见的。 性质 (v) 由no. 1 的命题 1 和 3 得出。

(c) 我们转向一般情况。由§ 7, no. 1，命题 1，存在G的开紧子群 G_0，其在(b)中考虑为型。然后 G 由 G_0 和元素 x_1, x_2, ..., x_n 的有限数生成。令 Aut_1G 为 u ∈ Aut G 的集合，使得 u(G_0) = G_0 且 u(x_iG_0) = x_iG_0（1 ≤ i ≤ n）。我们将定义与定理 1 的证明一样，部分 (c)，将 Aut G_0 的半直接乘积 P 通过 G_0^n 和 Aut_1G 的单同态 ζ 转换为 P，其像在 P 中闭合。

(d)、(e)：论证与定理 1 的证明部分 (d)、(e) 完全相同，其中 R 替换为 Q_p，并使用命题 3 代替命题 2。

#### 注 {#lie-iii-s10-n3-rem-1 .statement tag=0ALI}

如果 K = Q_p，且李群 G 由紧致子集 (cf. 习题 2) 生成，则定理 1 的断言 (i)、(ii)、(iii) 和 (vi) 仍然为真，但 (v) (习题 3) 不为真。

### 习题{#lie-iii-s10-exercises}

参见[习题为 § 10](exercises/s10/)。
