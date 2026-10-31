---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 4
section_title: Tensor products of algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 460-484, 626-627
pdf_pages: 0484-0508, 0650-0651
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS
      page: 460
      pdf_page: 484
    - "no": 2
      title: UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS
      page: 463
      pdf_page: 487
    - "no": 3
      title: MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS
      page: 465
      pdf_page: 489
    - "no": 4
      title: TENSOR PRODUCT OF ALGEBRAS OVER A FIELD
      page: 468
      pdf_page: 492
    - "no": 5
      title: TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS
      page: 470
      pdf_page: 494
    - "no": 6
      title: COMMUTATION LEMMAS
      page: 472
      pdf_page: 496
    - "no": 7
      title: TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS
      page: 474
      pdf_page: 498
    - "no": 8
      title: TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES
      page: 480
      pdf_page: 504
    - "no": 9
      title: ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS
      page: 482
      pdf_page: 506
statements: 43
exercises: 2
content_sha256: 99ba022d98aea5ed525d7e653e97c2a91a9025c34a721b4ccf4ee676ad8045c6
translated_from: content/en/alg/III/04_s4_tensor_products_of_algebras.md
translation_method: google
source_content_sha256: 25682b65ee25b300876c8d2b79b960cdd7e6d7279edee98e796e41613580d0ee
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: fc4603e5fcdb73021ff9fec81366f7396026f6f03459dde64e3e063ffff8b972
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 4。 张量积代数

从§ 4到§ 8（含），A表示交换环，并且，另外提及的除非，假设代数是结合且单位的，并且假设代数同态是单位的。

### 1. 代数有限家族的张量积

A 始终表示交换环和单位元。令 (E_i)_{i \in I} 为 A-代数的有限族，并令 E = \bigotimes_{i \in I} E_i 为 A-模 E_i (II, § 3, no. 9) 的张量积 A-模。我们将对 E 定义 A-代数结构。令 m_i: E_i \otimes_A E_i \to E_i 为A-线性映射，在 E_i (§ 1, no. 3) 上定义乘法。考虑A-线性映射

$$
m' = \bigotimes_{i \in I} m_i: \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

复合映射

$$
\left( \bigotimes_{i \in I} E_i \right) \otimes_A \left( \bigotimes_{i \in I} E_i \right) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

其中$\tau$是结合性同构（II, § 3, no. 9）是A-线性映射$m : E \otimes_A E \to E$；我们将看到 $m$ 定义是$E$ 上的（结合和单位）代数结构。因为，在显式执行由$m$定义的乘法时，我们获得公式

(1)
$$
\left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) = \bigotimes_{i \in I} (x_i y_i) \quad \text{for } x_i, y_i \text{ in } E_i \text{ and } i \in I.
$$

因此，通过线性已经看出，如果$e_i$是$E_i$的单位元，则$e = \bigotimes_{i \in I} e_i$是$E$的单位元。另一方面，每个$E_i$的结合性意味着关系

$$
\left( \left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) \right) \left( \bigotimes_{i \in I} z_i \right) = \bigotimes_{i \in I} (x_i y_i z_i) = \left( \bigotimes_{i \in I} x_i \right) \left( \left( \bigotimes_{i \in I} y_i \right) \left( \bigotimes_{i \in I} z_i \right) \right)
$$

从而，根据线性度，关系$x(yz) = (xy)z$对于$E$中的所有$x, y, z$。

#### 定义 1 {#alg-iii-s4-def-1 .statement tag=0608}

*给定一个族* $(E_i)_{i \in I}$ *的代数超过该族* $A$、*张量积，用 $\bigotimes_{i \in I} E_i$ 表示（或者，当 $I$ 是$\mathbf{N}$、$E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n$ 的间隔$\{1, n\}$ 或简单地$E_1 \otimes E_2 \otimes \cdots \otimes E_n$ 时） *通过给出由*(1)定义的*$A$*-模块*$E_i$*乘法的张量积获得代数。

关系 (1) 表明代数与$E_i$的*相反*张量积$\bigotimes_{i \in I} E_i^0$是反代数到$\bigotimes_{i \in I} E_i$；特别是，如果 $E_i$ 是*可交换的*，那么 $\bigotimes_{i \in I} E_i$ 也是可交换的。

令 $(E_i)_{i \in I}$ 和 $(F_i)_{i \in I}$ 为具有相同有限索引集合 $I$ 的两个$A$-代数族。对于每个 $i \in I$，令 $f_i : E_i \to F_i$ 为$A$-代数同态。然后是$A$-线性映射

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

是 *A-代数同态*，由 (1) 得出。

对于 $I$ 中的每个划分 $(I_j)_{j \in J}$，结合性同构

$$
\bigotimes_{j \in J} \left( \bigotimes_{i \in I_j} E_i \right) \to \bigotimes_{i \in I} E_i
$$

(II, § 3, no. 9) 也是 *代数* 同构，如下 (1) 及其定义。

当$I$是$\mathbf{N}$的间隔$[1, n]$且所有代数$E_i$都等于相同的代数$E$时，张量积代数$\bigotimes_{i \in I} E_i$也用$E^{\otimes n}$表示。

我们将把注意力集中在本号的其余部分。到两个代数的张量积的性质，留给读者将它们扩展到任意有限族的张量积的任务。

设$E, F$是两个$A$-代数；如果$a$（或$b$）是$E$（或$F$）的左理想，则$E \otimes_A F$中$a \otimes_A b$的典范像$\operatorname{Im}(a \otimes b)$是$E \otimes_A F$的左理想；用“右理想”或“双边理想”代替“左理想”，也有类似的结果。此外：

#### 命题 1 {#alg-iii-s4-prop-1 .statement tag=0609}

*令$E, F$为两个$A$代数，且$a$（或$b$）为$E$（或$F$）的两侧理想。然后是规范的 $A$-模块同构*

$$
(E/a) \otimes (E/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

（II, § 3, no. 6，推论 1 至命题 6）*为代数同构*。

这是从 (1) 和定义给定 *loc 得出的。引用*。

#### 推论 1 {#alg-iii-s4-prop-1-cor-1 .statement tag=060A}

*设$E$为$A$代数，$a$为$A$的理想。那么$A$-模块$aE$是$E$的双面理想和规范的$(A/a)$-模块同构*

$$
(A/a) \otimes_A E \to E/aE
$$

*是一个*$(A/a)$*-代数同构*。

#### 推论 2 {#alg-iii-s4-prop-1-cor-2 .statement tag=060B}

*如果 $a, b$ 是 $A$ 的两个理想，则 $(A/a) \otimes_A (A/b)$ 与 $A/(a + b)$* 自然同构。

#### 推论 3 {#alg-iii-s4-prop-1-cor-3 .statement tag=060C}

*令$E, F$为两个$A$代数，而$a$为$F$的湮没子所包含的$A$的理想。那么 $(A/a)$-代数 $E \otimes_A F$ 与 $(E/aE) \otimes_{A/a} F$* 是典型同构的。

#### 命题 2 {#alg-iii-s4-prop-2 .statement tag=060D}

*令$(E_\lambda)_{\lambda \in L}$和$(F_\mu)_{\mu \in M}$为$A$代数的两个族。 典范映射* (II, § 3, no. 7)

$$
\left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

*是代数同构*。

这紧接在$E \otimes F$上的乘法的II, § 3, no. 7、命题7和定义。

#### 命题 3 {#alg-iii-s4-prop-3 .statement tag=060E}

*令$A, B$为两个交换环、$\varphi : A \to B$环同态和$E, F$两个$A$代数。然后是规范的 $B$-模块同构*

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

(II, § 5, no. 1, 命题 3) *是一个$B$-代数同构*。

#### 命题 4 {#alg-iii-s4-prop-4 .statement tag=060F}

令$A, B$为两个交换环、$\rho : A \to B$环同态、$E$一个$A$代数和$F$一个$B$代数。然后是规范的 $A$-模块同构

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E))
$$

(II, § 5, no. 2, 命题 6) 是$A$-代数同构。

由于§ 1, no. 5，验证是微不足道的。

特别是，通过将标量的环$B$限制为$A$获得的$B \otimes_A E$上的$A$-代数结构与代数$B \otimes_A E$的结构、张量积相同$A$-代数$B$和$E$。

最后，如果$(A_i, \phi_{ji})$是交换环，$(E_i, f_{ji})$和$(F_i, g_{ji})$的直接系统，$A_i$-代数（$§ 1$，no. 6）和$A = \lim \rightarrow A_i$的两个直接系统，则规范的$A$-模同构

$$
\lim \rightarrow (E_i \otimes_{A_i} F_i) \to (\lim \rightarrow E_i) \otimes_A (\lim \rightarrow F_i)
$$

(II, § 6, no. 3, 命题 7) 也是一个$A$-代数同构，由定义如下。

例张量积代数。 (1) 设$A$为交换环和$M, N$两个$A$模； 典范映射

$$
\text{End}_A(M) \otimes_A \text{End}_A(N) \to \text{End}_A(M \otimes_A N)
$$

(II, § 4, no. 4) 是$A$-代数同态，由II, § 3, no. 2、公式 (5) 如下。当$M$或$N$是有限生成的射影$A$模时，我们知道这个同态是双射的（II, § 4, no. 4，命题4）。特别是，我们恢复了两个方阵中的张量积中的定义。

