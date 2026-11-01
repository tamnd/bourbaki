---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 3
section_title: Exponential invariants
lang: zh
source: lie-iv-vi
pdf_pages: 0207-0213, 0254-0254
extraction: ocr
subsections:
    - "no": 1
      title: GROUP ALGEBRA OF A FREE ABELIAN GROUP
      page: 0
      pdf_page: 207
    - "no": 2
      title: CASE OF THE GROUP OF WEIGHTS; MAXIMAL TERMS
      page: 0
      pdf_page: 208
    - "no": 3
      title: ANTI-INvariant ELEMENTS
      page: 0
      pdf_page: 209
    - "no": 4
      title: INVARIANT ELEMENTS
      page: 0
      pdf_page: 212
statements: 13
exercises: 2
content_sha256: 9d2b634d95a3695a57324bde45f7eaa142dac150c6f3af0343473002021737a0
translated_from: content/en/lie/VI/03_s3_exponential_invariants.md
translation_method: google
source_content_sha256: b9746d131eb1272ab4f94dead490215a8154be0c1a153b0693388de4edd688ad
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 67ebc9c29c95ec56d630cbcfec2cafa2f865123e947cc88b50940621778e516f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。指数不变量

在这个截面中，字母A表示交换环，与单位元，并没有减少到0。

### 1. 群代数免费阿贝尔的群

设 P 为有限秩 $l$ 的自由 $\mathbf{Z}$ 模。我们用 A 上 P 的加法群的 $A[P]$ 群代数表示（*代数*，第 III, § 2, no. 6）。对于任何$p \in P$，用$A[P]$的$e^p$相应的元素表示。那么$(e^p)_{p \in P}$是A-模$A[P]$的*基*，并且对于任何$p, p' \in P$，我们有
$$
e^p e^{p'} = e^{p + p'}, \quad (e^p)^{-1} = e^{-p}, \quad e^0 = 1.
$$

#### 引理 1 {#lie-vi-s3-lem-1 .statement tag=0AXN}

*假设 A 是阶乘*（*交换代数*，第 VII, § 3, no. 1 章，定义 1）。
(i) *环 $A[P]$ 是阶乘。*
(ii) *如果$u, v$与P不成比例元素，则$A[P]$的元素$1 - e^u, 1 - e^v$互质。*

令 $(p_1, p_2, \ldots, p_l)$ 为 P 的基，且 $X_1, X_2, \ldots, X_l$ 为不定数。从$A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$到$A[P]$需要$X_1^{n_1} X_2^{n_2} \ldots X_l^{n_l}$（其中$n_1, n_2, \ldots, n_l \in \mathbf{Z}$）到$e^{n_1 p_1 + \cdots + n_l p_l}$的A线性映射是环的同构。现在$A[X_1, \ldots, X_l]$是阶乘环（*交换代数*，第VII, § 3, no. 5章），而$A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$是$A[X_1, \ldots, X_l]$的分数的环，因此也是阶乘。

令$P'$（或$P''$）为P 的元素的集合，其中一些倍数、属于至$\mathbf{Z}u + \mathbf{Z}v$（或$\mathbf{Z}u$）。则群 $P/P'$ 和 $P'/P''$ 是无扭的，因而 $P'$ 中存在 $P''$ 的补集，P 中存在 $P'$ 的补集。因而，存在 $\mathbf{Z}$ 模 P 的基 $(z_1, z_2, \ldots, z_l)$ 和有理数整数$j, m, n$使得$u = jz_1, v = mz_1 + nz_2, j > 0, n > 0$。将 $X_i = e^{z_i}$ 代入 $1 \leq i \leq l$，则得到 $1 - e^u = 1 - X_1^j, 1 - e^v = 1 - X_1^m X_2^n$。设K为A的分数域代数闭包，则$A[P]$可以与环$B = K[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$的子环识别。对于单位元 $z$ 中的任何 $j$th 根，$1 - zX_1$ 是极值
$$
K[X_1, \ldots, X_l];
$$
而且，$1 - zX_1$包含生成的理想在$X_i$中没有单项式。我们结论认为B的理想$(1 - zX_1)B$是高度为1的素理想

