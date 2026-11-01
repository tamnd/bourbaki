---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: lie-iv-vi
pdf_pages: 0262-0270
extraction: ocr
statements: 0
exercises: 0
content_sha256: f014dd2d86cd644d2074c093e2e7492e98e1e938b6c371735d7220d02ede7ce7
translated_from: content/en/lie/VI/historical_note.md
translation_method: google
source_content_sha256: e623ff32c0c52d1434bd8f2b6d72cf7351f86f08cf0e2118f761f5553e4aa916
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7f01f0e2c6c66fb2c110ea2db6a38d7259b7fde77b59083953f27df8f373d114
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

(章IV、V和VI)

（注意 - 括号中的罗马数字指的是注末尾的参考书目。）

The groups considered in these chapters appeared in connection with various questions of Geometry, Analysis and the Theory of Lie groups, sometimes in the form of permutation groups and sometimes in the form of groups of displacements in euclidean or hyperbolic geometry, and these various points of view have been unified only recently.

该理论的历史根远早于群概念的引入：事实上，它们存在于几何图形的“规则性”或“对称性”的研究中，特别是在正多边形和多面体的确定中（这当然可以追溯到毕达哥拉斯学派），这是欧几里得元素的最高成就，也是最令人钦佩的创造之一希腊天才的。后来，特别是中世纪盛期的阿拉伯作家，以及开普勒，出现了由（不一定是规则的）全等多边形规则“平铺”平面或球体的数学理论的开端。这无疑与古代和阿拉伯文明所设计的各种型装饰有关（可以适当地认为是这些文明所发展的数学的正宗部分（XII））。

1830-1840年左右，晶体学研究（Hessel、Bravais、Möbius）导致了对问题的考虑，这实际上是确定3维数的欧氏空间中位移的有限群，尽管上面引用的作者尚未使用群理论的语言；直到大约 1860 年才真正投入使用，正是在群分类的背景下，约旦于 1869 年（VI），确定 $\mathbf{R}^3$ 的保持方向位移的离散群（更一般地，群的闭子群保持方向的位移）。

直到 19 世纪末，这一思想流向多个方向发展。其中最重要的进展如下：

1. 继续有限群理论中很早就出现的趋势，寻求生成元和关系的简单型位移的有限群的“表示”。因此，汉密尔顿在 1856 年（V）证明，欧氏空间 $\mathbf{R}^3$ 的旋转的有限群由两个生成元 S、T 满足关系 $S^p = T^q = (ST)^3 = 1$ 生成，对于适当的值 $p$和$q$。

2. 离散的群位移可能会也可能不会包含反射。 1852 年，莫比乌斯本质上是球面几何中*由反射生成的位移的确定有限群（这相当于 $\mathbf{R}^3$ 的欧氏位移的有限群的相同问题）：他发现，除了循环群之外，这样群以一个边长为形式 $\pi/p, \pi/q, \pi/r$ 的球面三角形作为基本域，其中 $p, q, r$ 是三个整数 $> 1$，使得 $\frac{1}{p} + \frac{1}{q} + \frac{1}{r} > 1$ (III) (cf. 第 V. § 4，练习4）。他还注意到这些群包含所有有限群的位移都是子群。

3. 继黎曼和施瓦茨关于超几何函数和共形表示的工作之后，当开始研究以圆弧为界的复平面或半平面的“平铺”时，后者的发展扩展到了一个新领域：克莱因和庞加莱将其作为“自同构函数”理论的基础，并在其中认识到（对于与固定直线正交的圆弧）问题相当于确定非欧双曲平面（用“庞加莱半平面”标识）（X）位移的离散群。

4. 正多面体的概念和这种多面体对$\mathbf{R}^3$的平铺，被Schlafli扩展到所有欧氏空间$\mathbf{R}^n$，其工作可以追溯到大约1850年，但直到很晚才发表，并且很长一段时间被忽视（IV）；他确定完全是每个 $\mathbf{R}^n$、群位移中的规则“多胞形”，使这样的多胞形保持不变，并且该群的基本域，如莫比乌斯研究的 $n = 3$ 情况，是一个“室”，其投影在球体 $S_{n-1}$ 上是球形单纯形。然而，他并没有考虑确定$\mathbf{R}^n$中反射产生的位移的有限群的逆问题；这个问题只能在很久以后由 Goursat 解决 $n = 4$ (VII)，以及 E. Cartan (IX f)) 和 Coxeter (XIV) 工作中的任意 $n$，我们稍后会返回。

