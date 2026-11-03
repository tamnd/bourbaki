---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 3
section_title: Disintegration of measures
lang: zh
source: int-i-vi
book_pages: INT VI.40-INT VI.51, INT VI.69-INT VI.71
pdf_pages: 0431-0442, 0460-0462
extraction: ocr
subsections:
    - "no": 1
      title: Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping
      page: 40
      pdf_page: 431
    - "no": 2
      title: Pseudo-image measures
      page: 44
      pdf_page: 435
    - "no": 3
      title: Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$
      page: 45
      pdf_page: 436
    - "no": 4
      title: Measurable equivalence relations
      page: 46
      pdf_page: 437
    - "no": 5
      title: Disintegration of a measure by a measurable equivalence relation
      page: 50
      pdf_page: 441
statements: 16
exercises: 12
content_sha256: ed8b0805cf0d8a3bec6a56ea3cd6d188887389b1f4aeaa07660b14ea293bbd64
translated_from: content/en/int/VI/03_s3_disintegration_of_measures.md
translation_method: google
source_content_sha256: af4e8435c165da3e46c8e743b1fe384a343285c290d2c1854e12b375334ea66b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 260b897428ae377c0244fec22d41f781672bca514440ebe16aabb40e0cc36c54
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。措施解体

### 1. 测量$\mu$相对于$\mu$-固有映射的分解

令 T 为具有可数基的局部紧致空间（在其他字中，是局部紧致波兰语空间 (GT, IX, §6, No. 1)。我们知道，对于 T 上的每一个正测度，积分和本质积分重合的概念（第 V, §1, No. 3，第 9 条命题）。另一方面，我们有以下属性：

#### 引理 1 {#int-vi-s3-lem-1 .statement tag=09C0}

*如果 Y 是局部紧致空间且具有可数基、空间 $\mathscr{H}(Y)$ 包含以及可数稠密子集。更准确地说，$\mathscr{H}(Y)$中存在函数$\geq 0$的可数子集S由……组成，这样，对于$\mathscr{H}(Y)$的每个函数$f \geq 0$，都存在函数$f_n \in S$的序列 ($n \geq 0$) 一致收敛于$f$，并且对于所有$n \geq 0$ 都是$f_n \leq f_0$。

对于，Y 是相对紧凑的开放集合的递增序列 $(U_n)$ 的并，使得 $\overline{U}_n \subset U_{n+1}$ 对于所有$n$（GT，I, §9, No. 9，命题 15）； 空间$\mathscr{H}(Y)$是Banach空间$\mathscr{H}(Y, \overline{U}_n)$的递增序列的并，并且已知后者中的每一个都是可分离的（GT，Ch.X, §3, No. 3，Th.1）。令$S'_n$为$\varphi \in S'_n$的函数$\varphi^+$的$\mathscr{H}(Y, \overline{U}_n)$、$S_n$集合中的可数稠密集合，以及$\mathscr{H}(Y, \overline{U}_{n+1})$中的$u_n$函数，其中$[0, 1]$ 中值且$U_n$ 中等于 1。我们取$S_n$的S并和$m u_n$的集合为$m$和$n$整数$\geq 0$。对于$\mathscr{H}(Y)$的每一个函数$f \geq 0$，$f$都包含在$U_n$之一中的支持，因此是函数$f_p \in S_n$（$p \geq 1$）的序列的统一极限。这些函数$f_p$统一以正整数$m$为界，取$f_0 = m u_n$就足够了。*

#### 引理 2 {#int-vi-s3-lem-2 .statement tag=09C1}

*如果 T 是具有可数基的局部紧致空间，则连续数值函数在无穷远处点趋于 0 的 Banach 空间 $\mathscr{K}(Y)$ 是可分离的。*

这个引理不是别人，正是Cor。至 Th。 GT 1，X, §3, No. 3。人们可能会发现，它也从引理 1 得出，并且$\mathscr{K}(Y)$ 上一致收敛的拓扑比子空间 $\mathscr{K}(Y, \overline{U}_n)$ 拓扑的直极限拓扑更粗糙。

#### 引理 3 {#int-vi-s3-lem-3 .statement tag=09C2}

— *令 T 和 X 为两个局部紧凑的空间，其中可数基、$\mu$ T 上的正测度，以及 $t \mapsto \lambda_t$ ($t \in T$) X 上的一系列正测度。如果映射 $t \mapsto \lambda_t$ 是 $\mu$ 标量可积（对于拓扑 $\sigma(\mathscr{M}(X), \mathscr{K}(X))$），则族 $t \mapsto \lambda_t$ 是 $\mu$ 充分的（$§ 1$，No. 1， 例).*

因为，引理 1 应用于 $\mathscr{K}(X)$，表明映射 $t \mapsto \lambda_t$ 是模糊地 $\mu$ 可测量的（$§ 1$、No. 5，命题 13）。

#### 定理 1 {#int-vi-s3-thm-1 .statement tag=09C3}

*设 T 和 B 为两个局部紧凑空间，具有可数基、$\mu$ T 的正测度，将 T 的 $\mu$-固有映射（Ch. V, §6, No. 1，定义 1）转换为 B，以及 $\nu = p(\mu)$ 像第 3 页下的 $\mu$则 T 上存在一个 $\nu$ 充分族 ($§ 1$, No. 1, 例) $b \mapsto \lambda_b$ ($b \in B$)，具有以下性质：

