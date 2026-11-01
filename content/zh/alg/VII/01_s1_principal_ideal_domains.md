---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 1
section_title: Principal ideal domains
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0360-0365, 0407-0413
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a principal ideal domain
      page: 0
      pdf_page: 360
    - "no": 2
      title: Divisibility in principal ideal domains
      page: 0
      pdf_page: 360
    - "no": 3
      title: Decomposition into irreducible factors in principal ideal domains
      page: 3
      pdf_page: 362
    - "no": 4
      title: Divisibility of rational integers
      page: 5
      pdf_page: 364
    - "no": 5
      title: Divisibility of polynomials in one indeterminate over a field
      page: 5
      pdf_page: 364
statements: 15
exercises: 28
content_sha256: 2883a95acd00321cf329ee0b5aabb28add637b11a2df8a4a2c752de61cf838d6
translated_from: content/en/alg/VII/01_s1_principal_ideal_domains.md
translation_method: google
source_content_sha256: fccb95f1c743016175d920f3d9b4107ca71a6669ffca75cd9cc5695d9f404b32
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1907332b
glossary_version: 34
glossary_terms_sha256: 4845d46bb9abea8b6f3d305d2ea89aed6d896a3f2eea1f4fb95f586415cea8ba
prompt_sha256: d0998a9bd80ce225884eb51dfb88b94167570132d7e43aad0d568af03105692e
---

## § 1。 主理想整环

### 1. 定义共主理想整环

回想一下 (I, p. 104)，如果对于某些 $a \in A$ 具有形式 $(a) = Aa$，则交换环 $A$ 的理想被称为“主要”。

#### 定义 1 {#alg-vii-s1-def-1 .statement tag=070X}

*主理想整环是整环（I，p. 116），其中每个理想都是主要的。*

#### 例 {#alg-vii-s1-n1-exa-1 .statement tag=070Y}

有理数整数的环$\mathbf{Z}$是主理想整环（I，p. 111）。如果$K$是交换域，那么在$K$上的一个不定数中，多项式环$K[X]$是主理想整环（IV，p. 11，命题11）；形式幂级数$K[[X]]$的环也是如此，对于这个环的每个理想都有形式$(X^n)$（IV，p. 38，提案12）。 \* 整数的环在 p 进数域中是主理想整环。 \*

如果$\mathbf{Q}(i)$表示从有理数的域$\mathbf{Q}$通过邻接不可约多项式$X^2 + 1$的根$i$获得域，则元素$a + bi$ $\mathbf{Q}(i)$，其中$a$和$b$是有理整数，形式子环$\mathbf{A}$$\mathbf{Q}(i)$，称为“高斯整数”，即主理想整环 （VII、p. 50、例 7）。相比之下，在域 $\mathbf{Q}(\rho)$ 中，其中 $\rho$ 是 $X^2 + 5$ 的根，子环 $B$ 由……组成元素 $a + bp$（a 和 b 有理数整数) 不是主理想整环（VII、p. 51、例 12）。

多项式环 $K[X, Y]$ 在域 $K$ 的两个不定数中不是主理想整环。事实上，非零的常数是唯一的元素，其中除既是$X$又是$Y$，并且它们都不是生成由$X$和$Y$生成的理想值。

### 2. 主理想整环的整除性

令$A$为主理想整环，令$K$为分数的域（I，p. 116）；我们将看到 $K$ 的主分数理想 (*VI*, p. 6) 的有序群 $\mathscr{P}^*$ 是格序的；更准确地说：

#### 命题 1 {#alg-vii-s1-prop-1 .statement tag=070Z}

*设$K$为主理想整环$A$分数域，并令$(x_i)_{i \in I}$为具有公共的分母$b \in K^*$的$K$元素的族（在其他情况下） 字 $bx_i \in A$ 全部$i$）。然后：*

a) $(x_i)$家族在$K$有gcd。
b) $(x_i)$ 的每个 gcd 都可以用形式 $d = \sum a_i x_i$ 表示，其中 $a_i$ 是 $A$ 的元素，几乎所有的都是零。

事实上，$A$的理想$\sum Abx$是主要的，形式$Ad'$也是如此。把$d' = bd \ (d \in K)$。从关系$d' = \sum a_i b x_i$，我们推导出$d = \sum a_i x_i$，其中$a_i \in A$。因此，$x_i$除$d$中的每个公共的除子。另一方面，由于$bd$是$bx$的公共的除子，根据构造，$d$是$x_i$的公共的除子。

