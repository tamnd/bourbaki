---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 11
section_title: Graded modules and rings
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 363-377, 424-425
pdf_pages: 0387-0401, 0448-0449
extraction: ocr
subsections:
    - "no": 1
      title: GRADED COMMUTATIVE GROUPS
      page: 363
      pdf_page: 387
    - "no": 2
      title: GRADED RINGS AND MODULES
      page: 364
      pdf_page: 388
    - "no": 3
      title: GRADED SUBMODULES
      page: 367
      pdf_page: 391
    - "no": 4
      title: CASE OF AN ORDERED GROUP OF DEGREES
      page: 371
      pdf_page: 395
    - "no": 5
      title: GRADED TENSOR PRODUCT OF GRADED MODULES
      page: 374
      pdf_page: 398
    - "no": 6
      title: GRADED MODULES OF GRADED HOMOMORPHISMS
      page: 375
      pdf_page: 399
statements: 28
exercises: 1
content_sha256: e8dbf7e870d6efc857a00de8c3a67954fabc76c9bdf5c93bd259705578a937a7
translated_from: content/en/alg/II/11_s11_graded_modules_and_rings.md
translation_method: google
source_content_sha256: cee0143d544bc99c4e8496ec6bc7458982857f3f0ed4fb081e4de491d7e81dfd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 24e02255526574841732e11873427be0d5630db32712235ef1a41a18b07ee125
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 11。分级为模和环

*从本段的no. 2开始，$\Delta$将表示可交换幺半群（I, § 2, no. 1），以加法形式书写，单位元素表示为0。*

### 1. 分级交换群

我们将把直和（§ 1, no. 8）翻译成另一个语言定义。

#### 定义 1 {#alg-ii-s11-def-1 .statement tag=05XX}

*给定可加的交换律群$G$和集合$\Delta$，$G$上型$\Delta$的毕业是$G$的子群的$(G_\lambda)_{\lambda \in \Delta}$，其中$G$是直和。 集合 $G$，其中结构由其群运算及其分级定义，称为型 $\Delta$ 的分级（交换）群。*

$\Delta$称为$G$的次数*的*集合。如果元素 $x \in G$ 被称为*同质*，如果它属于到 $G_\lambda$ 之一，则 *次数* $\lambda$ 如果 $x \in G_\lambda$ 是同质的。因此，元素 0 是所有次数的齐次；但如果$x \neq 0$是齐次的，则属于仅是$G_\lambda$之一； 指标$\lambda$，这样$x \in G_\lambda$就被称为*$x$的*次数（或有时$x$的*权*），并且有时由$\deg(x)$表示。每个$y \in G$可以唯一地写成齐次元素和$y_\lambda \in G_\lambda$的和$\sum_\lambda y_\lambda$； $y_\lambda$ 被称为 $y$ 的 * 次数* $\lambda$ 的齐次分量（或简称为次数* $\lambda$ 的 * 分量）。当使用字“权”代替“次数”时，形容词“均质”被“等压”替代。

#### 例 {#alg-ii-s11-n1-exa-1 .statement tag=05XY}

(1) 给定任何可交换幺半群$\Delta$（单位元素 0）和可交换群$G$，通过对$\lambda \neq 0$取$G_0 = G$和$G_\lambda = \{0\}$，在$G$上定义毕业$(G_\lambda)_{\lambda \in \Delta}$；这个毕业被称为*琐碎*。

(2) 令$\Delta, \Delta'$为$\Delta$的两个集合和$\rho$映射入$\Delta'$。令$(G_\lambda)_{\lambda \in \Delta}$为型$\Delta$在可交换群$G$上的毕业；对于$\mu \in \Delta'$，令$G'_\mu$为$G_\lambda$的和，使得$\rho(\lambda) = \mu$；显然，$(G'_\mu)_{\mu \in \Delta'}$是型$\Delta'$在$G$上的毕业，据说是通过映射$\rho$从$(G_\lambda)$“派生”的。

当 $\Delta$ 是可加地写成的交换律群且将 $\Delta$ 的 $\rho$ 映射 $\lambda \mapsto -\lambda$ 写到其自身上时，$(G'_\mu)$ 称为 $(G_\lambda)$ 的*对立*毕业。

(3) 如果$\Delta = \Delta_1 \times \Delta_2$ 是两个集合的积，则型 $\Delta$ 的毕业称为型 $\Delta_1, \Delta_2$ 的*二毕业*。对于所有$\lambda \in \Delta_1$，令$G'_\lambda = \bigoplus_{\mu \in \Delta_2} G_{\lambda \mu}$，对于所有$\mu \in \Delta_2$，令$G''_\mu = \bigoplus_{\lambda \in \Delta_1} G_{\lambda \mu}$；显然，$(G'_\lambda)_{\lambda \in \Delta_1}$是型$\Delta_1$的毕业，$(G''_\mu)_{\mu \in \Delta_2}$是型$\Delta_2$在$G$的毕业；这些毕业被称为*部分毕业*，源自大毕业$(G_{\lambda \mu})$。 注即$G_{\lambda \mu} = G'_\lambda \cap G''_\mu$；相反，如果$(G'_\lambda)_{\lambda \in \Delta_1}$和$(G''_\mu)_{\mu \in \Delta_2}$是$G$上的两个分度，使得$G$是$G_{\lambda \mu} = G'_\lambda \cap G''_\mu$的直和，则这些子群形式是型$\Delta_1, \Delta_2$的大分度$G$，其中$(G'_\lambda)$和$(G''_\mu)$为部分刻度。我们留给读者将其推广到 $\Delta$ 是集合的有限乘积的情况。

(4) 令$\Delta_0$为可加写的交换幺半群，单位元素用0表示；设$I$为任意集合，且$\Delta_0^{(I)} = \Delta$表示有限支撑的$(\lambda_i)_{i \in I}$族的乘积$\Delta_0^I$由……组成中的子幺半群。令 $\rho : \Delta \to \Delta_0$ 为 $\Delta$ 到由 $\rho((\lambda_i)) = \sum_{i \in I} \lambda_i$ 定义的 $\Delta_0$ 的满射（共对角）同态。从型$\Delta$的每个刻度，通过$\rho$（*例2*）得出型$\Delta_0$的刻度；它被称为与给定“多重毕业”型$\Delta$相关的*总毕业*。

此号码的定义和例。 扩展立即到$G$ 是群的情况，它*不一定是可交换的*；只需要通过“受限制的和”（§ 1, no. 6，*注*）来对直和的所有概念进行替换即可。 注，在这种情况下，$G_\lambda$是正常的$G$的子群，并且对于$\lambda \neq \mu$，$G_\lambda$的每个元素可以与$G_\mu$的每个元素进行置换。

### 2. 评分为环和模

#### 定义 2 {#alg-ii-s11-def-2 .statement tag=05XZ}

*鉴于环$A$和加法群$A$上的型$\Delta$毕业$(A_\lambda)$，据说该毕业与$A$上的环结构兼容*

