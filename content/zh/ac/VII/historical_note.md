---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: ac-i-vii
book_pages: 579-606
pdf_pages: 0597-0624
extraction: ocr
statements: 0
exercises: 0
content_sha256: 24254b1c2b68e87179b94735b0e75b1192d2cabd29244a1e74deba5fc90585f8
translated_from: content/en/ac/VII/historical_note.md
translation_method: google
source_content_sha256: bbb8b633a178f7d139d4a1446708b7b1e80f9f0ec88beab5aabe72c2e5e2295a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f4ad46b78be5f393eb6bec2b0a12cb49f40dd43d17bbf60d7ac49b06b70fd962
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（括号内的数指本注末尾的参考书目。）

《抽象》交换代数是最近的创作，但它的发展只能理解为代数数理论和代数几何理论的函数，代数几何理论是它的诞生。

据推测，著名的“证明”费马声称对于$p$奇素数而言，方程$x^p + y^p = z^p$是不可能的，而$x, y, z$整数$\neq 0$取决于分解

$$
(x + y)(x + \zeta y) \ldots (x + \zeta^{p-1} y) = z^p
$$

在环$\mathbf{Z}[\zeta]$（其中$\zeta \neq 1$是单位元的第$p$第根）以及环中的整除性论证，假设它是主理想整环。无论如何，拉格朗日（[2]，卷II，p. 531）概述了类似的论点； Euler ([1], vol. I, p. 488) (*) 和 Gauss ([3], vol. II, p. 387) 表明，正是通过这个型的参数，以及某些变化（特别是旨在降低方程次数的变量变换） Fermat 的定理代表 $p = 3$，高斯 (loc. cit.) 和 Dirichlet ([4], vol. I, p. 42) 代表 $p = 5$ 和 Dirichlet 方程的不可能性 $x^{14} + y^{14} = z^{14}$ ([4], vol. I, p. 190）。最后，在他关于数理论的第一个研究中，库默相信他已经以这种方式获得了一般的证明，毫无疑问，这个错误（狄利克雷向他指出的）引导他开始研究分圆域的算术，并最终成功地从中推导出他的素数证明的正确版本数$p < 100$[7d]。

另一方面，1831 年著名的高斯回忆录在双二次方程上

(*) 在证明中，欧拉认为$\mathbf{Z}[\sqrt{-3}]$是主理想整环，但事实并非如此；然而，通过考虑$\mathbf{Z}[\rho]$（$\rho$单位元的立方体根）的指挥，$\mathbf{Z}[\sqrt{-3}]$（cf.Sommer，Introduction à la théorie des nombres algébriques（trans.A.Lévy），巴黎（赫尔曼），他的论点可以被证明是正确的， 1911 年，p. 190）。

剩余类，其结果源自对“高斯整数”（[3]，卷II，p. 109）环 $\mathbf{Z}[i]$整除性的详细研究，清楚地表明了代数数整除性的扩张的兴趣坚持数理论的经典问题 (*)；因此，毫不奇怪，在 1830 年至 1850 年间，这一理论成为德国数学家众多著作的主题，首先是雅可比、狄利克雷和爱森斯坦，然后是稍后的库默和他的学生兼朋友克罗内克。我们这里不谈单位理论，它是数理论的一个过于专业的分支，进展非常迅速，爱森斯坦获得了三次域的单位的群的结构和克罗内克的分圆域，只是之前狄利克雷在 1846 年（[4]，卷I，p. 640）证明了一般性定理，埃尔米特几乎独立地达到了这一点（[8]，卷I，p. 159）。将分解转化为素数因子的问题（整个理论的核心）似乎要困难得多。由于拉格朗日已经给出了形式 $x^2 + D y^2$ (x, y, D 整数) 的数的例和除子，它们不是形式 $m^2 + D n^2$ ([2], vol. II, p. 465），众所周知，环$\mathbf{Z}[\sqrt{-D}]$一般不能预期为主理想整环，欧拉的鲁莽之后是相当谨慎的；当狄利克雷对于例证明关系 $p^2 - 5 q^2 = r^5$ ($p, q, r$ 整数) 等价于

$$
p + q \sqrt{5} = (x + y \sqrt{5})^5
$$

对于整数 x, y，他限制自己指出“对于许多其他素数数 [比5]也有类似的定理”（[4]，第I，p. 31）。在1831年高斯的回忆录和爱森斯坦关于立方剩余类的工作[6a]中，主理想整环$\mathbf{Z}[i]$和$\mathbf{Z}[\rho]$（$\rho = (-1 + i \sqrt{3})/2$，单位元的立方根）确实有完美类比的算术高级研究与有理整数理论和这些例至少在二次域的算术和高斯发展的二元二次形式理论之间的密切联系是非常明显的；但一般情况缺乏一个“字典”，可以通过高斯理论的简单翻译来处理二次域 (†)。

事实上，问题不是针对二次域，而是针对分圆域（其原因直到很久以后才会清楚地显现出来（cf.p. 585））。

(*) 高斯的研究关于双纽线和椭圆函数的除法与这条曲线有关，虽然在他生前没有发表，但可以追溯到1800年左右，一定引导他从这个时候开始考虑环$\mathbf{Z}[i]$的算术性质，除以数在这个环的理论中发挥了重要作用；请参阅 Jacobi 关于这个主题的说法（[5]，第 VI、p. 275）以及高斯论文中与这些问题相关的计算（[3]，第 II、p. 411；另请参阅 [3]，第 X_2 卷、p. 33 等）。

† 读者将在 Sommer 中找到二次形式和二次域之间的对应的精确描述，loc。引文，第 205-229 页。

首先解决了。从 1837 年开始，原本是一名分析师的库默尔转向分圆域的算术，这几乎占据了他 25 年的时间。和他的前辈一样，他研究了环$\mathbf{Z}[\zeta]$的整除性，其中$\zeta$是单位元$\neq 1$的第$p$根（$p$是奇素数）；他很快发现这里也遇到了环不是主理想整环，阻碍了算术[7a]中扩张或律的所有进展，直到1845年，之后8年的努力，曙光才出现，这要归功于他的“理想数”的定义 （[7c] 和 [7d]）。

用现代语言来说，库默所做的正是定义域$\mathbf{Q}(\zeta)$的估值：它们与他的“理想素数数”是一一对应的对应，因子出现在数$x \in \mathbf{Z}[\zeta]$的“分解”中的“指数”正好是值 $x$ 相应的估值。 由于$x$的共轭以及属于到$\mathbf{Z}[\zeta]$及其乘积$N(x)$（$x (*)$的“范数”）是有理整数，因此要定义的“理想素数因子”也必须是有理素数数的“因子”以及阶到定义，只要说出素数数$q \in \mathbf{Z}$的“理想素数除子”就足够了。 对于$q = p$，Kummer已经有效证明了[7a]主理想$(1 - \zeta)$是素数，并且其第$(p - 1)$第幂是主理想$(p)$；因此，本案没有提出新的问题。 对于 $q \neq p$ ，Kummer 的想法似乎是通过同余 $\Phi_p(u) \equiv 0 \pmod{q}$ 替换分圆方程 $\Phi_p(z) = 0$ ，在其他字中分解分圆多项式 $\Phi_p(X)$ 到域 $\mathbf{F}_q$ 并与每个不可约式关联该多项式的因子是“理想素数因子”。 一个简单的情况（在注 [7b] 中明确提到，库默在没有证明的情况下宣布了他的结果）是，其中 $q \equiv 1 \pmod{p}$;如果 $q = mp + 1$ 和 $y \in \mathbf{F}_q$ 是原语 $(q - 1)$-th 根 1，那么，在 $\mathbf{F}_q[X]$ 中，
$$
\Phi_p(X) = \prod_{k=1}^{q-1} (X - \gamma^{km})
$$

(*) 代数数的范数的概念回到拉格朗日：如果$\alpha_i$($1 \leq i \leq n$)是次数$n$多项式的根，他甚至考虑“范数形式”变量 $x_i$ 中的$N(x_0, x_1, \ldots, x_{n-1}) = \prod_{i=1}^n (x_0 + \alpha_i x_1 + \cdots + \alpha_i^{n-1} x_{n-1})$

毫无疑问，他的研究关于解的方程和“拉格朗日解析”（[2]，第VII，p. 170）向他暗示了这一点。值得注意的是，正是范数的乘法性质导致拉格朗日在二元二次形式、从而上的恒等式，高斯能够获得这些形式的“合成”（[2]，卷II，p. 522）。另一方面，当代数数理论大约在1830年出现时，它经常出现在方程$N(x_0, \ldots, x_{n-1}) = \lambda$的解的形式（特别是单位的研究中的$\lambda = 1$）或“范数”的研究中。 形式”（也称为“可分解的形式”）表示问题；即使在最近的著作中，这些特定丢番图方程的性质也得到了有效的应用，特别是在 p-adic 数理论中（Skolem，Chabauty）。

从$\gamma^{pm} = 1$开始。然后将每个因子 $X - \gamma^{km}$ 与 $q$ 的“理想素数因子” $q_k$ 联系起来，Kummer 表示，元素 $x \in \mathbf{Z}[\zeta]$（其中 P 是 $\mathbf{Q}$ 上的最小多项式）可被 $q_k$整除，如果$\mathbf{F}_q$、$P(\gamma^{km}) = 0$；到和以上，用现代语言，他将商环$\mathbf{Z}[\zeta]/q\mathbf{Z}[\zeta]$写为域的直接合成，与$\mathbf{F}_r$同构的。对于$q \not\equiv 1 \pmod{p}$，$\mathbf{F}_q[X]$中$\Phi_p(X)$的不可约因子不再是第一个次数，因此有必要用$P(X)$“伽罗瓦虚数”中的X替代因子的根 $\Phi_p$在$\mathbf{F}_q[X]$。 Kummer 通过经过（正如我们今天所说的那样）避免了这一困难，达到分解域 K of $q$； iff 是最小整数使得 $q^f \equiv 1 \pmod{p}$ 和 $p - 1 = ef$，K 只是伽罗瓦群的阶 f 子群的不变量的 $\mathbf{Q}(\zeta)$ 由……组成子域（阶的循环） $p - 1$) 中的 $\mathbf{Q}(\zeta)$ 超过 $\mathbf{Q}$；在其他字中，它是$\mathbf{Q}(\zeta)$的唯一子域，即次数e超过$\mathbf{Q}$；自高斯的论文集以来，它就广为人知，是由“时期”产生的

$$
\eta_k = \zeta_k + \zeta_{k+f} + \zeta_{k+2f} + \cdots + \zeta_{k+(e-1)f}
$$

$(0 \leq k \leq e-1, \zeta_v = \zeta^{g^v}$，其中 g 是同余 $z^{p-1} \equiv 1 \pmod{p}$) 的原语根，其中形式是它的正常基。如果$R(X)$是任何这些“周期”$\eta$的最小多项式（单调且具有有理整数系数），Kummer从高斯的公式开始，证明，在域$\mathbf{F}_r$上，$R(X)$也分解为不同的因子第一个次数 $X - u_j$ ($1 \leq j \leq e$) 的每一个 $u_j$ 现在与“理想素数因子” $q_j$ 相关联。对于定义“能被$q_j$整除”，Kummer 将每个$x \in \mathbf{Z}[\zeta]$写在形式$x = \sum_{k=0}^{f-1} \gamma^k y_k$中，其中每个$y_k \in K$本身可以唯一地写为次数$\leq e - 1$在$\eta$中的多项式，并且有理数整数系数；他说，$x$能被$q_j$整除，当且仅当，在F的$y_k$、元素中，用$u_j$代替$\eta$时，得到的都是零。但也需要$x$中$q_j$的“指数”定义。为此，Kummer 引入了我们现在所说的 $q_j$ 的均匀化器，即元素 $\rho_j \in K$，这样 $N(\rho_j) \equiv 0 \pmod{q}$、$N(\rho_j) \not\equiv 0 \pmod{q^2}$，最后使得 $\rho_j$ 可以被 $q_j$（在上面定义的意义上）整除，但不能被其他理想的因子整除$\neq q$，共$q$。这样一个$\rho_j$的存在已经被克罗内克在前一年的论文中有效地证明了（[9a]，p. 23）；然后写$\rho = N(\rho_j)/\rho_j$，库默说如果$x\rho_j^h \equiv 0 \pmod{q^h}$但$x\rho_j^{h+1} \not\equiv 0 \pmod{q^{h+1}}$，$q_j$在$x$中的指数等于h；当然，他从证明开始，关系$x\rho_j' \equiv 0 \pmod{q}$等价于$x$能被$q_j$整除（在上述意义上）。一旦完成了这些定义，“理想数”的通常整除性律的扩张到$\mathbf{Z}[\zeta]$不再提供严重的困难；从他的第一个回忆录 [7c] 库默甚至可以使用狄利克雷的“盒子方法”，证明“类”和“理想因子”在数中是有限的（*）。

(*)他只不过是在他的论文中重现了克罗内克的一个论点——

我们不会追究库默后来关于分圆域的工作的历史，涉及类数的确定以及在某些情况下费马定理对证明的应用。 我们只提一下，在 1859 年，他通过扩展方法获得（至少部分地）“Kummerian 域”$\mathbf{Q}(\zeta, \mu)$ 中的“理想素数数”，其中 $\mu$ 是不可约多项式 $P(X) = X^p - \alpha$ 的根，其中$\alpha \in \mathbf{Z}[\zeta]$[7e]。 有趣的是，Kummer 正是通过将 $\mathbf{Q}(<+)$ 视为域 $\mathbf{Q}(\zeta)$ 的循环扩张来设想问题，将其视为“基域”（†）：他从他假设的 $\mathbf{Z}[\zeta]$ 的“理想素数数”$q$ 开始除既不是$p$也不是$\alpha$，这次他检查（在现代的项）剩余类域$k$中的多项式$\overline{P}(X) = X^p - \bar{\alpha}$对$\mathbf{Q}(\zeta)$相应的到$q$的评估（$\bar{\alpha}$是$k$ 中的 $a$ 的典范像）。 由于$\mathbf{Q}(\zeta)$是单位元的第$p$第根的域，$\overline{P}$是不可约的$k$，或者第一个次数的因子的乘积。 在第一种情况下，Kummer 说 $q$ 在 $\mathbf{Z}[\zeta, \mu]$ 中仍然是素数；在第二个例子中，他引入了$\mathbf{Z}[\zeta]$的元素$w_i$（$1 \leq i \leq p$），其中$k$中的像是$\overline{P}$的根，并且他将每个指标$i$与一个理想素数因子联系起来$r_i$ / $q$；然后写 $W_i(X) = \prod_{j \neq i} (X - w_j)$，他说，对于系数为 $\mathbf{Z}[\zeta], f(\mu)$ 包含因子 $r_i$ $m$ 次的多项式 $f$，如果
$$
f(w_i) W_i^m(w_i) \equiv 0 \pmod{q^m}
$$
但是
$$
f(w_i) W_i^{m+1}(w_i) \not\equiv 0 \pmod{q^{m+1}}.
$$
到和以上，他以这种方式获得$\mathbf{Q}(\zeta, \mu)$的估值，该估值在$\mathbf{Q}$上未分支，这足以满足他所考虑的应用。

\*\*\*

库默在研究特定的域（他在费马的定理上的研究）时有机会遇到了数的偶然情况，这使得他们的研究变得更加容易。 扩张与形式方程组解的类有关
$$
N(x_0, x_1, \ldots, x_{n-1}) = a
$$
（[9a]，p. 25）。另一方面，Kummer 多次提到了 Dirichlet 在型方程上获得的结果（对于任何代数数域）；但这些结果既没有发表，也没有在狄利克雷的论文中找到。

(†) 在他的回忆录关于二次形式，系数为高斯整数的环中（[4]，第I卷，第533-618页）狄利克雷在不同的地方被引导考虑域的相对范数 $\mathbf{Q}(\sqrt{D}, i)$ 超过其二次方子域 $\mathbf{Q}(\sqrt{D})$。同样，爱森斯坦在研究单位元的第8个根时，将域和生成视为$\mathbf{Q}(i)$的二次方扩张，并相对于该子域使用范数（[&]、p. 253）。但库默的著作是对“亲戚域”进行深刻算术研究的第一个例。

库默的结果的一般情况存在相当大的困难，并且需要多年的努力。

以克罗内克和戴德金为主角，库默发现代数数之后的 40 年里，代数数理论的历史与 180 年前牛顿和莱布尼茨关于无穷小演算的发明的竞争没有什么不同（但幸运的是没有同样的尖酸刻薄）。 克罗内克（Kronecker）是库默尔在柏林的学生和后来的同事（正如我们所见，他的论文在库默尔的理论中起到了重要的点的作用）对“理想数”非常感兴趣，目的是将应用转化为他自己的研究；当我们看到他时，我们钦佩他惊人的洞察力，早在1853年（[9b]，p. 10）就宣布了阿贝尔的扩张的结构和阿贝尔的扩张的一般定理和$\mathbf{Q}$，也许更引人注目的是，在接下来的几年里，他创建了复数乘法理论并发现了第一个类域理论的萌芽（[9c] 和 [9d]）。 1857 年克罗内克写给狄利克雷的一封信（[9]，第 5 卷，第 418-421 页）表明，他当时已经掌握了库默的理论推广，而且库默本人也在他自己的一部著作中证实了这一点（[7e]，p. 57），并且克罗内克将在他的著作中多次提及这一理论。 回忆录 1860 至 1880 年间 (*)。

但是，尽管当时德国学校的数理论的数学家们都没有意识到克罗内克这些作品的存在，但克罗内克似乎只是将他的方法的原理传达给了有限的朋友和学生圈子，当他最终决定将其发表在他的1881年的回忆录上时[9e]，最重要的是，在他 1882 年伟大的“Festschrift”[9f] 中，戴德金忍不住表达了他的惊讶（[10]，第 III，p. 427），因为他想象这些过程与他听到的回声完全不同（[10]，第 III，p. 287）。此外，克罗内克远没有像戴德金那样拥有次数那样的非凡的阐述和清晰的天赋，因此毫不奇怪，它主要是后者的方法，已于1871年出版，它构成了代数数的理论框架；不管它多么有趣，克罗内克的“不定性的伴随”的方法，其中涉及数的理论，在我们眼中几乎不比戴德金的变体（cf.章VII, § 1，习题31）更重要，它主要是在另一个方向，面向代数几何，克罗内克的思想对于交换代数的历史具有重要意义，我们稍后会看到。

出于很久以后才能清楚地看到的原因，任何一般理论尝试的第一个预备当然是对代数整数的概念的澄清。这是在 1845-50 年左右获得的，尽管这很困难

(*) 关于他在这个主题上的思想的演变，请参阅他 1881 年关于判别式的回忆录的非常有趣的介绍 ([9e], p. 195)。

足以准确确定其出现的日期；似乎很可能是系统在加法和乘法（或者更准确地说，我们现在所说的有限秩的Z代数）下稳定的想法，或多或少有意识地导致了代数整数的一般定义：事实上，这个定义不可避免地受到了影响当形式$\mathbf{Z}[\theta]$的Z代数被限制为有限秩时，类比由单位元的根生成的环$\mathbf{Z}[\zeta]$，此时算术家关注的总是中心。无论如何，当狄利克雷（[4]，第I，p. 640）、埃尔米特（[8]，第I，第115和146页）和爱森斯坦（[6c]，p. 236）独立引入代数整数的概念时，他们似乎并不认为他们正在处理一个新概念，也不认为对其进行详细研究会有用；只有爱森斯坦有效地证明了（*loc.cit.*）两个代数整数的和和乘积是代数整数，并且没有进一步声称这个结果是原始的。

一个更微妙的点是环的确定，其中可以预期库默理论的推广。后者在他的第一个注[7b]中毫不犹豫地肯定，通过考虑环$\mathbf{Z}[\sqrt{D}]$（D整数），他可以重新获得他的方法高斯二元二次理论形式；他从未提出过这个想法，但显然他和任何其他人之前戴德金都认为，当$D \equiv 1 \pmod{4}$时，在环$\mathbf{Z}[\sqrt{D}]$中唯一的合成成为“理想”素数因子是不可能的（尽管根的立方体的例） 单位元表明，从高斯时代考虑的环$\mathbf{Z}[\rho]$与$\mathbf{Z}[\sqrt{-3}]$）不同（*）。 之前 Dedekind 和 Kronecker，唯一研究的环始终是型 $\mathbf{Z}[\theta]$ 或有时型 $\mathbf{Z}[\theta, \theta']$ (†) 的某些特定环 (†)。就克罗内克而言，考虑代数扩张的*所有*整数的想法可能是通过对代数函数的域的研究而首次向他提出的，其中这个环自然地出现为函数的集合，这是“有限的”在无限远的距离”；无论如何，他在 1881 年的回忆录中坚持对这些域中的“整数”的刻画的判别式（早在 1862 年就在柏林学院编写和宣布）[9e]。戴德金没有说明他自己关于这个点的想法的起源，但在他于1871年首次发表关于数域的文章中，环中的所有整数中的域在他的理论中发挥了重要作用；也是戴德金通过引入*导体*的概念，澄清了环及其子环与分数相同的域之间的关系[10c]。

(*) Although Kronecker must have been led to study the arithmetic of the rings $\mathbf{Z}[\sqrt{-D}]$ ($D > 0$) by his work on complex multiplication, he published nothing on this subject and the characterization of the integers of any quadratic field $\mathbf{Q}(\sqrt{D})$ is given explicitly for the first time by Dedekind in 1871 ([10c], pp. 105–106).

(†) 我们之前已经看到 Kummer [7e] 引入的例或环 $\mathbf{Z}[\zeta, \mu]$。 Earlier, Eisenstein had been led to envisage a subring generated by two elements of the ring of integers in the field of the 21st roots of unity [6b].

但这并不是唯一的困难。为了概括 Kummer 的思想，首先有必要通过分解域去除经过，这在非阿贝尔域的情况下自然不可能有类似物。而且这种迂回乍一看似乎非常令人惊讶和人为，因为从$\mathbf{Z}[X]$的不可约多项式$\Phi_p(X)$开始，人们可能想知道为什么库默不将他的想法推向逻辑结论，以及是什么阻止他使用当时众所周知的“伽罗瓦虚数”数理论。戴德金的学生 Selling 早在 1865 年就对推广进行了一次不幸的尝试，这一障碍更加明显地暴露出来：给定一个不可约多项式$P \in \mathbf{Z}[X]$，Selling将相应的多项式$\overline{P}(X)$分解为$\mathbf{F}_q[X]$中的不可约因子；因此，该多项式的根属于变为 $\mathbf{F}_q$ 的有限扩张 $F$；但是，在阶到定义中，以Kummer的方式销售$P(X)$的分裂域的整数中的$q$的“理想素数因子”的指数，毫不犹豫地说，*在域* $\mathbf{F}_r$，同余模 a *幂 of* $q$ ([11], p. 26);稍后，当他试图解决分枝问题时，他“邻接”了形式 $x^h = q$ ([11], p. 34) 方程的$\mathbf{F}_r$“想象的根”。显然，这些大胆的步骤（用$q$-adic 域取代有限域$\mathbf{F}_q$是合理的）在当时只能以无意义的结果告终。幸运的是，戴德金在 1857 年 [10a] 以“高等同余理论”为名，在另一个形式中再次提出了有限域 (*) 的理论：他将后者的元素解释为 $\mathbf{Z}[X]$ 的多项式关于 a 的“剩余类” 线性组合的“双模”由……组成，其系数为素数数$p$的$\mathbf{Z}[X]$和不可约一元多项式$P \in \mathbf{Z}[X]$（对于他来说，对于克罗内克来说，这毫无疑问是*模*一般思想的起源，其中他们将稍后独立到达）。根据他自己的证词（[10d]，p. 218），戴德金似乎是从攻击域$\mathbf{Q}(\xi)$中$p$的“理想因子”的问题开始的，其中$P \in \mathbf{Z}[X]$是$\xi$的最小多项式，如下（当然至少在“未分支”的情况下，即当$\mathbf{F}_p[X]$相应的到$P$中的多项式$p$没有倍数根时）：他在$\mathbf{Z}[X]$中写道，

$$
P = P_1 P_2 \ldots P_h + p \cdot G
$$

其中 $\overline{P}_i$ 不可约且在 $\mathbf{F}_p[X]$ 中不同；可以假设$G$（在$\mathbf{Z}[X]$中）不能被任何$P_i$整除，并且对于所有$i$，他写出$W_i = \prod_{j \neq i} P_j$；那么，如果$f \in \mathbf{Z}[X]$，则可以说$f(\xi)$包含是$p$的“理想因子”$p_i$

(*) 众所周知，该理论的某些结果由伽罗瓦首先发表，高斯在 1800 年左右获得了（以同余语言）； 之后高斯去世后，戴德金负责出版他的部分作品，并在回忆录于有限域留下的论文中被重新发现（[3]，第II卷，第212-240页）。

相应的到 $P_i$ $k$ 次如果

$$
f W_i^k \equiv 0 \pmod{p^k, P}
$$

和

$$
f W_i^{k+1} \not\equiv 0 \pmod{p^{k+1}, P}.
$$

与方法以及 Kummer 的“Kummerian 域”的关系在这里显而易见，并且 Kummer 最初的分圆域定义可以通过这种方式轻松恢复（参见例 Zolotareff 的工作 [14]，他最初独立于 Dedekind，后来发展了这些想法）。

However, neither Dedekind nor Kronecker who appears also to have made analogous attempts, could progress further in this direction, both of them halted by the difficulties presented by ramification ([10d], p. 218 and [9f], p. 325) (*). If 环 of 整数 $\mathbf{A}$ of 数域 $K$ under consideration admits 基 (over $\mathbf{Z}$) 由……组成 of 幂 of the same 整数 $\theta$，将上述方法推广到$\mathbf{Z}[\theta]$中的分支素数数（如Zolotareff指出*loc.cit.*））并不困难。但是有域$K$，而环$\mathbf{A}$中不存在这个型的基； and Dedekind even finished by discovering that there are cases where certain prime 数 $p$ (the "extraordinary 因子 of the discriminant" of 域 $K$) are such that, *for all* $0 \in \mathbf{A}$, 应用 the above 方法 of the minimal polynomial of $0$ over $\mathbf{Q}$ leads to attributing top 倍数 ideal 因子 when in fact $p$ is unramified in $\mathbf{A}$ ($\dagger$); he admits that he was held up for a long time by this unforeseen difficulty, 之前 managing to surmount it by the creation from scratch of the theory of 模 and ideals, in a masterly exposition (and already in a wholly modern style, in contrast with the discursive style of his contemporaries) in what is without doubt his masterpiece, the famous "11th 补充" to狄利克雷关于数理论的书 [10f]。 This work saw three successive versions, but already in the first (published as the "10th 补充" to the second edition of Dirichlet's book in 1871 [4 bis]) the essentials of 方法 are present and almost at one stroke the theory of algebraic 数 passes from sketches and earlier gropings to a fully mature discipline already possessing its essential tools: from the beginning, 数域的所有整数中的环放置在理论的中心处；戴德金证明了环超过$\mathbf{Z}$的基的存在性并且

(*) Zolotareff 通过改进他的方法来规避这个困难，这看起来只不过是轶事兴趣 [14]。

($\dagger$)克罗内克声称在单位元的第13个根的域的子域中遇到了同样的现象，但他没有更精确地描述（[9f]，p. 384）。 Dedekind 给出的判别式非凡的因子的例在 Hasse, Zahlentheorie (Berlin, Akad. 出版社，1949），p. 333；稍后，Hasse 给出了域 $K$ 的例，其中没有异常的判别式因子，但不存在 $\theta \in \mathbf{A}$ 使得 $\mathbf{A} = \mathbf{Z}[\theta]$ (*loc.cit.*, p. 335)。

由此推导出域的判别式的定义作为由整数的环的元素和整数的基及其共轭形成的行列式的平方；然而，对于二次域 ([10f], p. 202)，他只给出了分支素数数（作为判别式的素数因子）的第 11 个补充刻画，而他从 1871 年起就拥有了一般定理 (*)。这项工作的核心结果是理想到素数因子的存在以及分解的唯一性定理，为此戴德金首先发展了“模”的基本理论；事实上，在第十一章补充中，他为数域的子Z模块保留了这个名称，但他形式的概念和他所显示的结果已经以立即适用于一般模的方式进行了阐述（†）；值得注意的是，早在 1871 年，就​​引入了“传送器”概念，它在独特因数分解定理的第一个证明中发挥了重要作用（以及“上升链条件”）。在接下来的两个版本中，戴德金还给出了这个定理的另外两个证明，他公正地认为这是他的理论的基石。这里应该指出的是，正是在第三个证明中使用了分数理想（早在1859年Kummer就已经在分圆域中引入了分数理想），并且它们形式群得以建立；我们稍后将返回第二个证明（p. 594）。

所有这些结果（除了语言）毫无疑问已经为克罗内克在 1860 年左右所知，作为我们稍后讨论的更一般概念的特例（而戴德金承认他只是在 1869-70 年克服了他的理论的最后困难（[10e]，p. 351））（‡）；就数域而言，必须特别强调的是，此时克罗内克已经知道，整个理论在没有必要的变换的情况下是适用的，以“基域”k开始，它本身就是数域（除了$\mathbf{Q}$），点的观点复数乘法理论自然主导；因此，对于某些域 k，在 k ([9f], p. 269) 上存在无分支的代数扩张 $K \neq k$，这是不能对于 $k = \mathbf{Q}$ 成立的事实（如下来自 Hermite 和 Minkowski 对判别式的次要）。戴德金从未发展出最后的点观点（尽管他在1882年的关于不同的回忆录中表明了其可能性），而对“相对域”理论的首次系统阐述应归功于希尔伯特[16d]。

(*) 他只在不同的 [10e] 上的 1882 年的回忆录中给出了这个定理的证明。
(†) 在 1882 年关于代数曲线的回忆录（与 H. Weber 合作）[10之二]中，他以同样的方式使用模超过环$\mathbf{C}[X]$的理论。
(‡) 然而，在数域的情况下，克罗内克未能成功地通过他的方法获得完整的刻画分支理想。另一方面，他确实有一个变量的代数函数的域的刻画，并且进一步证明，在这种情况下，判别式不存在“异常因子”[9e]。

最后，在 1882 年[10e]，戴德金通过引入异性完成了该理论，这给了他一个新的判别式定义，并允许他定义精确地得到理想素数因子在后者分解中的指数。也正是在这个时候，他对伽罗瓦扩张所呈现的特殊特征产生了兴趣，引入了分解群的概念和惯性群（在他的1894年才发表的回忆录[10g]中），甚至（在他生前未发表的论文中（[10]，第11卷，第17页）。 410–411)) 分支群的草图，希尔伯特（独立于戴德金）稍后发展（[16c] 和 [16d]）。

这样，大约在1895年，代数数理论就完成了其发展的第一阶段；在这个形成时期形成的工具将使其几乎立即进入下一个阶段，即一般类域理论（或者，相当于阿贝尔的扩张或数域的理论），该理论一直延续到我们今天，我们在此不予描述。从交换代数的角度看点，可以说，同时戴德金域的历史实际上已完成，设定除了它们的公理刻画之外，还有这些域上的有限生成模的结构（在数域的情况下，将只有 Steinitz 在 1912 年才得到实质性阐明 [20b]) (*)。

\*   \*   \*

交换代数的后期进展主要源于完全不同的问题，源自代数几何（这还将直接影响数理论甚至之前当前时期的“抽象”发展）。

我们在这里不关心代数几何的详细历史，直到黎曼去世为止，代数几何几乎没有触及我们的主题。 只需回顾一下，它主要涉及复杂射影平面中的代数曲线的研究，通常通过射影几何方法（使用或不使用坐标）来实现。 There was a parallel development, with Abel, Jacobi, Weierstrass and Riemann, of the theory of "algebraic functions" of one complex variable and their integrals; mathematicians were obviously conscious of the connection between this theory and the geometry of plane algebraic curves and even on occasions were known to "apply Analysis to Geometry"; but the methods used for the study of algebraic functions were chiefly of a "transcendental" nature, even before Riemann (†); this character is still further accentuated in the work of the latter,

(*) Dedekind 已经开始研究代数数的模和环 [10h]。

(†) 但必须指出的是，维尔斯特拉斯在他的研究中关于阿贝尔的函数的论述（可以追溯到 1857 年，但仅在他 1865 年左右的讲座中进行了阐述，并且仅在他的全集（[17]，第 1 卷）中发表）。 IV))，与引入“黎曼曲面”和在该曲面上定义的任意解析函数形成对比。 几乎就在之后黎曼去世的同时，罗克，尤其是克莱布施认识到了从黎曼先验方法在曲线射影几何中的众多引人注目的应用所获得的深刻结果中获得的可能性，这当然会煽动当代几何学家给出这些结果的纯粹“几何”证明；该计划由 Brill 和 M 完备的，Clebsch 和 Gordan 未完全遵循。 几年后[13]，借助对给定曲线和辅助曲线（“伴随”）经过到点的系统的变量点的系统的研究。 但即使对于他的同时代人来说，黎曼的先验方法（尤其是他对拓扑概念和“狄利克雷的原理”的使用）似乎也建立在不确定的基础上；尽管布里尔和诺特比大多数当代“综合”几何学家要小心得多（见下文p. 593），但他们的几何分析方法也并非免受所有指责。 本质上，戴德金和韦伯在 1882 年就这一主题发表了他们伟大的回忆录 [10之二]，本质上是为了给平面代数曲线理论提供坚实的基：“下面发表的研究”，他们说，“旨在为一个变量的理论和代数函数奠定基础，这是黎曼的主要创造之一，其方式同时是简单、严格和完全的。一般。 在前面关于这个主题的研究中，一般来说，对所考虑的函数的奇异性做出了限制性假设，并且可能的例外情况要么在经过中作为限制情况提到，要么完全被忽略。 同样，关于连续性或分析性的某些基本定理被接受，其“证据”取决于不同性质的几何直觉”（[10之二]，p. 181）（*）。

