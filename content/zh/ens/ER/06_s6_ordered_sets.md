---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 6
section_title: Ordered sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 373-380
pdf_pages: 0378-0385
extraction: ocr
statements: 0
exercises: 0
content_sha256: 900b66fef71f4f6a3f2819dc46fdfe0552d7bb3d1f25f3335dfb460ddbc4d260
translated_from: content/en/ens/ER/06_s6_ordered_sets.md
translation_method: google
source_content_sha256: 971a0a96b2a9c9ae41e13935799a40e904d52151f935272d34c3c4e23f4b84cc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 92814ad0668c8b605cce9ebaf4e876394b82fe094020cc48709c9a76e003a0b8
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 6. 有序集

1. 集合 E 的两个泛型元素 x, y 之间的关系 $\omega\{x,y\}$，如果满足以下两个条件，则称其为 E 上的序关系：
(a) 关系“$\omega\{x,y\}$和$\omega\{y,z\}$”意味着“$\omega\{x,z\}$”(传递性)。
(b) 关系“$\omega\{x,y\}$和$\omega\{y,x\}$”相当于“$x=y$”。
条件 (b) 意味着 $\omega$ 是自反的。

设C为$E\times E$的子集，由关系$\omega\{x,y\}$定义为对$(x,y)$的性质。则条件 (a) 和 (b) 分别等价于： (a′) $C \circ C \subset C$； (b′) $C \cap \overline{C}^{-1} = \Delta$。这些意味着$C \circ C = C$。

当我们考虑集合$E$上的特定序关系时，我们说$E$是按这个关系排序的，并且关系定义序结构（cf.§8） （或订购）$E$。

如果$\omega\{x,y\}$在$E$上是序关系，那么$\omega^{-1}\{x,y\}$也是。这两个序关系，以及它们的定义，据说是彼此相反的。

令$\omega\{x,y\}$为$E$上的序关系，并令$A$为$E$的任意子集。 $A$ 的两个泛型元素 $x,y$ 之间的关系 $\omega\{x,y\}$ 则为 $A$ 上的序关系，并且$A$ 上的定义的排序据说是由$\omega\{x,y\}$ 上定义的排序引起的$E$。 $E$ 上的给定排序据说是 $A$ 上诱导排序的扩张。

$E$ 的两个泛型元素 $x,y$ 之间的自反和及物关系 $\overline{\omega}\{x,y\}$ 在 $E$ 上称为预序关系。 关系“$\overline{\omega}\{x,y\}$和$\overline{\omega}\{y,x\}$”是$E$上的等价关系$R$，并且$\overline{\omega}\{x,y\}$与此关系兼容（在$x$和$y$中）。 经过至商（相对于$x$和$y$），集合$E/R$序关系上的$\overline{\omega}\{x,y\}$诱导，据说与$\overline{\omega}\{x,y\}$相关。 集合赋予预序关系称为预购集合。

2. 包含关系“$Y \subset X$”是任意集合$E$的子集$\mathfrak{P}(E)$的集合上的序关系。

如果 $E$ 和 $F$ 是两个集合（可能不同，也可能不同），关系“$g$ 扩展 $f$”是所有映射中集合上的序关系子集的 $E$ 变为 $F$。

自然整数 [^1] 中的集合 $\mathbf{N}$ 按关系“$x \leq y$”订购。

3. 类推最后一个例，当集合$E$按关系$\omega\{x,y\}$排序时，通常可以方便地用$x \leq y$或$y \geq x$表示关系$\omega\{x,y\}$；这些关系被读作“$x$小于$y$”，或“$y$大于$x$”[^2]。 关系“$x<y$”和“$y>x$”（读作“$x$严格小于$y$”，或“$y$严格大于$x$”）通过定义相当于“$x\leq y$和$x\neq y$”。

关系“$x\leq y$”相当于“$x<y$或$x=y$”。 关系“$x\leq y$和$y<z$”意味着“$x<z$”；类似地，“$x<y$和$y\leq z$”意味着“$x<z$”。

