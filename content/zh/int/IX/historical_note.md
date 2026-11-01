---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: int-vii-ix
pdf_pages: 0302-0314
extraction: ocr
statements: 0
exercises: 0
content_sha256: c543d4d924c890da30ddf3cb16b6107c22b207e64b122e2a5910e3ab9355cc78
translated_from: content/en/int/IX/historical_note.md
translation_method: google
source_content_sha256: bdade34b7cba37740a59431245d21e998b2354e188820e734097d82be2331764
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 136bfdc375a93ffa6036eee05d0e5816decef08350c3a95aaeb181454ee7aea4
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（注：罗马数字指的是注末尾的参考书目。）

虽然对拓扑和测度论之间联系的研究可以追溯到现代实变量函数理论的开端，但直到最近，豪斯多夫拓扑空间的积分才以一般方式得到彻底解决。 之前设定在本综合之前的工作历史中，我们回顾了关系在拓扑和测量之间的思想演变的几个阶段。

对于勒贝格来说，这只是一个对一个或多个实变量积分函数的问题。 1913年，Radon定义了$\mathbf{R}^n$和相应的积分的一般测度；这一理论在第 1 章的书 (I) 中有详细阐述。 de la Vallée Poussin 并以恒定的方式依赖于欧氏空间的拓扑性质。稍后，在 1915 年，Fréchet 在 (II, a)) 中定义了配备部落的集合上的“抽象”测度，以及关于这些测度的积分；他指出，人们可以通过这种方式建立勒贝格理论的主要结果，而无需使用拓扑方法。他用以下字证明了他的承诺，摘自（II，b），第一个部分）的介绍：“Que par example dans l’espace à une infinité de coordonnées oùdiversities applications de l’Analyse avaient pipeline àvarious définitions non équivalentes d’une suite融合，替换 une de ces définitions par une autre, rien ne sera change dans les propriétés des familles et fonctionsadditions d’ensembles dans ces espaces ».(*) Fréchet 的调查由 Carathéodory 完成，他应于扩张获得重要的定理集合函数为一度量。萨克斯书的开头（III）给出了这个点观点的浓缩阐述。

局部紧致群 (cf.) 的 Haar 测度的发现

(*) “同时，对于例，在空间有无限多个坐标，其中数学分析的各种应用导致了收敛序列的各种不等价定义，如果替换其中一个定义乘以另一个，则族的属性不会发生任何改变，并且这些空间中的加性函数集合。”

第 3 章的历史注 VII和VIII）以及它立即收到的大量应用，然后是Weil和Gelfand关于调和数学分析的著作，导致了1940年左右对这种点观点的深刻修改：在这种问题中，最方便的做法是将测度视为连续函数的空间上的线性形式。这个方法迫使人们将自己限制在紧致或局部紧致空间，但这对于几乎所有的应用来说并不是一个不便：更好的是，J. Tate和A. Weil在$p$-adic 群和adèle 群上引入Harmonic 数学分析，已经允许了惊人的更新分析数理论。

正是从一个完全不同的方向，需要通过考虑非局部紧拓扑空间的措施来扩大这个点的视野：逐渐地，概率论导致了对这种空间的研究，并提供了许多非平凡的例。也许这些发展对测度论的影响迟缓的原因在于概率论的相对孤立，直到最近概率论仍然处于传统数学学科的边缘。

序列空间的措施

经典概率论最发达的分支之一是极限定理（大数的律，趋向高斯-拉普拉斯律，...）；这关系到统计规律性概念的​​深化，这一概念体现在大量人口发挥作用的现象中。这些问题的正确数学表述需要在序列空间上引入措施；这些空间构成了有限维空间中最明显的推广，是Fréchet、Lévy、Lusin等在1920年左右对“一般数学分析”进行调查的选择的主题。新概率论方法的创造者欣钦和柯尔莫戈洛夫都是卢辛的弟子，而Lévy很快就将自己定位于概率论问题：这些构成了新概率论方法的试金石，这也并非偶然。