（交换代数，第VII, § 1, no. 6），因而$1 - zX_1$在B中是极值。因而，B中$1 - X_1^j$的极值因子是形式$1 - zX_1$。现在B中的这些因子除$1 - X_1^m X_2^n$（对于从B到B的同态$f$，使得$f(X_1) = z^{-1}, f(X_i) = X_i$对于$i \geq 2$来说，满足

$$
f(1 - zX_1) = 0 \quad \text{and} \quad f(1 - X_1^m X_2^n) = 1 - z^{-m} X_2^n \neq 0).
$$

因而，$1 - X_1^j$和$1 - X_1^m X_2^n$在B中互质。因而，$A[P]$中$1 - X_1^j$和$1 - X_1^m X_2^n$的任何公共的除子在B中都是可逆的，因而，直到形式的乘法乘元素 $X_1^{k_1} X_2^{k_2} \ldots X_l^{k_l}$，等于A的元素$a$；在其他字中，$a$ 除 1 在 A 中，因此在 A 中可逆。因而，最终，$1 - X_1^j$ 和 $1 - X_1^m X_2^n$ 在 $A[P]$ 中互质。

### 2. 群权的案例；最大项

我们保留前面的数的记号，并让R在实数向量空间V中为约化根系。在这个截面的剩余部分中，我们取 R (§ 1, no. 9) 的权的 P 群。 群 $W = W(R)$ 作用于 P，因此也作用于代数 $A[P]$；我们有 $w(e^p) = e^{w(p)}$ 对应 $w \in W$ 和 $p \in P$。

令 C 为 R (§ 1, no. 5) 的一个室，并令 $B = (\alpha_i)_{1 \leq i \leq l}$ 为 R 的相应的基。我们为 V（因此也为 P）提供由 C 定义的阶结构。如果$p, p' \in P, p \geq p'$当且仅当$p - p'$是具有正系数的$\alpha_i$的线性组合。

#### 定义 1 {#lie-vi-s3-def-1 .statement tag=0AXO}

令 $x = \sum_{p \in P} x_p e^p$ 为 $A[P]$ 的元素。 $p \in P$的集合 S，使得$x_p \neq 0$称为x的支持度，S的极大元素的集合X称为x的最大支持度。 项 $x_p e^p$ 和 $p \in X$ 被称为 x 的最大项。

#### 引理 2 {#lie-vi-s3-lem-2 .statement tag=0AXP}

令 $x \in A[P]$ 和$(x_p e^p)_{p \in X}$ 为 x 的最大项族。令$q \in P$和$y \in A[P]$使得$e^q$是y的唯一最大值项。那么，$xy$的最大项的族就是$(x_p e^{p+q})_{p \in X}$。

输入$x = \sum_p x_p e^p, y = \sum_r y_r e^r$和$xy = \sum_t z_t e^t$。然后 $r \leq q$ 对于所有 $r \in P$ 使得 $y_r \neq 0$ 和 $z_t = \sum_{p+r=t} x_p y_r$。

如果$t = p + q = p' + r$与$p \in X$和$x_{p'} y_r \neq 0$，则$r \leq q$，因而$p' \geq p$，进而$p' = p$。因而$z_{p+q} = x_p y_q = x_p \neq 0$。这表明$X + q$包含在乘积$xy$的支撑中。

另一方面，如果 $t = p' + r$ 和 $x_{p'} y_r \neq 0$，则存在 $p \in X$，使得 $p' \leq p$ 并且我们有 $t \leq p + q$。因而$xy$的最大支持度包含在$X + q$中。由于$X + q$中没有两个元素具有可比性，因而$X + q$恰好是$xy$的最大支持度，并且我们在上面看到了$p \in X$的$z_{p+q} = x_p$，它完成了引理的证明。

#### 注 {#lie-vi-s3-n2-rem-1 .statement tag=0AXQ}

由于$x \neq 0$意味着$x$的最大支持度非空，引理2表明只要$y$承认形式$e^q$的唯一最大项，$x \neq 0$就意味着$xy \neq 0$。

### 3.反不变元素

我们保留前面的数的记号。用 $\varepsilon(w)$ 表示元素 $w \in W$ 的行列式。因此
$$
\varepsilon(w) = (-1)^{l(w)},
$$
长度$l(w)$是相对于反射系列$s_{\alpha_i}$而言的。

