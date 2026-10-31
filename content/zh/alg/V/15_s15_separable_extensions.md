---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 15
section_title: Separable extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.118-A V.126, A V.175-A V.177
pdf_pages: 0232-0240, 0289-0291
extraction: ocr
subsections:
    - "no": 1
      title: Characterization of the nilpotent elements of a ring
      page: 118
      pdf_page: 232
    - "no": 2
      title: Separable algebras
      page: 119
      pdf_page: 233
    - "no": 3
      title: Separable extensions
      page: 121
      pdf_page: 235
    - "no": 4
      title: Mac Lane's separability criterion
      page: 122
      pdf_page: 236
    - "no": 5
      title: Extensions of a perfect field
      page: 125
      pdf_page: 239
    - "no": 6
      title: The characterization of separability by automorphisms
      page: 125
      pdf_page: 239
statements: 21
exercises: 12
content_sha256: 82ba89ae04b84486987448db33aa384dbfd39bda05cac5844e51a1dd4722cd16
translated_from: content/en/alg/V/15_s15_separable_extensions.md
translation_method: google
source_content_sha256: 29004e5cd09fd460bf5167f0e6481b43d3d6e1b88934fe63c99d9a4a216f82d7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: ee9763ac3dc439168ec40abcf71fab60ea763ae9a3ca7c05101207eafcd4bd43
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 15。 可分扩张

### 1. 环幂零元刻画

#### 命题 1 {#alg-v-s15-prop-1 .statement tag=06TN}

— *设 A 为 A 的交换环且 x 元素。要使 x 幂零，$1 - xT$ 在环 $A[T]$ 中可逆是充分必要的。*

我们注，$A[T]$是形式幂级数环$A[[T]]$的子环，并且$1 - xT$在$A[[T]]$中有逆$\sum_{n=0}^{\infty} x^n T^n$（IV，p. 30，提案 5）。要使 $1 - xT$ 在 $A[T]$ 中可逆，$\sum_{n=0}^{\infty} x^n T^n$ 是多项式是必要且充分的，即 x 是幂零的。

#### 命题 2 {#alg-v-s15-prop-2 .statement tag=06TO}

— *令 A 为交换环。 A 的幂零元的集合是 A 的理想，等于 A 的所有素理想中集合的交。*

令x为A的幂零元，p为A的素理想。$x \mod p$的剩余类类是整环$A/p$的幂零元，因此是零；因此我们有$x \in p$。

令 x 为 A 的非幂零元素。根据命题 1，$A[T]$ 的主要理想$(1 - xT)$ 与$A[T]$ 不同。根据克鲁尔的定理（I，p. 104），存在最大理想m为$A[T]$包含$1 - xT$。那么 m 是 $A[T]$ 的素理想，因此 $p = A \cap m$ 是 A 的素理想。我们有 $1 \notin m$ 和 $1 - Tx \in m$，因此有 $Tx \notin m$ 和 *更不必说* $x \notin p$。

由此我们证明，A 的幂零元的集合 $\mathfrak{n}$ 是 A 的所有素理想的集合的交；因为每一个交都是一个理想，所以$\mathfrak{n}$也是一个理想。

#### 推论{#alg-v-s15-n1-cor-1 .statement tag=06TP}

— *要减少交换环* (*V*, p. 34, Def. 2) *它同构于域* 的乘积子环是必要且充分的。

条件显然就足够了。

让$\mathbf{A}$减少。根据命题2，$\mathbf{A}$的素理想集合的交$n$减少到0。对于$\mathbf{A}$的每个素理想$\mathfrak{p}$，令$k(\mathfrak{p})$为$\mathbf{A}/\mathfrak{p}$的分数域并且将$\mathbf{A}$的$\varphi_n$典范同态转换为$k(\mathfrak{p})$。设$\varphi$是$\mathbf{A}$的同态进入$\prod_{\mathfrak{p}} k(\mathfrak{p})$，指标$\mathfrak{p}$的分量是$\varphi_{\mathfrak{p}}$。 $\varphi_{\mathfrak{p}}$的核是$\mathfrak{p}$，因此$\varphi$的$n = 0$；因此$\varphi$是$\mathbf{A}$的同构到$\prod_{\mathfrak{p}} k(\mathfrak{p})$的子环。

