---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 4
section_title: Algebraically closed extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.19-A V.24, A V.150
pdf_pages: 0133-0138, 0264-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically closed fields
      page: 19
      pdf_page: 133
    - "no": 2
      title: Splitting extensions
      page: 21
      pdf_page: 135
    - "no": 3
      title: Algebraic closure of a field
      page: 22
      pdf_page: 136
statements: 20
exercises: 2
content_sha256: bdc1b996ee27a915cfc1a6e69c5a70eedf4c660b72c89a22d36c2523789c02f5
translated_from: content/en/alg/V/04_s4_algebraically_closed_extensions.md
translation_method: google
source_content_sha256: 532bb2954789915d393a9084c98ffe495892d82e18cded4cc49d55be2b67ab31
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0fc7f175dd7ae05d51a7afad98b1e17be697247fc93ff2f4effbbea9bc29a5ff
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 代数闭扩张

### 1.代数闭域

#### 命题 1 {#alg-v-s4-prop-1 .statement tag=06ID}

— 设 K 为域；那么以下属性是等价的：
(AC) 将 K[X] 中的 K[X] 分裂的的每个非常数多项式转化为次数 1 多项式的乘积（不同或不同）。
(AC') K[X] 的每个非常数多项式在 K 中至少有一个根。
(AC'') K[X] 中的每个不可约多项式都是次数 1。

(AC) K 的每个代数扩张都是次数 1（在其他字中，K 在 K 的每个扩张域中是相对代数封闭的）。

让我们首先证明属性 (AC)、(AC') 和 (AC'') 的等价。显然（AC）意味着（AC）。由于 K[X] 的每个非常数多项式都可以被不可约多项式（IV、p. 13，命题 13）整除，并且 K[X] 中的每个次数 1 多项式明确承认 K 中存在根，因此我们看到 (AC) 蕴涵 (AC')。 条件 (AC') 通过 n 上的归纳暗示，K[X] 中次数 n 的每个多项式都是次数 1 (IV, p. 14，命题 1) 的 n 个多项式中的乘积，因此 (AC') 暗示 (AC)。

仍有待观察的是 (AC) 和 (AC) 是等价的。如果(AC'')成立，则K上的代数K的扩张域L的每个元素都是次数1(V，p. 16，Th.1)，因此属于为K，成立(AC)。反之，令f为K[X]中次数$n \geq 1$的不可约多项式；商代数 K[X]/(f) 是 K 上的次数 n 并且是域，因此 K 的次数 n 的代数扩张（V，p. 18，命题 2）。现在很清楚，(AC) 意味着(AC'')。

#### 定义 1 {#alg-v-s4-def-1 .statement tag=06IE}

如果域 K 具有（等价）性质 (AC)、(AC')、(AC)、(AC)，则称其为代数封闭。

\* 例 1. — 复数的域 C 是代数封闭的（Gen. Top.、VIII、p. 100）。 \*

K 的扩张域 E 中相对代数封闭的域 K 不一定是代数封闭的（实际上，每个域本身都是相对代数封闭的，并且存在域不是代数封闭的，对于例 Q 或 $\mathbf{F}_p$ \* 或 R *）。然而：

#### 命题 2 {#alg-v-s4-prop-2 .statement tag=06IF}

设 $\Omega$ 为代数闭域，K 子域为 $\Omega$。那么$\Omega$中K的相对代数闭包$\bar{K}$就是代数闭域。

令 f 为 $\bar{K}[X] \subset \Omega[X]$ 中的非常数多项式。由于$\Omega$是代数闭的，所以多项式f在$\Omega$中至少有一个根，并且由于这个根是$\bar{K}$上的代数，所以它属于到$\bar{K}$（V，p. 19，命题4）。因此$\bar{K}$满足(AC')。

\* 例 2. — 根据命题 2，所有在 Q 上代数的复数（通常称为简单代数数）的集合是代数闭域。 \*

#### 命题 3 {#alg-v-s4-prop-3 .statement tag=06IG}

每个代数闭域都是无限的。

令 K 为有限域并放入 $f(X) = 1 + \prod_{a \in K} (X - a)$。多项式 $f \in K[X]$ 是非常数，而 $f(a) = 1$ 对于每个 $a \in K$ 都是非常数。所以域 K 不满足 (AC')，因此不是代数封闭的。

#### 定理 1（斯坦尼茨）{#alg-v-s4-thm-1 .statement tag=06IH}

令 K 为域，E 为 K 的代数扩张和 K 的 $\Omega$ 代数闭扩张；则存在 E 到 R 的 K 同态。

由V，p. 13，Scholium，存在$\Omega$的扩张域$\Omega'$以及E到$\Omega'$的K同态u。设 $x \in E$；因为 x 是 K 上的代数，所以 u(x) 是 u(K) 上的代数，并且 *更不必说* 是 $\Omega$ 上的代数（V，p. 17，Cor. 2）；由于 $\Omega$ 是代数封闭的，因此我们有 $u(x) \in O$。由此可见，$u$映射$E$变为$O$。

### 2.分裂扩张

#### 定义 2 {#alg-v-s4-def-2 .statement tag=06II}

*设 K 为域和 $(f_i)_{i \in I}$ $K[X]$ 中的非常数多项式族。通过$(f_i)_i$的分裂扩张，我们可以理解$K$的任何扩张$E$具有以下属性：*

*a) 对于每个$i \in I$，将$E[X]$中的多项式$f_i$分裂的转化为次数1多项式的乘积。*

*b) 对于每个$i \in I$，令$R_i$为$E$中$f_i$的根中的集合，然后$E = K \left( \bigcup_{i \in I} R_i \right)$。*

使用有时项 « 分裂域 » 代替 « 分裂扩张 »。

#### 注 {#alg-v-s4-n2-rem-1 .statement tag=0EEN}

*1) 对于每个$i \in I$，令$c_i$为$K$的非零元素，并令$f'_i = c_i f_i$。那么很明显，对于家庭$(f_i)_i$来说，每个分裂扩张对于家庭$(f'_i)_{i \in I}$来说也是分裂扩张，反之亦然。特别是，在研究分裂扩张时，我们可以将极限应用于一元多项式的情况。*

