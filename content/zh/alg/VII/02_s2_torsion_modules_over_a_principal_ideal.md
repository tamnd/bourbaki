---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 2
section_title: Torsion modules over a principal ideal domain
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.6-A VII.14, A VII.54-A VII.59
pdf_pages: 0365-0373, 0413-0418
extraction: ocr
subsections:
    - "no": 1
      title: Modules over a product of rings
      page: 6
      pdf_page: 365
    - "no": 2
      title: Canonical decomposition of a torsion module over a principal ideal domain
      page: 7
      pdf_page: 366
    - "no": 3
      title: 'Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate'
      page: 10
      pdf_page: 369
    - "no": 4
      title: 'Applications : II. The multiplicative group of units of the integers modulo a'
      page: 12
      pdf_page: 371
statements: 22
exercises: 15
content_sha256: f876f1a3279724d4563c51f0fa012da87ba4ed6fa24300d763b15455b0374fbd
translated_from: content/en/alg/VII/02_s2_torsion_modules_over_a_principal_ideal.md
translation_method: google
source_content_sha256: 798b6543b06067240b5dab1244bfefa178a908e9f4cf2fdc3e29b8faab35c2bc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 6e34b702193043724d519c0bca430eb16897d6f9726fe8b135b802d31d97f97d
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。 挠元模超过主理想整环

### 1. 模超过乘积共环

令$A$为环，$(b_i)_{i \in I}$为$A$的直接分解，即(I，p. 110，Def.7)$A$的双边理想的有限族，使得自然同态从$A$变为$A/b_i$ 的乘积是双射的。由*loc。引用*，第 10 条命题，存在 $A$ 的中心幂等族$(e_i)_{i \in I}$，使得 $b_i = A(1 - e_i)$、$\sum_{i \in I} e_i = 1$ 和 $e_i e_j = 0$ 对于 $i \neq j$。

对于每个左$A$-模块$M$，令$M_i$表示$m \in M$的集合，使得$b_i m = 0$；由于 $b_i$ 是双面理想，因此这是 $M$ 的子模；此外，如果$a, b \in A$和$a - b \in b_i$，则同位$a_{M_i}$和$b_{M_i}$重合；因此，$M_i$上有一个独特的$(A/b_i)$模块结构，从而通过同态$A \to A/b_i$导出$M_i$的$A$模块结构。

#### 命题 1 {#alg-vii-s2-prop-1 .statement tag=0724}

$A$-模块$M$是其子模$M_i$的直和。

让$p_i : M \to M$表示位似$m \mapsto e_i m$； 映射 $p_i$ 是 $A$ 线性，因为 $e_i$ 是中心；由于 $e_i^2 = e_i$、$\sum_{i \in I} e_i = 1$ 和 $e_i e_j = 0$ 对于 $i \neq j$，我们有

$$
p_i \circ p_i = p_i , \quad \sum_{i \in I} p_i = 1_M , \quad p_i \circ p_j = 0 \quad \text{for} \quad i \neq j ,
$$

以及 $p_i$ 形式投影算子的正交族，其和是恒等式（II，p. 209，Def. 7）。由*loc。引用*，第 12 号提案，模 M 是子模 $p_i(M) = e_iM$ 中的直和。在加法$e_iM$被$b_i = A(1 - e_i)$湮灭；如果$i \neq j$和$m \in M$，则$(1 - e_i)e_jm = e_jm$，从而，$e_jM$中没有非零元素被$1 - e_i$湮灭，因此更不必说被$b_i$湮灭。由此可见$e_iM = M_i$、命题得证。

#### 注 1 {#alg-vii-s2-n1-rem-1 .statement tag=0725}

相反，令$M'_i$为每个i的$(A/b_i)$模，并考虑A-模$M'_i$的A-模M、直和；然后用$M'_i$在重合之上构造子模$M_i$（只要注意，如果$i \neq j$，则$M'_j$的非零元素不会被$b_i$消灭，因为$b_i + b_j = A$）。因此，粗略地说，考虑A-模 M 或模的家庭$(M_i)$ 超过环 $A/b_i = A_i$ 相当于同样的事情。

#### 注 2 {#alg-vii-s2-n1-rem-2 .statement tag=0726}

