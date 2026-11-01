---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 8
section_title: Semisimple Rings
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.135-A VIII.150
pdf_pages: 0152-0167
extraction: native
subsections:
    - "no": 1
      title: Semisimple Rings
      page: 135
      pdf_page: 152
    - "no": 2
      title: Modules over a Semisimple Ring
      page: 138
      pdf_page: 155
    - "no": 3
      title: Factors of a Semisimple Ring
      page: 141
      pdf_page: 158
    - "no": 4
      title: Idempotents and Semisimple Rings
      page: 145
      pdf_page: 162
statements: 30
exercises: 6
content_sha256: f444e9f38ebdac8fd34670dcb5062e0c064d6216c8475d4958512822aed5847a
translated_from: content/en/alg/VIII/08_s8_semisimple_rings.md
translation_method: google
source_content_sha256: c3520cd3a5b6efacdd841870c3c2e342b0341edbd32074687bd212bc32731ee7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 101fe0e89db0f8232872ad8bc05f5ec856ceeb165ac270ab3fdeaaf49d0b580c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。 半单环

### 1.半单环

#### 定理 1（韦德伯恩）{#alg-viii-s8-thm-1 .statement tag=00S4}

设 A 为环。以下属性是等效的：

(i) A-模 $A_s$ 为半单。

(ii) 对于 A 的每个左理想 $\mathfrak{a}$，都存在 A 的左理想 $\mathfrak{b}$，使得 $A_s$ 是 $\mathfrak{a}$ 和 $\mathfrak{b}$ 的直和。

(iii) 环 A 为左阿廷的，$(A,A)$-双模$_sA_d$ 为半单。

(iv) 环 A 同构于简单环的有限族中的乘积。

(v) 存在整数$s\geqslant$0、域$D_1, . . . ,D_s$和整数$r_1\geqslant 1, . . .,r_s\geqslant 1$，使得环A与矩阵环$\mathbf{M}_{r_i}(D_i)$的乘积同构。

(vi) 环 A 为左阿廷的，且存在忠实且半单左A-模。

(i)和(ii)的等价由VIII、p. 56的推论2得出，(iv)和(v)的等价由VIII、p. 120的定理1得出。

A-模 $A_s$ 是有限生成的。如果是半单，那么就是左阿廷的（VIII、p. 71、命题 10）。由于 A-模 $A_s$ 是忠实的，这证明 (i) 蕴涵 (vi)。相反，假设性质 (vi) 成立；让M成为忠实的半单A-模。存在整数 $m\geqslant 1$，使得$A_s$同构于$M^m$的子模 (VIII, p. 50, 命题 5, a))；因为M是半单，所以$A_s$也是如此。因此我们证明了(i)和(vi)的等价。

让我们证明 (i) 蕴涵 (iii)。假设环 A 有性质 (i)；我们已经观察到 A 是左阿廷的。现在，左A-模$A_s$的自同态是A的右乘法除以元素。$(A$，A)-双模$_sA_d$是半单然后从命题6得出VIII，p. 86。

让我们证明 (iii) 蕴涵 (iv)。假设$(A$，A)-双模$_sA_d$是半单。它是有限生成的，因此存在一个由简单 $(A$、A)-子双模组成的有限族 $(\mathfrak{a}_i)_{i\in I}$，其中直和 $_sA_d$。在其他字中，$\mathfrak{a}_i$是A的非零的双面理想，A的加法群是$\mathfrak{a}_i$的直和，并且对于每个$i\in I$，$\mathfrak{a}_i$中包含的A的每个双面理想都等于0或$\mathfrak{a}_i$。每 $i\in I$ 集合 $\mathfrak{b}_i=\sum_{j\not=i}\mathfrak{a}_j$；这是 A 的双面理想。 映射 $a\mapsto (a+\mathfrak{b}_i)_{i\in I}$ 是从环 A 到乘积的环 $A/\mathfrak{b}_i$ 的同构。 $(A$，A)-双模$\mathfrak{a}_i$和$A/\mathfrak{b}_i$是同构的，因此$A/\mathfrak{b}_i$的每个双面理想都等于0或$A/\mathfrak{b}_i$。如果环 A 是左阿廷的，那么环 $A/\mathfrak{b}_i$ 同样成立，因此很简单（VIII、p. 120、定义 1）。

最后，让我们证明（iv）蕴涵（i）。假设 A 是简单环的有限族 $(A_i)_{i\in I}$ 中的乘积。用 $\pi_i$ 投影和指标 $i$ 从 A 到 $A_i$ 表示，并用 $M_i$ A-模表示，底层为加法群 $A_i$ 和律作用$(a, x)\mapsto \pi_i(a)x$。由于环$A_i$很简单，$A_i$模$(A_i)_s$是半单，所以A-模$M_i$是半单。由于A-模$A_s$只不过是乘积$\prod_{i\in I}M_i$，所以它是半单。

#### 定义 1 {#alg-viii-s8-def-1 .statement tag=0093}

如果环 A 具有定理 1 的等价属性 (i) 到 (vi)，则我们说环 A 是半单。 如果环底层 A 是，则代数 A 超过交换环 $k$ 是半单代数半单。

#### 命题 1 {#alg-viii-s8-prop-1 .statement tag=0094}