### 2.可分离代数

#### 定义 1 {#alg-v-s15-def-1 .statement tag=06TQ}

*令 $\mathbf{A}$ 为交换代数超过域 $K$。 Then $A$ is said to be separable over $K$, or also a separable $K$-algebra if the ring $L \otimes_K \mathbf{A}$ is reduced for every extension $L$ of $K$*.

每个可分离的代数都明显减少了。对于部分逆命题，请参阅 Th。 3（*V*，p. 125）。

#### 例 {#alg-v-s15-n2-exa-1 .statement tag=0DI7}

*1*) 设 $\mathbf{A}$ 为多项式代数 $K[X_i]_{i \in I}$。对于 $K$ 环 $L \otimes_K \mathbf{A}$ 的每个扩张 $L$ 都同构于 $L[X_i]_{i \in I}$ (III, p. 449, 注 2)，因此是整环 (*IV*, p. 9，提案 8）。在其他字中，域$K$上的每个多项式代数都是可分离的$K$代数。

2) 设$\mathbf{A}$为有限次数除域$K$的交换代数。要使 $\mathbf{A}$ 可分离，它必须是 etale (*V*, p. 34, Th. 4)。

3) 令$E$为域$K$的代数扩张。如果$L$是$K$的扩张，则环$L \otimes_K E$是子环$L \otimes_K F$的并，其中$F$的范围超过有限次数的所有子分机的集合 $E$；因此，当且仅当对于 $E$ 的每个子扩展 $F$、有限次数超过 $K$ 的$L \otimes_K F$ 都成立时，环 $L \otimes_K E$ 才会减少。考虑到例 2，我们发现 $E$ 在上述 Def 的意义上是一个可分离的代数。 1 当且仅当它是 Def 意义上的可分离代数扩张 。 1 个 *V*、p. 36。

#### 命题 3 {#alg-v-s15-prop-3 .statement tag=06TR}

*令$K$为域*。

a) *可分 $K$ 代数的每个子代数都是可分的*。

b) *可分 $K$-代数的每个直极限都是可分的*。

c) *可分 $K$-代数的每个乘积都是可分的*。

