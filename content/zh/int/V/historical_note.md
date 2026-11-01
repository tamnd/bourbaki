---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: int-i-vi
pdf_pages: 0378-0391
extraction: ocr
statements: 0
exercises: 0
content_sha256: 5477eb7da48ac89d42a1dc1ba454d97059ee868b78ded7f123a0fa834b01cf90
translated_from: content/en/int/V/historical_note.md
translation_method: google
source_content_sha256: 3d00fa85741617d26ce8593d9add45983d1d1f40fc67094a9040d7407e36d0dc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: b7bd56597c81b41484242125497fbe5b714b023fd7c24f46c41d0e286e6a6923
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

# 历史注记

（章II至V）

（注：罗马数字指的是注末尾的参考书目。）

现代积分概念的发展与函数概念的演变以及自 19 世纪初以来对实变量数值函数的深入研究密切相关。 众所周知，欧拉已经以相当普遍的方式构想了概念或函数，因为对他来说，给出了一条“任意”曲线，该曲线与平行于Oy轴定义函数$y = f(x)$的每条线相交于单个点（cf.FRV，Hist. 注对应章节。 I–III);然而，像他的大多数同时代人一样，他拒绝承认这样的函数可以“分析地”表达。 直到傅里叶的工作之前，这种点的观点才到了变换；但后者发现可以将不连续的函数表示为三角函数级数*的和，对习题对后世产生了决定性的影响。 说实话，傅里叶的证明完全缺乏严谨性，其有效范围也并不明显；然而，积分公式

$$
a_n = \frac{1}{\pi} \int_{-\pi}^{+\pi} \varphi(x) \cos nx \, dx , \quad b_n = \frac{1}{\pi} \int_{-\pi}^{+\pi} \varphi(x) \sin nx \, dx \quad (n \geqslant 1),
$$

给出$\varphi$的傅里叶级数展开的系数，当假设$\varphi$分段连续时，具有明显的直观意义，并且

\* 仅在相对意义上的“发现”：欧拉已经通过非周期函数的三角函数级数（例如$x$ 和 $x^2$）熟悉表示，并且公式 (1) 早在 1754 年的 Clairaut 的著作中就可以找到，在 1777 年的著作中也可以找到公式 (1)。欧拉的回忆录。但 18 世纪由于对级数中展开的含义缺乏清晰的概念，忽视了这样的结果，并保持了对于“不连续”函数不可能获得这样的展开的信念，相反，傅立叶宣称他的展开是收敛的“无论曲线如何” 相应的到 $\varphi(x)$，是否可以为其分配一个解析方程，是否依赖于任何正则律 ”（Œuvres，v. I，巴黎（Gauthier–Villars），1888，p. 210）。

* 而且，正是这些函数是狄利克雷限制本人一开始的，在著名的回忆录 (II) 中，他建立了傅里叶级数的收敛性；但在工作结束时，他已经全神贯注于他的成果中的扩张到更广泛的类至函数。 人们知道，正是在这个场合，狄利克雷精确地阐述了傅里叶的思想，定义了我们今天所理解的函数的一般概念；自然地，第一个要澄清的点是知道在哪些情况下可以再次为公式赋予含义（1）。 “当[$\varphi$]的连续性解在数中无限时……”狄利克雷（（II），p. 169）说道，“那么函数$\varphi(x)$必须是这样的，如果$a$和$b$表示之间的任何两个量$-\pi$和$+\pi$，我们总是可以在$a$和$b$之间放置其他数量$r$和$s$足够接近，使得函数在$r$到$s$的区间内保持连续。 考虑到[傅里叶]级数的各个项是定积分并回到积分的基本概念，人们很容易感觉到对这个限制的需要。 由此可见，函数的积分只有在函数满足刚才所说的条件时才有意义。”

在现代项中，狄利克雷似乎认为可积性相当于不连续性的点形式无处稠密集合；此外，几行之后，他注著名的函数的例等于 $x$ 有理数的 $c$，并且对于 $x$ 无理数等于不同的值 $d$，他断言这个函数 “不能代入积分中。 他还宣布了关于这个主题的未来作品，但这些作品从未出版，**并且25年来似乎没有人试图朝这个方向前进，也许是因为当时对函数如此“病态”的考虑似乎完全没有兴趣；无论如何，当黎曼在 1854 年（(III)，第 227-264 页）再次提出这个问题时（仍然与三角学级数***有关），他觉得有必要证明他的工作的合理性：“无论我们对无限小范围内力和物质状态随时间和地点变化的方式的无知，我们仍然可以肯定的是，狄利克雷研究不适用的函数不会出现在自然现象中。 然而，”他继续说道，“似乎狄利克雷未处理过的这些案例值得关注——

