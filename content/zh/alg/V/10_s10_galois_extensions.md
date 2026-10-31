---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 10
section_title: Galois extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.56-A V.76, A V.154-A V.160
pdf_pages: 0170-0190, 0268-0274
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Galois extensions
      page: 56
      pdf_page: 170
    - "no": 2
      title: The Galois group
      page: 58
      pdf_page: 172
    - "no": 3
      title: Topology of the Galois group
      page: 60
      pdf_page: 174
    - "no": 4
      title: Galois descent
      page: 62
      pdf_page: 176
    - "no": 5
      title: '*Galois cohomology*'
      page: 64
      pdf_page: 178
    - "no": 6
      title: Artin’s theorem
      page: 65
      pdf_page: 179
    - "no": 7
      title: The fundamental theorem of Galois theory
      page: 67
      pdf_page: 181
    - "no": 8
      title: Change of base field
      page: 69
      pdf_page: 183
    - "no": 9
      title: The normal basis theorem
      page: 72
      pdf_page: 186
    - "no": 10
      title: Finite $\Gamma$-sets and etale algebras
      page: 75
      pdf_page: 189
    - "no": 11
      title: The structure of quasi-Galois extensions
      page: 76
      pdf_page: 190
statements: 49
exercises: 23
content_sha256: ec2408697bfa957075e5c400761e42ec569b0fe7e97c6ac20d146b4378e07af3
translated_from: content/en/alg/V/10_s10_galois_extensions.md
translation_method: google
source_content_sha256: ed1a3cc64fa97276bda6bff686f4a827b57d0250dbe6c9cb5ce9dddcfe06ceb5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: ad8ed474e9a7b73881c945e4ba9d390b5d08a49aea25acd46520b65797fc4943
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 10。 伽罗瓦扩张

在本段中，K 表示域。

### 1. 定义 / 伽罗瓦扩张

#### 定理 1 {#alg-v-s10-thm-1 .statement tag=06MB}

— 令 N 为 K 的代数扩张和 N 的 K-自同构的 $\Gamma$ 群。则以下断言是等价的：
a) N 中 K 的 $\Gamma$ 属于至像下的每个元素不变量。
b) N 是 K 的可分离拟伽罗瓦扩展。
c) 对于每个$x \in N$，将$N[X]$中的x在K分裂的上的最小多项式转换为次数1的不同多项式的乘积。
b) 和 c) 的等价由 Cor 得出。命题 6 (V, p. 40) 和拟伽罗瓦扩展的定义 (V, p. 53, Def. 2)。让我们认同 K 及其在 N 中的典范像。
$a) \Rightarrow c)$：假设K是$\Gamma$的不变量的域。令 $x \in N$，在 K 上具有最小多项式 $f$，并令 A 为 N 中 f 的所有根的集合。
$$
g(X) = \prod_{y \in A} (X - y).
$$
A 的每自同构 $a \in \Gamma$ 诱导置换，因此多项式 $g \in N[X]$ 的系数保持不变。因此我们有$g \in K[X]$，并且从$g(x) = 0$开始，多项式g是$K[X]$中$f$的倍数（V，p. 16，Th.1）。此外，$f$和g是单数且g除$f$（IV，p. 16，命题5）；因此我们有$f = g$，这意味着$x$在$K$上的最小多项式$f$是次数1的不同多项式的$N[X]$中的乘积。

c) ⇒ a): 令 x 为 N 的元素而不是 K 的属于。用 K 包含于 N 的 Ω 代数闭包表示作为子扩展 (V, p. 23, Th. 2)。设 f 为 x 在 K 上的最小多项式，其次数 ≥ 2 乘以假设，并令 A 为 N 中 $f(X)$ 的根的集合。如果条件 c) 成立，则有 $f(X) = \prod_{y \in A} (X - y)$，因此 (V， p. 53，Cor. 1) A 是 Ω 中 x 的共轭的集合。由于 f 次数 ≥ 2，因此 A 元素 $y \neq x$ 中存在，因此 Ω 的 K-自同构 u 使得 $u(x) = y$。现在在假设 c) 下，K 的扩张 N 是拟伽罗瓦，因此 $u(N) = N$ (V, p. 54, Cor. 1)；由此可见，u 诱导 N 的 K-自同构 a，使得 $\sigma(x) = y \neq x$，因此 K 是 Γ 的不变量的域。

#### 定义 1 {#alg-v-s10-def-1 .statement tag=06MC}

— 如果 K 的扩张 N 是代数且满足 Th 的等价条件 a), b), c)，则称其为伽罗瓦 (Galois)。 1.

Let N be a field, Γ a group of automorphisms of N and $N_0$ the field of invariants of Γ. 当 N 是超过 $N_0$ 的代数时，它是 $N_0$ 的伽罗瓦扩张。 这不一定总是这样：对于例，假设 K 是无限的，并取 N 为有理分式 K(X) 的域；对于每个$a \in K$，令$\sigma_a$为K(X)的自同构，其中映射$f(X)$到$f(X + a)$。 集合 of all $a$, is 群 of 自同构 of K(X) whose 域 of invariants is easily seen to be K;然而 K(X) 不是 K 上的代数。

设 Ω 为 K 的代数闭包，令 A 表示 Ω 的元素集合可在 K 上分离，并且 B 表示共轭的集合在 A 的元素的 K 上可分离。则 B 由代数且可在 K 上分离的元素组成。因此 (V， p. 39，命题 6 和 p. 56，命题 5) 域 K(B) 是 K 的可分离拟伽罗瓦扩展；在其他字中，A(V,p. 55)生成的拟伽罗瓦扩张是K的伽罗瓦扩张；我们还可以说它是由 O 的子集 A 生成的 K 的伽罗瓦扩张。

特别是，K 上的可分离多项式族的 Ω 中的分裂域、K 的可分闭包是 K 的伽罗瓦扩张。

#### 命题 1 {#alg-v-s10-prop-1 .statement tag=06MD}

— 令 N 为 K 的扩张和 $(N_i)_{i \in I}$，N 的非空子扩展族。我们放入 $E = \cap_{i \in I} N_i$ 和 $F = K \left( \bigcup_{i \in I} N_i \right)$。如果所有扩张 N 都是 K 上的伽罗瓦，那么 E 和 F 也是如此。

首先，E 是代数且可在 K（V，p. 36，命题 1）上分离，对于 F（V，p. 41，命题 8）也是如此。此外，根据命题 4 (V, p. 55)，E 和 F 是 K 上的拟伽罗瓦。

#### 命题 2 {#alg-v-s10-prop-2 .statement tag=06ME}

— 令 N 为 K 的伽罗瓦扩张，E 为 N 的子外延、K 上的有限次数的子外延。存在 N 包含于 E、伽罗瓦和 K 上的有限次数的子外延 F。

由于 N 是 K 上的拟伽罗瓦，Cor。 V、p. 56的1证明了N包含E和有限次数在K上的拟伽罗瓦子扩张F的存在。由于N在K上可分，因此对于F（V，p. 36，命题1）同样成立，因此F是K上的伽罗瓦子扩张。

命题 2 意味着以下结果：令 R 为 K 和 E₁, ..., Eₙ 的代数闭包，包含在 R 中的 K 上有限次数的可分离代数扩张，则存在包含在 R 和包含 E₁, ..., Eₙ 中的 K 的伽罗瓦扩张 N，有限次数。

### 2.伽罗瓦群

#### 定义 2 {#alg-v-s10-def-2 .statement tag=06MF}

令N为域 K的伽罗瓦扩张。N的所有K-自同构的群将称为N在K上的伽罗瓦群，并表示为Gal(N/K)。

令N为K的有限伽罗瓦扩张。则N是K的有限可分拟伽罗瓦扩张。因此（V，p. 32，命题4和V，p. 54，命题3），Gal(N/K)的阶等于[N : K]。稍后我们将证明，如果 N 是 K 的伽罗瓦扩张，且 Gal(N/K) 是有限的，则 N 是 K 上的有限次数 (V，p. 66，Th.3)。

令 Ω 为 K 的代数闭扩张，并令 A 为可分离多项式 f ∈ K[X] 的 Ω 中根的集合。那么域 N = K(A) 是 K 的伽罗瓦扩张。很明显，N 的每个 K 自同构都使 A 保持稳定，并且由于生成 N 在 K 上，映射 a ↦ σ|A 是 Gal(N/K) 的同构到对称群的子群 Γ 上集合 A 的 S_A，将被称为多项式 f 的伽罗瓦群。从注 3 (V, p. 55) 可以得出，如果 x 和 y 属于到 A，则以下属性是等效的：

a) x 和 y 在 K 上共轭，
b) x 和 y 属于到 Γ 下的相同轨道，
c) x 和 y 是 f 的相同不可约因子的根。

特别是，当且仅当 A 非空并且 Γ 在 A 上传递操作时，f 是不可约的。

#### 例 1 {#alg-v-s10-n2-exa-1 .statement tag=06MG}

假设 K 的特征与 2 不同，令 N 为 K 的二次方扩张。如果 x ∈ N − K，则有 N = K(x)，并且 x 在 K 上的最小多项式为形式 f(X) = X² − aX + b，其中 a, b ∈ K。因此，我们有f(X) = (X − x)(X − y) 其中 y = a − x，因此 y 与 x 共轭；由于 f(X) 是可分的，扩张 N 是伽罗瓦。 群 Gal(N/K) 有两个元素，其中诱导集合 {x, y} 的两个置换。

#### 例 2 {#alg-v-s10-n2-exa-2 .statement tag=06MH}

\* 令 f = X³ + X² − 2X − 1 ∈ Q[X]。多项式 f 是不可约的，如果不是，那么它就有根 x ∈ Q；当写 x = a/b 且 a、b ∈ Z、a 和 b 互质时，我们应该找到 a(a² + ab − 2b²) = b3 和 a3 = b(b2 + 2ab − a2)；但这意味着除 b 且 b 除 a，因此 x = ±1，这是不可能的。将 ψ = e^{2\pi i / 7} ∈ C；则多项式 f 有根 α = ψ + ψ⁻1, β = Σ2 + Σ⁻2, γ = Σ3 + Σ⁻3。我们有 β = a² − 2 和 γ = a³ − 3α，因此扩张 Q(α) 是 Q 上的伽罗瓦。 Q(α) 在 Q 上的伽罗瓦群是阶 3 的循环，由元素 σ 生成，使得 σ(α) = β, σ(β) = γ, σ(γ) = α。 \*

#### 例 3 {#alg-v-s10-n2-exa-3 .statement tag=06MI}