设 A 为半单环。存在 A 的最小左理想的有限族 $(\mathfrak{m}_i)_{i\in I}$ 使得 $A_s=\oplus_{i\in I}\mathfrak{m}_i$。如果$(\mathfrak{m}_i)_{i\in I}$是这样一个族，那么每个单A-模都同构于$\mathfrak{m}_i$之一。 单A-模类集合是有限的。

第一个断言源自A-模$A_s$是半单并且是有限生成的。每个单模都同构于 $A_s$ (VIII, p. 46, 命题 1) 的商。第二个断言由VIII、p. 56的推论3得出，第三个断言是第二个直接的推论。

#### 例 {#alg-viii-s8-n1-exa-1 .statement tag=0095}

设 G 为有限群，K 交换域。 $*$我们将进一步从（VIII，p. 401，推论1）看出，当且仅当K的特征指数与$G.*$的阶素数时，群G的代数K[G]在域K上是半单环

#### 注 1 {#alg-viii-s8-n1-rem-1 .statement tag=0096}

令K为交换域，并令A为K上的半单代数。则存在K-代数$D_1, . . . ,D_s$，即域和整数$r_1\geqslant 1, . . . , r_s\geqslant 1$，使得K-代数A与乘积$\prod^s_{i=1}\mathbf{M}_{r_i}(D_i)$同构的。

#### 注 2 {#alg-viii-s8-n1-rem-2 .statement tag=0097}

设 K 为代数闭域，并设 A 为 K 上有限次数的代数。通过 VIII、p. 122、代数的注 4，A 为半单当且仅当存在整数 $n_1\geqslant 1, . . . , n_r\geqslant 1$ 使得 A 同构于代数$\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$。

#### 命题 2 {#alg-viii-s8-prop-2 .statement tag=0098}

a) 半单环的中心是半单。

b) 半单环的逆环是半单。

c) 半单环与双边理想的商为半单环。

d) 半单环有限族中的乘积是半单环。

设A为半单环。它同构于简单环的有限族 $(A_i)_{i\in I}$ 的乘积。 A的中心与$A_i$的中心的乘积同构，$A^o$与$A^o_i$的乘积环同构。因而，断言 a) 和 b) 由VIII、p. 121 的推论 1 得出。

设$\mathfrak{a}$为A的双面理想。A-模$A_s/\mathfrak{a}$，半单A-模$A_s$的商为半单。因而$(A/\mathfrak{a}$)-模$A_s/\mathfrak{a}$是半单； 断言 c)如下。

环是半单当且仅当它同构于简单环的有限族的乘积； 断言 d)如下。

#### 命题 3 {#alg-viii-s8-prop-3 .statement tag=0099}

设A为交换环。以下属性是等效的：

(i) 环 A 是半单。

(ii) 环 A 为阿廷的并减少 (V, §6, No. 7, p. 34)。

(iii) 环 A 同构于交换域有限族中的乘积。

可交换简单环为交换域 (VIII, p. 120, 注 1)。因而 (i) 等价于 (iii)。

显然，(iii) 暗示着(ii)。相反，假设环 A 是阿廷的并减少了。 A 素理想的集合的交由 A 的幂零元 (V, §15, No. 1, p. 118, 命题 2) 组成，因此由于 A 约简而被约等于 0。到VIII、p. 2，则存在 A 的不同素理想 $\mathfrak{p}_1, . . . ,\mathfrak{p}_r$，使得我们有 $\mathfrak{p}_1\cap  \cdots  \cap \mathfrak{p}_r= 0$。由VIII、p. 8的推论，阿廷环A的每个素理想$\mathfrak{p}_i$都是最大的；因而，只要 $i$ 和 $j$ 不同，我们就有$\mathfrak{p}_i+\mathfrak{p}_j= A$。由I, §8, No. 11、p. 110、典范同态中的命题 9，从A到环$\prod^r_{i=1}(A/\mathfrak{p}_i)$是同构。对于每个 $i$，环 $A/\mathfrak{p}_i$ 是域，因而 (ii) 意味着 (iii)。

有限次数超过域的交换代数是阿廷的交换环。因而，命题 3 概括了V, §6, No. 7、p. 34 的命题 5。

### 2.半单环上的模

#### 命题 4 {#alg-viii-s8-prop-4 .statement tag=009A}

设A为环。以下属性是等效的：

(i) 环 A 是半单。

(ii) 每个 A-模都是半单。

(iii) 存在生成的和半单A-模。

(iv) 存在忠实且半单A-模且对模有限生成。

(v) 每个 A-模都是投影。

(vi) 每个单生 A-模都是射影的。

$*$对于半单环的其他刻画，请参见X, §8的命题 6，n$^o4$，第1页。 $140.*$

我们首先证明(i)蕴涵(ii)和(v)。假设环 A 是半单，并考虑左A-模 M。到假设，A-模 $A_s$ 是半单，所以每个自由A-模都是半单。到II, §1, No. 11、p. 218的命题20，从L到M存在自由A-模L和满射A-线性映射$u$。令N为$u$的核。由于A-模L为半单，因此L中存在半单子模$N'$对N进行补充（VIII，p. 56，定理1）。 A-模 $N'$ 是射影，而 $u$ 诱导同构从 $N'$ 到 M。因而，M 是半单和射影。