d) *设$\mathbf{A}$为$K$代数，且$K'$扩张为$K$。为了使 $\mathbf{A}$ 可分离，从 $\mathbf{A}$ 通过扩张标量获得的 $K'$-代数 $\mathbf{A}_{(K')}$ 是可分离的*。

设$L$为$K$中的扩张。设$\mathbf{A}$是$K$和$B$子代数上的可分代数和$\mathbf{A}$；那么环$L \otimes_K \mathbf{A}$被约化，$L \otimes_K B$与$L \otimes_K \mathbf{A}$的子环同构，因此被约约。因此$B$是可分的并且*a)*被证明。 *以同样的方式可以证明$b$），使用$L \otimes_K \varprojlim A_i$的典范同构和$\varprojlim L \otimes_K A_i$（II，p. 290，命题7）和$c$）可以通过指出$L \otimes_K \left( \prod_{i \in I} A_i \right)$同构来证明子环 / $\prod_{i \in I} (L \otimes_K A_i)$（II、p. 306、提案 15）。

我们将使用$d$的记号）。对于 $K'$ 环 $L' \otimes_{K'} A_{(K')}$ 和 $L' \otimes_K A$ 中的每个扩张 $L'$ 都是同构的（II、p. 278，命题 2）。我们结论如果$A$是可分离的$K$代数，那么$A_{(K')}$是可分离的$K'$代数。相反，假设 $A_{(K')}$ 是可分离的 $K'$-代数；前面的注表明，对于$K$包含$K'$的每一个扩张$L'$作为子扩展，$L' \otimes_K A$都会减少。设$L$为$K$中的扩张；由 Scholium (V, p. 13) 存在 $K$ 包含 $K'$ 的扩张 $L'$ 作为子扩展，以及 $L$ 到 $L'$ 的$K$同态；因此，环$L \otimes_K A$同构于$L' \otimes_K A$的子环，因此被约简。这证明$A$是可分离的$K$代数。

#### 命题 4 {#alg-v-s15-prop-4 .statement tag=06TS}

— *令$A$为域$K$上可分离的代数，令$B$为$A$的分数之和环；那么 $K$-代数 $B$ 是可分的。*

令$S$为$A$的可取消元素的集合。我们已经确定了$A$与$B$的子环（I，p. 113）；此外，$S$的每个元素在$B$中都是可逆的，并且$B$的每个元素都有形式$a s^{-1}$以及$a \in A$和$s \in S$。令$L$为$K$的扩张和$x$幂零元为$L \otimes_K B$。那么$x$可以写成形式
$$
x = \sum_{i=1}^n y_i \otimes a_i s_i^{-1}
$$
$y_i \in L, a_i \in A, s_i \in S$ 为 $1 \leq i \leq n$。如果我们把 $s = s_1 \ldots s_n$
然后$x(1 \otimes s)$属于到子环$L \otimes_K A$共$L \otimes_K B$；因为$x(1 \otimes s)$是幂零的并且$A$可以在$K$上分离，所以我们有$x(1 \otimes s) = 0$，并且由于$s$在$B$中是可逆的，我们发现$x = 0$。这证明环$L \otimes_K B$减少了，从而命题。

#### 命题 5 {#alg-v-s15-prop-5 .statement tag=06TT}

— *令$K$为域且$A, B$可交换$K$-代数。如果 $A$ 减少且 $B$ 可分离，则 $A \otimes_K B$ 减少。*

由科。命题 2 (V, p. 119) $A$ 同构于乘积 $\prod_{i \in I} L_i$ 的子代数，其中 $L_i$ 是 $i \in I$ 的 $K$ 扩张。因此，$A \otimes_K B$同构于$\left( \prod_{i \in I} L_i \right) \otimes_K B$的子环，后者环同构于$\prod_{i \in I} (L_i \otimes_K B)$的子环（II，p. 306，命题15）。由于$B$是可分离的，所以环$L_i \otimes_K B$都被减少，因此$\prod_{i \in I} (L_i \otimes_K B)$也是如此，$A \otimes_K B$的*更不必说*也是如此。

#### 推论 1 {#alg-v-s15-prop-5-cor-1 .statement tag=06TU}

— *令$K$为域、$K$的$L$可分扩张以及$f$$K[X]$的多项式。如果$f$在$K[X]$中没有倍数因子，那么在$L[X]$中也没有倍数因子。*

如果$f$在$K[X]$中没有倍数因子，则减少商环$K[X]/(f)$；因为$f$是不可约多项式$f_i$在对互质的乘积，因此

K[X]/(f) 是同构的，根据 I、p. 110、第 9 条，到域 K[X]/(f_i) 的乘积。根据命题 5 环 L[X]/(f)，与 L ⊗_KK[X]/(f ) 同构，被约简；如果 g 是 L[X] 的非常数多项式，使得 g^2 除 f，则 L[X]/(f) 中 fg^{-1} 的剩余类类是非零幂零元；因此 f 在 L[X] 中没有倍数因子。

#### 推论 2 {#alg-v-s15-prop-5-cor-2 .statement tag=06TV}

— 令 A 和 B 为两个交换K-代数。 *如果* A 和 B 是可分离的，则 A ⊗_K B 也是如此。

令 L 为 K 的扩张。 环 L ⊗_K A 被约简，因为 A 是可分的；现在，第 5 条命题表明环 (L ⊗_K A) ⊗_KB （与 L ⊗_K (A ⊗_KB) 同构的）要约简，从而是推论。

### 3.可分扩张

令 K 为域。由于 K 的任意扩张都是 K-代数，所以 Def. 中引入了概念的可分离性。 1 (V, p. 119) 特别适用于 K 的扩张的情况。通过例 3 (V, p. 119)，在代数扩张的情况下，定义的可分性与 § 7 的可分性一致（V、p. 36、默认 1）。

#### 命题 6 {#alg-v-s15-prop-6 .statement tag=06TW}

— *域* K 的每个纯扩张都是可分的。
这立即源自例 1 (V, p. 119) 和提案 4 (V, p. 120)。

#### 命题 7 {#alg-v-s15-prop-7 .statement tag=06TX}

— 令 E 为 E 的 *自同构* 的域、G 群，K 为 G 的不变量的 E 由……组成的 *子域*。则 E 为 K 的可分扩张。

设L为K的扩张；存在L的代数闭扩张Ω，其对K的超越次数至少等于E对K的超越。 1 (V, p. 117) 存在 E 到 R 的 K 同态 u。我们用 v 表示 A = Ω ⊗_K E 到 Ω 的 Ω 代数同态，其中映射 λ ⊗ x 到 λ 。 u(x) 对于 λ ε Ω 且 x ε Ω；我们为 v 的核写一个。

对于每个 s ∈ G 令 h_s 为 0-代数 A 的自同构 Id, ⊗ s； A 的同态 v ∘ h_s 入 Ω 的核为 A 的素理想 a_s = h_s^{-1}(a)。显然，A 的理想 b = ⋂_{s ∈ G} a_s 在自同构 h_s 下是稳定的。因此 (V, p. 63, Cor.) 理想 b 为形式 c ⊗_K E，其中 c 是 Ω 的理想值。现在 b ⊂ a ≠ A，因此 c ≠ Ω；由于 Ω 为域，因此 c = 0，因此 b = 0。

A 的素理想族 (a_s), _s ∈ G 因此有零交。根据命题 2 (V, p. 118) 环被约简，更不必说同样适用于 A 的子环 L ⊗_K E。由于 L 是 K 的任意扩张，这证明 E 与 K 是可分的。

#### 命题 8 {#alg-v-s15-prop-8 .statement tag=06TY}

— 令 L 为域 K 的扩张。如果 L 在 K 上可分，则 L 的每个子外延在 K 上可分。反之，如果 L 的每个有限生成子外延在 K 上可分，则 L 在 K 上可分。

这立即从第 3 条命题 a) 和 b) (V, p. 119) 中得出。

因此可分性可以称为“有限特征标”的性质。

#### 命题 9 {#alg-v-s15-prop-9 .statement tag=06TZ}

— 令 L 为域 K 的扩张，M 为可交换的 L 代数（对于例、扩张 L）。如果 M 在 L 上可分且 L 在 K 上可分，则 M 在 K 上可分。

令K'为K的扩张。由于L是K的可分扩张，因此减少环$K' \otimes_K L$；由于 M 是可分离的 L 代数，因此命题 5 (V, p. 120) 表明环 $(K' \otimes_K L) \otimes_L M$ 要约简。现在环$K' \otimes_K M$同构于$(K' \otimes_K L) \otimes_L M$（II，p. 278，命题2），因此被约简。这证明M对于K是可分的。

如果扩张 M 在 K 上可分，则它不一定在 L 上可分（cf. 然而 V、p. 124，Cor. 3）。对于例，如果 p 是素数数，则有理分式的域 $F_p(X)$ 在 $F_p$ 上的一个不定X 上可在 $F_p$ 上分离（V、p. 121，命题 6），但它是$F_p(X^p)$ 的 p 根代数扩张；特别是$F_p(X)$在$F_p(X^p)$上是不可分的。

稍后（V，p. 137命题5）我们将研究复合扩张的可分性。

### 4.Mac Lane 的可分离性准则

#### 定理 1 {#alg-v-s15-thm-1 .statement tag=06U0}

— 令 K 为特征 0 的域。K 的每个约化K-代数，尤其是每个扩张都可在 K 上分离。

我们首先证明 K 的每个扩张 L 都是可分的。令 B 为 L 对 K (V, p. 109, Th. 1) 的超越基，并令$L_1 = K(B)$。那么 $L_1$ 在 K 上是可分的（V，p. 121，命题 6）。进一步地，L是$L_1$的代数扩张，$L_1$是特征0的域；因此 L 可以在 $L_1$ 上分离（V，p. 37，Cor.）。因此，根据命题 9，L 在 K 上是可分的。

现在让 A 成为域 K 的约化代数。根据命题 2 (V, p. 119)，存在 K 的$(L_i)_{i \in I}$族扩张，使得 A 同构于$\prod_{i \in I} L_i$的子代数。 代数 $L_i$ 中的每一个都可以按照前面所说的在 K 上分离，因此根据命题 3 a) 和 c)，A 具有相同的性质（V，p. 119）。

#### 定理 2 {#alg-v-s15-thm-2 .statement tag=06U1}

— 令 K 为特征 $p \neq 0$ 的域，$K^{p^{-\infty}}$ K 和 A 交换K-代数的完美闭包。以下属性是等效的：
a) A 是可分离的。
b) 存在 K 的扩张 K'，使得 K' 是完美的且$K' \otimes_K A$ 被约化。
c) 环 $K^{p^{-\infty}} \otimes_K A$ 减少。