对于黎曼来说，曲线亏格的纯代数定义，作为最小整数$p$，使得在给定任意点的情况下，曲线上存在极点位于$p + 1$的有理数函数。有趣的是，点发现，在曲线上只有一个极点的情况下，寻求获得元素作为函数，Weierstrass，之前最终为此目的使用超越函数，根据克罗内克（[9e]，p. 197），敦促后者扩展一个变量的代数函数，他当时刚刚获得的结果为数域（“理想素数因子”有效地扮演了维尔斯特拉斯所期望的角色）。

(*) 众所周知，尽管戴德金、韦伯和克罗内克做出了努力，但在 1870-1880 年德国代数几何的学校中已经可见的正确证明概念的松懈，在接下来两代法国尤其是意大利几何学家的工作中只会变得越来越严重。德国几何学家并发展了他们的方法，攻击代数曲面理论：这是代数学家经常谴责的“丑闻”（主要是自 1920 年以来），但在一定程度上被这些“不严谨”方法所取得的辉煌成功所证明是合理的，与此形成鲜明对比的是，直到 1940 年左右，戴德金的正统继承者才表明自己无法制定公式具有足够的灵活性和幂代数概念，这将允许给出这些结果的正确证明。

他们工作的基本思想是在戴德金刚刚发展的代数数理论的基础上，对一个变量的代数函数理论进行建模；为此，他们必须首先从“仿射”点的角度来看待它（与他们同时代的人相反，他们总是认为代数曲线嵌入在复射影空间中）：因此，他们从有理函数的域$\mathbf{C}(X)$的有限代数扩张K开始，并且K 中“积分代数函数”的环 A，即该域的元素在多项式环 $\mathbf{C}[X]$ 上积分；他们在不使用任何拓扑考虑（*）的情况下获得的基本结果是 A 是 Dedekind 域，可以对其进行必要的修改（甚至，如 Dedekind 和 Weber 注，尚未清楚地看到原因（[10]，第 I，p. 268），以更简单的方式）“11th 的所有结果” 补充”。完成此操作后，他们证明了它们的定理实际上是双有理不变的（在其他字中，仅取决于域 K），特别是不依赖于开始时创建的“无穷远线”的选择。毫无疑问，对我们来说更有趣的是，在“黎曼曲面”相应的到K的阶到定义点（特别是“无穷远的点”，其中不能对应到A的理想），他们被引导引入域 K 位置的概念：他们发现自己处于与 1940 年 Gelfand 发现自己相同的情况，当时他创立了规范化代数理论，知道元素的集合 K，而函数并没有给出开始时的函数，但人们想这样考虑；并且，为了获得假设的函数的定义集合，他们第一次有了将点 x 集合 E 以及与 E 的映射的集合 $\mathscr{F}$ 联系起来的想法（Gelfand 遵循了这一想法，并且通过在现代数学中的各个方面使用而变得司空见惯） $\mathscr{F}$到G的集合G映射$f \mapsto f(x)$，在考虑的其他字中，在表达式$f(x)$中，$f$作为变量而$x$作为固定的，与经典传统相反。最后，从位置的概念开始，他们毫无困难地定义“正除子”（术语中的“多边形”），其中包括作为特例的A的理想和对应到布里尔和诺特的“点的系统”；但是，尽管他们将微分的主除子和除子写为正除子的“商”，但他们并没有给出除子的一般定义，直到1902年，亨塞尔和兰茨伯格才通过与分数理想的类比引入了这个总是令人尴尬的概念纯粹“几何”方法的拥护者（尽管他们自己不得不将定义命名为“虚拟系统”，但因为无法给他们一个“具体”解释而感到不安）。

