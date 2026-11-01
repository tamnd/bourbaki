---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: int-vii-ix
pdf_pages: 0175-0182
extraction: ocr
statements: 0
exercises: 0
content_sha256: 25058635a2162b84410f4ba476f44fc6a66e9bcf8d8de6a486ee808c14f3223f
translated_from: content/en/int/VIII/historical_note.md
translation_method: google
source_content_sha256: 8310a10c50a658cc062070acbfc343e395a3fba746d5379e0f041cac27733c15
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 93fb50c5392e1b1bb976318e61bbed018b3be95e1b84dfcd6e752722824ae0af
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（章VII和VIII）

（注：罗马数字指的是注末尾的参考书目。）

对于希腊人来说，长度、面积和体积的概念本质上是基于它们在位移下的不变性：“重合 (εφαρμόxiοντα) 相等” (Eucl. El., Book I, ‘公共的概念’ 4)；正是通过巧妙地利用这个原理，所有公式给出了经典“图形”（多边形，圆锥截面，多面体，球体等）的面积或体积，有时通过有限分解的方法，有时通过“穷举”获得(*)。用现代语言来说，可以说，希腊几何学家所做的就是证明了“集合函数”的存在性，在位移下具有加性和不变性，但仅针对非常特殊的型中的集合进行了定义。积分演算可以被认为是对扩大这些集合函数的定义范围的需要的回应，并且，从卡瓦列里到H.勒贝格，正是这种关注成为了研究分析家的首要关注点；至于位移不变性的性质，它已进入次要地位，成为双或三重积分中变量变换的一般公式的微不足道的推论，并且正交变换的行列式等于$\pm 1$。即使在非欧几里德几何中（位移的虽然群是不同的），点的视图仍然是相同的：一般来说，黎曼德

(*) 可以证明，如果两个平面多边形 P、P' 具有相同的面积，则存在两个多边形 R ⊃ P、R' ⊃ P'，每个多边形都可以分解为有限数个多边形 R_i (resp. R'_i) (1 ≤ i ≤ m)，且没有公共的内部点，使得 R_i 和 R'_i 可以为通过位移（取决于 i）相互推导，并且使得 R（分别为 R'）是有限多边形族 S_j（分别为 S'_j）（0 ≤ j ≤ n）的并，没有公共的内部点，其中 S_0 = P、S'_0 = P'，并且 S'_j 可通过 S_j 的位移获得 1 ≤ j ≤ n。然而，M. DEHN 证明（Ueber den Rauminhalt, Math. Ann., 55 (1902), 465–478）这个性质对于多面体的体积不再有效，因此从 EUDOXUS 开始使用的穷举方法是不可避免的。

通过经典的欧氏公式，对面积或体积的无穷小元素（或它们的维数$\geqslant 3$的类似物）进行细化，从$ds^2$开始，并且它们在使$ds^2$不变的变换下的不变性因此几乎是同义反复。

直到 1890 年左右，随着“积分不变量”理论的发展，尤其是 H. Poincaré 和 E. Cartan 的发展，群下才出现了其他较少的直接的扩张测度不变量概念； H. Poincaré 只考虑了在空间的一部分中运行的一个参数群，而 E. Cartan 首先对位移的群感兴趣，但在空间中运行，而不是定义它们的地方。对于例，他因此确定了（II）不变量（在位移群下）在$\mathbf{R}^2$或$\mathbf{R}^3$线的空间上的测量（*）；此外，他指出，一般来说，李群的积分不变量不是别的，正是特定的微分不变量，因此可以通过李的方法来计算所有确定。然而，在 1897 年 A. Hurwitz 的基础工作（V）之前，似乎没有人考虑过或使用群本身的不变测度。寻求正交群下的形式多项式（在$\mathbf{R}^n$上）不变，Hurwitz从注开始，对于有限群线性变换，通过取任意变换$s \cdot \mathrm{P}$的*平均值*立即求解问题群的所有元素$s$的多项式P，这给了他对于正交群，替换关于不变测度的积分的平均值的想法；他在参数表示的帮助下通过欧拉角明确给出了后者的表达式，但立即观察到（独立于E.嘉当）李的方法对于每个李群产生了不变测度的存在。也许是由于20世纪初不变理论的衰落，赫尔维茨的思想几乎没有得到任何直接的的回应，直到1924年以后才被利用，用扩张压缩群，由I。 Schur 和 H. Weyl，关于 Frobenius 的线性表示和有限群的经典理论。前者将自己限制在正交群的情况，并展示了Hurwitz的方法如何允许扩展特征标的经典正交关系，H. Weyl将这一想法与E. Cartan关于半单李代数的工作结合起来，以获得不可约表示的特征标的显式表达式紧李群和定理的完全还原性 (XI *a*))，然后，通过“正则表示”概念的大胆扩张，著名的 Peter-Weyl 定理，完美模拟了正则表示的分解。

