---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 7
section_title: Approximation theorem
lang: zh
source: ac-i-vii
book_pages: 412-416, 460-461
pdf_pages: 0430-0434, 0478-0479
extraction: ocr
subsections:
    - "no": 1
      title: THE INTERSECTION OF A FINITE NUMBER OF VALUATION RINGS
      page: 412
      pdf_page: 430
    - "no": 2
      title: INDEPENDENT VALUATIONS
      page: 413
      pdf_page: 431
    - "no": 3
      title: THE CASE OF ABSOLUTE VALUES
      page: 415
      pdf_page: 433
statements: 14
exercises: 3
content_sha256: 8c4efeec5d4a065d2208a895a445bba34c4201788d04aff38f6afb496db3dde5
translated_from: content/en/ac/VI/07_s7_approximation_theorem.md
translation_method: google
source_content_sha256: b2cb895d1415aea075090da4a69834fe352e4f0135aedb112aadd7070f320371
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 160b867de9826227e382f8c6bf999ca29ab09ef410650cb48dab4676d66b659a
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 7. 近似值定理

### 1. 有限数估值环的交

#### 命题 1 {#ac-vi-s7-prop-1 .statement tag=04VN}

令$K$为域，$(\mathbf{A}_i)_{1 \leq i \leq n}$为$K$和$B = \bigcap_{i=1}^n \mathbf{A}_i$的估值环。我们写$p_i = B \cap m(\mathbf{A}_i)$。那么 $A_i = B_{p_i}$ 对于所有 $i$ 且 $B$ 的 jie 是 $K$。

显然$B_{p_i} \subset A_i$。为了证明逆命题包含，我们需要以下引理：

#### 引理 1 {#ac-vi-s7-lem-1 .statement tag=04VO}

令$v_i$ ($1 \leq i \leq n$) 为$K$ 和$x \in K^*$ 的评价。那么存在一个多项式 $(X)$ 形式

$$
f(X) = 1 + n_1 X + \cdots + n_{k-1} X^{k-1} + X^k \quad (k \geq 2,\ n_j \in \mathbf{Z} \text{ for } 1 \leq j \leq k - 1)
$$

这样$f(x) \neq 0$和元素$z = f(x)^{-1}$享有$1 \leq i \leq n$的以下属性：

$$
v_i(z) = 0 \qquad \text{if} \quad v_i(x) \geq 0 \\
v_i(z) + v_i(x) > 0 \qquad \text{if} \quad v_i(x) < 0.
$$

暂时假设引理，我们展示它如何暗示$A_1 \subset B_{p_1}$。令 $x$ 为 $A_i$ 的非零元素。我们将引理应用于$x$，并将$v_i$与$\mathbf{A}_i$相关联。然后$v_i(z) \geq 0$和$v_i(zx) \geq 0$对于所有$i$，因此$z \in B$和$zx \in B$。作为$v_1(x) \geq 0$，$v_1(z) = 0$，因此$z \notin p_1$。因此$x = zx/z \in B_{p_1}$。 域分数 $B$ 然后包含 $A_1$ 因此是$K$。

我们现在转到引理的证明。令$I$为指标$i$的集合，使得$v_i(x) \geq 0$。对于所有$i \in I$，让$\bar{x}_i$表示$\kappa(\mathbf{A}_i)$中$x$的典范像。对于所有$i \in I$，我们构造一个多项式，如下：如果存在形式(1)的多项式$g(X)$，使得$\kappa(\mathbf{A}_i)$中的$g(\bar{x}_i) = 0$，我们取，是这样一个多项式；否则我们取$f_i = 1$。然后我们写$f(X) = 1 + X^2 \prod_{i \in I} f_i(X)$。显然它是形式(1)的多项式。如果$i \in I$，则$f(x) \in A_i$，并且$(\bar{x}_i) \neq 0$乘以构造；因此$f(x) \notin m(\mathbf{A}_i)$、$v_i(f(x)) = 0$和$v(z) = 0$。如果$i \notin I$，则$v_i(x) < 0$，从而$v_i(f(x)) = kv_i(x)$（§ 3, no. 1，命题 1）并且

$$
v_i(x) + v_i(z) = (1 - k)v_i(x) > 0
$$

（自 $k \geq 2$ 起）。 从而引理。

#### 命题 2 {#ac-vi-s7-prop-2 .statement tag=04VP}

