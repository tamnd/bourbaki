---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 9
section_title: Radical
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.151-A VIII.172
pdf_pages: 0168-0189
extraction: native
subsections:
    - "no": 1
      title: The Radical of a Module
      page: 151
      pdf_page: 168
    - "no": 2
      title: The Radical of a Ring
      page: 154
      pdf_page: 171
    - "no": 3
      title: Nakayama’s Lemma
      page: 158
      pdf_page: 175
    - "no": 4
      title: Lifts of Idempotents
      page: 159
      pdf_page: 176
    - "no": 5
      title: Projective Cover of a Module
      page: 161
      pdf_page: 178
statements: 49
exercises: 31
content_sha256: 25713c0d37a965a01b409d7b6b45b0ce4c6749ab5d76db4ff11cf02f99fcef28
translated_from: content/en/alg/VIII/09_s9_radical.md
translation_method: google
source_content_sha256: 89095724e574bba079cd13ef874a02941adc59513c6a22e5a09bd9f01b4fa6cc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 3779351546ac5f2df18af6b9b9123ba1b43e515ebde4b94bd13acf05cc41b9db
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 9。激进

### 1.模的根

#### 定义 1 {#alg-viii-s9-def-1 .statement tag=00A1}

设 A 为环。 A-模 M 的根部子模定义为 M 的极大子模的交 (VIII, p. 48, 定义 2)，或等价地，M 的元素的集合被每个湮没同态从M到单A-模。

在这个章的其余部分，我们用$\mathfrak{R}_A(M)$或简称为$\mathfrak{R}(M)$来表示A-模M的根部。

设 A 为环。当且仅当存在单A-模的族$(S_i)_{i\in I}$和A-线性映射$f_i: M\rightarrow S_i$的$(f_i)_{i\in I}$族，使得我们有$\cap_{i\in I}$Ker($f_i$)时，A-模M的部首减少到0（在这种情况下，滥用语言，我们说M没有部首） $= 0$。这相当于 M 同构于子模或乘积或单A-模。

#### 例 1 {#alg-viii-s9-n1-exa-1 .statement tag=00A2}

令$\mathfrak{a}$为A的左理想。A-模$A_s/\mathfrak{a}$的根式等于$\mathfrak{a}'/\mathfrak{a}$，其中$\mathfrak{a}'$是包含$\mathfrak{a}$的最大左理想的交。特别是，对于每个素数数 $p$ 和每个整数 $n\geqslant 1$，$\mathbf{Z}$-模 $\mathbf{Z}$ 的根式被约化为 0，而 $\mathbf{Z}$-模 $\mathbf{Z}/p^n\mathbf{Z}$ 的根式等于 $p\mathbf{Z}/p^n\mathbf{Z}$。

#### 例 2 {#alg-viii-s9-n1-exa-2 .statement tag=00A3}

设 A 为主理想整环，它不是域，并令 K 为分数的域。当K-模时，K没有根式。让我们证明K的根式A-模等于K；等价地，我们必须证明从K到单A-模S的每个A-线性映射$f$都是零。通过VII, §4, No. 8，p. 25，我们可以假设S等于$A/(\pi )$，其中$\pi$是A的不可约元。对于每个$x\in K$，我们有$f(x) =f(\pi \frac{x}{\pi})=\pi f(\frac{x}{\pi})= 0$，因为$\pi S = 0$。

#### 命题 1 {#alg-viii-s9-prop-1 .statement tag=00A4}

设M和N为从M到N的A-模和$f$同态。我们有$f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$，如果$f$是满射且$f$的核包含在M的根式中，我们甚至还有等式。

设$g$为同态，从N到单A-模；那么$\mathfrak{R}(M)$包含在$g\circ f$的核中，因此$f(\mathfrak{R}(M))$包含在$g$的核中。因此我们有 $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$。现在假设 $f$ 是满射，并且它的核包含在 $\mathfrak{R}(M)$ 中。令$y$为$\mathfrak{R}$(N)的元素，并令$x$为$y$的逆像元素。如果$g$是从M到单A-模S的同态，那么它的核包含是M的根，因此核是$f$。由于同态$f$是满射，因此从N到S存在同态$h$使得$g=h\circ f$。从$y=f(x)$属于到$\mathfrak{R}$(N)，我们有$h(f(x)) = 0$，即$g(x) = 0$；因此$x$属于到$\mathfrak{R}$(M)​​，这证明了包含$\mathfrak{R}(N)\subset f(\mathfrak{R}(M))$。

#### 推论 1 {#alg-viii-s9-prop-1-cor-1 .statement tag=00A5}

设 M 为 M 的 A-模，N 子模。

a) 我们有$\mathfrak{R}(N)\subset \mathfrak{R}(M)\cap N$。

b) 我们有 $(\mathfrak{R}(M) + N)/N\subset \mathfrak{R}(M/N)$。如果 N 包含在 $\mathfrak{R}(M)$ 中，则我们有等式 $\mathfrak{R}(M/N) =\mathfrak{R}(M)/N$。

c) 模 $M/\mathfrak{R}(M)$ 没有部首。如果模$M/N$没有部首，那么我们有$\mathfrak{R}(M)\subset N$。

断言 a) 是从命题 1 应用于典范嵌入，从 N 到 M，断言 b) 是从命题 1 应用于典范映射，从 M 到 $M/N$。从 b) 中，我们推断，如果 $N =\mathfrak{R}(M)$，则 $M/N$ 没有部首；如果 $M/N$ 没有部首，则我们有 $\mathfrak{R}(M)\subset N$。

从例 1 可以得出，可以存在子模 N 包含于 $\mathfrak{R}(M)$，使得$M/N$的根式不是零。

#### 推出 2 {#alg-viii-s9-prop-1-cor-2 .statement tag=00A6}

令$(M_i)_{i\in I}$为A-模的族，P为乘积，S为直和。我们有$\mathfrak{R}(P)\subset \prod_{i\in I}\mathfrak{R}(M_i)$和$\mathfrak{R}(S) =\bigoplus_{i\in I}\mathfrak{R}(M_i)$。