(ii) $\Rightarrow$ (iii)：如果每个A-模都是半单，那么A-模$A_s$就是半单；而且是生成的。

(iii) $\Rightarrow$ (iv)：如果 M 为生成A-模，则它是忠实的（VIII，p. 80，定理 1 的推论），并且其对模是有限生成的（VIII，p. 99，推论 1）。

(iv) $\Rightarrow$ (i)：令 M 忠实且半单A-模且对模有限生成。由VIII、p. 8的引理 4，存在自然数$m$，使得$A_s$与$M^m$的子模同构。 A-模 $M^m$ 是半单，因而$A_s$ 也是。

蕴涵 (v) $\Rightarrow$ (vi) 是直接的。

(vi) $\Rightarrow$ (i)：假设每个单生 A-模都是射影的。设 $\mathfrak{a}$ 为 A 的左理想。由于 A-模 $A_s/\mathfrak{a}$ 是射影，因此存在 A 的左理想 $\mathfrak{b}$，使得 $A_s$ 为 $\mathfrak{a}$ 和 $\mathfrak{b}$ 的直和 (II, §2, No. 2, p. 231, 命题4)。因而，环 A 为半单（VIII、p. 135、定理 1）。

#### 引理 1 {#alg-viii-s8-lem-1 .statement tag=009B}

设A为左阿廷的环，设M为单A-模。那么环$A_M$就简单了。

由于环 A 为左阿廷的，因此对于环 $A_M$，通过VIII、p. 7 的命题 5 也是如此。现在，M是一个忠实且简单的$A_M$模块，因此环$A_M$很简单（VIII，p. 119，命题1）。

#### 命题 5 {#alg-viii-s8-prop-5 .statement tag=009C}

假设环 A 是半单。令 M 为左A-模。 M 的对模是有限生成的，我们有 $A_M= A''_M$。

首先考虑M为单A-模的情况。到引理 1，环 $A_M$ 就很简单了。然后从 VIII、p. 120 的引理 1 得出命题 5。

现在考虑一般情况。 单A-模类集合 $\mathscr{S}$ 是有限的（VIII、p. 136、命题 1）。对于$\lambda \in \mathscr{S}$，类$\lambda$的选择A-模$S_{\lambda}$，并用$D_{\lambda}$表示$S_{\lambda}$交换子的相反域。将引理 1 应用于简单的环 $A_{S_{\lambda}}, S_{\lambda}$ 是有限维向量空间超过域 $D_{\lambda}$；用 $m(\lambda )$ 表示其维数。设B为M的自同态环的逆环。我们在VIII，p. 84中看到，存在$(D_{\lambda}$，B)-双模$V_{\lambda}$，简单如B-模和同构 $(A$, B)-从 M 到 $\oplus_{\lambda\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ 的双模。由于 B-模，M 与 $\oplus_{\lambda\in\mathscr{S}}V^{m(\lambda)}_{\lambda}$ 同构的。由于 $\mathscr{S}$ 和 $m(\lambda )$ 是有限的，因而 M 是有限生成的 B-模。

A-模 M 为半单，其对模是有限生成的。因而，我们有 VIII、p. 83 中的 $A_M= A''_M$ × 命题 4。

#### 命题 6 {#alg-viii-s8-prop-6 .statement tag=009D}

令 M 为有限生成的半单A-模。用 $\mathscr{S}_M$ 表示其支持度 (VIII, p. 66)，并用 B 表示其自同态环。对于类 $\lambda$ 的每个 $\lambda \in \mathscr{S}_M$、选择单A-模 $S_{\lambda}$，并表示左B-模坎$_A(S_{\lambda},M)$ $V_{\lambda}$。

a) 环 B 为半单。

b)从M的支撑$\mathscr{S}_M$到单B-模的类的集合，映射$\lambda \mapsto$cl(V$_{\lambda}$)为双射。

c) 对于每个$\lambda \in \mathscr{S}_M$，A-模 M 的型 $\lambda$ 的同型成分等于B-模 M 的型 $V_{\lambda}$ 的同型成分。

被视为 B-模，M 是半单（VIII、p. 85、命题 5）且忠实。它的对模是有限生成的，因为我们有 $A_M\subset$ End$_B(M)$。因而，环 B 为半单 (命题 4)。如果 $(x_1, . . . , x_r)$ 是 A-模 M 的生成的序列，则从 $B_s$ 到 $M^r$ 的映射 $b\mapsto (bx_1, . . . , bx_r)$ 是 B 线性且单射的。每个单B-模都同构于 $B_s$ 的子模 (VIII, p. 136, 命题 1)，因此同构于 M 的 B-子模。 命题则紧随 VIII 的命题 5， p. 85。

#### 命题 7 {#alg-viii-s8-prop-7 .statement tag=009E}

设A为半单环。

a) 每个有限生成A-模都是自反的 (II, §2, No. 7, p. 239)。

b) 对于每个简单的左A-模 S，右A-模 $S^*$ 对偶于 S 是简单的，并且从单A-模类集合到映射 $\lambda \mapsto$ cl($\lambda^*$) 定义双射集合类单右A-模。

