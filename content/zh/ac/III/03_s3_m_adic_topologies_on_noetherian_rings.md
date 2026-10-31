---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 3
section_title: m-adic topologies on Noetherian rings
lang: zh
source: ac-i-vii
book_pages: 195-209, 245-255
pdf_pages: 0215-0229, 0265-0275
extraction: ocr
subsections:
    - "no": 1
      title: GOOD FILTRATIONS
      page: 195
      pdf_page: 215
    - "no": 2
      title: m-ADIC TOPOLOGIES ON NOETHERIAN RINGS
      page: 199
      pdf_page: 219
    - "no": 3
      title: ZARISKI RINGS
      page: 201
      pdf_page: 221
    - "no": 4
      title: THE HAUSDORFF COMPLETION OF A NOETHERIAN RING
      page: 202
      pdf_page: 222
    - "no": 5
      title: THE COMPLETION OF A ZARISKI RING
      page: 206
      pdf_page: 226
statements: 39
exercises: 27
content_sha256: aea5c3b5594657803e0e9f7b31beec863ad4eefa268a938e274f5adfe1277637
translated_from: content/en/ac/III/03_s3_m_adic_topologies_on_noetherian_rings.md
translation_method: google
source_content_sha256: e4eba8899949967667773f570b755a00419ebfdad78b7c56f68274079332363d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9c9ccda1c4a552673d6bdfe9e2b2f3a9be601166ea8f38f54246c2e7b50e5008
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 3. 诺特环上的$\mathfrak{m}$-adic 拓扑

假设本段中考虑的所有过滤都是详尽的。

### 1. 良好的过滤

令$\mathbf{A}$为过滤后的交换环，E为过滤后的$\mathbf{A}$模块，$(\mathbf{A}_n)$和$(E_n)$

$A$和$E$各自的过滤；假设$A_0 = A$。在多项式环 $A[X]$ 集合 $A' = \sum_{n \geq 0} A_n X^n$ 中是型 $\mathbf{N}$*的*分级亚A代数； $E \otimes_A A[X]$的子群$E' = \sum_{n \geq 0} E_n \otimes_A A X^n$是型$\mathbf{N}$的*分级$A'$模块*，因为
$$
A_m X^m (E_n \otimes_A A X^n) \subset (A_m E_n \otimes_A A X^n",") \subset E_{m+n} \otimes_A A X^{m+n}.
$$

#### 定义 1 {#ac-iii-s3-def-1 .statement tag=04FX}

*令$A$为交换环，$m$为$A$的理想，$E$为$A$模，$(E_n)$为子模的加法群$E$由……组成的过滤$E$。过滤 $(E_n)$ 被称为 m-good 如果：*
(1) $m E_n \subset E_{n+1}$ 对于所有 $n \in \mathbf{Z}$；
(2) *存在整数$n_0$使得*$m E_n = E_{n+1}$*对于*$n \geq n_0$。

然后$q$乘归纳，$m^q E_n = E_{n+q}$乘$n \geq n_0, q \geq 1$。 注条件 (1) 意味着如果$A$ 被赋予$m$-adic 过滤，则$(E_n)$ 过滤与$E$ 上的$A$ 模块结构兼容。显然，在每个$A$-模块$E$上，$m$-adic 过滤都是良好的。如果 $A$-模块 $E$ 上的过滤是 m-good，则 $E$ 的任何商模上的商过滤是 m-good。

#### 定理 1 {#ac-iii-s3-thm-1 .statement tag=04FY}

*令$A$为交换环，$m$为$A$的理想，$E$为$A$模块，$(E_n)$为无限生成的子$A$模块的加法群$E$由……组成的过滤。假设 $m E_n \subset E_{n+1}$ 代表所有 $n$。令$A'$为$A[X]$的分级子代数$\sum_{n \geq 0} m^n X^n$，$E'$为$A'$-模块$\sum_{n \geq 0} E_n \otimes_A A X^n$的分级。以下两个条件是等效的：*
(a) *过滤* $(E_n)$ *很好。*
(b) *$E'$是有限生成的$A'$模块。*

假设 $m E_{n-1} = E_n$ 对应 $n > n_0 \geq 0$。对于$i \leq n_0$，令$(e_i)_{i \leq n_0}$为$A$模$E_i$的生成元的有限系统。由于$A$-模块$E_n \otimes_A A X^n$是由元素$e_{n,j} \otimes X^n$为$0 \leq n \leq n_0$生成的，并且等于
$$
m^{n-n_0} E_{n_0} \otimes_A A X^n
$$
对于$n > n_0$，$A'$-模块$E'$由元素$e_{n,j} \otimes X^n$生成，对于$0 \leq n \leq n_0$和$1 \leq j \leq r_n$；那么它肯定是有限生成的。

相反，如果$E'$是有限生成的$A'$模块，则它是由形式$e_k \otimes X^{n(k)}$的元素有限族生成的，其中$e_k \in E_{n(k)}$。设$n_0$为整数$n(k)$中的最大的。然后对于 $n \geq n_0$ 和 $f \in E_n$，
$$
f \otimes X^n = \sum_k t_k (e_k \otimes X^{n(k)})
$$
其中$t_k \in A'$； 替换如果需要为$t$，则根据其齐次分量次数$n - n(k)$，我们可以假设为$t_k = a_k X^{n-n(k)}$，其中$a_k \in m^{n-n(k)}$。

如唯一元素 $X^n$ 形式基 of A-模 AX”，等式$f \otimes X^n = \left( \sum_k a_k e_k \right) \otimes X^n$蕴涵$f = \sum_k a_k e_k$。则$E_n \subset m^{n-n_0} E_{n_0}$；由于相反包含是明显的，

$$
E_n = m^{n-n_0} E_{n_0},
$$

从而 $E_n = m E_{n-1}$ $n > n_0$。

#### 引理 1 {#ac-iii-s3-lem-1 .statement tag=04FZ}

*设 A 为交换律诺特环，且 m 为 A 的理想。则 $A[X]$ 的子环 $A' = \sum_{n \geq 0} m^n X^n$ 为诺特。*

$A'$是$mX$生成的A-代数；因为A是诺特，$mX$是有限生成A-模，然后从§ 2, no. 10、推论3到定理2得出结论。

#### 命题 1 {#ac-iii-s3-prop-1 .statement tag=04G0}

