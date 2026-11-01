---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 1
section_title: Terms and relations
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 15-23, 56
pdf_pages: 0022-0030, 0063-0063
extraction: ocr
subsections:
    - "no": 1
      title: SIGNS AND ASSEMBLIES
      page: 15
      pdf_page: 22
    - "no": 2
      title: CRITERIA OF SUBSTITUTION
      page: 18
      pdf_page: 25
    - "no": 3
      title: FORMATIVE CONSTRUCTIONS
      page: 19
      pdf_page: 26
    - "no": 4
      title: FORMATIVE CRITERIA
      page: 21
      pdf_page: 28
statements: 5
exercises: 6
content_sha256: e27911f3f8706a6b208b062fd5fd57e720041cec01b0d9c1bb938ed8b1fe631f
translated_from: content/en/ens/I/01_s1_terms_and_relations.md
translation_method: google
source_content_sha256: cd4507767925ae07bcbde55aafd18fbe43b41682f9a57932503a95e444fb0094
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: ced26081c1530b300184f98546ffe744a9b90e1184c1081c1e6acdab52a8653c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 项与关系

### 1. 符号与组合

数学理论$\mathscr{T}$[^1]的*符号*如下：

(1) *逻辑符号*[^2]：$\square$、$\tau$、$\vee$、$\neg$。
(2) *字母*。

我们所说的字母是指大写和小写罗马字母，带或不带重音符号。因此 $A$、$A'$、$A''$、$A'''$、... 是字母。在文本的任何地方都可以引入除先前论证中出现的字母之外的字母。

(3) *具体标志*，取决于所考虑的理论。

在集合论中，我们将仅使用以下三个特定符号：$=$、$\in$、$\supset$。

$\mathscr{T}$中的*集合*是一系列$\mathscr{T}$的符号写在一个另一个旁边；除字母外，某些符号可以通过线上方的条线连接到对，称为*链接*。 \*对于例，在集合论中，其中$\in$是一个特定的符号，

