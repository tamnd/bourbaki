---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 3
section_title: Tensor product of hilbertian spaces
lang: zh
source: evt-i-v
book_pages: TVS V.25-TVS V.37, TVS V.73-TVS V.74
pdf_pages: 0283-0295, 0331-0332
extraction: ocr
subsections:
    - "no": 1
      title: Tensor product of prehilbertian spaces
      page: 25
      pdf_page: 283
    - "no": 2
      title: Hilbertian tensor product of hilbertian spaces
      page: 28
      pdf_page: 286
    - "no": 3
      title: Symmetric hilbertian powers
      page: 29
      pdf_page: 287
    - "no": 4
      title: Exterior hilbertian powers
      page: 33
      pdf_page: 291
    - "no": 5
      title: Exterior multiplication
      page: 35
      pdf_page: 293
statements: 20
exercises: 2
content_sha256: e8c42e0b242523ea1b361b91788f8d132b05758bd36e012aa54976e5c3d290d4
translated_from: content/en/evt/V/03_s3_tensor_product_of_hilbertian_spaces.md
translation_method: google
source_content_sha256: 02cb54c6e38040afaaa4704bd9864f0e39ab141fc23dcd61afa7b042aa7a7e87
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 58615ec435dee82523f31c7e633bfdc68359bc99c9e220c8c188ee4be2d0659d
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。 张量积希尔伯特空间

### 1. 前希尔伯特张量积空间

