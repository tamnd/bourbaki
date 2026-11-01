---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0296-0311
extraction: ocr
statements: 0
exercises: 0
content_sha256: f85fb544a8ce770a3bf552d0e61d62daeb783f14b58a5317e2c871e4fe630aa4
translated_from: content/en/alg/V/historical_note.md
translation_method: google
source_content_sha256: d3d8e5cd03c57035d1df9857d0aef27c2b8331659af5500d9a8d3e0120dca43a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 84d618280c461bc9de078697dbf21e5a0dd7fc9e828e1718dea3ee43a0a16151
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（章IV和V）

（括号内的数指本注末尾的参考书目。）

交换域理论以及与之密切相关的多项式理论，直接源自直到 19 世纪中叶为止构成代数方程的经典代数 : 解以及与它们等价的几何构造的问题主要对象的理论。

一旦人们试图求解次数 $> 1$ 的代数方程，人们就会发现自己面临着全新的计算困难，因为不再可能通过对数据执行“有理”计算来求解确定未知数。这个困难一定是在很早的阶段就被意识到的；巴比伦人最重要的贡献之一是，他们能够将二次和双二次方程的约化解转化为一个新的代数运算，提取平方根（正如我们在流传下来的文本中发现的以这种方式求解的许多数值方程所示） （[1]，p. 183-193））。就形式计算而言，古代代数方程的解中的问题从来没有超出过这个点；古典时代的希腊人实际上仅限于用几何项重述巴比伦的公式，并且他们在代数形式中的使用没有记录之前希罗（公元100年）和丢番图。

希腊人却在一个完全不同的方向上取得了决定性的进步。我们对巴比伦人如何构思和计算平方根或整数的信息知之甚少，平方并不完美\*；在我们收到的关于这个问题的罕见文本中，他们似乎满足于相当粗略的方法近似值（[1], p. 33-38）。毕达哥拉斯学派学校相当严格地确定了可通约量的概念，并为其附加了准宗教的特征标，但无法坚持这种点的观点；可能正是由于多次尝试理性地表达$\sqrt{2}$的失败，才导致他们最终证明了这个数是非理性的**。

\* 在巴比伦文本中所有二次和双二次方程的例中，数据的选择总是使得根式适用于完美的平方。
** 最近的一位作者提出了毕达哥拉斯学派所熟知的正五角星的巧妙的注构造（对于他们来说这是他们的神秘符号之一），

We have said elsewhere (cf. Hist. Note to Book III, Chapter IV) how this discovery, which marks a watershed in the history of Mathematics, reacted profoundly on the conception of « number » among the Greeks, and led them to create an algebra of exclusively geometrical character, in order to find a mode of representation (or perhaps an « existence » proof) for the incommensurable ratios, which they refused to consider as numbers. Most frequently an algebraic problem was reduced by them to the intersection of two auxiliary plane curves, appropriately chosen, or to several successive determinations of such intersections. Late traditions of little authority ascribe to Plato the introduction of a first classification of these constructions, destined to a long and brilliant career : for reasons that are philosophical rather than mathematical, it seems, that what are known as « ruler-and-compass-constructions », that is those where the only auxiliary curves occurring are straight lines and circles, have been put on one side *. In any case Euclid in his Elements [2] limits himself exclusively to treating problems that can be solved in this fashion (without however characterizing them by a particular name); a circumstance which undoubtedly contributed no little to fix the attention of mathematicians of succeeding centuries on these problems. But we know today ** that the algebraic equations that may be solved « by ruler and compasses » are of a very special type ; in particular, an irreducible equation leads immediately to a demonstration of the irrationality of $\sqrt{5}$, and he has put forward the hypothesis (which unfortunately is not supported by any text) that it was in this fashion that the Pythagoreans discovered irrational numbers (K. von Fritz, Ann. of Math., vol. 46 (1945), p. 242).

\* 与此原理相关，柏拉图还把平面曲线分类为“平面轨迹”（直线和圆）、“实体轨迹”（由固体平面截面获得的圆锥曲线，圆锥），所有其他曲线都以“τόποι γραμμικοί”的名称分组在一起。令人好奇的是，这种分类的影响甚至延伸到笛卡尔，他在他的《几何学》中将次数$2n - 1$和$2n$的方程排列在同一个“属”中，毫无疑问，因为次数1或2的方程可以通过“平面轨迹”的交求解，而次数3或4的方程可以通过«固体位点»的交。

** 确定直线和圆（或两个圆）的交的点相当于求第二个次数方程的解，其系数是所考虑的直线和圆（或两个圆）方程的有理数函数。很容易得出，点的坐标由给定的点属于到有理数的域Q的扩张L，按如下方式获得：如果K是通过与Q邻接给定的坐标获得的域点，则域之间存在递增序列$(L_i)_{0 \leq i \leq n}$中间K和L，$1 \leq i \leq n$存在满足条件$K = L_0, \quad L = L_n, \quad [L_i : L_{i-1}] = 2$。通过n上的归纳，我们推导出L生成的伽罗瓦扩张N的K上的次数是2的幂；反之，可以证明，如果条件成立，则在K和L之间存在域的序列$(L_i)$，具有上述性质，因此问题可以通过直尺和圆规来求解（cf.N. Tschebotarow，Grundzuge der）伽罗瓦理论 (transl. H. Schwerdtfeger), 格罗宁根 (P. Noordhoff), 1950, p. 351)。

