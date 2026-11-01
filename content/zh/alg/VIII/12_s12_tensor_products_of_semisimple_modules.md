---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 12
section_title: Tensor Products of Semisimple Modules
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.211-A VIII.228
pdf_pages: 0228-0245
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules over Tensor Products of Algebras
      page: 211
      pdf_page: 228
    - "no": 2
      title: Tensor Products of Simple Modules
      page: 213
      pdf_page: 230
    - "no": 3
      title: Tensor Products of Semisimple Commutative Algebras
      page: 215
      pdf_page: 232
    - "no": 4
      title: The Radical of a Tensor Product of Algebras
      page: 217
      pdf_page: 234
    - "no": 5
      title: Tensor Products of Semisimple Modules
      page: 218
      pdf_page: 235
    - "no": 6
      title: Tensor Products of Semisimple Algebras
      page: 221
      pdf_page: 238
    - "no": 7
      title: Extension of Scalars in Semisimple Modules
      page: 222
      pdf_page: 239
statements: 26
exercises: 17
content_sha256: 65753d384d055e0af1b8a71fa915b254d2cebb5b1bb6b5be4714ca4e2fcb8665
translated_from: content/en/alg/VIII/12_s12_tensor_products_of_semisimple_modules.md
translation_method: google
source_content_sha256: b311e3c926d1c35b21ba3909e0ec3e0584eb38f0337ee0f5d814716a0a8f67c8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 9d2468a93b9de4c2a9426c4c084a84037099e29b46cbcf3b537d626575ba2c5c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 12。 张量积 / 半单模

在这个截面中，字母K表示交换域。如果 E 和 F 在 K 上向量空间，那么我们用 $E\otimes F$ 表示张量积 $E\otimes_KF$。

### 1. 半单模超过张量积共代数

在这个小节中，我们考虑K-代数$A_1$和$A_2$；我们用 A 表示代数 $A_1\otimes A_2$。

#### 命题 1 {#alg-viii-s12-prop-1 .statement tag=00E6}

令$M_1$为$A_1$模，$M_2$为$A_2$模，均不减至0。如果模$M = M_1\otimes M_2$超过环$A = A_1\otimes A_2$是简单的（分别为同典型，半单），则$A_1$-模块$M_1$和$A_2$-模块$M_2$很简单（分别是同型，半单）。

假设M是半单A-模。令 $N_1$ 为 $M_1$ 的 $A_1$ 子模块。用N表示A-模 M中$N_1\otimes M_2$的典范像。根据VIII、p. 56的推论2，M中存在投影算子$p$，且像 N。由假设，我们有$M_2\not= 0$；因而，我们可以在K-向量空间$M_2$上对$M_2$和线性形式$\varphi$进行选择元素$m$，使得$\varphi (m) = 1$（II, §7, No. 5，p. 302，推论2）。令$u$为从$M_1$到由$u(m_1) =m_1\otimes m$定义的M的映射，并令$v$为从M到由$v(m_1\otimes m_2) =\varphi (m_2)m_1$表征的$M_1$的K-线性映射。 集合$q=v\circ p\circ u$。 映射$q: M_1\rightarrow M_1$是$A_1$线性，它的像包含在$N_1$中，并且对于每个$n\in N_1$我们有$q(n) =n$。因而，$q$ 是$M_1$ 中的投影算子和像 $N_1$。我们已经证明$M_1$是半单$A_1$模（VIII，p. 56，推论2）。

假设 M 很简单，并且 $M_1$ 是两个 $A_1$ 子模块 $M'_1$ 和 $M''_1$ 的直和。 集合$M'= M'_1\otimes M_2$和$M''= M''_1\otimes M_2$；那么M是A-子模$M'$和$M''$的直和。由于M很简单，$M'$或$M''$必须减少到0；因为我们有$M_2\not= 0$乘假设，所以我们有$M'_1= 0$或$M''_1= 0$（II, §3, No. 7，p. 256，推论2）。这证明$M_1$是一个简单的$A_1$模块。

现在假设 M 是同型A-模。令 S 和 T 为简单的$A_1$-$M_1$ 的子模块。 A-模$S\otimes M_2$和$T\otimes M_2$可以与M的非零的子模识别。因此它们与M具有相同的型的同型性。通过注VIII、p. 61，存在非零的 A-线性映射$f: S\otimes M_2\rightarrow T\otimes M_2$。 映射$f$尤其是$A_1$-线性。由于$A_1$模$S\otimes M_2$和$T\otimes M_2$分别是非零的且同型为型S和T，因此S和T是同构的。这证明$M_1$是同典型的$A_1$模。

#### 命题 2 {#alg-viii-s12-prop-2 .statement tag=00E7}

令 S 为环 $A = A_1\otimes A_2$ 上的单模，K 上的有限维。对于 $i\in  \{1,2\}$，存在一个简单的 $A_i$ 模 $S_i$，使得 $A_i$ 模 S 与型 $S_i$ 同型分支的。 A-模 S 同构于A-模 $S_1\otimes S_2$ 的商。

由于S是非零的$A_1$模，在K上是有限维的，因此它在$A_1$上有有限长度，并且存在一个简单的左$A_1$模$S_1$和非零的$A_1$-从$S_1$到S的线性映射。我们赋予$M_2=$Hom$_{A_1}(S_1,S)$，具有由外法则$(a_2, u)\mapsto (a_2)_S\circ u$定义的左$A_2$模块结构。我们通过构造得到$M_2\not= 0$，并且$M_2$是K上的有限维。因此，我们可以找到一个简单的左$A_2$-模$S_2$和非零的$A_2$-线性映射$\varphi : S_2\rightarrow M_2$。我们从 $S_1\otimes S_2$ 定义非零的 A-线性映射 $\psi$ 到 S

