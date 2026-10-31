---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 3
section_title: Rational fractions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.19-A IV.24, A IV.89-A IV.90
pdf_pages: 0028-0033, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Definition of rational fractions
      page: 19
      pdf_page: 28
    - "no": 2
      title: Degrees
      page: 20
      pdf_page: 29
    - "no": 3
      title: Substitutions
      page: 21
      pdf_page: 30
    - "no": 4
      title: Differentials and derivations
      page: 23
      pdf_page: 32
statements: 6
exercises: 7
content_sha256: 6de06227090e88dd4b9e0fa77da963aad41da27b51b46547aa81af120e9e50af
translated_from: content/en/alg/IV/03_s3_rational_fractions.md
translation_method: google
source_content_sha256: adebb07e34c4e82901da99d345bb6f746140b39d50f239de82732119ccaa1a31
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 539b55005f56f4445947fdd6a1bd57c4fbc1138de8845f6de407ec52b321795d
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 3。 有理分式

### 1. 定义 / 有理分式

#### 定义 1 {#alg-iv-s3-def-1 .statement tag=06BL}

*设 K 为交换域，I 集合。 整环$K[(X_i)_{i \in I}]$的分数(I，p. 116)的域用$K((X_i)_{i \in I})$或$K(X_i)_{i \in I}$表示。它的元素在不定式 $X_i$ 中称为有理分式，系数为 K。*

对于 $I = \{1, 2, \ldots, n\}$，我们写 $K(X_1, X_2, \ldots, X_n)$ 来代替 $K((X_i)_{i \in I})$。

设 A 为整环，K 为分数的域。 环 $A[(X_i)_{i \in I}]$ 可以等同于 $K[(X_i)_{i \in I}]$ 的子环，因此也等同于 $K((X_i)_{i \in I})$。对于每个$f \in K[(X_i)_{i \in I}]$，存在 A 的非零元素$\alpha$，使得$\alpha f \in A[(X_i)_{i \in I}]$。因此，$K((X_i)_{i \in I})$的每个元素都可以写成$u/v$，其中$u, v \in A[(X_i)_{i \in I}], v \neq 0$。因此，$K((X_i)_{i \in I})$可以被识别为域或分数或$A[(X_i)_{i \in I}]$。

现在设 K 为交换域，I 集合，J ⊂ I。设 B = K[(X_i)_{i ∈ J}]，则 K[(X_i)_{i ∈ I}] = B[(X_i)_{i ∈ I - J}]，由上可知，K((X_i)_{i ∈ I}) 可以标识为K'((X_i)_{i Î I - J})，其中 K' = K((X_i)_{i Î J})。

### 2.次数

设 K 为交换域。对于 K((X_i)_{i ∈ I}) 的每个元素 r，都存在 u, v ∈ K[(X_i)_{i ∈ I}]，使得 v ≠ 0 且 r = $\frac{u}{v}$。 关系$\frac{u}{v} = \frac{u_1}{v_1}$，其中v≠0，v_1≠0相当于uv_1=vu_1；如果 r ≠ 0，则 u ≠ 0 且 u_1 ≠ 0，因此 deg u + deg v_1 = deg v + deg u_1 (IV, p. 9)，或者 deg u − deg v = deg u_1 − deg v_1。因此，有理数整数 deg u − deg v 仅取决于 r；我们称之为次数，或者r的总次数，并用deg r表示。我们同意写 deg 0 = −∞。如果 J ⊂ I，我们同样可以关于指标 j ∈ J 的 X_j 定义次数。当 r 是多项式时，这些概念重合与 IV、p. 2 中定义的相同。

#### 命题 1 {#alg-iv-s3-prop-1 .statement tag=06BM}

— 设 r、s 为两个有理分式。

(i) 如果 deg r ≠ deg s，我们有

$$
r + s \neq 0 \quad \text{and} \quad \deg(r + s) = \sup(\deg r, \deg s)
$$

如果 deg r = deg s，则 deg(r + s) ≤ deg r。

(ii) 我们有 deg(rs) = deg r + deg s。

我们可以极限来解决 r 和 s 非零的情况。

让我们写 r = $\frac{u}{v}$, s = $\frac{w}{z}$，其中 u、v、w、z 是非零多项式。我们有 rs = $\frac{uw}{vz}$，所以

