---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 2
section_title: Functions
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 351-357
pdf_pages: 0356-0362
extraction: ocr
statements: 0
exercises: 0
content_sha256: b80045e0253cacbeaf23f1f64a4d71f50babce89e9d337192991125970db4d7d
translated_from: content/en/ens/ER/02_s2_functions.md
translation_method: google
source_content_sha256: e080ea464bff6a7c05c7dc505f506fc7d9e94e4178becde6cca23d33e3bb7827
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 1b7c741f686bcc98ce64a1ef55890ae6da0650af9992831611338be7b3a70745
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2.函数

1. 设 E 和 F 为两个集合，它们可能不同，也可能不同。 E 的变量元素 $x$ 和 F 的变量元素 $y$ 之间的关系被称为 $y$ 中的*泛函关系，如果对于所有 $x \in E$，存在唯一的 $y \in F$，它在给定的关系中$x$.*

我们将*函数*命名为运算，这样它就与给定的关系和$x$中的每个元素$x \in E$元素$y \in F$相关联； $y$ 被认为是函数在元素 $x$ 的 *值*，并且函数被认为是由给定函数关系 *确定*。两个*等效*功能关系确定*相同*函数。这样的函数被称为“在F中取其值”并“在E上定义”。更简单地说，它也被称为*E*到*F的*映射。

2. 集合 E 的映射到集合 F 是一个新的集合的 *元素*，* E 的映射到 * F 的 *集合。如果 $f$ 是其中任意元素 E 的元素 $x$ 处的 $f$ 的集合、值通常用 $f(x)$ 表示。在某些情况下，记号 $f_x$（称为*指示* 记号；集合 E 则称为*指标* 集合）更可取。 关系“$y = f(x)$”是$y$中的泛函关系，其中确定$f$。

当形式$y = \langle x \rangle$的关系（其中$\langle x \rangle$表示$x$可能出现的符号组合）是$y$、函数中的泛函关系时，确定通常表示为记号 $x \rightarrow \langle x \rangle$，甚至简单的$\langle x \rangle$；这是非常公共的的语言滥用。对于例，如果X和Y是集合E的两个泛型子集，则关系$Y = \complement X$在Y中泛函；将$\mathfrak{P}(E)$的映射转化为$\mathfrak{P}(E)$，其中确定表示为$X \rightarrow \complement X$，或简称为$\complement X$。

我们通常会更简单地说，“让$f: E \rightarrow F$”，而不是说“让$f$是E到F的映射”。

为了描述涉及多个映射的情况，我们还可以使用*图表*，例如

$$\begin{array}{ccccc}
 & & \mathrm{C} & & \\
 & \overset{g}{\nearrow} & & \overset{h}{\searrow} & \\
\mathrm{A} \overset{f}{\longrightarrow} \mathrm{B} & \underset{v}{\longrightarrow} & & & \mathrm{E} \\
\downarrow u & & & & \downarrow w \\
\mathrm{D} & \underset{t}{\longleftarrow} & & & \mathrm{F}
\end{array}$$

其中箭头所附的字母表示箭头尾部的集合到其头部的集合的映射。

E 的映射到 F 之间的等式“$f = g$”的关系相当于关系“对于所有 $x \in \mathrm{E}, f(x) = g(x)$”。

3. 函数，定义在集合 E上，对于E的每个元素$x$取相同的值$a$，称为E上的*常数*函数；它由函数关系$y = a$决定。

E 的映射到 E 中，与 E 的每个元素 $x$ 相关联，这个相同的元素被称为*恒等* 映射。它由函数关系$y = x$决定。

如果 A 是 E 的任何子集，A 到 E 的映射与 A 的每个元素 $x$ 关联，相同的元素 $x$ 被视为 E 的元素，称为 A 到 E 的*规范* 映射。

令 $f$ 为集合 E 的映射自身。如果 $f(x) = x$，E 的元素$x$ 被认为是*固定*（或*不变*）*低于*$f$。

E 的元素 $x$ 被称为在 E 的映射集合到 E 下是*固定*（或*不变*），如果它在它们每个下都是固定的。

4. 设$f$为E到F中的映射，并令X为E的任意子集。则*X*下*$f$的*像为所有元素的F由……组成的子集Y $y$，其中有性质“存在$x \in$ E，使得$x \in$X和$f(x) = y$”。

