---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: The Structure of Modules of Finite Length
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.25-A VIII.43
pdf_pages: 0042-0060
extraction: native
subsections:
    - "no": 1
      title: Local Rings
      page: 25
      pdf_page: 42
    - "no": 2
      title: Weyr–Fitting Decomposition
      page: 27
      pdf_page: 44
    - "no": 3
      title: Indecomposable Modules and Primordial Modules
      page: 30
      pdf_page: 47
    - "no": 4
      title: Semiprimordial Modules
      page: 32
      pdf_page: 49
    - "no": 5
      title: The Structure of Modules of Finite Length
      page: 37
      pdf_page: 54
statements: 37
exercises: 20
content_sha256: 90b8e8832a8b4ad84907f47547cb33ef1cb04814448b58d95a660b37c212e1ac
translated_from: content/en/alg/VIII/02_s2_the_structure_of_modules_of_finite.md
translation_method: google
source_content_sha256: 937d6660bbf18635e63c4c1addfaf3e44ee88a5456fdc47cb5c2eacabc9099b5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-85fdfe71
glossary_version: 34
glossary_terms_sha256: 3dab4ce5372bf7025fbd92132afe829dda18a9ad01498abe4ed3a8d21ae06720
prompt_sha256: 133cd3fc3c262b082830ff023554f589fe553d569c36079625221572907a2124
---

## § 2。 结构模有限长度

### 1.局部环

#### 命题 1 {#alg-viii-s2-prop-1 .statement tag=001P}

设 A 为非零环，并令 $\mathfrak{r}$ 为 A 的不可逆元素的集合。以下属性是等效的：

(i) 集合 $\mathfrak{r}$ 是 A 的双面理想。

(ii) 集合 $\mathfrak{r}$ 在加法下稳定。

(iii) 环 A 有唯一的最大左理想。

(iv) 对于每个$a\in A$，元素、$a$和$1-a$之一是可逆的。

(v) 对于每个$a\in A$，元素、$a$和$1-a$之一保持可逆。

蕴涵 (i) $\Rightarrow$ (ii) 由理想的定义得出。由于 1 不属于到 $\mathfrak{r}$，所以我们有 (ii) $\Rightarrow$ (iv)。

我们有 $\mathfrak{r}\not= A$，以及集合 $\mathfrak{r}$ 包含于 A 不等于 A 的每个左理想。如果 $\mathfrak{r}$ 是 A 的左理想，那么它就是 A 的唯一最大左理想。这证明 (i) 蕴涵 (iii)。

假设 A 有唯一的最大左理想 $\mathfrak{m}$。取$b\in A-\mathfrak{m}$。左理想$Ab$不包含在A的任何最大左理想中，因此等于A（I, §8, No. 6，p. 104，定理1），并且$b$是左可逆的。对于每个$a\in A$，元素$a$和$1-a$属于之一到A$-\mathfrak{m}$，因为$\mathfrak{m}$是一个不包含1的理想。因此，(iii)意味着(v)。

假设性质 (v) 成立。令$b$为A的左可逆元。令$c\in A$使得$cb= 1$。我们有$(1-bc)b= 0$和$b\not= 0$；因此，$1-bc$ 不是可逆的。通过性质 (v)，$bc$ 保持可逆，并且更不必说、$c$ 保持可逆。但$c$是可逆的； $b$ 是它的逆元，因此 $b$ 是可逆的。由此可见，(v) 蕴涵(iv)。

仍有待证明 (iv) 蕴含 (i)。假设 (iv) 成立。那么 $\mathfrak{r}$ 是 A 的双面理想，由以下断言 a) 到 d) 表示：

a) 我们有$0\in \mathfrak{r}$，因为环 A 是非零的。

b) A 的两个元素中的乘积，一个属于至$\mathfrak{r}$，另一个至A $-\mathfrak{r}$，属于至$\mathfrak{r}$。

c) 集合 $\mathfrak{r}$ 在加法下稳定。

事实上，让$a$和$b$是$\mathfrak{r}$的元素，这样$s=a+b$是可逆的。 b)、属于至$\mathfrak{r}$中的元素$s^{-1}a$和$s^{-1}b$；从 $s^{-1}b= 1-s^{-1}a$ 开始，(iv) 成立的与……矛盾假设成立。

d) 集合 $\mathfrak{r}$ 在乘法下稳定。

事实上，让$a$和$b$是$\mathfrak{r}$的两个元素。 b) 元素 $a'=-a(1-b)$ 属于至 $\mathfrak{r}$，从而元素 $ab$，等于 c) 中的 $a+a'$、属于至 $\mathfrak{r}$； 断言d)如下。

#### 定义 1 {#alg-viii-s2-def-1 .statement tag=001Q}

局部环是非零环，具有与命题 1 等效的属性。

环 A 是局部的当且仅当逆环 $A^o$ 是局部的。

若A为局部环，则A的不可逆元素的集合$\mathfrak{r}$为A的双面理想；它包含 A 不等于 A 的每个左理想或右理想。因此环 $A/\mathfrak{r}$ 是域，我们称之为 A 的剩余类域。 集合 $\mathfrak{r}$ 是 A 的唯一最大左（右、两侧）理想；我们简单地说$\mathfrak{r}$是A的最大理想。

