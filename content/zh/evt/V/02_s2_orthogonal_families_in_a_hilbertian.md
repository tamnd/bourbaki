---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 2
section_title: Orthogonal families in a hilbertian space
lang: zh
source: evt-i-v
book_pages: TVS V.17-TVS V.25, TVS V.70-TVS V.73
pdf_pages: 0275-0283, 0328-0331
extraction: ocr
subsections:
    - "no": 1
      title: External hilbertian sum of hilbertian spaces
      page: 17
      pdf_page: 275
    - "no": 2
      title: Hilbertian sum of orthogonal subspaces of a hilbertian space
      page: 18
      pdf_page: 276
    - "no": 3
      title: Orthonormal families
      page: 21
      pdf_page: 279
    - "no": 4
      title: Orthonormalisation
      page: 23
      pdf_page: 281
statements: 23
exercises: 16
content_sha256: 72a24e03e4fdfb9db63739480d81f812c8b449118cf2147d14169c87d4df300f
translated_from: content/en/evt/V/02_s2_orthogonal_families_in_a_hilbertian.md
translation_method: google
source_content_sha256: a7de25f8e6403d336b77dd0506a5e00a8938e7643c273332f7c1b37ad5210590
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 86eef560d8ada79cb14461ff21ca37c2cd99af1b29edb6d85d47cb272e65aed5
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。希尔伯特空间中的正交族

### 1. 希尔伯特空间的外部希尔伯特和

#### 命题 1 {#evt-v-s2-prop-1 .statement tag=07Z7}

*令 $(E_i)_{i \in I}$ 为所有族 $x = (x_i)_{i \in I}$ 的希尔伯特空间、P 乘积向量空间 $\prod_{i \in I} E_i$ 和 P 由……组成的 E 子集，使得 $\sum_{i \in I} \|x_i\|^2$ 是有限的。

a) E 是 P 的向量子空间。

b) 对于 E 中的每个 $x = (x_i)_{i \in I}$ 和 $y = (y_i)_{i \in I}$，族 $(\langle x_i|y_i \rangle)_{i \in I}$ 是可求和的。如果我们放置$\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$，我们定义在E上正分隔厄米特形式。

c) 对于如此定义的标量乘积，E 是希尔伯特空间； $E_i$ 的直和 S 在 E 中是稠密的。

对于 E 中的 $x = (x_i)_{i \in I}$ 和 $y = (y_i)_{i \in I}$，我们有
$$
\|x_i + y_i\|^2 \leq 2(\|x_i\|^2 + \|y_i\|^2),
$$
因此 $x + y = (x_i + y_i)_{i \in I}$ 属于为 E。这证明了 a)。

根据柯西-施瓦茨不等式，我们有
$$
|\langle x_i|y_i \rangle| \leq \|x_i\| \cdot \|y_i\| \leq \frac{1}{2}(\|x_i\|^2 + \|y_i\|^2)
$$
因此$\sum_{i \in I} |\langle x_i|y_i \rangle| < +\infty$。如果$x \neq 0$，我们就有$\langle x|x \rangle = \sum_{i \in I} \|x_i\|^2 > 0$，因此断言 b)如下。

我们记得，S 是所有族 $x = (x_i)_{i \in I}$ 的 P 由……组成的子空间，使得所有 $i \in I$ 的集合其中 $x_i \neq 0$ 是有限的。紧接着，S 在 E 中是稠密的；因此，仍然需要证明 E 对于由范数 $\|x\| = \langle x|x \rangle^{1/2}$ 获得的拓扑 $\mathscr{T}_1$ 来说是*完整的。设 $\mathscr{T}_2$ 是由 $\prod_{i \in I} E_i$ 上的乘积拓扑在 E 上诱发的拓扑。对于每个$r > 0$，令$B_r$为所有$x \in E$中的集合，使得$\|x\| \leq r$。这个关系意味着对于I的每个有限子集J，我们都有$\sum_{i \in J} \|x_i\|^2 \leq r^2$，因此$B_r$是$\prod_{i \in I} E_i$的闭子集，因此也是完备的。事实上，E 对于 $\mathscr{T}_1$ 是完整的，现在可以从 GT、III, § 3, No. 5 得出，cor。 2 支撑。 10.

#### 定义 1 {#evt-v-s2-def-1 .statement tag=07Z8}