假设$K = \mathbf{Q}$并取$f = X^3 - 2$。将整数的分解代入素数因子的乘积（I，p. 51），我们很容易看出2不是$\mathbf{Q}$的元素的立方。因此，多项式 $f$ 是不可约的，否则，$\mathbf{Q}$ 中将有根。令$A = \{ x_1, x_2, x_3 \}$为$\Omega$中的$f$根集合和$f$中的$\Gamma$伽罗瓦群。它传递地作用于 $A$；因此它的阶可以被三整除。另一方面，商 $j = \frac{x_2}{x_1}$ 与 1 不同，我们有 $j^3 = 1$。因此$j$满足关系$j^2 + j + 1 = 0$；现在多项式 $T^2 + T + 1 = \left( T + \frac{1}{2} \right)^2 + \frac{3}{4}$ 在 $\mathbf{Q}$ 中没有根，这表明 (例 1) $[\mathbf{Q}(j) : \mathbf{Q}] = 2$。因此$[\mathbf{N} : \mathbf{Q}]$可以被2整除，并且$\Gamma$的阶可以被6整除。由于$\Gamma$包含在阶6的群$\mathfrak{S}_A$中，所以我们有$\Gamma = \mathfrak{S}_A$。

#### 例 4 {#alg-v-s10-n2-exa-4 .statement tag=06MJ}

假设$K$具有特征$p \neq 0$，并令$K(T)$为有理分式和$U = T^p - T$的域。将$E = K[U]$和$F = K[T]$放入，则$E[X]$的多项式$f(X) = X^p - X - U$在$F$中有根$T, T+1, ..., T+p-1$。令$\sigma$为$F$的$K$自同构，使得$\sigma(T) = T+1$。我们有$\sigma^i(T) = T+i$和$\sigma(U) = U$。 群$G = \{ 1, \sigma, ..., \sigma^{p-1} \}$是阶$p$的循环，其不变量包含$E$的域；由于$[F : E] \leq p$，戴德金的定理（V，p. 27，Cor.2）意味着$E$是$G$和$[F : E] = p$的不变量的域。因此多项式 $f$ 不可约于 $E[X]$； $E$的扩张$F$是Galois，其伽罗瓦群$G$是阶$p$的循环，群$\Gamma$是群的循环置换共 $T, T+1, ..., T+p-1$。

对于此例中的推广，请参阅V、p. 93、例 2。

#### 例 5 {#alg-v-s10-n2-exa-5 .statement tag=06MK}

令$F = K(X_1, ..., X_n)$为$n$中有理分式的域，不定$X_1, ..., X_n$，系数在$K$中。放
$$
s_k = \sum_{1 \leq i_1 < ... < i_k \leq n} X_{i_1} ... X_{i_k}
$$
对于 $1 \leq k \leq n$ 和 $E = K(s_1, ..., s_n)$；我们用 $f(T)$ 表示多项式
$$
T^n - s_1 T^{n-1} + \cdots + (-1)^n s_n .
$$
我们有 $f(T) = \prod_{i=1}^n (T - X_i)$，因此 $F$ 是可分离多项式 $f(T) \in E[T]$ 的分裂域。此外，对于每个置换$a \in \mathfrak{S}_n$，都存在$F$的唯一$K$自同构$h_a$，使得$h_a(X_i) = X_{a(i)}$对应于$1 \leq i \leq n$； $1 \leq k \leq n$有$h_a(s_k) = s_k$，因此$h_a$是$F$的$E$自同构。其他字，$F$$E$伽罗瓦扩张和限制到$f(T)$定义同构根$\{ X_1, ..., X_n \}$集合 $\mathrm{Gal}(F/E)$ 到群 $\mathfrak{S}_n$。特别是，$E$由有理分式$f$组成，使得
$$
f(X_{\sigma(1)}, ..., X_{\sigma(n)}) = f(X_1, ..., X_n)
$$
对于每个$\sigma \in \mathfrak{S}_n$（cf.IV，p. 67，Cor.）。

#### 例 6 {#alg-v-s10-n2-exa-6 .statement tag=06ML}

假设 f 是次数 > 0 的单调，K 的特征 ≠ 2。定义在 A 上有一个全序，用 ≤ 表示，并设置 δ(f) = $\prod_{\alpha < \beta} (\beta - a)$、$(\alpha, \beta) \in A \times A$，并且对于每个 $\sigma \in \mathfrak{S}_A$ 放置 $\delta_\sigma(f) = \prod_{\alpha < \beta} (\sigma(\beta) - \sigma(\alpha))$。我们有$\delta_\sigma(f) = \varepsilon(u) \delta(f)$，其中$\varepsilon(u)$是$\sigma$（I，p. 64）和$\delta(f) \neq 0$的签名。对于每个$\tau \in \mathrm{Gal}(N/K)$，我们有$\tau(\delta(f)) = \delta_{\tau|_A}(f)$。因此，当且仅当$\delta(f) \in K$时，$\Gamma$包含在交错的群$\mathfrak{A}_A$中。此外，$\delta(f)^2 = \prod_{\alpha < \beta} (\beta - a)' = d(f)$是多项式f（IV，p. 81）的判别式。因此$\Gamma \subset \mathfrak{A}_A$当且仅当$d(f)$是K的元素的平方。因此，在例2中我们有$d(f) = 49 = 7^2$，在例3中，$d(f) = -108$（IV，p. 85）。

令 N 为 K 的伽罗瓦扩张，并令 L 为 N 的子扩展，N 是 K 上的伽罗瓦。N 诱导的每个 K-自同构 $\sigma$ 都是 L 的 K-自同构 $\sigma_L$ (V, p. 55, 注 1)。因此映射$\sigma \mapsto \sigma_L$是$\mathrm{Gal}(N/K)$的同态变成$\mathrm{Gal}(L/K)$，称为限制同态。

#### 命题 3 {#alg-v-s10-prop-3 .statement tag=06MM}

— *限制同态* 的 $\mathrm{Gal}(N/K)$ 到 $\mathrm{Gal}(L/K)$ *是满射*。

更一般地，考虑 N 的两个子扩展 L 和 L'，以及 L 到 L' 的 K 同构 $u$。 K 包含于 N 的选择代数闭包 $\Omega$ 作为子扩展（V、p. 23、Th.2）。存在$\Omega$的K-自同构$v$，其中重合与$u$在L上（V，p. 52，命题1），并且由于N是K的拟伽罗瓦扩展，$v$诱导a N 的 K-自同构 $\sigma$ (V, p. 55, 注 1)。其他$\mathrm{Gal}(N/K)$重合的字、元素$\sigma$和L的$u$。

### 3. 拓扑 / 伽罗瓦群

令 N 为 K 的伽罗瓦扩张和 N 与 K 的 $\Gamma$ 伽罗瓦群。 我们将N的所有映射的离散拓扑、集合$N^N$装备到自身中，并用因子的离散拓扑的乘积拓扑（“N中简单收敛的拓扑”）和群$\Gamma$ 拓扑由 $N^N$ 诱发。

令A为有限次数的N在K上的所有子扩展的集合。对于$\sigma \in \Gamma$和$E \in A$，我们将为$\Gamma$的元素$\tau$的集合写$U_E(\sigma)$，它们具有相同的限制 $\sigma$到E。如果$E = K(x_1, ..., x_n)$，集合$U_E(\sigma)$由元素$\tau \in \Gamma$组成，使得$\tau(x_i) = \sigma(x_i), ..., \tau(x_n) = \sigma(x_n)$。由此可见，$(U_F(\sigma))_{F \in \mathscr{F}}$族是$\Gamma$中$\sigma$的邻域过滤器的基。

When N is of finite degree over K, we have $N \in A$ and $U_N(\sigma) = \{\sigma\}$, hence the topology of $\mathrm{Gal}(N/K)$ is discrete; we recall (V, p. 58), that the group $\mathrm{Gal}(N/K)$ is finite in this case.

$\mathrm{Gal}(N/K)$的拓扑的描述表明，对于N的每个子扩展L，$\mathrm{Gal}(N/K)$*到*$\mathrm{Gal}(L/K)$*的*限制同态*是连续的*，它是N上的伽罗瓦。

设$A$为$\Gamma$的子集。说$A$是开放的意味着对于每个$\sigma \in A$，$A$中存在$E$，使得集合$U_E(\sigma)$包含在$A$中。 $A$的闭包$\overline{A}$由所有$\sigma \in \Gamma$组成，因此对于任何$E \in A$，都存在$\tau \in A$，其限制至$E$与$\sigma$相同； $\overline{A}$的不变量域与$A$的不变量相同。