对于$i\in I$，令$\pi_i$为投影，其中指标$i$从P到$M_i$。到命题 1 时，每 $i\in I$ 就有 $\pi_i(\mathfrak{R}(P))\subset \mathfrak{R}(M_i)$；这就证明了第一个断言。我们有$S\subset P$，因而

$$
\mathfrak{R}(S)\subset S\cap \mathfrak{R}(P)\subset S\cap \prod_{i\in I}\mathfrak{R}(M_i) =\bigoplus_{i\in I}\mathfrak{R}(M_i)
$$

此外，对于每个$i\in I$，我们有$M_i\subset S$，因此有$\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$，因此有$\oplus_{i\in I}\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$。

存在模族，使得乘积的部首与部首乘积不同构（VIII、p. 166的习题 3）。

#### 命题 2 {#alg-viii-s9-prop-2 .statement tag=00A7}

令 M 为有限生成A-模。

a) 如果 M 不减少到 0，则我们有 $\mathfrak{R}(M)\not= M$。

b) 如果 N 是 M 的子模，使得 $N +\mathfrak{R}(M) = M$，那么我们有 N = M。

令N为M的真子模。通过VIII、p. 49的命题 3，存在M 包含N的极大子模L。我们有$N +\mathfrak{R}(M)\subset L$和更不必说$N +\mathfrak{R}(M)\not= M$。这证明了 b);具体情况 N = 0 给出断言 a)。

#### 推出{#alg-viii-s9-n1-cor-1 .statement tag=00A8}

设 M 为 M 的 A-模、$(x_i)_{i\in I}$ 生成的族以及 M 的 $x$ 元素。以下属性是等效的：

(i) 我们有 $x\in \mathfrak{R}(M)$。

(ii) M 的每子模 N，使得 $N + Ax= M$ 等于 M。

(iii) 对于 A 的每个家庭 $(a_i)_{i\in I}$ 元素，家庭 $(x_i+a_ix)_{i\in I}$ 生成 A-模 M。

(i) $\Rightarrow$ (ii)：假设 $x$ 属于至 $\mathfrak{R}(M)$。令 N 为 M 的子模，使得 $N + Ax= M$。我们有$N +\mathfrak{R}(M) = M$；因此A-模$M/N$等于命题1的根部（推论1，b）。由于它是单生的，所以它是零 (命题 2)，并且我们有 M = N。

(ii) $\Rightarrow$ (iii)：令$(a_i)_{i\in I}$为A的元素族。用$(x_i+a_ix)_{i\in I}$族生成的M的N子模表示。每 $i\in I$ 就有 $x_i\in N + Ax$，因此有 $N + Ax= M$。如果性质 (ii) 成立，则 N 等于 M。

(iii) $\Rightarrow$ (i)：假设$x$ 不属于到$\mathfrak{R}(M)$。那么 M 中存在极大子模 N 个不存在包含 $x$。由于 N 是最大的，所以我们有 $N + Ax= M$；因而，元素 $x_i$ 中的每一个都可以写成 $y_i-a_ix$、$y_i\in N$ 和 $a_i\in A$。族$(x_i+a_ix)_{i\in I}$包含在N中，因此不包含生成M。

#### 命题 3 {#alg-viii-s9-prop-3 .statement tag=00A9}

a) 半单模没有部首。

b) 模是半单并且是有限生成的当且仅当它没有部首且阿廷的。

到定义，单模的根数就减为0。如果模 M是半单，那么它是简单子模的$(S_i)_{i\in I}$族的直和，由推论2我们有$\mathfrak{R}(M) =\bigoplus_{i\in I}\mathfrak{R}(S_i)$上面命题 1，因而$\mathfrak{R}(M) = 0$。

此外，如果 M 是有限生成的，则它是 VIII、p. 71 的阿廷的 × 命题 10。

相反，假设 M 是阿廷的并且没有根式。将VIII、p. 2应用于M的极大子模的集合，则存在M的极大子模的有限族$(N_i)_{i\in I}$，其交降为0。则M与$\bigoplus_{i\in I}(M/N_i)$的子模同构。因而，它是半单并且有有限长度，并且更不必说是有限生成的。

### 2.环的根

#### 定义 2 {#alg-viii-s9-def-2 .statement tag=00AA}

环 A 的雅各布森根式（或简称根式），用 $\mathfrak{R}(A)$ 表示，是 A-模 $A_s$ 的根式，即 A 的最大左理想的交。

通过滥用语言，如果我们有$\mathfrak{R}(A) = 0$，我们就说环 A 没有部首。

#### 命题 4 {#alg-viii-s9-prop-4 .statement tag=00AB}

环 A 是半单当且仅当它是左阿廷的并且没有根式。

这是从应用于 A-模 $A_s$ 的命题 3, b) 得出的。

#### 例 1 {#alg-viii-s9-n2-exa-1 .statement tag=00AC}

如果A是局部环，那么它有A的不可逆元素的唯一最大左理想$\mathfrak{r}$，由……组成（VIII，p. 25，命题1）；所以$\mathfrak{r}$是A的部首。特别是域没有部首。

#### 例 2 {#alg-viii-s9-n2-exa-2 .statement tag=00AD}

令K为变量$X_i$中形式幂级数的交换域和E代数$K[[X_i]]_{i\in I}$，系数在K中。通过之前VIII、p. 26的例和例4，E的根式由形式组成幂级数与常数项零。观察环 E 是整环并且它的根式没有减少到0，甚至虽然 E 是分数的域的子环，没有根式。

#### 例 3 {#alg-viii-s9-n2-exa-3 .statement tag=00AE}

假设A为主理想整环，设P为不可约元(VII, §1, No. 3，p. 3)的代表由……组成的系统。若A为域，则例1无根。若集合P无限，则A的最大理想$Ap$的交减至0，故A无根。但如果 P 是有限的并且非空，并且如果我们集合 $x=\prod_{p\in P}p$，那么 A 的根式等于 $\cap_{p\in P}Ap= Ax$ (VII, §1, No. 2，p. 3，命题 4)，因此不会减少到 0。

