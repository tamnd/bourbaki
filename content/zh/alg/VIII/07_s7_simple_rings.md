---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 7
section_title: Simple Rings
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.119-A VIII.133
pdf_pages: 0136-0150
extraction: native
subsections:
    - "no": 1
      title: Simple Rings
      page: 119
      pdf_page: 136
    - "no": 2
      title: Modules over a Simple Ring
      page: 122
      pdf_page: 139
    - "no": 3
      title: Degrees
      page: 124
      pdf_page: 141
    - "no": 4
      title: Ideals of Simple Rings
      page: 126
      pdf_page: 143
statements: 24
exercises: 16
content_sha256: f605d160c2f06b419447d6b75a1f8ecc61e7d1743499b623a922f46dcc266e6e
translated_from: content/en/alg/VIII/07_s7_simple_rings.md
translation_method: google
source_content_sha256: 0477da2a1cd441904c225c6cad3222346fc38778e44066ddeda16e447e7b81dd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 710bf4122cf5e04bbef12d8ed4009d56d5b50f48c7c3b04cc036d68a83602fa4
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 7。简单环

### 1. 简单环

#### 命题 1 {#alg-viii-s7-prop-1 .statement tag=0081}

设A为非零环。以下条件是等价的：

(i) A-模 $A_s$ 是同型的。

(ii) 环 A 是左阿廷的，并且 A 的每个双面理想都等于 0 或 A。

(iii) 环 A 是左阿廷的，并且存在简单且忠实的左A-模 S。

如果满足这些条件，则A-模$A_s$有有限长度且同构于型S，并且每个单A-模同构于S。

让我们证明 (i) 蕴涵 (ii)。假设满足(i)。那么有限生成A-模$A_s$是半单，因此有有限长度并且是阿廷的（VIII，p. 71，命题10）；因而，环 A 为左阿廷的。 左A-模 $A_s$ 的自同态是 A 的乘法与元素的对数。由于左A-模 $A_s$ 是同型的，因此从 VIII、p. 86 的命题 6, b) 得出$(A$, A)-双模$_sA_d$ 很简单。 $_sA_d$的子双模是A的两侧理想，因而(i)蕴涵(ii)。

让我们证明 (ii) 蕴涵 (iii)。 环 A不减为0；因而，存在单A-模 S。S 的湮没子是A 的真两侧理想。如果我们假设满足(ii)，则湮没子等于0。A-模 S 是忠实的，并且(ii) 蕴含(iii)。

让我们证明 (iii) 蕴涵 (i)。假设满足(iii)。则存在整数 $m\geqslant 1$，使得 $A_s$ 同构于 $S^m$ 的子模 (VIII, p. 50, 命题 5, a))。由于$S^m$是型S的同型A-模，因而$A_s$同样成立（VIII，p. 61，命题2）；因而，(iii) 意味着(i)。

假设满足条件(i)至(iii)。我们在上面已经看到，A-模$A_s$有有限长度并且是型S的同构。每个简单的左A-模都同构于$A_s$的商，因此也同构于S。

#### 定义 1 {#alg-viii-s7-def-1 .statement tag=0082}

如果环 A 满足命题 1 的等价条件 (i)、(ii) 和(iii)，我们称环 A 是简单的。设K 为交换域；如果 K-代数的底层环是简单的，则它被称为简单的。

#### 注 1 {#alg-viii-s7-n1-rem-1 .statement tag=0083}

回想一下，通过 II, §9, No. 1、p. 115 的定理 1，以下属性是等效的：

(i) A-模 $A_s$ 很简单。

(ii) 环 A 不会减少到 0，并且 A 不存在不同于 0 或 A 的左理想。

(iii) 环 A 为域。

因而，通过命题 1 (条件 (ii))，可交换简单环只不过是交换域。

#### 注 2 {#alg-viii-s7-n1-rem-2 .statement tag=0084}

