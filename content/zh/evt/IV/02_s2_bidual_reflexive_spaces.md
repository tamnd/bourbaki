---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 2
section_title: Bidual. Reflexive spaces
lang: zh
source: evt-i-v
book_pages: TVS IV.14-TVS IV.21, TVS IV.52-TVS IV.57
pdf_pages: 0196-0203, 0234-0239
extraction: ocr
subsections:
    - "no": 1
      title: Bidual
      page: 14
      pdf_page: 196
    - "no": 2
      title: Semi-reflexive spaces
      page: 15
      pdf_page: 197
    - "no": 3
      title: Reflexive spaces
      page: 16
      pdf_page: 198
    - "no": 4
      title: The case of normed spaces
      page: 17
      pdf_page: 199
    - "no": 5
      title: Montel spaces
      page: 18
      pdf_page: 200
statements: 32
exercises: 26
content_sha256: 3e54b6f6c3ad0beee01b85bfb077506b0f9c7b5fbf5e3a18e55cf804f47031c0
translated_from: content/en/evt/IV/02_s2_bidual_reflexive_spaces.md
translation_method: google
source_content_sha256: b91386e65623979a9a9994a73c883cd7ba5db67a5bb1adc0fbb46df95c3c8a73
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 7827e1e4f65328b8fcf609e3c1484cff1986b09b12bc708c6792e57b7282e255
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。双向。反射空间

### 1. 双向

#### 定义 1 {#evt-iv-s2-def-1 .statement tag=07S8}

— *令 $E$ 为局部凸空间，$E'_b$ 为其强对偶。局部凸空间 $E'_b$ 的对偶称为 $E$ 的对偶，记为 $E''$。*

对于每个$x \in E$，令$\tilde{x}$在$E'$上为线性形式$x' \mapsto \langle x, x' \rangle$；对于弱拓扑$\sigma(E', E)$来说它是连续的，因此*更不必说*，对于强拓扑在$E'$上；因此 $\tilde{x} \in E''$ 对于所有$x \in E$。 映射$c_E : x \mapsto \tilde{x}$从$E$到$E''$是线性映射，据说是*规范*。

#### 命题 1 {#evt-iv-s2-prop-1 .statement tag=07S9}

— $c_E : E \to E''$ 的 *核是 $E$ 中 0 的闭包。如果 $E$ 是 Hausdorff，则 $c_E$ 是单射。*

到构造，$c_E$的核是$E$上连续的线性形式的核交，*即*$E$中$\{0\}$的闭合（II， p. 24，cor。

当$E$是Hausdorff时，我们通过映射$c_E$将认同$E$与$E''$的子空间进行计算。

双向。反射空间

TVS IV.15

$E''$上的强拓扑是$\mathscr{S}$拓扑，其中$\mathscr{S}$是$E'$的所有强有界子集的族。由于$E'$的每个等连续子集都是强有界的（III，p. 22，道具9），$E$上的初始拓扑比通过在强的$c_E$下取逆像获得的拓扑更粗糙拓扑 $E''$；它可以严格更粗糙（IV，p. 52，练习1）。然而：

#### 命题 2 {#evt-iv-s2-prop-2 .statement tag=07SA}

— 假设空间 $E$ 是天生的或桶装的。 $E$上的初始拓扑是$E''$上强拓扑的$c_E$下的逆像。

因为，强有界的$E'$的每个子集都是等连续的（III，p. 22，道具10和III，p. 24）。

#### 命题 3 {#evt-iv-s2-prop-3 .statement tag=07SB}