$$
\psi (s_1\otimes s_2) =\varphi (s_2)(s_1) \tag{1}
$$

对于每个 $s_1\in S_1$ 和 $s_2\in S_2$。由于 S 是单A-模并且 $\psi$ 不是零，因此 $\psi$ 是满射，并且 S 与 $S_1\otimes S_2$ 的商同构。对于$i\in  \{1,2\}$，$A_i$-模$S_1\otimes S_2$是型$S_i$的同型，因此$A_i$-模S（VIII，p. 61，命题2）也是同型的。

对于任何K-代数 B，我们用简单（VIII，p. 51）左B-模的类的$\mathscr{S}_K(B)$集合表示，它们是K上的有限维。

#### 定理 1 {#alg-viii-s12-thm-1 .statement tag=00E8}

假设域 K 是代数封闭的。

a) 设 $M_1$ 是一个 $A_1$ 模，$M_2$ 一个 $A_2$ 模，都是 K 上的简单（分别是半单）和有限维。那么 $M_1\otimes M_2$ 是一个简单（分别是半单）模环 $A_1\otimes A_2$ 并且是 K 上的有限维。

b) 映射从$\mathscr{S}_K(A_1)\times \mathscr{S}_K(A_2)$到$\mathscr{S}_K(A_1\otimes A_2)$，发送(cl(S$_1$), cl(S$_2$))到cl(S$_1\otimes S_2$)，其中$S_1($resp。 $S_2)$ 是一个简单的 $A_1$ 模（分别为 $A_2$ 模），它是 K 上的有限维，是双射的。

为了证明部分a)，只要考虑$M_1$和$M_2$是简单的情况就足够了。设$M'$为$M = M_1\otimes M_2$的A-子模；它是$M_1\otimes M_2$的$A_1$子模，在形式$1_{M_1}\otimes u$的自同态集合下稳定，其中$u$贯​​穿$A_2$模$M_2$的同调集合。由于域 K 是代数闭集，Schur 的引理 (VIII, p. 47, 定理 1) 意味着 $M_1$ 的交换端 End$_{A_1}(M_1)$ 等于 K。 由 VIII 的推论 2， $M_1\otimes M_2$的p. 63、A-子模$M'$属于形式$M_1\otimes M'_2$，其中$M'_2$是$M_2$的$A_2$子模。我们假设 $M_2$ 是简单的；因此我们有$M'_2= 0$或$M'_2= M_2$，即$M'= 0$或$M'= M$。因而，M 很简单。

If S is 单模 over $A_1\otimes A_2$ that is finite-dimensional over K, then it follows from 命题 2 and 部分 a) that S is isomorphic to 模 of 形式 $S_1\otimes S_2$, where $S_1$ (resp. $S_2$) is a simple $A_1$-模块（分别为$A_2$-模块）。此外，作为$A_i$模，S是型$S_i$的同型，因而$S_i$的类仅取决于S的类。这就证明了部分b)。

#### 注 1 {#alg-viii-s12-n1-rem-1 .statement tag=00E9}

当域 K 不假设为代数封闭时，定理 1 的断言 a) 不再成立。我们可以给出例 (VIII, p. 225, 习题 4)，其中 $M_i$ 是一个简单的 $A_i$ 模，对于 $i\in  \{1,2\}$，它是 K 上的有限维，并且其中 A-模 $M_1\otimes M_2$ 不是半单或者是半单但并不简单。

#### 注 2 {#alg-viii-s12-n1-rem-2 .statement tag=00EA}

从$R_K(A_1)\otimes_{\mathbf{Z}}R_K(A_2)$到$R_K(A)$，存在以关系$\varphi ([M_1]\otimes [M_2]) = [M_1\otimes M_2]$为特征的同态$\varphi$。这可以用与VIII、p. 196的命题9相同的方式证明。如果域 K 是代数闭集，则 $\varphi$ 是从 $R_K(A_1)\otimes_ZR_K(A_2)$ 到 $R_K(A)$ 乘定理 1 的同构，b) 因为对于每个 K-代数 B，$\mathbf{Z}$ 模 $R_K(B)$ 对于基族是自由的$([S])_{S\in\mathscr{S}_K(B)}$（VIII，p. 195）。

### 2. Tensor Products of Simple Modules

令$A_1$和$A_2$为代数超过交换域K。我们用A表示K-代数$A_1\otimes A_2$。

#### 引理 1 {#alg-viii-s12-lem-1 .statement tag=00RB}

令$M_1$和$N_1$为$A_1$-模块，并令$M_2$和$N_2$为$A_2$-模块。我们制作以下假设：

(i) $A_1$-模块$M_1$ 是有限生成的。

(ii) $A_2$-模$M_2$是有限生成的，或者$N_1$是K上的有限维。

集合$M = M_1\otimes M_2$和$N = N_1\otimes N_2$，并将它们视为模超过环$A = A_1\otimes A_2$。 典范同态 (II, §3, No. 5, p. 251)

$\lambda :$ 坎$_K(M_1,N_1)\otimes$ 坎$_K(M_2,N_2)\longrightarrow$ 坎$_K(M,N)$

然后诱导同构 / K-向量空间

$\varphi :$坎$_{A_1}(M_1,N_1)\otimes$坎$_{A_2}(M_2,N_2)\longrightarrow$坎$_A(M,N)$。