(2) 设$S, T$为两个幺半群，以及幺半群$S$和$T$在环$A$(III, § 2, no. 6)上的$A^{(S)}$和$A^{(T)}$代数；那么有一个规范的$A$-代数同构

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}.
$$

元素$e_s \otimes e_t$（分别$e_{(s,t)}$），其中$s$穿过$S$，$t$穿过$T$，形式基，$A^{(S)} \otimes_A A^{(T)}$凭借II, § 3, no. 7，推论2 命题 7（分别为$A^{(S \times T)}$；所需的同构是通过映射$e_s \otimes e_t$到$e_{(s,t)}$获得的，并且从定义得出，这确实是代数同构。

### 2. 通用刻画张量积代数

#### 命题 5 {#alg-iii-s4-prop-5 .statement tag=060G}

令$(E_i)_{i \in I}$为$A$代数的有限族，对于每个$i \in I$，令$e_i$为$E_i$的单位元。对于每个 $i \in I$，令 $u_i : E_i \to E = \bigotimes_{i \in I} E_i$ 为由下式定义的 $A$ 线性映射

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{with } x'_i = x_i \text{ and } x'_j = e_j \text{ for } j \neq i.
$$

(i) *$u_i$ 是 $\mathbf{A}$-代数同构；此外，对于$i \neq j$，元素、$u_i(x_i)$和$u_j(x_j)$在$\mathbf{E}$中是可置换的，对于所有$x_i \in \mathbf{E}_i$和$x_j \in \mathbf{E}_j$，$\mathbf{E}$由子代数$u_i(\mathbf{E}_i)$的并生成。

(ii) *令$\mathbf{F}$为$\mathbf{A}$代数，对于所有$i \in \mathbf{I}$，令$v_i : \mathbf{E}_i \to \mathbf{F}$为$\mathbf{A}$代数同态，其中$v_i$使得，对于$i \neq j$，$v_i(x_i)$且对于所有 $x_i \in \mathbf{E}_i$ 和 $x_j \in \mathbf{E}_j$，$v_j(x_j)$ 在 $\mathbf{F}$ 中是可置换的。那么存在且仅有一个 $\mathbf{A}$-代数同态 $w : \mathbf{E} \to \mathbf{F}$ 使得*

$$
v_i = w \circ u_i \quad \text{for all } i \in \mathbf{I}.
$$

(i) 映射 $u_i$ 是 $\mathbf{E}$ 上乘法的代数同态与定义。如果$i \neq j$，$x_i \in \mathbf{E}_i, x_j \in \mathbf{E}_j$，那么

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{with } x'_i = x_i, x'_k = e_k \text{ for } k \neq i,
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{with } x''_j = x_j, x''_k = e_k \text{ for } k \neq j.
$$

显然，$x'_k x''_k = x''_k x'_k$对于所有$k \in \mathbf{I}$，因此$u_i(x_i)$和$u_j(x_j)$在$\mathbf{E}$中通过公式（1）（no. 1）在$\mathbf{E}$中定义乘法进行通勤。 最后一个断言源自关系 $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$。

(ii) 对于每个 $i \in \mathbf{I}$，令 $x_i$ 为元素 / $\mathbf{E}_i$。然后，乘积$\prod_{i \in \mathbf{I}} v_i(x_i)$在$\mathbf{F}$中独立于$\mathbf{I}$上的任何排序进行定义，因为代数$\mathbf{F}$是关联的并且元素$v_i(x_i)$是成对可置换的。 $\prod_{i \in \mathbf{I}} \mathbf{E}_i$到$\mathbf{F}$的映射$(x_i)_{i \in \mathbf{I}} \to \prod_{i \in \mathbf{I}} v_i(x_i)$显然是$\mathbf{A}$-多重线性，因此存在一个且仅有一个$\mathbf{A}$-线性映射$w : \mathbf{E} \to \mathbf{F}$使得

$$
w\left( \bigotimes_i x_i \right) = \prod_i v_i(x_i).
$$

现在，所需的$\mathbf{A}$-代数同态$w : \mathbf{E} \to \mathbf{F}$必须满足(5)，这是从(4)和$\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$事实得出的。这就证明了$w$的唯一性；仍有待证明由(5)定义的$\mathbf{A}$-线性映射$w$是$\mathbf{A}$-代数同态并且满足(4)。 $w$满足(4)的事实是显而易见的：将(5)应用于$x_j = e_j$对于$j \neq i$的情况就足够了，我们得到$w(u_i(x_i)) = v_i(x_i)$。最后，$w$是代数同态，对于

$$
w\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w\left( \bigotimes_i (x_i y_i) \right) = \prod_i v_i(x_i y_i)
$$
$$
= \prod_i (v_i(x_i) v_i(y_i)) = \left( \prod_i v_i(x_i) \right) \cdot \left( \prod_i v_i(y_i) \right)
$$

因为$v_i(x_i)$与$v_j(y_j)$通勤$j \neq i$；因此

$$
w w \left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w \left( \bigotimes_i x_i \right) . w \left( \bigotimes_i y_i \right)
$$

根据线性，完成证明。

The ordered pair consisting of E and the canonical mapping $\phi : (x_i) \mapsto \bigotimes_i x_i$ of $\prod_i E_i$ into E is a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1) where $\Sigma$ is the species of A-algebra structure, the morphisms being the A-algebra homomorphisms and the $\alpha$-mappings the mappings $\prod_i u_i$ of $\prod_i E_i$ into an A-algebra such that the $u_i$ are A-algebra homomorphisms and $u_i(x_i)$ and $u_j(x_j)$ commute for $i \neq j$, for all $x_i \in E_i$ and $x_j \in E_j$.

#### 推论{#alg-iii-s4-n2-cor-1 .statement tag=060H}

*设* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *为A-代数的两个有限族，并且对于所有* $i \in I$，*设* $f_i : E_i \to F_i$ *为代数同态。如果* $u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j$ *是典范同态、映射* $f = \bigotimes_i f_i$ *(cf. no. 1)* *是唯一的 A-代数同态，使得* $f \circ u_i = v_i \circ f_i$ *对于所有* $i \in I$。

同态 $g_i = v_i \circ f_i$满足注，使得$g_i(x_i) = v_i(f_i(x_i))$和$g_j(x_j) = v_j(f_j(x_j))$通勤$i \neq j$、$x_i \in E_i$和$x_j \in E_j$；然后应用命题5。

When, in 命题 5, 代数 F is assumed to be *commutative*, 假设 that $v_i(x_i)$ and $v_j(x_j)$ are permutable for $i \neq j$ is automatically satisfied.因此，*当 F 是可交换的*时，存在规范的双射

$$
\text{Hom}_{A\text{-alg.}} \left( \bigotimes_i E_i, F \right) \to \prod_i \text{Hom}_{A\text{-alg.}} (E_i, F),
$$

即与$\bigotimes_i E_i$的每一个同态$w$关联到$w \circ u_i$的F族中。

注，如果E是可交换的A-代数，则$E \otimes_A F$的环结构与$F_{(E)}$(§ 1, no. 5)相同。

### 3. 模以及超过张量积或代数的多模块

#### 定义 2 {#alg-iii-s4-def-2 .statement tag=060I}

*设 E 为（单位）A-代数。左（或右）E 模块是 E 的底层环上的左（或右）模。*

除非另外提到，所有模和多模块都在本号中考虑。是左模和多模块。

如果 M 是 E 模块，同态 $\eta : A \to E$ (§ 1, no. 4)，则 M 上的定义 A-模结构，称为 M 上 E 模块结构的底层；对于$\alpha \in A, s \in E, x \in M$，

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

因此，对于所有 $s \in E$，M 的位似 $h_s : x \mapsto sx$ 是基础 A-模结构的自同态。相反，在 M 上赋予 E 模块结构相当于在 M 上赋予 A-模结构并将 E 的 A-代数同态 $s \mapsto h_s$ 赋予$\mathrm{End}_A(M)$。

#### 定义 3 {#alg-iii-s4-def-3 .statement tag=060J}

*设E和F为两个（单位）A-代数和M集合，具有E模块结构和F模块结构。 M 在代数 E 和 F 上称为（左）双模，如果：*

(1) *M 是 E 和 F* 的基础环的双模 (II, § 1, no. 14)；
(2) *M 上的 E 模块和 F 模块结构下的两个A-模结构是相同的*。

后者条件表示如果e和$e'$分别是E和F的单位元，那么