随着《杀戮》和李群的 E. Cartan 的作品，一股新的思想流在 1890 年左右开始，并将在与之前的作品没有联系的情况下长期发展。在复杂半单李代数的结构的杀戮（VIII）和嘉当（IXa））的研究中，某些线性形式$\omega_\alpha$在这样的李代数的“嘉当子代数”$\mathfrak{h}$上$\mathfrak{g}$立即发挥了基础作用：它们是相对于$\mathfrak{h}$的“根”，之所以如此称呼，是因为它们出现为特征方程$\det(\operatorname{ad}_\mathfrak{g}(x) - T) = 0$的根，被视为$x \in \mathfrak{h}$的函数。 Killing 和 Cartan 建立的这些“根”的属性相当于断言，用第 1 章的语言来说。 VI，他们形式一个“约化根系”（cf.章节。VI。§ 1, no. 4）；然后他们表明，复杂的半单李代数约化到相关的“根系”的分类，其本身约化确定具有整数系数的某些矩阵（后来称为“嘉当矩阵”：cf.第VI, § 1, no. 5）。 Killing 和 Cartan 还表明，对于每个根 $\omega_{\alpha}$，根$^8$ 的集合的内卷置换 $S_{\alpha}$ 的存在；他们以基本方式使用置换的变换$C = S_{\alpha_1} S_{\alpha_2} \ldots S_{\alpha_l}$、乘积与$l$根相关，形成基本的系统（今天称为“考克塞特变换”的变换）；他们甚至将扩展这个置换转化为基本根$\omega_{\alpha_i}$($1 \leq i \leq l$)生成的向量空间的线性变换，并研究它的特征值((VIII.II),p. 20; (IXa))、p. 58)。但Killing和Cartan最初似乎都没有想到考虑由$S_{\alpha}$生成的群$G'$；而当Cartan稍晚一些时(IX b))，特征方程的确定伽罗瓦群$G$

$$
\det(\operatorname{ad}_g(x) - T) = 0
$$

对于“将军元素”$x \in \mathfrak{h}$，他最初研究它时没有引入$S_{\alpha}$；三十年后，在 H. Weyl 的影响下，他证明 (IX c)) $G'$ 是 $G$ 和确定在所有情况下结构商群 $G/G'$ 的正常子群，其中（对于简单的李代数 $g$) 是阶 1 或 2，除了型 $D_4$，它与 $S_3$ 同构的；同时，他将$G'$解释为群，由复杂的半单李代数的内自同构引起，留下固定的嘉当子代数$^9$。

我们刚才提到的 H. Weyl 的工作开创了群 $G'$ 的几何解释（此后称为 $g$ 的“Weyl 群”）；他的想法是将$S_{\alpha}$视为线性形式在$\mathfrak{h}$上的向量空间的反射，就像Killing和Cartan对$C$的变换一样。也是在 H. Weyl 的回忆录 (XIII) 中，出现了“仿射 Weyl 群”的基本域（但没有明确指出与“Weyl 群”$G'$ 的链接）； Weyl 用它来证明紧致半单群的基本群是有限的，在他的复数半单李代数的线性表示完全可约性的证明中，关键的点是关键的点。稍后，E. Cartan 完成了 H. Weyl 观点的全局点、他自己的实数或复数理论半单李代数以及他当时正在构建的黎曼对称理论空间的综合。在回忆录(IXd))中，他完成了Weyl群和仿射Weyl群的基本多胞位的确定，并引入了权的系统和部首权（第VI, § 1, no. 9章）；在(IX e))中，他扩展将讨论对称空间，特别是遇到了非约简根系的第一个例（第VI, § 4, no. 1章）。最后，文章(IXf))给出了第一个