映射 $\lambda$ 是单射 (II, §7, No. 7、p. 308、命题 16)，并将线性子空间 Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ 发送到 Hom$_A(M,N)$。因此，只要证明从 M 到 N 的每个A-线性映射，Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ 的属于到像乘$\lambda$就足够了。设$u: M\rightarrow N$为A-线性映射。让$x\in M_1$。用$u_x$表示从$M_2$到$N_1\otimes N_2$的$A_2$线性映射$y\mapsto u(x\otimes y)$。 集合 P = Hom$_{A_2}(M_2,N_2)$，并用$\nu$典范同态表示从$N_1\otimes P$到Hom$_{A_2}(M_2,N_1\otimes N_2)$（II, §4, No. 2，p. 269）。这个映射是单射的（II, §4, No. 2，p. 269，命题2，（i）应用于K-向量空间$N_1$）。到假设 (ii)，存在$N_1$的线性子空间$V_x$，K上的有限维，使得$u_x$在$V_x\otimes N_2$中呈现值。因此，$u_x$ 是像，$\nu$ 是唯一元素 $v_x$，$N_1\otimes P$。 映射$\widetilde{u}:x\mapsto v_x$从$M_1$到$N_1\otimes P$是$A_1$线性。通过假设 (i)，有限生成$A_1$-模$M_1$。 推理类似上面显示Hom$_{A_1}(M_1,N_1\otimes P)$中Hom$_{A_1}(M_1,N_1)\otimes P$的$\widetilde{u}$属于到像。接下来是引理 1。

#### 定理 2 {#alg-viii-s12-thm-2 .statement tag=00EB}

设$A_1$和$A_2$为代数超过交换域K；令 $S_1$ 为简单的 $A_1$ 模块，$S_2$ 为简单的 $A_2$ 模块。令$D_1$和$D_2$分别为$S_1$和$S_2$的交换子。 集合$M = S_1\otimes S_2,A = A_1\otimes A_2$和$D = D_1\otimes D_2$。我们将 M 视为左 $(A,D)$ 双模。

a) A-模 M 的交换子等于 $D_M$。

b) 映射 $\mathfrak{a}\mapsto \mathfrak{a}M$ 是从 D 右理想的集合（按包含排序）到 M 的 A-子模的集合（按包含排序）的同构。逆映射将M的子模N发送到元素$d$的理想D由……组成，使得$dM\subset N$。

断言 a) 由引理 1 得出，因为单模是单生的。

令 T 为 $(A_1,D_2$)-双模 $S_1\otimes (D_2)_d$。我们认同$M = S_1\otimes S_2$与$T\otimes_{D_2}S_2$（II, §3, No. 8，p. 258）；此标识与结构、左模、环$A = A_1\otimes A_2$相容的。

令 N 为 M 的A-子模；它是$T\otimes_{D_2}S_2$的$A_2$子模块，在形式$(a_1)_T\otimes 1_{S_2}$的自同态稳定，对于$a_1$运行到$A_1$。由VIII、p. 63的推论2得出，存在唯一的T的$(A_1,D_2)$子双模V，使得$N = V\otimes_{D_2}S_2$。

由$u(s\otimes d) = 1\otimes d\otimes s$定义的从$T = S_1\otimes (D_2)_d$到$((D_1)_d\otimes (D_2)_d)\otimes_{D_1}S_1$的同构$u$是$(A_1,D_2$）-线性。我们认同这些$(A_1,D_2)$双模块。与上面给出的类似，推理证明$D_1\otimes D_2$的右$(D_1\otimes D_2$)子模块$\mathfrak{a}$的存在和唯一性使得$V =\mathfrak{a}\otimes_{D_1}S_1$。由上式可知，$\mathfrak{a}$是$D = D_1\otimes D_2$的唯一右理想，使得$N =\mathfrak{a}M$。

我们刚刚证明了映射$\mathfrak{a}\mapsto \mathfrak{a}M$是双射的；接下来是最后一个断言。

#### 推论 1 {#alg-viii-s12-thm-2-cor-1 .statement tag=00EC}

模$S_1\otimes S_2$超过环$A_1\otimes A_2$是半单（分别是同型、简单）当且仅当环$D = D_1\otimes D_2$是半单（分别是简单、域）。特别是，如果 $S_1$ 或 $S_2$ 的交换子等于 K，则 $S_1\otimes S_2$ 是简单的。

定理 2 时，环 $D_1\otimes D_2$ 上的模 $S_1\otimes S_2$ 是半单（分别为同型、简单）当且仅当右D-模 $(D_1\otimes D_2)_d$ 是 (VIII， p. 109、命题10)。现在右D-模$D_d$是简单的当且仅当D是域；它是同典型的（分别半单）当且仅当环 D 是简单的（分别半单）（VIII，p. 120，定义 1；VIII，p. 121，推论 1；并且VIII、p. 137、命题 2)。

#### 推论 2 {#alg-viii-s12-thm-2-cor-2 .statement tag=00ED}

我们有$\mathfrak{R}_A(M) =\mathfrak{R}(D)M$。 A-模 M 没有部首当且仅当环 D 没有部首。

这是从 VIII、p. 108 和定理 2, b) 中的命题 8 得出的。

### 3. 张量积 / 半单交换代数

#### 定理 3 {#alg-viii-s12-thm-3 .statement tag=00EE}

设$Z_1$和$Z_2$为K上的半单交换代数。环$Z_1\otimes Z_2$的根式等于其幂零元的集合。

