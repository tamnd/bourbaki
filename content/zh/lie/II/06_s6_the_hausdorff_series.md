---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 6
section_title: The Hausdorff series
lang: zh
source: lie-i-iii
book_pages: 155-164, 201-204
pdf_pages: 0173-0182, 0219-0222
extraction: ocr
subsections:
    - "no": 1
      title: EXPONENTIAL AND LOGARITHM IN FILTERED ALGEBRAS
      page: 155
      pdf_page: 173
    - "no": 2
      title: HAUSDORFF GROUP
      page: 157
      pdf_page: 175
    - "no": 3
      title: LIE FORMAL POWER SERIES
      page: 158
      pdf_page: 176
    - "no": 4
      title: THE HAUSDORFF SERIES
      page: 160
      pdf_page: 178
    - "no": 5
      title: SUBSTITUTIONS IN THE HAUSDORFF SERIES
      page: 161
      pdf_page: 179
statements: 14
exercises: 6
content_sha256: 386c2bfe43a8eb15f8ed9586f9f2056968c45cb2f2e7bbe01c4b505bf987619d
translated_from: content/en/lie/II/06_s6_the_hausdorff_series.md
translation_method: google
source_content_sha256: 415bac69237edc26c3196e7b8c6ae4c55426a40b051a938d4b7c3803c5c86eba
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 045ce1d28a980285113df13bed2fc27b294e56664d9ba15e5e83ab3024522ec9
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 6。豪斯多夫级数

*在本段中，我们假设 $K$ 是特征 0 的域。*

### 1. 过滤后的指数和对数代数

令$A$为单位结合律代数，它是豪斯多夫且在真实过滤$(A_\alpha)$下完成。我们写$m = A_0^+ = \bigcup_{\alpha > 0} A_\alpha$。

对于$x \in m$，族$(x^n/n!)_{n \in \mathbf{N}}$是可求和的。我们写

$$
e^x = \exp x = \sum_{n \geqslant 0} x^n/n!.
$$

那么$\exp(x) \in 1 + m$和映射$\exp : m \to 1 + m$被称为$A$的*指数映射*。

对于所有$y \in 1 + m$，族$((-1)^{n-1}(y-1)^n/n)_{n \geqslant 1}$是可求和的。我们写

$$
\log y = \sum_{n \geqslant 1} (-1)^{n-1}(y-1)^n/n.
$$

那么$\log y \in m$和映射$\log : 1 + m \to m$被称为$A$的*对数映射*。

#### 命题 1 {#lie-ii-s6-prop-1 .statement tag=0A61}

*指数映射是 $m$ 到 $1 + m$ 的同胚，对数映射是逆同胚。*

对于$x \in A_\alpha$，$\frac{x^n}{n!} \in A_{n\alpha}$。由此可见，定义指数的级数对于$\alpha > 0$均匀收敛于集合$A_\alpha$；由于$A_\alpha$在$m$和$m = \bigcup_{\alpha > 0} A_\alpha$开，所以指数映射是连续的。类似地可以证明对数映射是连续的。

设 $e$ 和 $l$ 为形式幂级数，没有常数项

$$
e(X) = \sum_{n \geq 1} \frac{X^n}{n!}, \quad l(X) = \sum_{n \geq 1} (-1)^{n-1} X^n / n.
$$

我们知道（*代数*，章IV, § 6, no. 9）$e(l(X)) = l(e(X)) = X$在$\hat{A}(\{X\}) = K[[X]]$。通过代换 (§ 5, no. 1)，我们推断出

$$
e(l(x)) = l(e(x)) = x
$$

$x \in m$；作为

$$
\exp x = e(x) + 1, \quad \log(1 + x) = l(x)
$$

紧接着就是

$$
\log \exp x = x, \quad \exp \log(1 + x) = 1 + x
$$

对于$x$在$m$，从而命题。

#### 注 {#lie-ii-s6-n1-rem-1 .statement tag=0A62}

(1) 如果$x \in m, y \in m$和$x$和$y$通勤，则

$$
\exp(x + y) = \exp(x) \exp(y),
$$

因为族 $\left( \frac{x^i}{i!} \cdot \frac{y^j}{j!} \right)_{i,j \in \mathbf{N}}$ 是可求和的 (cf. *代数*, 章 IV, § 6, no. 9, 命题 11)。