令$E_1$和$E_2$为两个前希尔伯特空间，并令$F = E_1 \otimes E_2$为向量空间$E_1$和$E_2$的张量积。设$x_1 \in E_1$和$x_2 \in E_2$；由于从$E_1 \times E_2$到K的映射$(y_1, y_2) \mapsto \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle$是双线性的，因此在$E_1 \otimes E_2$上存在线性形式$\phi_{x_1, x_2}$使得
$$
\phi_{x_1, x_2}(y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
对于 $y_1 \in E_1$ 和 $y_2 \in E_2$。让$z \in F$。从$E_1 \times E_2$到K的映射$(x_1, x_2) \mapsto \overline{\phi_{x_1, x_2}(z)}$是双线性的；这可以通过在形式$z = \sum_{i=1}^n y_{i,1} \otimes y_{i,2}$中写$z$、$y_{i,1} \in E_1$和$y_{i,2} \in E_2$为$1 \leq i \leq n$来看到。那么$F = E_1 \otimes E_2$上存在线性形式$\psi_z$使得
$$
\psi_z(x_1 \otimes x_2) = \overline{\phi_{x_1, x_2}(z)} \quad (x_1 \in E_1, x_2 \in E_2).
$$
我们将$z, t$的$\Phi(z, t) = \psi_z(t)$放入F中。我们立即看到$\Phi$是$E_1 \otimes E_2$的倍半线性形式，其特征为
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
（cf.A，IX, § 1, No. 11）。

#### 命题 1 {#evt-v-s3-prop-1 .statement tag=080B}

— $E_1 \otimes E_2$ 上的倍半线性形式 $\Phi$ 为厄米特并且为正，因此将前希尔伯特空间的结构分配给 $E_1 \otimes E_2$。如果 $E_1$ 和 $E_2$ 是 Hausdorff，则该空间是 Hausdorff。

当 $z = x_1 \otimes x_2$ 和 $t = y_1 \otimes y_2$ 时，公式 $\Phi(z, t) = \overline{\Phi(t, z)}$ 由 (3) 得出。一般情况是通过线性获得的，因此$\Phi$是厄米特。

假设$E_1$和$E_2$是Hausdorff；我们将证明厄米特形式$\Phi$是正的且可分离的。令$z = \sum_{i=1}^n x_i \otimes y_i$为$F = E_1 \otimes E_2$的非零元素。令 $(e_1, ..., e_n)$ 为$E_1$ 的子空间的正交基，由$x_1, ..., x_n$ 生成（V，p. 23，cor. 1）。 $E_2$中存在元素$f_1, ..., f_m$，且不全为空，因此$z = \sum_{i=1}^n e_i \otimes f_i$，因此
$$
\Phi(z, z) = \sum_{i,j=1}^m \Phi(e_i \otimes f_i, e_j \otimes f_j)
$$
$$
= \sum_{i,j} \langle e_i | e_j \rangle \langle f_i | f_j \rangle = \sum_{i=1}^m \| f_i \|^2 > 0.
$$

对于一般情况，我们现在要证明 $\Phi$ 是正数。令$\tilde{E}_i$为与$E_i$相关的豪斯多夫前希尔伯特空间，并令$\pi_i$为从$E_i$到$\tilde{E}_i$（$i = 1, 2$）的典范映射。把$\pi = \pi_1 \otimes \pi_2$。令 $\tilde{\Phi}$ 为 $\tilde{E}_1 \otimes \tilde{E}_2$ 上的厄米特形式，其构造方式与 $\Phi$ 相同。我们有
$$
\Phi(z, t) = \Phi(\pi(z), \pi(t)) \quad (z \in F, \ t \in F),
$$
由于 $\tilde{\Phi}$ 为正，$\Phi$ 也为正。

前希尔伯特空间在道具中定义。 1 称为前希尔伯特空间* $E_1$ 和$E_2$ 的*张量积，写为$E_1 \otimes E_2$。从今以后，我们将把$\Phi(z, t)$写成$\langle z|t \rangle$，因此定义
$$
\langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle;
$$
我们还可以将 $\langle z|z \rangle^{1/2}$ 写为 $\|z\|_2$ 或 $\|z\|$。由(4)我们得到
$$
\|x_1 \otimes x_2\|_2 = \|x_1\| \cdot \|x_2\|,
$$
那么从$E_1 \times E_2$到$E_1 \otimes E_2$的双线性映射$(x_1, x_2) \mapsto x_1 \otimes x_2$是连续的。

对于$i = 1, 2$，令$F_i$为$E_i$的向量子空间，赋予诱发的前希尔伯特结构。那么$F_1 \otimes F_2$可以用$E_1 \otimes E_2$的向量子空间来识别（A，II, § 7, No. 7）。 公式 (4) 表明$F_1 \otimes F_2$ 与由$E_1 \otimes_2 E_2$ 诱发的前希尔伯特空间结构正好是$F_1 \otimes_2 F_2$。从今往后，我们将使用认同 $F_1 \otimes_2 F_2$ 以及 $E_1 \otimes_2 E_2$ 的前希尔伯特子空间。

#### 命题 2 {#evt-v-s3-prop-2 .statement tag=080C}

*对于$i = 1, 2$，令$E_i$和$F_i$为两个Hausdorff prehilbertian空间，并令$u_i \in \mathscr{L}(E_i; F_i)$。 线性映射 $u_1 \otimes u_2$ 从 $E_1 \otimes_2 E_2$ 到 $F_1 \otimes_2 F_2$ 是连续的，我们有*
$$
\|u_1 \otimes u_2\| = \|u_1\| \cdot \|u_2\|.
$$

考虑 $E_1$ 上的正厄米特形式由下式给出
$$
f(x_1, y_1) = \|u_1\|^2 \langle x_1 | y_1 \rangle - \langle u_1(x_1) | u_1(y_1) \rangle.
$$

通过道具。 1 (V, p. 25)，$E_1 \otimes E_2$ 上存在*正* 厄米特形式 $\Phi$，使得
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = f(x_1, y_1) \langle x_2 | y_2 \rangle =
$$
$$
= \|u_1\|^2 \langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle - \langle (u_1 \otimes 1)(x_1 \otimes x_2) | (u_1 \otimes 1)(y_1 \otimes y_2) \rangle
$$
对于$E_1$中的$x_1, y_1$和$E_2$中的$x_2, y_2$。根据线性我们有
$$
\Phi(z, t) = \|u_1\|^2 \langle z|t \rangle - \langle (u_1 \otimes 1)(z) | (u_1 \otimes 1)(t) \rangle
$$
$E_1 \otimes E_2$ 中的 $z, t$。由于$\Phi$为正，我们得到$\Phi(z, z) \geq 0$，即$\|(u_1 \otimes 1).z\|_2$

$$
\leq \|u_1\| \cdot \|z\|_2 \text{ for } z \in E_1 \otimes_2 E_2, \text{ or } \|u_1 \otimes 1\| \leq \|u_1\|. \text{ Similarly we prove the inequality } \|1 \otimes u_2\| \leq \|u_2\|, \text{ and since } u_1 \otimes u_2 = (u_1 \otimes 1) \circ (1 \otimes u_2), \text{ we get}
$$
$$
\|u_1 \otimes u_2\| \leq \|u_1\| \cdot \|u_2\|.
$$
另一方面，
$$
\|u_1\| \cdot \|u_2\| = \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|u_1(x_1)\| \cdot \|u_2(x_2)\|
$$
$$
= \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|(u_1 \otimes u_2)(x_1 \otimes x_2)\|_2 \leq \|u_1 \otimes u_2\|.
$$
这样就完成了道具的证明。 2.Q.E.D.

令 $E_1, ..., E_n$ 为前希尔伯特空间 ($n \geq 2$)。我们定义张量积$E_1 \otimes_2 ... \otimes_2 E_n$（也表示为$\bigotimes_{i=1}^n E_i$）归纳，
$$
E_1 \otimes_2 ... \otimes_2 E_n = (E_1 \otimes_2 ... \otimes_2 E_{n-1}) \otimes_2 E_n.
$$
因此，通过标量乘积的定义，我们有
$$
\langle x_1 \otimes ... \otimes x_n | y_1 \otimes ... \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle,
$$
特别是$^1$
$$
\|x_1 \otimes ... \otimes x_n\|_2 = \|x_1\| \cdots \|x_n\|,
$$
$E_i$ ($1 \leq i \leq n$) 中的 $x_i, y_i$。如果$E_i$是豪斯多夫，那么$E_1 \otimes_2 ... \otimes_2 E_n$也是豪斯多夫。

令$F_1, ..., F_n$为前希尔伯特空间，$u_i \in \mathscr{L}(E_i; F_i)$为$1 \leq i \leq n$。由归纳于$n$，道具。 2 意味着 $u_1 \otimes ... \otimes u_n$ 是从 $E_1 \otimes_2 ... \otimes_2 E_n$ 到 $F_1 \otimes_2 ... \otimes_2 F_n$ 的连续线性映射并且
$$
\|u_1 \otimes ... \otimes u_n\| = \|u_1\| \cdots \|u_n\|.
$$
设$\sigma \in S_n$为集合$\{1, 2, ..., n\}$中的置换。由于(6)，线性映射$p_\sigma$从$E_1 \otimes_2 ... \otimes_2 E_n$到$E_{\sigma^{-1}(1)} \otimes_2 ... \otimes_2 E_{\sigma^{-1}(n)}$，其特征为
$$
p_\sigma(x_1 \otimes ... \otimes x_n) = x_{\sigma^{-1}(1)} \otimes ... \otimes x_{\sigma^{-1}(n)}
$$
是前希尔伯特空间同构（“交换律 of 张量积”）。

同样，将 $\{1, 2, ..., n\}$ 的划分考虑为 $m$ 连续间隔 $I_1, ..., I_n$，将 $I_k = [a_k, a_{k+1} - 1]$ 视为 $1 \leq k \leq m$。放
$$
F_k = \bigotimes_{i=a_k}^{a_{k+1}-1} E_i \quad (1 \leq k \leq m).
$$

$^1$ 这里我们再次将 $\|z\|_2 = \langle z|z \rangle^{1/2}$ 对应于 $z$ 放入 $E_1 \otimes_2 ... \otimes_2 E_n$ 中。

典范同构从 $F_1 \otimes ... \otimes F_m$ 到 $E_1 \otimes ... \otimes E_n$，其中变换 $\bigotimes_{k=1}^{m} \bigotimes_{i=a_k}^{a_{k+1}-1} x_i$ 到 $x_1 \otimes ... \otimes x_n$ (A, II, § 3, No. 9) 是前希尔伯特空间同构 (结合性 of 张量积) »）。

### 2. 希尔伯特空间的希尔伯特张量积

#### 定义 1 {#evt-v-s3-def-1 .statement tag=080D}

令 $E_1, ..., E_n$ 为希尔伯特空间。 *豪斯多夫前希尔伯特空间* $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$的完成被称为*$E_i$的希尔伯特张量积，并用$E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$（或$\hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i$）表示。

令$F_1, ..., F_n$为希尔伯特空间，$u_i \in \mathscr{L}(E_i, F_i)$为$1 \leq i \leq n$。连续的线性映射$u_1 \otimes ... \otimes u_n$，然后扩展到连续的线性映射$u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$，从$E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$到$F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n$。我们有

$$
\|u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n\| = \|u_1\| ... \|u_n\|
$$

由公式 (8) 共 V、p. 27。此外，如果 $1_E$ 表示任何希尔伯特空间 $E$ 的恒等映射，我们有

$$
1_{E_1} \hat{\otimes}_2 ... \hat{\otimes}_2 1_{E_n} = 1_E \quad \text{with} \quad E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n .
$$

最后，如果$G_1, ..., G_n$是希尔伯特空间并且$v_i \in \mathscr{L}(F_i; G_i)$对于$1 \leq i \leq n$，我们得到

$$
(v_1 \circ u_1) \hat{\otimes}_2 ... \hat{\otimes}_2 (v_n \circ u_n) = (v_1 \hat{\otimes}_2 ... \hat{\otimes}_2 v_n) \circ (u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n) .
$$

我们将制定希尔伯特张量积的“交换律”和“结合性”的任务留给读者，与上面针对前希尔伯特空间所说的类似。

#### 注 {#evt-v-s3-n2-rem-1 .statement tag=080E}

令 $E_1, ..., E_n$ 为豪斯多夫前希尔伯特空间，$\hat{E}_1, ..., \hat{E}_n$ 为它们各自的完成。那么$E_1 \otimes_2 ... \otimes_2 E_n$是$\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$的前希尔伯特子空间。由于映射$(x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n$从$\hat{E}_1 \times ... \times \hat{E}_n$到$\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$是连续的，$E_1 \otimes_2 ... \otimes_2 E_n$在$\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$是稠密的。 *更不必说*$E_1 \otimes_2 ... \otimes_2 E_n$的补全正是希尔伯特空间$\hat{E}_1 \hat{\otimes}_2 ... \hat{\otimes}_2 \hat{E}_n$。这个完成度是有时，简单地写成$E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$（或$\hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i$）。

#### 命题 3 {#evt-v-s3-prop-3 .statement tag=080F}

令 $E_1, ..., E_n$ 为希尔伯特空间。假设$1 \leq i \leq n$空间$E_i$是封闭向量子空间的族$(E_{i,\alpha})_{\alpha \in A(i)}$的希尔伯特和。那么$E_1 \otimes_2 ... \otimes_2 E_n$是子空间$E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$族的希尔伯特和，$(\alpha_1, ..., \alpha_n)$范围超过$A(1) \times ... \times A(n)$。

由V的公式(6)、p. 27、$E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$的子空间$E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$相互正交。对于 1 到 $n$ 之间的每个整数 $i$，集合 $\bigcup_{\alpha \in A(i)} E_{i,\alpha}$ 总计在 $E_i$ 中，并且多线性映射 $(x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n$ 是连续的。

由此可见子空间 $E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$ 的并是总计，因此成立。 3.

#### 推论 1 {#evt-v-s3-prop-3-cor-1 .statement tag=080G}

— 对于 $1 \leq i \leq n$，令 $(e_{i,\alpha})_{\alpha \in A(i)}$ 为 $E_i$ 的正交基。那么当$(\alpha_1, \ldots, \alpha_n)$范围超过$A(1) \times \cdots \times A(n)$时，向量$e_{1,\alpha_1} \otimes \ldots \otimes e_{n,\alpha_n}$族是$E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$的正交基。

#### 推论 2 {#evt-v-s3-prop-3-cor-2 .statement tag=080H}

— 令 $E_1$ 和 $E_2$ 为两个希尔伯特空间，且 $(e_i)_{i \in I}$ 为 $E_1$ 的正交基。令$(y_i)_{i \in I}$是$E_2$的元素的族，使得$\sum_{i \in I} \| y_i \| ^2 < + \infty$。那么族$(e_i \otimes y_i)_{i \in I}$可在$E_1 \hat{\otimes}_2 E_2$中求和；此外，$E_1 \otimes E_2$的每个元素都可以用$\sum_{i \in I} \| y_i \| ^2 < + \infty$唯一地写成形式$\sum_{i \in I} e_i \otimes y_i$。

令 $F_i$ 为 $E_1$ 中由 $e_i$ ($i \in I$) 生成的线。那么$E_1$就是子空间$(F_i)_{i \in I}$族的希尔伯特和。通过道具。 3、空间$E_1 \hat{\otimes}_2 E_2$是子空间$(F_i \hat{\otimes}_2 E_2)_{i \in I}$族的希尔伯特和，因此cor。 2如下。

#### 例 1 {#evt-v-s3-n2-exa-1 .statement tag=080I}

由科。 1、空间$\ell^2(I) \hat{\otimes}_2 \ell^2(J)$与$\ell^2(I \times J)$自然同构，$x = (x_i)_{i \in I}$和$y = (y_j)_{j \in J}$的张量积$x \otimes y$可以与$(x_i y_j)_{i \in I, j \in J}$族识别。同样，通过cor。 2、$\ell^2(I) \hat{\otimes}_2 E$可以与$\ell^2_E(I)$等价，这样在希尔伯特空间$E$中，每一个$y$就有$(x_i)_{i \in I} \otimes y = (x_i y)_{i \in I}$。

#### 例 2 {#evt-v-s3-n2-exa-2 .statement tag=080J}

\* 令$X$为Hausdorff拓扑空间，且$\mu$为$X$的正测度。令 $E$ 为希尔伯特空间。我们以规范的方式将可以确定$L^2(X, \mu) \hat{\otimes}_2 E$与$L^2_E(X, \mu)$进行计算：如果$f$是$X$上平方可积标量函数$f$的类，并且如果$a$ 属于到 $E$，则 $f \otimes a$ 是函数 $x \mapsto f(x).a$ 中的类，值位于 $E$ 中。

令$Y$为Hausdorff拓扑空间，且$\nu$为$Y$的正测度。以类似的方式，我们可以确定希尔伯特空间$L^2(X, \mu) \hat{\otimes}_2 L^2(Y, \nu)$和$L^2(X \times Y, \mu \otimes \nu)$；那么$f \otimes g$可以在$X \times Y$上与函数$(x, y) \mapsto f(x)g(y)$的类进行识别。 \*

### 3. 对称希尔伯特幂

令$E$为希尔伯特空间，令$n$为正整数。让$\hat{T}^n(E)$或$E^{\hat{\otimes} n}$表示$n$希尔伯特空间的张量积，每个都等于$E$。在其他字中，$\hat{T}^n(E)$ 是 Hausdorff prehilbertian 空间结构定义的空间 $T^n(E) = E \otimes \ldots \otimes E$ ($n$ 因子) 的完成

$$
\langle x_1 \otimes \ldots \otimes x_n | y_1 \otimes \ldots \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle .
$$

如果$(e_i)_{i \in I}$是$E$的正交基，$I$中$i_1, \ldots, i_n$的向量$e_{i_1} \otimes \ldots \otimes e_{i_n}$族，是$\hat{T}^n(E)$的正交基（V， p. 29，cor。我们得到$\hat{T}^\circ(E) = K$。

设$\sigma \in S_n$为集合$\{ 1, 2, \ldots, n \}$中的置换。由V，p. 27，存在$\hat{T}^n(E)$的自同构$p_\sigma$，其特征为

$$
p_\sigma(x_1 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)} .
$$

我们在$\mathfrak{S}_n$中对$\sigma, \tau$有$p_{\sigma \tau} = p_{\sigma} p_{\tau}$，因此向量空间$\hat{\mathbf{T}}^n(E)$的自同态$\Pi_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} p_{\sigma}$是由$\mathfrak{S}_n$保持不变的所有元素的子空间的正射投影。然而 (A, III, § 6, No. 3), $\Pi_n$ 映射张量积 $\mathbf{T}^n(E)$ 到阶 $n$ 的所有对称张量的子空间 $\mathbf{TS}^n(E)$。在其他字中，$\Pi_n$的像是空间$\mathbf{TS}^n(E)$的完成，赋予$\mathbf{T}^n(E)$的标量乘积；该完成将用 $\widetilde{\mathbf{TS}}^n(E)$ 表示。

令$\mathbf{S}^n(E)$为向量空间$E$的第$n$对称幂（A，III, § 6, No. 1）。 典范映射从$\mathbf{T}^n(E)$到$\mathbf{S}^n(E)$定义，由限制同构$\lambda_n$从$\mathbf{TS}^n(E)$到$\mathbf{S}^n(E)$。我们立即验证逆同构由下式给出

$$
\mu_n(x_1 \ldots x_n) = \Pi_n(x_1 \otimes \ldots \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

$E$ 中的 $x_1, \ldots, x_n$。

我们将 $\mathbf{S}^n(E)$ 定义一个豪斯多夫前希尔伯特空间结构放入

$$
\langle u|v \rangle = n! \langle \mu_n(u)|\mu_n(v) \rangle .
$$

然后我们有（与 A 的公式 (29) 比较，III, § 11, No. 5）

$$
\langle x_1 \ldots x_n|y_1 \ldots y_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \prod_{i=1}^n \langle x_i|y_{\sigma(i)} \rangle ,
$$

特别是

$$
\langle x^n|y^n \rangle = n! \langle x|y \rangle^n .
$$

让$\hat{\mathbf{S}}^n(E)$表示前希尔伯特空间$\mathbf{S}^n(E)$的完成，以及$\hat{\mathbf{S}}(E)$希尔伯特空间$\hat{\mathbf{S}}^n(E)$的外部希尔伯特和。我们可以证明 (V, p. 73, 练习.1) 代数 $\mathbf{S}(E)$ 不能中的乘法通过连续性扩展到$\mathbf{S}(E)$, 除非 $E$ 只是 0。

#### 命题 4 {#evt-v-s3-prop-4 .statement tag=080K}

*令 $(e_i)_{i \in I}$ 为希尔伯特空间 $E$ 的正交基。对于$\mathbf{N}^{(I)}$中的每个$\alpha$，输入*

$$
z_{\alpha} = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2} .
$$

*那么 $(z_{\alpha})_{\alpha \in \mathbf{N}^{(I)}}$ 是 $\hat{\mathbf{S}}(E)$ 的正交基。*

令$E_0$为由向量$e_i$生成的$E$的向量子空间，$i$范围超过$I$。然后是向量空间$\mathbf{S}(E_0)$（A，III, § 6, No. 6）的$z_{\alpha}$形式基。但$E_0$在$E$是稠密的，并且从$E \times \cdots \times E$到$\mathbf{S}(E)$的多线性映射$(x_1, \ldots, x_n) \mapsto x_1 \ldots x_n$对于所有$n \geqslant 1$都是连续的；因此$\mathbf{S}(E_0)$在$\mathbf{S}(E)$中是稠密的。现在足以证明$z_\alpha$族是正交的。首先观察$\hat{S}^n(E)$ 和$\hat{S}^m(E)$ 对于$n \neq m$ 是正交的。因此证明公式就足够了

$$
\langle z_\alpha | z_\beta \rangle = \left\{ \begin{array}{ll}
1 & \text{if } \alpha = \beta \\
0 & \text{if } \alpha \neq \beta
\end{array} \right.
$$

当$|\alpha| = \sum_{i \in I} \alpha_i$和$|\beta| = \sum_{i \in I} \beta_i$等于相同的整数$n$时。

考虑集合$\{ 1, 2, ..., n \}$中的划分$(P_i)_{i \in I}$，使得卡$P_i = \alpha_i$适用于所有$i \in I$。如果 $k$ 属于等于 $P_i$，则放入 $x_k = e_i$，然后放入 $x_1 ... x_n = \prod_{i \in I} e_i^{\alpha_i}$。同样，我们定义$(Q_i)_{i \in I}$和$y_k$以这样的方式卡片$Q_i = \beta_i$和$y_1 ... y_n = \prod_{i \in I} e_i^{\beta_i}$。由于$e_i$相互正交，因此我们有$\langle x_k | y_{\sigma(k)} \rangle = 0$，除非存在索引$i \in I$使得$k \in P_i$和$\sigma(k) \in Q_i$。到公式 (15)，我们就有$\langle x_1 ... x_n | y_1 ... y_n \rangle = 0$除非，存在置换$\sigma \in \mathfrak{S}_n$，使得$\sigma(P_i) = Q_i$对于所有$i \in I$，这意味着$\alpha = \beta$。然后$\langle z_\alpha | z_\beta \rangle = 0$换$\alpha \neq \beta$。同样的论证证明$\| x_1 ... x_n \| ^2$等于$\sigma \in \mathfrak{S}_n$的数，使得$\sigma(P_i) = P_i$对于所有$i \in I$，因此等于$\prod_{i \in I} \alpha_i !$。我们得到$\| z_\alpha \| = 1$，并且命题被证明。

#### 推论 {#evt-v-s3-n3-cor-1 .statement tag=080L}

— *Suppose that the hilbertian 空间 E is 直和 of the orthogonal 子空间 M and N. 典范同构 g from $S(M) \otimes S(N)$ onto $S(E)$ (A, III, § 6, No. 6) 扩展 uniquely to a hilbertian 空间从$\hat{S}(M) \hat{\otimes}_2 \hat{S}(N)$到$\hat{S}(E)$需要同构小时。

Let $(e_i)_{i \in I}$ (resp. $(f_j)_{j \in J}$) be an orthonormal 基 of the hilbertian 空间 M (resp. N) and let $M_0$ (resp. $N_0$) be 向量子空间 of E generated by 向量 $e_i$（分别为$f_j$）。将$E_0 = M_0 + N_0$放入$g_0$，从$S(M_0) \otimes S(N_0)$到$S(E_0)$为典范同构。放

$$
z_\alpha = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2}, \quad t_\beta = \prod_{j \in J} f_j^{\beta_j}/(\beta_j!)^{1/2}
$$

对于 $\alpha \in \mathbf{N}^{(I)}$ 和 $\beta \in \mathbf{N}^{(J)}$。通过道具。 4，我们因此定义了$\hat{S}(M)$的正交基$(z_\alpha)_{\alpha \in \mathbf{N}^{(I)}}$，$\hat{S}(N)$的$(t_\beta)_{\beta \in \mathbf{N}^{(J)}}$和$\hat{S}(E)$的$(z_\alpha t_\beta)_{\alpha \in \mathbf{N}^{(I)}, \beta \in \mathbf{N}^{(J)}}$。 Since we have $z_\alpha t_\beta = g_0(z_\alpha \otimes t_\beta)$, and since 元素 $z_\alpha \otimes t_\beta$ 形式 an orthonormal 基 of $\hat{S}(M) \hat{\otimes}_2 \hat{S}(N)$ (V, p. 29, cor. 1), we see that $g_0$ 扩展 to a希尔伯特空间同构$h : \hat{S}(M) \hat{\otimes}_2 \hat{S}(N) \to \hat{S}(E)$。 By 构造, we have

$$
h(x_1 ... x_m \otimes y_1 ... y_n) = x_1 ... x_m y_1 ... y_n
$$

对于$M_0$中的所有向量$x_1, ..., x_m$和$N_0$中的$y_1, ..., y_n$。根据连续性，同样的关系也适用于M中的向量$x_1, ..., x_n$和N中的向量$y_1, ..., y_n$；其他字、$h$扩展$g$。 $h$的唯一性清晰。

令 E 和 F 为两个希尔伯特空间和 $u \in \mathscr{L}(E; F)$。从 $\hat{T}^n(E)$ 到 $\hat{T}^n(F)$ 的线性映射 $\hat{T}^n(u) = u \hat{\otimes}_2 ... \hat{\otimes}_2 u$ ($n$ 因子) 与范数 $\|u\|^n$ (V, p. 28, 公式 (10)) 连续。 Moreover, 公式 (13) and (14) of V, p. 30, show that there exists 同构 $\phi_{n,E}$ from $\hat{S}^n(E)$ onto 子空间 $\widehat{T S^n}(E)$ of $\hat{T}^n(E)$, and only one, such that

$$
(18) \quad \phi_{n,E}(x_1 \ldots x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)} \quad (x_1, ..., x_n \text{ in } E) .
$$