\* 对于傅里叶来说，积分仍然是借助面积的概念来定义的；我们记得积分的解析定义仅出现在柯西（cf.FRV，Hist.注对于Chs.I-III）。

** According to certain (rather obscure) indications of Lipschitz (J. de Crelle, 63 (1864), p. 296; translated into the French by P. Montel in Acta. Math., 36 (1912), pp. 261–295), Dirichlet perhaps believed that if the set of points of discontinuity is nowhere dense, its 'derived set' is finite, and would in any case have limited his investigations to the case that this is so.

*** 从狄利克雷和黎曼时代到现在，我们将看到积分与现在所谓的“调和数学分析”之间的紧密联系，这在某种意义上构成了积分的试金石。

化有两个原因。 First, as Dirichlet himself 注 at the end of his work, this subject is very closely related to 原理 of the infinitesimal 演算, and may serve to bring greater clarity and certainty to these 原理.由此点来看，其研究有直接的的趣味性。其次，傅里叶级数在物理学中的应用并不局限于研究； they are at present also applied with success in a domain of pure mathematics, the theory of 数, and it appears that it is precisely 函数 whose 展开 in trigonometric 级数 was not studied by Dirichlet, that show some importance there ((III), pp. 237–238).

黎曼的想法是从积分的近似过程开始，由柯西恢复到荣誉地位，当函数$f$的“黎曼和”在有界区间$[a, b]$内趋于极限（作为区间的最大值长度）时，到确定。细分趋向于 0)，问题毫无困难地获得了解，在下面的形式中：对于每个$\alpha > 0$，存在将$[a, b]$细分为最大长度的子区间，该子区间足够小，使得该区间的长度的和足够小$f$ 的振荡为 $> \alpha$ 的细分是任意小的。此外，他还表明，这个条件不仅对于函数分段连续且单调，而且对于某些可能具有密集集合或点不连续性的函数都是经过验证的。*

黎曼的回忆录直到1867年之后去世才发表。然而，这一次，时代对研究的型更加有利，“黎曼积分”自然地在思想潮流中占据了一席之地，然后导致了对实变量“连续统”和函数的深入研究（Weierstrass，Du） Bois-Reymond、Hankel、Dini），与 Cantor 一起出生到结论，并出生集合论。黎曼给条件的可积性给出的形式提出了在区间中函数的不连续性对集合的点的“度量”的想法；但近 30 年过去了之前，人们成功地为这一概念提供了富有成果且方便的定义。

Stolz、Harnack 和 Cantor (1884-85) 是这方面的首次尝试。到定义 $\mathbf{R}$ 有界子集 E 的“测量”，前两个考虑集合 $F \supset E$，它们是有限的并间隔，对相应的间隔的长度的每个 F 和进行取值，并将 E 的“测量”称为这些数的下确界；而康托尔将自己置于空间$\mathbf{R}^n$，考虑有界集合E和$\rho > 0$由点形成的E的邻域$V(\rho)$，其到E的距离为$\leq \rho$，并取$V(\rho)$“体积”的下确界。**这个定义，

\* 然而，H. J. Smith 早在 1875 年就给出了函数的第一个例在黎曼意义上不可积，其不连续性的集合和点并不稠密（Proc. London Math. Soc., (1), v. VI (1875), pp. 140–153）。
**康托没有给出这个“体积”的精确定义，而极限自己对集合的“测量”等于其闭包的测量，由此特别得出两个不相交的集合的并的“测量”可能小于这些“测量”的和两个集合。毫无疑问，为了缓解这最后一个困难，几年后，皮亚诺（V）和乔丹（VI）在康托尔的集合$A$的“度量”$\mu(A)$包含在盒子$I$中的同时，引入了它的“内部度量”$\mu(I) - \mu(I - A)$，并称为“可测量” 集合$A$（现在说是“可争论的”），这两个数重合。两个不相交的可争论集合 $A, B$ 中的并是可争论的，并且具有 $A$ 和 $B$ 的“度量”的“度量”和；然而，有界开集合不一定是可争论的，有理数的集合也不包含在有界区间中，这使得皮亚诺-乔丹概念失去了很多兴趣。