由上式证明，M的投影算子到分量$M_i$是同位。

#### 注 3 {#alg-vii-s2-n1-rem-3 .statement tag=0727}

A-模 M 是循环的当且仅当每个 $M_i$ 都是循环的：如果 $M = Am$，则 $M_i = A_i e_i m$；反之，如果$M_i = A_i m_i$和$m = \sum_{i \in I} m_i$，则$M = Am$；事实上，如果对于每个 i，$n \in M$ 投影到$a_i m_i$，并且对于每个 i，$a \in A$ 与$a_i$ mod $b_i$ 全等，则 am 和 n 在每个 $M_i$ 中具有相同的像，因此重合。

#### 注 4 {#alg-vii-s2-n1-rem-4 .statement tag=0728}

设M和N为两个A-模，其中分量$(M_i)$和$(N_i)$。令$u \in \mathrm{Hom}_A(M, N)$是从M到N的A线性映射；那么对于所有 i 和所有 $m \in M_i$，我们有 $u(m) \in N_i$，所以 u 诱导 $A_i$-线性映射 $u_i \in \mathrm{Hom}_{A_i}(M_i, N_i)$。很容易检查映射 $u \mapsto (u_i)$ 是 Z 模的同构（当 A 是可交换时，分别是 A-模）

$$
\mathrm{Hom}_A(M, N) \to \prod_{i \in I} \mathrm{Hom}_{A_i}(M_i, N_i).
$$

### 2. 挠元模超过主理想整环的规范分解

令 M 为模大于交换环 A。对于每个 $a \in A$，令 $M(\alpha)$ 表示 M 的自同态 $x \mapsto \alpha x$ 的核。如果 $a$ 和 $\beta$ 是 A 的两个元素，使得$\alpha$除$\beta$，那么显然是$M(a) \subset M(\beta)$。特别是，当 n 穿过有理数整数 $\geq 1$ 的集合时，子模 $M(\alpha^n)$ 形式递增序列；因此，$M(\alpha^n)$的并$M$是M的子模，M的元素的由……组成被a的一些幂湮灭。对于 M 的每个子模 N，显然有 $N_1 = N \cap M_a$。

#### 定义 1 {#alg-vii-s2-def-1 .statement tag=0729}

设$\pi$为主理想整环A的不可约元； A-模 M 称为 rr-primary *if*，对于所有 $x \in M$，存在整数 $n \geq 1$ 使得 $\pi^n x = 0$ （在其他字，如果 M 等于子模 $M_\pi$）。

显然，形式$A/(\pi^s)$的每个循环模都是rr-primary。对于任意 A-模 M，子模 $M_\pi$ 是 rr-primary。

#### 引理 1 {#alg-vii-s2-lem-1 .statement tag=072A}

设 M 为模大于主理想整环 A；对于所有$a \in A$使得$a \neq 0$，令$\alpha = \varepsilon \sum_{i=1}^r \pi_i^{n(i)}$是$\alpha$的分解变成不可约因子（VII，p. 4）。被a消灭的M的元素的子模$N = M(a)$是子模$M(\pi_i^{n(i)})$的直和，并且将每个$x \in M(\alpha)$发送到$M(\pi_i^{n(i)})$中其分量的映射有形式 $x \mapsto \gamma_i x \ (\gamma_i \in A)$。而且
$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}
$$
注首先N被a湮灭，因此具有天然的$A/(\alpha)$模结构。根据第4条VII、p. 3、典范同态从$A/(\alpha)$到环$A/(\pi_i^{n(i)})$的乘积为环同构；现在VII、p. 6的应用命题1，我们推导出N是$M(\pi_i^{n(i)})$的直和；这个分解的投影算子是同位，由VII，p. 7，注 2。包含$M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i}$是明显的；相反，让$x \in M(\alpha) \cap M_{\pi_i}$。那么存在 $\pi_i$ 的幂 $\pi_i^s$ 可以消灭 x；我们可以假设$s \geq n(i)$；根据 Bezout 的恒等式，存在 $\lambda, \mu \in A$，从而 $\pi_i^{n(i)} = \lambda \pi_i^s + pa$，因此 $\pi_i^{n(i)} x = 0$，最后$x \in M(\pi_i^{n(i)})$。