(2) 由于级数、$e$和$l$没有常数项且$A_\alpha$是$A$、$\exp A_\alpha \subset 1 + A_\alpha$和$\log(1 + A_\alpha) \subset A_\alpha$从而$\exp A_\alpha = 1 + A_\alpha$和$\log(1 + A_\alpha) = A_\alpha$的闭理想$\alpha > 0$。

(3) 设$B$为完全Hausdorff过滤单位结合律代数和$n = \bigcup_{\alpha > 0} B_\alpha$。令$f$是$A$到$B$的连续单位同态，使得$f(m) \subset n$。然后$f(\exp x) = \exp f(x)$对应$x \in m$，$f(\log y) = \log f(y)$对应$y \in 1 + m$；我们显示例其中第一个公式：

$$
f(\exp x) = \sum_{n \geq 0} f(x^n)/n! = \sum_{n \geq 0} f(x)^n/n! = \exp f(x).
$$

(4) 设E为单位结合词代数。如果a是E的幂零元，则族$\left( \frac{a^n}{n!} \right)_{n \in \mathbf{N}}$有有限支撑，我们写成$\exp a = \sum_{n \geq 0} a^n / n!$。如果 $b - 1$ 幂零的，则元素 b 是单能的；然后我们写

$$
\log b = \sum_{n \geq 1} (-1)^{n-1} (b - 1)^n / n.
$$

我们从关系$e(l(X)) = l(e(X)) = X$推出映射$a \mapsto \exp a$是E的幂零元的集合的双射到E的单能元素的集合，并且$b \mapsto \log b$是逆映射。

### 2.豪斯多夫群

设X为集合。我们使用记号或§ 5，没有。 1 和 2. 自由的李代数 L(X) 被识别为 A(X) 中的典范像 (§ 3, no. 1, 定理 1)。我们用$\hat{L}(X)$表示$\hat{A}(X)$中L(X)的闭包，即形式$a = \sum_{n \geq 1} a_n$的$\hat{A}(X)$的元素的集合，使得$a_n \in L^n(X)$对于所有$n \geq 0$；这是过滤了$\hat{A}(X)$的谎言子代数。

#### 定理 1 {#lie-ii-s6-thm-1 .statement tag=0A63}

*$\hat{A}(X)$到$\hat{L}(X)$的指数映射的限制是$\hat{L}(X)$的双射到马格努斯群$\Gamma(X)$的闭子群。*

我们写$A(X) = A, A^n(X) = A^n, \hat{A}(X) = \hat{A}, L^n(X) = L^n, \hat{L}(X) = \hat{L}, \Gamma(X) = \Gamma$。令 B 为代数 $A \otimes A$，型 $\mathbf{N}$ 的分级由 $B^n = \sum_{i+j=n} A^i \otimes A^j$ 定义。令 $\hat{B} = \prod_{n \geq 0} B^n$ 为关联的完整过滤代数 (*交换代数*, 章 III, § 2, no. 12, *例* 1)。 § 3, no. 1中定义的余积$c : A \to A \otimes A$，推论1到定理1的等级为次数0，因此扩展通过连续性到同态$\hat{c} : \hat{A} \to \hat{B}$给出：

$$
\hat{c}\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} c(a_n) \quad \text{for } a_n \in A^n.
$$

我们还将定义连续同态$\delta'$和$\hat{A}$的$\delta''$转化为$\hat{B}$

$$
\delta'\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (a_n \otimes 1), \qquad \delta''\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (1 \otimes a_n) \quad \text{for } a_n \in A^n.
$$

根据推论2到§ 3, no. 1的定理1，$L^n$是$a_n \in A^n$的集合，使得$c(a_n) = a_n \otimes 1 + 1 \otimes a_n$。由此可见，$\hat{L}$ 是 $a \in \hat{A}$ 的集合，使得

$$
\hat{c}(a) = \delta'(a) + \delta''(a).
$$

令$\Delta$为等于1的常数项的$b \in \hat{A}$和满足关系的集合

$$
\hat{c}(b) = \delta'(b) \cdot \delta''(b),
$$

