---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: int-i-vi
pdf_pages: 0023-0024
extraction: ocr
statements: 0
exercises: 0
content_sha256: 0b956bf20dd3b4e997187681a1e00e63641b6eac2a63c6d575c95fe446c0bcde
translated_from: content/en/int/I/historical_note.md
translation_method: google
source_content_sha256: 61a0e9809da1e06fbf74fbe28f6f19223c692979b397ccd8d7c3d2caf36893ee
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 863890370f13b9f67093596cf89a4b73c1fd001f627c39fad741888b839285d0
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

# 历史注记

（注：罗马数字指的是注末尾的参考书目。）

两个正数的算术平均值和几何平均值的概念可以追溯到古代，特别是毕达哥拉斯学派将它们作为他们最喜欢的主题之一。这些手段之间的不等式 $\sqrt{ab} \leq \frac{1}{2}(a + b)$ 也可能是他们所熟知的；无论如何，它是由欧几里得证明的，与最大化两个数（其和给定）的乘积的问题有关。显然，人们必须等到 1729 年相当晚的日期才能找到麦克劳林明确提到的推广、问题到$n$数，以及相应的不等式（而且这个，甚至虽然更困难的极值问题早已得到解决） 之前）。

从 18 世纪末开始，其他类似的不等式就出现在数学分析和几何中。因此，1789 年，Lhuilier 解决了与不等式相关的几何最大值问题

$$
\sqrt{\left( \sum_{k=1}^n a_k \right)^2 + \left( \sum_{k=1}^n b_k \right)^2} \leq \sum_{k=1}^n \sqrt{a_k^2 + b_k^2};
$$

柯西于 1821 年证明了特殊情况

$$
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
$$

Hölder 的不等式； 1859 年的 Buniakowsky 和 ​​1885 年的 H. A. Schwarz 将柯西的不等式推广到积分。

然而，直到19世纪末，凸性不等式才成为系统研究的对象。 O. Hölder 在 1888 年（I）产生了将单个变量的凸函数引入到问题中的想法：从而得到了以$\log x$的凹性为起点的几何平均值的不等式； 应用与函数$x^r$同样的想法，他证明了不等式以他的名字命名，并且一年前已经被L发现了。 J. Rogers 从几何平均值的不等式开始（cf. Exer. 4）。至于闵可夫斯基的不等式，后者在1896年证明了这一点（对于有限的和），结合他关于“数的几何”的令人难忘的著作（（II），第115-117页）；然而，虽然凸性的思想（对于任何数变量的函数）是这项工作的基本概念之一，但令人惊讶的是，闵可夫斯基没有注意到他的不等式可以通过霍尔德的方法应用于$(1 + x^r)^{1/r}$来获得（他将自己限制为应用经典方法用于通过无穷小演算求极值）。

为了更深入地研究凸性不等式及其应用，读者可以查阅 Hardy、Littlewood 和 Pólya 专门讨论该问题的书，这也是包含非常完整的参考书目（III）。

(I) O. Hölder，Ueber einen Mittelwertsatz，Göttinger Nachrichten (1889)，第 38-47 页。

(II) H. Minkowski，《Geometrie der Zahlen》，第 2 期。编辑，莱比锡-柏林（Teubner），1910 年。

(III) G. H. Hardy、J. E. Littlewood、G. Pólya，《不平等》，剑桥（大学出版社），1934 年。
