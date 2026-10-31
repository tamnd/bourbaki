---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 4
section_title: Modules over integrally closed Noetherian domains
lang: zh
source: ac-i-vii
book_pages: 512-544, 571-578
pdf_pages: 0530-0562, 0589-0596
extraction: ocr
subsections:
    - "no": 1
      title: LATTICES
      page: 512
      pdf_page: 530
    - "no": 2
      title: DUALITY; REFLEXIVE MODULES
      page: 517
      pdf_page: 535
    - "no": 3
      title: LOCAL CONSTRUCTION OF REFLEXIVE MODULES
      page: 521
      pdf_page: 539
    - "no": 4
      title: PSEUDO-ISOMORPHISMS
      page: 523
      pdf_page: 541
    - "no": 5
      title: DIVISORS ATTACHED TO TORSION MODULES
      page: 527
      pdf_page: 545
    - "no": 6
      title: RELATIVE INVARIANT OF TWO LATTICES
      page: 529
      pdf_page: 547
    - "no": 7
      title: DIVISOR CLASSES ATTACHED TO FINITELY GENERATED MODULES
      page: 531
      pdf_page: 549
    - "no": 8
      title: PROPERTIES RELATIVE TO FINITE EXTENSIONS OF THE RING OF SCALARS
      page: 535
      pdf_page: 553
    - "no": 9
      title: A REDUCTION THEOREM
      page: 540
      pdf_page: 558
    - "no": 10
      title: MODULES OVER DEDEKIND DOMAINS
      page: 543
      pdf_page: 561
statements: 56
exercises: 26
content_sha256: 5b175d00dd298238cd430d71888e3d89b36eed84af1b9156b799f34fc16b793d
translated_from: content/en/ac/VII/04_s4_modules_over_integrally_closed.md
translation_method: google
source_content_sha256: 72d54cdf6923d26d9507679e68c08eb8627c1c668375ce55e331655e15e45177
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 6c01c6d38dbf36816b7d6eb7d3a492643c505c1efe0cf9226ac74dbc24431228
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4. 模过度封闭的诺特域

在本段中，$\mathbf{A}$将是一个*可交换的整环*，其中域为分数$K$。从 no. 2 开始，$\mathbf{A}$ 将进一步假定为 *诺特且整体闭合*（因此是一个 Krull 域（$\S$ 1，no. 3，定理 2 的推论））；那么$P(\mathbf{A})$、$D(\mathbf{A})$、$C(\mathbf{A})$分别表示高度为1的$\mathbf{A}$素理想的集合（$\S$1、no. 6）、$\mathbf{A}$的除子群 $\mathbf{A}$ ($\S$ 1, no. 10) 的 ($\S$ 1, no. 3) 和除子类群，后者被写成*相加*。

在整体封闭的诺特域$\mathbf{A}$上研究有限生成模的一般方法由关于$\mathbf{A}$中*高度* 1的所有素理想$p \in P(\mathbf{A})$的“本地化”模组成；作为$\mathbf{A}$，那么有限生成的$\mathbf{A}_p$模块的*离散评估环*（$\S$1，no. 6，定理4），结构是众所周知的（*代数*，章 VII、$\S$ 4)，因此给出了有关有限生成的 $\mathbf{A}$ 模块的结构的信息。在$\mathbf{A}$是戴德金域的特殊情况下，我们可以得到与$\mathbf{A}$是主理想整环（no. 10）时一样完整的理论。

### 1. 格子

#### 定义 1 {#ac-vii-s4-def-1 .statement tag=052X}

*令 $V$ 为有限维向量空间超过域 $K$。相对于$\mathbf{A}$的$V$格（或简单地$V$格）被定义为以下条件的$V$满足的任何子$\mathbf{A}$模块$M$：*

$V$ 存在两个自由子$\mathbf{A}$ 模块$L_1,\ L_2$，例如$L_1 \subset M \subset L_2$ 和$\mathrm{rg}_{\mathbf{A}}(L_1) = \mathrm{rg}_K(V)$。

例
(1) 如果我们采用 $V = K$，$K$ 的格子只是 $K$ 的*分数理想* $\neq (0)$ ($\S$ 1, no. 1, 定义 1)。

(2) 如果$\mathrm{rg}_K(V) = n$，V的每个*空闲*子A模块L最多有基包含至多n个元素，V的每个子集在A上空闲，在K上空闲；为了使L成为V的格子，L有基n个元素是充分必要的（在其他字中，即$\mathrm{rg}_A(L) = n$）。

(3) 如果 A 是 *主理想整环*，V 的每个格子 M 都是有限生成A-模（因为 A 是诺特），它是无扭转的，因此是*自由* A-模 (*代数*, 章 VII, § 4, no. 3，推论2 至定理 2)。

#### 命题 1 {#ac-vii-s4-prop-1 .statement tag=052Y}

*对于V的子A模M成为V的格，KM =V并且M包含在V的有限生成的子A模中是必要且充分的。*

条件显然是必要的，对于V 的免费子 A 模块，其秩与 V 生成 V 相同。相反，如果 KM = V，则 V 的 M 包含基 $(a_i)_{1 \leq i \leq n}$ 超过 K，因此它包含是由 $a_i$ 生成的自由子 A 模块 L；另一方面，如果$M \subset M_1$（其中M）是由元素 b 的有限数生成的V的子A模，并且$(e_i)_{1 \leq i \leq n}$是K上V的基，则存在元素 s A 的 $\neq 0$，使得每个 b 是 $s^{-1}e_i$ 的线性组合，系数 *in* A；如果L是$s^{-1}e_i$生成的V的免费子A模块，则$M \subset L_2$。

#### 推论{#ac-vii-s4-n1-cor-1 .statement tag=052Z}

*假设A为诺特；对于V的子A模M成为V的格子，KM = V且M是有限生成的是必要且充分的。*

#### 注 (1) {#ac-vii-s4-n1-rem-1 .statement tag=0530}

回想一下，对于 V 典范映射 $M \otimes_A K \to V$ 的每个子 A 模块 M 都是单射的，并且具有像 KM (*代数*, 章 II, § 7, no. 10, 命题 26)；说 KM = V 意味着这个映射是*双射的*。

#### 命题 2 {#ac-vii-s4-prop-2 .statement tag=0531}

*设M为V的格子，M为V的子A模。如果$K^*$存在两个元素 x，y，使得$xM \subset M_1 \subset yM$，$M_1$是V的格子；相反，如果$M_1$是V的格，则A存在两个非零元素 a, b，使得$aM \subset M, \subset b^{-1}M$。*

如果$L_1, L_2$是V的两个自由格，那么$L, \subset M \subset L,$、关系$xM \subset M_1 \subset yM$意味着$xL_1 \subset M, \subset yL_2$、$xL_1$和$yL_2$是自由格；相反，如果 M, 是一个格，并且 L 的 $(e_i)_{1 \leq i \leq n}$ 基，在 A 上，关系 KM, = V 意味着存在 $x = a/s \in K^*$（其中 a 和 s 是 A 的非零元素），使得 $xe_i \in M,$ 对于所有$i$、从而 $xM \subset xL_2 \subset M_1$ 和 *更不必说* $aM \subset M,$；交换M和M的角色，类似地可以证明A中存在$b \neq 0$使得$bM_1 \subset M$。

#### 命题 3 {#ac-vii-s4-prop-3 .statement tag=0532}

(i) *如果$M_1$和$M_2$是V的格子，那么$M_1 \cap M,$和$M_1 + M_2$也是。

(ii) *如果W是V的向量子空间并且M是V的格子，则$M \cap W$是W的格子。*

(iii) 令 $V, V_1, \ldots, V_k$ 为有限秩中的向量空间超过$K$，并让
$$
f : V_1 \times \cdots \times V_k \to V
$$
是一个多线性映射，其像生成 $V$。 *如果$M_i$是$1 \leq i \leq k$的$V_i$的格，则$f$（$(M, x \ldots x M_k)$）生成的$V$的子A模是$V$的格。*

(iv) 设$V$和$W$是有限秩的两个向量空间超过$K$，$M$是$V$的格子，$N$是$W$的格子。 *子A模$N$：$\mathrm{Hom}_K(V, W)$的$M$，K-线性映射$f$的由……组成，使得$f(M) \subset N$是$\mathrm{Hom}_K(V, W)$的格子。*

(i) 由于命题 2，$A$中存在非零$a$和$b$，使得$aM_1 \subset M_2 \subset b^{-1}M_1$；我们结论，$M_1 \cap M_2$和$M_1 + M_2$位于$aM_1$和$b^{-1}M_1$之间，因此根据命题2是格子。

(ii) 设$S$是$V$中$W$的补集，$L_w$是$W$的自由格，$L_s$是$S$的自由格，因此$L = L_w \oplus L_s$是$V$的自由格。那么$K^*$中存在$x, y$使得$xL \subset M \subset yL$。我们推导出$xL_w \subset M \cap W \subset yL_w$，这表明$M \cap W$是$W$（命题2）的格子。

(iii) 作为 $KM_i = V$，显然由线性 $f$ ($M_1 x \ldots x M_n$) 生成向量 K 空间$V$；另一方面，对于所有$i$，存在一个有限生成的$V$的子A模块$N_i$，使得$M_i \subset N_i$；由$f(N_1 x \ldots x N_n)$生成的$V$的子A模$N$是有限生成的，并且包含$M$，因此$M$是$V$（命题1）的格子。

(iv) 令 $P$ ($Q$) 为 $V$ ($W$) 包含于 $M$ ($N$) 的自由格；显然$N : M \supset Q : P$。现在$Q : P$与$\mathrm{Hom}_A(P, Q)$同构的是直接的，因此秩$(\mathrm{rg}_A P)(\mathrm{rg}_A Q)$是自由A-模（*代数*，章II, § 1, no. 6，推论1到命题6）因此格子为 $\mathrm{Hom}_K(V, W)$。类似地，如果 $P'$（分别为 $Q'$）是包含在 $M$（分别为包含 $N$）中的 $V$（分别为 $W$）的自由格子，则 $Q' : P' \supset N : M$ 和 $Q' : P'$ 为$\mathrm{Hom}_K(V, W)$； 从而结论。

*注*
(2) 命题 3 (i) 表明 $V$ 晶格的集合 $R(V)$ 就包含而言是*晶格有序*；此外，如果$M$是$V$的固定格子，则$xM$，其中$x$贯穿$K^*$、形式子集，$R(V)$既是*初始*又*并尾*（*集合理论*， 章III, § 1, no. 7）。

(3) 命题 3(iv)中的记号、典范映射
$$
N : M \to \mathrm{Hom}_A(M, N),
$$
其中映射从$M$到$N$的每个K-线性映射$f \in N : M$到A-线性映射，与$f|_M$具有相同的图，是*双射的*，对于每个A-线性映射$g : M \to N$都可以嵌入K-线性映射
$$
g \otimes 1 : M \otimes_A K \to N \otimes_A K
$$

可以看出，$M \otimes_A K$和$N \otimes_A K$分别与$V$和$W$进行标识。

特别是，如果我们取 $W = K$、$N = A$、$\operatorname{Hom}_K(V, W)$ 只是 $V$ 和 $A$ 的*对偶向量 K 空间* $V^*$：$M$ 与*对偶 A-模* 进行标识$M^*$共$M$；今后我们将进行这种识别，我们将说$M^*$是$M$的*对偶格子*：因此它是*$x^* \in V^*$的*集合*使得*$\langle x, x^* \rangle \in A$*对于所有*$x \in M$。

#### 推论{#ac-vii-s4-n1-cor-2 .statement tag=0533}

*令 U、V、W 为 K 和 f 上有限秩的三个向量空间：U × V → W 左非简并 K 双线性映射* (代数、章 IX, § 1, no. 1、定义 3)。 *如果 M 是 V 的格子，N 是 W 的格子，集合 N: ,M of x ∈ U 使得 f (x, y) ε N for ally ∈ M 是 U* 的格子。

令 $s_f: U \to \operatorname{Hom}_K(V, W)$ 为 K-线性映射与 $f$ (代数, 章 IX, *loc. cit.*) 关联，使得 $s_f(x)$ 为线性映射 $y \mapsto f(x, y)$；回想一下，说 $f$ 保持非退化意味着 $s_f$ 是*内射*。由命题 3 (iv)，$N: M$是$\operatorname{Hom}_K(V, W)$的格子；由于 $N: fM = s_f^{-1}(N: M)$ 和 $s_f$ 是单射的，因此推论来自命题 3 (ii)。

*例*

(4) 令$S$为有限秩与单位元的（不一定结合）K-代数；那么$S \times S$到$S$的双线性映射$(x, y) \mapsto xy$（左和右）是非退化的。 If $M$ and $N$ are lattices of $S$ with respect to $A$, so are $M.N$ (命题 3 (iii)) and 集合 of $x \in S$ such that $xM \subset N$ (Corollary to 命题 3). 注存在$S$包含单位元的$S$的*子A代数*，它是$S$的*格子*； for consider 基 $(e_i)_{1 \leq i \leq n}$ of $S$ such that $e_1$ is 单位元 of $S$ and let $e_i e_j = \sum_k c_{ijk} e_k$ be 乘法表 of $S$ ($1 \leq i \leq n, 1 \leq j \leq n$), *so that* $c_{1jk} = \delta_{jk}, c_{i1k} = \delta_{ik}$（克罗内克符号）。令 $s \in A$ 为非零，且$c'_{ijk} = s \cdot c_{ijk} \in A$ 对于指标 $(i, j, k)$ 的所有三元组；如果我们将 $i \geq 2$ 写为 $e'_i = s^{-1} e_i$，那么

$$
e'_i e'_j = s c'_{ij1} e'_1 + \sum_{k \geq 2} c'_{ijk} e'_k
$$