d) *环* $K' \otimes_K A$ *每扩张* $K'$ *减少* $K$ *即有限次数和* $p$*-高度* $\leqslant 1$的根数。

e) *对于每个家庭* $(a_i)_{i \in I}$，*元素的* $A$ *线性自由超过* $K$，*族* $(a_i^p)_{i \in I}$，*线性自由超过* $K$。

f) *存在基* $(a_i)_{i \in I}$，*向量* $K$*-空间* $A$ *吸该族* $(a_i^p)_{i \in I}$，*在* $K$ 上线性自由。

如果$K$的扩张$K'$是完美域，则包含是$K$同构于$K^{p^{-\infty}}$的子扩展（$V$，p. 6，命题3）；此外，$K$的每个$p$根式扩展都同构于$K^{p^{-\infty}}$的子扩展（$V$，p. 26，命题3）。这些注显示了$a) \Rightarrow b) \Rightarrow c) \Rightarrow d)$的含义。

让我们证明 d) 蕴涵 e)。令$(a_i)_{i \in I}$为$A$中的线性自由族，并令$(A_i)_{i \in I}$为$K$中有限支撑的族，使得$\sum \lambda_i a_i^p = 0$。设$K'$为元素$\lambda_i^{p^{-1}}$生成的$K^{p^{-\infty}}$的子扩展；它的尺寸为有限次数，高度为$\leqslant 1$。将$x = \sum_{i \in I} \lambda_i^{p^{-1}} \otimes a_i$放入$K' \otimes_K A$；我们有

