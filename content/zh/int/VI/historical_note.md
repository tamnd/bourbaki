---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: int-i-vi
pdf_pages: 0463-0465
extraction: ocr
statements: 0
exercises: 0
content_sha256: 62ea4c1535acd1b90d7eb1538271e36db0d53819e13805d622066b8e24600606
translated_from: content/en/int/VI/historical_note.md
translation_method: google
source_content_sha256: ddd2484b153907abc4b504e7847024232e7bbd05fcbac91aba31ada63b157656
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: e14eed0a09d9c024b57383dc67f1aae228512b682fb478fb367f71f052647c6c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（注：罗马数字指的是注末尾的参考书目。）

随着 19 世纪“向量演算”的发展，当前的实践是必须对向量值函数进行积分，但只要它只是有限维空间中函数与值的问题，这个运算就不会产生任何问题。 问题。只有利用希尔伯特谱理论，我们才能满足运算，自然而然地得出更一般的积分概念：该理论实际上导致与希尔伯特空间 $\mathbf{H}$ 上的每个连续厄米特形式 $\Phi(x, y)$ 关联，正交族 $(E(\lambda))_{\lambda \in \mathbf{R}}$ 投影算子具有性质，对于$\mathbf{H}$的向量的每一个对$(x, y)$，函数$\lambda \mapsto (E(\lambda)x|y)$有界变化且$\Phi(x, y) = \int \lambda d(E(\lambda)x|y)$；如果与 $\Phi$ 厄米特运算符 $A$ 关联，使得 $\Phi(x, y) = (Ax|y)$，则很容易将前面的公式写为 $A = \int \lambda dE(\lambda)$。但只是从大约 1935 年开始，之后 Bochner 在 Banach 空间中引入了函数与值的（“强”）整的，人们才开始专注于定义向量值函数的积分（或关于向量测度的积分），以便能够合法地写公式如前一个。这个扩张主要是由Gelfand（III）、邓福德和佩蒂斯（IV）和（V）完成的；他们的结果是针对 Banach 空间给出的，但是扩展毫无困难地转换为更一般的局部凸空间。

将体积分解为“切片”并将体积上的积分减少为每个切片上的积分，然后进行一次积分的想法自无穷小演算开始就一直在数学分析中使用（卡瓦列里的“不可分的演算”只不过是这个原理的第一个轮廓，甚至可以追溯到阿基米德（参见《历史》。注书IV，章节I–III））。但在经典应用中，“切片”始终具有非常特殊和非常规则的性质（最常见的是解析曲面的开放子集，取决于参数的分析）；如果没有统一的一般理论，情况就不可能是别的样子。测度分解的一般问题由冯·诺​​依曼于1932年结合遍历理论（I）提出并解决；大约在同一时间（并且独立地），柯尔莫戈洛夫在为概率论奠定公理基础的同时，以一般方式引出了定义“条件概率”的概念，并证明了它的存在，问题本质上相当于测度的分解（II）。

(I) J. von NEUMANN，《经典机械学中的操作方法》，Ann。数学，(2)，33 (1932)，第 587–642 页。

(II) A. KOLMOGOROFF，Grundbegriffe der Wahrscheinlichkeitsrechnung，柏林（施普林格），1933 年。

(III)I。 GELFAND，抽象功能和线性操作员，Mat。 Sborn.，（NS），4（1938），第 235-284 页。

(IV) N. DUNFORD，线性空间的均匀性，Trans。阿米尔。数学。 《社会学会》，44 (1938)，第 305–356 页。

(V) N. DUNFORD 和 B. PETTIS，可求和函数上的线性运算，Trans。阿米尔。数学。 《社会学会》，47 (1940)，第 323–392 页。
