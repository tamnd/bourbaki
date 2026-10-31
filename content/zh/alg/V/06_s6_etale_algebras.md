---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 6
section_title: Etale algebras
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.26-A V.36, A V.151
pdf_pages: 0140-0150, 0265-0265
extraction: ocr
subsections:
    - "no": 1
      title: Linear independence of homomorphisms
      page: 26
      pdf_page: 140
    - "no": 2
      title: Algebraic independence of homomorphisms
      page: 28
      pdf_page: 142
    - "no": 3
      title: Diagonalizable algebras and etale algebras
      page: 28
      pdf_page: 142
    - "no": 4
      title: Subalgebras of an etale algebra
      page: 30
      pdf_page: 144
    - "no": 5
      title: Separable degree of a commutative algebra
      page: 31
      pdf_page: 145
    - "no": 6
      title: Differential characterization of etale algebras
      page: 33
      pdf_page: 147
    - "no": 7
      title: Reduced algebras and etale algebras
      page: 34
      pdf_page: 148
statements: 22
exercises: 2
content_sha256: 505457b29750f206649ccbc4d88bee8676e8e455ecc7b42a2100e8123b9baf5b
translated_from: content/en/alg/V/06_s6_etale_algebras.md
translation_method: google
source_content_sha256: 3c20d3c3070caf43cf4bd713b7f6047a4fcb2604b1f551ae1ea6b1868b0306eb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 50af687b67ee3cbcfad045795881c5ebd5041ea0f7b8e7677861f7bcc4d87f78
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 6。总计代数

在本段中，K 表示域。

### 1. 同态线性独立

设L为K的扩张，且V为K上的向量空间。在本段中，我们将用$\operatorname{Hom}_K(V, L)$集合来表示V的所有K-线性映射到L，配备向量空间结构于 L 使得：

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

对于$\mathrm{Hom}_K(V, L)$中的$x \in V,\ a \in L$和$f,\ g$。令 $V_{(L)} = L \otimes_K V$ 为 L 上的向量空间，由 V 通过标量扩张导出，$(V_{(L)})^*$ 是其对偶。到II，p. 277，我们有向量L的典范同构$u \mapsto 3$-空间从$(V_{(L)})^*$到$\mathrm{Hom}_K(V, L)$，这样$\tilde{u}(x) = u(1 \otimes x)$对于$x \in V$和$u$ $(V_{(L)})^*$。如果V是*有限*维数$n$超过$K$，向量空间$(V_{(L)})$超过$L$是维数$n$，以及它的对偶$(V_{(L)})^* = V_{(\bar{L})}^*$， 从而公式

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### 定理 1 {#alg-v-s6-thm-1 .statement tag=06JB}

— *设L为域K之扩张且A代数除以K；设$\mathscr{H}$为A的所有K-代数同态到L中的集合。那么 $\mathscr{H}$ 是向量空间 $\mathrm{Hom}_K(A, L)$ 超过 L 的免费子集。*

让我们通过整数$n \geq 0$上的归纳来证明，$\mathscr{H}$的不同元素的每个序列$(u_1, \ldots, u_n)$都是免费的。案例$n = 0$是微不足道的，我们从此可以假设$n \geq 1$；令 $a_1, \ldots, a_n$ 为 L 的元素，使得 $$\sum_{i=1}^n \alpha_i u_i = 0.$$ 对于 A 中的$x,\ y$，我们有
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
从而 $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ 通过归纳假设、元素 $u_1, \ldots, u_{n-1}$ 的 $\mathscr{H}$ 是线性独立的，从而 $\alpha_i [u_i(x) - u_n(x)] = 0$ 对于 $1 \leq i \leq n-1$ 和 A 中的所有 $x$。 $u_i$ 是不同的，这意味着 $\alpha_i = 0$ 对应于 $i \neq n$，因此 $\alpha_n u_n = 0$ 以及$\alpha_n = \alpha_n u_n(1) = 0$（用 A 的 1 单位元表示）。这样我们就证明了$a_1, \ldots, a_{n-1}, \alpha_n$是零，这就证明了定理。

#### 推论 1 {#alg-v-s6-thm-1-cor-1 .statement tag=06JC}

— *令$\Gamma$为幺半群，将$\Gamma$的同态的L域和X集合转换为L的乘法幺半群。那么 X 就是向量 L 的自由子集 - $L^\Gamma$ 的映射的 $\Gamma$ 到 L。*