因此，存在从$\hat{S}^n(E)$到$\hat{S}^n(F)$连续的线性映射$\hat{S}^n(u)$，并且只有一个使得下面的图表可交换

$$
\begin{array}{ccc}
\hat{S}^n(E) & \xrightarrow{\phi_{n,E}} & \hat{T}^n(E) \\
\downarrow \hat{S}^n(u) & & \downarrow \hat{T}^n(u) \\
\hat{S}^n(F) & \xrightarrow{\phi_{n,F}} & \hat{T}^n(F)
\end{array}
$$

We now prove 公式

$$
(19) \qquad \| \hat{S}^n(u) \| = \| u \|^{n} .
$$

我们显然有$\| \hat{S}^n(u) \| \leq \| \hat{T}^n(u) \| = \| u \|^{n}$。此外，对于所有$x \in E$，我们有$\hat{S}^n(u)(x^n) = u(x)^n, \| x^n \| = (n!)^{1/2} \| x \|^{n}$和$\| u(x)^n \| = (n!)^{1/2} \| u(x) \|^{n}$，这给出

$$
\| \hat{S}^n(u) \| \cdot \| x \|^{n} \geq \| u(x) \|^{n} ;
$$

紧接着是 $\| \hat{S}^n(u) \| \geq \| u \|^{n}$，因此是公式 (19)。