#### 例 1 {#alg-viii-s2-n1-exa-1 .statement tag=001R}

每个域都是局部环。

#### 例 2 {#alg-viii-s2-n1-exa-2 .statement tag=001S}

设 A 为非零环，其中每个元素都是可逆的或幂零的。那么A就是局部环。事实上，如果$a\in A$不可逆，那么到假设，存在整数$n\geqslant 0$使得$a^{n+1}= 0$，并且$1-a$有逆$1 +a+\cdots +a^n$。

#### 例 3 {#alg-viii-s2-n1-exa-3 .statement tag=001T}

令 X 为 $C^r$ 流形 (VAR, R, 5.1.5) 和 $x$ 点的 X。设$\mathscr{O}_x$为$C^r$函数$x$处的细菌环，值位于标量K的域中。则$\mathscr{O}_x$为交换局部环，其最大理想由

函数零 $x.*$ 的细菌

#### 例 4 {#alg-viii-s2-n1-exa-4 .statement tag=001U}

设 A 为形式幂级数的交换局部环和 $B = A[[X_i]]_{i\in I}$ 代数，系数为 A (III, §2, No. 11, p. 456)。由 IV, §4, No. 4、p. 30、环的命题 6 可知，B 是局部的，其最大理想由 A 的最大理想中的形式幂级数和常数项组成。特别是，如果 A 为域，则$A[[X_i]]_{i\in I}$ 由形式幂级数和常量项零组成。

#### 例 5 {#alg-viii-s2-n1-exa-5 .statement tag=001V}

设 $p$ 为素数数。我们用分数 $a/b$ 数由……组成域 $\mathbf{Q}$ $\mathbf{Z}_{(p)}$ 子环和 $a\in \mathbf{Z},b\in \mathbf{Z}$ 来表示，并且 $b$ 不能被$p*$(cf.整除)通讯，II, §2, No. 1，p. 60）。那么 $\mathbf{Z}$ 就是

$*(_{p)}$

交换局部环，极大理想$p\mathbf{Z}_{(p)}$。 $p$-adic 整数（V, §12, No. 3，p. 96）的环$\mathbf{Z}_p$为交换局部环，极大理想$p\mathbf{Z}_p$（VIII，p. 40，习题9）。

#### 例 6 {#alg-viii-s2-n1-exa-6 .statement tag=001W}

令 K 为特征 $p >0$ 的交换域，G 为$p$群（I, §6, No. 5、p. 76、定义 9）。 群 G 在 K (III, §2, No. 6, p. 446) 上的代数 K[G] 为局部环；它的最大理想是 K[G] 的元素 $(a_g)_{g\in G}$ 的集合，使得 $\sum_{g\in G}a_g= 0$ (VIII, p. 41, 习题 10)。

### 2.Weyr-Fitting 分解

设 A 为环、M A-模和 M 的 $u$ 自同态。对于任意整数 $p\geqslant 0$，我们用 $N_p$ 表示 $u^p$ 的核。 子模$(N_p)$的序列为递增，其并为在$u$下稳定的M的子模$N_{\infty}$。对于每个整数$p\geqslant 0$，我们有$N_{p+1}=\overset{-1}{u}(N_p)$，因此关系$N_p= N_{p+1}$意味着$N_{p+1}= N_{p+2}$。因而，要么序列$(N_p)$是严格递增的，要么存在整数$p\geqslant 0$使得$N_0, . . . ,N_p$不同且$N_p= N_{\infty}$。

对于任何整数$q\geqslant 0$，用$I_q$表示$u^q$的像。 子模$(I_q)$的序列为递减，其交为在$u$下稳定的M的子模$I_{\infty}$。对于每个整数$q\geqslant 0$，我们有$u(I_q) = I_{q+1}$，因此关系$I_q= I_{q+1}$意味着$I_{q+1}= I_{q+2}$。因而，要么序列$(I_q)$是严格递减，要么存在整数$q\geqslant 0$使得$I_0, . . . ,I_q$不同且$I_q= I_{\infty}$。

#### 命题 2 {#alg-viii-s2-prop-2 .statement tag=001X}

a) 假设序列 $(N_p)$ 是平稳的。那么我们有$N_{\infty}\cap I_{\infty}= 0$，$u$到$I_{\infty}$的限制是单射的，$N_{\infty}$的$u$诱导幂零自同态。

b) 假设序列 $(I_p)$ 是平稳的。那么我们有 M = $N_{\infty}+ I_{\infty}$ 和 $u(I_{\infty}) = I_{\infty}$。

c) （“Weyr-Fitting 分解”—有时称为“Fitting 分解”）假设序列$(N_p)$和$(I_p)$是静止的。那么M就是在$u$下稳定的子模、$N_{\infty}$和$I_{\infty}$的直和，以及$N_{\infty}$的$u$、诱导幂零自同态和$I_{\infty}$的自同构。

