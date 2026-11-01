---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 5
section_title: Commutation
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.77-A VIII.94
pdf_pages: 0094-0111
extraction: native
subsections:
    - "no": 1
      title: The Commutant and Bicommutant of a Module
      page: 77
      pdf_page: 94
    - "no": 2
      title: Generating Modules
      page: 79
      pdf_page: 96
    - "no": 3
      title: The Bicommutant of a Generating Module
      page: 82
      pdf_page: 99
    - "no": 4
      title: The Countermodule of a Semisimple Module
      page: 84
      pdf_page: 101
    - "no": 5
      title: Density Theorem
      page: 88
      pdf_page: 105
    - "no": 6
      title: Application to Field Theory
      page: 89
      pdf_page: 106
statements: 37
exercises: 19
content_sha256: 8b0d251abf60e27afc0d813ea8fe5aad8ef56a5c4e33b016a84d28b35a658ec6
translated_from: content/en/alg/VIII/05_s5_commutation.md
translation_method: google
source_content_sha256: 92146afa3071a759dfd60b0a1909d5b82cb570c6ed50a098e57fa1acd8ea9c00
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0a1afb599f21761ef844b26f74919dfb11fbee6f90399f5c9868ba9ca83df6fb
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 5。 交换

### 1. 模的交换矩阵和双交换矩阵

设 E 为 E 的环，B 子集。 B 在 E 中的交换子（或集中子）是元素的 E 由……组成子环 $B'$，与 B 的每元素交换。 $B'$ 的交换子 $B''$ 称为 B 的双交换子（或双中心子）。 我们有 $B\subset B''$ 和 $B'$ 重合及其双交换体 (III, §1, No. 2, p. 429)。 E的子环B中心为$B\cap B'$； $B'$和$B''$之公共中心是$B'\cap B''$。 如果 B 是 E 的交换子环，则我们有 $B\subset B'$，并且 $B''$ 是 $B'$ (III, §1, No. 2，p. 430) 的中心。

设 A 为环，M 为左（右）A-模。让我们将这些定义应用到当E是M的加法群的自同态环和M的同调$A_M$的B环时的情况。E中$A_M$的交换子$A'_M$称为M的交换子；是A-模 M 的自同态环。E 中$A_M$ 的双交换子$A''_M$ 称为M 的双交换子；是M的对模自同态环(VIII、p. 8、定义3)。我们有$A_M\subset A''_M$，环$A_M\cap A'_M$是$A_M$的中心，$A'_M\cap A''_M$是$A'_M$和$A''_M$的公共中心。

#### 定义 1 {#alg-viii-s5-def-1 .statement tag=005E}

如果我们有 $A_M= A''_M$，则A-模 M 是平衡的。

如果A-模 M 平衡，则环 $A_M$ 和$A'_M$ 具有相同的中心 $A_M\cap A'_M$。 模 M 是平衡的 A-模当且仅当它是平衡的 $A_M$ 模块。 A-模 M 中的对模是忠实且平衡的。

当环 A可交换时，M的双交换数$A''_M$为$A'_M=$End$_A(M)$的中心； M 是平衡的意味着 End$_A(M)$ 的中心被约化为同位。

对于 A 的任何元素 $a$，用 $\boldsymbol{\delta }_a$ 表示从 A 到 A 的右侧位似 $x\mapsto xa$，并用 $\boldsymbol{\gamma }_a$ 表示左侧位似 $x\mapsto ax$ (I, §8, No. 1, p. 97)。 映射$a\mapsto \boldsymbol{\delta }_a$是从$A^o$到左A-模$A_s$的交换子环同构（cf.II, §10, No. 7、p. 349，应用于$I =\{1\}$）。 映射$a\mapsto \boldsymbol{\gamma }_a$是从A到右A-模$A_d$的交换子的环同构（前述）。如果我们通过这个映射将认同与$A_d$的交换子进行A，那么$A_d$的对模就等同于$A_s$；因而，A-模 $A_d$ 是平衡的。同样，A-模$A_s$是平衡的。

设$n$为整数$\geqslant 1$。我们将$A^n$视为左$\mathbf{M}_n$(A)-模块（前述）。将$m\in \mathbf{M}_n(A)$发送到A-模$A^n_d$的自同态$x\mapsto mx$的映射是从$\mathbf{M}_n(A)$到右A-模$A^n_d$的交换子的环同构（见上文）。

#### 命题 1 {#alg-viii-s5-prop-1 .statement tag=005F}

令$(A_i)_{i\in I}$为环的族，对于每个$i\in I$，令$M_i$为$A_i$模块。 集合$A =\prod A_i,M =\prod M_i$和$N =\bigoplus M_i$。赋予M A-模的结构和作用 $((a_i),(x_i))\mapsto (a_ix_i)$ 的律。 集合 N 是 M 的 A-子模。

a) 映射$(u_i)\mapsto \prod u_i$从$\prod$结束$_{\mathbf{Z}}(M_i)$到结束$_{\mathbf{Z}}(M)$（II, §1, No. 5，p. 200）限制到环同构从$\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$，以及$\prod(A_i)''_{M_i}$到分别是$A_M,A'_M$和$A''_M$。

b) 映射$(u_i)\mapsto \bigoplus u_i$从$\prod$结束$_{\mathbf{Z}}(M_i)$到结束$_{\mathbf{Z}}(N)$（II, §1, No. 6，p. 203）限制到环同构从$\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$，以及$\prod(A_i)''_{M_i}$到分别是$A_N,A'_N$和$A''_N$。

