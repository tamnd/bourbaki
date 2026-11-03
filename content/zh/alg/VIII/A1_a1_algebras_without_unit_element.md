---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Algebras without Unit Element
appendix: true
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.435-A VIII.446
pdf_pages: 0452-0463
extraction: native
subsections:
    - "no": 1
      title: Regular Ideals
      page: 435
      pdf_page: 452
    - "no": 2
      title: Adjunction of a Unit Element
      page: 437
      pdf_page: 454
    - "no": 3
      title: The Radical of an Algebra
      page: 439
      pdf_page: 456
    - "no": 4
      title: Density Theorem
      page: 442
      pdf_page: 459
statements: 20
exercises: 15
content_sha256: ab8f4b606e69ce8ebe726ba438c983d6cb764338434aab8fd7fd498176656eda
translated_from: content/en/alg/VIII/A1_a1_algebras_without_unit_element.md
translation_method: google
source_content_sha256: 98c6a5e57906681f8c0a6b353e8a358c25cc514a68622fa99dc2d3817a1b28f4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 78c39d72b1849f87af20459dec5f7bd2aecab2a616c461bb9f7c8456961923e7
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 附录 1 代数无单位元

在这个附录中，$k$就是交换环； $k$-代数被假定为结合的，但不一定是单位的。

### 1. 常规理想

设 A 为 $k$ 代数。回想一下 (III, §1, No. 2, p. 430)，A 的左理想是 A 的$k$子模$\mathfrak{a}$，使得关系$a\in A, x\in \mathfrak{a}$隐含$ax\in \mathfrak{a}$。我们右理想和双面理想的定义概念同样如此。如果 A 是$k$-代数且 $\mathfrak{a}$ A 的双面理想，则当经过到商时，定义中的乘法 $k$-代数结构在$k$-模 $A/\mathfrak{a}$ 上（前述）。

如果 A 的左理想是包含的 A 的真左理想的集合的极大元素，则该左理想称为最大。

#### 定义 1 {#alg-viii-a1-def-1 .statement tag=00P4}

令 A 为 $k$ 代数，$\mathfrak{a}$ A 的左理想。A 的元素 $u$，使得每个 $a\in A$ 的 $au-a$ 属于到 $\mathfrak{a}$ 称为模右单位 $\mathfrak{a}$。如果存在模右单位$\mathfrak{a}$，我们说理想的$\mathfrak{a}$是正则的。

同样，如果 A 具有左模单位 $\mathfrak{b}$，即元素 $v$，使得对于每个 $a\in A$ 都有 $va-a\in \mathfrak{b}$，则我们说 A 的右理想 $\mathfrak{b}$ 是正则的。当一个理想是双面的时，需要指定它是正则为左理想还是右理想。

当代数 A 为单位时，对于 A 的每个左理想 $\mathfrak{a}$，A 的单位元为模右单位 $\mathfrak{a}$；在这种情况下，A 的每个左（或右）理想都是正则的。另一方面，如果 A 是 $k$ 代数，且元素均为幂零，则 A 是 A 的唯一（左或右）正则理想。

令 $\mathfrak{a}$ 为 A 和 $u$ 模右单位 $\mathfrak{a}$ 的正则左理想。如果$\mathfrak{b}$是包含$\mathfrak{a}$的左理想，则$u$是模右单位$\mathfrak{a}$，所以$\mathfrak{b}$是正则。因此，A 的最大且正则的左理想是 A 的正则真左理想的集合的极大元素。此外，包含于 $\mathfrak{a}$ 的左理想 $\mathfrak{b}$ 是正确的当且仅当 $u$ 不属于到 $\mathfrak{b}$。 包含于$\mathfrak{a}$的真左理想$\mathfrak{b}$的集合，按包含排序，因此是归纳集合。将集合理论、III, §2, No. 4、p. 154 中的定理 2 应用于此集合给出以下结果。

#### 命题 1 {#alg-viii-a1-prop-1 .statement tag=00P5}

A 的每个正则左（或右）理想都包含在正则最大左（或右）理想中。

#### 命题 2 {#alg-viii-a1-prop-2 .statement tag=00P6}

设 A 是可交换的 $k$-代数。 A 的理想 $\mathfrak{a}$ 是正则最大理想，当且仅当伪环 $A/\mathfrak{a}$ (I, §8, No. 1, p. 98) 为域。