对于 $i \geq 2$ 和 $j \geq 2$； $S$ 与基 $e_1$ 和 $e'_i$ ($2 \leq i \leq n$) 的格子是 $S$ 与单位元 $e_1$ 的亚 A 代数。

(5) 令$V$是$K$上的有限维向量空间，并且$f$是$V$上的非简并双线性形式。 If $M$ is a lattice of $V$, it follows from the Corollary to 命题 3 that 集合 $M^*_f$ of $x \in V$ such that $f(x, y) \in A$ for ally $\in M$ is also a lattice of $V$;如果 $s_f: V \to V^*$ 是线性映射与 $f$（双射的）相关联，则 $s_f(M^*_f)$ 只是 $M$ 的对偶晶格 $M^*$。

#### 命题 4 {#ac-vii-s4-prop-4 .statement tag=0534}

*设B为B和K的整环，A子环，以及L分别为A和B的域和分数。令V为K上的有限维向量空间。*

(i) For every lattice $M$ of $V$ with respect to $A$, 像 $BM$ of $M_{(B)} = M \otimes_A B$ in $V_{(L)} = V \otimes_K L$ is a lattice of $V_{(L)}$ with respect to $B$.

(ii) 进一步假设 $B$ 是一个平面 $A$ 模。那么典范映射 $M_{(B)} \to BM$ 是双射的。如果进一步$B$是忠实平坦的，则映射其中映射$V$相对于$A$的每个格子$M$到$V_{(L)}$相对于$B$的格子$BM$都是单射的。

(i) As $KM = V$, clearly $L . (BM) = V_{(L)}$; on the other hand $M$ is contained in a finitely generated sub-$A$-module $M_1$ of $V$ and hence $BM$ is contained in $BM_1$ which is a finitely generated $B$-module; whence assertion (i) (Proposition 1).

(ii) $V_{(L)} = V \otimes_K L = V \otimes_A L$ (章 II, § 2, no. 7, 命题 18) 并且，由于 $L$ 是扁平 $B$ 模，因此它也是扁平 $A$ 模 (章 I, § 2, no. 7，推论 3 至命题 8).由于$B$是平$A$模，典范映射$M \otimes_A B \to V \otimes_A B$是单射的；另一方面，由于 $V$ 是一个自由的 $K$ 模块，$K$ 是一个平面 $A$ 模块，$V$ 是一个平面 $A$ 模块（章 I, § 2, no. 7，推论 3 到命题 8），因此典范映射 $V \otimes_A B \to V \otimes_A L$ 是单射，它建立了第一个断言。还要看到，当$B$是忠实平坦的$A$模时，关系$BM_1 = BM_2$对于$V$的两个格子$M_1, M_2$相对于$A$意味着$M_1 = M_2$，注首先是$BM_1 \cap BM_2 = B(M_1 \cap M_2)$ （章I, § 2, no. 6，命题6）；因此，我们可以将注意力集中在$M_1 \subset M$的情况，然后我们的断言从章I, § 3, no. 1，命题3应用到典范嵌入$M_1 \to M_2$。

#### 推论{#ac-vii-s4-n1-cor-3 .statement tag=0535}

假设$A$是离散估值环。令$\hat{A}$为其补全，令$\hat{K}$为$\hat{A}$的分数的域（章VI, § 5, no. 3）。 映射$\phi$，其中映射$V$的每个格子$M$到$\hat{V} = V \otimes_K \hat{K}$的格子$\hat{A}M$相对于$\hat{A}$是双射且其逆映射$\hat{V}$的每个格子$M'$相对于$\hat{A}$到其交$M' \cap V$（$V$被规范地识别为$\hat{V}$的向量子K空间）。

如果$L$是$V$的自由格，则$aL$（对于$a \in A, a \neq 0$）形式是邻域的基本系统为0，对于$V$上的拓扑$\mathscr{T}$（与其兼容） $A$-模块结构），（当取$L$超过$A$的基时）被识别为$K^n$上的乘积拓扑）；凭借命题 2，对于$\mathscr{T}$，邻域的基本系统为0，也由$V$相对于$A$的所有格组成；显然$\hat{V}$是$V$相对于$\mathscr{T}$的补全。此外，如果$m$是$A$的最大理想，拓扑$\mathscr{T}$诱导在$V$的每个格子$M$上关于$A$的$m$进数拓扑，因为$M$是有限生成的$A$模块（章III, § 3, no. 2，定理2），$\hat{A}M$是$M$相对于此拓扑的补全（章III, § 2, no. 12， 命题16);此外，由于$M$在$V$、$\hat{A}M \cap V = M$中是开（因此闭）的，这再次证明$\dagger$是单射的（这直接从命题4，（ii）得出，因为$A$是一个忠实的平面$A$模）。最后，如果$M'$是$\hat{V}$相对于$\hat{A}$的格子，$M = M' \cap V$是$V$相对于$A$的格子，对于$\hat{A}$的每个元素是元素的乘积 $\hat{A}$的$A$和可逆元，因此从命题2得出，$A - \{0\}$中存在$a, b$，使得$a \hat{A}L \subset M' \subset b \hat{A}L$，从而$aL \subset M' \cap V \subset bL$。此外，$M'$在$V$中开放，并且由于$V$在$\hat{V}$中密集，所以$M'$是$M' \cap V = M$的完成；这证明$\phi$是满射，从而是推论。

例 (6) 设$S$是$A$的乘法子集，而不是包含 0；我们应用命题 4 到$B = S^{-1}A$；然后$L = K$，$BM = S^{-1}M$；因此$S^{-1}M$是$V$相对于$S^{-1}A$的格子。此外：

#### 命题 5 {#ac-vii-s4-prop-5 .statement tag=0536}

*让有限秩的$V, W$向量空间超过$K$，$M$$V$的格子和$N$$W$的格子。如果 $M$ 是有限生成的，则（在命题 3 的记号中）：*

(1)
$$
S^{-1}(N : M) = S^{-1}N : S^{-1}M
$$
*在*$\operatorname{Hom}_K(V, W)$。

显然，(1) 的左侧包含在右侧。相反，令$f \in S^{-1}N : S^{-1}M$且令$(x_i)_{1 \leq i \leq n}$为$M$的生成元系统。存在$s \in S$，使得$f(x_i) \in s^{-1}N$对于所有$i$，因此存在$sf \in N : M$，这证明了命题。

### 2.二元性；反身模

回想一下，从现在起，域 $A$ 被假定为 *诺特且整体闭合*，并且 $P(A)$（或简称为 $P$）表示集合 $A$ *高度* 1 的素理想。关于 $A$ 的每个格都是“有限生成的” $A$-模块（no. 1，命题 1 的推论）。

设$V$为有限秩除以$K$的向量空间，$V^*$为对偶，$V^{**}$为对偶；我们将通过典范映射$c_V$（*代数*，章II, § 7, no. 5，定理6）来认同$V$和$V^{**}$。设$M$为$V$的格子；回想一下，$M$的对偶$A$模$M^*$在规范上与$M$的*对偶格子*、$x^* \in V^*$的集合一致地识别，使得$\langle x, x^* \rangle \in A$对于所有$x \in M$；因此，$M$的*对偶的*$A$模$M^{**}$是$V$的*格子*，其中包含$M$。此外，$M^{***} = M^*$，对于关系$M \subset M^{**}$意味着$(M^{**})^* \subset M^*$，而另一方面$M^* \subset (M^*)^{**}$通过上述（cf.*集合理论*，章III, § 1, no. 5，命题2）。

如果 $p$ 是素理想，命题 5 与 $N = A$ 一起应用会得到关系 $(M^*)_p = (M_p)^*$，这证明记号 $M_p^*$ 对于项都是合理的。

#### 定理 1 {#ac-vii-s4-thm-1 .statement tag=0537}

*如果$M$是$V$的格子，则*$M^* = \bigcap_{p \in P} M_p^*$。

显然$M^*$包含在每个$M_p^*$中。相反，假设$x^* \in \bigcap M_p^*$；如果$x \in M$，则$\langle x, x^* \rangle \in \bigcap_{p \in P} A_p$，并且如$A = \bigcap_{p \in P} A_p$（§ 1, no. 6，定理 4），$x^* \in M^*$。

定理 1 应用于 $M^*$ 显示$M^{**} = \bigcap_{p \in P} M_p^{**}$。但由于 $A$ 是主理想整环（$§ 1$，编号 **6**，定理 **4**），$M$ 是有限生成的免费 $A$ 模块，因此 $M_p^{**}$ 被规范地标识为 $M$， （*代数*、章II、$§ 2$、第 **7**、命题 **14**）、从而推论。

对于任何格$M$相对于$A$，典范映射$c_M : M \to M^{**}$（*代数*，章11，$§ 2$，号**7**）将元素$x \in M$与其自身等同，因为$x$是唯一元素 $y$ / $V = V^{**}$，使得 $\langle x, x^* \rangle = \langle y, x^* \rangle$ 对于所有 $x^* \in M^*$，从 $M^*$ 生成 $V^*$ 开始。如果$M^{**} = M$（*loc.cit.*），我们可以说$M$是*自反*。正如我们上面的$M^* = (M^*)^{**}$，可以看出任何格子$M$的*对偶*总是*自反*。

#### 注 (1) {#ac-vii-s4-n2-rem-1 .statement tag=0538}

令 $M$ 为有限生成的 $A$ 模块； 直接的，$M$的对偶$M^*$，用$\operatorname{Hom}_A(M, K)$的子$A$模块标识，是向量$K$空间$\operatorname{Hom}_A(M, K)$的*格子*；特别是，每个有限生成的*自反*$A$-模块同构于合适的向量$K$-空间的格子。

#### 定理 2 {#ac-vii-s4-thm-2 .statement tag=0539}

*如果$M$是*$V$的格子，*以下条件是等价的*：
(a) $M$ *是反身的*。
(b) $M = \bigcap_{p \in P} M_p$。
(c) $\operatorname{Ass}(V/M) \subset P$。

(a) 和 (b) 的等价由推论得出定理 1。如​​果 (b) 成立，则 $V/M$ 被规范地识别为乘积 $\prod_{p \in P} (V/M_p)$ 的子$A$ 模块；但实际上，它包含在 *直和* $\bigoplus_{p \in P} (V/M_p)$ 中：因为如果 $L \subset M$ 是自由格，$L$ 的$(e_i)_{1 \leq i \leq n}$ 基，点 $x \in V$ 的每个坐标$x_i$ 相对于 $(e_i)$ 属于至 $A$，除了值的有限数或 $p \in P$。 关系 $V/M \subset \bigoplus_{p \in P} (V/M_p)$ 那么意味着：

$$
\operatorname{Ass}(V/M) \subset \bigcap_{p \in P} \operatorname{Ass}(V/M_p).
$$

由于$V/M_p$是$A_p$模，$A - p$不能的元素消灭$V/M_p$的元素$\neq 0$，因为$A - p$的元素可逆$A$；因此，$\operatorname{Ass}(V/M_p)$中的元素包含在$p$中并且是$\neq 0$，因为$V/M_p$是挠元$A$模；因为$p$的高度为**1**，如果$V/M_p \neq (0)$则必然为$\operatorname{Ass}(V/M_p) = \{ p \}$，如果$V/M_p = (0)$则必然为$\operatorname{Ass}(V/M_p) = \varnothing$；因此$\operatorname{Ass}(V/M) \subset P$。

最后，如果条件 (c) 成立，则

$$
\operatorname{Ass}(M^{**}/M) \subset \operatorname{Ass}(V/M) \subset P.
$$

另一方面，如果$p \in P$，则在定理1的推论的证明中可以看出，$M_p^{**} = M_p$，从而$p \notin \operatorname{Ass}(M^{**}/M)$（章IV，$§ 1$，no. 3，推论 1 至命题 7)。我们结论 Ass(M**/M) = ∅，从而 M** = M（章 IV, § 1, no. 1，推论 1 到命题 2）。

#### 推论{#ac-vii-s4-n2-cor-1 .statement tag=053A}

令 M、N 为关于 A 的两个V 格，使得 N 是自反的。在阶中，M ⊂ N，对于所有 p ∈ P，M_p ⊂ N_p 是充分必要的。

条件显然是必要的，如果满足的话，那么

$$
\bigcap_{p \in P} M_p \subset \bigcap_{p \in P} N_p = N.
$$

由于 M ⊂ M** = \bigcap_p M_p，当然 M ⊂ N。

例
(1) 每个自由格都是自反的。
(2) 取V = K。对于K的分数理想a是自反格，根据定理2和§ 1, no. 4、命题5和7的判据(b)，它是除数理想是充分必要的。
(3) 令M为关于A的格；如果 S 是 A 的乘法子集而不是包含 0，则 no. 1 的命题 5 表明 S^{-1}(M*) = (S^{-1}M)*；如果 M 是自反的，则 S^{-1}M 是相对于 S^{-1}A 的自反格。

#### 命题 6 {#ac-vii-s4-prop-6 .statement tag=053B}

(i) 如果 M_1 和 M 是 V 的自反格，则 M, n M 也是。
(ii) 如果 W 是 V 的向量子空间，并且 M 是 V 的自反格，则 M n W 是 W 的自反格。
(iii) 令V，W 为有限秩的两个向量空间，在K 和M（分别为N）上，为V（分别为W）的格子。如果 N 是自反的，则 Hom_K(V, W) (no. 1, 命题 3) 的格 N: M 是自反的。

(i) (M, n M_2)_p = (M_1)_p n (M_2)_p 对于所有 p ∈ P (章 II, § 2, no. 4, 定理 1)。如果 M_1 = \bigcap_{p \in P} (M_1)_p 且 M_2 = \bigcap_{p \in P} (M_2)_p，则

$$
M, n M_2 = \bigcap_{p \in P} (M, n M_2)_p
$$

从而根据定理 2 得出结论。
(ii) 类似地 (M n W)_p = M_p n W_p = M_p n W, 从而