令$\varepsilon$为$\Gamma$的中性元素，令$A'$为$N$的子外延集合（伽罗瓦）以及有限次数在$K$上的子外延。根据命题 2 (V, p. 57) 集合 $A'$ 在 $A$ 中是共尾的，因此族 $(U_E(\varepsilon))_{E \in A'}$ 是$\Gamma$ 中$\varepsilon$ 邻域的过滤器的基。此外，对于$E \in A'$集合$U_E(E)$来说，$\mathrm{Gal}(N/K) = \Gamma$的限制同态中的核变为$\mathrm{Gal}(E/K)$。由于$\mathrm{Gal}(E/K)$是有限的，因此$U_{\Gamma}(\varepsilon)$是一个开闭的子群，正常且在$\Gamma$中有限指标。

显然，我们有 $U_{\Gamma}(\sigma) = \sigma U_{\Gamma}(\varepsilon) = U_{\Gamma}(\varepsilon) \sigma$ 对应 $\sigma \in \Gamma$ 和 $E \in A'$。由于$U_{\Gamma}(\varepsilon)$对于所有$E \in A'$来说是$\Gamma$的正常子群，并且家庭$(U_E(\varepsilon))_{E \in A'}$在$\varepsilon$处是邻域的基，所以$\Gamma$的拓扑与群结构兼容（Gen.Top.，III，p. 223）。在其他字中，$\Gamma \times \Gamma$到$\Gamma$的映射$(\sigma, \tau) \mapsto \sigma \tau^{-1}$是连续的。

#### 命题 4 {#alg-v-s10-prop-4 .statement tag=06MN}

— 令 $N$ 为 $K$ 中的伽罗瓦扩张。那么伽罗瓦群 $\Gamma = \mathrm{Gal}(N/K)$ 是紧凑且完全断开的。

$\Gamma$的每个元素$\sigma$都有基邻域由……组成的开路和闭路集合$U_E(\sigma)$，因此$\Gamma$完全断开（Gen.Top.，I， p. 111）。我们有$\{\sigma\} = \bigcap_{E \in \Lambda} U_E(\sigma)$，因此$\Gamma$是分开的。对于$x$的共轭$\sigma(x)$的每个$x \in N$集合，当$\sigma$范围超过$\Gamma$时，是*有限的*，因为$x$是$K$的代数（V，p.Cor.1）；因此，$N^N$的因子空间上的$\Gamma$的所有投影都是有限的集合，这表明$\Gamma$在$N^N$中相对紧凑（Gen.Top.，I，p. 88）。尚待证明$\Gamma$于$N^N$关闭。现在，如果$u$在$N^N$中$\Gamma$的闭包中，那么对于$N$的点$(x, y)$的每个对，都存在$a \in \Gamma$和$u(x) = \sigma(x), \ u(y) = \sigma(y), \ u(x+y) = \sigma(x+y), \ u(xy) = \sigma(xy)$，从而$u(x+y) = u(x) + u(y)$和$u(xy) = u(x)u(y)$。同样的推理，对于所有$x \in K$，我们有$u(x) = x$，因此$u$是$N$到$N$的$K$同态；由于$N$是$K$的代数，$u$是$N$的$K$自同构（V，p. 52，命题1），因此$u \in T$。

令$N$为$K$的伽罗瓦扩张和$(N_i)_{i \in I}$递增有向$N$的子扩展族。假设对于所有 $i \in I$ 和 $N = \bigcup_{i \in I} N_i$，$N_i$ 是伽罗瓦超过$K$。对于每个$i \in I$，用$N_i$的$\Gamma_i$伽罗瓦群表示$K$；对于$I$中的$i \leq j$，我们定义了$N_i \subset N_j$和$\Gamma_j$到$\Gamma_i$的限制同态$\varphi_{ij}$。它是连续的，因此族$(\Gamma_i, \varphi_{ij})$是拓扑群的逆系。进一步，对于每个$i \in I$，用$\mathrm{Gal}(N/K)$中的$\lambda_i$限制同态表示为$\mathrm{Gal}(N_i/K) = \Gamma_i$；它是连续的，我们有 $\lambda_i = \varphi_{ij} \circ \lambda_j$ 对应 $i \leq j$，因此$(\lambda_i)_{i \in I}$ 定义族是 $\mathrm{Gal}(N/K)$ 的连续同态 $\Lambda$ 到 $\varprojlim \Gamma_i$。

#### 命题 5 {#alg-v-s10-prop-5 .statement tag=06MO}

— *同态* $\lambda$ *属于* $\mathrm{Gal}(N/K)$ *到* $\varprojlim \mathrm{Gal}(N_i/K)$ *是拓扑群* 的同构。

由于$\mathrm{Gal}(N/K)$是紧致的，$\lambda$连续且群$\varprojlim \mathrm{Gal}(N_i/K)$分离，因此足以证明$h$是双射的（*Gen.Top.*，*I*，p. 87，Cor.2）。设$u = (u_i)_{i \in I}$为$\varprojlim \mathrm{Gal}(N_i/K)$的元素；对于每个$i \in I$，$u_i$是$N_i$的K-自同构，$u_i$是$u_j$到$N_i$对于$i \leq j$的限制。从$N = \bigcup_{i \in I} N_i$开始，$\mathrm{Gal}(N/K)$存在唯一元素$\sigma$，对于所有$i \in I$，重合和$N_i$上存在$u_i$。因此$\sigma$是$\mathrm{Gal}(N/K)$的唯一元素，使得$\lambda(u) = u$，因此$\lambda$是双射的。

当我们将$(N_i)$族视为$N$的所有有限伽罗瓦子扩张族时，这尤其适用；那么每个群 $\mathrm{Gal}(N_i/K)$ 都是离散且有限的。因此，拓扑群 $\mathrm{Gal}(N/K)$ 同构于有限群的有向逆极限，配备离散拓扑；这就是有时，称为 *profinite* 拓扑群。

### 4.伽罗华血统

*In this No.* we denote by $N$ *a field*, $\Gamma$ *a group of automorphisms of* $N$, $e$ *the neutral element of* $\Gamma$ *and* $K$ *the field of invariants of* $\Gamma$.

令 $V$ 为向量空间超过 $N$。我们记得（II，p. 317）$V$上的*K结构*是$V$的向量子K空间$V_0$，使得K-线性映射$\varphi : N \otimes_K V_0 \to V$，其中映射$h \otimes x$到$\lambda x$是双射。令$V_0$是这样一个K-结构；对于每个$\sigma \in \Gamma$，我们放入$u_\sigma = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) \circ \varphi^{-1}$；那么对于元素$\lambda_i$的$N$和$e_i$的$V_0$从而的每个家庭我们都有$u_\sigma \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{i \in I} \sigma(\lambda_i) e_i$，我们得到关系
$$
\begin{align*}
u_\sigma(x + y) &= u_\sigma(x) + u_\sigma(y) \\
u_\sigma(\lambda x) &= \sigma(\lambda) u_\sigma(x) \\
u_\sigma \circ u_\tau &= u_{\sigma \tau} \\
u_e &= \mathrm{Id}_V
\end{align*}
$$
对于$\Gamma$中的$\sigma, \tau$、$V$中的$x, y$以及$N$中的$\lambda$。

#### 命题 6 {#alg-v-s10-prop-6 .statement tag=06MP}

— *a)* *让* $V$ *向量空间超过* $N$ *与a* $K$-*结构*。 *对于向量* $x \in V$ *右* $K$ *有理有据* $u_\sigma(x) = x$ *对于所有* $\sigma \in \Gamma$ 是必要且充分的。 *For a vector sub-N-space* $W$ *of* $V$ *to be rational over* $K$ *it is necessary and sufficient that* $u_\sigma(W) \subset W$ *for all* $\sigma \in \Gamma$.

*b)* *设* $V_1$ *和* $V_2$ *是两个向量空间超过* $N$，*每个都有一个* $K$-*结构*。 *对于线性映射* $f$ *的* $V_1$ *进入* $V_2$ *要理性地超过* $K$ *有充分必要* $f(u_\sigma(x)) = u_\sigma(f(x))$ *对于所有* $\sigma \in \Gamma$ *和所有* $x \in V_1$。

*很明显，$K$*是*$x \in N$*的集合*使得*$\sigma(xy) = x \sigma(y)$*对于所有*$\sigma \in \Gamma$*和所有*$y \in N$。 *命题因此由 Th 得出。 1*（II，p. 324）。

#### 推论{#alg-v-s10-n4-cor-1 .statement tag=06MQ}

— 令$V_0$为$K$上的向量空间，并令$W$为$N \otimes_K V_0$的向量子N空间。假设对于所有 $\sigma \in \Gamma$，$W$ 在映射 $\sigma \otimes \mathrm{Id}_{V_0}$ 下是稳定的。令$W_0$为$x \in V_0$的集合，使得$1 \otimes x \in W$；那么$W_0$是$V_0$的唯一向量子K空间，使得$W = N \otimes_K W_0$。

注形式 $1 \otimes x \ (x \in V_0)$ 的元素的集合是$N \otimes_K V_0$ 上的K 结构就足够了，对于$\sigma \in \Gamma$，我们有$u_\sigma = \sigma \otimes \mathrm{Id}_{V_0}$。

#### 命题 7 {#alg-v-s10-prop-7 .statement tag=06MR}

— 令$V$在$N$、$(u_\sigma)_\sigma$上成为向量空间，将$V$的映射组成的族纳入自身满足 (1) 至(4) 和$x \in V$的$V_0$集合，使得$u_\sigma(x) = x$对于所有$\sigma \in \Gamma$。

a) $V_0$是$V$的向量子K空间和$N \otimes_K V_0$的K-线性映射$\varphi$进入$V$，其中映射$\lambda \otimes x$到$\lambda x$是单射的。

b) 如果 $\Gamma$ 是有限的，则 $\varphi$ 是双射的，$V_0$ 是 $V$ 上的 K 结构。

显然$V_0$是$V$的向量子K空间。

公式$u_\sigma \circ \varphi = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0})$表明$\varphi$的核$W$在映射$\sigma \otimes \mathrm{Id}_{V_0}$下是稳定的；由科。根据命题6，因此存在$V_0$的子空间$W_0$使得$W = N \otimes_K W_0$。如果$x$属于到$W_0$，我们就有$x = \varphi(1 \otimes x) = 0$，因此$W_0 = 0$，所以$W = 0$。这就证明了a）。

现在假设 $\Gamma$ 是有限的；我们必须证明 $\varphi$ 是满射的，或者等效于 $V_0$ 生成向量 N 空间 $V$。因此，让$f$是$V$上的N线性形式，其限制到$V_0$是零。设 $x \in V$；对于$V$的每个$\lambda \in N$元素$y_\lambda = \sum_{\sigma \in \Gamma} u_\sigma(\lambda x)$，显然属于到$V_0$，从而$f(y_\lambda) = 0$，即
$$
\sum_{\sigma \in \Gamma} f(u_\sigma(x)) \sigma(A) = 0.
$$
根据 Dedekind 的定理 (V, p. 27, Cor. 2)，因此对于每个$\sigma \in \Gamma$，我们有 $f(u_\sigma(x)) = 0$；特别是，取$\sigma = \varepsilon$，我们找到$f(x) = 0$，这意味着$f = 0$。这证明了b)。

设 $M$ 为向量空间大于 $N$；对于每个$\sigma \in \Gamma$，令$M^\sigma$为向量空间超过$N$，具有与$M$相同的基础加法群，以及外法则$(A, x) \mapsto \sigma(\lambda) x$。写$V = \prod_{\sigma \in \Gamma} M^\sigma$； $V$的底层加法群是$\Gamma$到$M$的所有映射，其中外法则定义为
$$
(\lambda . h)(\sigma) = \sigma(\lambda) h(\sigma) \quad (\lambda \in N, h \in V, \sigma \in \Gamma).
$$
（乘积 $\sigma(\lambda) h(\sigma)$ 是在向量空间 $M$ 中计算的。）此外，我们在 $N \otimes_K M$ 向量空间结构上比$N$ 公式定义
$$
\lambda \left( \sum_i \mu_i \otimes x_i \right) = \sum_i \lambda \mu_i \otimes x_i
$$
最后我们将$N \otimes_K M$的$\psi$K-线性映射表示为$V$，其特征为关系
$$
\psi(\lambda \otimes x)(\sigma) = \sigma(\lambda) . x
$$
对于 $A \in N, x \in M$ 和 $\sigma \in \Gamma$。显然 $\psi$ 是 N 线性的

#### 命题 8 {#alg-v-s10-prop-8 .statement tag=06MS}