A 的元素$u$是（右或左）模单位$\mathfrak{a}$当且仅当$A/\mathfrak{a}$中$u$的典范像是代数$A/\mathfrak{a}$的单位元。因此，理想的$\mathfrak{a}$是正则的当且仅当代数$A/\mathfrak{a}$是单位的。假设满足这些条件。

映射$\mathfrak{b}\mapsto \mathfrak{b}/\mathfrak{a}$是从包含$\mathfrak{a}$的代数A的理想集合到代数$A/\mathfrak{a}$的理想集合的双射。 这些是环$A/\mathfrak{a}$的理想，因为这个代数是单位的。 最后，通过I, §9, No. 1、p. 115、环$A/\mathfrak{a}$的定理 1 是域当且仅当它是非零的且其唯一理想是0和它本身。 命题如下。

#### 例 1 {#alg-viii-a1-n1-exa-1 .statement tag=00P7}

令V为无限维向量空间超过交换域K。令End$^f_K(V)$为有限秩的自同态的End$_K(V)$由……组成的K-子代数。设W为V的线性子空间，并令$\mathfrak{a}_W$为End$^f_K(V)$的元素的集合，其核包含W；它是End$^f_K(V)$的左理想。 End$^f_K(V)$的元素$u$是模右单位$\mathfrak{a}_W$当且仅当我们对于每个$x\in W$都有$u(x) =x$。这样的元素$u$存在，即$\mathfrak{a}_W$是正则的，当且仅当W是有限维的。当且仅当 W 具有维数 1 时，理想的 $\mathfrak{a}_W$ 才是最大且正则的。

#### 例 2 {#alg-viii-a1-n1-exa-2 .statement tag=00P8}

令 T 为局部紧致空间，并令 $\mathscr{C}_0(T)$ 为从 T 到 $\mathbf{C}$ 的连续映射的交换 $\mathbf{C}$ 代数，在无穷大处趋于 0（Gen. Top.、X, §4, No. 4、p. 316）；当且仅当 T 是紧的时它才是单位的。设F为T的闭子集，并令$\mathfrak{a}_F$为$\mathscr{C}_0(T)$的元素的集合，其中限制到F为零函数；这是$\mathscr{C}_0(T)$的理想值。 $\mathscr{C}_0(T)$的元素$u$是模单位$\mathfrak{a}_F$当且仅当我们对于每个$t\in F$都有$u(t) = 1$。这样的元素$u$存在，即$\mathfrak{a}_F$是正则的，当且仅当F是紧的。 映射 $t\mapsto \mathfrak{a}_{\{t\}}$ 是$\mathscr{C}_0(T)$ (TS, I, §3, n$^o2$, p. 32, 推论 1) 的正则最大理想的双射到集合。假设T不是紧的，用紧支持的函数的$\mathscr{C}_0(T)$由……组成的$\mathfrak{a}$子集表示；那么$\mathfrak{a}$是$\mathscr{C}_0(T)$的一个理想，并且不包含在$\mathscr{C}_0(T)$的任何正则理想中。

#### 例 3 {#alg-viii-a1-n1-exa-3 .statement tag=00P9}

令$L^1(\mathbf{R})$为局部紧致群$\mathbf{R}$的卷积代数。回想一下 (cf. Int., VIII, §4, No. 5, p. 38)，$L^1(\mathbf{R})$ 是 $\mathbf{R}$ 上函数的类的空间，对于勒贝格测度可积。两个函数$f$和$g$类乘积是由公式定义的函数$f*g$类

$$
(f*g)(s) =\int_{-\infty}^{+\infty}f(t)g(s-t)dt
$$

几乎每$s\in \mathbf{R}$。 代数 $L^1(\mathbf{R})$ 不是单位。对于$\mathbf{R}$中的任意$a$，用$L^1(\mathbf{R})$满足的元素$f$$\mathfrak{m}_a$集合表示

$$
\int_{-\infty}^{+\infty}f(t)e^{-iat}dt= 0
$$

由TS可知，II, §3、n$^o2$、p. 252、定理 1、映射$a\mapsto \mathfrak{m}_a$是代数正则极大理想从$\mathbf{R}$到集合的双射 $L^1(\mathbf{R}).*$

### 2. 伴随 / 单位元