对序列空间措施的第一个隐式干预出现在 E. 的著作中。 Borel 在 1909 年提出了可数概率 (IV)。 Borel 的一个高度原创的想法在于，将他刚刚获得的概率结果应用于 0 到 1 之间的几乎所有实数的小数展开所具有的属性证明。 This application rests on the following fundamental remark: let us define every real number between 0 and 1 by the sequence of figures (or 'digits') in its expansion in a given base $q$ ($q \geqslant 2$); if one successively draws at random the various figures of a number $x$, independently of each other and with equal probability $1/q$ for $0, 1, \ldots, q - 1$, the probability that $x$ lies in an interval of $[0, 1[$ is equal to the length of that interval.

1923年，Steinhaus（V）严格建立了这些结果，并描述了Borel考虑的无限序列随机绘图的精确数学模型：为简单起见，我们取$q = 2$并用两个元素$\{0, 1\}$表示为I集合；一个为I配备由$\mu(0) = \mu(1) = \frac{1}{2}$定义的度量$\mu$； 乘积空间 $I^{\mathbf{N}}$ 的元素数的序列 $\varepsilon = (\varepsilon(n))_{n \in \mathbf{N}}$ 等于 0 或 1，映射 $\varphi : \varepsilon \mapsto \sum_{n \geq 0} \varepsilon(n) \cdot 2^{-n-1}$ 最多可数集合、双射 $I^{\mathbf{N}}$ 进入区间 $[0, 1]$；此外，$\varphi^{-1}$变换将$[0, 1]$上的勒贝格测度放入$I^{\mathbf{N}}$上的测度P中，即每个因子上的$\mu$测度的乘积。事实上，斯坦豪斯并没有可用的构造来应对乘积的措施；他利用准双射$\varphi$到构造的存在性，从$[0, 1]$上的勒贝格测度开始，在$I^{\mathbf{N}}$上测度P，然后给出P的公理化刻画。这样得到的同构使得将概率语言翻译成测度语言成为可能，并应用已知的概率语言。勒贝格积分上的定理。

在同一工作中，斯坦豪斯考虑了随机级数$\sum_{n \geq 0} \sigma_n \cdot a_n$，其中符号$\sigma_n = \pm 1$是彼此独立且以相等的概率$\frac{1}{2}$随机选择的； 1928 年至 1935 年间，他研究了许多其他随机级数。从他们的角度来看，Paley、Wiener 和 Zygmund 考虑了形式 $\sum_{n = -\infty}^{\infty} a_n \exp(2\pi i(nt + \Phi_n))$ 的随机傅里叶级数$^{(1)}$； “振幅”$a_n$是固定的，“相位”$\Phi_n$是均匀分布在$[0, 1]$上的独立随机变量。虽然从问题到另一个之一的分析难度有很大差异，但测度论在项中的翻译在所有情况下都是相同的，并且代表了Borel和Steinhaus处理的情况的扩张；这是在 $\mathbf{R}^{\mathbf{N}}$ 上构建一个测度，即乘积的一系列测度，与质量 1 的 $\mathbf{R}$ 上的同一个正测度 $\mu$ 相同；对于例，前面的随机傅里叶级数对应对于$\mu$是$[0, 1]$上的勒贝格测度的情况。

对于构造这样的乘积措施，可以使用两个方法。第一个是直接方法，由 Daniell (VI, a)) 在 1918 年首次精确曝光； 1934年，Jessen（VII）重新发现了$\mu$是$[0, 1]$的勒贝格测度。第二个方法是寻求类似于斯坦豪斯对约化到勒贝格测量$[0, 1]$的技巧；这种方式的优点是方便

(1) 关于随机傅立叶级数的说明，请参阅 J. P. KAHANE 在 Séminaire Bourbaki 中的阐述（No. 200，第 12 年，1959/60，本杰明，纽约）。

只要人们没有对一般测度论进行完整的阐述，因为它允许使用勒贝格的定理而不需要新的证明。(2)

布朗运动理论

该理论在当代科学发展中占据着特殊的地位，它见证了物理问题和“纯”数学之间不断而丰富的交流。植物学家布朗于 1829 年发现的布朗运动研究，在 19 世纪被众多物理学家集中进行，(3)，但第一个令人满意的数学模型直到 1905 年才由爱因斯坦发明。在粒子沿直线运动的简单情况下，爱因斯坦的基本假设可以表述如下：如果 $x(t)$ 是粒子在 $t$ 时刻的横坐标，并且如果$t_0 < t_1 < \cdots < t_{n-1} < t_n$，则连续位移$x(t_i) - x(t_{i-1})$（对于$1 \leq i \leq n$）是独立的高斯随机变量。本文不详细介绍 J. Perrin 激发爱因斯坦理论的重要实验工作。出于我们的目的，我们只需要保留佩兰的注，根据该理论，对布朗运动轨迹的观察不可避免地向他暗示了“数学家的函数无导数”。这个注是维纳最初的火花。

另一个当前的思想起源于气体动力学理论，由玻尔兹曼和吉布斯在 1870 年至 1900 年间发展。考虑在（绝对）温度 T 下由质量为 $m$ 的 N 个分子形成的气体，并用 $\mathbf{v}_1, \ldots, \mathbf{v}_N$ 表示气体中 N 个分子的速度； 系统的动能等于

$$
\frac{m}{2} (\mathbf{v}_1^2 + \cdots + \mathbf{v}_N^2) = 3NkT,
$$

其中 $k$ 是玻尔兹曼常数。根据吉布斯的思想，分子间的大量激波不允许精确确定分子的速度，因此可以方便地在由方程（1）定义的空间维数 3N 的球体S 上引入概率律 $P$。 “微观规范”假设在于假设

(2) 维纳还多次注意（cf.代表例（XI），第IX章）证明布朗运动的测度与$[0,1]$上的勒贝格测度同构。这种技巧的可能性在冯·诺依曼的一般定理中找到了解释，它给出了与$[0,1]$上的勒贝格测度同构的测度公理刻画。

(3) E. Nelson 最近出版的著作《布朗运动的动力学理论》，数学注，普林斯顿，1967 年对这段历史进行了非常生动的描述。

P 是质量为 1 在旋转下不变的球体 S 上的测量。 此外，麦克斯韦速度的律表明分子速度分量的概率律是方差为 $2kT/m$ (§ 6, No. 5, *注 3*) 的高斯测度。 Borel似乎是在1914年第一个观察到麦克斯韦的律是吉布斯假设的推论以及当分子的数非常大时球体的性质。 他认为在大维数的欧氏空间中的球体S以及质量1在S上的测量P在旋转下是不变的；使用基于斯特林公式的经典近似方法，他证明了P在坐标轴上的投影近似为高斯分布。 随后，Gâteaux 和 Lévy (IX, *a*) 对这些结果进行了锐化。 给定整数$m \geqslant 1$和数$r > 0$，用形式$(x_1, \ldots, x_m, 0, 0, \ldots)$序列和$x_1^2 + \cdots + x_m^2 = r^2$表示$S_{m,r}$集合；另外，用 $\sigma_{m,r}$ 表示旋转下 $S_{m,r}$ 上质量为 1 的测量不变性。 用现代语言表述，Gâteaux 和Lévy 的结果如下：$\sigma_{m,1}$ 的序列紧密趋向于原点$(0, 0, \ldots)$ 处的单位质量，$\sigma_{m, \sqrt{m}}$ 的序列紧密地趋向于形式的$\Gamma$ 测度

$$
d\Gamma(x_1, x_2, \ldots) = \prod_{n=1}^\infty d\gamma(x_n)
$$

（$\gamma$ 是$\mathbf{R}$ 的高斯测度，方差为 1）。

前面的测度$\Gamma$在无限维数中扮演了高斯测度的角色。 It seems indeed that Lévy had confusedly hoped to define in an intrinsic manner a Gaussian measure on every infinite-dimensional Hilbert space. 事实上，正如Lévy和Wiener所示，测度$\Gamma$在某种意义上是不变的$^{(4)}$在$l^2$的自同构下；不幸的是，平方可和的序列$(x_1, x_2, \ldots, x_n, \ldots)$的集合$l^2$对于$\Gamma$的测度为零。 现在已知，人们必须满足于在无限维希尔伯特空间.$^{(5)}$上有一个高斯*promesure*

We owe to Wiener the essential progress: if one does not have a reasonable Gaussian measure on an infinite-dimensional Hilbert space, one can construct by the operation of primitive a measure $w$ on a space of continuous functions starting from a Gaussian promeasure (cf. §6, No. 7, Th. 1 for the details). 我们将简洁地解释维纳原始的$w$（X）的构造；它直接受到 Gâteaux 的关系 $\Gamma = \lim_{m \to \infty} \sigma_{m, \sqrt{m}}$ 和 Lévy 的影响。 对于每个整数$m \geqslant 1$，用$T = ]0, 1]$上函数的$H_m$集合表示，在每个间隔$\left[ \frac{k-1}{m}, \frac{k}{m} \right]$（对于$k = 1, 2, \ldots, m$）上是恒定的，并用$\pi_m$表示质量1的测量，在旋转下不变，在欧氏上半径为 1 in $\mathbf{R}^m$ 的球体。 令$f_m$为$H_m$的同构到关联的$\mathbf{R}^m$，对于在区间$\left[ \frac{k-1}{m}, \frac{k}{m} \right]$、向量$(a_1, a_2 - a_1, \ldots, a_m - a_{m-1})$上取值$a_k$的每个函数 (从而项) “微分空间”维纳亲爱的）；用$w_m$表示$H_m$上的度量，即$f_m^{-1}$下$\pi_m$的像。 维纳将所需测度$w$定义为测度$w_m$中的极限。 准确地说，让我们用$T$上调节的函数的$H$集合来表示，拓扑一致收敛（对于每个整数$m \geqslant 1$，我们有$H_m \subset H$）；对于$H$上的每个有界均匀连续函数$F$，存在极限$A\{F\} = \lim_{m \to \infty} \int_{H_m} F(x) \, dw_m(x)$；接下来，维纳通过正面或反面游戏波动的微妙数学分析获得了一定的上界，并再次采用丹尼尔强调的紧凑性论证，他表明对于应用丹尼尔的扩张定理，一个低于条件。 一个结论存在由$\mathscr{C}(T)$携带的测度$w$并且使得$A\{F\} = \int_{\mathscr{C}(T)} F(x) \, dw(x)$。 然后，维纳能够证明爱因斯坦假设的测量$w$对应，（6）和他的估计使他能够在函数上对佩兰的注给出精确的含义，而无需导数：函数满足的集合a Lipschitz条件阶$\frac{1}{2}$对于$w$可以忽略不计（但是，对于每个$a$和$0 < a < \frac{1}{2}$，几乎每个函数都满足阶$a$的Lipschitz条件）。