第三个次数的（超过有理数的域）不能就是这样解决的，希腊人很早就遇到了第三个次数的问题，这些问题至今仍然著名，例如立方体的复制（$x^3 = 2$的解）和角的三等分；另一方面，圆的正交使它们面临着超越的问题。我们发现，为了解决这些问题，他们引入了许多曲线，包括代数曲线（圆锥曲线、戴奥克勒斯曲线、尼科梅德贝壳曲线）和超越曲线（迪诺斯特拉图斯四边形、阿基米德螺线）；这一切不可避免地导致他们对这些不同的曲线进行独立的研究，从而为解析几何、代数几何和无穷小演算的未来发展铺平了道路。但这些方法对代数方程的解没有任何进展*，唯一对这个问题做出了显着贡献并对中世纪和文艺复兴时期的代数学家产生持久影响的古代著作是欧几里得的元素的书X[2]；在这本书中（其中的主要结果被某些历史学家归咎于泰阿泰德），他考虑了由几个部首组合而成的表达式，例如$\sqrt{\sqrt{a} \pm \sqrt{b}}$（a和b有理数），给出了条件，在这些表达式下这些表达式是无理数，将它们分类为许多类别（他证明了这些类别是不同的），并研究了这些不同无理数之间的代数关系，例如我们将要讨论的那些今天写为

$$
\sqrt{\sqrt{p} + \sqrt{q}} = \sqrt{\frac{1}{2} (\sqrt{p} + \sqrt{p-q})} + \sqrt{\frac{1}{2} (\sqrt{p} - \sqrt{p-q})}
$$

一切都用*元素*这种常用的几何语言来表达，这使得阐述显得特别密集和尴尬。

之后古典希腊数学的衰落概念与代数方程相关的经历了修改。毫无疑问，在整个古典时期，希腊人拥有无限近似于平方根的方法，不幸的是，我们对此了解甚少**。

\* 由于缺乏可管理的代数方法计算方法，人们在希腊人中找不到任何对他们无法用直尺和圆规解决的问题分类的尝试；阿拉伯人是第一个使用约化众多问题（对于7或9条边的正多边形的例构造）到第三个次数的方程。

** For example, Archimedes' method for the approximate calculation of the number $\pi$ necessitates a knowledge of several square roots to a fairly good approximation, but we are ignorant of the procedure employed by Archimedes to obtain these values. The method of approximation of $\sqrt{2}$ which provides the expansion of this number as «continued fraction» is known (in geometric form) from a text by Theon of Smyrna (2nd century AD), but perhaps goes back to the first Pythagoreans. As regards the method of indefinite approximation of square roots which is still in use today in elementary teaching, this is not documented before Theon of Alexandria (4th century AD), even though it was no doubt known to Ptolemy. We note finally that an approximate calculation of a cube root is found in Hero (ca. 100 AD) (cf. G. Eneström, *Bibl. Math.* (3), vol. VIII (1907), p. 412).

对于印度教徒、后来的阿拉伯人和他们中世纪的西方模仿者来说，从所有阶中提取根就变成了运算，它往往被认为是基本的，与代数的有理数运算具有相同的权利，并且像后者一样，用在计算中越来越容易处理的符号来表示*。中世纪完善的第二次数方程理论（根的数，负根，不可能性情况，双根），以及双二次方程理论，为解方程提供了公式模型 «根式”，几个世纪以来，代数学家们一直在尝试为更高次数的方程的解建立类似的公式模型，首先是为第三次次数的方程建模。比萨的莱昂纳多在 13 世纪主要负责向西方介绍阿拉伯科学，他认识到无论如何，欧几里得在其第十本书不能中分类的无理数都可以用于此目的（一种新的不可能性证明，在一个充满它们的理论中），我们看到他已经尝试了立方体根的类似计算，得到关系比如

$$
\sqrt[3]{16} + \sqrt[3]{54} = \sqrt[3]{250},
$$

类似于欧几里得的公式代表平方根（我们实际上在阿拉伯人中发现了更早的例）。但三个世纪徒劳无功的努力仍需经过之前，西庇阿·德尔·费罗 (Scipio del Ferro) 在 16 世纪初，终于得出了等式$x^3 + ax = b$的解的公式：

(1) $$
x = \sqrt[3]{\frac{b}{2}} + \sqrt{\left( \frac{b}{2} \right)^2 + \left( \frac{a}{3} \right)^3} + \sqrt[3]{\frac{b}{2}} - \sqrt{\left( \frac{b}{2} \right)^2 + \left( \frac{a}{3} \right)^3}.
$$

我们在这里避免描述这一耸人听闻的发现的风景如画的一面——它一方面引发了塔尔塔利亚，另一方面卡尔达诺和他的学校之间的争吵——以及作为主角的学者们经常引人入胜的人物。但我们必须注在卡尔达诺和他的学生手中在方程理论方面取得了决定性的进展。卡尔达诺比大多数同时代人更不厌恶使用负数，因此观察到第三个次数的方程可能有三个根，而双二次方程四个（[3]卷IV，p. 259），他的注 $x^3 + bx = ax^2 + c$的三个根中的和（他知道如何使$x^2$中的项消失）始终等于a（同上）。毫无疑问，在这个关系和它的一般性特征标的直觉的引导下，他有了第一个关于重数或根的概念的想法；最重要的是，他有勇气（并非没有演讲预防措施），正式用表达方式计算表达包含

\* 当 a 为整数（不是完美的 n 次幂）时，$\sqrt[n]{a}$ 的无理性既没有被提及也没有被证明之前 Stifel（16 世纪）；后者的证明是以欧几里得的$n = 2$为蓝本的，这个简单的推广很可能没有被早期注意到。

平方根负数。很可能他是因为这样的事实而导致的：当$\left( \frac{b}{2} \right)^2 + \left( \frac{a}{3} \right)^3 < 0$（所谓的“不可约情况”，其中卡尔达诺认识到三个实数根的存在）时，使用公式（1）时自然会出现这样的表达式；无论如何，他的弟子 R. Bombelli 清楚地指出了这一点，他在代数 ([4], p. 293) 中证明了关系