如果有时不被约等于 0 并且其唯一的两侧理想是 0 和 A，我们就说环 A 是拟单。如果 A 承认忠实的单模，我们就说 A 是本原的。到命题 1 时，每个简单的环都是拟单。由于每个非零环都承认单模的单模和湮没子是双面理想，所以我们看到每个拟单环都是本原的。然而，存在不简单的拟单环和不是拟单的本原环（VIII，p. 128，习题2）；这样的环不是左阿廷的。

#### 定理 1（韦德伯恩）{#alg-viii-s7-thm-1 .statement tag=00S3}

环是简单的当且仅当它与矩阵环 $\mathbf{M}_r(D)$ 同构的，其中 $r\geqslant 1$ 是整数且 D 域。

#### 引理 1 {#alg-viii-s7-lem-1 .statement tag=0085}

设A是一个简单的环，S是一个简单的左A-模，D是域End$_A(S)$的逆环。那么 S 是可逆的 $(A,D)$-双模。它也是D上的有限维右向量空间，从A到End$_D(S)$映射$a\mapsto a_S$是环同构。

到命题 1，A-模 $A_s$ 具有有限长度并且与型 S 同型分支的。因而，存在整数 $m\geqslant 1$，使得 A-模 $A_s$ 和 $S^m$ 同构的。那么 A-模 S 是射影且有限生成的。它是生成的 (VIII、p. 80、定理 1)，并且引理 1 是从VIII、p. 101、(ii)$\Rightarrow$(i) 和 (ii)$\Rightarrow$(iii) 中的定理 1 得出的，适用于$(A,D)_{\mathbf{Z}}$-双模 S。

#### 引理 2 {#alg-viii-s7-lem-2 .statement tag=00R7}

令 D 为有限维 $r\geqslant 1$ 的域和 V 右向量空间在 D 上。则 V 为单模在环 E = End$_D(V)$ 上，且其交换子等于 $D_V$。 环 E 很简单，它的左长度等于$r$。

我们知道V是一个简单的E模（VIII，p. 45，例3），并且它的交换子等于$D_V$（VIII，p. 82，推论1）。令$(x_i)_{1\leqslant i\leqslant r}$为域D上V的基。映射$u\mapsto (u(x_i))_{1\leqslant i\leqslant r}$为从E模块$E_s$到E模块$V^r$的同构；因而，E 模$E_s$ 是长度 $r$ 的同型，所以环 E 是简单的。

现在让我们证明定理1。 回忆一下（II, §10, No. 7，p. 349），环$\mathbf{M}_r(D)$可以与右D-向量空间$D^r_d$的自同态环识别；此外，域 D 上的有限维 $r$ 的每个右向量空间都同构于 $D^r_d$ (II, §7, No. 1, p. 292)。 因而，定理 1 由引理 1 和 2 得出。

#### 注 3 {#alg-viii-s7-n1-rem-3 .statement tag=0086}

设 A 为域 End$_A(S)$ 的简单环、S 单A-模和 D 逆环。那么A-模$A_s$有有限长度，并且dim$_D(S)$等于long(A)。事实上，通过引理 1，环 A 与 End$_D(S)$ 同构的；然后我们应用引理2。

#### 推论 1 {#alg-viii-s7-lem-2-cor-1 .statement tag=0087}

a) 简单的环的中心是域。

b) 简单的环的逆环很简单。

c) 简单环的左长度等于它的右长度。

设 D 为域，Z 为中心，且在有限维 $r\geqslant 1$ 的 D 上V 右向量空间。我们用 E 表示 V 的自同态环。

映射$z\mapsto z_V$是从Z到E的中心乘VIII、p. 83的推论2的同构。 断言a)如下。 V的对偶$V^*$是右向量空间与D的相反的域$D^o$，并且它的维数等于$r$。 映射$u\mapsto^tu$是从E的逆环$E^o$到环结束$_{D^o}(V^*)$的同构。 因而，环$E^o$很简单，环E和$E^o$具有相同的左长度，等于$r$（引理2）。