#### 注 {#alg-vii-s1-n2-rem-1 .statement tag=0710}

没有限制的情况下，命题1适用于$A$的元素的任意族$(x_i)$（取$b = 1$），也适用于$K$的元素的任何有限族$(x_i)$（如果$x_i = c_i b_i$与$c_i \in A$且$b_i \in A$，则取$b$为$b_i$的乘积）。

#### 推论{#alg-vii-s1-n2-cor-1 .statement tag=0711}

— 令$(x_i)$为主理想整环$A$的元素的任意族，包含为整环$B$中的子环，并令$d$为$A$中族$(x_i)$的gcd。那么$(x_i)$家族在$B$有gcd，$d$就是其中之一。

事实上，$d$是$B$中$x_i$的公共的除子。另一方面，关系$d = \sum a_i x_i$显示$B$除$d$中$x_i$的每一个公共的除子。

该推论的一个重要应用是当$A = K[X]$和$B = E[X]$时，其中$K$是域，$E$是$K$的扩张（IV，p. 12，Cor.1）。

命题1的第一个断言表明有序的群$\mathscr{P}^*$是晶格有序的（$VI,$p. 10）。特别是元素 $K$ 的每个有限族都承认有一个 lcm。因此，我们可以将$VI$，第10至17页中标记为(DIV)的结果应用到主理想整环。

以下结果是提案 I 的第二个断言的推论 ：

#### 定理 1（《贝祖特的身份》）{#alg-vii-s1-thm-1 .statement tag=0712}

— 主理想整环 $A$ 的元素 $x_i \ (i \in I)$ 是集合互质当且仅当存在 $A$ 的元素 $a_i \ (i \in I)$，其中几乎所有零，这样 $\sum a_i x_i = 1$。

条件的必要性就是命题1。反之，如果$\sum a_i x_i = 1$则$x_i$除的每一个公共的除子都是1，所以1是$x_i$的gcd。

#### 命题 2 {#alg-vii-s1-prop-2 .statement tag=0713}

— 设$a, b, d, m$和$p$为主理想整环$A$的域、分数$K$的元素。
a) « $d$ 是 $a$ 和 $b$ » 的 gcd 等价于 « $(d) = (a) + (b)$ »。
b) « $m$ 是 $a$ 的 lcm，$b$ » 相当于 « $m = (a) \cap (b)$ »。
c) « $p$ 是 $A$ 的不可约元 » 相当于 « $(p)$ 是 $A$ 的非零的最大理想 » 以及 « $(p)$ 是 $A$ 的非零的素理想 »。

我们已经证明了 a)（命题 *1*）。 Since the common multiples of $a$ and $b$ are the elements of $(a) \cap (b)$, and since, by hypothesis, the ideal $(a) \cap (b)$ is principal, say $(a) \cap (b) = (m)$, it follows that $m$ is an Icm of $a$ and $b$, which proves b). 最后，说$p \neq 0$是$A$的不可约元意味着定义（VI，p. *17*）$(p)$是$A$主要理想族$\neq A$的极大元素，按包含排序；由于$A$除了主理想之外没有其他理想，这意味着$(p)$是$A$，从而c)的最大理想，通过VI，p. 17中的注。

在主理想整环 $A$ 中，有限数理想的和（或交）也称为这些理想的 gcd（或 lcm）。

#### 命题 3 {#alg-vii-s1-prop-3 .statement tag=0714}

*设$a, b, c$为主理想整环$A$分数域元素，且令$d$为$a$与$c$的gcd；那么同余$ax \equiv b \pmod{c}$有解$x_0 \in A$当且仅当$d$除$b$；在这种情况下，$A$的元素$x$，其中满足$ax \equiv b \pmod{c}$正是满足$x \equiv x_0 \pmod{cd}$*。

