---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 5
section_title: Magnus algebras
lang: zh
source: lie-i-iii
book_pages: 149-155, 193-201
pdf_pages: 0167-0173, 0211-0219
extraction: ocr
subsections:
    - "no": 1
      title: MAGNUS ALGEBRAS
      page: 149
      pdf_page: 167
    - "no": 2
      title: MAGNUS GROUP
      page: 150
      pdf_page: 168
    - "no": 3
      title: MAGNUS GROUP AND FREE GROUP
      page: 151
      pdf_page: 169
    - "no": 4
      title: LOWER CENTRAL SERIES OF A FREE GROUP
      page: 152
      pdf_page: 170
    - "no": 5
      title: '*p*-Filtration of Free Groups'
      page: 154
      pdf_page: 172
statements: 14
exercises: 12
content_sha256: 2afe4e4275e69980daf0fe577a38c2f20dac460703cfe70c50eb6132187c7570
translated_from: content/en/lie/II/05_s5_magnus_algebras.md
translation_method: google
source_content_sha256: 6bac6bb784fbb4b199b3afb36bd212ba5f589bd833743b3d4385ed3b9a405428
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 929605b8d0a8ea5545f1ebcc3df287eb9e44d603e2c35a7e3116652748540b28
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 5。马格努斯代数

In this paragraph, X denotes a set, F(X) the free group constructed on X (Algebra, Chapter I, § 7, no. 5) and A(X) the free associative algebra constructed on X with its total graduation $(A^n(X))_{n \geq 0}$ (cf. Algebra, Chapter III, § 3, no. 1, Example 3). X 在 F(X) 和 A(X) 中用其像来标识。

### 1. 马格努斯代数

设$\hat{A}(X)$为乘积模$\prod_{n \geq 0} A^n(X)$。我们按照规则定义在$\hat{A}(X)$乘法

$$
(a \cdot b)_n = \sum_{i=0}^n a_i \cdot b_{n-i}
$$

其中$a = (a_n)$和$b = (b_n)$在$\hat{A}(X)$中。我们知道（交换代数，章III, § 2, no. 12，例1），$\hat{A}(X)$是结合律代数，并且$A(X)$与$\hat{A}(X)$由……组成的子代数等同，序列的所有除了有限的数之外，项都是零。

$\hat{A}(X)$ 给出因子上离散拓扑的乘积拓扑

A^n(X);这拓扑使$\hat{A}(X)$成为完整的Hausdorff拓扑代数，当环 K具有离散的拓扑，并且$A(X)$在$\hat{A}(X)$中是稠密的

设 $a = (a_n) \in \hat{A}(X)$；族$(a_n)_{n \geq 0}$是可求和的并且$a = \sum_{n \geq 0} a_n$。

对于每个整数$m \geq 0$，令$\hat{A}_m(X)$表示级数$a = \sum_{n \geq m} a_n$的理想由……组成，使得$a_n \in A^n(X)$适用于所有$n \geq m$。这个理想的序列是$\hat{A}(X)$中0的邻域的基本系统以及$\hat{A}(X)$上的积分过滤。与上述过滤相关的阶函数用$\omega$表示；那么$\omega(0) = +\infty$和$\omega(a) = m$如果$a = \sum_{n \geq m} a_n$和$a_n \in A^n(X)$对于所有$n \geq m$和$a_m \neq 0$（§ 4，编号1和2）。

$\hat{A}(X)$ 被称为 K 中集合 X 和系数的 *Magnus 代数*。如果对 K 有任何歧义，我们写为 $\hat{A}_K(X)$。

#### 命题 1 {#lie-ii-s5-prop-1 .statement tag=0A5B}

*设 B 是单位结合词代数 ，具有实数过滤 $(B_\alpha)_{\alpha \in \mathbf{R}}$ ，使得 B 是 Hausdorff 且完全的（§ 4，第 1 和第 2 项）。令 f 为 B 中 X 的映射，使得存在 $\lambda > 0$ 且 $f(X) \subset B_\lambda$。那么 f 可以用一种且仅一种方式扩展到 B 中的 $\hat{A}(X)$ 的连续单位同态 $\hat{f}$。*

