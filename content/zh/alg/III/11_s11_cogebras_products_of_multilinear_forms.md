---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 11
section_title: Cogebras, products of multilinear forms, inner products and duality
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 574-611, 647-654
pdf_pages: 0598-0635, 0671-0678
extraction: ocr
subsections:
    - "no": 1
      title: COGEBRAS
      page: 574
      pdf_page: 598
    - "no": 2
      title: COASSOCIATIVITY, COCOMMUTATIVITY, COUNIT
      page: 578
      pdf_page: 602
    - "no": 3
      title: PROPERTIES OF GRADED COGEBRAS OF TYPE N
      page: 584
      pdf_page: 608
    - "no": 4
      title: BIGEBRAS AND SKEW-BIGEBRAS
      page: 585
      pdf_page: 609
    - "no": 5
      title: THE GRADED DUALS $T(M)^{*gr}$, $S(M)^{*gr}$ AND $\bigwedge(M)^{*gr}$
      page: 587
      pdf_page: 611
    - "no": 6
      title: 'INNER PRODUCTS: CASE OF ALGEBRAS'
      page: 594
      pdf_page: 618
    - "no": 7
      title: 'INNER PRODUCTS: CASE OF COGEbras'
      page: 597
      pdf_page: 621
    - "no": 8
      title: 'INNER PRODUCTS: CASE OF BIGEBRAS'
      page: 600
      pdf_page: 624
    - "no": 9
      title: INNER PRODUCTS BETWEEN $T(M)$ AND $T(M^*)$, $S(M)$ AND $S(M^*)$, $\Lambda(M)$ AND $\Lambda(M^*)$
      page: 603
      pdf_page: 627
    - "no": 10
      title: EXPLICIT FORM OF INNER PRODUCTS IN THE CASE OF A FINITELY GENERATED FREE MODULE
      page: 605
      pdf_page: 629
    - "no": 11
      title: ISOMORPHISMS BETWEEN $\wedge^p(M)$ AND $\wedge^{n-p}(M^*)$ FOR AN $n$-DIMENSIONAL FREE MODULE M
      page: 607
      pdf_page: 631
    - "no": 12
      title: APPLICATION TO THE SUBSPACE ASSOCIATED WITH A p-VECTOR
      page: 608
      pdf_page: 632
    - "no": 13
      title: PURE $p$-VECTORS. GRASSMANNIANS
      page: 609
      pdf_page: 633
statements: 40
exercises: 25
content_sha256: 6c4e9d6e5ab5cf33417f3e68c92853e42e9a88d445b294d1a22d9c5077e25b9b
translated_from: content/en/alg/III/11_s11_cogebras_products_of_multilinear_forms.md
translation_method: google
source_content_sha256: d9e2a61c3971782f685be044252b3450406801250b05574efb54eb00ac04501c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: ec45d76afbea11a2dd0c700e246b2615566e5a5663d1b0f9da8bb234079a787f
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 11。 余代数、乘积多重线性形式、内部乘积和对偶

在本段中，A 是交换环，具有平凡的毕业。对于型 N 的分级 A-模 M，M^{gr} 将表示型 N 的分级 A-模，其次数 n 的齐次元素是 A 线性形式，对于所有 k ≠ n，其在 M_k 上为零。

### 1.余代数

#### 定义 1 {#alg-iii-s11-def-1 .statement tag=067H}

A 上的余数 a（或 A-余数，或者如果不会引起混淆，则简称为余数 a）是集合 E，其中结构定义如下：
(1) E 上的 A-模结构；
(2) A-线性映射 c: E → E ⊗_A E 称为 E 的余积。

#### 定义 2 {#alg-iii-s11-def-2 .statement tag=067I}

给定两个余代数 E，E'，其余积分别用c和c'表示，E到E'的态射是A-线性映射 u: E → E'，使得
(1) $(u \otimes u) \circ c = c' \circ u,$在其他字中，它使得A-线性映射可交换图表

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow c & & \downarrow c' \\
E \otimes_A E & \xrightarrow{u \otimes u} & E' \otimes_A E'
\end{array}
$$

立即验证恒等映射是态射，两个态射的合成是态射，并且每个双射态射是同构。

#### 例 {#alg-iii-s11-n1-exa-1 .statement tag=067J}

(1) 典范同构 $A \to A \otimes_A A$ (II, § 3, no. 5) 定义 A 上的 A 代数结构。

(2) 设 E 为余代数，$c$ 为余积，$\sigma$ A-模 $E \otimes_A E$ 的规范自同构，使得 $\sigma(x \otimes y) = y \otimes x$ 为 $x \in E, y \in E$； A-线性映射 $\sigma \circ c$ 定义 E 上的新余代数结构。这样结构 E 被称为给定余代数 E 的*相反* 余代数。

(3) 令 B 为 A-*代数*，并令 $m : B \otimes_A B \to B$ 为 A-线性映射，在 B (§ 1, no. 3) 上定义乘法。那么转置$^t m$就是A-模B的对偶$B^*$到A-模$B \otimes_A B$的对偶$(B \otimes_A B)^*$的A-线性映射。如果 B 也是*有限生成射影* A-模，则典范映射 $\mu : B^* \otimes_A B^* \to (B \otimes_A B)^*$ 是 A-模同构 (II, § 4, no. 4)； 映射$c = \mu^{-1} \circ ^t m$则余积在A-模B的*对偶*$B^*$上定义*余代数*结构。

(4) 令X为X的形式线性组合或元素的集合、$A^{(X)}$A-模，系数在A(II, § 1, no. 11)和$A^{(X)}$的$(e_x)_{x \in X}$典范基。 A-线性映射$c : A^{(X)} \to A^{(X)} \otimes_A A^{(X)}$由条件$c(e_x) = e_x \otimes e_x$定义，因此在$A^{(X)}$上获得规范的余代数结构。

(5) 令M为M(§ 5, no. 1)的A-模和$T(M)$张量代数； II, § 3, no. 9 A-模 $T(M)$ 中存在且仅有一个 A-线性映射 $c$ 进入A-模 $T(M) \otimes_A T(M)$，使得对于所有 $n \geq 0$，

$$
c(x_1 x_2 \ldots x_n) = \sum_{0 \leq p \leq n} (x_1 x_2 \ldots x_p) \otimes (x_{p+1} \ldots x_n)
$$

对于所有$x_i \in M$（$x_1 x_2 \ldots x_n$表示代数$T(M)$中的乘积）。因此 $T(M)$ 被赋予 *余代数* 结构。

(6) 令M为A-模且$S(M)$为M的对称代数(§ 6, no. 1)； M 到 $M \times M$ 的对角线映射 $\Delta : x \mapsto (x, x)$ 是 A-线性映射，因此，A-代数 $S(M)$ 的对应同态 $S(\Delta)$ 到 A-代数 $S(M \times M)$ (§ 6, no. 2， 命题3）。 另一方面，在§ 6, no. 6中我们定义了规范分级代数同构$h : S(M \times M) \to S(M) \otimes_A S(M)$；因此，通过合成，我们得到 *A-代数* 同态

$$
c = h \circ S(\Delta) : S(M) \to S(M) \otimes_A S(M),
$$

从而在 $S(M)$ 上定义一个 *余代数* 结构。对于所有$x \in M$，通过§ 6, no. 6中给出的$h$的定义$S(\Delta)(x) = (x, x)$和定义表明

$$
h((x, x)) = x \otimes 1 + 1 \otimes x.
$$

由此可见 $c$ 是唯一代数同态，因此，对于所有 $x \in M$，

(4)
$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

由于$c$是代数同态，因此对于$n$元素或$M$的每个序列$(x_i)_{1 \leq i \leq n}$，

(5)
$$
c(x_1 x_2 \ldots x_n) = \prod_{i=1}^n (x_i \otimes 1 + 1 \otimes x_i)
$$
$$
= \sum (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}})
$$

(5) 右侧的求和覆盖严格递增的序列的所有有序对（在某些情况下为空）

$$
i_1 < i_2 < \cdots < i_p, \quad j_1 < j_2 < \cdots < j_{n-p}
$$

$\{1, n\}$的元素，其元素的集合互补。 元素 $c(x_1 x_2 \ldots x_n)$ 是 $S(M) \otimes_A S(M)$ 中 *总计次数* $n$ 的元素，其二度 $(p, n-p)$ 的分量为

(6)
$$
\sum_{\sigma} (x_{\sigma(1)} \ldots x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \ldots x_{\sigma(n)})
$$

其中对所有置换 $\sigma \in S_n$ 进行求和，即每个间隔 $\{1, p\}$ 和 $\{p+1, n\}$ 中的 *递增*。

(7) 令$M$为$A$模，并继续处理外部代数$\Lambda(M)$，如*例* 6中的$S(M)$一样；这次将 $A$-代数 $\Lambda(M)$ 的对角线映射 $\Delta : M \to M \times M$ 定义同态 $\Lambda(\Delta)$ 引入$A$-代数 $\Lambda(M \times M)$ (§ 7, no. 2, 命题 2)；另一方面，有一个规范的分级代数同构

$$
h : \Lambda(M \times M) \to \Lambda(M)^g \otimes_A \Lambda(M)
$$

(§ 7, no. 7, 命题 10), 从而到合成有一个 *代数* 同态 $c = h \circ \Lambda(\Delta) : \Lambda(M) \to \Lambda(M)^g \otimes_A \Lambda(M)$，它可以被视为$A$-模块同态 $\Lambda(M) \to \Lambda(M) \otimes_A \Lambda(M)$，因此定义位于$\Lambda(M)$一个*余代数*结构。可以如*例* 6 中那样证明$c$ 是唯一代数同态，这样，对于所有$x \in M$，

(7)
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$

从而，对于$M$的元素的每个序列$(x_i)_{1 \leq i \leq n}$，
$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = (x_1 \otimes 1 + 1 \otimes x_1) \wedge \ldots \wedge (x_n \otimes 1 + 1 \otimes x_n)
$$
其中右侧的乘积取自代数
$$
\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M);
$$
对于计算这个乘积，考虑，对于严格递增的序列$i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$、$[1, n]$的元素的每个有序对，其元素的集合互补，乘积 $y_1 y_2 \ldots y_n$，其中$y_{i_h} = x_{i_h} \otimes 1$ ($1 \leq h \leq p$) 和$y_{j_k} = 1 \otimes x_{j_k}$ ($1 \leq k \leq n - p$) 以及和取代了所有这些乘积。由于分级代数$\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$是反交换的，元素$x_i \otimes 1$和$1 \otimes x_i$总共次数1，由§ 4, no. 6，引理3和引理1组成，
$$(8)\quad c(x_1 \wedge x_2 \wedge \cdots \wedge x_n)$$
$$
= \sum (-1)^v (x_{i_1} \wedge \cdots \wedge x_{i_p}) \otimes (x_{j_1} \wedge \cdots \wedge x_{j_{n-p}})
$$
$v$是有序对$(h, k)$的数，使得$j_k < i_h$并且求和与(5)中相同的集合相同。 元素 $c(x_1 \wedge \cdots \wedge x_n)$ 是 $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ 中*总计次数* $n$，其二度 $(p, n - p)$ 的齐次分量等于
$$(9)\quad \sum_{\sigma} \varepsilon_\sigma (x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \wedge \cdots \wedge x_{\sigma(n)})
$$
对置换 $\sigma \in S_n$ 进行求和，每个区间*递增*$[1, p]$ 和 $[p + 1, n]$。

当将来我们将$A^{(x)}, T(M), S(M)$或$\bigwedge(M)$称为*余代数*时，我们的意思是，另外提到的除非，而余代数结构分别定义在*例* 4、5、6和7中。