*让*$(E_i)_{i \in I}$*成为希尔伯特空间的家族。希尔伯特空间 E 在道具中定义。 1 被称为族* $(E_i)_{i \in I}$ *的外部希尔伯特和，写为* $\bigoplus_{i \in I} E_i$ *或* $\bigoplus_{i \in I} E_i$^1。

令$f_i$为从$E_i$到E的映射，其中变换$z \in E_i$到元素$(x_k) \in E$，使得$x_k = 0$对于所有$k \neq i$和$x_i = z$；很明显，$f_i$是从希尔伯特空间$E_i$到E的闭向量子空间的同构。我们说$f_i$是从$E_i$到E的*典范映射*，我们通常会认同 $E_i$ 及其像在 E 中由同构组成。按照这个约定，$E_i$和$E_k$在$i \neq k$的E中*正交*，并且E是由子空间$E_i$的并生成的闭合向量子空间。

当I有限时，E为$E_i$的直和；由于从 E 到 $E_i$ 的规范投影算子对于所有 $i \in I$ 都是连续的，因此 E 也是 $E_i$ 的拓扑直和（GT，III, § 6, No. 2，道具 2）。如果$I = \{1, n\}$，我们也写$E_1 \oplus E_2 \oplus ... \oplus E_n$而不是$\bigoplus_{i=1}^n E_i$。

#### 例 {#evt-v-s2-n1-exa-1 .statement tag=07Z9}

— 令 E 为空间和 I 集合 of 指标的希尔伯特空间。令$\ell^2_E(I)$表示族$(E_i)_{i \in I}$的外部希尔伯特和，其中$E_i = E$代表所有$i \in I$。在其他字中，$\ell^2_E(I)$是E的元素的所有族$x = (x_i)_{i \in I}$的空间，使得$\sum_{i \in I} \|x_i\|^2 < +\infty$，赋予标量乘积$\langle x|y \rangle = \sum_{i \in I} \langle x_i|y_i \rangle$（平方的可求和族空间） E 的元素由 I 索引）。我们放$\ell^2(I) = \ell^2_K(I)$。

### 2. 希尔伯特空间的正交子空间的希尔伯特和

#### 定义 2 {#evt-v-s2-def-2 .statement tag=07ZA}

*希尔伯特空间 E 被认为是一个族* $(E_i)_{i \in I}$ *的希尔伯特和 *E 的封闭向量子空间，当* :

1) *对于两个不同的指标* $i, k$ *在 I、子空间* $E_i$ *和* $E_k$ *在* E 中正交；
2) *由* $E_i$ 的并生成的闭合向量子空间 *是* E。

1 必须注意不要将记号与空间 $E_i$ (A, II, § 1, No. 6) 的“代数”直和相混淆。

#### 定理 1 {#evt-v-s2-thm-1 .statement tag=07ZB}

— 令 E 为希尔伯特空间，它是 E 的封闭向量子空间的族 $(E_i)_{i \in I}$ 的希尔伯特和。从 E 到外部希尔伯特和，存在同构 $f$，并且只有一个。 $(E_i)$族的$\bigoplus_{i \in I} E_i = F$，使得对于所有$i \in I$，$f$到E的限制是从$E_i$到F的典范映射$f_i$。

令$S \subset F$为$E_i$的“代数”直和，令$g$为从S到E的线性映射$(x_i)_{i \in I} \mapsto \sum_{i \in I} x_i$。我们将证明$g$是来自前希尔伯特空间的同构 S 到 E 的（前希尔伯特）子空间 $g(S)$，由 $E_i$ 的并生成：对于两个元素 $x = (x_i)_{i \in I}$、$y = (y_i)_{i \in I}$，我们有

$$
\langle g(x)|g(y) \rangle = \langle \sum_{i \in I} x_i|\sum_{i \in I} y_i \rangle = \sum_{(i,k) \in I \times I} \langle x_i|y_k \rangle .
$$

但如果 $i \neq k$, $\langle x_i|y_k \rangle = 0$乘以假设，因此

$$
\langle g(x)|g(y) \rangle = \sum_{i \in I} \langle x_i|y_i \rangle = \langle x|y \rangle ;
$$

这证明了我们的断言。由于 S 在 F 中稠密，而 $g(S)$ 在 E 中稠密，因此从 F 到 E 有同构 $g$ 扩展到同构 $\overline{g}$（V，p. 8，更确切地说）。显然，$\overline{g}$中的逆同构$f$就是所需要的映射；它的唯一性是由$E_i$的并生成的E的闭子空间是E本身而得出的。

