---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 3
section_title: Graded algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 457-460, 626
pdf_pages: 0481-0484, 0650-0650
extraction: ocr
subsections:
    - "no": 1
      title: GRADED ALGEBRAS
      page: 457
      pdf_page: 481
    - "no": 2
      title: GRADED SUBALGEBRAS, GRADED IDEALS OF A GRADED ALGEBRA
      page: 459
      pdf_page: 483
    - "no": 3
      title: DIRECT LIMITS OF GRADED ALGEBRAS
      page: 460
      pdf_page: 484
statements: 4
exercises: 1
content_sha256: 4134b720c21ebc0e44e3ec6ddecbbb61c1e00f308595e50fdd4ac09faf7fc6eb
translated_from: content/en/alg/III/03_s3_graded_algebras.md
translation_method: google
source_content_sha256: d496b7e9119afe9a64c71792995d77ced2c25e2dbf7df0912c545226ff6cffa2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9d19881415a6ed27c3477d76f24a7e901a7b240231ce38b6d0d82dbcd273b438
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。评分代数

本段中考虑的毕业将具有作为次数的集合的*可交换幺半群，其单位元素由 0* 表示。

### 1. 评分代数

#### 定义 1 {#alg-iii-s3-def-1 .statement tag=0603}

*令 $\Delta$ 为可交换幺半群，$A$ 型 $\Delta$* (II, § 11, no. 2) 的分级环，$(A_\lambda)_{\lambda \in \Delta}$ *其分级和 E A-代数。 加法群 E 上的型 $\Delta$ 的毕业 * $(E_\lambda)_{\lambda \in \Delta}$ * 据说与 E 上的 A-代数结构兼容，如果它与 E 上的 A-模和环结构兼容，则在其他字中，如果对于所有$\Delta$中的$\lambda, \mu$，*

(1) $$ A_\lambda E_\mu \subset E_{\lambda + \mu} $$
(2) $$ E_\lambda E_\mu \subset E_{\lambda + \mu}. $$

*A-代数 E，有了这个分级，就被称为分级代数，分级为型 $\Delta$，分级为环 A。*

当 A 上的毕业*微不足道*（即 $\lambda \neq 0$ 的 (II, § 11, no. 1) $A_0 = A, A_\lambda = \{0\}$）时，条件 (1) 意味着 $E_\lambda$ 是 E 的 *子 A 模块*。这导致定义或概念的分级代数型$\Delta$超过*非分级*交换环$A$：$A$被赋予型$\Delta$的微不足道的分级，并且应用上述定义。

当我们考虑带有 *单位元* $e$ 的分级 $A$-代数 $E$ 时，总会理解$e$ 是次数* 0 (cf. 习题 1)。

由此可见，如果可逆元 $x \in E$ 是*齐次*且为次数 $p$，则其逆 $x^{-1}$ 为*齐次*且为次数 $-p$：足以将 $x^{-1}$ 分解为关系 $x^{-1}x = xx^{-1} = e$ 中同质元素的和。

令$E$和$E'$为型$\Delta$的两个分级代数，超过型$\Delta$的分级环$A$。如果 $u(E_\lambda) \subset E'_\lambda$ 对于所有 $\lambda \in \Delta$ 而言，$A$-代数同态 $u : E \to E'$ 被称为*分级代数同态*（其中 $(E_\lambda)$ 和 $(E'_\lambda)$ 分别表示 $E$ 和 $E'$ 的分级）；其中 $E$ 和 $E'$ 是结合且单位的，$u$ 是单位的，这个条件意味着 $u$ 是分级的环同态 (II, § 11, no. 2)。

令 $E$ 为型 $N$ 的分级 $A$ 代数。 $E$ 与型 $\mathbf{Z}$ 的分级 $A$ 代数一致，通过将 $n < 0$ 写为$E_n = \{0\}$。

#### 注 {#alg-iii-s3-n1-rem-1 .statement tag=0604}

定义 1 也可以被说解释为$E$是分级的$A$-模块并且$A$-线性映射

$$
m : E \otimes_A E \to E
$$

在 $E$ (§ 1, no. 3) 上定义乘法，当 $E \otimes_A E$ 的分级为型 $\Delta$ (II, § 11, no. 5) 时，次数* 0 是 *齐次的。