$$
M \cap W = \bigcap_{p \in P} (M \cap W)_p,
$$

这就证明了(ii)。
(iii) 由于 M 是有限生成的，由 no. 1, 命题 5 得出 (N: M)_p = N_p M_p；此外，关系 N = \bigcap_{p \in P} N_p 意味着：

$$
N: M = \bigcap_{p \in P} (N_p : M_p).
$$

对于如果$f \in \bigcap_{p \in P} (N_p : M_p)$和$x \in M$，则$f(x) \in \bigcap_{p \in P} N_p = N$，从而$f \in N : M$；这表明 $N : M$ 是自反的。

注
(2) 如果$M_1$和$M_2$是$V$的自反格，则格$M_1 + M_2$不一定是自反格（cf.§ 1，习题2）。
(3) 如果$M$是有限生成的$A$模，并且$T$是挠元子模，则$M$的对偶$M^*$与$M/T$的对偶相同，因为，对于每个线性形式$f$ $M$、像 $f(T)$ 是 $A$ 的挠元子模，因此是零。由于$M/T$同构于向量空间超过$K$的格，可以看出每个有限生成的$A$模的对偶是自反的。

#### 命题 7 {#ac-vii-s4-prop-7 .statement tag=053C}

令 $0 \to M \to N \to Q \to 0$ 为 $A$ 个模块中的正合序列。假设 $N$ 是有限生成且无扭转的。
(i) 如果$M$是自反的，则$\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$（在其他字中，与$Q$相关的每个理想，要么是$(0)$，要么是高度1）。
(ii) 相反，如果 $N$ 是自反的且 $\operatorname{Ass}(Q) \subset P \cup \{\{0\}\}$，则 $M$ 是自反的。

由于$A$是诺特，$M$也是有限生成的；如果我们写 $V = M_{(K)}$、$W = N_{(K)}$、$M$（分别为 $N$），则可以用 $V$（分别为 $W$）（no. 1、命题 1）的格子来规范地识别。考虑两个正合序列：
$$
0 \to V/M \to W/M \to W/V \to 0 \\
0 \to Q \to W/M \to W/N \to 0.
$$
(i) 我们推论 (章 IV, § 1, no. 1, 命题 3)：
$$
\operatorname{Ass}(Q) \subset \operatorname{ASS}(W/M) \subset \operatorname{ASS}(V/M) \cup \operatorname{ASS}(W/V).
$$
如果 $M$ 是自反的，则 $\operatorname{Ass}(V/M) \subset P$ (定理 2)；另一方面，显然$\operatorname{Ass}(W/V)$要么是空的，要么减少到$\{0\}$； 从而（一）。
(ii) 同样：
$$
\operatorname{Ass}(V/M) \subset \operatorname{Ass}(W/M) \subset \operatorname{Ass}(Q) \cup \operatorname{Ass}(W/N).
$$
因此，假设意味着 $\operatorname{Ass}(V/M) \subset P \cup \{\{0\}\}$。但$V/M$是挠元$A$-模块，因此$\{0\} \notin \operatorname{Ass}(V/M)$； 定理 2 那么表明 $M$ 是自反的。

#### 命题 8 {#ac-vii-s4-prop-8 .statement tag=053D}

令$R$和$S$是两个交换环，$p : R \to S$环同态和$M$有限生成的$R$模块。假设 $R$ 是诺特并且 $S$ 是一个平面 $R$ 模块。那么，如果 $M$ 是自反的，那么 $S$ 模块 $M_{(S)} = M \otimes_R S$ 也是自反的。
我们知道 (章 I, § 2, no. 10, 命题 11) 存在典范同构 $\omega_M : (M^*)_{(S)} \to (M_{(S)})^*$，使得
$$
\langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle = \rho(\langle x, x^* \rangle)
$$

€或 x \in M，x^* \in M^*。由于 M 是有限生成的自由 R 模 L 的商，因此 M* 同构于对偶 L* 的子 R 模，并且 L* 是自由且有限生成的；由于 $\mathbf{R}$ 是诺特，因此 M* 也是有限生成的 R 模块，从而同构 $\omega_{M^*}: (M^{**})_{(S)} \to ((M^*)_{(S)})^*$ 使得

$$
\langle x^* \otimes 1, \omega_{M^*}(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle)
$$

对于 $x^* \in M$ 和 $x^{**} \in M^{**}$。另一方面，还有同构$^t\omega_M: (M_{(S)})^{**} \to ((M^*)_{(S)})^*$、从而乘合成典范同构：

$$
\phi = (t\omega_M^{-1}) \circ (\omega_{M^*}): (M^{**})_{(S)} \to (M_{(S)})^{**}
$$

这样，在上面的记号中：

(1)

$$
\langle \omega_M(x^* \otimes 1), \phi(x^{**} \otimes 1) \rangle = \rho(\langle x^*, x^{**} \rangle).
$$

我们现在考虑典范同态 $c_M: M \to M^{**}$ 并证明复合同态 ：

(2)

$$
\psi: M_{(S)} \xrightarrow{c_M \otimes 1} (M^{**})_{(S)} \longrightarrow (M_{(S)})^{**}
$$

只是典范同态$c_{M_{(S)}}$。这直接从 (1) 得出关系 ：

$$
\langle \omega_M(x^* \otimes 1), \psi(x \otimes 1) \rangle = \rho(\langle x^*, c_M(x) \rangle)
$$
$$
= \rho(\langle x, x^* \rangle) = \langle x \otimes 1, \omega_M(x^* \otimes 1) \rangle
$$

并且从事实来看，元素$\omega_M(x^* \otimes 1)$生成$(M_{(S)})^*$。既然如此，假设 M 是自反的，则意味着 $c_M$ 是双射的，因此 $c_M \otimes 1$ 也是双射的，因此 $\psi = c_{M_{(S)}}$ 是双射的，这表明命题。

### 3. 反身模的本地构造

我们保留记号和no. 2的假设。我们可以说，如果 $p \in P$ 的集合不成立，那么性质 *对于几乎所有* $p \in P$ 都成立*是有限的*。

#### 定理 3 {#ac-vii-s4-thm-3 .statement tag=053E}

*设V为K和M上有限秩的向量空间，相对于A为V的格子。*

(i) *令 N 为相对于 A V 的格子；那么，对于 A 的每个素理想 p，$N_p$ 是关于 A 的V 格，并且对于几乎所有* $p \in P, N_p = M_p$。

(ii) *相反，假设对于 A 而言，给出所有* $p \in P$ *格子* $N(p)$ *的 V，使得* $N(p) = M_p$ *对于几乎所有* $p \in P$。 *那么*$N = \bigcap N(p)$*是A相对于A的自反格子，并且它是V关于A的唯一自反格子*$N'$*使得*$N'_p = N(p)$*对于所有*$p \in P$。

(i) 第一个断言由no. 1，命题4得出。此外，$\mathbf{K}^*$中存在$x, y$，使得$xN \subset M \subset yN$(no. 1，命题2)；我们知道，对于几乎所有$p \in P, v_p(x) = v_p(y) = 0$（$§ 1$，no. 6，定理 4），这表明$x$和$y$在$A$中是可逆的，因此$M_p = N_p$。

(ii) 我们可以将替换$M$乘以$x^{-1}M$，其中$x \neq 0$在$A$中，并假设$N(p) \subset M$，对于所有$p \in P$。令$p_1, \ldots, p_h$为$P$的元素，使得$N(p) = M$，因为$p$不同于$p_i$（$1 \leq i \leq h$）；我们写：

$$
Q = M \cap N(p_1) \cap \cdots \cap N(p_h).
$$

由于每个 $N(p_i)$ 包含都是关于 $A_{p_i}$ 的自由格，因此包含 *更不必说* 是关于 $A$ 的 $V$ 格，因此 $Q$ 包含是关于 $V$ 的格$A$ (no. 1, 命题 3) 并且，由于$Q$包含在$M$中，$Q$是关于$A$的格子。为了证明$Q_p = N(p)$对于所有$p \in P$，我们将使用以下引理：

#### 引理 1 {#ac-vii-s4-lem-1 .statement tag=053F}

*令$p$和$p'$为$A$的两个素理想，这样(0)是$p \cap p'$中包含的$A$的唯一素理想。然后，对于$V$的每个子A模块$E$，$(E_p)_{p'} = K.E.$*

令$S$为$A$的乘法子集$(A - p)(A - p')$；由章 II、$§ 2$、no. 3、命题 7、$(E_p)_{p'} = S^{-1}E$。此外，$A \subset S^{-1}A \subset K$； $S^{-1}A$ 对应的素理想到 $A$ 的素理想 $q$，使得 $q \cap S = \varnothing$ (章 II, $§ 2$, no. 5, 命题 11) 并且假设(0)是$A$唯一不满足$S$的素理想；因此$S^{-1}A = K$和$S^{-1}E = K.E.$

我们现在回到(ii)的证明。如果 $p \in P$ 与 $p_i$ ($1 \leq i \leq h$) 不同，则将引理 1 应用于 $N(p_i)$ 会得到 $((N(p_i))_{p_i})_p = (K.N(p_i))_p = V$，因为 $p_i$ 和 $p$ 的高度为 1。那么

$$
Q_p = M_p \cap (N(p_1))_p \cap \cdots \cap (N(p_h))_p = M_p = N(p)
$$

（章II、$§ 2$、no. 4）。另一方面，如果 $p$ 等于 $p_i$ ($1 \leq i \leq h$)，则根据上述参数和 $(N(p_i))_{p_i} = N(p_i)$、从而，$(N(p_i))_{p_j} = V$ 等于 $i \neq j$

$$
Q_{p_i} = M_{p_i} \cap N(p_i) = N(p_i).
$$

因此，我们证明了$Q_p = N(p)$对于所有$p \in P$。然后

$$
N = Q^{**} = \bigcap_{p \in P} Q_p
$$

是自反的并且满足所有$p \in P$的关系$N_p = Q_p = N(p)$； 唯一性性质紧接在 no. 2 的定理 2 之后。

#### 注 {#ac-vii-s4-n3-rem-1 .statement tag=053G}

令$L$为$V$相对于$A$的自由格。由于$A_p$对于$p \in P$来说是主理想整环，$N(p)$是与$L$相同的秩的自由$A$模块，并且存在$u(p) \in \mathbf{GL}(V)$使得$u(p)(L_p) = N(p)$；这个条件还有确定$u(p)$到乘法到$\mathbf{GL}(L_p)$的元素之内。 条件$N(p) = L_p$对于几乎所有$p \in P$意味着必然$u(p) \in \mathbf{GL}(L_p)$对于几乎所有$p \in P$。家庭$(u(p))_{p \in P}$满足后者性质形式乘法群$\mathbf{GL}_a(V)$包含为子群乘积$\prod_{p \in P} \mathbf{GL}(L_p)$。 定理 3 然后表明 V 自反格的 *集合与齐次空间* $\mathbf{GL}_a(V)/\prod_{p \in P} \mathbf{GL}(L_p)$ 处于规范的一对一对应中。如果选择 A 上的 L 的基 $(e_i)_{1 \leq i \leq n}$，则$\mathbf{GL}(V)$（分别为 $\mathbf{GL}(L_p)$）被识别为可逆矩阵 $\mathbf{GL}(n, K)$（分别为 $\mathbf{GL}(n, A, )$）和群的群 $\mathbf{GL}_a(V)$与阶$n$、$(U(p))_{p \in P}$的矩阵、系统群，使得$U(p) \in \mathbf{GL}(n, K)$对于所有$p \in P$以及$U(p) \in \mathbf{GL}(n, A_p)$对于几乎所有$p \in P$。如果 A 是 Dedekind 域，群 $\mathbf{GL}_a(V)$ 也可以用群 $\mathbf{GL}(n, A)$ 来标识，其中 A 是受限 adèles ($§ 2$, no. 4) 的环。

### 4. 伪同构

我们保留记号和 no 的假设。 2和3。

#### 命题 9 {#ac-vii-s4-prop-9 .statement tag=053H}

*设M为有限生成A-模。以下条件是等效的*：

(a) $M_p = 0$ 对于*每个素理想* $p$ 高度为 $\leq 1$。
(b) *湮没子* $a \triangleleft M$ *是理想* $\neq (0)$ *和* $A : a = A$ (*A*: $a$ 表示，如$§ 1$、no. 1、*集合的* $x \in K$ *这样* $xa \in A$）。

我们知道（章II，$§ 2$，no. 2，推论2到命题4）条件$M_p = 0$等价于$a + p$，因此也等价于$aA_p = A$，（章） II、$§ 2$、no. 5、*注*)；另一方面，对于A的每个积分理想$b \neq 0$，关系“*$bA_p = A$，对于所有$p \in P$*”相当于$D(A)$中的$\operatorname{div} b = \operatorname{div} A = 0$（$§ 1$，no. 4，命题7），或者也等于$\operatorname{div}(A : b) = 0$并且，由于$A : b$是除数（$§ 1$、no. 1、命题 1），因此关系也等于$A : b = A$。 命题然后注意到，说$a \notin p$ 代表$p = (0)$ 意味着$a \neq (0)$。

#### 注 (1) {#ac-vii-s4-n4-rem-1 .statement tag=053I}

命题 9 的等效条件也意味着 $\operatorname{Ass}(M)$ 包含没有身高 $\leq 1$ 的素理想。 *它们也可以被说解释为* $\operatorname{Supp}(M)$ *具有余维数* $\geq 2$ *在* $\operatorname{Spec}(A)$ 中。 \*

#### 定义 2 {#ac-vii-s4-def-2 .statement tag=053J}

*如果A-模 M 是有限生成的并且满足命题 9 的等价条件，则称为伪零。*

这个定义和命题9表明伪零A-模是*挠元A-模*； 逆命题是假的。

*例*
(1) 如果 A 是 Dedekind 域，则 A 的每个素理想的高度为 $\leq 1$；说 M 是伪零意味着 $\operatorname{Supp}(M) = \varnothing$，因此意味着 $M = 0$ (章 11, $§ 4$, no. 4)。

(2) 设$k$为域且$A = k[X, Y]$多项式环超过$k$，有两个不定式；如果$m$是$A$的最大理想$AX + AY$，则$A$模$A/m$是伪零；因为它的湮没子$m$不是高度$\leq 1$，因为它包含是主要素理想$AX$和$AY$并且与它们不同；因此$A : m = A$（§ 1, no. 6，推论1至定理3）。

#### 定义 3 {#ac-vii-s4-def-3 .statement tag=053K}

*令$M$和$N$为两个$A$模块和$f : M \to N$同态。如果 $\mathrm{Ker}(f)$（分别为 $\mathrm{Coker}(f)$、$\mathrm{Im}(f)$）是伪零，则 $f$ 称为伪内射（分别为伪满射伪零）；如果 $f$ 既是伪内射又是伪满射，则称为伪双射。*

伪双射同态也称为*伪同构*。

假设$M$和$N$是有限生成的；那么，对于 $f : M \to N$ 是伪内射（或伪满射、伪零），对于所有 $p \in P \cup \{\{0\}\}$、$f_p : M_p \to N_p$ 是内射（或伪满射、零）是必要且充分的；这是根据$A$-模块$A$的平坦度得出的，(cf.章I, § 2, no. 3，*注2*)。

*例 (3)* 令$M$为无扭有限生成$A$模；那么 $M$ 的典范映射 $c_M : M \to M^{**}$ 对其对偶是*伪同构*。对于$M$，用$V = M \otimes_A K$（no. 1，命题 1）的格子来识别；我们已经看到，对于所有 $p \in P$（no. 2、例 2），$M_p = M_p^{**}$ 以及对于 $p = 0$、$M_p$ 和 $M_p^{**}$ 都等于 $V$。

#### 定理 4 {#ac-vii-s4-thm-4 .statement tag=053L}

*令$E$为$E$和$M = E/T$的有限生成的$A$模，$T$挠元子模。存在伪同构*

$$
f : E \to T \times M.
$$

我们首先展示两个引理。

#### 引理 2 {#ac-vii-s4-lem-2 .statement tag=053M}

*设$(p_i)_{1 \leq i \leq k}$为$A$高度为1的非空有限素理想族，并设$S = \bigcap_i (A - p_i)$；那么环$S^{-1}A$就是主理想整环。*

$S^{-1}A$是一个半局部环，其最大理想是$1 \leq i \leq k$的$m_i = p_i S^{-1}A$，局部环$(S^{-1}A)_{m_i}$同构于$A$，（章11，§ 3, no. 5，命题17），因此是离散估值环。因此，环$S^{-1}A$是戴德金域（§ 2, no. 2，定理1（f）），并且由于它是半局部的，所以它是主理想整环（§ 2, no. 2，命题1）。

#### 引理 3 {#ac-vii-s4-lem-3 .statement tag=053N}

*存在同态$g : E \to T$，其限制到$T$既是位似又是伪同构。*

设$a$为$T$中的湮没子；因为$T$是有限生成的挠元$A$模块，$a \neq 0$。设 $p_i$ ($1 \leq i \leq k$) 为高度 1 包含 $a$ 的素理想（在数 ($§\ 1$, no. 6, 定理 4) 中是有限的）；如果数是0，T是伪零（命题9(a)），我们可以取$g = 0$。否则，设 $S = \bigcap_i (A - p_i)$；通过引理 2，$S^{-1}A$ 为主理想整环，因此 $S^{-1}M$（无扭转有限生成 $S^{-1}A$ 模块）是*自由*（*代数*，章 VII, §4, no. 3，推论 2 到定理 2) 并且，作为$S^{-1}M = (S^{-1}E)/(S^{-1}T)$，$S^{-1}T$是$S^{-1}E$的直因子(*代数*，章II, §1, no. 11，命题21)。现在，

