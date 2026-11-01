---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: lie-i-iii
book_pages: 410-433
pdf_pages: 0428-0451
extraction: ocr
statements: 0
exercises: 0
content_sha256: 7e71f4648c3bb5e660f57189c1776dd2301746b23d6aca3c875dfeb361da1ca9
translated_from: content/en/lie/III/historical_note.md
translation_method: google
source_content_sha256: a68f0d57dc7836cb581ee65ebe1fb8698658067c5dabcb4f0a5454ae4c96c939
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 346026ec5158ae0a5cc85cea258d07a7888d25754f1051f2ff19d08d9ea50290
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

# 历史注记

（章I至III）

I。创世纪

这个理论被称为近一个世纪的“李群理论”，基本上是由一位数学家索菲斯·李提出的。

之前从历史开始，我们简单总结一下早期的各种研究，为我们铺平了道路。

(a) 转变群（克莱因-李，1869-1872）
大约 1860 年，有限集合的置换群理论正在发展并开始使用（Serret、Kronecker、Mathieu、Jordan）。 另一方面，盛行的不变量理论让数学家们熟悉了在合成下稳定的一些无限集合几何变换（特别是线性或射影变换）。 But before the work of Jordan [7] in 1868 on "groups of movements" (closed subgroups of the group of displacements of 3-dimensional Euclidean space), no conscious link seems to have been established between these two currents of ideas.

1869 年，普吕克的学生、年轻的费利克斯·克莱因 (Felix Klein，1849-1925) 在柏林与比他年长几岁的挪威人索菲斯·李 (Sophus Lie，1842-1899) 建立了友谊，因为他们对普吕克的“线几何”，特别是线复形理论有着公共的的兴趣，所以走到了一起。大约在这个时候，李萌生了他最原创的想法之一，将不变量的概念引入数学分析和微分几何；来源之一是他的观察，即微分方程“求积”的经典方法积分完全取决于方程在“连续”变换族下不变的事实。 1869 年是 Lie 使用这个想法的第一部作品（由 Klein 编辑）的日期；在那里，他研究了“Reye 复形”（集合，由四条线将四面体的面以给定交叉比切割为四个点）以及允许作为该复形的切线的曲线和曲面 [3 a]：他的方法取决于 Reye 复形在 3 参数交换律群（最大环面 of $\mathbf{PGL}(4, \mathbf{C})$），使得四面体的顶点保持不变。同样的想法主导了克莱因和赖伊 1870 年春天在巴黎时共同撰写的作品 [1, a]；在那里，他们基本上确定了平面$\mathbf{PGL}(3, \mathbf{C})$的射影群的交换连通子群，并研究了其轨道的几何性质（以曲线或曲面V的名义）；这通过统一的程序赋予了它们各种曲线的性质，无论是代数曲线还是超越曲线，例如 $y = cx^m$ 或对数螺线。这两部著作都强调了伽罗瓦和乔丹的理论给他们留下的深刻印象（乔丹对伽罗瓦的评论曾出现在1869年的《数学年鉴》上；而李早在1863年就听说过伽罗瓦理论）。 1871 年，克莱因对非欧几里得几何产生了兴趣，他在那里看到了他的研究对所有已知几何的分类原理的开始，这导致他在 1872 年提出了“埃尔兰根纲领”。对于他的部分，Lie 在 1873 年写给 A. Mayer 的一封信中（[3]，卷V，p. 584），注明了他在巴黎逗留期间关于转型群的想法，而在 1871 年的作品中（[3 b] p. 208），他已经在使用项 “变换群”并明确提出问题确定$\mathbf{GL}(n, \mathbf{C})$的所有子群（“连续或不连续”）。说实话，克莱因和赖伊在进入这个新的数学宇宙时都经历了一些困难，克莱因将乔丹新出现的《论文》称为“用七印封印的书”（[2]，p. 51）；他还就[1 a]和[1 b]写道：“对谎言属于来说，算子连续群的启发式思想的所有功劳，特别是有关微分方程和偏导数积分的一切。他后来在连续群理论中发展的所有概念都已经存在于胚胎中，但是却很少详细说明，以至于只有之后长时间的对话可以让他相信I许多细节，因为例从曲线V的存在开始”（[2]，p. 415）。

(b) 无穷小变换

“无穷小”变换的概念至少可以追溯到无穷小演算的开始；我们知道，笛卡尔发现了旋转的瞬时中心，他承认“在无限小”中，每个平面运动都可以比作旋转：18世纪分析力学的阐述完全基于类似的想法。 1851年，西尔维斯特寻求线性群$\mathbf{GL}(3, \mathbf{C})$及其一些子群的形式不变量，给出了矩阵“无限小”增量形式$\alpha_j dt$中出现的参数，并表达了函数的事实通过写出方程 $f((z_j + \alpha_j(dt))) = f((z_j))$，$f((z_j))$ 是不变的；这给了他 $f$ 的线性偏微分方程 $Xf = 0$，其中

$$
Xf = \sum_j \alpha_j \frac{\partial f}{\partial z_j},
$$

因此，其中 X 是一个 *微分算子*，“方向参数 $\alpha_j$ 方向上的导数”（[5]，第 3 卷，第 326 和 327 页）；西尔维斯特似乎认为这是一个相当重要的一般原理，但似乎从未回到这个问题。稍后，Cayley（[6]，第 3 卷） II，第164-178页）对群的某些表示下的$\mathbf{SL}(2, \mathbf{C})$的不变量进行类似的处理，并表明它们是前两个阶偏微分方程$Xf = 0, Yf = 0$的解，其中X和Y如上所述从“无限”获得小”的转变

$$
\begin{pmatrix}
0 & 0 \\
dt & 0
\end{pmatrix}
\quad \text{and} \quad
\begin{pmatrix}
0 & dt \\
0 & 0
\end{pmatrix}.
$$

在现代项中，这通过X和Y生成李代数$\mathfrak{sl}(2, \mathbf{C})$的事实来表达；此外，凯莱明确计算了括号 XY — YX，并表明它也是从“无限小”变换导出的。

乔丹在 1868 年的回忆录关于群的运动中[7]，从头到尾都使用了“无限小变换”的概念，但完全是从几何点的角度来看的。毫无疑问，他负责通过无限小的变换“生成”单参数群的想法：对于乔丹来说，它是通过“适当地重复”无限小的变换而获得的集合变换（*loc.cit.*，p. 243）。克莱因和李在他们的回忆录中，使用了相同的表达方式“重复无限小变换”[1b]，但上下文表明他们理解的是微分系统的积分。如果他们考虑的单参数群由变换$x' = f(x, y, t),\ y' = g(x, y, t)$组成，则相应的“无限小变换”由下式给出

$$
dx = p(x, y) dt, \qquad dy = q(x, y) dt
$$

其中$p(x, y) = \frac{\partial f}{\partial t}(x, y, t_0),\ q(x, y) = \frac{\partial g}{\partial t}(x, y, t_0)$和$t_0$对应到群的恒等变换。由于克莱因和李明确地知道函数$f$和$g$，因此他们毫不费力地验证函数

$$
t \mapsto f(x, y, t) \quad \text{and} \quad t \mapsto g(x, y, t)
$$

给出参数形式微分方程的积分曲线

$$
q(\xi, \eta)\ d\xi = p(\xi, \eta)\ d\eta
$$

经过到点 $(x, y)$，但它们没有给出一般性论证；此外，他们在回忆录的其余部分中没有使用这一事实。

(c) *接触变换*

在接下来的两年里，李似乎放弃了变换理论群（尽管他与克莱因保持着非常密切的联系，克莱因于1872年发表了他的“纲领”），转而研究接触变换、第一个阶偏微分方程和关系在这两种理论之间的积分。我们在这里不关心这些问题的历史，我们将仅限于提及几个似乎在转化理论群的起源中发挥了重要作用的点。

