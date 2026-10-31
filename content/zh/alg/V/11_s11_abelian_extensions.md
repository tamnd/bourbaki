---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 11
section_title: Abelian extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.160-A V.166
pdf_pages: 0191-0207, 0274-0280
extraction: ocr
subsections:
    - "no": 1
      title: Abelian extensions and the abelian closure
      page: 77
      pdf_page: 191
    - "no": 2
      title: Roots of unity
      page: 78
      pdf_page: 192
    - "no": 3
      title: Primitive roots of unity
      page: 79
      pdf_page: 193
    - "no": 4
      title: Cyclotomic extensions
      page: 81
      pdf_page: 195
    - "no": 5
      title: Irreducibility of cyclotomic polynomials
      page: 83
      pdf_page: 197
    - "no": 6
      title: Cyclic extensions
      page: 85
      pdf_page: 199
    - "no": 7
      title: Duality of $\mathbf{Z}/n\mathbf{Z}$-modules
      page: 86
      pdf_page: 200
    - "no": 8
      title: Kummer theory
      page: 88
      pdf_page: 202
    - "no": 9
      title: Artin-Schreier theory
      page: 91
      pdf_page: 205
statements: 45
exercises: 23
content_sha256: fe0fc13ca8d29d600f9e71ef1b570c41846466590fa8d28f1c56d4b423fe264b
translated_from: content/en/alg/V/11_s11_abelian_extensions.md
translation_method: google
source_content_sha256: 3510a553a6737e108ce1bbc1176deb8962c17c7a4a3f4de1c127471caa214100
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 599578eae478dcc3ae885ecea292ed1ad918940076a5eba86734110cb47e441f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 11。 阿贝尔的扩张

在本段中，K 表示域。

### 1. 阿贝尔的扩张和阿贝尔的闭包

#### 定义 1 {#alg-v-s11-def-1 .statement tag=06OC}

— 如果 K 的扩张 E 是伽罗瓦且其伽罗瓦群是可交换的，则称其为阿贝尔的。

由于可交换性群的每个子群都是正规的，Cor. V,p. 68的4表明阿贝尔的扩张的每个子扩展都是阿贝尔的。

#### 命题 1 {#alg-v-s11-prop-1 .statement tag=06OD}

— 令 E 为 K 的伽罗瓦扩张，且 Γ 为伽罗瓦群。设 A 为 Γ (I, p. 10, Def. 4) 的导出群，A 的不变量为 F 域。对于 E 的子扩展 L 为阿贝尔的，它包含在 F 中是充分必要的。

首先，注 F 也是 Γ 中 A 的闭包$\bar{\Delta}$ 不变量的域，并且 $\bar{\Delta}$ 是 Γ 的闭法线子群。 作者：V、p. 68、Cor。 4、F因此是K的伽罗瓦扩张。 此外，F 在 K 上的伽罗瓦群与 $\Gamma / \bar{\Delta}$ 同构的，因此是可交换的。 因此 F 的每个子扩展都是阿贝尔的。 相反，令L为E中包含的K的阿贝尔的扩张，并令Π为E在L上的伽罗瓦群。 Since L is Galois, Π is a normal subgroup of Γ and the Galois group of L over K is isomorphic to $\Gamma / \Pi$ (V, p. 68, Cor. 4). 因此 $\Gamma / \Pi$ 是可交换的且 Π 包含于 A, 从而 $L \subset F$。

#### 推论{#alg-v-s11-n1-cor-1 .statement tag=06OE}

— 令 E 为 K 的扩张，并令 $(E_i)_{i \in I}$ 为 E 的子扩展族，使得 $E = K \left( \bigcup_{i \in I} E_i \right)$。假设每个扩张$E_i$都是阿贝尔的，那么E也是如此。

首先，E 是 K 的伽罗瓦扩张（V，p. 57，命题 1）。如果域 F 如命题 1 中定义，那么对于所有 $i \in I$、从而 $E = F$，我们都有 $E_i \subset F$。