#### 推论 2 {#alg-viii-s7-lem-2-cor-2 .statement tag=0088}

令$r$和$r'$严格为正整数，并令D和$D'$为域。 环 $\mathbf{M}_r(D)$ 和 $\mathbf{M}_{r'}(D')$ 同构当且仅当我们有 $r=r'$ 和域 D 和 $D'$ 同构。

条件显然就足够了。

相反，假设环 $B =\mathbf{M}_r(D)$ 和 $B'=\mathbf{M}_{r'}(D')$ 同构。由于$r$是$B_s$的长度，$r'$是$B'_s$（引理2），所以我们有$r=r'$。此外，B是与D和$B'$至$D'$(VIII，p. 102，例1)等价的森田。因而，域 D 和$D'$ 是 Morita 等价的，因此是同构的 (VIII, p. 111, 命题 13, c))。

#### 推论 3 {#alg-viii-s7-lem-2-cor-3 .statement tag=0089}

令 K 为交换域，并令 A 为有限次数的 K-代数，且底层为环。在 K 上存在整数 $r$ 和有限次数的 K-代数 D，即域，使得 A 与 $M_r(D)$ 同构。特别是，如果 K 是代数闭集，则 A 在 K 上同构于矩阵代数。

令 S 为简单的左A-模；它是 K 上的有限维 K-向量空间。因而，它的交换子是 K 上有限次数的代数。第一个断言由引理 1 得出。如果 K 是代数封闭的，则 D = K by VIII、p. 47 的定理 1。

#### 注 4 {#alg-viii-s7-n1-rem-4 .statement tag=008A}

设 K 为代数闭交换域，并设 A 为 K 上有限次数的代数。 代数当且仅当存在整数 $n\geqslant 1$ 且 A 与 $M_n(K)$ 同构时，A 才是简单的。那么它的中心与 K 同构。

### 2. 单环上的模

#### 引理 3 {#alg-viii-s7-lem-3 .statement tag=008B}

令 A 为简单的环，令 S 为单A-模。用 D 表示 S 的交换子的对数域。每个 A-模都同构于形式 $S\otimes_DV$ 的 A-模，其中 V 是域 D 上的左向量空间。

这是从VIII、p. 120和森田的定理（VIII、p. 103）中的引理 1 得出的。

#### 命题 2 {#alg-viii-s7-prop-2 .statement tag=008C}

设 A 为简单的环，S 为单A-模。

a) 每个 A-模都是射影且与型 S 同型分支的，因此有半单。如果它有长度$\mathfrak{a}$，那么它与$S^{(\mathfrak{a})}$同构。

b) 每个非零的A-模都是生成的。

c) 两个A-模同构当且仅当它们具有相同的长度。

用 D 表示 S 的交换子的对数域。由 VIII、p. 120 的引理 1，S 是可逆的 $(A$，D)-双模。设M为A-模；通过引理 3，它与形式$S\otimes_DV$的模同构，其中V是左向量空间超过域D。

D-模 V 是射影且与型 $D_s$ 同型分支的；当且仅当不减为0时才是生成的。最后，$S\otimes_DV$的长度等于D-向量空间V的维数，并且两个向量空间同构当且仅当它们具有相同的维数。鉴于VIII、p. 109中的命题10和VIII、p. 110中的12，命题2现在紧随其后。

设$r\geqslant 1$为整数。如果存在基数$\mathfrak{b}$使得$\mathfrak{a}=r\mathfrak{b}$，我们说基数$\mathfrak{a}$可以被$r$整除。如果 $\mathfrak{a}$ 是无限的，就会出现这种情况，因为我们有 $r\mathfrak{a}=\mathfrak{a}($集合理论、III, §6, No. 3、p. 188、推论 3)。由此可知，如果基数 $\mathfrak{a}$ 能被 $r$整除，则存在唯一的基数 $\mathfrak{b}$，使得$\mathfrak{a}=r\mathfrak{b}$。