接触变换的概念概括了点变换和逆极坐标变换。 $\mathbf{C}^n$ 上的接触变换†大致是同构的开子集 $\Omega$ 的流形 $T'(\mathbf{C}^n)$ 的余切向量到$\mathbf{C}^n$ 到另一个的开子集 $\Omega'$ $T'(\mathbf{C}^n)$ 映射 $\Omega$ 到 $\Omega'$ 的规范 1-形式。在其他字中，如果$(x_1, \ldots, x_n, p_1, \ldots, p_n)$表示$T'(\mathbf{C}^n)$的规范坐标，则接触变换为同构

$$
(x_i, p_i) \mapsto (X_i, P_i)
$$

satisfying the relation

$$
\sum_{i=1}^n P_i dX_i = \sum_{i=1}^n p_i dx_i.
$$

这种变换发生在形式偏微分方程积分的研究中

$$
F\left( x_1, x_2, \ldots, x_n, \frac{\partial z}{\partial x_1}, \ldots, \frac{\partial z}{\partial x_n} \right) = 0.
$$

Lie 在他的研究期间通过泊松括号的操作熟悉了这些问题

$$
(f, g) = \sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \frac{\partial g}{\partial p_i} - \frac{\partial g}{\partial x_i} \frac{\partial f}{\partial p_i} \right)
$$

以及型(1)的微分算子的括号‡$[X, Y] = XY - YX$；他将泊松括号 (3) 解释为与 $g$ 相关的型 (1) 变换对 $f$ 的影响，并观察到泊松括号的雅可比恒等式意味着微分算子相应的到 $f$ 和 $g$ 的括号与括号 $(g, h)$ 相关联。 研究转化为函数 $g$，从而得到 $(F, g) = 0$，这出现在雅可比的方法中，用于积分

† 这里我们关注的是“齐次”接触变换。早些时候，研究型 (2) 的方程，但$z$出现在$F$中，导致 Lie 考虑$2n + 1$变量$z, x_1, \ldots, x_n, p_1, \ldots, p_n$中的接触变换，其中需要找到 $2n + 2$ 函数 $Z, P_i, X_i$ ($1 \leq i \leq n$) 和$\rho$（后者每点 $\neq 0$），这样$dZ - \sum_i P_i dX_i = \rho(dz - \sum_i p_i dx_i)$。这种情况看起来更为普遍，可以很容易地简化为“齐次”情况（[4]，第 2 卷，第 135-146 页）。

‡这些已经出现在雅可比-克莱布希理论的第一个阶偏微分方程$X_j f = 0$（$1 \leq j \leq r$）、概念的“完全系统”中，相当于Frobenius的“完全可积系统”；表征这些系统的基本定理（相当于“弗罗贝尼乌斯的定理”）是，括号$[X_i, X_j]$必须是$X_k$的线性组合（带有可变系数）。

对于李来说，偏微分方程（2）成为对无穷小接触变换的研究，该变换使给定方程保持不变。 Finally, Lie was led to study sets of functions $(u_j)_{1 \leq j \leq m}$ of the $x_i$ and $p_i$ such that the brackets $(u_j, u_k)$ are functions of the $u_h$ and called these sets "groups" (they had already essentially been studied by Jacobi) [3 c].

II。连续群和无穷小变换

突然之间，1873年秋天，李再次开始了变换群的研究，并取得了决定性的成果。只要可以从 1873-1874 年写给 A. Mayer 的几封信中追踪他的思路（[3]，第 5 卷，第 584-608 页），他从对 $n$ 变量进行“连续群”变换开始

$$
x'_i = f_i(x_1, \ldots, x_n, a_1, \ldots, a_r) \quad (1 \leq i \leq n)
$$

有效地取决于$r$参数$a_1, \ldots, a_r$；他观察到，如果变换（4）是参数值$a_1^0, \ldots, a_r^0$的恒等式，‡则$x_i$的第一个阶泰勒展开：

$$
f_i(x_1, \ldots, x_n, a_1^0 + z_1, \ldots, a_r^0 + z_r)
$$
$$
= x_i + \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) + \cdots \quad (1 \leq i \leq n)
$$

给出一个线性依赖于 $r$ 参数 $z_j$ 的“通用”无限小变换

$$
dx_i = \left( \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) \right) dt \quad (1 \leq i \leq n).
$$

与克莱因的回忆录一样，李对微分系统进行了积分

$$
\frac{d\xi_1}{\sum_k z_k X_{k1}(\xi_1, \ldots, \xi_n)} = \cdots = \frac{d\xi_n}{\sum_k z_k X_{kn}(\xi_1, \ldots, \xi_n)} = dt,
$$

† 这个谎言意味着 $f_i$ 不能用小于 $a_j$ 的 $r$ 函数的项来表达，或者雅克比行列式矩阵 $(\partial f_i / \partial a_j)$ 是秩 $r$ 的“一般”。

‡ 在他的第一个注中，李认为他可以“先验”证明整个集合变换中恒等式和逆矩阵的存在性（4）在合成下稳定；他后来认识到他的证明是不正确的，恩格尔为他提供了一个反例，转载于[4]，卷。 1、§ 44。然而，Lie 展示了如何在合成下稳定的“连续”系统 (4) 可以减少为群转化萌芽：这样系统是形式 $G \circ h$，其中 $G$ 是群转化萌芽，$h$ 系统（[4]，第 1 卷，定理 26，p. 163 和第 3 卷，定理 46，p. 572）的变换。

这给了他每个点$(z_1, \ldots, z_r)$一个参数群

$$
t \mapsto x_i' = g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, t) \quad (1 \leq i \leq n)
$$

这样对于所有 $i$ 都有$g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, 0) = x_i$。他通过巧妙的方法，利用变换(4)形式集合在合成下稳定的事实，证明单参数群(8)是给定群[3d]的子群。新的想法，整个理论的关键，是将函数(4)的泰勒展开取到第二个阶。他的论证过程相当混乱且具有启发性（[3d] 和 [3]，第 5 卷，第 600-601 页）；它可以表述如下。对于足够小的$z_j$，令$t = 1$代入(8)；这样就得到了群变换的新参数$z_1, \ldots, z_r$（这实际上是“规范参数”的第一次出现）。然后通过定义，使用 (7)，

$$
\frac{\partial g_i}{\partial t} = \sum_k z_k X_{ki}(x_1', \ldots, x_n')
$$

从而

$$
\frac{\partial^2 g_i}{\partial t^2} = \sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x_1', \ldots, x_n') \frac{\partial x_j'}{\partial t}
$$
$$
= \sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x_1', \ldots, x_n') \left( \sum_n z_n X_{nj}(x_1', \ldots, x_n') \right)
$$

这给出了

$$
x_i' = x_i + \left( \sum_k z_k X_{ki}(x_1, \ldots, x_n) \right)t
$$
$$
+ \frac{1}{2} \left( \sum_{k,h,j} z_k z_h \frac{\partial X_{ki}}{\partial x_j}(x_1, \ldots, x_n) X_{hj}(x_1, \ldots, x_n) \right)t^2 + \cdots,
$$

从而，对于$t = 1$，参数$z_j$中的泰勒展开

$$
x_i' = x_i + \left( \sum_j z_k X_{ki} \right) + \frac{1}{2} \left( \sum_{k,h,j} z_k z_h X_{hj} \frac{\partial X_{ki}}{\partial x_j} \right) + \cdots \quad (1 \leq i \leq n).
$$

我们将与向量相关的关系缩减为 $x' = G(x, z)$

$$
x = (x_1, \ldots, x_n), \qquad x' = (x_1', \ldots, x_n'), \qquad z = (z_1, \ldots, z_r);
$$