当E是子空间族$(E_i)_{i \in I}$的希尔伯特和时，我们经常通过同构$f$将认同E与$E_i$的外部希尔伯特和F相结合。如果集合I是有限的，说E是族$(E_i)_{i \in I}$的希尔伯特和意味着$E_i$是二乘二正交并且向量空间E是族的直和 $(E_i)_{i \in I}$ 共子空间。

#### 推论 1 {#evt-v-s2-thm-1-cor-1 .statement tag=07ZC}

— 令 E 为希尔伯空间，它是 E 的闭向量子空间族$(E_i)_{i \in I}$ 的希尔伯和；对于所有$i \in I$，令$p_{E_i}$为从E到$E_i$的正射投影（V，p. 13）。

a) 对于所有$x \in E$，族$(\|p_{E_i}(x)\|^2)_{i \in I}$可在$\mathbf{R}$中求和，族$(p_{E_i}(x))_{i \in I}$可在E中求和，并且我们有

$$
\|x\|^2 = \sum_{i \in I} \|p_{E_i}(x)\|^2 , \quad x = \sum_{i \in I} p_{E_i}(x) .
$$

b) 相反，如果$(x_i)_{i \in I}$是E的元素族，使得$x_i \in E_i$对于所有$i \in I$和$\sum_{i \in I} \|x_i\|^2 < + \infty$，则该族是可求和的，并且和$x$是E中唯一的点，对于所有$p_{E_i}(x) = x_i$ $i \in I$。

c) 对于 E 的点 $x, y$ 中的每个对，我们有

$$
\langle x|y \rangle = \sum_{i \in I} \langle p_{E_i}(x)|p_{E_i}(y) \rangle .
$$

这些性质实际上对于$E_i$的外希尔伯特和来说是显而易见的，并且可以通过同构转移到E。

#### 推论 2 {#evt-v-s2-thm-1-cor-2 .statement tag=07ZD}

— 令 E 为 Hausdorff prehilbertian 空间, $(E_i)_{i \in I}$ E 的完整向量子空间族，使得对于 I, 子空间中不同指标 $i, k$ 的每个对 $E_i$ 和 $E_k$ 正交。令V为由$E_i$的并生成的E的闭向量子空间。对于每个 $i \in I$，令 $p_{E_i}$ 为从 E 到 $E_i$ 的正射投影。让$x \in E$。

1) 我们有$\sum_{i \in I} \|p_{E_i}(x)\|^2 \leq \|x\|^2$。

2) 以下条件是等效的： a) $x \in V$； b）$\sum_{i \in I} \|p_{E_i}(x)\|^2 = \|x\|^2$； c) 族$(p_{E_i}(x))_{i \in I}$在E中可求和，我们有$x = \sum_{i \in I} p_{E_i}(x)$。

3) 假设V是完整的。那么族 $(p_{E_i}(x))_{i \in I}$ 在 E 中可求和，并且
$$
p_V(x) = \sum_{i \in I} p_{E_i}(x), \quad \|p_V(x)\|^2 = \sum_{i \in I} \|p_{E_i}(x)\|^2,
$$
其中 $p_V$ 表示从 E 到 V 的正射投影。

令 $\hat{E}$ 为 E 的希尔伯特空间补全；我们认同 E，稠密子空间为 $\hat{E}$； $E_i$ 完成后，关闭 $\hat{E}$ 的子空间。 $\hat{E}$中V的闭包$\overline{V}$是由$E_i$的并和$V = \overline{V} \cap E$生成的$\hat{E}$的闭包向量子空间。 空间$\hat{E}$是$E_i$和子空间W的希尔伯特和，$\overline{V}$在$\hat{E}$的正交补集；将 $x_0 = p_W(x)$ 和 $x_i = p_{E_i}(x)$ 放入所有 $i \in I$。由科。 1，我们有$\|x\|^2 = \|x_0\|^2 + \sum_{i \in I} \|x_i\|^2$，$\hat{E}$中有$x = x_0 + \sum_{i \in I} x_i$。这意味着断言 1)，并且 2) 的条件 b) 和 c) 相当于条件 $x_0 = 0$，因此相当于条件 $x \in V$。最后，如果V是完整的，并且如果我们放入$x' = p_V(x)$，我们就有$x' - x_i = (x - x_i) - (x - p_V(x))$，因此$x' - x_i$与$E_i$正交，因此$x_i = p_{E_i}(x')$对于所有$i \in I$；现在将性质 2) 应用于向量 $x'$ 就足够了。

