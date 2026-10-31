---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 2
section_title: Identity element; cancellable elements; invertible elements
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 12-24, 126-129
pdf_pages: 0036-0048, 0150-0153
extraction: ocr
subsections:
    - "no": 1
      title: IDENTITY ELEMENT
      page: 12
      pdf_page: 36
    - "no": 2
      title: CANCELABLE ELEMENTS
      page: 14
      pdf_page: 38
    - "no": 3
      title: INVERTIBLE ELEMENTS
      page: 15
      pdf_page: 39
    - "no": 4
      title: MONOID OF FRACTIONS OF A COMMUTATIVE MONOID
      page: 17
      pdf_page: 41
    - "no": 5
      title: 'APPLICATIONS: I. RATIONAL INTEGERS'
      page: 20
      pdf_page: 44
    - "no": 6
      title: 'APPLICATIONS: II. MULTIPLICATION OF RATIONAL INTEGERS'
      page: 22
      pdf_page: 46
    - "no": 7
      title: 'APPLICATIONS: III. GENERALIZED POWERS'
      page: 23
      pdf_page: 47
    - "no": 8
      title: NOTATION
      page: 23
      pdf_page: 47
statements: 26
exercises: 17
content_sha256: cd164eb049a877336000d5dfcea021595a703af78ac84c06f999b3a0e5a83714
translated_from: content/en/alg/I/02_s2_identity_element_cancellable_elements.md
translation_method: google
source_content_sha256: 4e4d1e772eb5f248a858ce2f9c1dbddee958a8fa5c19120df031143b30855c75
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: bc647597dd984860af355cc6acc5499bd8eb7afbea6526cc0f9e0aa381f4b83b
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。 单位元素；可取消元素； 可逆元

### 1.单位元素

#### 定义 1 {#alg-i-s2-def-1 .statement tag=056M}

Under a law of composition $\top$ on a set $E$ an element $e$ of $E$ is called an identity element if, for all $x \in E$, $e \top x = x \top e = x$.

给定律$\top$下最多存在一个单位元素，因为如果$e$和$e'$是单位元素，则$e = e \top e' = e'$。 单位元素对于每个元素都是可置换的：它是中心元素。

#### 定义 2 {#alg-i-s2-def-2 .statement tag=056N}

单位元素的岩浆称为单一岩浆。如果$E, E'$是单一岩浆，则将岩浆$E$的同态转化为岩浆$E'$，其中$E$的映射单位元素到$E'$的单位元素称为单一同态（或态射）的$E$转化为$E'$。联合单位岩浆称为幺半群。

如果$E, E'$是幺半群，则$E$到$E'$的单位态射称为幺半群同态或$E$到$E'$的幺半群态射。

#### 例 {#alg-i-s2-n1-exa-1 .statement tag=056O}

(1) 在自然数的集合$\mathbf{N}$中，0是加法下的单位元素，1是乘法下的单位元素。这两个律中的每一个都给出$\mathbf{N}$一个可交换幺半群结构（集合理论，III, § 3, no. 3）。

(2) 在集合$E$子集集合中，$\varnothing$是律$\cup$下的单位元素和律$\cap$下的$E$。更一般地，在格子中，最小元素（如果存在）是单位元素在律之下；反之，如果在该律下存在单位元素，则它是集合中最小的元素。对于最大元素和律 inf 也是如此。

(3) 集合 $\mathbf{N}$ 在律 $(x, y) \mapsto x^y$ 下没有单位元素。在律$(X, Y) \mapsto X \circ Y$下$E \times E$子集之间，对角的$\Delta$为单位元素。在律$(f, g) \mapsto f \circ g$下，$E$的映射到$E$恒等映射的$E$到$E$之间是单位元素。

（4）设$E$为岩浆，$E$上的$R$等价关系与$E$（§ 1, no. 6）上的律兼容。 如果$E/R$中$e$是$E$的单位元素，$e$的典范像就是岩浆$E/R$的单位元素。

单位岩浆的单位元素是单位同态；两个单位同态的合成也是一。对于映射是单位岩浆同构来说，它是双射单位同态是必要且充分的，并且逆映射是单位同态。令$E$和$E'$为单一岩浆，$e'$单位元素为$E'$； $E$到$E'$映射$E$到$e'$的常数映射是单位同态，称为平凡同态。

单一岩浆族（或幺半群）的乘积是单一岩浆（或幺半群）。

单位岩浆（或幺半群）的每个商岩浆都是单位岩浆（或幺半群）。

令$E$为单一岩浆，$e$为单位元素。 $E$的子岩浆$A$使得$e \in A$被称为$E$的单一子岩浆。显然 $e$ 是岩浆 $A$ 的单位元素。每交 $E$ 的单位子岩浆都是 $E$ 的单位子岩浆。如果$X$是$E$的子集，则存在$E$包含$X$的最小的单一子岩浆；称为$X$生成的$E$单一次岩浆；如果 $X$ 为空，则它等于 $\{e\}$。如果$E$是幺半群，则$E$的单位次岩浆称为$E$的子幺半群。