设$y$为A的非零元素；我们将其写为$y=up^{i_1}_1\cdots p^{i_r}_r$，其中$u$在$A,p_1, . . . , p_r$中是可逆的，与P的成对不同的元素，并且$i_1, . . . , i_r$严格是正整数。 环 $A/Ay$ 的最大理想为$Ap_1/Ay, . . . ,Ap_r/Ay$；因此环$A/Ay$的部首是理想的$Ap_1\cdots p_r/Ay$。 特别是，当且仅当我们有 $i_1=\cdots =i_r= 1$ 时，环 $A/Ay$ 才没有根式；在这种情况下，我们说 $y$ 没有倍数因子。

#### 命题 5 {#alg-viii-s9-prop-5 .statement tag=00AF}

a) 环的根 A 为单A-模湮没子交；也是半单A-模的最小的湮没子。特别是，它是 A 的双面理想。如果 A 不减少到 0，则 A 的根式与 A 不同。

b) 设$\mathfrak{a}$为A的双面理想。我们有$(\mathfrak{R}(A) +\mathfrak{a})/\mathfrak{a}\subset \mathfrak{R}(A/\mathfrak{a})$。如果$\mathfrak{a}$包含在$\mathfrak{R}(A)$中，那么我们有$\mathfrak{R}(A/\mathfrak{a}) =\mathfrak{R}(A)/\mathfrak{a}$。

c) 环 $A/\mathfrak{R}(A)$ 没有部首；反之，A 的每个双面理想 $\mathfrak{a}$ 使得 $A/\mathfrak{a}$ 没有根式包含 $\mathfrak{R}(A)$。

d) A 的根式包含在 A 的最大双面理想的交中。

让$x\in A$。 Saying that $x$ belongs to the annihilator of every simple A-module is equivalent to saying that $x$ belongs to the annihilator of every element of every simple A-module, in other words (VIII, p. 46, Proposition 1), to every maximal left ideal of A.

令 M 为半单A-模。其湮没子是M的简单子模湮没子交，所以它包含$\mathfrak{R}(A)$。此外，如果$\mathscr{S}$是单A-模(VIII，p. 51)的类的集合，则直和$\oplus_{\lambda\in\mathscr{S}}\lambda$是半单A-模，其中湮没子是$\mathfrak{R}(A)$。假设A没有减少到0； 关系$\mathfrak{R}(A)\not= A$源自命题2，VIII的a)，p. 153应用于A-模$A_s$。我们已经证明了a）。

令$\mathfrak{a}$为A的两侧理想。$A/\mathfrak{a}$的最大左理想是形式$\mathfrak{m}/\mathfrak{a}$的理想，其中$\mathfrak{m}$是包含$\mathfrak{a}$的最大左理想。因而，环$A/\mathfrak{a}$的根式等于A-模$A_s/\mathfrak{a}$的根式。因而，断言 b) 和 c) 由VIII、p. 152 的推论 1 得出。

令$\mathfrak{a}$为A的最大双边理想。在环$A/\mathfrak{a}$中，唯一的双边理想是0和$A/\mathfrak{a}$。由于环 $A/\mathfrak{a}$ 未减至 0，因此其根式不等于 $A/\mathfrak{a}$。因此环 $A/\mathfrak{a}$ 没有根式，并且由 c) 得到 $\mathfrak{R}(A)\subset \mathfrak{a}$。这就证明了d）。

如果 A 的左（或右）理想由幂零元组成，我们就说它是零理想。我们说 A 的双面理想 $\mathfrak{a}$ 是幂零的，如果存在整数 $n\geqslant 1$ 使得 $\mathfrak{a}^n= 0$，即 (I, §8, No. 9, p. 107)，使得对于元素的每个序列 $(x_1, . . . , x_n)$ 都有$x_1\cdots x_n= 0$ $\mathfrak{a}$。每个幂零双面理想都是零理想，但是可以存在不包含在幂零双面理想中的零理想（VIII，p. 167，习题 9）。

#### 定理 1（雅各布森）{#alg-viii-s9-thm-1 .statement tag=00S5}

环的根 A 由元素 $x\in A$ 组成，使得对于每个 $a\in A$，$1 +ax$ 是可逆的（I, §2, No. 3，p. 15）。它也是最大的双面理想$\mathfrak{a}$，使得$1 +x$对于每个$x\in \mathfrak{a}$都是可逆的。 A 的包含左零理想的根式。

元素 1 生成 A-模 $A_s$，且$1 +ax$可逆当且仅当生成A-模$A_s$。因而，定理 1 的第一个断言是命题 2 (VIII，p. 153)推论的特例。

让$x\in \mathfrak{R}(A)$。由上可知，$1 +x$是可逆的；令$y$为A的元素，使得$y(1 +x) = 1$。然后我们有$1-y=yx$，所以$1-y$属于到$\mathfrak{R}(A)$；因而，$y$ 是可逆的。由于$y$也是右可逆的，因此它是可逆的（I, §2, No. 3，p. 16，命题3），它的右逆$1 +x$也是可逆的。

令$\mathfrak{a}$为A的左理想，使得$1 +x$对于每个$x\in \mathfrak{a}$都是可逆的。对于例，当$\mathfrak{a}$为零理想时，这是成立的，因为关系$x^n= 0$意味着$1-x+\cdots + (-x)^{n-1}$是$1 +x$的逆。让$x\in \mathfrak{a}$。对于每个$a\in A$，我们有$ax\in \mathfrak{a}$，所以$1 +ax$是可逆的；因而，我们有$x\in \mathfrak{R}(A)$。由此可见，$\mathfrak{a}$包含在$\mathfrak{R}(A)$中。

#### 推论 1 {#alg-viii-s9-thm-1-cor-1 .statement tag=00AG}