令 A 为幺半群 $\Gamma$ 的代数，其系数在 A 的 L 和$(e_\gamma)_{\gamma \in \Gamma}$ 典范基中，超过 L（III，p. 446）。对于 A 到 L 的每个 L-线性映射 $u$ 让我们写 $\tilde{u}(\gamma) = u(e_\gamma)$ （对于 $\gamma \in \Gamma$）；那么映射$u \mapsto 3$是向量L的同构-$\mathrm{Hom}_L(A, L)$到$L^\Gamma$的空间，其中映射到X集合的空间A 到 L 的L-代数同态。现在应用 Th 就足够了。 1 与 $K = L$。

#### 推论 2（戴德金定理）{#alg-v-s6-thm-1-cor-2 .statement tag=06JD}

*设E和L是K的两个扩张。E到L的K同态的集合在L上是自由的。如果 E 在 K 上为有限次数，则 E 到 L 的 K 同态的数至多等于 $[E : K]$。*

考虑到公式 (2)，最后一个断言从第一个开始。

### 2. 同态的代数独立性

#### 定理 2 {#alg-v-s6-thm-2 .statement tag=06JE}

— 令 K 为无限域，K 的 L 扩张和 K 上的 A 代数。令 $u_1, \ldots, u_n$ 不同于 A 的 K-代数同态到 L 和 f $L[X_1, \ldots, X_j]$ 中的多项式。如果我们对所有$x \in A$都有$f(u_1(x), \ldots, u_n(x)) = 0$，那么$f = 0$。

设B为形式$(u_1(x), \ldots, u_n(x))$$L^n$元素集合和$x \in A$。由 Th. 1、元素中不存在序列$(\alpha_1, \ldots, \alpha_n)$，L中并非所有零，使得$\sum_{i=1}^n \alpha_i u_i(x) = 0$适用于所有$x \in A$；因此 (II, p. 301, Th.7) B 生成向量空间 $L^n$ 超过 L。因此存在$A$的元素$a_1, \ldots, a_n$使得矩阵$(u_i(a_j))_{1 \leq i,j \leq n}$是可逆的。

让我们定义多项式 $g \in L[Y_1, \ldots, Y_n]$ 为
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
设$y_1, \ldots, y,$在$K$中；写$x = \sum_{i=1}^n y_i a_i$，我们有
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
从而$g(y_1, \ldots, y_n) = 0$
由 $f$ 假设出发。由于域 $K$ 是无限的，所以我们有 $g = 0$ (IV, p. 18, Cor. 2)；现在矩阵$(u_i(a_j))$有一个逆$(b_{ij})$，我们有
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
从而$f = 0$。

Th。 2 没有有限域的类似物。因此，令 $K$ 为有限域，其中 q 元素、$A = L = K$ 和 $f(X) = X^q - X$。我们对所有 $x \in K$ 有 $x^q = x$（V、p. 93，提案 2）；因此，如果$u$是$K$的恒等式自同构，则对于所有$x \in K$，我们有$f(u(x)) = 0$，甚至虽然$f$不是零。

### 3. 可对角化代数和 etale 代数

#### 定义 1 {#alg-v-s6-def-1 .statement tag=06JF}

— 令 A 大于 K 代数；则如果存在整数 $n \geq 0$ 使得 A 同构于乘积代数 $K^n$，则称 A 可对角化的。如果通过标量的扩张从 A 导出的代数 $A_{(L)}$ 在 L 上可对角化，我们就说 A 被 K 的扩张 L 对角化。如果存在对角化 A 的 K 的扩张，我们可以说 A 是 etale。

我们记得乘积代数$K''$是向量空间$K''$配备乘积定义

$$
(x_1, \ldots, x_n) \cdot (y_1, \ldots, y_n) = (x_1 y_1, \ldots, x_n y_n)
$$

如果$\varepsilon_1, \ldots, \varepsilon_n$是$K^n$的典范基，我们有

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{if} \quad i \neq j
$$

和$1 = \varepsilon_1 + \ldots + \varepsilon_n$。

每个 etale 代数超过 $\mathbf{K}$ 都是*可交换的*，并且 *有限次数* 超过 $K$。

#### 命题 1 {#alg-v-s6-prop-1 .statement tag=06JG}