*设 A 为交换律诺特环，m 为 A 的理想；令 A 接受 m-adic 过滤。令E、F为与过滤兼容的两个过滤的A-模和$j : F \to E$单同态。如果 E 是有限生成的且其过滤是 m-good，则 F 是有限生成的且其过滤是 m-good。*

由于 F 与 E 的子模同构，因此它是有限生成的，因为 A 是诺特并且 E 是有限生成的。令$(E_n)$、$(F_n)$分别为E和F上的过滤，由有限生成的子模组成；保留引理 1 中的记号，我们集合 $E' = \sum_{n \geq 0} E_n \otimes_A A X^n, F' = \sum F_n \otimes_A A X^n$；由于假设$F_n$同构于$E_n$的子模，我们看到F'同构于$E'$的子模。通过定理 1，$E'$ 是有限生成的 $A'$ 模，因此 F' 也是如此，因为 A' 是诺特 (引理 1)。因此根据定理 1 得出结论。

#### 推出 1（Artin-Rees 引理）{#ac-iii-s3-prop-1-cor-1 .statement tag=04G1}

*设 A 为可交换诺特环，m 是 A 的理想，E 有限生成A-模和 E 的 F 子模。E 上的 m-adic 过滤在 F 上引起的过滤是 m-good。*

在其他字中，存在整数$n_0$使得

$$
m((m^n E) \cap F) = (m^{n+1} E) \cap F
$$

对于所有$n \geq n_0$。

#### 推出 2 {#ac-iii-s3-prop-1-cor-2 .statement tag=04G2}

*设 A 为可交换的诺特环且 a, b 是 A 的两个理想。存在整数 h > 0 使得 $a^h \cap b \subset ab$。*

存在 n，使得推论 1 的 $a^{n+1} \cap b = a(a^n \cap b) \subset ab$ 应用于$E = A, F = b$。

#### 推出 3 {#ac-iii-s3-prop-1-cor-3 .statement tag=04G3}

*设 A 是可交换的诺特环，m 是 A 的理想，并且 x 元素是 $A$，它不是 $O$ 的除子。存在整数$k > 0$，对于所有$n \geq k$，关系$xy \in m^n$意味着$y \in m^{n-k}$。

推出 1 应用于 $E = A, F = A x$ 表明存在 $k$，使得对于所有 $n \geq k$，$m^n \cap Ax = m^{n-k}(m^k \cap Ax)$。那么，如果$xy \in m^n$，

$$
xy \in m^n \cap Ax \subset m^{n-k}x
$$

并且，由于$x$不是$0$的除子，我们推断出$y \in m^{n-k}$。

在运输者的记号（章I, § 2, no. 10）中，推论3的结论为

(2)
$$
m^n : Ax \subset m^{n-k}.
$$

#### 推出 4 {#ac-iii-s3-prop-1-cor-4 .statement tag=04G4}

令 $A$ 为可交换的诺特环，$m$ $A$、$E$ 的理想，分别生成 $A$ 模以及 $(E_n)$ 和 $(E'_n)$ 两个过滤由……组成子模 $E$。假设当$A$被给予$m$-adic过滤时，过滤$(E_n)$和$(E'_n)$与$E$上的$A$模块结构兼容。如果过滤 $(E_n)$ 为 $m$-良好，并且对于所有 $n \in \mathbf{Z}$ 为 $E'_n \subset E_n$，则过滤 $(E'_n)$ 为 $m$-良好。
这是命题 1 的特例。

#### 引理 2 {#ac-iii-s3-lem-2 .statement tag=04G5}

令$A, B$为两个可交换的诺特环、$\phi : A \to B$环同态、$E$有限生成的$A$模块和$F$有限生成的$B$模块。那么$\mathrm{Hom}_A(E, \phi_*(F))$是一个有限生成的$B$-模块。

假设存在满射$A$同态$v : A^n \to E$；因此，$\mathrm{Hom}_A(E, \phi_*(F))$到$\mathrm{Hom}_A(A^n, \phi_*(F))$的映射$u \mapsto u \circ v$是单射的，并且由于$B$是诺特，因此足以证明$\mathrm{Hom}_A(A^n, \phi_*(F))$是有限生成的$B$模；这是直接的，因为它与$F^n$同构的。

#### 命题 2 {#ac-iii-s3-prop-2 .statement tag=04G6}

令$A$是可交换的诺特环，$m$是$A$和$E, F$两个有限生成的$A$模的理想。如果$(F_n)$是$F$上的$m$-良好过滤，则子模$\mathrm{Hom}_A(E, F_n)$形式是$A$-模块$\mathrm{Hom}_A(E, F)$上的$m$-良好过滤。
正如 $m^k F_n \subset F_{n+k}$ 与 $n \in \mathbf{Z}, k \geq 0$ 一样，也成立

$$
m^k \mathrm{Hom}_A(E, F_n) \subset \mathrm{Hom}_A(E, F_{n+k});
$$

然后，该系列$(\mathrm{Hom}_A(E, F_n))_{n \in \mathbf{Z}}$是$\mathrm{Hom}_A(E, F)$上的过滤，与其模结构兼容，超过环$A$由$m$adic过滤过滤。由于$E$是有限生成的，因此存在整数$r > 0$和一个满射$A$同态$u : A^r \to E$，其中定义一个单射$A$同态

$$
v = \mathrm{Hom}(u, 1_F) : \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_A(A^r, F);
$$

显然 $v$ 与过滤$(\mathrm{Hom}_A(E, F_n))$ 和 $(\mathrm{Hom}_A(A^r, F_n))$ 相容的。
由于$\mathrm{Hom}_A(E, F)$和$\mathrm{Hom}_A(A^r, F)$是有限生成的（引理2），因此凭借命题1就足以表明过滤$(\mathrm{Hom}_A(A^r, F))$是m-good；但这是直接的，因为典范同构$\mathrm{Hom}_A(A^r, F_r) \to F_n^r$的存在以及关系$mF_n = F_n +$的事实，意味着$m(F_n^r) = (mF_n)^r = F_{n+1}^r$（代数，章II, § 3, no. 7，注）。

#### 命题 3 {#ac-iii-s3-prop-3 .statement tag=04G7}