a) $\| \lambda_b \| = 1$ 对于所有 $b \in p(T)$；

b) 对于所有 $b \in B$，$\lambda_b$ 集中在集合 $\overline{p}^{-1}(b)$（第 V, §5, No. 7，定义 4）；特别是，$\lambda_b = 0$代表$b \notin p(T)$；

c) $\mu = \int \lambda_b d\nu(b)$。

此外，如果 $b \mapsto \lambda'_b$ ($b \in B$) 是 T 上具有属性 b) 和 c) 的第二个 $\nu$ 充分正测度族，则对于测度 $\nu$，$\lambda'_b = \lambda_b$ 几乎在 B 中随处可见。

1) *唯一性.* 对于每个函数 $f \in \mathscr{K}(B)$，$f \circ p$ 是 $\mu$ 可积的，因为 p 是 $\mu$-固有的（Ch. V, §6, No. 2，Th. 1）；因而，对于每个函数 $g \in \mathscr{K}(T)$，函数 $t \mapsto g(t)f(p(t))$ 是 $\mu$ 可积的。由此得出结论（第 V, §3, No. 3，第 1 章），对于几乎每个 $b \in B$，函数 $t \mapsto g(t)f(p(t))$ 都是 $\lambda_b$ 可积的，并且

$$
\int g(t)f(p(t)) d\mu(t) = \int d\nu(b) \int g(t)f(p(t)) d\lambda_b(t).
$$

但由于 $\lambda_b$ 集中在 $\overline{p}^{-1}(b)$ 上，对于每个 $b \in B$，对于 $\lambda_b$ 几乎到处都有 $f(p(t)) = f(b)$，因而 (1) 的第二个成员等于 $\int f(b)\langle g, \lambda_b \rangle d\nu(b)$。类似的公式对于 $\lambda'_b$ 也成立；因而 $\int f(b)\langle g, \lambda_b \rangle d\nu(b) = \int f(b)\langle g, \lambda'_b \rangle d\nu(b)$ 对于所有 $f \in \mathscr{K}(B)$ 和 $g \in \mathscr{K}(T)$。在其他字中，B到$\mathscr{M}(T)$的两个映射、$b \mapsto \lambda_b$和$b \mapsto \lambda'_b$对于$\nu$几乎处处都局部标量相等，因此对于$\nu$几乎处处相等（引理1和§1, No. 1， 注2)。

2) *家庭临时定义*$b \mapsto \lambda_b$。对于每个函数 $f \in \mathscr{L}^1(\nu)$，$f \circ p$ 是 $\mu$ 可积（Ch. V, §6, No. 2，Th. 1），因而 $(f \circ p) \cdot \mu$ 是 T 上的有界测度，并且

$$
\|(f \circ p) \cdot \mu\| = \int |f \circ p| \, d\mu = \int |f| \, d\nu = N_1(f)
$$

（第 IV, §4, No. 7 章，第 12 条提案；第 V, §5, No. 3 章，第 1 章和 §6, No. 2，第 1 章）。由此可见，$(f \circ p) \cdot \mu$仅依赖于$L^1(\nu)$中$f$的类$\tilde{f}$，并且$\tilde{f} \mapsto (f \circ p) \cdot \mu$是$L^1(\nu)$的*等距*线性映射进入T上有界测度的Banach空间$\mathscr{M}^1(T)$，T的强对偶Banach 空间 $\mathscr{K}(T)$，可分离 (引理 2)。根据 Dunford–Pettis 定理（§2, No. 5，Th. 1 的 Cor.2），存在 B 的映射 $b \mapsto \lambda_b$ 进入 $\mathscr{M}^1(T)$ 的单位球，标量 $\nu$ 可测量（对于拓扑 $\sigma(\mathscr{M}^1(T), \overline{\mathscr{K}(T)})$），对于每个函数 $f \in \mathscr{L}^1(\nu)$，

$$
(f \circ p) \cdot \mu = \int f(b) \lambda_b \, d\nu(b),
$$

也可以写成，对于每个函数 $g \in \overline{\mathscr{K}(T)}$

$$
\int g(t) f(p(t)) \, d\mu(t) = \int f(b) \, d\nu(b) \int g(t) \, d\lambda_b(t).
$$

如果$f \geq 0$和$g \geq 0$，(3)的第一个成员是$\geq 0$，这证明对于$\mathscr{K}(T)$中的每个函数$g \geq 0$，测度$(\int g(t) \, d\lambda_b(t)) \cdot \nu$是$\geq 0$，因此$\int g(t) \, d\lambda_b(t) \geq 0$除了$b$ 属于到 $\nu$-可忽略不计的集合 $N(g)$（第 V, §5, No. 3 章，第 3 号提案第 3 条）。现在，空间$\mathscr{K}_+(T)$中存在函数$\geq 0$$\mathscr{K}(T)$（引理1）的稠密序列$(g_n)$。 $N(g_n)$ 的并 N $\nu$可以忽略不计，对于$b \notin N$，我们对所有$n$有$\int g_n(t) \, d\lambda_b(t) \geq 0$，因此对于每个函数$g \in \mathscr{K}_+(T)$，在其他字中，$\int g(t) \, d\lambda_b(t) \geq 0$ $\lambda_b \geq 0$。

既然如此，我们可以将替换$\lambda_b$每$b \in N$增加0，而不改变（3）的有效性；因此，我们可以假设已经进行了此修改，因此每个$b \in B$都有$\lambda_b \geq 0$。