设 A 为 $k$ 代数。 在III, §1, No. 2、p. 431中，我们定义了从A通过单位元$e$的伴随推导出来的单位代数$\widetilde{A}$。 我们认同 A 具有双面理想 $\widetilde{A}$。 $k$-模$\widetilde{A}$是子模$ke$和A的直和。

#### 命题 3 {#alg-viii-a1-prop-3 .statement tag=00PA}

a) 令$\widetilde{\mathfrak{a}}$为$\widetilde{A}$的左理想，使得$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$。我们集合$\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$。 A 存在元素 $u$，使得 $u-e$ 属于到 $\widetilde{\mathfrak{a}}$。如果$u$是元素，那么它是A模$\mathfrak{a}$的右单位，我们有$\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$；特别是，理想的$\mathfrak{a}$是有规律的。

b) 相反，令 $\mathfrak{a}$ 为 A 的正则左理想，$u$ 为 A 模$\mathfrak{a}$ 的右单位。 集合$\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$。那么$\widetilde{\mathfrak{a}}$是$\widetilde{A}$的左理想，使得$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$，我们有$\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$。

c) 如果$k$是域，则条件$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$等价于说，$\widetilde{\mathfrak{a}}$不包含在A中。

在a)的假设下，$\widetilde{A}$的元素$e$可以与$u\in A$和$u-e\in \widetilde{\mathfrak{a}}$写成$(e-u)+u$。令$x=\lambda e+a$为$\widetilde{A}$的元素，其中$\lambda \in k$和$a\in A$；如果$x$属于到$\widetilde{\mathfrak{a}}$，那么属于到$\mathfrak{a}$的元素$y=a+\lambda u=x+\lambda (u-e)$，我们有$x=y-\lambda (u-e)$；这就证明了等式$\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$。此外，对于A中的每个$a$，属于到$\mathfrak{a}$中的元素$au-a=a(u-e)$，所以$u$是模右单位$\mathfrak{a}$。这就证明了断言a)。

令$\mathfrak{a}$和$u$如b)中所示。由于$\widetilde{A}$是A和$k(u-e)$的直和，所以我们有$\widetilde{\mathfrak{a}}+ A =\widetilde{A}$和$\widetilde{\mathfrak{a}}\cap A =\mathfrak{a}$。 $\widetilde{\mathfrak{a}}$的每个元素都是形式$x+\lambda (u-e)$以及$x\in \mathfrak{a}$和$\lambda \in k$。对于每 $a\in A$，我们有

$$
a(x+\lambda (u-e)) =ax+\lambda (au-a)
$$

由于$u$是A模$\mathfrak{a}$的右单位，和$ax+\lambda (au-a)$属于到$\mathfrak{a}$，所以$\widetilde{\mathfrak{a}}$是A的左理想。这证明了b)。

最后，如果$k$是域，那么A是$\widetilde{A}$中的超平面，$\widetilde{A}$是$\widetilde{\mathfrak{a}}$和A的和当且仅当$\widetilde{\mathfrak{a}}$不包含在A中。

#### 推论 {#alg-viii-a1-n2-cor-1 .statement tag=00PB}

A 的正则左理想是形式 $A\cap \widetilde{\mathfrak{a}}$ 的理想，其中 $\widetilde{\mathfrak{a}}$ 是 $\widetilde{A}$ 的左理想，使得 $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$。

#### 命题 4 {#alg-viii-a1-prop-4 .statement tag=00PC}

a) 设$\mathfrak{a}$为A的正则最大左理想。存在$\widetilde{A}$的唯一左理想$\widetilde{\mathfrak{a}}$，使得$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$和$\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$。这个理想是最大的，并且不包含 A.

b) 映射 $\widetilde{\mathfrak{a}}\mapsto \widetilde{\mathfrak{a}}\cap A$ 是从 $\widetilde{A}$ 的最大左理想的集合而非包含 A 到 A 的常规最大左理想的集合的双射。

