---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 4
section_title: Finitely generated modules over a principal ideal domain
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.15-A VII.28, A VII.62-A VII.70
pdf_pages: 0374-0387, 0421-0429
extraction: ocr
subsections:
    - "no": 1
      title: Direct sums of cyclic modules
      page: 15
      pdf_page: 374
    - "no": 2
      title: Content of an element of a free module
      page: 16
      pdf_page: 375
    - "no": 3
      title: Invariant factors of a submodule
      page: 18
      pdf_page: 377
    - "no": 4
      title: Structure of finitely generated modules
      page: 19
      pdf_page: 378
    - "no": 5
      title: Calculation of invariant factors
      page: 20
      pdf_page: 379
    - "no": 6
      title: Linear mappings of free modules, and matrices over a principal ideal domain
      page: 21
      pdf_page: 380
    - "no": 7
      title: Finitely generated abelian groups
      page: 22
      pdf_page: 381
    - "no": 8
      title: Indecomposable modules. Elementary divisors
      page: 23
      pdf_page: 382
    - "no": 9
      title: Duality in modules of finite length over a principal ideal domain
      page: 25
      pdf_page: 384
statements: 40
exercises: 25
content_sha256: d64264de80a22857a60ddab8e1132be888680ac9d0b017fccd631daf2fd2adac
translated_from: content/en/alg/VII/04_s4_finitely_generated_modules_over_a.md
translation_method: google
source_content_sha256: e417e7dc96e464c48ed19a91e2e8d38e2c97d4afc92adb2cc15edbd954a62d34
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: def4c7564e697fae5b4153c3415f85c182b30431a04f56ba38068333088869db
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 有限生成模超过主理想整环

### 1.循环模的直和

设 A 为交换环。回想一下（II，p. 220，命题 22），循环 A-模同构于 *商模* $A/a$，其中 a 是 A 的理想。稍后我们将看到（第 4 节），主理想整环上的每个有限生成模是有限多个循环模的直和。

#### 命题 1 {#alg-vii-s4-prop-1 .statement tag=073N}

— *令 E 为模超过交换环 A；假设E是n循环模$\Lambda/\mathfrak{a}_k$($1 \leq k \leq n$)的直和，其中$\mathfrak{a}_k$是A的理想；*

那么，对于每个整数$p > 0$，$A$-模块$\bigwedge^p E$同构于模$A / a_H$的直和，其中对于$[1, n]$的每个$p$-元素子集$H = \{ k_1, \ldots, k_p \}$，理想的$a_H$是$\sum_{j=1}^p a_{k_j}$。

令$x_k$为$A / a_k$的规范生成元，即$A$的单位元的像，因此$E$为$Ax_i$（$1 \leq i \leq n$）的直和。然后我们知道（III，p. 515，命题10）外部代数$\bigwedge^n E$作为$A$模块与张量积$\bigotimes_{i=1}^n (\bigwedge (Ax_i))$同构的。现在$\bigwedge (Ax_i)$只是直和$A \oplus Ax_i$，因为$Ax_i$的任意两个元素的外乘积是零，所以$\bigwedge^p E$是模$M_H = (Ax_{k_1}) \otimes \ldots \otimes (Ax_{k_p})$的直和为$H = \{ k_1, \ldots, k_p \}$运行超过$p$的集合-$[1, n]$的元素子集（与$k_1 < \ldots < k_p$）；现在已知$M_H$与$A / a_{11}$同构的（II，p. 257，Cor.4），从而完成了证明。

我们现在看到，在命题1的记号中，如果理想$a_k$形式递增序列，它们完全由模$E$决定。更准确地说：

#### 命题 2 {#alg-vii-s4-prop-2 .statement tag=073O}

— *令$A$为交换环，并让$E$为$n$循环模$A / a_k$的直和，其中$a_k$满足$a_1 \subset a_2 \subset \ldots \subset a_n$。那么，对于$1 \leq p \leq n$，理想的$a_p$是$\bigwedge^p E$的湮没子；如果 $a_n \neq A$，则 $1 \leq p \leq n$ 为 $\bigwedge^p E \neq 0$，$\bigwedge^m E = 0$ 为 $m > n$。*

事实上，在命题1的记号中，我们有$a_p = a_{s(H)}$，其中$s(H)$表示子集$H$的最大元素。由于$s(H) \geq p$对于每个$p$元素子集$H$，并且由于$s(H) = p$对于$H = \{ 1, \ldots, p \}$，因此$a_p$是$a_r$的交，因为$H$的变化超过集合 $p$-$(1, n)$的元素子集；因此，根据命题 1，理想的 $a_p$ 确实是 $\bigwedge^p E$ 的湮没子。

#### 推论{#alg-vii-s4-n1-cor-1 .statement tag=073P}

— *在命题2的记号中，如果$a_n \neq A$，且$E$也同构于$m$循环模$A / a'_j$与$a'_1 \subset a'_2 \subset \ldots \subset a'_m \neq A$的直和，则$m = n$且$a_k = a'_k$ 对应 $1 \leq k \leq n$（*$a_k *$ 的唯一性）。

### 2.自由模元素的内容

令$A$为主理想整环，令$L$为自由$A$模块，令$x$为$L$的元素。由于$f$在$L$上穿过线性形式的集合$L^*$，元素$f(x)$形式是$A$的理想$c_L(x)$，称为$x$的*内容* $L$。如果生成是理想的$c_{L}(x)$，则$A$的元素$c$被称为$L$中$x$的*内容*；这相当于说，$L$上存在线性形式$f$，使得$f(x) = c$和$c$除$g(x)$对于$L$上的每个线性形式$g$。设$(e_i)_{i \in I}$为$L$中的基；把$x = \sum a_i e_i, a_i \in A$；那么理想的$c_L(x)$由和$\sum a_i b_i$组成，因为$(b_i)$贯穿集合$A'$；紧接着，$A$的元素$c$是$L$中$x$的内容当且仅当它是$x$坐标系$(a_i)$的gcd。