(8) 设$E, F$为两个$A$代数，$c, c'$分别为余积。让$\tau : (E \otimes_A E) \otimes_A (F \otimes_A F) \to (E \otimes_A F) \otimes_A (E \otimes_A F)$表示结合性同构，使得$\tau((x \otimes x') \otimes (y \otimes y')) = (x \otimes y) \otimes (x' \otimes y')$代表$E$中的$x, x'$，以及$F$中的$y, y'$。然后复合线性映射
$$
E \otimes_A F \xrightarrow{c \otimes c'} (E \otimes_A E) \otimes_A (F \otimes_A F) \xrightarrow{\tau} (E \otimes_A F) \otimes_A (E \otimes_A F)
$$
$A$模块$E \otimes_A F$上的定义余代数结构，称为余代数$E$和$F$的*张量积*。

令 $E$ 为余代数且 $\Delta$ 为可交换幺半群。如果 $c$ 是分级的次数 $O$ 的分级同态，则 $A$ 模块 $E$ 上的分级 $(E_\lambda)_{\lambda \in \Delta}$ 据说与余积* $c$ $E$ 相容的$A$-模块$E$进入分级$A$-模块（型$\Delta$）$E \otimes_A E$，在其他字（II, § 11, no. 5）如果
$$(10)\quad c(E_\lambda) \subset \sum_{\mu + \nu = \lambda} E_\mu \otimes_A E_\nu.$$

在下文中，我们最常关注极限与余积兼容的型$\mathbf{N}$的毕业；具有此类分级的 cogebrà 也称为*分级 cogebrà*。如果 F 是另一个分级余数，则 *分级余数态射* $\phi : E \to F$ 由定义得到一个余数态射 (定义 2)，它也是次数* 0 的分级余数同态 A-模。

#### 例 {#alg-iii-s11-n1-exa-2 .statement tag=067K}

(9) 上述定义的余代数、$T(M)$、$S(M)$、$\Lambda(M)$分级为余代数，为直接的。

### 2.共关联性，共交换性，余单位

令E为余数，$c$其余积、N、$N'$、$N''$三个A-模和$m$是$N \times N'$到$N''$的双线性映射。让$\tilde{m} : N \otimes_A N' \to N''$表示A-线性映射相应的到$m$。如果$u : E \to N$、$v : E \to N'$是两个A-线性映射，我们推导A-线性映射$u \otimes v : E \otimes_A E \to N \otimes_A N'$以及E的复合A-线性映射到$N''$：

$$
m(u, v) : E \xrightarrow{c} E \otimes_A E \xrightarrow{u \otimes v} N \otimes_A N' \xrightarrow{\tilde{m}} N''.
$$

显然，我们已经定义了$\mathrm{Hom}_A(E, N) \times \mathrm{Hom}_A(E, N')$到$\mathrm{Hom}_A(E, N'')$的A双线性映射$(u, v) \mapsto m(u, v)$。

当E是分级代数时，N，$N'$，$N''$将相同型的A-模分级，并将$\tilde{m}$将$N \otimes_A N'$的次数k的同态分级为$N''$，则，如果$u$ （分别$v$）是次数$p$的分级同态（分别$q$），$m(u, v)$是次数$p + q + k$的分级同态。

#### 例 {#alg-iii-s11-n2-exa-1 .statement tag=067L}

(1) 取E为分级余数$T(M)$(no. 1)，并假设N、$N'$、$N''$具有平凡的分级。将次数的同态、$T(M)$的$-p$分级为N（分别为$N'$、$N''$），然后将对应分级为$M^p$的多线性映射为N（分别为$N'$、 $N''$）。给定一个多线性映射 $u : M^p \to N$ 和一个多线性映射 $v : M^q \to N'$，上面的方法允许我们推导出一个多线性映射 $m(u, v) : M^{p+q} \to N''$，称为 *乘积* （相对于 $m$） $u$ 和 $v$。 公式 (3) (no. 1) 和 (11) 表明，对于 M 中的 $x_1, \ldots, x_{p+q}$，

$$
(m(u, v))(x_1, \ldots, x_{p+q}) = m(u(x_1, \ldots, x_p), v(x_{p+1}, \ldots, x_{p+q})).
$$

(2) 取E为分级代数$S(M)$(no. 1)，对N、$N'$、$N''$保持相同的假设。将次数的同态、$S(M)$的$-p$分级为N，然后将对应分级为$M^p$的*对称多线性映射*到N（§ 6, no. 3）。然后，我们从对称多线性映射 $u : M^p \to N$ 和对称多线性映射 $v : M^q \to N'$ 导出对称多线性映射 $m(u, v) : M^{p+q} \to N''$，也用 $u._m v$ （甚至$u.v$）表示（以避免混淆），并称为 *对称$u$和$v$的乘积*（相对于$m$）。 公式 (6) (no. 1) 和 (11) 表明，对于 M 中的 $x_1, \ldots, x_{p+q}$，

$$(u \cdot_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

对置换 $\sigma \in \mathfrak{S}_{p+q}$ 进行求和，在$[1, p]$ 和 $[p+1, p+q]$ 的每个区间上为递增。

(3) 取E为分级余代数$\bigwedge(M)$(no. 1)。然后我们从交错的多重线性映射 $u : M^p \to N$ 和交错的多重线性映射 $v : M^q \to N'$ 交错的多重线性映射 $m(u, v) : M^{p+q} \to N''$ 类似地推导，也表示为 $u \wedge_m v$ 或$u \wedge v$并称为$u$和$v$的*交错的乘积*（相对于$m$）。 公式 (9) (no. 1) 和 (11) 在这种情况下表明，对于 $M$ 中的 $x_1, \ldots, x_{p+q}$，

$$(u \wedge_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma \varepsilon_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

再次对置换$\sigma \in \mathfrak{S}_{p+q}$求和，在$[1, p]$和$[p+1, p+q]$的每个区间上，递增。

我们回到E是任意分级的余代数（型N）的情况，并假设三个模N，N'，N''都等于型$\mathbf{Z}$，映射的*分级A-代数*B的基础A-模 $m$在B中为乘法，因此$\tilde{m} : B \otimes_A B \to B$是次数0的分级A-线性映射。因此，在分级A-模$\mathrm{Homgr}_A(E, B) = C$上获得*分级A-代数*结构。

特别是，假设$B = A$（具有简单的分级），因此$\mathrm{Homgr}_A(E, A)$是*分级对偶*$E^{*gr}$，因此具有分级A-代数结构。

令 F 为另一个，分级为余代数 $c'$，其余积和 $\phi : E \to F$ 分级为余代数态射 (no. 1)；那么规范分级态射

$$\tilde{\phi} = \mathrm{Hom}(\phi, 1_B) : \mathrm{Homgr}_A(F, B) \to \mathrm{Homgr}_A(E, B)$$

是*分级代数同态*。对于$\mathrm{Homgr}_A(F, B)$和$x \in E$中的$u, v$，

$$(\tilde{\phi}(uv))(x) = (uv)(\phi(x)) = m((u \otimes v)(c'(\phi(x)))).$$

但到假设$c'(\phi(x)) = (\phi \otimes \phi)(c(x))$，因此

$$(u \otimes v)(c'((x))) = (\tilde{\phi}(u) \otimes \tilde{\phi}(v))(c(x))$$

因此$\tilde{\phi}(uv) = \tilde{\phi}(u)\tilde{\phi}(v)$，这证明了我们的断言。

特别地，分级转置$^t\phi : F^{*gr} \to E^{*gr}$是分级代数同态。

#### 注 {#alg-iii-s11-n2-rem-1 .statement tag=067M}

假设$E_p$是有限生成的射影$A$模块，因此可以规范地识别分级的$A$模块$(E \otimes_A E)^{*gr}$和$E^{*gr} \otimes_A E^{*gr}$（II, § 4, no. 4，推论1到命题4）。如果$A$-模块$A \otimes_A A$和$A$也被规范地识别（II, § 3, no. 4），线性映射$E^{*gr} \otimes_A E^{*gr} \to E^{*gr}$，其中$E^{*gr}$中的定义乘法可以称为分级的转置余积$c$。

#### 命题 1 {#alg-iii-s11-prop-1 .statement tag=067N}

*令 $E$ 大于$A$ 余代数。在阶中，对于每个结合律 $A$-代数 $B$，$A$-代数 $\mathrm{Hom}_A(E, B)$ 都是结合律，余积 $c : E \to E \otimes_A E$ 满足图表* 是充分必要的

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
\downarrow c & & \downarrow l_E \otimes c \\
E \otimes_A E & \xrightarrow{c \otimes l_E} & E \otimes_A E \otimes_A E
\end{array}
$$

*可交换。*

令 $B$ 为 $A$ 代数和 $u, v, w$ $C = \mathrm{Hom}_A(E, B)$ 的三个元素。让$m_3$表示$A$-线性映射$B \otimes_A B \otimes_A B \to B$，其中映射$b \otimes b' \otimes b''$到$bb'b''$。通过代数 $C$ 上的乘积定义，$(uv)w$ 是合成映射

$$
E \xrightarrow{c} E \otimes E \xrightarrow{c \otimes 1_E} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B
$$

而$u(vw)$是复合映射

$$
E \xrightarrow{c} E \otimes E \xrightarrow{l_E \otimes c} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B.
$$

由此可知，如果图表 (12) 是可交换的，则对于每个结合律 $A$-代数 $B$，代数 $\mathrm{Hom}_A(E, B)$ 都是结合律。 为了建立逆命题，只需证明存在一个关联的 $A$-代数 $B$ 和 $E$ 到 $B$ 的三个$A$-线性映射 $u, v, w$，使得 $E \otimes E \otimes E$ 的映射 $m_3 \circ (u \otimes v \otimes w)$ 到$B$ 是单射的。 将$B$作为$A$-代数$\mathscr{T}(E)$并将$E$的$u, v, w$典范映射代入$\mathscr{T}(E)$。 映射 $m_3 \circ (u \otimes v \otimes w)$ 那么典范映射 $E \otimes E \otimes E = \mathscr{T}^3(E) \to \mathscr{T}(E)$，它是单射的。

当余代数$E$满足条件或命题1时，称为共结合。

#### 例 {#alg-iii-s11-n2-exa-2 .statement tag=067O}

(4)立即验证余代数$A$(no. 1,例(1))余代数$A^{(X)}$(no. 1,例4)和余代数$\mathscr{T}(M)$(no. 1, 例 5) 是共联想的。如果 $B$ 是结合性 $A$-代数，它是有限生成的射影 $A$-模，则余代数 $B^*$ (no. 1, 例 3) 是共结合的：对于交换律 of 图表 (12) 则如下通过从图表转置，表达$B$（§ 1, no. 3）的结合性。相反，相同的论证以及 A-模 B 与其双元（II, § 2, no. 7，推论 4 到命题 13）的规范标识表明，如果余代数 B* 是共结合的，则代数 B 是结合的。最后，余代数 S(M) 和 $\Lambda(M)$ (no. 1、例 6 和 7) 是共结合的；这是从交换律到图表得出的

$$
\begin{array}{ccc}
M & \xrightarrow{\Delta} & M \times M \\
\downarrow & & \downarrow 1_M \times \Delta \\
M \times M & \xrightarrow{\Delta \times 1_M} & M \times M \times M
\end{array}
$$

S(M) (§ 6, no. 2) 和 $\Lambda(M)$ (§ 7, no. 2) 的函子性质，给出相应的可交换图表

$$
\left\{
\begin{array}{ccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \times M) \\
\downarrow S(\Delta) & & \downarrow S(\Delta_M \times 1) \\
S(M \times M) & \xrightarrow{S(\Delta \times 1_M)} & S(M \times M \times M)
\end{array}
\right.
$$
$$
\left\{
\begin{array}{ccc}
\Lambda(M) & \xrightarrow{\Lambda(\Delta)} & \Lambda(M \times M) \\
\downarrow \Lambda(\Delta) & & \downarrow \Lambda(1_M \times \Delta) \\
\Lambda(M \times M) & \xrightarrow{\Lambda(\Delta \times 1_M)} & \Lambda(M \times M \times M)
\end{array}
\right.
$$

以及典范同构对于直和（§ 6, no. 6和§ 7, no. 7）的对称和外部代数的存在性和函子性。

#### 命题 2 {#alg-iii-s11-prop-2 .statement tag=067P}

*设 E 大于 A 余代数。在阶中，对于每个可交换的 A-代数 B，A-代数 $\mathrm{Hom}_A(E, B)$ 是可交换的，余积 $c : E \to E \otimes_A E$ 满足图表* 是充分必要的

$$
\begin{array}{ccc}
E & & \\
 & \swarrow_c & \searrow_c \\
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E
\end{array}
$$

（其中$\sigma$是对称性同态，使得$\sigma(x \otimes y) = y \otimes x$）是*可交换的*（在其他字中，余代数E与其相反*相同*（no. 1，例2）就足够了。

设B是$C = \mathrm{Hom}_A(E, B)$的可交换A-代数和$u, v$两个元素。

由C中乘积的定义，$uv$和$vu$分别等于合数映射

$$
E \xrightarrow{c} E \otimes E \xrightarrow{u \otimes v} B \otimes B \xrightarrow{m} B
$$

和

$$
E \xrightarrow{c} E \otimes E \xrightarrow{v \otimes u} B \otimes B \xrightarrow{m} B.
$$

由此可见，如果图表 (15) 是可交换的代数 $\mathrm{Hom}_A(E, B)$ 对于每个可交换的 A-代数 B 都是可交换的。要建立逆命题，只需证明存在一个可交换的 A-代数 B 和两个 E 的 A-线性映射 $u, v$ 到B 使得 $m \circ (u \otimes v): E \otimes E \to B$ 是单射的。取 B 为 E 的典范映射 $E \oplus E \to S(E \oplus E)$ 和映射 $x \mapsto (x, 0)$（分别为 $x \mapsto (0, x)$）的代数 $S(E \oplus E)$ 和 $u$（分别为 $v$）合成代入 $E \oplus E$。如果$h: S(E) \otimes S(E) \to S(E \otimes E)$是典范同构（§ 6, no. 6，命题9）并且$\lambda: E \to S(E)$是典范映射，则$h^{-1} \circ m \circ (u \otimes v) = \lambda \otimes \lambda$。现在$\lambda \otimes \lambda$是单射的，因为$\lambda(E)$是$S(E)$的直因子（II, § 3, no. 7，推论5到命题7）。

当余代数 E 满足条件或命题 2 时，称其为共交换的。

#### 例 {#alg-iii-s11-n2-exa-3 .statement tag=067Q}

(5) It is immediate that the cogebra A (no. 1, Example 1) and the cogebra $A^{(X)}$ (II, § 11, no. 1, Example 4) are cocommutative. 由no. 1的公式(5)可知余代数$S(M)$是互交换的。 最后，对于 A-代数 B 使得 A-模 B 是射影的，且有限生成有性质，且余代数 $B^*$ (no. 1, 例 3) 是可交换的，则 B 是可交换的充分必要；对于（使用 A-模 B 及其双数 (II, § 2, no. 7) 的规范标识），这是因为图表 (14) 的交换律通过转置等价于表示 B (§ 1, no. 3) 的交换律的图表。

#### 命题 3 {#alg-iii-s11-prop-3 .statement tag=067R}

*设 E 在 A 上余代数。在阶中，对于每个单位A-代数 B，A-代数 $\mathrm{Hom}_A(E, B)$ 是单位，在 E 上存在线性形式 $\gamma$ 是充分必要的，呈现可交换的图表*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow \gamma \otimes 1_E \\
& & A \otimes_A E
\end{array}
$$
$h'$

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow 1_E \otimes \gamma \\
& & E \otimes_A A
\end{array}
$$
$h''$

其中$c: E \to E \otimes_A E$是余积和$h'$和$h''$典范同构

（II, § 3, no. 4，命题4）。 *Hom$_A$(E, B) 的 *单位 *则为线性映射* x $\mapsto$ $\gamma(x)1$（其中 1 表示 B 的单位元）。

令 $\gamma$ 为线性形式，在 E 渲染图表 (16) 上可交换。设 B 是 A-代数 C = Hom$_A$(E, B) 的单位 A-代数，其中单位元 1、$\eta:A \to B$ 典范映射和 $v = \eta \circ \gamma$ 元素。对于每个元素 $u \in C$，$uv$ 是复合映射

$$
\text{(17)} \quad E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes \gamma} E \otimes A \xrightarrow{u \otimes \eta} B \otimes B \xrightarrow{m} B.
$$

然后$uv = m \circ (u \otimes \eta) \circ h'' = u$。类似地证明$vu = u$，因此$v$是C的单位元。相反，让A-模A$\oplus$E被赋予单位代数结构，使得$(a, x)(a', x') = (aa', ax' + a'x)$对于A中的$a, a'$和E中的$x, x'$。令B 表示由此定义的A-代数，并令 C 为A-代数 Hom$_A$(E, B)。假设 C 是单位的，并令 $e:x \mapsto (\gamma(x), \lambda(x))$ 为其单位元（其中 $\gamma(x) \in A$ 和 $\lambda(x) \in E$）。另一方面，令$f$为C的元素$x \mapsto (0, x)$。直接的计算表明$fe$为元素

$$
x \mapsto (0, (h'')^{-1}((1_E \otimes \gamma)(c(x))))
$$

C. 条件 $fe = f$ 蕴含 (16) 的第二个图表的交换律，同样可以看出，条件 $ef = f$ 蕴涵 (16) 的第一个图表的交换律。

线性形式$\gamma$在E渲染图表(16)上交换称为余代数E的*余单位*。余代数承认*至多一个*余单位：因为它是代数Hom$_A$(E，A)的单位元。 余代数与余单位称为 *counital*。

#### 例 {#alg-iii-s11-n2-exa-4 .statement tag=067S}

(6) 恒等映射是余代数A中的余单位；在余代数 A$^{(X)}$ (no. 1, *例 4*) 线性形式 $\gamma$ 上，使得所有 $x \in X$ 的 $\gamma(e_x) = 1$ 为余单位。在余代数 T(M)（分别为S(M)、$\Lambda(M)$）线性形式$\gamma$，使得$\gamma(1) = 1$和$\gamma(z) = 0$对于$z$在$T^n(M)$（分别为$S^n(M)$、$\Lambda^n(M)$） $n \geq 1$ 是余单位。最后，令 B 为 A-代数，它是有限生成的射影 A-模并且具有单位元 $e$；那么余代数 B* (no. 1, *例 3*) 线性形式 $\gamma: x^* \mapsto \langle e, x^* \rangle$ 是余单位，因为这个形式只是 A 的 A-线性映射 $\eta_e: \xi \mapsto \xi e$ 的转置到 B 并通过转置图表 (16) 的交换律源自图表，它表达（使用$\eta_e$）$e$是B (§ 1, no. 3)的单位元；同样的论点还表明，相反，如果余代数 B* 承认 B 的余单位 $\gamma$，则$\gamma$ 定义单位元 $e = t_\gamma(1)$ 的转置。

#### 命题 4 {#alg-iii-s11-prop-4 .statement tag=067T}

*设E为余代数，承认余单位$\gamma$，并假设E中存在元素 e，使得$\gamma(e) = 1$；那么 E 是子 A 模块 Ae 的直和和 $E_{\gamma} = \mathrm{Ker}(\gamma)$ 并且*

$$
\text{(18)} \quad \begin{cases}
c(e) \equiv e \otimes e \pmod{E_{\gamma} \otimes E_{\gamma}} \\
c(x) \equiv x \otimes e + e \otimes x \pmod{E_{\gamma} \otimes E_{\gamma}} & \text{for all } x \in E_{\gamma}.
\end{cases}
$$

第一个断言是直接的，因为$\gamma(x - \gamma(x)e) = 0$和关系$\gamma(\alpha e) = 0$意味着$\alpha = 0$。设$c(e) = \sum_i s_i \otimes t_i$，这样
$$
e = \sum_i \gamma(s_i)t_i = \sum_i \gamma(t_i)s_i
$$
由 (16) 和$1 = \gamma(e) = \sum_i \gamma(s_i)\gamma(t_i)$。因此
$$
\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e) = \sum_i s_i \otimes t_i - \sum_i e \otimes \gamma(s_i)t_i \\
- \sum_i \gamma(t_i)s_i \otimes e \\
+ \sum_i \gamma(s_i)e \otimes \gamma(t_i)e
$$
根据上面的关系，就是$c(e) - e \otimes e$；因此这证明了(18)的第一个关系。另一方面，$E \otimes E$的分解为直和
$$
A(e \otimes e) \oplus ((Ae) \otimes E_\gamma) \oplus (E_\gamma \otimes (Ae)) \oplus (E_\gamma \otimes E_\gamma)
$$
允许我们写，对于$x \in E_\gamma$，$c(x) = \lambda(e \otimes e) + (e \otimes y) + z \otimes e) + u$，其中$u = \sum_j v_j \otimes w_j, y, z$以及$v_j$和$w_j$属于到$E_\gamma$。 余单位 $\gamma$的定义则给出$x = \lambda e + y = \lambda e + z$，并且作为$\gamma(x) = 0$，必然为$\lambda = 0, x = y = z$，从而 (18) 的第二个关系。

#### 注 {#alg-iii-s11-n2-rem-2 .statement tag=067U}

设 C 为单位共联想 A 余代数，B 为单位联想 A-代数，M 左B-模。 $B \times M$ 到 M 定义的 A 双线性映射 $(b, m) \mapsto bm$ A 双线性映射
$$
\operatorname{Hom}_A(C, B) \times \operatorname{Hom}_A(C, M) \to \operatorname{Hom}_A(C, M)
$$
通过本号开头描述的一般程序。立即验证，这个映射定义在$\operatorname{Hom}_A(C, M)$左模结构超过环$\operatorname{Hom}_A(C, B)$。

### 3. 余代数型 N 分级的特性

#### 命题 5 {#alg-iii-s11-prop-5 .statement tag=067V}

(i) *令 E 为余代数承认余单位 $\gamma$；那么 $\gamma$ 是次数 0 的齐次线性形式。*

(ii) *进一步假设存在元素$e \in E$使得$E_0 = Ae$和$\gamma(e) = 1$。那么$\gamma$的核$E_\gamma$等于$E_+ = \sum_{n \geq 1} E_n$、$c(e) = e \otimes e$并且*
$$
c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_+ \otimes E_+)
$$
*对于所有人*$x \in E_+$。

(i) 足以验证$\gamma(x) = 0$对于$x \in E_n$，对于所有$n \geq 1$。由于 $c$ 的评分为同态次数 0，

$$
c(x) = \sum_{0 \leq j \leq n} \left( \sum_i y_{ij} \otimes z_{i, n-j} \right)
$$

对于所有$j$，使得$E_j$中有$0 \leq j \leq n$、$y_{ij}$和$z_{ij}$； 应用 (16) (no. 2) 我们得到

$$
x = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(y_{ij}) z_{i, n-j} \right) = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(z_{i, n-j}) y_{ij} \right),
$$

从而，将次数 0 和次数 $n$ 两侧的分量相等

$$
x = \sum_i \gamma(y_{i0}) z_{in} = \sum_i \gamma(z_{i0}) y_{in}
$$
$$
0 = \sum_i \gamma(y_{in}) z_{i0} = \sum_i \gamma(z_{in}) y_{i0}
$$

因此$\gamma(x) = \sum_i \gamma(y_{in}) \gamma(z_{i0}) = \gamma(0) = 0$。

(ii) 由于$\mathrm{Ker}(\gamma)$和$E_+$都是$Ae = E_0$和$E_+ \subset \mathrm{Ker}(\gamma)$的补充子A模块（i），$E_+ = \mathrm{Ker}(\gamma)$（II, § 1, no. 8，注1）；另一个断言紧随命题 4 of no. 2。

#### 命题 6 {#alg-iii-s11-prop-6 .statement tag=067W}

*令 E 为 A 上的分级余代数。在阶中，对于每个可交换的 A-代数 B，通过平凡的毕业，型 $\mathbf{Z} \mathrm{Homgr}_A(E, B)$ (no. 2) 的分级 A-代数是反交换的 (§ 4, no. 9， 定义 7)，如果 $\sigma_g$ 表示 A-模 $E \otimes_A E$ 中的自同构，则满足*

$$
\sigma_g(x_p \otimes x_q) = (-1)^{pq} x_q \otimes x_p
$$

对于 $x_p \in E_p, x_q \in E_q$，*其中 p 和 q 是 $\mathbf{N}$、图表中的任意元素*

$$
\begin{array}{ccc}
E & & \\
 & \searrow^c & \swarrow^c \\
E \otimes_A E & \xrightarrow{\sigma_g} & E \otimes_A E
\end{array}
$$

*可交换。*

证明类似于 no. 2 的命题 2。

当分级余代数 E 满足条件或命题 6 时，称为*反交换*。

#### 例 {#alg-iii-s11-n3-exa-1 .statement tag=067X}

紧随no. 1的公式 (8)，对于每A-模 M，分级的余代数$\bigwedge(M)$是*反交换的*。

### 4. BIGEBRAS 和 SKE-BIGEBRAS

#### 定义 3 {#alg-iii-s11-def-3 .statement tag=067Y}

*环 A 上的分级 Bigebra（或倾斜分级 Bigebra）为集合 E，分级 A-代数结构为型 $\mathbf{N}$，分级 A-cogebra 结构为型 $\mathbf{N}$，具有相同的标的评级 A-模结构，这样：*

(1) *A-代数 E 是结合律且单位的。*

(2) *A-代数 E 是共联想和共体的。*
(3) *余积 c : E \to E \otimes_A E 是分级代数 E 的同态到分级代数 E \otimes_A E* （或 *分级代数 E^g \otimes_A E* (cf. § 4, no. 7））。
(4) *E 的余单位 $\gamma$ 是代数 E 分级为代数 A 的同态（具有普通分级），因此，如果 e 表示 A-代数 E 的单位元，则$\gamma(e) = 1$。*

如果 E 是一个分级的 bigebra，其分级是*琐碎的*，则 E 被简单地称为*bigebra*。如果底层代数是可交换的（或者如果底层余代数是可交换的），则分级大数称为可交换的（或可共交换的）；如果底层分级代数是反交换的（或者如果底层分级余代数是反交换的），则倾斜分级的 bigebra 被称为反交换的（或者反交换的）。

从定义 3 和 no. 2、命题 5 可以得出，对于分级 bigebra 或倾斜分级 bigebra E，

$$
c(e) = e \otimes e \\
c(x) \equiv x \otimes e + e \otimes x (\text{mod. } E_+ \otimes E_+) \quad \text{for } x \in E_+ = \bigoplus_{n \geq 1} E_n.
$$

如果 E 和 F 是两个分级 bigebra（分别是两个倾斜分级 bigebra），则映射 $\phi : E \to F$ 被称为 *分级 bigebra 态射*（分别是 *倾斜分级 bigebra 态射*），如果： (1) $\phi$ 是分级代数态射（因此E的映射单位元到F的单位元）； (2) $\phi$ 是分级的余代数态射，因此，如果 $\gamma$ 和 $\gamma'$ 分别是 E 和 F 的余单位，则$\gamma = \gamma' \circ \phi$。

#### 例 {#alg-iii-s11-n4-exa-1 .statement tag=067Z}

(1) 令 S 为具有单位元素 u 的幺半群，使得 A 上的幺半群 S 的代数 $E = A^{(S)}$ 承认单位元 $e_u$ (§ 2, no. 6)；另一方面，E 具有典型的共关联共交换 A-代数结构，其中余单位 $\gamma$ 使得 $\gamma(e_s) = 1$ 对于所有 $s \in S$ (no. 1、例 4 和 no. 2、例 4， 5 和 6)。 公式$c(e_s) = e_s \otimes e_s$给出余积也立即表明c是代数同态。因此，在 E 和 E 上定义了*共交换大数* 结构，其中结构被称为幺半群 S 在 A* 上的*大数数。

如果 T 是另一个幺半群，其中单位元 v、$f : S \to T$ 同态，使得 $f(u) = v$ 和 $f_{(A)} : A^{(S)} \to A^{(T)}$ A-代数同态源自 $f$ (§ 2, no. 6)，则立即验证$f_{(A)}$ 是一个 *bigebra 同态*。

(2) 设M为A-模。在 S(M) 定义上定义的分级 A-代数 (§ 6, no. 1) 和分级 A-cogebra (no. 1, 例 6) 结构在此集合上定义*可交换共交换分级大数* 结构；因为我们已经看到 (no. 1, 例 6) S(M) 上的余积是 *代数* 同态并且它是从余单位 $\gamma$ 的定义得出的 (no. 2, 例 6) $\gamma(1) = 1$ 和 $\gamma$ 是 E 到 A 的代数同态。

(3) 设M为A-模。我们在例 2 中看到，$\bigwedge(M)$ 定义上的分级 A-代数 (§ 7, no. 1) 和分级 A-余数 (no. 1, 例 7) 结构在这个集合上*反交换反交换偏斜分级bigebra* 结构。

#### 注 {#alg-iii-s11-n4-rem-1 .statement tag=0680}

如果 M 为 A-模，使得 $M \otimes_A M \neq \{0\}$，则 $T(M)$ 上的分级 A-代数 (§ 5, no. 1) 和分级 A-余数 (no. 1, 例 5) 结构 *不要定义* 大数数结构，一般来说

$$
c(x_1 x_2 y_1 y_2) \neq c(x_1 x_2) c(y_1 y_2)
$$

对于M的四个元素$x_1, x_2, y_1, y_2$，如no. 1的公式(3)所示。

### 5. 分级双打$T(M)^{*gr}$、$S(M)^{*gr}$ 和 $\bigwedge(M)^{*gr}$

*从现在开始，我们返回章对代数的一般约定，因此将假定（除非否则提及）是结合和单位的。*

设M为A-模； $T(M)$ (no. 1, 例 5), $S(M)$ (no. 1, 例 6) 和$\bigwedge(M)$ (no. 1, 例 7) 上定义的分级A-代数结构允许我们定义规范地对分级对偶 $T(M)^{*gr}$、$S(M)^{*gr}$ 和 $\bigwedge(M)^{*gr}$ *分级代数* 结构为型 N，凭借 no. 2、命题 1 和 3 以及制定的约定模 (no. 1) 的分级双学位毕业。此外，分级的代数$S(M)^{*gr}$是*可交换的*（no. 2，命题2和例5），而分级的代数$\bigwedge(M)^{*gr}$是*反交换的*（no. 3，命题） 6 和例）。在 $\bigwedge(M)^{*gr}$ *次数 1 中的每个元素都是零平方*；这样元素在M上与线性形式$f$识别，并且它的平方在$M^2$上是交错的双线性形式$f \wedge f$这样

$$
(f \wedge f)(x, y) = f(x) f(y) - f(y) f(x)
$$

（no. 2，例3）。

令 N 为 M 到 N 的另一个 A-模和 $u$ A-线性映射。我们知道 $u$ 定义规范分级代数同态

$$
\begin{cases}
T(u): T(M) \to T(N) \\
S(u): S(M) \to S(N) \\
\bigwedge(u): \bigwedge(M) \to \bigwedge(N)
\end{cases}
$$

（§ 5, no. 2、§ 6, no. 2 和 § 7, no. 2）。立即在no. 1的公式(3)中验证$T(u)$也是*余代数态射*。另一方面，如果$\Delta_M$（或$\Delta_N$）表示对角线映射$M \to M \times M$（或$N \to N \times N$），则有关系$(u \times u) \circ \Delta_M = \Delta_N \circ u$；由此可见 $S(u \times u) \circ S(\Delta_M) = S(\Delta_N) \circ S(u)$

（分别$\Lambda(u \times u) \circ \Lambda(\Delta_M) = \Lambda(\Delta_N) \circ \Lambda(u)$）。

在$S(M)$和$\Lambda(M)$（no. 1、例 6和7）中使用余积的定义以及典范同构的函子特征标

$$
S(M \times M) \to S(M) \otimes_A S(M)
$$

和$\Lambda(M \times M) \to \Lambda(M)^{\text{g}} \otimes_A \Lambda(M)$，可以看出$S(u)$和$\Lambda(u)$也是*余代数态射*†（因此在这种情况下是*bigebra*态射）。紧接着，同态 (23) 的*分级转置* (II, § 11, no. 6)

$$
\begin{align*}
tT(u): T(N)^{*gr} &\to T(M)^{*gr} \\
tS(u): S(N)^{*gr} &\to S(M)^{*gr} \\
t\Lambda(u): \Lambda(N)^{*gr} &\to \Lambda(M)^{*gr}
\end{align*}
$$

*评分代数同态*。

我们现在注，$M$的对偶$M^*$被识别为$T(M)^{*gr}$中次数1的元素的子模（分别为$S(M)^{*gr}$，$\Lambda(M)^{*gr}$）。因此，从张量代数 (§ 5, no. 1) 的泛性质和对称代数 (§ 6, no. 1) 的泛性质可以得出，*存在且仅有一个分级的代数同态*

$$
\theta_T: T(M^*) \to T(M)^{*gr}
$$

*其中扩展典范嵌入* $M^* \to T(M)^{*gr}$，*只有一个评级为代数同态*

$$
\theta_S: S(M^*) \to S(M)^{*gr}
$$

*其中扩展典范嵌入*$M^* \to S(M)^{*gr}$。另一方面，代数到$\Lambda(M)^{*gr}$*相反*的$M^*$的典范嵌入使得$M^*$的每个元素的平方是零；因此 (§ 7, no. 1, 命题 1) *存在且仅有一个分级代数同态*

$$
\theta_\Lambda: \Lambda(M^*) \to (\Lambda(M)^{*gr})^0
$$

*其中扩展典范嵌入*$M^* \to \Lambda(M)^{*gr}$.‡这些同态

† 这也是从 no. 1 的公式 (5) 和 (9) 得出的。
‡ 为了计算方便，将单射扩展到同态到反代数到$\Lambda(M)^{*gr}$，而不是同态到$\Lambda(M)^{*gr}$。

是函数式的：对于例，对于每个$A$-模块同态$u : M \to N$，图表

$$
\begin{array}{ccc}
T(N^*) & \xrightarrow{T(tu)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(N)^{*gr} & \xrightarrow{t_{T(n)}} & T(M)^{*gr}
\end{array}
$$

是可交换的，从泛性质 of 张量代数 (§ 5, no. 1) 立即如下； $\theta_S$ 和 $\theta_\wedge$ 有类似的交换律图表。

我们将显式地找到同态 $\theta_T, \theta_S$ 和 $\theta_\wedge$。为此，我们更一般地考虑$A$-cogebra $E$与余积$c$和定义通过$n$上的归纳，对于$n \geq 2$，线性映射$c_n$的$E$由 $c_2 = c$ 变为 $E^{\otimes n}$ 并且
$$
c_n = (c_{n-1} \otimes 1_E) \circ c.
$$
另一方面，我们用 $m_n : A^{\otimes n} \to A$ 表示规范的线性映射，使得 $m_n(\xi_1 \otimes \xi_2 \otimes \cdots \otimes \xi_n) = \xi_1 \xi_2 \cdots \xi_n$ 和注，对于 $n \geq 2$，
$$
m_n = m \circ (m_{n-1} \otimes 1_A)
$$
写$m = m_2$。有了这个记号：

#### 引理 1 {#alg-iii-s11-lem-1 .statement tag=0681}

(i) *在结合律代数 $E^* = \mathrm{Hom}_A(E, A)$ 中，次数 1 的 $n$ 元素 $u_1, u_2, \ldots, u_n$ 的乘积由下式给出*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n.
$$
(ii) *还假设余代数 $E$ 已评分。然后，在分级联想代数$E^{*gr} = \mathrm{Homgr}_A(E, A)$中，次数1的$n$元素$u_1, u_2, \ldots, u_n$的乘积由*给出
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ \delta_n
$$
*其中$\delta_n : E \to E^{\otimes n}$是线性映射，其中映射每个$x \in E$到多次$(1, 1, \ldots, 1)$的$c_n(x)$的分量。*

公式 (26) 只是$E^*$ 中乘积的定义对于$n = 2$；为了通过 $n$ 上的归纳证明这一点，请观察
$$
u_1 u_2 \ldots u_n
$$
$$
= m \circ ((u_1 u_2 \ldots u_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ ((m_{n-1} \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1}) \circ c_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ (m_{n-1} \otimes 1_A) \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1} \otimes u_n) \circ (c_{n-1} \otimes 1_E) \circ c
$$
$$
= m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n
$$
凭借 (24), (25), II, § 3, no. 3, 公式 (5) 和关系
$$
u_n = 1_A \circ u_n \circ 1_{E^*}.
$$

当 E 分级且元素 $u_i \in E^{*gr}$ 次数 1 均质时，则通过定义得到*均质* 元素 $x_i \in E$，

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_n)(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0
$$

除非所有 $x_i$ 都是次数 1, 从而公式 (27)。

由no. 1和公式(24)的公式(3)、(5)和(7)可知，当E取三个等级余代数$\mathbf{T}(M)$、$\mathbf{S}(M)$和$\mathbf{\Lambda}(M)$之一时，我们分别由归纳得到$n$（使用余积是次数 0的分级同态这一事实），对于M中的$x_1, x_2, \ldots, x_n$：

当$E = \mathbf{T}(M)$时，
$$
\delta_n(x_1 x_2 \cdots x_n) = x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$

当$E = \mathbf{S}(M)$时，
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$

当$E = \mathbf{\Lambda}(M)$时，
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma \cdot x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}.
$$

当$E = \mathbf{\Lambda}(M)$时，对于例，满足注，即表达式中
$$
c_n(x_1 x_2 \cdots x_n) = (c_{n-1} \otimes 1_E) \left( \sum (-1)^v (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}}) \right)
$$
由 no. 1 的公式 (8) 产生，唯一可以给出多次 $(1, 1, \ldots, 1)$ 的项的项是$n - p = 1$ 的那些，因此
$$
\delta_n(x_1 x_2 \cdots x_n)
$$
是和中多次 $(1, 1, \ldots, 1)$ 的项
$$
\sum_{i=1}^n (-1)^{n-i} c_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i
$$
而这个项必然等于
$$
\sum_{i=1}^n (-1)^{n-i} \delta_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i,
$$
从而归纳假设的结果。

在 $n$ 线性形式 $x_1^*, x_2^*, \ldots, x_n^*$ $M^*$ 的 $\mathbf{T}(M)^{*gr}$ 中使用引理 1、乘积由下式给出

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
对于 $x_i \in M$ ($1 \leq i \leq n$)； $\mathbf{S}(M)^{*gr}$中的$n$形式中的乘积由下式给出

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right);
$$

最后，$\bigwedge(M)^{*gr}$中的形式中的乘积由下式给出
$$
\langle x_1^* x_1^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \det(\langle x_i^*, x_j \rangle).
$$
对于这三种情况，我们分别有
$$
\theta_T(x_1^* \otimes x_2^* \otimes \ldots \otimes x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_S(x_1^* x_2^* \ldots x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) = x_n^* x_{n-1}^* \ldots x_1^* = (-1)^{n(n-1)/2} x_1^* x_2^* \ldots x_n^*
$$
因此我们从 (28), (29) 和 (30) 关系推出
$$(28\ \mathrm{bis})\quad \langle \theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*), x_1 \otimes x_2 \otimes \cdots \otimes x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle$$
（其他字$\theta_T$仅限于$T^2(M^*)$只是II, § 4, no. 4的典范同态）
$$(29\ \mathrm{bis})\quad \langle \theta_S(x_1^* x_2^* \ldots x_n^*), x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right)$$
$$(30\ \mathrm{bis})\quad \langle \theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*), x_1 \wedge x_2 \wedge \cdots \wedge x_n \rangle$$
$$
= (-1)^{n(n-1)/2} \det(\langle x_i^*, x_j \rangle).
$$

#### 命题 7 {#alg-iii-s11-prop-7 .statement tag=0682}

*设 M 为有限生成的射影 A-模。那么典范同态 $\theta_T : T(M^*) \to T(M)^{*gr}$ 和 $\theta_\Lambda : \bigwedge(M^*) \to (\bigwedge(M)^{*gr})^0$ 是双射的。此外，分级对偶 $\bigwedge(M)^{*gr}$ 等于 A-模 $\bigwedge(M)$ 的对偶 $\bigwedge(M)^*$。*

首先假设 M 有一个*有限基* $(e_i)_{1 \leq i \leq m}$，并令 $(e_i^*)_{1 \leq i \leq m}$ 为 $M^*$ (II, § 10, no. 4) 的对偶基。 公式 (28 bis) 表明，对于 $\mathbf{N}$ 区间 $[1, m]$ 的 n 元素中的每一个有限序列 $s = (j_k)_{1 \leq k \leq n}$，
$$
\theta_T(e_{j_1}^* \otimes \cdots \otimes e_{j_n}^*)
$$
是$(T^n(M))^*$的基中的指标元素，*对偶*到$e_s = e_{j_1} \otimes \cdots \otimes e_{j_n}$的$T^n(M)$由……组成的基（§ 5, no. 5，定理1）。因此 $\theta_T$ 是双射的。

类似地，公式（30之二）表明，对于$[1, m]$的每个有限子集 H，其中n为元素，$(-1)^{n(n-1)/2} \theta_\Lambda(e_H^*)$（§ 7, no. 8的记号，定理 1）是指标 H的元素 $(\bigwedge^n(M))^*$ 的基，*对偶的*到$\bigwedge^n(M)$ 由……组成的基 $e_H$。因此 $\theta_\Lambda$ 是双射的。

现在仅假设 M 是有限生成且射影的；则 M 是有限生成的自由A-模 L 的直因子，因此存在两个

A-线性映射$M \xrightarrow{j} L \xrightarrow{p} M$，其中合成是恒等式$l_M$。我们推导出交换律图表

$$
\begin{array}{ccc}
T(M^*) & \xrightarrow{T(tj)} & T(L^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(M)^{*gr} & \xrightarrow{tT(j)} & T(L)^{*gr}
\end{array}
$$
$$
\begin{array}{ccc}
T(L^*) & \xrightarrow{T(tp)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(L)^{*gr} & \xrightarrow{tT(p)} & T(M)^{*gr}
\end{array}
$$

以及类似的交换律图表，其中 $T$ 被 $\Lambda$ 替代。然后从以下引理得出命题：

#### 引理 2 {#alg-iii-s11-lem-2 .statement tag=0683}

*让*

$$
\begin{array}{ccccc}
X & \xrightarrow{u} & Y & \xrightarrow{v} & X \\
f \downarrow & & g \downarrow & & f \downarrow \\
X' & \xrightarrow{u'} & Y' & \xrightarrow{v'} & X'
\end{array}
$$

*是集合和映射的可交换图表，使得$v \circ u$和$v' \circ u'$分别是$X$和$X'$的恒等映射。那么，如果 $g$ 是单射（或满射、或双射），则 $f$ 也是。*

$u$ 是单射，因为 $v \circ u$ 是单射，因此，如果 $g$ 是单射，则 $u' \circ f = g \circ u$ 是单射，因此 $f$ 是单射。类似地，$v'$ 是满射，因为 $v' \circ u'$ 是；因此，如果 $g$ 是满射，则 $f \circ v = v' \circ g$ 是满射，因此 $f$ 是满射。

命题 7 的最后一个断言源自$\Lambda(M)$则为有限生成A-模（§ 7, no. 3、命题 6 和II, § 11, no. 6、注）。

现在，我们研究当 $M$ 是*射影且有限生成*时，关于同态 $\theta_S$ 可以说些什么。首先假设$M$承认有限的基$(e_i)_{1 \leq i \leq m}$。在记号中，章A-模$S^n(M)$的开头承认元素$e^\alpha$的家庭为基，使得$|\alpha| = n$。让$u_\alpha$（对于$|\alpha| = n$）表示指标$\alpha$中的元素在$(S^n(M))^*$的基*对偶*到$(e^\alpha)$。 元素$u_\alpha$，对于$\alpha \in \mathbf{N}^m$，因此代数$S(M)^{*gr}$的形式基，我们将明确获得这个基的乘法表。我们写

$$
u_\alpha u_\beta = \sum_{\gamma \in \mathbf{N}^m} a_{\alpha \beta \gamma} u_\gamma \quad \text{with } a_{\alpha \beta \gamma} \in A.
$$

然后定义

$$
a_{\alpha \beta \gamma} = \langle u_\alpha u_\beta, e^\gamma \rangle = m((u_\alpha \otimes u_\beta)(c(e^\gamma))),
$$

其中$A$和$c$上的$m : A \otimes A \to A$定义乘法是$S(M)$的余积。在其他字中，$a_{\alpha \beta \gamma}$就是将$c(e^\gamma)$写成$e^\xi \otimes e^\eta$的$S(M) \otimes S(M)$由……组成基项时$e^\alpha \otimes e^\beta$的系数，其中$\xi$和$\eta$贯穿$\mathbf{N}^m$。但由于$c$是代数同态，

$$
c(e^\gamma) = \prod_{i=1}^m (c(e_i))^{r_i} = \prod_{i=1}^m (e_i \otimes 1 + 1 \otimes e_i)^{r_i}
$$

由公式 (4) 共 no. 1；这给出了

(31)
$$
c(e^\gamma) = \sum_{\xi + \eta = \gamma} (\xi, \eta) e^\xi \otimes e^\eta
$$
我们写的地方

(32)
$$
((\xi, \eta)) = \prod_{i=1}^n \frac{(\xi_i + \eta_i)!}{\xi_i! \eta_i!} \quad \text{(cf. § 10, no. 4, formula (18))}.
$$
因此我们得到乘法表

(33)
$$
u_\alpha u_\beta = ((\alpha, \beta)) u_{\alpha + \beta}.
$$
另一方面，如果$(e_i^*)_{1 \leq i \leq m}$是$M^*$的基，对$(e_i)$，则从公式（29之二）得出，对于所有$\alpha \in \mathbf{N}^m$，

(34)
$$
\theta_S(e^{*\alpha}) = \alpha! u_\alpha
$$
在记号中，共 § 6, no. 6。因此，同态$\theta_S$是双射当且仅当$\alpha! u_\alpha$形式是$S(M)^{*gr}$的*基*，或者元素$\alpha! 1$是*可逆的*。

#### 命题 8 {#alg-iii-s11-prop-8 .statement tag=0684}

*假设环$A$是有理数数的代数大于域$\mathbf{Q}$；那么，对于每个有限生成的射影$A$-模$M$，同态*

$$
\theta_S : S(M^*) \to S(M)^{*gr}
$$
*是双射的。*

当 $M$ 有限生成并且自由时，它相当于证明；我们使用引理 2 从这种情况过渡到一般情况，如命题 7 的证明所示。

#### 注 {#alg-iii-s11-n5-rem-1 .statement tag=0685}

令$M$为$A$模块且$\rho : A \to B$交换环同态。那么有分级 $B$-代数同态的交换图表

$$
\begin{array}{ccc}
T((M^*)_{(B)}) & \longrightarrow & (T(M)^{*gr})_{(B)} \\
\downarrow_{T(u_M)} & & \downarrow^{u_{T(M)}} \\
T((M_{(B)})^*) & \xrightarrow{\theta_T} & T(M_{(B)})^{*gr}
\end{array}
$$

其中第一行是同态由同态 $\theta_T \otimes 1_B : T(M^*) \otimes_A B \to T(M)^{*gr}$ 和典范同构组成

$$
T((M^*)_{(B)}) \to T(M^*) \otimes_A B
$$

§ 5, no. 3、命题5)。使用公式 (28) 和同态 $v_E$ (II, § 5, no. 4) 的定义可以立即验证，这个图表是*可交换的*。当 M 是*有限生成射影* A-模时，$M_{(B)}$ 是有限生成射影 B-模（II, § 5, no. 1，命题 4 的推论），并且上述图表的所有同态都是*双射*（命题 7 和II, § 5, no. 4、命题 8)。还有类似的交换律图表，其中 T 替换为 S 或 $\Lambda$；当 M 是射影且有限生成时 (命题 7)，$\Lambda$ 的图表也由双射同态组成；如果进一步 A 是 $\mathbf{Q}$ 上的代数，则 S 的图表也由双射同态 (命题 8) 组成。