命题 1 中定义的环同构称为规范。 乘积$\prod(A_i)_{M_i}$常常通过这些同构与$A_M$识别，$\prod(A_i)'_{M_i}$与$A'_M$等识别。

从$\prod$End$_{\mathbf{Z}}(M_i)$到End$_{\mathbf{Z}}(M)$的映射$\varphi : (u_i)\mapsto \prod u_i$是单射环同态。到 M 上的 A-模结构的定义时，我们有 $\varphi (\prod(A_i)_{M_i}) = A_M$。让$u\in A'_M$。对于每个 $i\in I$，用 A 的 $h_i$ 元素表示，除了指标 $i$ 等于 0 之外，所有分量都等于 1 。如果 $x$ 是 M 的元素，且指标 $i$ 的分量等于 0，则我们有 $x=h_ix$，因而 pr$_i(u(x)) =$ pr$_i(u(h_ix)) =$ pr$_i(h_iu(x)) = 0$。因而，存在唯一群同态 $u_i: M_i\mapsto M_i$，使得每个 $y\in M$ 都有 pr$_i(u(y)) =u_i$(pr$_i(y)$)。我们有$u=\prod u_i$。由于映射 $u$ 是 A 线性的，因此对于每个 $i\in I$，映射 $u_i$ 都是 $A_i$ 线性。这就证明了$\prod(A_i)'_{M_i}$在$\varphi$包含$A'_M$下的像；反向包含是显而易见的。通过M的应用到对模，我们推导出$\varphi$诱导同构从$A''_M$到$\prod_i(A_i)''_{M_i}$。这就证明了断言a)。

b)的证明与a)的证明相同。

#### 命题 2 {#alg-viii-s5-prop-2 .statement tag=005G}

设A为环，设M为A-模。设I为集合。然后是A-模 $M^{(I)}$ 重合与$A''_M$-模$M^{(I)}$同调的环的二交换。

对于$i\in I$，我们用$\pi_i: (x_j)_{j\in I}\mapsto x_i$表示从$M^{(I)}$到M的投影同态，用$\iota_i: M\rightarrow M^{(I)}$表示相应的典范嵌入（I, §4, No. 9，p. 47）。

设$u$为End$_A(M^{(I)})$的元素。对于所有$i, j\in I$，合成$u_{i,j}=\pi_j\circ u\circ \iota_i$属于到M的交换子$A'_M$。对于$A''_M$的每个元素$b$和每个$(x_i)\in M^{(I)}$，我们有关系

$$
bu((x_i)_{i\in I})=b(\sum_{i\in I}u_{i,j}(x_i))_{j\in I}=(\sum_{i\in I}u_{i,j}(bx_i))_{j\in I}=u(b(x_i)_{i\in I})
$$

位似 $b_{M^{(I)}}$ 因此属于为 A-模 $M^{(I)}$ 的双交换数。

相反，令 $b$ 为 $M^{(I)}$ 的双交换数的元素。对于 $i, j\in I$、集合 $b_{i,j}=\pi_j\circ b\circ \iota_i$。将 $i, j\in I$ 与 $i\not=j$ 一起取。从$\iota_j\circ \pi_j$属于到A-模$M^{(I)}$的交换律，我们有

$$
b_{i,j}=\pi_j\circ \iota_j\circ \pi_j\circ b\circ \iota_i=\pi_j\circ b\circ \iota_j\circ \pi_j\circ \iota_i= 0
$$

同样，我们有

$$
b_{j,j}=\pi_j\circ b\circ \iota_j=\pi_i\circ \iota_i\circ \pi_j\circ b\circ \iota_j=\pi_i\circ b\circ \iota_i\circ \pi_j\circ \iota_j=b_{i,i}
$$

此外，$b_{i,i}$属于至$A''_M$。由此可知 $b$ 重合与 $A''_M$ 模块 $M^{(I)}$ 的位似。

### 2.生成模

设 A 为环。

#### 定义 2 {#alg-viii-s5-def-2 .statement tag=005H}

如果从 M 到 N 每个 A-模 N 都是由 A-线性映射的像生成，A-模 M 称为生成的。

令 M 为左A-模。我们用 $M^*$ 表示 M 的对偶，用 $M\times M^*$ (II, §2, No. 3, p. 233) 表示规范的双线性形式

$$
(x, x^*)\mapsto  \langle x, x^*\rangle =x^*(x)
$$

我们用形式$\sum^n_{i=1}\langle x_i, x^*_i\rangle$的A的元素$\tau (M)$集合来表示，其中$x_1, . . . , x_n$是M的元素，$x^*_1, . . . , x^*_n$是$M^*$的元素。它是A的两侧理想，称为M的迹理想。A-模$A_s$的迹理想是A。模的迹理想，即A-模的家庭$(M_i)_{i\in I}$的直和是理想$\sum_{i\in I}\tau (M_i)$。如果M是射影A-模，那么从II, §2, No. 6、p. 238的命题 12得出，我们有$M =\tau (M)M$。

#### 定理 1 {#alg-viii-s5-thm-1 .statement tag=005I}

设 M 为左A-模。以下属性是等效的：

(i) A-模 M 为生成的。