令 $f'$ 为 $A(X)$ 到 B 的唯一单位代数同态延伸$f$ (*代数*, 章 III, § 2, no. 7, 命题 7)。我们证明$f'$是*连续的*：$f'(A^n(X)) \subset B_{n\lambda}$从而$f'(\hat{A}_n(X) \cap A(X)) \subset B_{n\lambda}$。因此$f'$可以通过连续性以一种且仅一种方式扩展到同态$\hat{f} : \hat{A}(X) \to B$。

我们保留命题 1 的假设和记号，并令$u \in \hat{A}(X)$。 元素 $\hat{f}(u)$记为$u((f(x))_{x \in X})$，称为*用f(x)代替u*中的x的结果。特别是$u((x)_{x \in X}) = u$。现在让$u = (u_y)_{y \in Y}$是元素和$\hat{A}_1(X)$的一个家族，并让$v \in \hat{A}(Y)$。以上允许我们定义元素$v((u_y)_{y \in Y}) \in \hat{A}(X)$。用$v \circ u$表示。由于$u_y((f(x))) \in B_\lambda$，元素$u_y((f(x)))$可以代替v中的y。映射$v \mapsto (v \circ u)((f(x)))$和$v \mapsto v((u_y((f(x))))))$则$\hat{A}(X)$的单位代数到B中的两个连续同态取相同的值 $u_y((f(x)))$ 元素 $y \in Y$。因此 (命题1)

$$
(v \circ u)((f(x))) = v((u_y((f(x))))))
$$

对于所有$v \in \hat{A}(Y)$。

### 2. 马格努斯群

对于$\hat{A}(X)$中的所有$a = (a_n)_{n \geq 0}$，K的元素$a_0$将被称为a的*常数项*，并用$\varepsilon(a)$表示。 公式(1)表明$\varepsilon$是$\hat{A}(X)$的代数同态到K中。

#### 引理 1 {#lie-ii-s5-lem-1 .statement tag=0A5C}

*要使$\hat{A}(X)$的元素 a 可逆，其常数项在K中可逆是充分必要的。*

如果$a$在$\hat{\mathbf{A}}(\mathbf{X})$中可逆，则$\varepsilon(a)$在$K$中可逆。相反，如果$\varepsilon(a)$在$K$中可逆，则存在$u \in \hat{\mathbf{A}}_1(\mathbf{X})$使得$a = \varepsilon(a)(1-u)$；我们写$b = \left( \sum_{n \geq 0} u^n \right) \varepsilon(a)^{-1}$。那么$ab = ba = 1$和$a$是可逆的。

因此，常数项 1 的 $\hat{\mathbf{A}}(\mathbf{X})$ 的元素的集合是乘法幺半群 $\hat{\mathbf{A}}(\mathbf{X})$ 的子群，称为在$\mathbf{X}$（相对于 $K$）构建的 *Magnus 群*。在这个章中，它将由 $\Gamma(\mathbf{X})$ 或简称为 $\Gamma$ 表示。对于每个整数$n \geq 1$，我们用$a \in \Gamma$的$\Gamma_n$集合表示，这样$\omega(a-1) \geq n$。到 § 4, no. 5 的命题 2 时，序列 $(\Gamma_n)_{n \geq 1}$ 是 *$\Gamma$* 上的整体中央过滤。

### 3. 马格努斯群和免费群

#### 定理 1 {#lie-ii-s5-thm-1 .statement tag=0A5D}

*令 $r$ 为 $\mathbf{X}$ 的映射进入 $\hat{\mathbf{A}}(\mathbf{X})$，使得 $\omega(r(x)) \geq 2$ 对于所有 $x \in \mathbf{X}$。将自由群 $F(\mathbf{X})$ 的唯一同态 $g$ 放入 Magnus 群 $\Gamma(\mathbf{X})$，使得 $g(x) = 1 + x + r(x)$ 对于所有 $x \in \mathbf{X}$ 都是单射的。*

我们首先证明三个引理。

#### 引理 2 {#lie-ii-s5-lem-2 .statement tag=0A5E}

*令$n$为非零有理数整数。在正式幂级数$K[[t]]$的环中我们写$(1+t)^n = \sum_{j \geq 0} c_{j,n} t^j$。存在整数$j \geq 1$使得$c_{j,n} \neq 0$。

