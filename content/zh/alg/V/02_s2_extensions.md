---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 2
section_title: Extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.9-A V.15, A V.146-A V.147
pdf_pages: 0123-0129, 0260-0261
extraction: ocr
subsections:
    - "no": 1
      title: The structure of an extension
      page: 9
      pdf_page: 123
    - "no": 2
      title: Degree of an extension
      page: 10
      pdf_page: 124
    - "no": 3
      title: Adjunction
      page: 10
      pdf_page: 124
    - "no": 4
      title: Composite extensions
      page: 12
      pdf_page: 126
    - "no": 5
      title: Linearly disjoint extensions
      page: 13
      pdf_page: 127
statements: 19
exercises: 4
content_sha256: fdbe9749aee4a228cd45c44a5429b420921467ffddcf0a15a9691a3d4336e183
translated_from: content/en/alg/V/02_s2_extensions.md
translation_method: google
source_content_sha256: 101cc4d1109f50a0e0cf391686f5376a9cdac7d1f76b8f5bb4664a68d107975c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4b44960bba394b624c6ee9680d912dc77861b1f8afe6646ca51abd0afffa8478
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。 扩张

### 1. 结构 / 扩张

#### 定义 1 {#alg-v-s2-def-1 .statement tag=06GV}

— 令 K 为域。通过 K 的扩张，我们了解K-代数，其基础环为域。通过扩张 E 的子扩展（或子 K 扩展），我们理解 E 的子 K 代数为域。
令 E 为 K 的扩张。 映射 u : A ↦ λ 。 K 转入 E 的 1 为环同态；由 K 的 I、p. 115、u 诱导同构到 E 的子域 u(K)。
相反，如果 K、E 是域并且 u 是 K 的同态到 E 中，则 u 定义在 K 的扩张的 E 结构 (III，p. 433) 上。通过滥用语言，一个有时说（E，u）是K的扩张。
如果 u(K) = E，即，如果 E 是维数 1 除以 K 的向量空间，则称扩张是平凡的。
令L为K的扩张域。当我们将L视为K的扩张时，我们通过K的扩张（L，j）来理解，其中j是K的典范嵌入到L，或者也为L 相应的K-代数结构。那么L的子外延就是K和L之间的中间域，即L包含K的子域。如果L'是K的另一个扩张域，则L 到 L' 的 K 同态就是 L 的同态 f 到 L'，这样对于所有 x ∈ K，f(x) = x。我们注如果 f 是域的任意自同态 L，则L不变量的元素在f下的集合是L的子域K'，则f是L的K'-自同态。
特别地，令 P 为域 L 的素数子域。我们可以将L视为P的扩张，并且L的每个自同态都是一个P-自同态。
令 (E, u) 为 K 的扩张；由于 K 的 u 定义同构到 E 的子域 K_1，一般来说，通过 u 来识别 K 和 K_1 没有困难。我们不能允许这样的识别的一种情况是，其中K = E并且u因此是K的自同态；最常见的是，当域 K 的特征 ≠ 0 时，u 是 K 的自同构，或映射 u ↦ u''。
显然，K 的每个扩张都同构于扩张 (L, j)，其中 L 是域包含 K 作为子域，j 是 K 的典范嵌入到 L。

### 2. 次数 / 扩张

令 $A$ 为代数超过域 $K$。特别是向量空间超过$K$；这个向量空间的维数在$K$上称为$A$的次数，写成$[A : K]$(II、p. 293)。因此，定义$[A : K]$是$A$超过$K$的任何基的基数。该定义特别适用于扩张或$K$的情况。

次数 1 的扩张是微不足道的。 次数 2（或 3 等）的扩张称为二次（或三次等）。 An extension of finite degree is sometimes called, by abuse of language, a finite extension.

#### 定理 1 {#alg-v-s2-thm-1 .statement tag=06GW}

*令$E$为$K$和$A$代数的扩张超过$E$。那么我们就有$[A : K] = [A : E] \cdot [E : K]$。特别是，如果 $F$ 是 $E$ 的扩张，我们有*

$$
[F : K] = [F : E] \cdot [E : K].
$$

定理只是II、p. 222、25号提案的特例；更准确地说，如果$A$的$(a_i)$、、、、基超过$E$，并且$E$的$(b_j)$、$\in M$基超过$K$，那么家庭$(a_\lambda b_\mu)_{(\lambda,\mu) \in L \times J}$就是基 $A$超过$K$。