让我们首先处理$Z_1$和$Z_2$为扩张$L_1$和$L_2$为域K时的情况。如果需要的话，通过交换$L_1$和$L_2$，我们将约化处理为超越时的情况K 上$L_1$ 的次数小于 K 上$L_2$ 的次数。 $L_2$ 的选择代数闭包 Ω；根据V, §14, No. 6、p. 114的定理 5的推论1，我们可以假设$L_1$是Ω的子扩展。

A) 首先证明$L_1\otimes L_2$的部首包含在$L_1\otimes \Omega$的部首中。 集合$\mathfrak{a}=\mathfrak{R}(L_1\otimes L_2)(L_1\otimes \Omega )$；它是交换环$L_1\otimes \Omega$的理想，我们必须证明认为$\mathfrak{a}$包含在$L_1\otimes \Omega$的部首中。在其他字（VIII，p. 156，定理1）中，我们必须证明对于$x\in \mathfrak{a}$，元素$1 +x$在$L_1\otimes \Omega$中是可逆的。现在，由于Ω是$L_2$的代数扩张，因此存在$L_2$、有限次数的扩张$L_3$，使得$x$属于到$\mathfrak{R}(L_1\otimes L_2)(L_1\otimes L_3)$。显然只要证明$1 +x$在$L_1\otimes L_3$中可逆即可。现在，$C = L_1\otimes L_3$ 有限生成模超过环 $B = L_1\otimes L_2$。根据VIII、p. 175的推论，我们有$\mathfrak{R}(B)C\subset \mathfrak{R}$(C)，因此$x$属于对于C和$1 +x$的根式在C中是可逆的。

B) 让我们证明$L_1\otimes \Omega$的部首由幂零元组成。用 $p$ 表示 K 的特征指数，并用 P 表示 Ω 中 K 的相对 $p$ 根式（即纯粹不可分离的）闭包（V, §5, No. 2，p. 25）； 域 P 很完美。由于 P 是 K 的代数扩张，因此我们有 $L_1(P) = L_1[P]$（V, §3, No. 2，p. 18，推论 1）。令$\mathfrak{b}$为从$L_1\otimes P$到域$P_1= L_1[P]$的典范同态中的核。让$x\in \mathfrak{b}$；存在 P 的 $L_1$ 的元素 $y_1, . . . , y_n$ 和元素 $z_1, . . . , z_n$，使得 $x=\sum^n_{i=1}y_i\otimes z_i$ 和 $\sum_{i=1}^ny_iz_i= 0$。由于 P 是 K 上的 $p$ 根，因此存在 $p$ 的幂 $q$，使得 $z^q_1, . . . , z_n^q$ 属于到 K。然后我们有

$$
x^q=\sum_{i=1}^ny^q_i\otimes z_i^q=\sum_{i=1}^ny^q_iz_i^q\otimes 1 =(\sum_{i=1}^ny_iz_i)^q\otimes 1 = 0
$$

所以$\mathfrak{b}$由幂零元组成。

集合$\mathfrak{c}=\mathfrak{b}\otimes_P\Omega$；由上式可知，从$(L_1\otimes P)\otimes_P\Omega$到$P_1\otimes_P\Omega$是典范同态中的核，由幂零元构成。 现在，Ω 是 P 的代数闭扩张，$P_1$ 是 Ω 的子扩展。 由于域 P 是完美的，$P_1$ 是 P 的可分扩张 (V, §15, No. 5, p. 125, 定理 3)。 通过V的定理 4，交换环$P_1\otimes_P\Omega$的最大理想的p. 120、交减少到0。 在其他字中，与$((L_1\otimes P)\otimes_P\Omega )/\mathfrak{c}$同构的环$P_1\otimes_P\Omega$没有部首。 这就证明了 (VIII, p. 155, 命题 5) $\mathfrak{c}$ 包含环 $(L_1\otimes P)\otimes_P\Omega$ 的根式。 现在，这个环与$L_1\otimes \Omega$同构，$\mathfrak{c}$由幂零元组成。 因此，$L_1\otimes \Omega$的部首由幂零元组成。

C) 具体情况下证明结束。通过A)和B)，$L_1\otimes L_2$的部首$\mathfrak{r}$包含在该交换环的幂零元的集合$\mathfrak{n}$中。我们还知道$\mathfrak{n}$包含在$\mathfrak{r}$（VIII，p. 157，注2）中。

现在考虑一般情况。由于半单交换K-代数是域K的有限多个扩张（VIII，p. 137，命题3）的乘积，并且环的乘积的根部是乘积根部（VIII，p. 156，推论3），$Z_1\otimes Z_2$的根部是这个环的幂零元的集合。

### 4. 代数张量积的根式

设$A_1$和$A_2$为K-代数，并设$A = A_1\otimes A_2$。

#### 命题 3 {#alg-viii-s12-prop-3 .statement tag=00EF}

假设代数$A_1$和$A_2$是半单，分别是中心$Z_1$和$Z_2$。 集合$Z = Z_1\otimes Z_2$。

a) 映射 $\mathfrak{a}\mapsto \mathfrak{a}A$ 是从 Z 理想的集合（按包含排序）到 A 两侧理想的集合（按包含排序）的同构。

b) A 的根式等于 A 的最大两侧理想的交并且等于 $\mathfrak{R}(Z)A$。

c) 如果 K-代数 $Z_1$ 和 $Z_2$ 之一是可分的，特别是如果域 K 是完美的，则环 Z 和 A 的根式被约化为 0。