$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z =
= \deg r + \deg s.
$$

另一方面，我们有 r + s = $\frac{uz + vw}{vz}$。假设 deg r ≠ deg s，则字 deg u + deg z ≠ deg w + deg v。则 uz + vw ≠ 0，且

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&= \sup(\deg(uz), \deg(vw)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s).
\end{align*}
$$

假设 deg r = deg s，即 deg u + deg z = deg w + deg v。如果 r + s ≠ 0，则有

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r
\end{align*}
$$

\* 映射 r ↦ −deg r 因此是域 K((X_i)_{i ∈ I}) 的离散评估。 \*

### 3.代换

设 K 为交换域，E 为单位结合律 K-代数，$x = (x_i)_{i \in I}$ E 的成对可置换族元素。设所有非零 $v \in B$ 的 $B = K[(X_i)_{i \in I}]$ 和 $S_x$ 集合，使得 $v(x)$ 在 E 中可逆。 $u \in B,\ v \in S_x$和$f = \frac{u}{v} \in K((X_i)_{i \in I})$。 元素 $u(x)\ v(x)^{-1} = v(x)^{-1}u(x)$ 在 E 中定义；此外，如果 $u_1,\ v_1$ 是两个多项式，例如 $f = \frac{u_1}{v_1}$ 和 $v_1 \in S_x$，则 $uv_1 = vu_1$，因此 $u(x)v_1(x) = v(x)u_1(x)$ 等等
$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

让$f \in K((X_i)_{i \in I})$。如果存在*至少一对*$(u, v)$使得$f = \frac{u}{v}$和$v \in S_x$，我们可以说x在$f$中*可替代*；仅依赖于$f$和$x$的元素$u(x)\ v(x)^{-1}$则用$f(x)$或$f((x_i))$或$f((x_i)_{i \in I})$表示。

#### 命题 2 {#alg-iv-s3-prop-2 .statement tag=06BN}

*设 K 为交换域，E 为单位结合律 K-代数，$x = (x_i)_{i \in I}$ E 的成对可置换元素系列。$f \in K((X_i)_{i \in I})$ 的集合 $S_x^{-1}B$，使得 x 可在 $f$ 中替换为 K-子代数 $K((X_i)_{i \in I})$。 映射 $f \mapsto f(x)$ 是 $S_x^{-1}B$ 到 E 中的单位同态 $\varphi$。 像 $\varphi(S_x^{-1}B)$ 是所有 $yz^{-1}$ 的集合，其中 y 运行生成的 E 的单位子代数 $K[x]_E$由家庭 x 组成，其中 z 超过 $K[x]_E$ 的所有可逆元中的集合。

令$f_1 = \frac{u_1}{v_1},\ f_2 = \frac{u_2}{v_2}$为$K((X_i)_{i \in I})$的两个元素，使得$v_1,\ v_2 \in S_x$。我们有$f_1 + f_2 = \frac{u_1v_2 + u_2v_1}{v_1v_2},\ f_1f_2 = \frac{u_1u_2}{v_1v_2}$和$v_1,\ v_2 \in S_x$。因此 $S_x^{-1}B$ 是 $K((X_i)_{i \in I})$ 的 K-子代数。 命题的其余部分是清楚的。

#### 推论 {#alg-iv-s3-n3-cor-1 .statement tag=06BO}

*设L为L的交换域，K子域，L的$x = (x_i)_{i \in I}$L的元素，所有$f \in K((X_i)_{i \in I})$的$x_i$的M集合由……组成，U集合，使得x可以替换为将U的$f$和$\varphi$同态$f \mapsto f(x)$转化为L。那么$\varphi(U)$就是$KUM$生成的L的子域。*

令 L' 为 $KUM$ 生成的 L 的子域。我们有
$$
K \cup M \subset \varphi(U) \subset L'
$$
$\varphi(U)$ 是 L 的子环。现在，命题 2 意味着 $\varphi(U)$ 是 L 的子域，从而 $\varphi(U) = L'$。

令$f \in K((X_i)_{i \in I})$和$(g_i)_{i \in I}$是元素和$K((Y_l)_{l \in L})$的家庭。如果 (g_i) 在 f 中可替换，则 f((g_i)) 是 K((Y_l)_{l \in L}) 的元素。特别地，(X_i)_{i \in I} 可替换于 f 且 f = f((X_i)_{i \in I})。