E. Borel (IX) 的功绩在于发现了之前定义的缺陷并研究了如何弥补它们。自康托以来，人们就知道$\mathbf{R}$中的每个开集合$U$都是其“分量”可数族的并，这些“分量”是成对的不相交的开区间； Borel 根据之前的结果，建议将 $U$（当 $U$ 有界时）和的量度作为其分量的长度的量度，而不是试图通过将有限序列的区间包围来“从外部”接近 $U$。然后，他非常概括地描述了集合（随后称为“Borel 集合”）的类，从开放集合开始，通过无限迭代可数并的运算和“差”$A - B$，他指出对于这些集合，人们可以定义拥有*完全可加性*的基本性质的测度：如果序列 $(A_n)$ 由成对的不相交的 Borel 集合组成，那么它们的并的测度（假设有界）等于和他们的措施。

这个定义开启了数学分析的新纪元：一方面，与贝尔同时代的工作相结合，形成了点对集合、点的分类的整个拓扑性质研究的级数的出发点；最重要的是，它是勒贝格在 20 世纪初期进行的积分中的基与扩张或概念的积分。

在他的论文 (X a)) 中，勒贝格首先精确并发展了 E. Borel 的简洁指示；模仿 Peano–Jordan 方法，有界集合 $A \subset \mathbf{R}$ 的“外部测度”被定义为开集合包含 $A$ 测度的下确界；那么，如果 $I$ 是一个区间包含-

说可以通过倍数积分计算（（IV），第229-236页和257-258页）。很容易看出，他的定义相当于Stolz-Harnack的应用和Borel-Lebesgue定理。

\* 对于 Borel 来说，测度还只是研究有理函数的某些级数的技术手段，而他本人则强调，对于他自己集合的目标，测度的用处主要在于非零的测度的集合不可数((IX)，p. 48)。

计算$A$，$A$的“内部测度”是$I$和$I - A$的外部测度之差；因此，我们得到了“可测量的集合”的概念，它与Borel最初的“构造性”定义的区别仅在于Borel意义上的测量零的集合的伴随或子集。 This definition extended at once to the spaces $\mathbf{R}^n$; the old conception of the definite integral $\int_a^b f(t)\,dt$ of a bounded function $\geqslant 0$ as the 'area' bounded by the curve $y = f(x)$ and the lines $x = a$, $x = b$ and $y = 0$, thus provided an immediate extension of the Riemann integral to all of the functions $f$ for which the measure of the preceding set happens to be defined. 但勒贝格的独创性并不在于这个扩张*的想法，而在于他发现了在如此构想的积分中通向极限的基本定理，定理在他的著作中出现为测度的完全可加性的推论；**他立刻意识到了它的全部重要性，并使其成为说教的基石早在 1904 年，他就在其著名的“Leçons sur l'intégration et la recherche des fonctions Primus”(X b)) 中阐述了他的理论。***

我们在这里不能详细描述了勒贝格的结果在无穷小演算的经典问题研究中所带来的无数进步；我们将有机会在以后的书中强调其中的一些内容。勒贝格本人已经在他的论文中应用了他的理论，将经典的概念的长度和面积扩展到集合，比通常的曲线和曲面更普遍；对于这一理论在过去半个世纪中的长足发展，我们建议读者参考L最近的阐述。切萨里（XXVI）。我们还提到了三角函数级数的应用，勒贝格几乎立即在之后他的论文（Xc））中开发了三角函数级数，这些应用为这一理论打开了新的视野，其探索至今还远未完成（参见（XXV））。最后，最重要的是，$L^p$ 空间和 Riesz–Fischer 定理 ((XIII)、(XV a)) 和 (XV b)) 的定义； cf.历史注记（第V书）揭示了积分的新概念在泛函数学分析中可以发挥的作用；一个只会增加的角色

\* 独立于 Lebesgue，W. H. Young 对于半连续函数 (XI a)) 也有同样的想法。
** 这个定理的特殊情况，对于函数的序列在一致有界的紧致区间上可积，并且其极限在黎曼意义上可积，已由Arzelà（VII）证明。
***在积分一般理论中最重要的定理中的推论中，特别值得一提的是叶戈洛夫关于可测量函数（XVI）的序列收敛性的定理，它使Borel和Lebesgue的一些早期注变得精确。另一方面，可测（数值）函数最初由勒贝格定义为性质，对于这样的函数$f$，$\mathbf{R}$的每个区间的$f$下的逆像是可测的集合。然而，从 1903 年起，Borel 和 Lebesgue 开始关注这些函数的拓扑性质；它们被维塔利（Vitali）确定为形式，维塔利在1905年（XIIa））首先制定了可测量的函数的性质，我们在第1章中将其视为定义。 IV, §5（定理于 1912 年由 N. Lusin 重新发现，通常以他的名字命名）。