$$
(\alpha e)x = (\alpha e')x \quad \text{for } \alpha \in A, x \in M;
$$

那么用$\alpha x$来表示两侧的公共的值。

也可以说，在 E 和 F 上给出 M 双模结构相当于在 M 上给出 A-模结构，并且还将 E 的两个 A-代数同态 $s \mapsto h'_s$ 放入$\mathrm{End}_A(M)$ 和 F 的 $t \mapsto h''_t$ 放入$\mathrm{End}_A(M)$，这样$h'_s h''_t = h''_t h'_s$ 适用于所有 $s \in E$ 和 $t \in F$。因而，$E \otimes_A F$到$\mathrm{End}_A(M)$的(no. 2,命题5)A-代数同态$u \mapsto h_u$是规范导出的，使得$h_{s \otimes t} = h'_s h''_t = h''_t h'_s$对于$s \in E$和$t \in F$。在其他字中，因此在M上定义了$(E \otimes_A F)$模块结构，据说它与E和F上给定的双模结构相关联，并且在该结构下

$$
(s \otimes t).x = s(tx) = t(sx) \quad \text{for } s \in E, t \in F \text{ and } x \in M.
$$

M 上给定的 E 模块和 F 模块结构可以通过标量的环的限制、相应的到两个典范同态 $E \to E \otimes_A F$ 和 $F \to E \otimes_A F$ 从此$(E \otimes_A F)$ 模块结构导出。

相反，如果在 M 上给出一个 $(E \otimes_A F)$ 模块结构，通过典范同态 $E \to E \otimes_A F$ 和 $F \to E \otimes_A F$ M 上的一个 E 模块结构和一个 F 模块结构，并且直接的 M 是代数 E 和 F 上的 *双模* 以及这两个结构并且给定$(E \otimes_A F)$-模块结构与此双模结构相关联。

因而，在代数 E 和 F 上，$(E \otimes_A F)$ 模块和双模之间建立了一对一的对应。显然，对于相关的 $(E \otimes_A F)$ 模块结构，M 的每个子双模都是子模，反之亦然。对于商、乘积、直和以及逆和直极限，也有类似的结果。最后，如果$M'$在代数E和F上是另一个双模并且$f : M \to M'$是双模同态，$f$也是$(E \otimes_A F)$模同态，反之亦然。

显然右双模结构有相应的叙述，或者当例有左E模结构和右F模结构时；在这种情况下，我们谈论的是$(E, F)$双模，并且给出这样的结构相当于在E和$F^o$上给出左双模结构。

#### 例 {#alg-iii-s4-n3-exa-1 .statement tag=060K}

(1) 设B为A-代数； 环 B 具有规范的 (B, B)-双模结构 (II, § 1, no. 14, 例 1)，并且，如果 e 是 B 的单位元，则对于所有 $x \in B$ 和所有 $\alpha \in A$ ，$(\alpha e)x = x(\alpha e) = \alpha x$；因而，B 可以被认为是代数 B 和 $B^o$ 的左双模（与 B 相反）；因而，B 上的 (B, B)-双模结构与 (B $\otimes_A B^o$)-模结构相关联，这样，对于 B 中的 $b, x$ 和 $b'$，

$$
(b \otimes b').x = bx b'
$$

右边是环 B 中的乘积。

(2) 设E和F为两个A-代数、$e, e'$各自的单位元，M为E模，N为F模；这些模结构定义在 M 双模结构上超过环 A 和 E，以及在 N 双模结构上超过环 A 和 F；因而，从这些推导出双模结构在环E和F上张量积$M \otimes_A N$，定义为

$$
x.(m \otimes n) = (x.m) \otimes n, \quad y.(m \otimes n) = m \otimes (y.n)
$$

对于 $x \in E, y \in F, m \in M, n \in N$ (II, § 3, no. 4)；还可以看出，条件 (8) 成立，因此上述双模结构与$M \otimes_A N$上的$(E \otimes_A F)$模块结构相关联，这样

$$
(x \otimes y).(m \otimes n) = (x.m) \otimes (y.n)
$$

对于$x \in E, y \in F, m \in M, n \in N$。

特别是，采用 $M = E_s, E_s \otimes_A N$ 具有规范的 $(E \otimes_A F)$ 模块结构；另一方面，$E \otimes_A N$在规范上与$E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N$相同，其中$E \otimes_A F$被认为具有由典范同态$v : F \to E \otimes_A F$定义的正确F模块结构；对于 E 中的 $x, x'$，$y \in F, n \in N$、$x' \otimes n$ 与 $(x' \otimes e') \otimes n$ 相同，$(x \otimes y).(x' \otimes n') = (xx') \otimes (y.n)$ 与 $((xx') \otimes y) \otimes n$ 相同。因此，$(E \otimes_A F)$-模块$E_s \otimes_A N$与通过同态$v$（II, § 5, no. 1）将标量扩展到$E \otimes_A F$而从N派生的$(E \otimes_A F)$-模块进行标识。 N 到 $E_s \otimes_A N$ 的典范映射 $n \mapsto e \otimes n$ 与 N 到 $(E \otimes_A F) \otimes_F N$ 的典范映射 $n \mapsto (e \otimes e') \otimes n$ 进行识别；这被称为 F-同态。

同样的记号，令P为右(E \otimes_A F)模；那么有一个规范的 Z 模同构

(11) $$ P \otimes_{E \otimes_A F} (E_s \otimes_A N) \to P \otimes_F N $$

其中，右侧 P 通过典范同态 $v$ 被视为右 F 模。因为 P 被规范地与 $P \otimes_{E \otimes_A F} (E \otimes_A F)$ 和 $(E \otimes_A F) \otimes_F N$ 与 $E \otimes_A (F \otimes_F N)$ 以及$E \otimes_A N$ 等同，从而建立了所述的同构（II, § 3, no. 8、命题 8 和 II, § 3, no. 4、命题 4）。

以上所有扩展到*多模块* (II, § 1, no. 14)。

### 4. 张量积代数超过域

设 K 是可交换的 *域*，E、F 是 K 上的两个代数，其各自的单位元 $e, e'$ 均为*非零*。那么同态 $\eta_E : K \to E$ 和 $\eta_F : K \to F$ (§ 1, no. 3) 是单射，这使得我们可以用认同 K 和 E（分别是 F）的子域来表示。由$u(x) = x \otimes e'$和$v(y) = e \otimes y$定义的典范同态$u : E \to E \otimes_K F$和$v : F \to E \otimes_K F$是*单射*（II, § 7, no. 9，命题19），并允许我们使用$E \otimes_K F$的*子代数*来计算认同E和F，两者都有单位元单位元$e \otimes e'$共$E \otimes_K F$。在$E \otimes_K F, E \cap F = K$（II, § 7, no. 9，命题19）。

如果 E' 和 F' 分别是 E 和 F 的子代数，典范同态 $E' \otimes_K F' \to E \otimes_K F$ 是单射的，并且允许我们通过 $E' \cup F'$ (II, § 7, no. 7, 命题 14) 生成认同 $E' \otimes_K F'$ 和 $E \otimes_K F$ 的子代数。

#### 命题 6 {#alg-iii-s4-prop-6 .statement tag=060L}

*设 E、F 为 E（分别为 F）和 C'（分别为 D'）的交换域、K、C（分别为 D）子代数和 C'（分别为 D'）上的两个非零代数，即 E 中的 C（以及 F 中的 D）的中心化器。那么 C \otimes_K D 在 E \otimes_K F 中的中心化器就是 C' \otimes_K D'.*

这都是约化验证$C \otimes_K D$（$x_i \in F, y_i \in F$）属于到$C' \otimes_K D'$的扶正器的元素$z = \sum_i x_i \otimes y_i$；我们知道

$$
C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')
$$

（II, § 7, no. 7，命题 14 的推论）。 $y_i$ 可以假设与 K 线性无关；对于所有$x \in C$，必然$(x \otimes e')z = z(x \otimes e')$，即$\sum_i (xx_i - x_ix) \otimes y_i = 0$，从而$xx_i = x_ix$，对于所有$i$（II, § 3, no. 7，推论1至命题7）；因此对于所有 $i$ 来说必然有$x_i \in C'$，因此$z \in C' \otimes_K F$；类似地可以证明$z \in E \otimes_K D'$，从而命题。

#### 推论{#alg-iii-s4-n4-cor-1 .statement tag=060M}

*如果Z和Z'分别是E和F的中心，则E \otimes_K F 的中心是Z \otimes_K Z'*。

设E和F是代数G在交换域K上的两个子代数；假设 E 的每个元素与 F 的每个元素都可交换。那么典范嵌入 $i : E \to G, j : F \to G$ 定义典范同态 $h = i \otimes j : E \otimes_K F \to G$ (no. 2, 命题 5) 使得
$$
(i \otimes j)(x \otimes y) = xy \quad \text{for } x \in E, y \in F.
$$

#### 定义 4 {#alg-iii-s4-def-4 .statement tag=060N}

*给定代数G超过交换域K，G的两个子代数E，F被认为是线性不相交的超过K，如果它们满足以下条件：*
(1) *E 的每元素与 F 的每元素通勤；*
(2) *G 中的 $E \otimes_K F$ 的典范同态是单射的。*

#### 命题 7 {#alg-iii-s4-prop-7 .statement tag=060O}

*设 G 为交换域 K 上的代数，且 E、F 为 G 的两个子代数，使得 E 的每个元素与 F 的每个元素交换。对于 E 和 F 在 K 上线性不相交的，存在 E 在 K 上的基是充分必要的，这是一个自由G 的子集用于 G 上的右侧 F 模块结构。当情况如此时：*
(i) *典范同态$h : E \otimes_K F \to G$是$E \otimes_K F$的同构到$E \cup F$生成的G的子代数上；*
（二）$E \cap F = K;$
(iii) *E（或 F）在 K 上的每个自由子集都是 G 的自由子集及其右或左 F 模（或 E 模）结构。*

叙述的条件显然是必要的，因为E在K上的每个基都是$E \otimes_K F$的基及其正确的F模结构（II, § 3, no. 7，推论1到命题7）。看出条件就足够了，注即h下$E \otimes_K F$的像H是G中和$\sum_i x_i y_i = \sum_i y_i x_i$的集合，其中$x_i \in E$和$y_i \in F$；如果 $(a_\lambda)$ 是 E 在 K 上的基，则 H 也是由 $(a_\lambda)$ 生成的（右或左）F 模 G 的子模。因此，叙述的条件意味着存在E的基$(a_\lambda)$，它也是F模H的基；由此可见 h 是单射的。 断言 (iii) 从以下事实得出：E 的每个自由子集都包含在 E 的基 (II, § 7, no. 1, 定理 2) 中。

#### 推论 1 {#alg-iii-s4-prop-7-cor-1 .statement tag=060P}

*为了使 $E \otimes_K F$ 的典范同态成为双射，E 在 K 上存在基是（右或左）F 模 G 的基，这是必要且充分的。*

#### 推论 2 {#alg-iii-s4-prop-7-cor-2 .statement tag=060Q}

*设E、F是G的两个子代数，K上的有限秩，使得E的每个元素与F的每个元素可交换。对于E和F在K上线性不相交的，必要且充分的是G的子代数H由下式生成$E \cup F$ 是这样*
$$
[H : K] = [E : K] \cdot [F : K].
$$
这表示满射典范同态 h 的秩 : E \otimes_K F \to H 等于 E \otimes_K F 超过 K 的秩，这相当于说这个同态是双射 (II, § 7, No. 4, 命题9)。

### 5. 张量积代数的无限家族

设 A 为交换环且 (E_i)_{i \in I} 为（单位）A-代数的任意族。对于 I 的每个有限子集 J，令 E_J 表示代数的张量积 $\bigotimes_{i \in J} E_i$ E_i 指标 $i \in J$；让$e_i$表示E_i的单位元和E_J的$e_J = \bigotimes_{i \in J} e_i$单位元；让$f_{J,i}$表示典范同态$E_i \to E_J$对于$i \in J$（no. 2，命题5）。如果 J、J' 是 I 的两个有限子集，则 $J \subset J'$、同态 $f_{J'J} : E_J \to E_{J'}$ 是规范导出的（no. 2、命题 5），对于所有 $i \in J$，通过条件 $f_{J'J} \circ f_{J,i} = f_{J',i}$ 进行规范导出。此外，$f_{J'J}$的唯一性意味着，如果J，J'，J''是I的三个有限子集，使得$J \subset J' \subset J''$，则$f_{J''J} = f_{J''J'} \circ f_{J'J}$。在其他字中，$(E_J, f_{J'J})$是A-代数的直接系统，其索引集合是I的有限子集的右有向集合$\mathscr{F}(I)$。

#### 定义 5 {#alg-iii-s4-def-5 .statement tag=060R}

*直接系统*$(E_J, f_{J'J})$的直极限E被称为A-代数*$(E_i)_{i \in I}$家族的张量积。

如果 I 是有限的，则 E 等于 $\bigotimes_{i \in I} E_i$。由于滥用记号，即使 I 是无穷大，E 也可以表示为$\bigotimes_{i \in I} E_i$。

对于 I 的每个有限子集 J，令 $f_J$ 表示典范同态 $\bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i$（写为 $f_i$ 而不是 $f_{\{i\}}$）；如果 e 是 $\bigotimes_{i \in I} E_i$ 的单位元，则对于所有 $J \in \mathscr{F}(I)$ 来说，$f_J(e_J) = e$。 直接的如果所有代数 E_i 都是可交换的，那么$\bigotimes_{i \in I} E_i$ 也是可交换的。

#### 命题 8 {#alg-iii-s4-prop-8 .statement tag=060S}

(i) *同态* $f_i : E_i \to E = \bigotimes_{k \in I} E_k$ *对于两个指标* i, j *使得* $i \neq j$、$f_i(x_i)$ *和* $f_j(x_j)$ *通勤于* E *对于所有* $x_i \in E_i$ *和* $x_j \in E_j$； *进一步，*E *由子代数*$f_i(E_i)$的并生成。

(ii) *设 F 为 A-代数，并且对于所有* $i \in I$，*令* $u_i : E_i \to F$ *为 A-代数同态，使得对于* $i \neq j$、$u_i(x_i)$ *和* $u_j(x_j)$ *通勤* F *对于所有* $x_i \in E_i$ *和* $x_j \in E_j$。 *那么存在且仅有一个A-代数同态*$u : E \to F$*使得*$u_i = u \circ f_i$*对于所有*$i \in I$。

(i) 因为，对于 I 的每个有限子集 J，$f_i = f_J \circ f_{J,i}$，(i) 中的第一个断言是从 no. 2、命题 5 得出的，取 J 包含 i 和 j；第二个也是从no. 2、命题 5 得出，考虑到当 J 穿过$\mathscr{F}(I)$ 时，E 是$f_J(E_J)$ 的并。

(ii) 对于 I 的每个有限子集 J，从 no. 2、命题 5 可以得出，存在唯一同态 $u_J : E_J \to F$，使得对于所有 $i \in J$ 都有$u_J \circ f_{J,i} = u_i$；从唯一性性质可以立即得出，对于$J \subset J'$，$u_J = u_{J'} \circ f_{J'J}$；在其他字中，$u_J$形式a *直接系统*同态。 Let $u = \lim \to u_J : E \to F$; then by definition $u_J = u \circ f_J$ for every finite subset $J$ of $I$ and in particular $u_i = u \circ f_i$ for all $i \in I$; the uniqueness of $u$ follows from these relations and the fact that the $f_i(E_i)$ generate the algebra $E$.

#### 推论{#alg-iii-s4-n5-cor-1 .statement tag=060T}

*设* $(E_i)_{i \in I},\ (E'_i)_{i \in I}$ *为两个族* $A$*-代数，具有相同的索引集合，并且对于所有* $i \in I$，*设* $u_i : E_i \to E'_i$ *为代数同态。那么存在一个且唯一的* $A$*-代数同态* $u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i$ *这样，对于所有* $i \in I$，*图表*

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
| & & | \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

*可交换*，$f_i$ *和* $f'_i$ *表示典范同态*。

应用命题8至同态$f'_i \circ u_i$就足够了。

命题 8 的推论中定义的同态 $u$ 用$\bigotimes_{i \in I} u_i$ 表示。如果$J$是$I$中的任意一个子集，命题8可以应用于典范同态$f_i : E_i \to \bigotimes_{i \in I} E_i = E$的族$(f_i)_{i \in J}$；推导出典范同态$E_J \to E$，也用$f_J$表示，并且当$J$是*有限*时，重合和同态如上所述表示。

现在让 $(x_i)_{i \in I}$ 为 $\prod_{i \in I} E_i$ 的元素，这样族 $(x_i - e_i)_{i \in I}$ 有 *有限支撑* $H$。就是直接的，如果$J$和$J'$是$I$包含$H$的两个有限子集，那么

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

$I$的有限子集$J \supset H$的$f_J((x_i)_{i \in J})$的公共的值用$\bigotimes_{i \in I} x_i$表示。

#### 命题 9 {#alg-iii-s4-prop-9 .statement tag=060U}

*设*$(E_i)_{i \in I}$*是*$A$*-代数族，并且对于每个*$i \in I$*让*$B_i$*是*$E_i$的基*使得单位元*$e_i$*属于到*$B_i$。 *设*$B$*为形式*$\bigotimes_{i \in I} x_i$元素集合，*其中*$(x_i)$*贯穿*$\prod_{i \in I} B_i$*元素集合，使得族*$(x_i - e_i)$*有有限支撑*。 *那么*$B$*是代数*$\bigotimes_{i \in I} E_i$*中的基*还有这个基包含单位元*$e$。

对于$I$的每个有限子集$J$，对于$i \in J$（II, § 3, no. 9），令$B_J$为基$B_i$的$E_J = \bigotimes_{i \in J} E_i$张量积的基。紧接着从定义可以得出，当$J$穿过$\mathscr{F}(I)$时，$B$是$f_J(B_J)$的并，当$J \subset J'$时，$f_{J',J}(B_J) \subset B_{J'}$；因此，$(B_J)$是$E_J$和$B = \lim \rightarrow B_J$的子集中的直接系统；然后从II, § 6, no. 2得出结论，推论到命题5。

基$B$也称为$i \in I$的基$B_i$的*张量积*；当命题 9 的条件满足时，典范同态 $f_J : E_J \to E = \bigotimes_{i \in I} E_i$ 对于 $I$ 的每个子集 $J$ 都是“内射”，因为如果 $B_J$ 是 $E_J$ 张量积的基对于$i \in J$的$B_i$，立即验证$f_J$到$B_J$的限制是单射的，并且映射$B_J$到$B$的子集。

### 6.交换引理

#### 引理 1 {#alg-iii-s4-lem-1 .statement tag=060V}

*设$A$为交换环，$E$一个$A$-代数，$E$元素$(x_i)_{1 \leq i \leq n}$有限序列，$A$元素$(\lambda_i)_{1 \leq i \leq n}$有限序列和 $E$ 的 $y$ 元素；假设*
$$
x_i y = \lambda_i y x_i \quad \text{for } 1 \leq i \leq n.
$$
*然后*
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

引理对于$n = 1$来说是微不足道的，我们通过归纳对$n \geq 2$进行论证。现在
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1})(x_n y)
= (x_1 \ldots x_{n-1})(\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n,
$$
通过归纳假设，等于
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
从而引理。

#### 引理 2 {#alg-iii-s4-lem-2 .statement tag=060W}

*设$A$为交换环、$E$一个$A$代数以及$(x_i)_{1 \leq i \leq n}$和$(y_i)_{1 \leq i \leq n}$两个有限序列或$E$的$n$元素；假设对于 $1 \leq j \leq i \leq n$,*
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{with } \lambda_{ij} \in A.
$$
*然后*
$$
(x_1 x_2 \ldots x_n)(y_1 y_2 \ldots y_n) = \left( \prod_{i > j} \lambda_{ij} \right) (x_1 y_1)(x_2 y_2) \ldots (x_n y_n).
$$

引理对于$n = 1$来说是微不足道的，我们再次通过归纳对$n$争论$n \geq 2$。凭借引理1，
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1 (x_2 \ldots x_n) y_1 (y_2 \ldots y_n)
= \left( \prod_{i > 1} \lambda_{i1} \right) (x_1 y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
然后应用归纳假设就可以得到(16)。

对于$\mathbf{A}$的元素的每个家庭$\lambda = (\lambda_{ij})$，以及$1 \leq j < i \leq n$，以及每个置换$\sigma \in \mathfrak{S}_n$，我们写

$$
\varepsilon_\sigma(\lambda) = \prod_{i > j,\ \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)}.
$$

观察到，当$\mathbf{A} = \mathbf{Z}$和$\lambda_{ij} = -1$对于每个有序对$(i, j)$使得$1 \leq j < i \leq n$时，$\varepsilon_\sigma(\lambda)$只是置换$\sigma$（I, § 5, no. 7）的签名$\varepsilon_\sigma$。

#### 引理 3 {#alg-iii-s4-lem-3 .statement tag=060X}

*令$\mathbf{A}$为交换环，$\mathbf{E}$一个$\mathbf{A}$代数，$\mathbf{E}$的元素的$(x_i)_{1 \leq i \leq n}$有限序列，并假设对于每个有序对$(i, j)$ 整数使得$1 \leq j < i \leq n$，*

$$
x_i x_j = \lambda_{ij} x_j x_i \quad \text{with } \lambda_{ij} \in \mathbf{A}.
$$

*然后，对于每置换 $\sigma \in \mathfrak{S}_n$，*

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \cdots x_n.
$$

引理对于$n = 1$和$n = 2$来说是微不足道的；我们于$n$乘归纳前往$n \geq 3$。如果 $\sigma(n) = n$，关系 (19) 由归纳假设得出。因此，假设 $\sigma(n) = k, k \neq n$，并令 $\tau$ 为 $\{1, n\}$ 的置换，定义为

$$
\begin{cases}
\tau(i) = i & \text{for } i < k \\
\tau(i) = i + 1 & \text{for } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$

设 $\pi = \tau^{-1} \circ \sigma$； 置换$\pi$叶$n$固定；现在$\sigma = \tau \circ \pi$，因此，写$y_i = x_{\tau(i)},\ y_{\pi(i)} = x_{\sigma(i)}$。如果$i \neq n$和$j \neq n$，关系$\pi(i) > \pi(j)$和$\sigma(i) > \sigma(j)$是等价的（因为$\tau$是$\{1, n-1\}$到$\{1, n\}$的严格递增的映射）。对于 $i \neq n, j \neq n$ 和 $\sigma(i) > \sigma(j)$，

$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i),\ \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i),\ \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$

从而，由归纳假设（使用$\pi(n) = n$这一事实）：

$$
y_{\pi(1)} y_{\pi(2)} \cdots y_{\pi(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) y_1 y_2 \cdots y_n
$$

那就是

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) x_{\tau(1)} \cdots x_{\tau(n)}.
$$

现在

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k
$$

引理 1 等于

$$
\left( \prod_{j > k} \lambda_{jk} \right) x_1 \cdots x_n = \left( \prod_{\sigma(i) > \sigma(n)} \lambda_{\sigma(i),\ \sigma(n)} \right) x_1 \cdots x_n.
$$

最后，（20）和（21）给出

$$
x_{\sigma(1)} \cdots x_{\sigma(n)} = \alpha \cdot x_1 \cdots x_n
$$

与

$$
\alpha = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) \cdot \left( \prod_{i < n, \sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right)
$$
$$
= \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} = \varepsilon_\sigma(\lambda)
$$