令 $\mathfrak{a}$ 为 A 的正则最大左理想。通过命题 3，a)，$\widetilde{A}$ 的左理想 $\mathfrak{b}$，使得 $\mathfrak{b}+ A =\widetilde{A}$ 和 $\mathfrak{b}\cap A =\mathfrak{a}$ 为理想 $\mathfrak{a}+k(u-e)$，其中 $u$ 为模右单位 $\mathfrak{a}$。因此，为了证明$\widetilde{\mathfrak{a}}$的唯一性，只需证明A模$\mathfrak{a}$的两个右单位$u$和$u'$模$\mathfrak{a}$全等即可。让我们通过反证推理，假设$u-u'$不属于到$\mathfrak{a}$。 公式 $x(u-u') = (xu-x)-(xu'-x)$ 表明我们有 $A(u-u')\subset \mathfrak{a}$；由此可见，$\mathfrak{a}+k(u-u')$是包含$\mathfrak{a}$的左理想，与$\mathfrak{a}$不同。由于 $\mathfrak{a}$ 是最大的，因此我们有 $\mathfrak{a}+k(u-u') = A$，因此 AA $\subset \mathfrak{a}$。对于每个 $x\in A$，我们有 $x\equiv xu$ (mod $\mathfrak{a}$)，因此通过上面的$x\in \mathfrak{a}$，即与……矛盾假设 $\mathfrak{a}\not= A$。

因而，存在$\widetilde{A}$的唯一左理想$\widetilde{\mathfrak{a}}$，使得$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$和$\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$。令$\mathfrak{b}$为$\widetilde{A}$包含于$\widetilde{\mathfrak{a}}$的真左理想。那么$\mathfrak{b}\cap A$是包含$\mathfrak{a}$的真左理想。因此它等于$\mathfrak{a}$，因为$\mathfrak{a}$是最大的，这意味着$\mathfrak{b}=\widetilde{\mathfrak{a}}$乘以引理 2 of VIII，p. 4。这就证明$\widetilde{\mathfrak{a}}$是$\widetilde{A}$的极大理想；对于这样的理想，条件$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$意味着$\widetilde{\mathfrak{a}}$不包含A。

尚待证明，如果$\widetilde{\mathfrak{a}}$是$\widetilde{A}$的最大左理想，且不是包含A，则A的左理想$\mathfrak{a}= A\cap \widetilde{\mathfrak{a}}$最大。令$\mathfrak{b}$为包含$\mathfrak{a}$的真左理想。令 $u$ 为模右单位 $\mathfrak{a}$，使得 $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ (命题 3)。也是模右单位$\mathfrak{b}$；用$\widetilde{\mathfrak{b}}$表示$\widetilde{A}$的理想$\mathfrak{b}+k(u-e)$。到命题 3，b)，我们有$\mathfrak{b}= A\cap \widetilde{\mathfrak{b}}$。理想的$\widetilde{\mathfrak{a}}$等于$\mathfrak{a}+k(u-e)$，包含在$\widetilde{\mathfrak{b}}$中，因此等于$\widetilde{\mathfrak{b}}$，因为$\widetilde{\mathfrak{b}}$与$\widetilde{A}$不同，并且$\widetilde{\mathfrak{a}}$是最大值。因而，我们有 $\mathfrak{a}=\mathfrak{b}$，并且 $\mathfrak{a}$ 是最大的。

我们留给读者将命题 3 和 4 翻译成正确的理想。

### 3. 代数的根

设 A 为 $k$ 代数。 A 上的左拟模是一个 $k$ 模 M，其在伪环 A 上具有左拟模的结构（II、附录、No. 2、p. 378），这样我们就有 $a(\lambda x) =\lambda (ax) = (\lambda a)x$ 对应于 $\lambda \in k$， $a\in A$和$x\in M$。同样，我们对 A 定义右伪模。

设 M 大于 A 的左拟模；我们定义 M 上的左$\widetilde{A}$模块结构被设定称为规范

$(\lambda e+a)x=\lambda x+ax$ 换$\lambda \in k, a\in A, x\in M$。

相反，通过将运算符的环限制为$k$和A，每个左$\widetilde{A}$-模块都被规范赋予，其中左拟模的结构在A上。因而，左拟模的结构种在A上并且模在A上$\widetilde{A}$ 等效（集合理论、IV, §1, No. 7、p. 262）。

设M在A上左拟模，并令N为M的$k$子模。则N是M的$\widetilde{A}$子模当且仅当它在A的作用下稳定；然后我们说 N 是 M 的子伪模。

就像环的情况一样，我们在A上定义左拟模$A_s$以及右边的伪模$A_d$。 A 的左（或右）理想是子伪模或 $A_s$（或 $A_d$）。