— *N-线性映射* $\psi$ *of* $N \otimes_K M$ *到* $V = \prod_{\sigma \in \Gamma} M^\sigma$ *是单射的，并且如果* $\Gamma$ *是有限的，那么它是双射的。*

对于每个 $a \in \Gamma$，我们将 $V$ 的定义映射 $u_\sigma$ 转换为 $V$

$$
(u_\sigma h)(\tau) = h(\tau \sigma)
$$

对于 $h \in V$ 和 $\tau \in \Gamma$。 *(1)-(4)*的验证为直接的。用$h \in V$的$V$、集合表示，使得$u_\sigma(h) = h$适用于所有$\sigma \in \Gamma$。对于每个$x \in M$，令$\theta(x)$为$\Gamma$到$M$的常数映射，其中值$x$；那么$\theta$是$M$到$V$的K同构。如果我们如上所述定义同态 $\varphi : N \otimes_K V, \to V$，我们就有 $\psi = \varphi \circ (\mathrm{Id}_N \otimes \theta)$，现在第 8 条提案是从第 7 条提案得出的。

#### 推论{#alg-v-s10-n4-cor-2 .statement tag=06MT}

— *让* $\psi$ *成为* $N \otimes_K N$ *的K-线性映射 *进入乘积向量空间* $N^\Gamma$ *使得* $\psi(x \otimes y)\,(a) = \sigma(x)\,y$ *对于* $x,\,y$ *在* $N$ *和* $\sigma \in \Gamma$。 *那么* $\psi$ *是单射的，并且当* $\Gamma$ *是有限的时，它是双射的。*

这是第 8 条提案的特殊情况$M = N$。

#### 注 1 {#alg-v-s10-n4-rem-1 .statement tag=06MU}

令F是K的扩张和$N$F的子扩展，并令$\Gamma$是$N$的自同构的*有限*群，其中K是不变量的域。命题 8 暗示存在 K-代数 $0 : N \otimes_F F \to F^\Gamma$ 的同构，其特征在于 $x \in N,\,y \in F$ 和 $\sigma \in \Gamma$ 的$\theta(x \otimes y)\,(a) = \sigma(x)\,y$。

#### 注 2 {#alg-v-s10-n4-rem-2 .statement tag=06MV}

记号 K、N 和$\Gamma$ 与之前含义相同。对于每个整数$n \geqslant 1$，令$A_n$为与$N$相同的n个K-代数中的张量积；设$B_n$为$N$为$\Gamma^{n-1}$映射集合。通过 $n$ 上的归纳，我们可以从 Cor 中推出。提案 8 中存在同构 $\varphi_n : A_n \to B_n$、映射 $x_1 \otimes \ldots \otimes x_n$ 至函数 $(\sigma_1, \ldots, a, ) \quad \sigma_1(x_1) \cdot \sigma_n(x_{n-1})\,x_n$。

### 5. *伽罗瓦上同调*

令$N$为域，$\Gamma$$N$的自同构的*有限*群和$\Gamma$的不变量K域。对于每个整数$n \geqslant 1$，我们用阶$n$的方阵的$\mathbf{GL}(n, N)$群表示，系数在$N$和非零行列式（II；p. 349）。我们让群$\Gamma$按照规则$\sigma(A) = (\sigma(a_{ij}))$对$A = (a_{ij})$操作群$\mathbf{GL}(n, N)$。

#### 命题 9 {#alg-v-s10-prop-9 .statement tag=06MW}

— *让* $(U_\sigma)_{\sigma \in \Gamma}$ *成为* $\mathbf{GL}(n, N)$ 的元素家庭。 *对于* $A$ *存在于* $GL(n, N)$ *使得* $U_\sigma = A^{-1}\,a(A)$ *对于所有* $\sigma \in \Gamma$ *有充分必要* $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ *对于* $\sigma,\,\tau$ *在* $\Gamma$。

条件是*必要的*：如果$U_\sigma = A^{-1}\,a(A)$，那么我们有

$$
U_\sigma \cdot \sigma(U_\tau) = A^{-1}\,\sigma(A)\,\sigma(A^{-1}\,\tau(A)) = A^{-1}\sigma\tau(A) = U_{\sigma \tau}.
$$

条件 *足够*：我们 $N^n$ 的认同元素，其中矩阵 $n$ 行和一个列，系数在 $N$ 中。我们让群$\Gamma$作用于$N^n$：
$$
\sigma(x) = (\sigma(x_i))_{1 \leq i \leq n} \quad \text{for} \quad x = (x_i)_{1 \leq i \leq n}.
$$
对于每个 $a \in \Gamma$，我们将 $N^n$ 的 $u_\sigma$ 映射 $x \mapsto U_\sigma \cdot \sigma(x)$ 表示为自身。 V、p. 62的公式(1)至(3)验证为直接的。此外，我们有$u_\varepsilon \circ u_\varepsilon = u_\varepsilon$，并且由于$u_\varepsilon$是双射，所以我们有$u_\varepsilon = \mathrm{Id}_{N^n}$。令$V_0$为向量$x \in N^n$中的集合，使得$u_\sigma(x) = x$对于所有$\sigma \in \Gamma$。根据命题7（V，p. 63），$V_0$是$N^n$上的K结构；特别是存在$V_0$向量$b_1, \ldots, b_n$，在$N$上形成$N^n$的基。因此，矩阵 $B$ 与列 $b_1, \ldots, b_n$ 是可逆的，关系 $u_\sigma(b_i) = b_i$ 对于 $1 \leq i \leq n$ 相当于 $U_\sigma \cdot \sigma(B) = B$。写出$A = B^{-1}$，我们得到所有$a \in \Gamma$的$U_\sigma = A^{-1} \sigma(A)$。

#### 推论 1 {#alg-v-s10-prop-9-cor-1 .statement tag=06MX}

*令$(c_\sigma)_{\sigma \in \Gamma}$为$N$的非零元素族。为了使$a \neq 0$存在于$N$中，使得$c_\sigma = \sigma(a) \cdot a^{-1}$对于所有$\sigma \in \Gamma$来说，$c_{\sigma \tau} = c_\sigma \cdot \sigma(c_\tau)$对于$\Gamma$中的$\sigma, \tau$来说是必要且充分的。*

#### 推论 2 {#alg-v-s10-prop-9-cor-2 .statement tag=06MY}

*令$(a_\sigma)_{\sigma \in \Gamma}$为元素和$N$的家庭。对于$b$存在于$N$中，使得$a_\sigma = \sigma(b) - b$对于所有$\sigma \in \Gamma$来说，$a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$对于$\Gamma$中的$\sigma, \tau$来说是充分必要的。*

对于$N$中的所有$b$和$\Gamma$中的$\sigma, \tau$，我们都有$\sigma \tau(b) - b = [\sigma(b) - b] + \sigma[\tau(b) - b]$，从而是必要性。

相反，假设$a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$对于$\Gamma$中的任何$\sigma$和$\tau$。将$U_\sigma = \begin{pmatrix} 1 & a_\sigma \\ 0 & 1 \end{pmatrix}$换成$\sigma \in \Gamma$；那么我们在$\Gamma$中有$U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$对应$\sigma, \tau$；根据命题 9，因此存在矩阵 $A = \begin{pmatrix} x & y \\ z & t \end{pmatrix}$ 且行列式非零，使得 $\sigma(A) = A U_\sigma$ 对于所有 $a \in \Gamma$；写下关系 $\sigma(A) = A U_\sigma$ 我们发现
$$
\begin{pmatrix} \sigma(x) & \sigma(y) \\ \sigma(z) & \sigma(t) \end{pmatrix} = \begin{pmatrix} x & x a_\sigma + y \\ z & z a_\sigma + t \end{pmatrix} \quad (\sigma \in \Gamma).
$$
特别是，$x$和$z$属于到$K$，我们有
$$
\sigma(y) = x a_\sigma + y, \quad \sigma(t) = z a_\sigma + t \quad (\sigma \in \Gamma).
$$
如果$x \neq 0$我们有$a, = \sigma(b) - b$和$b = x^{-1} y$；如果$z \neq 0$，我们有与$b = z^{-1} t$相同的关系。现在 $x$ 和 $z$ 不能都是零因为
$$
xt - yz = \det A \neq 0.
$$

### 6.阿丁的定理

#### 定理 2（阿丁）{#alg-v-s10-thm-2 .statement tag=06MZ}

— *令$N$为域，$N$的自同构的$\Gamma$群以及$\Gamma$的不变量$K$域。设$V$是有限维*的$N$在K上的向量子K空间。那么V的每个K-线性映射u进入N是线性组合，N中的系数为限制到V 元素共 $\Gamma$。

设u为N中V的K-线性映射，并令$V_{(N)} = N \otimes_K V$为从V通过扩张标量导出的向量N空间；用 $\tilde{u}$ 表示 $V_{(N)}$ 上的 N 线性形式，使得 $\tilde{u}(x \otimes y) = x \cdot u(y)$ 代表 $x \in N$ 和 $y \in V$。对于每个$a \in \Gamma$，在$V_{(N)}$上都存在一个N线性形式h，使得$h_\sigma(x \otimes y) = x \sigma(y)$对于$x \in N$和$y \in V$。 $V_{(N)} = N \otimes_K V$到$N \otimes_K N$的典范映射是单射的。现在科。命题8（V，p. 64）表明线性形式 h的核在$V_{(N)}$上的交减少到0。因此（II，p. 302，Cor.1）存在$a_1, \ldots, \sigma_n$ $\Gamma$和$a_1, \ldots, a_n$在$N$中，使得$\tilde{u} = \sum_{i=1}^n a_i h_{\sigma_i}$从而$u(x) = \sum_{i=1}^n a_i \sigma_i(x)$对于所有$x \in V$。

让我们用因子的离散拓扑的乘积拓扑将N的所有映射中的集合$N^N$装备到N中。 Th。 2 表示线性组合的集合的系数位于 $\Gamma$ 的元素的 N 中，在 N 的 K-线性映射的集合中稠密。

#### 定理 3 {#alg-v-s10-thm-3 .statement tag=06N0}

— 令 N 为 N 的域、N 的自同构的 $\Gamma$ 有限群，以及 $\Gamma$ 的不变量的 K 域。设 n 为 $\Gamma$ 的基数。
a) 我们有$[N : K] = n$，N 是K 的伽罗瓦扩张，其中伽罗瓦群 $\Gamma$。
b) 令 $\sigma_1, \ldots, \sigma_n$ 为 $\Gamma$ 的元素和 N 除以 K 的 $(x_1, \ldots, x_n)$ 基，然后为 $\det (\sigma_i(x_j)) \neq 0$。
c) 让 u 成为 N 中的 K-线性映射。存在 N 的元素的唯一族$(a_\sigma)_\sigma$，使得$u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ 对于所有 $x \in N$。