这些变换在合成下的集合的基本稳定性性质可以写成

$$
G(G(x, u), v) = G(x, H(u, v))
$$

其中$H = (H_1, \ldots, H_r)$独立于$x$； $H(u, 0) = u$和$H(0, v) = v$是直接的，从而展开

$$
H_i(u, v) = u_i + v_i + \frac{1}{2} \sum_{h,k} c_{ikh} u_h v_k + \cdots,
$$

其中省略的项在$u$或$v$中不是线性的。右(10)进行变换，利用(9)和(11)，然后比较两侧$u_h v_k$中的项。谎言获得关系

$$
(12)\quad \sum_{j=1}^n \left( X_{hj} \frac{\partial X_{ki}}{\partial x_j} - X_{kj} \frac{\partial X_{hi}}{\partial x_j} \right) = \sum_{l=1}^r c_{lhk} X_{li} \quad (1 \leq h, k \leq r, 1 \leq i \leq n).
$$

他在偏微分方程理论方面的经验使他将这些条件写成更简单的形式：按照（1）的模式，他将设定$z_k = 1, z_h = 0$对于（6）中的$h \neq k$（微分算子）获得的每个无限小变换相关联

$$
(13)\quad \Lambda_k(f) = \sum_{i=1}^n X_{ki} \frac{\partial f}{\partial x_i},
$$

并将条件(12)重写为形式

$$
(14)\quad [\Lambda_h, \Lambda_k] = \sum_l c_{lhk} \Lambda_l,
$$

他的理论的基石。在此之前他漠不关心地使用项“无穷小变换”和“无穷小变换”（例如[3 e]）； 关系 (14) 的简单性使他将算子 (13) 称为无穷小变换 $dx_i = X_{ki} dt$ ($1 \leq i \leq n$) [3 d] 的“符号”，并且很快他将算子 (13) 本身称为“无穷小变换”（[3 d] 和 [3]，第 5 卷，p. 589）。

然后，他意识到“连续群”理论与他早期的接触变换和偏微分方程的研究理论之间的密切联系。这种汇集使他充满了热情：“我早期的作品就好像一切都准备好了一样，等待着发现新的转型理论群”，他在 1874 年写给梅耶尔（[3]，第 5 卷，p. 586）。

在接下来的几年里，李继续进行转型群的研究。除了下面总结的一般定理（§III）之外，他还得到了一些更特殊的结果：线平面变换群的确定、射影群中低余维的子群、至多6个参数的群等。他并没有长期放弃微分方程。事实上，对他来说，变换群的理论似乎是微分方程积分的工具，其中变换群起到了类似于代数方程伽罗瓦群的作用。†

† 这个研究对微分方程的一般理论影响不大，因为这样的方程的自同构群通常是微不足道的。作为补偿，对于某些型方程（对于例线性方程），Picard、Vessiot 以及最近的 Ritt 和 Kolchin 后来获得了有趣的结果。

我们注认为，这个研究同样引导他在无限个参数中引入某种变换集合，他称之为“无限连续群”；他为上述型（4）参数的有限数中的变换群保留了名称“有限连续群”。

李群-李代数“字典”

“有限连续”理论群是由李自1874年开始在众多回忆录中发展起来的，在与F.恩格尔合作撰写的雄伟论文“Theorie der Transformationsgruppen”（[4]，1888-1893））中系统地阐述；它是第一卷和第三卷最后五个章的研究对象，第二卷专门研究接触变换。

正如标题所示，这项工作只涉及方程（4）意义上的变换群，其中“变量”$x_i$的空间和“参数”$a_j$的空间最初发挥了如此重要的作用。另一方面，“抽象”群的概念在那个时期还没有被明确孤立； 1885 年 ([3f], §5) Lie 指出，在 (10) 的记号中，方程 $w = H(u, v)$ 给出了群定义两个变换的合成的参数，一个新的群，他将其视为对群的变换空间个参数，从而得到他所谓的“参数群”（他甚至得到了两个，即左翻译的群和右翻译的群†）。

方程（4）中的变量$x_i$和参数$a_j$在原理中被假定为复数（除了第3卷的章XIX–XXIV），函数$f_i$被假定为解析； Lie 和 Engel 当然意识到，这些函数并不是对 $x_i$ 和 $a_j$ 的所有复杂值进行一般性定义，因此此类函数的合成会带来严重的困难（[4]，第 1 卷，第 15-17 页，第 33-40 页和帕西姆）；尽管他们在自始至终都写得好像他们正在研究的变换中的合成在没有限制的情况下也是可能的，但这无疑是为了方便

‡ 今天他们被称为“谎言伪团体”；应注意不要将它们与本卷中定义的“Banach”李群相混淆。
§ 从1886年到1898年，李占据了莱比锡由克莱因留下的空缺职位，并让恩格尔担任他的助手；这种情况有利于活跃的数学学校的产生，以及李思想的传播，而在此之前，人们对他的思想知之甚少（特别是因为他的第一个回忆录通常是用挪威语写成的，并发表在《克里斯蒂安学院的Comptes Rendus de l'Académie de Christiania》上，而该书在其他地方很少使用）。因此，在年轻的法国数学家去德国求学的情况很少见的时候，E. Vessiot 和 A. Tresse 在莱比锡跟随 Sophus Lie 学习了一年。
† 置换群的类似概念已由乔丹在他的“论文”中介绍和研究。

的结果，并在必要时明确重申视图的“本地”点（cf.loc.cit.，p. 168或189代表例或同上，第3卷，p. 2，注在页面底部）；在其他字中，他们研究的数学对象与我们在这篇论文中所说的律chunk of 运算很接近。有时，他们会毫不犹豫地考虑全局群，因为例是经典群的4个级数（[4]，第3卷，p. 682），但似乎并没有问自己一般来说什么构成“全局群”的问题；他们满足于获得经典群的“参数”（这些群的“变量”没有引入任何困难，因为所讨论的变换是$\mathbf{C}^n$的线性变换）恒等变换的邻域中参数的“局部”系统，而不用担心他们正在编写的公式的有效域下来。然而，它们集合本身问题巧妙地源于局部理论‡：“混合”群的研究，即群具有有限的数连通分量，例如正交群（[4]，第1卷，p. 7）。他们将这项研究作为对合成下稳定变换的集合的研究，以及到集合$H_j$的并的逆转换的研究，其中每一个都由函数$(f_i^{(j)})$的系统描述，如（4）中所示；每个$H_j$的（基本）参数中的数甚至是先验假设的$a$依赖于$j$，但他们表明事实上这个数对于所有$H_j$都是相同的。他们的主要结果是存在有限连续群$G$，使得$H_j = G \circ h_j$对于某些$h_j \in H_j$和对于所有$j$；他们还确定 $G$ 在混合群中是正规的，并指出后者约化的不变量与 $G$ 和不连续群的不变量的确定（[4]，第 1 卷，章 18）。

[4]中发展的一般理论通过实现一个“字典”而结束（没有作者说如此非常系统地），将“有限连续”群的属性翻译成其无穷小变换的集合的属性。它基于“谎言的三个定理”，每个谎言由断言及其逆命题组成。

第一个定理（[4]，第1卷，第33和72页以及第3卷，p. 563）首先肯定，如果（4）中的参数有效，则形式的偏微分方程函数$f_i$满足系统

$$
\frac{\partial f_i}{\partial a_j} = \sum_{k=1}^r \xi_{kji}(f(x, a)) \psi_{kj}(a) \quad (1 \leq i \leq n)
$$

其中矩阵 $(\xi_{kji})$ 的最大值为秩和 $\det(\psi_{kj}) \neq 0$；反之，如果

