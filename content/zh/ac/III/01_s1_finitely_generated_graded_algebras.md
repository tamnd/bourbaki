---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 1
section_title: Finitely generated graded algebras
lang: zh
source: ac-i-vii
book_pages: 155-162, 232-233
pdf_pages: 0175-0182, 0252-0253
extraction: ocr
subsections:
    - "no": 1
      title: SYSTEMS OF GENERATORS OF A COMMUTATIVE ALGEBRA
      page: 155
      pdf_page: 175
    - "no": 2
      title: Criteria of Finiteness for Graded Rings
      page: 156
      pdf_page: 176
    - "no": 3
      title: PROPERTIES OF THE RING $A^{(d)}$
      page: 157
      pdf_page: 177
    - "no": 4
      title: GRADED PRIME IDEALS
      page: 160
      pdf_page: 180
statements: 13
exercises: 3
content_sha256: dc0f5728a664edc679de983f1d477052e40cea343b801d8026303843eb1d2f19
translated_from: content/en/ac/III/01_s1_finitely_generated_graded_algebras.md
translation_method: google
source_content_sha256: 4ef8d10c43b0b3fc4352b08bd49dd75b1412e18ba3d610df64784225920b10c7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8830fc613e4cf8f84f1697bdf1d91169e3f95b7eb9a199783e34f6221bf6e7a6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 有限生成分级代数

### 1. 系统生成元交换代数

令$\mathbf{A}$为交换环且$\mathbf{B}$为可交换的$\mathbf{A}$代数。让我们回忆一下（代数，章IV, § 2, no. 1），如果$x = (x_i)_{i \in I}$是$\mathbf{B}$的元素族，则从多项式代数$\mathbf{A}[X_i]_{i \in I}$到$\mathbf{B}$的映射$f \mapsto f(x)$是将$\mathbf{A}[X_i]_{i \in I}$的同态放到由$x_i$生成的$\mathbf{B}$的子代数上，其核$a$是多项式$f$的理想，使得$f(x) = 0$，称为*代数关系的理想（系数在 $\mathbf{A}$ 中）在 $x_i$* 之间。

#### 定义 1 {#ac-iii-s1-def-1 .statement tag=04D1}

*在交换环$\mathbf{A}$上的交换代数$\mathbf{B}$中，$\mathbf{B}$的元素的族$(x_i)_{i \in I}$被称为在$\mathbf{A}$上代数自由（或者$x_i$在$\mathbf{A}$上被称为代数独立），如果$x_i$之间的代数关系，系数在$\mathbf{A}$，减少到0。在$\mathbf{A}$上不是代数自由的族$(x_i)$也称为代数相关（或其元素也称为在$\mathbf{A}$上代数相关）。*

这个定义概括了代数、章V, § 5, no. 1、定义1中给出的元素或交换域的家庭。

(*) 除了在§ 5中使用章I, § 4的结果并因此同源代数之外，在这章中没有使用除了本书I到VI和章I和II之外的任何书籍。

说一个族$(x_i)_{i \in I}$在$A$上是代数自由的，相当于说，$x$中的单项式$\prod_i x_i^{n_i}$在$A$上“线性独立”；特别是 $x_i$ 与 $A$ 线性无关。

#### 定义 2 {#ac-iii-s1-def-2 .statement tag=04D2}

*交换代数* $B$ *超过交换环* $A$ *如果它是由元素的有限族生成的，则称为有限生成。*

这相当于说$B$同构于形式$A[X_1, \ldots, X_n]/a$的$A$代数（其中$X_i$是不定的，而$a$是多项式环$A[X_1, \ldots, X_n]$的理想）。

如果$A$-代数$B$是一个*有限生成的$A$-模*，那么它显然是一个有限生成的$A$-代数； 逆命题为假，如多项式代数的例所示 (cf. 章 V)。