如果$c_L(x) = A$，我们说$x$是*不可整除的*，也就是说，如果$x$相对于$L$的基的坐标是集合互质的。

#### 引理 1 {#alg-vii-s4-lem-1 .statement tag=073Q}

*设$L$为自由模大于主理想整环$A$，并令$x$为元素除以$L$。那么下面的条件是等价的*：

(i) $x$ 不可分割；
(ii) *在$L$上存在线性形式$f$使得$f(x) = 1$；
(iii) $x$是非零的并且子模$Ax$是$L$中的直因子；
(iv) $x$是$L$中的一些基中的元素。

(i) $\Rightarrow$ (ii) ：这是从定义得出的。
(ii) $\Rightarrow$ (iii) ：令$f$在$L$上为线性形式，使得$f(x) = 1$；那么$x \neq 0$和映射$y \mapsto f(y)x$是$L$的投影算子，还有像$Ax$。
(iii)$\Rightarrow$(iv)：令$L'$为$L$中$Ax$的补集，并令$B'$为$L'$的基(*VII*，p. 15，Cor.2)；那么 $B' \cup \{x\}$ 就是 $L$ 的基。
(iv) $\Rightarrow$ (i)：微不足道。

#### 注 {#alg-vii-s4-n2-rem-1 .statement tag=073R}

— 1) 如果$x$是$L$的非零元素且$c$是$x$的含量，则存在$L$的唯一元素$y$使得$x = cy$；表示这个元素 $x/c$ ；那么$x/c$是$L$不可分割的元素。
2) 内容$c_L(x)$是挠元模中湮没子$L/Ax$。

令$L$为自由模大于主理想整环$A$，并令$M$为$L$的子模；由 *VII*, p. 4, 引理 1, 族$c_L(x), x \in M$, 拥有极大元素 ;如果$M \neq \{0\}$那么这样的极大元素就是非零的。

#### 命题 3 {#alg-vii-s4-prop-3 .statement tag=073S}

*令$L$为自由模超过主理想整环$A$，令$M$为非零的子模除$L$。令$x$为$M$的元素，使得$c_L(x)$在$M$的元素的内容中最大，令$c$为$L$中$x$的内容，并令$f$为线性形式在$L$上，这样$f(x) = c$。

a) $L$ 是$A(x/c)$ 的直和和核 $K$ $f$。
b) $M$ 是 $Ax$ 和 $K \cap M$ 中的直和。
c) $g(M) \subset Ac$ 对应 $L$ 上的每线性形式 $g$。

把$y = x/c$；显然$Ay \cap K = \{0\}$，从$f(y) = 1$开始。 此外，对于每个$u \in L$，我们有
$$
u = f(u)\,y + (u - f(u)\,y),
$$
与 $f(u)y \in Ay$ 和 $u - f(u)y \in K$ ；这证明了*a)*。 现在注，对于$u \in M$，我们有$f(u) \in Ac$：确实，让$u \in M$，并让$d$是$f(u)$和$c$的gcd；那么存在 $\lambda, \mu \in A$ 使得 $d = Xf(u) + \mu c = f(Xu + \mu x)$ ；因此元素$\lambda u + \mu x$的内容为$M$除$d$；根据$c$的最大值，这意味着$d$是$c$的关联，因此$f(u) \in Ac$。 因此对于$M$中的所有$u$，我们可以写
$$
u = (f(u)/c)\,x + (u - (f(u)/c)\,x) \in Ax + (K \cap M),
$$
显示 *b)*。 最后，让$g$在$L$上成为线性形式； by *a)* there exists a scalar $\alpha \in A$ and 线性形式 $h$ on $K$ such that $g(u) = \alpha f(u) + h(u - f(u)\,y)$ ;因此通过

b) we have $g(M) \subset Ac + h(K \cap M)$.因此，为了证明 c)，只需证明 $K$ 上的每个线性形式 $h$ 都有 $h(K \cap M) \subset Ac$，或者等效地，$L$ 上的每个线性形式 $h$ 使得 $h(x) = 0$；现在，如果$u \in K \cap M$和$d$是$h(u)$和$c$的gcd，则存在$A, \mu \in A$和$d = \lambda h(u) + \mu c$；然后$(f + h)(Au + \mu x) = d$，如上所述，这意味着$h(u) \in Ac$，c）如下。

### 3. 子模的不变因子

#### 定理 1 {#alg-vii-s4-thm-1 .statement tag=073T}

— 令$L$为主理想整环$A$之上的自由模，并令$M$为有限秩$n$的$L$子模。那么存在$L$的基$B$、$B$的$n$元素$e_i$以及$A$($1 \leq i \leq n$)的$n$非零元素$\alpha_i$这样：
a) $M$中的$\alpha_i e_i$形式基；
b) $a_i$ 除 $\alpha_{i-1}$，对于 $1 \leq i \leq n-1$。

而且由$(e_i)$生成的模$M'$和主理想$A\alpha_i$由上述条件唯一确定； 模$M'/M$是$L/M$的挠元子模，并且与$A$模块$A/A\alpha_i$的直和同构；最后$L/M$是$M'/M$的直和并且自由模同构于$L/M'$。

1) $e_i$和$\alpha_i$的存在。

如果 $M = \{0\}$ 那么定理是微不足道的。如果$M \neq \{0\}$，则根据命题3，存在$L$的元素$e_1$，$A$的非零元素$a$，以及$L$的子模$L_1$，使得$L$是$Ae_1$和$L_1$的直和，使得$M$是$A\alpha_1 e_1$的直和和$L$的子模$M_1 = M \cap L_1$，并且使得$g(M) \subset A\alpha_1$对于每个线性形式$g$于$L$。