以及这个概念的后续推广，我们稍后会谈到。

但首先，让我们再详细讨论一下勒贝格投入最多精力的问题之一，即积分概念和本原概念之间的联系。 随着黎曼引入积分的推广，自然产生了这样的问题：积分和本原之间的经典对应对于连续函数是否有效，是否再次在更一般的情况下存在。 现在，很容易给出函数$f$的例，在黎曼意义上可积，使得$\int_a^x f(t) \, dt$在某些点（cf.FRV，II, §2，Exer.1）处没有导数（甚至不是右导数或左导数）；相反，Volterra 在 1881 年证明，函数 $F(x)$ 可以有一个导数，该导数在区间 I 内有界，但在 I 中不可积（在黎曼意义上）。 通过非常微妙的数学分析（其中在积分中定理到极限是远远不够的），勒贝格成功地证明了如果$f$在$[a, b]$上可积（在他的意义上），那么$F(x) = \int_a^x f(t) \, dt$几乎处处都有等于$f(x)$（X b））的导数。 相反，如果函数 $g$ 在 $[a, b]$ 上可微且其导数 $g' = f$ 是*有界*，则 $f$ 可积且公式 $g(x) - g(a) = \int_a^x f(t) \, dt$ 成立。 然而，Lebesgue 确定当 $g'$ 无界时，问题要复杂得多；在这种情况下，$g'$不一定是可积的，因此第一个问题是表征连续的函数$g$，其中$g'$几乎无处不在并且可积。 将自己限制在$g$的导数*之一处处*有限*的情况，勒贝格表明$g$必然是函数*有界变分*。最后，他建立了最后结果的逆命题：有界变分的函数$g$几乎处处都允许导数，而$g'$是可积；然而，情况不再一定是这样的

$$
g(x) - g(a) = \int_a^x g'(t) \, dt;
$$

\* $g$ 在点 $x$ 的右导数是两个极限

$$
\limsup_{h \to 0, h > 0} (g(x + h) - g(x))/h, \quad \liminf_{h \to 0, h > 0} (g(x + h) - g(x))/h.
$$

左导数的定义类似。

** 这些函数是Jordan在修正曲线时引入的（VI）；他证明可以给出以下等价的定义： a) $f$ 是两个递增函数之差； b) 对于$[a, b]$间隔递增有限序列的点$(x_i)_{0 \leq i \leq n}$的每个细分，其中$a = x_0$，$b = x_n$，和$\sum_{i=1}^n |f(x_i) - f(x_{i-1})|$以数为界，与所考虑的细分无关。这些和的上界是$f$在$[a, b]$上的*总变分*。

这个关系的两个成员之间的差异是有界变化的函数，它是非常数的并且几乎到处都有导数零（“单数”函数）。仍然需要描述有界变化的函数 $g$ 使得关系 (2) 成立。勒贝格确定，这些函数（维塔利对它们进行了详细研究，称之为“绝对连续”）是具有以下性质的那些：$g$在开集合U上的总变化（和在U的每个连通分量上的$g$总变化）趋于0，测量为U。

我们将在下面看到这些结果在减弱的形式之后如何获得更普遍的意义。在他们最初的形式中，他们的域的应用仍然相当有限，没有超出实变量函数的“精细”理论框架；它们也超出了本论文的范围。*更重要的是，原语理论的后来发展也是如此。我们将满足于在这里提到丹乔伊及其模仿者和继承者（佩隆、德拉瓦莱-普桑、辛钦、卢辛、巴纳赫等）的深刻著作；读者可以在 S. Saks (XXIV) 的书中找到对这些问题的详细阐述。