如果 $B$ 是有限生成的 $A$-代数，并且 $A'$ 是任何可交换的 $A$-代数，$B_{(A')} = B \otimes_A A'$ 是有限生成的 $A'$-代数，因为如果 $(x_i)_{i \in I}$ 是生成元的系统 $A$-代数$B$，显然是$A$-代数$B_{(A')}$的生成元的$x, \otimes 1$形式系统。

如果$B$是有限生成的$A$-代数，$C$是有限生成的$B$-代数，则$C$是有限生成的$A$-代数；因为从定义可以立即得出，如果$(b_\lambda)_{\lambda \in L}$是$A$代数$B$的生成元的系统，并且$(c_\mu)_{\mu \in M}$是$B$代数的生成元的系统 $C$，$C$的每一个元素都等于一个多项式，系数在$A$、$b_\lambda$和$c_\mu$。

### 2. 分级环的有限性判据

*在此编号中。以下，所有考虑的毕业（代数、章 II, § 11）均假定为型* $\mathbf{Z}$。 *如果* $A$ *（分别为M）* *是分级的环*（分别为*分级的模*）、$A_i$（分别为$M_i$）*将表示次数*同质元素的集合* $i$ *在* $A$ *（分别为 M）*。

*如果* $A_i = \{0\}$ *（分别为$M_i = \{0\}$）* $i < 0$，$A$ *（分别为M）* *将缩写为分级环*（分别为*模*）*且次数*为正值。

#### 命题 1 {#ac-iii-s1-prop-1 .statement tag=04D3}

*令*$A = \bigoplus_{i \in \mathbf{Z}} A_i$*为具有正值次数的分级交换环，m为分级理想*$\bigoplus_{i \geq 1} A_i$*和*$(x_\lambda)_{\lambda \in L}$*元素*$A$*次数*$\geq 1$的同质元素族。 *以下条件是等效的*：

(a) *理想的* $A$ *由家庭产生* $(x_\lambda)$ *等于* $m$。

(b) *族* $(x_\lambda)$ *是* $A$*-代数* $A$ 的生成元系统。

(c) *对于所有* $i \geq 0$，** $A$*-模块* $A_i$ *由形式* $\prod_\lambda x_\lambda^{n_\lambda}$ *中的元素生成，其中次数* $i$ *位于* $A$。

显然条件 (b) 和 (c) 是等价的。如果它们成立，则 m 的每个元素都是形式 $f((x_i))$，其中 $f$ 是 $A_0[X_\lambda]_{\lambda \in L}$ 的多项式，没有常数项；然后$m = \sum_{\lambda \in L} A x_\lambda$，证明(c)蕴涵(a)。相反，假设条件 (a) 成立。令 $A' = A_0[x_\lambda]_{\lambda \in L}$ 为由$(x_\lambda)$族生成的 A 的子代数，并让我们证明$A' = A$。为此，只要证明 $A_i \subset A$ 对于所有 $i \geq 0$ 就足够了。我们在$i$上经过归纳，性质对于$i = 0$来说是显而易见的。然后令$y \in A$，与$i \geq 1$。由于$y \in m$，存在有限支撑的A的元素的族$(a_\lambda)_{\lambda \in L}$，使得$y = \sum_\lambda a_\lambda x_\lambda$，并且我们可以假设每个$a_\lambda$是次数$i - \deg(x_\lambda)$的齐次（如果需要的话可以通过替换通过它的齐次分量） 次数);如$\deg(x_\lambda) > 0$、归纳假设表明，对于所有$\lambda \in L$、从而、$y \in A'$和$A_i \subset A'$，$a_\lambda \in A'$，证明(a)蕴涵(b)。

#### 推论 {#ac-iii-s1-n2-cor-1 .statement tag=04D4}

*让*$A = \bigoplus_{i \in \mathbf{Z}} A_i$，*成为一个分级的交换环，其中次数*和$m$*分级理想*，$\bigoplus_{i \geq 1} A_i$。

(i) *以下条件是等效的*：
(a) *理想*$m$ *为有限生成A-模*。
(b) *环* $A$ *是有限生成的 A,-模*。

(ii) *假设(i)中的条件保持并让*$M = \bigoplus_{i \in \mathbf{Z}} M_i$*成为有限生成的分级A-模。那么，对于所有* $i \in \mathbf{Z}$，$M_i$ *是一个有限 A,-模，并且存在* $i_0$ *这样* $M_i = \{0\}$ *对于* $i < i_0$。

(i) 如果 A 的元素的族 $(y_\mu)$ 是 A-模 m 的生成元的系统（分别是 A，模 A），则 $y_\mu$ 的同质组件的族由……组成也是如此； 条件 (a) 和 (b) 的等价由命题 1 得出。

(ii) 我们可以假设 A 是由次数 $> 1$ 的齐次元素 $a_i$ ($1 < i < r$) 生成（作为 A-模），而 M 是由齐次元素 $x_j$ ($1 < j < s$) 生成（作为 A-模）；让$h_i = \deg(a_i), k_j = \deg(x_j)$。显然，M 由线性组合和 $A_0$ 中的系数为元素 $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_r^{\alpha_r} x_j$ 组成，使得 $\alpha_i$ 为整数 $\geq 0$ 满足关系 $k_j + \sum_{i=1}^r \alpha_i h_i = n$；对于每个$n$，只有有限的数家庭$(\alpha_i)_{1 \leq i \leq r}$满足这些条件，因为$h_i \geq 1$对于所有$i$；我们结论知道$M_n$是有限生成的A,-模，而且当$n < \inf(k_j)$时显然是$M_n = \{0\}$。

### 3. 环 $A^{(d)}$ 的特性

设$A = \bigoplus_{i \in \mathbf{Z}} A_i$为分级的环，$M = \bigoplus_{i \in \mathbf{Z}} M_i$为分级的A-模；对于整数$(d, k)$中的每个有序对，使得$d \geqslant 1$和$0 \leqslant k \leqslant d - 1$，集合

$$
A^{(d)} = \bigoplus_{i \in \mathbf{Z}} A_{id}, \quad M^{(d, k)} = \bigoplus_{i \in \mathbf{Z}} M_{id + k}.
$$

显然，$A^{(d)}$是$A$的分级子环，而$M^{(d, k)}$是$A^{(d)}$的分级模块；此外，如果$N$是$M$的分级子模，则$N^{(d, k)}$是$M^{(d, k)}$的分级子模块$A^{(d)}$。我们应该写$M^{(d)}$而不是$M^{(d, 0)}$；对于每个$d \geqslant 1$，$M$是$A^{(d)}$模块$M^{(d, k)}$$(0 \leqslant k \leqslant d - 1)$的直和。

#### 命题 2 {#ac-iii-s1-prop-2 .statement tag=04D5}

*令$A = \bigoplus_{i \in \mathbf{Z}} A_i$为分级交换环，其中次数为正，$M = \bigoplus_{i \in \mathbf{Z}} M_i$为分级$A$模块。假设 $A$ 是有限生成的 $A_0$ 代数，$M$ 是有限生成的 $A$ 模。然后，对于整数中的每个有序对 $(d, k)$，使得$d \geqslant 1, 0 \leqslant k \leqslant d - 1$：*

(i) $A^{(d)}$ 是有限生成的 $A$ 模块。
(ii) $M^{(d, k)}$ 是有限生成的 $A^{(d)}$ 模块。

让我们证明 $A$ 是*有限生成的 $A^{(d)}$*-*模*。令$(a_i)_{1 \leqslant i \leqslant s}$为齐次元素的$A$代数$A$由……组成的生成元的系统。 形式 $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_s^{\alpha_s}$的$A$的元素（在数有限），使得$1 \leqslant i \leqslant s$的$0 \leqslant \alpha_i \leqslant d$构成$A^{(d)}$模$A$的生成元的系统；对于整数 $n_i \geqslant 0$ $(1 \leqslant i \leqslant s)$ 的每个系统，都有正整数 $q_i, r_i$，使得 $n_i = q_i d + r_i$ 其中 $r_i < d$ $(1 \leqslant i \leqslant s)$；那么

$$
a_1^{n_1} a_2^{n_2} \ldots a_s^{n_s} = (a_1 \ldots a_s^{q_s})^d (a_1^{r_1} \ldots a_s^{r_s})
$$

这证明了我们的断言，对于每个同质元素$x \in A$都满足$x^d \in A^{(d)}$。那么，如果$M$是有限生成的$A$模，那么它也是有限生成的$A^{(d)}$模；由于$M$是$M^{(d, k)}$$(0 < k < d - 1)$的*直接的*和，因此每个$M^{(d, k)}$都是有限生成的$A^{(d)}$模块，这证明了(ii)。

让我们将上述应用于分级$A$-模块$m = \bigoplus_{i \geqslant 1} A_i$，它是由no. 2的命题 1 的推论有限生成的；可以看出$m^{(d)}$是有限生成的$A^{(d)}$模块；因此（no. 2，命题 1 的推论）$A^{(d)}$ 是有限生成的 $A$ 代数。

#### 引理 1 {#ac-iii-s1-lem-1 .statement tag=04D6}

*令$A$为分级交换环，使得$A = A_0[A_1]$，$M$为分级$A$模块，以及$(y_\lambda)_{\lambda \in L}$系统为$M$的同质生成元，使得$\deg(y_\lambda) \leqslant n_0$对于所有$\lambda \in L$。然后，对于所有 $n \geqslant n_0$ 和所有 $k \geqslant 0$，$M_{n+k} = A_k \cdot M_n$。*

设$n \geqslant n_0$和$x \in M_n$。由于$y_\lambda$生成$M$，存在元素的$(a_\lambda)_{\lambda \in L}$族有限支撑的$A$使得$x = \sum_\lambda a_\lambda y_\lambda$；我们可以进一步假设每个 $a_\lambda$ 都是齐次的并且具有次数 $n + 1 - \deg(y_\lambda)$（如果需要，替换可以由次数的齐次分量组成）。作为

$A = A_0[A_1]$和$\deg(a_\lambda) > 0$，每个$a_\lambda$是形式$bb'$元素和，其中$b \in A_0, b' \in A$、从而$x \in A_1 M_n$。然后$M_{n+1} = A_1 M_n$，从而$M_{n+k} = A_k M_n$，由归纳于$k$。

#### 引理 2 {#ac-iii-s1-lem-2 .statement tag=04D7}

*令 $A$ 为分级交换交换环，使得 $A = A_0[A_1]$ 并令 $S = \bigoplus_{i \geq 0} S_i$ 为分级交换 $A$ 代数，且次数为正数，这是有限生成的 $A$ 模。那么存在整数 $n_0 \geq 0$ 这样：*

(i) *对于 $n \geq n_0$ 和 $k \geq 0$、$S_{n+k} = S_k \cdot S_n$。*
(ii) *对于 $d \geq n_0$、$S^{(d)} = S_0[S_d]$。*

到引理 1 时，存在整数 $n_0 \geq 0$，使得对于 $n \geq n_0$ 和 $k \geq 0$、$S_{n+k} = A_k S_n$、从而 *更不必说* $S_{n+k} = S_k S_n$，成立 (i)。然后，对于$d \geq n_0$和$m > 0$，$S_{m d} = (S_d)^m$如下由归纳在$m$应用(i)上；这就建立了(ii)。

#### 命题 3 {#ac-iii-s1-prop-3 .statement tag=04D8}

*令 $R = \bigoplus_{i \geq 0} R_i$ 为具有正次数的分级交换环，这是有限生成的 $R_0$ 代数。存在整数 $e \geq 1$，使得 $R^{(me)} = R_0[R_{me}]$ 对于所有 $m \geq 1$。*

令$(x_j)_{1 \leq j \leq s}$为$R_0$-代数$R$的齐次生成元的系统，其次数为$\geq 1$。 令$h_j = \deg(x_j)$，令$q$为$h_j$的公共的倍数，并让我们为$1 \leq j \leq s$写出$q_j = q/h_j$；那么元素$x_j^{q_j}$就是次数$q$的全部。 设$B$为$x_j^{q_j}$生成的$R$的子$R_0$代数；如果$i$不是$q$的倍数，则其分级为$R$和$B_i = 0$的子代数。 令$A$（或$S$）为分级的环，其底层环为$B$（或$R^{(q)}$），其分级由$A_i = B_{iq}$（或$S_i = R_{iq}$）组成。 然后$A = A_0[A_1]$乘定义除$B$。 Consider the elements of $R$ (finite in number) of the form $x_1^{\alpha_1} x_2^{\alpha_2} \ldots x_s^{\alpha_s}$, where $0 \leq \alpha_j \leq q_j$ and $\alpha_1 h_1 + \ldots + \alpha_s h_s \equiv 0$ (mod. $q$); let us show that they generate the $B$-module $R^{(q)}$. 足以证明形式$x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s}$的$R^{(q)}$的每一个元素都是上述元素的$B$线性组合。 现在，存在正整数$k_j, r_j$使得$n_j = k_j q_j + r_j$其中$r_j < q_j$($1 \leq j \leq s$)；然后