*设 A 为有限次数 n 中的代数除以域 K ；那么下面的条件是等价的：*
  *a)* *代数 A 可对角化的。*
  *b)* *A 存在基 $(e_1, \ldots, e_n)$，使得 $e_i^2 = e_i$ 和 $e_i e_j = 0$ 对应 $i \neq j$。*
  *c)* *将 A 的K-代数同态转换为 $\mathbf{K}$ 生成向量 K 空间 A 的对偶。*
  *d)* *每个 A-模是子模的直和，其中维数 1 除以 K。*

*a)* 和 *b)* 的等价由公式 (6) 得出；另一方面，n 投影 $K^n \to K$ 是代数同态，因此 *a)* 意味着 *c)*。如果*c)*成立，将A的代数同态转化为A的对偶(*V*,p. 27,Th.1)的$\mathbf{K}$形式基，我们用$u_1, \ldots, u_n$表示；那么 $a \mapsto (u_i(a))$ 是 A 的同构到代数 $K''$，从而 *a)*。由此我们建立了等价条件 *a)*、*b)* 和 *c)*。

假设*b)*成立并令M为A-模；那么比率$e_i$的同位$(e_i)_M$是$M$的投影算子，$M$是$e_i M$的直和，它们都是子A模。因此，我们可以假设存在指标$i$，使得$(e_j)_M = 0$对应于$j \neq i$。因此，$M$的每个向量子空间都是一个子A模块，从而*d)*。

相反，假设 *d)* 成立并考虑 A-模 A,。那么向量 K 空间 A 存在基 $(f_i)$，使得$Af_i = Kf_i$ 对于$i = 1, \ldots, n$。 之后替换每个$f_i$乘以一个合适的标量倍数，如有必要，我们可以假设$1 = f_i + \ldots + f_n$。如果$i \neq j$，则$f_i f_j$属于到$Af_i \cap Af_j = Kf_i \cap Kf_j$，因此它是零。现在$f_i = f_i f_1 + \ldots + f_i f_n = f_i^2$，从而 *b)*。

#### 推论{#alg-v-s6-n3-cor-1 .statement tag=06JH}

*设L为K的扩张，将A的代数同态的$\mathscr{H}$集合代入L。当且仅当 A 被 L 对角化时，我们有卡片 $\mathscr{H} \leq [A : K]$，其中等式。如果 A 按 L 对角化，则 $\mathscr{H}$ 是向量 L-空间 $\mathrm{Hom}_K(A, L)$ 的基。*

向量空间 $\mathrm{Hom}_K(A, L)$ 超过 L 有维数 $[A : K]$，由公式 (2) 提供，$\mathscr{H}$ 是 Th 的 $\mathrm{Hom}_K(A, L)$ 的免费子集。 1（*V*，p. 27）。因此，当且仅当$\mathscr{H}$是$\mathrm{Hom}_K(A, L)$的基时，我们才有卡$\mathscr{H} \leq [A : K]$和等式。存在同构向量 L 空间，例如 $\pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^*$，其特征为 $u(x) = (\pi u)(1 \otimes x)$ 代表 $x \in A$，以及 $\pi$ 映射 $\mathscr{H}$ 到集合 $\mathscr{H}_L$ L-$A(\cdot)$到L的代数同态。最后，命题 1 中 a) 和 c) 的等价表明，L上的代数$A_{(L)}$可对角化当且仅当$\mathscr{H}_L$生成向量空间$A_{(L)}^*$超过L。这就完成了推论的证明。

#### 命题 2 {#alg-v-s6-prop-2 .statement tag=06JI}

— *令 A 为 K 上的代数且 K 上的 $\Omega$ 代数闭扩张。以下断言是等效的*：

a) *代数 A 是 etale*。
b) *存在有限次数对角化A*的扩张。
c) K 的 *扩张 $\Omega$ 对角化 A*。

假设 A 是 etale。令$n$为A在K上的次数，令L为将A对角化的K的扩张，令$\mathscr{H}$为A的代数同态到L的集合。由科。对于命题 1，我们有卡片 $\mathscr{H} = n$。另一方面，对于每个$u \in \mathscr{H}$，我们有$[u(A):K] \leq n$。 V、p. 18、周四。 2、$\mathscr{H}$的元素的像生成的L的子扩展L'在K上是有限次数。由于A到L'中存在$n$不同的同态，所以扩张 L' 通过 Cor 对角化 A。命题 1 的 1. 这表明 a) 蕴涵 b)。