对于定义分级环$A$上的型$\Delta$的分级$A$-代数结构，以$E$作为基础分级$A$-模块，因此相当于为每个有序对进行定义$\Delta$ 元素 $(\lambda, \mu)$ $\mathbf{Z}$-双线性映射

$$
m_{\lambda \mu} : E_\lambda \times E_\mu \to E_{\lambda + \mu}
$$

这样对于指标$(\lambda, \mu, \nu)$和$\alpha \in A_\lambda,\ x \in E_\mu,\ y \in E_\nu$的每个三倍，

$$
\alpha . m_{\mu \nu}(x, y) = m_{\lambda + \mu, \nu}(\alpha x, y) = m_{\mu, \lambda + \nu}(x, \alpha y).
$$

#### 例 {#alg-iii-s3-n1-exa-1 .statement tag=0605}

(1) 令$B$为型$\Delta$的*分级环*；如果 $B$ 被赋予其规范的 $\mathbf{Z}$-代数结构 (§ 1, no. 1, *例* 2)，$B$ 是分级的 $A$-代数（$\mathbf{Z}$ 被赋予简单的毕业）。

(2) 设$A$为型$\Delta$的分级交换环，$M$为型$\Delta$的分级$A$模块。假设幺半群$\Delta$的所有元素都是*可消去*，这允许（II, § 11, no. 6）我们在$\mathrm{Homgr}_A(M, M) = \mathrm{Endgr}_A(M)$上定义一个型$\Delta$的分级$A$模块结构；由于此毕业与$\mathrm{Endgr}_A(M)$（II, § 11, no. 6）上的环结构兼容，因此定义是$A$-代数*结构在$A$-代数$\mathrm{Endgr}_A(M)$上的*统一分级。

(3) *代数岩浆。* 令 $S$ 为岩浆，$\phi : S \to \Delta$ 同态。对于所有$\lambda \in \Delta$，我们写为$S_\lambda = \phi^{-1}(\lambda)$；然后$S_\lambda S_\mu \subset S_{\lambda + \mu}$。设$A$为型$\Delta$的分级交换环，$(A_\lambda)_{\lambda \in \Delta}$为其毕业；我们将对岩浆$S$（§ 2, no. 6）的代数$E = A^{(S)}$进行定义分级$A$代数结构。为此，令$E_{\lambda}$表示由形式$\alpha.s$的元素生成的$E$的加法子群，使得$\alpha \in A_{\mu}, s \in S_{\nu}$和$\mu + \nu = \lambda$。由于$S_{\lambda}$是成对的不相交的，$E$是$A_{\mu}S_{\nu}$的直和，因此也是$E_{\lambda}$的直和，$E_{\lambda}$满足是直接的条件 (1) 和 (2)，因此定义在 $E$ 上得到所需分级的 $A$-代数结构。如果$S$承认单位元素$e$，也可以假设$\phi(e) = 0$。一种特殊情况是环 $A$ 的毕业是微不足道的；那么$E_{\lambda}$就是$S_{\lambda}$生成的$E$的子$A$模块。更具体地，如果我们采用$S = \mathbf{N}^{(I)}, \Delta = \mathbf{N}$和$\phi$映射使得$\phi((n_i)) = \sum_{i \in I} n_i$，环$A$具有平凡的分级，则因此在多项式代数$A[X_i]_{i \in I}$上获得分级，其中次数是齐次多项式$\neq 0$ 是§ 2, no. 9 (cf. § 6, no. 6) 中定义的总次数。

现在，我们将$S$作为集合$B$（I, § 7, no. 2）和$\phi$同态$Mo(B) \to \mathbf{N}$的自由幺半群$Mo(B)$，它与每个字及其长度相关联。因此，在集合 $B$ (§ 2, no. 7; cf. § 5, no. 5) 的自由结合代数上获得分级$A$-代数结构。

### 2. 分级子代数，分级代数的分级理想