勒贝格理论带来的重要进展之一涉及倍数积分。这个概念是在18世纪中叶引入的，最初是在“不定积分”形式中（类比单变量函数的积分理论，$\iint f(x, y)\, dx\, dy$表示方程$\frac{\partial^2 z}{\partial x \partial y} = f(x, y)$的解）；但欧拉早在 1770 年就对双积分扩展到有界域（受解析曲线的限制）有一个非常清晰的概念，并且他正确地写出了公式通过两个连续的单积分（I）来评估这样的积分。只要被积分的函数是连续的，并且积分的域不太复杂，证明“黎曼和”的项中的公式是不难的；但一旦想要处理更一般的情况，黎曼过程就遇到了严重的困难（$f(x, y)$可以在黎曼意义上可积，而当在黎曼意义上进行单积分时$\int dx \int f(x, y)\, dy$没有意义）。当传到勒贝格的定义时，这些困难就消失了；后者已经在他的论文中表明，当$f(x, y)$是有界“Baire 函数”时，函数$y \mapsto f(x, y)$（对于每个$x$）和$x \mapsto \int f(x, y)\, dy$也是有界的，并且有公式

$$
\iint f(x, y)\, dx\, dy = \int dx \int f(x, y)\, dy
$$

\* 然而，我们提到，概率演算中的现代“鞅”理论不断使用与微分研究中使用的论证具有很强的类比性的论证。

（在矩形上进行积分）。稍后，Fubini（XIV）通过证明对此结果进行了重要补充，即如果仅假设$f$可积，则$x$的集合使得$y \mapsto f(x, y)$不可积，其度量为零，这允许立即将公式（3）扩展到这种情况。

最后，在 1910 年 (X d))，勒贝格对其单积分导数的结果进行了扩张到倍数积分。因此，他联想到函数$f$，可积在$\mathbf{R}^n$的每个紧致子集上，集合函数$F(E) = \int_E f(\mathbf{x})\, d\mathbf{x}$，为$\mathbf{R}^n$的每个可积子集E定义，这概括了“不定”的概念积分'；他在这个场合观察到这个函数具有以下两个性质： 1° 它是完全相加的； 2° 它是“绝对连续”，因为 $F(E)$ 在 E 的测量下趋于 0。勒贝格的回忆录的本质部分存在于这个命题的证明逆命题。* 但他并没有停留在那里，并且在同一方向上，提请注意泛化的可能性有界变化的函数的概念，通过考虑可测量的集合的函数$F(E)$，完全相加，并且使得$\sum_n |F(E_n)|$对于E的每个可数划分保持有界到可测量的集合$E_n$。而且，如果他实际上限制自己只在$\mathbf{R}^n$盒中的集合上考虑这样的函数，那么很明显，只需要再迈出一步即可达到J. Radon在1913年达到定义的一般测度概念，将勒贝格积分和勒贝格积分包含在一次综合中Stieltjes 整的，我们现在必须谈论它。

1894 年，T. Stieltjes 发表了题为“Recherches sur les 分数 continues”（VIII）的高度原创性的回忆录，其中从一个看似相当特殊的问题出发，在实变量的解析函数和函数理论中提出了完全新颖的问题，并提出了问题。 **在阶表示解析函数的某个序列的极限时，斯蒂尔耶斯除其他外，引入了直线上正“质量分布”的概念，这是一个在物理科学中长期熟悉的概念，但迄今为止仅在数学中在限制性假设下被考虑（一般来说，存在每点出现一个“密度”，以连续方式变化）；他观察到，给出这样的分布相当于递增函数 $\varphi(x)$ 的分布，它给出了 $x > 0$ 的端点为 0 和 $x$ 的区间中包含的总质量，并且该质量的符号更改为 $x < 0$，$\varphi$ 相应的的不连续性群众“集中”

\* 在这个证明中，主要工具是维塔利（XII b））早些时候证明的覆盖定理，并且它在这个型问题中仍然是基础。
** 正是在那里，著名的“时刻问题”被表述和解决（cf.书V的历史。注）。