如果$n > 0$，则$c_{n,n} = 1$乘以二项式公式。
假设$n < 0$并设$m = -n$。如果 $c_{j,n} = 0$ 对于所有 $j \geq 1$，则 $(1+t)^n = 1$、从而，取相反的$(1+t)^m = 1$，即与……矛盾公式 $c_{m,m} = 1$。*

#### 引理 3 {#lie-ii-s5-lem-3 .statement tag=0A5F}

*令$x_1, \ldots, x_s$为$\mathbf{X}$的元素，使得$s \geq 1$和$x_i \neq x_{i+1}$对应于$1 \leq i \leq s-1$；令 $n_1, \ldots, n_s$ 为非零有理数整数。那么$\hat{\mathbf{A}}(\mathbf{X})$的元素$\prod_{i=1}^s (1+x_i)^{n_i}$就是$\neq 1$。

令$m$为$K$和$k$域$K/m$的最大理想；令$p : \hat{\mathbf{A}}_K(\mathbf{X}) \to \hat{\mathbf{A}}_k(\mathbf{X})$为单位$K$代数的唯一连续同态，使得$p(x) = x$对于$x \in \mathbf{X}$（no. 1，命题1）。只要证明$p\left( \prod_{i=1}^s (1+x_i)^{n_i} \right) \neq 1$和问题减少到$K$是域的情况就足够了。

在引理 2 的记号中：

$$
\prod_{i=1}^s (1+x_i)^{n_i} = \sum_{b_1 \geq 0} \cdots \sum_{b_s \geq 0} c_{b_1, n_1} \cdots c_{b_s, n_s} x_1^{b_1} \cdots x_s^{b_s}.
$$

到引理 2，存在整数 $a_i > 0$，使得$c_{a_i, n_i} \neq 0$ ($1 \leq i \leq s$)。通过 *代数*、章 I, § 7, no. 4、命题 6，没有单项式 $x_1^{b_1} \cdots x_s^{b_s}$ 使得 $b_i \geq 0$ 和 $(b_1, \ldots, b_s) \neq (a_1, \ldots, a_s)$ 可以等于 $x_1^{a_1} \ldots x_s^{a_s}$。由此可见，$\prod_{i=1}^s (1 + x_i)^{n_i}$中$x_1^{a_1} \ldots x_s^{a_s}$的系数是$c_{a_1, n_1} \ldots c_{a_s, n_s} \neq 0$，这暗示了结果。

#### 引理 4 {#lie-ii-s5-lem-4 .statement tag=0A5G}

*令 $\sigma$ 为 $\hat{A}(X)$ 的连续自同态，使得 $\sigma(x) = x + r(x)$ 对应 $x \in X$ (no. 1, 命题 1)。那么对于所有 $m \in \mathbf{N}$，$\sigma$ 就是自同构和 $\sigma(\hat{A}_m(X)) = \hat{A}_m(X)$。

$\sigma(x) \equiv x \mod \hat{A}_2(X)$对于$x \in X$、从而，对于$X$中的$n \geq 1$和$x_1, \ldots, x_n$，
$$
\sigma(x_1) \ldots \sigma(x_n) \equiv x_1 \ldots x_n \mod \hat{A}_{n+1}(X);
$$
对于所有$a \in A^n(X)$，特别是$\sigma(A^n(X)) \subset \hat{A}_n(X)$，$\sigma(a) \equiv a$以$\hat{A}_{n+1}(X)$为模，遵循线性关系。由此可见，$\sigma(A^n(X)) \subset \hat{A}_n(X)$对应$m \geq n$，从而$\sigma(\hat{A}_n(X)) \subset \hat{A}_n(X)$。在其他字中，$\sigma$与$A(X)$上的过滤$(\hat{A}_m(X))$相容的，并且其限制与相关分级环是同一性。因此 $\sigma$ 是双射 (*交换代数*, 章 III, § 2, no. 8, 推论 3 到定理 1)。

最后我们证明定理 1。令$w \neq 1$为$F(X)$的元素。由*代数*，章I, § 7, no. 5，命题7，$X$中存在$x_1, \ldots, x_s$和非零有理数整数$n_1, \ldots, n_s$，使得$s \geq 1$，$x_i \neq x_{i+1}$（$1 \leq i \leq s-1$）和
$$
w = x_1^{n_1} \ldots x_s^{n_s}.
$$
在引理4中的记号，
$$
g(w) = \prod (1 + \sigma(x_i))^{n_i} = \sigma(\prod (1 + x_i)^{n_i}),
$$
因此 $g(w) \neq 1$ 乘以引理 3 和 4。