*2) 假设I是有限的，并放入$f = \prod_{i \in I} f_i$。将多项式分解的唯一性转化为 $E[X]$ 中的不可约因子（IV、p. 13、命题 13），我们可以轻松证明多项式 $f$ 的分裂扩张为分裂扩张为家庭$(f_i)_i$，反之亦然。在其他字中，有限族的情况可以简化为单个多项式的情况。*

*3) 令$f \in K[X]$为次数$\geq 1$的多项式，令$E$为$f$的分裂扩张。如果$x_1, \ldots, x_n$在$E$中关闭根，则我们有$E = K(x_1, \ldots, x_n)$并且$[E : K]$是有限的（$V$，p. 18，Th.2）；但也有可能 $E$ 与单个根生成的子域 $K(x_1), \ldots, K(x_n)$ 不同；即使 $f$ 不可约$^1$，这种情况也可能发生。然而，我们注，当$f$不可约时，域$K(x_i)$在$K$上都具有相同的次数$n$，并且每当$E$等于其中之一时，我们就有$[E : K] = n$，因此$E = K(x_1) = \cdots = K(x_n)$.*

#### 命题 4 {#alg-v-s4-prop-4 .statement tag=06IJ}

*设K为域和$(f_i)_{i \in I}$$K[X]$中的非常数多项式族；那么家庭$(f_i)_{i \in I}$就存在分裂扩张。*

我们可以将多项式 $f_i$ 视为多项式 (注 1)。设$i \in I$，并令$f_i$的次数为$d_i$。根据IV，p. 73，命题5，存在交换代数$A$，超过$K$，不减少到0，以及$A_i$的元素$\xi_{i,1}, \ldots, \xi_{i,d_i}$，这样：