$$
x^p = \sum_{i \in I} \lambda_i \otimes a_i^p = 1 \otimes \sum_{i \in I} \lambda_i a_i^p = 0
$$

到假设 d)，我们对所有 $i \in I$ 都有 $x = 0$、从而 $A_i = 0$。

显然，e) 蕴涵 f)，并且还需要证明 f) 蕴含 a)。因此，令$(a_i)_{i \in I}$为$A$在$K$上的基，使得族$(a_i^p)_{i \in I}$在$K$上线性自由。令$L$为$K$的扩张，并令$x$为$L \otimes_K A$的元素，使得$x^p = 0$。将所有 $i \in I$ 写为 $x = \sum_{i \in I} \lambda_i \otimes a_i$ 和 $A_i \in L$。我们有$x^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p = 0$，并且由于家庭$(a_i^p)_{i \in I}$在$K$上是线性自由的，所以我们对所有$i \in I$有$\lambda_i^p = 0$，从而$\lambda_i = 0$；由此可见$x = 0$。这样我们就证明了$x^p = 0$在$L \otimes_K A$中隐含了$x = 0$，由此可以立即得出$L \otimes_K A$的约简。

#### 推论 1（Mac Lane）{#alg-v-s15-thm-2-cor-1 .statement tag=06U2}

— *Let* $K$ *be a field of characteristic exponent* $p$, $\Omega$ *a perfect extension of* $K$ *and* $L$ *a subextension of* $\Omega$. *那么以下条件是等价的*：

a) $L$ *可在* $K$ 上分离。

b) $L$ *从* $K^{p^{-\infty}}$ *经过* $K$ 线性地不相交的。