在点'。* Stieltjes 那么形式，对于区间 $[a, b]$ 内的这种质量分布，“黎曼和”$\sum_i f(\xi_i)(\varphi(x_{i+1}) - \varphi(x_i))$ 并表明，当 $f$ 在 $[a, b]$ 上连续时，这些和趋向于他表示的极限 $\int_a^b f(x)\, d\varphi(x)$。 由于除了连续（甚至可微）之外不需要对函数进行积分，Stieltjes 没有进一步推动这个积分**的研究**，十年来这个概念似乎没有引起任何关注。*** 然而，在 1909 年，F. Riesz (XV c))，解决了几年前由 Hadamard (cf. the Hist.) 提出的问题。 书V的注），证明了Stieltjes积分$f \mapsto \int_a^b f\, d\varphi$是$I = [a, b]$上连续实值函数空间$\mathscr{C}(I)$上最一般的连续线性泛函（$\mathscr{C}(I)$配备一致收敛的拓扑）；****以及这个结果几乎立刻就产生了各种推广。 最幸运的是J. Radon，1913 年 (XVII)：结合了 F. Riesz 和 Lebesgue，他展示了如何通过 Lebesgue 程序从任意“完全加法集合函数”（在 Lebesgue 测度的可测量集合上定义）开始而不是从 Lebesgue 测度开始，来计算定义积分。 在这样定义的$\mathbf{R}^n$上的“氡气测量”概念中，人们发现吸收了函数“有界变化”的概念：作为两个递增函数之差的函数的分解是作为两个正测量之差的测量分解的特殊情况；类似地，将“绝对连续”函数的“基$\mu$”对应到概念和分解的任意度量转换为基$\mu$的度量和与$\mu$不同的度量，有界变分的函数的勒贝格分解作为绝对连续函数的和和“奇异”函数。 此外，Radon 通过使用 F 的早期思想表明，当 $\mu$ 是勒贝格测度为基的测度时，具有基 $\mu$ 的测度相对于 $\mu$ 的“密度”再次存在。 Riesz（后来又被 J. von Neumann 等人再次采用并推广），它包含

\* Stieltjes 尚未区分具有相同端点 $a, b$ 的区间的各个型，这使他设想在 $\varphi$ 不连续性的点 $c$ 处，质量的一个部分集中在具有左端点的区间的 $c$ 属于 $c$，另一个部分到右端点$c$的区间，取决于$\varphi(c)$的值。

** 然而，人们应该注首次出现在Stieltjes的作品中，序列度量的“收敛”思想（（VIII），p. 95；事实上，它是强极限）。

*** 然而，随着 1906 年希尔伯特和他的学校算子谱理论的发展，它变得越来越重要。正是在这个场合，海灵格在 1907 年左右定义了积分，例如他表示为 $\int \frac{(dg)^2}{df}$ 的积分，乍一看似乎比 Stieltjes 的积分更普遍，但事实上 Hahn 早在 1912 年就表明它们可以简化为后者（这些是“测度的函数”概念的特例；cf. Ch. 1）。 V, §5, No. 9）。

**** 也正是在这部作品中，出现了措施序列的模糊极限的概念（（XVc）），p. 49）。

坚持将$\mathbf{R}^n$的映射$\theta$下的$\mu$测度的像构造成$\mathbf{R}$，选择使得$\theta(\mu)$是$\mathbf{R}$上的勒贝格测度（cf.Ch.V, §6，Exer.8c））。

几乎在之后Radon的回忆录出现后，Fréchet观察到该工作中的几乎所有结果都可以扩展到“完全加法集合函数”的情况，而不是为$\mathbf{R}^n$的可测量子集定义，而是为任意任意的子集定义集合 $E$（这些子集使得可数并和“差”的运算产生集合，函数再次被定义）。然而，在形式 $g \cdot \mu$ 中基 $\mu$ 的测度表达式，与 Lebesgue 和 Radon 一起，以一种本质方式基于涉及 $\mathbf{R}^n$ 的拓扑的论证（并且我们已经看到，Radon 的证明仅适用于 $\mu$ 是具有以下性质的测度）勒贝格测度为基)；直到 1930 年，O. Nikodym (XX) 通过直接论证，在其一般形式中获得了定理（几年后，由于使用了 $L^2$ 空间的性质，J. von Neumann 进行了显着简化（(XXII)，第 127-130 页））。

With Radon’s memoir, the general theory of integration may be considered as completed in its broad outlines; as later substantial acquisitions, one can only scarcely mention the definition of an infinite product of measures, due to Daniell (XIX b)), and that of the integral of a function with values in a Banach space, given by Bochner in 1933 (XXI), which paved the way for the study of the ‘weak integral’ which we shall treat in Chapter VI. 但它仍然是为了普及新理论，并使其成为日常使用的数学工具，而在 1910 年左右，大多数数学家仍然将“勒贝格积分”视为一种非常精确、易于操作的工具，注定只能用于极端微妙和极端抽象的研究。 这就是卡拉西奥多里 (Carathéodory) 的著作，该书长期以来一直是经典 (XVIII)，而且通过大量原创观察丰富了氡气理论。