$$\overline{\overline{\tau \vee \neg \in \square} A' \in \square} A''$$

是一个程序集。\*

单独使用组合会给印刷者和读者带来难以克服的困难。因此，当前文本使用缩写符号（特别是普通语音的字），而不使用属于至形式数学。此类符号的引入就是*定义*的目的。它们的使用“对于理论来说并不是必不可少的”，并且常常会导致混乱，而只有对主题有一定的熟悉程度才能使读者避免这种混乱。

*例*

#### 例 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

集合$\vee 1$由$\Rightarrow$表示。

#### 例 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

以下符号代表组合 （以及非常长的符号）：

“3和4”

$$\varnothing$$

$$\mathbf{N}$$

$$\mathbf{Z}$$

“实直线”

“$\Gamma$函数”

$$f\circ g$$

$$\pi=\sqrt{2}+\sqrt{3}$$

$$1\in 2$$

“每个有限除法环都是域”

“$\zeta(s)$中除了$-2$、$-4$、$-6$、...之外的零都位于$R(s)=1/2$线上。”

一般来说，用来表示程序集的符号包含程序集中出现的所有字母。然而，这个原理可以被侵犯有时，而不会产生混淆的风险。 *对于例，“X的完成”代表着包含字母X的集合，但也代表包含字母，代表X制服结构随行人员的集合。另一方面，

$$\int_0^1 f(x)\,dx$$

表示字母$x$（和字母$d$）未出现的程序集；而$\mathbf{N}$、$\mathbf{Z}$代表的组合，“$\Gamma$函数”不包含包含任何字母。*

*数学理论*（或简称为*理论*）包含规则允许我们断言某些组合符号是理论的*项或关系*，以及其他规则允许我们断言某些组合是理论的*定理*。

这些规则中的描述，会出现在这个章中，*不会出现属于到形式数学*；规则涉及组合或多或少是未确定的，对于例未确定的字母。为了简化说明，用不太麻烦的符号来表示这样的组合是很方便的。我们将特别使用（数学理论的）符号、粗体斜体字母（有或没有指标或重音符号）以及特定符号的组合，其中将给出一些例。 *由于我们的目的只是为了避免迂回*（cf.注（*），§ 3, no. 1，p. 28），我们不会对这些符号的使用阐明严格的一般规则；在每种特定情况下，读者将能够轻松地重建所讨论的组件。通过滥用语言，我们经常会说符号*是*组合，而不是它们*表示*组合：因此，在以下规则的叙述中，诸如“程序集$A$”或“字母$x$”之类的表达应替换为“由$A$表示的程序集”或“ $x$”表示的字母。

令$A$和$B$为组合。我们将用$AB$表示通过在程序集$A$右侧写入程序集$B$而获得的程序集。我们用$\vee A\neg B$表示通过从左到右书写符号$\vee$、集合$A$、符号$\neg$、集合$B$而获得的集合。等等。

令 $A$ 为集合，令 $x$ 为字母。我们将用$\tau_x(A)$表示构造如下的程序集：形式程序集$\tau A$，将$A$中每个出现的$x$链接到写在$A$左侧的$\tau$，然后通过符号将替换$x$链接到它出现的所有地方$\square$。因此，由 $\tau_x(A)$ 表示的组件*不包含* $x$。

#### 例 {#ens-i-s1-n1-exa-3 .statement tag=03RY}

符号$\tau_x(\in xy)$代表装配

$$
\tau\in\square y.
$$

令$A$和$B$为组合，并令$x$为字母。由替换$x$获得的程序集，无论它出现在$A$中的任何位置，由程序集$B$表示为$(B\mathbin{|}x)\,A$（读作：$A$中的$B$替换$x$）。如果$x$没有出现在$A$中，则$(B\mathbin{|}x)\,A$与$A$相同；特别是，

$$
(B\mathbin{|}x)\,\tau_x(A)
$$

与$\tau_x(A)$相同。

#### 例 {#ens-i-s1-n1-exa-4 .statement tag=03TO}

如果我们将替换$x$除以$\square$，只要$x$出现在程序集$\vee\in xy=xx$中，我们就获得程序集$\vee\in\square y=\square\square$。

如果$A$是一个集合，并且我们对字母$x$特别感兴趣，或者两个不同的字母$x$和$y$（可能会也可能不会出现在$A$中），我们通常会写$A\{x\}$或$A\{x,y\}$。在这种情况下，我们写 $A\{B\}$ 而不是 $(B\mathbin{|}x)\,A$。我们用$A\{B,C\}$表示*同时*替换$x$用$B$和$y$用$C$获得的装配，无论它们出现在$A$中（注，$x$和$y$可能出现在$B$ 和$C$）；如果$x'$和$y'$是不同的字母，$x$和$y$除外，它们既没有出现在$A$，$B$，也没有$C$中，那么$A\{B,C\}$与$(B\mathbin{|}x')(C\mathbin{|}y')(x'\mathbin{|}x)(y'\mathbin{|}y)A$相同。

#### 注 {#ens-i-s1-n1-rem-1 .statement tag=03P2}

当通过定义引入缩写符号$\Sigma$来表示某个程序集时，（通常是默认的）约定是用程序集$B$替换原程序集中的字母$x$得到的程序集，用替换中的字母$x$得到的符号来表示。 $\Sigma$ 由程序集 $B$（或者更常见的是，由表示程序集 $B$ 的缩写符号）。

¶ *对于例，定义了符号$E\otimes F$代表什么程序集，其中$E$和$F$是字母——顺便说一句，包含除了$E$和$F$之外还有其他字母——符号$Z\otimes F$可以使用，无需进一步解释。*

¶ 该规则可能会导致混乱，可以通过使用各种印刷设备来避免；最公共的由$(B)$代替$B$由替换$x$组成。

¶ *对于例，$M\cap N$ 表示程序集包含字母 $N$。如果我们用 $P\cup Q$ 表示的程序集替换 $N$，我们会得到由 $M\cap(P\cup Q)$ 表示的程序集。*

### 2. 代换判据

形式数学包含仅明确写为组合。然而，即使使用缩写符号，严格按照这个原理发展数学也会导致推理的链条非常长。为此，我们应建立与不确定的组合相关的判据；这些判据中的每一个都将一次性描述对这些组合进行确定的序列操作的最终结果。因此，这些判据对于理论来说并不是必不可少的；他们对元数学的辩护属于。

元数学本身的发展在实践中需要使用缩写符号，其中一些已经被指出。大多数这些符号也用于数学中。

我们将使用以下判据，称为 *代换判据* ：

CS1。令$A$和$B$为组合，并令$x$和$x'$为字母。如果$x'$没有出现在$A$中，则$(B|x)A$与$(B|x')(x'|x)A$相同。

CS2。令$A$、$B$和$C$为组合，并令$x$和$y$为不同的字母[^3]。如果$y$没有出现在$B$中，则$(B|x)(C|y)A$等同于

$$(C'|y)(B|x)A,$$

其中 $C'$ 是集合 $(B|x)C$。

CS3。 *设$A$为集合，$x$和$x'$为字母。如果 $x'$ 没有出现在 $A$ 中，则 $\tau_x(A)$ 与 $\tau_{x'}(A')$ 相同，其中 $A'$ 是程序集 $(x'|x)\,A$。*

CS4。 *令$A$和$B$为组合，并让$x$和$y$为不同的字母。如果 $x$ 没有出现在 $B$ 中，则 $(B|y)\tau_xA$ 与 $\tau_x(A')$ 相同，其中 $A'$ 是程序集 $(B|y)\,A$。*

CS5。 *令$A$、$B$、$C$为组合，并令$x$为字母。 组合 $(C|x)(\neg A)$、$(C|x)(\vee AB)$、$(C|x)(\Rightarrow AB)$、$(C|x)(sAB)$（其中$s$为特定符号）分别与$\neg A'$、$\vee A'B'$、$\Rightarrow A'B'$、$sA'B'$相同，其中$A'$、$B'$分别为$(C|x)\,A$、$(C|x)\,B$。*

作为例，让我们表示CS2验证的原理。比较将我们从 $A$ 到 $(B|x)(C|y)\,A$ 的运算与将我们从 $A$ 到 $(C|y)(B|x)\,A$ 的运算。在每个运算中，$A$中出现的且与$x$和$y$不同的符号没有改变。在$A$中出现$x$的每个地方，我们都必须在第一个运算中用$B$替换$x$；对于第一个运算，这一点很明显，而对于第二个$y$，它没有出现在$B$中。最后，在$A$中出现$y$的每个地方，第一个运算包含在替换中，$C$代表$y$，然后在$x$出现在$C$中的每个地方，$B$代表$x$；但很明显，这与替换 $y$ 是一样的，无论它出现在 $A$ 中，还是程序集 $(B|x)\,C$。

### 3. 形成性构造

理论的一些具体标志称为“关系性”，其他则称为“实质性”。每个特定的标志都与自然数相关联，称为 *权* （实际上总是数 2）。

¶ 如果一个程序集以 $\tau$ 开头，或以实数符号开头，或由单个字母组成，则称该程序集属于 *first 类*；否则它是*第二个类*。

¶ $\mathscr{T}$ 理论中的*形成性构造* 是组合的序列，它具有以下性质：对于序列的每个组件$A$，满足以下条件之一：

(a) $A$ 是一个字母。

(b) 在序列中存在第二个类的集合$B$，其位于$A$之前，使得$A$是$\neg B$。

(c) 第二个类（无论是否不同）有两个组合、$B$和$C$，位于$A$之前，使得$A$是$\vee BC$。

(d) 在 $A$ 之前存在第二个类的集合 $B$，以及字母 $x$，使得 $A$ 为 $\tau_x(B)$。

(e) $\mathscr{T}$ 中存在权 $n$ [^4] 的特定符号$s$，以及第一个类的$n$ 组合 $A_1,A_2,\ldots,A_n$，位于 $A$ 之前，使得$A$ 是 $sA_1A_2\ldots A_n$。

出现在 $\mathscr{T}$ 的构成构造中的第一个类的组合（分别为第二个类）在 $\mathscr{T}$ 中称为项（分别为关系）。

#### 例 {#ens-i-s1-n3-exa-1 .statement tag=077Q}

*在集合论中，其中$\in$是权2的关系符号，组合的后续序列是形成构造：*

$$
\begin{array}{c}
A\\
A'\\
A''\\
\in AA'\\
\in AA''\\
\neg\in AA'\\
\vee\neg\in AA'\in AA''
\\[2pt]
\tau\vee\neg\in\square A'\in\square A''
\end{array}
$$

因此，no. 1中给出的例的装配是集合论中的项。*

#### 注 {#ens-i-s1-n3-rem-1 .statement tag=077R}

直观上，项是组合，代表对象，关系是组合，代表断言，可以由这些对象组成。 条件(a)表示字母代表对象。 条件 (b) 意味着如果$B$ 是断言，则$\neg B$（称为$B$ 的否定）是断言（读作：不是$B$）。 条件 (c) 表示如果$B$ 和$C$ 是断言，则$\vee BC$（称为$B$ 和$C$ 的或）是断言（读作：$B$ 或$C$）；因此$\neg\to BC$是断言（在字中：“要么不是$B$，要么$C$”，或者“$B$意味着$C$”）。 条件(d)意味着如果$B$是断言并且$x$是一个字母，那么$\tau_x(B)$是一个对象。让我们将断言$B$视为对象$X$的性质的表达；那么，如果存在一个具有性质的对象，$\tau_x(B)$ 代表一个具有该性质的杰出对象；如果不是，$\tau_x(B)$代表一个无话可说的对象。最后，条件(e)意味着如果$A_1,A_2,\ldots,A_n$是对象，并且如果$s$是权$n$的关系（或实数）符号，那么$sA_1A_2\ldots A_n$关于对象是断言 $A_1,\ldots,A_n$（分别取决于$A_1,\ldots,A_n$的对象）。

#### 例 {#ens-i-s1-n3-exa-2 .statement tag=0E3Y}

符号$\varnothing$、$\mathbf{N}$、“实直线”、“$\Gamma$函数”、$f\circ g$代表项。符号$\pi=\sqrt{2}+\sqrt{3}$、$1\in2$、“每个有限除法环都是域”、“除了$-2$、$-4$、$-6$、...之外的$\zeta(s)$的零位于直线$\mathfrak{R}(s)=1/2$上”表示关系。符号“3和4”既不代表项，也不代表关系。

关系的初始符号是$\vee$、$\neg$或关系符号。 项的初始符号是 $\tau$ 或实数符号，前提是项不由单个字母组成。后者断言源自项是第一个类的集合。如果$A$是关系，那么$A$具有构成构造的特征，不是字母，并且不以$\tau$开头，因此可能出现三种情况： (1) $A$前面有一个集合$B$，使得$A$是$\neg B$； (2) $A$前面有两个组合、$B$和$C$，使得$A$等于$\vee BC$； (3) $A$前面有组合$A_1$、$A_2$、...$A_n$，使得$A$是$sA_1A_2 ... A_n$，$s$是关系符号。

### 4. 形成性判据

CF1。如果$A$和$B$在理论$\mathscr{T}$中是关系，则$\vee AB$在$\mathscr{T}$中是关系。

考虑两个形成的构造（在$\mathscr{T}$中），其中一个包含$A$，另一个$B$。考虑通过先写入第一个构造的组合，然后写入第二个构造的组合，最后写入$\vee AB$来获得组合的序列。由于$A$和$B$属于第二个类，所以立即验证这个序列是$\mathscr{T}$的构成构造。集合$\vee AB$是第二个类的集合，因此它是$\mathscr{T}$中的关系。

以下三个判据的建立方式类似：

CF2。如果$A$在理论$\mathscr{T}$中是关系，则$\neg A$在$\mathscr{T}$中是关系。

CF3。如果$A$在理论$\mathscr{T}$中是关系，并且如果$x$是字母，那么$\tau_x(A)$在$\mathscr{T}$中是项。

CF4。如果 $A_1$、$A_2$、...、$A_n$ 是理论 $\mathscr{T}$ 中的项，并且如果 $s$ 是 $\mathscr{T}$ 中权 $n$ 的关系（或实数）符号，则$sA_1A_2...A_n$ 是$\mathscr{T}$ 中的关系（分别为项）。

这些判据立即意味着以下内容：

CF5。如果$A$和$B$在理论$\mathscr{T}$中是关系，则$\Longrightarrow AB$在$\mathscr{T}$中是关系。

CF6。令$A_1$、$A_2$、...、$A_n$为理​​论$\mathscr{T}$中的形成构造，并令$x$和$y$为字母。假设$y$没有出现在任何$A_i$中。那么$(y|x) A_1$、$(y|x) A_2$、...、$(y|x) A_n$ 是$\mathscr{T}$ 中的构成构造。

为了证明 CF6，令 $A_i'$ 为集合 $(y|x)A_i$。如果$A_i$是一个字母，那么$A_i'$也是一个字母。如果$A_i$属于形式$\neg A_j$，其中$A_j$是构造中位于$A_i$之前的第二个类的集合，则$A_i'$与CS5中的$\neg A_j'$相同，并且$A_j'$是组装第二个类。如果$A_i$是形式$\vee A_jA_k$或$sA_{j_1}A_{j_2}\ldots A_{j_m}$，推理是类似的，$s$是$\mathscr{T}$的特定符号。如果最终$A_i$是形式$\tau_z(A_j)$，其中$A_j$是构造中位于$A_i$之前的第二个类的集合，则需要考虑多种情况：

(a) $z$ 是一个不同于 $x$ 和 $y$ 的字母。那么$A_i'$与CS4中的$\tau_z(A_j')$相同，$A_j'$是第二个类的集合。

(b) $z$ 与 $x$ 相同。那么$A_i$不等于包含$x$，因此$A_i'$与$A_i$相同，也就是说与$\tau_x(A_j)$相同；由于$y$没有出现在$A_j$中，所以$\tau_x(A_j)$与CS3中的$\tau_y(A_j)$相同。

(c) $z$ 与$y$ 相同。那么$A_i$就是集合$\tau A_j$，因为$y$没有出现在$A_j$中；因此$A_i'$是$\tau A_j'$的集合，即$\tau_u(A_j')$，其中$u$是$A_j'$中没有出现的字母。

CF7。 *在理论$\mathscr{T}$中，令$A$为关系（分别为项），并令$x$和$y$为字母。那么 $(y|x)A$ 就是 $\mathscr{T}$ 中的关系（或项）。*

令 $A_1,A_2,\ldots,A_n$ 为形成构造，其中出现$A$。我们将逐步证明，如果$A_i$是关系（分别是项），那么$(y|x)A_i$（我们用$A_i'$表示）也是关系（分别是项）。假设这个点已经为$A_1,A_2,\ldots,A_{i-1}$成立；让我们证明$A_i$。如果$A_i$是一个字母，那么$A_i'$也是一个字母。如果构造中$A_i$位于关系$A_j$之前，使得$A_i$等于$\neg A_j$，则$A_i'$与CS5中的$\neg A_j'$相同，并且$\neg A_j'$与CF2中的关系相同。如果 $A_i$ 前面有关系 $A_j,A_k$，使得 $A_i$ 是 $\vee A_jA_k$，或者如果 $A_i$ 前面有项 $A_{j_1},\ldots,A_{j_m}$，使得 $A_i$ 是 $sA_{j_1}\cdots A_{j_m}$，则参数类似，其中$s$是权$m$的$\mathscr{T}$的特定符号。最后，如果$A_i$前面是关系$A_j$，使得$A_i$是$\tau_z(A_j)$，则需要考虑多种情况：

(a) $z$ 不同于 $x$ 和 $y$。那么$A_i'$与CS4中的$\tau_z(A_j')$相同，并且我们已经知道$A_j'$是关系；因而，根据 CF3，$A_i$ 为项。

(b) $z$ 与 $x$ 相同。那么 $A_i$ 不等于包含 $x$，因而 $A_i'$ 与 $A_i$ 相同，因此是项。

(c) $z$ 与$y$ 相同。然后令$u$为一个字母，与$x$和$y$都不同，它不会出现在$A_1,A_2,\ldots,A_j$中。通过CF6，组合$(u|y)A_1,\ldots,(u|y)A_j$的序列（我们用$A_1'',\ldots,A_j''$表示）构成了$\mathscr{T}$中的构成构造。由于$y$不再出现在这个新的构造中，$(y|x)A_1'',\ldots,(y|x)A_j''$是CF6形成的构造，所以$(y|x)A_j''$是$\mathscr{T}$中的关系；因而 $\tau_u((y|x)A_j'')$ 是 $\mathscr{T}$ 的项。但是这个项与CS4的$(y|x)\tau_u(A_j'')$相同，因此与CS3的$(y|x)\tau_y(A_j)$相同，因此与$A_i$相同。

CF8。令$\mathscr{T}$中的$A$为关系（或项），令$x$为字母，$\mathscr{T}$中的$T$项。那么$(T|x)A$在$\mathscr{T}$中就是关系（分别是项）。

令 $A_1, A_2, \ldots, A_n$ 为形成构造，其中出现$A$。令 $x_1, x_2, \ldots, x_p$ 为$T$ 中出现的不同字母。让我们将每个字母$x_i$与一个字母$x_i'$关联起来，与每个字母$x_1, \ldots, x_p$和$A_1, \ldots, A_n$中出现的字母不同，这样字母$x_1', \ldots, x_p'$都是不同的。大会

$$
(x_1'|x_1)(x_2'|x_2)\ldots(x_p'|x_p)T
$$

CF7 为项 $T'$，$(T|x)A$ 与

$$
(x_1|x_1')(x_2|x_2')\ldots(x_p|x_p')(T'|x)A
$$

通过应用CS1。因而，只要证明 $(T'|x)\,A$ 是关系（或项）即可；在其他字中，我们可以假设从现在起$T$中出现的字母不会出现在$A_1, \ldots, A_n$中。

¶ 我们将逐步证明，如果$A_t$是关系（分别是项），那么$(T|x)\,A_t$（我们将用$A_t'$表示）是关系（分别是项）。假设对于$A_1,A_2,\ldots,A_{i-1}$这个点已经成立，让我们对$A_i$证明它。如果$A_i$是一个字母，那么$A_i'$要么是同一个字母，要么是$T$，因此项。如果$A_i$是形式$\neg A_j$，其中$A_j$是关系，在构造中它在$A_i$之前，那么$A_i$与CS5中的$\neg A_j'$相同，并且我们已经知道$A_j'$是关系，因而 $A_i'$ 通过 CF2 等于关系。如果 $A_i$ 是形式 $\vee A_jA_k$ 或 $sA_{j_1}\ldots A_{j_m}$，证明是类似的。最后，如果$A_i$是形式$\tau_z(A_j)$，其中$A_j$是关系，并且在构造中先于$A_i$，则需要考虑多种情况：

(a) $z$ 不同于$x$ 以及$T$ 中出现的字母。那么$A_i'$与CS4中的$\tau_z(A_j')$相同，并且我们已经知道$A_j'$是关系；因此CF3 $A_i'$ 是项。

(b) $z$ 与$x$ 相同。那么 $A_i$ 不会包含 $x$，因而 $A_i'$ 与 $A_i$ 相同，因此是项。

(c) $z$ 出现在 $T$ 中。那么$z$不会出现在$A_j$中，因而$A_i'$与$\tau A_j'$相同；因而 $A_i'$ 与 $\tau A_j'$ 相同。现在，我们已经知道$A_j'$是关系，$\tau A_j'$与$\tau_u(A_j)$相同，其中$u$是$A_j$中没有出现的字母；由CF3可知$A_i'$是项。

直观上，如果$\mathscr{T}$中$A$是关系，我们可以将其视为表达对象$x$的性质，断言$(B|x)\,A$相当于说，对象$B$有这个性质。如果$A$在$\mathscr{T}$中是项，则它表示一个对象在某种程度上依赖于$x$表示的对象； 项$(B|x)\,A$表示当我们将$x$作为对象$B$时，对象$A$会变成什么。

### 习题{#ens-i-s1-exercises}

参见[习题为 § 1](exercises/s1/)。

[^1]: The meaning of this expression will become clear as the chapter progresses.
[^2]: For the intuitive meanings of these signs, see no. 3, Remark.
[^3]: In accordance with what was said in no. 1, the phrase “$x$ and $y$ are distinct letters” is an abuse of language: it means that $x$ and $y$ denote distinct letters in the assemblies under consideration.
[^4]: As was said above, it would be possible, for the development of present-day mathematical theories, to limit our consideration to specific signs of weight 2, and consequently to avoid using the expression “natural number $n$” in the definition of a formative construction.