$$
A_\lambda A_\mu \subset A_{\lambda + \mu} \quad \text{for all } \lambda, \mu \text{ in } \Delta.
$$

*环 $A$ 具有此等级的环型 $\Delta$。*

#### 命题 1 {#alg-ii-s11-prop-1 .statement tag=05Y0}

*如果$\Delta$的每个元素都可以取消，并且$(A_\lambda)$是型$\Delta$的毕业，与环$A$的结构兼容，则$A_0$是子环的子环 $A$（尤其是$1 \in A_0$）。*

由于$A_0 A_0 \subset A_0$乘以定义，足以证明$1 \in A_0$。令 $1 = \sum_{\lambda \in \Delta} e_\lambda$ 为 1 的分解的齐次分量。如果$x \in A_\mu$，则$x = x . 1 = \sum_{\lambda \in \Delta} x e_\lambda$；比较次数$\mu$的组成部分，（因为$\mu + \lambda = \mu$意味着$\lambda = 0$）$x = x e_0$。由于这个关系对于$A$的每个齐次元素都成立，因此对于所有$x \in A$都成立；特别是$1 = 1 . e_0 = e_0 \in A_0$。

#### 定义 3 {#alg-ii-s11-def-3 .statement tag=05Y1}

*令$A$为型$\Delta$的分级环，$(A_\lambda)$其分级，$M$为左（右）$A$模块； 加法群 $M$ 上型 $\lambda$ 的毕业$(M_\lambda)$ 与$M$ 上的$A$ 模块结构兼容 if*

(2)
$$
A_\lambda M_\mu \subset M_{\lambda + \mu} \quad (\text{resp. } M_\mu A_\lambda \subset M_{\lambda + \mu})
$$
*适用于$\Delta$中的所有$\lambda, \mu$。具有此分级的模$M$则称为左（或右）分级模或型$\Delta$超过分级的环$A$。*

当$\Delta$中的元素可取消时，从(2)和命题1可得出$M_\lambda$是$A_0$模。

显然，如果$A$是型$\Delta$的分级环，则左侧$A$-模块$A_s$（分别是右侧$A$-模块$A_d$）的分级为型$\Delta$。

#### 例 {#alg-ii-s11-n2-exa-1 .statement tag=05Y2}

(1) 在任意环 $A$ 上，型 $\Delta$ 的平凡分度与环结构兼容。如果 $A$ 通过平凡分度进行分级，则为了使 $A$ 模块 $M$ 上的型 $\Delta$ 的分度 $(M_\lambda)$ 与 $A$ 模块结构兼容，$M_\lambda$ 是必要且充分的*子模* 共 $M$。

(2) 设$A$为型$\Delta$的分级环，$M$为型$\Delta$的分级$A$模，以及$\Delta$的$\rho$同态为可交换幺半群$\Delta'$，其单位元素用0表示。那么$A$是型$\Delta'$的分级环，$M$是型$\Delta'$的分级模，对于以下的毕业型 $\Delta'$ 由 $\rho$ 以及 $A$ 和 $M$ 上的型 $\Delta$ 的分度通过 no. 1 的过程得出，*例* 1：这紧随关系 $\rho(\lambda + \mu) = \rho(\lambda) + \rho(\mu)$。

特别是，如果 $\Delta = \Delta_1 \times \Delta_2$ 是两个可交换幺半群的乘积，则投影 $\mathrm{pr}_1$ 和 $\mathrm{pr}_2$ 是同态，相应的刻度只是从型 $\Delta$ 的刻度导出的*部分刻度* （no. 1，*例* 3）；因此，这些部分刻度与$A$的环结构和$M$的模结构兼容。

类似地，如果$\Delta = \Delta_0^{(r)}$（其中$\Delta_0$是交换幺半群，单位元素用0表示），则型$\Delta_0$的*总毕业*（no. 1，例4）源自型的毕业$A$ 上的$\Delta$（或$M$）通过余对角线同态与$A$ 上的环结构兼容（或$M$ 上的模结构）。

(3) 设$A$为型$\Delta$的分级环，$M$为型$\Delta$的分级$A$模，以及$\Delta$的$\lambda_0$元素；对于所有$\lambda \in \Delta$，令$M'_\lambda = M_{\lambda + \lambda_0}$和$M'$为$\mathbf{Z}$-模块$\bigoplus_{\lambda \in \Delta} M'_\lambda$。由于$A_\lambda M'_\mu \subset M_{\lambda + \mu + \lambda_0} = M'_{\lambda + \mu}$，$M'$是$A$模块，$M'$上的$M'_\lambda$形式具有型$\Delta$的刻度，与$M'$的$A$模块结构兼容；由此定义的型$\Delta$的分级$A$-模块$M'$据说是通过将$M$的分级移位$\lambda_0$获得的，并用$M(\lambda_0)$表示。当$\Delta$为群时，分级$A$模块$M'$的底层$A$模块被标识为$M$。

*(4) 设$B$为交换环。 多项式环 $B[X]$ 在一项不定中由子群 $BX^n$ ($n \geqslant 0$) (cf. III, § 2, no. 9 和 IV) 分级为型 $\mathbf{N}$。*

*(5) 设$B$为交换环，$E$为$B$模，$Q$为$E$上的二次方形式以及$C(Q)$$Q$的克利福德代数 （cf.IX, § 9）。 $C(Q)$上的子$B$模块$C^+(Q)$和$C^-(Q)$形式，型$\mathbf{Z}/2\mathbf{Z}$的毕业与$C(Q)$上的环结构兼容。*

#### 注 {#alg-ii-s11-n2-rem-1 .statement tag=05Y3}

(1) 最常用的刻度为型 $\mathbf{Z}$ 或型 $\mathbf{Z}^n$；当我们谈到分级（或二分级、三分级等）模和环而不提及型时，可以理解，我们指的是型$\mathbf{Z}$（或$\mathbf{Z}^2, \mathbf{Z}^3$等）； 型 $\mathbf{N}$ 的分级环（分别为模）也称为具有正次数的分级环（分别为模）。

(2) 型 $\Delta$的分级$\mathbf{Z}$模，当$\mathbf{Z}$有平凡毕业时，就是定义 1的分级交换律群（次数的集合是交换幺半群） （no. 1）。

#### 定义 4 {#alg-ii-s11-def-4 .statement tag=05Y4}

*令$A, A'$为相同型$\Delta$和$(A_\lambda), (A'_\lambda)$各自等级的两个等级环。如果 $h(A_\lambda) \subset A'_\lambda$ 对于所有 $\lambda \in \Delta$，环同态 $h : A \to A'$ 称为分级。

令$M, M'$为型$\Delta$的两个分级模，超过型$\Delta$的分级环。令$u : M \to M'$为$A$同态，且$\delta$元素为$\Delta$；如果所有 $\lambda \in \Delta$ 都有 $u(M_\lambda) \subset M_{\lambda + \delta}$，则$u$ 被称为次数 $\delta$ 分级。