(4) 更准确地说，有以下结果。令$U$为希尔伯特空间$l^2$的自同构，以及$U$的$(u_{mn})$矩阵。令E为所有实数序列$(x_n)_{n \geqslant 1}$的向量空间和由序列$(x_n)_{n \geqslant 1}$形成的E的F子空间，其中级数$\sum_{n \geqslant 1} u_{mn} x_n$对于每个$m \geqslant 1$收敛。将F的公式$(\widetilde{U}x)_m = \sum_{n \geqslant 1} u_{mn} x_n$定义线性映射$\widetilde{U}$转化为E，$\Gamma$的度量集中在F上，以及$\widetilde{U}(\Gamma) = \Gamma$。

(5) 这个概念是由I以“弱正则分布”的名义引入的。 E. Segal（*Trans. Amer. Math. Soc.* **88** (1958), 12–42）。其中之一归功于这位作者对高斯测度的详细研究，以及它们在域量子理论中某些问题的应用。
} 构造通过原语的运算测量$w$ 在连续函数的空间上，从高斯测度开始（cf. §6, No. 7，详细信息请参见Th.1）。我们将简洁地解释维纳原始的$w$（X）的构造；它直接受到 Gâteaux 的关系 $\Gamma = \lim_{m \to \infty} \sigma_{m, \sqrt{m}}$ 和 Lévy 的影响。对于每个整数$m \geqslant 1$，用$T = ]0, 1]$上函数的$H_m$集合表示，在每个间隔$\left[ \frac{k-1}{m}, \frac{k}{m} \right]$（对于$k = 1, 2, \ldots, m$）上是恒定的，并用$\pi_m$表示质量1的测量，在旋转下不变， $\mathbf{R}^m$ 中半径为 1 的欧氏球体。令$f_m$为$H_m$到$\mathbf{R}^m$的同构，对每个函数在区间$\left[ \frac{k-1}{m}, \frac{k}{m} \right]$、向量$(a_1, a_2 - a_1, \ldots, a_m - a_{m-1})$(从而)取值$a_k$维纳亲爱的项“微分空间”）；用$w_m$表示$H_m$上的度量，即$f_m^{-1}$下$\pi_m$的像。维纳将所需测度$w$定义为测度$w_m$中的极限。准确地说，让我们用$T$上调节的函数的$H$集合来表示，拓扑一致收敛（对于每个整数$m \geqslant 1$，我们有$H_m \subset H$）；对于$H$上的每个有界均匀连续函数$F$，存在极限$A\{F\} = \lim_{m \to \infty} \int_{H_m} F(x) \, dw_m(x)$；接下来，维纳通过正面或反面游戏波动的微妙数学分析获得了一定的上界，并再次采用丹尼尔强调的紧凑性论证，他表明对于应用丹尼尔的扩张定理来说，一个人低于条件。其中一个结论存在由$\mathscr{C}(T)$携带的测度$w$，并且使得$A\{F\} = \int_{\mathscr{C}(T)} F(x) \, dw(x)$。然后，维纳能够证明，对爱因斯坦假设的测量$w$对应，(6) 和他的估计使他能够在没有导数的情况下对佩兰的注在函数上给出精确的含义：函数满足利普希茨的集合阶 $\frac{1}{2}$的条件对于$w$来说可以忽略不计（但是，对于每个$a$和$0 < a < \frac{1}{2}$，几乎每个函数都满足阶的Lipschitz条件 $a$）。