如果 K 的阿贝尔的扩张并且 K 的每个阿贝尔的扩张同构于 E 的子扩展，则称 K 的扩张 E 是 K 的阿贝尔的闭包。 命题 1 意味着 K 的阿贝尔的闭包的存在： for let $K_s$是K的可分闭包，与伽罗瓦群$\Gamma$并让$(\overline{\Gamma}, \overline{\Gamma})$是$\Gamma$的导出群的闭包；用 $(\overline{\Gamma}, \overline{\Gamma})$ 的不变量 $K_{ab}$ 域表示；因为 K 的每个可分离代数扩张都同构于 $K_s$ 的子扩展（V，p. 45，Cor.）。命题1表明$K_{ab}$是K的阿贝尔的闭包。K上$K_{ab}$的伽罗瓦群与$\Gamma / (\overline{\Gamma}, \overline{\Gamma})$自然同构。现在让我们展示阿贝尔的闭包的唯一性：令 E, E' 是 K 的两个阿贝尔的闭包；由定义存在 K-同态 $u : E \to E'$ 和 $v : E' \to E$，并且命题 1 (V, p. 52) 意味着 $v(u(E)) = E$ 和 $u(v(E')) = E'$，因此 $u$ 是 E 到 E' 的 K-同构。 E 到 E' 的任何其他 K 同构都是形式 $u_1 = \sigma_0 \circ u$ 和 $\sigma_0 \in \mathrm{Gal}(E'/K)$；由于$\mathrm{Gal}(E'/K)$是可交换的，$\mathrm{Gal}(E/K)$到$\mathrm{Gal}(E'/K)$的同构$\sigma \mapsto u \circ \sigma \circ u^{-1}$独立于$u$；它被称为$\mathrm{Gal}(E/K)$到$\mathrm{Gal}(E'/K)$的典范同构。

### 2. 根 / 单位元

#### 定义 2 {#alg-v-s11-def-2 .statement tag=06OF}

*如果存在整数$n > 0$使得$\zeta^n = 1$，则K的元素$\zeta$被认为是单位元的根；对于每个整数$n > 0$，使得$\zeta^n = 1$、$\zeta$被称为单位元的第n个根。*

相当于说，单位元的根是K的非零元素的乘法群$K^*$*有限阶*元素（I，p. 51）。 单位元形式子群 $\mu_\infty(K)$（$K^*$）中的根，$\mu_\infty(K)$中的第n个根形式子群$\mu_n(K)$。如果$n$除$m$，我们有$\mu_\infty(K) = \bigcup_{n \geq 1} \mu_n(K)$和$\mu_n(K) \subset \mu_m(K)$。对于单位元 $\zeta$的每个根，至少存在整数$n \geq 1$，使得$\zeta$属于到$\mu_n(K)$，即群中$\zeta$的阶 $K^*$。

群$\mu_n(K)$，是多项式$X^n - 1$的根的集合，是有限的阶$\leq n$。令$p$为K的特征。当$p = 0$，或$p \neq 0$和$n$不能被$p$整除时，$X^n - 1$的导数$nX^{n-1}$与$X^n - 1$互质，因此多项式$X^n - 1$是*可分离的；此外，如果 K 是代数闭集，则 $\mu_n(K)$ 是 $n$ 元素的群。

假设K具有非零特征$p$，且令$r \geq 0$为整数；由于 K 到 K 的映射 $x \mapsto x^{p^r}$ 是单射的，因此对于每个整数 $n \geq 1$，我们都有 $\mu_{np^r}(K) = \mu_n(K)$。

我们注域可能包含单位元中除了 1 之外没有第 n 个根：对于任何奇数整数 $n$，例的质数域 $\mathbf{Q}$ 和 $\mathbf{F}_p$ 就是这种情况。

#### 定理 1 {#alg-v-s11-thm-1 .statement tag=06OG}

*令$p$为K的特征指数，令$n > 0$为整数。则K中单位元的第n个根的群$\mu_n(K)$是循环的，其阶除$n$；当 K 是代数闭且 $n$ 与 $p$ 互质时，群 $\mu_n(K)$ 是阶 $n$ 的循环。*

只需证明定理的第一个断言，即以下更精确的引理中的推论：

#### 引理 1 {#alg-v-s11-lem-1 .statement tag=06OH}

*设G为阶$m$的$K^*$的有限子群；那么 G 是循环的，我们有 $G = \mu_m(K)$.*

将 G 视为 Z 模；对于所有$x \in G$，我们都有$mx = 0$，因此G的湮没子是形式$r\mathbf{Z}$的理想，其中整数$r \geq 1$除$m$。因此我们有$G \subset \mu_r(K)$。将引理 4 (V，p. 74)与$A = \mathbf{Z}$和$M = G$应用的，存在阶$r$的G的元素$x$；令$G'$为由$x$生成的G的循环子群。我们有$G' \subset \mu_r(K)$、卡$(G') = r$、卡$\mu_r(K) \leq r$；因此我们有

G' = μ_r(K) ⊃ G 且 G 是阶 r 的循环，因此等于 μ_r(K)。由于 G 有阶 m，所以我们有 m = r 和引理。

#### 命题 2 {#alg-v-s11-prop-2 .statement tag=06OI}

— 令 K 为代数闭集，并令 p 为其特征指数。在群 Q/Z[1/p] 上存在 μ_∞(K) 的同构。

我们将 1/p 生成的 Q 表示为 Z[1/p] 子环，即形式 a/p^n 的有理数的集合，其中 a ∈ Z 且 n ≥ 1；因此，如果 K 的特征为 0，则我们有 Z[1/p] = Z。

令 (v_n) 为所有不可被 p 整除的整数中的严格递增的序列由……组成，如果 p ≠ 1；将 X = v_1 v_2 ... v_n 并用单位元的第 λ_n-th 根的 H_n 群表示；我们有 H_{n+1} ⊃ H_n 和 μ_∞(K) = U H_n。由于 H_n 是阶 X (Th. 1) 的循环，因此存在根单位元的序列 (a_n)，使得 a_n 生成 H_n 且 a_n = α_n^{v_n + 1}。

进一步令β_n为1/λ_n的剩余类类 mod Z[1/p]，并令H'_n为由β_n生成的Q/Z[1/p]的循环子群。显然，β_n = v_{n+1} β_{n+1} 且 H'_n 为阶 λ_n，因为如果 p ≠ 1，则 X 不能被 p 整除。因此，对于所有 n ≥ 1 同构 φ_n ： H_n → H'_n 使得 φ_n(α_n) = β_n 且关系 α_n = α_{n+1}^{v_n + 1}，β_n = v_{n+1} β_{n+1}，证明 φ_n+，扩展 φ_n。最后，在 Q/Z[1/p] 上存在一个唯一的 μ_∞(K) 同构 φ 延伸同构 φ_n，即对于所有 n ≥ 1，φ(α_n) = β_n。

#### 注 1 {#alg-v-s11-n2-rem-1 .statement tag=06OJ}

当 K 是特征 0 的代数闭域时，群 μ_∞(K) 因此与 Q/Z 同构的（非规范）。 *当K是复数的域C时，我们可以写出这样的显式同构：实际上映射x↦e^{2πix}是Q的同态到C*与核Z和像 μ_∞(C);因此，通过将 Q/Z 的定义同构传至 μ_∞(C)。*

#### 注 2 {#alg-v-s11-n2-rem-2 .statement tag=06OK}

可以显示以下结果（cf.V，p. 165，例21）：设G和H是两个可交换的群，其元素都是有限的阶。假设对于每个整数 n ≥ 1，方程 nx = 0 具有相同的数和解，假设 G 和 H 中有限。则群 G 和 H 同构的。这提供了提案 2 的新证明。

#### 注 3 {#alg-v-s11-n2-rem-3 .statement tag=06OL}

对于每个素数数 l 设 μ_{l∞}(K) = U μ_{ln}(K)。当l是K的特征p时，我们有μ_{p∞}(K) = {1}。从 I、p. 80、Th。 4，我们推导出 μ_∞(K) 是子群 μ_{l∞}(K) 的直和，其中 l 运行于与 p 不同的所有素数数的集合。对于给定的素数数 l，只有两种情况是可能的：要么 μ_{l∞}(K) 是有限的，然后 μ_{l∞}(K) 同构于 Z/l^nZ 对于合适的 n (Th. 1)，或者 μ_{l∞}(K) 是无限的，然后 μ_{l∞}(K) 同构于 Z[l^{-1}]/Z (cf.) 注2）。

### 3. 单位元的原语根

设 n ≥ 1 为整数。通过 n 的欧拉指示符，写作 φ(n)，我们可以理解数或可逆元环 Z/nZ 整数模 n。到下一个命题$\varphi(n)$也是整数$k$的数与$n$素的，这样$0 \leq k < n$。

#### 命题 3 {#alg-v-s11-prop-3 .statement tag=06OM}

*令$k$和$n \geq 1$为两个整数。那么下面的断言是等价的*：

a) *$k$ mod $n$ 的剩余类类在环 $\mathbf{Z}/n\mathbf{Z}$ 中可逆；*
b) *$k$ mod $n$ 生成的剩余类类循环群 $\mathbf{Z}/n\mathbf{Z}$;*
c) *整数 $k$ 和 $n$ 互质* (*I*, p. 112)。

条件 a) 和 b) 均表示存在整数 $x$ 使得$kx \equiv 1 \pmod{n}$，即存在两个整数 $x$ 和$y$ 使得$kx + ny = 1$。后者条件只是意味着$k$和$n$互质。

#### 推论 1 {#alg-v-s11-prop-3-cor-1 .statement tag=06ON}

*令$G$为阶$n$的循环群，令$d$为$n$的除子。那么$G$中的阶$d$元素数就等于$\varphi(d)$。特别地，$\varphi(n)$是$G$的生成元中的数。*

由于$G$与$\mathbf{Z}/n\mathbf{Z}$同构的，根据命题3，$G$的生成元数等于$\varphi(n)$。设$g$为$G$的生成元；然后$G$的元素$h$使得$h^d = 1$构成由$g^{n/d}$生成的$G$的子群$H$；这个群是阶$d$的循环，阶$d$的$G$的元素是$H$的生成元，因此它们的数是$\varphi(d)$。

#### 推论 2 {#alg-v-s11-prop-3-cor-2 .statement tag=06OO}

*对于每个整数 $n \geq 1$，我们有*
$$
\sum_{d \mid n} \varphi(d) = n,
$$
*其中整数 $d$ 超过除子的集合 > $n$ 的 0* ^1。

与Cor的记号。 1，$G$的每个元素都有一个有限的阶，即$n$的除子$d$，对于固定的$d$，有$\varphi(d)$这样的元素。

$\varphi(n)$的计算是基于两个公式：

(2) $\varphi(mn) = \varphi(m)\varphi(n)$ 如果 $m$ 和 $n$ 互质，
(3) $\varphi(p^a) = p^{a-1}(p-1)$（$p$素的，$a \geq 1$）。

第一个直接来自以下事实：环$\mathbf{Z}/mn\mathbf{Z}$和$(\mathbf{Z}/m\mathbf{Z}) \times (\mathbf{Z}/n\mathbf{Z})$是同构的（*I*，p. 112），并且$(A \times B)^* = A^* \times B^*$是两个环$A$和$B$。证明(3)我们注$p^a$的正除子是$1, p, p^2, \ldots, p^a$；因此，当且仅当它不能被$p$整除时，除了$1$之外，整数$k$没有公共的除子与$p^a$；由于$0$和$p^a - 1$之间存在$p$的$p^a - 1$倍数，所以我们确实找到了（3）。

公式 (2) 和 (3) 立即表明
$$
\varphi(n) = n \prod_p (1 - 1/p),
$$
其中 $p$ 超过 $n$ 素数除子的集合。