由于 K 的有限次数的每个扩张同构于 $\Omega$ 的子外延 (V, p. 20, Th. 1)，b) 蕴涵 c)。最后，c) 清楚地暗示了 a)。

### 4. 一个 etale 代数的子代数

#### 命题 3 {#alg-v-s6-prop-3 .statement tag=06JJ}

— *设 A 是 K 上的 etale 代数。仅存在子代数的有限数和 A 的理想。此外，对角化 A 的 K 的每个扩张也对角化 A 的每个子代数和每个商代数；特别是这些代数是 etale*。

只要证明代数$K^n$只有子代数的有限数和理想，并且子代数和$K^n$的商代数可对角化。我们用$K^n$的$(\varepsilon_1, \ldots, \varepsilon_n)$典范基来表示。

设A为$K^n$中的子代数，并令$v_1, \ldots, v_n$为n个投影$K^n \to K$中A的限制。由于$v_i$的核的交显然为0，$v_i$生成向量K空间对偶于A（II，p. 302，Cor.1）；因此 K-代数 A 是可对角化的（V，p. 29，命题 1）。

对于$\{1, 2, \ldots, n\}$的每个子集I，放入$\varepsilon_I = \sum_{i \in I} \varepsilon_i$。显然元素$\varepsilon_I$是$K^n$的幂等；当且仅当I为空时，我们才有$\varepsilon_I = 0$，以及$\varepsilon_I \varepsilon_J = \varepsilon_{I \cap J}$。如上所述，$K^n$的每个子代数 A 都是可对角化的；根据命题 1 的条件 b)，$K^n$ 的每个子代数 A 因此承认基$(\varepsilon_{I_1}, \ldots, \varepsilon_{I_p})$，其中$(I_1, \ldots, I_p)$ 是$\{1, 2, \ldots, n\}$ 的划分，并且这样的数是有限的。 子代数。

对于$(1, 2, \ldots, n)$的每个子集I，令$a_i$为$K^n$的向量子空间，对于$i \in I$具有基幂等$\varepsilon_i$；则显然$a_i$是$K^n$的理想；此外，如果$J = (1, 2, \ldots, n) - I$，则$\varepsilon_j$模$a_i$的剩余类类$\overline{\varepsilon}_j$，对于$K^n / a_i$的$j \in J$形式基。如果 $j \neq k$，我们有 $\overline{\varepsilon}_j^2 = \overline{\varepsilon}_j$ 和 $\overline{\varepsilon}_j \overline{\varepsilon}_k = 0$，因此，根据 V、p. 29 的命题 1，代数 $K^n / a_I$ 是可对角化的。

还需要证明 $K^n$ 的每个理想都是形式 $a_I$。令I为整数$i$的集合，使得$1 \leq i \leq n$和$\varepsilon_i \in a$，然后$a_i \subset a$。令$x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n$为$a$的元素（$x_1, \ldots, x_n$在$K$中），并令$i$在$(1, 2, \ldots, n) - I$中。我们有$x_i \varepsilon_i = x \varepsilon_i \in a_i$、$\varepsilon_i \notin a$、从而$x_i = 0$。因此$x = \sum_{i \in I} x_i \varepsilon_i$，这表明$x \in a_i$。现在我们已经展示了$a \subset a_I$、从而，最后$a = a_i$。

#### 推论{#alg-v-s6-n4-cor-1 .statement tag=06JK}

— *令 $A_1, \ldots, A_r$ 大于 $K$ 和 $A = A_1 \times \cdots \times A_r$ 代数。对于 $A$ 是 etale，$A_1, \ldots, A_r$ 是 etale 是充分必要的。*

假设$A$是etale；每个代数 $A_1, \ldots, A_r$ 都同构于 $A$ 的商，因此根据命题 3 成立。相反，$K$ 的每个扩张对角化 $A_1, \ldots, A_r$ 显然对角化 $A$。

### 5. 可分离次数或交换代数

令$A$为有限次数$n$除以$K$的交换代数。对于$K$的任何扩张$L$，$A$的代数同态到$L$的数$h(L)$是有限的，并且上面的边界是$n$（V，p. 29，科。）。