### 6.内部乘积：代数案例

设$E = \bigoplus_{p \geq 0} E_p$为型$\mathbf{N}$的*分级A-代数*，P为型$\mathbf{Z}$的A-模分级；对于每个 *同质* 元素 $x \in E_p$，x 的*左* 乘法是 E 的 A-线性映射 $e(x)$ 自身，其 * 分级为次数 p*。对于每个元素 $u \in \mathrm{Homgr}_A(E, P)$，u 与 x* 的*右内部乘积（用 $u \perp x$ 表示）是 $\mathrm{Homgr}_A(E, P)$ 的元素 $u \circ e(x)$。我们还写 $(i(x))(u) = u \perp x$，我们看到 $i(x)$ 是分级 A-模 $\mathrm{Homgr}_A(E, P)$ 的次数 p 的分级自同态。如果现在$x = \sum_{p \geq 0} x_p$是E的任意元素（$x_p \in E_p$代表所有$p \geq 0$，$x_p = 0$，除了$p$的值的有限数），我们写为$i(x) = \sum_{p=0}^\infty i(x_p)$，因此自同态 A-模 $\mathrm{Homgr}_A(E, P)$。

要记住表达式 $u \perp x$ 中的哪个元素对另一个“操作”，请观察对 u “操作”的元素 x 放置在 $\perp$ 中水平线的自由端。