#### 引理 2 {#alg-vii-s2-lem-2 .statement tag=072B}

设 M 为整环 A 上的挠元模 (II, p. 313)。对于 M 的元素的每个有限族 $(x_i)_{1 \leq i \leq n}$，A 中存在元素 $\gamma \neq 0$，使得 $x_i$ 所有属于至 $M(\gamma)$。
事实上，对于每个指标 i，A 中都存在元素 $\alpha_i \neq 0$，它会消灭 $x_i$，而元素 $\gamma = \prod_{i=1}^n \alpha_i$ 就符合要求。

#### 定理 1 {#alg-vii-s2-thm-1 .statement tag=072C}

设 M 为挠元模超过主理想整环 A；对于A的每个不可约元$\pi$，令$M_\pi$是元素的M由……组成的子模被$\pi$的一些幂消灭。若P为A的不可约元的代表系统，则M为$\pi \in P$为其子模$M_\pi$的直和。
对于某些 $a \neq 0$，每个元素 $x \in M$ 属于到子模 $M(\alpha)$，因此引理 1 是元素的有限数的和，其中每个属于到一些子模 $M_\pi$。另一方面，如果 $\sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi$，其中 $x_\pi, y_\pi \in M_\pi$ 代表所有 $\pi \in P$，并且几乎所有 $x_\pi$ 和 $y_\pi$ 都是零，则引理 2 表明 A 中存在 $\gamma \neq 0$，使得所有$x_\pi$ 和 $y_\pi$ 属于至相同的子模 $M(\gamma)$； 应用引理 1 到 $M(\gamma)$ 显示 $x_\pi = y_\pi$ 对于所有 $\pi \in P$，从而完成证明。

显然，如果$\pi$和$\pi'$是不可约元的两个关联，则$M_\pi = M_{\pi'}$；因此，对于给定的模 M，子模 $M_\pi$ 仅取决于 A 的理想$(\pi)$；它被称为模 M 的 rr-primary 分量，M 的分解作为 $M_\pi$ 的直和被称为 M 的规范分解作为其 rr-primary 分量的直和。

#### 推出 1 {#alg-vii-s2-thm-1-cor-1 .statement tag=072D}

— *挠元模 M 的每个子模 N 是其子模 N ∩ M 的直和*。

这是因为 N ∩ M, 是 N 的 π 一次分量 N,。

#### 推出 2 {#alg-vii-s2-thm-1-cor-2 .statement tag=072E}

— *挠元 A-模 M 的子模 N 是直因子当且仅当 N 是 M 的直因子，对于 A* 的每个不可约元 π。

事实上，如果 N 和 N' 是 M 的两个子模，则 M = N ⊕ N' 当且仅当 M, − N, ⊕ N'_π 对于 $\mathscr{A}$ 的每个不可约元 π （Cor. 1）。

#### 推出 3 {#alg-vii-s2-thm-1-cor-3 .statement tag=072F}

— *令 N 为挠元 A-模 M 的子模。如果对于 A 的每个不可约元 π，N = 0 或 $(M/N)_\pi = 0$，则 N 为 M* 的直因子。

事实上，条件$(M/N)_\pi = 0$意味着$N_\pi = M_\pi$和Cor。 2 适用。

如果 M 的每个子模都是直因子 (cf. A, VIII, § 3)，A-模 M 称为 *半单*。

#### 推论 4 {#alg-vii-s2-thm-1-cor-4 .statement tag=072G}

— *设 A 为主理想整环，不是域，并设 M 为 A-模。那么 M 是半单当且仅当 M 是挠元模并且对于 A* 的每个不可约元 π，M, = M(π)。

首先假设M是半单；设 x ∈ M 且 π 为 $\mathscr{A}$ 的不可约元。如果N是M中$Annx$的补集，那么我们可以写成$x = \alpha \pi x + y$，还有$\alpha \in \mathscr{A}$和$y \in N$；但这意味着$y = (1 - \alpha n)x$，所以
$$
\pi(1 - \alpha \pi)x \in A\pi x \cap N = 0 .
$$
首先M是挠元模；如果还有$x \in M_\pi$，则$\pi(1 - \alpha \pi)x = 0$，因此$\pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x$是零和$M_\pi = M(\pi)$。