^1 关系 $d \mid n$ 整数 > 0 之间表示 « d 除 n » (VI, p. 5)。

如果阶 $n$ 的第n 个根单位元被认为是原始的；如果存在根$\zeta$，则群$\mu_n(K)$属于阶$n$，由$\zeta$生成。 \* 对于例，$\mathbf{C}$中单位元的原语n个根是数$e^{2\pi i k / n}$，其中$0 \leq k < n$和$k$与$n$素的。 \* 科。命题 3 的 1 现在意味着以下结果。

#### 命题 4 {#alg-v-s11-prop-4 .statement tag=06OP}

— 令 $n \geq 1$ 为整数；假设 K 中存在单位元的第 n 个根（如果 K 是可分离闭的且$n . 1, \neq 0$，则对于例成立）。那么K中单位元的原语第n个根的数等于$\varphi(n)$。

### 4. 环切术扩张

令$p$为K的特征指数，令$n \geq 1$为整数与$p$素的；通过 K 上 $n$ 级的分圆扩张，我们可以理解 K 上多项式 $X^n - 1$ 的任何分裂扩张 E (V, p. 21)。由于该多项式是可分的，因此 E 是 K 的伽罗瓦扩张，有限次数 (V，p. 57)。 E 中存在单位元的第 n 个本原根；如果$\zeta$是这样的根，那么单位元的每n个根都是$\zeta$的幂，因此$E = K(\zeta)$。

对于这个数的其余部分，我们将K的选择可分闭包$K_s$。对于$p$群$\mu_n(K_s)$的每个$n \geq 1$素数是阶$n$和域的循环

$$
R_n(K) = K(\mu_n(K_s))
$$

是 K 级 $n$ 的分圆扩张。我们可以将$\mu_n(K_s)$视为秩 1 的自由模超过环$\mathbf{Z}/n\mathbf{Z}$，以及$\mathrm{Gal}(K_s/K)$诱导的每个元素$a$ 自同构共$\mu_n(K_s)$；因此，对于$K_s$中单位元$\zeta$的每第n个根、$\mathrm{Gal}(K_s/K)$中的每个$u$以及整数，存在以公式$u(\zeta) = \zeta^j$为特征的同态$\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ $j$ 剩余类类 $\chi_n(u)$ mod $n$。由于$R_n(K) = K(\mu_n(K_s))$，$\chi_n$的核是$\mathrm{Gal}(K_s/K)$的子群$\mathrm{Gal}(K_s/R_n(K))$；因此我们有$\chi_n = \varphi_n \circ \psi_n$，其中$\psi_n$是$\mathrm{Gal}(K_s/K)$的限制同态超过$\mathrm{Gal}(R_n(K)/K)$，$\varphi_n$是$(\mathbf{Z}/n\mathbf{Z})^*$中$\mathrm{Gal}(R_n(K)/K)$的单同态。特别是我们有以下结果：

#### 命题 5 {#alg-v-s11-prop-5 .statement tag=06OQ}

— 对于 K 的每个整数 $n \geq 1$ 与 $p$ 扩张 $R_n(K)$ 的质数是有限次数的阿贝尔的，其伽罗瓦群同构于 $(\mathbf{Z}/n\mathbf{Z})^*$ 的子群及其次数除阶$\varphi(n)$共$(\mathbf{Z}/n\mathbf{Z})^*$。

设Q为有理数的域Q的代数闭包，并令n为整数。那么$n$级的分圆多项式$\Phi_n$定义为

$$
\Phi_n(X) = \prod_{\zeta \in S_n} (X - \zeta),
$$

其中$S_n$是$Q$中单位元的原始第n个根的集合。首一多项式 $\Phi_n$ 为次数 $\varphi(n)$（命题 4）。很明显，$\Phi_n(X)$在$\bar{\mathbf{Q}}$的所有自同构下是不变的，因此属于到$\mathbf{Q}[X]$。由于$S_n$的每一个元素$\zeta$都是多项式$X^n - 1$的根，所以多项式$\Phi_n(X)$除$X^n - 1$，下面的引理表明$\Phi_n(X)$是一元多项式具有整数系数。

#### 引理 2 {#alg-v-s11-lem-2 .statement tag=06OR}

*设 f、g 和 h 为 $\mathbf{Q}[X]$ 中的一元多项式，使得 $f = gh$。如果 f 有整数系数，g 和 h 也是如此。*

令$a$（或$b$）为整数 $\alpha \geq 3$（或$\beta \geq 1$）中最小的一个，使得$\alpha g$（或$\beta h$）有整数系数；我们放入 $g' = ag$ 和 $h' = bh$ 并通过 *reductio adabsurdum* 显示 $a = b = 1$。如果不是这样，就会有 $ab$ 的素数除子 $p$。如果$u \in \mathbf{Z}[X]$，让我们将域$\mathbf{F}_p$中的系数写为$\bar{u}$，该多项式是通过对$u$的系数进行约简模$p$获得的。我们有$g'h' = abf$、从而$\bar{g}'\bar{h}' = 0$；由于环$\mathbf{F}_p[X]$是整环（IV，p. 9，命题8），因此我们有$\bar{g}' = 0$或$\bar{h}' = 0$。在其他字、$p$除中，$g'$的所有系数或$h'$和此与……矛盾假设的所有系数。

我们有关系

$$
X^n - 1 = \prod_{d|n} \Phi_d(X) .
$$

因为我们有 $X^n - 1 = \prod_{\zeta \in \mu_n(\mathbf{Q})} (X - \zeta)$ 和集合 $S_d$，$d$ 除 $n$ 形式划分 $\mu_n(\mathbf{Q})$。

公式 (6) 确定 $\Phi_n(X)$ 当我们知道 $\Phi_d(X)$ 为所有除子 $d < n$ 的 $n$ 时；由于$\Phi_1(X) = X - 1$，因此我们有一个递归过程来计算$\Phi_n$。对于例对于素数 $p$ 我们有

$$
X^p - 1 = (X - 1)\Phi_p(X) ,
$$

从而

$$
\Phi_p(X) = X^{p-1} + X^{p-2} + \cdots + X + 1 ,
$$

和

$$
\Phi_{p^r+1}(X) = \Phi_p(X^{p^r}) \quad \text{for} \quad r \geq 0 .
$$

让我们列出 $1 \leq n \leq 12$ 的多项式 $\Phi_n(X)$ 的值：

$$
\begin{align*}
\Phi_1(X) &= X - 1 \\
\Phi_2(X) &= X + 1 \\
\Phi_3(X) &= X^2 + X + 1 \\
\Phi_4(X) &= X^2 + 1 \\
\Phi_5(X) &= X^4 + X^3 + X^2 + X + 1 \\
\end{align*}
$$

$$
\Phi_6(X) = X^2 - X + 1
$$
$$
\Phi_7(X) = X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_8(X) = X^4 + 1
$$
$$
\Phi_9(X) = X^6 + X^3 + 1
$$
$$
\Phi_{10}(X) = X^4 - X^3 + X^2 - X + 1
$$
$$
\Phi_{11}(X) = X^{10} + X^9 + X^8 + X^7 + X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_{12}(X) = X^4 - X^2 + 1
$$

$\Phi_1, \Phi_2, \Phi_3, \Phi_4, \Phi_5, \Phi_7, \Phi_8, \Phi_9$和$\Phi_{11}$的值直接由(7)得出；现在我们有$\Phi_1 \Phi_2 \Phi_3 \Phi_6 = X^6 - 1$和$\Phi_1 \Phi_2 \Phi_3 \Phi_4 \Phi_6 \Phi_{12} = X^{12} - 1$，从而$\Phi_4 \Phi_{12} = \frac{X^{12} - 1}{X^6 - 1} - X^6 + 1$，最后是$\Phi_{12} = \frac{X^6 + 1}{X^2 + 1} = X^4 - X^2 + 1$。案例$n = 6$和$n = 10$可类似处理。