对于$x, y$同质，代数E的*结合性*转到关系$e(xy) = e(x) \circ e(y)$； 从而，由 $i(x)$ 的定义，

$$
i(xy) = i(y) \circ i(x)
$$

首先对于 $x, y$ 齐次，然后通过线性，对于 E 中的*任意* $x, y$；这也可以写成

$$
(u \perp x) \perp y = u \perp (xy)
$$

对于 E 中的 $x, y$ 和 $u \in \mathrm{Homgr}_A(E, P)$；另一方面，显然$i(1)$是恒等映射（因为这是从$e(1) = 1_E$得出的）并且$x \mapsto i(x)$是*A-线性的*，可以看出合成$(x, u) \mapsto u \perp x$（$x \in E, u \in \mathrm{Homgr}_A(E, P)$）定义的外法则， 加法，$\mathrm{Homgr}_A(E, P)$ 上的*右 E 模块* 结构。

特别是，我们考虑情况 $P = A$，$\mathrm{Homgr}_A(E, P)$ 在这种情况下是 $E$ 的*分级对偶* $E^{*gr}$；那么$i(x)$是$A$线性映射$e(x)$（II, § 11, no. 6）的*分级转置*，在其他字中，对于$E$、$u \in E^{*gr}$中的所有$x, y$，