(*) 平面线空间上的不变测度已经在“几何概率”中与问题相关联而得到了本质上的确定，特别是由 CROFTON 确定，当时 E. CARTAN 可能还不知道他的作品。

有限群 (XI, b)) 理论中的不可约成分。

一年前，O. Schreier 创立了拓扑群的一般理论，从那时起，很明显，Peter-Weyl 回忆录中的论点对于每个可以定义“不变测度”的拓扑群仍然有效。事实上，当时拓扑和测度的一般概念还处于快速发展阶段，无论是希望在其上得到定义不变测度的拓扑群范畴，还是要定义这种“测度”的集合，似乎都没有明确的界定。唯一明显的点是，人们不能希望扩展对于一般情况来说无穷小方法证明存在李群上的不变测度。现在，从勒贝格测度的工作中发展出来的另一个潮流，恰恰导致了更直接的方法攻击。 Hausdorff 在 1914 年证明，不存在加法集合函数，但不完全相同的零，它是为 $\mathbf{R}^3$ 的 $\textbf{all}$ 子集定义的，并且在位移下不变，因此很自然地要研究这个结果是否也适用于 $\mathbf{R}$ 和$\mathbf{R}^2$：问题，S. Banach 在 1923 年以令人惊讶的方式解决了这个问题，相反，它表明这样的“度量”确实存在（I）；他的方法非常巧妙，已经基于构造和超限归纳，并考虑了函数和元素翻译的“手段”$\frac{1}{n} \sum_{k=1}^n f(x + \alpha_k)$和群（*）。正是类似的想法使得 A. Haar 在 1933 年 (IV) 采取了决定性的一步，通过证明，存在局部紧凑群的不变测度，以及开集合的可数基：在经典积分中，由近似体积的方法引导演算，通过并置任意小的全等立方体，借助对角线方法，他获得了“近似测量”的序列的不变测度，即极限，这一过程本质上是我们在第1章中使用的过程。 VII, §1。这一发现产生了非常大的影响，特别是因为它立即使 J. von Neumann 能够通过纯拓扑性质（不包括预先给出的所有微分结构）来求解紧凑群，著名的希尔伯特“第 5 问题”关于李群的刻画的问题。然而，人们立即意识到，为了有效地利用不变测度，不仅需要知道它的存在，而且还需要知道它在常数因子范围内是唯一的；这个点首先由J. von Neumann针对紧凑群证明，使用方法通过连续函数的“均值”定义哈尔测度，类似于Banach (VII a))；然后是 J. 冯·诺依曼

(*) J. von NEUMANN 在 1929 年表明，一方面 $\mathbf{R}$ 和 $\mathbf{R}^2$ 之间的行为差异，另一方面 $n \geq 3$ 的 $\mathbf{R}^n$ 行为差异的根本原因可以在空间旋转的群的交换律中找到$\mathbf{R}^2$。

(VII b)) 和 A. Weil (X)，通过不同的方法，同时获得局部紧致群情况下的唯一性，同时 A. Weil 指出了如何将 Haar 的方法扩展到一般局部紧致群。 A. Weil (loc. cit.) 也因齐次空间上存在相对不变的测度而获得了条件，并最终证明了 Hausdorff 拓扑群上存在一个“测度”（具有合理的性质），这意味着群是局部预紧的。这项工作基本上完成了Haar测度的一般理论；最近唯一被引用的加法是准不变测度的概念，该概念在1950年左右几乎没有被识别出之前，与希尔伯特空间的局部紧致群的表示理论有关。

