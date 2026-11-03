---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 7
section_title: Lie groups over an ultrametric field
lang: zh
source: lie-i-iii
book_pages: 326-337, 391-395
pdf_pages: 0344-0355, 0409-0413
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 327
      pdf_page: 345
    - "no": 2
      title: EXPONENTIAL MAPPINGS
      page: 328
      pdf_page: 346
    - "no": 3
      title: STANDARD GROUPS†
      page: 328
      pdf_page: 346
    - "no": 4
      title: FILTRATION OF STANDARD GROUPS
      page: 330
      pdf_page: 348
    - "no": 5
      title: POWERS IN STANDARD GROUPS
      page: 331
      pdf_page: 349
    - "no": 6
      title: LOGARITHMIC MAPPING
      page: 333
      pdf_page: 351
statements: 26
exercises: 10
content_sha256: 40b382739a92ebbb792212a02a09bf83edd7c53764a91dadcd90a59fb6cb0e5d
translated_from: content/en/lie/III/07_s7_lie_groups_over_an_ultrametric_field.md
translation_method: google
source_content_sha256: a4785cb8d75380fad37a9781d0116e8b216b652f0d5b68e842a5a1dfdd3864bc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 7c14a099f44de88c4b9de3a438f586d6c1482718383bb8355ebe061862532708
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 7。 李群超过超测量域

在本段中，假设域$K$是超度量且特征为0。让$A$表示$K$的评估环，$m$表示$A$的最大理想，$p$表示剩余类域的特征$A/m$。如果 $K$ 是局部紧致的，则 $p \neq 0$ (*交换代数*, 章 VI, § 9, 定理 1)。

### 1. 从李代数到李群的通道

#### 命题 1 {#lie-iii-s7-prop-1 .statement tag=0AH2}

令 G 为李群 germ 和单位元素 e。 G 的谎言子群的 G 由……组成中存在 e 的开邻域的基系统。

令 L(G) 被赋予范数与其拓扑兼容，并且使得$\| [x, y] \| \leq \| x \| \| y \|$ 对于L(G) 中的所有 x, y。令 G_1 为由 L(G) 定义的李群。通过§ 4, no. 2、定理2，G 和G_1 局部同构。然后应用§ 4, no. 2、引理 3 (iii) 即可。

#### 定理 1 {#lie-iii-s7-thm-1 .statement tag=0AH3}

令 L 为完全范数李代数。存在李群 G 使得 L(G) 同构于 L。两个这样的群是局部同构的。

第一个断言已在§ 4, no. 2、引理3中得到证明。第二个是§ 4, no. 2、定理2的特例。

#### 定理 2 {#lie-iii-s7-thm-2 .statement tag=0AH4}

设 G 为李群，并且 h 为 L(G) 的谎言子代数，承认拓扑补充。 G 存在一个谎言子群 H，使得 L(H) = h。如果 H_1 和 H_2 是 G 的谎言子群，使得 L(H_1) = L(H_2) = h，则 H_1 \cap H_2 在 H_1 和 H_2 中开集。

第一个断言源自命题1和§ 4, no. 2，定理3。第二个§ 4, no. 2，定理3的特殊情况。

#### 定理 3 {#lie-iii-s7-thm-3 .statement tag=0AH5}

令G和H为李群，h为L(G)到L(H)的连续态射。

(i) 存在 G 的开子群 G' 和 G' 的李群态射 $\phi$ 进入 H，使得 $h = L(\phi)$。

(ii) 令 G_1、G_2 将 G 的子群和 G_i 的$\phi_i$ 态射开入 H，使得 $h = L(\phi_i)$。然后$\phi_1$和$\phi_2$重合在G的开子群上。

到命题 1，这是从 § 4, no. 1、定理 1 得出的。

#### 命题 2 {#lie-iii-s7-prop-2 .statement tag=0AH6}

设 G 为李群，并且有一个 L(G) 的谎言子代数，承认拓扑补充。以下条件是等效的：

(i) 存在 G 的开子群 G' 和 G' 的正规李子群 H，使得 L(H) = h。

(ii) h 是 L(H) 的理想值。