相反，由 Cor. 2 足以证明A-模 M被不可约元 π 湮灭为半单；但这很明显，因为 M 在域 $\mathscr{A}/(\pi)$ 上有一个自然的结构向量空间，而 M 的子模正是在这个结构下的向量子空间。

#### 注 1 {#alg-vii-s2-n2-rem-1 .statement tag=072H}

— 显然，τ 初级模的每个元素 ≠ 0 的湮没子都有形式 $A\pi^k$ (k > 0 整数)，因为它是 τ 的主要理想包含幂。令x为M的元素；对于每个$\pi \in P$，令$x_\pi$为$M_\pi$中x的分量； x 的湮没子是非零的 $x_\pi$ 的湮没子的 lcm，但根据上面的描述，在这种情况下它等于非零的 $x_\pi$ 的湮没子的 *乘积*（VI，p. 16，Prop. 12（DIV））。

#### 命题 2 {#alg-vii-s2-prop-2 .statement tag=072I}

— *如果 M 是在主理想整环 A 上有限生成的挠元模，则 M 的 n 次分量是零，除了其中有限的数，并且 M 的投影算子在这些分量 $M_\pi$ 上是同位*。

这紧随引理 1，因为到引理 2，$\mathscr{A}$中存在$\alpha \neq 0$，使得$M = M(\alpha)$。

#### 注 2 {#alg-vii-s2-n2-rem-2 .statement tag=072J}

— 通过VII、p. 7、注 3，有限生成的挠元A-模是循环的当且仅当其每个π-primary 分量都是循环的。

一个重要的特殊情况，Th。 1和命题2适用于$A = \mathbf{Z}$； $\mathbf{Z}$-模块只是一个 *阿贝尔的群*。如果阿贝尔的群是挠元$\mathbf{Z}$模块，即如果它的所有元素都有*有限的阶*，则阿贝尔的群被称为*挠元群*。那么$P$被取为素数数$> 0$的集合；对于每个素数数 $p > 0$，如果其所有元素都有阶（即 $p$ 的幂），则 (阿贝尔的) 群被称为 $p$ 扭转。在这个术语，Th。图 1 显示*每个挠元阿贝尔的群都是 p 扭转群的直和*。在有限群的情况下，这也是从 I、p. 80、Th 得出的。 4.

### 3. 应用：I。有理数和有理函数的正则分解在一个不定中

#### 定理 2 {#alg-vii-s2-thm-2 .statement tag=072K}

*令$A$为主理想整环，令$K$为其域产物，令$P$为$A$的不可约元的代表系统。 给定元素$x \in K$，$P$、元素$a_0 \in A$和$a, \in A$在$A$（$p \in H$）和整数中存在不可被$p$整除的有限子集$H$，以及整数 $s(p) > 0$ ($p \in H$) 这样*

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

*其中$H$和$s(p)$由这些条件唯一确定。*

*此外，如果$R_p$表示$A$包含中的子集，则$A (p \in P)$中每个剩余类类 mod $p$恰好有一个元素，则每个$x \in K$可以在形式中唯一表达*

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

*其中 $a \in A$ 和 $r_{ph} \in R_p$ 对于所有 $h$ 和 $p$，并且几乎所有 $r_{ph}$ 都是零。*

将 $K$ 视为 $A$ 模块；那么$A$是由1生成的子模。商模$K/A$是由等价关系$x' - x \in A$生成$K$的商，也写成VI、p. 6的记号为$x \equiv x'$（模 1）；让$f$表示从$K$到$M = K/A$的自然同态。

商模 $M$ 是一个 *挠元模*，对于 $M$ 的每一个元素都有形式 $f(a/b)$ ($a \in A, b \in A, b \neq 0$), 从而 $b f(a/b) = f(a) = 0$。因此，Th。 VII、p. 8 中的 1 个适用。设$M_p$($p \in P$)为$M$的元素子模被$p$的幂湮灭；那么$f^{-1}(M_p)$就是形式$a p^{-n}$$K$元素子环$A_p$，其中$a \in A$和$n \geq 0$是整数。 模 $M$ 是 $M_p$ 的直和，因此每个 $x \in K$ 与 $A_p$ 的和模 1 到元素全等；在其他字，公式 (1) 中，$s(p)$ 整数 $> 0$ 和$a$，$A$ 的有限多个元素使得 $a$ 不是倍数 $p$。