‡ 回想一下（历史注记到代数、章 VIII），继 H. Poincaré 的注（[14]，第 V，第 77-79 页）之后，几位作者研究了有限维结合律的可逆元的群代数。对于注来说，在这个主题上有趣的是，E. Study在他关于这个主题的著作中引入了一种象征意义，其本质上相当于考虑由参数群定义的抽象群。

函数$f_i$有这个性质，公式（4）定义群转变的萌芽。

第二个定理（[4]，第 1 卷，第 149 和 158 页，以及第 3 卷，p. 590）在一方面 $\xi_{kli}$ 和另一方面 $\psi_{ij}$ 之间给出关系：$\xi_{kli}$ 上的条件可以写成形式

$$
\sum_{k=1}^n \left( \xi_{ik} \frac{\partial \xi_{jkl}}{\partial x_k} - \xi_{jk} \frac{\partial \xi_{iil}}{\partial x_k} \right) = \sum_{k=1}^r c_{ij}^k \xi_{kli} \quad (1 \leq i, j \leq r, 1 \leq l \leq n)
$$

其中 $c_{ij}^k$ 是 $i, j$ 中斜对称的常数 ($1 \leq i, j, k \leq r$)。 Maurer [10]给出的形式中$\psi_{ij}$上的条件为：

$$
\frac{\partial \psi_{kl}}{\partial a_m} - \frac{\partial \psi_{km}}{\partial a_l} = \frac{1}{2} \sum_{1 \leq i, j \leq r} c_{ij}^k (\psi_{il} \psi_{jm} - \psi_{jl} \psi_{im}) \quad (1 \leq k, l, m \leq r).
$$

通过引入$(\psi_{ij})$的逆变矩阵$(\alpha_{ij})$和无穷小变换

$$
X_k = \sum_{i=1}^n \xi_{kli} \frac{\partial}{\partial x_i}, \qquad A_k = \sum_{j=1}^r \alpha_{kj} \frac{\partial}{\partial a_j} \quad (1 \leq k \leq r)
$$

(16)和(17)可分别写成：

$$
[X_i, X_j] = \sum_{k=1}^r c_{ij}^k X_k \quad (1 \leq i, j \leq r).
$$
$$
[A_i, A_j] = \sum_{k=1}^r c_{ij}^k A_k
$$

相反，如果给定线性无关的$r$无限小变换$X_k$（$1 \leq k \leq r$）和满足条件（19），则由这些变换生成生成的单参数子群是$r$基本参数中的变换群。

最后，第三个定理（[4]，第1卷，第170和297页以及第3卷，p. 597）约化确定无穷小变换$(X_k)_{1 \leq k \leq r}$满足（19）到纯代数问题的系统：以下必须成立：

$$
c_{ij}^k + c_{ji}^k = 0
$$
$$
\sum_{l=1}^r (c_{il}^m c_{lj}^k + c_{kl}^m c_{lj}^i + c_{jl}^m c_{ki}^l) = 0 \quad (1 \leq i, j, k, m \leq r).
$$

相反，\footnote{† 这个逆命题并不是没有困难就能得到的。 Lie [3 d] 给出的第一个证明包含在经过到伴随群中，并且实际上仅当给定李代数的中心为 \{0\} 时才有效。然后他给出了两个一般性的证明（[4]，第2卷，章17和第3卷，第599-604页）；非常重要的是，第一个基于接触变换，并且 Lie 发现它比第二个更自然。}如果满足 (21) 和 (22)，则存在系统无穷小变换满足关系 (19)，从而带有 r 参数的变换群（在其他字，具有常数系数形式李代数的X_k的线性组合以及相反的每个有限维李代数都可以通过这种方式获得）。

这些结果是通过研究同构的问题而完成的。 如果两个变换群可以通过变量上的可逆坐标变换和参数上的可逆坐标变换从一个变换到另一个变换，则称为相似变换：从他的研究一开始，Lie在定义“规范参数”时就很自然地关注这个概念。 He showed that two groups are similar if, by a transformation on the “variables”, it is possible to transform the infinitesimal transformations of the one into those of the other ([4], vol. 1, p. 329). 要实现这种情况，必要的条件是这两个群中的李代数是同构的，这由说表示群是“gleichzusammengesetzt”；但这条件还不够，整个章（[4]，第1卷，章19）致力于获得补充条件，以确保群“相似”。 另一方面，置换群的理论提供了两个这样的群的“全息体同构”的概念（底层“抽象”群的同构）； Lie 将这个概念转置为变换群，并表明两个这样的群是“全面同构”当且仅当它们的李代数是同构的（[4]，第1卷，p. 418）。 特别是，每个变换群与其每个参数群都是全面同构的，这表明，当我们希望研究群的结构时，它所操作的“变量”并不重要，事实上，重要的是李代数。†

总是通过与置换群的理论进行类比，李介绍了子群的概念、正常子群和“分面体同构”（满同态），并证明它们对应到子代数、理想和满射的理论李代数同态；他之前已经遇到过“多面体同构”的一个特别重要的例，即伴随表示，并认识到它的关系与中心的群（[3.f]，§ 3, no. 9）。对于这些结果，对于基本定理，基本工具是 Jacobi-Clebsch 定理，它给出了微分系统的完全可积性（定理的形式之一称为“Frobenius”）；然而，他使用单参数群给出了新的证明（[4]，第1卷，章6）。

† 类似的演变可以在“抽象”理论群，特别是有限群中指出。它们首先被定义为变换群，但凯莱已经指出，重要的是变换由一个另一个组成的方式，而不是群的具体表示作为特定对象的置换群的性质。

传递性的概念和原性，对于置换群来说非常重要，对于“有限连续”变换群来说同样自然地发生，并且Lie-Engel论文对此进行了详细的研究（[4]，第1卷，章13和passim）； 关系与稳定子子群的点和同质空间的概念被感知（在不考虑全局点的情况下可能）（[4]，第1卷，p. 425）。

最后，在[4]中，通过引入导出群的概念和可解的群（Lie称为“可积群”；这个术语，由微分方程理论提出，一直沿用到H. Weyl的著作）（[4]，第1卷，p. 261和第 3 卷，第 678–679 页）； 换位子和括号之间的关系已于 1883 年在其他地方被 Lie 感知到（[3]，第 5 卷，p. 358）。

基本定理的其他证明

在[8]中，F. Schur 表明，在正则坐标中，(15) 满足的微分方程的 $\psi_{ik}$

$$
\frac{d}{dt} (t \psi_{ik}(ta)) = \delta_{ik} + \sum_{j,l} c_{jl}^k t a_l \psi_{ij}(ta).
$$

这些被积分并给出公式等价于公式

$$
\sigma(X) = \sum_{n > 0} \frac{1}{(n+1)!} (\operatorname{ad}(X))^n
$$

我们的章III, § 6, no. 4、命题12；特别是，在规范坐标中，$\psi_{ij}$可以扩展到$a_k$的积分函数。 F. Schur 推导出了一个结果，使李的早期注变得精确：如果在变换群的定义(4)中，仅假设$f_i$是类$C^2$，则群与解析式全面同构群。

† 谎言已经在没有证明的情况下陈述了此型 ([3 g], no. 7) 的结果。他在几何基础上的研究（“亥姆霍兹的问题”）的带领下到达了那里，他指出分析假设不是自然的。

F. Schur 的结果导致希尔伯特在 1900 年提出，如果仅假设 $f_i$ 是连续的，同样的结论是否仍然成立（“希尔伯特的 5 次问题”）。这问题刺激了很多研究。沿着这条线最完整的结果是下面的定理，由 A. Gleason、D. Montgomery 和 L 证明。拉链；每个局部紧拓扑群都有一个开子群，它是李群的逆极限；这意味着每个局部欧氏群都是李群。有关此问题的更多详细信息，cf. D. Montgomery 和L。齐平[41]。