#### 推论 1 {#alg-v-s2-thm-1-cor-1 .statement tag=06GX}

*令$K, E, F$为三个域，使得$K \subset E \subset F$和$[F : K]$是有限的。那么次数$[E : K]$和$[F : E]$就是$[F : K]$的除子。

如果次数 $[F : K]$ 是素数，则除了 $K$ 和 $F$ 之外，$F$ 没有子扩张。但注，当$[F : K]$不是素数时，除了$K$和$F$之外，不一定存在$F$的子扩张（cf.V、p. 146、习题1）。*

#### 推论 2 {#alg-v-s2-thm-1-cor-2 .statement tag=06GY}

*令$K, E$和$F$为三个域，使得$K \subset E \subset F$。假设$[F : K]$是有限的，则关系$[E : K] = [F : K]$等价于$E = F$，关系$[F : E] = [F : K]$等价于$E = K$。

因为如果 $L$ 是 $L'$ 的扩张域，则 $[L : L'] = 1$ 相当于 $L' = L$。*

#### 命题 1 {#alg-v-s2-prop-1 .statement tag=06GZ}

*设$A$为有限次数中的代数超过域$K$。如果元素$a \in A$不是$A$中零的左（或右）除子，则它在$A$中是可逆的。

对于 $K$ 上的向量空间 $A$ 来说，有限维的假设和线性映射 $x \mapsto ax$（分别为 $x \mapsto xa$）将 $A$ 变为 $A$ 单射的；因此它是双射 (II, p. 298, Cor.) 并且因此 (I, p. 16, 注) $a$ 在 $A$ 中是可逆的。*

#### 推论{#alg-v-s2-n2-cor-1 .statement tag=06H0}

*令$A$为有限次数中的交换代数超过域$K$。如果$A$是整环，那么它就是域。*

### 3.伴随

令$E$为域$K$中的扩张。给定$E$的元素的族$x = (x_i)_{i \in I}$，我们用$K(x_i)_{i \in I}$（或$K(x)$或$K(x_1, \ldots, x_r)$，当$I$是N的区间（1，n）时）表示E包含的最小子扩张$(x_i)_i$；我们说$K(x_i)_i \in I$是由$(x_i)_i, I$族的元素的伴随到K获得的，并且$(x_i)_i, I$族（或其元素的集合）是关于K（或超过K）的$K(x_i)_i \in I$族生成的族。 域$K(x_i)_i \in I$仅取决于家庭$(x_i)_i \in I$的元素的集合A；我们也用$K(A)$来表示它。特别是我们有 $K(E) = E$ 和 $K(\emptyset) = K . 1$。所有上述内容尤其适用于 E 为域包含 K 为子域时。

应该注意的是，A一般不是代数$K(A)$的生成的集合，其他字$K(A) \neq K[A]$。 “尽管如此，当$K(A)$是K的代数扩张时，我们将看到$K(A) = K[A]$（V，p. 18，Cor.1）。 \*

#### 命题 2 {#alg-v-s2-prop-2 .statement tag=06H1}

— *如果 M 和 N 是域 K 的扩张中的任意两个子集，则* $K(M \cup N) = K(M)(N) = K(N)(M)$。

对于 $K(M \cup N)$ 包含 $K(M)$ 和 N，因此$K(M)(N)$；因为$K(M)(N)$是域包含$K \cup M \cup N$，所以包含$K(M \cup N)$，从而命题。

我们将有时写成$K(M, N)$而不是$K(M \cup N)$。

#### 注 {#alg-v-s2-n3-rem-1 .statement tag=06H2}

