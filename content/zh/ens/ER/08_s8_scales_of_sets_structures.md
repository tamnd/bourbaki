---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 8
section_title: Scales of sets. Structures
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 383-385
pdf_pages: 0388-0390
extraction: ocr
statements: 0
exercises: 0
content_sha256: 1dd1f97844784d4ba467f9cbe66df3dea108aa96298dd707e5af99f4fe327cc5
translated_from: content/en/ens/ER/08_s8_scales_of_sets_structures.md
translation_method: google
source_content_sha256: 1729e7f56fb13a5cfb4b19ed30304bcfc4d735d7f99cdf7c9579aa41117e6f82
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: df21e6b836f0466e28732c7b36df2d340248e921d98cfdee1547d0980cd1ddd7
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 8. 集合的音阶。 结构

1. 例如，给定三个*不同* 集合 E、F、G，我们可以通过取子集的集合，或者通过单独形成其中一个的乘积，或者再次通过在某个序中取其中两个乘积，来从它们中获得形式其他集合。这样我们就得到*十二*新的集合。如果我们将这些添加到三个原始集合 E，F，G，我们可以在这十五个集合上重复相同的运算，省略那些给我们已经获得的集合；等等。一般来说，通过此过程获得的集合中的任何一个（根据显式概形）被称为属于到E、F、G上集合*的*规模*为基*。

例如，令 M、N、P 为该尺度的三个集合，并令 $R\{x,y,z\}$ 分别为 M、N、P 的泛型元素 $x$、$y$、$z$ 之间的 *关系*。那么$M \times N \times P$的R定义子集，因此（通过规范的对应）$(M \times N) \times P$的子集，即$\mathfrak{P}((M \times N) \times P)$的元素。因此，在同一标度中给出多个集合的元素之间的 *关系* 与在标度中给出另一个集合的 *元素* 相同。同样，例如，要将 M 的映射放入 N 中，（通过考虑此映射的图形），相当于将 $M \times N$ 的子集赋予，即 $\mathfrak{P}(M \times N)$ 的元素，这在标度中又是集合。最后，给出 M 中的两个元素（例如）相当于给出乘积集合 $M \times M$ 中的单个元素。

因此，在一个比例中被赋予一定的集合的元素的数，这些集合的通用元素之间的关系，以及这些集合中的某些子集的映射进入其他，所有这些都在最终的数学分析中被赋予了一个*量表中集合之一的单个元素*。

2.我们之前说过(§6)，如果E上的集合$\mathfrak{P}(E \times E)$定义序结构的元素C，如果它具有属性(a)$C \circ C \subset C$和(b)

$$C \cap C^{-1} = \Delta.$$

一般来说，考虑集合范围内的集合 M，其基为了例而由三个集合 E、F、G 组成。 让我们给自己一个 M 的泛型元素的明确规定属性的某个数，并让 T 为由这些属性定义的 M 的子集的交。 T 的元素 $\sigma$ 被称为 E、F、G 上 *类* T 的定义 a *结构*。 因此，类 T 的结构的特征在于由 E、F、G 形成 M 的概形，以及定义 T 的属性，这些属性被称为这些结构的*公理*。 我们为相同类的所有结构指定一个特定的名称。 作为命题“$\sigma \in T$”（即定义 T 的公理）的结果的每个命题都被认为属于物种 T 的结构的“理论”；例如，§ 6中陈述的命题属于有序集合结构理论。

在最后的例，公理可以表示为完全任意的基集合E。因此，我们给结构和满足这些公理赋予相同的名称，独立于定义它们的集合；从这些公理推导出来的命题在任何集合中都是有效的，因为它们的公式不涉及集合E的任何特殊性质。只要公理具有这种性质[^1]，这样的注就适用。

最常见的是，当一个音阶与多个集合 E、F、G 中的基由……组成一起使用时，其中一个集合，例如 E，在考虑中的结构中发挥着主导作用。因此，通过滥用语言，这些结构被认为是在集合E中定义的，而F和G被视为辅助集合。

最后，为了简化语言，通常给集合赋予一个特定的名称，它被赋予了确定的类的结构。因此，我们说的是*有序的集合*，在这个级数的稍后部分中，我们将定义概念*群，环，域，拓扑空间，均匀空间*等，所有这些都是字表示集合具有一定的结构。