3) *扩张公式* (3)。

$\alpha)$ 对于每个函数 $f \in \mathscr{L}^1(\nu)$，从 (3) 可以得出，B 的映射 $b \mapsto \lambda_b$ 到 $\mathscr{M}(T)$ 对于测度 $|f \cdot \nu|$ 和拓扑 $\sigma(\mathscr{M}(T), \mathscr{K}(T))$ 是可标量可积的，因此 (引理 3) 族$b \mapsto \lambda_b$是$|f \cdot \nu|$-*足够了*。现在令 $g$ 为在 T 上定义的数值函数，对于测度 $|(f \circ p) \cdot \mu|$ 可积，即 (Ch. V, §5, No. 3, Th. 1)，使得 $t \mapsto g(t)f((p(t)))$ 是 $\mu$ 可积；然后从(2)、Th 得出。第 1 章。 V, §3, No. 3 和来自 Th。第 1 章。 V, §5, No. 3，对于几乎每个 $b \in B$，$g$ 对于 $\lambda_b$ 是可积的，函数（几乎到处定义）$b \mapsto \int g(t)\, d\lambda_b(t)$ 对于 $|f \cdot \nu|$ 是可积的，并且公式 (3) 再次有效。

$\beta)$ 对于每个函数 $g \in \overline{\mathscr{K}(T)}$，从 (3) 得出，应用于 $f \in \mathscr{K}(B)$，映射 $p$ 适合度量 $|g \cdot \mu|$（第 1 章） V, §6, No. 1，防御。 1) 而$g \cdot \mu$测度的$p$下的像是密度$b \mapsto \int g(t)\, d\lambda_b(t)$相对于$\nu$的测度。 如果$f$被取为函数，使得$f \circ p$对于测度$|g \cdot \mu|$可积，也就是说，使得$t \mapsto g(t)f(p(t))$是$\mu$可积（第1章）。 V, §5, No. 3，Th。 1), 公式 (3) 再次有效 (Ch. 1) V, §6, No. 2，Th。 1）。

4) *家庭财产* $b \mapsto \lambda_b$。通过性质$\beta)$，我们可以通过取$f = 1,\ g \in \mathscr{K}(T)$来应用公式（3）；这证明$b \mapsto \lambda_b$是$\nu$标量可积的（对于拓扑$\sigma(\mathscr{M}(T), \mathscr{K}(T))$），因而$\nu$-*足够*（引理3），并且$\mu = \int \lambda_b\, d\nu(b)$。

现在令$\psi$为$\mathscr{K}(B)$中的任意函数； 性质 $\alpha)$ 的条件可以通过取 $f \in \mathscr{K}(B)$ 和 $g = \psi \circ p$ 来满足，因为函数 $\psi(p(t))f(p(t))$ 是 $\mu$ 可积的，因为 $f\psi$ 属于到 $\mathscr{K}(B)$ 和 $p$ 是$\mu$-正确。那么 $\psi \circ p$ 对于几乎每个 $b \in B$ 都是 $\lambda_b$ 可积的，并且

$$
\int f(p(t))\psi(p(t))\, d\mu(t) = \int f(b)\, d\nu(b) \int \psi(p(t))\, d\lambda_b(t);
$$

但第一个成员是定义$\int f(b)\psi(b)\, d\nu(b)$。因而，我们看到对于每个函数 $\psi \in \mathscr{K}(B)$，度量 $\psi \cdot \nu$ 和密度 $b \mapsto \int \psi(p(t))\, d\lambda_b(t)$ 的度量是相同的。因而（第 3 章第 V, §5, No. 3，Cor.2）存在$\nu$ 可忽略的集合 $N'(\psi)$，这样，对于每个 $b \notin N'(\psi)$，函数 $\psi \circ p$ 是 $\lambda_b$ 可积且$\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$。

令 S 为 $\mathscr{K}(B)$ 的可数子集，具有引理 1 中所述的属性（与 $Y = B$），并令 $N'$ 为可忽略的 $\nu$ 集合，即 $\psi \in S$ 的 $N'(\psi)$ 的并。 $\mathscr{K}(B)$的每函数$\psi \geq 0$与$\psi_n \leq \psi_0$是S的元素序列$(\psi_n)$的统一极限。因而，对于$b \notin N'$，勒贝格的定理一方面表明$\psi \circ p$是$\lambda_b$可积，在其他字中$p$是$\lambda_b$可积，另一方面表明$\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$。在其他项、映射 $b \mapsto \varepsilon_b$ 和 $b \mapsto p(\lambda_b)$ 中，B 到 $\mathscr{M}(B)$（后者几乎在所有地方都有定义）对于 $\nu$（以及对于拓扑 $\sigma(\mathscr{M}(B), \mathscr{K}(B))$）来说几乎处处都相等；由此可见，对于 $\nu$，这些映射几乎在任何地方都相等（引理 1 和 §1, No. 1，*注* 2）。最后，如果 $p(\lambda_b) = \varepsilon_b$、集合 $B - \{b\}$ $\varepsilon_b$ 可忽略，则集合 $T - \bar{p}^{-1}(B)$ $\lambda_b$ 可忽略（第 V, §6, No. 2 章，第 2 条的 Cor. 2），在其他字中$\lambda_b$集中于$\overline{p}^{-1}(b)$；另一方面，$\| \lambda_b \| = \int d\lambda_b = \int d((p(\lambda_b))) = \| \varepsilon_b \| = 1$（第 V, §6, No. 2，第 1 章）。