同年 1882 年，人们等待了 20 多年的克罗内克伟大的回忆录也出现了[9f]。比戴德金的作品雄心勃勃得多——

(*) 他们强调，由于这一事实，如果域 $\mathbf{C}$ 被所有代数数的域取代（[10]，卷 I，p. 240），他们的所有结果将仍然有效。

不幸的是，韦伯的说法也更加模糊和晦涩。 其中心主题（用现代语言来说）是研究多项式环 $\mathbf{C}[X_1, \ldots, X_n]$ 或 $\mathbf{Z}[X_1, \ldots, X_n]$ 之一上的有限积分代数的理想； Kronecker limits himself $a\ priori$ to those ideals which are finitely generated (the fact that they all are was only to be proved (for the ideals of $\mathbf{C}[X_1, \ldots, X_n]$)) some years later by Hilbert in the course of his work on invariants [16a]). 就$\mathbf{C}[X_1, \ldots, X_n]$或$\mathbf{Z}[X_1, \ldots, X_n]$而言，这自然会导致将环之一的每个理想与零公共的的“代数簇”由……组成与该理想的所有元素相关联； 19 世纪 2 和 3 维数中对几何学的研究直观地得出这样的观点：每个变体都是有限数个“不可约”变体的并，而这些“不可约”变体的“维数”不一定完全相同。 似乎这个事实的证明就是克罗内克集合本人的目标，尽管他没有明确说过，并且在他的回忆录中找不到“不可约多样性”的定义，也没有“维数”。 事实上，他极限自己总结性地指出了一般消除方法（*）如何从所考虑的理想的生成元的系统开始给出有限的数代数簇，其中每个代数簇在合适的坐标系统中，某个数坐标是任意的，其他坐标是“代数簇”其中函数" (†)。 但是，如果克罗内克的目标确实是分解进入不可约簇，那么必须认识到，他只是在基本理想的基本情况下才到达那里，在那里他有效地证明了，在$\mathbf{Z}[X]$上扩展了高斯的经典引理（[3]，第1卷）。 I, p. 34)，域$\mathbf{C}[X_1, \ldots, X_n]$和$\mathbf{Z}[X_1, \ldots, X_n]$是阶乘；而且，在一般情况下，克罗内克是否拥有素理想的概念是值得怀疑的（他所说的“Primmodulsystem”是一个不可分解的理想，就像另外两个理想的乘积一样（[9f]，p. 336）；这更令人惊讶，因为戴德金在1871年已经给出的定义是完全普遍的）。