c) $L$ *线性不相交的超过* $K$ *从每个* $p$*-* $K$ *包含在* $\Omega$，*有限次数和高度* $\leqslant 1$ 中。

$K$ 的特征为 0 的情况是微不足道的，因为按照惯例，$L$ 可在 $K$ (Th.1) 和 $K^{p^{-\infty}} = K$ 上分离。假设$p \neq 1$，让我们首先证明a）蕴涵b）。假设$L$在$K$上可分，并且令$(a_i)_{i \in I}$是$L$在$K$上的基。令$(\lambda_i)_{i \in I}$是$K^{p^{-\infty}}$的元素的有限支撑的族，使得$\sum_{i \in I} \lambda_i a_i = 0$；存在 K 的整数 $f \geqslant 0$ 和元素 μ_i，使得 λ_i = μ_i^{p^{-f}}。我们有

$$
\sum_{i \in I} \mu_i a_i^{p^f} = \left( \sum_{i \in I} \lambda_i a_i \right)^{p^f} = 0
$$

和Th。 2 意味着，通过 f 上的归纳，族 $(a_i^{p^f})_{i \in I}$ 在 K 上是线性自由的。因此，对于所有 $i \in I$，我们有 $\mu_i = 0$、从而 $\lambda_i = 0$。最后L是从$K^{p^{-\infty}}$在K上线性不相交的。

很明显，b) 暗示了 c)。最后假设c)成立，令K'为有限次数的K的扩张和高度为$\leq 1$的p根。 环 $K' \otimes_K L$ 与 $\Omega$ 的子环同构，因此被约化。现在它是从 Th 开始的。 2 L 在 K 上可分。

#### 推论 2 {#alg-v-s15-thm-2-cor-2 .statement tag=06U3}

— *令K为特征指数p的域，K的完美闭包$K^{p^{-\infty}}$和K的L可分扩张。则环$L \otimes_K K^{p^{-\infty}}$为域。此外，如果L是K上的代数，那么$L \otimes_K K^{p^{-\infty}}$是L的完美闭包。*

案例 $p = 1$ 很简单，所以让我们假设 $p \neq 1$。令$\Omega$成为L的完美闭合。由科. 1 存在$L \otimes_K K^{p^{-\infty}}$到$L[K^{p^{-\infty}}]$的K-代数同态，其中$x \in L$和$y \in K^{p^{-\infty}}$有映射$x \otimes y$到$xy$。由于$K^{p^{-\infty}}$是K上的代数，环$L[K^{p^{-\infty}}]$是$\Omega$的子域（V，p. 18，Cor.1）。进一步假设L是K上的代数，则$L[K^p]$是完美域$K^{p^{-\infty}}$的代数扩张，因此是完美域（V，p. 43，Cor.1）；最后，由于域$L[K^{p^{-\infty}}]$是L的近似扩展（V，p. 25，Cor.），它是L的完美闭包。

#### 推论 3 {#alg-v-s15-thm-2-cor-3 .statement tag=06U4}

— *令 L 为 K 的代数扩张，M 为可交换的 L-代数（对于 L 的例扩张）。如果 M 在 K 上可分，则它在 L 上可分。*

代数 L 与 M 的子代数 K 同构的，因此 L 是 K 的可分扩张。因此（Cor. 2）存在 $L^{p^{-\infty}}$ 到 $K^{p^{-\infty}} \otimes_K L$ 的 L 同构的。因此，环$L^{p^{-\infty}} \otimes_L M$同构于$(K^{p^{-\infty}} \otimes_K L) \otimes_L M$，也同构于$K^{p^{-\infty}} \otimes_K M$（II，p. 278，命题2），并且后者环被约化，因为M可与K分离。因此环 $L^{p^{-\infty}} \otimes_L M$ 被约简，证明 M 在 L (V, p. 122, Th. 2) 上是可分的。

#### 注 {#alg-v-s15-n4-rem-1 .statement tag=06U5}

— Mac Lane 准则可以在不引入除 L 之外的任何 K 扩张的情况下制定。对于 Cor 的 c) 而言。 1、L在K上可分当且仅当L和$K^P$在K上线性不相交的。由于映射$x \mapsto x^p$是L的同构到子域$L^P$，我们得到以下准则（cf. V、p. 177，Ex. 11 用于代数的类似标准）：