#### 定义 2 {#lie-vi-s3-def-2 .statement tag=0AXR}

*元素* $x \in A[P]$ *据说在* $W$ *if* 下是反不变的
$$
w(x) = (-1)^{l(w)}.x
$$
*对于所有人*$w \in W$。

$A[P]$ 形式的反不变量元素 $A$ $A[P]$ 子模。对于任意 $x \in A[P]$，将
$$
J(x) = \sum_{w \in W} \varepsilon(w).w(x).
$$
(1)

对于 $x \in A[P]$ 和 $w \in W$，我们有
$$
w(J(x)) = \sum_{v \in W} \varepsilon(v).wv(x) = \varepsilon(w) \sum_{v \in W} \varepsilon(v).v(x) = \varepsilon(w).J(x)
$$
且 $J(x)$ 是反对不变的。另一方面，令$q = \mathrm{Card}(W)$。对于 $A[P]$ 的任何反不变量元素 $x$，我们有 $J(x) = q.x$。由此可知，如果 $q$ 在 $A$ 中可逆，则映射 $q^{-1}J$ 是从 $A[P]$ 到反不变量元素的子模的 *投影*。

让 $\overline{\omega}_1, \ldots, \overline{\omega}_l$ 成为腔室 $C$ 的基本权相应的。 $P \cap \overline{C}$（或$P \cap C$）的元素是形式$n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$的权，以及$n_i \geq 0$（或$n_i > 0$）对于$1 \leq i \leq l$（§ 1, no. 10）。另一方面，
$$
\rho = \overline{\omega}_1 + \cdots + \overline{\omega}_l
$$
是正值根的一半和（*loc.cit.*），因此$P \cap C$的元素是形式$\rho + p$和$p \in P \cap \overline{C}$的权。最后，如果$p \in P \cap C$，则$w(p) < p$对于所有$w \neq 1$（§ 1, no. 6，适用于第18号提案），并且$e^p$因此是$J(e^p)$的唯一最大值项。

#### 命题 1 {#lie-vi-s3-prop-1 .statement tag=0AXS}

*If* 2 *is not a zero divisor in* $A$, *the elements* $J(e^p)$ *for* $p \in P \cap C$ *form a basis of the module of anti-invariant elements of* $A[P]$.

权 $w(p)$ 对于 $w \in W$ 和 $p \in P \cap C$ 是成对不同的。由此可见，$J(e^p)$ 与 $p \in P \cap C$ 是线性无关的。

另一方面，令 $x = \sum_p x_p e^p$ 为 $A[P]$ 的反不变量元素。如果 $p_0$ 属于到一堵墙，它在反射 $s \in W$ 下是不变的，并且
$$
x = \sum_p x_p e^p = -s(x) = -\sum_p x_p e^{s(p)}.
$$
由此可知$2x_{p_0} = 0$，所以$x_{p_0} = 0$。由于每个不与任何墙属于相关的元素都可以用 $w \in W$ 和 $p \in P \cap C$ 唯一地写成形式 $w(p)$，因此我们有
$$
x = \sum_{p \in P \cap C} \sum_{w \in W} x_{w(p)} e^{w(p)}. \tag{2}
$$
由于$w(x) = \sum_p x_p e^{w(p)} = \varepsilon(w) \sum_p x_p e^p$、$x_{w(p)} = \varepsilon(w)x_p$，我们从 (2) 推出
$$
x = \sum_{p \in P \cap C} x_p J(e^p),
$$
完成证明。