$$
\operatorname{Hom}_{S^{-1}A}(S^{-1}E, S^{-1}T) = S^{-1} \operatorname{Hom}_A(E, T)
$$

（章II, §2, no. 7，命题19）；因此存在$s_0 \in S$和$g_0 \in \operatorname{Hom}_A(E, T)$使得$s_0^{-1}g_0$是$S^{-1}E$的投影算子到$S^{-1}T$。如果$h_0 \in \operatorname{Hom}_A(T, T)$表示$g_0$到$T$中的限制，则存在$s_1 \in S$，使得$s_1 h_0(x) = s_1 s_0 x$对于所有$x \in T$；因此，写 $s = s_1 s_0$、$g = s_1 g_0$、$h = s_1 h_0$、$h$ 是 $T$ 上比率 $s$ 的位似，并且是 $g$ 到 $T$ 的限制。 $h$是伪同构还有待验证。现在，如果 $p = 0$ 或 $p \in P$ 不同于 $p_i$ ($1 \leq i \leq k$)、$T_p = 0$ (章 II, §4, no. 4、命题 17) 并且 $h,\ : T_p \to T_p$ 是同构；相反，如果$p$等于$p_i$（$1 \leq i \leq k$）之一，$s$在$A$中是可逆的，并且$h_{,,}$，位似与$T_{p_i}$的比率$s$，也是同构，完成引理 3 中的证明。

现在我们证明定理 4。令$g : E \to T$为同态满足引理 3的性质；令$h$为$g$至$T$的限制，令$x$为$E$到$M$的规范投影。我们证明同态$f = (g, x) : E \to T \times M$可以解决问题。有交换律图表：

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T & \longrightarrow & E & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow h & & \downarrow f & & \downarrow I_M & & \\
0 & \longrightarrow & T & \longrightarrow & T \times M & \longrightarrow & M & \longrightarrow & 0
\end{array}
$$

其中行是准确的。蛇图表 (章 I, §1, no. 4, 命题 2) 给出正合序列：

$$
0 \to \operatorname{Ker}(h) \to \operatorname{Ker}(f) \to 0 \to \operatorname{Coker}(h) \to \operatorname{Coker}(f) \to 0
$$

因此 $\operatorname{Ker}(f)$ 与 $\operatorname{Ker}(h)$ 同构的，$\operatorname{Coker}(f)$ 与 $\operatorname{Coker}(h)$ 同构的。由于$h$是伪同构，$f$也是伪同构。

我们可以说“在伪同构内”定理 4 约化有限生成$A$模块的研究一方面是无扭转模块的研究，另一方面是挠元模的研究。此外，我们在上面（*例 3*）看到，无扭转模块与其双元伪同构，因此与*自反* 模伪同构。对于挠元模，有以下结果，确定它们在伪同构内：

#### 定理 5 {#ac-vii-s4-thm-5 .statement tag=053O}

令 T 为有限生成的挠元 A-模。存在两个有限族$(n_i)_{i \in I}$和$(p_i)_{j \in I}$，其中$n_i$是整数$\geq 1$，$p_i$是高度为1的$A$的素理想，这样，如果我们写成$T' = \bigoplus_{i \in I} A/p_i^{n_i}$，则存在$T$的伪同构$T'$。此外，带有性质的$(n_i)_{i \in I}$和$(p_i)_{i \in I}$在索引集合的双射和$T$的$p_i$包含湮没子内是唯一的。

唯一性：如果：$T \to T'$是伪同构，$p \in P, f_p : T, \to T'_p$是同构。现在，$T'_p$是$A_p/p^{n_i}A_p$的直和，和超过指标$i$，使得$p_i = p$；因此，$p^{n_i}A_p$是挠元$A$模块$T$的*基本除子*，(*代数*，章VII, § 4, no. 7)；他们的唯一性已在*代数*、章VII, § 4, no. 7、命题7中得到证明。

存在性：我们可以将注意力集中在$T \neq 0$的情况。令 $a$ 为 $T$、$p_i$ ($1 \leq i \leq k$) 的湮没子（非零且与$A$不同），$A$的高度为 1 包含 $a$（在数内有限） （$§ 1$、no. 6、定理 4））和$S = \bigcap_i (A - p_i)$。半局部环$A' = S^{-1}A$是主理想整环（引理2）并且具有极大理想$m_i = p_iA'$；由于 $S^{-1}T$ 是有限生成的挠元 $A$ 模块，因此它与有限直和 $\bigoplus_{j \in I} A'/m_{\phi(j)}^{n_j}$ 同构的，其中 $\phi$ 是有限集合 $I$ 到 $[1, k]$ 的映射 （*代数*、章VII, § 4, no. 7、命题7）；由于 $A'/m_{\phi(j)}^{n_j}$ 与 $S^{-1}(A/p_{\phi(j)}^{n_j})$ (章 II, § 2, no. 4) 同构的，我们获得了所需型的挠元 $A$-模块$T'$ 和同构 $f_0$ $S^{-1}T$ 到$S^{-1}T'$。由于$\operatorname{Hom}_{S^{-1}A}(S^{-1}T, S^{-1}T')$等于$S^{-1} \operatorname{Hom}_A(T, T')$（章11，§ 2, no. 7，命题19），因此存在$s \in S$和同态$f : T \to T'$使得$f_0 = s^{-1}f$。仍有待证明$f$是伪同构：现在，如果$p = 0$或$p \in P$与$p_i$、$T_p = T'_p = 0$不同（章II, § 4, no. 4、命题17）；相反，如果$p$是$p_i$（$1 \leq i \leq k$）之一，$s$在$A_p$中是可逆的，并且，由于$f_{p_i} = s(f_0)_{p_i}$和$(f_0)_{p_i}$是$T_{p_i} = (S^{-1}T)_{m_i}$到$T'_{p_i} = (S^{-1}T')_{m_i}$的同构，所以也是$f_{p_i}$。

#### 注 (2) {#ac-vii-s4-n4-rem-2 .statement tag=053P}

在定理 5 中的叙述中，模 $A/p_i^{n_i}$ 可以替换为 $A/p_i^{(n_i)}$（$§ 1$、no. 4、命题 8）。对于所有 $p \in P$，典范映射 $g : A/p^n \to A/p^{(n)} = A/(A \cap p^nA_p)$ 是伪同构，就像对于所有与 $p$、$A_q/p^nA_q = A_q/p^{(n)}A_q = 0$ 和 $A_p/p^nA_p = A_p/p^{(n)}A_p$ 不同的 $q \in P$ 而言。

\* 给定$A$模块的正合序列，$E \to F \to G$，如果$E$和$G$是伪零，$F$也是伪零，如下从定义2和章II, §2, no. 4，定理1。在语言中的类别，我们可以说，在 $A$ 模块的类别 $\mathscr{C}$ 中，伪零模的子类别 $\mathscr{C}'$ 是*满*，然后我们可以定义的*商*类别 $\mathscr{C}/\mathscr{C}'$：该类别中的对象也是 $A$ 模块但从$E$到$F$的态射集合（对于$\mathscr{C}/\mathscr{C}'$中的$E, F$）是可交换的群$\mathrm{Hom}_A(E', F')$的集合直极限，其中$E'$ （分别为$F'$）穿过$E$的子模的集合（分别为商模的集合、$F$的$F/F''$），使得$E/E'$（分别为$F''$）是伪零。当然，对于$A$模块$E, F$的每一个有序对，都有典范同态$\mathrm{Hom}_{\mathscr{E}}(E, F) \to \mathrm{Hom}_{\mathscr{E}/\mathscr{E}'}(E, F)$。说同态$u \in \mathrm{Hom}_A(E, F)$是伪零（分别是伪内射、伪满射、伪双射）意味着它在$\mathrm{Hom}_{\mathscr{E}/\mathscr{E}'}(E, F)$中的典范像是零（分别是单同态、泛同态、同构）。 \*

### 5.除子附加到挠元模

我们保留与第 1 条中相同的记号和假设。 2、3和4。回想一下，$D(A)$（或简称为$D$）表示$A$的*除子群*，相加写成：我们知道（§ 1, no. 3，定理2）$D$是免费的$\mathbf{Z}$-由$P$的元素生成的模块。

令 $T$ 为有限生成的挠元 $A$ 模块。对于所有$p \in P$，$T_p$是有限生成的挠元$A_p$模块，因此模为*有限长度*（章IV, § 2, no. 5，推论2到命题7）；我们用$l_p(T)$来表示这个长度。现在$T_p = 0$对于所有$p$而不是包含湮没子或$T$，因此对于几乎所有$p$（§ 1, no. 6，定理4），这证明了以下定义：

#### 定义 4 {#ac-vii-s4-def-4 .statement tag=053Q}

*如果$T$是有限生成的挠元$A$-模块，除子：*

$$
\chi(T) = \sum_{p \in P} l_p(T) \cdot p.
$$

*称为$T$*的内容。

#### 命题 10 {#ac-vii-s4-prop-10 .statement tag=053R}

(i) *令$0 \to T_1 \to T_2 \to T_3 \to 0$为有限生成的挠元$A$模块的正合序列。然后*

$$
\chi(T_2) = \chi(T_1) + \chi(T_3).
$$

(ii) *如果存在伪同构$f : T_1 \to T_2$，则$\chi(T_1) = \chi(T_2)$。*

(iii) *在阶和$\chi(T) = 0$中，$T$为伪零是必要且充分的。*

鉴于定义 4，对于挠元模，考虑$l_p$中的每个$p \in P$值就足够了。 性质 (i) 然后从章 II, § 2, no. 4、定理 1 以及长度在正合序列中的可加性得出 (*代数* 章 11, § 1, no. 10, 命题 16) 以及属性 (ii) 和 (iii) 紧随no. 4 中的定义。

#### 推论{#ac-vii-s4-n5-cor-1 .statement tag=053S}