然而，必须指出的是，克罗内克消除方法，如果应用得当，肯定会导致代数簇的分解变成其不可约成分：这是由E. Lasker在他1905年伟大的关于多项式理想的回忆录的开头明确建立的[19]；他定义正确的是

(*) 通过坐标的线性变换，可以假设理想的生成元 $F_i$ ($1 \leq i \leq r$) 是多项式，其中 $X_1$ 中最高次数的项是形式 $c_i X_1^{m_i}$，其中$c_i$是常数$\neq 0$。 还可以假设$F_i$没有公共的因子。 Consider then for $2r$ indeterminates $u_i, v_i$ ($1 \leq i \leq r$) the polynomials $\sum_{i=1}^r u_i F_i$ and $\sum_{i=1}^r v_i F_i$ as *polynomials in* $X_1$; form their Sylvester resultant, which is a polynomial in the $u_i$ and $v_i$ with coefficients in $\mathbf{C}[X_2, \ldots, X_n]$ (resp. $\mathbf{Z}[X_2, \ldots, X_n]$); by annihilating these coefficients, a system of equations is obtained whose solutions $(x_2, \ldots, x_n)$ are precisely the projections of the solutions $(x_1, \ldots, x_n)$ of the system of equations $F_i(x_1, x_2, \ldots, x_r) = 0$ ($1 \leq i \leq r$). 然后可以在$n$上通过归纳继续应用方法。