如果存在具有 (i) 性质的 G' 和 H，则 L(G') = L(G) 且 L(H) 是 L(G') × § 3, no. 12、命题 47 的理想。

假设 h 是 L(G) 的理想。存在李群 F 使得 L(F) = L(G)/h (定理 1)。令h为L(G)到L(F)的规范态射。到定理 3 (i)，存在 G 的开子群 G' 和 G' 的李群态射 $\phi$ 进入 F，使得 $L(\phi) = h$。通过§ 3, no. 8，$\phi$的核 H是G'和$L(H) = \mathrm{Ker}\ L(\phi) = \mathrm{Ker}\ h = h$的谎言子群。最后，从 $H = \mathrm{Ker}\ \phi$ 开始，H 在 G' 中是正规的。

### 2. 指数映射

#### 命题 3 {#lie-iii-s7-prop-3 .statement tag=0AH7}

令 G 为李群。 G 存在一个指数映射 $\phi$，具有以下性质：
(i) $\phi$ 定义在加法群 $L(G)$ 的开子群 U 上；
(ii) $\phi(U)$ 是 G 的开子群，$\phi$ 是解析式流形 U 到解析式流形 $\phi(U)$ 的同构；
(iii) $\phi(nx) = \phi(x)^n$ 适用于所有 $x \in U$ 和所有 $n \in \mathbf{Z}$。

让 $L(G)$ 被赋予与其拓扑兼容的范数，并且使得 $\| [x, y] \| \leq \| x \| \| y \|$ 适合 $L(G)$ 中的 $x, y$。设 $G_1$ 为由 $L(G)$ 定义的李群。让$\psi = \mathrm{Id}_{G_1}$，它是$G_1$的指数映射。对于所有$\mu > 0$，令$L_\mu$为$x \in L(G)$的集合，使得$\| x \| < \mu$。那么，对于足够小的$\mu$，$L_\mu$是加法群$L(G)$的开子群，$\psi(L_\mu)$是$G_1$的开子群（§ 4, no. 2，引理3），对于所有$x \in L_\mu$和所有$n \in \mathbf{Z}$，$\psi|L_\mu$是$L_\mu$解析流形到$\psi(L_\mu)$和$\psi(nx) = \psi(x)^n$的同构。 $L_\mu$ 形式邻域的基本系统为 $L(G)$ 中的 0。到定理 1，存在$\mu$和G的开子群$G'$，使得$\psi(L_\mu)$和$G'$同构，从而命题。

#### 命题 4 {#lie-iii-s7-prop-4 .statement tag=0AH8}

令 G 为李群且 $\phi$ G 的单射指数映射。假设 $p > 0$。对于$L(G)$中的所有$x, y$，

(1)
$$
x + y = \lim_{n \to +\infty} p^{-n} \phi^{-1}(\phi(p^n x) \phi(p^n y))
$$
(2)
$$
[x, y] = \lim_{n \to +\infty} p^{-2n} \phi^{-1}(\phi(p^n x) \phi(p^n y) \phi(-p^n x) \phi(-p^n y)).
$$

这些是命题 4 of § 4, no. 3 的特殊情况。

### 3. 标准群†

如果 $S(X_1, X_2, \ldots, X_n)$ 是形式幂级数，系数在 $A$ 中，那么，对于 m 中的所有 $x_1, \ldots, x_r$，级数 $S(x_1, x_2, \ldots, x_r)$ 是收敛的。更准确地说，$m \times m \times \cdots \times m$包含在$S$的绝对收敛域中（可微且解析流形，R，4.1.3）。

#### 定义 1 {#lie-iii-s7-def-1 .statement tag=0AH9}

设 r 为整数 $\geq 0$。 K 上的维数 r 的标准群是李群 G，具有以下属性：
(i) G 的基础解析流形为 $m \times m \times \cdots \times m$ (r 因子)；
(ii) 在 2r 个变量中存在形式幂级数 F，$A^r$ 中有系数，没有常数项，使得对于 G 中的所有 $x, y$ 都有 $x.y = F(x, y)$。

那么G的$0.0 = 0$和单位元素就是$m \times m \cdots \times m$的原点。

† 结果。当 K 的特征为 $> 0$ 时，3 和 4 及其证明仍然成立。

L(G) 将用 K' 标识。由§ 5，公式 (13)，L(G) 的结构相对于典范基属于到A的常数。我们需要在相同的证明中考虑m×...×m的元素，现在为G 的元素，现在为 L(G) 的元素。

#### 例 {#lie-iii-s7-n3-exa-1 .statement tag=0AHA}

令G = 1 + M_n(m)，这是M_n(K)的开子集。如果 x ∈ G，则 det x ∈ 1 + m，因此 G ⊂ GL(n, K)。显然 GG ⊂ G。如果 x = 1 + y 且 y ∈ M_n(m)，矩阵的逆计算首先证明 x^{-1} ∈ M_n(A)；如果我们写 x^{-1} = 1 + y'，则 y + y' + yy' = 0，因此 y' ∈ M_n(m)，因此 x^{-1} ∈ G。因此 G 是 GL(n, K) 的开子群。我们通过映射 (\delta_{ij} + y_{ij}) ↦ (y_{ij}) 来认同 G 和 m^{n^2}。显然 G 是标准群。

#### 定理 4 {#lie-iii-s7-thm-4 .statement tag=0AHB}

令 G 为有限维李群。存在与标准群同构的G的开子群。

通过替换 G 和群同构于 G 的开子群，问题被简化为 G 是 K' 的开子集，其中单位元素 0 并且乘积 x.y 的坐标和逆坐标x^{[-1]} 由公式给出

(3) $$(x.y)_i = x_i + y_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta i} x^\alpha y^\beta \quad (i = 1, 2, \ldots, r)$$