4. 集合 E 的子集 X，按关系“$\leq$”排序，如果对于所有 $x\in X$ 和所有 $y\in X$，我们有 $x\leq y$ 或 $y\leq x$（或者等价地，$x<y$ 或 $x=y$ 或$x>y$，这三种关系是互斥的）。
有序集的空子集始终是全序的。 可能会发生整个集合 E 完全有序的情况，就像集合 $\mathbf{N}$ 和关系 $x\leq y$ 的情况一样。
全序集中的每个子集都通过归纳排序完全排序。
在有序集合 E 中，如果 $a$ 和 $b$ 是两个元素，则元素 $x$ 的 E 由……组成的 $a\leq b$、子集，则 $a\leq x\leq b$ 被称为*闭区间，其中左端点a和右端点b*，用$[a,b]$表示。 所有$x\in E$的集合，使得$a\leq x<b$（或$a<x\leq b$）被称为*右侧半开区间*（或*左侧*），端点为$a$和$b$，并由$[a,b[$（或$]a,b]$）表示。 所有$x\in E$的集合，使得$a<x<b$被称为具有端点$a$和$b$的*开区间*，并且由$]a,b[$表示。
所有$x\in E$中的集合，使得$x\leq a$（或$x<a$）称为*封闭*（或*开*）*区间，左侧无界，右侧端点a*，并用$] \leftarrow,a]$（或$]\leftarrow,a[$）表示；同样，所有$x\in E$中的集合，使得$x\geq a$（分别为$x>a$）被称为*封闭*（分别为*开*）*区间在右侧无界，左端点a*，并由$[a,\rightarrow[$（分别为$]a,\rightarrow[$）表示。 最后，我们认为 E 本身是一个*开区间在两个方向上无界*，因此我们用$]\leftarrow,\rightarrow[$表示它。

5. 如果X是有序集合E的子集，则X至多有一个元素$a$，使得所有$x\in X$都有$a\leq x$；当存在元素 $a$ 和这个性质时，称为X* 的*最小元素。同样，至多存在一个元素 $b$，使得 $x\leq b$ 对于所有 $x\in X$； $b$，如果存在，则称为X*的*最大元素。
在*全序集 E*中，每个*有限*非空子集都有最大元素和至少元素，分别称为子集的*最大和最小*元素。
一个有序的集合，其中每个非空子集至少有元素被称为“良序”。 自然整数的集合 $\mathbf{N}$ 是有序的； $\mathbf{N}$的子集有最大元素当且仅当它是有限且非空的。通过使用选择公理，可以证明在每个集合上都存在良序（*Zermelo的定理*）。
在集合 E 子集集合 $\mathfrak{P}(E)$ 中，按包含排序，$\mathfrak{P}(E)$ 子集 $\mathfrak{F}$ 具有至少元素当且仅当集合交 $\mathfrak{F}$属于到$\mathfrak{F}$，那么这个交就是最小的元素。类似地，$\mathfrak{F}$具有最大元素当且仅当$\mathfrak{F}$属于集合并到$\mathfrak{F}$，而这个并则为最大元素。
如果对于每个$y\in E$，存在$x\in X$使得$y\leq x$（或$y\geq x$），则有序集合E的子集X被称为E中的*cofinal*（或*coinitial*）。说有序集合 $E$ 具有最大的（或至少）元素意味着存在单个元素的 $E$ 由……组成的共尾（或初始）子集。

6. 设$X$为有序集合$E$的子集。每个$x\in X$都不存在元素$z\in X$，其中$z<x$被称为$X$的*最小元素*。每个$y\in X$都不存在元素$z\in X$，其中$z>y$被称为$X$的*极大元素*。 极大元素中的集合（或最小元素中的集合）可能为空；它也可能是无限的。如果 $X$ 至少有元素 $a$，则 $a$ 是 $X$ 的*唯一*最小元素；同样，如果$X$有最大元素$b$，那么$b$是$X$中*唯一*的极大元素。

7. 设$X$为有序集合$E$的子集。如果元素$x\in E$使得$z\leq x$对于所有$z\in X$，则$x$被称为$X$的*上界*。类似地，元素$y\in E$，使得所有$z\in X$的$z\geq y$被称为$X$的*下界*。

子集$X$的上界集合（或下界集合）可能为空。 子集$X$，其上界（或下界）的集合不为空，则称为*上界*（或*下界*）。 上下都有界的集合被简单地称为“有界”。 每个大于$X$的上界的元素都是$X$的上界； $X$ 中每小于下界的元素就是 $X$ 中的下界。

如果子集$X$的上界集合具有至少元素$a$，则$a$称为$X$的*最小上界*或*最高*。如果$X$的下界的集合有最大元素$b$，则$b$称为$X$的*下确界*或*下确界*。如果这些边界存在，则它们通过定义是唯一的，并且分别用$\sup_E X$（或$\sup X$）、$\inf_E X$（或$\inf X$）表示。如果$X$有最大元素，则它是其最小的上界；如果 $X$ 至少有元素，则为它的下确界。相反，如果 $X$ 的最小上界（或下确界）存在且属于到 $X$，则它是 $X$ 的最大的（或元素）。

设$f$为集合$A$到$E$的映射。如果$f(A)$在上方有界（分别在下方有界，有界），则$f$被称为*在上方有界*（分别在*下方有界，有界*）。如果 $f(A)$ 在 $E$ 中具有至少上界（或下确界），则此界限称为 $f$ 的*最小上界*（或 *下确界*），并用 $\sup_{x\in A} f(x)$（或 $\inf_{x\in A} f(x)$）表示。

8. 一个预定的集合$E$，其中$E$的每个*有限非空*子集都*上界*（或*下界*）被称为*右向*（或*定向*）（分别*左向*）。

一个有序的集合 $E$，其中 $E$ 的每个*有限非空* 子集都有至少上界和下确界称为*格子*。

任何集合的子集的集合按包含排序，是一个*格子*。每个全序集都是一个格子。

9. 如果有序集合 E 满足以下条件，则称其为“归纳式”：*E 的每个总有序子集都有上界*。

集合 $\mathfrak{P}(E)$，按包含排序，是归纳的。 当 f 和 g 之间按关系“g 扩展 f”排序时，集合 E 的子集映射集合也变成集合 F。

归纳集合的任意子集通常不是归纳的。但如果 a 是归纳集合 E 的任意元素，则所有元素 $x \in E$ 的 E 由……组成子集使得$x \geq a$ 是归纳性的。

10. 借助选择公理证明以下命题，称为*Zorn的引理*：

*每个订购的感应集合至少有一个极大元素。*

11. 集合 E 的子集 $\mathfrak{P}(E)$ 集合中，按包含排序，E 的子集集合 $\mathfrak{F}$ 中最小的上界为$\mathfrak{F}$ 的集合 *并*。应用 Zorn 的引理给出以下结果：

*如果$\mathfrak{F}$是集合E的子集的集合，则对于$\mathfrak{F}$的每个子集$\mathfrak{G}$（按包含的关系完全排序），$\mathfrak{G}$的集合的并属于到$\mathfrak{F}$，则$\mathfrak{F}$至少有一个极大元素*（即E的子集，其中属于到$\mathfrak{F}$，但不包含在E 属于到$\mathfrak{F}$的任何其他子集中）。

集合 E 的子集集合 $\mathfrak{F}$ 被认为是*有限的特征标*，如果性质“$X \in \mathfrak{F}$”*等价于*性质“X的每个*有限*子集” 属于至 $\mathfrak{F}$”。有了这个定义，我们就有了以下定理：

*有限特征标的E的子集的每个集合至少有一个极大元素。*

12. 有序集合 E 的子集 A 的映射 f 到有序集合 F 被称为 *递增*（或 *递减*），如果 A 的泛型元素之间的关系 $x \leq y$ 意味着 $f(x) \leq f(y)$（或 *递减*）。 $f(y) \leq f(x)$）。 因此，A 上的每个常数函数都是递增和递减，并且如果 A 是（右或左）有向的，则逆命题为真。

如果关系 $x < y$ 蕴含 $f(x) < f(y)$（或 $f(x) < f(y)$），则映射 f 被称为 *严格递增的*（或 *严格递减*）。

如果 E 是*全序*，则 E 的子集 A 的每个 *严格递增的*（或 *严格递减*）映射到有序集合 F 都是*内射*。

如果I是指标的*有序*集合，则集合E的子集的$(X_i)_{i \in I}$族被称为*递增*（或*递减*），如果映射$i \to X_i$为I入$\mathfrak{P}(E)$，按包含顺序排列，是递增（分别为递减）。

13. 令I为有向集合，并令$(E_\alpha)_{\alpha \in I}$为由I索引的集合族。对于I中指标的每个对$(\alpha, \beta)$使得$\alpha \leq \beta$，令$f_{\beta \alpha}$为映射*of*$E_\alpha$*进入*$E_\beta$，并假设关系$\alpha \leq \beta \leq \gamma$意味着$f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha}$。

令F为集合$(E_\alpha)_{\alpha \in I}$族的和。 通过滥用语言，我们将F的认同$E_\alpha$与相应的子集。 给定 F 中的两个元素 x 和 y，令 R $\{x, y\}$ 为以下关系（其中$\alpha$和$\beta$表示$I$的元素，使得$x\in E_\alpha$和$y\in E_\beta$）：“存在$\gamma\in I$使得$\gamma\geq\alpha$、$\gamma\geq\beta$、$f_{\gamma\alpha}(x)=f_{\gamma\beta}(y)$”。 那么$R$就是$F$上的等价关系。 令$E$为商集$F/R$，令$f$为典范映射$F\to F/R$。 集合$E$称为直极限家族*$(E_\alpha)_{\alpha\in I}$*相对于映射*$(f_{\beta\alpha})$家族，$f$至$E_\alpha$的限制$f_\alpha$称为典范映射家族$E_\alpha$ 变为$E$。 每当 $\alpha\leq\beta$ 时，我们就有 $f_\beta\circ f_{\beta\alpha}=f_\alpha$。 我们写

$$
E=\underset{\longrightarrow}{\lim}\,(E_\alpha,f_{\beta\alpha})
$$

或者在不存在混淆风险的情况下简单地输入$E=\underset{\longrightarrow}{\lim}\,E_\alpha$。通过滥用语言，对$((E_\alpha),(f_{\beta\alpha}))$被称为相对于*$I$的集合的*直接系统。

如果$f_{\beta\alpha}$是单射的，那么$f_\alpha$也是单射的。 在这种情况下，我们通常应该认同$E_\alpha$和$f_\alpha(E_\alpha)$，因此将$E$视为$E_\alpha$的*并*。 相反，如果集合$E'$是子集的$(E'_\alpha)_{\alpha\in I}$族的并，则关系$\alpha\leq\beta$意味着$E'_\alpha\subset E'_\beta$，并且如果（对于$\alpha\leq\beta$）$j_{\beta\alpha}$表示典范嵌入将$E'_\alpha$转化为$E'_\beta$，那么我们可以将认同$\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$与$E'$，将$E'_\alpha$的典范映射转化为$\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$，将$E'_\alpha$的典范嵌入转化为$E$。

更一般地，令$(E_\alpha,f_{\beta\alpha})$相对于$I$为集合的直接系统，并且对于每个$\alpha\in I$，令$g_\alpha$为$E_\alpha$的映射到集合$E'$，使得关系 $\alpha\leq\beta$ 意味着$g_\beta\circ f_{\beta\alpha}=g_\alpha$。那么$E=\underset{\longrightarrow}{\lim}\,E_\alpha$存在唯一映射$g$到$E'$，使得$g_\alpha=g\circ f_\alpha$对于所有$\alpha\in I$。 映射 $g$ 是满射当且仅当 $E'$ 是 $g_\alpha(E_\alpha)$ 的并。 映射 $g$ 是单射当且仅当，对于每个 $\alpha\in I$、关系 $x\in E_\alpha$、$y\in E_\alpha$、$g_\alpha(x)=g_\alpha(y)$ 意味着存在 $\beta\geq\alpha$ 使得 $f_{\beta\alpha}(x)=f_{\beta\alpha}(y)$。如果$g$是双射，则$E'$是有时，与$E_\alpha$的直极限相同。

令$(A_\alpha,\varphi_{\beta\alpha})$和$(B_\alpha,\psi_{\beta\alpha})$是集合相对于相同指标集合$I$的两个直接系统。令$A=\underset{\longrightarrow}{\lim}\,(A_\alpha,\varphi_{\beta\alpha})$、$B=\underset{\longrightarrow}{\lim}\,(B_\alpha,\psi_{\beta\alpha})$，对于每个$\alpha\in I$，让$\varphi_\alpha$（或$\psi_\alpha$）表示$A_\alpha$的典范映射到$A$（或$B_\alpha$到$B$）。对于每个$\alpha\in I$，让$u_\alpha$是$A_\alpha$到$B_\alpha$的映射，这样只要$\alpha\leq\beta$就有$u_\beta\circ\varphi_{\beta\alpha}=\psi_{\beta\alpha}\circ u_\alpha$。 $(u_\alpha)$ 家族被称为 *直接系统 of 映射 of* $(A_\alpha,\varphi_{\beta\alpha})$ *到* $(B_\alpha,\psi_{\beta\alpha})$。在这些条件下，存在唯一映射$u:A\to B$，使得$u\circ\varphi_\alpha=\psi_\alpha\circ u_\alpha$适用于所有$\alpha\in I$。 映射$u$被称为*$u_\alpha$的*直极限，并写作$u=\underset{\longrightarrow}{\lim}\,u_\alpha$，前提是不存在混淆的风险。令$(C_\alpha,\theta_{\beta\alpha})$相对于$I$为集合的另一个直接系统，令$(v_\alpha)$相对于$(C_\alpha,\theta_{\beta\alpha})$为$(B_\alpha,\psi_{\beta\alpha})$的映射直接系统，并令$v=\underset{\longrightarrow}{\lim}\,v_\alpha$。然后

$$
\underset{\longrightarrow}{\lim}\,(v_\alpha\circ u_\alpha)=v\circ u.
$$

保留上面的记号，令$D_\alpha=A_\alpha\times B_\alpha$和$\omega_{\beta\alpha}=\varphi_{\beta\alpha}\times\psi_{\beta\alpha}$。那么家庭$(D_\alpha,\omega_{\beta\alpha})$就是直接系统/集合。设$D=\underset{\longrightarrow}{\lim}\,(D_\alpha,\omega_{\beta\alpha})$，设$\omega_\alpha$为$D_\alpha$的典范映射入$D$，设$D'=A\times B$，并设$\omega'_\alpha=\varphi_\alpha\times\psi_\alpha$。那么存在一个唯一的双射（称为规范）$f:D\to D'$，使得$f\circ\omega_\alpha=\omega'_\alpha$适用于所有$\alpha\in I$。我们通常会使用直极限中的认同乘积$D'$和乘积$D_\alpha$中的直极限$D$。

设$J$为$I$的并尾子集；那么$J$也是有向的。如果$( (E_\alpha)_{\alpha\in I},(f_{\beta\alpha})_{\alpha,\beta\in I})$相对于$I$是集合的直接系统，则$( (E_\alpha)_{\alpha\in J},(f_{\beta\alpha})_{\alpha,\beta\in J})$相对于$J$是集合的直接系统。令$E'$为其直极限，并令$f'_\alpha$为所有$\alpha\in J$的$E_\alpha$到$E'$的典范映射。那么存在唯一映射$g:E'\to E$，使得$g(f'_\alpha(x))=f_\alpha(x)$对于所有$\alpha\in J$和所有$x\in E_\alpha$（其中$f_\alpha$表示$E_\alpha$到$E$的典范映射）。这个映射就是双射，通过它$E'$通常可以与$E$识别。

14. 令$I$为预定的集合，并让$(E_\alpha)_{\alpha\in I}$为由$I$索引的集合族。对于$I$的指标的每个对$(\alpha,\beta)$使得$\alpha\leq\beta$，令$f_{\alpha\beta}$为$E_\beta$的映射到$E_\alpha$，并假设关系$\alpha\leq\beta\leq\gamma$意味着$f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$。

令$G$为集合$(E_\alpha)_{\alpha\in I}$家族的乘积。令$E$为所有元素$x$中$G$由……组成的子集，其中满足所有关系$pr_\alpha x=f_{\alpha\beta}(pr_\beta x)$，对于指标$\alpha,\beta$的每个对这样$\alpha\leq\beta$。 集合$E$相对于映射$(f_{\alpha\beta})$的家族称为$(E_\alpha)_{\alpha\in I}$家族的逆极限，$pr_\alpha$至$E$的限制$f_\alpha$称为典范映射 $E$ 变为$E_\alpha$。每当 $\alpha\leq\beta$ 时，我们就有 $f_\alpha=f_{\alpha\beta}\circ f_\beta$。我们写

$$
E=\lim (E_\alpha,f_{\alpha\beta}),
$$

或者简单地

$$
E=\lim E_\alpha
$$

当不存在混淆风险时。

通过滥用语言，相对于$I$，对$((E_\alpha),(f_{\alpha\beta}))$被称为集合的逆系。

应该提到的是，即使所有 $E_\alpha$ 都非空且所有映射 $f_{\alpha\beta}$ 都是满射，$E$ 也可以为空。

对于每个$\alpha\in I$，让$g_\alpha$是集合$E'$到$E_\alpha$的映射，这样关系$\alpha\leq\beta$意味着$f_{\alpha\beta}\circ g_\beta=g_\alpha$。那么$E'$存在唯一映射$g$到$E$，使得$g_\alpha=f_\alpha\circ g$对于所有$\alpha\in I$。为了使$g$是单射的，对于$E'$的不同元素$x',y'$的每个对来说，应该存在$\alpha\in I$使得$g_\alpha(x')\neq g_\alpha(y')$。

令$(A_\alpha,\varphi_{\alpha\beta})$和$(B_\alpha,\psi_{\alpha\beta})$是集合相对于相同指标集合$I$的两个逆系。令$A=\lim(A_\alpha,\varphi_{\alpha\beta})$、$B=\lim(B_\alpha,\psi_{\alpha\beta})$，对于每个$\alpha\in I$，令$\varphi_\alpha$（分别为$\psi_\alpha$）为$A$到$A_\alpha$的典范映射（分别为$B$到$B_\alpha$）。对于每个$\alpha\in I$，令$u_\alpha$为$A_\alpha$到$B_\alpha$的映射，使得每当$\alpha\leq\beta$时$\psi_{\alpha\beta}\circ u_\beta=u_\alpha\circ\varphi_{\alpha\beta}$。 $(u_\alpha)$家族被称为$(A_\alpha,\varphi_{\alpha\beta})$的映射入$(B_\alpha,\psi_{\alpha\beta})$的逆系。在这些条件下，存在唯一映射$u:A\to B$，使得$\psi_\alpha\circ u=u_\alpha\circ\varphi_\alpha$适用于所有$\alpha\in I$。 映射$u$被称为$u_\alpha$的逆极限，在没有混淆风险的情况下写成$u=\underset{\longleftarrow}{\lim}\,u_\alpha$。令$(C_\alpha,\theta_{\alpha\beta})$相对于$I$为集合的另一个逆系，令$v_\alpha$相对于$(C_\alpha,\theta_{\alpha\beta})$为$(B_\alpha,\psi_{\alpha\beta})$的映射逆系，并令$v=\underset{\longleftarrow}{\lim}\,v_\alpha$。那么我们就有$\underset{\longleftarrow}{\lim}\,(v_\alpha\mathbin{\circ}u_\alpha)=v\mathbin{\circ}u$。
令$J$为$I$的共尾子集，并假设$J$是*有向的*（相对于从$I$导出的排序）。如果$((E_\alpha)_{\alpha\in I},(f_{\alpha\beta})_{\alpha,\beta\in I})$相对于$I$是集合的逆系，且逆极限$E$，则相对于$J$，$((E_\alpha)_{\alpha\in J},(f_{\alpha\beta})_{\alpha,\beta\in J})$也是集合的逆系。令$E'$为其逆极限，并令$f'_\alpha$为$E'$的典范映射进入$E_\alpha$，其中$\alpha\in J$。对于每个$x\in E$，让$g(x)=(f_\alpha(x))_{\alpha\in J}\in E'$（其中$f_\alpha$表示$E$中的典范映射到$E_\alpha$）。那么$g$就是$E$到$E'$的*双射*，由此$E'$通常被识别为$E$。

[^1]: 根据我们在本结果摘要中的点观点，我们假设整数的理论已知。 但不应该认为这个理论是构建集合论所必需的；读者会发现，通过参考章III，相反，可以从集合论的结果定义整数，并证明它们所有已知的性质。 In our terminology, $0$ belongs to $\mathbf{N}$.
[^2]: Thus, in our terminology, “less than” and “greater than” do not exclude “equal to”.
