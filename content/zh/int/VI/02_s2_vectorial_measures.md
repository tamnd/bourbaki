---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 2
section_title: Vectorial measures . "
lang: zh
source: int-i-vi
book_pages: INT VI.18-INT VI.40, INT VI.62-INT VI.69
pdf_pages: 0409-0431, 0453-0460
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a vectorial measure
      page: 18
      pdf_page: 409
    - "no": 2
      title: Integration with respect to a vectorial measure
      page: 20
      pdf_page: 411
    - "no": 3
      title: Majorizable vectorial measures
      page: 22
      pdf_page: 413
    - "no": 4
      title: Vectorial measures with base $\mu$
      page: 25
      pdf_page: 416
    - "no": 5
      title: The Dunford–Pettis theorem
      page: 27
      pdf_page: 418
    - "no": 6
      title: Dual of the space $L^1_F$ (F a separable Banach space)
      page: 32
      pdf_page: 423
    - "no": 7
      title: Integration of a vector-valued function with respect to a vectorial measure
      page: 33
      pdf_page: 424
    - "no": 8
      title: Complex measures
      page: 34
      pdf_page: 425
    - "no": 9
      title: Bounded complex measures⁶
      page: 37
      pdf_page: 428
    - "no": 10
      title: Image of a complex measure; induced complex measure; product of complex measures\footnote{Cf. Ch. V, §6, No. 4; Ch. IV, §5, No. 7 and Ch. V, §7; Ch. III, §4 and Ch. V, §8, Nos. 2–5.}
      page: 39
      pdf_page: 430
statements: 42
exercises: 27
content_sha256: fe3cae52bc56b849738530e8e4211a08c515642da48c975c1e323718a003901e
translated_from: content/en/int/VI/02_s2_vectorial_measures.md
translation_method: google
source_content_sha256: f78c02d6746badeb5841481f1c8cf6849e885db53fc5c1bf28fc919724113c17
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 222718c96f0c9912147077695b468cb0c2f68a85e083f94f66d4141138d8109c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 2。矢量测量

### 1. 矢量测量的定义

定义中给出的措施。 III, §1, No. 3可以概括如下：

#### 定义 1 {#int-vi-s2-def-1 .statement tag=09A3}

*设 F 是 R 上的 Hausdorff 局部凸空间。我们将 F 中的每个连续线性映射的空间 $\mathscr{K}(T)$ 称为 T 上的矢量测度，其中 F 中的值到 F 中。*

定义。 1 也可以表示为：F 中的值的 T 上的向量测度是 $\mathscr{K}(T)$ 到 F 中的线性映射 m，使得对于 T 的每个紧凑子集 K，m 到 $\mathscr{K}(T, K)$ 的限制对于一致收敛的拓扑是连续的。如果$f \in \mathscr{K}(T)$，还可以写$\int f dm$或$\int f(t)\,dm(t)$，而不是$m(f)$。 $\mathbf{R}$ 中带有值的度量为有时，称为 *真实* 度量（第 III, §1, No. 5）或 T 上的 *标量* 度量。

#### 例 {#int-vi-s2-n1-exa-1 .statement tag=09A4}

— 1) $\mathscr{K}(T)$ 的恒等映射是 T 上的矢量测度，值位于 $\mathscr{K}(T)$ 中。

2) *设H为复数希尔伯特空间，$\mathscr{L}(H)$H的连续自同态的范数代数。设A为$\mathscr{L}(H)$的子代数，可交换、闭、自伴且包含恒等式；证明在X上连续复形函数的代数$\mathscr{K}_\mathbf{C}(X) = \mathscr{C}_\mathbf{C}(X)$上存在规范代数A的紧空间X和同构，配备范数 $\|f\| = \sup_{x \in X} |f(x)|$。 逆同构，仅限于 $\mathscr{K}(X)$，是 X 上的矢量测度 m，其中值在 $\mathscr{L}(H)$ 中，使得 $m(fg) = m(f)m(g)$.*_

#### 注 {#int-vi-s2-n1-rem-1 .statement tag=09A5}

— 1) 为了使 $\mathscr{K}(T)$ 的线性映射 m 成为 F 中的向量测度，对于 T 的每个紧凑子集 K，像在单位球 $\|f\| \leq 1$ 的 $\mathscr{K}(T, K)$ 的 m 下，有界于 F 中是有界的。因此，F 中具有值的矢量测度的概念对于 F 上允许相同有界集合的所有 Hausdorff 局部凸拓扑是相同的，特别是对于与 F 和 F' 之间的对偶性兼容的所有拓扑（TVS，IV, §1, No. 1，命题 1）。

2) 令$T_1$为局部紧致空间，$F_1$为$\mathbf{R}$上的Hausdorff局部凸空间，u为$\mathscr{K}(T_1)$的连续线性映射入$\mathscr{K}(T)$，v为F的连续线性映射入$F_1$。如果 m 是 T 上的矢量测度，F 中的值，则 $v \circ m \circ u$ 是 $T_1$ 上的矢量测度，$F_1$ 中的值。特别是，如果 g 是 T 上的连续有限数值函数，则 $f \mapsto m(gf)$ 是 T 上的向量测度，F 中的值表示为 $g \cdot m$；如果 h 是 T 上的第二个连续有限数值函数，则 $g \cdot (h \cdot m) = (gh) \cdot m$。

3) 由于空间 $\mathscr{K}(T)$ 是 Banach 空间 $\mathscr{K}(T, K)$ 的直极限，并且特别是桶装（TVS、III, §4, No. 1、第 2 条命题的 Cor. 和第 3 条命题的 Cor. 3），在阶中， F 中 $\mathscr{K}(T)$ 的线性映射 m 是矢量测度，对于每个 $z' \in F'$，$z' \circ m$ 是 T 上的标量测度是必要且充分的（TVS，II, §6, No. 4，第 5 条命题和IV, §1, No. 3，第 7 条命题）。

4) 鉴于注 1，第 1 章命题 1。 III, §2, No. 1 及其证明对于矢量测量再次有效。因此，可以将 T 上的向量测度 m 的 *支持* 定义设为最大的开集合 $U \subset T$ 的补集，使得 m 对 U 的限制为零。

### 2. 关于矢量测量的积分