(4) $$(x^{[-1]})_i = -x_i + \sum_{|\alpha| > 1} d_{\alpha i} x^\alpha \quad (i = 1, 2, \ldots, r)$$

其中右侧的级数对于 G 中的 x、y 是收敛的 (§ 5, no. 1)。令 λ ∈ K* 并令群运算通过比率 λ 的位似从 G 传输到 G' = λG。对于 G' 中的 x', y'，乘积 x'.y' 和 G' 中计算的逆 x'^{[-1]} 具有坐标

$$(x'.y')_i = x'_i + y'_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c'_{\alpha \beta i} {x'}^\alpha {y'}^\beta \quad (i = 1, 2, \ldots, r)$$

$$({x'}^{[-1]})_i = -x'_i + \sum_{|\alpha| > 1} d'_{\alpha i} {x'}^\alpha \quad (i = 1, 2, \ldots, r)$$

哪里

$$c'_{\alpha \beta i} = \lambda^{-|\alpha|-|\beta|+1} c_{\alpha \beta i}, \qquad d'_{\alpha i} = \lambda^{-|\alpha|+1} d_{\alpha i}.$$

由于级数 (3) 和 (4) 收敛，我们看到，对于 |λ| 足够大，对于所有 α、β、i，

$$|c'_{\alpha \beta i}| \leq 1, \qquad |d'_{\alpha i}| \leq 1$$

即 c'_{\alpha \beta i} ∈ A 和 d'_{\alpha i} ∈ A;另一方面 G' ⊃ m × m × ... × m。那么 m × m × ... × m 是 G' 的开子群，并且是标准群。

### 4. 标准群过滤

我们再次使用定义 1 的记号。我们选择数 $a > 1$ 以及 $K$ 的实际估值 $v$，这样 $|x| = a^{-v(x)}$ 对于所有 $x \in K$ (交换代数， 章VI, § 6、命题3)。如果$a$是包含在$m$中的$A$的非零（因此开）理想，则让$G(a)$表示$G$的元素的集合，其坐标属于到$a$。如果$\lambda \in \mathbf{R}$，令$a_\lambda$（或$a_\lambda^+$）表示$x \in K$的集合，使得$v(x) \geq \lambda$（或$v(x) > \lambda$）；然后$a_0 = A$，$a_0^+ = m$。对于$x = (x_1, \ldots, x_r) \in G$，我们应该写

$$
\omega(x) = \inf(v(x_1), \ldots, v(x_r)).
$$

#### 命题 5 {#lie-iii-s7-prop-5 .statement tag=0AHC}

令$G$为标准群。

(i) 如果$a$是包含在$m$中的$A$的非零理想，则$G(a)$是$G$的开法线子群。

(ii) $G(a_\lambda)$，对于$\lambda > 0$，形式是$G$中$e$的邻域的基本系统。

(iii) 假设 $\lambda \geq \lambda_0$ 为 $a_\lambda \subset a$，并让 $\lambda \geq \lambda_0$ 的 $G(a)/G(a_\lambda)$ 被赋予离散的拓扑。那么拓扑群$G(a)$就是群$G(a)/G(a_\lambda)$的逆极限。

(iv) 设$a, b$为$m$中包含的$A$的非零理想，使得$a \supset b \supset a^2$。 $G(a)$的映射$x \mapsto (x_1 \bmod b, \ldots, x_r \bmod b)$进入$(a/b) \times \cdots \times (a/b)$定义，经过至商同构，群$G(a)/G(b)$进入加法群$(a/b) \times \cdots \times (a/b)$。

如果$x \in G$和$y \in G(a)$，$x$和$x.y$的坐标等于模$a$。因此，对于$G$中的$x', x''$和$G(a)$中的$y', y''$，$x'.x''$和$(x'.y').(x''.y'')$的坐标等于模$a$。这就证明了(i)。

(ii) 是显而易见的。

(iii) 由上述和一般拓扑、章 III, § 7、命题 2 得出。

如果$x \in G(a)$和$y \in G(a)$，$x.y$的坐标与$x + y$模$G(a^2)$除以§ 5的公式（4）的坐标一致。这就证明了(iv)。

#### 推论 {#lie-iii-s7-n4-cor-1 .statement tag=0AHD}

假设 $K$ 是局部紧致的，并设 $q = \mathrm{Card}(A/m)$。

(i) 如果$a = m^a$和$b = m^b$与$b \geq a \geq 1$，则$G(a)/G(b)$是基数$q^{r(b-a)}$的$p$群。

(ii) $G(a)$ 是 $p$ 组中的逆极限。

$G(a)/G(b)$中元素的数为$(\mathrm{Card}(a/b))^r$；如果$b = a + 1$，$a/b$是$A/m$，从而上的一维向量空间 (i) 在这种情况下；一般情况下是$b - a$上的归纳。 断言 (ii) 由 (i) 和命题 5 (iii) 得出。

#### 命题 6 {#lie-iii-s7-prop-6 .statement tag=0AHE}

令 $a, b, c, c'$ 为 $m$ 中包含的 $A$ 的非零理想，使得

$$
c' \subset c, \quad ab \subset c, \quad ab^2 \subset c', \quad a^2b \subset c'.
$$

如果$x \in G(a)$和$y \in G(b)$，则$x^{[-1]}y^{[-1]}x.y, x.y.x^{[-1]}y^{[-1]}$和$[x,y]$属于到$G(c')$并且模$G(c')$全等。

由§ 5, no. 2，命题 1，存在$c_{\alpha\beta} \in A'$使得
$$
x^{[-1]}y^{[-1]}x.y - [x,y] = \sum_{|\alpha| + |\beta| \geq 3} c_{\alpha\beta} x^\alpha y^\beta.
$$
如果$x = 0$或$y = 0$，则$x^{[-1]}y^{[-1]}x.y - [x,y] = 0$；因此$c_{0\beta} = c_{\alpha 0} = 0$。
另一方面，条件
$$
x \in G(a), \quad y \in G(b), \quad |\alpha| \geq 1, \quad |\beta| \geq 1, \quad |\alpha| + |\beta| \geq 3
$$
暗示
$$
c_{\alpha\beta} x^\alpha y^\beta \in G(a^2 b + ab^2) \subset G(c')
$$
因此$x^{[-1]}y^{[-1]}x.y - [x,y] \in G(c')$。我们同样看到
$$
x.y.x^{[-1]}y^{[-1]} - [x,y] \in G(c').
$$
最后，通过§ 5，公式（13），$[x,y] \in G(ab) \subset G(c)$。

#### 命题 7 {#lie-iii-s7-prop-7 .statement tag=0AHF}

(i) *族* $(G(a_\lambda))$ *是对* $G$ *(章 II, § 4, no. 4, 定义 2)* 的中央过滤。
(ii) *对于* $\lambda \in \mathbf{R}_+^*$、$G(a_\lambda) = \{ x \in G | \omega(x) \geq \lambda \}$、$G(a_\lambda^+) = \{ x \in G | \omega(x) > \lambda \}$。
(ii) 是显而易见的。我们证明（i）。显然$G(a_\lambda) = \bigcap_{\mu < \lambda} G(a_\mu)$和$G = \bigcup_{\lambda > 0} G(a_\lambda)$。
另一方面，如果 $x \in G(a_\lambda)$ 和 $y \in G(a_\mu)$，则
$$
x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})
$$
命题 6 与 $a = a_\lambda, b = a_\mu, c = c' = a_{\lambda+\mu}$ 一起应用。

通过章II, § 4, no. 4，我们可以将形式群$\mathrm{gr}(G)$与群$G$相关联，并进行中央过滤$(G(a_\lambda))$。 对所有$\lambda > 0$写出$G_\lambda = G(a_\lambda)/G(a_\lambda^+)$，我们得到$\mathrm{gr}(G) = \bigoplus_{\lambda > 0} G_\lambda$。 回想一下（*loc.cit.*，命题 1），$G$中的换位子允许我们在$\mathrm{gr}(G)$中使用定义括号，其中$\mathrm{gr}(G)$是李代数，如下所示：如果$\bar{x} \in G_\lambda$和$\bar{y} \in G_\mu$，则选择 $G(a_\lambda)$中$\bar{x}$的代表$x$和$G(a_\mu)$中$\bar{y}$的代表$y$；那么$[\bar{x}, \bar{y}]$是$G_{\lambda+\mu}$中$x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})$的类。 到命题 6，与$a = a_\lambda, b = a_\mu, c = a_{\lambda+\mu}, c' = a_{\lambda+\mu}^+$一起应用，我们看到$[\bar{x}, \bar{y}]$也是$G_{\lambda+\mu}$中$[x, y]$的类。 因此，当 $G$ 被视为 $L(G) = K^r$ 的谎言子代数时，经 $G(a_\lambda)$ 过滤，相关分级李代数 (章 II, § 4, no. 3) 等于 $\mathrm{gr}(G)$。

### 5. 标准幂群

我们保留 no. 4 的记号。

#### 命题 8 {#lie-iii-s7-prop-8 .statement tag=0AHG}

*设*$n \in \mathbf{Z}$*和*$h_n$*为映射*$x \mapsto x^n$*的*$G$*到*$G$。 *让*$a$*成为*$A$*包含在*$m$中的非零理想，*使得*$n \notin a$。 *然后* $h_n|G(a)$ *是解析流形* $G(a)$ *的同构到解析流形* $G(na)$。

根据标准群的定义，$h_n$等于整个$G$到级数积分的和与$A'$中的系数。由 § 5、公式 (4) 得出，此级数为形式
$$
h_n(x) = nx + \sum_{|\alpha| \geq 2} a_\alpha x^\alpha.
$$
因此，对于$x \in G$，
$$
\begin{align*}
h_n(nx) &= n^2 \left( x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha \right) \\
&= n^2 S(x)
\end{align*}
$$
我们写$S(x) = x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha$。这个级数$S(x)$定义是$G$到$G$的解析映射，也用$S$表示。由*代数*，章IV, § 6，命题8，$r$变量中存在积分级数$S'$，$A'$中存在系数，使得$S'(S(X)) = S(S'(X)) = X$。因此，$S$是流形$G$自身解析的同构，并且对于$A$的每个非零理想$b$包含在$m$，$S(G(b)) \subset G(b)$，$S'(G(b)) \subset G(b)$中，因此
$$
S(G(b)) = G(b).
$$
对于$y \in nG$的$h_n(y) = n^2 S \left( \frac{1}{n} y \right)$，我们看到$h_n|nG(b)$是解析式流形$nG(b)$到解析式流形$n^2 G(b)$的同构。但是，由于 $n \notin a$、$|n| > |\lambda|$ 对于所有 $\lambda \in a$，因此 $n^{-1} a \subset m$ 以及$a$ 都是形式 $nb$，其中 $b$ 是$m$ 中包含的 $A$ 的非零理想。

