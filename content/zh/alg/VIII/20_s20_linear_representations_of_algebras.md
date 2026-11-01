---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 20
section_title: Linear Representations of Algebras
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.373-A VIII.395
pdf_pages: 0390-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: Linear Representations of Algebras
      page: 373
      pdf_page: 390
    - "no": 2
      title: Restricted Dual of an Algebra
      page: 375
      pdf_page: 392
    - "no": 3
      title: Coefficients of a Module
      page: 377
      pdf_page: 394
    - "no": 4
      title: Restricted Dual and Matrix Coefficients
      page: 379
      pdf_page: 396
    - "no": 5
      title: Dual of a Semisimple Algebra
      page: 380
      pdf_page: 397
    - "no": 6
      title: Character of a Representation
      page: 382
      pdf_page: 399
    - "no": 7
      title: Coefficients of a Set of Classes of Modules
      page: 387
      pdf_page: 404
    - "no": 8
      title: Cogebra Structure on the Restricted Dual
      page: 388
      pdf_page: 405
statements: 31
exercises: 6
content_sha256: d19ce9dab9162f9d61b851dcc99302caed1f731f7cd0ac4a5216a0f14f9098f9
translated_from: content/en/alg/VIII/20_s20_linear_representations_of_algebras.md
translation_method: google
source_content_sha256: f366c2c3ce31096fbcd7ad9041a4e06384cc60f8e5e5fd661e93b1a5434b90dc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8508cb4b71f8ef39a37146f8fd921fffce0eb5763cae3a86b2aafc17624ee495
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 20。 线性表示代数

在这个截面中，K是交换环，A是K-代数。从No. 2开始，我们假设K是域，并用$A^*$表示向量空间A对K的对偶。在这个截面中，记号$A^*$永远不会指代环A的乘法群。

### 1. 线性表示 / 代数

#### 定义 1 {#alg-viii-s20-def-1 .statement tag=00MD}

令 M 为 K-模。 M中代数A的线性表示是从A到代数End$_K(M)$的K同态$\pi$。

我们也说对$(M, \pi )$是代数A的线性表示。当M是自由K-模时，M的维数称为$\pi$的次数（或维数）。

令$\pi$为M中A的线性表示。M上的加法律和M上的外法则$(a, x)\mapsto \pi (a)(x)$定义左A-模结构，我们用$M_{\pi}$表示。我们说$M_{\pi}$是表示$\pi$中的模。 M 上的K-模结构是通过$M_{\pi}$ 上的A-模结构通过限制标量获得的。

相反，令 E 为左A-模。设 M 为从 E 通过从 A 到 K 的标量限制推导出来的 K-模，并令 $\pi$ 为从 A 到 End$_K(M)$ 的同态 $a\mapsto a_E$。那么$\pi$就是A在M中的表示，我们有$E = M_{\pi}$。我们说 $\pi$ 是线性表示与 A-模 E 相关联。

研究 A 的 A-模或线性表示效果相同。我们会将模的某些定义翻译为线性表示的语言。

令$\pi$为M中A的线性表示。同态$\pi$的核是A的双面理想，简单来说就是A-模$M_{\pi}$的湮没子。 同态 $\pi$ 是单射当且仅当 A-模 $M_{\pi}$ 忠实；然后我们说$\pi$是A的忠实表示。

令$(M, \pi )$和$(M', \pi ')$为A的线性表示。A-线性映射从$M_{\pi}$到$M'_{\pi'}$是满足关系的K-线性映射$u: M\rightarrow M'$

$$
\pi '(a)\circ u=u\circ \pi (a) \tag{1}
$$

$a\in A$。从$M_{\pi}$到$M'_{\pi'}$的同构是K-模$u: M\rightarrow M'$满足条件中的同构

$$
\pi '(a) =u\circ \pi (a)\circ u^{-1} \tag{2}
$$

$a\in A$。如果 A-模 $M_{\pi}$ 和 $M'_{\pi'}$ 同构的，我们就说 $\pi$ 和 $\pi '$ 同构的。如果 $M_{\pi}$ 是 $M'_{\pi'}$ 的子模（分别是商模），我们就说 $\pi$ 是 $\pi '$ 的子表示（分别是表示）。

假设给定 A 的线性表示的族$(M_i, \pi_i)$。令 M 为K-模，即 $M_i$ 的直和；对于任何$a\in A$，令$\pi (a)$为M的自同态$(x_i)_{i\in I}\mapsto (\pi_i(a)(x_i))_{i\in I}$。则$\pi$为M中A的线性表示。A-模$M_{\pi}$为A-模的直和 $(M_i)_{\pi}(i\in I)$；我们说$\pi$是$\pi_i$的直和，我们写成$\pi =\bigoplus\pi_{i^i}$。

如果 A-模 $M_{\pi}$ 是简单的，我们就说 M 中 A 的表示 $\pi$ 是简单的或不可约的；我们说 A 在 M 上的表示 $\pi$ 是半单或完全可约，如果 A-模 $M_{\pi}$ 是半单。

令$\pi$为M中A的线性表示。令$M^*$为K-模对偶M。映射$a\mapsto^t(\pi (a))$从$A^o$到End$_K(M^*)$是$\pi$的转置表示。

令L为交换K-代数，并令$(M, \pi )$为K-代数A的线性表示。同态$\pi_{(L)}: A_{(L)}\rightarrow$结束$_L(M_{(L)})$相应的到$M_{(L)}$上的$A_{(L)}$模块结构为L-代数$A_{(L)}$的线性表示。我们说$\pi_{(L)}$是代数$A_{(L)}$的线性表示，是从表示$\pi$通过将标量K的环延伸到L推导出来的。

假设 K 为域，L 为非零的交换K-代数。

设$\pi$和$\pi '$为代数A的线性表示。从VIII、p. 37、定理3可知，表示、$\pi$和$\pi '$同构当且仅当$\pi_{(L)}$和$\pi '_{(L)}$ 是。

假设K是域。令 L 为 K 的扩张。考虑 A-模的格罗滕迪克群 $R_K(A)$（分别为 $R_L(A_{(L)})$），它们是 K 上的有限维（分别是 $A_{(L)}$ 模，它们是 L 上的有限维）。我们已经看到群同态

$$
u: R_K(A)\longrightarrow R_L(A_{(L)})
$$

由标量扩张定义是单射的；此外，当且仅当$u(\xi )$为(VIII，p. 195，定理 1)时，元素$\xi \in R_K(A)$才有效。

### 2. 代数的限制对偶

从现在开始我们假设 K 是域。

对于$a\in A$，从A到A用$\boldsymbol{\gamma }(a)$映射$x\mapsto ax$和$\boldsymbol{\delta }(a)$映射$x\mapsto xa$表示。则$\boldsymbol{\gamma }$是A中A的线性表示，称为左正则表示；同样，$\boldsymbol{\delta }$是A中$A^o$的线性表示，称为（滥用语言）A的右正则表示。通过换位，我们从代数A和$A^o$的$\boldsymbol{\delta }$和$\boldsymbol{\gamma }$推出线性表示 $A^*$ 左A-模结构上的向量空间 $A^*$ 定义以及左$A^o$ 模块结构。这两个结构对应到$(A$，A)-双模结构在$A^*$上，外法则由公式定义

$$
\langle af, b\rangle =\langle f, ba\rangle \tag{3}
$$

$$
\langle f a, b\rangle =\langle f, ab\rangle \tag{4}
$$

对于 $a, b,\in A$ 和 $f\in A^*$。

回想一下 (II, §2, No. 4, p. 234, 定义 4)，如果 E 是 A 的线性子空间，则其在 $A^*$ 中的正交$E'$ 是 A 上线性形式的集合，而 A 的限制到 E 为零。同样地，$A^*$的线性子空间F在A中的正交$F'$是线性形式属于的核与F的交。

我们知道(II, §7, No. 5,p. 299,定理7)从有限余维A的线性子空间集合到子空间的线性集合映射$\varphi : E\mapsto E'$为双射 $A^*$ 共有限维。逆映射 $\varphi^{-1}$ 将 $A^*$ 的有限维子空间 F 发送到 A 中与其正交的 $F'$。

#### 命题 1 {#alg-viii-s20-prop-1 .statement tag=00ME}

a) 映射 $\varphi$ 诱导双射从 A 的有限余维的集合理想到右A-子模的集合（分别为左A-子模、子双模） $A^*$ 有限维超过 K。