令$p$为自然数，使得$N_p= N_{\infty}$，并令$v=u^p$。通过构造，$v$和$v^2$具有相同的核$N_{\infty}$，$I_p$是$v$的像。对于$N_{\infty}\cap I_p$中的$x$，存在$y\in M$，使得$x=v(y)$，因此存在$v^2(y) =v(x) = 0$；因而，我们有$y\in N_{\infty}$，因此有$x= 0$。特别是，我们有$N_{\infty}\cap I_{\infty}= 0$。由于$u$的核$N_1$包含在$N_{\infty}$中，因而$u$到$I_{\infty}$的限制是单射的；另一方面，我们有$u^p(N_{\infty}) = 0$。这就证明了a）。

令$q$为自然数，使得$I_q= I_{\infty}$，并令$w=u^q$。那么$w$和$w^2$有相同的像$I_{\infty}$，$N_q$是$w$的核。让$x\in M$。我们有$w(x)\in I_{\infty}$，所以存在$y\in M$使得$w(x) =w^2(y)$；然后我们有$x-w(y)\in N_q$，从而$M = N_q+ I_{\infty}$和更不必说$M = N_{\infty}+ I_{\infty}$。我们有$u(I_{\infty}) =u(I_q) = I_{q+1}= I_{\infty}$。这证明了b)。

断言 c) 紧随 a) 和 b)。

#### 注 1 {#alg-viii-s2-n2-rem-1 .statement tag=001Y}

令$p$为整数，使得$N_p= N_{p+1}$；上面给出的证明表明，$u$到$I_p$的$N_{\infty}\cap I_p= 0$和限制是单射的。 同样，令$q$为整数，使得$I_q= I_{q+1}$；那么我们有$N_q+ I_{\infty}= M$，并且$M/N_q$从$u$通过经过推导出自同态，商是满射的。

#### 注 2 {#alg-viii-s2-n2-rem-2 .statement tag=001Z}

假设M是在$u$下稳定的两个子模N和I中的直和，并且N中的$u$诱导幂零自同态$u_N$和I中的自同构。然后我们有 $N_{\infty}= N$ 和 $I_{\infty}= I$，并且序列 $(N_p)$ 和 $(I_p)$ 是静止的。此外，以下整数是相等的：

$\alpha )$ 至少整数 $p\geqslant 0$ 使得$N_p= N_{\infty}$，

$\beta )$ 至少整数 $q\geqslant 0$ 使得$I_q= I_{\infty}$，

$\gamma )$ 至少整数$r\geqslant 0$使得$(u_N)^r= 0$。

#### 注 3 {#alg-viii-s2-n2-rem-3 .statement tag=0020}

如果A-模 M 为诺特，则满足断言 a) 的假设；如果M是阿廷的，则满足断言b)的假设； VIII、p. 2、断言的命题 1、假设 c) 如果 M 具有有限长度，则满足。

#### 推论 1 {#alg-viii-s2-prop-2-cor-1 .statement tag=0021}

设A为环，设M为A-模。

a) 如果模 M 是诺特，则M 的每个满射自同态都是双射的。

b) 如果模 M 是阿廷的，则M 的每个单射自同态都是双射的。

c) 如果模 M 具有有限长度，则 M 的每个单射或满射自同态都是双射的。

d) 如果环 A 是可交换的并且 A-模 M 是有限生成的，则 M 的每个满射自同态都是双射的。

令$u$为A-模M的自同态。我们使用在小节开头介绍的记号。如果自同态 $u$ 是满射，那么我们有 $I_{\infty}= M$。 断言 a) 然后从命题 2, a) 和注 3 得出。同样，如果自同态 $u$ 是单射的，我们有 $N_{\infty}= 0$。因此，断言 b) 由命题 2、b) 和注 3 得出。断言 c) 紧随a) 和b) 得出。

Now, suppose that 环 A is commutative, A-模 M is finitely generated, and 自同态 $u$ is surjective.让我们证明 $u$ 是单射的。令 $x$ 为 M 的元素，使得 $u(x) = 0$。 选择有限生成 family $(x_i)_{i\in I}$ of A-模 M and, for every $i\in I$, 元素 $y_i$ of M such that $u(y_i) =x_i$. There exist families $(a_i)_{i\in I}, (b_{ij})_{(i,j)\in I\times I}$, and $(c_{ij})_{(i,j)\in I\times I}$ of 元素 of A such that we have

$$
x=\sum_{i\in I}a_ix_i,y_j=\sum_{i\in I}b_{ij}x_i,u(x_j) =\sum_{i\in I}c_{ij}x_i
$$

对于每个$j\in I$。令$A'$为包含元素$a_i,b_{ij}$的诺特子环，以及$c_{ij}$（VIII，p. 12，推论3）。令$M'$为$(x_i)_{i\in I}$族生成的M的$A'$子模。我们有$u(x_j)\in M',y_j\in M'$，每个$j\in I$有$u(y_j) =x_j$； hence $u$ 定义, by 限制, 满射自同态 $u'$ of the $A'$-module $M'$.由于环$A'$是诺特，有限生成的$A'$模$M'$是诺特（VIII，p. 7，命题 4 a））。 By a), 自同态 $u'$ of $M'$ is bijective. By 构造, $x$ 属于 to $M'$, and we have $u'(x) =u(x) = 0$.因此我们有 $x= 0$，这证明了 d)。