#### 引理 1 {#alg-v-s6-lem-1 .statement tag=06JL}

— *令$\Omega$为$K$中的代数闭包；那么对于$K$的每个扩张$L$，我们有$h(L) \leq h(\Omega)$，当$L$是代数封闭时，等式。*

令$L'$为$L$中$K$的代数闭包。对于$A$到$L$的每个同态$u$，我们有$[u(A) : K] \leq n$，因此$u(A) \subset L'$乘以V，p. 18，命题2；因此我们有$h(L') = h(L)$。由于$K$的扩张$L'$同构于$\Omega$的子扩展（V，p. 20，Th.1），所以我们有$h(L') \leq h(\Omega)$。如果$L$是代数闭集，则$L'$是$K$的代数闭包； 扩张 $L'$ 和 $K$ 的 $\Omega$ 是同构的（V、p. 23、Th.2），因此 $h(L') = h(\Omega)$； 引理直接由此得出。

到引理 1，数 $h(L)$ 对于 $K$ 的所有代数闭扩张 $L$ 具有相同的值；这个数将被表示为$[A : K]$，并称为$A$的*可分离的次数*。

令$A$和$B$为有限次数除$K$中的两个交换代数。我们将建立公式

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

令$L$为$K$的代数闭扩张，并用$A$的代数同态的$\mathscr{H}(A)$集合表示为$L$，类似地定义、$\mathscr{H}(B)$和$\mathscr{H}(A \otimes_K B)$。 到定义时，我们有了卡 $\mathscr{H}(A) = [A : K]$ 和相应的公式，分别为 [B : K] 和 [A \otimes_K B : K]。 此外，$\mathscr{H}(A) \times \mathscr{H}(B)$的III，p. 465，公式(6))，公式$(u * v)(a \otimes b) = u(a)v(b)$定义双射$(u, v) \mapsto u * v$到$\mathscr{H}(A \otimes_K B)$，从而公式(7)如下。

设$K'$为$K$的扩张；我们将证明公式
$$
[A_{(K')}: K'], = [A: K], .
$$
取$L$为$K'$的代数闭包。 公式 $\tilde{u}(x) = u(1 \otimes x)$（对于 $x \in A$） 定义双射 $u \mapsto \tilde{u}$ $K'$ 的集合 - $A_{(K')}$ 到 $L$ 和集合的同态$K$-$A$同态为$L$、从而 (8)。

最后，假设$K'$是$K$的有限次数的扩张；如果 $A'$ 是有限次数的交换性 $K'$ 代数，那么它也是有限次数的交换性 $K$ 代数，并且我们有 $[A': K] = [A': K'] \cdot [K': K]$ (V. p. 10, Th. 1)。我们将证明公式
$$
[A': K], = [A': K']_s \cdot [K': K], .
$$
令$S$（$T$）是$K$的集合-$K'$（$A'$）同态到$K$的代数闭包$L$；对于每个$\sigma \in S$，我们用元素$f$或$T$的$T_\sigma$集合表示，这样对于所有$a \in K'$来说$f(a \cdot 1) = \sigma(a)$。那么家庭$(T_\sigma)_\sigma$是$T$的划分，我们有卡$S = [K': K]$；现在对于每个$\sigma \in S$集合$T_\sigma$都由$A'$的$K'$同态组成$K'$的代数闭扩张$(L, \sigma)$，因此卡$T_\sigma = [A': K']_s$，因此我们证明了（9）。

#### 命题 4 {#alg-v-s6-prop-4 .statement tag=06JM}

— 设$A$为有限次数除$K$的交换代数；那么 $[A: K], \leq [A: K]$ 与等式当且仅当 $A$ 是 etale。

令$\Omega$为$K$的代数闭包，将$A$的代数同态的$A?$集合代入$\mathbf{R}$。我们有卡$A? = [A: K]$，并且$A$是etale当且仅当$A$被$K$的扩张$\Omega$对角化（V，p. 30，命题2）。因此，第 4 号提案源自 Cor。 V、p. 29。

#### 推论 1 {#alg-v-s6-prop-4-cor-1 .statement tag=06JN}

— 令 $A, B$ 为 $K$ 的 2 个交换代数，其中有限非零次数。那么，要使代数 $C = A \otimes_K B$ 成为 etale，$A$ 和 $B$ 成为 etale 是充分必要的。

对于可分离的次数，我们有 $[C: K] = [A: K] \cdot [B: K]$ 和相应的公式 (7)。此外，对于$B$和$C$，我们还有$[A: K], \leq [A: K]$和相应的公式。由此可见，当且仅当我们同时拥有 $[A: K] = [A: K]$ 和 $[B: K] = [B: K]$ 时，$[C: K] = [C: K]$；现在应用提案 4 就足够了。

#### 推论 2 {#alg-v-s6-prop-4-cor-2 .statement tag=06JO}

— 令 $K'$ 为 $K$ 中的扩张。

a) 对于 $K$-代数 $A$ 是 etale，$K'$-代数 $A_{(K')}$ 是 etale 是充分必要的。