$$
\sqrt[3]{2 + \sqrt{-121}} = 2 + \sqrt{-1}
$$

谁细心地给出了形式中复数的计算规则，这已经非常接近现代的阐述*。最后在1545年另一个卡尔达诺的学生，L。法拉利，借助第三次次数**的辅助方程，成功求解了第四次次数的一般方程。

之后如此迅速的进步，随后的时期，直到18世纪中叶，几乎没有发展出意大利人学校引入的新思想。由于他给代数记号带来的重要进展，Vieta能够以一般方式表达代数方程的系数和根之间的关系，至少当根均为正***时（[5]，p. 158）。更大胆的是，A. Girard [6] 毫不犹豫地断言（当然没有证明）次数 $n$ 的方程恰好有 $n$ 根，只要计算了“不可能的根”，每个方程都有重数的次数，并且这些根满足关系由 Vieta 提供；他还首次得到了和等于幂等于根的表达式，直到指数4。

但17世纪的精神转向了其他方向，代数只是间接地从解析几何和无穷小演算的新发现中获得了一些好处。因此笛卡尔的方法获得

\* Bombelli ([4], p. 169 和 190) 将复数视为具有正系数的 « 线性组合 »，其中四个基元素 : « piu » (+ 1), « meno » (− 1), « piu de meno » (+ $i$) 和« meno de meno » (− $i$);特别是，他假设了一个公理，即“piu”和“piu de meno”不能相加，这是线性独立性概念的首次出现。

** 等式简化为形式 $x^4 = ax^2 + bx + c$，我们确定数 $z$ 使得等式右边

$$
(x^2 + z)^2 = (a + 2z)x^2 + bx + (c + z^2)
$$

是一个完美的平方，它给出了$z$的第三个次数的方程。

*** 维埃塔（Vieta）是古人的狂热崇拜者，他系统地避免在他的论点中引入负面的数；尽管如此，当后者中的某些为负时，他有时仍能够用他的语言表达系数之间的关系和根；对于例，如果方程 $x^3 + b = ax$ 有两个正数根 $x_1, x_2$ ($a > 0, b > 0$)，Vieta 表明$x_1^2 + x_2^2 + x_1x_2 = a$ 和 $x_1x_2(x_1 + x_2) = b$ ([5], p. 106)。

代数曲线的切线（cf. Hist。注到书IV，第I-II-III，p. 46）与代数方程的根的重数准则有关，由他的弟子陈述胡德 ([7], p. 433 和 507-509)。毫无疑问，代数函数和超越函数之间的区别也应该归因于笛卡尔的影响，这与他在《几何》中介绍的“几何”曲线和“机械”曲线类似（cf.历史。注到书IV，第1章）。 I-II-III、p. 46 和 61）。无论如何，J. Gregory 完全清楚地阐明了这种区别，他在 1667 年甚至试图证明扇形的面积不能是弦和半径 * 的代数函数。 “先验”一词源自莱布尼茨，他在整个职业生涯中从未停止对这些分类问题感兴趣，并且他于 1682 年左右发现了格雷戈里所追求的结果的一个简单的证明，即证明，即 sin x 不是 x 的代数函数（[8]，第 V， p. 97-98)**。莱布尼茨和他的朋友 Tschirnhaus 实际上是他那个时代少数仍然对代数方程“根式”的问题或解感兴趣的数学家之一。在他一开始，我们发现他研究了第三次次数方程的“不可约情况”，并说服自己（碰巧，证明不足）在这种情况下不可能从解的公式消除虚数（[9]，p. 547-564）。大约在同一时间，他用五次方根式次数攻击解，但也没有成功；后来 Tschirnhaus 声称通过变换形式 y = P(x)（其中 P 是适当选择的第四次次数多项式），使除两个极端之外的所有项都消失来求解问题时，莱布尼茨立即注意到方程中的确定 P(x) 的系数次数 > 5，并且认为方法注定会失败（[9]，p. 402-403）。

似乎是新的数学分析的需要，逐渐重新燃起了对代数的兴趣。莱布尼茨和约翰·伯努利对有理分式的积分，以及与之密切相关的虚对数问题，提供了一个机会来更深入地发展虚数数的计算，并再次将多项式的分解问题转化为第一个次数的因子（《基本定理》）海藻-

\* J. Gregory，Vera Circuli et Hyperbolae Quadratura...，Pataviae，1667； cf. G. 海因里希，圣经。数学（3），卷。 II (1901)，p. 77-85。

** 莱布尼茨在《超越量》中给出的定义（[8]，卷V，p. 228；另见同上，p. 120）似乎适用于函数而不是数（用现代语言来说，他所做的相当于定义了超越元素）将有理数的域邻接问题的数据得到域）；然而，他很可能对超验的数有相当清晰的概念（甚至虽然，后者似乎在18世纪末也没有以精确的方式定义之前）；无论如何，他明确地观察到，超越的函数可以为变量的有理值假设有理值，因此他对sin x的超越的证明不足以证明$\pi$是无理的（[8]，第V，p. 97和124-126）。