*令 $0 \to T_n \to T_{n-1} \to \ldots \to T_0 \to 0$ 为有限生成的挠元 $A$ 模块中的正合序列。然后*$\sum_{i=0}^n (-1)^i \chi(T_i) = 0$。

鉴于章 II, § 2, no. 4、定理 1，这再次从 $l_p$ 的类似性质得出（*代数*、章 II, § 1, no. 10，推论 3 至命题 16）。

回想一下(章II, § 5, no. 4)，我们可以谈论有限生成A-模**类*集合*$F(A)$相对于同构的关系；对于每个有限生成A-模 M，令 $\mathrm{cl}(M)$ 表示 $F(A)$ 的相应的元素；我们用有限生成的挠元A-模的$F(A)$由……组成、类的$T(A)$子集来表示。显然，$T(A)$到$D(A)$的$\chi$定义映射，也用$\chi$表示，使得$\chi(\mathrm{cl}(T)) = \chi(T)$。

#### 命题 11 {#ac-vii-s4-prop-11 .statement tag=053T}

*设 G 是可加写的交换律群和 $\phi : T(A) \to G$ 映射；对于每个有限生成的挠元 A-模 T，我们还滥用语言写出 $\phi(T) = \phi(\mathrm{cl}(T))$。假设满足以下条件：
(1) *如果* $0 \to T_1 \to T_2 \to T_3 \to 0$ *是有限生成的挠元 A-模中的正合序列，则* $\phi(T_2) = \phi(T_1) + \phi(T_3)$。
(2) *如果* T *是伪零，则* $\phi(T) = 0$。
*那么存在唯一同态* $\theta : D(A) \to G$ *使得* $\phi = \theta \circ \chi$。*

由于$\chi(A/p) = p$对于所有p，必然对于所有$p \in P$来说$\theta(p) = \phi(A/p)$，这证明了$\theta$的唯一性，因为P形式的元素$D(A)$的基。相反，让$\theta$是从$D(A)$到G的同态，这样对于所有$p \in P$都有$\theta(p) = \phi(A/p)$，并让我们证明它可以解决问题。为此，我们写

$$
\psi(T) = \phi(T) - \theta(\chi(T))
$$

对于每个有限生成的挠元 A-模 T；显然，如果将$\phi$替换为$\psi$，则条件（1）和（2）也满足。另一方面，如果$p \in P$，则$\psi(A/p) = 0$；如果 p 是素理想 $\neq 0$ 并且不在 P 中，则 $A/p$ 的湮没子不包含在 P 的任何理想中，因此 (no. 4, 定理 5) $A/p$ 是伪零，因此 $\psi(A/p) = 0$。既然如此，每个有限生成的挠元A-模T承认分解级数，其因子同构于形式$A/p$的A-模，其中$p \in \mathrm{Supp}(T)$ （章 IV, § 1, no. 4、定理 1 和 2），因此为 $p \neq 0$，因为 T 为挠元模。通过分解级数的长度上的归纳，我们推论（鉴于$\psi$的性质（1））$\psi(T) = 0$。

\* 我们可以像no. 4一样，考虑有限生成的挠元A-模的类别$\mathscr{T}$的商类别$\mathscr{T}/\mathscr{T}'$与有限生成的伪零挠元A-模的完整子类别$\mathscr{T}'$。在阿贝尔的类别的语言中，命题11则表示阿贝尔的类别$\mathscr{T}/\mathscr{T}'$的*格罗滕迪克群*与$D(A)$自然同构。 \*

#### 命题 12 {#ac-vii-s4-prop-12 .statement tag=053U}

*如果a是A的理想$\neq 0$，

$$
\chi(A/a) = \chi((A : a)/A) = \mathrm{div}\, a.
$$

让$p \in P$。然后$aA_p = p^{n_p}A_p$，其中$n_p \geq 0$，因为$A_p$是离散估值环。 *如* $(A/a)_p = A_p/aA_p,\ l_p(A/a) = n_p$、从而 $\chi(A/a) = \sum_{p \in P} n_p p = \mathrm{div}\, a$（§ 1, no. 4、命题 7）。

另一方面，$(A : a) = A ; aA_p = p^{-n_p}A_p$，因此$l_p((A : a)/A) = n_p$，我们以同样的方式结论。

### 6. 两个格的相对不变量

我们保留记号和 no 的假设。 2 到 5. 设 V 为 $K$ 上有限秩 $n$ 的向量空间，M 为关于 A 的 V 格子。设 W 为外部幂 $\bigwedge^n V$，即 *秩的向量空间 1* 在 $K$ 上，令 $M_w$ 表示在典范映射 $V^n \to \bigwedge^n V$ 下由 $M^n$ 的像生成的 W 晶格 (no. 1, 命题 3 (iii); 注，$M_w$ 不一定同构于$\bigwedge^n M$（*代数*、章III, § 5、习题9））。如果$e$是W除以K的基，我们可以写成$M = a.e$，其中a是A的分数理想$\neq 0$。

令$M'$为V的另一个晶格，并记为$M'_w = a'.e$，其中$a'$是A的分数理想$\neq 0$； 除子 $\operatorname{div}(a) - \operatorname{div}(a')$ *不依赖于当基改变时，W、a和$a'$的基* $e$的选择乘以$K^*$的相同元素；我们将写成$\chi(M, M') = \operatorname{div}(a) - \operatorname{div}(a')$，并说这个除子是$M'$*相对于*M的*相对不变量*。显然，如果M、$M', M''$是V的三个格子，那么：

(3)
$$
\chi(M, M') + \chi(M', M'') + \chi(M'', M) = 0
$$
(4)
$$
\chi(M, M') + \chi(M', M) = 0.
$$

对于所有$p \in P$，它紧随定义而来的是$(M_w)_p = (M_p)_w$；此外，由于 M 是*自由* A，-模，因为 A 是 M 的主理想整环、基，在 A 上，是 K 上的 V 的基，因此 $(M_p)_w = \bigwedge^n (M_p)$ (章 II, § 2, no. 8)，分数理想 $a_p = aA_p$ 是主理想整环。如果我们集合$a_p = p^{n_p}A_p$，$a' = p^{n'_p}A_p$，那么：
$$
\chi(M, M') = \sum_{p \in P} (n_p - n'_p).p,
$$
也可以写成：
(5)
$$
\chi(M, M') = \sum_{p \in P} \chi(M_p, M'_p)
$$
将$D(A_p)$与$p$生成的$D(A)$的子Z模块进行识别。

#### 命题 13 {#ac-vii-s4-prop-13 .statement tag=053V}

*设 M 为 V 的格子，u 为 V 的 K-自同构。然后*：
(6)
$$
-\chi(M, u(M)) = \operatorname{div}(\det(u)).
$$
对于所有$p \in P$，则$\bigwedge^n (u(M)_p) = \bigwedge^n (u(M_p))$；如果 $(e_i)_{1 \leq i \leq n}$ 是 $M_p$ 中的基，则
$$
\bigwedge^n (M_p) = A_p \cdot e_1 \text{ } A \text{ } e_2 \text{ } A \ldots A \text{ } e_n,
$$

和$\bigwedge^n (u(M_p)) = A_p \cdot \det(u) e_1 \wedge e_2 \mathbf{A} \ldots \mathbf{A} e_n$，从而命题凭借公式（5）。

#### 命题 14 {#ac-vii-s4-prop-14 .statement tag=053W}

*如果 M, M' 是 V 的两个格子，使得 M' \子集 M, M/M' 是有限生成的挠元 A-模并且：*

$$
\chi(M, M') = -\chi(M/M').
$$

显然 M/M' \子集 V/M' 是有限生成的挠元模；另一方面，对于所有$p \in P$，我们知道（*代数*，章VII, § 4, no. 2，定理1）存在M的基$(e_i)_{1 \leq i \leq n}$，以及$M'_p$的$(e'_i)_{1 \leq i \leq n}$，使得$e'_i = \pi^{v_i} e_i$对于$1 \leq i \leq n$和整数$v_i \geq 0$，$\pi$是$A_p$的均匀化器。因此（上面介绍的记号）$n'_p - n_p = \sum_{i=1}^n v_i$；另一方面，