#### 推论 2 {#alg-viii-s2-prop-2-cor-2 .statement tag=0022}

In 左诺特环, every left or right 可逆元 is invertible.

事实上，考虑左诺特环 A 的元素 $x,y$ 使得$xy= 1$。 Denote by $\boldsymbol{\delta }(x)$ and $\boldsymbol{\delta }(y)$, respectively, 自同态 $a\mapsto ax$ and $a\mapsto ay$ of A-模 $A_s$.我们有$\boldsymbol{\delta }(y)\circ \boldsymbol{\delta }(x) = 1_{A_s}$；因此 $\boldsymbol{\delta }(y)$ 是满射的。根据推论 1, a)，$\boldsymbol{\delta }(y)$ 是双射的。 自同态 $\boldsymbol{\delta }(x)$ is then 逆双射 of $\boldsymbol{\delta }(y)$, and we have $yx= (\boldsymbol{\delta }(x)\circ \boldsymbol{\delta }(y))(1) = 1$.推论如下。

### 3.不可分解模和原始模

设 A 为环。 Recall the following 定义 (VII, §4, No. 8, p. 23, 定义 3).

#### 定义 2 {#alg-viii-s2-def-2 .statement tag=0023}

A-模 M is called indecomposable if it is not 直和 of a family of 子模 distinct from 0 and M.

By the corollary of 命题 12 of II, §1, No. 8, p. 209, the following properties are equivalent:

a) A-模 M 不可分解。

b) A-模 M is 非零的, and every 直因子子模 of M is equal to 0 or M.

c) A-模 M is 非零的, and 环 End$_A(M)$ 包含 no idempotent disctinct from 0 and $1_M$.

特别是，由于A-模$A_s$的自同态环与A的逆环同构，我们看到A-模$A_s$不可分解当且仅当环A是非零的它的幂等性只有 0 和 1。

#### 例 {#alg-viii-s2-n3-exa-1 .statement tag=0024}

假设环 A 是主理想整环。不可分解的有限生成A-模 A-模同构于 A 或 $A/p^nA$，其中 $p$ 是 A 的不可约元，$n$ 整数 $>0$ (VII, §4, No. 8, p. 24, 命题8)。

#### 命题 3 {#alg-viii-s2-prop-3 .statement tag=0025}

诺特 or 阿廷的 A-模 M is 直和 of a finite family of indecomposable 子模.

Let us first prove that every 非零的子模 P of M has an indecomposable 直因子. If this were not the case, then every 直因子子模 of P would be decomposable;继续进行归纳，然后我们可以对P的每个$n\in \mathbf{N}$，非零的，子模，$N'_n$和$N''_n$进行构造，使得对于$n\geqslant 1$有$P = N'_0\oplus N''_0$和$N'_{n-1}= N'_n\oplus N''_n$。 But then, 序列 of 子模 $N''_0+\cdots + N''_n$ would be 严格递增的, and that of 子模 $N'_n$ would be 严格递减. 模 M would be neither 诺特 nor 阿廷的, contrary to 假设.

现在，假设 M 不是不可分解的子模有限族中的直和。到归纳，对于每个$n\in \mathbf{N}$，我们构造不可分解M的子模$P''_n$和M的非零的子模$P'_n$，这样$M = P'_0\oplus P''_0$和$P'_{n-1}= P'_n\oplus P''_n$对于$n\geqslant 1$。事实上，M 是非零的，证明的第一个部分应用于 P = M，提供$P'_0$ 和 $P''_0$。由于模$P'_k$和$P''_k$是为$k < n$定义的，通过证明的第一个部分，存在子模、$P'_n$和$P''_n$，使得$P'_{n-1}= P'_n\oplus P''_n$和$P''_n$不可分解的。 关系$M = P'_n\oplus P''_0\oplus  \cdots  \oplus P''_n$则意味着$P'_n\not= 0$，因为M不是不可分解模有限族中的直和。

子模$P''_0\oplus  \cdots  \oplus P''_n$中的序列是严格递增的，子模$P'_n$中的序列是严格递减。这个与……矛盾假设M就是诺特或者阿廷的。

模分解唯一性与不可分解的子模直和的问题将在接下来的小节中研究。

#### 定义 3 {#alg-viii-s2-def-3 .statement tag=0026}

如果自同态环是本地的，则模称为原始[^1]。

到定义时，局部环并未减至0；因而，原初模是非零的。此外，当且仅当环 A 是局部的时，A-模 $A_s$ 才是原初的。

#### 命题 4 {#alg-viii-s2-prop-4 .statement tag=0027}

a) 原初模是不可分解的。

b) 有限长度中的不可分解模是本初的。

设 M 为 A-模。假设M是原初的；令$e$在局部环End$_A(M)$中幂等。由于$e^2=e$，$e$是可逆的，我们有$e= 1$，或者$1-e$是可逆的，我们有$e= 0$。这证明M是不可分解的（VIII，p. 30）。