c) 令 M 为有限生成的左A-模。 右A-模 $M^*$ 对偶 M 是有限生成的，并且与 M 具有相同的长度。此外，对于每个单A-模 S，我们都有 $[M : S] = [M^*: S^*]$。

设M为有限生成A-模。

由 VIII、p. 138、A-模的命题 4 M 是有限生成且射影的；因而，根据II, §2, No. 7、p. 240的推论4，它是自反的。特别是，每个单A-模都是自反的。还可以得出结论，两个有限生成的左模同构当且仅当它们的对偶同构。

令 S 为简单的左A-模。令$(T_i)_{i\in I}$是单右A-模的族，直和是S的对偶$S^*$。由于S是自反的，所以它与$(S^*)^*$同构的，因此与$\prod_{i\in I}T^*_i$同构的。 模 $T_i$ 中的每一个都是自反的；特别是，每 $i\in I$ 就有 $T^*_i\not= 0$。由于单模 S 与$\prod_{i\in I}T^*_i$ 同构的，集合 I 有一个元素，因此$S^*$ 很简单。

由于M是半单并且是有限生成的，所以它是简单子模$S_1, . . . ,S_r$的直和。那么$M^*$同构于$S^*_1, . . . ,S^*_r$族的直和，我们刚刚看到模$S^*_i$是简单的。 断言 c) 紧随其后。

### 3. 因子 / 半单环

在这个小节中，我们考虑半单环A。

我们用$\mathscr{S}$（VIII，p. 51）表示简单的左A-模的类集合；它是有限的（VIII，p. 136，命题 1）。对于每$\lambda \in \mathscr{S}$，我们选择单A-模$S_{\lambda}$类$\lambda$。我们用$\mathfrak{b}_{\lambda}$表示它的湮没子，用$D_{\lambda}$表示它的交换端$_A(S_{\lambda})$的相反的域。

#### 命题 8 {#alg-viii-s8-prop-8 .statement tag=009F}

a) 对于每个 $\lambda \in \mathscr{S},S_{\lambda}$ 都是超过域 $D_{\lambda}$ 的有限维右向量空间。当经过求商时，映射$a\mapsto a_{S_{\lambda}}$定义环同构从$A/\mathfrak{b}_{\lambda}$到End$_{D_{\lambda}}(S_{\lambda})$。

b) 对于每个$\lambda \in \mathscr{S}$，环$A/\mathfrak{b}_{\lambda}$很简单，并且从A到$\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$的典范同态$\psi$是环同构。

环 $A/\mathfrak{b}_{\lambda}$ 与 $A_{S_{\lambda}}$ 同构的。通过VIII、p. 139中的引理 1，这个环就简单了。给定的从$A/\mathfrak{b}_{\lambda}$到End$_{D_{\lambda}}(S_{\lambda})$的映射可以用从$A_{S_{\lambda}}$到$A''_{S_{\lambda}}$的映射来识别。到VIII、p. 139中的命题5，是同构。

A-模$A_s$是半单，忠实且平衡。 同态$\psi$可以从$A_s$的双交换体到$\prod_{\lambda\in\mathscr{S}}$结束$_{D_{\lambda}}(S_{\lambda})$与态射识别，即同构（VIII，p. 86，命题7， c))。

简单的环$A/\mathfrak{b}_{\lambda}$称为型$\lambda$的A的单因子。

#### 例 {#alg-viii-s8-n3-exa-1 .statement tag=009G}

令 K 为代数闭交换域，并令 A 为 K 上有限次数的半单代数。令 $(V_i)_{i\in I}$ 为单A-模的族，使得每个单A-模同构于唯一的 $V_i$。那么 I 是有限集合 (VIII, p. 136, 命题 1), 向量空间 $V_i$ 是域 K 上的有限维，$V_i$ 的交换子等于$K\cdot 1_{V_i}$（VIII、p. 47、定理 1）和映射 $a\mapsto (a_{V_i})_{i\in I}$ 是从 A 到 $\prod_{i\in I}$ End$_K(V_i)$ (命题 8) 的代数同构。

我们将 (VIII, p. 50) 最小双面理想定义为集合或非零的双面理想中的最小元素，按包含排序。在其他字中，A的最小双面理想$\mathfrak{a}$是$(A$，A)-$_sA_d$的子双模。同样，我们将A的最大双面理想定义视为A的真双面理想集合的极大元素。A的最大双面理想$\mathfrak{a}$只是$_sA_d$（VIII，的最大$(A$，A）子双模， p. 48、定义 2)。如果环 A 是简单的，那么理想 0 是 A 的最大双边理想，A 是最小双边理想。

对于任何$\lambda \in \mathscr{S}$，我们用$\mathfrak{a}_{\lambda}$表示A-模$A_s$的型$\lambda$的同型成分。对于 $\mathscr{S}$ 中的任意子集 Λ，我们集合 $\mathfrak{a}_{\Lambda}=\sum_{\lambda\in\Lambda}\mathfrak{a}_{\lambda}$。

#### 命题 9 {#alg-viii-s8-prop-9 .statement tag=009H}

a) 通过包含A的双面理想$\mathscr{S}$子集和集合$\mathscr{B}_A$阶集合$\mathfrak{P}(\mathscr{S})$。 映射$\Lambda \mapsto \mathfrak{a}_{\Lambda}$是从$\mathfrak{P}(\mathscr{S})$到$\mathscr{B}_A$的有序集中的同构。