#### 命题 3 {#alg-iv-s3-prop-3 .statement tag=06BP}

— 设 E 为 K 上的代数，它是结合律、交换律、单位且非零。令 f \in K((X_i)_{i \in I}) 并对于每个 i \in I，令 g_i \in K((Y_l)_{l \in L})。给定 E 的元素族 y = (y_l)_{l \in L} ，假设 y 可代入每个 g_i 并且 (g_i(y))_{i \in I} 可代入 f 。然后：
(i) (g_i)_{i \in I} 可代入 f 中；
(ii) 如果我们用 K((Y_l)_{l \in L}) 的 h 元素 f((g_i)) 表示，则 y 可在 h 中替换，且 h(y) = f((g_i(y)))。

我们可以认为 I 是有限的。通过假设，对于每个$i \in I$，$g_i$可以放入形式$p_i/q_i$，其中$p_i, q_i \in K[(Y_l)_{l \in L}]$和$q_i(y)$在E中可逆。同样，f可以写成$u/v$，其中$u, v \in K[(X_i)_{i \in I}]$和$v((g_i(y)))$是可逆的。设$m = \sup(\deg u, \deg v)$，并设$w = \prod_{i \in I} q_i \in K[(Y_l)_{l \in L}]$，$u_1 = u((g_i)) w^m$，$v_1 = v((g_i)) w^m$。多项式 u 是单项式 $\prod_{i \in I} X_i^{\nu_i}$ 的 K 线性组合，使得 $\sum_{i \in I} \nu_i \leq m$。我们有 $w^m \prod_{i \in I} g_i^{\nu_i} = w^m \left( \prod_{i \in I} p_i^{\nu_i} \right) \left( \prod_{i \in I} q_i^{\nu_i} \right)^{-1} \in K[(Y_l)_{l \in L}]$ x 选择米。因此$u_1 \in K[(Y_l)_{l \in L}]$，类似的$v_1 \in K[(Y_l)_{l \in L}]$。此外，$v_1(y) = (w(y))^m v((g_i(y)))$是可逆的。因此$v_1 \neq 0$，因为$E \neq 0$，所以$v((g_i)) \neq 0$。因此族$(g_i)$可以在f中替换。此外，我们还有$f((g_i)) = u_1/v_1$，因此y可以在$h = f((g_i))$和$h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y)))$中替换。

设 K 为交换域，E 为交换结合律且单位 K-代数，并令 f \in K((X_i)_{i \in I})。令 T_f 为 f 中可替换的所有 x = (x_i)_{i \in I} \in E^I 的集合。 映射 x \将 T_f 的 f(x) 映射到 E 称为与 f（和 E）相关的有理函数；我们有时用\tilde{f}表示它。如果 g \in K((X_i)_{i \in I}) 我们有 T_f \cap T_g \子集 T_{f+g}, T_f \cap T_g \子集 T_{fg}，因此与 f + g (resp. fg) 相关的有理数函数定义在 T_f \cap T_g 上并且具有相同的值在此集合上为 \tilde{f} + \tilde{g} （分别为 \tilde{f}\tilde{g}）。令 T'_f 为 T_f 中 x \的集合，使得 f(x) 可逆；如果 x \in T'_f，x 在 1/f 中是可替换的，并且与 1/f 相关的有理数函数取 x 值 f(x)^{-1}。

如果 K 是无穷大交换域，则 f \in K((X_i)_{i \in I})、g \in K((X_i)_{i \in I}) 和 \tilde{f}、\tilde{g} 是与 f、g（和 K）相关的有理数函数，并且如果对于所有 x \in 而言，\tilde{f}(x) = \tilde{g}(x) T_f \cap T_g 则 f = g。如果 f = u/v 且 g = u_1/v_1，其中 u、v、u_1、v_1 是多项式，则对于所有 x，我们有 u(x)v_1(x) = u_1(x)v(x)，使得 v(x)v_1(x) \neq 0，因此 uv_1 = u_1v (IV, p. 18, Th. 2)。因此映射 f \mapsto \tilde{f} 是单射的，我们经常会使用认同 f 和 \tilde{f}。