(ii) 对于每个A-模 N，从$M^{(I)}$到N存在集合I和满射A-线性映射。

(iii)从$M^n$到$A_s$存在整数$n\geqslant 0$和满射A-线性映射。

(iv) 存在整数$n\geqslant 0$，使得$A_s$与$M^n$的直因子子模同构。

(v) 理想迹 $\tau (M)$ 等于 A。

(vi) M存在整数$n\geqslant 0$、元素$x_1, . . . , x_n$，以及$M^*$满足$\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$中的元素$x^*_1, . . . , x^*_n$。

(i) $\Rightarrow$ (ii)：假设M为生成的，令N为左A-模。存在从 M 到 N 的A-线性映射族$(u_i)_{i\in I}$，因此我们有$N =\sum_{i\in I}u_i(M)$。从 $M^{(I)}$ 到 N 的映射 $(x_i)\mapsto \sum_{i\in I}u_i(x_i)$ 是 A 线性且满射的。

(ii)$\Rightarrow$(iii)：假设性质(ii)成立，取$N = A_s$。然后我们有集合 I 和一个满射线性映射 $u: M^{(I)}\rightarrow A_s$。由于$A_s$是由元素1生成的，因此存在I的有限子集J，使得$u(M^{(J)}) = A_s$，从而 (iii)。

(iii) $\Rightarrow$ (iv)：这是从II, §1, No. 12、p. 218 的命题 21 得出的。

(iv) $\Rightarrow$ (v)：设$n\geqslant 1$为整数，使得$A_s$同构于M的直因子子模。我们有$A =\tau (A_s)\subset \tau (M^n) =\tau (M)$，因此有$\tau (M) = A$。

(v) $\Rightarrow$ (vi)：这很清楚。

(vi)$\Rightarrow$(i)：设$n$为M的整数$\geqslant 0,x_1, . . . , x_n$元素，以及$M^*$满足$\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$的$x^*_1, . . . , x^*_n$元素。令N为N的左A-模和$y$元素。从M到N的映射$u_i:x\mapsto  \langle x, x^*_i\rangle y$是A线性的，我们有$y=\sum^n_{i=1}u_i(x_i)$。这就证明M是生成A-模。

#### 推论{#alg-viii-s5-n2-cor-1 .statement tag=00R1}

生成A-模是忠实的。

让$a\in A$满足$aM = 0$。使用定理 1 的蕴涵 (i) $\Rightarrow$ (iv)，我们得到 $aA_s= 0$，从而得到 $a= 0$。推论如下 (II, §1, No. 12, p. 219)。

#### 例 1 {#alg-viii-s5-n2-exa-1 .statement tag=005J}

A-模$A_s$是生成的。

#### 例 2 {#alg-viii-s5-n2-exa-2 .statement tag=005K}

每个非零的自由A-模都是生成的。更一般地，每个具有生成的商的模本身就是生成的。

#### 例 3 {#alg-viii-s5-n2-exa-3 .statement tag=005L}

设 M 为半单A-模，其中对模是有限生成的。那么M就是生成的$A_M$-模。事实上，通过VIII、p. 8的引理 4，存在自然数$m$，使得$(A_M)_s$同构于$M^m$的子模。由于$M^m$是半单$A_M$模，$(A_M)_s$与$M^m$的直因子子模同构，M是生成的$A_M$模(定理1)。

#### 例 4 {#alg-viii-s5-n2-exa-4 .statement tag=005M}

设A为主理想整环，设P为有限生成A-模。 A 的理想 $(\mathfrak{a}_i)_{1\leqslant i\leqslant n}$ 存在整数 $n\geqslant 1$ 和递增序列，使得 P 同构于 $A/\mathfrak{a}_i$ 的直和 (VII, §4, No. 4, p. 19, 定理 2)； P 的湮没子$\mathfrak{a}$等于$\mathfrak{a}_1$。那么 P 是生成模超过环 $A/\mathfrak{a}$。如果 P 不是挠元模，那么我们有 $\mathfrak{a}= 0$ 并且 P 是生成A-模。

#### 引理 1 {#alg-viii-s5-lem-1 .statement tag=005N}

设A为交换环，M为有限生成A-模，Ann(M)为湮没子。令 $\mathfrak{a}$ 为 A 的理想。以下性质是等效的：

（一）$\mathfrak{a}M = M$。

(ii) 安 (M) $+\mathfrak{a}= A$。

(iii) 存在$\mathfrak{a}$的元素$a$，使得每个$m\in M$都有$am=m$。

(i) $\Rightarrow$ (ii)：令$(x_1, . . . , x_n)$为A-模 M的生成的族。如果$\mathfrak{a}M = M$，则每个$x_i$可写为$\sum^n_{j=1}c_{ij}x_j$，其中$c_{ij}$属于至$\mathfrak{a}$。用 C 表示矩阵 $(c_{ij})$，并用 $x_1, . . . , x_n$ X 表示列矩阵。我们有 ($I_n-C$)X = 0。令$d$为矩阵$I_n-C$的行列式，V为辅因子矩阵。通过III, §8, No. 6、p. 532的公式(26)，我们有$dX=^tV$($I_n-C$)X = 0，因而$d\in$Ann(M)。另一方面，从 $c_{ij}$ 属于到 $\mathfrak{a}$，我们有 $d\equiv$ 1(mod $\mathfrak{a}$) (III, §8, No. 5, p. 529, (18))，因此有 $1\in$ Ann(M) $+\mathfrak{a}$。