#### 注 {#alg-v-s11-n4-rem-1 .statement tag=06OS}

\* 对于每个整数 $n > 0$ 函数 $\mu(n)$ 定义如下：如果 $n$ 能被素数数的平方整除，我们放入 $\mu(n) = 0$，否则 $\mu(n) = (-1)^h$ 如果 $n$ 是乘积 $h$ 不同素数数 (« 莫比乌斯函数 »)。可以证明

$$
\Phi_n(X) = \prod_{d|n} (X^{n/d} - 1)^{\mu(d)},
$$

或者更明确地

$$
\Phi_n(X) = \prod_{p_1 < \ldots < p_h} (X^{n/p_1 \cdots p_h} - 1)^{(-1)^h}
$$

其中 $(p_1, \ldots, p_h)$ 超过 $n$ 素数除子的所有严格递增的序列的集合（cf. 谎言、II、p. 207，例 1）。

### 5.分圆多项式的不可约性

令$p$为$K$的特征指数，令$n$为整数素数顶。我们用$\mathbf{Z}[X]$的唯一同态下具有整数系数$\Phi_n$的多项式的$\Phi_n \in K[X]$像表示为$K[X]$，其中映射$X$到$X$。

#### 引理 3 {#alg-v-s11-lem-3 .statement tag=06OT}

*$K_s$中$\Phi_n$的根是单位元的原始$n$-第根。*

用$K_s$中$\Phi_n$根$S$、集合表示。通过公式 (6)，集合 $\mu_n(K_s)$ 是 $d$ 除 $n$ 的 $S_d$ 的并。 单位元的每个原语$n$-第根，因此属于到$S_n$和引理现在都来自第4条命题（V，p. 81）。

#### 命题 6 {#alg-v-s11-prop-6 .statement tag=06OU}

— 令 $p$ 为 $K$ 的特征指数，令 $n \geq 1$ 为整数 $p$ 的素数。为了使多项式 $\Phi_n(X)$ 在 $K[X]$ 中不可约，同态 $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ 应该是满射的，这是充分必要的。

到引理 3，对于$\Phi_n(X)$的每个根$\zeta$，我们都有$R_n(K) = K(\zeta)$，因此当且仅当$\Phi_n(X)$的次数$\varphi(n)$等于$[R_n(K):K]$时$\Phi_n(X)$在$K[X]$中不可约。此外，$R_n(K)$在$K$上的伽罗瓦群是阶$[R_n(K):K]$，并且它与$(\mathbf{Z}/n\mathbf{Z})^*$的子群同构，即$\chi_n$的像。现在，第 6 条命题是从 $(\mathbf{Z}/n\mathbf{Z})^*$ 是阶 $\varphi(n)$ 的事实得出的。

#### 定理 2（高斯）{#alg-v-s11-thm-2 .statement tag=06OV}

— 令$Q$为$Q$的代数闭包，并令$n \geq 1$为整数。

a) 分圆多项式$\Phi_n(X)$在$Q[X]$中不可约。

b) $R_n(Q)$ 与$Q$ 的次数是$\varphi(n)$。

c) $\mathrm{Gal}(\bar{Q}/Q)$ 到 $(\mathbf{Z}/n\mathbf{Z})^*$ 的同态 $\chi_n$ 是满射，定义是通过将 $\mathrm{Gal}(R_n(Q)/Q)$ 的商同构传到$(\mathbf{Z}/n\mathbf{Z})^*$。

考虑到命题 6，我们只需证明 c)。 每个整数$r$与$n$素数都是数$p_1, \ldots, p_s$素数乘积不除$n$；因此足以证明，对于每个素数数$p$，不将$n$、$\mu_n(Q)$的映射$x \mapsto x^p$除以扩展到$R_n(Q)$的自同构。 只要证明$\zeta$是单位元的原语第$n$第根，$\zeta$在$Q$上的最小多项式$f$等于$\zeta^p$在$Q$上的最小多项式$g$。

我们假设$f \neq g$并通过反证法进行论证。多项式$f$和$g$在$Q[X]$和除$X^n - 1$中是不可约的，因此存在$u \in Q[X]$使得$X^n - 1 = fg u$（IV，p. 13，命题13）。 引理 2 (V, p. 82) 表明$f, g$ 和$u$ 具有整数系数。让我们用 $\bar{v}$ 表示系数为 $\mathbf{F}_p$ 的多项式，该多项式是从多项式 $v \in \mathbf{Z}[X]$ 通过归约 mod $p$ 获得的。因此我们在$\mathbf{F}_p[X]$中有$X^n - 1 = \bar{f} \bar{g} \bar{u}$。

此外，我们有$g(\zeta^p) = 0$，因此$g(X^p)$是$\mathbf{Q}[X]$中$f(X)$的倍数。到引理 2 时，存在$h \in \mathbf{Z}[X]$，从而$g(X^p) = f(X) \cdot h(X)$。现在我们对每个多项式$v \in \mathbf{F}_p[X]$都有$v(X^p) = v(X)^p$。通过约简 mod $p$，我们得到 $\bar{g}^p = \bar{f} \bar{h}$。如果$v$是$\mathbf{F}_p[X]$除以$\bar{f}$的不可约多项式，那么它必定是除$\bar{g}$。从$\bar{f} \bar{g}$除$X^n - 1$开始，我们在$\mathbf{F}_p[X]$结论$v^2$除$X^n - 1$。这是荒谬的，因为多项式 $X^n - 1$ 在 $\mathbf{F}_p[X]$ 中是可分的。

可以证明，对于$Q$上有限次数的每个阿贝尔的扩张$E$，都存在整数$n \geq 1$，使得$E$同构于$R_n(Q)$的子扩展。 \* 在其他字中，域$Q(\mu_{\infty}(C))$是阿贝尔的闭包$Q$。 *（《克罗内克-韦伯定理》）。

### 6.循环扩张

#### 定义 3 {#alg-v-s11-def-3 .statement tag=06OW}

— *如果 K 的扩张 E 是伽罗瓦且其伽罗瓦群是循环的，则称它是循环的。*

#### 例 {#alg-v-s11-n6-exa-1 .statement tag=0DI2}

*1) 素数次数的每个伽罗瓦扩张都是循环的，因为素数阶$p$的每个有限群G都是循环的（对于G的每个元素$x \neq 1$都是阶$p$，因此生成 G）。

2) 令$F(X) = X^2 + aX + b$为$K[X]$中的不可约多项式。 $F(X)$ 不可分离的唯一情况是$K$ 具有特征 2 和 $a = 0$。我们先把这个案子放在一边；令 E 为由 $F(X)$ 的根 $x$ 生成的 K 的扩张。我们有$[E : K] = 2$和$F(X) = (X - x)(X + a + x)$，因此E是K的伽罗瓦扩张。E在K上的伽罗瓦群是阶2，因此是循环的。

3) 令$\mathbf{F}$为有限阶的域和$\sigma$自同构。 $\sigma$ 的不变量域 E 也是 $\sigma$ 生成的阶 $n$ 的循环群的不变量域，因此 (V, p. 66, Th. 3) F 为E 的次数 $n$ 的循环扩张。

我们知道（I，p. 50）循环群的每个*子群*和每个*商群*都是循环的。因此（V，p. 68，Cor.4），如果E是域K、次数$n$的循环扩张，则E的每个子扩展F都是*K*上的循环，并且*E是F*上的循环。对于 $n$ 的每个除子 d，在 E 中包含的 K 上都存在一个唯一的次数 d 子域 F：对于阶 $n$ 的循环群，存在一个唯一的子群指标d。

#### 定理 3（*希尔伯特*）{#alg-v-s11-thm-3 .statement tag=06OX}

— *令 E 为 K 的循环扩张，并令 a 为 E 在 K 上的伽罗瓦群 $\Gamma$ 的生成元。