在$b = \sum_{n \geq 0} b_n$的其他字、集合中，使得$b_n \in \mathbf{A}^n$适用于所有$n \geq 0$，$b_0 = 1$和$c(b_n) = \sum_{i+j=n} b_i \otimes b_j$适用于$n \geq 0$。后者刻画表明$\Delta$是$\Gamma$的闭子集；因为$\hat{\epsilon}$、$\delta'$和$\delta''$是环同态，并且$\delta'(\hat{\mathbf{A}})$中的每个元素与$\delta''(\hat{\mathbf{A}})$、限制中的每个元素通勤到映射$c$中的$\Gamma$和$\delta'\delta''$是群同态并且$\Delta$是$\Gamma$中的子群。

By Proposition 1 of no. 1, the exponential mapping of $\hat{\mathbf{A}}$ is a bijection of the set $\hat{\mathbf{A}}^+$ of elements of $\hat{\mathbf{A}}$ with no constant term onto $\Gamma$. 设$a \in \hat{\mathbf{A}}^+$和$b = \exp a$。 由于$\hat{\epsilon}$是连续的环同态，

$$
\hat{\epsilon}(b) = \hat{\epsilon}\left( \sum_{n \geq 0} a^n/n! \right) = \sum_{n \geq 0} \hat{\epsilon}(a)^n/n! = \exp \hat{\epsilon}(a).
$$

The relations

$$
\delta'(b) = \exp \delta'(a), \quad \delta''(b) = \exp \delta''(a)
$$

类似地被证明，并且由于 $\delta'(a)$ 与 $\delta''(a)$ (no. 1, 注 1) 通勤，

$$
\delta'(b) \delta''(b) = \exp (\delta'(a) + \delta''(a)).
$$

因此$a$满足(3)当且仅当$b$满足(4)，这就证明了定理。

#### 注 {#lie-ii-s6-n2-rem-1 .statement tag=0A64}

上述证明表明，$\exp(\hat{\mathbf{L}})$是$b$满足(4)的$\Gamma$由……组成中的子群$\Delta$。

因此，$\Delta$的群运算可以通过指数映射传输到$\hat{\mathbf{L}}$。在其他字中，$\hat{\mathbf{L}}$是一个完全拓扑群，律为合成$(a, b) \mapsto a \mathbin{\mathbf{h}} b$，由下式给出

$$
a \mathbin{\mathbf{h}} b = \log(\exp a \cdot \exp b).
$$

由此获得的拓扑群称为*Hausdorff群*（源自相对于K的X）。

令$g$为群$F = F(X)$进入$\Gamma$的同态，使得$g(x) = \exp x$代表$x \in X$。由于$\exp x - 1 - x = \sum_{n \geq 2} x^n/n!$是阶$\geq 2$，$g$是§ 5, no. 3的定理1单射。因此*映射$\log \circ g$是$F$的单同态进入Hausdorff群，其中扩展典范嵌入$X \to \hat{\mathbf{L}}$*。

对于每个整数$m \geq 1$，我们用$\hat{\mathbf{L}}$中阶$\geq m$的元素的$\hat{\mathbf{L}}_m$集合和$u \in \Gamma$的$\Gamma_m$集合表示，这样$u - 1$是阶$\geq m$。然后$\hat{\mathbf{L}}_m = \exp(\Gamma_m)$乘注2 / no. 1；由于 $(\Gamma_m)_{m \geq 1}$ 是$\Gamma$ (§ 4, no. 5 命题 2) 上的整体式中央过滤，$(\hat{\mathbf{L}}_m)_{m \geq 1}$ *是群 $\hat{\mathbf{L}}$* 上的整体式中央过滤。

### 3. 正式谎言幂级数

#### 引理 1 {#lie-ii-s6-lem-1 .statement tag=0A65}

*设$\mathfrak{g}$为过滤后的李代数（§ 4, no. 1），$(\mathfrak{g}_\alpha)_{\alpha \in \mathbf{R}}$为过滤后的$\alpha \in \mathbf{R}$。 设 P 是不定式 $(\Gamma_i)_{i \in I}$ (§ 2, no. 4) 中次数 n 的齐次李多项式。 Then $P((a_i)) \in \mathfrak{g}_{n\alpha}$ for every family $(a_i)_{i \in I}$ of elements of $\mathfrak{g}_\alpha$*.

次数 $n \geqslant 2$ 的每个李多项式都是形式 $[Q, R]$ 的项的有限和，其中 $Q$ 和 $R$ 分别是次数 $< n$ 和和次数等于$n$（§ 2, no. 7，命题7）。 引理随后是$n$ 上的归纳。