$$
x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s} = (x_1^{q_1})^{k_1} \ldots (x_s^{q_s})^{k_s} \cdot (x_1^{r_1} \ldots x_s^{r_s})
$$

并通过假设 $\sum_{j=1}^s n_j h_j \equiv 0$ (mod. $q$)，因此 $\sum_{j=1}^s r_j h_j \equiv 0$ (mod. $q$)；随着$x_j^{q_j}$属于到$B$乘以定义，这证明了我们的断言。由于$S$是有限生成的$A$模块，因此可以应用引理2：存在$n_0$，对于$d > n_0$、$S^{(d)} = S_0[S_d]$，因此对于$d \geq n_0$也存在$R^{(qd)} = R_0[R_{qd}]$。 命题后面跟着$e = q n_0$。

### 4. 分级素理想

令$A = \bigoplus_{i \geq 0} A_i$为分级交换环，其中*正*次数和$m$为分级理想$\bigoplus_{i \geq 1} A_i$；如果存在整数$n_0$使得$a_n = b_n$对应$n \geq n_0$（显然是等价关系），我们将称$A$的两个分级理想$a = \bigoplus_{i \geq 0} a_i, b = \bigoplus_{i \geq 0} b_i$*等价*。如果分级理想不等于 $m$，则称为“基本”。