### 4. 自由群的下部中央级数

我们要证明以下两个定理：

#### 定理 2 {#lie-ii-s5-thm-2 .statement tag=0A5H}

*假设在环$K$关系$n.1 = 0$中对于每个整数$n$意味着$n = 0$。 令$r$为$X$的映射进入$\hat{A}(X)$，使得$x \in X$为$\omega(r(x)) \geq 2$，并令$g$为$F(X)$的同态进入马格努斯群$\Gamma(X)$，使得$g(x) = 1 + x + r(x)$ $x \in X$。 对于所有 $n \geq 1$，$C^n F(X)$ 是逆像 $g$ 子群 $1 + \hat{A}_n(X)$ $\Gamma(X)$。*

#### 定理 3 {#lie-ii-s5-thm-3 .statement tag=0A5I}

*对于所有$x \in X$，令$c(x)$为$F(X)/(F(X), F(X))$中$x$的典范像。 令 $g$ 为与 $F(X)$ (§ 4, no. 6) 的过滤 $(C^n F(X))_{n \geq 1}$ 相关的分级李 $\mathbf{Z}$ 代数。 自由李$\mathbf{Z}$-代数$L_\mathbf{Z}(X)$到扩展$c$的$g$的独特同态是同构。*

宽松地说，与自由群 $F(X)$（与下部中央级数）相关联的分级李 $\mathbf{Z}$ 代数是自由李 $\mathbf{Z}$ 代数 $L_\mathbf{Z}(X)$。

我们记作$F(X) = F, \Gamma(X) = \Gamma, \hat{A}(X) = \hat{A}, \hat{A}_\mathbf{Z}(X) = \hat{A}_\mathbf{Z}, C^n F(X) = C^n, \Gamma_n = 1 + \hat{A}_n(X)$，并令$\alpha : L_\mathbf{Z}(X) \to g$为在定理3的叙述中引入的同态。

(A) 初步削减。

让$\gamma$表示$F$的同态到由$\gamma(x) = 1 + x$为$x \in X$定义的$\Gamma$中。到引理 4 时，存在代数 $\hat{A}$ 的自同构 $\sigma$ 与$\hat{A}$ 上的过滤兼容，使得 $\sigma(1 + x) = g(x)$ 对于所有 $x \in X$；那么 $\sigma(\Gamma_n) = \Gamma_n$ 代表所有 $n$。作为$F$的同态$g$和$\sigma \circ \gamma$进入$\Gamma$重合在$X, g = \sigma \circ \gamma$上，因此$g^{-1}(\Gamma_n) = \gamma^{-1}(\Gamma_n)$。在定理 2的假设下，$\mathbf{Z}$可以与$K$的子环等同；因此，Magnus 代数 $\hat{A}_\mathbf{Z}$ 与 $\hat{A}$ 的子环相同，$\hat{A}_\mathbf{Z}$ 上的过滤由 $\hat{A}$ 上的过滤引起。将$\gamma$映射$F$转化为$\hat{A}_\mathbf{Z}$，我们看到在补充假设$K = \mathbf{Z}, r = 0$下证明定理2和3就足够了，因此在$g = \gamma$下，我们将做出假设。

(B) $\alpha$ 的满射性。

作为$X$生成群$F = C^1$、集合$c(X)$生成$\mathbf{Z}$-模块$g^1 = C^1/C^2$。但是$g^1$生成谎言$\mathbf{Z}$-代数$g$（§ 4, no. 6，命题5），因此$c(X)$生成$g$，这证明$\alpha$是满射的。