令$A$为型$\Delta$的分级环，$A'$为型$\Delta'$和$\rho : \Delta \to \Delta'$同态的分级环。如果 $h$ 是型 $\Delta'$ 的分级环的分级同态，则环同态 $h : A \to A'$ 称为分级，当 $A$ 的分级为型时$\Delta'$ 由型 $\Delta$ 的分度通过$\rho$ (no. 1, 例 2) 导出；因此，这意味着 $h(A_\lambda) \subset A'_{\rho(\lambda)}$ 对于所有 $\lambda \in \Delta$。

如果存在$\delta \in \Delta$使得$u$的分级为次数$\delta$，则$A$同态$u : M \to M'$称为分级。如果$u \neq 0$和$\Delta$中的每个元素可取消，则$u$中的次数$\delta$被唯一确定。

如果$h : A \to A', h' : A' \to A''$是型$\Delta$分级环的两个分级同态，$h' \circ h : A \to A''$也是如此；为了使映射 $h : A \to A'$ 成为分级的环同构，$h$ 是双射且 $h$ 和逆映射 $h'$ 分级为同态是充分必要的； $h$ 是分级同态的双射也足够了。由此可见，分级同态可取为型$\Delta$分级环结构的类的态射（*集合理论*，IV, § 2, no. 1）。

类似地，如果$u : M \to M'$和$u' : M' \to M''$分别是型$\Delta$的分级A-模和次数$\delta$和$\delta'$的两个分级同态，则$u' \circ u : M \to M''$是同态的分级同态次数$\delta + \delta'$。如果 $\delta$ 在 $\Delta$ 中存在逆元 $-\delta$，并且 $u : M \to M'$ 是分级为同态的双射，次数 $\delta$，则逆元映射 $u' : M' \to M$ 是分级为同态的双射次数$-\delta$。由上可知，次数*0的*分级同态可取为型$\Delta$的分级A-模的类的态射。但是，如果 $M$ 和 $N$ 非零且 $\Delta$ 的元素可以取消，则次数 $\neq 0$ 分级的同态 $u : M \to N$ 不是分级的 A-模同构。

#### 例 {#alg-ii-s11-n2-exa-2 .statement tag=05Y5}

(6) 如果$M$是分级A-模，$M(\lambda_0)$是通过平移(no. 2, *例 3*)得到的分级A-模，则$M(\lambda_0)$到$M$的$\mathbf{Z}$线性映射为每个$M_{\lambda + \lambda_0}$上的重合和典范嵌入是次数$\lambda_0$的分级同态（当$\Delta$是*群*时，它是双射的）。

(7) 如果$a$是次数$\delta$属于到$A$的中心的齐次元素，则任何分级的A-模$M$的位似$x \mapsto ax$是评分为同态，共次数$\delta$。

*注* (3) 如果*均匀* 元素存在$M$ 由……组成的基 $(m_i)_{i \in I}$，则分级A-模 $M$ 称为*分级自由A-模*。假设是，并且 $\Delta$ 是可交换的 *群*；令$\lambda_i$为$m_i$的次数，并考虑每个$i$移位的A-模$A(-\lambda_i)$（no. 2，*例3*）；如果 $e_i$ 表示 $A$ 中的元素 1，则视为 $A(-\lambda_i)$、A-线性映射 $u : \bigoplus_{i \in I} A(-\lambda_i) \to M$ 中次数* $\lambda_i$ 的元素 *，使得 $u(e_i) = m_i$ 对于所有$i$，是*分级A-模同构*。

假设始终$\Delta$是可交换的群，现在让$N$是$N$的*齐次*生成元的分级A-模、$(n_i)_{i \in I}$系统，并假设$n_i$是次数 $\mu_i$。然后 A-线性映射 $v : \bigoplus_{i \in I} A(-\mu_i) \to N$，使得所有 $i$ 的 $u(e_i) = n_i$ 是次数* 0 的 *满射分级 A-模同态。如果 $N$ 是分级 A-模的 *有限生成*，则总有一个有限$N$的齐次生成元的系统，因此上面的型有满同态，其中$I$*有限*。

### 3. 评分子模

#### 命题 2 {#alg-ii-s11-prop-2 .statement tag=05Y6}

*令A为型$\Delta$的分级环，M为型$\Delta$的分级A-模，$(M_\lambda)$其分级，N为M的子A模块。以下属性是等效的：*

(a) $N$ *是家庭的和* $(N \cap M_\lambda)_{\lambda \in \Delta}$。
(b) *N 属于到 N* 的每个元素的均质成分。
(c) $N$ *由齐次元素*生成。

N 的每个元素都可以唯一地写为$M_\lambda$ 的元素的和，因此直接的 (a) 和(b) 是等价的，并且(a) 蕴涵(c)。我们证明（c）蕴涵（b）。然后令$(x_i)_{i \in I}$为N的齐次生成元$\neq 0$族，并令$\delta(i)$为$x_i$的次数。 N 中的每个元素都可以写成 $\sum_i a_i x_i$ 和 $a_i \in A$；如果$a_{i,\lambda}$是次数$\lambda$的$a_i$的分量，则从关系得出结论

$$
\sum_{i \in I} \left( \sum_{\mu \in \Delta} a_{i,\mu} x_i \right) = \sum_{\lambda \in \Delta} \left( \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i \right).
$$

**注 (1)** 在上面的记号中，关系$\sum_{i \in I} a_i x_i = 0$因此相当于关系$\sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i = 0$的系统。当$\Delta$是群时，这些关系可以写成$\sum_{i \in I} a_{i,\lambda - \delta(i)} x_i = 0$。

当M的子模 N具有命题 2中所述的等价性质时，显然$N \cap M_\lambda$ 形式与N的A-模结构兼容的分级，称为M上的“引起的分级”；具有此等级的 N 称为 M 的 *等级子模*。

#### 推论 1 {#alg-ii-s11-prop-2-cor-1 .statement tag=05Y7}

*如果N是M的分级子模且$(x_i)$是N的生成的系统，则N的$x_i$形式生成的系统的均质成分。*

#### 推论 2 {#alg-ii-s11-prop-2-cor-2 .statement tag=05Y8}

*如果 N 是 M 的有限生成的子模，N 承认齐次元素的有限生成系统由……组成。*

应用推论 1 即可，注意到 M 的元素仅具有有限的数齐次分量 $\neq 0$。

$A_s$（或$A_d$）的分级子模称为分级环A的*分级左*（或*右*）*理想*。对于$A(B \cap A_\lambda)(B \cap A_\mu) \subset B \cap A_{\lambda+\mu}$的每个子环B；如果 B 是 A 的*分级子$\mathbf{Z}$-模块*，则 A 上的分级在 B 上引起的分级因此与 B 上的环结构兼容； B 则被称为 A 的*分级子环*。