a) 对于元素$x \in E$到满足$N_{E/K}(x) = 1$，$y \in E^*$存在使得$x = y / \sigma(y)$是充分必要的；每个 $y_1 \in E^*$ 和 $x = y_1 / \sigma(y_1)$ 都是形式 $\lambda y$，其中 $\lambda \in K^*$。

b) 对于元素$x \in E$到满足$\mathrm{Tr}_{E/K}(x) = 0$，$z \in E$与$x = z - \sigma(z)$存在是充分必要的；那么每个$z_1 \in E$和$x = z_1 - \sigma(z_1)$都是形式$z + \mu$，其中$\mu \in K$。

我们先证明引理.*

#### 引理 4 {#alg-v-s11-lem-4 .statement tag=06OY}

*设$\Gamma$是阶$n$的循环群，$\Gamma$的$\sigma$生成元，M是可交换的群，其中$\Gamma$根据规则$\gamma . (m + m') = \gamma . m + \gamma . m'$对所有进行运算$\gamma \in \Gamma$ 和 $m, m' \in M$。设 Z 为 $\Gamma$ 的所有映射中的集合到 M 满足关系*

$$
f(\tau \tau') = f(\tau) + \tau . f(\tau') \quad \text{for } \tau, \tau' \text{ in } \Gamma
$$

将 $u(f) = f(a)$ 替换为 $f \in Z$，将 $t(m) = \sum_{\tau \in \Gamma} \tau . m$ 替换为 $m \in M$。然后序列

$$
0 \to Z \xrightarrow{u} M \xrightarrow{t} M
$$

是准确的。

设 $f \in \mathbf{Z}$；将$\tau = \tau' = 1$代入(10)，我们发现$f(1) = 0$。此外，通过$m \geqslant 0$上的归纳我们推导出关系

$$
f(\sigma^m) = f(\sigma) + \sigma \cdot f(\sigma) + \cdots + \sigma^{m-2} \cdot f(\sigma) + \sigma^{m-1} \cdot f(\sigma)
$$

我们有$\sigma^n = 1$、从而$f(\sigma^n) = 0$；前面的关系和$m = n$相当于等式$t(u(f)) = 0$、从而$\operatorname{Im}\ u \subset \operatorname{Ker}\ t$。此外，从(11)可以得出$\operatorname{Ker}\ u = 0$。

令$m \in M$使得$t(m) = 0$，即$m + \sigma \cdot m + \cdots + \sigma^{n-1} \cdot m = 0$。让我们将 $\Gamma$ 的定义映射 $f$ 化为$M$

$$
f(\sigma^j) = m + \sigma \cdot m + \cdots + \sigma^{j-2} \cdot m + \sigma^{j-1} \cdot m
$$

$0 \leqslant j \leqslant n - 1$。可以留给读者来建立关系(10)。我们显然有$m = f(a)$，从而$\operatorname{Im}\ u \supset \operatorname{Ker}\ t$。

引理现已证明，让我们取$y \in E^*$和$x = y/\sigma(y)$；我们有$N_{E/K}(\sigma(y)) = N_{E/K}(y)$，从而$N_{E/K}(x) = 1$。相反，令$E^*$中的$x$使得$N_{E/K}(x) = 1$；将引理 4应用于$M = E^*$，$\Gamma$和$c_\sigma = x$中存在$\tau, \tau'$的$E^*$满足关系$c_{\tau \tau'} = c_\tau \cdot \tau(c_{\tau'})$族元素$(c_\tau)_{\tau \in \Gamma}$。由科.提案 9 的第 1 条（V，p. 65）对于所有$\tau \in \Gamma$，从而，特别是$x = c_\sigma = y/\sigma(y)$，都存在$y \in E^*$和$c_\tau = y/\tau(y)$。如果$y_1 \in E^*$满足$x = y_1/\sigma(y_1)$，那么我们有

$$
\sigma(y_1 y^{-1}) = y_1 y^{-1},
$$

因此$y_1 y^{-1}$属于到$K^*$，因为$a$生成伽罗瓦群超过$E$超过$K$。这就证明了a）。

断言 b) 以类似的方式来自 Cor。第 9 号提案第 2 条（V、p. 65）。

### 7. $\mathbf{Z}/n\mathbf{Z}$-模块的对偶性

在这个编号中，我们用$n$整数$> 0$和$T$表示阶$n$的循环群。如果$g^n = 1$对于所有$g \in G$来说，群$G$据说会被$n$消灭；此外，如果$G$是可交换的，$G$的群结构是一个独特的$\mathbf{Z}/n\mathbf{Z}$模块结构的基础。

对于每个群$G$，我们用$G$的同态的$\operatorname{Hom}(G, T)$群表示为$T$；它是一个被 $n$ 湮没的交换律群。

#### 命题 7 {#alg-v-s11-prop-7 .statement tag=06OZ}

— 设 $G$ 为 $G$ 的交换律群，被 $n$ 和 $H$ 子群湮灭。那么限制同态 $\operatorname{Hom}(G, T) \to \operatorname{Hom}(H, T)$ 是满射。

让 $f : H \to T$ 为同态；我们将证明存在$G$到$T$延伸$f$的同态。 首先假设$G$是循环的，由阶$r$除$n$生成元素$g$；用 $T$ 的 $t$ 生成元表示。 r 存在除子 s，使得 H 由 $g^s$（I、p. 50，命题 19）生成，并且对于每个$x \in \mathbf{Z}$，我们有 $f(g^{sx}) = t^{ax}$，其中 a 是整数，使得 n 除 $ar/s$。 那么$a/s = (ar/ns)(n/r)$就是G的整数和同态$g^x \mapsto t^{(a/s)x}$，$x \in \mathbf{Z}$，变成T扩展f。 在一般情况下，考虑对$(H', f')$的集合，其中$H'$是G包含H的子群，$f'$是$H'$的同态延伸到$f$，让我们阶这个如果$f''$至$H'$中的$H' \subset H''$和限制为$f'$，则集合乘以关系$(H', f') \leq (H'', f'')$。 根据集合理论，III，p. 154，Def。 3和Th。 2、这个集合有极大元素$(H_1, f_1)$，只要证明$H_1 = G$即可；如果不是，则存在$g \in G, g \notin H_1$，并且足以证明$f_1$可以扩展到由$H_1$和g生成的G的子群的同态 T。 现在，如果C表示由g生成的循环群，则$f_1$的限制到$C \cap H_1$扩展到C的同态$f_2$进入T和同态$xy \mapsto f_1(x) f_2(y), x \in H_1, y \in C,$将$H_1C$代入T就是所需的映射。

#### 推论 1 {#alg-v-s11-prop-7-cor-1 .statement tag=06P0}

— 如果 G * 是 * 被 *n* 和 $G \neq \{1\}$ 湮没的交换律群，则 $\mathrm{Hom}(G, T) \neq \{1\}$。

因为只要注是，如果H是不同于$\{1\}$的G的循环子群，则$\mathrm{Hom}(H, T) \neq \{1\}$，并应用命题7。

#### 推论 2 {#alg-v-s11-prop-7-cor-2 .statement tag=06P1}

— 如果 G *是*一个*有限*交换律群被 *n* 湮灭，则群 G 和 $\mathrm{Hom}(G, T)$ 具有相同的阶。

如果 G 是阶 *r* 的循环，其中生成元 g，则映射 $f \mapsto f(g)$ 是 $\mathrm{Hom}(G, T)$ 的双射到 T 的元素 t 的集合，使得 $t^r = 1$，因此在这种情况下是断言。另一方面，如果 H 是 G 的循环子群，则有 $\mathrm{Card}(G) = \mathrm{Card}(H) \cdot \mathrm{Card}(G/H)$；此外，我们还有正合序列

$$
\{1\} \to \mathrm{Hom}(G/H, T) \to \mathrm{Hom}(G, T) \to \mathrm{Hom}(H, T) \to \{1\}
$$

（II、p. 227、Th.1 和上述 Prop.7），因此

$$
\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(\mathrm{Hom}(H, T)) \cdot \mathrm{Card}(\mathrm{Hom}(G/H, T)).
$$

从$\mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H)$开始，证明G或$G/H$的推论是相同的。现在结果是 $\mathrm{Card}(G)$ 上的归纳。

