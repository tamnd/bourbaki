---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 6
section_title: Borel's graph theorem
lang: zh
source: evt-i-v
book_pages: TVS III.49-TVS III.50
pdf_pages: 0166-0169, 0181-0182
extraction: ocr
subsections:
    - "no": 1
      title: Borel’s graph theorem
      page: 34
      pdf_page: 166
    - "no": 2
      title: Locally convex Lusin spaces
      page: 34
      pdf_page: 166
    - "no": 3
      title: Measurable linear mappings on a Banach space $^1$
      page: 36
      pdf_page: 168
statements: 8
exercises: 6
content_sha256: 4563993593351606b30845ffc46379b5c26c1f8fdc5518631ddb4381ccf12d54
translated_from: content/en/evt/III/06_s6_borel_s_graph_theorem.md
translation_method: google
source_content_sha256: 207efa273694316acd7d5b27dedee7a3292c04e1a0a2e90cfe57fd450ad44773
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 085998502d265cd6bc715185083805e6f15251679f7c06dd37f325173263eb6e
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 6。 Borel 的图定理

### 1. Borel 的图定理

#### 定理 1 {#evt-iii-s6-thm-1 .statement tag=07Q4}

— 令 E 为局部凸空间，它是 Banach 空间的归纳极限，F 为苏斯林局部凸空间，例如 Lusin 空间（GT、IX, § 6, No. 2 和 No. 4），以及从 E 到 F 的 u 线性映射。如果 u 的图是 Borel E × F 的子集，则 u 是连续的。

令 E_i 为 Banach 空间的族，并且 (u_i) 为连续线性映射 u_i 的族：E_i → E，使得 E 的拓扑是 u_i 连续的最佳局部凸拓扑。足以证明组合的映射 u ∘ u_i 是连续的，或者事实上（GT，IX, § 2, No. 6，命题 10）u ∘ u_i 的限制到 E_i 满足的每个闭子空间 G 可数性第一公理是连续的。这个限制的图是 u 在连续映射 u_i × Id_F : G × F → E × F 下的图的逆像，因此是 G × F 中的一个 Borel 集合。 在加法中，G × F 是一个 Souslin 空间并且每个 Borel苏斯林空间的子集是苏斯林空间（GT，IX, § 6, No. 3，道具 10）。 Th。然后从 th 得出 1。 4、GT，IX, § 6, No. 8。

#### 注 {#evt-iii-s6-n1-rem-1 .statement tag=07Q5}

回想一下 (III, p. 12)，每个同调 Hausdorff 和半完备空间，例如每个 Fréchet 空间，都是 Banach 空间的归纳极限。 \* 对于自反 Fréchet 空间的强对偶也是如此（IV，p. 23，道具 4）。 \*

### 2. 局部凸 Lusin 空间

#### 命题 1 {#evt-iii-s6-prop-1 .statement tag=07Q6}

— 令 E 为 Hausdorff 局部凸空间。假设存在 Fréchet 空间满足可数性第一公理序列 (E_n)_{n \in \mathbf{N}}，且连续线性映射 u_n : E_n → E 使得 E = \bigcup_{n \in \mathbf{N}} u_n(E_n)。那么 E 是 Lusin 空间。

令 P_n 为 u_n 的核；那么 u_n 定义是从商空间 E_n/P_n 到 u_n(E_n) 的双射连续映射。 由于 E_n/P_n 是 Fréchet 空间满足可数性第一公理 (GT, IX, § 3, No. 1)，因此波兰语空间 (GT, IX, § 6, No. 1, def. 1)，u_n(E_n) 是 E (GT, IX, § 6, No. 4, prop. 1) 的 Lusin 子空间。 11）。 因而，根据 GT，IX, § 6, No. 7，cor。的。 3、空间 E，常规（GT，III, § 3, No. 1）是 Lusin 空间。

#### 例 1 {#evt-iii-s6-n2-exa-1 .statement tag=07Q7}

每个 Fréchet 空间满足可数性的第一公理都是波兰语空间，因此是 Lusin 空间。因而，空间$\mathscr{C}(X)$也是如此，其中X是局部紧致的并且具有可数基（$\mathscr{C}(X)$的拓扑是紧致收敛的，cf.GT，X, § 3, No. 3，推论和§ 1, No. 6，cor.3）； \* 空间 $\mathscr{C}_0^\infty(U)$，其中 U 是 $\mathbf{R}^n$ (III, p. 9) 的开子集和 $\mathscr{H}(U)$，其中 U 是 $\mathbf{C}^n$ (III, p. 10) 的开子集。