5) *家庭的修改* $b \mapsto \lambda_b$。因而，我们在 T 上定义了 $\geqslant 0$ 的$\nu$-充分族$b \mapsto \lambda_b$，叙述的满足条件c)，这样，对于几乎每个$b \in B$，$p$都是$\lambda_b$-适当的，并且$\lambda_b$集中在$\overline{p}^{-1}(b)$上，并具有范数 1。令$N''$为点$b \in B$的$\nu$可忽略的集合，其中最后三个属性之一未验证；然后我们可以通过以下方式修改$\lambda_b$。若$b \in B - p(T)$，则取$\lambda_b = 0$；如果$b \in p(T) \cap N''$，则取$\lambda_b = \varepsilon_{\xi(b)}$，其中$\xi(b)$是$\overline{p}^{-1}(b)$中的任意点。由于 $B - p(T)$ 是 $\nu$-可以忽略不计（第 V, §6, No. 2 章，提案 2 的 Cor. 3），我们仅在点处修改了 $\lambda_b$ 可忽略不计的集合，因此族 $b \mapsto \lambda_b$ 仍然是 $\nu$-足够的，并且有性质 c)；此外，它现在满足a)和b)，从而完成证明。

T 上的每个$\nu$-充分族$b \mapsto \lambda_b$，具有 Th 的属性 b) 和 c)。 1，据说是相对于$\mu$-适当的映射$p$措施$\mu$的“分解”。

### 2. 伪图像措施

#### 定义 1 {#int-vi-s3-def-1 .statement tag=09C4}

*设 T 和 B 为两个局部紧凑空间，$\mu$ T 上的正测度，并且将 T 的 $\mu$ 可测映射放入 B 中。如果满足以下条件，B 上的正测度 $\nu$ 被称为 p 下 $\mu$ 的伪像测度： B 的子集 N 局部$\nu$-可忽略，$\overline{p}^{-1}(N)$局部$\mu$-可忽略是必要且充分的。*

#### 例 {#int-vi-s3-n2-exa-1 .statement tag=09C5}

— 1) 如果 $p$ 是$\mu$-固有且$\nu = p(\mu)$，则$\nu$ 是$p$ 下$\mu$ 的伪像测度（第 V, §6, No. 2 章，第 2 条的 Cor.2）。

2) 令$B'$为局部紧致空间，$\nu'$为$B'$的正测度；对于 T 空间 $B \times B'$，对于 $\mu$，采取措施 $\nu \otimes \nu'$；如果$p$是T在B上的投影，则$\nu$是$p$下$\mu$的伪像（第V, §8, No. 2章，第4条命题和No. 3，第7条命题的Cor.1）。

注意，如果$\nu$是$\mu$在$p$下的伪像测度，则$\nu$由$p(T)$携带。

如果$\nu$是$p$下$\mu$的伪像，则$\mu$在$p$下的伪像的测度的集合是等价于$\nu$的正测度的类，并且与$\mu$等价的每个正测度都承认相同$p$下的伪图像测量。 $\nu$的类据说是$p$下$\mu$的*伪图像类*。

#### 命题 1 {#int-vi-s3-prop-1 .statement tag=09C6}

— *设 T 为无穷大处可数的局部紧致空间，T 上的正测度$\mu$，以及 T 的 $\mu$ 可测映射 $p$ 为局部紧致空间 B。则在下存在$\mu$ 的伪像测度$p$.*

因为，T 上存在一个“有界”测度 $\mu'$，相当于 $\mu$（第 V, §5, No. 6 章，第 11 条命题）；那么$p$就是$\mu'$-正确的。

### 3. 测量$\mu$相对于$\mu$的伪图像的分解

#### 定理 2 {#int-vi-s3-thm-2 .statement tag=09C7}

— *令 T 和 B 为两个局部紧致空间，具有可数基，$\mu$ T 上的正测度，$p$ T 到 B 的 $\mu$ 可测映射，以及 $\nu$ $p$ 下 $\mu$ 的伪像测度。那么 T 上存在一个$\nu$-充分族$b \mapsto \lambda_b$ ($b \in B$)，具有以下性质：
a) $\lambda_b \neq 0$ 为 $b \in p(T)$；
b) 每$b \in B$，$\lambda_b$集中在集合$\overline{p^{-1}}(b)$；特别是，$\lambda_b = 0$代表$b \notin p(T)$；
c) $\mu = \int \lambda_b \, d\nu(b)$。

此外，如果$\nu' = r \cdot \nu$是$p$下$\mu$的第二个伪像测度，并且如果$b \mapsto \lambda'_b$是T上关于$\nu'$具有属性b）和c）的$\nu'$充分正测度族，则$\lambda_b = r(b)\lambda'_b$几乎在B中无处不在（*对于$\nu$ 或 $\nu'$*)。

T 上存在一个定义的连续且有限的数值函数 $f$，使得对于每个 $t \in T$ 都有 $f(t) > 0$，并且 $\mu'' = f \cdot \mu$ 是有界的（第 V, §5, No. 6，第 11 章）。设$\nu'' = p(\mu'')$，相当于$\nu$，并写成$\nu'' = g \cdot \nu$，$g$有限且$\nu$局部可积；此外，我们可以假设 $g(b) > 0$ 对于所有 $b \in B$（第 V, §5, No. 6 章，命题 10）。 Th。 No. 1的1，应用于$\mu''$和$\nu''$，表明存在T上的积极措施的$\nu''$充分族$b \mapsto \lambda''_b$（$b \in B$），使得：