#### 命题 4 {#ac-iii-s1-prop-4 .statement tag=04D9}

*设$p = \bigoplus_{i \geq 0} p_i$为$A$的分级理想；要使 $p$ 成为质数，必要且充分的是，如果 $x \in A, \ y \in A,$ 满足 $x \notin p$ 和 $y \notin p,$，则$xy \notin p$。*

条件显然是必要的。反之，如果满足，则两个同质元素$\neq 0$的分级环$A/p = \bigoplus_{i \geq 0} A_i/p_i$乘积是$\neq 0$，因此$A/p$是整环（*代数*，章） II, § 11, no. 4、命题7)。

#### 命题 5 {#ac-iii-s1-prop-5 .statement tag=04DA}

*令$a = \bigoplus_{i \geq 0} a_i$为$A$和$n_0$整数$> 0$的分级理想。对于存在分级素理想 $p = \bigoplus_{i \geq 0} p_i$ 使得 $n \geq n_0,$ 的 $p_{n_0} = a,$ ，必要且充分的是，对于次数 $\geq n_0,$ 关系 $xy \in a$ 的齐次元素 $x, y$ 的对意味着'“$x \in a$或$y \in a$”。如果存在$n \geq n_0$，使得$a_n \neq A_n,$素理想满足，则上述条件是唯一的。*