但也正是在这本书中，积分概念首次让位给了测度概念，该概念曾是勒贝格最关注的领域（他的论文标题（X a））和他在这些问题上的主要工作（X b）））首次让位于测量概念，测量概念一直是勒贝格的辅助技术（就像乔丹之前他一样）。对于卡拉西奥多里来说，点中的变换无疑是由于他似乎过于重视“$p$维度度量”。*从那时起，

\* 这是‘平面曲线的长度’概念中的推广到正在研究的底层空间的任意值$n$和维数的$p$和空间的维数；当然，人们假设$0 \leq p \leq n$，但并不总是假设$p$是整数。自明可夫斯基、卡拉西奥多里和豪斯多夫以来，这个问题一直是众多作者著作的主题。勒贝格本人在他的论文中讨论了一些特殊情况，除了对他刚刚打造的工具进行测试幂的机会之外，似乎没有看到任何其他东西。

讨论整合问题的作者们在这两种点观点之间存在分歧，并非没有陷入争论，这些争论即使没有流血，也已经引起了很多墨水的流淌。在他们越来越抽象和越来越公理化的阐述中，度量及其所带来的所有技术改进不仅发挥着主导作用，而且往往与拓扑结构失去联系，事实上它在它出现的问题的大部分中都与拓扑结构联系在一起。其他论述，例如本论文，或多或少地遵循 W. H. Young 于 1911 年在回忆录中指出的方法，不幸的是很少有人注意到（XI b）），并随后由 Daniell 发展。前者处理勒贝格积分，从具有紧支撑的连续函数的“柯西积分”开始，假设已知，在阶到定义相继（正如我们在第IV, §1中所做的那样）下半连续函数的上积分，然后是任意数值函数的上积分， 可积函数的从而定义，以纯粹“功能”的方式模仿勒贝格的之后集合。 Daniell 在 1918 年 ((XIX a))、cf. (XXVII)) 将此阐述扩展为在任意集合上定义的函数；并有几个变体；他的主要优点是在抽象理论中认识到条件$\lim_{n \to \infty} \int f_n d\mu = 0$对于每个递减序列$(f_n)$逐点趋向0的作用​​（这在氡气测量理论中不会那么清楚地出现，其中条件通过迪尼的定理自动满足）。在相同的阶思想中（以及在 Gelfand 之前的谱理论中使用的严格的关系到方法），我们还必须提请注意 F. Riesz (XV d) 的回忆录），它将有序空间理论的几个结果放入简洁而优雅的形式中，这些结果发挥了在整合理论中的作用；我们非常密切地关注了他在第 1 章中的阐述。 II。

与读起来或多或少令人愉快但其基本内容不再有太大变化的说明性著作不同，人们必须在应用方面寻找自 1920 年以来积分理论所实现的进步：概率论（以前是谜题和悖论的借口，自柯尔莫戈洛夫（XXIII）公理化以来已成为积分理论的一个分支，尽管它是一个独立的分支，有自己的方法和问题）；遍历理论；自从哈尔发现了以他的名字命名的测度，以及这一发现引发的思想运动以来，谱理论和调和数学分析已经成为群理论中最重要的工具之一。带着这些问题，我们离开了现在注的框架；其中一些将在以后的章或书籍中进行处理。

\* Cf. the reviews by P. Halmos of the first volume of this Book (Bull. Amer. Math. Soc., 59 (1953), p. 249) and by J. Dieudonné of the book of Mayrhofer (ibid., 59 (1953), p. 479).

(I)L。欧拉，《Opera Omnia：Deformulisintegralibusduplicatis》(1)，v.XVII，莱比锡-柏林 (Teubner)，1915 年，第 289-315 页。

(II) G. Lejeune–Dirichlet, Sur la convergence des séries trigonométriques qui servent à représenter une fonction arbitraire entre des limites données, J. de Crelle, 4 (1829), pp. 157–169 (= Werke, v. I, pp. 118–132, Berlin (G. Reimer), 1889).

(III) B. Riemann，Gesammelte Mathematische Werke，第二。编辑，莱比锡（Teubner），1892 年。

(IV) G. Cantor，Gesammelte Abhandlungen，柏林（施普林格），1932 年。

(V) G. Peano，《无穷小几何几何应用》，都灵，1887 年。