完成引理 3 中的证明。

### 7. 张量积分级为代数相对于交换因子

#### 定义 6 {#alg-iii-s4-def-6 .statement tag=060Y}

*设* $(\Delta_i)_{i \in I}$ *是加法编写的可交换幺半群的有限族。 交换因子的系统超过* $\Delta_i$ *，交换环* $\mathbf{A}$ 中的值 *是映射* $\varepsilon_{ij}: \Delta_i \times \Delta_j \to \mathbf{A}$ 系统，*其中* $i \in I$， $j \in I$、$i \neq j$ *满足以下条件*：

(22)
$$
\varepsilon_{ij}(\alpha_i + \alpha'_i, \beta_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha'_i, \beta_j)
$$
(23)
$$
\varepsilon_{ij}(\alpha_i, \beta_j + \beta'_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha_i, \beta'_j)
$$
(24)
$$
\varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ji}(\beta_j, \alpha_i) = 1,
$$

*对于所有* $\alpha_i, \alpha'_i$ *在* $\Delta_i$，$\beta_j, \beta'_j$ *在* $\Delta_j$。

如果给 I 一个总排序，并且 $\Delta_i$ 是群，则交换因子的系统是在 $\Delta_i$ 上定义的，方法是对每个有序对 $(i, j)$ 进行取值，使得 $i < j$ 是任意的将 $\Delta_i \times \Delta_j$ 的 $\mathbf{Z}$-*双线性* 映射代入环 $\mathbf{A}$ 的 *可逆* 元素的 (*乘法*) $\mathbf{Z}$-模$\mathbf{A}^*$，然后写入