b) 有限余维包含的 A 的每个左理想或右理想都是有限余维的两侧理想。

公式 (3)和(4)证明，若E是A的左理想，则$E'$是$A^*$的右A-子模；如果V是$A^*$的右A-子模，则$V'$是A的左理想。右理想和双边理想的情况类似地处理。这就证明了a）。

令 $\mathfrak{a}$ 为有限余维 A 的左理想。 左A-模 $E = A_s/\mathfrak{a}$ 是 K 上的有限维，End$_K(E)$ 也是如此。因而，从 A 到 End$_K(E)$ 的同态 $a\mapsto a_E$ 的核是$\mathfrak{a}$ 中包含的有限余维 A 的双面理想。 经过到逆环$A^o$，我们看到有限余维包含的A的每个正理想都是有限余维的双面理想。

#### 定义 2 {#alg-viii-s20-def-2 .statement tag=00MF}

受限双

K-代数 A 的，记为 θ(A)，是有限余维 A 的两侧理想的正交线 $A^*$ 中的并。

通过命题 1，我们可以给出 θ(A) 的等价描述：

– 有限余维 A 的左理想的正交并

– the union of the orthogonals of the right ideals of A of finite codimension – the union of the orthogonals of the two-sided ideals of A of finite codimension – the union of the left A-submodules of $A^*$ of finite dimension over K

– K 上有限维 $A^*$ 右A-子模并

– $(A$ 的并，A) K 上有限维的$A^*$ 的子双模。

如果 A 在 K 上有有限次数，我们就有 $\Theta (A) = \Theta (A^o)$ 和 $\Theta (A) = A^*$。令 $f\in A^*$；则 $f$ 属于到 θ(A) 当且仅当 $Af$（分别为 $fA, AfA$）是 $A^*$ 和有限维在 K 上的线性子空间。

K 上有限维的 $A^*$ 的两个 $(A$, A)-子双模的和在 K 上有有限维。因而，θ(A) 是 $A^*$ 的 $(A$, A)-子双模。

### 3.模的系数

设E为左A-模。令 $E^*$ 为向量空间 E 与 K 的对偶；我们赋予它天然的右A-模结构。给定 E 的元素 $x$ 和 $E^*$ 的 $x^*$，我们用 $c_E(x, x^*)$ 线性形式表示

$$
c_E(x, x^*) :a\mapsto  \langle x^*, ax\rangle \tag{5}
$$

这些线性形式称为E的系数。由E的系数生成的$A^*$的子空间记为$\Theta_E(A)$。如果E是非零的，则它是非零的。

如果 F 与 E A-模同构，则 E 和 F 具有相同的系数，并且我们有 $\Theta_F(A) = \Theta_E(A)$。让我们将 $E^*$ 视为左 $A^o$ 模块； E的系数是$E^*$和$\Theta_E(A)\subset \Theta_{E^*}(A^o)$的系数。因而，如果 E 是 K 上的有限维，则 E 和 $E^*$ 具有相同的系数，并且我们有 $\Theta_E(A) = \Theta_{E^*}(A^o)$。

令$(M, \pi )$为代数A的线性表示。A-模$M_{\pi}$的系数也称为表示$\pi$的系数。 $x\in M$和$x^*\in M^*$的系数$c_{M_{\pi}}(x, x^*)$也用$c_{\pi}(x, x^*)$表示； 向量空间$\Theta_{M_{\pi}}(A)$也用$\Theta_{\pi}(A)$表示。

#### 注 1 {#alg-viii-s20-n3-rem-1 .statement tag=00MG}

假设 M 在 K 上是有限维的。令 $(e_1, . . . , e_n)$ 为 V 的基，并令 $(e^*_1, . . . , e^*_n)$ 为其对偶基。相对于V的基$(e_1, . . . , e_n)$用$\pi (a)$的$(\pi_{ij}(a))$矩阵表示；我们有$\pi_{ij}=$$c_{\pi}(e_j, e^*_i)$。从A到$\mathbf{M}_n(K)$，映射$a\mapsto (\pi_{ij}(a))$是同态；这样同态就是有时，称为代数A的矩阵表示。

#### 注 2 {#alg-viii-s20-n3-rem-2 .statement tag=00MH}

设E为A-模，$E'$为E的子模。根据II, §7, No. 5、p. 299的定理 5的推论，我们有$\Theta_{E'}(A)\subset \Theta_E(A)$和$\Theta_{E/E'}(A)\subset \Theta_E(A)$。

令$\gamma_E$为从$E\otimes_KE^*$到$A^*$的唯一的K-线性映射，将$x\otimes x^*$发送到$c_E(x, x^*)$。它是$(A$，A)-双线性，它的像是$\Theta_E(A)$。我们从中推导出 A-线性映射 $c'_E: E\rightarrow$ Hom$_A(E^*,A^*)$ 和 $c''_E: E^*\rightarrow$ Hom$_A(E,A^*)$ 这样

$$
c'_E(x)(x^*) =c_E(x, x^*) =c''_E(x^*)(x)
$$

表示为 $\theta_E$ K-线性映射 $\theta_E: E\otimes E^*\rightarrow$ 结束$_K(E)$ 特征为关系

$$
\theta_E(x\otimes x^*)(y) =\langle x^*, y\rangle x
$$

对于 $x, y\in E$ 和 $x^*\in E^*$。其像为有限秩E自同态集合End$^f_K(E)$(VIII，p. 463)。通过迹线的定义（前述），我们有

Tr($\theta_E(x\otimes x^*)$) $=\langle x^*, x\rangle$

对于 $x\in E$ 和 $x^*\in E^*$；因此我们有

$\langle \gamma_E(x\otimes x^*), a\rangle =\langle x^*, ax\rangle =$Tr($\theta_E(ax\otimes x^*)$)$=$Tr($\theta_E(x\otimes x^*)a$)。

这给出了关系

$\langle \gamma_E(h), a\rangle =$Tr($\theta_E(h)\circ a_E$)

对于 $a\in A$ 和 $h\in E\otimes_KE^*$。这证明$\Theta_E(A)$是A上线性形式$a\mapsto$Tr($u\circ a_E$)的集合，其中$u$穿过End$^f_K(E)$。

#### 引理 1 {#alg-viii-s20-lem-1 .statement tag=00MI}

映射 $c''_E$ 是双射的。如果 E 是有限维的，那么 $c'_E$ 也是有限维的。

当F为右A-模且G为K-向量空间时，我们定义了从Hom$_K(F\otimes_AE,G)$到Hom$_A(E$的K-向量空间的II, §4, No. 1、p. 268、命题1，a) 同构$\gamma$，坎$_K(F,G))$。这个同构送入$\varphi : F\otimes_AE\rightarrow G$到同态$e\mapsto (f\mapsto \varphi (f\otimes e))$。从$A_d\otimes_AE$经过典范同构到E（II, §3, No. 4，第$249$）$,\gamma$，当$F = A_d$且G = K时，可与$c''_E$识别。