现在让 G 和 H 是两个群和 $f : G \times H \to T$ 一个双乘映射，也就是说，对于任何 $g, g' \in G, h, h' \in H$ 我们有

$$
f(gg', h) = f(g, h) f(g', h), \quad f(g, hh') = f(g, h) f(g, h')
$$

我们定义群同态

$$
s_f : G \to \mathrm{Hom}(H, T), \quad d_f : H \to \mathrm{Hom}(G, T),
$$

由 $s_f(g)(h) = d_f(h)(g) = f(g, h)$ (cf. II, p. 268，适用于命题 1，当 G 和 H 是可交换的时)。

#### 命题 8 {#alg-v-s11-prop-8 .statement tag=06P2}

— *假设 G 和 H 是可交换的并且被 n 湮灭。如果 s_f 是双射且 H 是有限的，则 d_f 是双射并且我们有 Card(G) = Card(H).*

如果 s_f 是双射且 H 是有限的，则我们有 Cor 。 2 到命题 7 关系 Card(G) = Card(Hom(H, T)) = Card(H)，因此 Card(G) 是有限的，并且通过另一个应用推论，Card(Hom(G, T)) = Card(H)。所以只要证明d_f是单射的就足够了。现在，如果 h \in \mathrm{Ker}(d_f)，则对于所有 g \in G，我们有 f(g, h) = 1，因此由于 s_f 是双射的，因此对于所有 \varphi \in \mathrm{Hom}(H, T)，\varphi(h) = 1；根据命题 7，这意味着 \mathrm{Hom}(\mathrm{Ker}(d_f), T) = \{1\}，因此 \mathrm{Ker}(d_f) = \{1\} 1 至提案 7。

### 8.库默理论

在这个数中，我们用$n$整数>0表示，并且我们假设$\mu_n(K)$有$n$元素；由 V, p. 78 这也意味着 $n$ 与 K 的特征指数互质，并且 K 的代数闭包 $\Omega$ 中单位元的所有 n 个根都位于 K 中。

We shall say that an extension L of K is *abelian of exponent dividing n* if it is abelian (V, p. 77, Def. 1) and its Galois group Gal(L/K) is annihilated by $n$ (V, p. 86).

设 A 为 $K^*$ 的子集；我们用$K(A^{1/n})$表示由所有$0 \in \Omega$生成的$\Omega$的子扩展，使得$\theta^n \in A$。

#### 引理 5 {#alg-v-s11-lem-5 .statement tag=06P3}

— *$K(A^{1/n})$ 是指数除以 n 的 K 的阿贝尔的扩张。*

由于多项式 $X^n - a, a \in A$ 在 K 上可分，因此 $L = K(A^{1/n})$ 是可分的，因此 K 的伽罗瓦扩张。令 $\sigma \in \mathrm{Gal}(L/K)$ 并令 $0 \in \Omega$ 使得 $\theta^n \in A$。我们有$\sigma(\theta)^n = \theta^n$；因此存在$\zeta \in \mu_n(\Omega) = \mu_n(K)$使得$\sigma(\theta) = \zeta \theta$；这意味着$\sigma^n(\theta) = \zeta^n \theta = 0$，从而$\sigma^n = 1$。如果$\sigma'$是$\mathrm{Gal}(L/K)$的另一个元素，则存在$\zeta' \in \mu_n(K)$使得$\sigma'(\theta) = \zeta' \theta$，从而$\sigma'\sigma(\theta) = \zeta \zeta' \theta = \sigma\sigma'(\theta)$等等$\sigma'\sigma = \sigma\sigma'$。

#### 引理 6 {#alg-v-s11-lem-6 .statement tag=06P4}

— *令L为K的伽罗瓦扩张。$\mathrm{Gal}(L/K) \times ((L^n \cap K^*)/K^{*n})$存在唯一映射$(\sigma, a) \mapsto \langle \sigma, a \rangle$进入$\mu_n(K)$，使得对于每个$\sigma \in \mathrm{Gal}(L/K)$和每个元素$0 \in L^*$，使得$\theta^n \in K$我们有，表示为$\overline{\theta^n}$ 剩余类类 $\theta^n$ mod $K^{*n}$:*

$$
\langle \sigma, \overline{\theta^n} \rangle = \sigma(\theta)/\theta
$$

*这个映射是双乘的。*

实际上，(13) 的右侧是单位元的第 n 个根，它仅​​取决于剩余类类 mod $K^{*n}$ of $\theta^n$；这就证明了第一个断言。第二个断言毫无困难地得到验证。

对于 K 的每个伽罗瓦扩张 L 让我们写

$$
k_L : (L^n \cap K^*)/K^{*n} \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mu_n(K)) ,
$$
$$
k'_L : \mathrm{Gal}(L/K) \to \mathrm{Hom}((L^n \cap K^*)/K^{*n}, \mu_n(K)) ,
$$

对于同态由上述二乘映射 (V, p. 87) 导出。

#### 命题 9 {#alg-v-s11-prop-9 .statement tag=06P5}

*对于 K 的有限次数 L 的每个伽罗瓦扩张，同态 $k_L$ 是双射的。*

令$0 \in L^*$满足$0^n \in K$和$0^n \mod K^{*n}$属于的剩余类类到$k_L$的核。 对于每个 $\sigma \in \mathrm{Gal}(L/K)$，我们有定义 $\sigma(\theta) = 0$；因此$0 \in K^*$和$\theta^n \in K^{*n}$。 这就证明了$k_L$的单射性。 现在令$f : \mathrm{Gal}(L/K) \to \mu_n(K)$为同态；对于所有 $\sigma, \tau \in \mathrm{Gal}(L/K)$ 我们有

$$
f(\sigma \tau) = f(\sigma) f(\tau) = f(\sigma) \cdot \sigma f(\tau) , \quad f(\sigma)^n = 1 .
$$

V，p. 65，Cor。 1 存在 $0 \in L^*$ 使得 $f(\sigma) = \sigma(\theta)/\theta$ 对于所有 $\sigma \in \mathrm{Gal}(L/K)$；从$f(\sigma)^n = 1$开始，我们对所有$\sigma \in \mathrm{Gal}(L/K)$都有$\sigma(\theta^n) = 0^n$，因此$0^n \in K^*$；如果$a$是$\theta^n \mod K^{*n}$的剩余类类，我们通过定义$f(\sigma) = \langle \sigma, a \rangle$得到$\sigma \in \mathrm{Gal}(L/K)$，因此$f = k_L(a)$。

#### 推出{#alg-v-s11-n8-cor-1 .statement tag=06P6}

*如果L是K的伽罗瓦扩张，则同态$k_L$是单射，其像是拓扑群$\mathrm{Gal}(L/K)$的连续同态到离散群的群$\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mu_n(K))$ $\mu_n(K)$.*

根据上述事实，L 是递增定向伽罗瓦扩张 $L_i$ 有限次数的并，并且$\mathrm{Gal}(L/K)$ 到$\mu_n(K)$ 的同态是连续的，当且仅当它可以通过其中一个商因式分解时$\mathrm{Gal}(L_i/K)$ / $\mathrm{Gal}(L/K)$。

#### 定理 4 {#alg-v-s11-thm-4 .statement tag=06P7}

*a) The mapping $H \mapsto K(H^{1/n})$ is an inclusion preserving bijection of the set of subgroups of $K^*$ containing $K^{*n}$ onto the set of abelian subextensions of exponent dividing n of $\Omega$. 映射的逆元是 $L \mapsto L'' \cap K^*$。