现在考虑代数 $A[\frac{1}{2}P]$ 的元素 $d$ 定义为
$$
d = \prod_{\alpha \in R, \alpha > 0} (e^{\alpha/2} - e^{-\alpha/2}) \\
= e^{\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (1 - e^{-\alpha}) \\
= e^{-\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (e^{\alpha} - 1).
$$
从$\rho \in P$、$d \in A[P]$开始。

#### 命题 2 {#lie-vi-s3-prop-2 .statement tag=0AXT}

(i) *(3)定义的元素 d是A[P]的反不变量元素；其独特的最大值项*（no. 2，默认值1）*是*$e^{\rho}$*和*$d = J(e^{\rho})$。
(ii) *对于任何* $p \in P$，*元素* $J(e^p)$ *可被* $d$ *唯一整除，并且商* $J(e^p)/d$ *是* $A[P]$ *在* $W$下不变的元素。
(iii) *如果2不是$A$中的零因子，*乘法由*$d$*从*$A[P]$*元素集合到双射*$W$*下不变* $A[P]$ 的反不变量元素的集合。

我们知道，对于$1 \leq i \leq l$，除了$\alpha_i$和$s_i(\alpha_i) = -\alpha_i$之外，反射$s_i = s_{\alpha_i}$使正根的集合保持稳定（§ 1, no. 6，第17条命题的Cor.1）。因此，
$$
s_i(d) = (e^{-\alpha_i/2} - e^{\alpha_i/2}) \prod_{\alpha \in R, \alpha > 0, \alpha \neq \alpha_i} (e^{\alpha/2} - e^{-\alpha/2}) \\
= -d = \varepsilon(s_i).d.
$$
由于$s_i$生成$W$，这证明了(i)中的第一个断言。 (i) 中的第二个断言紧随 (3) 和引理 2，注意 1 是 $1 - e^{-\alpha}$ 对于 $\alpha \in R, \alpha > 0$ 的唯一最大值项。

现在假设$A = \mathbf{Z}$。根据命题 1，

$$
d = \prod_{p \in P \cap C} c_p J(e^p) \quad \text{with} \quad c_p \in \mathbf{Z}.
$$

另一方面，很明显

$$
d = e^\rho + \sum_{q < \rho} c'_q e^q.
$$

如果$p \in P \cap C$与$p \neq \rho$，则$p > \rho$和$d$中$e^p$的系数由(5)得出零。因此，$c_p = 0$。此外，比较（4）和（5）中$e^\rho$的系数表明$c_\rho = 1$，因此$d = J(e^\rho)$。

我们继续假设$A = \mathbf{Z}$。令$p \in P, \alpha \in \mathbf{R}$和$M$为系统，代表元$W$关于子群$\{1, s_\alpha\}$的右陪集。然后，

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} + \sum_{w \in M} \varepsilon(s_\alpha w) e^{s_\alpha w(p)}.
$$

现在$s_\alpha w(p) = w(p) - \langle \alpha^*, w(p) \rangle \alpha = w(p) + n_w \alpha$，还有$n_w \in \mathbf{Z}$。因此，

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} (1 - e^{n_w \alpha}).
$$

如果$n_w \geq 0$，显然$1 - e^{n_w \alpha}$可以被$1 - e^\alpha$整除，并且从$1 - e^{n_w \alpha} = -e^{n_w \alpha}(1 - e^{-n_w \alpha})$开始，当$n_w < 0$时也是如此。因此，在 $\mathbf{Z}[P]$ 中，$J(e^p)$ 可以被 $1 - e^\alpha$整除。

通过引理 1，$\mathbf{Z}[P]$ 是阶乘，元素 $1 - e^\alpha$ $\alpha \in \mathbf{R}$ 和 $\alpha > 0$ 互质。由此可见，$J(e^p)$ 在 $\mathbf{Z}[P]$ 中可被乘积 $\prod_{\alpha > 0} (1 - e^\alpha)$整除，因此也可被 $d = e^{-\rho} \prod_{\alpha > 0} (1 - e^\alpha)$整除。

回到一般情况，通过从$\mathbf{Z}$到$A$的标量的扩张，我们从上面推出$d = J(e^\rho)$，并且每个元素$J(e^p)$都可以被$d$整除。由于$e^\rho$是$d$的唯一极大值项，no. 2的注表明存在唯一元素$y \in A[P]$使得$J(e^p) = dy$并且紧接着$y$在$W$下不变，因此$d$ 和 $J(e^p)$ 是反对不变的。这就证明了(i)和(ii)。

最后，如果2不是$A$中的零因子，no. 2的注和命题1意味着(iii)。

#### 注 1 {#lie-vi-s3-n3-rem-1 .statement tag=0AXU}

如果 2 不是 $A$ 中的零因子，则很容易检查 $d$ 是 $A[P]$ 的唯一反不变量元素，其中 $e^\rho$ 为其最大值项。