(†) 他将这个任意坐标的数称为 *维数*（“Stufe”）。

不可约簇（在 $\mathbf{C}^n$ 中）的概念作为代数簇V，使得两个多项式的乘积在整个簇上只能是零，如果其中一个是V，并且他还给出独立于选择的定义轴。在这部作品中插入的有趣的历史考虑中，拉斯克表明，他不仅对克罗内克和戴德金的纯代数倾向感兴趣，而且对由克莱布什和 M.诺特的学校的几何方法提出的问题感兴趣，特别是后者在 1873 年证明的著名的定理 [12]。正如我们今天所说，他本质上关心的是确定 $\mathbf{C}[X_1, \ldots, X_n]$ 的多项式的理想$\mathfrak{a}$，对于给定的 $\mathbf{C}^n$ 的集合 M，其在点处为零；通常，M 是零公共的到多项式 f 的“代数簇”，在数内有限，而且很长一段时间以来，人们似乎都接受（当然没有理由）至少对于 $n = 2$ 或 $n = 3$，理想的 $\mathfrak{a}$ 是由 f 简单生成的，(*)。 M. Noether 证明，即使对于 $n = 2$ 和两个多项式 $f_1, f_2$，这通常也是错误的，并且他给出了足够的条件，以便由 $f_1$ 和 $f_2$ 生成 $\mathfrak{a}$。十年后，内托证明，在$f_1$和$f_2$上没有假设，$\mathfrak{a}$的幂总是包含在$f_1$和$f_2$[15]、定理生成的理想中，这是希尔伯特于1893年在他的著名论文中推广的零点定理[16b]。毫无疑问，受到这个结果的启发，拉斯克在他的回忆录中，在环$\mathbf{C}[X_1, \ldots, X_n]$和$\mathbf{Z}[X_1, \ldots, X_n]$中引入了初等理想（†）的一般概念（之后已经给出了这些初等理想环定义，通过抄写戴德金的定义) 并显示 (*) 初等分解的存在

(*) 请参阅 M. Noether 在其回忆录 [13] 开头的注。 注在这个问题上有趣的是，根据拉斯克的说法，凯莱在 1860 年左右推测，对于$\mathbf{C}^3$ 中的每条扭曲代数曲线，存在有限的数多项式生成的 $\mathbf{C}[X, Y, Z]$ 多项式的理想，其在曲线上为零（在其他情况下） 字，希尔伯特有限性的特例定理[16a]）。

(†) 戴德金在“阶”中遇到了不是素理想幂的初理想例，即代数数的环，以及给定的数域作为域分数（[10]，卷III，p. 306）。克罗内克还给出了“不可分解”理想的例作为另外两个非平凡理想的乘积，即由$p^2$和$X^2 + p$生成的$\mathbf{Z}[X]$的理想，其中$p$是素数数（对于由$X$ 和 $p$ ([9f], p. 341))。

(‡) 拉斯克在所考虑的理想 $\mathfrak{a}$ 的零的簇V 的不可约成分的最大维数 $h$ 上前进归纳。在现代项中，他首先考虑素理想$\mathfrak{p}_i$（$1 \leq i \leq r$）包含$\mathfrak{a}$，其中对应到V的最大维数$h$的不可约分量。对于每个$\mathfrak{p}_i$，他将$\mathfrak{a}$的饱和度$q_i$与$\mathfrak{p}_i$相关联（cf.章IV, § 2, no. 3，命题5）；然后，他考虑$\mathfrak{a}$中$q_i$的运输者$b_i = \mathfrak{a} : q_i$，将$\sum b_i$元素c属于接收到$\mathfrak{p}_i$中的任何一个，并一方面表明$\mathfrak{a}$是$q_i$的交和 $\mathfrak{a} + (c) = \mathfrak{a}'$，另一方面，对于这些环 (*) 中的每个理想，都有V'。在这个分解中，他似乎并不关心唯一性的问题；稍后，麦考利 [21] 介绍了“沉浸式”和“非沉浸式”基本理想之间的区别，并表明后者是唯一确定的，而不是前者。最后应该指出的是，拉斯克还通过使用Weierstrass的“准备定理”，将点的邻域中收敛幂级数的扩展结果环。他的回忆录中的部分无疑是第一个从纯代数点的角度考虑环的地方，而拉斯克在此场合发展的方法强烈影响了克鲁尔，当时他在1938年创建了局部环（cf.）的一般理论[29d]、p. 204 和 passim）。

\*\*\*

催生现代交换代数的思想运动大约在1910年开始形成。如果说域的一般概念是在20世纪初达成的，那么第一个定义概念或环的一般著作可能是Fraenkel在1914年的著作[23]。此时，已经有了环的例，不仅有数理论和代数几何的整环，还有幂级数的环（形式收敛）和最后的代数（可交换或不可交换） 基域。然而，对于域和环的理论，催化剂作用似乎是由Hensel的$p$进数数理论发挥的，Fraenkel和Steinitz [20a]特别提到它是他们的研究的起始点。

Hensel 关于这个主题的第一篇出版物可以追溯到 1897 年。他从戴德金和韦伯在代数函数域 K 的黎曼曲面点与数域 $k$ 的素理想之间的类比开始；他建议继承数“Puiseux 展开”理论（19世纪中叶的经典理论），该理论在K的黎曼曲面的任何点的邻域中，允许每个元素$x \in \mathbf{K}$可以用收敛的形式来表示考虑点处的“均匀化器”的级数或幂（级数仅具有项的有限数）

$a'$的零只有维数$\leq h - 1$的不可约分量，这使得他可以通过归纳来结论。

(*) 有趣的是注，戴德金的唯一分解定理的第二个证明首先建立了唯一的简化初等分解的存在；在第 11 篇补充中未发表的一段话中，戴德金明确指出，证明的这个部分不仅对数域 K 的所有整数中的环 A 有效，而且对 K 的所有“阶”有效（[10]，卷III，p. 303）。只有在之后明确表明A是“完全积分封闭”（在术语之内）时，他才利用这一事实证明了上述分解的初等理想实际上是素理想的幂（[10]，卷III，p. 307）。

带负指数）。 Hensel 的类似证明，如果 $\mathfrak{p}$ 是$k$ 的素理想，位于素数数 $p$ 之上，则“$p$-adic 级数”可能与形式 $\sum_i \alpha_i p^i$（或 $\sum_i \alpha_i p^{i/e}$）的每个 $x \in k$ 相关联当$\mathfrak{p}$在$p$上分支时），$\alpha_i$被取为理想$\mathfrak{p}$的剩余类的域的给定代表系统；但他的伟大独创性在于，即使当对应到$k$*没有元素*时，他也考虑了这样的“展开”，通过类比黎曼曲面上超越函数积分级数中的展开[18a]。

在他余下的职业生涯中，Hensel 致力于一点一点地打磨和完善他的新演算；如果我们觉得他的态度犹豫不决或笨重，我们一定不能忘记，至少在开始时，他没有任何可以帮助他完成任务的现代数学拓扑或代数工具。 此外，在他的第一份出版物中，他几乎没有谈到拓扑概念，总的来说，对他来说，$p$进数整数的环（$\mathfrak{p}$是整数$\mathbf{A}$的环的素理想数域） $k$)，在现代项，环$\mathbf{A}/\mathfrak{p}^n$的逆极限对于$n$递增无限，在纯粹代数意义上；为了建立这个环及其分数的域的属性，在每一步都需要使用或多或少痛苦的*临时*参数（对于例来证明$p$-adic整数形式整环）。 将拓扑概念引入到$p$进数域的想法并没有出现在Hensel的作品之前 1905 [18d]中；直到 1907 年，之后出版了这本书，其中他根据自己的想法重新阐述了代数数理论 [18f])，他才得出了定义和 $p$-进数绝对值 [18e] 的基本性质，从这里开始，他将能够在柯西的基础上对其进行建模理论，一个新的“$p$-adic 数学分析”，他将能够在数理论中卓有成效地应用它（特别是通过使用$p$-adic指数和对数），从那时起，其重要性一直在增长。

亨塞尔从一开始就清楚地看到他的理论给经典阐述带来的简化，通过允许问题“局部化”并在域中进行工作，其中不仅可整性性质微不足道，而且由于他早在1902年就发现了基本的引理[18c]，多项式的研究“简化”多项式 mod $p$ 没有倍数根简化为对有限域以上多项式的研究。 早在 1897 年，他就对这些简化给出了惊人的例，特别是在与判别式相关的问题上（特别是他几年前给出的关于“非凡的除子”存在的标准的简短证明）。 但长期以来，$p$进数数似乎引起了当代数学家相当大的不信任；毫无疑问，当前对“太抽象”的想法的态度，但在部分中，作者的相当过分的热情也证明了这种态度（在数学新理论的狂热者中如此常见）。 Not content to apply his theory fruitfully to algebraic numbers, Hensel, impressed as all his contemporaries were, by the proofs of the transcendence of $e$ and $\pi$ and perhaps misled by the adjective "transcendental" applied both to numbers and to functions, had come to think that there existed a connection between his p-adic numbers and transcendental real numbers and he had thought for a moment that he had obtained a simple proof of the transcendence of $e$ and even of $e^e$ ([18d], p. 556) (*).

