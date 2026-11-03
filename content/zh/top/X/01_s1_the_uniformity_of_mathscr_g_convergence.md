---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 1
section_title: The uniformity of $\mathscr{G}$-convergence
lang: zh
source: top-v-x
pdf_pages: 0280-0289, 0324-0327
extraction: ocr
subsections:
    - "no": 1
      title: THE UNIFORMITY OF UNIFORM CONVERGENCE
      page: 0
      pdf_page: 280
    - "no": 2
      title: $\mathfrak{S}$-convergence
      page: 0
      pdf_page: 281
    - "no": 3
      title: EXAMPLES OF $\mathscr{E}$-CONVERGENCE
      page: 0
      pdf_page: 283
    - "no": 4
      title: PROPERTIES OF THE SPACES $\mathscr{F}_\mathscr{S}(X; Y)$
      page: 0
      pdf_page: 284
    - "no": 5
      title: COMPLETE SUBSETS OF $\mathscr{F}_\mathscr{S}(X; Y)$
      page: 0
      pdf_page: 285
    - "no": 6
      title: $\mathscr{E}$-CONVERGENCE IN SPACES OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 286
statements: 33
exercises: 12
content_sha256: 0458f3b20e66448cc93f0fa4443116454a62b2ee819df0de499b70ed4e062804
translated_from: content/en/top/X/01_s1_the_uniformity_of_mathscr_g_convergence.md
translation_method: google
source_content_sha256: 745807f99ebf8ccad98600e79411f1137bc903046fec07540ab638fc2319dece
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: c9d06d7461dc5dc4259a8f5833f7c9db76b1d982a6a56ba9e06e0781d24d874c
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. $\mathscr{G}$收敛的均匀性

记号。如果$X$和$Y$是任意两个集合，我们记得$X$到$Y$的所有映射中的集合用$\mathscr{F}(X; Y)$表示，并且可以用乘积集合$Y^X$来标识（集合理论、章II, § 5, no. 2）。对于$\mathscr{F}(X; Y)$的每个子集$H$和每个$x \in X$，我们将用元素$u(x) \in Y$的$H(x)$集合表示，因为$u$穿过$H$。如果$\Phi$是$\mathscr{F}(X; Y)$上的过滤器基，我们用$\Phi(x)$表示由集合$H(x)$形成的$Y$上的过滤器基，因为$H$穿过$\Phi$。最后，我们记得，对于$X$的每个$u \in \mathscr{F}(X; Y)$和每个子集$A$，$u|A$表示$u$到$A$的限制，即$A$的映射到$Y$；如果$H$是$\mathscr{F}(X; Y)$的子集，则$H|A$将表示函数$u \in H$的限制$u|A$的集合。

### 1. 均匀收敛的均匀性

令$X$为集合，令$Y$为均匀空间。 对于$Y$的每个随行$V$，让$W(V)$表示$X$到$Y$的映射的所有对$(u, v)$的集合，使得$(u(x), v(x)) \in V$对于所有$x \in X$。 由于$V$贯穿$Y$周边的集合，集合$W(V)$形式是$\mathscr{F}(X; Y)$上均匀性的基本系统周边。 因为他们显然满足公理$(U'_1)$（章II, § 1, no. 1）；如果$V, V'$是$Y$的两个随从，使得$V \subset V'$，我们有$W(V) \subset W(V')$，因此集合$W(V)$满足