(8) 记号 $\omega_{\alpha}$ 和 $S_{\alpha}$ 对应分别对应第 1 章的记号 $\alpha$ 和$s_{\alpha}$。 VI, § 1。
(9) 记号 $G$ 和 $G'$ 对应分别对应第 1 章的记号 $A(R)$ 和 $W(R)$ VI, § 1, no. 1。

证明由$\mathbf{R}^n$中的反射生成的每个不可约有限群都有一个基本域，其投影到$S_{n-1}$是一个球面单纯形；正是在这项工作中，他通过几何考虑证明了最高根的唯一性（对于根系的任意字典顺序）。

稍后，van der Waerden (XVI)从H. Weyl的回忆录开始，表明复杂半单李代数的分类与约化根系的分类是等价的，他是通过基本几何考虑来实现的（而对于Killing和Cartan，这种分类是行列式复杂计算的结果）。大约在同一时间，Coxeter 确定明确地指出了由反射产生的欧氏位移的所有不可约有限群 (XIV c))；这完成了嘉当的回忆录 (IX d))，它仅确定了“晶体学”群（即与根系相关的那些，或者嵌入在无限离散的群位移中）。第二年 (XIV d))，Coxeter 表明，由反射生成的有限群是唯一承认生成元 $R_i$ 的演示的有限群（最多同构），但受形式 $(R_i R_j)^{m_{ij}} = 1$ 的关系限制($m_{ij}$整数)，因此命名为“Coxeter”群，因为群（有限或非）承认这样的呈现。

我们上面描述的研究的两个流之间的第一个链接似乎是由Coxeter（XIV之二）建立的，然后是由Witt（XVII）建立的。他们观察到，由反射对应双射（最多同构）到复杂简单李代数产生的不可约无限群欧氏位移。 Witt 通过表征 Coxeter 群同构于欧氏位移的无限离散群，给出了该型的离散群以及上面提到的 Coxeter (XIV d)) 的扩展定理的新确定。这个结果，以及双曲几何中类似的群也是Coxeter群$^{10}$的事实，导致了后者群被直接研究，最初强调几何实现（（XV），（XXV）），然后跟随J. Tits（XXV），在纯粹的代数框架。

从维特的工作开始，半单李群理论和由反射产生的离散群理论继续彼此极其富有成效地相互作用。 1941 年，Stifel (XVIII) 注认为 Weyl 群恰好是由留下晶格不变量的反射生成的有限群。 Chevalley (XIX a)) 和 Harish-Chandra (XX a)) 在 1948-51 年给出了“晶体学”群和复数半单李代数之间的双射对应的*先验* 证明：在此之前，只能对于简单李代数的每个型分别验证这个对应。

(10) 这些群，在维数 2 的情况下进行了深入研究，迄今为止仅在维数 $\geq 3$ 中被顺便考虑过。

另一方面，在 1950 年左右观察到，Weyl 群下的多项式不变量在无限维线性表示 (XX a)) 理论和李群的拓扑理论中发挥着重要作用。 Coxeter (XIV f)) 再次开始研究通过对反射产生的有限群 W 的基本反射取乘积所形成的变换 C。他观察到（通过对每个型的单独检查），W下不变多项式的代数是由代数独立的元素生成的，其次数以简单的方式与C的特征值相关。这些结果的先验证明由第一个领域的 Chevalley (XIX b)) 给出，第二个领域由 Coleman (XXIII) 和 Steinberg (XXIV) 给出。