(ii)$\Rightarrow$(iii)：假设(ii)成立，存在$a\in \mathfrak{a}$和$b\in$Ann(M)使得$a+b= 1$。然后，每 $m\in M$ 就有 $am=m$。

(iii)$\Rightarrow$(i)：这很清楚。

#### 命题 3 {#alg-viii-s5-prop-3 .statement tag=00R2}

设 A 为交换环。每个有限生成且忠实的射影A-模都是生成的。更一般地，有限生成的射影 A-模 P 是生成的 $A_P$ 模。

令 P 为有限生成的射影 A-模。我们有$\tau (P)P = P$（VIII，p. 80）。

如果 A-模 P 是忠实的，则理想的 $\tau (P)$ 等于 A (引理 1)，A-模 P 为生成的 (定理 1)；这导致第一个断言。第二个接着是下面的引理2。

#### 引理 2 {#alg-viii-s5-lem-2 .statement tag=005O}

设 A 为环，M 为射影 A-模。 $A_M$模 M 是射影的。

令$(x_i)_{i\in I}$为A-模M的生成的族。在A-模M上存在线性形式的$(x^*_i)_{i\in I}$族，使得对于每个$x\in M$，$(\langle x, x^*_i\rangle )_{i\in I}$族有有限支撑和$x=\sum_{i\in I}\langle x, x^*_i\rangle x_i$ （II, §2, No. 6、p. 238、命题12）。对于每个$i\in I$，映射$x\mapsto  \langle x, x^*_i\rangle_M$在$A_M$-模块M上是线性形式，并且对于每个$x\in M$我们有$x=\sum_{i\in I}\langle x, x^*_i\rangle_Mx_i$。按地点。如上所述，M 是射影 $A_M$ 模。

### 3. 生成模的双相变

#### 定理 2 {#alg-viii-s5-thm-2 .statement tag=005P}

生成模是平衡的。

设A为环，设M为生成A-模；通过定义，存在M的整数$n\geqslant 0$、元素$x_1, . . . , x_n$，以及M满足$\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$的对偶$M^*$的元素$x^*_1, . . . , x^*_n$。回想一下（II, §4, No. 2，p. 271），我们定义群同态$\theta : M^*\otimes_AM\rightarrow$结束$_A(M)$由公式$\theta (x^*\otimes y)(x) =\langle x, x^*\rangle y$。如果$u$是M的双交换量的元素，则它与End$_A(M)$可交换；因而，对于每个 $y\in M$，我们有

$$
u(y) =u(\sum_{i=1}^n\langle x_i, x^*_i\rangle y)=\sum_{i=1}^nu(\theta (x^*_i\otimes y)(x_i))
$$

$$
=\sum_{i=1}^n\theta (x^*_i\otimes y)(u(x_i)) =(\sum_{i=1}^n\langle u(x_i), x^*_i\rangle )y
$$

因而，$u$属于到$A_M$，并且M是平衡的。

#### 推论 1 {#alg-viii-s5-thm-2-cor-1 .statement tag=005Q}

自由模是平衡的。

如果模是零，并且非零的自由模是生成的（VIII，p. 81，例2），这一点是清楚的。

#### 推论 2 {#alg-viii-s5-thm-2-cor-2 .statement tag=00R3}

令A为环，令$n$为整数$\geqslant 0$。 $\mathbf{M}_n(A)$的中心由标量矩阵和A的中心中的条目组成。我们将$A^n$视为左$\mathbf{M}_n(A)$模块（II, §10, No. 7，p. 349）。这个模中的自同态是映射$x\mapsto xa$，其中$a$穿过A。

令 M 为右A-模 $A^n_d$。它由推论 1 平衡。因而，$A_M, A'_M$ 的中心，以及 $A''_M$ 重合。推论 2 由以下事实得出：$A_M$ 与 A 相同，$A'_M$ 与 $\mathbf{M}_n(A)$ 相同。

#### 注 {#alg-viii-s5-n3-rem-1 .statement tag=005R}

令 M 为 A-模。如果$A_M$-模块M是生成的，那么我们将$A_M= A''_M$乘以定理2应用于$A_M$-模块M，因此M是平衡的A-模。

#### 推论 3 {#alg-viii-s5-thm-2-cor-3 .statement tag=005S}

每个有限生成射影模超过交换环都是平衡的。

事实上，有限生成射影模 M 是 VIII、p. 82 的命题 3 的生成的 $A_M$ 模。因而，推论由上面注得出。

#### 推论 4 {#alg-viii-s5-thm-2-cor-4 .statement tag=005T}

每个有限生成模超过主理想整环都是平衡的。

事实上，有限生成模 M 超过主理想整环 A 是生成的 $A_M$-模（VIII，p. 81，例 4）。

#### 推论 5 {#alg-viii-s5-thm-2-cor-5 .statement tag=005U}

令 K 为交换域，K 上的 V 有限维向量空间，以及 V 的 $u$ 和 $v$ 自同态。以下属性是等效的：

(i) K[X] 中存在多项式 P 使得 $v= P(u)$。

(ii) The endomorphism $v$ commutes with every endomorphism of V that commutes with $u$.

取A为环 K[X]，M为从V和$u$（VII, §5, No. 1，p. 28）推导出来的K[X]模。 断言 (i) 意味着$v\in K[X]_M$ 和 (ii) $v\in K[X]''_M$。因而，推论 5 是推论 4 的特例。