#### 推论 {#lie-iii-s7-n5-cor-1 .statement tag=0AHH}

*如果 $n$ 在 $A$ 中可逆，则 $h_n$ 是流形 $G$ 自身解析的同构。对于$m$、$h_n(G(a)) = G(a)$中包含的$A$的每个非零理想$a$。对于所有 $x \in G$、$\omega(x^n) = \omega(x)$。*

这紧随命题 8。

#### 命题 9 {#lie-iii-s7-prop-9 .statement tag=0AHI}

*假设$p \neq 0$。
(i) 令$a, b$为$A$的非零理想，使得$b \subset a \subset m$。 在群 $G(a)/G(b)$ 中，每个元素都有 $p$ 的阶幂。
(ii) 假设$v(p) = 1$。 如果 $x \in G$ 满足 $\omega(x) > \frac{1}{p-1}$，那么*
$$
\omega(x^p) = \omega(x) + 1.
$$
由 § 5、公式 (4)，对于所有 $x \in G$，
$$
x^p = px + \sum_{|\alpha| \geq 2} c_\alpha x^\alpha
$$
其中$c_\alpha \in A'$代表所有$\alpha$。 即使对于证明(i)，也可以假设$v(p) = 1$。 Then if $\omega(x) \geq 1$, it follows that $\omega(x^p) \geq \omega(x) + 1$ and hence $\omega(x^{p^n})$ tends to $+\infty$ as $n$ tends to $+\infty$; this proves (i). 由于对于$1 \leq i \leq p - 1$，$\binom{p}{i}$可被$p$整除，§ 5, no. 3的命题2，证明$c_\alpha \in pA'$对于
$$
2 \leq |\alpha| \leq p - 1
$$
因此
$$
\omega(c_\alpha x^\alpha) > \omega(px) = \omega(x) + 1 \quad \text{for } 2 \leq |\alpha| \leq p - 1.
$$
另一方面，如果$|\alpha| \geq p$，$\omega(c_\alpha x^\alpha) \geq p \omega(x)$和$p \omega(x) > \omega(x) + 1$，如果$\omega(x) > \frac{1}{p - 1}$。 这就证明了(ii)。

