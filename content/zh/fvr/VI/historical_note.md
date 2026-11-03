---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: fvr-i-vii
book_pages: 299-303
pdf_pages: 0314-0318
extraction: ocr
statements: 0
exercises: 0
content_sha256: ca30baaf846bf99e254c967ee8c9226d1d2abf1e5bb757d39b5ded6e210998bc
translated_from: content/en/fvr/VI/historical_note.md
translation_method: google
source_content_sha256: d8a5592a597762e1f275eadce1711d9ba2cf99ed118eac2fff4c293bcbbd8a29
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 0d23bd21147681ac910b5d76bc50da64a0f6f4f19dbfbd42e929e10637b4dadd
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

# 历史注记

（章V和VI）

（注意：罗马数字指的是在此注末尾找到的参考书目。）

不同阶的“无限小”（或“无限大”）之间的区别隐含地出现在关于微分演算的第一个著作中，例如在费马的著作中；它与牛顿和莱布尼茨完全阐明，具有“更高阶的差异”的理论；并且没有浪费时间之前注意到，在最简单的情况下，形式$f(x)/g(x)$在点处的表达式极限（或“真值”），其中$f$和$g$都趋于0，由泰勒给出其中展开函数邻域点被考虑（“l’Hôpital 规则”，可能归功于 Johann Bernoulli）。

除了基本情况之外，从XVII$^{th}$世纪末开始，数学家们所看到的“渐近求值”原理问题就是当$n$非常大时，对形式$\sum_{k=1}^n f(k)$的和进行精确或近似的计算；对于插值和级数的和的数值评估来说，确实需要这样的计算，就像在概率的演算中一样，其中“大数的函数”，例如$n!$或$\binom{a}{n}$发挥着重要作用。 牛顿已经在 $n$ 大时为 $\sum_{k=1}^n \frac{1}{a+k}$ 获得近似值，在计算欧拉-麦克劳林公式 (I) 中的第一个项时指示了方法和约化（在本例中）。 到本世纪末，雅各布·伯努利（Jakob Bernoulli）在《概率论》演算中的研究、集合自己到确定和$S_k(n) = \sum_{p=1}^{n-1} p^k$、$n$中的多项式中发现了形成的一般律（没有给出证明) $^4$，因而，在这些多项式的系数表达式中，第一次引入以他的名字命名的数，以及允许对它们进行计算的归纳关系((II)，p. 97)。 1730年，斯特林通过递归计算系数的过程，获得了$\sum_{k=1}^n \log(x+ka)$的渐近展开，因为$n$无限增加。

$^4$ 它们是“伯努利多项式”$B_k(x)$ 的原语。

欧拉关于级数和相关问题的决定性著作可以追溯到1730年至1745年。将$S(n) = \sum_{k=1}^{n} f(k)$放入，他将泰勒公式应用到函数$S(n)$，这给了他

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2 S}{dn^2} + \frac{1}{3!} \frac{d^3 S}{dn^3} - \cdots,
$$

他通过未定的系数的方法“反转”了一个方程，寻找形式的解

$$
S(n) = \alpha \int f(n)\, dn + \beta\, f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2 f}{dn^2} + \cdots;
$$

他因此逐项获得，

$$
S(n) = \int f(n)\, dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3 f}{dn^3} + \frac{1}{30\,240} \frac{d^5 f}{dn^5} - \cdots
$$

首先无法确定律形成系数（III $a$ 和 $d$）。但大约在 1735 年，类比多项式到线性因子的分解，他毫不犹豫地写成了公式

$$
1 - \frac{\sin s}{\sin \alpha} = \left(1 - \frac{s}{\alpha}\right) \left(1 - \frac{s}{\pi - \alpha}\right)
$$
$$
\left(1 - \frac{s}{-\pi - \alpha}\right) \left(1 - \frac{s}{2\pi - \alpha}\right) \left(1 - \frac{s}{-2\pi - \alpha}\right) \cdots
$$