现在，假设 M 不可分解且为有限长度。由VIII、p. 27的命题2、c)，M的每一个自同态都是可逆的或幂零的；因而，环End$_A(M)$是VIII、p. 26中的例2的局部。

$\mathbf{Z}$-模块$\mathbf{Z}$不可分解，诺特，但阿廷的不可分解。它的自同态环与 $\mathbf{Z}$ 同构的，因此不是局部的。因而，$\mathbf{Z}$不是原始的$\mathbf{Z}$模块。

$*$设$p$为素数数。 $\mathbf{Z}$模块$\mathbf{Q}_p/\mathbf{Z}_p$的自同态环同构于局部环$\mathbf{Z}_p$（cf.VII, §4、p. 65、习题13）；因此它是一个原始的 $\mathbf{Z}$ 模块。

单射模不可分解当且仅当它是原初 (X, §1, n$^o9$, p. 21, 命题 $14$)$.*$

### 4.半原始模

#### 定义 4 {#alg-viii-s2-def-4 .statement tag=0028}

如果模是原始子模族中的直和，则称模为半原始的。

#### 例 1 {#alg-viii-s2-n4-exa-1 .statement tag=00SE}

$*$每个单模都是原始的（VIII，p. 45）；因而，每个半单模都是半原始的（VIII，p. 55，定义1）。

#### 例 2 {#alg-viii-s2-n4-exa-2 .statement tag=01L7}

如果 A 是左诺特环，则每个单射A-模都是半原初的（X, §1、n$^o9$、p. 21、命题 14 和 X, §1、n$^o10$、p. 22、定理） 3、b)).$*$

#### 定理 1（东屋）{#alg-viii-s2-thm-1 .statement tag=00RX}

设A为环，L为原初A-模，M为半原初A-模。存在一个唯一的基数，记为[M : L]，其性质如下：

对于 M 的每个分解 $M =\bigoplus_{i\in I}M_i$ 作为原初模的直和，指标 $i\in I$ 的集合，使得 $M_i$ 同构于 L 有基数 [M ： L]。

证明是基于以下四个引理。

#### 引理 1 {#alg-viii-s2-lem-1 .statement tag=0029}

设M为M的A-模，M的$M'$原始子模，以及M的$M''$子模，对$M'$的补充。设$u$为M的自同态。则M的$u$或$1_M-u$诱导同构从$M'$到子模补充$M''$。

令$p$为从M到$M'$的投影以及核$M''$，并令$v$为$p\circ u$到$M'$的限制。首先，假设$v$是$M'$的自同构。由于$v$是单射的，$u$到$M'$的限制是单射的，我们有$u(M')\cap M''= 0$。由于$v$是满射，我们有$u(M')\oplus M''= M$。因而，从$M'$到子模，$u$诱导同构是M中$M''$的补充。现在，假设$v$不是$M'$的自同构。那么$1_{M'}-v$是$M'$的自同构，因为$M'$是本初的。现在，$1_{M'}-v$是$p\circ (1_M-u)$到$M'$的限制。前面的推理证明了M对$M''$的补充从$M'$到子模的$1_M-u$诱导同构。

#### 引理 2 {#alg-viii-s2-lem-2 .statement tag=002A}

令M为A-模，即原始子模的$(M_i)_{i\in I}$家庭的直和，并令$u$为M的自同态。对于每个子集J，集合$v= 1_M-u$和$M_J=\bigoplus_{i\in J}M_i$ I。然后是以下两个性质成立之一：

a) 存在指标$i\in I$，使得M的$M_i$到直因子子模存在$u$诱导同构。

b) 对于从$M_J$到子模的I$,v$诱导同构的每个有限子集J，作为$M_{I-J}$的补充。

如果性质 b) 成立，则 $v$ 是单射的。