如果$ax \equiv b \pmod{c}$，有$x \in A$，则存在$y \in A$使得$b = ax + cy$，所以$d$除$b$。相反，如果 $d$ 除 $b$，则 $b = ax_0 + cy_0$ 和 $x_0, y_0 \in A$（命题 *1*），所以 $ax_0 \equiv b \pmod{c}$；此外，关系$ax \equiv b \pmod{c}$等价于$a(x - x_0) \equiv 0 \pmod{c}$；把$a = da'$和$c = dc'$放在一起，后者就变成了$a'(x - x_0) \equiv 0 \pmod{c'}$。但这是等价的（对于$x \in A$）$x - x_0 \equiv 0 \pmod{c'}$，因为$a'$和$c'$是互质的（VI，p. 14，命题*10*（DIV）和VI，p. 15，Cor.2到命题11） （DIV））。

#### 命题 4 {#alg-vii-s1-prop-4 .statement tag=0715}

*令$(a_i)$、$i \leq n$为主理想整环$A$的成对互质元素的有限族。那么典范同态 (I, p. 110) 从 $A / \left( \prod_{r=1}^n a_r \right)$ 到乘积 $\prod_{r=1}^n A/(a_r)$ 就是$A$-代数的同构。*

这是从I、p. 110、提案 9 和提案 2 *a)* 得出的。

如果不假设 $a_i$ 是成对互质的，则命题 4 的结论无效（cf. VII、p. 24、命题 9）。

### 3. 分解化为主理想整环中的不可约因子

我们现在将与分解相关的VI、p. *18*的结果应用到不可约元、主理想整环。根据命题2，$A$的元素$p \neq 0$是不可约的当且仅当环$A/(p)$是域（I，p. *115*，Cor.1），即当且仅当同余$ax \equiv b \pmod{p}$对于每个$b \in A$和每个$a \in A$，在$A$中承认解，这不是$p$的倍数。

#### 定义 2 {#alg-vii-s1-def-2 .statement tag=0716}

*令$A$为整环。 $A$的不可约元的代表的系统是$A$的不可约元的$(p_\alpha)$家族，使得$A$的每个不可约元恰好是一个$p_\alpha$的关联。*

#### 定理 2 {#alg-vii-s1-thm-2 .statement tag=0717}

— 令$\mathbf{A}$为主理想整环，令$(p_\alpha)$为系统，是$\mathbf{A}$的不可约元的代表。那么$A$的分数的域的每一个非零元素$x$都可以唯一地表达为形式

$$
x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}},
$$

其中$u$是$\mathbf{A}$的可逆元，并且$n_{\alpha}$是整数，其中几乎所有的都是零。对于$x$到属于到$\mathbf{A}$，所有$n_{\alpha}$为正是必要且充分的。

我们将定理关于分解作为不可约元的和（VI，p. 18，Th.2），其中上面的叙述只是一个翻译。由于$\mathscr{P}^*$是一个群有序的格子，因此我们足以证明$\mathbf{A}$包含极大元素的主理想的每个非空集合，在阶中来检查这个假设定理确实很满意；现在从下一个引理开始：

#### 引理 1 {#alg-vii-s1-lem-1 .statement tag=0718}

令$A$为环，使得$A$的每个左理想都是有限生成的。那么$\mathbf{A}$的左理想中的每一个非空集合$\Phi$，按包含排序，都有极大元素。

根据佐恩的引理（集合理论，III，p. 154，Th.2）足以证明$\Phi$是归纳性的。现在，如果$(a_\lambda)$是$\Phi$的元素的全序族，那么理想$a_i$的并$a$是$\mathbf{A}$的左理想，因此承认生成元$(a_i)_{1 \leq i \leq n}$的有限系统。由于每个$a_i$属于到一个理想$a_{\lambda_i}$，并且由于家庭$(a_\lambda)$是完全有序的，因此理想$a_{\lambda_i}$的$a_i$所有属于到最大的，例如$a_1$。然后$a = a_1$属于到$\Phi$，因此确实是归纳集合。

稍后我们将研究那些环$B$，称为诺特环，使得$B$包含极大元素的理想中的每一个非空集合。

#### 注 {#alg-vii-s1-n3-rem-1 .statement tag=0719}

$(u, (n_\alpha))$族被称为$x$的分解为不可约因子；通过滥用语言，我们还说公式 (1) 是$x$ 的分解变为不可约因子。如果$x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}}$和$y = v \prod_{\alpha} p_{\alpha}^{m_{\alpha}}$是$x$和$y$的分解不可约因子，那么$x$到除$y$的充分必要条件就是$n_{\alpha} \leq m_{\alpha}$，对于所有$\alpha$；由此我们推导出公式