### 6. 对数映射

#### 引理 1 {#lie-iii-s7-lem-1 .statement tag=0AHJ}

假设$p \neq 0$。 令$G$为李群，$G_1$是$G$的开子群，它与标准群和$x \in G$同构的。 以下条件是等效的：
(i) $x$存在幂，其中属于到$G_1$；
(ii) 存在整数的严格递增的序列$(n_i)$，使得$x^{n_i}$趋于$e$，而$i$趋于$+\infty$。
(ii) $\Rightarrow$ (i)：显而易见。
(i) $\Rightarrow$ (ii)：假设$y = x^m \in G_1$。 在 no. 5 的命题 9 (i) 处，$y^{p^n}$ 趋向 $e$，$n$ 趋向 $+\infty$，在其他字 $x^{m p^n}$ 趋向 $e$，$n$ 趋向 $+\infty$。

#### 命题 10 {#lie-iii-s7-prop-10 .statement tag=0AHK}

假设$p \neq 0$。令 $G$ 为有限维李群。令$G_f$为$x \in G$的集合，其中存在整数的严格递增的序列$(n_i)$，使得$x^{n_i}$趋于$e$，而$i$趋于$+\infty$。
(i) $G_f$于$G$开放。
(ii) $G_f$ 到 $L(G)$ 中存在且仅有一个映射 $\psi$，具有以下性质：
(a) $\psi(x^n) = n \psi(x)$ 对于所有 $x \in G_f$ 和所有 $n \in \mathbf{Z}$；
(b) $G$ 中存在$e$ 的开邻域 $V$，使得$\psi|V$ 是单射指数映射的逆映射。
(iii) 映射 $\psi$ 是解析性的。