并且在将两边的展开的系数等于整个级数时，他特别得到了（对于$\alpha = \pi / 2$）著名的级数$\sum_{k=1}^{\infty} \frac{1}{n^{2k}}$表达式

$\pi$幂项（III$b$）$^5$。几年后，他终于认识到，$\pi$的幂中的系数是由与他的求和公式相同的方程给出的，并认识到它们与伯努利引入的数的联系，以及与级数展开的系数的联系。 $z/(e^z - 1)$（III$g$）。

独立于欧拉，麦克劳林大约在同一时间以稍微不那么危险的方式得出了相同的求和公式，接近我们在文本中遵循的方式；他有效地迭代了“泰勒”公式，它在差异$f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$、公式的项中表达了$f(x)$，这是他通过将这些差异的泰勒展开“反转”为方法而获得的

$^5$ 1743 年，欧拉在回应各种当代批评家的意见时，给出了三角函数函数的“欧拉展开”的更合理的推导；例如，作为无限乘积的 $\sin x$ 的展开是从表达式 $\sin x = \frac{1}{2i}(e^{ix} - e^{-ix})$ 以及 $e^{ix}$ 是多项式 $\left(1 + \frac{ix}{n}\right)^n$ (III $e$) 的极限的事实导出的。

未确定系数 (IV);但他没有感知欧拉发现的系数的形成的律。

但麦克劳林像欧拉和他那个时代的所有数学家一样，将所有这些公式表示为级数展开，甚至没有研究其收敛性。 并不是说收敛级数的概念在这一时期被完全忽略了；自雅各布·伯努利以来，人们就知道调和级数是发散的，而欧拉甚至借助他的求和公式（IIIc和d）对级数的第一个$n$项求和，从而清楚地表明了这一结果；欧拉还指出，两个连续伯努利数的比率无限增加，因而，将这些数作为系数不能收敛的整个级数收敛（（IIIf），p. 357）$^6$。 但形式化演算的倾向更为强烈，即便如此，欧拉非凡的直觉也没有阻止他陷入荒谬，例如，他写下$0 = \sum_{n=-\infty}^{+\infty} x^n$((IIIf)，p. 362)$^7$。

我们已经看到（历史注记至第IV章）XIX$^{th}$世纪初的数学家们厌倦了这种肆无忌惮、毫无根据的形式主义，如何将数学分析带回严谨的方式。一旦收敛级数的概念变得精确，就需要简单的判据来显示积分的收敛性，并需要级数与已知积分或级数进行比较；柯西在他的分析代数（Va）中给出了这样的判据的数，而阿贝尔在他死后的回忆录（VI）中得到了对数收敛判据。另一方面，柯西（V b）阐明了级数的悖论，如斯特林的悖论，由应用欧拉-麦克劳林公式（通常称为“半收敛级数”）获得：他证明了如果（鉴于欧拉的注关于伯努利数）此类级数的一般项$u_k(n)$，对于$n$的固定值，随$k$无限增加，尽管如此，对于$k$的固定值，部分和 $s_k(n) = \sum_{h=1}^k u_h(n)$给出由级数“表示”的函数的渐近展开（因为$n$趋于$+\infty$），相应地，当$k$更大时更精确。

在经典数学分析的大多数计算中，可以获得函数的渐近展开的一般律形成，其中数具有任意大的项；这一事实导致了级数和渐近展开之间产生持久的混淆（至少在语言上）；以至于 H. Poincaré 在 1886 年（VIII）不厌其烦地编纂渐近展开的基本规则（继$1/x$的整数幂和$+\infty$的邻域）时，仍然使用了以下词汇： 理论共级数。只是随着来自解析数理论的渐近展开的出现，

$^6$ 由于欧拉在这里考虑的级数是为了数值计算而引入的，因此他只取开始减少的项的总和，并从项开始增加的索引中用他没有指出其起源的余数代替它们（欧拉-麦克劳林公式中的一般形式的余数直到柯西才出现）。
$^7$ 讽刺的是，这个公式紧随欧拉警告不要不加考虑地使用发散级数的段落之后的一页！

