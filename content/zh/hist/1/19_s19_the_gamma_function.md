---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 19
section_title: The Gamma Function
lang: zh
source: hist
pdf_pages: 0205-0205
extraction: ocr
statements: 0
exercises: 0
content_sha256: f46ad536f3977366f3124885f5df696ff64a53c74b3183d29fd2e0a2f8240d73
translated_from: content/en/hist/1/19_s19_the_gamma_function.md
translation_method: google
source_content_sha256: 7092fa519a4f115973a096a09aabbecb5a46cdac0f410b2a08e230e4c0142ff8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 53e17aa31e3fad8ffdcb80cc3ef26f4b694e274dfa364c1200c9ed5063fcf078
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 19. 伽玛函数。

将序列 $(u_n)$ 通过依赖于实数参数 $\lambda$ 的积分的值进行“插值”并且对于 $\lambda = n$ 等于 $u_n$ 的想法可以追溯到 Wallis（cf. 第 187 页 ff.）。正是这个思想成为欧拉的主要指导思想，在 1730 年 ([108 a], (1), v. XIV, pp. 1-24)，他提出了对阶乘的序列进行插值的想法。他首先指出，$n!$等于无限乘积$\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n}$，这个乘积是为$n$的每个值（整数或非整数）定义的，特别是，对于$n = \frac{1}{2}$，它需要值$\frac{1}{2} \sqrt{\pi}$沃利斯的公式。这个结果与沃利斯的结果的类比导致他再次采用后者已经考虑过的积分$\int_0^1 x^e (1-x)^n dx$（$n$整数，$e$任意）。欧拉通过二项式展开得到其值$\frac{n!}{(e+1)(e+2)\cdots(e+n)}$；变量的变换然后向他显示积分$\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx$的$n!$是极限，因为$z$趋于0，从而是“第二欧拉积分”$n! = \int_0^1 (\log \frac{1}{x})^n dx$；通过同样的方法并使用沃利斯的公式，他获得公式$\int_0^1 \sqrt{\log \frac{1}{x}} dx = \frac{1}{2} \sqrt{\pi}$。在他后来的工作中，欧拉经常回到这些积分。他以这种方式发现了补码的关系 ([108 a], (1), v. XV, p. 82 和 v. XVII, p. 342), 公式 $B(p, q) = \Gamma(p) \Gamma(q) / \Gamma(p + q)$ ([108 a], (1), v. XVII，p. 355），以及勒让德-高斯公式相应的到$x = 1$的特殊情况（[108a]，（1），v.XIX，p. 483）；当然，所有这一切都不用担心收敛问题。

高斯继续研究$\Gamma$函数以及他的研究关于超几何函数的研究，其中函数$\Gamma$是极限情况（[124a]，v.III，第125-162页）；正是在这个研究期间，他获得了乘法的将军公式（勒让德已经注意到不久之前对于$p = 2$）。 $\Gamma$后续的工作主要关注这个函数到复数域的扩张。直到最近，人们才注意到函数方程$f(x+1) = x f(x)$的所有解中，对数凸性性质的特征为$\Gamma(x)$（在实数域）高达因子（[26]，第149-164页）； Artin 已经展示了 [7d] 关于 $\Gamma(x)$ 的所有经典结果如何可以简单地与这个性质联系起来。