b) 对于$K^*$包含$K^{*n}$同态的每个子群H

$$
k' : \mathrm{Gal}(K(H^{1/n})/K) \to \mathrm{Hom}(H/K^{*n}, \mu_n(K))
$$

是双射的，当群$\mathrm{Hom}(H/K^{*n}, \mu_n(K))$配备简单收敛的拓扑时，它是同胚。

c) 设 H 为 $K^*$ 包含 $K^{*"n}$ 中的子群。对于每个$a \in H/K^{*n}$，令$\theta_a$为$\Omega$的元素，使得$\theta_a^n$是H中a的代表。然后是向量K空间$K(H^{1/n})$的$\theta_a, a \in H/K^{*n}$、形式基。尤其，

$$
[K(H^{1/n}):K] = (H:K^{*"n}) .
$$

A) 对于除以 n 的指数 K 的每个阿贝尔的扩张 L，让我们放入 $H_L = L'' \cap K^*$。如果 $[L:K]$ 是有限的，则 $\mathrm{Gal}(L/K)$ 到 $\mathrm{Hom}(H_L, \mu_n(K))$ 的同态 $k'_L$ 根据命题 9 和 V、p. 88、命题 8 是双射的。

由于指数除法$n$的K的每个阿贝尔的扩张都是指数除法$n$的阿贝尔的有限次数的递增有向并的子扩展，我们通过逆极限推论$k'_L$是一个对于 K 除 n 的每个阿贝尔的扩张 L，拓扑群同胚。

B) 令L为K的指数除以$n$的有限次数的阿贝尔的扩张，并令$L' = K(H_L^{1/n})$；这是 L 的子扩展；而且$H_{L'}$包含于$H_L$所以等于它。由于同态 $k'_L$ 和 $k'_{L'}$ 是 A) 和 $H_L = H_{L'}$ 的双射，群 Gal$(L/K)$ 和 Gal$(L'/K)$ 具有相同的阶，因此相等。这表明$L' = L$，因此也表明$L = K(H_L^{1/n})$。如果L是K的指数除以$n$的阿贝尔的扩张，我们有$K(H_L^{1/n}) = L$，因为$K(H_L^{1/n})$是L的子扩展，其中包含每个有限次数的子扩展L。

C) 设H为$K^*$包含于$K^{*n}$中的子群；放入$L = K(H^{1/n})$，则这是指数除$n$（V，p. 88，引理 5）的K的阿贝尔的扩张。我们有$H \subset H_L$，从而，我们获得交换性群被$n$消灭的正合序列

$$
\{1\} \to H/K^{*n} \to H_L/K^{*n} \to H_L/H \to \{1\}.
$$

由此我们得到正合序列

$$
\{1\} \to \operatorname{Hom}(H_L/H, \mu_n(K)) \to \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) \xrightarrow{\iota} \operatorname{Hom}(H/K^{*n}, \mu_n(K)),
$$

其中 $\iota$ 是限制同态。

如果我们通过同构$k'_L$将认同$\operatorname{Hom}(H_L/K^{*n}, \mu_n(K))$与Gal$(L/K)$一起使用，则$\iota$的核与$\sigma \in \operatorname{Gal}(L/K)$的集合进行识别，使得$\sigma(\theta) = \theta$对于所有$\theta \in H^{1/n}$。由此可见 $\iota$ 是单射的，因此 $\operatorname{Hom}(H_L/H, \mu_n(K))$ 被简化为 (1) ；由科. V、p. 87 中的 1 个，因此我们有 $H = H_L$。这样就完成了 a) 和 b) 的证明。

D）让我们证明c）。如果$a, b \in H$，我们有$\theta_a \theta_b / \theta_{ab} \in K$。由此可见，$\theta_a$生成的$K(H^{1/n})$的向量子空间在乘法下是稳定的，因此重合与$K(H^{1/n})$是稳定的。只需要证明 $\theta_a$ 是线性无关的；为此，我们显然可以假设 $H/K^{*n}$ 是有限的；然后 $[K(H^{1/n}) : K] = (\operatorname{Gal}(K(H^{1/n})/K) : \{1\}) = (H : K^{*n})$ 由 b) 和 Cor。 2 个V、p. 87；由于$\theta_a$的数等于$(H : K^{*n})$，并且它们生成向量K空间$K(H^{1/n})$，因此它们是线性独立的。

#### 例 1 {#alg-v-s11-n8-exa-1 .statement tag=06P8}

$\Omega$ 中包含 K 的指数除以$n$，存在最大的阿贝尔的扩张；它是通过将所有元素中的第 n 个根与 K 邻接而获得的；它的伽罗瓦群可以与$\operatorname{Hom}(K^*/K^{*n}, \mu_n(K))$识别，因此也可以与$\operatorname{Hom}(K^*, \mu_n(K))$识别。

#### 例 2 {#alg-v-s11-n8-exa-2 .statement tag=06P9}

\* 让我们取$K = \mathbf{Q}$和$n = 2$。那么$\mathbf{Q}^*/\mathbf{Q}^{*2}$是向量$\mathbf{F}_2$-空间，其中$\{-1\}$和所有素数数的基并和集合。因此$\mathbf{C}$中包含的Q的指数2的最大的阿贝尔的扩张是$\mathbf{C}$的子域$\mathbf{Q}(i, \sqrt{2}, \sqrt{3}, \sqrt{5}, \ldots)$。它的伽罗瓦群由元素$i,\ \sqrt{2},\ \sqrt{3},\ \sqrt{5}$等乘以$\pm 1$得到的所有自同构组成。 \*

#### 例 3 {#alg-v-s11-n8-exa-3 .statement tag=06PA}

令L为次数$n$的K的循环扩张；那么群$(L^n \cap K^*)/K^{*n}$是阶$n$的循环。如果$a \in K^*$使得$a$ mod $K^{*n}$的剩余类类是群的生成元，则L与$K[X]/(X^n - a)$是K同构，并且群$\mathrm{Gal}(L/K)$由$n$自同构映射$X$至$\zeta X$、$\zeta \in \mu_n(K)$。

#### 例 4 {#alg-v-s11-n8-exa-4 .statement tag=06PB}

相反，令 $a \in K^*$ 并令 $r$ 至少为整数 $> 0$，使得 $a' \in K^{*n}$；那么由多项式$X^n - a$的根生成的$\Omega$的子域$L$是次数$r$的$K$的循环扩张。特别是，当且仅当$r = n$时，$X^n - a$是不可约的。

#### 注 {#alg-v-s11-n8-rem-1 .statement tag=06PC}

令 $a \in K^*$ 且令 r 最小为整数 $> 0$，使得 $a' \in K^n$。令B为多项式$X^{n/r} - a$的K中根的集合；那么我们有