令 $m$ 为 $T$ 上的矢量测度，值为 $F$。对于每个 $z' \in F'$，映射 $z' \circ m$ 是 $T$ 上的标量度量，线性依赖于 $z'$。如果 $f$ 是在 $T$ 上定义的数字函数，我们会滥用语言说，对 $(f, m)$ 有性质 $P$，如果对于每个 $z' \in F'$，对 $(f, |z' \circ m|)$有性质$P$。例如，如果对于每个$z' \in F'$，函数$f$对于$|z' \circ m|$本质上可积，我们可以说$f$对于*$m$本质上是可积的。同样的道理，$f$ 本质上对于$(z' \circ m)^+$ 和$(z' \circ m)^-$ 的每一个测度都是可积的（第 V, §2, No. 2 章，第 3 条命题第 2 条）。

#### 命题 1 {#int-vi-s2-prop-1 .statement tag=09A6}

*令 $m$ 为 $T$ 上的矢量测度，$F$ 中的值，$f$ $T$ 上的数值函数，本质上可积为 $m$。 映射*
$$
z' \mapsto \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-
$$
*是线性形式于 $F'$*。

用$\Phi$表示这个映射，对于所有$\lambda \in \mathbf{R}$来说，$\Phi(\lambda z') = \lambda \Phi(z')$就是直接的。一切都归结为展示$\Phi(y' + z') = \Phi(y') + \Phi(z')$。 集合$\mu = |y' \circ m| + |z' \circ m|$；根据Lebesgue–Nikodym 定理，可以写出$y' \circ m = g \cdot \mu$和$z' \circ m = h \cdot \mu$，其中$g$和$h$是两个有界且局部$\mu$可积的数值函数（Ch.V, §5, No. 5，Th.2）；此外，$(y' \circ m)^+ = g^+ \cdot \mu$和$(y' \circ m)^- = g^- \cdot \mu$，以及类似的关系保持，其中$y'$被$z'$（分别$y' + z'$）替换，$g$被$h$（分别$g + h$）替换。既然如此，$f$本质上是$\mu$可积的直接的（第V, §2, No. 2章，第3命题Cor.1），并且关系需要证明约化到$(g + h)^+ - (g + h)^- = (g^+ - g^-) + (h^+ - h^-)$，这是显而易见的。

#### 定义 2 {#int-vi-s2-def-2 .statement tag=09A7}

*令 $m$ 为 $T$ 上的矢量测度，值为 $F$，$f$ 为 $T$ 上的数值函数，本质上可积为 $m$。称$f$相对于$m$的积分，并用$m(f)$或$\int f \, dm$表示，或者又用*定义的$\int f(t) \, dm(t)$、元素表示${F'}^*$

$$
\langle z', \int f \, dm \rangle = \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-.
$$

我们观察到，如果$f \in \mathscr{K}(T)$，元素$\int f \, dm$如此定义重合，元素在No. 1中同样表示，因为（1）的第二个成员是$\int f \, d(z' \circ m) = z'(m(f))$乘以定义。此外，如果特别是应用 Def. 2 对于 $F = \mathbf{R}$ 的情况，我们可以看出，对于每一个 $z' \in F'$，f 本质上对于实测度 $z' \circ m$ 是可积的，并且 (1) 的第二个成员可以写成 $\int f d(z' \circ m)$。

现在假设$f$本质上可积为$m$，并令$z' \in F'$。 集合$\mu = |z' \circ m|$；根据Lebesgue–Nikodym 定理，我们可以写出$z' \circ m = g \cdot \mu$，其中$g$是局部$\mu$可积且$\|g\| \leq 1$，并且第1条命题的证明表明$\int f d(z' \circ m) = \int fg d\mu$。因而，

$$
\left| \int f d(z' \circ m) \right| \leq \int |f| d|z' \circ m|.
$$

很明显，有限数值函数对于$m$本质上可积的集合在$\mathbf{R}$上是向量空间；我们将用$\mathscr{L}(m)$来表示这个空间配备了最粗糙的局部凸拓扑，使所有线性形式$f \mapsto \int f d(z' \circ m)$连续，其中$z'$运行超过$F'$。请注意，一般来说，局部凸空间 $\mathscr{L}(m)$ *不是 Hausdorff*。

#### 例 {#int-vi-s2-n2-exa-1 .statement tag=09A8}

— 让我们将 $\mathscr{K}(T)$ 的 $m$ 恒等映射代入其自身。由于 $\mathscr{K}(T)$ 的对偶是 $T$ 上标量测量的空间 $\mathscr{M}(T)$，因此函数 $f \in \mathscr{L}(m)$ 本质上是对*每个*标量测量 $\mu$ (cf. Exer. 1) 可积的那些，并且积分$\int f dm$ 是线性形式 $\mu \mapsto \int f d\mu$ $\mathscr{M}(T)$。一个不能对于每一个度量$\mu \in \mathscr{M}(T)$除非$f = 0$都有$\int f d\mu = 0$，就像在取$\mu = \varepsilon_t$时看到的那样，其中$t$在$T$中是任意的；在其他字中，映射$f \mapsto \int f dm$是$\mathscr{L}(m)$的*单射*到$\mathscr{M}(T)$的代数对偶，其中扩展恒等映射是$\mathscr{K}(T)$。因此，关系 $\int f dm \in F = \mathscr{K}(T)$ 相当于$f \in \mathscr{K}(T)$。

令 $u$ 为 $F$ 的连续线性映射成为 Hausdorff 局部凸空间 $G$，并让我们通过将${F'}^*$ 的线性映射双转置为 $u$ 再次表示其扩张为${G'}^*$（§ 1, No. 1）。有了这个约定：

#### 命题 2 {#int-vi-s2-prop-2 .statement tag=09A9}

*每个数值函数* $f$ *本质上可积* $m$ *本质上可积* $u \circ m$、*和* $\int f d(u \circ m) = u(\int f dm)$。

考虑到所有 $y \in G'$ 的等式 $y' \circ u \circ m = {}^t u(y') \circ m$，命题是显而易见的。

一般来说，如果$f \in \mathscr{L}(m)$，$\int f dm$属于积分到${F'}^*$，但不积分到$F$（参见上面的*例*）。然而：

#### 命题 3 {#int-vi-s2-prop-3 .statement tag=09AA}

*如果像位于* $m$ *的集合的* $f \in \mathscr{K}(T)$ *使得* $\sup_{t \in T} |f(t)| \leq 1$ *在* $F$ 中弱相对紧致，*则* $\int f dm \in F$ *对于每个有界数值函数* $f$ *基本上可积分* $m$。

令$A$为$f \in \mathscr{L}(m)$的集合，使得$\sup_{t \in T} |f(t)| \leq 1$，并令$B = A \cap \mathscr{K}(T)$；由假设可知，$m(B)$在$F$中是弱相对紧的，因此只要证明对于拓扑$\sigma({F'}^*, F')$，$m(A)$包含在$m(B)$的闭包中（在${F'}^*$中）；由于$m(B)$是凸且平衡的，只需证明$F'$中$m(B)$的极点包含在$m(A)$的极点中（TVS，II, §6, No. 3，Th.1）。现在，对于线性形式$z' \in F'$到属于到$(m(B))^\circ$，对于每个函数$g \in B$，$|\langle z', m(g)\rangle| = |\int g d(z'\circ m)| \leq 1$是充分必要的，这意味着标量测度$|z'\circ m|$是有界的并且是范数 $\leq 1$（第III, §1, No. 8）；但通过（2），后者条件意味着$|\langle z', m(f)\rangle| \leq 1$对于每个函数$f \in A$，从而$z' \in (m(A))^\circ$。

#### 推论 1 {#int-vi-s2-prop-3-cor-1 .statement tag=09AB}

*如果，对于 T 的每个紧致子集 K，像在 $f \in \mathscr{H}(T, K)$ 的集合的 m 之下，使得 $\sup_{t \in T} |f(t)| \leq 1$ 在 F 中是弱相对紧致，则 $\int f dm \in F$ 对于每个有界且具有紧支撑的函数 $f \in \mathscr{L}(m)$，并且每函数 $f \in \mathscr{L}(m)$ $\int f dm \in F''$。*

第一个断言可以立即从命题3推导出来：如果$f$有界并且具有紧支撑，并且如果U是$f$支撑的相对紧开邻域，则$m$到子空间$\mathscr{H}(U)$的限制是$m_U$的测度U满足第3条的条件和$\int f dm_U = \int f dm$（第V, §7, No. 1，Th.1），因此$\int f dm \in F$。

现在让 $f$ 为 $\mathscr{L}(m)$ 中的任意元素；对于 T 的每个紧凑子集 K 和每个整数 $n > 0$，令 $f_{n,K}$ 为 T 上的数值函数，定义如下： if $t \notin K$, $f_{n,K}(t) = 0$；如果$t \in K$和$|f(t)| \leq n$，$f_{n,K}(t) = f(t)$；最后，如果$t \in K$和$|f(t)| > n$，则$f_{n,K}(t) = nf(t)/|f(t)|$。 很明显，对于每个 $t \in T$，$f(t)$ 是 $f_{n,K}(t)$ 相对于 Fréchet 滤波器的乘积滤波器和 T 的紧凑子集（递增有向）有序集的分段滤波器的限制。 从$|f_{n,K}| \leq |f|$开始，它遵循勒贝格的定理和第10章第10条命题。 V, §1, No. 3，应用于每个标量度量$|z'\circ m|$，$f_{n,K}$相对于前面的过滤器在$\mathscr{L}(m)$中收敛到$f$。 因而，整的$\int f dm$位于$m(f_{n,K})$的集合M的${F'}^*$（对于拓扑$\sigma({F'}^*, F')$）的闭包中。 但推论的第一个部分表明$M \subset F$，另一方面，对于每个$z' \in F'$，都有$|\langle z', m(f_{n,K})\rangle| \leq \int |f| d|z'\circ m|$，这表明M有界于$F_\sigma$，因此也在F中（TVS，IV, §1, No. 1，命题1）。 因而，§1, No. 2的引理1表明$\int f dm \in F''$。

#### 推论 2 {#int-vi-s2-prop-3-cor-2 .statement tag=09AC}

*如果 F 是半自反的，则对于每个数值函数 $f$ $\int f dm \in F$ 本质上可积为 $m$。*

### 3. 主要向量测量

令$q$为F上的下半连续半范数。我们将用$z' \in F'$的$A'_q$集合表示，使得$|\langle z', x\rangle| \leq q(x)$对于所有$x \in F$。这是

$x \in F$ 集合的$F'$ 极点使得 $q(x) \leq 1$；对于每$x \in F$，
$$
q(x) = \sup_{z' \in A'_q} |\langle x, z' \rangle|.
$$

#### 定义 3 {#int-vi-s2-def-3 .statement tag=09AD}

*令 $m$ 为 $T$ 上的向量测度，值为 $F$ 中的向量测度。如果 $q$ 是 $F$ 上的下半连续半范数，并且存在正测度 $\mu$ 使得对于每个 $z' \in A'_q$ 都有 $|z' \circ m| \leq \mu$，则 $m$ 被称为 *q-可大化*；当 $z'$ 超过 $A'_q$（第 III, §2, No. 4，第 3 章）时，$|z' \circ m|$ 的上限值表示为 $q(m)$。有人说，如果对于$F$上的每个连续半范数$q$来说，$m$是*可大化的*，那么它是*q-可大化的*。

如果 $m$ 和 $m'$ 都是 *q-大调*，则直接的 $m + m'$ 也是 *q-大调* 并且
$$
q(m + m') \leq q(m) + q(m').
$$

当 $F$ 是规范的空间时，范数表示为 $|x|$，因此说 $m$ 是可大化的，因此意味着度量 $|z' \circ m|$（其中 $|z'| \leq 1$）在 $^1$ 之上受到相同的正度量的限制；则用 $|m|$ 表示这一系列测度的最高值。

如果$F = \mathbf{R}$，则$\mathbf{R}$重合上的措施$|m|$相应的到欧氏范数$|x|$以及第1章中的$|m|$表示的措施。 III, §1, No. 5。

#### 命题 4 {#int-vi-s2-prop-4 .statement tag=09AE}

*设* $(F_i)_{1 \leq i \leq n}$ *为Hausdorff局部凸空间、$F = \prod_{i=1}^n F_i$的有限族，它们的乘积、$q_i$ ($1 \leq i \leq n$) *$F_i$上的下半连续半范数*，*和* $q$ *半范数* $F$ *由* $q(x_1, \ldots, x_n) = \sum_{i=1}^n q_i(x_i)$ 定义。 *如果* $m_i$ ($1 \leq i \leq n$) *是对* $T$ *与值在* $F_i$ *即* $q_i$*-可极大化*的矢量测量，*则测量* $m = (m_1, \ldots, m_n)$ *与值在* $F$ *是* *q-大调*。

因为，对偶$F'$可以用$\prod_{i=1}^n F_i'$来识别，这样如果$x = (x_i) \in F$，$z' = (z_i') \in F'$，则$\langle x, z' \rangle = \sum_{i=1}^n \langle x_i, z_i' \rangle$。如果对每个$x \in F$都有$|\langle x, z' \rangle| \leq q(x)$，那么特别是对$1 \leq i \leq n$有$|\langle x_i, z_i' \rangle| \leq q_i(x_i)$，逆命题是明显的，这表明集合$A'_q$是$A'_{q_i}$的乘积。由于假设 $|z_i' \circ m_i| \leq q_i(m_i)$ 对于 $z_i' \in A'_{q_i}$，因此可以得出：
$$
|z' \circ m| \leq \sum_{i=1}^n |z_i' \circ m_i| \leq \sum_{i=1}^n q_i(m_i)
$$
对于每个$z' \in A'_q$，这证明了命题。

$^1$ 专业人士。

#### 推论 {#int-vi-s2-n3-cor-1 .statement tag=09AF}

— *如果空间 F 是有限维的，则 F 中具有值的每个向量测度 m 都是可大化的。在阶中，数值函数对于m本质上可积，它对于|m|*本质上可积是必要且充分的（其中|x|表示F上的任何范数）。

#### 命题 5 {#int-vi-s2-prop-5 .statement tag=09AG}

— *设 q 为 F 上的下半连续半范数。设 m 为 q 可极大化测度，设 f 为函数，对于 m 本质上可积，且$\int f dm \in F$。然后*

$$
q\left( \int f dm \right) \leq \int^\bullet |f| dq(m).
$$

对于，

$$
q\left( \int f dm \right) = \sup_{z' \in A'_q} \left| \langle z', \int f dm \rangle \right| \leq \sup_{z' \in A'_q} \int |f| d|z' \circ m| \leq \int^\bullet |f| dq(m)
$$

凭借（1）和关系$|z' \circ m| \leq q(m)$对于$z' \in A'_q$。

#### 命题 6 {#int-vi-s2-prop-6 .statement tag=09AH}

— *令 F 为准完备、Hausdorff 局部凸空间，m 是 T 上的可大化测度，F 中包含值。如果 f 是对于所有测度 q(m) 本质上可积的数值函数（其中 q 超过 F 上连续半范数的集合），则 f 本质上对于 m 可积，并且$\int f dm \in F$。

我们将利用以下辅助结果。令 $(\mu_\iota)_{\iota \in I}$ 为 T 上递增有向测度族。让我们用 T 上有限数值函数的 $\mathscr{L}^1((\mu_\iota)_{\iota \in I})$ 向量空间表示，本质上对于每个 $\iota \in I$ $\mu_\iota$ 可积，配备由半范数 $f \mapsto \mu_\iota(|f|)$ 定义的拓扑 （$\iota \in I$）。令$\mathscr{L}_0$为乘积$g \varphi_K$生成的$\mathscr{L}^1((\mu_\iota)_{\iota \in I})$的线性子空间，其中g运行于T上连续有限数值函数的集合，并且K运行于T的紧致子集的集合。

#### 引理 1 {#int-vi-s2-lem-1 .statement tag=09AI}

— *当$\mathscr{L}_0$和$\mathscr{K}(T)$配备由$\mathscr{L}^1((\mu_\iota)_{\iota \in I})$诱发的拓扑时：
a) $\mathscr{L}_0$的每个元素都在$\mathscr{K}(T)$的某个有界子集的闭包中；
b) $\mathscr{L}^1((\mu_\iota)_{\iota \in I})$ 的每个元素都位于 $\mathscr{L}_0$ 的某个有界子集的闭包中。*

为了证明a)，我们可以将自己限制在形式$f = g \varphi_K$($g \in \mathscr{C}(T)$)的元素的情况，K紧缩在T)中。 直接的（凭借Urysohn的定理），$f$位于形式$gh$的函数的集合B闭包中，其中h将T的连续映射的集合描述为$[0,1]$，在 K 上等于 1，在 K 的固定紧邻域 H 的补集上等于 0。此外，集合 B 是有界的，因为$\mu_\iota(|gh|) \leq \mu_\iota(|f\varphi_H|)$ 对于每个函数 h 都具有前述属性。

现在让我们证明 b);我们可以将自己限制在元素$f \geq 0$或$\mathscr{L}^1((\mu_\iota)_\iota \in I)$的情况。对于每个$\iota \in I$和每个$\varepsilon > 0$，都存在T的紧子集$K(\iota, \varepsilon)$，使得$f$到$K(\iota, \varepsilon)$的限制是连续的并且$|\mu_\iota(|f - f\varphi_{K(\iota, \varepsilon)}|)| \leq \varepsilon$。很明显，$f$处于$f\varphi_{K(\iota, \varepsilon)}$的集合C闭包中（其中$\iota \in I,\ \varepsilon > 0$）。凭借Urysohn的定理，$\mathscr{L}_0$中包含集合C；此外，它是有界的，因为$\mu_\kappa(f\varphi_{K(\iota, \varepsilon)}) \leq \mu_\kappa(f)$对于所有$\iota \in I,\ \kappa \in I$和$\varepsilon > 0$。

现在让我们证明命题6：对于每个函数$g \in \mathscr{K}(T)$和F上的每个连续半范数q，$q\left( \int g\,dm \right) \leq \int |g|\,d(q(m))$（命题5），这意味着当$\mathscr{K}(T)$配备了$\mathscr{L}^1((q(m))_{q \in Q})$的拓扑（Q是F上的连续半范数的集合）时，$\mathscr{K}(T)$到F的映射$g \mapsto \int g\,dm$是连续的。 因而，根据前面的引理和TVS的第10条命题III, §1, No. 6，这个映射可以通过连续性进行扩展，首先将$\mathscr{L}_0$的连续线性映射$v_0$延伸到F中，然后将$\mathscr{L}^1((q(m))_{q \in Q})$的连续线性映射$v$延伸到F中。 此外，对于每个$z' \in F'$关系$\langle z', v(f) \rangle = \int f\,d(z' \circ m)$成立，通过$v$的定义，对于每个$f \in \mathscr{K}(T)$；由于$|z' \circ m| \leq q(m)$对于$q(z) = |\langle z', z \rangle|$，映射$f \mapsto \int f\,d(z' \circ m)$在$\mathscr{L}^1((q(m))_{q \in Q})$上是连续的，因此再次根据连续性，关系$\langle z', v(f) = \int f\,d(z' \circ m)$对于每个函数$f \in \mathscr{L}^1((q(m))_{q \in Q})$成立。 接下来是$v(f) = \int f\,dm$，从而完成证明。

### 4. 使用基 $\mu$ 进行矢量测量

#### 定义 4 {#int-vi-s2-def-4 .statement tag=09AJ}

*令 $\mu$ 为 T 上的正测度。T 上的矢量测度 $m$，F 中为值，如果存在 T 到 F 中的映射 $f$，则称其为具有基 $\mu$ 的测度，且可在局部标量 $\mu$ 可积，使得每函数 $g \in \mathscr{K}(T)$ $m(g) = \int gf\,d\mu$。然后有人说$f$是$m$相对于$\mu$的密度，有人写为$m = f \cdot \mu$。*

直接的，如果$f_1$和$f_2$是$m$相对于$\mu$的两个密度，那么$f_1 - f_2$在局部标量$\mu$可忽略不计（第V, §5, No. 3，第3条的Cor.2）；回想一下，一般来说，这并不意味着$f_1 - f_2$在几乎所有地方都是零（cf.§1，Exer.12和No. 1，*注2*）。

令 $m$ 为基 $\mu$ 与密度 $f$ 的测度。对于数值函数 $g$ 对于 $m$ 本质上可积，$gf$ 本质上是 $\mu$ 标量可积是必要且充分的（Ch. V, §5, No. 3，Th. 1）。

#### 命题 7 {#int-vi-s2-prop-7 .statement tag=09AK}

— 令 $f$ 为映射对于 $T$ 上的正测度 $\mu$ 可以在局部标量可积，这样，对于每一个函数 $g \in \mathscr{K}(T)$，都有 $\int gf\,d\mu \in F$。那么$\mathscr{K}(T)$到$F$的映射$g \mapsto \int gf\,d\mu$是$T$上的矢量测度，基$\mu$和密度$f$相对于$\mu$。

对于 (No. 1, 注 3)，只需证明设定 $m(g) = \int gf\,d\mu$、$z' \circ m$ 是每个 $z' \in F'$ 的标量测度。但从$z'(m(g)) = \int g\langle z', f \rangle\,d\mu$开始，一个人就有了$z' \circ m = \langle z', f \rangle \cdot \mu$，从而我们的断言。

#### 命题 8 {#int-vi-s2-prop-8 .statement tag=09AL}

— 设$\mu$为$T$的正测度，$m$为$T$的测度，值为$F$，基$\mu$和密度$f$关于$\mu$。令$q$为$F$的下半连续半范数。

a) 如果对于$T$的每个紧致子集$K$，上积分$\int_K^*(q \circ f)\,d\mu$是有限的，则$m$是$q$可大化的。

b) 如果$m$是$q$可大化的，那么$q(m)$有基$\mu$；如果在加法 $f$ 中，$\mu$ 可测为 $T$ 的映射到 $F_\sigma$，则 $q \circ f$ 是局部 $\mu$ 可积且 $q(m) = (q \circ f) \cdot \mu$。

a) 对于$A'_q$的每个有限子集$J$，让我们用$\lambda_J$表示测度$|z' \circ m|$的上界，其中$z'$超过$J$；如果$g_J = \sup_{z' \in J} |\langle z', f \rangle|$则$\lambda_J = g_J \cdot \mu$（第V, §5, No. 2章，提案2）。对于$T$的每个相对紧开子集$U$，令$\lambda_{J,U}$为$\lambda_J$到$U$的限制；让我们首先证明，当$J$超过$A'_q$的有限子集的有向集合$\mathfrak{F}$时，族$(\lambda_{J,U})$在$\mathscr{M}(U)$中上界。事实上，对于$K(U)$中的每一个函数$h \geq 0$，