每个代数 $A_i$ 都是有限多个单代数中的乘积。 现在，环的乘积的中心是中心的乘积，并且我们有类似的断言用于根式（VIII，p. 156，推论3）和双面理想（I, §8, No. 10，p. 109， 命题8)。 因此，只要证明假设下的命题3，$A_1$和$A_2$是单代数即可。

对于 $i\in  \{1,2\}$、集合 $B_i= A_i\otimes A^o_i$，并将 $A_i$ 视为 $B_i$ 模，其中同位由公式给出

$$
(x\otimes y)z=xzy
$$

对于$x,y$，以及$A_i$中的$z$。 $B_i$模$A_i$的交换子是$(Z_i)_{A_i}$，集合与$Z_i$的元素同调；我们用$Z_i$来认同。此外，$A_i$的$B_i$子模是$A_i$的双面理想，并且由于环$A_i$很简单，所以唯一的双面理想是0和$A_i$。因此 $A_i$ 是一个简单的 $B_i$ 模块。此外，$A_1\otimes A_2$的$(B_1\otimes B_2$)子模是环$A_1\otimes A_2$的双面理想。

断言 a) 因此从 VIII, p. 214, 定理 2, b) 得出，应用到简单的 $B_1$-模块 $A_1$，带有交换子 $Z_1$，以及简单的 $B_2$-模块 $A_2$，带有交换子$Z_2$。

让我们证明断言 b)。 A 的最大双面理想的交是$(B_1\otimes B_2$)模$A_1\otimes A_2$的根式；由VIII、p. 215的推论2，这个交重合与$\mathfrak{R}(Z)A$。 代数 $Z_1$ 和 $Z_2$ 是可交换的且半单。因此，环 Z 的部首由幂零元 (VIII、p. 215、定理 3) 组成，环 A 的双面理想 $\mathfrak{R}(Z)A$ 包含在部首 $\mathfrak{R}(A)$ (VIII， p. 157、注 1)。然而，最大双面理想包含 $\mathfrak{R}(A)$ (VIII, p. 155, 命题 5, d)) 的交。这就证明了断言 b)。

可分离的交换代数和减少的交换代数的张量积是减少的环（V, §15, No. 2，p. 120，命题5）。 代数 $Z_1$ 和 $Z_2$ 是可交换的，并且半单是约简的。如果代数$Z_1$和$Z_2$之一是可分离的，则代数Z减少；因此，VIII、p. 215的定理 3 没有根式，我们有$\mathfrak{R}(A) =\mathfrak{R}(Z)A = 0$。特别是当域 K 是完美的时，因为完美域上的每个约化交换代数都是可分离的（V, §15, No. 5、p. 125、定理 3）。

#### 推论{#alg-viii-s12-n4-cor-1 .statement tag=00EG}

假设代数$A_1$和$A_2$是简单的，并且$A_1$的中心$Z_1$约化为K。那么环$A_1\otimes A_2$除了0和它本身之外没有其他双面理想。

到假设，我们有$Z_1= K$，并且由于$A_2$很简单，它的中心$Z_2$是域（VIII，p. 121，推论1，a））。因此，环 $Z = Z_1\otimes Z_2$ 为域，推论由命题 3, a) 得出。

### 5. 张量积 / 半单模

#### 命题 4 {#alg-viii-s12-prop-4 .statement tag=00EH}

对于$i\in  \{1,2\}$，令$A_i$为K-代数、$M_i$半单$A_i$模，以及$M_i$的交换子$Z_i$中心。 集合$A = A_1\otimes A_2$、$M = M_1\otimes M_2$、$Z = Z_1\otimes Z_2$。我们有$\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$。如果代数 $Z_1$ 和 $Z_2$ 之一在 K 上可分，特别是如果域 K 是完美的，则 A-模 M 没有根式。

对于$i\in  \{1,2\}$，让$S_i$是一个简单的$A_i$模块，$D_i$是它的交换子，$I(i)$集合。我们首先处理$M_i$是$A_i$模块$S_i^{(I(i))}$的情况。我们将其与$D_i$的中心交换到认同中心$Z_i$。 集合$D = D_1\otimes D_2$。我们有$\mathfrak{R}(D) =\mathfrak{R}(Z)D$（VIII，p. 217中的命题 3）和$\mathfrak{R}_A(S_1\otimes S_2) =$$\mathfrak{R}(D)(S_1\otimes S_2)$（VIII，p. 215，推论2），因此$\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(Z)(S_1\otimes S_2)$。 A-模 M 是A-模族的直和，与$S_1\otimes S_2$同构的，模族的直和部首是部首的直和（VIII，p. 152，推论2）。因此我们有$\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$。