A的根等于逆环$A^o$的根，即A的最大右理想的交。

对于每个 $x\in \mathfrak{R}$(A)，$1 +x$ 在环 A 中是可逆的，因此在环 $A^o$ 中。由于$\mathfrak{R}(A)$是$A^o$的双面理想，所以我们有$\mathfrak{R}(A)\subset \mathfrak{R}(A^o)$。 等式之后是交换 A 和$A^o$ 的角色。

#### 推论 2 {#alg-viii-s9-thm-1-cor-2 .statement tag=00AH}

A 的元素是可逆的当且仅当其环 $A/\mathfrak{R}(A)$ 中的典范像可逆。

条件显然是必要的。让我们证明它是足够的。令 $x$ 为 A 的元素，其环 $A/\mathfrak{R}(A)$ 中的典范像可逆。则 A 存在元素 $y$，使得 $xy$ 属于至 $1 +\mathfrak{R}(A)$。 定理 1$,xy$ 可逆；因而 $x$ 是右可逆的。 $x$可逆的证明是类似的。

#### 推论 3 {#alg-viii-s9-thm-1-cor-3 .statement tag=00AI}

环的族$(A_i)_{i\in I}$的乘积的部首是$\mathfrak{R}(A_i)$的乘积。

设$x= (x_i)_{i\in I}$为$\prod_{i\in I}A_i$的元素。对于 $\prod_{i\in I}A_i$ 的每个元素 $a= (a_i)_{i\in I}$，当且仅当对于每个 $i\in I$，$1 +a_ix_i$ 在$A_i$ 中保持可逆，元素 $1 +ax$ 保持可逆。推论 3 如下。

#### 推论 4 {#alg-viii-s9-thm-1-cor-4 .statement tag=00AJ}

环 A 是局部的当且仅当环 $A/\mathfrak{R}(A)$ 是域。如果是这种情况，则 $\mathfrak{R}(A)$ 是 A 的不可逆元素的集合。

将 A 的不可逆元素的集合表示为 $\mathfrak{r}$。如果环 A 是局部的，则其根式等于 $\mathfrak{r}$ (VIII, p. 154, 例 1)，环 $A/\mathfrak{r}$ 域 (VIII, p. 26)。相反，假设环$A/\mathfrak{R}(A)$是域。根据推论 2，我们有 $\mathfrak{r}=\mathfrak{R}$(A)，因此 $\mathfrak{r}$ 是 A 的双面理想。因此环 A 是局部的（VIII，p. 26，定义 1）。

#### 例 4 {#alg-viii-s9-n2-exa-4 .statement tag=00AK}

设 K 为整环、I 非空集合、A 多项式环 $K[X_i]_{i\in I}$。让我们证明环 A 没有根式。 A 的唯一可逆元是 K 的可逆元（IV, §1, No. 5，p. 9，推论 2）。让$f\in \mathfrak{R}(A)$。 选择元素$i\in I$。那么$1 +fX_i$是可逆的（定理1），这意味着$f= 0$。

注当K为交换域时，环$A = K[X_i]_{i\in I}$是$B = K[[X_i]]_{i\in I}$的子环，并且我们有$\mathfrak{R}(A) = 0$和$A\cap \mathfrak{R}(B)\not= 0$（cf.VIII，p. 154，例2）。

#### 例 5 {#alg-viii-s9-n2-exa-5 .statement tag=00AL}

令$\mathfrak{a}$为A的双面理想。A上的$\mathfrak{a}$进数拓扑为拓扑，与A的环结构兼容，其中理想$\mathfrak{a}^n$（对于$n\geqslant 1$）形式是0邻域的基本系统 （Gen.Top.、III, §6, No. 3、p. 275、例 3）。假设环 A 是 Hausdorff 并且对于这个拓扑是完备的 (Gen. Top., III, §6, No. 5, p. 276)；对于例，这是理想的$\mathfrak{a}$幂零时的情况。对于每个 $x\in \mathfrak{a}$，级数 $\sum^{\infty}_{n=0}(-x)^n$ 都会收敛。令$y$为其和。我们有$y-1 =\sum^{\infty}_{n=1}(-x)^n=-xy$，因此有$(1 +x)y= 1$。同样，我们有$y(1 +x) = 1$，所以$1 +x$是可逆的。由定理 1，可知理想的 $\mathfrak{a}$ 包含在 A 的根部中。

#### 注 1 {#alg-viii-s9-n2-rem-1 .statement tag=00AM}

到定理 1 时，环 A 的每个左零理想都包含在

这是激进的。令 $x$ 为 A 的幂零且中心元素；则 $Ax$ 是 A 的零理想，因此 $x$ 属于是 A 的根式。然而，有可能存在 A 的非零幂零元但 A 没有根式。对于例，对于每个整数$n\geqslant 2$，矩阵环$\mathbf{M}_n(K)$超过域K是简单的，因此没有根式（VIII，p. 154，命题4），并且它包含幂零元，对于例矩阵单位 $E_{ij}$ 和 $i\not=j$。

#### 注 2 {#alg-viii-s9-n2-rem-2 .statement tag=00AN}

设A为交换环。 A的幂零元$a$的集合是A的理想$\mathfrak{N}(A)$，称为A的零根；它是A的素理想的交（V, §15, No. 1，p. 118，命题2）。我们有$\mathfrak{N}(A)\subset \mathfrak{R}(A)$； $*$如果A是阿廷环（VIII，p. 173，推论2），或者在交换域上有限生成的交换代数（通信算法，V, § 3，n$^{\circ}4$，定理，我们有等式） $3$)$*$。我们当然可以有$\mathfrak{N}(A)\not=\mathfrak{R}(A)$。这是当 A 为环 K[[X]] 时的情况，其中 K 为交换域：则我们有 $\mathfrak{N}(A) = 0$ 和 $\mathfrak{R}(A) =$ AX (VIII、p. 154、例 2)。

### 3.中山引理

#### 命题 6 {#alg-viii-s9-prop-6 .statement tag=00AO}