我们用 N 代数结构装备环 $N \otimes_K N$，其外法则由 N 中$\lambda, x, y$ 的 $\lambda(x \otimes y) = x \otimes \lambda y$ 给出。则向量 N 空间 $NO, N$ 的维数为 $[N : K]$。 乘积向量 N 空间 $N^\Gamma$ 的维数等于 n。 映射 $\psi$ 在 Cor 中定义。命题 8 (V, p. 64) 是 $NO, N$ 到 $N^\Gamma$, 从而 $[N : K] = n$ 的 N 同构。设A是N的K-自同构的群。我们有$\Gamma \subset A$，因此K是A的不变量的域，N是K的伽罗瓦扩张。此外，根据戴德金的定理，A的阶至多等于$[N : K]$ （V，p. 27，Cor.2）并且由于$\Gamma$的阶等于$[N : K]$，我们有$\Gamma = A$。因此$\Gamma$是N除以K的伽罗瓦群，这证明了a)。

将b)的记号放入$f_i = \psi(x_i \otimes 1)$；我们有 $f_i(\sigma) = \sigma(x_i)$ 对应 $1 \leq i \leq n$ 和 $\sigma \in \Gamma$。由于$\psi$是向量N空间的同构，序列$(f_1, \ldots, f_n)$是N除以N的基，从而$\det (f_j(\sigma_i)) \neq 0$，即

$$
\det (\sigma_i(x_j)) \neq 0
$$

这证明了b)。

最后，c) 由 Th 得出。 2（V，p. 65）证明了一个族$(a_\sigma)_{\sigma \in \Gamma}$的存在，使得$u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$（对于所有$x \in N$）和来自Dedekind的定理（V，p. 27，Cor.2）证明唯一性共 $(a_\sigma)_{\sigma \in \Gamma}$。

### 7. 伽罗瓦理论的基础定理

#### 定理 4 {#alg-v-s10-thm-4 .statement tag=06N1}

— 令 N 为 K 的伽罗瓦扩张，且 $\Gamma$ 为伽罗瓦群。令$\mathscr{K}$为N的子扩张的集合，以及$\Gamma$的闭子群的$\mathscr{G}$集合。对于每个子群$A \in \mathscr{G}$，我们用A的不变量$k(\Delta)$域表示，对于每个*子域*$E \in \mathscr{K}$，我们用N的E-*自同构*的$g(E)$群表示。*然后* $A \mapsto k(\Delta)$ 是$\mathscr{G}$ 到$\mathscr{K}$ 的双射，$E \mapsto g(E)$ 是逆双射。

A) 关系 $E = k(g(E))$（对于$E \in \mathscr{K}$）是以下更精确的引理中的推论：

#### 引理 1 {#alg-v-s10-lem-1 .statement tag=06N2}

设 E 是 N 的子扩张。那么 N 是 E 的伽罗瓦扩张，$\mathrm{Gal}(N/E)$ 是 $\mathrm{Gal}(N/K)$ 的闭子群以及导出的拓扑。

设 $x \in N$； $E[X]$ 中 x 在 E 除上的最小多项式 f x 在 K 上的最小多项式 $g$（V，p. 17，Cor. 2）。由于 N 是 K 上的伽罗瓦，因此多项式 g 是次数 1 的不同因子的 $N[X]$ 中的乘积；因此 f 也是如此，因此 N 是 E 上的伽罗瓦。

令$\Gamma$是N在K上的伽罗瓦群，A是N在E上的伽罗瓦群。通过定义，A是所有$\sigma$的$\Gamma$由……组成的子群，使得$\sigma(x) = x$对于所有$x \in E$。现在，对于 $\Gamma$ 的每个 $x \in E$ 映射 $\sigma \mapsto \sigma(x)$ 到离散空间中，N 是连续的，因此 D 在 $\Gamma$ 中是封闭的。让$\sigma \in \Gamma$；对于N中的$x_1, \ldots, x_n$，令$U(x_1, \ldots, x_n)$为所有$\tau \in \Gamma$中的集合，使得$\tau(x_i) = \sigma(x_i)$对于$1 \leq i \leq n$；把

$$
V(x_1, \ldots, x_n) = U(x_1, \ldots, x_n) \cap \Delta.
$$

那么集合$U(x_1, \ldots, x_n)$（分别$V(x_1, \ldots, x_n)$）的家族是$\Gamma$（分别A）中$\sigma$的邻域的基。因此A上的拓扑是由$\Gamma$引起的。

B) 关系 $A = g(k(\Delta))$（对于$A \in g$）是以下更精确的引理中的推论：

#### 引理 2 {#alg-v-s10-lem-2 .statement tag=06N3}

设 A 为 $\Gamma$ 的子群。令 E 为 A 的不变量的域；那么 N over E 的伽罗瓦群就是 A 在 $\Gamma$ 中的闭包。

N 在 E 上的伽罗瓦群在 $\Gamma$ (引理 1) 和包含 A 中闭合，因此包含 A 的闭包 $\bar{\Delta}$。令 $\sigma$ 为 N 的 E 自同构，并令 $x_1, \ldots, x_n$ 在 N 中。因为 N 是 E 上的伽罗瓦(引理 1) 存在 (V, p. 57, 命题 2) N 的子扩张 $N_0$，伽罗瓦在 E 上的有限次数和包含 $x_1, \ldots, x_n$。设$A_0$为$\mathrm{Gal}(N_0/E)$下$\mathrm{Gal}(N/E)$的限制同态下$\mathrm{Gal}(N/E)$的子群A像。由于$[N_0 : E]$是有限的，戴德金的定理（V，p. 27，Cor.2）表明$\mathrm{Gal}(N_0/E)$是有限的。因此$A_0$是有限的，并且由于E是$A_0$的不变量的域，所以我们有$\Delta_0 =$

Gal(N_0/E) (V、p. 66、Th.3)。特别是，$\sigma$至$N_0$中的$\Delta_0$包含限制。因此，存在$\tau \in A$使得$\sigma$和$\tau$具有相同的限制至$N_0$、从而$\sigma(x_1) = \tau(x_1), \ldots, \sigma(x_n) = \tau(x_n)$。由此可见，$\sigma$ 是$\Gamma$ 中$A$ 的极限点，因此是$\mathrm{Gal}(N/E) \subset \overline{\Delta}$。

#### 推论 1 {#alg-v-s10-lem-2-cor-1 .statement tag=06N4}

*设E和E'为N包含K中的两个子域；则 E $\subset$ E' 当且仅当 g(E) $\supset$ g(E')。如果 A 和 A' 是 $\Gamma$ 的两个闭子群，则 A $\subset$ A' 当且仅当 k($\Delta$) $\supset$ k($\Delta'$)。*

对于两个逆双射 $E \rightleftharpoons g(E)$ 和 $A \rightleftharpoons k(\Delta)$ 是包含反转的。

#### 推论 2 {#alg-v-s10-lem-2-cor-2 .statement tag=06N5}

*令$(E_i)_{i \in I}$为子域、N包含K的家庭；输入$L = \bigcap_{i \in I} E_i$和$M = K\left( \bigcup_{i \in I} E_i \right)$。那么g(L)是最小的闭子群的包含$U_{i \in I} g(E_i)$，我们有$g(M) = \bigcap_{i \in I} g(E_i)$。*

第一个断言来自Cor。 1，第二个是直接的。

#### 推论 3 {#alg-v-s10-lem-2-cor-3 .statement tag=06N6}

*对于 i = 1, 2，令 $E_i$ 为 N 包含 K 的子域，并令 $\Delta_i = g(E_i)$。对于任何 $\sigma \in \Gamma$ 关系 $\sigma(E_1) = E_2$ 和 $\sigma \Delta_1 \sigma^{-1} = \Delta_2$ 都是等价的。*

因为我们有$\tau \in g(\sigma(E_1))$当且仅当$\tau \sigma(x) = \sigma(x)$，即$\sigma^{-1} \tau \sigma(x) = x$，对于所有$x \in E_1$；这相当于说 '即 $\sigma^{-1} \tau \sigma \in \Delta_1$、从而 $g(\sigma(E_1)) = \sigma \Delta_1 \sigma^{-1}$。

#### 推论 4 {#alg-v-s10-lem-2-cor-4 .statement tag=06N7}

*设 E 为 N 包含 K 的子域，并设 $A = g(E)$。为了使 E 成为 K 上的伽罗瓦，A 应该是 $\Gamma$ 的正规子群是充分必要的。在这种情况下，将 $\Gamma$ 的限制同态代入 $\mathrm{Gal}(E/K)$ 定义，通过商将 $\Gamma / \Delta$ 的拓扑群同构代入 $\mathrm{Gal}(E/K)$。*

由于 N 在 K 上可分，因此 E 也是如此（V，p. 36，命题 1）。因此，E 是 K 上的伽罗瓦当且仅当它是 K 上的拟伽罗瓦；这也意味着$\sigma(E) = E$对于N的每个K-自同构$\sigma$（V，p. 52，命题1和p. 54，命题3）。由科. 3 这相当于所有 $\sigma \in \Gamma$ 的 $\sigma \Delta \sigma^{-1} = A$。

限制同态 $\varphi : \mathrm{Gal}(N/K) \to \mathrm{Gal}(E/K)$ 是连续且满射的（V、p. 60，命题 3），且其核显然等于 $A = \mathrm{Gal}(N/E)$。由于$\Gamma$是紧的，$\Gamma / \Delta$到$\mathrm{Gal}(E/K)$的同态通过商的方式从$\varphi$导出，是拓扑群的同构（Gen.Top.，I，p. 87，Cor.2）。

#### 推论 5 {#alg-v-s10-lem-2-cor-5 .statement tag=06N8}

*设 E 为 N 包含 K 的子域。对于 E 的有限次数超过 K，g(E) 在 $\Gamma$ 中开是充分必要的。当这种情况发生时，指标 $(\Gamma : g(E))$ 是有限的并且等于 [E : K]。*

为了使$g(E)$开，存在N的子扩展F、有限次数在K上的子扩展F是必要且充分的，使得在V的记号中，p. 60。

g(E)包含$U_F(\mathrm{Id}_N) = g(F)$。 关系 $g(E) \supset g(F)$ 相当于 Cor 的 $E \subset F$。 1 (V, p. 68), 从而 Cor 的第一个断言。 5.