胸罩»）*。就在18世纪初，二项式方程$x^n - 1 = 0$的解被Cotes和de Moivre简化为将圆除以$n$等于部分；因此，要获得其根 « 通过根式 » 的表达式，只要知道当 $n$ 是奇素数时如何做到这一点就足够了，并且 de Moivre 注代换 $y = x + \frac{1}{x}$ 然后约化问题到解 « 通过根式 » 的方程次数$(n-1)/2$。就“基本定理”而言，之后“激进式”一般解的反复失败（包括欧拉[10]的几次尝试），努力开始倾向于先验证明，而不是使用解的显式公式。无需进入方法提议的细节（这将在拉格朗日和高斯的证明中结出果实；cf.历史。注到书II。第VI-VII和书III，第7章）。 VIII），这里的注适合从18世纪中叶看到问题的角度看点；承认（除了模糊的普遍性感觉之外，没有任何理由，毫无疑问，就像A. Girard一样，从系数和根之间存在关系）次数$n$的方程总是有$n$“理想”根，其计算可以如下进行数，不知道它们是数（实数还是复数）；需要证明的是（如果需要的话，可以对理想的根进行计算），这些根中至少有一个是普通的复数**。在这个有缺陷的形式中，可以认识到“形式伴随”一般思想的第一个萌芽，尽管高斯有反对意见（[13]，第III。p. 1），但它最终成为了交换域现代理论的基。

随着拉格朗日 (Lagrange) ([11], a) 和范德蒙德 (Vandermonde) [12] 的基本回忆录的出现，1770 年见证了代数方程历史上一个新的、决定性的时期的开始。或多或少幸运地尝试找到公式或解的经验主义，在此之前一直是不可分割的，随后是系统性的数学分析和问题的提出以及能够解决它们的方法，数学分析在六十年内导致了伽罗瓦的最终结果。拉格朗日和范德蒙德都是从次数$\leq 4$方程的解的公式中根式的倍数确定引入的歧义出发；这一事实已经引起了欧拉 ([lo], a) 的注意，他除其他外还展示了如何在 del Ferro 的公式中将出现的部首关联起来，以获得 3 根而不是 9。拉格朗日指出，del Ferro 的公式中的每个立方体根可能是

\* 当人们看到莱布尼茨（他是当时数学家中最常使用该技术的人之一）表达自己好像不可能将 $x^4 + 1$ 分解为第二个次数的两个实数因子时，人们就可以很好地了解当时复数计算的基本状态（[8]，第 1 卷）。 V，p. 359-360）。

** 需要说明的是，18世纪数学家所说的“虚数根”往往只是上面的“理想”根；他们试图证明这些根是形式$a + b \sqrt{-1}$（参见例[11]，b）。

用形式$\frac{1}{3} (x_1 + \omega x_2 + \omega^2 x_3)$写成，其中$\omega$是所提出方程的单位元和$x_1, x_2, x_3$根的立方根，在某个阶中取，并且他做出了基本观察，即三个中的函数$(x_1 + \omega x_2 + \omega^2 x_3)^3$对于三个根中的每个*置换*，根只能采用*两个*不同的值，这解释了这个等式中方法或解的*先验*成功。 第四个次数方程的解的方法的类似数学分析导致他得到四个根中的函数$x_1 x_2 + x_3 x_4$，对于根的每个置换只需要*三个*不同的值，因此第三个次数的方程的根，其系数在给定方程的系数中是有理数函数*；这些事实构成了拉格朗日所说的“*真实的原理，可以说，第三和第四个次数方程的解的形而上学* **”（[11]，*a*），p. 357）。 在这些例的指导下，他计划总体研究次数 $n$ 数 $v$ 的值 *** 的方程，当后者任意排列时，$n$ 根的有理函数 V 可以假设。 ;因此，他实际上开创了（在这个术语中仍然紧密地适应于方程理论）群和域的理论，其中他已经通过使用与今天所使用的相同的原理获得了几个基本结果。 对于例，他证明数$v$是$n!$的除子，通过推理，今天可以证明有限群除阶的子群阶群。 更值得注意的是定理，其中他证明，如果$V_1$和$V_2$是根的两个有理数函数，使得$V_1$和$V_2$在相同的置换下保持不变，那么其中一个是另一个的有理数函数，并且方程的系数（特殊情况）伽罗瓦的定理将伽罗瓦扩张的子扩展描述为伽罗瓦群的不变量的域）：“*这个问题*”他说“*对我来说似乎是最重要的方程理论之一，我们将给出的一般解将有助于对此提出新的见解部分 / 代数* » ([11], *a*), p. 374)。

在拉格朗日看来，所有这些研究自然是代数方程中可能的方法或解的数学分析的预兆，通过连续简化为较低的次数方程，如他所表明的，方法与根的有理函数的形成有关，需要更少的时间比$n$值低于置换或根。毫无疑问，在第三次次数方程的结果的指导下，他一般性地引入了“拉格朗日求解器”$y_k = \sum_{h=1}^n \omega_k^h x_h$，其中

\* Waring also makes this observation in his Meditationes algebraicae, published in that same year 1770, but he is far from drawing the same conclusions as Lagrange.
** In this word, flowing so frequently from the pen of 18th century authors, may be discerned a first (still very vague) glimpse of the modern concept of *structure*.
*** Lagrange already makes a distinction between the different *rational fractions* obtained from $V$ by permuting the indeterminates $x_i$ ($1 \leq i \leq n$), and the different *values* these fractions take when the $x_i$ are roots of an algebraic equation with given numerical coefficients ; but there still subsists in his exposition a certain hesitation on this subject, and it is only with Galois that the distinction becomes clear-cut.

ω_k 是单位元的第 n 个根 (1 ≤ k ≤ n)，清楚地表明这些 n 数的知识如何蕴含根 x_k 的知识，并检查 y_k 所满足的方程的一般次数；他证明，对于例，如果 n 是素数，则 y_k^n 是次数 n − 1 方程的根，其系数是次数 (n − 2) 方程的根有理数函数！其系数可以通过给定方程的系数合理地表达。 «这里，除非I错了»他结论，«是方程解的真实原理，而数学分析最适合引导我们到达那里；正如我们所看到的，一切约化都是一种演算的组合，通过这种组合，人们可以先验地找到我们应该期望的结果»（[11]，a），p. 403）。