$$
\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}
$$

$i < j$。

注，由于$\varepsilon_{ij}(\alpha_i, \beta_j)$是可逆的，

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

凭借（22）和（23）。

#### 例{#alg-iii-s4-n7-exa-1 .statement tag=060Z}

(1) 交换因子的*平凡* 系统由 $\varepsilon_{ij}$ 组成，使得 $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ 对于所有 $i, j$、$\alpha_i \in \Delta_i$、$\beta_j \in \Delta_j$。

(2) 如果对所有$i \in I$取$\mathbf{A} = \mathbf{Z}$和$\Delta_i = \mathbf{Z}$，则通过取$\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$得到交换因子的系统。 注，这个数仅取决于$\alpha_i$和$\beta_j$的奇偶性，因此当某些$\Delta_i$等于$\mathbf{Z}/2\mathbf{Z}$而其他$\mathbf{Z}$时，$\varepsilon_{ij}$可以被视为交换因子。

这两个例是应用中最常遇到的情况。

#### 命题 10 {#alg-iii-s4-prop-10 .statement tag=0610}

令 $\mathbf{A}$ 为交换环和 $(\Delta_i)_{i \in I}$ 有限族可交换幺半群的加法写法；对于每个 $i \in I$ 令 $E_i$ 为型 $\Delta_i$ 的分级 $\mathbf{A}$ 代数。最后，令 $(\varepsilon_{ij})$ 为交换因子的系统与 $\mathbf{A}$ 中的值的$\Delta_i$ 之比。那么存在一个型 $\Delta = \prod_{i \in I} \Delta_i$ 的分级 $\mathbf{A}$-代数 $E$，并且对于每个 $i \in I$ 代数同态 $h_i : E_i \to E$，具有以下属性：

(i) *如果$\phi_i : \Delta_i \to \Delta$为典范同态，则$h_i$为同态* (II, § 11, no. 2)，在其他字、$h_i(E_i^{\alpha_i}) \subset E^{\phi_i(\alpha_i)}$中，其中$(E_i^{\alpha_i})$和$(E^{\alpha})$分别表示$E_i$和$E$。

(ii) *如果 $i \neq j$ 和 $x_i$（分别为 $x_j$）是 $E_i$（分别为 $E_j$）和次数 $\alpha_i \in \Delta_i$（分别为 $\beta_j \in \Delta_j$）的齐次元素，那么*

$$
h_i(x_i) h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) h_j(x_j) h_i(x_i).
$$

(iii) *对于每个$\mathbf{A}$-代数$F$和同态$f_i : E_i \to F$满足条件的每个系统*

$$
f_i(x_i) f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) f_j(x_j) f_i(x_i),
$$