很明显我们有公式

$$
(20) \qquad \hat{S}^n(1_E) = 1_{\hat{S}_n(E)}
$$
$$
(21) \qquad \hat{S}^n(v \circ u) = \hat{S}^n(v) \circ \hat{S}^n(u) \quad \text{for} \quad v \in \mathscr{L}(F ; G) .
$$

最后，$S^n(E)$上的$\hat{S}^n(u)$重合，以及A中定义的线性映射$S^n(u) : S^n(E) \to S^n(F)$，III, § 6, No. 2，因为对于$E$中的每个$x_1, ..., x_n$，变换$x_1 ... x_n$进入$u(x_1) ... u(x_n)$。

#### 例 1 {#evt-v-s3-n3-exa-1 .statement tag=080M}

令$d \geq 1$为整数，$\omega$为$\mathbf{R}^d$上的正函数，可相对于勒贝格测度$\mu$局部可积。令$E$为希尔伯特空间$L^2(\mathbf{R}^d, \omega.\mu)$，并令$S = S(E)$。然后$S$可以用所有序列$f = (f_n)_{n \geq 0}$中的空间来识别，其中每个$f_n$是$(\mathbf{R}^d)^n$上的函数，可以相对于勒贝格测度$\mu \otimes ... \otimes \mu$（$n$）进行测量因子）和$(\mathbf{R}^d)^n$中$n$因子的置换下的*不变*，并且是这样的