(VI)C。乔丹，Cours d’Analyse，v. I，第二名。编辑，巴黎（Gauthier-Villars），1893 年。

(VII) C. Arzelà: a) Sulla integrabilità di una serie di funzioni, Rendic. Acc. dei Lincei, (4), 1 (1885), pp. 321–326; b) Sulla integrazione per serie, ibid., pp. 532–537 and 566–569.

(VIII) T. Stieltjes，《关于分数的研究》继续，Ann。事实。科学。图卢兹，8 (1894)，J. 1 至 J. 122。

(IX) E. Borel，Leçons sur la théorie des fonctions，巴黎（Gauthier-Villars），1898 年。

(X) H. Lebesgue: a) Intégrale, longueur, aire, Annali di Mat., (3), 7 (1902), pp. 231–359; b) Leçons sur l’Intégration et la recherche des fonctions primitives, Paris (Gauthiers–Villars), 1904; c) Sur les séries trigonométriques, Ann. Éc. Norm. Sup., (3), 20 (1903), pp. 453–485; d) Sur l’intégration des fonctions discontinues, Ann. Éc. Norm. Sup., (3), 27 (1910), pp. 361–450.

(XI) W. H. Young: a) On upper and lower integration, Proc. Lond. Math. Soc., (2), 2 (1905), pp. 52–66; b) A new method in the theory of integration, Proc. Lond. Math. Soc., (2), 9 (1911), pp. 15–50.

(XII) G. VITALI: a) Una proprieta delle funzioni misurabili, R. Ist. Lombardo, Rendiconti, (2), 38 (1905), pp. 599–603; b) Sui gruppi di punti e sulle funzioni di variabili reali, Rendic. Acc. Sci. di Torino, 43 (1908), pp. 229–236.

(XIII) E. FISCHER, Sur la convergence en moyenne, C. R. Acad. Sci., 144 (1907), pp. 1022–1024.

(XIV) G. FUBINI, Sugli integrali multipli, Rendic. Acc. dei Lincei, (5), 16 (1907), pp. 608–614.

(XV) F. RIESZ: a) Sur les systèmes orthogonaux de fonctions, C. R. Acad. Sci., 144 (1907), pp. 615–619; b) Untersuchungen über Systeme integrierbarer Funktionen, Math. Ann., 69 (1910), pp. 449–497; c) Sur certains systèmes singuliers d’équations intégrales, Ann. Éc. Norm. Sup., (3), 28 (1911), pp. 33–62; d) Sur quelques notions fondamentales dans la théorie générale des opérations linéaires, Ann. of Math., (2), 41 (1940), pp. 174–206.

(XVI) D. EGOROFF, Sur les suites de fonctions mesurables, C. R. Acad. Sci., 152 (1911), p. 244.

(XVII) J. RADON, Theorie und Anwendungen der absolut additiven Mengenfunktionen, Sitzungsber. der math. naturwiss. Klasse der Akad. der Wiss. (Wien), 122, Abt. IIa (1913), pp. 1295–1438.

(XVIII)C。 CARATHÉODORY，《Vorlesungen über reelle Funktionen》，莱比锡-柏林（Teubner），1918 年。

(XIX) P. J. DANIELL: a) A general form of integral, Ann. of Math., (2), 19 (1918), pp. 279–294; b) Integrals in an infinite number of dimensions, Ann. of Math., (2), 20 (1919), pp. 281–288.

(XX) O. NIKODYM, Sur une généralisation des intégrales de M. J. Radon, Fund. Math., 15 (1930), pp. 131–179.

(XXI) S. BOCHNER, Integration von Funktionen deren Werte die Elemente eines Vektorraumes sind, Fund. Math., 20 (1933), pp. 262–276.

(XXII) J. von NEUMANN, On rings of operators. III, Ann. of Math., (2), 41 (1940), pp. 94–161.

(XXIII) A. KOLMOGOROFF，Grundbegriffe der Wahrscheinlichkeitsrechnung，柏林（施普林格），1933 年。

(XXIV) S. SAKS，积分理论，第二。编辑，纽约（Stechert），1937 年。

(XXV) A. ZYGMUND，三角函数级数，华沙，1935 年（第二版，剑桥大学出版社，1959 年）。

(XXVI)L。 CESARI，表面积，普林斯顿，1954 年。

(XXVII)L。 H. LOOMIS，抽象谐波数学分析简介，伦敦-纽约-多伦多 (van Nostrand)，1953 年。