$$
X^n - a = \prod_{b \in B} (X' - b),
$$

关系 $T^{n/r} - a = \Pi (T - b)$ 中的 T 为 $X'$ 的代换。到例 4，每个多项式 $X' - b$ 都是不可约的，因此 (14) 是 $X^n - a$ 的分解变为 $K[X]$ 中的不可约多项式。

### 9.Artin-Schreier理论

在这个数中，我们将使用$p$来表示素数数，并假设K具有特征$p$。我们用 K 的 $\Omega$ 代数闭包和 $\Omega$ 的加法群 $\varphi$ 自同态表示，定义为

$$
\varphi(x) = x^p - x.
$$

通过V，$\varphi$的p. 93核是$K$的质数子域$\mathbf{F}_p$。对于 K 的每个子集$A$，我们用$K(\varphi^{-1}(A))$表示由所有$x \in \Omega$生成的$\Omega$的子扩展，使得$\varphi(x) \in A$。

#### 引理 7 {#alg-v-s11-lem-7 .statement tag=06PD}

$K(\varphi^{-1}(A))$是指数除$p$的$K$阿贝尔的扩张。

由于多项式 $\varphi - a = X^p - X - a,\ a \in A$ 在 $K$ 上可分，因此扩张 $L = K(\varphi^{-1}(A))$ 是伽罗瓦。设$a \in \mathrm{Gal}(L/K)$和$x \in \varphi^{-1}(A)$；我们有$\varphi(\sigma(x)) = \varphi(x)$，因此有$\sigma(x) - x \in \mathbf{F}_p$，即$\sigma(x) = x + i,\ i \in \mathbf{F}_p$。这意味着$\sigma^p(x) = x + pi = x$，因此$u^p = 1$；类似地，如果$a' \in \mathrm{Gal}(L/K)$和$\sigma'(x) = x + j$，那么我们有$\sigma \circ \sigma'(x) = x + i + j = a' \circ \sigma(x)$，所以$\sigma \circ \sigma' = \sigma' \circ \sigma$。

#### 引理 8 {#alg-v-s11-lem-8 .statement tag=06PE}

令L为K的伽罗瓦扩张。$\mathbf{F}_p$中存在$\mathrm{Gal}(L/K) \times ((\varphi(L) \cap K)/\varphi(K))$的唯一映射$(\sigma, a) \mapsto [a, a')$，使得对于所有$\sigma \in \mathrm{Gal}(L/K)$和每个元素$x \in L$，使得$\varphi(x) \in K$我们有，表示为$\overline{\varphi(x)}$ 剩余类类 $\varphi(x)$ mod $\varphi(K)$，

$$
[\sigma, \overline{\varphi(x)}] = \sigma(x) - x.
$$

这个映射是Z双线性的（对于$\sigma, \tau \in \mathrm{Gal}(L/K)$，$a, b \in (\mathscr{P}(L) \cap K)/\mathscr{P}(K)$，我们有$[\sigma \tau, a) = [\sigma, a) + [\tau, a)$，$[\sigma, a + b) = [\sigma, a) + [a, b)$）。

对于(15)的右侧是$\mathbf{F}_p$的元素，它仅​​取决于$\mathscr{P}(x) \mod \mathscr{P}(K)$的剩余类类；这就证明了第一个断言；第二个可以毫无困难地验证。

对于$K$的每个伽罗瓦扩张$L$让我们写

$$
a_L : (\mathscr{P}(L) \cap K)/\mathscr{P}(K) \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mathbf{F}_p)
$$
$$
a_L' : \mathrm{Gal}(L/K) \to \mathrm{Hom}((\mathscr{P}(L) \cap K)/\mathscr{P}(K), \mathbf{F}_p)
$$

对于同态，从上述Z-双线性映射（V，p. 87）获得。

#### 命题 10 {#alg-v-s11-prop-10 .statement tag=06PF}

*对于$K$的有限次数的每个伽罗瓦扩张$L$，同态$a_L$是双射的。*

令$x \in L$使得$\mathscr{P}(x) \mod \mathscr{P}(K)$的$\mathscr{P}(x) \in K$和剩余类类位于$a_L$的核中。对于每 $\sigma \in \mathrm{Gal}(L/K)$，我们有定义 $\sigma(x) = x$；因此$x \in K$和$\mathscr{P}(x) \in \mathscr{P}(K)$。这就证明了$a_L$的单射性。现在令$f : \mathrm{Gal}(L/K) \to \mathbf{F}_p$为同态；对于所有 $\sigma, \tau \in \mathrm{Gal}(L/K)$ 我们有

$$
f(\sigma \tau) = f(\sigma) + \sigma(f(\tau)), \quad f(\sigma) \in \mathbf{F}_p.
$$

V，p. 65，Cor。 2 存在$x \in L$，使得$f(u) = \sigma(x) - x$对于所有$o \in \mathrm{Gal}(L/K)$。由于$f(o) \in \mathbf{F}_p$我们有$\mathscr{P}(\sigma(x)) = \mathscr{P}(x)$，因此对于所有$a \in \mathrm{Gal}(L/K)$和$\mathscr{P}(x) \in K$都有$\sigma(\mathscr{P}(x)) = \mathscr{P}(x)$。如果$a$是$\mathscr{P}(x) \mod \mathscr{P}(K)$的剩余类类，我们有$f(\sigma) = [\sigma, a)$，所以$f = a_L(a)$。

#### 推论{#alg-v-s11-n9-cor-1 .statement tag=06PG}

*如果$L$是$K$的伽罗瓦扩张，则同态$a_L$是单射，其像是拓扑群$\mathrm{Gal}(L/K)$的连续同态到离散的群$\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mathbf{F}_p)$ 群$\mathbf{F}_p$.*

这与 Cor 的证明方式相同。提案 9，V，p. 89。

#### 定理 5 {#alg-v-s11-thm-5 .statement tag=06PH}

*a) The mapping $A \mapsto K(\mathscr{P}^{-1}(A))$ is a bijection of the set of subgroups of $K$ containing $\mathscr{P}(K)$ onto the set of abelian subextensions of exponent dividing $p$ in $\Omega$. 映射的逆元是 $L \mapsto \mathscr{P}(L) \cap K$。
b) 对于 $K$ 包含于 $\mathscr{P}(K)$ 中的每个子群 $A$，同态

$$
a' : \mathrm{Gal}(K(\mathscr{P}^{-1}(A))/K) \to \mathrm{Hom}(A/\mathscr{P}(K), \mathbf{F}_p)
$$

是双射的，当$\mathrm{Hom}(A/\mathscr{P}(K), \mathbf{F}_p)$配备简单收敛的拓扑时，它是同胚。
c) 设$A$为$K$包含于$\mathscr{P}(K)$的子群，并令$B$为向量$\mathbf{F}_p$-空间$A/\mathscr{P}(K)$的基。对于每个$a \in B$，令$x_a$为$\Omega$的元素，使得$\mathscr{P}(x_a)$是$A$中$a$的代表。然后单项式 $x^\alpha = \prod_{a \in B} x_a^{\alpha(a)}$ 与 N^{(B)} 中的 a = (\alpha(a)) 使得 0 \leq \alpha(a) < p 对于向量 K 空间 K(\mathfrak{p}^{-1}(A)) 的 B 形式基中的每个 a \。特别是我们有 [K(\mathfrak{p}^{-1}(A)):K] = (A:\mathfrak{p}(K))。

Th。 5 的证明方法与 Th 相同。 4 (V, p. 89) 已作必要修改。

#### 例 1 {#alg-v-s11-n9-exa-1 .statement tag=06PI}

存在除 p 的指数 K 最大的阿贝尔的扩张，包含在 \Omega 中；是K(B^1(K))，它的伽罗瓦群可以用Horn(K/\mathfrak{p}(K),\mathbf{F}_p)来表示。

#### 例 2 {#alg-v-s11-n9-exa-2 .statement tag=06PJ}

设L为次数p的K的循环扩张；那么群 (\mathfrak{p}(L) \cap K)/\mathfrak{p}(K) 是阶 p 的循环。如果 \in K 使得 mod \mathfrak{p}(K) 的剩余类类是该群的生成元，则 L 与 K[X]/(X^p - X - a) 是 K 同构的，并且伽罗瓦群 Gal(L/K) 由 p 自同构映射 X 到 X + i，i \in \mathbf{F}_p 组成。

#### 例 3 {#alg-v-s11-n9-exa-3 .statement tag=06PK}

反之，如果 a \in K - \mathfrak{p}(K)，则多项式 X^p - X - a 是不可约的，由其根生成的 \Omega 的子域 L 是次数 p 的 K 的循环扩张。如果 a \in \mathfrak{p}(K)，则 X^p - X - a = \prod_{a \in \mathfrak{p}^{-1}(a)} (X - \alpha)。

### 习题{#alg-v-s11-exercises}

§ 11](exercises/s11/)参见[习题。
