---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 255-257
pdf_pages: 0261-0263
extraction: ocr
statements: 0
exercises: 0
content_sha256: 295c74c5f70b339373cfb8b721b752bf4bea4a06d4adb8cbba7d024f7eba10f1
translated_from: content/en/ens/III/historical_note.md
translation_method: google
source_content_sha256: 35c7fafb7fcf59df7cdf3b82fc528a165d03d9d6a7897b9d7068e48d10fcf9a5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 07f91158ec25a8daa9cf5dde7b5f965b4a3aa7a71faa30c1d362c06add673f83
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

(章III, § 5)

（括号内数指参考书目
在这个注的结尾。）

概念、整数和基数数相关思想的演变与集合论和数理逻辑的历史密不可分，读者可参考章IV之后的历史注记。这个注的目的是简要说明计数和“组合分析”历史上的一些显着事实。

历史和考古学向我们揭示了巨大的数“计数的系统”，其主要目的是为每个人整数（根据实际使用的需要，最多可达极限）一个名字和一个书面的表示，由有限的数符号根据或多或少的规则形成。 律。到目前为止，最公共的的过程是将整数分解为“连续单位”$b_1$、$b_2$、...、$b_n$、...的和，其中每个和都是其前一个倍数的积分；尽管一般情况下 $b_n/b_{n-1}$ 被视为固定的数 $b$（系统的“基”，通常为 10），但此规则有许多已知的例外情况。对于例，在巴比伦语系统中，$b_n/b_{n-1}$是有时10和有时6[1]，而在玛雅人的时间顺序中系统，除了$n = 2$和$b_2/b_1 = 18$之外，$b_n/b_{n-1}$等于20 [2]。对于相应的文字符号，必须表示每个序$i$的“单位”$b_i$的数。在许多系统（对于埃及、希腊和罗马的例），连续的倍数$k.b_i$（其中$k$从1到$(b_{i+1}/b_i) - 1$变化）由依赖于$k$和$i$的符号表示。第一步也是重要的一步是用相同的符号表示所有数$k.b_i$（对于$k$的相同值）：这是“按位置计数”的原理，其中指标$i$由代表$k.b_i$的符号出现这一事实来指示“在第$i$位”。这种性质的第一个系统是巴比伦人的，他们肯定早在2000年B.C.，用相同的符号表示所有倍数$k.60^{\pm i}$相应的到指数$i$的各种值（[1]，第17页）。 93-109）。只要没有任何东西表明某个序中的单位是否不存在，即只要系统不是通过引入“零”来完成的，这样系统的不便之处当然在于它的歧义性。然而，巴比伦人在其更伟大的部分历史中却没有这样的标志，并且除了在B.C的最后两个世纪外，没有使用“零”，然后仅在数内；到那时，仅凭上下文就可以澄清所考虑的符号的含义。只有另外两个系统系统地使用了“零”：玛雅人的（显然，自基督教时代开始以来就在使用[2]）和我们现在的十进制系统，它来自（通过阿拉伯人）来自印度教数学，其中零的使用自公元一世纪以来就得到了证实。 零与数（而不仅仅是作为分隔符号）及其引入计算中是印度教徒的原创贡献 [3]。当然，一旦获得了“按位置计数”的原理，就很容易将扩展变成任意的基。对17世纪以来提出的不同“基”优劣的讨论取决于数值计算技术，这里进入不能。我们注只是位于这些系统中的根的运算，即所谓的“欧几里得除法”，在希腊时代并没有出现之前，并且无疑可以追溯到早期的毕达哥拉斯学派，他们将其作为理论算术中的重要工具。

枚举的一般问题，以“组合分析”的名称组合在一起，似乎在古典时代的最后几个世纪没有尝试过之前；在公元三世纪，只有公式 $\binom{n}{2}=\frac{1}{2}n(n-1)$ 得到证实。印度教数学家 Bhaskara（12 世纪）知道 $\binom{n}{p}$ 的通式公式。在 Levi ben Gerson（13 世纪初）的一份手稿中发现了更系统的研究：他一次获得了 $n$ 对象 $p$ 的排列数 $V_n^p$ 的归纳公式，特别是置换的数 $n$对象，并且他阐述了相当于关系$\binom{n}{p}=V_n^p/p!$和$\binom{n}{p}=\binom{n}{n-p}$的规则（[4]，第64-65页）。但这份手稿似乎仍然不为他的同时代人所知，其结果只是在随后的几个世纪中才逐渐被数学家重新发现。至于后来的进展，我们记录一下Cardan证明了$n$元素的集合非空子集数是$2^n-1$。帕斯卡和费马在创立概率论演算时，重新发现了$\binom{n}{p}$的表达式，而帕斯卡是第一个在数和二项式定理之间观察到关系的人，这似乎从13世纪开始为阿拉伯人所熟知，而在14世纪为中国人所知，并且16世纪初在西方重新发现，连同被称为“帕斯卡三角”的系数计算的归纳法方法（[4]，第35-38页）。最终，大约在 1676 年，莱布尼茨获得了（但没有发表）“多项式系数”的广义公式，该方程被德莫弗尔独立重新发现并于 20 年后发表。

# 参考书目

1. O. NEUGEBAUER, *Vorlesungen über die Geschichte der antiken Mathematik*, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
2. S. G. MORLEY, *The Ancient Maya*, Stanford University Press, 1946.
3. B. DATTA and A. N. SINGH, *History of Hindu Mathematics*, vol. I, Lahore (Motilal Banarsi Das), 1935.
4. J. TROPFKE, *Geschichte der Elementar-Mathematik*, vol. VI : Analysis, Analytische Geometrie, Berlin-Leipzig (de Gruyter), 1924.