— 令 $E$ 为局部凸 Hausdorff 空间。在阶中，$E$的强对偶$E'_b$被桶装，有必要且充分的是$E''$的每个子集（其边界为$\sigma(E'', E')$）包含在$\sigma(E'', E')$的边界子集的闭包中$E$。

$E''$的等连续子集是子集，包含在$E''$的子空间$E$的有界子集的双极（对于$E''$和$E'$之间的对偶性）。现在只需使用双极的定理（II、p. 45、cor.3）和桶装空间（III、p. 24）的定义即可。

#### 注 {#evt-iv-s2-n1-rem-1 .statement tag=07SC}

令 $E$ 为局部凸 Hausdorff 空间，$E'$ 为对偶，$E''$ 为对偶。我们有$E \subset E'' \subset {E'}^*$，其中${E'}^*$是$E'$的代数对偶。如果$B$是$E$的有界子集，则赋予$\sigma({E'}^*, E')$的${E'}^*$中的闭包$\overline{B}$包含在$E''$中：因为$B$在$E'$中的极$U = B^\circ$为$E'_b$中有0的邻域，我们有$\overline{B} \subset U^\circ \subset E''$。

### 2. 半反身空间

#### 定义 2 {#evt-iv-s2-def-2 .statement tag=07SD}

— 设 $E$ 为局部凸空间。如果从$E$到$E''$的典范映射$c_E$是双射的，我们说$E$是半自反的。

这意味着$E$是Hausdorff，并且$E'$上的每个线性形式（对于强拓扑$\beta(E', E)$连续）是形式$x' \mapsto \langle x, x' \rangle$和$x \in E$，即对于弱拓扑$\sigma(E', E)$连续。

#### 定理 1 {#evt-iv-s2-thm-1 .statement tag=07SE}

— 局部凸 Hausdorff 空间是半自反的，当且仅当 $E$ 的每个有界子集对于弱化的拓扑 $\sigma(E, E')$ 来说相对紧凑。如果 $E$ 是半自反的，则 $E$ 的强对偶 $E'_b$ 是桶状的。

第二个断言来自 prop. 3（IV，p. 15），以及初始拓扑的有界子集和$E$的弱化拓扑之间的恒等式（III，p. 27，cor.3）。

说$E$是半自反意味着$E'_b$上的拓扑与$E$和$E'$之间的对偶性兼容，在其他字中，通过Mackey的定理（IV，p. 2，第1）， $E'_b$上的拓扑比$\tau(E', E)$更粗糙（事实上与它相同）；由定义 (IV, p. 2)，这意味着 $E$ 的每个闭、凸、有界子集对于 $\sigma(E, E')$ 都是紧致的，这相当于说，E 的每个有界子集对于 $\sigma(E, E')$ 都是相对紧致的，因为闭凸E 的有界子集的包络线是有界的（III，p. 3，道具 1）。

#### 推论{#evt-iv-s2-n2-cor-1 .statement tag=07SF}

— *令 E 为局部凸半自反空间。 E 的每个闭向量子空间 M 都是半自反的；此外，$E'/M^\circ$（视为M的对偶）上的强拓扑是E'上的强拓扑的商。

设B是M的有界子集。由于B在E中有界，并且M上的弱化拓扑$\sigma(M, M')$是由$\sigma(E, E')$（IV，p. 10，命题11）诱导的，因此赋予$\sigma(M, M')$的M中B的闭包是紧的。因而，通过th。 1、M是半自反的。推论最后一个断言由命题得出。 IV、p. 9的10，应用于E的所有闭、凸、有界子集的集合$\mathscr{S}$。

#### 注 1 {#evt-iv-s2-n2-rem-1 .statement tag=07SG}

假设 E 是半自反的。 E 的每个子集对于初始拓扑是凸的、封闭的且有界的，对于拓扑 $\sigma(E, E')$ 是紧凑的（IV，p. 1，道具 1）。 *另一方面，无限维希尔伯特空间 E 的单位球体（使用方程 $\|x\| = 1$）对于初始拓扑是封闭且有界的，但对于弱化的拓扑不是封闭的，即使 E 是半自反的。 \*

#### 注 2 {#evt-iv-s2-n2-rem-2 .statement tag=07SH}

通过IV、p. 5的注 3，我们可以重新表述th。 1 如下： *Hausdorff 空间 E 是半自反的当且仅当它对于其弱化的拓扑是准完备的。*如果它是半自反的，那么它对于它的初始拓扑* (IV, p. 5, 注 2) 是*准完备的。

#### 注 3 {#evt-iv-s2-n2-rem-3 .statement tag=07SI}

在上述推论的假设下，空间 E/M 不一定是半自反的（IV，p. 63，练习 10）。

### 3. 自反空间

#### 定义 3 {#evt-iv-s2-def-3 .statement tag=07SJ}

— *如果从 E 到 $E''$ 的典范映射 $c_E$ 是从 E 到 $E'_b$ 的强对偶的拓扑向量空间同构，则称局部凸空间 E 是自反的。*

特别是，自反空间是半自反的，因此豪斯多夫。

#### 命题 4 {#evt-iv-s2-prop-4 .statement tag=07SK}

— *自反空间的强对偶是自反的。*

这立即来自 def。 3.

#### 定理 2 {#evt-iv-s2-thm-2 .statement tag=07SL}

— *在阶中，局部凸 Hausdorff 空间 E 是自反的，它是桶形的，并且 E 的每个有界子集对于弱化的拓扑 $\sigma(E, E')$ 来说是相对紧凑的。*

到了。 1 (IV, p. 15)，这与说相同，E *是自反的当且仅当它是半自反的并且是桶形的*。

如果 E 是自反的，则 $E'_b$ 也是自反的（命题 4），因而 E 是桶状的（IV、p. 15、第 1）。相反，如果 E 是半自反且桶状的，则 $c_E$ 是双射，并且通过 IV、p. 15 是双连续的。 2，因此E是自反的。

#### 注 1 {#evt-iv-s2-n3-rem-1 .statement tag=07SM}

令 E 为无限维实希尔伯特空间。令 F 表示空间 E，赋予弱化的拓扑。 空间 E 和 F 具有相同的对偶 E'，且 E 是自反 Banach 空间 (V, p. 17)。因而，F 是*半自反*。

然而，E 上的强拓扑和弱拓扑是不同的，因而 F *不是自反的*。

#### 注 2 {#evt-iv-s2-n3-rem-2 .statement tag=07SN}

设E是自反空间，M是E的闭向量子空间。可能会发生M和E/M都不是自反空间（IV，p. 63，练习10）。 \* 对于标准化空间的情况，请参阅 prop. 7 个IV、p. 17。 \*

### 4. 范数空间的情况

令 E 为赋范空间。 E 的对偶 E' 上的强拓扑由范数定义

(1)
$$
\|x'\| = \sup_{x \in E, \|x\| \leq 1} |\langle x, x' \rangle|,
$$
E 的强对偶是 Banach 空间 (III, p. 24, cor. 2)。那么 E 的双元 E'' 也是 Banach 空间，对于范数定义为

(2)
$$
\|x''\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x', x'' \rangle|.
$$

通过道具。 8、(i) IV、p. 7，规范的线性映射 $c_E : E \to E''$ 是等轴测图。从今以后，*我们将认同 E 及其双 E''* 的标准化子空间。

#### 命题 5 {#evt-iv-s2-prop-5 .statement tag=07SO}

— *令 E 为范数空间，E' 为对偶，E'' 为对偶。 E'' 中的（闭合）单位球是 E 中单位球 B 的闭合，对于弱拓扑 $\sigma(E'', E')$。*

根据公式 (1) 和 (2)，E'' 中的单位球是 B 的双极 $B^{\circ \circ}$。 命题 5 然后从双极的定理得出（II，p. 45，cor. 3）。

#### 注 {#evt-iv-s2-n4-rem-1 .statement tag=07SP}

— 对于强拓扑，Banach 空间 E 在其双 E'' 中闭合，但对于弱拓扑来说是稠密的（命题 5）。

在阶中，规范化的空间是*自反的*，它是*半自反的*是充分必要的；因为，E 的初始拓扑总是由 E'' 的强拓扑诱发。 Th。 1 (IV, p. 15) 则意味着以下结果：

#### 命题 6 {#evt-iv-s2-prop-6 .statement tag=07SQ}

— *在阶中，范式空间 E 是自反的，对于弱化的拓扑 $\sigma(E, E')$，E 中的单位球是紧凑的是必要且充分的。*

我们观察到自反范数空间是完整的，因此是 Banach 空间，并且它的对偶是自反 Banach 空间的属性。 4 个IV、p. 16。

#### 命题 7 {#evt-iv-s2-prop-7 .statement tag=07SR}

— *设 E 是自反 Banach 空间，M 是 E 的闭向量子空间。则 M 和 E/M 是自反 Banach 空间。*

令 E' 为 E 的对偶和 $M^\circ$ M 在 E' 中的正交。作为规范化的空间，我们将可以确定空间$E'/M^\circ$与M的对偶$M'$（IV，p. 9，道具10）。由于 M 是半自反的（IV，p. 16，推论），因此它是自反的，因而 $E'/M^\circ$ 也是如此；类似地，$M^\circ$是自反的，它的对偶$E/M^{\circ \circ} = E/M$也是如此。

#### 例 {#evt-iv-s2-n4-exa-1 .statement tag=07SS}

— 1) 让 $\ell^\infty(\mathbf{N})$ 表示标量有界序列 $x = (x_n)_{n \in \mathbf{N}}$ 的 Banach 空间，其中范数

(3) $$
\| \mathbf{x} \| = \sup_{n \in \mathbf{N}} |x_n| \quad (\text{I, p. 4}) .
$$

令$c_0(\mathbf{N})$为序列趋于0的$\ell^\infty(\mathbf{N})$由……组成的闭向量子空间。最后，令$\ell^1(\mathbf{N})$为可和序列的向量空间，赋予范数

(4) $$
\| \mathbf{x} \|_1 = \sum_{n \in \mathbf{N}} |x_n| .
$$

我们可以证明 (IV, p. 47, exerc.1) $c_0(\mathbf{N})$ 的对偶可以与 $\ell^1(\mathbf{N})$ 等同，我们有

(5) $$
\langle \mathbf{x}, \mathbf{x}' \rangle = \sum_{n \in \mathbf{N}} x_n x'_n
$$

对于所有 $\mathbf{x} \in c_0(\mathbf{N})$ 和 $\mathbf{x}' \in \ell^1(\mathbf{N})$。类似地，$\ell^1(\mathbf{N})$的对偶可以用$\ell^\infty(\mathbf{N})$来识别，这样我们对于所有$\mathbf{x} \in \ell^1(\mathbf{N})$和所有$\mathbf{x}' \in \ell^\infty(\mathbf{N})$都有关系（5）。因而 $\ell^\infty(\mathbf{N})$ 是 $c_0(\mathbf{N})$ 的双数，后者空间不是自反的。

\* 2) 每个希尔伯特空间都是自反Banach空间（V，p. 17）。
\* 3) 令X为豪斯多夫拓扑空间，$\mu$为X的复测度。对于每个实数 $p > 1$，Banach 空间 $L^p(X, \mu)$ 是自反的，其对偶可以用 $L^q(X, \mu)$ 和 $p^{-1} + q^{-1} = 1$ 来识别（INT、V、第 2 版、§ 5, No. 8 和 IX, § 1, No. 10）。

### 5. 蒙特尔空间

#### 定义 4 {#evt-iv-s2-def-4 .statement tag=07ST}

*局部凸 Hausdorff 和桶状空间，其中每个有界子集相对紧凑，称为 Montel 空间。*

#### 例 1 {#evt-iv-s2-n5-exa-1 .statement tag=07SU}

每个有限维 Hausdorff 空间都是 Montel 空间。规范化的空间是 Montel 空间 ，它是局部紧致的，因此是有限维的（I，p. 15，第 3 个）。

#### 例 2 {#evt-iv-s2-n5-exa-2 .statement tag=07SV}

具有记号和假设的支柱。 III、p. 6、空间 E 中的 7 个，是 Banach 空间的感应极限，被装桶（III、p. 25）；此外，E 的每个有界子集都是相对紧凑的（III，p. 6，道具 7）。在其他字中，E是Montel空间。特别是，Gevrey 空间（III，p. 10）是Montel 空间。 \* 这对于函数细菌的空间 $\mathscr{H}(K)$ 由……组成在$\mathbf{C}^n$（III，p. 10）的紧凑子集 K 的邻域中解析是正确的。*

#### 例 3 {#evt-iv-s2-n5-exa-3 .statement tag=07SW}

Montel 空间 (II, p. 33) 的序列 $(E_n)$ 的每个严格归纳极限 E，使得对于所有 n，$E_n$ 在 $E_{n+1}$ 中闭合，是 Montel 空间；事实上，E 是 Hausdorff（II，p. 32，第 9 (i) 条），桶状（III，p. 25，cor.3），并且 E 的每个有界子集都包含在$E_n$（III，p. 5，命题 6) 因此在 $E_n$ 中相对紧凑，因此在 E 中也是如此。

#### 例 4 {#evt-iv-s2-n5-exa-4 .statement tag=07SX}

\* 令U为$\mathbf{R}^n$中的开集合，并令$\mathscr{C}^\infty(U)$为U上无限可微函数的Fréchet空间（III，p. 9）。我们将证明这是一个 Montel 空间。由于 $\mathscr{C}^\infty(U)$ 是 Fréchet 空间，因此它是桶装的（III、p. 25，推论）。设 B 为 $\mathscr{C}^\infty(U)$ 的有界子集，并令 K 为 U 的紧凑子集。对于每个 $\alpha \in \mathbf{N}^n$，令 $H_{\alpha, K}$ 为限制的集合到函数 $\partial^\alpha f$ 的 K，因为 $f$ 穿过 B。 $\alpha \in \mathbf{N}^n$；对于每个$\beta \in \mathbf{N}^n$，使得$|\beta| = |\alpha| + 1$、集合、$H_{\alpha, K}$有界于$\mathscr{C}(K)$，因为B有界于$\mathscr{C}^\infty(U)$；由 VAR, R., No. 2.2.3, 集合 $H_{\alpha, K}$ 是等连续的，因而 (GT, X, § 2, No. 5) 在 $\mathscr{C}(K)$ 中相对紧凑。但$\mathscr{C}^\infty(U)$的拓扑是拓扑中最粗糙的，从$\mathscr{C}^\infty(U)$到$\mathscr{C}(K)$的所有映射$f \mapsto \partial^\alpha f|K$都是连续的，因此B在$\mathscr{C}^\infty(U)$中相对紧凑（GT，I, § 4, No. 1，第3条和§ 9, No. 5，推论）。

类似地，在 U* (III, p. 9) 中具有紧凑支持的所有无限可微函数中的 *空间 $\mathscr{C}_0^\infty(U)$ 是 Montel 空间*。因为，$\mathscr{C}_0^\infty(U)$是Fréchet空间(III，p. 9)的序列$\mathscr{C}_{H_n}^\infty(U)$的严格归纳极限，足以看出空间$\mathscr{C}_{H_n}^\infty(U)$都是Montel 空间（*例3*）。但是 $\mathscr{C}_0^\infty(U)$ 有界且封闭的子集在 $\mathscr{C}^\infty(U)$ 中是封闭且有界的，因此在 $\mathscr{C}^\infty(U)$ 中是紧致的，因此在 $\mathscr{C}_{H_n}^\infty(U)$ 中也是紧致的。 \*

#### 命题 8 {#evt-iv-s2-prop-8 .statement tag=07SY}

*设 E 为 Montel 空间和 $\mathfrak{T}$ E 上的滤波器，对于弱化的拓扑，其收敛到 E 中的点 $x_0$。如果 $\mathfrak{T}$ 是可数基，或包含是有界集合，则 $\mathfrak{T}$ 也会收敛到 $x_0$，以获得初始拓扑。*

首先假设$\mathfrak{T}$中存在有界集合$\overline{B}$。对于 E 的初始拓扑，B 的闭包 $\overline{B}$ 是有界的；在加法中，$\overline{B}$ 是紧的，因为 E 是 Montel 空间。由 $\sigma(E, E')$ 引发的 $\overline{B}$ 上的拓扑是 Hausdorff，并且比由初始拓扑引发的拓扑更粗糙；因而，他们重合（GT，I, § 9, No. 4）。对于这种情况，这证明了命题。

接下来假设$\mathfrak{T}$有一个可数的基。考虑序列$(x_n)_{n \geq 1}$对于$\sigma(E, E')$趋向于$x_0$的情况就足够了（GT，I, § 6, No. 8，道具11）。令 B 为 $n \geq 0$ 的所有 $x_n$ 中的集合。这个集合以$\sigma(E, E')$为界，因此也适用于初始的拓扑（III，p. 27，cor.3）。这样我们就减少到了第一个情况证明。

*每个 Montel 空间都是自反的*：这来自 def。 4 并从 th 开始。 2 个IV、p. 16。进一步：

#### 命题 9 {#evt-iv-s2-prop-9 .statement tag=07SZ}

*Montel 空间的强对偶是 Montel 空间。*

令 E 为 Montel 空间和 $E'_b$ 其强对偶。由于 E 是自反的，$E'_b$ 是桶状的（IV、p. 15、第 1）。由于 E 的每个有界子集都是相对紧致的，因而 $E'$ 重合上的强拓扑与拓扑具有紧致收敛性。设 B 为 $E'_b$ 有界子集；它对于弱拓扑 $\sigma(E', E)$ 有界，因此是等连续的，因为 E 是桶形的。那么Ascoli 的定理（GT，X, § 2, No. 4，cor. 和§ 2, No. 5，cor.1）意味着$\sigma(E', E)$ 的B 闭包对于紧致收敛的拓扑是紧致的；因而 B 在 $E'_b$ 中是相对紧的。

#### 命题 10 {#evt-iv-s2-prop-10 .statement tag=07T0}

*每个可度量的 Montel 空间满足可数性第一公理。*

令 E 为可度量的 Montel 空间。我们知道（II，p. 5）E可以与规范化的空间的乘积序列的$F = \prod_{n \in \mathbf{N}} F_n$和子空间等同，甚至可以假设对于所有$n \in \mathbf{N}$，我们都有$\mathrm{pr}_n(E) = F_n$。如果每个可度量的空间 $F_n$ 满足可数性第一公理，那么 F (GT, IX, § 2, No. 8) 也满足，因而 E 也满足。

我们通过“归谬法”来论证。假设例 $F_0$ 不满足可数性第一公理。令$B_0$为$F_0$中的单位球（闭合）；这是一个度量空间，它不是满足可数性的第一个公理。我们将使用以下引理 ：

#### 引理 1 {#evt-iv-s2-lem-1 .statement tag=07T1}

*假设度量空间 X 不是满足可数性第一公理。那么X中存在实数$\varepsilon > 0$和不可数子集A，使得$d(x, y) \geq \varepsilon$对于A中所有不同的$x, y$。*

对于每个整数$n \geq 1$，令$\mathfrak{F}_n$为X的子集D的集合（按包含排序），使得$d(x, y) \geq \frac{1}{n}$对于D中不同的$x, y$。集合$\mathfrak{F}_n$是有限的特征标，因此拥有极大元素$D_n$（S，III, § 4, No. 5）。那么对于所有$y \in X$，在$D_n$中存在点$x$，使得$d(x, y) < \frac{1}{n}$，凭借$D_n$的最大特征标。

把$D = \bigcup_n D_n$；那么集合 D 在 X 中是稠密的，并且由于 X 不是可数第一公理满足，因此 D 不可数，因此 $D_n$ 中的一个不可数。

Q.E.D.

将引理 1 应用于 $B_0$，存在不可数的 $F_0$ 和数 $\varepsilon > 0$ 子集 $A_0$，使得 $\|x\| \leq 1$ 和 $\|x - y\| \geq \varepsilon$ 对于不同的$x, y$ $A_0$。我们有$\mathrm{pr}_0(E) = F_0$，因此E中存在子集A，使得$\mathrm{pr}_0$诱导双射从A到$A_0$。

#### 引理 2 {#evt-iv-s2-lem-2 .statement tag=07T2}

*A 存在不同的元素序列 $(x_m)_{m \geq 0}$ 由……组成，其有界于 E。*

我们将A的点的构造序列$(x_m)_{m \geq 0}$乘以归纳；以及满足的递减序列 $(C_m)_{m \geq 0}$ 子集以下条件 ：
a) 集合 $C_m$ 都不是可数的。
b) 对于每个 $n \geq 0$，集合 $\mathrm{pr}_k(C_m)$ 都以 $F_k$ 为界，对于 $0 \leq k \leq m$。
c) 对于每个$m \geq 0$，我们有$x_m \in C_m - C_{m+1}$。