随着 A. Borel 在线性代数群 (XXII) 上的工作，新的发展开始导致李群理论的显着扩展。 A. Borel 强调了李群的最大连通可溶子群（自称为“Borel 子群”）的重要性，并使它们成为将经典理论的大量部分传输到代数闭域代数群的主要工具（但没有获得简单代数的分类） 群$^{11}$）。 Borel 子群（在实数或复数经典群的情况下）早在几年前就已经出现在Gelfand和Neumark关于无限维表示的工作中； 1954 年，F. Bruhat 发现了一个值得注意的事实，即对于经典简单群，群的分解到 Borel 子群上的双陪集，可以通过 Weyl 群 (XXI) 以规范的方式进行索引。该结果随后被 Harish-Chandra (XX b)) 扩展到所有实数和复数半单群。另一方面，1955 年，Chevalley (XIX c)) 成功地将半单李代数 g 和每个交换域 k、矩阵的群与 k 中具有 Bruhat 分解的系数关联起来；他用最后一个事实来表明，除了少数数例外，如此定义的群是简单的（在抽象群理论的意义上）。因此，他“解释”了乔丹和李已经注意到的，型A、B、C、D的简单李群（在李群理论的意义上）与在任意域上以纯代数方式定义的经典简单群之间的巧合（直到那时才被认为是巧合）由 Dickson 扩展到特殊的型 G_2 和 F_4 (XI b) 和 c)))。特别是，通过取有限域 k，Chevalley的构造，对于复杂简单李代数的每个型，提供了一组有限简单群，包含当时已知的有限简单群的一个大数以及三个新的级数（相应的到型 F_4、E_7 和 E_8 的简单李代数）。不久之后，通过各种方法，并使用 Chevalley 的修改，几位作者（Herzig、Suzuki、

$^{11}$ 维数 > 0 的代数群被认为是简单的（在代数几何的意义上），如果它除了自身之外不包含维数 > 0 的任何正常代数子群。如果它与简单非阿贝尔群的乘积同构，则称其为半单。

Ree, Steinberg and Tits) showed on the one hand that the other finite simple groups known at the time could be obtained in an analogous way, with the exception of the alternating groups and the Mathieu groups, and on the other hand constructed other series of new finite simple groups (cf. (XXIX)).

大约在同一时间，Chevalley (XIX d)) 再次开始研究线性代数群，并利用 Bruhat 分解的技术以及 Borel 子群归一化器的关键结果表明，半单线性代数群的理论任意特征$^{12}$的代数闭域$k$导致与$k = \mathbf{C}$的Killing-Cartan分类基本相同的型。 之后，J. Tits（XXV a）和 b））分析了 Chevalley 的方法，得出了 Bruhat 分解（“BN 对”）的公理化版本，在一个非常通用的形式中，仅涉及群结构；正是这个概念现在被称为“奶子系统”。我们上面讨论的所有简单的群（具有项的各种含义）都规范地配备了Tits系统，并且Tits本人（XXVc））已经证明了抽象群G中存在这样的系统，以及纯的一些附加属性群理论，允许人们证明 G 是*简单的*，定理涵盖了迄今为止为这些群给出的证明的大部分（cf. 第 IV。§ 2, no. 6）。另一方面，他与 A. Borel 合作，通过证明半单线性代数群的有理点群中 Tits 系统在*任意*上的存在性，推广了 Chevalley 在 (XIX d)) 中的结果域（XXVII）。

这些问题中遇到的所有 Tits 系统都有有限的 Weyl 群。 例的另一个类别是由Iwahori和Matsumoto发现的（XXVI）；他们证明，如果在 Chevalley 的构造 (XIX c)) 中，$k$ 是$p$-adic 域，则获得的群具有一个 Tits 系统，其 Weyl 群是 *仿射* Weyl 群复杂的半单李代数一开始。这个结果已被 Bruhat 和 Tits (XXVIII) 扩展到局部域上的所有半单代数群。

(12) 特征$p > 0$的域上存在大量“病态”简单李代数，可能会导致一些人怀疑Killing-Cartan分类的普遍性特征标。