显然，如果 N（分别为 B）是 M 的分级子 A 模块（分别为 A 的分级子环），则典范嵌入 $N \to M$（分别为 $B \to A$）为模同态为次数 0（分别为 a评分环同态）。

如果N是分级A-模M的分级子模和$(M_\lambda)_{\lambda \in \Delta}$M的分级，则$M/N$形式的子模$(M_\lambda + N)/N$与该商模的结构兼容的*分级*。因为，如果$N_\lambda = M_\lambda \cap N$、$(M_\lambda + N)/N$与$M_\lambda/N_\lambda$相同，并且从命题2和§ 1, no. 6、公式(26)可以得出，$M/N$是它们的直和。而且，

$$
A_\lambda(M_\mu + N) \subset A_\lambda M_\mu + N \subset M_{\lambda+\mu} + N
$$
因此$A_\lambda((M_\mu + N)/N) \subset (M_{\lambda+\mu} + N)/N$，它建立了我们的断言。

。分度 ((M_\lambda + N)/N)_{\lambda \in \Delta} 称为 M 与 N 的商分度，以该分度的商模 M/N 称为 M 除以子模 N 的分度商模； 典范同态 M \to M/N 是本次毕业的同态次数 0。

如果b是A的分级双边理想，则A/b上的商分级与A/b上的环结构兼容；具有此分级的环 A/b 称为 A 除以 b 的商环； 典范同态 A \ 到 A/b 是本次毕业评分环的同态。

#### 命题 3 {#alg-ii-s11-prop-3 .statement tag=05Y9}

*设 A 为型 \Delta 的分级环，M、N 为型 \Delta 的两个分级 A-模，u: M \to N 为次数 \delta 的分级 A 同态。然后：*
(i) Im(u) 是 N 的分级子模。
(ii) *如果 \delta 是 \Delta 的正则元素，则 Ker(u) 是 M 的分级子模。*
(iii) *如果 \delta = 0，则双射 M/Ker(u) \to Im(u) 与 u 规范相关，是分级模的同构。*

断言 (i) 紧随定义和命题 2(c)。如果 x 是 M 的元素，使得 u(x) = 0 且 x = \和_\lambda x_\lambda 是其分解的齐次分量（其中 x_\lambda 是次数 \lambda），则
$$
\sum_\lambda u(x_\lambda) = u(x) = 0
$$
u(x_\lambda) 为次数 \lambda + \delta；如果 \delta 是正则关系 \lambda + \delta = \mu + \delta 意味着 \lambda = \mu，因此 u(x_\lambda) 是 u(x) 的齐次分量，并且对于 \Delta 中的所有 \lambda \ 必然 u(x_\lambda) = 0，这证明了 (ii)。 双射 v: M/Ker(u) \to Im(u) 与 u 规范关联，则为次数 \delta 的分级同态，如下从商分级的定义得出； 从而 (iii) 当 δ = 0 时。

#### 推论{#alg-ii-s11-n3-cor-1 .statement tag=05YA}

*设 A、B 为型 \Delta 的两个分级环，u：A \to B 为分级环的分级同态。那么 Im(u) 是 B 的分级子模，Ker(u) 是 A 的分级双面理想，并且双射 A/Ker(u) \to Im(u) 与 u 规范相关，是分级环的同构。*

应用命题 3 足以将 u 视为分级 \mathbf{Z} 模块的次数 0 的同态 。

#### 命题 4 {#alg-ii-s11-prop-4 .statement tag=05YB}

*设 A 为型 \Delta 的分级环，M 为型 \Delta 的 A-模。*
(i) *M 的分级子模中的每个和和每交都是一个分级子模。*
(ii) *如果 x 是次数 \mu 的 M 的齐次元素，并且可以在 \Delta 中消去，则 x 的湮没子是 A 的分级左理想。*
(iii) *如果 \Delta 的所有元素均可取消，则 M 的分级子模的湮没子是 A 的分级双面理想。*

如果$(\mathbf{N}_i)$是$M$的分级子模族，则命题2的性质(c)证明$\mathbf{N}_i$的和是由齐次元素生成，命题2的性质(b)证明齐次$\bigcap_i \mathbf{N}_i$ 属于至 $\bigcap_i \mathbf{N}_i$ 的每个元素的分量； 从而（一）。

为了证明(ii)，注满足$\operatorname{Ann}(x)$是$A$-模块$A_s$到$M$的同态$a \mapsto ax$的核并且这个同态的等级为次数 $\mu$；结论来自命题 3(ii)。 最后，（iii）是（i）和（ii）的推论，$M$的分级子模$N$的湮没子是$N$的齐次元素的湮没子交，凭借命题2。

#### 注 2 {#alg-ii-s11-n3-rem-2 .statement tag=05YC}

Let $M$ be a graded $A$-module and $E$ a submodule of $M$; it follows from Proposition 4(i) that there exists a *largest* graded submodule $N'$ of $M$ contained in $E$ and a *smallest* graded submodule $N''$ of $M$ containing $E$; $N'$ is the set of $x \in E$ all of whose homogeneous components belong to $E$ and $N''$ is the submodule of $M$ generated by the homogeneous components of a generating system of $E$.

#### 命题 5 {#alg-ii-s11-prop-5 .statement tag=05YD}

*令$A$为型$\Delta$的分级环。如果$\Delta$的每个元素都是可取消的，那么，对于每个齐次元素$a \in A$，$A$（I, § 1, no. 5）中$a$的中心化器是$A$的分级子环。*

假设$a$为次数$\delta$；令 $b = \sum_\lambda b_\lambda$ 为元素可置换，$a$，$b_\lambda$ 为所有 $\lambda \in \Delta$ 的次数 $\lambda$ $b$ 的齐次分量。那么由假设$\sum_\lambda (ab_\lambda - b_\lambda a) = 0$和$ab_\lambda - b_\lambda a$齐次的次数$\lambda + \delta$；由于$\delta$是可取消的，因此$ab_\lambda = b_\lambda a$适用于所有$\lambda$，这证明了我们的断言。

#### 推论{#alg-ii-s11-n3-cor-2 .statement tag=05YE}

*如果$\Delta$的每个元素都是可取消的，则$A$的分级子环$B$（特别是$A$的中心）的集中器是$A$的分级子环。*

它是$B$的齐次元素的中心化子交。

Remark (3) *A direct system $(A_\alpha, \phi_{\beta\alpha})$ of graded rings of type $\Delta$ (resp. a direct system $(M_\alpha, f_{\beta\alpha})$ of graded $A_\alpha$-modules of type $\Delta$) is a direct system of rings (resp. $A_\alpha$-modules) such that each $A_\alpha$ (resp. $M_\alpha$) is graded of type $\Delta$ and each $\phi_{\beta\alpha}$ (resp. $f_{\beta\alpha}$) is a *homomorphism of graded rings* (resp. an *$A_\alpha$*-homomorphism of degree 0 of *graded modules*). 如果$(A^\lambda_\alpha)_{\lambda \in \Delta}$（或$(M^\lambda_\alpha)_{\lambda \in \Delta}$）是$A_\alpha$（或$M_\alpha$）的毕业，我们写

