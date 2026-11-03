---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 4
section_title: Central filtrations
lang: zh
source: lie-i-iii
book_pages: 142-149, 187-193
pdf_pages: 0160-0167, 0205-0211
extraction: ocr
subsections:
    - "no": 1
      title: REAL FILTRATIONS
      page: 142
      pdf_page: 160
    - "no": 2
      title: ORDER FUNCTION
      page: 143
      pdf_page: 161
    - "no": 3
      title: GRADED ALGEBRA ASSOCIATED WITH A FILTERED ALGEBRA
      page: 144
      pdf_page: 162
    - "no": 4
      title: CENTRAL FILTRATIONS ON A GROUP
      page: 145
      pdf_page: 163
    - "no": 5
      title: AN EXAMPLE OF A CENTRAL FILTRATION
      page: 147
      pdf_page: 165
    - "no": 6
      title: INTEGRAL CENTRAL FILTRATIONS
      page: 148
      pdf_page: 166
statements: 12
exercises: 18
content_sha256: 4d567a9ba868197f141ad9486ec05a097ef2e9d0dff8aa466bf734f0523d7611
translated_from: content/en/lie/II/04_s4_central_filtrations.md
translation_method: google
source_content_sha256: 6dd2b136d04753cfdf0792754a0655d7811d3c21519c55e6a5ca6b7546279e90
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 14cbc22a741efd767857a24573a763717e476d9b22cbc84a301769ff0e69fb91
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。中央过滤

### 1. 真正的过滤

#### 定义 1 {#lie-ii-s4-def-1 .statement tag=0A4H}

设$G$为群。对$G$的真正过滤是$G$的子群的$(G_\alpha)_{\alpha \in \mathbf{R}}$族，使得
$$
G_\alpha = \bigcap_{\beta < \alpha} G_\beta \quad \text{for all } \alpha \in \mathbf{R}.
$$

公式 (1) 意味着 $\beta < \alpha$ 为 $G_\alpha \subset G_\beta$，因此族 $(G_\alpha)$ 是 *递减*。如果$\bigcap_\alpha G_\alpha$约化到单位元素，则过滤$(G_\alpha)$称为*分离*，如果$G = \bigcup_\alpha G_\alpha$，则称为*详尽*。

#### 注 {#lie-ii-s4-n1-rem-1 .statement tag=0A4I}

设$(G_n)_{n \in \mathbf{Z}}$为$G$的子群中的递减序列。 它是*交换代数*、章III, § 2, no. 1、定义1意义上的递减过滤。 对于$\mathbf{R}$的区间$]n-1, n]$中的每个整数$n$和所有$\alpha$，我们写$H_\alpha = G_n$，特别是$H_n = G_n$。 因此，我们立即获得了对 $G$ 的真正过滤 $(H_\alpha)_{\alpha \in \mathbf{R}}$；这种过滤称为“整体过滤”。 因此，*交换代数*、章III, § 2意义上的递减过滤可以通过积分过滤来识别。

设$A$为代数；如果$A_\alpha . A_\beta \subset A_{\alpha + \beta}$适用于$\mathbf{R}$中的$\alpha, \beta$，$K . A_\alpha \subset A_\alpha$适用于$\alpha \in \mathbf{R}$，则$A$的加法群上的真实过滤$(A_\alpha)$称为与代数结构兼容。如果过滤是彻底的，则$(A_\alpha)$是$A$上拓扑下0的邻域的基本系统，与代数结构兼容。设$B$为单位代数；如果代数结构和$1 \in B_0$ 相容的，则$B$ 加法群上的真实过滤$(B_\alpha)$ 称为与单位代数结构兼容。

### 2. 阶函数

设 $G$ 为群，其中单位元素 $e$。令$(G_\alpha)$为$G$的真实过滤。对于$G$中的所有$x$，令$I_x$表示实数$\alpha$中的集合，使得$x \in G_\alpha$。如果$\alpha \in I_x$和$\beta < \alpha$，则$\beta \in I_x$，因此$I_x$是区间（*一般拓扑*，章IV, § 2, no. 4，命题1）。使用关系 (1)，我们看到当它是有限的时，$I_x$ 包含是最小的上界。因此$I_x$等于形式$]-\infty, v(x)] \cap \mathbf{R}$和$v(x) \in \overline{\mathbf{R}}$；我们有$v(x) = \sup \{ \alpha \mid x \in G_\alpha \}$。