b) 令$A'$在$K'$之上为代数，而不是减少到0。为了使$A'$在$K$之上，$A'$在$K'$之上并且$K'$在$K$之上是必要且充分的。

我们争论Cor。 1、应用这次 a) 为 (8)，b) 为 (9)。

### 6. etale 代数的微分刻画

#### 定理 3 {#alg-v-s6-thm-3 .statement tag=06JP}

— 设 $A$ 为有限次数中的交换代数除以 $K$。对于$A$来说，$K$的模$\Omega_K(A)$-$A$的微分应减少到$0$是必要且充分的。

A) 设$L$为$K$的代数闭包（$V$，p. 23，Th.2）。要使 $A$ 成为 etale，代数 $A_{(L)}$ 超过 $L$ 应该可对角化（$V$，p. 30，命题 2）。此外，$A$-模块$\Omega_L(A_{(L)})$同构于$\Omega_K(A) \otimes_A A_{(L)}$（III、p. 572，命题20），因此同构于$\Omega_K(A) \otimes_K L$，结合性同构于张量积；因此$\Omega_K(A) = 0$等价于$\Omega_L(A_{(L)}) = 0$。为了证明Th. 3 因此，考虑 $K$ 代数闭的情况并证明代数 $A$ 可对角化当且仅当 $\Omega_K(A) = 0$ 就足够了。

B) 假设$A$可对角化的；那么 ($V$, p. 29, 命题 1), 向量空间 $A$ 由 $A$ 的幂等生成。因此断言$\Omega_K(A) = 0$是以下引理中的推论：

#### 引理 2 {#alg-v-s6-lem-2 .statement tag=06JQ}

令$A$比$K$更交换代数，并且$e$是$A$的幂等；那么$\Omega_K(A)$中有$de = 0$。

从关系$e = e^2$我们推导出$de = 2e \cdot de$；乘以$e$，我们得到$e \cdot de = 2e \cdot de$，因此得到$e \cdot de = 0$，最后得到$de = 2e \cdot de = 0$。

C）我们首先证明两个引理：

#### 引理 3 {#alg-v-s6-lem-3 .statement tag=06JR}

令$A$为有限次数除以代数闭域$K$的交换代数，从而得到$\Omega_K(A) = 0$。那么对于$A$的每个最大理想$m$，我们都有$m = m^2$。

代数$A/m$为代数闭域$K$有限次数、从而$[A/m : K] = 1$扩张。因此，对于每个$a \in A$，都存在一个唯一的标量$\lambda$，使得$a - \lambda \cdot 1 \in m$；将$a - \lambda \cdot 1$ mod $m^2$ 的剩余类类写为$D(a)$。很明显，$D$是$A$到$A$模块$m/m^2$的$K$派生。 $\Omega_K(A)$（III、p. 569）和假设$\Omega_K(A) = 0$的泛性质现在意味着$D = 0$、从而$m/m^2 = 0$等$m = m^2$。

#### 引理 4 {#alg-v-s6-lem-4 .statement tag=06JS}

令$A$为交换环，并令$a$为$A$的有限生成理想，使得$a = a^2$。那么$A$中存​​在幂等$e$，使得$a = Ae$。