$$(M/M')_p = M_p/M'_p$$与挠元A,-模$\bigoplus_{i=1}^n A_p/p^{v_i} A_p$同构的，因此其长度为$\sum_{i=1}^n v_i$，根据(5)和no. 5的定义 4证明命题。

#### 推论 {#ac-vii-s4-n6-cor-1 .statement tag=053X}

*设L_1，L_2为两个自由A-模且相同的秩n，并令f: L_1\to L_2为同态。令 U 相对于 L_1 和 L_2 的基偏离矩阵。对于 Coker(f) 挠元 A-模，满足 \det(U) \neq 0 是必要且充分的，然后：*

$$
\chi(\operatorname{Coker}(f)) = \operatorname{div}(\det(U)).
$$

L_1和L_2可以分别视为$V_1 = L_1 \otimes_A K$和$V_2 = L_2 \otimes_A K$中的格，f扩展到K-同态$f_{(K)}: V_1 \to V_2$。然后

$$(\operatorname{Coker}(f))_{(K)} = \operatorname{Coker}(f_{(K)})$$

说$\operatorname{Coker}(f)$是挠元A-模意味着$\operatorname{Coker}(f_{(K)}) = 0$；现在，说 $f_{(K)}$ 是满射或者 $\det(U) \neq 0$、从而第一个断言等价相同。另一方面，我们可以写成$f(L_1) = u(L_2)$，其中$u$是行列式$\det(U)$的$L_2$的自同态；作为

$$\operatorname{Coker}(f) = L_2/u(L_2),$$

公式 (8) 由 (7) 和 (6) 得出。

#### 例 {#ac-vii-s4-n6-exa-1 .statement tag=053Y}

如果 $A = \mathbf{Z}$，$A$ 的除子群等同于有理数数 > 0 的乘法群 $\mathbf{Q}_+^*$。对于每个有限交换群 T，$\chi(T)$ 是 T 的 *阶*；上述推论表明，群$\operatorname{Coker}(f)$的阶等于$\det(U)$的*绝对值*（cf.*代数*，章VII, § 4, no. 7，推论3到定理 3）。

### 7. 除子类附加到有限生成模

我们保留记号和 no 的假设。 2 到 6. 回想一下，C(A)（或简称为 C）表示 $A$ 的除子类群，$D(A)$ 与本金除子的子群的商。对于每个除子$d \in D$，我们将用$c(d)$表示其C中的类。

#### 命题 15 {#ac-vii-s4-prop-15 .statement tag=053Z}

*设M为有限生成A-模。存在 M 的自由子模 L，使得 M/L 为挠元模并且 C 的元素 $c(\chi(M/L))$ 不依赖于所选择的自由子模 L。*

我们写 $S = A - \{0\}$ 并令 $V = S^{-1}M = M \otimes_A K$；如果$n$在K上是V的秩，则在V形式基中存在典范像的M的$n$元素$e_i$($1 \leq i \leq n$) V；这些元素显然在M中线性无关，因此生成是M的一个自由子模L，使得$S^{-1}(M/L) = S^{-1}M/S^{-1}L = 0$，因此M/L是挠元模。

现在让L，秩$n$M的另一个自由子模。由于$S^{-1}L = S^{-1}L_1$，存在$s \in S$使得$sL_1 \subset L$；因此，我们可以将极限自己推导为证明，如果$L_1 \subset L_2$是秩$n$中M的两个自由的子模，那么

$$
c(\chi(M/L_1)) = c(\chi(M/L_2)).
$$

现在，$\chi(M/L_1) = \chi(M/L_2) + \chi(L_2/L_1)$，从no. 6得出，推论到命题14，$\chi(L_2/L_1)$是本金除子，因此

$$
c(\chi(L_2/L_1)) = 0.
$$

以下将元素$c(\chi(M/L))$记为$-c(M)$；我们可以说 $c(M)$ 是除子类附加到 M 上。

#### 命题 16 {#ac-vii-s4-prop-16 .statement tag=0540}

(i) *令 $0 \to M_1 \xrightarrow{\alpha} M_2 \xrightarrow{g} M_3 \to 0$ 为正合序列 / 有限生成A-模。然后*

$$
c(M_2) = c(M_1) + c(M_3).
$$

(ii) *如果从M_1到M_2存在伪同构，则$c(M_1) = c(M_2)$。

(iii) *如果 T 为挠元模，则$c(T) = -c(\chi(T))$。

(iv) *如果 $a \neq 0$ 是 K 的分数理想，则*

$$
c(a) = c(\operatorname{div}(a)).
$$

(v) *如果 L 是自由A-模，则 $c(L) = 0$。

为了证明 (i)，考虑 M 的自由子模块 $L_1$（分别为 $L_3$）（分别为 $M_3$），使得 $M_1/L_1$（分别为 $M_3/L_3$）为挠元模。由于 $L_3$ 是自由的，$g$ 是满射的，$g^{-1}(L_3)$ 中存在 $\operatorname{Ker}(g)$ 的自由补集 $L_{23}$，它与 $L_3$ 同构的 (*代数*, 章 II, § 1, no. 11, 命题 21）；但是 $\operatorname{Ker}(g) = f(M_1)$ 包含 $f(L_1) = L_{12}$ 是自由的，因为 $f$ 是单射的。 和 $L_2 = L_{12} + L_{23}$ 是直接的，因此 $L_2$ 是 $M$ 的*免费* 子模。此外还有交换律图表：

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L_1 & \longrightarrow & L_2 & \longrightarrow & L_3 & \longrightarrow & 0 \\
0 & \longrightarrow & M_1 & \xrightarrow{f} & M_2 & \xrightarrow{g} & M_3 & \longrightarrow & 0
\end{array}
$$

其中行是精确的，垂直箭头是单射。因此，我们从蛇中得到图表 (章 I, § 1, no. 4, 命题 2) 正合序列：

$$
0 \to M_1/L_1 \to M_2/L_2 \to M_3/L_3 \to 0.
$$

由于$M_1/L_1$和$M_3/L_3$是挠元模，因此正合序列首先表明$M_2/L_2$也是如此，然后，凭借no. 5的命题10，可以得出：

$$
\chi(M_2/L_2) = \chi(M_1/L_1) + \chi(M_3/L_3)
$$

这就证明了(i)。

断言 (iii) 和 (v) 从定义显而易见。我们证明(ii)。因此，令$f : M_1 \to M_2$为伪同构，并令$L_1$为$M_1$的自由子模，使得$M_1/L_1$为挠元模。我们集合$L_2 = f(L_1)$；由于$\mathrm{Ker}(f)$是伪零，所以它是挠元模，因此$\mathrm{Ker}(f) \cap L_1 = 0$，因此$L_2$是免费的。设 $\tilde{f} : M_1/L_1 \to M_2/L_2$ 为同态，由 $f$ 取商得出； $\mathrm{Ker}(\tilde{f})$ 与 $\mathrm{Ker}(f)$ 同构的，$\mathrm{Coker}(\tilde{f})$ 与 $\mathrm{Coker}(f)$ 同构的，因此 $\tilde{f}$ 是伪同构；而且

$$
\mathrm{Coker}(\tilde{f}) = M_2/f(M_1)
$$

是挠元模，$f(M_1)/L_2 = \tilde{f}(M_1/L_1)$也是，因此$M_2/L_2$是挠元模，并且从no. 5，命题10 (ii)

$$
\chi(M_1/L_1) = \chi(M_2/L_2).
$$

最后剩下证明(iv)。令$x \in K^*$ 使得$a \subset xA$。通过考虑正合序列 $0 \to a \to xA \to xA/a \to 0$，我们得到

$$
c(a) = c(xA) - c(xA/a) = -c(xA/a)
$$

通过(i)和(v)。但$xA/a$同构于$A/x^{-1}a$、从而，由于 (iii)，

$$
c(xA/a) = -c(\chi(A/x^{-1}a)) = -c(\mathrm{div}(x^{-1}a)) = -c(\mathrm{div}(a))
$$

（no. 5，命题12）。这样就完成了证明。

当$M$是$V$相对于$A$、$\chi(M/L) = -\chi(M, L)$（no. 6、命题14）的*格子*时；设$(e_i)_{1 \leq i \leq n}$为$L$、$e = e_1 \wedge e_2 \wedge \ldots \wedge e_n$中的基，并且

$M_w = a \cdot e$（记号 / no. 6）；然后$\chi(M, L) = \operatorname{div}(a)$，从而$c(M) = c(\operatorname{div}(a))$，它概括了命题 16 (v)。

#### 推论 1 {#ac-vii-s4-prop-16-cor-1 .statement tag=0541}

*设* $0 \to M, \xrightarrow{u} M_{n-1} \to \cdots \to M_0 \to 0$ *为正合序列 of 有限生成A-模。*则

$$
\sum_{i=0}^n (-1)^i c(M_i) = 0.
$$

我们通过归纳对$n$进行论证，情况$n = 2$为命题16(i)。如果$M'_{n-1} = \operatorname{Coker}(u)$，则有两个正合序列：

$$
\begin{align*}
0 &\to M, \to M_{n-1} \to M'_{n-1} \to 0 \\
0 &\to M'_{n-1} \to M_{n-2} \to \cdots \to M_0 \to 0.
\end{align*}
$$

第一个表明 $M'_{n-1}$ 是有限生成的，并且归纳假设给出

$$
(-1)^{n-1} c(M'_{n-1}) + \sum_{t=0}^{n-a} (-1)^t c(M_t) = 0
$$

和

$$
c(M'_{n-1}) = c(M_{n-1}) - c(M_n),
$$

从而推论。

正合序列

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to E \to 0
$$

其中 $L_i$ ($0 \leq i \leq n$) 是*有限生成的自由* A-模，称为 A-模 E 的*有限自由分辨率*。

#### 推论 2 {#ac-vii-s4-prop-16-cor-2 .statement tag=0542}

*如果除数分数理想* $a \neq 0$ *of* $\mathbf{A}$ *承认有限自由分辨率，则它是主要的。*

事实上，我们将推论 1 应用于 $a$ 的有限自由分辨率：

$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to a \to 0.
$$

凭借命题 16 (v)、$c(a) = 0$，因此，凭借命题 16 (iv)，$\operatorname{div}(a)$ 是主要的；由于 $a$ 被假定为除数，因此它是本金 (§ 1, no. 1)。

#### 推论 3 {#ac-vii-s4-prop-16-cor-3 .statement tag=0543}

*如果* $\mathbf{A}$ *的每个除数理想* $\neq 0$ *都承认有限自由分辨率，* $\mathbf{A}$ *是阶乘。*

这是推论2的直接的推论和§ 3, no. 1、定义1。

\* 稍后我们将看到，正则局部环满足推论 3 的假设，因此是*阶乘。* \*

如果M是有限生成A-模，我们将用$r(M)$表示它的*秩*（回想一下，它是$M_{(K)} = M \otimes_A K$的K上的秩）；如果$0 \to M_1 \to M_2 \to M_3 \to 0$是有限生成A-模中的正合序列，则序列

$$
0 \to (M_1)_{(K)} \to (M_2)_{(K)} \to (M_3)_{(K)} \to 0
$$

也是精确的，因此$r(M_2) = r(M_1) + r(M_3)$。我们写

$$
\gamma(M) = (r(M), c(M)) \in \mathbf{Z} \times C(A);
$$

因此，$\gamma$满足命题16的性质(i)，并且如果M是伪零，$\gamma(M) = 0$（因为M是挠元模）。从$F(A)$到$\mathbf{Z} \times C(A)$存在唯一映射，也用y表示，这样对于每个有限生成A-模M都有$\gamma(M) = \gamma(\mathrm{cl}(M))$。我们将看到上述属性本质上表征了y：

#### 命题 17 {#ac-vii-s4-prop-17 .statement tag=0544}

设 G 是 *加法* 写成的交换性群和从 *有限* 生成的 A-模的类集合 $F(A)$ 到 G 的$\phi$ *映射*；对于*每个有限*生成的A-模M，我们还通过滥用语言写出$\phi(M) = \phi(\mathrm{cl}(M))$。 *假设*以下条件*满足*：
  (1) *如果* $0 \to M_1 \to M_2 \to M_3 \to 0$ 是正合序列 *有限*生成的A-模，则$\phi(M_2) = \phi(M_1) + \phi(M_3)$。
  (2) *如果* T 是伪零，则 $\phi(T) = 0$。
*那么*存在唯一同态$\theta : Z \times C \to G$使得$\phi = 8 \circ y$。

凭借命题 16 (iv)，对于某些合适的有限生成A-模 M，$Z \times C$的每个元素都是形式$(r(M), c(M))$； 从而唯一性共$\theta$。我们从no. 5到限制的应用命题11到$-\phi$到$T(A)$：那么存在同态$\theta_0 : D \to G$使得

$$
-\phi(T) = \theta_0(\chi(T))
$$

对于每个有限生成的挠元 A-模 T。令 x 为 A 的非零元素； 应用性质 (1) 至正合序列：

$$
0 \longrightarrow A \xrightarrow{h_x} A \longrightarrow A/xA \longrightarrow 0
$$

其中$h_x$是x乘以乘法，我们得到$\phi(A/xA) = 0$，从而$\theta_0(\mathrm{div}(x)) = 0$。对每个挠元 A-模 T 取商，$\theta_0$ 因此定义同态 $\theta_1 : C \to G$ 和 $\phi(T) = \theta_1(c(T))$。我们现在证明，由 $\theta(n, z) = n.\phi(A) + \theta_1(z)$ 定义的同态 $\theta$ 可以求解问题。为此，我们为每有限生成A-模 M 写 $\phi'(M) = \phi(M) - \theta(\gamma(M))$；显然，如果将$\phi$替换为$\phi'$，条件(1)仍然满足。此外，当M为挠元模或自由模时，$\phi'(M) = 0$；但对于每一个有限生成A-模 M，都存在 M 的一个自由子模 L，使得 M/L 为挠元模 (命题 15)，性质 (1) 表明对于每有限生成A-模 M 都有 $\phi'(M) = 0$。

\* 在阿贝尔的类别的语言中，命题17表明$\mathbf{Z} \times C(A)$与商类别$\mathscr{F}/\mathscr{F}'$的格罗滕迪克群规范同构，其中$\mathscr{F}$是有限生成A-模的类别，$\mathscr{F}'$是有限生成A-模的完整子类别伪零模的$\mathscr{F}$由……组成。 \*

### 8. 与标量环的有限扩张相关的性质

在此式中，A和B表示两个整体闭的诺特域，使得$A \subset B$和B分别为A和B的分数的有限生成A-模和K和L域。对于A-模，我们将分别写为div$_A$、$\chi_A$、$c_A$、$\gamma_A$、$r_A$，而不是div、$\chi$、c、y、r，并使用类似的记号来表示B-模。

我们知道(§ 1, no. 10)，对于B的素理想$\mathfrak{p}$的高度为1，$\mathfrak{p} = \mathfrak{P} \cap A$的高度为1是充分必要的；此外（前述，命题 14）对于$\mathfrak{p} \in P(A)$，只有有限的数素理想$\mathfrak{P} \in P(B)$位于$\mathfrak{p}$之上。简而言之，我们将用$\mathfrak{P}|_{\mathfrak{p}}$关系表示““$\mathfrak{P}$位于$\mathfrak{p}$之上”（即$\mathfrak{p} = \mathfrak{P} \cap A$）；然后我们将用$e_{\mathfrak{P}/\mathfrak{p}}$或$e(\mathfrak{P}/\mathfrak{p})$表示指标$e(v_{\mathfrak{P}}/v_{\mathfrak{p}})$的分支估值 $v_{\mathfrak{P}}$ 高于估值 $v_{\mathfrak{p}}$ (章 VI, § 8, no. 1) 以及 $f_{\mathfrak{P}/\mathfrak{p}}$ 或 $f(\mathfrak{P}/\mathfrak{p})$ 剩余类类次数 $f(v_{\mathfrak{P}}/v_{\mathfrak{p}})$（前述离散估值）； $v_{\mathfrak{p}}$和$v_{\mathfrak{P}}$被规范，$f_{\mathfrak{P}/\mathfrak{p}}$是$B/\mathfrak{P}$分数域次数超过$A/\mathfrak{p}$分数域。 集合 $n = r_A(B)$，其中 B 被视为 A-模；因此，定义 $n = [L:K]$，并且对于所有 $\mathfrak{p} \in P(A)$，$n$ 也是自由 A 的秩，对于所有 $\mathfrak{P}|_{\mathfrak{p}}$，则可以得出。 章 VI, § 8, no. 5、定理 2 对于所有 $\mathfrak{p} \in P(A)$：

$$
\sum_{\mathfrak{P}|_{\mathfrak{p}}} e_{\mathfrak{P}/\mathfrak{p}} f_{\mathfrak{P}/\mathfrak{p}} = n.
$$

正是如此，由于$D(A)$和$D(B)$是免费的$\mathbf{Z}$模块，我们对定义递增同态订购群$N : D(B) \to D(A)$（也表示为$N_{B/A}$）， 条件：

$$
N(\mathfrak{P}) = f_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{p} \quad \text{for} \quad \mathfrak{P} \in P(B), \quad \text{where} \quad \mathfrak{p} = \mathfrak{P} \cap A.
$$

另一方面（§ 1, no. 10，命题 14）我们定义了有序群$i : D(A) \to D(B)$（也用$i_{B/A}$表示）的递增同态，通过条件：

$$
i(p) = \sum_{\mathfrak{P}|_p} e_{\mathfrak{P}/\mathfrak{p}} \cdot \mathfrak{P} \quad \text{for} \quad p \in P(A).
$$

显然，对于 A（或 B）的除子的每个家庭 $(d_i)$（或 $(d'_i)$）：

$$
N(\sup(d'_i)) = \sup(N(d'_i)), \qquad N(\inf(d'_i)) = \inf(N(d'_i))
$$
$$
i(\sup(d_i)) = \sup(i(d_i)), \qquad i(\inf(d_i)) = \inf(i(d_i)).
$$

公式 (9) 表明：

(14) $$ N \circ i = n . 1_{D(A)} $$

对于所有 $a \in A$（§ 1, no. 10、命题 14）：

(15) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(a). $$

我们推论（通过（13）），对于$A$的每个分数理想$a$，也：

(16) $$ i(\operatorname{div}_A(a)) = \operatorname{div}_B(aB). $$

对于每个元素 $b \in B$，我们知道（章 V, § 1, no. 3，命题 11 的推论）$N_{L/K}(b) \in A$；此外（章VI, § 8, no. 5，公式（9））：

(17) $$ v_p(N_{L/K}(b)) = \sum_{\mathfrak{p}/p} f_{\mathfrak{p}/p} v_{\mathfrak{p}}(b) $$

从而：

(18) $$ N(\operatorname{div}_B(b)) = \operatorname{div}_A(N_{L/K}(b)). $$

公式 (15) 和 (18) 表明，通过取商，同态 $N$ 和 $i$ 定义同态，通过滥用语言，也可以表示为：

$$ N : C(B) \to C(A), \quad i : C(A) \to C(B). $$

注同态 $i : C(A) \to C(B)$ 不是一般的单射（§ 3，习题 7）。

回想一下，对于每个$B$-模块$R$，$R_{[A]}$表示通过将标量限制为$A$（代数，章11，§ 1, no. 13）从$R$获得的$A$模块。

#### 命题 18 {#ac-vii-s4-prop-18 .statement tag=0545}

(i) *为了使$R$成为伪零$B$模，$A$模$R_{[A]}$是伪零是必要且充分的。*

(ii) *要使$R$有限生成挠元$B$-模，$R_{[A]}$是有限生成的挠元$A$-模是必要且充分的，然后：*

(19) $$ \chi_A(R_{[A]}) = N(\chi_B(R)). $$

(iii) *为了使$R$是有限生成的$B$-模，$R_{[A]}$是有限生成的$A$-模是必要且充分的，然后：*

(20) $$ c_A(R_{[A]}) = N(c_B(R)) + r_B(R)c_A(B) $$
(21) $$ r_A(R_{[A]}) = n . r_B(R) \quad \text{(recall that } n = r_A(B)). $$

由于$B$是有限生成的$A$模，对于$R$是有限生成的$B$模，$R_{[A]}$是有限生成的$A$模是充分必要的。另外，如果$b$是$R$的湮没子，$b \cap A = a$就是$R_{[A]}$的湮没子；由于 $B$ 是 $A$ 的积分，除了 0 之外，没有任何理想值位于 $A$ 的理想 0 之上（章 V, § 2, no. 1，推出 1 到命题 1），因此说 $a \neq 0$ 或 $b \neq 0$ 是一样的。

(i) 凭借最后的注，我们可以将注意力集中在$R$是挠元$B$模的情况。如果$b$包含在素理想$\mathfrak{p} \in P(B)$中，则$a$包含在高度为1的$\mathfrak{p} \cap A = p$中。反之，如果$a$包含在素理想$p \in P(A)$中，则存在$B$的素理想$\mathfrak{p}$，其中包含 $b$ 且位于 $p$ 之上（章 V, § 2, no. 1，推论 2 至定理 1）。 断言 (i) 由注和no. 4、定义 2 得出。

(ii) 对于每个有限生成的挠元$B$-模块$R$，我们写

$$
\phi(R) = \chi_A(R_{[A]});
$$

显然（对于有限生成的挠元$B$模块）$\phi$满足no. 5的命题II的条件（1）和（2）（考虑到（i））。因此，对于每个有限生成的挠元$B$-模块$R$，存在同态$\theta : D(B) \to D(A)$，使得$\phi(R) = \theta(\chi_B(R))$。 同态 $\theta$ 由形式 $B/\mathfrak{p}$ 的每个 $B$ 模块的值确定，其中 $\mathfrak{p} \in P(B)$，自 $\chi_B(B/\mathfrak{p}) = \mathfrak{p}$ 起。现在，对于$P(A)$、$p \notin q$以及$(B/\mathfrak{p})_q = 0$中的每个素理想$q \neq p = \mathfrak{p} \cap A$。另一方面，如果我们集合$S = A - p$，$\mathfrak{p}.S^{-1}B$是$S^{-1}B$和$(B/\mathfrak{p})_p = S^{-1}B/\mathfrak{p}$的最大理想。 $S^{-1}B$同构于$B/\mathfrak{p}$分数域(章II, § 2, no. 5，命题11)，即$v_{\mathfrak{p}}$剩余类域；因此，作为 $A$ 模块，其长度为 $f_{\mathfrak{p}/p}$；这就证明了 $\theta = N$ (no. 5, 定义 4)。

(iii) 如果$T$是$R$中的挠元子模，则$T_{[A]}$是$R_{[A]}$和$(R/T)_{[A]} = R_{[A]}/T_{[A]}$中的挠元子模；因此，为了证明（21），我们可以将注意力集中在$R$无扭转的情况。 然后$R$被识别为$R_{(L)}$的子$B$模块和$L$上$R_{(L)}$的包含基$(e_i)_1 < < m$。 If $(b_j)_1 s < n$ is a basis of $L$ over $K$ consisting of elements of $B$, the $b_j e_i$ form a basis of $R_{(L)}$ over $K$ consisting of elements of $R$, whence (21). 另一方面，令$M$为$R$的自由子$B$模块，使得$R/M$为挠元$B$模块；因为 $M_{[A]}$ 是 $r_B(R)$ $A$ 的直和，与 $B$ 同构的，乘以命题 16 (i)

$$
c_A(M_{[A]}) = r_B(R).c_A(B).
$$

此外，根据(19)，$c_A((R/M)_{[A]}) = -c_A(N(\chi_B(R/M)))$；但对于所有 $d \in D(B)$ 定义同态 $N : C(B) \to C(A)$，$c_A(N(d)) = N(c_B(d))$，以及$c_B(\chi(R/M)) = -c_B(R)$ 定义，最后

$$
c_A((R/M)_{[A]}) = N(c_B(R));
$$

那么只需应用命题 16 (i) 即可得到 (20)。

#### 命题 19 {#ac-vii-s4-prop-19 .statement tag=0546}

让$R$*有限*生成$B$-模块。 *为了*$R$成为*自反*，$R_{[A]}$成为*自反*$A$模是必要*且充分的。

我们在命题 18 的证明中指出，要使R成为无扭转B-模，$R_{[A]}$是无扭转A模是充分必要的。因此，我们可以假设 R 是关于 B 的$W = R \otimes_B L$ 晶格。我们将使用以下引理：

#### 引理 4 {#ac-vii-s4-lem-4 .statement tag=0547}

*令W为有限秩在L上的向量空间，并令R为W相对于B的格子。那么，对于所有$p \in P(A)$，$(R_{[A]})_p = \bigcap_{\mathfrak{p}/p} R_{\mathfrak{p}}$。*

如果$S = A - p$，环$S^{-1}B$的素理想是由B不满足S的素理想生成的，在其他字中，理想$\mathfrak{P}_i$（$1 \leq i \leq m$）位于p和理想（0）之上；这表明$S^{-1}B$是一个半局部环，其最大理想是m，$= \mathfrak{P}_i(S^{-1}B)$对于$1 \leq i \leq m$；此外，局部环$(S^{-1}B)_{\mathfrak{P}_i}$同构于$B_{\mathfrak{p}_i}$（章11、§ 2, no. 5、命题11），因此是离散估值环。因此，环$S^{-1}B$是戴德金域（§ 2, no. 2，定理1（f）），并且由于它是半局部的，所以它是主理想整环（§ 2, no. 2，命题1）。既然如此，$(R_{[A]})_p$等于$S^{-1}R$，视为A,-模；由上可知，$S^{-1}R$是W相对于$S^{-1}B$的自由格，因此可以将no. 2的2个定理应用于它，给出$S^{-1}R = \bigcap_i (S^{-1}R)_{m_i}$：但是$(S^{-1}R)_{m_i} = R_{\mathfrak{p}_i}$，这证明了引理。

回到命题19的证明，到引理4，

$$
\bigcap_{\mathfrak{p} \in P(B)} R_{\mathfrak{p}} = \bigcap_{p \in P(A)} (R_{[A]})_p
$$

由no. 2、定理2得出结论。

#### 推论{#ac-vii-s4-n8-cor-1 .statement tag=0548}

*环 B 是反身A-模。*

#### 命题 20 {#ac-vii-s4-prop-20 .statement tag=0549}

(i) *要使有限生成A-模 M 为伪零，$M \otimes_A B$ 为伪零B-模是充分必要的。*
(ii) *如果 M 是有限生成的挠元 A-模，$M \otimes_A B$ 是有限生成的 B-模并且：*
(22)
$$
\chi_B(M \otimes_A B) = i(\chi_A(M)).
$$
(iii) *如果 M 为有限生成A-模，则 $M \otimes_A B$ 是有限生成的 B-模并且：*
(23)
$$
c_B(M \otimes_A B) = i(c_A(M))
$$
(24)
$$
r_B(M \otimes_A B) = r_A(M).
$$

(i) 设$\mathfrak{p}$为$B$、$\mathfrak{p} = \mathfrak{P} \cap A$的素理想；那么 $(M \otimes_A B)_{\mathfrak{p}} = M \otimes_A B_{\mathfrak{p}}$ (章 11, § 2, no. 7, 命题 18) ，另一方面
$$
M \otimes_A B_{\mathfrak{p}} = (M \otimes_A A_p) \otimes_{A_p} B_{\mathfrak{p}} = M_p \otimes_{A_p} B_{\mathfrak{p}};
$$
因此，关系$M_p = 0$等价于$(M \otimes_A B)_{\mathfrak{p}} = 0$（章II, § 4, no. 4，引理4）。将这个注应用于理想$\mathfrak{P} = (0)$和理想$\mathfrak{p} \in P(B)$就足以证明(i)，同时考虑到no. 4，定义2。

为了证明(ii)，我们将使用以下引理：

#### 引理 5 {#ac-vii-s4-lem-5 .statement tag=054A}

*令$M_1, M$为两个有限生成的$A$模块，以及$f : M_1 \to M_2$单同态。那么 $f \otimes 1 ; M_1 \otimes_A B \to M_2 \otimes_A B$ 的核就是伪零。*

令 $\mathfrak{p}$ 为高度为 $\leq 1$ 的 $A$ 的素理想。然后$(M_i \otimes_A B)_\mathfrak{p} = (M_i)_\mathfrak{p} \otimes_{A_\mathfrak{p}} B_\mathfrak{p}$（$i = 1, 2$）（章11，§ 2, no. 7，命题18）和$(f \otimes 1_B)_\mathfrak{p} = f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$； 假设 $f$ 是单射意味着 $f$ 也是单射，(章 II, § 2, no. 4, 定理 1)；另一方面，鉴于$\mathfrak{p}$的选择，$A_\mathfrak{p}$是主理想整环和$B_\mathfrak{p}$有限生成的无扭转$A_\mathfrak{p}$模，因此是*自由*；我们结论 $f_\mathfrak{p} \otimes 1_{B_\mathfrak{p}}$ 本身是单射的。如果$I = \mathrm{Ker}(f \otimes 1)$，则$I_\mathfrak{p} = \mathrm{Ker}((f \otimes 1)_\mathfrak{p})$（章11，§ 2, no. 4，定理1）；因此 $I_\mathfrak{p} = 0$, 从而 *更不必说* $I_\mathfrak{p} = (I_\mathfrak{p})_\mathfrak{p} = 0$ 对应 $\mathfrak{p}|p$，这就证明了引理 (no. 4, 定义 2)。

现在我们回到 (ii) 的证明。对于每个有限生成的挠元$A$-模块$M$，写$\phi(M) = \chi_B(M \otimes_A B)$；从 (i) 可以得出，如果 $M$ 是伪零，则 $\phi(M) = 0$。另一方面，考虑有限生成的挠元 $A$-模块中的正合序列 ：
$$
0 \to M_1 \to M_2 \to M_3 \to 0.
$$
从引理 4 可以得出，有正合序列个 $B$ 模块：
$$
0 \to I \to M_1 \otimes_A B \to M_2 \otimes_A B \to M_3 \otimes_A B \to 0
$$
其中 $I$ 是伪零。使用no. 5，推论命题 10，我们因此获得$\phi(M_2) = \phi(M_1) + \phi(M_3)$。因此，我们从 no. 5 的命题 11 中得出结论，存在同态 $\theta : D(A) \to D(B)$，这样对于每个有限生成的挠元 $A$-模块 $M$，都有 $\phi(M) = \theta(\chi_A(M))$。为了证明$\theta = i$，只要证明$\phi(A/p) = i(p)$对于所有$p \in P(A)$就足够了；现在$(A/p) \otimes_A B = B/pB$，对于所有$\mathfrak{p} \in P(B)$，$(B/pB)_{\mathfrak{p}} = B_{\mathfrak{p}}/pB_{\mathfrak{p}}$；如果 $\mathfrak{p}$ 不高于 $p$，则最后一个模为 0；如果相反$\mathfrak{p}|p$，则$B_{\mathfrak{p}}/pB_{\mathfrak{p}}$是长度$e(\mathfrak{p}/p)$除定义的指标分支的$B_{\mathfrak{p}}$模（章VI, § 8, no. 1）；因此$\chi_B(B/pB) = \sum_{\mathfrak{p}|p} e_{\mathfrak{p}/p} . 13 = i(p)$，它完成了(ii)的证明。

公式 (24) 为直接的，对于
$$
(M \otimes_A B) \otimes_B L = M \otimes_A L = (M \otimes_A K) \otimes_K L
$$

$(M \otimes_A K) \otimes_K L$超过$L$的秩等于$M \otimes_A K$超过$K$的秩。为了显示(23)，考虑$M$的自由子模$H$，使得$Q = M/H$是挠元$A$模。 应用引理 4 如上所述，我们得到$B$个模块中的正合序列：

$$
0 \to I \to H \otimes_A B \to M \otimes_A B \to Q \otimes_A B \to 0
$$

其中 $I$ 是伪零。因此，从 no. 7、命题 16(ii) 和 (v) 以及推论 1 到命题 16 可以得出：

$$
c_B(M \otimes_A B) = c_B(Q \otimes_A B) = -c_B(\chi_B(Q \otimes_A B)) = -c_B(i(\chi_A(Q)))
$$

凭借(ii)；但是通过同态$i : C(A) \to C(B)$中的定义，
$c_B(i(\chi_A(Q))) = i(c_A(\chi_A(Q))) = -i(c_A(M))$，完备的 (23) 的证明。

**注**
(1) 如果 $M$ 是自反 $A$ 模，则 $M \otimes_A B$ 不一定是自反 (习题 6)。然而，当 $B$ 是平面 $A$ 模（no. 2，命题 8）时，情况就是如此。
(2) 令$C$为第三个整体闭诺特域，使得$B \subset C$和$C$是有限生成的$B$模块（因此也是有限生成的$A$模块）。那么我们有传递性方程：

(25)
$$
N_{C/A} = N_{B/A} \circ N_{C/B},
$$
(26)
$$
i_{C/A} = i_{C/B} \circ i_{B/A}
$$

紧接着由指标和剩余类类次数 (章 VI, § 8, no. 1, 引理 1) 的传递性方程得出。

### 9. 减少定理

我们保留记号和 no 的假设。 2 至 7。

#### 引理 6 {#ac-vii-s4-lem-6 .statement tag=054B}

*令 $R$ 为交换环和 $p_i$ ($1 \leq i \leq n$) $R$ 不同的素理想。*

(i) *对于$1 \leq i \leq n$，令$H_i$为$R/p_i$满足的子集，以下条件：不存在元素$\alpha_i \in R/p_i$使得$\alpha_i + H_i$包含是理想的$\neq 0$ $R/p_i$。那么存在$a \in R$，对于$1 \leq i \leq n$，$R/p_i$中$a$的典范像不会属于到$H_i$。*

(ii) *如果 $\operatorname{Card}(H_i) < \operatorname{Card}(R/p_i)$，则 (i) 中的 $H_i$ 满足条件。*

(i) 我们通过归纳对$n$进行争论，$n = 0$的情况是微不足道的。因此令$n \geq 1$。我们可以在指标$i$上得到置换，并且可以假设$p_1$在$p_i$中是最小的，因此，对于$2 \leq i \leq n$，存在$c_i \in p_i$使得$c_i \notin p_1$。到归纳假设时，存在$b \in R$，使得$R/p_i$中的$b$的典范像不会对于$2 \leq i \leq n$来说属于到$H_i$。对于所有$x \in R$，我们写为$a_i = b + x c_2 c_3 \ldots c_n$；作为 $c_i \in p_i$，显然 $a_i \equiv b \pmod{p_i}$ 对应 $2 \leq i \leq n$。因此，只要证明存在$x \in \mathbf{R}$使得$\mathbf{R}/p_1$中$a_i$的典范像不存在属于到$H_1$即可。现在，$\mathbf{R}/p_1$中的$a_i$的典范像的集合（其中$x$穿过$\mathbf{R}$）只是$\beta + c$，其中$\beta$是$b$和$c$的典范像由$c_2 c_3 \ldots c_n$的典范像生成$\mathbf{R}/p_1$的理想；凭借$c_i$的选择，$c \neq 0$，因为$\mathbf{R}/p_1$是整环，并且$H_1$上的假设意味着存在解决问题的$x$。

(ii) 由于$\mathbf{R}/p_i$是整环，$\mathbf{R}/p_i$的每个理想$\neq 0$的基数都等于$\mathbf{R}/p_i$的基数，对于$\mathbf{R}/p_i$、从而的元素的任何理想平移也是如此。

#### 定理 6 {#ac-vii-s4-thm-6 .statement tag=054C}

*设 M 为无扭有限生成A-模。存在 M 的自由子模 L，使得 M/L 同构于 A 的理想。*

我们用$n$表示$M$的*秩*（$V = M \otimes_A K$在$K$上的秩），并将$M$视为$V$相对于$A$的格子。那么，对于所有$p \in P(A)$，$M_p$是$V$相对于$A_p$的格子（no. 1，*例6*），并且，如$A$，是主理想整环，$M$，是一个*自由* $A$-秩$n$的模数。我们将写：

$$
M(p) = M_p/pM_p.
$$

我们用$A/p$的分数的$k(p)$域来表示（与$A_p$的剩余类域同构）；因此，$M(p) = M \otimes_A k(p)$ 是秩 $n$ 中的向量空间与 $k(p)$ 之比。对于所有$x \in M$，我们将用$M(p)$中的$x$中的$x(p)$典范像来表示。

#### 引理 7 {#ac-vii-s4-lem-7 .statement tag=054D}

*令$x_i$ ($1 \leq i \leq m$) 与$M$ 线性无关元素（超过$A$ 或$K$，其结果相同），并令$L$ 为由$x_i$ 生成的$M$ 的子A 模。那么，对于几乎所有 $p \in P$，$x_i(p) \in M(p)$ 都与 $k(p)$ 线性无关；为了使它们在 $k(p)$ 上对于所有 $p \in P$ 线性独立，$M/L$ 无扭转是必要且充分的。*

令$x_1, \ldots, x_n$为$M$的元素，其中$x_1, \ldots, x_n$、形式基为$V$，并让$N$为由$x_i$生成的$M$的自由子A模块（$1 \leq i \leq n$）。从no. 3、定理 3 可以得出$N = M$，几乎所有$p \in P$；由于 $N(p)$ 的 $x_1(p), \ldots, x_n(p)$ 形式基超过 $k(p)$，这就建立了第一个断言。

如果 $M/L$ 是无扭转的，则对于所有 $p \in P$（no. 1，*例 6*），$(M/L)_p = M_p/L_p$ 也是无扭转的，并且，由于 $A_p$ 是主理想整环，$M_p/L_p$ 是自由的。因此$M$，是$L$的直和，以及秩$n - m$的免费$A$模​​块$E$；因此$M(p)$是$L(p)$的直和和向量$k(p)$空间$E/pE$秩$n - m$；因此 $L(p)$ 是秩 $m$，并且由于它是由 $x_i(p)$ ($1 \leq i \leq m$) 生成的，因此后者是线性无关的。

相反，假设对于所有 $p \in P$，$x_i(p)$ ($1 \leq i \leq m$) 与 $k(p)$ 线性无关。那么，对于所有 $p$（章 II, § 3, no. 2，推论 1 到命题 5），$L$ 是 $M$ 的直因子，因此对于所有 $p \in P$，$M_p/L_p = (M/L)_p$ 是无扭转的。我们结论通过章IV, § 1, no. 2得到$P \cap \operatorname{Ass}(M/L) = \varnothing$，推论到命题5。但是由于L是自反的，所以从no. 2，命题7（i）可以得出属于到的唯一素理想$\operatorname{Ass}(M/L)$ 是理想值（0）；因此 $M/L$ 是无扭转的。

#### 引理 8 {#ac-vii-s4-lem-8 .statement tag=054E}

*假设$M$中的秩$n$为$\geqslant 2$；则存在 $M$ 的元素 $x \neq 0$，使得 $M/Ax$ 无扭转。*

设$y \neq 0$为$M$的元素。通过引理 7，$p \in P$ 的集合 $Y$，使得 $y(p) = 0$ 是有限的。如果$Y = \varnothing$，则从引理 7 得出，应用于单个元素 $y$ 的序列 $(x_i)$ 由……组成，$M/Ay$ 是无扭转的。因此假设 $Y \# @$ 并写成 $S = \bigcap_{p \in Y} (A - p)$；我们知道（no. 4，引理 2）$S^{-1}A$是半局部主理想整环，其最大理想是$pS^{-1}A$，其中$p \in Y$，相应的局部环是$A_p$。因此
$$
S^{-1}A/pS^{-1}A = k(p),
$$
从而
$$
S^{-1}M/pS^{-1}M = (M/pM) \otimes_A S^{-1}A = M \otimes_A ((A/p) \otimes_A S^{-1}A) = M \otimes_A k(p) = M(p)
$$
对于所有$p \in Y$。到章II, § 1, no. 2、命题6，存在元素$z/s \in S^{-1}M$($z \in M, s \in S$)，其$p \in Y$的$M(p)$中的典范像都是$\neq 0$。通过 $S$ 的定义，因此所有 $p \in Y$ 为 $z(p) \neq 0$。我们可以进一步假设$y$和$z$在$K$上“线性独立”。在相反的情况下，考虑元素$t \in M$，它与$y$线性无关（从$n \geqslant 2$开始就存在）；另一方面，取元素$a \neq 0$属于到$\bigcap_{p \in Y} p$（由于$A$是整环，因此不会减少到0）并写出$z' = z + at$：显然$y$和$z'$在$K$上是线性独立的以及所有$p \in Y$的$z'(p) = z(p) \neq 0$。

因此，假设$y$和$z$在$K$上线性无关，令$Z$是$p \in P - Y$的集合，使得$y(p)$和$z(p)$在$k(p)$上线性无关；从引理 7 可以得出，这个集合是*有限的*。因此，对于所有$p \in Z$，我们可以在$\lambda(p) \in k(p)$处写出$z(p) = \lambda(p)y(p)$。现在，$\operatorname{Card}(A/p) > 2$适用于所有$p \in P$；因此，从引理 6 可以得出，存在$b \in A$，使得对于所有$p \in Z$，$A/p$中$b$的典范像不同于$\lambda(p)$。现在我们证明元素$x = z - by$可以解决问题；它足以（凭借引理 7 与 $m = 1$ 的应用）来验证$x(p) \neq 0$ 对于*所有* $p \in P$。现在：

— 如果$p \in Y$，则$x(p) \neq 0$乘以构造；
— 如果$p \in Z$，则$x(p) = \mu_p y(p)$，其中$\mu_p \neq 0$凭借$b$的选择，因此自$y(p) \# 0$以来$x(p) \neq 0$；
— 如果 $p \in P - (Y \cup Z)$、$y(p)$ 和 $z(p)$ 是线性独立的，因此$x(p) \neq 0$。

建立了这些引理后，我们转到定理的证明 6。我们通过归纳对$n$进行论证，$n \leq 1$的情况是微不足道的，因为$M$本身同构于$A$的理想。因此假设 $n \geq 2$；由于引理 8，存在秩 1 的$M$的自由子模$L_0$，使得$M/L_0$无扭转；因此，$M/L_0$ 是秩 $n - 1$。到归纳假设时，存在$M/L_0$的自由子模$L$，使得$(M/L_0)/L_1$同构于理想的$A$。令$L$为$M$中$L_1$的逆像； $L/L_0$与$L_1$同构的，并且由于$L_1$是自由的，$L$与$L_0 \oplus L_1$同构的（代数，章II, § 1, no. 11，命题21），因此是自由的；由于$M/L$与$(M/L_0)/L_1$同构的，定理已被证明。

#### 注 {#ac-vii-s4-n9-rem-1 .statement tag=054F}

如果 $M$ 是自反的，那么 $M/L$ (习题 9) 则不一定成立。

### 10. 模超过 DEDEKIND 域

我们现在假设$A$是一个戴德金域；那么我们知道理想 $p \in P$ 是最大的，并且它们是 $A$ 的唯一素理想 $\neq 0$ ($§ 2$, no. 1 )； 群$D(A)$与$A$的分数理想$\neq 0$的群$I(A)$进行识别。

#### 命题 21 {#ac-vii-s4-prop-21 .statement tag=054G}

令 $A$ 为 Dedekind 域。每个伪零$A$模都是零。每个伪内射（分别是伪满射、伪双射、伪零）$A$-模同态都是单射（分别是满射、双射的、零）。

第一个断言已显示（no. 4、例1）；其他人立即跟进。

#### 命题 22 {#ac-vii-s4-prop-22 .statement tag=054H}

令 $A$ 为 Dedekind 域，$M$ 为有限生成的 $A$ 模。以下属性是等效的：
(a) $M$ 无扭转。
(b) $M$ 是自反的。
(c) $M$ 是投影。

我们已经知道（在整环 $A$ 上没有假设），(b) 意味着 (a) (no. 2, 注 1) 并且 (c) 意味着 (b) (代数, 章 II, § 2, no. 7，推论 4 命题14)。如果$M$无扭转，则用$V = M \otimes_A K$相对于$A$的晶格来识别；因此，对于每个最大理想$p \in P$，$M$是一个免费的$A_p$模块，因为$A$是主理想整环。由章II, § 5, no. 2、定理1(b)得出结论。

#### 推论{#ac-vii-s4-n10-cor-1 .statement tag=054I}

令$M$为有限生成的$A$模块，并令$T$为其挠元子模。那么$T$是$M$的直接因子。

由于 $M/T$ 是无扭转且有限生成的，因此它通过命题 22 进行投影，因此推论来自代数、章 II, § 2, no. 2、命题 4。

#### 命题 23 {#ac-vii-s4-prop-23 .statement tag=054J}

令 $A$ 为 Dedekind 域，$T$ 为有限生成的挠元 $A$ 模。存在两个有限族$(n_i)_{i \in I}$和$(\mathfrak{p}_i)_{i \in I}$，其中$n_i$是整数$\geq 1$，$P$的$\mathfrak{p}_i$元素，使得$T$同构于直和 $\bigoplus_{i \in I} (A/\mathfrak{p}_i^{n_i})$。此外，族$(n_i)_{i \in I}$和$(\mathfrak{p}_i)_{i \in I}$在索引集合的双射内是唯一的。

这是从 no. 4、定理 5 得出的，考虑到这里存在伪同构同构。

#### 命题 24 {#ac-vii-s4-prop-24 .statement tag=054K}

令 $A$ 为 Dedekind 域，$M$ 为有限生成的无扭转 $A$ 模 & 秩 $n \geq 1$。那么存在$A$的理想$b \neq 0$，使得$M$同构于模$A^{n-1}$和$b$的直和。而且，理想$b$的类是由这个条件唯一确定的。

no. 9的定理 6表明存在$M$的自由子模$L$，使得$M/L$同构于$A$的理想$a$。如果$a = 0$，我们取$b = A$。否则，$a$ 为秩 1，因此 $L = A^{n-1}$ 和 $a$ 是*射影* 模 (命题 22)；因此，$M$与$L$和$a$的直和同构（*代数*，章II, § 2, no. 2，命题4），这证明了命题的第一个部分。另外，根据no. 7、命题16(i)、(iv)、(v)，可得出$b$的类的$c(M) = c(b)$从而唯一性。

注
(1) 命题 23 和 24 以及命题 22 确定完全结构有限生成的 $A$ 模块的推论。 命题 24 表明，无扭转有限生成的 $A$ 模块由其 *秩* 和附加到它的 *除子* 类确定至同构。
(2) 可以证明，在非有限生成的 Dedekind 域投射模必然是*自由* (习题 21)，并且投射模的每个子模都是射影 (习题 20)。

### 习题{#ac-vii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