A *谎言形式幂级数*† （系数在 $K$ 中）*在不定式中* $(T_i)_{i \in I}$ 是李代数 $\hat{L}((T_i)_{i \in I}) = \hat{L}(I)$ 中的任何元素。这样的元素$u$可以唯一地写成可和族$(u_\nu)_{\nu \in \mathbf{N}^{(I)}}$的和，其中$u_\nu \in L^\nu(I)$。

假设 $I$ 是*有限*。令 $g$ 为完整的 Hausdorff 过滤李代数，使得 $g = \bigcup_{\alpha > 0} g_\alpha$；让$t = (t_i)_{i \in I}$成为元素和$g$的一个家庭。

#### 命题 2 {#lie-ii-s6-prop-2 .statement tag=0A66}

*同态* $f_t : L(I) \to g$ *使得* $f_t(T_i) = t_i$ (§ 2, no. 4) *可以通过连续性扩展到一个且仅一个连续的同态* $\hat{f}_t$ *的* $\hat{L}(I)$ *到* $g$。

存在$\alpha > 0$，使得$t_i \in g_\alpha$对于所有$i \in I$；因此$f_t(L^\nu(I)) \subset g_{|\nu| \wedge \alpha}$对于所有$\nu$（引理 1），这意味着$\hat{f}_t$的连续性。

如果$u \in \hat{L}(I)$，我们写$u((t_i)) = \hat{f}_t(u)$。特别是取$g = \hat{L}(I)$、$u = u((T_i))$；一般情况下，$u((t_i))$称为李形式幂级数$u((T_i))$中用$t_i$代替$T_i$的结果。如果$u = \sum_{\nu \in \mathbf{N}^{(I)}} u_\nu$，其中$u_\nu \in L^\nu(X)$，族$(u_\nu((t_i)))_{\nu \in \mathbf{N}^{(I)}}$是可求和的，并且
$$
u((t_i)) = \sum_{\nu \in \mathbf{N}^{I}} u_\nu((t_i)).
$$

令 $\sigma$ 为 $g$ 的连续同态到完整的 Hausdorff 过滤李代数 $g'$，使得 $g' = \bigcup_{\alpha > 0} g'_\alpha$。对于每个*有限*家庭$t = (t_i)_{i \in I}$/元素/$g$以及所有$u \in \hat{L}(I)$，
$$
\sigma(u((t_i))) = u((\sigma(t_i))),
$$
对于同态 $\sigma \circ \hat{f}_t$ 是连续的，对于$i \in I$，映射 $T_i$ 到 $\sigma(t_i)$。

令$u = (u_j)_{j \in J}$是$\hat{L}(I)$的元素的*有限*族，并令$v \in \hat{L}(J)$；将$v$中的$u_j$替换为$T_j$，我们得到$\hat{L}(I)$的元素$w = v((u_j)_{j \in J})$，用$v \circ u$表示。然后
$$
w((t_i)_{i \in I}) = v((u_j((t_i)_{i \in I}))_{j \in J})
$$
对于$g$的元素的每个“有限”族$t = (t_i)_{i \in I}$，正如通过在方程$w = v((u_j)_{j \in J})$上使用连续的同态$\hat{f}_t$操作可以看到的。

设$u = \sum_{\nu \in \mathbf{N}^{I}} u_\nu \in \hat{L}(I)$，其中$u_\nu \in L^\nu(I)$。 $g^I$到$g$的映射$\tilde{u}$$(t_i) \mapsto u((t_i))$是*连续的*：对于每个开集合$g_\alpha$和$\alpha > 0$$\tilde{u}_\alpha$的族是一致可求的，并且足以证明每个$\tilde{u}_\nu$ 是连续的，即 $|\nu|$ 上的直接的乘归纳。

† 谎言形式幂级数一般不是 *代数*、章 IV, § 6 意义上的形式幂级数。

### 4. 豪斯多夫级数

令 {U, V} 为集合和两个元素。

#### 定义 1 {#lie-ii-s6-def-1 .statement tag=0A67}

*元素* $H = U \circledast V = \log(\exp U \cdot \exp V)$ (no. 2) *李代数* $\hat{L}_\mathbf{Q}(\{U, V\})$ *被称为不定式* U * 和* V 中的 Hausdorff 级数。