类似地，在II, §4, No. 1、p. 268、命题 1、b) 中定义的同构$\beta$专门化为从Hom$_K(E^*\otimes_AA_s,K)$到Hom$_A(E^*$、Hom$_K(A_s,K))$的同构$\beta$。当E是有限维时，E可以规范地与Hom$_K(E^*,K)$等同，$E^*$与$E^*\otimes_AA_s$规范等同；然后同态$\beta$被识别为$c'_E$。

#### 命题 2 {#alg-viii-s20-prop-2 .statement tag=00MJ}

令 E 为左A-模。

a) E的系数集合从E到$A^*$是A-线性映射像并。

b) 此外，假设 E 对 K 具有有限维 $n$。则左A-模 $\Theta_E(A)$ 同构于 $E^n$ 的商，A-模 E 同构于 $\Theta_E(A)^n$ 的子模，并且每个$\Theta_E(A)$的元素是$E^n$的系数。

断言 a) 由$c''_E$ 的满射性推出。

让我们证明b)。令$(e^*_1, . . . , e^*_n)$为$E^*$在K上的基。由于$\Theta_E(A)$是由E的系数生成的，A-线性映射

$$
(x_1, . . . , x_n)\mapsto \sum_{i=1}^nc_E(x_i, e^*_i)
$$

从 $E^n$ 到 $\Theta_E(A)$ 是满射的。由a)可知，$\Theta_E(A)$的每一个元素都是$E^n$的系数。而且，A-线性映射

$$
x\mapsto (c_E(x, e^*_1), . . . , c_E(x, e^*_n))
$$

从 E 到 $\Theta_E(A)^n$ 是单射的；这给出了b)。

#### 注 3 {#alg-viii-s20-n3-rem-3 .statement tag=00MK}

令 E 为 $A^*$ 的左A-子模。令E上的$\varepsilon$为线性形式$y\mapsto y(1)$。对于E中的每个$x$，我们有$x=c_E(x, \varepsilon )$，所以E是$\Theta_E(A)$的A-子模。

### 4. 限制双重和矩阵系数

#### 命题 3 {#alg-viii-s20-prop-3 .statement tag=00ML}

设$(V, \pi )$为代数A的有限维线性表示。$\pi$的核$\mathfrak{a}$是有限余维A的双面理想，$\Theta_{\pi}(A)$是$\mathfrak{a}$的正交$A^*$。 转置的映射 $\pi$ 定义同构，从K-向量空间 $\pi (A)$ 到 $\Theta_{\pi}(A)$ 的对偶。

由于 End$_K(V)$ 是有限维的，$K,\mathfrak{a}$ 是有限余维 A 的双面理想。 向量空间$\Theta_{\pi}(A)$是$A^*$的有限维子空间，其在A中的正交等于$\mathfrak{a}$；通过 II, §7, No. 5、p. 301、空间 $\Theta_{\pi}(A)$ 的定理 7 因此是 $\mathfrak{a}$ 在 $A^*$ 的正交。此外，由于$\mathfrak{a}$是$\pi$的核，映射$\pi$定义同构的转置从$\pi (A)$的对偶到$\mathfrak{a}$的正交$A^*$（II, §7, No. 5，p. 299，定理 5 的推论）。

#### 推论 {#alg-viii-s20-n4-cor-1 .statement tag=00MM}

A 的受限对偶 θ(A) 是 A 的有限维线性表示的系数的集合。

通过定义，θ(A) 是有限余维 A 的两侧理想的正交的并。因此，对于 A 的每个有限维线性表示 $\pi$，我们都有 $\Theta_{\pi}(A)\subset \Theta (A)$。相反，令 $f$ 为 θ(A) 的元素，并令 $\mathfrak{a}$ 为有限余维的双面理想，包含在 $f$ 的核中（VIII、p. 376、定义 2）。用$A/\mathfrak{a}$中A的$\pi$线性表示表示，从A中左侧正则表示按经过推导出商。令$x$为1的类（mod$\mathfrak{a}$），并令$x^*$为从$f$推导出的$A/\mathfrak{a}$上的线性形式。我们有$f=c_{\pi}(x, x^*)$，所以$f$是$\pi$的系数。

取注，如果$(V, \pi )$是K上非有限维A的线性表示，则空间$\Theta_{\pi}(A)$不一定包含在θ(A)中。

### 5. 半单代数的对偶

设$\Theta^{ss}(A)$为左A-模 θ(A)的底层，即θ(A)的(VIII,p. 65)最大的半单子模。我们用简单（左）A-模的类的$\mathscr{S}_K$集合表示，它们是K上的有限维。当A是K上的有限次数的半单代数时，我们有$A^*= \Theta (A) = \Theta^{ss}(A)$，因为每个左A-模都是半单 （VIII、p. 138、命题 4）。

#### 定理 1 {#alg-viii-s20-thm-1 .statement tag=00MN}

a) 集合 $\Theta^{ss}(A)$ 由 A 的有限维半单表示的系数组成。它是 $A^*$ 的 $(A,A)$ 子双模。

b) 对于每个$S\in \mathscr{S}_K$，型 S 的 θ(A) 的同型分量等于 $\Theta_S(A)$。 左A-模$\Theta^{ss}(A)$是子模$\Theta_S(A)$的直和，其中S穿过$\mathscr{S}_K$。

c) 对于 $\mathscr{S}_K$ 中的每个 S，右A-模 $S^*$ 都是简单的，$\Theta_S(A)$ 是右A-模 θ(A) 的型 $S^*$ 的同型分量。 The mapping that sends S to cl($S^*$) is a bijection from $\mathscr{S}_K$ to the set of classes of simple $A^o$-modules of finite dimension over K.

d) 视为右A-模，θ(A) 有底层 $\Theta^{ss}(A)$。

令 E 为 K 上有限维的半单A-模。从 E 到 $A^*$ (VIII、p. 378、命题 2)，属于到像 A-线性映射的每个系数，因此属于到$\Theta^{ss}(A)$。相反，设$f\in \Theta^{ss}(A)$。那么 A-模 $Af$ 是 K 上的有限维且是半单。到VIII中的注，p. 367$,f$是$Af$的系数。

对于$\mathscr{S}_K$中的每个S，型S的θ(A)的同型分量由A-线性映射的像从S到$A^*$生成；因此，它等于$\Theta_S(A)$乘命题2，a) of VIII，p. 378。另一方面，如果 S 是单A-模，在 K 上不是有限维，则型 S 的 θ(A) 的同型分量是零：事实上，θ(A) 的每个简单子模都是单调的，因此在 K 上是有限维的。因为 θ(A) 的底层是直和其同型成分 (VIII, p. 65, 命题 4), 这就证明了 b).

令 S 为 K 上的有限维的单A-模。由于 K-向量空间 S 不会减少到 0，因此对于 $S^*$ 也是如此。令E为右A-模$S^*$中的子模； S 中的正交 $E'$ 是 S 的 A-子模。由于 S 很简单，我们有 $E'= 0$（在这种情况下为 $E = S^*$）或 $E'= S$（在这种情况下 E = 0）。因此 $S^*$ 是单右A-模。