$$
\langle u \sqcup x, y \rangle = \langle u, xy \rangle.
$$

根据段落开头的约定，注，如果$x \in E_p$，则$i(x)$ 是$E^{*gr}$ *次数* $-p$ 的自同态。

对于每个齐次元素$x \in E_p$，$x$的*右*乘法类似地由$e'(x)$和$\mathrm{Homgr}_A(E, P)$的元素$u \circ e'(x)$表示，称为u的x*的*左内部乘积， $x \sqcup u$；我们写 $i'(x) = x \sqcup u$ 和 $i'(x)$ 因此是自同态 $\mathrm{Homgr}_A(E, P)$ 次数 $p$；如上所述，这个定义可以扩展到$x$是$E$的任意元素的情况。在这个例子中$e'(xy) = e'(y)e'(x)$，

$$
i'(xy) = i'(x) \circ i'(y)
$$

也可以写成

$$
x \sqcup (y \sqcup u) = (xy) \sqcup u
$$

并显示合成$(x, u) \mapsto x \sqcup u$定义的外法则，以及加法，$\mathrm{Homgr}_A(E, P)$上的*左E模块*结构。另一方面，$E$的结合性意味着$e(x) \circ e'(y) = e'(y) \circ e(x)$对于$x, y$齐次于$E$、从而关系

$$
(y \sqcup u) \sqcup x = y \sqcup (u \sqcup x)
$$

这样 $\mathrm{Homgr}_A(E, P)$ 定义上的合成的两个外法则在此集合上有 *(E, E)*-*双模* 结构 (II, § 1, no. 14)。

当我们取$P = A$时，$i'(x)$就是$e'(x)$的分级转置；在其他字中，对于 $E$、$u \in E^{*gr}$ 中的所有 $x, y$，

$$
\langle y, x \sqcup u \rangle = \langle yx, u \rangle.
$$

当分级的代数$E$是*可交换的*时，显然是$u \sqcup x = x \sqcup u$。当$E$是*反交换*且$P = A$时，则对于$x \in E_p$、$y \in E_r$和$u \in E_q^*$、$yx = (-1)^{pr} xy$、从而，由(37)和(41)得出$\langle u \sqcup x, y \rangle = (-1)^{pr} \langle y, x \sqcup u \rangle$。但由于这个关系的两边除$r = q - p$外都是零，

$$
x \sqcup u = (-1)^{p(q-p)} u \sqcup x.
$$

令 $F$ 为另一个分级的 $A$-代数，并且 $\phi : E \to F$ 为分级代数的 $A$ 同态；那么$\tilde{\phi} = \mathrm{Hom}(\phi, 1_P) : \mathrm{Homgr}_A(F, P) \to \mathrm{Homgr}_A(E, P)$是次数0的分级$A$同态；由定义，为$E$和$u \in \mathrm{Homgr}_A(F, P)$中的$x, y$

$$
\begin{align*}
(\tilde{\phi}(u \sqcup \phi(x)))(y) &= (u \sqcup \phi(x))(\phi(y)) \\
&= u(\phi(x)\phi(y)) = u(\phi(xy)) = (\tilde{\phi}(u))(xy) = (\tilde{\phi}(u) \sqcup x)(y)
\end{align*}
$$

或者也

$$
\tilde{\phi}(u \sqcup \phi(x)) = \tilde{\phi}(u) \sqcup x
$$

和类似地

$$
\tilde{\phi}(\phi(x) \sqcup u) = x \sqcup \tilde{\phi}(u).
$$

在其他字中，当 Homgr_A(F, P) 通过环同态 $\phi : E \to F$ 被视为 (E, E)-双模时，可以看出 $\tilde{\phi}$ 是 (E, E)-双模同态 （或者也是 (F, F)-双模的 E 同态Homgr_A(F, P) 转换为 (E, E)-双模 Homgr_A(E, P))。

#### 例 {#alg-iii-s11-n6-exa-1 .statement tag=0686}

特别地，当E是代数T(M)、S(M)或A-模M和P A-模的分级代数T(M)、S(M)或$\bigwedge(M)$之一时，可以应用以上内容（具有普通分级）。为了显式地找到由此获得的双模结构，Homgr_A(T(M), P)（分别为Homgr_A(S(M), P)、分别为Homgr_A($\bigwedge(M)$, P)）的次数 $-n$的注和元素用*n线性映射*（分别为。 *$M^n$ 到 P 的*对称 n 线性映射*，分别为 *交错的 n 线性映射*)。足以表达乘积

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$

（分别$f \sqcup (x_1 x_2 \ldots x_p)$），分别。 $f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p)$）对于M的元素的每个有限序列$(x_i)_{1 \leq i \leq p}$以及左侧内部乘积的类似物。从定义可以立即得出

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f = 0
$$

*if* $p > n$ and that, for $p \leq n$, $f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)$ (resp.

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)
$$

是 *(n - p)*-线性映射，定义为