(I) J. HESSEL, Krysalloometrie oder Krystallonomie und Krystallographie（1830 年，重述于奥斯特瓦尔德的 Klassiker，第 88 和 89 期，莱比锡 (Teubner)，1897 年）
(II) A. Bravais, Mémoires sur les polyèdres de forme symétrique, Journal de Math., (1), v. XIV (1849), p. 141-180。
(III) A. 莫比乌斯: a) Ueber das Gesetz der Symmetrie der Krystalle und die Anwendung dieses Gesetze auf die Eintheilung der Krystalle in Systeme, J. für die reine und angewandte Math., v. XLIII (1852), p. 365-374（= Gesammelte Werke，v.II，莱比锡（希泽尔），1886 年，p. 349-360）； b) 对称图形理论，Gesammelte Werke，v. II，莱比锡 (Hirzel)，1886，p. 561-708。
(IV)L。 SCHLAFLI，《vielfachen Kontinuität 理论》。登克施尔。瑞士。自然研究。 Gesellschaft，v. XXXVIII (1901)，p. 1-237（= Ges. math. Abhandlungen，v. I，巴塞尔 (Birkhäuser)，1950，p. 167-387）。
(V) W. R. HAMILTON，关于单位元的根新系统的备忘录，Phil。 Mag.，(4)，第 XII (1856)，p. 446。
(VI)C。乔丹，《群 de 运动回忆录》，安。 di Mat.，v.II (1868-69)、p. 167-215 和 322-345（= Oeuvres，v.IV，巴黎 (Gauthier-Villars)，1964 年，p. 231-302）。
(VII) E. GOURSAT，Sur les 代换正交和空间划分，Ann。例如。 范数。 Sup., (3), v. VI (1889), p. 9-102。
(VIII) W. KILLING, Die Zusamensetzung der stetigen endlichen Transformationsgruppen: I) 数学。安.，v. XXXI (1888)，p. 252-290； II）同上，第XXXIII（1889），p. 1-48； III）同上，第XXXIV（1889），p. 57-122； IV）同上，v.XXXVI（1890），p. 161-189。
(IX) E. CARTAN: a) Sur la 结构 des 群 de 变换完成并继续（论文）。巴黎 (Nony)，1894 年（= 作品集，巴黎 (Gauthier-Villars)，1952 年，v. I1，p. 137-287）； b) Sur la réduction à sa forme canonique de la 结构 d’un groupe de conversions fini et continue, Amer.日记。数学，v. XVIII (1896)，p. 1-46（= Oeuvres complètes，巴黎 (Gauthier-Villars)，1952，v. I1，p. 293-353）； c) Le Principe de Dualité et la théorie des 群 simples et 半单，Bull。科学。 Math.，v. XLIX (1925)，p. 361-374（= Oeuvres complètes，巴黎 (Gauthier-Villars)，1952，v. I1，p. 555-568）； d) La géométrie des 群 simples，安。 di Mat., (4), v. IV (1927), p. 209-256 (= Oeuvres complètes, 巴黎 (Gauthier-Villars), 1952, v. I2, p. 793-840)； e) Sur certaines 形式 riemanniennes remarquables des géométries à groupe foldamental simple，Ann。例如。 范数。 Sup., (3), v. XLIV (1927), p. 345-467 (= Oeuvres complètes, 巴黎 (Gauthier-Villars), 1952, v. I2, p. 867-989)； f) 补充记忆“Sur la géométrie des 群 simples”，Ann。 di Mat., v, V (1928), p.

253-260 (= Oeuvres complètes, Paris (Gauthier-Villars), 1952, v. I2, p. 1003-1010)。

(X) R. FRICKE 和 F. KLEIN，自形态 Funktionen 理论，莱比锡 (Teubner)，1897 年。

(XI)L。 E. DICKSON：a) 任意域中线性群的理论，Trans。阿米尔。数学。 Soc.，v. II (1901)，p. 363-394； b) 简单群的新系统，数学。安，t。 LX (1905), p. 137-150; c) 群的类在与立方体表面夸脱上 27 条线的配置相关的任意领域中。日记。数学.. v. XXXIII (1901), p. 145-173 和 v. XXXIX (1908)。 p. 205-209。

(XII) A. 斯派瑟。 Theorie der Gruppen von endlicher Ordnung，柏林（施普林格），1924 年。

(XIII) H. WEYL，线性变换中连续线性变换的理论，数学。 Zeitschr., v. XXIII (1925)、p. 271-309、v. XXIV (1926)、p. 328-395 和 789-791（= Selecta，巴塞尔-斯图加特（Birkhäuser），1956 年， p. 262-366）。

(XIV) H.S.M.COXETER: a) 群，其基本区域是单纯形，Journ。伦敦。数学。 Soc.，v. VI (1931)，p. 132-136； b）具有规则棱柱形图形的多面体，Proc。伦敦。数学。 Soc.，(2)，v. XXXIV (1932)。 p. 126-189； c) 由反射生成的离散群，Ann。数学，(2)，v. XXXV (1934)，p. 588-621； d) 形式$R_i^2 = (R_i . R_j)^{k_{ij}} = 1$有限群的完整枚举，Journ。伦敦。数学。 Soc.，v. X (1935)，p. 21-25； e) 正则多胞体，纽约 (Macmillan)，1948 年（第 2 版，1963 年）； f) 乘积 / 生成元 / 有限群由反射生成，杜克大学数学。 Journ.，v. XVIII (1951)，p. 765-782。