命题1表明空间$\mathscr{C}_0^\infty(U)$，其中U是$\mathbf{R}^n$中的开集合，$\mathscr{G}_s(I)$，其中I是$\mathbf{R}$和$s \geq 1$中的紧区间，以及$\mathscr{H}(K)$，其中K是紧$\mathbf{C}^n$中的子集都是Lusin空间（III，p. 10）。 \*

#### 定理 2 {#evt-iii-s6-thm-2 .statement tag=07Q8}

— 令 E 为局部凸空间，它是 E 的递增序列 $(E_n)_{n \in \mathbf{N}}$ 的子空间的归纳极限，赋予可数性第一公理 Fréchet 空间满足的拓扑。假设E的每个紧致子集都包含在其中一个$E_n$中，并且在这个空间中是紧致的。设 F 为 Fréchet 空间满足，可数性第一公理。那么空间 $\mathscr{L}_c(E; F)$ 就是 Lusin 空间。

空间 E 是天生的 (III, p. 12)，因此空间 $\mathscr{L}_c(E; F)$ 是完整的 (III, p. 23, 命题 12)。 线性映射$j : f \mapsto (f|E_n)_{n \in \mathbf{N}}$是单射从$\mathscr{L}_c(E; F)$变为乘积空间$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$；根据E的紧致子集和$\mathfrak{S}$拓扑的定义上的假设，$j$是从$\mathscr{L}_c(E; F)$到其像的同构（赋予由乘积诱导的拓扑） 拓扑);此外，由于$\mathscr{L}_c(E; F)$是完备的，所以这个像是$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$的闭子空间（GT，II, § 3, No. 4，道具8）。因而，通过GT，IX, § 6, No. 4，足以证明空间$\mathscr{L}_c(E; F)$中的每一个都是Lusin空间。对于证明的其余部分，我们假设 E 是 Fréchet 空间满足可数性第一公理。

由于 F 是可数第一公理 Fréchet 空间满足，因此它同构于 Banach 空间 $F_n$ 的可数乘积的闭子空间，其中每个商都是 F (II， p. 5)，因此满足可数性第一公理。 线性映射$j' : f \mapsto (\mathrm{pr}_n \circ f)_{n \in \mathbf{N}}$是从$\mathscr{L}_c(E; F)$到乘积空间$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F_n)$的单射，并且通过使用$\mathfrak{S}$拓扑的定义和乘积中的开放集合， $j'$是从$\mathscr{L}_c(E; F)$到像的同构；而且，由于$\mathscr{L}_c(E; F)$是完备的，所以这个像是$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F)$的闭子空间。因而，只需证明空间 $\mathscr{L}_c(E; F_n)$ 中的每一个都是 Lusin 空间 (GT, IX, § 6, No. 4)，因而，我们可以假设 F 是 Banach 空间满足可数性第一公理。

空间 $\mathscr{L}_c(E; F)$ 是并等连续且封闭的子集可数族（III、p. 19，cor. 1 和 GT、X, § 2, No. 3、道具 6）。但是 $\mathscr{L}_c(E; F)$ 的每个等连续子集 H 都是可度量的，并且满足可数性第一公理（III，p. 18，第 6 条和 GT，X, § 2, No. 4，第 1 条）；如果 H 是闭集，那么它是由 $\mathscr{L}_c(E; F)$ 的制服结构引发的完整空间，因为后者是完整的 在其他字中，H 是波兰语空间，并且 *更不必说* 是 Lusin 空间；因而，常规的空间 $\mathscr{L}_c(E; F)$ 是 Lusin 空间（GT，IX, § 6, No. 7，第 3 个的对应）。

#### 推论 {#evt-iii-s6-n2-cor-1 .statement tag=07Q9}

— *关于 E 的假设与 th 中一样。 2、假设，在加法中，E的每个有界子集都是相对紧的。那么 E 的强对偶是 Lusin 空间。* *特别是，Fréchet 空间满足的强对偶可数性第一公理，也是 Montel 空间，是 Lusin 空间。*

\* 例 2. — 令 U 为 $\mathbf{R}^n$ 的开子集。 推论特别适用于 Fréchet 空间 $E = \mathscr{C}_c^\infty(U)$；那么它的对偶$\mathscr{C}_c^{-\infty}(U)$（在U上具有紧凑支持的发行版的空间）就是Lusin空间。

空间 $\mathscr{C}_c^\infty(U)$ 是 Fréchet 空间 $\mathscr{C}_{K_n}^\infty(U)$ 满足序列的严格归纳极限可数性第一公理 (III, p. 9)。我们可以证明每个空间$\mathscr{C}_{K_n}^\infty(U)$都是Montel空间；在加法中，$\mathscr{C}_c^\infty(U)$的每个有界子集都包含在空间$\mathscr{C}_{K_n}^\infty(U)$之一（III，p. 5，道具6）。然后我们可以应用 th 的推论。 2. 那么$\mathscr{C}_c^\infty(U)$（U 上的分布空间）的对偶$\mathscr{C}_c^{-\infty}(U)$ 是强拓扑的Lusin 空间。