至于范德蒙德的回忆录，独立于拉格朗日的虽然，它在点的数与后者有联系，特别是在研究根的有理函数的思想中，在根的置换下采取尽可能少的不同值*，以及他为此目的还介绍的“拉格朗日解析”的研究。他的工作远没有拉格朗日的工作那样清晰和概括。然而，在点上，他显然走得更远，在应用中，对于圆的分割方程 x^n − 1 = 0（n 为奇素数）有相同的想法。虽然拉格朗日满足于回忆这个方程约化到具有有理系数的次数 m = (n − 1)/2 的方程，而没有尝试在 n ≥ 11 时求解它，但范德蒙德确认后一个方程的拉格朗日解方程的 m 个幂是有理数，因为各个方程之间的关系 x^n − 1 = 0 的根；但他仅限于验证 n = 11 时断言的充分根据，而没有普遍证明它的合理性。

仅仅三十年后，范德蒙德公布的结果才被C彻底证明。 F.高斯**。他对方程 x^n − 1 = 0（n 为奇素数）的决定性结果符合他令人难忘的算术研究（[13]，卷 I、p. 413 等）的一般程序，并且它们特别说明了他对我们现在所说的循环群理论的掌握。 之后证明了多项式 Φ_n(x) = (x^n − 1)/(x − 1) 对于奇素数 n *** 是不可约的，他有了将 n − 1 根写成形式的想法

\* 在这个研究（实际上他只为第5次次数的方程展开）中，首次出现了不原性的概念（[12]，p. 390-391）。人们也很容易将拉格朗日和范德蒙德的方法与他们当代关于行列式的工作进行比较，这使他们熟悉置换的概念以及与之相关的所有内容。

** 高斯在他的论文中没有引用范德蒙德，但他很可能读过后者的回忆录 (cf. [13], vol. X_2, Abh. 4, p. 58)。

*** 不可约多项式（具有有理系数）的概念可以追溯到17世纪，牛顿和莱布尼茨已经给出了允许（至少在理论上）确定具有显式有理系数的多项式的不可约因子的过程（[8]，卷IV，p. 329和355）；但高斯的证明是任意高次数多项式的第一个不可约性证明应用到整个类。

ze^{g^k} = ze_k \quad (0 \leq k \leq n - 2)，其中 g 是同余 z^{n-1} \equiv 1 \pmod{n} 的原语根 （在现代项中，它证明了方程的群 $\Gamma$ $\Phi_n(x) = 0$ 是循环的）。对于$n - 1$的每一个除子 e，他将$f = (n - 1)/e$ «周期»$\eta_v = 5, + \zeta_{v+}, + \zeta_{v+2e} + \ldots + \zeta_{v+(f-1)e}$ ($1 \leq v \leq f$)联系起来，并且他本质上证明了线性组合与由任意一个f周期生成的$\eta_v$形式域的有理系数$\eta_v$，以及有理数的次数f超过域（这个域当然是阶e的$\Gamma$对应到子群）。我们不能在这里详细介绍这个数学分析，以及它所涉及的重要算术推论；让我们仅仅注，它特别给了他著名的定理，关于“用尺子和圆规”构造具有数边数等于形式$2^{2^k} + 1$*的素数数的正多边形的可能性。至于由方程 $\Phi_n(x) = 0$ 的根式计算的解，这很容易从周期理论中得出，应用于拉格朗日解析器$\sum_{\nu=0}^{f-1} \omega^\nu \eta_\nu$（其中 $\sigma^f = 1$）** 的 f 次幂。

与拉格朗日直接相关的是他的同胞鲁菲尼的研究，与《论文集》同时期；继续解决拉格朗日留下的问题点，他们的目标是证明，即第五次数的“一般”方程不可能“由根式”实现解。鲁菲尼的证明冗长晦涩，仍然不完整，甚至虽然也经过多次修改；但它已经非常接近阿贝尔后来得到的证明（在原理中正确）****。它的主要兴趣在于引入代换的演算和群理论的第一个概念，其中

\* 高斯明确指出，他有证明的事实，这是唯一一种可以通过尺子构造并圆规具有奇数素数数边的正多边形的情况 ([13].vol.1)。 I, p. 462);但这个证明从未发表过，也没有在他的论文中找到。

** 事实上，如果我们只想证明方程可被根式解，我们可以将极限自己应用于$e = 1$，并通过归纳对$n$进行论证。

*** 通过这种方式，19 世纪的数学家本质上理解了一个方程，其系数在域有理数上“不定”。但现代的不确定性概念在19世纪末期之前才刚刚出现；在此之前，人们总是通过“多项式”或“有理分式”来理解复杂变量的*函数*。 “一般”代数方程被认为是这样一个方程，其系数是独立的复变量，其根是这些变量的“代数函数” — 概念事实上，如果人们赋予字函数 » 现在的含义，那么它实际上完全缺乏精确的含义。当然，推理与这些“代数函数”一般来说本质上是正确的，这可以通过将其翻译成现代代数语言来确定。

**** 参见 P. Ruffini，*Opere Matematiche*，第 3 卷。 Roma（Ed. Cremonese），1953-1954，以及 H. Burkhardt，*Zeitschr。数学。和物理*卷。 *XXXVII*（1892），增刊。 p. 121-159。

鲁菲尼证明，当根任意排列时，大于 2 且小于 5 值的方程的 5 个根中不存在函数。

