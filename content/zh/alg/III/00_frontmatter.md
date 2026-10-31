---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
kind: front
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: "427"
pdf_pages: 0451-0451
extraction: ocr
statements: 0
exercises: 0
content_sha256: 7901408099fbd8fff4bad3a039c2f6cca35576df33bbfc5945a2db4e539eb406
translated_from: content/en/alg/III/00_frontmatter.md
translation_method: google
source_content_sha256: 6265d61279faab9dcf08066eb99e498297b3d05106b7e1efab665fe26a7b784b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 63bd3e7c5b96449b2eea87f07709c7d2bbb434039200b331234aee3541d9de01
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 章 III

# 张量代数，外部代数，对称代数

回想一下章 I 中引入的指数记号，我们将经常使用它（I, § 7, no. 8）：

设$(x_\lambda)_{\lambda \in L}$是环$A$的成对可置换族元素；对于有限支撑的每一个映射$\alpha : L \to N$我们应该写

$$
x^\alpha = \prod_{\lambda \in L} x_\lambda^{\alpha(\lambda)}.
$$

如果$\beta$是$L$的另一个映射转化为有限支撑的$N$，则$\alpha + \beta$表示映射

$$
\lambda \mapsto \alpha(\lambda) + \beta(\lambda)
$$

of $L$ into $N$; with this law of composition the set $N^{(L)}$ of mappings of $L$ into $N$ of finite support is the free commutative monoid derived from $L$ and

$$
x^\alpha x^\beta = x^{\alpha + \beta}.
$$

对于所有$\alpha \in N^{(L)}$，我们写为$|\alpha| = \sum_{\lambda \in L} \alpha(\lambda) \in N$；然后$|\alpha + \beta| = |\alpha| + |\beta|$； $|\alpha|$ 称为“多重索引”$\alpha$ 的阶。对于所有$\lambda \in L$，令$\delta_\lambda$表示$N^{(L)}$的元素，使得$\delta_\lambda(\lambda) = 1$、$\delta_\lambda(\mu) = 0$代表$\mu \neq \lambda$（克罗内克指标）； $\lambda \in L$ 的 $\delta_\lambda$ 是阶 1 中 $N^{(L)}$ 的唯一元素。 $N^{(L)}$ 给出由乘积对 $N^L$ 排序引起的排序，因此关系 $\alpha \leq \beta$ 等价于“$\alpha(\lambda) \leq \beta(\lambda)$对于所有$\lambda \in L$”；那么多重索引$\lambda \mapsto \beta(\lambda) - \alpha(\lambda)$用$\beta - \alpha$表示，因此它是满足$\alpha + (\beta - \alpha) = \beta$的唯一多重索引。对于所有$\alpha \in N^{(L)}$，只有有限的数个多重索引$\beta \leq \alpha$； $\delta_\lambda$是集合$N^{(L)} - \{0\}$的最小值元素； 关系 $\alpha \leq \beta$ 意味着$|\alpha| \leq |\beta|$，如果$\alpha \leq \beta$ 和$|\alpha| = |\beta|$ 都存在，则$\alpha = \beta$。

最后，我们写$\alpha! = \prod_{\lambda \in L} (\alpha(\lambda))!$，从$0! = 1$开始就有意义。

从§ 4到§ 8（含），$A$表示交换环，并且，除非另有说明，代数被假定为结合且单位，代数同态被假定为单位。