X和Y之间的定义关系在Y中起作用，因此$\mathfrak{P}(\mathrm{E})$的确定映射进入$\mathfrak{P}(\mathrm{F})$。这个映射被称为*$f$的*规范扩张*到子集的集合；*通过滥用语言，它也被表示为$f$，我们写为$\mathrm{Y} = f(\mathrm{X})$。

对于所有 $f$ 和 $x$ 我们有

$$f(\emptyset) = \emptyset \quad \text{and} \quad f(\{x\}) = \{f(x)\}.$$

滥用语言，$f$在$x$的*值*$f(x)$也被称为*$x$*下*$f$的*像。

如果$y$是F的泛型元素，则性质“$y \in f(\mathrm{E})$”可以用说表示“$y$*是形式*$f(x)$”。

滥用语言，$f$下的E的像$f(\mathrm{E})$是有时，称为*$f$的*像。

如果我们有$f(\mathrm{E}) = \mathrm{F}$，也就是说，对于所有$y \in$ F，存在$x \in$ E，使得$y = f(x)$，则$f$被称为E *到* F上的映射，或*满射* 映射，或*满射*。

令 $x$ 为 E 的任意元素和 X 任意子集。 $f(x)$ 不是说，而是 $x$ 处的 $f$ 的值，以及 $f(\mathrm{X})$ 像 X在$f$下，是有时表示$f$*变换*（或*映射*）$x$转化为$f(x)$，X转化为$f(\mathrm{X})$； $f(x)$和$f(\mathrm{X})$分别被$x$和X的$f$称为*变换*。

如果 $f$ 是 E 的映射自身，则 E 的子集 X 被认为在 $f$ 下*稳定（如果 $f(\mathrm{X}) \subset \mathrm{X}$）。如果X在每个映射下都是稳定的，则子集X被称为在E到E的映射的集合下*稳定*。

5. 令$f$为E到F中的映射。则我们有以下命题，其中X和Y表示E的任意子集：

(a) 关系 $\mathrm{X} \subset \mathrm{Y}$ 意味着 $f(\mathrm{X}) \subset f(\mathrm{Y})$。

(b) 性质 $\mathrm{X} \neq \emptyset$ 相当于$f(\mathrm{X}) \neq \emptyset$。

(c) 对于所有 X，Y 我们有

$$(11) \qquad f(\mathrm{X} \cup \mathrm{Y}) = f(\mathrm{X}) \cup f(\mathrm{Y}),$$

$$(12) \qquad f(\mathrm{X} \cap \mathrm{Y}) \subset f(\mathrm{X}) \cap f(\mathrm{Y}).$$

6. 令$f$为E到F中的映射，并令Y为F中的任意子集。*$f$下*Y*的*逆像是所有元素的E由……组成的子集X $x$ 有性质 $f(x) \in \mathrm{Y}$。

X和Y之间的定义关系在X中起作用，因此$\mathfrak{P}(F)$的确定映射进入$\mathfrak{P}(E)$，称为f到集合的*逆扩张子集*，记为$\overset{-1}{f}$；因此我们写$X = \overset{-1}{f}(Y)$。

特别是，如果$y$是F的元素，那么$\overset{-1}{f}(\{y\})$将是所有$x \in E$的集合，使得$f(x) = y$。 关系“$f(x) = y$”和“$x \in \overset{-1}{f}(\{y\})$”是等效的。由于语言滥用，我们经常用 $\overset{-1}{f}(y)$ 来代替 $\overset{-1}{f}(\{y\})$。

E 在给定子集 A 上的子集 X 的 *迹* $X_A$ 是 A 的典范映射到 E (no. 3) 下的 X 的逆像。

7. 令 $f$ 为 E 到 F 的映射。则我们有以下命题，其中 X 和 Y 表示 F 的任意子集：

(a) 关系 $X \subset Y$ 意味着 $\overset{-1}{f}(X) \subset \overset{-1}{f}(Y)$。

(b) 对于所有 X，Y 我们有

(13) $$\overset{-1}{f}(X \cup Y) = \overset{-1}{f}(X) \cup \overset{-1}{f}(Y),$$