根据命题 1 的假设，进一步假设$\mathbf{A}_i \not\subset \mathbf{A}_j$ 对应$i \neq j$。那么$p_i$是$B$的不同最大理想，$B$的每个最大理想都等于$p_i$之一。

如果$p_i \subset p_j$代表$i \neq j$，则$\mathbf{A}_i = B_{p_i} \supset B_{p_j} = \mathbf{A}_j$。然后应用章II, § 3, no. 5就足够了，推论到命题17。

#### 推论 1 {#ac-vi-s7-prop-2-cor-1 .statement tag=04VQ}

假设 $A_i \not\subset A_j$ 对应 $i \neq j$。对于元素$a_i \in A_i$（$1 \leq i \leq n$）的每个家庭，都存在$x \in B$，使得$x \equiv a_i \pmod{m(A_i)}$对应于$1 \leq i \leq n$。

由于$p_i$是$B$、$A_i/m(A_i) = B_{p_i}/p_iB_{p_i} = B/p_i$的最大理想，因此可以假设$a_i \in B$对于所有$i$。由此得出的推论是，从 $B$ 到 $\prod_{i=1}^n (B/p_i)$ 的典范映射是满射（章 11、§ 1, no. 2、命题 5）。

#### 推论 2 {#ac-vi-s7-prop-2-cor-2 .statement tag=04VR}

假设 $A_i \not\subset A_j$ 对应 $i \neq j$。存在 $K$ 的元素 $x_i$ ($1 \leq i \leq n$)，使得 $v_i(x_i) = 0$ 和$v_j(x_i) > 0$ $i \neq j$。

对于每个指标$i$，将推论1应用于$(a_i)$族，使得$a_i = 1$和$a_j = 0$适用于$j \neq i$。

#### 推论 3 {#ac-vi-s7-prop-2-cor-3 .statement tag=04VS}

每估价环 $K$ 包含 $B$ 包含 $A_i$ 之一。

我们可以将注意力集中在$A_i \not\subset A_j$代表$i \# j$的情况。令$V$为$K$包含$B$的估值环。我们写
$$
p = m(V) \cap B.
$$
存在最大理想 $p_i$ $B$ 包含 $p$、从而
$$
A_i = B_{p_i} \subset B, \subset V.
$$

### 2. 独立估值

#### 定义 1 {#ac-vi-s7-def-1 .statement tag=04VT}

令$A$和$A'$为相同域$K$的两个估值环。如果$K$是由$A$和$A'$生成的环，则称$A$和$A'$是独立的。如果环是独立的，则$K$ 的两个估值称为独立的，否则称为独立的。

对 $K$ 的不正确估值独立于对 $K$ 的每个估值。为了使 $K$ 上的高度 1 的两个估值是独立的，它们不等价是充分必要的 (§ 4, no. 5, 命题 6 (c))。

#### 定理 1（估值的近似值定理）{#ac-vi-s7-thm-1 .statement tag=04VU}

令$v_i$ ($1 \leq i \leq n$) 为域 $K$ 的估值，它们在$v_i$ 的对和$\Gamma_i$ 阶群中是独立的。设 $a_i \in K$ 和 $\alpha_i \in \Gamma_i$ ($1 \leq i \leq n$)。那么存在$x \in K$使得$v_i(x - a_i) \geq \alpha_i$对于所有$i$

如果$v_i$不正确，则$a_i = 0$和关系$v_i(x - a_i) \geq a_i$对于所有$x \in K$都成立。因此我们可以假设$v_i$并无不当。

令$A_i$为$v_i$、$B = \bigcap_{i=1}^n A_i$和$p_i = m(A_i) \cap B$的环。到no. 1的命题 1，$a_i$可以写成$a_i = b_i/s$（$b_i \in B, s \in B - \{0\}$）；如果我们写$x = y/s$和$\alpha_i' = \alpha_i + v_i(s)$，那么$v_i(y - 6_i) \geq \alpha_i'$。这表明我们可以假设 $a_i \in B$ 对于所有$i$；我们也可以假设 $\alpha_i > 0$ 对于所有$i$。令$v_i$为$z \in \mathbf{K}$的集合，这样$v_i(z) \geq a$，我们写为$q_i = v_i \cap B$。对于$x \in B, v_i(x - a_i) \geq \alpha_i$相当于$x \equiv a_i (\mathfrak{q}_i)$。因此，我们需要证明典范同态 $B \to \prod_{i=1}^n (B/q_i)$ 是满射，即 $q_i + q_j = B$ 对应 $i \neq j$ (章 11, § 1, no. 2, 命题 5)。由于 B 的最大理想是 $\mathfrak{p}_i$ (命题 2)，因此只要证明 $q_i \notin \mathfrak{p}_j$ 对应 $i \neq j$ 就足够了。

