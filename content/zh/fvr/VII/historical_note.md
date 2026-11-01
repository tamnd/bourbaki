---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: fvr-i-vii
book_pages: 329-331
pdf_pages: 0344-0346
extraction: ocr
statements: 0
exercises: 0
content_sha256: e6b05817b3cc3b64efad05ee20b14cf25505960155e523c800915cbdc7f419a5
translated_from: content/en/fvr/VII/historical_note.md
translation_method: google
source_content_sha256: 7c83612bea7e1b59873862456e66760a322c976bfe451e25a58e19896cc17b96
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: d4533a760fb7003182babbfdd3d272651112c4f775b7ecf08f8df9f5827b7401
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（注意：罗马数字指的是在注末尾找到的参考书目。）

根据实参数 $\lambda$ 并等于$u_n$（对于$\lambda = n$）的积分，通过值“插值”序列 $(u_n)$的想法可以追溯到 Wallis (III, p. 55)。正是这个想法主要指导了欧拉，在 1730 年 ((I), v. XIV, p. 1-24) 他集合亲自对阶乘的序列进行插值。他首先指出，$n!$等于无限乘积$$
\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n},
$$，其中乘积是为$n$中的每个值（或不是整数）定义的，特别是，对于值$n = \frac{1}{2}$，它需要值 $\frac{1}{2} \sqrt{\pi}$，沃利斯的公式。这个结果与沃利斯的结果之间的类比促使他重新审视积分
$$
\int_0^1 x^e (1-x)^n dx
$$
$(n$整的，$e$任意）后者已经考虑过了。欧拉获得值
$$
\frac{n!}{(e+1)(e+2)\ldots(e+n+1)}
$$
对于它，使用二项式展开；变量的变换然后向他表明$n!$是极限，因为$z$趋于0，整的
$$
\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx,
$$
从而“第二欧拉积分”
$$
n! = \int_0^1 \left( \log \frac{1}{x} \right)^n dx;
$$
通过同样的方法，并使用沃利斯的公式，他得到了公式
$$
\int_0^1 \sqrt{\log 1/x} dx = \frac{1}{2} \sqrt{\pi}.
$$
在他后来的著作中，欧拉经常回到这些积分。因此他发现了补数’ 关系 ((I), t.XV, p 82 和 t.XVII, p. 342), 公式 $\mathbf{B}(p, q) = \Gamma(p)\Gamma(q)/\Gamma(p+q)$ ((I), t.XVII, p. 355)，以及勒让德-高斯公式相应的至 $x = 1$ ((I)，t. XIX，p. 483) 的特殊情况；当然，所有这些都不用担心收敛问题。

高斯结合他的超几何函数上的研究继续研究$\Gamma$函数，其中$\Gamma$函数是极限情况（II）；正是在这个研究的过程中，他获得了将军乘法公式（勒让德早先已经注意到$p = 2$）。后来对$\Gamma$的工作主要是将这个函数扩展到复数域。直到最近才认识到，对数凸性的性质表征了$\Gamma(x)$（在实数域中），直到函数方程$f(x + 1) = x\, f(x)$（III）的解中的常数因子； Artin 展示了 (IV) 如何将 $\Gamma(x)$ 上的所有经典结果简单地链接到这个性质。我们非常密切地关注他的阐述。

(I)L。欧拉，Operaomnia，莱比锡-柏林（Teubner）：t。 XIV（1924），t。 XV（1927），t。 XVII (1915) 和 t。 XIX（1932）。
(II) C.F.高斯，韦尔克，t。 III，哥廷根，1866 年。
(III) H. Bohr 和 J. Mollerup，Laerebog i matematisk Analyse，t。 III，哥本哈根，1922 年，p. 149-164。
(IV) E. Artin，Einführung in die Theorie der Gammafunktion，莱比锡 (Teubner)，1931 年。