我们用$H_n$（或$H_{r,s}$）表示总次数 n（或$(r, s)$）中H的齐次分量。然后

$$
H = \sum_{n \geq 0} H_n = \sum_{r, s \geq 0} H_{r,s}, \quad H_n = \sum_{r+s=n \atop r, s \geq 0} H_{r,s}.
$$

#### 定理 2 {#lie-ii-s6-thm-2 .statement tag=0A68}

*如果 r 和 s 是两个正整数，使得* $r + s \geq 1$，*则* $H_{r,s} = H'_{r,s} + H''_{r,s}$，*其中*

$$
(r + s)H'_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s-1 \\ 1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} (V)
$$

$$
(r + s)H''_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) (U).
$$

在$\hat{A}_\mathbf{Q}(\{U, V\})$，$\exp U \cdot \exp V = 1 + W$，其中$W = \sum_{r+s \geq 1} \frac{U^r V^s}{r! s!}$，从而

$$
H = \sum_{m \geq 1} (-1)^{m-1} W^m / m \text{ (no. 2)}, \text{ that is:}
$$

$$
H_{r,s} = \sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_m + s_m \geq 1}}
\prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!}.
$$

线性映射 $P_n$，由$\{U, V\}$中的$n \geq 1$和$x_1, \ldots, x_n$的$P_n(x_1, \ldots, x_n) = \frac{1}{n} \left( \prod_{i=1}^{n-1} (\mathrm{ad}\, x_i) \right)(x_n)$定义，是$A^n_\mathbf{Q}(\{U, V\})$到$L^n_\mathbf{Q}(\{U, V\})$的投影算子（§ 3, no. 2，命题的推论） 1）；如 $H_{r,s}$ 属于至 $L^{r+s}_\mathbf{Q}(\{U, V\})$、$H_{r,s} = P_{r+s}(H_{r,s})$。现在

$$
P_{r+s} \left( \prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!} \right)
= \frac{1}{r+s} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} \frac{(\mathrm{ad}\, V)^{s_{m-1}}}{s_{m-1}!} (V)
$$

当 $s_m \geqslant 1$ 且

$$
(13)\quad P_{r+s}\left(\prod_{i=1}^{m} \frac{U r_i}{r_i!} \frac{V s_i}{s_i!}\right) = \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m-1}}{r_m!} \right)(U)
$$

当$r_m \geqslant 1$和$s_m = 0$时。此外，如果$p \geqslant 2$和$(\mathrm{ad}\ t)^0.t = t$，显然$(\mathrm{ad}\ t)^{p-1}.t = 0$。由此可见，当$s_m \geqslant 2$时，(12)的两侧为零，而当$r_m \geqslant 2$时，(13)的两侧为零。因为$H'_{r,s}$是型(12)的项和并且$H''_{r,s}$是型(13)的项和，所以定理跟随。

#### 注 {#lie-ii-s6-n4-rem-1 .statement tag=0A69}

(1) 我们将$A(X)$的(§ 3, no. 2,注)投影算子$Q$定义到$L(X)$上，使得$Q(a^m) = 0$适用于$a \in L(X)$和$m \geqslant 2$和$Q(1) = 0$。然后立即$H = Q(\exp H) = Q(\exp U.\exp V)$，从而

$$
(14)\quad H_{r,s} = Q \left( \frac{U^r V^s}{r! s!} \right) \quad \text{for } r + s \geqslant 1.
$$

(2) 我们有

$$
(15)\quad H(U, V) \equiv U + V + \frac{1}{2}[U, V] + \frac{1}{12}[U, [U, V]] \\
+ \frac{1}{12}[V, [V, U]] - \frac{1}{24}[U, [V, [U, V]]]
$$
右 $\sum_{n \geqslant 5} L^n(\{U, V\})$ 取模。

(3) 每整数 $n \neq 1$、从而 $H_{0,n} = H_{n,0} = 0$

$$
(16)\quad H(U, 0) = H(0, U) = U.
$$

另一方面，如 $[U, -U] = 0$，

$$
(17)\quad H(U, -U) = 0.
$$

### 5. 代换在豪斯多夫级数

