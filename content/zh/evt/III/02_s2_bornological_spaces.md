---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 2
section_title: Bornological spaces
lang: zh
source: evt-i-v
book_pages: TVS III.11-TVS III.13, TVS III.40-TVS III.41
pdf_pages: 0143-0145, 0172-0173
extraction: ocr
statements: 6
exercises: 4
content_sha256: deed514616cbd5ae5f929a3ca928b011f118da7604adeaf5e9f66e34074f6866
translated_from: content/en/evt/III/02_s2_bornological_spaces.md
translation_method: google
source_content_sha256: 40a687273614f4755635004c7de82956200bd4dc25c1f116ef776c135c6ae0d1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: c29cf43af0620abfa42040e6a77043ee7f2cd67cf8795794699849c297612ac9
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。生育学空间

在本段中，E 表​​示局部凸空间，$\mathscr{B}$ 表示其规范出生学（III，p. 3，def. 5）。

#### 引理 1 {#evt-iii-s2-lem-1 .statement tag=07M8}

— *设 G 为半范数空间，p 为半范数，u 线性映射从 G 变为 E。以下条件是等价的* ：

(i) *u 是连续的* ；
(ii) u下G的单位球的*像有界于E*；
(iii) *对于G的点的每个序列$(x_n)$趋于0，序列$(u(x_n))$在E*中有界。

直接的 (i) 暗示 (ii) (III, p. 4, cor. 1) 并且 (ii) 暗示 (iii)。设 E 中 V 为 0 的邻域；如果G中$u^{-1}(V)$不是0的邻域，则存在$G - u^{-1}(V)$的点的序列$(y_n)$使得$p(y_n) \leq \frac{1}{n^2}$。因此，序列$x_n = n y_n$在G和$u(x_n) \notin nV$中趋于0，这意味着序列$(u(x_n))$无界。因此(iii)意味着(i)。

#### 命题 1 {#evt-iii-s2-prop-1 .statement tag=07M9}

*以下条件是等效的*：
(i) *E 上的每个半范数以 E 的有界子集为界是连续的*。
(i') *E 的每个凸平衡子集吸收 E* 的有界子集 (I, p. 7, def. 4) *是 E* 中 0 的邻域。
(ii) *E 是半范数空间 $E_A$ 的归纳极限，其中 A 的范围超过 E* 的闭、凸、平衡且有界子集的有向递增集合。
(ii') *存在半范数空间的族$(E_i)_{i \in I}$，对于每个$i \in I$，线性映射$u_i : E_i \to E$，使得E的拓扑是最精细的局部凸拓扑，其中$u_i$是连续的*。
(iii) *对于任意局部凸空间 F，线性映射 $u : E \to F$ 是连续的当且仅当对于 E 中点的每个序列 $(x_n)$ 趋于 0，序列 $(u(x_n))$ 在 F* 中有界。

(iii') *对于任意半范数空间 F, 线性映射 u : E → F 是连续的当且仅当对于 E 中的每个有界集合 X，u(X) 在 F 中有界。*

就对应而言，(i) 和 (i') 在半范数和凸、平衡、吸收子集 (II, p. 20) 之间是等价的，直接的。如果 p 是 E 上的半范数，且在每个 E_A 上连续，则 p 有界于 E 的有界子集；因此 (i) 意味着 (ii) (II, p. 27, 命题 5)。显然，(ii) 意味着(ii')。

现在让 (E_i, u_i)_{i \in I} 与 (ii') 中一样，并让 u 为从 E 到局部凸空间 F 的线性映射，使得 (u(x_n)) 在 F 中对于 E 的点趋向于 0 的每个序列 (x_n) 有界。 引理 1 of III, p. 11 线性映射 u \circ u_i : E_i \to F 对于I 中的所有 i \ 是连续的。因此，如果 E 的拓扑是 u_i 连续的最精细局部凸拓扑，则 u 是连续的（II，p. 27，道具 5）。这证明(ii')蕴涵(iii)。

It is immediate that (iii) implies (iii') (III, p. 3, cor.) Finally, if p is a semi-norm on E, which is bounded on bounded subsets of E, the condition (iii') asserts that the identity map is continuous from E into the semi-normed space (E, p); in other words, p is continuous. 这证明(iii')蕴涵(i)。

#### 定义 1 {#evt-iii-s2-def-1 .statement tag=07MA}

*如果满足等价的 prop 条件，则局部凸空间被认为是天生的。 1.*

#### 例 {#evt-iii-s2-n0-exa-1 .statement tag=07MB}

— 1) 每个半范数空间都是天生的。
2) 特别地，每个有限维局部凸空间都是天生的。
3）考虑到最终局部凸拓扑的传递性（II，p. 28，cor.2），我们立即从条件（ii'）推断出，如果（E_i）_{i \in I}是局部凸出生学空间族，并且如果E被分配为最好的局部凸拓扑对于其中线性映射 u_i : E_i \to E (对于 i \in I) 是连续的，则 E 是出生学的。特别是，*归纳极限、直和、出生学空间的商空间是出生学空间*。

另一方面，天生的空间的闭合子空间不一定是天生的（IV，p. 63，练习 8）。

#### 推论{#evt-iii-s2-n0-cor-1 .statement tag=07MC}

*每个 Hausdorff 和半完全出生学空间都是 Banach 空间的归纳极限。*

事实上，空间 E_A，其中 A 是闭集且有界的，即 Banach 空间（III，p. 8，推论）。

#### 命题 2 {#evt-iii-s2-prop-2 .statement tag=07MD}

*局部凸可度量空间是天生的。*

假设 E 是可度量的，并且 p 是 E 上的半范数，其边界在 E 的有界子集上，但不连续。令 A 为所有 $x \in E$ 中的集合，使得 $p(x) < 1$。令$(V_n)_{n \geq 1}$为递减序列，在E中形成0的邻域的基本系统。由于p不连续，因此A不是0的邻域；因此，对于每个$n > 0$，我们有$A \not\supseteq n^{-1} V_n$，并且在$V_n$中存在点$x_n$，这样$n^{-1} x_n \notin A$，即$p(x_n) \geq n$。 序列 $(x_n)$ 趋于 0，因此有界（III，p. 3，推论）；这个与……矛盾假设位于第 12 页。

#### 推论{#evt-iii-s2-n0-cor-2 .statement tag=07ME}

— *每个 Fréchet 空间* (II, p. 24) *是 Banach 空间* 的归纳极限。

### 习题{#evt-iii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