$$
(22) \qquad \| f \|^{2} = \sum_{n=0}^{\infty} n! \int_{\mathbf{R}^d} ... \int_{\mathbf{R}^d} |f_n(x_1, ..., x_n)|^2 \omega(x_1) ... \omega(x_n) dx_1 ... dx_n
$$

是有限的。 $S$中的范数$\| f \|$由公式(22)定义。上面定义的希尔伯特空间$S$被称为*权*$\omega$的*对称Fock空间*相应的。

#### 例 2 {#evt-v-s3-n3-exa-2 .statement tag=080N}

令$X$为豪斯多夫拓扑空间，$\mu$为$X$上范数1的正测度，$E$为真实希尔伯特空间$L^2_{\mathbf{R}}(X, \mu)$的希尔伯特子空间。如果满足以下等效的条件，我们就说 $E$ 是 *高斯空间* ：

a) 对于所有 $f \in E$，我们有 $\int_X e^{i f} d\mu = \exp(-\| f \|^{2}/2) ;$

b) 对于所有 $f \in E$ 和范数 1，$f$ 下的度量 $\mu$ 的像是度量
$$
(2\pi)^{-1/2}\ e^{-x^2/2} dx .
$$
$\mathbf{R}$。

*假设$E$是高斯空间。*令$f_1, ..., f_n$为函数，其类$f_i$属于到$E$。我们定义函数：$f_1 ... f_n$：X（称为$f_1, ..., f_n$的《Wick’s 乘积》）由公式
$$
(23)\quad :f_1 ... f_n: = \sum_{0 \leq 2p \leq n} (-1)^p \sum_{\sigma \in I_p} \prod_{i=1}^p \langle f_{\sigma(2i-1)}|f_{\sigma(2i)} \rangle \prod_{j=2p+1}^n f_{\sigma(j)},
$$
其中 $I_p$ 是置换 $\sigma$ $\{1, 2, ..., n\}$ 的集合，这样我们有
$$
\begin{align*}
&\sigma(1) < \sigma(2), ..., \sigma(2p-1) < \sigma(2p) \\
&\sigma(1) < \sigma(3) < ... < \sigma(2p-1) \\
&\sigma(2p+1) < \sigma(2p+2) < ... < \sigma(n).
\end{align*}
$$