#### 推论 {#alg-viii-s7-n2-cor-1 .statement tag=008D}

令$k$为交换域，并令A为有限次数在$k$上的简单$k$代数。每个单A-模都是 $k$ 上的有限维。两个A-模同构当且仅当它们的维数大于$k$相等。

每个单A-模都同构于 $A_s$ 的商，因此在 $k$ 上是有限维的。然后从命题 2, c) 得出推论。

#### 命题 3 {#alg-viii-s7-prop-3 .statement tag=008E}

设 A 是一个简单的环。 A-模 M 是自由的当且仅当其长度能被 A 的长度整除。如果是这种情况，则 M 的所有基具有相同的基数，用 dim$_A(M)$ (II, §7, No. 3, p. 294, 注 2) 表示，并由下式确定关系

（1）长$_A(M) =$长（A）$\cdot$暗$_A(M)$。

假设M是自由的，令$(e_i)_{i\in I}$为M的基。A-模M为A-模$Ae_i$的直和，它们均与$A_s$同构。 集合$r=$长$_A(A_s)$； 整数大于或等于 1（VIII、p. 119、命题 1）。我们有VIII、p. 73的公式(13)长$_A(M) =r$卡(I)。

相反，假设基数long$_A(M)$能被$r$整除。令$\mathfrak{a}$为基数，使得长$_A(M) =r\mathfrak{a}$。则A-模 M 与$A^{(\mathfrak{a})}_s$ 具有相同的长度，因此与命题 2 同构。这证明M 是自由的。

#### 命题 4 {#alg-viii-s7-prop-4 .statement tag=008F}

设 A 为简单的环，M 为非零的 A-模。用B表示A-模M的自同态环，将M视为左B-模。

a) 映射 $a\mapsto a_M$ 是从 A 到 B-模 M 的自同态环的同构。

b) 假设 M 的有限长度为 A-模。那么环 B 很简单，我们有

(2) 长$_A(M) =$长(B)和长$_B(M) =$长(A)。

A-模 M 是 VIII、p. 122 中的生成的乘以命题 2。到定义，我们有$B = A'_M$，并且断言 a) 因此从VIII、p. 82 的定理 2 得出。

假设 M 是有限长度中的 A-模。 选择单A-模 S，令 D 为 S 的自同态环的对数域。由引理 3，A-模 M 同构于形式 $S\otimes_DV$ 的模，其中V 是左向量空间超过域 D。向量空间 V 是有限维的。由VIII、p. 64、环的定理 3，B同构于End$_D(V)$；通过引理 2 (VIII, p. 121)，环 B 因此是简单的。考虑注 1 of VIII, p. 63，我们得到等式

长（B）=暗$_D(V) =$长$_A(M)$。

通过 VIII、p. 63 中的注 1 和 VIII、p. 121 中的 3 个，我们有关系

长$_B(M) =$长$_{End_D(V)}(S\otimes_DV) =$暗淡$_D(S) =$长(A),

这给出了最后一个关系。

### 3. 次数

考虑 B 的环 B 和子环 A。 赋予 B 一个 $(A$，A)-双模的结构，该限制标量从 $_sB_d$ 上的 $(B$，B)-双模结构推导出来。

#### 命题 5 {#alg-viii-s7-prop-5 .statement tag=008G}

设 B 为环，A 为 B 的简单子环，S 为简单左A-模。那么B是一个自由的左A-模长维数长$_A(B\otimes_AS)$。

令$r$为A的长度； A-模 $A_s$ 与 $S^r$ 同构。现在，左A-模 B 同构于 $B\otimes_AA_s$ (II, §3, No. 4, p. 249)，因此也同构于 $(B\otimes_AS)^r$ (II, §3, No. 7, p. 255, 命题 7)。因而，我们有 long$_A(B) =r$ long$_A(B\otimes_AS)$，并且命题 5 是从 VIII、p. 123 的命题 3 得出的。