如今，已知有许多构造维纳测度。因此，佩利和维纳使用随机傅里叶级数（XI，Ch.IX）：对于每个实数

(6) 这可以由公式翻译
$$
\int_{\mathscr{C}(T)} f(x(t_1), \ldots, x(t_n)) \, dw(x) =
(2\pi)^{-n/2} \prod_{i=1}^n (t_i - t_{i-1})^{-1/2} \int \cdots \int f(x_1, \ldots, x_n) \exp \left( -\frac{1}{2} \sum_{i=1}^n \frac{(x_i - x_{i-1})^2}{t_i - t_{i-1}} \right) dx_1 \cdots dx_n,
$$
其中$f$是$\mathbf{R}^n$上的任意有界连续函数，其中$0 = t_0 < t_1 < \cdots < t_n \leqslant 1$（约定为$x_0 = 0$）。维纳接受了哈代的严格分析训练，并且对当时概率论的基础抱有合理的怀疑，因此小心翼翼地不使用概率术语或结果。由此可见，他的回忆录充满了强大的公式，前述只是其中的一个例子；这种情况是延迟维纳思想传播的因子之一。

序列$\mathbf{a} = (a_n)_{n \geq 1}$以及每一个整数$m \geq 0$，让我们在$]0,1]$定义函数$f_{m,\mathbf{a}}$