$$
\begin{cases}
(f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p))(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(x_1, \ldots, x_p, y_1, \ldots, y_{n-p}) \\
((x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(y_1, \ldots, y_{n-p}, x_1, \ldots, x_p).
\end{cases}
$$

对于 $p > n$，Homgr_A(S(M), P)（分别为 Homgr_A($\bigwedge(M)$, P)）公式 (44) 中也有 $x_1 \otimes x_2 \otimes \cdots \otimes x_p$ 替换为 $x_1 x_2 \ldots x_p$（分别为 $x_1 \wedge x_2 \wedge \cdots \wedge x_p$）。对于 $p \leq n$，(45) 定义中的相同代换 *对称* *(n - p)*-线性映射 $f \sqcup (x_1 x_2 \ldots x_p)$ 和 $(x_1 x_2 \ldots x_p) \sqcup f$（分别为 *交错的* *(n - p)*-线性映射

$$
f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \quad \text{and} \quad (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \sqcup f).
$$

当$n = p$时，上述乘积等于$M$上的常数函数等于$f(x_1, \ldots, x_p)$。

如果 $u : M \to N$ 是$A$-模同态，$T(u) : T(M) \to T(N)$ 是分级 $A$-代数同态，那么根据我们上面所看到的，$(T(u))^\sim$ 是 $(T(N), T(N))$-双模 $\mathrm{Homgr}_A(T(N), P)$ 的 $T(M)$ 同态$(T(M), T(M))$-双模$\mathrm{Homgr}_A(T(M), P)$，相对于环同态$T(u)$。 $(S(u))^\sim$ 和 $(\wedge(u))^\sim$ 也有类似的结果。

### 7.内部乘积：余代数的情况

令 $E = \bigoplus_{p \geq 0} E_p$ 为分级为余代数的共联想单位。然后我们知道（no. 2，命题 1 和 3），分级双$E^{*\mathrm{gr}}$（根据段落开头制定的毕业惯例）分级代数结构为型$\mathbf{N}$超过$A$，乘积两个这个代数的元素$u, v$由$uv = m \circ (u \otimes v) \circ c$定义，其中$c : E \to E \otimes_A E$是余积和$m : A \otimes_A A \to A$定义乘法。在其他字中，如果对于$x \in E$，$c(x) = \sum_i y_i \otimes z_i$，我们可以写（规范地识别$A \otimes_A E$和$E$）

$$
\langle x, uv \rangle = (uv)(x) = \sum_i u(y_i)v(z_i) = v\left( \sum_i u(y_i)z_i \right)
= v(((u \otimes 1_E) \circ c)(x)) = \langle ((u \otimes 1_E) \circ c)(x), v \rangle.
$$

这可以通过说解释为，对于$E^{*\mathrm{gr}}$中次数$p$的所有$u$齐次，$E^{*\mathrm{gr}}$中的左侧乘法$e(u) : v \mapsto uv$是自同态的分级转置次数$-p$

$$(46)$$
$$
i(u) = (u \otimes 1_E) \circ c
$$
$E$；因此，在上面的记号中，

$$
(i(u))(x) = \sum_i u(y_i)z_i.
$$

公式 (46) 还为每个元素 $u \in E^{*\mathrm{gr}}$ 定义元素 $i(u) \in \mathrm{Endgr}_A(E)$；对于所有 $x \in E$ 和所有 $u \in E^{*\mathrm{gr}}$，我们写

$$(47)$$
$$
x \perp u = (i(u))(x)
$$
因此，对于$E^{*\mathrm{gr}}$中的$u$和$v$，

$$
\langle x, uv \rangle = \langle x \perp u, v \rangle.
$$

$E$的元素$x \perp u$被$u$称为$x$的右内部乘积。

这里，在$x$上“操作”的元素$u$再次被放置在$\underline{\phantom{x}}$中水平线的自由端。

对于$E^{*\mathrm{gr}}$中的任意两个元素$u, v$，

$$
x \underline{\phantom{(uv)}} = (x \underline{\phantom{u}}) \underline{\phantom{v}},
$$

其他字

$$
i(uv) = i(v) \circ i(u).
$$

如上令$c(x) = \sum_i y_i \otimes z_i$，从而$x \underline{\phantom{(uv)}} = \sum_i (uv)(y_i)z_i$。如果

$$
c(y_i) = \sum_j y_{ij}' \otimes y_{ij}'',
$$

然后

$$
x \underline{\phantom{(uv)}} = \sum_{i,j} u(y_{ij}')v(y_{ij}'')z_i.
$$

另一方面，如果$c(z_i) = \sum_k z_{ik}' \otimes z_{ik}''$，那么

$$
(x \underline{\phantom{u}}) \underline{\phantom{v}} = \sum_{i,k} u(y_i)v(z_{ik}')z_{ik}''.
$$

现在，$E$的共结合性表明 (no. 2, 命题 1)

$$
\sum_{i,j} y_{ij}' \otimes y_{ij}'' \otimes z_i = \sum_{i,k} y_i \otimes z_{ik}' \otimes z_{ik}''
$$

表达式(49)和(50)的等式源自以下事实：它们分别是(51)的左侧和右侧的像在线性映射$f$下从$E \otimes E \otimes E$到$E$使得$f(x \otimes y \otimes z) = u(x)v(y)z$。

另一方面，我们记得（no. 2，命题 3），代数$E^{*\mathrm{gr}}$的单位元是线性形式$e : x \mapsto \gamma(x).1$；因此

$$
x \underline{\phantom{e}} = \sum_i \gamma(y_i)z_i = x
$$

凭借余单位的定义。由于映射$u \mapsto i(u)$是线性的，可以看出合成$(u, x) \mapsto x \underline{\phantom{u}}$定义的外法则是$E$上的*右*$E^{*\mathrm{gr}}$-模块结构。

同样，我们定义，对于所有$u \in E^{*\mathrm{gr}}$，$E$的自同态

$$
i'(u) = (1_E \otimes u) \circ c
$$

并且，对于所有 $x \in E$，我们写

$$
(i'(u))(x) = u \underline{\phantom{x}}
$$

而$E$的这个元素被u*称为x的*左内部乘积。如上所示，外法则$(u, v) \mapsto u \sqcup x$定义*左$E^{*\mathrm{gr}}$模块结构*在$E$上。而且，这两个结构是*相容的*的，在其他字，

$$(54)$$
$$(u \sqcup x) \sqcap v = u \sqcup (x \sqcap v)$$

$E^{*\mathrm{gr}}$ (II, § 1, no. 14) 中的 $u, v$。与上面相同的记号，(54)的左手边是$\sum_{i,j} u(z_i)v(y_{ij}')y_{ij}''$，右手边是$\sum_{i,k} v(y_i)u(z_{ik}'')z_{ik}'$；它们的等式源自以下事实：它们是（51）的左侧和右侧在$E \otimes E \otimes E$的线性映射$g$下各自的像进入$E$，使得$g(x \otimes y \otimes z) = v(x)u(z)y$。

因此可以看出，$E$定义上的合成的两个外法则在这个集合上是一个$(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-双模块*结构。

当余代数 $E$ *可交换*时，则 $u \sqcup x = x \sqcap u$ 对于所有 $x \in E$ 和 $u \in E^{*\mathrm{gr}}$；当它是*反交换*（§ 4, no. 9）和$u \in E_p^*$和$x \in E_q$时，我们可以将$c(x) = \sum_{0 \leq j \leq q} \left( \sum_i y_{ij} \otimes z_{i, q-j} \right)$与$y_{ij}$和$z_{ij}$写在$E_j$中，对于所有$j$，然后写成假设

$$\sum_i z_{ij} \otimes y_{i, q-j} = (-1)^{j(q-j)} \sum_i y_{ij} \otimes z_{i, q-j}.$$

定义、$x \sqcap u = \sum_{0 \leq j \leq q} \left( \sum_i u(y_{ij})z_{i, q-j} \right)$ 和

$$u \sqcup x = \sum_{0 \leq j \leq q} \left( \sum_i u(z_{i, q-j})y_{ij} \right).$$

作为 $u(y_{ij}) = 0$（分别为 $u(z_{i, q-j}) = 0$ 除非 $j = p$（分别为 $q - j = p$），从上面可以看出 $u \sqcup x = (-1)^{p(q-p)} x \sqcap u$。

最后，让$\phi : E \to F$成为*分级的余代数态射*；那么可以看出(no. 2)分级的转置$t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$是*分级的代数同态*；因此，对于$F^{*\mathrm{gr}}$中的$x \in E$、$u, v$，

$$
\langle \phi(x \sqcap t\phi(u)), v \rangle = \langle x \sqcap t\phi(u), t\phi(v) \rangle = \langle x, t\phi(u)t\phi(v) \rangle = \langle x, t\phi(uv) \rangle
$$
$$
= \langle \phi(x), uv \rangle = \langle \phi(x) \sqcap u, v \rangle
$$

从而

$$(55)$$
$$\phi(x) \sqcap u = \phi(x \sqcap t\phi(u));$$

和类似地

$$(56)$$
$$u \sqcup \phi(x) = \phi(t\phi(u) \sqcup x).$$

在其他字中，$\phi$ 是 $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-bimodule* $E$ 到 $(F^{*\mathrm{gr}}, F^{*\mathrm{gr}})$*-bimodule* $F$ 的 $F^{*\mathrm{gr}}$*-同态*，相对于环同态

$$
t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}.
$$

#### 例 {#alg-iii-s11-n7-exa-1 .statement tag=0687}

特别地，当E是余代数T(M)、S(M)或对于A-模M(no. 1、例5、6和7)的$\Lambda(M)$之一时，可以应用以上内容。 为了明确地找到由此获得的双模结构，我们再次认同在$T(M)^{*gr}$（分别$S(M)^{*gr}$，$\Lambda(M)^{*gr}$）中具有次数n的齐次元素f，具有*n线性形式*（分别为。 *对称 n 线性形式*，分别。 *交错的 n 线性形式*，也称为 *n 形式*）在 $M^n$ 上。 表达乘积就足够了

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f \text{ (resp. } (x_1 x_2 \ldots x_p) \triangleleft f,
$$

分别。 $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f$对于M的元素的每个有限序列$(x_i)_{1 \leq i \leq p}$以及左侧内部乘积的类似物。现在，no. 1的定义(46)和(52)以及公式(3)、(6)和(9)分别给出：

$$
\begin{cases}
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = 0 \\
(x_1 x_2 \ldots x_p) \triangleleft f = f \triangleright (x_1 x_2 \ldots x_p) = 0 \quad \text{for } p < n. \\
(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = 0
\end{cases}
$$

对于$p \geq n$，我们分别有

(58) $(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f(x_1, \ldots, x_n)x_{n+1} \otimes \cdots \otimes x_p$

(59) $(x_1 x_2 \ldots x_p) \triangleleft f = \sum_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \cdots x_{\sigma(p)}$

(60) $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}$

（其中，在（59）和（60）中，对置换 $\sigma \in \mathfrak{S}_p$ 进行求和，即 $\mathbf{N}$ 的每个区间* $[1, n]$ 和 $[n+1, p]$ 上的 *递增；并且类似地

(61) $f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = f(x_{p-n+1}, \ldots, x_p)x_1 \otimes x_2 \otimes \cdots \otimes x_{p-n}$

(62) $f \triangleright (x_1 x_2 \ldots x_p) = \sum_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \cdots x_{\sigma(p-n)}$

(63) $f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p-n)}$

（其中，在（62）和（63）中，对置换 $\sigma \in \mathfrak{S}_p$ 进行求和，即 $\mathbf{N}$ 的每个区间* $[1, p-n]$ 和 $[p-n+1, p]$ 上的 *递增）。

### 8. 内部乘积：BIGEBRAS 案例

令 E 为分级 bigebra（或倾斜分级 bigebra）（no. 4，定义 3）；然后是 nos 的结果。对于所有 $x \in E$ 和所有 $u \in E^{*\mathrm{gr}}$，6 和 7 可以应用于定义右侧（分别为左侧）内部乘积 $x \triangleleft u \in E$ 和 $u \triangleleft x \in E^{*gr}$（分别为 $u \triangleright x \in E$ 和 $x \triangleright u \in E^{*gr}$）。这样在$E$上就得到了$(E, E)$双模结构和$(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$双模结构。更远：

#### 命题 9 {#alg-iii-s11-prop-9 .statement tag=0688}

*令$E$为分级bigebra（分别为倾斜分级bigebra）。对于 $E$ 中次数 1 的每个元素 $x$，内部乘积与 $x$ 的左、右内部乘积分别是代数的推导（反推导）（$§ 10$、no. 2） $E^{*\mathrm{gr}}$.*

在no. 6的记号中，对于分级bigebra（或倾斜分级bigebra）$E$中*次数* 1的每个齐次元素$x$，
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$
由 no. 3 的命题 5 以及 $c$ 是次数 0 的同态组成。首先假设 $E$ 是一个分级大数。对于所有$y \in E$，由定义
$$
\langle (uv) \mathbin{\&} x, y \rangle = \langle uv, xy \rangle = m((u \otimes v)(c(xy)))
$$
由于 $c$ 是 *代数* 同态，$c(xy) = c(x)c(y)$。让$c(y) = \sum_i s_i \otimes t_i$与$s_i$和$t_i$在$E$中；因此
$$
c(xy) = \sum_i (xs_i) \otimes t_i + \sum_i s_i \otimes (xt_i).
$$
因此$\langle (uv) \mathbin{\&} x, y \rangle = \sum_i u(xs_i)v(t_i) + \sum_i u(s_i)v(xt_i)$。但我们可以写
$$
\sum_i u(xs_i)v(t_i) = m(((u \mathbin{\&} x) \otimes v)(c(y))) = \langle (u \mathbin{\&} x)v, y \rangle
$$
和类似地
$$
\sum_i u(s_i)v(xt_i) = m((u \otimes (v \mathbin{\&} x))(c(y))) = \langle u(v \mathbin{\&} x), y \rangle,
$$
从而，返回记号$i(x)$，持续内部乘积。
$$(64)$$
$$(i(x))(uv) = ((i(x))(u))v + u((i(x))(v))$$
这证明$i(x)$是$E^{*\mathrm{gr}}$中的*推导*。

现在假设 $E$ 是一个 *skew* 分级大数，即 $u \in E_p^*$、$v \in E_q^*$ 和 $y \in E_r$；那么我们可以写
$$
c(y) = \sum_{0 \leq j \leq r} \left( \sum_i s_{ij} \otimes t_{i,r-j} \right)
$$
其中 $s_{ij}$ 和 $t_{ij}$ 属于至 $E_j$；通过 $E^g \otimes_A E$ 中的乘积的定义，则
$$
c(xy) = c(x)c(y) = \sum_{0 \leq j \leq r} \left( \sum_i (xs_{ij}) \otimes t_{i,r-j} + (-1)^j \sum_i s_{ij} \otimes (xt_{i,r-j}) \right)
$$
这次从而
$$
\langle (uv) \mathbin{\&} x, y \rangle = \sum_{0 \leq j \leq r} \left( \sum_i u(xs_{ij})v(t_{i,r-j}) + (-1)^j \sum_i u(s_{ij})v(xt_{i,r-j}) \right).
$$

然后还有$\sum_{0 \leq j \leq r} \left( \sum_i u(x s_{ij}) v(t_{i,r-j}) \right) = \langle (u \sqcup x)v, y \rangle$。另一方面，$u(s_{ij}) = 0$除非$j = -p$，因此我们也可以写
$$
\sum_{0 \leq j \leq r} (-1)^j \left( \sum_i u(s_{ij}) v(x t_{i,r-j}) \right) = (-1)^p \langle u(v \sqcup x), y \rangle.
$$
因此我们结论
$$
(i(x))(uv) = ((i(x))(u))v + (-1)^p u((i(x))(v)),
$$
在其他字$i(x)$中是$E^{*gr}$中的*反推导*。 $E$中的次数1的元素$x$与左内部乘积有关的断言也同样证明。

#### 注 {#alg-iii-s11-n8-rem-1 .statement tag=0689}

(1) 令$E$为$A$和$N, N', N''$三个分级$A$模的分级大数。设$m$是$N \times N'$到$N''$的$A$双线性映射；对于$u \in \mathrm{Homgr}_A(E, N)$和$v \in \mathrm{Homgr}_A(E, N')$，让$u.v$表示将$E$分级为$N''$的同态$m \circ (u \otimes v) \circ c$。另一方面，让$i(x)$表示$A$-模块$\mathrm{Homgr}_A(E, N)$、$\mathrm{Homgr}_A(E, N')$和$\mathrm{Homgr}_A(E, N'')$中的（右或左）内部乘积和$x \in E$。那么，如果 $x$ 是次数* 1 的*，
$$
(i(x))(u.v) = ((i(x))(u)).v + u.((i(x))(v))
$$
对于所有 $u \in \mathrm{Homgr}_A(E, N)$ 和 $v \in \mathrm{Homgr}_A(E, N')$。

在相同条件下，如果$E$是斜分级大数且$u$是次数$p$的齐次，则
$$
(i(x))(u.v) = ((i(x))(u)).v + (-1)^p u.((i(x))(v)).
$$
证明与命题 9 相同。

(2) 与上述证明相同的论证，更一般地证明，对于所有$x \in E$，如果$c(x) = \sum_j x'_j \otimes x''_j$，那么，对于$E^{*gr}$中的所有$u, v$，“莱布尼茨公式”
$$
(i(x))(uv) = \sum_j (i(x'_j))(u).(i(x''_j))(v)
$$
成立。特别是，对于分级 bigebra $E$ 的每个“原始”元素，即 $c(x) = x \otimes 1 + 1 \otimes x$、$i(x)$ 是 $E^{*gr}$ 的 *推导*。

#### 命题 10 {#alg-iii-s11-prop-10 .statement tag=068A}

*令$E$为分级bigebra（分别为倾斜分级bigebra）。对于 $E^{*gr}$ 中次数 1 的每个元素 $f$，左和右内部乘积是代数 $E$ 的推导（或反导数）。*

让$x \in E_p, y \in E_q$（$p \geq 1, q \geq 1$）。通过命题 5 of no. 3，我们可以写出
$$
c(x) = x \otimes 1 + \sum_{1 \leq j \leq p-1} \left( \sum_i x'_{ij} \otimes x''_{ij,p-j} \right) + 1 \otimes x
$$
$$
c(y) = y \otimes 1 + \sum_{1 \leq k \leq q-1} \left( \sum_i y'_{i,k} \otimes y''_{i,q-k} \right) + 1 \otimes y
$$

其中$x'_{ij}$和$x''_{ij}$属于到$E_j$，$y'_{ik}$和$y''_{ik}$到$E_k$。如果 $E$ 是分级大数，则 $c(xy) = c(x)c(y)$ 属于到 $E_1 \otimes E$ 的分量等于
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
因此定义
$$
(xy) \leftarrow f = \sum_i f(x'_{i,1})x''_{i,p-1}y + \sum_i f(y'_{i,1})xy''_{i,q-1}
$$
$$
= (x \leftarrow f)y + x(y \leftarrow f)
$$
右内部乘积乘$f$是*推导*。另一方面，如果 $E$ 是倾斜分级大数，则 $c(xy)$ 属于到 $E_1 \otimes E$ 的分量等于
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + (-1)^p \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
这次我们得到
$$
(xy) \leftarrow f = (x \leftarrow f)y + (-1)^p x(y \leftarrow f)
$$
这表明 $i(f)$ 是一个*反导数*。对于左边内部乘积 $f$ 的论证类似。

#### 例 {#alg-iii-s11-n8-exa-1 .statement tag=068B}

命题 9 和 10 特别适用于分级 bigebra $S(M)$ 和倾斜分级 bigebra $\Lambda(M)$。 $S(M)$（或$S(M)^{*gr}$）中的内部乘积乘以次数1的元素是*推导*，它*可与1另一个*交换，因为$S(M)$（或$S(M)^{*gr}$）是可交换的。

类似地，$\Lambda(M)$（或$\Lambda(M)^{*gr}$）中次数 1 的内部乘积和元素是*反导数*，即*零平方*，对于元素的平方代数 $\Lambda(M)$（或$\Lambda(M)^{*gr}$）中的次数 1 为零。

### 9. $T(M)$和$T(M^*)$、$S(M)$和$S(M^*)$、$\Lambda(M)$和$\Lambda(M^*)$之间的内部乘积

$T(M)$（分别$S(M)$、$\Lambda(M)$）上的右内部乘积定义，以及代数$T(M)^{*gr}$（分别$S(M)^{*gr}$、$\Lambda(M)^{*gr}$）上的右模结构 （no. 7，*例*）。 使用 no. 5 的典范同态 $\theta_T$（分别为 $\theta_S$、分别为 $\theta_\Lambda$），我们得出
$T(M)$ 上的右$T(M^*)$模块结构
$S(M)$ 上的右$S(M^*)$模块结构
$\Lambda(M)$ 上的左$\Lambda(M^*)$模块结构。

这些结构中的任何一个外法则也表示为
$$
(z^*, t) \mapsto i(z^*) \cdot t
$$

（滥用语言）；在$T(M)$或$S(M)$的情况下，我们也写$t \prec z^*$而不是$i(z^*) . t$；另一方面，我们在$\Lambda(M)$的情况下写为$z^* \prec t$，并说这是$t$乘$z^*$的*左*内部乘积，从那时起我们就有了一个*左*$\Lambda(M^*)$-模块律。对于次数$n$的$z^*$齐次和次数$p$的$t$齐次，如果$p < n$则为$i(z^*) . t = 0$，并且对于$x_i \in M$（$1 \leq i \leq p$），$x_j^* \in M^*$ ($1 \leq j \leq n$)和$p \geq n$，凭借no. 7的公式(58)、(59)和(60)，

$$
(66)\quad i(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) . (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$
$$
= \left( \prod_{j=1}^n \langle x_j^*, x_j \rangle \right) x_{n+1} \otimes \cdots \otimes x_p
$$

$$
(67)\quad i(x_1^* x_2^* \ldots x_n^*) . (x_1 x_2 \ldots x_p) = \sum_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
$$

$$
(68)\quad i(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) . (x_1 \wedge x_2 \wedge \cdots \wedge x_p)
$$
$$
= (-1)^{n(n-1)/2} \sum_\sigma \varepsilon_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}
$$

其中，公式 (67) 和 (68)，$\sigma$ 穿过置换 $\sigma \in \mathfrak{S}_p$ 的集合，即在区间 $\{1, n\}$ 和 $\{n + 1, p\}$ 上的 *递增*。

我们还可以在内部乘积记号中写，

$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_T(u^* v^*) \rangle \quad \text{for } t \in T(M), u^*, v^* \text{ in } T(M^*)
$$
$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_S(u^* v^*) \rangle \quad \text{for } t \in S(M), u^*, v^* \text{ in } S(M^*)
$$
$$
\langle v^*, u^* \prec t \rangle = \langle \theta_\Lambda(u^* \wedge v^*), t \rangle \text{ for } t \in \Lambda(M), u^*, v^* \text{ in } \Lambda(M^*).
$$

我们留给读者的任务是明确找到左内部乘积的类似公式，这次使用公式（61）、（62）和（63）。

The above can be applied with $M$ replaced by its dual $M^*$; $M^*$ must then be replaced by the bidual $M^{**}$ and $T(M^*)$, for example, thus has a right module structure over the algebra $T(M^{**})$. 但是典范映射$c_M : M \to M^{**}$定义代数同态$T(c_M) : T(M) \to T(M^{**})$，通过它$T(M^*)$有一个*右*$T(M)$-*模*结构。 Similarly $S(M^*)$ (resp. $\Lambda(M^*)$) has a *right* $S(M)$-*module* (resp. *左*$\Lambda(M)$-*模*)结构。 通过交换$M$和$M^*$的角色，直接从上面导出这些模的显式公式给出外法则。 注，对于所有 $x \in M$，$i(x)$ 始终是 *推导*（分别是 *分级代数 $S(M^*)$（分别为 $\Lambda(M^*)$）的零平方*）的反推导。

#### 命题 11 {#alg-iii-s11-prop-11 .statement tag=068C}

*典范同态* $\theta_T : T(M^*) \to T(M)^{*gr}$（分别$\theta_S : S(M) \to S(M)^{*gr}$，分别$\theta_\Lambda : \Lambda(M^*) \to \Lambda(M)^{*gr}$）*是右* $T(M)$-*模*（分别*右* $S(M)$-*模*，分别*左* $\Lambda(M)$-*模*） *同态.*

我们首先证明，对于 $z^* \in T(M^*)$ 和 $t \in T(M)$，

$$
\theta_T(z^* \wedge t) = \theta_T(z^*) \wedge t.
$$

由于$M$是代数$T(M)$的生成的系统，所以当$t = x \in M$时我们只需证明(69)；此外，我们可以将注意力限制在$z^* = x_1^* \otimes x_2^* \otimes \cdots \otimes x_p^*$、$x_j^* \in M^*$的情况，然后通过（66）将$M$和$M^*$的角色互换，$z^* \wedge x = \langle x, x_1^* \rangle x_2^* \otimes \cdots \otimes x_p^*$。因此，对于$M$中的所有$y_2, \ldots, y_p$，

$$
\begin{align*}
\langle \theta_T(z^* \wedge x), y_2 \otimes y_3 \otimes \cdots \otimes y_p \rangle &= \langle x, x_1^* \rangle \prod_{j=2}^p \langle y_j, x_j^* \rangle \\
&= \langle \theta_T(z^*), x \otimes y_2 \otimes \cdots \otimes y_p \rangle \\
&= \langle \theta_T(z^*) \wedge x, y_2 \otimes \cdots \otimes y_p \rangle
\end{align*}
$$

从而 (69)。

其次，我们证明对于 $z^* \in S(M^*)$ 和 $t \in S(M)$，

$$
\theta_S(z^* \wedge t) = \theta_S(z^*) \wedge t.
$$

如上所述，我们可以将极限应用于案例 $t = x \in M$。但更进一步，这里$i(x)$是$S(M^*)$的推导和$S(M)^{*gr}$的推导。因此（§ 10, no. 7，命题 9 的推论）足以验证$z^* = x^* \in M^*$的（70），因为$M^*$是生成的系统 of $S(M^*)$；但这是微不足道的，两条边等于 $\langle x^*, x \rangle$。类似的论证证明关系

$$
\theta_\wedge(t \wedge z^*) = t \wedge \theta_\wedge(z^*)
$$

对于$z^* \in \Lambda(M^*)$和$t \in \Lambda(M)$：观察到，对于$x \in M$，$i(x)$是$\Lambda(M^*)$以及$\Lambda(M)^{*gr}$的反导数，并使用§ 10, no. 7，推论命题 9。左有一个类似的结果内部乘积。

### 10. 在有限生成自由模的情况下显式内部乘积形式

令$M$为有限生成的自由$A$模块，$M$的$(e_i)_{1 \leq i \leq n}$基和$M^*$的$(e_i^*)_{1 \leq i \leq n}$对偶基。对于$\{1, n\}$的元素中的每个有限序列$s = (i_1, \ldots, i_p)$，令$e_s = e_{i_1} \otimes e_{i_2} \otimes \cdots \otimes e_{i_p}$（分别为$e_s^* = e_{i_1}^* \otimes \cdots \otimes e_{i_p}^*$）。我们知道（§ 5, no. 5，定理 1）$A$模块$T(M)$的$e_s$形式基和$A$模块的$e_s^*$基 $T(M^*)$。如果$s, t$是$\{1, n\}$的元素的两个有限序列，令$s.t$表示序列，如下获得：如果$s = (i_1, \ldots, i_p)$和$t = (j_1, \ldots, j_q)$，则$s.t$是序列$(i_1, \ldots, i_p, j_1, \ldots, j_q)$与$p + q$项。然后$e_{s.t} = e_s \otimes e_t$。然后从 (66) 得出

$$
\begin{cases}
e_s \wedge e_t^* = 0 & \text{if } s \text{ is not of the form } t.u \\
e_{t.u} \wedge e_t^* = e_u.
\end{cases}
$$

类似地，对称代数 $S(M)$ 具有单项式 $e^\alpha$ 的基集合以及单项式 $e^{*\alpha}$ 的 $\alpha \in \mathbf{N}^n$ (§ 6, no. 6, 定理 1) 和 $S(M^*)$ 集合与 $\alpha \in \mathbf{N}^n$；回想一下（no. 5），$u_\alpha$对于$|\alpha| = k$来说，表示$(S^k(M))^*$的基的元素，是$S^k(M)$的基$(e^\alpha)_{|\alpha|=k}$的对数； $u_\alpha$ 对应 $\alpha \in \mathbf{N}^n$，因此形式基等于 $S(M)^{*gr}$。右内部乘积的定义在 $S(M)^{*gr}$ 中乘以 $e^\beta$ 作为乘法的转置在 $S(M)$ 中乘以 $e^\beta$ 那么表明

$$
\begin{cases}
u_\alpha \perp e^\beta = 0 & \text{if } \alpha \not\geq \beta \\
u_\alpha \perp e^\beta = u_{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(73)

类似地，由于$S(M)$在这里被规范地与$S(M)^{*gr}$的分级对偶等同，$i(u_\beta)$是$S(M)^{*gr}$中$u^\beta$对乘法的分级转置，因此来自乘法表 (33) (no. 5) 基 $(u_\alpha)$ 我们推断

$$
\begin{cases}
e^\alpha \perp u_\beta = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp u_\beta = (\beta, \alpha - \beta)e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(74)

至于$S(M)$的元素的右内部乘积到$S(M^*)$的元素，这个乘积的定义(no. 9)和no. 5的公式(34)让我们可以推导出(74) 公式

$$
\begin{cases}
e^\alpha \perp e^{*\beta} = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp e^{*\beta} = \frac{\alpha!}{(\alpha-\beta)!} e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(75)

内部乘积 $S(M^*)$ 元素元素 $S(M)$ 交换有类似的公式 $M$ 和$M^*$ 的角色（因为$M^{**}$ 在这里被标识为$M$）。

#### 注 {#alg-iii-s11-n10-rem-1 .statement tag=068D}

给出基 $(e_i)_{1 \leq i \leq n}$ 可以让我们用多项式代数 $A[X_1, \ldots, X_n]$ (§ 6, no. 6) 来计算认同代数 $S(M)$； 公式(75)表明内部乘积除以$e^{*\alpha}$只是微分算子$D^\alpha = D_1^{\alpha_1}D_2^{\alpha_2}\ldots D_n^{\alpha_n}$，其中$D_i = \partial/\partial X_i$对应$1 \leq i \leq n$（§ 10, no. 11，例）。

最后考虑外部代数$\Lambda(M)$，其具有元素$e_J$的基集合，其中$J$穿过$\mathbf{N}$区间$\{1, n\}$的集合或子集 （§ 7, no. 8，定理1）；同样，$\Lambda(M^*)$有基元素$e_J^*$。由no. 9的公式(68)得出

$$
\begin{cases}
e_K^* \wedge e_J = 0 & \text{if } K \notin J \\
e_K^* \wedge e_J = (-1)^{p(p-1)/2} \rho_{K, J-K} e_{J-K} & \text{if } K \subset J \text{ and } p = \operatorname{Card}(K),
\end{cases}
$$

(76)

其中$\rho_{K, J-K}$是由§ 7, no. 8的公式(19)定义的数。有类似的公式，但$M$和$M^*$的角色互换。

### 11. 对于 $n$ 维度自由模 M，同构介于 $\wedge^p(M)$ 和 $\wedge^{n-p}(M^*)$ 之间

#### 命题 12 {#alg-iii-s11-prop-12 .statement tag=068E}

*设M为维数n中的自由A-模；令$e \in \wedge^n(M)$为元素，形成$\wedge^n(M)$的基，并令$e^*$为$\wedge^n(M^*)$的元素，使得$\{(-1)^{n(n-1)/2} \theta_{\wedge}(e^*)\}$为$(\wedge^n(M))^*$中$\{e\}$的对偶基。令$\phi : \wedge(M^*) \to \wedge(M)$为映射$z \mapsto z \wedge e^*$和$\phi' : \wedge(M^*) \to \wedge(M)$映射$z^* \mapsto z^* \wedge e$。令$\phi_p$（分别$\phi'_p$）为限制 / $\phi$（分别$\phi'$）到$\wedge^p(M)$（分别$\wedge^p(M^*)$）。然后：

(i) *映射$\phi$是左$\wedge(M)$-模块同构且映射$\phi'$是左$\wedge(M^*)$-模块同构；此外，映射 $\phi$ 和 $\phi'$ 是 1 另一个的倒数。*

(ii) *映射$\phi_p$是A-模$\wedge^p(M)$中的同构到A-模$\wedge^{n-p}(M^*)$，并且映射$\phi'_p$是A-模$\wedge^p(M^*)$中的同构到A-模$\wedge^{n-p}(M)$。

(iii) *如果我们将$u \in \wedge(M)$和$v^* \in \wedge(M^*)$写为$B(u, v^*) = \langle u, \theta_{\wedge}(v^*) \rangle$，那么，对于$u^* \in \wedge^p(M^*)$和$v^* \in \wedge^{n-p}(M^*)$，

$$
B(\phi'_p(u^*), v^*) = (-1)^{p(n-p)} B(u^*, \phi'_{n-p}(v^*)).
$$

$\phi$ 是 $\wedge(M)$ 线性且 $\phi'$ 是 $\wedge(M^*)$ 线性这一事实是从公式 $(u \wedge v) \wedge e^* = u \wedge (v \wedge e^*)$ 和 $(u^* \wedge v^*) \wedge e = u^* \wedge (v^* \wedge e)$ (no. 6, 公式 (37)) 得出的，使用$\theta_{\wedge}$ 是$\wedge(M^*)$的同构到反代数到$\wedge(M)^*$。另一方面，M 存在基 $(e_i)_{1 \leq i \leq n}$，使得

$$
e = e_1 \wedge e_2 \wedge \cdots \wedge e_n \quad \text{and} \quad e^* = (-1)^{n(n-1)/2} e_1^* \wedge e_2^* \wedge \cdots \wedge e_n^*,
$$

其中$(e_i^*)$是基对数$(e_i)$。我们写$I = \{1, n\}$；从 (76) 可以看出，对于 I 的每个子集 J 且 p 元素，

$$
\begin{cases}
\phi(e_J) = (-1)^{n(n-1)/2 + p(p-1)/2} \rho_{J, I-J} e_I^* J \\
\phi'(e_J^*) = (-1)^{p(p-1)/2} \rho_{J, I-J} e_{I-J}.
\end{cases}
$$

这就证明了$\phi$和$\phi'$是双射的；此外$\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$（§ 7, no. 8，公式（21））；如数

$$
\frac{n(n-1)}{2} + \frac{p(p-1)}{2} + \frac{(n-p)(n-p-1)}{2} + p(n-p) = n(n-1)
$$

是偶数，因此 $\phi$ 和 $\phi'$ 是 1 另一个的倒数。最后，要证明(77)，只需取$u^* = e_J^*$和$v^* = e_{I-J}^*$即可；验证也遵循$\theta_{\wedge}$、公式 (78) 和关系 $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (§ 7, no. 8、公式 (21)) 的定义。 注对于 $u^* \in \wedge^p(M^*)$ 和 $v^* \in \wedge^{n-p}(M^*)$，

B(\phi_p'(u^*), v^*) 是 $u^* \wedge v^*$ 相对于 $\Lambda^n(M^*)$ 的基 $\{e^*\}$ 在符号范围内的系数。

#### 命题 13 {#alg-iii-s11-prop-13 .statement tag=068F}

*假设记号为命题 11，每自同态 g 为 A-模 M。*

$$(79)$$
$$(\det g)\phi = \Lambda^{(tg)} \circ \phi \circ \Lambda(g).$$

显然$\Lambda^{(tg)} = \theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}$；因为 $\Lambda(g)$ 是代数 $\Lambda(M)$ 的自同态和定义，对于所有
$$z \in \Lambda(M), \quad \theta_{\Lambda}(\Lambda(g)(z) \perp e^*) = \theta_{\Lambda}(e^*) \perp \theta_{\Lambda}(\Lambda(g)(z)),$$
我们从 no. 6 的公式 (42) 推断出
$$
((\theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}) \circ \phi \circ \Lambda(g))(z) = \theta_{\Lambda}^{-1}(t\Lambda(g)(\theta_{\Lambda}(e^*)) \perp z)
= z \perp (\Lambda^{(tg)}(e^*)) = (\det g)(z \perp e^*) = (\det g)\phi(z)
$$
考虑到 § 8, no. 4、命题 8。

#### 推出{#alg-iii-s11-n11-cor-1 .statement tag=068G}

*每自同构克E，*
$$(80)$$
$$\Lambda^{(tg^{-1})} = (\det g)^{-1}\phi \circ (\Lambda(g)) \circ \phi^{-1}.$$

### 12. 与 p 向量相关的子空间的应用

令 K 为域，E 向量空间超过 K。回想一下，每个 $p$ 向量 $z \in \Lambda^p(E)$ 都与 E 的有限维子空间 $M_z$ 相关联，即 E 的最小的向量子空间 M，使得$z \in \Lambda^p(M)$（§ 7, no. 2，命题 4 的推论）。

#### 命题 14 {#alg-iii-s11-prop-14 .statement tag=068H}

(i) *$M_z$在$E^*$中的正交是$x^* \in E^*$的集合使得$x^* \perp z = 0$。*

(ii) *与 z 相关的子空间 $M_z$ 是 $\Lambda^{p-1}(E^*)$ 的映射 $\lambda_z : u^* \mapsto u^* \perp z$ 下的 $\Lambda^{p-1}(E^*)$ 像进入 E。*

令 N 表示 $\lambda_z$ 的像。对于 $x^* \in E^*$ 和 $u^* \in \Lambda^{p-1}(E^*)$，
$$
\langle \theta_{\Lambda}(x^*), u^* \perp z \rangle = \langle \theta_{\Lambda}(u^* \wedge x^*), z \rangle = (-1)^{p-1} \langle \theta_{\Lambda}(x^* \wedge u^*), z \rangle \\
= (-1)^{p-1} \langle \theta_{\Lambda}(u^*), x^* \perp z \rangle.
$$
因此，为了使$x^*$与N正交，$x^* \perp z$与$\theta_{\Lambda}(\Lambda(E^*))$正交是充分必要的。现在，后者条件相当于说即$x^* \perp z = 0$；令 $(e_{\lambda})_{\lambda \in L}$ 为 E 的基；给L一个全序，可以看出（§ 7, no. 8，定理1），对于J来说，$e_J$，经过L的有限子集的集合$\mathscr{F}(L)$，$\Lambda(E)$的形式基；然后从no. 5的公式(30)得出，元素$\theta_{\wedge}(e_J^*)$在一个符号内是$\wedge(E)$上相对于基$(e_J)$的坐标形式； 从而我们的断言。

因此，N 的正交由 $x^* \in E^*$ 组成，使得 $x^* \perp z = 0$ 并且 (i) 的结论将由 (ii) 得出。

我们首先显示$N \subset M_z$。令 M 为 E 的向量子空间，使得 $z \in \wedge(M)$ 且令 $j : M \to E$ 为典范嵌入；设$\mu_z$将$\wedge^{p-1}(M^*)$的映射$v^* \mapsto v^* \perp z$代入M；从 no. 7 的公式 (60) 可以得出，存在规范因式分解

$$
\lambda_z : \wedge^{p-1}(E^*) \xrightarrow{\wedge^{p-1}(t_j)} \wedge^{p-1}(M^*) \xrightarrow{\mu_z} M \xrightarrow{j} E
$$

这通过$M_z$的定义证明了$N \subset M$，从而证明了$N \subset M_z$。仍有待验证$N = M_z$。假设逆命题：则存在$M_z$和元素$x^* \in E^*$的基$(e_i)_{1 \leq i \leq n}$，使得$\langle x^*, e_1 \rangle = 1, \langle x^*, e_j \rangle = 0$对应$2 \leq j \leq n$，并且$x^*$与N正交，因此$x^* \perp z = 0$。我们写为$z = \sum_H a_H e_H$，其中和用$p$元素取代了$\{1, n\}$的子集。通过 (68) (no. 9)，

$$
x^* \perp e_H = 0 \quad \text{if } 1 \notin H \\
x^* \perp e_{\{1\} \cup H} = e_H \quad \text{if } H \subset \{2, n\}
$$

这表明关系$x^* \perp z = 0$意味着$a_H = 0$代表$1 \in H$。但这是不可能的，因为$z$将属于变为$\wedge^p(M')$，其中$M'$是$e_2, \ldots, e_n$生成的M的子空间。

### 13.纯$p$-向量。格拉斯曼尼亚人

设 K 为域，E 向量空间超过 K。如果$p$-向量 $z \in \wedge^p(E)$ 为非零且 E 中存在向量 $x_1, \ldots, x_p$ 使得 $z = x_1 \wedge x_2 \wedge \cdots \wedge x_p$，则称其为*纯*（或有时 *可分解*）。为此，与 $z$ 关联的子空间 $M_z$（对于 $z \neq 0$ 始终为维数 $\geq p$）*精确*为维数 $p$（因为 $\wedge^p(M_z)$ 是维数1)。特别是，当 E 为维数 $n$ 时，每个*非零*标量、$E = \wedge^1(E)$ 的每个非零元素、$\wedge^n(E)$ 的每个非零元素都是*纯*。

#### 命题 15 {#alg-iii-s11-prop-15 .statement tag=068I}

*设E为维数n的向量空间，并令e为$\wedge^n(E)$的元素$\neq 0$（因此形成此向量空间的基）。令 $\phi : \wedge(E) \to \wedge(E^*)$ 为与 e (no. 11, 命题 12) 相关联的向量空间同构。如果 z 是 $\wedge^p(E)$ 的纯元素，则 $\phi(z)$ 是 $\wedge^{n-p}(E^*)$ 的纯元素，并且与 z 和 $\phi(z)$ 关联的子空间是正交的。*

案例 $p = 0$ 和 $p = n$ 是微不足道的。因此假设$1 \leq p \leq n - 1$并令$z = x_1 \wedge \cdots \wedge x_p \neq 0$。那么 E 存在基 $(e_i)_{1 \leq i \leq n}$，使得 $e_i = x_i$ 对应于 $1 \leq i \leq p$ 和 $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$。然后从no. 11的公式(78)得出$\phi(z) = \pm e_{p+1}^* \wedge \cdots \wedge e_n^*$、从而命题。

#### 推论{#alg-iii-s11-n13-cor-1 .statement tag=068J}

*如果 E 的大小为维数 n，则每个非零 $(n-1)$ 向量 E 都是纯向量。*

#### 命题 16 {#alg-iii-s11-prop-16 .statement tag=068K}

*为了使 $\bigwedge^p(E)$ 中的元素 $z \neq 0$ 是纯净的，对于所有 $u^* \in \bigwedge^{p-1}(E^*)$ 是必要且充分的，

$$
(u^* \perp z) \wedge z = 0.
$$

情况$p = 0$很简单，我们假设$p \geq 1$。如果$z = x_1 \wedge \cdots \wedge x_p$、公式 (68) (no. 9) 与$n = p - 1$ 则表明$u^* \perp z$ 是$x_i$ ($1 \leq i \leq p$)、从而 (81) 的线性组合。另一方面，如果与$z$关联的子空间$M_z$是维数$> p$，则考虑该子空间的基$(e_j)_{1 \leq j \leq n}$与$n > p$。从no. 11、命题 13 可以得出，对于某些$u^* \in \bigwedge^{p-1}(E^*)$，每个$e_j$ 都是形式 $u^* \perp z$，而关系 (81) 因此意味着$1 \leq j \leq n$ 的$e_j \wedge z = 0$。由此可见，在表达式$z = \sum_H a_H e_H$中（其中H通过$\{1, n\}$的子集的集合与$p$元素），所有系数$a_H$为零、从而$z = 0$，与假设。

当$u^*$穿过$\bigwedge^{p-1}(E^*)$的*基*时，命题16的标准相当于写出条件(81)。特别是，假设 E 为有限维 $n$，并令 $(e_i)_{1 \leq i \leq n}$ 为 E 的基。条件 (81) 等价于条件

$$(82-(J, H))$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge z \rangle = 0
$$
对于$\{1, n\}$的所有子集 J、H，使得$\mathrm{Card}(J) = p + 1$和$\mathrm{Card}(H) = p - 1$。现在，如果我和我'是$\{1, n\}$的两个子集和$p$元素，no. 10的公式（76）和§ 7, no. 8的乘法表（20）表明

$$
\langle e_J^*, \langle e_H^* \perp e_I \rangle \wedge e_{I'} \rangle = 0
$$
*除非* 存在$i \in \{1, n\}$使得$I - H = \{i\}$和$J - I' = \{i\}$，在这种情况下

$$(83)$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = (-1)^{(p-1)(p-2)/2} \varepsilon_{i, J, H}
$$
其中$\varepsilon_{i, J, H} = \rho_{\{i\}, H} \rho_{\{i\}, I'}$；那么可以说，对于$i \in J \cap C H$，$\varepsilon_{i, J, H}$等于$+1$，如果J的元素的数（$< i$）和H的元素的数（$< i$）具有*相同的奇偶性*，并且否则$-1$。

紧接着，如果我们写$z = \sum_I a_I e_I$，其中我用$p$元素遍历$\{1, n\}$的子集的集合，关系（82–（J，H））相当于关系

$$
\sum_{i \in J \cup C_H} \varepsilon_{i, J, H} a_{J-\{i\}} a_{H \cup \{i\}} = 0.
$$

关系（84）称为*草人的关系*；因此，这些条件是必要且充分的（当J描述子集的集合与$p + 1$元素以及子集的H集合与$p - 1$元素描述$\{1, n\}$时） 元素$z \neq 0$/$\bigwedge^p(E)$*纯净*。

注关系 (84) 不是独立的。对于例、$n = 4$ 和 $p = 2$，Grassmann 的关系约化到单个关系

$$
a_{12} a_{34} - a_{13} a_{24} + a_{14} a_{23} = 0.
$$

令$D_p(E)$为*纯*$p$向量的$\bigwedge^p(E)$由……组成的子集；显然$D_p(E)$在$u$和$v$之间相对于等价关系是饱和的：“存在$\lambda \in K^*$使得$v = \lambda u$”并且$D_p(E)$的两个元素$u, v$在这个关系下是等价的当且仅当与它们相关联的E的子空间$M_u$和$M_v$是相同的。因此，我们因此获得了 E 的 p 维向量子空间* 的 *集合的*规范双射* 到 $D_p(E)$ 的 *像* $G_p(E)$ *在与关联的射影空间* $\mathbf{P}(\bigwedge^p(E))$ 上$\bigwedge^p(E)$。 $\mathbf{P}(\bigwedge^p(E))$的子集$G_p(E)$称为向量空间E的指标$p$的*格拉斯曼*。当E是有限维且$(e_i)_{1 \leq i \leq n}$是E的基时，指标的格拉斯曼$p$是$\mathbf{P}(\bigwedge^p(E))$的点的集合，其中齐次坐标$(a_I)$的系统（相对于$\bigwedge^p(E)$的基$(e_I)$）满足Grassmann的关系 (84)。

当$E = K^n$时，我们有时写为$G_{n,p}(K)$而不是$G_p(K^n)$，这样$G_{n,1}(K) = P_{n-1}(K)$。 映射$M \mapsto M^0$，与$K^n$中的每个$p$维子空间相关联$E^*$中的*正交*子空间（与基的选择下的$K^n$对偶$K^n$的典范基）因此定义将$G_{n,p}(K)$的规范*双射*放到$G_{n,n-p}(K)$上； 命题 15 表明，这个双射是射影空间 $\mathbf{P}(\bigwedge^p(K^n))$ 到射影空间 $\mathbf{P}(\bigwedge^{n-p}(K^n))$ 的规范 *同构* 的 *限制* 到 $G_{n,p}(K)$。

### 习题 {#alg-iii-s11-exercises}

§ 11](exercises/s11/)参见[习题。