b) A 的最小两侧理想是理想 $\mathfrak{a}_{\lambda}$。

c) 对于每个$\lambda \in \mathscr{S}$，我们都有$\mathfrak{b}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\{\lambda\}}$，理想$\mathfrak{b}_{\lambda}$是A的最大两侧理想。

d) 对于从 $\mathfrak{a}_{\lambda}$ 到 $A/\mathfrak{b}_{\lambda}$ 的 A-模，从 A 到 $A/\mathfrak{b}_{\lambda}$ 诱导同构的每个 $\lambda \in \mathscr{S}$、典范映射。

断言 a) 源自命题 8，d) 的 VIII，p. 87 应用于A-模 $A_s$。由此可见，A 的最小两侧理想是 $\mathfrak{a}_{\lambda}$，最大两侧理想是理想 $\mathfrak{c}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\lambda}$（对于 $\lambda \in \mathscr{S}$）。

仍然要显示 $\mathfrak{b}_{\lambda}$ 中的等式以及每 $\lambda \in \mathscr{S}$ 的 $\mathfrak{c}_{\lambda}$。令$\lambda$和$\mu$在$\mathscr{S}$中不同。 $S_{\lambda}$A-子模$\mathfrak{a}_\mu S_{\lambda}$是$x\in S_{\lambda}$从$\mathfrak{a}_\mu$到$S_{\lambda}$线性映射$a\mapsto ax$像并。因而，它是零，我们有$\mathfrak{a}_\mu\subset \mathfrak{b}_{\lambda}$。因而，我们有$\mathfrak{c}_{\lambda}\subset \mathfrak{b}_{\lambda}$，最后有$\mathfrak{c}_{\lambda}=\mathfrak{b}_{\lambda}$，因为$\mathfrak{c}_{\lambda}$是A的最大双面理想，而$\mathfrak{b}_{\lambda}$与A不同。

#### 推论{#alg-viii-s8-n3-cor-1 .statement tag=009I}

令 $(A_i)_{i\in I}$ 为从 A 到 $\prod_{i\in I}A_i$ 的简单环和 $f$ 同构的有限族。对于每个$i\in I$，存在$\mathscr{S}$的唯一元素$\varphi (i)$，使得pr$_i\circ f$的核是$\mathfrak{b}_{\varphi(i)}$。 映射$\varphi$是双射从I到$\mathscr{S}$；每$i\in I$从$A/\mathfrak{b}_{\varphi(i)}$到$A_i$映射$_i\circ f$诱导同构$f_i$。

因而，$f$是从A到$\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$的典范同构的合成和从$\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$到$\prod_{i\in I}A_i$的同构从半单环的分解的$f_i($“唯一性推导出来乘积简单的环”）。

让我们证明一下推论。设 $i\in I$；用 $\mathfrak{b}'_i$ 表示 pr$_i\circ f$ 的核。由于简单的环$A_i$与$A/\mathfrak{b}'_i$同构，因此A的双面理想$\mathfrak{b}'_i$极大。到命题 8，c)，因此存在$\mathscr{S}$的唯一元素$\varphi (i)$，这样我们就有$\mathfrak{b}'_i=\mathfrak{b}_{\varphi(i)}$。当经过为商时，从 $A/\mathfrak{b}_{\varphi(i)}$ 到 $A_i$ pr$_i\circ f$ 定义同构 $f_i$。此外，如果$i\not=j$和$\cap_{i\in I}\mathfrak{b}'_i= 0$（cf.I, §8, No. 11，p. 110，命题10），我们还有$\mathfrak{b}'_i+\mathfrak{b}'_j= A$。由此和命题 8 可以得出，从I到$\mathscr{S}$，$\varphi$是双射。

#### 命题 10 {#alg-viii-s8-prop-10 .statement tag=009J}

用 Z 表示 A 的中心。对于 $\lambda \in \mathscr{S}$，令 $Z_{\lambda}$ 为域 $D_{\lambda}$ 的中心。

a) 映射 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}}$ 是同构从环 Z 到乘积 $\prod_{\lambda\in\mathscr{S}}Z_{\lambda}$。

b) Z 理想的阶集合 $\mathscr{I}_Z$ 和 A 两侧理想的集合 $\mathscr{B}_A$ 通过包含。 映射$\mathfrak{a}\mapsto \mathfrak{a}A$是从$\mathscr{I}_Z$到$\mathscr{B}_A$的有序集中的同构。 逆同构将 A 的双边理想 $\mathfrak{b}$ 发送到 Z 的理想 $\mathfrak{b}\cap Z$。

这个命题源自VIII的命题8，p. 87应用于A-模$A_s$，其双交换子是A。

#### 推论{#alg-viii-s8-n3-cor-2 .statement tag=009K}

设 B 为环。以下属性是等效的：

(i) 环 B 很简单。

(ii)环B为半单，其中心为域。

(iii) 环 B 为半单，且仅存在一个类 B-简单模。

#### 命题 11 {#alg-viii-s8-prop-11 .statement tag=009L}