$$
A = \lim_{\longrightarrow} A_\alpha,\quad A^\lambda = \lim_{\longrightarrow} A^\lambda_\alpha \quad (\text{resp. } M = \lim_{\longrightarrow} M_\alpha,\ M^\lambda = \lim_{\longrightarrow} M^\lambda_\alpha),
$$

从 § 6, no. 2、命题 5 可以得出，$(A^\lambda)$（分别为 $(M^\lambda)$）是 A 级（分别为 M），并且可以从 I, § 10、第 5 个得出。 3 和 4 表明该刻度与 A 上的环结构兼容（分别与 M 上的 A-模结构）。分级的环 A（分别分级为A-模 M）称为分级环 $(A_\alpha, \phi_{\beta\alpha})$（分别分级为模 $(M_\alpha, f_{\beta\alpha})$）的直接系统的直极限。如果$\phi_\alpha : A_\alpha \to A$（分别$f_\alpha : M_\alpha \to M$）为典范映射，则$\phi_\alpha$（分别$f_\alpha$）为分级环的同态（分别为分级$A_\alpha$模块的次数0的同态）。

### 4. 有序群 OF 次数的情况

如果对于所有 $\rho \in \Delta$，关系 $\lambda \leq \mu$ 隐含$\lambda + \rho \leq \mu + \rho$，则可加地编写的可交换群 $\Delta$ 上的阶结构（由 $\leq$ 表示）被认为与群结构 *相容的*。 群 $\Delta$ 与阶结构则称为*有序群*。我们将在VI, § 1详细研究这些群；这里我们将自己限制为注，在这种情况下，群关系$\lambda > 0$意味着所有$\mu$的$\lambda + \mu > \mu$，因为它通过定义暗示$\lambda + \mu \geq \mu$，并且关系$\xi + \mu = \mu$相当于$\xi = 0$。

令$\Delta$为有序交换群，A为型$\Delta$的分级环和$(A_\lambda)$其分级，并假设关系$A_\lambda \neq \{0\}$蕴涵$\lambda \geq 0$；那么根据上面的注，从定义可以得出，$\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$是A的*分级双边理想*。

#### 命题 6 {#alg-ii-s11-prop-6 .statement tag=05YF}

*令$\Delta$为有序交换群，A为型$\Delta$的环，$(A_\lambda)$其毕业，M为型$\Delta$的A-模和$(M_\lambda)$其毕业。假设关系$A_\lambda \neq \{0\}$蕴含$\lambda \geq 0$，并且存在$\lambda_0$使得$M_{\lambda_0} \neq \{0\}$和$M_\lambda = \{0\}$对应于$\lambda < \lambda_0$。那么，如果 $\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$，$\mathfrak{I}_0 M \neq M$.*

令$x$为$M_{\lambda_0}$的非零元素；假设$x \in \mathfrak{I}_0 M$。然后$x = \sum_i a_i x_i$，其中$a_i$是$\mathfrak{I}_0$的同质元素$\neq 0$，以及M的$x_i$同质元素$\neq 0$，对于所有$i$（no. 2），$\deg(x) = \deg(a_i) + \deg(x_i)$。但是，如$\deg(a_i) > 0$、$\lambda_0 = \deg(a_i) + \deg(x_i) > \deg(x_i)$，即与……矛盾假设。

#### 推论 1 {#alg-ii-s11-prop-6-cor-1 .statement tag=05YG}

*假设$\Delta$和A为命题6，如果M是有限生成的分级A-模，使得$\mathfrak{I}_0 M = M$，则$M = \{0\}$。*

假设$M \neq \{0\}$。设$\lambda_0$为齐次元素$\neq 0$M由……组成有限生成系统次数集合的最小元素；那么命题6的假设就得到满足，这意味着矛盾。

#### 推论 2 {#alg-ii-s11-prop-6-cor-2 .statement tag=05YH}

*假设$\Delta$和A为命题6，令M为有限*生成的分级$\mathbf{A}$模块，且$\mathbf{N}$为$\mathbf{M}$的分级子模，使得$\mathbf{N} + \mathfrak{J}_0 \mathbf{M} = \mathbf{M}$；然后$\mathbf{N} = \mathbf{M}$。

$\mathbf{M}/\mathbf{N}$是有限生成的分级$\mathbf{A}$模块，假设意味着$\mathfrak{J}_0 . (\mathbf{M}/\mathbf{N}) = \mathbf{M}/\mathbf{N}$；因此$\mathbf{M}/\mathbf{N} = 0$。

#### 推论 3 {#alg-ii-s11-prop-6-cor-3 .statement tag=05YI}

*根据命题 6 的$\Delta$ 和$\mathbf{A}$ 的假设，令$u : \mathbf{M} \to \mathbf{N}$ 为分级右$\mathbf{A}$ 模块的分级同态，其中$\mathbf{N}$ 假设为有限生成。如果同态*

$$
u \otimes 1 : \mathbf{M} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) \to \mathbf{N} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

*是满射，那么 $u$ 是满射。*

$u(\mathbf{M})$ 是 $\mathbf{N}$ 的分级子模和 $(\mathbf{A}/\mathfrak{J}_0)$ 模块

$$
(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

与 $(N \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0))/\mathrm{Im}(u \otimes 1)$ (§ 3, no. 6, 命题 6) 同构的。因此，根据推论 1，假设意味着$(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) = 0$，进而意味着$\mathbf{N} = u(\mathbf{M})$。

#### 注 {#alg-ii-s11-n4-rem-1 .statement tag=05YJ}

从推论 1 的证明可知，当不假设 $\mathbf{M}$（分别为 $\mathbf{N}$）是有限生成时，推论 1 和 2（或推论 3）仍然有效，而是得出以下假设：存在子集 $\Delta^+$ $\Delta$满足以下条件：

(1) 对于$\lambda \notin \Delta^+$、$M_\lambda = \{0\}$（分别为$N_\lambda = \{0\}$）；
(2) $\Delta^+$ 中的每个非空子集至少有元素。

如果 $\Delta = \mathbf{Z}$ 和 $\mathbf{M}$（分别为 $\mathbf{N}$）是评分为模并具有*正* 次数，则会出现这种情况。

#### 命题 7 {#alg-ii-s11-prop-7 .statement tag=05YK}

*假设$\Delta = \mathbf{Z}$。根据$\mathbf{A}$和$\mathbf{M}$为命题 6的假设，考虑分级$\mathbf{A}_0$-模块$\mathbf{N} = \mathbf{M}/\mathfrak{J}_0 \mathbf{M}$并假设以下条件成立：
(i) 每个被视为$\mathbf{A}_0$模块的$N_\lambda$都承认基$(y_{i\lambda})_{i \in I_\lambda}$；
(ii) 典范同态 $\mathfrak{J}_0 \otimes_{\mathbf{A}} \mathbf{M} \to \mathbf{M}$ 是单射的。