*令 $A$ 为诺特环，且 $m$ 为 $A$ 的理想，使得 $A$ 为 Hausdorff，并且相对于 m 进数拓扑而言是完整的。令$E$为过滤环$A$上的过滤$A$模，$A$的过滤$(E_n)$使得$E_0 = E$和$E$是相对于由$(E_n)$定义的拓扑的Hausdorff。那么下面的条件是等价的：
(a) $E$ 是有限生成的 $A$ 模块，$(E_n)$ 是 m-good 过滤。
(b) $\mathrm{gr}(E)$ 是有限生成的 $\mathrm{gr}(A)$ 模块。
(c) 对于所有$n \geq 0$，$\mathrm{gr}_n(E)$是有限生成的$A$模块，并且存在$n_0$，使得对于$n \geq n_0$典范同态
$$
\mathrm{gr}_1(A) \otimes_A \mathrm{gr}_n(E) \to \mathrm{gr}_{n+1}(E)
$$
是满射的。*

从定义可以立即得出 (a) 蕴涵 (c)。 (b) 蕴含 (c) 的事实是 § 1, no. 3、引理 1 中的推论；相反，如果 (c) 成立，显然 $\mathrm{gr}(E)$ 是由 $p \leq n_0$ 的 $\mathrm{gr}_p(E)$ 的和生成为 $\mathrm{gr}(A)$ 模，因此假设承认生成元的有限系统。仍有待证明(c)蕴涵(a)；因为$\mathrm{gr}_n(E)$是有限生成的，$E_n = E$，显然首先是由归纳在$n$上生成的，$E/E_n$是所有$n$的有限生成的$A$模块；因此，足以证明，对于$n > n_0$，$E_n$是有限生成的$A$模块，并且$mE_n = E_{n+1}$。现在，考虑具有详尽和分离过滤$(E_{n+k})(k \geq 1)$的$A$模块$E_{n+1}$； $mE_n \subset E_{n+1}$； 假设 (c) 意味着$\mathrm{gr}_{n+1}(E) = E_{n+1}/E_{n+2}$中$mE_n$的像等于$\mathrm{gr}_{n+1}(E)$和生成分级的$\mathrm{gr}(A)$模$\mathrm{gr}(E_{n+1})$。由于 $\mathrm{gr}_{n+1}(E)$ 是由假设有限生成的 $A$ 模块，因此从 § 2, no. 9、命题 12 可以得出 $mE_n = E_{n+1}$ 和 $E_{n+1}$ 是有限生成的 $A$ 模块。

### 2. 诺特环上的 m-ADIC 拓扑

#### 命题 4 {#ac-iii-s3-prop-4 .statement tag=04G8}

*设$A$是可交换的诺特环，$m$是$A$的理想，$E$是有限生成的$A$模。 $E$ 定义上的所有 m-good 过滤均相同拓扑（即 m-adic 拓扑）。*

令 $(E_n)$ 为$E$ 上的 m-good 过滤。由于这种过滤是详尽的，$E$属于的每个元素到$E_n$之一，并且由于$E$是有限生成的并且$E_n$是$A$模块，因此存在整数$n_1$使得$E_{n_1} = E$。另一方面，令 $n_0$ 使得 $mE_n = E_{n+1}$ 对于$n \geq n_0$；那么，对于$n > n_0 - n_1$，
$m^n E \subset E_{n+n_1} = m^{n+n_1-n_0} E_{n_0} \subset m^{n+n_1-n_0} E$，证明命题。

#### 定理 2（克鲁尔）{#ac-iii-s3-thm-2 .statement tag=04G9}

*设$A$是可交换的诺特环，$m$是$A$的理想，$E$是有限生成的$A$模，$F$子模是$E$。然后$F$上的$m$-adic 拓扑由$E$上的$m$-adic 拓扑诱导。

从no. 1、命题 1 可以看出，$E$ 上的$m$-adic 过滤在$F$ 上引起的过滤是m-good，然后从命题 4 得出结论。

#### 推论 {#ac-iii-s3-n2-cor-1 .statement tag=04GA}

*令$A$是可交换的诺特环，$m$是$A$的理想，$E$是$A$模，$F$是有限生成的$A$模。每个$A$-线性映射$u : E \to F$都是严格的态射*（一般拓扑、章 111、§ 2, no. 8）*对于$m$-adic拓扑*。

由于$u(m^nE) = m^n u(E)$，$u$是$E$到$u(E)$的严格态射，对于这两个模上的$m$-adic拓扑，以及$u(E)$上的$m$-adic拓扑由$m$-adic 拓扑于 $F$ 定理 2。

#### 命题 5 {#ac-iii-s3-prop-5 .statement tag=04GB}

*设$A$是可交换的诺特环，$m$是$A$的理想，$E$是有限生成的$A$模。 $E$*中$\{0\}$的闭包*$\bigcap_{n=1}^m m^nE$*相对于$m$-adic拓扑是$x \in E$的集合，其中存在元素$m \in m$使得*$(1 - m)x = 0$。

如果$x = mx$，其中$m \in m$，$x = m^n x \in m^nE$对于每个整数$n \geq 0$，因此$x \in F = \bigcap_{n=0}^m m^nE$。 Conversely, if $x \in F$, $Ax$ is contained in the intersection of the neighbourhoods of 0 in $E$; it then follows from Theorem 2 that the $m$-adic topology on $Ax$, which is induced by that on $E$, is the coarsest topology; as $mx$ is by definition a neighbourhood of 0 with this topology, $mx = Ax$ and hence there exists $m \in m$ such that $x = mx$.

我们也可以说 $mF = F$ 因为
$$
F = \bigcap_{n=1}^\infty m^{n+1}E \subset m. \bigcap_{n=1}^\infty m^nE = mF;
$$
由于$A$是诺特，$F$是有限生成的$A$模块；那么应用章II, § 2, no. 2、推论3到命题4就足够了。

#### 推论（克鲁尔）{#ac-iii-s3-n2-cor-2 .statement tag=04GC}

*设$A$是可交换的诺特环，而$m$是$A$的理想。 理想的* $\bigcap_{n=1}^m m^n$ *是元素* $x \in A$ *的集合，其中存在* $m \in m$ *使得* $(1 - m)x = 0$。 *In particular, for* $\bigcap_{n=1}^\infty m^n = \{0\}$, *it is necessary and sufficient that no element of* $1 + m$ *be a divisor of* $0$ *in* $A$.

应用命题5到$E = A$就足够了。

#### 注 {#ac-iii-s3-n2-rem-1 .statement tag=04GD}