由于 $K$ 是域包含 $\mathbf{Q}$，因此 Hausdorff 级数可以被视为李形式幂级数，系数为 $K$。因此，如果$g$是用$g = \bigcup_{\alpha > 0} g_\alpha$进行完整Hausdorff过滤的李代数，则$g$中的$a, b$，$a$和$b$可以替代$H$中的$U$和$V$ （cf.no. 3和§ 2, no. 5、注）。

特别地，令 $A$ 为完整的豪斯多夫过滤单位联想代数。我们将$\alpha \in \mathbf{R}$写为$m = \bigcup_{\alpha > 0} A_\alpha$和$m_\alpha = A_\alpha \cap m$；因此$m_\alpha = A_\alpha$对应$\alpha > 0$，$m_\alpha = m$对应$\alpha \leqslant 0$。加上括号$[a, b] = ab - ba$，$m$是完整的Hausdorff滤波李代数，可以应用上面的内容。有了这个记号，我们就得到了以下结果，它完成了no. 1的命题 1。

#### 命题 3 {#lie-ii-s6-prop-3 .statement tag=0A6A}

*如果$a \in m, b \in m$，则$\exp H(a, b) = \exp a . \exp b$。*

设$a, b$在$m$中；存在$\alpha > 0$使得$a \in A_\alpha$和$b \in A_\alpha$。那么存在 Magnus 代数 $\hat{A}(\{U, V\})$ 到 $A$ 映射 $U$ 到 $a$ 和 $V$ 到 $b$ 的连续同态 $\theta$ (§ 5, no. 1， 命题1)。

$\theta$至$\hat{L}(\{U, V\})$的限制是$L(\{U, V\})$的李代数到$m$的连续同态，其中映射$U$（分别为$V$）至$a$ （分别$b$）。通过no. 3的公式(6)，因此$\theta(H) = H(a, b)$。然后将连续的同态$\theta$应用到关系的两侧即可
$$
\exp H(U, V) = \exp U . \exp V
$$
考虑到 no. 1 的 *注 3*。

#### 注 1 {#lie-ii-s6-n5-rem-1 .statement tag=0A6B}

如果 $a$ 和 $b$ 可交换，则 $H_{r,s}(a, b) = 0$ 对于 $r + s \geq 2$，对于次数 $\geq 2$ 的每个齐次李多项式在 $(a, b)$ 处都是零。然后$H(a, b) = a + b$和命题3恢复公式
$$
\exp(a + b) = \exp a . \exp b.
$$

#### 命题 4 {#lie-ii-s6-prop-4 .statement tag=0A6C}

*令$g$为完整的Hausdorff过滤李代数，使得$g = \bigcup_{\alpha > 0} g_\alpha$。 映射$(a, b) \mapsto H(a, b)$是$g$上的群运算，与$g$上的拓扑兼容，其中$0$是单位元素，$-a$是所有$a \in g$的$a$的逆。*

$g \times g$到$g$的映射$(a, b) \mapsto H(a, b)$是连续的（no. 3）；由于映射$a \mapsto -a$显然是连续的，因此只需证明关系即可
$$
\begin{align*}
(18) \quad & H(H(a, b), c) = H(a, H(b, c)) \\
(19) \quad & H(a, -a) = 0 \\
(20) \quad & H(a, 0) = H(0, a) = a
\end{align*}
$$
$g$ 中的 $a, b, c$。通过no. 3的公式(7)，当$a, b, c$是三个不定且$g = \hat{L}(\{a, b, c\})$时，足以证明这些公式。现在，指数映射到$\hat{L}(\{a, b, c\})$的限制是单射进入马格努斯代数$\hat{A}(\{a, b, c\})$，乘以命题3：
$$
\begin{align*}
\exp H(H(a, b), c) &= \exp H(a, b) . \exp c = \exp a . \exp b . \exp c \\
\exp H(a, H(b, c)) &= \exp a . \exp H(b, c) = \exp a . \exp b . \exp c \\
\exp H(a, -a) &= \exp a . \exp(-a) = \exp(a - a) = \exp 0 \\
\exp H(a, 0) &= \exp a . \exp 0 = \exp a \\
\exp H(0, a) &= \exp 0 . \exp a = \exp a.
\end{align*}
$$
这就建立了关系 (18) 到 (20)。

#### 注{#lie-ii-s6-n5-rem-2 .statement tag=0A6D}