#### 命题 4 {#alg-viii-s5-prop-4 .statement tag=005V}

半单模与有限生成的对模是平衡的。

这是从VIII、p. 81 和注的例 3 得出的。

#### 推论 1 {#alg-viii-s5-prop-4-cor-1 .statement tag=005W}

令 $(S_i)_{i\in I}$ 为成对非同构单A-模的有限族。对于$i\in I$，用$S_i$ 自同态域 $D_i$ 逆环表示。假设对于每个$i\in I$，$D_i$向量空间$S_i$是有限维的。那么从A到$\prod_{i\in I}$End$_{D_i}(S_i)$的映射$a\mapsto (a_{S_i})_{i\in I}$是满射。

考虑A-模$M =\prod_{i\in I}S_i$。由于I是有限的，所以我们也有$M =\bigoplus_{i\in I}S_i$，并且M中$S_i$的像是型$S_i$的M的同型分量。因而，A-模 M 的自同态为映射 $(s_i)\mapsto (s_id_i)$，其中$(d_i)_{i\in I}$ 穿过$\prod_{i\in I}D_i$（VIII、p. 66、命题 5）。由于I是有限的，并且对于每个$i\in I$，右$D_i$向量空间$S_i$是有限维的，M的对模是有限生成的。到命题 4，A-模 M 达到平衡。现在，A-模 M 的双交由形式 $\prod_{i\in I}u_i$ 的 End$_{\mathbf{Z}}(M)$ 的元素组成，其中 $(u_i)\in \prod_{i\in I}$ End$_{D_i}(S_i)$ (VIII, p. 78, 命题 1) 因为End$_{D_i}(S_i)$ 是$S_i$ 的二交换数。由此得出推论。

这个推论尤其适用，当 A 是代数超过交换域 K 并且每个 $S_i$ 是单A-模时，它是有限维的 K-向量空间：事实上，$D_i$ 然后包含同位$\alpha_{S_i}$，其中 $\alpha$ 穿过 K，并且$S_i$ 在 $D_i$ 上是有限维的，因为它在 K 上也是有限维的。

#### 推论 2（伯恩赛德定理）{#alg-viii-s5-prop-4-cor-2 .statement tag=00S0}

设 A 为代数闭交换域 K 上的代数，并令 S 为单A-模，其有限维为 K-向量空间。那么从 A 到 End$_K(S)$ 映射 $a\mapsto a_S$ 是满射。

事实上，A-模 S 的自同态的域由同位$\alpha_S$ 与 $\alpha \in K$ (VIII、p. 47、定理 1) 组成。然后我们将推论 1 应用于单A-模 S。

### 4. 对模 / 半单模

设 A 为环。用$\mathscr{S}$表示单A-模的类的集合。对于每个$\lambda \in \mathscr{S}$，类$\lambda$的选择单A-模$S_{\lambda}$，并用$D_{\lambda}$表示$S_{\lambda}$的自同态域逆环。我们将$S_{\lambda}$视为$(A,D_{\lambda}$)-双模。

设M为半单A-模，设B为M的自同态环。用C表示M的二交换数。对于每个 $\lambda \in \mathscr{S}$，用 $V_{\lambda}$ 表示左侧 $(D_{\lambda}$，B)-双模 Hom$_A(S_{\lambda},M)$。最后，用$\mathscr{S}_M$(VIII,p. 66)表示A-模M的支持度；它也是元素 $\lambda$ $\mathscr{S}$ 的集合，使得 $V_{\lambda}$ 是非零的。

#### 注 1 {#alg-viii-s5-n4-rem-1 .statement tag=00R4}

A-模 M 的规范描述 $\alpha_M$ 是左$(A$ 的同构，B)-双模。根据命题 9, VIII, p. 71, 映射 $f\mapsto ($Hom(1$_{S_{\lambda}}, f$))$_{\lambda\in\mathscr{S}_M}$从B到$\prod_{\lambda\in\mathscr{S}_M}$End$_{D_{\lambda}}(V_{\lambda})$的推论是环同构。

#### 命题 5 {#alg-viii-s5-prop-5 .statement tag=005X}

a) M 的对模是半单。

b) 对于每个 $\lambda \in \mathscr{S}_M$，B-模 $V_{\lambda}$ 都是简单的，其交换子等于 $(D_{\lambda})_{V_{\lambda}}$。

c) 映射 $\lambda \mapsto$ cl(V$_{\lambda}$) 是双射从A-模 M 的支持到其对模的支持。

d) 对于每个$\lambda \in \mathscr{S}_M$，B-子模$M_{\lambda}$是B-模M的型$V_{\lambda}$的同型分量，并且M中$V_{\lambda}$的重数等于dim$_{D_{\lambda}}(S_{\lambda})$。

e) 对于$s\in S$，用$\widetilde{s}$表示从$V_{\lambda}=$Hom$_A(S_{\lambda},M)$到M的映射$\varphi \mapsto \varphi (s)$。它是 B 线性的。从$S_{\lambda}$到Hom$_B(V_{\lambda},M)$的所得的映射$s\mapsto \widetilde{s}$是$(A,D_{\lambda})$双模的同构。