$$
f_{m,\mathbf{a}}(t) = a_1 t + 2 \sum_{k=2}^{2^{m+1}} \frac{1}{\pi k} a_{k-1} \sin \pi kt;
$$

可以证明，对于$\Gamma$，函数$f_{m,\mathbf{a}}$的几乎每一个序列$\mathbf{a}$、序列都趋向于连续的函数$f_\mathbf{a}$，并且$w$是像 $\Gamma$低于映射（几乎到处都有定义）$\mathbf{a} \mapsto f_\mathbf{a}$。后来，Lévy 屈服于 (IX, b), c)) 构造，非常接近我们在 §6, No. 7 中曝光的内容。最后，Kac、Donsker 和 Erdös 在 1950 年左右展示了如何通过更通用的度量来实现维纳原始构造中$\mathbf{R}^m$ 上的替换球形度量$\pi_m$。他们的结果在维纳测度和概率论的极限定理之间建立了牢固的联系；它们将由普罗霍罗夫（XIII）完成并系统化，我们将在稍后返回。

这里不是分析维纳的发现所带来的众多重要的概率论著作的地方；如今，布朗运动仅作为马尔可夫过程中最重要的例之一出现。我们只提及 Kac 对某些抛物型偏微分方程的解应用维纳测度；这是一个在量子域理论中采用费曼思想的问题——然而数学和物理问题相互影响的另一个例。

逆极限措施

这是主要为了适应概率论的需要而发展起来的理论。当知道序列的律$P_X$时，关于随机变量$X_1, \ldots, X_n$的有限序列的问题在原理中求解：这是对质量1的$\mathbf{R}^n$的正测量，使得同时获得不等式$a_1 \leq X_1 \leq b_1, \ldots, a_n \leq X_n \leq b_n$的概率等于$P_X(C)$，其中$C$是$\mathbf{R}^n$中封闭的盒子$[a_1, b_1] \times \cdots \times [a_n, b_n]$。实际上，相对于勒贝格测度，$P_X$要么具有离散支持，要么承认密度。当处理无限序列$(X_n)_{n \geq 1}$随机变量时，通常知道每个整数$n \geq 1$的部分序列$(X_1, \ldots, X_n)$的律$P_n$；这些数据满足兼容性条件，表示序列$(P_n)_{n \geq 1}$是逆系（或“投影系统”）的度量。直到大约 1920 年，与无限序列相关的事件概率或多或少都是通过从有限情况的概率到极限的“自然”过渡以隐含的方式定义的；因此，我们假设游戏终止的概率为极限，因为 $n$ 趋于无穷大，游戏最多在 $n$ 步中终止的概率。当然，这样的理论不是很连贯，而且不排除“悖论”的存在，即当一个人通过两个程序中的一个或另一个进行评估时，收到两个不同估计的概率相同，每个程序都与另一个程序一样“自然”。

斯坦豪斯（V）似乎是第一个感到需要考虑（对于正面或反面游戏）的人，不仅需要考虑逆系$(P_n)_{n \geq 1}$，而且还需要考虑极限。稍早一点，即 1919 年，丹尼尔（VI，$b$）已经普遍证明了这样的逆极限，$^{(7)}$的存在，但这个结果在欧洲似乎仍然未知。 1933 年，柯尔莫戈洛夫在其著作 (XII) 中重新发现了它，作者在其中阐述了概率论的公理化概念。 Daniell 和 Kolmogoroff 的证明使用了紧性论证，这与我们在 Th 中使用的基本相同。 §4, No. 3 中的 2 个，位于 Dini 的定理上。