*其中$i, j, x_i, x_j, \alpha_i, \beta_j$如(ii)中所示，则存在且仅一个代数同态$f : E \to F$，使得$f_i = f \circ h_i$对于所有$i \in I$。此外，$E$的底层$\mathbf{A}$模块是张量积$\bigotimes_{i \in I} E_i$。*

考虑$\mathbf{A}\text{-module}$$E = \bigotimes_{i \in I} E_i$；它由子模$E^{\alpha}$的直和标识，其中，对于每个$\alpha = (\alpha_i) \in \Delta$，我们写$E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i}$； $E^{\alpha}$ 因此形式在$\mathbf{A}$-模块$E$ 上有型 $\Delta$ 的毕业。我们将在$E$上进行定义*分级$\mathbf{A}$-代数*结构，共型$\Delta$。为此，让 $I$ 得到全序；对于元素$\alpha = (\alpha_i), \beta = (\beta_i)$或$\Delta$的每个有序对，我们必须首先将定义将$E^{\alpha} \times E^{\beta}$的$\mathbf{A}$双线性映射到$E^{\alpha + \beta}$，或者将$\mathbf{A}$线性映射$m_{\alpha \beta}$ $E^{\alpha} \otimes_{\mathbf{A}} E^{\beta}$ 变为$E^{\alpha + \beta}$。我们将在条件之前定义$m_{\alpha \beta}$

$$
m_{\alpha \beta} \left( \left( \bigotimes_{i \in I} x_i \right) \otimes \left( \bigotimes_{i \in I} y_i \right) \right) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

对于 $x_i \in E_i^{\alpha_i}, y_i \in E_i^{\alpha_i}$，其中

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

(27) 的右侧显然属于到$E^{\alpha + \beta}$ 和映射 $(x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)$ 是$\mathbf{A}$-$E_i^{\alpha_i}$ 和$E_i^{\beta_i}$ ($1 \leq i \leq n$) 的乘积中的多重线性。那么必须证明这样定义在E上的乘法是结合律；现在，如果$\gamma = (\gamma_i)$是$\Delta$的三分之一元素，$z_i \in E_i^{\gamma_i'}$是$1 \leq i \leq n$，那么

$$
\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) \left( \bigotimes_i z_i \right) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$

$$
\left( \bigotimes_i x_i \right) \left( \left( \bigotimes_i y_i \right) \left( \bigotimes_i z_i \right) \right) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$

约化验证身份

$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$

但后者紧随关系而来

$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$

直接的推论定义 (28) 和 (22) 和 (23)。

如果对于所有 $i \in I$，$e_i$ 表示 $E_i$ 的单位元，我们知道 $e_i$ 是次数 0 (§ 3, no. 1) 的齐次，因此 $e = \bigotimes_{i \in I} e_i$ 是次数 0 的齐次，并且由 (27) 得出， (28) 和关系

$$
\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1
$$

$e$ 是 $E$ 的单位元，从而在所需评分的 A-代数结构的 $E$ 上完成定义。然后取$h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j$；为了验证$E_i$中的$x_i, x_i'$有$h_i(x_i x_i') = h_i(x_i) h_i(x_i')$，可以将注意力限制在$x_i$和$x_i'$齐次的情况，然后这个关系紧随(27)和关系$\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$；同样的关系和(24)也证明了叙述的$h_i$满足条件(i)和(ii)并且

$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$

其中右侧是 E 中有序序列 $(h_i(x_i))_{i \in I}$ 的乘积，在 I (I, § 1, no. 2) 上给定总排序（足以通过 $x_i$（假设同质）的数上的归纳与$e_i$ 不同）进行争论。

尚待证明条件(iii)； 注那个映射

$$
(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i),
$$

其中右侧是有序序列 $(f_i(x_i))_{i \in I}$ 的乘积，且在 $I$ 上给定总排序，是 A-多重线性。那么存在且仅有一个 A-线性映射 $f : E \to F$ 使得

$$
f\left( \bigotimes_{i \in I} x_i \right) = \prod_{i \in I} f_i(x_i).
$$

显然$f(e)$是$F$和$f \circ h_i = f_i$的单位元；为了验证$f$是代数同态，在其他字中$f(x)f(y) = f(xy)$对于$E$中的$x, y$，注意力可以通过线性限制于$x = \bigotimes_{i \in I} x_i$和$y = \bigotimes_{i \in I} y_i$，$x_i$（分别为）的情况。 $y_i$)对于所有$i \in I$来说是次数$\alpha_i$(分别是$\beta_i$)的齐次。 关系待验证约化，由 (27) 得到

$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$

但是，考虑到关系 (26)，这是推论引理 2 no. 6。

显然，代数$E$和典范映射$\psi : \bigotimes_{i \in I} E_i \to E$构成了*普遍映射问题*（*集合理论*，IV, § 3, no. 1）的解，其中$\Sigma$是类 A-代数结构以及从 $\prod_i E_i$ 到 A-代数、满足条件的 $\alpha$ 映射 $\prod_i f_i$ (26)。

对于 $I$ 的固定总排序，命题 10 中证明中定义的分级代数 $E$ 将称为该系列的*分级张量 $\varepsilon$-产品型* $\Delta$ 代数型 $\Delta_i$ 的$(E_i)_{i \in I}$，将用$^{\varepsilon} \bigotimes_{i \in I} E_i$表示（如果$I$的排序不会产生混淆）；类似地，在命题 10 的证明中定义的同态$f : E \to F$将被表示为$^{\varepsilon} \bigotimes_{i \in I} f_i$。 同态 $h_i$ 被称为*规范*。当$I = \{1, n\}$和所有$E_i$等于相同的代数$G$时，我们也写为$^{\varepsilon} G^{\otimes n}$。

#### 注 {#alg-iii-s4-n7-rem-1 .statement tag=0611}

(1) 我们恢复no. 1中定义的代数的张量积（此外还有其因子的分度张量积），对所有$i, j, \alpha_i$和$\beta_j$取$\varepsilon_{ij}(\alpha_i, \beta_j) = 1$。

（2）假设所有$\Delta_i$都等于$\mathbf{Z}$，写为$\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$； 张量$\varepsilon$-乘积$^{\varepsilon} \bigotimes_{i \in I} E_i$相应的到交换因子的系统则称为分级代数$E_i$的*倾斜*张量积型$\mathbf{Z}$并用$^{\varepsilon} \bigotimes_{i \in I} E_i$表示（或用$E \ ^{\varepsilon} \otimes_A F$表示两个代数，或用$^{\varepsilon} G^{\otimes n}$代替$^{\varepsilon} G^{\otimes n}$）。

#### 推论 1 {#alg-iii-s4-prop-10-cor-1 .statement tag=0612}

在命题 10的记号中，进一步假设F是型$\Delta$的分级A-代数，并且每个$f_i$是相对于$\phi_i : \Delta_i \to \Delta$的分级代数同态；那么$f = \varepsilon \bigotimes_i f_i$就是分级的代数同态。

这直接从 $f$ 的定义以及以下事实得出：
$$
\sum_{i \in I} \phi_i(\alpha_i) = (\alpha_i)
$$
由$\phi_i$的定义。

因此可以看出，$(E, \psi)$也是另一个普遍映射问题的解，其中$\Sigma$是类*分级A-代数*结构*型*$\Delta$， 态射被分级为型 $\Delta$ 的代数同态和 $\alpha$ 映射映射 $\prod_i f_i$，其中，在加法到条件 (26) 中，假设 $f_i$ 是分级的代数同态相对于 $\phi_i$。

#### 推论 2 {#alg-iii-s4-prop-10-cor-2 .statement tag=0613}

*让*$(E_i)_{i \in I}, (F_i)_{i \in I}$*是*A*代数的两个有限族，其中*$E_i$*和*$F_i$*分级为型*$\Delta_i$*对于所有*$i \in I$。 *对于每个*$i \in I$，*让*$g_i : E_i \to F_i$*成为型*$\Delta_i$的分级代数同态。 *然后，如果* $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i$ *和* $h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i$ *是典范同态，则存在一个且仅有一个同态型* $\Delta$、$g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i$ *的分级* A* 代数，使得* $g \circ h_i = h'_i \circ g_i$ *对于所有* $i \in I$。 *此外，如果每个* $g_i$ *是双射，那么* $g$ 也是双射。

将推论1应用到$f_i = h'_i \circ g_i$就足够了，注意条件(26)然后从关系(25)应用到$h'_i$。

推论2中定义的同态也用$\varepsilon \bigotimes_i g_i$表示（如果不会引起混淆）；如果对于每个$i \in I$，$G_i$是型$\Delta_i$的第三个分级A-代数，并且$g'_i : F_i \to G_i$是代数同态，则
$$
\left( \varepsilon \bigotimes_i g'_i \right) \circ \left( \varepsilon \bigotimes_i g_i \right) = \varepsilon \bigotimes_i (g'_i \circ g_i),
$$
如下式（30）所示。

在型 $\mathbf{Z}$ 的分级代数 *倾斜* 张量积的情况下，对于型的分级代数的同态 $f_i : E_i \to F_i$，我们写 $\varepsilon \bigotimes_i f_i$ 而不是 $\varepsilon \bigotimes_i f_i$ $\mathbf{Z}$；当$I = \{1, 2\}$时，这个同态也表示为$f_1 \varepsilon \otimes f_2$；当$I = \{1, n\}$和所有$E_i$（或$F_i$）相等并且所有$f_i$等于相同的同态$f$时，我们写为$\varepsilon f^{\otimes n}$。