*a) 代数 $A_i$ 由$(\xi_{i,1}, \ldots, \xi_{i,d_i})$生成；*

(1) 取例$K = \mathbf{Q}$和$f = X^3 - 2$。

b) 我们在$A_i[X]$中有$f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k})$。

设$A$为代数$(A_i)_{i \in I}$家族的张量积，并令$\varphi_i$为$A_i$的典范同态进入$A$（III，p. 470）。 代数 $A$ 则可交换且不减至 0；根据克鲁尔的定理（I，p. 104），因此在$A$中存在最大理想$a$，而$E = A/a$是域$K$的扩张。

将$A$的$\psi$典范同态代入$E$，并将$x_{i,k} = \psi(\varphi_i(\xi_{i,k}))$代入$i \in I$和$l \leq k \leq d_i$。由于代数$A$是由$\bigcup \varphi_i(A_i)$生成的，扩张$E$是由$(x_{i,k})$家族生成的。此外，我们还有$i \in I$

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ in } E[X]. $$

因此$E$是家庭$(f_i)_{i \in I}$的分裂扩张。

#### 命题 5 {#alg-v-s4-prop-5 .statement tag=06IK}

— *令 K 为$K[X]$、K 的 E 扩张中的域、$(f_i)_{i \in I}$ 非常数多项式族，以及 E 的 F、F' 子扩展，其中每个都是 $(f_i)_{i \in I}$ 的分裂扩张。然后$F = F'$。

令$R_i$为E中$f_i$的根和$R = \bigcup_{i \in I} R_i$的集合。由于$f_i$是$F[X]$中第一个次数的多项式的乘积，因此我们有$R_i \subset F$。由Def。 2、我们有$F = K(R)$；同理我们发现$F = K(R)$。

#### 推论 {#alg-v-s4-n2-cor-1 .statement tag=06IL}

— *设 K 为域、$(f_i)_{i \in I}$，$K[X]$ 中的非常数多项式族，以及 $(f_i)_{i \in I}$ 的 F、F' 分裂扩张。那么存在 F 到 F 的 K 同构的。

这是根据第 5 号提案和 V、p. 13、Cor. 得出的。提案 4。

### 3. 代数闭包 / 域

#### 定义 3 {#alg-v-s4-def-3 .statement tag=06IM}

— *令 K 为域。通过 K 的代数闭包，我们可以理解 K 的任何扩张，它是代数和代数闭的。

#### 例 1 {#alg-v-s4-n3-exa-1 .statement tag=06IN}

复数域C为实数域代数闭包R（Gen.Top.、VIII、p. 100）\*

#### 例 2 {#alg-v-s4-n3-exa-2 .statement tag=06IO}

令K为K的域和$\Omega$代数闭扩张。如果$\overline{K}$是K在$\Omega$中的相对代数闭包，则根据V，p. 20，命题2，K是K的代数闭包。\*特别地，所有代数数（V，p. 20，例2）的域是有理数的域Q的代数闭包。 \*

#### 命题 6 {#alg-v-s4-prop-6 .statement tag=06IP}

— *令 $\Omega$ 为域 K 的扩张。对于 $\Omega$ 为 K 的代数闭包，它应该是代数的，并且 $K[X]$ 中的每个非常数多项式都应将 $\Omega[X]$ 中的分裂的化为乘积因子次数 1。

(AC) 需要条件。相反，假设$\Omega$是$K$上的代数，并且$K[X]$上的每个非常数多项式是次数1的因子的$\Omega[X]$中的乘积。令$\Omega'$是一个代数扩张的 $\Omega$ 并让 $x \in \Omega'$。由于$x$是$\Omega$上的代数，$\Omega$是$K$上的代数，$x$是$K$上的代数（V，p. 19，命题3）。令 $f$ 为 $x$ 在 $K$ 上的最小多项式。将$\Omega[X]$中的假设多项式$f \in K[X]$分裂的代入次数1、从而$x \in \Omega$的因子乘积。因此我们有 $\Omega' = \Omega$ 并且 $\Omega$ 是代数封闭的，因为它满足 (AC)。