Daniell-Kolmogoroff 定理对于随机序列 $(X_n)_{n \geq 1}$ 的情况没有留下任何不足之处，但是 Kolmogoroff、Feller 和 Doob 自 1935 年起对随机函数的研究却存在相当另一个阶的困难。考虑例的间隔$T$为$\mathbf{R}$，代表“随机过程”观察时刻的集合；可能轨迹中的集合为乘积空间$\mathbf{R}^T$，视为部分积$\mathbf{R}^H$的逆极限，其中$H$超过$T$的有限子集的集合；通常假设给定逆系措施$(\mu_H)$ (cf. §4, No. 2)。 Kolmogoroff 的定理确实产生了 $\mathbf{R}^T$ 的测度，但它是在比 Borel 部落小得多的部落上定义的。$^{(8)}$ Kolmogoroff 的构造的一个变体，产生了拓扑空间上的测度，由 Kakutani 提出（*Proc. Imp. Acad. Tokyo* 19） (1943), 184–188)，此后多次被重新发现：人们将$\mu_H$视为$\mathbf{R}^H$对$\overline{\mathbf{R}}^H$的测度；$^{(9)}$紧致空间$E = \overline{\mathbf{R}}^T$是有限乘积的逆极限 $\overline{\mathbf{R}}^H$，并且可以在$E$上定义测量$\mu$作为$\mu_H$的逆极限（cf.章节III, §4, No. 5）。然而，这个过程有一个严重的不便； $\overline{\mathbf{R}}^T$的元素不具备规律性性质，无法推进过程的概率研究，甚至可以简单地消除由$\mathbf{R}$的紧致化$\overline{\mathbf{R}}$引入的寄生值$\pm \infty$。这可以通过在特定的子空间上引入$\overline{\mathbf{R}}^T$的测量$\mu$来补救（在布朗运动的情况下为例$\mathscr{C}(T)$）；根本的困难在于，函数空间，即使是常见的型之一，也不一定能在$\overline{\mathbf{R}}^T$中测量$\mu$，甚至函数空间的选择也可能是有问题的。$^{(10)}$

(7) Daniell 处理了$\mathbf{R}$紧致区间乘积$\prod_{n \geq 1} I_n$的测度情况，但他的方法扩展立即处理了空间紧致区间乘积的情况；这本质上是我们在第 1 章中使用的方法。 III, §4, No. 5。

(8) 柯尔莫哥洛夫测度仅针对形式$A \times \mathbf{R}^{T-D}$的$\mathbf{R}^T$中的Borel集合定义，其中$D$是$T$的可数子集，$A$是$\mathbf{R}^D$的Borel子集；因此，对于任意乘积 $\mathbf{R}^T$，柯尔莫戈洛夫的定理是可数乘积情况下的直接的推论。

(9) 可以将替换 $\overline{\mathbf{R}}$ 乘以任何紧致空间包含 $\mathbf{R}$ 作为稠密子空间。
消除由 $\mathbf{R}$ 的紧致化 $\overline{\mathbf{R}}$ 引入的寄生值 $\pm \infty$。这可以通过在特定的子空间上引入$\overline{\mathbf{R}}^T$的测量$\mu$来补救（对于布朗运动的情况下为例$\mathscr{C}(T)$）；根本的困难在于，函数空间，即使是常见的型之一，也不一定能在$\overline{\mathbf{R}}^T$中测量$\mu$，甚至函数空间的选择也可能是有问题的。$^{(10)}$

1956 年，普罗霍罗夫在其著作 (XIII) 中迈出了决定性的一步，该著作对随机过程理论产生了决定性的影响。 By putting into a suitable axiomatic form the methods used by Wiener in the article analyzed above, he established a general existence theorem for inverse limits of measures on function spaces that is a special case of Th. 1 of §4, No. 2 corresponding to Polish spaces.

1947 年，Bochner (XIV) 引入了更严格的类逆系；它们是由有限维实数向量空间和满射线性映射形成的逆系。这样的系统的逆极限可以以自然的方式与实向量空间$E$的代数对偶$E^*$识别，配备弱拓扑$\sigma(E^*, E)$； 相应的逆系的措施有极限，这是在比$E^*$的Borel部落小得多的部落上定义的措施$\mu$。博赫纳通过其傅里叶变换完全描述了此类“promeasures”，即$E$上的函数。但在$E$上缺少拓扑的情况下，这个结果几乎没有用处，在这种情况下，我们必须检验将$\mu$视为$E$的拓扑对偶$E'$的测度的可能性。 R. Fortet 和 E. Mourier 以独立的方式，在寻求将 Banach 空间中的值概率论的某些经典结果（大数的律，中心极限定理）推广到随机变量的同时，也证明了傅里叶变换在此类问题中所发挥的基础作用。但直到 1956 年 Gelfand (XV, b)) 才取得实质性进展，提出傅里叶变换的自然设定不是巴纳赫空间或希尔伯特空间，而是核弗雷谢空间。他推测，在这样的空间上，正型的每一个连续函数都是其对偶测度的傅里叶变换，这一结果很快由 Minlos (XVI) 确立。它的重要性首先源于它适用于分布的空间，并且函数空间的准总体是空间分布的Borel子集（因此构成了比$\mathbf{R}^T$更好的容器）。$^{(11)}$随机理论分布是一个完整的展开区域，我们应该满足于引用

(10) 关于普罗霍洛夫之前使用的函数、空间、方法的构建措施问题的详细讨论，参见J.L。杜布，公牛。阿米尔。数学。苏克。 53（1947），15-30。
(11)可查阅X的说明。费尼克，安。研究所。 Fourier 17 (1967), 1–92，其中还有包含大量关于紧收敛的结果。