$G$的映射$v$进入$\overline{\mathbf{R}}$称为与实际过滤$(G_\alpha)$相关的*阶函数*，$v(x)$称为$x$的*阶*。这个映射有以下性质：

(a) *对于$x \in G$和$\alpha \in \mathbf{R}$，关系$x \in G_\alpha$和$v(x) \geq \alpha$是等价的。*

(b) *对于$G$中的$x, y$，*
$$
v(x^{-1}) = v(x), \qquad v(e) = +\infty.
$$
$$
v(xy) \geq \inf(v(x), v(y)).
$$

*此外，如果 $v(x) > v(y)$，则 (3) 中我们有等式。*

(c) *对于所有$\alpha \in \mathbf{R}$，令$G_\alpha^+$表示$x \in G$的集合，使得$v(x) > \alpha$。那么 $G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta$，特别是 $G_\alpha^+$ 是子群的 $G$。*

相反，令$v$为$G$的映射代入$\overline{\mathbf{R}}$满足关系(2)和(3)。对于所有$\alpha \in \mathbf{R}$，令$G_\alpha$为$x \in G$的集合，使得$v(x) \geq \alpha$。那么$(G_\alpha)_{\alpha \in \mathbf{R}}$是$G$的真实过滤，$v$是与该过滤相关的阶函数。

为了使过滤$(G_\alpha)$成为整体，将$v$映射$G$转化为$\mathbf{Z} \cup \{+\infty, -\infty\}$是必要且充分的。为了使其详尽（或分离），$-v^{-1}(-\infty) = \varnothing$（或$-v^{-1}(+\infty) = \{\epsilon\}$）是必要且充分的。

令$A$为K-代数（分别为单位K-代数）。综上所述，关系

$$
"x \in A_\alpha \Leftrightarrow v(x) \geq \alpha \quad \text{for } x \in A \text{ and } \alpha \in \mathbf{R}"
$$

定义双射 / 集合详尽的真实过滤$(A_\alpha)_{\alpha \in \mathbf{R}}$ 与代数（分别为单元代数）结构于$A$ 到集合于映射 $v : A \to \overline{\mathbf{R}}$ 不采用值 $-\infty$ 和满足公理 (4) 至 (7)（分别为 (4) 至 (8)）：

(4) $$v(x + y) \geq \inf(v(x), v(y)) \quad (x, y \text{ in } A)$$
(5) $$v(-x) = v(x) \qquad (x \in A)$$
(6) $$v(\lambda x) \geq v(x) \qquad (\lambda \in K, x \in A)$$
(7) $$v(xy) \geq v(x) + v(y) \qquad (x, y \text{ in } A)$$
(8) $$v(1) \geq 0.$$

#### 注 {#lie-ii-s4-n2-rem-1 .statement tag=0A4J}

如果 $v(x)$ 并非处处都等于 $+\infty$，则条件 (7) 和 (8) 意味着 $v(1) = 0$。

### 3. 分级代数与过滤后的代数相关

令 $G$ 成为具有真实过滤 $(G_\alpha)_{\alpha \in \mathbf{R}}$ 的*可交换* 群。正如之前我们写的

$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta;
$$