让$\lambda \in \mathscr{S}_M$。用$E_{\lambda}$表示环结束$_{D_{\lambda}}(V_{\lambda})$；由于$V_{\lambda}$是非零的$D_{\lambda}$向量空间，它是一个简单的$E_{\lambda}$模，(VIII，p. 45，例3)，其交换子等于$(D_{\lambda})_{V_{\lambda}}$(VIII， p. 82，定理 2 的推论 1）。由于$E_{\lambda}$是B-模$V_{\lambda}$同位的环（VIII，p. 71，命题9的推论），这就证明了b)。

M 定义同构 $\alpha_{\lambda}$ 从 $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ 到 $M_{\lambda}$ 的规范描述 $\alpha_M$。由于$V_{\lambda}$是单B-模，B-模$V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$是型$V_{\lambda}$的同型（VIII，p. 61，命题1）；因此，同样适用于B-模$M_{\lambda}$，这证明了a)。

由上面的注 1，存在B的元素$e_{\lambda}$，对于$\lambda$穿过$\mathscr{S}_M$，使得对于$\mu\in \mathscr{S}_M$和$\mu\not=\lambda$来说$(e_{\lambda})_{V_{\lambda}}= 1_{V_{\lambda}}$和$(e_{\lambda})_{V_\mu}$ = 0。因此单B-模$V_{\lambda}$是成对非同构的，这证明了c)和d)的第一个断言。 B-模$M_{\lambda}$与$V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$同构，因此dim$_{D_{\lambda}}(S_{\lambda})$是M中$V_{\lambda}$的重数（II, §3, No. 7，p. 255，推论1）。

映射$\sum_{\lambda\in\mathscr{S}_M}\alpha_{\lambda}$从$\bigoplus_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$到M提供半单B-模M的描述（VIII，p. 69，定义5）。到VIII，p. 70，命题 8，b)，对于e)中描述的从$S_{\lambda}$到Hom$_B(V_{\lambda},M)$的每个$\lambda \in \mathscr{S}_M$，映射是双射且$D_{\lambda}$线性的。由于它显然是 A 线性的，因此证明了 e)。

#### 注 2 {#alg-viii-s5-n4-rem-2 .statement tag=00R5}

由证明得出映射

$$
\sum_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}\longrightarrow M
$$

由M的规范描述引起的是M的对模的描述。

#### 命题 6 {#alg-viii-s5-prop-6 .statement tag=005Y}

a) 将 M 视为 $(A,B^o)$ 双模，M 为半单。

b) 对于每个 $\lambda \in \mathscr{S}_M,M_{\lambda}$ 都是 M 的简单 $(A,B^o)$ 子双模。

c) 对于 M 的每个 $(A,B^o)$-子双模 N，都存在 $\mathscr{S}_M$ 的唯一子集 Λ，使得 N 等于 $\oplus_{\lambda\in\Lambda}M_{\lambda}$。

设$\lambda$在$\mathscr{S}_M$中。 左A-模$S_{\lambda}$和右B-模$V_{\lambda}$简单，$D_{\lambda}$是$S_{\lambda}$自同态域逆环。根据VIII、p. 63的推论2，$(A,B^o$)双模$S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$很简单，$M_{\lambda}$也是简单的，与其同构。这证明了b)，并且a)如下。

如果 $\lambda$ 和 $\mu$ 在 $\mathscr{S}_M$ 中不同，则 $M_{\lambda}$ 和 $M_\mu$ 不与 A-模同构，更不必说也不与 $(A,B^o$) 双模同构。 断言 c) 由VIII、p. 68 的推论 2 得出。

#### 命题 7 {#alg-viii-s5-prop-7 .statement tag=005Z}

a) For every element $c$ of the bicommutant C of M and every $\lambda \in \mathscr{S}_M$, there exists a unique element $c_{\lambda}$ of End$_{D_{\lambda}}(S_{\lambda})$ such that for every $\varphi \in$ Hom$_A(S_{\lambda},M)$ and every $s\in S_{\lambda}$, we have $c\varphi (s) =\varphi (c_{\lambda}s)$.

b) 赋予$S_{\lambda}$（对于贯穿$\mathscr{S}_M$的$\lambda$），具有由a)定义的C模块结构。那么从$\bigoplus_{\lambda\in\mathscr{S}_M}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$到M的典范映射$\alpha_M$是$(C,B^o)$双模的同构。

c) 从C到$\prod_{\lambda\in\mathscr{S}_M}$结束$_{D_{\lambda}}(S_{\lambda})$，映射$c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$是同构。

断言 a) 和 c) 从 VIII、p. 71、命题 9 得出，因为从 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ 到 M 的典范映射 $\alpha_M$ 提供了 B-模 M (注 2) 的描述。此外，$\alpha_M$是$(C,B^o$)-线性，这证明了b)。

#### 注 3 {#alg-viii-s5-n4-rem-3 .statement tag=0060}

赋予$S_{\lambda}$，对于$\lambda \in \mathscr{S}_M$，具有由命题7，a)给出的C模块结构。如果我们在命题 5 中替换 A 与 B 以及 B 与 C (VIII, p. 85)，那么我们看到对于每个 $\lambda \in \mathscr{S}_M$，左边的 C-模$S_{\lambda}$ 是简单的，有交换律 $D_{\lambda}$， C模块M的型$S_{\lambda}$的同典型分量等于$M_{\lambda}$，并且映射$\lambda \mapsto$cl$_C(S_{\lambda})$从A-模M的支撑到双射的支撑C-模 M。最后，观察从 $S_{\lambda}$ 到 M 的 A-线性映射和 C 线性映射是相同的，M 的 A-子模和 C 子模也是相同的，并且环 End$_A(M)$ 和 End$_C(M)$ 相等。

