---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 4
section_title: The height of a valuation
lang: zh
source: ac-i-vii
book_pages: 393-399, 449-453
pdf_pages: 0411-0417, 0467-0471
extraction: ocr
subsections:
    - "no": 1
      title: INCLUSION OF VALUATION RINGS OF THE SAME FIELD
      page: 393
      pdf_page: 411
    - "no": 2
      title: ISOLATED SUBGROUPS OF AN ORDERED GROUP
      page: 394
      pdf_page: 412
    - "no": 3
      title: COMPARISON OF VALUATIONS
      page: 395
      pdf_page: 413
    - "no": 4
      title: THE HEIGHT OF A VALUATION
      page: 396
      pdf_page: 414
    - "no": 5
      title: VALUATIONS OF HEIGHT 1
      page: 397
      pdf_page: 415
statements: 18
exercises: 11
content_sha256: edea06520931b2926e8ffb8e041c60a172ee07bfd955a0542bcee774f4b0dcde
translated_from: content/en/ac/VI/04_s4_the_height_of_a_valuation.md
translation_method: google
source_content_sha256: c4cced628ead73d8a7f7dea6021c8771973779a0bf6c280142bacc5c87e4b329
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 6f0b717ac2d38e6e7c34fcb2c208eac3996a0ddb4ca09b2881165c78436cac43
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4. 估值的高度

### 1. 包含相同的环估值域

#### 命题 1 {#ac-vi-s4-prop-1 .statement tag=04TV}

*令$K$为域，且$A$为$K$的估值环。然后：*
(a) *每个环$B$使得$A \subset B \subset K$是环对$K$的估值；
(b) *此类环的最大理想$m(B)$包含在$A$中，并且它是$A$的素理想；
(c) *映射$\mathfrak{p} \mapsto A$，是$A$素理想的集合递减双射到环$B$的集合，使得$A \subset B \subset K$；它的逆双射是映射$B \mapsto m(B)$。

如果$B$是环使得$A \subset B \subset K$和$x \in K - B$，则$x \in K - A$，从而$x^{-1} \in m(A) \subset B$，这证明$B$是$K$的估值环并且$m(B) \subset m(A)$；由于$m(B) = m(B) \cap A$是$A$的素理想，我们已经证明了（a）和（b）。此外，$A_{m(B)} \subset B$；相反，如果$x \in B - A$，则$x^{-1} \in A$和$x^{-1} \notin m(B)$，因此$x \in A_{m(B)}$；因此$A_{m(B)} = B$。最后令$\mathfrak{p}$为$A$的素理想；我们写$B = A_{\mathfrak{p}}$；然后$m(B) \cap A = \mathfrak{p}$。 （章II, § 2, no. 5，命题11）和$m(B) \subset A$由（b）；因此$m(B) = \mathfrak{p}$，这表明映射$\mathfrak{p} \mapsto A$和叙述的$B \mapsto m(B)$是逆双射。

#### 推论{#ac-vi-s4-n1-cor-1 .statement tag=04TW}

*K 包含于 A 的集合 & 子环完全按包含排序。*

$A$素理想的集合完全按包含排序（$\S$ 1, no. 2, 定理 1 (e)），映射 $\mathfrak{p} \mapsto A_{\mathfrak{p}}$反转包含关系。

#### 命题 2 {#ac-vi-s4-prop-2 .statement tag=04TX}

*令 K 为域，B 为 K 和 h 的估值环，h 是与 B 相关的地点和 K（$\kappa(B)$ 中的值）。然后将B中K的估值环的集合$\mathscr{A}$的映射$A \mapsto h_B(A)$定义双射转移到$\kappa(B)$的估值环的集合$\mathscr{A}'$。