如果$F$是没有单位元素的岩浆，则$F$的子岩浆可能拥有单位元素。对于例，如果 $F$ 是结合律且 $h$ 是 $F$ (I, § 1, no. 4) 的幂等元素，则 $h \uparrow x \uparrow h$ 的集合（其中 $x$ 穿过 $F$）是$F$的次岩浆，$h$为单位元素。

如果 $E$ 是具有单位元素 $e$ 的岩浆，则 $E$ 的子岩浆 $A$ 使得 $e \notin A$ 可能仍拥有单位元素。

#### 定义 3 {#alg-i-s2-def-3 .statement tag=056P}

令 $E$ 为单一岩浆。 $E$的单位元素称为$E$元素空族的合成。

如果$(x_\alpha)_{\alpha \in \varnothing}$是E的元素的空族，则其合成$e$也用$\prod_{\alpha \in \varnothing} x_\alpha$表示。对于例，我们写
$$
\prod_{q \leq i \leq p} x_i = e
$$
当$p < q$（$p, q \in \mathbf{N}$）时。类似地，我们将任意 $x$ 写为 $\prod^0 x = e$。 *使用这些定义定理 1 和 3 § 1 保持为真，如果假设集合 A 和 B_i 非空被抑制。* 类似地，公式 $\prod^{m+n} x = \left( \prod^m x \right) \prod^n \left( \prod^n x \right)$ 和 $\prod^{mn} x = \prod^m \left( \prod^n x \right)$ 对于 $m \geq 0, n \geq 0$ 也为真。

令 E 为单一岩浆，其律表示为 $\top$，$e$ 表示为单位元素。 E 的元素家​​庭$(x_i)_{i \in I}$ 的*支持*是指标 $i \in I$ 的集合，使得$x_i \neq e$。令$(x_i)_{i \in I}$是E*与有限支撑*的元素的族。以下两种情况我们应定义合成$\prod_{i \in I} x_i$：

(a) 集合 I 全序；
(b) E 是结合律，并且 $x_i$ 是成对可置换的。

在这两种情况下，令 S 为家庭的支持$(x_i)$。如果 J 是 I 包含 S 的有限子集，则 $\prod_{i \in J} x_i = \prod_{i \in S} x_i$，如 J 中元素的数上的归纳所示，在情况 (a) 中，应用定理 1 为 § 1，并且在情况 (b) 中，定理 3 / § 1。令$\prod_{i \in I} x_i$表示合成$\prod_{i \in J} x_i$的公共的值，对于I包含S的所有有限子集。当I是$\mathbf{N}$的区间$[p, \to]$时，我们也写$\prod_{i = p}^\infty x_i$。

有了这些定义和记号，§ 1和注中的定理 1和3，继定理 3 扩展之后，送给有限支撑的家庭。

*加法*书写的律的单位元素通常用0表示，称为*零*或*空元素*（或有时*原点*）。在律写作*乘法*时，通常用1表示并称为*单位元*（或*单位*）。

### 2.可取消元素

#### 定义 4 {#alg-i-s2-def-4 .statement tag=056Q}

*给定集合 E 上的合成 $\top$ 律，E 的映射 $x \mapsto a \top x$（或 $x \mapsto x \top a$）自身被称为元素 $a \in E$ 的左翻译（或右翻译）。*

在经过到相反的律，左翻译变成右翻译，反之亦然。

令$\gamma_a, \delta_a$（或$\gamma(a), \delta(a)$）表示$a \in E$的左右平移；然后
$$
\gamma_a(x) = a \top x, \qquad \delta_a(x) = x \top a.
$$

#### 命题 1 {#alg-i-s2-prop-1 .statement tag=056R}

*如果律* $\mathsf{T}$ *是结合律，则对于所有* $x \in E$ *和* $y \in E$

$$
\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y, \qquad \delta_{x \mathsf{T} y} = \delta_y \circ \delta_x.
$$

对于所有$z \in E$：

$$
\gamma_{x \mathsf{T} y}(z) = (x \mathsf{T} y) \mathsf{T} z = x \mathsf{T} (y \mathsf{T} z) = \gamma_x(\gamma_y(z))
$$
$$
\delta_{x \mathsf{T} y}(z) = z \mathsf{T} (x \mathsf{T} y) = (z \mathsf{T} x) \mathsf{T} y = \delta_y(\delta_x(z))
$$

其他字、映射$x \mapsto \gamma_x$是同态从$E$到集合$E$的映射的$E^E$与律自身结合$(f, g) \mapsto f \circ g$； 映射 $x \mapsto \delta_x$ 是 $E$ 的同态变成集合 $E^E$ 与相反的律。如果 $E$ 是幺半群，则这些同态是单位的。

#### 定义 5 {#alg-i-s2-def-5 .statement tag=056S}

*元素* $a$ *岩浆* $E$ *如果左（或右）平移* $a$ *是单射的，则称为左（或右）可取消（或常规）。左右可取消元素称为可取消（或常规）元素。*