令$(a_1, ..., a_r)$为理想$a$的生成的系统；从$a = a^2$开始，$a$中存在元素$x_{ij}$，使得$a_i = \sum_{j=1}^r x_{ij} a_j$对应于$1 \leq i \leq r$。将阶$r$的平方矩阵写成$M$，其中元素是$\delta_{ij} - x_{ij}$，并令$D$为其行列式。 $A$ 中存在阶 $r$ 和元素 (III, p. 532, 公式 (26)) 平方矩阵 $N$，使得 $N \cdot M = D \cdot I$， 从而立即$Da_j = 0$$1 \leq j \leq r$，最后$Da = 0$。现在矩阵 $M$ 等于 $I$ mod $a$，因此 $D \equiv I$ mod $a$。把$e = 1 - D$；然后 $e \in a$ 和 $ex = x$ 对于所有 $x \in a$。由此可知 $e$ 是幂等的，$a$ 等于 $Ae$。

建立这些引理后，让我们通过$A$的次数上的归纳证明，如果$K$是代数闭且$\Omega_K(A) = 0$，则$A$可对角化。令 $m$ 为 $A$ (I, p. 104) 的最大理想。到引理 3 和 4，存在幂等$e$，使得$m = Ae$；我们已经看到，$A/m$ 比 $K$ 为次数 1。因此，$A$是理想$a = (1 - e)A$和$m$的直和，并且我们有$[a : K] = 1$，因此$A$与$K \times A/a$同构的。由于 $\Omega_K(A/a)$ 与 $\Omega_K(A)$ 的商同构（III、p. 573，命题 22），因此它是零，并且归纳假设表明 $A/a$ 可对角化。这表明 $A$ 是可对角化的。

### 7. 减少代数和 etale 代数

#### 定义 2 {#alg-v-s6-def-2 .statement tag=06JT}

— *令$A$为交换环；那么如果$A$的每个幂零元（I，p. 98）都是零，则称$A$减少了。*

如果$A$是减少的环的域、或整环、或乘积，则它是减少的环。 为了减少交换环$A$，对于$A$中的每个$a \neq 0$，$a^2 \neq 0$是必要且充分的：因为由此我们在$n$、$a^{2^n} \neq 0$上通过归纳获得，因此对于$A$中的任何$a \neq 0$获得$a^n \neq 0$。

如果代数的底层环减少，则称代数“减少”。

#### 命题 5 {#alg-v-s6-prop-5 .statement tag=06JU}

— *令 $A$ 为有限次数中的交换代数除以 $K$。 For $A$ to be reduced it is necessary and sufficient that there exist extensions $L_1, \ldots, L_s$ of finite degree over $K$ such that $A$ is $K$-isomorphic to $L_1 \times \cdots \times L_s$.*

所规定的条件显然是足够的。

反之，假设$A$减少；通过归纳对$A$的次数论证，我们发现只要证明如果$A$不是域，则存在两个非零代数、$A_1$和$A_2$，使得$A$同构于$A_1 \times A_2$，或者$A$中存在不同于0和1的幂等。

假设从现在开始$A$被减少并且不是域。在$A$不同于0和$A$的理想中，令$a$为维数作为向量$K$空间最小的理想。对于$a$中的任何$x \neq 0$，我们有$x^2 \neq 0$，因为$A$减少了，从而$a' \neq \{0\}$。我们有$a^2 \subset a$，通过$a$的极小值，我们发现$a' = a$。到引理 4 时，存在幂等$e$，使得$a = Ae$，并且我们有$e \neq 0, e \neq 1$，因为$a$不同于0和$A$。

#### 定理 4 {#alg-v-s6-thm-4 .statement tag=06JV}

— *令$A$为有限次数中的交换代数除以$K$。那么下面的断言是等价的：
a) 代数 $A$ 是 etale。
b) 对于$K$中的每一个扩张$L$，环$L \otimes_K A$都会减少。
c) 存在$K$的完美扩张域$P$，使得环$P \otimes_K A$减少。
d) $K$ 存在可分离代数扩张 $L_1, \ldots, L_s$，使得 $A$ 同构于 $L_1 \times \cdots \times L_s$。*
特别是，每个 etale 代数都会减少。

A) 我们首先证明$a$、$b$和$c$的等价。

假设$A$是etale，并令$L$为$K$的扩张。令$\Omega$为$L$的代数闭扩张域（V，p. 23，Th.2）。那么$L \otimes_K A$同构于$\Omega \otimes_K A$的子环，并且后者根据命题2同构于环$\Omega^n$（V，p. 30）。因此环 $L \otimes_K A$ 减少。