让$\lambda \in \mathscr{S}$。 A的同型成分$\mathfrak{a}_{\lambda}$既是型$S_{\lambda}$的$A_s$的同型成分，又是型$S^*_{\lambda}$的$A_d$的同型成分。此外，我们还有

(1) $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}] =$ 暗淡$_{D_{\lambda}}S_{\lambda}$

和

(2) 长(A) = 长(A$^o$)$=\sum_{\lambda\in\mathscr{S}}$暗$_{D_{\lambda}}S_{\lambda}$。

第一个断言是命题6、c)VIII、p. 139的具体情况$M = A_s$。 等式$[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}]$由VIII、p. 140的命题7推出，因为左A-模$A_s$的对偶与右A-模$A_d$同构。由命题 8, a) 和 9, c)、映射 $a\mapsto a_{S_{\lambda}}$ 定义同构至左A-模从 $\mathfrak{a}_{\lambda}$ 至 End$_{D_{\lambda}}(S_{\lambda})$。由于$[A_s: S_{\lambda}]$是由定义、左A-模$\mathfrak{a}_{\lambda}$的长度、关系$[A_s: S_{\lambda}] =$暗淡$_{D_{\lambda}}S_{\lambda}$从VIII的引理2得出， p. 121。最后，通过对$\lambda$取和，从(1)得到关系(2)。

#### 学院{#alg-viii-s8-n3-sch-1 .statement tag=009M}

设 A 为半单环，Z 为中心。以下集合之间存在规范的双射：

a) 简单左A-模类集合$\mathscr{S}(A)$

b) 单右A-模类集合 $\mathscr{S}(A^o)$

c) A 的最小双面理想的集合

d) A 的最大两侧理想的集合

e) 集合 $\mathscr{S}(Z)$ / 类简单 Z 模块

f) Z 的最小理想的集合

g) Z 的最大理想的集合。

因此，对于$\mathscr{S}$（A）的每个元素$\lambda$，存在单右A-模$S^*_{\lambda}$的对应类$\lambda^*$，$S_{\lambda}$的对偶，A的最小双面理想$\mathfrak{a}_{\lambda}$（ 型$\lambda$的$A_s$），A的最大两侧理想$\mathfrak{b}_{\lambda}$（单模$S_{\lambda}$的湮没子），简单Z模类$Z\cap \mathfrak{a}_{\lambda}$，Z的最小理想$Z\cap \mathfrak{a}_{\lambda}$，以及Z 的最大理想$Z\cap \mathfrak{b}_{\lambda}$。

#### 命题 12 {#alg-viii-s8-prop-12 .statement tag=009N}

设M在半单环A和$\mathscr{S}_M\subset \mathscr{S}$的支持上为模，则M的湮没子Ann(M)为双边理想$\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$，M的迹理想$\tau (M)$为双边理想$\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$。特别地，A是Ann(M)的直和和$\tau (M)$。

由定义 (VIII, p. 84)$,\mathscr{S}_M$ 由M 的简单子模类组成。由于模 M 为半单，因此M 的湮没子为湮没子交类 $\lambda$ 模的$\mathfrak{b}_{\lambda}$，对于$\lambda$ 穿过$\mathscr{S}_M$。现在，每 $\lambda \in \mathscr{S}$ (命题 9) 就有 $\mathfrak{b}_{\lambda}=\sum_{\mu\not=\lambda}\mathfrak{a}_\mu$。由于A是$(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$族的直和，M的湮没子确实等于$\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$。

通过定义（VIII，p. 80），理想迹$\tau (M)$是从M到$A_s$由A-线性映射的像生成的$A_s$的A-子模。因为M是半单，所以说$\tau (M)$是由$A_s$的简单子模与类属于到$\mathscr{S}_M$生成的。因此我们有 $\tau (M) =\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$。

#### 推论{#alg-viii-s8-n3-cor-3 .statement tag=009O}

设 M 为模超过半单环 A。以下属性是等效的：

(i) A-模 M 是忠实的。

(ii) M 的支持度等于$\mathscr{S}$。

(iii) A-模 M 为生成的。

事实上，M 忠实的说意味着它的湮没子减少到0，并且当且仅当它的迹等于A（VIII，p. 80，定理1）时，M才是生成的。

### 4.幂等和半单环

设 A 为环。回想一下，如果我们有 $e^2=e$，则 A 的元素 $e$ 被称为幂等（I, §1, No. 4，p. 7）。那么它也是 A 的逆环 $A^o$ 的幂等元素。

#### 命题 13 {#alg-viii-s8-prop-13 .statement tag=009P}

a) A 的左理想 $\mathfrak{a}$ 在 $A_s$ 中承认补充当且仅当 A 中存在幂等 $e$ 使得 $\mathfrak{a}= Ae$。理想的$\mathfrak{a}$由A的元素$x$组成，使得$x=xe$。

b) 令$e$和$f$在A中幂等。当且仅当我们有$ef=e$时，我们才有$Ae\subset Af$。

c) 设 M 为 A-模。则 M 是射影且单生的当且仅当 A 中存在幂等$e$，使得 M 与 $Ae$ 同构的。