如果$A \in \mathscr{A}$，则$h_B(A) \in \mathscr{A}'$：因为如果$x' = h_B(x)$（其中$x \in B$）是$\kappa(B) - h_B(A)$的元素，则$x \notin A$，因此$x^{-1} \in A$和$h_B(x)^{-1} \in h_B(A)$。另一方面，对于 $A \in \mathscr{A}$、$A \supset m(B)$ (命题 1 (b)) 以及映射，

$A \mapsto h_B(A)$ 是单射的。最后令$A' \in \mathscr{A}'$和$A = h_B(A') \subset B$；我们将展示$A \in \mathscr{A}$，这将完成证明；如果$x \in K - A$，则$x \notin B$或$x \in B$；如果$x \notin B$，则$x^{-1} \in m(B) \subset A$；如果$x \in B$，则$h_B(x) \in \kappa(B)$和$h_B(x) \notin A$，因此$h_B(x^{-1}) \in A$，我们再次结论$x^{-1} \in A$；因此$A \in \mathscr{A}$。

#### 推论{#ac-vi-s4-n1-cor-2 .statement tag=04TY}

*令A和B为K的两个估值环，其中$A \subset B$；让$A' = h_B(A)$，这是$\kappa(B)$的估值环。 $A'$ 的剩余类域 $\kappa(A')$ 与 A 的剩余类域 $\kappa(A)$ 自然同构，与 A 关联的位置 $h_A$ 是与 A 和 B 关联的位置的合成 $h_{A'} \circ h_B$。*

由于局部环 $A'$ 是局部环 $A$ 的商，因此它们的剩余类域是规范同构的，并且方程 $h_A(x) = h_{A'}(h_B(x))$ 对于 $x \in A$ 成立。另一方面，如果$x \in B - A$，则$h_B(x) \notin A'$和方程两边等于$\infty$；如果 $x \in K - B$ 也是如此。

#### 注 {#ac-vi-s4-n1-rem-1 .statement tag=04TZ}

相反，令$f$是K的一个地方，值在$K'$中，而$f'$是$K'$的一个地方，值在$K''$中。那么$f' \circ f$就是K的一个地方，它的环包含在$f$地方的环中。

### 2. 隔离子群有序群

为了从估值的角度研究no. 1和点的情况，我们需要下面的定义1和命题3。

#### 定义 1 {#ac-vi-s4-def-1 .statement tag=04U0}

*如果关系$0 \leq y \leq x$且$x \in H$隐含$y \in H$，则有序群G的子群H称为孤立的。*

#### 例 (1) {#ac-vi-s4-n2-exa-1 .statement tag=04U1}

设$A$和$B$是两个有序的群；让$A \times B$按照字典顺序给出阶（即“$(a, b) \leq (a', b')$”相当于“$(a < a') \text{ or } (a = a' \text{ and } b \leq b')$”）。如立即可见，$A \times B$ 的第二个因子 $B$ 是$A \times B$ 的孤立子群。

#### 命题 3 {#ac-vi-s4-prop-3 .statement tag=04U2}

令 $G$ 为其正元素的有序群和 $P$ 集合。

(a) *$G$的递增同态到有序群的核是$G$的孤立子群。*

(b) *相反，令$H$是$G$的孤立子群和$G$的$g$典范同态在$G/H$上。那么$g(P)$是$G/H$上有序群结构的正元素的集合。此外，如果$G$是全序的，$G/H$也是全序的。*

(a) 令$f$为递增同态，从$G$到有序的群；让 $H$ 表示核关闭。如果$0 \leq y \leq x$和$x \in H$，则$0 \leq f(y) \leq f(x) = 0$，从而$f(y) = 0$，即$y \in H$。因此$H$是孤立的。

(b) 令$H$为$G$和$g : G \to G/H$的孤立子群。让$P' = g(P)$。显然$P' + P' \subset P'$。还有

$$
P' \cap (-P') = \{0\},
$$