研究关于微分系统的积分，E. Cartan ([12], vol. II_2, p. 371)于1904年引入 Pfaffian 形式

$$
\omega_k = \sum_{i=1}^r \psi_{ki} da_i \quad (1 \leq i \leq r)
$$
（在（15）的记号中），后来称为*Maurer-Cartan形式*。 Maurer 条件 (17) 可以写成

$$
d\omega_k = -\frac{1}{2} \sum_{i,j} c_{ij}^k \omega_i \wedge \omega_j;
$$

E.嘉当证明，有限连续群理论可以从$\omega_k$开始发展，并建立了这个点视图和李视图的等价。但是，对他来说，这个方法的兴趣首先在于它可以适应“无限连续群”，他比李更进一步推进了这一理论，这使他能够发展他的广义“移动框架”理论。

IV。 李代数的理论

一旦在变换群和李代数之间获得了对应，该理论就进行了相当多的代数转向，并集中于对李代数的深入研究。†

第一个短暂时期，从 1888 年到 1894 年，以恩格尔和他的学生 Umlauf，尤其是 Killing 和 E. Cartan 的作品为标志，在复杂的李代数上取得了级数的惊人成果。我们之前已经看到，可解李代数的概念是由Lie本人造成的，他（在复杂的情况下）证明了定理可解的线性李代数还原为三角形形式（[4]，第1卷，p. 270）。‡ Killing观察到[11]存在李代数最大的可解理想（我们现在称之为根式），李代数与其根式的商有零根式；他用零部首*半单*来称呼李代数，并证明它们是单代数的乘积（后者概念已经由Lie引入，他证明了“经典”代数的简单性（[4]，第3卷， p. 682))。

另一方面，Killing 在李代数中引入了特征方程 $\det(\mathrm{ad}(x) - \omega . 1) = 0$，这是 Lie 在研究二维 Lie 子代数包含给定元素李代数时遇到的。我们将在本书的其他历史注记中回到方法的数学分析，其中杀戮，同时深入研究亲

† 项“李代数”由 H. Weyl 于 1934 年提出：在他 1925 年的作品中，他使用了“无穷小群”这一表达方式。早些时候，数学家简单地谈到了群的“无穷小变换X_1f，...，X_rf”，李和恩格尔经常将其缩写为说“群X_1f，...，X_rf”！

‡ 几乎在研究的开始，李遇到了可解线性群，甚至实际上是幂零线性群 [3 h]。

半单代数的“通用”特征方程根的性质，取得了最显着的成果，即（复杂）简单李代数的完整确定。§

Killing 证明了可解代数的导出代数是“秩 0”（这意味着 ad $x$ 对于代数的每个元素 $x$ 都是幂零的）。恩格尔几乎立即证明了“秩 0”的代数是可解的（这个叙述本质上就是我们所说的恩格尔在章I, § 4, no. 2中的定理）。另一方面，嘉当在他的论文中介绍了我们现在所说的“杀戮形式”，并建立了两个基本的判据，其特征在于这个形式可解李代数和半简单的李代数。

Killing 肯定了([11], IV)李代数的派生代数是半单代数的和及其部首，它是幂幂的，但他的证明是不完备的。稍后，E. Cartan 在没有证明（[12]，第 I_1 卷，p. 104）的情况下宣布，更一般地，每个李代数都是其部首的和和半单子代数；这一时期在这个方向上无可争议地确立的唯一结果是恩格尔的定理，确认在每个不可解的李代数中，存在维数 3 的简单李子代数。第一个发表的嘉当叙述的证明（对于复数李代数）是由于E. E.列维[18]； 另一个证明（在实际情况下同样有效）由 J. H. C 给出。怀特海于 1936 年[26a]。 1942 年，A. Malcev 在“Levi 截面”共轭之前完成了唯一性定理的结果。

从他的第一部作品开始，Lie 就关注任意李代数和线性李代数之间的同构的问题。他相信通过考虑伴随表示（并从中推导出他的“第三个定理”的证明），他已经肯定地解决了这个问题[3 d]；他意识到他的证明仅对于李代数和零中心是正确的，给出了另一个错误的证明（[3f]，§ 3, no. 9），然后认识到（[3g]，p. 231）问题仍然悬而未决。事实上，这个问题长期以来一直如此，直到1935年才最终被阿多[27]肯定地解决。另一方面，Lie本质上提出了确定最小维数的简单李代数的线性表示的问题，并解决了经典的群；在他的论文中，嘉当也解决了这个问题的特殊问题单代数†；他为此使用的方法二十年后被他推广以获得实数或复简单李代数的所有不可约表示。

§ 直到他发现了维数 52 的两个例外群，但没有注意到它们是同构的。 （他只考虑了复杂简单的李代数，而当时还没有考虑更一般的问题；Killing的方法实际上对于特征0的任何代数闭域都有效）。

† 嘉当的方法包括研究简单李代数的非平凡扩张李代数和最小维数的（交换）根式。

线性表示完全可约的性质似乎是Study第一次遇到（在几何形式中）。在一份未发表的手稿中，但在[4]，卷中引用。 3，第785-788页，他证明了李代数$\mathbf{SL}(2, \mathbf{C})$的线性表示的性质，并获得了$\mathbf{SL}(3, \mathbf{C})$和$\mathbf{SL}(4, \mathbf{C})$的部分结果。 Lie 和 Engel 在这次猜想中，对于所有 $n$，$\mathbf{SL}(n, \mathbf{C})$ 完全可归约定理成立。 线性表示与半单李代数的完全可约性是由 H. Weyl 在 1925 年† 通过全局型论证建立的（见下文）。第一个代数证明于 1935 年由 Casimir 和 van der Waerden 获得 [32]；此后，R. Brauer [31]（这是我们复制的）和 J. H. C 给出了其他代数证明。怀特海[26 b]。

最后，在指数映射（cf.见下）的研究过程中，H. Poincaré（[14]，第3卷）考虑了所有阶的微分算子的结合代数，由李代数的算子生成；他本质上表明，如果$(\mathbf{X}_i)_{1 \leq i \leq n}$是李代数的基，则由$\mathbf{X}_i$生成的结合律代数与基一样，具有$\mathbf{X}_i$的某些对称函数（源自a的非交换“单项式”的和）由因子的所有置换给出单项式）。他的证明本质上是代数性质的，并允许他获得我们在章I中抽象的定义的包络代数结构。 G. Birkhoff [29 b] 和 E. Witt [30] 于 1937 年给出了类似的证明。‡

上面引用的大多数结果仅限于实数或复数李代数，其中单独的对应到李群通常意义上的。除了$\mathbf{R}$或$\mathbf{C}$之外，李代数对域的研究是由Jacobson [28a]开始的，他表明绝大多数经典结果（即章I的结果）对于特征零的任何域仍然成立。

V。指数和豪斯多夫公式

指数映射上的第一个研究归功于E. Study和F. Engel； Engel [9 b] 指出，对于 $\mathbf{SL}(2, \mathbf{C})$，指数不是满射（对于 $a \neq 0$，例 $\begin{pmatrix} -1 & a \\ 0 & -1 \end{pmatrix}$ 不是指数），但它对于 $\mathbf{GL}(n, \mathbf{C})$ 来说是满射的，因此对于 $\mathbf{PGL}(n, \mathbf{C})$ 也是满射的（后者性质已经被 $n = 2$ 的研究注意到）；因此$\mathbf{SL}(2, \mathbf{C})$和$\mathbf{PGL}(2, \mathbf{C})$给出了两个局部同构的群的例，然而它们与全局同构有很大不同