*L在K上可分离当且仅当子域$L^P$和L的K在$K^P$上线性不相交的。*

### 5. 扩张 / 完美域

为了便于参考，我们总结了扩张和完美域的主要属性：

#### 定理 3 {#alg-v-s15-thm-3 .statement tag=06U6}

— 令 K 为完美域。
a) K 的每个代数扩张都是完美域。
b) K 的每个扩张都是可分的。
c) 为了使K-代数可分离，减少它是必要且充分的。
d) 令 A 和 B 为 2 约简 K-代数。那么$A \otimes_K B$就减少了。
e) 如果 E 和 F 是 K 的两个扩张，则环 $E \otimes_K F$ 会减少。

断言 a) 就是 Cor。第 11 号提案第 1 条（V、p. 43）。
断言 b) 由 Th 推出。 1 (V, p. 122) 当 K 的特征为 0 且来自 Cor 时。当 K 具有特征 $p \neq 0$ 时，1 (V, p. 123)。
让我们证明c）。 K 的特性为 0 的情况由 Th 得出。 1（V，p. 122）。因此，只要证明 K 是特征 $p \neq 0$ 的完美且 A 是约化的 K-代数，则 A 与 K 是可分的。 但这是从 Th 的条件 a) 和 b) 的等价得出的。 2（V，p. 122；取b）中的$K' = K$）。
最后，d) 由 c) 和命题 5 (V，p. 120) 得出，而 e) 是 d) 的一个特例。

### 6. 刻画与自同构的可分离性

#### 定理 4 {#alg-v-s15-thm-4 .statement tag=06U7}

— 令 $\Omega$ 为域 K 的代数闭扩张，且L $\Omega$ 的子扩展。那么下面的条件是等价的：
a) L 在 K 上可分。
b) $\Omega \otimes_K L$到$\Omega$的0代数同态的核的交减少到0。
c) 对于 L 的任何元素 $a_1, \ldots, a_n$ 与 K 线性无关，存在 $\Omega$ 的 K 自同构 $\sigma_1, \ldots, \sigma_n$，使得 $\det(\sigma_i(a_j)) \neq 0$。
d) 设V为有限维的L的向量子K空间。 V到$\Omega$的每个K-线性映射都是$\Omega$的K自同构的限制到V的线性组合（系数在R中）。

$d) \Rightarrow c)$：令$a_1, \ldots, a_n$为L的元素，与K线性无关，并令V为由$a_1, \ldots, a_n$生成的L的向量子K空间。 映射 $f \mapsto (f(a_1), \ldots, f(a_n))$ 是 $\mathrm{Hom}_K(V, R)$ 到 $\Omega^n$ 的 R 线性双射。假设 d) 成立，则存在 $\Omega$ 的 K-自同构 $a_1, \ldots, a_n$，使得 $\Omega^n$ 的元素 $(\sigma_i(a_1), \ldots, \sigma_i(a_n))$（对于 $1 \leq i \leq n$）形式基 $\Omega^n$。因此我们有 $\det(\sigma_i(a_j)) \neq 0$，因此 d) 蕴含 c)。

c) $\Rightarrow$ b)：假设c)成立且令x在$\Omega \otimes_K L$中。我们将 x 写在形式 $\sum_{j=1}^n x_j \otimes a_j$ 中，$x_1, \ldots, x_n$ 写在 $\Omega$ 中，L 的元素 $a_1, \ldots, a_n$ 与 K 线性无关。选择 K-自同构 $\sigma_1, \ldots, \sigma_n$ $\Omega$ 使得$\det \sigma_i(a_j) \neq 0$；令$\chi_1, \ldots, \chi_n$为$\Omega \otimes_K L$到$\Omega$的R同态，使得$\chi_i(a \otimes b) = a \cdot \sigma_i(b)$对应于$a \in \Omega$和$b \in L$。假设$\chi_i(x) = 0$对应$1 \leq i \leq n$，在其他字中，$\sum_{j=1}^n x_j \cdot \sigma_i(a_j) = 0$对应$1 \leq i \leq n$。由于我们假设矩阵 $(\sigma_i(a_j))$ 具有非零行列式，因此我们有 $x_i = 0$ 对应于 $1 \leq i \leq n$ 以及$x = 0$。