令$E$为型$\Delta$的分级代数，超过型$\Delta$的分级环$A$。 If $F$ is a sub-$A$-algebra of $E$ which is a graded sub-$A$-module, then the graduation $(F_{\lambda})$ on $F$ is compatible with its $A$-algebra structure, since $F_{\lambda} = F \cap E_{\lambda}$; in this case $F$ is called a graded subalgebra of $E$ and the canonical injection $F \to E$ is a graded algebra homomorphism.

Similarly, if $a$ is a left (resp. right) ideal of $E$ which is a graded sub-$A$-module, then $E_{\lambda}a_{\mu} \subset a_{\lambda+\mu}$ (resp. $a_{\lambda}E_{\mu} \subset a_{\lambda+\mu}$), since $a_{\lambda} = a \cap E_{\lambda}$; then $a$ is called a graded ideal of the algebra $E$. 如果 $b$ 是 $E$ 的分级双面理想，则模 $E/b$ 上的商分级与 $E/b$ 上的代数结构兼容，并且典范同态 $E \to E/b$ 是分级代数同态。

如果$u : E \to E'$是分级代数同态，$\operatorname{Im}(u)$是$E'$的分级子代数，$\operatorname{Ker}(u)$是$E$的分级双边理想，而双射规范地与$u$相关联的$E/\operatorname{Ker}(u) \to \operatorname{Im}(u)$是分级的代数同构。

#### 命题 1 {#alg-iii-s3-prop-1 .statement tag=0606}

*Let $A$ be a graded 交换环 of 型 $\Delta$, $E$ a graded $A$-algebra of 型 $\Delta$ and $S$ 集合 of homogeneous 元素 of $E$。那么$S$生成的子$A$代数（分别为左理想、右理想、两侧理想）就是分级的子代数（分别为分级理想）。*。

$S$生成的$E$的子代数是$S$的元素的有限乘积生成的子$A$模，它们是齐次的；类似地，$S$生成的左（或右）理想是形式$u_1(u_2(\ldots(u_n s))\ldots)$（或$(\ldots((s u_n) u_{n-1})\ldots) u_2$）$u_1$）的元素生成的子$A$模块，其中s ∈ S和u_j ∈ E是齐次的（n任意）并且这些乘积是齐次的，从而在这种情况下是根据II, § 11, no. 3、命题 2)得出的结论；最终 S 生成的两侧理想为并或序列 (\mathfrak{I}_n)_{n \geq 1}，其中 \mathfrak{I}_1 是 S 生成的左理想，而 \mathfrak{I}_{2n} （分别为\mathfrak{I}_{2n+1}）由 \mathfrak{I}_{2n-1} （或 \mathfrak{I}_{2n}）生成的右（或左）理想，完成证明。

### 3. 直极限评分代数

设 (A_\alpha, \phi_{\beta \alpha}) 为型 \Delta (II, § 11, no. 3, 注 3) 的分级交换环的有向直接系统，对于每个 \alpha，令 E_\alpha 为型 \Delta 的分级 A_\alpha 代数；对于 \alpha \leq \beta 设 f_{\beta \alpha}：E_\alpha \to E_\beta 是分级代数的 A_\alpha 同态，并假设 f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha} 对于 \alpha \leq \beta \leq \gamma；那么我们将在型 \Delta 的分级交换环的有向直接系统 (A_\alpha, \phi_{\beta \alpha}) 上调用 (E_\alpha, f_{\beta \alpha}) 型 \Delta 的分级代数的有向直接系统。然后我们知道 (II, § 11, no. 3) E = \lim \to E_\alpha 在分级环 A = \lim \to A_\alpha 和乘法上具有规范的模结构型 \Delta 分级，使得 E^\lambda E^\mu \子集 E^{\lambda + \mu} （其中(E^\lambda)表示E)上的刻度；那么这个乘法和 E 定义上的分级 A-模结构在 E 上分级的 A-代数结构型 \Delta； E，这个结构，被称为分级代数的直接系统(E_\alpha, f_{\beta \alpha})的直极限。 典范同态 E_\alpha \ 到 E 取分级代数的 A_\alpha 同态。此外，如果 F 是型 \Delta 的分级 A-代数和 A_\alpha 同态 u_\alpha 的 (u_\alpha) 直接系统：E_\alpha \to F，则 u = \lim \to u_\alpha 是分级代数的 A-同态。

### 习题{#alg-iii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