在其他字中，为了使$a$在律$\mathsf{T}$下可消去，关系$a \mathsf{T} x = a \mathsf{T} y, x \mathsf{T} a = y \mathsf{T} a$中的每一个都暗示$x = y$是必要且充分的（据说这些等式中的每一个都“可以消去a”）。如果律$\mathsf{T}$下存在单位元素$e$，则在该律下可以取消：$\gamma_e$和$\delta_e$的翻译就是$E$的恒等映射自身。

#### 例 {#alg-i-s2-n2-exa-1 .statement tag=056T}

(1) 每自然数可在加法下取消；每自然数$\neq 0$均可在乘法下取消。

(2) 在一个格子中，除了单位元素（至少元素）之外，律sup下不能有可取消的元素（如果存在的话）；同样对于 inf。特别是集合$E$子集集合，$\varnothing$是律$\cup$下唯一可取消的元素，而$E$是元素下唯一可取消的元素律$\cap$。

#### 命题 2 {#alg-i-s2-prop-2 .statement tag=056U}

*可取消的集合（左可取消，右可取消）元素关联岩浆是子岩浆。*

如果 $\gamma_x$ 和 $\gamma_y$ 是单射的，那么 $\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y$ (命题 1) 也是单射的。对于 $\delta_{x \mathsf{T} y}$ 也是如此。

### 3.可逆元

#### 定义 6 {#alg-i-s2-def-6 .statement tag=056V}

*设*$E$*为单一岩浆，$\mathsf{T}$其合成的律，e其单位元素和*$x$*和*$x'$**$E$的两个元素。 $x'$ *被称为* $x$ *if* $x' \mathsf{T} x = e$ *（或$x \mathsf{T} x' = e$，或$x' \mathsf{T} x = x \mathsf{T} x' = e$）的左逆（或右逆，或逆）。*

*元素* $x$ *of* $E$ *如果它有左逆（或右逆、或逆），则称为左可逆（或右可逆、或可逆）。*

*所有元素可逆的幺半群称为群。*

对称和可对称使用有时代替逆和可逆。当E上的律写成加法时，我们通常说负数而不是逆数。

#### 例 {#alg-i-s2-n3-exa-1 .statement tag=056W}

(1) 单位元素是它自己的逆元。

(2) 在 E 的映射的集合到 E 元素中，如果 f 是满射（或单射），则 f 是左可逆的（或右可逆的）。左逆（或右逆）则为与 f（集合理论、II, § 3, no. 8、定义 11）关联的退化（或截面）。为了使 f 可逆，f 为双射是充分必要的。那么它的唯一逆元就是 f 的逆双射。

设 E 和 F 是两个单位岩浆，f 是 E 到 F 中的单位同态。如果 x' 是 E 中 x 的逆，f(x') 是 F 中 f(x) 的逆。因此，如果 x 是 E 的可逆元，则 f(x) 是 F 的可逆元。

In particular, if R is an equivalence relation compatible with the law on a unital magma E, the canonical image of an invertible element of E is invertible in E/R.

#### 命题 3 {#alg-i-s2-prop-3 .statement tag=056X}

设 E 为幺半群，且 x 元素为 E。

(i) 为了使 x 左（或右）可逆，x 的右（或左）平移是满射的是必要且充分的。

(ii) 对于 x 可逆，它是左可逆和右可逆的充分必要条件。在这种情况下，x 有一个唯一的逆元，这也是其唯一的左（或右）逆元。

如果 x' 是 x 的左逆，则 (命题 1)

$$
\delta_x \circ \delta_{x'} = \delta_{x' \top x} = \delta_e = \mathrm{Id}_E
$$

且 $\delta_x$ 是满射。相反，如果$\delta_x$是满射，则存在E的元素$x'$，使得$\delta_x(x') = e$和$x'$是$x$的左逆元。 (i) 的其他断言类似。

如果$x'$（或$x''$）是$x$的左（或右）逆，则

$$
x' = x' \top e = x' \top (x \top x'') = (x' \top x) \top x'' = e \top x'' = x'',
$$

从而（二）。

#### 注 {#alg-i-s2-n3-rem-1 .statement tag=056Y}

设 E 为幺半群，x 元素为 E。如果 x 是可逆的，则它是可取消的；因为，如果 $x'$ 是 $x$ 的左逆，那么

$$
\gamma_{x'} \circ \gamma_x = \gamma_{x' \top x} = \gamma_e = \mathrm{Id}_E
$$

且 $\gamma_x$ 是单射的。特别是，如果 x 是左可逆的，则 x 的左右平移是双射的。相反，假设 $\gamma_x$ 是双射；存在$x' \in E$使得$xx' = \gamma_x(x') = e$；那么 $\gamma_x(x'x) = (xx')x = x = \gamma_x(e)$ 进而$x'x = e$，因此 x 是可逆的。我们类似地看到，如果 $\delta_x$ 是双射的，则 x 是可逆的。

#### 命题 4 {#alg-i-s2-prop-4 .statement tag=056Z}

设 E 为幺半群，E 的 x 和 y 可逆元分别具有逆 x' 和 y'。那么 y' $\top$ x' 是 x $\top$ y 的倒数。

这是从关系得出的
$$
(y' \top x') \top (x \top y) = y' \top (x' \top x) \top y = y' \top y = e
$$
以及 (x $\top$ y) $\top$ (y' $\top$ x') 的类似计算。