卷积乘积的历史更为复杂。从 19 世纪初开始，人们发现，如果对于例，F(x, t) 是 x 和 t 中线性且具有常系数的偏微分方程的解，则

$$
\int_{-\infty}^{+\infty} F(x - s, t) f(s) \, ds
$$

也是同一个方程的解；自之前 1820 年起，泊松等人就用这个想法在形式中写出了热方程的解

(1)
$$
\int_{-\infty}^{+\infty} \exp \left( - \frac{(x - s)^2}{4t} \right) f(s) \, ds.
$$

过了一会儿，表情

(2)
$$
\frac{1}{2\pi} \int_{-\pi}^{+\pi} \frac{\sin \frac{2n+1}{2}(x-t)}{\sin \frac{x-t}{2}} f(t) \, dt
$$

对于傅里叶级数的部分和，以及狄利克雷对这个积分的极限的研究，当n趋于$+\infty$时，提供了环面$\mathbf{T}$上“正则化”$f \mapsto \rho_n * f$的第一个例（实际上，通过非正“核”的序列，这使研究变得非常复杂）；在“奇异积分”的名义下，类似的积分表达式是 19 世纪末和 20 世纪初分析师们（从 P. du Bois-Reymond 到 H. Lebesgue）选择的主题。在$\mathbf{R}$上，Weierstrass在定理的证明中利用了多项式近似的积分(1)，并就此给出了形式的正‘核’$\rho_n$的序列正则化的一般原理 $x \mapsto c_n \rho(x/n)$。在$\mathbf{T}$，最著名的正核正则化例稍后由Fejér给出，从这一刻起，它是标准程序，即函数的级数的大多数“求和方法”的基。

然而，这些工作由于“核”和函数正则化所扮演的角色不对称，几乎没有揭示卷积乘积的代数性质。我们首先要感谢 Volterra 对这个点的重视。他对两个变量的两个函数的‘合成’$F * G$进行了概括研究

$$
(F * G)(x, y) = \int_x^y F(x, t)G(t, y)\, dt,
$$

他将其视为推广，“通过从有限到无限的过渡”，两个矩阵（IX）中的乘积。他很早就提出了 F 和 G 仅依赖于 $y - x$ 的情况（称为“闭环”，因为它在遗传理论中的解释）； $H = F * G$也是如此，如果集合$F(x, y) = f(y - x)$，$G(x, y) = g(y - x)$，那么

$$
H(x, y) = h(y - x),
$$

在哪里

$$
h(t) = \int_0^t f(t - s)g(s)\, ds,
$$

因此，对于$t \geq 0$，$h$重合与函数$f_1, g_1$的卷积分别等于$t \geq 0$时的$f$和$g$，以及$t < 0$时的0。

然而，Volterra发展的代数形式主义并没有揭示$\mathbf{R}$与群结构和傅立叶变换的联系。这里不是讲述后者历史的地方；但对于注来说，从柯西开始，处理傅立叶积分的分析家们首先致力于寻找更宽的条件来证明各种“反演”公式的有效性，而在某种程度上忽略了它的代数性质。对于傅里叶本人的著作（或拉普拉斯关于类似积分$\int_0^{+\infty} e^{-st} f(t)\, dt$的著作），我们当然不能说同样的话；但这些变换本质上是与线性问题相关的，因此，很长一段时间之前有人想到考虑两个傅里叶变换的乘积（除了三角函数级数或幂级数的乘积例外，这并不奇怪，但是与离散测量的卷积的联系显然在 19 世纪是无法被感知的）。第一次提到这个乘积和$\mathbf{R}$上的卷积可能是在Tchebychef (VIII)的回忆录中找到的，与概率论问题有关。事实上，在这个理论中，两个“概率的律”在$\mathbf{R}$（总质量1的正测量）上的卷积$\mu * \nu$正是$\mu$和$\nu$的“组合”概率律（对于相应的的“随机”加法）变量”）。可以肯定的是，对于 Tchebychef 来说，这仍然只是一个概率律具有密度（相对于勒贝格测度）的卷积问题，因此是函数的卷积问题；而且，它只以片段的方式出现在他的作品中，在1920-1930年期间之前出现的几部罕见作品中也是如此。 1920 年，P. J. Daniell 在当时很少被注意到的注 (III) 中定义了这种测度的 $\mathbf{R}$ 和傅里叶变换上两个任意测度的卷积，并明确观察到傅里叶变换将卷积转移到了普通的乘积——从 1925 年开始，这种形式主义被认为是一种形式主义。被概率学家广泛使用，特别是在 P. Lévy 之后。但卷积在群理论中的根本重要性直到1927年才被H. Weyl充分认识到；他注意到，对于紧凑的群，函数的卷积在有限群的代数中扮演了乘法的角色，允许他随后定义得到“正则表示”；同时，他在正则化中发现了单位元元素相当于代数或有限群。剩下的工作就是对所有这些点的观点进行综合，这在A. Weil的书中完成（X），一方面为后来构成I的后来的推广铺平了道路。 Gelfand 的范数代数理论，以及分布的卷积理论。

