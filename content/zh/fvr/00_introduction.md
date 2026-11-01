---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: zh
source: fvr-i-vii
book_pages: 1-2
pdf_pages: 0016-0017
extraction: ocr
statements: 0
exercises: 0
content_sha256: 142b9195994a423fea08df54bade398319b38136203aa6bb2abfa86922c53d89
translated_from: content/en/fvr/00_introduction.md
translation_method: google
source_content_sha256: 85e0ba02d9e87d1ef4af523569a61f14e491623624b2c9c740da85ac45ab1be5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: a09638cf7500f7e73c1667bd3f996c031d663b6dd895b05a13dd51cad4425c92
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 介绍

本书的目的是对一个实变量的无穷小性质进行初步研究；这些属性的扩张到几个实数变量的函数，或者更一般的空间上定义的函数，将仅在以后的书中进行处理。

我们将证明的结果首先在实变量的关系到（有限）实值函数中有用；但其中大多数扩展没有进一步论证实变量的函数，在$\mathbf{R}$上的拓扑向量空间中取值（见下文）；由于这些函数经常出现在数学分析中，我们将为它们说明所有不特定于实值函数的结果。

我们刚才讲的拓扑向量空间的概念，在这级数的书V中有详细的定义和研究；但本书中我们不需要第V的任何结果；然而，一些定义是需要的，为了方便读者，我们将在下面复制它们。

我们不会在（交换的）域 K（代数，II，p. 193）上重复向量空间的定义。 $^1$ 拓扑向量空间 E 在拓扑域 K 上是向量空间在具有拓扑的 K 上，使得函数 $x + y$ 和 $xt$ 分别在 $E \times E$ 和 $E \times K$ 上连续；特别是，这样的拓扑与E的加法群的结构兼容。本书中考虑的所有拓扑向量空间都隐含地假设为Hausdorff。当拓扑群 E 完备时，我们就说拓扑向量空间 E 完备。每个在定值域 K（Gen. Top.、IX、p. 169）$^2$上的赋范向量空间都是K上的拓扑向量空间。

令 E 为实域 $\mathbf{R}$ 上的向量空间（有或没有拓扑）；如果 x, y 是点 $xt + y(1-t)$ 的 E 集合中的任意点，其中 t 穿过闭区间

$^1$元素（或向量）向量空间E超过交换域K通常在这个章中用粗小写字母表示，标量用罗马小写字母表示；最常见的是，我们将标量t放在向量x的乘积的右侧，将乘积写为$xt$；有时我们会允许自己在某些更方便的情况下使用左边的记号$tx$；另外，有时我们将在形式$x/t$中写出标量$1/t$（$t \neq 0$）和向量x的乘积。

$^2$ 我们记得 E 上的范数是在 E 上定义的实数函数 $\|x\|$，取有限非负值，这样关系 $\|x\| = 0$ 等价于 $x = 0$ 并且这样

$$
\|x + y\| \leq \|x\| + \|y\| \quad \text{and} \quad \|xt\| = \|x\| \cdot |t|
$$

对于所有$t \in K$（$|t|$是K中$t$的绝对值值）。

$\mathbf{R}$ 的线段 [0, 1] 称为具有端点 $x, y$ 的*闭合线段*。有人说，如果对于$A$中的任何$x, y$，具有端点$x$和$y$的闭线段包含在$A$中，则$E$的子集$A$是“凸”。对于例，仿射线性簇是凸的；任何闭合线段也是如此；在 $\mathbf{R}^n$ 中任何平行四面体 (*Gen.Top.*, VI, p. 34) 都是凸的。凸集合的每个交都是凸的。

如果原点（以及 $E$ 的任何点）具有 *凸* 邻域的基本系统，我们就说域 $\mathbf{R}$ 上的拓扑向量空间 $E$ 是“局部凸”。每个 *normed* 空间都是局部凸的；事实上，$\|x\| \leq r \ (r > 0)$形式是$E$中0的邻域的基本系统，并且每个球都是凸的，因为关系$\|x\| \leq r,\ \|y\| \leq r$意味着

$$
\|xt + y(1-t)\| \leq \|x\| t + \|y\| (1-t) \leq r
$$

对于$0 \leq t \leq 1$。

最后，一个（可交换的）*拓扑域* $K$上的*拓扑代数* $A$是代数超过$K$，赋予拓扑，其中函数$x + y,\ xy$和$xt$连续分别为$A \times A,\ A \times A$和$A \times K$；当一个人仅将拓扑和向量空间结构赋予$A$超过$K$时，则$A$是拓扑向量空间。每个*范数代数*在*值域*$K$（*Gen.Top.*，IX，p. 175）上都是$K$上的拓扑代数。