那么$\mathbf{M}$是一个分级的免费$\mathbf{A}$-模块（no. 2，注3），准确地说，如果$x_{i\lambda}$是$M_\lambda$的元素，而$N_\lambda$中的像是$y_{i\lambda}$，那么这个族$(x_{i\lambda})_{(i, \lambda) \in I}$（其中$I$是$I_\lambda$的集合和）是$\mathbf{M}$的基。*

我们知道（no. 2，*注 3*）有一个分级免费$\mathbf{A}$-模块$\mathbf{L}$（毕业$(L_\lambda)$）和满同态$p : \mathbf{L} \to \mathbf{M}$的次数0，这样$p(e_{i\lambda}) = x_{i\lambda}$对于所有$(i, \lambda) \in I$（$(e_{i\lambda})_{(i, \lambda) \in I}$为同质元素$e_{i\lambda} \in L_\lambda$的$\mathbf{L}$由……组成基）。从上面的*注*得出$p$是*满射*。考虑分级的$\mathbf{A}$-模块$\mathbf{R} = \mathrm{Ker}(p)$和注，$R_\lambda = \{0\}$对于$\lambda < \lambda_0$乘定义；我们需要证明$\mathbf{R} = \{0\}$，到命题 6就足以证明$\mathfrak{J}_0 R = R$。考虑交换性图表 (§ 3, no. 6, 命题 5)

$$
\begin{array}{ccccccccc}
\mathfrak{J}_0 \otimes R & \xrightarrow{1 \otimes j} & \mathfrak{J}_0 \otimes L & \xrightarrow{1 \otimes p} & \mathfrak{J}_0 \otimes M & \longrightarrow & 0 \\
\downarrow a & & \downarrow b & & \downarrow c & & \\
0 & \longrightarrow & R & \xrightarrow{f} & L & \xrightarrow{p} & M & \longrightarrow & 0
\end{array}
$$

其中$j$是典范嵌入，$a, b, c$源自典范嵌入$\mathfrak{J}_0 \to A$（§ 3, no. 4，命题4）；必须证明 $a$ 是满射的。 注，由于$L$是自由的，$b$是单射的（§ 3, no. 7，推论6到命题 7），并且$c$是假设的单射。则令$t$为$R$中的元素，且$t$为$R / \mathfrak{J}_0 R$中的类；那么就有正合序列（§ 3, no. 6、命题 5 以及推论 2 到命题 6）

$$
R / \mathfrak{J}_0 R \xrightarrow{j} L / \mathfrak{J}_0 L \xrightarrow{\bar{p}} M / \mathfrak{J}_0 M \longrightarrow 0
$$