#### 推出 1 {#alg-i-s2-prop-4-cor-1 .statement tag=0570}

设 E 为幺半群；如果 E 的元素的有序序列 $(x_\alpha)_{\alpha \in A}$ 的每个元素 $x_\alpha$ 都有一个逆 $x'_\alpha$，合成 $\prod_{\alpha \in A} x_\alpha$ 都有逆 $\prod_{\alpha \in A'} x'_\alpha$，其中 A' 是通过替换从 A 导出的全序集阶在 A 上，与对面的阶相接。

该推论由 A 中元素的数上的命题 4 通过归纳得出。

特别是，如果 x 和 x' 是倒数，则对于每个整数 $n \geq 0$，$\prod^n x$ 和 $\prod^n x'$ 都是倒数。

#### 推出 2 {#alg-i-s2-prop-4-cor-2 .statement tag=0571}

在幺半群中，集合可逆元是稳定的。

#### 命题 5 {#alg-i-s2-prop-5 .statement tag=0572}

如果在幺半群中 x 和 x' 互逆并且 x 与 y 交换，那么 x' 也是如此。

从$x \top y = y \top x$，我们推导出$x' \top (x \top y) \top x' = x' \top (y \top x) \top x'$，从而推导出$(x' \top x) \top (y \top x') = (x' \top y) \top (x \top x')$，即$y \top x' = x' \top y$。

#### 推出 1 {#alg-i-s2-prop-5-cor-1 .statement tag=0573}

令 E 为幺半群，E 的 X 子集以及 X' X 的中心化器。 X' 属于到 X' 的每个可逆元的逆。

#### 推出 2 {#alg-i-s2-prop-5-cor-2 .statement tag=0574}

在幺半群中，中心可逆元的逆是中心元素。

### 4. 交换幺半群的分数幺群

在这个数中，e 表示幺半群的单位元素，x* 表示 E 的可逆元 x 的逆。

令 E 为可​​交换幺半群，E 的 S 子集和由 S 生成的 E 的 S' 子幺半群。

#### 引理 1 {#alg-i-s2-lem-1 .statement tag=0575}

在 E $\times$ S' 关系 R$\mathscr{R}$x, y$\mathscr{R}$ 中定义为：

“存在$a, b \in E$和$p, q, s \in S'$使得$x = (a, p), y = (b, q)$和$aqs = bps$”

等价关系与乘积幺半群 E $\times$ S' 上的律兼容。

R 是自反且对称的，即直接的。令$x = (a, p), y = (b, q)$和$z = (c, r)$为E$\times$S'的元素，使得R$\mathscr{R}$x，y$\mathscr{R}$和R$\mathscr{R}$y，z$\mathscr{R}$成立。那么存在 S' 的两个元素 s 和 t 使得
$$
aq s = bps, \quad br t = cqt,
$$
从而由此可见
$$
ar(stq) = bpsrt = cp(stq)
$$

因此，对于 $stq$ 属于到 $S'$，$R \{ x, z \}$ 成立。因此关系 $R$ 是及物性的。

此外，令$x = (a, p), y = (b, q), x' = (a', p'),$和$y' = (b', q')$为$E \times S'$的元素，使得$R \{ x, y \}$和$R \{ x', y' \}$成立。 $S'$中存在$s$和$s'$使得
$$
aqs = bps, \qquad a'q's' = b'p's',
$$
从而由此得出$(aa')(qq')(ss') = (bb')(pp')(ss')$，因此$R \{ xx', yy' \}$ 代表$ss' \in S'$。因此，等价关系 $R$ 与$E \times S'$ 上的合成的律兼容。

商 magma $(E \times S')/R$ 是一个交换幺半群。

#### 定义 7 {#alg-i-s2-def-7 .statement tag=0576}

*令$E$为可交换幺半群，$E$的$S$子集和由$S$生成的$E$的$S'$子幺半群。商幺半群$(E \times S')/R$，其中等价关系$R$如引理1中所述，用$E_S$表示，称为$E$的分数†的幺半群，与$S$相关（或与$S$).*

对于$(a, p)$模$R$的$a \in E$和$p \in S'$类，一般用$a/p$表示，称为分子$a$分母$p$的分数。然后到定义$(a/p).(a'/|p') = aa'/|pp'$。 分数$a/p$和$a'/|p'$相等当且仅当$S'$和$spa' = sp'a$中存在$s$；如果是，则$S'$中存在$\sigma$和$\sigma'$，以及$a\sigma = a'\sigma'$和$p\sigma = p'\sigma'$。特别是，$a \in E$对应$a/p = sa/sp$，$S'$对应$s, p$。 $E_S$的单位元素是分数$e/e$。