Gelfand 和 Vilenkin 的书的读者 (XVII)。

刚才提到的逆极限的结果利用了基空间上拓扑的存在性。人们可能会问，在“抽象”措施的情况下是否存在类似的理论。冯·诺依曼于 1935 年证明了在所有情况下都存在乘积测度，但是 Jessen 和 Andersen 发现的反例 (XVIII) 破灭了每个逆系测度都承认极限的希望。已发现两种缓解方法：1949 年，C。约内斯库-图尔恰通过适当崩解的存在性，确立了可数逆极限的存在性，(12) 对于马尔可夫过程的研究来说，这是一个非常有趣的结果；此外，据观察，空间的拓扑仅通过紧凑子集的集合中介进行干预。因此，很自然地尝试通过类 of 子集 of 集合的紧凑概念，在抽象理论中公理化这种情况。这项工作是由Marczewski（他通过这种方式建立了摘要逆极限定理）和Ryll-Nardzewski（他处理了措施的瓦解）于1953年完成的。(13)

一般拓扑空间和紧收敛的措施

对拓扑和测度论之间联系的研究首先被认为是对测度的正则性性质的研究，特别是“外”正则性和“内部”正则性的研究；(14) 内部正则性等价于局部紧致无穷大可数空间上的外正则性。勒贝格给出的对线的子集的度量的构造突出了这两种规律性，而波兰空间的度量的外部规律性性质似乎在1935年左右就已经声名狼藉。但直到1940年，A. D. Alexandroff在一篇文章中才指出，该文章的传播因战争而受阻。 (XIX)突出了内部正则性的作用，并表明波兰空间的测度具有它；这个结果后来被 Prokhorov (XIII) 重新发现，并且经常被错误地归因于该作者。直到最近才意识到这个性质扩展到苏斯林空间；正因为如此，

(12)“抽象”措施理论的极限的标志似乎是缺乏令人满意的解体理论。这种困难在与条件概率相关的概率论中以持续的方式再次出现。
(13) 对于这一理论的阐述，可以参考 J. PFANZAGL 和 W. PIERLO, Lecture 注 in Mathematics (Springer–Verlag), Vol. 11。 16（1966）。
(14) 如果每个 Borel 集合的测度是开集合包含的测度的下确界，则 Hausdorff 拓扑空间的 Borel 族上的“抽象”测度 $\mu$ 被称为外正则；如果每个 Borel 集合的度量是其紧凑子集的度量的至高，则称度量 $\mu$ 是内部正则。

这些空间的重要性已大大增加，甚至更重要的是，人们认识到他们的理论可以在没有任何可计量性假设的情况下得出，并且函数空间的准总体是苏斯林（最常见的是，甚至是卢辛）。(15) 这些是促使我们在这方面把重点放在内部常规措施上的原因。 章。

通过将测度的空间与连续函数的空间放入对偶性，可以最方便地实现测度收敛模式的定义。 概括 F 的旧结果。 里斯，A. 一个。 马尔科夫于 1938 年在 $\mathscr{C}(X)$ 上的正泛函与紧凑空间 X 上的常规测度之间建立了一对一的对应。 在已经引用的著作 (XIX) 中，A. D . Alexandroff 扩展将这些结果应用于完全正则空间的情况：他在完全正则空间X上的有界连续函数的空间$\mathscr{C}^b(X)$上引入了正线性形式的集合中的层次结构，（16）他定义紧密收敛有界措施并证明以下两个定理：

a) 如果X是波兰语，$\mathscr{C}^b(X)$相应的上的线性形式对测度的集合由于序列弱收敛而关闭；
b) 如果有界测度的序列具有紧极限，则“无穷大处没有质量逃逸”（这是紧收敛上普罗霍罗夫的定理的逆命题的弱形式）。

从这些丰富的概念和定理中，普罗霍罗夫能够提取对随机过程理论重要的结果，并以简单而引人注目的形式的形式呈现它们。在他 1956 年的伟大著作（XIII）中，大量的部分致力于波兰空间的有界积极措施；推广Lévy的构造，他定义是质量1的正测量的集合的度量，使其成为波兰空间，然后建立紧收敛的重要紧致性准则（cf.§5, No. 5，Th.1）。独立于 Prokhorov，Le Cam (XX) 获得了数的紧致结果，以实现措施的紧密收敛；他认为，在空间上，他没有进行可度量化假设，并且在局部紧凑的情况下，他的结果约化是 Dieudonné 早期的定理。

(15) 为了尝试解决某些概率困难（特别是随机独立或依赖的各种概念之间的关系），数作者引入了受限制的类“抽象”度量：柯尔莫戈洛夫-格内登科的“完美”空间，Kolmogoroff-Gnedenko的“Lusin”空间布莱克威尔，罗克林的“勒贝格”空间。事实上（至少假设可数性相当弱假设），所有这些定义都给出刻画“抽象”测度，与Souslin空间上的有界正测度同构。关于这一主题，人们可以查阅脚注（13）中引用的著作。