假设 $A$ 是 *诺特* 在此推论中至关重要。对于例，令$A$为映射从$\mathbf{R}$对其自身无限微分的环，并令$m$为函数$f$的$A$由……组成的（极大）理想，使得$f(0) = 0$。 $\bigcap_{n=0}^\infty m^n$是函数$f$的集合是直接的，使得$f^{(n)}(0) = 0$对于所有$n \geq 0$并且存在这样的函数与$f(x) \neq 0$，对于所有$x \neq 0$，对于例函数 $f$ 由 $f(x) = e^{-1/x^2}$ 定义为 $x \neq 0$ 和 $f(0) = 0$。

#### 定义 1 {#ac-iii-s3-def-1-bis .statement tag=04GE}

*设$\mathbf{A}$为拓扑环。如果$\mathbf{A}$的双边理想$m$使得$\mathbf{A}$上的给定拓扑是$m$进数拓扑，则$m$称为定义理想&$\mathbf{A}$上的拓扑。*

令$A$为交换律诺特环，$m$为$A$的理想，$t$其根式（章II, § 2, no. 6）。如果$m'$是$m$-adic拓扑的定义理想，则存在整数$n > 0$，使得${m'}^n \subset m$（$§ 2$，no. 5），因此$m' \subset t$；相反，由于$A$是诺特，因此存在整数$k > 0$使得$t^k \subset m$（章II, § 2, no. 6，命题15），因此$t$是*最大的定义理想* $m$-adic 拓扑。

### 3.扎里斯基环

#### 命题 6 {#ac-iii-s3-prop-6 .statement tag=04GF}

*令$A$为可交换的诺特环，且$m$为$A$的理想。以下属性是等效的：
(a) $m$ 包含在$A$ 的雅各布森根中。
(b) *每个有限生成的 $A$-模都是具有 $m$-adic 拓扑的 Hausdorff。*
(c) *对于每个有限生成的$A$-模块$E$，$E$的每个子模相对于$E$上的$m$-adic 拓扑都是封闭的。*
(d) *$A$ 的每个最大理想相对于 $m$-adic 拓扑都是封闭的。*

让我们证明 (a) 蕴涵 (b)。假设$m$包含在$A$的雅各布森根式中，并令$E$为有限生成的$A$模。如果$x \in E$和$m \in m$使得$(1 - m)x = 0$，则$x = 0$，因为$1 - m$在$A$中是可逆的。那么 (no. 2, 命题 5) $E$ 就是 Hausdorff 和 $m$-adic 拓扑。

让我们证明（b）蕴涵（c）。假设(b)成立。令 $E$ 为有限生成的 $A$ 模块，并且 $F$ 子模为 $E$。那么$E/F$是带有$m$-adic 拓扑的Hausdorff，它是$m$-adic 拓扑在$E$上的商拓扑；那么 $F$ 在 $E$ 关闭。

显然（c）意味着（d）。最后让我们证明（d）蕴涵（a）。从(d)可知，对于$A$的每个最大理想$a$，$A$-模$A/a$是具有$m$进数拓扑的Hausdorff。这意味着$m(A/a) \neq A/a$、除非、$A/a$上的$m$-adic 拓扑是最粗糙的拓扑和$A/a$减少到0，这是荒谬的，因为$A/a$是*ajield*。因此，$A/a$中$m$的典范像是与$A/a$不同的$A/a$的理想，因此减少到0；然后$m \subset a$，证明$m$包含在$A$的雅各布森根式中。

#### 定义 2 {#ac-iii-s3-def-2 .statement tag=04GG}

*拓扑环 $A$ 被称为 Zariski 环，如果它是可交换的且诺特，并且在 $A$ 满足上存在拓扑的定义理想 $m$，相当于命题的条件 6.*

Zariski 环 $A$ 必然是 *Hausdorff* (命题 6)，并且其拓扑的*每个*定义理想都包含在 $A$ 的雅各布森根中。

*扎里斯基的例环*

#### 例 1 {#ac-iii-s3-n3-exa-1 .statement tag=04GH}

令$A$是可交换的诺特环，而$m$是$A$的理想。如果 $A$ 是 *Hausdorff 并与 m-adic 拓扑* 完备的，则$A$ 是一个 Zariski 环与此拓扑，凭借 § 2, no. 13、引理 3。

#### 例 2 {#ac-iii-s3-n3-exa-2 .statement tag=04GI}

Zariski 环的每个 *商环* $A/b$ 都是 Zariski 环，因为它是诺特，并且，如果 $m$ 是 $A$ 的定义理想，则 $m(A/b) = (m + b)/b$ 包含在 $A/b$ 的雅各布森根中（*代数*、章VIII, § 6, no. 3、命题7）。

#### 例 3 {#ac-iii-s3-n3-exa-3 .statement tag=04GJ}

令 $A$ 为 *诺特半局部* 环，$r$ 为其雅各布森根式。那么 $A$ 与 $r$-adic 拓扑是 Zariski 环。当我们将诺特半局部环视为拓扑环时，这始终是拓扑的问题（除非另有说明）。

#### 命题 7 {#ac-iii-s3-prop-7 .statement tag=04GK}

*令$A, A'$为两个交换环和$h : A \to A'$环同态。假设 $A$ 是诺特并且 $A'$ 是有限生成的 $A$ 模块（结构由 $h$ 定义）。令$m$为$A$的理想，并令$m' = mA'$。然后：*

(i) *要使$A'$上的$m'$进数拓扑成为Hausdorff，$1 + h(m)$的元素不是$A'$中的$0$的除子是必要且充分的。*

(ii) *如果 $A$ 与 $m$-adic 拓扑是 Zariski 环，则 $A'$ 与 $m'$-adic 拓扑是 Zariski 环。*