让$a/e = \varepsilon(a)$代表所有$a \in E$。上式表明，$\varepsilon$是$E$到$E_S$的同态，称为规范。对于所有$p \in S'$、$(p/e).(e/p) = e/e$，因此$e/p$是$\varepsilon(p) = p/e$的逆；因此 $\varepsilon(S')$ 的每个元素都是可逆的。然后$a/p = (a/e).(e/p)$，从而
$$
a/p = \varepsilon(a)\varepsilon(p)^*
$$
对于$a \in E$和$p \in S'$，幺半群$E_S$因此由$\varepsilon(E) \cup \varepsilon(S)^*$生成。

#### 命题 6 {#alg-i-s2-prop-6 .statement tag=0577}

*记号是定义 7 的值，$\varepsilon$ 表示$E$ 到$E_S$ 的典范同态。
(i) 设$a$和$b$在$E$中；在阶、$\varepsilon(a) = \varepsilon(b)$中，存在$s \in S'$和$sa = sb$是充分必要的。
(ii) 要使 $\varepsilon$ 成为单射，$S$ 中的每个元素都可以取消是必要且充分的。
(iii) 要使 $\varepsilon$ 成为双射，$S$ 的每个元素都是可逆的。*

断言 (i) 很清楚，表明$\varepsilon$是单射的当且仅当$S'$的每个元素都是可取消的；但由于$E$的可取消的元素的集合是$E$的子幺半群(no. 2，命题2)，所以说$S$的每个元素都是可取消的。

† 如果 $E$ 上的律是相加的，则也称为“差异幺半群”。

如果$\varepsilon$是双射的，S的每个元素都是可逆的，因为$\varepsilon(S)$由$E_S$的可逆元组成。相反，假设 S 的每个元素都是可逆的；那么$S'$的每个元素都是可逆的（no. 3，推论2到命题4），因此可以取消。那么 $\varepsilon$ 被 (ii) 内射，$a/p = \varepsilon(a.p^*)$ 被 (1) 内射，因此 $\varepsilon$ 是满射。

#### 定理 1 {#alg-i-s2-thm-1 .statement tag=0578}

*设 E 为可交换幺半群，E 的 S 子集，$E_S$ 与 S 相关的分数幺半群以及$\varepsilon : E \to E_S$ 典范同态。进一步令 f 为 E 的同态成为幺半群 F（不一定可交换），使得 $f(S)$ 的每个元素在 F 中都是可逆的。存在且仅有一个 $E_S$ 的同态 $\bar{f}$ 到 F 中，使得 $f = \bar{f} \circ \varepsilon$。*

如果 $\bar{f}$ 是 $E_S$ 的同态到 F 中，使得 $f = \bar{f} \circ \varepsilon$，则
$$
\bar{f}(a/p) = \bar{f}(\varepsilon(a)\varepsilon(p)^*) = \bar{f}(\varepsilon(a))\bar{f}(\varepsilon(p))^* = f(a)f(p)^*
$$
对于 $a \in E$ 和 $p \in S'$，从而唯一性 $\bar{f}$。