#### 注 {#evt-v-s2-n2-rem-1 .statement tag=07ZE}

令 E 为 Hausdorff prehilbertian 空间，$(V_i)_{i \in I}$ E 的向量子空间族，使得对于不同指标 $i, k$、子空间 $V_i$ 和 $V_k$ 的每个对都是正交的。 Then, for every $k \in I$, the intersection of $V_k$ and of the closed vector subspace $W_k$ generated by the union of the $V_i$ for all $i \neq k$ reduces to 0 for, if $x$ belongs to $V_k$ and also to $W_k$, then it is orthogonal to all the $V_i$ for $i \neq k$, hence to $W_k$. 特别地，$x$与其自身正交，因此是零。

#### 命题 2 {#evt-v-s2-prop-2 .statement tag=07ZF}

— 令 E 为希尔伯特空间且 $(V_\lambda)_{\lambda \in L}$ E 的闭向量子空间族；对于每个$\lambda \in L$，令$(W_{\lambda \mu})_{\mu \in M_\lambda}$是$V_\lambda$的闭族向量子空间，使得$V_\lambda$是该族的并生成的闭族向量子空间。在阶中，E是族$(W_{\lambda \mu})_{\lambda \in L, \mu \in M_\lambda}$的希尔伯特和，E是族$(V_\lambda)_{\lambda \in L}$的希尔伯特和是充分必要的，并且对于每个$\lambda \in L$，$V_\lambda$是族和的希尔伯特和 $(W_{\lambda \mu})_{\mu \in M_\lambda}$（“希尔伯特和的结合性”）。

为了证明条件是必要的，只要看到 $V_\alpha$ 和 $V_\beta$ 是正交的，如果 $\alpha \neq \beta$ 就足够了。但是，$W_{\alpha \mu}$ ($\mu \in M_\alpha$) 的每个元素都与所有 $W_{\beta v}$ ($v \in M_\beta$) 正交，因此与它们生成的闭向量子空间 $V_\beta$ 正交；同样的论证表明，$V_\beta$的每个元素都与$V_\alpha$正交，即与所有$W_{\alpha \mu}$（$\mu \in M_\alpha$）正交。

为了证明条件是充分的，只要验证一下，如果满足的话，E等于$W_{\lambda \mu}$的并生成的闭向量子空间F就足够了（$\lambda \in L$，μ ∈ M_λ）；但是，对于每个 λ ∈ L，F 包含由 W_{λμ} 的并生成的闭向量子空间，使得 μ ∈ M_λ，即 F 包含 V_λ；因此F是V_λ的并生成的闭向量子空间，即E由假设生成。

### 3. 正交族

#### 定义 3 {#evt-v-s2-def-3 .statement tag=07ZG}

在前希尔伯特空间中，如果 e_i 和 e_k 对于所有 i ≠ k 都是正交的，则向量的族 (e_i)_{i∈I} 被称为正交，并且如果对于所有 $i \in I$ 在加法 $\|e_i\| = 1$ 中，则被称为正交。

E 的子集 S 使得由恒等映射从 S 到自身定义的族是正交的，则称为正交集合。如果 (e_i)_{i∈I} 是正交族，则映射 $i \mapsto e_i$ 是单射；然后我们就可以漠不关心地谈论正交族或正交集合。

如果 (e_i)_{i∈I} 是正交族，则完整的一维向量子空间 D_i = Ke_i 是二乘二正交。对于每个 x ∈ E，x 在 D_i 上的正交投影是 $\lambda_i e_i$ 和 $⟨e_i|x - \lambda_i e_i⟩ = 0$，从而给出 $⟨e_i|x⟩ = \lambda_i ⟨e_i|e_i⟩ = \lambda_i$。将No. 2应用于子空间D_i的结果意味着以下命题：

#### 命题 3 {#evt-v-s2-prop-3 .statement tag=07ZH}

在 Hausdorff prehilbertian 空间 E 中，每个正交族在拓扑上都是独立的。

我们注意到，这个性质紧随拓扑独立族的刻画（IV，p. 1和II，p. 43，cor.2），因为根据K等于R或空间共轭来识别E的对偶与E的完成或空间共轭到E C（V、p. 17、注）。

