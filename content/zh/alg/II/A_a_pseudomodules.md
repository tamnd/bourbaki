---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 0
section_title: Pseudomodules
appendix: true
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 378-379, 425
pdf_pages: 0402-0403, 0449-0449
extraction: ocr
subsections:
    - "no": 1
      title: ADJUNCTION OF A UNIT ELEMENT TO A PSEUDO-RING
      page: 378
      pdf_page: 402
    - "no": 2
      title: PSEUDOMODULES
      page: 378
      pdf_page: 402
statements: 0
exercises: 1
content_sha256: b7c2d5759bdc0b9ffb23a686f628285744c345821551d5a123e4592a39b05027
translated_from: content/en/alg/II/A_a_pseudomodules.md
translation_method: google
source_content_sha256: db883a717633a15e64137f982b71d8ce6f40a59783e9d1c7d5ac706248c39106
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8921a4aff337285350099364662e7a83ca686bf058c815f86308834378d1719e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录

# 伪模

### 1. 伴随 OF 单位元到伪环

设 A 为伪环 (I, § 8, no. 1)。在集合$A' = \mathbf{Z} \times A$我们定义以下律或合成：

$$
\begin{cases}
(m, a) + (n, b) = (m + n, a + b) \\
(m, a)(n, b) = (mn, mb + na + ab).
\end{cases}
$$

立即验证$A'$与合成的这两个律是环，其中元素$(1, 0)$是单位元。 集合$\{0\} \times A$是$A'$的双面理想，$i : x \mapsto (0, x)$是伪环A到子伪环$\{0\} \times A$的同构，由此识别A和$\{0\} \times A$。 $A'$ 称为环，由伪环 A 与单位元邻接而派生。

如果 A 已经有单位元素 $\varepsilon$，则 $A'$ 的元素 $e = (0, \varepsilon)$ 是 $A'$ 的幂等属于到中心，这样

$$
A = eA' = A'e.
$$

那么$(eA', (1 - e)A')$是$A'$的直接分解（I, § 8, no. 11），并且环$(1 - e)A'$与$\mathbf{Z}$同构的。

### 2.伪模

给定一个带有或不带有单位元的伪环 A，A 上的左拟模是一个可交换的群 E（加法写），承认 A 作为运算符的集合以及 § 1, no. 1 的满足公理 $(\mathrm{M}_I), (\mathrm{M}_{II})$ 和 $(\mathrm{M}_{III})$， 定义 1. A 上的右伪模的定义类似。

令$A'$为通过将单位元与A邻接而获得的环。如果E在A上是左拟模，则对于所有$x \in E$和每个元素$(n, a) \in A'$，E上的左$A'$模块结构通过写入与它相关联，

$$
(n, a) . x = nx + ax.
$$

§ 1, no. 1、定义 1 的公理$(\mathrm{M}_I)$到$(\mathrm{M}_{IV})$立即得到验证；

此外，通过将这个模结构的运算符集合限制为$\{0\} \times A$（用$A$标识），我们得到最初给出的$E$伪模结构。

对于$E$的子集$M$为子群，且运算符为伪模$E$（在这种情况下，诱导的结构显然也是左拟模结构超过$A$），有必要且充分$M$是关联的$A'$模块$E$的子模，并且该子$A'$模块与伪模$M$相关联。此外，商$A'$-模$E/M$然后通过运算符$E/M$与商群相关联，这显然是伪模超过$A$。

如果$E, F$是$A$上的两个伪模，则群的同态$E \to F$（带有运算符）与分别与伪模$E$相关联的$A'$模块的$A'$线性映射$E \to F$相同$F$。如果$(E_i)_{i \in I}$是$A$上的伪模族，则带有运算符$\prod_{i \in I} E_i$和$\bigoplus_{i \in I} E_i$的群是$A$上的伪模，并且关联的$A'$模块分别是乘积和关联的$A'$模块$E_i$的直和。 伪模的逆和直极限也有类似的结果。因此，伪模超过$A$的理论可以完全简化为$A'$模的理论。

### 习题 {#alg-ii-a0-exercises}

请参阅[习题附录 0](exercises/a0/)。