A-模 $A_s$ 的自同态是 A 的乘法与元素的对数。A-模 $A_s$ 中的投影算子因此是映射 $x\mapsto xe$ 其中$e$在A中是幂等的。此外，$A_s$的子模是左理想，这样的子模承认补充当且仅当它是投影算子的像（II, §1, No. 9，p. 211， 命题14)。 断言a)如下。

关系 $Ae\subset Af$ 相当于$e\in Af$。根据a)，它等于$e=ef$； 断言 b)如下。

如果 A-模 M 是单生的，则存在满射A-线性映射 $u: A_s\rightarrow M$。此外，如果 M 是射影的，则存在 $A_s$ 的子模 $\mathfrak{a}$ 与 $u$ 的核的补充。然后从$\mathfrak{a}$到M的$u$诱导同构。相反，如果M与$A_s$的直因子同构，则它是单生且射影的。 断言 c) 因此由 a) 得出。

#### 注 1 {#alg-viii-s8-n4-rem-1 .statement tag=009Q}

设$\mathfrak{a}$为A的左理想。由上述证明和集合的II, §1, No. 8、p. 209、映射$e\mapsto A(1-e)$定义双射的命题12推论A 中的幂等 $e$ 使得 A 的左理想 $\mathfrak{b}$ 的 $\mathfrak{a}= Ae$ 到集合使得 $A_s=\mathfrak{a}\oplus \mathfrak{b}$。

#### 注 2 {#alg-viii-s8-n4-rem-2 .statement tag=009R}

令 $e$ 和 $f$ 在 A 中是幂等的。通过命题 13, b)，当且仅当 $ef=e$ 和 $f e=f$ 时，我们才有 $Ae= Af$。因而，如果环 A 是可交换的，则关系 $Ae= Af$ 等价于 $e=f$。这一般不成立，如例$A =\mathbf{M}_2(\mathbf{Z}), e = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$和$f = \begin{pmatrix} 1 & 0 \\ 1 & 0 \end{pmatrix}$所示。

如果 $ee'=$ $e'e= 0$，我们说环 A 中的幂等$e$ 和 $e'$ 是正交的。令 $(e_i)_{i\in I}$ 为 A 中成对正交幂等的有限族。因为我们有

$$
(\sum_ie_i)^2=\sum_ie^2_i+\sum_{i\not=j}e_ie_j=\sum_ie_i
$$

A 的元素 $\sum_{i\in I}e_i$ 是幂等的。

A 中幂等 $e$ 的划分是 A 中成对正交幂等的有限族 $(e_i)_{i\in I}$，使得 $e=\sum_{i\in I}e_i$。如果存在不同于 0 和 $e$ 的成对正交幂等的 $e$ 由……组成中的划分，我们说 A 中的幂等 $e$ 是可分解的；在相反的情况下，我们说它是不可分解的。观察到 0 是可分解幂等的。

#### 命题 14 {#alg-viii-s8-prop-14 .statement tag=009S}

令 $e$ 为 A 中的幂等。

a) 如果$(e_i)_{i\in I}$是$e$中的划分，则A-模$Ae$是家庭$(Ae_i)_{i\in I}$的直和。

b) 令 $(\mathfrak{a}_i)_{i\in I}$ 为 A 的左理想有限族，其中直和 $Ae$。对于$i\in I$，用$e_i$表示$\mathfrak{a}_i$中$e$的分量。那么$(e_i)_{i\in I}$就是$e$的划分，每一个$i\in I$就有$\mathfrak{a}_i= Ae_i$。

c) A-模 $Ae$ 不可分解当且仅当幂等 $e$ 不可分解。

设$(e_i)_{i\in I}$为$e$的划分。对于每个 $i\in I$，我们有

$$
e_ie=\sum_je_ie_j=e^2_i+\sum_{j\not=i}e_ie_j=e_i
$$

因而$Ae_i\subset Ae$。对于每个$i\in I$，我们通过设定$p_i(x) =xe_i$在$Ae$中得到定义一个A线性投影算子$p_i$。如果$i\not=j$，我们就有$p_ip_j= 0$，并且对于$Ae$中的每个$x$，

$$
x=xe=\sum_ixe_i=\sum_ip_i(x)
$$

因而，(II, §1, No. 8，p. 20，命题$12$)$, Ae$是$p_i$的像中的直和。现在，我们有$ee_i=e_ie=e_i$，所以$p_i$中的像是$Ae_i$。这就证明了a）。

取 b) 的记号和假设。让$i\in I$。从$e_i$属于到$Ae$，我们有$e_i=e_ie=\sum_je_ie_j$。由于对于每个$j$，$Ae$是$\mathfrak{a}_j$和$e_ie_j$属于到$\mathfrak{a}_j$的直和，因此对于$i\not=j$，我们有$e_i=e_ie_i$和$e_ie_j= 0$。在其他字中，$(e_i)_{i\in I}$是幂等$e$的划分。根据a)，$Ae$是$Ae_i$的直和。到假设，我们有$Ae_i\subset \mathfrak{a}_i$，$Ae$是$\mathfrak{a}_i$的直和。因而，每 $i\in I$ 就有 $Ae_i=\mathfrak{a}_i$。我们已经证明了b）。

最后，c) 紧随 a) 和 b) 之后。

#### 注 3 {#alg-viii-s8-n4-rem-3 .statement tag=00R8}