† H. Weyl 在这个场合评论说，E. Cartan 对于不可约表示给出的构造隐含地使用了这个性质。

‡ 由 $\mathbf{X}_i$ 生成的更高阶微分算子的首次使用无疑是对完全约简性定理的证明使用“卡西米尔算子”。 1950年的之后，Gelfand和他的学校的研究以及无限维线性表示上的Harish-Chandra，将这些算子带到了最前沿。

点的视野。恩格尔还证明，指数对于其他经典群来说是满射的；这项工作由 Maurer、Study 和其他人接手并进行，但没有产生实质性的新成果。

1899 年，H. Poincaré（[14]，第 3 卷，第 169-172 和 173-212 页）从不同的点角度开始研究指数映射。他的回忆录似乎被匆忙编辑过，因为在几个地方他确认相连的群的每一个元素都是指数，而他在其他地方给出了例相反。他的结果主要与伴随表示有关：他证明这样的群G的半单元素可能是李代数L(G)的无穷大元素的指数，而非半单元素可能不是完全是指数级的。如果 ad(X) 没有特征值，即 $2\pi i$ 的非零倍数，则 exp 的 étale 位于 X。他还证明，如果 U 和 V 描述 L(G) 中的循环，并且 W 由连续性定义，使得 $e^U.e^V = e^W$，则有可能不返回到 W 的原始值。他使用了剩余类公式，本质上等于

$$
\Phi(\mathrm{ad}\,X) = \frac{1}{2\pi i} \int \frac{\Phi(\xi)\,d\xi}{\xi - \mathrm{ad}\,X}
$$

其中$\mathrm{ad}(X)$是半单元素，其非零特征值为重数1，$\Phi$是级数的积分，收敛半径为足够大，积分是在特征值周围的轮廓上进行的$\mathrm{ad}\,X$；他还研究了当X倾向于与倍数特征值进行变换时会发生什么。

研究已被转换为 W 的函数和公式 $e^U.e^V = e^W$ 中的 V，只是之前 Poincaré 的工作，已成为坎贝尔 [13] 的两个回忆录的对象。正如贝克稍后所写的“……*谎言理论以一种明显的方式表明，乘积*$e^Ue^V$*是形式*$e^W$*其中*W*是*U*和*V*中的交替项的级数...”。后来关于这个主题的工作旨在使这个断言精确，并为W给出明确的公式（或构造的方法）（“Hausdorff公式”）。 之后 Campbell 和 Poincaré、Pascal、Baker [15] 和 Hausdorff [16] 回到了这个问题；各自认为前辈的证明没有说服力；主要的困难在于“交替”的含义：它们是特殊的元素还是李代数，还是通用的“符号”表达式？坎贝尔、庞加莱和贝克都没有明确表达自己对这个点的看法。另一方面，豪斯多夫的回忆录则非常精确；他首先研究了有限数中的（非交换）结合形式幂级数的代数，并将 U、V、W 视为该代数的元素。他通过类似于他的前辈的微分方程论证证明了 W 的存在。他用同样的论证证明了当不定式被有限维李代数的元素代替时级数的收敛性。正如贝克和庞加莱独立所说，这个结果可以用来给出李的第三个定理中的证明；他在李群和李代数之间澄清了对应，对于涉及换位子子群的例。

1947 年，Dynkin [39] 再次提出这个问题，并通过从一开始就考虑规范的李代数（有限维或其他，超过 $\mathbf{R}, \mathbf{C}$ 或超度量域），获得了 Hausdorff 公式的显式系数。†

VI。线性代表和全局李群

我们刚才提到的所有作品都没有对定义和研究全球李群做出任何诚实的尝试。 H. Weyl 率先朝这个方向迈出了一步。他受到了两个理论的启发，这两个理论在此之前都是独立发展的：E. Cartan提出的线性表示理论和复半单李代数理论，以及Frobenius提出的线性表示理论和有限群理论，并且刚刚被I转置为正交群。舒尔，使用了赫尔维茨的想法。后者展示了 [17] 如何通过关于不变测度的积分，通过有限群上平均值的替换运算获得正交群或酉群的形式不变量。他还指出，通过应用这个方法到酉群，获得了一般线性群的不变量，即“一神论技巧”的第一个例。 1924年，I。 Schur [20] 使用该过程通过构造不变的非简并正定厄米特形式来证明正交群 $\mathbf{O}(n)$ 和酉群 $\mathbf{U}(n)$ 表示的完全可约性；他通过“一神论把戏”推导出$\mathbf{O}(n, \mathbf{C})$和$\mathbf{SL}(n, \mathbf{C})$的全纯表示的完全可约性，为$\mathbf{O}(n)$和$\mathbf{U}(n)$的特征标建立了正交关系，并确定了$\mathbf{O}(n)$的特征标。 H. Weyl 立即将这个方法扩展到复半单李代数 [21]。给定这样的代数$g$，他证明它有一个“紧实数形式”（相当于说，它是通过$\mathbf{R}$到$\mathbf{C}$的标量扩张从代数$g_0$超过$\mathbf{R}$获得的）其伴随群 $G_0$ 是紧的）。此外，他证明了$G_0$的基本群是有限的，因此$G_0$的万有覆盖‡是紧的。通过对 Schur 程序的适当修改，他推论出表示与 $g$ 的完全可约性，并且还通过全局方法给出了

† 在超度量情况下，由于 $1/n$ 的 $p$ 进数绝对值的渐近行为，$n$ 趋于无穷大，上界不能的经典方法无需采取预防措施即可扩展。

‡ H. Weyl 并没有明确地定义这个概念，自从编辑黎曼曲面课程（1913）以来他就已经熟悉了这个概念。 O. Schreier [22] 在 1926-1927 年首次给出了拓扑群的定义和“连续”群（即局部同胚于欧氏空间），以及这种拓扑的普遍覆盖的构造。 群。

特征标表示$g$。在给I的信中。 Schur (Sitzungsber. Berlin, 1924, pp. 338–343)，H. Weyl 总结了 Schur 不知道的 Cartan 的结果（cf. [20], p. 299, 注在页面底部），并比较了两种方法：Cartan 的方法给出了所有的全纯表示只需将群与李代数 $g$ 连接起来；在正交群的情况下，表示是由双覆盖（后来称为旋量群）获得的，它逃脱了 Schur；另一方面，Schur 的方法具有显示完全可约性并明确给出特征标的优点。

之后 H. Weyl、E. Cartan 在其关于对称空间和李群的研究中采用了公开的全局方法。这种方法是他 1930 年对“有限连续”理论的阐述（[12]，第 I_2 卷，第 1165-1225 页）群的基。特别是，我们在这里找到了第三基本定理的全球版本的第一个证明（给定李代数存在李群）；嘉当还表明，实李群的每个闭子群都是李群（章III, § 8, no. 2，定理2），这概括了J. von Neumann关于线性群的闭子群的结果[23]。在这个回忆录中，冯·诺依曼还证明了半单群的每一个连续的表示都是实解析的。

有了之后这些作品，“经典”意义上的李群理论（即有限维超过$\mathbf{R}$或$\mathbf{C}$）在其本质上或多或少是完整的。 Pontrjagin 在他的拓扑学著作群 [36] 中对此进行了首次详细阐述；在那里，他遵循的方法与李的方法非常接近，但仔细区分了本地和全球。随后Chevalley的书[38]也是包含第一次系统讨论解析流形和外微分演算的理论； Lie 的“无穷小变换”在那里表现为向量域和李群 G 的李代数与 G 上的左不变量域的空间相同。他省略了任何关于“群细菌”和“变换群”的讨论。

VII。 扩张概念李群