显然 $G_\alpha^+$ 是 $G_\alpha$ 中的子群。我们写 $\operatorname{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ 并且

$$
\operatorname{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \operatorname{gr}_\alpha(G).
$$

与过滤后的群* $G$ 伴随的 *分级群为群 $\operatorname{gr}(G)$，其自然分级为型 $\mathbf{R}$。

#### 注 {#lie-ii-s4-n3-rem-1 .statement tag=0A4K}

当过滤$(G_\alpha)$为积分时，$\operatorname{gr}_\alpha(G) = \{0\}$为非积分$\alpha$，$\operatorname{gr}_n(G) = G_n / G_{n-1}$为每个整数$n$。相关分级的群的定义因此重合本质上与*交换代数*、章III, § 2, no. 3相同。

令$A$为代数（分别为单位代数），并且$(A_\alpha)_{\alpha \in \mathbf{R}}$为与代数（分别为单位代数）结构（no. 1）兼容的真实过滤。然后

$$
A_\alpha \cdot A_\beta \subset A_{\alpha + \beta}, \qquad A_\alpha^+ \cdot A_\beta + A_\alpha \cdot A_\beta^+ \subset A_{\alpha + \beta}^+
$$

以及将商双线性映射在$A$定义上将$A_\alpha \times A_\beta$的双线性映射转换为$A_{\alpha + \beta}$限制的乘法

$$
\operatorname{gr}_\alpha(A) \times \operatorname{gr}_\beta(A) \to \operatorname{gr}_{\alpha + \beta}(A).
$$

我们将 gr(A) × gr(A) 的双线性映射推导为 gr(A)，这使其成为型 $\mathbf{R}$ 的分级代数（分别为单位分级代数）。如果 A 是结合律（分别是交换律、谎言）代数，那么 gr(A) 也是结合律。

### 4. 群上的中央过滤

#### 定义 2 {#lie-ii-s4-def-2 .statement tag=0A4L}

设G为群。 如果$G = \bigcup_{\alpha > 0} G_\alpha$且$G_\alpha$的元素x和$G_\beta$的元素y的交换子$(x, y) = x^{-1}y^{-1}xy$属于$G_{\alpha + \beta}$，则G上的实过滤$(G_\alpha)$称为中心过滤。

在阶函数v的项中，上面的定义转化为关系
$$
v(x) > 0, \quad v((x, y)) \geq v(x) + v(y) \quad \text{for all } x, y \text{ in } G.
$$
我们推断 $v((x, y)) > v(x)$ if $v(x) \neq +\infty$;如果我们写 $x^y = y^{-1}xy$ (cf. 代数, 章 I, § 6, no. 2)，那么 $x^y = x.(x, y)$, 从而
$$
v(x^y) = v(x).
$$
这个关系表达了G的子群$G_\alpha$都是正规的。 $G_\alpha$形式e的邻域的基本系统对于拓扑与G上的群结构兼容（一般拓扑，章III, § 1, no. 2，例）据说是由过滤定义的$(G_\alpha)$。

在该编号的其余部分中，G 表示群，带有中央过滤 $(G_\alpha)$。对于所有 $\alpha \in \mathbf{R}$，我们将 G 的定义子群 $G_\alpha^+$ 通过
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta.
$$
特别是 $G_\alpha^+ = G_\alpha = G$ 对应 $\alpha \leq 0$。回想一下，如果 A 和 B 是 G 的两个子群，则 (A, B) 表示由换位子 $(a, b)$ 与 $a \in A$ 和 $b \in B$ 生成的 G 的子群。有了这个记号，我们就有了公式
$$
(G_\alpha, G_\beta) \subset G_{\alpha + \beta}
$$
$$
(G_\alpha^+, G_\beta^+) \subset G_{\alpha + \beta}^+
$$
$$
(G, G_\alpha) \subset G_\alpha^+.
$$
根据(14)，对于所有$\alpha \in \mathbf{R}$，$G_\alpha^+$是$G_\alpha$的正常子群，并且商群$\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$是可交换的。我们写$\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$，并给这个群型$\mathbf{R}$的毕业，其中$\mathrm{gr}_\alpha(G)$由次数$\alpha$的元素组成。然后$\mathrm{gr}_\alpha(G) = \{0\}$换$\alpha \leq 0$。

#### 命题 1 {#lie-ii-s4-prop-1 .statement tag=0A4M}

(i) 设$\alpha, \beta$在$\mathbf{R}$中。存在双加法映射
$$
\phi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)
$$

其中映射$(xG_\alpha^+, yG_\beta^+)$到$(x, y)G_{\alpha+\beta}^+$。

(ii) 设$\phi$为$\mathrm{gr}(G) \times \mathrm{gr}(G)$到$\mathrm{gr}(G)$的双加法映射，对于每个有序对$(\alpha, \beta)$，限制到$\mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G)$是$\phi_{\alpha\beta}$。 映射$\phi$给出$\mathrm{gr}(G)$一个谎言$\mathbf{Z}$-代数结构。

(i) 回忆身份