很快之后1910年，情况变换，随着下一代的崛起，受到Frtchet和F.Riesz关于拓扑的思想以及斯坦尼茨关于代数的思想的影响，从一开始就致力于“抽象”；它会知道如何吸收亨塞尔的作品并将其放置在其真正的位置。早在 1913 年，Kürschak [22] 就给出了绝对值的概念的一般定义，认识到超度量绝对值的重要性（其中p进绝对值为例），证明了（通过对证明建模） 实数) 域相对于绝对值的完备性的存在性，最重要的是，通常表明将绝对值扩展到给定域的任何代数扩张的可能性。但他没有看到绝对值的超度量特征标已经在素数域中显露出来；这个点是由Ostrowski建立的，他还确定了域$\mathbf{Q}$上的所有绝对值值以及将域特征化的基本定理与非超量度绝对值值作为$\mathbf{C}$的子域 [24]。从1920年到1935年，该理论将通过对绝对值进行更详细的研究来完成，这些绝对不一定是离散的，其中包括对经过到代数或超越扩张中出现的各种情况的检查（Ostrowski，Deuring，F. K. Schmidt）；另一方面，1931年，Krull介绍并研究了估价的一般概念[29b]，它将在随后的几年中被Zariski和他的代数几何的学校（†）大量使用。这里我们还必须提到，尽管超出了我们的范围，但对完整值域和完整局部环的结构的更深入研究可以追溯到同一时期（Hasse-Schmidt，Witt，Teichmuller，I.Cohen）。

\*\*\*

上面提到的Fraenkel的工作（p. 594）只处理了一个非常特殊的

(*) 这个研究不惜一切代价在 p-adic 级数和 Taylor 级数之间狭隘的平行性，也导致 Hensel 使自己显得很奇怪问题：他证明了例每个 p-adic 整数都可以写成级数的形式 $\sum_{k=0}^{\infty} a_k p^k$，其中$a_k$是有理数，选择这样使得级数不仅收敛于$\mathbf{Q}_p$，而且收敛于$\mathbf{R}$（也许与泰勒级数类比，它同时在多个地方收敛？）（[16e]和[16f]）。

(†) 例高度 2 的估值已由 H. Jung 于 1925 年偶然引入[27]。

环的型（阿廷的只有一个素理想，并且被假定为主理想）。除了斯坦尼茨关于域的工作[20a]之外，关于一般交换环研究的第一部重要著作是E.诺特关于理想理论的两本伟大的回忆录：1921年的著作[25a]，专门研究初等分解，它再次全面概括并完成了拉斯克和拉斯克的许多点结果。麦考利；以及 1927 年的 Dedekind 域公理化特征 [25b]。正如斯坦尼茨在域中所展示的那样，在这些回忆录中可以看出，一小部分数的抽象思想，例如不可约理想的概念、链条条件和整体封闭域的思想（最后两个，正如我们所见，已经由戴德金揭示）本身可以导致似乎密不可分的一般结果以及在先前已知的情况下的纯计算结果。

有了 E. Noether 的这些回忆录，再加上 Artin-van der Waerden 稍后关于除数理想的著作 [31] 以及 Krull 将这些理想与基本评估联系起来的著作 [29b]，一个世纪前开始的对理想的分解的长期研究 (*) 就这样完成了，同时现代的交换代数也开始了。

无数后来的研究关于交换代数的作品最容易根据几个重要的发展方向进行分组：

(A) 局部环和拓扑

尽管早期所有关于数理论和代数几何的著作中都包含了这一萌芽，但局域化的总体思想却非常缓慢地被揭示出来。 环或分数的一般概念仅由E. Noether的学生H. Grell于1926年定义，并且仅针对整环 [28]；它的扩张到更一般的环只能在1944年由C给出。 Chevalley 的诺特环以及 1948 年 Uzkov 的一般情况。直到大约 1940 年，克鲁尔和他的学校实际上是唯一在一般论证中使用局部环 A 和整环 A 的考虑；从 1940 年开始，这些环才会在 Chevalley 和 Zariski 的著作中开始明确出现在代数几何中 (†)。

对局部环本身的一般研究直到 1938 年 Krull 才开始

(*) 继定义除数理想之后，研究中相当多的数作品（Priifer、Krull、Lorenzen等）是在理想下进行的，这些理想在其他运算$a \mapsto a'$满足公理条件下不变，类似于运算的性质$a \mapsto A$：（A：a）产生分歧的理想；以这种方式获得的结果尚未在代数几何和数理论中找到应用。

(†) 在亨塞尔和他的学生关于数理论的著作中，局部环A，为了他们的完成而被系统性地忽视，毫无疑问是因为应用亨塞尔的引理对后者的可能性。

太棒了回忆录 [29d]。这项工作最重要的成果涉及维数理论和常规环，这里不谈；但这里第一次出现任意任意诺特局部环的完成，以及与局部环相关的分级环的仍然不完美的形式（*）；后者仅在 1948 年左右由 P. Samuel [36] 定义，并由 Leray 和 H. Cartan 在研究 on Algebraic 拓扑中独立定义。克鲁尔在上述工作中几乎没有使用拓扑语言；但早在 1928 年[29a]，他就证明了，在诺特环 $\mathbf{A}$ 中，理想$\mathbf{a}$ 的幂的交是$x \in \mathbf{A}$ 的集合，使得$x(1 - a) = 0$ 对于某些$a \in \mathbf{a}$；由此很容易推断出，对于$\mathbf{A}$的每个理想$m$，$\mathbf{A}$诱导上的$m$-adic拓扑在理想$\mathbf{a}$上，在$\mathbf{a}$上有$m$-adic拓扑；在 1938 年的回忆录，克鲁尔在证明完成了这个结果，在诺特局部环，所有理想都已结束。这些定理很快被Chevalley扩展到诺特半局部环，然后由Zariski扩展到以他的名字命名的环[33b]； Chevalley 还可以追溯到拓扑环中“线性紧性”的引入，以及完全半局部环结构的确定 [32b]。

(B) 从本地到全球的转变

自 Weierstrass 以来，一个变量的解析函数（特别是代数函数）习惯性地与其定义的黎曼曲面的点处的“展开”的集合相关联。在他关于数理论的书的介绍中（[18f]，V），Hensel 类似地将元素相应的的代数数域 $k$ 集合的每个元素关联到它在$k$相对于$k$（$\dagger$）上所有绝对值的完成中。可以说，正是这种点观点，在现代的交换代数中，取代了理想的分解公式，成为素理想的乘积（在某种意义上延伸了库默最初的点观点）。 Hensel 的注隐含地将 $k$ 嵌入到其所有完成的乘积中；这就是 Chevalley 在 1936 年用他的理论明确所做的事情

(*) 如果$m$是考虑中的诺特局部环$\mathbf{A}$的最大理想，并且$(\alpha_i)_{1 \leq i \leq r}$，则$m$的生成元的最小系统，Krull定义对于$\mathbf{A}$中的$x \neq 0$ $x$的“初始形式”如下：如果$j$是最大的整数，使得$x \in m^j$，则$x$的初始形式都是次数$j$的齐次多项式， $P(X_1, \ldots, X_r)$ 的系数为剩余类域 $k = \mathbf{A}/m$，因此 $x \equiv P(\alpha_1, \ldots, \alpha_r) \pmod{m^{j+1}}$。对于$\mathbf{A}$的每个理想$\mathbf{a}$，他将由$\mathbf{a}$的所有元素的初始形式生成的分级理想$k[X_1, \ldots, X_r]$相关联（“Leitideal”）；对他来说，这两个概念取代了相关分级的环。

($\dagger$) Hensel 将次数 $n$ 的域 $K$ 上的$\mathbf{Q}$、函数 $x \mapsto |x^{(i)}|$ 作为非超测量绝对值（其中 $1 \leq i \leq n$ 的 $x^{(i)}$ 为$x$的共轭）目前自狄利克雷以来一直使用；稍后奥斯特洛夫斯基将证明，这些函数本质上是$K$上唯一的非超测量绝对值。

“idèles”[32a]，它完善了 Priifer 和 von Neumann 早期的类似想法（后者将自己限制在将 $k$ 嵌入其 $p$ 进补的乘积中）(*)。虽然这有点超出了我们的范围，但在这里值得一提的是，由于idèles的群上适当的拓扑，局部紧致群的所有技术（包括哈尔测度）因此可以非常有效地应用于数理论。

在更一般的背景下，克鲁尔的定理[29b]将整体封闭域描述为评估环的交（这也相当于将正在考虑的域嵌入到评估环的乘积中）通常有助于对这些环的研究，尽管方法只是真正的易于处理克鲁尔域的基本评估。此外，克鲁尔经常展示[29e]（相当初级）“从本地到全球的通道”的例，方法由……组成，通过验证其“本地化”环$A_i$，显示整环$A$的性质， $A$ 其所有主要理想 ($\dagger$)；最近，Serre 发现这个方法适用于任意交换环 $A$，它也适用于 $A$ 模块，甚至足以“本地化”在 $A$ 的最大理想（章 II, §3，定理 1）： 点的视图与“谱”和在这些谱上定义的滑轮的想法密切相关（见下文，p. 602）。

(C) 整数和积分闭包
我们已经看到，代数整数的概念最初是为数域引入的，已经被 Kronecker 和 Dedekind 扩展到代数函数域，尽管在这种情况下它可能显得相当人为（不是相应的到射影概念）。 E. Noether 1927 年的回忆录，以及 Krull 从 1931 年开始的工作，表明了这些概念对更一般的环 ($\ddagger$) 的兴趣。克鲁尔特别负责