叙述的条件显然是必要的。如果$a_n = A_n$对于所有$n \geq n_0,$来说显然每个素理想包含$m$都是解到问题；因此可能有几个素理想可以解问题；然而，这些理想中的任何两个显然是等效的。假设存在齐次元素 $a \in A_d$（带有 $d \geq n_0$）而不是属于到 $a_d$。令$p$为$x \in A$的集合，使得$ax \in a$。显然$p$是$A$的理想；由于$ax$的齐次分量是$x$的齐次分量乘积乘以$a$，且$a$是分级理想，$p$是分级理想；此外，$1 \notin p$，因此$p \neq A$。要证明 $p$ 是素数，只需证明，如果 $x \in A, \ y \in A,$ 满足 $x \notin p$ 和 $y \notin p,$，则 $xy \notin p$ (命题 4)。然后$ax \notin a_{m+d}, ay \notin a_{n+d},$从而乘假设

$$
a^2xy \notin a_{m+n+2d};
$$

我们从$xy \notin p$开始结论即$axy \notin a_{m+n+d}$。最后，如果$n \geq n_0$和$x \in A_n,$条件$x \in a,$和$ax \in a_{n+d}$与假设等价，因此$p \cap A_n = a_n$完成了分级素理想$p$的存在性证明，从而解决了问题。如果$p'$也是$A$的另一个分级素理想，使得$n \geq n_0,$为$p' \cap A_n = a_n$，则$a \notin p'$和$ax \in p'$对于所有$x \in p,$从而$p \subset p'$，因为$p'$是素数。另一方面，如果$x$是次数的齐次元素，$p',$$n \geq 0$的齐次$ax$是次数$n + d \geq n_0$的齐次，因此属于到$p' \cap A_{n+d} = a_{n+d}$，从而通过定义$x \in p$，这表明$p' \subset p$，最后是$p' = p$。