假设 $[E : K]$ 是有限的。设$\Omega$为$K$包含$N$的代数闭包作为子外延（V，p. 23，Th.2），并令$\mathscr{H}$为$K$的集合-同态$E$ 变为$\Omega$。 $\mathscr{H}$的每个元素都是由$\Omega$的$K$自同构引起的（V，p. 52，命题1），并且由于$N$是$K$，映射的拟伽罗瓦$\Gamma$到$\mathscr{H}$的$\sigma \mapsto \sigma|_E$是满射。为了使$\Gamma$中的$\sigma$和$\sigma'$具有相同的限制至$E$，$\sigma^{-1}\sigma' \in g(E)$、从而卡$A? = (\Gamma : g(E))$是充分必要的。最后，由于 $E$ 是 $K$ 的 etale 代数，我们有卡片 $\mathscr{H} = [E : K]$（V，p. 32，命题 4），所以结论是我们有 $(\Gamma : g(E)) = [E : K]$。

#### 推论 6 {#alg-v-s10-lem-2-cor-6 .statement tag=06N9}

— 对于$i = 1, 2$，令$E_i$为$N$的$N$和$\Gamma_i$伽罗瓦群在$E_i$上的子扩展。以下条件是等效的：
a) 群 $\Gamma$ 是子群 $\Gamma_1$ 和 $\Gamma_2$ 的直接乘积。
b) 扩张 $E_1$ 和 $E_2$ 是 $K$ 上的伽罗瓦，我们有 $E_1 \cap E_2 = K$ 和
$$
K(E_1 \cup E_2) = N .
$$

为了使$\Gamma$成为子群、$\Gamma_1$和$\Gamma_2$的直接乘积，以下条件成立是必要且充分的（I，p. 48，命题15）：
(i) 子群、$\Gamma_1$和$\Gamma_2$在$\Gamma$中是正常的；
(ii) $\Gamma_1 \cap \Gamma_2 = \{ \varepsilon \}$，其中$\varepsilon$是$\Gamma$的中性元素；
（三）$\Gamma = \Gamma_1 . \Gamma_2$。

现在 (i) 意味着 $E_1$ 和 $E_2$ 是 $K$ 上的伽罗瓦 (Cor. 4)。由科. 2、条件(ii)等价于$N = K(E_1 \cup E_2)$，最后如果(i)和(ii)成立，则$\Gamma_1 \Gamma_2$是$\Gamma$包含$\Gamma_1 \cup \Gamma_2$中最小的子群；它是封闭的，因为$\Gamma_1$和$\Gamma_2$是紧致的，并且$\Gamma_1 \times \Gamma_2$到$\Gamma$的映射$(a, \tau) \mapsto \sigma \tau$是连续的（Gen.Top.，I，p. 63，Cor.1）。科。现在图2表明(iii)等于$E_1 \cap E_2 = K$，这证明了a)和b)的等价。

#### 注 {#alg-v-s10-n7-rem-1 .statement tag=06NA}

与Cor的记号。 6 假设条件 a) 和 b) 成立。 限制同态 $\varphi_i : \Gamma \to \mathrm{Gal}(E_i/K)$ 对于 $i = 1, 2$ 诱导拓扑群同构
$$
\Psi_1 : \Gamma_2 \to \mathrm{Gal}(E_1/K) , \quad \Psi_2 : \Gamma_1 \to \mathrm{Gal}(E_2/K)
$$
通过a)我们看到映射$\sigma \mapsto (\varphi_1(\sigma), \varphi_2(\sigma))$是$\mathrm{Gal}(N/K)$到$\mathrm{Gal}(E_1/K) \times \mathrm{Gal}(E_2/K)$的拓扑群同构。

### 8.基域变换

令$N$为$K$之伽罗瓦扩张且$N$之$\Gamma$伽罗瓦群超过$K$；进一步令$N'$为$K'$的伽罗瓦扩张和伽罗瓦群$\Gamma'$。 我们将认同$K$（或$K'$）及其像放在$N$（或$N'$）中。 设$u$为$K$的同态入$K'$，$v$同态入$N$入$N'$，其限制至$K$等于$u$（cf.）

图1）。设 $\sigma \in \Gamma'$；由于$u(K) \subset K'$，$a$是$N'$的$u(K)$自同构；此外，$v(N)$是$u(K)$的伽罗瓦扩张，因此$a$诱导是$v(N)$的$u(K)$自同构（V，p. 55，注1）。在其他字中，对于每个$\sigma \in \Gamma'$，都存在$\Gamma$的唯一元素$v^*(\sigma)$，使得

(8)

$$
v \circ v^*(\sigma) = \sigma \circ v .
$$

![图表显示 N, N', K, K' 之间的映射 v 和 u]（图 1）

映射 $v^*$ 是 $\mathrm{Gal}(N'/K')$ 的同态到 $\mathrm{Gal}(N/K)$。对于每个$x \in N$，$\Gamma'$的映射$a \mapsto v^*(o)(x) = v^{-1}(\sigma(v(x)))$进入离散空间$N$是连续的，因此$v^*$是连续的。

三个特殊情况很重要：

a) 如果$F$是$K$的伽罗瓦扩张并且$E$是$F$的子扩展，我们知道（V，p. 67，引理1）$F$是$E$的伽罗瓦扩张。让我们将上述内容应用到$N = F$、$K' = E$、$N' = F$和$v = \mathrm{Id}_F$的情况。那么$v^*$仅仅是典范嵌入

$$
j : \mathrm{Gal}(F/E) \to \mathrm{Gal}(F/K) .
$$

这就是有时，称为膨胀同态。

b) 假设在加法 $E$ 中，伽罗瓦在 $K$ 上。让我们将上述内容应用到$N = E$、$K' = K$、$N' = F$和$v$是$E$的典范嵌入到$F$的情况。那么$v^*$就是限制同态

$$
\pi : \mathrm{Gal}(F/K) \to \mathrm{Gal}(E/K)
$$