我们现在展示这些条件在$s(p)$和$a$上，完全是确定$H$和$s(p)$。事实上，$H$ 是$p \in P$ 的集合，这样$M_p$ 中$f(x)$ 的分量就是$\neq 0$。另一方面，如果$s$和$s'$是两个整数$> 0$，使得 s \geq s' 并且如果$a$和$a'$是$A$的元素不能被$p$整除，这样$ap^{-s} \equiv a'p^{-s'} \pmod{1}$，则推导出$a \equiv a'p^{s-s'} \pmod{p^s}$；如果$s > s'$则$a \equiv 0 \pmod{p}$，与假设相矛盾。这个论证还表明每个 $a_i$ 都是明确定义的 mod $p^{s(p)}$。

为了完成证明，我们首先注意到，在$A$中的每个剩余类类模$p^i$中，存在形式$\sum_{h=0}^{s-1} r_h p^h$的唯一元素，以及$r_h \in R_p$对应$0 \leq h \leq s-1$。事实上，我们在$s$上继续进行归纳（性质是从$R_p$的定义得出$s = 1$）：让$x \in A$； 假设 $x$ mod $p^{s-1}$ 的剩余类类中有形式 $\sum_{h=0}^{s-2} r_h p^h$ ($r_h \in R_p$) 唯一元素；那么$x - \sum_{h=0}^{s-2} r_h p^h$就是$p^{s-1}$的倍数$ap^{s-1}$；现在存在唯一元素 $r_s$，其中 $R_p$ 使得 $a \equiv r_s \pmod{p}$； 从而$x \equiv \sum_{h=0}^{s-1} r_h p^h \pmod{p^s}$。要获得公式 (2)，现在只需将此事实应用于公式 (1) 中的每个 $a_p$ 即可。综上所述，唯一性就很清楚了。

以下是 Th 最重要的应用。 2：

I。 *环 A 是有理数整数的环 Z，并且 K = Q*。令 P 为素数数 > 0 的集合，对于每个$p \in P$，令 $R_p$ 为 $\mathbf{Z}$ 中的区间 $(0, p-1)$。因此我们有规范的分解

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

与 $a \in \mathbf{Z}$、$e_{ph} \in \mathbf{Z}$ 和 $0 \leq e_{ph} \leq p-1$。

II。 *环 A 是交换域 E 上的一个不定多项式的环 E[X]，且 K = E(X)*。令 P 为 $E[X]$ (VII, p. 5) 中的单调不可约多项式的集合。对于$p \in P$，我们可以根据多项式（IV，p. 10）的欧几里得除法，将$R_p$取为严格小于$p$的次数多项式的集合。因此我们有一个有理数函数 $r(X) \in E(X)$ 的分解（称为规范）：

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

其中，对于所有 $p$ 和 $h$，$a(X)$ 是多项式，$v_{ph}(X)$ 是次数严格小于 $p(X)$ 的多项式。特别是，如果域 E 是*代数闭的*，则 $p(X)$ 具有形式 $X - a$ 和 $a \in E$，因此 $v_{ph}(X)$ 是常数。

因此我们可以说向量空间 $E(X)$ 在域 E 上有单项式 $X^n$ ($n \geq 0$ 整数) 的基由……组成以及形式的有理数函数 $X^m / (p(X))^h$，其中$p \in P$、$h$和$m$是整数、$h \geq 1$和$0 \leq rn < \deg(p)$。

### 4. 应用：II。 乘法群 / 单位 / 整数模 a

设a为有理数整数 > 1，且令$(\mathbf{Z}/a\mathbf{Z})^*$为环$\mathbf{Z}/a\mathbf{Z}$的可逆元的乘法群。如果$a = \prod p_i^{n(i)}$是a的分解到素数因子，则环$\mathbf{Z}/a\mathbf{Z}$同构于环$\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$的乘积（VII，p. 3，命题4）并且群$(\mathbf{Z}/a\mathbf{Z})^*$同构于群$(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$的乘积。因此，我们只剩下对群 $(\mathbf{Z}/p^n\mathbf{Z})^*$ 的研究，其中 p 是素数数；回想一下（V，p. 80），$(\mathbf{Z}/p^n\mathbf{Z})^*$的阶$\varphi(p^n)$是$p^n - p^{n-1} = p^{n-1}(p-1)$。

首先假设 $p > 2$； 群的自然同态$\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$限制到同态从$(\mathbf{Z}/p^n\mathbf{Z})^*$到$(\mathbf{Z}/p\mathbf{Z})^*$，其核我们表示U$(p^n)$；由 VII, p. 3, 命题 3 剩余类类 mod $p^n$ of 整数 m 是可逆的当且仅当 m 与 p 互质，即当且仅当剩余类类 of $m$ mod $p$是可逆的。由此可见，U$(p^n)$ 由整数的所有剩余类类 mod $p^n$ 组成，与 1 mod p 全等，因此有 $p^{n-1}$ 元素，并且有正合序列

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

类似地，对于$n \geq 2$，令U$(2^n)$表示自然同态从$(\mathbf{Z}/2^n\mathbf{Z})^*$到$(\mathbf{Z}/4\mathbf{Z})^*$的核；这是阶 $2^{n-2}$ 的群，剩余类类整数的所有由……组成 mod $2^n$ 与 1 mod 4 全等，并且有正合序列

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### 引理 3 {#alg-vii-s2-lem-3 .statement tag=072L}

令x、y、k为整数且$k \geq 0$，并令$p > 2$为素数数。如果$x \equiv 1 + py \mod p^2$则$x^{p^k} \equiv 1 + p^{k+1}y \mod p^{k+2}$。 *如果*$x \equiv 1 + 4y \mod 8$则$x^{2^k} \equiv 1 + 2^{k+2}y \mod 2^{k+3}$。

要证明第一个断言，只需证明，如果$k \geq 1$和$x \equiv 1 + p^ky \mod p^{k+1}$，则$x^p \equiv 1 + p^{k+1}y \mod p^{k+2}$，然后通过归纳对整数 k 进行论证。对于所有$a \in \mathbf{Z}$和$k \geq 1$，直接的
$$
(1 + p^ka)^p \equiv 1 + p^{k+1}a \mod p^{k+2},
$$
因此
$$
(1 + p^ky + p^{k+1}z)^p = (1 + p^k(y + pz))^p \equiv \\
= 1 + p^{k+1}(y + pz) \equiv 1 + p^{k+1}y \mod p^{k+2}.
$$
类似地，对于 $k \geq 1$ 我们有
$$
(1 + 2^{k+1}a)^2 \equiv 1 + 2^{k+2}a \mod 2^{k+3},
$$
所以
$$
(1 + 2^{k+1}y + 2^{k+2}z)^2 \equiv 1 + 2^{k+2}y \mod 2^{k+3},
$$
k 上从而第二个断言 by 归纳。

#### 命题 3 {#alg-vii-s2-prop-3 .statement tag=072M}

令$p > 2$为素数数，令$n > 0$为整数；那么群$U(p^n)$是阶$p^{n-1}$的循环；如果 $n \geq 2$ 则整数 $x$ 的剩余类类 mod $p^n$ 等于 1 mod $p$ 是 $U(p^n)$ 的生成元当且仅当 $x$ 不等于 1 mod $p^2$。设$m > 1$为整数；那么群$U(2^m)$是阶$2^{m-2}$的循环；如果 $m \geq 3$，则整数 $x$ 的剩余类类 mod $2^m$ 与 1 mod 4 全等，是 $U(2^m)$ 的生成元当且仅当$x$ 不等于 1 mod 8。

由于$U(p^n)$有阶$p^{n-1}$，$U(p^n)$的每元素$u$的阶是$p$的幂，$u$是$U(p^n)$的生成元当且仅当$u^{p^{n-2}} \neq 1$。 现在，如果$u$是$x = 1 + py$的类，那么$u^{p^{n-2}}$是$1 + p^{n-1}y$的类，乘以引理3，从而$u$生成$U(p^n)$当且仅当$y \not\equiv 0 \mod p$，其他字$x \not\equiv 1 \mod p^2$。 例如，类$1 + p$生成$U(p^n)$。 类似地，当且仅当$u^{2^{n-3}} \neq 1$时，$x$ mod $2^n$的类$u$生成$U(2^n)$，这意味着根据引理3，$x$不等于1 mod 8；这由$x = 5$满足。

#### 引理 4 {#alg-vii-s2-lem-4 .statement tag=072N}

令$A$为主理想整环，并令$0 \to N \to M \to P \to 0$为$A$模块的正合序列。假设存在互质元素$a, b \in A$使得$aN = 0$和$bP = 0$。然后正合序列分裂的。如果加法、$N$和$P$都是循环的，那么$M$也是循环的。

自 $abM = 0$ 起，模 $M$ 为挠元。第一个断言来自Cor。 3 个VII、p. 9。如果$N$和$P$是循环的，那么它们是有限生成的，因此$M$也是有限生成的（II，p. 17，Cor.5）；由于$M$的每个$p$-primary 分量同构于$N$或$P$的$p$-primary 分量，因此从VII、p. 10的注 2得出， $M$是循环的。

#### 定理 3 {#alg-vii-s2-thm-3 .statement tag=072O}

如果$a = \prod p_i^{n(i)}$是整数$a > 1$的素数分解，则环$\mathbf{Z}/a\mathbf{Z}$的可逆元的群$(\mathbf{Z}/a\mathbf{Z})^*$同构于群的乘积 $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$。如果$p > 2$是素数数且$n \geq 1$整数，则群$(\mathbf{Z}/p^n\mathbf{Z})^*$是阶$p^n \ ^1(p - 1)$的循环。 群 $(\mathbf{Z}/2\mathbf{Z})^*$ 是微不足道的；对于 $n \geq 2$ 群 $(\mathbf{Z}/2^n\mathbf{Z})^*$ 是由 5 mod $2^n$ 的剩余类类生成的阶 $2^n \ ^2$ 的循环群的直接乘积和循环阶 2 的群剩余类类 1 的由……组成以及$-1$ mod $2^n$。

$U(p^n)$的阶$p^n \ ^1$和$(\mathbf{Z}/p\mathbf{Z})^*$的$p - 1$互质；由于 $U(p^n)$ 和 $(\mathbf{Z}/p\mathbf{Z})^*$ 是循环的（命题 3 和 V、p. 78、引理 1），群 $(\mathbf{Z}/p^n\mathbf{Z})^*$ 是循环的（将引理 4 应用于正合序列 (3)）。如果$n \geq 2$则同态$v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^*$到子群$(1, -1)$的限制是双射；因此，群$(\mathbf{Z}/2^n\mathbf{Z})^*$是子群的直接乘积和$v$的核$U(2^n)$；结果由命题 3 得出。

#### 注 {#alg-vii-s2-n4-rem-1 .statement tag=072P}

设 $p > 2$ 为素数数，并令 $x$ 为整数全等于 1 mod $p$，且不等于 1 mod $p^2$；有正合序列

$$
\{0\} \to \mathbf{Z}/p^n \ ^1\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{\nu} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

群，其中$v$是自然的投影，而$u$是由映射$r \mapsto x^r$在商上诱发的。令 $\mathbf{Z}_p$ 为 $p$-adic 整数 ($V$, p. 96) 的环，并令 $x$ 为 $\mathbf{Z}_p$ 的元素，使得 $x - 1 \in p\mathbf{Z}_p$ 和$x - 1 \notin p^2\mathbf{Z}_p$； 经过至逆极限、正合序列 (5) 诱导正合序列

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

其中$v$是自然映射，连续映射$u$扩展映射$n \mapsto x^n$（$n \in \mathbf{Z}$）。我们经常把$x^n = u(x)$代替$n \in \mathbf{Z}_p$。

类似地，如果$x \in \mathbf{Z}_2$与$x - 1 \in 4\mathbf{Z}$和$x - 1 \notin 8\mathbf{Z}_2$，则有分裂正合序列

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

其中 $u$ 是映射 $n \mapsto x^n$ 的连续扩张

### 习题 {#alg-vii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