— 令 P 为域 E 的素数子域 (V, p. 2)；对于 E 的每个子集 A，$P(A)$ 是 E 包含 A 的最小子域。特别是，如果 K 是 E 的子域，则我们有 $P(K \cup A) = K(A)$。如果 K 和 K' 是 E 的两个子域，则我们有 $P(K \cup K') = K(K') = K'(K)$；该域是E 包含 K或K'中最小的子域，或者也是E的子域的集合中K和K'的上界，按包含排序；我们有时说这个域是由E中的K和K'生成的域。

#### 命题 3 {#alg-v-s2-prop-3 .statement tag=06H3}

— *令$\mathscr{F}$为域E的子域集合，相对于关系$\subset$。 $\mathscr{F}$域并L为域。*

因为如果x和y是L的两个元素，则存在$\mathscr{F}$的两个域R，S使得$x \in R,\ y \in S$；令T为$\mathscr{F}$包含R和S的域；然后$x \in T,\ y \in T$，因此$x + y,\ xy$和$x^{-1}$（如果$x \neq 0$）属于到T，因此到L。

#### 推论{#alg-v-s2-n3-cor-1 .statement tag=06H4}

— *令 E 为域 K 和 $A \subset E$ 中的扩张。 域$K(A)$是域$K(F)$的并，其中F的范围超过A的所有有限子集的集合。*

对于域$K(F)$的集合来说，关系$\subset$有向，因为$F \subset F'$蕴含$K(F) \subset K(F')$。因此，这些域中的并L是域包含$K \cup A$并包含在$K(A)$中，因此与$K(A)$相同。

#### 定义 2 {#alg-v-s2-def-2 .statement tag=06H5}

— *如果有限生成族有有限生成族，则域K的*扩张E被认为是有限生成的。如果 E 中存在 x 且满足 * $E = K(x)$，则称其为单生的。

科。命题 3 表明，域 K 的每个扩张 E 都是 E 中包含的有限生成的扩张的有向并。很明显，有限次数 K 的每个扩张 E 也是有限生成的，因为 E 的基（视为 K 上的向量空间）也是有限生成的。 生成的 E 超过 K 的家族；稍后我们会看到逆命题不成立。

### 4.复合扩张

设E和F是域K的两个扩张。通过$E$和F的复合扩张，我们可以理解任何三元组$(L, u, v)$，其中L是K的扩张，$u$是E到L的K同态， $v$是F到L的K同态，其中域L由$u(E) \cup v(F)$生成（cf.图1）。

![图表显示扩张 E、F、K、L、同态 u、v、r](../images/fig_1.png)

图 1.

与 E 和 F 的复合扩张 $(L, u, v)$ 到 E 和 F 的复合扩张 $(L', u', v')$ 的一般定义 (E, IV, p. 6) 同构一致，是 L 的 K-同构 $\varphi$ 到$L'$使得$u' = \varphi \circ u$和$v' = \varphi \circ v$。

令$(L, u, v)$为E和F的复合扩张。$E \otimes_K F$的K-线性映射$w$进入L，将$x \otimes y$发送到$u(x)v(y)$为K-代数同态；在这个编号中我们用$u * v$来表示。它的像是$u(E) \cup v(F)$生成的L的子环。

#### 命题 4 {#alg-v-s2-prop-4 .statement tag=06H6}

— 令 E、F 为 K 的两个扩张。

a) 设$(L, u, v)$为E和F的复合扩张；那么同态$u * v$的核p到$E \otimes_K F$到L就是一个素理想。

b) 令p为$E \otimes_K F$的素理想；则存在 E 和 F 的复合扩张 $(L, u, v)$，使得 p 是 $u * v$ 的核，并且任意两个这样的复合扩张是同构的。

断言 a) 从环到域的同态到核是素理想（I，p. 116-117）这一事实得出。

令 p 为 A 的 $E \otimes_K F$、A 商环 $(E \otimes_K F)/p$ 和分数的 L 域。对于$x \in E$（或$y \in F$），我们用$u(x)$（或$v(y)$）表示剩余类类 mod p $x \otimes 1$（或 $1 \otimes y$）。那么$u$（分别$v$）是E（分别F）到L和$u(E) \cup v(F)$生成A的K同态为环，因此L为域。因此$(L, u, v)$是E和F的复合扩张；我们立即看到$u * v$是$E \otimes_K F$到L的典范同态，因此它的核等于p。

令$(L', u', v')$为E和F的复合扩张，使得$u' * v'$的核等于p。由于$u * v$和$u' * v'$具有相同的核，因此在$u' * v'$的像$A'$上存在A的同构$\psi$，其特征为$u' * v' = \psi \circ (u * v)$。但$A'$是$u'(E) \cup v'(F)$生成的$L'$的子环，因此L'是A'的分数的域。因此，L的$\psi$扩展到同态$\varphi$到L'，并且显然$\varphi$是$(L, u, v)$到$(L', u', v')$的同构。

#### 注 {#alg-v-s2-n4-rem-1 .statement tag=06H7}

