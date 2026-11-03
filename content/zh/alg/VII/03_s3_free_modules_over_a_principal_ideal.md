---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 3
section_title: Free modules over a principal ideal domain
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.14-A VII.15, A VII.59-A VII.62
pdf_pages: 0373-0374, 0418-0421
extraction: ocr
statements: 6
exercises: 11
content_sha256: aa6166dbb7cdf83d65c968ee4fda1be29050ca643f9d9d9f2fbadfec4d1e63ad
translated_from: content/en/alg/VII/03_s3_free_modules_over_a_principal_ideal.md
translation_method: google
source_content_sha256: fc7f397e634b76ed9e27c6fa8e0cbf059c23e62ee408af71f36a239a6f0c2d07
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 180cdd4a06e9c1cb851b6b5b67688ca7b30519d20c191e48050b1782bb970887
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。 自由模超过主理想整环

#### 定理 1 {#alg-vii-s3-thm-1 .statement tag=0735}

— *令$A$为环，使得$A$的每个左理想都投影（II，p. 231，Def.1）作为$A$模。那么自由左$A$-模$L$的每个子模$M$都是模的直和同构于$A$的理想。*

令$(e_i)_{i \in I}$为$L$的基，并令$p_i$为该基的坐标函数相应的。 选择 $I$ 的*良好排序* (*集合理论*, III, p. 153) 并令 $L_\alpha$ 表示由 $e_i$ 生成的子模，对于 $\alpha \leq i$；把$M_\alpha = M \cap L_\alpha$。坐标函数 $p_i$ 映射 $M_\alpha$ 到理想$a_\alpha$ $A$；由于$a_\alpha$是射影$A$模，因此存在$M$的(II，p. 231，命题4)子模$N_\alpha$，使得映射$x \mapsto p_i(x)$从$N_\alpha$进入$a_\alpha$ 是双射的。令$M'_\alpha$为由$N_\alpha$生成的$L$的子模，对于$\alpha \leq i$；我们将证明所有$\alpha$都有$M'_\alpha = M_\alpha$，这意味着$M$是由$(N_\alpha)_{\alpha < i}$族生成的。事实上，假设所有 $\lambda < i$ 都是 $M'_\lambda = M_\lambda$；然后$p_\lambda(x) \in a_\lambda$，对于所有$x \in M_\lambda$；因此存在$y \in N_\lambda$使得$x - y$是有限多个元素$e_i$中的线性组合，其中$\alpha < \lambda$；在其他字$x - y$是$M_\alpha$的元素，对于某些$\lambda < i$；归纳法假设表明$x - y \in M'_\lambda \subset M'_\alpha$，即$x \in M'_\alpha$，等等$M'_\alpha = M_\alpha$。还需要证明$N_\alpha$中的和是直接的；现在假设存在一个线性关系 $\sum a_\alpha = 0$，其中 $a_\alpha \in N_\alpha$，其中 $a_\alpha$（除了有限多个都是零）并不都是零。令$p$为最大的指标$\alpha$，使得$a_\alpha \neq 0$；因为$p_\mu(a_\lambda) = 0$对应$\lambda < \mu$，我们有$p_\mu(a_\mu) = p_\mu\left( \sum a_\alpha \right) = 0$，所以$a_\mu = 0$，与$p$的选择相矛盾。

#### 推论 1 {#alg-vii-s3-thm-1-cor-1 .statement tag=0736}

— *如果 $A$ 的每个左理想都是射影的，则射影左 $A$ 模的每个子模都是射影的。*

事实上，每个射影$A$-模块都是自由$A$-模块的子模（II，p. 231，命题4），并且Th。 1 适用。

#### 推论 2 {#alg-vii-s3-thm-1-cor-2 .statement tag=0737}

— *超过主理想整环的每子模自由模都是免费的。*
    这紧随 Th 而来。 1、因为主理想整环的每一个理想都是自由的。

#### 推论 3 {#alg-vii-s3-thm-1-cor-3 .statement tag=0738}

— *每超过投射模超过主理想整环都是免费的。*
#### 注 {#alg-vii-s3-n0-rem-1 .statement tag=0739}

Th 的证明。图1表明，$A^{(I)}$的每个子模都同构于直和$\bigoplus a_i$，其中每个$a_i$都是$A$的理想。

命题I。 — *如果L是有限秩n的自由模超过主理想整环A，则L的每个子模M是秩$\leq n$的自由模。*
    事实上 M 是 Cor 的自由模。 2至Th。 1，通过前面的注，或者通过下面的引理，它有秩$\leq n$：

#### 引理 1 {#alg-vii-s3-lem-1 .statement tag=073A}

— *令 L 为交换环 A 上的模，由 n 元素生成，并令 M 为 L 的自由子模；那么 M 有秩 $\leq n$。*
    首先假设L是免费的。让 i 将 M 的典范嵌入表示为 L。由 III、p. 520、Cor. 可知，同态 $\bigwedge^n i : \bigwedge^n M \to \bigwedge^n L$ 是单射；根据 III、p. 511、第 6 条命题、$\bigwedge^n L = \{0\}$，所以 $\bigwedge^n M = \{0\}$；由此可知 M 有秩 $\leq n$ (III, p. 518, Cor. 1)。现在考虑一般情况； 模L是秩n的自由模L'中的商。存在与 M 同构的 L 子模 M'（II，p. 218，命题 21）。根据参数 M' 的第一个部分，有秩 $\leq n$，结果如下。

#### 推论 {#alg-vii-s3-n0-cor-1 .statement tag=073B}

— *令 E 为模超过主理想整环 A，由 n 元素生成。那么 E 的任意子模 F 最多可以由 n 元素生成。*
    确实存在从$A^n$到E（II，p. 216，Cor.3）的同态 f，并且$f^{-1}(F)$，即秩$m \leq n$的自由模，由n元素生成； f 生成 F 下的像其中元素。

### 习题{#alg-vii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