我们有$\Theta (A^o) = \Theta (A)$（VIII，p. 376）；我们认同右A-模与左侧 $A^o$ 模块。由于K上的有限维的每个向量空间都同构于它的对偶，上面证明简单的类的映射$S\mapsto$cl($S^*$)是双射从$\mathscr{S}_K$到集合 $A^o$-有限维的模在 K 上。现在，对于 $\mathscr{S}_K$ 中的 S，型 $S^*$ $\Theta (A^o)$ 的同典型分量等于 $\Theta_{S^*}(A^o)$，将断言 b) 应用于代数 $A^o$，我们有$\Theta_{S^*}(A^o) = \Theta_S(A)$。 断言 c) 和 d) 紧随其后。

#### 推论 1 {#alg-viii-s20-thm-1-cor-1 .statement tag=00MO}

K 上有限维的每个单A-模同构于 θ(A) 的 A-子模。

这是从定理 1, b) 得出的，因为对于每个非零的 A-模 E，我们都有 $\Theta_E(A)\not= 0$。

#### 推论 2 {#alg-viii-s20-thm-1-cor-2 .statement tag=00MP}

如果 K 上的有限维中的两个单A-模有公共的非零的系数，则它们是同构的。

令 $S_1$ 和 $S_2$ 为 K 上有限维的单A-模，系数为公共的非零的。那么我们就有$\Theta_{S_1}(A)\cap \Theta_{S_2}(A)\not= 0$。现在，$\Theta_{S_1}(A)$ 是型 $S_1$ 的同型，$\Theta_{S_2}(A)$ 是型 $S_2$ 的同型。所以$S_1$同构于$S_2$。

到定理 1，$\Theta^{ss}(A)$ 是 S 的 $(A$、A)-双模 $\Theta_S(A)$ 的 $A^*$、直和的 $(A$、A)-双模，穿过 $\mathscr{S}_K$。这些双模是成对非同构的，因为它们已经与左A-模非同构。

在 $\mathscr{S}_K$ 中修复一个 S。用D表示End$_A$(S)的对数域，并将S视为右D-模，将$S^*$视为左D-模。根据这些约定，S 是$(A$，D)-双模，$S^*$ 是$(D$，A)-双模，$S\otimes_DS^*$ 是$(A$，A)-双模。

#### 命题 4 {#alg-viii-s20-prop-4 .statement tag=00MQ}

a) 从$S\otimes_DS^*$到$\Theta_S(A)$存在群同态$\lambda_S$，其特征为

$$
\lambda_S(x\otimes x^*) =c_S(x, x^*) \tag{6}
$$

$x\in S$ 和 $x^*\in S^*$。这个映射是$(A,A)$双模的同构。

b) $(A,A)$-双模块$\Theta_S(A)$很简单。

以公式 $\gamma_S(x\otimes x^*) =c_S(x, x^*)$为特征的映射$\gamma_S: S\otimes_KS^*\rightarrow \Theta_S(A)$是$(A$，A)-线性和满射，并且对于$x\in S,x^*\in S^*$和$d\in D$满足$\gamma_S(xd\otimes x^*)$$=\gamma_S(x\otimes dx^*)$。因此定义是一个满射$(A$，A)-线性映射$\lambda_S: S\otimes_DS^*\rightarrow \Theta_S(A)$，其特征在于公式 (6)。

让我们证明$S\otimes_DS^*$是一个简单的$(A$，A)-双模。根据VIII，p. 63的推论2，$S\otimes_DS^*$的每个$(A$，A)-子双模都是形式$S\otimes_DH$，其中H是$S^*$的$(D$，A)-子双模。由于 $S^*$ 是单右A-模 (VIII, p. 380, 定理 1, c))，我们有 H = 0 或 $H = S^*$；接下来是断言。

同态$\lambda_S$是$(A$，A)-线性且非零的；由于 $S\otimes_DS^*$ 是简单的双模，因此 $\lambda_S$ 是单射 (VIII, p. 47, 命题 2, a))。

#### 注 {#alg-viii-s20-n5-rem-1 .statement tag=00MR}

当域 K 是代数闭集时，我们有 D = K by VIII、p. 47 的定理 1，并且 $\lambda_S$ 是 $(A$ 的同构，A) 从 $S\otimes_KS^*$ 到 $\Theta_S(A)$ 的双模。

### 6.表示的特征标

令 E 为 K 上有限维的左A-模。E 的特征标或 E 的迹，用 Tr$_E$ 表示，为线性形式 $a\mapsto$ Tr($a_E$)。令 $(e_1, . . . , e_n)$ 为 E 的基，$(e^*_1, . . . , e^*_n)$ 为对偶基。到定义，我们有关系

(7) Tr$_E=\sum_{i=1}^nc_E(e_i, e^*_i)$。

线性形式Tr$_E$属于至$\Theta_E(A)$。如果 E 和 $E'$ 是两个同构 A-模，我们有 Tr$_E=$ Tr$_{E'}$。所以Tr$_E$仅取决于E的同构类。

令$\pi$为A在有限维的向量空间V在K上的线性表示。$\pi$或$\pi$的有时特征标的迹定义为A-模的特征标 $V_{\pi}$。我们用 Tr$_{\pi}$ 表示。如果$(e_1, . . . , e_n)$是K上V的基，并且对于这个基，如果$(\pi_{ij}(a))$是$\pi (a)$的矩阵，那么我们有

(8) Tr$_{\pi}(a) =\sum_{i=1}^n\pi_{ii}(a)$。

线性形式Tr$_{\pi}$属于至$\Theta_{\pi}(A)$。

#### 命题 5 {#alg-viii-s20-prop-5 .statement tag=00MS}

设 S 为 K 上有限维的单A-模，设 D 为 S 的交换子的对数域，设 Z 为 D 的中心。以下性质是等价的：

(i) S 的特征标 Tr$_S$ 不是零。

(ii) 存在元素$d\in D$使得Tr$_{D/K}(d)\not= 0$。

(iii) K 的扩张 Z 是可分离的，且 K 的特征$p$ 不除次数 [D : Z]。

右D-向量空间 S 是有限维的。令$(e_1, . . . , e_n)$为S在D上的基，并令$u$为End$_D(S)$的元素。令$(d_{ij})$为$u$相对于基$(e_1, . . . , e_n)$的矩阵。我们有 $u(e_j) =\sum^n_{i=1}e_id_{ij}$ 对应 $j\in [1, n]$。用 $u_K$ 映射 $u$ 表示为 K-向量空间 S 的自同态，并用 $u_K$ 的 $(u_{ij})$ 矩阵相对于 K-向量空间 S 的分解 $(e_iD)$ 表示为直和（II, §10, No. 5，p. 346）。我们有 Tr($u_K$) $=\sum_i$ Tr($u_{ii}$)。而且，$u_{ii}$是$u_{ii}(e_id) =e_id_{ii}d$对$d\in D$定义的K-向量空间$e_iD$的自同态，所以它的迹等于Tr$_{D/K}(d_{ii})$。由此我们证明了等式

(9) Tr($u_K$)$=$Tr$_{D/K}(\sum_id_{ii})$。

根据 Burnside 的定理（VIII，p. 83，命题 4 的推论 1），从 A 到 End$_D(S)$ 的映射 $a\mapsto a_S$ 是满射的。因而，性质 (i) 和 (ii) 的等价由公式 (9) 得出。

如果 K 的扩张 Z 是可分的，则存在元素 $d\in Z$，使得 Tr$_{Z/K}(d)\not= 0$（V, §8, No. 2，p. 49，命题 1 的推论）。此外，我们还有 Tr$_{D/K}(d) = [D : Z]$ Tr$_{Z/K}(d)$（III, §9, No. 4，p. 548，推论）；因而，如果 $p$ 不除 [D : Z]，则我们有 Tr$_{D/K}(d)\not=$ 0。这证明 (iii) 蕴涵 (ii)。