我们投入$C_0 = A$。假设$0 \leq m \leq n$定义了集合$C_m$，则$0 \leq m \leq n$定义了满足a)和b)，$0 \leq m < n$定义了$C_m - C_{m+1}$中的点$x_m$。对于每个整数 $r \geq 1$，令 $C_{n,r}$ 为所有 $x \in C_n$ 中的集合，使得

$$
r - 1 \leq \| \mathrm{pr}_{n+1}(x) \| < r .
$$

由于$C_n$不可数，因此存在整数$r \geq 1$使得$C_{n,r}$不可数。我们将选择点$x_n$放入$C_{n,r}$并放入$C_{n+1} = C_{n,r} - \{ x_n \}$。显然，$C_{n+1} \subset C_n$和$x_n \in C_n - C_{n+1}$，集合$C_{n+1}$不可数，$\mathrm{pr}_k(C_{n+1})$对于$0 \leq k \leq n + 1$来说在$F_n$内。

我们有 $x_m \in C_m$，所以 $x_m \in C_n$ 其中 $m \geq n$。因此，$F_n$上序列$(x_m)_{m \geq 0}$的投影对于所有$n \geq 0$都是有界的；在其他字中，序列 $(x_m)_{m \geq 0}$ 有界于 E，从而建立引理 2。

Q.E.D.

当记号为引理 2 时，有界序列 $(x_m)_{m \geq 0}$ 在 E 中具有极限点 $y$。因此序列 $(\mathrm{pr}_0(x_m))_{m \geq 0}$ 在 E 中具有极限点 $\mathrm{pr}_0(y)$ $F_0$，但是$A_0$的这个与……矛盾构造。

#### 推论{#evt-iv-s2-n5-cor-1 .statement tag=07T3}

— 令 E 为可​​度量的 Montel 空间。那么E的强对偶中存在可数稠密集合。

在E的对偶E'上，强拓扑与紧收敛相同，因为E是Montel空间。现在应用 cor 就足够了。 1 道具。 6 个III、p. 18。

我们可以证明，如果 E 是无限维的（IV，p. 57，练习 1），可度量的 Montel 空间 E 的强对偶是不可度量的。

### 习题{#evt-iv-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