假设存在$i, j$使得$q_i \subset \mathfrak{p}_j$和$i \neq j$。我们很快就会看到，$q_i$的根式是B的*素的*理想$p$。然后是$p \subset \mathfrak{p}_j$，还有$\alpha_i > 0$以来的$p \subset \mathfrak{p}_i$，因此是$q_i \subset \mathfrak{p}_i$。因此 $A_1 = B_s \subset B_p$ (no. 1, 命题 1) 以及类似的 $A_1 \subset B_r$。现在，为$v_i \neq (0)$和$v_i = B_{\mathfrak{p}_i} q_i$（章11、§ 2, no. 4、命题10）、$q_i \neq (0)$、从而、$p \neq (0)$和$B_r \neq K$。这个与……矛盾假设即$A_1$和$A_1$是独立的。

仍有待证明 $p$ 是质数。现在，这是从以下引理得出的：

#### 引理 2 {#ac-vi-s7-lem-2 .statement tag=04VV}

*设 A 为估值环，b 为 A 与 A 不同的理想。则 b 的根式 c 为素理想。*

假设$xy \in c$。那么存在$n \geq 1$使得$(xy)^n \in b$。令 $v$ 为与 A 相关的估值。如果对于例，$v(x) \geq v(y)$，则

$$
v(x^{2n}) \geq v(x^n y^n),
$$

从而$x^{2n} \in b$和$x \in c$。

#### 推论 1 {#ac-vi-s7-lem-2-cor-1 .statement tag=04VW}

*对于元素$\gamma_i \in \Gamma_i$（$1 \leq i \leq n$）的每个家庭，都存在$x \in K$使得$v_i(x) = \gamma_i$（$1 \leq i \leq n$）。

我们可以假设 $A_i \neq K$ 对于所有$i$。那么，对于所有$i$，都存在一个$a_i \in K$，这样$v_i(a_i) = \gamma_i$，并且存在一个$a_r \in \Gamma_r$，这样$\gamma_i < a_r$。我们应用定理 1 到这些元素 $a_i$：存在$x \in K$使得$v_i(x - a_i) > v_i(a_i)$； 从而，如$x = a_i + (x - a_i)$、$v_i(x) = v_i(a_i) = \gamma_i$（$§ 3$、no. 1、命题 1）。

#### 推论 2 {#ac-vi-s7-lem-2-cor-2 .statement tag=04VX}

*设$\mathscr{T}_i$为$v_i$在$K$上定义的拓扑；让$K^n$被赋予$\mathscr{T}_i$的拓扑乘积。如果$v_i$没有不当的话，$K^n$的对角线在$K^n$是密集的。

#### 命题 3 {#ac-vi-s7-prop-3 .statement tag=04VY}

*令$v$和$v'$为同一域$K$的两个非不当估值。对于$v$和$v'$到定义，$K$上的相同拓扑，它们依赖是必要且充分的。

假设由 $v$ 和 $v'$ 定义的拓扑 $\mathscr{T}_v$ 和 $\mathscr{T}_{v'}$ 是相同的。由于 $\mathscr{T}_v$ 是 Hausdorff，$K^2$ 的对角线是闭合的，因此 $v$ 和 $v'$ 是相关的（推论 2 到定理 1）。

相反，假设 $v$ 和 $v'$ 是相关的。那么它们的环$A$和$A'$包含在与$K$不同的相同环$A''$中，并且$A''$是评估$v''$的环（$§ 4$，no. 1， 命题1)。只要证明拓扑 $\mathscr{T}_{v''}$ 与 $\mathscr{T}_v$ 相同即可。设$\Gamma$和$\Gamma''$为$v$和$v''$的阶群。在$\Gamma''$上存在$\Gamma$的递增同态$\lambda$使得$v'' = A \circ v$($§ 4$,no. 3)。若$a'' \in I?''$，令$a \in \lambda^{-1}(a'')$； 条件 $v(x) \geq \alpha$ 意味着 $v''(x) \geq a''$。设$\beta \in \Gamma$和$\beta'' = \lambda(\beta)$； 条件$v(x) \leq \beta$意味着$v''(x) \leq \beta''$，因此条件$v''(x) > \beta''$意味着$v(x) > \beta$。由于$v$和$v''$并非不恰当，因此对于$\mathscr{T}_v$和$\mathscr{T}_{v''}$，邻域的定义基本系统为0。因此$\mathscr{T}_v = \mathscr{T}_{v''}$，它完成了证明。