如果 K 的扩张 Z 不可分离，则对于每个 $x\in Z$，我们有 Tr$_{Z/K}(x) = 0$，因此对于每个 $d\in D$，有 Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) $= 0$。

现在假设 $p$ 除次数 [D : Z]。然后是 D 在 Z 上的除减少的次数。对于每个 $d\in D$，我们有 Tr$_{D/Z}(d) = 0$ (VIII, p. 344, 注)，因而 Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) $= 0$。这就完成了蕴涵 (ii) $\Rightarrow$ (iii) 的证明。

#### 推论 {#alg-viii-s20-n6-cor-1 .statement tag=00MT}

如果域 K 是完美的，则性质 (i) 到 (iii) 成立。

由于域是完美的，K的扩张Z是可分离的（V, §15, No. 5，p. 125，定理3）。 性质 (iii) 然后从VIII、p. 323 的推论 3 得出。

#### 命题 6 {#alg-viii-s20-prop-6 .statement tag=00MU}

令 $\mathscr{S}_0$ 为 K 上的有限维单A-模类集合，并带有非零的迹。 线性形式 (Tr$_S$)$_{S\in\mathscr{S}_0}$ 的家人在 K 上免费。

令F为$\mathscr{S}_0$的有限子集，令S为F的元素。到假设，存在元素$a\in A$使得Tr$_S(a)\not= 0$。根据命题 4 (VIII, p. 83) 的推论 1，存在元素 $b\in A$，使得对于每个 $T\in F-\{S\}$ 都有 $b_S=a_S$ 和 $b_T= 0$。我们有 Tr$_S(b)\not= 0$ 和 Tr$_T(b) = 0$ $T\in F-\{S\}$。因此，族 (Tr$_S$)$_{S\in F}$ 是免费的。接下来是命题6。

#### 注 {#alg-viii-s20-n6-rem-1 .statement tag=00RR}

设$\mathscr{S}_K$是K上的有限维单A-模类集合。命题6也从$\Theta_S$(A)的和得出，对于穿过$\mathscr{S}_K$的S来说，是直接的。

让

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

是 A-模的正合序列，都是 K 上的有限维。通过 III, §9, No. 2、p. 543 的命题 1，我们有 Tr$_E=$ Tr$_{E'}+$ Tr$_{E''}$。由格罗滕迪克群$R_K(A)$（VIII，p. 194）的定义及其泛性质（VIII，p. 186，命题4），存在加法群的同态 $\theta$从$R_K(A)$到$A^*$，其特征为关系$\theta ([E]) =$Tr$_E$，对于K上有限维的每一个A-模E。特别是，E的半化简迹等于E的迹。我们从$\theta$推出K-线性映射$\theta_K: K\otimes_{\mathbf{Z}}R_K(A)\rightarrow A^*$。

#### 推论{#alg-viii-s20-n6-cor-2 .statement tag=00MV}

a) 假设域 K 的特征为 0。同态 $\theta$ 和 $\theta_K$ 是单射的。 K 上的两个有限维半单A-模同构当且仅当它们的特征标相等。

b) 假设域 K 是非零的特征$p$ 的完美。那么同态$\theta_K$是单射的，$\theta$的核是$pR_K(A)$。令 E 为 K 上有限维的半单A-模。线性形式 Tr$_E$ 为零当且仅当存在 A-模 F，使得 E 同构于 $F^p$。

令$\mathscr{S}_K$为K.元素[S]上的有限维单A-模类集合，其中S穿过$\mathbf{Z}$模的$\mathscr{S}_K$、形式基 $R_K$(A)，所以 K-向量空间 $K\otimes_{\mathbf{Z}}R_K(A)$ (VIII, p. 195) 中的元素 $1\otimes [S]$ 形式基。

假设域 K 是完美的。由命题 6 以及 VIII、p. 383、元素 $\theta ([S]) =\theta_K(1\otimes [S]) =$ Tr$_S$ $A^*$ 的推论与 K 线性无关。因此，同态 $\theta_K$ 是内射的，核的同态 $\theta$ 由元素 $\sum_{S\in\mathscr{S}_K}n_S[S]$ 和 $R_K(A)$ 组成，这样每个$S\in \mathscr{S}_K$就有$n_S\cdot 1_K= 0$。因此，$\theta$的核等于$pR_K$(A)，其中$p$是K的特征。特别是，如果K的特征为0，则同态$\theta$是单射的。

a) 的最后一个断言由VIII、p. 190的推论得出。

假设b)的假设满足，并令E为K上有限维的半单A-模。如果存在A-模F，使得E与F同构于$p$子模的直和，则模F为半单且K 上的有限维，我们有 Tr$_E=p$ Tr$_F= 0$。相反，假设 Tr$_E= 0$。我们有$[E]\in pR_K$(A)，所以E中每个单模$S\in \mathscr{S}_K$的重数是$p$的倍数（VIII，p. 190，命题7）；我们可以把它写成$p n_S$和$n_S\in \mathbf{N}$。族$(n_S)$有有限支撑。 集合$F =\oplus_{S\in\mathscr{S}_K}S^{n_S}$。然后我们有 $[E] = [F^p]$，因此 E 和 $F^p$ 同构的（VIII，p. 190，推出）。

设 E 为 K 上有限维的 A-模。设 $a\in A$。用 $\chi_E(a; T)$ 表示 K[T]-模 $E[T] = K[T]\otimes_KE$ (III, §8, No. 11, p. 541) 的自同态 $1_E+ Ta_E$ 的行列式。我们有关系

(10) $\chi_E(a; T)\equiv 1 +$ Tr$_E(a)T$ (mod $T^2K[T]$)

（前述，公式 (49)）。由于该多项式的常数项等于 1，因此它是可逆形式幂级数 (IV, §4, No. 4, p. 30)。此外，如果

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

是 A-模的正合序列，都是 K 上的有限维，那么我们有 $\chi_E(a; T) =\chi_{E'}(a; T)\chi_{E''}(a,T)$ (III, §8, No. 7, p. 534, 公式 (31))。由格罗滕迪克群 $R_K(A)$ (VIII, p. 194) 的定义及其泛性质 (VIII, p. 186, 命题 4)，存在唯一同态 $\chi_a$ 群 $R_K(A)$ 到乘法群 1 + TK[[T]] 使得 $\chi_a([E]) =\chi_E(a; T)$ 对于 K 上有限维的每个 A-模 E。我们从公式 (10) 关系推论

(11) $\chi_a(x)\equiv 1 +\theta (x)(a)T$ (模 $T^2K[[T]]$)

对于 $x\in R_K(A)$ 和 $a\in A$。

如果 E 和 $E'$ 是 K 上有限维的两个 A-模，具有同构半简化，则我们有 $\chi_E(a; T) =\chi_{E'}(a; T)$。

#### 定理 2 {#alg-viii-s20-thm-2 .statement tag=00MW}

设$\mathscr{A}$为K-向量空间A的生成子集。由关系$\chi_{\mathscr{A}}(x) = (\chi_a(x))_{a\in\mathscr{A}}$定义的同态$\chi_{\mathscr{A}}: R_K(A)\rightarrow$(1 + TK[[T]])$^{\mathscr{A}}$是单射的。

令$x$为$R_K(A)$的元素，使得$\chi_{\mathscr{A}}(x) = 1$。根据(11)，对于每个$a\in \mathscr{A}$，我们都有$\theta (x)(a) = 0$，因此也有$\theta (x) = 0$，因为$\theta (x)$是A上的K线性形式，并且$\mathscr{A}$生成K-向量空间A。如果K的特征是零，那么这意味着$x= 0$ (VIII, p. 384, 命题 6 的推论)，因此是本例中的结果。假设从现在开始K的特征$p$是非零的。