where $j$ and $\bar{p}$ derive from $j$ and $p$ when passing to the quotients and $\bar{p}$ is by hypothesis a bijection; then $j(\bar{t}) = 0$, in other words $j(t) \in \mathfrak{J}_0 L$. 那么有元素$z \in \mathfrak{J}_0 \otimes L$使得$j(t) = b(z)$；作为 $p(b(z)) = 0$、$c((1 \otimes p)(z)) = 0$，并且由于 $c$ 是单射的，$(1 \otimes p)(z) = 0$。 在其他字中，$z$是$1 \otimes j$下元素$t' \in \mathfrak{J}_0 \otimes R$的像，然后是$j(a(t')) = b(z) = j(t)$；由于$j$是单射的，这意味着$t = a(t')$。

我们稍后将展示（交换代数，II, § 3, no. 2，命题 5）如何将这个命题扩展到非分级模。

#### 引理 1 {#alg-ii-s11-lem-1 .statement tag=05YL}

*对于交换性群$\Delta$，$\Delta$上存在与$\Delta$的群结构兼容的全序，$\Delta$无扭转是必要且充分的。*

如果$\Delta$上存在这样的阶结构并且$\lambda > 0$，则对于所有$\mu \geq 0$存在$\lambda + \mu > 0$，特别是整数$n > 0$，$n.\lambda > 0$上的归纳，这证明$\Delta$是无扭转（因为 $\Delta$ 的每个元素 $\neq 0$ 要么是 $> 0$ 要么 $< 0$）。 Conversely, if $\Delta$ is torsion-free, $\Delta$ is a sub-$\mathbf{Z}$-module of a vector $\mathbf{Q}$-space (§ 7, no. 10, Corollary 1 to Proposition 26) which may be assumed of the form $\mathbf{Q}^{(I)}$; if $I$ is given a well-ordering (*Set Theory*, III, § 2, no. 3, Theorem 1) and $\mathbf{Q}$ its usual ordering, the set $\mathbf{Q}^{(I)}$ with the *lexicographical ordering* is totally ordered (*Set Theory*, III, § 2, no. 6); it is immediate that this ordering is compatible with the additive group structure of $\mathbf{Q}^{(I)}$.

#### 命题 8 {#alg-ii-s11-prop-8 .statement tag=05YM}

*令$\Delta$为无扭交换律群，而$A$为型$\Delta$的分级环。如果两个齐次元素$\neq 0$的$A$中的乘积为$\neq 0$，则环$A$没有0的除子。*

让 $\Delta$ 得到与其群结构 (引理

1) 令$x = \sum_{\lambda \in \Delta} x_\lambda, y = \sum_{\lambda \in \Delta} y_\lambda$为$A$的两个非零元素（$x_\lambda$和$y_\lambda$对于所有$\lambda \in \Delta$来说是次数$\lambda$的齐次）；令$\alpha$（或$\beta$）为元素$\lambda \in \Delta$的最大的，使得$x_\lambda \neq 0$（或$y_\lambda \neq 0$）；如果$\lambda \neq \alpha$或$\mu \neq \beta$，则$x_\lambda y_\mu = 0$或$\deg(x_\lambda y_\mu) < \alpha + \beta$为直接的；因此，次数 $\alpha + \beta$ 的$xy$的齐次分量为$x_\alpha y_\beta$，其非零假设； 从而$xy \neq 0$。

### 5. 已评分张量积已评分模

令 $\Delta$ 为可交换幺半群，其单位元素表示为 0，$A$ 为型 $\Delta$ 的分级环，$M$（或$N$）为分级右（或左） $A$-型$\Delta$的模块。令$(A_\lambda)$（或$(M_\lambda), (N_\lambda)$）为$A$（或$M, N$）的毕业； $\mathbf{Z}$模块$M$和$N$的张量积$M \otimes_{\mathbf{Z}} N$是$M_\lambda \otimes_{\mathbf{Z}} N_\mu$（§ 3, no. 7，命题7）的直和，因此后者形式是型$\Delta, \Delta$在此$\mathbf{Z}$模块上。考虑$M \otimes_{\mathbf{Z}} N$与本次大毕业相关的型$\Delta$的*总毕业*（no. 1，*例4*）；它由子$\mathbf{Z}$模块$P_\lambda = \sum_{\mu + \nu = \lambda} (M_\mu \otimes_{\mathbf{Z}} N_\nu)$组成。已知$\mathbf{Z}$模$M \otimes_A N$是元素$(xa) \otimes y - x \otimes (ay)$生成的子$\mathbf{Z}$模$Q$与$M \otimes_{\mathbf{Z}} N$的商，其中$x \in M, y \in N$和$a \in A$(§ 3, no. 1)；如果对于所有$\lambda \in \Delta$，$x_\lambda, y_\lambda, a_\lambda$分别是$x, y, a$的次数$\lambda$的齐次分量，显然$(xa) \otimes y - x \otimes (zy)$是齐次元素$(x_\lambda a_\nu) \otimes y_\mu - x_\lambda \otimes (a_\nu y_\mu)$的和，在其他字 $Q$ 是 $M \otimes_{\mathbf{Z}} N$ (no. 3, 命题 2) 的*分级*子$\mathbf{Z}$模块和商

$$
M \otimes_A N = (M \otimes_{\mathbf{Z}} N)/Q
$$

因此，标准的分级 $\mathbf{Z}$ 模块结构为型 $\Delta$ (no. 3)。 Moreover (no. 3, Proposition 5), the *centre* $C$ of $A$ is a graded subring of $A$; the graduation which we have just defined on $M \otimes_A N$ is *compatible with its module structure over the graded ring* $C$. 对于 $M \otimes_{\mathbf{Z}} N$ 来说，具有规范的*两个* $C$ 模块结构，对于 $x \in M, y \in N, c \in C$ (§ 3, no. 3) 分别有 $c(x \otimes y) = (xc) \otimes y$ 和 $(x \otimes y)c = x \otimes (cy)$；如果$x \in M_\lambda, y \in N_\mu, c \in C \cap A_v$，则两个元素$c(x \otimes y)$和$(x \otimes y)c$属于到$(M \otimes_{\mathbf{Z}} N)_{\lambda + \mu + v}$以及它们的差属于到$Q$，因此它们在$M \otimes_A N$属于中的公共的像到$(M \otimes_A N)_{\lambda + \mu + v}$，这建立了我们的断言。 当我们将$M \otimes_A N$称为*分级*$C$-*模*时，我们总是指这样定义的结构，另外提到的除非。 注，$(M \otimes_A N)_\lambda$可以定义为由$x_\mu \otimes y_\nu$生成的$M \otimes_A N$的加法群，其中$x_\mu \in M_\mu, y_\nu \in N_\nu$和$\mu + \nu = \lambda$。

令$M'$（分别$N'$）分别为次数、$\alpha$和$\beta$的另一个分级为右（分别为左）$A$模块，并且$u : M \to M', v : N \to N'$分级为同态。那么从上面的注可以立即得出$u \otimes v$是次数$\alpha + \beta$的*分级*（C-模）同态。

当$A$可交换时，在任何有限数分级$A$-模的张量积上类似地定义分级（与$A$-模结构兼容）；另外，$(M \otimes N) \otimes P \to M \otimes (N \otimes P)$($§ 3$、no. 8、命题8)等结合性同构、直接的、*分级*模的同构。

#### 注 {#alg-ii-s11-n5-rem-1 .statement tag=05YN}

当$A$具有*平凡*分级（no. 1，*例* 1）时，$(M \otimes_A N)_\lambda$只是$M \otimes_A N$的子$Y$模块$M_\mu \otimes_A N_\nu$的直和，使得$\mu + \nu = \lambda$。

令$M$（分别$N$）为型$\Delta$的分级右（或左）$A$模块，$P$为型$\Delta$的分级$\mathbf{Z}$模块，并令$f$为$M \times N$到$§ 3$、no. 1的$P$、满足条件 (1) 的$\mathbf{Z}$双线性映射，此外还有
$$
f(x_\lambda, y_\mu) \in P_{\lambda+\mu} \quad \text{for } x_\lambda \in M_\lambda, y_\mu \in N_\mu, \lambda, \mu \text{ in } \Delta.
$$
然后是$f(x, y) = g(x \otimes y)$，其中$g : M \otimes_A N \to P$是$\mathbf{Z}$线性映射（$§ 3$，no. 1，命题1），并且从上面的条件可以得出$g$是一个*分级*$\mathbf{Z}$-模块同态共次数 0。

设$B$为型$\Delta$的另一个分级环，以及环的$\rho : A \to B$同态（no. 2）；那么$\rho^*(B_d)$是型$\Delta$的分级右$A$模。如果$E$是型$\Delta$的分级左$A$-模块，并且$\rho^*(B_d) \otimes_A E$给出了上面定义的型$\Delta$的分级$\mathbf{Z}$-模块结构，则规范的左$B$-模块结构（$§ 5$， no. 1) 与毕业兼容
$$
E_{(B)} = \rho^*(E) = \rho^*(B_d) \otimes_A E.
$$
由此获得的分级$B$模块据说是通过将标量的环通过$\rho$扩展到$B$而获得的，当我们将$E_{(B)}$或$\rho^*(E)$称为分级$B$模块时，我们总是指这个结构， 除非另有提及。

### 6. 已评分模已评分同态

我们假设在这个没有。幺半群 $\Delta$ 是 *群*。 令$A$为型$\Delta$的分级环和$M, N$两个分级左（对于例）$A$-型$\Delta$的模块。 Let $H_\lambda$ denote the additive group of *graded homomorphisms of degree* $\lambda$ of $M$ into $N$ (no. 2); in the additive group $\mathrm{Hom}_A(M, N)$ of *all* homomorphisms of $M$ into $N$ (with the *non-graded* $A$-module structures) the sum (for $\lambda \in \Delta$) of the $H_\lambda$ is *direct*. 因为，如果对于所有 $\lambda$ 存在关系 $\sum_\lambda u_\lambda = 0$ 和 $u_\lambda \in H_\lambda$，则可以得出对于所有 $\mu$ 和所有 $x_\mu \in M_\mu$ 都有 $\sum_\lambda u_\lambda(x_\mu) = 0$。 由于$\Delta$的元素可消去，$u_\lambda(x_\mu)$是次数$\lambda + \mu$的$\sum_\lambda u_\lambda(x_\mu)$的齐次分量；因此，对于每个有序对$(\mu, \lambda)$和每个$x_\mu \in M_\mu$，$u_\lambda(x_\mu) = 0$，这意味着对于所有$\lambda \in \Delta$，$u_\lambda = 0$。 我们将（在本段中）用$\mathrm{Homgr}_A(M, N)$表示$H_\lambda$的$\mathrm{Hom}_A(M, N)$和的添加剂子群，我们将称其为$M$的*分级*$A$-*模同态*的加法群。 $N$。 令$C$为$A$的中心，这是分级的子环（no. 3，命题5的推论）；对于 $\mathrm{Hom}_A(M, N)$ 上的规范 $C$ 模块结构（$§ 1$、no. 14、*注* 1），$\mathrm{Homgr}_A(M, N)$ 是 *子模* 并且毕业 $(H_\lambda)$ 与 $C$ 模块结构*相容的*： for, if $c_v \in C \cap A_v$、$x_\mu \in N_\mu$ 和 $u_\lambda \in H_\lambda$，然后是定义 $(c_vu_\lambda)(x_\mu) = c_v.u_\lambda(x_\mu) \subset N_{\lambda+\mu+v}$，因此$c_vu_\lambda \in H_{\lambda+v}$。