(14) $$\overset{-1}{f}(X \cap Y) = \overset{-1}{f}(X) \cap \overset{-1}{f}(Y),$$

(15) $$\overset{-1}{f}(\complement X) = \complement \overset{-1}{f}(X).$$

注公式 (12) 和 (14) 之间的差异；如果我们将 F 中的任意映射替换为 E 中的 $\overset{-1}{f}$，则 (14) 不适用于所有 X 和 Y。同样，对于任意映射的扩张，不存在 (15) 的类似物。

此外，我们还有$\overset{-1}{f}(\emptyset) = \emptyset$；但对于 F 的非空子集 X，我们也可以有 $\overset{-1}{f}(X) = \emptyset$。在序中，$X \neq \emptyset$ 应该暗示 $\overset{-1}{f}(X) \neq \emptyset$，$f$ 应该是 E *到* F 上的映射是充分必要的。

8. 如果 E 到 F 的映射 $f$ 使得对于所有 $y \in F$ 存在*至多一个* $x \in E$ 使得 $y = f(x)$ （在其他字中，集合 $\overset{-1}{f}(y)$ 要么为空，要么由单个元素组成），那么 $f$ 被称为 E 到 F 的*一对一* 映射，或*内射* 映射，或 *单射的*。那么，对于所有子集 X，E 的 Y，

(16) $$f(X \cap Y) = f(X) \cap f(Y).$$

9. 如果 E 到 F 的映射 $f$ 使得对于所有 $y \in F$ *恰好存在一个* $x \in E$ 使得 $y = f(x)$ （在其他字中，$\overset{-1}{f}(y)$ 由单个元素组成），则 $f$ 被称为E *到* F 的 *一对一* 映射，或 *双射的* 映射，或 *双射的*。这样的映射可以被表征为E到F上的映射和E到F上的“一对一”映射。

如果$f$是E到F的一对一映射，则关系$y=f(x)$不仅在$y$中起作用，而且在$x$中也*起作用。作为$x$中的泛函关系，它确定是F到E上的一对一的映射，称为映射$f$的*逆*。

注 $f$ 的逆矩阵 *扩张与 $f$ 的扩张的逆矩阵相同。

令 $g$ 为 $f$ 的倒数。那么关系“$y=f(x)$”和“$x=g(y)$”*等价*。 $g$的倒数是$f$。如果 $f$ 是 E 到 F 的一对一映射，我们不仅有关系 (16)，而且对于 E 的所有子集 X，

$$f(\mathrm{C}X)=\mathrm{C}f(X).$$

此外，$f$的扩张是$\wp(E)$到$\wp(F)$的一一对应的映射。

E 到 F 上的一对一映射及其逆映射据说*实现了 E 和 F 之间的一对一对应*；或者，我们说 E 和 F * 通过这些映射* 一对一地放入对应中。

集合 E 的一对一映射称为 E 的 *置换*。恒等映射是置换。如果置换与其逆元相同，则称为*对合*；对于例，$\wp(E)$的映射$X\rightarrow \mathrm{C}X$自身是对合的。

10. 在下面的命题中，X表示E的任意子集，Y表示F的任意子集：

(a) 如果 $f$ 是 E *到* F 的映射，我们有

(17)
$$f^{-1}(Y)=f^{-1}(Y\cap f(E)),$$

(18)
$$X\subset f^{-1}(f(X)),$$

(19)
$$f(f^{-1}(Y))\subset Y.$$

(b) 性质“对于所有 Y，$f(f^{-1}(Y))=Y$”和“$f$ 是 E 到 F 上的映射”是*等价的*。

(c) 属性“对于所有 X、$f^{-1}(f(X))=X$”和“$f$ 是 E 到 F 的*一对一*映射”是*等价的*。

(d) 属性“对于所有 X 和 Y，

$$f^{-1}(f(X))=X\qquad\text{and}\qquad f(f^{-1}(Y))=Y$$

和“$f$是E到F的*一对一*映射”是*等价*。

11. 令E、F、G为三个集合，它们可能不同，也可能不同。设$f$为E入F的映射，$g$为F入G的映射。E入G的映射，其值在E的任意元素$x$处为$g(f(x))$，称为合成* $g$和$f$，并用$g \circ f$表示，或者在不存在歧义的情况下简单地用$gf$表示。