令 $\mathfrak{a}$ 为 A 和 $u$ 模右单位 $\mathfrak{a}$ 的正则左理想。 集合$M = A_s/\mathfrak{a}$，并用$z$表示M中$u$的像。我们有$M = Az$，$\mathfrak{a}$是$z$的湮没子。

相反，令 M 为 A 上的左拟模，并令 $z$ 为 M 的元素，使得 $M = Az$。那么A存在元素$u$使得$z=uz$。对于每个$a\in A$，我们有$(au-a)z= 0$，因而$z$的$au-a$属于到湮没子$\mathfrak{a}$。因而，$\mathfrak{a}$是A的正则左理想，元素$u$为模右单位$\mathfrak{a}$，当经过到商时，映射$a\mapsto az$定义同构 $A_s/\mathfrak{a}$ 至 M。

#### 定义 2 {#alg-viii-a1-def-2 .statement tag=00PD}

如果我们有 AM $\not= 0$ 并且 0 和 M 是 M 的唯一子伪模，我们就说 A 上的伪模 M 是简单的。

从对应到说，$\widetilde{A}$模块M很简单，并且它的湮没子不包含A。当A是环并且M是A-模时，我们有AM = M，所以定义2重合定义 1 个，共 VIII、p. 45。

#### 命题 5 {#alg-viii-a1-prop-5 .statement tag=00PE}

a) 令$\mathfrak{m}$为A的正则最大左理想。则伪模$A_s/\mathfrak{m}$很简单，并且存在$A_s/\mathfrak{m}$与湮没子$\mathfrak{m}$的非零元素。

b) 设M是简单的伪模，$x$是M的非零元素。我们有$M = Ax$，湮没子$\mathfrak{m}$是$x$的正则最大左理想，当经过到商时， 映射 $a\mapsto ax$ 定义同构从 $A_s/\mathfrak{m}$ 到 M。

c) 令 M 为伪模，不减少为 0。那么 M 是简单的，当且仅当对于 M 的每个非零元素 $x$，我们都有 $M = Ax$。

令$\mathfrak{m}$为A的正则最大左理想。我们已经看到，$A_s/\mathfrak{m}$存在非零元素$z$，其中湮没子等于$\mathfrak{m}$，且$Az= A_s/\mathfrak{m}$；特别是，我们有 $A(A_s/\mathfrak{m})\not= 0$。此外，$A_s/\mathfrak{m}$的每个子伪模都是形式$\mathfrak{n}/\mathfrak{m}$，其中$\mathfrak{n}$是包含$\mathfrak{m}$的左理想。由于$\mathfrak{m}$是最大的，唯一的可能性是$\mathfrak{n}=\mathfrak{m}$和$\mathfrak{n}= A$，因此伪模$A_s/\mathfrak{a}$很简单。这就证明了a）。

在b)的假设下，M的元素$y$的集合使得$Ay= 0$是与M不同的M的子伪模，因此减少到0。因而，$Ax$是M的非零的子伪模，其中意味着$M = Ax$。 断言 b) 然后从注之前定义 2 得出。

设 M 为非零的伪模。假设对于 M 的每个非零元素 $x$，我们都有 $Ax= M$。特别是，我们有 AM $\not= 0$。令N为M的非零的子伪模，并令$x$为N的非零元素。我们有$Ax= M$，因此N = M。因此M是简单的。相反，如果 M 很简单，那么对于 b) 的每个$x\not= 0$，我们都有 $M = Ax$。

#### 定义 3 {#alg-viii-a1-def-3 .statement tag=00RT}

$k$-代数 A 的根基，用 $\Re (A)$ 表示，是 A 的正则最大左理想的交。

当A为环时，A的每个左理想都是正则的，因此根基重合的定义和VIII的定义2，p. 154。

#### 例 1 {#alg-viii-a1-n3-exa-1 .statement tag=00PF}

$k$-代数端$^f_k(V)$的根基减少到0（VIII，p. 436，例1）$.*$同样适用于代数$\mathscr{C}_0(T)$和$L^1(\mathbf{R}).*$

#### 例 2 {#alg-viii-a1-n3-exa-2 .statement tag=00PG}

设 A 为伪环，其中所有元素都是幂零的。 A 的根基等于 A，因为 A 是唯一的正则左理想。

命题 5 立即意味着以下结果。

#### 命题 6 {#alg-viii-a1-prop-6 .statement tag=00PH}