现在我们可以在$M$的秩$n$上进行归纳。由于$L_1$是自由模（VII，p. 15，Cor.2）并且$M_1$有秩$n-1$，因此存在$L_1$，$(n-1)$的基$B_1$ $B_1$的元素$e_2, \ldots, e_n$，以及$A$的非零元素$\alpha_2, \ldots, a$，使得$(\alpha_2 e_2, \ldots, \alpha_n e_n)$是$M_1$的基，以及$\alpha_i$除$\alpha_{i+1}$ $2 \leq i \leq n-1$。如果$L'$是$L$的子模，由与$e_1, \ldots, e_n$不同的$B_1$的元素生成，则$L$是$L'$的直和和模$M'$生成$e_1, \ldots, e_n$；现在 $M'$ 的$(e_1, \ldots, e_n)$ 是基，$(\alpha_1 e_1, \ldots, \alpha_n e_n)$ $M$ 的基。现在只剩下显示$a_i$除$a_i$；但$A\alpha_2$有形式$g(M_1)$，其中$g$是$L$上的线性形式，由$g(e_2) = 1, g(e_i) = 0$为$i \neq 2$和$g(L') = (0)$定义；我们在上面已经看到了$g(M_1) \subset A\alpha_1$。

2）唯一性属性。

由于$a_i$是非零的，模$M'$是$x \in L$的集合，这样$\beta x \in M$对于$A$中的一些$\beta \neq 0$；其他字$M'/M$是$L/M$中的挠元子模。这是独一无二的确定$M'$。

显然，$M'/M$同构于$n$循环模$A/A\alpha_i$（II，p. 204，公式（26））的直和。令$r$为理想$A\alpha$的数，与$A$不同：因此第一个$n-r$理想$A\alpha_i$等于$A$，最后一个罕见的$A$不同。那么$M'/M$也同构于模$A/A\alpha_n, \ldots, A/A\alpha_{n-r+1}$的直和，其中$A\alpha_n \subset A\alpha_{n-1} \subset \ldots \subset A\alpha_{n-r+1} \neq A$。

因此Cor的条件。满足命题 2 (VII, p. 16)：理想$Aa_i$ ($1 \leq i \leq n$) 因此由模 $M'/M$ 唯一确定。

由于$L$是$M'$和$L'$的直和，因此$L/M$是$M'/M$和$(L' + M)/M$的和，并且这个和从$(L' + M) \cap M' = M$开始是直接的；另一方面，$(L' + M)/M$同构于$L'/(M \cap L')$（I，p. 41，Th.4，c）），即$L'$，这表明$(L' + M)/M$与自由模同构于$L/M'$。

#### 推论{#alg-vii-s4-n3-cor-1 .statement tag=073U}

— 自由模 $L$ 中有限秩的子模 $M$ 在主理想整环 $A$ 上有$L$ 中的补集当且仅当$L/M$ 是挠元自由时。

Th 记号。 1、如果$L/M$是挠元自由，则$M = M'$和$M'$在$L$中有补$L'$。相反，如果 $M$ 在 $L$ 中有补集 $L'$，则 $L/M$ 同构于 $L'$，后者是自由的（VII、p. 15，Cor. 2），并且更不必说挠元是自由的。

#### 注 {#alg-vii-s4-n3-rem-1 .statement tag=073V}

自由模 $L$ 中无限等级的子模 $M$ 可能会导致 $L/M$ 是挠元自由，但 $M$ 在 $L$ 中没有补集（VII，p. 60，例 6， b））。

#### 定义 1 {#alg-vii-s4-def-1 .statement tag=073W}

— 在记号和 Th 的假设中。 1、$A$的理想$A\alpha_i$称为子模$M$相对于模$L$的不变量因子。

如果$A$是有理数整数的环$\mathbf{Z}$或多项式环$K[X]$在域$K$上的一个不确定中，则有一种为$A$的每个理想选择生成元的规范方法：在$\mathbf{Z}$的情况下是正整数，或者在$K[X]$的情况下是一元多项式（VII，p. 5）。在每种情况下，不变量因子$Aa_i$的规范生成元也被滥用语言称为$M$相对于$L$的不变量因子。

### 4. 结构 / 有限生成模

#### 定理 2 {#alg-vii-s4-thm-2 .statement tag=073X}

— 主理想整环 $A$上的每个有限生成模$E$同构于循环模$A/a_k$的有限数$m$的直和，其中$a_k$是$A$的理想（其中一些可能是零），使得$a_1 \subset a_2 \subset \ldots \subset a_m \neq A$，并且由这些条件唯一确定。

如果$E$可以由$q$元素生成，则它与商模$L/M$同构的，其中$L = A^q$（II.p. 218）。 由于$M$有有限秩$n \leq q$（VII，p. 15，命题1），Th的条件。 1（VII，p. 18）满足。 Then in the notation of Th. 1 $L/M$ is isomorphic to a direct sum of a complement $L'$ of $M'$ in $L$ and the torsion module $M'/M$. 模 $L'$ 不包含有限秩 $p = q - n$，因此与 $A^p$ 同构的。 如果 $r$ 是最小的指标，使得 $A\alpha_r \neq A$，则对于 $r \leq i \leq n$，$M'/M$ 同构于模 $A/A\alpha_i$ 的直和。 如果我们取$m = p + (n - r + 1)$，$a_k = (0)$代表$1 \leq k \leq p$，$a_j = A\alpha_n , - ,$代表$1 \leq j \leq n - r + 1$，那么所规定的条件将得到满足。 唯一性源自 Cor。 VII，p. 16。

#### 推论 1 {#alg-vii-s4-thm-2-cor-1 .statement tag=073Y}

— *每个有限生成模 E 超过主理想整环都是 E 的挠元子模和自由模的直和。*

E 的挠元子模通常有几个不同的补集。对于例，如果$E = \mathbf{Z} \times (\mathbf{Z}/(2))$则E的挠元子模为$\{0\} \times (\mathbf{Z}/(2))$；它具有子模 $\mathbf{Z} \times (0)$ 的补集，以及所有元素 $(n, \overline{n})$ 的子模由……组成，其中 $n$ 贯穿 $\mathbf{Z}$，$\overline{n}$ 是剩余类类 $n$ 模 2。

#### 推论 2 {#alg-vii-s4-thm-2-cor-2 .statement tag=073Z}

— *每超过主理想整环挠元免费有限生成模都免费有限秩。*
这立即来自Cor。 1.

条件模是有限生成的，这一点至关重要。对于 A 的分数 K 域例加法群，挠元自由为 A-模；然而，如果 $A \neq K$，它就不是自由模，因为一方面 K 的任何两个元素都有公共的除子，另一方面 K 不是循环 A-模，否则 $K = ab^{-1}A$ ($a, b \in A$), 从而 $b^{-2} = acb^{-1}$ ($c \in A$)，所以$b^{-1} = ac \in A$和$K = A$。

#### 定义 2 {#alg-vii-s4-def-2 .statement tag=0740}

— *在记号和 Th 的假设中。 2、理想$a_k$称为模E的不变量因子。*
正如在定义中一样。 1（VII，p. 19），当$A = \mathbf{Z}$或$A = K[X]$时，理想$a_k$（正整数或一元多项式）的规范生成元也被滥用语言称为有限生成模E的*不变量因子*。

我们必须小心，不要将模 E 的不变量因子与自由模 L *关于* 模 L（默认I）的子模 M 的不变量混淆。

### 5. 不变量因子的计算

#### 命题 4 {#alg-vii-s4-prop-4 .statement tag=0741}

— *设 A 为主理想整环，设 L 为自由A-模，且有限基 $(u_j)$ ($1 \leq j \leq k$)，设 M 为 L 子模，设 $(x_i)$ 为生成元系统 M 并令 $A \alpha_i$ ($1 \leq i \leq n$) 为 M 关于 L 的不变量因子。那么$1 \leq m \leq n$乘积$\delta_m = \alpha_1 \ldots \alpha_m$是矩阵的第m个阶次要的最大公约数，其列是$x_i$相对于基$(u_j)$的坐标向量。

由 Th. 1 显然$M \subset \alpha_1 L$；因此M的任何元素的坐标都是$a_1$的倍数。另一方面，存在以$a_1$为L的内容的M的元素$x$。将$x$表示为$x_i$的线性组合，则$a_1$是由$x_i$的坐标生成的理想的元素。由于这些都是$a_1$的倍数，因此$a_1$确实是他们的gcd，而我们的断言是在$m = 1$的情况下证明的。

对于一般的$m$，考虑M的第m个*外部幂* $\bigwedge^m M$（III，p. 507）。 In the notation of Th. 1 there exists a basis $(a_i)$ for M where $a_i = \alpha_i e_i$ ($1 \leq i \leq n$); thus $\bigwedge^m M$ has a basis consisting of the elements $a_{i_1} \wedge \ldots \wedge a_{i_m}$, as $(i_1, \ldots, i_m)$ runs through the set of strictly increasing sequences of $m$ elements of $(1, n)$. 现在元素$e_{i_1} \wedge \ldots \wedge e_{i_m}$属于到基$B_m$$\bigwedge^m L$。 因此，从$\bigwedge^m M$到$\bigwedge^m L$的规范映射是同构从$\bigwedge^m M$到$\bigwedge^m L$的子模，具有基元素$(\alpha_{i_1} \ldots \alpha_{i_m})\, e_{i_1} \wedge \ldots \wedge e_{i_m}$，并且我们认同这个子模与$\bigwedge^m M$。 由于$\alpha_j$对于$j \geq k$来说是$\alpha_k$的倍数，所以元素$\alpha_{i_1} \ldots \alpha_{i_m}$都是$\delta_m = \alpha_1 \ldots \alpha_m$的倍数，其中之一等于$\delta_m$；因此，$\delta_m$是相对于$\bigwedge^m M$的生成元、元素、系统的$B_m$的坐标的gcd。 参数的第一个部分表明，$\delta_m$是$\bigwedge^m M$的生成元的任何系统坐标相对于$\bigwedge^m L$的任何基的坐标集合的gcd。 取$L$的基$(u_j)$推导出基为$\bigwedge^m L$，以及$(x_i)$的外部乘积的$\bigwedge^m M$由……组成为生成元的系统，可得这些坐标的表达式行列式（III、p. 528、命题 9）中的项中的乘积给出了规定的结果。

### 6. 自由模中的线性映射，以及矩阵超过主理想整环

设$A$为主理想整环。考虑将线性映射$f$从秩$m$的免费$A$模块$L$转换为秩$n$的免费$A$模块$L'$。前面的结果允许我们通过为$L$和$L'$选择合适的基，将$f$的矩阵放入一个特别简单的形式中，称为矩阵的*规范形式*。

#### 命题 5 {#alg-vii-s4-prop-5 .statement tag=0742}

*令$A$为主理想整环，并且$f$将秩$r$的线性映射从秩$m$的自由$A$模块$L$转换为$A$模块$L'$ 秩 $n$。那么存在$L$的基$(e_i)$($1 \leq i \leq m$)和$L'$的$(e'_j)$($1 \leq j \leq n$)，使得$1 \leq i \leq r$有$f(e_i) = \alpha_i e'_i$，$i > r$有$f(e_i) = 0$，其中$\alpha_i$ 是$A$ 中的非零元素，每个除下一个；理想$A \alpha_i$是$f(L)$在$L'$中的不变量因子，因此是唯一确定的。*

设$L_0 = f^{-1}(0)$为$f$的核；商$L/L_0$同构于模$f(L)$，即$L'$的子模，因此自由（*VII*，p. 15，Cor.2）；因此$L_0$在$L$中有一个补集$L_1$（*II*，p. 218，命题21），并且$f$到$L_1$的限制是从$L_1$到同构 $f(L) = M'$。如果理想 $A \alpha_i$ ($1 \leq i \leq r$) 是 $M'$ 在 $L'$ 中的不变量因子，则 Th。 *VII*、p. 18的1表示存在$L'$的基$(e'_j)$($1 \leq j \leq n$)使得$(\alpha_i e'_i)$($1 \leq i \leq r$)是$M'$的基。由于$f$到$L_1$的限制是从$L_1$到$M'$的同构，因此存在$L_1$的基$(e_i)$($1 \leq i \leq r$)使得$f(e_i) = \alpha_i e'_i$。 $L$的基扩展到基$(e_s)$($1 \leq k \leq m$)通过取$(e_s)$($r+1 \leq s \leq m$)为核$L_0$的基。

#### 推论 1 {#alg-vii-s4-prop-5-cor-1 .statement tag=0743}

— 设 X 为秩 r 的矩阵，有 n 行和 m 列，超过主理想整环 A；则存在矩阵 $X_0$ 相当于形式的 X (II, p. 354)

$$
\begin{pmatrix}
\alpha_1 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & \alpha_2 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & \alpha_r & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0 \\
0 & 0 & \ldots & 0 & 0 & \ldots & 0
\end{pmatrix}
$$

其中$\alpha_i$是A的非零元素，每个除都是下一个。在这些条件下，$\alpha_i$由可逆元唯一确定到乘法。

假设两个矩阵、X和$X'$是等价的，如果在A上存在阶n和m的可逆方阵P和Q，使得$X' = PXQ$，Cor。 1只是用项或矩阵表达的命题5。

在第 5 号提案和 Cor 的记号中。 1、(非零的)理想$Au$，称为线性映射 f 或矩阵 X 的不变量因子。然后紧接着Cor. I：

#### 推论 2 {#alg-vii-s4-prop-5-cor-2 .statement tag=0744}

— 两个矩阵 X 和 $X'$ 具有 n 行且 m 列在主理想整环 A 上，当且仅当它们具有相同的不变量因子时，它们是等价的。

注当A为域时，可取$\alpha_i$等于1，则恢复II、p. 360的第13条命题。

如果相对于L的任意基和L'的任意基，X是线性映射 f的矩阵，则X的列是坐标向量，相对于L'的基，L'的元素，其中生成元的形式系统对于$f(L)$。因此，以下结果是命题 4 的直接的推论。

#### 命题 6 {#alg-vii-s4-prop-6 .statement tag=0745}

— 令X为秩r在主理想整环A上的矩阵，并令$A \alpha_i$($1 \leq i \leq r$)为其不变式因子的序列。那么$\alpha_1$就是X的元素的gcd； 乘积$\alpha_1 \ldots \alpha_q$是$q \leq r$的X的第q个阶未成年人的gcd。

### 7. 有限生成阿贝尔的群

在$A = \mathbf{Z}$情况下，可以表示截面 4的结果

#### 定理 3 {#alg-vii-s4-thm-3 .statement tag=0746}

— 每个有限生成的阿贝尔的群 G 是其挠元子群 F 的直和（G 中有限阶元素子群）和一个自由的阿贝尔的有限秩 p 的群（与$\mathbf{Z}^p$同构的）。 群 F 是阶 $n_1, n_2, \ldots, n_q$ 的循环群的有限数的直和，其中$n_i$ 是整数 $> 1$，其中每个除是前一个除一；而且，整数$p, q$和$n_i$($1 \leq i \leq q$)由$G$唯一确定。

#### 注 {#alg-vii-s4-n7-rem-1 .statement tag=0747}

而F为直和的循环群的阶$n_1, \ldots, n_q$则由Th的整除性条件很好地定义。 3，对于群本身来说*不*相同：对于例，在$\mathbf{Z}/(p)$的乘积G与其自身（对于p素数），子群恰好是$\mathbf{F}_p$向量子空间，并且G是两个一维的直和子空间以 $p(p+1)$ 不同的方式。

#### 推论 1 {#alg-vii-s4-thm-3-cor-1 .statement tag=0748}

— *在有限的阿贝尔的群G中，存在元素，其阶是G的元素所有阶的lcm；这个阶 n 是 G 的第一个不变量因子。*

#### 推论 2 {#alg-vii-s4-thm-3-cor-2 .statement tag=0749}

— *任何有限阿贝尔的群 G，其阶不能被任何整数 $> 1$ 的平方整除，是循环的。*
让我们保持Th的记号。 3. 然后$p = 0$，因为G是有限的，$q \leq 1$，否则G的阶可以被$n_q^2$整除。因此G是循环的。

#### 推论 3 {#alg-vii-s4-thm-3-cor-3 .statement tag=074A}

— *令L和M为秩n的两个自由$\mathbf{Z}$模，令$(e_i)$为L的基和$(f_i)$基为M（$1 \leq i \leq n$），令u为同态将L代入M，并令U为其相对于基$(e_i)$和$(f_i)$的矩阵。那么$\mathrm{Coker}\,u = M/u(L)$是有限的当且仅当$\det(U) \neq 0$，然后$\mathrm{Card}(\mathrm{Coker}(u)) = |\det(U)|$。
如果需要的话，通过改变L和M中的基，我们可以假设U具有VII，p. 22，Cor中描述的形式。 1 到提案 5（其中 $a_i$ 在本例中为整数）；那么推论就变得明显了，因为如果 $a_i$ 之一是零，则$\mathbf{Z}$-模块 $\mathbf{Z}/\alpha_i \mathbf{Z}$ ($1 \leq i \leq n$) 的直和的阶是无限的，否则等于 $|\alpha_1 \alpha_2 \ldots a_n|$。

### 8.不可分解模。小学除子

#### 定义 3 {#alg-vii-s4-def-3 .statement tag=074B}

— *左模 M 超过环如果 A 是真非零的子模族的直和，则称 A 是可分解的。否则它就被认为是不可分解的。*
因此，零模是*可分解的*，是子模空族的直和。
设$\mathfrak{a}$为环A的左理想； $A/\mathfrak{a}$的子模只是商$b/\mathfrak{a}$，其中$b$是包含$\mathfrak{a}$的理想（I，p. 41，Th.4）；如果$b$和$c$是包含$\mathfrak{a}$的两个理想，那么模$A/\mathfrak{a}$是子模$b/\mathfrak{a}$和$c/\mathfrak{a}$的直和当且仅当$A = b + c$ 和 $b \cap c = \mathfrak{a}$。结果：

#### 引理 2 {#alg-vii-s4-lem-2 .statement tag=074C}

— *模 $A/\mathfrak{a}$ 不可分解当且仅当 $\mathfrak{a} \neq A$ 并且不存在与 A 和 $\mathfrak{a}$ 不同的 A 的理想对 $(b, c)$，使得 $A = b + c$ 和 $b \cap c = \mathfrak{a}$。*

#### 命题 7 {#alg-vii-s4-prop-7 .statement tag=074D}

— 令$A$为交换环，令$\mathfrak{p}$为$A$的素理想（I，p. 117，Def.3），并令$q$为$\mathfrak{p}$中包含的$A$的理想。假设对于每个$x \in \mathfrak{p}$，都存在整数$n > 0$，使得$x^n \in q$。那么$A$-模块$A/q$是不可分解的。

令$b$和$c$为$A$的两个理想，使得$A = b + c$和$b \cap c = q$。然后$bc \subset b \cap c = q \subset \mathfrak{p}$；如果$x \notin \mathfrak{p}$和$x \in c$，则$xb \subset p$，所以$b \subset \mathfrak{p}$（I，p. 316，命题4）；因此 $b \subset \mathfrak{p}$ 或 $c \subset p$。假设例为$c \subset \mathfrak{p}$，则$b + p = A$；那么存在$x \in b$和$y \in \mathfrak{p}$使得$1 = x + y$；令 $n \in \mathbf{N}$ 使得 $y^n \in q$；然后$1 = (x + y)^n$。所以$1 \in xA + y^nA \subset b + q \subset b$，所以$b = A$。 引理 2 现在表明 $A/q$ 是不可分解的。

现在假设$A$是主理想整环；根据VII、p. 2、命题2，$A$的素理想是理想$(p)$，其中$p$是$A$的不可约元，以及理想$0$；由前面的命题、模、$A$和$A/(p^n)$，对于$p$不可约和$n > 0$，是不可分解的。由于每个循环模都是这个型的模的直和（VII，p. 3，命题4），并且因为每个有限生成的$A$模都是循环模的直和 （VII，p. 19，Th.2），我们推导出：

#### 命题 8 {#alg-vii-s4-prop-8 .statement tag=074E}

— 令$A$为主理想整环，并令$M$为有限生成的$A$模块。

a) $M$ 不可分解当且仅当它同构于 $A$ 或形式 $A/(p^n)$ 的模，其中$p$ 是$A$ 的不可约元，$n > 0$ 是整数。

b) $M$ 是不可分解的子模有限族中的直和。

上述命题的部分b)可以更精确，如下：

#### 命题 9 {#alg-vii-s4-prop-9 .statement tag=074F}

— 令$A$为主理想整环，令$P$为$A$的不可约元代表的系统，并令$M$为有限生成的$A$模块。那么存在正整数 $m(0)$ 和 $m(p^n)$ ($p \in P, n > 0$)，除了它们的数量有限之外，由 $M$ 和零唯一确定，使得 $M$ 同构于 $A^{m(0)}$ 的直和，并且$(A/(p^n))^{m(p^n)}$（$p \in P, n > 0$）。

整数 $m(0)$ 和 $m(p^n)$ ($p \in P, n > 0$) 的存在性由命题 8 得出。 整数 $m(0)$ 是唯一确定的：它是自由模的秩，即 $M$ 除以挠元的商子模。最后，$M$的$p$主成分与$(A/(p^n))^{m(p^n)}$的直和同构；由于理想族 $(p^n)$ ($n \geq 1$) 是完全按包含排序的，$m(p^n)$ 的唯一性由 Cor 得出。 VII、p. 16 的第 2 条建议。

#### 定义 4 {#alg-vii-s4-def-4 .statement tag=074G}

— 在第 9 条的记号中，那些理想$(p^n)$ ($p \in P, n \geq 1$ 整数)使得$m(p^n) > 0$被称为模$M$的初等除子，整数$m(p^n)$被称为它们的重数；如果整数$m(0)$是$> 0$，则称为初等除子0的重数。

至于不变量因子（VII，p. 19，Def.1），当$A = \mathbf{Z}$或$A = K[X]$（K交换域）时，则理想$(p^n)$（正整数或一元多项式）的规范生成元也被称为滥用语言， 有限生成模 $M$ 的基本除子。

#### 注 1 {#alg-vii-s4-n8-rem-1 .statement tag=074H}

如果$M$是有限的阿贝尔的群，那么它的结构可以通过写下它的基本除子来描述，每个重数重复一次。 We will say, for example, that $M$ is « of type $(2, 2, 4, 27, 27, 25)$ » (or that it is « a group $(2, 2, 4, 27, 27, 25)$ ») if it is isomorphic to the product of two groups $\mathbf{Z}/(2)$, one group $\mathbf{Z}/(2^2)$, two groups $\mathbf{Z}/(3^3)$ and one group $\mathbf{Z}/(5^2)$.

#### 注 2 {#alg-vii-s4-n8-rem-2 .statement tag=074I}

如果在主理想整环 $A$ 上有限生成的挠元模 $M$ 被给定为与 $A/(a_i)$ 同构的循环模的直和（特别是如果 $M$ 的不变量因子已知），则$M$的初等除子及其多重性，可以通过注意到$A/(a)$同构于$A/(p^{n(p)})$的乘积来确定，其中$a = e \prod_{p \in P} p^{n(p)}$是$a$的分解不可约因子 （$VII$，p. 3）。让我们研究例乘法群 $G(464\ 600)$，其中 $G(n)$ 表示乘法群 $(\mathbf{Z}/n\mathbf{Z})^*$（$VII$，p. 12）。从$464\ 600 = 2^3 \cdot 5 \cdot 23 \cdot 101$开始，这个群同构于群$G(2^3)$、$G(5^2)$、$G(23)$和$G(101)$的乘积（$VII$、p. 13、Th.3）；现在最后三个群是阶20、22和100的循环，$G(2^3)$是阶2的两个循环群的乘积(\emph{loc.cit.})；由于$20 = 2^2 \cdot 5$、$22 = 2 \cdot 11$和$100 = 2' \cdot 5^2$，群$G(464\ 600)$等于型$(2, 2, 2, 2^2, 2^2, 2^2, 5, 5^2, 11)$。

#### 注 3 {#alg-vii-s4-n8-rem-3 .statement tag=074J}

对于挠元模的计算不变量因子，其初等除子已知，我们再次依赖于以下事实：如果 $a_i$ 是 $A$ 的成对互质元素，则乘积 $\prod A/(a_i)$是循环模同构于 $A/(a_1 a_2 ... a_n)$ ($VII$, p. 3, 命题 4)。让我们通过观察群$G(464\ 600) = M$的例来说明方法：将$M$的初等除子$p^n$（它们是相同不可约$p$的幂）写在同一行上，从最大的开始指数；通过在必要时放入 1，将扩展这些行转换为等于长度的行：

$$
\begin{array}{cccccc}
2^2 & 2^2 & 2 & 2 & 2 \\
5^2 & 5 & 1 & 1 & 1 \\
11 & 1 & 1 & 1 & 1 .
\end{array}
$$

那么不变式因子是元素的乘积在同一个列：$1100, 20, 2, 2, 2$。事实上，根据$VII$、p. 3的命题4，$M$同构于阶1100、20、2、2、2的循环群的乘积；由于每个阶都是下一个倍数，因此这些是$M$的不变因子（$VII$，p. 22，Th.3）。

#### 注 4 {#alg-vii-s4-n8-rem-4 .statement tag=074K}

An $A$-module is called simple ($I$, p. 37) if it is nonzero and has no submodules other than itself and $0$; it is then necessarily cyclic, so finitely generated, and indecomposable; since the modules $A/(p^n)$ are not simple for $n \neq 1$, while the modules $A/(p)$ are, and since $A$ is simple only if the ring $A$ is a field, we deduce that the simple $A$-modules are:
a) free modules of rank 1, when $A$ is a field;
b) modules isomorphic to quotients $A/(p)$, where $p$ is an irreducible element of $A$, when $A$ is not a field.