令 g 为 $E \times S'$ 的映射到由 $g(a,p) = f(a)f(p)^*$ 定义的 F 中。我们证明 g 是 F 中 $E \times S'$ 的同态。首先，
$$
g(e,e) = f(e)f(e)^* = e.
$$
令$(a,p)$和$(a',p')$为$E \times S'$中的两个元素；如$a'$和$p$在E通勤，$f(a')$和$f(p)$在F通勤，从而$f(a')f(p)^* = f(p)^*f(a')$经no. 3，命题5。此外$f(pp')^* = f(p'p)^* = (f(p')f(p))^* = f(p)^*f(p')^*$经no. 3， 命题 4、从而
$$
g(aa',pp') = f(aa')f(pp')^* = f(a)f(a')f(p)^*f(p')^* = f(a)f(p)^*f(a')f(p')^*
= g(a,p)g(a',p').
$$
我们证明 g 在 $E \times S'$ 上与等价关系 R 相容的：如果 $(a,p)$ 和 $(a',p')$ 是全等的 mod。 R，存在$s \in S'$和$spa' = sap'$，从而$f(s)f(p)f(a') = f(s)f(a)f(p')$。由于$f(s)$是可逆的，因此$f(p)f(a') = f(a)f(p')$，然后向左乘法乘$f(p)^*$，向右乘法乘$f(p')^*$
$$
g(a',p') = f(a')f(p')^* = f(p)^*f(a) = f(a)f(p)^* = g(a,p).
$$
因此，F 中存在 $E_S$ 的同态 $\bar{f}$，使得 $\bar{f}(a/p) = g(a,p)$，从而 $\bar{f}(\varepsilon(a)) = \bar{f}(a/e) = f(a)f(e)^* = f(a)$。因此$\bar{f} \circ \varepsilon = f$。

#### 推论 {#alg-i-s2-n4-cor-1 .statement tag=0579}

*设E和F是两个可交换幺半群，S和T分别是E和F的子集，E的f同态进入F，使得$f(S) \subset T$和$\varepsilon : E \to E_S, \eta : F \to F_T$典范同态。存在且仅有一个同态 $g : E_S \to F_T$ 使得 $g \circ \varepsilon = \eta \circ f$。*

E 的同态 $\eta \circ f$ 到 S 的每元素到 $F_T$ 的 $F_T$ 映射到可逆元。

#### 注 {#alg-i-s2-n4-rem-1 .statement tag=057A}

(1) 定理 1 也可以用说表示，对于 E，$(E_S, \varepsilon)$ 是普遍映射问题的解，相对于幺半群，E 的幺半群同态和同态转化为幺半群， S 的映射元素到可逆元（*集合理论*、IV、、no. 1）。由此可见 (*loc.cit.*)，这个问题中的所有其他解以独特的方式同构于 $(E_S, \varepsilon)$

(2) 对于解对于上述普遍映射问题的存在性，无需假设幺半群E是可交换的，由*集合理论*可知，IV, § 3, no. 2(cf.习题17)。

我们提到了分数幺半群的两个重要特例。

(a) 设 $\overline{E} = E_E$。 As the monoid $\overline{E}$ is generated by the set $\varepsilon(E) \cup \varepsilon(E)^*$, which is composed of invertible elements, every element of $\overline{E}$ is invertible (no. 3, Corollary 2 to Proposition 4). 在其他字中，$\overline{E}$是可交换的群。 此外，通过定理 1，E 到群 G 中的每一个同态 $f$ 都可以在形式 $f = \bar{f} \circ \varepsilon$ 中唯一因式分解，其中 $\bar{f}: \overline{E} \to G$ 是同态。 $\overline{E}$ 称为 * E 的分数的 *群（或者在加法记号的情况下，称为 * E 的差的 *群）。

(b) 设$\Phi = E_{\Sigma}$，其中$\Sigma$由E的可取消元素组成。由命题6，(ii)，E的典范同态到$\Phi$是单射的； 认同 E 的像 $\Phi$ 将会有利可图。因此E是$\Phi$的子幺半群，E的每个可取消的元素在$\Phi$都有一个逆，$\Phi$的每个元素是形式$a/p = a.p^*$以及$a \in E$和$p \in \Sigma$；那么$a/p = a'/p'$当且仅当$ap' = pa'$。容易看出，$\Phi$的可逆元为分数$a/p$，其中$a$和$p$可取消，$p/a$是$a/p$的逆。

现在令 S 为 E 的可取消元素的集合，$S'$ 为 S 生成的 E 的子幺半群。如果 $a/p$ 和 $a'/p'$ 是 $E_S$ 的两个元素，则 $a/p = a'/p'$ 当且仅当 $ap' = pa'$ （对于$sap' = spa'$ 意味着所有 $s \in S'$ 都有 $ap' = pa'$）。因此，$E_S$可以被识别为$E \cup S^*$生成的$\Phi$的子幺半群。

如果E的每个元素都是可取消的，则$\Phi = \overline{E}$和E是交换性群$\Phi$的子幺半群。相反，如果E与群的子幺半群同构，则E的每个元素都是可取消的。

### 5. 应用：I。理性整数

考虑自然数的交换幺半群 $\mathbf{N}$ 和律合成加法；在此律下，$\mathbf{N}$ 的所有元素均可取消（*集合理论*、III, § 5, no. 2、推论 3）。 $\mathbf{N}$之差群记为$\mathbf{Z}$；它的元素称为*有理整数*；它的律称为有理整数*的*加法，也用+表示。 从$\mathbf{N}$到$\mathbf{Z}$的典范同态是单射的，我们将$\mathbf{N}$的每个元素认同及其在$\mathbf{Z}$中的像。 $\mathbf{Z}$的元素由定义等价类确定，在$\mathbf{N} \times \mathbf{N}$中由关系在$(m_1, n_1)$和$(m_2, n_2)$之间确定，写为$m_1 + n_2 = m_2 + n_1$； $\mathbf{N}$的元素$m$与元素$(m + n, n)$的类由……组成进行识别，其中$n \in \mathbf{N}$；它承认元素$(n, m + n)$的$\mathbf{Z}$类为负。 $\mathbf{N} \times \mathbf{N}$的每个元素$(p, q)$如果$p \geq q$可以写在形式$(m + n, n)$中，如果$p \leq q$则可以写在形式$(n, m + n)$中；由此可见，$\mathbf{Z}$是$\mathbf{N}$的*并，以及集合是$\mathbf{N}$*的元素的负数。 The identity element 0 is the only element of $\mathbf{N}$ whose negative belongs to $\mathbf{N}$.

对于每个自然数$m$，$-m$表示$m$的负有理数整数，$-\mathbf{N}$表示$m \in \mathbf{N}$的元素$-m$的集合。然后

$$
\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N}) \quad \text{and} \quad \mathbf{N} \cap (-\mathbf{N}) = \{0\}.
$$

对于$m \in \mathbf{N}$，$m = -m$当且仅当$m = 0$。

设$m$和$n$为两个自然数；

(a) 如果$m \geq n$，则$m + (-n) = p$，其中$p$是$\mathbf{N}$的元素，使得$m = n + p$；
(b) 如果$m \leq n$，则$m + (-n) = -p$，其中$p$是$\mathbf{N}$的元素，使得$m + p = n$；
(c) $(-m) + (-n) = -(m + n)$。

