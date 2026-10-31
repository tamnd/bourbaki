---
book: alg
book_title: Algebra
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0021-0023
extraction: ocr
statements: 0
exercises: 0
content_sha256: d4e19865cae087512bb1dcaaad0e126e1f0b32041684a12b4bed5c72a84619b5
translated_from: content/en/alg/00_introduction_i_iii.md
translation_method: google
source_content_sha256: 95936eb99f28c9abcab27ec59169aeb970a237913763d70013fdd74c7e6811c6
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 5f16cd8c865149145093f88678649f5719b9f864618e7e69955a32e42e7b9f3b
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 介绍

代数本质上涉及计算，即在集合的元素上执行“代数运算”，其中最著名的例是由初等算术的“四个规则”提供的。

这里不是回顾渐进抽象过程的地方，代数运算的概念最初仅限于自然数和可测量的量值，逐渐扩大了它的领域，而“数”的概念获得了平行的推广，直到超越后者的经过，它开始被应用到元素，没有“数字”特征标，对于集合的例置换（参见历史注记到章 I）。毫无疑问，这些连续的扩张的可能性，其中形式的计算保持不变，而进行这些计算的数学实体的性质却有很大差异，这导致了现代数学的指导原理逐渐孤立，即数学实体本身并不重要；重要的是他们的关系（参见书I）。无论如何，可以肯定的是，代数比数学的其他分支之前更好地达到了这个抽象水平，并且长期以来它一直被视为代数运算的研究，独立于它们可以应用的数学实体。

除去通常代数运算背后的任何特定特征标、公共的概念的情况，非常简单：对同一集合 E 的两个元素 $a, b$ 执行代数运算，意味着与有序对关联$(a, b)$ 集合 E 的明确定义的第三个元素 $c$。 In other words, there is nothing more in this notion than that of function: to be given an algebraic operation is to be given a function defined on $E \times E$ and taking its values in E; the only peculiarity lies in the fact that the set of definition of the function is the product of two sets identical with the set where the function takes its values; to such a function we give the name law of composition.

除了这些“内部律”之外，数学家还被引导（主要是在几何学的影响下）考虑“律或合成”的另一个型；这些是“作用的律”，其中，除了集合 E（仍保留在前台）之外，还出现辅助集合$\Omega$，其元素称为运算符：律这次与有序对关联操作符 $\alpha \in \Omega$ 的 $(\alpha, a)$ 由……组成和元素 $a \in E$ E 的第二个元素 $b$。对于欧氏空间 E 上给定中心的例位似与实数 $k$（“位似比率”，这里是运算符）和 E 的点 A 另一个点 A' 相关联：这是 E 上作用的律。

符合一般定义（集合理论，IV, § 1, no. 4），在集合E上给出合成的一个或几个律或作用定义结构的律；对于以这种方式定义的结构，我们保留代数名称结构，正是对这些的研究构成了代数。

代数结构有多个类（集合理论，IV, § 1, no. 4），一方面以合成的律或作用的律为特征，另一方面以定义为特征的公理为这些律受到影响。当然，这些公理并不是任意选择的，而只是应用中出现的大多数律的性质，例如结合性、交换律等。章I本质上致力于阐述这些公理以及由此推导出的一般推论；还对代数结构中两个最重要的类、群（其中合成中仅出现一个律）和环（其中合成中出现了两个律）进行了更详细的研究，其中域结构是一个特例。

在章I中还存在群中带有运算符的定义和带有运算符的环，其中除了合成中的律之外，还出现了作用中的一个或多个律。最重要的群运算符是模，其中向量空间是一个特殊的例，它在古典几何和现代数学分析中都发挥着重要作用。 模结构的研究起源于线性方程组，从而得名线性代数；有关此主题的结果可在章 II 中找到。

类似地，最常出现的运算符的环称为代数（或超复数系统）。在章III和IV中，对代数的两个特殊的型：外代数进行了详细的研究，其及其衍生的行列式理论是线性代数的宝贵工具；和多项式代数，它们是代数方程理论的基础。

章V阐述了交换域的一般理论及其分类。该理论的起源是对未知数的代数方程的研究。今天产生这个问题的问题只不过是一种历史兴趣，但交换域的理论仍然是代数的基础，一方面是代数数理论的基础，另一方面也是代数几何的基础。

由于自然数的集合有合成、加法、乘法两个律，所以作为自然数的研究的古典算术（或数理论）从属于代数。然而，与这两个律定义的代数结构相关的是序关系“a 除 b”定义的结构；而古典算术的独特之处恰恰在于对这两个相关的结构之间的关系的研究。这并不是唯一一个例，其中阶结构因此通过“整除性”关系与代数结构相关联：这个关系在多项式环中起着同样重要的作用。因此，将在章VI对此进行一般研究；这项研究将应用于章VII，在某些特别简单的环上确定模的结构，特别是“基本除子”的理论。

章、VIII和IX致力于更具体的理论，但在数学分析中有很多应用：一方面，半单模和环的理论，与群的线性表示的理论密切相关；另一方面，二次形式和厄米特形式的理论，以及与之相关的群的研究。最后，从纯代数点的角度研究章、II、VI和IX中的基本几何（仿射、射影、欧氏等）：这里只不过是一种新的语言来表达已经在别处获得的代数的结果，但它是一种特别适合代数几何和微分几何的后来发展，这章作为介绍。