(iii) *If $h$ is injective (thus identifying $A$ with a subring of $A'$), the $m'$-adic topology on $A'$ induces on $A$ the $m$-adic topology.*

回想一下，$A'$ 重合上的$m'$-adic 过滤和*A-模* $A'$ 上的$m$-adic 过滤（§ 2, no. 1，*例 3*）。因此，断言 (i) 是no. 2 的命题 5 的特例，而断言 (iii) 是no. 2 的定理 2 的特例。最后让我们展示(ii)。假设 $A$ 是具有 $m$-adic 拓扑的 Zariski 环，并令 $E'$ 为有限生成的 $A'$-模；它也是有限生成的$A$-模块以及$E'$重合上的$m$-adic和$m'$-adic过滤；那么$E'$是带有$m'$进数拓扑的Hausdorff。最后，$A$-模块$A'$是诺特，因此环$A'$是诺特，这完成了证明，$A'$是Zariski环。

### 4. 诺特环的豪斯多夫补全

令$A$为交换环，$m$为$A$的理想，$E$为$A$模；让$\hat{A}$和$\hat{E}$分别表示$A$和$E$相对于$m$进数拓扑和$j_E$典范映射$E \to \hat{E}$的豪斯多夫完成。 $\hat{A} \times E$到$\hat{E}$定义的$A$双线性映射$(a, x) \mapsto aj_E(x)$和$A$线性映射

$$
\alpha_E : \hat{A} \otimes_A E \to \hat{E},
$$

称为*规范*。令$u : E \to F$为$A$模同态，令$\hat{u} : E \to \hat{F}$为由经过完成Hausdorff完成而获得的映射；对于$a \in \hat{A}$，$x \in E$，

$$
\alpha_F(a \otimes u(x)) = aj_F(u(x)) = a\hat{u}(j_E(x)) = \hat{u}(\alpha_E(a \otimes x)),
$$

其他字、图表

$$
\begin{array}{ccc}
\hat{A} \otimes_A E & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A F \\
\downarrow \alpha_E & & \downarrow \alpha_F \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{F}
\end{array}
$$

是可交换的。最后，从 § 2, no. 12, 命题 16 可以得出，如果 E 是有限生成的，则同态 $\alpha_E$ 是满射的。

#### 定理 3 {#ac-iii-s3-thm-3 .statement tag=04GL}

*设A是可交换的诺特环，m是A和E、F、G三个有限生成A模的理想。然后：*

(i) *如果* $E \xrightarrow{u} F \xrightarrow{v} G$ *是 A-线性映射的正合序列，序列* $\hat{E} \xrightarrow{\hat{u}} \hat{F} \xrightarrow{\hat{v}} \hat{G}$ *由经过获得的 Hausdorff 完备的（相对于 m-adic 拓扑）是准确的。*

(ii) *规范 A-线性映射* $\alpha_E : \hat{A} \otimes_A E \to \hat{E}$ *是双射的。*

(iii) *A-模* $\hat{A}$ *平坦。*

我们已经看到，$u$和$v$是拓扑群严格的态射（no. 2，定理2的推论）。 断言 (i) 然后从 § 2, no. 12, 引理 2 得出。当 $E = A$ 时，断言 (ii) 是明显的，并且 E 是自由有限生成A-模的情况可以立即简化为该情况。在一般情况下，E 承认有限表示

$$
L \xrightarrow{u} L' \xrightarrow{v} E \longrightarrow 0
$$

（章I, § 2, no. 8，引理8）。我们推导出可交换的图表

$$
\begin{array}{ccccccccc}
\hat{A} \otimes_A L & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A L' & \xrightarrow{1 \otimes v} & \hat{A} \otimes_A E & \longrightarrow & 0 \\
\downarrow \alpha_L & & \downarrow \alpha_{L'} & & \downarrow \alpha_E \\
\hat{L} & \longrightarrow & \hat{L}' & \longrightarrow & \hat{E} & \longrightarrow &
\end{array}
$$

第一行是精确的 (章 I, § 2, no. 1, 引理 1)，第二行 (i) 也是如此。我们已经知道 $\alpha_E$ 是满射 (§ 2, no. 12, 命题 16)；另一方面，由于 $\alpha_L$ 和 $\alpha_{L'}$ 是双射，$1 \otimes v$ 是满射，$\alpha_E$ 凭借章 I, § 1, no. 4 是单射的，推论 2 到命题 2；这表明 (ii)。

然后从(i)和(ii)得出，如果$a$是A的理想（必然是有限生成的），则典范映射$\hat{A} \otimes_A a \to \hat{A}$是单射的，是$\hat{a} \to \hat{A}$和$\alpha_E$的合成，这证明$\hat{A}$是平的$A$模（章I, § 2, no. 3，命题1）。

在定理 3 的条件下，$\hat{A} \otimes_A E$通常通过典范映射$\alpha_E$与$E$识别。如果 $u : E \to F$ 是有限生成的 $A$ 模块中的同态，则$\hat{u} : E \to \hat{F}$ 则凭借图表的交换律与 $1 @ u$ 进行识别 (4)。

#### 推论 1 {#ac-iii-s3-thm-3-cor-1 .statement tag=04GM}

设$A$是可交换的诺特环，$m$是$A$的理想，$E$是有限生成的$A$模，$F$和$G$两个子模 $E$。让$A, E, F, G$被赋予$m$-adic拓扑，并让$i$从$E$到$e$为典范映射。然后：

$$
\hat{F} = \hat{A}.i(F), \quad (F + G)^{\wedge} = \hat{F} + \hat{G}, \quad (F \cap G)^{\wedge} = \hat{F} \cap \hat{G},
$$
$$
(F : G)^{\wedge} = \hat{F} : \hat{G}.
$$

此外，如果$a$和$b$是$A$和$c = ab, \hat{c} = \hat{a}\hat{b}$的两个理想。

到定理 3，$\hat{E}, \hat{F}, \hat{G}$ 被规范地标识为 $\hat{A} \otimes_A E, \hat{A} \otimes_A F, \hat{A} \otimes_A G$，从而建立了前两个公式。第三个和第四个分别是章I, § 2, no. 6、命题6和no. 10、命题12。最后，如$\hat{a} = \hat{A}i(a), \hat{b} = \hat{A}i(b), \hat{c} = \hat{A}i(c)$，
$$
\hat{c} = \hat{A}i(ab) = \hat{A}i(a)i(b) = \hat{a}\hat{b}.
$$

#### 推论 2 {#ac-iii-s3-thm-3-cor-2 .statement tag=04GN}

令 $A$ 为交换诺特环，$m$ $A$ 的理想，$\hat{A}$ $A$ 相对于 $m$-adic 拓扑的豪斯多夫完成。如果元素$a \in A$不是$A$中的0的除子，则$\hat{A}$中的典范像$a'$也不是$\hat{A}$中的0的除子。

由于 $\hat{A}$ 是扁平 $A$ 模，因此推论是章 I, § 2, no. 4、命题 3 (i) 的特例。

#### 推论 3 {#ac-iii-s3-thm-3-cor-3 .statement tag=04GO}

如果$A$是可交换的诺特环，则形式幂级数$A[[X_1, \ldots, X_n]]$的环是平$A$模。

多项式环的完成
$$
B = A[X_1, \ldots, X_n]
$$
对于$m$-adic 拓扑，其中$m$是没有常数项的多项式的集合（$§ 2,$no. 12，例1）；因为 $B$ 是诺特（$§ 2,$ no. 10，推论 2 到定理 2），$A[[X_1, \ldots, X_n]]$ 是定理 3 的扁平 $B$ 模，并且，因为 $B$ 是免费的 $A$ 模， $A[[X_1, \ldots, X_n]]$ 是扁平 $A$ 模（章 I, § 2, no. 7，推论 3 到命题 8）。

#### 命题 8 {#ac-iii-s3-prop-8 .statement tag=04GP}

令 $A$ 为交换诺特环，$m$ $A$，$\hat{A}$ $A$ 相对于 $m$-adic 拓扑和 $j$ 的豪斯多夫完成式典范映射从$A$到$\hat{A}$。的：
(i) $\hat{A}$ 是 Zariski 环，$\hat{m} = \hat{A}.j(m)$ 是 $\hat{A}$ 的定义理想。

(ii) *映射* $n \mapsto A = \hat{A}.j(n)$ *是* $A$ *包含* 最大理想集合双射* $m$ *到* $\hat{A}$ *最大理想集合和* $q \mapsto j^{-1}(q)$ *是逆双射*。

(iii) *设*$n$*为*$A$*包含*$m$的最大理想。 *同态* $j': A_n \to \hat{A}_{\hat{n}}$ *源自* $j$ *是单射；如果* $A$，*通过* $j$ *与* $\hat{A}$的子环进行识别，** $(nA_n)$*-adic 拓扑 on* $A_n$ *由* $A$*-adic 拓扑 on*诱导$\hat{A}_{\hat{n}}$ *和* $A_n$ *密集于* $A$，*与* $A$*-adic 拓扑*。

让我们展示（i）。由于$m$是有限生成的理想，$(m^n)^{\wedge} = (\hat{m})^n = m^n \hat{A}$（§ 2, no. 12，推论2到命题16）和$\hat{A}$上的拓扑是$m$-adic拓扑。由于$\hat{A}/\hat{m}$与$A/m$同构的，它是诺特环，并且$\hat{m} = m \hat{A}$是有限生成的$A$模块，因此$\hat{A}$是诺特（§ 2, no. 10，推论5 定理2);最后，由于 $\hat{A}$ 是 Hausdorff 并且相对于 $m$-adic 拓扑来说是完整的，$\hat{A}$ 是 Zariski 环 (no. 3, *例* 1)。

断言 (ii) 紧接着从$j$派生的典范同态$A/m + \hat{A}/\hat{m}$是双射的事实以及$\hat{A}$包含于$\hat{m}$的每个最大理想，因为$\hat{A}$是Zariski环和Jacobson根式$\hat{A}$ 然后包含 $m$（no. 3，命题 6）。

最后让我们证明(iii)。作为$n = j^{-1}(A)$，$j(A - n) \subset \hat{A} - \hat{n}$和$j$当然是定义同态$j': A_n \to \hat{A}_{\hat{n}}$（章II, § 2, no. 1，命题2）。让我们证明 $j'$ 是单射的；让$a \in A, s \in A - n$这样
$$
j'(a/s) = j(a)/j(s) = 0;
$$
则存在$s' \in \hat{A} - \hat{n}$，使得$\hat{A}$中$j(a)$的$s'j(a) = 0$（章II, § 2, no. 1，*注* 3）和湮没子因此不包含在$\hat{n}$中。现在，如果$A$中$b$是$a$的湮没子，则$\hat{A}$中$j(a)$的湮没子是$b$（推论1到定理3）；因此$b \notin n$，它表明$a/s = 0$。

此外，还有一个可交换的图表
$$
\begin{array}{ccc}
A/n^k & \longrightarrow & A_n/(nA_n)^k \\
h \downarrow & & h' \downarrow \\
\hat{A}/\hat{n}^k & \longrightarrow & \hat{A}_{\hat{n}}/(\hat{n}\hat{A}_{\hat{n}})^k
\end{array}
$$
其中$h$和$h'$分别源自$j$和$j'$，水平箭头是章II, § 3, no. 3、命题9的典范同构。 由于$n^k$是$A$的开放理想（因为它包含$m^k$），$h$是双射的，因此$h'$也是双射的。 这首先表明$A_n$上的$(nA_n)^k = j'((\hat{n}\hat{A}_{\hat{n}})^k)$以及拓扑是由$A_n$上的⟦⟦⟧诱导的；此外，$\hat{A}_{\hat{n}} = A_n + (\hat{n}\hat{A}_{\hat{n}})^k$对于所有$k > 0$，因此$A_n$在$A_n$中处处稠密。

#### 推论{#ac-iii-s3-n4-cor-1 .statement tag=04GQ}

*设* $A$ *为诺特局部*（或*半局部*）*环和*$m$ *其雅各布森激进式。那么* $\hat{A}$ *是诺特局部*（或*半局部*）*环，其雅各布森根式是* $\hat{m}$。

$\hat{A}$ 是诺特命题 8 (i)，其余部分由命题 8 (ii) 和推论 1 中的第三个公式到定理 3。

### 5. 完成 ZARISKI 环

#### 命题 9 {#ac-iii-s3-prop-9 .statement tag=04GR}

设$A$是可交换的诺特环，$m$是$A$的理想；让 $A$ 被赋予 $m$-adic 拓扑。为了使 $\hat{A}$ 成为忠实的扁平 $A$ 模，$A$ 是 Zariski 环是充分必要的。

对于每个有限生成的$A$-模块$M$，典范映射$M \to M \otimes_A \hat{A}$都用典范映射$M \to \hat{M}$标识，从$M$到其相对于$m$-adic拓扑（no. 4，那么这个映射的定理3)和核就是$M$中的$\{0\}$相对于这个拓扑的闭包。我们已经知道，$\hat{A}$是一个平坦的$A$模块（no. 4，定理3），命题源自忠实平坦的模（章I, § 3, no. 1，命题1（b））的刻画，并且扎里斯基的刻画环（no. 3，命题6）。

如果 $A$ 是 Zariski 环并且 $E$ 是有限生成的 $A$ 模块，我们可以（凭借命题 9）认同 $E$ 以及 $\hat{E}$ 的子集通过典范映射 $j_E : E \to \hat{E}$。有了这个标识：

#### 推论 1 {#ac-iii-s3-prop-9-cor-1 .statement tag=04GS}

令 $A$ 为 Zariski 环，$E$ 为有限生成的 $A$ 模块，$F$ 子模为 $E$。然后$F = \hat{F} \cap E = (\hat{A}F) \cap E$。

这是章 I, § 3, no. 5, 命题 10 (ii) 的特例，它也是从 no. 3, 命题 6 得出的。

#### 推论 2 {#ac-iii-s3-prop-9-cor-2 .statement tag=04GT}

令 $A$ 为 Zariski 环，$E$ 为有限生成的 $A$ 模块。如果 $\hat{E}$ 是免费的 $A$ 模块，则 $E$ 是免费的 $A$ 模块。

令 $m$ 为 $A$ 的定义理想，因此它包含在 $A$ 的雅各布森根式中。 我们应用章II, § 3, no. 5、命题5的标准：典范映射$j_E : E \to \hat{E}$定义双射$i_E : E/mE \to \hat{E}/(mE)^{\wedge}$；同样典范映射$j_A : A \to \hat{A}$定义双射$i_A : A/m \to \hat{A}/\hat{m}$，即环同构。 然后$(mE)^{\wedge} = \hat{A}.mE = \hat{m}\hat{E}$ (no. 4, 定理 3)，因此$\hat{E}/(mE)^{\wedge}$被赋予一个$(\hat{A}/\hat{m})$模块结构，因此（通过$i_A$）一个$(A/m)$模块结构。 It is immediate that $i_E$ is $(A/m)$-linear, so that it is an $(A/m)$-module isomorphism. 由于 $\hat{E}/\hat{m}\hat{E}$ 是免费的 $(\hat{A}/\hat{m})$ 模块，$E/mE$ 是免费的 $(A/m)$ 模块。

另一方面，令$\nu : m \otimes_A E \to E$为典范同态；因为 $(m \otimes_A E) \otimes_A \hat{A}$ 与 $m \otimes_A \hat{E}$ 和 $E \otimes_A \hat{A}$ 与 $\hat{E}$ (no. 4, 定理 3)、假设被规范地标识为 $\hat{E}$ 是一个自由的 $\hat{A}$ 模块，这意味着同态 $\nu \otimes 1 : \hat{m} \otimes_{\hat{A}} \hat{E} \to \hat{E}$ 是单射。由于 $\hat{A}$ 是一个忠实的扁平 $A$ 模 (命题 9)，我们结论 $\nu$ 是单射 (章 I, § 3, no. 1, 命题 2) 和条件对于应用上述标准确实是实现了。

#### 推论 3 {#ac-iii-s3-prop-9-cor-3 .statement tag=04GU}

令$A$为Zariski环，使得$\hat{A}$为整环，并令$a$为$A$的理想。如果$\hat{A}$的理想$a\hat{A}$为主，则$a$为主。

这是推论2的一个特例。

#### 推出 4 {#ac-iii-s3-prop-9-cor-4 .statement tag=04GV}

令$A$为Zariski环，使得$\hat{A}$为整环，$\hat{A}$的分数的$L$域以及分数的$K \subset L$域 $A$；然后$\hat{A} \cap K = A$。

显然$A \subset \hat{A} \cap K$；另一方面，如果$x \in \hat{A} \cap K$，则$\hat{A}x \subset \hat{A}$，因此为$\hat{A}x = \hat{A} \otimes_A (Ax)$（no. 4，定理 3），$\hat{A} \otimes_A ((Ax + A)/A) = 0$。由于$\hat{A}$是一个忠实的扁平$A$模（命题9），我们推断出$Ax \subset A$，从而$x \in A$。

#### 推出 5 {#ac-iii-s3-prop-9-cor-5 .statement tag=04GW}

令$A$是可交换的诺特环，$E, F$两个有限生成的$A$模，$u : E \to F$是$A$同态。对于 $A$ 的每个最大理想 $m$，令 $A(m)$（分别为 $E(m), F(m)$）表示 $A$（分别为 $E, F$）相对于 $m$-adic 拓扑和 $u(m) : E(m) \to F(m)$ 的 Hausdorff 完成相应的同态至$u$。对于 $u$ 是单射的（分别是满射、双射的、零），$u(m)$ 对于每个最大理想 $m \notin A$ 都是必要且充分的。

我们知道，要使 $u$ 成为单射（或满射、双射的、零），$u_m : E_m \to F$ 对于 $A$ 的每个最大理想 $m$ 都是必要且充分的（章 II, § 3, no. 3、定理 1）。我们现在注，$A$是诺特局部环（章II, § 2, no. 4，推论2到命题10），因此是Zariski环，并且存在规范的$A$-代数同构$\hat{A}_m \to A(m)$（§ 2, no. 13，命题18）。另一方面（从no. 4开始），有一个可交换的图表

$$
\begin{array}{ccc}
E_m \otimes_{A_m} A(m) & \longrightarrow & E \otimes_A A(m) \longrightarrow E(m) \\
u_m \otimes 1 \downarrow & & \downarrow u \otimes 1 \downarrow u(m) \\
F_m \otimes_{A_m} A(m) & \longrightarrow & F \otimes_A A(m) \longrightarrow F(m)
\end{array}
$$

其中左侧的水平箭头来自张量积和同构 $E_m \to E \otimes_A A_m, F_m \to F \otimes_A A_m$ 的结合性；由于$E$和$F$是有限生成的$A$模块，因此从no. 4，定理3可以得出，这个图表的行由同构组成；因此，我们被简化为证明，$u_m$是单射（分别是满射、双射的、零）等价于$u_m \otimes 1$。但这源于以下事实：$\hat{A}_m$（因此也是$A(m)$）是命题 9（章I, § 3, no. 1、命题 1 和 2）的忠实平坦$A_m$模。

#### 命题 10 {#ac-iii-s3-prop-10 .statement tag=04GX}

令 $A, B$ 为两个 Zariski 环、$\hat{A}, \hat{B}$ 它们的完成，$f : A \to B$ 连续的环同态和 $\hat{f} : \hat{A} \to \hat{B}$ 同态从 $f$ 通过经过获得到完成；如果 $\hat{f}$ 是双射的，则 $A$-模 $B$ 是忠实平坦的。

由于 $A$ 和 $B$ 是 Hausdorff，因此 $\hat{f}$ 是双射的假设首先意味着 $f$ 是单射的。通过off方法将$A$与$f(A)$（代数地）识别，并通过$\hat{f}$将$\hat{A}$与$\hat{B}$进行识别，然后我们得到包含物$A \subset B \subset \hat{A} = \mathbf{8}$；我们知道$\hat{A}$是一个忠实平坦的$A$模块和一个忠实平坦的$B$模块（命题9）；我们结论认为$B$是一个忠实的扁平$A$模块（章I, § 3, no. 4，注2）。

#### 命题 11 {#ac-iii-s3-prop-11 .statement tag=04GY}

令$\mathbf{A}$为诺特局部环，$m$其最大理想，$\hat{\mathbf{A}}$其$m$进数补全，以及$B$环使得$\mathbf{A} \subset B \subset \hat{\mathbf{A}}$。假设$B$是诺特局部环，其最大理想$n$满足关系$n = mB$。然后

$$
n^k = m^kB = \hat{m}^k \cap B
$$

对于所有$k \geq 1$，$B$上的$n$-adic 拓扑是由$\hat{\mathbf{A}}$上的$m$-adic 拓扑诱导的，$B$是一个忠实的平坦$\mathbf{A}$-模，并且有同构 $\hat{\mathbf{A}}$ 到 $B$ 的$n$-adic补全$\hat{B}$，其中扩展典范嵌入$\mathbf{A} \to B$。

验证关系$n^k = \hat{m}^k \cap B$就足够了，因为$B$在$\hat{\mathbf{A}}$中是稠密的，并且$n$-adic拓扑是由$m$-adic拓扑诱导的，最后一个断言将从*一般得出拓扑*、章 II, § 3, no. 9，推论 1 到命题 18 以及命题 10 中的最后一个，单射 $j_A : \mathbf{A} \to \hat{\mathbf{A}}$（分别为 $j : B \to \hat{\mathbf{A}}$）定义通过取商单同态

$$
i_1 : \mathbf{A}/(\hat{m} \cap \mathbf{A}) \to \hat{\mathbf{A}}/\hat{m}
$$

（分别$i_B : B/(\hat{m} \cap B) \to \hat{\mathbf{A}}/\hat{m}$）。我们知道$m \cap \mathbf{A} = m$和$i_A$是双射的，因此$i_B$是双射的，这表明$B/(\hat{m} \cap B)$是域，因此$\hat{m} \cap B$是$B$的极大理想，因此$m \cap B = n$。如$\mathbf{A} = \mathbf{A} + m$、$B = A + n = A + mB$；由归纳在 $k$ 我们推断出

$$
B = A + m^kB = A + n^k
$$

对于所有$k > 1$。作为$n^k \subset \hat{m}^k \cap B$，证明$\hat{m}^k \cap B \subset n^k$就足够了；如果$b \in \hat{m}^k \cap B$，我们可以写成$b = a + z$，其中$a \in \mathbf{A}$，$z \in n^k$； 从而

$$
a = b - z \in \hat{m}^k \cap \mathbf{A} = m^k \subset n^k
$$

和$b \in n^k$。

\* 应用此方法的一个重要情况如下：$B$是级数在完整值域上的$n$变量的积分环，其收敛于0的邻域，$\mathbf{A}$是局部环

$$
K[X_1, \ldots, X_n]_{\mathfrak{p}}
$$

其中 $\mathfrak{p}$ 是没有常数项的多项式的最大理想由……组成，$\hat{\mathbf{A}}$ 是形式幂级数 $K[[X_1, \ldots, X_n]]$ 的环。 \*

#### 注 {#ac-iii-s3-n5-rem-1 .statement tag=04GZ}

局部环$B$使得$\mathbf{A} \subset B \subset \hat{\mathbf{A}}$，其最大理想$n$等于$mB$并且其$n$-adic拓扑由$\mathbf{A}$上的$m$-adic拓扑诱导，不一定是诺特（习题14）。

#### 命题 12 {#ac-iii-s3-prop-12 .statement tag=04H0}

令 $A$ 为交换律诺特环，$m$ $A$ 的理想，$S$ $A$ 的乘法子集 $1 + m$ 和 $E$ 有限生成$A$-模块。在这些条件下：

(i) $S^{-1}A$ 是 Zariski 环与 ($S^{-1}m$)-adic 拓扑。

(ii) *典范映射* $f : E \to S^{-1}E$ *是连续的，如果* $E$ *给定 m-adic 拓扑且* $S^{-1}E$ ** $(S^{-1}m)$-adic 拓扑且 $\hat{f} : E \to (S^{-1}E)^{\wedge}$ *为同构。*

$1 + (S^{-1}m)$的每个元素都是形式
$$
1 + (m/(1 + m')) = (1 + m + m')/(1 + m)
$$
其中 $m \in m$ 和 $m' \in m$；因此它在 $S^{-1}A$ 中是可逆的，这证明 $S^{-1}m$ 包含在 $S^{-1}A$ 的雅各布森根式中；因为 $S^{-1}A$ 是诺特（章 II, § 2, no. 4，推论 2 到命题 10），$S^{-1}A$ 是带有 $(S^{-1}m)$-adic 拓扑的 Zariski 环，这证明了 (i)。让我们展示 (ii)。对于所有$n > 0$，
$$
\bar{f}^{-1}((S^{-1}m)^nE) = \bar{f}'(S^{-1}(m^nE)) = m^nE:
$$
首先显然是$f(m^nE) \subset S^{-1}m^nE$；反之，令$x$为$\bar{f}^{-1}(S^{-1}m^nE)$的元素；则存在$m$和$x'' \in m^nE$的元素$m', m''$使得$(1 + m')((1 + m'')x - x'') = 0$，从而$(1 - m)x = x'$，其中
$$
m = -(m' + m'' + m'm'') \in m
$$
和$x' = (1 + m')x'' \in m^nE$；我们结论那个
$$
x = (1 + m + \cdots + m^{n-1})x' + m^n x \in m^nE.
$$
这证明$f$是严格的态射。此外，$f$的核，即$x \in E$的集合，存在一些$s \in S$使得$sx = 0$，与典范映射$j : E \to \hat{E}$的核相同（no. 2， 命题5)。然后有一个拓扑同构$f_0 : j(E) \to f(E)$使得$f = f_0 \circ j$；因为$\hat{f}$是拓扑同构，问题约化来验证$f(E)$在$S^{-1}E$中是稠密的。现在$S^{-1}E$的每一个元素都可以写成$x/(1 - m)$，其中$m \in m$，立即验证：
$$
x/(1 - m) \equiv ((1 + m + \cdots + m^{n-1})x)/1 \pmod{S^{-1}m^nE}
$$
完成证明。

### 习题{#ac-iii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