#### 注 2 {#lie-vi-s3-n3-rem-2 .statement tag=0AXV}

no. 2 的引理 2 显示商$J(e^p)/d$（对于$p \in P \cap C$）的唯一最大值项是$e^{p-\rho}$。

### 4. 不变元素

令$A[P]^W$为$A[P]$由……组成的元素的子代数在$W$下不变。 对于$p \in P$，用$W$下$p$的$W.p$轨道表示，并令$S(e^p) = \sum_{q \in W.p} e^q$为$e^p$的$W$变换的和；这是一个$W$不变量元素。

如果$p \in P \cap \overline{C}$、$w(p) \leq p$对于所有$w \in W$（$\S$ 1、no. 6，命题18）且$e^p$是$S(e^p)$的唯一最大值项。

设 $x = \sum_p x_p e^p \in A[P]^W$；那么$x_{w(p)} = x_p$对于所有$p \in P$和所有$w \in W$。

另一方面，$P$中$W$的每个轨道恰好在一个点中满足$P \cap \overline{C}$（$\S$1，no. 5，Th.2）。因此，

$$
x = \sum_{P \cap \overline{C}} x_p S(e^p).
$$

我们推论：

#### 引理 3 {#lie-vi-s3-lem-3 .statement tag=0AXW}

*$S(e^p)$适用于$A$模块$A[P]^W$的$p \in P \cap \overline{C}$形式基。*

$$
e_{i_0} = x_{i_0} - \sum_{j < i_0} a_{i_0 j} e_j,
$$
由此得出(b)。因此$J' \in \mathfrak{S}$是一个矛盾。由此，$J = I$和引理得证。

现在我们证明命题3。我们应用引理 4 和$I = P \cap \overline{C}$。令$q \in I$，并令$I_q$为$p \in I$的集合，使得$p \leq q$。如果$p \in I_q$，关系
$$
q - p \geq 0,\quad p \in \overline{C},\quad q \in \overline{C}
$$
暗示
$$
(q - p|p) \geq 0 \quad \text{and} \quad (q - p|q) \geq 0,
$$
因此
$$
(p|p) \leq (p|q) \leq (q|q).
$$
因此集合$I_q$是*有界的*。由于 $I$ 是离散的，因此$I_q$ 是*有限*，并且显然 $I$ 满足条件 (MIN)。另一方面，对于所有$p \in I$，
$$
x_p = e^p + \sum_{q < p} c_{pq} e^q
$$
所以由（6）。
$$
x_p = S(e^p) + \sum_{q < p, q \in I} c_{pq} S(e^q).
$$
命题现在紧随引理 3 和 4。

#### 定理 1 {#lie-vi-s3-thm-1 .statement tag=0AXX}

*令$\overline{\omega}_1, \ldots, \overline{\omega}_l$为室$C$的基本权相应的，对于$1 \leq i \leq l$，令$x_i$为$A[P]^W$的元素，其中$e^{\overline{\omega}_i}$为其唯一最大值项。让*
$$
\varphi : \Lambda[X_1, \ldots, X_l] \to A[P]^W
$$
*从多项式代数$\Lambda[X_1, \ldots, X_l]$到$A[P]^W$得到同态，需要$X_i$到$x_i$。那么，映射$\varphi$就是同构。*

引理 2 意味着单项式 $X_1^{n_1} \ldots X_l^{n_l}$ 的 $\varphi$ 下的像是元素，且唯一最大值为项 $e^{n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l}$。由于$P \cap \overline{C}$的每一个元素都可以唯一地写成形式$n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$，因此命题3表明单项式$X_1^{n_1} \ldots X_l^{n_l}$的$\varphi$下的像是$A[P]^W$的基，因此定理。

#### 例 1 {#lie-vi-s3-n4-exa-1 .statement tag=0AXY}

我们可以拿$x_i = S(e^{\overline{\omega}_i})$。

#### 例 2 {#lie-vi-s3-n4-exa-2 .statement tag=0AXZ}

通过*注* 2 of no. 3，我们可以得到$x_i = J(e^{\rho + \overline{\omega}_i})/d$（no. 3中有记号）。

### 习题{#lie-vi-s3-exercises}

记号和假设是no。 2、3、4。

§ 3](exercises/s3/)参见[习题。