$$
\int h\,d\lambda_{J,U} = \int hg_J\,d\mu \leq \int^*(q \circ f)h\,d\mu \leq \|h\| \int_U^*(q \circ f)\,d\mu,
$$

从而我们的断言（章节II, §2, No. 2）。令 $\nu_U$ 为$\mathscr{M}(U)$ 中该测度系列的至高无上。如果$U'$是$T$的第二个相对紧开子集，使得$U \subset U'$，则$\nu_U$是$\nu_{U'}$到$U$的限制，直接从测度递增有向集合的上界表达式如下（第 II, §2, No. 2 章）以及$\lambda_{J,U}$ 是 $\lambda_{J,U'}$ 的限制到 $U$。因此，存在且仅有一个正测度$\nu$，其限制与每个$U$的$\nu_U$（第III, §2, No. 1，命题1），并且很明显$\nu = q(m)$。

b) 由于测度$\lambda_J$有基$\mu$，因此它们的上界$q(m)$也有（第V, §5, No. 5，第2章）。如果$f$对于$F$上的拓扑$\sigma(F, F')$是$\mu$可测的，则立即从定义得出$T$的映射$g : t \mapsto (g_J(t))_{J \in \mathfrak{F}}$到乘积空间 $\mathbf{R}^\mathfrak{F}$ 是 $\mu$ 可测量的。 $q \circ f = \sup_{J \in \mathfrak{F}} g_J$的限制对于$g$连续的每个紧凑体$T$的子集来说是下半连续的；因而 $q \circ f$ 是 $\mu$ 可测的（第 8 章第 IV, §5, No. 5 章和第 15 号建议No. 10）。令 $K$ 为 T 的紧子集；它承认$\mu$可忽略的集合的划分由……组成和紧集的序列$(K_n)$，其中$g$是连续的。然后对所有 $n$（第 IV, §1, No. 1、第 1 章和第 V, §7, No. 1、第 1 条提案）使用 $\int_{K_n}^*(q \circ f)\, d\mu = \sup_J \int_{K_n} g_J\, d\mu \leq \int_{K_n} dq(m)$、从而 $\int_K^*(q \circ f)\, d\mu = \sum_n \int_{K_n}^*(q \circ f)\, d\mu \leq \int_K dq(m)$。但这证明了$q \circ f$是局部$\mu$可积的，并且$\lambda_J \leq (q \circ f) \cdot \mu \leq q(m)$对于所有$J \in \mathscr{F}$； 从而，定义，$q(m) = (q \circ f) \cdot \mu$。

#### 注 {#int-vi-s2-n4-rem-1 .statement tag=09AM}

假设$A_q'$中存在可数子集D，其对于$\sigma(F', F)$来说是稠密的；那么， 函数 $q \circ f$ 始终是 $\mu$ 可测量的，因为 $q(f(t)) = \sup_{z' \in D} |\langle z', f(t) \rangle|$（第 IV, §5, No. 4 章，第 2 章的 Cor. 1）。然后，对于 T 的每个紧凑子集 K，$\int_K^*(q \circ f)\, d\mu = \sup_J \int_K g_J\, d\mu$，其中 J 运行于 D 的有限子集的可数有向集合（Ch. IV, §1, No. 1，Th. 3 的 Cor.）；因而，我们可以看出，在这种情况下，条件，对于 T 的每个紧凑子集 K，$\int_K^*(q \circ f)\, d\mu < +\infty$ 对于 m $q$ 可大化来说是必要且充分的。

#### 命题 9 {#int-vi-s2-prop-9 .statement tag=09AN}

— *令 F 为有限维 Banach 空间。 T 上的每个测度 m（F 中具有值）都是具有基 $|m|$ 的测度。如果 $m = f \cdot |m|$，则 $|f(t)| = 1$ 局部几乎处处都是 $|m|$。为了使 m 具有基 $\mu$，$|m|$ 具有基 $\mu$ 是充分必要的，并且如果 $m = g \cdot \mu$ 则$|m| = |g| \cdot \mu$。

令$(e_i)_{1 \leq i \leq n}$和$(e'_i)_{1 \leq i \leq n}$是F和F'的对偶基（A，II, §2, No. 6），对于所有i，$|e'_i| = 1$。那么对于每个指标 i 都有 $|e'_i \circ m| \leq |m|$，因而 (Ch. V, §5, No. 5, Th. 2) $e'_i \circ m = h_i \cdot |m|$，其中 $h_i$ 有界且 $|m|$ 可测。 设定$h = \sum_{i=1}^n h_i \cdot e_i$，因此我们有$m = h \cdot |m|$。如果 $m = f \cdot |m|$，第 8 条命题表明 $|m| = |f| \cdot |m|$、从而 $|f(t)| = 1$ 几乎在所有地方都适用于 $|m|$（V, §5, No. 3 章，第 3 条命题第 2 章）。最后的断言立即来自第8号提案。

#### 注 {#int-vi-s2-n4-rem-2 .statement tag=09AO}

如果$z = \sum_{i=1}^n z_i e_i$，则$\psi(z_1, \ldots, z_n) = |z|$是$\mathbf{R}^n$上的正齐次连续函数。 设定$\mu_i = e'_i \circ m = h_i \cdot |m|$，作者定义（第V, §5, No. 9）$\psi(\mu_1, \ldots, \mu_n) = \psi(h_1, \ldots, h_n) \cdot |m| = |h| \cdot |m| = |m|$。

### 5. 邓福德-佩蒂斯定理

令 $\mu$ 为 T 的正测度。 如果对于每个 $z' \in F'$，标量测度 $z' \circ m$ 的基数为 $\mu$，则 T 上的矢量测度 m（其值在 F 中）被称为 *基数* $\mu$ 的标量（或具有基数 $\mu$ 标量）。 如果 $F$ 中带有值的向量测度 $m$ 具有基 $\mu$，则它标量地具有基 $\mu$：对于，如果 $m = f \cdot \mu$，则对于每个 $z' \in F'$，$z' \circ m = \langle z', f \rangle \cdot \mu$。 但是，存在基$\mu$标量的向量测度，但没有基$\mu$（Exer.17），另一方面，对于任何正测度$\nu$，存在非基$\nu$标量的向量测度； 注然而，根据 Lebesgue-Nikodym 定理，在 *范数* 空间中，每个 * 可大化的 * 测量 $m$ 和值都是基 $|m|$ 的标量。

#### 例 {#int-vi-s2-n5-exa-1 .statement tag=09AP}

— 让我们取 $\mathscr{H}(T)$ 的 $m$ 恒等映射。说$m$是基$\mu$的标量意味着$T$上的每个实测度都有基$\mu$。特别是，点测度$\varepsilon_t$（$t \in T$）必须具有基$\mu$，这要求每个$t \in T$都有$\mu(\{t\}) > 0$，并且特别意味着$T$的每个紧凑子集都是*可数的*。

在这一篇中，我们将证明一个结果，该结果概括了 Lebesgue-Nikodym 定理的推论之一，即 $L^1(\mu)$ 的对偶是 $L^\infty(\mu)$（Ch. V, §5, No. 8，Th. 4），并且对于标量为 的矢量测量给出了足够的条件基$\mu$有基$\mu$。

设$\pi$是$\mathscr{L}^\infty(\mu)$到$L^\infty(\mu)$的典范映射。我们可以说，如果存在$G$的线性映射$\rho$进入$\mathscr{L}^\infty(\mu)$（称为$G$的*提升*），则$L^\infty$的线性子空间$G$具有*提升性质*，使得$\pi \circ \rho$是$G$ 和 $|\rho(f)(t)| \leq N_\infty(f)$ 适用于所有 $t \in T$ 和 $f \in G$。

证明如果$\mu$是$\mathbf{R}^n$上的勒贝格测度，则整个空间$L^\infty(\mathbf{R}^n, \mu)$具有提升性质（Exer.18）。

#### 引理 2 {#int-vi-s2-lem-2 .statement tag=09AQ}

*Banach 空间* $L^\infty(T, \mu)$ *的每个可分离子空间* $G$ *都有提升性质*。

到假设，存在$G$的可数稠密子集$H$，它是关于有理数的域$\mathbf{Q}$的线性子空间；设$(h_n)$是$H$超过$\mathbf{Q}$的（可数）基。对于每个整数$n$，令$h'_n$为$\mathscr{L}^\infty$的元素，从而$\pi(h'_n) = h_n$，并令$\rho'$为$H$到由$\rho'(h_n) = h'_n$定义的$\mathscr{L}^\infty$的$\mathbf{Q}$线性映射；显然$\pi \circ \rho'$是$H$上的恒等式。此外，对于每个$h \in H$，除了点$t$之外，还有一个$|\rho'(h)(t)| \leq N_\infty(h)$，其中集合$A(h)$可以忽略不计。令$A$为$h \in H$的$A(h)$的并，这在局部也是可以忽略不计的。对于每个$h \in H$，用$\rho(h)$函数$h'' \in \mathscr{L}^\infty$表示，这样如果$t \notin A$则为$h''(t) = \rho'(h)(t)$，如果$t \in A$则为$h''(t) = 0$。很明显，$\rho$是$H$到$\mathscr{L}^\infty$中有界函数的子空间$\mathscr{B}$的$\mathbf{Q}$线性映射，使得$\pi \circ \rho$是$H$上的恒等式，并且$|\rho(h)(t)| \leq N_\infty(h)$对于所有$h \in H$ 和 $t \in T$。由于$\mathscr{B}$是范数$\|f\| = \sup_{t \in T} |f(t)|$（第IV, §5, No. 4，Th.2）的Banach空间，$\rho$可以扩展到连续的$\mathbf{R}$线性映射，再次表示为$\rho$，将$G$映射到$\mathscr{B}$，这显然是$G$的提升。

#### 定义 5 {#int-vi-s2-def-5 .statement tag=09AR}

— 令 F 为 Hausdorff 局部凸空间，$F'_s$，其对偶配备拓扑$\sigma(F', F)$。我们将 T 的映射 $f$ 的 $\mathscr{L}_{F'_s}^\infty$ 向量空间表示为 $F'_s$，使得 $f$ 是标量 $\mu$ 可测量的，并且几乎在任何地方（对于$\mu$）都在局部标量上等于 T 的映射为等连续$F'$ 中的子集。我们将$\mathscr{L}_{F'_s}^\infty$的$L_{F'_s}^\infty$商空间表示为$\mu$-可忽略的T的映射到$F'_s$的局部标量空间。

当F满足§1, No. 5、第13条命题的假设时，$\mathscr{L}_{F'_s}^\infty$中的函数对于弱拓扑$\sigma(F', F)$来说是$\mu$可测的，但对于$F'$上的强拓扑不一定是可测的，即使F 是 Banach 空间（§1，Exer.17）。在相同的条件下，T到$F'_s$的局部$\mu$可忽略的映射与T到$F'_s$的局部$\mu$可忽略的映射相同（§1, No. 1，注2）。

当F是可分离范数空间时，$\mathscr{L}_{F'_s}^\infty$的元素是T的映射$f$进入$F'_s$，使得$f$是标量$\mu$可测的并且$|f|$在测度上是有界的；然后，通过为范数$N_\infty$（第IV, §6, No. 3）配备定义，可以在空间$L_{F'_s}^\infty$上实现空间结构。

#### 引理 3 {#int-vi-s2-lem-3 .statement tag=09AS}

令 F 为 Hausdorff 局部凸空间、$f$ 元素 $\mathscr{L}_{F'_s}^\infty$。对于每一个$z \in F$，都有$\langle z, f \rangle \in \mathscr{L}^\infty$，并且F到$L^\infty$的线性映射$z \mapsto \pi(\langle z, f \rangle)$是连续的；此外，如果 F 是范数空间，则$N_\infty(\langle z, f \rangle) \leq |z| \cdot \sup_{t \in T} |f(t)|$。

由定义可知$\langle z, f \rangle$是$\mu$可测且有测界； 替换如果需要$f$通过函数属于到$L_{F'_s}^\infty$的相同类，我们可以在加法中假设$f(T) \subset V^\circ$，其中V是F中0的平衡凸邻域（它不会修改$\langle z, f \rangle$ 除了局部可忽略不计的集合，取决于$z$）。那么关系$z \in V$意味着$|\langle z, f(t) \rangle| \leq 1$对于所有$t \in T$，这就证明了$z \mapsto \pi(\langle z, f \rangle)$的连续性。最后的断言是显而易见的。

#### 引理 4 {#int-vi-s2-lem-4 .statement tag=09AT}

令 F 为 Hausdorff 局部凸空间、$f$ 元素 $\mathscr{L}_{F'_s}^\infty$。对于每个数值函数 $g \in \overline{\mathscr{L}}^1$，函数 $gf$ 本质上是 $\mu$ 可积且$\int gf\, d\mu \in F'$。

对于每个$z \in F$，$\langle z, f \rangle$属于到$\mathscr{L}^\infty$，从而第一个断言。此外，我们可以假设，在不修改$\int gf\, d\mu$的情况下，$f(T) \subset V^\circ$，其中V是F中0的平衡凸邻域。那么对于所有$t \in T$，从而$|\langle z, \int gf\, d\mu \rangle| = |\int \langle z, f \rangle g\, d\mu| \leq \overline{N}_1(g)$，关系$z \in V$意味着$|\langle z, f(t) \rangle| \leq 1$，这证明了$\int gf\, d\mu \in F'$。

#### 定理 1 {#int-vi-s2-thm-1 .statement tag=09AU}

— 令 F 为 Hausdorff 局部凸空间且包含可数稠密子集。对于每个函数$f \in \mathscr{L}_{F'_s}^\infty$和每个$z \in F$，令$v_f(z) = \pi(\langle z, f \rangle) \in L^\infty$； 映射$f \mapsto v_f$定义，通过商，$L_{F'}^\infty$的线性双射到空间$\mathscr{L}(F; L^\infty)$，$F$的连续线性映射进入$L^\infty$。 *如果 $F$ 是标准化的空间，则此双射是等距。*

根据引理3，如果证明对于$F$到$L^\infty$的每个连续映射$u$，都存在一个函数$f \in \mathscr{L}_{F'}^\infty$，使得$\pi(\langle z, f \rangle) = u(z)$对于所有$z \in F$，并且$L_{F'}^\infty$中$f$的类是由该条件唯一确定的，则第一个断言得到证明。 第二个点是直接的，因为如果$\pi(\langle z, f \rangle) = \pi(\langle z, f_1 \rangle)$对于所有$z \in F$，那么$f_1 - f$在标量上局部可以忽略不计。 另一方面，存在将 $u(F)$ 提升到 $\mathscr{L}^\infty$ (引理 2) 的$\rho$。 对于每个$t \in T$，映射$z \mapsto \rho(u(z))(t)$是$F$上的连续线性形式，即$F'$的元素$f(t)$。 对于每个$z \in F$，函数$f$从$\langle z, f \rangle = \rho(u(z)) \in \mathscr{L}^\infty$开始可按比例$\mu$测量；一个有 $\pi(\langle z, f \rangle) = u(z)$；最后，对于$L^\infty$的单位球的$u$下的每个$t \in T$和每个$z$属于到逆像$V$，

$$
|\langle z, f(t) \rangle| = |\rho(u(z))(t)| \leq N_\infty(u(z)) \leq 1,
$$

这表明对于所有 $t \in T$ 都有 $f(t) \in V^\circ$。

此外，如果 $F$ 是范数空间，则上式表明

$$
\sup_{t \in T} |f(t)| \leq \|u\|.
$$

但另一方面，(引理 3)，$N_\infty(u(z)) \leq |z| \cdot \sup_{t \in T} |f(t)|$，当$f$在局部可忽略不计的集合上任意修改时，不等式继续成立。由此可知$\|u\| = N_\infty(|f|)$。

#### 推论 1 {#int-vi-s2-thm-1-cor-1 .statement tag=09AV}

*令$F$为豪斯多夫局部凸空间包含可数稠密子集。对于每个函数$f \in \mathscr{L}_{F'}^\infty$、每个$z \in F$和每个函数$g \in \mathscr{L}^1$，让$\Phi_f(z, \tilde{g}) = \int \langle z, f(t) \rangle g(t)\, d\mu(t)$。 映射$f \mapsto \Phi_f$定义，通过商，$L_{F'}^\infty$的线性双射到$F \times L^1$上连续双线性形式的空间$\mathscr{B}(F, L^1)$。 *如果 $F$ 是标准化的空间，则此双射是等距。*

我们可以假设 $f(T)$ 是 $F'$ 的等连续子集。则可知$\Phi_f$单独连续，且记号为Th。 1 和附录，有一个（考虑到 $L^\infty$ 是 $L^1$（第 V, §5, No. 8，第 4 章）的对偶）$^l \Phi_f = v_f$。 推论然后从 Th 开始。上面的 1 以及来自附录、No. 1、第 1 号提案及其推论。

#### 推论 2（邓福德-佩蒂斯定理）{#int-vi-s2-thm-1-cor-2 .statement tag=09AW}

— *令 $F$ 为 Hausdorff 局部凸空间包含可数稠密子集。对于每个函数$f \in \mathscr{L}_{F'}^\infty$和每个函数$g \in \mathscr{L}^1$，让$w_f(\tilde{g}) = \int gf\, d\mu \in F'$（引理4）。 映射$f \mapsto w_f$定义，通过商，$L_{F_s}^\infty$的线性双射*到线性映射$u$的空间$\mathscr{R}(L^1, F')$进入$L^1$ $F'$使得$L^1$的单位球的$u$下的像是$F'$的等连续子集。 *如果$F$是规范的空间（在这种情况下，$\mathscr{R}(L^1, F')$是$L^1$的连续线性映射到$F$的强对偶的空间），双射$f \mapsto w_f$是一个等距。*

考虑到$L^\infty$是$L^1$的对偶，这是从前面的推论以及附录、No. 1、第1条命题及其推论得出的。

#### 注 {#int-vi-s2-n5-rem-1 .statement tag=09AX}

— 很明显，对于$F'$上的每个$\mathscr{G}$拓扑，映射$u \in \mathscr{R}(L^1, F')$都是连续的（$\mathscr{G}$由有界子集覆盖$F$）。相反，如果还假设$F$是*桶状*，则$L^1$的每个连续线性映射进入$F'$，配备$\mathscr{G}$拓扑变换单位球$L^1$进入有界子集等于 $F'$，因此是等连续的（TVS、III, §4, No. 2、Th.1）。

#### 推论 3 {#int-vi-s2-thm-1-cor-3 .statement tag=09AY}

*令 $F$ 为 Hausdorff 局部凸空间包含可数稠密子集，$m$ $T$ 上的向量测度，值位于 $F$ 的弱对偶 $F'$ 中。如果像位于$\mathscr{K}(T)$中的集合$B$、函数$g$的$m$下，使得$\mu(|g|) \leq 1$包含在$F'$的闭凸等连续子集$H'$中，则$m$ 有基 $\mu$，并且相对于 $\mu$ 存在 $m$ 的密度 $f$，使得 $f(t) \in H'$ 对于所有 $t \in T$。*

假设意味着当$\mathscr{K}(T)$配备由$\mathscr{L}^1(\mu)$（由半范数$N_1$定义）诱导的拓扑时，$m$是连续的；因此，它可以扩展到$\mathscr{L}^1(\mu)$的连续线性映射$u$到$F$弱对偶的完成$G$；但由于$H'$是$G$的紧凑子集和像在集合$\overline{B}$的$u$下$f \in \mathscr{L}^1$，因此$N_1(f) \leq 1$包含在$H'$的闭包中$G$，一个有$u(\overline{B}) \subset H'$，因此$u$映射$\mathscr{L}^1$变成$F'$。由于关系$N_1(f) \leq \varepsilon$意味着$u(f) \in \varepsilon H'$，如果$g$是$\mu$可忽略不计，则有$u(g) = 0$，并且Cor。因此，2 可以应用于 $L^1$ 的映射到从 $u$ 经过到商获得的$F'$； 从而推论。

#### 推论 4 {#int-vi-s2-thm-1-cor-4 .statement tag=09AZ}

*令$F$为可分离范数空间，而$m$为$T$的测度，其中值位于强对偶$F'$中，可对$F'$的范数进行大化。那么 $m$ 是一个具有基 $|m|$ 的度量，如果 $m = f \cdot |m|$ 那么 $|f(t)| = 1$ 几乎在任何地方都适用于 $|m|$。*

到假设，对于每一个$z \in F$使得$|z| \leq 1$，对于每一个函数$g \in \mathscr{K}(T)$都有$|\langle z, m(g) \rangle| \leq |m|(|g|)$，因而$|m(g)| \leq |m|(|g|)$（TVS，IV, §2, No. 4，公式（1））。由于 $F'$ 中的每个球都是等连续的，Cor. 3适用并表明$m$有基$|m|$；此外，如果$m = f \cdot |m|$，则$f$对于$\sigma(F', F)$（§1, No. 5，第13条命题）和$|m| = |f| \cdot |m|$（No. 4，第8条命题）来说是$|m|$可测的，这就证明了推论（V, §5, No. 3，Cor.提案 3 中的 2）。

如果将此推论应用于$F$（如果是有限维）的情况，则可以将第9条命题的第一个部分恢复为特殊情况。

### 6. 空间 $L^1_F$ 的双重（F 是可分离的 Banach 空间）

#### 命题 10 {#int-vi-s2-prop-10 .statement tag=09B0}

— *令 F 为可分离的 Banach 空间。对于每个函数$f \in \overline{\mathscr{L}}^1_F$和每个函数$g \in \mathscr{L}_{F'_s}^\infty$，数值函数$\langle f, g \rangle : t \mapsto \langle f(t), g(t) \rangle$本质上是$\mu$可积的，并且*

$$
\left| \int \langle f, g \rangle \, d\mu \right| \leq \overline{N}_1(f) N_\infty(g) .
$$

*对于每个类$\dot{g} \in L_{F'_s}^\infty$，令$\theta(\dot{g})$为$L^1_F$上的连续线性形式，由$\overline{\mathscr{L}}^1_F$上的线性形式$f \mapsto \int \langle f, g \rangle \, d\mu$通过商推出；那么$\theta$是$L_{F'_s}^\infty$到Banach空间$L^1_F$的强对偶$(L^1_F)'$的线性等距。

对于 T 的每个紧致子集 K 和每个 $\varepsilon > 0$，都存在 K 的紧致子集 $K'$，使得 $f$（分别为 $g$）到 $K'$ 的 $\mu(K - K') \leq \varepsilon$ 和限制是连续的将 $K'$ 的映射转换为 F（分别转换为 $F'_s$）；因而$g(K')$是弱紧致的，因此在$F'$上等连续（TVS，III, §4, No. 2，Th.1或IV, §1，Exer.10）。现在，F 的 $F \times F'$ 到乘积上的规范双线性形式的限制和 $F'$ 的等连续子集对于 F 的拓扑和 $\sigma(F', F)$ 的乘积拓扑是连续的（GT， X, §2, No. 1，第 1 条第 4 条）；由此可见，$\langle f, g \rangle$到$K'$的限制是连续的，因而$\langle f, g \rangle$是$\mu$可测的。而且，

$$
|\langle f(t), g(t) \rangle| \leq |f(t)| \cdot |g(t)| \leq |f(t)| N_\infty(g)
$$

局部几乎无处不在，因而 $\langle f, g \rangle$ 本质上是 $\mu$ 可积的，并且不等式 (3) 成立（Ch. IV, §5, No. 6、Th. 5 和 Ch. V, §1, No. 3、引理）。

仍有待证明 $\theta$ 是满射等距。令$u$为$L^1_F$上的连续线性形式。 映射 $(\tilde{h}, z) \mapsto u(\tilde{h}z)$ 是 $L^1 \times F$ 上的连续双线性形式，因为

$$
|u(\tilde{h}z)| \leq \|u\| \cdot N_1(hz) \leq \|u\| \cdot |z| \cdot N_1(h) .
$$

由科. 1 Th。 No. 5 1，存在 T 的映射 $g$ 到 $F'$、属于到 $\mathscr{L}_{F'_s}^\infty$，这样对于所有 $t \in T$ 都有 $|g(t)| \leq \|u\|$，对于每个函数 $h \in \mathscr{L}^1$ 都有 $u(\tilde{h}z) = \int \langle hz, g \rangle \, d\mu$ $L^1$ 和每 $z \in F$ 类 $\tilde{h}$。在其他字、线性形式$u$和$\theta(\dot{g})$重合中，由形式$\tilde{h}z$($\tilde{h} \in L^1, z \in F$)的元素生成$L^1_F$的子空间。由于子空间在$L^1_F$（第IV, §3, No. 5，命题10）中是稠密的，因此可以得出$u = \theta(\dot{g})$，这已经证明了$\theta$是满射的。此外，由（3），$\| \theta(\dot{g}) \| \leq N_\infty(g) \leq \| u \| = \| \theta(\dot{g}) \|$，从而$\| \theta(\dot{g}) \| = N_\infty(g)$，还有这个结论证明。

### 7. 向量值函数相对于向量测量的积分

#### 命题 11 {#int-vi-s2-prop-11 .statement tag=09B1}

— *令* $F, G, H$ *为三个Banach 空间*、$\Phi$ *将* $F \times G$ *连续双线性映射到* $H$。 *让*$m$*成为*$T$上的可主化矢量测度，*其中值在*$G$中。 *则存在一个且仅有一个连续的线性映射* $I_{\Phi,m}$ *of* $\overline{\mathscr{L}}^1_F(|m|)$ *进入* $H$ *这样，对于每个* $z \in F$ *和每个数字函数* $h$ *可积为* $|m|$，*一个有* $I_{\Phi,m}(hz) = \Phi(z, \int h dm)$。 *此外，

$$
|I_{\Phi,m}(f)| \leq \| \Phi \| \int |f| d|m|
$$

*每函数* $f \in \overline{\mathscr{L}}^1_F(|m|)$。

如果存在这样的映射，则$|m|$可积集合上的*步骤*函数$f$的值是唯一确定的：因为，已知可以写出$f = \sum_i a_i \varphi_{X_i}$，其中$X_i$是$|m|$-可积和不相交的，以及$a_i \in F$（第IV, §4, No. 9、引理）。因此，$I_{\Phi,m}(f)$的值必须等于$\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$。现在，我们有（No. 3，提案 5）

$$
\left| \sum_i \Phi \left( a_i, \int \varphi_{X_i} dm \right) \right| \leq \| \Phi \| \cdot \sum_i |a_i| \cdot |m|(X_i) = \| \Phi \| \int |f| d|m|,
$$

这首先表明$H$的元素$\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$不依赖于形式$\sum_i a_i \varphi_{X_i}$中$f$的特定表达式，因此我们可以用$I_{\Phi,m}(f)$来表示它。我们立即验证这样定义的映射$I_{\Phi,m}$在步骤函数的空间$\mathscr{E}_F$上与$|m|$可积集合是线性的：因为，只需将$\mathscr{E}_F$的两个函数$f, g$写在形式$f = \sum_i a_i \varphi_{X_i}$和$g = \sum_i b_i \varphi_{X_i}$具有相同的成对不相交的$|m|$可积有限族集合$X_i$（这可以通过第IV, §4, No. 9章的引理实现）。 不等式 (5) 然后证明 $I_{\Phi,m}$ 在 $\mathscr{E}_F$ 上是连续的，并且由于这个子空间在 $\overline{\mathscr{L}}^1_F$ 中是密集的（第 19 章第 IV, §4, No. 10，第 19 章的 Cor. 1 和第 V, §1, No. 3），因此可以推断出唯一性的存在性和唯一性 $I_{\Phi,m}$，以及不等式 (4)。

有人说$I_{\Phi,m}(f)$是$f$*相对于*$m$的积分（相对于双线性映射$\Phi$）；当点$(x,y)$处的双线性映射$\Phi$的值表示为$xy$时，我们应写为$\int f\,dm$而不是$I_{\Phi,m}(f)$。

当记号为No. 6时，$\int \langle f, g \rangle\,d\mu$的积分就是$I_{\Phi,m}(f)$与$\Phi(x,x') = \langle x, x' \rangle$和$m = g \cdot \mu$的积分。

#### 推出 {#int-vi-s2-n7-cor-1 .statement tag=09B2}

*如果* $m$ *和* $m'$ *是* $T$、*与值在* $G$、*则* $I_{\Phi,m+m'} = I_{\Phi,m} + I_{\Phi,m'}$ *和* $I_{\Phi,\lambda m} = \lambda I_{\Phi,m}$ *对于每个标量* $\lambda$ 的两个主要度量。

第二个断言是直接的。第一个表示对于每个函数$f$，它既是$|m|$可积又是$|m'|$可积，

$$
I_{\Phi,m+m'}(f) = I_{\Phi,m}(f) + I_{\Phi,m'}(f).
$$

函数 $f$ 是 $(|m| + |m'|)$ 可积（第 V, §2, No. 2 章，命题 3 的 Cor.1），因此 *更不必说* $(|m + m'|)$ 可积，并且 (6) 的第一个成员确实有意义。为了证明 (6)，只需对 $f$ 在 $(|m| + |m'|)$ 可积集合上移动函数就足够了，因为这些函数中的集合在 $\mathscr{L}_F^1(|m| + |m'|)$ 中是稠密的，并且 (6) 的两个成员在后者空间中是连续的，通过凭借（4）。但是对于$f = a \varphi_X$，其中$X$是$(|m| + |m'|)$可积的，(6)约化到$\Phi(a, \int \varphi_X\,dm) + \Phi(a, \int \varphi_X\,dm')$的两个成员，从而推论。

#### 注 {#int-vi-s2-n7-rem-1 .statement tag=09B3}

— 当$m$为形式$b\mu$时，其中$b \in G$和$\mu$是$T$的实测度，

$$
I_{\Phi,m}(f) = \int \Phi(f(t), b)\,d\mu(t)
$$

对于每个函数$f \in \mathscr{L}_F^1(\mu)$，因为当$f$是$|\mu|$可积集合上的一步函数时，两个成员在空间和重合上都是连续的。

### 8. 复杂的措施

#### 定义 6 {#int-vi-s2-def-6 .statement tag=09B4}

*有人称复数测量为* $T$ *复数向量空间* $\mathscr{K}_C(T)$上的每个连续线性形式。\脚注{Cf.章。 III, §1, No. 3，防御。 2.}

因此，$T$ 上的复测度空间 $\mathscr{M}_C(T)$ 是 Hausdorff 局部凸空间 $\mathscr{K}_C(T)$ 的“对偶”。

如果$m$是$T$上的复测度，则其限制到$\mathscr{K}(T)$是$T$上的矢量测度，其中值在$\mathbf{C}$上（视为向量空间超过$\mathbf{R}$）；

m 由此限制确定，因为如果 $f = f_1 + i f_2 \in \mathscr{H}_\mathbf{C}(T)$，则 $f$ 的实数部分 $f_1$ 和虚数部分 $f_2$ 位于 $\mathscr{H}(T)$ 和 $m(f) = m(f_1) + i m(f_2)$ 中。相反，对于 T 上的每个向量测度 $m_0$ 以及 $\mathbf{C}$ 中的值、公式 $m(f) = m_0(f_1) + i m_0(f_2)$ 定义一个复测度 $m$，T 上唯一一个限制到 $\mathscr{H}(T)$ 为 $m_0$。因此，今后我们将使用认同一个复杂的衡量标准，其限制到$\mathscr{H}(T)$；这样的测度$m$是形式$m = \mu_1 + i \mu_2$，其中$\mu_1$和$\mu_2$是T上的两个实测度，分别称为$m$的实数部分和虚数部分。 $m$的支持度是$\mu_1$和$\mu_2$的支持度的并。我们知道 $m$ 是可大化的（No. 3，Cor. of Prop. 4）；我们将把$m$的绝对值值称为$|m|$相应的到$\mathbf{C}$上的绝对值值$|x_1 + i x_2| = \sqrt{x_1^2 + x_2^2}$。其中一个有 $|m| = (\mu_1^2 + \mu_2^2)^{1/2}$（No. 4、注，遵循第 9 条）、$^3$ 和 $|\mu_1| \leq |m|$、$|\mu_2| \leq |m|$、$|m| \leq |\mu_1| + |\mu_2|$；此外，$m$是基$|m|$的度量，并且可以写成$m = h \cdot |m|$，其中$h \in \mathscr{L}_\mathbf{C}^\infty(|m|)$和$|h(t)| = 1$在本地几乎无处不在$|m|$（No. 4，第9条）。$^4$的支持$m$ 和 $|m|$ 相同。

对于 T 的每个映射 $f$ 到复数 Banach 空间 F，基本上可相对于 $|m|$ 可积，可以定义 (No. 7) $f$ 相对于$m$（相应的到 R 双线性映射）的积分将$F \times \mathbf{C}$的$(x, \lambda) \mapsto \lambda x$代入F)，记为$\int f \, dm$；它立即从第11号提案的唯一性性质得出（与前面的记号）$\int f \, dm = \int f \, d\mu_1 + i \int f \, d\mu_2 = \int f h \, d|m|$。因此，我们有 $m(f) = \int f \, dm$ 对应 $f \in \mathscr{H}_\mathbf{C}(T)$。我们说$f$相对于$m$本质上是可积的，如果$|m|$也是如此；$^5$映射是$m$可积，$m$可测，局部$m$可积， $m$-可忽略或局部$m$-可忽略的定义类似。我们写
$$
\mathscr{L}_F^p(T, m) \quad \text{(resp. } \overline{\mathscr{L}}_F^p(T, m), \ L_F^p(T, m) \text{)}
$$
而不是 $\mathscr{L}_F^p(T, |m|)$（或 $\overline{\mathscr{L}}_F^p(T, |m|), \ L_F^p(T, |m|)$）；这些很复杂向量空间。

为了使 $f$ $m$ 可积（或本质上 $m$ 可积），由于 $|m|, |\mu_1|, |\mu_2|$ 和关系之间的不等式，$f$ 对于四个测度 $\mu_1^+, \mu_1^-, \mu_2^+, \mu_2^-$ 中的每一个是可积的（或本质上可积）是必要且充分的$|\mu_k| = \mu_k^+ + \mu_k^-$（第 V, §2, No. 2 章，第 3 条提案及其修正 1）。

如果$f$本质上是$m$可积（分别是$m$可积），那么$|f|$本质上是可积的

---
$^3$特别是$|m|$重合与第1章中的定义。 III, §1, No. 6（cf.章节V, §5, No. 9）。
$^4$Cf。章。 V, §5, No. 5，科。 3 Th。 2 以获得更锐利的叙述。
$^5$Cf。章。 V, §1、注在 No. 3 末尾。

本质上是$|m|$可积（分别是$|m|$可积），并且从命题11可以得出：

$$
\left| \int \mathbf{f}\, dm \right| \leq \int |\mathbf{f}| \, d|m|.
$$

设 F 和 G 是两个复数 Banach 空间，$u$ F 到 G 的连续线性映射。如果 $\mathbf{f}$ 本质上是 T 到 F 的 $m$ 可积（或 $m$ 可积）映射，则 $u \circ \mathbf{f}$ 本质上是$m$-可积（分别为$m$-可积）和$\int (u \circ \mathbf{f})\, dm = u(\int \mathbf{f}\, dm)$；这立即从前述和类似的命题中得出，对于本质上 $|m|$ 可积函数（Ch. IV, §4, No. 2、Th. 1 和 Ch. V, §1, No. 3、引理和 Def. 3）。

令 $m$ 为 T 上的复数测度，令 $h$ 为局部 $m$ 可积复数函数。对于每个函数 $f \in \mathscr{K}_C(T)$，函数 $fh$ 是 $m$ 可积的，并且映射 $f \mapsto \int fh\, dm$ 是一个复杂测度，表示为 $h \cdot m$ 并称为测度 *和密度* $h$ $m$。若$m = g \cdot |m|$，则显然$h \cdot m = hg \cdot |m|$；此外，因为，$|g(t)| = 1$对于$|m|$来说几乎处处都是局部的，对于$\mathbf{f}$对于$n = h \cdot m$来说本质上可积，$fh$本质上$m$可积是必要且充分的，在这种情况下$\int \mathbf{f}\, dn = \int (\mathbf{f}h)\, dm$。而且，$|h \cdot m| = |h| \cdot |m|$。我们再次说，形式$h \cdot m$的每个测度都是一个复杂测度*与基*$m$；两个复杂的度量$m, m'$被认为是*等价的*，如果每个都相对于另一个具有密度，或者，如果$m' = h \cdot m$与$h$局部$m$可积，并且$h(t) \neq 0$局部几乎处处对于$|m|$来说是相同的。显然，$m$和$|m|$是等价的，并且，为了使$m$和$m'$等价，$|m|$和$|m'|$等价是充分必要的。

如果$m$和$m'$是T上的两个复测度，并且$\mathbf{f}$是函数，其中值位于复数Banach空间F中，对于$m$和$m'$本质上可积（或可积），那么，对于任何复数 $\lambda$ 和 $\lambda'$，$\mathbf{f}$ 对于 $\lambda m + \lambda' m'$ 本质上可积（或可积），并且

$$
\int \mathbf{f}\, d(\lambda m + \lambda' m') = \lambda \int \mathbf{f}\, dm + \lambda' \int \mathbf{f}\, dm'.
$$

因为，这是从 Cor 得出的。 No. 7第 11 号提案。

在加法中，从定义得出

$$
|\lambda m + \lambda' m'| \leq |\lambda| \cdot |m| + |\lambda'| \cdot |m'|.
$$

我们将复杂测度$m$的*共轭测度*称为由$\overline{m}(f) = m(\overline{f})$为$f \in \mathscr{K}_C(T)$定义的复杂测度$\overline{m}$。如果$m = \mu_1 + i \mu_2$，其中$\mu_1$和$\mu_2$是实测度，则$\overline{m} = \mu_1 - i \mu_2$和$|\overline{m}| = |m|$；如果$m = h \cdot |m|$则$\overline{m} = \overline{h} \cdot |m|$。如果 $f$ 本质上是 $m$ 可积（分别为

m-可积) 函数与复数值，则 $\overline{f}$ 本质上是 $\overline{m}$-可积（或 $\overline{m}$-可积）并且

$$
\int \overline{f}\, d\overline{m} = \overline{\int f\, dm}.
$$

#### 命题 12 {#int-vi-s2-prop-12 .statement tag=09B5}

*令 m 为 T、p 和 q 共轭指数（第 IV, §6, No. 4）的复测度。 双线性形式 $(f,g) \mapsto \int fg\, dm$ 在乘积 $\mathscr{L}_C^p(m) \times \mathscr{L}_C^q(m)$ 上定义且连续； 不等式$|\int fg\, dm| \leq N_p(f)N_q(g)$成立，$N_q(g)$是从线性形式$f \mapsto \int fg\, dm$经过商推导出$\mathscr{L}_C^p(m)$上的连续线性形式的范数。

此外，如果$1 \leq p < +\infty$，则复数向量空间$\mathscr{L}_C^p(m)$上的每个连续线性形式都是型$f \mapsto \int fg\, dm$，其中$g$是$\mathscr{L}_C^q(m)$中的函数，其类在$\mathscr{L}_C^q(m)$是唯一确定的。

从 $m = h \cdot |m|$ 开始，$|h(t)| = 1$ 几乎无处不在，第一个断言立即来自 Hölder 的不等式（第 IV, §6, No. 4，第 2 章）；第二个来自第 3 章的命题 3。 IV, §6, No. 4。最后，如果$u$是$\mathscr{L}_C^p$上的连续线性形式，则其限制到$\mathscr{L}_C^p$的（实数）子空间$\mathscr{L}^p$是$\mathscr{L}^p$到$\mathbf{C}$的连续$\mathbf{R}$线性映射；如果$1 \leq p < +\infty$，则它是型$f \mapsto \int fg_1\, d|m| + i \int fg_2\, d|m|$，其中$g_1$和$g_2$属于到$\mathscr{L}^q$（第V, §5, No. 8，第4章）； 从而决赛断言，于设定$g = (g_1 + ig_2)h^{-1}$。

### 9. 有界复杂测度⁶

对于$T$上的每个复杂度量$m$，一个集合

$$
\|m\| = \sup_{\|f\| \leq 1,\, f \in \mathscr{H}_C(T)} |m(f)|.
$$

有人说，如果$\|m\| < +\infty$，则$m$是*有界的*；同样的说法是，$m$在$\mathscr{H}_C(T)$上连续，并具有一致收敛的拓扑，因此可以扩展到连续复数函数倾向的Banach空间$\mathscr{H}_C(T)$上的连续线性形式（范数$\|m\|$）无穷远处为 0。

#### 引理 5 {#int-vi-s2-lem-5 .statement tag=09B6}

*令 m 为 T 上的复数测度，f 为 m 可积复数函数。然后$\int |f|\, d|m| = \sup |\int fh\, dm|$，因为h在$\mathscr{H}_C(T)$中运行函数的集合，使得$|h(t)| \leq 1$对于所有$t \in T$*。

⁶参见。章。 III, §1, No. 8。

如果$m = g \cdot |m|$，则$\int |f| d|m| = \int |f g| d|m|$和$\int f h \, dm = \int f g h \, d|m|$。当$f(t)g(t) = 0$时集合$\zeta(t) = 0$，当$f(t)g(t) \neq 0$时$\zeta(t) = \frac{f(t)g(t)}{|f(t)g(t)|}$； $\zeta$ 是 $|m|$ 可测的，因此对于每个$\varepsilon > 0$，都存在 T 的紧子集 K，使得 $\int_{T-K} |f| \, d|m| \leq \varepsilon$、$\zeta$ 到 K 的限制是连续的，$|\zeta(t)| = 1$ 在 K 上。因此，根据 Urysohn 的定理，存在在 T 上定义的连续函数 $\zeta_1$，具有复数值，使得 K 上有 $\zeta_1 = \zeta$，并且对于每个 $t \in T$ 都有 $|\zeta_1(t)| \leq 2$ 和 $\zeta_1(t) \neq 0$； 设定$h(t) = \zeta_1(t)/|\zeta_1(t)|$，我们看到$h$在T上连续，重合与$\zeta$在K上连续，并且对于所有$t \in T$来说$|h(t)| = 1$。最后，让$u$是T到$[0,1]$的连续映射，在K上等于1并且有紧支撑； 设定$h_1 = h^{-1}u$，我们有
$$
\left| \int f h_1 \, dm - \int |f| \, d|m| \right| \leq 2 \int_{T-K} |f| \, d|m| \leq 2\varepsilon ,
$$
这就证明了引理。

#### 命题 13 {#int-vi-s2-prop-13 .statement tag=09B7}

— *令 m 为复数测度，且 $\mu = |m|$。为了使 m 有界，$\mu$ 有界是必要且充分的，在这种情况下，$\|m\| = \|\mu\|$。*

我们有 $m = g \cdot \mu$，其中 $g$ 是 $\mu$ 可测量的，而 $|g(t)| = 1$ 对于所有 $t \in T$ 都是可测量的。如果 $\mu$ 有界，则对于每个函数 $f \in \mathscr{K}_\mathbf{C}(T)$，
$$
|m(f)| = \left| \int f g \, d\mu \right| \leq N_\infty(fg)\|\mu\| = \|f\| \cdot \|\mu\|,
$$
因此$m$是有界的并且$\|m\| \leq \|\mu\|$。如果 $m$ 有界，那么对于每个 $f \in \mathscr{K}_\mathbf{C}(T)$，考虑到引理 5，
$$
|\mu(f)| \leq \|f\| \cdot \|m\|,
$$
因此$\mu$是有界的并且$\|\mu\| \leq \|m\|$。 从而命题。

#### 推论 {#int-vi-s2-n9-cor-1 .statement tag=09B8}

— *令 m 为有界复数测度。每个函数 $f \in \mathscr{L}_\mathbf{F}^\infty(m)$ 都是 m 可积的，并且 $\left| \int f \, dm \right| \leq N_\infty(f)\|m\|$。*

因为，$f$是$m$可测量的，并且设定$\mu = |m|$，我们有
$$
\int^* |f| \, d\mu \leq N_\infty(f)\|\mu\| = N_\infty(f)\|m\|,
$$
因此 $f$ 是 $|m|$ 可积（Ch. IV, §5, No. 6，Th. 5）并且
$$
\left| \int f \, dm \right| \leq \int |f| \, d\mu \leq N_\infty(f)\|m\|.
$$

### 10. 复杂措施的像；诱导复杂测量； 乘积复杂措施\脚注{参见。章。 V, §6, No. 4；章。 IV, §5, No. 7 和章。 V, §7；章。 III, §4 和 Ch. V, §8，第 2–5 号。}

令 $m$ 为 $T$ 上的复测度，并令 $\pi$ 为 $T$ 的映射成为局部紧凑的空间 $X$。如果$\pi$是$|m|$-本征，我们可以说$\pi$是$m$-本征（第V, §6, No. 1章，定义1）；那么直接的对于每个函数$f \in \mathscr{H}_C(X)$，函数$f \circ \pi$本质上是$m$可积，并且

$$
\left| \int (f \circ \pi)\, dm \right| \leq \int |f \circ \pi|\, d|m| = \int |f|\, d(\pi(|m|)),
$$

因此映射$f \mapsto \int (f \circ \pi)\, dm$在$\mathscr{H}_C(X)$上是连续的，另外字是$X$上的复测度，记作$\pi(m)$，称为$\pi$下$m$的*像*。此外，由(8)得出$|\pi(m)| \leq \pi(|m|)$。如果 $m$ 和 $m'$ 是 $T$ 上的两个复数测度，且 $\pi$ 既是 $m$-真值又是 $m'$-真值，则对于任何复数标量 $\lambda, \lambda'$，$\pi$ 是 $(\lambda m + \lambda' m')$-真值，并且$\pi(\lambda m + \lambda' m') = \lambda \pi(m) + \lambda' \pi(m')$。

令 $Y$ 为 $T$ 的局部紧凑子空间。对于$T$上的每个函数$f \in \mathscr{H}_C(Y)$，函数$f'$，如果$t \in Y$则由$f'(t) = f(t)$定义，如果$t \notin Y$则由$f'(t) = 0$定义，是$m$可积的（第1章） IV, §5, No. 7); 直接的映射 $f \mapsto \int f'\, dm$ 是 $Y$ 上的复杂测度，称为 $m$ 在 $Y$ 上“诱导”的测度并表示为 $m_Y$。如果$m = g \cdot |m|$，很明显$m_Y = g_Y \cdot |m|_Y$，其中$g_Y$是函数$g$的限制到$Y$，它对于$|m|_Y$（第V, §7, No. 1）是局部可积的；此外，由于 $|g_Y| = 1$ 局部几乎无处不在 $|m|_Y$（第 V, §7, No. 1 章，第 1 号提案的 Cor.1），我们有 $|m_Y| = |m|_Y$。章。 IV, §5, No. 7、引理 3.}

令 $T$ 和 $T'$ 为两个局部紧凑的空间，$m$（分别为 $m'$）为 $T$（分别为 $T'$）的复测度。 写出$m = g \cdot |m|$和$m' = g' \cdot |m'|$。 对于正测度 $|m| \otimes |m'|$，函数 $g \otimes g'$ 可在 $T \times T'$ 上局部积分（第 1 章） V, §8, No. 5, Prop. 10), and one verifies immediately that if $g$ (resp. $g'$) is replaced by a function $g_1$ (resp. $g'_1$) equal to $g$ (resp. $g'$) locally almost everywhere for $|m|$ (resp. $|m'|$), then $g_1 \otimes g'_1$ is equal to $g \otimes g'$ locally almost everywhere for $|m| \otimes |m'|$. 因此，$T \times T'$上的复测度$(g \otimes g') \cdot (|m| \otimes |m'|)$仅取决于$m$和$m'$；它表示为 $m \otimes m'$，并称为 $m$ 和 $m'$ 的 *乘积* 度量。 由于 $|g \otimes g'| = 1$ 局部几乎无处不在 $|m| \otimes |m'|$（第 1 章） V, §8, No. 2，命题4），我们有$|m \otimes m'| = |m| \otimes |m'|$。\footnote{Cf.章。 III, §4, No. 2，命题 3。}

读者将很容易验证第 1 章中所有命题的证明。 V相对于正测度的像、由正测度引起的测度以及正测度的乘积，除了上积分或基本上积分介入的情况外，当正测度被任意复杂测度替代时仍然有效。

最后，一个定义如§1中的复数测度m的标量本质上m可积函数的概念；对于函数 f 具有此性质，f 对于 $|\mu_1|$ 和 $|\mu_2|$ 基本上可标量积是必要且充分的，其中 $\mu_1$ 和 $\mu_2$ 是 $m$ 的实部和虚部部分，在这种情况下为 $\int f dm = \int f d\mu_1 + i \int f d\mu_2$。我们留给读者的任务是将§1的结果应用到复杂的测量中。

### 习题{#int-vi-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