假设性质 a) 不成立，让我们在 J 基数上通过归纳建立性质 b)。如果 $J =\emptyset$ 则无需证明。因而，假设J是J的非空、选择元素$i$、以及集合$J'= J-\{i\}$。由M的归纳假设、$v$诱导同构从$M_{J'}$到子模补充$M_{I-J'}= M_{I-J}\oplus M_i$；因而，子模$M''=v(M_{J'})\oplus M_{I-J}$是$M_i$的补充。由$u$的引理 1和假设、$M_i$至子模的自同态$v$诱导同构补充$M''$；因而，$v$诱导同构从$M_J= M_i\oplus M_{J'}$到子模是对$M_{I-J}$的补充。

最后一个断言源自以下事实：M是子模$M_J$的并，其中J穿过I的有限子集。

#### 引理 3 {#alg-viii-s2-lem-3 .statement tag=002B}

设M为A-模，即原始子模的家庭$(M_i)_{i\in I}$的直和，并令$p$为M的非零的投影算子。存在指标$i\in I$使得$p$诱导同构从$M_i$到直因子子模共$p(M)$。

由于 $p$ 是非零的，因此 $1_M-p$ 不是单射的。到引理 2，存在指标 $i\in I$，使得 M 的 $M_i$ 到直因子子模 $p$ 诱导同构。M 的每个投影算子与像 $p(M_i)$ 定义、限制、$p(M)$的投影算子和像$p(M_i)$，所以$p(M_i)$是$p(M)$的直因子子模。

#### 引理 4 {#alg-viii-s2-lem-4 .statement tag=002C}

设M为A-模，即原始子模的$(M_i)_{i\in I}$家族的直和，令L为原初A-模，令N为M的直因子子模。假设N为$(N_j)_{j\in J}$家族的直和子模与L同构，并用指标$i\in I$的$I_L$集合表示，使得$M_i$与L同构。然后我们有

(1)卡片(J)$\leqslant$卡片(I$_L$)。

设$N_0$是M对N的补充的子模。模M是$N_0$和家庭$(N_j)_{j\in J}$的直和。对于每个 $j\in J$，用 M 的 $p_j$ 投影算子表示，其中像 $N_j$ 与此分解相关（II, §1, No. 8、p. 209、命题 12）。对于每个$i\in I$，用指标$j\in J$的$J(i)$集合表示，使得$p_j$诱导同构从$M_i$到$N_j$。这个集合是有限的：事实上，如果$x$是$M_i$的非零元素并且K是J的有限子集，使得$x$属于到$N_0+\sum_{k\in K}N_k$，那么我们有$j\in J$的$p_j(x) = 0$- K，使得 $J(i)$ 包含在 K 中。

让$j\in J$。到引理 3，存在指标$i\in I$，使得$N_j$从$M_i$到直因子子模有$p_j$诱导同构。由于 $M_i$ 是非零的并且 $N_j$ 是原初的，因此不可分解（VIII、p. 31、命题 4），所以我们有 $p_j(M_i) = N_j$ 和 $j$ 属于 $J(i)$。由于模$M_i$同构于$N_j$，因此也与L同构，指标$i$属于同构于$I_L$。这证明J是有限族集合$(J(i))_{i\in I_L}$的并。如果集合 J 无穷大，则集合 $I_L$ 无穷大，我们有 (集合理论，III, §6, No. 3，p. 188，推论 3)

卡(J)$\leqslant \sum_{i\in I_L}$卡(J($i$))$\leqslant$卡(I$_L$)。

现在，假设集合 J 是有限的，让我们在 J 的基数上用归纳证明引理。如果 J 为空，则无需证明。因此，假设J为非空，J的选择元素$j$。由上式可知，从$M_i$到$N_j$，存在指标$i\in I_L$使得$p_j$诱导同构。 集合$I'= I-\{i\}$和$J'= J-\{j\}$。 模 M 是$M_i$ 的直和和$p_j$ 的核。它也是$M_i$和子模$M'=\oplus_{i'\in I'}M_{i'}$的直和。因此，从 Ker $p_j= N_0\oplus_{j'\in J'}N_{j'}$ 到$M'$，存在（II, §1, No. 9，p. 210，命题 13 的推论）同构 $\varphi$。 集合$N'=\varphi (\sum_{j'\in J'}N_{j'})$。 $M'$的子模$N'$是直因子并且是原始子模的$(\varphi (N_{j'}))_{j'\in J'}$族的直和与L同构。让我们将归纳假设应用于 $M'$ 和 $N':$，我们有 Card(J$'$)$\leqslant$ Card(I$_L-\{i\}$)，因此不等式 (1)。

让我们证明定理 1。令$(M_i)_{i\in I}$和$(N_j)_{j\in J}$是原始子模与直和M的两个族。令$I_L$（或$J_L$）是$i\in I$（或$j\in J$）的集合，使得$M_i$（分别为$N_j$）与L同构。我们通过引理 4 得到 Card(J$_L$)$\leqslant$ Card(I$_L$)。通过交换 I 和 J 的角色，我们得到逆不等式，从而得到定理。

定理 1 中定义的基数 [M : L] 在 M 中称为 L 的原始重数。

#### 推论 1 {#alg-viii-s2-lem-4-cor-1 .statement tag=002D}

设 M 和 N 为半原始模。那么 M 和 N 是同构的当且仅当我们对于每个原初模 L 都有 [M : L] = [N : L]。

#### 推论 2 {#alg-viii-s2-lem-4-cor-2 .statement tag=00QY}

设M为半原始模。 Let $(M_i)_{i\in I}$ and $(M'_j)_{j\in J}$ be families of 原始子模 of M such that

$$
M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j
$$

那么存在M的自同构$u$和从I到J的双射$\varphi$，这样对于每个$i\in I$我们都有$u(M_i) = M'_{\varphi(i)}$。

对于任何原初模 L，令 $I_L$（分别为 $J_L$）为指标 $i\in I$（分别为 $j\in J$）的集合，使得 $M_i$（分别为 $M'_j$）同构于L。 The nonempty sets of the form $I_L$ (resp. $J_L$) form a partition of I (resp. J)，对于每个 L，我们有

卡(I$_L$) $=$ 卡(J$_L$) $= [M : L]$;

推论如下。

#### 推论 3 {#alg-viii-s2-lem-4-cor-3 .statement tag=002E}

设 M、N 和 P 为半原始模。假设 $M\oplus P$ 与 $N\oplus P$ 同构，并且 [P : L] 对于每个原初模 L 都是有限的。则 M 和 N 同构。

到假设，我们有

[M : L] + [P : L] = [N : L] + [P : L]

对于每个原始模L。由于 [P : L] 是有限的，因此根据 (集合理论, III, §3, No. 4, p. 162, 命题 8) 的归纳，我们对于每个原初模有 [M : L] = [N : L] L。因此，根据推论 1，模 M 和 N 同构。

#### 推论 4 {#alg-viii-s2-lem-4-cor-4 .statement tag=002F}

设 M 和 N 为半原始模。假设存在整数$d >0$使得$M^d$同构于$N^d$。则模 M 和 N 同构。

设L为原初模。 By 假设, we have

$$
d[M : L] =d[N : L]
$$

因此，我们有等式 [M : L] = [N : L]：事实上，对于每个无限基数 $\mathfrak{a}($集合理论，III, §6, No. 3，p. 188，推论 4），我们都有 $d\mathfrak{a}=\mathfrak{a}$。根据推论 1，模 M 和 N 同构。

#### 推论 5 {#alg-viii-s2-lem-4-cor-5 .statement tag=002G}

令 M 为半原始模，即原始子模的有限族 $(M_i)_{i\in I}$ 的直和。对于 I 中的任意子集 J，写为 $M_J=\bigoplus_{i\in J}M_i$。令 N 为 M 的直因子子模。

a) 存在I的子集 J，使得$M_J$是子模对N的补充。

b) 令 J 为 I 的子集。如果$M_J$是N的补集，则模N与$M_{I-J}$同构并且是半原初的。

我们用指标 $i\in I$ 的 K 集合表示，使得 $N\cap M_i= 0$；让我们在 K 的基数上计算使用归纳法。如果 M = N，则推论很清楚。假设 $M\not= N$。设$p$为M与核N的投影算子。用P表示其像。它是非零的，并且由引理3，存在$j\in I$使得$p$诱导同构从P 的$M_j$ 到直因子子模。我们有$N\cap M_j= 0$。 集合$N'= N\oplus M_j$。我们有$N'= N\oplus p(M_j)$。 P 中对 $p(M_j)$ 的补充子模也对 M 中的$N'$ 进行补充，因此$N'$ 是 M 的直因子子模。指标 $i\in I$ 的集合使得$N'\cap M_i= 0$ 包含在 K $-\{j\}$ 中。到归纳假设，存在I的子集$J'$，使得$M_{J'}$是M中$N'$的子模补充。集合$J = J'\cup  \{j\}$。那么$M_J$是M中N的子模补充。

令J为I的子集，使得$M_J$是N中M的子模补充。由于$M_J$也是$M_{I-J}$的补充，模N和$M_{I-J}$是同构的，并且N是半本初的。

#### 推论 6 {#alg-viii-s2-lem-4-cor-6 .statement tag=002H}

每超过有限生成射影模超过局部环免费。[^2]

设A为局部环。 A-模 $A_s$ 是本初 (VIII, p. 31)。 如果 M 是有限生成射影 A-模，则存在 A-模 N 和自然数 $n$，使得 $M\oplus N$ 同构于 $A^n_s$（II, §2, No. 2，p. 232，推论 1）。 从推论 5 可以得出，对于整数 $m$，模 M 本身与 $A^m_s$ 同构，使得 $0\leqslant m\leqslant n$ 是自由的。

#### 注 {#alg-viii-s2-n4-rem-1 .statement tag=002I}

设 M 和 $M'$ 为半原初 A-模。 从VIII、p. 33的引理 4 立即可以得出，当且仅当我们对每个原初A-模L都有$[M': L]\leqslant [M : L]$时，$M'$同构于M的直因子子模。 特别地，如果L是原初A-模，[M : L]是基数$\mathfrak{a}$的最大的，其中存在与$L^{(\mathfrak{a})}$同构的M的直因子子模。

因此，关系 [M : L] = 0 意味着不存在与 L 同构的 M 的直因子子模。这并不排除M同构于L的子模的存在；只需考虑例，其中 $A =\mathbf{Z}, L =\mathbf{Z}/2\mathbf{Z}$ 和 $M =\mathbf{Z}/4\mathbf{Z}:$，$\mathbf{Z}$-模块 L 和 M 是原始的且不是同构的，因此 [M : L] = 0 且 L 与子模同构M 的$2\mathbf{Z}/4\mathbf{Z}$。

### 5. 有限长度模结构

#### 定理 2（克鲁尔-雷马克-施密特）{#alg-viii-s2-thm-2 .statement tag=00RY}

设 A 为环，M 为有限长度的 A-模。

a) 存在M 的不可分解子模的有限族$(M_i)_{i\in I}$，使得$M =\bigoplus_{i\in I}M_i$ 和模 M 是半原初的。

b) 设$(M_i)_{i\in I}$和$(M'_j)_{j\in J}$是M的不可分解子模的两个有限族，使得$M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j$。从I到J存在双射$\sigma$和M的自同构$u$，这样对于每个$i\in I$我们都有$u(M_i) = M'_{\sigma(i)}$。

c) 令N为M的直因子子模，并令$(M_i)_{i\in I}$为M的不可分解子模与直和M的有限族。存在I的子集J，使得$\bigoplus_{i\in I-J}M_i$是N的补集。模N同构于$\bigoplus_{j\in J}M_j$。