#### 定义 2 {#alg-viii-s7-def-2 .statement tag=008H}

设B为环，A为B的简单子环。自由左A-模B的维数称为B在A上的（左）次数，并用[^1]$[B : A]_s$表示。

通过替换 A 和 B 与逆环，我们从上面推出 B 是一个自由的右A-模。我们用$[B : A]_d$表示它的维数，并称其为B在A上的右次数。

我们可以给出域 B 和子域 A 的例，使得次数 $[B : A]_s$ 和 $[B : A]_d$ 不同。[^2]

设 B 为环，A 为 B 的简单子环，S 为简单左A-模。设 M 为左A-模，$\mathfrak{a}$ 为长度。 A-模 M 和 $S^{(\mathfrak{a})}$ 是同构的（VIII、p. 122、命题 2），因而 B-模 $B\otimes_AM$ 和 $(B\otimes_AS)^{(\mathfrak{a})}$ 也是同构。 关系

(3) 长$_A(B\otimes_AM) = [B : A]_s$ 长$_A(M)$

由命题 5 和定义 2 得出。

#### 命题 6 {#alg-viii-s7-prop-6 .statement tag=008I}

令C为环，B为C的简单子环，A为B的简单子环。然后我们有$[C : A]_s= [C : B]_s[B : A]_s$。

让我们介绍将C视为左B-模的基$(e_i)_{i\in I}$和将B视为左A-模的基$(f_j)_{j\in J}$。那么$(f_je_i)_{j\in J,i\in I}$是C的基，被视为左A-模（II, §1, No. 13，p. 222，命题25）；接下来是命题6。

#### 注 1 {#alg-viii-s7-n3-rem-1 .statement tag=008J}

假设 A 是简单环 B 的简单子环，并且右侧次数 $[B : A]_d$ 是有限的。设C为B的自同态环，视为右A-模；这是一个简单的环乘以命题 4, b) 的 VIII, p. 123。对于B中的任意$b$，令从B到B的$\gamma (b)$为映射$x\mapsto bx$；那么$\gamma :b\mapsto \gamma (b)$是从B到C的子环的同构。另外，如果$(x_1, . . . , x_m)$是右A-模B的基，则从C到$B^m_s$发送$c$到$(c(x_1), . . . , c(x_m))$的态射就是左B-模的同构；因而，我们有关系

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

考虑到VIII的关系(2)，p. 123应用于右A-模B，我们看到

(5)长(C)$= [B : A]_d$长(A)。

#### 注 2 {#alg-viii-s7-n3-rem-2 .statement tag=008K}

设 K 为交换域。如果A在K上是有限次数的代数B的单子代数，则B在A上的左次数满足关系$[B : A]_s[A : K] = [B : K]$乘以VIII、p. 125的命题6。同样，我们有$[B : A]_d[A : K] = [B : K]$。接下来是等式$[B : A]_s= [B : A]_d$。

### 4. 单环的理想

令 D 为域且 V 右向量空间超过 D 的有限维 $n\geqslant 1$。 考虑简单的环 A = End$_D(V)$。 对于V的任何线性子空间W，我们用$\mathfrak{a}(W)$（或$\mathfrak{b}(W)$）表示A的满足$aW = 0$（或$aV\subset W$）的元素集$a$。

#### 命题 7 {#alg-viii-s7-prop-7 .statement tag=008L}

a) 映射$W\mapsto \mathfrak{a}(W)$是从V的线性子空间的集合到A的左理想集合的双射。

b) 映射$W\mapsto \mathfrak{b}(W)$是从V线性子空间的集合到A的右理想集合的双射。

c) 令$W_1$和$W_2$是子空间与V的线性关系。 关系 $W_1\subset W_2$、$\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$ 和 $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ 等效。

断言 b) 源自 VIII、p. 104 的例 1、b)，应用于可逆 $(D^o,A^o$)-双模 V，关系 $W_1\subset W_2$ 和 $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ 的等价也是如此。