如今，李理论的生命力体现在其应用的多样性（拓扑、微分几何、算术等）以及并行理论的创建中，其中底层的流形结构被类似的结构（$p$-adic流形，代数簇，概形，形式化）所取代。 概形，。我们在这里不关心这些发展的历史，我们将仅限于章III中涉及的内容：Banach李群和$p$-adic李群。

(a) 巴拿赫李群

这里我们关心的是“无限维”李群。从局部点来看，欧氏空间中0的邻域被Banach空间中0的邻域替代。这就是 G. Birkhoff 在 1936 年所做的[29 a]，从而实现了*完整规范的李代数* 的概念以及在 Banach 空间的开放集合上定义的对应和“群胚芽”。大约 1950 年，Dynkin 通过将 Hausdorff 公式扩展到这种情况（cf. *同上*），完成了这些结果。

定义以及 Birkhoff 和 Dynkin 的结果是局部的。直到最近，似乎还没有人试图使相应的全局理论变得明确，这无疑是因为缺乏应用。†

(b) *p-adic 李群*

这样的群于1907年在Hensel [19]关于*p*-adic解析函数（由展开定义为积分级数）的著作中首次遇到。他特别研究了指数和对数；尽管级数和定义有*先验*令人惊讶的行为（对于例，指数级数并非处处收敛），它们的基本功能属性仍然有效，这在加法群和乘法群之间提供了$\mathbf{Q}_p$的*局部同构*（或者更一般地，任何完整的超度量） 域 / 特征零）。

A. Weil [33] 和 E. Lutz [34] 在 *p*-adic 椭圆曲线 (1936) 的研究中同样关注交换性（但这次是非线性的）群。除了算术应用之外，基于不变微分形式的积分，在群和加法群之间构建了局部同构。正如C所指出的，方法同样适用于阿贝尔的品种。不久之后，查博蒂在没有进一步解释的情况下使用它来证明“莫德尔猜想”的一个特殊情况[35]。

从那时起，很明显，李群的*局部*理论几乎可以应用于*p*-adic情况，而几乎没有任何变换。 李群–李代数的基本“字典”定理于1942年在Chevalley的学生R. Hooke [37]的论文中建立；这项工作还包含 E. Cartan 的定理在实李群的封闭子群上的 *p*-adic 类似物。

最近，M. Lazard [42 b] 开发了一个更精确的形式的“字典”，用于在 $\mathbf{Q}_p$ 上进行紧凑分析群。他证明了紧致群 G 上 *p*-进解析结构的存在与 G 上的某些过滤密切相关，并给出了其各种应用（对于 G 的例到上同调）。 Lazard 的工具之一是 Dynkin 对 *p*-adic Hausdorff 级数收敛结果的改进 [42 a]。

† 如果尽管缺乏应用，我们在章III中提到了“Banach”群，那是因为Banach流形在数学分析中越来越多地使用（甚至用于有限维流形的研究），并且因为，此外，这个推广没有提供额外的困难。

VIII。免费李代数

剩下要说的是关于李代数的作品的级数，它与李群理论的联系非常薄弱；另一方面，这个研究对于“抽象”理论群，尤其是幂零群有着重要的应用。

它的起源是 P. Hall [24] 的作品，发表于 1932 年。然而，这里不讨论李代数：P. Hall 想到的是研究 $p$ 群中的某个类，他称之为“常规”群。但这促使他详细检查迭代的换位子和群的下中央级数；在这个主题上，他建立了雅可比恒等式的一个版本（cf.章II, § 4, no. 4，公式（20））和“大厅公式”

$$(xy)^n = x^n y^n (x, y)^{n(1-n)/2} \ldots$$（cf.章II, § 5，习题9）。

W. Magnus（[25 a] 和 [25 b]）和 E. Witt [30] 的基础著作几乎立即（1935-1937 年）出现。在[25a]中，马格努斯使用了与豪斯多夫相同的形式幂级数$A$的代数（自称为“马格努斯代数”）；他将游离的群F嵌入其中，利用$A$的自然过滤得到F的子群的递减序列$(F_n)$；它是过滤的前例之一。他猜想F的下中央级数的$F_n$重合和项。这个猜想在他的第二个回忆录中得到了证明[25b]；同样在这项工作中，他明确地表明了他的想法与 P. Hall 的想法之间的接近关系 ，并定义了自由的李代数 L（作为 $A$ 的子代数），他表明它本质上与 F 的分级代数相同。在[30]中，Witt 在各种点上完成了这个结果。他特别证明了L的包络代数是一个自由结合律代数，并立即推导出L的齐次分量的秩（“维特公式”）。

至于L的基的证明被称为“大厅基”（cf.章II, § 2, no. 11），似乎只在1950年出现在M. Hall的注中[40]，尽管它在P. Hall和W. Magnus引用的作品中是隐含的上面。

1. F. KLEIN and S. LIE: (a) Sur une certaine famille de courbes et surfaces, C. R. Acad. Sci., 70 (1870), pp. 1222–1226 and 1275–1279 (= [2], pp. 416–420 and [3], vol. 1, pp. 78–85); (b) Über diejenigen ebenen Kurven, welche durch ein geschlossenes System von einfach unendlich vielen vertauschbaren linearen Transformationen in sich übergehen, Math. Ann., 4 (1871), pp. 50–84 (= [2], pp. 424–459 and [3], vol. 1, Abh. XIV, pp. 229–266).
2. F. KLEIN, Gesammelte mathematische Abhandlungen, Bd. I, Berlin (Springer), 1921.
3. S. LIE, Gesammelte Abhandlungen, 7 vol., Leipzig (Teubner): (a) Über die Reziprozitätsverhältnisse des Reyeschen Komplexes, vol. I, Abh. V, pp. 68–77 (= Gött. Nach. (1870), pp. 53–66); (b) Über eine Klasse geometrischer Transformationen, vol. I, Abh. XII, pp. 153–214 (= Christiana For. (1871), pp. 182–245); (c) Über partielle Differentialgleichungen erster Ordnung, vol. III, Abh. VII, pp. 32–63 (= Christiana For. (1873), pp. 16–51); (d) Theorie der Transformationsgruppen II, vol. V, Abh. III, pp. 42–75 (= Archiv f. Math., 1 (1876), pp. 152–193); (e) Ueber Gruppen von Transformationen, vol. V, Abh. I, pp. 1–8 (= Gött. Nachr. (1874), pp. 529–542); (f) Allgemeine Untersuchungen über Differentialgleichungen, die eine kontinuierliche endliche Gruppe gestatten, vol. VI, Abh. III, pp. 139–223 (= Math. Ann., 25 (1885), pp. 71–151); (g) Beiträge zur allgemeinen Transformationentheorie, vol. VI, Abh. V, pp. 230–236 (= Leipziger Ber. (1888), pp. 14–21); (h) Theorie der Transformationsgruppen III, vol. V, Abh. IV, pp. 78–133 (= Archiv f. Math., vol. III, (1887), pp. 93–165).
4. S. LIE and F. ENGEL, Theorie der Transformationsgruppen, 3 vol., Leipzig (Teubner), 1888–1893.
5. J. J. SYLVESTER, Collected Mathematical Papers, 4 vols., Cambridge, 1904–1911.
6. A. CAYLEY, Collected Mathematical Papers, 13 vols., Cambridge, 1889–1898.

7. C. Jordan, Mémoire sur les groupes de mouvements, Annali di Math., 11 (1868–1869), pp. 167–215 and 332–345 (= Oeuvres, vol. IV, pp. 231–302).

8. F. Schur: (a) Zur Theorie der aus Haupteinheiten gebildeten Komplexen, Math. Ann., 33 (1889), pp. 49–60; (b) Neue Begründung der Theorie der endlichen Transformationsgruppen, Math. Ann., 35 (1890), pp. 161–197; (c) Zur Theorie der endlichen Transformationsgruppen, Math. Ann., 38 (1891), pp. 273–286; (d) Über den analytischen Character der eine endliche continuierliche Transformationsgruppe darstellende Funktionen, Math. Ann., 41 (1893), pp. 509–538.