### 9. 模有限长度主理想整环的对偶性

其中，截面$A$表示主理想整环，它不是域（因此至少有一个不可约元），并且$K$域是$A$的分数。对于每个$A$-模块$M$，放入

$$
D(M) = \operatorname{Hom}_A(M, K/A);
$$

我们知道$D(M)$以自然的方式配备了结构或A-模，即对于每个同态$u : M \to K/A$和每个$\alpha \in A$，同态$\alpha u$映射$x$到$\alpha u(x) = u(\alpha x)$。 A-模的每个同态 $f : M \to N$ 都与同态 $D(f) : D(N) \to D(M)$ 相关联，其中 $D(f)(v) = v \circ f$ (II, p. 196)。对于$x \in M$和$x' \in D(M)$，我们输入$\langle x, x' \rangle = x'(x) \in K/A$；那么$(x, x') \mapsto \langle x, x' \rangle$是从$M \times D(M)$到$K/A$的*A双线性*映射，称为*规范*。

如果 M 和 $N$ 是两个 A-模，则每个 A 双线性映射 $\varphi : M \times N \to K/A$ 都与 A-线性映射 $d_\varphi : N \to D(M)$ 和 $s_\varphi : M \to D(N)$ 相关联，其中 $d_\varphi(y)(x) = \varphi(x, y) = s_\varphi(x)(y)$（II、p. 268，对应命题 *1*）。特别是规范的 A-双线性映射 $M \times D(M) \to K/A$ 定义一个 A-线性映射（也称为*规范*）