对于每 A-模 M，我们有 $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$。如果 A-模 M 是射影的，我们有等式。

令 P 为 M 的极大子模； A-模 $M/P$ 很简单，因此被$\mathfrak{R}(A)$ 被VIII、p. 155 的命题 5 消灭。因此，对于 M 的每个极大子模 P，我们都有$\mathfrak{R}(A)M\subset P$，因此有$\mathfrak{R}(A)M\subset \mathfrak{R}(M)$。

我们显然有$\mathfrak{R}(A_s) =\mathfrak{R}(A)A_s$。如果A-模 M 是射影的，则存在A-模 N 使得$M\oplus N$ 是自由的，即模同构于$A_s$ 的族$(L_i)_{i\in I}$ 的直和。根据VIII、p. 152的推论2，我们有$\mathfrak{R}(M\oplus N) =\mathfrak{R}(M)\oplus \mathfrak{R}(N)$和$\mathfrak{R}(\bigoplus_{i\in I}L_i)=\bigoplus_{i\in I}\mathfrak{R}(L_i)$。然后我们从等式$\mathfrak{R}(L_i) =\mathfrak{R}(A)L_i$推出$\mathfrak{R}(M) =\mathfrak{R}(A)M$。

#### 定理 2（“中山引理”）{#alg-viii-s9-thm-2 .statement tag=00S6}

设 M 为 A-模，$\mathfrak{a}$ A 的两侧理想。假设满足以下条件之一：

(i) A-模 M 是有限生成的，$\mathfrak{a}$ 包含在 A 的根中。

(ii) 理想的 $\mathfrak{a}$ 是幂零的。

如果 N 是 M 的子模，使得 $M = N +\mathfrak{a}M$，则我们有 N = M。特别是，如果模 M 是非零的，则我们有 $M\not=\mathfrak{a}M$。

假设 M 是有限生成的并且我们有 $\mathfrak{a}\subset \mathfrak{R}(A)$。令 N 为 M 的子模，使得 $M = N +\mathfrak{a}M$。到命题 6，我们有 $M = N +\mathfrak{R}$(M)，因此 M = N 乘以命题 2, b) of VIII，p. 153。

现在假设 $\mathfrak{a}$ 幂零，并令 N 为 M 的子模，使得 $M = N +\mathfrak{a}M$。到归纳整数$n\geqslant 0$，我们建立关系$M = N +\mathfrak{a}^nM$。到假设，存在整数$n\geqslant 0$使得$\mathfrak{a}^n= 0$；因此M = N。

定理的最后一个断言由上式得出，取N为0。

#### 推论 1 {#alg-viii-s9-thm-2-cor-1 .statement tag=00R9}

我们保留定理 2 中的假设。令$(x_i)_{i\in I}$ 为M 的元素的家族，并令$\overline{x}_i$ 为$M/\mathfrak{a}M$ 中$x_i$ 的典范像。如果系列 $(\overline{x}_i)_{i\in I}$ 生成 $(A/\mathfrak{a})$-模块 $M/\mathfrak{a}M$，则系列 $(x_i)_{i\in I}$ 生成 A-模 M。

这是从定理 2 应用于由$(x_i)_{i\in I}$族生成的M的子模 N 得出的。

#### 推论 2 {#alg-viii-s9-thm-2-cor-2 .statement tag=00AP}

我们保留定理 2 中的假设。此外，令$M'$ 为A-模，$u: M'\rightarrow M$ 为同态。如果从 $u$ 乘以经过到商推出的从 $M'/\mathfrak{a}M'$ 到 $M/\mathfrak{a}M$ 的同态 $\overline{u}$ 是满射，则 $u$ 是满射。

事实上，$u:$的应用定理2到像N就足够了，$\overline{u}$的像是$(N +\mathfrak{a}M)/\mathfrak{a}M$，所以$\overline{u}$是满射当且仅当我们有$N +\mathfrak{a}M = M$。

### 4.幂等的提升

#### 引理 1 {#alg-viii-s9-lem-1 .statement tag=00AQ}

令 $a$ 为环 A 的元素，使得 $a-a^2$ 幂零。 $X + (X-X^2)\mathbf{Z}[X]$ 中存在多项式 P，使得 $P(a)$ 在 A 中幂等。

令$n$严格为正整数，使得$(a-a^2)^n= 0$。 集合 P(X) = $1-(1-X^n)^n$。多项式P(X)是$X^n$的倍数，多项式$1-P(X)$是$(1-X)^n$的倍数，所以$P(X)-P(X)^2$是$(X-X^2)^n$的倍数，我们有$P(a) = P(a)^2$。此外，$X-P(X)$是X和$1-X$的倍数，因此倍数等于$X-X^2$。

#### 命题 7 {#alg-viii-s9-prop-7 .statement tag=00AR}

令 $\mathfrak{a}$ 为 A 的两侧零理想，并令 $\overline{e}$ 为环 $A/\mathfrak{a}$ 中的幂等。 A 中存在幂等$e$，其$A/\mathfrak{a}$ 中的典范像等于$\overline{e}$。

设$a$是A中$\overline{e}$的任意代表。A的元素$a-a^2$是幂幂的，因为它属于到$\mathfrak{a}$。 选择引理的多项式 $P\in \mathbf{Z}[X]$ 满足条件 1。我们有 $a-P(a)\in A(a-a^2)$，所以 A 的元素 $e= P(a)$ 有所需性质。

假设环$A/\mathfrak{a}$中的$\overline{e}$属于到中心。 A 提升$\overline{e}$（VIII，p. 172，习题 31）的中心 Z 中不一定存在幂等$e$。然而，如果$A/\mathfrak{a}$中Z的$\overline{e}$属于到像，则它提升到Z中的幂等，因为$Z\cap \mathfrak{a}$是Z的零理想。

#### 推论 1 {#alg-viii-s9-prop-7-cor-1 .statement tag=00AS}