#### 命题 6 {#ac-iii-s1-prop-6 .statement tag=04DB}

*设 d 为整数 $\geq 1$。*

(i) *对于 A 的每个基本分级理想 p，$p \cap A^{(d)}$ 是 $A^{(d)}$ 的基本分级素理想。*

(ii) *相反，对于$A^{(d)}$的每个基本分级素理想$p'$，都存在一个唯一的（必然是必要的）A的分级素理想$p$，使得$p \cap A^{(d)} = p'$。*

(i) 如果$a \in A_k$ 不属于到$p_k$，$a^{kd}$ 不属于到$p_{kd}$，因此$p \cap A^{(d)}$ 是必需的。

(ii) 对于所有$n \geq 0$，集合$p \cap A$，必须等于$x \in A$的集合$a_n$，使得$x^d \in p'$。让我们证明$a = \bigoplus_{n \geq 0} a_n$是一个分级素理想；如$a_n = p'_n$，当$n$是$d$的倍数时，由于$p'$是素数，这将证明$p$的唯一性。现在，如果 $x \in a_n$、$y \in a_m$、$(x - y)^{2d}$ 是项的和，其中每一个都是 $x^d$ 的乘积或 $y^d$ 通过次数 $nd$ 的齐次元素且因此$(x - y)^{2d} \in p'$，并且由于$p'$是素数，$(x - y)^d \in p'$，因此$a_n$是$A$的子群。由于$p'$是$A^{(d)}$的理想，$a$是$A$的分级理想；最后，关系$(xy)^d \in p'$隐含$x^d \in p'$或$y^d \in p'$，通过命题4完成证明。