注
(1) 命题 3 表明关系 '“$v$ 和 $v'$ 是相关的”' 是等价关系。
(2) 考虑到高度 1 的估价和超测量绝对值值 (§ 6, no. 2) 之间的关系，对于高度 1 的估价，命题 3 也可从等效绝对值值的刻画得出（一般拓扑、章） IX, § 3, no. 2、命题5)。

#### 命题 4 {#ac-vi-s7-prop-4 .statement tag=04VZ}

*让 $v_1, \ldots, v_n$ ($n \geq 2$) 成为对相同域 $K$ 的成对相关估值。那么 $v_1, \ldots, v_n$ 生成子环 $\delta \ K$ 的环 $A_1, \ldots, A_n$ 与 $K$ 不同。*

对于 $n = 2$ 命题 4，从定义 1 得出。假设它适用于 $n - 1$ 估值。则存在不同于 K 的 K 的子环 A 和包含 $A_1, \ldots, A_{n-1}$；还存在子环 B $\neq K$ 包含于 $A_{n-1}$ 和 $A_n$。由于 A 和 B 包含于 $A_{n-1}$，它们在包含方面具有可比性（§ 4, no. 1，命题 1 的推论）。因此，这两者中较大的一个为包含所有 $A_i$。

### 3.绝对值的情况

#### 定理 2（绝对值值的近似值定理）{#ac-vi-s7-thm-2 .statement tag=04W0}

*令 $f_i$ ($1 \leq i \leq n$) 为绝对值，且与域 $K$ 相同，这不是不恰当的，并且没有两个是等价的。设$a_i \ (1 \leq i \leq n)$为$K$和$\varepsilon$实数$> 0$的元素。那么存在 $x \in K$ 使得 $f_i(x - a_i) \leq \varepsilon$ 对于所有 $i$。*

让$K_i$表示域K，拓扑由$f_i$定义。待证明的结果等价于：在乘积$P = K_1 \times \cdots \times K_n$中，对角线D的闭包$\overline{D}$等于P。这对于$n = 1$来说是显而易见的。假设在$k < n$有k绝对值的情况下，这个点已经成立。

我们首先证明，对于$2 \leq h \leq n$，K 存在元素 $x_h$，使得$f_1(x_h) < 1, f_2(x_h) > 1$ 和$f_i(x_h) \neq 1$ 对于$3 \leq i \leq h$。我们在归纳在$h$争论。如果$h = 2$，这是因为$f_1$和$f_2$不等价。因此我们假设$x_{h-1}$的存在性已被证明，并证明$x_h$的存在性。如果$f_h(x_{h-1}) \neq 1$，我们可以取$x_h = x_{h-1}$；如果$f_h(x_{h-1}) = 1$，我们选择$z \in K^*$，这样$f_h(z) \neq 1$和$x_h = z(x_{h-1})^s$可以解决问题的s足够大。这样我们就证明了$x_h$的存在。

由于整数$q$趋于无穷大，$f_1(x_n^q)$趋于0，$f_2(x_n^q)$趋于$+\infty$，$f_i(x_n^q)$趋向于0或$+\infty$（对于$i \geq 3$）。写$y_q = x_n^q(1 + x_n^q)^{-1}$，
$$
1 - y_q = (1 + x_n^q)^{-1};
$$
因此，序列$(y_q)$在$K_1$中趋于0，在$K_2$中趋于1，在$K_i$中对于$i \geq 3$趋于0或1。通过改变$K_i$的编号，因此可以假设存在整数$r$($1 \leq r < n$)使得$\overline{D}$包含点$(e_1, \ldots, e_n)$其中$e_i = 1$代表$1 \leq i \leq r$并且$e_i = 0$ 换$r + 1 \leq i \leq n$。现在， $\overline{D}$ 是 P 的向量子 K 空间。因此 $\overline{D}$ 包含的对角线 D' 和 D''
$$
P' = K_1 \times \cdots \times K_r,
$$
和$P'' = K_{r+1} \times \cdots \times K_n$。 归纳假设、$P' = \overline{D}'$ 和 $P'' = \overline{D}''$。因此$\overline{D} = P$。

### 习题 {#ac-vi-s7-exercises}

§ 7](exercises/s7/)参见[习题。