我们知道（V，p. 60，命题 3）$\pi$ 是满射，核 $\mathrm{Gal}(F/E)$ 并且通过取商可以将定义 $\mathrm{Gal}(F/K)/\mathrm{Gal}(F/E)$ 的拓扑群同构推到 $\mathrm{Gal}(E/K)$ (V， p. 68，Cor.4）。

c) 假设$v^{-1}(K') = K$和$N' = K'(v(N))$；让我们证明同态

$$
v^* : \mathrm{Gal}(N'/K') \to \mathrm{Gal}(N/K) ,
$$

是一个拓扑群同构、有时，称为平移。由于群$\mathrm{Gal}(N'/K')$是紧致的，群$\mathrm{Gal}(N/K)$是分离的，$v^*$是连续的；因此足以证明 $v^*$ 是双射的（Gen. Top., I, p. 87, Cor. 2）。现在$v^*$的核的每个元素$\sigma$都是$N'$的自同构，其中诱导是$K'$和$v(N)$上的恒等式，因此是$a = \epsilon$，因为$N' = K'(v(N))$；由此可见 $v^*$ 是单射的。此外，$v^*$的像是$\mathrm{Gal}(N/K)$的闭子群$A$

（Gen. Top.，I，p. 81，*同上。*）$A$的不变量域等于$v^{-1}(K') = K$；因此我们有 $A = \mathrm{Gal}(N/K)$ (V, p. 67, Th. 4)，所以 $v^*$ 是满射。

一般情况可以减少合成。首先我们注，$K'(v(N))$是$v^*$核$A$$N'$中的不变量域；因为$A$是$\mathrm{Gal}(N'/K')$的正规子群，$K'$的扩张$K'(v(N))$是Galois（V，p. 68，Cor.4）。因此$v^*$由同态组成

$$
\mathrm{Gal}(N'/K') \to \mathrm{Gal}(K'(u(N))/K') \xrightarrow{\psi} \mathrm{Gal}(N/v^{-1}(K')) \xrightarrow{j} \mathrm{Gal}(N/K);
$$

在这个序列$\pi$是限制同态与三元组$K' \subset K'(u(N)) \subset N'$相关联，$\psi$是与图表的中心平方相关联的翻译同构（图2），$j$是与膨胀同态相关联三倍$K \subset v^{-1}(K') \subset N$。

接下来的定理给出了关于翻译同构的结构的更多详细信息。

![图表显示扩张和翻译](fig2.png)

图2

#### 定理 5 {#alg-v-s10-thm-5 .statement tag=06NB}

*令$N'$为由两个子扩展$K'$和$N$生成的$K$的扩张。假设 $N$ 是 $K$ 上的伽罗瓦，其中伽罗瓦群 $\Gamma$ 以及 $K' \cap N = K$。那么$K'$的扩张$N'$就是伽罗瓦，$K' \otimes_K N$的典范同态$\varphi$到$N'$就是同构。令 $\sigma \in \mathrm{Gal}(N/K)$ 并令 $\sigma'$ 为 $\mathrm{Gal}(N'/K')$ 的元素，其中对应在翻译同构下；那么我们就有 $\sigma' \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes u)$.*

我们有 $N' = K'(N)$ 且 $N$ 是代数且可在 $K$ 上分离；因此（V，p. 42，命题10），$K'$的扩张$N'$是代数且可分的。由科. V、p. 54、扩张、$K'$的$N'$中的4个是拟伽罗瓦。因此$K'$的扩张$N'$是伽罗瓦。通过c)，上面的映射$\sigma \mapsto \sigma|_N$是$\mathrm{Gal}(N'/K')$的同态$\lambda$到$\mathrm{Gal}(N/K)$。

我们有$N = K'[N]$，因为$N$是$K$的代数（V，p. 18，Cor.1），因此$\varphi$是满射。如果 $a$ 属于到 $\mathrm{Gal}(N/K)$，我们有

$$
\lambda^{-1}(\sigma) \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes \sigma).
$$

因此，$\varphi$的核在映射$\mathrm{Id}_{K'} \otimes \sigma$下是稳定的，因此形式$K' \otimes_K N_0$与$N_0 \subset N$（V，p. 63，Cor.）。对于$N_0$中的$x$，我们有$x = \varphi(1 \otimes x) = 0$，因此$N_0 = 0$，因此$\varphi$是单射的。

#### 推论 1 {#alg-v-s10-thm-5-cor-1 .statement tag=06NC}

*令$E'$为$N'$包含$K'$中的子域。存在唯一的子域 $E$ $N$ 包含 $K$ 以及 $E' = K'(E)$。我们有$E = E' \cap N$。*

输入$E = E' \cap N$，然后输入$E' \supset K'(E)$。现在类似地放置$\Gamma = \mathrm{Gal}(N/K)$和$A = \mathrm{Gal}(N/E)$，以及定义$\Gamma'$和$A'$。 映射$A : a \mapsto a|_N$是$\Gamma'$到$\Gamma$的同构，也是$A'$到$A$的同构；在其他字中，$A'$由那些$\sigma \in \Gamma'$组成，其中$\lambda(\sigma)$属于到$A$。如果$\sigma \in \Gamma'$使$K'(E)$的元素固定，则$\lambda(\sigma) \in A$、从而$a \in A'$和$a$使$E'$的元素固定；由科. V、p. 68 中的 1 个，因此我们有 $K'(E) \supset E'$。

我们已经证明了等式$E' = K'(E)$、从而$\varphi^{-1}(E') = K' \otimes_K E$。如果$F$是$N$包含$K$的子域并且$E' = K'(F)$，我们同样有$\varphi^{-1}(E') = K' \otimes_K F$，从而$F = E$。

#### 推论 2 {#alg-v-s10-thm-5-cor-2 .statement tag=06ND}

*令$N$为$K$中的伽罗瓦扩张。假设$N$在$K$上的伽罗瓦群$\Gamma$是两个闭子群$\Gamma_1$和$\Gamma_2$的直乘积，并用$E_i$域的不变量表示$\Gamma_i$ 换$i = 1, 2$。那么$E_1 \otimes_K E_2$到$N$的典范同态就是同构。*

我们有 Cor 的 $E_1 \cap E_2 = K$ 和 $N = K(E_1 \cup E_2)$。 6 (V, p. 69)，因此应用定理 5 就足够了。

#### 注 {#alg-v-s10-n8-rem-1 .statement tag=06NE}

令$K$和$K'$为$K$的两个域和$u$同态到$K'$。设$K_s$（$K'_s$）为$K$（$K'$）的可分闭包（V，p. 45，命题14）和$\Pi$（$\Pi'$）伽罗瓦群 $K_s$超过$K$（或$K'_s$超过$K'$）。由于$K_s$是$K$的可分代数扩张且$K$的扩张$(K'_s, u)$是可分闭代数，因此存在(V, p. 45, Cor.)同态$v$ $K_s$ 进入$K'_s$ 延伸$u$。从$v$我们获得$\Pi'$到$\Pi$的连续同态$v^*$。设$v_1$为$u$的另一个扩张；由于$K_s$是$K$的准伽罗瓦扩展，因此存在$\Pi$的元素$a_s$使得$v_1 = v \circ a_s$。我们结论为所有$\tau \in \Pi$提供$v_1^*(\tau) = \sigma_0^{-1} v^*(\tau) \sigma_0$。

### 9.正常基定理

令$N$为$K$的伽罗瓦扩张，其中伽罗瓦群$\Gamma$。我们认同$\Gamma$与典范基群代数$K^{(\Gamma)}$（III，p. 446）；那么$N$可以被认为是左$K^{(\Gamma)}$-模块（III，p. 447，例），这样

$$
u \cdot x = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x) \quad \text{for} \quad x \in N \quad \text{and} \quad u = \sum_{\sigma \in \Gamma} a_\sigma \sigma \quad \text{in} \quad K^{(\Gamma)}.
$$

如果$N$是有限次数超过$K$，群$\Gamma$由戴德金的定理有限（V，p. 27，Cor.2），我们可以定义元素 $t = \sum_{\sigma \in \Gamma} a$ $K^{(\Gamma)}$；那么我们有

$$
\mathrm{Tr}_{N/K}(x) = \sum_{\sigma \in \Gamma} \sigma(x),
$$

也就是说，对于所有 $x \in N$，$\mathrm{Tr}_{N/K}(x) = t \cdot x$。

让我们定义作用在右边，通过 $\Gamma$ 在 $N$ 通过 $x^\sigma = \sigma^{-1}(x)$。以类似的方式，我们可以将乘法群$N^*$视为右$Z^{(\Gamma)}$模块，外法则写作$(x, u) \mapsto x^u$。对于例、记号$x^{2a + 3r + \pi}$，其中$a, r, \pi$是$\Gamma$的元素，表示乘积$(x^a)^2 \cdot (x^r)^3 \cdot x^\pi$。如果如上所述，$N$ 的有限次数超过$K$ 和 $t = \sum_{\sigma \in \Gamma} a$，则我们有 $N_{N/K}(x) = \prod_{\sigma \in \Gamma} x^\sigma$，即，对于所有 $x \in N^*$，我们有 $N_{N/K}(x) = x'$。

假设此后$N$ 是有限次数超过$K$。给定$x \in N$，对于$\{x\}$是$\mathbf{K}^{(\Gamma)}$模块$N$的基，族$(\sigma(x))_{\sigma \in \Gamma}$应该是$N$的基超过$K$是充分必要的。这样的基被称为$N$超过$K$*的*正常基。

#### 定理 6 {#alg-v-s10-thm-6 .statement tag=06NF}

*令$N$为有限次数之伽罗瓦扩张超过$K$，令$\Gamma$为$N$之伽罗瓦群超过$K$。那么存在正常的基为$N$超过$K$；在其他字中，$\mathbf{K}^{(\Gamma)}$模块$N$不含秩1。*

我们将给出这个叙述中的两个证明。第一个使用以下引理，将在章VIII（§ 2, No. 5）中证明。

\* 引理 3. — 令$A$为$K$代数，$M_1$和$M_2$是有限秩在$K$上的两个$A$模，并假设存在扩张$L$ $K$使得模$L \otimes_K M_1$和$L \otimes_K M_2$超过环$L \otimes_K A$是同构的。那么$A$-模块$M_1$和$M_2$是同构的。

当$A = \mathbf{K}^{(\Gamma)}$、$M_1 = N$、$M_2 = A$、$L = N$的情况下，我们应用引理3。由科。 V，p. 64 存在$N \otimes_K N$ 到$N \otimes_K \mathbf{K}^{(\Gamma)}$ 的$K$ 同构$\varphi$，其中映射 $x \otimes y$ 到$\sum x u^1(y) \otimes \sigma$。很明显，$\varphi$是$N \otimes_K \mathbf{K}^{(\Gamma)}$模块的同构，因此定理是从引理3得出的。

对于第二个证明，我们将使用以下命题：

#### 命题 10 {#alg-v-s10-prop-10 .statement tag=06NG}

*设$x \in N$，则对于$\mathbf{K}^{(\Gamma)}$-模$N$的$\{x\}$到形式基，$\det(\sigma \tau(x))_{\sigma, \tau \in \Gamma} \neq 0$是充分必要的。

由于$\mathbf{K}^{(\Gamma)}$和$N$在$K$上具有相同的维数，所以说$\{x\}$是$N$的基在$\mathbf{K}^{(\Gamma)}$上意味着$\mathbf{K}^{(\Gamma)}$的映射$a \mapsto ax$变成$N$ 是单射的。这反过来意味着 $N \otimes_K \mathbf{K}^{(\Gamma)}$ 到 $N \otimes_K N$ 的映射 $b \mapsto b(1 \otimes x)$ 是单射的（II，p. 306，命题 14）。现在有一个$N \otimes_K N$的$N \otimes_K \mathbf{K}^{(\Gamma)}$模块同构到$N \otimes_K \mathbf{K}^{(\Gamma)}$，其中映射$1 \otimes x$到$\sum \sigma^{-1}(x) \otimes \sigma$。由此可见，$\{x\}$ 是 $N$ 的基超过 $\mathbf{K}^{(\Gamma)}$ 当且仅当，对于元素 $(n_\tau)$ 的每个非零族，$N$ 我们有 $\left( \sum n_\tau \otimes \tau \right) \left( \sum \sigma^{-1}(x) \otimes \sigma \right) \neq 0$。但这最后一个关系意味着存在$\sigma \in \Gamma$使得$\sum n_\tau \sigma^{-1}(x) \neq 0$，从而命题。

\* A) 假设 $K$ 是无穷大； $N$ 到$N$ 的映射 $x \mapsto \det(\sigma \tau(x))$ 是$K$ 上的多项式映射 (IV, p. 54)。通过从 $K$ 到 $N$ 的标量扩张，我们得到向量 $N$-空间 $N \otimes_K N$ 的相应的映射，我们刚刚看到后者并不相同零（因为 $N \otimes_K N$ 是秩 1 超过$N \otimes_K \mathbf{K}^{(\Gamma)}$）。因此存在 $x \in N$ 使得 $\det(\sigma \tau(x)) \neq 0$ (IV, p. 18, Th. 2)；更一般地说，从相同的参考文献中我们可以得到：

#### 命题 11 {#alg-v-s10-prop-11 .statement tag=06NH}

— 假设 K 是无限的，并且令 P : N → K 是 K 上非零的多项式映射。存在 x ∈ N，使得 P(x) ≠ 0 并且 {x} 是 N 在 $\mathbf{K}^{(\Gamma)}$ 上的基。

B) 假设 K 是有限的。根据命题 4 (V, p. 95)$^1$，K 上有限次数的每一个扩张都有一个循环伽罗瓦群。因此，我们将更普遍地考虑群$\Gamma$是阶n的循环的情况；我们用$\Gamma$的$\gamma$生成元来表示。

下面的引理是章VII中证明的更一般结果的特例。 环 $A$ 是有理数整数的环 $\mathbf{Z}$ 或域 $K$ 上的多项式的环 $K[X]$。

#### 引理 4 {#alg-v-s10-lem-4 .statement tag=06NI}

设 M 是由元素的有限数 $x_1, ..., x_h$ 生成的挠元 A-模；则存在 M 的元素 x，其湮没子 (II, p. 219) 等于 M 的湮没子。

在这两种情况下，$A$都是整环，并且$A$的每个理想都是主要的。当$A = \mathbf{Z}$（或$A = K[X]$）时，我们用素数数（或$K[X]$中不可约单调多项式的集合）的$\mathscr{P}$集合表示。对于$A$的每个元素$a \neq 0$，存在$A$的可逆元$u$和$(v_p(a))_{p \in \mathscr{P}}$族，其中有限支撑，正整数使得$a = u \prod_{p \in \mathscr{P}} p^{v_p(a)}$和$u$和整数 $v_p(a)$ 是唯一确定的（I、p. 51 和 IV、p. 13，第 13 条命题）。

设$a_i$为$x_i$的湮没子（对于$1 \leq i \leq h$）以及M的$a$湮没子；令$a_1, ..., a_h, a$为$A$的非零元素，使得$a_i = Aa_i$和$a = Aa$；自 $a = a_1 \cap ... \cap a_h$ 以来，从上述内容可以得出：