存在$G$的开子群，它与标准群（no. 3，定理4）同构的。 断言 (i) 然后从引理 1 得出。

设$U$是$L(G)$的开子群，$\phi : U \to \phi(U)$是$G$的指数映射，具有no. 2的命题3的性质。可以假设$U$对于$\phi(U) \subset G_f$来说足够小。让$x \in G_f$。存在$m \in \mathbf{Z} - \{0\}$使得$x^m \in \phi(U)$。 元素 $\frac{1}{m} \phi^{-1}(x^m)$ 不依赖于 $m$ 的选择。让 $m' \in \mathbf{Z}$ 等于 $x^{m'} \in \phi(U)$。然后 $x^{m m'} \in \phi(U)$ 和
$$
m' \phi^{-1}(x^m) = \phi^{-1}(x^{m m'}) = m \phi^{-1}(x^{m'})
$$
从而我们的断言。让$\psi(x) = \frac{1}{m} \phi^{-1}(x^m)$。然后$\psi|\phi(U) = \phi^{-1}$。另一方面，如果$n \in \mathbf{Z}$，那么
$$
\psi(x^n) = \frac{1}{m} \phi^{-1}(x^{nm}) = \frac{n}{m} \phi^{-1}(x^m) = n \psi(x).
$$

因此$\psi$具有命题的性质(a)和(b)。 $x$中的邻域中，$\psi$由映射$x \mapsto x^m$、$y \mapsto \phi^{-1}(y)$和$z \mapsto \frac{1}{m} z$组成；因此 $\psi$ 是对 $G_f$ 的解析。

最后，令$\psi'$为$G_f$的映射进入$L(G)$和$V'$$G_f$中$e$的邻域，使得$\psi'(x^n) = n \psi'(x)$代表$x \in G_f$和$n \in \mathbf{Z}$，并且$\psi'|V'$是单射指数映射的逆映射。然后是$e$的邻域$W$上的$\psi$和$\psi'$重合。如果$x \in G_f$，则存在$n \in \mathbf{Z}$使得$x^n \in W$。然后
$$
n \psi'(x) = \psi'(x^n) = \psi(x^n) = n \psi(x)
$$
因此$\psi = \psi'$。

#### 定义 2 {#lie-iii-s7-def-2 .statement tag=0AHL}

*命题 10 的映射 $\psi$ 称为 $G$ 的对数映射，并用 $\log_G$ 或简称为 $\log$ 表示。*

#### 命题 11 {#lie-iii-s7-prop-11 .statement tag=0AHM}

*假设$p \neq 0$。令$x, y$是$G_f$的两个可置换的元素。然后是$xy \in G_f$和$\log(xy) = \log x + \log y$。*

事实上，$xy \in G_f$源自引理 1。设$U$是加法群$L(G)$的开子群，$\phi : U \to \phi(U)$是$G$的指数映射，具有命题 3的性质no. 2；可以假设$U$足够小，使$\log|\psi(U)|$成为$\phi$的倒数映射。对于$n \in \mathbf{Z} - \{0\}$，适当选择$x^n \in \phi(U)$、$y^n \in \phi(U)$。让$u = \log x^n$，$v = \log y^n$，从而$x^n = \phi(u)$，$y^n = \phi(v)$。 公式 (2)，$[u, v] = 0$。 Hausdorff 公式则证明 $\phi(\lambda(u + v)) = \phi(\lambda u) \phi(\lambda v)$ 对于 $|\lambda|$ 足够小；因此，对于每个足够大整数 $i$，
$$
\phi(p^i(u + v)) = \phi(p^i u) \phi(p^i v)
$$
那就是
$$
p^i (\log x^n + \log y^n) = \log(x^{np^i} y^{np^i})
$$
或
$$
np^i (\log x + \log y) = np^i \log(xy).
$$

#### 命题 12 {#lie-iii-s7-prop-12 .statement tag=0AHN}

*假设$p \neq 0$。让$x \in G_f$。以下条件是等效的：
（一）$\log x = 0$；
(ii) $x$ 在 $G$ 中具有有限的阶。*

如果存在整数$n > 0$使得$x^n = e$，则有
$$
n \log x = \log x^n = 0,
$$
从而$\log x = 0$。如果$\log x = 0$，则令$V$为$G_f$中$e$的邻域，使得$\log|V|$是单射指数映射的倒数映射。存在整数$n > 0$使得$x^n \in V$； 等式 $\log x^n = 0$ 意味着 $x^n = e$。

#### 命题 13 {#lie-iii-s7-prop-13 .statement tag=0AHO}

*假设$p \neq 0$。如果 $G$ 是紧凑型或标准型，则 $G_f = G$.*

如果G是标准的，则使用引理1就足够了。假设G是紧的。令$x \in G$和V为G中e的邻域。令y为序列$(x^n)_{n \geq 0}$的极限点。对于所有$n > 0$，存在两个整数$n_1, n_2$，例如$n_1 \geq 2n_2 \geq n$和$x^{n_1} \in yV, x^{n_2} \in yV$、从而、$x^{n_1 - n_2} \in V^{-1}V$和$n_1 - n_2 \geq n$。因此$x \in G_f$。

#### 推论 {#lie-iii-s7-n6-cor-1 .statement tag=0AHP}

*假设K是局部紧的。那么 $G_f$ 就是 G 的紧致子群的并。*

让$x \in G$。如果 x 属于为 G 的紧子群，则$x \in G_f$ (命题 13)。假设$x \in G_f$。由于 K 是局部紧致的，因此存在紧致 G 的开子群 $G_1$。那么存在整数$m > 0$使得$x^m \in G_1$。由$x^m$生成的闭子群$G_2$包含在$G_1$中，因此是紧致的。然后x与$G_2$的元素交换，因此$G_2 \cup xG_2 \cup \cdots \cup x^{m-1}G_2$是G的紧子群，其中包含x。

#### 例 {#lie-iii-s7-n6-exa-1 .statement tag=0AHQ}

假设 K 是局部紧致的。令U为A的可逆元的集合；它是李群 $K^*$ 的紧凑型开放子群。然后$U \subset (K^*)_f$乘命题13；另一方面，如果$x \in K^*$使得$x \notin U$，则当n趋向于$+\infty$时$x^n$趋于0，或者当n趋于$-\infty$时$x^n$趋于0；因此$U = (K^*)_f$。 函数 $\log_{K^*}$ 在 U 上定义和解析，值在 $L(K^*) = K$ 中，并且使得 $\log_{K^*}(xy) = \log_{K^*}(x) + \log_{K^*}(y)$ 对于 U 中的所有 $x, y$； U 的元素 x，使得 $\log_{K^*}(x) = 0$ 是 K 的单位元的根。

我们再次使用记号 。 3、4 和 5。

#### 命题 14 {#lie-iii-s7-prop-14 .statement tag=0AHR}

*假设$p \neq 0$和v被选择使得$v(p) = 1$。令 G 为 G 的指数函数（或 G 的对数函数）的标准群和 E(X)（或 L(X)）展开作为关于 0 的积分级数。*

(i) *绝对收敛域*（可微分和解析流形，R，4.1.3）*E 包含集合 $\Delta$ 的 $x \in G$ 使得 $\omega(x) > \frac{1}{p-1}$。让$E'$表示由这个级数在$\Delta$上定义的映射。那么$E'$是G的指数映射，并且是流形$\Delta$自身的同构。*

(ii) *L包含G的绝对收敛域。令$L'$表示由级数定义的G上的映射。那么$L'$是G的对数映射，$L'$到$\Delta$的限制是$E'$的倒数映射。*

(iii) *映射 $E'$ 是 $\Delta$ 的同构，通过 Hausdorff 律，到 G 的子群 $\Delta$。*

使用记号或 § 5，编号。 3 和 4、$E = \sum_{m \geq 1} \frac{\psi_{m,m}}{m!}$（$§ 5$、no. 4、命题 3）。作为系数 $c_{\alpha \beta \gamma}$ 属于到 A，$\| \psi_{m,m} \| \leq 1$（可微分和解析流形，R，附录）$K^r$ 假定有范数

$$
\| (\lambda_1, \ldots, \lambda_r ) \| = \sup(|\lambda_1|, \ldots, |\lambda_r|)
$$

章II, § 8, no. 1、引理1、$v(m!) \leq \frac{m-1}{p-1}$。如果$\omega(x) > \frac{1}{p-1}$，我们看到$m \omega(x) - v(m!)$趋于$+\infty$，$m$，从而
$$
\left\| \frac{\psi_{m,m}}{m!} \right\| \|x\|^m \leq \frac{1}{|m!|} \|x\|^m
$$
当 $m$ 趋于 $+\infty$ 时，它趋于 0，并且
$$
\omega\left( \frac{\psi_{m,m}(x)}{m!} \right) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1} \quad \text{for } m \geq 1.
$$
因此$\Delta$包含在$E$和$E'(\Delta) \subset \Delta$的绝对收敛域内。显然 $E'$ 是指数映射。

如果$L_m$表示次数$m$的$L$齐次分量，§ 5, no. 4的命题3，证明$L_m$的每个系数都是形式
$$
a_1 + \frac{1}{2} a_2 + \cdots + \frac{1}{m} a_m
$$
$a_1, a_2, \ldots, a_m$ 位于 $A$；但是
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) = o(\log m) \quad \text{as } m \text{ tends to } +\infty
$$
和
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) \geq v\left( \frac{1}{m!} \right) \geq -\frac{m-1}{p-1}.
$$
因此，如果$\omega(x) > 0$，$\|L_m\| \cdot \|x\|^m$趋于0，就像$m$趋于$+\infty$一样，从而$G$包含在$L$的绝对收敛域内。另一方面，如果$\omega(x) > \frac{m}{p-1}$，则$\omega(L_m(x)) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1}$对应$m \geq 1$，因此$L'(\Delta) \subset \Delta$。