现在考虑一般情况。对于$i\in  \{1,2\}$，用$\mathscr{S}_{M_i}$表示对$A_i$模块$M_i$的支持。对于$\lambda \in \mathscr{S}_{M_i}$，用$M_{i;\lambda}$表示型$\lambda$的$M_i$的同型成分，用$Z_{i;\lambda}$表示其交换子的中心。我们认同环 $Z_i$ 乘积环 $Z_{i;\lambda}$ $\lambda \in \mathscr{S}_{M_i}$。令$\lambda \in \mathscr{S}_{M_1}$和$\mu\in \mathscr{S}_{M_2}$。用$i_{\lambda}: Z_{1;\lambda}\rightarrow Z_1$唯一的K-线性映射表示，使得pr$_{\lambda}\circ i_{\lambda}$在$Z_{1;\lambda}$上是恒等映射，并且pr$_{\lambda'}\circ i_{\lambda}$对于$\lambda '\in \mathscr{S}_{M_1}-\{\lambda \}$来说是零映射。 定义$i_\mu: Z_{2;\mu}\rightarrow Z_2$同样。 集合$Z_{\lambda ,\mu}= Z_{1;\lambda}\otimes Z_{2;\mu}$和$i_{\lambda ,\mu}=i_{\lambda}\otimes i_\mu$，并用$\pi_{\lambda ,\mu}$表示从Z到$Z_{\lambda ,\mu}$的映射pr$_{\lambda}\otimes$pr$_\mu$。 映射 $\pi_{\lambda ,\mu}$ 是一个满射环同态；因此我们有 $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))\subset \mathfrak{R}(Z_{\lambda ,\mu})$ (VIII, p. 155, 命题 5, b))。我们来证明逆包含。设$z$为$\mathfrak{R}(Z_{\lambda ,\mu})$的元素；由于$Z_{1;\lambda}$和$Z_{2;\mu}$是域，$z$是幂幂的（定理 3 of VIII，p. 215）。我们在$Z_{\lambda ,\mu}$中有$i_{\lambda ,\mu}(xy) =i_{\lambda ,\mu}(x)\cdot i_{\lambda ,\mu}(y)$对应$x, y$；因而，$i_{\lambda ,\mu}(z)$是幂零的，因此属于到$\mathfrak{R}(Z)$。由于$\pi_{\lambda ,\mu}\circ i_{\lambda ,\mu}$在$Z_{\lambda ,\mu}$上是恒等映射，因此元素$z$属于到$\pi_{\lambda ,\mu}(\mathfrak{R}(Z))$。这样我们就证明了等式$\pi_{\lambda ,\mu}(\mathfrak{R}(Z)) =\mathfrak{R}(Z_{\lambda ,\mu})$。

集合$M_{\lambda ,\mu}= M_{1;\lambda}\otimes M_{2;\mu}$；这是 M 的子模在 Z 下稳定。对于 $z\in Z$ 和 $m\in M_{\lambda ,\mu}$，我们有 $zm=\pi_{\lambda ,\mu}(z)m$。因而，在同典型情况下，$\mathfrak{R}(Z)M_{\lambda ,\mu}$ 等于$\mathfrak{R}(Z_{\lambda ,\mu})M_{\lambda ,\mu}$，因此也等于 $\mathfrak{R}_A(M_{\lambda ,\mu})$。由于直和的部首是部首（VIII，p. 152，推论2）中的直和，并且M是$(\lambda , \mu)\in \mathscr{S}_{M_1}\times \mathscr{S}_{M_2}$的子模$M_{\lambda ,\mu}$中的直和，所以等式$\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$得证。 最后一个断言然后从 VIII、p. 217 中的命题 3 开始。

#### 引理 2 {#alg-viii-s12-lem-2 .statement tag=00EI}

令$A_1$和$A_2$是交换域K上的代数。令$M_1$是K上有限维的$A_1$模，$M_2$是有限长度的$A_2$模。那么$A_1\otimes A_2$-模块$M_1\otimes M_2$有有限长度。

集合$M = M_1\otimes M_2$。令 $(e_1, . . . , e_n)$ 为 $M_1$ 的基在域 K 上。映射 $(x_1, . . . , x_n)\mapsto \sum^n_{i=1}e_i\otimes x_i$ 是从 $A_2$ 模块 $M^n_2$ 到 $A_2$ 模块 M 的同构。因为 $M_2$ 是有限长度的$A_2$模，M也是。此外，M的每个A-子模都是$A_2$子模；因而，M 是 A-模或有限长度。

#### 命题 5 {#alg-viii-s12-prop-5 .statement tag=00RC}

令 $A_1$ 和 $A_2$ 为交换域 K 上的代数。令 $M_1$ 为半单 $A_1$ 模，该模是 K 上的有限维模，且为 $M_2$ 半单 $A_2$ 模。对于$i\in  \{1,2\}$，用$D_i$表示$A_i$模$M_i$的交换子，用$Z_i$表示$D_i$的中心。 集合$A = A_1\otimes A_2$，M = $M_1\otimes M_2,D = D_1\otimes D_2$，$Z = Z_1\otimes Z_2$。

a) A-模 M 的交换子可与 D 等价，其中心为 Z。若$A_2$模$M_2$ 有有限长度，则A-模 M 有有限长度，环 D 正确，左阿廷的，且环 Z 为阿廷的。

b) 以下属性是等效的：

(i) A-模 M 为半单。

(ii) 环 Z 与交换域族的乘积同构。

(iii) 环 Z 减小。

c) 以下属性是等效的：

(i) A-模 M 是同型的并且不会减少到 0。

(ii) 环 Z 为域。

(iii) 环 Z 为整环。

由假设，$M_1$是K上的有限维。因而，M的交换子可以用D（VIII，p. 213，引理1）来识别，并且它的中心是Z（III, §4, No. 4，p. 468，推论）。假设$A_2$-模块$M_2$有有限长度。 A-模 M 有有限长度 by 引理 2。由于 $M_2$ 是半单并且是有限生成的，环 $D_2$ 是半单 (VIII, p. 139, 命题 6)，其中心$Z_2$是交换域有限族中的乘积。因而，$D_2$-模块$(D_2)_s$和$Z_2$-模块$(Z_2)_s$各有有限长度。此外，由于$M_1$是K上的有限维，所以$D_1$和$Z_1$也是有限维的。到引理2，模$(D_1\otimes D_2)_s$有有限长度；因而，环$D_1\otimes D_2$是左阿廷的。我们同样证明环$D_1\otimes D_2$是右阿廷，环$Z_1\otimes Z_2$是阿廷的。 断言a)如下。