（XIV之二）H. S. M. COXETER 和 H. WEYL，连续群的结构和表示（Adv. Study 研究所，由 N. Jacobson 和 R. Brauer 油印注，1934-35）：附录。

(XV) H. S. M. COXETER 和 W. O. J. MOSER，生成元和关系用于离散群，Ergebn。 der Math.，Neue Folge，Bd。 14，柏林（施普林格），1957 年（第 2 版，1963 年）。

(XVI) B. L。 van der WAERDEN，Die Kclassification der einfachen Lieschen Gruppen，数学。 Zeitschr.，v. XXXVII (1933)。 p. 446-462。

(XVII) E. WITT，Spiegelungsgruppen und Aufzählung halbeinfacher Lieschen Ringe，Abh。数学。 SEM。汉布。大学，v. XIV (1941)，p. 289-322。

(XVIII) E. STIFEL，Ueber eine Beziehung zwischen geschlossenen Lie’sche Gruppen und discontinuierlichen Bewegungsgruppen euklidischer Räume und ihre Anwendung auf die Aufzählung der einfachen Lieschen Gruppen，Comm。数学。 Helv.，v. XIV (1941-42)，p. 350-380。

(XIX)C。谢瓦利：a) Sur la Classification des algèbres de Lie simples et de leurs representations, C。 R.阿卡德。科学，第 CCXXVII (1948)，p. 1136-1138； b) 由反射生成的有限群不变量，Amer。日记。数学，第 LXXVII (1955)，p. 778-782； c) Sur certains 群 simples，东北数学。杂志，(2)，第 VII (1955)，p. 14-66； d) Classification des 群 de Lie algébriques，第 2 卷，巴黎（Inst. H. Poincaré），1956-58。

(XX) HARISH CHANDRA: a) 关于半单李代数的通用包络代数的一些应用，Trans。阿米尔。数学。 Soc.，v. LXX (1951)，p. 28-96； b) Bruhat 引理，Journ。 de Math.，(9)，v. XXXV (1956)，p. 203-210。

(XXI) F. BRUHAT，群谎言半单复合体的代表，C。 R.阿卡德。 《科学》，第 CCXXXVIII (1954)，p. 437-439。

(XXII) A. BOREL，群 lineéaires algébriques，Ann。数学，(2)，v. LXIV (1956)，p. 20-80。
(XXIII) A. J. COLEMAN，简单群的 Betti 数，Can。日记。数学，第 X (1958)，p. 349-356。
(XXIV) R. STEINBERG，有限反射群，Trans。阿米尔。数学。 Soc.，诉XCI (1959)，p. 493-504。
(XXV) J. TITS: a) 群 simples et géométries associées，Proc。国际。国会数学，斯德哥尔摩，1962 年，p. 197-221； b) 定理 de Bruhat et sous-groupes paraboliques, C。 R.阿卡德。科学，第 CCLIV (1962)，p. 2910-2912； c) 代数和抽象简单群，安。数学，(2)，第 LXXX (1964)，p. 313-329。
(XXVI) N. IWAHORI 和 H. MATSUMOTO，关于 p-adic Chevalley 群的 Hecke 环的一些 Bruhat 分解和结构，出版。数学。 I.H.E.S.、no. 25 (1965)、p. 5-48。
(XXVII) A. BOREL 和 J. TITS。 群 réductifs，出版。数学。 I.H.E.S.、no. 27 (1965)、p. 55-150。
(XXVIII) F. BRUHAT 和 J. TITS, 群 algébriques simples sur un corps local, Proc.会议。本地域、p. 23-36。柏林（施普林格），1967 年。
(XXIX) R. CARTER，简单群和简单李代数，Journ。伦敦。数学。 Soc.，v. XL (1965)，p. 193-240。