Haar 测度和卷积已迅速成为代数化趋势中的重要工具，这强烈地标志着现代数学分析；我们将有机会在以后的书中开发它们的大量应用。我们在这些章中处理的唯一一个涉及局部紧致群的封闭子群（尤其是离散子群）的“变体”。这一理论源自K. Mahler 在《数几何》中的结果，并于1950 年由C 创立。 Chabauty，并且刚刚由 Macbeath 和 Swierczkowski (VII) 进行了相当大的发展和深化，我们在这里重现了他们的主要结果。

(I) S. Banach, Sur le problème de la mesure, Fund. Math., 4 (1923), pp. 7–33.

(II) E. Cartan, Le principe de dualité et certaines intégrales multiples de l’espace tangentiel et de l’espace réglé, Bull. Soc. Math. France, 24 (1896), pp. 140–177 (= Œuvres complètes, v. II₁, pp. 265–302).

(III) P. J. Daniell，Stieltjes–Volterra 乘积，国会议员。实习生。 《数学》，斯特拉斯堡，1920 年，第 130–136 页。

(IV) A. Haar, Der Massbegriff in der Theorie der kontinuierlichen Gruppen, Ann. of Math., (2), 34 (1933), pp. 147–169 (= Gesammelte Arbeiten, pp. 600–622).

(V) A. Hurwitz，Ueber die Erzeugung der Invarianten durch Integration，Gött。 Nachr.，1897 年，第 71–90 页（= Math. Werke，v. II，第 546–564 页）。

(VI) A. M. Macbeath, S. Swierczkowski, Limits of lattices in a compactly generated group, Canad. J. Math., 12 (1960), pp. 427–437.

(VII) J. von Neumann, a) Zum Haarschen Mass in topologischen Gruppen, Comp. Math., 1 (1934), pp. 106–114 (= Collected Works, v. II, n° 22); b) The uniqueness of Haar’s measure, Mat. Sbornik, 1 (43) (1936), pp. 721–734 (= Collected Works, v. IV, n° 6).

(VIII) P. Tchebychef, Sur deux théorèmes relatifs aux probabilités, Acta. Math., 14 (1890), pp. 305–315) (= Œuvres, v. II, pp. 481–491).

(IX)V。 Volterra，Leçons sur les fonctions de lignes，巴黎（Gauthier-Villars），1913 年。

(X) A. Weil，L’在群拓扑和应用中的集成，实际。科学。 et Ind.，n° 869，Paris，Hermann，1940（2e ed.，同上，n° 869-1145，Paris，Hermann，1953）。

(XI) H. Weyl，a) Theorie des Darstellung kontinuierlicher halbeinfacher Gruppen durch Lineare Transformationen，数学。 Zeit., 23 (1925)，第 271–309 页、24 (1926)，第 328–395 页和 789–791（= Selecta，巴塞尔–斯图加特 (Birkhäuser)，1956 年，第 262–366 页）； b) (与 F. Peter) Die Vollständigkeit der Primien Darstellungen einer geschlossenen kontinuierlichen Gruppe，数学。 Ann.，97 (1927)，第 737–755 页（= Selecta，第 387–404 页）。