让我们首先处理 K 是代数闭的情况。由上述和loc。如上所述，我们就有 $x\in pR_K(A)$。设$y\in R_K(A)$使得$x=py$。对于$\mathscr{A}$中的每一个元素$a$，我们有$\chi_a(y)^p=\chi_a(py) =\chi_a(x) = 1$。所以我们有$(\chi_a(y)-1)^p= 0$，因此有$\chi_a(y) = 1$，因为环 K[[T]] 是整环。所以$y$属于到核共自同态$\chi_{\mathscr{A}}$。接下来是归纳，对于每整数$n \geq 1$，$x$属于到$p^n R_K(A)$。由于$R_K(A)$是一个自由的$\mathbf{Z}$模块，这意味着$x = 0$，因此在这种情况下$\chi_{\mathscr{A}}$具有单射性。

如果$K$不再被认为是代数封闭的，那么我们对$K$进行选择代数闭包$\overline{K}$，并考虑群和群同态的图表

$$
\begin{array}{ccc}
R_K(A) & \xrightarrow{\chi_{\mathscr{A}}} & (1 + TK[[T]])^{\mathscr{A}} \\
|_u & & |_i \\
R_{\overline{K}}(A_{(\overline{K})}) & \xrightarrow{\overline{\chi}_{\mathscr{A}}} & (1 + T\overline{K}[[T]])^{\mathscr{A}},
\end{array}
$$

其中，$u$是同态从$K$到$\overline{K}$（VIII，p. 195）标量的扩张推导出来，$i$是典范嵌入，$\overline{\chi}_{\mathscr{A}}$是同态$z \mapsto (\chi_{1 \otimes a}(z))_{a \in \mathscr{A}}$。由III, §9, No. 1、p. 542、图表(12)的公式(12)是可交换的。由上可知，同态$\overline{\chi}_{\mathscr{A}}$是单射的。由于 $u$ 是单射 (VIII, p. 195, 定理 1)，同态 $\chi_{\mathscr{A}}$ 是单射。

#### 推论 1 {#alg-viii-s20-thm-2-cor-1 .statement tag=00MX}

*设E和F为K上有限维的半单A-模，$\mathscr{A}$为K-向量空间A的生成子集。假设对于每个$a \in \mathscr{A}$，自同态$a_E$和$a_F$的特征多项式为K-向量空间 E 和 F 相等。那么 A-模 E 和 F 同构。*

令 $a$ 为 $\mathscr{A}$ 的元素。 $a_E$和$a_F$的特征多项式具有相同的次数，因此E的维数等于F的维数；我们用$n$表示。令$\mathrm{Pc}_E(a; T)$为$a_E$的特征多项式。在 $K(T)$ 中，我们有等式

$$
\chi_E(a; T) = \det(1 + a_E T) = (-T)^n \det \left( \frac{-1}{T} - a_E \right) = (-T)^n \mathrm{Pc}_E \left( a; \frac{-1}{T} \right),
$$

$\chi_F(a; T)$ 由类似的公式给出。因为我们有假设，所以我们有$\chi_E(a; T) = \chi_F(a; T)$。到定理 2，我们有 [E] = [F]，这意味着 E 和 F 是同构的（VIII，p. 190，命题 7 的推论）。

#### 推论 2 {#alg-viii-s20-thm-2-cor-2 .statement tag=00MY}

*设 A 为 K 上有限次数的中心单代数。设 B 为半单 K-代数，设 f 和 g 为从 B 到 A 的代数同态，并设 $\mathscr{B}$ 为 K-向量空间 B 的生成子集。以下性质是等效的：

(i) A 存在内自同构$\theta$使得$g = \theta \circ f$。
(ii) 对于每个$b \in \mathscr{B}$，我们有$\mathrm{Pc}_{A/K}(f(b); X) = \mathrm{Pc}_{A/K}(g(b); X)$。*当K有特征零时，这些属性等价于以下：

(iii) 对于每$b\in \mathscr{B}$，我们有 Tr$_{A/K}(f(b)) =$ Tr$_{A/K}(g(b))$。

用M和N表示分别将A的加法群赋予外法则$(b, a)\mapsto f(b)a$和$(b, a)\mapsto g(b)a$而获得左B-模。由VIII、p. 257、性质(i)中的命题1等价于B-模M和N同构。通过构造，与B的元素$b$关联的位似$b_M$在A中被留下乘法由$f(b)$；因而，我们有关系

电脑$_M(b; X) =$ 电脑$_{A/K}(f(b); X)$,

Tr$_M(b) =$ Tr$_{A/K}(f(b))$

以及两个类似的关系，其中替换 M 与 N 以及 $f$ 与 $g$。我们知道（VIII，p. 386，推论 1）B-模 M 和 N 是同构的，当且仅当对于每个$b\in \mathscr{B}$，我们都有 Pc$_M(b; X) =$ Pc$_N(b; X)$。当域 K 的特征为 0 时，这个关系也相当于对于每个 $b\in \mathscr{B}$ 的 Tr$_M(b) =$ Tr$_N(b)$（VIII，p. 384，命题 6 的推论）。当 K 具有特征 0 时，属性 (i) 和 (ii) 以及 (i) 和 (iii) 的等价如下。

### 7. 集合类模的系数

令$\mathscr{C}$为A-模的类的遗传集合（VIII，p. 183，定义1）。我们假设型$\mathscr{C}$的每个A-模都是K上的有限维，并用型$\mathscr{C}$的A-模的系数$\Theta_{\mathscr{C}}(A)$集合表示。由VIII、p. 378、集合$\Theta_{\mathscr{C}}(A)$的命题2也是A-线性映射$u: E\rightarrow A^*$的像中的并，其中E经过$\mathscr{C}$；它也是子空间的并 $\Theta_E(A)$ $A^*$，其中 E 穿过$\mathscr{C}$（前述）。 $A^*$的$(A$，A)-子双模族$(\Theta_E(A))_{E\in\mathscr{C}}$是有向的，所以它的并$\Theta_{\mathscr{C}}(A)$是$(A$，A)-$A^*$的子双模。

#### 命题 7 {#alg-viii-s20-prop-7 .statement tag=00MZ}

当且仅当 K 上的有限维的 $A^*$ 的左A-子模包含在 $\Theta_{\mathscr{C}}(A)$ 中，当且仅当它是型 $\mathscr{C}$。

令V为有限维的$A^*$在K上的左A-子模。我们在VIII、p. 379、注3中看到我们有$V\subset \Theta_V(A)$。如果V是型$\mathscr{C}$，那么我们有$\Theta_V(A)\subset \Theta_{\mathscr{C}}$（A），所以V包含在$\Theta_{\mathscr{C}}(A)$中。相反，假设V包含在$\Theta_{\mathscr{C}}(A)$中。由于$\Theta_{\mathscr{C}}(A)$是有向族$(\Theta_E(A))_{E\in\mathscr{C}}$的并，并且V是K上的有限维，因此存在型$\mathscr{C}$的模E，使得V包含在$\Theta_E(A)$中。现在，存在自然数$n$，使得$\Theta_E(A)$同构于$E^n$商（VIII，p. 378，命题2）。由于$\mathscr{C}$是遗传性的，V是型$\mathscr{C}$。

#### 推论{#alg-viii-s20-n7-cor-1 .statement tag=00N0}

设 E 为 K 上有限维的 A-模。则当且仅当 $\Theta_E(A)$ 包含在 $\Theta_{\mathscr{C}}(A)$ 中时，E 为型 $\mathscr{C}$。