$$
c_M : M \to D(D(M))
$$

这样对于$x \in M$和$x' \in D(M)$来说$\langle x', c_M(x) \rangle = \langle x, x' \rangle$。

#### 命题 10 {#alg-vii-s4-prop-10 .statement tag=074L}

— 如果 *M 是有限长度的 A-模，则 $D(M)$ 是*（通常非自然地）*与 M 同构的，并且规范的映射 $c_M : M \to D(D(M))$ 是同构。*
使用 VII，第 17 页*19*，周四。 2 和 **II**，p. 203，Cor。 1，我们约化到$M$是循环的情况。因此我们可以假设$M = A/tA$和$t \neq 0$。 注任何同态$u : A/tA \to K/A$完全由像$\xi \in K/A$在*1*模$tA$的类$\varepsilon$$u$下确定，而这个元素必须满足关系$t\xi = 0$;相反，对于任何$\xi \in K/A$使得$t\xi = 0$，存在同态$u : A/tA \to K/A$使得$u(\varepsilon) = \xi$。由此可见，$D(M)$与$t^{-1}A/A$同构的，并且由于$t$乘位似在K上是双射，因此我们也有$D(M)$与$A/tA$同构的，这证明了第一个断言。这就证明了 $M$ 和 $D(D(M))$ 同构的，所以有相同的长度 ；另一方面，$c_M$是单射的，因为如果$y \in A$使得关系$tz \in A$（对于$z \in K$）意味着$yz \in A$，那么取$z = t^{-1}$我们有$y \in tA$。由此可见像$c_M(M)$必然等于$D(D(M))$。