因此我们已经证明a) 蕴含b)，并且c) 是b) 的特例。现在假设 c) 成立。为了使 K-代数 $A$ 成为 etale，P 代数 $A_{(P)}$ 应该成为 etale 是必要且充分的（V，p. 32，Cor. 2）。因此，代数 $A$ 由以下引理构成：

#### 引理 5 {#alg-v-s6-lem-5 .statement tag=06JW}

*令 B 为完美域 P 的有限次数减少代数；那么 B 就是 etale。*

根据命题5，存在$P$的扩张$L_1, \ldots, L_n$，使得$B$同构于代数$L, x \ldots x L_n$。由于 etale 代数的有限乘积是 etale（V，p. 31，Cor.），因此足以检查 $B$ 是 $P$ 的扩张的情况。由 Th. 3（V，p. 33）足以证明对于所有$x \in B$，$\Omega_P(B)$中有$dx = 0$。

设 $x \in B$；因为$B$是$K$上的有限次数，$x$是$K$上的代数（V，p. 18，命题2）。令 $f$ 为 $x$ 的最小多项式，并令 $f'$ 为导数。多项式 $f$ 是非常数。假设$f' = 0$；由V，p. 9，Cor。 域 $P$ 具有特征 $p \neq 0$，我们有 $f \in P[X^p]$；由于$P$是完美的，我们有$P[X^p] = P[X]^p$，但不可约多项式$f$不能位于$P[X]^p$。

因此，我们有 $f' \neq 0$，并且由于 $f'$ 的次数严格小于该值，因此我们有 $f'(x) \neq 0$。现在，我们从$f(x) = 0$推出$\Omega_P(B)$、从而$dx = 0$中的$f(x) \cdot dx = 0$，正如我们必须证明的那样。

*B) 假设$A$是etale；通过a)和b)的等价代数$A$减少，因此存在$K$的扩张$L_1, \ldots, L_n$，使得$A$同构于$L_1 \times \cdots \times L_n$（命题5）。由于$A$是etale，扩张$L_i$都是一个etale代数（V，p. 31，Cor.），因此定义是$K$的可分离代数扩张。

蕴涵$d) \Rightarrow a)$源自V、p. 31、Cor。 \*

#### 推论{#alg-v-s6-n7-cor-1 .statement tag=06JX}

— *假设$K$具有特征$p \neq 0$。对于 $A$ 来说，$A = K[A^p]$ 是必要且充分的。对于$A$中的每一个基$(a_i)_i$超过$K$，族$(a_i^p)_i$就是$A$中的基超过$K$。*

让我们选择代数闭包 $\Omega$ $K$。给定$A$到$\Omega$的两个$K$同态$u$和$v$，如果$u$和$v$具有相同的限制到$K[A^p]$，我们有

$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p,
$$

从而$u(x) = v(x)$

对于所有$x \in A$。因此我们有不等式 $[A : K], \leq [K[A^p] : K]_s$；如果 $A$ 是 etale，那么我们有

$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$

从而$A = K[A^p]$

相反，假设我们有 $A = K[A^p]$；令$(a_i)_{i \in I}$为$A$除$K$的基。根据$V$，p. 4，命题2，b），族$(a_i^p)_{i \in I}$生成向量$K$-空间$K[A^p]$，并且由于$A = K[A^p]$等于有限维等于$I$的基数，所以族$(a_i^p)_{i \in I}$ 是$A$ 中的基超过$K$。令$u$为$\Omega \otimes_K A$的元素，使得$u^2 = 0$、从而$u^p = 0$；由于$(a_i)_{i \in I}$是$A$的基超过$K$，因此存在$\Omega$的元素的$(\lambda_i)_{i \in I}$族，使得$u = \sum_{i \in I} \lambda_i \otimes a_i$，从而$u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p$。由于$(a_i^p)_{i \in I}$是$A$的基超过$K$和$u^p = 0$，所以对于所有$i \in I$，我们必须有$\lambda_i^p = 0$，从而$\lambda_i = 0$，所以$u = 0$。这表明环$\Omega \otimes_K A$要减少；因为 $\Omega$ 是完美的，代数 $A$ 超过 $K$ 是 Th 的 etale。 4.

对于 etale 代数的另一个刻画，请参阅$V$、p. 48、命题 1。

### 习题{#alg-v-s6-exercises}

§ 6](exercises/s6/)参见[习题。