我们已经说过（历史注至I）群或置换理论的第一个纲要是如何在几年后被柯西发展和系统化的。但是，如果拉格朗日关于代换的思想的发展所必需的概念因此而逐渐澄清，那么仍然有必要以同样清晰的方式陈述域理论的第一个原理。这正是鲁菲尼所缺乏的，而阿贝尔和伽罗瓦在代数方程的问题或解的最后阶段中承担了这一点。

在他短暂的一生中，阿贝尔从未停止过对这个问题的关注。几乎还是个孩子的时候，他就相信已经通过五次方次数的根式找到了解的公式。后来，当他认识到自己的错误时，他并没有休息，直到在证明中成功证明这样的公式不存在（[14]，卷I，p. 166）。但他并没有就此止步。虽然他的竞争对手雅可比作为分析者发展了椭圆函数理论，但代数点的观点在阿贝尔关于这个问题的工作中占主导地位，其中心是椭圆函数除法方程组理论（[14]，卷I，p. 265，377等）帕西姆）。因此，他通过模仿高斯圆分割方程的方法，得到了新的根式可解方程型（[14]，卷I、p. 310和358）*；由此他提出了“阿贝尔的”方程的概念，并在著名的回忆录中证明了根式的可溶性（[14]，卷I，p. 478）；正是在这个场合，他在给定的域（域由他正在研究的方程的系数生成）**上以精确的方式概念计算了不可约多项式的定义。最后，死亡于 1829 年击倒了他，当时他正在攻击所有根式可解方程的刻画的一般问题，并且刚刚向 Crelle 和 Legendre 传达了已经非常接近 Galois 的结果（[14]，第 II、p. 219-243、269-270 和279）。

三年后，这座建筑的加冕正是为后者保留的[15]。像阿贝尔一样，但以更精确的方式，他首先定义（术语除外）属于由给定数量生成的域，伴随的概念以及给定的不可约多项式

\* 高斯已经在他的论文中指出了将他的方法推广到双纽线除法方程的可能性（[13]，第I，p. 413），并在最近几年出版的注中发展了除以5的特殊情况（[13]，第15卷⟦）。 X、p. 161-162 和 517）。正如高斯乐于在他的著作中散布的许多其他简短而神秘的指示一样，《论文研究集》的这句话生动地震撼了他同时代的人的头脑。我们知道，这对鼓励 Abel 和 Jacobi 在他们的研究中关于这个问题的贡献不小。

** 域的概念（更一般地说，集合）对于数学思想之前康托尔和戴德金来说实际上是陌生的。阿贝尔和伽罗瓦的《基域》中的定义元素可以理性地表达为已知量的函数，而无需考虑明确考虑由这些元素形成的集合。

域。 给定一个没有倍数根的方程 $F(x) = 0$，系数在给定的域 $K$ 中，他连续地证明了 « *总是有可能形式函数 V 的根，使得没有通过在这个函数中以所有可能的方式排列根等于另一个*而获得值，这个函数 « *享受性质，给定方程的所有根可以有理地表达为函数 V* » 并且，如果 $V, V', V'', ...$ 是由 $V$ 满足的不可约方程的根， « *如果 $a = f(V)$ 是所提出方程的根，则 $f(V')$* » ([15], p. 36-37);在现代项中，他因此证明了$V$，以及它的任何一个共轭超过$K$生成域$N$或根或$F$。 然后，将$F$的定义群$\Gamma$视为根$x_i$的置换集合，将$x_i$的有理式中的$V$代入为$V$中的函数，$V$中的共轭中的任意一个；并且他立即通过性质获得$K$的元素的基本刻画，在$\Gamma$的每个置换下保持不变（[15]，p. 38-39）。 然后他证明，如果另一个多项式的$N$包含根域$L$，则$N$的群超过$L$是$\Gamma$的正规子群（概念）他在这个场合介绍了这一点）（[15]，p. 41和25-26）。 由此，他最终通过推理推导出根式方程可溶性的标准，其基本运行如下：基域$K$假设为包含单位元的所有根，假设存在一个上升的序列 $K$和$N$之间的中间体域的$(K_i)_0, ...,$，其中$K_0 = K, K_m = N$、域$K_{i+1}$由二项式方程$x^{n_i} - a_i = 0$的所有根的伴随到$K_i$获得（其中$a_i \in K_i$）。 因此，在$\Gamma$中存在子群的下降序列$(\Gamma_i)$，使得$\Gamma_0 = \Gamma, \Gamma_m = \{ E \}$（中性元素），$\Gamma_{i-1}$在$\Gamma_i$和商群$\Gamma_i / \Gamma_{i+1}$中是正常的，是循环的（这种情况群 $\Gamma$ 据说是*可解*）。 相反，当这种情况发生时，使用拉格朗日求解表明，$K_{i+1}$是由二项式方程的所有根的$K_i$通过伴随获得的，因此方程$F(x) = 0$可被根式*解。 因此，次数$n > 4$的“一般”方程的根式解不可能是推论，因为该方程的群$\Gamma$同构于对称的群$\mathfrak{S}_n$（V， p. 59、例 5)，不可溶（I、p. 142、实施例 10 和p. 143、实施例 16）。

\* 如果 K 不包含单位元的所有根并且如果 E 是通过邻接 K 所有这些根获得的域，则 $E \cap N$ 是 K 的阿贝尔的扩张 ； 从而很容易推断出（使用有限阿贝尔的群的结构），要使 N 对 K 的群可溶，E(N) 对 E 的群成立是必要且充分的。 考虑到单位元的根可以通过“根式”表达，我们看到伽罗瓦准则独立于域 K 上的任何假设（并且对于特征 0 的任何域更普遍有效）。 In actual fact Galois makes no simplifying hypothesis about K and argues by induction on the order of the radicals successively adjoined to K ([15], p. 43).