渐近展开和级数的概念之间的明确区别最终得以确立，因为在理论处理的大多数问题中，一个不能比明确寻求的展开中的项的一个非常小的数（通常只有一个）要多。

这些问题还使数学家熟悉了变量的（实数或整数）幂以外的比较尺度的使用。这个扩张首先要归功于P. du Bois-Reymond（VII）的著作，他首先系统地处理了邻域和点中函数的比较，并在非常原创的作品中认识到了比较量表的“非阿基米德”特征标，同时他以一般方式研究了积分和微分。对比关系，推导出一大堆有趣的推论（VII b）。他的证明有时缺乏清晰性和严谨性，这对 G.H. Hardy (IX) 认为正确表述 du Bois-Reymond 的结果是正确的：他的主要贡献在于认识到证明“基本函数”的集合的存在，(H) 函数，其中通常适用数学分析的运算（特别是微分）比较关系 $^8$。

$^8$ 开发这些章方法不是我们的职责，它们允许人们获得函数属于的渐近展开到某些特定类别，例如依赖于参数的某些积分型，这在数学分析中经常出现；关于这个点（特别是关于拉普拉斯和达布的重要方法），读者可以查阅已经提到的哈代的书（IX），其中包含是一个非常完整的参考书目。

(I)I。 牛顿，在圣。 P. RIGAUD，《科学家的对应》，牛津，1841 年，t。 II，p. 309-310。
(II) 雅各布·伯努利 (Jakob Bernoulli)，Ars conjectandi，巴莱，1713 年。
(III)L。 欧拉，Operaomnia (1)，t。 XIV； 分析评论。 。 。 ，莱比锡-柏林 (Teubner)，1924 年：a) Methodus Generalis summandi Progresses，p. 42-72 (=Comm. 阿卡德。彼得罗普,T. VI (1732-33)); b) De summis serierum reciprocarum, p. 73-86 (=Comm. 阿卡德。彼得罗普., t. VII (1734-35)); c) De Progressibus Harmonis 观察值，p. 87-100（同上）； d) Inventio summae cujusque seriei 。 。 。 , p. 108-123 (=通讯。 阿卡德。彼得罗普., t. VIII（1736））； e) De summis serierum reciprocarum 。 。 。论文修改。 。 。 , p. 138-155 (=杂项。 贝罗尔，t。 VII（1743））； f) 考虑进展是。 。 。 , p. 350-363 (=通讯。 阿卡德。彼得罗普., t. XI（1739））； g) De seriebus quibusdam 注意事项，p. 407-462 (=Comm. 阿卡德。彼得罗普., t. XII（1740））。
(IV)C。 麦克劳林，《流数完整论文》，爱丁堡，1742 年。
(V) A. L。 柯西：a) Cours d’Analyse de l’Ecole Royale Polytechnique, 1re party, 1821 (=Œuvres, (2), t. III，巴黎（Gauthier-Villars），1897 年； b) Œuvres, (1), t。 VIII，p. 18-25，巴黎（高蒂尔-维拉尔），1893 年。
(VI)N. H. 阿贝尔，苏弗尔，t。 II，p. 197-205，编辑。 西洛和谎言，克里斯蒂安尼亚，1881。
(VII) P. DU BOIS-REYMOND: a) Sur la grandeurrelative des infinis des functions，Ann。迪马特。 (2)，t。 IV (1871), p. 338-353; b) Ueber asymptotische Werthe、infinitäre Approximationen 和 infinitäre Auflösung von Gleichungen，数学。 安，t。 VIII (1875)，p. 362-414。
(VIII)H. 庞加莱，关于线性方程组的不可积，数学学报，t。 VIII (1886)，p. 295-344。
(IX)G. H. HARDY，无穷大的阶，剑桥小册子，第 12 期，第二版，剑桥大学出版社，1924 年。