类似地，我们证明对于$\mathbf{C}^n$的每个开子集U，以及对于$\mathbf{C}^n$的每个紧子集K，$\mathscr{H}(U)$的强对偶和$\mathscr{H}(K)$的强对偶是Lusin空间。 \*

#### 注 {#evt-iii-s6-n2-rem-1 .statement tag=07QA}

— 设 E 与 th 相同。 2；设 F 为 Hausdorff 局部凸空间，即连续线性映射 $u_n : F_n \to F$ 序列像并，其中每个 $F_n$ 是 Fréchet 空间满足第一个公理可数性；那么 $\mathscr{L}_c(E ; F)$ 就是 Lusin 空间。正如在道具中一样。 1、我们首先将约化变为每个$u_n$都是单射的情况；然后，如第证明所示。 2、我们可以假设E是Fréchet空间满足可数性第一公理。然后，通过I，p. 20，道具。 1、$\mathscr{L}(E ; F)$是$\mathscr{L}(E ; F_n)$的并；此外，典范嵌入$\mathscr{L}_c(E ; F_n) \to \mathscr{L}_c(E ; F)$是连续的（GT，X, § 1, No. 4，道具3）。由于空间 $\mathscr{L}_c(E ; F_n)$ 中的每一个都是 Lusin 空间。 2, $\mathscr{L}(E ; F_n)$ 也是由 $\mathscr{L}_c(E ; F)$ 引起的拓扑的 Lusin 空间（GT，IX, § 6, No. 4，第 11 条）；因而 $\mathscr{L}_c(E ; F)$ 凭借 GT、IX, § 6, No. 7、推论是 Lusin 空间。 3.

### \*3。可在 Banach 空间 $^1$ 上测量线性映射

#### 命题 2 {#evt-iii-s6-prop-2 .statement tag=07QB}

— *设 E 为 Banach 空间，F 为从 E 到 F 的局部凸空间，u 线性映射。假设对于 F 的每个闭子集 B，E 的每个紧致子集 X 以及每个测度 $\mu$ X、交 $X \cap u^{-1}(B)$ 是 $\mu$ 可测量的。那么 u 是连续的。*

首先假设F是基域。对于E的每个紧凑子集X和X上的每个度量$\mu$，$u$到X的限制是$\mu$可测（INT，IV）。假设 $u$ 不连续。然后我们可以在E中找到点$(x_n)$的序列，这样对于每个整数$n$都有$\sum_n \| x_n \| < \infty$和$|u(x_n)| \geq n$。考虑从立方体 $C = [0, 1]^{\mathbf{N}}$ 到 E 中的映射 $g : (t_n) \mapsto \sum_n t_n x_n$；显然$g$是连续的。因而，$f = u \circ g$对于C（INT，V）上的每个度量都是可测量的；特别是测量$\mu$，它是勒贝格测量C的因子的乘积。因而，存在C的紧子集D，使得$\mu(D) > \frac{1}{2}$并且$f$的限制到D是连续的，因此也是有界的。令 M 为 D 上 $|f|$ 的上界，并令 $p \in \mathbf{N}$ 使得 $p \geq 4M$。令$s = (s_n)$和$t = (t_n)$是D的两个点，使得$s_n = t_n$对于所有$n \neq p$。然后

$$
f(s) - f(t) = u(\sum_n s_n x_n - \sum_n t_n x_n) = (s_p - t_p) u(x_p) .
$$

从$|f(s) - f(t)| \leq 2M$和$|u(x_p)| \geq p \leq 4M$开始，我们得到

$$
|s_p - t_p| \leq \frac{1}{2} .
$$

Lebesgue-Fubini 定理（INT，V，第 2 版，§ 8, No. 3，第 7 条第 2 条）意味着 $\mu(D) \leq \frac{1}{2}$；这就产生了矛盾。因此$u$是连续的。

在一般情况下，根据前面的论证，对于每个 $v \in F'$，线性形式 $v \circ u$ 都是连续的。令$(x_n)_{n \in \mathbf{N}}$为E趋于0的点的序列；如果 F 被赋值为拓扑 $\sigma(F, F')$，则 F 中序列 $(u(x_n))_{n \in \mathbf{N}}$ 趋于 0；因此，这个序列以$\sigma(F, F')$为界，因此它以F（III，p. 27，cor.3）为界。由于 E 是出生学的（III，p. 12，命题 2）； 线性映射 $u : E \to F$ 是连续的。 \*

$^1$这个截面的结果取决于积分书。

习题

### 习题 {#evt-iii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