$$(xx', y) = (x, y)x'(x', y)$$

对于$G$中的$x, x', y$（*代数*、章I, § 6, no. 2、公式（4之二））。

对于$x \in G_\alpha$和$y \in G_\beta$，$G_{\alpha+\beta}$的元素$(x, y)$对$G_{\alpha+\beta}^+$取模类将表示为$f(x, y)$。对于$G_{\alpha+\beta}$中的$a$和$G$中的$x'$、$a^{-1}.ax' = (a, x') \in G_{\alpha+\beta}^+$；特别地，$f(x, y)$等于类对$G_{\alpha+\beta}^+$对$(x, y)x'$取模。 公式 (15) 因此意味着

$$f(xx', y) = f(x, y)f(x', y).$$

现在$(y, x) = (x, y)^{-1}$，从而

$$f(y, x) = f(x, y)^{-1}.$$

由(16)和(17)我们推导出

$$f(x, yy') = f(x, y)f(x, y').$$

我们必须在取商映射$\phi_{\alpha\beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha+\beta}(G)$时证明映射$f : G_\alpha \times G_\beta \to \mathrm{gr}_{\alpha+\beta}(G)$定义。由(16)和(18)足以证明$f(x, y) = 0$如果$x \in G_\alpha^+$或$y \in G_\beta^+$，这是从(13')得出的。

(ii) 作为 $(x, x) = e$，从 (17) 可以得出 $\phi$ 是交错的 $\mathbf{Z}$-双线性映射。因此，还需要证明，对于 $u \in \mathrm{gr}_\alpha(G)$、$v \in \mathrm{gr}_\beta(G)$ 和 $w \in \mathrm{gr}_\gamma(G)$，

$$\phi(u, \phi(v, w)) + \phi(v, \phi(w, u)) + \phi(w, \phi(u, v)) = 0.$$

令$x \in G_\alpha, y \in G_\beta$和$z \in G_\gamma$为元素，分别代表$u, v$和$w$。我们知道$x^y$和$x$是$G_\alpha$的两个元素，它们对模$G_\alpha^+$全等，因此$x^y$是$G_\alpha$中$u$的代表；由于$(y, z)$是$G_{\beta+\gamma}$中$\phi(v, w)$的代表，我们看到$(x^y, (y, z))$是$G_{\alpha+\beta+\gamma}$中$\phi(u, \phi(v, w))$的代表。通过循环置换，我们看到$(y^z, (z, x))$和$(z^x, (x, y))$分别代表$G_{\alpha+\beta+\gamma}$中的$\phi(v, \phi(w, u))$和$\phi(w, \phi(u, v))$。 关系 (19) 则为以下恒等式的推论 (*代数*, 章 I, § 6, no. 2, 公式 (15))：

$$(x^y, (y, z)).(y^z, (z, x)).(z^x, (x, y)) = e.$$

命题 1 中定义的李代数 $\mathrm{gr}(G)$ 超过 $\mathbf{Z}$ 称为与过滤后的群* $G$ 伴随的*分级李代数。

### 5. 中央过滤例

令 $A$ 为单位结合律代数，并带有单位代数过滤 $(A_\alpha)$，使得 $A_0 = A$；那么$A_\alpha$是所有$\alpha \in \mathbf{R}$的$A$的双面理想。让$A^*$表示$A$的可逆元中的乘法群。对于所有$\alpha > 0$，令$\Gamma_\alpha$表示$x \in A^*$的集合，使得$x - 1 \in A_\alpha$；我们将$\beta \leq 0$写为$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$和$\Gamma_\beta = \Gamma$。

#### 命题 2 {#lie-ii-s4-prop-2 .statement tag=0A4N}

*集合$\Gamma$是$A^*$的子群，$(\Gamma_\alpha)$是$\Gamma$的中央过滤。*

$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$由构造和关系$\Gamma_\alpha = \bigcap_{\beta < \alpha} \Gamma_\beta$遵循$A_\alpha = \bigcap_{\beta < \alpha} A_\beta$。

我们证明$\Gamma_\alpha$是$A^*$的子群。现在$1 \in \Gamma_\alpha$；令$x, y$位于$\Gamma_\alpha$、从而$x - 1 \in A_\alpha, y - 1 \in A_\alpha$中。由于$A_\alpha$是$A$的双面理想，公式
$$
(21) \quad xy - 1 = (x - 1)(y - 1) + (x - 1) + (y - 1),
$$
$$
(22) \quad x^{-1} - 1 = -x^{-1}(x - 1),
$$
意味着$xy - 1 \in A_\alpha$和$x^{-1} - 1 \in A_\alpha$，从而$xy \in \Gamma_\alpha$和$x^{-1} \in \Gamma_\alpha$。

作为 $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$，这是 $A^*$ 中的子群。

最后让$\alpha > 0, \beta > 0, x \in \Gamma_\alpha$和$y \in \Gamma_\beta$。让$x - 1 = \xi$和$y - 1 = \eta$。然后
$$
(23) \quad (x, y) - 1 = x^{-1}y^{-1}(\xi \eta - \eta \xi);
$$
由假设、$\xi \in A_\alpha$ 和 $\eta \in A_\beta$、从而 $\xi \eta - \eta \xi \in A_{\alpha + \beta}$。因为$A_{\alpha + \beta}$是$A$、$(x, y) - 1 \in A_{\alpha + \beta}$、从而$(x, y) \in \Gamma_{\alpha + \beta}$的双面理想。

#### 注 {#lie-ii-s4-n5-rem-1 .statement tag=0A4O}

设$\alpha \geq 0, \beta \geq 0$和$x \in \Gamma_\alpha, y \in \Gamma_\beta$。 公式 (21), (22) 和 (23),
$$
(24) \quad x^{-1} - 1 \equiv -(x - 1) \pmod{A_{2\alpha}}
$$
$$
(25) \quad xy - 1 \equiv (x - 1) + (y - 1) \pmod{A_{\alpha + \beta}}
$$
$$
(26) \quad (x, y) - 1 \equiv [(x - 1), (y - 1)] \pmod{A_{\alpha + \beta + \inf(\alpha, \beta)}}.
$$

我们证明例如（26）。如果 $x - 1 = \xi$ 和 $y - 1 = \eta$，则 (23) 给出：
$$
(x, y) - 1 - [\xi, \eta] = ((x^{-1} - 1) + (y^{-1} - 1) + (x^{-1} - 1)(y^{-1} - 1))[\xi, \eta].
$$
现在$[\xi, \eta] \in A_{\alpha + \beta}$，$(x^{-1} - 1) \in A_\alpha$，$(y^{-1} - 1) \in A_\beta$，从而我们得到（26）。

令$G$为群且$\rho : G \to \Gamma$同态。对于所有真实的$\alpha$，我们写为$G_\alpha = \rho^{-1}(\Gamma_\alpha)$。由于$(\Gamma_\alpha)$是$\Gamma$上的中央过滤，所以$(G_\alpha)$是$G$上的中央过滤是直接的。

#### 命题 3 {#lie-ii-s4-prop-3 .statement tag=0A4P}

(i) *对于所有$\alpha \in \mathbf{R}$，存在唯一群同态$g_\alpha : \mathrm{gr}_\alpha(G) \to \mathrm{gr}_\alpha(A)$，其中映射类以$G_\alpha^+$为模元素$a \in G_\alpha$到类以$A_\alpha^+$为模$\rho(a) - 1$.*

(ii) 令 g 为 gr(G) 到 gr(A) 的群同态，其中限制到 gr_\alpha(G) 是所有 α 的 g_\alpha。 映射 g 是李 \mathbf{Z}-代数的单同态。

(i) 令 α > 0。到假设，对于 G_\alpha 中的所有 a，\rho(a) - 1 \in A_\alpha；设 p_\alpha(a) 表示 \rho(a) - 1 模 A_\alpha^+ 的类。由于 A_{2\alpha} \子集 A_\alpha^+，关系 (25) 意味着 p_\alpha(ab) = p_\alpha(a) + p_\alpha(b)。那么 a \in G_\alpha^+ 当且仅当 \rho(a) - 1 \in A_\alpha^+;因此 G_\alpha^+ 是 G_\alpha 的同态 p_\alpha 的核到 gr_\alpha(A) 中。在经过到商，p_\alpha 然后将 gr_\alpha(G) 的定义单同态 g_\alpha 转化为 gr_\alpha(A)。

对于 \alpha \leq 0，gr_\alpha(G) = \{0\} 且唯一的选择是 g_\alpha = 0。

(ii) 由于 g_\alpha 对于所有实数 α 都是单射的，因此 g 是单射的。我们证明 g 是李代数同态。由于 gr_\alpha(G) = \{0\} 对于 \alpha \leq 0，足以建立公式

$$
p_{\alpha+\beta}((a, b)) = [p_\alpha(a), p_\beta(b)]
$$

对于 α > 0，β > 0，G_alpha 中的 rightarrow 和 G_beta 中的 b，由 (26) 得出。

### 6. 整体中央过滤

回想一下 (no. 1, 注)，如果对于每个整数 n 且所有 \alpha \in \{n-1, n\} 都有 G_\alpha = G_n，则群 G 上的过滤 (G_\alpha) 称为积分。在群 G 上给予积分中央过滤相当于给予 G 满足条件子群的序列 (G_n)_{n \geq 1}

(i) \quad G_1 = G
(ii) \quad G_n \supset G_{n+1} \quad \text{对于所有 } n \geq 1
$(iii) \quad (G_m, G_n) \subset G_{m+n}$适用于$m \geq 1$和$n \geq 1$。

对于每个整数 n \geq 1，G_n 是 G 的正规子群，并且商 gr_n(G) = G_n/G_{n+1} 是可交换的。将商, 映射 (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy of G_m \times G_n 代入 G_{m+n} 允许我们在 gr(G) = \bigoplus_{n \geq 1} gr_n(G) 上计算定义李代数结构型 \mathbf{N} 超过环 \mathbf{Z}。

回想一下 (代数, 章 I, § 6, no. 3, 定义 5)，群 G 的下中心级数定义为

$$
C^1G = G, \quad C^{n+1} = (G, C^nG) \quad \text{for } n \geq 1.
$$

相应的过滤称为G的下中央过滤。

#### 命题 4 {#lie-ii-s4-prop-4 .statement tag=0A4Q}

(i) G 的下部中央级数是 G 上的整体中央过滤。

(ii) 如果 (G_n)_{n \in \mathbf{N}^*} 是 G 上的积分中心过滤，则对于所有 n \in \mathbf{N}^* C^nG \子集 G_n。

断言(i)已在代数、章I, § 6, no. 3、公式(7)中得到证明。

我们通过 n 上的归纳证明 (ii)； C^1G = G = G_1;对于 n > 1，

$$
C^nG = (G, C^{n-1}G) \subset (G, G_{n-1}) \subset G_n.
$$

#### 命题 5 {#lie-ii-s4-prop-5 .statement tag=0A4R}

令 G 为群，gr(G) 为与 G 上的较低中心过滤相关的分级李$\mathbf{Z}$-代数。然后 gr(G) 由 $\mathrm{gr}_1(G) = G/(G, G)$ 生成。

令L为$\mathrm{gr}_1(G)$生成的gr(G)的谎言子代数；我们证明，$L \supset \mathrm{gr}_n(G)$乘以归纳在n上，断言对于$n = 1$来说是微不足道的。假设$n > 1$和$L \supset \mathrm{gr}_{n-1}(G)$。由于 gr(G) 上 $C^nG = (G, C^{n-1}G)$、构造的李代数律立即表明

$$
\mathrm{gr}_n(G) = [\mathrm{gr}_1(G), \mathrm{gr}_{n-1}(G)] \subset L.
$$

上述证明表明李代数gr(G) (§ 2, no. 7)的下中心级数由下式给出

$$
\mathscr{C}^n(\mathrm{gr}(G)) = \sum_{m \geq n} \mathrm{gr}_m(G).
$$

#### 注 {#lie-ii-s4-n6-rem-1 .statement tag=0A4S}

令 k 为 n 行的下三角矩阵的环、n 整数 $> 0$ 和 A 集合，k 中有 n 个列和元素。对于$p \geq 0$，令$A_p$为$(x_{ij}) \in A$的集合，使得$x_{ij} = 0$对应于$i - j < p$。然后是$A_0 = A$和$A_pA_q \subset A_{p+q}$。让$\Gamma_p = 1 + A_p$。那么$\Gamma_1$是$\mathbf{GL}(n, k)$的子群，称为阶n在k上的严格下三角群。通过no. 5的命题2，$(\Gamma_p)$是$\Gamma_1$上的积分过滤。作为 $\Gamma_n = \{1\}$，我们看到群 $\Gamma_1$ 是幂零的（代数、章 I, § 6, no. 3、定义 6）。

### 习题{#lie-ii-s4-exercises}

在下面的习题中，字母G表示群。

参见[习题为 § 4](exercises/s4/)。