让我们证明b)。 半单模的交换子的中心与交换域族的乘积同构（VIII，p. 87，命题8，a））；这证明了 (i) 蕴涵 (ii)。含义 (ii) $\Rightarrow$ (iii) 是明确的。

假设环 Z 被减少。然后我们有 $\mathfrak{R}(Z) = 0$ (VIII, p. 215, 定理 3) 和 $\mathfrak{R}_A(M) = 0$ (VIII, p. 218, 命题 4)。由于$A_2$-模块$M_2$是半单，因此存在简单的$A_2$-模块系列$(S_i)_{i\in I}$和从$M_2$到$\bigoplus S_i$的同构。因而，A-模 M 与 $\bigoplus M_1\otimes S_i$ 同构的。因而，对于每个 $i\in I$，A-模 $M_1\otimes S_i$ 都没有根式。由a)可知，有有限长度；因此它是半单 (VIII, p. 153, 命题 3, b))。 A-模 M 是半单模家族的直和，因此是半单。这证明(iii)蕴涵(i)和b)的结论证明。

A-模是同型的，非零的当且仅当它是半单并且其交换子的中心是域（VIII，p. 87，命题8，b））。因而，c) 由 b) 推出。

#### 推论{#alg-viii-s12-n5-cor-1 .statement tag=00EJ}

如果$Z_1$或$Z_2$是域K上的可分代数（对于例，K是完美的情况），那么A-模$M_1\otimes M_2$是半单。

环 $Z_1$ 和 $Z_2$ 同构于域的乘积，因此被约化环。特别是，如果 K 是完美的，则它们在 K (V, §15, No. 5, p. 125, 定理 3) 上可分离代数。通过可分离的代数的V, §15, No. 2、p. 120、张量积中的命题 5以及减少的代数进行了减少。所以 Z 是环的约化，推论来自命题 5，b)。

### 6. 张量积 / 半单代数

#### 命题 6 {#alg-viii-s12-prop-6 .statement tag=00EK}

令$A_1$和$A_2$为非零的K-代数。如果环 $A_1\otimes A_2$ 是简单的（分别为半单），则环 $A_1$ 和 $A_2$ 都是简单的（分别为半单）。

环 B 是半单（分别是简单）当且仅当 B-模 $B_s$ 是半单（分别是同型和非零的）。因而，命题是从命题1（VIII，p. 211）得出的。

#### 命题 7 {#alg-viii-s12-prop-7 .statement tag=00EL}

设$A_1$和$A_2$为半单K-代数，分别为中心$Z_1$和$Z_2$。假设$A_1$比K有有限次数。那么环$A_1\otimes A_2$是左阿廷的，它的中心$Z_1\otimes Z_2$也是。 环$A_1\otimes A_2$是简单的（或半单）当且仅当环$Z_1\otimes Z_2$是域（或减少的环）。

这是VIII、p. 219的命题5的$M_1= (A_1)_s, M_2= (A_2)_s$的情况。

#### 推论 1 {#alg-viii-s12-prop-7-cor-1 .statement tag=00EM}

设$A_1$和$A_2$为半单K-代数；假设$A_1$是K上的有限维。假设$A_1$或$A_2$的中心是K上可分离的代数，对于例来说，这是K完美时的情况。那么$A_1\otimes A_2$就是半单。

这就是VIII、p. 221的推论$M_1= (A_1)_s, M_2= (A_2)_s$的情况。

#### 推论 2 {#alg-viii-s12-prop-7-cor-2 .statement tag=00RD}

令$A_1$和$A_2$为单K-代数；假设$A_1$是K上的有限维。如果$A_1$或$A_2$的中心等于K，则代数$A_1\otimes A_2$是简单的。尤其是当 K 是代数封闭时的情况。

$A_1$和$A_2$中的中心、$Z_1$和$Z_2$分别为域；如果环$Z_1$和$Z_2$之一等于K，则环$Z_1\otimes Z_2$为域。因此应用命题7就足够了。

如果域 K 是代数闭的，则 $A_1$ 的中心等于 K。

### 7. 半单模中的标量的扩张

#### 命题 8 {#alg-viii-s12-prop-8 .statement tag=00EN}

设 A 为 K-代数，M A-模，以及域 K 的 L 扩张。用 D 表示 M 的交换子，用 Z 表示 D 的中心。

a) 假设 $A_{(L)}$-模块 $M_{(L)}$ 很简单（分别为同型，半单）。那么 A-模 M 是简单的（分别是同型，半单）。

b) 假设 A-模 M 为半单，并且 M 或 L 是 K 上的有限维。当且仅当环 $Z_{(L)}$ 被约化时，$A_{(L)}$ 模 $M_{(L)}$ 才是半单。 $A_{(L)}$模$M_{(L)}$是同型的，并且非零的当且仅当环$Z_{(L)}$是整环。

c) 假设 A-模 M 是简单的。当且仅当环 $D_{(L)}$ 是半单（分别是简单、域）时，$A_{(L)}$-模$M_{(L)}$ 是半单（分别是同型、简单）。

断言 a) 是命题 1 (VIII, p. 211) 的特例，断言 b) 是命题 5 (VIII, p. 219) 的特例，断言 c) 是推论的特例1 个VIII、p. 215。

#### 推论 1 {#alg-viii-s12-prop-8-cor-1 .statement tag=00EO}

a) 假设 A-模 M 为半单，K 的扩张 L 是可分的，且 M 或 L 是 K 上的有限维。则 $A_{(L)}$ 模 $M_{(L)}$ 为半单。