#### 注 {#alg-iii-s4-n7-rem-2 .statement tag=0614}

在命题 10 的证明中，$I$ 上的总排序被用于定义和张量积 $\bigotimes_{i \in I} E_i$ 上的 A-模 *代数* 结构

E_i。如果 I 上的排序发生变化，$\bigotimes_{i \in I} E_i$ 上会出现另一个乘法结构，但由此获得的新代数与上述规范“同构的”，因为两者都是相同普遍映射问题的解。对于例，当代数 $E_1 \overset{\varepsilon}{\otimes}_A E_2$ 的 $I = \{1, 2\}$、典范同构到代数 $E_2 \overset{\varepsilon}{\otimes}_A E_1$ 映射 $x_1 \otimes x_2$ 到 $\varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1$，其中 $x_1$ 是次数的齐次$\alpha$ 和$x_2$ 次数 $\beta$ 齐次。

令 J 为 I 的子集，对于每个 $i \in J$，考虑典范同态 $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E$。凭借关系 (25) 典范同态 $h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E$ 是从这些同态规范地（通过命题 10）导出的，这样，对于所有 $i \in J$、$h'_i = h \circ h_i$、$h'_i$ 都是典范同态 $E_i \to E'$。取 I 上选择的 J 上的总排序，我们得到

$$
h\left( \bigotimes_{i \in J} x_i \right) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

其中中间的项是*有序的序列*$(h_i(x_i))_{i \in J}$的乘积，并且在右手中项，$x'_i = x_i$代表$i \in J$，$x'_i = e_i$代表$i \notin J$。

#### 命题 11 {#alg-iii-s4-prop-11 .statement tag=0615}

（张量 $\varepsilon$-产品的“结合性”）。 *在命题 10 的记号中，设*$(J_\lambda)_{\lambda \in L}$*为我的划分，并写*$\Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i$*对于所有*$\lambda \in L$。 *Let* $E'_\lambda$ *be a graded tensor $\varepsilon$-product of type* $\Delta'_\lambda$ *of the family* $(E_i)_{i \in J_\lambda}$ *for some total ordering chosen on* $J_\lambda$. *另一方面，对于* $\lambda, \mu$ *在* $L$ *和* $\lambda \neq \mu$，*我们写，对于* $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$，$\beta'_\mu = (\beta_j)_{j \in J_\mu}$，

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

*那么*$(\varepsilon'_{\lambda \mu})$*是交换因子的系统在*$\Delta'_\lambda$*和值在*$A$*并且存在且仅有一个型的分级代数*同态* $\Delta$，$v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$，*这样*

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*对于所有* $(x_i) \in \prod_{i \in I} E_i$，*假设对 I 采取总排序，其中诱导对每个* $J_\lambda$ *选择总排序，并且对于* $\lambda < \mu$ *在* $L$、$i \in J_\lambda$ *和* $j \in J_\mu$、$i < j$。

事实上，交换因子的$\varepsilon'_{\lambda \mu}$形式系统是微不足道的。让$h_{i,\lambda} : E_i \to E'_\lambda$，$h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$*为典范同态*（对于$\lambda \in L$，$i \in J_\lambda$）*并写*$h''_i = h'_\lambda \circ h_{i,\lambda}$； *凭借普遍映射问题的* 解唯一性就足够了，证明 $\varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ 和命题 10 的 $h''_i$ 满足条件。现在，对于所有 $\lambda \in L$，令$f'_\lambda : E'_\lambda \to F$ 为唯一代数同态，使得 $f'_\lambda \circ h_{i,\lambda} = f_i$ 对于所有 $i \in J_\lambda$。我们证明，对于 $\lambda \neq \mu$，$\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}, \beta'_\mu = (\beta_j)_{j \in J_\mu}$，

$$
f'_\lambda(x'_\lambda)f'_\mu(x'_\mu) = \varepsilon'_{\lambda\mu}(\alpha'_\lambda, \beta'_\mu)f'_\mu(x'_\mu)f'_\lambda(x'_\lambda)
$$

对于$x'_\lambda \in E'_\lambda$（或$x'_\mu \in E'_\mu$）同质的次数$\alpha'_\lambda$（或$\beta'_\mu$）；当$x'_\mu = \bigotimes_{i \in J_\lambda} x_i, x'_\mu = \bigotimes_{j \in J_\mu} x_j, x_i$（或$x_j$）与次数$\alpha_i$（或$\beta_j$）齐次于$E_i$（或$E_j$）对于$i \in J_\lambda, j \in J_\mu$时，通过线性就足以验证它。但这是从公式 (30) 得出的，其中定义 no. 6 的 $f'_\lambda$ 和引理 3，考虑到假设 (26) 和定义 (32)。因此，存在且仅有一个代数同态 $f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F$，使得 $f \circ h'_\lambda = f'_\lambda$ 对于所有 $\lambda \in L$； 从而$f \circ h''_i = f_i$对于所有$i \in I$和$f$的唯一性来说是微不足道的。

### 8. 张量积评分为代数相同型

假设no. 7、命题 10 的假设成立，进一步假设所有$\Delta_i$都等于*相同的可交换幺半群*$\Delta_0$；然后，我们可以考虑张量$\varepsilon$-产品$\varepsilon \bigotimes_{i \in I} E_i$的*总毕业*型$\Delta_0$，与型$\Delta = \Delta_0^I$在这个代数（II, § 11, no. 1）上的毕业相关；我们称$\varepsilon \bigotimes_{i \in I} E_i$为毕业，*分级为张量$\varepsilon$-家庭$(E_i)_{i \in I}$的型*$\Delta_0$的产品，分级为代数的型$\Delta_0$。

总是保留no. 7的命题 10的记号，假设$F$也是型* $\Delta_0$的*分级A-代数，并且$f_i$是代数的*同态型*$\Delta_0$。那么 $f : \varepsilon \bigotimes_{i \in I} E_i \to F$ 也是型* $\Delta_0$ 的分级代数的 *同态：因为从公式 (30) (no. 7) 可以得出，如果 $x_i$ 是齐次的并且是次数 $\alpha_i \in \Delta_0, \bigotimes_{i \in I} x_i$和$\prod_{i \in I} f_i(x_i)$都是次数$\sum_{i \in I} \alpha_i \in \Delta_0$的齐次。

因此可以说，$\varepsilon \bigotimes_{i \in I} E_i$与型$\Delta_0$的总分级，与典范映射$\psi$、解一起构成了第三个普遍映射问题，其中$\Sigma$是*分级的类型* $\Delta_0$的A-代数，态射是同态，型$\Delta_0$的分级代数，$\alpha$映射是映射$\prod_i f_i$，其中， 加法至条件(26)(no. 7)，假设每个$f_i$是型$\Delta_0$的分级代数中的同态。

对于 I 的每个子集 J，典范同态 $\varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i$ (no. 7) 实际上是同态的分级代数的型 $\Delta_0$，如下所示。

#### 命题 12 {#alg-iii-s4-prop-12 .statement tag=0616}

（张量$\varepsilon$的“结合性”-相同型的分级代数的产品）。 *对于记号 of 命题 10 of no. 7，假设所有$\Delta_i$都等于同一个幺半群$\Delta_0$；设$(J_\lambda)_{\lambda \in L}$为I的划分。对于no. 7的命题11的记号，假设公式(32)(no. 7)的右侧仅取决于和$\alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j$，对于每个不同指标的有序对$(\lambda, \mu)$，所有$\alpha'_\lambda \in \Delta'_\lambda$和所有$\beta'_\mu \in \Delta'_\mu$；让 $\varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu)$ 表示 (32) 的右侧。 *那么 $(\varepsilon''_{\lambda \mu})$ 是交换因子中的系统超过家庭 $(\Delta''_\lambda)_{\lambda \in L}$，其中 $\Delta''_\lambda = \Delta_0$ 代表所有 $\lambda \in L$。 *如果$E''_\lambda$是$(E_i)_{i \in J_\lambda}$族的张量$\varepsilon$-型$\Delta_0$的积，则型的分级代数存在且仅有一个同构 $\Delta_0$，$w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$，这样

$$
w \left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*前提是在 $J_\lambda$ 和 I 上选择总排序，如no. 7、命题 11 中所述。*

通过假设，对于$\Delta_0$中的$\gamma, \delta$，$\varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta)$对于一些$i_0 \in J_\lambda$和一些$j_0 \in J_\mu$，正如通过考虑元素$\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$和$\beta'_\mu = (\beta_j)_{j \in J_\mu}$使得$\alpha_{i_0} = \gamma, \alpha_i = 0$对于$i \neq i_0$，$\beta_{j_0} = \delta, \beta_j = 0$对应$j \neq j_0$；紧接着是交换因子的$\varepsilon''_{\lambda \mu}$形式系统。 证明的其余部分类似于命题 11 (no. 7) 并留给读者。