(C) 我们认同分级为代数$\mathrm{gr}(\hat{A})$，$A(X)$低于典范同构$A^n(X) \to \hat{A}_n/\hat{A}_{n+1}$。对于每个整数 $n \geq 1$，我们写 $F^n = \gamma^{-1}(\Gamma_n)$；我们知道（§ 4, no. 5）$(F^n)_{n \geq 1}$是$F$的整体中央过滤。让 $g'$ 表示相关的分级李 $\mathbf{Z}$-代数 (§ 4, no. 4)。让$f$是$g'$的李代数同态到与$\gamma$相关联的$A(X)$（§ 4, no. 5，命题3）。现在，对于每个整数 $n \geq 1$（§ 4, no. 6，命题 4），$C^n \subset F^n$，因此 $g = \bigoplus_{n \geq 1} C^n/C^{n+1}$ 中有典范同态 $\varepsilon$ 进入 $g' = \bigoplus_{n \geq 1} F^n/F^{n+1}$

$$
L_\mathbf{Z}(X) \xrightarrow{\alpha} g \xrightarrow{\varepsilon} g' \xrightarrow{f} A(X).
$$

我们写$\beta = f \circ \varepsilon$；我们明确地给出$\beta$如下：如果$u$是$C^n$的元素$w$右$C^{n+1}$取类模，那么$\gamma(w) - 1$是$\hat{A}$中的阶$\geq n$并且$\beta(u)$是次数$n$的$\gamma(w) - 1$的齐次分量。尤其，

$$
\beta(c(x)) = x \quad \text{for all } x \in X.
$$

(D) 定理 2 和 3 的证明。

李代数同态 $\beta \circ \alpha : L_\mathbf{Z}(X) \to A(X)$ 限制为 $X$ 是 (3) 的恒等式，因此是典范嵌入 (§ 3, no. 1)。因此 $\alpha$ 是单射的，因此与 (B) 是双射的；这证明了定理 3。由于$\beta \circ \alpha = f \circ \varepsilon \circ \alpha$是单射，$\alpha$是双射，$\varepsilon$是单射。对于所有$n \geq 1$，

$$
\varepsilon_n : C^n/C^{n+1} \to F^n/F^{n+1}
$$

是单射的，因此

$$
C^n \cap F^{n+1} = C^{n+1}.
$$

C^1 = F = F^1;如果 C^n = F^n，则 C^n \cap F^{n+1} = F^{n+1} 从而 C^{n+1} = F^{n+1}
在 n \geqslant 1 上通过归纳证明定理 2。

#### 推论 {#lie-ii-s5-n4-cor-1 .statement tag=0A5J}

$$
\bigcap_{n \geqslant 1} C^n F(X) = \{e\}.
$$

应用定理 2 且 K = \mathbf{Z} 且 r = 0，
$$
\bigcap_{n \geqslant 1} C^n F(X) = \bigcap_{n \geqslant 1} g^{-1}(1 + \hat{A}_n(X)) = g^{-1}\left(\bigcap_{n \geqslant 1} (1 + \hat{A}_n(X))\right) = g^{-1}(1) = \{e\}.
$$

#### 注 {#lie-ii-s5-n4-rem-1 .statement tag=0A5K}