代数A的根基是简单的伪模的湮没子交。特别是，它是 A 的双面理想。

#### 命题 7 {#alg-viii-a1-prop-7 .statement tag=00PI}

A的根基是$\widetilde{A}$的根基在A上的迹；它也等于反代数$A^o($的根基，即等于A)的正则最大右理想的交。如果环$k$没有根基，则A的根基等于$\widetilde{A}$。

等式 $\Re (\widetilde{A})\cap A =\Re (A)$ 由VIII、p. 438、b) 中的命题 4 得出。由于$\widetilde{A}$和$\widetilde{A}^o$具有相同的根基（VIII、p. 156、推论 1），因此等式$\Re (A) =\Re (A^o)$如下。如果$k$没有根基，则$\widetilde{A}$包含A的最大左理想的交等于A。因而，$\Re (\widetilde{A})$包含在A中，因此等于$\Re (A)$。

#### 注 {#alg-viii-a1-n3-rem-1 .statement tag=00PJ}

设A的$x$和$y$为元素；我们说$x$是$y$的左逆，或者$y$是$x$的右逆，如果$\widetilde{A},x-e$是$y-e$的左逆，也就是说，如果我们有$x+y=xy$。通过命题 7 和 Jacobson 的定理 (VIII, p. 156, 定理 1)，A 的根基由 A 的元素 $x$ 组成，使得 $ux-e$ 可逆$\widetilde{A}$对应于$\widetilde{A}$中的每$u$。由于我们有$(a+\lambda e)x-e=ax+\lambda x-e$（对于$a\in A,\lambda \in k$），A的根基是A的元素$x$的集合，这样对于每个$a\in A$和$\lambda \in k$，$ax+\lambda x$在A中有一个左逆。

### 4. 稠密性定理

设 A 为 $k$ 代数。如果左拟模 M 是简单左拟模族的直和，则称为半单。

#### 引理 1 {#alg-viii-a1-lem-1 .statement tag=00PK}

设 M 为半单左 A 伪模。设B是$\widetilde{A}$模M的双交换子。则M的每个A子伪模是M的B-子模。

$\widetilde{A}$模M是半单。设N是M的A子伪模。那么N是M的$\widetilde{A}$子模。通过VIII、p. 56的推论2，存在A-模M的投影算子$p$和像N。因为我们有关系 $pb=bp$ 对于每一个 $b\in B$，我们得到 N 是 M 的 B-子模。

#### 引理 2 {#alg-viii-a1-lem-2 .statement tag=00PL}

设M为半单左A伪模块，并令$x$为M的元素。存在元素$a\in A$使得$ax=x$。

令 N 为左 A 伪模块 $\widetilde{A}x/Ax$。它满足AN$=\{0\}$。将VIII、p. 56中的推论 3 应用于$\widetilde{A}$模块M和$\widetilde{A}x$，A-伪模块N为半单。到定义时，N 中的每个简单子伪模 S 都满足 AS $\not=\{0\}$。因而，伪模 N 是零，我们得到$x\in Ax$。

#### 定理 1（雅各布森的稠密性定理）{#alg-viii-a1-thm-1 .statement tag=00SD}

设 M 为半单左 A 伪模块。令$b$为$\widetilde{A}$模块M的双交换子的元素。令$F =\{x_1, . . . , x_n\}$为M的有限子集。则存在元素$a\in A$，使得对于每个$i\in [1, n]$有$bx_i=ax_i$。

令 B 为 $\widetilde{A}$ 模块 M 的双交换子。A 伪模块 $M^n$ 为半单。让$\boldsymbol{x}= (x_1, . . . , x_n)\in M^n$。从引理 2 得出 $\boldsymbol{x}\in$ $A\boldsymbol{x}$。 $\widetilde{A}$模$M^n$重合的双交换子与B-模$M^n$同位（VIII，p. 79，命题2）。到引理 1 时，$M^n$ 的 A 子伪模$A\boldsymbol{x}$ 因此是 $M^n$ 的B-子模。因此我们包含了$B\boldsymbol{x}\subset A\boldsymbol{x}$。所以存在$a\in A$使得$b\boldsymbol{x}=a\boldsymbol{x}$。结果如下。

### 习题 {#alg-viii-a1-exercises}

参见[习题附录 1](exercises/a1/)。