注当 $\Delta_0 = \mathbf{Z}$ 时，满足命题 12 的附加假设，并且 $(\varepsilon_{ij})$ 是，对于所有 $i, j$ 来说，因子 $(\varepsilon_{ij}(\alpha_i, \beta_j)) = 1$ 的平凡系统，或者系统因子由$\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$定义；在后一种情况下，公式 (32) 的右侧等于 $(-1)^\gamma$，其中

$$
\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = \left( \sum_{i \in J_\lambda} \alpha_i \right) \left( \sum_{j \in J_\mu} \beta_j \right).
$$

#### 注 {#alg-iii-s4-n8-rem-1 .statement tag=0617}

(1) 令 I 为无限索引集合且 $\Delta_0$ 为可交换幺半群；让$(\Delta_i)_{i \in I}$表示家庭，使得$\Delta_i = \Delta_0$对于所有$i$，并假设为I映射$\varepsilon_{ij} : \Delta_i \times \Delta_j \to A$满足条件的不同指标$(i, j)$的每个有序对给出（22），（23）和（24） （no. 7）；这也将被称为家庭* $(\Delta_i)$ 的*系统交换因子。考虑一个$(E_i)_{i \in I}$等级为A-代数为型$\Delta_0$的家庭；对于 I 的每个有限子集 J，令 $E_J$ 表示子族 $(E_i)_{i \in J}$ 的型* $\Delta_0$ 的*分级张量 $\varepsilon$ 乘积（具有 J 上总排序的任意选择）。如果J，J'是I的两个有限子集，使得型$\Delta_0$的分级代数的$J \subset J'$，典范同态，h_{J'J}：E_J\to E_{J'}，已在上面定义，并且这些同态的属性唯一性立即证明如果 J \子集 J' \子集 J'' 是 I 的三个有限子集，则 h_{J''J} = h_{J'J'} \circ h_{J'J}。因此，型$\Delta_0$(§ 3, no. 3)的分级代数有直接系统(E_J，h_{J'J})，其索引集合是I的有限子集的右有向集合$\mathfrak{F}(I)$。 型$\Delta_0$的代数，这个直接系统（§ 3, no. 3）的*直极限*，被称为家族的*分级张量$\varepsilon$-型*$\Delta_0$的产品$(E_i)_{i \in I}$；也用$\varepsilon \bigotimes_{i \in I} E_i$表示。当所有$\Delta_i$等于$\mathbf{Z}$和$\varepsilon_{ij}(a_i, \beta_j) = (-1)^{\alpha_i \beta_j}$时，张量积$\varepsilon \bigotimes_{i \in I} E_i$也称为族$(E_i)_{i \in I}$的*倾斜*张量积，并用$g \bigotimes_{i \in I} E_i$表示。我们将公式化的任务留给读者，证明命题将no. 7的命题10推广到I无限的情况，正如no. 5的命题8将no. 2的命题5推广到我的情况是无限的。 注$\varepsilon \bigotimes_{i \in I} E_i$的底层A-模与no. 5中定义的非分级代数系列$(E_i)_{i \in I}$的（非分级）张量积相同。

(2) 令E为型$\Delta_0$的分级A-代数（其中$\Delta_0$是可交换幺半群）和$\rho : A \to B$环同态； $\rho^*(E)$ (II, § 11, no. 5) 上的刻度与分级张量积 $B \otimes_A E$ 上的刻度相同，其中B 具有平凡的刻度。

### 9. 反交换代数和交错的代数

#### 定义 7 {#alg-iii-s4-def-7 .statement tag=0618}

*如果对于 E 的所有非零齐次元素 x, y，则型 $\mathbf{Z}$ 的分级 A-代数 E 称为反交换的

$$
xy = (-1)^{\deg(x)\deg(y)} yx.
$$

*代数 E 如果它是反交换的，则称为交错的，并且对于奇数次数的每个齐次元素 $x \in E$，也称为 $x^2 = 0$。*

#### 注 {#alg-iii-s4-n9-rem-1 .statement tag=0619}

(1) 设$E^+$为$E_{2n}$($n \in \mathbf{Z}$)的E直和的分级子代数；从定义 7 可以得出，如果 E 是反交换的，则 $E^+$ 是包含在* E 的中心中的 *子代数（因此是可交换的）。

(2) 假设2不是E中0的除子；那么如果 E 是反交换的，则 E 是交错的，因为对于 $x \in E$ 齐次且奇数次数，$x^2 = -x^2$ 由 (36) 得出，从而 $2x^2 = 0$ 且$x^2 = 0$ 凭借假设。

(3) 我们将在交错的代数的§ 7重要例进行详细学习。

#### 引理 4 {#alg-iii-s4-lem-4 .statement tag=061A}

*设 E 为型 $\mathbf{Z}$ 的分级代数，S 集合为同质元素 $\neq 0$； E 的元素的集合 F，其所有均质成分 $x \neq 0$ 满足关系 (36) 对于所有 $y \in S$ 都是 E 的分级子代数。*

注满足： (1) 如果$x', x''$是相同次数$p$的两个齐次元素，$y$是次数$q$和$x'y = (-1)^{pq}yx'$的齐次元素， $x''y = (-1)^{pq}yx''$，然后还有$(x' + x'')y = (-1)^{pq}y(x' + x'')$； (2) 如果$x', x''$分别是次数、$p', p''$、$y$的两个齐次元素、次数、$q$和$x'y = (-1)^{p'q}yx'$、$x''y = (-1)^{p''q}yx''$的齐次元素，则
$$
(x'x'')y = (-1)^{(p'+p'')q}y(x'x'').
$$

#### 命题 13 {#alg-iii-s4-prop-13 .statement tag=061B}

*设E为型$\mathbf{Z}$的分级A-代数和同质元素$\neq 0$的代数E由……组成的S生成的系统；为了使 E 是反交换的（分别为交错的），(36) 对于所有 $x \in S$ 和 $y \in S$ 成立是必要且充分的（分别是，这个条件成立，并且进一步，$x^2 = 0$ 对于奇数次数属于的所有 $x$ 齐次成立S).*

我们首先考虑反交换代数的情况。通过引理 4，子代数 F 由……组成元素的所有同质分量 $x \neq 0$ 满足 (36) 对于所有 $y \in S$，包含所有元素 S，因此$F = E$。如果现在 $F'$ 类似地是元素的 E 由……组成的子代数，其所有同质分量 $x \neq 0$ 满足 (36) 对于每个齐次元素 $y \neq 0$，则从上式可以得出 $F'$ 包含于 S 的所有元素，因此 $F' = E$，在这种情况下完成命题的证明。

为了在交错的代数的情况下证明命题，可以假设E已经是反交换的；那么直接的，E中奇数次数的每个齐次元素都是形式$\sum_i z_ix_i$，其中$z_i \in E^+$和$x_i \in S$是奇数次数（使用$E^+$包含在E) 的中心；由此可知，自$x_i^2 = 0$乘以假设，$\left( \sum_i z_ix_i \right)^2 = \sum_i z_i^2x_i^2 + \sum_{i<j} z_i z_j (x_ix_j + x_jx_i) = 0$乘以(36)乘以$x_ix_j + x_jx_i = 0$。

#### 命题 14 {#alg-iii-s4-prop-14 .statement tag=061C}

*令 E 和 F 为型 $\mathbf{Z}$ 的两个等级 A-代数，均为反交换的（分别为交错的）。那么偏斜张量积 $E^g \otimes_A F$ (no. 7) 是一个反交换律（分别为交错的）代数。*

$E^g \otimes_A F$的生成的系统由$x \otimes y$组成，其中$x$（或$y$）是E（或F）的齐次元素$\neq 0$。考虑两个这样的元素$x \otimes y, x' \otimes y'$，以及$\deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q'$，因此$x \otimes y$是次数$p + q$，$x' \otimes y'$是次数$p' + q'$。然后由定义 (no. 7, 公式 (27)) 并凭借 (36)，
$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq'+pp'+qq'}(xx') \otimes (yy')
\end{align*}
$$
命题 13 的判据表明，$E^g \otimes_A F$ 自 $pq' + pp' + qq' - qp' \equiv (p + q)(p' + q')$（模 2）以来是反交换的。如果进一步E和F是交错的且$p + q$是奇数，则数$p, q$之一必然是奇数，因此$(x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0$和命题13表明$E^g \otimes_A F$是交错的。

#### 推论{#alg-iii-s4-n9-cor-1 .statement tag=061D}

*设 E 为反交换律*（分别为 *交错的*）*分级为 A-代数或型 $\mathbf{Z}$。那么对于每个环同态 $\rho : A \to B$，分级 B 代数 $\rho^*(E)$ (no. 8, *注 2*) *是反交换的*（分别是 *交错的*）。

具有平凡分度的环 B 可以被视为交错的 A-代数和$\rho^*(E) = E^g \otimes_A B$，因此可以应用命题 14。

#### 注 {#alg-iii-s4-n9-rem-2 .statement tag=061E}

令 E 为型 $\mathbf{Z}$ 的反交换律 A-代数。那么由E($§ 1$,no. 3)的乘法定义的$E \otimes_A E$入E的A-线性映射就是分级的A-代数$E^g \otimes_A E$入E的同态，对于命题14的记号来说， 代数E,
$$
(xy)(x'y') = (-1)^{qp'}(xx')(yy').
$$

### 习题{#alg-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