$$
v_p(a) = \sup_{1 \leq i \leq h} v_p(a_i) \quad \text{for all } p \in \mathscr{P}.
$$

让我们在形式$up_1^{n(1)} ... p_r^{n(r)}$中写出$a$，而$p_1, ..., p_r$在$\mathscr{P}$、$n(1) > 0, ..., n(r) > 0$和$A$的$u$可逆元中不同。让$j = 1, ..., r$；由(10) 存在整数$c(j)$使得$1 \leq c(j) \leq h$和$v_{p_j}(a_{c(j)}) = n(j)$； $A$中存在$b_j$，$a_{c(j)} = p_j^{n(j)} b_j$和元素，$y_j = b_j x_{c(j)}$有湮没子理想的$Ap_j^{n(j)}$。

让我们证明 $y = y_1 + ... + y_r$ 的湮没子 b 等于 M 的湮没子 a。在任何情况下，我们都有 $a \subset b$，因此 b 为形式 $Ap_1^{m(1)} ... p_r^{m(r)}$，$0 \leq m(j) \leq n(j)$ 为 $1 \leq j \leq r$。如果我们有$a \neq b$，就会存在整数，这样$1 \leq j \leq r$和$m(j) < n(j)$，因此$d_j = a/p_j$会消灭$y$。现在我们有$d_j y_k = 0$对应$k \neq j$，从而我们得到$d_j y_j = 0$；但$y_j$的湮没子是$Ap_j^{m(j)}$，而$d_j$不是$p_j^{m(j)}$的倍数。所以假设$a \neq b$是荒谬的。

$^1$ 读者可以轻松地说服自己，正常的基定理并没有在命题的任何地方使用之前证明。

我们将引理 4应用于$A$是多项式环$K[X]$和$M$阿贝尔的群$N$，其中外法则由$a \cdot x = \sum_{k=0}^m c_k \gamma^k(x)$定义为$a = \sum_{k=0}^\infty c_k X^k$ $K[X]$ 和 $x \in N$。令$a$为$M$的湮没子，然后为$\gamma^n = 1$，因此多项式$X^n - 1$位于$a$。令 $F \in a$； *由IV*，p. 11，Cor。存在 $K$ 和 $G \in K[X]$ 中的元素 $c_0, c_1, \ldots, c_{n-1}$ 使得

$$
F(X) = c_0 + c_1 X + \cdots + c_{n-1} X^{n-1} + (X^n - 1) G(X).
$$

因此，我们在$\operatorname{Hom}_K(N, N)$中有$c_0 + c_1 \gamma + \ldots + c_{n-1} \gamma^{n-1} = 0$，并且由于$N$的自同构$1, \gamma, \gamma^2, \ldots, \gamma^{n-1}$是不同的，戴德金的定理（*V*，p. 27，Cor.2）意味着$c_0 = c_1 = \ldots = c_{n-1} = 0$。最后，我们有

$$
F(X) = (X^n - 1) G(X), \quad \text{that is, } a = (X^n - 1) K[X].
$$

到引理 4 时，$N$ 中存在元素 $x$，其$K[X]$ 中的湮没子等于$(X^n - 1) K[X]$。由于$K[X]$的向量子空间的单项式$1, X, \ldots, X^{n-1}$形式基补充$(X^n - 1) K[X]$（*IV*，p. 11，Cor.），元素 $N$ 中的$x, \gamma(x), \ldots, \gamma^{n-1}(x)$ 在$K$ 上线性无关。由于$[N : K] = n$（*V*、p. 66、Th.3），序列$(x, \gamma(x), \ldots, \gamma^{n-1}(x))$因此是$N$超过$K$的（正常）基。

### 10. 有限 $\Gamma$ 集和 etale 代数

令$K_s$为$K$的可分闭包（*V*，p. 45，命题14），以及$K$的$\Gamma$伽罗瓦群，超过$K$。通过$\Gamma$-*集合*，我们理解集合$X$和群$\Gamma$的作用$(\sigma, x) \mapsto \sigma x$，这样$X$的每个点的稳定子都是一个*开* 子群共 $\Gamma$。当$X$配备离散的拓扑时，$\Gamma \times X$到$X$的映射$(\sigma, x) \mapsto \sigma x$是“连续的”。

令 $X$ 为*有限* $\Gamma$ 集合。我们将$\Gamma$的定义作用在$X$的映射的$K$-代数$K_s^X$通过公式转化为$K_s$

$$
u_\sigma f(x) = \sigma(f(\sigma^{-1}x))
$$

对于 $\pi \in \Gamma, f \in K_s^X$ 和 $x \in X$。令$\Theta(X)$为$K_s^X$中$\Gamma$的不变量的集合；这是映射$f : X \to K_s$的$K_s^X$由……组成的子K代数，使得$f(\sigma x) = \sigma(f(x))$对应$\sigma \in \Gamma$和$x \in X$。

#### 引理 5 {#alg-v-s10-lem-5 .statement tag=06NJ}

*令$X$为有限$\Gamma$集合，并令$x_1, \ldots, x_n$为$X$的点，使得轨道$\Gamma x_1, \ldots, \Gamma x_n$形式划分为$X$。对于$1 \leq i \leq n$，令$\Delta_i$为$\Gamma$中$x_i$的稳定子，并令$L_i$为$A_i$的不变量的域。那么$L_1, \ldots, L_n$就是$K$的有限次数可分扩张，而映射$f \mapsto (f(x_1), \ldots, f(x_n))$就是$\Theta(X)$的K-代数同构到$L_1 \times \ldots \times L_n$。*

$\Gamma$ 假设子群 $A_i, \ldots, A_n$ 已开放，Cor. V、p. 68 的 5，显示$K$ 的子扩展$L_1, \ldots, L_n$，是有限次数超过$K$。显然，它们是可分离的；现在引理 5 中的最后一个断言是直接的。

从引理 5 和 Th. 4 (*V*, p. 34f.) 我们立即得到以下结果。

#### 命题 12 {#alg-v-s10-prop-12 .statement tag=06NK}

— 对于每个有限 $\Gamma$ 集 $X$ 代数 $\Theta(X)$ ，$K$ 的 etale，次数等于 $X$ 的基数。此外，$K$之上的每个etale代数都同构于形式$\Theta(X)$的代数。

#### 注 {#alg-v-s10-n10-rem-1 .statement tag=06NL}

a) 容易证明，对于$\Theta(X)$到$K$的每个$K$-代数同态$\varphi$，都存在$X$的唯一元素$x$，使得对于所有$f \in \Theta(X)$都有$\varphi(f) = f(x)$。

2) 令$X$和$Y$为两个有限$\Gamma$集合。 让$\mathfrak{T}_\Gamma(X, Y)$是映射的集合，$X$的$u$进入$Y$，这样$u(\sigma x) = \sigma u(x)$对于所有$\sigma \in \Gamma$和所有$x \in X$。 对于$u \in \mathfrak{T}_\Gamma(X, Y)$，我们通过$u^*(f) = f \circ u$ 定义 $K$-代数同态$u^*: \Theta(Y) \to \Theta(X)$。 对于$\Theta(Y)$的每个同态$\Psi$进入$\Theta(X)$，都存在$\mathfrak{T}_\Gamma(X, Y)$的唯一元素$u$，使得$\Psi = u^*$。

### 11.拟伽罗瓦扩展的结构

#### 命题 13 {#alg-v-s10-prop-13 .statement tag=06NM}

— 令 $N$ 为 $K$ 的拟伽罗瓦扩展。我们用$N$的所有$K$-自同构的$N_r$、域表示群的不变量，并用$N_s$表示$N$中$K$的相对可分代数闭包（$V$， p. 44）。然后：

a) $N_r$ 是$N$ ($V$, p. 25) 中$K$ 的相对$p$-激进闭包。

b) $N$，是$K$的伽罗瓦扩张以及$N_s$扩展的每个$K$自同构，以独特的方式与$N$的$N_r$自同构。

c) 域 $N_r$ 和 $N$，在 $K$ 上呈线性不相交的，我们有 $N = K[N, \cup N_s]$；其他字、$N_r \otimes_K N$的典范同态，变成$N$就是同构。

设$\Omega$为$K$包含$N$的代数闭包作为子扩展（$V$，p. 23，Th.2）。 $\Omega$ 诱导自同构 $N$ 的每个 $K$ 自同构，因为 $N$ 是拟伽罗瓦。因此，$N_r$的每个元素在$K$的群下是不变的-$\Omega$的自同构，因此$p$-在$K$上的激进（$V$，p. 53，Cor.3）。相反，$N$的每个元素（在$K$上是$p$激进）在$N$的每个$K$自同构下显然是不变的，因此属于到$N_r$。这就证明了a）。

$\Omega$ 映射 $N$ 到 $N$ 的每个 $K$ 自同构，因此 $N_r$ 到 $N_r$，所以 $N_r$ 是 $K$ 的拟伽罗瓦扩展 ($V$， p. 54，提案 3）。由此可见，$N_s$ 是$K$ 的伽罗瓦扩张。 $N_r \cap N$ 的每个元素，在 $K$ 上都是可分离的代数和 $p$ 根式，因此属于到 $K$（$V$，p. Cor. 3）；因此我们有$K_r \cap K_s = K$。现在$N$是$N_r$上的$p$根式（$V$，p. 44，命题13），并且是$N_r$上的可分离代数（$V$，p. 56，Th.1），因此$p$-激进且可分离超过$K(N_r \cup N_s)$。因此我们有$N = K(N_r \cup N_s)$ ($V$, p. 39, Cor.3) 和断言 b), c) 从Th 开始。 5（$V$，p. 71）。

#### 推论{#alg-v-s10-n11-cor-1 .statement tag=06NN}

— 令$p$为$K$、$\overline{K}$、代数闭包的$K$、$K_s$的特征指数，$\overline{K}$中$K$的相对可分闭包和$K^{p^{-\infty}}$为$K$的完美闭包。那么$K^{p^\infty} \otimes K_s$到$\overline{K}$的典范同态就是同构。

#### 注 {#alg-v-s10-n11-rem-1 .statement tag=06NO}

令$R$（或$S$）为$K$的$p$根（或可分离代数）扩张。 Then 代数 $R \otimes_K S$ is 域 : for $R$ (resp. $S$) is isomorphic to a subextension of $K^{p^\infty}$ (resp. $K_s$) and it suffices to apply the above Cor.以及$V$、p. 17的第1条建议。

### 习题{#alg-v-s10-exercises}

§ 10](exercises/s10/)参见[习题。