然后存在一个*同构* $\phi$ *从* $\hat{S}(E)$ *到* $L^2_R(X, \mu)$的希尔伯特子空间，其中$f_1, ..., f_n$的变换乘积$f_1 ... f_n$，在$\hat{S}(E)$中计算， $(:f_1 ... f_n:)$。假设X是苏斯林空间，并且存在函数的可数族$(f_n)$，其类属于到E并且将点与X分开。那么$\phi$就是从$\hat{S}(E)$到$L^2_R(X, \mu)$的同构。 \*

### 4. 外部希尔伯特幂

令 E 为希尔伯特空间和 $n$ 正整数。对于每个置换$\sigma \in \mathfrak{S}_n$，让$\varepsilon_\sigma$表示其签名；将$a_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma p_\sigma$放入$\mathscr{L}(\hat{T}^n(E))$（V，p. 29）。

$a_n$是正射投影仪，直接的，其像$\overline{\mathbf{A}'_n}(E)$是阶$n$的所有反对称张量在空间$\mathbf{A}'_n(E)$在$\hat{T}^n(E)$的闭包（A， III, § 7, No. 4）。从$\Lambda^n(E)$到$\mathbf{A}'_n(E)$存在同构$\pi_n$，其特征为
$$
(24)\quad \pi_n(x_1 \wedge ... \wedge x_n) = a_n(x_1 \otimes ... \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)}
$$
对于E中的$x_1, ..., x_n$。我们现在可以通过将定义一个豪斯多夫前希尔伯特空间结构放在$\Lambda^n(E)$上
$$
(25)\quad \langle u|v \rangle = n!\langle \pi_n(u)|\pi_n(v) \rangle .
$$
更明确地说，我们有（与 A 的公式 (30)，III, § 11, No. 5 进行比较）。
$$
(26)\quad \langle x_1 \wedge ... \wedge x_n|y_1 \wedge ... \wedge y_n \rangle = \det(\langle x_i|y_j' \rangle)
$$
对于 E 中的所有 $x_1, ..., x_n$ 和 $y_1, ..., y_n$。

令$\hat{\Lambda}^n(E)$表示前希尔伯特空间$\Lambda^n(E)$的完成，$\hat{\Lambda}(E)$表示希尔伯特空间$\hat{\Lambda}^n(E)$的外部希尔伯特和。

#### 例 {#evt-v-s3-n4-exa-1 .statement tag=080O}

— *用V、p. 32的例 1 记号，我们可测量所有序列$(f_n)_{n \geq 0}$的可以确定希尔伯空间$\hat{\Lambda}(E)$和集合函数，其中（22）中定义的*数$\|f\|$是有限的，并且其中每个函数$f_n$是*反对称*，即满足关系

$$
f_n(x_{\sigma(1)}, ..., x_{\sigma(n)}) = \varepsilon_\sigma f_n(x_1, ..., x_n)
$$

每置换 $\sigma \in \mathfrak{S}_n$。希尔伯特空间 $\hat{\Lambda}(E)$ 被称为 *权* $\omega$ 的 *反对称 Fock 空间* 相应的。 \*

#### 命题 5 {#evt-v-s3-prop-5 .statement tag=080P}

*让* $(e_i)_{i \in I}$ *成为希尔伯特空间* E 的正交基。*赋予* I *具有全序结构。那么所有元素* $e_{i_1} \wedge ... \wedge e_{i_n}$ *对于* $i_1 < ... < i_n$ *的集合是* $\hat{\Lambda}^n(E)$ 的正交基。

我们知道（A，III, § 7, No. 8）元素涉及向量空间$\Lambda^n(E_0)$的形式基，其中$E_0$是由向量$e_i$生成的E的向量子空间。进一步地，对于$i_1 < ... < i_n$，标量乘积$\langle e_{i_k}|e_{i_l} \rangle$的矩阵是阶n的单位矩阵；由(26)，我们有$\|e_{i_1} \wedge ... \wedge e_{i_n}\| = 1$。最后，如果 $(i_1, ..., i_n)$ 和 $(j_1, ..., j_n)$ 是两个不同的，I 元素严格递增的序列，则存在与 $i_1, ..., i_n$ 不同的元素 $j_\ell$，因此对于 $1 \leq k \leq n$，我们有 $\langle e_{i_k}|e_{j_\ell} \rangle = 0$，并通过 (26)，$\langle e_{i_1} \wedge ... \wedge e_{i_n}|e_{j_1} \wedge ... \wedge e_{j_n} \rangle = 0$。在其他字中，元素$e_{i_1} \wedge ... \wedge e_{i_n}$族，对于$i_1 < ... < i_n$来说，是正交的。

但$E_0$在E中是稠密的，并且映射$(x_1, ..., x_n) \mapsto x_1 \wedge ... \wedge x_n$从$E \times \cdots \times E$到$\Lambda^n(E)$是连续的。因而，$\Lambda^n(E_0)$在$\Lambda^n(E)$中是稠密的，命题5紧随其后。

#### 推论{#evt-v-s3-n4-cor-1 .statement tag=080Q}

*假设希尔伯特空间* E *是两个正交子空间* M *和* N的直和。 *典范同构* g *从* $\Lambda(M) \otimes \Lambda(N)$ *到* $\Lambda(E)$ *(A, III, § 7, No. 7)* *扩展以独特的方式实现希尔伯特空间同构从*$\hat{\Lambda}(M) \hat{\otimes}_2 \hat{\Lambda}(N)$*到*$\hat{\Lambda}(E)$。

证明类似于 prop 的推论。 4（V，p. 31）。

令 E 和 F 为两个希尔伯特空间和 $u \in \mathscr{L}(E; F)$。我们将证明，在对称幂 $\hat{S}^n(E)$ (V, p. 32) 的情况下，线性映射 $\hat{\Lambda}^n(u)$ 从 $\hat{\Lambda}^n(E)$ 到 $\hat{\Lambda}^n(F)$ (A, III, § 7, No. 4) 扩展到连续的线性映射 $\hat{\Lambda}^n(u)$从$\hat{\Lambda}^n(E)$变为$\hat{\Lambda}^n(F)$。 We have 关系

$$
\hat{\Lambda}^n(1_E) = 1_{\hat{\Lambda}^n(E)} , \tag{27}
$$
$$
\hat{\Lambda}^n(v \circ u) = \hat{\Lambda}^n(v) \circ \hat{\Lambda}^n(u) \quad \text{if } v \text{ belongs to } \mathscr{L}(F; G) , \tag{28}
$$
$$
\|\hat{\Lambda}^n(u)\| \leq \|u\|^n . \tag{29}
$$

一般来说，公式 (29) (TS, IV, § 6) 中没有等式。 最后，我们有从$\hat{\Lambda}^n(E)$到$\hat{T}^n(E)$的子空间$\overline{\mathbf{A}}'_n(E)$定义的同构$\psi_n = \psi_{n,E}$

$$
\psi_n(x_1 \wedge ... \wedge x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)} . \tag{30}
$$