设M和P为从P到M的A-模和$u$满射A-线性映射。假设P是射影的，并且存在A的幂等双面理想$\mathfrak{a}$，使得$u$的核N包含在$\mathfrak{a}P$中。令$M'$和$M''$为M的子模，其中直和为M。则P为子模、$P'$和$P''$的直和，使得$u(P') = M'$和$u(P'') = M''$。

用 P 的自同态 $f$ 的 End$_A(P)$ 由……组成的 B 子环表示，使得$f(N)\subset N$。令$\overline{B}$为M的自同态环。对于$f\in B$，令$\overline{f}$为M的唯一内同态，使得$\overline{f}\circ u=u\circ f$。从 B 到 B 映射 $f\mapsto \overline{f}$ 是环同态。由于模 P 是射影，所以这个同态是满射；它的核$\mathfrak{b}$由自同态$f\in B$组成，这样$f(P)\subset N$。令$n$为自然数，使得$\mathfrak{a}^n= 0$。我们有

$$
P =\mathfrak{a}^0P\supset \mathfrak{a}^1P\supset  \cdots  \supset \mathfrak{a}^{n-1}P\supset \mathfrak{a}^nP = 0
$$

并且，对于每个 $f\in \mathfrak{b}$ 和每个整数 $j\geqslant 0$，

$$
f(\mathfrak{a}^jP) =\mathfrak{a}^jf(P)\subset \mathfrak{a}^jN\subset \mathfrak{a}^{j+1}P
$$

因为$N\subset \mathfrak{a}P$乘假设。因此，我们每自然数 $j$ 和每 $f\in \mathfrak{b}^j$ 都有 $f(P)\subset \mathfrak{a}^jP$。特别是，我们有$\mathfrak{b}^n= 0$。

令$\varepsilon '$为M的投影算子，其中像$M'$和核$M''$。将命题 7 应用于环 B 和幂等双面理想$\mathfrak{b}$，B 中存在幂等$e'$，使得$\overline{e'}=\varepsilon '$，即$\varepsilon '\circ u=u\circ e'$。 集合 $e''= 1-e'$、$\varepsilon ''=\overline{e''}, P'=e'$(P) 和 $P''=e''(P)$。那么 P 是子模 $P'$ 和 $P''$ 的直和，我们有

$$
u(P') =u(e'(P)) =\varepsilon '(u(P)) =\varepsilon '(M) = M'
$$

类似地证明等式$u(P'') = M''$。

#### 推论 2 {#alg-viii-s9-prop-7-cor-2 .statement tag=00AT}

设 A 为环，$\mathfrak{a}$ 为 A 的幂等双面理想。如果 P 是射影 A-模，则$P/\mathfrak{a}P$ 是$A/\mathfrak{a}$ 上的投射模，并且A-模 P 不可分解当且仅当$A/\mathfrak{a}$ 模$P/\mathfrak{a}P$ 不可分解。

设 P 为射影 A-模，并令 $\overline{P}$ 为$A/\mathfrak{a}$模$P/\mathfrak{a}P$。 A-模 P 为零当且仅当 $\overline{P}$ 为零（VIII、p. 158 中的定理 2）。现在假设$P\not= 0$。由于$A/\mathfrak{a}$模P与$\overline{A}\otimes_AP$同构的，因此它是射影的（II, §5, No. 1，p. 279，命题4的推论）。如果 P 不可分解，则根据推论 1 $\overline{P}$ 也是不可分解的。相反，假设 P 可分解并且非零的，并令 $P'$ 和 $P''$ 是 P 的两个非零的子模，使得 $P = P'\oplus P''$。到中山引理（VIII、p. 158、定理 2），我们有$P'+\mathfrak{a}P\not= P$和$P''+\mathfrak{a}P\not= P$；如果$\overline{P}'$和$\overline{P}''$是P中$P'$和$P''$的典范像，那么我们有$\overline{P}'\not= P,\overline{P}''\not= P$和$\overline{P}=\overline{P}'\oplus \overline{P}''$。这证明$\overline{P}$是可分解的。

### 5.模的投射覆盖

#### 定义 3 {#alg-viii-s9-def-3 .statement tag=00AU}

设A为环，设M为A-模。 M 的投影覆盖是对 $(P, u)$，其中 P 是从 P 到 M 的投影 A-模和 $u$ 满同态，这样对于 P 的每个真 A-子模 $P'$，我们都有 $u(P')\not= M$。

#### 注 1 {#alg-viii-s9-n5-rem-1 .statement tag=00AV}

对于每个射影 A-模 M，对 $(M,1_M)$ 是 M 的射影覆盖。

#### 注 2 {#alg-viii-s9-n5-rem-2 .statement tag=00AW}

假设$(P, u)$是A-模M的射影覆盖。令$(x_i)_{i\in I}$是P的元素族，并令$P'$是P的子模，即它生成；那么$u(P')$是由$(u(x_i))_{i\in I}$族生成的。因而，当且仅当族 $(u(x_i))_{i\in I}$ 生成 A-模 M 时，族 $(x_i)_{i\in I}$ 生成 A-模 P。特别是，当且仅当 M 是有限生成时，P 是有限生成的。

#### 命题 8 {#alg-viii-s9-prop-8 .statement tag=00AX}

设M和$M'$分别为M和$M'$的投影覆盖，A-模、$(P, u)$和$(P', u')$以及$g: M\rightarrow M'$A-线性映射。

a) 存在A-线性映射$f: P\rightarrow P'$使得$u'\circ f=g\circ u$。

b) 令$f$为映射。如果 $g$ 是满射（或双射），则 $f$ 是满射（或双射）。如果 $g$ 是单射，其像是 $M'$ 的直因子，则 $f$ 是单射，其像是 $P'$ 的直因子。

通过假设，A-模 P 是射影，映射 $u'$ 是满射。因而，存在A-线性映射$f: P\rightarrow P'$使得$g\circ u=u'\circ f$(II, §2, No. 2，p. 231，命题4)。 断言 a)如下。