性质 (b) 和 (c) 由no. 3、命题 4 得出；如$\mathbf{N}$中的$\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$、加法以及属性(a)、(b)和(c)完整地描述了$\mathbf{Z}$中的加法。

更一般地，$-x$ 用于表示任意有理数整数 $x$ 的负数； 合成 $x + (-y)$ 缩写为 $x - y$ (cf. no. 8)。

自然数之间的序关系$\leq$具有以下性质的特征：$m \leq n$当且仅当存在整数$p \in \mathbf{N}$使得$m + p = n$（*集合理论*，III, § 3, no. 6，命题 13 和 § 5, no. 2、命题 2)。有理数整数$x$和$y$之间的关系$y - x \in \mathbf{N}$是$\mathbf{Z}$上的*总计阶*关系，其中$\mathbf{N}$上的扩展序关系$\leq$。对于，对于所有$x \in \mathbf{Z}$，$x - x = 0 \in \mathbf{N}$；如果$y - x \in \mathbf{N}$和$z - y \in \mathbf{N}$，那么

$$
z - x = (z - y) + (y - x) \in \mathbf{N},
$$

对于$\mathbf{N}$在加法下是稳定的；如果$y - x \in \mathbf{N}$和$x - y \in \mathbf{N}$，则$y - x = 0$，因为0是$\mathbf{N}$中唯一的元素，其负属于到$\mathbf{N}$；对于任意有理数整数 $x$ 和 $y$、$y - x \in \mathbf{N}$ 或 $x - y \in \mathbf{N}$，对于 $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$；最后，如果$x$和$y$是自然数，则$y - x \in \mathbf{N}$当且仅当存在$p \in \mathbf{N}$使得$x + p = y$。这个序关系也用$\leq$表示。

从此以后，当 $\mathbf{Z}$ 被认为是有序的集合时，它总是，否则会提到除非，根据刚刚定义的排序，自然数被标识为整数 $\geq 0$；它们也被称为*正*整数； 整数 $\leq 0$，正整数的负数，称为*负数* 整数； 整数 $> 0$（分别为 $< 0$）被称为*严格正数*（分别为*严格负数*）； 整数$> 0$中的集合是有时，用$\mathbf{N}^*$表示。

设$x$、$y$、$z$为三个有理数整数；那么 $x \leq y$ 当且仅当 x + z \leq y + z。对于 x - y = (x + z) - (y + z)。这个性质用说表示，$\mathbf{Z}$上的序关系在平移下是不变的。

### 6. 应用：II。有理数乘法整数

#### 引理 2 {#alg-i-s2-lem-2 .statement tag=057B}

设 E 为幺半群，且 E 的 x 元素。
    (i) E 中存在 $\mathbf{N}$ 的唯一同态 f，对于所有$n \in \mathbf{N}$，$f(1) = x$ 和 $f(n) = \frac{n}{1} x$。
    (ii) 如果 x 可逆，则 E 中存在 $\mathbf{Z}$ 的唯一同态 g，使得 $g(1) = x$ 和 g 重合，且 f 在 $\mathbf{N}$ 上。

    为所有$n \in \mathbf{N}$、公式写$f(n) = \frac{n}{1} x$
    $$
    \frac{0}{1} x = e \quad \text{and} \quad \left( \frac{m}{1} x \right) \cdot \left( \frac{n}{1} x \right) = \frac{m+n}{1} x
    $$
    (no. 1) 将f 是$\mathbf{N}$ 的同态的事实表达到E 中，显然是$f(1) = x$。如果$f'$是将$\mathbf{N}$的同态代入E，使得$f'(1) = x$，则$f = f'$乘以§ 1, no. 4，命题1，(iv)。

现在假设 x 是可逆的。根据no. 3，推论2到命题4，$f(n) = \frac{n}{1} x$对于每个整数$n \geq 0$都是可逆的。通过构造，$\mathbf{Z}$ 是 $\mathbf{N}$ 之差的群，因此 (no. 4, 定理 1) f 扩展与 $\mathbf{Z}$ 的同态 g 唯一到 E。如果 $g'$ 是$\mathbf{Z}$的同态与$g'(1) = x$进入E，$g'$至$\mathbf{N}$的限制$f'$是$\mathbf{N}$的同态与$f'(1) = x$进入E。因此$f' = f$，从而$g' = g$。

    我们将引理 2应用于幺半群E为$\mathbf{Z}$的情况；因此，对于每个整数$m \in \mathbf{Z}$，都存在$\mathbf{Z}$的自同态$f_m$，其特征为$f_m(1) = m$。如果m在$\mathbf{N}$，$\mathbf{N}$的映射$n \mapsto mn$进入$\mathbf{N}$是岩浆$\mathbf{N}$的自同态（集合理论，III, § 3, no. 3，推论到命题5）；因此$f_m(n) = mn$对于$\mathbf{N}$中的所有$m, n$。

    因此，$\mathbf{N}$上的乘法可以通过$\mathbf{Z}$中的$m, n$的公式$mn = f_m(n)$延长至$\mathbf{Z}$上的乘法。我们将建立公式：

    (2) $$ xy = yx $$
    (3) $$ (xy)z = x(yz) $$
    (4) $$ x(y+z) = xy + xz $$
    (5) $$ (x+y)z = xz + yz $$
    (6) $$ 0.x = x.0 = 0 $$
    (7) $$ 1.x = x.1 = x $$
    (8) $$ (-1).x = x.(-1) = -x $$