— 如果$p$和$p'$是$E \otimes_K F$的两个不同的素理想，相应的*$E$和$F$的复合扩张*（通过上述证明的过程构造）不是同构的。然而，它们仍然可以同构为 K 的 *扩张*（*V*，p. 146，例 2）。

#### 推论{#alg-v-s2-n4-cor-1 .statement tag=06H8}

*存在E和F*的复合扩张。

因为由于交换环$E \otimes_K F$没有减少到0，所以它有素理想：克鲁尔的定理（*I*，p. 104）证明了极大理想的存在，并且每个极大理想都是素数。

我们可以如下使这个推论更加精确。令$(E, u)$和$(F, v)$为K的两个扩张； 选择交换环 $E \otimes_K F$ 的最大理想 m 并放入 $L = (E \otimes_K F)/m$；那么L是K的扩张。对于$x \in E$，将$x \otimes 1$ mod m的剩余类类写成$u'(x)$，同样将剩余类类写成$v'(y)$ $1 \otimes y$ mod $m$ 适用于所有 $y \in F$。然后我们有一个可交换的图表域同态

$$
\begin{array}{ccc}
F & \xrightarrow{v'} & L \\
| & & | \\
K & \xrightarrow{u} & E .
\end{array}
$$

通过替换$(L, u')$通过E的同构扩张，我们可以假设L包含E为子域并且$u'$是E在L中的典范嵌入。通过改变记号，我们得到以下 scholium ：

#### 学院{#alg-v-s2-n4-sch-1 .statement tag=06H9}

*设K和E为K到E的两个域和u同态。如果K'为域包含K为子域，则存在域E'包含E为子域且将 K' 的同态 u' 转化为 E'，延伸 u*'。

### 5.线性不相交的扩张

*在本文中，R 表示域 K* 中的扩张。

设A和B为R的两个子K代数。存在代数同态$\varphi : A \otimes_K B \to R$其中映射$x \otimes y$到$xy$。 $\varphi$的像是由A U B生成的$\Omega$的子环C。此外，由II，p. 256，如果$(b_\mu)$是B在K上的基和$(a_\lambda)$ A 的基超过 K，然后 C 重合与线性组合 $\sum_{\mu} \alpha_{\mu} b_{\mu}$ 的集合其中 $\alpha_{\mu} \in A$，所有 $\sum_{\lambda} \beta_{\lambda} a_{\lambda}$ 的集合其中 $\beta_{\lambda} \in B$ 以及所有 $\sum_{\lambda,\mu} \gamma_{\lambda\mu} a_{\lambda} b_{\mu}$ 中的集合，其中 $\gamma_{\lambda\mu} \in K$。

如果$\varphi$是$A \otimes_K B$到C的*同构*，我们可以说A和B在*K上*线性不相交的。然后我们有 $A \cap B = K$； B（分别 A）关于 K 的每个自由子集对于 A（分别 B）都是自由的；相反，对于 A 和 B 在 K 上线性不相交的，只要存在 B 在 K 上的*一个* 基（对于例）就足够了，它相对于 A 是自由的（II、p. 256 和 III、p. 469）。

特别考虑 A 和 B 是 $\Omega$ 的*子扩展*的情况。

#### 命题 5 {#alg-v-s2-prop-5 .statement tag=06HA}

*设E和F是$\Omega$中包含的K的两个扩张。*

*a)* *如果F在K上有有限次数，则$E \cup F$生成的$\Omega$的子环是域，与$E(F)$重合，并且$E(F)$在E上的次数是有限的；我们有* $[E(F):E] \leq [F:K]$，*与等式当且仅当E和F在K上线性不相交的。在这种情况下，$E(F)$是E-*同构的*到$E \otimes_K F$。*

*b)* *如果进一步 E 在 K 上为有限次数，则 $E(F) = K(E \cup F)$ 在 K 上为有限次数。我们有* $[K(E \cup F):K] \leq [E:K][F:K]$ *与等式当且仅当 E 和 F 在 K 上线性为不相交的。*

令C为由$E \cup F$生成的$\Omega$的子环；如果$(b_j)_{1 \leq j \leq n}$是F在K上的基，则C是由$b_j$生成的$\Omega$的向量子E空间，因此C是*有限*秩$\leq n$的代数 E;由于环C包含在域中，因此它是整环，因此是*域*，由Cor。至提案 1 (V、p. 10)、从而 $C = E(F)$ 和 $[E(F):E] \leq [F:K]$。 关系 $[E(F):E] = [F:K]$ 表示 $b_j$ 与 E 线性无关，因此 E 和 F 与 K 线性不相交的；这证明了命题的部分 *a)*。 部分 *b)* 现在立即跟随，因为 $[E(F):K] = [E(F):E][E:K]$。