令$A$为分级交换环，其中次数为正，$p$为$A$的基本分级素理想。 集合 $S$ *同质* 元素 $A$ 不是属于到 $p$ 是乘法，因此分数 $S^{-1}A$ 的环是规范分级的 (章) II, § 2, no. 9)（注，在这个毕业中通常会有同质的元素$\neq 0$负次数）。我们用次数 0 的齐次元素的$S^{-1}A$ 由……组成 $A_{(p)}$ 子环表示，其他分数 $x/s$ 的字集合，其中$x$和$s$是$A$和$s \notin p$中相同的次数齐次。类似地，对于每个分级的$A$-模块$M$，$S^{-1}M$均按规范分级（*loc.cit.*），我们将用$M_{(p)}$子群表示次数0的同质元素，这显然是一个$A_{(p)}$-模块。

#### 命题 7 {#ac-iii-s1-prop-7 .statement tag=04DC}

*设$p$为$A$的分级素理想，$d$整数$\geq 1$，$p'$为$A^{(d)}$的分级素理想$p \cap A^{(d)}$；对于每个分级的$A$-模块$M$，从典范嵌入$M^{(d)} \to M$派生的同态$(M^{(d)})_{(p')} \to M_{(p)}$是双射的。*

如果$S$是$A$的齐次元素的集合而不是属于到$p$和$S' = S \cap A^{(d)}$，典范同态$\phi : {S'}^{-1}M^{(d)} \to S^{-1}M$是次数0的齐次同态并且它是单射的，对于，如果$x \in M_{nd}$对于$s \in A_n, s \notin p$满足$sx = 0$，则也满足$s^dx = 0$和$s^d \in A_{md}, s^d \notin p'$。尚需证明$(M^{(d)})_{(p')}$的$\phi$下的像是$M_{(p)}$的全部；但如果$x \in M_n, s \in A_n$和$s \notin p$，那么还有$x/s = (xs^{d-1})/s^d$，其中$xs^{d-1} \in A_{nd}, s^d \in A_n$和$s^d \notin p'$，从而我们的断言。

#### 命题 8 {#ac-iii-s1-prop-8 .statement tag=04DD}

*设$m = \bigoplus_{i \geq 1} A_i$；令 $(p^{(k)})_{1 \leq k \leq s}$ 为 $A$ 的分级素数*理想和分级理想 $\mathfrak{a} \subset A$ 的有限族，使得 $\mathfrak{a} \cap m \not\subset p^{(k)}$ 对于所有 $k$；那么对于任何 $p^{(k)}$ 都存在齐次元素 $z \in \mathfrak{a} \cap m$ 而不是属于。

我们通过归纳对$n$进行争论，命题对于$n = 1$来说是微不足道的。如果存在指标$j$，使得$\mathfrak{a} \cap m \cap p^{(j)}$包含在指标$k \neq j$的$p^{(k)}$之一中，则从归纳假设得出，对于任何一个元素$z' \in \mathfrak{a} \cap m$而非属于，存在齐次$p^{(k)}$对于$k \neq j$，因此也不是属于到$p^{(j)}$，并且这个元素解决了问题。假设对于每个指标$j$，$\mathfrak{a} \cap m \cap p^{(j)}$不包含在指标$k \neq j$的任何$p^{(k)}$中；因此，归纳假设意味着存在同质的元素$y_j \in \mathfrak{a} \cap m \cap S_j$属于，不存在$S_j$对于$k \# j$；由于$y_j$都是次数$\geq 1$，我们可以通过替换通过合适的幂（因为$p^{(k)}$是素数）假设$y_1$和$\prod_{j=2}^n y_j$是相同的次数。那么$z = y_1 + \prod_{j=2}^n y_j$是次数$\geq 1$的齐次，并且与章II, § 1, no. 1相同的论证，命题2表明$z$解决了问题。

### 习题{#ac-iii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