条件显然是必要的。

相反，假设$\Theta_{\mathscr{C}}(A)$包含于$\Theta_E(A)$。 A-模 $\Theta_E(A)$ 是 K (VIII, p. 378, 命题 2) 上的有限维，因此它是型 $\mathscr{C}$ × 命题 7。现在，存在整数 $n\geqslant 0$ 使得 E 为同构于 $\Theta_E(A)^n$ (VIII, p. 378, 命题 2) 的A-子模。由于$\mathscr{C}$是遗传性的，所以E是型$\mathscr{C}$。

### 8. 余代数结构受限双轨

对于 A 中的任意 $a$，我们用 θ(A) 上的 $\eta (a)$ 线性形式 $f\mapsto f(a)$ 表示。因此，我们从 A 定义 K-线性映射 $\eta$ 到向量空间 θ(A) 的对偶 $\Theta (A)^*$。 集合$\varepsilon =\eta (1)$。

#### 命题 8 {#alg-viii-s20-prop-8 .statement tag=00N1}

在向量空间 θ(A) 上，存在唯一的余代数结构 (III, §11, No. 1, p. 574)，使得映射 $\eta : A\rightarrow \Theta (A)^*$ 是从A 到θ(A) 的对偶代数 (III, §11, No. 2, p. 579) 的同态。 余代数 θ(A) 是共结合的并且承认$\varepsilon$ 为余单位。

对于每个整数$n\geqslant 1$，考虑K-线性映射$j_n$从$\Theta (A)^{\otimes n}$到特征为公式的对偶$A^{\otimes n}$

$$
\langle j_n(f_1\otimes  \cdots  \otimes f_n), a_1\otimes  \cdots  \otimes a_n\rangle =\prod_{i=1}^n\langle f_i, a_i\rangle \tag{13}
$$

对于$A^n$中的$(a_i)$和$\Theta (A)^n$中的$(f_i)$。到命题 16，II, §7, No. 7、p. 308、映射 $j_n$ 的 (ii) 是单射的。分别用K和A中的乘法推导出$m_K: K\otimes K\rightarrow K$和$m_A: A\otimes A\rightarrow A$映射表示。对于 $f, g\in \Theta (A)$ 和 $a, b\in A$，我们有

$$
\langle j_2(f\otimes g), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(f\otimes g)
$$

因此我们有

$$
\langle j_2(t), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(t) \tag{14}
$$

对于每个$t\in \Theta (A)\otimes \Theta (A)$。

#### 引理 2 {#alg-viii-s20-lem-2 .statement tag=00RS}

设$c : \Theta(A) \to \Theta(A) \otimes \Theta(A)$为K-线性映射。 Then $\eta$ is a homomorphism from $A$ to the dual algebra of the cogebra $(\Theta(A), c)$ if and only if the following diagram commutes:

$$
\begin{array}{ccc}
\Theta(A) & \xrightarrow{c} & \Theta(A) \otimes \Theta(A) \\
| & & | \\
A^* & \xrightarrow{t m_A} & (A \otimes A)^*
\end{array}
$$

Indeed, $\eta$ is a homomorphism from $A$ to the dual algebra of the cogebra $(\Theta(A), c)$ if and only if we have $\eta(ab) = m_K \circ (\eta(a) \otimes \eta(b)) \circ c$ for all $a, b \in A$, that is

$$
\eta(ab)(f) = m_K \circ (\eta(a) \otimes \eta(b))(c(f))
$$

对于 $a, b \in A$ 和 $f \in \Theta(A)$。现在，我们有

$$
\eta(ab)(f) = f(ab) = \langle t m_A(j_1(f)), a \otimes b \rangle
$$

并且，通过 (14)，

$$
m_K \circ (\eta(a) \otimes \eta(b))(c(f)) = \langle j_2(c(f)), a \otimes b \rangle
$$

对于所有$a, b \in A$和每个$f \in \Theta(A)$。接下来是引理。

由于$j_2$是单射的，因此最多存在一个线性映射$c$使得图表高于通勤。 为了证明它的存在，我们必须证明$t m \circ j_1$的像包含在$j_2$的像中。 在其他字中，我们必须证明存在，对于$\Theta(A)$的每个元素$f$，自然数$n$和$\Theta(A)$满足关系的元素$f'_1, \ldots, f'_n, f''_1, \ldots, f''_n$

$$
f(ab) = \sum_{i=1}^n f'_i(a) f''_i(b)
$$

对于$a, b \in A$。然后我们将有

$$
c(f) = \sum_{i=1}^n f'_i \otimes f''_i.
$$

由VIII、p. 379的推论，在$K$上存在有限维的左$A$模$E$，以$f$为系数。令$(e_1, \ldots, e_n)$为$E$的基、$(e_1^*, \ldots, e_n^*)$对偶基、$E$的$x$元素以及$E^*$的$x^*$元素，使得$f = c_E(x, x^*)$。 集合 $f'_i = c_E(e_i, x^*)$ 和 $f''_i = c_E(x, e_i^*)$ $i \in [1, n]$；对于 A 中的 a、b，我们有

$$
f(ab) = \langle x^*, abx \rangle = \langle x^* a, bx \rangle = \left\langle \sum_i \langle x^* a, e_i \rangle e_i^*, bx \right\rangle
$$
$$
= \sum_i \langle x^* a, e_i \rangle \langle e_i^*, bx \rangle = \sum_i \langle x^*, ae_i \rangle \langle e_i^*, bx \rangle = \sum_i f_i'(a) f_i''(b),
$$
因此 (16)。

让我们证明 c 的共结合性。为此，请考虑 K-线性映射
$$
c' = (c \otimes 1_{\Theta(A)}) \circ c \quad \text{and} \quad c'' = (1_{\Theta(A)} \otimes c) \circ c
$$
从$\Theta(A)$到$\Theta(A)^{\otimes 3}$。我们有关系
$$
\langle j_3(f \otimes c(g)), a \otimes b \otimes c \rangle = \langle f, a \rangle \langle j_2 \circ c(g), b \otimes c \rangle
$$
$$
= \langle f, a \rangle \langle g, bc \rangle
$$
$$
= \langle j_2(f \otimes g), a \otimes bc \rangle
$$
$$
= \langle t(\mathrm{Id}_A \otimes m_A) \circ j_2(f \otimes g), a \otimes b \otimes c \rangle
$$
对于 $f, g \in \Theta(A)$ 和 $a, b, c \in A$。由此，我们推断出以下图表是通勤的：

$$
\begin{array}{ccc}
\Theta(A) \otimes \Theta(A) & \xrightarrow{\mathrm{Id}_{\Theta(A)} \otimes c} & \Theta(A) \otimes \Theta(A) \otimes \Theta(A) \\
\downarrow j_2 & & \downarrow j_3 \\
(A \otimes A)^* & \xrightarrow{t(\mathrm{Id}_A \otimes m_A)} & (A \otimes A \otimes A)^*.
\end{array}
$$

由于图表的交换律和(15)，对于$f \in \Theta(A)$和$a, a', a'' \in A$，我们有
$$
\langle j_3 \circ c'(f), a \otimes a' \otimes a'' \rangle = \langle f, (aa')a'' \rangle;
$$
我们可以展示关系
$$
\langle j_3 \circ c''(f), a \otimes a' \otimes a'' \rangle = \langle f, a(a'a'') \rangle
$$
同样。由于 A 中的乘法是结合律，因此我们有 $j_3 \circ c' = j_3 \circ c''$，因此也有 $c' = c''$，因为 $j_3$ 是单射的。