令 M 为半单A-模。用A-模M的双交换子C的Z中心表示；它也是 M 的交换子 B 的中心。赋予 M 和 $S_{\lambda}$，对于 $\lambda \in \mathscr{S}_M$，Z 模结构由 C 模结构中的标量限制推导出来。对于每个$\lambda \in \mathscr{S}_M$，用$Z_{\lambda}$表示域$D_{\lambda}$中的中心。

#### 命题 8 {#alg-viii-s5-prop-8 .statement tag=0061}

a) 映射 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ 是域 $Z_{\lambda}$ 中从 Z 到乘积的同构。

b) A-模 M 是同型的且非零的当且仅当 Z 是域。

c) 令 Λ 为子集或 $\mathscr{S}_M$。用Z的$e_{\Lambda}$唯一元素表示，使得$(e_{\Lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$代表$\lambda \in \Lambda$，$(e_{\Lambda})_{S_{\lambda}}= 0$代表$\lambda \in \mathscr{S}_M-\Lambda$。我们有 $(e_{\Lambda})_{M_{\lambda}}= 1_{M_{\lambda}}$ 对应 $\lambda \in \Lambda$，$(e_{\Lambda})_{M_{\lambda}}= 0$ 对应 $\lambda \in \mathscr{S}_M-\Lambda$。

d) 如果M的支持度$\mathscr{S}_M$是有限的，则映射$\Lambda \mapsto e_{\Lambda}Z$从$\mathscr{S}_M$的子集的集合到Z理想的集合为双射，并且映射从Z理想的集合到M的$(A,B^o)$子双模的集合，$\mathfrak{a}\mapsto \mathfrak{a}M$是双射。这些双射是有序集的同构。反向双射将M的$(A,B^o)$子双模N发送到Z的元素$z$的理想由……组成，将N发送到M中。

对于$\lambda \in \mathscr{S}_M, Z_{\lambda}$来说，是交换子$D_{\lambda}$的公共中心，以及A-模$S_{\lambda}$的双交换子$C_{\lambda}$。根据上述命题 7, c)，从 C 到 $\prod_{\lambda\in\mathscr{S}_M}C_{\lambda}$，映射 $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ 为同构。通过限制到中心，我们从Z到$\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$，从而得到同构$z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$，从而a)。

环$\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$是域当且仅当集合$\mathscr{S}_M$有一个元素，从而b)。

断言 c) 由命题 7, a) 得出。假设 $\mathscr{S}_M$ 是有限的。由a)和I, §8, No. 10、p. 109的命题 8得出，映射$\Lambda \mapsto e_{\Lambda}Z$是从Z理想的$\mathfrak{P}(\mathscr{S}_M)$到集合的有序集的同构。令Λ为子集 $\mathscr{S}_M$。到c)，我们有关系 $e_{\Lambda}$ZM $=e_{\Lambda}M =$ $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$；因为命题 6, c) of VIII, p. 86，所以剩下来描述逆双射。但是$z\in Z$将M发送到$\bigoplus_{\lambda\in\Lambda}M_{\lambda}$当且仅当$z=e_{\Lambda}z$，即$z\in e_{\Lambda}Z$。

#### 推论{#alg-viii-s5-n4-cor-1 .statement tag=0062}

假设 A 是代数闭交换域 K 上的代数，M 是半单A-模，即 K 上的向量空间有限维。对于 $\mathscr{S}_M$ 中的每个 $\lambda$，用 M 的 $e_{\lambda}$ 投影算子和像 $M_{\lambda}$ 表示和核$\oplus_{\lambda\not=\mu}M_\mu$。那么$(e_{\lambda})_{\lambda\in\mathscr{S}_M}$是向量空间Z在K上的基。

由于 M 在 K 上是有限维向量空间，即非零的子模 $(M_{\lambda})_{\lambda\in\mathscr{S}_M}$ 族的直和，因此集合 $\mathscr{S}_M$ 是有限的，并且对于 $\lambda \in \mathscr{S}_M$，空间 $S_{\lambda}$ 中的每一个都是 K 上的有限维。 域 K 是代数闭集，我们有 $D_{\lambda}= Z_{\lambda}= K$ (VIII, p. 47, 定理 1)，并且映射 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ 是从 Z 到 $K^{\mathscr{S}_M}$ (命题 8, a)) 的同构。然后从命题 8 的部分 c) 得出推论。

### 5.稠密性定理

#### 定理 3（雅各布森）{#alg-viii-s5-thm-3 .statement tag=00S1}

设M为半单A-模，$c$为加法群M的自同态。则$c$属于为M的二共交$A''_M$当且仅当满足以下条件：

(D) 对于 M 的每个有限子集 F，存在 A 的元素 $a$，使得 $c$ 重合且 F 上有 $a_M$。

首先，假设$c$满足条件(D)。令$u$为$A'_M$的元素。令$x$为M的元素，并将条件(D)应用于子集$F =\{x, u(x)\}$。 A 存在元素$a$，使得$c(x) =ax$和$c(u(x)) =au(x)$，因此$u(c(x)) =u(ax) =au(x) =c(u(x))$。由于$x$是任意的，所以我们有$cu=uc$；因为这对于所有$u$都成立，所以我们有$c\in A''_M$。