1) $\| \lambda''_b \| = 1$换$b \in p(T)$；
2）每$b \in B$，$\lambda''_b$集中在$\overline{p^{-1}}(b)$；
3）$\mu'' = \int \lambda''_b \, d\nu''(b)$。

对于每一个$b \in B$，让我们定义在T上通过公式$\lambda_b = (1/f) \cdot (g(b)\lambda''_b)$进行正测量$\lambda_b$。显然，族$b \mapsto \lambda_b$具有叙述的属性a）和b）。另一方面，对于每个函数 $h \in \mathscr{K}(T)$，$h/f$ 属于到 $\mathscr{K}(T)$，因此

$$
\int h(t) \, d\mu(t) = \int (h(t)/f(t)) \, d\mu''(t) = \int d\nu''(b) \int (h(t)/f(t)) \, d\lambda''_b(t).
$$

但由于函数 $b \mapsto \int (h(t)/f(t)) \, d\lambda''_b(t)$ 是 $\nu''$ 可积，函数 $b \mapsto g(b) \int (h(t)/f(t)) \, d\lambda''_b(t)$ 是 $\nu$ 可积（Ch. V, §5, No. 3，Th. 1）。

通过$\lambda_b$的定义，这个函数是$b \mapsto \int h(t) d\lambda_b(t)$，从而（*loc.cit.*）$\int h(t) d\mu(t) = \int d\nu(b) \int h(t) d\lambda_b(t)$，这就证明了$\mu = \int \lambda_b d\nu(b)$。

为了建立叙述的第二个部分，我们可以假设 $r(b) > 0$ 对于所有 $b \in B$（第 V, §5, No. 6，命题 10）； 集合$\lambda'''_b = f \cdot \left( (r(b)/g(b)) \lambda'_b \right)$；如上所示，对于每函数 $h \in \mathscr{K}(T)$，关系

$$
\int h(t) d\mu(t) = \int d\nu'(b) \int h(t) d\lambda'_b(t)
$$

意味着

$$
\int h(t) d\mu(t) = \int d\nu''(b) \int (h(t)/f(t)) d\lambda'''_b(t) .
$$