(*) 由于亨塞尔的注，数域$K$上的非超测量绝对值值习惯上被（滥用语言）称为$K$的“无限处”，与戴德金和韦伯定义的过程类比仿射曲线黎曼曲面的“无穷远点”(cf.p. 591)。

($\dagger$) 在谈到“从局部到全局的过渡”时，通常会提到与类域理论相关的更困难的问题，其中最著名的例是哈斯的回忆录（[26a]和[26b]）中关于二次形式的问题代数数域 $k$；除其他外，他还表明，对于方程 $f(x_1, \ldots, x_n) = a$ 在 $k^n$ 中具有解（$f$ 二次方形式、$a \in k$），它在 $k$ 的每个完成中具有解是充分必要的。根据 Hasse 的说法，型或定理的想法是由他的老师 Hensel 向他提出的 [26c]。这个“哈塞的原理”到群除了正交群之外的扩张是代数群的“阿代尔化”现代理论的目标之一。

($\ddagger$) Krull 和 E. Noether 极限自己整环，但他们的方法扩张对于一般情况并不困难；最有趣的回忆录定理将素理想提升为积分代数[29c]，以及扩展Dedekind-Hilbert的分解和惯性群理论[29b]。至于 E. Noether，我们要归功于她对归一化引理 (*) 的一般表述（从中得出希尔伯特零点定理），这也是整环在该域上的积分闭包有限的第一个一般标准（抄录克罗内克和戴德金的经典论证）。

最后，这里需要指出的是，整闭域概念目前如此重要的原因之一是Zariski对代数簇的研究；他发现“正常”簇（即那些局部环是完整闭域的簇）具有特别令人愉快的特性，特别是它们不具有“余维 1 的奇点”；然后我们发现，类似的现象对于“解析空间”也是成立的。因此，“归一化”（即运算，对于各种局部环，包括取它们的积分闭包）已成为现代代数几何武器库中的强大武器。

(D) 模及同源代数影响的研究

E. Noether 和 W. Krull 在代数中的工作的显着特征之一是“线性化”倾向，扩展了 Dedekind 和 Steinitz 对域理论的类似发展；在其他字中，理想首先被视为模，因此线性代数的所有构造（商，乘积和最近的张量积以及同态模的形成）都对它们产生影响，通常产生不再是理想的模。由此可见，在许多问题（对于交换环或非交换环）中，兴趣不应该仅限于研究环 A 的理想，相反，定理应该一般地表述为A-模（有时受到一定的有限性条件）。

同源代数的介入有力地强化了上述趋势，因为代数的这个分支本质上涉及的是线性性质的问题。我们不会在这里追溯它的历史；但有趣的是点指出，同源代数的几个基本概念（例如投射模和Tor函子）是在对模在戴德金域上相对于张量积的行为进行仔细研究时产生的，这是H. Cartan在1948年进行的一项研究。

关于这个主题的是I。 Cohen 和 Seidenberg 扩展 Krull 的提升定理，准确地表明了极限的有效性 [35]。值得一提的是，E. Noether 在她 1927 年的回忆录（[25b]，p. 30）中明确提到了这种推广的可能性。

(*) 希尔伯特 (Hilbert) 在 1893 年就已经断言了一个特殊情况 ([16b], p. 316)。

相反，可以预见，同源代数作为Ext函子（投射模和单射模）和Tor函子（平坦模）的“通用湮没子”自然引入的模的新类将为交换代数带来新的曙光。碰巧，主要的投射模和更扁平的模已经显示出自己的有用性：后者的重要性首先来自于注，由Serre首先提出[38b]，本地化和补全自然地引入了扁平模，从而以更令人满意的方式“解释”了这些已知的运算的属性，并使它们更容易使用。更值得一提的是（正如我们将在后面章看到的），同调代数的应用远不止于此，它在代数几何中发挥着越来越重要的作用。

(E) 频谱概念
最新的概念和交换代数有着复杂的历史。希尔伯特谱定理引入了希尔伯特空间的正交投影算子的有序集，形成了“布尔代数”（或者更确切地说是布尔格）（*），一对一的对应与类的布尔格可测量子集（对于合适的测量）$\mathbf{R}$。毫无疑问，他早期对希尔伯特空间算子的研究，大约是在1935年，促使M. H. Stone对布尔格进行了全面的研究，特别是通过集合的子集（或相对于某个等价关系的子集的类）来寻找其中的“表示”。他观察到，如果 $xy = \inf(x, y)$ 定义了乘法且 $x + y = \sup(\inf(x, y'), \inf(x', y))$ 定义了加法，则布尔格就变成了*可交换的* 环（而且是一个非常特殊的型）。在所讨论的布尔格是有限集合 $X$ 的所有子集的集合 $\mathfrak{P}(X)$ 的特殊情况下，立即可以看出 $X$ 的元素与对应具有自然的一对一关系，其最大理想为相应的“布尔”环； Stone 通过类似地考虑相应的环的极大理想的集合并与包含的极大理想的布尔格子集合的每个元素相关联，精确地获得了布尔格的一般表示定理 [30a]。

另一方面，拓扑空间的开子集的集合是布尔格的著名经典例。在第二篇论文 [30b] 中，Stone 表明事实上每个布尔格也与这种性质的布尔格同构。为此，当然有必要在“布尔”环的最大理想的集合上定义一个*拓扑*；这非常

(*) *布尔格子*是一个格序集合$E$，至少有元素$a$和最大元素$\omega$，其中律sup和inf中的每一个都相对于另一个进行*分配*，并且对于所有$a \in E$，存在一个唯一的$a' \in E$使得$\inf(a, a') = a$和$\sup(a, a') = w$（cf.*集合理论*，章III, § 1，习题17）。

只需将最大理想包含$a$的每个理想$a$集合作为封闭集合即可完成。

这里我们不谈这些思想对泛函数学分析的影响，它们在I发展的范数代数理论的诞生中发挥了重要作用。 格尔凡德和他的学校。 但在 1945 年，雅各布森观察到 [34]，斯通发明的定义拓扑的过程实际上可以应用于任何环$A$（可交换或不可交换），只要所采用的理想的集合不是最大理想的集合，而是双边“原始”理想的集合（即双面理想$b$使得$A/b$是本原环）；对于交换环来说，这些当然是最大的理想。 Zariski 在 1944 年 [33a] 的部分中，在代数函数域的 *位* 的集合上使用了类似的方法到定义拓扑。 然而，对于大多数代数学家来说，这些拓扑仍然只是好奇心，因为它们通常不是豪斯多夫拓扑，而且对研究这种不寻常的对象感到非常反感，这是可以理解的。 这种不信任只有在 A. Weil 在 1952 年证明，每个代数簇都可以被赋予上述型的自然拓扑，并且这个拓扑允许定义，与 *纤维束* 的概念的可微分或解析流形的情况完美类比 [37]；不久之后，Serre 有了将“相干滑轮”理论扩展到这些簇的想法，因此，在“抽象”簇的情况下，拓扑在基域为 $\mathbf{C}$ 时提供与通常的拓扑相同的服务，尤其是代数的应用方法涉及拓扑（[38a]和[38b]）。

从那时起，在整个交换代数中使用这种几何语言就很自然了。人们很快发现，考虑最大理想通常不足以获得有用的断言 (*)，而足够的概念是以相同方式拓扑的环*素的*理想的集合。随着谱的概念的引入，现在存在一个字典，允许交换代数的每个定理以非常接近Weil-Zariski时期代数几何的几何语言来表达；而且，这立即带来了后者范围的相当大的扩大，因此交换代数几乎不超过它最基本的部分[39]。

(*) 将注意力限制在“最大谱”上的不便源于以下事实：如果$\phi : A \to B$是环同态且$n$$B$的最大理想，$\phi^{-1}(n)$不一定是$A$的最大理想，而对于每个素理想$p$ $B$、$\phi^{-1}(p)$是$A$的素理想。因此，一般来说，极大理想$B$的集合的映射到$A$不能的最大理想集合自然会与$\phi$相关联。

1. L. Euler, Vollständige Anleitung zur Algebra (=Opera Omnia (1), vol. I, Leipzig-Berlin (Teubner), 1911).
2. J. L. Lagrange, Oeuvres, 14 volumes, Paris (Gauthier-Villars), 1867–1892.
3. C. F. Gauss, Werke, 12 volumes, Gottingen, 1870-1927.
4. P. G. Lejeune-Dirichlet, Werke, 2 volumes, Berlin (Reimer), 1889–1897.
4 (bis). P. G. Lejeune-Dirichlet, Vorlesungen über Zahlentheorie, 2te Aufl., Braunschweig (Vieweg), 1871.
5. C. G. J. Jacobi, Gesammelte Werke, 7 volumes, Berlin (Reimer), 1881–1891.
6. G. Eisenstein: (a) Beweis der Reciprocitatsgesetzefur die cubischen Reste in der Theorie der aus dritten Wurzeln der Einheit zusammengesetzen Zahlen, Crelle’s Journal, 27 (1844), pp. 289–310; (b) Zur Theorie der quadratischen Zerfallung der Primzahlen 8n + 3, 7n + 2 und 7n + 4, Crelle’s Journal, 37 (1848), pp. 97–126; (c) Über einige allgemeine Eigenschaften der Gleichung von welcher die Teilung der ganzen Lemniscate abhangt, nebst Anwendungen derselben auf die Zahlentheorie, Crelle’s Journal, 39 (1850), pp. 160–179 and 224–287.
7. E. Kummer: (a) Sur les nombres complexes qui sont formés avec les nombres entiers réels et les racines de l’unité, J. de Math., (1), 12 (1847), pp. 185–212; (b) Zur Theorie der complexen Zahlen, Crelle’s Journal, 35 (1847), pp. 319–326; (c) Ueber die Zerlegung der aus Wurzeln der Einheit gebildeten complexen Zahlen in Primfactoren, Crelle’s Journal, 35 (1847), pp. 327–367; (d) Mémoire sur les nombres complexes composés de racines de l’unité et des nombres entiers, J. de Math., (1), 16 (1851), pp. 377–498; (e) Über die allgemeinen Reciprocitatsgesetze unter den Resten und Nichtresten der Potenzen deren Grad eine Primzahl ist (Abh. der Kon. Akad. der Wiss. zu Berlin (1859), Math. Abhandl., pp. 19–159).
8. C. Hermite, Oeuvres, 4 Volumes, Paris (Gauthier-Villars), 1905–1917.
9. L. Kronecker, Werke, 5 volumes, Leipzig (Teubner), 1895–1930: (a) De unitatibus complexis, vol. I, pp. 5–71 (= Inaug. Diss., Berolini, 1845); (b) Über die algebraisch auflosbaren Gleichungen I, vol. IV, pp. 1–11 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1853, pp. 365–374); (c) Über die elliptischen Functionen fur welche complexe Multiplication stattfindet vol. IV, pp. 177–183 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1857, pp. 455–460); (d) Uber die complexe Multiplication der elliptischen Functionen, vol. IV, pp. 207–217 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1862, pp. 363–372); (e) Über die Discriminante algebraischer Functionen einer Variabeln, vol. II, pp. 193–236 (= Crelle’s Journal, 91 (1881), pp. 301–334); (f) Grundzuge einer arithmetischen Theorie der algebraischen Grössen, vol. II, pp. 237–387 (=Crelle’s Journal, 92 (1882), pp. 1–122).