3. 考虑相同类 T 的结构，其中 T 是集合 M 的子集，规模为集合。 如果我们将新的“公理”与定义 T 的公理相连接，则公理的系统由此获得包含在 T 中的 M 的定义子集 U。 据说类 U 的结构比类 T 的结构“更丰富”。 例如，*全序* 集合的结构比有序集的结构更丰富，因为$\mathfrak{P}(E \times E)$的元素C其中定义这样的结构必须满足附加公理

$$C \cup \overline{C}^{-1} = E \times E.$$

4. 设M、M′为同尺度的两个集合，即E、F、G为基。令 T 为 M 的子集，T′ 为 M′ 的子集，每个都由某些明确陈述的公理定义。每当我们能够将 T 的定义一对一映射*显式地映射到 T′ 上时，我们就可以考虑两个元素 $\sigma \in T$、$\sigma' \in T'$，其中对应在这个映射下彼此相连，就像在 E、F、G 上定义*相同的结构* 一样；和系统公理，其中定义 T 和 T′ 被称为“等价”。

*拓扑结构*提供了这种情况的例；它们可以通过几个等价公理系统来定义，其中两个系统特别有用（参见*一般拓扑*、章I, § 1）。

5. 令 E、F、G 为三个集合，并假设我们将 E、F、G 的*双射* 映射分别赋给另外三个集合 E′、F′、G′。由于我们知道如何将双射映射的 *典范扩张* 子集 (§ 2, no. 9) 的定义到集合以及乘积集合 (§ 3, no. 14)，我们可以一步一步地定义， *给定双射的扩张*到两个集合M、M′分别根据E、F、G的集合尺度上的*相同的概形*和基于E′、F′、G′的集合M、M′分别构建。令$f$为M到M′上的双射。如果$\sigma$在E，F，G上是结构，即M的子集T的元素，我们说$f(\sigma)$是通过给定的方法将结构$\sigma$*传输*到E′，F′，G′上获得的结构双射 E 到 E′，F 到 F′，G 到 G′。与 E、F、G 上的结构 $\sigma$ 相关的每个命题都会产生（通过使用适当的扩张）到与 E'、F'、G' 上的结构 $f(\sigma)$ 相关的命题。

相反，如果 $\sigma'$ 可以通过将 E、F、G 的双射分别*传输* $\sigma$ 到 E'、F'、G' 上来获得，则 E、F、G 上的结构 $\sigma$ 和 E'、F'、G' 上的结构 $\sigma'$ 被称为“同构的”；然后，这些映射被称为构成 $\sigma$ 到 $\sigma'$ 的 *同构的*。

当我们关心单个集合 E上的结构时，E的双射到E′上，其中迁移$\sigma$到$\sigma'$也称为集合E的*同构的，赋予结构$\sigma$，到集合 E′，赋予结构 $\sigma'$.*

当F和G是两个辅助集合时，这个映射也称为*同构的*，而这两个集合的双射是F和G自身的*恒等式*映射。

集合 E 的 *同构的*，赋予结构 $\sigma$，其自身称为 *自同构*。

当存在集合 E 的*同构的*，赋予结构 $\sigma$，到集合 E′，赋予结构 $\sigma'$时，通常可以方便地将*认同* E 与E′，即，给元素*相同的名称* 集合 M 是基于 E 的音阶中的元素，即像在$f$ 至集合 M 的适当扩张下。

6. 给定在集合范围内定义集合M的子集T的公理系统，我们应该确保，之前谈到结构和满足这些公理，集合T*不一定是空的*；否则公理将被称为“矛盾”或“不一致”。

7. 可能会发生这样的情况：在集合上定义结构的公理中的系统可以针对任意集合进行陈述，但是当我们考虑两个结构满足这些公理并定义在两个不同的集合 E、F 上时，我们从公理发现这些公理结构（如果存在）必然是*同构的*（这特别意味着 E 和 F 是*等价的*）。那么结构满足这些公理中的理论被称为*单价*；否则它们被称为“多价”。

整数的理论、实数的理论以及经典的欧氏几何都是单价理论； 有序集、群、理论和拓扑中的理论是多价理论。对多价理论的研究是现代数学区别于古典数学的最显着特征。

[^1]: The reader may have observed that the indications given here are left rather vague; they are not intended to be other than heuristic, and indeed it seems scarcely possible to state general and precise definitions for structures outside of the framework of formal mathematics (see Chapter IV).