因为，*如果*$x$和$y$是$P$的元素，使得$g(x) = -g(y)$，则$x + y \in H$、从而、$x \in H$和$y \in H$，因为$H$是孤立的；因此$g(x) = g(y) = 0$。因此，$P'$是$G/H$上有序群结构的正元素的集合（*代数*，章VI, § 1, no. 3，命题3）。最后，如果$G$是全序的，那么$P \cap (-P) = G$、从而$P' \cup (-P') = G/H$，因此$G/H$是全序的（*loc.cit.*）。

#### 例 (2) {#ac-vi-s4-n2-exa-2 .statement tag=04U3}

如果我们重新考虑例，其中 $G$ 是字典式乘积 $A \times B$ 和 $H = B$，则有序的群 $G/H$ 被规范地标识为 $A$。

### 3. 估值比较

令 $K$ 为域，且 $A$ 的估值为环为 $K$。对于$K$包含$A$中的每子环$B$，$U(A) \subset U(B)$。然后还有$\Gamma_A = K^*/U(A)$到$\Gamma_B = K^*/U(B)$的典范同态$\lambda$，其核是$U(B)/U(A)$。然后，让$v_A$和$v_B$表示由$A$和$B$（§ 3, no. 2）定义的$K$的规范估值，

(1)

$$
v_B = \lambda \circ v_A.
$$

由于$A \subset B$，$\lambda$映射是$\Gamma_A$的正元素到$\Gamma_B$的正元素，因此是递增。因此，$\lambda$的(命题 3)核$H$是$\Gamma_A$和$\lambda$因子到$\Gamma_A \to \Gamma_A/H_B \xrightarrow{\mu} \Gamma_B$的孤立的子群，其中$\mu$是递增双射同态，因此是完全有序的群的*同构*；因此 $\Gamma_B$ 等同于全序商群 $\Gamma_A/H_B$。

#### 命题 4 {#ac-vi-s4-prop-4 .statement tag=04U4}

*The mapping* $B \mapsto H_B$ *is an increasing bijection of the set of subrings of* $K$ *containing* $A$ *onto the set of isolated subgroups of* $\Gamma_A$.

给定 $H$，$v_B$ 定义为等价，因此 $B$ 是唯一确定的。另一方面，令$H$是$\Gamma_A$的孤立子群；将$\Gamma_A / H$视为全序群 (命题 3)，复合映射

$$
K^* \xrightarrow{v_A} \Gamma_A \longrightarrow \Gamma_A / H
$$

是对 $K$ 的估值，其环包含 $A$。

#### 注 {#ac-vi-s4-n3-rem-1 .statement tag=04U5}

在上述假设下，令$f$表示$B$的典范同态到$\kappa(B)$和$A' = f(A)$；它的估值为环为$\kappa(B)$（命题2，no. 1）。那么$f^{-1}(\kappa(B)^*) = U(B), f^{-1}(A') = A, f^{-1}(m(A')) = m(A)$，因此

$$
f^{-1}(U(A')) = U(A).
$$

然后有$U(B)/U(A)$的典范同构到$\kappa(B)^*/U(A') = \Gamma_{A'}$。 正合序列

$$
0 \to U(B)/U(A) \to \Gamma_A \to \Gamma_B \to 0
$$

然后给出正合序列

$$
0 \to \Gamma_{A'} \to \Gamma_A \to \Gamma_B \to 0.
$$

#### 例 {#ac-vi-s4-n3-exa-1 .statement tag=04U6}

设$k$为域，

$$
E = k(X) \quad \text{and} \quad K = k(X, Y) = E(Y)
$$

$(X, Y$ 不确定）。令$B = E[Y]_{(Y)}$为$K$的估值环，由主理想整环$E[Y]$的极值元素$Y$定义（§ 1, no. 4，命题3）。 剩余类域 $\kappa(B)$ 被规范地标识为 $E[Y]/(Y) = E$。同样，令$A' = k[X]_{(X)}$为$E = k(X)$的估值环，由$k[X]$的极值元素$X$定义。用$h$表示与$B$相关的$E$的位置并写作$A = h_B^{-1}(A')$，定义了$K$的评估环$A$，其包含在$B$和$\kappa(A) = \kappa(A') = k$中。规范位置$h$：$K \to k$可以描述如下：如果$(X, Y)$是$K$的元素，那么我们首先将$Y = 0$ inf（它给出$\tilde{E} = k(X)^*$的元素），然后将$X = 0$放入获得的结果中。 群 $\Gamma_{A'}$ 和 $\Gamma_B$ 与 $\mathbf{Z}$ (§ 3, no. 4, 例 4) 自然同构。 *不难证明(cf.§ 10, no. 2,引理2)群$\Gamma_A$与词典乘积$\mathbf{Z} \times \mathbf{Z}$同构的，并且$v_A$的估值等价于§ 3, no. 4中定义的估值，结束例 6.*

### 4. 估值的高度

令$G$为全序群。 Given two isolated subgroups $H$ and $H'$ of $G$, one of them is contained in the order: for otherwise there would exist a positive element $x$ of $H$ not belonging to $H'$ and a positive element $x'$ of $H'$ not belonging to H; let, for example $x \geq x'$; as H is isolated, $x' \in H$, which is a contradiction.

这也从 no. 3 的命题 4 和 no. 1 命题 1 的推论得出，考虑到每个完全排序的群是评估的阶群 (§ 3, no. 4, 例 6)。

#### 定义 2 {#ac-vi-s4-def-2 .statement tag=04U7}

*设G是全序群。如果与 G 不同的 G 的孤立子群的数是有限的且等于 n，则称 G 的高度为 n。如果这个数是无穷大，则称 G 具有无穷高。*

例
(1) 群 $G = \{0\}$ 的高度为 0。
(2) 群 $\mathbf{Z}$ 和 $\mathbf{R}$ 的高度为 1。
(3) 设$G$为全序群，$H$为$G$的孤立子群。如果 $h(H)$ 和 $h(G/H)$ 分别表示全序群 $H$ 和 $G/H$ 的高度，那么
$$
h(G) = h(H) + h(G/H),
$$
因为$G$的孤立子群的集合是完全按包含排序的。特别地，如果 $G$ 是两个全序群 $H$ 和 $H'$ 的字典序乘积，则
$$
h(G) = h(H) + h(H')
$$
（cf.no. 2，例2）；因此字典顺序乘积 $\mathbf{Z} \times \mathbf{Z}$ 的高度为 2。

另一方面，通过嵌入$\mathbf{R}$（cf.§ 3, no. 4，例6的末尾）排序的$\mathbf{Z} \times \mathbf{Z}$的高度等于1（下面的cf.命题8）。

#### 定义 3 {#ac-vi-s4-def-3 .statement tag=04U8}

*估价阶群的高度称为该估价的高度。*

对于例，离散估值的高度为 1。只有不正确的估值的高度为 0。命题 1 和 4 意味着：

#### 命题 5 {#ac-vi-s4-prop-5 .statement tag=04U9}

*估值的高度等于其环中非零素理想的数。*

### 5. 身高估值 1

#### 命题 6 {#ac-vi-s4-prop-6 .statement tag=04UA}

*令$\mathbf{K}$为域且$A$为$\mathbf{K}$的子环。假设$A$不是域。那么下面的条件是等价的：*
(a) $A$ 是$\mathbf{K}$ 上高度 1 的估值的环；
(b) $A$是$\mathbf{K}$的估值环，除了$(O)$和$m(A)$之外没有其他素理想；
(c) $A$是与$\mathbf{K}$不同的$\mathbf{K}$的子环中最大的。

no. 4中的命题5表明(a)蕴涵(b)，而no. 1中的命题1表明(b)蕴涵(c)。仍有待证明 (c) 蕴涵 (a)。假设 A 是不同于 K 的 K 的子环中最大。设 m 是 A 的最大理想，V 是 K 支配 A_m 的评估环（§ 1, no. 2，定理 2 的推论）；因为 m(V) ∩ A = m 且 m ≠ (0)（因为 A 不是域），V ≠ K，从而 V = A，这证明 A 不是 K 上 v 的估值的环。因此，v 的高度为 1 命题 1 (no. 1) 和 5 (no. 4)。

#### 命题 7 {#ac-vi-s4-prop-7 .statement tag=04UB}

对于域的估值高度为1，其阶群同构于\mathbf{R}的非零有序子群是必要且充分的。

这实际上是从以下命题得出的：

#### 命题 8 {#ac-vi-s4-prop-8 .statement tag=04UC}

令 G 为全序群且未简化为 O。以下条件是等效的：
(a) G 的高度为 1；
(b) 对于 G 中所有 x > 0 且 y ≥ 0，存在整数 n ≥ 0，使得 y ≤ nx；
(c) G 同构于有序加法群 \mathbf{R} 的子群，且未约简为 O。

设 x 为 G 的正元素，并令 H 为 y ∈ G 的集合，使得存在整数 n ≥ 0 满足 |y| ≤ nx。很容易验证 H, 是 G 的孤立子群，并且 G 包含于 x 包含于 H, 的每个孤立子群。因此，条件 (a) 等价于“H, = G for all x > 0”，即条件 (b)。

显然（c）意味着（b）。相反，假设条件 (b) 成立，并让 Q 表示 G 的元素 >0 的集合。首先假设 Q 具有至少元素 x；对于所有 y ∈ Q，令 n 为最小整数，使得 y ≤ nx；如果 y < nx，则 nx − y ≥ x，从而 y ≤ (n − 1)x，与 n 的选择相反；则 y = nx，这表明 G = \mathbf{Z}x 与 \mathbf{Z} ⊂ \mathbf{R} 同构的。现在假设 Q 至少有元素；我们应用到一般拓扑、章V, § 2的有序集合 P = Q ∪ (0) 命题 1 （这是可能的，因为条件 (b) 只是“阿基米德公理”）；可见 P 到 \mathbf{R}_+ 存在严格递增的映射 f 使得

$$
f(x + y) = f(x) + f(y)
$$

对于 x Î P 且 y Î P；通过线性f可以将G的同构扩展到\mathbf{R}的子群，这证明了(b)蕴涵(c)。

#### 命题 9 {#ac-vi-s4-prop-9 .statement tag=04UD}

令 K 为域，v 为 K 的非不当估值，v 的 A 环。为了使 A 完全积分闭合（章 V, § 1, no. 4，定义 5），v 的高度为 1 是充分必要的。

假设 v 的高度为 1。令 x ∈ K 使得 x^n (n ≥ 0) 全部包含在 K 的有限生成的子 A 模块中。存在 d ∈ A − {0}，使得 dx^n ∈ A 对于所有 n ≥ 0。然后 v(d) + nv(x) ≥ 0，即对于所有 $n \geqslant 0$，n(−v(x)) ≤ v(d)， 从而$-v(x) \leqslant 0$（命题8（b））和$x \in A$。因此 A 是全闭的。

现在假设 v 的高度不是 1。则存在 $y \in m(A)$ 和 $t \in A$，使得 $nv(y) < v(t)$ 对于所有 $n \geqslant 0$ (命题 8 (b))。然后 $ty^{-n} \in A$ 对于所有 $n \geqslant 0$，但$y^{-1} \notin A$。因此 A 不是完全积分闭的。

#### 推论{#ac-vi-s4-n5-cor-1 .statement tag=04UE}

*设K为域，$(v_\alpha)_{\alpha \in I}$K上高度1的估值族，以及v的环的A交。*则A是一个完全积分闭域。

完全积分闭域并不总是高度 1 (习题 6) 的估值环的交。

### 习题{#ac-vi-s4-exercises}

§ 4](exercises/s4/)参见[习题。