#### 命题 4 {#evt-v-s2-prop-4 .statement tag=07ZI}

令 E 为豪斯多夫前希尔伯特空间，(e_i)_{i∈I}为 E 中的正交族，V 由 e_i 生成的 E 的闭向量子空间。

1) 对于每个 x ∈ E，我们有

$$
\sum_{i\in I} |⟨e_i|x⟩|^2 \leq \|x\|^2
$$

（贝塞尔的不等式）；这里所有$i \in I$中的集合使得$⟨e_i|x⟩ \neq 0$是可数的。此外，以下条件是等价的：a）$x \in V$； b）$\|x\|^2 = \sum_{i\in I} |⟨e_i|x⟩|^2$； c) 族$⟨e_i|x⟩.e_i$在E和$x = \sum_{i\in I} ⟨e_i|x⟩.e_i$中可求和。

2) 如果V是完备的，那么对于所有$x \in E$和$\sum_{i\in I} ⟨e_i|x⟩.e_i = p_V(x), \sum_{i\in I} |⟨e_i|x⟩|^2 = \|p_V(x)\|^2$，所有$⟨e_i|x⟩.e_i$的族在E中是可求和的。

3) 假设V是完整的。对于每个标量族$(\lambda_i)_{i\in I}$，例如$\sum_{i\in I} |\lambda_i|^2 < +\infty$，都存在一个唯一的点$x \in V$，使得$⟨e_i|x⟩ = \lambda_i$对于所有$i \in I$。如果 $(\mu_i)_{i\in I}$ 是第二个标量族，使得 $\sum_{i\in I} |\mu_i|^2 < +\infty$，并且如果对于所有 $i \in I$，$y \in V$ 使得 $⟨e_i|y⟩ = \mu_i$，则 $⟨x|y⟩ = \sum_{i\in I} \overline{\lambda_i} \mu_i$。

#### 命题 5 {#evt-v-s2-prop-5 .statement tag=07ZJ}

— 令 $(e_i)_{i \in I}$ 为 Hausdorff prehilbertian 空间 E 中的正交族。以下属性是等效的：
a) 家庭总人数$(e_i)$；
b) 对于每个$x \in E$，族$\langle e_i | x \rangle \cdot e_i$在E中可求和，并且我们有$x = \sum_{i \in I} \langle e_i | x \rangle \cdot e_i$；
c) 对于每 $x \in E$，

$$
\|x\|^2 = \sum_{i \in I} |\langle e_i | x \rangle|^2
$$

（帕塞瓦尔的关系）。

当 E 是希尔伯特时，这些条件也相当于：
d) 关系 $\langle e_i | x \rangle = 0$ 对于所有 $i \in I$ 意味着 $x = 0$。

条件 a)、b)、c) 的等价紧随 prop. 4. 当 E 为希尔伯特时，条件 a) 和 d) 的等价由 cor 得出。 1 个V、p. 16。

#### 定义 4 {#evt-v-s2-def-4 .statement tag=07ZK}

— Hausdorff prehilbertian 空间 E 中的正交和全族称为 E 的正交基。

Hausdorff prehilbertian 空间 E 的正交基也是 E 的完备性的正交基。

令 $(e_i)_{i \in I}$ 为 E 的正交基；对于每个$x \in E$，数$\langle e_i | x \rangle$，通过滥用语言，称为$x$相对于基$(e_i)$的坐标。对于 E 中的每个 $x$ 和 $y$，我们有

$$
\langle x | y \rangle = \sum_{i \in I} \overline{\langle e_i | x \rangle} \langle e_i | y \rangle .
$$

一般来说，E 的正交基不是 A、II、p. 25 中定义的意义上的 E 相对于域 K 的基；为了避免任何混淆，我们总是说 loc 意义上的前希尔伯特式空间 E 的基。引用。是 E 对 K 的代数基。

令 E 和 F 为两个豪斯多夫预希尔伯特空间和 $u$ 从 E 到 F 的连续线性映射。令 $(e_i)_{i \in I}$（或 $(f_j)_{j \in J}$）为 E（或 F）的正交基。放

$$
u_{ji} = \langle f_j | u(e_i) \rangle
$$