最后，公式(16)和(17)意味着$\Theta(A)$承认$\varepsilon$为余单位。

#### 注 1 {#alg-viii-s20-n8-rem-1 .statement tag=00N2}

令$(\mathbf{V}, \pi)$为代数A的有限维线性表示。让我们介绍V的基$(e_1, \ldots, e_n)$和$\mathbf{V}^*$的对偶基$(e_1^*, \ldots, e_n^*)$。到引理 2 的证明时，我们有关系
$$
c(c_\pi(x, x^*)) = \sum_{k=1}^n c_\pi(e_k, x^*) \otimes c_\pi(x, e_k^*)
$$

对于 $x\in V$ 和 $x^*\in V^*$。对于 $1\leqslant i, j\leqslant n$、集合 $\pi_{ij}=c_{\pi}(e_j, e^*_i)$。对于每个$a\in A$，$\pi (a)$的矩阵相对于V的基$(e_1, . . . , e_n)$等于$(\pi_{ij}(a))$。对于 $1\leqslant i\leqslant n$ 和 $1\leqslant j\leqslant n$，我们有

$$
c(\pi_{ij}) =\sum_{k=1}^n\pi_{ik}\otimes \pi_{kj} \tag{20}
$$

#### 定义 3 {#alg-viii-s20-def-3 .statement tag=00N3}

令C为余代数超过域K，并且$c$为余积。 C的子余代数是C的任何线性子空间$C_1$，使得$c(C_1)$包含在$C\otimes_KC$中的$C_1\otimes_KC_1$的典范像中。

设$j$为$C_1$到C的典范嵌入。通过这个定义，存在唯一的线性映射$c_1: C_1\rightarrow C_1\otimes_KC_1$，这样我们有

$$
c\circ j= (j\otimes j)\circ c_1 \tag{21}
$$

这个关系意味着$j$是余代数从$(C_1, c_1)$到$(C, c)$的态射（III, §11, No. 1，p. 574）。

如果 C 是共结合的，则 $C_1$ 是共结合的。如果 C 是可交换的，那么 $C_1$ 也是可交换的。如果C有余单位$\varepsilon$，那么$\varepsilon$到$C_1$的限制就是$C_1$的余单位。

#### 命题 9 {#alg-viii-s20-prop-9 .statement tag=00N4}

令 θ 为 θ(A) 的线性子空间。以下属性是等效的：

(i) θ 是 θ(A) 的 $(A,A)$ 子双模。

(ii) θ 是 θ(A) 的子余代数。

(iii) 在 K 上存在类 A-模有限维的遗传集合$\mathscr{C}$，使得 $\Theta  = \Theta_{\mathscr{C}}(A)$。

当(iii)中提到的这些性质成立、集合$\mathscr{C}$唯一确定时。

最后一个断言由VIII、p. 388的推论得出：集合$\mathscr{C}$由有限维的A-模E的类在K上组成，使得$\Theta_E(A)$包含在θ中。

(iii)$\Rightarrow$(ii)：设$\mathscr{C}$为有限维的A-模的类的世袭集合，则$\Theta_{\mathscr{C}}(A)$为有向家族$(\Theta_E(A))_{E\in\mathscr{C}}$的并。由于对于每个 $E\in \mathscr{C}$ (VIII, p. 390, 公式 (19))，$\Theta_E(A)$ 是 θ(A) 的子余代数，因此对于 $\Theta_{\mathscr{C}}(A)$ 也是如此。

(ii) $\Rightarrow$ (i): 令$f\in \Theta (A)$。设 $f'_1, . . . , f'_n, f''_1, . . . , f''_n$ 为 θ(A) 满足 $c(f) =\sum f'_i\otimes f''_i$ 的元素。对于 A 中的 $a,b$，我们有 $f(ab) =\sum f'_i(a)f''_i(b)$，因而

$$
bf=\sum_{i=1}^nf''_i(b)f'_i,f a=\sum_{i=1}^nf'_i(a)f''_i
$$

（VIII、p. 375、公式（3）和（4））。因而， θ(A) 的子余代数是 $(A$, A)-子双模。

(i) $\Rightarrow$ (iii)：假设 θ 是 θ(A) 的$(A$, A)-子双模；令$\mathscr{C}$为有限维的类或A-模E的集合除以K，使得$\Theta_E(A)$包含在θ中。 集合 $\mathscr{C}$ 是遗传性的（VIII、p. 377、注 2），我们通过构造得到了$\Theta_{\mathscr{C}}(A)\subset \Theta$。设$f\in \Theta$和$E = Af$。那么 E 在 K 上是有限维的。因而，E 上的每个线性形式都是形式 $u_a:g\mapsto g(a)$，其中 A 中的$a$（II, §7, No. 5，p. 302，推论 2）。现在，对于 $a, b, x\in A$，我们有

$$
c_E(af, u_b)(x) =\langle u_b, xaf\rangle =f(bxa) =af b(x)
$$

这样$c_E(af, u_b) =af b$。因此我们有$\Theta_E(A)\subset \Theta$。因而，A-模 E 是型 $\mathscr{C}$，$f$ 是其系数之一。因而，我们有 $\Theta \subset \Theta_{\mathscr{C}}(A)$，最后是 $\Theta  = \Theta_{\mathscr{C}}(A)$。

#### 注 2 {#alg-viii-s20-n8-rem-2 .statement tag=00N5}

令 θ 为 θ(A) 的子余代数。我们赋予 K 离散的拓扑和代数 A 赋予最粗糙的拓扑，其中映射 $f: A\rightarrow K$ 对于 $f$ 穿过 θ 是连续的（Gen. Top.、I, §2, No. 2、p. 175）。这个拓扑赋予A拓扑K-模的结构。 A 的双面理想 $\mathfrak{a}$ 是开的，当且仅当它有有限余维并且它的正交$\mathfrak{a}'$ 包含在 θ 中。通过VIII、p. 379的命题 3，形式的开放两侧理想是A中0邻域的基本系统。因而，A上的拓扑与其环结构兼容。

令$\mathscr{C}$为有限维的A-模的类在K上的遗传集合，使得$\Theta  = \Theta_{\mathscr{C}}$(VIII，p. 391，命题9)。令 E 为 K 上的有限维的左A-模。我们赋予它离散的拓扑。以下属性是等效的：

(i) A-模 E 为型 $\mathscr{C}$。

(ii) A-模 E 中的湮没子在 A 中打开。

(iii) 映射$(a, x)\mapsto ax$从$A\times E$到E是连续的。

最后一个性质意味着E是一个拓扑A-模。

令 $\Theta^*$ 为余代数 θ 的对偶代数。我们赋予$\Theta^*$最粗糙的拓扑，其中映射$\varphi \mapsto \varphi (u)$从$\Theta^*$到K，对于$u$穿过θ，是连续的。 代数上的拓扑 $\Theta^*$ 与$\Theta^*$ 上的加法群结构兼容。 形式$\Theta_E$(A)的集合$\Theta^*$的正交，其中E是型$\mathscr{C}$的A-模，形式邻域0的基本系统。现在，这样的集合是θ 的子余代数，因此其正交是 $\Theta^*$ 的理想。因此，$\Theta^*$ 上的拓扑与其环结构兼容。规范的代数同态 $\eta : A\rightarrow \Theta^*$（将 $a\in A$ 发送到 θ 上的线性形式 $f\mapsto f(a)$）定义同构来自 A 的完整 Hausdorff 空间 $\widehat{A}$（Gen. Top.， II, §3, No. 7、p. 191) 至 $\Theta^*$。

### 习题 {#alg-viii-s20-exercises}

§ 20](exercises/s20/)参见[习题。