(16) 他通过递减阶的通用性区分了$\sigma$-措施（XBorel部落的“抽象”措施）、$\tau$-措施（外部常规措施）和拉紧措施（内部常规措施）。当X是波兰语时，这三个概念重合。 术语本身归功于 McShane 和 Le Cam (XX)。人们可以在V中找到对这种分类产生的作品的描述。 S. VARADARAJAN（美国数学学会翻译 (2), 48, 161–228）。

(I) 第 3 章de la Vallée Poussin，Intégrales de Lebesgue，Fonctions d’ensembles，类 de Baire，巴黎（Gauthier-Villars），第一。编辑，1916；第二。编辑，1936 年。

(II) M. Fréchet：a) Sur l’intégrale d’une fonctionnelle étendue à un ensemble Abstrait，Bull。苏克。数学。法国，43 (1915)，第 248–265 页； b) Les familles et functionadditionsd’ensemblesabstraits，基金。 《数学》，4 (1923)，第 329–365 页；同上。 5 (1924)，第 206-251 页。

(III) S. Saks，积分理论，第二。编辑，纽约（Stechert），1937 年。

(IV) E. Borel，Les probabilités dénombrables et leurs applications arithmétiques，Rend。循环。数学。巴勒莫，27 (1909)，第 247–271 页。

(V) H. Steinhaus，Les probabilités dénombrables et leur rapport à la théorie de la mesure，基金。 《数学》，4 (1923)，第 286–310 页。

(VI) P. J. Daniell：a) 维数的无限数中的积分，Ann。数学，20 (1918–19)，第 281–288 页； b) 维数的无限数中的有限变化函数，同上。 21 (1919–20)，第 30–38 页。

(VII) B. Jessen，维数的无限数的空间积分理论，数学学报，63 (1934)，第 249–323 页。

(VIII) A. 爱因斯坦，《布朗运动理论研究》，纽约（多佛），1956 年。

(IX) P. LÉVY: a) Leçons d’Analyse Fonctionnelle，巴黎 (Gauthier-Villars)，1922 年（第二版于 1951 年由同一出版商出版，标题为 Problèmes concrets d’Analyse Fonctionnelle）； b) Processus stochastiques et mouvement Brownien，巴黎（Gauthier-Villars），1948 年； c) 布朗尼运动，记忆。科学。数学，126（1954）。

(X)N.维纳，微分空间，J.数学。物理。麻省理工学院，2 (1923)，第 131–174 页（= Selecta，第 55–98 页，剑桥（麻省理工学院出版社），1964 年）。

(XI)R.E.A.C。 PALEY 和 N. WIENER，复杂域中的傅里叶变换，Amer。数学。苏克。座谈会。出版。 No. 19，纽约，1934 年。

(XII) A. N. KOLMOGOROFF，Grundbegriffe der Wahrscheinlichkeitsrechnung，柏林（施普林格），1933 年。

(XIII)朱。 V。 PROKHOROV，随机过程的收敛性和概率论中的极限定理，理论。概率应用，1 (1956)，第 156–214 页。

(XIV) S. BOCHNER，谐波数学分析和概率论，伯克利（加州大学出版社），1960 年。

(XV)I。 M. GELFAND：a) 广义随机过程（俄语），Dokl。阿卡德。 Nauk SSSR，100 (1955)，第 853–856 页； b) 功能性数学分析的一些问题（俄语），Uspehi Mat。 Nauk，11 (1956)，第 3–12 页（= Amer. Math. Soc. Transl. (2), 16 (1960)，第 315–324 页）。

(XVI) R. A. MINLOS，广义随机过程及其扩张度量（俄语），Trudy Moskov。数学。 Obšč., 8 (1959)，第 497–518 页（= 数理统计和概率翻译精选，III (19)，第 291–313 页）。

(XVII)I。 M. GELFAND 和 N. Ya。 VILENKIN，广义函数，卷。 IV，纽约（学术出版社），1964（英文译本）。

(XVIII) E. SPARRE-ANDERSSON 和 B. JESSEN，关于无限乘积集合中措施的引入，丹麦。视频。塞尔布斯卡布。垫。费斯。 Medd.，25 (1948)，No. 4，第 1–7 页。

(XIX) A. D. ALEXANDROFF，加法集合函数摘要空间。 I（第 1 章），马太福音。 Sbornik，8 (1940)，第 307–348 页； II（第 2 章和第 3 章），同上，9 (1941)，第 563–628 页； III（第 4 至 6 章），同上，13 (1943)，第 169–238 页。

(XX)L。 LE CAM，随机过程分布的收敛性，大学。卡尔。出版。统计，No. 11 (1957)，第 207–236 页。