#### 注 1 {#alg-v-s4-n3-rem-1 .statement tag=06IQ}

如果 $\Omega$ 是 $K$ 上的代数，并且 $K[X]$ 的每个非常数多项式在 $\Omega$ 中都有根，则 $\Omega$ 是 $K$ 的代数闭包 (V， p. 156，例如 20)。

#### 命题 7 {#alg-v-s4-prop-7 .statement tag=06IR}

— *令$\Omega$为域$K$的代数扩张。
a) 如果 $\Omega$ 是代数闭集，则 $K$ 的每个代数扩张同构于 $\mathbf{R}$ 的子扩张。
b) 相反地假设$K$的有限次数的每个代数扩张同构于$\Omega$的子扩张；那么 $\Omega$ 是代数闭的。*

断言 *a)* 由 Th 得出。 1（V，p. 20）。现在假设 *b)* 的假设并考虑一个非常数多项式 $f \in K[X]$。设E为$f$的分裂域（V，p. 21，命题4）；由于E是有限次数在$K$上的代数（V，p. 18，Th.2），我们可以假设E是$\Omega$的子扩展。那么多项式$f$就是$\Omega[X]$中次数1的多项式的乘积，并且第6命题表明$\Omega$是代数封闭的。

现在我们可以证明代数闭包和域的存在性和唯一性（直到同构）。

#### 定理 2（斯坦尼茨）{#alg-v-s4-thm-2 .statement tag=06IS}

— *令$K$为域；那么存在$K$的代数闭包。如果$\Omega$和$\Omega'$是$K$的两个代数闭包，则存在$\Omega$到$\Omega'$的$K$同构。*

根据第 6 条，$K$ 的代数闭包只不过是 $K[X]$ 中所有非常数多项式的集合的分裂扩张。 Th。因此，2 是从第 4 号提案V、p. 21 和 Cor. V、p. 22 得出的。

#### 推论{#alg-v-s4-n3-cor-1 .statement tag=06IT}

— *令$K$和$K'$为域、$K$的$\Omega$代数闭包和$K'$的$\Omega'$代数闭包。对于$K$到$K'$的每个同构$u$，都存在$\Omega$到$\Omega'$延伸$u$的同构$v$。*

应用Th就足够了。 2至代数闭包$\Omega$和$(\Omega', u)$$K$。

#### 注 2 {#alg-v-s4-n3-rem-2 .statement tag=06IU}

在前述推论的记号中，一般存在不同于恒等式的$K$-自同构$\Omega$。因此，一般不存在$\Omega$的唯一性约同构$v$到$\Omega'$延伸$K$的同构$u$到$K'$。出于类似的原因，对于同一个多项式族$(f_i)_{i \in I}$，通常在分裂扩张$E'$上存在分裂扩张$E$中的多个同构。相比之下，我们记得，对于完美的闭合，我们有唯一性（V，p. 5）。

#### 注 3 {#alg-v-s4-n3-rem-3 .statement tag=06IV}

令 K 为域和 $\Omega$ 代数闭包 of $K$。那么对于$K[X]$中的非常数多项式族$(f_i)_{i \in I}$，对于分裂扩张，可以给出以下构造：令$R_i$为$f_i$的根的集合 $\Omega$，让$R = \bigcup_{i \in I} R_i$。那么$K(R)$是$\Omega$的唯一子扩展，它是$(f_i)_{i \in I}$的分裂扩张（V，p. 22，第5条）。

#### 注 4 {#alg-v-s4-n3-rem-4 .statement tag=06IW}

设 K 为 $K$ 的有限域和 $\Omega$ 代数闭包。那么 $\Omega$ 是无限的（$V,$ p. 20，命题 3）；由于 K 的有限次数的每个扩张都是有限域，因此 $\Omega$ 是 $K$ 的*无限* 次数的代数扩张。

### 习题 {#alg-v-s4-exercises}

§ 4](exercises/s4/)参见[习题。