10. R. Dedekind, Gesammelte mathematische Werke, 3 volumes, Braunschweig (Vieweg), 1932: (a) Abriss einer Theorie der höheren Kongruenzen in bezug auf einen reellen Primzahl-Modulus, vol. I, pp. 40–66 (=Crelle’s Journal, 54 (1857), pp. 1–26; (b) Sur la Théorie des Nombres entiers algébriques, vol. III, pp. 262–296 (=Bull. Sci. Math., (1), 11 (1876), pp. 278–288 and (2), 1 (1877), pp. 17–41, 69–92, 144–164, 207–248); (c) Uber die Anzahl der Ideal-Klassen in den verschiedenen Ordnungen eines endlichen Korpers, vol. I, pp. 105–157 (=Festschrift der Technischen Hochschule in Braunschweig zur Säkularfeier des Geburtstages von C. F. Gauss, Braunschweig, 1877, pp. 1–55); (d) Über den Zusammenhang zwischen der Theorie der Ideals und der Theorie der höheren Kongruenzen, vol. I, pp. 202–230 (=Abh. Kön. Ges. Wiss. zu Gottingen, 23 (1878), pp. 1–23); (e) Uber die Discriminantend endlicher Korper, vol. I, pp. 351–396 (=Abh. Kön. Ges. Wiss. zu Gdttingen, 29 (1882), pp. 1–56); (f) Uber die Theorie der ganzen algebraischen Zahlen, vol. III, pp. 1–222 (=Supplement XI von Dirichlets Vorlesungen über Zahlentheorie, 4 Aufl. (1894), pp. 434–657); (g) Zur Theorie der Ideale, vol. 11, pp. 43–48 (=Nachr. Gottingen, 1894, pp. 272–277); (h) Uber eine Erweiterung des Symbols (a, b) in der Theorie der Moduln, vol. II, pp. 59–85 (=Nachr. Göttingen, 1895, pp. 183–208).

10(bis). R. Dedekind-H. Weber, Theorie der algebraischen Funktionen einer Veränderlichen, Crelle’s Journal, 92 (1882), pp. 181–290 (=R. Dedekind, Ges. Math. Werke, vol. I, pp. 238–349).

11. E. Selling, Ueber die idealen Primfactoren der complexen Zahlen, welche aus den Wurzeln einer beliebigen irreductiblen Gleichung rational gebildet sind, Zeitschr.fur Math. und Phys., 10 (1865), pp. 17–47.

12. M. Noether, Uber einen Satz aus der Theorie der algebraischen Funktionen, Math. Ann., 6 (1873), pp. 351–359.

13. A. Brill-M. Noether, Ueber algebraischen Funktionen, Math. Ann., 7 (1874), pp. 269–310.

14. G. Zolotareff, Sur la théorie des nombres complexes, J. de Math. (3), 6 (1880), pp. 51–84 and 129–166.

15. E. Netto, Zur Theorie der Elimination, Acta Math., 7 (1885), pp. 101–104.

16. D. Hilbert: (a) Uber die Theorie der algebraischen Formen, Math. Ann., 36 (1890), pp. 473–534; (b) Uber die vollen Invariantensysteme, Math. Ann., 42 (1893), pp. 313–373; (c) Grundzuge einer Theorie des Galoischen Zahlkorpers, Gött. Nachr., (1894), pp. 224–236; (d) Zahlbericht, Jahresber. der D. M. V., 4 (1897), pp. 175–546 (translated into French by A. Lévy and Th. Got under the title “Théorie des corps de nombres algébriques”, Paris (Hermann), 1913).

17. K. Weierstrass, Mathematische Werke, 7 volumes, Berlin (Mayer und Muller), 1894–1927.

18. K. HENSEL: (a) Über eine neue Begriindung der Theorie der algebraischen Zahlen, Jahresber. der D. M. V., 6 (1899), pp. 83–88; (b) Ueber die Fundamentalgleichung und die ausserwesentlichen Diskriminantentheiler eines algebraischen Korpers, Gött. Nachr., (1897), pp. 254–260; (c) Neue Grundlagen der Arithmetik, Crelle’s Journal, 127 (1902), pp. 51–84; (d) Über die arithmetische Eigenschaften der algebraischen und transcendenten Zahlen, Jahresber. der D. M. V., 14 (1905), pp. 545–558; (e) Ueber die arithmetischen Eigenschaften der Zahlen, Jahresber. der D. M. V., 16 (1907), pp. 299–319, 388–393, 474–496; (f) Theorie der algebraischen Zahlen, Leipzig (Teubner), 1908.

19. E. LASKER, Zur Theorie der Moduln und Ideale, Math. Ann., 60 (1905), pp. 20–116.

20. E. STEINITZ: (a) Algebraische Theorie der Korper, Crelle’s Journal, 137 (1910), pp. 167–308; (b) Rechteckige Systeme und Moduln in algebraischen Zahlkörpern, Math. Ann. 71 (1912), pp. 328–354 and 72 (1912), pp. 297–345.

21. F. S. MACAULAY, On the resolution of a given modular system into primary systems including some properties of Hilbert numbers, Math. Ann., 74 (1913), pp. 66–121.

22. J. KÜRSCHAK, Über Limesbildung und allgemeine Körpertheorie, Crelle’s Journal, 142 (1913), pp. 211–253.

23. A. FRAENKEL, Uber die Teiler der Null und die Zerlegung von Ringen, Crelle’s Journal, 145 (1914), p p 139–176.

24. A. OSTROWSKI, Über einige Lösungen der Funktionalgleichung $\phi(x)\phi(y) = \phi(x.y)$, Acta Math., 41 (1917), pp. 271–284.

25. E. NOETHER: (a) Idealtheorie in Ringbereichen, Math. Ann., 83 (1921), pp. 24–66; (b) Abstrakter Aufbau der Idealtheorie in algebraischen Zahl- und Funktionenkörpern, Math. Ann., 96 (1927), pp. 26–61.

26. H. HASSE: (a) Ueber die Darstellbarkeit von Zahlen durch quadratischen Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 129–148; (b) Ueber die Äquivalenz quadratischer Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 205–224; (c) Kurt Hensels entscheidender Anstoss zur Entdeckung des Lokal-Global-Prinzips, Crelle’s Journal, 209 (1960), pp. 3–4.

27. H. JUNG, Algebraischen Flachen, Hannover (Helwing), 1925.

28. H. GRELL, Beziehung zwischen den Idealen verschiedener Ringe, Math. Ann., 97 (1927), pp. 490–523.

29. W. KRULL: (a) Primidealketten in allgemeine Ringbereichen, Sitz. Ber. Heidelberg Akad. Wiss., 1928; (b) Allgemeine Bewertungstheorie, Crelle’s Journal, 167 (1931), pp. 160–196; (c) Beiträge zur Arithmetik kommutativer Integritatsbereiche, III, Math. Zeitschr., 42 (1937), pp. 745–766; (d) Dimensionstheorie in Stellenringen, Crelle’s Journal, 179 (1938), pp. 204–226; (e) Idealtheorie, Berlin (Springer), 1935.

30. M. H. Stone: (a) The theory of representations for Boolean algebras, Trans. Amer. Math. Soc., 40 (1936), pp. 37–111; (b) Applications of the theory of Boolean rings to general topology, Trans. Amer. Math. Soc., 41 (1937), pp. 375–481.
31. B. L. van der Waerden, Moderne Algebra, vol. II, Berlin (Springer), 1931.
32. C. Chevalley: (a) Généralisation de la théorie du corps de classes pour les extensions infinies, J. de Math., (9), 15 (1936), pp. 359–371; (b) On the theory of local rings, Ann. of Math., 44 (1943), pp. 690–708.
33. O. Zariski: (a) The compactness of the Riemann manifold of an abstract field of algebraic functions, Bull. Amer. Math. Soc., 50 (1944), pp. 683–691 ; (b) Generalized semi-local rings, Summa Bras. Math., 1 (1946), pp. 169–195.
34. N. Jacobson, A topology for the set of primitive ideals in an arbitrary ring, Proc. Nat. Acad. Sci. U.S.A., 31 (1945), pp. 333–338.
35. I. Cohen-A. Seidenberg, Prime ideals and integral independence, Bull. Amer. Math. Soc., 52 (1946), pp. 252–261.
36. P. Samuel, La notion de multiplicité en Algèbre et en Gtomtrie algébrique, J. de Math., (9), 30 (1951), pp. 159–274.
37. A. Weil, Fibre-spaces in Algebraic Geometry (Notes by A. Wallace), Chicago Univ., 1952.
38. J. P. Serre: (a) Faisceaux algébriques cohérents, Ann. of Math., 61 (1955), pp. 197–278; (b) Géométrie algébrique et géométrie analytique, Ann. Inst. Fourier, 6 (1956), pp. 1–42.
39. A. Grothendieck, Éléments de géométrie algébrique, Publ. math. Inst. Htes Et. Scient., 1960.