正如我们已经说过的（第I章的cf.历史注），从19世纪中叶开始，代数学家大大扩展了他们的研究领域，直到那时几乎完全局限于方程的研究。根据伽罗瓦的发现，人们认识到“根据根式”的问题或解只是无理数分类的一般问题的一个特殊的、有点人为的情况。后者在整个 19 世纪末受到来自各方的攻击，逐渐积累了无数不同的结果，为斯坦尼茨的综合奠定了基础。

首先，就代数无理数而言，伽罗瓦理论提供了基本的原理分类，将代数方程的研究简化为群。由于这个原因，它首先是置换群的理论，我们的任务不是在这里谈论它（cf.历史注至第I章），它在纯粹的代数中形成了那个时期研究的主要对象。代数域理论的其余进展归功于数理论和代数几何的同时发展。实际上这一进展主要涉及理论的阐述，主要归功于戴德金[18]，他引入了域和环*的概念，并且（结合他对超复数系统的研究）系统地发展了扩张理论的线性方面（[18]，第 3 卷，p. 33 等）。正是他将伽罗瓦群视为所考虑的扩张的自同构由……组成，而不仅仅是一个方程的根的置换群，并且他证明了（对于数域）他的基本原理定理关于自同构的线性独立性（[18]，第3卷，p. 29）以及伽罗瓦扩张的正常基的存在性（[18]，第2卷，p. 433）。最后，他解决了无限次数和注的代数扩张的问题，伽罗瓦理论不能可以按原样应用（伽罗瓦群的任意子群不必总是与扩张的群相同）一个子扩展），并且凭借大胆的直觉，他已经尝试将伽罗瓦群视为拓扑群**——这一想法只有在克鲁尔于1928年提出的无限次数的伽罗瓦扩张理论中才达到成熟[24]。

与概念平行于域的先验元素的演变变得精确。超越数的存在由Liouville于1844年基于丢番图近似理论，通过构造的显式过程首次证明[17]；康托在 1874 年给出了另一个“非建设性”证明，使用集合的幂的简单反射（cf.V，p. 147），例如。 3）；最终 Hermite 在 1873 年证明了 e 和 Lindemann 在 1882 年的超越性：

\* 字 « 域 » 来自戴德金本人； « 环 » 由希尔伯特引入（戴德金称为环 « 阶 »）。
** « ...所有这些置换形式的集合在某种意义上是一个连续的流形，这个问题我们在这里不再进一步讨论»（[18]，第2卷，p. 288）。

$\pi$乘方法类似于埃尔米特的，从而最终结束了对圆*的正交问题的讨论。

关于超越数在代数计算中的作用，克罗内克在1882年观察到，如果$x$超越域$K$，则域$K(x)$同构于域或有理分式 $K(X)$（[19]，a），p. 7）。他实际上将伴随的不定式到域作为他阐述代数理论数的基石（[19]，a））。另一方面，Dedekind 和 Weber 在同一年展示了算术方法如何用于集合代数曲线理论（[18]，第 I、p. 238）。算术和代数几何之间的类比对于一方和另一方来说都是非常富有成效的，因此可以从几个方向看到。

在所有这些研究域中，出现的研究域由经典数学意义上的“具体”元素组成——复数变量**的（复数）数或函数。但克罗内克在 1882 年就已经完全意识到这一事实（只有高斯和伽罗瓦隐晦地瞥见了），即“不定性”在他的理论中只扮演了代数的基元素的角色，而不是数学分析意义上的变量（[19]，a），p. 93-95）； 1887 年，他提出了这个想法，并结合了一个庞大的计划，该计划旨在通过拒绝所有将不能简化为整数上的代数运算（cf. 历史。注到书 I，第 1 章）的一切来重新奠定所有数学的基础。 IV）。正是在这个场合，克罗内克采用了柯西[16]的思想，柯西将复数的域$\mathbf{C}$定义为剩余类类域$\mathbf{R}[X]/(X^2 + 1)$，Kronecker展示了代数数的理论如何完全独立于“基本原理” 代数的定理 » 甚至实数的理论，因为每个代数数域 （有限次数）同构于剩余类类域 $\mathbf{Q}[X]/(f)$ （其中$f$ 是$\mathbf{Q}$ 上的不可约多项式) [19], b)。正如 H. Weber [20] 注几年后在发展域公理化理论的第一个草图时一样，克罗内克的方法实际上适用于任何基域$K$。韦伯特别指出，域$\mathbf{Z}/(p)$（$p$质数）可以被视为$K$，从而允许同余“模p”的演算包含在域的理论中；前者在 18 世纪下半叶由欧拉、拉格朗日、勒让德和高斯形成，它与以下理论的类比：

\* 这些定理中的简单证明可以在 D. Hilbecht, Gesammelte Abhandlungen 中找到例。卷。 I、p. 1，柏林（施普林格），1932 年。

** 与他们的前辈一样，克罗内克、戴德金德和韦伯实际上都不是一个或多个复杂变量的“代数函数”的定义概念。 In effect it is impossible to define correctly an « algebraic function » of a complex variable (in the sense of Analysis) until the corresponding Riemann surface has been defined, and it is precisely the definition of this Riemann surface (by purely algebraic means) that Dedekind and Weber are trying to achieve. 当《代数函数 a 的域被定义为域有理分式的抽象代数扩张时，这种明显的恶性循环当然就消失了：事实上，戴德金和韦伯使用的只是这个定义，这显然使他们的结果合法化。

代数方程很容易被观察到；在发展这个类比时，伽罗瓦（根据他在群理论中的研究）毫不犹豫地引入了不可约同余模$p^*$的“理想根”，并指出了它的主要性质（[15]，p. 15-23）**。当克罗内克的方法应用于$\mathbf{Z}/(p)$时，结果是（除了术语）Serret和Dedekind（[18]，卷I，p. 40）已经给出的这些“伽罗瓦想象”的表示。