\* 使用 $K[(X_i)_{i \in I}]$ 的阶乘（Comm. Alg.、VII, § 3, No. 2 p. 502 和 Th. 2 p. 506 的 Cor.），可以轻松地显示以下内容：对于每个 $f \in K((X_i)_{i \in I})$ 都存在 $u, v \in K[(X_i)_{i \in I}]$，使得：
    1）$f = u/v$；
    2) 为了使$x \in K^I$可以被$f$替代，$v(x) \neq 0.$是充分必要的

### 4. 微分和推导

设$K$为交换域。根据III，p. 558，第5号提案，每推导$D$$K[(X_i)_{i \in I}]$扩展以独特的方式到推导$\bar{D}$$K((X_i)_{i \in I})$。如果$D, D'$是$K[(X_i)_{i \in I}]$的可置换推导，则括号$[D, D'] = DD' - D'D$是零，因此$[\bar{D}, \bar{D}']$是$K((X_i)_{i \in I})$的推导延伸$[D, D']$是零；在其他字、$D$和$D'$是可置换的。特别是$K((X_i)_{i \in I})$的推导$D_i$(IV，p. 6)扩展到推导再次由$D_i$表示并且是成对可置换的。如果$f \in K((X_i)_{i \in I}), D_i f$也写成$D_{x_i} f$或$\frac{\partial f}{\partial x_i}$或$f'_{x_i}$。当只有一个不确定的$X$时，可以使用记号$Df, \frac{df}{dX}, f'$。

让$B = K[(X_i)_{i \in I}], C = K((X_i)_{i \in I})$。作者：III，p. 574，第 23 号提案，典范映射

$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$

是同构个空间，共向量 $C$ 个空间。记住III，p. 570，我们看到向量$C$-空间$\Omega_K(C)$承认基家族$(dX_i)_{i \in I}$微分的$X_i$。令$\partial_i$为指标$i$在$\Omega_K(C)$上相对于基的坐标形式。那么$C$的映射$u \mapsto (\partial_i, du)$自身就是$C$的推导，其中对于$j \neq i$，映射$X_i$为1，$X_j$为0，因此等于$D_i$；在其他字中，我们有

$$
du = \sum_{i \in I} (D_i u) dX_i
$$

每$u \in C$。如果$I$是有限的，则$(D_i)_{i \in I}$是向量$C$的基-$C$的推导的空间。

#### 命题 4 {#alg-iv-s3-prop-4 .statement tag=06BQ}

— *令 $E$ 为结合律、可交换且单位的$K$代数，$x = (x_i)_{i, I}$为$E$和$f \in K((X_i)_{i, I})$的元素族。假设$x$可以替代$f$和$y = f(x)$。
(i) 对于$K((X_i)_{i, I})$中的每个推导$A$，其中映射$K[(X_i)_{i, I}]$自身，$x$可在$Af$中替换。
(ii) 对于 $E$ 中的每个推导 $D$ 到 $E$ 模块，我们有

$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

令$f = \frac{u}{v}$与$u, v \in K[(X_i)_{i \in I}]$和$v(x)$在E中可逆。令A为$K((X_i)_{i \in I})$映射$K[(X_i)_{i \in I}]$自身的推导。我们有
$$
\Delta f = \frac{(\Delta u)\ v - u(\Delta v)}{v^2}
$$
并且$v^2(x)$是可逆的，因此x可以在$Af$中替换。其次放入$r = u(x)$、$s = v(x)$；我们有 $y = s^{-1}r$，因此对于 E 的每个推导 D 到 E 模块，我们有
$$
\begin{align*}
Dy &= s^{-2}(s(Dr) - r(Ds)) \\
&= s^{-2}\left( s \sum_{i \in I} (D_iu)(x) \cdot Dx_i - r \sum_{i \in I} (D_iv)(x) \cdot Dx_i \right)
\end{align*}
$$
根据 IV 的第 4 号提案，p. 6。因此 $Dy = \sum_{i \in I} w_i \cdot Dx_i$ 与
$$
w_i = v(x)^{-2}(v(x)(D_iu)(x) - u(x)(D_iv)(x)) = (D_if)(x).
$$

### 习题 {#alg-iv-s3-exercises}

§ 3](exercises/s3/)参见[习题。