b) $\Rightarrow$ a)：由于特征0的域的每个扩张都是可分离的（V，p. 122，Th.1），因此足以检查K具有特征$p \neq 0$的情况。令X为$\Omega \otimes_K L$的所有R-代数同态到$\Omega$的集合，以及$\Omega \otimes_K L$的f同态到由$f(u) = (\chi(u))_{\chi \in X}$为$u \in \Omega \otimes_K L$定义的$\Omega^X$。 条件 b) 意味着 f 是单射的，因此意味着环 $\Omega \otimes_K L$ 被约化。因此 Th 的条件 b)。 2 (V, p. 122) 满足$K' = \Omega$，因此L 在 K 上可分。

a) $\Rightarrow$ d): 假设L在K上可分。令V为L的有限维的向量子K空间，$V_{(\Omega)} = \Omega \otimes_K V$向量$\Omega$空间衍生自V乘以标量的扩张，并在$V_{(\Omega)}$上乘以$f_0$线性形式，使得$f_0(x \otimes y) = xy$等于$x \in \Omega, y \in V$。用 $\Omega$ 的 K-自同构的 G 群表示；对于$\sigma \in G$，我们放置$\sigma_V = \sigma \otimes \mathrm{Id}_V$和$g_\sigma = \sigma \circ f_0 \circ \sigma_V^{-1}$。

对于$V_{(\Omega)}$到$\Omega$的每个$\sigma \in G$映射$g_\sigma$都是$\Omega$线性，映射$x \otimes y$到$x \cdot \sigma(y)$对于$x \in \Omega, y \in V$。因此，$g_\sigma$的核$N_\sigma$是$V_{(\Omega)}$的向量子空间，$N = \cap_{\sigma \in G} N_\sigma$也是如此。如果p是K的特征指数，则$\Omega$中G的不变量域等于$K^{p^{-\infty}}$（V，p. 112，命题10）。显然，我们对所有 $\sigma \in G$ 都有 $\sigma_V(N) = N$；因此（V，p. 63，Cor.）向量$\Omega$-空间N由$N_0 = N \cap (K^{p^{-\infty}} \otimes V)$生成。由于L在K上可分离，域$K^{p^{-\infty}}$和L在K上线性不相交的（V，p. 123，Cor.1）；我们有 $K^{p^{-\infty}} \otimes_K V \subset K^{p^{-\infty}} \otimes_K L$ 和 $f_0(x \otimes y) = xy$ 对应 $x \in \Omega$ 和 $y \in V$。由此可见，$f_0$到$K^{p^{-\infty}} \otimes_K V$的限制是单射的。现在$f_0 = g_1$在N上是零，在$N_0 \subset K^{p^{-\infty}} \otimes_K V$上是更不必说。因此我们有 $N_0 = 0$、从而 $N = 0$。由于V在K上是有限维，所以$V_{(\Omega)}$在$\Omega$上是有限维； 线性形式$g_\sigma$核交是零，因此(II，p. 301，Th.7)族$(g_\sigma)_{\sigma \in G}$生成$V_{(\Omega)}$的对偶。现在让$u$是V的K-线性映射变成$\Omega$；让$\tilde{u}$在$V_{(\Omega)}$上成为线性形式，其中映射$x \otimes y$到$xu(y)$对于$x \in \Omega$和$y \in V$。如上所述，存在G的元素$\sigma_1, \ldots, \sigma_n$和$\Omega$的$\lambda_1, \ldots, \lambda_n$，使得对于所有$y \in V$，$\tilde{u} = \sum_{i=1}^n \lambda_i g_{\sigma_i}$，从而$u(y) = \sum_{i=1}^n \lambda_i \sigma_i(y)$。所以我们已经证明a) 蕴涵d)。

### 习题{#alg-v-s15-exercises}

§ 15](exercises/s15/)参见[习题。