$i \in I,\ j \in J$。相对于正交基 $(e_i)$ 和 $(f_j)$，$(u_{ji})_{(i,j) \in I \times J}$ 族被称为 $u$ 的矩阵。设$x \in E$和$y = u(x)$；如果我们分别为 $x$ 和 $y$ 的坐标写为 $\xi_i = \langle e_i | x \rangle$ 和 $\eta_j = \langle f_j | y \rangle$，则所有 $j \in J$ 都会得到 $\eta_j = \sum_{i \in I} u_{ji} \xi_i$。当$(e_i)$是E的代数基并且$(f_j)$是F的代数基时，我们的定义与A的II, § 10, No. 4一致。

#### 例 {#evt-v-s2-n3-exa-1 .statement tag=07ZL}

令 E 为 $\mathbf{R}$ 上所有复值连续函数的空间，使得 $x \in \mathbf{R}$ 和 $n \in \mathbf{Z}$ 为 $f(x + n) = f(x)$。我们将标量乘积分配给 E，定义为

$$
\langle f | g \rangle = \int_0^1 \overline{f(t)}\ g(t)\ dt .
$$

那么 E 是豪斯多夫前希尔伯特空间，但不完备。对于每个整数$n \in \mathbf{Z}$，让$e_n(x) \in \mathbf{e}(nx)$。 $(e_n)_{n \in \mathbf{Z}}$在E中是正交的，它是直接的。而且，E上一致收敛的拓扑比从范数$\|f\|_2 = \langle f|f \rangle^{1/2}$推导出来的拓扑是更细。对于一致收敛 (GT, X, § 4, No. 4)，族 $(e_n)_{n \in \mathbf{Z}}$ 在 E 中是总的，而 *更不必说* 在前希尔伯特空间 E 中。因此，$(e_n)_{n \in \mathbf{Z}}$ 是 E 的正交基。

### 4. 正交化

#### 定理 2 {#evt-v-s2-thm-2 .statement tag=07ZM}

*对于希尔伯特空间 E 中的每个正交集合 L，都存在 E 包含 L 的正交基 B。*

事实上，令 $\mathfrak{D}$ 为 E 的所有正交子集的族，按包含线性排序；这个族有有限的特征标（S，III, § 4, No. 5）是直接的。因此，在 $\mathfrak{D}$ 包含 L 中存在一个*极大*族 B。 S 1，III, § 4, No. 5。还需要证明 B 的总和是集合。如果不是，则存在与B的所有向量正交的向量$y \neq 0$（V，p. 22，命题5），将y乘以合适的标量，我们可以假设$\|y\| = 1$；那么，$B \cup \{y\}$ 将是与 B 和包含 B 不同的正交集合； B的这个与……矛盾定义；因此定理。

#### 推论 1 {#evt-v-s2-thm-2-cor-1 .statement tag=07ZN}

*在每个希尔伯特空间中，都存在一个正交基。*

应用th就足够了。 2 到案例$L = \varnothing$。

#### 推论 2 {#evt-v-s2-thm-2-cor-2 .statement tag=07ZO}

*每个希尔伯特空间同构于空间$\ell^2(I)$。*

更准确地说，令 $(e_i)_{i \in I}$ 为希尔伯特空间 E 的正交基。通过道具。 4 (V, p. 21) 和 5 (V, p. 22), 映射 $\phi$ 定义为
$$
\phi(x) = (\langle e_i|x \rangle)_{i \in I}
$$
是从 E 到 $\ell^2(I)$ 的希尔伯特空间同构。 逆同构 $\psi$ 定义为
$$
\psi((\lambda_i)_{i \in I}) = \sum_{i \in I} \lambda_i e_i .
$$

#### 命题 6 {#evt-v-s2-prop-6 .statement tag=07ZP}

*设 E 为 Hausdorff prehilbertian 空间，并设 $(a_n)_{n \in I}$（$\mathbf{N}$ 的 I 区间，原点为 1）是 E 的向量可数（有限或非）独立族。存在正交族 $(e_n)_{n \in I}$，且仅一，在E中，具有以下属性：

1) 对于每个整数$p \in I$，$e_1, e_2, ..., e_p$生成的E的向量子空间与$a_1, a_2, ..., a_p$生成的E的向量子空间相同；
2) 对于每个整数 $p \in I$，数 $\langle a_p|e_p \rangle$ 都是实数，$> 0$。