对于 $\mathbf{Z}$ 中的 $x, y, z$。 （*在其他字中，$\mathbf{Z}$是交换环。*）公式$x(y+z) = xy + xz$和$x.0 = 0$表示$f_x$是加性幺半群$\mathbf{Z}$的自同态，$f_x(1) = x$可以写成$x.1 = x$。 $\mathbf{Z}$ 映射 1 到 $xy$ 的自同态 $f_x \circ f_y$，因此等于 $f_{xy}$、从而 (3)。现在$f_x(-y) = -f_x(y)$，即$x(-y) = -xy$；类似地，$\mathbf{Z}$映射 1 到$-x$的自同态$y \mapsto -xy$，从而$(-x).y = -xy$因此
$$
(-x)(-y) = -(x(-y)) = -(-xy) = xy.
$$
对于$\mathbf{N}$中的$m, n$、$mn = nm$（集合理论、III, § 3, no. 3、命题5的推论）、从而$(-m).n = n(-m)$和$(-m)(-n) = (-n)(-m)$；作为 $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$、$xy = yx$ 对应 $\mathbf{Z}$ 中的 $x, y$；这个公式意味着(5)由(4)引出并完成公式(6)到(8)的证明。

### 7. 应用：III。广义幂

令 E 为幺半群，其中单位元素 $e$ 和合成的律表示为 $\top$。如果 $x$ 在 E 中可逆，则令 $g_x$ 为 $\mathbf{Z}$ 的同态到 E 映射 1 到 $x$。让$g_x(n) = \frac{n}{\top} x$代表所有$n \in \mathbf{Z}$；到引理 2 为止，此记号与 $n \in \mathbf{N}$ 和之前介绍的记号兼容。然后
$$
\begin{align*}
\text{(9)} \quad & \frac{m+n}{\top} x = \left( \frac{m}{\top} x \right) \top \left( \frac{n}{\top} x \right) \\
\text{(10)} \quad & \frac{0}{\top} x = e \\
\text{(11)} \quad & \frac{1}{\top} x = x
\end{align*}
$$
对于 $x$ 在 E 中可逆，$m, n$ 在 $\mathbf{Z}$ 中可逆。进一步，如果$\mathbf{Z}$入E的$y = \frac{m}{\top} x$、映射$n \mapsto g_x(mn)$为同态映射1到$y$、从而$g_x(mn) = g_y(n)$，则
$$
\text{(12)} \quad \frac{mn}{\top} x = \frac{n}{\top} \left( \frac{m}{\top} x \right).
$$
由于$-1$是$\mathbf{Z}$中1的负数，$\frac{-1}{\top} x$是E中$x = \frac{1}{\top} x$的倒数。如果我们在(9)中写出$n = -m$，则可见$\frac{-m}{\top} x$是$\frac{m}{\top} x$的倒数。

### 8.记号

(a) 作为一般规则，可交换幺半群的律是可加写的。因此，约定$-x$表示$x$的负数。 记号 $x + (-y)$ 缩写为 $x - y$ 类似
$$
x + y - z, \quad x - y - z, \quad x - y + z - t, \quad \text{etc. . . .}
$$
分别代表
$$
x + y + (-z), \quad x + (-y) + (-z), \quad x + (-y) + z + (-t), \quad \text{etc. . . .}
$$

对于 $n \in \mathbf{Z}$ 记号 $\overset{n}{\top} x$ 替换为 $nx$。 公式 (9) 到 (12) 则变为

(13) $$
(m + n).x = m.x + n.x
$$
(14) $$
0.x = 0
$$
(15) $$
1.x = x
$$
(16) $$
m.(n.x) = (mn).x
$$

其中$m$和$n$属于到$\mathbf{N}$，或者如果$x$承认负数，甚至到$\mathbf{Z}$。在后一种情况下，关系$(-1).x = -x$也成立。我们还有注公式

(17) $$
n.(x + y) = n.x + n.y.
$$

(b) 令 E 为乘法写成的幺半群。对于 $n \in \mathbf{Z}$ 记号 $\overset{n}{\top} x$ 替换为 $x^n$。我们有关系

$$
x^{m+n} = x^m.x^n \\
x^0 = 1 \\
x^1 = x \\
(x^m)^n = x^{mn}
$$

如果 $x$ 和 $y$ 通勤，则还有 $(xy)^n = x^ny^n$。

当$x$有逆元时，这正是$x^{-1}$。也使用记号$\frac{1}{x}$代替$x^{-1}$。最后，当幺半群E可交换时，$\frac{x}{y}$或$x/y$也可用于$xy^{-1}$。

### 习题 {#alg-i-s2-exercises}

§ 2](exercises/s2/)参见[习题。