应用之前对 A 的逆环的结果，我们特别看到，单生右A-模 M 是射影的，当且仅当 A 中存在幂等 $e$ 使得 M 与 $eA$ 同构的。此外，当且仅当$e$不可分解时，$eA$是不可分解的权利模。

现在假设环 A 为半单，并用$\mathscr{S}$ 表示简单左A-模的类的集合。 A-模$A_s$是半单，$A_s$的每子模是直因子。设$\mathfrak{a}$为A的左理想。由上可知，A中存在幂等$e$，使得$\mathfrak{a}= Ae$，且A-模$\mathfrak{a}$是简单的当且仅当它是不可分解的，即当且仅当$e$不可分解时。

令 $(\mathfrak{m}_i)_{i\in I}$ 为 A 的最小左理想族，这样我们就有 $A_s=\oplus_{i\in I}\mathfrak{m}_i$。到命题 14 时，存在 1 由……组成的划分 $(\varepsilon_i)_{i\in I}$ 不可分解幂等，使得每 $i\in I$ 就有 $\mathfrak{m}_i= A\varepsilon_i$。

对于每个$\lambda \in \mathscr{S}$，令$S_{\lambda}$为类$\lambda$的A-模，并令$\mathfrak{a}_{\lambda}$为A-模$A_s$的型$\lambda$的同型成分。由于 A 是族 $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$ 的直和，因此存在 1 的划分 $(e_{\lambda})_{\lambda\in\mathscr{S}}$，使得每个 $\lambda \in \mathscr{S}$ 都有 $\mathfrak{a}_{\lambda}= Ae_{\lambda}$。对于$\lambda \in \mathscr{S}$，用指标$i\in I$的$I(\lambda )$集合表示，使得单A-模$\mathfrak{m}_i$为型$\lambda$。到命题 4, b) of VIII, p. 65，我们有

$$
\mathfrak{a}_{\lambda}=\bigoplus_{i\in I(\lambda)}\mathfrak{m}_i \tag{3}
$$

幂等$e_{\lambda}$是$\mathfrak{a}_{\lambda}$中1的组成部分，所以$e_{\lambda}=\sum_{i\in I(\lambda)}\varepsilon_i$。

#### 命题 15 {#alg-viii-s8-prop-15 .statement tag=009T}

假设环 A 是半单。

a) 对于每个 $\lambda \in \mathscr{S},e_{\lambda}$ ，唯一元素中心 Z 满足关系 $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ 和$(e_{\lambda})_{S_\mu}= 0$ $\mu\not=\lambda$。

b) 环 Z 中的不可分解幂等是$e_{\lambda}$，Z 的最小理想是$\lambda \in \mathscr{S}$ 的$Ze_{\lambda}$。

c) 设 M 为 A-模和 $(M_{\lambda})_{\lambda\in\mathscr{S}}$ 其同型组分族。与M的分解关联到$M_{\lambda}$（VIII，p. 65）的直和的投影算子族是$((e_{\lambda})_M)_{\lambda\in\mathscr{S}}$，每个$\lambda \in \mathscr{S}$有$M_{\lambda}=\mathfrak{a}_{\lambda}M$。

令$\lambda$和$\mu$在$\mathscr{S}$中不同。我们有$e_{\lambda}\in \mathfrak{a}_{\lambda}$，$\mathfrak{a}_{\lambda}$包含在A-模$S_\mu$的湮没子$\mathfrak{b}_\mu$中（VIII，p. 142，命题9）。因此我们有$(e_{\lambda})_{S_\mu}= 0$。 关系 $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ 紧随其后，因为我们有 $1 =\sum_{\nu\in\mathscr{S}}e_{\nu}$。 断言 a) 则为命题 8 of VIII, p. 141 中的推论。

令$\lambda$位于$\mathscr{S}$中。 A 的双边理想 $\mathfrak{a}_{\lambda}$ 由元素 $x$ 组成，使得 $x=xe_{\lambda}$；因此我们有 $Z\cap \mathfrak{a}_{\lambda}= Ze_{\lambda}$，因而 b) 乘以命题 10，b)。

让我们证明c）。令$x$为M的元素。对于每个$\lambda \in \mathscr{S}$，我们有$e_{\lambda}\in \mathfrak{a}_{\lambda}$。由于从$A_s$到M的映射$a\mapsto ax$是A线性的，所以我们有$\mathfrak{a}_{\lambda}x\subset M_{\lambda}$（VIII，p. 66，命题5），特别是$e_{\lambda}x\in M_{\lambda}$。我们有$1 =\sum_{\lambda\in\mathscr{S}}e_{\lambda}$，因此有$x=\sum_{\lambda\in\mathscr{S}}e_{\lambda}x$。因而，$e_{\lambda}x$是$M_{\lambda}$中$x$的分量。

#### 注 4 {#alg-viii-s8-n4-rem-4 .statement tag=009U}

假设环 A 是半单。令 $(e_i)_{i\in I}$ 为 A 的中心 Z 中非零的幂等的 1 由……组成的划分。如果 Card(I) = Card($\mathscr{S}$)，则 $e_i$ 是 Z 中不可分解的幂等。

### 习题 {#alg-viii-s8-exercises}

§ 8](exercises/s8/)参见[习题。