#### 推论{#alg-vii-s4-n9-cor-1 .statement tag=074M}

— *令 M、N 为有限长度中的两个 A-模，并令 $\varphi$ 为从 $M \times N$ 到 $K/A$ 的 A 双线性映射，使得： 1) 关系 $\varphi(x, y) = 0$ 对于所有 $y \in N$ 意味着$x = 0$; 2) 关系 $\varphi(x, y) = 0$ 对于所有 $x \in M$ 意味着 $y = 0$。那么与 $\varphi$ 伴随的 A 线性映射 $s_\varphi : M \to D(N)$ 和 $d_\varphi : N \to D(M)$ 是同构。*
事实上，关于 $\varphi$ 的假设意味着 $s_\varphi$ 和 $d_\varphi$ 是*内射*，并且由于 $\mathrm{long}(D(N)) = \mathrm{long}(N)$ 和 $\mathrm{long}(D(M)) = \mathrm{long}(M)$ 根据命题 *10*，这意味着 $\mathrm{long}(M) = \mathrm{long}(N)$，因而 $s_\varphi$ 和 $d_\varphi$ 是双射的。

#### 命题 11 {#alg-vii-s4-prop-11 .statement tag=074N}

— *如果 $M' \xrightarrow{u} M \xrightarrow{v} M''$ 是有限长度 A-模正合序列，则序列 $D(M'') \xrightarrow{D(v)} D(M) \xrightarrow{D(u)} D(M')$ 是精确的* [^1]。