设E和F为$\Omega$中包含的K的扩张；如果 E 和 F 在 K 上具有无限次，子环 $C = K[E \cup F]$ 不一定是域 $^1$；然而C的分数*的*域然后是重合和$K(E \cup F)$。更一般地，令A为E的子环，使得E为A的分数的域，并令B为F的子环，使得F为B的分数的域；那么如果C是$A \cup B$生成的$\Omega$的子环，$K(E \cup F)$重合和C的分数*的*域，因为后者域是最小的$\Omega$ 包含于 C 的子域以及包含 E 和 F。 此外：

#### 命题 6 {#alg-v-s2-prop-6 .statement tag=06HB}

*设E和F为$\Omega$中包含的K的两个扩张，A和B在K上的$\Omega$的两个子代数，使得E为A的分数的域和B的分数的域。则对于E和F要在 K 上线性不相交的，A 和 B 在 K 上线性不相交的是必要且充分的。*

条件显然是必要的。相反，如果 A 和 B 在 K 上线性不相交的，A 和 F 也是如此，因为如果 $\Omega$ 的元素族对于 B 是自由的，那么它对于 B 的分数 F 的域也是自由的（II，p. 315，Cor. 1）和p. 316，Cor.3）；现在，相同的论证表明 E 和 F 在 K 上呈线性不相交的。

$^1$ 对于例，只需考虑两个不定数X 以及Y 和$E = K(X), F = K(Y)$ 中$\Omega$ 是有理分式的域 $K(X, Y)$ 的情况就足够了。

#### 命题 7 {#alg-v-s2-prop-7 .statement tag=06HC}

— 令 E 和 F 为 $\Omega$ 中包含的 K 的两个扩张；如果 E 和 F 在 K 上线性不相交的，则 E 的每个子扩展和 F 的每个子扩展在 K 上线性不相交的。相反，如果对于 E 和 F 的每个对有限生成的子扩展 E'、F' 分别，E' 和 F' 在 K 上线性不相交的，则 E 和 F 在 K 上线性不相交的不相交的超过 K。

对于 E 和 F 的条件在 K 上线性不相交的可以表示如下：如果 $(a_\alpha)$ 是 E 中的自由族并且 $(b_\beta)$ 是 F 中的自由族，则关系 $\sum_{\alpha,\beta} \lambda_{\alpha\beta} a_\alpha b_\beta = 0$，其中 $\lambda_{\alpha\beta} \in K$ 意味着每个$\lambda_{\alpha\beta} = 0$ 对后缀。但是，如果对于每个对个有限自由族都成立，那么这个条件对于每个对个自由族都满足。

因此，直观地说，我们可以说线性析取是有限特征标的性质 «。

#### 命题 8 {#alg-v-s2-prop-8 .statement tag=06HD}

— 令 E、F、G 为 $\Omega$ 中包含的域 K 中的三个扩张，使得 $F \subset G$。为了使 E 和 G 在 K 上线性不相交的，E 和 F 在 K 上线性不相交的以及 E(F) 和 G 在 F 上线性不相交的是充分必要的。

$$
\begin{array}{ccccc}
E & \longrightarrow & E(F) \\
K & \longrightarrow & F & \longrightarrow & G.
\end{array}
$$

图 2.

条件是必要的：假设 E 和 G 在 K 上线性不相交的。E 和 F 也同样成立（命题 7）；另一方面，如果 B 是 E 除以 K 的基，则这也是代数 F[E] 除 F 的基；因为 B 在 G 上自由假设，所以 F[E] 和 G 在 F 上线性不相交的，根据命题 6，$E(F) = F(E)$ 和 G 也是如此。

条件是足够的：同样的记号意味着 B 在 F 上是自由的，因此它是 F[E] 在 F 上的基；由于 F[E] 和 G 在 F 上通过假设线性不相交的，B 在 G 上自由，这表明 E 和 G 在 K 上线性不相交的。

### 习题{#alg-v-s2-exercises}

§ 2](exercises/s2/)参见[习题。