由于*可微解析流形*的形式幂级数 $L(E(X))$和$E(L(X))$等于$X$、no. 4.1.5，R证明：
$$
L'(E'(x)) = E'(L'(x)) = x
$$
$x \in \Delta$。因此，$E'$是流形$\Delta$自身的同构，逆同构是$L'$到$\Delta$的限制。

$L(X^{[n]}) = nL(X)$ $n$ 整数 $> 0$ (cf. § 5, no. 4)。由于$G$包含在$L$和$X^{[n]}$的绝对收敛域中，因此$L'(x^n) = nL'(x)$对于所有$x \in G$。 关系 $L'|_{\Delta} = {E'}^{-1}$ 意味着 $L'(x^n) = \log x^n$ 对应 $n$ 足够大。因此$L'(x) = \log x$。这样我们就证明了(i)和(ii)。

令$H = \sum_{r,s \geq 0} H_{r,s}$为豪斯多夫形式幂级数，$h$为相对于$L(G)$的豪斯多夫函数。 $\tilde{H}$ 包含于 $\Delta \times \Delta$ 和 $h$ 的绝对收敛域定义在 $\Delta \times \Delta$ (章 II, § 8, 命题 2) 上。然后
$$
E'(x)E'(y) = E'(h(x, y))
$$
对于 $x, y$ 足够接近 0 ($§ 4$, 定理 4 (v))。因此，在no. 3、定义 1 的记号中，形式上的幂、级数、$F(E(X), E(Y))$和$E(H(X, Y))$是相等的。令 $x, y$ 为 $\Delta$ 中的元素。然后
$$
\sup_m \left| \frac{\psi_{m,m}}{m!} \right| (\sup \|x\|, \|y\|)^m < 1 \\
\sup_{r,s} \|H_{r,s}\| \|x\|^r \|y\|^s < |\rho|^{1/(p-1)}
$$
由章 II, § 8、公式 (14)。通过*可微分和解析流形*，R，4.1.5，$E'(x)E'(y)$是通过用$x$代替$X$和$y$代替$Y$获得
$$
F(E(X), E(Y))
$$
$E'(h(x, y))$是通过将$E(H(X, Y))$中的$X$替换为$x$、将$Y$替换为$y$而得到。因此$E'(x)E'(y) = E'(h(x, y))$。

### 习题 {#lie-iii-s7-exercises}

参见[习题为 § 7](exercises/s7/)。