让我们首先展示给定的正合序列

(1)
$$
0 \to M' \to M \to M'' \to 0
$$

相应的序列

$$
0 \to D(M'') \to D(M) \to D(M') \to 0
$$

是准确的；事实上我们知道序列

$$
0 \to D(M'') \to D(M) \to D(M')
$$

是精确的（II，p. 227，Th.1）；另一方面，由 (1) 得出

$$
\operatorname{long}(M) = \operatorname{long}(M') + \operatorname{long}(M'')
$$

（II、p. 212、提案 16）；根据命题 10，我们有

$$
\operatorname{long}(D(M)) = \operatorname{long}(D(M')) + \operatorname{long}(D(M''))
$$

其他字$\operatorname{long}(D(M')) = \operatorname{long}(D(M)/D(M''))$。由于$D(M)/D(M'')$自然地等同于$D(M')$的子模，所以它一定等于$D(M')$，这就证明了我们的断言。

这立即意味着如果 $u : M' \to M$ 是单射的，那么 $D(u) : D(M) \to D(M')$ 是满射的；由II、p. 199、注4得出结论。

对于每个 A-模 M，让 $\mathfrak{S}(M)$ 表示 M 的子模的集合。对于 M 的每个子模 N（分别为 D(M) 的每个子模 N'），让 $N^0$（分别为 ${N'}^0$）表示 M 的子模那些$x' \in D(M)$（或$x \in M$）中的$D(M)$（或M）由……组成，使得$(y, x') = 0$适用于所有$y \in N$（或$(x, y') = 0$适用于所有$y' \in N'$）。

#### 命题 12 {#alg-vii-s4-prop-12 .statement tag=074O}

*设 M 为 A-模 / 有限长度。那么映射将M的每子模N发送到$N^0$是从$\mathfrak{S}(M)$到$\mathfrak{S}(D(M))$的双射，逆双射将D(M)的每子模N'发送到M的子模${N'}^0$； 模 $D(N)$ 自然地与 $D(M)/N^0$ 等同，$D(M/N)$ 与 $N^0$ 等同。此外，我们还有*

(2)
$$
(N_1 + N_2)^0 = N_1^0 \cap N_2^0, \quad (N_1 \cap N_2)^0 = N_1^0 + N_2^0
$$

对于 M 的所有子模 $N_1, N_2$。

对于 M 中的每个子模 N，有正合序列

$$
0 \to N \to M \to M/N \to 0
$$

因此（命题 11）正合序列

$$
0 \to D(M/N) \to D(M) \to D(N) \to 0
$$

由于$D(M)$中$D(M/N)$的像显然是$N^0$，我们看到（命题10）$\operatorname{long}(N^0) = \operatorname{long}(M) - \operatorname{long}(N)$；因为根据第 10 条，$M$ 与$D(D(M))$ 相同，我们也有类似的

$$
\operatorname{long}(N^{00}) = \operatorname{long}(M) - \operatorname{long}(N^0) = \operatorname{long}(N);
$$

在加法中，很明显$N \subset N^{00}$，所以$N^{00} = N$。此外，(2)中的第一个关系是明显的，通过应用到子模$N_1^0$和$D(M)$的$N_2^0$，我们有$(N_1^0 + N_2^0)^0 = N_1 \cap N_2$，所以$N_1^0 + N_2^0 = (N_1^0 + N_2^0)^{00} = (N_1 \cap N_2)^0$。这样就完成了命题的证明。

#### 例 1 {#alg-vii-s4-n9-exa-1 .statement tag=074P}

对于$A = \mathbf{Z}$，有限长度的$\mathbf{Z}$模恰好是有限的阿贝尔的群；然后$K = \mathbf{Q}$，所以$K/A = \mathbf{Q}/\mathbf{Z}$。然后对于定义$D(M)$，我们有时采用与其同构的$\mathbf{Z}$模块来代替$\mathbf{Q}/\mathbf{Z}$，例如（V，p. 79，命题2）群$R$特征 0 的代数闭域中的单位元（乘法以下）的根；然后我们输入$D(M) = \operatorname{Hom}_{\mathbf{Z}}(M, R)$。我们让读者在相应的记号中重写这种特殊情况的前述结果。

#### 例 2 {#alg-vii-s4-n9-exa-2 .statement tag=074Q}

设$a$为$A$的非零元素。 映射$x \mapsto x/a$从$A$进入$K$诱导同构在商模从$A/(a)$到子模$(K/A)(a)$$K/A$由……组成元素被$a$消灭。如果 $M$ 是被 $a$ 消灭的 $A$ 模块，或者等效地是 $A/(a)$ 模块，则 $A$ 模块 $D(M)$ 被标识为 $\operatorname{Hom}_{A/(a)}(M, A/(a))$。我们让读者将这种特殊情况的前面结果重写为相应的记号（cf.V，p. 86）。

### 习题 {#alg-vii-s4-exercises}

§ 4](exercises/s4/)参见[习题。

[^1]: 稍后我们会看到 (A, X, p. 18) A-模 K/A 是单射的。由此可见，第 11 条命题对于任意 A-模 M、M' 和 M" 仍然有效。