令 $V^*$ 为 V 的对偶，视为右向量空间相对于 D 的域 $D^o$。对于V 的任何子空间 W，用 $W'$ 表示 W 在 $V^*$ 中的正交。从V子空间集合到$V^*$子空间集合映射$W\mapsto W'$为双射。如果$W_1$和$W_2$是V的两个子空间，则关系$W_1\subset W_2$和$W'_1\supset W'_2$是等价的。现在，从A到End$_{D^o}(V^*)$的逆环，映射$u\mapsto^tu$是同构；它将A的变换左理想转化为End$_{D^o}(V^*)$和$\mathfrak{a}(W)$的右理想，转化为$V^*$的自同态$h$的集合$\mathfrak{b}(W')$，使得$h(V^*)\subset W'$。 断言 a)，以及关系 $W_1\subset W_2$ 和 $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$ 的等价，则从断言开始，类似于 b)，对于 V 的对偶 $V^*$。

#### 推论 {#alg-viii-s7-n4-cor-1 .statement tag=008M}

a) A 的最小左理想是理想 $\mathfrak{a}(H)$，其中 H 是 V 中的超平面。 A 的最大左理想是理想 $\mathfrak{a}(L)$，其中 L 是V 中的一条线。

b) A 的最小右理想是理想$\mathfrak{b}(L)$，其中L 是V 中的一条线。 A 的最大右理想是理想 $\mathfrak{b}(H)$，其中 H 是 V 中的超平面。

设 $(L_i)_{i\in I}$ 是与直和 V 的线族。让$(\varepsilon_i)_{i\in I}$是与分解$V =\oplus_{i\in I}L_i$相关的投影算子族。 $\varepsilon_i$ 在 A 中是幂等的，对于 $i\not=j$ 和 $\sum_{i\in I}\varepsilon_i= 1$，我们有 $\varepsilon_i\varepsilon_j= 0$。用$H_i$表示超平面$\sum_{j\not=i}L_j$；是$\varepsilon_i$中的核。然后我们有

$$
\mathfrak{a}(H_i) = A\varepsilon_i,\mathfrak{b}(L_i) =\varepsilon_iA
$$

A-模$A_s$是最小左理想族$(\mathfrak{a}(H_i))_{i\in I}$的直和，$A_d$是最小右理想族$(\mathfrak{b}(L_i))_{i\in I}$的直和。

考虑具体情况 $V = D^n_d$ 和认同 A 与矩阵环 $\mathbf{M}_n(D)$。用I表示$\mathbf{N}$中的区间$[1, n]$，用$(v_i)_{i\in I}$表示V的典范基； 集合$L_i=v_iD$，并用$E_{ij}$矩阵单位（II, §10, No. 3，p. 341）表示。然后我们就有$\varepsilon_i= E_{ii}$。左理想AE$_{ii}$等于DE$_{1i}+\cdots +$DE$_{ni}$，并由矩阵和所有列组成，除了第$i$等于零。正确的理想$E_{ii}A$等于DE$_{i1}+\cdots +$DE$_{in}$，并由矩阵组成，除了第$i$之外的所有行都等于零。我们还有关系

$$
E_{ii}A E_{jj}= E_{ii}A\cap A E_{jj}= D E_{ij}
$$

对于 $i$ 和 $j$ 在 1 和 $n$ 之间。

### 习题{#alg-viii-s7-exercises}

参见[习题为 § 7](exercises/s7/)。

[^1]: 如果 A 和 B 为交换域，请注意不要将等于 [B : A] 的次数与 A 的扩张 B 的可分离次数混淆，定义在 V, §6, No. 5、p. 31 中，也用 $[B : A]_s$ 表示。
[^2]: cf.A. H. Schofield，Artin 的问题倾斜域扩张，数学。 过程。 剑桥斐洛斯。 苏克。 **97** (1985)，第 1-6 页。