$(B_1)$（章I, § 6, no. 3）；我们有$\widehat{W(V)} = W(\overline{V})$，所以满足$(U''_{II})$；最后，关系“$(u(x), v(x)) \in V$对于所有$x \in X$”和“$(v(x), w(x)) \in V$对于所有$x \in X$”意味着关系“$(u(x), w(x)) \in \overline{V}^2$对于所有$x \in X$”；在其他字中，我们有$\widehat{W(V)} \subset W(\overline{V}^2)$，这证明了$(U'''_{III})$。

#### 定义 1 {#top-x-s1-def-1 .statement tag=0CAR}

*uniformity on 集合 $\mathscr{F}(X; Y)$ which has as a fundamental 系统 of entourages 集合 of 子集 $W(V)$, where $V$ runs through 集合 of entourages of $Y$, is called the uniformity of uniform convergence. 拓扑它诱导称为一致收敛的拓扑。如果$\mathscr{F}(X; Y)$上的滤波器$\Phi$相对于此拓扑收敛到元素$u_0$，则称$\Phi$均匀收敛到$u_0$。*

请注意，$\mathscr{F}(X; Y)$ 上一致收敛的*拓扑* 取决于$Y$ 的一致结构，而不仅仅取决于$Y$ (习题 4) 的拓扑。

赋予$\mathscr{F}(X; Y)$一致收敛的一致性而得到的一致空间记为$\mathscr{F}_u(X; Y)$。

### 2. $\mathfrak{S}$-收敛

#### 定义 2 {#top-x-s1-def-2 .statement tag=0CAS}

*设$X$是一个集合，$Y$是一个均匀空间，$\mathfrak{S}$是$X$的子集的集合。 $\mathfrak{S}$的集合均匀收敛的均匀性，或者简称为$\mathfrak{S}$收敛的均匀性，是$\mathscr{F}(X; Y)$上的最粗均匀性，它使得$\mathscr{F}(X, Y)$的均匀连续限制映射$u \to u|A$变成均匀的空间 $\mathscr{F}_u(A; Y)$，其中$A$穿过$\mathfrak{S}$。 赋予$\mathscr{F}(X; Y)$均匀性$\mathfrak{S}$收敛性，得到均匀空间记为$\mathscr{F}_{\mathfrak{S}}(X; Y)$。*

由$\mathfrak{S}$收敛的均匀性引起的拓扑称为$\mathfrak{S}$收敛*的*拓扑；它是最粗糙的，其中 $\mathscr{F}(X; Y)$ 到 $\mathscr{F}_u(A; Y)$ ($A \in \mathfrak{S}$) 的所有映射 $u \to u|A$ 都是连续的 (章 II, § 2, no. 3、命题 4、推论)。

$\mathscr{F}(X; Y)$上的滤波器$\Phi$相对于$\mathfrak{S}$的拓扑收敛到$u_0$，当且仅当$u|A$对于所有$A \in \mathfrak{S}$（章）相对于$\Phi$一致收敛到$u_0|A$ I, § 7, no. 6、命题 10)，因此$\Phi$*一致收敛到$u_0$于$\mathfrak{S}$的集合*。

$\mathscr{F}_{\mathfrak{S}}(X; Y)$上的滤波器基$\Phi$是柯西滤波器基当且仅当对于映射$u \to u|A$下$\Phi$的每个$A \in \mathfrak{S}$、像是$\mathscr{F}_u(A; Y)$上的柯西滤波器基 （章II, § 3, no. 1、命题4）。

令 $f$ 为拓扑（或均匀）空间 $Z$ 到 $\mathscr{F}_{\mathfrak{S}}(X; Y)$ 的映射。那么 $f$ 是连续的（或一致连续的）当且仅当，对于 $Z$ 到 $\mathscr{F}_u(A; Y)$ 的每个 $A \in \mathfrak{S}$、映射 $z \to f(z)|A$ 是连续的（或一致连续的）（章 I, § 2, no. 3、命题 4； 章II, § 2, no. 3、命题4)。

最后，令$M$为$\mathscr{F}_{\mathfrak{S}}(X; Y)$的子集；那么$M$是预紧的，当且仅当对于每个$A \in \mathfrak{S}$，$u \in M$的限制集$u|A$是$\mathscr{F}_u(A; Y)$的预紧子集（II, § 4, no. 2章，命题3）。

#### 注 1 {#top-x-s1-n2-rem-1 .statement tag=0CAT}

初始均匀性（章 II, § 2, no. 3，命题 4）的一般定义表明，$\mathscr{F}_\mathscr{S}(X; Y)$ 的基本系统可以如下获得： 对于基本的每个 $A \in \mathscr{S}$ 和每个$V$随行人员 $Y$ $\mathscr{B}$ 系统，令 $W(A, V)$ 为 $X$ 映射 $(u, v)$ 所有对到$Y$ 的集合，使得每个$(u(x), v(x)) \in V$ $x \in A$；由于$A$贯穿$\mathscr{S}$且$V$贯穿$\mathscr{B}$，集合* $W(A, V)$形式的*有限交是$\mathscr{F}_\mathscr{S}(X; Y)$随行人员的基本系统。

这个描述立即表明，如果$\mathscr{S}, \mathscr{S}'$是$X$的子集的两个集合，使得$\mathscr{S} \subset \mathscr{S}'$，那么$\mathscr{S}'$收敛的均匀性比$\mathscr{S}$收敛的均匀性*更细*。

#### 注 2 {#top-x-s1-n2-rem-2 .statement tag=0CAU}

然而，$\mathscr{S}$收敛的均匀性不会因$X$*的所有子集*的替换$\mathscr{S}$、集合$\mathscr{S}'$而改变，这些子集包含在*$\mathscr{S}$的集合的有限并中。 因此，在研究$\mathscr{S}$收敛性时，我们可能总是将自己限制在集合$\mathscr{S}$满足以下两个条件的情况：

(F'$_1$) **$\mathscr{S}$*属于到*$\mathscr{S}$的集合每子集。

(F'$_2$) **$\mathscr{S}$*属于到*$\mathscr{S}$的集合的每个有限并。

如果满足(F'$_2$)，则通过取所有集合$W(A, V)$，我们获得$\mathscr{F}_\mathscr{S}(X; Y)$的基本随从系统，其中$A$穿过$\mathscr{S}$，$V$穿过$Y$的基本随从系统。

#### 注 3 {#top-x-s1-n2-rem-3 .statement tag=0CAV}

$\mathscr{S}$收敛的均匀度是逆像，在$\mathscr{F}(X; Y)$的映射$u \to (u|A)_{A \in \mathscr{S}}$下进入$\prod_{A \in \mathscr{S}} \mathscr{F}_u(A; Y)$，这个乘积空间的均匀度（章II, § 2, no. 6，命题） 8).如果$\mathscr{S}$是$X$的*覆盖*，则此映射是*内射*，因此$\mathscr{F}_\mathscr{S}(X; Y)$同构于$\prod_{A \in \mathscr{S}} \mathscr{F}_u(A; Y)$的一致子空间，即映射的像。

#### 命题 1 {#top-x-s1-prop-1 .statement tag=0CAW}

*如果* $Y$ *是Hausdorff，并且* $\mathscr{S}$ *是* $X$的覆盖，*则空间* $\mathscr{F}_\mathscr{S}(X; Y)$ *是Hausdorff*。

令$u, v$为$\mathscr{F}_\mathscr{S}(X; Y)$的两个元素，使得$(u, v) \in W(A, V)$对应于$Y$的每个随行人员$V$以及每个$A \in \mathscr{S}$。由于$Y$是Hausdorff，因此在每个集合$A \in \mathscr{S}$上都有$u$和$v$重合，并且由于$\mathscr{S}$涵盖$X$，我们必须有$u = v$。

#### 注 4 {#top-x-s1-n2-rem-4 .statement tag=0CAX}

设$H$为$\mathscr{F}(X; Y)$的子集。通过滥用语言，由$\mathscr{S}$在$\mathscr{F}(X; Y)$上收敛的均匀性（分别拓扑）在$H$上引起的均匀性（分别拓扑）被称为$\mathscr{S}$在集合上收敛的均匀性（分别拓扑） $H$。

#### 注 5 {#top-x-s1-n2-rem-5 .statement tag=0CAY}

令$L$经过滤器$\mathfrak{S}$过滤为集合，并令$\lambda \to u_\lambda$为$L$的映射进入$\mathscr{F}_\mathscr{S}(X; Y)$，相对于$\mathfrak{S}$有极限$v$；那么我们说，*相对于过滤器* $\mathfrak{S}$，*映射* $u_\lambda$ *of* $X$ *进入* $Y$ *均匀收敛到* $v$ *[或者族* $(u_\lambda)$ *均匀收敛到* $v$] *在每个集合*$\mathscr{S}$。 *如果*$L = \mathbf{N}$*和*$\mathfrak{S}$*是Fréchet滤波器*，我们在这个叙述*中省略$\mathfrak{S}$*的提及。

更具体地，假设在$Y$上定义了合成（加法写）的交换律和结合律律。如果$(u_n)$是$X$的映射到$Y$的任何序列，则令$v_n$为映射，定义如下

$$
v_n(x) = \sum_{k=0}^n u_k(x) \quad (n \in \mathbf{N});
$$

我们说*级数，其一般项是* $u_n$ *在* $\mathscr{G}$的每个集合一致收敛 *如果序列* $(v_n)$ *在* $\mathscr{G}$的每个集合一致收敛。同样，我们通过考虑映射 $x \to \sum_{\lambda \in J} n_\lambda(x)$ 对于 $L$ 的所有有限子集 $J$，将定义 $X$ 映射的$(u_\lambda)_{\lambda \in L}$ 转化为 $Y$，并且$\mathscr{F}_\mathscr{G}(X; Y)$中的映射中的极限相对于$L$的有限子集有向集合(章III, § 5, no. 1)。

#### 注 6 {#top-x-s1-n2-rem-6 .statement tag=0CAZ}

紧接着从定义 1 和 2 可以得出，对于$x \in \bigcup_{A \in \mathscr{G}} A$，$\mathscr{F}_\mathscr{G}(X; Y)$ 到$Y$ 的映射 $u \to u(x)$ 是*均匀连续*。因此，特别是，如果$\overline{H}$表示子集$H$对$\mathscr{F}_\mathscr{G}(X; Y)$的闭包，则对于所有$x \in \bigcup_{A \in \mathscr{G}} A$我们有$\overline{H}(x) \subset \overline{H(x)}$（章I, § 2, no. 1，定理1）。

### 3. 例 OF $\mathscr{E}$-收敛

I。 *在*$X$的子集均匀收敛。令$A$为$X$的子集并取$\mathscr{G} = \{ A \}$。 $\mathscr{G}$收敛的均匀性（分别为拓扑）则称为*$A$中一致收敛的*均匀性*（分别为*拓扑*）；如果$\mathscr{F}_\mathscr{G}(X; Y)$上的过滤器$\Phi$收敛到$u_0$，则据说在*$A$*均匀地收敛到$u_0$。当$A = X$时，我们恢复了no. 1中定义的一致收敛性结构。

II。 *在*$X$的子集中逐点收敛。令$A$为$X$中的子集，并取$\mathscr{G}$为$X$中所有子集中的集合，其中子集由单个点属于到$A$组成（通过注 2 of no. 2 如果我们将 $\mathscr{G}$ 视为集合中的有限子集 $A$，则结果是一样的）。 $\mathscr{G}$收敛的均匀性（分别为拓扑）被称为*$A$中逐点收敛的*均匀性*（分别为*拓扑*）；如果$\mathscr{F}_\mathscr{G}(X; Y)$上的过滤器$\Phi$收敛到$u_0$，则据说在*$A$*逐点收敛到$u_0$。当且仅当对于每个 $x \in A$，$u_0(x)$ 相对于过滤器 $\Phi$ 是 $u(x)$ 的极限时，才会出现这种情况。

特别是，当$A = X$时，$X$中逐点收敛的均匀性（相应于拓扑）简称为逐点收敛*的*均匀性*（相应于*拓扑*）；将这个结构赋予$\mathscr{F}(X; Y)$得到的均匀空间用$\mathscr{F}_s(X; Y)$表示。请注意，逐点收敛的拓扑只是 $Y^X$ 上的 *乘积* 拓扑，因此仅取决于 $Y$ 的拓扑，而不取决于其统一的结构。

III。紧凑收敛。假设$X$是拓扑空间，并取$\mathscr{S}$为$X$的所有紧致子集中的集合。 $\mathscr{S}$收敛的均匀性（拓扑）则称为紧收敛的均匀性（拓扑），而通过赋予$\mathscr{F}(X; Y)$这种均匀性而获得的均匀空间表示为$\mathscr{F}_c(X; Y)$。紧致收敛的结构比一致收敛更粗，如果$X$是紧致的，则两个重合；逐点收敛性也比更细大于结构，如果$X$是离散的，这两个重合。

如果$X$是一致的空间，我们可以通过将$\mathscr{S}$取为$X$的所有预紧式子集的集合来在$\mathscr{F}(X; Y)$预紧式收敛的一致性上得到定义。同样，如果$X$是一个度量空间，我们可以将$\mathscr{S}$视为$X$的所有有界子集中的集合； $\mathscr{S}$-收敛的一致性称为有界收敛的一致性。

### 4. 空间 $\mathscr{F}_\mathscr{S}(X; Y)$ 的特性

#### 命题 2 {#top-x-s1-prop-2 .statement tag=0CB0}

令$X_1, X_2$为两个集合，令$Y$为统一的空间，令$\mathscr{S}_i$为$X_i$($i = 1, 2$)的子集集合和$\mathscr{S}_1 \times \mathscr{S}_2$集合子集 / $X_1 \times X_2$ / 形式 $A_1 \times A_2$，其中$A_i \in \mathscr{S}_i, i = 1, 2$。然后是规范的双射
$$
\mathscr{F}(X_1 \times X_2; Y) \to \mathscr{F}(X_1; \mathscr{F}(X_2; Y))
$$
（集合理论，R，§ 4, no. 14）是制服空间的同构
$$
\mathscr{F}_{\mathscr{S}_1 \times \mathscr{S}_2}(X_1 \times X_2; Y)
$$
到$\mathscr{F}_{\mathscr{S}_1}(X_1; \mathscr{F}_{\mathscr{S}_2}(X_2; Y))$。

令$V$为$Y$的随从，令$A_i \in \mathscr{S}_i (i = 1, 2)$；那么从定义紧接着，$W(A_1 \times A_2, V)$ 通过规范的双射与 $W(A_1, W(A_2, V))$ 进行识别，结果是直接的。

#### 命题 3 {#top-x-s1-prop-3 .statement tag=0CB1}

a) 设$X$为集合；令$\mathscr{S}$为$X$子集集合；设$Y, Y'$为两个统一的空间；令 $f : Y \to Y'$ 为均匀连续的映射。那么$\mathscr{F}_\mathscr{S}(X; Y)$到$\mathscr{F}_\mathscr{S}(X; Y')$的映射$u \to f \circ u$是均匀连续的。

b) 设$X, X'$为二集合；令$\mathscr{S}$（或$\mathscr{S}'$）为$X$（或$X'$）的子集集合；设$Y$为统一的空间；并令$g : X' \to X$为映射，使得对于每个$A' \in \mathscr{S}'$，$g(A')$包含在$\mathscr{S}$的集合的有限并中。那么$\mathscr{F}_\mathscr{S}(X, Y)$到$\mathscr{F}_{\mathscr{S}'}(X'; Y)$的映射$u \to u \circ g$是均匀连续的。

#### 命题 4 {#top-x-s1-prop-4 .statement tag=0CB2}

令$X, Y$为两个集合，令$(X_\lambda)_{\lambda \in L}$为集合的家族，并令$(Y_\mu)_{\mu \in M}$为制服空间的家族。对于每个$\lambda \in L$，令$\mathscr{S}_\lambda$为$X_\lambda$的子集集合，令$g_\lambda$为$X_\lambda$的映射到$X$，并令$\mathscr{S}$为集合 $X$ 中的子集，即集合 $g_\lambda(\mathscr{S}_\lambda)$ 中的并。对于每个$\mu \in M$，令$f_\mu$是$Y$到$Y_\mu$的映射，并赋予$Y$最粗糙的均匀性，使得$f_\mu$均匀连续。那么$\mathscr{S}$-收敛于$\mathscr{F}(X; Y)$的均匀度就是使$\mathscr{F}(X; Y)$的映射$u \to f_\mu \circ u \circ g_\lambda$均匀连续到$\mathscr{F}_{\mathscr{S}_\lambda}(X_\lambda, Y_\mu)$的最粗均匀度。

这些命题是描述的直接的推论，是no. 2、注1中给出的$\mathscr{S}$收敛的均匀性的基本系统； 证明的细节留给读者去了解。 命题 4 特别意味着：

#### 推论{#top-x-s1-n4-cor-1 .statement tag=0CB3}

令$X$为集合，令$(Y_i)_{i \in I}$为制服空间家族，令$\mathscr{S}$为$X$子集集合。如果我们赋予 $\prod_{i \in I} Y_i$ 乘积均匀性，则将均匀空间 $\mathscr{F}_\mathscr{S}(X, \prod_{i \in I} Y_i)$ 的规范双射转移到乘积均匀空间 $\prod_{i \in I} \mathscr{F}_\mathscr{S}(X; Y_i)$ (集合理论, R, § 4, no. 13）是同构。

### 5. 完成子集 / $\mathscr{F}_\mathscr{S}(X; Y)$

#### 命题 5 {#top-x-s1-prop-5 .statement tag=0CB4}

令$\Phi$为集合，$Y$统一为空间，以及$X$的子集为$\mathscr{S}$集合。然后，$\mathscr{F}_\mathscr{S}(X; Y)$上的滤波器$\Phi$收敛到$u_0$当且仅当$\Phi$关于$\mathscr{S}$收敛的均匀性是柯西滤波器，并且逐点收敛到$B = \bigcup_{A \in \mathscr{S}} A$中的$u_0$。

由于$B$中的逐点收敛的结构比$\mathscr{S}$收敛更粗糙，因此足以表明对于每个$A \in \mathscr{S}$和$Y$的每个封闭周边$V$，$W(A, V)$在$B$中相对于点式收敛的拓扑是封闭的（章II, § 3, no. 3、命题7）。现在$W(A, V)$随着$x$贯穿$A$而在映射$(u, v) \to (u(x), v(x))$下为$V$逆像交；这些映射相对于逐点收敛的拓扑是连续的（no. 2，注6），结果如下。

#### 推论 1 {#top-x-s1-prop-5-cor-1 .statement tag=0CB5}

$\mathscr{F}_\mathscr{S}(X; Y)$的子空间$H$是完备的，当且仅当对于$H$上的每个柯西滤波器$\Phi$，存在$u_0 \in H$使得$\Phi$逐点收敛到$B = \bigcup_{A \in \mathscr{S}} A$中的$u_0$。

这紧接着命题 5。

#### 推论 2 {#top-x-s1-prop-5-cor-2 .statement tag=0CB6}

令$\mathscr{S}_1, \mathscr{S}_2$为$X$的子集的两个集合，其并相同且满足$\mathscr{S}_1 \subset \mathscr{S}_2$，并令$H$为$\mathscr{F}(X; Y)$的子集。那么如果$H$对于$\mathscr{S}_1$收敛是完备的，那么它对于$\mathscr{S}_2$收敛也是完备的。

对于每个关于$\mathscr{G}_2$收敛的柯西滤波器也是关于$\mathscr{G}_1$收敛的柯西滤波器，并且我们可以应用推论1。

#### 推论 3 {#top-x-s1-prop-5-cor-3 .statement tag=0CB7}

*令 $H$ 为 $\mathscr{F}(X; Y)$ 的子集，这样，对于每个*
$$
x \notin B = \bigcup_{A \in \mathscr{G}} A,
$$
*$Y$中$H(x)$的闭包是$Y$的完整子空间。那么$\mathscr{F}_{\mathscr{G}}(X; Y)$中$H$的闭包$\overline{H}$就是一个完整的子空间。*

令$\Phi$为$\overline{H}$和定义映射$v : X \to Y$的柯西滤波器，如下所示。如果$x \in B$，$\Phi(x)$是$\overline{H(x)}$（no. 2，注6）上的柯西滤波器，因此到假设它至少有一个极限点；取 $v(x)$ 为其中极限之一。如果$x \notin B$，则取$v(x)$为$Y$中的任意点。通过$v$的定义，很明显$\Phi$在$B$中逐点收敛到$v$，因此$v$是$\mathscr{F}_{\mathscr{G}}(X; Y)$中$\Phi$的极限乘命题5。

特别地，如果$Y$完整，则对于每个$H \subset \mathscr{F}(X; Y)$满足命题5中的推论3中的假设；因此：

#### 定理 1 {#top-x-s1-thm-1 .statement tag=0CB8}

*令$X$为集合，令$\mathscr{G}$为$X$的子集集合，令$Y$为完整的制服空间。这样制服空间$\mathscr{F}_{\mathscr{G}}(X; Y)$就完成了*

### 6. $\mathscr{E}$-连续映射的空间收敛

令$X, Y$为两个拓扑空间，并令$\mathscr{C}(X; Y)$表示$X$的所有*连续映射到$Y$*的集合。如果$\mathscr{G}$是$X$的子集的集合，并且如果$Y$是一致的空间，我们用$\mathscr{C}_{\mathscr{G}}(X; Y)$集合$\mathscr{C}(X; Y)$表示赋予$\mathscr{G}$收敛的一致性。其中$\mathscr{C}_s(X; Y), \mathscr{C}_c(X; Y)$和$\mathscr{C}_u(X; Y)$分别表示集合和$\mathscr{C}(X; Y)$，分别具有逐点收敛、紧致收敛和一致收敛的一致性。

#### 命题 6 {#top-x-s1-prop-6 .statement tag=0CB9}

*令$X$为拓扑空间，$Y$为均匀的空间，以及$X$的子集的$\mathscr{G}$集合。对于$A \in \mathscr{G}$和$Y$的每个封闭随行人员$V$，$W(A, V)$和$W(\overline{A}, V)$在$\mathscr{C}(X; Y) \times \mathscr{C}(X; Y)$上的痕迹是相同的。*

因为如果$u, v$是连续的$X$到$Y$的映射，$X$到$Y \times Y$的映射$x \mapsto (u(x), v(x))$是连续的，因此对于所有$x \in A$来说$(u(x), v(x)) \in V$意味着假设对于所有 $x \in \overline{A}$（章 I, § 2, no. 1，定理 1），$(u(x), v(x)) \in \overline{V} = V$。

如果$\bar{\mathscr{G}}$表示$\mathscr{G}$的集合$X$的闭包集合，命题6表明，$\mathscr{G}$的*在*$\mathscr{C}(X; Y)$、结构收敛，并且$\bar{\mathscr{G}}$-收敛性相同。

**连续映射空间的 G 收敛**

#### 推论 {#top-x-s1-n6-cor-1 .statement tag=0CBA}

*设 B 为 X 的稠密子集。在$C(X; Y)$上，一致收敛的结构与B中一致收敛的结构相同。*

#### 命题 7 {#top-x-s1-prop-7 .statement tag=0CBB}

*令X为拓扑空间，令$\mathfrak{S}$为X的子集的集合，并令Y为均匀空间。如果 Y 是 Hausdorff，并且如果 $\mathfrak{S}$ 的集合的并 B 在 X 中稠密，则 $C_{\mathfrak{S}}(X; Y)$ 是 Hausdorff。*

因为如果$(u, v)$属于对所有集合$W(A, V)$，其中$A \in \mathfrak{S}$和V是Y的随从，假设Y是Hausdorff告诉我们$u(x) = v(x)$对所有$x \in B$；如果$u$和$v$连续，则$u = v$乘以扩张的原理恒等式（章I, § 8, no. 1，命题2，推论1）。

特别是，在 $C(X; Y)$ 上，X 的“密集”子集中的逐点收敛的拓扑是 Hausdorff。

#### 命题 8 {#top-x-s1-prop-8 .statement tag=0CBC}

*令X为集合，$\mathfrak{T}$为X的过滤器，并令Y为统一的空间。然后映射$u : X \to Y$的集合H使得$u(\mathfrak{T})$是Y上的柯西滤波器基在$F_u(X; Y)$中闭合。*

令$u_0 : X \to Y$位于$F_u(X; Y)$中H的闭包中。 对于 Y 的每个对称周边V，存在映射$u \in H$，使得$(u_0(x), u(x)) \in V$对于所有$x \in X$；另一方面，到假设时，存在集合 $M \in \mathfrak{T}$，使得只要 $x$ 和 $x'$ 在 M 中，就有 $(u(x), u(x')) \in V$。 由于$(u_0(x), u(x)) \in V$和$(u_0(x'), u(x')) \in V$，只要$x$和$x'$在M中，就可以得出$(u_0(x), u_0(x')) \in V$，因此$u_0(\mathfrak{T})$是Y上的柯西滤波器基。

#### 推论 1 {#top-x-s1-prop-8-cor-1 .statement tag=0CBD}

*设X为拓扑空间，Y为均匀空间。 X的映射到Y的集合在点连续$x_0 \in X$在$F_u(X; U)$封闭。*

如果V是X中$x_0$的邻域过滤器，则$u(x_0)$是$u(V)$的集群点；因此，当且仅当$u(V)$是Y上的柯西滤波器基（章II, § 3, no. 2，命题5，推论2）时，$u$在$x_0$连续。

#### 推论 2 {#top-x-s1-prop-8-cor-2 .statement tag=0CBE}

*设X、L分别为经过过滤器$\mathfrak{T}, \mathfrak{G}$过滤后的两个集合，并令Y为完整的均匀空间。对于每个$\lambda \in L$，令$u_\lambda$为Y中X的映射。假设(i)族$(u_\lambda)_{\lambda \in L}$在X（相对于滤波器$\mathfrak{G}$）均匀收敛到映射$v : X \to Y$； (ii) 对于每个 $\lambda \in L$，$u_\lambda$ 相对于过滤器 $\mathfrak{T}$ 具有极限 $y_\lambda$。在这些条件下，v相对于$\mathfrak{T}$有极限，并且v相对于$\mathfrak{T}$的每个极限是家族$(y_\lambda)_{\lambda \in L}$相对于$\mathfrak{G}$的极限。*

因为 v 位于 $F_u(X; Y)$ 中 $u_\lambda$ 的集合的闭包中，因此凭借命题 8，$v(\mathfrak{T})$ 是 Y 上的柯西滤波器基；这表明 v 对于 $\mathfrak{T}$ 有极限 y，因为 Y 是完整的。让

X' = X \cup \{ \omega \} 是与滤波器$\mathscr{F}$（第I, § 6, no. 5章）关联的拓扑空间，并将$u_\lambda$（或$v$）扩展到$X'$的映射$\bar{u}_\lambda$（或$\bar{v}$）到$Y$ 通过放置$\bar{u}_\lambda(\omega) = y_\lambda$ [分别。 $\bar{v}(\omega) = y$]。 则映射$\bar{u}_\lambda, \bar{v}$在$X'$上连续，$\bar{u}_\lambda$相对于$\mathscr{G}$在$X$均匀收敛到$\bar{v}$；由于$X$在$X'$是稠密的，推论到命题6表明$\bar{u}_\lambda$在$X'$到$\bar{v}$均匀收敛，特别是$y = \lim_{\mathscr{G}} y_\lambda$。

#### 定理 2 {#top-x-s1-thm-2 .statement tag=0CBF}

*令$X$为拓扑空间，$Y$为均匀空间。那么$X$的连续映射到$Y$的集合$C(X; Y)$就是空间$F(X; Y)$的闭子集，且拓扑具有一致收敛性。*

对于每个$x \in X$，$X$的映射到$Y$的集合在$x$连续，在$F_u(X; Y)$中闭（命题8，推论1）；因此，这些集合中的交 $C(X; Y)$ 也被关闭。

这个结果可以用形式来表示，即*连续函数的均匀极限是连续的*。

#### 推论 1 {#top-x-s1-thm-2-cor-1 .statement tag=0CBG}

*如果$Y$是完整的制服空间，则$C_u(X; Y)$是完整的。*

因为，通过定理 2，$C_u(X; Y)$是均匀空间$F_u(X; Y)$的封闭均匀子空间，它由no. 5的定理1完成。

#### 推论 2 {#top-x-s1-thm-2-cor-2 .statement tag=0CBH}

*令$X$为拓扑空间，$\mathscr{S}$集合为$X$的子集，$Y$为均匀空间。 令$\tilde{C}_\mathscr{S}(X; Y)$表示$X$的所有映射到$Y$的集合，其中限制到$\mathscr{S}$的每个集合是连续的。 Then $\tilde{C}_\mathscr{S}(X; Y)$ is a closed subspace of the uniform space $F_\mathscr{S}(X; Y)$ and is complete if $Y$ is complete.*

假设$u$位于$F_\mathscr{S}(X; Y)$中$\tilde{C}_\mathscr{S}(X; Y)$的闭包内；那么(no. 2)，对于每个$A \in \mathscr{S}$，$u|A$位于$F_u(A; Y)$中$C(A; Y)$的闭包中，因此连续定理2。

#### 推论 3 {#top-x-s1-thm-2-cor-3 .statement tag=0CBI}

*令$X$为拓扑空间，其可度量或局部紧凑，并令$Y$为均匀空间。那么$C(X; Y)$在均匀空间$F_c(X; Y)$中闭合；如果加法 $Y$ 已完成，则制服空间 $C_c(X; Y)$ 已完成。*

凭借推论 2 就足以证明，如果我们将$\mathscr{S}$视为$X$的紧凑子集的集合，则在考虑的两种情况下我们都有$\tilde{C}_\mathscr{S}(X; Y) = C(X; Y)$。如果 $X$ 是局部紧致的，这一点是很清楚的。如果$X$是可度量的，并且$u : X \to Y$是映射，其限制对于$X$的每个紧凑子集是连续的，那么对于$x \in X$和$X$的点的每个序列$(z_n)$，收敛到$x$，我们有$u(x) = \lim_{n \to \infty} u(z_n)$，因此$u$在$x$连续（章IX, § 2, no. 6，命题10）。

请注意，只要 $x$ 的每个点都有一个“可数”基本系统邻域，上述论点就适用。

#### 注 1 {#top-x-s1-n6-rem-1 .statement tag=0CBJ}

一般来说，集合$\mathscr{C}(X; Y)$在$\mathscr{F}(X; Y)$相对于拓扑的*逐点*收敛并不封闭：在其他字中，连续函数的逐点极限不一定是连续的[习题 5 a)]。

#### 注 2 {#top-x-s1-n6-rem-2 .statement tag=0CBK}

$\mathscr{C}(X; Y)$ 上的滤波器可以*逐点*收敛到*连续*函数，而不均匀收敛到这个函数。

例如，在区间$I = [0, 1]$上，令$u_n$为实值函数，对于$x = 0$和$2/n \leq x \leq 1$等于0，对于$x = 1/n$等于1，并且在区间$[0, 1/n]$和$[1/n, 2/n]$中都是线性的。 序列$(u_n)$逐点收敛于0，但在$I$（cf.习题6）中不均匀收敛于0。

#### 注 3 {#top-x-s1-n6-rem-3 .statement tag=0CBL}

如果$X$是均匀的空间，则证明类似于命题8，表明$X$的“均匀连续”映射到$Y$的集合在$\mathscr{F}_u(X; Y)$中是“闭集”。

#### 注 4 {#top-x-s1-n6-rem-4 .statement tag=0CBM}

假设一致的空间 $Y$ 带有合成的交换律和结合律律（加法书写），使得映射 $(y, y') \to y + y'$ 在 $Y \times Y$ 上连续。那么，如果$(u_n)$是$X$的连续映射到$Y$的序列，那么级数其一般项是$u_n$*一致收敛*在$X$，和级数在 $X$ 上连续。

我们让读者来陈述连续映射的*一致可求*族（no. 1，注 5）的相应的结果。

#### 命题 9 {#top-x-s1-prop-9 .statement tag=0CBN}

*令$X$为拓扑空间，$Y$为均匀空间。那么$\mathscr{C}_u(X; Y) \times X$到$Y$的映射$(f, x) \to f(x)$是连续的。*

令$f_0 : X \to Y$为连续映射，令$x_0$为$X$的点，令$V$为$Y$的随从。连续映射$f : X \to Y$的集合$T$，使得所有$x \in X$的$(f(x), f(x_0)) \in V$是$\mathscr{C}_u(X; Y)$中$f_0$的邻域。另一方面，由于$f_0$是连续的，$X$中存在$x_0$的邻域$U$，使得所有$x \in U$都有$(f_0(x), f_0(x_0)) \in V$。因此，每当$(f, x) \in T \times U$时，我们就有$(f(x), f(x_0)) \in V$，结果得证。

### 习题 {#top-x-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