对于逆命题，我们使用以下引理。

#### 引理 3 {#alg-viii-s5-lem-3 .statement tag=0063}

设M为半单A-模。设 B 为 A-模 M 的二交矩阵。则 M 的每个 A-子模都是 M 的 B-子模。

令N为M的A-子模。由VIII、p. 56的推论2，存在A-模M与像N的投影算子$p$；它从属于到$A'_M$。由于对于每个 $b\in B$，我们都有关系 $pb=bp$，因此我们得出 N 是 M 的 B-子模。

让我们定理的结论证明 3. 假设 $c$ 属于到 $A''_M$，并令 F = $\{x_1, . . . , x_n\}$ 为 M 的有限子集。 将 $M^n$ 的元素 $(x_1, . . . , x_n)$ 表示为$x$。 A-模$M^n$是半单，并且通过VIII的命题2，得到p. 79，其双交换体重合与$A''_M$模$M^n$的同调。到引理 3，$M^n$的A-子模$Ax$是$M^n$的$A''_M$子模块。令 $a\in A$ 使得 $(cx_1, . . . , cx_n)$ 等于 $ax$。然后$c$重合与$a_M$在$\{x_1, . . . , x_n\}$上，这意味着条件（D）。

#### 注 {#alg-viii-s5-n5-rem-1 .statement tag=0064}

用E表示M的加法群的自同态环。赋予M离散的拓扑； 环 E 由从 M 到 M 的映射组成，我们可以赋予它由乘积拓扑在 $M^M$ 上诱导的拓扑（“M 中简单收敛的拓扑”，Gen. Top.，I, §2, No. 3， p. 31）。 E 上的拓扑是 Hausdorff，并且与 E 上的加法群结构兼容。对于 E 中的每个 $f$，从 E 到 E 的映射 $g\mapsto f\circ g$ 和 $g\mapsto g\circ f$ 是连续的。因而，E 的每个子集的交换子在 E 中都是闭集。因而，定理 3 意味着$A''_M$ 是 E 中$A_M$ 的闭集。

### 6. 域理论的应用

#### 命题 9 {#alg-viii-s5-prop-9 .statement tag=0065}

令L为域，且End$_{\mathbf{Z}}(L)$的E子环，对于每个$a\in L$，包含映射$\boldsymbol{\gamma }_a:x\mapsto ax$。用元素 $a$ 的 K 集合 L 表示，使得 L 中的每个 $x$ 以及 E 中的每个 $u$ 都有$u(xa) =u(x)a$；是L中的子域。

令V为右K-向量空间L的有限维线性子空间，令$h$为从V到L的K-线性映射。 E 存在元素，重合与 $h$ 在 V 上。

我们将L视为左E模块。由于E 包含左乘法$\boldsymbol{\gamma }_a$，L的每个E子模都是域L的左理想；因而，E 模块L 很简单。与$\boldsymbol{\gamma }_a$通勤的L加法群每自同态是形式$\boldsymbol{\delta }_b:x\mapsto xb$与L中的$b$。因而，从K到End$_E$(L)的逆环，$b\mapsto \boldsymbol{\delta }_b$是同构，即域。

因而，E 模块 L 的双交换体 $E''$ 由右侧 K-向量空间 L 的自同态组成。设$v$为K-向量空间L中的自同态，其限制到V重合与$h$；是$E''$中的元素。设$(x_i)_{i\in I}$是K上V的基；通过定理 3 (VIII, p. 88)，存在 E 的元素 $u$，使得 $u(x_i) =v(x_i) =h(x_i)$ 对应 $i\in I$。根据线性关系，V 中的每个$x$ 都有$u(x) =h(x)$。

#### 推论{#alg-viii-s5-n6-cor-1 .statement tag=0066}

令L为域。令 Γ 为域 L 自同构群子群，并令 K 为 Γ 的不变量域。令 V 为 K 上有限维 $n$ 的 L 的右 K 线性子空间。则存在 Γ 的元素 $\sigma_1, . . . , \sigma_n$，其中性质：对于每个 K-线性映射 $u$从V到L，L中存在元素$a_1, . . . , a_n$，因此V中的每个$x$都有$u(x) =\sum_{i=1}^na_i\sigma_i(x)$。

用映射的E集合从L到形式$x\mapsto$$\sum_{\sigma\in\Gamma}a_{\sigma}\sigma (x)$的L表示，其中$(a_{\sigma})_{\sigma\in\Gamma}$是L的元素与有限支撑的族。对于L中的每个$a$，我们有$\boldsymbol{\gamma }_a\in E$，并且E是L的加法群自同态环子环。此外，域 K 由 L 的元素 $a$ 组成，使得 L 中的每个 $x$ 以及 E 中的每个 $u$ 都有 $u(xa) =u(x)a$。

设H为左L-向量空间Hom$_K(V,L)$；它有维数 $n$。到命题 9，由元素的限制到V生成。存在$n$元素$\sigma_1, . . . , \sigma_n$，其中H的限制到V形式基超过L。由此得出推论。

#### 注 {#alg-viii-s5-n6-rem-1 .statement tag=0067}

当域L可交换时，约化到Artin的定理（V, §10, No. 6，p. 65）的推论。

### 习题{#alg-viii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