因此 Th。 No. 1中的1，应用于$\mu''$和$\nu''$，意味着几乎每个$b \in B$，$\lambda'''_b = \lambda''_b$，从而$\lambda_b = r(b)\lambda'_b$。

#### 定义 2 {#int-vi-s3-def-2 .statement tag=09C8}

*令 T 和 B 为两个波兰局部紧空间。给定 T 上的正测度 $\mu$，T 到 B 的 $\mu$ 可测映射 p，以及 p 下 $\mu$ 的伪像测度 $\nu$，T 上正测度的每个 $\nu$ 充分族 $b \mapsto \lambda_b$ ($b \in B$) 都具有以下属性Th 的 b) 和 c)。 2 称为 $\mu$ 相对于 $\nu$ 的分解。*

当$p$是$\mu$-固有且$\nu = p(\mu)$时，相对于$p$的崩解概念因此重合具有相对于$\nu$的崩解概念。在 Th 的假设下。 2、对于$\nu$，$\mu$相对于相同伪图像测量$\nu$的两次分解几乎处处相等。

#### 注 {#int-vi-s3-n3-rem-1 .statement tag=09C9}

— Th。第 1 章。 V, §3, No. 4表明（考虑到T和B具有可数基的事实），对于T上定义的每个函数$f$，其中值在$\overline{\mathbf{R}}$或在Banach空间F和$\mu$可积中，集合 $b \in B$使得$f$不是$\lambda_b$可积，$\nu$可忽略不计，函数$b \mapsto \int f(t) d\lambda_b(t)$几乎到处都有定义，是$\nu$可积，并且

$$
\int f(t) d\mu(t) = \int d\nu(b) \int f(t) d\lambda_b(t) .
$$

类似的结果适用于标量 $\mu$ 可积函数，在 §1, No. 1 的应用命题 3 上。

### 4. 可测量等价关系

给定拓扑空间X和X中的等价关系R，如果商空间X/R是Hausdorff，我们可以说R是*Hausdorff*。

回想一下（GT，I, §8, No. 3，命题 8），当 R 是开等价关系时，同样可以说 R 在 X × X 中的图是闭的。

令 p 为 X 的映射进入豪斯多夫拓扑空间 B，并令 R 为 X 中的等价关系 $p(x) = p(y)$；如果 K 是 X 的紧子集，使得 p 到 K 的限制是连续的，则 R 在 K 上诱导的关系 $R_K$ 是 Hausdorff，因为商空间 $K / R_K$ 同胚于空间 $p(K)$，紧凑（GT、I, §9, No. 4、Th.2 及其 Cor.2）。如果 T 是局部紧致空间，$\mu$ 是 T 的正测度，并且 p 是 T 到 Hausdorff 拓扑空间 B 的 $\mu$ 可测映射，因此可以看出存在$\mu$ 稠密集合（第 1 章）。 T 的紧凑子集 K 的IV, §5, No. 8)，其中关系 $R_K$ 是 Hausdorff。因此，我们做出以下定义：

#### 定义 3 {#int-vi-s3-def-3 .statement tag=09CA}

*设 T 为局部紧致空间，$\mu$ T 上的正测度。如果存在 T 的紧致子集 K 的 $\mu$ 稠密集合 K，则称 T 中的等价关系 R 是 $\mu$ 可测的。 关系 $R_K$ 是豪斯多夫。*

如果 R 是 Hausdorff，则 R 是 $\mu$ 可测的，因为如果 $\varphi$ 是 T 的典范映射到 Hausdorff 拓扑空间 T/R，则$\varphi$ 是连续的，并且 R 等效于 $\varphi(x) = \varphi(y)$。类似地，如果 R 使得 T 的每个紧凑子集的 R 的饱和度是封闭的（特别是，如果 R 是封闭的等价关系），则 R 是 $\mu$ 可测的，因为对于 T 的每个紧凑子集 K，关系 $R_K$ 是封闭的，因此 Hausdorff (GT, I, §10, No. 4，提案 8）。

请注意，如果 R 是 $\mu$ 可测的，那么对于 T 上具有基 $\mu$ 的每个测度，R 也是可测的。

#### 命题 2 {#int-vi-s3-prop-2 .statement tag=09CB}

*令 T 为无穷大处可数的局部紧致空间，$\mu$ T 的正测度。

1) 对于 T 中的每个 $\mu$ 可测等价关系 R，都存在一个局部紧致空间 B 和 T 到 B 的 $\mu$ 可测映射 p，使得 R 等价于关系 $p(x) = p(y)$。

2) 此外，如果 T 承认可数基，则可以假设 B 承认可数基。*

由于 T 在无穷大处可数，存在 T 的紧凑子集的递增序列 $(K_n)_{n \geq 1}$，使得 T 是 $K_n$ 的并和$\mu$-可忽略的集合 N，并且使得每个关系 $R_{K_n}$ 是豪斯多夫。令 $B_n$ 为商空间 $K_n / R_{K_n}$，这是紧致的，并令 $B'_n$ 为紧致空间，即 $B_n$ 和点 $a_n$ 的拓扑和。设$q_n$是$K_n$的典范映射到$B_n$；我们通过以下方式将 T 的扩展 $q_n$ 到映射 $p_n$ 转换为 $B'_n$：如果 $x \in T$ 等价于 mod R 到元素 $y \in K_n$，集合 $p_n(x) = q_n(y)$；相反，集合$p_n(x) = a_n$。

令 $B'$ 为乘积空间 $\prod_{n=1}^{\infty} B'_n$，这是紧致的，并令 $p'$ 为 T 到 B' 的映射 $x \mapsto (p_n(x))$。让我们证明$p'$是$\mu$可测的：它足以证明映射$p_n$中的每一个都是可测的（Ch.IV, §5, No. 3，Th.1），并且为此，$p_n$的限制对于每个限制就足够了$K_m$是可测量的。现在，如果 $m \leq n$; 就很明显了；相反，如果$m > n$，则令$K_{nm}$为$K_n$对$R_{K_m}$的饱和度，这是$K_m$的紧凑子集（GT，I, §9, No. 4，Th.2）；由于$p_n$在$K_m - K_{nm}$上恒定，因此足以证明$p_n$到$K_{nm}$的限制是连续的，这在$K_{nm}/R_{K_{nm}}$和$K_n/R_{K_n}$之间的典范同构是明显的（GT，I, §9, No. 4，Cor.4） 2）。

令 A 为关系 R 的 $\bigcup_n K_n$ 饱和度，并令 $N' = T - A \subset N$。我们将看到关系$p'(x) = p'(y)$等价于关系«$R\{x, y\}$或$(x, y) \in N' \times N'$»。对于，如果 $R\{x, y\}$ 那么 $p_n(x) = p_n(y)$ 对于所有 $n$，因而 $p'(x) = p'(y)$；如果 $x \in N'$，$y \in N'$，那么对于所有 $n$ 来说，$p_n(x) = p_n(y) = a_n$，因而$p'(x) = p'(y)$。另一方面，如果 $x$ 和 $y$ 在 A 中且不等价 mod R，则存在整数 $n$、元素 $x' \in K_n$（分别为 $y' \in K_n$）等价 mod R 到 $x$（分别为 $y$），使得$x'$ 不等于 $y'$ mod $R_{K_n}$；因而$p_n(x) \neq p_n(y)$，因而$p'(x) \neq p'(y)$。最后，如果$x \in N'$和$y \in A$，那么$p_n(y) \in B_n$代表$n$足够大，$p_n(x) = a_n$代表所有$n$，因而$p'(x) \neq p'(y)$，这建立了我们的断言。

然后考虑商集$B_0 = N'/R_{N'}$；让$q_0$是$N'$的典范映射到$B_0$，$s_0$截面到$q_0$。 集合 $p_0(x) = s_0(q_0(x))$ 对于 $x \in N'$ 和扩展 $p_0$ 到 T，通过将 $p_0$ 在 A 上设为等于 T 的元素的常数。则 $p = (p', p_0)$ 是 T 的 $\mu$ 可测映射，局部紧凑空间 $B = B' \times T$；如果 $x \in N'$、$y \in N'$、关系 $p_0(x) = p_0(y)$ 蕴含$R\{x, y\}$，则为直接的；因而$p$满足要求。此外，如果 T 承认可数基，则商空间 $B_n$ 中的每一个也承认（GT，IX, §2, No. 10，命题 17），因而 B' 承认可数基，因而 B 也是如此。

#### 命题 3 {#int-vi-s3-prop-3 .statement tag=09CC}

— *设 T 为波兰局部紧空间，$\mu$ T 上的正测度，T 中的 R 等价关系。以下属性是等效的：*

a) $R$ 是 $\mu$ 可测量的。

b) *在豪斯多夫拓扑空间中存在映射$p_n : T \to F_n$的序列，使得每个$p_n$都是$\mu$可测，并且关系$R\{x, y\}$等价于«对于所有$n$， $p_n(x) = p_n(y)$».*

c) *存在 $\mu$ 可测量集合的序列 $(A_n)$，对于 R 饱和，使得对于 R 而言，x 的每个 $x \in T$ 类是那些 $A_n$ 的交包含 x。*

与b)的叙述中的记号、集合$p(x) = (p_n(x))$； 性质 b) 表示 T 到乘积空间 $\prod F_n$ 的映射 $p$ 是可测量的（Ch. IV, §5, No. 3，Th. 1），并且关系 $R\{x, y\}$ 相当于$p(x) = p(y)$；因此 b) 意味着 a)。

接下来让我们证明 c) 蕴涵 b)。假设c)已验证；那么特征函数 $\varphi_{A_n}$ 是 $\mu$ 可测量的，并且假设 c) 意味着关系 $R\{x, y\}$ 相当于 «对于每个 $n$, $\varphi_{A_n}(x) = \varphi_{A_n}(y)$»。

最后，让我们证明 a) 蕴涵 c)。根据命题 2，存在一个局部紧致空间 B，其中可数基，以及 T 到 B 的 $\mu$ 可测映射 $p$，使得关系 $R\{x, y\}$ 等价于 $p(x) = p(y)$。令 $(U_n)$ 为 B 的拓扑的可数基。集合 $A_n = \overline{p^{-1}(U_n)}$ 为 $\mu$ 可测（第 IV, §5, No. 5，第 7 章）且对于 R 是饱和的；如果$x, y$是T的点使得$p(x) \neq p(y)$，则存在指标$n$使得$p(x) \in U_n$和$p(y) \notin U_n$，这意味着$x \in A_n$和$y \notin A_n$。

#### 注 {#int-vi-s3-n4-rem-1 .statement tag=09CD}

如果 R 是 T 中的 $\mu$ 可测等价关系，则 T 的紧凑子集的 R 饱和度不一定是 $\mu$ 可测（例 5）。

#### 定理 3 {#int-vi-s3-thm-3 .statement tag=09CE}

— *令 T 为局部紧致空间，具有可数基、$\mu$ T 上的正测度，且 R 在 T 中为 $\mu$ 可测等价关系。那么，存在 T 的 $\mu$ 可测子集 S，与每个相交类相对于 R 而言，只有一个点（R 的“可测量截面”）。*

我们可以清楚地假设测度$\mu$是有界的，而$\mu(T) \leq 1$（第V, §5, No. 6章，命题11）。我们将对 *Borel* 子集 (GT, IX, §6, No. 3) 的定义序列 $(S_n)$ 进行计算，使得关于 R 的每个等价类与 $S_n$ 的并 $S'$ 相交至多一个点，对于每个$n$，$S_p$与指标$p \leq n$的并的饱和度$T_n$是可测量的$\mu$，并且$\mu(T - T_n) \leq 1/2^n$。因此，$S'$的饱和度$T'$将是$\mu$可测量的，并且$N = T - T'$将具有测量零。如果$S''$是关系$R_N$的N中的任何截面，则$S = S' \cup S''$将满足要求，因为$S'$是Borel集合，是$\mu$可测量（第IV, §5, No. 4，Cor.3） Th 2)，并且 $S''$ 的度量为零。

根据命题2，$R\{x, y\}$等价于关系$p(x) = p(y)$，其中$p$是T的$\mu$可测量映射到局部紧致空间F。假设为$k \leq n$定义了$S_k$。由于$T - T_n$是$\mu$可测且测度为$\leq 1/2^n$，因此存在$T - T_n$的紧子集 K，使得$\mu(T - (T_n \cup K)) \leq 1/2^{n+1}$且$p$到K的限制是连续的。由于诱导的关系 $R_K$ 是封闭的并且 K 是可度量的，我们知道存在 K 的 Borel 子集 $S_{n+1}$，使得在 K 中，每个点等价于 (mod R) 一个且唯一一个 $S_{n+1}$ 的点 (GT, IX, §6, No. 8， Th.4）。因此$p(S_{n+1}) = p(K)$，即F中的紧集； R 的 $S_{n+1}$ 饱和度为逆像 $\overline{p^{-1}(p(K))}$，因此是 μ 可测的（第 IV, §5, No. 5 章，第 7 条）；很明显，这个集合包含K，因此T_n和$\overline{p}^{-1}(p(K))$的并T_{n+1}是μ可测的，对于R是饱和的，并且使得$\mu(T - T_{n+1}) \leq 1/2^{n+1}$，从而完成证明。

### 5. 通过可测量的等价关系来分解测量

设 T 为波兰局部紧致空间，$\mu$ T 上的正测度，R 为 T 中的 $\mu$ 可测等价关系。则存在（No. 4，命题 2）波兰局部紧致空间 B 和 $\mu$ 可测将 T 的映射 p 转换为 B，使得关系 $p(x) = p(y)$ 等价于 R$\{x, y\}$。每个测度 $\nu$ 是 $\mu$ 在 p (No. 2) 下的伪像，将通过关系* R 称为 $\mu$ 的 *商测度；如果$b \mapsto \lambda_b$是$\mu$相对于测度$\nu$的分解，我们可以说$b \mapsto \lambda_b$是关系* R对$\mu$的分解。凭借p和$\lambda_b$的属性，每个测度$\lambda_b$集中于等价类相对于 R，如果 $b \neq c$，则度量 $\lambda_b$ 和 $\lambda_c$ 集中在不同的类上。

空间 B、映射 p 和 B 上的伪像测度 $\nu$ 通常可以通过无限多种方式进行选择。然而，R对$\mu$的各种分解都可以从其中之一推导出来，如以下定理的推论：

#### 定理 4 {#int-vi-s3-thm-4 .statement tag=09CF}

*设 T 为 T 上的波兰局部紧致空间，$\mu$ T 的正测度，R 为 T 中的$\mu$可测等价关系。设 B、B' 为 T 到 B 中的两个波兰局部紧致空间，p，p' 两个$\mu$可测映射，分别为 B'，使得 R$\{x, y\}$ 等于 $p(x) = p(y)$ 和$p'(x) = p'(y)$。令$\nu, \nu'$分别为$\mu$在p、p'下的伪像测度；令$b \mapsto \lambda_b, b' \mapsto \lambda_{b'}$分别为$\mu$相对于$\nu, \nu'$的分解。*

*在这些条件下，B（分别为B'）中存在集合N（分别为N'），对于$\nu$（分别为$\nu'$）和双射f，B - N到B' - N'上的f可以忽略不计，具有以下属性：*

a) *映射 f（在 B 中几乎所有地方都有定义）是 $\nu$ 可测的，其逆映射 $f'$ 是 $\nu'$ 可测的； f（分别 $f'$）下 $\nu$（分别 $\nu'$）的每个伪像度量都相当于 $\nu'$（分别 $\nu$）。*

b) *对于每个$b \in B - N$，T 上的$\lambda'_{f(b)}$测度为形式$r(b)\lambda_b$，其中$r(b) \neq 0$和r是局部$\nu$可积的。*

为了建立 a)，我们可以将极限应用于 $\nu$ 和 $\nu'$ 是*有界*测度的情况（第 V, §5, No. 6，第 11 章）。设$N_0 = B - p(T)$，$N'_0 = B' - p'(T)$；我们知道，$N_0$（或$N'_0$）对于$\nu$（或$\nu'$）（No. 2）可以忽略不计。对于所有 $t \in T$，存在由 $f(p(t)) = p'(t)$ 定义的 B - $N_0$ 到 B' - $N'_0$ 的双射 f；令$f'$为$f$的逆映射，从而得到$f'(p'(t)) = p(t)$。对于 B 的每个子集 M，关系 « M 是 $\nu$ 可测量 » 等价于 « $\overline{p}^{-1}(M)$ 是 $\mu$ 可测量 »，即 « $p'(f(M))$ 是 $\mu$ 可测量 »，因此最终到 « $f(M)$ 是$\nu'$-可测量 »（第 V, §6, No. 2 章，第 3 号提案的Cor.）。因而，我们看到$f$（分别为$f'$）变换每个$\nu$可测量（分别为$\nu'$可测量）集合转换为$\nu'$可测量（分别为$\nu$可测量） 集合；由于 B 和 $B'$ 是可测量的并且具有可数基，因而 $f$ 和 $f'$ 是可测量的（Ch. IV, §5, No. 5，Th. 4）。此外，如果 $M \subset B$ 是 $\nu$-可忽略，则 $\overline{p}^{-1}(M) = p'(f(M))$ 是 $\mu$-可忽略，因而 $f(M)$ 是 $\nu'$-可忽略（第 V, §6, No. 2 章，第 2 条 Cor.2）；同样，$f'$变换每$\nu'$可忽略不计的集合变成$\nu$可忽略不计的集合。因而，$f$下$\nu$的像（由于$\nu$有界而定义，这意味着$f$是$\nu$-固有的）等价于$\nu'$，并且在$\nu'$下的像等价$f'$ 相当于 $\nu$（第 V, §5, No. 6 章，第 10 条提案）。仍有待证明b)。凭借Th。 No. 3中的第2个，我们可以将自己限制在$\nu' = f(\nu)$的情况。从$\mu = \int \lambda_{b'}' d\nu'(b')$开始，对于每一个函数$h \in \mathscr{K}(T)$，

$$
\int h(t) d\mu(t) = \int d\nu'(b') \int h(t) d\lambda_{b'}'(t) = \int d\nu(b) \int h(t) d\lambda_{f(b)}'(t)
$$

（第 V, §3, No. 4、第 1 章和第 §6, No. 2、第 1 章）；其他字，$\mu = \int \lambda_{f(b)}' d\nu(b)$。但由于 $\mu = \int \lambda_b d\nu(b)$ 和之后，对于每个 $b \in B - N_0$、$\lambda_b$ 和 $\lambda_{f(b)}'$ 都由 $\overline{p}^{-1}(b)$、Th 承载。 No. 3 的 2 意味着几乎每个$b \in B - N_0$都有$\lambda_b = \lambda_{f(b)}'$，因此几乎每个$b \in B$。 Th 的条件。因此，通过取$N_0$的N并和$b \in B$的集合来验证4，使得$\lambda_b \neq \lambda_{f(b)}'$。

### 习题 {#int-vi-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