在世纪之交，除了所有这些“抽象域”的例之外，还添加了Veronese [21]引入的形式幂级数的域，以及最重要的是Hensel [22]的p-adic域。正是后者的发现导致斯坦尼茨（正如他明确指出的那样）在一篇基础论文[23]中将抽象的概念公共的与所有这些理论分离，该论文可以被认为是产生了当前的代数概念。他系统地发展了交换域的公理的推论，从而引入了素数域的概念、可分（代数）元素、完美域的定义、次数的超越扩张，最后证明任意域存在代数闭扩张。

最近，斯坦尼茨的理论在几个重要方面得到了完善。一方面，Artin 的工作证明了伽罗瓦理论的线性特征标 [25]。另一方面，由 Dedekind（[18]，第 2 卷，p. 412）感知的推导的一般概念（以经典微分演算的形式属性为模型），由 Steinitz 在域的有理分式的特殊情况中引入（[23]， p. 209-212），已成功用于超越扩张的研究（现代代数几何的基本），特别是在推广或概念与后者的可分离性中[26]。

\* 在一份可能可追溯至 1799 年但仅在他去世后之后发表的手稿中，高斯已经有了引入此类“想象”的想法，并且他获得了伽罗瓦结果的大量部分（[13]，卷II，p. 212-240，特别是p. 217）。

** 伽罗瓦完全了解这些代数计算的形式特征标，并且对于例，毫不犹豫地取同余左侧的导数，以表明后者没有倍数 «虚数 » 根 ([IS], p. 18)。他特别强调，原语元素的定理对于有限域和数域（[15]，p. 17，注²）同样有效，但没有给出证明。

参考书目

1. O. Neugebauer, Vorlesungen uber Geschichte der antiken Mathematik, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
2. Euclidis Elementa, 5 vol., ed. J. L. Heiberg, Lipsiae (Teubner), 1883-88.
2 bis. T. L. Heath, The thirteen books of Euclid's Elements..., 3 vol., Cambridge, 1908.
3. H. Cardano, Opera, Lyon, 1663.
4. R. Bombelli, L'Algebra, Bologne (G. Rossi), 1572.
5. Francisci Vietae, Opera mathematica..., Lugduni Batavorum (Elzevir), 1646.
6. A. Girard, Invention nouvelle en Algèbre, Amsterdam, 1629.
7. R. Descartes, Geometria, Latin transl. by Fr. van Schooten, 2 ed., 2 vol., Amsterdam (Elzevir), 1659-61.
8. G. W. Leibniz, Mathematische Schriften, ed. C. I. Gerhardt, 7 vol., Berlin-Halle (Ascher-Schmidt), 1849-63.
9. Der Briefwechsel von Gottfried Wilhelm Leibniz mit Mathematikern, herausg. von C. I. Gerhardt, vol. I, Berlin (Mayer und Müller), 1899.
10. L. Euler, Opera Omnia (1), vol. VI, Berlin-Leipzig (Teubner), 1921 : a) De Formis Radicum Aequationum..., p. 1-19 ; b) De Resolutione Aequationum cujusvis gradus, p. 170-196.
11. J.-L. Lagrange, Œuvres, t. III, Paris (Gauthier-Villars), 1869 : a) Reflexions sur la resolution algébrique des equations, p. 205-421 ; b) Sur la forme des racines imaginaires des équations, p. 479.
12. A. Vandermonde, Mémoire sur la résolution des equations, Hist. de l'Acad. royale des sciences, année 1771, Paris (1774), p. 365-416.
13. C. F. Gauss, Werke, vol. I-X, Gottingen, 1863-1923.
14. N. H. Abel, Œuvres, 2 vol., ed. Sylow et Lie, Christiania, 1881.
15. E. Galois, Œuvres mathématiques, Paris (Gauthier-Villars), 1897.
16. A.-L. Cauchy, Œuvres complètes (1), t. X, Paris (Gauthier-Villars), 1897, p. 312 et 351.
17. J. Liouville, Sur des classes très étendues de quantites dont la valeur n'est ni algébrique, ni même réductible à des irrationnelles algébriques, Journ. de Math. (1), t. XVI (1851), p. 133.
18. R. Dedekind, Gesammelte mathematische Werke, 3 vol., Braunschweig (Vieweg), 1932.
19. L. Kkonecker : a) Grundziige einer arithmetischen Theorie der algebraischen Grössen, Crelle's J., XCII (1882), p. 1-122 (= Werke, vol. II, Leipzig (Teubner), 1897, p. 245-387) ; b) Ein Fundamentalsatz der allgemeinen Arithmetik, Crelle's J., C (1887), p. 490-510 (= Werke, vol. III₁, Leipzig (Teubner), 1899, p. 211-240).
20. H. Weber, Untersuchungen über die allgemeinen Grundlagen der Galoisschen Gleichungstheorie, Math. Ann., vol. XLIII (1893), p. 521-544.
21. G. Veronese, Fondamenti di geometria, Padova. 1891.
22. K. Hensel, Theorie der algebraischen Zahlen, Leipzig-Berlin (Teubner), 1908.
23. E.-Steinitz, Algebraische Theorie der Korper, Crelle's J., vol. CXXXVII (1910), p. 167-309.
24. W. Krull, Galoissche Theorie der unendlichen algebraischen Erweiterungen, Math. Ann., vol. C (1928), p. 687.
25. E. Artin, Galois Theory..., Ann Arbor, 1946.
26. A. Weil, Foundations of algebraic geometry, Amer. Math. Soc. Coll. Public., vol. XXIX, New York, 1946.