### 5. 外观乘法

Let E be a hilbertian 空间. For every 整数 $n \geqslant 0$, let $\theta_n$ be 典范映射 from $T^n(E)$ onto $\Lambda^n(E)$;然后

$$
\theta_n(x_1 \otimes \ldots \otimes x_n) = x_1 \wedge \ldots \wedge x_n
$$

对于E中的$x_1, \ldots, x_n$。令$p$和$q$为两个正整数；由于公式 (30) 和 (31) 我们有

$$
u \wedge v = \theta_{p+q}\left( \frac{1}{(p!)^{1/2}} \psi_p(u) \otimes \frac{1}{(q!)^{1/2}} \psi_q(v) \right)
$$

对于 $u \in \Lambda^p(E)$ 和 $v \in \Lambda^q(E)$。从$\| \theta_n \| \leq (n!)^{1/2}$开始，我们得到不等式

$$
\| u \wedge v \| \leq \left( \frac{(p+q)!}{p! \ q!} \right)^{1/2} \| u \| \cdot \| v \|
$$

对于 $u \in \Lambda^p(E)$ 和 $v \in \Lambda^q(E)$。因而，映射$(u, v) \mapsto u \wedge v$扩展通过从$\hat{\Lambda}^p(E) \times \hat{\Lambda}^q(E)$到$\hat{\Lambda}^{p+q}(E)$连续到双线性映射，范数至多等于$\left( \frac{(p+q)!}{p! \ q!} \right)^{1/2}$（cf.V，p. 73，执行。 2）。 We again denote this by $(u, v) \mapsto u \wedge v$.

#### 命题 6 {#evt-v-s3-prop-6 .statement tag=080R}

*设 E 为希尔伯特空间。我们有*

$$
\| x \wedge u \| \leq \| x \| \cdot \| u \|
$$

*for* $x \in E$ *and* $u \in \hat{\Lambda}(E)$.

考虑$\| x \| = 1$的情况显然就足够了。

令 F 为所有与 x 正交的向量的 E 由……组成的希尔伯特子空间。由于 E 是 F 和线 K.x 的希尔伯特和，因此从 V、p. 34 的推论可以得出，映射 $(v, w) \mapsto v + x \wedge w$ 是从 $\hat{\Lambda}(F) \oplus \hat{\Lambda}(F)$ 到 $\hat{\Lambda}(E)$ 的希尔伯特空间同构。如果$u = v + x \wedge w$和$v, w$在$\hat{\Lambda}(F)$中，我们有$x \wedge u = x \wedge v$，因此有$\| x \wedge u \| = \| v \| \leq (\| v \|^2 + \| w \|^2)^{1/2} = \| u \|$。

#### 推论 1 {#evt-v-s3-prop-6-cor-1 .statement tag=080S}

*a)* *设* $x_1, \ldots, x_n$ *为希尔伯特空间* E 的元素。 *我们有*

$$
\| x_1 \wedge \ldots \wedge x_n \| \leq \| x_1 \| \ldots \| x_n \|,
$$

*其中，仅当* $x_i$ * 之一为空，或者序列* $(x_1, \ldots, x_n)$ * 正交时，等式才成立。*

*b)* *设* $x_1, \ldots, x_n, y_1, \ldots, y_n$ *为希尔伯特空间* E 的元素。 *我们有*

$$
|\det(\langle x_i, y_j \rangle)| \leq \| x_1 \| \ldots \| x_n \| \cdot \| y_1 \| \ldots \| y_n \|;
$$