令 H 为相对于 X (§ 2, no. 10) 的霍尔集合。设 M 为由合成 (x, y) 的律 (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy 在 F(X) 上定义的岩浆，并设 $\phi$ 为 M(X) 的同态到 M，其限制为X 是身份。 $\phi(H)$ 的元素被称为与大厅集合 H 相关的 F(X) 的*基本换位子*。对于每个整数 n \geqslant 1，令 H_n 为 H 的子集元素的由……组成长度n；我们知道 (§ 2, no. 11, 定理 1) H_n 的典范映射到 L_\mathbf{Z}(X) 中是阿贝尔的群 L_\mathbf{Z}^n(X) 的基。此外，$\phi(H_n) \subset C^n$；对于所有 m \in H_n，令 $\phi_n(m)$ 表示类 mod。 C^{n+1} / $\phi(m) \in C^n$。 定理 3 然后表明 $\phi_n$ 是 H_n 的 *双射到阿贝尔的群* C^n/C^{n+1} 的基。紧接着，对于所有 w \in F(X) 和所有 i \geqslant 1，存在 $\mathbf{Z}^{(H_i)}$ 的唯一元素 $\alpha_i$，这样，对于 n \geqslant 1，

$$
w = \prod_{i=1}^n \prod_{m \in H_i} \phi(m)^{\alpha_i(m)} \mod. C^{n+1},
$$

其中乘积是根据H上给出的总排序计算的。

#### 例 {#lie-ii-s5-n4-exa-1 .statement tag=0A5L}

假设 X 是集合，有两个元素 x, y，令 H_1 = \{x, y\}, H_2 = \{xy\}。因此，F(X) 的每个元素 w 都可以写成
$$
w \equiv x^a y^b (x, y)^c \mod. C^3 \quad \text{with } a, b, c \text{ in } \mathbf{Z}.
$$
对于 w = (xy)^n、a = b = n 且 c = n(1 - n)/2 (cf. 习题 9)、从而
$$
(xy)^n \equiv x^n y^n (x, y)^{n(1-n)/2} \mod. C^3.
$$

### 5. *p*-过滤游离群

在这个数中，*p* 表示素数数，我们假设 K = \mathbf{F}_p。对于X中的x，令$\gamma$为F(X)的同态进入由$\gamma(x) = 1 + x$定义的$\Gamma(X)$；我们写$F_n^{(p)}(X) = \gamma^{-1}(1 + \hat{A}_n(X))$。 序列 $(F_n^{(p)}(X))_{n \geqslant 1}$ 是 F(X) 上的积分中央过滤，它是“分离的”，因为 $\gamma$ 是单射的（no. 3，定理 1）。这称为 F(X) 上的 *p* 过滤。

#### 命题 2 {#lie-ii-s5-prop-2 .statement tag=0A5M}

*假设X是有限的。对于每个整数 n \geqslant 1，群 F(X)/F_n^{(p)}(X) 是幂零的有限 p 群类 \leqslant n.*

由归纳对$n$论证，足以证明$F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$是所有$n \geqslant 1$的有限交换$p$群。对于所有$w \in F_n^{(p)}(X)$，$\hat{A}(X)$的元素$\gamma(w) - 1$是阶$\geqslant n$；我们用$\delta_n(w)$表示次数$n$的$\gamma(w) - 1$的齐次分量。 映射 $\delta_n : F_n^{(p)}(X) \to A^n(X)$ 是同态与核 $F_{n+1}^{(p)}(X)$ (§ 4, no. 5, 命题 3)，因此 $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ 与 $A^n(X)$ 的子群同构。由于$X$是有限的，$A^n(X)$是有限维向量空间超过$\mathbf{F}_p$，因此是有限交换的$p$群，$F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$也是如此。

#### 命题 3 {#lie-ii-s5-prop-3 .statement tag=0A5N}

*对于$F(X)$中的所有$w \neq 1$，存在一个有限$p$群$G$和$F(X)$的同态$f$进入$G$，使得$f(w) \neq 1$。*

存在$X$和整数$n_1, \ldots, n_r$使得$w = x_1^{n_1} \ldots x_r^{n_r}$存在元素$x_1, \ldots, x_r$。让$Y = \{x_1, \ldots, x_r\}$。 $Y$的典范嵌入变为$X$扩展至同态$\alpha : F(Y) \to F(X)$；另一方面，设$\beta$是$F(X)$到$F(Y)$的同态，其中限制到$Y$是恒等式，映射$X - Y$到$\{1\}$。那么$\beta(\alpha(y)) = y$对应$y \in Y$，因此$\beta \circ \alpha$是$F(Y)$的恒等式自同构。显然$F(Y)$中存​​在$w'$使得$w = \alpha(w')$；然后$\beta(w) = w' \neq 1$；现在$\bigcap_{n \geqslant 1} F_n^{(p)}(Y) = \{1\}$，因此存在整数$n \geqslant 1$，使得$\beta(w) \notin F_n^{(p)}(Y)$。通过命题 2，群 $G = F(Y)/F_n^{(p)}(Y)$ 是有限 $p$ 群。如果$f$是$\beta$的合成和$F(Y)$的典范同态到$G$，则$f(w) \neq 1$。

#### 推论 {#lie-ii-s5-n5-cor-1 .statement tag=0A5O}

*$F(X)$中有限指标的正常子群的交为$\{1\}$。*

### 习题 {#lie-ii-s5-exercises}

在下面的习题中，我们假设§ 5的假设和记号。 $F$ 表示 $F$ 的自由群 $F(X)$ 和 $g$ 唯一同态进入 Magnus 群 $\Gamma(X)$，使得 $g(x) = 1 + x$ 对于所有 $x \in X$ (cf. 定理 1）。

参见[习题为 § 5](exercises/s5/)。