9. F. Engel: (a) Über die Definitionsgleichung der continuierlichen Transformationsgruppen, Math. Ann., 27 (1886), pp. 1–57; (b) Die Erzeugung der endlichen Transformationen einer projektiven Gruppe durch die infinitesimalen Transformationen der Gruppe, I, Leipziger Ber., 44 (1892), pp. 279–296, II (mit Beiträgen von E. Study), ibid., 45 (1893), pp. 659–696.

10. L. Maurer, Über allgemeinere Invarianten-Systeme, Sitzungsber. München, 18 (1888), pp. 103–150.

11. W. Killing, Die Zusammensetzung der stetigen endlichen Transformationsgruppen: (I) Math. Ann., 31 (1888), pp. 252–290; (II) ibid., 33 (1889), pp. 1–48; (III) ibid., 34 (1889), pp. 57–122; (IV) ibid., 36 (1890), pp. 161–189.

12. E. Cartan, Oeuvres complètes, 6 vol., Paris (Gauthier-Villars), 1952–54.

13. J. E. Campbell: (a) On a law of combination of operators bearing on the theory of continuous transformation groups, Proc. London Math. Soc., (1) 28 (1897), pp. 381–390; (b) On a law of combination of operators (second paper), ibid., 29 (1898), pp. 14–32.

14. H. Poincaré, Oeuvres, 11 vol., Paris (Gauthier-Villars), 1916–1956.

15. H. F. Baker, Alternants and continuous groups, Proc. London Math. Soc., (2) 3 (1905), pp. 24–47.

16. F. Hausdorff, Die symbolische Exponentialformel in der Gruppentheorie, Leipziger Ber., 58 (1906), pp. 19–48.

17. A. Hurwitz, Über die Erzeugung der Invarianten durch Integration, Gött. Nachr. (1897), pp. 71–90 (= Math. Werke, vol. II, pp. 546–564).

18. E. E. Levi, Sulla struttura dei gruppi finiti e continui, Atti Acc. Sci. Torino, 40 (1905), pp. 551–565 (= Opere, vol. I, pp. 101–115).

19. K. Hensel, Über die arithmetischen Eigenschaften der Zahlen, Jahresber. der D.M.V., 16 (1907), pp. 299–319, 388–393, 474–496.

20. I. Schur, Neue Anwendungen der Integralrechnung auf Probleme der Invariantentheorie, Sitzungsber. Berlin, 1924, pp. 189–208, 297–321, 346–355.

21. H. Weyl, Theorie der Darstellung kontinuierlicher halb-einfacher Gruppen durch lineare Transformationen, I, Math. Zeitschr., 23, (1925), pp. 271–309; II, *ibid.*, **24** (1926), pp. 328–376; III, *ibid.*, **24** (1926), pp. 377–395 (= *Werke*, vol. II, pp. 543–647).

22. O. Schreier: (*a*) Abstrakte kontinuierliche Gruppen, *Abh. math. Sem. Hamburg*, **4** (1926), pp. 15–32; (*b*) Die Verwandschaft stetiger Gruppen in grossen, *ibid.*, **5** (1927), pp. 233–244.

23. J. Von Neumann, Zur Theorie der Darstellung kontinuierlicher Gruppen, *Sitzungsber. Berlin*, 1927, pp. 76–90 (= *Collected Works*, vol. I, pp. 134–148).

24. P. Hall, A contribution to the theory of groups of prime power order, *Proc. London Math. Soc.*, (3) **4** (1932), pp. 29–95.

25. W. Magnus: (*a*) Beziehungen zwischen Gruppen und Idealen in einem speziellen Ring, *Math. Ann.*, **111** (1935), pp. 259–280; (*b*) Über Beziehungen zwischen höheren Kommutatoren, *J. Crelle*, **177** (1937), pp. 105–115.

26. J. H. C. Whitehead: (*a*) On the decomposition of an infinitesimal group, *Proc. Camb. Phil. Soc.*, **32** (1936), pp. 229–237 (= *Mathematical Works*, I, pp. 281–289); (*b*) Certain equations in the algebra of a semi-simple infinitesimal group, *Quart. Journ. of Math.*, (2) **8** (1937), pp. 220–237 (= *Mathematical Works*, I, pp. 291–308).

27. I. Ado: (*a*) Note on the representation of finite continuous groups by means of linear substitutions (in Russian), *Bull. Phys. Math. Soc. Kazan*, **7** (1935), pp. 3–43; (*b*) The representation of Lie algebras by matrices (in Russian), *Uspehi Mat. Nauk*, **2** (1947), pp. 159–173 (English translation: *Amer. Math. Soc. Transl.*, (1) **9**, pp. 308–327).

28. N. Jacobson: (*a*) Rational methods in the theory of Lie algebras, *Ann. of Math.*, **36** (1935), pp. 875–881; (*b*) Classes of restricted Lie algebras of characteristic $p$, II, *Duke Math. Journal*, **10** (1943), pp. 107–121.

29. G. Birkhoff: (*a*) Continuous groups and linear spaces; *Rec. Math. Moscou*, **1** (1936), pp. 635–642; (*b*) Representability of Lie algebras and Lie groups by matrices, *Ann. of Math.*, **38** (1937), pp. 526–532.

30. E. Witt, Treue Darstellung Lieschen Ringe, *J. Crelle*, **177** (1937), pp. 152–160.

31. R. Brauer, Eine Bedingung für vollständige Reduzibilität von Darstellungen gewöhnlicher und infinitesimaler Gruppen, *Math. Zeitschr.*, **41** (1936), pp. 330–339.

32. H. Casimir-B. L. van der Waerden, Algebraischer Beweis der vollständigen Reduzibilität der Darstellungen halbeinfacher Liescher Gruppen, *Math. Ann.*, **111** (1935), pp. 1–12.

33. A. Weil, Sur les fonctions elliptiques $p$-adiques, *C. R. Acad. Sci.*, **203** (1935), p. 22.

34. E. Lutz, Sur l’équation $y^2 = x^3 - Ax - B$ dans les corps $p$-adiques, *J. Crelle*, **177** (1937), pp. 237–247.

35. C. Chabauty, Sur les points rationnels des courbes algébriques de genre supérieur à l’unité, *C. R. Acad. Sci.*, **212** (1941), pp. 882–884.

36. L. S. Pontrjagin, Topological groups, Princeton Univ. Press, 1939.
37. R. Hooke, Linear $p$-adic groups and their Lie algebras, Ann. of Math., **43** (1942), pp. 641–655.
38. C. Chevalley, Theory of Lie groups, Princeton Univ. Press, 1946.
39. E. Dynkin: (a) Evaluation of the coefficients of the Campbell–Hausdorff formula (in Russian), Dokl. Akad. Nauk, **57** (1947), pp. 323–326; (b) Normed Lie algebras and analytic groups (in Russian), Uspehi Mat. Nauk, **5** (1950), pp. 135–186 (English translation: Amer. Math. Soc. Transl., (1) **9**, pp. 470–534).
40. M. Hall, A basis for free Lie rings and higher commutators in free groups, Proc. Amer. Math. Soc., **1** (1950), pp. 575–581.
41. D. Montgomery-L. Zippin, Topological Transformation Groups, New York (Interscience), 1955.
42. M. Lazard: (a) Quelques calculs concernant la formule de Haudorff, Bull. Soc. Math. France, **91** (1963), pp. 435–451; (b) Groupes analytiques $p$-adiques, Publ. Math. I.H.E.S., no. 26 (1965), pp. 389–603.