如果向量 $x_i$ 和 $y_i$ 非空； 等式在(36)中成立当且仅当$(x_1, ..., x_n)$和$(y_1, ..., y_n)$各自是E的相同向量子空间的正交基。

不等式 (35) 由命题得出。 6 by 归纳 on $n$; 不等式(36)可以通过V、p. 33的$\Lambda^n(E)$和公式(26)中的应用柯西-施瓦茨不等式推出。

假设序列 $(x_1, ..., x_n)$ 是正交的。然后

$$
\| x_1 \wedge ... \wedge x_n \|^2 = \det(\langle x_i | x_j \rangle) = \prod_{i=1}^n \| x_i \|^2
$$

从$\langle x_i | x_j \rangle = 0$开始$i \neq j$。

现在假设向量 $x_1, ..., x_n$ 不为空，并且形式不是正交的序列。由于$\| x_1 \wedge ... \wedge x_n \|$对称地依赖于向量$x_1, ..., x_n$，我们可以假设$x_1$与$x_2, ..., x_n$生成的E的子空间F不正交，并且F不只是0。我们可以将$x_1$分解为形式 $x'_1 + y$，其中 $y \neq 0$ 在 F 中，且 $x'_1$ 与 F 正交；然后$\| x'_1 \| < \| x_1 \|$。但是

$$
x_1 \wedge x_2 \wedge ... \wedge x_n = x'_1 \wedge x_2 \wedge ... \wedge x_n,
$$

等等

$$
\begin{align*}
\| x_1 \wedge ... \wedge x_n \| &\leq \| x'_1 \| \| x_2 \| ... \| x_n \| \\
&< \| x_1 \| \| x_2 \| ... \| x_n \|.
\end{align*}
$$

假设向量 $x_i$ 和向量 $y_i$ 不为空。 关系(36)中的等式等价于等式中的合取

(37) $$ |\langle x_1 \wedge ... \wedge x_n | y_1 \wedge ... \wedge y_n \rangle| = \| x_1 \wedge ... \wedge x_n \| \cdot \| y_1 \wedge ... \wedge y_n \| $$

(38) $$ \| x_1 \wedge ... \wedge x_n \| = \| x_1 \| ... \| x_n \| , \quad \| y_1 \wedge ... \wedge y_n \| = \| y_1 \| ... \| y_n \| . $$

通过证明的第一个部分，等式（38）意味着序列、$(x_1, ..., x_n)$和$(y_1, ..., y_n)$都是正交的，这又意味着$x_1 \wedge ... \wedge x_n \neq 0$和$y_1 \wedge ... \wedge y_n \neq 0$。在这些条件，关系（37）下意味着存在一个标量$\lambda \neq 0$，使得$y_1 \wedge ... \wedge y_n = \lambda x_1 \wedge ... \wedge x_n$（V，p. 3，注1）；在其他字中，$(x_1, ..., x_n)$和$(y_1, ..., y_n)$是E（A，III, § 11, No. 13）的相同向量子空间的基。

#### 推论 2 {#evt-v-s3-prop-6-cor-2 .statement tag=080T}

— 设 $(a_{ij})_{1 \leq i,j \leq n}$ 为厄米特矩阵，复数为元素，行列式为 D。假设不等式

$$
\sum_{i,j=1}^n a_{ij} \overline{z}_i z_j \geq 0
$$

对于所有复数 $z_1, ..., z_n$ 都成立。然后

$$
0 \leq D \leq a_{11} ... a_{nn}.
$$

假设 D 非空； 等式$D = a_{11} ... a_{nn}$成立当且仅当$a_{ij} = 0$对于所有$i \neq j$成立。

令 $\Phi$ 为向量空间 $\mathbf{C}^n$ 上的厄米特形式，由下式给出

$$
\Phi(\mathbf{z}, \mathbf{z}') = \sum_{i,j=1}^n a_{ij} \overline{z}_i z'_j
$$

对于$\mathbf{C}^n$中的$\mathbf{z} = (z_1, ..., z_n)$和$\mathbf{z}' = (z'_1, ..., z'_n)$。到假设时，$\Phi$为正。

首先假设$\Phi$是分离的，即D非空。如果$(e_1, ..., e_n)$是$\mathbf{C}^n$的典范基，我们有$\Phi(e_i, e_j) = a_{ij}$，并且cor。 2 紧随 cor.2 之后。 1, a) 通过放入 $x_i = e_i$。

从 $a_{ii} = \Phi(e_i, e_i) \geq 0$ 开始，如果 $D = 0$，我们还有不等式 (40)。

#### 推论 3（《哈达玛不等式》）{#evt-v-s3-prop-6-cor-3 .statement tag=080U}

— 设 $(a_{ij})_{1 \leq i, j \leq n}$ 为矩阵，且具有复数元素，且行列式为 D。

$$
c_i = \left( \sum_{j=1}^n |a_{ij}|^2 \right)^{1/2} \quad \text{for} \quad 1 \leq i \leq n,
$$

和$m = \sup_{i,j} |a_{ij}|$。然后我们有

$$
|D| \leq c_1 ... c_n \leq m^n \cdot n^{n/2}.
$$

如果$D \neq 0$，在阶中$|D| = c_1 ... c_n$，矩阵$(a_{ij})_{1 \leq i, j \leq n}$的行$y_i = (a_{ij})_{1 \leq j \leq n}$是二乘二正交的向量是必要且充分的。

让空间 $\mathbf{C}^n$ 被分配一个标量乘积定义为

$$
\langle \mathbf{z}|\mathbf{z}' \rangle = \sum_{i=1}^n \overline{z}_i z'_i.
$$

令$(\mathbf{x}_1, ..., \mathbf{x}_n)$为$\mathbf{C}^n$和$\mathbf{y}_i$向量的典范基，其中$a_{ij}$为$1 \leq j \leq n$。 $1 \leq i \leq n$我们有$\| \mathbf{x}_i \| = 1$和$\| \mathbf{y}_i \| = c_i$；还有$\langle \mathbf{x}_i|\mathbf{y}_j \rangle = a_{ji}$。 不等式$|D| \leq c_1 ... c_n$和等式的条件则为V、p. 35的特例。 1. 显然我们有$c_i \leq m \cdot n^{1/2}$，因此有$c_1 ... c_n \leq m^n \cdot n^{n/2}$。

### 习题 {#evt-v-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