等式 $h = g \circ f$ 被称为 $h$ 的*因式分解*。

注，如果G与E不同，我们可能不会谈论$f$和$g$的合成（其中序），并且记号$f \circ g$没有任何意义。如果G与E相同，则$f \circ g$和$g \circ f$不是相同的集合除非的元素，F也与E相同；即使是这样，通常情况也是$f \circ g \neq g \circ f$。因此$f$和$g$的合成的*序*是必不可少的。

令$\varphi$为$g$和$f$的合成，令X为E的任意子集，令Z为G的任意子集。那么我们有

(20) $$\varphi(\mathrm{X}) = g(f(\mathrm{X})),$$
(21) $$\overset{-1}{\varphi}(\mathrm{Z}) = \overset{-1}{f}(\overset{-1}{g}(\mathrm{Z})).$$

如果 $f$ 是 E *onto* F 的*一对一* 映射，并且如果 $g$ 是 F *onto* G 的*一对一* 映射，则 $g \circ f$ 是 E *onto* G 的*一对一* 映射。

令 $h$ 为 G 到集合 H 的映射。然后我们有

$$h \circ (g \circ f) = (h \circ g) \circ f;$$

E入H的这个映射写为$h \circ g \circ f$，称为这个序中三个映射$h$、$g$、$f$的*合成*。三个以上映射的合成的定义类似。

如果$f$是E到自身的映射，$f$的*迭代*被定义为E到自身的映射$f^n$($n$整数$\geqslant 1$)，由$n$上的归纳定义关系$f^1 = f$、$f^n = f^{n-1} \circ f$； $f^n$ 被称为$f$ 的*n 次迭代*。我们有$f^{m+n} = f^m \circ f^n$。

12. 一般来说，映射$f$的逆扩张和扩张的合成$\overset{-1}{f} \circ f$不是$\mathfrak{P}(\mathrm{E})$的恒等映射自身。同样，$f \circ \overset{-1}{f}$通常不是$\mathfrak{P}(\mathrm{E})$的恒等映射自身。仅当$f$是E到F上的*双射*时，这两个条件才能同时满足。

如果$f$是E到F上的双射，并且如果$g$表示$f$的逆，那么合成、$g \circ f$和$f \circ g$分别是E到E上的恒等映射和F到F上的恒等映射。

相反，如果$f$是E到F的映射，并且F到E的$g$映射，使得$g \circ f$是E的置换，$f \circ g$是F的置换，则$f$是E到F的双射，并且$g$ 是 F 到 E 的双射。

此外，如果$g\circ f$是E在其自身上的恒等映射，则$g$是$f$的逆。

13. 设$f$为E到F的映射，并令A为E的任意子集。A到F的映射$f_A$，其中值在A的任意元素$x$处为$f(x)$称为*$f$至子集A*的限制；它只是$f$的合成和A的典范映射进入E。如果E到F的两个映射$f$，$g$对A具有相同的限制，则称它们在A上*同意（或重合）*。反之， $f$ 据说是 $f_A$ 到 E 的 *扩张*。

14. 集合 E *到* 集合 F 的映射也称为 F *通过* E 的*参数表示*；那么E就被称为这个表示的*参数集合*，E的元素取*参数*的名称。

集合 F 的元素* 家族由 F 的定义子集赋予参数表示；在其他字中，被赋予F的元素家族，相当于将一些集合E的映射赋予F。这个映射下的E的像称为家族*的元素的*集合。 注 F 的元素的两个不同家族可能具有与其元素的集合相同的 F 子集。

对于集合 F 的每个子集 A，我们总是可以将元素的族关联起来，其元素的集合是 A。将 A 的 *典范映射* 定义的族考虑到 F 就足够了。

F 的元素系列，由集合 I 的映射 $\iota\mapsto x_\iota$ 定义到 F 中，用 $(x_\iota)_{\iota\in I}$ 表示，或者如果指标集合不存在歧义，则简单地表示为 $(x_\iota)$。

如果J是I的子集，则$(x_\iota)_{\iota\in J}$族被称为$(x_\iota)_{\iota\in I}$族J的*亚族*相应的；它由限制到映射$\iota\mapsto x_\iota$的J定义。