$$
\gcd(x, y) = \prod_{\alpha} p_{\alpha}^{\inf(n_{\alpha}, m_{\alpha})}
$$
$$
\operatorname{lcm}(x, y) = \prod_{\alpha} p_{\alpha}^{\sup(n_{\alpha}, m_{\alpha})}
$$

性质用Th表示。对于环比主理想整环更一般的类，2 成立；稍后我们将把它们作为独特的因式分解域来研究；我们将看到任意多个不定式中的多项式环和形式幂级数环都是唯一的因式分解域（Comm. Alg.，VII, § 3）。

### 4. 有理数整数的整除性

正如截面 1中指出的，有理整数的环$\mathbf{Z}$是主理想整环；其分数的域为$\mathbf{Q}$。 $\mathbf{Z}$可逆元乘法群$U$有两个元素1和$-1$。 The group $Q_+^*$ of rational numbers $> 0$ contains precisely one element from each class of associate elements of $\mathbf{Q}$; it is thus isomorphic to the multiplicative group $\mathscr{P}^* = Q^*/U$ of principal fractional ideals of $\mathbf{Q}$, with which it is usually identified. 特别是，当gcd或lcm用于域$\mathbf{Q}$（相对于环$\mathbf{Z}$）时，可以理解为元素$\geqslant 0$；这个约定使我们能够谈论有理数族的gcd和lcm。

$\mathbf{Z}$中的不可约整数$> 0$正是我们所说的素数数（I，p. 50）（它们是有时称为有理素数数）；因此$\mathbf{Z}$的每个不可约元都是形式$p$或$-p$，其中$p$是素数数，素数数的集合$P$是系统的代表不可约元共$\mathbf{Z}$。

#### 命题 5 {#alg-vii-s1-prop-5 .statement tag=071A}

— 素数数的集合是无限的。

Indeed, given an arbitrary finite family $(p_i)$ ($1 \leq i \leq n$) of distinct prime numbers, any prime divisor $q$ of the number $\left( \prod_{i=1}^n p_i \right) + 1$ (which is $> 1$) is distinct from all the $p_i$, for otherwise it would divide 1.

### 5. 多项式在域上的一个不定式的整除性

多项式环 $K[X]$ 在交换域 $K$ 的一个不定数中是主理想整环（IV、p. 11，命题 11）。它的分数的域是$X$中的有理函数的域$K(X)$，系数来自$K$。 次数 0 多项式的环 $K[X]$ 包含子环，即常数域，用$K$标识； $K^*$的元素在$K$中是可逆的，因此在$K[X]$中是可逆的；反之公式 $\deg(uv) = \deg(u) + \deg(v)$ 表明每个可逆多项式都有次数 0；因而，$K[X]$的可逆元的群$U$正好是$K^*$。因而，两个关联多项式仅相差非零的常数因子；特别是关联多项式包含的每个类都是唯一的一元多项式。 乘法群 $K(X)^*$的子群由一元多项式生成，因此包含唯一元素来自关联有理函数的每个类，因此与群同构

$$
\mathscr{P}^* = K(X)^*/U
$$

$K(X)$ 的主分数理想。特别是，每当提到域$K(X)$（相对于环$K[X]$）中的gcd或lcm时，通常会理解这些是一元多项式的商（或0）；这个约定使我们能够谈论有理数族函数的gcd或lcm。

$K[X]$的不可约元正是通常意义上的不可约多项式（IV，p. 13，Def.2），而单调不可约多项式的集合是$K[X]$的不可约元的代表的系统。

第一个次数多项式始终是不可约的。如果 $K$ 是代数闭域，则逆命题为真（V，p. 19，命题 1）；因而，在这种情况下，$K[X]$中次数$n$的每个多项式$p(X)$都可以唯一地写成形式（最多因子的阶）

$$
p(X) = c(X - a_1)(X - a_2) \ldots (X - a_n)
$$

其中$c$和$a_i$是$K$的元素。

#### 命题 6 {#alg-vii-s1-prop-6 .statement tag=071B}

对于任何域 $K$，$K[X]$ 中的单调不可约多项式的 *集合* 是无限的。

事实上，给定不同单调不可约多项式的任意非空有限族$(p_i)$（$1 \leq i \leq n$），首一多项式$\left( \prod_{i=1}^n p_i \right) + 1$是不可逆的，并且该多项式的任何单调不可约因子$q$必然与所有$p_i$不同，否则它会除1。

### 习题{#alg-vii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