令$M'$和$N'$为型$\Delta$和$u': M' \to M$的两个分级左$A$模块，$v': N \to N'$分别为次数$\alpha$和$\beta$分级同态。然后是直接的，$\mathrm{Hom}(u', v'): w \mapsto v' \circ w \circ u'$映射$\mathrm{Homgr}_A(M, N)$进入$\mathrm{Homgr}_A(M', N')$，并且其限制到$\mathrm{Homgr}_A(M, N)$是次数*$\alpha + \beta$*分级*同态进入$\mathrm{Homgr}_A(M', N')$*。

特别是$\mathrm{Homgr}_A(M, M)$是$\mathrm{End}_A(M)$的*分级子环*，用$\mathrm{Endgr}_A(M)$表示。

#### 注 {#alg-ii-s11-n6-rem-1 .statement tag=05YO}

如果 $M$ 和 $N$ 被分级为左 $A$ 模块，则 $\mathrm{Homgr}_A(M, N)$ 通常与 $\mathrm{Hom}_A(M, N)$ 不同。然而，当 $M$ 是*有限生成的* $A$ 模块时，这两个集合是相等的。因为 $M$ 是由齐次元素 $x_i$ ($1 \leq i \leq n$) 的有限数生成；设$d(i)$为$x_i$的次数；令$u \in \mathrm{Hom}_A(M, N)$，对于所有$\lambda \in \Delta$，让$z_{i,\lambda}$表示次数$\lambda + d(i)$的$u(x_i)$的齐次分量。我们证明存在同态 $u_\lambda : M \to N$，使得所有 $i$ 都存在 $u_\lambda(x_i) = z_{i,\lambda}$。足以证明，如果$\sum_i a_ix_i = 0$和$a_i \in A$对于$1 \leq i \leq n$，那么$\sum_i a_iz_{i,\lambda} = 0$对于所有$\lambda \in \Delta$（$§ 1$，no. 7，*注*）。可以假设每个 $a_i$ 都是次数 $d'(i)$ 的齐次，使得 $d(i) + d'(i) = \mu$ 对于所有 $i$ (no. 3, *注* 1)；然后$\sum_i a_iu(x_i) = 0$；对左侧取次数$\lambda + \mu$的齐次分量，可得$\sum_i a_iz_{i,\lambda} = 0$，从而存在同态$u_\lambda$；显然，$u_\lambda$的*分级*为次数$\lambda$。最后，$u_\lambda = 0$除了值与$\lambda$的有限数，以及$u = \sum_\lambda u_\lambda$乘以定义，这证明了我们的断言。

特别是，对于每个分级左$A$-模块$M$，$\mathrm{Homgr}_A(A_s, M) = \mathrm{Hom}_A(A_s, M)$；此外，$\mathrm{Hom}_A(A_s, M)$有一个*分级的左A-模*结构（而不仅仅是分级的$C$模块结构），并且直接的将$M$的结构典范映射转换为$\mathrm{Hom}_A(A_s, M)$（$§ 1$， no. 14，*注* 2) 是*分级A-模同构*。

类似地，$\mathrm{Homgr}_A(M, A_s)$有一个*分级的右A-模*结构（而不仅仅是分级的$C$模块结构）；它被称为分级$A$-模块$M$的*分级对偶*，并用$M^{*\mathrm{gr}}$表示，或者在没有混淆结果时简称为$M^*$。如果 $u : M \to N$ 是次数 $\delta$ 的分级同态，则由上可知 ${}^t u = \mathrm{Hom}(u, 1_{A_s})$ 的限制到 $N^{*\mathrm{gr}}$ 是分级对偶 $N^{*\mathrm{gr}}$ 的分级对偶同态到分级对偶中$M^{*\mathrm{gr}}$，次数$\delta$，称为$u$的*分级转置*。

我们有时考虑在分级对偶$M^{*\mathrm{gr}}$上借助$\Delta$的同构$\lambda \mapsto -\lambda$（no. 1，例2）得出的分级，以便次数$\lambda$的齐次元素 $M^{*\mathrm{gr}}$中是次数* $-\lambda$在$M$上的评分线性形式*（当$A$有微不足道的毕业时，这些是指标的$M_\mu$的零线性形式） $\mu \neq \lambda$）。然后，如果 $u : M \to N$ 是次数 $\delta$ 的分级同态，则 $u'$ 将变为次数 $-\delta$ 的分级同态。

假设$A$是*可交换的*并且分级为型$\Delta$，并令$M, N, P, Q$为四个*分级*$A$-型$\Delta$的模块。然后有 *规范分级同态或次数* 0

(3) $$
\operatorname{Homgr}_A(M, \operatorname{Homgr}_A(N, P)) \to \operatorname{Homgr}_A(M \otimes_A N, P)
$$
(4) $$
\operatorname{Homgr}_A(M, N) \otimes_A P \to \operatorname{Homgr}_A(M, N \otimes_A P)
$$
(5) $$
\operatorname{Homgr}_A(M, P) \otimes_A \operatorname{Homgr}_A(N, Q) \to \operatorname{Homgr}_A(M \otimes_A N, P \otimes_A Q)
$$
(张量积被给予no. 5中定义的刻度)通过限制§ 4中定义的典范同态获得，第100条。 1、2和4；因为，如果 $u : M \to \operatorname{Homgr}_A(N, P)$ 的评分为次数 $\delta$，则对于所有 $x \in M_\lambda$，$u(x)$ 的评分为同态 $N \to P$ 次数 $\delta + \lambda$，因此，对于 $y \in N_\mu$， $u(x)(y) \in P_{\delta + \lambda + \mu}$；如果$v : M \otimes_A N \to P$对应规范于$u$，则可以看出$v$是次数$\delta$的分级同态，从而我们的关于（3）的断言；而且可以看出，这个同态是*双射的*。 (4) 和(5) 的论证类似。

如果特别是 (5) 中的 $P = Q = A$，则存在次数 0 的规范 *分级* 同态

(6) $$
M^{*\mathrm{gr}} \otimes_A N^{*\mathrm{gr}} \to (M \otimes_A N)^{*\mathrm{gr}}.
$$

### 习题{#alg-ii-s11-exercises}

§ 11](exercises/s11/)参见[习题。