(2) 取$g$为李代数$\hat{L}(X)$。上面介绍了群运算命题重合以及no. 2中定义的律。在其他字中，
$$
a \mathbin{\mathbf{h}} b = H(a, b) \quad \text{for } a, b \text{ in } \hat{L}(X);
$$
因此 Hausdorff 群运算由 Hausdorff 级数给出。

(3) 令 $g$ 为李代数，并由下中央级数定义积分过滤 ($\mathscr{C}^n g$)。假设存在$m \geq 1$使得$\mathscr{C}^m g = \{0\}$。 拓扑源自过滤$(\mathscr{C}^n g)_{n \geq 1}$，李代数$g$是Hausdorff，完整甚至离散。然后$P(a_1, \ldots, a_r) = 0$对于$g$中的$a_1, \ldots, a_r$以及次数$\geq m$的每个齐次李多项式$P$；特别是，$H_{r,s}(a, b) = 0$对于$r + s \geq m$和级数$H(a, b) = \sum_{r,s} H_{r,s}(a, b)$只有一个有限的数非零项。 $g$ 上的群运算 $(a, b) \mapsto H(a, b)$ 则为多项式映射 (§ 2, no. 4)。

#### 命题 5 {#lie-ii-s6-prop-5 .statement tag=0A6E}

*令$K_{r,s}$为多次$(r, s)$的$H(U + V, -U)$的分量。然后*
$$
K_{n,1}(U, V) = \frac{1}{(n+1)!} (\operatorname{ad} U)^n(V) \quad \text{for } n \geq 0.
$$

我们写$K(U, V) = H(U + V, -U)$，$K_1(U, V) = \sum_{n \geq 0} K_{n,1}(U, V)$。我们用 L（或 R）左（或右）乘法表示 $U$ 在 $\hat{A}(\{U, V\})$ 上。

我们可以写
$$
e^{U}V e^{-U} = \sum_{p, q} \frac{U^p}{p!} V \frac{(-U)^q}{q!}
= \sum_{n \geq 0} \frac{1}{n!} \left( \sum_{p+q=n} \frac{n!}{p!q!} (L^p(-R)^q) \cdot V \right)
= \sum_{n \geq 0} \frac{1}{n!} (L - R)^n V
$$
因此
$$
e^{U}V e^{-U} = \sum_{n \geq 0} \frac{1}{n!} (\operatorname{ad} U)^n V.
$$
我们现在对计算对 $A(\{U, V\})$ 的理想 $\sum_{m \geq 0} \sum_{n \geq 2} A^{m,n}(\{U, V\})$ 取模。对于所有$n \geq 1$，
$$
(U + V)^n \equiv U^n + \sum_{i=1}^{n-1} U^i V U^{n-1-i}
$$
从而
$$
(\operatorname{ad} U)(U + V)^n \equiv ((L - R) \sum_{i=1}^{n-1} L^i R^{n-i}) \cdot V \\
\equiv (L^n - R^n) \cdot V \\
\equiv U^n V - V U^n.
$$
因此
$$
(\operatorname{ad} U) \cdot e^{U+V} \equiv e^{U}V - V e^{U}
$$
总计超过$n$。

另一方面，$K_1(U, V) \equiv K(U, V)$和$e^{K_1(U, V)} \equiv 1 + K_1(U, V)$，因此
$$
K_1 \equiv e^K - 1 \equiv e^{U+V}e^{-U} - 1
$$
由命题 3. 我们推断
$$
\begin{align*}
(\mathrm{ad}\ U)K_1 &\equiv Ue^{U+V}e^{-U} - e^{U+V}e^{-U}U \\
&\equiv (e^{UV} - Ve^U)e^{-U} \quad \text{(by (23))} \\
&\equiv e^{UV}e^{-U} - V \\
&\equiv \sum_{n \geq 1} \frac{1}{n!} (\mathrm{ad}\ U)^n V \quad \text{(by (22))} \\
&\equiv (\mathrm{ad}\ U)\left( \sum_{n \geq 0} \frac{(\mathrm{ad}\ U)^n}{(n+1)!} V \right).
\end{align*}
$$
然后应用§ 2, no. 11的*注*就足够了。

### 习题 {#lie-ii-s6-exercises}

§ 6](exercises/s6/)参见[习题。