d) 设 N 为 A-模。如果存在整数$d >0$使得模$M^d$和$N^d$同构，则模M和N同构。

e) 令 N 和 P 为 A-模或有限长度。如果模 $M\oplus P$ 和 $N\oplus P$ 同构，则 M 和 N 同构。

有限长度中的模既是阿廷的又是诺特（VIII、p. 2、命题 1）。此外，对于有限长度的模，不可分解或原始等价于（VIII，p. 31，命题4）。 断言 a) 然后从命题 3 of VIII, p. 30 得出。 断言 b)、c) 和 e) 分别来自VIII、p. 32 定理 1 的推论 2、5 和 3。最后，断言 d) 由 VIII、p. 35 的推论 4 得出，因为在 d) 的假设下，模 N 具有有限长度，因此与 a) 是半原初的。

#### 定理 3 {#alg-viii-s2-thm-3 .statement tag=002J}

令 K 为交换域，A K-代数，M 和 N 模为有限长度。令$K'$为非零的交换K-代数，使得$A_{(K')}$模块$M_{(K')}$和$N_{(K')}$同构。则 A-模 M 和 N 同构。

a) 首先，假设代数$K'$在K上有有限次数$d$。则A-模$M_{(K')}$与$M^d$同构，A-模$N_{(K')}$与$N^d$同构，因此A-模 $M^d$ 和 $N^d$ 同构。由定理 2，d)，A-模 M 和 N 同构。

b) 现在，假设 K-代数 $K'$ 是由有限多个元素生成的。 选择最大理想$\mathfrak{m}$为$K'$，以及集合$K''= K'/\mathfrak{m}$。通过希尔伯特零点定理（VIII，p. 462，定理 1的推论1）$, K''$是K的有限次扩张。通过从$K'$到$K''$的标量扩张，我们推出： $A_{(K')}$-线性同构 $M_{(K')}\rightarrow N_{(K')}$ $A_{(K'')}$-线性同构 $M_{(K'')}\rightarrow N_{(K'')}$。由证明的部分a)，A-模M和N是同构的。

c) 最后，让我们处理一般情况。令$u: M_{(K')}\rightarrow N_{(K')}$为$A_{(K')}$模块和$v: N_{(K')}\rightarrow M_{(K')}$逆同构的同构。表示由有限多个元素生成的$K'$K-子代数$\mathscr{E}$集合。如果E是这样的子代数，则$A_{(E)}$与$A_{(K')}$的子环标识，并且$M_{(E)}$和$N_{(E)}$分别与$M_{(K')}$和$N_{(K')}$的$A_{(E)}$子模块标识（II, §7, No. 7， p. 306);此外，$M_{(K')}$和$N_{(K')}$分别是右向族$(M_{(E)})_{E\in\mathscr{E}}$和$(N_{(E)})_{E\in\mathscr{E}}$的并。 A-模 M 和 N 为有限长度，因此是有限生成的；令 S 为 A-模 M 的有限生成子集和 T 有限生成子集 A-模 N。存在 K-代数 $E\in \mathscr{E}$，这样我们对于每个 $s\in S$ 都有 $u(1\otimes s)\in N_{(E)}$ 并且每 $t\in T$ $v(1\otimes t)\in M_{(E)}$。根据线性关系，我们有 $u(M_{(E)})\subset N_{(E)}$ 和 $v(N_{(E)})\subset M_{(E)}$。 映射$u$和$v$，然后诱导逆双射从$M_{(E)}$到$N_{(E)}$以及从$N_{(E)}$到$M_{(E)}$。这些双射显然是 $A_{(E)}$ 线性的。因此，$A_{(E)}$-模块$M_{(E)}$和$N_{(E)}$是同构的。由证明的部分b)可知，A-模M和N是同构的。

#### 注 {#alg-viii-s2-n5-rem-1 .statement tag=002K}

令E和F为交换域K上的两个有限维向量空间，并令$K'$为K的扩张。令$u$为E的自同态和F的$v$自同态，并令$u_{(K')}$和$v_{(K')}$为$E_{(K')}$和$F_{(K')}$的自同态由标量的扩张获得。由VII, §5, No. 3、p. 32的推论1和2得出，自同态、$u$和$v$相似当且仅当自同态$u_{(K')}$和$v_{(K')}$相似。这也是从上面的定理 3 应用于代数 A = K[X] 和 A-模 $M = E_u$ 和 $N = F_v$ (VII, §5, No. 1, p. 29) 得出的。

### 习题{#alg-viii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。

[^1]: Note added in translation: some authors use the terminology “module with local endomorphism ring” for “primordial module.”
[^2]: It can be shown that every projective module over a local ring is free (VIII, p. 42, Exercise 18).