令 $f$ 为映射，如 a) 中所示。假设 $g$ 是满射。由于$u$是满射，我们有$M'=g(u(P)) =u'(f(P))$。由于$(P', u')$是M’的射影覆盖，我们有$f(P) = P'$，所以$f$是满射的。按地点。如上所述，$f$的核承认补子模$P_1$，所以$f(P_1) = P'$。现在假设 $g$ 是双射的。我们有$g(u(P_1)) =u'(f(P_1)) =u'(P') = M'$，因此有$u(P_1) = M$。由于 $(P, u)$ 是 M 的投影覆盖，因此我们有 $P_1= P$，因而 Ker($f$) $= 0$。所以 $f$ 是单射的；因为我们已经知道 $f$ 是满射，所以 $f$ 是双射。

对于结论，假设$g$是单射的，并且它的像是$M'$的直因子。那么存在A-线性映射$g': M'\rightarrow M$使得$g'\circ g= 1_M$。由a)，存在A-线性映射$f': P'\rightarrow P$使得$u\circ f'=g'\circ u'$。我们有$u\circ (f'\circ f) =g'\circ u'\circ f= (g'\circ g)\circ u$；根据上一段，映射$f'\circ f$是双射的。用$h$表示逆命题双射；我们有$(h\circ f')\circ f= 1_P$，所以$f$是单射的，它的像是$P'$的直因子（II, §1, No. 9，p. 212，推论2）。

#### 推论 1 {#alg-viii-s9-prop-8-cor-1 .statement tag=00AY}

设 M 为A-模。令$(P, u)$和$(P', u')$为M的射影覆盖。从P到$P'$存在同构$f$使得$u=u'\circ f$。

注，$f$不一定由关系$u=u'\circ f$（VIII，p. 170，习题21）唯一确定。

#### 推论 2 {#alg-viii-s9-prop-8-cor-2 .statement tag=00AZ}

设$(P, u)$是A-模M的射影覆盖。如果Q是射影A-模且$g: Q\rightarrow M$是满射线性映射，则存在满射线性映射$f: Q\rightarrow P$使得$g=u\circ f$。

#### 命题 9 {#alg-viii-s9-prop-9 .statement tag=00B0}

设 M 为 A-模，$(P, u)$ M 的投影覆盖。用 $\mathfrak{r}$ 表示环 A 的根式。 $u$乘以经过推出同态$\overline{u}: P/\mathfrak{r}P\rightarrow M/\mathfrak{r}M$，商为同构。

同态 $u$ 与定义满射，因此 $\overline{u}$ 是满射。用 N 表示 $u$ 的核。我们有 $u^{-1}(\mathfrak{r}M) = N +\mathfrak{r}P$。让我们证明我们有$N\subset \mathfrak{r}P$，这意味着$\overline{u}$的单射性。对于 P 的每个极大子模 $P'$，我们有 $u(P')\not= M$，因此有 $P'+ N\not= P$；由于 $P'$ 是最大的，所以我们有 $N\subset P'$。因此，P 的子模 N 包含在 P 的根中。现在，后者等于$\mathfrak{r}P$乘以VIII、p. 158的命题 6。

#### 推论{#alg-viii-s9-n5-cor-1 .statement tag=00B1}

如果 A-模 M 具有投影覆盖，则 $A/\mathfrak{r}$-模 $M/\mathfrak{r}M$ 是投影的。

事实上，如果$(P, u)$是M的射影覆盖，那么$(A/\mathfrak{r}$)模$M/\mathfrak{r}M$同构于$P/\mathfrak{r}P$(命题9)。由于 A-模 P 是射影的，因此 $(A/\mathfrak{r}$)-模 $P/\mathfrak{r}P$ 也是射影的。

#### 注 3 {#alg-viii-s9-n5-rem-3 .statement tag=00B2}

假设环 A 没有根式。当且仅当$u$是同构时，到命题9，$(P, u)$是A-模M的投影覆盖。因此，投影覆盖只能存在于投影A-模。

环 $\mathbf{Z}$ 没有部首（VIII、p. 154、例 3）。设$n\geqslant 2$为整数。 $\mathbf{Z}$-模块$\mathbf{Z}/n\mathbf{Z}$不是投影的，因此不允许投影覆盖。

#### 注 4 {#alg-viii-s9-n5-rem-4 .statement tag=00B3}

假设每个有限生成A-模都有一个投影覆盖；则 A 与其根式的商 $A'$ 为半单。事实上，每一个有限生成模超过环 $A'$ 都是推论的投影。特别是，对于$A'$的每个左理想$\mathfrak{a}$，$A'$模$A'_s/\mathfrak{a}$是射影的。然后我们的断言是从VIII、p. 138中的命题4开始的。

我们可以给出交换环 A 的例，其中 $A/\mathfrak{r}$ 为半单，以及有限生成A-模 M 的例，它不允许投影覆盖（VIII、p. 170、习题 22）。

#### 命题 10 {#alg-viii-s9-prop-10 .statement tag=00B4}

设 M 为 A-模，P 为射影 A-模，且 $u: P\rightarrow M$ 线性映射。设 $\mathfrak{a}$ 为 A 的双面理想。假设由 $u$ 通过经过推导出商的线性映射 $\overline{u}: P/\mathfrak{a}P\rightarrow M/\mathfrak{a}M$ 是双射的，并且满足以下条件之一：

(i) A-模 M 和 P 是有限生成的，$\mathfrak{a}$ 包含在 A 的根中。

(ii) 理想的$\mathfrak{a}$是幂零的。

那么$(P, u)$就是M的投影覆盖。

在假设下，同态$u$是满射（VIII，p. 159，推论2）并且其核N包含在$\mathfrak{a}P$中。令 $P'$ 为 P 的真子模。通过中山引理 (VIII, p. 158, 定理 2)，我们有 $P'+\mathfrak{a}P\not= P$，因此有 $u(P')\not= M$。所以$(P, u)$是M的投影覆盖。

#### 推论 1 {#alg-viii-s9-prop-10-cor-1 .statement tag=00B5}

令 P 为射影 A-模。假设 P 是有限生成的或者 A 的根$\mathfrak{r}$ 是幂幂的双边理想。用 $u$ 表示从 P 到 $P/\mathfrak{r}P$ 的典范映射。那么$(P, u)$是$P/\mathfrak{r}P$的投影覆盖。

#### 推论 2 {#alg-viii-s9-prop-10-cor-2 .statement tag=00B6}

令 $\mathfrak{a}$ 为 A 和 M A-模的双面理想，使得 $(A/\mathfrak{a})$ 模 $M/\mathfrak{a}M$ 是自由的。假设满足以下条件之一：

(i) 模 M 是有限生成的，$\mathfrak{a}$ 包含在 A 的根中。

(ii) 理想的$\mathfrak{a}$是幂零的。

那么M就有一个投影覆盖。

更准确地说，令 P 为 P 的自由A-模、$(e_i)_{i\in I}$ 基，并令 $u: P\rightarrow M$ 为同态，使得 $M/\mathfrak{a}M$ 形式基的典范像元素 $u(e_i)$ $(A/\mathfrak{a})$-模块$M/\mathfrak{a}M$。那么$(P, u)$就是M的投影覆盖。

$(A/\mathfrak{a}$)-模块$P/\mathfrak{a}P$是免费的，并且同态$\overline{u}$从$P/\mathfrak{a}P$到$M/\mathfrak{a}M$从$u$通过经过推导出变换基的商$P/\mathfrak{a}P$ 变成 $M/\mathfrak{a}M$ 的基，因此是双射的。

如果$\mathfrak{a}$是幂零的，那么它就足以满足应用命题10。现在假设环A是非零的并且模M是有限生成的；那么$(A/\mathfrak{a}$)-模块$M/\mathfrak{a}M$也是如此，因而$(A/\mathfrak{a}$)-模块$P/\mathfrak{a}P$也是如此。那么 $P/\mathfrak{a}P$ 中的每个基都是有限的。由此可知集合 I 是有限的并且 A-模 P 是有限生成的。然后我们再次应用命题10。

#### 推论 3 {#alg-viii-s9-prop-10-cor-3 .statement tag=00B7}

每个有限生成模超过局部环都有投影覆盖。

设 A 为局部环，$\mathfrak{r}$ 其根式。它是 A 的双面理想 (VIII, p. 155, 命题 5, a))，环 $A/\mathfrak{r}$ 是域 (VIII, p. 157, 推论 4)。如果M是A-模，那么$M/\mathfrak{r}M$是向量空间超过域$A/\mathfrak{r}$，因此是一个免费的$(A/\mathfrak{r}$）模块。那么应用推论2就足够了。

#### 注 5 {#alg-viii-s9-n5-rem-5 .statement tag=00B8}

设 A 为局部环，$\mathfrak{r}$ 其根式。设 M 为有限生成A-模，P 为有限生成的射影 A-模，以及 $u: P\rightarrow$ M 同态。由推论 6 VIII、p. 36、A-模 P 是免费的。 P.集合$x_i=u(e_i)$的选择基$(e_i)_{i\in I}$，并用$\overline{x}_i$表示$M/\mathfrak{r}M$中的$x_i$的典范像。以下属性是等效的：

(i) 对 $(P, u)$ 是 M 的投影覆盖。

(ii) $(x_i)_{i\in I}$ 家族是 A-模 M 的最小生成的家族。

(iii) 家庭$(\overline{x}_i)_{i\in I}$ 基向量空间 $M/\mathfrak{r}M$ 超过域 $A/\mathfrak{r}$。

我们通过推论 2 得到 (i) $\Rightarrow$ (ii) 注 2 of VIII、p. 161 和 (iii) $\Rightarrow$ (i)。此外，如果家庭 $(x_i)$ 是A-模 M 的最小生成的家庭，则家庭$(\overline{x}_i)$ 是生成的族的最小族，即基，其中向量空间 $M/\mathfrak{r}M$ 超过 $A/\mathfrak{r}$（VIII，p. 158，推论 1）。

#### 命题 11 {#alg-viii-s9-prop-11 .statement tag=00B9}

设 A 为环和 $\mathfrak{a}$ A 的幂幂双面理想。设 M 为射影 $A/\mathfrak{a}$ 模。存在射影 A-模 P 和满射A-线性映射 $u: P\rightarrow M$ 以及核 $\mathfrak{a}P$。

这样对$(P, u)$是M的投影覆盖，被视为A-模。

存在一个$A/\mathfrak{a}$-模块$M'$，使得$M\oplus M'$是一个免费的$A/\mathfrak{a}$-模块。 选择自由A-模 L 和满射A-线性映射 $v: L\rightarrow M\oplus M'$ 以及核 $\mathfrak{a}L$。根据命题 7 (VIII,p. 159)的推论1，存在直和分解$L = P\oplus P'$，使得$v(P) = M$和$v(P') = M'$。 A-模 P 是射影，A-线性映射 $u$ 从 P 到 M，重合与 $v$ 在 P 上是满射，与核 $\mathfrak{a}P$。第一个断言如下。

设 P 是从 P 到 M 且具有核 $\mathfrak{a}P$ 的射影 A-模和 $u$ 同态。到命题 10 时，对 $(P, u)$ 是 M 的投影覆盖。

#### 推论{#alg-viii-s9-n5-cor-2 .statement tag=00RA}

令 P 和 $P'$ 射影 A-模。如果模 $P/\mathfrak{a}P$ 和 $P'/\mathfrak{a}P'$ 同构的，则 P 和 $P'$ 同构的。

由于 $P/\mathfrak{a}P$ 和 $P'/\mathfrak{a}P'$ 是投影的，因此推论来自投影覆盖的命题 11 和唯一性（VIII，p. 162，推论 1）。

### 习题 {#alg-viii-s9-exercises}

§ 9](exercises/s9/)参见[习题。