事实上，令 $V_n$ 为$a_1, a_2, ..., a_n$ 生成的子空间（维数 n）。如果$n + 1 \in I$和$b_{n+1} = a_{n+1} - p_{V_n}(a_{n+1})$（其中$p_{V_n}$是完整的子空间$V_n$上的正射投影），则线$K b_{n+1}$是$V_{n+1}$中$V_n$的正交。如果命题的$e_n$满足条件1)，我们必须有$e_{n+1} = \lambda b_{n+1}$； 条件$\|e_{n+1}\| = 1$则意味着$|\lambda|^2 \|b_{n+1}\|^2 = 1$并且条件$\langle a_{n+1}|e_{n+1} \rangle > 0$意味着$\lambda \langle a_{n+1}|b_{n+1} \rangle > 0$；这完全确定$\lambda$，并且我们已经证明，我们可以通过归纳，一个正交族$(e_n)_{n \in I}$，并且只有一个，来确定，从而命题的满足条件1）和2）。

据说序列$(e_n)_{n \in I}$是通过独立族$(a_n)_{n \in I}$的“正交归一化”获得的。显然，$(e_n)$族生成的向量子空间与$(a_n)$族生成的向量子空间相同。特别是，如果 $(a_n)$ 是总序列，则 $(e_n)$ 也是，那么它就是 E 的正交基；因此我们得到：

#### 推论 {#evt-v-s2-n4-cor-1 .statement tag=07ZQ}

*在每个 Hausdorff prehilbertian 空间 E 满足可数性第一公理中，都存在可数正交基。*

如果E满足可数性第一公理，则E中存在总序列，并且我们总能从这样的序列（A，II, § 7, No. 1，第2）中提取一个独立的总族。

我们可以给出 Hausdorff prehilbertian 空间的例，不具有任何正交标准基（V，p. 70，练习 2）。
#### 例 {#evt-v-s2-n4-exa-1 .statement tag=07ZR}

令I为$\mathbf{R}$的区间$(-1, 1)$和I上的实值连续函数的E向量空间。令$x$表示从I到$\mathbf{R}$的典范嵌入，视为E的元素。根据Stone-Weierstrass，定理序列$(x^n)_{n \in \mathbf{N}}$是均匀收敛GT的拓扑在E中的总和， X, § 4, No. 2）。
将 E 视为实数 Hausdorff prehilbertian 空间，其中标量乘积由下式给出
$$
\langle f | g \rangle = \int_{-1}^{1} f(t) \, g(t) \, dt .
$$
序列 $(x^n)_{n \in \mathbf{N}}$ 则在前希尔伯特空间 E 中求和。令 $(\Pi_n)_{n \in \mathbf{N}}$ 为通过序列 $(x^n)_{n \in \mathbf{N}}$ 正交化获得的序列。我们可以证明 $\Pi_n = (n + \frac{1}{2})^{1/2} P_n$，其中勒让德多项式 $P_n$ 定义为
$$
P_n(x) = \frac{1}{2^n n!} \left( \frac{d}{dx} \right)^n (x^2 - 1)^n .
$$

#### 命题 7 {#evt-v-s2-prop-7 .statement tag=07ZS}

*在希尔伯特空间 E 中，两个正交基是等价的。*

令 B 和 C 为 E 的两个正交基。当两个集合 B、C 之一是有限的情况是微不足道的，因为有限正交基是空间的代数基。因此假设 B 和 C 是无限的。对于每个$x \in B$，令$C_x$为所有$y \in C$的C由……组成中的子集，使得$\langle x | y \rangle \neq 0$。 集合 $C_x$ 是可数的（V，p. 21，道具 4）。对于每个$y \in C$，都存在$x \in B$使得$y \in C_x$，因为B是正交的基和$y \neq 0$；在其他字C是可数集$C_x$的并，因为$x$范围超过B。C的基数因此小于$\mathbf{N} \times B$的基数，因此小于B的基数（S，III, § 6, No. 3，cor.4）；类似地，B的基数小于C；这样就完成了证明。

希尔伯特空间 E 的任意正交基的基数称为 E 的 *希尔伯特维数*。

#### 推论 1 {#evt-v-s2-prop-7-cor-1 .statement tag=07ZT}

*给定希尔伯特空间 E 中的两个正交基，存在 E 的自同构将第一个基转换为第二个。*

#### 推论 2 {#evt-v-s2-prop-7-cor-2 .statement tag=07ZU}

— 在阶中，希尔伯特空间、$\ell^2(I)$和$\ell^2(J)$同构的，I和J等价是充分必要的。

### 习题 {#evt-v-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