b) 假设 A-模 M 是简单的，且其交换子等于 K。则 $A_{(L)}$ 模 $M_{(L)}$ 是简单的。

断言 a) 由推论VIII、p. 221得出。 断言 b) 是命题 8, c) 的特例。

#### 推论 2 {#alg-viii-s12-prop-8-cor-2 .statement tag=00RE}

令 L 为域 K 的扩张。用 Z 表示 K-代数 A 的中心。

a) 如果L-代数$A_{(L)}$是半单，则K-代数A是半单。

b) 假设 K-代数 A 为半单，并且 L 或 A 是 K 上的有限维。当且仅当环 $Z_{(L)}$ 被约化时，L 代数 $A_{(L)}$ 才为半单；尤其是当 L 是 K 的可分扩张时。L-代数 $A_{(L)}$ 是简单的当且仅当环 $Z_{(L)}$ 是整环；当 A 的中心等于 K 时尤其如此。

断言 a) 和 b) 源自命题 8，a) 和 b) 应用于 A-模 $A_s$。

#### 命题 9 {#alg-viii-s12-prop-9 .statement tag=00EP}

设 A 为 K 的 K-代数和 L 可分扩张。

a) 如果 M 是A-模，没有部首，则$A_{(L)}$模$M_{(L)}$没有部首。

b) 如果K-代数 A 没有根式，则L-代数$A_{(L)}$ 没有根式。

让我们证明断言a)。设 M 为A-模，不带根式。我们认同 M 及其典范像在$M_{(L)}$。令 N 为 M 的极大子模。由于 A-模 $M/N$ 很简单，因此从 VIII、p. 218 的命题 4 得出，$A_{(L)}$ 模 $(M/N)_{(L)}= M_{(L)}/N_{(L)}$ 没有部首，因此由推论 1 得出 $\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset N_{(L)}$， c) VIII、p. 152。现在，从II, §7, No. 7、p. 306的命题 14的推论得出，$N_{(L)}$的交，其中N穿过M的极大子模的集合，被减少到0。因而，$A_{(L)}$模$M_{(L)}$ 没有部首。

断言 b) 源自断言 a) 应用于 A-模 $A_s$。

#### 命题 10 {#alg-viii-s12-prop-10 .statement tag=00EQ}

设 A 为 K 的 K-代数和 L 扩张。设 M 为 A-模。

a) 我们制作以下两个假设之一：

(i) A-模 M 是有限生成的，L 是 K 上的代数。

(ii) 环 A 为左阿廷的。

然后我们就有了包含

$$
\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})
$$

b) 如果 K 的 L 是可分扩张，那么我们有包含

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

让我们证明断言 a)。考虑情况(i)。首先假设L比K有有限次数。那么A-模$M_{(L)}$是有限生成的。用$f$表示从A到$A_{(L)}$的典范同态； 环 $A_{(L)}$ 由其中心和$f(A)$ 的并生成。因而，我们可以将VIII、p. 174中的应用命题 3 转换为$A_{(L)}$模块$M_{(L)}$。这给出了包含 $\mathfrak{R}_A(M_{(L)})\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ 和更不必说 $\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$（VIII，p. 152，推论 1）。

现在让我们来处理一般情况。设$x_1, . . . , x_n$为$\mathfrak{R}_A(M)$的生成A-模M和$x$元素的元素。设$a_1, . . . , a_n$为$A_{(L)}$的元素；由于L是K上的代数，因此L中存在包含K的有限扩张$L'$，使得$a_i$属于到$A_{(L')}$。由上式，$x$属于到$A_{(L')}$模$M_{(L')}$的部首；根据VIII、p. 153的推论，元素$x_i+a_ix$对于$1\leqslant i\leqslant n$生成，$A_{(L')}$-模块$M_{(L')}$，因而$A_{(L)}$-模块$M_{(L)}$。根据同样的推论，$x$ 属于对应于 $A_{(L)}$ 模 $M_{(L)}$ 的部首。

现在让我们考虑情况(ii)。设$\mathfrak{r}$为A的根式，则A-模M的根式等于$\mathfrak{r}M$（VIII，p. 174，推论）。 A 的根式 $\mathfrak{r}$ 是 A 的幂幂双面理想 (VIII, p. 173, 命题 1)；因而，$\mathfrak{r}_{(L)}$是$A_{(L)}$的幂幂双面理想。由此可见，$\mathfrak{r}_{(L)}\subset \mathfrak{R}(A_{(L)})$（VIII、p. 156、定理 1）和VIII、p. 158的命题 6 意味着$\mathfrak{R}(A_{(L)})M_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$。因而，我们有 $\mathfrak{R}_A(M) =\mathfrak{r}M\subset$ $\mathfrak{R}_{A_{(L)}}(M_{(L)})$，其中结论证明或断言 a)。

模 $M/\mathfrak{R}_A(M)$ 没有部首。如果L是K的可分扩张，则从VIII、p. 223的命题9得出$A_{(L)}$模$(M/\mathfrak{R}_A(M))_{(L)}$没有根式。因而，我们有包含

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

#### 推论{#alg-viii-s12-n7-cor-1 .statement tag=00ER}

令 L 为 K 的可分扩张。如果 L 是 K 上的代数，或者如果环 A 是左阿廷的，则我们有 $\mathfrak{R}(A_{(L)}) =$ $\mathfrak{R}(A)_{(L)}$。

这是$M = A_s$ 命题 10 的情况。

### 习题{#alg-viii-s12-exercises}

参见[习题为 § 12](exercises/s12/)。
